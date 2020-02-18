# What is the downside of single 18650 cells with high (higher) Ah?

### Replies: 77 Views: 5092

## \#1 Posted by: jga Posted at: 2017-02-06T14:35:54.147Z Reads: 348

```
I noted that the nominal Ah of 18650 cells can vary a lot. Typically everybody is using 2500 mAh as the standard, but some can have 3000 mAh or above, which should in theory give you a better range if put in parallel.
But I assume there is a price to pay for that (and I don't mean the price of the cell itself...), considering you can find these cells at a very competitive price. So where is the catch?
```

---
## \#2 Posted by: VikasG Posted at: 2017-02-06T14:47:06.488Z Reads: 336

```
Voltage sag. Higher capacity usually means lower discharge rate. Unless you're making a 8p pack you'll face voltage sag.
```

---
## \#3 Posted by: osbor Posted at: 2017-02-06T14:53:05.326Z Reads: 326

```
oh dear, would that plague a setup such as using two of these 6s 8000mah packs in series?
https://hobbyking.com/en_us/turnigy-graphene-8000mah-6s-15c-w-xt60.html
```

---
## \#4 Posted by: willpark16 Posted at: 2017-02-06T15:20:08.928Z Reads: 316

```
I still cannot determine weather these are as good as 18650s
```

---
## \#5 Posted by: Maxid Posted at: 2017-02-06T15:23:31.735Z Reads: 309

```
Higher capacity cells usually have lower discharge capabilities.
Which is why when you find one that has high capacity AND can handle high currents you usually have to pay for it.
In the end we typically stick to a couple of proven cells and choose the one we can afford.
```

---
## \#6 Posted by: anorak234 Posted at: 2017-02-06T15:35:39.407Z Reads: 293

```
Forget 18650. If you want decent discharge *and* high capacity, I've found 26650 cells to be more than adequate. Basen 4500 is the best way to go
```

---
## \#7 Posted by: jga Posted at: 2017-02-06T16:12:33.947Z Reads: 289

```
Ah! now we are back on the debate 18650 vs 26650. i remember reading not so long ago that it was still better to use 18650, even though I could not remember the excat argumentation. But I must have that somewhere.
i am open to using 26650 if it's really better, I do not have space issue.
```

---
## \#8 Posted by: chuttney1 Posted at: 2017-02-06T16:37:45.235Z Reads: 272

```
Simple answer is to use what fits in your design parameters.
```

---
## \#9 Posted by: Okami Posted at: 2017-02-07T00:30:57.688Z Reads: 267

```
I think the 26650 is generally more expensive.. There's also these 'huge'' headway cells which are really easy to connect (screw terminals) but they also cost quite a lot $$$


--

Look up samsung 30Q. 

These seem to be good cells. Some even say they are /somewhat/ - '_'derated''_ and can reasonably be used or compared to 20A cells..

---

I can totally agree on this one:

[quote="VikasG, post:2, topic:17296"]
Voltage sag. Higher capacity usually means lower discharge rate.
[/quote]

So you should ''chain'' enough in parallel to make ''decent pack'' I think 4P is a good recommendation / start point..
```

---
## \#10 Posted by: Hummie Posted at: 2017-02-07T02:22:45.667Z Reads: 262

```
great battery find!  cheap.
https://hobbyking.com/en_us/turnigy-graphene-8000mah-6s-15c-w-xt60.html

I wonder about these.  only 15c rating but the graphene are touted as really stout at high discharge and maybe it'd be a true 15c all the way down to 3.5 volts.  If it's true 15c, an 8ah pack would be 120amps and good enough for sure.  get them and hook up the vescs to data log and tell us how you do going up steep stuff when your pack is already low please!
48mm for 6s and could be cut down to 2s and slimmer than a typical 2s lipo.    super cheap for a graphene battery which has a life cycle ability similar to li-ion but with power output ability of lipo.  these are a dream come true at that price...if they do 15c
```

---
## \#11 Posted by: PXSS Posted at: 2017-02-07T04:41:50.239Z Reads: 256

```
The issue is that for some reason it became the standard to use 25R cells, they are rated to 20A but are just horrible as far as voltage sag or capacity goes. They perform worse than Sanyo GA cells which are only rated to 10A and have 3500mAh capacity. 

I honestly don't know how this cell became the standard. It's got nothing outstanding in its spec sheet other than its "rating"...

Good high capacity cell:
Sanyo GA
LG MJ1
Samsung 35E
These cells suffer from some voltage sag but a 4P pack is great for up to 20A avg with bursts up to 50A. 

Good high power cell:
Sony VTC6 
Samsung 30Q
LG HG2
These cells sacrifice capacity for power. Voltage sag is non issue and a 4P pack should be good up to 40-50A avg with bursts up to 100A.

IMO, LiPos belong in places where very high power density is really required (rc airplanes/multi-rotors). Not the case in longboards unless you live in a SF hills kind of area or are just trigger happy.
```

---
## \#12 Posted by: mmaner Posted at: 2017-02-07T05:14:51.386Z Reads: 234

```
[quote="PXSS, post:11, topic:17296"]
IMO, LiPos belong in places where very high power density is really required (rc airplanes/multi-rotors). Not the case in longboards
[/quote]

I'm gonna call bullshit on that.  I've run an 8s n x2 10s lion packs and multiple lipo packs.  Hands down lipos give more raw power.  

Sure you can only charge them a third as many times as a decent lion packs.  But they cost a third as much and sometimes less.  

Yes you have to balance charge...But noone out here is 'building' a good board that can't handle balance charging.

Plus...Voltage sag is non-existent, they are incredibly easy to replace, offer many more customization options and can save you $200 on a total build.

The only thing lion has is more watt hours, on average, and any 3 year old can charge them.
```

---
## \#13 Posted by: jga Posted at: 2017-02-07T08:41:38.202Z Reads: 215

```
Thanks @PXSS for these indications. That's what I was looking for.
@mmaner  I had a look at Lipos and you have quite good deals at the moment on HK so it was tempting, but I have the impression that Lipos are too sensitive to handle for a dummy like me, especially in terms of charging. My objective is also to build a modular battery that can travel by plane, and I have the impression Li-ion offer more flexibility from that point of view.
The idea is to have a 10S5P on the model of what @okami did with XT60. As it is to go on a large board with pneumatic wheels, I want to ensure I have enough capacity to do a significant distance. No big hills where i am.
```

---
## \#14 Posted by: osbor Posted at: 2017-02-07T14:07:37.812Z Reads: 206

```
oh lord i do not have nearly the spare cash at the moment to grab a cell, a VESC, and a motor and a remote to test the voltage sag
they seem like very interesting cells though
```

---
## \#15 Posted by: mmaner Posted at: 2017-02-07T14:12:16.907Z Reads: 204

```
[quote="jga, post:13, topic:17296"]
Lipos are too sensitive to handle
[/quote]

They really aren't, they are no more sensitive than lion.  You just have to balance charge, which is very simple.

[quote="jga, post:13, topic:17296"]
a modular battery that can travel by plane
[/quote]

Lipos disconnect with a single plug, much easier than lion.  If you want a 10s battery that is 99wh per pack, then get [Turnigy 5000mAh 2S 30C Lipo Pack](https://hobbyking.com/en_us/turnigy-5000mah-2s-30c-lipo-pack.html).  A little over $100 and you are ready to go.

Seriously, do what you want, that's the beauty of this thing.  But don't let people talk you into something that is simple not accurate.  Talk to different people, get different opinions, then make up you own mind.  You can seriously limit yourself by accepting opinion as fact and acting on that assumed fact.

In this case, I would put x5 2s 30c packs against any lion pack and leave them in my wake.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-02-07T15:05:13.560Z Reads: 194

```
[quote="osbor, post:3, topic:17296"]
oh dear, would that plague a setup such as using two of these 6s 8000mah packs in series?
[/quote]

He's mostly referring to Li-ion cells which usually have a much lower C rating than Lipos. 
Those Lipo cells can handle 120a discharge 
One Li-ion cell will only handle 20-25a discharge and therefore must be multiplied in parallel.
```

---
## \#17 Posted by: jga Posted at: 2017-02-07T16:08:41.199Z Reads: 189

```
Ok but how far would get me 5000mAh?
and how do you charge your 5 batteries?
```

---
## \#18 Posted by: mmaner Posted at: 2017-02-07T16:31:17.709Z Reads: 196

```
Was that you just being argumentative or do you honestly not know?

[quote="jga, post:17, topic:17296"]
Ok but how far would get me 5000mAh?
[/quote]

Depends on how you ride, but probably 70-80% as a 7500mah lion, and a third the cost.

[quote="jga, post:17, topic:17296"]
how do you charge your 5 batteries?
[/quote]

WIth either a 10s charger, or make a 15 pin port for each set of P cells.  I would opt for the 15 pin adaptor port and use a accucel balance charger.

That's actually one of the great things about lipos, most people balance charge so every time you charge your packs you KNOW what condition your cells are in.  Not so much on lion packs.

I don't have anything against lion packs, but for people that want less voltage sag, ease of replacement, modularity & lower cost its a win win.
```

---
## \#19 Posted by: PXSS Posted at: 2017-02-07T19:46:58.403Z Reads: 196

```
Bullshit? 
I stated that LiPos are more power dense than Liions, FACT. 
I stated that they are used where high power density is required. FACT
Voltage sag can be just as good with Liions if you choose the right cell, FACT. 
High power density is not required in longboards, FACT. 
I can make a 10S6P pack that can easily output 3KW and has a capacity of 18Ah and is smaller than your 8S 5500Ah LiPo. FACT

The only real reason to go with LiPos is cost. They are cheap. Dirt cheap. I just bought 12 3S 2.2Ah packs for $45. That's the equivalent energy of 27 Samsung 30Q cells which cost ~4ea but I didnt say anything about cost in my previous post

How do LiPos offer more customization than Liions?
Have you seen White Pony's builds? What do you think those would look like if the were made with massive Lipos?? Please explain this one cause I absolutely think you're just plain wrong. 

Liions can be replaced too, theres a user that is using sleds and can swap out any one bad cell.
There's another user that made his pack split in 5, so he can easily replace modules or disconnect them and fly with them. I still cant believe you said that Lipos are more customizable. 

My post was not me passing my opinions as facts. It was me using facts to answer someone elses question.

And you can also balance charge Liions. I don't know why you have the impression it's any different than LiPos.

<img src="/uploads/db1493/original/3X/d/f/df8a0dc445353b42c8dfa14c74123ae6893ea911.jpg" width="375" height="500">
10S4P pack with real world max continuous power output of 1000W, burst up to 2000W for a minute and a whooping 504Wh *measured*.
Its charged as 2 5S packs and has balance connectors too.
```

---
## \#20 Posted by: mmaner Posted at: 2017-02-07T20:24:46.684Z Reads: 186

```
[quote="PXSS, post:19, topic:17296"]
I can make a 10S6P pack that can easily output 3KW and has a capacity of 18Ah and is smaller than your 8S 5500Ah LiPo. FACT
[/quote]

For 3 times the cost of a comparable Lipo pack, and the lipo pack wold have a higher discharge rate.

[quote="PXSS, post:11, topic:17296"]
IMO, LiPos belong in places where very high power density is really required (rc airplanes/multi-rotors). Not the case in longboards unless you live in a SF hills kind of area or are just trigger happy.
[/quote]

Thats point that I was trying to make.  Not that lipos were better, just different but definitely had a place in the powered skateboard community.  There are many reasons other than cost to go with lipo packs that just cost...higher discharge rates for a lot less money, easier to install and implement than building a lion pack, you always know your cell health when balance charging, all the points I made earlier.

[quote="PXSS, post:19, topic:17296"]
How do LiPos offer more customization than Liions?Have you seen White Pony's builds? What do you think those would look like if the were made with massive Lipos?? Please explain this one cause I absolutely think you're just plain wrong.
[/quote]

What I meant was that you can by 2 5s 5000mah lipo packs and have a 10s 5000mah or a 5s 20000mah with the switch of an XT/bullet connector.  The same can be said with 3s, 4s, etc. packs.  

[quote="PXSS, post:19, topic:17296"]
Liions can be replaced too, theres a user that is using sleds and can swap out any one bad cell.There's another user that made his pack split in 5, so he can easily replace modules or disconnect them and fly with them.
[/quote]

Of course lion cells can be replaced, never said they couldn't, just said it was easier with lipos.  Pull a pack then insert a pack.  No soldering required.  Can't say that about lion packs unless you are talking about sleds, and most people don't like sleds as they are fragile.  I can pull my lipo packs in less than 2 minutes, tape up the connectors and fly with them too, didn't have to make anything special to do it either.

In closing, I was rebutting you statement of...
**LiPos belong in places where very high power density is really required (rc airplanes/multi-rotors). Not the case in longboards.**  I absolutely think you're just plain wrong.

[quote="PXSS, post:19, topic:17296"]
My post was not me passing my opinions as facts. It was me using facts to answer someone elses question.
[/quote]

I was simply offering the "opinion" that you were wrong.  I think making blanket statements like something should not be used to someone who is new to this process is irresponsible.  Most people can drop $600 to build a powered board, most people will think twice about dropping $1000 to $1200.  I've built $400 boards with lipos, not great boards, not beautiful boards, but damned fun to ride.  My current daily board is great and beautiful (said lush as hell) and it is hovering around a $1000 now...with a 10s3p pack that I got at a heavy discount.  My 6s lipo packs were faster, had less sag and still cost half as much. FACT
```

---
## \#21 Posted by: Okami Posted at: 2017-02-07T20:42:20.179Z Reads: 179

```
I thought I might leave this diagram here, for reference to the different li-ion cells and what to expect from them.. 

<img src="/uploads/db1493/original/3X/7/0/70f87794dc472cf862f8fd5b0ea73b6ff61b3817.jpg" width="690" height="487">

It has been taken from Vapers community, so they have ohms / watt rating at the lower side, basically all is said at the two top descriptions - one is for capacity, the next one (lower) for discharge rate)
```

---
## \#22 Posted by: deucesdown Posted at: 2017-02-07T21:37:50.239Z Reads: 186

```
I self-paralyzed over battery considerations. Rather than say this is better than that, I'll add a few more things to consider.

  - you don't want to fully discharge on every trip, that kills batteries fast. plan 50-100% excess capacity
  * same thing for rate of discharge/charge. If you're near the max discharge per cell, performance/capacity/life drop, sometimes a LOT.
  * when considering price, consider price per charge.
  * safety/durability -- what happens if you beat the hell out of a battery? too hot, too cold, overcharge, overdischarge, sit on shelf for a year... does it blow up? does it lose capacity?

Depending on your use, all cells mentioned (and I'll add A123) can make sense.
```

---
## \#23 Posted by: radium Posted at: 2017-02-07T22:36:57.764Z Reads: 190

```
I'll throw my 2c into the ring. I built a 12S5P lithium ion pack using Samsung 18650 30Q for about $300 it could be cheaper depending on 18650 cell and supplier. It's a lot of cells, but it allowed me to configure and arrange them how I wanted and needed to make them fit. The pack has a capacity of 15Ah and 75A continuous discharge rate.

I also have 2 6S Multistar 16Ah batteries that are supposedly 10C max discharge. Realistically for our use, they're about 5C, otherwise the voltage sag is too great. They were about $150 shipped. They are bulky batteries, I had to make a second enclosure just for when I run the Multistars because of their height. I could break them apart and a rebuild the packs, but that negates one of their supposed benefits of out of the box simplicity. They're also heavy.

Overall the 18650 pack is lighter and will offer a longer cycle life and is more configurable, but at 2x the price. I went with that at first because I'm familiar with 18650 cells and didn't know much about lipos.

The voltage sag on the 18650 pack is comparable to the Multistars but they don't get quite as hot running at 75-80A drain. I'm not sure the Multistars could really handle 160A drain for very long I assume they would get very hot.
```

---
## \#24 Posted by: PXSS Posted at: 2017-02-08T01:19:36.030Z Reads: 191

```
The reason I don't see higher discharge rate as a plus is because people have been using the wrong 18650 cell all along for the sake of saving $20-30.

You are talking about using Lipos that can discharge at 200A continuous to discharge on average 20A and peak 100A. A 10S4P 30Q pack can do up to 60A continuous with very little sag and up to 120A burst. 

I can buy these cells for a total of $180. Plus other materials maybe $50
A total of $230 and my time for a 10S4P that kills any LiPo pack In the $100 range maybe even in the $200 range just because you will not be needing the extra discharge ability and capacity on Lipos still sucks plus now youre carrying a massive brick under you. 

My girlfriends build cost a total of $650 with a 10S4P Li-ion pack bms and charger, the pack is the one in the picture above. 

-Lipos have less voltage sag. True but voltage sag is not an issue with the appropriate cells. For example here is the discharge curve for 25R cells which are the standard vs 30Q cells:
<img src="/uploads/db1493/original/3X/1/3/134f66dd216e004465bcde39cdd3686fd39982b9.PNG" width="690" height="387">
Top curve is 0.2A, second is 5A and third is 10A
In a 4P pack, this would correspond to 0.8A (close enough to no load), 20A, and 40A. As you can see, the 30Q cell has less sag at 10A than the 25R does at 5A! In fact, after 50% capacity the 30Q has the same voltage sag at 15A than the 25R at 5A. That means that you see the same voltage sag when pulling 20A on a 10S4P 25R pack than you do pulling 60A on the 30Q pack! That is laughable. 

-Lipos have more power/dollar, True but again that is per dollar. 

-Lipos are easier to install than building your own pack. Not if you use single cells... Using 18650 is the equivalent of using single cells. You can buy an assembled pack that is just as easy to use. Once again it comes down to cost being the difference. LiPos have a way bigger market than 18650 cells and therefore there are made in massive amounts in all kinds of sizes, while 18650 packs are not used widely so finding assembled packs is more costly. 

-You always know the health by balance charging. How is this a pro for Lipos? I can also balance charge Liions/Lipos/Lifepos/nimh. Nothing to do with the battery chemistry itself. 

It all comes down to the dollar signs... which is admittedly a large factor. Large enough that people do choose to go that route. 

Performance wise, there is absolutely no reason to go there though. If you did then your system was designed with the wrong cell with all respect to you.

I think @radium nailed it with the one on one comparison. Performance wise, from what he described 30Q pack is the winner. Once you take cost into account, not too sure.
```

---
## \#25 Posted by: mmaner Posted at: 2017-02-08T01:42:04.276Z Reads: 173

```
[quote="PXSS, post:24, topic:17296"]
I can buy these cells for a total of $180. Plus other materials maybe $50A total of $230 and my time for a 10S4P
[/quote]

That's my entire point, right there in that sentence.  "You" can buy the cells and build the pack.  Most people don't have access to a spot welder or maybe aren't willing to take the time to learn battery layouts or any of a number of reasons.  To buy a 10s4p pack is $400 bucks.  I can buy 2 4S 8000mah lipos for $100 plus $30 for a charger and get the same performance.  

[quote="PXSS, post:24, topic:17296"]
Lipos have less voltage sag. True but voltage sag is not an issue with the appropriate cells.
[/quote]

I've never ridden a board that used lion's that didn't slow down on a 15-20% grade, but with lipos I accelerate. 

[quote="PXSS, post:24, topic:17296"]
Lipos are easier to install than building your own pack. Not if you use single cells... Using 18650 is the equivalent of using single cells.
[/quote]

In what world is it as easy to use individual lion cells as lipo packs?  I use 2 packs, meaning I solder 1 xt60 series adaptor.  2 mins work, tops.  How fast can you build a lion pack?

[quote="PXSS, post:24, topic:17296"]
You always know the health by balance charging. How is this a pro for Lipos? I can also balance charge Liions/Lipos/Lifepos/nimh.
[/quote]

I realize you can balance charge your lion packs.  But do you?  Do most people?  I would say the overwhelming majority of lion users do not.  Why buys a BMS if your going to balance charge?

I even built a 6s lipo pack with a BMS, I prefer to balance charge so I took it off.  My b6 charged faster anyways.

[quote="PXSS, post:24, topic:17296"]
Performance wise, there is absolutely no reason to go there though. If you did then your system was designed with the wrong cell with all respect to you.
[/quote]

Maybe all of my lion packs were badly designed, I doubt it, but maybe.  Regardless, in 10 mins with lipos I am up and running, no worries.  With lion packs, the majority of us are relying on the lion pack builder to make no mistakes, use the best cells, make it dummy proof, etc.  I don't have that worry with lipos.

If I get a bad cell in a lion pack I have to take or ship it to someone to get it fixed.  At least 2 weeks down.  If I have a bad lipo pack I replace it with another that took me 2 days to receive.

Once again, I'm not saying there is anything wrong with lion packs, I will even stipulate that they are moderately safer and "may' not sag if built correctly.  But nothing you've argued has proven that lipos have no place in the building and use of powered boards.
```

---
## \#26 Posted by: radium Posted at: 2017-02-08T01:58:06.015Z Reads: 157

```
Mine doesn't slow down on a 10-15% grade, and I get over 30 miles on a single charge. My total of $300 included a BMS and an appropriate charger. To get a comparable lipo config outside of the Multistar lineup would probably cost around $300 with a charger that could balance charge the batteries simultaneously.

I haven't had my board working for too long, but in my limited testing I've never pulled more than 107A with 2 6355 motors. It was measured with that in line Turnigy power meter. How many amps are you pulling with Li Ion where you start to notice a slow down going up hills?

Another consideration is that I could probably add another 10-20 cells into my 18650 config if I put it into an enclosure the size of the one required for the Multistar batteries.

Either way, both are definitely useable, my only experience is with Multistar because it offered the most capacity for the right price. I imagine other lower capacity packs don't get as hot.
```

---
## \#27 Posted by: PXSS Posted at: 2017-02-08T03:01:25.477Z Reads: 169

```
[quote="mmaner, post:25, topic:17296"]
To buy a 10s4p pack is $400 bucks.  I can buy 2 4S 8000mah lipos for $100 plus $30 for a charger and get the same performance.
[/quote]

If you buy a pack with built with 25Rs sure but they are crappy cells. If you buy a 10S4P made with 30Q cells, then no, the performance will not be the same. Power-wise they might be similar, endurance-wise, you'll ride the 30Q pack twice as far. 
8S 8Ah Lipo = 236Wh
10S4P Liion = 432Wh. 

The point you make is that Lipos are cheap and I agree but performance wise compared to a 30Q pack they get left behind. 

[quote="mmaner, post:25, topic:17296"]
I've never ridden a board that used lion's that didn't slow down on a 15-20% grade, but with lipos I accelerate.
[/quote]
Were they all using 25R cells? If so, point is moot. 
The data above shows that cell sucks. 

[quote="mmaner, post:25, topic:17296"]
In what world is it as easy to use individual lion cells as lipo packs? I use 2 packs, meaning I solder 1 xt60 series adaptor. 2 mins work, tops. How fast can you build a lion pack?
[/quote]
I meant if you used single cell LiPos. Sorry for the confusion. The rest of that paragraph should make more sense now. Lol

[quote="mmaner, post:25, topic:17296"]
I realize you can balance charge your lion packs. But do you? Do most people? I would say the overwhelming majority of lion users do not. Why buys a BMS if your going to balance charge?
[/quote]

What do you think a BMS does exactly?
A BMS is meant to balance cells when fully charged, protect from over voltage, protect from under voltage, protect from over current and protect from a short. All for $40. 

I know your B6 doesn't charge as fast as my $25 200W charger given that the Imax B6 mini is rated for 60W IF you got an authentic one. If not, you should know that you may be overcharging your batteries as the fakes tend to overcharge by up to 0.1V and I recommend you check it with a multimeter next time you charge. 

The overwhelming majority use a BMS, so yes, they do balance their batteries on every charge. There are a few exceptions of course like White Pony and even then he knows how to take care of his cells so that they don't go out of balance.  

[quote="mmaner, post:25, topic:17296"]
But nothing you've argued has proven that lipos have no place in the building and use of powered boards.
[/quote]
I meant it as in performance boards. Cheap builds under $600 that you can put together in less than a day, sure. They're certainly better than ready to ride systems out there. But it doesn't rival a properly built DIY system on the same budget. I spent $700 total plus roughly 3 weekends to get everything up and running on my gfs setup. It was my first build.

Sirry for the slow replies. I'm taking care of the pupp and shes needy.
```

---
## \#28 Posted by: mmaner Posted at: 2017-02-08T03:27:46.831Z Reads: 156

```
[quote="PXSS, post:27, topic:17296"]
If you buy a pack with built with 25Rs sure but they are crappy cells. If you buy a 10S4P made with 30Q cells, then no, the performance will not be the same. Power-wise they might be similar, endurance-wise, you'll ride the 30Q pack twice as far.
[/quote]

No argument here, but 25R's are what is most available, so that's what most of us end up with.  When comparing an 8s lipo pack with 236wh to a 10s3p with 270wh the difference is minimal and the C rating is much higher on the lipo.  The cost is 1/3.

[quote="PXSS, post:27, topic:17296"]
What do you think a BMS does exactly?
[/quote]

I dig that, but I actually see the voltage of each individual cell.  With a lion pack you have to jump through lots of hoops to do that.  

[quote="PXSS, post:27, topic:17296"]
I know your B6 doesn't charge as fast as my $25 200W charger
[/quote]

No argument, but it charges my lipos as fast as a 2a lion pack charger, that's all I was trying to demonstrate.  My accucel and by are legit, I've checked.  I was kind of hoping it wasn't so I could get the $50 gift card from Amazon 😀.

[quote="PXSS, post:27, topic:17296"]
The overwhelming majority use a BMS, so yes, they do balance their batteries on every charge.
[/quote]

Not arguing against that point either, just saying that I actually 'see' the voltage of each cell everytime I charge.  That means I'll see a problem that could potentially be unsafe much sooner than those that assume their BMS is doing its job.

[quote="PXSS, post:27, topic:17296"]
I meant it as in performance boards. Cheap builds under $600 that you can put together in less than a day, sure
[/quote]

That's what I'm saying.  Most people begin the DIY route because an @onloop or @longhairedboy powered board is mondo expensive.  So telling people to NOT use lipos and that the only alternative is a $400 lion pack is going to turn a lot of people off to powered boards.

The way I see it, the more people involved, the more products, the products get cheaper, laws have to change because of pressure from skaters, etc.  All that is good shit.

Go take of your dog, give her a scratch for me.  Good dogs are one of the things, like skateboards, that make life bearable sometimes.
```

---
## \#29 Posted by: mmaner Posted at: 2017-02-08T03:40:59.271Z Reads: 140

```
Here's a question, and keep in mind I'm not asking you to build me a battery, just curious.

If I ordered and had shipped to you with a return shipping label ao you were out no money, only your time, the following...

30 30Q cells, 10 meters of nickel strip, a 10s3p BMS, cell heat shrink and pack heat shrink, 10m of 10g silicon wire, switch, charge port, volt meter and 2a charger what would you charge to build a 10s3p battery?
```

---
## \#30 Posted by: radium Posted at: 2017-02-08T04:00:16.996Z Reads: 141

```
I'd do it for free. I have nickel wire and a bunch of 10AWG copper. Maybe mark it up 20 bucks for the half hour it would take me to spot weld the cells, solder the BMS wires, heat shrink it and drop it back in the post.

Not that it's worth it to build a single pack, but if you are interested in building 18650 packs for other uses(repairing power tool batteries is a big one, as well as old laptop cells or making your own power bricks for portable charging) a reasonable non commercial use spot welder can be had for under $200 including the extension that allows you to do it away from the machine.

I think one reason they're so expensive is they have to be warrantied and they have to offer support should something go wrong.
```

---
## \#31 Posted by: mmaner Posted at: 2017-02-08T04:08:40.155Z Reads: 137

```
[quote="radium, post:30, topic:17296"]
I'd do it for free
[/quote]

I'm trying to figure out a reasonable cost for a 10s3p lion pack with 30q's.  The material cost is about $200, without shopping too hard.

So if a 10s3p with 25r's has a material cost of $140 and the average market price is $360 (low end avg), then the mark-up is $220.  Add the 30q material cost to that mark-up and you have $420. 

I couldn't find anyone to make one for less than $500 and couldn't find a ready-built at all.
```

---
## \#32 Posted by: radium Posted at: 2017-02-08T04:17:41.486Z Reads: 137

```
You can order the cells from verified resellers overseas for much cheaper than they can be had in the states, maybe a group buy on materials could be arranged to negate shipping costs as well. Shipped from China or S. Korea 100+ 30Q cells or similar should be obtainable for around $4.20 each shipped and around $4.00 in larger quantities. I'd have to verify but I imagine quantities of 1,000 or greater could be had as low as $3.75 each.

You run the risk of fake cells even when they come from S. Korea, but it's fairly easy to test when doing an initial bulk charge at 1.5A per cell. The fakes and old batteries being passed off as legit will be much hotter than new, properly stored 30Q or whatever. After identification you can remove the battery wrap of the potential fakes to observe the markings underneath and at this point if you're convinced it's a fake you can drain it and calculate the capacity. Then contact the reseller. This happens even with fairly reputable resellers and probably contributes to the cost of the 18650 packs you were talking about.
```

---
## \#33 Posted by: PXSS Posted at: 2017-02-08T04:36:27.907Z Reads: 134

```
It takes me 2-3 hours of actual assembly time once I have the design finalized and all the materials in hand.
My hourly rate based on my salary is $30 so at most $90. Most likely less, I build things for fun not for profit.
My girlfriend and I love to build quadcopters too!

[quote="mmaner, post:31, topic:17296"]
So if a 10s3p with 25r's has a material cost of $140 and the average market price is $360 (low end avg), then the mark-up is $220.  Add the 30q material cost to that mark-up and you have $420. 

I couldn't find anyone to make one for less than $500 and couldn't find a ready-built at all.
[/quote]

Gross...
Reasons to DIY instead of buying packs...
```

---
## \#34 Posted by: mmaner Posted at: 2017-02-08T04:38:47.731Z Reads: 122

```
I found them for around $5, in quantities over 25, here I. The states.  But that is good info, thanks
```

---
## \#35 Posted by: PXSS Posted at: 2017-02-08T04:40:16.643Z Reads: 136

```
I found them at $33 for 8. Dont remember the website but it was reputable according to endless sphere.

[quote="mmaner, post:28, topic:17296"]
No argument here, but 25R's are what is most available, so that's what most of us end up with.  When comparing an 8s lipo pack with 236wh to a 10s3p with 270wh the difference is minimal and the C rating is much higher on the lipo.  The cost is 1/3.
[/quote]

That's why I build, not buy. Think about motor mounts, it's $10 worth of stock and 10 minutes worth of machining, in fact you can cut 10 in an hour with $25 worth of stock and they sell for $30. Enclosures are $10 worth of ABS, sold for $60. 3D printed wheel pulleys, about $4 worth of material, sold for $30. All of that crap adds up fast!

[quote="mmaner, post:28, topic:17296"]
I dig that, but I actually see the voltage of each individual cell.  With a lion pack you have to jump through lots of hoops to do that.
[/quote]

Again, you can do that with Liions too if you decide to charge them with an RC charger, I did that for the past month while waiting on the BMS and charger to come from China. Over a month because of the Chinese new year...

[quote="mmaner, post:28, topic:17296"]
No argument, but it charges my lipos as fast as a 2a lion pack charger, that's all I was trying to demonstrate.  My accucel and by are legit, I've checked.  I was kind of hoping it wasn't so I could get the $50 gift card from Amazon :grinning:.
[/quote]

I'm still kinda salty about that... LOL

[quote="mmaner, post:28, topic:17296"]
Not arguing against that point either, just saying that I actually 'see' the voltage of each cell everytime I charge.  That means I'll see a problem that could potentially be unsafe much sooner than those that assume their BMS is doing its job.
[/quote]

Agreed, but that's not something that is out of the realm of things you can do with Liions if we are comparing pros and cons.

[quote="mmaner, post:28, topic:17296"]
Go take of your dog, give her a scratch for me.  Good dogs are one of the things, like skateboards, that make life bearable sometimes.
[/quote]
And she's also the reason all my hobbies have come to a stall lately hahaha.
```

---
## \#36 Posted by: mmaner Posted at: 2017-02-08T04:42:41.639Z Reads: 113

```
I'm all for businesses making a healthy profit but $500 is freaking gross misconduct 😀.  But to does offer some explanation as to why some people lean twords lipos.  

It's like diesel vs gasoline.  Diesel engines, as a whole, make better use of diesel fule that gasoline engines do of gasoline.   Diesell is not to be had at every gas station, so it's rairity effects purchasability.
```

---
## \#37 Posted by: mmaner Posted at: 2017-02-08T04:49:14.720Z Reads: 112

```
I found them for $5.45 each, in quantities over 25, at lionwholesale.com.

SAMSUNG INR18650-30Q BATTERY 15A 3000MAH - FLAT TOP - WHOLESALE DISCOUNT, GENUINE AND TESTED

liionwholesale.com/products/samsung-inr18650-30q-battery-15a-3000mah-flat-top-wholesale-discount-genuine-and-tested?variant=2915614724

For 30 that's $163.50 plus $12.15 shipping. Total $175.65.
```

---
## \#38 Posted by: PXSS Posted at: 2017-02-08T04:51:26.810Z Reads: 114

```
I get the 500+ discount since we buy so many cells from them at work.
Ummm here's the link to the 33 for 8, http://www.gearbest.com/batteries/pp_399866.html
```

---
## \#39 Posted by: mmaner Posted at: 2017-02-08T04:53:06.836Z Reads: 115

```
That's $4.18 each, good deal.
```

---
## \#40 Posted by: PXSS Posted at: 2017-02-08T04:56:29.697Z Reads: 116

```
Yep, I also continued our conversation on an edited post above.
I have personally never bought from them since I have access to Liionwholesale discount but according to endless sphere they are legit.
```

---
## \#41 Posted by: mmaner Posted at: 2017-02-08T05:13:14.665Z Reads: 126

```
[quote="PXSS, post:35, topic:17296"]
That's why I build, not buy. Think about motor mounts, it's $10 worth of stock and 10 minutes worth of machining, in fact you can cut 10 in an hour with $25 worth of stock and they sell for $30. Enclosures are $10 worth of ABS, sold for $60. 3D printed wheel pulleys, about $4 worth of material, sold for $30. All of that crap adds up fast!
[/quote]

Without a doubt.  I can handle most of the individual components with tools I have it can use at work.  He'll, I used a pre-WW2 Handdle Dibetail lathe to size some barrel nuts the other day.  I'm just not willing to spend $200 bucks for a spot welder that I'll use 3 times in 3 years.  If I was gonna sell batteries sure, but I barely have time to skate as it is.

I actually figured the cost of my current daily driver if I made everything other than deck, trucks, wheels, bearings, nuts and bolts, motors, VESC's, wire, etc. assuming NO tool cost and it was surprising...  wait for it. ...Savings Total of $184.50.  

it would have been a week worth of work though, so not really value for time in my case.

[quote="PXSS, post:35, topic:17296"]
you can do that with Liions too if you decide to charge them with an RC charger,
[/quote]

I've honestly never heard of anyone doing that, although I assumed you could.  Having built a lipo pack with BMS the architecture of the total pack is very similar.[quote="PXSS, post:35, topic:17296"]
she's also the reason all my hobbies have come to a stall lately hahaha.
[/quote]

That I can dig.  I have a 12 year old Jack Russell (said "miniature T-Rex").  He takes some management to say the least.
```

---
## \#42 Posted by: PXSS Posted at: 2017-02-08T13:47:03.538Z Reads: 116

```
[quote="mmaner, post:41, topic:17296"]
Without a doubt.  I can handle most of the individual components with tools I have it can use at work.  He'll, I used a pre-WW2 Handdle Dibetail lathe to size some barrel nuts the other day.  I'm just not willing to spend $200 bucks for a spot welder that I'll use 3 times in 3 years.  If I was gonna sell batteries sure, but I barely have time to skate as it is.
[/quote]

Our lathe at work must be at least as old as I am lol.
Thank god for CNC milling machines!

[quote="mmaner, post:41, topic:17296"]
I've honestly never heard of anyone doing that, although I assumed you could.  Having built a lipo pack with BMS the architecture of the total pack is very similar.
[/quote]

We do that at work all the time! I have built up to 10S10P packs for some of our UAVs and we charge them in under 2 hours with a 600W RC charger. That's also what I've been doing with my girlfriends setup while I wait for stuff from China. I'm sure I'm not the first one to think of it!

I'm also just going to link this here for you and let you think of the possibilities ;)
http://www.progressiverc.com/isdt-sc-608.html
I considered integrating that into my board when I was thinking about wiring my Liion Pack as 6S.
```

---
## \#43 Posted by: mmaner Posted at: 2017-02-08T13:58:14.696Z Reads: 106

```
[quote="PXSS, post:42, topic:17296"]
I'm also just going to link this here for you and let you think of the possibilities :wink:http://www.progressiverc.com/isdt-sc-608.html
[/quote]

Damn, that is niiiiiiice.  If it would charge 10s I'd order 2 right now.
```

---
## \#44 Posted by: PXSS Posted at: 2017-02-08T14:01:58.582Z Reads: 102

```
I know!!!!
```

---
## \#45 Posted by: radium Posted at: 2017-02-08T14:53:00.091Z Reads: 102

```
I'd be wary of a site claiming to ship from the US at $4.33/cell. If the dudes on endless sphere say it's legit though, they'd probably know better than me. The other major downside to lithium ion cells is that there's a huge number of counterfeits and even reputable resellers like liionwholesale and illumn have received big batches of fake cells that were physically indistinguishable from the real cells. Only an analysis of charge/discharge characteristics when compared with a legitimate cells revealed them to be fakes.
```

---
## \#46 Posted by: radium Posted at: 2017-02-08T14:57:46.135Z Reads: 104

```
That little charger is very cool. I like that it has a fan so it's probably actually capable of real balancing unlike the BMS. BMS is ok for balancing brand new cells that are all nearly identical and thus require very little balancing, but the amount of drain it's capable of applying is pretty pathetic.
```

---
## \#47 Posted by: PXSS Posted at: 2017-02-08T15:20:20.791Z Reads: 103

```
I usually ask for Liionwholesale to provide a batch analysis report with the cells I purchase. They test a few out of the whole batch. I have not had any issues with fakes from them after buying over 1000 cells. I personally checked the first 700ish and then I kinda stopped.
```

---
## \#48 Posted by: Okami Posted at: 2017-02-08T15:24:08.535Z Reads: 108

```
Some of you should check (@mmaner especially):

https://ru.nkon.nl/checkout/cart/configure/id/1452182/

<img src="/uploads/db1493/original/3X/c/f/cf27685d5370f171e0fff2901ea70915b8dcfbc1.png" width="690" height="499"> 

Total is ~98 Eur, that comes close to 105 USD or so..

So 3,5$ a piece..

[EDIT] Im not entirely sure whenever this is a glitch or not.. but I assume you could ''legally order'' as long as they havent changed anything on their page and you should have no problems..


--

<img src="/uploads/db1493/original/3X/f/2/f22ffe3923c0595c63af0b67b38bfb4785d964cc.png" width="456" height="166">

Looks like there should be no tax addition, also!

+ No waiting I believe and at least their EU counterpart seems to be reliable.

---
---
@PXSS I think you meant: http://www.gearbest.com/ 

 I've heard it might take a while before they ship the cells till destination.. there were even some partially shipped packages.. so I would be cautions ordering from there.. unless you've got a patience on your side and have no hurry with them..
```

---
## \#49 Posted by: jga Posted at: 2017-02-08T16:51:31.841Z Reads: 99

```
That's indeed cheap as I saw them at €5.35 on the European part of the nkon site
```

---
## \#50 Posted by: radium Posted at: 2017-02-08T17:07:55.799Z Reads: 98

```
Damn that's cheap. I couldn't find any for less than $3.75, it came out over $4 each with the dangerous goods shipping tacked on.
```

---
## \#51 Posted by: Okami Posted at: 2017-02-08T17:41:35.300Z Reads: 94

```
Im not sure whenever this is true or is it some kind of glitch.. one thing though - this price has stayed such for about 2weeks.. You can see the individual cells.. and if you order less than 20.. the price is a lot higher.. also agree that for Eu site, the price is higher..

Plus, it seems like they have increased the price for ''pre-welded tabs'' onto the cells.. it was something like 20-30cents per cell a while ago.. now it is a whopping 55cents per cell..
```

---
## \#52 Posted by: PXSS Posted at: 2017-02-08T18:17:11.736Z Reads: 91

```
@Okami, are you still getting parcel shipping option? I only get Fedex as an option.
E: if you buy more than 100 Euros, they only ship through fedex...
```

---
## \#53 Posted by: Okami Posted at: 2017-02-08T18:19:55.081Z Reads: 92

```
@PXSS Not sure, you should probably contact them personally.. I never went further with the purchase at them and got my cells from elsewhere (plus, I would need to order from Eu site)..

I hope it is not that way.. otherwise the price ''gets spoiled'' a bit.. and 2weeks also does not sounds as good. as I believe they should be able to ship in a week.. or so.. (+ the risk of tax, they mention in the comment)
```

---
## \#54 Posted by: PXSS Posted at: 2017-02-08T18:37:00.865Z Reads: 89

```
Anyone else from the US want to get in on a group buy of Nkon 30Q cells? I'm buying 40 but shipping is 30eu and can take several weeks so I was hoping to lower the cost of shipping by getting a group buy.
```

---
## \#55 Posted by: mmaner Posted at: 2017-02-08T20:05:33.878Z Reads: 89

```


I'd buy x30 30Q cells, just to try them out.  Get a pack made for the new top speed that's on its way.
```

---
## \#56 Posted by: jga Posted at: 2017-02-08T21:01:19.401Z Reads: 90

```
Anyone knows where we can find them at a decent price in Europe?
```

---
## \#57 Posted by: PXSS Posted at: 2017-02-08T21:13:12.839Z Reads: 89

```
I'll order them tonight. Lets talk details on PM!
```

---
## \#58 Posted by: Okami Posted at: 2017-02-08T21:26:17.035Z Reads: 88

```
@PXSS If you can, please give us some update once it gets sorted out.. im especially interested will you get to avoid the tax.. these taxes can be sometimes a real hindrance
```

---
## \#59 Posted by: PXSS Posted at: 2017-02-08T22:06:41.975Z Reads: 88

```
As far as I'm aware customs doesnt care for packages under 500usd.
```

---
## \#60 Posted by: jga Posted at: 2017-02-09T08:20:36.547Z Reads: 86

```
In UK they can be a PITA even for small amounts
```

---
## \#61 Posted by: Okami Posted at: 2017-02-09T09:53:47.951Z Reads: 81

```
[quote="PXSS, post:52, topic:17296"]
if you buy more than 100 Euros, they only ship through fedex...
[/quote]

This explains the fedex option them.. so I think 30-32 cells is the 'magic number' to go after to get 18usd cheaper shipping
```

---
## \#62 Posted by: radium Posted at: 2017-02-11T12:29:06.841Z Reads: 79

```
mmaner I'm not sure where you're at, but I'd be happy to assemble the pack for you, or guide you through it, either soldering or spot welding. Either way you have to solder the balance leads and + - connections though.
```

---
## \#63 Posted by: radium Posted at: 2017-02-11T12:34:06.157Z Reads: 80

```
If you guys are doing a big group buy I'll throw my recommendation in for battery bro. It won't be as cheap as nkon, but on larger orders of cells it should come out around $4 or so. Also shipping and customer service with him has been top notch.
```

---
## \#64 Posted by: PXSS Posted at: 2017-02-11T13:15:26.541Z Reads: 79

```
@mmaner and I already ordered through nkon. Thanks!
```

---
## \#65 Posted by: mmaner Posted at: 2017-02-11T14:23:05.304Z Reads: 82

```
I'm not sure what type of layout I'm going to yet, most likely a flat 10s3p, sans bms, but I'll let you know when I get there 😀.  Thanks
```

---
## \#66 Posted by: jga Posted at: 2017-02-15T16:23:51.288Z Reads: 82

```
@mmaner I am thinking of following your good advice and go with Lipo to try it. I was thinking of six of these https://hobbyking.com/en_us/turnigy-5800mah-4s-25c-lipo-pack.html to make a 12S 11,8Ah that would surely give a good autonomy to my single motor Evolve GT AT type planned built.
I do not want to make any fancy arrangement for the charge, so I was thinking of just a balance board and plugging the three packs each time with their balance lead.
Any opinion on the choice of battery? Any idea that could simplify the charging (nothing complicated that would freek me out...)?
Thanks
```

---
## \#67 Posted by: mmaner Posted at: 2017-02-15T16:51:37.600Z Reads: 84

```
I would be careful of 12s, it can easily over volt the VESC.  I would go 10s4p with x4 5s 5000mah 30c lipos, 2 sets in series then both in parallel.  As long as you have an easy method to remove the batteries for charging you shouldn't have an issue.  If you don't want to remove the batteries you almost have to use a BMS.
```

---
## \#68 Posted by: jga Posted at: 2017-02-15T18:52:25.557Z Reads: 83

```
Ok. With 5S and 5Ah I should still be ok to travel with them. I will see if I can find them at a decent price.
Is it easy to connect a BMS to Lipos? I believe it should be easier with the balance leads already there.
```

---
## \#69 Posted by: mmaner Posted at: 2017-02-15T20:25:48.900Z Reads: 84

```
It's not too bad.  There are plenty of diagrams on how to do it here.
```

---
## \#70 Posted by: Acido Posted at: 2017-12-24T08:42:19.625Z Reads: 54

```
You cant deny that liiions are as easy to replace as lipos
Lipos are just plug and play while almost all liions are spot welded
```

---
## \#71 Posted by: PXSS Posted at: 2017-12-24T13:49:23.431Z Reads: 57

```
[quote="Acido, post:70, topic:17296"]
***almost all*** liions are spot welded
[/quote]

I highlighted the important bit. 
Also read this:

[quote="PXSS, post:19, topic:17296"]
Liions can be replaced too, theres a user that is using sleds and can swap out any one bad cell.
There's another user that made his pack split in 5, so he can easily replace modules or disconnect them and fly with them.
[/quote]
```

---
## \#72 Posted by: Acido Posted at: 2017-12-24T13:54:26.396Z Reads: 53

```
Here you can find like 500 spot welded and 10 which aren't stop trying to be a smart ass and accept FACTS like you like to say
And that almost is not comparable to every lipo which is plug and play
```

---
## \#73 Posted by: PXSS Posted at: 2017-12-24T13:59:58.886Z Reads: 55

```
It’s Christmas eve and I cannot be bothered. Whatever you say bud.
```

---
## \#74 Posted by: GrecoMan Posted at: 2017-12-24T22:11:58.451Z Reads: 53

```
dude... @PXSS makes li-ion packs for a living. you need to stop pretending like you know everything.
```

---
## \#75 Posted by: i2oadsweepei2 Posted at: 2017-12-24T22:51:04.070Z Reads: 56

```
[quote="GrecoMan, post:74, topic:17296"]
makes li-ion packs for a living
[/quote]

And also introduced us to the advantages of the 30q cell if I remember right. Be good to me memory :cold_sweat:
```

---
## \#76 Posted by: Acido Posted at: 2017-12-25T08:25:48.344Z Reads: 55

```
Liions can be made to be modular and easily replacable but that just isnt the case with people Ive seen only maybe 3 or 4 builds like that
Anyways this is just my personal opinion
```

---
## \#77 Posted by: PXSS Posted at: 2017-12-25T16:53:49.028Z Reads: 49

```
That’s the point. You can make them modular if you want to! If you want to keep it as a single brick, you can also do that. 

***It is up to you***
You build it however you want to. 
Modular packs for traveling. 
Slim pack for cruising. 
Large pack for long distance or climbing steep hills. 
It’s up to the builder, you are not bound to a pack being made a specific way or anything.
```

---
