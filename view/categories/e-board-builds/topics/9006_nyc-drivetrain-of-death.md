# NYC Drivetrain of Death

### Replies: 21 Views: 2511

## \#1 Posted by: michaeld33 Posted at: 2016-09-05T23:07:15.091Z Reads: 304

```
Alright, here is the drivetrain @Mikeomania12 and I have been working on for a little while, which I have appropriately titled: "The NYC Drivetrain of Death"
Best run in a dual diagonal setup, but can work in a regular single drive if necessary.
Here are the specs:

- Custom Steel Motor Mount
- 20/36T Gearing
- 245KV SK3 Motor
- I run this setup at 6S, Mike runs his at 8S. A dual setup is important for getting max acceleration using this setup.

Here's a pic of this setup:
<img src="/uploads/db1493/original/2X/9/9243b1932b9800a13458921bc9ffdc03a87f3edf.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/5/59f3f580c0674e3405374cf132d901469d48a6ca.JPG" width="375" height="500">
 <img src="/uploads/db1493/original/2X/0/06ae32471161add6f98a519ffe2b94f9f13ee367.JPG" width="375" height="500">
```

---
## \#2 Posted by: paragon Posted at: 2016-09-06T00:24:04.490Z Reads: 270

```
So what about it is new?
```

---
## \#3 Posted by: XIII Posted at: 2016-09-06T00:29:00.318Z Reads: 270

```
It's fast i guess
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-09-06T01:27:01.681Z Reads: 258

```
Other than the steel motor mount, nothing. I don't hear about setups with 20 teeth often though. I posted it because I was recommended to. It's also just a sweet setup, and an easy way of getting good speed.
```

---
## \#5 Posted by: caustin Posted at: 2016-09-06T01:39:19.905Z Reads: 245

```
Yeah, I have seen those parts before but at least I don't remember seeing them together in a single configuration.

20T/36T/245kv. Can you tell us more about performance?

Don't see many 20T motor pulleys, would be interested about how that makes the torque vs speed trade off as I am moving in the other direction, larger wheel pulleys + wheels (44T/197mm) and smaller regular motor pulleys 15T.
```

---
## \#6 Posted by: michaeld33 Posted at: 2016-09-06T01:43:11.598Z Reads: 221

```
Surprisingly functions pretty well. The only issue I have run into is with my ESC, if I try to bring the motor up to speed too quickly, the ESC will cut out. Must have to do with a current limit or something... The torque is fine, even on single-drive, but I would say that may depend since I am VERRY light. You should come by and try it out for yourself! It's a lot of fun!
```

---
## \#7 Posted by: barajabali Posted at: 2016-09-06T04:11:57.390Z Reads: 200

```
those arent M4 bolts are they? the main 2
```

---
## \#8 Posted by: thisrealhuman Posted at: 2016-09-06T05:38:26.939Z Reads: 175

```
With 83mm wheels that should be 24-28mph, and if your system uses 3kw (reasonable estimate) that's only 70A per motor at 22.2v. With the right esc's this should be a really solid system. I wonder what the brakes feel like at 10s.
```

---
## \#9 Posted by: whitepony Posted at: 2016-09-06T05:50:13.172Z Reads: 167

```
pulley otherway round doesnt fit?
```

---
## \#10 Posted by: michaeld33 Posted at: 2016-09-06T11:28:25.279Z Reads: 151

```
Unfortunately not...
```

---
## \#11 Posted by: michaeld33 Posted at: 2016-09-06T11:29:09.385Z Reads: 151

```
I'm not sure which you are talking about. The tensioning ones are M4
```

---
## \#12 Posted by: michaeld33 Posted at: 2016-09-06T11:29:26.834Z Reads: 142

```
Yep! It's a sweet system
```

---
## \#13 Posted by: er2528 Posted at: 2016-09-06T12:23:25.907Z Reads: 143

```
nice setup!  I like how simple and clean it is.

This topic caught my eye.  I just registered, but can't figure out how to make my own posts.  I'd like to share my very own drivetrain of death...36aH of capacity, 3 batteries and 4 motors in AWD configuration.  Yours is much more elegant and functional.  Mine is more like a battleship
```

---
## \#14 Posted by: erikorjehag Posted at: 2016-09-06T12:40:22.434Z Reads: 133

```
The pulley on the motor looks nice. Do you know where I can find it?
```

---
## \#15 Posted by: Mikeomania12 Posted at: 2016-09-06T15:39:21.874Z Reads: 129

```
@erikorjehag  The pulley is from TB and has one flange removed since the wheel pulley already has an inner flange. 

The steel mount is something I was forced to make because all my other mounts (TB all versions, and psycho) of 6mm thick aluminum kept snapping after short periods of time. Not sure if they are too thin or maybe aluminum is too flexible, or maybe this gear ratio caused too much stress on them. If anyone wants to try them I had a few extras made.

I've been running this drive train setup on dual diagonal for almost a year now. 
97mm wheels on 7s a123, 245kv 20t/36t ratio

Regarding the speed, torque and efficiency of this setup:

**Speed**: 
comes to 38mph max
its very fast!! :smile: 
it doesn't like to go slow...difficult to maintain walking speed with this gearing. 

**Torque**:
For my weight (150 lbs) i need a dual motor to make it ride-able. it has no torque with just one motor. it constantly cogs and takes forever to get to a usable speed to stop cogging.  

For @michaeld33 luckly hes like a stick figure so one motor is good enough lol 

**Efficiency:**
Not the most efficient gearing. Especially with just one motor the it pulls crazy amps and gets very hot. you will need a very powerful battery capable of high current with thick wires everywhere. 

With 2 motors it is a lot better. Basically no cogging unless I floor the throttle from a standstill. and even then the wheels usually just start skidding and burning the pavement lol. The system runs warm most of the time. but after riding fast and hard the sk3 6364 (which is actually closer to a 50mm motor) get too hot to touch and i can fry an egg on the outside area of the enclosure where the ESC is located inside. I am using 6s hobbyking car ESC with the fan on it and its been holding up very nicely. I would never recommend using the VESC here it would melt in a second :fire:

I just recently switched to better motors and they are actual 63mm. They barely get warm even after hard acceleration.

The ideal setup here for mono-drive is probably 15t/36t but me and @michaeld33 did this kinda spontaneously one night and were limited to the parts we had on hand. My 15t pulleys were only 9mm and I didnt have anymore 9mm belts so had to settle for 20t 15mm pulley. but he got lucky cuz hes light ;)
```

---
## \#16 Posted by: caustin Posted at: 2016-09-06T17:00:23.211Z Reads: 97

```
Interesting. What are the 103mm wheels you are running this on?  MBS ATL 100mm or ABEC 107mm or pneumatic?
```

---
## \#17 Posted by: Mikeomania12 Posted at: 2016-09-06T17:03:05.385Z Reads: 97

```
97mm flywheel clones...trying hard to find some electric flywheels!!
```

---
## \#18 Posted by: tomi-rc Posted at: 2016-09-06T17:40:21.089Z Reads: 90

```
Hey Mike! I'm interested in the motor mounts since i'm about to build another board. They are made for caliber trucks right? I'm willing to pay, of course. Let me know. How are the flywheel clones holding up? I'm about to buy some 83mm ones. Thanks!
```

---
## \#19 Posted by: Mikeomania12 Posted at: 2016-09-06T19:25:24.286Z Reads: 85

```
Hey Tomi! Yes I have some. They are for caliber trucks and fit almost exact though you may prefer to put a little shrink tube in between to make it more snug. They cost $60 each. How many you need? 

The clones kinda suck. They are hard and vibrate alot especially 83mm. Also i've had 4 cores crack on me with those wheels. clone wheels should only be a temp solution.  

I would get some real flywheels. If you get clones go for the 97mm because they will feel smoother.
```

---
## \#20 Posted by: tomi-rc Posted at: 2016-09-06T20:58:16.312Z Reads: 74

```
Alright! Do you have pictures of the mount alone? Maybe i'll go with real flywheels. Thanks!
```

---
## \#21 Posted by: Mikeomania12 Posted at: 2016-09-06T21:12:32.969Z Reads: 69

```
Sure! 

<img src="/uploads/db1493/original/3X/f/e/fe33eacd8d85523d2e40972e0b8da2dd668b9125.jpg" width="690" height="388">
```

---
