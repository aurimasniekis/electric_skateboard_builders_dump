# VESC possibly fried

### Replies: 16 Views: 847

## \#1 Posted by: erikkondo Posted at: 2017-12-14T01:34:20.653Z Reads: 91

```
I have two new VESCs from DIY. 
I set them both up via the BLDC tool. 
One was fully connected to the motor, battery, and transmitter. It was working fine when tested.
Next, I connected the 2nd VESC via the XT90 parallel connector. At that point, both VESCs stopped working.
The lights now no longer go on for both VESCs. They don't connect to the BLDC tool.

My battery is a 8s.

It check the wiring. It doesn't seem to be reverse polarity since one VESC was working.

Any thoughts on what I should do now? If I buy new ones, I don't want the same thing to happen.
Or maybe there is a simple repair. 
I would appreciate any advice.<img src="/uploads/db1493/original/3X/9/3/9368c896dfa324d3fd4a79273fb608d9ac64776e.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/4/8/48832015288fa6c4f521dadf6544b74d6ebfb1d6.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/0/900b85046836d06d0ec629665c88a616c4501084.JPG" width="640" height="480">
```

---
## \#2 Posted by: scepterr Posted at: 2017-12-14T01:36:03.689Z Reads: 80

```
You plugged in 2nd vesc while first was powered on?
Some pics would also be helpful, all the wiring, vesc, etc

Ahh seems you likely blew can transciever
If connected via can, you must power on at the same time
```

---
## \#3 Posted by: erikkondo Posted at: 2017-12-14T01:37:16.263Z Reads: 79

```
Yes. 1st was power on.
I just added pics.
```

---
## \#4 Posted by: erikkondo Posted at: 2017-12-14T01:38:07.808Z Reads: 81

```
Can it be repaired?
```

---
## \#5 Posted by: scepterr Posted at: 2017-12-14T01:38:27.378Z Reads: 83

```
Quite easily 

https://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142/111
```

---
## \#6 Posted by: erikkondo Posted at: 2017-12-14T01:39:02.675Z Reads: 82

```
Thanks for your help!!!
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-12-14T01:59:57.337Z Reads: 72

```
If want to be sure you can always follow these step. 

https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
## \#8 Posted by: erikkondo Posted at: 2017-12-14T02:23:49.698Z Reads: 57

```
Thanks. I just ordered a multimeter.
```

---
## \#9 Posted by: bimmer Posted at: 2017-12-14T02:27:26.720Z Reads: 56

```
If you cant fix them I'd take them off your hands for the price of 1 new one.
```

---
## \#10 Posted by: erikkondo Posted at: 2017-12-14T02:32:17.085Z Reads: 54

```
Good to know.
```

---
## \#11 Posted by: erikkondo Posted at: 2017-12-14T02:34:16.819Z Reads: 56

```
I have been searching for more information on repairing the U401.
Is there anything else that will get me more info?
```

---
## \#12 Posted by: bimmer Posted at: 2017-12-14T02:41:05.501Z Reads: 51

```
U need a smd reflow solder station and then replace this part.<img src="/uploads/db1493/original/3X/9/7/97790035b43b1a9c9ffc1937f17918c05cb2488a.jpg" width="243" height="500">
```

---
## \#13 Posted by: erikkondo Posted at: 2017-12-14T02:59:04.974Z Reads: 51

```
Thank you.
```

---
## \#14 Posted by: erikkondo Posted at: 2017-12-14T03:01:45.522Z Reads: 49

```
Get this part?
http://www.st.com/content/ccc/resource/technical/document/datasheet/82/ce/d2/e8/13/25/4f/b3/CD00001375.pdf/files/CD00001375.pdf/jcr:content/translations/en.CD00001375.pdf
```

---
## \#15 Posted by: erikkondo Posted at: 2017-12-14T03:13:12.159Z Reads: 45

```
It looks like I should be getting one of these.
https://www.google.com/search?rlz=1C1CHBD_enUS770US770&biw=1536&bih=710&tbm=shop&ei=tesxWriYHoXi_AaE0b6QDA&q=can+bus+transceiver&oq=can+bus+transceiver&gs_l=psy-ab.3...6256.12510.0.12846.38.27.1.0.0.0.417.2344.16j4j1j0j1.22.0....0...1c.1.64.psy-ab..19.7.990...0.0.nMsBMSv2FMs

Anyone know exactly which one?
```

---
## \#16 Posted by: scepterr Posted at: 2017-12-14T03:15:18.076Z Reads: 43

```
https://github.com/vedderb/bldc-hardware/blob/master/design/BLDC4.12_BOM.ods

https://github.com/vedderb/bldc-hardware
```

---
