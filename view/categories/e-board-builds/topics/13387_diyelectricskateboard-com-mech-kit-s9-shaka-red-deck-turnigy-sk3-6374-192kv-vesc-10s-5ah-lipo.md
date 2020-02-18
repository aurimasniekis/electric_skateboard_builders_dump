# DIYelectricskateboard.com mech kit &#124; S9 Shaka Red deck &#124; Turnigy SK3 6374 192kv &#124; VESC &#124; 10S 5Ah LiPo

### Replies: 8 Views: 2002

## \#1 Posted by: Yecrtz Posted at: 2016-11-21T00:34:18.998Z Reads: 284

```
Hi everyone, long time /r/ElectricSkateboarding and youtube lurker here. Decided the time has come to make my own electric longboard. The last couple of weeks I've been watching tutorials and red most of the information topics here on the forum. 

Before I throw my part selection on your screen, let me tell you a bit more about myself and my riding plans: I'm light, 62kg/136lbs and will be using the board to do city cruising and short trips around the area. I was roughly aiming at a max speed around 45kmh/27mph. The riding surface will mostly be flat, like the rest of the Netherlands.

My selection of parts:

* Sector Nine Shaka red (8-ply Maple) deck (already in my possession)
* The [Single Motor Mechanical Kit](diy-electric-skateboard-kits-parts/torqueboards-single-motor-mechanical-kit/) (from diyelectricskateboard) including:
** (1) TorqueBoards Bolt On Motor Mount v4 (Black)
** Choose between 50mm or 63mm Spacing.
** (2) 50 Degree TorqueBoards v2 Trucks (Black or Blue)
** (1) 36T Drive Wheel Pulley + (6) M6x50 Bolts (HTD5)
** (1) 16T Motor Pulley (HTD5)
** (1) 255mm 12mm High Torque Timing Belt (HTD5)
** (2) 265mm High Torque Timing Belt (HTD5) *Reverse Mount
** (4pcs – 1 set) 83mm 76a E-Power Longboard Wheels (Black)
** (2) 1/8″ Risers
** (8) High Speed ABEC Bearings
** (4) Bearing Spacers
** (8) Deck Hardware
* Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner Motor
* [TorqueBoards 2.4Ghz Mini Remote Controller](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/) (from diyelectricskateboard)
* [VESC BLDC Speed Controller](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/) (from diyelectricskateboard)
* 2x Turnigy 5000mAh 5S 20C Lipo Pack (in series)

As far as my knowledge goes, and my calculations are right this setup gives me 6912 engine revolutions per minute resulting in a max speed of 48 kmh/30mph, thus matching my expectations. Did I make any mistakes here?

Also, I would like to use an anti spark switch and 2 volt meters in my setup. Any recommendations and tips/tricks? The same goes for the enclosure, I'm not quite sure what I will be using for that. Last point, how do I attach the motor pulley to the shaft without it freewheeling? (probably a small and simple solution I overlooked?).

I would love to hear your opinion and maybe change some things before I order all the parts (if necessary atleast). Thanks!
```

---
## \#2 Posted by: Jinra Posted at: 2016-11-21T00:40:43.199Z Reads: 266

```
If you're going to be reverse mounting your drive train, you may need to modify the mount like I did here

<img src="/uploads/db1493/original/3X/a/5/a5d1e70893cc741e092fe15af59a6b065417b0d5.jpg" width="374" height="500"> 

Also with 16/36 in reverse mount, you'll need a 280mm belt. 265 is too short and will cause the motor to hit the trucks. You'll also want angled risers to help get the mount further from the ground. I'd also recommend 97mm wheels to help with that as well.

Honestly though, try to get the drive train mounted inward as it's a bit of work to make it work in reverse.

TB sells an antispark switch which will work as well. You can pick up any voltmeter that's made for 10s or has a 10s option. This is mine

https://www.amazon.com/gp/product/B01LQ7MT4K/ref=oh_aui_detailpage_o00_s02?ie=UTF8&psc=1
```

---
## \#3 Posted by: Yecrtz Posted at: 2016-11-21T13:58:24.606Z Reads: 202

```
Thanks for the reply!

I'm currently looking into which extra connectors I need to order to make everything fit.
The lipos have 4mm bullets so if I swap those out with [XT90](https://hobbyking.com/en_us/nylon-xt90-connectors-male-female-5-pairs.html) I can connect those in serie with [this](https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html) plug.

Step two will be changing the 5.5mm bullets on the spark plug to XT90 to connect those to the battery and XT90 of the VESC. Step 3, Change the 3x 5.5mm bullet plug on the vesc to 3x 4mm to connect the motor. Or should I go for 3x 5.5mm? Last thing is to use the [servo connector](diy-electric-skateboard-kits-parts/male-male-servo-connector/) to connect the receiver to the vesc. I'm probably going to solder the volt meter in the xt90 connector from the vesc.

I will also need some shrink tube and a spare belt. I'm not going for a reverse setup, so [this](diy-electric-skateboard-kits-parts/255mm-htd5-12mm-belt/) one will do? Is there a place where I can buy those for cheap in bulk? Do these belts have a specific number so I can find them on ebay?

Could someone confirm this will all work together, especially my connector plans?
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-21T19:54:42.908Z Reads: 180

```
I recommend XT60 headers just because it saves space. I also use 5.5mm bullets myself as I find 4mm bullets tend to slip out sometimes. Servo connector is good, just make sure it's long enough for what you need. They're super easy to find in other shops too, just search "male to male servo".

You should use a center distance calculator to find out what size belt you need (https://sdp-si.com/eStore/CenterDistanceDesigner)

I use vbeltsupply.com for my belts. However, they're search algorithm SUCKS. I can't even find the belt I want with their search. Instead, use google to search and find the result from vbeltsupply. Use the convention below to search

beltsize-pitch-width (example: 280-5m-15 will find you a 280mm belt with HTD5m pitch and 15mm width)
```

---
## \#5 Posted by: Yecrtz Posted at: 2016-11-21T20:25:47.390Z Reads: 166

```
Good idea to go for XT60, also added some 5.5mm connectors to my hobbyking basket. On the kit page I can choose between a 13 and 16T (HDT5 12mm) motor pulley. Which one do your recommend and why? According to the description it is a 255mm 12mm one so I suppose [this one](http://www.vbeltsupply.com/255-5m-12-synchronous-timing-belt.html) will be perfect (255-5m-12)? The amount of variables regarding belts is a little overwhelming.
```

---
## \#6 Posted by: Jinra Posted at: 2016-11-21T21:32:02.759Z Reads: 155

```
13 for more torque, 16 for more speed. I use 16T myself. I think 255 would work, but do a test setup and measure the C distance first.

It's a bit overwhelming at first, but once you get it down, you'll know for the future and never have to worry about it again.
```

---
## \#7 Posted by: Yecrtz Posted at: 2016-11-21T21:51:32.877Z Reads: 153

```
Thanks for your help! I just ordered all the parts + some extra stuff I need for the assembling. Going to buy a nice voltage meter locally here that can handle all the power.

Let the waiting games begin!
```

---
## \#8 Posted by: Blitz Posted at: 2017-12-29T19:33:11.377Z Reads: 64

```
How is the build going, You long board
 seems like what i was aiming for
```

---
