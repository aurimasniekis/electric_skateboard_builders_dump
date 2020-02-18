# VESC Brakes grabbing coming to stop

### Replies: 56 Views: 2774

## \#1 Posted by: SkaterBoy58 Posted at: 2018-02-20T12:24:38.815Z Reads: 324

```
Just testing out a new build with dual motors 140kV 10S 4.12HW 3.34FW vescs with max brake current set to -25A. Wheels are pneumatic 175mm diam with 66T wheel cog and 15T motor cog. Sensored motors with sensorless above 7,000 erpm. Acceleration is very smooth .

The brakes are very smooth and fine coming from speed - but when slowing down at about 3km/h they grab quite hard . This is approx 3,000 erpm.

Any idea what is causing this ?  . I recall reading somewhere that the vesc shorts two phases for final braking- maybe this is what is happening. If so - is there a setting to switch this off or to reduce the braking current a bit.
Thanks
```

---
## \#2 Posted by: mccloed Posted at: 2018-02-20T15:22:42.203Z Reads: 294

```
Are you running FOC or BLDC?
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-02-20T15:46:30.821Z Reads: 286

```
The setting you're looking for is labeled something like "minimum ERPM to apply full brake", or at least it is in the original bldc tool and vesc tool. I haven't used ack's extended tool though.
```

---
## \#4 Posted by: SkaterBoy58 Posted at: 2018-02-20T23:05:31.785Z Reads: 268

```
Running FOC  with CAN bus  - 

I cant find a setting on VESC Tool for "minimum ERPM to apply full brake"  

Is it something to do with the hand brake settings?

Thanks
```

---
## \#5 Posted by: GreasyGearsWRX Posted at: 2018-02-21T07:21:42.517Z Reads: 249

```
I'm interested to know what this could be. I just switched to a new motor without changing any setting that weren't crucially needed for a new motor and am having this happen below 5mph.
```

---
## \#6 Posted by: auggie246 Posted at: 2018-02-21T10:10:03.630Z Reads: 250

```
Exact same thing is happening to me on my Maytech motor. I am using vesc tool too. 
Atm when braking I do not full break and use foot brake at the end instead.
```

---
## \#7 Posted by: Tomer Posted at: 2018-02-21T10:56:18.966Z Reads: 243

```
Have you tried to calibrate your remote controller in the VESC Tool?
```

---
## \#8 Posted by: telnoi Posted at: 2018-02-21T10:57:54.956Z Reads: 235

```
Trampa mentioned in the past that bat min and motor min have to be more or less identical for linear braking in FOC mode. I haven't tried it myself/switched to BLDC.
```

---
## \#9 Posted by: SkaterBoy58 Posted at: 2018-02-21T11:03:30.555Z Reads: 232

```
My braking is very linear and smooth down to about 3-4km/hr then it grabs hard.
Must be a dfferent setting somewhere but I cant find it
Cheers
```

---
## \#10 Posted by: SkaterBoy58 Posted at: 2018-02-21T11:04:21.870Z Reads: 224

```
Yes -The remote is calibrated fine using vesc tool
```

---
## \#11 Posted by: telnoi Posted at: 2018-02-21T11:04:29.179Z Reads: 219

```
so were mine, except at low speed. That is the advice trampa gave based on my experience/exact same issue you are describing. Something to do with motor min being used predominantly at low speed. Worth a shot right? Set both bat & motor min at the min bat value.
```

---
## \#12 Posted by: SkaterBoy58 Posted at: 2018-02-21T11:13:08.131Z Reads: 205

```
No worries -Thanks for the hint-will give it a go and see how it goes
```

---
## \#13 Posted by: SkaterBoy58 Posted at: 2018-02-21T11:19:24.307Z Reads: 204

```
Just checked my settings and they are both set to -25A
```

---
## \#14 Posted by: telnoi Posted at: 2018-02-21T11:20:21.771Z Reads: 210

```
crap, that's a shame. Would be worth posting the feedback in the vesc-tool thread.
It would appear a fair number of people are having this issue with FOC.
```

---
## \#15 Posted by: SkaterBoy58 Posted at: 2018-02-21T11:21:50.576Z Reads: 200

```
It is defintly a speed issue and is very repeatable and it seems to not be related to braking motor current at that particular speed when it grabs
```

---
## \#16 Posted by: Clonkex Posted at: 2018-02-21T12:28:08.188Z Reads: 203

```
This is what @MysticalDork is referring to: 

![image|690x407](upload://158ltpTfKxTCXEXhuQ2K8kDGBOC.png)
```

---
## \#17 Posted by: SkaterBoy58 Posted at: 2018-02-21T13:23:29.367Z Reads: 192

```
Dont think Vesc tool has that setting
```

---
## \#18 Posted by: SkaterBoy58 Posted at: 2018-02-22T09:44:37.391Z Reads: 191

```
Guys
I think I have found a solution to this by directly editing some motor xml file parameters.
Just doing final testing now
Cheers
```

---
## \#19 Posted by: SkaterBoy58 Posted at: 2018-02-22T23:41:31.482Z Reads: 194

```
So below is what I tried and it seems to work OK - **Try below at your own risk** 

I an running dual DIYE 4.12HW vescs in FOC that came with 2.18FW. Updated vescs to 3.34FW using vesc tool 0.87.

The parameter "Max ERPM at full brake in current control mode" exists in BLDC tool but for some reason seems to have disappeared in the vesc tool.   

So the first thing I did is to save motor xml file from vesc and then load it into BLDC tool. All parameters seemed to load OK into BLDC tool  with same current and voltage settings. 

Noticed that the value of "Max ERPM at full brake in current control mode" was 1500 erpm which corresponds to the speed at which the brakes were grabbing . 

You may be able to adjust that setting in BLDC tool - then do a xml save and then load xml file into vesc tool and then download to vesc. I didn't want to try this due to possibility that bldc tool could upset parameters in vesc tool and possibly fry the vesc.

So what I did was to get a xml file editor ( I used one from mediafreeware.com ) 

Then get the vesc  motor  xml file from vesc tool and load it into the xml editor.

Look for a line showing 

![parameter|526x91](upload://dTGNEgfF9YP5RpRGyj8wldn0VmP.jpg)

The using xml editor - change the 1500 no to 200 ( about 1km/hr for me) with no other changes.

Then using xml editor save the xml file , then load that modified xml file into the vesc tool and then push motor config to the vesc. repeat for the other vesc if running dual drives

Note - one of my vescs came with 1500 for  "Max ERPM at full brake in current control mode" and one was showing 500 . I guess these were different default settings on initial 2.18FW set-up and have not been changed by the vesc tool ( A bit strange!).

 I changed both vescs to 200 erpm and it seems to work fine.

Cheers![before|589x500](upload://hyfAuxyUHzrB0tqE6Ko174fVWrl.jpg)
```

---
## \#20 Posted by: telnoi Posted at: 2018-02-23T06:22:35.680Z Reads: 192

```
@trampa

Can you expose that parameter in the gui in a future update?

Explains why random people have this issue. Different stock values.
```

---
## \#21 Posted by: Silverline Posted at: 2018-03-08T17:56:09.765Z Reads: 185

```
Just updated my FOCBOXES to the newest Firmware... now i have this "issue" as well.... pretty annoying......

Is the @SkaterBoy58 way, stil the only way ?
```

---
## \#22 Posted by: deucesdown Posted at: 2018-03-08T18:18:53.052Z Reads: 180

```
It's strange that it works as in BLDC Tool that setting is in a section labeled "BLDC only"
```

---
## \#23 Posted by: kyletrainy Posted at: 2018-03-08T18:28:00.843Z Reads: 176

```
I think so. I set mine to 500 and braking is a lot more manageable
```

---
## \#24 Posted by: Silverline Posted at: 2018-03-08T18:29:02.286Z Reads: 170

```
Is it something in vesc-tool you set to 500 ? Or do i need to do this bldc/xml thing ?
```

---
## \#25 Posted by: kyletrainy Posted at: 2018-03-08T18:57:17.675Z Reads: 166

```
Edit the xml
```

---
## \#26 Posted by: Charles_Chan Posted at: 2018-04-18T08:43:30.850Z Reads: 161

```
If I don't edit the xml file, just use vesc-tool to setup, can I do full break? thanks
```

---
## \#27 Posted by: trampa Posted at: 2018-04-18T10:30:39.709Z Reads: 161

```
Hi SkateBoy58, personally I do prefer strong brakes over weak ones... Imagine you are going down a steep hill at relatively slow speed. You will need brakes that have some grip to prevent an unwanted acceleration down that hill. People should be able to brake to a near stand still on a hill. Without strong brakes that is not possible.
It is no big trick to release the brake trigger further when slowing down to a near stand still. If you ride a car you do the same, approaching traffic lights. On the last few mph you usually start to release the brakes a bit since the kinetic energy the brakes need to work against is getting very little close before the full stop.

A lot also depends on your motor and gearing. Your setup is quite rich of torque. In consequence your brakes do also work quite well.
```

---
## \#29 Posted by: Sender Posted at: 2018-06-15T23:26:28.410Z Reads: 147

```
@SkaterBoy58 i think this fix is a bit out of my wheelhouse. @mmaner?
```

---
## \#30 Posted by: mmaner Posted at: 2018-06-16T00:17:28.231Z Reads: 145

```
The post was deleted so I don't know.
```

---
## \#31 Posted by: Eboosted Posted at: 2018-06-16T00:47:41.163Z Reads: 143

```
[quote="SkaterBoy58, post:19, topic:46946"]
The parameter “Max ERPM at full brake in current control mode” exists in BLDC tool but for some reason seems to have disappeared in the vesc tool.
[/quote]

When you say VESC Tool are you refering to the latest version ESC Tool?

this one?
![image|690x437](upload://9SXh5jtB3dlYaEFX9t3OuU2CWCY.png)
```

---
## \#32 Posted by: chinzw Posted at: 2018-09-06T16:53:21.556Z Reads: 124

```
He's not complaining about the torque of his brakes.
I'm having the same issue since updating to the latest firmware. Brakes are fine, then i get to about 2-3 mph and the motors lock up. It has nothing to do with releasing the break trigger...
The max ERPM setting needs to be exposed for FOC, its as simple as that.
```

---
## \#33 Posted by: Jc06505n Posted at: 2018-09-06T17:05:16.570Z Reads: 129

```
https://www.electric-skateboard.builders/t/wheels-brake-locking-in-foc-right-before-dead-stop/39136?u=jc06505n

These two topics should really be merged
```

---
## \#34 Posted by: brenternet Posted at: 2018-09-06T17:06:03.427Z Reads: 130

```
I'm experiencing this as well on my new build. 6355, focbox, FOC, 16/40 belt. Slowing down/stopping from any speed above around 4mph is smooth - all the way to stand still. Anything below 4mph and it doesn't matter how gentle I am on the brakes it just locks up and jerks.

Manageable but annoying. I'm using ackmaniac, has anyone found a solution other than editing the xmls yet?
```

---
## \#35 Posted by: ervinelin Posted at: 2018-09-06T17:11:43.813Z Reads: 125

```
Editing XML didn't work for me
```

---
## \#36 Posted by: brenternet Posted at: 2018-09-06T17:15:51.166Z Reads: 124

```
Well that's wank 😑
```

---
## \#37 Posted by: Sender Posted at: 2018-09-06T18:38:31.761Z Reads: 119

```
Yup I am subscribed to all these; hopefully a fix come about. It is present on all my builds.  All ack firmware FOC sensored.

10s6p on 107s with 18/40
12s5p on 6shooters 20/60
6s3p on 83s with 14/36
```

---
## \#38 Posted by: Silverline Posted at: 2018-09-07T09:50:10.278Z Reads: 111

```
Still hate this "handbrake" thing.
```

---
## \#39 Posted by: vjsharpeyes Posted at: 2018-12-11T00:44:55.250Z Reads: 96

```
Just set up my first FOC build and am joining this club.
If anyone has any resources on exporting, editing and reloading an XML file with the VESC tool I would appreciate seeing them before I give it a shot.
```

---
## \#40 Posted by: tsr Posted at: 2018-12-12T07:03:17.892Z Reads: 91

```
In the PID Controllers section, reduce the value of "Minimum ERPM" and see if this fixes the problem. This value is used while braking, and if the current erpm is lower than this value, it switches to "duty cycle" mode and sets the duty cycle to 0 which I think causes this sudden sticky stop while doing low speed braking... Anyway, made it a lot better for me when i reduced this from 900 to 300, so you might wanna give it a try
```

---
## \#41 Posted by: deltazeta Posted at: 2018-12-12T07:18:30.936Z Reads: 90

```
Where does it switch to duty cycle mode?
```

---
## \#42 Posted by: tsr Posted at: 2018-12-12T16:02:22.742Z Reads: 87

```
![image|690x197](upload://lsnAbmvgvAhSLzl3HQ1jKqlpbvD.png)
```

---
## \#43 Posted by: deltazeta Posted at: 2018-12-12T20:46:06.685Z Reads: 86

```
Doesn't that just switch according to some hard coded 0.03? s_pid_min_erpm doesn't get touched unless you're in speed control.
```

---
## \#44 Posted by: ervinelin Posted at: 2018-12-13T01:05:46.378Z Reads: 84

```
Still no solution to this?

Mine was slightly lessened when I changed from a 15T to 18T pinion... But it's definitely still there.

8" wheels on dual focboxes.
```

---
## \#45 Posted by: lrdesigns Posted at: 2018-12-13T02:04:22.196Z Reads: 83

```
This was also being discussed over here. @Deodand said he was going to look into it but I am sure he will be way too busy for while. 

https://www.electric-skateboard.builders/t/vesc-based-controllers-brakes-locking-at-low-speed-for-larger-wheels-in-foc-possible-unity-fix/73547?u=lrdesigns
```

---
## \#46 Posted by: deltazeta Posted at: 2018-12-13T04:05:55.698Z Reads: 80

```
I wonder if you could just lower the hard coded value in @tsr 's codeblock. If the controller isn't actually losing sync, then brakes would be fine.

anyone willing to test? risk of losing brakes at low speeds
```

---
## \#47 Posted by: vjsharpeyes Posted at: 2018-12-14T04:07:11.116Z Reads: 73

```
Hey! Thanks so much for the advice. I have been messing with that value and it a lot better. Still not perfect, but I feel a lot more comfortable coming to a dead stop now.
Thanks for taking the time to reply and share your knowledge.

For anyone else looking in on this, I run 100mm wheels and have set it to 450.
```

---
## \#48 Posted by: Deodand Posted at: 2018-12-14T04:12:34.310Z Reads: 77

```
This is on my todo list, FYI in FOC the setting described doesn't do anything it is used in BLDC only. That hard coded value of 0.03 is a percent duty cycle (3%) and when your motors get there the controller in braking switch from current control to duty cycle control and this causes the dramatic transition 

I know the problem and am working on a fix but with everything going on it will prob be a few weeks out.
```

---
## \#50 Posted by: Sender Posted at: 2018-12-14T04:40:29.466Z Reads: 79

```
Man, too much beer. Don't mind me!
```

---
## \#51 Posted by: tsr Posted at: 2018-12-14T05:57:05.394Z Reads: 79

```
[quote="Deodand, post:48, topic:46946"]
the setting described doesn’t do anything it is used in BLDC only
[/quote]

You are right about the 0.03% stuff. Actually checked this months ago and was in a hurry when I wrote my last reply. Anyway, maybe this value doesn't change anything meaningful (or maybe only in speed control mode), but:its used in FOC as well:


We are talking about this field:
![image|690x302](upload://eJdljdn6iYwo3FYAokpakV90FpN.png) 

Right?

And here it is used:
![image|628x500](upload://xbW8BXncczrD3uvhLnaNWmG9uFg.png) 

Funny thing in my opinion is that, according to my understanding of the code, this should only affect speed control mode, because otherwise m_speed_pid_set_rpm is always 0 (only set to different values in mcpwm_foc_set_pid_speed) and I am running all my boards only on current control mode. Nevertheless braking behaviour seemed to change at low speed when I changed this value... Maybe I was mistaken and actually nothing changed, but I can't test it currently because its too freaking cold outside - and testing braking behaviour on snow might also not be the best idea;)

Maybe this will help a little bit when you work on the fix.
```

---
## \#52 Posted by: neiru37 Posted at: 2018-12-14T06:53:17.870Z Reads: 71

```
Commenting to subscribe to this thread.
```

---
## \#53 Posted by: lrdesigns Posted at: 2018-12-14T07:05:31.450Z Reads: 75

```
Bro, just click the thing in the bottom left to subscribe. :wink: :grinning:

![image|538x500](upload://3tTDIU8sdDUlIV2RXE91W78PDtC.png)
```

---
## \#54 Posted by: neiru37 Posted at: 2018-12-14T07:19:50.670Z Reads: 79

```
TIL

10char
```

---
## \#55 Posted by: Deodand Posted at: 2018-12-14T16:00:29.685Z Reads: 73

```
I think this might be a placebo, but I will definitely investigate, as you say this parameter should only take effect in speed control mode so if it is effecting current control I would consider that a bug. 

The normal behavior with the change in brake force is less of a bug and more of a poorly switched control strategy to handle very slow speed braking. Abruptly switched control strategies causes an abrubt change in braking force, amplified with certain motor/gearing systems. One solution I've been mulling over is a soft transition, start switching to duty control around 10% instead and compute both current control and duty control then linear map between the two as you go from 10 to 2 percent say. Need to look more into it all to see if such a thing would be possible.
```

---
## \#56 Posted by: skatardude10 Posted at: 2018-12-15T03:40:58.805Z Reads: 69

```
How I imagine that riding sounds amazing. If you could acomplish what you describe, it would be like you coding free buckets of ice cream for the entire FOC community.
```

---
## \#57 Posted by: DAddYE Posted at: 2018-12-18T18:24:29.719Z Reads: 61

```
I can confirm that lowering it to 100 improved quite a bit the issue. I also reduced the deadband to 2% and now the dead stop is almost gone. I’m running 90mm wheels 6355 200kv motors on 11s3p. 40/-40 30/-7 motor/battery
```

---
## \#58 Posted by: McErono Posted at: 2018-12-24T19:41:54.108Z Reads: 48

```
I can confirm aswell! it does help a lot!
```

---
