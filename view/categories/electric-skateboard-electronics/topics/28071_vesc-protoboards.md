# Vesc Protoboards

### Replies: 11 Views: 855

## \#1 Posted by: marcoluz Posted at: 2017-07-20T00:51:44.172Z Reads: 203

```
I would love to know how and why my vesc with a few miles only just died without any reason while I was eskating on flat concrete. I have a dual setup and everything was setup nice and adjusted. Eskating is great, I loved it!!! But man... it is getting to expensive. There is always something to fix again.
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-20T00:58:01.147Z Reads: 202

```
Do you have screenshots of your settings? It was most likely not the hardware but in your settings that caused the fried vesc
```

---
## \#3 Posted by: sl33py Posted at: 2017-07-20T03:28:04.098Z Reads: 181

```
what's your setup?  

Wheels - Motor (kv) - Voltage - Gearing ?

Would want to make sure you were below 60k ERPM.

Did both die?  or just one?

If it's just the DRV the repair isn't that hard if you can reflow, or send for repair and be back up and running in decent time!

GL!
```

---
## \#4 Posted by: marcoluz Posted at: 2017-07-20T11:13:51.211Z Reads: 143

```
<img src="/uploads/db1493/original/3X/1/0/1020e17b211a70f83ce0d5741287be73e3e3c0ec.png" width="690" height="408"><img src="/uploads/db1493/original/3X/8/3/832a24ebb57c97ca8e2cb10a0e5831b4291d7888.png" width="690" height="403"> this is only from the vesc that hasn't burned. the other can't even connect it.
```

---
## \#5 Posted by: marcoluz Posted at: 2017-07-20T11:20:13.036Z Reads: 126

```
Hi there,

My setup is:

6s 10Ah 
Dual vesc
Dual 190kv motor
97mm ABEC11
Antispark switch
Gearing 36/15

Vesc are not connected to each other, they are both independent, I control them thru the receptor (dual connection). Just one vesc died.

What is the DRV? I am not that expert :slight_smile: 

Thanks for the help!
```

---
## \#6 Posted by: sl33py Posted at: 2017-07-20T18:24:23.804Z Reads: 106

```
This look about right - top speed approx 18mph?:

<img src="/uploads/db1493/original/3X/6/e/6e4da5f3db973803056990082bf5f0ea9252a042.png" width="690" height="476">

Nowhere near the 60k ERPM limit and see you have it limited in the software as well.

DRV chips fail.  If it's not the 60k ERPM limit which is pretty much guaranteed to fry the DRV chip - sometimes they just die on their own.  

The chip is not simple to replace as you need hot air or SMD rework skill/experience.  It's not rocket science, but it is very small/detailed work and not something i'd recommend w/ a simple soldering iron you try.  The replacement chip is about $6-8 ea, and there are some folks online who will repair.  You'll have to dig as i'm not familiar with who does this, and it likely would be better to keep to someone in your area vs shipping around the globe.  

HTH - GL!
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-20T20:16:33.772Z Reads: 81

```
DRV8302 is the long ic chip on the VESC it's responsible for firing off the fast signals to the MOSFETs (big black square components down where the motor leads connect, control flow of power to the coils).  The VESC also has another ic on it for the main processing of input signals and data collection and doing the configuration called a STM32 it's an ARM architecture processor like those in cell phones or raspberry pis.  Anyhow unnecessary detail but those are the main components on the board outside of capacitors resistors and I think one inductor, the thing that blows out or fries most often is the drv chip though.  Forget who it is here that does replacements it is pretty hard to do if you aren't familiar with smd reworking though (I tried on one I blew but failed)
```

---
## \#8 Posted by: ninja Posted at: 2017-07-20T20:33:04.409Z Reads: 72

```
In your screen shots mot. min. is higher than mot. max.

Is mot. min. supose to be same or lower than mot. max.? 

Anybody...?
```

---
## \#9 Posted by: marcoluz Posted at: 2017-07-21T12:03:15.371Z Reads: 63

```
Well, that's some good and useful information! I am going to try to fix it for sure. Don't want to waste more 150€ for another vesc. Thank you so much for the advices! I will let you know if succeeded :)
```

---
## \#10 Posted by: marcoluz Posted at: 2017-07-21T12:48:01.798Z Reads: 60

```
as far as i know they are just values that allow you to control the amount of power (acceleration) and brake power. they are different because they are in tune for my needs.
```

---
## \#11 Posted by: marcoluz Posted at: 2017-07-24T18:28:31.080Z Reads: 33

```
I cant find this chip locally. Where can I buy it from Europe or Globally????????
```

---
