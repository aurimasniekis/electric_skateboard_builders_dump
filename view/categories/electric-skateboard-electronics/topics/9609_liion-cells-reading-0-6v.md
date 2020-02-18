# Liion Cells Reading 0.6v?

### Replies: 28 Views: 2242

## \#1 Posted by: michaeld33 Posted at: 2016-09-14T19:13:58.021Z Reads: 101

```
So I tested my liion pack with a multimeter today, it's a 10S pack, reading a voltage of 6V!? There may be a split in one of the wires or something somwhere, but when I measure the individual cells they read between 0.5-1.3v? I only tested a couple but this seems really dangerous! I have no idea how they got this far discharged considering I'm using a VESC, and the limits are set to 30v cutoff...?
Any ideas?
What about the pack? Is it totaled?
```

---
## \#2 Posted by: Pantologist Posted at: 2016-09-14T19:20:12.794Z Reads: 97

```
They're gone if their individual voltage is that low. Internal resistance increases and there cell loses capacity...

I wouldn't charge them again....

Did you short circuit or leave a load on without knowing?
```

---
## \#3 Posted by: michaeld33 Posted at: 2016-09-14T19:21:16.185Z Reads: 94

```
They have shorted before... this sucks, never even used the pack.
```

---
## \#4 Posted by: Pantologist Posted at: 2016-09-14T19:28:05.765Z Reads: 90

```
Dang... Did you have a BMS on it?

One of my multimeter probes fell out of my hands as I was measuring individual cell voltage and it short circuited the pack but my BMS saved it somehow. Not a single volt down or loss of capacity.
```

---
## \#5 Posted by: michaeld33 Posted at: 2016-09-14T19:40:58.314Z Reads: 86

```
Nope, do now tho
```

---
## \#6 Posted by: michaeld33 Posted at: 2016-09-14T19:47:25.311Z Reads: 84

```
  Unfortunately having one now doesn't really help
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-09-14T21:09:17.903Z Reads: 77

```
 All right just got home, took a look at the batteries and measured him with the multimeter again, and I think I must've just overreacted way too quickly earlier because I must not have had proper contact with the pad, because now they read 3 V
```

---
## \#8 Posted by: michaeld33 Posted at: 2016-09-14T21:09:58.656Z Reads: 76

```
<img src="/uploads/db1493/original/3X/9/9/99a3e05677554bc4bea113706dd7b8f726c69bef.JPG" width="375" height="500">
```

---
## \#9 Posted by: Pantologist Posted at: 2016-09-14T21:17:56.832Z Reads: 74

```
Weird... Each one is fine now? Kinda odd that you got that reading for all the cells individually. Maybe you had flux or adhesive on your probes.
```

---
## \#10 Posted by: michaeld33 Posted at: 2016-09-14T21:19:42.823Z Reads: 74

```
 Yeah I think my probes have been like coated with something, I think I might've used one of them to  scratch something recently, and that may have left a coating on them 😬...  I had only measured like three or four cells originally
```

---
## \#11 Posted by: sl33py Posted at: 2016-09-14T21:19:46.501Z Reads: 75

```
Dude - that's awesome!  i was bummed for you when i thought your pack was dead.  that's some serious $ down the drain if it's dead.

I might check each individual cell w/ your MM and just confirm none have any issue.  Did you also wire your pack for balancing already?  I don't see any balance leads in the picture above your MM?  

Fingers crossed and GL!
```

---
## \#12 Posted by: michaeld33 Posted at: 2016-09-14T21:22:29.948Z Reads: 73

```
 I originally thought the issue with having to do  with the battery, when the VESC and the LCD were not lighting up, But it happened to be that the XT 90 anti-spark blew up… As far as I believe.  I just took a look at my XT90S, and it's bulging and very hot
```

---
## \#13 Posted by: sl33py Posted at: 2016-09-14T21:37:56.225Z Reads: 69

```
[quote="michaeld33, post:12, topic:9609"]
I just took a look at my XT90S, and it's bulging and very hot
[/quote]


Pic?  Wonder if you have too long of a "loop" and smaller wire or resistance caused an issue?
```

---
## \#14 Posted by: michaeld33 Posted at: 2016-09-14T21:40:07.286Z Reads: 66

```
It's actually not a loop key, just the connector on the battery... Is that not recommended?
```

---
## \#15 Posted by: michaeld33 Posted at: 2016-09-14T21:40:43.885Z Reads: 64

```
I'm going to switch it out to be an xt90s loop key and a regular xt90 battery connector
```

---
## \#16 Posted by: sl33py Posted at: 2016-09-14T21:47:12.225Z Reads: 64

```
the direct connect w/o it being a loop key is actually preferred.

sounds like a qc issue, or you didn't fully seat it - so it was running through the resistor section of the connection?
```

---
## \#17 Posted by: sl33py Posted at: 2016-09-14T21:47:54.653Z Reads: 60

```
[quote="michaeld33, post:15, topic:9609, full:true"]
I'm going to switch it out to be an xt90s loop key and a regular xt90 battery connector
[/quote]


That's what i do, simply so i don't need a ton of the anti-spark connectors (one for ea battery) vs a single loop key for all batteries.
```

---
## \#18 Posted by: michaeld33 Posted at: 2016-09-14T21:48:17.366Z Reads: 64

```
I don't think it was properly connected.
```

---
## \#19 Posted by: michaeld33 Posted at: 2016-09-14T21:48:59.803Z Reads: 63

```
Ahh so you use the anti-spark side as the actual key, and the female end in the board so you only one key? Interesting...
```

---
## \#20 Posted by: sl33py Posted at: 2016-09-14T21:55:46.687Z Reads: 56

```
Yep!  I did a quick how-to.  Remedial, but for your perusal:

http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

Simple and works.  Just don't do a huge loop.  Paracord works well if you need a handle...
```

---
## \#21 Posted by: michaeld33 Posted at: 2016-09-14T21:56:57.612Z Reads: 54

```
Cool! I have an XT-60 loop key on my old board board which works pretty well...
```

---
## \#22 Posted by: michaeld33 Posted at: 2016-09-15T03:27:12.506Z Reads: 48

```
So I charged the pack, and it reads the correct voltage... But I'm not sure, I tried to measure the amp output of the pack when connected to the VESC, or even just a voltage monitor, and it read ~3.5A. But it wouldn't go on. Now I thought it may have to do with the BMS, so I connected it just as I would without a BMS (even though the BMS was still soldered on) and it still only pulled ~3.5A, and still didn't have enough power (or too much? though I doubt it) to turn on the VESC or display... Is there something wrong? Why would this be happening? Does it have to do with the BMS?
```

---
## \#23 Posted by: Namasaki Posted at: 2016-09-15T05:08:17.774Z Reads: 46

```
[quote="Pantologist, post:4, topic:9609"]
One of my multimeter probes fell out of my hands as I was measuring individual cell voltage and it short circuited the pack but my BMS saved it somehow. Not a single volt down or loss of capacity.
[/quote]


If your using a Bestech BMS, They have exterior short circuit protection.
```

---
## \#24 Posted by: michaeld33 Posted at: 2016-09-15T13:23:57.122Z Reads: 40

```
The BMS was also really hot... But I believe that was from charging
```

---
## \#25 Posted by: michaeld33 Posted at: 2016-09-16T13:25:00.117Z Reads: 33

```
Ok, well I figured it out. It was the crappy BMS, it was preventing the battery from properly discharged, so I took it off. I've been waiting for the supower BMS for like a month now and I have no idea where it is? But I will use that when I get it. It works now though!
```

---
## \#26 Posted by: Namasaki Posted at: 2016-09-17T05:54:39.324Z Reads: 26

```
What brand of BMS was the bad one?
Supower Bms are good but they are really struggling with shipping to USA
```

---
## \#27 Posted by: michaeld33 Posted at: 2016-09-17T12:02:11.927Z Reads: 23

```
I emailed supowerbattery and they told me it was sent back because of the heightened security around the g20 summit. The sent it back and gave me the new tracking number.
```

---
## \#28 Posted by: Namasaki Posted at: 2016-09-17T14:49:23.177Z Reads: 20

```
I had the same problem with them so I got a refund and bought from Bestech instead and they had no problem delivering quickly.
```

---
