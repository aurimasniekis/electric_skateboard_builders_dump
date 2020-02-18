# Dual BLDC - Single VESC works :)

### Replies: 9 Views: 1684

## \#1 Posted by: JTAG Posted at: 2016-12-25T22:14:08.599Z Reads: 241

```
@MrEpiquad asked me to evaluate a little experiment:

 <img src="/uploads/db1493/original/3X/d/7/d7e722a2ec717b523752e19e75b847a1ab06ab53.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/8/4808342f846d6b48e15586a3e464a7644d527986.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/2/3/2313769cc1404c7155b87f3eb3238b3c3f477373.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/8/5/8530368df2ea5753e4845b72163dba37919edb60.jpg" width="666" height="500">

Before doing this we adjusted the rotor such that the rotor flux angle matched (by moving the magnets on the axle of one of the motors until we saw that the output phase / output pattern matched):
<img src="/uploads/db1493/original/3X/1/5/15e650e64d0c7083066b021cc5e99486b6103f4c.jpeg" width="690" height="322">

Succes!:
https://youtu.be/GZkbB82-YBM

No load power is 25 to 30W. We event went to 500W with propeller until we got scared (propeller was not balanced).

#YOLO #difflock #dual motor esk8.
```

---
## \#2 Posted by: mmaner Posted at: 2016-12-25T22:35:12.334Z Reads: 231

```
That is too cool and very interesting.  Would you mind elaborating on the steps you took?  Does this seem to be a production solution to you?
```

---
## \#3 Posted by: chuttney1 Posted at: 2016-12-25T23:37:42.587Z Reads: 221

```
This concept has been shown to work in the RC world with very short lifespan on the ESC. How long would the VESC last like this with varying loads.
```

---
## \#4 Posted by: JTAG Posted at: 2016-12-25T23:43:36.344Z Reads: 220

```
As long as the mechanical coupling stays intact (magnet assembly not moving on the axle) the whole assembly should still act like a normal motor but with half the inductance and halve the resistance. We are going to build a 1.5kW load setup to evaluate the performance over time. Lets hope for the best :smiley:!
```

---
## \#5 Posted by: landonkun Posted at: 2016-12-26T01:57:15.831Z Reads: 203

```
I need to know what is going on with that table.
```

---
## \#6 Posted by: JTAG Posted at: 2016-12-26T01:59:38.484Z Reads: 204

```
That's my force shield for the potential high velocity debris xD.
```

---
## \#7 Posted by: kdee122 Posted at: 2017-01-02T12:19:28.161Z Reads: 169

```
I have done this in the past with pump (without the rotors locked together). I had 2 BLDC pumps and was able to run them off one VESC. We only used them on our test bench for an few hours so i cant confirm the life of the VESC.
```

---
## \#8 Posted by: JTAG Posted at: 2017-01-02T14:40:50.842Z Reads: 154

```
Did you synchronized the rotor? Or just tried on good luck?
```

---
## \#9 Posted by: kdee122 Posted at: 2017-01-02T21:49:52.561Z Reads: 129

```
There was no need to sync the rotors since it was a pump applications. The two motors "found"  the same rotor position during startup and since the load on both pumps was the same they stayed in sync. 

I was a bit surprised it worked.  I image it would not work if the motors have a high start up load like in ground vehicle.
```

---
