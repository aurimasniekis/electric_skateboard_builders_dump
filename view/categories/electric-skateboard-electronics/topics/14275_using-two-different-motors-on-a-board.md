# Using two different motors on a board?

### Replies: 15 Views: 949

## \#1 Posted by: capfirepants Posted at: 2016-12-06T20:06:27.476Z Reads: 150

```
Would this be possible?
For instance, I'd be using 1 6374 190kv and 1 6374 200kv.
Would this be a problem? They would be running from a vesc each. I get the signal from a gt2b so could split it if needed. What do you think?
```

---
## \#2 Posted by: sk8ace Posted at: 2016-12-06T21:30:31.434Z Reads: 138

```
Should be perfectly fine. I am running a Tacon Bigfoot 245kv and an Enertion 190kv with 2 vescs. I have the Tacon on the front truck and enertion on the rear truck, both on left (heel) side. Works great. Probably going to switch out the enertion for another tacon for more top speed soon.
```

---
## \#3 Posted by: NNGG Posted at: 2016-12-06T23:20:47.115Z Reads: 109

```
what voltages do you run?
```

---
## \#4 Posted by: Nate Posted at: 2016-12-07T02:28:27.985Z Reads: 98

```
Wait, did I read that correctly? Both on the heel side? Does it ride well? Sounds gnarly dude.
```

---
## \#5 Posted by: sk8ace Posted at: 2016-12-07T04:03:23.274Z Reads: 86

```
Yep both on the same side. Should help prevent torque steer. Rides great. No issues after ~30 miles of riding.<img src="/uploads/db1493/original/3X/1/a/1a17b314a7c08d5b8b88bd0229791dd21e016fc6.jpg" width="374" height="500">
```

---
## \#6 Posted by: sk8ace Posted at: 2016-12-07T04:04:29.871Z Reads: 82

```
If you mean me, I use 12s.
```

---
## \#7 Posted by: caustin Posted at: 2016-12-07T04:15:23.107Z Reads: 78

```
Hmmm, interesting. I was running that same exact uneven drive UD setup this summer and everyone warned about the 245kv component on 12s and exceeding 60K erpm limits. Sounds like you did not have any issue with that?  Will have to say, the same heel side is not one I considered, ran diagonal UDD setup lol.
```

---
## \#8 Posted by: sk8ace Posted at: 2016-12-07T04:29:31.208Z Reads: 75

```
I was running the 245kv as a single drive on 12s for a while without issue. With dual motors now, I'm not really worried about it but I will report if I have a failure. 
I considered the diagonal setup like everyone else but when I thought about it, it seemed to force a lot of torque steer (both when accelerating as well as braking). With the motors are on the same side, the torque on the trucks mostly cancel each other out.
```

---
## \#9 Posted by: barajabali Posted at: 2016-12-07T04:47:01.812Z Reads: 67

```
Interesting setup. Not sure that I've ever seen this on the forum before. 

Simple but innovative nice job!
```

---
## \#10 Posted by: caustin Posted at: 2016-12-07T04:54:52.582Z Reads: 65

```
Checkout @lowGuido UDR thread on this...fascinating!
```

---
## \#11 Posted by: barajabali Posted at: 2016-12-07T05:18:05.216Z Reads: 63

```
Im just referring to the both motors on heel side. pretty neat.
```

---
## \#12 Posted by: caustin Posted at: 2016-12-07T05:20:59.989Z Reads: 63

```
Yes, I am going to have to try that as well. Never thought of that layout instead of diagonal. Kewl!
```

---
## \#13 Posted by: capfirepants Posted at: 2016-12-07T07:42:32.241Z Reads: 54

```
Can someone tell me why both motors heel side would get rid of torque steering? Id imagine both diagonal to each other would, because one pulls on each side? what am I missing?

Has someone else done this? I guess I will be setting this up if it works as well as @sk8ace says.
```

---
## \#14 Posted by: sk8ace Posted at: 2016-12-07T08:38:55.351Z Reads: 51

```
I chose heelside simply because I most likely keep more of my weight on my heels. Thought that might give me more traction if more weight is over the drive wheels. Both motors on Toe side would probably work just the same.

My thought process is that the motor torque is trying to rotate the trucks. The rotation of the trucks is how you turn.
 When you have one motor on the left side of the rear truck and you accelerate, the motor is pulling you forward as well as trying to twist the rear truck to the right. If you then have your second motor on the right side of the front truck, that motor is pulling you forward and trying to twist the front truck to the left. That means the motors are basically trying to put you in a left hand turn. If you go hop on your board right now and lean left like you are going to turn, the front truck twists left and the rear truck twists right. In this same configuration, braking is doing the exact opposite, trying to put you in a right turn. (Front twists right and rear twists left).
When you have the motors on the same side, both motors are trying to twist the trucks in the same direction. Trucks can't twist in the same direction, they are only designed to twist in opposite directions. So that means that the motors can't torque steer your board.
```

---
## \#15 Posted by: capfirepants Posted at: 2016-12-07T12:20:22.824Z Reads: 41

```
I see, that seems logical.
```

---
