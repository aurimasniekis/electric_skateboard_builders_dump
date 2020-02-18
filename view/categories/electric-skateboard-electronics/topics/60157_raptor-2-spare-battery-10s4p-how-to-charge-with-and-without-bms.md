# Raptor 2 Spare battery 10s4p how to charge? with and without bms?

### Replies: 36 Views: 1077

## \#1 Posted by: Boxer86 Posted at: 2018-06-26T23:33:17.731Z Reads: 158

```
I am in Australia so getting a lithium ion setup is a little more difficult to get if you don't want to put it together yourself. As the 10s4p Raptor 2 spare battery pack is readily available in Australia i was hoping to use it on my dual 6374/focbox setup. The problem is i am not sure how to effectively charge it as it does not have a bms built in. From what i have read it can be charged using a charger and the cells should self balance. Is this correct? Also how would i go about doing this? eg what charger, what connectors to link charger to battery. As far as i am aware no one has actually used this particular pack  on a diy yet, either with or without bms but if you have please let me know how you did it. Thanks heaps. To save you going to enertions site the specs are below:

The NEW Enertion S.P.A.C.E Cell Elite 
Spare Battery - Designed specifically for your Raptor 2 

> The battery is 10S4P - A total of 40 Cells, 4 Parallel groups of 10 cells in series.

> Premium Quality Samsung 30Q Cells. 

> Battery Chemistry INR/NCA

> 432Wh pack. 4X greater capacity compared with market average.

> 36V nominal voltage

> Total weight 2070 grams

> Dimension of 370mm X 140mm X 22mm

> Cells Only. No BMS inside this pack
![image|500x500](upload://dQMhWf0z7j4RjxXDariVM5NFGlz.jpg)
```

---
## \#2 Posted by: Skitzor Posted at: 2018-06-26T23:38:50.027Z Reads: 147

```
Hi Man,

A BMS is always optional. But I would always advise to get one to compliment the lifespan of your cells. Any 10S BMS will do. Could be that you need to reverse the BMS connector. But that's not a really hard job to get done. Apart from that, this pack is as compact as a 10s4p can get.

Edit: if you would go for BMS-less. you'll need a 42V 2A or 4A charger, remove the plug and install a XT60 connector
```

---
## \#3 Posted by: Boxer86 Posted at: 2018-06-26T23:41:04.874Z Reads: 141

```
I forgot to mention if not using a bms i was going to set up the battery cut off in the focboxes to around 20% capacity stop it overdrawing the battery and then charge the battery up the around 85% of full capacity. Just not sure how i would charge the battery this way
```

---
## \#4 Posted by: wafflejock Posted at: 2018-06-26T23:44:47.591Z Reads: 139

```
If you just search "10S balance chargers" you'll find ones that will allow you to balance charge, I don't think just charging off of the main discharge leads without any cell levelling/balancing is a good idea.
```

---
## \#5 Posted by: Skitzor Posted at: 2018-06-26T23:46:50.479Z Reads: 133

```
A decent BMS + charger is cheaper than a decent and respectable "balance" charger

Edit: search topics here if you'd want
```

---
## \#6 Posted by: Boxer86 Posted at: 2018-06-26T23:49:32.070Z Reads: 124

```
Now i see why most people use a bms

It seems a lot are using this bms Would this work:
http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

and if i hooked up this bms with the factory settings and a compatible 42v charger it would automatically balance my cells?
```

---
## \#7 Posted by: wafflejock Posted at: 2018-06-26T23:50:28.408Z Reads: 122

```
10S are pricier but not needing to carry your charge circuitry everywhere and have it constantly subject to vibrations is a plus.  I use 2 5S lipos so it's not as bad to get a couple cheap chargers and charge them separately and they connect in series in the enclosure on my board.
```

---
## \#8 Posted by: Boxer86 Posted at: 2018-06-26T23:54:36.419Z Reads: 115

```
I was thinking of using lipos but i have a 17km two way commute to work (34km round trip) with hills so I would need 4x 8000mah 5s lipos to make the trip which in Australia cost the same as the raptor 2 pack. As i have read i will get better lifespan out of the lithium ion pack so i thought this would be the better option. What are your thoughts?
```

---
## \#9 Posted by: Skitzor Posted at: 2018-06-26T23:56:38.680Z Reads: 126

```
Thats (imho) a good BMS to have. Keep in mind, you can only order them per 2 as a B2C customer.
Try finding someone to chime in, or a GB on this forum.

@wafflejock we're talking lion here. both have pro's and cons. But given the instabilty of lipo. I personally would not cheap out on chargers/ BMS.
```

---
## \#10 Posted by: wafflejock Posted at: 2018-06-27T00:01:52.385Z Reads: 127

```
iMax b6 is basically tried and tested and there have been people using lipos in rc hobbies for much longer than people have been hacking together their own 18650 based packs.  Cheap doesn't always mean bad.  Regarding dangers I've seen far more 18650 based boards ablaze here than lipo based packs the extra fear makes us extra precautious about punctures.

Regarding range you need about 10Wh per km on average I can get 12 miles on most of 185Wh, so you may not need quite what you're thinking also if you can plug it in at work or like I did get it up so swapping batteries is pretty easy then you can carry extra cells with you.
```

---
## \#11 Posted by: Boxer86 Posted at: 2018-06-27T00:02:34.264Z Reads: 120

```
Yes thanks for that i will either buy two and sell the other or get a spare off someone. Just confirming though that the bms will infact keep the cells balanced and that the factory specs of the bms are fine for this particular battery pack? Also what 42 volt charger would work with this bms and what is the best way of connecting it? Thanks heaps for your input by the way. I have been reading this stuff for weeks now and it is slowly starting to sink in :sweat:
```

---
## \#12 Posted by: Skitzor Posted at: 2018-06-27T00:08:34.915Z Reads: 113

```
@wafflejock I'm not against Lipo. But dont compare RC cars/drones to eboards. They have to carry some abuse in the hard way. Both are fine. All the different builds in here show that. I personally have seen/read more mess with Lipo than Lion. 

@Boxer86 In the end, You'll have to decide on your build. It's up to you to choose your connector. You can have the standard charger one. Or replace it with an XT60 (If going for this battery). Lots of good schematics and parts on this forum

Edit: Any 42V (10s) charger will do. 2A is slow 4A is fast (2h max)
```

---
## \#13 Posted by: wafflejock Posted at: 2018-06-27T00:16:37.668Z Reads: 112

```
I don't really see how it's not an apt comparison seeing as how we use just about all the same technology, people on 6S with quads can pull 100A+ when flying to the moon :)  The point really though is 18650s aren't inherently safer especially with the abuse we put everything on our boards through just riding them around on crappy ass roads.  Just use the search feature here and search for 'fire' see how many 18650 fires you have to wade through to find anything about lipos, so far I only found a thread about how to not start a fire with lipos (safe charging).  Granted there are more people using 18650s so the number of failures is going to be higher but literally can't find a lipo one in there (even searching for 'lipo fire' I'm finding things about 18650s exploding only)
```

---
## \#14 Posted by: Boxer86 Posted at: 2018-06-27T00:19:33.628Z Reads: 106

```
Thanks heaps for that. I will continue the research and work out the best setup for me.
```

---
## \#15 Posted by: Boxer86 Posted at: 2018-06-27T00:23:13.787Z Reads: 106

```
By the way the only reason i am slightly swayed toward lithium ion is that i have read you get considerably more life out of them and if it is going to cost the same i might as well go with the longer life pack. I am however aware that the lithium ion pack will probably sag more but i am willing to take this for the longer life i will get out of the pack. As for the fires from what i have read if you are sensible either option will work and be safe as long as you take all the precautions when charging/discharging so i am not too concerned about that.
```

---
## \#16 Posted by: wafflejock Posted at: 2018-06-27T00:27:24.451Z Reads: 104

```
Curious where you saw about differences in the number of cycles, as far as I know that's more dependent on the quality of the cells than the packaging: https://scottiestech.info/2015/06/21/lithium-polymer-vs-lithium-ion-batteries-whats-the-deal/

Have been using my original pair of 5S Turnigy batteries for a while now but can't say I've been logging the health with regard to mAh put in while charging, maybe will check it out soon.  I just got another new pair for swapping out the two sets if I do end up needing to take a longer than usual trip.
```

---
## \#17 Posted by: Skitzor Posted at: 2018-06-27T00:30:33.107Z Reads: 103

```
That's why the parallel groups matter. at 4P. There is no sag to be mentioned (a bit at 3P, again my experience) 

@wafflejock It's hard to compare those statistics, that's also why I don't mention them and like I said. Personal prefs. If you Like big power. Lipo is prolly the way to go. And I think they're more dangerous charging than being abused. (as a sidenote). But even on my powerdrills, I'm enjoying lions more than older tech. Lifespan being the main part
```

---
## \#18 Posted by: wafflejock Posted at: 2018-06-27T00:31:44.468Z Reads: 105

```
I don't really get where the extra lifespan comes from I'd imagine the lifespan is really a product of the internal resistance and how much the battery is cooking itself (how stressed it is relative to that internal resistance).

Regarding overcharging and all I guess I just got accustomed to taking care and monitoring things with charging my quad batteries but seems safer than having your potential fire attached to an extra fuel source if it does go (plus worst case scenario I lose one 5S instead of a 10S).
```

---
## \#19 Posted by: Skitzor Posted at: 2018-06-27T00:33:13.671Z Reads: 105

```
Fact is, after 500 charges, the lipo is done. lion survives 1000. Why is there no lipo to be found in your cellphone ? or like I mentioned, good cordless power drills.
```

---
## \#20 Posted by: Boxer86 Posted at: 2018-06-27T00:34:24.045Z Reads: 106

```
Interesting read. I did notice that in the article it said it is the number of cells that gives li-ion more life which makes sense. Comparing the li-ion 10s4p (40 cells) vs lipo - 5s 8000ah x4 (20 cells) with the offset that iipo have more volume for the same space resulting in more punch.
```

---
## \#21 Posted by: Skitzor Posted at: 2018-06-27T00:37:22.991Z Reads: 93

```
Ok guys, fun topic, But if I don't want to be a zombie tomorrow. I gotta catch some sleep. Gladly respond tomorrow !
```

---
## \#22 Posted by: Boxer86 Posted at: 2018-06-27T00:42:16.078Z Reads: 90

```
Haha it is 10:40 am here in Australia. You had better get some sleep. Thanks again for all your help.
```

---
## \#23 Posted by: wafflejock Posted at: 2018-06-27T00:43:22.229Z Reads: 93

```
With regard to consumer products I believe the reasoning is just mass scale translates to cheaper products and having a standard dimension for the cell for different devices means they can all buy the cells from the same manufacturer, but that doesn't really have anything to do with the performance of the cells or the chemistry going on inside them.  All I'm saying in general is both of them are dangerous and you should be cautious either way, don't treat 18650 package like it's somehow tamed the lithium-ions inside :slight_smile:

The [write up here](https://www.quora.com/Which-is-a-better-battery-for-a-smartphone-Li-Ion-or-Li-Po) goes into more elaborate detail and does point out the 18650 cells shell stops the cell from expanding/contracting which can prolong its life but I don't know that I've seen anyone actually get 1000 cycles out of any cell.  Mostly everything I've seen says they range from 300-500 regardless of packaging but again I imagine this all depends on how you stress them both in charging and discharging (Tesla's get extreme longevity out of 18650 cells by not fully utilizing their capacity from what I've read)  http://www.instructables.com/id/How-to-Prolong-the-Life-of-an-18650-Battery/
```

---
## \#24 Posted by: Boxer86 Posted at: 2018-06-27T00:49:37.259Z Reads: 85

```
Thanks for your input i will have a read. By the way does anyone know if i can use the enertion fast charger that is on sale to charge the raptor 2 battery with or without bms? I am assuming i can seeing as though it was designed to charge the same battery (admittedly through the raptors bms) It must be a standard 42 volt charger right?
```

---
## \#25 Posted by: strattos Posted at: 2018-06-27T00:52:33.670Z Reads: 85

```
All phones I've seen are lipo. Lion are inherently safer on the cell level. I think the reason we've seen more lion packs catch fire then lipo is because all these lion packs are being made by diyers. Look at any cell testing and 18650's are much safer.
```

---
## \#26 Posted by: bandrews510 Posted at: 2018-06-27T01:07:17.570Z Reads: 86

```
You are going to need a female DC power jack wired in parallel to the pack in order to charge to charge the pack straight off the Enertion charger. Would highly recommend the aforementioned BMS as you can solder the DC jack to the designated charging spots on the BMS and solves the problem of balancing. 

For me going with a lion pack eliminated a lot of wiring as far as the series and parallel configurations of the Lipos I had in the past.
```

---
## \#27 Posted by: wafflejock Posted at: 2018-06-27T01:13:38.169Z Reads: 94

```
@strattos can you elaborate on inherently safer... I mean I understand the likelihood of puncture with a lipo pouch is higher than with a metal cylinder around it but I don't see it as inherently safer.  With the solid cylinder there is an escape vent for the gas/heat to blow out of in case of a failure but the most recent PSA the poster commented about them shooting off like rockets which doesn't sound super safe (packing together 40-60 of them is going to be more dangerous than an individual cell, more points of failure and chain reaction).

@bandrews510 I was thinking about this earlier in this thread as well, if you do the 2S or 3S in sets then the wiring does get more unwieldy I went with 5S which is less than ideal in terms of the thickness, but along with [some 3d prints](https://www.thingiverse.com/thing:2243206) makes hooking them up and disconnecting easier.

I can definitely see the convenience angle of BMS but I just don't like the idea of all the components on there rattling around all the time then trusting them to balance my cells really.  Only ones I saw that I'd trust plus price of quality 18650 pack was just too much of a gap for me.
```

---
## \#28 Posted by: onloop Posted at: 2018-06-28T00:21:54.654Z Reads: 86

```
You can do it with this type of charger, then you don't need to wire up a BMS.

https://www.icharger.co.nz/icharger-1010b
```

---
## \#29 Posted by: Itsmedant Posted at: 2018-06-28T00:29:54.026Z Reads: 86

```
I ordered that exact one through www.buildkitboards.com

He is a fellow diy'er on this forum (@JLabs)
```

---
## \#30 Posted by: strattos Posted at: 2018-06-28T00:57:39.091Z Reads: 88

```
I've had lithium ion cells vent in my hands (I was wearing thin gloves and didn't notice the heat build up).

All your safety concerns would be addressed by pack design Imo. Cells should be properly secured so they can't go flying off like rockets. 

Of course different chemistries have different dangers for 18650's but as a general rule of thumb they're essentially lipo's in a strong container designed to fail the same way. 

The biggest issue I personally find with battery builds is that people aren't monitoring what's going on down there temp wise current wise Nada. The only reason I'm using a bms is because I can actively monitor 2 temperature sensors current in current out and individual cell voltages all the good stuff. 

Just look at some cell data sheets for a 30Q. Would you put a lipo in a 140C oven for 7 hours, would you crush a lipo, would you overcharge a lipo with 4x the voltage and amperage intended to be charged at? 30Q's passed all of those tests with L1 failure (defined as leakage). 

Now I'm not gonna lie I didn't check any datasheets for major Lipo manufacturers that are being used for eskate's. 

But in my personal experience I'd much rather have an 18650 vent in front of me then a lipo pack.
```

---
## \#31 Posted by: Boxer86 Posted at: 2018-06-28T01:58:28.313Z Reads: 82

```
That’s great. If I got the raptor 2 pack would it give me the range I need (35km with a few smaller hills). Will be using dual focbox with 6374 190kv
```

---
## \#32 Posted by: ElskerShadow Posted at: 2018-06-28T07:26:05.451Z Reads: 78

```
[quote="Skitzor, post:2, topic:60157"]
remove the plug and install a XT60 connector
[/quote]

Why use xt60 instead of regular charger port?
```

---
## \#33 Posted by: onloop Posted at: 2018-06-28T09:22:01.121Z Reads: 76

```
10wh/km is fairly common, the battery is 432wh
```

---
## \#34 Posted by: Skitzor Posted at: 2018-06-28T22:45:30.139Z Reads: 56

```
In his case he presented he had no bms or charger plug. Wanted to buy a R2 spare battery and a charger. What's the easiest and cheapest (not recommended) way of making that charge and connect to the rest of the system?
```

---
## \#35 Posted by: Skitzor Posted at: 2018-06-28T22:48:32.037Z Reads: 57

```
There is no such thing bro. All lion (as far as 2015 for sure) how would you adress the fast charging without puffing packs. Or the limited charge cycles?
```

---
## \#36 Posted by: ElskerShadow Posted at: 2018-06-29T08:08:48.613Z Reads: 47

```
Just use a classic charger, 30Q are really amazing cells and can self balance themselves
```

---
