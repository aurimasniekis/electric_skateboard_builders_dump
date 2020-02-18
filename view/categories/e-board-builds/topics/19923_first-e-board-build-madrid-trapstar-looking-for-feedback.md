# First E-Board build &#124; Madrid Trapstar &#124; looking for feedback

### Replies: 15 Views: 1286

## \#1 Posted by: TTOO Posted at: 2017-03-29T14:43:47.837Z Reads: 139

```
So basically im trying to build my first electric longboard and im having trouble understanding everything. On top of this i live in france so part of the research i do leads me parts that is only available (at a reasonable price) in the us.
So what i have for the moment is:
Deck: Madrid Trapstar
Trucks: Caliber 180mm (came with the board)
Wheels: 80a 76mm (also came with the board) (thinking of changing to bigger wheels but i dont know which wheels to choose and costs money)
And this is what im currently looking at for the rest (tell me whats wrong with this if you can it would be very helpful)(also im trying to stay on a budget so i dont know if its possible to get a good board for 300-450e in addition to the parts i already have):
Motor: Turnigy Aerodrive SK3 - 6374-149kv Brushless Outrunner Motor (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html) ( I looked around and im wondering if i should maybe get a higher kv motor)
VESC/ESC: ? i dont know how to choose one
Batteries: 4x ZIPPY Flightmax 5000mAh 3S1P 20C (https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html) ( i did a bit of research but i still dont really understand how to choose batteries so i got these from another build and i am not sure if they fit my needs)
Charger: ? not sure how to choose this one either
Remote: Arduino nunchuk controller
Misc: 
+Battery capacity tester: (http://www.ebay.com/itm/172143986261?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)

Finally i dont know how im going to go about mounting the motor (on my budget, should i get a motor mount ?) and the electronics (3d printing?)
```

---
## \#2 Posted by: mmaner Posted at: 2017-03-30T00:16:12.674Z Reads: 98

```
Those wheels are going to be difficult.  The minimum, typically, is 83mm.  There are people who have made them work but you will loose a lot of speed and they will hard to fit with a pulley.  Look for 83mm or 90mm flywheel clones on eBay or pretty much anywhere online for skate parts. 

For a single motor build 149kv is great torque but not much speed. I'd go with a 190kv or 245kv preferably at 6374.

Batteries are a touchy subject.  I prefer lipos but many prefer li-ion.  I would look at a 10s configuration with x2 5s lipos in series considering your budget.

Don't forget about motor mount, wheel and motor pulley, enclosure, switch or loop key, enclosure and wire and bits.   Once you decide on the hardware it will be easy to figure out the bits you need.

Check out  (@torqueboards).  He has some pretty sweet (free) shipping options for orders over $300 (I think), includes international too.
```

---
## \#3 Posted by: saul Posted at: 2017-03-30T00:37:48.875Z Reads: 91

```
[quote="TTOO, post:1, topic:19923"]
Finally i dont know how im going to go about mounting the motor (on my budget, should i get a motor mount ?) and the electronics (3d printing?)
[/quote]

I printed my first enclosure, it takes forever and uses almost a whole roll. they also break.

what your budget? range? speed? you need _at least_ $500 + deck, if you are near paris you should talk to @unik
he's got nice mounts and enclosures!
```

---
## \#4 Posted by: TTOO Posted at: 2017-04-05T12:42:46.757Z Reads: 65

```
**Wheels**
I looked around for flywheel clones but couldn really find anything(except on ebay with like 40e in shipping :frowning: )
so i looked for builds that people in france had previously done and found that the orangatang kegel wheels came up often (along with the flywheels that cost 90e withouth shipping) the pb is that they are also quite expensive 80e with shipping, is this normal for wheels? If not im having a hard time finding flywheel clones in france :confused:. 
 

----------

**Motor**
I quickly found these two motors:
[Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner Motor](https://hobbyking.com/fr_fr/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html)
[Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner Motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?___store=en_us)
The thing is i would use this to get to school everyday but i got a steep hill to go up so i think the 192 kv would be better (then again i dont really know if its necessary)


----------
**Batteries**
I found these batteries which looked interesting but im not sure what peak discharge is to a longboard build ( this is the only difference that justifiies the price difference:
[Turnigy 5000mAh 5S 20C Lipo Pack](https://hobbyking.com/en_us/turnigy-5000mah-5s-20c-lipo-pack.html)
[Turnigy 5000mAh 5S 25C Lipo Pack](https://hobbyking.com/en_us/turnigy-5000mah-5s-25c-lipo-pack.html)
[Turnigy 5000mAh 5S 30C Lipo Pack](https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack.html)


Thanks for your feedback ;)
```

---
## \#5 Posted by: mmaner Posted at: 2017-04-05T12:51:42.882Z Reads: 58

```
Wheels can be pricey, a lot of people use FlyWheel clones (I do).  Do a search on eBay for something close to you and the shipping will be less.  I get 90mm FlyWheel clones shipped for $26USD.

The lower the KV the more torque, the higher the KV the more speed.  For hills you want torque.  If it was me I'd use the 192KV motor, then maybe go dual later on.

THose batteries look good, you can get 2 and wire them in series and have a 10s2p 5000mah pack.  You can get 4 and wire 2 sets in series then in parallel and and have 10s4p 10000mah.
```

---
## \#6 Posted by: TTOO Posted at: 2017-04-05T12:52:54.057Z Reads: 57

```
So i shouldn't 3d print my enclosure, but how should i go about making something that looks clean ( or should i just buy one)?
My budget is around 530dollars and im looking for a board to mainly go to my school and back but it would be nice to have the range to go out and just have fun :slight_smile:
```

---
## \#7 Posted by: TTOO Posted at: 2017-04-05T12:55:56.904Z Reads: 54

```
[quote="mmaner, post:5, topic:19923"]
Those batteries look good
[/quote]

Just whats the difference between the three batteries i  linked (20C, 25C and 30C)?
```

---
## \#8 Posted by: mmaner Posted at: 2017-04-05T12:57:56.532Z Reads: 50

```
The higher the C rating the higher the AMP delivery, the the higher the amp delivery the more torque.  I use 30c lipos, but 20 should be fine, just not as torquey.
```

---
## \#9 Posted by: TTOO Posted at: 2017-04-06T13:42:18.663Z Reads: 46

```
Could you help me choose a vesc? I really dont know how to choose one. Thanks in advance :slight_smile:
```

---
## \#10 Posted by: mmaner Posted at: 2017-04-06T13:44:22.838Z Reads: 54

```
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
http://www.enertionboards.com/electric-skateboard-parts/vesc-x-programmable-brushless-motor-controller/
https://miamielectricboards.com/shop-1/vesc

I have used all of these, they are all very good VESC's.
```

---
## \#11 Posted by: TTOO Posted at: 2017-04-06T14:06:28.795Z Reads: 53

```
And what about these wheels?
diy-electric-skateboard-kits-parts/83mm-longboard-e-power-flywheels/
or is the extra size necessary?
diy-electric-skateboard-kits-parts/90mm-longboard-epower-flywheels/
```

---
## \#12 Posted by: mmaner Posted at: 2017-04-06T14:36:13.444Z Reads: 49

```
THose wheels should be fine.  I would look on eBay, you can get Flywheel clones for $25'ish.

http://www.ebay.com/itm/Blank-Pro-97mm-Multiple-Color-Longboard-Flywheels-ABEC-7-Bearing-Spacers/281842542918?_trksid=p2047675.c100011.m1850&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D40130%26meid%3Df0974d2965c2486f8614b3eae6c73cd6%26pid%3D100011%26rk%3D1%26rkt%3D12%26mehot%3Dpp%26sd%3D141727706244
http://www.ebay.com/itm/Blank-Pro-83mm-Multiple-Color-Longboard-Flywheels-ABEC-7-Bearing-Spacers/281661805302?_trksid=p2047675.c100013.m1986&_trkparms=aid%3D555012%26algo%3DPW.MBE%26ao%3D1%26asc%3D40130%26meid%3D2cafa0ececec4871a3a6599283f3a062%26pid%3D100013%26rk%3D6%26rkt%3D12%26sd%3D141727706244
```

---
## \#13 Posted by: TTOO Posted at: 2017-04-06T14:56:56.611Z Reads: 42

```
Problem is that they have 50$ shipping for me :frowning:
```

---
## \#14 Posted by: TTOO Posted at: 2017-04-06T15:07:03.481Z Reads: 49

```
Ok now that i basically have the electrical components, i still need a way to mount everything so first of all, how should i choose a motor mount?
I have to choose between these two:
13T/36T 12mm ABEC Drive Wheel Kit
16T/36T 12mm ABEC Drive Wheel Kit
And how should i mount the electronic?
Finally do i need any extra wires after buying the vesc batteries and motor?
```

---
## \#15 Posted by: mmaner Posted at: 2017-04-06T16:10:53.891Z Reads: 49

```
[quote="TTOO, post:13, topic:19923, full:true"]
Problem is that they have 50$ shipping for me
[/quote]
Uggghhhh, that sucks.  The TB wheels ares good, no worries there.

[quote="TTOO, post:14, topic:19923"]
I have to choose between these two:13T/36T 12mm ABEC Drive Wheel Kit16T/36T 12mm ABEC Drive Wheel Kit
[/quote]
I would go with a 16/36 pulley set, check out DIY/TB options.
diy-electric-skateboard-kits-parts/36t-abec-drive-pulley-belt-combo-kit/

DIY has motor mounts too, or PM @korryh, he makes them.
diy-electric-skateboard-kits-parts/single-bolt-on-motor-mount-only/

[quote="TTOO, post:14, topic:19923"]
how should i mount the electronic
[/quote]
Look at @psychotiller 's site, he makes awesome enclosure.  Very mod-able and tough.
http://psychotiller.com/products/shop/enclosures

[quote="TTOO, post:14, topic:19923"]
do i need any extra wires after buying the vesc batteries and motor
[/quote]
You will absolutely need some bits and pieces.  Look at hobbyking.com, or a local resource if you have one.  You will need silicone wire (14 & 10 gauge should be good enough), 5.5mm connectors, XT60 connectors, XT90 connectors & probably an XT90-S connector for a loop key, unless you batter has a BMS with an e-switch.
```

---
