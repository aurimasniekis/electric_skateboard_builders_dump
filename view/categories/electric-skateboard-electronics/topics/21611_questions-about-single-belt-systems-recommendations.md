# Questions about single belt systems &amp; recommendations

### Replies: 15 Views: 996

## \#1 Posted by: lastmango Posted at: 2017-04-23T14:07:43.290Z Reads: 81

```
Hello,

Been in a few discussions, and after initially wanting to try hub motors for my first build, have decided to go with a single belt system instead—I'm interested in a simple setup  (translated as "I'm not a rocket scientist, so the more plug and play, the better")

BATTERY
I already have a Space Cell 3 Pro (10s3p) with on/off, charging, etc. I think it has an xt60 connector for the vesc.

MOTOR / DRIVETRAIN
6374, I've been told. I'm leaning towards the SK3, but certainly open to other options... I'm not a huge fan of the way it looks (I know that's not important to some & I get that.). Do all 63mm motors for esk8s have the same screw patterns, or do I need to match certain motors with certain mounts? I want Caliber II 50's, so I'm interested in mounts for those trucks that DO NOT require mods to the truck. How about ratios? I'm pretty confused about which ratio to buy, but I'm about 185lbs. I live in Florida, so hills are pretty much non-existent. I don't need crazy torque. Are flywheel clones a good choice, or is the consensus for the real deal—or Kegels? Oh yeah... I'm hearing 190kv as well... good?

Thanks, gang!
```

---
## \#2 Posted by: mmaner Posted at: 2017-04-23T14:13:44.260Z Reads: 74

```
Look at DIY's 6374, good stuff.  If you start with a 16t motor pulley and a 36t wheel pulley you'll get plenty of torque and decent speed.  In fact you could get the motor mount, pulley kit and motor from DIY and save some on shipping and Dexter (@torqueboards)  has great support.
```

---
## \#3 Posted by: anorak234 Posted at: 2017-04-23T14:14:48.158Z Reads: 69

```
Just FYI - hub motors are wayyyy more "plug n play" than a belt drive system. The reason most of us go with belt drive is bc it's better on hills and draws less amps
```

---
## \#4 Posted by: lastmango Posted at: 2017-04-23T14:20:57.221Z Reads: 68

```
Understood, @anorak234, and that (along with the clean look) was why I initially considered hubs. Most are telling me that hubs are in a weird spot of evolution at the moment though... pricier, without the reliability it seems (except the types only available in the high-end prebuilts). School me if i'm wrong, but I'm trying to get off the ground with something I know will work—I can't afford to create a testbed, lol. I also skate on Caliber trucks already, so fitting something to them makes sense to me.
```

---
## \#5 Posted by: lastmango Posted at: 2017-04-23T14:24:10.928Z Reads: 63

```
Thanks, @mmaner... I certainly appreciate your help & insight—it's not lost on me.
```

---
## \#6 Posted by: mmaner Posted at: 2017-04-23T14:26:16.086Z Reads: 60

```
No worries, holler if you need anymore help.
```

---
## \#7 Posted by: lastmango Posted at: 2017-04-23T14:27:52.746Z Reads: 57

```
Question about the sensor wire on that 6374 from DIY... that connects to what exactly? I haven't seen them on other motors, unless I just missed it.
```

---
## \#8 Posted by: mmaner Posted at: 2017-04-23T14:30:16.313Z Reads: 57

```
Most motors are sensored. You will need a sensor wire extension, but then it just plugs into the VESC. You can run un-sensored, it's much simpler, then connect the sensor later.
```

---
## \#9 Posted by: anorak234 Posted at: 2017-04-23T14:35:55.081Z Reads: 54

```
If you want something that is clean and will work indefinitely - go get a carvon hub. Expensive, but bulletproof in terms of reliability and durability. If price is a concern for you, get the torqueboards hub motors. They are cheap, and tend to have issues due to a lack of glue holding the magnets in place but I found that a 10 minute job with some epoxy will make it ride like a dream again. In terms of looks - the carvon motors are not inside the wheel, but instead on the truck for a more efficient design, whereas the torqueboards motor is entirely enclosed in the wheel. My advice? If you have the money, carvon motors are past the evolving state and are literally the best thing you can get
```

---
## \#10 Posted by: mmaner Posted at: 2017-04-23T14:36:02.903Z Reads: 57

```
Here's everything you need...

diy-electric-skateboard-kits-parts/single-bolt-on-motor-mount-with-drive-wheel-kit/

Choose 63mm, caliber, black, 16/36 12mm abec.

diy-electric-skateboard-kits-parts/motor-6374-190kv-3150w/

diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
```

---
## \#11 Posted by: lastmango Posted at: 2017-04-23T14:52:18.262Z Reads: 55

```
Awesome—that's what I'll do. So, you had replied to another post that you thought my battery connection was an xt60 or xt90—I can probably find the answer to that, but that connects to the vesc, right? The 3 bullets from the motor connect to the 3 bullets on the vesc. The sensor wire on the motor goes unused (just cut & shrink-wrap end?). How does the connection from the Rx work (still have not purchased yet; looking at small, thumbwheel type)? How/where does that tie into the system... it must connect to the vesc, but how? Also, I realize I may need to solder connector types to make compatible—just confused about exactly "what connects to what".
```

---
## \#12 Posted by: lastmango Posted at: 2017-04-23T15:00:42.407Z Reads: 50

```
Right on, but they're unavailable at the moment. Someone told me they'd likely only be available to purchase separately if you had purchased their V2's in the past, since they're pushing their completes right now. I've heard great things about them, but if I can't actually order them, it's somewhat of a moot point, no?
```

---
## \#13 Posted by: Blasto Posted at: 2017-04-23T15:19:38.211Z Reads: 47

```
[quote="mmaner, post:10, topic:21611"]
Here's everything you need...
[/quote]

What this man said.

Anyways you'll get hooked and your new found addiction will force you to build different and new setups
```

---
## \#14 Posted by: lastmango Posted at: 2017-04-23T15:24:18.671Z Reads: 46

```
Exactly—my feeling exactly. Thx.
```

---
## \#15 Posted by: mmaner Posted at: 2017-04-23T15:41:42.010Z Reads: 44

```
Yep on the motor, VESC and battery  

Don't cut the sensor wire, just fold it iber and heat shrink it.  You can tuck it into the enclosure with you phase wires (motor wires). 

Whatever remote you decide on, it will connect to the VESC PPM port.  I personally don't like trigger remotes, I prefer the thumb throttle.  Check this thread for more info..
https://www.electric-skateboard.builders/t/remotes-commercially-available-options/15162
```

---
