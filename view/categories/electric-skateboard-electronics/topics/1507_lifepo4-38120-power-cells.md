# LifePo4 38120 Power Cells

### Replies: 5 Views: 1706

## \#1 Posted by: Monk Posted at: 2016-02-23T00:01:50.796Z Reads: 133

```
Straying from the mechanical side of my first build for a while I have been contemplating power solutions.i I originally intended to go the quick and easy route and snag a S.P.A.C.E Cell. But mounting on my deck choice becomes a challenge. So I exploring all angles. Please forgive me if this has been covered already but does anyone have any experience with or see any problems with using LifePo4 38120 3.2v batteries? My build is oriented around commuting. I know they are bigger but I'm using a top mount deck and 107mm wheels so I don't think ground clearance is an issue. I like that these have integrated screw terminals. And I'm seeing ratings of 10,000 Ah and 100A discharge capabilities. I calculated that I could fit 8 - 12 of these nicely under my deck. Do I need to be concerned about frying motors or controllers? What ESC amp ratings would be appropriate? Are these as finicky as LiPo's about charging/discharging? Anything anyone can share about this choice for power cells would be greatly appreciated.
```

---
## \#2 Posted by: siggs3000 Posted at: 2016-02-23T00:53:57.243Z Reads: 129

```
I'm using LifePo4's on my board with a VESC and single motor, though not individual cells (like I think you're describing?)

I'm using pack-form. Two of these in series for 8S total: http://www.hobbyking.com/hobbyking/store/__14074__ZIPPY_Flightmax_8400mAh_4S2P_30C_LiFePo4_Pack.html

They work just like LiPo's but with a few key differences:

 - Less of a fire hazzard when charging. This chemistry is way more stable
 - They operate at a slightly lower voltage than Lipo's so you need to make sure you calculate your min and max charge numbers properly so you don't over and undercharge them
 - You need to make sure your charger has a LifePo mode 

Aside from that, mine have been really nice so far, though I don't have many miles on my board yet. I chose LifePo over LiPo after freaking myself out by watching videos of Lipo's on fire. We all know that if you take care of Lipos, you will have no problems and loads of fun. But from what I've read, LifePo is a little safer from a fire standpoint, though slightly bulkier and lower voltage for the s's. This was my first foray into this so I went with what I felt more comfortable with.
```

---
## \#3 Posted by: Monk Posted at: 2016-02-23T02:04:16.302Z Reads: 115

```
Thank you for your input. Greatly appreciated. Not sure if you've seen my build thread yet but someone pointed out to me that attaching a S.P.A.C.E. Cell on the bottom of this this deck might detract from the ThreeSix's stunning good looks. Of course ANYTHING I put under there might do that. So I'm trying to make the power cell as visually attractive as possible while maintaining functionality. What I was thinking if I use this particular battery is this: the 38120 is a hair under 1.5" in diameter. And almost 4.75" long. It's 10Ah. I actually just found a 38140 for a few dollars more which is 12Ah. Both the positive and negative ends are threaded for 6mm fasteners. If I use short lengths of 6mm threaded rod to join these together end to end I think I have room lengthwise under the deck for 3 or maybe even 4. If I insert these into a 1.5"ID X 1/8" or 1/16" wall thickness aluminum tube and gang 3 or four of these tubes together side by side with threaded end caps containing potted jumper wires to connect them together I think I can achieve a visually appealing effect. Probably have them powder coated in black. This should leave me room for a similarly conceived ESC package. Thinking outside the box here literally. Wish I had a CAD application to depict this. Critiques welcome.
```

---
## \#4 Posted by: Monk Posted at: 2016-02-23T02:29:55.048Z Reads: 104

```
Now that I think about it if I keep these "stick" cells to 2 batteries per stick end to end for a total of 8 and paint em up to look like sticks of dynamite when someone asks me what powers my board I can say TNT! Maybe use cloth covered green jumper wires for simulated wicks. Four sticks side by side fore and four aft with space in the middle for an ESC enclosure with a seven segment LED battery level meter simulating a detonator timer. Doubt I'd be able to fly anywhere with this though without the TSA getting a little touchy. Kinda fun idea though.
```

---
## \#5 Posted by: Pablo_702 Posted at: 2016-08-06T10:27:53.484Z Reads: 53

```
Would u mind sharing a picture of ur 107mm build?
```

---
