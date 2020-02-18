# Thoughts of mixed Kv

### Replies: 13 Views: 505

## \#1 Posted by: IndyPilot Posted at: 2019-05-03T11:36:12.133Z Reads: 242

```
I was lost deep in thought about things mechanical rather than the loved ones surrounding me...mechanical contraptions are a drug...

Is there any benefit to running 2 different motors, one low geared low KV, the other high geared and high KV?  For acceleration and top speed (race) or for varying terrain (flat to hill transition; pavement vs gravel/sand/grass$?  Only one motor would be on at a time and the handover (gear shift) would be electronically managed.  Would the parasitic drag of the off motor negate any benefits?  Could the off motor do some charging?

Like I said, thoughts of an idiot who should be more focused on the here and now, lol.
```

---
## \#2 Posted by: yelnats8j Posted at: 2019-05-03T11:40:18.535Z Reads: 237

```
https://www.electric-skateboard.builders/t/what-happens-if-2-motors-different-kvs/55179?u=yelnats8j
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-05-03T11:50:00.437Z Reads: 226

```
I dont think traction control works though, you should probably turn that off if youre going to do different KVs
```

---
## \#4 Posted by: Jinra Posted at: 2019-05-03T15:50:21.282Z Reads: 167

```
https://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113
```

---
## \#5 Posted by: maxchilton Posted at: 2019-05-03T16:12:40.179Z Reads: 143

```
You could have a belted drive attached to a hub motor.  The belted drive would be geared very high for massive torque, the motor pulley would have freewheel pulley, so once the belted drive maxes out the hub drive takes over and provides top speed.
```

---
## \#6 Posted by: Andy87 Posted at: 2019-05-03T16:21:44.699Z Reads: 136

```
Don’t forget that this would decrease the free roll as well.
```

---
## \#7 Posted by: thisguyhere Posted at: 2019-05-03T16:24:46.272Z Reads: 133

```
sorry to derail.

@maxchilton are you THE max chilton, former f1 driver?
```

---
## \#8 Posted by: Hummie Posted at: 2019-05-03T17:14:49.270Z Reads: 117

```
no one has logged data that ive seen while doing two drastically different kv but it really shouldnt make much difference.  be nice to see the current draw and if the motors are putting out the same torque or not.   would really also depend on your settings but assuming they were the same for both motors   

  you'll be limited to a top speed determined by the higher kv.  in fact you could end up with two motors fighting each other if you hit throttle at full speed with different kv as the lower kv motor when you throttle if it's beyond it's no-load speed it will brake.  

traction control wouldnt be effected and super nice.
```

---
## \#9 Posted by: Gamer43 Posted at: 2019-05-05T07:48:04.962Z Reads: 73

```
No

The low kv motor acts as a generator above a certain speed and will start rectifying current back into the battery through the ESC MOSFET body diodes. This effectively limits your speed to max speed of the low kv motor.

Unless you disconnect the ESC completely (this can be accomplished using relays, but the ESCs will NOT like the switchovers. 

Better off trying to figure out how to implement a wye-delta starter in these motors xD. That's what larger motors, especially ones used in industrial machinery, employ.
```

---
## \#10 Posted by: b264 Posted at: 2019-05-05T08:12:11.980Z Reads: 64

```
If you wrote some custom firmware and used CANBUS this could be really neat, but without custom firmware that you make yourself, you're limited to the limitations others have pointed-out.  Also, you'd probably need some custom hardware as well.
```

---
## \#11 Posted by: Hummie Posted at: 2019-05-05T21:02:47.819Z Reads: 43

```
regardless of kv the motor will get just as hot if doing the some torque output so there’s no normal benefit running different kv.  U could limit the erpm of the higher kv motor so the low kv motor doesn’t end up becoming a brake when beyond it’s no-load speed when u throttle. If u do that you’re safe in that regard.
```

---
## \#12 Posted by: b264 Posted at: 2019-05-05T23:45:49.232Z Reads: 25

```
But with custom firmware you could just not send power to that unit in those conditions.  If its back EMF exceeded your system voltage you may start to have issues, though.  You also may need custom hardware if it's bleeding through the FET body diodes.
```

---
## \#13 Posted by: Wilsonliang777 Posted at: 2019-05-06T01:21:33.325Z Reads: 22

```
Using 2 different kv motor is almost the same as using 2 different gear ratio system.  Like same kv when gear 40/15 and 40/12 gears.
```

---
