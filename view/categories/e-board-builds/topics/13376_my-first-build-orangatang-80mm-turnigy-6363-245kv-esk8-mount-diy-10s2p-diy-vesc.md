# My first build &#124; Orangatang 80mm &#124; Turnigy 6363 245kv &#124; esk8 mount &#124; DIY 10S2P &#124; DIY VESC

### Replies: 12 Views: 1501

## \#1 Posted by: Maxx Posted at: 2016-11-20T18:42:29.280Z Reads: 177

```
Hello 

this is my first build so if you got any suggestions or ideas please comment...

Part list:

* [Hammond Longboard](https://www.amazon.de/gp/product/B00JR6PQ2A/ref=oh_aui_detailpage_o08_s00?ie=UTF8&psc=1)
*  [80mm Orangatang Kegel](http://www.ebay.com/itm/331956837087?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)
* DIY VESC (still busy soldering SMD shit ;) )
* AntiSparkSwitch 1.3
* AWG 10 cables
* 6300mAh LiPo pouch cells soldered together in 10S2P configuration
* [10S 60A BMS](https://www.aliexpress.com/item/10S-60A-version-S-lipo-lithium-Polymer-BMS-PCM-PCB-battery-protection-board-for-10-Packs/32730392818.html?spm=2114.13010608.0.0.tvTJxB)
* [Turnigy SK3 6364 245kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html)
* [esk8 motor mount](http://www.ebay.com/itm/122199145952?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)
* [14T 15mm motor pulley](http://www.ebay.com/itm/122166834609?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)
* [36T wheel pulley 3D printed](http://www.thingiverse.com/thing:1677410)
* [15mm 255 belt](http://www.hug-technik.com/shop/product_info.php?info=p5540_zahnriemen-htd-5m-laenge--255---15mm-breit----255-5m-15mm.html)

Still need to figure out a case for all the stuff, especially the cells.
```

---
## \#2 Posted by: ThieryB Posted at: 2016-11-21T15:35:10.086Z Reads: 139

```
Build your case! I like what you have going on so far, it's cool! but what are you going to use for a remote?
```

---
## \#3 Posted by: Maxx Posted at: 2016-11-21T15:41:55.993Z Reads: 137

```
I was thinking about a carbon fiber custom case but first I want to get everything working ;)
Oh forgot about including that: [a RF nunchuk but not the Kama because it was sold out everywhere](https://www.amazon.de/gp/product/B002BPNY6O/ref=oh_aui_detailpage_o08_s00?ie=UTF8&psc=1)
```

---
## \#4 Posted by: Maxx Posted at: 2016-11-21T15:49:20.750Z Reads: 122

```
And what kind of charger should I use ? The BMS does the balancing according to the aliexpress listing so what charger is the cheapest? :D
```

---
## \#5 Posted by: jujet Posted at: 2016-11-21T16:05:56.977Z Reads: 121

```
We're trying to do a group buy for this laptop style charger for 10s 

http://www.electric-skateboard.builders/t/cheap-chargers-with-customizeable-end-of-charge-voltage/6902/104

Have a look and if you want to join, reply there
```

---
## \#6 Posted by: Namasaki Posted at: 2016-11-21T16:11:32.210Z Reads: 108

```
245kv x 42v = 10290 rpm
10290 x 7= 72030 erpm 
The Vesc has an erpm limit of 60k
This motor/voltage combination could cause the Vesc's drv chip to fail.
```

---
## \#7 Posted by: Maxx Posted at: 2016-11-21T16:15:20.812Z Reads: 109

```
[quote="Namasaki, post:6, topic:13376, full:true"]
245kv x 42v = 10290 rpm
10290 x 7= 72030 erpm 
The Vesc has an erpm limit of 60k
This motor/voltage combination could cause the Vesc's drv chip to fail.
[/quote]


o.O anyway around that?
I´m pretty sure I saw a 245kv / 10S setup on here before
```

---
## \#8 Posted by: Namasaki Posted at: 2016-11-21T16:26:46.425Z Reads: 102

```
You'll have to limit the erpm in Vesc settings but there's a trick way to do it so that you don't get sudden shut down while accelerating. 
I don't know how to do it but someone on this forum has done it.
```

---
## \#9 Posted by: Maxx Posted at: 2016-11-21T16:36:28.581Z Reads: 95

```
So the first upgrade would be a 190kv motor? :D
```

---
## \#10 Posted by: SirDiff Posted at: 2016-11-21T17:00:48.387Z Reads: 97

```
Yeah go for a 190kv with a 10s on vesc. People have done it with a 245kv, just not paired with a vesc
```

---
## \#11 Posted by: Namasaki Posted at: 2016-11-21T18:12:59.520Z Reads: 90

```
190kv + 10s + Vesc = performance and dependability
```

---
## \#12 Posted by: Maxx Posted at: 2016-11-21T18:35:36.036Z Reads: 91

```
So this guy is using the same motor with 10S and apparently there seems to be not problem...
http://www.electric-skateboard.builders/t/1st-eskate-build-drop-through-6364-outboard/2986
```

---
