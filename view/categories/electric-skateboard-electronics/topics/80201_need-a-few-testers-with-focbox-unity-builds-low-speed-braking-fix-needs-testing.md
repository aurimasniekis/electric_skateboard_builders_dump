# NEED A FEW TESTERS WITH FOCBOX UNITY BUILDS - Low-speed Braking Fix Needs Testing

### Replies: 97 Views: 1467

## \#1 Posted by: Deodand Posted at: 2019-01-07T18:35:46.694Z Reads: 350

```
Hey guys, poured some hours this weekend into fixing low-speed FOC braking in the unity firmware. This change can easily be applied to any VESC based design as well if/when I confirm it works well without introducing any unforeseen behaviors on different builds. 

Let's start with the TLDR. **Would love it if some experienced people with builds that contain a focbox unity could download and test this FW update.** Bonus points if your build experiences the low-speed braking issue. Should be safe I've ridden like 10-20 miles on my board with this FW rev but maybe take it slow to start. **PLEASE ONLY DO THIS IF YOU ARE FAMILIAR WITH FW UPDATES FOR VESC BASED CONTROLLERS**

[DOWNLOAD LINK FOR FOCBOX UNITY TEST FW](https://drive.google.com/open?id=1KoP-eeQurP8rBsdcTPd1vyXQ6decOJDR)

Now for the details. For context this is a thread discussing the issue: 

[quote="thisguyhere, post:1, topic:73547"]
with the unity under active development, i thought we could persuade @Deodand to finally address the locking brakes issue for larger diameter wheels in FOC.
[/quote]

Maybe slightly wrong to start new topic but I need testers and want to make sure this wasn't a post buried in a thread. I tried tons of different stuff and what ended up fixing the issue is the following snippet (this is how it is currently) : 

    // When the filtered duty cycle in sensorless mode becomes low in brake mode, the
    // observer has lost tracking. Use duty cycle control with the lowest duty cycle
    // to get as smooth braking as possible.
    if (m_control_mode == CONTROL_MODE_CURRENT_BRAKE
    		&& fabsf(duty_filtered) < 0.03) {
    	control_duty = true;
    	duty_set = 0.0;
    }

And changed it to:

    if (m_control_mode == CONTROL_MODE_CURRENT_BRAKE
            && fabsf(duty_filtered)*GET_INPUT_VOLTAGE() < 0.5
            && (fmax( m_iq_set , 0.5/m_conf->foc_motor_r ) >  (double) fabsf(m_motor_state.iq_filter))) {
          control_duty = true;
          duty_set = 0.0;
        }

Essentially before, anytime your board dropped to 3% of the maximum voltage (AKA  you were going 3% of max speed)  while braking the motor controller would short all leads together. This is necessary because brakes should always oppose motion and at very low speed even a sensored motor only has a good sense of speed and not of its velocity. Thus the sign of the velocity might change rapidly and cause the motor to vibrate, so instead by shorting the leads of the motor we guarantee a viscous damping force. Problem is the 3% duty cycle means different things for different setups. Imagine a build running 12V and 0.1 ohm winding resistance for the sake of example. At 3% duty cycle shorting the motor leads induces a current of 

    0.03*12V/(2/3*0.1ohm) = 5.4 Amps

This is probably not going to result in much braking force. Now imagine a build running 50V and 20 mOhm winding resistance (probably a high kv motor 6374 or bigger) 

    0.03*50V/(2/3*0.02ohm) = 112 Amps

This is an extreme example but 112 amps is likely to throw lots of people from their boards. So the first change I made was to remove the dependence of source voltage on the switch-over to duty-cycle control. Instead of 3% duty cycle we instead switch over at  0.5V (duty cycle*source voltage). This is acceptable because the voltage resolution of ADC doesn't change with different source voltages (fixed resistor voltage dividers for this measurement) so if 3% duty cycle works at 12V then that voltage should work for any source voltage. Here is the part of the if statement that handles that:

    fabsf(duty_filtered)*GET_INPUT_VOLTAGE() < 0.5

The second change I made is a bit trickier, this is to fix the brakes "sticking" so to speak. Once you enter this low speed mode the duty is commanded to zero and you never stop shorting the motor leads until you either exceed the maximum motor amps or you release the brake fully. Mainly this is noticeable on steep downhills, hold in your brakes till you come to a complete stop then feather off most of the way but not all. You will realize your board is locked in with very strong braking force regardless of how you feather the throttle. This was a bit trickier to make an exit condition for. Essentially you don't want to exit if either the current commanded motor amps are less than the induced amps **OR** if your current phase voltage would be too low to brake properly. Trouble is we have commanded the phase voltage to zero, so instead we have to figure out what the phase voltage *would* be if we weren't shorting the leads. This can be done since we know the amps flowing and the winding resistance. Note that I compute it with a bit of added cushion to try and introduce a bit of hysteresis to prevent rapid mode switching or inaccuracies due to changing winding resistance. This is the part of the if statement that computes this: 

    fmax( m_iq_set , 0.5/m_conf->foc_motor_r ) >  (double) fabsf(m_motor_state.iq_filter)
```

---
## \#2 Posted by: Indiangummy Posted at: 2019-01-07T18:40:17.112Z Reads: 286

```
I can give it a go when I get home today. But what diameter wheels is this proplem most forseen with? @thisguyhere  I have 107mm's and a gear drive and haven't had any problems with braking.
```

---
## \#3 Posted by: Deodand Posted at: 2019-01-07T18:41:32.710Z Reads: 281

```
For most setups it's mainly just a nuisance. Before you update play around a bit with very low speed and soft braking. Notice the stiff ramp up in braking force right before you stop. With some setups it isn't noticeable much at all on others it's extremely obvious.
```

---
## \#4 Posted by: evoheyax Posted at: 2019-01-07T18:51:49.553Z Reads: 277

```
I've noticed this with my hummie hubs since forever, lol. That last 2 or 3 mph, the brake force is super strong, throw off strong. But great at any other speed. I first noticed this 3 years ago with the 4.12 and every vesc since then.
```

---
## \#5 Posted by: Deodand Posted at: 2019-01-07T18:57:24.138Z Reads: 259

```
It's one of those things you can overlook, but why not just fix it.
```

---
## \#6 Posted by: thisguyhere Posted at: 2019-01-07T18:58:07.201Z Reads: 246

```
107mm wasn't an issue, the 160mm psycho sixshooters is when it happens for me.

i'll test the unity as soon as i get all my battery orders out the door, hopefully in the next week or so.
```

---
## \#7 Posted by: Indiangummy Posted at: 2019-01-07T18:59:15.967Z Reads: 226

```
Alirght, would love to help but don't see how as i don't have a problem with my setup.
```

---
## \#8 Posted by: Deodand Posted at: 2019-01-07T19:00:30.850Z Reads: 227

```
If you can just flash the firmware and confirm that everything continues to work as expected that is also helpful :smile: but don't feel obligated.
```

---
## \#9 Posted by: Indiangummy Posted at: 2019-01-07T19:04:33.112Z Reads: 222

```
Ok yeah I could do that. Will update you.
```

---
## \#10 Posted by: briman05 Posted at: 2019-01-07T19:11:35.794Z Reads: 218

```
Do it for Science but maybe wear extra padding as a just in case
```

---
## \#11 Posted by: Indiangummy Posted at: 2019-01-07T19:13:03.498Z Reads: 219

```
I got it covered 
https://giphy.com/gifs/little-giants-KkaCYAbceftwA?utm_source=media-link&utm_medium=landing&utm_campaign=Media%20Links&utm_term=https://giphy.com/gifs/little-giants-KkaCYAbceftwA
```

---
## \#12 Posted by: ShutterShock Posted at: 2019-01-07T19:37:05.303Z Reads: 209

```
I don't have a FOCBOX unity but I am running two normal FOCBOX's with this issue.  Like @evoheyax said it is extreemely strong last 2-3 mph.  Makes sense to equal out to about 2-3% of the voltage.  I only run 90mm wheels.
```

---
## \#13 Posted by: Deodand Posted at: 2019-01-07T19:41:21.670Z Reads: 207

```
Yeah the change for regular focbox is identical just needs to be compiled. Wanna make sure this works for people.
```

---
## \#14 Posted by: evoheyax Posted at: 2019-01-07T19:41:55.021Z Reads: 204

```
Great to hear, now that I'm running 4 focboxes! Can't wait to try it out!
```

---
## \#15 Posted by: ShutterShock Posted at: 2019-01-07T19:45:20.048Z Reads: 202

```
From what I read tho basically you were saying even if you feather off the brake {in your fixed version} it will still have the same amount of brake force?  Or were you explaining the problem version?

[quote="Deodand, post:1, topic:80201"]
You will realize your board is locked in with very strong braking force regardless of how you feather the throttle. This was a bit trickier to make an exit condition for.
[/quote]


Was I reading this wrong?  I feel like as you feather off the brake, you would want the brake force to decrease gradually, like it normally does?
```

---
## \#16 Posted by: Deodand Posted at: 2019-01-07T20:01:56.114Z Reads: 193

```
Yeah the brake force should now release as expected. Previously it did not. Sorry if that was ambiguous.
```

---
## \#17 Posted by: ShutterShock Posted at: 2019-01-07T20:08:45.292Z Reads: 191

```
Okay good haha, no that is probably my misreading
```

---
## \#18 Posted by: AlexBE Posted at: 2019-01-07T22:34:35.055Z Reads: 184

```
I would love to test this, but with my gearing and wheels the braking is completely smooth :frowning:
```

---
## \#19 Posted by: skatardude10 Posted at: 2019-01-08T00:45:46.049Z Reads: 180

```
Yes! I can't wait to test this (dual focbox, no unity) when these get compiled for other vescs. 

I'm even considering forking acks fw and making the changes myself until this gets pushed elsewhere by someone else... Hmmmmm.... 

Anyways thanks @Deodand for putting in the work to get this fixed!
```

---
## \#20 Posted by: Indiangummy Posted at: 2019-01-08T05:37:59.669Z Reads: 173

```
a bit of update @thisguyhere @Deodand i actually realized that i do have this problem. i just never noticed it because i jumped off the board for the last few mph so it was never a concern for me. i got home late today but im getting the firmware on the unity now and i'l test tomorrow.  what motor and brake settings do you recommend to test it @Deodand?
```

---
## \#21 Posted by: Blasto Posted at: 2019-01-08T06:20:32.033Z Reads: 159

```
I’d say take note of your current settings and use the same ones so you can compare the feeling
```

---
## \#22 Posted by: Indiangummy Posted at: 2019-01-08T06:23:36.886Z Reads: 154

```
allright, yeah i'l try the same settings then. thanks.
```

---
## \#23 Posted by: dougpage Posted at: 2019-01-08T16:13:29.917Z Reads: 147

```
I can also test this when I get home. My hummies are considered small diameter but I have noticed this.
```

---
## \#24 Posted by: Indiangummy Posted at: 2019-01-08T20:30:04.046Z Reads: 142

```
@Deodand yup that fw fixed it. Completely smooth braking down to 0 mph. im uploading a video now. Nice Work!
```

---
## \#25 Posted by: Indiangummy Posted at: 2019-01-08T20:39:34.136Z Reads: 141

```
https://youtu.be/jzMezNXdkR4
```

---
## \#26 Posted by: thisguyhere Posted at: 2019-01-08T20:44:36.840Z Reads: 141

```
looks like 97mm wheels?

i have no braking issues on foc up to 107mm wheels but can't wait to try it regardless.
```

---
## \#27 Posted by: Indiangummy Posted at: 2019-01-08T20:46:33.864Z Reads: 141

```
107mm wheels. i did have braking issues before this. i just always jumped of the board for the last few mph. it was never this smooth. and yeah someone else should try it to confirm.
```

---
## \#28 Posted by: Indiangummy Posted at: 2019-01-08T20:47:41.380Z Reads: 138

```
i can revert my firmware to do a before and after. but id have to crack open the enclosure again.
```

---
## \#29 Posted by: thisguyhere Posted at: 2019-01-08T20:49:58.854Z Reads: 137

```
i think that's still a very good sign.  @Deodand may have done it again.
```

---
## \#30 Posted by: lrdesigns Posted at: 2019-01-09T00:50:07.440Z Reads: 135

```
@Deodand this is exciting development work. :grinning:

I just want to reiterate that I get this issue in BLDC too, so I am wondering if the code pieces your modifying are **exclusivley** used during FOC? 

If not maybe there is a similar code issue under BLDC mode?

Id love to help test but I dont have a unity. 

Keep up the good work. :ok_hand:
```

---
## \#31 Posted by: kalebludlow Posted at: 2019-01-09T00:51:58.875Z Reads: 127

```
Never heard of this being an issue in BLDC, are you using sensored or unsensored?
```

---
## \#32 Posted by: lrdesigns Posted at: 2019-01-09T00:56:01.777Z Reads: 122

```
Sensored. 5065 dual 140kv, 2:1 gearing, 12s lipo, 97mm wheels with 4.12 maytech vescs. 

I was able to get rid of the problem with the old firmware that had an option to reduce the max brake eprm number. But that option is missing in the newer firmwares.
```

---
## \#33 Posted by: Deodand Posted at: 2019-01-09T01:05:16.708Z Reads: 125

```
Yeah this will only fix the issue in FOC. Probably won't spend the time to debug BLDC as my familiarity with the code is lower and FOC is the future :smile:
```

---
## \#34 Posted by: AlexBE Posted at: 2019-01-09T01:15:15.993Z Reads: 130

```
I have installed the test firmware on my board, though I didn't notice a problem braking previously. 

* 140kv, 15T->72T -> 200mm diameter wheels. 25A braking.
* much stronger braking at low speed than previously.
* vibration at very low speed as the board comes to a stop. Is it possible that the Unity is oscillating between braking modes. I notice you have added hysteresis, maybe there isn't enough.

I can make a video if you like, anything else you would like me to modify? not sure if the test firmware has a different version number, but I suggest you change version number, could be helpful especially if you need 5 beta revisions tested before official release.
```

---
## \#35 Posted by: Deodand Posted at: 2019-01-09T01:37:09.900Z Reads: 125

```
yeah I didn't iterate firmware version only because it would make the configuration app unable to connect, this will definitely et a bump in rev number. 

There's a small amount of vibration as it hops between modes for me at very low speed but its pretty minor. How severe is it on your board? My guess is I can figure out how to tune it out once I collect some data.

You feel stronger braking at low speed? This is strange. Is it strong in a bad way? Like it unnexpectedly increases or just stays more consistent at low speed?
```

---
## \#36 Posted by: Indiangummy Posted at: 2019-01-09T01:41:09.315Z Reads: 118

```
Yeah I didn't feel any vibrations or stronger braking. Just smoother overall braking.
```

---
## \#37 Posted by: dougpage Posted at: 2019-01-09T02:05:31.186Z Reads: 120

```
I am trying to install the new firmware on the unity and right as it finishes it disconnects and now I am not able to get the motors to spin. I am not sure what I am doing wrong.
```

---
## \#38 Posted by: Indiangummy Posted at: 2019-01-09T02:09:18.359Z Reads: 119

```
Are you getting the invalid serial port error?
```

---
## \#39 Posted by: dougpage Posted at: 2019-01-09T02:11:19.433Z Reads: 120

```
Where would it say that, It connects just fine and when I go to download the firmware it writes it but when it finishes writing it just disconnects
```

---
## \#40 Posted by: Indiangummy Posted at: 2019-01-09T02:12:12.912Z Reads: 122

```
Disconnecting is normal. Look on the bottom right corner when you try to reconnect. See if there is a error.
```

---
## \#41 Posted by: dougpage Posted at: 2019-01-09T02:14:25.028Z Reads: 115

```
No error for me... should I try to rewrite the old firmware?
```

---
## \#42 Posted by: Deodand Posted at: 2019-01-09T02:16:48.801Z Reads: 116

```
What are you using to flash firmware, tool or UI? Are you on USB?
```

---
## \#43 Posted by: dougpage Posted at: 2019-01-09T02:17:39.964Z Reads: 114

```
The focbox UI over the type c connection from my pc
```

---
## \#44 Posted by: Indiangummy Posted at: 2019-01-09T02:18:45.111Z Reads: 118

```
ohhhh I updated via the tool.
```

---
## \#45 Posted by: Deodand Posted at: 2019-01-09T02:19:06.076Z Reads: 117

```
So you flash the firmware and the unit reboots? Should be normal behavior, means flash went successfully I think. What makes you think its not updating?
```

---
## \#46 Posted by: dougpage Posted at: 2019-01-09T02:21:25.515Z Reads: 112

```
When it reconnects it does not work, my remote is connected and when I spin the motor it reads it on the HUD but, it just wont work.
```

---
## \#47 Posted by: Indiangummy Posted at: 2019-01-09T02:22:38.557Z Reads: 113

```
Did you rerun motor detection?
```

---
## \#48 Posted by: dougpage Posted at: 2019-01-09T02:23:02.634Z Reads: 113

```
No but I will now.
```

---
## \#49 Posted by: dougpage Posted at: 2019-01-09T02:24:28.513Z Reads: 111

```
Nope still not working.
```

---
## \#50 Posted by: Indiangummy Posted at: 2019-01-09T02:25:10.560Z Reads: 114

```
Hmmm, interesting.
```

---
## \#51 Posted by: Blasto Posted at: 2019-01-09T02:27:32.972Z Reads: 115

```
Go through the whole wizzard, the fw sets the app back to disable. You need to reselect fwd with brake
```

---
## \#52 Posted by: dougpage Posted at: 2019-01-09T02:28:40.893Z Reads: 115

```
I went through the guided setup if that is what you mean.
```

---
## \#53 Posted by: Indiangummy Posted at: 2019-01-09T02:35:22.551Z Reads: 117

```
[quote="Blasto, post:51, topic:80201"]
the fw sets the app back to disable. You need to reselect fwd with brake
[/quote]

yeah double check this. this is what happend to me at first.
```

---
## \#54 Posted by: dougpage Posted at: 2019-01-09T02:38:20.788Z Reads: 114

```
OHHHHHH thank you so much! Ill go outside and test now.
```

---
## \#55 Posted by: AlexBE Posted at: 2019-01-09T03:21:06.484Z Reads: 119

```
Two videos where you can hear the vibration. It's definitely not belt skipping or anything like that. https://photos.app.goo.gl/s5p4nnfNptV4DKnDA

Stronger braking at low speed in a good way. Though I didn't really test immediately back to back with the firmware so that could be my imagination.
```

---
## \#56 Posted by: dougpage Posted at: 2019-01-09T03:51:43.130Z Reads: 126

```
https://www.youtube.com/watch?v=ss6T27BmMPY

Thank you Jeff!
```

---
## \#57 Posted by: skatardude10 Posted at: 2019-01-09T05:09:32.714Z Reads: 125

```
@Deodand  Sorry I jumped the gun, tested fix on my non-unity build. Works great, although you can hear cogging at the *very end* as you will see... sound most evident in second vid:

https://www.youtube.com/watch?v=2S6y-wHaoc0
https://www.youtube.com/watch?v=8YESNxsOV7w

Thank you for this fix!!! 

If anyone else out there is currently running Ackmaniac's 3.102 with standard ( **NON-UNITY** ) 410, 411, 412 vesc hardware, [i've forked ack's FW with the fix applied](https://github.com/skatardude10/bldc) for you to download and build for yourself, currently only forked to make change, but builds locally just fine for those interested.

Alternatively, here's Ackmaniac's FW 3.102 build files with the brake fix applied for vescs other than unity: [Link](https://drive.google.com/drive/folders/1oFsT_JJH-np0c4J39KroElioYzZMl4Wo?usp=sharing)
```

---
## \#58 Posted by: AlexBE Posted at: 2019-01-09T05:25:19.371Z Reads: 123

```
This is exactly the same sound I get in my videos. 

p.s. How the HELL do you accelerate at 160A like that?
```

---
## \#59 Posted by: skatardude10 Posted at: 2019-01-09T05:27:34.267Z Reads: 124

```
It's motor current not battery current :-)

160A battery max... **JEEBERS** I could only imagine...
```

---
## \#60 Posted by: AlexBE Posted at: 2019-01-09T05:29:51.691Z Reads: 125

```
That's what I mean, 160A motor current = a heap of torque. Unless you have a high KV motor I suppose and much higher gearing than me. I can only just get to 30A+30A motor current, that is with 140kV motors geared to 40km/h top speed. (70Kg)
```

---
## \#61 Posted by: skatardude10 Posted at: 2019-01-09T05:30:48.370Z Reads: 122

```
dual 190kv motors with 20/36 gearing on 107mm flywheels, 10S4P 25R, 80A motor max 40A battery max per focbox. I think it's the gearing... i've always geared for speed, so the torque is never anything too crazy.
```

---
## \#62 Posted by: AlexBE Posted at: 2019-01-09T05:35:02.931Z Reads: 117

```
Ahh ok that makes some sense, you have almost twice the gearing (top speed) that I do, giving me double the torque-per-amp.
```

---
## \#63 Posted by: skatardude10 Posted at: 2019-01-09T06:01:35.472Z Reads: 118

```
Not sure if these will be of any use, but here's some data from my vescs.

![Brake%20Fix%20Vesc%20Log1|690x224](upload://yUqqliCyFFG34AG6qpBxeDhI9ny.png) ![Brake%20Fix%20Vesc%20Log2|690x224](upload://3lAULqrlUDXkaA36FctARBMn6We.png)
```

---
## \#64 Posted by: AlexBE Posted at: 2019-01-09T06:13:12.720Z Reads: 114

```
Ooo, how are you getting the data out? I couldn't get ackmaniac to work....
```

---
## \#65 Posted by: skatardude10 Posted at: 2019-01-09T06:19:53.555Z Reads: 117

```
Just to be clear, you _should not_ run Ackmaniac's firmware on the Unity.

I used this fix applied to Ackmaniac's FW on the standard FOCBOX with a bluetooth adapter and ESC Monitor.

Are you running a Unity?


BTW, I watched your videos with the braking sound... same exact thing, you're right!
```

---
## \#66 Posted by: AlexBE Posted at: 2019-01-09T06:25:59.934Z Reads: 112

```
Ahh sorry, my mistake. I meant running Ackmaniac's Android app and getting it to speak via a BT module to the unity. Totally missed that you were testing on VESCs and not a Unity.
```

---
## \#67 Posted by: Deodand Posted at: 2019-01-09T06:40:30.407Z Reads: 111

```
Nice guys, I'll see if I can do anything about the low speed chatter. To be clear, do you find it to be a small nuisance or is it prohibitive to your riding experience in some way?
```

---
## \#68 Posted by: skatardude10 Posted at: 2019-01-09T06:46:06.975Z Reads: 113

```
Personally, a small nuisance on my setup, if that.

Relatively speaking, having the 'chatter' is maybe only 10% worse than what I imagine it would be like if it were not being there at all... but it's 110% better than locking up completely.
```

---
## \#69 Posted by: AlexBE Posted at: 2019-01-09T06:46:25.942Z Reads: 112

```
For me it is a nuisance to the extent that I thought my belt was skipping. I think the sensible assumption though is that these boards are not the worst possible case of it. Any ideas as to what is causing it?
```

---
## \#70 Posted by: skatardude10 Posted at: 2019-01-09T06:49:00.322Z Reads: 109

```
That's a good point... it can sound like a belt skipping. Does it feel like belt skipping when that happens, or do you just get that impression from the sound?

I didn't get that impression personally, from the feel... and I know my belts don't skip, but when they did, it does make a *similar* sound.
```

---
## \#71 Posted by: AlexBE Posted at: 2019-01-09T06:53:53.240Z Reads: 109

```
It sounds and feels like a belt skipping at very high speed, ie fast skips. I know I'm going low speed, and so I know its not a belt skipping. It's also completely repeatable. I bet its a hysteresis problem. Definitely interesting!
```

---
## \#72 Posted by: DAddYE Posted at: 2019-01-09T07:04:34.712Z Reads: 109

```
Thanks sir. I’ll test as soon as the SF weather allows me to do so. Can’t wait!
```

---
## \#73 Posted by: ShutterShock Posted at: 2019-01-09T07:53:38.133Z Reads: 113

```
To be honest I would rather have the brakes lock at 1-2mph than make a sound like that.  I know what that oscillation in these videos feels like because there is one little tiny spot in my brake throttle that I can force it to make that sound and I definitely do not like it hahah

I have not updated to this fix yet :stuck_out_tongue:  still waiting for the bugs to get worked out.  I ride this board every single day :smiley:
```

---
## \#74 Posted by: Bjork3n Posted at: 2019-01-09T09:15:43.850Z Reads: 108

```
How exactly do I apply the fix to the fw?
Using ack 3.102.
Do I need to reinstall the firmware to apply it?
```

---
## \#75 Posted by: Deodand Posted at: 2019-01-09T17:26:17.795Z Reads: 105

```
I'd say there isn't actually much feel to it. It's mostly audible. Basically it's switching between duty cycle control and current control but motor amps are close to identical so the feel is still smooth (on my setup at least) it just sounds chattery.

I think I can find some way to introduce a bit more hysteresis to solve it anyways. But if I can't I still think it feels better on my setup. I'll take a small chatter sound at 1 mph over sticky non-linear brakes any day. Not really too worried though, there should be a fix.
```

---
## \#76 Posted by: ShutterShock Posted at: 2019-01-09T17:53:58.607Z Reads: 105

```
Aight well I will keep watching, maybe I will try it out anyway.  I can always revert if I don't like it :stuck_out_tongue:
```

---
## \#77 Posted by: skatardude10 Posted at: 2019-01-09T20:53:33.450Z Reads: 111

```
[Non-Unity Instructions] TLDR: select bin from the custom file tab under firmware.

Yeah, you need to reinstall the FW to apply it. I'd recommend loading and saving all your motor and app settings to xml prior to the update just incase unless you don't mind setting things up again possibly. Remember to re-apply settings after FW update.

After connecting via ESC Tool, firmware tab, you need to choose the custom file tab and navigate to the VESC Default.bin that you downloaded for your hardware version from my link above- Google drive, not GitHub. 

I didn't update the repo with the recompiled bins, so you can also clone the repo and rebuild the bins locally if you want. The wrong HW version will probably brick your vesc. 

Then click the write button. Once you are reconnected, reapply saved settings you had before. Your low speed FOC brakes should be different now.
```

---
## \#78 Posted by: topcloud Posted at: 2019-01-09T21:24:52.152Z Reads: 103

```
[quote="Deodand, post:75, topic:80201"]
I’ll take a small chatter sound at 1 mph over sticky non-linear brakes any day.
[/quote]


this 👍🏽 ty
```

---
## \#79 Posted by: Eboosted Posted at: 2019-02-11T03:56:17.186Z Reads: 95

```
This is great, subscribed
```

---
## \#80 Posted by: Eboosted Posted at: 2019-02-26T00:20:04.189Z Reads: 82

```
Hello Guys, I was planning to write this firmware but there is only a link for the Unity not the regulaer Focbox, can someone point me to the right direction?
```

---
## \#81 Posted by: CarlCollins Posted at: 2019-02-26T00:22:07.835Z Reads: 81

```
Firmware is only for Unity, There isn't any updated one for regular FOCBOX
```

---
## \#82 Posted by: Blasto Posted at: 2019-02-26T00:28:34.658Z Reads: 77

```
This fix has been pushed to the lattest unity fw. Just grab it from the git
```

---
## \#83 Posted by: Battosaii Posted at: 2019-02-26T00:30:50.530Z Reads: 76

```
I run 160a battery max and 320a motor max but I run a big battery and 4wd.

Going to test out the new firmware next ride :slight_smile: @CarlCollins @Deodand does the new FW update allow us to turn off 2 Unities with 1 button now?
```

---
## \#84 Posted by: CarlCollins Posted at: 2019-02-26T00:31:42.262Z Reads: 74

```
@Battosaii
I am not sure about it, haven't tested it yet, may @Deodand will help you with this :slight_smile:
```

---
## \#85 Posted by: Blasto Posted at: 2019-02-26T00:34:06.512Z Reads: 76

```
[quote="Battosaii, post:83, topic:80201"]
does the new FW update allow us to turn off 2 Unities with 1 button now?
[/quote]

We will be testing that out this week
```

---
## \#86 Posted by: Battosaii Posted at: 2019-02-26T00:35:45.608Z Reads: 79

```
Can't wait to see the results :slight_smile:

I love my Unities but that would make them complete.
```

---
## \#87 Posted by: Eboosted Posted at: 2019-02-26T00:37:22.958Z Reads: 79

```
[quote="CarlCollins, post:81, topic:80201, full:true"]
Firmware is only for Unity, There isn’t any updated one for regular FOCBOX
[/quote]

I'm sure there is a fix already, not sure how reliable is though

[quote="Blasto, post:82, topic:80201, full:true"]
This fix has been pushed to the lattest unity fw. Just grab it from the git
[/quote]

But I'm not runing an Unity at the moment, just regular dual Focboxes
```

---
## \#88 Posted by: Blasto Posted at: 2019-02-26T00:38:51.263Z Reads: 80

```
Ah sorry, misread you. 

I don’t have a definitive answer to your question
```

---
## \#89 Posted by: CarlCollins Posted at: 2019-02-26T00:40:47.005Z Reads: 84

```
[quote="Eboosted, post:87, topic:80201"]
I’m sure there is a fix already, not sure how reliable is though
[/quote]

What issues you are having with your dual FOCBOXes?
Is it a Raptor?
```

---
## \#90 Posted by: CarlCollins Posted at: 2019-02-26T00:41:25.791Z Reads: 82

```
@Battosaii
Do share your results as well :slight_smile:
```

---
## \#91 Posted by: Indiangummy Posted at: 2019-02-26T00:41:53.941Z Reads: 88

```
If I'm running the breaking firmware that Jeff linked in the op can, I update to the latest FW though the unity UI app?
```

---
## \#92 Posted by: CarlCollins Posted at: 2019-02-26T00:43:17.535Z Reads: 89

```
It will be best if you use USB-C cable and Windows version of FOCBOX UI Version 1.1 to update the firmware.

Firmware upgrade using Bluetooth will drop if connection is unstable
```

---
## \#93 Posted by: Eboosted Posted at: 2019-02-26T01:00:36.715Z Reads: 88

```
[quote="CarlCollins, post:89, topic:80201"]
What issues you are having with your dual FOCBOXes?
Is it a Raptor?
[/quote]

The issue stated in the thread header Low Speed Braking, it's not a Raptor 2 BTW
```

---
## \#94 Posted by: Jc06505n Posted at: 2019-02-26T04:28:42.759Z Reads: 87

```
Ben has a fix for this it should be somewhere on his git for the vesc
```

---
## \#95 Posted by: CarlCollins Posted at: 2019-02-26T10:21:26.314Z Reads: 82

```
Haven't you adjusted the braking using the tool or something?
```

---
## \#96 Posted by: Stillshreddin Posted at: 2019-02-26T10:29:28.610Z Reads: 81

```
Starting my first build these next few weeks or months...just bought my board today. I would love. The opportunity to test or try out anything you guys make! ![20190225_223237|629x500](upload://g9cwq3SbffRcfVWQ8Flcdoxyj9D.jpeg)
```

---
## \#98 Posted by: district9prawn Posted at: 2019-04-21T00:57:41.689Z Reads: 43

```
Tried this fix on an ebike. The hysteresis implemented in the latest official firmware didn't really help much with the cogging but this fix nailed it!
```

---
