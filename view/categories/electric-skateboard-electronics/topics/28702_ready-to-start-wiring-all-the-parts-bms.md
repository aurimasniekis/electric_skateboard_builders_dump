# Ready to start wiring all the parts BMS!

### Replies: 8 Views: 2400

## \#1 Posted by: AndrewFox Posted at: 2017-07-26T19:39:59.689Z Reads: 148

```
Huge shoutout to @Namasaki for being patient and and answering my questions. 

Original Post: [High Power 10s Lipo Battery Pack with BMS](http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014)

My board: [Frankenstein 1st Build](http://www.electric-skateboard.builders/t/frankenstein-1st-build-earthwing-superglider-longboard-unbranded-esk8-market-190kv-63mm-10s-lipo-5-x-2s-5000mah-60c-abec-clones-90mm-vesc/20833) 

So, I've got the battery system wired up (5x2s 5300mAH 65C) and hardwired together. My BMS is set and ready for install. My Ollin VESC is also set **(I haven't set it up yet with BDLC)**. I wanted to post up what I'll be doing and get the "green-light" from the experts before I start cutting and soldering. 

I'm following "this" diagram, but having a hard time understanding it. 

<img src="/uploads/db1493/original/3X/3/1/316f3036c6b27bcadca66e25bdf73ec658732e49.PNG" width="664" height="500">

**I'll need to cut the XT90 switch off the VESC.**

<img src="/uploads/db1493/original/3X/7/b/7b18f22ee89499e80800f766ebf43f9d82ecc3c7.JPG" width="375" height="500">

**Step 1:** The black wire from battery one is going to B-. Soldering on. A second black wire is being soldered from P- to the black wire of the VESC. I'll need to create a connection through **hardwired/banana connection**.

**Step 2:** The red wire from battery 5 is being soldered directly to the VESC (also the red wire). I need to split this wire to the charge port. Which then get's hardwired to C-.

**Step 3**: Hardwire the balance wires directly to the wires from the BMS. The balance wire has three colors (red, blue, and black,) the extension has black, black, and red.

<img src="/uploads/db1493/original/3X/e/0/e0c8152811335c1de7cb66bd9b3528847100b7aa.JPG" width="666" height="500">

Do I just need to trace the black wire from the battery to the corresponding black wire on the extension, and then exclude it from the soldering? 

**Step 4:** How exactly do I need to wire the charge port to the bms?

<img src="/uploads/db1493/original/3X/f/c/fcd9d1d3e1c6494b1dd05182c8de70de98d1e002.JPG" width="375" height="500">

For right now, I think I'll have enough on my plate.
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-07-26T19:50:43.802Z Reads: 125

```
I believe the BesTec page should have a basic wiring diagram as well?  If I remember correctly.  I have a 12S SuPower one in the mail coming and whoever answers this thread will help me out a lot too :slight_smile: 

All of the black wires in the balance connectors, are they supposed to be connected to the BMS or do they just go to a common ground?
```

---
## \#3 Posted by: mmaner Posted at: 2017-07-26T20:11:05.221Z Reads: 116

```
I wouldn't cut the XT90 off, I would suggest you make an adaptor using the opposite side of the XT90, that way you can remove the VESC from the circuit if needed.
```

---
## \#4 Posted by: ShutterShock Posted at: 2017-07-26T21:42:46.086Z Reads: 108

```
That is what I did as well @mmaner it's not too hard, I'd suggest the same. Makes it easier to replace if it goes too
```

---
## \#5 Posted by: AndrewFox Posted at: 2017-07-26T22:15:00.576Z Reads: 96

```
The batteries run off of 12awg while the VESC is connected with 10awg wire. Is this an issue?
```

---
## \#6 Posted by: mmaner Posted at: 2017-07-26T22:22:45.372Z Reads: 95

```
nope, i would use 10 on everything major if you have it, but there's no issues with using the wire that's all ready in use.
```

---
## \#7 Posted by: nmagz3 Posted at: 2017-07-27T04:59:05.455Z Reads: 80

```
@Namasaki and @mmaner are a huge help with regards to a BMS.  Great post!
```

---
## \#8 Posted by: Namasaki Posted at: 2017-07-27T06:30:08.772Z Reads: 73

```
The benefit of larger wire besides it's ability to handle more current is that it will have less resistance than smaller wire.
Keeping your wire runs as short as possible also helps reduce resistance.
So while 12awg is usually adequate for a street board, 10awg would be better especially if your wire runs are long.
adding 10awg to the existing 12awg is not an issue and my only suggestion would be to trim the 12awg short and run the majority of the length with the heavier wire.
```

---
