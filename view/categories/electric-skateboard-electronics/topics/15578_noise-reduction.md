# Noise reduction?

### Replies: 11 Views: 1822

## \#1 Posted by: ayospringroll Posted at: 2017-01-03T09:23:42.151Z Reads: 163

```
I noticed that when other people ride my electric skateboard that the motor is really loud. Its so loud I could hear it coming from all the way up my street. Im interested to know if there is a way to reduce the noise coming from the motor? Im running a 6s system with a VESC and a 200kv 6374 motor.
```

---
## \#2 Posted by: jbruce Posted at: 2017-01-03T09:27:14.737Z Reads: 163

```
FOC mode!!
```

---
## \#3 Posted by: ayospringroll Posted at: 2017-01-03T09:48:09.096Z Reads: 162

```
would you recommend using FOC? I heard of vescs breaking from using this.
```

---
## \#4 Posted by: JTAG Posted at: 2017-01-03T14:31:11.742Z Reads: 146

```
We have build 7 skateboards mixed single and dual motor all on 6S all on FOC. It is super quiet :).
```

---
## \#5 Posted by: evoheyax Posted at: 2017-01-03T15:51:03.217Z Reads: 138

```
I run exclusively on FOC. I have 8 vescs in FOC and not one has broken. But they are chaka vescs, which means they are are beefed up and less likely to break in the first place.
```

---
## \#6 Posted by: wmj259 Posted at: 2017-01-03T15:59:36.433Z Reads: 131

```
Will have to go this way, any difference notable other then noise reduction?
```

---
## \#7 Posted by: treenutter Posted at: 2017-01-03T16:01:20.228Z Reads: 131

```
@ayospringroll yes FOC mode! Make sure to re-update your VESC firmware to reset everything before you try it. Some folks speculate that old settings from previous modes can interfere with the transition. Not sure if that has been corrected.
```

---
## \#8 Posted by: evoheyax Posted at: 2017-01-03T16:09:53.515Z Reads: 127

```
Slightly more torque and slightly less top speed, in addition to the massive noise reduction.
```

---
## \#9 Posted by: mccloed Posted at: 2017-01-03T19:08:07.749Z Reads: 109

```
I, too, run exclusively on FOC. Two Chinese VESC's on two separate boards and two torqueboards VESC's on a mountainboard. All on 10s with no problems, so far. :+1:
```

---
## \#10 Posted by: ayospringroll Posted at: 2017-01-03T19:09:45.988Z Reads: 106

```
Thank you everyone! I switched over to FOC and I am loving it! I got an instant noise reduction which is perfect. The only thing I did notice was the loss of top speed but I can live with that.
```

---
## \#11 Posted by: ayospringroll Posted at: 2017-01-04T01:45:41.258Z Reads: 85

```
I have one more question. If you were using BLDC before switching to FOC did you guys keep the same settings?
```

---
