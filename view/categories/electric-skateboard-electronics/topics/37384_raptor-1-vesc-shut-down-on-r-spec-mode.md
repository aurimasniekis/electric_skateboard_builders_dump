# Raptor 1 VESC shut down on &lsquo;R-Spec&rsquo; Mode

### Replies: 19 Views: 830

## \#1 Posted by: headrec Posted at: 2017-11-05T01:12:22.033Z Reads: 131

```
Hey as of late I've experienced VESC resetting when in R-spec mode only when high amp draw situations happen.  I'm curious if my vesc settings have reset or anything anyone would add

6355 190kv dual setup
10s3p motor

All stock raptor 1 setup outside of 97mm abec 11 wheels.

Curious if I should make any changes to settings or if the extra draw of the 97 mm wheels is causing the VESCs to reset.  Here is a screen shot.  If any other info is needed let me know.

[img]https://i.imgur.com/QAqy6Mf.png[/img]
```

---
## \#2 Posted by: headrec Posted at: 2017-11-05T06:00:53.054Z Reads: 107

```
Bump to the top
```

---
## \#3 Posted by: ARetardedPillow Posted at: 2017-11-05T07:11:25.056Z Reads: 104

```
Limit max rpm to 60k
```

---
## \#4 Posted by: scepterr Posted at: 2017-11-05T07:48:31.519Z Reads: 104

```
Possible that your batteries are sagging below cutoff at high load?
Got any ride charts?
```

---
## \#5 Posted by: headrec Posted at: 2017-11-05T10:58:04.523Z Reads: 96

```
The battery does sag but it will do this even on a bench test at a full charge.
```

---
## \#6 Posted by: scepterr Posted at: 2017-11-05T11:32:48.029Z Reads: 91

```
How much does it sag on the bench....that's not good
```

---
## \#7 Posted by: headrec Posted at: 2017-11-05T17:21:08.970Z Reads: 77

```
It will drop about 12 percent on the initial jump and settle at a 6 percent sag when at full speed on the bench.  Seems like it's been about like this since I got it.
```

---
## \#8 Posted by: headrec Posted at: 2017-11-06T02:17:44.304Z Reads: 67

```
Bump to the top
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-11-06T02:21:24.706Z Reads: 67

```
Get a Bluetooth module to monitor things. It's probably the battery tho
```

---
## \#10 Posted by: headrec Posted at: 2017-11-06T02:27:02.990Z Reads: 63

```
I can understand it shutting off if the battery dropped to a certain extent but I can't see it sagging from 100 to shut off rate right out of the gate on the bench.
```

---
## \#11 Posted by: Titoxd10001 Posted at: 2017-11-06T02:32:27.476Z Reads: 62

```
I think I've read of other raptor batteries going bad. 25rs aren't that great and 10s3p is small for a dual. I have same cells in 12s4p format and they sag a bunch. Going to upgrade that pack soon. Bluetooth module is cheap and ackmaniacs app is free
```

---
## \#12 Posted by: Battosaii Posted at: 2017-11-06T07:28:10.480Z Reads: 52

```
check your vesc capacitors, i had mine fail on my Raptor and i could not fully accelerate or the vesc would shut off, after i replaced the caps this thing rips again.
```

---
## \#13 Posted by: headrec Posted at: 2017-11-07T00:45:20.026Z Reads: 47

```
[quote="Battosaii, post:12, topic:37384, full:true"]
check your vesc capacitors, i had mine fail on my Raptor and i could not fully accelerate or the vesc would shut off, after i replaced the caps this thing rips again.
[/quote]

How do you check the capacitors?
```

---
## \#14 Posted by: headrec Posted at: 2017-11-07T00:45:35.886Z Reads: 48

```
[quote="Titoxd10001, post:11, topic:37384, full:true"]
I think I've read of other raptor batteries going bad. 25rs aren't that great and 10s3p is small for a dual. I have same cells in 12s4p format and they sag a bunch. Going to upgrade that pack soon. Bluetooth module is cheap and ackmaniacs app is free
[/quote]

I'm a little worried about that.
```

---
## \#15 Posted by: Battosaii Posted at: 2017-11-07T10:57:58.092Z Reads: 37

```
in my case one of the soldered leads was broken off the capacitor i was able to move the capacitor up off the pcb. in theory i could have soldered it back but i had already ordered new capacitors from Axel. Also if the capacitor looks "puffed" up its bad the metal cap on top should be completely flat if its domed or puffed its bad.
http://www.markdigital.com/wp-content/uploads/2011/02/bulging_capacitors.jpg
```

---
## \#16 Posted by: headrec Posted at: 2017-11-08T01:16:10.351Z Reads: 39

```
[quote="Battosaii, post:15, topic:37384, full:true"]
in my case one of the soldered leads was broken off the capacitor i was able to move the capacitor up off the pcb. in theory i could have soldered it back but i had already ordered new capacitors from Axel. Also if the capacitor looks "puffed" up its bad the metal cap on top should be completely flat if its domed or puffed its bad.
[/quote]

Capacitors all look good to go and solidly connected.
```

---
## \#17 Posted by: headrec Posted at: 2018-04-01T17:17:09.148Z Reads: 30

```
Bump this to the top.  Weather is finally getting good again and looking to ride.  

Again rides fine in normal mode but switching to R spec mode the VESC shut down riding and on the bench test as well.
```

---
## \#18 Posted by: fakesantos Posted at: 2018-05-17T14:05:57.878Z Reads: 20

```
I have the same problem with my Bolt Motion. I have two speeds. At slower speed, everything is great. At faster speed, the board resets often (every 30 seconds?). Even more frequently going up a hill.  Not sure what the problem is either. Any luck?  Did you try the capacitor thing?
```

---
## \#19 Posted by: headrec Posted at: 2018-05-17T14:36:24.538Z Reads: 13

```
Still haven't figured it out. Capacitors seem fine.
```

---
