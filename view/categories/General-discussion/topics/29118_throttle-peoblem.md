# Throttle peoblem

### Replies: 26 Views: 1159

## \#1 Posted by: Takis Posted at: 2017-07-30T11:10:52.979Z Reads: 74

```
Hi I'm new here , and I have a question . I'm having a Maytech VESC I control with a servo tester (which t
It has modified a hall sensor, a thumb throttle , when I push the throttle it stops and when I release it it accelerates , does anybody have any idea how to overturn it ? In the BLDC TOOL I didn't find anything that can help . Thanks
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-07-30T12:04:20.160Z Reads: 72

```
Turn everything off and swap any two of the three motor wires would be my first move. That's how I reverse the direction for my esk8's. if you are running sensored foc or hybrid then I would wait for a more experienced user to answer. There may be more to it than I know.

Good luck.
```

---
## \#3 Posted by: JLabs Posted at: 2017-07-30T12:10:03.023Z Reads: 64

```
Did you run motor detection and set you min and max pulse width values?
```

---
## \#4 Posted by: Takis Posted at: 2017-07-31T05:41:46.074Z Reads: 41

```
I have the min pulse to 1.25 and max about 1.50 , but when I press the throttle is 1.25 and when I release it is 1.50  and I don't see any option that inverts that :confused:
```

---
## \#5 Posted by: Takis Posted at: 2017-07-31T05:42:39.789Z Reads: 37

```
It's not the motor direction it's the throttle that works inverted .
```

---
## \#6 Posted by: trancejunkiexxl Posted at: 2017-07-31T05:47:31.559Z Reads: 38

```
ok so i had this issue as well.. i fixed it by ppm calibration

too be more specific watch the display when you hold the throttle down.. record that value and then make it your min.. i beleive this is how i fixed it

do you have winning remote?
```

---
## \#7 Posted by: krloz Posted at: 2017-07-31T07:09:20.595Z Reads: 38

```
Could your potentiometer you use as throttle be wired upside down?
```

---
## \#8 Posted by: trancejunkiexxl Posted at: 2017-07-31T08:28:15.481Z Reads: 31

```
I thought this as well when I first got my remotes,so I tested another one. it seems all my winning remotes, do this right out of the bag.
```

---
## \#9 Posted by: krloz Posted at: 2017-07-31T09:00:01.897Z Reads: 29

```
Sorry I don't know that remote.  Is it maybe possible it has a invert switch like some remotes have for the direction wheel.
```

---
## \#10 Posted by: Takis Posted at: 2017-07-31T15:22:41.696Z Reads: 24

```
well that does not do anything at all , no I don't have a remote , I have a thumb trottle connected (bypass) in a servo tester <img src="/uploads/db1493/original/3X/9/f/9f6e941ed7ad57c1eb0d913a5ea95e03de149935.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/a/2a2e7956f51cbe0ef11dce6de2244ea7a62fc471.jpg" width="375" height="500">
```

---
## \#11 Posted by: trancejunkiexxl Posted at: 2017-07-31T15:24:19.231Z Reads: 22

```
ahh I mis-read.. that looks like a really neat setup!! talk to senior waffle..maybe he can help ya!
```

---
## \#12 Posted by: Takis Posted at: 2017-07-31T15:24:28.047Z Reads: 20

```
I don't know , I can try it but if I burn it I'll need a month until I recieve another one (Aliexpress)
```

---
## \#13 Posted by: Takis Posted at: 2017-07-31T15:26:41.778Z Reads: 19

```
Well I'm new here 😛I don't know anyone  I'm trying to put it in reverse and change the motor wires but it does not go reverse at all and I don't know why
```

---
## \#14 Posted by: trancejunkiexxl Posted at: 2017-07-31T15:27:29.112Z Reads: 19

```
can u see input in display in bldc.. I'm fresh off the boat as well, found my home XD
```

---
## \#15 Posted by: Takis Posted at: 2017-07-31T15:28:52.340Z Reads: 19

```
Btw I have an alien power systems 6374 60kv that says max 10s I l ask  them and they told me it can handle 12s  but they have not   tested it , any idea ?
```

---
## \#16 Posted by: trancejunkiexxl Posted at: 2017-07-31T15:32:08.456Z Reads: 18

```
if you can see input in bloc ppm window, then it might just be programming.. ya motor/battery rating is fine I believe...always seek a second or third opinion =)
```

---
## \#17 Posted by: Takis Posted at: 2017-07-31T15:32:29.801Z Reads: 19

```
I can't see any input in BLDC :stuck_out_tongue:
```

---
## \#18 Posted by: Takis Posted at: 2017-07-31T15:35:15.752Z Reads: 18

```
It will take a lot of stress and I'm trying to find a way to have it cool and I think 12s is better than 10s , I'm also thinking to change from BLDC mode to FOC but many guys say it might destroy the VESC
```

---
## \#19 Posted by: psychotiller Posted at: 2017-07-31T15:36:40.930Z Reads: 18

```
You may need to get a different servo tester. I had the same problem a couple of years ago.
```

---
## \#20 Posted by: Takis Posted at: 2017-07-31T15:37:39.848Z Reads: 17

```
Yes I did that but the throttle works inverted more pulse when free less pulse when pushed
```

---
## \#21 Posted by: Takis Posted at: 2017-07-31T15:38:23.992Z Reads: 17

```
I have one I will try , thanks
```

---
## \#22 Posted by: psychotiller Posted at: 2017-07-31T15:40:00.504Z Reads: 16

```
If it helps, I had to use a servo tester that had the pot dial on it.
```

---
## \#23 Posted by: Takis Posted at: 2017-07-31T15:42:43.506Z Reads: 14

```
Well mine also has but I needed to take it out and bypass the signal from hall sensor to servo
<img src="/uploads/db1493/original/3X/5/6/563f21c8a6766584f3034aa4f252c443241883ff.png" width="281" height="500">
```

---
## \#24 Posted by: psychotiller Posted at: 2017-07-31T15:49:58.222Z Reads: 12

```
I did it differently by soldering the signal wire to the middle pin on the pot if I remember right. Then I adjusted the pot to zero out the signal between forward and reverse.
```

---
## \#25 Posted by: Takis Posted at: 2017-07-31T16:04:10.782Z Reads: 12

```
Mate thanks a lot I fixed it 😁😁
```

---
## \#26 Posted by: psychotiller Posted at: 2017-07-31T16:05:01.287Z Reads: 12

```
Right on!!! Good job
```

---
