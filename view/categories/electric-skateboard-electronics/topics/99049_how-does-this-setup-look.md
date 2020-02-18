# How does this setup look?

### Replies: 9 Views: 237

## \#1 Posted by: Ultimiant Posted at: 2019-07-24T17:02:40.147Z Reads: 89

```
Hey y'all,

![esk8_setup|690x395](upload://lGooJIBmZ3ByyXPrLg04zBm1V1j.jpeg) 

If you see any issues please let me know, I have most of the parts aside from the battery and am starting to solder stuff together. Figured I would check first to make sure I don't mess anything up too badly lol. (I should add that the battery is going to have the BMS built in, so no need to worry about that)

This is the **[solder](https://www.amazon.ca/Austor-1-0mm-Lead-Solder-Rosin/dp/B071R3XVPN/ref=sr_1_1?keywords=AUSTOR+Lead+Free+Solder+Wire+with+Rosin+Core+1.0mm&qid=1563987327&s=hi&sr=1-1)** I am using:


This is the **[12 gauge wire](https://www.amazon.ca/BNTECHGO-Gauge-Silicone-Wire-black/dp/B00TG1TSUC/ref=sr_1_2?keywords=BNTECHGO+12+Gauge+Silicone+Wire+Ultra+Flexible&qid=1563987382&s=electronics&sr=8-2)** I am using:


An this is the **[tinned flat copper braid](https://www.amazon.ca/Tinned-Copper-Bright-Diameter-Length/dp/B003HGHQYC/ref=sr_1_fkmr0_1?keywords=Flat+Tinned+Copper+Braid%2C+Bright%2C+1%2F4%22+Width%2C+25%27+Length+%28Pack+of+1%29&qid=1563987429&s=hi&sr=8-1-fkmr0)** I am using to connect the battery along the deck:


And I am planning on insulating the copper wire with this **[tape](https://www.amazon.ca/DAOKI-Temperature-Resistant-Polyimide-Resisting/dp/B01CS068M8/ref=sr_1_1?keywords=DAOKI+5+Size+5mm+10mm+20mm+30mm+50mm+30m%2F100ft+BGA+High+Temperature+Film+Heat+Resistant+Polyimide+Kapton+Tape+Gold+Resisting+Sticky&qid=1563987481&s=office&sr=1-1)**.


Let me know if im missing anything or if there is anything I should beware of, im excited to get this build on the road!
```

---
## \#2 Posted by: Lumaci Posted at: 2019-07-24T19:29:26.064Z Reads: 77

```
The remote also has two wires you need to add to the vesc positive and negative for battery percentage reading.

Looks fine otherwise.
```

---
## \#3 Posted by: Lumaci Posted at: 2019-07-24T19:30:10.602Z Reads: 76

```
Maybe add a 60/80A fuse on the positive battery end just to make sure it cant go wrong there.
```

---
## \#4 Posted by: Ultimiant Posted at: 2019-07-24T20:24:36.882Z Reads: 62

```
Would a fuse like **[this](https://www.amazon.com/PACK-ANL-FUSES-GOLD-PLATED/dp/B003HYD52Q)** work? And what do you mean by "wrong" lol, im guessing to prevent excessive current from flowing through, in which case should I aim for a 90A fuse in case I decide to use all terrain tires and want to pull more power?
```

---
## \#5 Posted by: rusins Posted at: 2019-07-24T20:49:29.423Z Reads: 50

```
What you need is either an anti-spark switch (I know of none on the market at the moment that actually lasts) or a loop-key to turn your board on or off. (Or you can live without one if your battery's BMS has an e-switch, those seem to work quite well.)

WIthout an anti-spark current spikes could kill your fuse, so most people don't use a fuse between their battery and ESC. Fuse on the chargeport, however, is a good idea.
```

---
## \#6 Posted by: Lumaci Posted at: 2019-07-25T08:46:31.299Z Reads: 37

```
The VESC has an antispark switch built in.
```

---
## \#7 Posted by: Lumaci Posted at: 2019-07-25T08:47:11.312Z Reads: 38

```
Id just go for those car replaceable fuse boxes and use that, and go with a fuse that matches the max output of your batterypack.
```

---
## \#8 Posted by: rusins Posted at: 2019-07-25T08:58:57.937Z Reads: 39

```
Does it? I don't see it mentioned anywhere on the product page https://flipsky.net/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink
```

---
## \#9 Posted by: Ultimiant Posted at: 2019-07-25T17:18:05.472Z Reads: 20

```
Its **[this one](https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-plus-based-on-vesc6)** and mine has the pro switch which is anti-spark.
```

---
