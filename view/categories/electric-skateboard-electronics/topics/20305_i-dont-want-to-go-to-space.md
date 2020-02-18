# I don&rsquo;t want to go to space!

### Replies: 8 Views: 864

## \#1 Posted by: Geddi Posted at: 2017-04-04T22:26:54.805Z Reads: 208

```
In both cases I will be using:
VESC
BMS.
Wheel Pulley Teeth: 32
Motor Pulley Teeth: 15
83mm Wheels
I choose those two setups, because of what I will explain below:

Please help me with this. The [esk8 speed calculator](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":9,"motor-kv":245,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":32,"wheel-size":83}|)  is giving me mad results (insane top speeds). 
I have read everywhere that the VESC erpm limit should be set to 60000, which is about 8000rpm on a motor with 7polepairs. So I want my topspeed to be arround 8000rpm right? According to this formula I get the  rpm by calculating my motor kv with my volts. So that would for example 190*44.4 = 8524rpm * 7 = 59673erpm, which is still under the 60000 limit. 
Is this the way you are supposed to choose the motor and battery combination? Because I have no idea how I am supposed to approach this otherwise. If I want to use a VESC I should not be using 6S, because to many Amps. 9S and 12S is both good from a VESC's perspective I heard, but I don't need more then 30kmh topspeed. What I need is efficiency.
So one of my big questions is: Should I choose a lower kv motor, because I don't plan on going to space with 5% throttle.  
 
1.
Turnigy Aerodrive SK3 - 6364-245kv
9S1P (3x 5000mAh 3S1P 25C in series)


2.
Turnigy Aerodrive SK3 - 6374(or 64)-192kv
12S1P (3x 5000mAh 4S1P 25C in series)
```

---
## \#2 Posted by: saul Posted at: 2017-04-04T22:50:01.857Z Reads: 175

```
12t is too small. you should use at least 14t.

my board does 40 kph, so its just cruising at 30 which is good. 8s 245kv. 
but 10s 190 has better hill climbing and less heat. 12s 190 is a bit crazy. :laughing:
```

---
## \#3 Posted by: Geddi Posted at: 2017-04-04T22:55:29.220Z Reads: 168

```
Crazy in what terms? Crazy is fine I can always limit the speed in some way, but in terms of heat and stuff? good or bad?
I thought about going 8S 245, but that would be only 7252rpm.  So i thought about going higher kv.
But in general is this the way to do it?
```

---
## \#4 Posted by: sl33py Posted at: 2017-04-05T00:46:46.321Z Reads: 133

```
Agree with @Saul - 14t would be minimum for motor gear.

i'd go with lower 190kv motor, or 168kv, or 149kv to keep speeds "reasonable".  I wouldn't "flirt" with the 60k ERPM limit unless you are certain you'll never coast/brake downhill and possibly kill your DRV chip...  l would go with 9 or 10s w/ the 190kv personally.

In order to keep speeds down i'd also go bigger on the wheel gear - 36 or 40t.  DIYes has both for Flywheel in 12mm i believe, or @Titoxd10001 has a 15/40 setup for 15mm which is a nice option. 

Are you going single or dual motor?  How much do you weigh, and are you riding hills?

GL!
```

---
## \#5 Posted by: Geddi Posted at: 2017-04-05T09:22:36.806Z Reads: 105

```
@sl33py @saul
Sorry guys. Typing Mistake. I am actually going to be using a 15t motor gear. I changed it in the initial post.
I think you are right @sl33py maybe I should not be going to close to the rpm limit.
I am really tall, but not that heavy (arround 90kg) and I will have to be able to climb hills, not insanly steep hill, but hills. And it is going to be a single motor build, to keep the cost down a bit. 
I really liked the idea to go for the bigger motor, but it is almost twice as heavey (so only if I really need it). Also 10S is a problem, because I don't want to use either 5x2S or 2x5S batteries. So it has to be either 8S, 9S or 12S. I made a little table to find the sweetspot. <img src="/uploads/db1493/original/3X/b/8/b849a4dfb0bbbcebfb312368d56b0293dab7df79.PNG" width="690" height="124">
This pretty much leaves me with three options. What do guys think about that?
```

---
## \#6 Posted by: sl33py Posted at: 2017-04-05T18:11:32.209Z Reads: 72

```
Hey Johannes - i feel you man.  I am also very tall (6'8"/2m), but not as skinny as i once was...  about 120kg now.    

I've ridden multiple boards - single 50 and 63, dual 50 and 63mm setups.  I understand keeping costs down, but i would strongly suggest going with higher voltage if you are doing a single and 90kg/198lbs - that's not light!  My single motor (50mm) on my Marbel board did an amazing job taking my heavy ass up hills the last time i really pushed it and i was very pleasantly surprised.  Still walked up a few...

What size hills are you trying to ride up? (10%, 15%, 20%, or 25%+?)  Getting a "running start" at one always helps, but i really would suggest getting one of the bigger 6374's if you are only doing a single motor.  And being a bigger guy - definitely go w/ a 15mm wide belt.  the SK3 149kv might be a good fit, keep your speeds down and is a longer motor.  Or if you can find one the 168kv might be the real "sweet spot" for power.  Then with higher voltages like 12s (sticking to BLDC, not FOC unless you get VESC 6 or VESC X) - i think you'll have the "best" setup for a single motor and still have some oomph for hills.

I have to finish one of my boards i'm setting up for guests - 149kv and 8s most likely (keep speeds reasonable for newbies).  I will try 12s and some of the steeper hills by my house to compare w/ my marbel.

You have a good plan i think - i'd suggest more voltage and find the motor kv that keeps you from "going to space" speeds!  Plus the 40t wheel gear as a must-have to keep speeds and gearing down for hills.

HTH - GL!
```

---
## \#7 Posted by: Geddi Posted at: 2017-04-05T19:47:30.663Z Reads: 58

```
@sl33py
Thanks for your nice response. I really appreciate it.
 Alright so turns out I am realllllllly bad at guessing how steep a hill is. I live 80% of the year in a big City with 0 hills. No need for dual motor anyways. And when I am back in my hometown for some time of the year there is one particular hill that have in mind that I will have to climb everyday. It did some math and it turns out it is for sure less then 10% probably less then 8%. 
I was gonna use the VESC from alien as well as their mount with 35t and yes a 15mm belt. I can always change that, but it is my first build so I want to keep things as simple as possible. I worry more about batteries and charging and not blowing up or frying anything.
Also, what do thing about this [motor](http://alienpowersystem.com/shop/brushless-motors/alien-6374-hev-outrunner-brushless-motor-240kv-3300w/)? Do you think it would get too hot because of the enclosure?
```

---
## \#8 Posted by: sl33py Posted at: 2017-04-06T00:58:41.643Z Reads: 43

```
hehehe - yeah guessing a hills "grade" is more of a science than art - and i'm really bad at it.  I think i have an app on my phone i can hold on the hill and it'll tell me... somewhere... maybe!

I strongly would suggest sticking to the lower kv motors if you want some power for hills.  Or for accelerating, or for not going stupid fast.  If you stick to the 149 or 168kv motors on 12s - you will be happy.  I would also stress your gearing - go as low as you can.  No fewer than 14t on your motor gear, and try to fit 40t on your wheel gear!

my old speed calc shows this as:

83mm - 168kv - 12s - 15/40 = 7250rpm and 25mph/42kph (i target 25mph as my top speed)
83mm - 149kv - 12s - 15/40 = 6430rpm and 22mph/37kph 

Either of those if you go to 36t wheel gear will add 2-3mph top speed.

My .02 = Stick to the 149 or 168 and 12s.  Still like the price of @Titoxd10001's 15/40 gears - not sure cost to ship to EU and import fees vs Alien, but seems quality and a good price. 

Best of luck my friend!
```

---
