# Are my VESC settings correct?

### Replies: 46 Views: 3494

## \#1 Posted by: Smorto Posted at: 2017-02-04T21:18:41.033Z Reads: 330

```
Hello, I am making this thread so that someone can confirm that my VESC seeing or correct or see what I did wrong. This is an @chaka  VESC that has already had some trouble in its very short lifetime. The day I got it I screwed it up my inputting some wrong voltage values. So I sent it back and they fixed it free of charge which is awesome. This time I am going to be a little more careful by checking on the forum first. I will include some screenshots of my settings below. One more weird thing though. When I was setting it up, I (for whatever reason) pulled the receiver out of the VESC while the vesc was still turned on. Then, every time I connect to the BLDC tool, it comes up in a different modem number, for example it used to say "cu.usbmodem301", but the next time I booted up it said "cu.usbmodem9", then it said "cu.usbmodem14" and it keeps changing every single time. You can see this on the last two pictures that they are different from all the others. Thanks for your advice in advance!

EDIT- My Batt min (regen) I believe is set to -5A, not -10A


<img src="/uploads/db1493/original/3X/b/3/b351d778f24e81e8017cba7c8826250f31282f44.png" width="690" height="387">

<img src="/uploads/db1493/original/3X/7/8/7892f668db8175a21088a9a6896738860fc2d90d.png" width="690" height="387">

<img src="/uploads/db1493/original/3X/5/8/58088a4a02c733990c75bd718ce7ef945e5271c1.png" width="690" height="387">

<img src="/uploads/db1493/original/3X/d/b/db6cff542420c1db0797776a7975d22b8cb0dd58.png" width="690" height="387">
```

---
## \#2 Posted by: Martinsp Posted at: 2017-02-04T21:25:31.312Z Reads: 293

```
I dont think that the USB connection or modem or whatever is a problem, If the VESC settings still write on the VESC memory it should be OK. 

To tell you If your voltages and other stuff is correct we would need to know more info about your setup, type of battery, what the max current ratings are and cell count and so on...
```

---
## \#3 Posted by: Smorto Posted at: 2017-02-04T21:29:26.306Z Reads: 297

```
Oh crap! I was going to write that, just forgot to I guess. Here are my specs 190kv sensored motor (I don't have the adapter for the sensor wire yet so when I do I will run motor detection again). Two 4s 5000mah 20c lipos in series for one 8s battery. Is there anything else you need to know?
```

---
## \#4 Posted by: Martinsp Posted at: 2017-02-04T21:37:49.697Z Reads: 287

```
No not really, most of the other settings are just personal preferences in my opinion. Voltage and amperage is what can kill your VESC, motor and battery. 

The settings seem to be fine just the "motor min" is in my opinion too low, here where I live I need it to be higher because that is what determines your braking force. If you live in a "hilly" area that might be an issue because of not enough power for braking down hill. Also climbing the hills with 40 amps (depending on your weight etc) might be an issue. but on the other hand having more amps and not enough air flow might over heat the VESC. All of the values are set pretty safe as they are so the VESC should not get damaged by them. And if you find them to not be right for you you can change them but that needs test riding atc.. 
Hope this helps :)
```

---
## \#5 Posted by: Smorto Posted at: 2017-02-04T21:48:17.313Z Reads: 257

```
I am not sure if you saw my edit but my batt min (regen) is actually set to -5A I think. Am I correct in saying that that value is the amperage you can charge your battery at? Because 5A would be 1c for me which I use for charging anyway. And I am a bit confused by what you were saying about my "motor min" what do you think I should change it to? I way around 120 pounds and I would only have to climb a few smallish hills, maybe a few larger ones. Thanks for your help btw.
```

---
## \#6 Posted by: Martinsp Posted at: 2017-02-04T22:03:12.159Z Reads: 250

```
did not see the edit sorry. The regen is OK at 5 and 10 is doable it wont relly damage the battery because lipos are made to be drained at high amperage (for such aplications that is) so they will handle 2c charging but it might shorten their life a little bit. 
The motor min seems OK, you are quite light so it might be all right. But as I said, try it preferably on flat ground first and you will see what you need to adjust. I usually set it to the same as my motor max so I can reverse the same speed as i go forward and also because i like hard braking and the hills are steep here.
```

---
## \#7 Posted by: Smorto Posted at: 2017-02-04T22:08:52.730Z Reads: 238

```
Ok, so the motor min (regen) will increase braking force? Sorry if I am asking dumb questions but I know very little about the VESC.
```

---
## \#8 Posted by: Martinsp Posted at: 2017-02-04T22:13:55.800Z Reads: 229

```
Yes motor min and max is what adjusts (increases or decreases) the power (power equals amperage times voltage) so the motor max is the max amount of amps that the VESC is going to allow to be sent to the motor windings and the same for motor min. In your aplication (current no reverse with brake) it will adjust the braking speed (motor min) and the forward power of the motor or acceleration (motor max). Often times this gets confused with battery min and max which set the draining amps from battery and the charging or regen amps.
```

---
## \#9 Posted by: Martinsp Posted at: 2017-02-04T22:15:16.021Z Reads: 213

```
no question is dumb in my opinion, everyone has to get the knowledge somehow, asking and researching is the only way :D
```

---
## \#10 Posted by: Smorto Posted at: 2017-02-04T22:24:22.120Z Reads: 202

```
Thanks for that! I have read a ton but much of it still goes over my head. I will defiantly keep this in mind, thank you!
```

---
## \#11 Posted by: Martinsp Posted at: 2017-02-04T22:30:56.010Z Reads: 199

```
Iam happy that it helped :) ride safe!
```

---
## \#12 Posted by: Smorto Posted at: 2017-02-04T22:52:24.009Z Reads: 198

```
Anyone else have anything to add? :slight_smile:
```

---
## \#13 Posted by: rpn314 Posted at: 2017-02-05T01:53:09.579Z Reads: 190

```
You could change your ERPM limits to 60000 instead of 100,000, but not a huge thing.
You could also probably increase your batt max later on if you feel like you want more power. I think your batteries can handle 50+ amps
When you finish doing the motor detection, and it didn't fail, make sure you click "apply" under "Start Detection" or the parameters won't be applied. The values you have are close, so I can't tell if it automatically rounded up (which is often does) or not. I can't remember how much it rounds.
```

---
## \#14 Posted by: Smorto Posted at: 2017-02-05T03:25:28.911Z Reads: 189

```
Hello, I rounded the motor detection results to the nearest 5 for Int. Limit, and the nearest 50 for BEMF Coupling as stated in the @torqueboards tutorial on youtube [here](https://www.youtube.com/watch?v=dxDXUrk-7ek). I will run it again though once I get my VESC sensor wire adaptor which I ordered today. So for changing my ERPM would I change both max and min to 60,000? Also what exactly do you mean by "more power" does this correlate to more torque or more speed? Thanks!
```

---
## \#15 Posted by: rpn314 Posted at: 2017-02-05T03:37:49.753Z Reads: 189

```
I'd say just let the program handle the rounding. Vedder built it quite well and it'll put it close enough to where you need it. Run motor detection, make sure it didn't fail, and then just hit apply.

I would change both the the max and min ERPM to 60000 (the min stays negative though). The VESC can handle 100,000, but I tend to side on the safer side and set it a bit lower. Some agree while others will disagree. I'd search through other's posts on the ERPM limit if you want to know more cause I don't think I'd explain it as well as they have.

You'll feel the difference in battery current when you're speeding up (especially from a stop) and when you're going uphill. Basically if you ever feel like it's sluggish at either, I'd start by increasing your batt max.

I'll also make a note about the motor min/max. When you're hitting the edge of what you've set, either the motor max/min is going to hit the limit first or the battery is. I tend to set the battery limits according to what the batteries can handle and then just set the motor limits really high (like 60 and -60). So then I never hit that motor limit because I always hit my battery limit first. That's also partially because I have a good understanding of what the batt min/max means and I don't entirely understand how the current that the vesc takes in from my batteries translates to the current the vesc sends to a motor.
```

---
## \#16 Posted by: Smorto Posted at: 2017-02-05T03:43:27.103Z Reads: 179

```
Thanks, I will have to explore the settings of my battery and motor limits as I get some more tests in. But for now nothing is going to blow up if I give it a few test runs? :slight_smile:
```

---
## \#17 Posted by: rpn314 Posted at: 2017-02-05T03:44:47.450Z Reads: 178

```
I don't see any other issues in what you posted so far. Can you post the Motor Configuration Advanced tab? That would be the last thing I'd check.
```

---
## \#18 Posted by: Smorto Posted at: 2017-02-05T03:56:56.569Z Reads: 178

```
There you go. Only thing I changed was startup boost though.<img src="/uploads/db1493/original/3X/d/1/d1e9e6164c8c7cf82ef80c45de6c86a173818d73.png" width="690" height="387">

Also changed Batt max to 30 and ERPMs to 60k. As well as run motor detection again and clicked apply instead of rounding.
```

---
## \#19 Posted by: rpn314 Posted at: 2017-02-05T04:02:49.625Z Reads: 168

```
K. I think you're set! Just go easy on the throttle when you start out ;)
```

---
## \#20 Posted by: Smorto Posted at: 2017-02-05T04:09:47.778Z Reads: 160

```
Haha will do. Just gonna be tests in my basement until this north eastern winter goes away though :slight_smile:.
```

---
## \#21 Posted by: Smorto Posted at: 2017-02-05T14:45:48.674Z Reads: 144

```
Oh! One more thing I forgot to ask you, do **you** think that modem switching thing that I mentioned in my first post is a big deal or nothing to worry about? Have you ever heard/seen of this happening before?
```

---
## \#22 Posted by: rpn314 Posted at: 2017-02-05T14:56:00.901Z Reads: 145

```
Less than nothing to worry about. Happens to me as well. It's what your computer has labeled it (i.e. the number is not coming from and has little to do with the VESC itself). I can give you a longer explanation, but it's not really worth it for either of us.
```

---
## \#23 Posted by: Smorto Posted at: 2017-02-05T15:29:52.929Z Reads: 141

```
Awesome, thanks.
```

---
## \#24 Posted by: Smorto Posted at: 2017-04-29T18:56:25.824Z Reads: 129

```
Hello again, thinking of changing my Batt Max to 45 for a bit more power as well as motor min to -45 for a bit more braking force, will these settings do anything bad for my VESC or make it more at risk for damage?

@rpn314

@Martinsp

Maybe @Ackmaniac could help too.
```

---
## \#25 Posted by: rpn314 Posted at: 2017-04-29T19:44:29.332Z Reads: 124

```
I foresee no issues with that (mostly based on my previous comment that the batteries should be able to handle 50+ amps)
```

---
## \#26 Posted by: Smorto Posted at: 2017-04-29T20:30:28.558Z Reads: 123

```
Awesome, what do you think is the highest I could safely raise my motor min to to increase braking? (That is what the motor min (regen) does correct?)
```

---
## \#27 Posted by: rpn314 Posted at: 2017-04-29T20:47:12.450Z Reads: 122

```
Braking strength is a combination of battery min, motor min, and some controller setting. For example, if you're battery limit is -1, it won't really matter what your motor min is cause it will always go with the battery. I actually have my motor limits set to 70 and -70 I believe, and then I just set my battery to how much charge current my battery pack can handle
```

---
## \#28 Posted by: Smorto Posted at: 2017-04-29T20:49:45.108Z Reads: 121

```
So my battery min is -5A which is 1c for my pack. Will increasing the motor min increase braking force at all?
```

---
## \#29 Posted by: rpn314 Posted at: 2017-04-29T20:52:52.948Z Reads: 122

```
My guess is yes it is, but it's hard to say for sure. You'd have to have some recorded telemetry data from you riding it to see if it's hitting the -5 limit. You can probably up that to -10 and be okay. Or you can change the motor min, try it out, and then change the battery and try it out.
```

---
## \#30 Posted by: Smorto Posted at: 2017-04-29T20:55:59.473Z Reads: 121

```
So If I increase Batt Min (regen) to -10 and Batt Max to 45 and motor min to -45 I should have a little more power, a little more breaking force, and I will still be safe in terms of frying my VESC?
```

---
## \#31 Posted by: rpn314 Posted at: 2017-04-29T21:08:08.791Z Reads: 118

```
You are nowhere near frying your vesc. I'm much more worried about your batteries and you (getting thrown because it too hard or hitting something because it couldn't stop fast enough) than your vesc.
```

---
## \#32 Posted by: Smorto Posted at: 2017-04-29T21:10:53.684Z Reads: 116

```
I am paranoid about frying my vesc because $170 dollars for a part in a hobby project is a lot for a high school student lol, I will change those settings. :slight_smile:. Thanks for your help.
```

---
## \#33 Posted by: rpn314 Posted at: 2017-04-29T21:16:57.791Z Reads: 118

```
No worries! I'm finishing my undergrad as well, so I totally understand. Most of the issues frying VESCs that I've seen were related to too high of a current ramp step (one of the advanced settings) and improper FOC configuration. If you don't have any extra cooling (heat sink or something), you'd have to push the battery current up closer to 80A before I'd be worried.
```

---
## \#34 Posted by: Hummie Posted at: 2017-04-29T21:20:41.115Z Reads: 121

```
Motoramps.com.  For simplicity:  to get low speed power up the motor amps (up to 160 is fine if you like it) and high speed power decided more by the battery amps.
```

---
## \#35 Posted by: flywithgriff Posted at: 2017-04-30T00:36:58.364Z Reads: 117

```
I appreciate the info in this thread! I am also tuning my VESC and am really not sure what does what. Is it as simple as:

Braking is controlled by:
Startup acceleration is controlled by:
Top end acceleration is controlled by:
Top speed is controlled by (other than gearing and battery size):

I'm running 6s, 15/36, 97mm. Currently have plenty of top speed (22 mph) but barely any brakes and acceleration on takeoff could be stronger. 

<img src="/uploads/db1493/original/3X/d/c/dc6e49efd50440816e39d6d1d41c3554c3c55daf.JPG" width="666" height="500">
```

---
## \#36 Posted by: Smorto Posted at: 2017-04-30T02:49:03.382Z Reads: 112

```
Really? You have barely any brakes with those values? I don't know very much about VESC's but your values are higher than mine so I would assume you would have more breaking force. Is your belt tight enough? That's the only other thing I can think of.

As for startup acceleration that could also be a loose belt but the 'startup boost" setting might help as well.
```

---
## \#37 Posted by: flywithgriff Posted at: 2017-04-30T02:53:30.427Z Reads: 109

```
I'm running a pretty tight belt as I have never had any skipping. I just upped my startup boost and have spend the past hour scouting the forum for motor and battery max and mins without much confidence inspiring luck.

Anyone want to chime in with setting for highest performance? I need low end power.

6s 8ah 30c, 15/32, 97mm VESC.  I'm a big guy at 250lbs
```

---
## \#38 Posted by: Smorto Posted at: 2017-04-30T02:59:57.306Z Reads: 111

```
What motor?
```

---
## \#39 Posted by: flywithgriff Posted at: 2017-04-30T03:00:41.758Z Reads: 114

```
Tacon Bigfoot 160
```

---
## \#40 Posted by: rpn314 Posted at: 2017-04-30T03:09:11.963Z Reads: 114

```
The basics of it is there are max/min limits and steps (most of what you see on the Advanced tab of Motor Configuration. The VESC will not allow things to go over any of those min/max limits and the steps control how fast things are allowed to change from one thing to another. 
WARNING: The advanced settings are very sensitive and are under the advanced tab for a reason. You can get yourself hurt and/or fry your VESC if you don't know what you're doing with them. If you feel you must modify them, see what the default settings are (click "Read Default Configuration") and modify them in very small increments relative to those settings. YOU HAVE BEEN WARNED.

Credit (where credit is due): I knew a lot of the main ones, but some of the more advanced ones I got from @Ackmaniac's modified BLDC-Tool (he has done a lot of work on it, including adding mouseover help windows for pretty much every setting)

These are the things that I'm aware of. I wouldn't consider this 100% complete, cause I probably missed something, but a solid starting point.

Responsiveness: (how quickly any power output changes; applies to pretty much all of the things below so I listed them together here): Gain, Duty Ramp Step, Max Current Ramp Step, KP, KI, KD.

Braking is controlled by: Batt Min (regen), Motor min (regen)
Startup acceleration is controlled by: Batt Max, Startup Boost, 
Top end acceleration is controlled by: (Not sure exactly what you mean by this, but it's pretty much the same as startup I believe)
Top speed is controlled by (other than gearing and battery size): Max ERPM, Batt Max, Motor Max.
```

---
## \#41 Posted by: Smorto Posted at: 2017-04-30T03:13:42.820Z Reads: 108

```
KV? If it is the 245 version then there is your culprit for not enough low end torque IMO.
```

---
## \#42 Posted by: Hummie Posted at: 2017-04-30T03:14:16.914Z Reads: 104

```
Start up acceleration is controlled by motor amps
Motoramps.com

If u want low speed power you've got all the way up to 160 motor amps and not a problem @flywithgriff
```

---
## \#43 Posted by: rpn314 Posted at: 2017-04-30T03:25:42.859Z Reads: 102

```
[quote="Hummie, post:42, topic:17213, full:true"]
Start up acceleration is controlled by motor amps
Motoramps.com

If u want low speed power you've got all the way up to 160 motor amps and not a problem @flywithgriff
[/quote]

@Hummie when you typed Motoramps.com a few posts up, I thought it was some typo so I ignored it. Seeing it again, I figured it wasn't so I actually went there. WOW. Guys, stop reading this and go there. www.motoramps.com See you in a few hours ;P
```

---
## \#44 Posted by: flywithgriff Posted at: 2017-04-30T03:54:59.099Z Reads: 98

```
Yes it's the 245kv as I was told to get for 6s when I first started my build.

@Hummie knowing what I'm running what would be your suggested starting numbers? Please sir
```

---
## \#45 Posted by: PXSS Posted at: 2017-04-30T03:56:12.721Z Reads: 97

```
@flywithgriff
Read what I posted on your thread
```

---
## \#46 Posted by: Hummie Posted at: 2017-04-30T04:22:51.686Z Reads: 96

```
id ask devin to do the math to get you consistent power out at every rpm.  You'll need your motor's resistance number off your vesc motor test.   if you write him I'm sure he'd do it.  the formula is relatively simple I think despite it's looks but I dont bother.   Or get ackamaniacs software.  I'd say just up the motor amps but I've been surprised by the numbers sometimes.
```

---
