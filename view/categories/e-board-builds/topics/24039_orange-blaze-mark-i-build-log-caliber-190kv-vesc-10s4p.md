# Orange Blaze Mark I Build Log / Caliber / 190kv / VESC / 10s4p

### Replies: 9 Views: 909

## \#1 Posted by: markyoe Posted at: 2017-05-28T03:43:52.454Z Reads: 161

```
First of all, thanks to all the community members who have been answering my questions about my build!

**Here the setup:** 

Repainted [Goldcoast longboard deck](http://www.ebay.com/itm/GOLDCOAST-PINTAIL-LONGBOARD-DECK-44-THE-STANDARD-ORANGE-/152512837754?hash=item238279387a:g:WEYAAOSwRUhY81mV) (I think I paid $40-60 when I bought it last year...not sure why they're $200 now)
[190kv Motor](diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/)
[VESC](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)
[10s4p 18650 Li-ion battery pack](https://www.imrbatteries.com/lg-he2-18650-2500mah-20a-flat-top-battery/) 
[60A BMS](http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html )
[Battery capacity monitor](https://www.amazon.com/DROK-Black-light-Capacity-Automotive-Indicator/dp/B01LQ7MT4K/ref=sr_1_10?ie=UTF8&qid=1494256336&sr=8-10&keywords=lcd+voltage+display )
[17T motor pulley](http://shop.sdp-si.com/catalog/product/?id=A_6A25M017DF1508 )
[36T wheel pulley](http://www.ebay.com/itm/272641770207?ul_noapp=true)
[Key anti-spark plug](http://www.ebay.com/itm/Amass-XT90-S-Anti-Spark-Female-Battery-Connector-Plug-for-LiPo-or-NiMH-Batteries-/232117244276?hash=item360b441174:g:N~QAAOSwGJlZGRBz) to power on
[Steeze remote](https://longhairedboy.com/collections/frontpage/products/2-4ghz-steeze-remote-for-electric-skateboards) from @longhairedboy 

**Hopefully will feature:** 

- USB charging capability for my phone. I'll run 5V from the RX port of the VESC.
- ABS vacuum formed enclosures. 
- Regen braking


Alright here are the pictures that you came to see.

I began by soldering the battery pack. 

<img src="/uploads/db1493/original/3X/0/8/0813940f391a18d7722962616919e7ac3e75b96e.jpg" width="375" height="500">

Added the BMS

<img src="/uploads/db1493/original/3X/c/6/c62453ad2f3544416b6b8444e2f76f3b52177d4f.jpg" width="666" height="500">

Tested charging and I finally put heat shrink on the battery instead of gorilla tape. :slight_smile: 

<img src="/uploads/db1493/original/3X/8/2/829b1e499a0bc09ba0e519fa5111e34b9559b1e7.jpg" width="375" height="500">

Mold to vacuum form

<img src="/uploads/db1493/original/3X/8/8/88f4e5c2a6807f0f593307f94f7930883525cf4a.jpg" width="375" height="500">

Vacuum forming table I just built and a terrible first mold I made

<img src="/uploads/db1493/original/3X/6/7/67a7504c6fe0b1fced1cdb327666c7c23d635fa2.jpg" width="375" height="500">

YES, heating the ABS sheet on the BBQ does work!!!

<img src="/uploads/db1493/original/3X/d/4/d47b3c02a19c2a33326e766b8d90fbee79231ce1.jpg" width="375" height="500">

Vacuum formed cases before touchup shaping with a heat gun and trimming the excess.

<img src="/uploads/db1493/original/3X/d/3/d3b25124c44ec0bfcff1464ffb86ce744df37d9b.jpg" width="375" height="500">

Drive train with 3D printed belt cover. Great design by @mmaner ! 

<img src="/uploads/db1493/original/3X/1/c/1cc021aa34a47282d5e1f7fdc586a4b63ab9a71d.jpg" width="375" height="500">

More pictures and updates to follow!
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-05-28T06:24:11.129Z Reads: 143

```
Sick build :)
```

---
## \#4 Posted by: TranxFu Posted at: 2017-05-30T11:37:59.481Z Reads: 72

```
Measure the voltage coming from you charger to make sure its not the charger but sth. with the board/battery
```

---
## \#5 Posted by: markyoe Posted at: 2017-07-25T20:22:36.055Z Reads: 52

```
Here are some pics of the finished build! I reached 29mph with a 17/36 setup but switched to a 13/36 setup for my torque(top speed 25mph). I have a 20 mile range. Feel free to ask any questions.

<img src="/uploads/db1493/original/3X/b/1/b122a6356bea8697f9ae0a2efb0e28edcde8a343.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/8/d8d23e43788475aa388bc410223cba212453917c.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/c/b/cbca0220f3ab268477152aca2853e4adf678f480.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/6/a/6a9d7608fe5542b8b3a20ff57f59c6908c0519eb.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/0/0040eb336d25dfc0493a0a57302e7a62fc913134.jpg" width="666" height="500">
```

---
## \#6 Posted by: gliz5714 Posted at: 2017-07-25T20:47:20.886Z Reads: 44

```
[quote="markyoe, post:5, topic:24039"]
I have a 20 mile range.
[/quote]

So I haven't even built my first board yet (still in assembly) but interested in that battery pack... You are able to get 20 miles out of that??? 

If you cut the number of batteries in half (make it a 10s2p) would that just make it a 10 mile pack?
```

---
## \#7 Posted by: markyoe Posted at: 2017-07-25T20:51:43.310Z Reads: 41

```
You would most likely get way less than 10 miles with a 10s2p because the current will drop more quickly than a 4p(somebody correct me if I'm wrong). If you went with 5s4p, that'd be a different story, but that would be really slow. I'm fairly light (135) and the terrain I ride is pretty flat, so that helps my range.
```

---
## \#8 Posted by: gliz5714 Posted at: 2017-07-25T21:00:00.958Z Reads: 37

```
Ahh I gotcha.  I am not about to build my own pack, but I may in the future and that just seemed like a very expensive battery!  (based on your link, $200?)
```

---
## \#9 Posted by: markyoe Posted at: 2017-07-25T21:05:57.859Z Reads: 36

```
$150 for a 10s4p right now because of the bulk discount. They're $3.75 a piece when you buy 30.  I just bought 32 a couple weeks ago and they were on sale for $3.50 a piece. Just look and wait for the deals.
```

---
## \#10 Posted by: gliz5714 Posted at: 2017-07-25T21:13:07.514Z Reads: 31

```
Ahh bulk discount.  So basically watch for sales to drop that even further, makes total sense!

I can see how this hobby is time and money consuming...
```

---
