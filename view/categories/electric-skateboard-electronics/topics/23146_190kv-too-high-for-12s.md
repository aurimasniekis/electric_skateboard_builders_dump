# 190kv too high for 12s?

### Replies: 77 Views: 5712

## \#1 Posted by: thisguyhere Posted at: 2017-05-15T21:57:01.629Z Reads: 450

```
i'm sure we've all read through this already: https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125

i'm still conflicted on whether a 190kv motor would be ok for a 12s pack?  or drop down to 170kv?
```

---
## \#2 Posted by: JLabs Posted at: 2017-05-15T21:59:12.332Z Reads: 436

```
Technically you can use a 190kv if you limit the ERPM L, but get 170kv if available.
```

---
## \#3 Posted by: torqueboards Posted at: 2017-05-15T22:09:54.100Z Reads: 429

```
We use 12S with 190KV and have no issues. As JLabs mentioned just set ERPM to -60/60k and uncheck the apply negative torque option. You can always down gear to 13/36 or 16/40 as well.
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-05-15T22:13:26.210Z Reads: 425

```
got ya, not sure where but i read the erpm limitation doesn't just limit the erpm, but the power just drops off?  that would be a bit alarming, especially at full speed.

anyway, @torqueboards i'm going to place the 218mm trucks on order now and if i include two 6355 190kv motors in the same order, can you ship them together?  i'm in no rush to get them, just putting stuff together for next build.
```

---
## \#5 Posted by: torqueboards Posted at: 2017-05-15T22:15:06.789Z Reads: 399

```
@thisguyhere - Yeah, sure. We'll combine them.

Unless, you plan on going 30-35mph.. I don't think you'll hit the ERPM limit. I haven't hit. Maybe someone has more info on that.
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-05-15T22:16:05.392Z Reads: 383

```
yea true, i'm already in full freak out mode when it gets to like 20mph so this shouldn't be an issue.

cool, you should see an order come through in a bit.

thanks!
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-16T00:50:46.881Z Reads: 355

```
Yea from what I've heard it's a hard stop. There's a soft eRPM limit you can configure in app configuration, however.
```

---
## \#8 Posted by: Mikeomania12 Posted at: 2017-05-16T01:16:43.416Z Reads: 342

```
Whoa doesn't sound good... Wtf is a hard stop? Like throw u off the board?
```

---
## \#9 Posted by: Namasaki Posted at: 2017-05-16T03:29:18.690Z Reads: 328

```
[quote="Jinra, post:7, topic:23146"]
Yea from what I've heard it's a hard stop.
[/quote]


Doesn't unchecking the "use negative torque" box eliminate that?
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-16T03:35:33.569Z Reads: 325

```
I guess it would! I never used it before but I'll have to soon with my 10s 230kv setup.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-05-16T05:07:20.215Z Reads: 312

```
Still, I would think that hitting the erpm limit while accelerating would at least be like releasing  the throttle suddenly which could be enough to throw some riders.
I think the best thing to do is to build below the erpm limit and then no worries.
```

---
## \#12 Posted by: pennyboard Posted at: 2017-05-16T05:44:33.939Z Reads: 312

```
I have a 12s 192kv setup, with 13/36 gearing. It's worked great for the last 6 months. (Until I blew up my sk3 motor last Saturday but that's another story haha). The fastest I've got it is 30mph, theoretically it should be going 32, but I figure 30 is the fastest I'll get when I take losses into account. So you should be fine doing 12s 190kv. 

@torqueboards, do you think I would be hitting the ERPM limit in that set-up though? My roommate has the same thing just with 16/36 gearing so it should be getting like 35 mph but we've only ever got it up to 30 mph. Now I'm wondering if that's the ERPM of lack of necessary power to hit that speed.
```

---
## \#13 Posted by: markyoe Posted at: 2017-05-16T16:36:57.225Z Reads: 297

```
Here's my possible setup:
10s4p pack
VESC
245kv motor
17T motor pulley to 36T wheel pulley 

From your guys' experience, is that a recipe for disaster?
Will limiting the ERPM to 60k and unchecking negative torque for my VESC in the BLDC tool protect me from being thrown off my board if I surpass the ERPM limit? In other words, what would happen if I surpassed the limit?
```

---
## \#14 Posted by: pennyboard Posted at: 2017-05-17T01:45:50.450Z Reads: 292

```
That's gonna have way too much top speed and not enough low end torque. Your top speed with that set-up would be around 41 mph (if your motor has enough power to get you up to 41 mph). 

Why not just do 10s4p, 190kv motor, and 13/36T gearing? That'll give you a top speed of around 25 mph and lots of low end torque.
You could even switch out the 13/36T gearing for 16/36T to go a little faster (around 30 mph).

Unless you're trying to hit really high top speeds there's no point in having a 10s battery, 245kv and 17/36T gearing. Most people do 10s or 12s battery, 190kv motor, and then adjust the gearing to get desired top speed.
```

---
## \#15 Posted by: markyoe Posted at: 2017-05-17T02:03:11.910Z Reads: 284

```
Ok, thanks for the info. I didn't think about low end torque. I already had a 245kv motor, but I can buy a 190kv and I'm stuck with a 17/36 ratio right now.

Does it matter which one of these I get? Is there a big advantage to the pricier one?
diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/

diy-electric-skateboard-kits-parts/motor-6374-190kv-3150w/
```

---
## \#16 Posted by: pennyboard Posted at: 2017-05-17T02:07:43.598Z Reads: 264

```
No problem. Having 17/36T ratio is fine. One of my boards uses the more inexpensive motor of those two and has 16/36T, so almost the same as yours. It can accelerate fine and climb moderately steep hills, so you should be fine with the cheaper one. The only difference between the two is that the cheaper one is less powerful (2500 watts vs 3150 watts for the more expensive one). 
You can also buy a 13T pulley to replace the 17T from that same site for something like $15, so you aren't really stuck with 17/36T if you want low end torque or hill climbing ability.
```

---
## \#17 Posted by: markyoe Posted at: 2017-05-17T02:30:13.670Z Reads: 252

```
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

Better alternative to the $90 diyelectric one, or nah?
```

---
## \#18 Posted by: pennyboard Posted at: 2017-05-17T02:45:19.226Z Reads: 248

```
I'd say no. That's the exact motor on my main board. I've had a few problems with it, the first is that it doesn't have a key shaft cut into the motor shaft so you have to file down the shaft and use a set screw as a keyway, I otherwise the drive pulley just slips on the motor shaft. Also it seems to get a lot warmer than the diyelectric one I have on my other board while climbing the same hill, I'm not sure why. 
And by the time you pay for shipping it'll be about the same price, as the diyelectric one. 

However, it is more powerful and slightly cheaper, so if that's something you really value then go for it, but in my opinion, if I had to buy a motor all over again, I'd just get the diyelectric one.
```

---
## \#19 Posted by: Titoxd10001 Posted at: 2017-05-17T02:50:35.769Z Reads: 249

```
This is a good tool to know if you'll reach the 60k erpm. If you do a lot of downhill riding you might exceed safety limit

https://scottkellum.github.io/Esk8-RPM-finder/
```

---
## \#20 Posted by: thisguyhere Posted at: 2017-05-17T02:53:55.811Z Reads: 263

```
keep in mind also you'll only be fit one 6374 motor per truck.

if later on you want to go dual, it'll either have to be diagonal, or criss-cross drive.

i ran dual 6374 in diagonal when i started, and even though the power was incredible, it was generally a pain in the ass to maintain.

setting up for a dual rear 6355 setup at the moment.
```

---
## \#21 Posted by: markyoe Posted at: 2017-05-17T02:56:33.173Z Reads: 251

```
In the speed limit box, I put the potential highest speed I will go?

@thisguyhere good to know, thanks!
```

---
## \#22 Posted by: Titoxd10001 Posted at: 2017-05-17T03:04:54.981Z Reads: 248

```
Yeah, put the highest top speed you'll reach (even downhill speed) or you can up the speed till you get to 60k to know your safety limit
```

---
## \#23 Posted by: markyoe Posted at: 2017-05-17T04:23:13.910Z Reads: 240

```
Do I have a gear ratio of 2.18 with a 17T motor pulley and 36T wheel pulley? If so, my top speed can be 39mph before I break 60k ERPM.. there's no way I'll even go that fast even downhill. Are my calculations incorrect?
```

---
## \#24 Posted by: Titoxd10001 Posted at: 2017-05-17T04:39:03.938Z Reads: 234

```
That is correct (2.118). The less reduction you have, the harder it is to reach higher erpm. Hubs are 1:1 and have low erpm. The calculator is for for standard 7 poles.

If you spin the motors max throttle on bench you may have problems though so don't do that
```

---
## \#25 Posted by: Eboosted Posted at: 2017-05-17T05:04:20.709Z Reads: 229

```
Why not just buy a 15T pulley from @Titoxd10001 and keep the 37T drive pulley? 

I used 10S4P on 190KV motors and 16/36Y pulleys and for me it's the perfect combination. 

On the other hand I'm building a Trampa on 12S4P, dual 190KV, that setup should hit 59,052 ERPM, 30MPH on 85% efficiency. I think that's going to be the sweet spot, perfect setup for the 4.12 VESC
```

---
## \#26 Posted by: Jinra Posted at: 2017-05-17T05:08:46.516Z Reads: 218

```
technically, 63680 eRPM on that setup. Though you may not reach full voltage duty cycle, a bit of decline could kick it over eRPM.
```

---
## \#27 Posted by: pennyboard Posted at: 2017-05-17T05:31:26.143Z Reads: 216

```
Yep, you literally described my exact situation right now. I started off with a single 6374, and this summer I'm planning to go dual rear 6355, for more power and less wheel and belt slippage.
```

---
## \#28 Posted by: markyoe Posted at: 2017-05-17T05:38:50.013Z Reads: 212

```
What 190kv motor do you have? @pennyboard is right about having low end torque with my 245kv setup but I can't decide if the more expensive motor from diyelectric will be needed. I'm only 135lbs...
```

---
## \#29 Posted by: Eboosted Posted at: 2017-05-17T05:46:11.816Z Reads: 213

```
I'm using the electric skateboard calculator:

<img src="/uploads/db1493/original/3X/d/a/da4df3530c52765997fcc85c9bdd059932ece789.png" width="367" height="500">

8436 RPM x 7 pair of poles = 59052 eRPM

How are you getting 63680 eRPM?
```

---
## \#30 Posted by: Jinra Posted at: 2017-05-17T05:47:40.465Z Reads: 202

```
Basing it off max theoretical voltage.

50.4v * 7 pole pairs * 190kv * .95 max duty cycle = 63,680
```

---
## \#31 Posted by: Eboosted Posted at: 2017-05-17T05:49:32.701Z Reads: 206

```
[quote="markyoe, post:28, topic:23146"]
What 190kv motor do you have?
[/quote]

I have the 6374 190kv 3600W motor from @kaly and I also use the 6355 190KV 2500W motor from @torqueboards
```

---
## \#32 Posted by: markyoe Posted at: 2017-05-17T05:50:50.352Z Reads: 209

```
Being that one is 3600W and one 2500W, have you seen much of a difference in the torque?
```

---
## \#33 Posted by: Eboosted Posted at: 2017-05-17T05:52:28.586Z Reads: 207

```
I haven't used that formula before but the electric skateboard calculator usually gives me a consistently exactly the eRPM number I get on the board in real life.
```

---
## \#34 Posted by: Eboosted Posted at: 2017-05-17T05:55:21.795Z Reads: 204

```
I really hope so, it's a lot of difference, theoreticaly I should get more than 40% of additional power, way more torque and crazy acceleration, as I'm jumping from dual 6355 to dual 6374.
```

---
## \#35 Posted by: Jinra Posted at: 2017-05-17T06:03:21.580Z Reads: 200

```
It's the same math
```

---
## \#36 Posted by: pennyboard Posted at: 2017-05-17T07:16:50.136Z Reads: 196

```
I'm 165 lbs and I've carried another person on my back while riding that board (so over 300 lbs) and the motor was able to handle it and even carry us up a slight incline, so I think you should be alright with the lower power motor.

But honestly, it's $30 more, which isn't much in the grand scheme of the entire cost of your board, so if you're really worried about it, just go for the more powerful one. Just make sure you want don't want to get dual rear motors later cause if you get the more expensive one, it's too big to fit dual rear motors so you'd need to get 2 new ones (which is the problem I find myself facing now).
```

---
## \#37 Posted by: Okami Posted at: 2017-05-17T16:57:49.553Z Reads: 188

```
So what exactly happened that you 'blew'' your motor?

was it because you carried 2 persons not just yourself?

.. anyways.. im really interested to hear the story!
```

---
## \#38 Posted by: pennyboard Posted at: 2017-05-17T17:12:59.401Z Reads: 183

```
No actually, the motor was fine carrying 2 people, what ended up blowing it was the bolts that hold the motor together were slowly coming loose, and I went on a 6 mile ride on a rough road, and the extra heat on the motor from it already being loose caused the loctite on the bolts to loosen up and the rough road shook them loose. The motor physically fell apart more so than it blew up.

But Luckily I was able to salvage the motor and its back to running like normal now
```

---
## \#39 Posted by: Hummie Posted at: 2017-05-17T17:27:21.465Z Reads: 176

```
U won't get any more power unless u change ur esc settings.  Have u tried simply upping the motor and battery amp settings on the motors u use now?  Do ur motors get hot yet?  How hot
. When they put a wattage ratting on a motor it means very little

What are ur settings
```

---
## \#40 Posted by: Eboosted Posted at: 2017-05-17T17:34:43.506Z Reads: 177

```
I have a pretty high setting:

Motor Max: 90A
Motor Min: -60
Batt Max: 40A
Batt min: -10A

Max Watt: Unchecked
```

---
## \#41 Posted by: Okami Posted at: 2017-05-17T17:44:05.953Z Reads: 174

```
hah thanks for story.. hadnt heard of turnigys burning out.. so was really curious.. :D

then it was more of a technical failure than a physicial/electronic one directly to the motor.
```

---
## \#42 Posted by: Hummie Posted at: 2017-05-17T17:45:08.647Z Reads: 171

```
Do the motors get hot because if not u can surely go up if the cells can. With the same settings on a bigger motor should be prett much same power possible
```

---
## \#43 Posted by: Titoxd10001 Posted at: 2017-05-17T18:04:08.646Z Reads: 170

```
I have similar settings and it still felt sluggish. Played with throttle curve and there is no way I can stay on the board if my finger accidentally pressed full throttle now. 6355s
```

---
## \#44 Posted by: longhairedboy Posted at: 2017-05-17T19:58:16.606Z Reads: 168

```
i use 190kv motors on 12S all the time. Its basically all i build with at all ever. 

My boards don't throw you when you hit top speed, they just don't go any faster. 

I've been close to 40mph before but haven't quite gotten there yet because i'm still only using 15T motor pulleys. I want some 16s and 17s.
```

---
## \#45 Posted by: Jinra Posted at: 2017-05-17T20:12:51.549Z Reads: 160

```
Do you set up any limiters like max erpm?
```

---
## \#46 Posted by: Eboosted Posted at: 2017-05-17T20:45:28.748Z Reads: 158

```
Yeah! But you will loose throttle regulation as 80% and 100% will feel the same
```

---
## \#47 Posted by: Titoxd10001 Posted at: 2017-05-17T21:06:17.710Z Reads: 158

```
That is true. I don't think dual 6374 would be any different though. I think that's just how the vesc operates, I cannot seem to find the middle ground between speed level and punch level like a regular car esc that has separate punch level setting.
```

---
## \#48 Posted by: Eboosted Posted at: 2017-05-17T21:35:28.888Z Reads: 158

```
You can tune your current ramp up if you do like crazy torque from a dead stop.
```

---
## \#49 Posted by: Titoxd10001 Posted at: 2017-05-17T22:00:29.252Z Reads: 155

```
Yeah I changed ramp up. I meant punch throughout the throttle curve. Still experimenting
```

---
## \#50 Posted by: Eboosted Posted at: 2017-05-17T22:22:28.482Z Reads: 156

```
Try a smaller drive pulley, a lot more power on mid range
```

---
## \#51 Posted by: longhairedboy Posted at: 2017-05-17T22:27:12.915Z Reads: 155

```
not usually. Is something supposed to happen if i don't? because it hasn't happened yet, whatever it is.
```

---
## \#52 Posted by: Jinra Posted at: 2017-05-17T22:33:33.411Z Reads: 154

```
Just wondering, since I'm sure you know about the the whole 60k+ eRPM == blown VESC thing. Glad to hear you haven't had any issues though! Gives me confidence since I'm about to slap on 230kv's motors to my 10s build.
```

---
## \#53 Posted by: Titoxd10001 Posted at: 2017-05-17T23:05:44.369Z Reads: 154

```
My point is a vesc has different power dilivery than a car esc imo. Car ESCs feel linear in speed yet punchy. Vesc feel current base so you have to jam throttle to get a punch and adjust accordingly for speed. A vesc will make you think 6355s are weak, but they're not. Limiting factor will most likely be battery and for sure vesc if you're not using direct fet version.
```

---
## \#54 Posted by: torqueboards Posted at: 2017-05-19T00:44:03.286Z Reads: 157

```
I got 16T and 18T in 12mm.
```

---
## \#55 Posted by: pennyboard Posted at: 2017-05-19T01:56:34.162Z Reads: 157

```
Where in the BLDC tool can you set the power curve? Or are you just referring to the start-up boost?
```

---
## \#56 Posted by: Titoxd10001 Posted at: 2017-05-19T02:26:07.311Z Reads: 157

```
Extended bldc tool by @ackmaniac has adjustable throttle curve
```

---
## \#57 Posted by: Kaly Posted at: 2017-05-19T02:46:24.227Z Reads: 165

```
To start using the @Ackmaniac firmware the throttle is super predictable and pairing this to dual 6374-190Kv and a 12S battery pack, the starting torque is just no comparison to the dual 6355. 

You should give it a try, it's just pure fun. Riding alone or with tandem.
```

---
## \#58 Posted by: Titoxd10001 Posted at: 2017-05-19T04:48:46.059Z Reads: 169

```
For a mountain board I would surely go with 6374s. On urethane dual 6355s are enough for me after trying out max6 and seeing what the potential is in terms of acceleration. The settings​ on a vesc (sue me trampa) need to be set really high, values that id never reach to get similar feeling. Thats has been my experience. I have tried single 6374, yet try dual. How many amps do you pull on dual 6374 setup?
```

---
## \#59 Posted by: Kaly Posted at: 2017-05-19T09:35:55.231Z Reads: 175

```
I need to get a android device to log it in realtime.
My set up is as follows 
12S-4P LG HG2
3.6v x 12= 43.2V x 3 x x4 = 518.4wh 
And I get 20 miles range on this set. 
518.40 / 20 = 25.92 Wh/mile :blush: 
My gearing is 40T/16T on 97mm flywheels. 

Comparing it to my wife board it's the same setup but with dual 6355 and a range of 24 miles.
It will be 518.40/24= 21.60 Wh/mile
```

---
## \#60 Posted by: Ackmaniac Posted at: 2017-05-19T14:15:59.598Z Reads: 172

```
The difference of a Max6 to a VESC is that it runs with duty cycle control. So when you give like 20% throttle it tries to reach 20% of the motors kv speeed. So it kicks in with very high power because it knows that it is too slow at startup and tries as hard as it can to reach that speed. this makes it hard to control the power, because to get a smooth acceleration you constantly have to slowly increase the throttle. 

The duty cycle control mode of the VESC works more or less the same. Biggest difference is that it also trys to slow down when you release the throttle. That can be changed in the software but current control (and watt control) is much more advanced. You don't control the speed, instead you control the current. So for example 20 % throttle would result in 20% acceleration at all speeds.

I haven't driven a Max6 to be honest but that is more or less how it works.
```

---
## \#61 Posted by: Okami Posted at: 2017-05-19T14:19:34.766Z Reads: 156

```
@Ackmaniac  Nice explanation! This might describe why I witness 'delay'' when applying throttle, it just cannot keep it up as quickly to accelerate the motor so fast.

Though I havent tried other settings for acceleration as these are not as good for startup.

Thanks for explaing, once again!
```

---
## \#62 Posted by: Hummie Posted at: 2017-05-19T14:30:27.062Z Reads: 154

```
i'm confused as  duty cycle is based on motor speed so a 20% increase in throttle will make the motor want to go 20% faster and it will pour out amps to get there I guess (and lots of instant power), but with current control a 20% increase in throttle would result in a 20% acceleration at all speeds.  Can you please elaborate on the distinction between the two. I'd think a 20% increase in acceleration would net you 20% increase in speed or something about that but the real question is: why is it harder to get to max amp draw with the current control than the duty cycle control irronically as it's named "current control"
```

---
## \#63 Posted by: Ackmaniac Posted at: 2017-05-19T15:46:16.577Z Reads: 152

```
It's not harder, you only need to pull the trigger more. And who knows at which current the Max6 stops.

Let's say your board can go 40 km/h max because then you kv are reached and you are doing 50% throttle from a standstill. And your max motor amps are 80A.

In Duty Cycle Control that would pull you with 80A like a bull to 20 km/h and then keeps that speed.

In Current Control it would accelerate you with half the allowed motor amps (40A) till max speed. Because the 40A would be easily enough to reach that speed.

The acceleration is of course not the same at all speeds because of the increasing resistance from nature forces which want to stop you. The torgue is the same. But we went through this acceleration example too many times already. Need to be more careful in the future.
```

---
## \#64 Posted by: Hummie Posted at: 2017-05-19T17:05:36.748Z Reads: 148

```
What do u mean about "easy enough to get there" with half the current even though in current control and full throttle?  From asking on vedder's forum I was told w the current control the load will determine the current besides the throttle pull so if u have the motor amp limit very high, which I had, I still was unable to get there.  Why cant current control simply control the current directly with the throttle.  
You always have to be careful yes
```

---
## \#65 Posted by: Titoxd10001 Posted at: 2017-05-19T17:28:37.577Z Reads: 147

```
In my testing max6 is so much more controllable. The max6 has so much more punch throughout the throttle curve and separately it has punch settings. I prefer controlling speed for example on the bench or in real life for that matter the max6 won't spin up to full speed with 1/4 throttle. My settings to get close to sensation of punch of car esc are 90 motor/40 battery per vesc with the throttle curve up and ramp up high. In summary the max6 feels like it has way more power and it feels controllable to me. Although max6 is slow top speed because it's 8s, if it was 12s I might have made the switch. 

@ackerman if you can fix the duty cycle so there is netruel when trigger is released​, that would be great.
```

---
## \#66 Posted by: Ackmaniac Posted at: 2017-05-19T17:50:29.288Z Reads: 152

```
Can you post Screenshots of the settings of the Max6. Just for curiosity. 
I thought about improving the duty cycle control. But i didn't find something yet that i would like. 
My watt control mode for example makes current control even softer. I just like the controllability. But that is simply personal preference. For my best friend for example it would be enough if his offroad bike has a simple button for power on/off.
I just like that i can go on the throttle even if i ride a hard corner or while i am carving. Because the throttle is so smooth. The most people i have seen would make the corner and then go on the throttle again on the straight.

For example 10 years ago a 150 hp motor cycle was much harder to handle and way more aggressive then the 200 hp beasts today which can be handled by anybody. For the old bikes you needed something heavy in your pants.

@Titoxd10001 if your 90A/40A is for 12S then you can reach around 2300 watts. That is in my comport zone with 12S. I mean i set my board for 2500 watts and could go even higher. But i don't want that because that power is enough and nicely controllable. And pushes me up the hills in my area with more than 50 km/h easily. So i guess the Max6 punishes the motor really hard with very high currents by simply opening the door for the current and tell the motor to take whatever he wants.
```

---
## \#67 Posted by: longhairedboy Posted at: 2017-05-19T18:00:18.607Z Reads: 151

```
[quote="Ackmaniac, post:66, topic:23146"]
For the old bikes you needed something heavy in your pants.
[/quote]

Like giant balls? You meant giant balls, didn't you! You're talking about balls! Balls are really funny!

<img src="/uploads/db1493/original/3X/e/b/ebb19911e1a67fcd5271da06371fe9b10d742d98.jpg" width="690" height="490">
```

---
## \#68 Posted by: Titoxd10001 Posted at: 2017-05-19T18:11:25.242Z Reads: 141

```
I'm talking about a Hobbywing Max6. The only setting for throttle it has is​ punch level 1-5. Imo the vesc right now feels like driving a car with a bad carburetor, you press the throttle and nothing happens. You press full throttle to get acceleration, but you have to keep adjusting for speed. It's a trade off with vesc you either have "smooth" (I would say lag/delayed) throttle or you up your settings and have no control using 1/4 throttle all the time for good acceleration. With max6 I feel I can get both. predictable, but powerful

@ackmaniac I have the vesc settings that high on vesc and I keep forgetting to check results on your app because I turn off my board before I look at my phone. But the times I've checked I'm getting over 2000 watts peak. I don't think it's that max6 six uses more amps it's just the throttle delivery is so different. Max6 feels (speed) linear, yet punchy when I need it to.
```

---
## \#69 Posted by: TarzanHBK Posted at: 2017-05-19T20:49:14.555Z Reads: 137

```
who is @ackerman? :smiley:
```

---
## \#70 Posted by: Okami Posted at: 2017-05-19T20:58:07.353Z Reads: 136

```
@Ackmaniac
```

---
## \#71 Posted by: Titoxd10001 Posted at: 2017-05-19T21:06:58.989Z Reads: 137

```
Fixed. My @ function doesn't work for some reason and i was going off memory lol
```

---
## \#72 Posted by: Titoxd10001 Posted at: 2017-05-20T01:05:52.791Z Reads: 128

```
Tried duty cycle. Only tried it for short time under 20mph for safety reasons, but it's seems be spot on in terms of speed control and acceleration off the line. Maybe that's what I'm use to, but aren't all (car/rc) escs duty cycle standard? What do boosted
 and evolve use?

If you could implement nuetral in to duty cycle I'd buy you a beer 🍺
```

---
## \#73 Posted by: Eboosted Posted at: 2017-05-20T03:20:08.977Z Reads: 126

```
Welcome @ackerman, now we have 2 VESC software developers? :grin:
```

---
## \#74 Posted by: Eboosted Posted at: 2017-05-20T03:22:50.574Z Reads: 123

```
[quote="Titoxd10001, post:72, topic:23146"]
If you could implement nuetral in to duty cycle
[/quote]

When you left off the throttle in Watt or Current mode, would you get a slight deceleration?

Wouldn't the ramp up current value make the VESC act as a regula ECS in terms of power delivery?
```

---
## \#75 Posted by: Titoxd10001 Posted at: 2017-05-20T03:41:57.324Z Reads: 122

```
In watt or current mode it goes to nuetral when you release throttle. In duty mode if you release throttle it goes straight to brake and if you're not pressing anything it's braking already. Freaking scary if you lose grip of trigger

Not even close, to me. Well you can mimic acceleration I guess, but the way you press throttle is different. You're controlling speed so if you press 1/3 throttle it will go to 10mph, you press 1/2 throttle it goes 15mph and stays there. The difference being you teleport to those speeds lol *if you want to. Without needing to jam throttle then release to go slow speed. You can still accelerate at normal pace, you need more throttle precision though because you have way more power at your finger tips. Trigger control recommend, maybe if you're using thumb you won't like having all the power
```

---
## \#76 Posted by: Eboosted Posted at: 2017-05-20T04:04:21.878Z Reads: 120

```
I wouldn't like to go back to current mode, I really like to have a rescaled full throttle range every time I press the throttle back again. 

I still use my Evolve Bamboo and I really hate when I let off the throttle and have to reach the engaging point where it starts to push again, I really don't know when to throw myself forward. In Watt mode I know exactly when and how much to lean forward or backwards.
```

---
## \#77 Posted by: Titoxd10001 Posted at: 2017-05-20T04:29:56.554Z Reads: 121

```
Every mode has its trade off I guess
```

---
