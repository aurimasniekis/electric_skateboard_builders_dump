# VESC 147A Motor Current - &ldquo;Abs Over Current ERROR&rdquo;

### Replies: 5 Views: 1693

## \#1 Posted by: upgration Posted at: 2016-07-22T16:58:39.378Z Reads: 258

```
Hi guys,

today I flashed my home made(soldered everything 
manually) VESC and everything seemed fine, until I tried to detect the 
motors parameters. It only jumped a bit and then stopped. The bldc tool 
says:"bad detection result received".  In order to narrow down the error
 I disconnected the motor from the vesc. However in the realtime data tab 
it says:" Fault code abs over current". The motor current says: 147A, 
which obviously is not correct, since the battery current is less than 
0.2A. So these two results doesn't sound good. For the VESC I used 
0,5mOhm shunt instead of 1mOhm... Can this fact cause such an error? I 
did a continuity test for the MOSFETS circuit and there where no shorts 
or solder bridges.

If anyone has an explanation for the errors I get or even has a suggestion to solve the problem I'd appreciate it.

Thanks,
Oliver
```

---
## \#2 Posted by: Jeff Posted at: 2016-07-22T17:17:02.944Z Reads: 248

```
was anything (like a belt) hooked up to the motor when you ran the detection?
```

---
## \#3 Posted by: upgration Posted at: 2016-07-22T17:27:55.685Z Reads: 241

```
Hi Jeff,

no the motor could have spun freely. Sorry if I expressed myself in an unclear way... After my first failed test I disconnected the Motor completely from the vesc. The over-current error appears if I connect a battery to the vesc and connect it to the bldc tool without a motor connected to it.
```

---
## \#4 Posted by: upgration Posted at: 2016-07-22T18:39:37.496Z Reads: 231

```
Also I just noticed that the vesc draws power the whole time without doing anything. It's around 4.4Watts. Maybe knowing this helps finding a solution
```

---
## \#5 Posted by: upgration Posted at: 2016-07-22T20:35:00.994Z Reads: 208

```
Solved it. One of the shunts wasn't soldered correctly. One of the two small pins didn't have contact with the smd pad.
```

---
