# Dual Raptor: 2-speed drivetrain using remote buttons?

### Replies: 13 Views: 1450

## \#1 Posted by: bucksd Posted at: 2016-10-02T01:35:54.801Z Reads: 185

```
Had a thought, just for fun, and am wondering if it's possible:

I have a Dual Raptor. Could I put different gearing on each motor (one for acceleration and the other for top speed) and program one of the remote buttons to switch between controlling one motor vs the other?

Effectively, it would create a 2-speed drive system: use the motor geared for acceleration from 0-20mph, then hit a button on the remote to start controlling the other motor which would be geared for something like 15-35/40mph?

I think the motors are capable of doing 35mph when used together. Not sure what the top speed would be for a single motor.

Just seemed like a fun idea. Plus, you'd probably get more range since you're only using one motor at a time and with a more efficient gear ratio all the time.
```

---
## \#2 Posted by: bucksd Posted at: 2016-10-02T01:37:05.429Z Reads: 177

```
I'm sure there's a good reason this is a bad idea, mainly based on the fact that Tesla doesn't do this...
```

---
## \#3 Posted by: chinzw Posted at: 2016-10-02T01:52:11.434Z Reads: 170

```
You can definitely program the VESC to act this way, but it will require quite a bit of programming.
```

---
## \#4 Posted by: ra.rend Posted at: 2016-10-02T02:46:17.234Z Reads: 160

```
Use two remotes :D
```

---
## \#5 Posted by: treenutter Posted at: 2016-10-02T03:50:28.533Z Reads: 146

```
I believe @lowGuido did an experiment a while back with two different motors (one with higher Kv, The other lower). It worked alright if I recall. He used the same gearing on each wheel. 

It's an interesting concept @bucksd
```

---
## \#6 Posted by: Namasaki Posted at: 2016-10-02T04:07:39.905Z Reads: 146

```
Sounds like pure madness to me!
I think a better solution is to build a quad drive and gear it for speed.
Just having 4 motors should give plenty of torque.
```

---
## \#7 Posted by: thisrealhuman Posted at: 2016-10-02T04:44:47.424Z Reads: 137

```
Use the steering channel to control the second esc, design a remote with two triggers.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-10-02T06:48:07.036Z Reads: 121

```
Or just let both motors run at the same time but with different gearings or kv. This way the acceleration will be the smoothest. You could also modify the firmware to change from one motor to the other at a specific speed but I think to always run them at the same time is the best idea. 
But if they run at the same time then traction control needs to be switched off.
```

---
## \#9 Posted by: lowGuido Posted at: 2016-10-02T07:45:24.639Z Reads: 109

```
It isnt an experiment anymore. Its a street rocket tha gets ridden regularly.  Its Fast!
```

---
## \#10 Posted by: bucksd Posted at: 2016-10-02T19:08:09.606Z Reads: 102

```
@lowGuido Do you have a link to your build or can you comment on the results of running two different motors?
```

---
## \#11 Posted by: lowGuido Posted at: 2016-10-02T21:18:43.665Z Reads: 100

```
http://www.electric-skateboard.builders/t/uneven-dual-rear-drive/
```

---
## \#12 Posted by: laurnts Posted at: 2016-10-02T21:25:15.003Z Reads: 96

```
@lowGuido uneven dual drive will solve this problem. If you put uneven motor or uneven gearing, both motor will eventually balance out each other torque, giving you balance drive for both worlds. This is very beneficial especially combined with VESC current control as both motor will eventually will run max speed with the slightest touch on the controller.
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-07-25T04:15:40.175Z Reads: 39

```
I tried an extreme version of this and it didnt work very well. 130kv hub with a 70kv hub. End result was slightly better acceleration and a big drop in stop speed. Once the 70kv motor reached its no load max speed it started fighting against the 130kv hub that still wanted another 15mph. The drag was very noticeable.
```

---
