# 8s2p battery charging?

### Replies: 16 Views: 2452

## \#1 Posted by: m4almbergs Posted at: 2017-01-23T22:46:22.935Z Reads: 155

```
HI!

I have searched the forum for 2 days now and can't fined any one ho have the battery setup I want and I don't know how to charge it.......

i want to have a 8s2p battery consisting of 4 x 4s 5000mAh 25c batteries ( [this one](https://hobbyking.com/en_us/turnigy-5000mah-4s-25c-lipo-pack.html) ) i know how to  hook them up to make it "2 packs" of 8s in parallel but how do I charge them ? Ofc I want to charge them all att the same time if that is possible. I am willing to invest in a expensive charger if necessary.

I know @trbt555 is really good at this stuff and have made some awesome diagrams befor mayby he can help.

Any contribution is greatly appreciated!
```

---
## \#2 Posted by: Okami Posted at: 2017-01-23T23:30:10.171Z Reads: 147

```
Turnigy accucel 8 seems to have 8cell charging

Otherwise split - charge as 4s, though you will.then get capacity x4 for charging and from safety perspective it would also be better to charge at once smaller pack
```

---
## \#3 Posted by: m4almbergs Posted at: 2017-01-23T23:43:46.585Z Reads: 140

```
Hmmm but how do people ho have 10s batteries charge then ? And I still would have to charge the 2 "8s packs" ( 2 x 4s in series) one by one and how do I do with the balance cables? 

Thank you anyway for the tip
```

---
## \#4 Posted by: mmaner Posted at: 2017-01-23T23:49:00.394Z Reads: 133

```
Typically anything over 6s is going to be Lion with a BMS.  If you are talking Lipos in series, then using a balance charger with x2 4s to 8s adaptor is about your only choice.
```

---
## \#5 Posted by: m4almbergs Posted at: 2017-01-23T23:55:08.453Z Reads: 135

```
[quote="mmaner, post:4, topic:16571"]
x2 4s to 8s adaptor
[/quote]

I can't seem to find exactly that :confused:
```

---
## \#6 Posted by: m4almbergs Posted at: 2017-01-23T23:59:32.185Z Reads: 128

```
if I find the 2x 4s to 8s adapter is ther no way to charge 2 8s in parallel?
```

---
## \#7 Posted by: Okami Posted at: 2017-01-24T00:02:58.938Z Reads: 143

```
You would prolly need to make your own adapter then. If you cant find 4s x2 to 8s x1

Check ebay for 8s jst connector. I believe it needs to have 9pins. 1 positive, 8 negative.

Check charger i mentioned. It is in blue color and quite beefy.

Otherwise consider getting some bms. Im not sure though how great does they work for lipos
```

---
## \#8 Posted by: Okami Posted at: 2017-01-24T08:19:23.158Z Reads: 130

```
https://hobbyking.com/en_us/turnigy-accucel-8-150w-7a-balancer-charger.html

8S charger.. this might make it a bit easier to charge up everything.. will try to look up that 8s wire harness

----

http://www.ebay.com/itm/New-8S-JST-XH-Connector-balance-silicone-wire-CellLog-9-PIN-/181713383731?hash=item2a4ef63133:g:YJgAAOSwymxVJ3Pc

This is the cheapest you can get it I think! Also im not sure can you get these in Eu.. at least I didnt see them on hobbyking.. + 8s seems not be a popular choice, so it is hard to find much for 8s

---
You combine the previous cable with this one:

http://www.ebay.com/itm/2Pcs-JST-XH-Lipo-4S-Balance-Wire-Extension-Adapter-with-20CM-Silicone-Wire-Model-/281488194605?hash=item418a00fc2d:g:x9oAAOSwLa9UWkr2

You would need to cut down the ''male'' connector and solder the wires to the 8s connector..

This way you should be able to plug your 2X 4S batteries into 1x 8S cable (when soldered together!)

**EDIT:** You can also buy 4 of these cables and then just wire/solder them to one 8s cable..

----
Otherwise, just get / buy cable like this:

http://www.ebay.com/itm/Parallel-2x-JST-XH-Balance-Adapter-8S-/291322427289?hash=item43d42b7799:g:CVYAAOSwwbdWJVJ8

**Unfortunately, I could not find one from china!** This is from usa.. When going with multiple battery packs connected, the bad part is the wiring.. 

**You will also need to adjust the lenght of cables** (make them longer, for example) to make it comfortable to reach the balance charger from your battery/board! 

---

You will need to know how to solder! It is not that hard to solder these small wires (just hold them down steady).. but you will need to know how to wire them up correctly!

I also would advise to buy **silicon** balance leads, they will be a lot better than these tiny/cheap ones. (the ones shown, should be silicon wire already but im not sure will you order the same items at the end!)

--
**EDIT:**

Found an alternative, looks like some **UK vendors** also have these cables in stock:

http://www.ebay.com/itm/JST-XH-8S-30cm-LIPO-BALANCE-Silicone-Wire-Lead-Cable-connector-plug-UK-SELLER-/162334310382?hash=item25cbe0ffee:g:ATwAAOSwL7VWkUHk

----
Look it up, for some of the cables, the quality might not be the same. but the one I gave you here, looks quite ok!

You would also need to cut into the cable to make the **parallel connections**.. 

To join 2x 8s batteries, you will need to make a parallel connection.. Unless you charge them seperately / one by one.. which wont be fun I think..

--

This is all I could give.. the rest is up to you..

Text diagram, to make it easier for you:

_2x 4s batteries goes into 1x 8s battery cable, then 2x 8s battery cables goes into one 1x 8s battery cable, which is connected to the charger._

|Battery| Male connector -> Female connector (4s) > Bare wires (5pcs) -> Bare wires (5pcs) -> Bare wires (9pcs) -> Male connector | 1x 8s connector| 

_1x 8s connector (Male) + 1x 8s connector (Male) -> 1x 8s Female connector (per each) -> Wires -> 1s 8s Male connector_


-----

Good site to compare / take a look at balance wires:

http://www.progressiverc.com/wires-connections/charge-cables/balance-cables/

If there was a ''ready made'' cable for 4s x 4 to 8s x1, then it would be pure gold in your situation...

Perhaps it is possible for you to make it a ''direct cable'' but it is up to you how do you see it easier..

So yeah, you can actually buy 4s x 4 female cables with wires, then solder all of them to one 8s 1x cable.. IT will look something like this:

<img src="/uploads/db1493/original/3X/2/2/2274f4f1115b21cc2caccdb1896b6e0c6539e847.jpg" width="328" height="209">
```

---
## \#9 Posted by: m4almbergs Posted at: 2017-01-24T09:22:57.883Z Reads: 98

```
Wow! So much great information! Not at home right now will look more closely in to it wen I get home and give a more detailed answer.
```

---
## \#10 Posted by: Okami Posted at: 2017-01-24T09:35:22.538Z Reads: 103

```
yeah.. spend some time.. and decide how you do it.. wont be as easy to change something later! Also get all your supplies at once.. so there's not much waiting time for little parts.. (like connectors or wires)..

If you got that ~60-70 eur for the charger, I would say go for it.. you might save a bit by going with ''weaker'' 50w 6s charger, but your wiring will probably be a bit different and you wont be able to monitor cells/battery as closely, as with this setup..

**50w (B6) charger costs around ~20-25 eur I believe** 
+ _??? Power supply price (unless B6AC model ~40eur)_

**150w charger (accucel 8) around 60-65 eur**
+ _??? Power supply price (can use ''server psu'' or old PC psu, but some modification, to these will be needed!)_

for your pack - 8s 10 000mah, 

**I would advise to get that 150w charger.**. (~4.3amp charging, when at 145w on the charger)

Should get you ''ready'' in about 2h 15min +/- (2h30min) more likely. This is at 9600mah capacity, as I believe you wont be able to sqeeze all of it.

---

Now compare that to 50w charger..

_4 x 5000mah = 20 000mah (derated to 19 200mah)_
_at 48W (16.8v = 4.2v x 3) = 2.86A charging_
_6h 45min.. or so.._

So yeah, choose do you want to charge in about **2h30min or 6h 45min..** 

----

By the way.. with this big battery, I believe you should be able to ride around **28km**
as your battery should be around 284 Wh. (I derated it a bit, to 9.6ah x 29.6v)
Typical longboard consumtion is ~10wh per km

This is without hills.. if you got them.. probably around 20km is also achievable possible, depending on hills.. will be some really nice long distance eboard :)
```

---
## \#11 Posted by: m4almbergs Posted at: 2017-01-24T15:59:38.970Z Reads: 92

```
[quote="Okami, post:8, topic:16571"]
You will need to know how to solder! It is not that hard to solder these small wires (just hold them down steady).. but you will need to know how to wire them up correctly!
[/quote]

soldering will be no problem as I have soldered electronics many times before.

[quote="Okami, post:8, topic:16571"]
2x 4s batteries goes into 1x 8s battery cable, then 2x 8s battery cables goes into one 1x 8s battery cable, which is connected to the charger
[/quote]

at the exact moment i read this i relist two things.

1. that I previously during my search for information on this came a cross some one had do something similar but with 3s batteries and what I din't like about that set up was the fact that he was charging 2 cells for each weir on the balance lead. essentially tricking the charge that it was charging 6 cells wen it actually was charging 12 cells. The problem with this that someone i can't remember was that you could get unbalanced cells in the long run and had to charge the batteries in 
their original "pack" ones in a while to prevent this. And i don't want to do that and i want board to be as reliable as possible.

2. How stupid i am not thinking about that when i posted this! ofc you can't balance charge every individual cell if put all of my 16 cells  in to a 8s,6s or 4s balanced charging JST-XH cable! I feel so bad now that you have done all this research on my faulty question :disappointed: so sorry man! 

But all is not lost! I still need 1 or 2 of the  JST-XH cables you found for me. Because I think i found a solution to my problem that requires them! will post my solution just need to draw a diagram to make it easier to explain.

Ones again thank you even if it din't solve my problem directly, the info you gave me was 100% necessary for me to make my own solution
```

---
## \#12 Posted by: Okami Posted at: 2017-01-24T16:11:14.826Z Reads: 88

```

you can always check cell state (of each pack) by yourself! Just leave the wires somewhere, so you can access them!

You know, you actually have ''simple config''.. Take a look at li-ion packs.. Some people build 6-10cells in parallel, You will have only 2.. Of course lipo seems to go out of balance after a while (less stable) but I think 2P config is not that bad..

Ive got 4P cells myself (li-ion) and ppl on this forum also usually build using 2-4P when going li-ion..

The ''math'' is in the fact that cells in parallel should balance each other out.. so let's say, if one cell is a bit weaker, the rest of the cells (the other pack, in your case) will need to ''balance it out''.

I think it is a bit worse for ''series'' cells, as they dont get balanced between each other..
If one of your lipo packs will go bad, you will probably see that in total voltage of the pack.. or the capacity wont be as good as it should be..

Im not sure will you find 16s charger.. :) and motors / esc / electronics here also does not support 16s.. 

IF you compare, then it seems that BMS modules some ppl use (instead of balance chargers) sometimes does not balance cells like they should or they mess up / cut of the energy too fast / too early.. and you wont even see what bms is doing.. unless you check by yourself all the voltages..

So yeah, I think you should stick to 8s 2P.. I think you now understand that 4S 4P is a lot worse.. way bigger pack and less chance to see the actual voltages..

Your only other option now would be to get ''bulk charger'' + bms.. the choice is up to you..

I think the problem might be in that we use ''hobby chargers'' which usually dont have as high voltages as we use.. So that's why they are usually only 6-8s capable.

---

You can always leave the packs ''seperate'' and charge them one by one.. that will also be 2x the effort and 2x the time probably..
```

---
## \#13 Posted by: m4almbergs Posted at: 2017-01-24T18:46:13.118Z Reads: 82

```
[quote="Okami, post:12, topic:16571"]
you can always check cell state (of each pack) by yourself! Just leave the wires somewhere, so you can access them!
[/quote]


I am still not sure about charging the 2 packs of one JXT- HS 8s balance cable. how often would i have to check ? and is charging that way safe? don't it reduce the longevity of the batteries? 

 [quote="Okami, post:12, topic:16571"]
You can always leave the packs ''seperate'' and charge them one by one.. that will also be 2x the effort and 2x the time probably..
[/quote]

i think that is what i will do! and have a Duo charger like this [one](https://www.amazon.com/s/ref=nb_sb_noss?url=search-alias%3Dtoys-and-games&field-keywords=UP100AC+Duo+Dual+2+Port)
or just charge the 8s packs one by one with the charger you suggested.  

this is how i am planning to hook every thing up. I put in 2 XT90 S loop keys that are in doted boxes. Those two i simply remove  wen i want to charge.
<img src="/uploads/db1493/original/3X/8/d/8d4d847135503e432b3840c2c155036d81ded3be.png" width="690" height="380"> 

after spending so much time on this forum this week i rely need to study so i won't be back until tomorrow night
```

---
## \#14 Posted by: Okami Posted at: 2017-01-25T09:38:25.944Z Reads: 73

```
https://www.amazon.com/UP120AC-12Amps-120Watts-240Watts-Total/dp/B00SZ1CBVC/ref=sr_1_fkmr2_1?s=toys-and-games&ie=UTF8&qid=1485336677&sr=1-1-fkmr2&keywords=UP100AC+Duo+Dual+2+Port

<img src="/uploads/db1493/original/3X/2/9/29fc6f258e8ab6a7a80eae3946c1872da83bc346.jpg" width="690" height="387">

IF you can grab this one.. it has (it states) 240w total, 120w for each channel..

Though, it is a 6s charger, so you will have to split your pack once again.. and you wont be able to escape the need to charge in parallel.. if you got 4 x 4s batteries, your only chance would be to have 4 charge leads, 4 balance ports and then charge all of that on 4 port charger.. (or 2 chargers with 2ports each).. does not sound very practical..

Try to look up some topics on here about charging in parallel..

I could suggest you using 8s dual charger.. unfortunately I dont know one, which would be dual and 8s.. so far I only know turnigy reaktor with 4 ports (30a total or so).. it is quite expensive..one

---

hah yeh I had the same situation last year.. I was so much into researching about eboard building that some other things had to step aside a bit.. for a while.

---

**Take a look at some of these videos / resources:**

https://www.google.lv/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=charging+in+parallel+lipo

I think it will be easier to ''convince'' you to use parallel charging, than it will be to find a suitable charger for the situation you imagine. The ''iCharger'' series seems to have some 8s capable chargers but they are at over 200usd in price and Im not sure how easy it is to buy one (+ tax will be also on top of that, probably)

--

This guy chargers a ''ton of batteries'', look at him:

http://www.rchelicopterfun.com/parallel-lipo-charging.html

And he is doing that for 6yrs already.. there is just some ''common sense'' knowledge you should be aware of.. like dont charge if batteries are way too off from each other etc.. you just need to rig it all up, so you get some sort of insight at what level are your batteries before charging (that is if you want to make 100% sure everything is as it should be).
```

---
## \#15 Posted by: boutch55555 Posted at: 2017-05-01T00:10:34.259Z Reads: 60

```
I went the iCharger way, ordered a 1010b+ since it was 5$ cheaper than the 208b. I also have 8s2p in the form of 4x 2s 5000mah, x2 . Main power on top, balancing at bottom, my plan looks like this : <img src="/uploads/db1493/original/3X/f/2/f2c82a70584a6e014d5b9c19d4afee5caf1deece.png" width="690" height="446">
```

---
## \#16 Posted by: Sleepingalex24 Posted at: 2017-06-20T00:37:39.727Z Reads: 52

```
Would it be possible to do an 8s2p setup with a bms? I'm wondering because then all the cells are not monitored, only pairs of cells. This means that one of the pairs could be very low and the other high and equal a normal voltage. Would this ever happen?
```

---
