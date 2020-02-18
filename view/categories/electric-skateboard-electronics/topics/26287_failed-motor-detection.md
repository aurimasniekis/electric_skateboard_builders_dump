# Failed Motor Detection

### Replies: 18 Views: 881

## \#1 Posted by: abenny Posted at: 2017-06-27T20:23:15.853Z Reads: 101

```
Hey guys, so ive had a VESC from torqueboards for about a year now and have run it 8s with a single 6374.

This summer i decided to upgrade to dual motor, so i bought 2x 6354 260kv (sk3) and another vesc from torqueboards.


I gave the old vesc (master) ID 0, send status over CAN, and multiple ESCS over CAN.

These are my motor settings.
<img src="/uploads/db1493/original/3X/b/f/bfac47e5dc395c8b78b9106a9d593ec2183bfd45.png" width="690" height="293">

I followed dual vesc setup instructions from here http://www.lp-electronic.com/vesc/connect-two-vesc-via-can-bus/ 
.

So, i initially detected both motors just fine an set up. i was finishing the build part, and took for a test around the block, half way around the block i lost all control and when i press throttle only one motor would spin for a moment.

I am now back at my garage and trying to redetect motor on the master vesc, and it is failing. i got a bunch of drv8302 faults when i look for faults in the terminal..


here they are.
<img src="/uploads/db1493/original/3X/f/8/f84f1aff9a8b76e198c8877a68030a802ab5ce44.png" width="477" height="500">

Ive never had an issue with this vesc and it seems pretty shitty to me that as soon as i tried a dual setup it broke :(

can anyone give me any suggestions on troubleshooting, repair, etc? Im at the end of my wits here and this is my last week with my board before i need to fly back out to school and was really looking forward to playing with my new dual drive setup

edit: the new vesc works just fine though, motor detection runs fine, and no faults; its the old one that got the DRV fault
```

---
## \#2 Posted by: JLabs Posted at: 2017-06-27T21:38:47.360Z Reads: 76

```
Check your battery cutoff start and battery shut off end. They look to be reversed.
```

---
## \#3 Posted by: abenny Posted at: 2017-06-27T21:43:38.582Z Reads: 77

```
good eye, i just fixed that and still no dice :frowning:
```

---
## \#4 Posted by: Jinra Posted at: 2017-06-27T23:13:41.677Z Reads: 68

```
Looks like you blew your DRV. You'll need to get that or the VESC replaced. FYI you do **NOT** use "send status over can" on the main VESC, this might be why your DRV blew.

Send status over can = slave
Multiple ESCs over can = master
```

---
## \#5 Posted by: abenny Posted at: 2017-06-27T23:30:04.352Z Reads: 62

```
noted... i hope i can get this sorted. i messaged @JohnnyMeduse about a repair and will hopefully go through with that.
```

---
## \#6 Posted by: abenny Posted at: 2017-06-29T03:49:58.935Z Reads: 55

```
i also think it could have had something to do with my erpm setting,  alot of reading around has lead me to believe it should be set to 60k max? can someone confirm this for me, for future reference and maybe anyone int he future looking for the info.
thanks
```

---
## \#7 Posted by: Jinra Posted at: 2017-06-29T03:51:19.129Z Reads: 50

```
Unless your motor is over 260 kv, you shouldn't even come close to 60k eRPM, doubt that was the problem. You don't need to set the limit if your setup is good

EDIT: just saw your motor is 260kv, yea it probably wasn't that
```

---
## \#8 Posted by: abenny Posted at: 2017-06-29T04:10:16.852Z Reads: 50

```
so with dual 260kv i should be fine with the current erpm settings?
```

---
## \#9 Posted by: Jinra Posted at: 2017-06-29T04:11:44.319Z Reads: 47

```
Yea, the max theoretical eRPM with your setup is 58,094 which you'll never hit in a real world scenario anyway
```

---
## \#10 Posted by: Namasaki Posted at: 2017-06-29T05:42:24.150Z Reads: 44

```
[quote="Jinra, post:4, topic:26287"]
Send status over can = slave
Multiple ESCs over can = master
[/quote]


Wow! I never knew that. 
Good thing I never tried to use canbus. I probably would have fried my Master Vesc.
I just stick with Dual Master Vescs using a signal Y cable.
```

---
## \#11 Posted by: Jinra Posted at: 2017-06-29T05:53:03.307Z Reads: 41

```
Yea i tried send on both once and my motors spazzed out. Simply unchecked it from master and they ran fine. A good practice when testing anything you're not sure about is to never give it more than a little throttle for less than a second to make sure nothing's acting funny.
```

---
## \#12 Posted by: abenny Posted at: 2017-06-29T05:57:25.358Z Reads: 41

```
so you used a parallel servo cable to control both vescs with identical settings?
```

---
## \#13 Posted by: Namasaki Posted at: 2017-06-29T06:34:45.521Z Reads: 33

```
Yes, I plugged each vesc into the bldc tool one at a time loaded identical settings on both then use a Y splitter from the receiver to the 2 vescs.  Being careful to supply 5v to the receiver from only one of the vesc's by clipping the red wire from one of the signal cables.
I've been using this setup since day one on both of my builds and it works flawlessly.
```

---
## \#14 Posted by: abenny Posted at: 2017-06-29T06:42:17.450Z Reads: 34

```
alright im likely going to do that once i get my stuff repaired..and get back from school next year to use it...i have a handful of extra servo cables... so the key is to ensure that only one red wire is connected to either one of the two vescs?
```

---
## \#15 Posted by: Namasaki Posted at: 2017-06-29T13:40:51.458Z Reads: 29

```
Yes only one Vesc should supply 5v to the receiver
```

---
## \#16 Posted by: Jinra Posted at: 2017-06-29T14:30:52.781Z Reads: 27

```
technically two servos from the vescs would still provide 5v when they're both connected since it's in parallel
```

---
## \#17 Posted by: Namasaki Posted at: 2017-06-29T14:34:38.861Z Reads: 26

```
Good point, guess it really doesn't matter. 
In fact, supplying 5v from both might have an advantage. Like if the buck converter fails on one Vesc, the other will keep things going.
```

---
## \#18 Posted by: krloz Posted at: 2017-06-29T15:05:56.955Z Reads: 22

```
But in that case your y cabble better have diodes to prevent the good bec from feeding 5v to the damaged vesc
```

---
