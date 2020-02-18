# Small Bestech BMSs!

### Replies: 58 Views: 4224

## \#1 Posted by: Jinra Posted at: 2017-06-21T03:46:10.264Z Reads: 455

```
I ordered some small BMS's (for balancing only) since my build is pretty cramped for room. They look great and are spec'd for exactly what I need. Good option for the space conscious builder. Specs are exactly the same for both BMS's so I only included one.

**HCX-D250**
<img src="/uploads/db1493/original/3X/7/7/7782501a750c3331062c3daeb9e02a538b26fff9.png" width="356" height="500">
<img src="/uploads/db1493/original/3X/1/a/1a45e99e0b5afb323b5f553a47a7d73515efd57c.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/e/b/ebd70ec4151c6473c27546db9622a98e833ec89c.jpg" width="666" height="500">

**HCX-D239**
<img src="/uploads/db1493/original/3X/f/e/fea1f107164c7ff91610d6d3fe0055cb6df9bf83.png" width="690" height="309">
<img src="/uploads/db1493/original/3X/2/c/2cc8b64338930d001ed213e99f1c5ab39c17f14e.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/6/a/6a472008e7010765112d06e9bc5623bc9086afdb.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/2/428d18718528406b99ff6d1f7f2696b43052cb8d.jpg" width="666" height="500">

**Prices**
<img src="/uploads/db1493/original/3X/6/5/656b5fd545106fc2854a950343d9f5125358e782.png" width="690" height="342">
```

---
## \#2 Posted by: sl33py Posted at: 2017-06-21T04:03:19.082Z Reads: 389

```
@Jinra - you are READING my mind!  I just got my 10s and 12s 80A BMS'ssss  They are pretty frickin' huge.  I'd love a super small 10s and 12s BMS just for charging when i build an 18650 pack!

Any suggestions on similar small 12s BMS?
```

---
## \#3 Posted by: Jinra Posted at: 2017-06-21T04:04:34.044Z Reads: 379

```
I just took a look here and looked for one with my size requirements. Here's the page for 12s

http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/
```

---
## \#4 Posted by: Jinra Posted at: 2017-06-21T04:06:35.950Z Reads: 372

```
Size-wise these look pretty manageable

http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D108.html
http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCB-D132.html

Whatever you choose make sure theres a value for "balance", some don't have balancing.
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-21T06:22:41.384Z Reads: 353

```
Hmm @Namasaki,

Have you had any issues with your BMSs from Bestech? I just tried both and neither go higher than 40.7v on my 10s setup.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-06-21T11:32:34.991Z Reads: 329

```
One time because I replaced 1 pack that got a broken wire and the new pack was too far out of balance from the rest. 
I manually balanced all five packs separately with my hobby charger and it's been fine ever since.
```

---
## \#7 Posted by: Rob69de Posted at: 2017-06-21T11:41:09.442Z Reads: 320

```
<img src="/uploads/db1493/original/3X/b/3/b3ec7093e71992f650172b55d16a17b16670bb2d.JPG" width="375" height="500">

Hope I don't offend 🤔
Enertion bms
```

---
## \#8 Posted by: LukePL Posted at: 2017-06-21T12:11:19.252Z Reads: 305

```
A beginers question...... So you use BMS only while charging and than drawing directly from battery while riding?
```

---
## \#9 Posted by: Migro Posted at: 2017-06-21T13:08:10.412Z Reads: 304

```
@LukePL thats correct for what i understand from bms's. 

@Jinra  do you know og these would Work with lipos aswell or do you know any small ones that does?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-06-21T13:42:20.233Z Reads: 298

```
There are 2 options. 
You can use a bms for charging only or for charging and discharging.   
The 2nd option is the best because it protects the battery while riding as well as charging.
```

---
## \#11 Posted by: Vieo Posted at: 2017-06-21T13:44:39.060Z Reads: 294

```
From what I gather, alternatively you can also draw power via the BMS _(requires a high Amp output)_ and this can help with safety; eg. monitoring each cell in a battery pack to ensure isn't over-discharged.

[BMS - Wikipedia](https://en.wikipedia.org/wiki/Battery_management_system)

I believe these BMS in discussion are for charge-only setups



_damn u @Namasaki beat me 2 it_
```

---
## \#12 Posted by: LukePL Posted at: 2017-06-21T14:06:28.833Z Reads: 290

```
Thanks guys! As I thought... BMS used for charging only, can be smaller and cheaper. If cells are balanced while charging and I plan to use VESC so I can limit a curent, it should be quite safe system, right? I have SONY VTC5 cells and I want to build 10s4p pack to power one 6374 170KV motor.
And I read on some ebike forum that you should wait after charging because BMS is still balancing the cells. Is that true?
thanks
Luke
```

---
## \#13 Posted by: Jinra Posted at: 2017-06-21T14:42:12.168Z Reads: 284

```
All my cells are 4.04-4.07v with a total charge of 40.6v on 10s. Both my 42.2v chargers won't charge anymore than that.

Weird thing is the problem exists on both BMSs
```

---
## \#14 Posted by: Vieo Posted at: 2017-06-21T14:48:13.161Z Reads: 271

```
After looking at the BMS data-sheet

**Over Charge Release Voltage:** 4.05V

Maybe this?
```

---
## \#15 Posted by: Jinra Posted at: 2017-06-21T15:03:15.319Z Reads: 268

```
While the number is about right, this is the release voltage and not the overcharge detection voltage (4.2 on sheet). They said they test every module before shipping so i don't know.
```

---
## \#16 Posted by: Vieo Posted at: 2017-06-21T15:08:59.857Z Reads: 266

```

http://batterypoweronline.com/images/PDFs_articles_whitepaper_appros/MPE_LiIonSafety.pdf

> **Overcharge Release**
> The safety circuit will allow charging to take place after the
> cell’s voltage drop below the overcharge release threshold. 

This is just a quick google I did. Maybe somone with better BMS/Battery knowledge can help though
```

---
## \#17 Posted by: Jinra Posted at: 2017-06-21T15:11:01.895Z Reads: 259

```
It does seem that may be causing problems, but i feel the release shouldn't trigger until it gets the overcharge limit
```

---
## \#18 Posted by: JLabs Posted at: 2017-06-21T15:15:28.017Z Reads: 261

```
I feel like they are really over charging... Quality is good tho (from what everyone says on the forum).
```

---
## \#19 Posted by: darkkevind Posted at: 2017-06-21T15:43:58.628Z Reads: 259

```
Guys, noob question here. If I have an 8s4p pack, do I need 4 BMS's?

If not, how does it work with just one BMS and 4 'packs' in parallel?
```

---
## \#20 Posted by: Namasaki Posted at: 2017-06-21T15:43:58.918Z Reads: 263

```
I think the problem in your case is the charger.
If your using a brick charger, I believe the charger turns itself off when it detects what it thinks is full charge. 
I'm using a power supply with my bms's and it doesn't shut off, it just slowly reduces current to the battery until the cells are full. 
I think the brick chargers, especially the cheap 2a models are just not dependable
```

---
## \#21 Posted by: Jinra Posted at: 2017-06-21T15:48:35.240Z Reads: 259

```
I have two chargers that both output 42.2v. Also my BMS (that doesn't balance) charged to full.

@darkkevind You only need 1 BMS, and yes you treat each parallel group as 1 cell.

>I think the brick chargers, especially the cheap 2a models are just not dependable

I think in the case of brick chargers, charging is entirely dependent on the BMS. The charger only thinks it's full because the BMS is blocking any more current from flowing. I'm sure this is how all commercial boards are built as well. I'm guessing my BMS's are just duds, or the overcharge release is somehow affecting charging behavior
```

---
## \#22 Posted by: Vieo Posted at: 2017-06-21T16:30:38.954Z Reads: 248

```
Maybe try contacting **BesTech** they seem to communicate well? Would be nice to have the answer to this
```

---
## \#23 Posted by: sl33py Posted at: 2017-06-21T17:05:09.730Z Reads: 248

```
[quote="darkkevind, post:19, topic:25819, full:true"]
Guys, noob question here. If I have an 8s4p pack, do I need 4 BMS's?

If not, how does it work with just one BMS and 4 'packs' in parallel?
[/quote]


No just one 8s BMS.  The 4p is seen as a single larger cell and charges as one.  each group in parallel gets the single balance lead to BMS - regardless if 1, 2, or 10p.

so for simple math - 25R in 4p is seen as 1 10,000mAh cell not 4 x 2500 mAh cells - per balance lead.  As expected when you charge 2500mAh vs 10,000mAh - it'll charge slower the larger the capacity.

HTH - GL!
```

---
## \#24 Posted by: NAT-Frank Posted at: 2017-06-21T17:05:37.176Z Reads: 238

```
This is exactly what I've been looking for to use on my 10s Lipo board. I only wanted the charging option in a small footprint. Now how do I got about buying one? :unamused:
```

---
## \#25 Posted by: smurf Posted at: 2017-06-21T17:41:09.222Z Reads: 236

```
That may be true for some BMS's but it is a good idea to let the battery cool down after charging for 20-30 minutes before using it and vice versa don't charge a hot battery pack immediately after using it.
```

---
## \#26 Posted by: Mobutusan Posted at: 2017-06-22T04:48:22.141Z Reads: 239

```
These look lif like a good small, inexpensive solution. But that shipping cost is pretty steep. Maybe someone can set up a group buy for these and we can all save on shipping.
```

---
## \#27 Posted by: Sleepingalex24 Posted at: 2017-06-22T14:16:17.476Z Reads: 235

```
@sl33py Is what I have here correct when you have batteries in parallel and in series? <img src="/uploads/db1493/original/3X/4/7/479a8a9d3f125d69beebdbc16c895785d79142dd.png" width="607" height="345">
```

---
## \#28 Posted by: Namasaki Posted at: 2017-06-22T15:29:44.754Z Reads: 224

```
It is correct if your not bypassing the bms during discharge and you have a bms capable of high discharge current.
```

---
## \#29 Posted by: Sleepingalex24 Posted at: 2017-06-22T15:31:52.880Z Reads: 223

```
I bought a 60A BMS and I don't have very many hills in my city so I imagine I will never reach that type of current.
```

---
## \#30 Posted by: memesupreme Posted at: 2017-06-22T15:44:14.042Z Reads: 219

```
Those are tiny! My 12s 80amp bms is like 200mm long and 120mm wide! Well, not the actual bms but the sheet of metal it's attached to, by the way is it safe to drill through that metal? It looks like just a normal sheet of aluminium, might actually be a heat sink, I don't know
```

---
## \#31 Posted by: Namasaki Posted at: 2017-06-22T16:07:37.121Z Reads: 213

```
60a will be plenty to handle discharge and you will have all the protection that the bms affords.
```

---
## \#32 Posted by: darkkevind Posted at: 2017-06-23T10:42:27.571Z Reads: 207

```
@Jinra how do you order from Bestech? I've found a BMS I'd like but there's no prices and I can't see a way to order?

Cheers :thumbsup:
```

---
## \#33 Posted by: TarzanHBK Posted at: 2017-06-23T11:17:21.442Z Reads: 201

```
you have to write them an email.
```

---
## \#34 Posted by: darkkevind Posted at: 2017-06-23T11:18:39.836Z Reads: 200

```
Ah I thought that but then I thought, no wayyyyy they must have an online shop! lol

I guess not. Cheers :thumbsup:
```

---
## \#35 Posted by: darkkevind Posted at: 2017-06-23T12:58:01.946Z Reads: 206

```
I just bought some LG INR18650-HG2 3000mAh - 20A Li-ion batteries to make up an 8s4p pack, can anyone recommend a good BMS please?

I have a question, why can't I just use 4 x TP4056 boards and a 33.6v 10A charging brick?
```

---
## \#36 Posted by: LukePL Posted at: 2017-06-23T13:17:36.895Z Reads: 217

```
Any one tried this one?
https://www.banggood.com/10S-36V-Li-ion-Lithium-Cell-20A-18650-Battery-Protection-BMS-MOS-Board-With-Balance-Function-p-1127995.html?rmmds=search
or this one
https://www.banggood.com/10S-36V-35A-Li-ion-Lithium-Battery-Protection-BMS-PCB-Board-With-BALANCE-p-1148775.html?rmmds=search
It's cheap with free delivery.
Thanks
Luke
```

---
## \#37 Posted by: banjaxxed Posted at: 2017-06-23T14:01:03.356Z Reads: 220

```
I bought the second one from banggood in advance of a more serious BMS like Besttech I am planning to use it on the charging side only due to it's low Amp rating. It doesn't having any charging wires

Anyone have experience of these ones?
http://www.ebay.co.uk/itm/122557037984

http://www.ebay.co.uk/itm/162414146757?var=461438635593
```

---
## \#38 Posted by: darkkevind Posted at: 2017-06-23T16:18:57.515Z Reads: 216

```
Can you use an 10s or 12s BMS on an 8s pack? You just don't connect up the extra wires right? It'll still charge and discharge each cell to the correct voltage won't it?
```

---
## \#39 Posted by: darkkevind Posted at: 2017-06-23T16:22:12.520Z Reads: 214

```
Also, another question, is the AMP rating you get with most BMS' discharge capability for each cell/ 's' or the whole output overall?
```

---
## \#40 Posted by: Guacamoleface Posted at: 2017-06-23T16:23:59.532Z Reads: 220

```
@Jinra 
did you have to order two from them or do they allow only one? I recall they put their lowest limit on 2 products but not sure.

EDIT: I did notice they are adjustable aswell as there seem to be different variants of the BMS with different overcharge voltages. Maybe you got the wrong one or voltage is just set low?
```

---
## \#41 Posted by: Jinra Posted at: 2017-06-23T18:34:46.014Z Reads: 208

```
Yea you have to order at least 2. They sent me a datasheet with each BMS which overcharge voltage was listed as 4.25v. No cells go over 4.06~v though
```

---
## \#42 Posted by: Guacamoleface Posted at: 2017-06-23T18:45:04.090Z Reads: 207

```
Allright! may be worth it eventhough I have to order 2, Currently running without bms and have no problem but would be a nice thing to have.

Also lacking space so the size of them really appeals!
```

---
## \#43 Posted by: Jinra Posted at: 2017-06-27T06:03:44.435Z Reads: 196

```
FOLLOWUP:

Turns out you actually **need** to solder on B- on the BMS. I thought the B- from the balance lead would be sufficient, but apparently not. My pack now charges to 42v with a ~.7v cell deviation at the highest.
```

---
## \#44 Posted by: Namasaki Posted at: 2017-06-27T11:34:14.287Z Reads: 191

```
Yes, for bypassing (not recommended) you still need to connect the battery's negative  main to B- 
But you don't use the P- except for negative charge wire unless the bms has a separate pad for charge C- in which case you don't use the P- at all
```

---
## \#45 Posted by: Jinra Posted at: 2017-06-27T14:37:53.279Z Reads: 189

```
Yes, i just thought I'd be fine with balance negative since my other bms worked perfectly fine without it.
```

---
## \#46 Posted by: sl33py Posted at: 2017-06-27T15:03:10.672Z Reads: 198

```
I'll definitely find a use for the one i got (80A discharge so big w/ heatsink), but would like small if i'm going to build into a thin board...

For the folks who know - is there a supower 12s that's also small and bypass?  Or is bestech the way to go?
```

---
## \#47 Posted by: Sebike Posted at: 2017-06-27T15:34:13.765Z Reads: 201

```
<img src="/uploads/db1493/original/3X/2/3/23d423034adc1822067d6b03ab6ddf9d51737a45.jpeg" width="690" height="388">
Would this be the correct way of bypassing BMS during discharge then?
```

---
## \#48 Posted by: Jinra Posted at: 2017-06-27T16:22:18.728Z Reads: 199

```
looks good to me
```

---
## \#49 Posted by: sprocket12 Posted at: 2017-06-27T16:41:45.549Z Reads: 195

```
So, what about this for an 8s setup with balance charging only and VESC discharging?

https://hobbyking.com/en_us/8s-li-ion-pcm-charge-4a-discharge-10a.html
```

---
## \#50 Posted by: memesupreme Posted at: 2017-06-28T08:15:39.381Z Reads: 189

```
If 10 amps is the amount of current you want to draw from the battery then yeah that should be fine, that would mean your motors will be getting 10 amps max, on 8s that's only 296 watts of power.. being such a low current though you're not going to have any trouble with over heating I'm pretty sure
```

---
## \#51 Posted by: jrpwit Posted at: 2017-06-28T10:27:52.556Z Reads: 190

```
I have the same battery configuration and same cell. I have been using a 8s battery support 60 amp bms. 

However ordered some new cells for a 12s pack cause 8s is enough for me!!!  

Good luck with your pack!
```

---
## \#52 Posted by: aigenic Posted at: 2017-07-09T11:29:13.640Z Reads: 178

```
Hi, I am looking for a small BMS just for charging...I have found [this](http://www.ebay.co.uk/itm/10S-37V-16A-Li-ion-Lithium-Battery-BMS-PCB-PCM-Board-For-Ebike-Electric-Bicycle-/352104358559?hash=item51fb0e229f:g:LrYAAOSwyltZWh6h) one on ebay, is it okay? Does anyone have experience with it?

I am quite limited by space, because I will be using split enclosures and I dont know how to charge...I dont want to remove the enclosures everytime to charge like I did so far...should I bypass small BMS, buy normal one and use it even for charging (I would have to lead balance wires under the grip tape to the enclosure with VESC) or find some multi pin connector and use BMS outside the board (12 pin would be enough in case of 10S, 1 pin would be empty)

Any advice is welcome :)
```

---
## \#53 Posted by: Jinra Posted at: 2017-07-09T16:03:58.345Z Reads: 171

```
that bms doesn't balance. why not use one of the bms's mentioned in this thread?
```

---
## \#54 Posted by: aigenic Posted at: 2017-07-09T16:44:38.300Z Reads: 174

```
@jinra I thought it is bigger :O Ok ,t will go with it :D sorry about that :D 

How can I order from them? do I have to write an email or is there any store?
EDIT: I found it, it was posted few replies abouve this one :D
```

---
## \#55 Posted by: willpark16 Posted at: 2017-08-12T07:31:43.249Z Reads: 157

```
Which do u recommend more and are the switches working?
```

---
## \#56 Posted by: Guacamoleface Posted at: 2017-10-24T17:11:58.339Z Reads: 138

```
@Jinra 

How are theese bms holding up? Tried both or the one u initially installed works fine still?

Figured  I may aswell try and get some space now that winter is coming and I aint riding :frowning:
```

---
## \#57 Posted by: Jinra Posted at: 2017-10-24T18:42:41.168Z Reads: 139

```
I'm using the red one, great so far on two different packs!
```

---
## \#58 Posted by: sid1 Posted at: 2018-01-16T04:13:47.518Z Reads: 101

```
i am so confused. I either want to do 2 5s, or 2 4s, in series, so can someone tell me what is a good bms, charging port, charger, and how to wire all the stuff. Sorry for asking noob questions
```

---
