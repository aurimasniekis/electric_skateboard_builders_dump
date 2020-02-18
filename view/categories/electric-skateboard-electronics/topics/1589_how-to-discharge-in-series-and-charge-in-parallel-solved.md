# How to discharge in series and charge in parallel \[solved\]

### Replies: 42 Views: 11251

## \#1 Posted by: mohammedex Posted at: 2016-02-28T23:52:14.841Z Reads: 383

```
Hello guys, my question is regarding this 4s2p battery from hobbyking

http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=66309

According to the information I've gathered this battery is has 4 cells hooked up in series in 2 parallel groups (because its a 4s2p)
Does this mean that I have 16000 mah x2 for a total of 32000 mah, or is it 16000 total.
```

---
## \#2 Posted by: psychotiller Posted at: 2016-02-29T00:08:10.528Z Reads: 378

```
Minimum Capacity: 16000mAh
Configuration: 4S2P / 14.8V / 4Cell
Constant Discharge: 10C
Peak Discharge (10sec): 20C
Pack Weight: 1290g
Pack Size: 173 x 74 x 45mm
Charge Plug: JST-XH
Discharge Plug: XT90

These are the specs. This is what you'll have.
```

---
## \#3 Posted by: mohammedex Posted at: 2016-02-29T00:17:20.344Z Reads: 355

```
Thanks for the quick reply.

I've already seen the specs. So it has 8000mah in series for 16000 mah total?
```

---
## \#4 Posted by: cmatson Posted at: 2016-02-29T00:20:04.748Z Reads: 340

```
16000 is the battery capacity, so yes, it two x 8000
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2016-02-29T04:26:18.965Z Reads: 337

```
It's basically two 4s 8000 mah packs in parallel. All you have to worry about is the 4s part and the stated capacity.
```

---
## \#6 Posted by: mohammedex Posted at: 2016-02-29T09:14:43.727Z Reads: 319

```
Thanks a lot, can't wait to receive them. :grinning:
```

---
## \#7 Posted by: mohammedex Posted at: 2016-02-29T12:10:59.311Z Reads: 334

```
I am planning to use two 6s2p batteries instead of the aforementioned 4s battery. and I am also planning to make a waterproof build to acommodate for the rainy danish weather. So I want to make a build that has a sealed enclosure that doesn't require me to swap batteries or remove them for charging.
Being 19 years old, makes you want to go faster all the time, to get that adrenaline pumping, therefore I am going to wire the 6s batteries in series.

I normally just try stuff and if it shorts out I know I did something wrong. I've shorted at least 3 batteries in the last month, that was all fun and harmless as I only ruined 3s or 6s batteries. Shorting the batteries also made me realize that I don't know nearly enough about the electronics I am using as I thought I knew (damn :sweat_smile:, I also dont have any background at all in electronics so that might have something to do with it). And now that I am planning to upgrade from 6s to 12s I feel that working with 12s might require me to be  a liiittle bit more careful. And that's where you guys come in :smiley: 

I made you a little sketch of how I am planning to wire stuff together and would love to get some feedback/suggestions. 

<img src="/uploads/db1493/original/2X/2/2c14bcae17f7a43bdf58b5f12c59dbc96435d700.png" width="690" height="344">

My gut feeling tells me that unfortunately this will burn down my parents house. Do I have reason to believe that?
```

---
## \#8 Posted by: trbt555 Posted at: 2016-02-29T15:00:14.623Z Reads: 317

```
Be careful. If you tend to "feel" your way around setting a board up, you're in for some fireworks !

I think you may be over-complicating things by trying to parallel-charge and series-discharge in one setup.
Too many things that can go wrong, it gets complicated fast. Keep it simple.
If I were you I'd rig my board to discharge in series and charge is series as well. You'll need less wires and less connectors plus there's less that can go wrong.
Here's a quick sketch of what might work:
<img src="/uploads/db1493/original/2X/4/490533cd31c32b19df35c199e62ca059b155920c.PNG" width="542" height="500">

You'd remove the anti-spark loop key when charging and you'd need to rig your balance wires correctly into a series configuration, which is not difficult but needs to be done precisely in the correct order.
I don't know if you already own a charger, you'd need a 12S charger to pull this off.
```

---
## \#9 Posted by: RogerD Posted at: 2016-02-29T15:00:43.535Z Reads: 295

```
As it is, you are trying to link x2 6s batteries in series to get 12s - and feed the VESC. Correct,
You cannot then link the two same batteries in parallel to charge them, as you are trying to do. (that would short them out)
You can only charge the pack as 1 x 12s pack - via the same leads the VESC uses.
You could charge each 6s pack seperately with appropriate leads.
OR, to charge them in parallel you'd have to have a switch on the link between the two packs' (+ and - link) - but that would be very dangerous if you forgot to switch it each time you were charging. You'd have a fire on your hands.

Personally, I'd start with 6s - nothing wrong with 6s. You'll get just the same top speed with 6s and the right gearing. The types of speed you can achieve with 10-12s if you want to, are completely dangerous and unusable. Trust me, I've got experience. You'll end up gearing down your 12s setup to the point you might just as well have gone 6 or 8s and save lots of money on ESCs and chargers.

And yes, you run a very real risk of burning down your parents house. You've shorted three packs already.... I've never shorted a pack. There is a LOT of energy in a 12s pack, let alone a 6s pack. Not only fire, but the ability to weld metal objects through your skin....
```

---
## \#10 Posted by: mohammedex Posted at: 2016-02-29T23:10:55.325Z Reads: 276

```
Sorry for late reply was out all day.
Wow @trbt555 nice work on that sketch. It seems like that would work, but as you said I would need a 12s charger.

Seeing as I have already spent about 80$ + 50$ on 2 decent 6s chargers (both still work without complaints), I would much rather use one of these chargers to charge my batteries instead of spending another 230$ on a 12s charger even if that makes my setup more complicated. I would be happy to get myself a 12s charger if that is indeed the only way this will work, but does everyone here who run >6s setups really have those kind of chargers?

Thanks for the sketch, I'll probably try wiring up my stuff like that if parallel charging is too big of a hassle. I've actually already ordered the xt90s because those would be useful in any case.
```

---
## \#11 Posted by: mohammedex Posted at: 2016-02-29T23:45:08.604Z Reads: 262

```
Man, to be honest, even with your nice input you kinda scare me.
your idea of putting "a switch on the link between the two packs" I really like! Of course forgetting to turn it off would probably make my parents' house suffer catasprophical consequences, but shouldn't that be avoidable if I put a 50v capacitor in my circuit? I've never used a capacitor before, though I believe they can be used to avoid shorts right?

I also started out with 6s with enertion 83mm wheels and 14/36 configuration. I've since upgraded to heli 12s esc without brakes and I can do 45km/h, but my need for speed is making me want to go faster, which is why im looking into making myself a more permanent 12s solution along with 97mm flywheels to up my max speed. I wouldn't say im a pro eboarder, but I've had a finished build for about 2½ or 3 months that I have a few 100 kms on, It almost completely replaced my need for a bike (and we usually bike a lot in Denmark).
```

---
## \#12 Posted by: lowGuido Posted at: 2016-03-01T03:00:55.216Z Reads: 258

```
[quote="RogerD, post:9, topic:1589"]
As it is, you are trying to link x2 6s batteries in series to get 12s - and feed the VESC. Correct,You cannot then link the two same batteries in parallel to charge them, as you are trying to do. (that would short them out)You can only charge the pack as 1 x 12s pack - via the same leads the VESC uses.
[/quote]

you can hook up in series for discharge and then parallel to charge. its a little tricky but not impossible.
you will need a loop key in between the 2 batteries and a parallel charge board to plug into the 2 balance leads once the loop is removed.
discharge as one 12S and parallel charge as two 6S

in fact this is exactly how I intend to wire my next board
```

---
## \#13 Posted by: trbt555 Posted at: 2016-03-01T06:17:47.986Z Reads: 250

```
I actually run 12S on my board.
I also have two 6S chargers.
But I need to open up my box and connect my batteries manually.
This also gives me the benefit of being able to swap packs on the go, which gives me more range than I ever use.
I understand you want to avoid this but I think you'll have a hard time not having to open your box for charging.
```

---
## \#14 Posted by: trbt555 Posted at: 2016-03-01T08:07:06.757Z Reads: 260

```
@mohammedex I've been giving this some more thought and here's a schematic of how you could rig your setup to discharge in series as 12S (insert loop key) and charge both packs separately as 6S using your two chargers (remove loop key).
<img src="/uploads/db1493/original/2X/2/2677600ddb451bf7ea5cb112584e83df8ee9e82a.PNG" width="479" height="500">

@lowGuido, it was your comment that got me thinking, is this what you were planning ? However I don't see how you could rig this to charge both packs in parallel using only one charger and one charge port without adding additional connectors/loop keys.
How would you do this ?
```

---
## \#15 Posted by: lowGuido Posted at: 2016-03-01T08:54:31.821Z Reads: 240

```
Yeah you are on the right track. You just need a parallel charging board to allow your 2 chargers to be replaced with one. Other than that, spot on.
```

---
## \#16 Posted by: mohammedex Posted at: 2016-03-01T12:04:17.928Z Reads: 233

```
That's actually really nice and simple. as lowGuido said it's probably easier with a charging board and a single charger, but is there any danger to always having the balancers hooked up in parallel?

Having to "only" plug in 3 connectors when charging can't hurt :smiley:
```

---
## \#17 Posted by: trbt555 Posted at: 2016-03-01T15:19:23.403Z Reads: 244

```
You can't have your balance or charge leads connected in parallel while your batteries are connected in series.
So basically you'll need to parallel connect everything on the outside of your board so it can be removed for normal operation. 
Which means you'll have two charge ports connected to one charger via a parallel harness and two balance ports connected to a parallel balance board. Plus one loop key port.
```

---
## \#18 Posted by: Dunkirk Posted at: 2016-03-01T17:18:50.855Z Reads: 251

```
If you are going to use separate enclosures I think this way is the best way to change your connection between parallel and series. Also you don't have to buy a new charger.<img src="/uploads/db1493/original/2X/2/24c0c02a0cd52ad3b04ba000a21023443a47b232.jpeg" width="375" height="500">
I am using two 5s2p Li-ion batteris. The xt60 connectors from batteries are glued together. When I am charging the board I connect the parallel connector and parallel balancing connector. When riding I use the series connector.
 Hope this helps!
```

---
## \#19 Posted by: mohammedex Posted at: 2016-03-01T22:20:48.593Z Reads: 248

```
Thanks alot guys, I dont know what I'd do without you. I'll make sure to post lots of pics when I finish my build and receive the VESC's in a months time :)
```

---
## \#20 Posted by: RogerD Posted at: 2016-03-02T16:41:33.365Z Reads: 275

```
You could of course save yourself a WHOLE lot of hassle and just grab a "brick" style 12s charger and charge in series.

http://www.ebay.co.uk/itm/44V-48V-50-4V-4A-Lithium-ion-LiPo-Li-Po-Battery-Charger-12S-12x-3-6V-3-7V-Lion-/321188975380?hash=item4ac85ad314:m:mqmWXCDka0aufrpc5JzfhRg

I use a 6s variant for my board (I have proper 6s RC chargers but this makes it simple and neat)

http://www.ebay.co.uk/itm/221213088365?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
## \#22 Posted by: Hummie Posted at: 2016-03-17T14:56:19.605Z Reads: 260

```
I think u can leave blue connected and charge w one charger
```

---
## \#23 Posted by: DeathCookies Posted at: 2016-03-17T15:15:44.573Z Reads: 261

```
Well,
i have a dual output charger with 2x 400w output.

If i am in a hurry i can charge it (at 16A each battery) in half an hour. (Batteries max charge rate 16A).
Also i already soldered it like the diagramm but for my future plan i am looking to get a bms.

For now i just need to know if i can leave the parallel adapter plugged to the batteries?
```

---
## \#24 Posted by: mccloed Posted at: 2016-03-17T15:38:43.583Z Reads: 250

```
So, your only running 6S?
```

---
## \#25 Posted by: DeathCookies Posted at: 2016-03-17T16:26:17.198Z Reads: 242

```
Yes, only 6S at the moment.
```

---
## \#26 Posted by: mccloed Posted at: 2016-03-17T19:18:44.244Z Reads: 238

```
I agree with @Hummie. If you charge in parallel both batteries have the same connection. Therefore, their is no need for a second charger. You could get a parallel 6s balance adapter like this one: http://www.ebay.com/itm/Parallel-2x-JST-XH-Balance-Adapter-6S-/301177571701?hash=item461f950975:g:a8MAAOSwv0tU~3EY

Although the balance leads probably shouldn't be hit with more than 3 amps.
```

---
## \#27 Posted by: NerijusM Posted at: 2016-03-17T19:23:56.471Z Reads: 234

```
How to charge in series? I have 2x6S in series and I need to charge it with 6S charger. I dont want to unscrew 4 screws every time... I can do ports in case and so on....
```

---
## \#28 Posted by: Hummie Posted at: 2016-03-17T19:38:31.095Z Reads: 234

```
you cant do (2) 6s packs in series with a 6s max charger.  

but you could simply parallel charge them.  I dont know if your charger could monitor all 12 cells though and doubt it.
```

---
## \#29 Posted by: mccloed Posted at: 2016-03-17T21:21:13.610Z Reads: 223

```
I usually charge my batteries on separate chargers if I run them in series. Usually it's two 3s batteries to give me 6s. So, two 3s chargers. I leave the balance plugs on the outside of the enclosure. If you leave them in series and try to use the parallel adapter I listed above, I believe you would fry the adapter.
```

---
## \#21 Posted by: DeathCookies Posted at: 2016-03-17T23:29:41.780Z Reads: 261

```
Hey everyone,
this is a excerpt of my wiring. I left everything i dont need for this question.

<img src="/uploads/db1493/original/2X/c/c3cdd2261717b7be6dcadd611aecd20d1a217559.jpg" width="271" height="500">

When i charge my board i deplug the xt90 plug from the parallel adapter from the vesc [1].
Then i deplug the parallel adapter (blue filled plugs) [2]
After that i plug my dual charger in the two separate charging wires [3]

I am doing part [2] because i think it is not a good idea to have a connection (parallel adapter) between the two batteries. Am i right? Does it matter or do i am able to leave the parallel adapter plugged?
Maybe you have a better idea?

My goal is to create an easy solution for charging my board without the need to disconnect anything at all: just plug two charging cables into it and get ready for charging.

Thanks in advance
```

---
## \#30 Posted by: lowGuido Posted at: 2016-03-17T23:32:31.575Z Reads: 216

```
I merged these topics because the same info is covered.
```

---
## \#31 Posted by: DeathCookies Posted at: 2016-03-18T07:22:33.805Z Reads: 218

```
[quote="lowGuido, post:30, topic:1589, full:true"]
I merged these topics because the same info is covered.
[/quote]

Thank you very much. Somehow I did not find this thread but it is very helpfull!

[quote="trbt555, post:14, topic:1589"]
I've been giving this some more thought and here's a schematic of how you could rig your setup to discharge in series as 12S (insert loop key) and charge both packs separately as 6S using your two chargers (remove loop key).
[/quote]

This sounds like a plan!
```

---
## \#32 Posted by: Bender Posted at: 2016-06-21T12:33:13.489Z Reads: 196

```
<img src="/uploads/db1493/original/2X/3/3da4c7516f7f5063c7b42614869161bf0d18d8e8.jpg" width="479" height="500">
Love your diagram
I think this is what I'm going to try to do
One question, is there a reason I couldn't combined the 2 charge leads into one (so there is only one XT-60 for charging) if I'm going to be charging in parallel?
```

---
## \#33 Posted by: XIII Posted at: 2016-06-21T13:10:15.932Z Reads: 187

```
Read again, that is what LowGuido said.
```

---
## \#34 Posted by: Hummie Posted at: 2016-06-21T13:23:15.570Z Reads: 187

```
If u connect the batteries to a single plug they will be permanently in parallel and then u can't break the connection to do series.
```

---
## \#35 Posted by: Maxid Posted at: 2016-06-21T13:36:46.462Z Reads: 183

```
I think he just means a parallel harness that he connects the two batteries to for charging.
That would work.
```

---
## \#36 Posted by: Hummie Posted at: 2016-06-21T13:37:50.198Z Reads: 180

```
Yea if he removes the plug/connection when riding.
```

---
## \#37 Posted by: Bender Posted at: 2016-06-24T20:23:20.312Z Reads: 183

```
<img src="/uploads/db1493/original/2X/3/3da4c7516f7f5063c7b42614869161bf0d18d8e8.jpg" width="479" height="500">

Ok, is there a way to do this replacing the XT-90s loop key with TB's anti-spark switch?
```

---
## \#38 Posted by: Pablo_702 Posted at: 2016-06-24T22:22:47.718Z Reads: 179

```
<img src="/uploads/db1493/original/2X/b/ba1fffe24e70934051549b4dd5fe6f0cf9082498.jpg" width="374" height="500">
This would be a solution especailly if u have a 12s system
```

---
## \#40 Posted by: fraannk Posted at: 2017-03-29T08:42:26.728Z Reads: 113

```
Sorry for reviving the thread. I just have one question :P 

With this wiring diagram, would you be able to make a custom connector that connects the batteries in parallel outside of the board, as well as connecting the balancing cables in parallel, to replace the two chargers with one 6S charger? 
Just want to be sure
```

---
## \#41 Posted by: Jeefberky Posted at: 2017-07-17T20:18:25.628Z Reads: 81

```
Could your diagram be used with one charger (parallel charging two batteries)? 
I have an antispark switch between the VESC and the batteries. The potential problem I see with using one charger with this diagram is, the VESC (or in my case the anti spark switch) would be powered up by the charger while parallel charging the batteries. Or wont this be a problem because of the anti spark switch?
```

---
## \#42 Posted by: Nicoalix Posted at: 2017-09-27T07:49:24.781Z Reads: 65

```
<img src="/uploads/db1493/original/2X/b/ba1fffe24e70934051549b4dd5fe6f0cf9082498.jpg" width="374" height="500">[quote="Pablo_702, post:38, topic:1589"]
This would be a solution especailly if u have a 12s system
[/quote]

Has anyone implemented this diagram? Its viable? have any risk balancing the batteries?
```

---
## \#44 Posted by: xBRAZILx Posted at: 2018-02-10T12:56:37.505Z Reads: 41

```
man, so simple and clean.
this is the best solution for those already have a charger and don´t wanna buy a BMS.
and have an option to run in parallel if you need more juice instead power.

but one question:
do you protect the balance lead cables?
```

---
