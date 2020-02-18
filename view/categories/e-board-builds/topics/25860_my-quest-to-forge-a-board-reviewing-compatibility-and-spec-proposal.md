# My quest to forge a board-reviewing compatibility and spec proposal

### Replies: 10 Views: 747

## \#1 Posted by: samhelm Posted at: 2017-06-21T16:25:19.465Z Reads: 90

```
Hey. I'll be starting my first long board build soon. I was hoping before I started anyone could let me know of any potential compatibility or functionality errors with the parts I've chosen. Here's my spec:

Trucks- Caliber truck co. 9” (40$.£31.5): https://www.amazon.com/Caliber-Truck-Co-Skateboard-50-Degree/dp/B00J5J6KZ6/ref=sr_1_4?s=sporting-goods&ie=UTF8&qid=1497994489&sr=1-4&keywords=caliber+longboard+trucks

Wheels- Abec 11 90mm fly wheels (85$/£65): http://www.abec11.com/products/abec11/abec-11-76mm-83mm-90mm-97mm-flywheels-75a-78a

Bearings- bones reds bearings (22$/£18.5): https://www.amazon.com/gp/product/B000FDRQ1S/ref=as_li_tl?ie=UTF8&tag=howto0ad-20&camp=1789&creative=9325&linkCode=as2&creativeASIN=B000FDRQ1S&linkId=eaba1dbb8bdc74c3a79381e53f31aa4c

Motor mount- DIY Torqueboards bolt on motor mount (60$/£47.5): diy-electric-skateboard-kits-parts/single-bolt-on-motor-mount-only/

Motor- DIY 5055 190kv motor (70$/£55.5): diy-electric-skateboard-kits-parts/electric-skateboard-motor-5055-190kv/

Belt, motor pulley and wheel pulley-36T ABEC 11 drive wheel pulley (12mm), 13T motor pulley (12mm, 15 teeth) (47$/£37): diy-electric-skateboard-kits-parts/36t-abec-drive-pulley-belt-combo-kit/

Battery-Multistar 8000mAh 6S 10C Multi-Rotor Lipo Pack (76$/£60):
 https://hobbyking.com/en_us/multistar-high-capacity-6s-8000mah-multi-rotor-lipo-pack.html

ESC: Hobbywing QUICRUN WP-8BL150 150A Waterproof Brushless ESC (113.5$/£90):
 https://wheelspinmodels.co.uk/i/266815/?gclid=Cj0KEQjwyZjKBRDu--WG9ayT_ZEBEiQApZBFuHrzrV9xFyjd2_DBXcr01EkYwvGi4DMGWXA6SckRIBsaAlCB8P8HAQ

Controller: HobbyKing HK-GT2B 3CH 2.4GHz (25$/£18.50):
  https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html?___store=en_us

Enclosure-DIY's ESC enclosure (35$/£27.5): diy-electric-skateboard-kits-parts/esc-enclosure/

Board: custom (will be building it from scratch by sticking two 4mm and one 6mm pieces of beech plywood together with waterproof wood glue then covering with wood glaze and grip tape. The method is outlined in the following video: https://www.youtube.com/watch?v=4_ImE0sRnfM)

Any help is much appreciated!
```

---
## \#2 Posted by: smurf Posted at: 2017-06-21T17:22:58.980Z Reads: 63

```
That's a really thick battery probably wouldn't fit in the enclosure. Better to use 4 thin 3s battery's. Or 5 2s
```

---
## \#3 Posted by: rpn314 Posted at: 2017-06-23T11:25:52.522Z Reads: 44

```
I'm very partial to the VESC so if it were me, I'd swap the car ESC for that. Other than that, looks quite good. Maybe a 6355 motor instead of a 5055? If you're only going with a single motor setup, I'd do that or even a 6374
```

---
## \#4 Posted by: samhelm Posted at: 2017-06-23T15:34:10.722Z Reads: 37

```
hey smurf, thanks for the response. would a few of these be more appropriate?
https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html

if not would you be able to recommend me an alternative? many thanks.
```

---
## \#5 Posted by: mmaner Posted at: 2017-06-23T15:50:14.845Z Reads: 31

```
[quote="samhelm, post:4, topic:25860"]
would a few of these be more appropriate?
ZIPPY Flightmax 8000mAh 3S1P 30C Lipo Pack
[/quote]

I use x2 of these on my 6S beater board...
http://www.electric-skateboard.builders/t/mikeyz-beater-board-jet-spud-33-caliber-iis-blue-6s-8000mah-vesc-260-kv/22814

They are not super powerful but do pretty well on flats with minimal hills, hills require you get some speed up first.
```

---
## \#6 Posted by: samhelm Posted at: 2017-06-23T15:52:57.506Z Reads: 29

```
hey rpn, thanks for the advice. i think i'll go with your advice and upgrade to the 6374. as for the vesc again, I'll take your advice. I'm thinking of going for the Torque ESC VESC:
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
but can't find many reviews. do you think it would be worth going higher to something like Ollin board's 4.12 vesc or is it not worth it?

cheers again.
```

---
## \#7 Posted by: samhelm Posted at: 2017-06-23T15:55:19.416Z Reads: 24

```
thanks mmaner. i guess i'll go with a couple of these then.
```

---
## \#8 Posted by: mmaner Posted at: 2017-06-23T16:06:20.255Z Reads: 26

```
The only other suggestion I would make is X5 os the cheap 2s zippys in series for 10s total.  You will need to do some soldering and it's best to use a BMS. 

https://hobbyking.com/en_us/zippy-5000mah-2s1p-30c-hardcase-pack.html
```

---
## \#9 Posted by: rpn314 Posted at: 2017-06-23T23:11:12.740Z Reads: 25

```
I've haven't heard of too many issues with those. Ollin makes a very solid board and frankly you can't get much better right now. Axle (@zmoney on here) may be another one to consider. If you're at all considering FOC, I'd say go Ollin.
```

---
## \#10 Posted by: sl33py Posted at: 2017-06-23T23:18:41.102Z Reads: 25

```
Agree with @rpn314 on @zmoney's Axle VESC option - if he has them in stock and ready to go.  They have the upgraded BOM similar to @Chaka's older non-direct-fet version.  Improved over most 4.12 VESC including DIYes (which is also good).

Best but $$ - Chaka/Ollin direct FET
FOCBOX - VESC-X (direct FET from Enertion)
Axle 4.12 VESC w/ upgraded BOM
DIYes
...
...
...
...
Maytech VESC (no thanks)

my .02 - HTH and GL!
```

---
