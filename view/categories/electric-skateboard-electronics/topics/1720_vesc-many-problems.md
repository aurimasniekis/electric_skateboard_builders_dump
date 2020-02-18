# VESC many problems

### Replies: 34 Views: 5773

## \#1 Posted by: DeathCookies Posted at: 2016-03-08T17:12:24.170Z Reads: 279

```
Hey, 
I have a little problem. Well some problems...
Before I had a YEP heli ESC and i will use it for comparison. 
Here are all details of my current build and problems

My E-Board specs:
[213kv motor][1]
[2x 8000mah 6S battery in parallel][2]
VESC 4.10
All-Terrain-Wheels
9:40 Gear ratio

After i charged my batteries (25,2V) i (60kg)  drove about 7.1 km on a flat terrain and had 22,8V left. At the begining i could drive about 30km/h and maybe faster (did not have throttle on full).
After 3-4km I just could drive about 20km/h...

When I accelerate fully in the start of my ride i get a drop out. When i accelerate slowly i dont get it.
Later when i am stucked at 20km/h i can accelerate fully and do not get a drop out...

At the half of my ride i did a little brake (2-3 minutes) and after that i could go fast for a minute but then i get stucked at 20km/h again.

The brake is not strong at all... It brakes slowly and gently but in my oppinion to weak. Also i do not have any torque. It just accelerate slowly... 
With my heli ESC I had more torque and stronger breaking behaviour! 

My VESC lays on foam so i tested the heating. 
I tested it several times and the VESC was always warm but it was not Hot. So i dont think it is overheating. 

I installed the firmware for VESC 4.10 and the software says that 2.15 is on my VESC.
Here are my settings of the bldc tool:
[Motor Configuration][3]
[AppConfiguration  General][4]
[AppConfiguration PPM][5]

In a nutshell: 
(1) The speed shouldnt decrease after the half of a ride unless the cutoff is reached. 
(2) The brake and even the torque should be much much higher. 
(3) I should be able to drive twice as long. 
(4) If i accelerate only in the beginning of a ride fully i shouldnt get a drop out? 

I appreciate any help. Just tell me what and how to check and i will do it. 

  [1]: http://www.hobbyking.com/hobbyking/store/__45240__Turnigy_Aerodrive_SK3_6364_213kv_Brushless_Outrunner_Motor_EU_Warehouse_.html
  [2]: http://www.hobbyking.com/hobbyking/store/__64437__Multistar_High_Capacity_6S_8000mAh_Multi_Rotor_Lipo_Pack_US_Warehouse_.html
  [3]: http://fs5.directupload.net/images/160308/mpaancld.jpg
  [4]: http://fs5.directupload.net/images/160308/iucuo3fl.jpg
  [5]: http://fs5.directupload.net/images/160308/a6aslbld.jpg
```

---
## \#2 Posted by: treenutter Posted at: 2016-03-08T19:51:03.584Z Reads: 244

```
@DeathCookies There are two ERPM settings on VESC, make sure both are at the right value. However, being able to go full speed for a while and then becoming power-limited suggests that you're exceeding one of the VESC voltage cutoff thresholds. You probably need to edit that setting.
```

---
## \#3 Posted by: NerijusM Posted at: 2016-03-08T21:00:45.885Z Reads: 230

```
Your VESC is overheating. Same there.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-03-08T21:26:36.632Z Reads: 232

```
Now i will share all details of my build and problem

My E-Board specs:
[213kv motor][1]
[2x 8000mah 6S battery in parallel][2]
VESC 4.10
All-Terrain-Wheels
9:40 Gear ratio

After i charged my batteries (25,2V) i drove about 7.1 km on a flat terrain and had 22,8V left. At the begining i could drive about 30km/h and maybe faster (did not have throttle on full).
After 3-4km I just could drive about 20km/h...

When I accelerate fully in the start of my ride i get a drop out. When i accelerate slowly i dont get it.
Later when i am stucked at 20km/h i can accelerate fully and do not get a drop out...

At the half of my ride i did a little brake (2-3 minutes) and after that i could go fast for a minute but then i get stucked at 20km/h again.

The brake is not strong at all... It brakes slowly and gently but in my oppinion to weak. Also i do not have any torque. It just accelerate slowly... 
Also i do not have any torque with my setting which i hat before with the heli Esc. I am just accelerating very slow. 

My VESC lays on foam so i tested the heating. 
I tested it several times and the VESC was always warm but it was not Hot. So i dont think it is oberheating. 

I installed the firmware for VESC 4.10 and the software says that 2.15 is on my VESC.
Here are my settings of the bldc tool:
[Motor Configuration][3]
[AppConfiguration  General][4]
[AppConfiguration PPM][5]

In a nutshell: 
(1) The speed shouldnt decrease after the half of a ride unless the cutoff is reached. 
(2) The brake and even the torque should be much much higher. 
(3) I should be able to drive twice as long. 
(4) If i accelerate only in the beginning of a ride fully i shouldnt get a drop out? 

I appreciate any help. Just tell me what and how to check and i will do it. 

  [1]: http://www.hobbyking.com/hobbyking/store/__45240__Turnigy_Aerodrive_SK3_6364_213kv_Brushless_Outrunner_Motor_EU_Warehouse_.html
  [2]: http://www.hobbyking.com/hobbyking/store/__64437__Multistar_High_Capacity_6S_8000mAh_Multi_Rotor_Lipo_Pack_US_Warehouse_.html
  [3]: http://fs5.directupload.net/images/160308/mpaancld.jpg
  [4]: http://fs5.directupload.net/images/160308/iucuo3fl.jpg
  [5]: http://fs5.directupload.net/images/160308/a6aslbld.jpg
```

---
## \#5 Posted by: DeathCookies Posted at: 2016-03-08T21:28:16.325Z Reads: 210

```
[quote="NerijusM, post:3, topic:1720, full:true"]
Your VESC is overheating. Same there.
[/quote]
It is in a first aid enclosure and the VESC is getting warm but not hot
```

---
## \#6 Posted by: NerijusM Posted at: 2016-03-08T21:29:54.375Z Reads: 209

```
Take a look on live data in BLDC tool. 
I measured FETS with IR Thermometer. With hands doesnt feel right.
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-03-08T21:34:23.231Z Reads: 214

```
[quote="NerijusM, post:6, topic:1720, full:true"]
Take a look on live data in BLDC tool. I measured FETS with IR Thermometer. With hands doesnt feel right.
[/quote]

Well, i have no IR Thermometer. I did test the heat of the VESC after some rides today and every time it was just warm not hot.
The vesc lays on foam, maybe the foam reflect the heat? 

Also this does not explain that i can only drive about 7 miles / 45 minutes with a 16ah 6s setup. I do only weight 60kg and i drive on flat terrain. Before i drove with a YEP heli ESC and could drive a bit longer with only one ZIPPY FlightMax 8ah 6S battery. It feels so strange...
```

---
## \#8 Posted by: DeathCookies Posted at: 2016-03-09T16:34:43.903Z Reads: 200

```
I reorganized and improved the structure of my first post from this thread. Please take the time and read it again ;) 
Some Feedback and help would make me happy even if you are guessing!
```

---
## \#9 Posted by: Sebastiaan Posted at: 2016-03-09T16:41:42.564Z Reads: 202

```
Can you measure both of the lipo packs seperatly? Just guessing ...
```

---
## \#10 Posted by: DeathCookies Posted at: 2016-03-09T16:49:17.913Z Reads: 207

```
I have in mind that both lipos were depleted equally. But when i am at home i will make another testride and check it  exactly.
```

---
## \#11 Posted by: evoheyax Posted at: 2016-03-09T16:49:36.295Z Reads: 208

```
My guess is you are seeing less range due to inefficient settings in the VESC. Your also running on the short side of the VESC with your battery. 10s+ will mean more torque with less heat.

And it seems you are hitting some limit with heat. At 6s, you pull many more amps, and more heat. With a single drive train at 6s, I can't imagine the VESC staying cool. I burned up 2x 120 amp fvt escs back in the day on a 6s. While the settings had some to do with it, the VESC is rated at half of that, 60a.

**My point is I would recommend putting you lipos in series to get 8ah at 12s.**

More range and less heat, and I think most of your problems would go away.

In terms of the other problems, Weak braking is a sign of bad settings, so is weak torque (though again, 12s torque is much better than 6s torque). You need to learn to configure the VESC with the correct settings in order to get the performance you want.
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-03-09T16:57:03.845Z Reads: 197

```
I had no problems of overheating with the YEP 14S 120a heli Esc running at 6s! Also the VESC does Not get Hot just warm. 

But when i am at home i will solder a series Adapter and try again. 

Bad bldc settings? I just posted pictures of my settings. Which setting is insufficient?
```

---
## \#13 Posted by: trbt555 Posted at: 2016-03-09T17:05:43.107Z Reads: 189

```
You appear to have the motor type set to FOC, are you aware of this ?
Before you do anything else, I would advise you to set the motor type to BLDC and run a motor detection as described in [this][1] thread.
Then do a test ride and report back.

  [1]: http://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500
```

---
## \#14 Posted by: evoheyax Posted at: 2016-03-09T17:23:04.894Z Reads: 196

```
Your YEP 120a esc can run at double the amps (which means it dissipates heat better also). the VESC can only run at 60a constant max.

On 6s, I bet you are hitting that 60 amp limit for most of your ride, which is heating up the VESC.

Remember, more amps = more heat.

You may need closer to 80 or 100 amps constantly with a 6s config.
Higher voltage requires less amps for the same acceleration and speed.
On a 12s config, you may need only 40 or 50 amps constantly, meaning less heat.

However, I had not checked your motor. It seems like your motor is a 10s max, you you will blow out your motor if you run at 12s.

**So do NOT put the in series as I suggested before with this motor**

I would recommenced a motor like the r-spec with the battery at 12s. Alternatively, you can go back to your old esc.

This motor with the VESC would take your board to whole nother level :smile:

http://www.enertionboards.com/electric-skateboard-parts/6374-190kv-electric-skateboard-motor/
```

---
## \#15 Posted by: DeathCookies Posted at: 2016-03-10T06:49:27.678Z Reads: 180

```
I was aware that i have setted up FOC. 
Anyways i did forgot to do a Motor detection...  

Yesterday i made a Motor detection and made another test run. As always i can drive about 30km/h in the beginning but after some time stucked at 20. I also do not have a good acceleration. If i make a Brake and wait for a a moment i can drive fast again.
```

---
## \#16 Posted by: dogeatgod Posted at: 2016-03-10T11:30:49.167Z Reads: 185

```
Low Voltage Cut Off

Link to your battery pack states 22.2V - the start of your low voltage cutoff is 22V

Overheating VESC - suggest :-

Take out of 1st aid enclosure and see if that makes a difference, if it does:-

Heat sink FETS
Install a 5V fan in enclosure

I had similar issue - turned out LV cut off was set too high and also VESC was overheating when enclosed.

<img src="/uploads/db1493/original/2X/7/761517e4da80eaa5ce02e12997a5bfa51694dc6f.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/c/c9b9215f07bca38b95be59b75ddce273fe252558.jpg" width="666" height="500">
```

---
## \#17 Posted by: dogeatgod Posted at: 2016-03-10T14:46:26.025Z Reads: 168

```

My low voltage cut off is set at 33V - 10S2P 8000mAh

I've just skated until LVC kicked in -  measured battery at 35.8V.

Try lowering your LVC to 19.8 and see if it makes a difference.
```

---
## \#18 Posted by: Sebastiaan Posted at: 2016-03-10T15:22:50.814Z Reads: 162

```
Maybe there is a voltage sag under load and the LVC kicks in too soon?
```

---
## \#19 Posted by: dogeatgod Posted at: 2016-03-10T16:42:24.508Z Reads: 164

```
Yes, exactly :smiley:

My settings provide a good LV buffer -  3.58V, can easily limp another mile or so without risk.
```

---
## \#20 Posted by: DeathCookies Posted at: 2016-03-11T07:09:34.568Z Reads: 164

```
I tested to lower the LVC but it does not help.

I will attach a fan to VESC and test it again.
I will keep you guys informed ;)
```

---
## \#21 Posted by: dogeatgod Posted at: 2016-03-11T09:15:57.001Z Reads: 162

```
I'd try just taking it out of the enclosure first.

Perhaps VESC is not the tool for your setup and simply cannot supply constant draw required for the performance you want. The VESC works within your motors parameters whereas your earlier ESC has a 'take it you bitch' attitude - I liked that with mine.

To get performance to a level or greater than that of your earlier ESC, you may, as other posters have stated, need to change motor to lower kV and step up to 10 or 12S. As this requires a significant cash outlay you will need to weigh up pros and cons of doing so.

I do hope that cooling solves your problems.
```

---
## \#22 Posted by: RogerD Posted at: 2016-03-11T13:05:57.816Z Reads: 157

```
Bear in mind when the FETS overheat on a VESC they will be back to normal temperature by the time you feel them (it takes seconds for them to cool back down), unless you can ride with your hand on the VESC. So feeling the VESC after riding isn't a good indicator of heat performance.

All you have to do is take it out of your enclosure and you'll see immediately if you have a heat problem.

6S setups put far too many Amps through VESCs. They are rated at around 60-70Amps. My 6S setup pulls over 100Amps regularly. Hence I use a EZRun Pro car ESC.

When my battery is at 22.8v (your "empty" voltage) - I still have loads to go. 22.9v on mine and I have 4Ah of usable power remaining, leaving a firther 20% as a safetly margin). - That equates to over 4 miles for me. I end up at around 21volts empty.

With @dogeatgod 's board, we had overheating even at 10s, with the correct gearing for 30mph+. Adding a fan has instantly removed the problem. But he's (as am I) heavier than younger riders. Both around 90kg
```

---
## \#23 Posted by: DeathCookies Posted at: 2016-03-11T22:33:56.583Z Reads: 152

```
Thanks for all the nice help!! 
You are right, my VESC was overheating. So i attached a Fan. (Fortunatly i had a sbec for a future light mod with 12v output  :) ) 
Now it is driving like a charm. 
Again Thanks to the supporters, nice forum!! 

 <img src="/uploads/db1493/original/2X/2/25d562106659c0c4a5affb1af1384e82c591450b.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/7/7ddd54868bd8f711c13e1b1d13d0c7f576008d70.jpg" width="375" height="500">
```

---
## \#24 Posted by: dogeatgod Posted at: 2016-03-11T22:42:12.382Z Reads: 140

```
Glad you got it sorted : )
```

---
## \#25 Posted by: trbt555 Posted at: 2016-03-12T08:29:54.489Z Reads: 140

```
If I were you I'd get rid of that foil. It's a short circuit waiting to happen.
```

---
## \#26 Posted by: DeathCookies Posted at: 2016-03-12T13:04:13.644Z Reads: 138

```
I am glad that i get feedback of the foil because i dont know if it was the ideal idea.
Before the vesc lays on Form. Can You maybe give me a Tip what i could use?
```

---
## \#27 Posted by: trbt555 Posted at: 2016-03-12T13:27:01.408Z Reads: 144

```
You already have a heat problem so you want as little thermal insulation as possible, so get rid of the foam as well.
Ideally you should mount the VESC to your enclosure using standoffs so air can reach the underside of the PCB.
You can see the standoffs in this picture:
<img src="/uploads/db1493/original/2X/a/ae77dd4e87ba29c674fe80ba82cf42a3c6a570ed.JPG" width="666" height="499">

To prevent accidental short circuits I'd also advise you to shrink-wrap your VESC but leave the MOSFET visible so they can be cooled.
```

---
## \#28 Posted by: lowGuido Posted at: 2016-03-19T08:02:25.581Z Reads: 140

```
LOL I only just saw this post, and the foil!! 

did you run it like that???? did it even work?
```

---
## \#29 Posted by: DeathCookies Posted at: 2016-03-19T12:39:18.693Z Reads: 133

```
Yes, i drove it one Run like that. About 10km. And yes it worked ;)
```

---
## \#30 Posted by: evoheyax Posted at: 2016-03-19T18:40:05.112Z Reads: 132

```
As has been said, keep ANY conductive surface (i.e. most metals) away from the circuit board. Your very luck it still works after putting it inside of aluminum foil.

I'm glad you got it working with the fan.

Still, I would recommend in the future thinking about upgrading the motor to something capable of running at 12s (like the enertion motor I posted above), and putting the batteries in series to run at 12s. This will likely eliminate the need to have a fan, and will drastically increase torque and top speed. This means you can travel faster, and up steeper inclines. It just makes for a better board.
```

---
## \#31 Posted by: Hummie Posted at: 2016-03-19T19:07:54.378Z Reads: 132

```
I bet ud have no problem running that motor on 12s.  If u rev it to the higher rpm it might be too many computations for the vesc with the high kv though.  

How fragile are the fets?  I have them out of a box exposed to possible flying gravel from the wheels.  Keeps them cool,
```

---
## \#32 Posted by: evoheyax Posted at: 2016-03-19T19:22:24.781Z Reads: 132

```
If you look at the link he posted in the first post, it said the max the motor could take was 10s...
```

---
## \#33 Posted by: Hummie Posted at: 2016-03-19T19:35:44.521Z Reads: 133

```
So it says but it can probably take more. Limited by wire enamel and rpm.  Doubt he'll get near the rpm limit of the bearings. 
More realistic is a max wattage number to determine heat that will degrade the enamel.  But too too high voltage will bust through the ename regardless but that's much more
```

---
## \#34 Posted by: samusaki Posted at: 2016-05-30T05:38:31.967Z Reads: 110

```
Lad, it seems like you don't know much about basic electronics, but you made a working thing and you enjoying it , Great  work !
```

---
