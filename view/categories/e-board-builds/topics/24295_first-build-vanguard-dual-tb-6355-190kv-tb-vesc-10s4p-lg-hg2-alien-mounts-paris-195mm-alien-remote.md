# First Build: Vanguard &#124; Dual TB 6355 190KV &#124; TB VESC &#124; 10S4P LG HG2 &#124; Alien mounts &#124; Paris 195mm &#124; Alien remote

### Replies: 46 Views: 4092

## \#1 Posted by: Mathias Posted at: 2017-05-31T21:06:30.004Z Reads: 426

```
Hi,

finally starting my first build! I read tons of build threads on this awesome forum, but I'd appreciate feedback for my plan:
I am aiming for 40km/h / 25mph, and I live in a very steep area, and I'd like to be able to tackle ~20% hills. I want to keep the option to change the gear ratio for increased top speed, though.

**Deck:** [Vanguard Flex 1](http://loadedboards.com/vanguard-longboard-skateboard): I'll go with the advice from @whitepony and use Flex 1.  

**Motors:** dual [TB 6355 190KV](diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/) should get me up the hills.

**ESC:** [Torque ESC](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/). I am planing to use FOC, and I read mixed reports about it. Although, I had the feeling that blown DRVs are usually caused by wrong configuration (as long as you have the v4.12). So I hope these ESCs should do. 

**Battery:** 10s4p [Samsung 30Q](https://www.imrbatteries.com/samsung-30q-18650-3000mah-15a-flat-top-battery/). Thanks for the comments, guys! I'll go for these instead of HG2.

**Trucks:** [Paris 195mm](https://www.amazon.com/Paris-195mm-Black-Skateboard-Trucks/dp/B00EKR48T8). I like the idea of having a bit wider trucks and wide belts. So Paris 195 mm it is.

**Motor mount:** [Alien mounts](http://alienpowersystem.com/product-category/cnc-kit/transmission-parts/page/2/). First: those go onto Paris trucks. Second: I like the flexibility to switch to different motors and trucks, including DIY truck adapters @whitepony style.  

**Pulleys:** [15mm 15T/40T pulley kit](https://www.electric-skateboard.builders/t/lower-price-15mm-steel-motor-pulley-40t-abec-flywheel-mbs-all-terrain-pulley/16586) from @Titoxd10001. Probably 12mm would be enough, but I really want to go for maximum reliability and durability. Also I don't like the very limited choice of belt vendors and lenghts for 12mm. This was the only option that I found to have wide belts, a large motor pulley, and still sufficient gear reduction. 

**Remote:** [Alien remote](http://alienpowersystem.com/shop/). I figured I'll give this remote a shot. I'll test it's connection and failsafe feature before I actually step on the board, but I expect it to work just fine. Looks solid, not as bulky as (unmodded) GT2B, receiver with enclosure and antenna, and a fail-safe feature. 

**Enclosures:** [printed](https://www.electric-skateboard.builders/t/loaded-vanguard-and-never-summer-reaper-enclosures-for-sale/17137/45) by @Eboosted I like the idea of making carbon fiber or thermoformed enclosures myself. But at the moment I have no tools and equipment whatsoever. Also I can't wait to finally stand on an esk8. Next build I guess...

**Wheels:** [90 mm flywheel clones](diy-electric-skateboard-kits-parts/90mm-longboard-epower-flywheels/). The roads here can be rough. I want big wheels, I don't like green wheels. So clones it is.

**BMS:** [bypassed 30 A batterysupports](http://www.batterysupports.com/36v-37v-42v-10s-30a-10x-36v-lithium-ion-lipolymer-battery-bms-p-265.html). This is a tricky thing: I definitely want to bypass it and only use it for charging. On one hand the protection of the battery is not really needed if you carefully choose the settings of the VESC. But what's more important: I don't want this thing to "protect" my battery by deactivating my brakes... "So I totally ran into this car, but at least my battery didn't get overcharged." I live pretty much on a hill, so for my usual rides I will simply not fully charge the battery and live happily ever after. 
Since I bypass it anyway, I could probably take a way smaller BMS/balancing circuit , but I couldn't find one with a decent balancing current. In my opinion a maximum balancing current of 65 mA is already quite small for a 12 Ah pack. 

**All the other stuff:** I am of course aware that I'll need tons of small pieces like an antispark and connenctors etc... First thing will be a diy spotwelder that I'm working on. I will update as the parts arrive...

Cheers everyone!
```

---
## \#2 Posted by: TranxFu Posted at: 2017-05-31T21:26:20.354Z Reads: 365

```
All fine :) But go for 30Q instead of the 25R. They are better in every regard. 

And I'd still opt for the kegels. Even if they are 83mm. Just way better than clones.
```

---
## \#3 Posted by: Mathias Posted at: 2017-05-31T21:35:55.073Z Reads: 356

```
Thanks for the feedback! But I was going for HG2. They are rated for 20A/4A discharge/charge. Q30 only for 15A/4A. And I'd really like the 90mm wheels, and it seems there are plenty of decent clones around. I'm not sure which ones are the best, though.
```

---
## \#4 Posted by: Smorto Posted at: 2017-05-31T21:57:37.645Z Reads: 334

```
How about these    https://liionwholesale.com/collections/batteries/products/basen-4500mah-26650?variant=14135870212

You could build a 10s2p with the same amperage for a little less money and less space in your enclosure.
Or you could build a 10s3p with more range, way more amp draw, less space, and less money.

EDIT- The 10s3p would be more expensive.
```

---
## \#5 Posted by: Mathias Posted at: 2017-05-31T22:03:30.973Z Reads: 324

```
[quote="Smorto, post:4, topic:24295"]
You could build a 10s2p with the same amperage for a little less money and less space in your enclosure.Or you could build a 10s3p with more range, way more amp draw, less space, and less money.
[/quote]

But it is not cheaper. The charge/money ratio and charge/weight ratio is way worse than for HG2.
```

---
## \#6 Posted by: Decdog Posted at: 2017-05-31T22:06:17.898Z Reads: 295

```
Nice build plan! It should work!
```

---
## \#7 Posted by: Smorto Posted at: 2017-05-31T22:17:13.696Z Reads: 301

```
Im sorry, I spoke too soon about the 10s3p pack of the Basen cells, however, for around $17 extra, IMO you could build yourself a much larger pack.

A 10s4p pack of theLg HG2 cells would cost **$200** for the cells. This would give you **12,000 Mah, 80A continuous pack.**

A 10s3p pack of the Basen Cells would cost **$217** for the cells. This would give you **13,500 Mah, 120A continuous pack.**

However, I am not sure about the weight and I am assuming you are correct about their ratio of power and capacity to weight and size.
```

---
## \#8 Posted by: Peeta Posted at: 2017-05-31T22:20:35.870Z Reads: 292

```
Sorry if I hijack your thread a little bit. I plan on doing a similar build as to the trucks, board, motors, and escs. What would   you guys say if I used two 6s lipo batteries (1 for each esc+motor) instead and skipped the bms? For simplicity sake, is that possible?
```

---
## \#9 Posted by: Mathias Posted at: 2017-05-31T22:30:13.253Z Reads: 290

```
OK, I didn't use the bulk price for the energy/money ratio:
HG2: **230 Wh/kg**, 2.2 Wh/$, 
Basen: **170 Wh/kg**, 2.3 Wh/$
The increased weight is a no-go for me, and there is no use for the additional power, since the 10p4s will give pretty much the maximum that the VESC can handle. So I get the same power at the same price with a significantly increased weight. And it will not fit as nicely into the enclosures.

EDIT: Corrected units... not Wh/g
```

---
## \#10 Posted by: Smorto Posted at: 2017-05-31T22:32:56.096Z Reads: 276

```
Ahhh I see, the higher amp draw would lead to less stress on electronics I think, as well as reduce voltage sag though that shouldn't be a big issue anyway. The Basen cells would give me slightly more range as well but if they don't fit in your enclosure and your mind is mad cup about the Hg2 cells, that is completely fine :slight_smile:.
```

---
## \#11 Posted by: TranxFu Posted at: 2017-05-31T22:35:09.005Z Reads: 264

```
I'd still opt for the 30Q over the HG2. The discharge curve of the 30Q is superior to all of them. And they have way less voltage sag than the HG2. I went with 25R for my build but I'd trade for 30Q every day :)
```

---
## \#12 Posted by: Mathias Posted at: 2017-05-31T22:36:28.323Z Reads: 272

```
[quote="Peeta, post:8, topic:24295, full:true"]
Sorry if I hijack your thread a little bit. I plan on doing a similar build as to the trucks, board, motors, and escs. What would   you guys say if I used two 6s lipo batteries (1 for each esc+motor) instead and skipped the bms? For simplicity sake, is that possible?
[/quote]

I looked into LiPos too, and decided against them because they are usually way heavier for the same amount of energy, and have a way shorter life span. Also you will need a balance charger. 
In my opinion LiPo can make sense for you in the following case: my pack Li-Ion is pretty large, but it NEEDS to be this big to give me the full power. A smaller pack will not give enough Voltage/Amperage. You WILL, however find LiPos with way lower capacity and at lower cost that will provide you with 80A discharge. So if 10s4p exceeds your budget, you might go for LiPo. Otherwise I would bite the bullet, which also means spot welding and all the crap that comes with it. You'll get a way lighter and more durable pack with Li-Ion.

EDIT: Oooor, the Basen cells that @Smorto suggested here could be a good option for a small pack with full power :wink:. Now I see an upside to them!
```

---
## \#13 Posted by: Mathias Posted at: 2017-05-31T22:37:59.200Z Reads: 251

```
[quote="Smorto, post:10, topic:24295"]
Ahhh I see, the higher amp draw would lead to less stress on electronics I think, as well as reduce voltage sag though that shouldn't be a big issue anyway. The Basen cells would give me slightly more range as well but if they don't fit in your enclosure and your mind is mad cup about the Hg2 cells, that is completely fine :slight_smile:.
[/quote]

I don't see how. You get more range per cell, but that's not what it's about, right? You don't get more range for your $$, and your board will be way heavier. So I don't see the upside of the Basen.
```

---
## \#14 Posted by: Mathias Posted at: 2017-05-31T22:41:42.734Z Reads: 270

```
[quote="TranxFu, post:11, topic:24295, full:true"]
I'd still opt for the 30Q over the HG2. The discharge curve of the 30Q is superior to all of them. And they have way less voltage sag than the HG2. I went with 25R for my build but I'd trade for 30Q every day
[/quote]

Hm, OK. I didn't really go as far as comparing discharge curves. But are you sure that the 30Q still comes out in top if you discharge both at the same Amperage? Because the HG2 is rated for a higher A, and the curve highly depends on that. Could you post a direct comparison? I really want the 40A/motor. At my weight and the mad hills around here I need insane torque.

EDIT: Found it
http://abload.de/img/lginr18650hg2vssamsun8ppq8.png

The discharge curves at 15 A are about the same. I fell better with drawing 20 A from the HG2, though.
```

---
## \#15 Posted by: Smorto Posted at: 2017-05-31T22:55:23.930Z Reads: 257

```
The upside IMO is that dollar for dollar, you get more Wh which essentially means more range.

Using standard pricing (not bulk) we calculate that the **LG cells** have 3.6* 3=**10.8 Wh per cell** (using nominal voltage). 
Then we take that and divide it by the price for each cell which gives us 10.8/6=**1.8 Wh per Dollar**




Same thing for the **Basen cells** gives us 3.7*4.5=**16.65 Wh per cell** (using nominal voltage)
Then we take that and divide by the price of each cell which gives us 16.65/7.98= **2.09 Wh per Dollar**
```

---
## \#16 Posted by: Mathias Posted at: 2017-05-31T22:59:28.521Z Reads: 248

```
Except I'll by the [HG 2 for 5$](https://www.imrbatteries.com/lg-hg2-18650-3000mah-20a-flat-top-battery/), which will give you about the same WH/$ as the Basen. :wink:
```

---
## \#17 Posted by: Smorto Posted at: 2017-05-31T23:03:29.081Z Reads: 270

```
<img src="/uploads/db1493/original/3X/a/0/a0cc3bad03215d88a5228ac9bfc2b31597764e3f.png" width="690" height="280">

This says $6. If you are taking about the bulk pricing, I mentioned in that post that I would be using the standard pricing, not the bulk :wink:.
```

---
## \#18 Posted by: Mathias Posted at: 2017-05-31T23:10:29.926Z Reads: 270

```
[quote="Smorto, post:17, topic:24295"]
This says $6. If you are taking about the bulk pricing, I mentioned in that post that I would be using the standard pricing, not the bulk :wink:.
[/quote]
Don't you think it makes more sense to use the price that you actually have to pay for the comparison? I really think as long as you don't need more amps, you should go with HG2/30Q (@TranxFu has intrigued me now and I am looking into those too).  If you are on a tight budget and want a small pack rated for 80A, this might be a good choice. But the extra weight kills it for me.
```

---
## \#19 Posted by: nihliphobe Posted at: 2017-05-31T23:31:39.307Z Reads: 251

```
@Mathias What did you have in mind for the diy spotwelder? I'm in a similar boat and trying to avoid shelling out the 200$ for something commercial :wink:
```

---
## \#20 Posted by: Mathias Posted at: 2017-05-31T23:40:33.390Z Reads: 273

```
[quote="nihliphobe, post:19, topic:24295"]
@Mathias What did you have in mind for the diy spotwelder? I'm in a similar boat and trying to avoid shelling out the 200$ for something commercial :wink:
[/quote]
I'll try a quick and dirty solution with capacitors and a lab power supply:
https://www.aliexpress.com/snapshot/0.html?orderId=84158446186333&productId=32570929215
http://www.ebay.com/itm/60V-5A-DC-Regulated-Power-Supply-Adjustable-Variable-Switching-Digital-Lab-/192150061976?hash=item2cbd094398:g:sjkAAOSw32lYvklW
The capacitors are dirt cheap and the power supply will be my adjustable 5 A charger (in combination with the BMS). The first parts will arrive any day now, and if it doesn't blow up I'll report about it in the DIY spot welder threads. But for now I don't want to make any promises.  In principle I like the solutions using car batteries, but I don't have a car at the moment and no salvage yard anywhere near me, as a cheap source.
```

---
## \#21 Posted by: Smorto Posted at: 2017-06-01T00:48:01.049Z Reads: 250

```
Well If I was using the bulk price, the Basen cells would be discounted as well :slight_smile:. Yes, I understand that cell for cell the Basen cells way more however, you will need less of them to get a similar pack to the HG2 cells. I also like the fact that by needing less of them, you take up less room in your enclosure. If weight is that big of an issue though, by all means go for the HG2 or 30Q, I was just trying to bring a new idea into the mix :slight_smile:.
```

---
## \#22 Posted by: Mathias Posted at: 2017-06-01T02:47:46.618Z Reads: 244

```
I used the discounted price for both. Those things are way larger than 18650 cells, hence the name 26650. I will not fit nearly as much energy into the same enclosure. Look at this:
<img src="/uploads/db1493/original/3X/4/c/4cb230ff1fd851a7e0d39c6feefc3cfb99006b96.png" width="454" height="177">
So as I said: they are good if you want high discharge with few cells. Apart from that they are outperformed by the 18650 in energy/weight and energy/space. Energy/$$ is the same.
```

---
## \#23 Posted by: will_manners Posted at: 2017-06-01T02:48:55.185Z Reads: 236

```
The capacity and voltage sag differences are negligible. However, for the same performance the 30Q is generally cheaper than the HG2.
```

---
## \#24 Posted by: Mathias Posted at: 2017-06-01T02:54:23.184Z Reads: 244

```
[quote="will_manners, post:23, topic:24295, full:true"]
The capacity and voltage sag differences are negligible. However, for the same performance the 30Q is generally cheaper than the HG2.
[/quote]
Can you recommend a vendor? What I found so far was about 5$/cell for either, unless it was a vendor that doesn't really seem trustworthy. I've read a lot about fake HG2 and 30Q cells. Looking at the discharge curves it seems that the higher Amp rating for HG2 is kind of arbitrary compared to 30Q... Well, and the 80 Amp would really only be drawn for a short time...
```

---
## \#25 Posted by: whitepony Posted at: 2017-06-01T04:39:29.041Z Reads: 240

```
[quote="TranxFu, post:11, topic:24295"]
And they have way less voltage sag than the HG2
[/quote]

i used hg2 in pretty much all my builds with equal or less than 40 cells and even down to 30cells, they sag little to no! very happy with hg2!

@mathias the flex2 might be too soft for 90kg, its probably borderline even for my taste for soft boards! about stability: i go 50kph all the time with my flex2 vanguard and my even softer diy bamboo deck - never ever had speed wobble, but im also running cast ronins which i like a million times better than paris (which I like even less than calibers)!
```

---
## \#26 Posted by: Mathias Posted at: 2017-06-01T05:19:32.609Z Reads: 249

```
[quote="whitepony, post:25, topic:24295"]
@mathias the flex2 might be too soft for 90kg, its probably borderline even for my taste for soft boards! about stability: i go 50kph all the time with my flex2 vanguard and my even softer diy bamboo deck - never ever had speed wobble, but im also running cast ronins which i like a million times better than paris (which I like even less than calibers)!
[/quote]

@whitepony Thanks for the feedback! I guess I'll switch to Flex 1! About the trucks: yeah, I read all your build threads and noticed a slight preference for cronins :wink:. I considered getting them but got scared off by the need for the DIY mount adapter and the extended axle to fit 15mm belts + dual 6355 on them...
```

---
## \#27 Posted by: ChrisChaput Posted at: 2017-06-01T06:40:12.733Z Reads: 255

```
I know that that Flywheel clones are cheap and clones come in different colors, but they typically have really bad urethane and no chemical bond with the core. They also represent a slap in the face to me and my company who designed the first series of Flywheels and Flywheel Cores back in the year 2000. We did all of the design work, testing, racing, tooling, marketing, and advertising, and the Chinese just knocked us off without having to do any of the heavy lifting. Argh. But I'm not here to whine about the clones, I'm here to let you know that there will be a number of "non-green" Flywheels made right here in the USA in both our Classic and Reflex formulas. We've started to co-brand genuine Abec 11 Flywheels. Metroboard is doing red wheels with black cores (and possibly black wheels in the future), Carvon will be doing blue on black, and soon Evolve and others will be bringing out even more colors.

Perhaps even more exciting, Abec 11 is planning on making some new wider "SuperFly" wheels in our exclusive 74a Reflex Formula urethane, They'll be lime green on orange cores, but other companies may co-brand them in other colors as well. The sizes will include 83mm, 90mm, 97mm and 107mm, and the inside edge will be 100% compatible with all existing flywheel pulley adapters. SuperFly's are wider to the outside and therefore "offest" instead of centerset. They are a bit like our popular HD wheels, but with the Flywheel core. They have a much wider contact patch and a more flexible outside lip than the "Classic" Flywheels. I want to also provide 32T, 34T, 36T, 38T, and 40T wheel pulleys that you can slip into OR bolt into Flywheels with or without a pulley bearing. We'll be testing these out in a 71a durometer to see how the hold up. The 74a is already butter smooth, but we need to know how soft Reflex can go. 

I'd encourage all the eSk8 companies to co-brand some Abec 11 Flywheels in order to get great urethane in more colors out there. I'll do everything that I can to support the electric skateboard industry with wheels, trucks, bushings, bearings, pulleys, and motor mounts - the mechanical side of things.

Sincerely,

Chris Chaput
Abec 11 Genuine Flywheels, proudly made in Huntington Beach, CA *** USA ***
```

---
## \#28 Posted by: Smorto Posted at: 2017-06-01T10:08:19.345Z Reads: 213

```
Ok, thanks for the info :slight_smile:.
```

---
## \#29 Posted by: Maxid Posted at: 2017-06-01T10:18:23.241Z Reads: 228

```
[quote="TranxFu, post:11, topic:24295, full:true"]
I'd still opt for the 30Q over the HG2. The discharge curve of the 30Q is superior to all of them. And they have way less voltage sag than the HG2. I went with 25R for my build but I'd trade for 30Q every day :)
[/quote]

That's not true. The king right now is VTC6. HG2 are also "better" than 30Q because they can withstand even higher currents. The reason to use 30Q over HG2 is their price.
```

---
## \#30 Posted by: TranxFu Posted at: 2017-06-01T11:42:48.594Z Reads: 219

```
pardon me then :) I've somehow gotten the idea that they were the go to 18650 recently.
```

---
## \#31 Posted by: Maxid Posted at: 2017-06-01T11:46:10.579Z Reads: 240

```
[quote="TranxFu, post:30, topic:24295, full:true"]
I've somehow gotten the idea that they were the go to 18650 recently.
[/quote]

They are - but only because we are all cheap bastards ;)
```

---
## \#32 Posted by: jon-liionwholesale Posted at: 2017-06-05T23:07:21.657Z Reads: 250

```
Since my job is basically testing batteries all day on high end equipment and engineering battery packs, I figured I could give some input on the HG2 vs 30Q vs VTC6 vs Basen argument.  Note the links I post will be to our website, hopefully that's OK.

Since the end of 2016 HG2's have been worse after LG Chem retooled manufacturing, so you have to be careful of the results you look at and when they were tested.  Despite LG's higher 20A rating, the 15A 30Q and VTC6 perform better at both 15 and 20A.  HG2 is still an awesome battery but it's outshined by the 30Q and VTC6 now after the HG2 changes.  The VTC6 is the absolute best of the bunch, but pricing is high on them.  Personally I recommend the 30Q to most people as it's very close to as good as the VTC6 but at a much lower price.

Here's a link to all the batteries above since this forum will only let me put two links in here, remember that all of these get quantity discounts for buying in bulk:  [3000mAh high discharge batteries](https://liionwholesale.com/collections/batteries/3000mah+18650?sort_by=price-ascending)

As for the Basen 4500mAh, it's a great 26650 but it's a little affected by what I call "Chinese Ratings Syndrome".  Really it shouldn't be used above 25A or so, and if you're using it at high current it's closer to 4200-4300mAh.  If you absolutely want a 26650, the [iJoy 26650](https://liionwholesale.com/products/ijoy-26650-battery-40a-4200mah-genuine-and-tested) is the way to go as it can comfortably go to 30A.  It's phenomenal.  But even that I think the 30Q is usually going to be better on both a performance/weight perspective, a performance/size perspective, and a performance/cost perspective.

In summary, if you want the best of the best, go with the VTC6.  If you want very close to that at a much lower price, go 30Q.  I wouldn't recommend going 26650 at this time unless you have a really good reason to.
```

---
## \#33 Posted by: Mathias Posted at: 2017-06-06T02:54:46.323Z Reads: 226

```
OK thank you, that is really helpful! I guess I'll change my plan to 30Q...
```

---
## \#34 Posted by: smurf Posted at: 2017-06-08T07:02:40.877Z Reads: 214

```
I would be interested in your opinion of the new 20700 sized battery.
```

---
## \#35 Posted by: jon-liionwholesale Posted at: 2017-06-08T13:31:51.004Z Reads: 213

```
New 20700's are awesome.  Unfortunately the two really good ones, the 20700A and the Samsung 21700, are impossible to get at the moment.  We do have the [iJoy 20700 3000mAh](https://liionwholesale.com/products/ijoy-20700-battery-40a-3000mah-genuine-and-tested) and the Panasonic [NCR20700B 4000mAh](https://liionwholesale.com/products/panasonic-sanyo-ncr20700b?variant=30186936017) which are both very solid cells.  The iJoy would be the better one for this application, the NCR20700B is more of a high capacity long lasting cell so it's more at home doing 8A or less with quick bursts up to maybe 15A.  The iJoy can do 30A with no problem.  Actually if you have the little bit of extra room and the extra budget for it using iJoy 20700s in place of 18650s would be pretty cool.  Probably not worth the cost though.
```

---
## \#36 Posted by: will_manners Posted at: 2017-06-08T14:53:55.021Z Reads: 207

```
@ChrisChaput  Very exciting stuff! Can't wait to see what you guys offer in the future. With the scarcity of the highly praised 75A's it's encouraging to see that you're looking at doing even softer durometers! Can't wait for the 71A ;)

@jon-liionwholesale That pretty much confirms what we've seen in past discharge tests comparing the 30Q and HG2. Even with the lower rating of the 30Q it consistently outperformed the HG2 in voltage sag and at a lower price!
```

---
## \#37 Posted by: jrpwit Posted at: 2017-07-14T08:33:51.423Z Reads: 180

```
Wow thanks for this info! I always went with hg2 before.

One question. Why is the 30q rated at 15A if it can do 20A comfortably?
```

---
## \#38 Posted by: jon-liionwholesale Posted at: 2017-07-14T13:18:30.910Z Reads: 189

```
Discharge ratings are up to the discretion of the manufacturer.  On this one LG just decided to be more aggressive than Samsung did, that's all.
```

---
## \#39 Posted by: chsknight Posted at: 2017-07-14T18:26:37.013Z Reads: 196

```
Do you have any data on the actual difference between the old HG2's and the new or is this just observation?
```

---
## \#40 Posted by: jon-liionwholesale Posted at: 2017-07-14T21:27:21.734Z Reads: 204

```
Yes, I have data supporting it.  I'll put that on the list for potential blog posts in the future but it would be a lot of effort to put it together and publish.
```

---
## \#41 Posted by: Mathias Posted at: 2017-10-20T19:51:30.779Z Reads: 177

```
I finally had time to build the board! The only thing I changed from my plan was to go with Trampa Stickies instead of cheap flywheel clones. 
<img src="/uploads/db1493/original/3X/2/7/277c6cce19da318c98948cebcefba634a1e40c42.jpg" width="690" height="208">
<img src="/uploads/db1493/original/3X/8/2/82f2dd18f49a68b5658baba9056cec92d8cbd220.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/2/5/251150910384aef88e335a8b754ce733a3384c5e.jpg" width="245" height="499">

First test rides went fine with one exception: although I filed the hanger round the mount just wouldn't stay in place, no matter how tight it was. So I got some [Steel Epoxy](https://www.amazon.com/gp/product/B014OVHAOY/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1) and glued the APS truck adapter. 
<img src="/uploads/db1493/original/3X/9/4/94b3be598d871e6e59ccabceea75e1fa9403b405.jpg" width="374" height="500">
```

---
## \#42 Posted by: Rinzler Posted at: 2017-10-20T19:55:32.954Z Reads: 168

```
[quote="Mathias, post:41, topic:24295"]
I finally had time to build the board! The only thing I changed from my plan was to go with Trampa Stickies instead of cheap flywheel clones.
[/quote]

Arent trampa Stickies just a flywheel clone with a fancy name, with a higher pricetag ?
They certainly look like they are.
```

---
## \#43 Posted by: Mathias Posted at: 2017-10-20T20:00:37.288Z Reads: 165

```
[quote="Rinzler, post:42, topic:24295"]
Arent trampa Stickies just a flywheel clone with a fancy name, with a higher pricetag ?
They certainly look like they are.
[/quote]

Well, first of all they ride really well, and I haven't tried those cheap clones but the bad reviews made me change my mind. And second, they had an offer when bought with ceramic bearings: ~90 GBP for both is not actually that expensive.
```

---
## \#44 Posted by: Rinzler Posted at: 2017-10-20T20:05:14.134Z Reads: 156

```
If you like them then i guess they are good, what duro are they ?
```

---
## \#45 Posted by: Mathias Posted at: 2017-10-20T20:12:01.671Z Reads: 158

```
76a. It's super soft, but the roads around my place are ridiculously bad. I'm so glad I have the soft wheels and the flexy deck!
```

---
## \#46 Posted by: Mathias Posted at: 2017-12-12T00:59:44.307Z Reads: 139

```
After a few hundred km on the board: it's really awesome! I live in Berkeley and was worried about plenty of things: 

Terribly rough roads: I got to say the flexy deck and the soft wheels pay off. On top of that I added shock pads, and now it's OK. By now I know the area well enough to avoid the worst of the worst. One of the worst is unfortunately the road to my apartment...

Then there is tons of stop and go (millions of students crossing everywhere, tons of 4-way-stop-sign-crossings. Seriously, California, why do you do this??? As a German this annoys the crap out of me!). But the brakes are plenty strong and on average I recover about 25%  of the energy, which is way more than I hoped for!

Another thing is the REALLY steep terrain around here. I'm glad I didn't cheap out on the motors, and that I went with the wide belts! Yesterday I put it to the test and rode up Grizzly Peak:
<img src="/uploads/db1493/original/3X/9/4/941f2db2a457e8b09e437bb66b548d3bebd2af98.png" width="281" height="500"><img src="/uploads/db1493/original/3X/9/c/9cdc4cd3f33e1d7dd20f9a9d714e8540ac17c3e4.png" width="281" height="500"><img src="/uploads/db1493/original/3X/5/1/51c048ecb703906a98582fa5efec0684d18aa714.jpg" width="281" height="500">
and it was a cake walk for the board! The only things slowing me down were traffic and the road quality! (Awesome route by the way! If someone lives nearby, go through Tilden Park!). 

On average I ride at 9.3 Wh/km (15 Wh/mile). Even though I didn't ride the board super fast so far, I think this way better than what most people get, especially considering that I ride in constant stop and go and on rough, steep roads! I guess this is thanks to: big motors, (fairly) low KV/high gear reduction, and super loose belts! I'm glad I went with the 15 mm belts. They are floppy as hell, and my board rolls so nicely, I could easily push it (not that I ever ran out of battery). And I've never had them skip! Even the killer steep climb above I had an average of 11 Wh/km!

So conclusion: I'm glad I read up on ESkates on this forum before I bought some crap on ebay (which I was seriously considering at the beginning). And thanks to everyone on this forum for sharing their experience!
```

---
