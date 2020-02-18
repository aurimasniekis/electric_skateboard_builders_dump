# eSk8 will not carry any weight

### Replies: 16 Views: 1452

## \#1 Posted by: sprocket12 Posted at: 2016-08-08T08:53:33.180Z Reads: 188

```
First build and noob question.  Can't find any pertinent info that relates to my issue.  I got the board set up and I thought configured but when I went for a first 'test' ride, the board would take no weight.  When no weight on board the powered wheel spins fine.  When starting at a roll while standing on board, the motor tries to go but just strains against belt and motor mount.

Things that should make it go consist of:

* 8s3p (18650's with 90-100% charge- verified to VESC)
* VESC 4.12
* Turing Aerodrive SK3-6354-260kv motor
* TorqueBoards 2.4GHz mini remote (configured and working)

I've followed what I thought was needed in configuring VESC but clearly am not getting enough torque. 
All help is appreciated.
```

---
## \#2 Posted by: kampfhahn Posted at: 2016-08-08T08:58:39.320Z Reads: 186

```
Does "configured and working" means, that your remote covers the complete 0-100% span in the "display" section of the bldc tool? I could imagine that you reach 100% power immediately when pushing the remote even just 1mm and the VESC then failsafes.
```

---
## \#3 Posted by: flatsp0t Posted at: 2016-08-08T08:59:46.427Z Reads: 176

```
Could you provide some BLDC-tool Screenshots please?

Maybe there is something wrong with the battery or motor config.
```

---
## \#4 Posted by: sprocket12 Posted at: 2016-08-08T09:10:51.030Z Reads: 159

```
<img src="/uploads/db1493/original/2X/5/53b85e3acd6c9f7df4a64e604aa1d26fc7950748.png" width="690" height="431"><img src="/uploads/db1493/original/2X/1/15c2467141bd6155d1eb28a8fffc150da4cd618b.png" width="690" height="431"><img src="/uploads/db1493/original/2X/a/ab8f3b53b8385024fb3a85681578103e07c777c7.png" width="690" height="431">
```

---
## \#5 Posted by: sprocket12 Posted at: 2016-08-08T09:13:56.435Z Reads: 136

```
If you mean the remote shows the pulse width covering the full 0-100%, then yes.  I adjust it slightly to offset motor running when first turned on with no trigger pull.
```

---
## \#6 Posted by: kampfhahn Posted at: 2016-08-08T09:19:15.780Z Reads: 133

```
25A batt max is a very low value and reached very fast when accelerating an 8s setup. What kind of batterys are you using?

EDIT: Got it: Your battery cut off values don´t fit your 8s but a 10s setup, that´s why your VESC doesn´t provide any power because it´s saving the battery from deep discharge. Change the values to 28/27 and you should be ready to ride.
```

---
## \#7 Posted by: sprocket12 Posted at: 2016-08-08T09:24:40.166Z Reads: 133

```
Awesome!  Thank you for the help. My insomnia is over (it's 2:23 am here). I'll try it in the morning. 

Thanks again
```

---
## \#8 Posted by: thisrealhuman Posted at: 2016-08-08T09:26:11.026Z Reads: 134

```
What is your drive ratio?  if its 36t/15t and 83mm you are probably too steep for the limited current.
```

---
## \#9 Posted by: elkick Posted at: 2016-08-08T12:55:32.975Z Reads: 118

```
Your battery cutoff start/end values are way to high for 8s (should rather be something around 26/24V). Also, why are you using multiple VESCs over CAN in the app tab, are you on a dual motor setup? And as mentioned, battery max. should be higher too.

Edit: Sorry, overlooked the posting of kampfhahn mentioning the same. :slight_smile:
```

---
## \#10 Posted by: chaka Posted at: 2016-08-08T13:40:46.188Z Reads: 103

```
Yes, you voltage cutoffs are way too high but your pack is also very small for 18650's. You should drop your motor max down to 30 amps .
```

---
## \#11 Posted by: sprocket12 Posted at: 2016-08-08T15:17:38.467Z Reads: 95

```
Thanks to all (@kampfhahn, @elkick, and @chaka) who caught the voltage issues.  I was able to get moving by lowering the battery cutoff limits.

@elkick- I don't know hwy I had dual VESC's set.  Unless that is default.  I have rectified that too.

Related to this, even though I can now ride under power, I need to ramp my speed up *really* slowly.  I can't even be rolling much at start.  Any suggestions/thoughts?  Would this be related to the "APP Configuation" -> "PPM" tab settings?
```

---
## \#12 Posted by: sprocket12 Posted at: 2016-08-08T15:19:25.763Z Reads: 88

```
@thisrealhuman, I don't know the gear ratio.  It is an Enertion set up I bought from a fellow eSk8 builder.
```

---
## \#13 Posted by: elkick Posted at: 2016-08-08T19:39:13.966Z Reads: 74

```
[quote="sprocket12, post:11, topic:7299"]
I don't know hwy I had dual VESC's set.  Unless that is default.  I have rectified that too.
[/quote]

Seems to be Enertiin default even on single setups.
```

---
## \#14 Posted by: sprocket12 Posted at: 2016-08-08T20:07:10.233Z Reads: 70

```
@chaka- thanks.  I've dropped the motor max down to 30 amps.
```

---
## \#15 Posted by: sprocket12 Posted at: 2016-08-09T22:15:09.427Z Reads: 46

```
What should the batt max be?  How do I calculate this?
```

---
## \#16 Posted by: kampfhahn Posted at: 2016-08-10T06:26:39.248Z Reads: 37

```
It depends on which batterys you are using and what their max. discharge rate is.
```

---
