# Charging without a BMS

### Replies: 7 Views: 370

## \#1 Posted by: BenL Posted at: 2018-11-15T02:31:09.939Z Reads: 81

```
I bought the following 4A 12S charger:
https://www.aliexpress.com/item/50-4V-4A-Charger-50-4V-4A-Li-ion-Charger-for-44-4V-12S-Electric-Bike/32871550795.html?spm=a2g0s.9042311.0.0.1a734c4d7MmVYy

Since it is CC/CV, I should be able to charge without a BMS, right?
I expect it to limit the current to 4A. 

I'm not worried about balancing - I can manually balance the battery when need be.
```

---
## \#2 Posted by: PXSS Posted at: 2018-11-15T02:34:51.618Z Reads: 76

```
Yes, the only thing to be careful is the trickle charging. Li-ions should not be trickle charged.
Do they have a charge profile? Ask them for one. Good find for the price!

As long as you keep an eye on the balance you should be fine. I recommend getting a balance board anyways so you don't accidentally over charge a cell if too much time goes by between balancing cycles.
```

---
## \#3 Posted by: BenL Posted at: 2018-11-15T03:08:05.828Z Reads: 71

```
Thanks for the reply! I was unaware of the issue with trickle charging. 

For anyone else reading, here is some more information about the problem of trickle charging a li-ion battery.

From https://batteryuniversity.com/learn/article/charging_lithium_ion_batteries
"Li-ion cannot absorb overcharge. When fully charged, the charge current must be cut off. A continuous trickle charge would cause plating of metallic lithium and compromise safety. To minimize stress, keep the lithium-ion battery at the peak cut-off as short as possible."

From https://www.microchip.com/stellent/groups/designcenter_sg/documents/market_communication/en028061.pdf
"Stage 4: Charge Termination -- Unlike nickel-based batteries, it is not recommended to continue
to trickle charge Li-Ion batteries. Continuing to trickle charge can cause plating of metallic
lithium, a condition that makes the battery unstable. The result can be sudden, automatic,
and rapid disassembly. "

I couldn't find anything definitive about why the trickle charging was bad though other than the fact that the battery is already full charged. I suspect that this charger has a potentiometer to adjust the end voltage. I wonder if I set it to say 50V rather than 50.4V, whether trickle is no longer a concern?

@PSXX Oh, I sent a message to the supplier asking for the charge profile. If they get back to me, I'll attach it here.
```

---
## \#4 Posted by: PXSS Posted at: 2018-11-15T04:16:37.685Z Reads: 57

```
Trickle charging is bad because it leaves the battery at a high voltage for a prolonged period if time. 

I'm not sure they trickle charge at all as they do have a cutoff current of 5% charge current. Another thing to look for is at what voltage is charging re-enabled
```

---
## \#5 Posted by: Trdolan03 Posted at: 2018-11-15T06:38:49.139Z Reads: 51

```
No no no no. You must use a BMS for charging. Charging without one caused this. Cc/CV is a requirement for all chargers when charging liion. The CC/CV doesn’t keep the cells balanced. It just won’t over charge the pack a s a whole. Doesn’t protect you from anything. Absolutely DO NOT charge without a BMS. ![image|375x500](upload://fhT7HVLwJSBUqGxd5Wph8Mq8Dc2.jpeg)
```

---
## \#6 Posted by: PXSS Posted at: 2018-11-15T08:58:05.797Z Reads: 41

```
Sorry and no offense but no. 
The lack of a bms did not cause that fire. Your inexperience making batteries and using them appropriately did. The BMS is a very very very important safety feature but not by any means vital.

I do not condone or suggest anyone to build a pack without a BMS but with enough experience and care, it can be done as proven by @whitepony. It just means you have to be conservative in your discharge and charge levels as well as checking your battery every once in a while for balancing.
```

---
## \#7 Posted by: BenL Posted at: 2018-11-15T23:24:40.060Z Reads: 31

```
I currently charge without a BMS with this monstrosity. I trust myself checking the balance of the cells more than I trust a BMS to do a good job of it. 

![IMG_20181115_180942_resized_20181115_061257127|375x500](upload://dqxJlcAsiSxWYt3pgFaWQC06R7N.jpeg) 

It's a 12V power supply connected to a Drok boost converter. https://www.ebay.com/itm/DROK-Numerical-Control-Regulator-DC-8-60V-to-10-120V-15A-Boost-Converter-Cons-/282243271517#rwid
It's great because I can control the charge voltage (I almost never charge past 49.5V) and current. However, I wanted something more portable and less noisy. The Drok makes a surprisingly loud high pitch noise.
```

---
