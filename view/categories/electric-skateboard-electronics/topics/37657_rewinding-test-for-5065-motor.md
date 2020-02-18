# Rewinding test for 5065 motor

### Replies: 6 Views: 724

## \#1 Posted by: Quezacotl Posted at: 2017-11-07T20:56:10.692Z Reads: 125

```
Hello!

I got one broken motor. First the winding escaped little and made screeching noise while driving. I repaired that with a superglue. Not long until one magnet got loose, and made screeching noise while accelerating. Yet another problem, one of the mounting screwholes got rounded. At some point i bought another motor and i'm happy with it.
So i'm repairing this and though about what if i finally try a rewinding, that i have wanted for a long time.

There's no actual rewinding yet. Now i'm only asking for advices :)

Here's the patient:
<img src="/uploads/db1493/original/3X/3/f/3f76a370bb5f8a4aa4864d5bd0c677df115c7391.jpg" width="690" height="388">

I put it in a freezer overnight with penetrating oil(a tip from some other forum), and clamped on a vise, wiggled and hammered the stator out.
<img src="/uploads/db1493/original/3X/8/7/875b585372fd75cd9baabaab4ba98ffbc742b073.jpg" width="690" height="388">

There were about 75g of copper.
<img src="/uploads/db1493/original/3X/2/9/2949caba9787a6c49e646b0f9a685c6ef80e5e59.jpg" width="690" height="388">

The motor was supposed to be 270KV. And the facts; about 75g of 0,2x14 = 0,448mm2 stranded wire total.
Motor is 12 pole, 14 magnet. about 7-9 rounds per pole.

But then, i don't know what configuration i should be using. I find lots of conflicting info, and a lot of speculation.
When making wye, it is supposed to be around 1,7 times lower KV compared to delta. But then apparently almost all are winded as delta configuration(i think).

My goal is simply lower KV than it was, to be used on 10S and FOC.
I was thinking using something like 0,13x60 = 0,796mm2([link](https://www.aliexpress.com/item/0-13x60-strands-10m-pc-Litz-wire-stranded-enamelled-copper-wire-braided-multi-strand-wire/32796745628.html?spm=2114.search0104.3.209.JpFUcV&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10065_10151_10068_10344_10345_10342_10343_10340_10341_10541_10304_10307_5670020_10060_10302_10155_10154_10056_10055_10539_10537_10536_10059_10534_10533_100031_10103_10102_10142_10107_10171_10562_10084_10083_10561_5650020_5740017_10312_10313_10314_5660020_10550_10073_10551_10552_10553_10554_10557,searchweb201603_24,ppcSwitch_5&btsid=0338a971-3226-4865-9870-59ca330f7333&algo_expid=0f0024ff-6ea4-4120-8c39-af48db331b1e-32&algo_pvid=0f0024ff-6ea4-4120-8c39-af48db331b1e)) and dLRK evolution(delta) configuration.
Any advice?
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-07T21:59:49.471Z Reads: 113

```
Wye has less kv, but it also has a higher resistance, so it won't handle as much power without overheating. It also doesn't give as much back-emf signal, so for sensorless setups it's harder to track.

I'd recommend going with Delta and just changing the turns. 
If 8 turns gives you 270kv, then 11 or 12 turns should get you close to 190.

Keep in mind that if you change the magnets, and the new magnets are stronger or weaker, that will also affect the kv, stronger magnets make it lower.
```

---
## \#3 Posted by: Quezacotl Posted at: 2017-11-08T10:49:23.039Z Reads: 83

```
Okay. I thought turns versus KV was other way around.
Anyways. I'll make it then delta. And i might aswell buy both, thicker a thinner cable, and maybe try both and see the results, or just use the other to something else :smiley:
So another cable to test would be then this. 0,1x40(0,314mm2)
https://www.aliexpress.com/item/0-1x40-strands-20m-pc-Litz-wire-stranded-enamelled-copper-wire-braided-multi-strand-wire/1757475199.html?spm=a2g0s.13010208.99999999.263.Rn8AZA
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-11-08T15:34:16.490Z Reads: 70

```
I would recommend going with fewer strands of thick wire, rather than lots and lots of strands of thin wire.

The insulation on wires has thickness, and with a smaller wire, a larger fraction of the cross section is insulation rather than copper. Go on YouTube, there are several excellent videos on motor rewinds that show the whole process.
```

---
## \#5 Posted by: Quezacotl Posted at: 2017-11-08T19:48:48.855Z Reads: 52

```
Oh right! That was the claim i read that fewer(one) strand is better. I couldn't figure out why it is that, but now i see. That claim was about one strand, but yea, i'll get fewer-strand wires.

Good that there is chinese black friday on 11th, i'm stacking things on shopping carts before that date. So i haven't bought anything yet. :smile:
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-11-08T20:56:48.309Z Reads: 49

```
A single strand is best, but with motors this large, the wire ends up being thick enough to be very stubborn. A good compromise is 5 or so smaller wires that add up to the same mm² as a single large wire.

The best size is basically the largest that can be physically crammed into the space available and still get the desired turns. More copper = more better.
```

---
