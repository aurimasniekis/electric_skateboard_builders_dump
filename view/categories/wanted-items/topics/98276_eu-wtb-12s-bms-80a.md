# \[EU\] WTB 12s BMS 80a

### Replies: 11 Views: 98

## \#1 Posted by: zenobios Posted at: 2019-07-11T19:57:55.881Z Reads: 35

```
Hi,

looking for the BMS D596 (https://www.litechpower.com/product-detail/HCX-D596LI12S80A_08.html#). I want to connect 12S1p LiPos. 

Shipping should go to germany.

Thx
Andreas
```

---
## \#2 Posted by: Anubis Posted at: 2019-07-11T20:12:38.421Z Reads: 34

```
Fyi, while you can call it 12s1p, its often actually lipos taped together, often 6S are actually 12 lipo cells in 6S2P. 

Anyway, look on Ebay for charging ones and wire around the BMS for discharge, or https://eskating.eu/product-category/bestech-bmss/?v=79cba1185463
```

---
## \#3 Posted by: zenobios Posted at: 2019-07-11T20:29:18.072Z Reads: 27

```
I'll use two 6S1P zippy compact in series so I'm pretty sure that they are 12s1p.
```

---
## \#4 Posted by: Anubis Posted at: 2019-07-11T20:50:24.394Z Reads: 19

```
Right, but if they're 5000Mah, it could be 12 2500Mah lipo cells taped together.
```

---
## \#5 Posted by: Tinp123 Posted at: 2019-07-11T21:13:48.418Z Reads: 18

```
Hey! I have new bestech 12s d596 for sale. 60eur + shipping (probably under 10 eur)
```

---
## \#6 Posted by: zenobios Posted at: 2019-07-12T07:07:16.250Z Reads: 14

```
Great, which values did you choose for the adjustable ones ("over charge detection voltage", "over charge release voltage", "over discharge detection voltage" and "over discharge release voltage")?
```

---
## \#7 Posted by: Tinp123 Posted at: 2019-07-12T07:12:48.666Z Reads: 14

```
Here is data sheet for my bms:

![mail|230x500](upload://x6DClMGnXogbFY3wGFMrFdl9ygv.jpeg)
```

---
## \#8 Posted by: zenobios Posted at: 2019-07-12T08:00:38.246Z Reads: 13

```
Yeah ok. I personally see a problem in the "over discharge detection voltage" which is 2.8V. As I understood this is quite too low for LiPos and should be set to 3.0V.

On the other hand: I probably can use the over discharge detection in the VESC but I wonder how other people are doing this since I know that some are also using the D596 with LiPos.
```

---
## \#9 Posted by: Tinp123 Posted at: 2019-07-12T08:09:27.559Z Reads: 13

```
I see that some people consider even 3.6v on lipo empty, but I never saw bms with over discharge set at 3.6v. you can set up cut off voltage in vesc setting and everything will be okay. In my opinion, main function of bms is cell balancing function, and in this specific bms, e-switch.
```

---
## \#10 Posted by: zenobios Posted at: 2019-07-12T08:35:24.998Z Reads: 9

```
Additionally it also makes a difference *when* you measure the current voltage. If you measure during load then you probably should cut-off earlier (e.g. 3.6v). See also https://marinehowto.com/under-load-battery-voltage-vs-soc/ for rest vs. under-load voltage.

Back to the topic: Is the BMS new or did u use it already?
```

---
## \#11 Posted by: Tinp123 Posted at: 2019-07-12T09:26:49.850Z Reads: 8

```
well, if you meassure under load, because of voltage sag, temporary voltage will be lower than real voltage without load. for example, if you pull throttle, voltage will drop from 3.8v to 3.6v, but when you release it, voltage will stabilise back on 3.8v after few seconds. high discharge lipos should have minimal voltage sag. article you linked is about lead acid batteries, I have never heard that li ion or lipo battery will have higher voltage under load. when you brake hard, yes, but under load, never.

bms is new and packed, actually DHL should deliver it today.
```

---
