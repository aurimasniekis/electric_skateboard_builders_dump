# Motor Judders as soon as I jump on the board

### Replies: 11 Views: 584

## \#1 Posted by: ChrisH Posted at: 2017-08-26T18:50:29.428Z Reads: 110

```
Hey guys. 1st post and unfortunately I need a bit of help if you will be so kind! So, finished my build a couple of months ago and have been absolutely loving riding the board wherever possible! I rode the board yesterday and charged it up last night as always. Today I jumped on the board and whilst riding it seemed to judder a bit, but was then ok. This happened a few times as tho it was braking or seizing. Now it literally will not move with my weight on it. Turns freely, runs perfectly but when I get on, it just judders like crazy! I always push off, but just feels as tho it's cogging.  It's a 190kv paired with vesc and 10s3p battery! Do you think the motor has had it? Without an LC meter, how can I check? I've checked my wiring and vesc settings! Any help or anyone who has experienced this? Cheers.
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-08-26T19:51:00.011Z Reads: 100

```
one of three in my experience 
1. voltage cut off is too high
2. belt is too tight
3. motor is shorted
```

---
## \#3 Posted by: ChrisH Posted at: 2017-08-26T22:31:29.986Z Reads: 85

```
Thanks. I have a single carvon axle from an old board so will try that on this setup just carrying out motor detection and see how that works. I have a feeling it's the motor. Shame as it's not that old but guess it only takes a stone to get in or a glitch in production to cause fault. Il give it a go and see what occurs. Cheers!
```

---
## \#4 Posted by: Hummie Posted at: 2017-08-26T23:51:12.347Z Reads: 72

```
try the bldc and foc test.  you can get good resistance and inductance readings there too.
```

---
## \#5 Posted by: markyoe Posted at: 2017-08-26T23:54:21.852Z Reads: 72

```
I think I have the same problem. Is there anything to do about a shorted motor?
```

---
## \#6 Posted by: Hummie Posted at: 2017-08-27T00:07:08.490Z Reads: 68

```
rewind.   and do a good job of fixing the wires inside down solid so they don't rub and short through something again.  shorting the motor leads through the bearing tube seems common.

not many people rewind them but I'm sure there's tons of shorted motors out there that need only that.
no more stuttering or judders
```

---
## \#7 Posted by: ChrisH Posted at: 2017-08-27T09:24:01.146Z Reads: 53

```
Nail on the head! Opened it up and two of the phase wires have been rubbing where they are quite loose! May be able to get a bit of heat shrink over but the real bummer is I've now damaged the bearing taking it apart!! My fault for being impatient! Any ideas where I can get a bearing for a 6355 190kv r spec motor? In U.K, guess I just measure it and order one the same size? Or should I just purchase a new motor? Shame you can't get r specs anymore as it's real punchy but other than the car on I've not tried anything else? Thanks a lot guys for the input, what I like about this forum!! 👍
```

---
## \#8 Posted by: Cobber Posted at: 2017-08-27T09:43:25.996Z Reads: 45

```
you can change the bearing over dude...
it is not that hard, [here](http://www.scorpionsystem.com/building_technic/change_shaft/) is a video, the most important bit is to either use a arbor press or a drill press to fit and remove the bearings if they are pressure fit.
```

---
## \#9 Posted by: ChrisH Posted at: 2017-08-27T12:04:46.963Z Reads: 38

```
Helpful link, cheers! Il source a bearing somewhere and give that a go! Nothing to lose other than the cost of a bearing so may as well!!
```

---
## \#10 Posted by: ChrisH Posted at: 2017-08-27T19:10:47.348Z Reads: 31

```
Hey. Chances of having the same problem are slim, but I opened my motor and moving the phase wires about, I could see some discolouration where they pass over each other. This I think is where they move in and out of the motor housing when cornering if not fixed properly like in my case which I have now rectified! As the varnish is now rubbed through, they are shorting. I've managed to slide a piece of heat over the wire into the housing where the two pass over one another and shrunk it down with gradual heat from a hair dryer as not to do any more damage. Just tested it and seems to be fine now!!! I obviously still need to replace the bearing but figured i need to know if it's worthwhile. Hope this might help you or you manage to sort yours one way or another!!
```

---
## \#11 Posted by: markyoe Posted at: 2017-08-27T20:40:39.079Z Reads: 27

```
Oh sweet! I'll see if I can do the same to mine. Thanks!
```

---
