# Murad I - Vanguard 42&rdquo; Flex 2 &#124; Caliber II 50 10&rdquo; &#124; Dual 6355 190KV &#124; Whoosh boards mounts &#124; 10S2P Sanyo 20700b &#124; 2 x FOCBOX &#124; 90mm ABEC 11

### Replies: 38 Views: 2628

## \#1 Posted by: gmurad Posted at: 2018-07-20T12:21:06.550Z Reads: 398

```
Main components

* Loaded Vanguard 42" Flex 2:	http://www.longboarderlabs.com/product/loaded-vanguard-42-deck-flex-2/
* Caliber II 50 10: trucks:	https://www.amazon.com/Caliber-Trucks-Cal-50%C2%B0-Longboard/dp/B00NY3Q5NQ
* marcmt88 Caliber II drive system:	https://www.janux-esk8.com/product-page/caliber-drive-system-kit
* 2 x TB 6355 190KV	collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller
* 2 x FOCBOX: https://buildkitboards.com/collections/speed-controllers/products/focbox?variant=8114030575732
* 10s2p Sanyo pack from meepo: https://meepoboard.com/collections/parts-accessories/products/sanyo-20700b-battery-pack-10s2p-custom-made
* Ownboard Metal Battery Enclosure:	https://www.ownboard.net/collections/accessory-parts/products/metle-case-and-w1-deck-without-hand-hole?variant=13100413943850
* Nano V2 Remote:	collections/remote-controller/products/torqueboards-2-4ghz-nano-remote-controller
* Metr.at Bluetooth Module:	https://metr.at/shop
* Zealos bearings:	https://www.amazon.com/gp/product/B00BL9VCRE/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
* 90mm ABEC 11 (Already owned)
* 14/36T gearing

There are a bunch of other smaller components like Adaptors, heat shrink and so on, but everything together came to $1488.12. I realize I could have save more on some items like the remote, bluetooth module, motors and etc but time is also import for me, I rather spend less time shopping around and getting the items shipped together and faster.

This will be my 4th e-skate but my second DIY. I like metal cases, in the previous DIY build I spent a lot of time on different parts, for example, I built an aluminum case by hand and it turned out good but it took too many hours. This build should be fairly easy to put together which will also save time, the metal enclosures from ownboard will fit the pre-made Sanyo pack from meepo and I consider both of them good quality products.

My very first board was a boosted board and I never been able to recapture that experience with the other boards, my hope is that this build will do that but be even better: more acceleration, more range, better deck length and flex for my height/weight, bigger wheels for the roads here.

Some concerns:

 - I'm 225lbs so I worry about belt skipping. On another dual motor 12mm belt DIY it's a problem. I couldn't really do 15mm with the Caliber II trucks. My hope is that the Idlers on marcmt88's mounts will prevent skipping
 - Power: For this build I believe the battery will be the limiting factor. Sanyo 20700b has can do high discharge but it's still a 2p, hopefully it will be ok.
 - Range: On a Wowgo 2s with the same Sanyo 10s2p pack I could get around 22 kilometers of range, I hope I can get the same but I'm not sure if outboard motors use more power then hub mottors
 - Remote: This is not a big deal but I don't really like the nano remote but I like the mini remote even less. There doesn't seem to be an easy solution to this in the DIY world.

This is definetely not an original build, I've seen a lot of similar builds on the forum in the past but recently skatemetric released a video with actual benchmarks of a similar build and it stacked really well against other boards (Raptor 2, Boosted) so those number convinced me to do this. 

Everything has been ordered earlier this week, now waiting.
```

---
## \#2 Posted by: gmurad Posted at: 2018-07-21T12:16:10.456Z Reads: 329

```
Just realized that I didn't order the ESC Sensor wires, now I would have to pay high shipping fees to get it from Torqueboards: collections/electrical-connectors/products/vesc-sensor-wires

Will need to find another source

Also, I already have a bunch of 14 gauge silicon wire at home from other projects, I was planning on using that however I'm reading that I should go with 12 or 10 gauge to be safer.
```

---
## \#3 Posted by: AutoItKing Posted at: 2018-07-21T18:57:46.532Z Reads: 328

```
The Sanyo NCR20700B cells are rated for 15A continuous, maybe double that for burst (60A in pack). Also the wires (and XT60) coming out of the pack make it look like it was meant for a single motor build.

Dual motor builds are more resistant to belt slippage since there is basically double the number of teeth taking the load.
Belt drive is slightly less efficient since you have friction losses in the belt. Probably not a huge difference though.

14 AWG is not enough for a dual setup. I used 10 gauge for runs that carried the full current, and 12 where it splits.

You can find the sensor extension cables from almost anyone who sells or sold VESCs.
```

---
## \#4 Posted by: gmurad Posted at: 2018-07-21T21:41:26.885Z Reads: 305

```
Thanks for all these ideas.

That 10s2p pack is for the dual hub motor meepo board, I haven't noticed the 14 gauge wire they use! Hopefully it will be ok since it's a short distance. I was hoping to use XT60s all over the build for space savings, but I also have 5.5mm bullet connectors, maybe that's a better compromise.

I thought a lot about the 10s2p vs 10s4p. With 20 extra cells I would add an extra 2.65 lbs, but it would also mean that I would have to build my own battery and the perfectly fitting metal case I got from ownboard wouldn't work either so I would have to find something else like the eboosted enclosures.

I realize that the battery will be a bottle neck on this build, but hoping Sanyo 10s2p will be good enough to make it stronger then a boosted stealth and have more range.
```

---
## \#5 Posted by: AutoItKing Posted at: 2018-07-22T02:44:40.467Z Reads: 277

```
XT60's should be good enough, but keep in mind they are only rated for 60A continuous. I used XT90 where needed. Cruising current is of course lower than that limit, but I like to play it safe.
It should be able to keep up with a boosted stealth. Also keep in mind that Meepo tends to be Cheapo.

Speed assuming 16t/36t: 28 mph.
```

---
## \#6 Posted by: gmurad Posted at: 2018-08-07T16:50:32.745Z Reads: 257

```
Ended up upgrading the build to FOCBOX instead of the Torqueboards VESC. Everything has arrived at my home by last week except the battery from Meepo still waiting on that.
```

---
## \#7 Posted by: gmurad Posted at: 2018-08-07T16:54:06.663Z Reads: 260

```
I'm having some serious doubts on whether or not to route the Vanguard for the 2 x 10 AWG cables or just have the cable exposed under. I really want the clear look.

I already routed another deck of another build as a test before doing the vanguard but still don't feel too good about doing this to a $200+ deck. https://imgur.com/a/952rAa1
```

---
## \#8 Posted by: Schulerbible Posted at: 2018-08-07T22:34:10.231Z Reads: 258

```
I have the flex 1 and although I like the deck I would go with the shorter 38” if I would do it again. The 41” is just too long and awkward to carry around (e.g. public transport).

Also, those motor mounts are pretty long. I assume you need a 1/2 inch riser on the back to allow some space. This will end up with a higher ride height than what you are used to on your Boosted.
```

---
## \#9 Posted by: jaatis Posted at: 2018-08-12T16:10:29.436Z Reads: 266

```
I'm thinking of building my first esk8 with very similar components to yours @gmurad. If you already have the Ownboard enclosures, could you please measure the max. usable internal size of the battery enclosure? This would help me a lot to decide what kind of a batteries I could play with. Thanks in advance!
![case|354x362](upload://gXXfC2JHl8pH9ts359hYlifAfKb.jpg)
```

---
## \#10 Posted by: gmurad Posted at: 2018-08-12T23:14:06.302Z Reads: 254

```
I made an album here: https://imgur.com/a/fLizwkk

It's hard to measure the useable "square" space in the enclosure. It's full of non-square angles.

What kind of batteries are you considering? I highly recommend @Eboosted's enclosure, it would fit much nicer on the Vanguard. The only reason I'm using the owboard enclosure is because I'm using the meepo Sanyo Battery that was on Sale and is a direct fit on that enclosure. I'm already regretting that decision as I'm planning on opening up that pack and making it a 10s3p or 10s4p.
```

---
## \#11 Posted by: jaatis Posted at: 2018-08-13T13:52:57.292Z Reads: 229

```
Thanks for the images. I was considering lipos or a bit differently assembled 10s2p packs that are available from some EU vendors. But after seeing eboosted's enclosures I'm temped to build my own.. Let's see.
```

---
## \#12 Posted by: gmurad Posted at: 2018-08-27T00:42:25.965Z Reads: 236

```
2 full days of work, yesterday and today now build is done. I tested it and it rode pretty pretty! Went with FOC, Sensored, Motor: 80A, -35A, Battery: 20A, -12A

Might be safer to change the battery Max to 16A, I will monitor it.

After testing it I applied thread locker everywhere and now just need to wait 24 hours. Pics in the following post.
```

---
## \#13 Posted by: gmurad Posted at: 2018-08-27T01:31:36.404Z Reads: 266

```
Didn't take as many pictures as I wanted.

* Orbital sander with 80 grit took the spray on grip tape easily. 
(no picture for this step)

* Drilled some holes for the flat copper cable:
![image|281x500](upload://t0A9UcjMQ8enkA2ZXJKRtEzyhqR.jpg)![image|281x500](upload://yu038w1WNKE1oZUA2tvozxBmfDg.jpg)

* Taped flat wires with kapton tape
![image|690x388](upload://sdbjnErQrzAhtecspTdi3Tf4fuS.jpg)

* Heat Shrink and bullet connectors to save space
![image|690x388](upload://uZtV0iMIBFiZyM63HU0KjFM1vCd.jpg)

* Used XT60 on the battery side
![image|690x493](upload://hmgy8d5kjbnZFInYIjYcC4qMn9y.jpg)

* Motor mounts pre-assembled and flexible cable wrap on motor wires
![image|568x499](upload://lyGUokEJEBvbKzSprWf1D8FqUSA.jpg)

* Main electronics box was a tight fit. Added a bit of hot glue on all cables/parts that I didn't want movement
![image|281x500](upload://owjB6xTXnPlSyMR5x5j0mH4XYqU.jpg)

* Rubber Gaskets in place
![image|281x500](upload://ChCoKFMpbww268aVuzjZ2tefgx.jpg)

* Enclosures in
![image|690x388](upload://eyKlT5ny1hkAcpThY78SagRCki7.jpg)

* Making sure the pulleys and belt are well aligned
![image|491x500](upload://u4xE6Yn3o5PbhAf1nPMdztSZGb0.jpg)

* Simple grip tape design
![image|281x500](upload://eINukfVuQVq0iL4BuZNHz4ze0dT.jpg)

* Ended up removing the idlers
![image|690x388](upload://lIf4RwPd4BxGSOgc0fjSpu6p7H5.jpg)

* The Murad I joins the fleet
![image|281x500](upload://iGZ34hVPKCC0euWkOJgtvKB936e.jpg)
```

---
## \#14 Posted by: gmurad Posted at: 2018-08-28T11:42:03.916Z Reads: 227

```
Did the maiden voyage yesterday. Everything worked really well as far as I can tell! Max speed is hitting 41km/h which is great since I geared it to hit 42km/h

Here is the ride log: https://metr.at/r/DOZ6l

I set Battery max to 20A for each VESC so it's drawing 40 amps max and there is some heavy voltage drop in the graphs since I'm using a 2p pack. I know the Sanyo 20700b  is tested to do well with 16A continuous discharge without overheating so my question is: 

Is my setting of Max 20 Amps for each VESC too aggressive?

Another setting that I'm concerned about are the cutoffs, I think I have soft and hard at 31 and 28V
```

---
## \#15 Posted by: dalausb Posted at: 2018-08-28T12:17:23.344Z Reads: 217

```
Sweet lord! Nice build there! I'm completely new to the eSk8-world but whenever there's a question about batteries I'd run with Mooch's tests and recommendations. He's been testing 18650s for the vaping world for ages and there's a test of the Sanyo 20700b's up on e-cigarette-forum, too. 

In vaping it's not a big deal to exceed the continuous discharge rating by a good tad cause we're only pulling those amps for a couple of seconds at a time. For an esk8, though, I'd stick with the given (i.e. Mooch-tested) limit because you're pulling in a rather continuous manner. Everything above that is quite likely gonna ruin/degrade your batteries much quicker than usual/necessary.
```

---
## \#16 Posted by: gmurad Posted at: 2018-08-28T16:09:28.358Z Reads: 199

```
Did my first commute to work this morning, lowered the max battery amps to 16A on each VESC: https://metr.at/r/dZQWa
```

---
## \#17 Posted by: Jmding Posted at: 2018-08-28T16:56:01.997Z Reads: 211

```
That flat wire is really cool. Where'd you get that? Seems like a very elegant solution
```

---
## \#18 Posted by: gmurad Posted at: 2018-08-28T17:56:51.257Z Reads: 215

```
Flat Tinned Copper braid:

https://www.amazon.ca/gp/product/B003HGHQYM/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1

There is a version that is not Tinned but Tinned is easier.
```

---
## \#19 Posted by: Epskampie Posted at: 2018-08-29T06:55:22.100Z Reads: 205

```
Very nice build! I like the minimal grip tape design. The whole build reminds me of [this one](http://skatemetric.com/index.php/2018/07/03/ultimate-accessible-foosted-build-tutorial/) with the ownboard enclosures. 

What kind of range are you getting now that it’s done?
```

---
## \#20 Posted by: gmurad Posted at: 2018-08-29T10:03:26.247Z Reads: 197

```
Yesterday I rode 22km and still had 33V in the battery. At the end of tge commute there was sag but I was Still Able to go a up a hill at 25km/h. I'm 225lbs. Pretty happy with the range.

I mentioned the skatenetric build in the first post in this thread, however there were many boosted clones built in this forum before that.
```

---
## \#21 Posted by: Epskampie Posted at: 2018-08-29T11:25:12.813Z Reads: 181

```
That's awesome range! I might just start building the same thing next summer. Don't know if I can get used to the belt noise and drag coming from hub motors though...
```

---
## \#22 Posted by: gmurad Posted at: 2018-08-29T18:49:09.217Z Reads: 182

```
For this 22km ride I had battery max at 16A on each vesc so the power was just a bit underwhelming. 10s3p would be the sweet spot. it would probably give 30km of range for my weight with higher max batt amps, but then the build would be a bit more complicated.

Currently the battery is the bottleneck on this build, but I was aware of that before building it.

A few other observations. Flex 2 is really stiff compared to Flex 3, even for my weight it feels much different then riding a boosted v2 I didn't expect it to be that stiff. 42" is also a bit too long for a deck.
```

---
## \#23 Posted by: jerry9800 Posted at: 2018-08-29T20:52:11.546Z Reads: 174

```
Congrats on this build!! mine was similar to this except i'm doing a single motor set up and i used the ownboard 10s2p 4.0ah battery. Right now, I am waiting for the flipsky vesc 6 to arrive. Originally i had the torque board vesc 4.12, but it was dead on arrival and they want me to pay to replace it and i am not happy with that. Hopefully everything goes okay with the flipsky fsesc 6. Can't wait for it to arrive cause all i want to do is ride! i have never ridden an electric skateboard before.
```

---
## \#24 Posted by: gmurad Posted at: 2018-08-29T23:13:32.980Z Reads: 168

```
[quote="jerry9800, post:23, topic:62355"]
Hopefully everything goes okay with the flipsky fsesc 6. Can’t wait for it to arrive cause all i want to do is ride! i have never ridden an electric skateboard before.
[/quote]

I hear you. The return policy from torqueboards is really bad. I bought 2 of the VESC 4.12, didn't even remove them from the packaging and they wouldn't take them back. What does that say about their confidence in the product? Still trying to tell them brand new.
```

---
## \#25 Posted by: gmurad Posted at: 2018-09-01T21:03:55.610Z Reads: 153

```
Now that I have about 60km on this board things are really changing... I LOVE IT!

I'm really appreciating the 42" long deck and the flex on it now, the riding dynamics are just great! I find myself preferring to ride this board over the brand new lacroix I just got.
```

---
## \#26 Posted by: SecrIT Posted at: 2018-10-12T20:12:52.015Z Reads: 145

```
Jerry9800, how did your build go?  I'm about to start something similar.

I'm 170lbs, and was going to do a setup with the 10s2p 4ah battery from ownboard and 6355 single motor.

if you're done do you have any range data that you could share?

cheers,
dp
```

---
## \#27 Posted by: gmurad Posted at: 2018-10-12T23:20:42.724Z Reads: 153

```
The worst and only problem with my build are the motor mounts, had all sorts of problem with them. I'd try the dickyho mounts instead.

I rode about 22km once and still had a bit of juice left. Dual 6354, Focboxes, 16A max battery and 80A max motor current for each Focbox. I’m 225lbs and tall.

Power is good, probably better then a boosted stealth but nothing crazy because of the 16A battery max for each motor. It might be worth going 10s4p 30q or 10s3p Sannyo.
```

---
## \#28 Posted by: jerry9800 Posted at: 2018-10-13T04:04:06.972Z Reads: 149

```
Hi SecrIT,

I finished my build, however, my battery is in for repair. I have only gotten to ride my board twice for a short period of time on my street outside of my house. I am itching to go on longer rides as soon as i get my battery back. Sent it off sept 14 and still waiting for it to be sent back :( . sigh.... 

i'm 160 pounds and it seemed okay. I was afraid to go top speed on it lol. I felt like it did not accelerate as fast as i like, but speed seemed fine. Make sure you put some loctite on your clamp, cause mine started loosening after a very short ride. i did put loctite on my clamp, but i decided to only to not put loctite on one of the screws and that was the screw that went loose. 

i can update you when i get my battery back.
```

---
## \#29 Posted by: Russo Posted at: 2019-01-07T04:50:30.530Z Reads: 117

```
Hey! I know this is an old thread but I didn’t want to make a new one for this...
I am working on my first build and using the same Sanyo 20700b 10s2p battery on a one 6374 motor set up. Because it’s one motor, is it safe to put max battery amps at 30a? Thank you!
```

---
## \#30 Posted by: gmurad Posted at: 2019-01-07T10:38:59.190Z Reads: 117

```
For the battery it's safe. Even 32A is ok
```

---
## \#31 Posted by: gmurad Posted at: 2019-01-28T01:47:43.697Z Reads: 114

```
### Update to the build.
We are going through a harsh winter here in Toronto, Canada, so it's building time. Finally upgraded my motor mounts from marcmt88's mounts to Whoosh's mounts. I haven't ridden it yet but I'm very happy with the upgrade in terms of quality and design features. A lot of the problems I experienced are addressed with this design [mounts](https://whooshboards.com/product/dual-mount-complete-with-idlers-and-crossbars/).


![image|690x335](upload://yF0HdETDvf2gmtIgpjjPRDOFZ1K.jpeg) 

![image|690x335](upload://vCoAVR8IcInMrSpKE15QTd6bvQD.jpeg) 

![image|690x335](upload://wLlVUXimmiX1Z9St4zpGpcN5HU2.jpeg)
```

---
## \#32 Posted by: dcxeternal Posted at: 2019-02-21T03:47:21.542Z Reads: 102

```
Thanks for posting your build.  Gives me inspiration to start upgrading my Meepo NLS.
Pre-ordered a Focbox Unity and going to order a 10s2p Sanyo pack from Meepo as well.

I was really worry about the range on the 10s2p setup once I go for Torqueboard Direct drive or Belt motors once I get bored of the Meepo hub motors but my concerns are lifted due to your experiences. :+1::+1:
```

---
## \#33 Posted by: mixedcreation Posted at: 2019-02-21T04:34:45.750Z Reads: 96

```
Do yourself a favor and at the very least get a 10s3p setup.  The 10s2p is not going to be a smart choice unless you are building a very light, cruiser board for short distance travel. 

If youre spending money on a unity, then might as well get a battery worth the quality of your other components. 

If youre in the US, might want to get in touch with @hyperIon1 on a pack for your needs.
```

---
## \#34 Posted by: gmurad Posted at: 2019-02-21T04:53:13.717Z Reads: 96

```
With a Sanyo 10s2p pack you will get more range, acceleration and speed compared to something like a boosted stealth for example and the build will be lighter than using a larger battery pack, it also allows you to use the cheap and nice metal enclosures from Wowgo/ownboard  so there are good reasons to go with 10s2p. If he does get a Torqueboard DD a 10s2p battery would be a big bottle neck on the build tho.
```

---
## \#35 Posted by: dcxeternal Posted at: 2019-02-21T06:30:22.350Z Reads: 91

```
I dont know for sure what I want motor wise in the future but I do know I want the following:
Deck: Flex-y (NLS deck is pretty close to Loaded)
Weight: <18lbs
Speed: 26-30mph tops (42-48 km/h)
Power: 15% hill climb @ atleast 15mph (25km/h)
Range: 10 -12 miles (16-19km) 
Maintenance: Low to none

I weigh 165lbs so I think its pretty realistic i think.... lol
Basically like @gmurad I want this to eventually be a bit better than a boosted stealth in every aspect besides maybe the range.  Which I have no problems with getting a 2nd battery to carry in bag for longer rides.
```

---
## \#36 Posted by: dcxeternal Posted at: 2019-04-27T22:16:20.800Z Reads: 64

```
Hey any updates on how your battery is holding up and if you've rised the battery max over 16amp?
```

---
## \#37 Posted by: gmurad Posted at: 2019-04-27T23:00:56.037Z Reads: 67

```
I rode the board again this month (first time this year) and I can't tell any difference in the battery performance. Still getting 22km+. I kept battery max at 16A per motor (32A total). 

There are new options this year tho if you are looking for a ready to go pack + enclosure from china.

Some examples here
- https://www.meepoboard.com/accessories/extended-range-battery/
- (10s4p) https://apsuboard.com/collections/frontpage/products/38-apsuboard-dual-belt-electric-skateboard?variant=23717036425316
```

---
## \#38 Posted by: gmurad Posted at: 2019-04-28T13:39:56.659Z Reads: 55

```
Using the 10s2p 40T pack I linked above from meepo would make this build no longer be bottlenecked by the battery, however my concern is that range would go down significantly since I would set battery max to 30A for each VESC and I don't want to get less then 20km range. It's too bad because it would be a plug and play upgrade.

Here is a picture after I printed the Whooshboard mounts in PETG a while ago:

![image|690x335](upload://p3WhZK4WR15ZKcJLItAigVM7TGB.jpeg)
```

---
