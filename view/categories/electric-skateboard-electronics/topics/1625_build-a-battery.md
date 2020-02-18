# Build-A-Battery

### Replies: 38 Views: 4750

## \#1 Posted by: mrquin Posted at: 2016-03-02T03:58:34.705Z Reads: 184

```
I'm thinking about building a 12S battery from a bunch of the Turnigy 1S 5Ah flat packs for the slim profile.
http://www.hobbyking.com/hobbyking/store/__18560__Turnigy_5000mAh_1S_20C_Lipoly_Single_Cell_.html

I'm pretty good at soldering (work as an EE), but I've never tried soldering battery packs.  Any tips or tricks for these packs?

For this build I'm hoping to use a BMS for this from here
http://www.batterysupports.com/44v-48v-504v-12s-100a-12x36v-lithium-ion-lipolymer-battery-bms-p-393.html

Based on what I've read here on the forums, at 12S 5000mAh 20C, I should be able to pull 100A so is that BMS correct?  Any suggestions on a charger?  What kind of range should I be expecting from this battery? I plan on using Hummina's hub motors and VESC.
```

---
## \#2 Posted by: NNGG Posted at: 2016-03-02T04:24:45.331Z Reads: 178

```
not worth it, just do two 6s packs in series
```

---
## \#3 Posted by: SpartanScrub Posted at: 2016-03-02T04:47:14.233Z Reads: 182

```
obviously that's the easy way to go but this does seem like a pretty cool project. Could make a super flat pack like this. But I guess you could just pull the 6s packs apart and get the same result lol might need a little resoldering though

As for the 100A, pretty sure that's just the max the BMS can handle I don't think these boards really pull that much current. Your battery could technically handle that (20x5Ah) but it would drain in a few minutes and probably toast the motors/esc in the process
```

---
## \#4 Posted by: Namasaki Posted at: 2016-03-02T04:51:01.562Z Reads: 171

```
There is some info on the forum about disassembling 6s packs and laying the cells out in a flatter  configuration.
I don't know what your budget is, But if you really want a low profile battery. The S.P.A.C.E Cell is only 1" thick.
It has a built in BMS, on/off switch and a capacity meter. Is 36 volts nominal at 270 watt hour which is good for about 10-12 mile range. And there are very nice enclosures that are specifically made to house that battery. Also it is made of lithium ion cells which are less hazardous, last longer and as I understand, they don't drop voltage as there depleted like lipos do. It stays at 36 volts.
Another option would be the Zippy Flight Max 8000 3s 30c. there only about 1" thick and you could put 4 in series
12s 8000mah good for maybe as much as 16 miles and 240 amps
```

---
## \#5 Posted by: mrquin Posted at: 2016-03-02T05:39:31.234Z Reads: 156

```
@Namasaki I could disassemble some 6s packs but then I'd be at almost the same pricepoint and require more work/risk in taking them apart. For 12 of these at $84 +BMS I'm still way under the price of a S.P.A.C.E Cell.

@SpartanScrub What BMS limit should I go for if 100A is overkill? 60A?
```

---
## \#6 Posted by: Iceni Posted at: 2016-03-02T06:15:50.026Z Reads: 148

```
The space cell is rated at 30A discharge and thats generally all you need for normal usage.
But if you want a little more headroom 40A should do, 60A should be plenty even if you plan to ride aggressively.
In perspective, the dual motor Raptor uses a space cell with good effect.

At least that's what i've gathered from reading around on the forum here for while.
```

---
## \#7 Posted by: lox897 Posted at: 2016-03-02T07:38:45.867Z Reads: 145

```
The SPACE Cell is 60 amp continuous I'm pretty sure. It's 10s3p.
```

---
## \#8 Posted by: SpartanScrub Posted at: 2016-03-02T08:39:14.849Z Reads: 141

```
Looking at [this old space cell thread][1], it was (or was going to be?) a 50A BMS.


*Edit: My bad. Says right on the website it's [60A][2]*


  [1]: http://www.electric-skateboard.builders/t/space-cell-opened-up/510/9?u=spartanscrub
  [2]: http://www.enertionboards.com/electric-skateboard-parts/space-cell-electric-skateboard-battery/
```

---
## \#9 Posted by: Iceni Posted at: 2016-03-02T12:25:22.785Z Reads: 133

```
Interesting, not sure if it's been an update then, since mine got a 30A fuse.
Maybe it's just a lower rated fuse for safety reasons.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-03-02T12:38:50.200Z Reads: 131

```
I've tested for peak amps going 5 degs uphill hard with dual hub motors running on 12s and still pulled less than 60amps total.
```

---
## \#11 Posted by: cmatson Posted at: 2016-03-02T22:06:06.177Z Reads: 122

```
30amp fuses can burst 60amps for a couple seconds, which is usually just the very beginning of your acceleration. 

Unless you pull the trigger down all the way from a dead stop, you aren't likely to blow the fuse: especially if you have the space cell optimized VESC settings.
```

---
## \#12 Posted by: mccloed Posted at: 2016-03-02T23:50:39.417Z Reads: 121

```
I, personally, would go for the overkill. I usually wire the BMS to not be limited. Only use it for balancing the cells. The tabs on the singe 5000mah Turnigy cells have solder friendly tabs. The only downside is you spend a little more money on the single cells as opposed to the 3s or 6s packs.
```

---
## \#13 Posted by: NNGG Posted at: 2016-03-02T23:57:43.440Z Reads: 119

```
Was just going to say that but you can lay them down like three 2S packs in series for a super low profile.
```

---
## \#14 Posted by: mccloed Posted at: 2016-03-03T00:47:23.539Z Reads: 118

```
That's what I do with two 4s packs to make 8s. Lower profile than 18650 li-ions!
```

---
## \#15 Posted by: NNGG Posted at: 2016-03-03T01:09:15.739Z Reads: 120

```
Lipos are the economy route! I love the regular 3S pack profile though
```

---
## \#16 Posted by: mrquin Posted at: 2016-03-03T02:22:33.677Z Reads: 118

```
which 4s packs are you using?
```

---
## \#17 Posted by: NNGG Posted at: 2016-03-03T02:31:00.611Z Reads: 115

```
Maybe these? : http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=9177
```

---
## \#18 Posted by: mccloed Posted at: 2016-03-03T05:14:38.788Z Reads: 114

```
I used the multistars. They do not have adhesive or glue between the cells.
```

---
## \#19 Posted by: NNGG Posted at: 2016-03-03T06:33:15.569Z Reads: 114

```
Is their "C" rating adequate or is more than 10C needed?
```

---
## \#20 Posted by: Adam0311 Posted at: 2016-03-03T22:31:15.467Z Reads: 110

```
Very interested in this the dual hub amp draw. Planning out a dual hub build on 12s now. What was the peak amps you've observed? Did you notice heat in the motors? 

[quote="Namasaki, post:10, topic:1625, full:true"]
I've tested for peak amps going 5 degs uphill hard with dual hub motors running on 12s and still pulled less than 60amps total.
[/quote]
```

---
## \#21 Posted by: Namasaki Posted at: 2016-03-04T00:26:19.410Z Reads: 104

```
<img src="/uploads/db1493/original/2X/e/ee28a895da72ca77553181984a21f7ab77a7742a.jpeg" width="375" height="500">

Charging up this hill at about 20mph, I'm drawing about 54 amps from the battery. I'm 185 lbs and the board weights about 18 lbs.
The motors do generate heat under heavy load conditions but it hasn't been a problem. 
They have fan wheels that draw air through them and the aluminum sleeves act as heat sinks and quickly draw heat out of the motors.
Most important thing is to run the max voltage 12s to keep current at a minimum
```

---
## \#22 Posted by: Namasaki Posted at: 2016-03-04T03:48:23.178Z Reads: 99

```
http://youtu.be/HNI7497BTkE
Battery was a little low only 44.7 volts
Running at half throttle 
19.7 mph
```

---
## \#24 Posted by: Namasaki Posted at: 2016-03-04T03:54:42.429Z Reads: 98

```
<img src="/uploads/db1493/original/2X/0/08bacd7077e6df392382262a158c9a0ffe5880a2.jpeg" width="375" height="500">
```

---
## \#25 Posted by: Namasaki Posted at: 2016-03-04T04:01:05.080Z Reads: 97

```
I read on another forum that lipos with low C ratings often have higher internal resistance than those with high C ratings. 
More resistance = more heat in the battery and less power to the motors
Here is a Zippy pack with one bad cell. It was like this right out of the box. HK replaced it with a good one no problem. A good new pack should have less than 5 miliohms per cell. 
<img src="/uploads/db1493/original/2X/2/233304cc1deb21e438b7803223110e2ab1e8a509.jpeg" width="666" height="500">
```

---
## \#26 Posted by: TF22 Posted at: 2016-03-04T06:18:43.137Z Reads: 93

```
Does it then make sense to use higher "C" batteries like 30C over 20C? Is it worth the money? I have 4 batteries at 20C and they are fine for my applications
```

---
## \#27 Posted by: Namasaki Posted at: 2016-03-04T06:34:04.987Z Reads: 92

```
Ya, I would say keep using the batteries you have. i'm using these 25c batteries and there working fine.
Just if I was shopping for new batteries, I probably would stay away from the multi rotor 10s batteries.
5000mah is plenty at 12s. I have gone 7 miles on dual motors with hill climbing and a lot of accelerating up to 25 mph and still not reached min voltage.
I just recently learned about the internal resistance thing and I highly recommend getting one of these meters from Hobby King. Its a great tool for monitoring the true condition of your batteries. And checking new batteries before putting them into service. The Zippy in the pic was brand new right out of the box with a bad cell !
```

---
## \#28 Posted by: Adam0311 Posted at: 2016-03-04T06:46:22.508Z Reads: 88

```
Awesome! Seriously appreciate the response and video. That hill is probably a bit longer than the hill I live on. Looks like I'll be good to go with the 12s.
```

---
## \#29 Posted by: Namasaki Posted at: 2016-03-04T07:14:10.917Z Reads: 90

```
Ya, your gonna love running 12s with dual motors.  The power is exhilarating !!!
And a little addictive…
```

---
## \#30 Posted by: mrquin Posted at: 2016-03-04T21:51:00.833Z Reads: 86

```
Are those Carvon dual hubs?  They look sweet. Thanks for the tips!
```

---
## \#31 Posted by: Namasaki Posted at: 2016-03-04T22:27:01.507Z Reads: 85

```
Yes, they are Carvon v2 dual hub motors. 
145 KV  2250 watts and up to 3 hp each. 
They have a lot of torque without sacrificing top speed. And the free roll is very good when coasting.
```

---
## \#32 Posted by: Adam0311 Posted at: 2016-03-21T04:24:27.929Z Reads: 77

```
How is the breaking on the dual hubs? Also are you using VESCs?
```

---
## \#33 Posted by: Namasaki Posted at: 2016-03-21T05:49:53.641Z Reads: 75

```
The braking is very good.
I'm using Torquesboard 12s Esc's
And 12s Lipo battery
product/torqueboards-12s-120a-car-esc-opto-hv/
```

---
## \#34 Posted by: Adam0311 Posted at: 2016-03-21T06:05:52.833Z Reads: 74

```
Thanks once again. I'm pulling the trigger on the dual, just trying to decide if I want to use VESCs or TB's esc like you. Seems like the VESCs aren't optimal for Carvon motors from some posts.
```

---
## \#35 Posted by: Namasaki Posted at: 2016-03-21T11:40:29.658Z Reads: 73

```
I haven't tried using Vesc so I can't comment on it.  
The TB's  are plug n play simple and very robust with heavy duty heat sinks.
Check with Run play back about using Vesc with Carvon.
```

---
## \#36 Posted by: treenutter Posted at: 2016-03-21T12:40:25.267Z Reads: 65

```
@Namasaki do you have a build thread? I'd love to know more about this enclosure.
```

---
## \#37 Posted by: Namasaki Posted at: 2016-03-21T15:40:03.603Z Reads: 63

```
No thread but here's info on enclosure. 

http://www.serpac.com/s182.aspx

http://www.mouser.com/ProductDetail/SERPAC/182-B/?qs=sGAEpiMZZMsrGrAVj6eTvSToVYgBUh0ZaoP0W9%252bc%252b2w%3d
```

---
## \#38 Posted by: lowGuido Posted at: 2016-03-21T15:48:07.625Z Reads: 66

```
@Namasaki what ESC's are you running there?
```

---
## \#39 Posted by: Namasaki Posted at: 2016-03-21T17:30:47.872Z Reads: 63

```
Torquesboard 12s Esc's
And 12s Lipo battery
product/torqueboards-12s-120a-car-esc-opto-hv/
```

---
