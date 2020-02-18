# Lithium Polymer and Amp Hours vs Lithium Ion

### Replies: 9 Views: 694

## \#1 Posted by: skatardude10 Posted at: 2018-07-10T03:22:30.984Z Reads: 174

```
Besides the massive 20000 mAh lipo batteries out there, most of the good options seem to max out around 8000 mAh. 

A lot of builds I see seem to use something around 6x series 2S1P ~8000 mAh. 

One thing I haven't found in all my searching and reading on lipo vs liion is how mAh compares in real world scenarios. 12S1P lipo with 8 Ah is less than my 10S4P liion with 10 Ah by the numbers, and I consider my 10S4P pack to be relatively small. 

Does less voltage sag with high C rated lipos with less Ah equal out to effectively more useful energy from a smaller P pack?

I ask because based off my knowledge and experience with liions and Ah numbers, if I were to build a lipo pack I'd want somewhere around 16 Ah to get significantly more range than my liion 10S4P... But that would mean cramming 12x (6 series x 2 parallel) of the 8000 mAh 2S1P lipos into an enclosure... Something I rarely if ever see anyone do on here (multiple P lipo builds). Correct me if I'm wrong... 

Any insight from you lipo users would be appreciated.
```

---
## \#2 Posted by: dino15309 Posted at: 2018-07-10T03:57:45.291Z Reads: 157

```
I used LiPOs for my first build and they are great. I had a 6s1p 5Ah battery made of 2 3s1p cells from HobbyKing. Unfortunately, one of the cells died and I can no longer use the pack...

To answer your question, I don't think you can go wrong with either LiPO or Li-Ion because you can get the same performance out of each. They are both equally dangerous, just one requires more work. You can potentially save money by going with one or the other, but it wont be a huge difference.

Also, 16Ah is a hell of a lot of juice. Most prebuilt boards top out at about 10s and have about 10Ah. If you are u actualy going to get 16 Ah, you must be trying to get 30-45 miles of range. That is AWESOME, but your pack is gonna be HUGE!

I don't Know much about battery sag or how the amount of current effects it, so I unfortunately cannot help you there.

I think whatever you are planning is amazing, but I would watch out going to 12s, simply because you would be running your VESC at its max, potentially lowering it's life span.
```

---
## \#3 Posted by: PatRocks Posted at: 2018-07-10T04:10:58.203Z Reads: 142

```
The primary benefit to using lipos, besides being right when arguing about which one's better, is the amp output. However, as far as usable capacity goes, the lithium ion batteries are probably a better option. The reason I say that is that they can safely be discharged further than lipos.
```

---
## \#4 Posted by: Okami Posted at: 2018-07-10T04:42:00.018Z Reads: 132

```
Well one thing ive thought about is that lipos have nominal voltage of 3.7v, versus li-ions 3.6v 

It might not be much but still at 10s, one has 37 v, the other 36v. Times 10ah, for example, and theres 10wh 'extra', in theory at least.

 I know it is not much but one point might be that lipos stay in higher voltage range, more or less, than li-ons, i think.

Then again lipos have downside that in theory they could be messed up faster with way too much discharge, though i havent had experience with this but it always seems like people take extra care not to drain lipos down..

---

Interesting topic non the less.. maybe @PXSS has some quick ideas to spread here (with references to other existing topics, maybe). 

---

If going for capacity and somewhat little amp output doesnt scare off, multistar batteries have 10, 12ah and 16ah versions (for 6s). 

---

As about voltage sag and amp output. It might be a lot easier to load li-ions so they loose some capacity due high discharge. 

For lipos this might not be as easy to do, though I know lipos still get warm and i dont really have much data to back this up or compare their capacity loss at load and so on..

I Hope this brings discussion a bit further
```

---
## \#5 Posted by: pat.speed Posted at: 2018-07-10T05:21:27.945Z Reads: 119

```
I totally agree about the voltage range being higher with lipos, thus it will have a higher top speed than an identical li-ion pack will for the duration of the discharge. 

The main pros of lipos are cost, amp output and easy assembly. 

The exception to this is when a very large pack is needed, at which point it is cheaper to use 18650 cells.
```

---
## \#6 Posted by: PatRocks Posted at: 2018-07-10T05:28:14.741Z Reads: 115

```
As far as the parallel lipo question, my next battery is going to be a 12s2p, using four of the turnigy 6s 6Ah 65c packs. Although I have a DieBie bms coming, I'm still undecided on using it vs my quad channel hobby charger... 

As far as the large capacity lipos, I couldn't be happier with my 22Ah tattu packs. I charge about twice a month, and the sag is about 1 or 2 volts under a solid 80 amp load
```

---
## \#7 Posted by: Narnash Posted at: 2018-07-10T10:34:15.968Z Reads: 99

```
To directly answer the question
Most people don't pack as many LiPo's in parallel since they don't need to. You can however basicly as many in parallel as you want (more cells more chances of failure), if you're able to care and monitor them (befor, in periodigly while you use them and near their end of life) as you should do with any LiPo battery.



**The LiPo vs LiPo story**
 (the focus here is more on LiPo)

The bigest differences of LiPo and LI-Ion are the shape that they ship with, both have pros and cons.
However Li-Ions cells have usually arround 10Whr of max stored energy, cells with more will have a lower max. Ampere drain and charge, cells with less can be drained faster most of the time, at least when we talk quality cells. They are limited by their standart size, mass produced, usually well monitored in prodction and the most important come with a predetermined breaking point / failsafe by design (venting, it might cause fires but usually no explosion). When the preasure inside is to high they will vent, together with the relatively low stored energy per cell (still more energy than dynamite per size and weight mind you) the damage they cause is more limited compared tho LiPo.

LiPo on the otherhand, is basicly the same (it is not the same, due to the different use and properties of these cells they have different chemistries in them tailored to the use case but they are similar) but stored in a polymer bag. This bag is elastic and somewhat flexible (do not flex it by design !!!!!!!),it can (somewhat) easily manufactured in different sizes. 
When you drain a battery they build up preasure inside (depending on Load and the internal resistance of the battery it will heat up). Espacially LiPo cells also fail by the combustion of electrolyte, insulator or whatever is the weakest  (usually if the first fails the next will follow, rapidly and uproarious) when the temperature goes up (this can also happen, minutes after you had used them or in a hot car or room). Li-Ions will usually vent before it combusts, the exposure of the internals to oxygen sure is also violent but less than a fully charged cell exploding at an instand.


The internal resistance of the cells will rise: slowly by age (when stored correctly), by use and by maltreatment of the cell (both LiPo and Li-Ion, depending on chemistry a lil different but for the most part that is what it is).
What is mistreatment of Li-Ion/LiPo cells then? Well the most common is to high temperatures, which can have different reasons like a bad bad cell in a pack that has a very high internal resistance right at the first day or also very common a short due poorly build of a battery pack (shorts result a very very high amp draw on the cell till it fails). But also a battery that had to deliver to many Amps (over to long time) hence aged way faster than expected . Another common thing is deep discharging cells which will also damage them.


But what are the pros of LiPos then if Li-Ions are safer by their design, well one of the pros I already said it's easier to manufacture special sizes hence you can buy LiPos in various sizes. Another "pro" is their soft and flexible packaging together with tweaked chemistry they can produce cells which "puff" a bid which will recover later when it cools down (if the load is not completly exaggerated) this allows super extreme pulse amp draws, over all can LiPos more or less deliver more Amps than (most) Li-Ions. But it is not recomanded to use "pulse/burst ratings"  for transportation vehicles, since you don't want to push over the limit when standing on your board (for RC it's fine, you may create a lightshow out of your RC but this is better than not to see anything ever again if you know what I mean)


At the end some notes to the "cheap" Hobbyking and China LiPos. I like them, even for Esk8 they can deliver good results at very competitive prices. But you HAVE TO MONITOR AND CHECK THEM, you also should do this with Li-Ion cells tbh but you really have to do it with LiPos and espacially when you try to safe cash. 
1. Right when they arrive check for package damage
2.  unpack them (at best right after they arrive), check the left store voltage (each cell should be between 3.35-3.9V, and don't differ more than 0.05V from each other. You should well document the process, it will help when you try to change them on HK, a video is also not a bad idea. 
3. Don't charge a battery that doesn't meet the requirements above, contact HK they usually do replace them (and have to tbh)
4. Charge them up (4.2V, even when you usually only charge to 4.1 or 4.15V) , after let them sit for some minutes, check the voltage again. After that measure the internal resistance many chargers can do that by themself but usually on in mOhm (which is OK in my book) you can also use methods to calculate the internal resistance (you can find different How to's on YT), you may log the room temperature and/or cell temperature also resistance as always ist temperature dependant.
5. If you don't want to use, the batteries the next couple of days (2-5 days) discharge them (somewhat slowly with something like a light or fan or with one of the charger which ever is more convinient) to store voltage (neutral/no load 3.9-3.75V), but if you want you can also do ...
(6.)  You can measure/check the mAh of the battery, you have to define under which load you do that, manufacturers use usually a very low one 0.2C or less to bump the cell a bit. I would recomand something reasonable like 1C or a little bit lower than the anticipated load. But for better  compareability you should take always the same. A very fresh cell can result lower numbers than after a few charge/discharge cycles but it's still a good practice when you buy a new kind of cell.

As you can see LiPos espacially cheaper ones need quiete some care and time to be used safely (please don't leave your LiPos while testing).



LiPos have most of the time a bit flatter discharge curve curve Li-Ion cells which is handy, but arround 20-25% left charge usually 3.2V you should stop your ride since the voltage drop is very rapid. A high load then and it's very easy to damage your battery (less Voltage same load = more Amp draw = higher temperature) or even destroy it by deep discharging them (under 3V per cell)


You can and may should do all these steps I mentioned with your Li-Ions, too but again you basicly HAVE TO do it with LiPos and act accordingly when your LiPos start to misbehave.



**TL;DR (< than stay with Li-Ion you have to knwo much to use either but LiPo is even more finiky)**

**A LiPo battery can be nice when you have to need a certain formfactor for example, when you want a very light weight and slim low range commuter or when you really need to be able to draw high Amps.**
**But Li-Ions usually can achive a higher Energy density (at least by size, weight it's very close), convenience like a BMS for Li-Ion is also easier to find and you have a bit less hassle with them.**

Also their are way more sound datasheets about 18650 cells available than for LiPo packs.
BTW take "C Ratings" from HK with a grain of salt, they don't state under which circumstances they tested them or if the battery survived their testing. I usually calculate with 1/3 of the continuous C rating.


A LiPo discharge diagram (BTW for safety, both sould be used >65°C cell temperature, Li-Po may survive short jumps but it's kinda dangurous)
https://www.e-cigarette-forum.com/threads/turnigy-graphene-65c-1800mah-3s-lipo-pack-bench-test-results-only-a-28c-39c-pack-but-a-great-one.794599/

A Li-Ion discharge diagram
 (Li-Ions will damage >60-65°C cell temperature and may vent at any time)
https://www.e-cigarette-forum.com/threads/bench-retest-results-samsung-30q-3000mah-18650%E2%80%A6a-great-15a-20-battery.846955/
```

---
## \#8 Posted by: PXSS Posted at: 2018-07-10T12:03:54.819Z Reads: 77

```
I'll answer this topic in more depth tonight. Yes lipos have a slightly higher average voltage so for a battery of the same voltage and capacity the lipo will have slightly more energy. BUT a lipo and liion battery of the same voltage and capacity are different in size and weight. 

For example 
A 2s 3500 lipo battery from gens ace is 3500mah and 7.4v. It weighs 142g and it measures 97mm x 45mm x 16mm = 69.84cc

The equivalent liion is a 2s sanyo ga cell which comes at 7.2v and 3500mah. It weight 94g and measures 18.3mm x 36.6mm x 65.1mm = 43.60cc

So 66% of the weight and 62% of the volume for 97% of the energy.

--- 
Something closer in weight and size would be a 2500mah from gens ace tattu. 
Tattu 2500mAh 2S Fatshark Lipo Battery Specs:
Capacity: 2500mAh
Voltage: 7.4V (2S)
Net Weight: 102g
Size: 73.7*38.1*18.6 mm = 52.22cc

So 73% energy for 109% weight and 120% volume.
```

---
## \#9 Posted by: Cobber Posted at: 2018-07-10T14:16:12.557Z Reads: 62

```
Lipo's are great for punch! :facepunch:
The bigger your motors or the smaller your battery the more they make sense...

It is all the same shit different day, you can not have every thing. You want capacity you can not have discharge!

Also, a lot of the claimed Ii-ion Ii-po difference goes away if you treat your lipos right (the li-ion data is all slow discharge/slow charge (what they are good for) the li-po is fast discharge/fast charge (what they are good for)... charge to 4.15v, discharge to 3.7v static... With the leaky membrane of a lipo you can charge them much faster than a li-ion without them exploding in flames, but they will not last as long. Charge them slower they hold capacity longer... Same with charge cycles, you compare a battery charged at 10c to 1c, guess which will last longer?
```

---
