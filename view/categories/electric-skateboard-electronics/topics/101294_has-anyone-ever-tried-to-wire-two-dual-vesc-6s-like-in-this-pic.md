# Has anyone ever tried to wire two dual VESC 6&rsquo;s like in this pic

### Replies: 4 Views: 198

## \#1 Posted by: kchxaz Posted at: 2019-09-03T12:56:33.729Z Reads: 88

```
Has anyone wired two Dual VESC 6's in this fashion by soldering two parallel wires from the CANBUS on/off switch from one Dual VESC 6 to a second Dual VESC 6 and made a 4WD solution?
![46463184_233150697586651_4966375387077541888_n|640x480](upload://oRtRWal09wkJO7nmJvfcT15ePKe.jpeg) 

Did it work? Any suggestions or hints or tips that made it work? Did it not work at all? Did it smoke and spark?
```

---
## \#2 Posted by: Soflo Posted at: 2019-09-03T16:23:10.478Z Reads: 61

```
Why not just use 2 receivers bound to a single remote? Or split ppm?
```

---
## \#3 Posted by: esk8snith Posted at: 2019-09-03T17:22:36.449Z Reads: 54

```
I second this. A much better option, split ppm works great for 4wd setups.
```

---
## \#4 Posted by: kchxaz Posted at: 2019-09-03T18:43:12.735Z Reads: 50

```
I tried this last night. Fabricating a cable that splits the signal from the receiver to both VESC's but it doesn't work. 

This is only speculation but I think it is more because the VESC's are bunk to begin with. One VESC, after motor/app setup it only squeals extremely loud as the motor chokes trying to spin. The VESC that worked for one month now only spins one motor, the other motor is either idle or chokes and squeals loud as well. And it's so fucked up that I can't even use it as a single motor setup either.

As I mentioned in a separate post, earlier today I heard back from Flipsky and my contact, after consulting her engineering team has told me that this setup will indeed work, however it is very sketchy since too much heat at the solder point for the wires could damage the PCB board very quickly.

So first I have to figure out how to get the Flipsky Dual FSESC 6.6 pieces of shit to work like they should have worked from the beginning.
```

---
