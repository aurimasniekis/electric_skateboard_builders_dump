# VESC ERPM limit

### Replies: 22 Views: 3535

## \#1 Posted by: lennarn Posted at: 2018-07-12T22:22:47.222Z Reads: 422

```
Apparently at some point the VESC had an ERPM limit of 60,000.
https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125

Calculating ERPM for different motors/voltages I am considering:

    V:
    8s 	    29,6v
    10s 	37v
    12s 	44,4v
    14s 	51,8v

    RPM: (kv*v)
        	14s	    12s  	10s	    8s	
    130kv	6734	5772	4810	3848
    150kv	7770	6660	5550	4440
    170kv	8806	7548	6290	5032
    200kv	10360	8880	7400	5920
    245kv	12691	10878	9065	7252

APS is my first choice for motors.
All APS 63mm motors have 12 poles.

    ERPM: (RPM*poles)
        	14s	    12s	    10s	    8s
    130kv	80808	69264	57720	46176
    150kv	93240	79920	66600	53280
    170kv	105672	90576	75480	60384
    200kv	124320	106560	88800	71040
    245kv	152292	130536	108780	87024

Is this still the case? Can I only use the 130kv motor at 10s and below (and 150kv at 8s, etc)? Or is the VESC more capable now? I'm using the Torque VESC with 4.12 hw/3.34 fw.
How do I figure the safe kv for 12s with these motors? The formula given in the above link gives me an ideal kv of 115 which seems pretty low.
```

---
## \#2 Posted by: linsus Posted at: 2018-07-12T22:25:01.499Z Reads: 380

```
Depends which vesc you have
```

---
## \#3 Posted by: lennarn Posted at: 2018-07-13T13:07:34.318Z Reads: 352

```
I’m using the Torque VESC with 4.12 hw/3.34 fw.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2018-07-13T13:38:28.665Z Reads: 349

```
> ERPM: (RPM*poles)


The formula is almost right. It´s 
rpm x pole pairs - so usually 7 pole pairs.

A safe opinion on kV and voltages:
10s - 190 kV
12s - 170 kV
```

---
## \#5 Posted by: lennarn Posted at: 2018-07-13T13:43:54.808Z Reads: 337

```
That sounds better! I guess that means I can halve all my erpm numbers then? Should make for a lot more viable motors!
That should mean I can use the 200kv motor I wanted at 12s and only hit a max of 53,280 erpm, so it won't fry my vesc with its 60k limit! 🤔😀
```

---
## \#6 Posted by: E1Allen Posted at: 2018-07-13T14:15:10.643Z Reads: 317

```
Plus within the vesc you can set erpm limits so even with a really high kv motor you wouldn't exceed
```

---
## \#7 Posted by: lennarn Posted at: 2018-07-13T16:14:56.109Z Reads: 301

```
In that case the motor rpm would be bottlenecked by the erpm limit though, wouldn't it?
```

---
## \#8 Posted by: E1Allen Posted at: 2018-07-13T16:16:32.343Z Reads: 297

```
Of course.  But if you limited it to 60k erpm is it really a limit of it prevents your vesc from blowing a drv chip?
```

---
## \#9 Posted by: Sebike Posted at: 2018-07-13T16:24:00.777Z Reads: 294

```
and you should use v for a full battery and not the nominal voltage
```

---
## \#10 Posted by: lennarn Posted at: 2018-07-13T18:18:30.035Z Reads: 271

```
12s 18650: 50.4v
200kv = 10,080rpm
6 pole pairs, erpm = 60,480
Looks like I can just about make it, just throttling max rpm when the battery is full then. Keeping the 60k vesc limit should be enough for this to work, right?
```

---
## \#11 Posted by: E1Allen Posted at: 2018-07-13T20:42:51.776Z Reads: 249

```
Yes. It's fine. That 200kv motor is probably less than 200kv
```

---
## \#12 Posted by: lennarn Posted at: 2018-07-14T08:11:07.971Z Reads: 235

```
What makes you say that? It's that a common occurrence?
```

---
## \#13 Posted by: E1Allen Posted at: 2018-07-14T08:17:23.215Z Reads: 226

```
Yes it is.
```

---
## \#14 Posted by: Sebike Posted at: 2018-07-14T10:07:36.717Z Reads: 219

```
one of my 190 kv motors is actually 200. the other 190 kv is 180.
```

---
## \#15 Posted by: iamgeekusa Posted at: 2019-04-25T19:55:53.721Z Reads: 136

```
Can anyone explain what happens while riding if you hit this limit?   I recently had my diy build brake unexpectedly and throw me off and someone said this was the cause.  would hitting the limit cause motors to brake?
```

---
## \#16 Posted by: lennarn Posted at: 2019-04-26T09:41:21.812Z Reads: 130

```
If I understand it correctly, it bricks your vesc.
```

---
## \#17 Posted by: Andy87 Posted at: 2019-04-26T10:04:04.292Z Reads: 127

```
depends... which motors, which vescs you have and which voltage you drive on?

also, did you set the erpm limit to 60 000 while setting up your vesc or is the value on default?

aaalso, did you use bldc tool or vesc tool to set up your vesc up?

the bldc tool has the "limit max erpm with negative torque" field. if it´s activated than it might be the cause.

if you use the vesc tool than it should just lower your torque down the closer you come to the erpm limit you set.

if you used vesc tool but a combination of hw4.12 vesc plus high kV motors and 12s without to change the erpm limit while set up your vesc than your vesc should now be fried.
```

---
## \#18 Posted by: Unhealthy_Apple Posted at: 2019-05-26T08:47:54.988Z Reads: 103

```
I have had what I think is the same problem then @iamgeekusa. It would be extremely helpfully if I know what happened so I can fix it as I broke my collar bone due to the incident. :frowning: 
I have a 190kv Motor from Tourque boards AKA diyelectricskateboard I also have there VESC. I set the erpm in VESC tool on FOC I set mine to 60,000 ermp. there was no button for Negative touque. Powering all this is 2x 5s in series (36V)

Fw: 3.53
Hw:410

Any help is Muchly appreciated
```

---
## \#19 Posted by: Andy87 Posted at: 2019-05-26T08:53:48.096Z Reads: 95

```
Hope you get well soon!

What exactly happened? The board cut out or was braking or just lost acceleration? 
Your vesc still working or did the drv pop?

Do you use a bms as discharge? Which remote you use? There multiple reasons why a cut out can happen, doesn’t need to come from the vesc, that’s why I ask.
```

---
## \#20 Posted by: Unhealthy_Apple Posted at: 2019-05-26T09:08:02.835Z Reads: 93

```
Thanks, man.

I was throttling up and was getting pretty fast then the board just stopped and I got chucked off. my VESC is still working. I didn't have a BMS at the time but I have installed one now.
This is my remote:
https://www.aliexpress.com/item/32861920031.html?spm=a2g0s.9042311.0.0.7f3a4c4dEX7b5i

Note:
I have an inkling that it is the erpm or something with my electronics but a few days after my accident I went back to the Crash site and there were some rocks. I do have 100mm all terrain wheels. Just thinking it could be something else.
```

---
## \#21 Posted by: Andy87 Posted at: 2019-05-26T09:45:09.068Z Reads: 87

```
I don’t have experience with this remote, but I remember the older version had connection issues. You can use a calculator to get your erpm max. Even with 12s and 190kV you shouldn’t hit the erpm limit under load. Did the cut out happen at top speed?

https://calc./#/0
```

---
## \#22 Posted by: Unhealthy_Apple Posted at: 2019-05-26T10:25:22.016Z Reads: 81

```
The calculator says my max erpm is 49000.
I'm not 100% but I'm pretty sure it cut at a relatively high speed.
With the remote issue would it just disconnect from the board and then just coast or would it apply full brakes to the board?
```

---
