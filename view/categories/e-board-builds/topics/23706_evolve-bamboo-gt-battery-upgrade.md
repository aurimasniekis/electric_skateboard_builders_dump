# Evolve Bamboo GT battery upgrade

### Replies: 93 Views: 16495

## \#1 Posted by: Mattmccrary8 Posted at: 2017-05-22T19:25:43.496Z Reads: 640

```
Does anyone know how I can upgrade the evolve bamboos battery? The stock battery is absolutely horrible. Does anyone make them for plug and play?
```

---
## \#2 Posted by: anorak234 Posted at: 2017-05-22T19:28:32.111Z Reads: 613

```
@barajabali
```

---
## \#3 Posted by: Eboosted Posted at: 2017-05-23T05:58:25.362Z Reads: 590

```
1. Place an order for 40 Samsung 30Q in imrbatteries.com US$ 200
2. Buy an arduino spot welder US$ 90
3. Buy 4 meters of nickel strip US$ 10
4. Buy heatwrap for the pack
5. Build the battery
6. Diassemble the Evolve pack
7. Assemlethe new battery pack
8. Enjoy a Bamboo GT with more power and no battery sag
```

---
## \#4 Posted by: okp Posted at: 2017-05-23T06:07:21.403Z Reads: 581

```
yeah, that's exactly what I did to my friend :) he's getting now 25km in GT mode with AT tires, no battery sag and more than happy !

you may add
- 7.5 - carve/route an area on the deck above the ESC and remove 5mm so the BMS can sit flat.
- 7.6 - remove the foam on the deck and leave only a banner around 

and you're done :slight_smile:
```

---
## \#5 Posted by: Eboosted Posted at: 2017-05-23T17:41:05.712Z Reads: 554

```
I'm going to do that as soon as I finish my current board on my GF bamboo GT
```

---
## \#6 Posted by: Eboosted Posted at: 2017-05-23T17:55:40.944Z Reads: 540

```
[quote="okp, post:4, topic:23706"]
7.6 - remove the foam on the deck and leave only a banner around
[/quote]

Why would you remove the foam, isn't it better to avoid vibrations?
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-05-23T17:57:41.618Z Reads: 522

```
don't forget to cut about 2mm out of the deck with a CNC or create a 2mm hard plastic riser for the box. 

I have one on my bench right now and 18650s are just a hair too tall for the box. I'm actually doing this right now on two of these bamboos. One is on the bench and the other appears to have been lost in the mail on its way to me, i'm still trying to sort that out.
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-05-23T18:04:46.222Z Reads: 519

```
i'm actually not that terribly disappointed in the GT bamboo given what it is. yeah yeah voltage sag but a 7ah 10s1p prismatic pack ... i mean come on what do you expect... and that's a weird ass motor controller with indivdually switched phases on thier own ICs... where the fuck are the fets.. its alchemy in there. 

the motors and hardware seem solid. I was honestly expecting something a lot worse until i rode it around the block a few times in GT mode. Yeah compared to our boards its a limp dick in a whore house but compared to the shit chinese boards its kind of advanced.
```

---
## \#9 Posted by: Eboosted Posted at: 2017-05-23T18:05:16.264Z Reads: 510

```
Did you see what cells come on the Bamboo GT?
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-05-23T18:09:57.083Z Reads: 509

```
10 individual 7 ah li-ion prismatic pouches connected in series and heatshrinked in blue wrap along with a small BMS. I'd have to look up the cell serials to track them down, but if i had to guess, id say they came from the bargain bin at Goodwill.
```

---
## \#11 Posted by: Mattmccrary8 Posted at: 2017-05-23T18:12:22.740Z Reads: 496

```
I actually messaged you on Instagram Longhairedboy, I live in orlando and built my own board with a swappable lipo enclosure that gets a lot more distance than my Evolve. Could I pay you to teach me how to solder a better pack for my bamboo gt?
```

---
## \#12 Posted by: Mattmccrary8 Posted at: 2017-05-23T18:13:53.735Z Reads: 484

```
Could you make the bamboo gt a 12s pack?
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-05-23T18:15:58.672Z Reads: 480

```
i think 40 cells is the limit of that box, so you're loking at a 12S3P and you're going to have to replace the PCB with a 12S BMS PLUS you're own motor controllers because the evolve is a 10S setup. And when you do that you're going to lose the evolve remote and have to use your own.
```

---
## \#14 Posted by: Eboosted Posted at: 2017-05-23T18:44:27.292Z Reads: 469

```
Did you need to desolder the balance leads from the pouches? Or they had a connector? 

If you can, please check the voltage of each pack, I wonder if the packs have drifting
```

---
## \#15 Posted by: longhairedboy Posted at: 2017-05-23T19:58:07.172Z Reads: 465

```
i didn't tear the pack apart completely yet, just enough to see what was in there. The BMS is definitely the balancing type, and it connects to the main board via UART, apparently.
```

---
## \#16 Posted by: TranxFu Posted at: 2017-05-23T20:04:11.415Z Reads: 470

```
https://endless-sphere.com/forums/viewtopic.php?f=35&t=70435#p1062504

I have pretty much all his builds saved under my favorites lol :smile: @whitepony
```

---
## \#17 Posted by: Jebe Posted at: 2017-05-23T20:19:39.885Z Reads: 466

```
uart hey - thats why they told me a third party battery wouldn't work.
My carbon GT is back at evolve - 40 minute drive no biggie - looks like the BMS is shot - range dropped dramatically.
It stopped displaying individual cell voltages a while ago. They are discharge testing the individual cells. I told them I wanted to see the results and to replace cells that are low. 
Guys in the shop are really good to deal with, had a cruise around on the new evolve one - it's a bigger motor than the GT and goes ok. I'd let my grandmother ride it.
```

---
## \#18 Posted by: Jebe Posted at: 2017-05-25T01:50:52.722Z Reads: 440

```
Evolve confirmed BMS fked and cells 2 and 9 down.
All replaced under warranty :slight_smile:
```

---
## \#19 Posted by: okp Posted at: 2017-05-25T06:00:02.023Z Reads: 442

```
yeah - their BMS has UART + SW port. You need to use their BMS but it's straightforward if you have a soldering iron. Start wiring from the negative of the first bloc (from - to +)
```

---
## \#20 Posted by: Jebe Posted at: 2017-05-25T06:53:21.110Z Reads: 457

```
I don't ride it - it's the fiance's board !
I am planning a revolve.... stay tuned !
```

---
## \#21 Posted by: Eboosted Posted at: 2017-05-25T07:07:35.264Z Reads: 443

```
Damn, my BMS stopped displaying individual cell voltage a while ago as well, I contacted them. And they replaced the BMS under warranty, however as I'm located in Lima Peru I asked if I could replace it locally myself, they agreed and shipped me the BMS, nevertheless, as soon as I change the BMS my warranty is voided. 

Now I can't even go past 2 miles before the remote drops to ECO, so I'm guessing my battery pack is shot as well. 

I'm gonna contact then tomorrow to see if I could get the battery replaced under warranty, but to tell the truth, I rather build my own 18650 30Q battery pack and forget this about this tiny little 10S1P.
```

---
## \#22 Posted by: Jebe Posted at: 2017-05-25T07:20:36.366Z Reads: 425

```
Ship it to me - I'll take it down the road :slight_smile:
Only cost you 2 vesc enclosures and a reaper enclosure :P
```

---
## \#23 Posted by: longhairedboy Posted at: 2017-05-25T14:24:16.099Z Reads: 436

```
I don't solder packs, i tack weld them. But if you want to hang out and learn something, hell yeah. I have an open garage door policy. You can pay me in beer. Also i'll loan you some nickel if you want to try tacking something. 

you can get my welder on ebay.
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-05-26T01:28:56.200Z Reads: 433

```
evolve battery porn. NSFW 
<img src="/uploads/db1493/original/3X/b/2/b218c1b29604180b339610c795ff761008c4672f.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/e/0e5f8f9ed7480257c9c2b4c70ae04cfcfad955ee.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/d/f/df32823480b8b28bcbeb1aaf573293c5a7a15baa.JPG" width="666" height="500">

14awg mains made me spew my coke
```

---
## \#25 Posted by: longhairedboy Posted at: 2017-05-26T03:44:57.383Z Reads: 427

```
heh heh heh 
<img src="/uploads/db1493/original/3X/1/c/1cffbc7657f27cffde2766a68ee1b293f9796ca2.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/c/6cf7f3512bd9b98ee6e9c5d0b977c851bd5e909e.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/1/91881fc93ccf55110b439de6e630d6499cc40461.JPG" width="666" height="500">
```

---
## \#26 Posted by: longhairedboy Posted at: 2017-05-26T04:05:30.126Z Reads: 427

```
oooo hoo hoo hoo 
<img src="/uploads/db1493/original/3X/5/c/5c431d130c658a945bdf2bb1a0801b2b75ba998a.jpg" width="666" height="500">
```

---
## \#27 Posted by: Lambjr088 Posted at: 2017-05-26T04:56:22.125Z Reads: 420

```
What kind of glue is that in between the batteries and do you need a special glue gun for it?
```

---
## \#28 Posted by: Eboosted Posted at: 2017-05-26T05:11:57.536Z Reads: 426

```
Hey man our Bintang enclosure should fit perfectly on your Landyachtz or any droptrough deck

[img] http://i.imgur.com/kyzaaLJ.jpg[/img]
```

---
## \#29 Posted by: Eboosted Posted at: 2017-05-26T05:15:46.490Z Reads: 425

```
I so want to do this right now! That's a perfect use for my 40 cells of 25R laying around
```

---
## \#30 Posted by: okp Posted at: 2017-05-26T06:02:09.565Z Reads: 433

```
:slight_smile:

don't forget:
-  to route the deck below the ESC so you can put the BMS flat, you can leave it there but I thought it was less convenient
- that the board has a pretty significant flex, so you want your pack to be REALLY flexible. So welding the pack classically as you can do for a stiff deck won't work. When I did that few months ago, I did a flexible pack and connected some of the packs in series with AWG and foam to enable maximal flexibility


<img src="/uploads/db1493/original/3X/9/8/980b02f8c14aaa1f80f21951cce14db997690f65.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/a/e/ae8c5c7d884c9695f18c82c66bd0e95fa65a35ad.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/5/25c361c10bb760583bad59e9129b6079b56d0eea.JPG" width="666" height="500">
```

---
## \#31 Posted by: longhairedboy Posted at: 2017-05-26T11:25:10.787Z Reads: 414

```
black hot glue.
```

---
## \#32 Posted by: longhairedboy Posted at: 2017-05-26T11:36:36.924Z Reads: 421

```
i welded a flexi pack by first welding 5 2S4P sections then using short 12awg jumpers between them
<img src="/uploads/db1493/original/3X/4/6/4689ce46e2ec40df13286e4950e26759afedc4b1.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/5/0/5046cf551ad776d5186948f609b80dd51a771a34.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/7/3/73d341135db358beb9bb1388acd33a31e5c4ffd8.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/b/3/b30bfc8341f6710df7891201c0074cddb152ea4d.JPG" width="666" height="500">
```

---
## \#33 Posted by: longhairedboy Posted at: 2017-05-27T02:17:55.609Z Reads: 402

```
mwah ha ha hahaha

https://instagram.com/p/BUlCPywlZD1/
```

---
## \#34 Posted by: longhairedboy Posted at: 2017-05-27T04:20:41.536Z Reads: 400

```
<img src="/uploads/db1493/original/3X/b/4/b4bd7ceae8bc4dd8c48e29cd5fd593a3364cb607.JPG" width="666" height="500">
```

---
## \#35 Posted by: Eboosted Posted at: 2017-05-27T05:00:36.685Z Reads: 394

```
Amazing work, I really love to have all those tools.

The cnc routing machine is sick, perfect for routing decks. 

What range are you expecting on GT mode?
```

---
## \#36 Posted by: okp Posted at: 2017-05-27T06:51:58.267Z Reads: 388

```
25km in GT mode with AT tyres more or less; that's what my friend has
```

---
## \#37 Posted by: Eboosted Posted at: 2017-05-27T07:00:46.719Z Reads: 388

```
How about street tires like abec 11 97mm?
```

---
## \#38 Posted by: okp Posted at: 2017-05-27T07:12:48.122Z Reads: 394

```
don't know, but with AT tyres, we went from 14km (mixed) to 25km in GT mode so you can oversee that's gonna get your A LOT of coverage.
```

---
## \#39 Posted by: longhairedboy Posted at: 2017-05-27T17:01:40.359Z Reads: 401

```
i think we're in business. Forgive the maniacal laughter the entire time, sometimes i get carried away when i'm improving people's premium commercial boards. 

https://instagram.com/p/BUmnLfQlZC2/

also the CNC: Thsts an X-Carve. i got the 1000mm package to start and then modified it. the original price of the unit was $1300 shipped and you assemble it yourself. the mods i've done to it were $100 total. 

you can get the smaller X-Carve and then get the rails you need for your application along with it and do the whole thing at once for a less money. 

im STILL paying that thing off, i put the whole thing on my business credit card the second i got my business account like a damn fool.
```

---
## \#40 Posted by: longhairedboy Posted at: 2017-05-28T06:14:45.912Z Reads: 397

```
I finished it up and wired it in. IT runs, and charges. So far no explosions. We ran it around the block a few ties and we're pretty happy with how it turned out. 
https://www.instagram.com/p/BUm28mvlFqc/?taken-by=longhairedboy

https://www.instagram.com/p/BUnCkZRFWen/?taken-by=longhairedboy

I'm offering this as a service now. You send me your cells and board and i'll mod it for you. $350.

https://longhairedboy.com/collections/frontpage/products/evolve-bamboo-series-gt-battery-mod
```

---
## \#41 Posted by: okp Posted at: 2017-05-28T07:15:23.295Z Reads: 387

```
exactly - that's definitely my view !
```

---
## \#42 Posted by: CheerioCoil Posted at: 2017-05-30T13:55:29.537Z Reads: 388

```
[quote="Eboosted, post:21, topic:23706"]
18650 30Q battery pack
[/quote]

nice work. How long does it take to fully charge that new battery pack? I'm interested in building this, although I lack the tools to carve out the indentation on the deck. Maybe I can try to find a shop somewhere in town that'll let me rent some time on it for an hour.
```

---
## \#43 Posted by: longhairedboy Posted at: 2017-05-30T13:59:19.347Z Reads: 381

```
if you can't find one i'll carve the spots for you cheap + shipping. Consider it a favor of last resort if you can't dig up a guy locally.
```

---
## \#44 Posted by: CheerioCoil Posted at: 2017-05-30T14:23:27.795Z Reads: 382

```
Thanks! That would be swell!
```

---
## \#45 Posted by: Eboosted Posted at: 2017-05-30T20:10:36.891Z Reads: 385

```
<img src="/uploads/db1493/original/3X/e/7/e7549ffa65901fd2ac8aa13befb73b5072d283d6.jpg" width="374" height="500">

Starting my battery upgrade
```

---
## \#46 Posted by: CheerioCoil Posted at: 2017-05-30T22:05:39.868Z Reads: 379

```
Nice. Please show some intermediate steps if you can so I may look at it in the future when I try it :)
```

---
## \#47 Posted by: longhairedboy Posted at: 2017-06-01T18:52:32.081Z Reads: 368

```
looking forward to this! I love that this is a thing and people are doing it.
```

---
## \#48 Posted by: Aggdaddy Posted at: 2017-06-04T02:25:30.402Z Reads: 352

```
Could you build a bamboo GT battery and ship to the client and let the client install?  Perhaps for a lower service fee?
```

---
## \#49 Posted by: longhairedboy Posted at: 2017-06-12T13:59:12.110Z Reads: 350

```
I don't have any plans on doing that. you have to modify the deck with a router or CNC, so there's more going on than just swapping out a pack. Plus i have to use connectors from the original pack, and disposal/recycling of the original evolve pack is included. All together its worth the time to provide the service, but just building flexy packs wouldn't be something I could charge as much for and becomes less worth my time. It's a precarious balance. I almost didn't offer this service at all, but now that i've done three of them I'm getting into a groove with it.
```

---
## \#50 Posted by: Aggdaddy Posted at: 2017-06-12T14:15:06.965Z Reads: 346

```
Oh ok.  I thought I could make the mod with a dremel.
```

---
## \#51 Posted by: sl33py Posted at: 2017-06-12T23:10:21.397Z Reads: 351

```
[quote="longhairedboy, post:39, topic:23706"]
also the CNC: Thsts an X-Carve. i got the 1000mm package to start and then modified it. the original price of the unit was $1300 shipped and you assemble it yourself. the mods i've done to it were $100 total.
[/quote]


What did you modify and why?  I'm *this* close to getting CNC...  appreciate your experience and suggestions.

I just rode w/ a bunch of Bamboo GT guys last week on a meetup ride in my area.  What does this battery upgrade cost (if i'm chatting with one and want to send them your way)?

Great thread and pics LHB!
```

---
## \#52 Posted by: longhairedboy Posted at: 2017-06-13T18:04:05.192Z Reads: 345

```
$350 plus cells. I have it listed on my site now. Usually i send people to liionwholsale.com for the cells but you can get them wherever you want. Send them to me along with the board and i'll do the whole thing and send it back within a couple of days of getting the cells and board. I'm trying to do real fast turnarounds on these.

Oh also the mods on the x-carve: i made the Y axis longer to about 5' and the x-axis shorter to about 2.5 feet. I did that so i could cut out complete decks and not take up more space than i need to. 

On the bamboos i take out wood for the higher battery and more wood for the taller electronics stack, i have to take the BMS out and put it on top of the ESC so there needs to be a cavity there.
```

---
## \#53 Posted by: BelviGER Posted at: 2017-06-26T22:18:07.285Z Reads: 326

```
How much extra vertical space was needed in your experience to make the 18650s fit?

And how much would you charge just for the battery pack, sans wood milling?
```

---
## \#54 Posted by: longhairedboy Posted at: 2017-06-26T23:39:01.109Z Reads: 333

```
about 2 millimeters i beleive it is. packs are $200 plus cells and don't include BMS or switches or chargers or any of that.
```

---
## \#55 Posted by: Eboosted Posted at: 2017-07-05T05:50:25.432Z Reads: 342

```
Ok, I started today.

I think I'm gonna use this layout so there no need to use a router to make room for the BMS.

[img]http://i.imgur.com/bRUQgc6.jpg[/img]
```

---
## \#56 Posted by: davidbonde Posted at: 2017-08-08T13:15:34.587Z Reads: 318

```
How is it going? Think I want to make an upgrade a Vinter projekt. But I have absolutely no experience to that kind of work. Is it manageable?
```

---
## \#57 Posted by: longhairedboy Posted at: 2017-08-08T13:37:13.614Z Reads: 314

```
Fascinating. You still have room to not move the BMS when stacking like that after wiring everything? I feel like i tried this... I know i tried a lot of things...
```

---
## \#58 Posted by: Eboosted Posted at: 2017-08-08T17:15:46.622Z Reads: 311

```
Yes, there was a perfect fitment with the cells  stacked this way, however the wiring was a PIA, so I  switched the cell perpendicular to the deck, I also had to increase the size of the snclosure with fiberglass so there was no need to route the deck for the BMS.
```

---
## \#59 Posted by: nige Posted at: 2017-08-25T15:53:08.441Z Reads: 302

```
Hi I am trying to sort this upgrade, being in the uk longhairedboy is not a option.Would anyone have the cad drawings for the cut outs for the BMS and pack? Or anyone have dimensions I can work with ? Any help would be fantastic.
```

---
## \#60 Posted by: davidbonde Posted at: 2017-08-26T18:30:27.137Z Reads: 305

```
I am interested in this well. This might be my winter project.
```

---
## \#61 Posted by: CheerioCoil Posted at: 2017-10-07T22:34:59.504Z Reads: 290

```
I ordered all the materials needed for this project. I've been debating whether to do it myself or to hire someone to make it for me. In the end I decided that since I'm hooked on electric skateboards now, I might as well start collecting the tools needed to make additional batteries in the future. Well, here goes!
```

---
## \#62 Posted by: WhySpace Posted at: 2017-10-22T15:30:25.018Z Reads: 281

```
Is there an electrical schematic around?
```

---
## \#63 Posted by: darkkevind Posted at: 2017-10-22T16:13:00.944Z Reads: 280

```
If anybody needs this done in the UK I can help with the battery pack upgrade... I've just completed two and I have the correct Evolve-specific 11 pin connector for the BMS.

Pm me for more info...
```

---
## \#64 Posted by: Rockinjohn Posted at: 2017-11-22T04:45:46.564Z Reads: 259

```
Just got in on ThisGuyHere group buy on 40 cells.  Will be down your way in about a month how much time do you need.  Have you ever thought about taking on  One Wheel? I have two and I burn through both before the Bamboo dies.
```

---
## \#65 Posted by: Bowski Posted at: 2017-12-18T16:02:06.341Z Reads: 254

```
Hi All,

I am offering battery mods for Bamboo GT and Carbon GT in Germany.

If you are interested in this, please sent a PM. or contact me via WhatsApp 015120940064
```

---
## \#66 Posted by: fstclyz Posted at: 2018-02-13T00:13:37.821Z Reads: 232

```
I have a Evolve GTX and want the Samsung battery upgrade via "longhairedboy" but is there a new larger cover I can put on it rather than routing out wood on the OEM deck?

With all that flex, I'd rather not comprise the deck by taking wood out of it.
```

---
## \#67 Posted by: darkkevind Posted at: 2018-02-13T00:59:13.412Z Reads: 229

```
http://kevindark.co.uk/evolve-battery-upgrade :+1:
```

---
## \#68 Posted by: fstclyz Posted at: 2018-02-14T00:17:33.032Z Reads: 225

```
Kevin's new battery looks great.  I can solder so that shouldn't be a problem.  I think I'd opt for a 6mm foam or similar spacer over routing into the deck.  

Has anyone who routed out their deck noticed increased flex?  or maybe less durability due to losing that wood?
```

---
## \#69 Posted by: darkkevind Posted at: 2018-02-14T00:25:12.726Z Reads: 220

```
One of my customers said he really regrets routing the deck and that now he feels like it's going to snap on every ride :frowning:
```

---
## \#70 Posted by: GrecoMan Posted at: 2018-02-14T01:17:03.243Z Reads: 211

```
can’t he put a layer of glass on the bottom if it bothers him that much?
```

---
## \#71 Posted by: Deckoz Posted at: 2018-02-14T01:30:05.273Z Reads: 212

```
[quote="GrecoMan, post:70, topic:23706"]
layer of glass
[/quote]

That's a pretty good idea too. And it's already welled so you could easily do a resin injection on the glass to keep it super thin.
```

---
## \#72 Posted by: darkkevind Posted at: 2018-02-14T01:45:26.188Z Reads: 205

```
Yeah could do I guess. I'll suggest it to him ;)
```

---
## \#73 Posted by: longhairedboy Posted at: 2018-02-15T17:08:30.970Z Reads: 207

```
dug it too deep?
```

---
## \#74 Posted by: darkkevind Posted at: 2018-02-15T17:28:26.285Z Reads: 206

```
It's possible.. I don't know as I didn't do it but he feels it's too flexy now... :confused:
```

---
## \#75 Posted by: longhairedboy Posted at: 2018-02-15T17:35:21.374Z Reads: 210

```
*opens trampa's customer service handbook*

ok.. lets see what you could have done here... hmmm... ok... yeah. 

* Did you try blaming the customer and making them feel bad for even asking?
* Did you try hitting it with hammer?
* Have you tried trademarking the mod and telling them that's what they get for trying to produce a trademarked mod and make it seem like you're the only one that can do it?
```

---
## \#76 Posted by: mmaner Posted at: 2018-02-15T18:03:16.383Z Reads: 210

```
[quote="longhairedboy, post:75, topic:23706, full:true"]
opens trampa’s customer service handbook

ok… lets see what you could have done here… hmmm… ok… yeah.

Did you try blaming the customer and making them feel bad for even asking?
Did you try hitting it with hammer?
Have you tried trademarking the mod and telling them that’s what they get for trying to produce a trademarked mod and make it seem like you’re the only one that can do it?
[/quote]

All I can say is its a good thing you don't have boobs or I'd kiss you for that :slight_smile:
```

---
## \#77 Posted by: longhairedboy Posted at: 2018-02-15T18:10:18.800Z Reads: 206

```
i think you can still kiss me if you say "no-homo" afterwards. I'm pretty sure that's how it works. In fact you can have full on gay sex with a dude if you say "no-homo." It means you're not gay, just appreciative. 

at least that's what i've heard from the myriad homophobic maladjusted emotionally inept insecure egomaniacal... err..  i mean people.
```

---
## \#78 Posted by: mmaner Posted at: 2018-02-15T18:12:45.166Z Reads: 204

```
Well...I'm definitely maladjusted and egomaniacal, but definitely not homophobic.  Live and let live right ? :slight_smile:
```

---
## \#79 Posted by: longhairedboy Posted at: 2018-02-15T18:19:15.095Z Reads: 202

```
i've felt the kiss of death.. and you know what the reaper said to me as i was waking up on the street?

*"no homo bro..."*
```

---
## \#80 Posted by: GrecoMan Posted at: 2018-02-15T18:20:21.721Z Reads: 200

```
weird... same thing happened to me with skatan this morning 🤔
```

---
## \#81 Posted by: anorak234 Posted at: 2018-02-15T18:50:03.685Z Reads: 189

```
@longhairedboy I'm 666% sure you're the most entertaining person on this forum
```

---
## \#82 Posted by: Maralc Posted at: 2018-04-17T12:15:11.529Z Reads: 170

```
4 months later I still haven't received my battery and Kevin doesn't reply my messages anymore. What else to say?
```

---
## \#83 Posted by: darkkevind Posted at: 2018-04-17T12:39:01.583Z Reads: 173

```
@Maralc you know I've been trying to get this pack sent to you in Australia! However, every effort so far has failed... I've wasted over £150 on shipping because you told me how badly you wanted this battery.

However, I think it's time to give up! As you paid your deposit by bank transfer, I've already asked you for your bank details in order to send your money back...paypal would be easier though... but you haven't responded as yet...?
```

---
## \#84 Posted by: Maralc Posted at: 2018-04-17T12:52:21.599Z Reads: 172

```
I know you were trying. But last time you replied my messages was March 11. I messaged you many times since without feedback. Providing the bank details right now.
```

---
## \#85 Posted by: Maralc Posted at: 2018-04-17T12:56:41.271Z Reads: 180

```
The only shipment I know of was the first one which you declared as a marble board without discussing with me. Customs caught it and returned as false declaration. After the first one was returned there was no other feedback about any other shipment or any replies to my inquiries.
```

---
## \#86 Posted by: darkkevind Posted at: 2018-04-17T13:02:31.456Z Reads: 181

```
Well that's not entirely accurate. Turns out everything going by air to Australia gets x-rayed before it gets on the plane... Each time this has happened. It doesn't happen with any other destination I've found, just Australia which is why I no longer state I can ship there...

As soon as you provide me with your bank details I can send your deposit back.
```

---
## \#87 Posted by: CheerioCoil Posted at: 2018-05-16T03:16:48.120Z Reads: 171

```
Hmm...this thread hasn't died yet. Welp. Like everything in life, I procrastinated on this project and finally finished my 10s4p battery with LG HG2 cells 7 months later. It works great, although with AT wheels on my Evolve Bamboo GT it only goes 13 miles from 100% to 0%. It's a success, although I still wish it could go even farther. Anyway... good experience. I might try to double this capacity again and get a deeper enclosure from somewhere.
```

---
## \#88 Posted by: TarzanHBK Posted at: 2018-05-16T15:24:49.545Z Reads: 166

```
There is something wrong with your battery. A 10s4p of HG2 brings you much further, even under heavy stress with that board!
```

---
## \#89 Posted by: CheerioCoil Posted at: 2018-05-16T15:50:17.822Z Reads: 167

```
I don't know what to compare to though. Some reviews online say the stock battery can fetch 10-11 miles on flat terrain. My tires were underinflated so that could have contributed to the range that I got. I don't know. Not sure how I would test my battery capacity.
```

---
## \#90 Posted by: CheerioCoil Posted at: 2018-05-16T15:56:57.041Z Reads: 164

```
I also want to add that half of my test was done on dirt paths. I should do it on a flat asphalt surface...
```

---
## \#91 Posted by: CheerioCoil Posted at: 2018-05-30T02:20:21.988Z Reads: 155

```
I discovered several breakages in my welding lol. I made the pack a bit more flexible too after tearing it completely apart. It's pretty safe now. I get around 20 miles on fast mode. Good enough for me. I'll build a Trampa-type board for my next project.
```

---
## \#92 Posted by: Wizeartz Posted at: 2019-04-06T01:16:42.267Z Reads: 71

```
I suspect New Zealand are lithium-ion Nazis too :frowning:
```

---
## \#93 Posted by: G_FPV Posted at: 2020-02-06T16:20:40.208Z Reads: 9

```
Hi All, been reading through loads of threads on this topic.....why because my BMS is dead AGAIN and I`m not going to pander to Evolves Ludacris fees`s all for it to be the only component again that has 'Water' damage.  

Does anyone know if the UART code has ben collected or it there is a UART and switch bypass?

Ultimately I`ll move to Dual Vesc option, but right now I`d prefer to not spend the money and also work on a solution others could use?

Thanks to all for the valuable input around this topic so far 

G
```

---
