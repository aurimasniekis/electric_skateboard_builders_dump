# Wiring BMS for charge only

### Replies: 9 Views: 954

## \#1 Posted by: Morxy49 Posted at: 2018-09-30T14:51:31.774Z Reads: 134

```
Hi,

I'm currently sitting here trying to wire up my BMS to my skateboard in a charge-only with discharge bypass. I've been scratching my head for the last hour trying to figure this out without success... 

The BMS I have is [this one](https://www.ebay.com/itm/44V-48V-50-4V-12S-60A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System/221644780045?item=221644780045&ppid=PPX000608). 

The first thing I'm wondering is if the balance wires should be connected to positive or negative on the batteries?? I'm really getting mixed messages here.

Secondly, can someone please draw a picture of how I'm supposed to wire everything up. I would appreciate this sooo much right now because my brain is overheating and I can't think straight anymore...

Thanks so much in advance!
```

---
## \#2 Posted by: danile Posted at: 2018-09-30T15:01:40.349Z Reads: 122

```
https://www.electric-skateboard.builders/t/wiring-up-the-supower-12s-bms/31314/4?u=danile
```

---
## \#3 Posted by: Morxy49 Posted at: 2018-09-30T15:29:46.514Z Reads: 116

```
I don't understand. This is the same image provided by the manufacturer, ie the charge and discharge wiring, which I don't want.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-30T16:32:03.795Z Reads: 115

```
You take the - from your charge port and connect it to the p- or ch- depends how it’s labled on the bms. From the b- you go to your battery-.
The charge port + goes to the battery +.
As min that’s how it’s shown in the thread @danile linked.
```

---
## \#5 Posted by: danile Posted at: 2018-10-01T01:52:23.949Z Reads: 100

```
Sorry for the late reply.

You connect the battery to B-, and charge it via P-
But, your VESC/ESC is connected directly to B-/B+ with thick wires for the discharge.

I did something similar not that long ago, but for 6s battery: https://dosimplecarbon.com/how-to-wire-6s-bms-to-your-2x3s-lipo-esk8/

The idea is the same, look at the parallel wiring of B- in the link above.

Hope it helps,
Dani
```

---
## \#6 Posted by: skslingo21 Posted at: 2018-10-01T02:32:48.793Z Reads: 92

```
P- to charger negative(mine was red), B- to battery negative. :point_right:
![20180930_222324|375x500](upload://6qFzkKTjibtJOBZhR2LcH2qoHSm.jpeg)
notice the bare connector on the back of each balance lead. These negatives were mummified in hotglue 
since neither are typically needed. (batteries left intact ;) Only the negative next to cell one is used. 
The two xt90's in this setup were labeled accordingly with the balance leads so nothing could go wardbacks.
```

---
## \#7 Posted by: Morxy49 Posted at: 2018-10-01T14:07:29.366Z Reads: 77

```
Okay so if i get this straight, the power could go through the BMS when discharging too, but since electricity always takes the "easiest" path it will rather bypass the BMS and go straight into the motor controller?
```

---
## \#8 Posted by: danile Posted at: 2018-10-01T15:04:24.149Z Reads: 70

```
Yes, that's the idea.

Dani
```

---
## \#9 Posted by: Morxy49 Posted at: 2018-10-01T22:13:21.574Z Reads: 60

```
I did it! Thanks a lot everyone!
```

---
