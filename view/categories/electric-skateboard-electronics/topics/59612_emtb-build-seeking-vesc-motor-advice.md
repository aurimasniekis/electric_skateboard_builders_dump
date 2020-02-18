# eMTB build: seeking Vesc/motor advice

### Replies: 5 Views: 270

## \#1 Posted by: Atxraider Posted at: 2018-06-21T13:41:59.480Z Reads: 64

```
So I’m in process of building an eMTB using following:

*MBS Atom 95x board
*SPACE Cell battery + enclosure from Enertion dual belt motor
*Dual VESC-x 4.12
*switched from using canbus to Y-connection to receiver for enertion nano remote 
*front & rear Mountainboard trucks kit from Amazon/L-faster, includes dual motors with the following specs:
Model: N6374
Voltage: 36 Volt
Output: 2800 Watt
Rotate: 230KV
Rated Current: 120A 

So, I know it’s not gonna be up to par w the trampa builds I’ve seen on here, so please spare me those kinds of comments. 

Questions I have are:
*should I run it in FOC since motors are sensored, or just stick w BLDC
*are 230Kv motors too high, especially since I’m about 220lbs?
*if I do BLDC anyway to stop the jittering/stuttering of motors on startup from stop, or avoid having to push start?
*what setting in BLDC TOOL do you recommend? Currently have motor max set at 50, should I go to 60?

Thanks in advance!
```

---
## \#2 Posted by: TheMrLarin Posted at: 2018-06-21T14:14:23.758Z Reads: 51

```
About running FOC from what i've heard I wouldn't run it... It apparently burns out the VESC 4.12... I ran it for a bit before switching back to bldc after reading about the FOC tendency to be unreliable.

You can run BLDC mode sensored though. 

Have fun building.
```

---
## \#3 Posted by: ksfacinelli Posted at: 2018-06-21T18:39:19.630Z Reads: 43

```
I am using Focbox on MTB with dual 6374 - sensored and 10s5p and it is just so smooth. I also recommend can bus communication between modules.
```

---
## \#4 Posted by: Atxraider Posted at: 2018-06-21T23:28:50.619Z Reads: 27

```
Okay, thank you both. 

I also have 2 new FOCBOXs that I could switch out w the current dual Vesc-x 4.12, if you think there would be any benefits. Only reason I’m using the older vesc’s is bc they were already connected to battery and in enclosure I took off my old enertion dual belt driven board.....and they still work.
```

---
## \#5 Posted by: TheMrLarin Posted at: 2018-06-22T00:58:21.036Z Reads: 22

```
I'd go with the FOCBOXs
```

---
