# Vedder anti spark switch v1.3 *KIT* \[currently out of stock\]

### Replies: 105 Views: 13338

## \#1 Posted by: DeathCookies Posted at: 2016-09-21T18:41:51.642Z Reads: 943

```
Hey folks,
I wanted to build myself a vedder anti spark switch to save some money. So i decided to buy a few more of the components which i will sell. Please keep in mind that i am selling a **KIT** not a finished product!
 
[Vedder anti spark switch github](https://github.com/vedderb/SparkSwitch)
<img src="/uploads/db1493/original/3X/e/f/efc6f1448d3135228027dc91ce41040f3313a902.jpg" width="666" height="500">
The kit i am offering includes the following components:
R1, R2, C1, D2, Q1, Q2, PCB, 3x soft switches and 2x fuses (40A / 58V)
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/6/7/6788abc41e4d606599fc8aa5d3885c0d1d8c9710_1_666x500.jpg

To build a switch yourself you will need this kit + soldering skills (smd soldering for the mosfets) + wires + plugs. I assume you will have everything to build one yourself.

The result would looks like this:
<img src="/uploads/db1493/original/3X/1/7/176585ecbd4c5c3d1ec1d73259fc1a4ae5018781.jpg" width="666" height="500">

You can use another switch than the given one! You can use any Rocker Switch. E.G. you could use such a LED push switch:
<img src="/uploads/db1493/original/3X/0/5/05738bcce884d8195ee7aba7189e7fc8300e9574.jpg" width="480" height="360">
**Attention:** 
There are different ways to illuminate the switch when powering the board. E.G. use a BEC attached after the vedder switch to illuminate the softswitch. But if you do not want an external power supply you can buy an "illuminated rocker switch". Generally they are not as nice looking as the normal led push button but it will work out of the box!
**Wiring push button**:
Normally there are 5 pins: C, NC, NO, +, -
Ignore + and -. These are for the LED only.
<img src="/uploads/db1493/original/3X/e/5/e594848ed3834bdb62218a6d301a8aadfd2dc95a.jpg" width="624" height="500">


I am offering this KIT for 25€ + shipping.
I am located in germany but DHL says on [their site](https://www.deutschepost.de/de/b/briefe-ins-ausland/warenversand-international.html) that it does not matter in which country i will send them, the price will always be the same: 3,70€ + 2,50€ insurance/tracking.  :)

Somebody else has not the possibilty to solder the two MOSFETS on the PCB. Without an smd solder it is actually hard... So i will offer to solder the mosfets on the PCB for additional 3€ that you only need to solder the other components (which can be made with a normal solder iron)

If you buy more than one kit the shipping cost will be the same because the components are not big and will fit in a letter no matter how much.

**NON EU**-Customers:
If you want me to declare the package with a lower price (because of custom fees) the insurance will just cover the lower declared price in case of loosing the parcel on the way...

If you have interest just write a nice PM ;)
```

---
## \#2 Posted by: sl33py Posted at: 2016-09-21T20:01:03.514Z Reads: 687

```
This is a great option for folks in Europe!  I did the same and sold extra's (donating to Vedder some of the profit) and the only downside was cost to ship international is spendy!

A word of caution for those who get any kit - SMD soldering is not the same as regular soldering.  You will want a hot-air rework setup ideally, or look at reflow via oven or even "skillet" (google it).  Then you can solder the cables, fuse, etc.  But those small components can be fiddly if you haven't done SMD soldering before.  not actually that hard - but look before you leap!  (not trying to put a damper on your sale @DeathCookies) 

GL w/ your extras!
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-09-21T20:02:08.798Z Reads: 640

```
You are totally correct. I will edit my post but for everything except the mosfets you wont neet smd soldering ;)
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-09-22T17:52:36.358Z Reads: 593

```
Edited the first post
```

---
## \#5 Posted by: Pantologist Posted at: 2016-09-22T18:25:59.957Z Reads: 571

```
Is the picture of the final switch what you soldered? The traces of the mosfets are okay all bunched together like that?
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-09-22T18:38:07.112Z Reads: 549

```
[quote="Pantologist, post:5, topic:9949"]
Is the picture of the final switch what you soldered?
[/quote]

Yes, that is the one i have soldered myself.
[quote="Pantologist, post:5, topic:9949"]
The traces of the mosfets are okay all bunched together like that?
[/quote]

Only the left pin of both mosfets need to be seperated from the other pins! You can see in the plot of the switch that only the trace of the left pin goes somewhere else and the other pins go to the big trace down ;)

PS: i have tested my switch and it works flawlessly with 12S :)
```

---
## \#7 Posted by: Pantologist Posted at: 2016-09-22T18:49:40.538Z Reads: 469

```
Oh good. I bought the same kit before and thought I screwed up bad when the traces melted together!. I'll go ahead and test it then.
```

---
## \#8 Posted by: jackw Posted at: 2016-09-23T00:10:05.193Z Reads: 453

```
I've made one myself, I did managed to get everything soldered with a regular iron, just took a little time and patience :relaxed: Could use a spare though!
```

---
## \#9 Posted by: DeathCookies Posted at: 2016-09-23T11:56:18.971Z Reads: 445

```
I am regularly updating my first post. If there is something wrong or if i missed something please tell me ;)
```

---
## \#11 Posted by: DeathCookies Posted at: 2016-09-23T12:57:04.400Z Reads: 468

```
[quote="Pantologist, post:10, topic:9949"]
What are those standoffs for the fuse called?
[/quote]

What do you mean by that?


[quote="Pantologist, post:10, topic:9949"]
Any idea what their amp limit is?
[/quote]

I do have
[quote="DeathCookies, post:1, topic:9949"]
fuse (40A / 58V)
[/quote]
Here is the [datasheet](http://www.distrelec.de/Web/Downloads/a_/de/owTAC58V_data_DE.pdf?mime=application%2Fpdf)
It is rated to 80A for 5 seconds (if i am not mistaken?)
<img src="/uploads/db1493/original/3X/a/c/ac2c5b6bba5cc158931c90f69bc41ff74f9c776a.JPG" width="346" height="152">
```

---
## \#12 Posted by: Pantologist Posted at: 2016-09-23T12:59:04.642Z Reads: 432

```
Sorry, wrong thread.
```

---
## \#13 Posted by: jak Posted at: 2016-09-25T14:10:13.626Z Reads: 441

```
i will take one with the mosfets pre-soldered. 

<img src="/uploads/db1493/original/3X/c/7/c754dffe45ccabfe04d6cd0955ea33d7970437e8.png" width="400" height="224">
```

---
## \#14 Posted by: jackw Posted at: 2016-10-10T10:33:07.437Z Reads: 433

```
Received mine! All soldered up ready to be wrapped and good to go!

<img src="/uploads/db1493/original/3X/3/2/3268896c040784fc2f1cab2d88db255d6d414e94.jpg" width="669" height="500">

Just wanted to say a big thanks to @DeathCookies for the kit, the pre-soldered fets made my life a lot easier when putting it together. Great communication when going through the sale also! Would definitely recommend grabbing one of these kits if you are looking for a switch and don't mind a little bit of soldering (it's pretty fun anyway).
```

---
## \#15 Posted by: DeathCookies Posted at: 2016-10-10T16:14:39.479Z Reads: 412

```
Awesome job with the bullet connectors especially the heatshrink!
```

---
## \#16 Posted by: skinny_e-boarder Posted at: 2016-10-11T12:56:15.310Z Reads: 404

```
Just bought one of these kits yesterday.
DeathCookies was really responsive, he even sent me pictures of the presoldered mosfets and documented my order.
Today i received tracking information.
That is some awesome service :smiley:
I am reallly looking forward to solder the kit. As soon as it arrives, I am going to post some pictures of the finished pcb. 
I would buy from Daniel again. :slight_smile:
```

---
## \#17 Posted by: DeathCookies Posted at: 2016-10-11T13:08:54.043Z Reads: 398

```
Looking forward for the pictures :)
```

---
## \#18 Posted by: jak Posted at: 2016-10-12T16:29:12.878Z Reads: 400

```
ordered mine and received everything very promptly. DeathCookies is the man! fets pre-soldered for ease. will post a pic when i get the time to solder it up. if you want great service this is the kit for you. DeathCookies spent a ton of time bouncing ideas back and forth and explaining the process. buy em up boys you wont be disappointed.
```

---
## \#19 Posted by: TarzanHBK Posted at: 2016-10-13T07:22:28.291Z Reads: 396

```
is it possible to go with a higher rated fuse with that switch? Does someone knows the current limits?

because it would be cool to use that with low V - high A systems also.

with a imaxx mdp fuse for example:

http://www.distrelec.de/de/kfz-sicherung-midioto-60-58-vdc-gelb-imaxx-mdp060/p/11029346?channel=b2c&price_gs=1.6779&wt_mc=de.cse.gshop.de.-&source=googleps&gclid=CIuznZec188CFcWVGwodxhAFSQ
```

---
## \#20 Posted by: DeathCookies Posted at: 2016-10-13T08:06:19.453Z Reads: 396

```
Current limit of the mosfets is 240A.
Someone already had the idea to solder the fuse two times (in parallel) to double the current.

Actually i am sending every one two fuses so you should get 80A if i am not mistaken.
```

---
## \#21 Posted by: TarzanHBK Posted at: 2016-10-13T12:14:51.164Z Reads: 404

```
good to know thx :slight_smile: 

hmm interesting concept.. it´s possible but you have to take care that both cables and everything has the same length, to avoid any differences in load. 
I´d prefer a single fuse to be safe :monkey:
```

---
## \#23 Posted by: skinny_e-boarder Posted at: 2016-10-14T13:57:38.139Z Reads: 393

```
<img src="/uploads/db1493/original/3X/5/c/5c63d05561976518a07ca24461f1b4ad83d52ea6.jpg" width="690" height="388"> Here we go :D Bought the wrong switch, so here is a picture without one
```

---
## \#24 Posted by: DeathCookies Posted at: 2016-10-18T16:16:48.631Z Reads: 380

```
Updated the first post:
Added the matching soft-switch to the KIT for the same price of 25€ per KIT.

Now you will only need some wires and your system-matching plugs ;)

_Still some left._
```

---
## \#25 Posted by: Rob69de Posted at: 2016-10-18T16:54:29.686Z Reads: 364

```
Woul like one, paypal?
```

---
## \#26 Posted by: DeathCookies Posted at: 2016-10-18T18:03:55.771Z Reads: 353

```
pm sent. :)
```

---
## \#27 Posted by: sl33py Posted at: 2016-10-18T18:34:05.418Z Reads: 350

```
Super lame - see i was actually in DeathCookies' thread.  Sorry dude!  Not trying to poach...
```

---
## \#28 Posted by: smurf Posted at: 2016-10-18T18:57:57.126Z Reads: 347

```
Get another batch 😊
```

---
## \#29 Posted by: susplus Posted at: 2016-10-19T10:59:08.349Z Reads: 345

```
am I to late :( ???
```

---
## \#30 Posted by: Mox Posted at: 2016-10-19T19:58:04.825Z Reads: 340

```
If you happen to get more please contact me 
thanks
```

---
## \#31 Posted by: sl33py Posted at: 2016-10-19T20:52:06.326Z Reads: 344

```
Disregard - thought i was in _my_ "kit" thread.  Sorry DeathCookies!
```

---
## \#32 Posted by: DeathCookies Posted at: 2016-10-20T03:43:46.483Z Reads: 332

```
@susplus @Mox  I still have some left! 

@sl33py  no problem
```

---
## \#33 Posted by: susplus Posted at: 2016-10-20T19:10:12.497Z Reads: 317

```
Great...how can i put my hands on one :slight_smile:
```

---
## \#34 Posted by: DeathCookies Posted at: 2016-10-20T19:28:16.983Z Reads: 310

```
I prefer pm ;)
```

---
## \#35 Posted by: Aborn Posted at: 2016-10-23T16:47:51.441Z Reads: 299

```
I can use any switch with this right?
```

---
## \#36 Posted by: DeathCookies Posted at: 2016-10-23T16:48:58.692Z Reads: 296

```
Unfortuneatly not.
It has to be a On/Off/On switch. You will get in this kit 3 of these working switches ;)
```

---
## \#37 Posted by: Aborn Posted at: 2016-10-23T16:50:33.407Z Reads: 287

```
Alright, i will come back to you when my build is ready for ordering ;)
```

---
## \#38 Posted by: Joakim1 Posted at: 2016-10-25T14:07:10.134Z Reads: 283

```
Too late? Could be interested.. :smile:
```

---
## \#39 Posted by: DeathCookies Posted at: 2016-10-25T14:29:58.970Z Reads: 300

```
Actually you are not too late. Nearly. I just have some but some "interessted" people too ;)
Everybody who wants one should hurry up :D
pm'ed you
```

---
## \#40 Posted by: Mox Posted at: 2016-10-27T12:53:20.699Z Reads: 313

```
received .
Danke :slight_smile:
```

---
## \#41 Posted by: rasmukri Posted at: 2016-11-01T23:31:39.459Z Reads: 316

```
Got mine the other day, just got around to soldering it together tonight. Didn't have any XT60's lying around but it's basically done. Quick shopping and easy communication the whole time.<img src="/uploads/db1493/original/3X/9/7/97b11bfebdc269c2d48eb1ef3ac3f0397ec133c5.jpg" width="690" height="463">
```

---
## \#42 Posted by: Cramps Posted at: 2016-11-01T23:32:18.058Z Reads: 309

```
Hi, is there any chance that there is still one available? I'm new to this forum but have done a solid week or so of research and think this is well worth having.

Edit: I would pm you but I don't actually know how to...yet :grin:
```

---
## \#43 Posted by: DeathCookies Posted at: 2016-11-02T07:34:01.794Z Reads: 297

```
PM'ed you :wink:
```

---
## \#44 Posted by: Maxid Posted at: 2016-11-02T07:55:04.976Z Reads: 294

```
maybe a bit overkill for the three switch wires :confused:
```

---
## \#45 Posted by: TarzanHBK Posted at: 2016-11-02T07:57:17.009Z Reads: 294

```
better be safe than sorry :smiley:
```

---
## \#46 Posted by: TarzanHBK Posted at: 2016-11-02T07:59:48.980Z Reads: 301

```
it should be possible to use a switch like:

<img src="/uploads/db1493/original/3X/9/e/9e793bafbda67a84c9635de730f3ac9ca69514de.jpg" width="500" height="500">

it needs 12V supply for the led and 3 phase on and off contacs. Is it plug and play with this kit, or is there some modification needed to get this going?
```

---
## \#47 Posted by: DeathCookies Posted at: 2016-11-02T08:05:41.220Z Reads: 288

```
Yes you will another 12V supply for the LED otherwise it is **not** **shining as bright as it should be.**

I have a similiar switch and tested the switch itself. I could not power on/off my board with this kind of a switch. We need an **On/Off/On**-switch (**S**ingle **P**ole **D**ouble **T**hrow = Wechselschalter)
```

---
## \#48 Posted by: Bender Posted at: 2016-11-02T11:53:25.185Z Reads: 281

```
I got a STDP switch with a 5v led that works but I have to get the 5v from the vesc
```

---
## \#49 Posted by: rasmukri Posted at: 2016-11-02T12:18:54.303Z Reads: 282

```
Only wire I had was that or some 8 gauge so yeah I wasn't gonna buy new stuff for no reason :p
```

---
## \#50 Posted by: DeathCookies Posted at: 2016-11-02T13:12:52.337Z Reads: 283

```
Do you have a link?
```

---
## \#51 Posted by: Bender Posted at: 2016-11-03T13:45:05.227Z Reads: 287

```
Here ya go 

https://www.amazon.com/dp/B015X3E6DK/ref=biss_dp_sa1
```

---
## \#52 Posted by: DeathCookies Posted at: 2016-11-03T13:46:19.775Z Reads: 279

```
Interessting, i thought it needs to be a On/Off/On SPDT switch.... 
Such a switch like you have it is laying around at home. I need to test it more. 

Thanks for the link!
```

---
## \#53 Posted by: rasmukri Posted at: 2016-11-04T19:50:51.325Z Reads: 288

```
With the switch that came in the kit I'm all kinds of confused. It came with 3 on/on switches. i thought it needed an on/off/on one? And what is the switch supposed to do? i mean the on/on turns it off and on, but a on/off/on seems to do nothing? Also there are 3 wires for the switch, why? is one like low power for using for an LED or something? and what 2 wires make it on for normal usage? I'm so confused and I'm pretty sure its something simple and I'm just being retarded about it.
```

---
## \#54 Posted by: mccloed Posted at: 2016-11-04T20:24:45.509Z Reads: 289

```
Does this help?
<img src="/uploads/db1493/original/3X/4/0/40da12f966fea3f7f2eb55b0d7d85f2f2713605b.png" width="555" height="179">
```

---
## \#55 Posted by: rasmukri Posted at: 2016-11-04T20:33:45.419Z Reads: 293

```
that helps a bit, but why is there a connection when its "up" in your example? Why is it not just on and off? In your example when its "down" is this on or off?
```

---
## \#56 Posted by: jak Posted at: 2016-11-04T21:29:00.547Z Reads: 303

```
Finally got some free time to test my soldering job.
@DeathCookies thanks a bunch daniel i got the switch figured out no led though. Superb customer service and timing for shipping to the states. Check off another peice to the puzzle. Enjoy the pics.
<img src="/uploads/db1493/original/3X/2/3/23242564f8b73b8bf5d338235708031c231b7faf.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/4/c/4c3ed7cdb8fd697b6f6ba3ce112446b8820fb0b7.jpg" width="281" height="500">
```

---
## \#57 Posted by: DeathCookies Posted at: 2016-11-06T16:06:35.826Z Reads: 293

```
Updated the first Post with useful information
```

---
## \#58 Posted by: mccloed Posted at: 2016-11-08T23:08:00.855Z Reads: 291

```
Awesome! Thanks for the update!
```

---
## \#59 Posted by: CaptainMerricka Posted at: 2016-11-26T02:21:54.719Z Reads: 294

```
Any more of these switches?
```

---
## \#60 Posted by: Glenn Posted at: 2016-11-26T03:24:10.403Z Reads: 287

```
I am wondering the same thing, if they will be offering these kits again?
```

---
## \#61 Posted by: DeathCookies Posted at: 2016-11-28T07:47:18.366Z Reads: 291

```
Currently there are two left. One message with pay information is out.

Who is gonna pay it first will get one ore two ;)

I had planned to make anohter grou buy but this time with the
http://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738

Anybody interessted?
```

---
## \#62 Posted by: TarzanHBK Posted at: 2016-11-28T09:29:59.467Z Reads: 283

```
LED switch! LED switch! LED switch!

What Amp limit is this switch rated? Need something for my 80A dual builds :monkey:
Also - price?
```

---
## \#63 Posted by: DeathCookies Posted at: 2016-11-28T09:37:37.594Z Reads: 252

```
I want to build a dual FET switch which is up to 100A.

More or less the same price as this set. I think it will be a bit more expensive but include everything!
```

---
## \#64 Posted by: JdogAwesome Posted at: 2016-11-28T13:08:19.781Z Reads: 260

```
Hey guys thanks for your interest in my switch! I have two variants for my design, a single FET 40A design and a dual FET 80A design. Though both these switch's can handle burst currents of a lot higher and temporarily drawing more current going up a steep hill for example. I personally use my single FET design and I see 0 heat rise on it going very fast. Also my prices are $25 for single FET, that includes it pre soldered with XT60 connectors as well, and $35 for dual FET. Though if you plan on doing a group buy I could definetly make that a lot cheaper per unit. Also if you guys were interested in just a kit, including all the components and PCB I could do it for even cheaper.
```

---
## \#65 Posted by: DeathCookies Posted at: 2016-11-28T13:17:39.840Z Reads: 236

```
pm written!
```

---
## \#66 Posted by: hexakopter Posted at: 2016-11-28T17:09:21.772Z Reads: 229

```
@DeathCookies Why do you want to go a step back and using a perfboard instead of a "normal PCB"? For me that looks strange.
```

---
## \#67 Posted by: DeathCookies Posted at: 2016-11-28T17:41:37.996Z Reads: 243

```
Who has told you that i am going to use a perfboard?? 
I just told you that i will make a group buy for this specific switch (because  i do not think there is a better one?  = Performance/size/features) 

I will order some pcbs and make a Kit like this thread here ;)
If anybody is interessted just tell me that i can plan how much i am going to buy
```

---
## \#68 Posted by: hexakopter Posted at: 2016-11-28T18:03:39.553Z Reads: 247

```
[quote="DeathCookies, post:67, topic:9949"]
because  i do not think there is a better one?  = Performance/size/features
[/quote]
Maybe you should look at your first post in this thread to see a better one... :slight_smile: I think that his design isn't a 2 layer PCB is bad from the thermal perspective, because you haven't vias to the other side where you can cool the FETs if you want to. I don't see the size of his design over in the other thread, but I don't think that it is much smaller. But do whatever you like.
```

---
## \#69 Posted by: DeathCookies Posted at: 2016-11-28T18:19:20.977Z Reads: 237

```
It seems as his switch is a tiny bit smaller but now much. But it is smaller than the eboard mosfet switch which get very wide...

Maybe you can recommend me a better switch where i can **directly** attach a switch LED. Somehow I do not like the idea to get the power for the led switch from the VESC: What is when you have a OPTO ESC?
```

---
## \#70 Posted by: hexakopter Posted at: 2016-11-28T18:29:34.791Z Reads: 221

```
I don't see any problem using the power from the VESC.
```

---
## \#71 Posted by: DeathCookies Posted at: 2016-11-28T18:41:21.919Z Reads: 228

```
What if you dont have a vesc, a normal Esc without bec. Then you need go get another Power supply. 
This is the Part i dislike:
Why should i use a Power supply from another component?
```

---
## \#72 Posted by: TarzanHBK Posted at: 2016-11-28T20:14:42.156Z Reads: 235

```
thats the main reason i don´t like using the vedder switch. Imagine a vanguard build with 2 enclosures. You don´t want to go back with the cables from the vesc enclosure to your battery, just for using a nice switch.
```

---
## \#73 Posted by: DeathCookies Posted at: 2016-11-28T23:12:18.565Z Reads: 234

```
And an additional BEC is not needed because you can easily integrate the LED into The switch.
```

---
## \#74 Posted by: Sander Posted at: 2016-12-12T22:09:47.679Z Reads: 234

```
Hey I have got skills in PCB making. So all I need is the part list with which resistance R1, R2 etc...
And do I need to load any drivers or is it just solder on/smd.

I ask this because Im gonna intergrate this inside the circuit for my board reciever with lights, bluetooth, 2.4ghz remote etc...
```

---
## \#75 Posted by: lox897 Posted at: 2016-12-12T22:25:41.819Z Reads: 235

```
The BOM is on Vedder's github

And no it doesn't need drivers
```

---
## \#78 Posted by: DeathCookies Posted at: 2016-12-15T06:55:56.842Z Reads: 246

```
https://github.com/vedderb/SparkSwitch/blob/master/SparkSwitch_BOM.ods
```

---
## \#79 Posted by: Sander Posted at: 2016-12-23T20:52:00.125Z Reads: 253

```
I created some different version of the Vedder Switch.
And their intended for my Eboard.<img src="/uploads/db1493/original/3X/3/6/36785a30ea96f37faac85c12c960e8387dd2c2ff.png" width="690" height="388">

Front:
<img src="/uploads/db1493/original/3X/f/8/f87be9977f987d38134dcc2e5845d79dbc2df98b.png" width="500" height="242">

Back:
<img src="/uploads/db1493/original/3X/3/8/3853d8bd23106e2e9a939742ce71dfa36c853ef9.png" width="500" height="242">
```

---
## \#80 Posted by: Maxid Posted at: 2016-12-23T21:16:26.190Z Reads: 237

```
Half the size seems like no special feat when you also use just half the Mosfets...
```

---
## \#81 Posted by: Sander Posted at: 2016-12-23T21:39:24.589Z Reads: 249

```
Didn't say it was special or something.
<img src="/uploads/db1493/original/3X/2/2/2215ae8eb5304d7d0b96a98655238fa86c79e658.png" width="500" height="483">
I need the most compacted things...
```

---
## \#82 Posted by: mortorojo Posted at: 2016-12-23T23:36:05.946Z Reads: 243

```
Half the MOSFETS? He still using two mosfets, just both sides of the board.
```

---
## \#83 Posted by: chaka Posted at: 2016-12-24T00:10:08.587Z Reads: 250

```
That first one is the mod I made with vias. Before adding them the switch would get hot enough to make the solder flow and the mosfets would move during burst currents. I tried a double side switch like you have done but had the same problem during high discharge for prolonged periods. You may not have this issue if you dont pull a lot of amps but keep it in mind. Might want to shift the FETs so the are not right on top of each other if you plan on  having a lot of throughput.

Keep up the good work!
```

---
## \#84 Posted by: Sander Posted at: 2016-12-24T11:53:59.266Z Reads: 245

```
[quote="chaka, post:83, topic:9949, full:true"]
That first one is the mod I made with vias. Before adding them the switch would get hot enough to make the solder flow and the mosfets would move during burst currents. I tried a double side switch like you have done but had the same problem during high discharge for prolonged periods. You may not have this issue if you dont pull a lot of amps but keep it in mind. Might want to shift the FETs so the are not right on top of each other if you plan on  having a lot of throughput.

Keep up the good work!
[/quote]

Thanks. That was I thought! It would get a lot hotter.
But this was just an idea though, lol. ;)

And Merry Christmas!
```

---
## \#85 Posted by: TheImmortalJew Posted at: 2016-12-24T19:26:05.443Z Reads: 229

```
I'm working on making one of these right now and it's not going well. Could anyone share tips or expectations when it comes to hot air work like this? My problem is that the solder paste doesn't seem to hold nearly as good as a regular solder joint. I like to test how well the connection is by applying some force to see if the joint will hold. I soldered R1, R2, and C1 with a regular iron and solder and they are SOLID. But when I try to apply less than half that force to a hot air solder paste joint, it comes right off and smears the paste.

I've tried hot air temps from 180C (which the paste melts at) up to 250C with the same result. I'm fluxing everything with a pen too. Am I just expecting too much regarding how well paste holds vs regular solder? The paste also runs more than I expected, bridging the pins and spilling over the board. I tried using less and less but it still doesn't get sucked into the pads like I pictured.
```

---
## \#86 Posted by: DeathCookies Posted at: 2016-12-24T19:36:15.391Z Reads: 214

```
You should store them in the frigerator otherwise it will be damaged. Maybe your solder paste is too old?
```

---
## \#87 Posted by: TheImmortalJew Posted at: 2016-12-24T19:40:15.263Z Reads: 211

```
I just bought it a week ago lol. Expires in 2018.
```

---
## \#88 Posted by: PXSS Posted at: 2016-12-25T02:30:42.135Z Reads: 206

```
My pasted parts dont move ever... Are you using good quality paste? Good amount? Hot enough?
```

---
## \#89 Posted by: sl33py Posted at: 2016-12-25T07:49:19.911Z Reads: 212

```
[quote="PXSS, post:88, topic:9949"]
Hot enough?
[/quote]


That would be my first question - are you fully flowing the solder?  It should be just as strong as regular solder.
```

---
## \#90 Posted by: Bender Posted at: 2016-12-25T13:05:20.959Z Reads: 208

```
If it's still a matte grey and not a shiny silver then you didn't get it hot enough
I had the same problem on my first hot air attempt
```

---
## \#91 Posted by: TheImmortalJew Posted at: 2016-12-25T16:23:14.572Z Reads: 218

```
Success! Yep, temperature was the problem. I bumped it up to 325C and 4/8 on the air speed and it worked great! Sucked right into the pads. Live and learn.
```

---
## \#92 Posted by: DeathCookies Posted at: 2017-01-02T16:36:42.697Z Reads: 208

```
Now i could need some help @chaka @sl33py 
I have some broken switches... one stays permanently on and on does not power at all. 
I want to repair the broken switches but i do not know how to start...

How can i determine which part of the switch has failed with a voltmeter?
```

---
## \#93 Posted by: goldenHusky Posted at: 2017-01-02T16:49:52.499Z Reads: 220

```
[quote="DeathCookies, post:92, topic:9949"]
and on does not power at all
[/quote]

In this case you can measure the voltage between Gate and Source, if it is around 12V and still does not switch then your FETs are broken. If you switch on but your Vgs is still 0 your zener diode is broken.

[quote="DeathCookies, post:92, topic:9949"]
one stays permanently on
[/quote]

Also measure Vgs, if you switch off and Vgs is 0 but the switch is still on then your FETs are dead.
```

---
## \#94 Posted by: 3sly Posted at: 2017-01-20T11:51:24.451Z Reads: 222

```
Hey chaka,

As I saw it, you had made the final version of the vedder antispark (1.4) with the Via's. I made some of those through oshpark! Thank you first of all!

But I'd like to venture into personalising the design and add some features. I can't find your altium/kicad files (which i completely understand if you keep those private as you also sell them), but I can find vedder's. Allthough I'd like to add your improvements (the vias) to vedders design first, so that I get to start from the same working product.

So my question is: do the files in vedder's github (https://github.com/vedderb/SparkSwitch) contain the improvements you've made? I don't have access to open the programs right now but I'd like to start planning :stuck_out_tongue:

Kind regards,
Dries
```

---
## \#95 Posted by: chaka Posted at: 2017-01-20T15:20:37.973Z Reads: 222

```
I will upload the kicad .kicad_pcb board file to my google drive and share it here for you!

Edit: https://drive.google.com/open?id=0BzFdFRTGQpwZQzczRnljOWs0TG8

Let me know if it give you any trouble.
```

---
## \#97 Posted by: realtek Posted at: 2017-02-01T21:18:39.545Z Reads: 205

```
hello,i have a problem with my switch.
When i connect a 6s battery to the switch on the exit is still 5V it should be 0V right?
Can anyone help me with that problem please ?
```

---
## \#98 Posted by: TranxFu Posted at: 2017-02-14T20:07:13.044Z Reads: 207

```
Hey :) I have this one soldered up and tried the switch. I have it connected to a 12v supply. It shows me 10v(I guess the power supply is old and kind of defect). And when I toggle the switch it goes down to 9v. Same on my other supply which runs 6v and when toggled it goes down to 5v. 

Could there be a soldering failure somewhere ?
```

---
## \#99 Posted by: DeathCookies Posted at: 2017-02-14T21:12:53.172Z Reads: 212

```
Could you provide some pictures?
```

---
## \#100 Posted by: Mohammed Posted at: 2017-04-15T00:30:50.733Z Reads: 195

```
Hi, are you still offering these items? i would be interested if you still do. i live in NZ
```

---
## \#101 Posted by: solidgeek Posted at: 2017-04-19T21:44:57.397Z Reads: 182

```
Hi I am also interested in buying on of these anti spark switches! Will it be back in stock? I live in Denmark :slight_smile:
```

---
## \#102 Posted by: saybot Posted at: 2017-06-25T17:16:38.374Z Reads: 166

```
Hi is possible to order anti spark switch?
```

---
## \#103 Posted by: Silverline Posted at: 2017-06-25T17:38:04.085Z Reads: 167

```
Hallo im also interested in buying one anti spark switch with pre soldered mosfets. If stil possible 😃?
```

---
## \#104 Posted by: DeathCookies Posted at: 2017-06-26T15:22:45.210Z Reads: 167

```
No, but there are different threads where they are still offering some
```

---
## \#105 Posted by: Redfire1 Posted at: 2018-04-17T04:44:15.387Z Reads: 88

```
@DeathCookies Hi morning I living in Germany 33330 I bought a anti spark switch from Italy and I think one mosfet is damage,can I have one of this setup kit with the mosfet solder can you send me a PayPal and the amount please.
```

---
## \#106 Posted by: b264 Posted at: 2018-04-17T05:50:21.958Z Reads: 82

```
Get a replacement from [digikey](https://www.digikey.com/) or [mouser](https://www.mouser.com/).  The part number should be in [the BOM](https://github.com/vedderb/SparkSwitch/blob/master/SparkSwitch_BOM.ods).
```

---
## \#107 Posted by: Redfire1 Posted at: 2018-04-17T07:08:52.342Z Reads: 87

```
I found this,can I buy the complete parts to make my own anti spark switch on mouser ![image|230x500](upload://tfdbebyGxcGlTlMZyxwnoupsxHT.jpg)
```

---
## \#108 Posted by: b264 Posted at: 2018-04-17T07:22:19.087Z Reads: 82

```
They will have everything except the PCB
```

---
## \#109 Posted by: Redfire1 Posted at: 2018-04-18T05:17:24.300Z Reads: 86

```
@goldenHusky can I call you please
```

---
## \#110 Posted by: LiquidSkater Posted at: 2019-04-30T18:55:24.194Z Reads: 24

```
Hi, I bought an anti spark switch on ebay, I ordered the non - latching button and put another button on the NC wire and it worked perfectly fine. So I set up the board and went for a ride and 800 meters in power started to cit out, then it came back and I continued to ride, but on my way home (2nd km) power completely cut off and something started to smell. When I rushed home and opened the  enclosure I saw that the mosfets had melted a hole in shrink wrap...
I don't know what should I do now. If I had done something wrong or if I should cool it somehow...![15566504592414279644416883785934|374x500](upload://x6wPjx44n3iAxT1ByffDgT305nu.jpeg) ![15566504847895978260481251717062|375x500](upload://pMbvUX0r742SH0qRQDrnY42ELCJ.jpeg) 
I had the wires soldered correctly but it just melted...

The button i got (model 6)
https://www.ebay.com/itm/Anti-Spark-Power-On-Off-Switch-for-VESC-or-ESC-electric-skateboard-longboard-LED/163610874953?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D56949%26meid%3D607a686075f5439c9d2f2223b46b5922%26pid%3D100675%26rk%3D1%26rkt%3D15%26sd%3D163610874953%26itm%3D163610874953&_trksid=p2481888.c100675.m4236&_trkparms=pageci%3Ac2cc312f-6b78-11e9-9fab-74dbd180dd14%7Cparentrq%3A6f950d4f16a0aadc417ffeaaffeea806%7Ciid%3A1
```

---
