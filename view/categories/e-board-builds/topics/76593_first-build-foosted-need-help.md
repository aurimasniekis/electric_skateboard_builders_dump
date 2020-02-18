# First Build - &ldquo;Foosted&rdquo; need help

### Replies: 45 Views: 1384

## \#1 Posted by: JibeBigo Posted at: 2018-11-30T10:15:07.645Z Reads: 264

```
Hello dear builder,

I'm working on my first build and I have some question regarding parts. I've watched a ton of content and I'm starting to get the hang of the building process.
I know there's a lot of posts from new comers like me. Although there's some new alternatives on the market and I'm not really sure what to get.
I'm a happy Wowgo 2s owner but it failed on my lately, I think because of that freaking charging port cap which went off and let water in the battery enclosure. Not sure what component is failing, I want to rip off the heat shrinked PVC of the battery to look into it and see if there's corrosion but I won't be able to put it back on as my own heat shrink PVC didn't arrive yet.
I was hoping to use some components in my new build:

* ***The Board***:
* Loaded Vanguard flex 3 or 4 (I'm 62kg I'm not sure which one suits me the most)
* Caliber II 50" Trucks
* 85mm Orangatang 80a wheels
* Bones super red bearings
* 1/4" risers
-> 358€


## Recycled Components from wowgo:

* ***Battery*** : Samsung 44A 10s2p 4000mAh Battery -> 148Wh
-> Need to check if everything is right with it 
* ***Anti-Spark Switch*** 
-> This one should be good, just need to unsolder and resolder to the new setup.
* ***Enclosures***
-> These are not the most pretty enclosures but they'll save me ~50/100€
* ***Charging port***
-> It's included in the enclosure. I suppose this is not the failing component as my board charges normally when I plug the charger in.
-> Free :sunglasses:


## Purchased Components list:

* ***Motors***  : 2 x DIYesk8 6355 190kV - [Link ](products/electric-skateboard-motor-6355-190kv)
* ***Motor mount***  : 2 x Single motor mount by DIYesk8 - [Link ](products/single-bolt-on-motor-mount-set-red)
* ***Pulley***  : [this](products/36t-kegel-pulley-combo-kit) 16T option from DIYesk8

->290$

## Help me choose list:

* ***ESC***  : 
-> Here's where I need help. I originally ordered the Vesc 4.12 from DIYesk8 but I read here and there that they weren't that good. I'm thinking FOCBOX Unity but not sure when those will ship. Would love their push to start feature.
Otherwise I'm looking into Flipsky's Vesc 6.6. Do those have included anti-spark included ? 
If I get those, should I get 2x single ? 1x dual ?
Also they look to have many different versions [simplified](https://flipsky.net/collections/electronic-products/products/fsesc6-6-simplify-version-with-aluminum-heatsink) or [complete ?](https://flipsky.net/collections/electronic-products/products/flipsky-fsesc-6-6-based-upon-vesc%C2%AE-6-heat-sink). Not sure what the difference is between all those.

* ***Controller***  : I think I would go with enertion's nano x controller [link](https://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/). Would this work with Flisky's ESC or only with the focbox ?

* ***Lights***  : 
-> This is not a priority but I want to equip my board with front and rear lights for visibility and ideally they'd work with a voltage reducer on the same battery (where to solder this ?). Or should I buy a pre made solution such as shredlights (I've read mixed feelings reviews).

* ***Other*** : 
-> Here's also where I kinda lost. What do I need among these:

- Additional XT90 connectors 
- Additional XT60 ?
- Bullet connectors
- XT90/60 parallel / series connectors
- Can bus connector (I only need this if a take a 2x dual vesc i think)
- Servo connector (I think I need this in all cases to do esc -> remote receiver)
- anything else ? 

-> between 500 and 800$ i would guess


I do not have the budget for a big battery at the moment but hopefully I would upgrade later. 
What battery configuration (voltage / amps) would take full advantage from the motor specs ?
From my calculations if I build a 10s4p with Samsung 30Q 18650 cells it would cost me around 300€ including the purchase of a Spot Welder. Which is still cheaper than any website I browsed.

Sorry for the long post :slight_smile:
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-11-30T11:50:00.786Z Reads: 222

```
I would skip on the flipsky vesc due to all the little nuances that have popped up and haven't been remedied yet. Unity is too far away (time wise, I'm sure you actually want to ride the board, not stare at it )

I'm thinking used focboxes are your best bet, they can be found on the used items for sale tab

You said 10s4p was your plan for your battery and that's fine. Your other option would be 12s, which can lower system temperatures because lesser amperage flows for the same effect when you raise the voltage (** someone correct me if I'm wrong) and it provides a noticeable bump in speed 

If you're looking to get rid of your old hub motors I'm looking to grab some :slight_smile:

E: you forgot wheels! 
Would it be too shameless to link my 107mm? 😂
```

---
## \#3 Posted by: Grozniy Posted at: 2018-11-30T11:52:25.265Z Reads: 223

```
All the parts are good except:
You can't use antispark because it's inside the wowgo ESC. So you'll need a new antispark from @Martinsp or simple xt90s loop key.
Tb vesc are good. Just use them in 10s foc. You'll need canbus  or  ppm splitter.
Flipsky 6.6 dual is good in bldc.
Unity should be great. Should be shipped by this month but second batch is only in next year.
Everything else is good.
Get Riptide bushings and tunnel risers from @Alphamail
https://www.electric-skateboard.builders/t/bushing-set-up-help/42036?u=grozniy

10s4p battery is good.
```

---
## \#4 Posted by: Sn4pz Posted at: 2018-11-30T11:56:43.500Z Reads: 197

```
I don't mean to argue, but I wouldn't recommend putting TB vescs in foc mode, they pop like popcorn if you're not careful

E: that being said, 4.xx hardware that isn't the vesc x or focbox, or chakas vesc, has trouble with foc, so it's not only the tb vesc
```

---
## \#5 Posted by: Grozniy Posted at: 2018-11-30T11:58:04.168Z Reads: 191

```
That's possible yes. So if you want to be extra safe, use any vesc in bldc only ehehehe
```

---
## \#6 Posted by: JibeBigo Posted at: 2018-11-30T12:24:49.224Z Reads: 191

```
[quote="Sn4pz, post:2, topic:76593"]
E: you forgot wheels!
Would it be too shameless to link my 107mm? :joy:
[/quote]
Nice try but :stuck_out_tongue: 
[quote="JibeBigo, post:1, topic:76593"]
85mm Orangatang 80a wheels
[/quote]

I'm going to consider 12s4p then ! Still not sure which cells to use among [these](https://eu.nkon.nl/rechargeable/18650-size/price/0-4/min.-capacity-in-mah/1700-3600/discharge-current/15-35.html)

[quote="Sn4pz, post:2, topic:76593"]
If you’re looking to get rid of your old hub motors I’m looking to grab some
[/quote]

Yeah sure why not. I'm EU though so shipping might cost a lot if you're NA... They have around 600km I'd say but work perfectly.

Enertion doesn't seem to sell FOCBOX anymore :confused:

 

[quote="Sn4pz, post:2, topic:76593"]
I would skip on the flipsky vesc due to all the little nuances that have popped up and haven’t been remedied yet.
[/quote]
Could you please link me to a topic where those are stated ? I browsed the forum a lot and didn't seem to see anything about this.
```

---
## \#7 Posted by: Grozniy Posted at: 2018-11-30T12:26:23.341Z Reads: 145

```
Use 30q cells
```

---
## \#8 Posted by: JibeBigo Posted at: 2018-11-30T12:38:01.830Z Reads: 156

```
[quote="Grozniy, post:3, topic:76593"]
So you’ll need a new antispark from @Martinsp
[/quote]

It looks like all of them are out of stock. 

[quote="Grozniy, post:7, topic:76593, full:true"]
Use 30q cells
[/quote]
Why tho' ? If I get the 25R wouldn't the 80A max discharge be more useful than the additional 2Ah ? As said I'm a huge noobie on this
```

---
## \#9 Posted by: Grozniy Posted at: 2018-11-30T12:48:14.629Z Reads: 153

```
You'll want more range. 10s4p the discharge is plenty already
```

---
## \#10 Posted by: JibeBigo Posted at: 2018-11-30T13:31:44.606Z Reads: 163

```
I'm getting mixed reviews on the VESCs lol. 
I think I will go flipsky 6.6 and maybe upgrade to FOCBOX later. I could then use my old vesc with a shorter deck.
I'll also investigate if I can find a place where there's a shared spot welder saving most of the cost and space in my small city flat.
What are the basics I need ?
- Heat shrink for wires + for battery 
- Soldering iron
- Foam 
- Drill
- heat gun ? or hair dryer does the work ?
- Multimeter ?
- what else ?
```

---
## \#11 Posted by: Sn4pz Posted at: 2018-11-30T13:52:29.159Z Reads: 157

```
Yeah I'm in the US of a, I guess shipping will be too much 🙃

If you ever come to the states... Bring them with you? :D 

I'll link it in a second, let me type this out first so it doesn't lose my process 😂😂

I would honestly recommend the sanyo 20700 a cells, or whatever the name is 😂😂 they have 3000mah(I think?) And 30a discharge, meaning that if you stuck with 12s4p you would have tons of range and little voltage sag

But if you wanted to stick with 18650s , can't beat the 30q

Don't go 25r, sags more than Hopsins pants
```

---
## \#12 Posted by: brenternet Posted at: 2018-11-30T13:58:28.171Z Reads: 150

```
[quote="JibeBigo, post:10, topic:76593"]
what else ?
[/quote]

A damn good set of Allen keys. People here (myself included) like the wera set. If you buy cheap chocolate tools you'll strip everything on your board and curse yourself!

A good set of pliers/wire strippers and a handy tool to help you solder. 

On the topic of solder, a good solder sucker and some flux will save you frustration. You'll also need wire. 12awg, 14awg and I believe 20/22 for phase wires, someone can correct me there.
```

---
## \#13 Posted by: moon Posted at: 2018-11-30T14:18:10.755Z Reads: 136

```
Battery 10awg
Motor 12 awg
```

---
## \#14 Posted by: Grozniy Posted at: 2018-11-30T14:18:46.901Z Reads: 138

```
You can get @aulakiria spot welder or maletrics spot welder for around 100
```

---
## \#15 Posted by: brenternet Posted at: 2018-11-30T14:21:18.138Z Reads: 140

```
Do the math on it though. Welder, cells, nickel, fishpaper, time, mistakes/wastage.

Making a single battery, or even two, I'd be surprised if it was less expensive than buying one.
```

---
## \#16 Posted by: Trdolan03 Posted at: 2018-11-30T15:00:39.270Z Reads: 135

```
Esk8life.com. $250 for a 10s 3p or $300 for a 10s 4p. BMS comes installed and everything is ready to go. That price includes US shipping.
```

---
## \#17 Posted by: JibeBigo Posted at: 2018-11-30T15:06:59.790Z Reads: 137

```

[quote="Trdolan03, post:16, topic:76593"]
[Esk8life.com](http://Esk8life.com). $250 for a 10s 3p or $300 for a 10s 4p. BMS comes installed and everything is ready to go. That price includes US shipping.
[/quote]

Nice, that's what I needed !
Most of 10s4p are actually flat and that wouldn't fit a vanguard flexy deck ! This one is cheap as well !

According to my calculations, it should be 239$ so 210€ that's cheap AF
```

---
## \#18 Posted by: JibeBigo Posted at: 2018-11-30T17:08:11.726Z Reads: 131

```
Nevermind I contacted him and said the batteries he makes wouldn't fit a Vanguard deck. Also he mentionned EU shipping would be very costly. I need to find a battery maker in EU.
```

---
## \#19 Posted by: Sn4pz Posted at: 2018-11-30T17:25:37.254Z Reads: 130

```
@darkkevind
```

---
## \#20 Posted by: tardyparty7 Posted at: 2018-11-30T17:28:58.758Z Reads: 130

```
I made a parts list for this in the past:

https://docs.google.com/spreadsheets/d/1sdfZjVBC2iZ9OKkSeshiJ5TTy_HXXEuKdGuUJMCPmY8/edit#gid=0
```

---
## \#21 Posted by: JibeBigo Posted at: 2018-11-30T17:34:05.642Z Reads: 118

```
Thanks a lot ! Is that firefly remote still selling ? It looks dope.
```

---
## \#22 Posted by: Lumaci Posted at: 2018-11-30T17:36:11.135Z Reads: 115

```
If you ask around you can get someone to make one for you.

I may have a kit i need gone with all the parts for it.
```

---
## \#23 Posted by: Grozniy Posted at: 2018-11-30T18:08:50.455Z Reads: 113

```
@pjotr47 and @Acido and @OskarCastrone  make them
```

---
## \#24 Posted by: pjotr47 Posted at: 2018-11-30T18:17:06.370Z Reads: 112

```
I make all my packs custom made. So I can build everything you want. Check out [Electricpacks](https://www.instagram.com/electricpacks/)
```

---
## \#25 Posted by: tardyparty7 Posted at: 2018-11-30T23:22:04.502Z Reads: 112

```
It's a diy remote. If you are willing to get all the parts and stuff, it is really **fun**! You do need a soldering iron and stuff like that, but they're not really expensive. The most expensive parts are the 3d printed parts, but I'm sure there are places online where you can get the prints. Just ask on the forum!
```

---
## \#26 Posted by: mtuan293 Posted at: 2018-12-01T04:25:21.379Z Reads: 108

```
The Flipsky 6.6 (dual and single) is good, and their 4.12 is ok too. Just that 4.20 dual has issues.
Reference:
https://www.electric-skateboard.builders/t/poll-flipsky-information-in-one-place/68940/119
```

---
## \#27 Posted by: JibeBigo Posted at: 2018-12-01T13:28:11.096Z Reads: 109

```
Do you guys know where I could get Vanguard enclosures for ~50$ ESC and Battery ?
I've seen eboosted's but 150$ shipped is a huge hole in my budget I can't afford that given the cost of all the parts.
```

---
## \#28 Posted by: Alex753 Posted at: 2018-12-01T13:30:28.053Z Reads: 107

```
https://www.ownboard.net/products/metle-case-and-w1-deck-without-hand-hole

Thoses are really nice, not exactly the same as the boosted ones but looks great too

![image|690x307](upload://fnZNSPx1fY4anpqu1xtzbn67wMZ.jpeg)
```

---
## \#29 Posted by: JibeBigo Posted at: 2018-12-01T13:33:14.868Z Reads: 101

```
My bad, I own those but @pjotr47 told me that won't fit a 10s4p battery which I eventually want in my board.
He suggested a 10s2p Sanyo but will that work with "only" 30A max discharge or will I get a ton of sag ?
```

---
## \#30 Posted by: Alex753 Posted at: 2018-12-01T13:53:49.843Z Reads: 102

```
My two’s 8S 4.5 45C Hobbyking batteries mounted in serie fit in thoses, so 202A Max ! 

8S is enough for me but maybe you can buy 2 5S batteries if you didn’t already buy them.
Hobbyking have some 5S 8A pack so you could have a great 30Km range without problems !
```

---
## \#31 Posted by: JibeBigo Posted at: 2018-12-01T14:33:10.389Z Reads: 97

```
I'm more incline to go Li-ion rather than lipo though. Can you put a charging port for lipos ?
```

---
## \#32 Posted by: Alex753 Posted at: 2018-12-01T15:15:24.409Z Reads: 100

```
With a Bms yes, I guess that it work like a Li-ion ?
```

---
## \#33 Posted by: JibeBigo Posted at: 2018-12-08T15:50:59.520Z Reads: 99

```
Hey guys I'm looking for some copper flat wires to avoid having to drill channel for the wires.
Not so sure about what to get though.
I'm from UE so Ebay is fine, amazon.com not so much.

I found this not sure if it would meet the requirements for the current that would go through those cables:
https://www.ebay.com/itm/Wide-2mm-20mm-Flat-Braided-Tinned-Copper-Wire-tin-plating-copper-shield-tube/273455093236?hash=item3fab3195f4:m:mV6THvZVZQNfSP--foJ1lTw:rk:4:pf:0&var=572841534954

Then I'd put electrical tape on top and a brand new grip tape :)
```

---
## \#34 Posted by: KranzeKake Posted at: 2018-12-18T01:22:18.985Z Reads: 90

```
I made a build tutorial of my Foosted... Check it out if you want to!
https://www.youtube.com/watch?v=EbNoS0Tr8c8&feature=youtu.be
```

---
## \#35 Posted by: Alex753 Posted at: 2018-12-18T01:30:35.169Z Reads: 87

```
That’s so cool dude thank you !
```

---
## \#36 Posted by: swimmydude Posted at: 2018-12-18T05:45:58.846Z Reads: 85

```
Along with a good set of allen wrenches, my ceramic tweezers has been a godsend. I suppose needle-nose pliers works as well. It's been super useful but it pertains to doing electronic components stuff. Correct sizes for wire strippers too. So if you're not doing a lot of soldering and such, it doesn't matter too much. 

If you haven't already gotten a vesc, FocBoxes are for sale again. Pretty damn cheap too, I dunno if there is a limited supply or what though. 

I don't know if you're still decided on making your own battery pack or not but like people said before, you should consider mistakes and the learning process in your equation. I know the boss spot welder is pretty sweet. It does a good job and it is very small compared to the traditional spot welders you can buy. Even though it is about ~$100 (I know you use euros), the price for the correct li-po wasn't part of my initial price assessment and added about $50 more to the price. You can't get an underpowered lipo but I would have still opted for this spot welder. It's fantastic.
```

---
## \#37 Posted by: JibeBigo Posted at: 2018-12-18T09:53:58.332Z Reads: 77

```
![]( https://i.imgur.com/CFu8ouq.jpg)

Thanks man <3

@KranzeKake how long the copper wires need to be ? 
I have 2 retail solution one is 33cm for 4€ the other is 10m for 60€. Can i save a little buck on this ?
```

---
## \#38 Posted by: janpom Posted at: 2018-12-18T12:05:11.953Z Reads: 76

```
[quote="JibeBigo, post:10, topic:76593"]
* heat gun ? or hair dryer does the work ?
[/quote]

Hair dryer won't work for shrinking a heat shrink. A lighter will though. You don't really need a heat gun though it's a nice to have.

Get some 60/40 leaded solder. It's much easier to work with than unleaded.
```

---
## \#39 Posted by: KranzeKake Posted at: 2018-12-18T13:37:59.733Z Reads: 72

```
Well it depends on the length of your board
```

---
## \#40 Posted by: JibeBigo Posted at: 2018-12-18T13:40:00.400Z Reads: 69

```
Well I'm using the same as your build. How long were your copper cables ?
```

---
## \#41 Posted by: KranzeKake Posted at: 2018-12-18T13:50:52.953Z Reads: 67

```
Il measure it when I get home, should be in about an hour
```

---
## \#42 Posted by: JibeBigo Posted at: 2018-12-18T13:53:40.192Z Reads: 69

```
Well that's very nice of you I didn't expect so much :slight_smile: an estimation would've been good enough.
```

---
## \#43 Posted by: KranzeKake Posted at: 2018-12-18T16:22:06.301Z Reads: 66

```
They are about 40CM // 16 inches
```

---
## \#44 Posted by: JibeBigo Posted at: 2018-12-18T16:56:18.764Z Reads: 65

```
thx a lot buddy
```

---
## \#45 Posted by: JibeBigo Posted at: 2019-01-29T22:59:22.963Z Reads: 50

```
I'm a dumb brick. I bought a flispky dual 6.6 which doesn't fit eboosted's enclosure. Now I'm stuck... Holes are drilled in the deck...
```

---
