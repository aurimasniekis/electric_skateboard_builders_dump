# Boosted board Gorilla style &#124; Loaded Vanguard &#124; Torqueboards 6355 190kv &#124; VESC-X &#124; FOC &#124; 9s1p lipo

### Replies: 7 Views: 1447

## \#1 Posted by: sash Posted at: 2017-06-22T07:12:28.641Z Reads: 312

```
This is my second esk8 build.  

Goal:  Flexible lightweight customizable e-skateboard with easily removable battery.

Deck: Loaded Vanguard.   When I got this deck and first rode it as a regular longboard, I liked it so much that I thought I should just leave it as it is without electrifying it.   But I eventually put a motor on it.  However, I want to make a setup where I can easily remove the battery and other components and convert it back to a regular longboard.<img src="/uploads/db1493/original/3X/6/a/6a5c2c9f6d70d463062d71aaeba0b059728cd06f.jpg" width="317" height="500">

This is how it looks with electric components:
<img src="/uploads/db1493/original/3X/f/b/fb1c7b681f8004fbeccbc150eb12c193ff54d94c.jpg" width="283" height="500">

Currenty, all components are mounted to the deck with Gorilla tape.  I did not put any screws etc because I am going to experiment with different layouts of the components.   Eventually, I am going to make a nice looking board with custom enclosures.   But I will try to avoid making any holes in the deck and putting any screws.   In my first build, it was a pain to make inserts for screws.  In this build, I am going to attach everything to the deck with silicone caulk.    Silicone will provide extra flexibility of attachments, which should be good for a flexible deck.

I am considering various options for attaching the covers for the battery and VESC.   I want to make a system where I can easily exchange the battery on the fly without unscrewing any screws.   One option is to attach them using rubber cords. 

Drivetrain:   I am going to experiment with different motors, gear ratio, batteries, etc.

Current setup: Single Torqueboards 6355 190kv motor with 13/36 gear ratio, 83mm Flywheels. 

Other options:  
(a) Dual Torqueboards 6355 190kv motors
(b) Single Torqueboards 6374 190kv motor
(c) Dual Sk3 5055 280kv motors

Battery: 9s1p lipo,  more precisely 3 3s1p 5000mah 20C Zippy lipo packs connected in series.   This is how I mounted them with Gorilla tape:
<img src="/uploads/db1493/original/3X/0/f/0fe4700f4703b30724a556f1a6d8da5e3063112a.jpg" width="690" height="333">

I am making a custom fiberglass cover for the battery. <img src="/uploads/db1493/original/3X/6/8/682896e9d3217787cf2f2035befe4b9de6d26214.jpg" width="375" height="500">
This is how it currently looks (still needs some glazing trimming and polishing with sandpaper):
<img src="/uploads/db1493/original/3X/0/d/0d5d2192581651be89b05835e12d43ed5856a3c0.jpg" width="670" height="500"> 

VESC enclosure is made out of a plastic food container.  I will also replace it with a fiberglass one:
<img src="/uploads/db1493/original/3X/9/8/98973b67bf3deb9d0bc78a69a191c4a9aef61852.jpg" width="670" height="500">

VESC-X settings: sensored FOC mode

<img src="/uploads/db1493/original/3X/0/a/0a6ea16d8b3da6ade11ddb3f71757c7eaa752405.png" width="690" height="395">
<img src="/uploads/db1493/original/3X/3/6/3668eae2de0f8a1d05ae4fcfa5e5fb3f8dfe13c8.png" width="690" height="387">

Remote:  2.4ghz Mini Remote



I rode the board for about a week and it is pretty sweet.

Today, I was riding the board, checking FOC mode and testing the range of the battery ... and I've got a

BIG PROBLEM:

At some point, while riding, I noticed that the board is making slight jerking movements.  I stopped, checked everything.   Everything looked Ok, so I continued to ride.  At first, the board was riding normally, but then the jerking movements started again, and then become stronger and stronger.   The motor would erratically accelerate and brake even if I did not touch the remote.    Then I turned the remote off, and to my surprise, the erratic accelerations and brakings continued.    The board was totally out of control.   So I turned it off, removed the drive belt from the motor, and finished the rest of my trip by pushing the board.   When I tested the board at home, it again seem to work normally, and there are no error codes in VESC.   The lipo battery has about 1/2 charge in it:  All 9 cells have the same voltage 3.79 Volt.

So my questions to everybody:   Do my settings look Ok?  What is the most likely reason for erratic behavior of the skateboard?    What is the weakest link in my setup?

Here are some ideas about possible reasons:

1.  I have not changed the AA batteries in my mini remote for a while.  (I was using this remote in my first build.)   So far it worked without a problem.  Maybe now the batteries need to be replaced.   But, as I said, the erratic behavior continued even when I turned the remote off.   I guess this eliminates the possibility that the problem was in the remote.  Or does it?

2.  I read on this forum many horror stories how FOC fired VESC.  In particular, FOC is sensitive to the length of the cable between the battery and the VESC.  The cable needs to be less then 30cm.     I am using Boosted board style layout with battery in the front of the board and VESC in the back of the board.   The length of the cable between the battery and VESC in my setup is longer than 30cm.    I was riding in FOC mode last 3 days and it seemed to work fine.   But maybe today FOC started to act up. 

In my first build I was using BLDC mode.   In the second build I wanted to try FOC.   I like how the motor sounds (almost silent) in FOC mode when I am riding at slow speed among the people.   But, frankly speaking, this is a very minor advantage.   At normal cruising speed, FOC is as noisy as BLDC.   And at slow speed, when I am riding on a pavement among the people, I think it is more convenient just to push the board and not use the motor at all.

If there is a chance that FOC (long battery cable?) can cause such erratic accelerations and brakes I am definitely switching back to BLDC mode.

Are there any other possible reasons?
```

---
## \#2 Posted by: sash Posted at: 2017-06-23T02:21:38.149Z Reads: 212

```
Mystery solved!    

Today, I figured out what was happening with my board.    

First, I eliminated two things: 

(1) I put in new AA batteries to my 2.4Ghz Mini Remote Controller

(2)  I connected another VESC-X configured in BLDC mode.

After that, when I was riding around the city, the problem with random spinning up of the motor started to happen again.    I even made a video where my board is laying on the ground next to the remote controller and the motor would randomly spin up and and slow down by itself.

So it was not FOC mode, it was not batteries in the remote controller, the phase wires from the motor to VESC were connected OK without any shortages, and also the wires the battery to VESC were connected fine.

Can anybody guess what it was?
```

---
## \#3 Posted by: rpn314 Posted at: 2017-06-23T11:21:55.874Z Reads: 173

```
loose PPM cable from your remote receiver to the VESC would be my first guess.
```

---
## \#4 Posted by: sash Posted at: 2017-06-23T19:07:57.312Z Reads: 156

```
You are right!   This is exactly what happened - loose cable from the remote receiver to the VESC.  After I secured the cable with tape, the board works perfectly. 

For future reference, if the cable from the remote receiver gets loose the board becomes totally wild.  Can be very dangerous if one is riding at high speed.

I am curious what other people are doing to make sure that this cable won't get loose? (tape, glue, ???)
```

---
## \#5 Posted by: rpn314 Posted at: 2017-06-23T22:18:44.118Z Reads: 140

```
I always recommend you solder anything that connects to the VESC. Hot glue may be good enough (and it will definitely help some), but solder is really the best answer. 

Glad you figured it out though! Knowing if half the battle. It's definitely scary to have issues when riding it like that. :fearful:
```

---
## \#6 Posted by: sash Posted at: 2017-06-26T17:55:39.320Z Reads: 127

```
Thanks for the tip.  I am going to solder the PPM cable to VESC.

By the way, do you also solder CANBUS cable (for dual motor setup) to VESC?
```

---
## \#7 Posted by: rpn314 Posted at: 2017-06-28T11:23:06.966Z Reads: 106

```
I solder everything except for battery to vesc and vesc to motor. In both of those cases I use 5mm bullet connectors which are soldered to short 10awg wire and covered in heat shrink.
```

---
