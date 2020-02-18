# VESC first bench test; large spark

### Replies: 18 Views: 960

## \#1 Posted by: Topsle Posted at: 2017-06-17T03:17:53.951Z Reads: 131

```
I set up all of my components for my build to load my settings onto my VESCs and do a bench test. After having everything connected and ready to go, I pressed the button on my switch and there was a large spark. I couldn't tell where the spark occurred. I immediately turned off the switch, unplugged everything, and inspected the VESCs. I did not notice any black sut or blown components.

I would like to ask for some advice moving forward to diagnose what happened and the best thing to do to make sure I don't make a pair of $100 paper weights if I haven't already blown my VESCs.

**My components and build info are as follows.**

Carvon Dual v2.5
2x VESC
2x Zippy compact 25c, 4000 mAh 6 cell wired in series.
Mini remote
Batteries connected in series via a Y-splitter, into an electric on/off switch, into a parallel xt90 connector, into the the VESCs.
Everything purchased from torque boards except the Carvon and batteries.

Picture of set up with batteries disconnected

<img src="/uploads/db1493/original/3X/4/9/495ad05744af92f0b523d902df9f800a91541e14.jpg" width="666" height="500">


**Things that may have potentially contributed to the spark/Other stuff I did when I tried to power the system:**
-I soldered together custom adapters from 5.5mm to 4mm bullet for the motor wires.(Red heat shrink) I plan to test the resistance of these connectors with a DMM to see if they were soldered poorly.
-A small amount of solder/flux residue was in one VESC female 5.5mm connector from an attempt to solder female 4mm plugs into the 5.5mm connectors causing one of the male connectors to not sit as snug as the others. 
-I did have the can bus connected between the VESCs, the transmitter connected, and one VESC connected to my computer via USB when I powered on the system
-The batteries were at the storage capacity of ~30% and sat for awhile at that capacity.

Any advice is much appreciated! I'm hesitant to try another test before getting some input. 

You guys help out with one of the most challenging aspects of this hobby; just wanted to let you know that you're all appreciated greatly!
```

---
## \#2 Posted by: NickTheDude Posted at: 2017-06-17T03:23:10.945Z Reads: 118

```
Sorry, I don't have any advice for the electrical problems, but one thing to note, the carvons are mounted backwards.
```

---
## \#3 Posted by: Topsle Posted at: 2017-06-17T03:24:30.892Z Reads: 117

```
Thank you, I completely overlooked that! I was so eager to throw them on I wasn't paying attention.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-06-17T03:30:04.431Z Reads: 119

```
<img src="/uploads/db1493/original/3X/2/7/276d58fd994de2e9a1f87c9d10551aa1021a0bcc.jpg" width="666" height="500">

the two power lead aren't plug in the wright way : flat is positive (red cable) rounded side is negative (black cable)
```

---
## \#5 Posted by: Topsle Posted at: 2017-06-17T03:39:22.892Z Reads: 116

```
<img src="/uploads/db1493/original/3X/b/0/b0823138dbad75fae023322d6d57a53655e35969.jpg" width="375" height="500">

So then are these leads the wrong way then? I noticed the color of the shrink wrap did not follow the colors from the switch but I assumed the leads were correct since I bought both of these from torque boards.
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-17T03:44:01.642Z Reads: 113

```
Yea that's wrong. Flat side of an xt connector is always positive.
```

---
## \#7 Posted by: Topsle Posted at: 2017-06-17T03:45:04.870Z Reads: 113

```
Okay, thank you for the quick help.
I'm assuming both of my VESCs are blown then?
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-17T03:46:22.664Z Reads: 113

```
Fix the adapter, then try again, if they don't power on they're probably busted.
```

---
## \#9 Posted by: NickTheDude Posted at: 2017-06-17T05:04:31.652Z Reads: 109

```
Damn connectors, I did the exact same thing a couple weeks ago :cry:
```

---
## \#10 Posted by: Smorto Posted at: 2017-06-17T14:13:05.321Z Reads: 93

```
Thats why I try not to mix different types of connectors, not saying that its a bad thing just it can get confusing.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-06-18T04:55:21.259Z Reads: 74

```
this is one reason I like to use single 5.5 bullet connectors for everything. 
Keeping it simple.
```

---
## \#12 Posted by: Jinra Posted at: 2017-06-18T06:42:38.608Z Reads: 64

```
XT-60's are my favorite, much shorter
```

---
## \#13 Posted by: Smorto Posted at: 2017-06-19T01:18:33.617Z Reads: 47

```
XT60s for me too.
```

---
## \#14 Posted by: NickTheDude Posted at: 2017-06-19T01:34:15.354Z Reads: 45

```
Have you had any issues with them? I've always been hesitant to use them cause of the lower amp rating but it would definitely be nice to use smaller connectors.
```

---
## \#15 Posted by: Jinra Posted at: 2017-06-19T01:39:09.516Z Reads: 44

```
Not at all. The evolve gt uses even smaller connectors and draws even more amps and it runs fine.
```

---
## \#16 Posted by: Topsle Posted at: 2017-06-19T02:05:12.828Z Reads: 44

```
SHE LIVES!

The electric switch I was using took the hit from my stupidity and failed in an open circuit, so my VESCs were saved.
<img src="/uploads/db1493/original/3X/f/7/f70bf2c5b0c5aa797876e3b6daadb634a8a9e0f5.jpg" width="666" height="500">

On the topic of connectors:
Working on this project without wanting to desolder anything has made me hate the size of some of these connectors. Once I ride this board for a month or so, I plan to update it by at least removing all of the unnecessary wire and connectors, and replacing connectors with Deans or xt60s. 
Oh, and I can't forget about how annoying it is to have the motor wires and power wires running the same direction on the vescs. That is making mounting into my enclosure much more tedious than it should be.
```

---
## \#17 Posted by: Aggdaddy Posted at: 2017-06-19T02:22:38.658Z Reads: 41

```
I'm glad I'm not the only one that was thinking those cables on diyelectricskateboards.com parts were a bit long especially for the power switch.   I haven't used mine yet, but I'm glad yours was able to save your vescs.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-06-19T02:23:52.992Z Reads: 41

```
Well now, that was one expensive fuse!!!!
Still better that than the vescs
```

---
