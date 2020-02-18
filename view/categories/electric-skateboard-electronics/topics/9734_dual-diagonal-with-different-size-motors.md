# Dual diagonal with different size motors

### Replies: 12 Views: 1256

## \#1 Posted by: caustin Posted at: 2016-09-17T04:31:55.801Z Reads: 161

```
Pulling together a new build with spare parts I have lying around. Was going to match an enertion bigboy 6374 with a tacon Bigfoot 160 in dual diagonal setup for fit. Dual VESC setup on 12s4p. Assume the vescs can match these up, but is this a problem, or need special configuration?    Or other issues I have not thought about yet, or point me to thread that covers this as can't be the first to try this but did not find via search. Any thought advice much appreciated!!
```

---
## \#2 Posted by: saul Posted at: 2016-09-17T04:43:15.628Z Reads: 171

```
tacon on 12s will be too high eRpm. even it it wasn't, it'd be crazy fast!

aside from that with a split pwm line it should probably work, mess with setting for each vesc to matchup/complement torque curves. should be interesting...
```

---
## \#3 Posted by: Dunmer Posted at: 2016-09-17T08:26:52.465Z Reads: 144

```
Also interested in this. I have An sk3 192 single drive now and I was thinking to add a little motor, 50mm or so, in the front in diagonale setup to aid me a little. Curious if it works
```

---
## \#4 Posted by: Dunmer Posted at: 2016-10-03T19:00:42.604Z Reads: 107

```
Nobody tried this untill now? :slight_smile: 
a 192kv rear drive and a 190kv front drive, would it be a problem?
```

---
## \#5 Posted by: caustin Posted at: 2016-10-04T03:13:07.760Z Reads: 99

```
Have to assume that is within the fault tolerances of same spec motors, no?  I am benchtesting 190kv front and rear but different manufacturer so assume in same range if kv delta as your example. In fact one is 6375 and other 6354 so curious if that adds another variable to equation or negligible. Tbd I guess, still on bench not road test yet. You
```

---
## \#6 Posted by: saul Posted at: 2016-10-04T03:52:39.246Z Reads: 94

```
I think with 2 vesc and current control the only issue would be torque steer when the motors don't match up. other then that one motor would just run as if it were going down hill since the other is helping out....

If I can get my 8s pack mounted somehow i might just test this with 2 50mm motors i have... (custom 5050 - 85kv/ 5065 200kv)

but it would just be a proof of concept with printed mounts...
<img src="/uploads/db1493/original/3X/9/9/991eaa876ec75a7c11681169b1ed3bf5ba8d2099.jpg" width="690" height="387">
```

---
## \#7 Posted by: caustin Posted at: 2016-10-04T03:55:31.017Z Reads: 91

```
Let's see what happens,  for science. Though I am running split pwm rather than canbus linked.
```

---
## \#8 Posted by: saul Posted at: 2016-10-04T03:59:00.936Z Reads: 89

```
it should be really interesting if it works!
I would go with split pwm also, i was looking into vedders code for canbus(traction control) and its pretty basic but with some work it could be nice.
```

---
## \#9 Posted by: lowGuido Posted at: 2016-10-04T05:30:16.567Z Reads: 83

```
This seems to be coming up a lot lately. But yeah I have done this before. It works.
Just use split PWM instead of canbus link.
```

---
## \#10 Posted by: Dunmer Posted at: 2016-10-04T08:04:55.260Z Reads: 81

```
Ok cool. Then i will try it out with a smaller size 190kv front motor to aid me a bit. :slight_smile:
```

---
## \#11 Posted by: ekitesurfer Posted at: 2016-10-04T09:35:34.461Z Reads: 72

```
I was running split canbus on 2 different motors, seemed to be working, why is this bad?
```

---
## \#12 Posted by: lowGuido Posted at: 2016-10-04T10:56:38.368Z Reads: 68

```
never said it was bad. just though it would be best to keep the 2 ESC's totally separate.
I suppose as long as the traction control is disabled it should be fine.
```

---
