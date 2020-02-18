# Dead BMS - How do I prevent it?

### Replies: 11 Views: 830

## \#1 Posted by: KTMinni Posted at: 2017-05-14T20:13:29.111Z Reads: 109

```
So, basically I rode my board about a total of 5 miles and the battery died so I came home charged it and the VESC was still working.  I unplugged it to charge the battery and when I plugged it back in, no lights no nothing.  

Edit: and how exactly do I know it's the VESC thats dead? My battery is also not charging.  I don't know what's going on at this point
**This is now a conversation about avoiding a broken bms**
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-05-14T22:38:12.546Z Reads: 91

```
Hummm, sound more like a battery/BMS problem... what is your battery setup, you might have trigger the low voltage cutoff protection .
```

---
## \#3 Posted by: KTMinni Posted at: 2017-05-15T01:16:09.287Z Reads: 83

```
Jeez I actually figured that out moments after I posted this, but I had to leave for work.  I'm running a 10S2P of LG HE2 with a 10S BMS, which I'm pretty sure busted.  It won't charge, it keeps dropping voltage, and no current is actually going through the BMS(I connected an XT90 with 2 loose leads and it didn't spark). When I get home from work I plan on bypassing the discharge of the BMS to make sure the battery is ok. @JohnnyMeduse
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-05-15T01:55:38.111Z Reads: 79

```
Yes you could try that first

but this kind of behaviour :

[quote="KTMinni, post:3, topic:23056"]
it keeps dropping voltage
[/quote]
 
remind me of a broken pack, maybe something is disconnect along the pack
```

---
## \#5 Posted by: KTMinni Posted at: 2017-05-15T02:43:04.050Z Reads: 70

```
Mind you, only the voltage off the BMS is dropping not off the battery
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-05-15T02:50:32.952Z Reads: 67

```
Ok then it might be the bms... but it kind of a weird behaviour
```

---
## \#7 Posted by: KTMinni Posted at: 2017-05-15T03:16:25.488Z Reads: 62

```
Everything works fine without the BMS so definitely that.  But I don't know how it happened /how to prevent it from happening again.  I'm assuming the charger somehow friend the fuse or it got confused with discharging and recharging and just died
```

---
## \#8 Posted by: Tobi Posted at: 2017-05-15T04:05:04.258Z Reads: 61

```
How much ampere your bms could handle ?
```

---
## \#9 Posted by: KTMinni Posted at: 2017-05-15T04:05:27.981Z Reads: 65

```
10 charge 50 discharge @Tobi
```

---
## \#10 Posted by: Namasaki Posted at: 2017-05-15T18:09:44.930Z Reads: 38

```
What brand of bms is it
```

---
## \#11 Posted by: KTMinni Posted at: 2017-05-15T19:25:30.846Z Reads: 31

```
It's off brand or no obvious branding on it. http://m.ebay.com/itm/37V-42V-10S-50A-Lithium-ion-Li-ion-LiPo-NMC-Battery-BMS-PCB-System-Ebike-36V-/122355291406?txnId=1791132556002
```

---
