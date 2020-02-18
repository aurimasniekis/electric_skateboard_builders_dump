# How much juice can I throw at a dual FOCBOX setup?

### Replies: 47 Views: 4116

## \#1 Posted by: DanSkates Posted at: 2017-05-18T03:47:37.676Z Reads: 513

```
Hi Peeps,

I'm in the process of building an eMTB with a Trampa base, Direct Drive system from @Nowind and dual VESC-X (separate topic running [here](https://www.electric-skateboard.builders/t/e-mtb-build-would-this-trampa-foundation-work-and-the-future-of-e-mtb/21343)), but was after some specific electrical advice here so it wouldn't get lost with the other thread.  

Qs:

1. How much power can I put into the VESC-X?  I know a lot of eMTB builds focus on high burst lipos but is there a danger I'll buy too much power and not be able to use it or just blow my VESCs??  

2. Would I be silly spending loads of money on expensive lipos when some cheaper 20c would do the job if I have to restrict my BLDC settings??  

3. Speaking of which what are the safe max settings for the VESC-X? 

I have to say I'm totally useless when it comes to this side of things as I built my first board with a SPACE CELL 4 so all the hard work was done for me.  I'm having to work a little harder on this one!  

For motors I'll be using either SK3 6374 149kv or 168kv and was hoping to run a 12s2p battery with at least 10ah.  

Hopeful this isn't too vague, I know I'll also need to order connectors, and make a loop key or anti-spark so any additional info to help finish the electrical side of things would be greatly appreciated.  Ideally if anyone can point me towards a complete build to learn from that would be great.  

As per my linked topic above I want to ride this beast on BMX and motocross tracks so I'm mostly interested in immediate hard (but smooth!) acceleration / torque.

Thanks,

Dan
```

---
## \#2 Posted by: Sourcecode Posted at: 2017-05-18T05:10:31.421Z Reads: 476

```
This is what im using atm, hopefully it may be of some use to you in your build  :slight_smile:
Im running my dual VESC-X on 12S on my EMTB for some time now. linked via canbus.
No problems using 4 x 6S 45-90c 5000mah lipos ( 2 series packs in parallel so 10000mah total)
The batteries seem to cope well and only get slightly warm when i give my board death
My motor max is set at 80 amps on each vesc using 2 SK3 6374 192kv motors.
Limited to 60000 erpm
14 tooth Pinion, 66 tooth spur and 8inch wheel belt drive
heaps of power, can get up rather steep hills towing someone on a longboard behind me lol.
Draws about 25 Amps on each Vesc at 60kmh my range is around + - 20km ish 
Temps stay around 60c due to the heat sink i have them mounted on 
using 4 x 1watt 100ohm resistors in parallel as my anti spark atm 

But looking at the track you want to use you may want 2 x 12s car escs for more of a dirt bike feel with the lower kv motor (149 kv)and smaller pinion gear for more torque 
(dont shoot me for suggesting something other than a vesc lol  :joy: ) 

In conclusion to your questions:

1, power will depend on your gear your using in my rc experiences more c rating the better, however if you Get a higher mah pack you can have a lower c rating.

2, from the looks of it you shouldnt have to restrict anything apart for the voltage cutoffs for when your lipos are flat and maybe set motor max and batt max. for the lipos it will depend on the mah and C rating for how much power they can deliver
 in theory (somebody correct me if im wrong) 
a 20c 10000 mah pack can deliver 20 x 10000 = 200amps
or a 45c 5000 mah pack can deliver 45 x 5000  225amps
Having the batteries be able to burst high amps for a a few seconds is why i think the higher c rating is better
( For like starting off on a hill/on grass etc or towing a train of people behind you haha)  
so for a 5000mah 45-90c pack can give you 90 x 5000 = 450a for a few seconds
over time i think it will be less stress on your batteries having a higher c rating. 

3, Max setting will again depend on what gear you're using, as long as its with in the limits of the specification on the vesc -x you should be fine

cheers
```

---
## \#3 Posted by: Namasaki Posted at: 2017-05-18T06:27:09.130Z Reads: 400

```
I agree totally with @Sourcecode
I'm running 60/120C  5000 Lipos in series for 10s on my street board And it works well with minimum Voltage Sag even when charging up hills. 
With a mountain board, you need raw power. 
The Vescs in my opinion will not be the weak link. 
It seems to me that batteries are usually the weakest link. 
Therefore, I like to say that it is impossible to over build the battery.  My advise is get the highest C rated Lipos you can with at least 5000mah capacity.
And though it might seem like overkill, it really isn't. 
Because you need as much headroom with your batteries as you can get to reduce voltage sag, over heating, loss of power and loss of range.
```

---
## \#4 Posted by: Duffman Posted at: 2017-05-18T12:52:16.900Z Reads: 369

```
I have the impression, that the higher the C rating of a battery, the more it differs from the actual C rating the battery can deliver (at least for the same voltage sag). One thing is clear: The advertised values are only valid for new batteries and get worse over the time. 

In other words: It is a good idea to keep a good safety margin in your setup. Lets say the batteries should be able to deliver double the power the motors can pull, to be on the save side when your batteries get weaker.

So either go with small and light high discharge lipos and exchange them more often or take bigger medium discharge lipos for more range. It's up to you and your riding style.
```

---
## \#5 Posted by: DanSkates Posted at: 2017-05-18T16:32:59.587Z Reads: 324

```
Thanks @Sourcecode, @Namasaki & @Duffman - really good information there.  It's funny, when I look at the smaller but more extreme BMX tracks I wanna ride the ability to roll actually generates a lot of momentum and I just need that added boost in between transitions to get some air!   I'm proabbaly gonna end up building something with even more guts than I need but much better to have the power available than not.

Btw @Sourcecode do you have a link to that build anywhere?  Really nice looking board!  

I actually came across [these batteries](https://hobbyking.com/en_us/turnigy-lihv-5000mah-4s-15-2v-35c-hardcase-pack.html) earlier which look interesting.  I also think working with hardpacks like this and being able to build my own connectors would be pretty good.  @duffman, I've posted them on one of your topics too here as I'm blown away by the swappable batteries you made and think these would do very well in a similar design.
```

---
## \#6 Posted by: Duffman Posted at: 2017-05-18T17:07:41.292Z Reads: 296

```
Those are even better, as they already have the connectors build in. It was a shit load of work to build my battery connectors.

If you do it clever, you can build your board with 3s2p 'docking ports' for these batteries. Then you can choose everytime if you want to drive either with 3 packs for big jumps or with 6 packs for more range.

As long as you are 'rolling' on normal terrain, power draw should not be the problem. But if you start drifting things are getting serious...
```

---
## \#7 Posted by: DanSkates Posted at: 2017-05-18T17:25:30.243Z Reads: 279

```
Oh shit yeah!  I suppose similarly to how your's plug in I could just plant these face down directly on to the docks - loving your work!  Hey, btw what bullet connectors do you use?  Do you just solder standard 5.5mm gold ones at a right angle?  I don't have the skills or access to a 3d printer unfortunately, but I'm pretty sure I could fashion something halfway decent!
```

---
## \#8 Posted by: Duffman Posted at: 2017-05-18T18:53:06.334Z Reads: 253

```
I guess I was using 6mm connectors. Not 100% sure right now.

You could just use the connectors that come with the batterys, poke them trough a piece of cardboard  in the batteries, solder them on the backside and hold them in place with a huge load of hot glue, covered with a piece of wood.

Do yourself a favor and get a proper coulometer battery gauge. Not these crappy voltage based thingys. I can fully recommend the one I used in my builds. It says max 100A but I'm running up to 240A trough it without amy issues. Will post a link tomorrow...

You should also connect the balancing leads to some lipo savers to get notified if a cell runs low while the rest of the pack is still ok.
```

---
## \#9 Posted by: DanSkates Posted at: 2017-05-19T01:18:17.369Z Reads: 239

```
[quote="Duffman, post:8, topic:23352"]
Do yourself a favor and get a proper coulometer battery gauge. Not these crappy voltage based thingys. I can fully recommend the one I used in my builds. It says max 100A but I'm running up to 340A trough it without amy issues. Will post a link tomorrow...
[/quote]

I will for sure!  Please send the link and I'll jump right on it :slight_smile:

By lipo savers you mean these bad boys: https://hobbyking.com/en_us/hobbykingtm-lipoly-low-voltage-alarm-2s-6s.html.  You mentioned in your build that they have a reed switch which get's activated by the dock on the board - what's a reed switch? 

Thanks a lot for all your help - if I can get anything half way near your build I'll die a happy eMTB builder! :wink:
```

---
## \#10 Posted by: lrdesigns Posted at: 2017-05-19T01:22:55.172Z Reads: 228

```
About 250 ml's of apple juice should do it .......:joy:
```

---
## \#11 Posted by: DanSkates Posted at: 2017-05-19T01:52:12.977Z Reads: 224

```
LMAO!! :laughing:
```

---
## \#12 Posted by: DanSkates Posted at: 2017-05-19T01:53:08.760Z Reads: 223

```
...After all the drama over the name VESC I've changed the title to FOCBOX as per Jason's rebranding!  I couldn't give a FOC either way but happy to play the game :wink:
```

---
## \#13 Posted by: Duffman Posted at: 2017-05-19T07:26:00.134Z Reads: 228

```
Good news! There is already an upgraded version in a nicer case and with a shunt PCB of the coulometer I'm using available:

This is the 50A version, which seems to use the same shunt  as mine, through which I use to hammer up to 240A...
https://www.aliexpress.com/item/50A-New-TK15-Professional-Precision-Battery-Tester-for-LiFePO-Coulomb-Counter-Free-Shipping-with-Tracking-Number/32702066121.html?spm=2114.01010208.3.1.4ODWkd&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10065_10151_10068_5010019_10136_10157_10137_10060_10138_10155_10062_10156_437_10154_10056_10055_10054_10059_303_100031_10099_10103_10102_10101_10096_10147_10052_10053_10050_10107_10142_10051_10084_10083_10080_10082_10081_10177_10110_519_10111_10112_10113_10114_10181_10180_10183_10182_10185_10184_10078_10079_10073_10186_10123_142-10102_10112,searchweb201603_4,ppcSwitch_2&btsid=1e61e3a9-d827-4a56-a69b-59e4a93690e4&algo_expid=1c653148-6336-495b-a11d-0d4065e17af0-0&algo_pvid=1c653148-6336-495b-a11d-0d4065e17af0

This is the 100A version which should hold up even more abuse:
https://www.aliexpress.com/item/100A-New-TK15-Professional-Precision-Battery-Tester-for-LiFePO-Coulomb-Counter-Free-Shipping-12003194/32703947698.html?spm=2114.10010108.1000013.3.HeFSWj&traffic_analysisId=recommend_2088_2_82199_new&scm=1007.13339.82199.0&pvid=b86b57c5-d647-4bb3-aba3-c370889a3905&tpp=1

For the lipo alarm, I'm using the similar version with the small display, but the more important functionality is the beeper that warns you if a cell gets weak. Best would be a 12s lipo alarm, but I haven't found a proper and affordable version. This one would be a nice gadget: 
http://www.rcheli-store.de/Akkus-Zubehoer/Lipo-Checker-Monitor/MTTEC-Lipo-Waechter-BS12-V2-3-Einzelzellenueberwachung-Display-dual-Summer.htm?shop=rcheli&a=article&ProdNr=MTT-MT1813&t=9&c=20430&p=20430
```

---
## \#14 Posted by: Okami Posted at: 2017-05-19T12:30:08.156Z Reads: 213

```
Recently found this:

https://www.banggood.com/ISDT-BC-8S-Battery-Checker-with-Two-85dB-Buzzer-for-LiPo-LiHv-LiFe-LiIon-Batteries-p-1128253.html?rmmds=detail-top-buytogether

Looks like a pretty elegant solution,.. but then again, costs about the same as proper energy / wattmeter duffman already referenced to and works only up to 8s.
```

---
## \#15 Posted by: DanSkates Posted at: 2017-05-20T11:32:03.443Z Reads: 203

```
thanks @Duffman and @Okami these look great!
```

---
## \#16 Posted by: DanSkates Posted at: 2017-08-24T04:14:14.865Z Reads: 192

```
Hey guys / @Duffman - I'm nearing the final stages of my build now and have all the components I need including the [coulometer](https://www.aliexpress.com/snapshot/0.html?spm=a2g0s.9042647.0.0.VyFuu0&orderId=85417516404809&productId=32703947698). I've hunted around for wiring diagrams of how to link it in and I'm still a bit in the dark.  The diagram in the description just confuses me even more! :fearful:

So far I have my wiring harness built from the battery to the FOCBOXs with a loop key and it works great.  I’ve also just bought a 60A fuse too and it’s bloody ginormous - if I do end up blowing this it can accept up to 100A so I’ll grab one if and when it happens. I’m guessing for my fuse I can use it in place of the postive wire opposite the loop key which is on the negative wire and then join in the coulometer before the vescs?  My question is can I run it directly in the loop, or do I need to run it off to one side?  Sorry if this is vague, I’m not the most gifted when it comes to this side of things so any help is hugely appreciated – and if you have any pictures even better!! I’ll add a couple of pics of what I mean when I get home to make this clearer.  

Thanks for your help,

Dan
```

---
## \#17 Posted by: Duffman Posted at: 2017-08-24T05:07:33.711Z Reads: 192

```
Hey Dan,

the chinese diagrams are somewhat 'special'...

<img src="/uploads/db1493/original/3X/8/e/8eecd2abee22fb2996f4aa7865ce14b946c9b665.png" width="690" height="325">

But it is easier as it seems: 

The coulometer has 4 wires. Two for measuring the battery voltage (B+ B-) and two for measuring the current (RS+ RS-).
As our currents are too big to be measured directly, we have to use a shunt (in the diagram: The outer sampler). It has also 4 connectors. Two for the power wires (the big ones) and two for the measured current (-> connect to RS+ RS-).

It is important to connect one side of the shunt directly to the negative side of the battery. The other side should be connected to the ESC (-). The ESC (+) should be connected to the fuse, the fuse to the loop key and the loop key to the positive side of the battery.

Other as shown in the diagram the B+ connector of the coulometer should not be connected directly to the battery but after the loop key. Otherwise the coulometer would always be powered and would drain the battery even when the loop key is disconnected.

<img src="/uploads/db1493/original/3X/2/e/2e9f06fb4eb0adac93f7cf0ce769e8076882fd89.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/4/e/4e5ad2597c304523077516df7204e5c2d0cbbceb.jpg" width="690" height="388">


----------

For my builds I combined the loop key and the fuse. I'm using a 100A 'mini anl fuse' without case and directly soldered to the power wires:
<img src="/uploads/db1493/original/3X/8/a/8adad3a5d3f41de9603899bf794717dba87cc695.jpg" width="690" height="388">
```

---
## \#18 Posted by: DanSkates Posted at: 2017-08-24T08:00:27.287Z Reads: 182

```
Hey @Duffman - thank you for the fast response and detailed info - I'll look this over when I'm in front of the components to see if I can apply it.  So is your shunt the black part on the left in your photo?  Is that what your unit came with?  I currently have a huge copper looking unit with 2 bolts: 

<img src="/uploads/db1493/original/3X/9/9/99e58433968f433eff17358a63d988e1a59d572c.PNG" width="532" height="372">

Will this work in the same way or do I need to snip that cable?

I'll try and get hold of one of those fuses instead and use your method as the thing I bought is a bit bloody ridiculous :laughing:

<img src="/uploads/db1493/original/3X/9/c/9c3a1e8e8523238271f164444d90256657db64e9.JPG" width="375" height="500">

Btw - I have normal size hands - this thing is just huge!!
```

---
## \#19 Posted by: Duffman Posted at: 2017-08-24T11:02:09.236Z Reads: 178

```
If you have a shunt with a PCB and an extension cable like on the picture, then it's even easier to connect.

Just connect the power wires to the bolts, +- from the battery to the screw terminal and your loop key somewhere in the positive battery cable.
```

---
## \#20 Posted by: DanSkates Posted at: 2017-08-24T13:43:42.331Z Reads: 175

```
So could I then run the +- wires from my dual soldered focbox on to the shunt too? So battery in on one side and my focboxs off the other? It certainly saves connectors and strikes me it's doing the same? Thx
```

---
## \#21 Posted by: Duffman Posted at: 2017-08-24T14:17:01.283Z Reads: 169

```
If I got you right it is exactly the way I did it.

Wire the ESCs in parallel, connect them to the battery, cut both battery wires wherever you like and solder the shunt in the negative line and the loop key with fuse in the positive line.
```

---
## \#22 Posted by: DanSkates Posted at: 2017-08-24T23:17:58.963Z Reads: 163

```
I'll give it a try....what's the worst that could happen!? :wink:

<img src="/uploads/db1493/original/3X/7/d/7d6b012505a748322163a4b3baaa082496320461.jpg" width="690" height="431">
```

---
## \#23 Posted by: flywithgriff Posted at: 2017-08-24T23:42:00.710Z Reads: 152

```
Just a word of warning, be careful with the FOCBOX. I purchased two of them thinking they were great for FOC and now all I see are people having issues!
```

---
## \#24 Posted by: nw-esk8 Posted at: 2017-08-25T00:35:57.212Z Reads: 158

```
Are the recent ones still having issues or are you referring to the older ones?

(they were on my esc/vesc radar, too... but a few spots down)
```

---
## \#25 Posted by: flywithgriff Posted at: 2017-08-25T01:36:33.575Z Reads: 153

```
The brand new ones unfortunately. Seems they are actually just a relabeled vesc-x.
```

---
## \#26 Posted by: cypa9904 Posted at: 2018-04-15T11:38:53.090Z Reads: 121

```
Hi.
Are your FOCBOXes still OK? I also wonder if you are (were) using FOC of BDLC mode?
```

---
## \#27 Posted by: Brad Posted at: 2018-04-15T13:39:01.293Z Reads: 124

```
You got that one right. 

The massive "c"'s is really more wrong the bigger it gets. Here is spreadsheet 1 of 4 showing advertised c and true c. It is about 4 years old, but I would wager that the problem is still there with the newer batteries. 

There was even one Lipo company that was being truthful and advertised both competitive c and true c using c for customers.

If cycle and voltage did not bother me and I need as much juice as I need, I would still go LiPo.

![True c 1|566x500](upload://7XvigL8bdEENp3mHqUrO30l30Ui.PNG)
```

---
## \#28 Posted by: Deckoz Posted at: 2018-04-15T14:14:14.862Z Reads: 116

```
Hey @DanSkates It's probably a little late for me to answer this... But the focbox with decent cooling can do around 1900w continuous, and up to 3500 burst.

I'm sure your board is already setup..  but the copper pours on the PCB are only thick enough to handle ~60 battery amps, so I keep the battery amps at 50 or below... But the fets are rated up to 250A... I have my motor max at 125A and my absolute max at 190. In order to keep the heat down, I have a max wattage setup for 2500w, so as the duty cycles increases it lowers the motor amp..to stay in the Watt range it can dissipate. Give me incredible acceleration in the bottom...

I don't think @Nowind or @BigBoyToys used watt limits.. but the motor amps let's you accelerate from a dig with alot of force.
```

---
## \#29 Posted by: Cobber Posted at: 2018-04-15T14:24:46.865Z Reads: 111

```
Jenso is on 100BA 130MA 175AC... (from last video)

your'e on 50BA 125MA 190AC with a 2500w limit?

@Deckoz changed your profile again bro, your killing me! :zipper_mouth_face:
```

---
## \#30 Posted by: Deckoz Posted at: 2018-04-15T14:30:41.586Z Reads: 108

```
@Cobber but he's on vesc6 :slight_smile:
Meh... Profile bleh
```

---
## \#31 Posted by: Cobber Posted at: 2018-04-15T14:38:18.804Z Reads: 106

```
yeah for sure...
profile is how I know you dude! :neutral_face:

and now we are all getting on vesc 6.4 based stewii-b-box...

relatively you pushed MC & AC much more, might be something in that?
maybe with lower BC, MC & AC can be driven higher?
```

---
## \#32 Posted by: Deckoz Posted at: 2018-04-15T14:53:27.972Z Reads: 104

```
Lol

Identity crisis...

And I think the focbox only has 2oz copper pours...and vesc 6 and stewii new pcbs use 3oz..I'm not 100%

Either way those amperages would be burst in normal use unless your going up a long hill? As the motors unload some at higher speeds? 

I never ever see 100+ motor amps unless I'm under heavy acceleration at low speed..... contrary to that..the clone Evo uses no watt limit and he can hit 100a+ at 20mph.. if he gasses it... But it only last for a second since the motor unloads quickly. To me at higher rpms I feel like that many amps can "shift" the board to fast...so I like the motor amp to taper down as the speed increases... It makes it feel as if there is more "resolution" in the throttle... Speed increases, amp max goes down due to wattage/bat max, dumbing jerkyness in the throttle with the faster speed..making it predictable.

At least that's the advantages to me..... idk..I'm sure everyone's thumbs/body feeling are different.

My batmax is because of my batteries though... I have it split for continuous rating...(50A/50A).. if I used lipo or a bigger parallel I could go higher... But I don't know if I would trust the copper pours on the focbox for more then 50 battery amps... Without external cooling.... Where the vesc 6 can hold 70A continuous for 10min +
```

---
## \#33 Posted by: Cobber Posted at: 2018-04-15T15:02:10.336Z Reads: 98

```
your'e on the bleeding edge bro :astonished: not sure what to make ...
```

---
## \#34 Posted by: Deckoz Posted at: 2018-04-15T15:05:27.343Z Reads: 100

```
Idk...

I just think that the ESCs have more potential then people think... And the ability to make the bottom end a rocket...

Why put 250A direct fets on and only throw 30 amps through them...
```

---
## \#35 Posted by: Sourcecode Posted at: 2018-04-16T00:06:29.618Z Reads: 95

```
Both are still alive. Tho only ever used bldc. Thinking about swapping to foc but never did because of all the dramas I see people having lol.
```

---
## \#36 Posted by: Cobber Posted at: 2018-04-16T00:32:49.040Z Reads: 91

```
Are you getting any over current fault codes ever Decky?
```

---
## \#37 Posted by: Deckoz Posted at: 2018-04-16T00:43:52.128Z Reads: 91

```
Never. But sensors are necessary to use these numbers from a stop with no kick... Otherwise you may get a squeal and an AC fault ;) but that's with any non sensored setup... Can't no kick start without them..
```

---
## \#38 Posted by: Cobber Posted at: 2018-04-16T00:59:11.614Z Reads: 88

```
Are you going to wind up the current on your eMTB build?

I wasn't going to go past ~70 BA on my new one with ESCapes.
```

---
## \#39 Posted by: Deckoz Posted at: 2018-04-16T01:11:28.496Z Reads: 87

```
I dunno yet. Gonna wait to see how it feels. It wouldn't be to much higher at 6p... 120a/2... 

If I really wanted to crank it id need lipos.. but really I think if you wanna crank it you just have to setup the cooling to keep it cool... likely.
```

---
## \#40 Posted by: Cobber Posted at: 2018-04-16T01:17:17.784Z Reads: 86

```
Thing is Trampa gets all bucky with torsional twist and not just on acceleration, deceleration too. Just coming off the throttle can induce it at higher speeds/load. 

I def. don't want anymore than my 160kv even 150kv would be enough I think, but I have high "c" lipos...
```

---
## \#41 Posted by: Deckoz Posted at: 2018-04-16T01:24:36.649Z Reads: 84

```
You talking board flex from the flex being to weak vs a stronger flex?

Yea I'm aware of that. Flex boards do that, they feel like noodles lol. Gotta ride it out on a rail. My surfboards do torsional flex too... 

I'm not sure what other kind of bucking you would mean?
```

---
## \#42 Posted by: Cobber Posted at: 2018-04-16T01:31:15.401Z Reads: 82

```
Yeah, noodle :ramen: dude

RIP BigBoyToys struggled to get his monster 4wd over 40mph, around 35mph it started for him, as he would come off the throttle it would buck and throw him.

Maybe front wheel drive might be better, but I think Trampa is better for jumping than going fast so just use it for that!
```

---
## \#43 Posted by: Deckoz Posted at: 2018-04-16T01:32:51.832Z Reads: 84

```
Yea...my trampa likely gonna max around 30.. But I'll likely ride it in the 15-24 range and never feel the battery sag.. lol

Don't want it to go fast...

My vanguard was a noodle...and I took that thing over 30 all the time... Never again lol.

We have some mountains close to me. And alot of us love going out to them for the breweries...there's a couple mountain board tracks/MTB trails 😎
```

---
## \#44 Posted by: DanSkates Posted at: 2018-04-16T11:28:09.543Z Reads: 73

```
[quote="Deckoz, post:28, topic:23352"]
Hey @DanSkates It’s probably a little late for me to answer this… But the focbox with decent cooling can do around 1900w continuous, and up to 3500 burst.

I’m sure your board is already setup…  but the copper pours on the PCB are only thick enough to handle ~60 battery amps, so I keep the battery amps at 50 or below… But the fets are rated up to 250A… I have my motor max at 125A and my absolute max at 190. In order to keep the heat down, I have a max wattage setup for 2500w, so as the duty cycles increases it lowers the motor amp…to stay in the Watt range it can dissipate. Give me incredible acceleration in the bottom…
[/quote]

Dude - my board is anything but setup correctly!!!  It's rideable, but could defo do with some tweaks!  I actually buggered up one of the USB ports so haven't been able to adjust the settings for a while but my new soldering equipment will arrive this week and then I can fix this and all the other stuff I've broken or blown up :smile:

I can't wait to try out these settings - really appreciate you digging out this post and adding this information.  I've not heard anyone explain it like this before but having read some recent posts it makes perfect sense.
```

---
## \#45 Posted by: DanSkates Posted at: 2018-04-16T11:31:37.620Z Reads: 71

```
I'm all about the bottom end!!!  Having fallen on tarmac now fully strapped in I'm in no rush to race this thing on the road and it's just not possible to get up to full speed on grass/dirt.  It's all about the torque bro!
```

---
## \#46 Posted by: Acido Posted at: 2018-04-16T13:04:00.862Z Reads: 62

```
There are no 5ah cells you would need to go 4p of 30q for 80a constant and 12ah
```

---
## \#47 Posted by: Acido Posted at: 2018-04-16T13:04:54.787Z Reads: 61

```
Top speed does not matter much!
Especially if you are in the city where you need to stop and start a lot :)
```

---
