# Basic Parts Schematics

### Replies: 9 Views: 1187

## \#1 Posted by: thisguyhere Posted at: 2016-09-06T18:15:16.387Z Reads: 129

```
I'm a total newb.

Recently got a prebuilt Chinese knockoff (Benchwheel) which is [already failing me](http://www.electric-skateboard.builders/t/benchwheel-power-delivery/8771/12) in some ways.

I wanted to upgrade the board to VESCs and wanted to make sure I'm understanding the basic parts configuration.

Is this correct?

http://i.imgur.com/WRkidRT.jpg
```

---
## \#2 Posted by: sl33py Posted at: 2016-09-06T18:33:57.044Z Reads: 105

```
Looks good to me.  Are you keeping the existing BMS or upgrading the battery to higher voltage as well?
```

---
## \#3 Posted by: thisguyhere Posted at: 2016-09-06T20:18:24.449Z Reads: 90

```
keeping the current battery.

goal is to reuse as much as possible and upgrade incrementally to spread the costs out.

question, does the VESC require a certain voltage + amp levels?  or can you use the VESC with varying battery sizes?
```

---
## \#4 Posted by: sl33py Posted at: 2016-09-06T21:09:58.928Z Reads: 77

```
read through your other thread on issues you're having w/ your benchwheel.

Not sure that new VESCs will fix the one motor drag issue.  

the battery looks to be 6s4p - not sure on mAh of the pack - but really not critical except for range.  

To answer your question - VESC will function just fine on 6s.  I regularly do this as my GF rides her single motor setup on 6s or occasionally 8s.  She likes it a bit slower and this makes it easier for her.  I ride the 8s setup just fine too.  

You can configure low voltage settings in VESC which can cause issues here (swapping between higher and lower voltage battery packs), but i use a simple lipo alarm to alert when cells get low (3.6/3.7v).

If you liked the ride previously, what about swapping the motors with similar/replacement ones (or a matching replacement of the one suspect motor)?  I might also try cleaning the bearings or checking them to replace one if going bad.  Good clean/lube of bearings might be the least expensive fix!  (and do your skate bearings while you are at it)  Always helps!

GL!
```

---
## \#5 Posted by: thisguyhere Posted at: 2016-09-06T21:25:10.917Z Reads: 63

```
[quote="sl33py, post:4, topic:9082"]
I might also try cleaning the bearings or checking them to replace one if going bad.  Good clean/lube of bearings might be the least expensive fix!  (and do your skate bearings while you are at it)
[/quote]

when you say clean the bearings, are we talking about the motor bearing?  is there a bearing in the motor?

and when you say skate bearing, that's the wheel bearing, right?
```

---
## \#6 Posted by: sl33py Posted at: 2016-09-06T21:27:17.233Z Reads: 54

```
correct-a-mundo.  there are at least 2 bearings in the motor.  but might be a pain to get to.  You'll need to take the motor apart.  Usually a circlip on the motor shaft and then pull off the outer "can" of the motor.  

I'm pretty sure @Chaka was talking about an upgrade/option of ceramic bearings in his custom 50mm motors - with some pics which may help you.
```

---
## \#7 Posted by: thisguyhere Posted at: 2016-09-06T21:51:38.450Z Reads: 46

```
gotya.

dayum, the motors this board came with is enclosed, not sure if i can open it up.  hell, it's not even easy getting it off the mount.

anyway, i'll put things back tonight, grease up the bearings and see if that makes a difference, along @Mobutusan's suggestion on swapping out the phase cables.

what kind of grease is good for bearings?  WD-40?
```

---
## \#8 Posted by: chinzw Posted at: 2016-09-06T22:28:58.999Z Reads: 47

```
WD40 will ruin your bearings, its a cleaner and degreaser.
Get some Lithium Grease and use that.
```

---
## \#9 Posted by: thisguyhere Posted at: 2016-09-06T22:45:01.013Z Reads: 46

```
[quote="chinzw, post:8, topic:9082, full:true"]
WD40 will ruin your bearings, its a cleaner and degreaser.Get some Lithium Grease and use that.
[/quote]

glad i asked.  thank you.
```

---
