# Flat cables over deck (boosted board)

### Replies: 56 Views: 8213

## \#1 Posted by: AugustM Posted at: 2016-06-17T17:07:44.499Z Reads: 644

```
Hi everyone,

Does anyone know what these cables are and where to buy them?
I'd like to run my cables over the deck of my board connecting the batteries to the Vesc :) .
But i'm looking for flat cables that can handle the voltage and amperage.

Thanks!

<img src="/uploads/db1493/original/2X/f/f566f44178e2bbfeb8c680f7e2f24ecf5c972419.png" width="552" height="500">
<img src="/uploads/db1493/original/2X/b/bd485ef6d043385e6b462767e763b42db4200b04.png" width="499" height="500">
<img src="/uploads/db1493/original/2X/a/a991d9c6f44f0067f544c4a5c09ac72f21482d7f.png" width="319" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2016-06-17T17:10:37.730Z Reads: 632

```
You can use copper braid, just be careful not to short anything..

https://www.amazon.com/Small-Parts-Flat-Copper-Braid/dp/B003R501JK
```

---
## \#3 Posted by: AugustM Posted at: 2016-06-17T17:13:17.057Z Reads: 630

```
Oh so there is no insulation around the cable at all?
Won't it cause fire to the wooden deck?
And what is the orange foil they are using then? 

Thanks for the information!
It's my first build so i don't know that much :slight_smile:
```

---
## \#4 Posted by: treenutter Posted at: 2016-06-17T17:13:50.099Z Reads: 623

```
@AugustM keep in mind that there is a 20-30cm maximum length you can use with VESC if you run in FOC mode. If you BLDC the battery cable length matters less.
```

---
## \#5 Posted by: Jinra Posted at: 2016-06-17T17:16:54.227Z Reads: 615

```
I don't think the cables would get hot enough to start a fire on your deck, but you could sandwich it with some electrical tape for peace of mind.
```

---
## \#6 Posted by: barajabali Posted at: 2016-06-17T17:24:00.661Z Reads: 598

```
I know about braiding and all.... But what do you all think about using like 2 doubles up layers of 10mm wide nickel strip? 

Even one layer can handle like 20 amps or more.
```

---
## \#7 Posted by: Jinra Posted at: 2016-06-17T17:26:29.266Z Reads: 577

```
I'd just be worried about the repetitive motions of the board flexing and turning, it may wear the strip down. Also, I have NO idea about this, but wouldn't nickel strip have higher internal resistance than copper?
```

---
## \#8 Posted by: barajabali Posted at: 2016-06-17T17:27:58.194Z Reads: 566

```
Yea it's like 4 times more resistive than copper or something
```

---
## \#9 Posted by: RunPlayBack Posted at: 2016-06-17T17:42:11.478Z Reads: 564

```
How about keeping the battery and VESC next to each other to avoid short/power issues and running the motor phase wires across the top?
```

---
## \#10 Posted by: Kaly Posted at: 2016-06-17T17:44:48.697Z Reads: 563

```
I use flat wires on all my builds with no problem thus wires have less resistance than round wires,  they come with no insulation but heat shrink will solve that. 

Heat shrink 
http://www.mcmaster.com/#7856k15/=12w8c89

12AWG equivalent flat wire 
http://www.mcmaster.com/#69925k66/=12w8di4


Tip:

When soldering to a round wire just open the braid a little bit and stick 1/4 inch of the tinned round wire into the braid, use a strand of thing wire to loop 1-2 turns around the braided wire and solder.

I have use this wire with 12S lipos and 40V lifepo4 packs as well.
```

---
## \#11 Posted by: AugustM Posted at: 2016-06-17T18:57:28.900Z Reads: 539

```
My board has a lot of flex so, i'm afraid it will damage the batteries when they are placed in the middle.
That's why I was thinking of having my vesc+motor at one end, and the batteries at the other :slight_smile:

Thank you @Kaly and @Jinra , This was exactly what i needed to know!!
```

---
## \#12 Posted by: Kaly Posted at: 2016-06-17T19:09:11.149Z Reads: 537

```
<img src="/uploads/db1493/original/2X/7/7fa8ac9d52897b803ed974518e91db2911abc9e5.jpeg" width="375" height="499">
```

---
## \#13 Posted by: Lizardking0069 Posted at: 2016-06-17T19:33:45.072Z Reads: 519

```
@AugustM that orange foil is actually Kapton tape. Its a great electrical insulator.
```

---
## \#14 Posted by: Randyc1 Posted at: 2016-06-17T20:03:06.756Z Reads: 506

```
Hey Kaly,..Why is that braided wire Tin plated , do you know?
```

---
## \#15 Posted by: Jinra Posted at: 2016-06-17T20:39:42.033Z Reads: 503

```
to prevent oxidation
```

---
## \#16 Posted by: Kaly Posted at: 2016-06-17T20:43:34.069Z Reads: 502

```
Like @Jinra said because the oxidation. 
The fact that is pretinned makes it perfect for eboards.
```

---
## \#17 Posted by: Ulfberht Posted at: 2016-06-17T21:22:27.220Z Reads: 498

```
So let me get this straight....If I drop a screwdriver from the right angle, I can short out the wires on a boosted. That could be wicked dangerous!! What about if you crash a boosted? Is it possible that the "solder wick" wires could become exposed? I really despise that design. IMO
```

---
## \#18 Posted by: Jinra Posted at: 2016-06-17T21:27:49.566Z Reads: 490

```
it would probably be fine, the cables are taped under the grip tape. If you had a catastrophic failure where the cables are ripped from the board and short, I think you'd have bigger problems to worry about.
```

---
## \#19 Posted by: Arzamenable Posted at: 2016-06-17T21:44:31.123Z Reads: 504

```
That yellow tape is kapton tape. 
Foxnovo High Temperature Heat Resistant Kapton Tape Polyimide Film Adhesive Tape (20mm*33m) https://www.amazon.com/dp/B00N1RHE2Q/ref=cm_sw_r_cp_api_g7gzxb38RW287
```

---
## \#20 Posted by: Kaly Posted at: 2016-06-17T22:27:30.207Z Reads: 511

```
I am down with you on the poor design choice at least use shrink wrap.

On my vanguard i use heat shrink on top of that made 2 shallow channels in the deck for the wires and use epoxy to seal the cables. This high discharger and power battery packs are no joke, once shorted a 40V 20Ah pack and the current vaporized 1/4 in of the metal that touched, no melting just disappeared in smoke and i almost pee on my self.
```

---
## \#21 Posted by: barajabali Posted at: 2016-06-17T22:32:56.185Z Reads: 473

```
Hahahah I can't help but laugh at that.... Ever short a fully charged 12s? Mother fucking 50 volts 10amp hour it hurt my soul. Sounding like an arc welder
```

---
## \#22 Posted by: Hummie Posted at: 2016-06-17T23:20:17.230Z Reads: 481

```
Copper sheet painted in a thin polyurethane from smooth-on.com.  Super thin and super conductive

You could make  strips very thick and cut down on the wire inductance and maybe get away with the Long connections using foc

My avatar is all over the top of the page!! Winner for ten minutes
```

---
## \#23 Posted by: Kaly Posted at: 2016-06-18T00:42:57.637Z Reads: 478

```
Quickest way to learn :scream: 
After something like this extra careful all the time
```

---
## \#24 Posted by: kenf4345 Posted at: 2016-06-18T03:12:56.483Z Reads: 482

```
<img src="/uploads/db1493/original/2X/4/4418cd98104a014c900a8a7585c3f46555fc4ccd.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/0/0b006ce01cb0ede10bb6f4fb0f1e48d96e668f4f.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/a/a3719a214d45fd8cbd57507d0f587b5bd5973e97.jpg" width="375" height="500">

I had a company cut 2 half inch strips that were something like .51 mm thick. The area of the cross section of the copper strips was slightly bigger than 10 AWG wire.
```

---
## \#25 Posted by: Jinra Posted at: 2016-06-18T03:16:12.040Z Reads: 463

```
are those burn marks from the strip heating up?
```

---
## \#26 Posted by: kenf4345 Posted at: 2016-06-18T03:20:51.969Z Reads: 466

```
No  they are from soldering. I had to use a heat gun to get the temp hot enough to melt the solder. The copper strips dissipate the heat quickly, so a soldering iron is very difficult. I have ran it about 20 miles its there no heating issues at all. <img src="/uploads/db1493/original/2X/f/fb66b471ade05ad23c2a2ec34f655ebe87720ef4.JPG" width="375" height="500">  I siliconed the copper strips to the board. They flex nicely.
```

---
## \#27 Posted by: andymation Posted at: 2016-06-18T04:13:51.491Z Reads: 453

```
Love that setup!! Very similar to what I want to do. Do you have any pictures or info on your battery and battery enclosure build?
```

---
## \#28 Posted by: Lizardking0069 Posted at: 2016-06-18T13:45:45.122Z Reads: 441

```
What about flat speaker wire: https://www.amazon.com/gp/aw/d/B005SUM1PO/ref=mp_s_a_1_2?qid=1466257504&sr=8-2&pi=SX200_QL40&keywords=flat+speaker+wire&dpPl=1&dpID=41eS8rmTvnL&ref=plSrch
```

---
## \#29 Posted by: kenf4345 Posted at: 2016-06-19T13:42:15.934Z Reads: 435

```
Battery enclosures i designed and 3d printed. For the batteries i just used 2 zippy flight max 5000 mah batteries.
```

---
## \#30 Posted by: kenf4345 Posted at: 2016-06-20T15:02:30.000Z Reads: 422

```
Thats 16 AWG wire.  A little small for what we need.
```

---
## \#31 Posted by: Lizardking0069 Posted at: 2016-06-20T15:28:29.506Z Reads: 420

```
You could double up on the wire.
```

---
## \#32 Posted by: brun Posted at: 2016-08-07T16:44:31.872Z Reads: 394

```
Looking at that screen shot, the boosted board seems to have thin sheet of white plastic between the kapton tape and the grip tape to protect the braided wires (from things like dropped screw drivers).  That would probably protect them better than shrink wrap or even the wire's silicon casing.
```

---
## \#33 Posted by: brun Posted at: 2016-08-07T16:46:00.187Z Reads: 399

```
...and probably need something stiff there anyway to smooth out the 4 bumps or high spots in the deck that would otherwise be created by the 4 wires.
```

---
## \#34 Posted by: SimonVoss Posted at: 2016-10-17T16:03:24.565Z Reads: 362

```
http://www.electric-skateboard.builders/uploads/db1493/original/2X/0/0b006ce01cb0ede10bb6f4fb0f1e48d96e668f4f.jpg
can you pls tell me how thick the shell/case (and are they solid) that you have for the battries and for the VESC's. i wan't to 3D print my cases to but i don't know if they can take the load.
```

---
## \#35 Posted by: kenf4345 Posted at: 2016-10-21T01:32:21.544Z Reads: 341

```
they are .5 mm thick which i think is the perfect thickness. They are partially filled on the inside to reduced weight and filament usage.  Im new with the 3d printing. I went to 3dhubs.com and looked around for someone to print them. So far I have about 200 miles on my board with absolutely no problems. DM me if you have more questions.
```

---
## \#36 Posted by: SimonVoss Posted at: 2016-10-23T16:21:51.157Z Reads: 331

```
Are the case alco 5mm under the deck or is the components just placer rigt under the deck?
```

---
## \#37 Posted by: SimonVoss Posted at: 2016-11-10T18:58:00.928Z Reads: 321

```
What sort of material have you used to the cases ?
```

---
## \#38 Posted by: im-done Posted at: 2016-11-10T19:22:19.857Z Reads: 314

```
The orange foil looking stuff is called capton tape. Its like electical tape but not stretchey and will not melt.  It will burn just wont melt, makin it great for batterys that get warm.
```

---
## \#39 Posted by: SimonVoss Posted at: 2016-11-12T19:06:46.562Z Reads: 313

```
Are there a specific reason why you have not used cobber?
```

---
## \#40 Posted by: kenf4345 Posted at: 2016-11-13T03:24:22.107Z Reads: 304

```
I don't really know what cobber is
```

---
## \#41 Posted by: kenf4345 Posted at: 2016-11-13T03:25:58.632Z Reads: 290

```
I did it with abs
```

---
## \#42 Posted by: darkkevind Posted at: 2016-11-23T11:50:27.330Z Reads: 283

```
Haha! He means copper! lol
```

---
## \#43 Posted by: rtasca Posted at: 2016-11-24T02:05:13.767Z Reads: 282

```
I used for my build PCB material.  Cheap and easy to find. You can get very thin fiberglass backing so it will be very flexible ( it will even reinforce your deck ). You just have to route a channel in the middle or cut 2 separate strips. You can also make it as wide as you wish. Just havent got mileage on it but thin copper will take a lot of flexing ( hopefully ).
```

---
## \#44 Posted by: darkkevind Posted at: 2016-11-24T20:03:23.278Z Reads: 278

```
All you need is to sandwich either one or two pairs of this between your ply (if you're making your own board), or through one end over the top and then through to the bottom the other end (if you're covering the top in tape).
 http://www.ebay.co.uk/itm/121941430464
```

---
## \#45 Posted by: sash Posted at: 2017-07-18T20:42:40.592Z Reads: 236

```
Just found this old thread.

I am considering various ways to run cables from the battery to VESC's on Vanguard board (with dual Boosted-style enclosures).   I am not a big fan of drilling lots of holes and grooves in the deck.

Why do people usually run flat cables on the top of the deck?   Is it only because you can hide them under the grip tape?  Is it a good idea to run flat cables on the bottom of the deck?
```

---
## \#46 Posted by: darkkevind Posted at: 2017-07-19T06:59:38.765Z Reads: 215

```
You can run them under the deck, but you'll need to find a way to conceal them. . . Unless you're not bothered about seeing them. Did probably protect them in some way too...
```

---
## \#47 Posted by: KranzeKake Posted at: 2018-10-07T01:09:51.098Z Reads: 126

```
Can I use this one? Can it handle the current? https://www.amazon.com/Tinned-Copper-Braid-Bright-Length/dp/B003HGHQYM/ref=cm_cr_arp_d_product_top?ie=UTF8
```

---
## \#48 Posted by: Alex753 Posted at: 2018-12-21T15:25:56.020Z Reads: 101

```
Hey ! 

Little up of this thread because I need one actually for an 8S 50Amps setup, the amazon link look good but idk which diameter should I take ?
```

---
## \#49 Posted by: Alex753 Posted at: 2018-12-22T01:04:09.414Z Reads: 94

```
Anyone ?

Or another link I don’t care, it’s strange how it look like everyone use this method and there is no information all around the forum !
```

---
## \#50 Posted by: KranzeKake Posted at: 2018-12-22T01:45:46.607Z Reads: 89

```
I know, Use half inch, tin plated copper braided cable
```

---
## \#51 Posted by: Meeep Posted at: 2018-12-22T06:08:14.213Z Reads: 78

```
Going in this coming Christmas build :) https://www.amazon.com/gp/product/B01BIBQ940/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#52 Posted by: deltazeta Posted at: 2018-12-22T06:25:30.151Z Reads: 83

```
https://www.electric-skateboard.builders/t/phoenix-loaded-vanguard-hummie-hubs-v4-restored-dual-focbox-12s4p-30q-eboosted-enclosure/73511

It's been mentioned before 1/4 inch is 12 awg equivalent. I doubled up for headroom. A large restriction on power contraints is heat, so make sure you insulate with something.
```

---
## \#53 Posted by: Alex753 Posted at: 2018-12-22T08:21:21.199Z Reads: 79

```
That’s cool thanks !

Does it can touch the wood of the deck without shorting anything ? 
Like the top can be isolated with some tape but what about the part that is touching directly the deck ?
```

---
## \#55 Posted by: KranzeKake Posted at: 2018-12-22T12:07:45.998Z Reads: 73

```
Here is what I did: https://www.youtube.com/watch?v=EbNoS0Tr8c8
```

---
## \#56 Posted by: Alex753 Posted at: 2018-12-22T18:03:46.737Z Reads: 65

```
Nice thank you dude !
```

---
## \#57 Posted by: Hummie Posted at: 2018-12-22T18:05:13.074Z Reads: 63

```
Copper sheet works.  The deck wood is a good insulator
```

---
