# Diy hub motor question

### Replies: 32 Views: 1464

## \#1 Posted by: pat.speed Posted at: 2017-07-18T22:25:37.291Z Reads: 193

```
Hi guys a have a question about outrunner a that I couldn't find on the internet or on here. So I'm going to be making a hub motor for my new build and I was wondering if it will still run if I am to remove the shaft and put something else in the middle like plastic or a steel rod? I'm pretty sure the shaft keeps it aligned but I'm not worried about that at the moment I just want to know if it would actually work
```

---
## \#2 Posted by: wafflejock Posted at: 2017-07-18T22:32:57.107Z Reads: 189

```
Think you need to use a motor shaft of some sort still.  The shaft needs to fit into the bearings that hold it in place and is held to the rotor with grub screws.  Aside from needing it to be straight to avoid wobbling itself further out of alignment the shaft needs to be rigid enough as well I think you need hardened steel of some sort.  The coils are on the stator that drives the magnetic field rotation and the magnets are on the rotor so don't believe the shaft plays large part in actually driving the motor, but for reasons above still needs to be metal in the end.

There is a video series on YouTube of a fully 3d printed and hand assembled motor but it's huge... Still will give you a better idea of what's involved.
```

---
## \#3 Posted by: pat.speed Posted at: 2017-07-18T22:37:42.021Z Reads: 174

```
Ok thanks mate. I am planing on basically taking the shaft out of the motor and the putting a steel rod through the middle as a longer axle. So your saying it should still turn even without the axle apart from the alignment which I can fix later
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-18T23:02:42.295Z Reads: 159

```
Yeah I know they take special measures to balance the motors after the rotor is produced, actually wonder how much uneven urethane wear on hubs will mess up that balancing, but anyhow the parts responsible for the driving force are really just surrounding the shaft but not dependent on it as far as I know (all the force is from the stator coils or the rotor magnets)
```

---
## \#5 Posted by: torqueboards Posted at: 2017-07-19T01:48:37.683Z Reads: 140

```
You could build a hub motor but I think it would be typically cheaper to purchase than buy. You would need a lathe and possibly a CNC machine.
```

---
## \#6 Posted by: pat.speed Posted at: 2017-07-19T04:45:43.296Z Reads: 123

```
Ok thanks guys
```

---
## \#7 Posted by: gmdangelo Posted at: 2018-01-31T20:51:38.279Z Reads: 96

```
i built my own hub motors. i did use a lathe and a cnc to make all the parts. i even casted my own wheel to go over them. all turned out great. the problem i'm having now is with the VESC and settings. i can't get it to produce enough torque to go from a stop. and top end speed is really weak too. it's driving me crazy!!!!![21|666x500](upload://caRMqrMDJOE75plfY6H9hIIHhNS.jpg)![13|666x500](upload://cHmnQPRYhgrGRmYbIgXhnfZJWRu.jpg)![09|666x500](upload://us1khJQyds8SmtTUKxVPmivpAEA.jpg)
```

---
## \#8 Posted by: ATLesk8 Posted at: 2018-01-31T21:36:38.383Z Reads: 93

```
Dude you should create a detailed thread regarding your process for these...those look like awesome urethane wheels...
```

---
## \#9 Posted by: pat.speed Posted at: 2018-01-31T21:36:51.567Z Reads: 92

```
What kv motor are you using? And what voltage?
```

---
## \#10 Posted by: gmdangelo Posted at: 2018-01-31T22:07:36.111Z Reads: 91

```
i was going once i figure everything out. i'd rather write a thread on "how to" and not "how not to".
```

---
## \#11 Posted by: gmdangelo Posted at: 2018-01-31T22:18:44.105Z Reads: 90

```
I started this build a very long time ago and I have learned so much. I am not meeting the ideal number so that may be an issue. 

260Kv and 10S lipos, so 42v full and 37v nominal. I just learned yesterday that the VESC has a 100k eRPM limit and doesn't like anything over 60k eRPM. At full everything I’m at 76440 eRPM (7 pole motor). I figured it out when I fried the VESC. Now I’m questioning the entire build. Because of the design of hub motors my gear ration is backwards from belt driven builds, but that’s true for every hub design out there. Can I even make this thing go?
```

---
## \#12 Posted by: ZackoryCramer Posted at: 2018-01-31T22:22:02.595Z Reads: 87

```
260kv at 10s!!! You need a motor around 70kv for hubs. And your going to burn the motor if you keep trying to start up with it.

To give some numbers, you are aiming at 95mph with those motors.
```

---
## \#13 Posted by: GrecoMan Posted at: 2018-01-31T22:24:16.431Z Reads: 82

```
yea you will definitely be struggling in the torque department with 270kv hubs. reterminating from delta to wye should bring down the kv quite a bit.
```

---
## \#15 Posted by: gmdangelo Posted at: 2018-01-31T22:44:25.778Z Reads: 82

```
Do they even make 70Kv motors?
```

---
## \#16 Posted by: ZackoryCramer Posted at: 2018-01-31T22:48:04.570Z Reads: 88

```
Torqueboard makes 135kv motors for 12s and 75kv for 12s, and carvon makes 75kv hub motors, so 260kv hubs are definitely a bottleneck for power since you barely have the torque to even startup. You should've done more research before making them. Hope you can figure something out.
```

---
## \#17 Posted by: Lukas Posted at: 2018-01-31T22:55:23.168Z Reads: 83

```
@gmdangelo 
Here you go with 90 kv.

http://alienpowersystem.com/shop/brushless-motors/aps-6374s-sensored-outrunner-brushless-motor-90kv-2800w/

They also have 100 kv and 60 kv options.
You could also write them to rewind the motors to a specific kv, or learn how to rewind your motors on your own.
```

---
## \#18 Posted by: Hummie Posted at: 2018-01-31T23:02:10.510Z Reads: 79

```
you could just use a different high amp esc and run maybe 6s or even lower voltage and also reterminate them wye as was said.  Then they would be much more efficient and have a lot more torque but they still look like small motors besides that.
I also sell hub motors that I make.  steelhubs.com   but those are old smaller motors and the new I'm making now.  that's why I say they look small as they look smaller than what I used to sell.  what size are the motors or stators?  If you get the voltage down enough you will have a low top speed but will work fine.
```

---
## \#19 Posted by: ZackoryCramer Posted at: 2018-01-31T23:06:48.156Z Reads: 75

```
Are hub motors hard to make? I thought they required massive investments and designing. Although I would rather prefer belt since they are more powerful and replaceable.
```

---
## \#20 Posted by: gmdangelo Posted at: 2018-02-01T02:48:27.552Z Reads: 68

```
the secret to making nice wheels is a good 2 part polyurethane, good molds and a vacuum chamber to get the bubbles out. if you have any questions feel free to ask. i have pics of most of the process and videos but i can't upload them here without converting them first.
```

---
## \#21 Posted by: pat.speed Posted at: 2018-02-01T04:37:16.867Z Reads: 64

```
For more torque I would do what @Hummie said and reterminate the windings into wye. That way it will be around 160kV
```

---
## \#22 Posted by: Hummie Posted at: 2018-02-01T04:57:49.319Z Reads: 61

```
reterminating can be hard depending on the motor and if it's got the multi-strand wire coming out of the motor or just soldered on phase wires because trying to find the 6 different wires (starts and ends) in the motor can be really hard, and separating them and regrouping them can be pretty much impossible if its glued down well, which it likely is.  But if the multistrand comes out you can go through wire by wire finding starts and ends and then bundle all the ends together and be done.

but if you were to get a very high amp controller, like a 200 amp one or maybe even more, then you could run the motors at like 4s and have no complications trying to reterminate and get all the torque you'd want as well as efficiency but then you cant use the vesc and foc!  but you will be running.
```

---
## \#23 Posted by: pat.speed Posted at: 2018-02-01T05:00:34.592Z Reads: 61

```
Yes but it is still 260kv which is not even close to enough power. Even the ngv? board uses something like 190kV and they have 4 of them and it's still not very powerful
```

---
## \#24 Posted by: Hummie Posted at: 2018-02-01T05:03:24.100Z Reads: 61

```
kv is the inverse of kt and kt tells the torque per amp, so with the high kv it will have low kt so need more amps to get the same torque.  The high kv can get the same torque as a low kv and just needs more amps so you change the battery cocktail to be more amps and less volts.  same power out but a different mx.
this isn't any less efficient and it's all amps in the motor
```

---
## \#25 Posted by: pat.speed Posted at: 2018-02-01T05:05:04.395Z Reads: 54

```
Oh ok this is new to me, but I doubt his motor could handle more than maybe 80a cont
```

---
## \#26 Posted by: Hummie Posted at: 2018-02-01T05:07:03.883Z Reads: 53

```
80a continuous....is a lot.  ..is huge.   I don't think any motor we use could.  even an 80mm motor.  peak for sure he could do 80 motor amps.  no problem.  continuous is vague anyway and doesn't have a time frame or ambient temp or take into account the motor magnets' max temp before demag or the wire enamel's temp either
```

---
## \#27 Posted by: pat.speed Posted at: 2018-02-01T05:08:54.859Z Reads: 52

```
Yes that was absolute maximum. Most likely 50a and even that would heat up the motor like crazy
```

---
## \#28 Posted by: Hummie Posted at: 2018-02-01T05:10:12.271Z Reads: 52

```
the motor wont run any hotter on 4s vs 12s and there's no free ride with running voltage.  it's effectively converted to amps in the motor.  the vesc recognizes this and you have both a battery and motor amp limit.
```

---
## \#29 Posted by: gmdangelo Posted at: 2018-02-01T05:13:48.457Z Reads: 58

```
motors state 70A MAX.

this is a bunch of good info that i'm digesting. i think that reterminating the motors and the rest of it is over my head. i'm a mechanical engineer so i think the best path for me is to remake the wheels with the correct motors. i just need to machine some new parts and select some motors.

can anyone tell me why most hub motors are at 500 watts and most people are running 2000 watts and up for  belt drives?
```

---
## \#30 Posted by: Hummie Posted at: 2018-02-01T05:19:41.457Z Reads: 57

```
the stated amp max numbers are bunk.   there's no standard for comparison and manufacturers just make up a number.  is that 70 max or peak ...and they're hugely different.   I'm sure you could do way more than 70 amps for a short period of time and they will be doing that even if you have a watt meter coming from the battery showing much lower amperage.  the esc switches it to amps and it will be much higher in the motor at low speeds.  I have my esc to put out I think 40 true amps from the battery and 120 motor amps.  I will have both happen


I do way more amps than any belt drive I've come across in san Francisco.   When I have new bigger motors complete I'll take on all comers in a race up any hill.  if there's any reason hub motors are limited in their potential power it would be their size and inability to dissipate built up heat but otherwise it's all the same.

and when they state a 2000 watt motor or whatever...it doesn't mean they even do that and the esc and also the battery can be the bottleneck and most likely is.  there's empty statements all over
```

---
## \#31 Posted by: gmdangelo Posted at: 2018-02-01T17:49:28.580Z Reads: 48

```
If wattage and amp statements are all over the place then how do you recommend someone spec a motor? i still want to build my own hub motors because that's where my mechanical expertise is (and ability to fabricate). 

i found this. do you think would make a good hub motor? 
http://alienpowersystem.com/shop/brushless-motors/aps-5065diy-outrunner-brushless-motor-90kv-1800w-diy-project/
```

---
## \#32 Posted by: Hummie Posted at: 2018-02-01T18:59:28.514Z Reads: 47

```
thats a very low kv for a motor that's so small.   quite a find.  Wish it said how many turns of wire

size or weight is a good indication of what power a motor will really do.   Winding resistance at a given kv would maybe be even better but many manufacturers seem to make that up also

I think that would make a good hub motor for a vesc but what you made already with the high kv would be fine with a very high amp controller running on lower voltage like I said.  It would be practically just as good. 

 Scorpion motors do a similar more expensive kit but with better components and more options of sizes.  I think you have to wind those too which maybe you'd want to do.  it's not as complicated as it looks.



 As an obvious example of unreal amp or power numbers hobbyking rate their house brand motors with really high wattage and amp numbers compared to everything else similarly sized.
```

---
## \#33 Posted by: gmdangelo Posted at: 2018-02-02T03:59:20.902Z Reads: 40

```
I found these I think they will work.
![image|690x426](upload://mXtC4iGPfiIx9fUcExd7xwUuczu.png)
Here are my calcs
![image|690x95](upload://j22VMXBTqSSRQYqoQHABiAZ4hcE.png)
and they should have enough torque
```

---
