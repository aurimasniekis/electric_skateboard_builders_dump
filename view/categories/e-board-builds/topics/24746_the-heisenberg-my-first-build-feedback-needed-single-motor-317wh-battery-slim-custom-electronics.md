# The Heisenberg - My first build (Feedback Needed) - Single Motor - 317Wh Battery - Slim - Custom Electronics

### Replies: 16 Views: 1009

## \#1 Posted by: Heisenberg Posted at: 2017-06-06T20:40:26.655Z Reads: 167

```
I've decided to start on my own adventure with building an electric skateboard, code name **The Heisenberg**, because well, no reason, don't question it. I've been looking around at other models people have created and I think I've come up with a good balance between price and performance. I plan to make two of these boards in the next few weeks for a friend and I. I've started to order the parts and wanted your opinion on them. I'm still not 100% set on these parts, and will take any advise from people who have built them before.



# The Parts List

###The Board
* BLANK Longboard Deck - $34 - [Ebay](http://www.ebay.com/itm/322501738120) - UNDECIDED
* Longboard 180mm Trucks Combo - $45 - [Amazon](https://www.amazon.com/dp/B01B08HCL0/ref=cm_sw_r_cp_dp_T1_j1WnzbYWT3VW9)
* Space Cell Pro Enclosure - $45 - [Enertion](http://www.enertionboards.com/on-sale/space-cell-pro-enclosure/)

###Battery
* 2x LG 36V 4.4AH 18650 Battery Pack 40 Cells - $70 - [Ebay](http://www.ebay.com/itm/172630688902?rmvSB=true)
* 100x 18650 Spacers - $5 - [Ebay](http://www.ebay.com/itm/331976414961)
* Hoverboard Charging Port - $7 - [Ebay](http://www.ebay.com/itm/112046817386)
* Hoverboard 42V 2A Charger - $8  - [Ebay](http://www.ebay.com/itm/262623199401)

###Motor
* N5065 1820W Brushless Motor - $62 - [Ebay](http://www.ebay.com/itm/122299056010)
* Hobbywinng SkyWalker 80A ESC - $30 - [Ebay](http://www.ebay.com/itm/182451350788)
* Hobbywing LED Program Card - $12 - [Ebay](http://www.ebay.com/itm/112036674110)
* 9mm Wide Drive Pulley Kit - $30 - [Enertion](http://www.enertionboards.com/electric-skateboard-parts/9mm-wide-drive-pulley-kit/)
* I need to find a good motor mount, but I'm currently planning to DIY my own with my 3D Printer and some Nylon/ABS filament. 

### Custom Remote - Base on [GreatScott!](http://www.instructables.com/id/Make-Your-Own-Electric-Motorized-Longboard/)
* Wii Nunchuck - $1.50 - [Ebay](http://www.ebay.com/itm/162517201847)
* 433Mhz Transmitter/Receiver - $2 - [AliExpress](https://www.aliexpress.com/item/433MHz-100-Meters-Wireless-Module-Kit-ASK-Transmitter-STX882-ASK-Receiver-SRX882-2Pcs-Copper-Spring-Antenna/32637181317.html?spm=2114.13010608.0.0.aM2Xqs)
* Battery Charger + Protection - $1.60 - [AliExpress](https://www.aliexpress.com/item/5PCS-Micro-USB-5V-1A-18650-Lithium-Battery-Charger-Board-With-Protection-Module/32657317361.html?spm=2114.13010608.0.0.aM2Xqs)
* ATTiny45 - $2 Each - [AliExpress](https://www.aliexpress.com/item/Free-Shipping-3PCS-ATTINY45-20PU-ATTINY45-DIP8/32669100067.html?spm=2114.13010608.0.0.aM2Xqs)
* NE5534P Amplifier IC - $2 - [AliExpress](https://www.aliexpress.com/item/10PCS-NE5534P-NE5534-DIP-8-Low-Noise-Operational-Amplifier-IC/32728186157.html?spm=2114.13010608.0.0.aM2Xqs)
* 3.7V 380mAh LiPo - $ 4.50 - [Ebay](http://www.ebay.com/itm/322386950137)

The total price of the board comes out to around $400 depending on shipping and vendors. I'm debating waiting until I can afford a dual motor setup, although I'm not sure how it will effect efficiency in terms of speed/range. 

I need help trying to find the best battery setup. I'm going to be using 40 18650 cells. I am not so knowledgeable when it comes to how I should set them up, or how I should manage them. I've been going between using a BMS and not. I haven't been able to find the best setup for my board. Any advise on this is highly appreciated.

Currently I have purchased the electronics for the controller, and the batteries for the board. Since these parts will not change based on which motor/ESC configuration I go with.
```

---
## \#2 Posted by: t0m_r1dd1e Posted at: 2017-06-06T21:14:55.671Z Reads: 142

```
Make a 10s4p battery. And YES you need a BMS. 

Also you should go with a bigger motor. 6355 or 6374 size. And you should go at least 12mm wide on the belt if you're only doing a single motor or it will skip like crazy.
```

---
## \#3 Posted by: Guacamoleface Posted at: 2017-06-06T21:22:18.846Z Reads: 140

```
[quote="t0m_r1dd1e, post:2, topic:24746"]
And YES you need a BMS
[/quote]

Its highly recommended but alot of people running li-lon setups without BMS, Im one of them :)

Edit: the batteries in the link already has a bms it seem? or are you gonna split them and rebuild to twice as big?
```

---
## \#4 Posted by: Smorto Posted at: 2017-06-06T21:22:23.708Z Reads: 135

```
I would not use those batteries, they are only rated for 10A continuous so a 10S4P would still only give you 40A continuous which is assuming that the seller is being 100% honest and the batteries live up to that. I would get genuine cells from liionwholesale.com or imrbatteries. I recommend Samsung 30Q, Samsung 25R, or Lg Hg2 cells.


Also, if you are going to use those trucks you are welcome to design a motor mount and print it but it will most likely not last very long, although @Print3r has some experience here I believe. I made my motor mount with those same trucks which you can check out the build log of my build for more details but here are some pictures.
<img src="/uploads/db1493/original/3X/3/4/342ff0350da7e960d1fab21caea5a288f20e500f.jpg" width="690" height="459">
<img src="/uploads/db1493/original/3X/e/e/ee9a73ad391d4b75999e35b688e0d710ce674ebb.jpg" width="690" height="459">
<img src="/uploads/db1493/original/3X/5/6/56a57363bf11a38e2b2b9a1416bf63569febc473.jpg" width="690" height="459">
```

---
## \#5 Posted by: Heisenberg Posted at: 2017-06-06T21:27:54.107Z Reads: 122

```
@t0m_r1dd1e

I was personally planning more of a 5S8P battery setup, in order to get up to 80A continuous out of the batteries. I've purchased a pack from them in the past and they are exactly like they are listed on eBay. They come with a BMS, but I plan to completely tear them apart for my build, and would like to only have to run a single BMS to charge everything if possible.  I can't decide on a single/dual motor, but I'll keep that in mind.
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-06-06T21:29:11.559Z Reads: 120

```
amperage is multiplied across parallel cells in your pack, not serial.

i would just go with the more commonly used caliber ii trucks.  you'll find mounts already made for them.  otherwise get ready to machine some bespoke parts.

also i would use a vesc.  i know they're pricey but the configurability will far out weight the extra cost.
```

---
## \#7 Posted by: Heisenberg Posted at: 2017-06-06T21:31:15.683Z Reads: 111

```
Whoops, Thanks for catching that.
```

---
## \#8 Posted by: t0m_r1dd1e Posted at: 2017-06-06T21:31:55.627Z Reads: 111

```
But if they really can put out a constant 10 amps each, 50 amps constant should be plenty.
```

---
## \#9 Posted by: Guacamoleface Posted at: 2017-06-06T21:34:12.619Z Reads: 106

```
Not very experienced with ESC, but I would say the VESC is one of the most sweet things I've bought for my board. However they are pricey, but well worth it.

Otherwise you should check how the ESC delivers in terms of braking power. I know alot of them are delivering very weak braking power - especially when only one motor. Search the forum and see if anyone use it and ask :)
```

---
## \#10 Posted by: Heisenberg Posted at: 2017-06-06T21:35:08.195Z Reads: 110

```
I plan to tear the thing apart and make a large 40 cell battery
```

---
## \#11 Posted by: Heisenberg Posted at: 2017-06-06T21:40:31.478Z Reads: 100

```
Is it possible to run two motors off of a single VESC?
```

---
## \#12 Posted by: Smorto Posted at: 2017-06-06T21:40:37.726Z Reads: 96

```
Then if you use 5s, you really aren't going to get enough voltage to get some good speed. if you plan on using 5s though, I wouldn't go for a VESC, if you are 6s or under, use a hobby esc, much cheaper. The VESC should be used if you go above 6s though.
```

---
## \#13 Posted by: Guacamoleface Posted at: 2017-06-06T21:51:33.776Z Reads: 92

```
No you're gonna want a vesc for each motor.

Im currently only single motor on mine and Im super pleased with it. I dont have much big hills here to climb with the board and Im fairly light(75kg). Just posted a video in my thread you can check out. - not max throttle tho.(10s4p)
```

---
## \#14 Posted by: SimosMCmuffin Posted at: 2017-06-06T23:25:07.140Z Reads: 81

```
There is a mistake in this thread's title. The total energy capacity of your 2x 36V 4.4 Ah battery packs is 316,8 Wh. where did you even get that 792 Wh of energy capacity for the battery?
```

---
## \#15 Posted by: Heisenberg Posted at: 2017-06-07T00:30:26.482Z Reads: 75

```
I actually have no clue how I got 792Wh, Must have messed something up while calculating it all.
```

---
## \#16 Posted by: Gabriel_Robinson Posted at: 2017-06-07T01:42:02.011Z Reads: 72

```
Nice name and profile picture. I am currently bingeing the show(Breaking Bad). Good luck with your build and ask me if you have any questions.
```

---
