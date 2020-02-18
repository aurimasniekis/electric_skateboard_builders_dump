# Range extender plugged into charge port

### Replies: 145 Views: 3911

## \#1 Posted by: amazingdave Posted at: 2018-08-09T09:42:14.618Z Reads: 564

```
I’m buying all the bits for my next build and have realised that the 10s5p battery I’m building won’t quite get me to work on my commute.... 

So I’ve come up with a slightly sideways plan. 

If I make a 2s5p battery pack and plug that into my loopkey I’d have a 12s5p for my long commutes and my slick lovely @Hummie with @bigben enclosure for the rest of life...

I’m not going to use the bms for discharge btw. 

Thoughts?
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-09T10:23:44.087Z Reads: 535

```
Wouldn’t you need to add a parallel pack to get more range?🤔
Serial connections will give you higher voltage and more speed. Not sure if the range would add up too
```

---
## \#3 Posted by: amazingdave Posted at: 2018-08-09T10:31:25.596Z Reads: 529

```
50 cells plus 10 more cells= 20% more range

And yes I’d have to limit my Erpm but that’s what I do on my current board anyway running 12s.

I could burn through the extra capacity with speed but I don’t have to pull that trigger! 

The main issue I see is have to change my vesc settings each time I go from one to the other....
```

---
## \#4 Posted by: Skunk Posted at: 2018-08-09T11:56:13.200Z Reads: 500

```
Sounds easier to just move closer lol
```

---
## \#5 Posted by: Wraith Posted at: 2018-08-09T12:00:12.082Z Reads: 483

```
Does the bigben enclosure fit the 12s5p nicely or do you need to mount the vescs externally?
```

---
## \#6 Posted by: pat.speed Posted at: 2018-08-09T12:00:48.597Z Reads: 481

```
Using a Bluetooth module certain boards allow you to have different setting of each board, you could just have two different settings one for 10s and one for 12s
```

---
## \#7 Posted by: bigben Posted at: 2018-08-09T12:06:04.296Z Reads: 472

```
You would have to mount the vescs externally. I'm going to look at a double stack enclosure when I get time....
```

---
## \#8 Posted by: Wraith Posted at: 2018-08-09T12:08:00.893Z Reads: 457

```
double stack would be fantastic keeping it slim with nice clearance would likely be easier due to the recess. Wonder how much that would weigh on a build though :thinking:
```

---
## \#9 Posted by: Skunk Posted at: 2018-08-09T12:09:32.124Z Reads: 443

```
Even just a single stack with a bulge in it to fit vescs would be great.
```

---
## \#10 Posted by: bigben Posted at: 2018-08-09T12:10:06.216Z Reads: 427

```
I'll have a muck about with some cells to see what the impact would be.
```

---
## \#11 Posted by: Wraith Posted at: 2018-08-09T12:12:12.213Z Reads: 418

```
single stack is doable on 12s4p with vescs according to @hummie. I'm considering those squeeze packs He's got planned on the 2 hole deck. Not having to solder would be great :laughing:
```

---
## \#12 Posted by: Skunk Posted at: 2018-08-09T12:28:32.295Z Reads: 389

```
60 cells or bust
```

---
## \#13 Posted by: TinnieSinker Posted at: 2018-08-09T12:28:50.076Z Reads: 389

```
im working on a piggyback battery at the moment. It'll plug into the charge port  and charge as you ride.

using a 6s lipo and a buck boost to get 42v

Have seen pics of others doing this but no details. hopefully i'll have some parts to test with soon and let you now how it goes
```

---
## \#14 Posted by: Wraith Posted at: 2018-08-09T12:33:03.032Z Reads: 377

```
sounds awesome! so you can put one together for specific battery configs?
```

---
## \#15 Posted by: TinnieSinker Posted at: 2018-08-09T12:55:37.948Z Reads: 384

```
probably! :smiley: the buck-boost has a variable output, however, the bigger the difference between voltages the fewer amps it can push out.

https://www.ebay.com.au/itm/DC-DC-600W-10-60V-to-12-80V-Boost-Converter-Step-up-Module-car-Power-Supply-AU/162286536954?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

https://hobbyking.com/en_us/multistar-high-capacity-6s-12000mah-multi-rotor-lipo-pack.html
```

---
## \#16 Posted by: Wraith Posted at: 2018-08-09T12:57:40.484Z Reads: 359

```
That would be kind of like having swappable packs! so charging while riding? I wouldn't want to do that but charging at a place without any wall plugs, Then I see much more convenience in it!

Unfortunately establishments without wall plugs can be quite common where I'm based :confused:
```

---
## \#17 Posted by: TinnieSinker Posted at: 2018-08-09T13:02:04.690Z Reads: 358

```
yea same, i'd prefer to charge up while i'm still out. but yea some people put all this in a box sitting in between their feet while they ride for super long trips. you could even keep extra lipos in your backpack and swap them out then keep going .... for everrrrr!

yea its basically a huge powerbank XD
```

---
## \#18 Posted by: Skunk Posted at: 2018-08-09T13:04:35.999Z Reads: 341

```
A "how to" thread would be great for this. I'm not sure about charging and riding.  But charging without outlets would be great for some of the trails I wanna take.
```

---
## \#19 Posted by: Wraith Posted at: 2018-08-09T13:04:52.337Z Reads: 338

```
That would be so cool to have! Lets you get the range from those bigger packs without having to worry about building the board around it and its handy to have!

I’m keen on seeing how that goes! Its a wonder why like you mentioned, nobody is posting about these things :laughing:
```

---
## \#20 Posted by: amazingdave Posted at: 2018-08-09T13:07:43.207Z Reads: 333

```
I wonder what the efficiency losses are with the charging through a buck converter method, must be well over 10% at a guess... anyone do better than guess work?
```

---
## \#21 Posted by: TinnieSinker Posted at: 2018-08-09T13:09:08.569Z Reads: 300

```
yea great idea, I couldn't find any threads about it so yea I can make one as I build and test.

it's so hard to fit a huge pack into a board so having an auxilery would be great
```

---
## \#22 Posted by: Wraith Posted at: 2018-08-09T13:11:11.057Z Reads: 294

```
Yeah something you can take along in a pack when you expect to ride hard or go longer distances.

Would be ideal to have them well enclosed if worst case you wipe out with them connected or on your pack.

Edit:
Just remembered there are some lipo bags that could be used for this purpose while carrying it around
```

---
## \#23 Posted by: DeathByBacon Posted at: 2018-08-09T13:15:01.858Z Reads: 293

```
I don't think charging while riding is advisable. 

I've played resource intensive games on my mobile phone while charging and the battery can get pretty hot. I can only imagine how it is like in  a bigger scale like esk8s. I'm no expert though so I could be wrong.

Although a "powerbank" for esk8s would be really cool and useful though.
```

---
## \#24 Posted by: Skunk Posted at: 2018-08-09T13:15:21.865Z Reads: 286

```
They paved an Old Logging railroad track and turn it into a bike path that goes out around and past a lake just outside of my town. Tons of camping spots out there. Would be great to ride out, stay the night and ride back.
```

---
## \#25 Posted by: TinnieSinker Posted at: 2018-08-09T13:16:14.969Z Reads: 280

```
can't be much worse than regenerative braking?
```

---
## \#26 Posted by: Wraith Posted at: 2018-08-09T13:16:27.954Z Reads: 284

```
Would love to pick a few up once you iron it all out! 

I want that 60 cell performance but I dont have space for the deck and vescs 😅
```

---
## \#27 Posted by: DeathByBacon Posted at: 2018-08-09T13:25:23.414Z Reads: 293

```
To be honest, I really don't know. The idea just popped in my head while reading your comment as I was charging while playing earlier with my phone and how the back panel really got hot. And that's just using a 5v 1-2amp phone charger. Probably also the reason that's why nobody has made a thread about doing it.

I hope the experts in the forum can chime in. I so want to be wrong though. Charging while riding could be a game changer. But safety first.
```

---
## \#28 Posted by: Skunk Posted at: 2018-08-09T13:29:22.573Z Reads: 283

```
the guys from corridor did it with a onewheel but he's yet to really do a recap or a review after more testing. 
https://youtu.be/tbqWFVm9cD0
```

---
## \#29 Posted by: Skunk Posted at: 2018-08-09T13:43:03.773Z Reads: 284

```
I want a action 360 camera so bad. 
His friend is terrible....
```

---
## \#30 Posted by: TinnieSinker Posted at: 2018-08-09T13:43:37.035Z Reads: 288

```
I don't know either haha definitely some testing to be done. @amazingdave efficiency testing as well. Ideally the volts would be the same.

is has been done, just no threads on how and if there are problems

a friend found these on an evolve forum
![38216645_10156540121272442_783782212410540032_n|375x500](upload://fYOd86780xYxjs48dRURdSVVDbo.jpg)![38412059_10156542091487442_6909721786414268416_n|666x500](upload://fFiUmCeda2ykkHBNhFW4gMrTqTA.jpg)
```

---
## \#31 Posted by: skatardude10 Posted at: 2018-08-14T15:47:27.689Z Reads: 264

```
I'd like to give this a try... My commute to work leaves me with very little headroom on my 10S4P battery, and it would be great to be able to plug in an external battery while I'm riding to keep charged a little more. Anyone that has done this I'd love to hear about your experience.
```

---
## \#32 Posted by: marsrover001 Posted at: 2018-08-14T18:00:20.174Z Reads: 261

```
Oh. I can actually offer useful advice here. I've done charge and ride both on a onewheel and an eboard multiple times. They use the same hardware, big lipo battery and a boost converter. 

Not sure what to say about it though. It works. Better acceleration when the battery is low and charging. Better range. Sits either in your backpack or between your legs. Didn't notice extra heat or wear, so I'd recommend it fully.

Tried to find pictures, but I guess they were all Instagram stories.
```

---
## \#33 Posted by: amazingdave Posted at: 2018-08-14T18:29:58.631Z Reads: 253

```
Which boost converter do you use?
```

---
## \#34 Posted by: marsrover001 Posted at: 2018-08-14T18:38:49.310Z Reads: 254

```
The green one on Amazon. Can't remember the name as I'm at work. but it's got a screen and let's you set all the features. Was about $40
```

---
## \#35 Posted by: Schulerbible Posted at: 2018-08-14T22:21:47.449Z Reads: 249

```
We have a couple of these in Sydney and currently on the way to replicate them. The price people pay for these is ridiculous since only about $200-240 in materials is used. Circuit is pretty simple, they use a lipo low voltage indicator too. Here is a quick drawing![image|690x101](upload://gjKpSbELJ4BkUd8WWHl2tVL7P7P.jpeg)
```

---
## \#36 Posted by: TinnieSinker Posted at: 2018-08-15T03:15:09.787Z Reads: 249

```
coooool, good to hear they're around and working!

Im thinking of building one with some large car batteries to use as portable fast chargers. couple AT boards at a big park, BBQ and riding all day woop woop
```

---
## \#37 Posted by: skatardude10 Posted at: 2018-08-15T06:07:36.444Z Reads: 246

```
I am in between a small pack I can clip to the middle of my board such as [this 7S2P](http://www.diyeboard.com/7s2p-lg-18650-lithiumion-battery-pack-294v-4400mah-11088wh-p-457.html) that will be *enough* to get me where I need to go... or if I should just go all in and have the option for [this 10S5P with enclosure](http://www.diyeboard.com/10s5p-360wh-18650-battery-power-kit-with-bmscharger-enclosure-p-656.html) that I could also strap onto the top of my deck, [stuff this thing inside](https://www.amazon.com/DROK-Numerical-Regulator-Converter-Adjustable/dp/B01GFVI6R6/ref=cm_cr_arp_d_product_top?ie=UTF8), and basically double my range instead of adding less than a quarter of my current range (1.25x instead of 2x the current watthours) with the 7S... and be able to not only get where I need to go but have waayyyy enough wiggle room to cruise the extra long routes back and forth.

I was originally looking at purchasing a BMS, wire, connectors, cases, a boost converter, individual cells, and DIYing the whole thing, but it looks like I can get a lot more cells with a built in BMS going the pre-made route.  This way, all I have to do is connect the pack to a boost converter, program the boost converter, mount it, and plug it in when I want the extra range. 

The advantage I saw of putting my own together from scratch was the performance from quality cells. But, the fact that this will just be drawing a relatively small continuous current, and not directly affecting the boards performance... only supplementing it, I don't really care about having super high quality cells... only capacity.

I would really really love to supplement my current 10S4P with a 10S5P battery to charge while riding. I wonder how close this would be to basically having a 10S8P or 10S9P battery- hopefully somewhat comparable for range, but im going to assume surely not alike for pure amp draw potential of a 10S9P.
```

---
## \#38 Posted by: skatardude10 Posted at: 2018-08-15T17:41:51.162Z Reads: 245

```
I am sold now. Picked up the boost converter, a range of high voltage fuses with various amp ratings and fuse holders... 

Hesitant to order batteries from China, I checked out Lowe's. I didn't expect to find much in terms of price competitiveness, but the portable power tool batteries are actually priced equal to or better than the Chinese batteries per watt hour! 

![20180815_103226|690x335](upload://3rfnwaABVLHd54T0SdkxpaJbvr4.jpg)![20180815_103245|690x335](upload://mb36fTaiAIXoN4QyrTWd4RE8iWD.jpg)

Two of these batteries comes out to 192 watt hours. Add in the quick charger and the price comes out to be cheaper than a "LG/Samsung" 6S4P 211 watt hour battery without charger from China. Not only is it cheaper, I can design it to be 100% modular with 3D printed mounts / boost converter enclosure that all just snaps onto the board... plug and play additional batteries as needed, carry extras in the backpack to hotswap on the road. Sounds so nice! Plus no shipping cost to save $35, and get them today 😎 

I see a fun project on the horizon.
```

---
## \#39 Posted by: skatardude10 Posted at: 2018-08-19T01:55:52.300Z Reads: 237

```
I don't know if it's something I did wrong, or if the converter I got was faulty... But it died on me after an hour of charging- screen flickering, power output ceased, unit got very hot, fan turned on and turned off... Now it's dead. My excitement is dampened. [This is the one](https://www.amazon.com/gp/aw/d/B01GFVI6R6) I got. It was great, charged really fast at 5A when it was working.... Got my board from 30 to 60% in relatively little time compared to my standard 2A brick charger. 

I'm swapping it for [a new one](https://www.amazon.com/gp/aw/d/B076ZJX1YZ) now... Hopefully this one doesn't just die on me... With the slightly reduced range on my pneumatics, I really could use the extra range now. I'm still trying to think of a clever way to mount the unit and battery holder to my board, rather than just clipping it to the top... But I'll probably just keep it clipped to the top. Maybe I'll go for a rear mount to keep it out of the way. Having clip on extra range will be great, I'll keep dreaming for now until one of these boost converters actually works.
```

---
## \#40 Posted by: pat.speed Posted at: 2018-08-19T02:08:51.273Z Reads: 242

```
I can vouch for this charger, I use it to charge my 12s build at about 3-5 amps with an input of 24v.



https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com.au%2Fulk%2Fitm%2F142869845961

This is making me want to buy a 6s lipo
```

---
## \#41 Posted by: skatardude10 Posted at: 2018-08-20T06:23:33.493Z Reads: 247

```
Unfortunately I already ordered another one. If these things in general are as finicky as the first one I got and the second different kind kicks the can, I will definitely be going off your word and picking that one up. Thanks for the recommendation!

As for the one that is coming in the mail tomorrow, I drew up a rear mounted battery / boost converter holder that integrates with my steering damper in the rear. I tried just plopping the various designs together, but I ended up starting from scratch. Pics posted [in the pics no words thread](https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/6540?u=skatardude10), but i'll post them again here since this is more the topic for it. 

I designed the boost converter enclosure to be modular, to slide on and off as needed... and I will probably use some 3.5mm bullet connectors to hook it all up so I can keep the battery clip installed and wired up... and if I need to try the boost converter you suggested then I can draw up a new enclosure with the same attachment, print, wire it up, solder bullet connectors to the new converter, pop it on the pack of the board and just plug it in without having to re-print *eeevveeerrrryyythinnnggg*.

![20180819_234227|690x335](upload://xdt11OTb3qMgD2OJ0Z142LWi0Nt.jpg)![20180819_234155|690x335](upload://9nMhBKL2E18ns8GVcyskqf7ULCx.jpg)![Battery_and_Boost_Converter_Mount_2018-Aug-20_05-18-05AM-000_CustomizedView25775353744_png|690x381](upload://LrglptaKhD7WdsSdBDvmzXmBzn.jpg)![Battery%20and%20Boost%20Converter%20Holding%20Riser%202|684x500](upload://b9HxQXYmf8sjLm0rotYTFqL7ZS2.jpg)![Battery_and_Boost_Converter_Mount_2018-Aug-20_05-18-29AM-000_CustomizedView20199872276_png|690x381](upload://xmboOHwRQoca0TkoK57AqkpXYg6.jpg)![Battery_and_Boost_Converter_Mount_2018-Aug-20_05-23-38AM-000_CustomizedView15816063827_png|690x381](upload://y3lQJ08BuhLBCikCyV1H41Smvvc.jpg)![Battery_and_Boost_Converter_Mount_2018-Aug-20_05-19-43AM-000_CustomizedView19271978252_png|690x381](upload://nLY1V8msGoxaL48xExBhxkkPdAk.jpg)![Battery_and_Boost_Converter_Mount_2018-Aug-20_05-20-14AM-000_CustomizedView10983910333_png|690x381](upload://xI7ZL5DEnuV1YNdjrjdZGaAQG3L.jpg)![Battery%20and%20Boost%20Converter%20Holding%20Riser|582x499](upload://nEedZBNjzrtzngZyzbAYS9ktgn3.jpg)![Battery_and_Boost_Converter_Mount_2018-Aug-20_05-19-18AM-000_CustomizedView15659169258_png|690x381](upload://21FDU2WTm2NTGKTBCDpYnnk4JrM.jpg)
```

---
## \#42 Posted by: skatardude10 Posted at: 2018-08-24T00:18:04.436Z Reads: 239

```
Okay, burnt out my second boost converter. I think third time will be the key. Made an anti spark switch, no more Sparks... Gonna draw up and print an enclosure for this new boost converter. This thing looks well soldered, and is quite hefty. Thanks for the suggestion @pat.speed. also picked up a watt meter per pats suggestion. ![20180823_173310|690x335](upload://djQ7Ga0OXWGQQ23lGRYM77lVkEo.jpg)![20180823_173336|690x335](upload://7RL4PyAPjlNbs1PSQXYbNDHWZnD.jpg)

Edit 1:

Wired up to test and working mmmmmm!!! Voltages and amp outputs of the meter are accurate enough 😬😎

![20180823_195821|690x335](upload://975g4lZyTqSG3UIg2MxH4hybwJ9.jpg)

Edit 2: After some testing, first 4AH battery charged my 10AH battery by about 30%. If second battery charges to 70% before empty... The math in my head says this boost process is about 70% efficient... And I am totally good with that .. it will get me back uphill and home from work with greater than 1% battery to spare,which is all I need. I am a happy camper at the moment, none of the wires are overheating and everything seems to work well now. 

If anyone in the US is curious, these are the two things I ordered for this from Amazon:. [Boost converter...](https://www.amazon.com/gp/aw/d/B01MG4211N?psc=1&ref=yo_pop_mb_pd_title) and [this fairly accurate enough watt meter](https://www.amazon.com/gp/aw/d/B01LVTST80?psc=1&ref=yo_pop_mb_pd_title).

Now to draw up the final enclosure and dye everything black.
```

---
## \#43 Posted by: skatardude10 Posted at: 2018-08-25T06:13:32.478Z Reads: 238

```
Got it all hooked up and working! Now I just gotta cable manage a bit... 

Okay, here's a photo vlog: 

![20180823_173310|690x335](upload://djQ7Ga0OXWGQQ23lGRYM77lVkEo.jpg)

![20180824_213134|690x335](upload://bYinbFiHftRFQYPNofn8CvGRWoo.jpg)

![20180824_214921|690x335](upload://7msT2RWg8JmrAcroyQiJIQGRYJU.jpg)

![20180824_220338|690x335](upload://8qxrOrZ4lXmDeRsNv3owBmec7CD.jpg)

![20180824_220428|690x335](upload://dvNtHy0TEM43NT5r97OshukS0O4.jpg)

![20180824_225236|690x335](upload://em7SEfDpaFAXm76xEV25eADgLMr.jpg)

![20180824_225800|690x335](upload://n0l6WqbgQaKml6Kgn2N7GAHFxa3.jpg)

![20180824_230550|690x335](upload://tffEUQGrELPAjf8SDE8BGQia0fT.jpg)

![20180824_231328|690x335](upload://yWShjxQRyVIVbw6IAouaoIFfMwr.jpg)

![20180824_231540|690x335](upload://wGqQD7ze0GTwTh428RgHnZNB0rq.jpg)

![20180824_232650|690x335](upload://19n3bKcswuBUmiNV3xZckXjp4ed.jpg)

![20180825_000159|690x335](upload://f96DrRo1KGMGANU3FfQlTMMaUHs.jpg)

![20180825_000212|690x335](upload://3ixxd5Mm8mUin7JO1XKbMN8kIaS.jpg)

![20180825_000456|243x500](upload://62StJrEehlGJLTGzTUVvp4WOqIo.jpg)

![20180825_000514|690x335](upload://t4z9OtBjU5UYvlOt76aKw02OSwd.jpg)

I'll probably update when I get the cable management down.
```

---
## \#44 Posted by: TinnieSinker Posted at: 2018-08-25T06:54:18.186Z Reads: 216

```
nice one! How did you mount the boost converter with the heat sink poking out?

I have mine on the bench testing at the moment, same parts but with a lipo. so far its good
```

---
## \#45 Posted by: skatardude10 Posted at: 2018-08-25T07:05:44.741Z Reads: 222

```
The heatsink mounts to the boost converter on the four corners of the PCB, with four 6mm tall spacers between the heatsink and PCB. I thought this would be a great place to mount everything, in place of those spacers to print a Nylon shell for the PCB, with a cutout in the bottom of the shell for the PCB to make contact with the heatsink, and just let the heatsink hang loose out the bottom (I've since secured it to the deck as an additional point of strength for mounting the entire assembly. 

Anyways... Here are some pics of the cable management. I ended up running the charge cable under the lips of my enclosure... And the charge port when not in use just wedges securely under the battery enclosure lip... Totally didn't plan on doing it this way (I had no plans, just winging it).

And a little video of hooking it up as if I were on the road... Such a satisfying click.

![20180825_005438|690x335](upload://33aVVg3lGCFPnNEHceTOIRRfI7Y.jpg)![20180825_005312|690x335](upload://wG7HrjGWtolXYw2qkwiXaCWG7VB.jpg)![20180825_005428|690x335](upload://9QflU2seiQuVC18q3SYHFRGDPa9.jpg)
![20180825_011236|690x335](upload://nuTHECyGmaGvYEpfI4Ih3MB9pOf.jpg)![20180825_011217|243x500](upload://wJ1EBUGny6QqPyDahT9bzHbpPBi.jpg)![20180825_011151|690x335](upload://3NYpc9ZKjrjHIeH6g8JtAwUJYqq.jpg)

https://youtu.be/BmLwvZJj7ac
```

---
## \#46 Posted by: skatardude10 Posted at: 2018-08-26T01:00:41.057Z Reads: 201

```
Got to try this out today. Two batteries, each drained half way... After 4.5 miles only dropped from ~39v to ~38v with 4P 25r charging at around 3.5-4A... the board meter reading somewhere around 80-85%, down to 75% when I got home. This was all while riding my higher power mode pushing 80A battery max with sligly reduced 16A battery min to compensate for the additional continuous charging. 

I also notice a volt or two less voltage drop in the higher power modes, and it just feels noticably snappier for the voltage I was riding at. 

I thought I would attach the batteries when I needed the extra range, I think I'll probably just ride with the batteries all the time now. 

I need to make a few changes: E6000 to protect the electronics from bumps and vibration, hot glue to better secure the ingoing and outgoing wires to the boost module and for better water sealing around the edges of the boost module enclosure. Also, I need to solder on an extension to the negative output wire from the boost module- it's just a tad too short for comfort at the moment.
```

---
## \#47 Posted by: AutoCar Posted at: 2018-08-26T01:04:23.168Z Reads: 191

```
Sorry for bothering you. I just joined this group. How can i post? It does not seem to have any link for post new topic...
```

---
## \#48 Posted by: skatardude10 Posted at: 2018-08-26T01:05:24.992Z Reads: 187

```
Huh, for me there is a new topic button on the main forum page. 

Maybe for new users there is a limitation until you have so many posts or something.
```

---
## \#49 Posted by: pat.speed Posted at: 2018-08-26T10:56:53.122Z Reads: 185

```
Yeah you need to have a certain amount of time on the forum I’m pretty sure, let’s delete these posts after a day as to not clutter this awesome thread
```

---
## \#50 Posted by: DeathByBacon Posted at: 2018-09-12T09:56:19.080Z Reads: 172

```
Cool! Does this just plugin directly to your charging port?
```

---
## \#51 Posted by: amazingdave Posted at: 2018-09-12T10:38:53.109Z Reads: 174

```
Yes it does...
```

---
## \#52 Posted by: DeathByBacon Posted at: 2018-09-14T18:52:33.218Z Reads: 177

```
So 6s is the minimum battery config to use for this, is there any advantage in using a higher config say, 10s? 

And how efficient is it when used while riding? If you have 10% battery left and you plug it in, will it be able to charge it fast enough for the battery not to get empty while you continue to ride?
```

---
## \#53 Posted by: Pedrodemio Posted at: 2018-09-14T19:45:13.382Z Reads: 178

```
The problem with 10S is that you would need a DC-DC converter that can step-up and step-down, they exist, but are harder to find

To make simple and only use a step-up the minimum skate battery voltage should be higher than the maximum battery booster voltage with some margin between the two

10S fully discharged = 28~30V
6S fully charged = 25.2V
7S fully charged = 29.4
```

---
## \#54 Posted by: mynamesmatt Posted at: 2018-09-28T04:30:16.859Z Reads: 170

```
wouldn't plugging into the loop key blow something up? the loop key completes the circuit on one rail whether it be positive or negative. if you added another battery it'd essentially need another antispark. wouldn't it?
```

---
## \#55 Posted by: TinnieSinker Posted at: 2018-09-28T11:01:08.522Z Reads: 173

```
it will definitely blow up :flushed: 

we're using boost converters to charge through the charge port while riding.
```

---
## \#56 Posted by: mynamesmatt Posted at: 2018-09-28T11:21:08.583Z Reads: 181

```
![jpg_1538101931103|257x500](upload://7Xga5kI0DK5SbHhIE6K6uAfKsOk.jpeg)
yep just got mine
```

---
## \#57 Posted by: amazingdave Posted at: 2018-09-28T11:23:02.090Z Reads: 171

```
If you plug in a 2s battery with the same spec and state of charge as your 10s to expand your pack from 10s to 12s  with an antispark connector and changing your vesc settings to suit the new 12s configuration then no problem. (The long battery leads may make for their own problems with regards to blowing up your vesc). 

The much more elegant solution as far as I understand it is with the boost converter and charge port. This is the method I’m going for.
```

---
## \#58 Posted by: visnu777 Posted at: 2018-10-06T17:54:17.749Z Reads: 167

```
I did just that, plugged in a 2s lipo into my loopkey connector (with an antispark XT-90s of course) and It worked like a charm. 10s works great for me most of the time but sometimes I want a little extra power, eg. climbing steep passages. I just tested it for some minutes today, I'll drive around more tomorrow and keep you updated :) Btw, it was even FOC with a FSESC 4.12 (oh my :D)
One thing: I thought it would be a good idea to put a lipo low voltage alarm with the booster pack. Strangely the alarm went off just after driving some minutes. It calmed down when I unplugged the XT-90s from my board and when I measured voltage I got 8.3V, so the question is: Why did the alarm go off?
```

---
## \#59 Posted by: amazingdave Posted at: 2018-10-06T18:35:12.605Z Reads: 160

```
What voltage did you have the alarm set to?
```

---
## \#60 Posted by: visnu777 Posted at: 2018-10-06T18:40:03.011Z Reads: 166

```
The alarm is fixed to 3.3V according to Hobbyking https://hobbyking.com/de_de/hobbykingtmlipoly-low-voltage-alarm-2s-3s.html
I have it so I can simply unplug the booster when its too low. Later I want to add a similar thing to my liion pack.
```

---
## \#61 Posted by: Pedrodemio Posted at: 2018-10-06T18:51:47.198Z Reads: 155

```
Also don't forget that if you don't change the battery cut off on the VESC you can over discharge the batteries
```

---
## \#62 Posted by: visnu777 Posted at: 2018-10-06T18:52:28.908Z Reads: 149

```
That's why I tried the alarm thing ;)
```

---
## \#63 Posted by: amazingdave Posted at: 2018-10-06T18:55:26.922Z Reads: 153

```
This is the type I’ve always used... adjustable alarm voltage....

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F253530303509
```

---
## \#64 Posted by: Pedrodemio Posted at: 2018-10-06T18:56:20.543Z Reads: 149

```
Assuming that the capacity of the booster is identical or lower per P group of the main pack you should be good, if it's higher than the main pack you can still have energy left on the booster and over discharge the main pack
```

---
## \#65 Posted by: visnu777 Posted at: 2018-10-06T19:00:18.346Z Reads: 153

```
OK, so basically it should work as long I watch both packs for over discharge?
My battery is a 10s3p vtc6 pack with 9.3Ah, the lipo is a 2s 8Ah zippy.
```

---
## \#66 Posted by: Pedrodemio Posted at: 2018-10-06T20:37:46.207Z Reads: 158

```
Exactly, but with this mixed setup you will need to pay even closer attention

The lowest you should go with the Lipo is 3.5~3.6 V, but the 18650 you can go between 2.8~3 V
```

---
## \#67 Posted by: visnu777 Posted at: 2018-10-07T11:09:59.615Z Reads: 168

```
Yesterdays prototype:
![booster_prototyp|499x500](upload://e2aLr07ebaJVG4nWlQp4BugLdMs.jpeg) 

It was working but is way too bulky (I used an old external harddrive case) so since it rained today I build a better one out of spare kydex:
First you have to build some shape out of wood or similar:
 ![kydex_1|685x500](upload://wYSlWo2zo1yxhsTv3vSCEWQygis.jpeg) 
Then you heat up the kydex in an oven (150°C) for some minutes until it becomes soft. This soft mat has to be placed quickly on top of your shape and then you use some foam and wood to press it as good as possible onto the shape. If its not perfect its not that bad, you can always use a heatgun to make it soft again and improve it punctually (foam plus wood and press)
 ![kydex_2|556x500](upload://tOnODyWMQMK2aeTSlHKxwGTj12i.jpeg)
After some time it looks like this (actually I already cut the outer shape with a saw on the picture)
 ![kydex_3|690x460](upload://x3u2W3r2mCp4pKGcZsG8TZG3Ixr.jpeg)
I then placed the lipo in it (using neoprene for insulation and less vibrations), put a cut out plain piece of kydex on top and hotglued it together
![kydex_4|690x459](upload://5b8R436x9KU5SEl2YPnI4CPmwJt.jpeg)
![kydex_5|690x460](upload://kPFTkJCgcDhYGbZSfD0FSKe3RLI.jpeg) 
The Lipo discharge warner fits perfectly:
![kydex_warner|690x460](upload://ufCMSYTV2vu7bKCsNFc2wiSn2id.jpeg) 
Complete build, now you see why I put in the higher spots ;)
![kydex_complete|690x460](upload://wPPAaN9SJUXwyKlxY2gySuUi8UR.jpeg)

btw, the warner got loose yesterday, I'm almost sure that todays test will be more successful :)
```

---
## \#68 Posted by: visnu777 Posted at: 2018-10-08T19:08:00.030Z Reads: 150

```
Update: It works perfectly, I'm not sure if I want 10s all the time so the booster is a nice way of having the extra power when I want it :)
```

---
## \#69 Posted by: danieloath Posted at: 2018-10-14T10:26:55.901Z Reads: 145

```
The tool batteries have their own internal BMS with low-voltage cutoff, correct? This would eliminate the need for a low-voltage alarm and manual disconnect, right?
```

---
## \#70 Posted by: b264 Posted at: 2018-10-14T22:36:19.397Z Reads: 144

```
@amazingdave I think you should change the title on this thread so the word “loopkey” is not in it. This is dangerous and they way it's being done isn’t what the initial title suggested. I think you're using the charge port, right?
```

---
## \#71 Posted by: mmaner Posted at: 2018-10-14T23:00:53.717Z Reads: 146

```
This ⬆️

We should all attempt to be clear on topic titles. In this case I'd hate for a 14 year old to plug a lipo into the loop key because he failed to read.
```

---
## \#72 Posted by: Skunk Posted at: 2018-10-14T23:02:33.839Z Reads: 143

```
You know damn well there plenty of adults on here that dont read too.
```

---
## \#73 Posted by: mmaner Posted at: 2018-10-14T23:03:50.056Z Reads: 142

```
Yeah, I know a few... @Skunk, I mean I've even talked privately with a few @Skunk.  I wonder if I should name names @Skunk.  😀
```

---
## \#74 Posted by: Skunk Posted at: 2018-10-14T23:06:12.977Z Reads: 146

```
My problem is i read to much so nothing sticks lol 
Oversaturation
```

---
## \#75 Posted by: skatardude10 Posted at: 2018-10-15T00:54:54.490Z Reads: 148

```
![20181014_185417|690x335](upload://nkoBkLvShfrj2J6bi7TbtQjnFE7.jpeg) ![20181014_185400|690x335](upload://swUuI3natkiTPyB8njj7ORI5TXg.jpeg)
```

---
## \#76 Posted by: mmaner Posted at: 2018-10-15T01:53:56.076Z Reads: 139

```
I went ahead and changed it, looks like the op hasn't been on in a few days.
```

---
## \#77 Posted by: lrdesigns Posted at: 2018-10-15T01:56:03.632Z Reads: 137

```
This thread all ways did my head in, I was like how can this work?? Then it got cleared up and made sense. Over the weekend I was thinking, we should really change the title of this  thread. !! I can sleep soundly now.
```

---
## \#78 Posted by: mmaner Posted at: 2018-10-15T01:57:15.842Z Reads: 139

```
Yeah me too.  I've been worried for days that someone was gonna plug a lipo in their loop key port just to see if it worked 😀
```

---
## \#79 Posted by: visnu777 Posted at: 2018-10-15T02:35:46.045Z Reads: 140

```
when you take care of

* polarity (has to be in series with your main battery of course)
* that both batteries never get drained below cutoff
* use xt90s as connector to prevent the spark

it works fine.
```

---
## \#80 Posted by: lrdesigns Posted at: 2018-10-15T03:21:08.932Z Reads: 139

```
OK. But that is more of a voltage booster than range extender. So slightly different topic. Also I'm on 12s, so I can't just add more series voltage with current vesc hardware.  Its a cool idea though, you could have a 6s / 12s build for slow and fast versions. Id want to be able to change vesc settings by bluetooth for this though.
```

---
## \#81 Posted by: TinnieSinker Posted at: 2018-10-15T03:50:11.212Z Reads: 132

```
And if you could switch between 6s X2 in parallel and series for 12s for range or speed, that'd be cool
```

---
## \#82 Posted by: visnu777 Posted at: 2018-10-15T04:13:15.602Z Reads: 136

```
The problem is: if both batteries get drained differently the vesc doesn't know about that, it just has the overall cutoff. That's why I used the lipo voltage warner and will also build something similar for the main battery ;)
```

---
## \#83 Posted by: skatardude10 Posted at: 2018-10-15T04:48:34.252Z Reads: 149

```
![20181014_224641|690x335](upload://kBmVAxtF32snxrmYkryLxf8VcUn.jpeg) ![20181014_224726|690x335](upload://bYuBqSN1E85arvz2UlBdxLA1aci.jpeg) ![20181014_222000|690x335](upload://tEmwSgO8wAdA1Qx5dhJM2o8Bg7F.jpeg) ![20181014_221832|690x335](upload://WNzxAQ6KBWOIdFySsTv2kaa73P.jpeg) ![20181014_221950|690x335](upload://ohsEMcQF9IwxRC5QG1TkQCmQOey.jpeg) ![20181014_221825|690x335](upload://rICgf83U3wbzgvj8XIr7VA18Gfg.jpeg)

Fits in my backpack well and having the cord come out of the right side with the cable retractor connected towards the plug seems to work well too for keeping the cable out of the tires when crouched. My wife says it looks stupid so I'm not going to try to get pics. I'll probably only use it when I really need it.
```

---
## \#84 Posted by: amazingdave Posted at: 2018-10-15T06:15:09.702Z Reads: 137

```
I take your point on changing the title, though the original intent was to directly plug a matched 2s battery into the loopkey of my 10s to make a series connected 12s....

This does work but is a shitty and inelegant workaround that if misunderstood could blow some shit up. 

The boost converter through charge port is the way I’m headed now.

Thanks @mmaner I missed the posts till now.
```

---
## \#85 Posted by: TowerCrisis Posted at: 2018-10-15T06:24:04.588Z Reads: 132

```
[quote="lrdesigns, post:80, topic:64327"]
But that is more of a voltage booster than range extender.
[/quote]
Those are one and the same. Increasing voltage, OR increasing amp hours will increase your range. What actually determines range is the watt-hour rating of the battery which is voltage times amp hours.

People have probably seen people describe their boards as "consuming x amount of watt hours per mile" because that's a universal range rating. As long as you know the Wh/mi, the voltage, and the amp hours, you can know the exact range.
```

---
## \#86 Posted by: lrdesigns Posted at: 2018-10-15T06:28:51.554Z Reads: 129

```
I get that, but as the example above. You have a 10s pack, then add 2s to the loop key. You can only add a similar capacity size battery as they have to drain evenly. Its not much watt hours you can add. 

But if you connect to the charge port you can add any size watt hour battery.
```

---
## \#87 Posted by: TowerCrisis Posted at: 2018-10-15T06:32:47.092Z Reads: 125

```
I'd just like to point out that a battery connected to a loop key port connected in series with the battery is probably MUCH safer than a battery hooked up to a charge port. On a charge port you need to worry about using a boost converter, and worry about unequal discharge of the packs (your boost converter will need to have a low input voltage cutoff)

By connecting pack in series with the loop key port, you only need to worry about three things:
1. Your vesc being tuned to have min / max voltages that account for the voltage boost
2. Your packs starting at relatively the same capacity (just have a little headroom in the low voltage cutoff)
3. Making sure your boost pack has the same rated amp hour rating as your main pack.

As long as you follow those three rules, there is no additional risk (besides having another battery outside of an enclosure, but the charge port method also suffers from this)

On a separate note: Yes, @lrdesigns you're right about the capacity limit. You should not exceed 12S, so you can only boost voltage so much. But for boards that are running on 8S or less, this is a great method.
```

---
## \#88 Posted by: Pedrodemio Posted at: 2018-10-15T12:05:20.875Z Reads: 121

```
[quote="TowerCrisis, post:87, topic:64327"]
Making sure your boost pack has the same rated amp hour rating as your main pack.
[/quote]

That’s not enough, only if use the same cell that was subject to a similar load across its life 

Internal resistance changes a lot, they can have the same capacity and still discharge at different rates 

That’s why is never recommended to mix new and used batteries 

But do like @visnu777 and monitor both internal and external packs and you should be good
```

---
## \#89 Posted by: skatardude10 Posted at: 2018-10-15T22:21:48.706Z Reads: 123

```
Huh... I like the title change, but realized maybe this whole topic could just be range extenders speed boosters or something along those lines. But the title isn't a big deal, it's pretty fitting ATM. 

Now that we are talking the difference between plugging into the charge port vs loop key (or maybe now that I've started paying attention), it seems like both have benefits. 

I want to figure out a way to keep my range extender plugged into the charge port, and also have the option to plug in a speed booster into the loopkey port. I am thinking since the loopkey speed booster isn't connected to the BMS, and won't be extended by the charger (right?) that it could safely be 1-2P larger than the rest of the pack, or even double, to ensure that it won't die when the rest of your pack is being charged. Or, would the pack plugged in after the BMS still be charged with the rest of the pack, just not balanced? Then again, all this is making me want to just build a 12-13s 8-9p pack and be done with it.
```

---
## \#90 Posted by: TowerCrisis Posted at: 2018-10-15T22:23:15.611Z Reads: 113

```
Hence why I said leave some headroom on the low voltage cutoff
```

---
## \#91 Posted by: skatardude10 Posted at: 2018-10-15T22:27:55.407Z Reads: 122

```
I'm merging conversations here, but headroom for however many S in voltage you are boosting with... ?

I'm going on my third beer, doesnt this defeat the purpose to begin with? I do get this makes sense with differing internal resistance though. Forgive me for combining conversations... I'm asking if you are charging your main pack and not your voltage boosting pack at the same time.
```

---
## \#92 Posted by: TowerCrisis Posted at: 2018-10-15T22:30:16.092Z Reads: 122

```
I'm not saying that much, probably 10% of the total pack capacity including the booster would be fine.

Ideally, just stick an RC low voltage chirper on the booster pack.
```

---
## \#93 Posted by: skatardude10 Posted at: 2018-11-01T01:12:54.907Z Reads: 123

```
Before I go forward, I want to get the community's thoughts on my plans to see if there are any blatant issues or dangers with what I want to do. I want to do the original range extender this thread was based on (but as a voltage/speed booster) plugged into a loop key, in addition to my current range extender plugged into the charge port. 

My current 24v power tool battery swapping mechanism to boost converter (42v 5a) plugged into the charge port works great for my 10S4P 25r 10Ah battery... And I intend to keep this at the same time as having the voltage boost option in the loopkey... I'm assuming this will be fine, charging 10S at 42V while boosting the output of all that with another 2S pack that's not being charged.

Now, I want to splice a loop key into the red wire that leaves the pack and plug either a loop key or a 2S18P pack of Samsung 30A (6a discharge / charge = 108A, need so many P to not stress the cells and provide at least 80A to match the rest of my 10S4P packs max output) It would be a 45Ah pack based on my testing of each cell. 

I would maintain 10S voltage cutoffs and just keep an eye on my 10S batteries voltage via the % lcd on the pack and my power tool range extender's voltage monitor connected to the 10S pack, and rely on the BMS cutoffs as a fallback if those fail me somehow or I get blackout lazy for some reason (not expecting this...)

I would monitor the voltage/% of the 2S18P voltage boosting loopkey pack separately with another external voltage display, and being 45Ah I don't anticipate it draining even half before I can fully recharge my main battery with all the external batteries I have. This I think will have the benefit of not needing to charge the "speed boost" pack as much and/or maintain a higher voltage slightly for the duration of my rides. 

For charging, I don't intend to use any kind of BMS, instead have two barrel connectors, or 3/4 bullet connectors and just connect these to contacts in a 3d printed 18650 sized shell that I will simply slot into an 18650 charger to charge the whole pack at 2amps. I'd expect this to take forever, but I'm not trying to buy a fast 4.2/8.4v charger /2S 80A BMS.

Since all the 30A cells are spot welded in 3p groups, I was going to connect 6x 3P groups with 14awg silicone wire, soldered to the nickel strips, and solder 10awg wire for the positive and ground to the entire pack and to connect between the two large P groups. 
 
The idea is that I can carry this pack in a padded 3D printed case that I can clip onto the top of my board, disconnect the antispark loopkey and plug in this pack to the same port to instantly boost from 10S to 12S when someone wants to race or something. Do you all see any issues with any of this? I'm curious how well this will work, or if it will work at all.
```

---
## \#94 Posted by: AlexBE Posted at: 2018-11-28T07:30:18.689Z Reads: 106

```
As convoluted and crazy as all that is, I'm pretty sure it will all work.
```

---
## \#95 Posted by: skatardude10 Posted at: 2018-12-18T20:23:32.753Z Reads: 112

```
In the spirit of the original post on this thread, I've decided to make a 1S voltage boosting pack to get a tad bit higher top speed and maybe a bit more range while I'm at it. I've documented the build here: https://www.electric-skateboard.builders/t/the-demonseed-tb-218-tb-6374s-190kv-tb-mounts-chibattery-10s4p-dual-focboxes-superflys/50610/99?u=skatardude10

Bench tested it and it works great. The extra voltage makes my board sound mean and scary. Ahh!! Glad I didn't boost to 12S, I like my gearing and speed where it's at.
```

---
## \#96 Posted by: b264 Posted at: 2018-12-18T20:25:25.838Z Reads: 108

```
Boosting voltage this way, instead of capacity, is very dangerous.

I hope you have some way to verify the packs are balanced and know if any P-group falls below a cutoff voltage.
```

---
## \#97 Posted by: marsrover001 Posted at: 2018-12-18T20:57:28.902Z Reads: 108

```
The thing to note here is he did it through a loop key. Making a 10s into an 11s. Junk cells in a giant 1s1p config works I guess. If a cell dies it's not much of a loss.

If the focbox is not configured, this may cause high voltage cutoff. Future readers beware.
```

---
## \#98 Posted by: skatardude10 Posted at: 2018-12-18T22:21:03.935Z Reads: 106

```
The main packs BMS low voltage cutoff per P group, main pack battery percentage meter, and a secondary main pack voltage/watt meter. So the main pack I have 3 ways to monitor as voltage gets low, and it never really gets too low since it's always charging. 

For the big 1S pack, all the cells are wired in parallel and should balance each other. The packs voltage is monitored with a 1S low voltage alarm set to 3.2v cutoff. 

As for my vesc low voltage cutoff, I don't plan on running the 1S pack when the main 10S packs voltage drops below 36V since I tend to get sag, and don't want to sag below 28V when the resting voltage reads 39V with the 1S pack, since the vescs low voltage cutoffs are set to 28-30v for 10S. 

Good enough, or do you think I'm missing something?
```

---
## \#99 Posted by: skatardude10 Posted at: 2018-12-18T22:22:56.383Z Reads: 106

```
Plugged in, the voltage is less than 12S, 46V both main and secondary battery fully charged. My high voltage cutoff is set to default at 57V I believe.
```

---
## \#100 Posted by: skatardude10 Posted at: 2018-12-19T00:18:06.288Z Reads: 103

```
Pack works. See post on build thread: https://www.electric-skateboard.builders/t/the-demonseed-tb-218-tb-6374s-190kv-tb-mounts-chibattery-10s4p-dual-focboxes-superflys/50610/100?u=skatardude10
```

---
## \#101 Posted by: mishrasubhransu Posted at: 2018-12-27T03:43:26.858Z Reads: 98

```
To be very precise it should be called portable charger on the go.
```

---
## \#102 Posted by: Winfly Posted at: 2019-01-01T22:45:31.902Z Reads: 101

```
Skimmed through the whole thing. Cus I'm a lazy mfker. Did OP end up doing the 2s5p external pack?

For the 10s to 12s boost, it would only work if it's plugged into loopkey and cell voltage difference between internal and external pack is small, and Metr to reflashing the # cell and voltage cutoff settings. Otherwise, you might risk completely destroying the internal pack when you run it dry.

I'm thinking of making a 13s1p pack with my cheap 2000mah Sanyo18650UR for my Hummie. Kited with a cheap charge discharge BMS and boost converter to plug in at the charge port. Does anybody know if the BMS will limit current draw or should I just get a boost converter than has a limited Current rating. (Will essentially step up to 54.6 voltage applying CV to the charge port all the time until discharge bms cut off the external pack)

Edit: actually I'll be setting the boost to 52v to be safe, cus I don't usually fully charge my batteries anyways unless I wanna be a fast boi that day. Oh and that pack will only be used as a range extender.

What happens when I plug in 52v at the charge port and international pack is higher?
```

---
## \#103 Posted by: amazingdave Posted at: 2019-02-06T18:00:55.252Z Reads: 105

```
Well I’m finally getting around to getting this implemented on my board. Thanks to everyone who’s lead the way on this. 

The key thing for me with this add on is to have a range boost that can be added in seconds when needed and then removed in seconds leaving my board all sleek and beautiful again. 

So far I’ve built a 10s3p 30q pack shaped to fit above the charge port and around the boost converter and bought the boost converter and watt meter. 

Next step will be the enclosure. I’m going to cnc a Delrin top and bottom with sheet ABS between as walls. I’m going to have 2 loop keys, one for powering on the boost pack and one anti spark to enable charging power to the board. The watt meter will be incorporated into the lid. 

The charge port will be connected as soon as the extender is installed....

![image|666x500](upload://xQwtVCYLMLvUBVGTsnBPBZF1wcy.jpeg) ![image|375x500](upload://vxbCtDRtPl3xLK1ISwL3QChODUj.jpeg) ![image|374x500](upload://7pa67TgYTMpL4naWng3lijkAS7w.jpeg)
```

---
## \#104 Posted by: skatardude10 Posted at: 2019-02-06T19:06:54.987Z Reads: 104

```
Looking good! I have a feeling this is going to work out well for you 😎 

I noticed that having the boost converter charging while riding was a great buffer for the reduced efficiency riding Pneumatics, so that too!

Can't say it enough, couldn't get by on my 10S4P without my boost converter setup. I'm considering building a 12S8P, but even then still considering continuing to use the boost converter.
```

---
## \#105 Posted by: DeathByBacon Posted at: 2019-03-14T01:06:40.124Z Reads: 97

```
So I finally tried to build my own range extender but encountered a problem - magic smoke.

So my setup was this:

6s3p 30Q -> [Protection Module](https://www.ebay.com.au/itm/12-36V-XH-M609-Battery-Low-Voltage-Disconnect-Protection-Module-DC-Output-/401520817020?hash=item5d7c81737c) -> [Step-Up Converter](https://www.ebay.com.au/itm/DC-600W-10-60V-to-12-80V-Boost-Converter-Step-up-Module-Car-Power-Supply-/262784414278?var=&hash=item3d2f2bf246) -> Charging port

When there was no load, it was doing what it was supposed to do. But during a load, the insulation on the wires from the 6s3p going to the protection module melted and caused a short. It is possible I might have used a thin wire (although it's the same wire I've been using to charge my board at 4A). Is there a minimum AWG wire I should be using on this setup? Or is there another reason why it happened?
```

---
## \#106 Posted by: TowerCrisis Posted at: 2019-03-14T01:24:58.809Z Reads: 93

```
Keep in mind that the current on your boost battery side will be greater than that of the charge current.

So if your boost converter was converting from 12V -> 24V with a 4A output, your real current draw from the boost battery would be 8A.

It sounds like your main battery was nearly full and your boost battery was low, leading to a very high current draw.

Also, the relay for switching the protected battery on and off is rated for 14V, 20A. Exceeding that could cause additional issues (this is the manufacturers fault, since the board is designed for up to 36V)
```

---
## \#107 Posted by: DeathByBacon Posted at: 2019-03-14T01:40:26.843Z Reads: 92

```
It was actually the opposite, my main battery was 40% and the boost battery was full. After the incident, all the components still work fine. Is it worth trying again but this time using a bigger gauge wire from the boost battery to the protection module?
```

---
## \#108 Posted by: TowerCrisis Posted at: 2019-03-14T01:42:00.681Z Reads: 97

```
Well that's probably your problem. Was it possible that the main battery voltage was actually higher than the range extender?
```

---
## \#109 Posted by: DeathByBacon Posted at: 2019-03-14T02:29:51.840Z Reads: 96

```
Output voltage from the step-up converter was a constant 42v.
```

---
## \#110 Posted by: TowerCrisis Posted at: 2019-03-14T02:32:51.975Z Reads: 97

```
Oh fair enough, that makes sense.. I'm really not sure what's wrong
```

---
## \#111 Posted by: mynamesmatt Posted at: 2019-03-14T03:16:47.168Z Reads: 97

```
![20190313_221924|666x500](upload://fO57E7JWGIyu2sOAg4jh2parwvj.jpeg) 

mines coming along nicely hehe

10s 8000mah 10s4p pack on top of my nano tech 10s2p 9000mah. so probs an extra 18-20km on top of 25km range
```

---
## \#112 Posted by: Petermartin9 Posted at: 2019-03-14T04:13:28.090Z Reads: 97

```
You just described an unregulated charger!  This is not a boost battery pack that can stay connected during a ride.
The constant 42v requires considerable current from your 6s pack. Anything other than a fully charged main pack will attempt to draw serious amps from your "charger pack".  All sorts of overheating will occur, including and especially the internal wiring to the main battery.  When they melt completely and short....
```

---
## \#113 Posted by: TinnieSinker Posted at: 2019-03-14T04:21:09.531Z Reads: 91

```
thats not quite true. the boost converter regulates the amps, preventing it from drawing too much.
when the 42v boost is connected to a half charge pack, the volts drop to what ever the pack is. same with a regular wall charger.

@DeathByBacon did you adjust the amps during a bench test to ensure it was set appropriately? you'll need a watt meter for this
```

---
## \#114 Posted by: DeathByBacon Posted at: 2019-03-14T04:28:42.121Z Reads: 94

```
If you read through this thread, that's what they've been doing. Using a 6s pack + step up to charge 10s, even 12s packs.

But that's another thing that came to mind right away. "Maybe it drew too much amp because my main battery was already quite drained at 40%. How have the others used it? Should have I used it on the get go and not until the main battery's been spent?"
```

---
## \#115 Posted by: Petermartin9 Posted at: 2019-03-14T04:31:48.438Z Reads: 89

```
Is you main battery an OEM pack and connected to an OEM charge port?
```

---
## \#116 Posted by: DeathByBacon Posted at: 2019-03-14T04:31:57.090Z Reads: 91

```
I did a 10 minute ride around the block to drain the battery a bit so I could test my setup. It charged like a normal charger, but then again it didn't have any load.

I set the step up converter to discharge at 2A, 42V. I'm not sure if I can regulate the amps I can draw from the booster battery though.
```

---
## \#117 Posted by: DeathByBacon Posted at: 2019-03-14T04:35:16.825Z Reads: 92

```
The main pack is a 10s3p 30Qs pack that I made myself. The charging port I'm using for the pack is a xt60 with 16awg wires.
```

---
## \#118 Posted by: Petermartin9 Posted at: 2019-03-14T04:41:04.564Z Reads: 88

```
I am sorry I thought this was to stay connected during the ride.  If it is a charger you want, Tinnie is correct about regulating current.  To melt your battery wires you need to be pulling over 10A thru thin wires. Setting the current draw to 5A out should get you close to 10A in.

I suspect your regulator is not regulating too well.
```

---
## \#119 Posted by: TinnieSinker Posted at: 2019-03-14T05:01:54.491Z Reads: 88

```
[quote="DeathByBacon, post:116, topic:64327"]
I set the step up converter to discharge at 2A, 42V
[/quote]

thats very conservative. im surprised that cause a melty wires. feel like we're missing something here
```

---
## \#120 Posted by: TowerCrisis Posted at: 2019-03-14T05:08:25.330Z Reads: 87

```
@DeathByBacon can you post pictures of your full setup (except with the range extender NOT plugged into your board)
```

---
## \#121 Posted by: DeathByBacon Posted at: 2019-03-14T05:12:55.632Z Reads: 85

```
@Petermartin9

I was actually going to use it while riding. (I think that's what everyone in this thread have been doing? Or did I assume incorrectly?) It's just that, a minute after I've connected the booster pack to the main pack, the insulation on the thin wire connecting the booster pack to the protection module started to melt. 

@TinnieSinker

I know. I wanted to stay on the conservative side and be safe, apparently it wasn't. How did you guys make yours? And were you able to use it while riding?
```

---
## \#122 Posted by: TinnieSinker Posted at: 2019-03-14T06:28:10.913Z Reads: 88

```
@DeathByBacon charging while riding is definitely the goal here. I've tried charging at 4 and 6 amps without problems. your booster looks the same as mine as well.
```

---
## \#123 Posted by: pat.speed Posted at: 2019-03-14T20:13:49.448Z Reads: 88

```
At amps higher than 4 I’ve found that the standard 2.5mm barrel plugs start to melt and even weld together. For anything higher than that I would recommend using xt30 or higher rated plugs
```

---
## \#124 Posted by: Petermartin9 Posted at: 2019-03-14T21:17:11.932Z Reads: 88

```
My recommendation is to buy two more 30Qs.
Make a 10s2p. 
Plug it into your XT60 charge port when both packs are about the same voltage and then go riding with the goofy grin you get when you notice less sag, greater acceleration and almost double your current range; all without the side effects of shorting out cells or burning down your trailer park.

Charge and ride them all at the same time so they self balance. Be safe and have a blast riding, not from exploding cells and burning wires.
```

---
## \#125 Posted by: pat.speed Posted at: 2019-03-15T05:20:44.948Z Reads: 82

```
The only problem here is the age of the cells will be different resulting in one pack supplying more power than the other. Also both packs will need a bms
```

---
## \#126 Posted by: Petermartin9 Posted at: 2019-03-15T05:40:34.418Z Reads: 83

```
Agreed. However, this is superior to any 6s3p + voltage booster combo. Imagine what happens following a 30s acceleration or hill climb. i.e. the differential power supply that would occur.
```

---
## \#127 Posted by: Adam0311 Posted at: 2019-03-15T14:22:23.972Z Reads: 83

```
This is totally outside my wheelhouse, so forgive my ignorant questions, but wouldn’t the 6s battery + booster + watt meter work just fine as long as you avoid big amp draw from hills or hard extended acceleration? I’m just trying to determine if it’s worth the effort to build one for my 10s3p board.
```

---
## \#128 Posted by: Petermartin9 Posted at: 2019-03-15T20:38:24.517Z Reads: 80

```
It really seems cool. Assuming you don't start a fire, at some point the 6s pack will empty before the main pack...
```

---
## \#129 Posted by: skatardude10 Posted at: 2019-03-15T22:10:02.705Z Reads: 78

```
I keep a voltage meter programmed for 6s voltage and a low voltage alarm together to alarm when one P group goes below some threshold or the entire packs voltage gets too low to let me know it's time to unplug... they usually alarm at the exact same time. It gets balance charged via charge only BMS. 

6S power tool packs are great with their little built in BMSs, they automatically cut off when empty.

6S batteries --> boost converter --> watt meter works great. Boost converter limits the amp draw (mines set to 4A). Hills and acceleration don't make a difference on amp draw with this setup, constant amp draw, remains stable regardless of load. I just notice 4A worth less voltage sag on my saggy 25rs
```

---
## \#130 Posted by: Petermartin9 Posted at: 2019-03-15T23:11:32.646Z Reads: 77

```
Thanks so much for explaining the entire project. You are very patient with me. I get it now.  I thought Bacon was building a custom 6s3p while attempting to burn his place down. So I was like why not a 10s2p without all the toys?...

Have fun with it. Stay safe.
```

---
## \#131 Posted by: anders Posted at: 2019-05-01T01:12:27.635Z Reads: 71

```
![57343402_634851450319591_6198349166381367296_n|666x500](upload://cr1azEj6OCl8r2kxjYEM8aoxjto.jpeg) 

[boost 900w 15A](https://www.aliexpress.com/item/DC-DC-8V-30V-30V-60V-to-12-130V-Boost-Module-15A-900W-Continuously-Adjustable-Output/32919093000.html?spm=a2g0s.9042311.0.0.1dc14c4dQ6LqSq)

[6-13s BMS](https://www.aliexpress.com/item/BMS-6S-7S-8S-9S-10S-11S-12S-13S-4-2V-25A-Adjustable-BMS-Lithium-Li/32931097519.html?spm=a2g0s.9042311.0.0.1dc14c4dQ6LqSq)

[Watt meter](https://www.aliexpress.com/item/1Pcs-Blue-DC-60V-100A-Balance-Voltage-Battery-Power-Analyzer-RC-Watt-Meter-Checker-Free-Shipping/32572133851.html?spm=a2g0s.9042311.0.0.1dc14c4dQ6LqSq)

Making a portable charger for my 12s 4.6ah graphene lipo.

[Remover of Obstacles](https://www.electric-skateboard.builders/t/remover-of-obstacles-first-build-rayne-amazon-sk3-6374-149kv-12s-graphene/86399?u=anders)
```

---
## \#132 Posted by: skatardude10 Posted at: 2019-05-01T01:52:40.696Z Reads: 71

```
I love this boost converter. If you take it on a board, be sure to pot the components with some e6000 or silicone or something to help resist vibrations. I did this, but missed a single mosfet, and when it failed a few months in it was that mosfet that I didn't glob e6000 around.
```

---
## \#133 Posted by: b264 Posted at: 2019-05-01T01:55:29.029Z Reads: 68

```
What is e6000?  Is this some sort of esk8 waterproofing agent I'm unaware of?  :slight_smile:

How does it work compared to conformal coating?
```

---
## \#134 Posted by: skatardude10 Posted at: 2019-05-01T01:59:08.836Z Reads: 68

```
I don't know exactly, it's clear, goopy, dries into a slightly flexible putty, and it's sold in fabric stores and Walmart but the name is from something about being able to withstand 6000 volts of electricity or something, I guess it was originally designed for electronics?

I may be wrong, but in my search for neutral cure silicone locally, e6000 came up a lot on the Google... 

And I may have misused the term potting but a quick Google said potting was for helping electronics withstand vibration so it seems like the right word to use in this case. 

And you have never heard of e6000 for real?

I've never used it as conformal coating. It's way too globby and thick, I wouldn't use it for conformal coating.
```

---
## \#135 Posted by: b264 Posted at: 2019-05-01T02:02:08.607Z Reads: 67

```
Sometimes I want globby and thick, sometimes I don't.  I'll have to pick up some of this.
```

---
## \#136 Posted by: skatardude10 Posted at: 2019-05-01T02:07:55.458Z Reads: 71

```
Only thing I've been trying to figure out is if it is neutral cure or not. This is the only thing keeping me from applying it to batteries atm.
```

---
## \#137 Posted by: pat.speed Posted at: 2019-05-01T02:26:20.522Z Reads: 72

```
Be careful with that converter, if it doesn’t have a fan to cool the heat sink it will over heat at higher than 4A. I burnt my hands on it last time lol. After adding a fan I can push 8a with a holdable heat sink
```

---
## \#138 Posted by: anders Posted at: 2019-05-01T03:31:05.968Z Reads: 72

```
I was thinking to output 50.4v 4A and input 42v guess input will be 6A efter efficiency losses, better look for a fan.
Thanks for your advice.
```

---
## \#139 Posted by: anders Posted at: 2019-05-01T03:40:43.235Z Reads: 73

```
Thanks for your advice, I can see that happening if you take it aboard, I will definitely secure the components.
```

---
## \#140 Posted by: anders Posted at: 2019-05-03T07:14:36.731Z Reads: 74

```
Did a first charge with my portable charger, battery 10s2p samsung 22p with bms, 15A 900w voltage boost module, watt meter on boosted side, tiny charge bms and cell checker.

![59473127_2263424653975396_4063770061154811904_n|666x500](upload://wpXlHUAfvWvDsI3ewqaKTQuGVcP.jpeg) ![58604201_1257710541034763_1891521112035033088_n|375x500](upload://9lDOCxML8OCQ94d7qzLbtHyBYkU.jpeg) ![59343023_2340961286192440_6295148211585679360_n|375x500](upload://7q6jbX8USA5H2CE1wQLGGmZgB7t.jpeg) 

I set the unloaded voltage to 50.4, when I started charging the charger was giving out 1A then adjusted it to 3.5A output. the charging slowed down and finished at 49.8v 4.15v/cell not sure why? checked later with my Icharger and the cells where balanced within 10mv.
Everything stayed very cool during charging.
```

---
## \#141 Posted by: Tangent Posted at: 2019-05-03T13:25:37.016Z Reads: 70

```
Just read all this, great idea, went to my box of bits and pulled out this boost converter I had used in the past as an led driver, looks like I'll be making a portable charger as well😊
![IMG_20190503_140912|375x500](upload://96KGunTRZTpYEgIf85VPVjKOX21.jpeg)
```

---
## \#142 Posted by: pat.speed Posted at: 2019-05-03T22:08:45.901Z Reads: 65

```
Sometimes it will stop a little early if the current drops below about 60mA. You can just set it a little bit above your actual pack full charge voltage to get the last little bit of charge. Eg. I set my 12s to 50.5 and it usually charges to 50.3
```

---
## \#143 Posted by: amazingdave Posted at: 2019-06-18T09:25:41.630Z Reads: 56

```
Finished 10s 3p range extender.....

Loop key to power up and a separate key to connect the charge port. It mounts straight onto my charge port and charges my 12s4p at 4 amps. It adds a little over half of my standard range so a nice little boost. 

![image|499x500](upload://mOhjr0lcNwaOLDAnP5WSZWItaa9.jpeg) ![image|415x500](upload://n4oN23ifGrXTrRfD8L80xvclrrE.jpeg) ![image|309x500](upload://fKyK8F89zpYFuaDVfBgWjgDWKiu.jpeg) ![image|645x500](upload://2jkSbZ3NRTWf9QcAaoSuFX14my5.jpeg) ![image|690x447](upload://xn3KvLI8H73uHhfiuq6E1ep5NXP.jpeg)
```

---
## \#144 Posted by: Tijmen Posted at: 2019-06-30T23:04:41.724Z Reads: 49

```
I checked out this thread a while ago and also wanted to go down the charging route at first. However, after thinking about it, and taking into account that charging batteries while they're warm isn't ideal, I decided to try a different way.

I'm currently working on finishing up the build and taking some pictures, but basically I've added a port to my board which connects to the output of my antispark switch. When I want to use the external pack, I turn the antispark off, cutting flow from the main pack, and I plug in the external pack which then connects directly to my vescs. This allows me to use each pack independently and prevent unnecessary wear on the cells, or any energy loss due to the use of a converter. Current limitation is the 30A continues rating of the port I'm using. Haven't had time to extensively stress test it yet, but it seems it can handle regular cruising totally fine. I'd use this dual pack setup for long trips regardless with the intent of distance rather than crazy shredding. Even then, the external pack can be used for distance, and I can switch to the onboard pack when I want to dial up the amps.
```

---
## \#145 Posted by: amazingdave Posted at: 2019-07-01T08:05:52.758Z Reads: 45

```
That sounds like a good plan. I’d want a fuse in both the pack and between the anti spark and the port....
```

---
