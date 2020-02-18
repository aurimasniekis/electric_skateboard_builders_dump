# Questions about your AMP draw on your DUAL 6374 12s setup

### Replies: 14 Views: 1109

## \#1 Posted by: E1Allen Posted at: 2017-11-01T20:42:37.188Z Reads: 159

```
I've currently purchased all the parts for my build except the batteries.  I am borrowing some LiPos from a friend, the same friend who is going to build a lipo pack based on my needs for this board.  To get a better idea I was wondering if anyone has any data they have pulled based on cruising on flatish ground between 20-30mph.  Any data especially amps pulled would be helpful.  

Eric
```

---
## \#2 Posted by: thisguyhere Posted at: 2017-11-01T21:07:33.975Z Reads: 153

```
this is from dual TB 6374, focboxes, 12s4p lg hg2 cells:

hard acceleration:

https://www.electric-skateboard.builders/uploads/db1493/original/3X/d/f/dffb2f0c05d5f39c5b755c5df0af31dfe620acd5.jpg

nearing top speed cruise:

https://www.electric-skateboard.builders/uploads/db1493/original/3X/2/8/2874003e35753d452ed851f85c889a99d38c9388.jpg

https://www.electric-skateboard.builders/uploads/db1493/original/3X/8/c/8c75bfb705ddc278bb1ce19435c7aa91fc06eb97.jpg

also take a look here for voltage sag at max current draw:

https://www.electric-skateboard.builders/t/6v-sag-too-much/32002
```

---
## \#3 Posted by: E1Allen Posted at: 2017-11-01T21:11:18.509Z Reads: 133

```
Whats your rough total weight board and rider?
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-11-01T21:11:44.374Z Reads: 134

```
board + rider about 170-180lb.
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-11-01T21:14:13.670Z Reads: 132

```
i should note, the battery amp draw in the first image is limited via vesc, i've set the batt max to 40a per motor since battery pack continous discharge is 80a (hg2 cells are 20a continous x 4).

if allowed, i'm sure the motor would draw even more current since they're rated 4000+ watts, but that's limited to what the battery pack can supply.
```

---
## \#6 Posted by: E1Allen Posted at: 2017-11-01T21:14:37.319Z Reads: 130

```
and the Power, Motor Current, Battery Current from the screenshot is a reading from the combined motor output?
```

---
## \#7 Posted by: thisguyhere Posted at: 2017-11-01T21:15:39.250Z Reads: 122

```
correct, divide everything by 2 and that's what each focbox is doing.
```

---
## \#8 Posted by: E1Allen Posted at: 2017-11-01T21:16:06.963Z Reads: 118

```
I'll be somewhere around the 210lb range board and rider.
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-11-01T21:18:55.209Z Reads: 117

```
depending on what lipos you're using you may be able to set the battery max to an even higher value (50a?) if the lipos are rated properly.

whatever, even at 40a per motor, it's way more torque and acceleration i'll ever need.

in fact, i use mostly a mono drive nowadays.

it's fun to drive a build to its extremes but it isn't ideal for daily practicality.
```

---
## \#10 Posted by: E1Allen Posted at: 2017-11-01T21:43:07.411Z Reads: 109

```
So the hg2 cells are 3000mah each?  and 12s4p gives you 12,000mah total?  so wouldn't your constant cont amp draw be 12x20=240a?  Or are the batteries a different ah rating?  the 4p wouldn't matter since its the mah total that counts
```

---
## \#11 Posted by: E1Allen Posted at: 2017-11-01T21:45:33.527Z Reads: 106

```
Good to know that it's hard to get much more power just based off being able to stay on the board.
```

---
## \#12 Posted by: thisguyhere Posted at: 2017-11-01T21:47:53.183Z Reads: 104

```
no, discharge and capacity is multiplied across P count, not S count.

voltage is multiplied across S count.
```

---
## \#13 Posted by: NickTheDude Posted at: 2017-11-01T21:54:12.970Z Reads: 102

```
You're confusing C rating with amp rating. Lipos use the C rating system while liions just list the amp draw limit.
```

---
## \#14 Posted by: E1Allen Posted at: 2017-11-01T21:55:30.352Z Reads: 103

```
I did do that :( oops
```

---
