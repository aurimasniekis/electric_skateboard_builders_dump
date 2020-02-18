# How to make a board that reaches 35+ MPH?

### Replies: 117 Views: 4249

## \#1 Posted by: ArmandR Posted at: 2016-08-20T01:06:32.213Z Reads: 445

```
As the title states, I want to make a fast board, would I have to use VESC and 12S? Can anyone recommend any ways to reach those speeds preferably without Hub motors as they don't have much torque or acceleration. thanks.
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-08-20T01:13:19.015Z Reads: 429

```
You'll hit the eRPM limit on the VESC that fast... use a different speed controller. I recommend a torqueboards 12S esc or a car ESC. You can hit a theoretical max of 37mph easily with a 7s battery 20/36 gearing, and 245kv motors with some fairly large wheels 90-100mm
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-08-20T01:15:51.641Z Reads: 423

```
Just play around with this...don't guess 


http://calc.esk8.it
```

---
## \#4 Posted by: Photorph Posted at: 2016-08-20T01:20:10.801Z Reads: 413

```
My belt drive board gets to those speeds.  12s4p, dual R spec, 16/33, 83 mm wheels, chaka VESCs.  Has enough torque still to fly up any hill.  Make those wheels 90mm or 97mm to get close to 40 mph.  

Do the same battery with 116 kv carvon hubs, theoretical max of 57 mph.  Or get 4 of hummies 200 kv hubs and go 60+ mph.  Whatever floats your boat.
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-20T01:27:19.606Z Reads: 390

```
If you're using evolve pulley's its 16/32
```

---
## \#6 Posted by: ArmandR Posted at: 2016-08-20T01:28:21.581Z Reads: 372

```
Yeah I have seen your builds! They fly!!
```

---
## \#7 Posted by: Titoxd10001 Posted at: 2016-08-20T01:31:58.818Z Reads: 371

```
Planning similar. Going to wait for vesc v6. 90mm wheels 15t or 16t motor pulley with 36t wheel pulley on 12s with 190-200kv motor. I go over 30 with v4 vesc but it's risky going over the suggested 60k rpm limit so I'll wait for v6 to go max speed which should be 35mph
```

---
## \#8 Posted by: jrpwit Posted at: 2016-08-20T01:38:47.522Z Reads: 350

```
Simple 12s 190kv does hit erpm limit but shouldn't harm the vesc.
```

---
## \#9 Posted by: Photorph Posted at: 2016-08-20T02:05:58.000Z Reads: 346

```
33 tooth HTD-5M evolve pulley is what for wheel pulley per lhb
```

---
## \#10 Posted by: caustin Posted at: 2016-08-20T02:29:26.104Z Reads: 332

```
Count 'em, 32T
```

---
## \#11 Posted by: anorak234 Posted at: 2016-08-20T02:41:16.948Z Reads: 315

```
You could go cheap (and dangerous) and use a crazy gear ratio... 36:5 :joy:
```

---
## \#12 Posted by: ArmandR Posted at: 2016-08-20T02:45:35.987Z Reads: 308

```
I dont want to kill myself.. :joy: :joy:
```

---
## \#13 Posted by: Skitzor Posted at: 2016-08-20T03:03:14.820Z Reads: 303

```
order one at @longhairedboy :grin:
He proves that 12s4p, enertion R-spec 6355 and vesc are reliable tech !
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-20T03:08:41.174Z Reads: 302

```
well except for the braking problems
```

---
## \#15 Posted by: Photorph Posted at: 2016-08-20T03:23:34.514Z Reads: 303

```
braking problems resolved after VESC settings were adjusting, just needed to throw more current at it.  Now brakes never cut out...but it does brake pretty strong though (which is a good thing I suppose, as long as you don't accidentally tap the joystick backwards cuz that would cause major physical well being issues)

You may be right about the teeth on wheel pulley, maybe LHB made a mistake.  I would have to count them.
```

---
## \#16 Posted by: Kaly Posted at: 2016-08-20T03:43:24.195Z Reads: 299

```
This set up gave me a run for my money

Dual TB 230Kv
Dual TB 12S ESC 
GEAR  16/40
12S Lipo 8000mAh 35C
MBS 100mm AT wheels 

You can even use the http://calc.esk8.it/ to check
```

---
## \#17 Posted by: stuxtruth Posted at: 2016-08-20T03:57:55.785Z Reads: 286

```
This is exactly what you need for 35MPH

https://www.youtube.com/watch?v=fyV2cPLuFuA
```

---
## \#18 Posted by: ArmandR Posted at: 2016-08-20T13:05:37.492Z Reads: 270

```
Is this an offroad setup? Is the torque and acceleration really good?
```

---
## \#19 Posted by: crameur Posted at: 2016-08-20T13:08:51.628Z Reads: 259

```
Can't wait to see the coffinboard!
```

---
## \#20 Posted by: Kaly Posted at: 2016-08-20T13:09:23.842Z Reads: 261

```
It's not off-road, just the mbs 100 wheels 
The torque is really good and acceleration superb. 

I weight 208 lb and this thing handles the load really good.
```

---
## \#21 Posted by: ArmandR Posted at: 2016-08-20T13:10:16.001Z Reads: 247

```
That's actually a great name! I might actually use it if you don't mind.
```

---
## \#22 Posted by: ArmandR Posted at: 2016-08-20T13:11:03.823Z Reads: 252

```
Where did you buy your gears? Like the wheel pulley teeth?
```

---
## \#23 Posted by: Kaly Posted at: 2016-08-20T14:23:35.056Z Reads: 246

```
The pulley I got from here
http://shop.sdp-si.com/catalog/product/?id=A_6A25M040NF1510
You will need to modify the center bore and  drill holes. 

You can check Miami electric skateboards he have 40T plastic ones
```

---
## \#24 Posted by: oriol360 Posted at: 2016-08-20T14:35:43.963Z Reads: 239

```
My board hits 40+ mph
12s
16/36 gearing
250kv motor
My Twin ESC
83 or 90 mm wheels
```

---
## \#25 Posted by: barajabali Posted at: 2016-08-20T16:12:31.889Z Reads: 226

```
Oh man.... You guys are crazy.
```

---
## \#26 Posted by: Mrmoonlight Posted at: 2016-08-20T17:12:18.021Z Reads: 224

```
I tried the V2.5 single and it had torque and acceleration comparable to a belt drive. It felt a bit different since it's a hub, but it held its own. Still need to push start, although if you push your weight in just the right way as you hit the throttle, you don't have to. I'm sure the duals will perform much better when it comes to torque and acceleration and have the higher top speed you want. It may be your solution.

Note that larger wheels and different gear ratios may give you a higher top speed, but you also lose when it comes to torque and acceleration as you make those changes.
```

---
## \#27 Posted by: RunPlayBack Posted at: 2016-08-20T17:29:00.714Z Reads: 214

```
I'm a little surprised at how many people are endorsing going 35+ mph on an eboard without asking why and what for.
```

---
## \#28 Posted by: RogerD Posted at: 2016-08-20T18:00:37.150Z Reads: 210

```
My board has clocked over 35 mph downhill, 32 on the flat.

SK 6354 motor, 6S batteries, EZRun car esc.

You dont' need high voltage, or a Vesc.

I've since geared it down to 20 mph max for obvious safety reasons.
```

---
## \#29 Posted by: oriol360 Posted at: 2016-08-20T18:01:52.189Z Reads: 200

```
Personally I've always wanted to do downhill longboarding but living in miami that's impossible. 
So very fast electric longboards are the next best thing. I just wish it was easier to slide with them.

I also think its like a car.. there are prius and tesla. Some people just always want more speed and power. That translates to just about any vehicle.
```

---
## \#30 Posted by: ArmandR Posted at: 2016-08-20T18:04:08.006Z Reads: 195

```
Your right! I'm in Miami too, so I would love to also get a little of speed. Of course I would ALWAYS wear protective gear.
```

---
## \#31 Posted by: ArmandR Posted at: 2016-08-20T18:05:04.919Z Reads: 189

```
Here in Florida, it's completely flat, so no downhill riding, I love downhill riding, so instead i wanted to make a fast board, while always using safety precautions and gear.
```

---
## \#32 Posted by: Michaelinvegas Posted at: 2016-08-20T18:08:56.136Z Reads: 186

```
Didn't we discuss how falling off at 20+ mph get worse for every 1mph faster you go?
```

---
## \#33 Posted by: ArmandR Posted at: 2016-08-20T18:14:34.748Z Reads: 183

```
Im probably not going to use that speed everyday, I just want to have it if I ever need it to get that adrenaline rush.
```

---
## \#34 Posted by: Michaelinvegas Posted at: 2016-08-20T18:19:20.486Z Reads: 180

```
What you want really is the torque ... The rush to top speed is amazing...yeah running fast is cool sometimes but rather uncomfortable especially if the road isn't meant for it or just too many people or cars around....
```

---
## \#35 Posted by: ArmandR Posted at: 2016-08-20T18:21:19.348Z Reads: 181

```
Yeah I understand, im thinking either 230 or 250 kv with 16/36. And I ride completely flat and im light.
```

---
## \#36 Posted by: Michaelinvegas Posted at: 2016-08-20T18:24:38.673Z Reads: 183

```
It's gonna fly...and I doubt you'll have that trigger pulled all the way for long lol
```

---
## \#37 Posted by: RunPlayBack Posted at: 2016-08-20T18:32:41.768Z Reads: 191

```
Totally, I get it, the adrenaline rush is addicting. With the right safety checklist to minimize risk, it's a blast, and looks like you have em all. But in all honesty, even hitting 25+ on flats will give you a rush. 35-40mph will approach a speed where every part of your build has to be working in perfect harmony and if not, one wrong move could kill you. Trust me I know, a friend recently suffered a traumatic brain injury and almost died on an eboard going about 20mph. Here's a little rundown off the top of my head for practicing top speed runs. 

1. Experience (you'd be surprised at how many people want to hit top speeds with little to no experience on a skateboard or longboard)

2. Environment (empty, smooth asphalt parking lots on weekends, velodromes or closed courses are best)

3. Safety Gear (full face, armor, pads, etc.)

4. Spotter (this one is actually really helpful, these days we always ride with a spotter and communicate through bluetooth intercoms, each person calls out obstacles, cracks in the road, cars, etc. basically watching each other's backs and to keep each other safe)
```

---
## \#38 Posted by: Michaelinvegas Posted at: 2016-08-20T18:36:34.077Z Reads: 185

```
Lol @LEVer said that you and me ride the same @RunPlayBack lol
```

---
## \#39 Posted by: ArmandR Posted at: 2016-08-20T18:37:50.887Z Reads: 184

```
Thank you. Yes, I heard about your friend, I truly hope he is doing much better. I completely understand, I wont be hitting those speeds every day. I will try to use the safest protection and use safety precautions. Thanks again.
```

---
## \#40 Posted by: RunPlayBack Posted at: 2016-08-20T18:38:42.354Z Reads: 176

```
Like stance? I ride goofy...you guys need to do a run on a path without a million people riding through it lol
```

---
## \#41 Posted by: Michaelinvegas Posted at: 2016-08-20T18:39:16.792Z Reads: 169

```
Lol like style

But me no do the stink bug lol
```

---
## \#42 Posted by: RunPlayBack Posted at: 2016-08-20T18:39:50.890Z Reads: 165

```
Hey no prob man, again apologies for getting all "dad-like" just wanna make sure no one gets hurt :slight_smile:
```

---
## \#43 Posted by: RunPlayBack Posted at: 2016-08-20T18:41:30.085Z Reads: 164

```
Hahah yeah I'm gonna go on the record and say I'm unapologetic for the stink bug. I got short legs and it helps me turn better lol
```

---
## \#44 Posted by: Michaelinvegas Posted at: 2016-08-20T18:41:48.663Z Reads: 161

```
He saw a little bit of how I really ride when I tried out his hub
```

---
## \#45 Posted by: Mrmoonlight Posted at: 2016-08-20T18:44:39.313Z Reads: 165

```
So true. A lot of people have no idea what 35mph feels like on a skateboard.  It's exhilerating, but yeah, one wrong move can kill you. Anyone hitting those speeds better have a lot of experience riding fast.
```

---
## \#46 Posted by: Titoxd10001 Posted at: 2016-08-20T19:03:55.625Z Reads: 161

```
What voltage are you thinking?
```

---
## \#47 Posted by: treenutter Posted at: 2016-08-20T19:13:13.051Z Reads: 157

```
@RunPlayBack I was just about to write something similar. Good looking out!
```

---
## \#48 Posted by: treenutter Posted at: 2016-08-20T19:21:10.525Z Reads: 159

```
[quote="Michaelinvegas, post:41, topic:7938"]
stink bug lol
[/quote]

@Michaelinvegas Is the stink bug the full-squat stance? I've been trying it out! It felt weird at first but the low center of gravity is really interesting. I'll start a new thread to talk about riding stances. Esk8 opens up a whole new range of them!
```

---
## \#49 Posted by: Mobutusan Posted at: 2016-08-20T19:23:15.474Z Reads: 162

```
And don't forget the random asshole throwing shit in your path to try to make you SYF. Sad, but true.
```

---
## \#50 Posted by: RunPlayBack Posted at: 2016-08-20T19:56:58.609Z Reads: 167

```
So like in my vids, if you notice how I ride goofy - my low stance is my back heel turned up and back knee turned up with my right knee helping to steer. The lower center of gravity means I can go faster with little wind resistance. So when I turn a hard right I'll grab the board with my left hand. When I turn left I'll throw my left on the ground with a sliding glove to give me another point of contact on the turn and to provide a little friction without having to use brake. It's a little weird technique and is kind of like stink bug on a longboard but because I favor my right hand on the controller and I'm not really riding on soft wheels and I'm not sliding, it makes sense and I actually feel safer. It's not for everyone but it works for me.

http://runplayback.com/wp-content/uploads/2016/06/IMG_9800.jpg
```

---
## \#51 Posted by: Michaelinvegas Posted at: 2016-08-20T21:15:09.685Z Reads: 155

```
Hahah I remember that .... 

That's fucked up hahahh. True story lol
```

---
## \#52 Posted by: Michaelinvegas Posted at: 2016-08-20T21:19:43.424Z Reads: 155

```
See you guys are getting down....

I stand up but I use my hands and hips to flare around corners like snowboarding .... Hence how I ride .... I'm pretty animated when I get groovin' on twisties .... I feel if I get down...something happens like a wheel breaks loose...I won't have time to get up and run it off and save myself...
```

---
## \#53 Posted by: anon33082420 Posted at: 2016-08-20T21:28:22.633Z Reads: 151

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#54 Posted by: Michaelinvegas Posted at: 2016-08-20T21:43:00.874Z Reads: 150

```
Lol @RunPlayBack can be my partner in doubles lol
```

---
## \#55 Posted by: ArmandR Posted at: 2016-08-20T22:29:25.511Z Reads: 154

```
12s Li-ion!
```

---
## \#56 Posted by: Namasaki Posted at: 2016-08-20T22:59:10.161Z Reads: 153

```
You should include rider weight in your calculations.
140lb rider vs  180lb ride makes a world of difference.
```

---
## \#57 Posted by: Michaelinvegas Posted at: 2016-08-21T01:13:50.040Z Reads: 157

```
This would be an instance for the use of a stink bug move... Lol .... But rare you would slide .... No need to if you have brakes ... 

I feel standing up, digging and positioning the body and arms is just as effective in helping you make those turns that would you otherwise not make 

But to each thier own...can't wait to get in a race league and run through courses .... We'll be playing for board pink slips lol

https://youtu.be/xxm6sFSOh5Y
```

---
## \#58 Posted by: Titoxd10001 Posted at: 2016-08-21T02:31:00.104Z Reads: 160

```
I think that's to high of a kv unless you want to go faster than 40mph. 190-200kv would be good imo something about efficiency. Just look at @Photorph board that lhb built. And vesc v6 should be coming out this year hopefully and should be worth the wait.
```

---
## \#59 Posted by: evoheyax Posted at: 2016-08-21T07:02:04.548Z Reads: 164

```
I'm almost done a build of a 4wd hub motors with 4x VESC with a custom 10s4p battery. I'm estimating I should be able to do 28 mph, with pretty good torque. Hubs can have good torque, but they need to be a lower kv. The carvons can do 35 mph no questions asked. But torque at 149 kv sucks, it's too high for any sort of hills. With hummies 80 kv, torque is good. I'm exited to see what 4wd feels like.

12s I feel is important. I would do 12s right now if I had space for more batteries.

I think the best way to achieve this comfortly is to through more motors on the board. You want torque and speed and it's the classic battle I think ever builder has had or is having.

I think hubs are simpler and can have great torque in speed. But you need more of them to make up for the lack of gearing.
```

---
## \#60 Posted by: anon33082420 Posted at: 2016-08-21T07:51:48.183Z Reads: 165

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#61 Posted by: evoheyax Posted at: 2016-08-21T16:42:43.950Z Reads: 169

```
Oh, I know. I'm curious as to how they feel in comparison to the 149 kv. I'm about 200 lbs, and with hummies 80 kv motors, I have great torque. With his 90 kv motors, I have close to the same torque, a few mph higher. I'm combining the 2x 90kv with 2x 80 kv right now, which should blend to 85 kv. The difference are his wheels are 83mm. You use 90mm, which has a higher top speed, but you'll lose a bit of torque at that cost. I'm trying to create a board with as much torque as a good belt setup.

I;m really temped to send my carvons back to get the 85kv. But I'm even more curios as you how my torque would change if I did a 4wd of the 149 kv's. I'd like to have a super high top speed board, in addition to a more efficent board that's more practical for city commuting.

@LEVer is it possible to get my carvon v2 sensored by you? It's really only that first 0-10 mph that lacks torque with the 149 kvs. Once your at 20 especially the toqrue on up is insane.
```

---
## \#62 Posted by: iWackett Posted at: 2018-10-29T23:46:21.920Z Reads: 96

```
Hey man 

I have been reading a few of your posts and I have a task I need some guidance with if possible please. I have a Evolve Carbon GT and I love it but I want a board that goes 30mph plus with AT MBS 8 inch roadie tires. I want to strip the guts out of my evolve board and put new more powerful motors and all new electronic Parts. I know I won’t be be able to use any existing inner parts so I would love to know what you would use in terms or motors and parts if you had to rebuild this board as a Frankenstein street sleeper. 

I appreciate any help. Cheers man
```

---
## \#63 Posted by: curtis Posted at: 2018-11-04T19:06:56.996Z Reads: 82

```
That calculator doesn't make any sense. How can making the gear ratio so the motor gear is bigger make the board go twice as fast?
```

---
## \#64 Posted by: psychotiller Posted at: 2018-11-04T19:11:22.564Z Reads: 87

```
The calculator works perfectly.
```

---
## \#65 Posted by: brenternet Posted at: 2018-11-04T19:16:12.325Z Reads: 87

```
This is a 2 year old necro thread guys :rofl:
```

---
## \#66 Posted by: Indiangummy Posted at: 2018-11-04T19:27:02.954Z Reads: 90

```
Ohh Curtis....
```

---
## \#67 Posted by: ArmandR Posted at: 2018-11-04T19:27:36.895Z Reads: 90

```
jeez haven't been here in a while...
```

---
## \#68 Posted by: curtis Posted at: 2018-11-04T19:38:59.819Z Reads: 92

```
Theoretically I could go faster then airplanes if I did this setup.![gearing%20ratio|690x338](upload://3RED99kKMEVCssp5bvNTRY1IsyL.png)
```

---
## \#69 Posted by: Indiangummy Posted at: 2018-11-04T20:01:45.722Z Reads: 89

```
Yeah give it a shot.
```

---
## \#70 Posted by: Indiangummy Posted at: 2018-11-04T20:04:33.649Z Reads: 92

```
Read this if you actually want to learn 
https://www.vexrobotics.com/vexiq/education/iq-curriculum/mechanisms/gear-ratio
```

---
## \#71 Posted by: Scream Posted at: 2018-11-04T20:54:53.309Z Reads: 91

```
I think of it like this...

If your motor pulley has 15 teeth, and your wheel pulley has 36 teeth, this means one rotation of your motor pulley will turn your wheel pulley 15/36ths (or 5/12ths) of a full rotation... a bit UNDER half a rotation.

If you increased your motor pulley to 20 teeth, one rotation of the motor pulley would turn your wheel pulley 20/36ths (or 5/9ths) of a full rotation... a bit OVER half a rotation.

So once both motors meet their maximum rpm (revolutions per minute) - which set up do you think will be going faster? Answer: the one with the 20t motor pulley, as it will create more rotations of the wheel pulley in the same time.

Of course the 20t set up will require the motor to work harder to reach max rpm... so there’s a limit to how far you can push that calculation. Your 1000mph setup won’t actually work because a 360kv motor isn’t going to handle that kind of torque. And if you tried to put a 5t wheel pulley on a 90mm wheel, the belt would almost certainly slip (think of trying to turn a large screw with too small of a screwdriver).
```

---
## \#72 Posted by: professor_shartsis Posted at: 2018-11-04T21:41:28.864Z Reads: 92

```
[quote="curtis, post:68, topic:7938"]
Theoretically I could go faster then airplanes if I did this setup.
[/quote]

https://image.ibb.co/ghGoQ0/1b173741604d48004467b5266ec42002f536a8cb.png

https://image.ibb.co/cG5Xk0/1000mph.jpg

@curtis unloaded (board upsidedown w/ no rider) and ignoring bearing losses, the edge of the wheel can go that 1000mph speed if the wheel/drivetrain can handle the centrifugal force, but with the total 3 lbs thrust @ 80a motor current with 2 motors and the wind drag of a rider, in reality, loaded with a rider you'll only get about 15mph top speed on flat ground with that setup...

https://image.ibb.co/kAD7JL/1000mph-2.jpg
```

---
## \#73 Posted by: Skunk Posted at: 2018-11-04T22:00:57.492Z Reads: 86

```
This was a funny read.
I love threads frpm 2016.
Watching people talk about 35mph like its some next level sh**. 
Times have changed.
```

---
## \#74 Posted by: professor_shartsis Posted at: 2018-11-04T22:07:33.578Z Reads: 87

```
@curtis try a no load test with that kv & gear ratio (with appropriate safety goggles) & you'll probably witness your wheel do something like this:

https://youtu.be/n-DTjpde9-0

https://youtu.be/zs7x1Hu29Wc
```

---
## \#75 Posted by: curtis Posted at: 2018-11-05T02:51:36.815Z Reads: 87

```
No I understand it, but I think it's stupid to think that changing the gear ratio can make the motor go faster than a commercial airplane.
```

---
## \#76 Posted by: Lunasi Posted at: 2018-11-05T03:35:20.642Z Reads: 88

```
Personally I'd do a single motor 6355, 6374 or 6380 on a 12s battery with a 16-36 gear ratio to hit that 35+
```

---
## \#77 Posted by: Boardnamics Posted at: 2018-11-05T04:03:40.829Z Reads: 88

```
It won't....it just will in theory.

It's power that will give you that speed. Assuming no losses at all you actually would get to 1000mph but it would take a very long time still.

Please don't try that ratio...
```

---
## \#78 Posted by: J0ker3366 Posted at: 2018-11-05T04:05:46.553Z Reads: 88

```
40+mph 

Single 6374 195kv
Focbox
16/36
12s
100mm
```

---
## \#79 Posted by: curtis Posted at: 2018-11-05T05:06:58.555Z Reads: 86

```
I defiantly understand. I don't know how many times I have to say that calculator calculates how fast it would go in theory. If you don't account for gravity, a rider, wind resistance, or even heat.
```

---
## \#80 Posted by: curtis Posted at: 2018-11-05T05:10:08.188Z Reads: 86

```
Wouldn't it be smarter to have 2 motors if your going to be going that fast? Actually no you are trading stability for speed.
```

---
## \#81 Posted by: J0ker3366 Posted at: 2018-11-05T05:38:20.678Z Reads: 84

```
No I'm not. I'm very stable @ 40+. Don't believe me?

2000 South Colorado Blvd
Denver, Co. 80203

You cone ride it any time you want. Until then, please don't assume one board is like another. Because you would be sadly mistaken.
```

---
## \#82 Posted by: moone Posted at: 2018-11-05T05:45:21.317Z Reads: 82

```
I'm coming to stay! ❤
```

---
## \#83 Posted by: Michaelinvegas Posted at: 2018-11-05T07:06:07.105Z Reads: 86

```

[quote="curtis, post:63, topic:7938, full:true"]
That calculator doesn’t make any sense. How can making the gear ratio so the motor gear is bigger make the board go twice as fast?
[/quote]

[quote="psychotiller, post:64, topic:7938, full:true"]
The calculator works perfectly.
[/quote]

[quote="brenternet, post:65, topic:7938"]
This is a 2 year old necro thread guys :rofl:
[/quote]
![image|220x220](upload://5bGEriAEdVtjInNCOuNz9yPistP.gif) 

What’s up....gees  fell asleep for a minute 

[quote="curtis, post:68, topic:7938"]
Theoretically I could go faster then airplanes if I did this setup.
[/quote]

So fast in fact you can go back to the future 

https://youtu.be/Roy_RtMhiHo

[quote="Skunk, post:73, topic:7938, full:true"]
This was a funny read.
I love threads frpm 2016.
Watching people talk about 35mph like its some next level sh**.
Times have changed.
[/quote]

38mph next level shit
https://youtu.be/K-X3e12mlMU


.....


I have no idea what is happening im just throwing random stuff up on this two year old thread
```

---
## \#84 Posted by: curtis Posted at: 2018-11-08T23:31:42.953Z Reads: 72

```
How much power would people say that you need for a setup like the original thread? to make a board that goes? 35+ mph.
```

---
## \#85 Posted by: professor_shartsis Posted at: 2018-11-08T23:50:24.000Z Reads: 72

```
[quote="curtis, post:84, topic:7938, full:true"]
How much power would people say that you need for a setup like the original thread? to make a board that goes? 35+ mph.
[/quote]

35mph on flat ground: ~1055w mechanical
35mph on 5% slope: ~1750w mechanical
35mph on 10% slope: ~2440w mechanical
35mph on 31.5% slope: ~5237w mechanical

add roughly somewhere between 100w - 1000w copper loss or so to get the electrical wattage
```

---
## \#86 Posted by: curtis Posted at: 2018-11-09T00:51:03.570Z Reads: 67

```
cool. Now what about if you have 2 180 kv motors.
```

---
## \#87 Posted by: mmaner Posted at: 2018-11-09T01:07:56.826Z Reads: 66

```
![Screenshot_20181108-190434_1541725645165|690x398](upload://qoFsAGfBs6IqoXNKzazomQLilfY.png)
```

---
## \#88 Posted by: professor_shartsis Posted at: 2018-11-09T01:14:47.538Z Reads: 66

```
[quote="curtis, post:86, topic:7938, full:true"]
cool. Now what about if you have 2 180 kv motors.
[/quote]

you could do pretty close to 35mph up a 31.5% grade (yellow line, bottom left chart, vehicle thrust pounds, 2 motors) assuming:

(2) 180kv motors, 0.05ohm,  83mm tire, 28T wheel, 15T motor, 1.86:1 gearing, 80a motor current limit, 60a battery current limit per motor, 46v battery after sag


https://image.ibb.co/dydvXq/35mph.jpg
```

---
## \#89 Posted by: Battosaii Posted at: 2018-11-09T01:25:48.240Z Reads: 58

```
Easy way to go 35+? Use 107mm wheels and 12s you will reach that with most gear ratios lol
```

---
## \#90 Posted by: professor_shartsis Posted at: 2018-11-09T01:31:56.151Z Reads: 65

```
@curtis @Battosaii  yes, with 107mm tire, you could do 38T wheel 15t motor, 2.53:1 gear for similar results:

https://image.ibb.co/fan8JV/35mph-2.jpg
```

---
## \#91 Posted by: chaka Posted at: 2018-11-09T02:33:13.849Z Reads: 64

```
@Wallgreeens has said he can reach 38 mph on his FreeRide. Its a 12s build with 16/36 tooth drive on 90mm wheels. I have a similar build but i have been running 16/ 32 tooth on my drive and I regularly clock in around 43 mph but I am tucking as much as I can. Motors lack a lot of torque when they pass 80% duty cycle so I need to tuck hard to get that last bit of top speed. Both builds are running 200kv motors.
```

---
## \#92 Posted by: Skunk Posted at: 2018-11-09T02:41:27.396Z Reads: 63

```
[quote="Battosaii, post:89, topic:7938"]
107mm wheels and 12s
[/quote]

Not me.... topping at 33mph.
16t-40t
Acceleration is nuts tho 
Swapping  to 36t on my wheels soon.
```

---
## \#93 Posted by: accrobrandon Posted at: 2018-11-09T02:45:40.547Z Reads: 60

```
This was a good read as I was curious about the mechanics of things... However... Numbers aside is there any advantage of changing the gearing on the wheel vs motor... Like yeah the ratio can be tuned regardless up or down but does changing it at one location offer any benefits vs the other?
```

---
## \#94 Posted by: professor_shartsis Posted at: 2018-11-09T02:46:37.356Z Reads: 62

```
[quote="accrobrandon, post:93, topic:7938"]
However… Numbers aside is there any advantage of changing the gearing on the wheel vs motor… Like yeah the ratio can be tuned regardless up or down but does changing it at one location offer any benefits vs the other?
[/quote]

changing the # teeth on the motor pulley generally has a larger effect on the gear ratio per tooth changed than changing the same # teeth on the wheel pulley.
```

---
## \#95 Posted by: accrobrandon Posted at: 2018-11-09T02:51:13.188Z Reads: 62

```
Thanks just what I was looking to hear =)
```

---
## \#96 Posted by: mmaner Posted at: 2018-11-09T02:52:26.962Z Reads: 62

```
I'm running 20/44 on 12s eith 107s and I hit 35 today with some throttle left.
```

---
## \#97 Posted by: chaka Posted at: 2018-11-09T02:53:09.433Z Reads: 64

```
Most guys around here wont like this but my board is now running 76mm wheels and it feels way more powerful than when i was spinning massive 90mm wheels. Dont get me started on how much embodied energy us in a 107.
```

---
## \#98 Posted by: professor_shartsis Posted at: 2018-11-09T02:55:26.759Z Reads: 62

```
90mm/76mm=1.18.. or about 18% more acceleration
```

---
## \#99 Posted by: chaka Posted at: 2018-11-09T03:00:55.861Z Reads: 61

```
True but the board handles much better and out accelerates another board we have that has a similar top speed with 90s.
```

---
## \#100 Posted by: Battosaii Posted at: 2018-11-09T03:01:47.688Z Reads: 63

```
Some people like the comfort of big wheels and with some crazy set ups today power is not an issue. I hope to get my 6 shooters up to 50mph with my new set up.
```

---
## \#101 Posted by: professor_shartsis Posted at: 2018-11-09T03:01:57.009Z Reads: 60

```
i meant the 76mm should have 18% more peak acceleration compared to the 90mm
```

---
## \#102 Posted by: chaka Posted at: 2018-11-09T03:04:14.283Z Reads: 60

```
Just remember that those big wheels are heavy and if the board starts getting wobs it is way harder to get them back under control compared to a lighter wheel.
```

---
## \#103 Posted by: Battosaii Posted at: 2018-11-09T03:06:02.288Z Reads: 60

```
That's true, we shall see if that ever happens. I have yet to get a speed wobble on my Evo but I have the trucks dialed in perfect for me :).
```

---
## \#104 Posted by: mmaner Posted at: 2018-11-09T03:10:59.435Z Reads: 61

```
That makes perfect sense to me.  The problem, at least for me, is the shit-tastic roads with pebbles all over. Bugger wheels means less chance of a sudden stop, as in the roll over capability is higher the bigger the wheel.
```

---
## \#105 Posted by: chaka Posted at: 2018-11-09T03:18:14.923Z Reads: 63

```
Yeah but i have noticed that at these speeds I just blow through the rough stuff same as a larger wheel. In fact the wider lip on the smaller wheels feels more stable in the rough patches but this is only in my experience.
```

---
## \#106 Posted by: mmaner Posted at: 2018-11-09T03:20:38.968Z Reads: 66

```
Maybe it's a difference in topological conditions because I've seen the opposite. We have lots of asphalt, which is great when it's new but turns into a frikkin runics cube of obstructions.
```

---
## \#107 Posted by: chaka Posted at: 2018-11-09T03:32:15.107Z Reads: 65

```
Checkout this video, these guys are probably running a max wheel size of 73 mm on some of the worst pavement in SoCal. Usually a harder duro than us as well. In this race it looks like they top out around 35 mph. Some of these riders also do world record events. During the WR events some guys run big wheels but the roads are buttery smooth anyway. Now that I am venturing back to a standard size for DH riding I am starting to see some of the drawbacks of really big wheels at high speed. It could be the wider contact patch, at this point I'm not really sure. @MoeStooge has the right idea on going big without a lot of weight. Heavy wheels feel like they want to bounce a lot when I hit rough patches at high speed.

https://youtu.be/s7OW7hieOeU
```

---
## \#108 Posted by: mmaner Posted at: 2018-11-09T03:42:37.310Z Reads: 65

```
I think something like centrax wheels, ultra wide (77mm I think) with a solid core might be a have changed.
```

---
## \#109 Posted by: Frenchy Posted at: 2018-11-09T03:43:22.796Z Reads: 68

```
Finally some one to back me a bit . I've been saying the same. 90 max. I'm not into the Tonka truck wheels. I want lighter boards to be like my DH and pusher boards that are nimble as fuck. ill lose 2 to 3 pound easy changing from abec 11 97 to 85 seismic speedvents when @PXSS helps me out.. I think we need your 76mm sooner @chaka
```

---
## \#110 Posted by: chaka Posted at: 2018-11-09T03:56:28.199Z Reads: 68

```
I used to race mtbikes in my younger days, I would train on relatively heavy wheels, slime ect.. On race day I would run my race wheels which were very light. The effect was similar to using weights on a bat to warm up in baseball. Rotational weight plays a huge role in performance.

 FYI, you can find 76mm wheels now but they need to be modified a little to fit most drives and that is why we are working to have another option made ;)
```

---
## \#111 Posted by: Frenchy Posted at: 2018-11-09T04:08:00.567Z Reads: 67

```
I'm not to familiar with the belt set up or gear I'm still new to this game .. I've only bought pre built hub not know of the diy game till this year and i built a speeddrive this year..so only familiar with hubs drives really but ive been riding skatboards for 25 years and just got into this eskate I'm just gonna save up for your sweet katana set up and wait patiently for you to release the goods as I've been reading and watching and your gear is killer @chaka. I loved my old cronin back on the day
```

---
## \#112 Posted by: chaka Posted at: 2018-11-09T04:16:19.210Z Reads: 68

```
Thanks @Frenchy I am a big proponent of an adjustable drive, now more than ever as I tune my boards for the upcoming race. No sense in having a board that reaches insane speeds if the course won't allow it. Being able to use a combination of wheel sizes and drive ratios is going to be key to winning in years to come.
```

---
## \#113 Posted by: Frenchy Posted at: 2018-11-09T04:26:38.479Z Reads: 66

```
This is 100 % true I use to race quads and my yamaha banshee I had a three different tires sizing for different tracks ..smaller tighter tracks I ran smaller tire with a larger paddle tread and larger wheel with smaller paddle on jumping tracks ..then I had my x cross tires for wooded tracks
```

---
## \#114 Posted by: Mikenopolis Posted at: 2018-11-09T04:44:42.108Z Reads: 71

```
18/36 12s 107mm. I got to 34mph and I didn’t “floor it” yet. No idea how some people regularly go that fast. 
![image|690x485](upload://j65PDgc6mBJVVGv1MbFZ1Jkmr4O.jpeg)
```

---
## \#115 Posted by: skatardude10 Posted at: 2018-11-09T08:03:20.241Z Reads: 69

```
When I had my board setup to 20/32, 107mm superflys and 10S I got up to 48.9mph and wobbed out... 35 is easy... But I don't try to go faster than 40 these days, so 20/36/107mm/10S has been serving me well. Reach 40 mph easy with a little headroom left if I'm feeling crazy.
```

---
## \#116 Posted by: curtis Posted at: 2018-11-10T05:59:03.004Z Reads: 64

```
Ok. so with 2 motors it wouldn't use more power?
```

---
## \#117 Posted by: Wallgreeens Posted at: 2018-12-26T11:26:41.842Z Reads: 48

```
38.7 mph on flats bro.  Don't skimp me out of my .7 mph.
```

---
