# The Anubis &#124; Laying It Down Low &#124; Hummies V4 Hub Motor Drivetrain &#124; 30Q 18650 10s4p &#124; Dual Focboxes in FOC &#124; eBoosted Custom Vanguard Enclosure &#124; Arduino Firefly Remote &#124;

### Replies: 58 Views: 5379

## \#1 Posted by: Jc06505n Posted at: 2018-02-25T02:47:00.420Z Reads: 555

```
If you like hardwork and hate lazy fuckers, lol you're going to hate me.

So the tale of this build is going to be a bit different than most. It's both a semi-DIY build and an experiment. 

The experiment: How long can I stay a lazy motherfucker. You'll see what I mean by the end of the Build Log. I'm nowhere near having this build completed, but I'm hoping that posting early, you guys can help and recommend better parts and stuff

Build List and pricing are at the bottom. 

**Deck Wise** I'm running with the [Laying it Down Low](http://www.customskateboards.com/Blank-Laying-It-Down-Longboard) (LIDL) deck from CustomSkateboards.com. I've ordered 2 decks LIDL decks from them (one coated and one uncoated) with the uncoated deck being sent to @treenutter for it to be painted in [Blackout Black](https://www.instagram.com/p/BXRKE65j6ea/?taken-by=redemberboards). That should take two months min with manufacturing, shipping, and paint time. Thank you again @treenutter! The Flex on this board is real! 

![image|500x500](upload://ptSVfmNft8fsgyt7R0hLSV5tNBN.jpeg)

**Drive Wise** I'm going to be running [Hummies V4](http://www.electric-skateboard.builders/t/new-hummie-hubs/25251) which come with a [Paris V2 195mm 50° Longboard Skateboard Truck](https://www.amazon.com/Paris-195mm-Longboard-Skateboard-Trucks/dp/B076B35C5Y) with custom 12mm axels, two tires and, two [ABEC 11 Centrax Wheels](http://www.abec11.com/products/abec11/abec-11-77mm-centrax-77a-80a-83mm-centrax-77a-80a). Since I'm trying to achieve a Gold-Black-White Anubis Theme, I'll be substituting the ABEC wheels for [Build Kit Board's 78a Premium Build Wheels 97mm Black Wheels](https://buildkitboards.com/collections/wheels/products/90mm-build-wheels?variant=5041515135006). I'm in desperate need of good quality & preforming Black-Gold Bearings so if you have any suggestions or solutions, **please share!** I'm also thinking of swapping out the Paris V2 195mm for [Paris V2 180mm Matte Black & Gold](https://www.tactics.com/paris/v2-50-degree-longboard-trucks/black-matte-180mm). Any differences between the 190mm and the 180mm? 

https://cdn.shopify.com/s/files/1/1320/9269/products/Paris_Trucks_195-50-black_720x.jpg?v=1487984928

![image|500x500](upload://wUyYfzD1IOd4emYfCg2457gUxD7.jpg)

http://www.abec11.com/wp-content/uploads/2016/07/Abec11_83mm_Centrax_80aLRG1.jpg

https://cdn.shopify.com/s/files/1/1929/9189/products/IMG_0814_large.JPG?v=1508003485

**VESC,  Battery, & Enclosure Wise**

 I'm running [Dual FocBoxes](http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/) bought from @JdogAwesome, the same one used in the [Enertion FOCBOX Teardown & Internals](http://www.electric-skateboard.builders/t/enertion-focbox-teardown-internals/42633) so it has MG Chemicals Acrylic Conformal Coating. They originally had 3.5mm bullet connectors with 4mm Bullet Adaptors attached, but I opted out and commissioned @longhairedboy to swap out the 3.5mm connectors for 5.5mm Bullet Connectors. This is great since I can request @Hummie to do 10awg with 5.5 Bullet Plugs for motor wires. I also commissioned @longhairedboy to directly solder on CANBUS cables to the FOCBOXES for maximum security. No wires coming off today. Hopefully. I'm going to be running 18650 10S4P Samsung 30Q 18650 3000mAh 15A Battery Cells. The Pack will be custom made by @psychotiller. The FOCBOXES, along with any associated cables & accessories, will be housed by @Eboosted's  [Custom Vanguard Fiberglass Enclosures](http://www.electric-skateboard.builders/t/eboosted-enclosures-thread/38073). In addition to the battery pack, the Battery Enclosure will be outfitted with an LCD, BMS. Antispark Switch and USB port. The VESC Enclosure will be outfitted with Grommet Holes based on @Deckoz's [VESC Enclosure](http://www.electric-skateboard.builders/uploads/db1493/original/3X/a/f/af17d2850d2a65b2168a28711f99f22924565273.jpg) (I think it's the best for modularity purposes) for Motor wires/Cable Riser wires, all by @psychotiller who's also agreed to do wire routing. 

![19be9a8aec92c43d351a5ccbfa4737c800c92085_1_690x459|690x459](upload://qY676UKbiSyC5ZBMj0qyY8ffmsr.jpg)

**Telemetry Wise** I'm using @rpasichnyk's [METR HM-10 Bluetooth Module](METR.at) since it basically gives me access to all telemetry-display apps available. I was going to originally use @GrecoMan's modules, but I've decided to save them for potential later builds. 

**Remote Wise** I'm having a Red and Black (since that was originally the Color theme of the board, too late to change colors now) [Arduino Firefly Remote](http://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543). I've commissioned @SeeTheBridges to assemble the remote and components. Right now he's in the midst of finding a way to make the Arduino receiver plug and play (I bug him about it cause I'm a lazy bastard), as well as being able to update the Arduino via the USB port for future updates. 

![image|375x500](upload://ksIXxbIhMjBx8zEjPL6rSykWEZT.jpeg)

**Additional Shit Wise** Additionally, I'm going to be using [UNIK Switchblade E-Cable Risers with 30cm Cable Wires](https://www.unikboards.com/en/boutique/riser-pad/) (Yes I know, I could've 3D Printed it, soldered the cable wires on, and saved a hell of a lot of money, but I'm a very lazy bastard). The cable wires should help make the board look clean and sleekier. 



I'm thinking of adding a Tile Pad or equivalent in the VESC enclosure just for added security measure. Won't do much, but nice to have. 

**Build Log**

* Laying It Down Low Blank Uncoated Deck + @treenutter Paintjob : **$160**
* Hummies V4 + Trucks & Paris V2 195mm 50° Longboard Skateboard Truck + ABEC 11 Centrax Wheels: **$460**
* Dual Enertion FocBoxes + @longhairedboy Upgrade **$316.91**
*Ardunio Firefly Remote **$100**
* Ollin CANBUS cable **$9.95**
* eBoosted Vanguard Enclosure + Hardware Bolt Kit + Enclosure Rubber Gaskets **$196.70**
* 10S5P Samsung 30Q Battery Pack + LCD, BMS. Antispark a Switch, Charger, and USB port + Enclosure Outfitting + routing + Assembly (all by @psychotiller cause he's a champ) **$650-$700**
*  METR HM-10 Bluetooth Module **$33.95**
* 2 @GrecoMan Bluetooth Module **$34.29**
* UNiK Switchblade E-Cable Riser **$72.39** (This one made me cry the most)
* Build Kit Board's 78a Premium Build Wheels 97mm Black Wheels **$53.94**
* Paris V2 180mm Matte Black & Gold **$24.95**
* Clear Red 83mm Metro board Wheels (Cause fuck me) **$97**


**Unaccounted Pricing**

* [Black & Gold Bearings](https://www.muirskate.com/longboard/bearings/55931/holesom-holy-roller-built-in-bearings)

https://www.muirskate.com/photos/products/4708/hd_product_Holesom-Holy-Roller-Bearings-%28Set-HD%29.png

* Tile Bluetooth Tracker **$30.14**
* The Blackest Grip Tape Possible

**Maybe Items**
* [Custom Grip Tape](http://www.customskateboards.com/custom-grip-tape-printing)

**Cost so far: $2,290.22**

Fuck.Me. I've been avoiding the numbers since I bought the Hummies. For that price, I could've ordered the Deck and commissioned LongHairedBoy to build something. Or even get a Custom Kaly-board but I'm in too deep now! A Good $500 comes from my laziness and spending mistakes (about $50 is not being counted). I intend to sell the Paris V2 195mm 50° Longboard Skateboard Truck, ABEC 11 Centrax Wheels, 83mm Red Clear Wheels (if not refund it), and even the Bluetooth Modules if anyone wants. Hit me up if interested. This build is a nice experiment to see how much it would cost to commission the "DIY" part with the additional insight with what products we're lacking over here in the states.

Let me know your thoughts (please be gentle) and I'll keep you guys updated on this outrageously priced build!
```

---
## \#2 Posted by: mmaner Posted at: 2018-02-25T03:07:04.016Z Reads: 445

```
Normally I dog on people for not putting in the work, but this made me laugh. I'll by you a beer if we ever meat, you lazy bastard 😀
```

---
## \#3 Posted by: Eboosted Posted at: 2018-02-25T03:08:52.957Z Reads: 437

```
We need pictures!!!

Man you really did nothing on your own!!!! :sweat_smile:
```

---
## \#4 Posted by: Jc06505n Posted at: 2018-02-25T03:15:04.315Z Reads: 432

```
I'll pay you for the beer delivery. :wink: 

Though I do regret a sum of this build due to my indecisive and impulsive nature. A lot could've been saved, even with my laziness. Much more research could've been done to avoid the uneeded cost. 

But it's a good experiment nonetheless for the lazy. Hopefully, something beautiful comes out of this abomination.

Edit: Also this was done on a 95% disposable income. Wanted to see the results. After this build (or the next one cause there's something I really want to make). I'm locking down.
```

---
## \#5 Posted by: ATLesk8 Posted at: 2018-02-25T03:18:14.507Z Reads: 382

```
Dude this is going to be a sweet ass build and totally not lazy to put it together. It's surely going to be worth it, however I'd go 12s4p but potato potato
```

---
## \#6 Posted by: Jc06505n Posted at: 2018-02-25T03:20:20.806Z Reads: 376

```
Pictures will come soon. The deck I showed you before is going towards a DIYEboard (yes I wasted even more money, I know I know, fuck me). 

The first array of pictures will come from Treenutter during his paint job. 

If you ever end up making Vanguard Enclosure with Fins, I'll probably upgrade.
```

---
## \#7 Posted by: Jc06505n Posted at: 2018-02-25T03:25:26.434Z Reads: 365

```
I feel like Specs/Price, It's a bit (a lot) underpowered, (though the only thing holding such back is the enclosure size which can easily be fixed by order the 12s Vanguard Case). 

The reason I avoided 12s though is the unreliability of it not breaking the Focboxes down. 10s is safer and has shown that it works, so I opted for 10s (which gives me the mileage I want).

Some people would ask why I didn't opt for a Raptor 2 or Trampa, I don't like the deck or either board, and I didn't want a Boosted. I wanted a shape of a very specific deck, enclosure and look that didn't compromise my laziness and this was the result :cry: . I really hope it comes out looking like a sleek motherfucker.
```

---
## \#8 Posted by: pixelsilva Posted at: 2018-02-25T03:28:01.714Z Reads: 340

```
.... therefore, in the Year of the Lord twenty eighteen thu should name thee build as: **Lazy Board**

All members of the guild, repeat with my: Aaaaaa-meennnnn!
```

---
## \#9 Posted by: Jc06505n Posted at: 2018-02-25T03:33:37.918Z Reads: 335

```
I would hate it, but one of my favorite DBS characters Beerus is basically an Anubis that Sleeps all the time, I'll take it! 

Does That mean I can get a "Lazy sonofabitch" Tag :grinning: ?
```

---
## \#10 Posted by: ATLesk8 Posted at: 2018-02-25T04:28:47.275Z Reads: 338

```
Oh dude 10s will be more than enough honestly my 10s boards are too quick so now I've converted to controllers with slow mode (it also saves an unbelievable amount of battery). No joke i get almost 50% more battery life in slow mode which is more than suitable for 90% of riding around unless you want to do a speed run i guess. 30mph is more than fast enough for most riders most of the time. I'd much rather have the super torquey take of to smoke the other group riders up the hills
```

---
## \#11 Posted by: Jc06505n Posted at: 2018-02-25T04:41:13.747Z Reads: 332

```
Hopefully, someone comes up with a way to program slow modes on the Arduino remotes , I barely ride fast , but would still like to have it just for special occasions (ESK8Con 2018 😉)
```

---
## \#12 Posted by: ATLesk8 Posted at: 2018-02-25T04:49:29.116Z Reads: 368

```
So currently my fav remote is my benchwheel. I had always use the mini but i hate swapping rechargable batteries all the time and a few of my boards have usbs on them so worst case i can stop for a sec and charge the remote off the board battery. I also no have a nano x for my spud (has very little room for throttle or braking response or a short throw and pull if that makes more sense), and a new maytech (close second favorite) which all charge usb and have slow modes built in that are great! My last remote i haven't used yet is a mastercho gt2b that i built
```

---
## \#13 Posted by: Jreamer Posted at: 2018-02-25T04:50:25.725Z Reads: 386

```
I would consider not switching to the 180mm paris trucks from the 195. The hub motors will stick out farther than the wheels up front creating kind of a dragster look. 
I run this board with 180's and 195's but have it set up as a front wheel drive.
![IMG_0402|333x500](upload://upqTjyjip6vQKgC0Yj7PgZUFlI3.JPG)
```

---
## \#14 Posted by: Eboosted Posted at: 2018-02-25T05:01:17.700Z Reads: 368

```
I use 12S FOC on dual focboxes on all my boards, I won't ever go back to BLDC or 10S. 12S is the king and it's reliable
```

---
## \#15 Posted by: Jc06505n Posted at: 2018-02-25T05:01:40.901Z Reads: 351

```
Fuck. That sucks. Why can't Paris have more color options for the 195mm Series :cry:
```

---
## \#16 Posted by: Jc06505n Posted at: 2018-02-25T05:11:27.193Z Reads: 345

```
I see, even then the last thing i want to do is push my focboxes to the absolute limit. I rather have it working comfortable fine at 10s with specs that's enough for me.
```

---
## \#17 Posted by: Jreamer Posted at: 2018-02-25T05:13:13.501Z Reads: 348

```
You could switch out the base plate. The hanger will still be black though.
```

---
## \#18 Posted by: ATLesk8 Posted at: 2018-02-25T05:14:09.099Z Reads: 348

```
Just paint them any color yourself. I've had pretty good luck painting trucks
```

---
## \#19 Posted by: Jc06505n Posted at: 2018-02-25T05:15:24.706Z Reads: 345

```
Lol 

[quote="ATLesk8, post:18, topic:47391"]
Just paint them any color yourself
[/quote]

@ATLesk8, you already know the second name of this board.
```

---
## \#20 Posted by: pat.speed Posted at: 2018-02-25T05:17:43.150Z Reads: 332

```
Lol just pay @Hummie extra to paint them for you
```

---
## \#21 Posted by: Jc06505n Posted at: 2018-02-25T05:20:25.069Z Reads: 291

```
I would, but the last thing I'm going to do is give that man more work than he already has. At least for right now. 

And there's not much difference between the 195mm and 180mm that I think, only the Bushings are different. Maybe I'll just get gold colored bushings and call it a day.
```

---
## \#22 Posted by: Exiledd_Top Posted at: 2018-02-25T05:20:54.650Z Reads: 288

```
I can relate to all the not wanting to look at the cost on my 4wd carvon drive build 😂😭 battery alone cost me 1k 12s6p 30q bypassed and 2 carvons drives 1k aswell  to a total of past 3k $ and I have everything but the carvon drives should be in By next week
```

---
## \#23 Posted by: Jc06505n Posted at: 2018-02-25T05:23:20.474Z Reads: 304

```
Holy Fuck 3K? 

What the bloody hell going to be your specs man? 

The one thing I'm worried about my build is weight. I'm going to be carrying this thing, and I would hate if it ends up weighing more than 17lbs
```

---
## \#25 Posted by: Jc06505n Posted at: 2018-02-25T05:30:55.154Z Reads: 294

```
Bizzare Idea: If I bought the 180mm, could I swap out all of the gold parts on that truck to the 190s?
```

---
## \#26 Posted by: Exiledd_Top Posted at: 2018-02-25T05:35:56.315Z Reads: 291

```
My battery alone wiegh 12 pounds LOL 
It's 4wd carvon Xl drives 4 focbox's and 12s6p 30q BMS bypassed,landyatch evo with 107's abec wheels, I estimate it to be around 30-35 pounds
```

---
## \#27 Posted by: pat.speed Posted at: 2018-02-25T05:38:40.748Z Reads: 292

```
You wanna know the good thing?

At least your battery is big enough that you will never have to carry it🤣
```

---
## \#28 Posted by: ATLesk8 Posted at: 2018-02-25T05:39:57.786Z Reads: 309

```
I mean a good 12s5p 30q 60amp bms pack with switch and charger are going for $600-700 or so I've seen. Plus $150 per focbox . Thats $1.3K without the drivetrain or anything else. And then 2 carvons is another grand. So we're at $2.3K. Deck lets say $120 (price of sweet hummie deck). Enclosure $65. $140 for 107s. $30 for bearings. $50 for remote. That's about $2725 i think
```

---
## \#29 Posted by: Jreamer Posted at: 2018-02-25T05:42:27.408Z Reads: 296

```
Yes you can
```

---
## \#30 Posted by: Exiledd_Top Posted at: 2018-02-25T05:42:31.266Z Reads: 291

```
Mine is 12s6p but dimensions for the landytach evo I always go BMS bypassed 4 motors there is no BMS that is not bypassed that would fit XD
```

---
## \#31 Posted by: Jc06505n Posted at: 2018-02-25T05:44:13.632Z Reads: 288

```
Danm, that thing is going to be a beast. If ESK8con ever happens, I want to see you and your crazy board there.
```

---
## \#32 Posted by: Jc06505n Posted at: 2018-02-25T05:45:11.378Z Reads: 284

```
Lol he can always cheap out and get Zealous bearings.
```

---
## \#33 Posted by: Jc06505n Posted at: 2018-02-25T05:47:30.196Z Reads: 301

```
Bet. that's most likely what I'm ganna do. Guess I'm going to have to sell an impure 180mm Paris Truck

Aw fuck, I'm going to need to If I'm going to swap out the Hub motor's trucks components, can I even do that? I also wonder how open @Hummie is to having the cover gold-color :sweat_smile:
```

---
## \#34 Posted by: Exiledd_Top Posted at: 2018-02-25T05:48:51.915Z Reads: 321

```
![20180224_214610|374x500](upload://jXSU11O84h0qLgVrv7mVpUSmort.jpg)![20180224_214652|666x500](upload://77vvqxVn15wnjb0ok3mHvFluRpF.jpg)![20180224_214711|666x500](upload://uE6N3zs9vOfkslHDKmQgUmkac40.jpg)! 
My battery if very thick and heavy and so is my enclosure
```

---
## \#35 Posted by: Exiledd_Top Posted at: 2018-02-25T05:52:32.400Z Reads: 314

```
Am copying Derek's build but the difference is that he was using 25r with 15 amps compared to my 30q 20 amps and he was using speed r and am using xl but I should hit 35mph easily. Also it would have bin cheaper going 25r by 400$ and speed r by another 200$
http://esk8builds.com/photo/view/?id=89
```

---
## \#36 Posted by: E1Allen Posted at: 2018-02-25T06:00:01.194Z Reads: 296

```
No mention of who is putting everything together on the board for you???
```

---
## \#37 Posted by: Exiledd_Top Posted at: 2018-02-25T06:01:58.524Z Reads: 296

```
If your referring to me, I am putting it together. I already bought 10awg wire and solderd the cables to make it fit and changed the xt60 focbox to xt90 rip warranty
```

---
## \#38 Posted by: ATLesk8 Posted at: 2018-02-25T06:40:42.657Z Reads: 292

```
I love zealous bearings no joke...i use the built ins in all my boards. Best cheap built in bearings I've found. The muirskate brand ones are good and cheap to imho
```

---
## \#39 Posted by: Jc06505n Posted at: 2018-02-25T06:53:30.858Z Reads: 298

```
I would get Zealous bearings ,  But for cosmetic purposes , I need Gold-Black Bearings.
```

---
## \#40 Posted by: Jc06505n Posted at: 2018-02-25T16:17:41.365Z Reads: 290

```
Boys I think we found our [Bearings](http://www.holesom.com/product-page/holy-roller-bearings)

![image|498x498](upload://fHWkjyTnxARKraqVBW1urP7YS4V.jpeg)
```

---
## \#41 Posted by: Jc06505n Posted at: 2018-02-25T19:53:33.721Z Reads: 282

```
Crazy idea: Can i run different mm wheels in the front? Like say 97mm on the front and 83 on the back :grinning:
```

---
## \#42 Posted by: GrecoMan Posted at: 2018-02-25T20:24:24.976Z Reads: 253

```
why the hell would you want to do that 🤣
```

---
## \#43 Posted by: Jc06505n Posted at: 2018-02-25T20:34:58.138Z Reads: 267

```
For science! 

.


.



.

Because Hummies are 83mm I believe but I want big wheels :frowning: . I suppose I could ask for 80KV and just get 83mm black wheels (if i can find them in a soft Duro). Should provide me with decent Tourque with a great top speed.
```

---
## \#44 Posted by: Jc06505n Posted at: 2018-02-25T20:45:46.107Z Reads: 270

```
*Sees @trampa 83mm 76a Black Stickies Wheels*

*Sees Shipping Prices*

*nopes the fuckout*

*Goes to ebay and every online e-boarding group looking for third party sales.*
```

---
## \#45 Posted by: Jc06505n Posted at: 2018-02-28T00:32:04.731Z Reads: 267

```
The UNiK Switchblade Cable Risers came 😀! 

![image|375x500](upload://1QfHlEjJApGDKS2HqliOtYUdM0B.jpeg)

![image|375x500](upload://o0UolREYlEa5mAEGOryCOatQgfk.jpeg)


Oh how the Gods test me... 

![image|375x500](upload://l9n2KGnZpDc3OoWxpnifKpcnFNx.jpeg)

FUCK
```

---
## \#46 Posted by: Bensaida Posted at: 2018-02-28T15:49:40.711Z Reads: 251

```
Solder time 😝
```

---
## \#47 Posted by: Jc06505n Posted at: 2018-03-02T03:59:52.598Z Reads: 263

```
[quote="Bensaida, post:46, topic:47391"]
Solder time :stuck_out_tongue_closed_eyes:
[/quote]

Dub 😃. 
 
**Will edit later for spelling, grammar, names, and pictures but for now:**

**Update**: Got a few things rolling along: 

* Contacted Paris Trucks and was able to order 195mm Trucks with Gold Components. Have them almost en route to Hummies to use for my motors. 

Edit: The sent regular trucks with gold components. Maybe for the best since I didn't realize that the Paris Trucks have custom axels for hummies.

* Ordered some Neoprene for padding and to place between the enclosures components and deck. Do you guys recommend making small holes or a cut out for the VESC for heat purposes 🤔? Ganna have to get another Exacto knife. 

* Also ordered a Gold and white Tile Pro for shits and giggles, I was under the assumption that they had an abrasive back to stick in surfaces (have no idea why. Have to find a comfortable place to put them in one of the enclosures. Don’t want them somehow messing anything up by ratting all free everywhere.

![image|375x500](upload://pvG359ZWp74NKvEZNuBf4cVn5sa.jpeg)![image|375x500](upload://rlaTdLwCL5UBGzFRpMMla5vKFMx.jpeg)![image|375x500](upload://cM6bsi3bXuJuxP0jO76APfLzz3P.jpeg)

* Just got a tracking number from CustomSkateboards, Way faster than last time and the estimated production time. A really good reliable source for decks in times when Chinese Manufactures shut down. Going to try to reroute the package to @treenutter if possible. Please don’t let me down UPS.  

* Just got the [97mm 78a Black Wheels](https://buildkitboards.com/collections/wheels/products/90mm-build-wheels?variant=5041515102238) from @JLabs . When I first got my Meepo It has a smell I couldn’t identify. With these wheels, I realized It was the smell of Polyurethane. They bounce nice but I’m not an expert so I can’t really judge them. I’ll be using these wheels in the event that @Hummie  ever release a 97mm PU.

![image|666x500](upload://l83zarY2XKIDOQD242XR50bP4tH.jpeg)![image|666x500](upload://grQq23q0L60coTei32gJv8CZNpq.jpeg)

* I’ll have to find someone in NYC who’ll be able to solder on 5.5mm Bullet Plugs onto the UNiK cable riser wires.  

![943cda9607e522178e15ae7ee1253241de1b3d8b_1_375x500|375x500](upload://gCny7DNxszwHqtQazU4f2J58KpJ.jpeg)

* In the meantime I’ll be trying to design some Aluminium metal plates for the vanguard enclosures to act as washers. Going to be a real pain in the ass. 

* One of the focal points of this build is semi- modularity. The ability to change drive trains is what I want to achieve in the end game. Following @Deckoz design choice with the gasket holes VESC Enclosure, swapping drivetrains should be just unscrewing trucks, unplugging Wires, screwing back in, plugging back in, and Configurement detection/setup. 

Edit: It seems that’s totally possible with the perimetr app! Even wireless detection could be done! 


* Would I have to plug my Focboxes in to configure every time I swap drive trains or could I use one of the mobile VESC Bluetooth applications modes feature to achieve the same effect? I’m thinking one mode, in say the METR counterpart app, would be for Hummies Hub Drives while another mode would be for Belt Drive. Can anyone please critique this idea and tell me if it’s possible or the probably faults? 

* Lastly: What is the ultimate Belt Drive set up? (Not talking in terms of batteries or board and what not, but only drivetrain and components)

Edit: The answer for the Anubis ? 6374 190 KV Dark Matter 2:1 Gear Ratio. While I might be running 83mm wheels, I can always upgrade in the future!


TL;DR: Got a sum of materials (Neoprene, Tile Tracker), with a few Enroute for adjusting ( Custom Paris Trucks, Deck) and need Idea critiquing and a question of the ultimate belt drive component.

Edit: Grammar & Spelling
```

---
## \#48 Posted by: Bensaida Posted at: 2018-03-02T06:23:07.158Z Reads: 226

```
You would need to plug in to do motor detection.
```

---
## \#49 Posted by: Jc06505n Posted at: 2018-03-02T06:27:34.718Z Reads: 252

```
After a few mins of poking and asking [It seems Perimetr allows for Wireless Motor Detection](http://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483/50?u=jc06505n)

![image|281x500](upload://cC6oArkAd9H33QuHxjcjfSCPZIW.jpg)
```

---
## \#50 Posted by: GrecoMan Posted at: 2018-03-02T12:00:47.024Z Reads: 227

```
@scepterr is in NYC 😉
```

---
## \#51 Posted by: Jc06505n Posted at: 2018-03-02T12:41:26.076Z Reads: 240

```
Oh trust me , my man waaaaaay ahead of you 😉.
```

---
## \#52 Posted by: Jc06505n Posted at: 2018-03-07T22:14:59.867Z Reads: 269

```
**Update**: 

Still have to polish that last update up but: 

Contacted @scepterr  to see if I could commission him to build a Belt Drive Train for the Anubis. He said yes :smiley: . The belt drive is going to be using a [218mm Tourqueboard](collections/longboard-trucks/products/torqueboards-218mm-trucks) Caliber Clone with a Caliber II Baseplate. I'll also be swapping out the pivot cup for [WFB 96a Pivot Cups](http://www.riptidesports.com/wfb-96a-pivot-cup-choices/) the bushings for [KranK Canons 84a](http://www.riptidesports.com/krank-canon-duro-choices/) and [KranK Magnums 84a](http://www.riptidesports.com/krank-magnum-duro-choices/) that were recommended from @Alphamail. (Thank you man!) 

http://www.riptidesports.com/wfb-96a-pivot-cup-choices/
http://www.riptidesports.com/krank-canon-duro-choices/
http://www.riptidesports.com/krank-magnum-duro-choices/

Since one of the goals for the Anubis was semi-modularity, my goal is to switch only the rear trucks (which I’ll refer to as Drive Train Trucks) and leaving the front 195mm Paris V2 trucks on. That means that if I’m going to run Belt Drive, I’ll have two different types of kingpin 50-degree trucks on one board. What can go wrong? :smiley:

In terms of motors, the belt drive will be using Dual [6374 190 KV Dark Matter Motors](http://www.electric-skateboard.builders/t/limited-edition-6374-190kv-sensored-dark-matter-motor-for-sale/44200/1). Due to the wheels I’m using being 83mm  ( because the front trucks and Hummies PU are 83mm), the belt will run in a 15-30 configuration as an attempt to lessen the torque and have more control running 83mm. The wheel pulleys and motor mounts will be from @marcmt88. 

http://www.electric-skateboard.builders/t/limited-edition-6374-190kv-sensored-dark-matter-motor-for-sale/44200

http://www.electric-skateboard.builders/t/motor-mount-with-dual-idlers/35183

http://www.electric-skateboard.builders/t/customized-pom-htd5m-pulleys-for-abec-kegel-evolve-gt-mbs-100-abec-clones/46612

Sent my Focboxes to LHB and I received them a few days ago, he put some 5.5mm bullets as well as soldered on Canbus cables between the VESC’s.  

![A1F46810-A051-45D2-97B4-505F01CF817F|603x500](upload://n0kyaRm0Bs3FsU3BWhoGQy5inHN.jpeg)

Also ordered some Rubber Gaskets from @Eboosted cause I'm a lazy bastard. Once this snowstorm clears up I'll be able to go to work where I can cut some adhesive Neoprene foam for enclosure padding!  

![0597f95c720a6d27d41e8f17ea18623f9c7f85bf_1_281x500|281x500](upload://tjR8hEyzEILDtPysQI5opYRjoRv.jpg)

**Update Edit: **

Bearings came ! 

![image|666x500](upload://yLYUAs3LAdb2l2JoIn56JH4g06Q.jpeg)
```

---
## \#53 Posted by: Jc06505n Posted at: 2018-03-22T04:38:13.000Z Reads: 250

```
Oh, I think you guys are going to like this.:

Before:

![image|500x500](upload://nCIw1Syu7Yl63cyXVAvz8pEajRB.jpeg)

**After:** 

![image|500x500](upload://oBTxTeYCdzPEG6aGDJYjXaeJJAB.jpeg)

All done by @treenutter 

The deck came uncoated (as intended) with one end a bit nudged up as you guys can see here: 

![image|500x500](upload://eog4Q9T0LZ5ymTMk5rINM8SmzTQ.jpeg)![image|500x500](upload://3sQS90HJirYBpVg3hB82llLfbAt.jpeg)

Treenutter being the G that he is fixed that right up and even countersunk the truck mounting holes.

![image|500x500](upload://qxaIvvhSKyBMaV7WukO5BdhuPOu.jpeg)![image|500x500](upload://36VRuVLDwlxacOpAyBKBjgpm56A.jpeg)

He 

> Sanded w 150 then 220. Rounded over that dinged point we a bladder sanded then polished it. Countersunk the holes. Wiped clean to pre-raise the grain. Then a sand w 400 to prep for coloring.

After staining, he let it dry overnight. 

![image|500x500](upload://gveqmhQdonj5gWKRSLr10iQ7dJN.jpeg)

> It dried nicely! At this point, the stain is fragile so I wear gloves while handling it. Any moisture or oil will ruin the coloring.The next step will be to start laying down clear coats. It looks very matte now, but it will darken and have more of a gloss once I spray it...  Blackout [black] takes extra care to blend the edges the top and bottom. End -grain absorbs more color so I have to prime (by sanding edges at s higher grit) to get it as even as even as possible. Painting these with spraypaint would make it a lot easier but then you don’t get to see the wood patterns. Staining is one of the ways I differentiate myself from factory decks and large manufacturers


And that’s not even half of what treenutter can do. If you’re looking for a killer deck that’s designed and created carefully,l and beautifully [I really recommend checking out treenutters decks! ](https://www.instagram.com/redemberboards/?hl=en)

https://www.instagram.com/redemberboards/?hl=en
```

---
## \#54 Posted by: Eboosted Posted at: 2018-03-25T18:23:33.518Z Reads: 205

```
Beautiful deck man! I haven't seen anything like this before, I wonder if it has an aggressive concave. 

Try to increase the wheelbase as much as you can, it always looks better
```

---
## \#55 Posted by: Jc06505n Posted at: 2018-03-25T19:26:16.667Z Reads: 224

```
Thanks man , it’s really all of @treenutter’s work that’s making it so beautiful. It looks like he’s almost close to finishing up the deck so you’ll see the finish version soon. 

I was thinking of giving the Encolsures I got from you the same treatment but decided against it as I’m a lazy bum 😃. In all seriousness I’ll have to see first before doing anything. I ordered some Gold Hardeware from @Money, just waiting on restock. Planning on dying some ABEC Centrax Wheels Black with gold nuts on the axels. 

In terms on concave it has a taco concave, with th rubber gasket and neoprene, your enclosure fits perfectly on it here’s how your Encolsures fits on the same kind of deck: 

![image|375x500](upload://gvn0D34vcRmA4n71F7eyDexjg1d.jpeg)![image|375x500](upload://iDfqLt8myWJwduAAZQkFo8GT6Ps.jpeg)![image|375x500](upload://nFRIAjktk5PN2LeEV6S2JWr8D4.jpeg)

Do you think the wheel base is too short? ![image|666x500](upload://Al2ijhYbu58oZ3FOnguaJ47wxfP.jpeg)
```

---
## \#56 Posted by: Jc06505n Posted at: 2018-03-25T19:54:50.680Z Reads: 218

```
Also a little Drive Train Comparison between the Anubis on Hummies and the Anubis on Dark Matter: 

Hummies: ![image|281x500](upload://8GVfcyYChAB0FkhYd1ja28gnzIL.jpg)

Dark Matter: ![image|281x500](upload://96wdjJGVG2iSF9ZsAKn1S8XMOEb.jpg)

Nearly identical specs with Belts pulling in more top speed. Still tying to see if swappability is worth it. If not I might put the Dark Matter on another build. 

Got some rubber gaskets, Velcro, and waterproof switch covers from Eskating.eu: 

![image|666x500](upload://ei1MAwq1v09ID9K0uKTpfvlwM3z.jpeg)![image|375x500](upload://gsqyGpBqZxOaKttEqCJNEAiDqSG.jpeg)

Got a bunch Incase if any future builds. He Velcro should help secure some electronics to the enclosure. Hopefully Psychotiller finds use for them in terms of securing the battery to the enclosure when I send everthing his way.
```

---
## \#57 Posted by: Jc06505n Posted at: 2018-04-29T22:22:08.646Z Reads: 181

```
** Late April Update: **

Not much in terms of update except this glorious paint job by @treenutter

![image|500x500](upload://Ah9unUGgvzuM9gJsJDsSZdFO9N5.jpeg)![image|500x500](upload://lBrsqupPvdWgaH0tM4ChqksFVq2.jpeg)![image|500x500](upload://vK1aMKADVNtuR6TcmUZw5rfZUzz.jpeg)
```

---
## \#58 Posted by: Jc06505n Posted at: 2018-05-29T21:42:29.365Z Reads: 152

```
Been a while since I touched the project...

Laid down enclosures down to see how they’ll look in the Anubis. The trucks will be used on the Jet Spud Build , but I like the stealthy look of it. 


![image|375x500](upload://4rMmrYxrAQRtxbmrDuOeuX8NXOY.jpeg)![image|666x500](upload://sN5FToScb6o6MGUPEWZJZMQ6S5O.jpeg)![image|666x500](upload://dD5IokYKm87lOAdR9pLuEzGz7kC.jpeg)
```

---
## \#59 Posted by: Jc06505n Posted at: 2018-07-20T23:58:59.734Z Reads: 113

```
Been another while , but things are finally in semi progress, 

Sent off 2 Focboxes , the Deck , the Encolsures , and the screws off to @psychotiller for routing, drilling, and installment. Should arrive around Tuesday: 

![image|375x500](upload://1v895N53ZoeeXeth5lju9Qqnn7v.jpeg)

And it’s about time. The decks been sitting around collecting dust and playing dress up for months now 

![image|666x500](upload://vhBBKiAn5PvvyHYRMcM4WLzZDGp.jpeg)![image|374x500](upload://4FstIsLWrKYDiedaNC3SllqgScd.jpeg)![image|666x500](upload://ci2buNK1FC3Fu6Jy2Vn4y9gTX.jpeg)

Also took some comparison shots between EBoosted’s Vanguard Enclosure & Boosted’s 

![image|375x500](upload://nqnX3Io5CTCsNT7YOfXQ5O6XOjB.jpeg)![image|375x500](upload://hcR1wslplkbjH8PUoAGLLS3Sts.jpeg)![image|375x500](upload://bIzDRDzOZFQRRZbidwvPuj51aKO.jpeg)
```

---
