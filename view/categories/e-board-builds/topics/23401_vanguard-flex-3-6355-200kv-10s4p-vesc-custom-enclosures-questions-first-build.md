# Vanguard Flex 3, 6355 200kv, 10s4p, VESC, custom enclosures + Questions! (FIRST BUILD)

### Replies: 44 Views: 3162

## \#1 Posted by: rok Posted at: 2017-05-18T20:27:29.179Z Reads: 322

```
Yo, i'm from Germany and i'm about to start ordering parts for my build. Since this is the first build i would appreciate your help, guidance and opinions. It will hopefully be similar to @Eboosted, @pyttroll and @whitepony builds. I am looking for atleast 30km/h and hopfully around 30km range on charge. If you could just tell me how to achieve it, that would be great :joy:.
My limit is under 700€.
Keep in mind that i'm 1,78cm and i weight 61kg.

**PARTS:**

-Vanguard Loaded Flex 3

-Maytech VESC: https://www.aliexpress.com/item/Maytech-Benjamin-Vedder-Electronic-Speed-controller-VESC-for-electric-longboard-DIY-skateboard/32712595711.html?spm=2114.13010208.99999999.271.xNWewE

-Motor: 6355 200kv from ESK8.de

-Motor mount, pulleys, belts, trucks and flywheel clones: https://world.taobao.com/item/545683147963.htm?fromSite=main&spm=a312a.7700824.w4004-13745567645.36.du8v6a

-Benchwheel remote: https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-remote-control-bench-technology/32731985084.html?spm=2114.13010208.99999999.264.xNWewE

-Charger 36V-42V: https://world.taobao.com/item/533987952568.htm?spm=a312a.7700714.0.0.fmqxg9#detail

-Battery monitor: https://world.taobao.com/item/524929127650.htm?spm=a312a.7700714.0.0.idmlv8#detail

-Battery: I am planning to make 10s4p battery pack out of Samsung 25R; https://eu.nkon.nl/rechargeable/18650-size/samsung-18650-inr18650-25r.html


-Enclosures and risers will be 3D printed.

I will ask questions in the comments. Thanks boys!
```

---
## \#2 Posted by: Maxid Posted at: 2017-05-18T20:29:19.014Z Reads: 287

```
Please don't get a maytech VESC and support some of our more established brands. Also don't use 25R cells but rather 30Q. No idea if the pulley fits to the motor - it is all in chinese. Did you account for VAT you'll have to pay?
```

---
## \#3 Posted by: IsTalo Posted at: 2017-05-18T20:34:03.399Z Reads: 276

```
I have a Maytech vesc without issues, what happened to you that make you think it is not that good?
```

---
## \#4 Posted by: rok Posted at: 2017-05-18T20:34:25.260Z Reads: 266

```
Since i'm on a budget gonna try Maytech first.
So something like this: https://www.nkon.nl/rechargeable/18650-size/lg-18650-hg2.html
```

---
## \#5 Posted by: IsTalo Posted at: 2017-05-18T20:34:49.372Z Reads: 259

```
Bms and Switch you can buy at Alien, like the Vesc too
```

---
## \#6 Posted by: Maxid Posted at: 2017-05-18T20:35:19.182Z Reads: 258

```
No bootloader, inferior parts (good luck running FOC with those) plus they don't support the developer of the VESC the way they should.
```

---
## \#7 Posted by: Maxid Posted at: 2017-05-18T20:36:33.042Z Reads: 254

```
I said Samsung 30Q - if you have the money go for HG2. With VAT a Maytech VESC will not be much cheaper than a European one.
Cheapest Anti Spark you can find is esk8.de's for 28€. Or get a XT90S. BMS is not necessary with quality cells and a proper charger.
```

---
## \#8 Posted by: IsTalo Posted at: 2017-05-18T20:37:26.315Z Reads: 246

```
Mine came with bootloader, maybe Bruno did it.

And Foc? I would just try Foc with Hub Motors
```

---
## \#9 Posted by: Maxid Posted at: 2017-05-18T20:38:48.428Z Reads: 240

```
What have hub motors to do with FOC? Also Alien seems to not sell Maytech but Flier VESCs (not better though in terms of quality)
```

---
## \#10 Posted by: IsTalo Posted at: 2017-05-18T20:43:06.466Z Reads: 236

```
Alien Sells Both, I choose maytech, and everybody says that Foc is better with Hub Motors, because with normal motors u can burn your Vesc, but lets not hijack this post
```

---
## \#11 Posted by: Jammeslu Posted at: 2017-05-18T21:19:21.702Z Reads: 228

```
You cannot order from taobao if you are not located eithin china
```

---
## \#12 Posted by: rok Posted at: 2017-05-18T21:26:13.719Z Reads: 226

```
@Jammeslu Actually you can through agent over at https://www.superbuy.com/ , etc.

@Maxid Thanks, i found the batteries and XT90S. But are you saying i should run the build without BMS? If so, how is it done? sorry, its a noob question :upside_down:
```

---
## \#13 Posted by: Eboosted Posted at: 2017-05-18T21:26:57.338Z Reads: 232

```
I might be killed by some but you could avoid the BMS and just buy with that money instead a Korad Power supply.

https://www.amazon.com/KORAD-KA6003P-Programmable-Precision-Adjustable/dp/B00AXL7UJA/ref=sr_1_1?ie=UTF8&qid=1495142615&sr=8-1&keywords=korad+60v

If you cells drift, you could easily recharge them individually, but if the solder job is good they won't drift at least not as much.

You can also replace the antispark switch with a loop key, it won't ever brake and people seam to be very hhappy with it, from my personal opinion I like antispark switches, with their fancy blue circled light and perfect finish.
```

---
## \#14 Posted by: rok Posted at: 2017-05-18T21:37:31.830Z Reads: 214

```
@Eboosted Whats the major difference between loop key and anti-spark switch then?
```

---
## \#15 Posted by: Namasaki Posted at: 2017-05-18T21:53:16.900Z Reads: 216

```
[quote="Eboosted, post:13, topic:23401"]
If you cells drift, you could easily recharge them individually, but if the solder job is good they won't drift at least not as much.
[/quote]

Cells will self balance in parallel but not in series. Without a bms, you would have to charge each parallel group separately to get the whole pack balanced.
```

---
## \#16 Posted by: Eboosted Posted at: 2017-05-18T21:55:13.231Z Reads: 209

```
Yes, you could do that with your charger, just connecting each parallel group.
```

---
## \#17 Posted by: Eboosted Posted at: 2017-05-18T22:02:21.446Z Reads: 208

```
With the antispark switch you just press a button or switch to turn on the battery, with the loop key you plug a connector on the battery and might hear or see a small harmless spark as you plug it, in order to turn off the battery/e-board just remove the loop key.
```

---
## \#18 Posted by: rok Posted at: 2017-05-18T22:30:11.274Z Reads: 216

```
@Eboosted I think i will be going with the anti-spark switch, thanks. 

_**Also thread was updated with some specifics about my desires with range and speed (>30km/h and 30km range), and a second option with motor and battery.**_
```

---
## \#19 Posted by: Eboosted Posted at: 2017-05-18T23:55:34.927Z Reads: 233

```
This would be my recomendation:

1. Get 2 x 6355 motors (you won't regret it, get the sensored version in order to get a smooth start)

diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/

2. Get a jst connector to connect the VESC sensors

[http://www.ebay.com/itm/JST-2-0mm-PH-6-Pin-Male-Female-Connector-with-wire-x-10-Sets-/171361716283?](http://www.ebay.com/itm/JST-2-0mm-PH-6-Pin-Male-Female-Connector-with-wire-x-10-Sets-/171361716283?)

3. Get a battery capacity testeer, these are pretty good, good sample rate:

http://www.ebay.com/itm/12V-24v-36V-48V-Lead-acid-Lithium-Indicator-Battery-capacity-Tester-volt-meter-/172018886570?hash=item280d1fe7aa:g:np0AAOSwcBhWYWik

4. Forget about the benchwheel remote, get this one, it's the best one out ther, no dropouts and amazing response. The best part is that it's cheaper:

http://www.ebay.com/itm/2-4GHz-Receiver-Binding-Plug-Radio-Remote-Controller-For-Electric-Skateboard-NEW-/232284516689?hash=item36153c7151:g:gfMAAOSwax5Y2PAs
```

---
## \#20 Posted by: Maxid Posted at: 2017-05-19T05:00:17.987Z Reads: 217

```
The bench wheel remote is supposed to be pretty good and much stealthier than the mini remote. 
Which is a big deal in Germany with esk8 being illegal.

If you want cheap motors you can just get some from banggood - they are pretty good. 

Yes BMS is not necessary - you can build your pack with "split" balance cables so that you can use a 6S RC charger to balance them from time to time and use a 10S charger as your regular charger.

But honestly I don't want to support a Maytech build - so others should try and answer your questions.
```

---
## \#22 Posted by: rok Posted at: 2017-06-10T19:47:53.120Z Reads: 200

```
OK so i got the batteries and most of the parts, still wainting for a motor, antispark switch and the vanguard. 
The parts from taobao arrived pretty quickly, i think it was 10 days from when i ordered till they arrived in my doorstep in Germany. 
Also, all parts from taobao looks very solid. So money-quality wise, thats seems promising, we will see once i get to put them together. VESC also LOOKS fine, i will se if it has a firmware on already, once i supply the energy. 
So i only made one change to my original plan and that was the motor. I'm going with the smaler 6355 200kv motor from ESK8.de. 
The rest of the parts should arrive this week and then i start building.
```

---
## \#23 Posted by: metos Posted at: 2017-07-27T09:37:47.199Z Reads: 187

```
I saw a pic of your board on another topic
could you post some pics of your build ?
```

---
## \#24 Posted by: rok Posted at: 2017-07-27T12:36:45.113Z Reads: 191

```
I won't document a build process YET, because it's still a prototype, but here are some pics :smirk:
<img src="/uploads/db1493/original/3X/7/2/72680141179d9758b46f1bb184338160b6c6edad.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/2/e24567b2881c749d13971d9f3c781fbc51b7b94a.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/4/b/4bade451329d44af3b9c0386c4f2a4201f17e647.jpg" width="374" height="500">
```

---
## \#25 Posted by: SpeedyGornzallez Posted at: 2017-07-27T12:42:29.155Z Reads: 181

```
What did you use to cut away channels for wires in the board? A router?
```

---
## \#26 Posted by: darkkevind Posted at: 2017-07-27T14:12:24.524Z Reads: 176

```
What are you pairing that benchwheel remote with? You need a receiver....
```

---
## \#27 Posted by: rok Posted at: 2017-07-27T14:24:39.780Z Reads: 177

```
A router :+1:
```

---
## \#28 Posted by: rok Posted at: 2017-07-27T14:26:21.711Z Reads: 172

```
What makes you think i don't have a reciever? :confused:
I got it with the remote :wink:
```

---
## \#29 Posted by: darkkevind Posted at: 2017-07-27T14:57:09.865Z Reads: 171

```
That listing is for transmitter only.

Do you get a receiver with it too then?
```

---
## \#30 Posted by: rok Posted at: 2017-07-27T15:25:31.907Z Reads: 170

```
[quote="rok, post:1, topic:23401"]
-Benchwheel remote: https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-remote-control-bench-technology/32731985084.html?spm=2114.13010208.99999999.264.xNWewE
[/quote]

Link with reciever and remote: https://de.aliexpress.com/item/Electric-skateboard-refitting-parts-DIY-800MAH-remote-receiver-2-4G-bench-technology-benchwheel/32791243047.html?trace=msiteDetail2pcDetail
```

---
## \#31 Posted by: rok Posted at: 2017-07-27T15:41:38.824Z Reads: 168

```
[quote="rok, post:1, topic:23401"]
-Enclosures and risers will be 3D printed.
[/quote]

Were actually made out  of a fiberglass :sweat_smile:.
```

---
## \#32 Posted by: darkkevind Posted at: 2017-07-27T15:51:10.542Z Reads: 164

```
This is the one I got. It's no longer available. You can't get a receiver anymore...
```

---
## \#33 Posted by: rok Posted at: 2017-07-28T06:40:35.923Z Reads: 154

```
There is an option to order it through Superbuy agent from taobao: https://m.intl.taobao.com/detail/detail.html?spm=a1z5f.7632060.0.0&id=548548804338
```

---
## \#34 Posted by: darkkevind Posted at: 2017-07-28T07:31:53.754Z Reads: 150

```
Oh nice, thanks for that. :thumbsup:
```

---
## \#35 Posted by: rok Posted at: 2017-07-28T10:19:15.478Z Reads: 150

```
No problemos :wink:. Why do you need another one?
```

---
## \#36 Posted by: darkkevind Posted at: 2017-07-28T10:49:49.996Z Reads: 146

```
Second build! 😉
```

---
## \#37 Posted by: rok Posted at: 2017-07-30T20:29:29.902Z Reads: 142

```
Soooo, the Maytech VESC just died. And before you guys go all shitting over maytech it was actually the bolt from the battery indicator that came loose and fucked up the vesc. Now, the question is, buy a new Maytech or a more expensive Vesc with better quality i guess? What do you guys think?
```

---
## \#38 Posted by: BoostedBuilder Posted at: 2017-07-31T20:17:18.497Z Reads: 127

```
Get a VESC X for almost the same price from a group buy))
```

---
## \#39 Posted by: rok Posted at: 2017-07-31T20:45:43.399Z Reads: 128

```
Would love to, but need it sooner than late august :(
```

---
## \#40 Posted by: BoostedBuilder Posted at: 2017-08-01T09:58:44.082Z Reads: 131

```
http://www.electric-skateboard.builders/t/new-focbox-for-sale-us-free-shipping-price-reduction/19089/194
There you go, he has them sooner then late August)
```

---
## \#41 Posted by: rok Posted at: 2017-08-01T12:55:12.079Z Reads: 133

```
Thanks, contacted him :slight_smile:
```

---
## \#42 Posted by: rok Posted at: 2017-08-15T11:52:01.927Z Reads: 119

```
Does anyone have any idea why my board doesn't like hils? 
Previously, still on maytech vesc and short motor wires, i was able to climb pretty steep hills without any problems but now all i changed was the maytech vesc to Esk8.de speed controller and i ran the motor wires under the griptape and into the enclosure. 
I run into a problem sometimes when i go up the hill and motor just looses power about half way up, at the end it becomes so weak, that i need to step down and walk. Do you think the cables are too long? 
I am posting picture of cables wired through and vesc settings. I changed max current to 65 and braking to 60 and motor detection was higher, 105. No other changes.
<img src="/uploads/db1493/original/3X/1/2/120ead141619335e6fe28cf1a6302b718a7338e5.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/8/2/8238cc742787857cae23b68561a8baed01108c29.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/9/e9ac7f62bbe2562812806a477ca70c099253ac37.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/f/1f17ace6126c29977ada202a868dc73c7a6b3d95.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/8/289523f8b6e64b671ce008f3310b5a02d1bec25b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/0/70e055be67aea10578ba68359236795bdb933c1a.jpg" width="666" height="500">
```

---
## \#43 Posted by: overint Posted at: 2017-08-16T00:59:26.096Z Reads: 100

```
Hey dude, looks like an awesome build!
How did you make the enclosure?
```

---
## \#44 Posted by: rok Posted at: 2017-08-17T16:45:14.228Z Reads: 92

```
Just very basicly made from fiberglass. No vakum pump used.
```

---
## \#45 Posted by: WawiKirsinger Posted at: 2017-08-18T00:26:00.442Z Reads: 89

```
hey! new here and im on the phase of learning and Reading! really nice build! can you take more photos under the deck to see those cases and photos of the inside to see how did you managment the space plz! and can you make the same batterie case with lipos in it? (10S1p) i know you arer using 18650 but i just wonder if it would be the same space or how much more it would be... thanks!
```

---
