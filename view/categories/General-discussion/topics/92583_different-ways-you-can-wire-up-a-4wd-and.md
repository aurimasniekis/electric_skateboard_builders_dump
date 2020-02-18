# Different ways you can wire up a 4wd and

### Replies: 8 Views: 226

## \#1 Posted by: Pablo_702 Posted at: 2019-05-02T18:57:01.416Z Reads: 85

```
guys i been off the diy world for 2 years now and a lot has changed, getting ready to start a new build and im debating between 2wd (DD) or 4wd (DD), been reading for the last few weeks daily trying to get up to speed with all the new hardware theres now a day, i read somewhere but cant find it anymore, a guy asking about running a quad board with 4 12s packs one for each motor and esc, is this a crazy idea? is it doable? any pros or cons? also when it comes to 4 esc's what are the options for controlling (remote) such board??? also read somenthing about combining receivers but not quite sure, any help, input or even link that can point me in the right direction its appreciated
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-05-02T22:48:21.884Z Reads: 72

```
Go with 2wd dual 6374 if you want stupid amounts of torque and speed. 4wd is overkill and alot more expensive. The enclosure and battery will be enourmous and you will have wasted potential. The only 4wd i would even make is a hub motor board. 2wd lacks the acceleration an experienced rider would want

Btw, i weigh about 220lbs and carry 30lbs of gear plus my 15lb board. Dual 6355 will throw me off if i floor it. Dual 6374 is PLENTY
```

---
## \#3 Posted by: brenternet Posted at: 2019-05-03T00:22:07.731Z Reads: 62

```
Depends on the DD. If its a TBDD and 90kv I would say 4WD would be insane but great. 75kv 2WD gives you a nice little middle ground.

If it's lofty they are only 50odd kv, both 2wd and 4wd would be ok but I might wait until they bring out the 75kv and do that instead.

Carvon doesn't exist anymore, thank Skatan.

@b264 can talk about separating drivetrain power, it's not done often. If you don't it's easy to get two dual esc's and canbus or split ppm them to make it 4WD, it's not hard at all with one big ol' battery. 

Search for 4WD builds and make up your mind. 

Personal opinion: 2WD is going to do pretty much anything you want, go nuts if you want to though, yolo and all that.
```

---
## \#4 Posted by: Pablo_702 Posted at: 2019-05-03T01:21:01.091Z Reads: 46

```
I like that "YOLO" And yes thats why i want to do this build,i come from a 12s single 6374 149kv belt drive and that thing is a torque beast so i know 4wd is really not necessary, i just want to do it, and i understand the kind of room you would need to house all the electronics for a 4wd, as i was designing this 4wd i remember i read about giving each motor a battery pack and i was wondering how can this be done, so what ibwas thinking was 12 18650 cells for each motor for a total of 48 cells that would be a 12s4p total, with 4 motors the overall draw for each one should be way less than one or even 2 motor,  im looking at the TB DD kits and im thinking 75kv as 30mph is more than enough for me i like the idea of being able to climb pretty much any hill at a steady speed with out running out of momentum at the top or even half way of the hill, whoever can shed some light on this matter i will greatly appreciate you, also controling 4 motor from one remote whatbare the possible options???
```

---
## \#5 Posted by: b264 Posted at: 2019-05-03T05:20:41.720Z Reads: 36

```
[quote="Pablo_702, post:1, topic:92583"]
a quad board with 4 12s packs one for each motor and esc, is this a crazy idea? is it doable? any pros or cons? also when it comes to 4 esc’s what are the options for controlling (remote) such board??? also read somenthing about combining receivers but not quite sure, any help, input or even link that can point me in the right direction its appreciated
[/quote]

*See @Dirt_Bag's tips on why you don't need 4WD at all.*  Also consider dual-diagonal if it's insane amounts of traction you desire.

*But if you want it*, there are a few ways to get it.  I'm going to assume you're going to use ESCs based on VESC here.

1) one [remote receiver per ESC](https://forum./t/how-to-bind-the-mini-remote/95) (quad independent)
1) one remote receiver per pair of ESCs using CANBUS
1) one remote receiver per pair of ESCs using split PWM ("PPM")
1) one remote receiver for all ESCs using split PWM ("PPM")


Only option 4 can be used if using a remote that does not support multiple receivers.  I'd suggest option 1, and especially if using 4 batteries.  That sounds very reliable, because if anything breaks, you still have 3 drivetrains working.

There is a certain specific way you have to wire the loopkey if using 4 batteries, and I would not use CANBUS with that wiring.
```

---
## \#6 Posted by: Pablo_702 Posted at: 2019-05-03T05:28:06.495Z Reads: 30

```
I was thinking proton or maytech r2 remote, ill check if these support multiple receivers, thank you so much for your help,  now the most reliable option like u said would be 1, but if i use some of these new dual vesc, if one vesc breaks the whole unit (both) shot downs usually or not??? Also 12 18650 cells per motor, doesnt that seem low for range?
```

---
## \#7 Posted by: Dirt_Bag Posted at: 2019-05-03T05:37:27.326Z Reads: 24

```
If you still want to go 4wd, go ahead. But the board will weigh to much to carry, it will be a massive waste of potential, and the cost is stupid. Dual 6374 vs single 6374 is well over twice the power. Both motors will be running at better effeciency and can get more traction with 2 belts instead of 1. I used dual 149kv 6374s on my full size offroad board. I still dont dare accelerate at full throttle, even to get up a grassy/muddy steep hill.
```

---
## \#8 Posted by: Dirt_Bag Posted at: 2019-05-03T05:42:10.420Z Reads: 23

```
Also, "12 cells per motor" is gonna suck. A 12s4p pack with 4wd is going to give hardly any current, and last only a few miles. You need atleast 6p if you want mildly acceptable performance. I have no clue how you could even fit a 12s6p, 4 esc, and inward facing motors on a build. It would look like a potbelly pig with wheels. 1 bump and its over
```

---
