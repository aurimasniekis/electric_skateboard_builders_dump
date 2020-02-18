# Super Spud &#124; Jet Spud &#124; 10S2P &#124; Dual 5055 &#124; ABEC11 Flywheels &#124; Psychotiller Enclosure &#124; VESC

### Replies: 17 Views: 2168

## \#1 Posted by: NickTheDude Posted at: 2017-10-24T19:20:54.016Z Reads: 398

```
Hey (Please excuse the cheesy name)! So I'm building yet another board. This one is primarily for my commute to work which is about 8km from where I live and mostly flat. Because of that I decided to try out the chinese dual 5055 kit to see how much power it can take. I'm shooting for ~1800W and I think they'll be able to handle it. Originally I was planning to put them on one of my other builds, but I saw the Jet Spud @JLabs  was selling and couldn't resist making a whole new build with it.

For this one I decided to go all out, Li-ion pack, fancy psychotiller enclosure and all that jazz.

The parts list is as follows:

* [Jet Spud 29" BKB Edition](https://buildkitboards.com/collections/decks/products/jet-spud-29-bkb)
* [270kV Dual 5055 Ebay Kit](http://www.ebay.ca/itm/DIY-dual-1500W-electric-longboard-drive-kit-83MM-wheel-7-trucks-CNC-mounts-/322549102279?hash=item4b196cb6c7:g:I0UAAOSwbtVZOttQ)
* [Psychotiller Coupe 12" Enclosure](https://psychotiller.com/product/the-coupe-12) 
* [Dual Torqueboards VESCs](collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller)
* [Bestech 60A 10S E-Switch BMS](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCB-D345.html)
* [10S2P 3000mAh LG HB6 Pack](https://liionwholesale.com/collections/batteries/products/lg-hb6-18650-battery-genuine-tested-30a-continuous-1500mah-flat-top-wholesale-discount?variant=13978272644)
* [1/4" Soft Rubber Riser Pads](http://www.ebay.ca/itm/122563419503?_trksid=p2047675.m570.l6004&_trkparms=gh1g%3DI122563419503.N41.S1.R1.TR1)
* [ABEC11 83mm 75A Flywheels](https://www.muirskate.com/longboard/wheels/1314/83mm-abec-11-flywheels-downhill-longboard-wheels)

Currently I'm waiting on the enclosure and risers to ship, as well as the battery pack. I don't have the necessary tools to build a pack for myself so @landonkun offered to help me out (THANK YOU THANK YOU THANK YOU!). 

I went with those cells since from what I can find they seem to have the highest discharge out of any 18650s on the market, and at 1500mAh a 2P is enough range for my commute which lets me make the pack smaller and lighter.

Other things to note, the motors are way to high kV for 10S so I'm going to run them with the ERPM limit at 60k. Any advice on how to set that up to avoid any risks would be appreciated. If I find that I'm lacking power or efficiency because of the limiter, I'm going to try and re terminate the motors to wye which should drop the kV down to roughly 170kV. At that point I'll probably increase the motor pulley size to get more top speed. If I do that I have a feeling that the belt will be rubbing up against the pulley cover, so I may need to file it down some. Also, the mounts that come with the kit aren't adjustable in any way so I'll likely have to file out the holes where the motor mounts on in order to properly tension the belt.

The bushings that the kit came with were complete garbage, and the baseplate they came with didn't have a long enough kingpin bolt to put on other bushings. Because of that I swapped the baseplate out to a caliber 2 baseplate, and put some Blood Orange 89A bushings on.

I'm super exited to get this thing running, so here are some pictures of what I've got so far to please your eyeballs.

<img src="/uploads/db1493/original/3X/8/f/8f48aa3871442bc7d254e2760dc5aaf21462c14b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/7/87f4e4f46b6ba9557165a753dc4d90aeda8e477a.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/d/edadd066698b32ee92fe74cff5841c07fbf45558.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/c/ac69d9785cfc4d90007d39f981071de2576456df.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/5/f/5f7194121dfe55d31fbcda8620ee8f58b21ebfc8.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/b/2/b2bc052628af075c901aa2e998b8583bddbfc7e8.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/f/2/f2ba2f3e844015aeb531a477a23ad311646c8f5c.jpg" width="666" height="500">
```

---
## \#2 Posted by: Michael319 Posted at: 2017-10-24T19:54:53.513Z Reads: 344

```
Are you using any risers?
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-10-24T20:03:26.565Z Reads: 347

```
Right now it's only got some 1/8" risers on it. The deck hits the motors before it hits the wheels though and sadly you can't adjust the motor position. I've got some 1/4" risers that are getting shipped over right now so hopefully they should help a little with clearance.
```

---
## \#4 Posted by: Jcullinan09 Posted at: 2017-10-25T07:20:14.555Z Reads: 321

```
Please update this post when you finish this build. I am very curious to know how this Chinese branded motor kit works out!
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-10-25T10:53:56.674Z Reads: 300

```
sweet build!

i’m building a spud atm also, single Tacon 245kv and...  10s6p!  20 miles range here we come
```

---
## \#6 Posted by: FredrikHems Posted at: 2017-10-25T11:31:41.987Z Reads: 283

```
@GrecoMan  I think with a 10s6p, you will easily destroy that 20 miles. At least if you use the samsung 30Q or similar!:sweat_smile:
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-10-25T11:42:39.243Z Reads: 285

```
13.2ah at 27wh/mile should get me just about 20 miles! 

was a bit of a plan change lol, was gonna use 6s2p but @scepterr gave me a deal I couldn’t resist on some 10s2p LG MF1 packs...
```

---
## \#8 Posted by: FredrikHems Posted at: 2017-10-25T11:48:11.372Z Reads: 288

```
27wh/mile?! You run pneumatics? if not what kind of setup is you running. I am using like 17wh/mile:joy:, and its quiet hilly where i live.
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-10-25T12:31:14.899Z Reads: 282

```
nope 6s single drive with 83mm wheels

I have a very good amount of 25%+ hills on my daily ride and almost always ride above 20mph
```

---
## \#11 Posted by: Jammeslu Posted at: 2018-01-27T16:54:06.683Z Reads: 239

```
How is voltage sag and do you get cut out caused by Battery? Im building the very same board so
```

---
## \#12 Posted by: stormboard1 Posted at: 2018-01-28T10:05:48.603Z Reads: 228

```
Any updates of this finished ?
```

---
## \#13 Posted by: NickTheDude Posted at: 2018-01-28T10:27:19.619Z Reads: 229

```
Sadly I've ran out of money/time for now, plus it's all snowy around here so I'll be waiting till summer to get back too it.

Plan is to route out a few mm of the deck and possibly get a bigger enclosure and maybe try fitting a 30T 10S2P if they ever become available. However for the time being it's gonna have to wait.
```

---
## \#14 Posted by: NickTheDude Posted at: 2018-04-16T23:56:56.066Z Reads: 196

```
ALRIGHT! SO. Its getting a little warmer out here so I've caught the ESK8 bug all over again. The plan has changed a little. Since I might end up upgrading to dual 6355s, a 10S2P isn't going to cut it. Because of this I've decided to go with a 9S 5000mAh 40C lipo setup. I'm also gonna use the Bestech BMS with an eswitch. I whipped up a nice diagram to get everything planned out. The idea is to have everything detachable so I can swap out a batter pack/BMS/charge port/volt meter/switch if anything needs replacing.

![Untitled Diagram|690x360](upload://gMRFK1BU0CLPDaTtv0MvoRQJCoL.png)

In the meantime since I really wanted to ride something, I soldered up some old parts I had lying around and made this disgusting monstrosity.

![20180413_111443|666x500](upload://7ITWZRm8ph8GGJh4fgrA6OEaBsK.jpg)![20180413_111422|666x500](upload://edEK9BjXBqj2097g4FZdnMWZTyP.jpg)

Psychotillers on the case making me a custom enclosure with interior dimensions of 340x160x32mm to fit everything and the batteries and everything I need to make a nice wiring setup is on the way here from HobbyKing.  Now I'm just waiting on Bestech to get back to me about ordering a BMS.
```

---
## \#15 Posted by: Deckoz Posted at: 2018-04-16T23:58:31.345Z Reads: 184

```
You better watch out for wheelbite dude.. no risers and 83mm wheels. Lol don't eat it..
```

---
## \#16 Posted by: NickTheDude Posted at: 2018-04-16T23:59:24.998Z Reads: 184

```
I've got some 0.25" risers on it, and anyways since you can't adjust the angle of the motor mounts the deck actually smacks into the mount before hitting the wheels.
```

---
## \#17 Posted by: Deckoz Posted at: 2018-04-17T00:01:17.054Z Reads: 188

```
But the front... The back doesn't even have to move. I've bit the wheels on the Potato multiple times not even trying on 83mm flywheels... Idk...guess you don't lean that hard..

Because 70mm wheels almost bite... 83 bit all the time for me.
![IMG_20180416_200344|666x500](upload://aR7MY7LKtutW6Z0YN9JvfqODOnC.jpg)
```

---
## \#18 Posted by: NickTheDude Posted at: 2018-04-17T00:06:41.313Z Reads: 188

```
Took a picture of me leaning on it pretty hard with all my weight. I can get the front wheel to bite but it's pretty hard and I have some decently hard bushings on it so the outside wheels actually start to come off the ground before it bites.

![20180416_200255|666x500](upload://dGlVV2hjFtRdNg3jlvBPJWEyqJr.jpg)

That being said I'll definitely be careful about it, I've had setups more prone to wheel bite before though.
```

---
