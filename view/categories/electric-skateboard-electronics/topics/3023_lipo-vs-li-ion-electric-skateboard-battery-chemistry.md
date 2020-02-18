# LIPO vs LI-ION - Electric Skateboard Battery Chemistry

### Replies: 24 Views: 11775

## \#1 Posted by: makepeace Posted at: 2016-05-09T06:24:42.019Z Reads: 723

```
Hey guys,

So I've been seeing more and more Li-Ion packs being built up, both by hobbyists and manufacturers (Enertion, LHB, etc), over LiPo packs.

What I've been wondering is... Why the switch?

As far as I'm aware, and please correct me here if I'm wrong, Li-ion's are heavier per unit Wh, more expensive per unit Wh and less power dense ie lower current handling capacity per unit mass. They also take up more space for equivalent pack sizes (lots of wasted space in the negative volume between those cylinders!).

What I do understand is that they theoretically have a longer life span than LiPo, and they are way safer. However, we all know that if you look after your LiPos, they are perfectly safe and can last for ever (2-3 years of daily use).

The other (theoretical) benefit is that they are easier to make up a pack, but only if you have access to a spot welder, which isn't really a benefit to the DIYist.

The only moot point between the two is the charging mechanism, as they both require balance charging, although you can charge LiPos a bit faster.

So, why the move? Should I consider buying an induction welder and head for Li-Ion?
```

---
## \#2 Posted by: willpark16 Posted at: 2016-05-09T06:30:19.721Z Reads: 693

```
Well you have the option of shaping your pack this may be minor to some but people with flexy decks are restricted with where they put their lipos. There is also the advantage of making a custom pack for that specific setup. This means my 190kv gets a pack that maxes out at 80amps and is limited by 60 from the vesc so i no longer have to worry about an explosion.

Edit- this is just what I can only assume. I personally prefer the 26650 lifepo4s, Also i dont think a lipo can last anywhere close to as many cycles a a li ion. So you have the added benefit of not having to open up your battery to switch out for a few years.
```

---
## \#3 Posted by: makepeace Posted at: 2016-05-09T06:36:21.298Z Reads: 671

```
The possibility of custom packs exists equally if not more accessibly (as mentioned above) with LiPos. I only make custom LiPo packs, as the form factor of the off the shelf LiPo "bricks" is far from suitable for eboards. It's very easy to solder up your own LiPo pack. I make mine from 5000mAh Hobbyking 25C single cells.

As regards switching out, bearing in mind you're spot welding your Li-Ion packs and you (usually) have 24+ cells to check for the dud, replacing a LiPo is much easier, as long as you have a consistent supply of single cells.

Edit: Didn't read your post properly. Noted extra life with Li-Ion/LiFePo4.
```

---
## \#4 Posted by: seanpain4 Posted at: 2016-05-09T07:07:44.897Z Reads: 657

```
You can get really high discharge 18650's, some are capable of around 15C from a single cell. They are also a lot safer and more durable. I also like the customization of shape. However you can pull apart a lipo and lay it out flat for an ultra thin battery.
```

---
## \#5 Posted by: onloop Posted at: 2016-05-09T11:15:58.050Z Reads: 639

```
For me, it was primarily about quality & consistency, followed by longevity & aesthetics.

My first few eboard builds were made using Cheap Lipo From Hobbyking... mostly 6S 8000mah Zippy Flight Max Bricks.

For the first few builds, they seemed pretty good... but i soon realised there was a problem! they were not all the same, on my fourth or fifth one the quality seemed to drop off, the physical size changed & there were a lot more puffy/bad cells starting to appear when they hadn't before, i assume hobbyking frequently change suppliers and just whack the same label on.

However, this was a major problem for me as i was just starting my business making custom eboards for people, i invested in 20 aluminium cases that were a perfect fit for this particular zippy flight max pack i was using... well as it turned out the tolerances for pack dimensions were crazy big... some varied by 3-4mm in width, height & length.... so eventually the batteries that i was receiving wouldn't fit in the cases anymore..

I then started searching for suppliers who could custom make the LIPO pack to my specifications, this was cool, i actually got some really high-quality packs rated to 60C! I was able to make really slim builds now with much more AH, not having any problems with puffing or bad cells either, but i was still only at 6s.

**WHEN THE VESC ARRIVED ON THE SCENE...**

This changed everything....

Because the vesc could handle up to 60V it seemed logical to make higher voltage packs, Mostly because I was having lots of heat problems when my heavier mates were trying to climb hills... so i was sort of forced to go higher voltage in an attempt to reduce current throughput.

The other contributing factor was that most of my mates had no fucking idea what a LIPO balance charger was.... They keep fucking the battery charge sequence up and one even caught fire and nearly burnt down a house...

I wanted higher voltage & also wanted onboard charging via a built-in BMS.... this way my big non-tech-savvy mates can ride up hills without over-heating and charge without any prior knowledge about proper battery care.

**This is where it got interesting...**

So I started asking a few lipo manufacturers about higher voltage packs with built in BMS, most of them had no idea what i was talking about.... Which was surprising... It turned out that most factories that made LIPO didn't use or understand the purpose of a BMS

After months & months of researching the ebike scene it appeared there was a common pattern, most battery packs that have built in BMS were made using 18650 format... it didn't really dawn on me at the time, i just assumed it was because it was a better technology, which it is for our use case... but there is more to it....

## Of course, it is possible to build a LIPO with a BMS! But the reason it is rarely done in the industry is because of these two points.

1. LIPO is a high output, low cost, lightweight battery technology which has a much shorter lifespan (charge cycles) to other chemistry like li-ion. Adding the cost, complexity & weight of a BMS sort-of defeats the key advantages of a lipo pack. To justify the cons (cost, complexity, weight, size) of using a BMS a battery must have a longer life span so that the cost of adding the BMS gets spread out over a longer period of time & often can make the cost per charge cycle equal to or in most cases better than a LIPO - so, in the long run, you sort of get the BMS for free & you also get the benefits of a BMS in exchange for a slightly larger back that cost more upfront. So the point is, the upfront cost is not that critical when considering a battery you should calculate the cost per charge cycle, longevity & how well it matches your project requirements.

2. Weight & Power Density, adding unnecessary electronics not only adds to upfront cost & can limit power output (most common BMS can't pump out 200A), but it also adds to volume & weight. You might not realise it but one of the biggest industry for LIPO is UAV & of course RC hobby industry... All these unmanned aircraft have payload restrictions/limitations, every gram counts!... so LIPO is the obvious choice, You need a small, cheap  & powerful pack that is designed to be removed & replaced frequently. There is no need for each pack to have a charging circuit because it can be charged outside the craft whilst the craft is being used. There is no real benefit of longevity (charge cycles) because the pack is so easily swappable & fairly inexpensive to replace - it's a consumable item!. In an electric vehicle designed for transporting humans, you don't really want to be limited to short trips & have to replace batteries frequently, especially if you could simply install a larger one in the first place! Human grade vehicles tend to be more robust in design with sleek aesthetics & integrated batteries to help improve the form, not so much the function. Also, The total weight isn't going to change if you have the battery in a carry bag or already integrated into the vehicle, so just install it! bigger & heavier is normally ok for EV...... OK... So the primary difference between EV & UAV is that the pilot goes with the EV & Doesnt with UAV, so for EV having small separate packs that need to be swapped out regularly is counter intuitive. With UAV though it makes a lot of sense to have smaller & swappable packs...the pilot is stationary and outside of the craft, they can easily have a bag full of batteries charge cycling ready to install once the UAV has landed. The weight & quantity of the spare batteries doesn't impact on the performance of the UAV because they are not onboard. In fact, smaller high-output packs improve UAV performance because of the power to weight ratios.

So to summarise, for EV you tend to want to go with longer life & bigger packs with built-in charging circuitry so 18650 Li-ion fits well, for small hobby grade toys you pilot remotely you want the lightest cheapest chemistry with no onboard circuits.

Furthermore.... the aesthetics of the 18650 cell are also important, they never change size! even if you change brands! they are consistently the same size! which is really important when you are designing & investing in expensive molds for your EV & battery enclosures.

Finally, the Quality! 18650 type cells are made by very large well known mega companies that spend billions to get 1-2% gains & have strict quality controls... Samsung, Panasonic, LG... so you know you are getting some quality chemistry with proven performance... LIPO's are mostly brandless silver pouches with colourful stickers attached, who knows where the fuck they come from... If you do spend time researching & testing you can find good LIPO, I certainly did.

I will happily say that I will never use lipo again on an EV
```

---
## \#6 Posted by: makepeace Posted at: 2016-05-09T11:20:45.199Z Reads: 531

```
Thanks for the great reply @onloop. I'm going to stick with LiPo for now, as I'm still very much on a budget and one of my core design aims is to try and keep things cheap. But I'm definitely going for a 18650 build in the near future.
```

---
## \#7 Posted by: onloop Posted at: 2016-05-09T11:28:34.585Z Reads: 525

```
[quote="makepeace, post:6, topic:3023"]
I'm going to stick with LiPo
[/quote]

Good call, I think everyone should consider using LIPO for their first build, Its a great way to learn about battery technology & balancing cells & battery handling/maintenance & wiring etc.

Also, they are cheap! so if you fuck it up you don't blow away $400+ dollars.

ALSO, most first builds are not exactly what you think they will be, once it is built & you are riding you might realise that the deck you selected is too short/long, the performance might not be as expected.... so there is a good chance you will be planning your 2nd build or at least some mods in the near distant future....


keeping the cost down whilst learning is not a stupid idea, just don't skimp out too hard...  a quality motor controller is a good thing to consider.
```

---
## \#8 Posted by: makepeace Posted at: 2016-05-09T11:38:30.967Z Reads: 499

```
Thanks for the advice. I'm a pretty experience designer and electro mechanical engineer, and I've already built a board. Haven't posted about it yet as I'm still fiddling with it. I've ordered some VESCs and new motors and batteries for a second build which I'm planning, using what I learned from the first. 3rd build will probably be Li-Ion. I'm also not an OEM manufacturer or something (yet), so LiPo makes sense to me, from a cost point perspective.
```

---
## \#9 Posted by: onloop Posted at: 2016-05-09T12:01:38.658Z Reads: 479

```
Sounds like it's time to buy a spot welder ;)
```

---
## \#10 Posted by: Hummie Posted at: 2016-05-09T16:20:53.598Z Reads: 465

```
Li-ion are much more energy dense by weight.


On my scale:
  Multistar 10c. 5200mah. 20.8 grams per amphour 
Zippy compact 35c. 4500mah. 26.6 grams per amp hour 
Lg hg2. (20amp per cell) 3000mah 15.0 grams per amphour. 

There are li-ion cells with 3500mah and 12.7grams per amp hour. 

Li-ion is much lighter
will have many more lifecycle
much more physically robust 
 much less prone to thermal runaway and a fire.  

The LG HG2 chemistry is particularly safe.
```

---
## \#11 Posted by: makepeace Posted at: 2016-05-09T16:31:03.873Z Reads: 456

```
That's good enough for me. Sounds like it's time to go Li-Ion.

10s4p here I come, when I can afford it.

Any best bang for buck recommendations in terms of cells and also on the manufacturing side?
```

---
## \#12 Posted by: treenutter Posted at: 2016-05-09T17:41:12.222Z Reads: 429

```
2 posts were split to a new topic: [Understanding 10s4p 18650 battery packs](/t/understanding-10s4p-18650-battery-packs/3032)
```

---
## \#13 Posted by: matejstambuk Posted at: 2016-10-17T10:28:19.141Z Reads: 356

```
[quote="onloop, post:5, topic:3023"]
If you do spend time researching & testing you can find good LIPO, I certainly did.
[/quote]

Thanks for so much info, I see you know a thing or two about LiPo's. I'm searching for a good LiPo for a month now, but I couldn't find a good quality ones. Would you be so kind to show me some manufacturers of quality LiPo's because I cannot afford myself a mistake?
```

---
## \#14 Posted by: 2-alex-2 Posted at: 2016-10-17T10:38:12.756Z Reads: 343

```
I used to to use gensace lipo in my RC cars and they were really good quality and they have a huge selection of configurations take a look at there website.
```

---
## \#15 Posted by: matejstambuk Posted at: 2016-10-17T10:52:27.451Z Reads: 326

```
The thing is, I want them to be **very** safe and reliable. Gensace seems like another chinese product.
```

---
## \#16 Posted by: 2-alex-2 Posted at: 2016-10-17T13:28:25.337Z Reads: 316

```
All lipo are safe if used in a good manor. So for a safe lipo you need a few things. First being either a good bms or a good quality balance charger. If no bms you would then need the low voltage cutoff settings set right. If you buy a pre built lipo like a 6s and split it make thinner the cells should get much better matched than buying two 3s in series as manufacturers normally only match the pack to closest cells, so you could have two packs further apart than what's in the 3s. If all safety measures are followed you should have no issues what so ever even if you brought cheap ones just their life cycle will be less from my experience. The gensace are a good battery read the reviews I have been racing with mine for best part of three years now with not swelling or issues as kept in storage mode.
```

---
## \#17 Posted by: Hummie Posted at: 2016-10-17T14:24:40.133Z Reads: 302

```
It's not the lipo brand that is either safe or not, more so the user.  If ur worried about finding a safe lipo...get Li-ion or better yet li-iron
```

---
## \#18 Posted by: 2-alex-2 Posted at: 2016-10-17T15:28:31.504Z Reads: 306

```
Yea probably all made in same factory's just the better brand pay to get the best ones out of the batches made and then lower ones are cheaper as not turned out as good.
```

---
## \#19 Posted by: tommyjamez Posted at: 2017-01-11T06:30:16.169Z Reads: 284

```
<img src="/uploads/db1493/original/3X/6/8/68a467db60e951ff5d16cb40f3acc96e1ef2d581.JPG" width="666" height="500">
I bought a spot welder because if you notice everything is using 18650 battery packs. When I looked up the replacement battery for my fiik street surfer and it said $1,550.00 for battery and charger that's when I decided to make my own.  Then my battery on my Roomba went and guess what 18650! My underwater jet-ski uses slag (lead batteries) so I built a much better, long lasting, a third of the weight 18650 pack with a BSM, used shrink wrap and done.  I highly recommend the welder.  It's not just going to be for your skateboard.  Hope this helped! I sent a pick of my welder but I'm not sure if it loaded properly.
```

---
## \#20 Posted by: killaton Posted at: 2018-09-18T15:55:38.296Z Reads: 119

```
Does anyone know why the cells, with their extra weight of the metal casing, are coming in lighter per Watt Hour then the pouch "lipos"? I thought they are both able to use pretty much the same chemistries?
```

---
## \#21 Posted by: Volts Posted at: 2018-10-30T08:24:40.785Z Reads: 100

```
lion cell are under press the jelly roll is encased in a nickle cell which acts to compress the anode and cathode together, you can do the same with the the lipos, to do so you need to compress the flat side between two plates, have this setup on my current board haven't done any long term test yet but from the information gathered from testing it so far my bet would be that they out preform the lion cell.
```

---
## \#22 Posted by: Faceplant Posted at: 2019-05-04T20:40:12.613Z Reads: 55

```
Can somebody explain this battery to me please. 
It's 7s1p rated at 25.2v 
If they're li ion wouldn't 6s be 25.2v? And 7s 29.4v? 4.2v per cell at full charge.
Do they base the voltage on what the lower end will be after discharge or something?![114bc72696ee25ac330e44547ff5d905efd25df6_2_750x1000|375x500](upload://x0HQlKBCcyqwOvOuQkOP05IPUXS.jpeg)
```

---
## \#23 Posted by: rich Posted at: 2019-05-04T21:03:57.464Z Reads: 53

```
You don't count with full voltage, it's nominal voltage. Li-ion have 3.6V per cell so 7s is 25.2V. A 7s lipo would have 25.9V (3.7V per cell). Both are fully charged 29.4V.
```

---
## \#24 Posted by: Faceplant Posted at: 2019-05-04T22:11:46.243Z Reads: 44

```
Thanks :) I appreciate it, must get old having to field questions like this. 
So I could theoretically replace my battery with a 7s lipo and a low voltage alarm? Waiting to hear back from the board's seller.
Also the esc is hooked up to a charge port on my board for the Li ion pack, would it be better to disconnect that or leave as is? Not to charge the lipo's just wondering if leaving it connected would cause problems.
```

---
