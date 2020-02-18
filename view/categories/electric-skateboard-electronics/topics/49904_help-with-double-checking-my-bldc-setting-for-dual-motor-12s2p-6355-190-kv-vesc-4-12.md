# Help with Double Checking My BLDC setting for Dual Motor &#124; 12s2p &#124; 6355 190 KV &#124; VESC 4.12

### Replies: 10 Views: 625

## \#1 Posted by: threebysix Posted at: 2018-03-23T06:27:24.116Z Reads: 89

```
Hi everyone,

I'm starting my first DIY build with parts purchased from TorqueBoards. I will be running dual motor & dual VESC using CanBus. The parts are not here, yet. But I have been doing a lot of research and I want to get my BLDC settings down for each VESC to familiarize myself with it before my parts arrive.

I mostly built this board for long range distance and riding bike paths, a lot of sidewalks, and occasional hills. I'm pretty light weight, around 120lb. I prefer a mellow/gentle balance between torque and speed. I'm do not need insanely high speed or high torque (for now).

Main components from TB are:
 - 12s2p 18650 30Q battery pack (44.4V, 6Ah, 266.4Wh) with BMS (30A continuous / 80A Max)
 - VESC 4.12 
 - 6355 190 KV 
 - 16/36T
 - 12mm belt
 - Mostly likely ABEC 107mm or 90mm 

The settings I have come up with for each VESC is:

 Motor Max: 65A
 Motor Min: -60A
 Battery Max: 30A
 Battery Min (Regen): -8
 Abs Max: 140

 Min Input: 8V
 Max Input: 57V
 Battery Cutoff Start: 36V
 Battery Cutoff End: 33.6

 Min ERPM: -60K
 Max ERPM: 60K
 Max ERPM at Full Break: 300
 Max ERPM at Full Break in Current Control: 1500
 "I Unchecked limit ERPM with negative torque"

Please let me know if these settings are optimal for my setup. Thank you to everybody in advance.
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-03-23T06:53:47.033Z Reads: 81

```
[quote="threebysix, post:1, topic:49904"]
Min Input: 8V
Max Input: 57V
[/quote]

I recommend:
Min Input: 36V
Max Input: 60V

Not sure what the battery cutoff "start" and "end" are. :thinking:
```

---
## \#3 Posted by: scepterr Posted at: 2018-03-23T06:56:03.622Z Reads: 80

```
No max input shouldn't be changed to 60v, please explain why you would suggest this
```

---
## \#4 Posted by: ZackoryCramer Posted at: 2018-03-23T06:56:39.295Z Reads: 80

```
I just don't want the vesc cutting me off on a break spike. Idk, maybe 3v of difference means frying the drv, but I'd rather have the drv pushed to the limits to save you than giving up and leave flying down a hill. :butterfly:
```

---
## \#5 Posted by: scepterr Posted at: 2018-03-23T06:58:39.605Z Reads: 79

```
Sorry didn't realize it was 12s, 36 is fine for that, but max input should not be changed, its to protect the drv
```

---
## \#6 Posted by: threebysix Posted at: 2018-03-23T06:59:21.119Z Reads: 80

```
The battery cutoff and start values were obtained from Ackmaniac's reply here for 12s :

http://www.electric-skateboard.builders/t/critique-my-vesc-settings-12s4p-dual-6355-190/32110/3?u=threebysix

Would this be not the right config?
```

---
## \#7 Posted by: threebysix Posted at: 2018-03-23T07:05:09.294Z Reads: 76

```
That's what I had read as well. IIRC, Someone posted saying how Vedder said 57V is better for VESC..
```

---
## \#8 Posted by: threebysix Posted at: 2018-03-23T07:18:33.274Z Reads: 74

```
What would be the different in min input of 8v versus 36v in term of performance? How do I calculate min input?
```

---
## \#9 Posted by: scepterr Posted at: 2018-03-23T07:23:48.338Z Reads: 69

```
Performance is the same, that's the voltage the vesc will shut off at
Min/max you can leave default 8/57

And just adjust battery cut start/end 38.4/36
```

---
## \#10 Posted by: threebysix Posted at: 2018-03-23T07:37:08.001Z Reads: 65

```
Gotcha, thanks for the info!
```

---
