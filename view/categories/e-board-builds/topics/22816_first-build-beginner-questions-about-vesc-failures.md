# First build &amp; beginner questions about VESC failures

### Replies: 7 Views: 1073

## \#1 Posted by: sash Posted at: 2017-05-10T22:54:17.627Z Reads: 152

```
This is my first build:

38'' Remember TED deck
Caliber II 50 degree trucks
83mm 75a Abec 11 Flywheels
Bones Ceramic Super Reds bearings

dual Torqueboards 6355 190kv motors
2x Torqueboards motor mounts
2x Torqueboards 36T ABEC Pulley Combo Kit (pulleys, belts, ..) using 13T motor pulley (also got 16T motor pulleys, if I'll need more top speed in the future)

2x VESC-X from Enertion
Space Cell Pro3 10S battery 

2.4Ghz Mini Remote (with wheel removed)

Misc wires and connectors (XT60, 12gauge silicon wires, vesc sensor wires, servo connector, vesc can bus connector)

Recent addition: Shredlights headlights


VESC SETTINGS:   sensored BLDC mode.   

Followed all steps to setup VESC that I found on this forum.

Initial settings

motor max 40a
motor min -20
batt max 30 
batt min -12
absolute max 130

Then I raised motor max to 60a and motor min to -30 or -40. 



THE GOOD

I've been riding this e-skateboard for several weeks and it absolutely rocks.  It totally changed the way how I commute to work, travel around the city.  I discovered a lot of new places, etc.  I am totally converted to e-skateboarding.

Now I can ride when there is no snow to snowboard, no wind to kitesurf, and no waves to surf.


THE BAD

Problems.

1:   I could hear rattling from the board when I ride over rough pavement.   I was trying eliminate all possible causes (loose screws, under/over tightened belts, etc), but I could not figure out the case of the rattling.   I was blaming the spacers or the bearings in the wheels.

I now think that the rattling was coming from the motors, because when I changed the motor (more on this below) the rattling stopped.   When I shake the motors I cannot hear any rattling or loose things inside.   But when I was riding with a certain speed over rough pavement, I could hear a very distinctive rattle.

Question:   Does this motor rattling happen to anybody else?   Is it normal?

2:   In one of the motors, the shaft is not permanently attached to the outer body of the motor, as it should be.   I can actually rotate it back a forth with my hand a little bit.   This is the same problem (and the same motor) as discussed in this thread:

https://www.electric-skateboard.builders/t/motor-problem-motor/21233


3:   More serious problem.    Last week I was riding slowly, actually I was about to stop, moving maybe at 3-5 mph, when the board suddenly stopped.   Lucky, I jumped off the board and did not fall.   After this the motors stopped working.   Then I pressed the throttle the motors would just stutter, and would not spin. 

By elimination, I found that the problem was in one of the VESC's.    One of the VESC's could detect both motors and seemed to work fine, but the other VESC would power up and connect to BLDC_Tool, but would not detect any of the motors.   However, there was no any VESC fault codes, in BLCD_Tool. 

Currently, I bought another motor and I reconfigured the board in single motor setup.

New setup:

single Torqueboards 6374 190kv motor + VESC-X

Good thing is that this single motor is still pretty good.  Maybe I lost a bit in uphill and braking performance, but it is still quite powerful.   Also this made the board a bit lighter and the electric system a bit less complicated.

I am going to ride with this single motor setup until I sort things out with VESC and motors.


More on the VESC-X problem:

When I tested the VESC the next day, I was actually able to detect the motor a couple of times, but then it stopped detecting the motor.   I tried everything I could find on this forum.   The phase wires and all solder points are fine, where are no any shortages.   I reinstalled the firmware on VESC, etc.   But I could not make it detect the motor.

A week later, after I got a new motor, I tried to detect it with the faulty VESC and it worked.   So now this VESC seem to be working.


THE UGLY

Now I have no trust in this faulty VESC.   Because sometimes it works and sometimes it does not work.   And I don't know the reason why and when this is happening.    I don't want to ride 20+ mph with this VESC because it can stop working anytime and send me flying.


Questions:    I know that many people fried their VESC's.   How and when does it usually happens (riding too fast, going up a steep hill, braking, ...)?    What does usually happen when VESC misbehave?  Does the skateboard suddenly become irresponsive, start to accelerate, or brake hard, or everything of the above.

Are there any signs that a VESC is about to fail?    Or this just suddenly happens without any prior indications.   (This sounds a bit like riding on top of a time bomb.)

Basically, I am trying to minimize the risk of an accident caused by faulty VESC.


Any tips and suggestions on how I should proceed with my VESC/motor issues?

Thanks!
```

---
## \#2 Posted by: laurnts Posted at: 2017-05-10T23:11:20.119Z Reads: 118

```
I can answer one. The rattling issue probably ur smashed ur motor bearing. Its hard to state whats wrong with VESC, most people fail to configure or connect VESC poorly or just faulty setup. On top of that the enclosure might be static discharge, loose wires and so on. This is no1 VESC issue in the forums.
```

---
## \#3 Posted by: sash Posted at: 2017-05-11T03:58:13.524Z Reads: 105

```
I think you are right about rattling.   I guess I need to change motor bearing.
```

---
## \#4 Posted by: Tuomalar Posted at: 2017-05-21T12:51:08.111Z Reads: 74

```
Did it help? My board also rattle a lot and i can't find any reason why. Motors are new so i dont think it's bearings.
```

---
## \#5 Posted by: sash Posted at: 2017-05-22T17:08:23.371Z Reads: 74

```
I think that it was a bearing in one of the motors, because when I changed this motor the rattling stoped.  (There was another problem with this motor related to its shaft, so I needed to fix it anyway.)

But there are many other possible reasons why a board can rattle.  For example, a few days ago, my board suddenly started to rattle a lot again.  I first thought that it was a bearing in the second motor.  But it turned out to be not the motor, but the metal ring attached to wheel pulley that disconnected from the pulley.  I contacted Dexter at diyelectricskateboards and he explained me that this ring is not really needed, and I can just remove it and ride without it.
```

---
## \#6 Posted by: sash Posted at: 2017-05-22T17:46:28.017Z Reads: 66

```
Here are some updates for my build:

I managed to break the deck (Remember TED deck).  That deck had a micro drop.  So, in order to make space for motors when turning the board, I had to make some cutouts in the deck.  This weakened the deck; and I broke it when I rode over a crack in the pavement.   Luckily, I did not break anything else.

My new deck is Earthwing Supermodel 38'' 

https://www.earthwingboards.com/product-page/supermodel-2017

I think this deck works much better for an electric skateboard.

The Earthwing deck has drop-through holes.   Currently, I am using this hole in the deck to route the wires from the motor to the enclosure.  I top mounted the trucks.  The wires go from the back of the board through the drop-thought hole over rear truck.

Is anybody else doing this?

Eventually, I am going to use this cable riser
https://www.electric-skateboard.builders/t/cable-risers-and-bash-guard-files/20987
(I've already 3D printed the riser.)
```

---
## \#7 Posted by: TranxFu Posted at: 2017-05-22T19:17:07.099Z Reads: 52

```
That's actually a pretty nice idea ! Have a drop through myself. Also top mounted.
```

---
