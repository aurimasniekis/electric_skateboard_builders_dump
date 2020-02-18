# VESC - Receiver connection questions

### Replies: 15 Views: 1779

## \#1 Posted by: Nicolai Posted at: 2016-07-24T16:44:10.644Z Reads: 229

```
Hey ESK8 friends,
My Enertion VESC finally arrived last week and I've since begun my first build! However I have a few questions about the VESC that I can't seem to find the answers to on other threads. My VESC came completely shrink-wrapped, which is fine, but it means that the PPC connection didn't come with any wires for the receiver that came with my GT2B controller. I'm wondering what the best way to link them would be. I have a soldering gun and I'm not afraid to use it if needed, but I'm curious to see what you guys would say to this issue. <img src="/uploads/db1493/original/2X/f/fd6fa60a324b1beee5a14551a4a7f1185a7b7e1f.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/2X/2/22bf86ed079e64ff88e67db606a35e59d92c9dad.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/2X/0/0a430984a63f4b94018d907f368cdacbcb5794f4.jpeg" width="666" height="500">
Another question about the VESC: it came without any connected motor connectors. The three wires that connect to the motor were just left with bare ends, but the bronze motor connectors came separately. I just soldered them on so that I could easily plug in my motor - is this wrong or will it work?<img src="/uploads/db1493/original/2X/c/c939505501c3ec2acd6f14123e5e32b036dbce5e.jpg" width="375" height="500">

Any help is appreciated! Thanks!
```

---
## \#2 Posted by: makevoid Posted at: 2016-07-24T16:56:58.424Z Reads: 217

```
Yes you need dupont or equivalent female/female cables (3 pins). Then you need some heatshrink tube or electrical tape (heatshrink is recommended though) to cover completely those female bullet connectors powering the motor.
```

---
## \#3 Posted by: joeadams101 Posted at: 2016-07-24T17:09:13.533Z Reads: 212

```
[quote="makevoid, post:2, topic:6558"]
dupont
[/quote]

Can you link the cable with the female connectors? The one he needs to connect the GT2B to the VESC? I need it to. Thanks in advance
```

---
## \#4 Posted by: Blasto Posted at: 2016-07-24T17:11:01.331Z Reads: 207

```
Go to your local hobby shop and get a servo cable like this one

https://solarbotics.com/product/15006/?gclid=Cj0KEQjwztG8BRCJgseTvZLctr8BEiQAA_kBDzqM9TMFAUweOrXOPsyOAaWbm-GcMUkbzvaZtcgxT4saAktz8P8HAQ
```

---
## \#5 Posted by: Nicolai Posted at: 2016-07-24T17:15:19.958Z Reads: 199

```
Thanks so much! So it sounds like my soldered-on motor connectors will work, I'll just shrink tube them completely. Really appreciate the help!
```

---
## \#6 Posted by: Blasto Posted at: 2016-07-24T17:24:26.120Z Reads: 197

```
Also add a tack of hot glue on the connector so it doesn't vibrate off
```

---
## \#7 Posted by: joeadams101 Posted at: 2016-07-24T19:31:33.728Z Reads: 182

```
Anyone know what type of screws will be the best for the motor since mine didn't come with them?
```

---
## \#8 Posted by: Nicolai Posted at: 2016-07-24T19:46:49.753Z Reads: 177

```
@joeadams101 Mine didn't either. I went to my local hardware store and went searching for screws in the metric machine screw section until I found screws that fit the threads of the motor perfectly. I think they were "M4 ⅞ metric screws"...
```

---
## \#9 Posted by: joeadams101 Posted at: 2016-07-25T04:58:11.544Z Reads: 164

```
got it! thanks a lot! now just waiting on space cell! i live in LA if you are close by for a group meeting. I have a friend who is waiting for just battery as well
```

---
## \#10 Posted by: t1m0007 Posted at: 2016-07-25T05:01:37.603Z Reads: 163

```
I'm game for this meetup as well. Awaiting VESC and spacecell
```

---
## \#11 Posted by: NICOMUTTER Posted at: 2017-04-11T08:10:58.577Z Reads: 102

```
[quote="makevoid, post:2, topic:6558"]
heatshrink
[/quote]
 Hello guys, 
So this cable is use to connect the VESC to the receiver of my GT2B
, that's right ? :)
<img src="/uploads/db1493/original/3X/7/8/783a89b241a5ed0aa80c658619b92a51bff3bcaa.jpg" width="375" height="281">
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-04-11T08:12:56.330Z Reads: 98

```
Yep. It´s called a servo cable
```

---
## \#13 Posted by: NICOMUTTER Posted at: 2017-04-11T08:23:03.187Z Reads: 98

```
Ok ty ! :)
[quote="TarzanHBK, post:12, topic:6558, full:true"]
Yep. It´s called a servo cable
[/quote]
```

---
## \#14 Posted by: NICOMUTTER Posted at: 2017-04-11T12:04:10.011Z Reads: 94

```
<img src="/uploads/db1493/original/3X/a/9/a93554f1877b56a0f5653dd053c47bf911e4c7d4.JPG" width="302" height="279">

Do you know if this cable fit ? Because he is cheaper :)))
here is the link : https://www.amazon.fr/C%C3%A2ble-dExtension-Trucks-RC-Lot-voiture/dp/B00LARAEZS/ref=sr_1_fkmr1_1?ie=UTF8&qid=1491912113&sr=8-1-fkmr1&keywords=150mm+Futaba-style+Servo+cable%2C+Double+Female
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-04-11T12:36:26.671Z Reads: 92

```
no, you need a male to male servo cable, this one is a male to female.
But you could buy these and solder the female part on the vesc.
```

---
