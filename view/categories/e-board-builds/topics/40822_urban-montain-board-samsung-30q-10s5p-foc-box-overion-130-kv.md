# Urban/ montain board - samsung 30Q 10s5p - FOC BOX - OVERION 130 KV

### Replies: 40 Views: 2505

## \#1 Posted by: MDK Posted at: 2017-12-12T13:45:22.752Z Reads: 329

```
HI,

I m finishing my e-mtb and i would like to have some advice about the configuration of my FOC BOXs 
i use 2 130kv sensored motors with 15/66t as transmition 

I am good with carbon work and other stuf but I m clearly not in electronics and programming 

I have 5x15A of descharge so that make me a 75A ( some say that we can go up to 20A per cell with samusng 30Q > do you have feedback or experience with it?)

Actually I programised my FOC BOX with motor max min 50A -40A and batt max/ min +30 -20A
But when i test it is going so slow and with no power 

here are som pics 

[https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683855-fullsizerender.jpg](https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683855-fullsizerender.jpg)
-
[https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683856-img-3571.jpg](https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683856-img-3571.jpg)
-
[https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683857-img-3572.jpg](https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683857-img-3572.jpg)
-
[https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683857-img-3581.jpg](https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683857-img-3581.jpg)
-
And insie the beast :slight_smile: 
-
[https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683857-img-3577.jpg](https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683857-img-3577.jpg)
-
[https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683855-img-3553.jpg](https://image.noelshack.com/fichiers/2017/50/2/1513085655-1512683855-img-3553.jpg)
```

---
## \#2 Posted by: mmaner Posted at: 2017-12-12T14:23:19.051Z Reads: 291

```
Beautiful build.  I really like the the method you used to route the motor phase wires to the FocBox's.  I run dual FocBox's on my Evo build, which has 6in wheels.  I run Motor Max 80A, Motor Min -80A, Battery Max 30A & Battery Min -20A.  Give that a try and see if you have more juice.

*EDIT:  I am also running a 10s4p 30Q pack, so 20A per series is fine, the 30Q specs are underrated
```

---
## \#3 Posted by: MDK Posted at: 2017-12-12T17:56:34.186Z Reads: 271

```
Excellent!  thanks for your help
 I will try that asap. I wonder if it is not the tention device that slow down every thing but I really doubt about it because it use abec7 bearings 

How many charges have you done with this configuration? Do you see any loss of range or power during the time?

I will make those changes during the week and will let you know
```

---
## \#4 Posted by: mmaner Posted at: 2017-12-12T18:26:45.629Z Reads: 254

```
If you are talking about belt tension, that can definitely slow you down.  You want to find the sweet spot between too much (no downward flex in the belt) and too little (belt skips on the teeth.  A good starting point it to be able to push the belt down 3/8in without much force.  Then adjust the tension UP if you get skips or DOWN if it doesn't freewheel well.

I'm really guessing on the charges but probably a dozen or so? Maybe?  :slight_smile:

 I normally don't run a board down past 3.6 but I have on this one a couple of times because its so freekin carvy I just hate to get off of it.
```

---
## \#5 Posted by: cwazy1 Posted at: 2017-12-12T18:33:40.542Z Reads: 234

```
I agree with Mike here, your motor settings are weak. I run +60 and -50 on each of my 6355's for my 6" wheels. Keep your battery where its at now though, you don't want to go any higher.
```

---
## \#6 Posted by: Idle Posted at: 2017-12-12T18:44:42.039Z Reads: 241

```
 <img src="/uploads/db1493/original/3X/b/d/bd866a71dbcb1bffd15186e894937584df77fa93.JPG" width="375" height="500"> 


Uh... your belt "clearanced" the belt cover here?

Edit:  the belt is too loose.
It's kind of hard to tell, but It also looks like you may have alignment issues as well. 
Either the mount, or the idler is askew, possibly making the belt run off the inside of the wheel pulley and rub on the housing.

The #clearanced part would likely only be rubbing the housing off throttle and when braking.
```

---
## \#7 Posted by: Eboosted Posted at: 2017-12-12T19:23:24.758Z Reads: 229

```
With your configuration, you are going 25km/hr tops on 80% efficiency, that's slower than my grandmother riding her bike. 

<img src="/uploads/db1493/original/3X/a/0/a0ad6b1b846a603b47bc5401ba8156220142ac31.jpg" width="243" height="500">

Change the wheel pulley, use 8" wheels, modify the battery to get a 12s4p array or increase the pulley count on the motor. Those will give you faster speeds and more power band
```

---
## \#8 Posted by: MDK Posted at: 2017-12-12T20:00:23.018Z Reads: 211

```
Thanks for your help 

@ idle
 
It's normal it's a picture where the motor is not yet installed so there is no tension it is just an iron rod used to simulate the axis of the motor so I couldn't put any tentions on it ;) 

@ eboosted

I use 8" wheel already but clearly de specs used to programise my focbox are much too low 
I'm thinking about changing the motor pulley with 18t instead of 15 
But here the problem comes from the figures used for the vesc because I'm supposed to have a lot of torke witch I don't have now  

If after all of this it doesn't improve I will go for a new battery pack but it will be my last choice  

@mmaner

I did some test and I seen clear differences wilethe belts were to tight or too loose I think I found the right position now thx :slight_smile:
```

---
## \#9 Posted by: danielz Posted at: 2017-12-12T20:29:36.755Z Reads: 213

```
Nice build i might pinch the belt enclosure idea.

Changing up to 18t will decrease your torque, and you say you have little already. Is it acceleration or is it top speed that is bothering you?

Im on 200mm pneumatic too.  I use 15/80,  2x192kv sk3, 2x 4.10, 12s 2 x 6s 5000mah lipo in series 30c. One  recommendation is to you sensor your motors it made a big difference for me under 5mph. I can go at walking speeds up hills now. 

For reference. My battery max is 80a i peak at about 60a and average 8a.

You might want to watch you voltage drop to see if it is indeed your battery that is the weak point. Set up some telemetry. 

<img src="/uploads/db1493/original/3X/e/c/ec9bf5d17a199a3370bf323102c4b92516be8f0f.png" width="690" height="480">
```

---
## \#10 Posted by: squad Posted at: 2017-12-12T20:50:53.549Z Reads: 196

```
Really nice one man! Nice to see eMTB build using other mounts  than ones from Nowind or Idea :D I particularly like Your passive focbox cooling, nice and neat! 
Have one advice for You, SEAL those slots in your battery tray, shit tons of debris is going to get in there :sunglasses:
```

---
## \#11 Posted by: MDK Posted at: 2017-12-12T21:12:25.031Z Reads: 201

```
:grin: thx
Yes I already put an adhesive foam between the two 3D printed extremities but I think it will not be enough. The thing is that even with ms polymers or other glue I think it will not work properly because the junction have tendencies to move a little bit when the deck is bending. 
For the all length I use a Rubber scheet that allows the box to bend while keeping the inside protected from dust and water ( I will take more pics to show you ;) )

I hope it is clear enough what I say because I m French speaking :confused:
```

---
## \#12 Posted by: MDK Posted at: 2017-12-13T21:25:26.895Z Reads: 196

```
right now I  have a power switch with a 40A fuse but it's clearly not enough. it is a car blade fuse
I have in stock a 50A fuse from boat battery system that support a 50A continuous current and can resist till 120 if it is momentary do you think it's enough? do you think that It will work if I unsold the fuse holder with the 40A fuse from the power switch and I sold a bigger fuse such as a 80A or a 100A 

What do you have on your build?

any advice to not burn my board at the first acceleration is welcome :grin:

@squad
here are the pics of the battery waterproof case ;)
[http://image.noelshack.com/fichiers/2017/50/3/1513200058-vedder-switch.png](http://image.noelshack.com/fichiers/2017/50/3/1513200058-vedder-switch.png)

-

[http://image.noelshack.com/fichiers/2017/50/3/1513200063-img-3580.jpg](http://image.noelshack.com/fichiers/2017/50/3/1513200063-img-3580.jpg)

[http://image.noelshack.com/fichiers/2017/50/3/1513200061-img-3579.jpg](http://image.noelshack.com/fichiers/2017/50/3/1513200061-img-3579.jpg)
 

-

[http://image.noelshack.com/fichiers/2017/50/3/1513200274-img-3578.jpg](http://image.noelshack.com/fichiers/2017/50/3/1513200274-img-3578.jpg)

-

-

[http://image.noelshack.com/fichiers/2017/50/3/1513200272-vedder-switch.png](http://image.noelshack.com/fichiers/2017/50/3/1513200272-vedder-switch.png)
```

---
## \#13 Posted by: mmaner Posted at: 2017-12-13T21:40:39.121Z Reads: 175

```
<img src="/uploads/db1493/original/3X/0/f/0f2903b3bbe4991acb71908fe6005b2ad91e8025.jpg" width="525" height="500">
```

---
## \#14 Posted by: MDK Posted at: 2017-12-13T21:46:07.131Z Reads: 166

```
how many amps fuse did you use?  I really like to see how you did it with the cooler on the mofset :+1:
```

---
## \#15 Posted by: mmaner Posted at: 2017-12-13T22:53:40.067Z Reads: 164

```
80 amp, @goldenHusky send it to me with the switch.
```

---
## \#16 Posted by: MDK Posted at: 2017-12-14T19:44:03.404Z Reads: 173

```
hi everybody i come back from a test cession and it's really disapointing :( no any power even if i pull up my specs 
i don't understand were the prob comes from 
the motors are  slighly coghing while i accelerate 
I took a video to show you what happen with a full acceleration! :unamused:

https://youtu.be/8ozuXaESAzU

here are the last parameters I used for this test
the previous ones were motor max/min +/-60 and bat +/- 25/12
[http://image.noelshack.com/fichiers/2017/50/4/1513280544-untitled.png](http://image.noelshack.com/fichiers/2017/50/4/1513280544-untitled.png)
```

---
## \#17 Posted by: MDK Posted at: 2017-12-14T19:53:52.576Z Reads: 151

```
And to not help me it s pouring down those last days in Belgium :angry:
```

---
## \#18 Posted by: Pedrodemio Posted at: 2017-12-14T20:03:38.280Z Reads: 153

```
Did you do motor detection on both FOCbox? By the sound the motors are making something if definitely wrong
```

---
## \#19 Posted by: mmaner Posted at: 2017-12-14T20:07:28.798Z Reads: 153

```
Like @Pedrodemio said, make sure you do the motor detection.  Also make sure your remote is setup correctly in the  PPM tab.  Are you running FOC?  I would make sure you can run well in BLDC and then move up from there.  Is there any chance your wiring is not a large enough gauge?  Post some pics of the inside so we can proof your electronics.
```

---
## \#20 Posted by: MDK Posted at: 2017-12-14T20:44:25.382Z Reads: 148

```
somone from esk8.fr have the same broblem and it seem to be the motor that is changed by OVERION and due to this there is a problem with the erpm detection
```

---
## \#21 Posted by: mmaner Posted at: 2017-12-14T20:45:43.503Z Reads: 127

```
That sucks. Maybe you can find somebody local that will loan you some Motors to test with?
```

---
## \#22 Posted by: MDK Posted at: 2017-12-14T20:53:45.091Z Reads: 126

```
i have a 190kv but i need to remove it from an other build and i dont want that. especially that it have a 10mm shaft insted of the 8mm once i have with this build
```

---
## \#23 Posted by: mmaner Posted at: 2017-12-14T20:55:27.750Z Reads: 130

```
Looks like you will have to buy new motors then.  Sucks brother.
```

---
## \#24 Posted by: MDK Posted at: 2017-12-14T20:57:13.044Z Reads: 131

```
or vesc 6 witch i dont have money for and also and mainly not the place to integrate on this build 

or I buy two vesc old generation :s as you sayd It totally suck
```

---
## \#25 Posted by: stormboard1 Posted at: 2017-12-14T22:06:30.735Z Reads: 128

```
did you do the graphics on the board looks class
```

---
## \#26 Posted by: MDK Posted at: 2017-12-14T22:50:16.950Z Reads: 127

```
no the 95 comp mbs were like that
```

---
## \#27 Posted by: MDK Posted at: 2017-12-15T12:05:29.161Z Reads: 129

```
I found were the problem was and it was certainly not the one i expected. Yesterday night i test the voltage of my battery and it was at 31.5v !!! :fearful:

That lead me to an other question;
how is it possible to lose so many volts with a battery pack of 15Amp without using it? do you have any idea? 
is it possible that there is something in my build that uses electricity without percept it?

 I received the cell from NKON at 3.5V per unit and i certainly not expected that it would decrease so fast since I only did some few tests and settings and since the first time I tried to ride it it were going at max 7km/h !!! 
As someone said my grand mother could go faster by bike but at this speed even by walking she wouldn't have any difficulties to over pass me :laughing:

Or maybe when weld the battery pack??? but i think i tested it after i finished it to be sure that the balance wires were ok :confused:


in conclusion I charged the battery this morning and it goes perfecly now. @Eboosted It is completly mad :imp: even with the +65/-65 motor max and 40/-12 batt max min > for the motor max 90A and batt max 50A I will wait to be used with that power before to upgrade it but thanks for your precious help. Right now I have the feeling that it will snach my leg when i press the trigger :yum:

torque and speed are there but i need to programise the braking curve because i'm in stress to brake so it's strong ^^
```

---
## \#28 Posted by: rich Posted at: 2017-12-15T12:25:47.552Z Reads: 131

```
Nice build!

[quote="MDK, post:27, topic:40822"]
i recived the cell from NKON at 35.4V per unit and i certainly not expected that it woud decrese so fast since I only did some few tests and proramations and since the first time I tried to ride it it were going at max 7km/h !!!
[/quote]

35.4V is at the low end of 10S and the voltage decreases very fast at this point. Also the FOCBOXes have probably reduced the power due to battery cutoff settings. Below 36V there is not much power left...
I killed my 10S 10AhLipo because I forgot to switch off my board. It decreased from 35V to 9V within 28 hours :astonished:

[quote="MDK, post:27, topic:40822"]
i need to programise the braking curve because i'm in stress to brake so it's strong ^^
[/quote]

Try to lower the max brake to 30-40A on each FOCBOX, that should help and is what I do.
```

---
## \#29 Posted by: MDK Posted at: 2017-12-15T13:45:13.471Z Reads: 120

```
ok so just the fact to let your vesc open you think it can decrease the battery voltage at this point! good to know i will check  my other board that i didn't used since months ;)

the thing is that the last time on the first build i did it was with one vesc+ 1x 190 kv motor and a battery pack of 10s3p samsung 30q 9Amp. when i finished to build it i could make 5-6km before the first charge 

This time i use a 10s 5P with 15amp so I thought that just programise it would not use as much electricity as my first build ...

I will check regularly the volt to be sure that there is no loss in the build (focbox, antispark, fuse??? ) let us hope that it is normal and that my focbox used all the energy
```

---
## \#30 Posted by: rich Posted at: 2017-12-15T14:46:26.619Z Reads: 121

```
[quote="MDK, post:29, topic:40822"]
good to know i will check  my other board that i didn't used since months
[/quote]


with a vesc connected? R.I.P. battery :skull_crossbones: or do you use a BMS for discharge?

[quote="MDK, post:29, topic:40822"]
This time i use a 10s 5P with 15amp so I thought that just programise it would not use as much electricity as my first build ..
[/quote]

Was your first build a longboard? Because with a MTB you only get about 50% range compared to longboard (with same battery) due to rolling resistance. But 5-6km with 10s3p sounds not enough, that's strange.

On my MTB with 10s 10Ah Lipo, dual 6364 motors, 8" tires and 15/66 pulleys I got about 20km range.
```

---
## \#31 Posted by: MDK Posted at: 2017-12-15T17:27:36.540Z Reads: 112

```
I used it one month ago I hope it is not too late I will check tomorrow 

It is a full carbon handmade board with a 10s3p but the 6km was just after I finished it with 35v. If I charge it to the full (42v) I'm doing 25-30km :) 

I will open a post with it when I have time
```

---
## \#32 Posted by: PXSS Posted at: 2017-12-17T05:35:07.518Z Reads: 110

```
[quote="rich, post:28, topic:40822"]
35.4V is at the low end of 10S and the voltage decreases very fast at this point.
[/quote]

Wrong

[quote="rich, post:28, topic:40822"]
I killed my 10S 10AhLipo
[/quote]

Lipos and 18650 are different. 

---
35V is roughly 35% charged which is just under the recommended 40% storage. 31V is roughly 10-15%

If @MDK has not charged his batteries since he got them then all the testing and such discharged the batteries to where they are now. 

---
The lack of power is due to your vesc settings. Your low voltage start and end are probably set up too high for your battery. For Lipos, you'd want it at like 34/30 which is probably what you have. For 18650, you'd want it at 31/28. 

Fully discharged 18650 is at 2.5V, so 2.8V is still plenty above the safe range to keep your battery happy
```

---
## \#33 Posted by: rich Posted at: 2017-12-17T19:18:51.239Z Reads: 101

```
[quote="PXSS, post:32, topic:40822"]
Wrong
[/quote]


Yes and no :wink:, I think I've used the wrong word in english (which is not my language). But for me 3.5V per cell is the beginning of the end and 3.2V per cell is the end. I never discharge more (lipo & li-ion). From my experience the voltage drop from 3.5V to 3.2V per cell is very quick, for example my MTB had a range of 20km but the voltage drop from 3.5V to 3.2V per cell was within 50-100m.
```

---
## \#34 Posted by: PXSS Posted at: 2017-12-17T20:53:08.098Z Reads: 103

```
[quote="rich, post:33, topic:40822"]
for me 3.5V per cell is the beginning of the end and 3.2V per cell is the end.
[/quote]

It may be the end for you, but you are still objectively wrong. 

[quote="rich, post:33, topic:40822"]
From my experience the voltage drop from 3.5V to 3.2V per cell is very quick
[/quote]

Was this on a lipo or 18650 pack? You are comparing apples and oranges...
```

---
## \#35 Posted by: rich Posted at: 2017-12-18T13:17:02.539Z Reads: 102

```
[quote="PXSS, post:34, topic:40822"]
It may be the end for you
[/quote]

That's why I wrote "for me". Of course you can discharge a li-ion more than a lipo, no doubt.

[quote="PXSS, post:34, topic:40822"]
Was this on a lipo or 18650 pack?
[/quote]

It was a 10s 10Ah turnigy graphene 15c lipo pack. I built a li-ion pack as well but didn't test it yet so I have no comparison.
```

---
## \#36 Posted by: MDK Posted at: 2017-12-19T18:53:11.229Z Reads: 101

```
i made some test on my first board 10s3p and no drift at all even with vesc pluged so it's ok :slight_smile:

for the montain board i made somes balads in forest but it was really muddy due to the rain we had in belgium those last days. It was really fun exept when i needed to go back home and take the car.  :scream: lol

http://image.noelshack.com/fichiers/2017/51/2/1513709300-img-3605.png

http://image.noelshack.com/fichiers/2017/51/2/1513709300-img-3612.png

http://image.noelshack.com/fichiers/2017/51/2/1513709306-img-3606.jpg

http://image.noelshack.com/fichiers/2017/51/2/1513709305-img-3609.jpg

yesterday i did some change of parameters and set my focbox in hall sensor plus a change of the throttle curve
I will try it to go at work tomorrow

http://image.noelshack.com/fichiers/2017/51/2/1513709545-tortle-curve.png
```

---
## \#37 Posted by: MDK Posted at: 2017-12-19T19:07:14.995Z Reads: 92

```
here are some pics of my previous build ;)


http://image.noelshack.com/fichiers/2017/51/2/1513709899-img-2164.jpg

http://image.noelshack.com/fichiers/2017/51/2/1513709905-img-2283.jpg

http://image.noelshack.com/fichiers/2017/51/2/1513709909-img-2642-1953.jpg
http://image.noelshack.com/fichiers/2017/51/2/1513710152-img-2110-copy.jpg


http://image.noelshack.com/fichiers/2017/51/2/1513709899-img-2599.jpg

http://image.noelshack.com/fichiers/2017/51/2/1513710323-img-2575.jpg

http://image.noelshack.com/fichiers/2017/51/2/1513710326-img-2163.jpg
```

---
## \#38 Posted by: Eboosted Posted at: 2017-12-20T14:44:14.273Z Reads: 77

```
What deck was that one?
```

---
## \#39 Posted by: MDK Posted at: 2017-12-20T15:21:02.086Z Reads: 77

```
Full carbon hand made deck with erex foam and Carbon layers.
```

---
## \#40 Posted by: MDK Posted at: 2018-09-02T15:05:05.085Z Reads: 44

```
I get a short circuit on one of my focbox :s. 

Do you think it is possible to fix this? 

![image|281x500](upload://jrnwPaXkzmkTEF4UydSmyRZeiOY.jpeg)![image|375x500](upload://87VdCnymRrS5PioLL608iHPgN8p.jpeg)
```

---
