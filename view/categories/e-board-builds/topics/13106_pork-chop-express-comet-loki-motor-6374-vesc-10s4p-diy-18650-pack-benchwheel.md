# Pork Chop Express &#124; Comet Loki &#124; Motor 6374 &#124; VESC &#124; 10S4P DIY 18650 Pack &#124; Benchwheel

### Replies: 35 Views: 5322

## \#1 Posted by: Norco Posted at: 2016-11-15T16:02:17.034Z Reads: 409

```
Hi everyone,

This will eventually become my build diary but for now looking want to lay out my plan and check it will achieve what I am after.

Basically I am a tad on the heavy side at about 104kg (230lb) and just over 6ft 1" 

I want to build a board that I can use to commute which is 3.2miles each way (along a reasonable condition cycle route and in a city that is pretty much totally flat). Ideally not wanting to charge while I am at work. I have an OK understanding of electronics from my racing drone builds.
I have read the guidance for build advice for a heavier rider (along with a ton of other threads) and come up with the plan below:
Single Drive (mostly for cost)
Board tbc prob second hand and a stiff DH board
Battery 8s2p (looking at 4 5000mAh 2x series then in parallel)
Motor looking 6355 235kv (Probably ADS with the sale they have on at the moment)

I have looked at the Europe Group buy and will probably pick up some:
90mm wheels 
Maytech VESC
Pulley 36/16
Mini remote 
Anti Spark switch 
%battery level readout

The leads to these figures - which I am more than happy with (granted expecting max speeds to be lower due to weight)

<img src="/uploads/db1493/original/3X/c/f/cf7e78ced7670dd2ebd9ca5e50d0eb7d763e4daa.png" width="690" height="431">


Does this all look ok? Should I be looking at a bigger motor?

Any help or guidance (or even a couple of ideas for decks to look out for would be a great help)

Thanks
Norcs
```

---
## \#2 Posted by: Jinra Posted at: 2016-11-15T16:17:13.571Z Reads: 375

```
All these settings would generally be okay if you were lighter. Here are some things you might want to think about changing

* Motor - if you're going single, get a 6374. Otherwise, you can do dual 6355's.
* Motor pulley - 16T is great for speed, but can be taxing on your motor if you're heavier, consider dropping this down to 14T.
* Motor kv - heavier riders tend to stick with sub 200kv motors. They tend to have more copper, leading to more torque.
* Wheel size - you should be fine with 90's, but if you're worried about torque, you can drop this down to 83mm. It doesn't have as much influence on torque as the previous three.
* VESC - you may want to reconsider getting a cheap VESC as it's arguably the most important component to **not** cheap out on
```

---
## \#3 Posted by: Norco Posted at: 2016-11-15T16:48:27.856Z Reads: 353

```
Thanks for the advice. Would all of these measures be necessary? 

I could fix 2 problems with the Turnigy Aerodrive SK3 - 6374-192kv but if I reduce the motor pulley teeth to 14 the top end speed dips to below 20mph.

If I keep it at 16t then I would get just over 21mph (in theory) - is there anyway I can look for an estimate of range on these set ups too?

I'll probably stick to 90mm to try and mitigate some of the poorer parts of the cycle track.

Thanks
Norcs
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-15T16:51:02.102Z Reads: 320

```
Not all are necessary, but all help. The most important one is motor size. Definitely go for a 6374 if you're running single. You could consider using the 192kv with a 14T motor pulley but upgrade your battery to 10s. This will put you at roughly 25mph.

A rough range guide is 10wh = 1km. This will vary depending on board efficiency.
```

---
## \#5 Posted by: Photorph Posted at: 2016-11-15T17:01:10.326Z Reads: 304

```
well.. I was in the middle of typing something out but Jinra covered everything I was gonna say and more.  So what he said.
```

---
## \#6 Posted by: Norco Posted at: 2016-11-15T17:08:40.668Z Reads: 294

```
Ok that all makes sense. Maybe I revisit the battery situation. 8s seemed a good balance of power vs cost.
```

---
## \#7 Posted by: Mikenopolis Posted at: 2016-11-15T17:44:06.774Z Reads: 286

```
I'm 210lb and the single 6374 is more than enough on flats
```

---
## \#8 Posted by: Norco Posted at: 2016-11-15T18:26:02.264Z Reads: 281

```
OK that sounds good. What battery are you using?
```

---
## \#9 Posted by: Mikenopolis Posted at: 2016-11-15T18:50:50.181Z Reads: 280

```
I went the lazy route and got Enertions SpaceCellPro 4 (10S). I was skeptical of the single 6374 over dual 6355s but wanted the range and it's been good for me so far
```

---
## \#10 Posted by: Norco Posted at: 2016-11-17T10:56:34.276Z Reads: 248

```
Any real issues with using 2x 5s or 6s 10000mAh batteries. Charging I suppose will be a bit more of an issue but I already have a couple of lipo chargers. I was swaying towards building my own pack but I may save that for a later version.
```

---
## \#11 Posted by: Tuomalar Posted at: 2016-11-17T12:00:55.169Z Reads: 241

```
You should consider 18650 li-ion cells. In my opinion its's waste of money buy lipos at first and then notice how much easier li-ions are.i
```

---
## \#12 Posted by: Norco Posted at: 2016-11-17T12:29:35.857Z Reads: 253

```
You are probably right. There is the cost factor too. Lipos would cost me probably £160 - £180 and I already have the chargers. Building a pack would mean £160 on cells, BMS, charger, nickel plates, spot welder. Likely over £250 even if I soldered rather than welded.
```

---
## \#13 Posted by: SirDiff Posted at: 2016-11-17T12:36:34.583Z Reads: 251

```
I think there are some group buys coming for liion packs in Europe. Recently one has been able to provide a 10s4p for 190 € welded with copper, it was about 250 at the end including bms, charger, led status indicator and integrated switch (euros, which is something like 200 pounds). Would are probably good with a 10s3p, that would cost even less. @ajaynagra may have something for you in the near future, ask him
```

---
## \#14 Posted by: Tuomalar Posted at: 2016-11-17T12:41:06.294Z Reads: 248

```
Check eu.nkon.nl 
For example 10s4p pack (40 samsung r25 cells) 120e cells alone
```

---
## \#15 Posted by: Norco Posted at: 2016-11-17T12:42:08.550Z Reads: 248

```
Good point. I have shown interest in the Europe group buy for a fair few parts so will look for a battery buy too. Still torn. With some thinking about the enclosure I am not totally sure it would be that much of an issue to open it up and charge a couple of batteries each night. That said if it can be done for not much more then it would be great to just plug in.
```

---
## \#16 Posted by: Norco Posted at: 2016-11-17T12:44:07.925Z Reads: 255

```
Thats a great price. Thanks! Have you used them before?
```

---
## \#17 Posted by: Norco Posted at: 2016-12-13T17:15:34.198Z Reads: 324

```
So the board, batteries and nickel strip are here. I feel like I have ordered parts from every corner of the globe and everyday the postie comes down the drive its like christmas!

Good deal on a benchwheel remote now too. Just to finalize my order through the group buy and everything will be ordered. Incidentally anyone know where I could get a 12mm / 14t motor pulley if they aren't available with the group buy. 
I have seen this website but not really sure what I am looking for?
http://www.beltingonline.com/timing-pulleys-bars-272/?zenid=m0jfch7qt65ked5ue6c4m025a2 

Thanks
Norcs

<img src="/uploads/db1493/original/3X/8/a/8aa3aafb51bdae66e2c1220dcfbf95e622d761f6.jpg" width="320" height="320">
```

---
## \#18 Posted by: Norco Posted at: 2016-12-23T01:02:16.022Z Reads: 322

```
So a quick little progress update. 

I have collected all I needed now for the battery build so I have been working on that. 

I have capped off all the positive terminals with insulation rings and then glued the parallel sets together.

Then I have soldered the nickel plates to the batteries and reinforced the serial connections. Next I will solder strips to connect these two halves then fold them out on themselves. I am checking connections as I go and all looks solid so far. The only thing that concerns me is how I would know if one of these solder joints was to go bad?

The glue and tape seems to hold them tight and the shrink wrap will pull around the pack so perhaps it wont be an issue. I must say soldering has been fine. Its pretty cold in the workshop at the moment (unheated) so not having any issues with too much heat in the cells.

Anyway I couple of pics to show progress and a hat tip to @whitepony for inspiration 

Norcs

<img src="/uploads/db1493/original/3X/f/9/f9abe6a0e75a33adff5a6cc2f4caca67d989e38e.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/5/25a74470b4a3c8fc7057ed302b14f92525019735.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/a/2/a29a67ab75298bade0480eeefdf57b5d216029b4.jpg" width="690" height="388">
```

---
## \#19 Posted by: wmj259 Posted at: 2016-12-23T03:53:24.089Z Reads: 311

```
Are those Samsung inr?
```

---
## \#20 Posted by: Norco Posted at: 2016-12-23T07:08:30.731Z Reads: 309

```
Yes,  sure are :slight_smile:
```

---
## \#21 Posted by: Norco Posted at: 2017-01-06T23:46:05.739Z Reads: 298

```
So the battery build is almost finished apart from an xt90 to cap off the power leads and a mesh wrap and shrink wrap over the top. Pretty happy with it for a first attempt and Soldered only. Was a little concerned about the balancing wires wearing through and shorting out on the side of the nickle as they run over the battery and down the middle so I have encased them in hot glue at the turn. Checked the balance leads are all working and they are and the whole battery is sat at 35.7v 😀 Can't wait for the rest of my parts to turn up now.
```

---
## \#22 Posted by: Norco Posted at: 2017-01-06T23:51:52.053Z Reads: 323

```
<img src="/uploads/db1493/original/3X/5/2/52f7e59dcb7bb7e126952b89e09ac9afd2d74bb0.jpeg" width="281" height="500">
<img src="/uploads/db1493/original/3X/3/4/3425c36e5357b4e1820ef919933070451a489fb4.jpeg" width="690" height="388">
<img src="/uploads/db1493/original/3X/f/2/f21c5aaf261b131ae229192db6f38edad1d59980.jpeg" width="690" height="388">
```

---
## \#23 Posted by: Norco Posted at: 2017-01-07T23:26:36.647Z Reads: 310

```
Battery finished 😊
<img src="/uploads/db1493/original/3X/4/2/4205609e39000ba892536d411558f7d38d968f36.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/4/6/4631267d17b02598dbda1402a5d1cb8487d32fa9.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/b/b/bb3d3cd7481153b678e5f807279e759bd101edc2.jpg" width="281" height="499">
```

---
## \#24 Posted by: Norco Posted at: 2017-04-10T23:53:38.216Z Reads: 267

```
OK so I have been quietly getting parts together and making the last plans but the biggest progress comes from my enclosure. I've built a vacuum forming oven and table and managed to get a good form on a single piece enclosure for my battery, VESC and receiver with room to spare! Here are a few pics. <img src="/uploads/db1493/original/3X/4/f/4f88a99a17c8ddf9f73a66a28ddc9712e6477774.jpeg" width="690" height="388"> <img src="/uploads/db1493/original/3X/d/2/d29a84376ea206ac7a01b5344d89e9ddb8aaa0ee.jpeg" width="690" height="388"> 
<img src="/uploads/db1493/original/3X/7/a/7aba0001d425fb121ad3ede049cb82a5f5337864.jpg" width="690" height="388">

Not happy with this one. I didn't get the frame over the mould cleanly enough. 
<img src="/uploads/db1493/original/3X/9/2/92f3c0ff7caf66503b3027ecbf912c2c328addd7.jpeg" width="690" height="388">
This one was much better
<img src="/uploads/db1493/original/3X/b/d/bdfd74ef388e077564c4f21b9314ba6252117973.jpeg" width="690" height="388"><img src="/uploads/db1493/original/3X/c/c/cc6ca9661c06cc55aef0cbd7b5dd8e3f14a7cedd.jpeg" width="690" height="388">
```

---
## \#25 Posted by: Norco Posted at: 2017-04-23T21:26:53.993Z Reads: 241

```
Things have moved on a bit now so here are a few pic updates. I actually plugged it all in a couple of nights ago with a 3s lipo and all seemed to go well. Tonight I wired the battery, antispark and VESC together in the enclosure and (with fingers crossed)  switched it on. All seems to be well. I'll have time this week to set up the VESC while I wait for a friend to trim down and weld my motor mount. Really can't wait to see this thing finished now and give it a ride!
```

---
## \#26 Posted by: Norco Posted at: 2017-04-23T21:31:52.043Z Reads: 247

```
<img src="/uploads/db1493/original/3X/f/d/fd8c74bc8ee823071ff088f392671eb8c1086e4f.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/a/f/af0bcd8b39ff39eca5cfd6ba5aa6e3520db7a64d.jpg" width="281" height="499">
```

---
## \#27 Posted by: Norco Posted at: 2017-04-27T23:50:49.925Z Reads: 229

```
Well I'm not sure that the inserts that I have are going to be suitable for holding the enclosure on but it is otherwise finished so u grabbed a couple of massive velcro straps (you know the ones that hold mattresses on a roll at ikea) strapped the enclosure to the bottom of the board and gave it a run.

OH MY GOD THIS IS INCREDIBLE. 

I mean I know most guys have a big grin when riding but I wasn't expecting that! So much fun I didn't want to stop but it's gone midnight here! Benchwheel remote will take some getting used to (slow mode is really slow so it's really just one mode). 

My mount is welded so to get the right space for the belt I had to add an extra washer to the truck. Don't think this will cause me any issues in the long run. But more pressing is that I lost 2 set screws from the motor pulley. As I will have to remove it to get the trucks sprayed I didn't use loctite. Fail. Will pick up some more but in peoples experience is loctite enough to hold them in and stop the pulley moving across the motor shaft? I have a keyway so not concerned about the pulley slipping. 

I'm still stood here smiling!
```

---
## \#28 Posted by: markyoe Posted at: 2017-05-07T23:44:59.558Z Reads: 198

```
Looks good! Maybe you haven't had a chance to test it yet, but do you know your range/top speed yet? I'm planning on a similar setup with a 10s4p battery, so I'm curious. Do you have a BMS wired up?
```

---
## \#29 Posted by: markyoe Posted at: 2017-05-07T23:45:58.712Z Reads: 194

```
Oh also, how are you monintoring the battery voltage while you ride?

Thanks!
```

---
## \#30 Posted by: Norco Posted at: 2017-05-08T09:55:57.959Z Reads: 187

```
Hey,

Yes I have had chance to do some limited testing before I smashed my motor :confounded:!

Bearing in mind I am a pretty heavy guy (circa 103kg) I was getting about 12 miles or about 20km on a (40.5v) charge with a reserved cut off of 33v (could go lower but there isn't much capacity past 33v). Board tops out at about 26mph (40kph), which I think is plenty fast enough. Crusing at about 15-18mph is comfortable. 

I dont use a BMS.and rely on the VESC cutoffs. What I have been doing until I am confident that there is little drift between charges is checking balancing using the balance plugs. This has been a bit pf a pain to be honest.

One thing I am yet to get my head around is how other people are so confident that the battery build is good. I have had a balance lead come adrift which was an easy fix but even with a BMS I would want to be confident that everything is still wired up ok.

I have a battery monitor which needs wiring in but I want to vacform a cover for it first. Still a work in progress! :slight_smile:
```

---
## \#31 Posted by: markyoe Posted at: 2017-05-08T14:25:44.153Z Reads: 169

```
Considering, that's a pretty good range and top speed. Thanks for all the info. Are you going to go for a battery monitor with an alarm? Also, what heat shrink/wrap did you use?
```

---
## \#32 Posted by: Jinra Posted at: 2017-05-08T14:41:53.713Z Reads: 168

```
I have a bms, and​ for the first couple cycles, i check the voltage of each pack after charging. This keeps my confidence in my pack :)
```

---
## \#33 Posted by: Norco Posted at: 2017-05-08T14:52:47.214Z Reads: 169

```
Probably not as I will be able to see the voltage while riding so know my limits and I doubt I'll ever ride it the full 12miles. The heat shrink was actually a bit awkward to find in the UK. I ended up ordering some 195mm wide stripe from aliexpress.
```

---
## \#34 Posted by: Norco Posted at: 2017-05-08T14:54:16.164Z Reads: 169

```
I'm thinking about rebuilding my pack and checking all of the capacities as I go then add a charge only bms. Going to keep cycling it for now and see though as the drift does seem minimal.
```

---
## \#35 Posted by: taycro Posted at: 2017-11-22T00:39:01.542Z Reads: 97

```
What are the dimensions of this 10s4p pack that you made? Thanks :slight_smile: 
<img src="/uploads/db1493/original/3X/5/5/55f5a68c50ad1e5cf9fd000d51f03c84b7f8f1c7.png" width="281" height="500">
```

---
