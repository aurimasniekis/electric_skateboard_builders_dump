# Lifepo4 pack question

### Replies: 17 Views: 1154

## \#1 Posted by: themegak Posted at: 2016-08-09T17:36:51.839Z Reads: 113

```
Hello,
Forgive me if this has already been asked.  I recently got a 36volt 5ah Lifepo4 pack from a friend.  I am aware that the chemistry is more stable and there is a voltage difference between LifePO4 cells  and 18650 lipos like the ones in the Space cell.  I'm wondering if anyone knows what the battery settings would be for programming a Vesc to use this type of battery.  I also noticed that this Lifepo4 pack is made of 12 lifepo4 cells (12S?) as well, I suppose that is to account for the voltage difference and is normal for Lifepo4 packs.  If anyone could shed some light or share their insight on these types of battery packs, I would greatly appreciate it.  Thanks.
```

---
## \#2 Posted by: XIII Posted at: 2016-08-09T17:40:11.729Z Reads: 107

```
can it deliver enough constant amps? it seems to be a 10s 2p or something. 

You will need a continious discharge of 60+A
```

---
## \#3 Posted by: Pantologist Posted at: 2016-08-09T17:44:29.773Z Reads: 107

```
LiFePO4 can deliver higher currents than lithium ion cells.

@themegak

Could you take pics of your battery? 12S lifepo4 should be a voltage total of 38.4, not 36.
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-09T17:45:15.456Z Reads: 104

```
If it's 12s it should be a 38.4v nominal pack. Do you know what cells they are specifically? Like @XIII said, it should have an adequate discharge rate if you're using it for esk8.

The main settings you'll have to set on the VESC is the battery cutoff start and end.
```

---
## \#5 Posted by: themegak Posted at: 2016-08-09T17:48:55.405Z Reads: 97

```
it came from her metroboard that used to power a 63mm single drive motor.  So i know it's up to the task of powering an Eboard.
```

---
## \#6 Posted by: themegak Posted at: 2016-08-09T17:53:19.405Z Reads: 92

```
Your probably right about the voltage, I'm going by what the label said on the battery pack itself.  I'm pretty sure it has adequate discharge rate for esk8 as the battery pack came out of a metroboard single drive 63mm motor setup.  What do you think the cutoff would be for this type of battery ?
```

---
## \#7 Posted by: Pantologist Posted at: 2016-08-09T17:56:47.916Z Reads: 92

```
It's hard to tell without knowing the exact cells. 

36v sounds like a 10S lithium ion pack. 

Could you get pics of the cells?
```

---
## \#8 Posted by: themegak Posted at: 2016-08-09T18:03:14.037Z Reads: 88

```
I was thinking the same thing but the label says 36 volt 5ah lifepo4 and does have 12 cells.  Below are the pics.
<img src="/uploads/db1493/original/2X/9/9baaa9e25e13eda6d7e24e5d034e20b3e72a707b.JPG" width="289" height="500">

View of the 12 Cells

<img src="/uploads/db1493/original/2X/e/eefd29c2eb343887d97664a2178e874440fd9904.JPG" width="558" height="500">

Side View of the BMS

<img src="/uploads/db1493/original/2X/5/536fa2610695334dda9fc6919dc500a6dc6ecbd0.JPG" width="619" height="499">
```

---
## \#9 Posted by: Pantologist Posted at: 2016-08-09T18:10:22.111Z Reads: 83

```
Prismatic pouch LiFePO4 I guess. Still should be 3.2v. Maybe that just had the sticker and round to the nearest voltage that had. They usually don't have that high of a current rating. 12S seems risky.
```

---
## \#10 Posted by: Kaly Posted at: 2016-08-09T18:14:24.303Z Reads: 81

```
Can you get a picture of the bms. Or try to find the serial or part number on it. 

The problem here is the discharge rate. but for the capacity it's good for around 8-10 miles.

In the VESC configure the voltage cut off at 30V that's 2.5V per cell. Wich is a safe cut off for this chemistry.
```

---
## \#11 Posted by: themegak Posted at: 2016-08-09T18:45:16.082Z Reads: 80

```
Attached below.  Remember this came out of a Metorboard Electric Skateboard.  The board was a slightly bigger deck version of [this](http://metro-board.com/shop/36-metroboard-midsize-brushless-outrunner-motor/) board, except it used a beefier older motor which they don't use anymore. 

<img src="/uploads/db1493/original/2X/6/6e332623377e06b30ee22d2bbc6516d7fff7c6ca.JPG" width="690" height="459">
```

---
## \#12 Posted by: themegak Posted at: 2016-08-09T18:45:55.372Z Reads: 78

```
Anyone know what the actual cutoff values would be for this kind of battery ?
```

---
## \#13 Posted by: Kaly Posted at: 2016-08-09T18:48:32.094Z Reads: 78

```
For the lifep04 chemistry is 2.5 V 
They can go down to 2V. 

This is the chemistry battery I use in my boards.
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-09T18:53:49.493Z Reads: 75

```
Cut off values are up to you, but maybe go for 2.7v cutoff start per cell and 2.5v end. For a 12S pack it'll be 32.4v start and 30v end.
```

---
## \#15 Posted by: themegak Posted at: 2016-08-09T19:02:42.658Z Reads: 74

```
Sweet.  I'm curious how you have your battery arranged in your enclosure.  As you can see from my pictures above, the pack i have is only 5ah and is really thick.  What does your battery look like ?  I like the stable chemistry of this battery but the size is ridiculous and I will have to take it apart and rewire if i want a slimmer enclosure under my deck.  Curious on what your set up looks like.
```

---
## \#16 Posted by: themegak Posted at: 2016-08-09T19:03:07.144Z Reads: 72

```
thanks for the info.  Appreciate it.
```

---
## \#17 Posted by: Kaly Posted at: 2016-08-09T19:06:19.430Z Reads: 73

```
You will need to split the pack to be able to fit it under the board. On my board I'm using 8in wheels so I have enough clearance.
```

---
