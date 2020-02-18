# The old banana build log

### Replies: 14 Views: 810

## \#1 Posted by: flozilla Posted at: 2019-01-20T14:30:32.703Z Reads: 188

```
Hi there,

My name is Florian. Sitting in Austria and lurking around this time eater for quite a long time now.
After finishing up the 3rd iteration of my first build now I want to go dual...

https://www.electric-skateboard.builders/t/punderstorm-10s2p-single-vesc-4-2-driven-230kv-aps-motor-17-7-wheelymachine/72553

I am planning this build for a while now wanna share the progress as well as ask for your input on it.

Here is what I have:

- Deck: Custom, cut from my old freeride salomon transfer wide snowboard (hence the name of the build)
- 2 FOCBOXES from @fottaz
- dual APS Drivetrain 15x32 from @SPIRITRON 
- Avenue RKP Longboard Trucks 180mm from @colinphotovideo (fingers crossed they'll arrive) 
- metr module
- Questions...

Before I start bothering you with my plans and dilemmas, have some pics first:

Here is the deck i want to speed up

![photo_2019-01-20_15-04-53|666x500](upload://yG4lZKixxMme2h6gNqIwE2swFpq.jpeg) ![photo_2019-01-20_15-04-29|375x500](upload://vn4nKfmAa2MCW1zTW2hMe60nggc.jpeg) 

How I drew it up when somewhat finished
![top|690x371](upload://waGczyzMMNw8dmt0PORizI4SDgw.png) ![bottom|690x453](upload://6w6ACYw6yE7dDSJ45KWma06dst3.png) 

Now for the questions:

- Motors: I'll go with 6355s for sure.
Since this boad will run in FOC mode I am unsure if I will need/want sensored motors.
Currently I am looking at those swirrlers:

APS 6355HEV 190kv unsensored

https://alienpowersystem.com/shop/brushless-motors/aps-6355hev-outrunner-brushless-motor-190kv-2400w/

Buildkitboard 6354 208kv sensored

https://buildkitboards.com/products/6354-208kv-motor

- Enclosure: Atm I plan to have it milled out of a single piece of either PE1000 or PA. Not sure if it would hold up or just break since the deck is flexy as hell... Alternatively I would have a mold milled and laminate CFK (all a mess and work included)

- Battery: I want to get into all the hazzle and build my own Liion pack for this.  
From mocking it up in CAD i could either get away with 12s3p or 10s4p configuration (see below)

12s3p 
![12s3p_variant|690x230](upload://uk1cgMtVZQQi4SrYroWPoOfXC8J.png) 

10s4p
![10s4p_variant|690x251](upload://4KB1A7YMzByD7xgtmoMkwvR3kJ8.png) 

This is really hard for me to decide. On one hand I want this banana to scare me to go flat out, on the other hand I want no range anxiety ever on this...

For cell protection I think I will do charge only bms... Any advice or suggestion what to get is highly appreciated!

- Remote: I will do a custom gt2b. Which of all the great designs out of this community will house it is undecided yet.

- Wheels: Want to roll on 78 - 85mm max. I am looking at seismic wheels and cagumas.
For the seismic I would have to make my own pulley design. Been emailing back and forth with dan from seismic to get the speedvents pattern, but have not received promised file yet (not sure if he is just grilling me or wants to help indeed...)

To conclude: 
Inputting everything to the calculator it should be  the 12s3p battery juicing the buildkit motors rolling on 78mm wheels at least. 

What do you think? Happy to receive feedback by you!

cheers 
Florian
```

---
## \#2 Posted by: Grozniy Posted at: 2019-01-20T18:01:29.797Z Reads: 127

```
Don't get aps, plenty motors have problems.
Your better off with maytechs.
https://www.unikboards.com/fr/boutique/moteur-skateboard-electrique-polaris-sensored-6355-190kv/
https://electricboardsolutions.com/collections/motor/products/sensored-waterproof-motor
https://street-wing.com/product/6355-190kv-sealed-motor-with-sensor/
```

---
## \#3 Posted by: flozilla Posted at: 2019-01-20T21:10:07.500Z Reads: 105

```
Hey @Grozniy !
Thx for your feedback!
What about the buildkit motor? It looks an awful lot similar to the flipskys' ...
```

---
## \#4 Posted by: Grozniy Posted at: 2019-01-20T21:20:06.234Z Reads: 100

```
@jlabs has been around far longer than flipsky. So take that into account. Flipsky motors have issues. If his motors have issues, I'm sure he'll help solve them.
```

---
## \#5 Posted by: flozilla Posted at: 2019-01-21T21:40:50.770Z Reads: 72

```
i want good motors...

they don't come cheap huh?
```

---
## \#6 Posted by: ShutterShock Posted at: 2019-01-22T05:45:02.447Z Reads: 63

```
No they don't really come cheap - I have used three different motor companies that I think are great.

I have two 6355 motors on my main board that have close to 400 miles on them, and boy can you tell lol they are beat up.  Still run great though, I have broken the sensor wires and resoldered them, because of the way I ran my cables.  These are TorqueBoards motors and I think they look great.

On my first client build is a turnigy 6365 motor that is still running great - probs 2-300 miles.  This is unsensored, wouldn't recommend but he was on a very tight budget.

Second client build has a @barajabali special edition 6380 sensored motor on it.  Awesome beast and sounds super cool.  Running perfect after ~200 miles.  

Third client build has two maytech sealed 6365 motors.  These look like they will hold up spectacularly and are fully sealed.  Also quite expensive but I got them from hyperIon1 for a good price.  I don't know if he has any more.  

I wouldn't cheap out on your motor, otherwise you'll just buy more later when bearings break and things go wrong.  There are many options out there but I would not go with Flipsky.

But anyway back to my board, I am running the Torqueboards motors and they are still running great.  The bearings are a little bit noisy after this many miles but that is to be expected.  They are also a good price for people in the US, especially if you choose the 5065 ones.  - but alas you are not in the US, my bad lol
```

---
## \#7 Posted by: flozilla Posted at: 2019-01-28T21:55:43.426Z Reads: 49

```
So after consulting the forum, the [3D Servisas esk8 calculator](https://calc.3dservisas.eu/?RY_NCsIwEITfJWeRpKb155pKT0qgYO82hwjGBHoU393MJNXbN8PO7O5b3I0XJ_F8xJfYZHHNYrftMi9mzKwaooVNMqBWSooeSrWFMdMUn50qYxprMDEnmUsWriYxBOpLMRFmR_wVzd7UptmfMx0k8Ya4BgdTmwLP3tOzEayJ_7uDietnblpQhl1uuKzPuGHCNAew7CjF5ws=) and the vendors sites I arrived here:

Going with 170kv Motor @12s I won't run into the 60k erpm barrier of the FOCBOXes by a mere margin of 24 erpm... well OK

I wanted to know where I would have to set the erpm limit using a 190kv motor @12s while still being able to hit 50 kph. 

Therefore I did this calculation:
https://docs.google.com/spreadsheets/d/12U9p5adCv9E0vVuJOheviVLf3JIMXv114Kjst-rsxL8/edit?usp=sharing

There seems to be a problem in there: I can change motor kv, the 2nd layer of the calculation (where the erpm cap is calculated) does not change... would be very happy if someone could have a look. I can't find the bug... thx

Until the calc is solved, the only vendor in europe that has 170kv Maytech motors I find is electric board solutions...

Next  I want to choose cells for my battery pack. @3p I want high capacity, high discharge cells.
Since the Price is real good and discharge is huge I lean over to https://eu.nkon.nl/sony-us18650vtc5a-flat-top.html

objections?

AND I stumbled upon the Master Cho gt2b Mod on Thingiverse. 

https://www.thingiverse.com/thing:3363820

will try this and the Sparkle mod by OKP

https://www.thingiverse.com/thing:2066350


thats all for now...
```

---
## \#8 Posted by: moon Posted at: 2019-01-28T22:00:39.693Z Reads: 43

```
[quote="ShutterShock, post:6, topic:81503"]
Second client build has a @barajabali special edition 6380 sensored motor on it. Awesome beast and sounds super cool. Running perfect after ~200 miles.
[/quote]

Is that the SK3 one?

[quote="flozilla, post:3, topic:81503"]
What about the buildkit motor? It looks an awful lot similar to the flipskys’ …
[/quote]

Different motors, BKB motors are SK3 based

Maytech or motors made by Sunray Tech (SK3, BKB) would be my only choice for motors
```

---
## \#9 Posted by: ShutterShock Posted at: 2019-01-29T02:54:21.961Z Reads: 39

```
[quote="moon, post:8, topic:81503"]
Is that the SK3 one?
[/quote]

Yeah it is! Silver one, 6380 modified a good bit. It's sensored too
```

---
## \#10 Posted by: moon Posted at: 2019-01-29T02:56:31.008Z Reads: 38

```
Link to the thread, I am guessing its just a 6374

With sensors and keyway
```

---
## \#11 Posted by: ShutterShock Posted at: 2019-01-29T07:39:43.374Z Reads: 35

```
I didn't actually make a build thread for that build unfortunately.  I can find a picture of the motor somewhere, but from what Bara said it was basically a 6380 (design looks like an SK3 like the turnigy ones) with an extended shaft, keyway, and sensors.

I don't know what you're getting at exactly lol
```

---
## \#12 Posted by: Virol Posted at: 2019-02-09T18:06:49.442Z Reads: 28

```
Sorry to interrupt here XD 

So if I read right Maytech, sk3 and BKB motors are made by sunray, and the BKB motors (6354) are based on the SK3 and I should not worry? Cus I just bought 2 of them for my build, saw that BKB was a really good brand and I haven't found someone complain about their motors
```

---
## \#13 Posted by: moon Posted at: 2019-02-09T18:09:59.004Z Reads: 31

```
No complaints
```

---
## \#14 Posted by: skatardude10 Posted at: 2019-02-09T18:20:29.689Z Reads: 25

```
![20190209_111953|377x500](upload://xB7yUc0qHKTVxPtNb2EO7EQ2e97.jpeg)
Top banana
```

---
