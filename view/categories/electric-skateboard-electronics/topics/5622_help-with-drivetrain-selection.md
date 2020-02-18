# Help with drivetrain selection

### Replies: 11 Views: 684

## \#1 Posted by: AugustM Posted at: 2016-07-05T21:21:09.655Z Reads: 76

```
Hi there!

I'm a new builder and looking for advise from some experts here :slight_smile:

-----What i already have----
-Kegel wheels (80mm)
-DIY mount (v4) + Pulley 36T/14T + 9mm belt
-Enertion Vesc (when it arrives)
-3* 3S 4AH Battery: http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=32631
(-> So 9S 4AH in total)

----What I am looking for------
-Motor (mainly which version/KV of SK3): I was thinking of this one: http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=42031
-BMS for my 9s battery

I know there is the rc calculator for this and i did do my calculations ;) .
I just wanted to have some second opinions/recommendations  on my build and double check whether my thinking is right, also i can't seem to find a place to buy the BMS .

I'd like to go around 27kph max, but more important to me is torque (i have a lot of steep hills in my area).

Thank you for taking the time to help me out!
I have a limmited budget and can't afford a wrong decision :confused:
```

---
## \#5 Posted by: Jinra Posted at: 2016-07-05T21:26:23.859Z Reads: 63

```
You'll probably want to stick to 200-230 kv at most. This will keep you under the VESC eRPM limit (assuming you're using a VESC) SK3/R-Spec/OM5065/DIY are all good choices!
```

---
## \#6 Posted by: AugustM Posted at: 2016-07-05T21:30:16.266Z Reads: 61

```
[quote="AugustM, post:1, topic:5622"]
I just wanted to have some second opinions/recommendations  on my build and double check whether my thinking is right, also i can't seem to find a place to buy the BMS .
[/quote]


Thank you for your response, I forgot to add that i'll indeed use the VESC! (When it finally arrives from Enertion haha).
I did read conflicting posts on the form that the lower you go in KV the higher torque you get. Is this true or should i just chose my Kv based on my desired topspeed?

Kind regards,
August M
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-05T21:34:19.317Z Reads: 56

```
top speed is inversely proportional to torque, so yea, you should generally receive more torque for lower kv. sticking to 230kv max for 9s will give you the max speed for the VESC and your gearing should give you adequate torque. If you're doing a single setup 14/36 is good, but with a 9mm, it may snap. If you're going to run 9mm's you may want to invest in a 2nd motor to provide you 18mm's worth of braking rubber.
```

---
## \#8 Posted by: sl33py Posted at: 2016-07-05T21:37:07.185Z Reads: 56

```
Welcome AugustM!

using an old speed calc i got from ADS, your setup will be a LOT faster 27kph!
[quote]
 
 
 
 
 
  Diameter
  
  Motor KV
  
  Battery S/V
  
  M pully
  
  Hub pulley
 
 
  
  
  
  
  
  
  
  
  
 
 
  80
  
  190
  
  9
  
  14
  
  36
 
 
  
  
  
  
  
  
  
  
  
 
 
  Speed= KPH
  40.11706

  Speed= MPH
  24.1669
 
  actual speed
  20.3002
[/quote]

i like the option to go to 12s, so i've usually done 190-200kv motors.

A missing part of info - how much do you weigh?  If you are trying to ride a single motor 9mm wide belt - you likely will have belt skipping on hard stopping (later when worn also on accelerating).  You would do better on 12 or 15mm wide belts for a single setup unless you are really light.  

i doubt you are going to snap a belt, but you will likely get skipping and wear the belt more quickly as a result.  Agreed a second motor would be good for hills and distribute the accell/decell forces, but not sure if you need to spend the $ on second motor/mount/pulleys/VESC etc.  Until we know your weight and how steep of hills are in your area?

HTH - GL!
```

---
## \#9 Posted by: AugustM Posted at: 2016-07-05T22:05:40.084Z Reads: 43

```
And @jinra thank you for your quick responses, the community here is amazing!! 

I didn't realise that 9mm would be such a problem. I weigh 70KG, but usualy wear a bag while riding so don't know wheter that's so reliable :/ .

Dual motor isn't an option at this moment, due to the high price.  But is there anything Else i can change cheaply to circomvent this problem? (Other gearing?). Diy only has 9mm kegel drive, so i'm out of luck there...

Thank you!
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-05T22:08:49.925Z Reads: 45

```
You may be fine with 9mm's if you don't slam on the brakes up or go up big hills. Just be careful when riding! miamielectricboards.com has a 15mm kegel pulley, but I say since you already have the DIY one, just try it out, but be careful!
```

---
## \#11 Posted by: sl33py Posted at: 2016-07-05T22:22:26.294Z Reads: 40

```
at 70kg (150lbs) - you should be fine w/ 9mm setup.  I ride 9mm on my GF's board all the time and i'm 120kg (also 2m).  I can't do hills on it, but moderate riding it's fine.

The only time you should have an issue with skipping is if you try to gear down to 12t on the motor - the contact area isn't enough and it WILL skip - A LOT.  My old dual motor setup i used 12t motor pulleys.  I usually will do 13 or 14t as a result to help avoid this.  I like big wheels (83-97- eventually 107's) and high voltage(8-12s), so until i can find a good 42/44t wheel pulley for ABEC Flywheels... my only option is to gear down the motor pulley as far as i can.

I'd ride it as is and have fun.  You might need to walk up some steep hills, but that's life.  Save up $ and get a second motor down the road w/ mount/esc/etc. to run duals then!

Best of luck!
```

---
## \#12 Posted by: sl33py Posted at: 2016-07-05T22:28:18.736Z Reads: 37

```
I have some 149kv SK3's to test and compare w/ other 190 and 200kv motors.  I've heard the lower kv= torque as well, but these motors need RPM to produce power...  So DIYes/Torqueboards has been saying for quite a while to get the 230-240kv motor and keep the rpms up to climb hills.

at 150lbs it may not be much of an issue - but for hills dual motors might be the best way to go regardless.
```

---
## \#13 Posted by: Jinra Posted at: 2016-07-05T22:30:40.526Z Reads: 36

```
A bit anecdotal, but my GT runs 130kv motors and climbs hills like nobody's business. Running high kv with high voltage will cause VESC errors as well.
```

---
## \#14 Posted by: sl33py Posted at: 2016-07-05T23:37:50.659Z Reads: 29

```
I feel you man.  It's not a matter of will it work, but which works better.  Hard to really validate, except to test.  I might try sometime, but mostly lack of time and lazy...  My GF is out this week, so it might be the week of ME!  Gaming and board building every nite!!!  Soldering station and CF crap all over the living-room table in 3...2...1!

edit - yeah i stick to 200kv or less so i can do 12s.  I've had great luck on 8s and will be using 3s x 4 on next build (for thin setup), with the 190 R-specs.

And dual motors is just simply awesome.  I had my dual DIYes 5065 200kv's on 8s and LOVED it.  geared for 25mph, but did 30mph once (tailwind?).  Stupid fast (and stupid of me to do it at midnight in the dark behind my house), ridiculously stable (GBomb drop deck = amazing), and accelerated like a batt out of hell.  Nothing like having built in foot braces for accelerating and braking!

I have dual R-Spec 6355 190's for my next build.  SLOWLY building it.  Board/Deck may have changed (again), but the end result will be worth it!  Going to re-create the e-GBomb - only better.
```

---
