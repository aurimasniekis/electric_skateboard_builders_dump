# Magsafe as charge port

### Replies: 79 Views: 7631

## \#1 Posted by: Maxid Posted at: 2016-11-22T09:29:09.603Z Reads: 683

```
Since I am currently trying to build a stealthy build I thought about charging port solutions.
The standard 5.5mm plugs seem pretty low-tech and I thought about how amazing the magnetic Apple charger port actually is.
Has anybody ever thought about using this type of plug for the DIY build? Seems like a great idea with a self-locking mechanism and dual power rails.

It should easily be doable with a magsafe 1 plug and a magsafe 1 to 2 converter that acts as the female end on the board. Solder the cables to the male magsafe 2 side and you should be done.

magsafe 1 charge cable
http://i.ebayimg.com/images/g/P4cAAOSw5dNWkkxz/s-l1600.jpg

magsafe converter (proposed female side on the board)
https://library.syr.edu/services/technology/loaner/images/plug.png

there are even caps out there to seal it up after charging
http://img.banggood.com/images/upload/2012/liuguanglian/SKU05833203.JPG
```

---
## \#2 Posted by: lox897 Posted at: 2016-11-22T09:35:06.531Z Reads: 619

```
And you could use the two outside pins for negative and the inside 3 for positive, or the other way around. That way you could plug it in any way and not have to care about polarity.
```

---
## \#3 Posted by: Maxid Posted at: 2016-11-22T09:35:27.634Z Reads: 615

```
exactly!
Just wondering if there are other reasons why people have not already done this.
```

---
## \#4 Posted by: Mark Posted at: 2016-11-22T09:39:35.235Z Reads: 610

```
Well lets try it then! Great idea!
```

---
## \#5 Posted by: sanka Posted at: 2016-11-22T09:40:02.258Z Reads: 596

```
Really good idea!
```

---
## \#6 Posted by: lox897 Posted at: 2016-11-22T09:46:50.420Z Reads: 590

```
Pretty cool teardown: http://www.righto.com/2013/06/teardown-and-exploration-of-magsafe.html
```

---
## \#7 Posted by: Maxid Posted at: 2016-11-22T10:04:47.509Z Reads: 592

```
Hm - I wonder if the voltage for a 10S system will destroy that small PCB and chip.
Also I don't know if the chip is wired in parallel so that the energy transfer can still take place even when the chip is blown. LEDs and stuff we don't need anyway - just a direct connection from one cable to the other is already enough.

Well there are even female boards:
https://eustore.ifixit.com/out/pictures/generated/product/1/380_340_100/31bc750303092083d09940537e8e022b.ZxaqCvFp5MKMRvFU.jpg
https://eustore.ifixit.com/en/Parts/MacBook-Parts/MacBook-13-3-MagSafe-DC-In-Board-Black.html

but they ain't cheap at 25€ :astonished:
```

---
## \#8 Posted by: lox897 Posted at: 2016-11-22T10:13:22.111Z Reads: 561

```
We'd probably be better off just using an xlr connector lol.
```

---
## \#9 Posted by: Maxid Posted at: 2016-11-22T10:14:48.240Z Reads: 549

```
where is the fun in that? ;)
```

---
## \#10 Posted by: tueboard Posted at: 2016-11-22T10:48:38.987Z Reads: 542

```
good idea @Maxid i really like the magnetic magsafe port, go ahead ;)
```

---
## \#11 Posted by: rmrf Posted at: 2016-11-22T11:17:40.230Z Reads: 525

```
@Maxid wow this idea is just BRILLIANT
```

---
## \#12 Posted by: Hillso Posted at: 2016-11-22T11:31:37.020Z Reads: 510

```
[pogo](https://www.aliexpress.com/item/SMT-7-5mm-male-pogo-pin-connector/32738317754.html?spm=2114.01020208.3.30.KwONxy&s=p&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_10084_10083_10080_10082_10081_10060_10061_10062_10056_10055_10037_10054_10059_10032_10099_10078_10079_10077_10073_10100_10096_10070_10052_423_10050_424_10051,searchweb201603_2&btsid=4c526398-8b66-4918-a08f-ab51f8e995eb) + [3d printing](http://www.instructables.com/id/3D-printed-magnetic-connector/)?
edit: [cheaper pogos](https://www.aliexpress.com/item/10pcs-Ultra-small-spring-loaded-pogo-pin-Diameter-2-3mm-3-0mm-heigth-brass-material-with/32621909653.html?spm=2114.01020208.3.65.qiplNq&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_10084_10083_10080_10082_10081_10060_10061_10062_10056_10055_10037_10054_10059_10032_10099_10078_10079_10077_10073_10100_10096_10070_10052_423_10050_424_10051,searchweb201603_2&btsid=6f1f37c7-21d8-4996-a410-60ad91eefb31)
```

---
## \#13 Posted by: Maxid Posted at: 2016-11-22T13:56:34.027Z Reads: 502

```
Well i think the hard part is not to get spring contacts but to actually make it magnetic. That 3D printed solution seems weirdly familiar no? ;)
```

---
## \#14 Posted by: Hillso Posted at: 2016-11-22T14:06:33.756Z Reads: 501

```
[ring magnet](https://www.aliexpress.com/item/1pcs-Internal-Dia-19mm-Ring-Rare-Earth-Neodymium-Magnet-N50-Strong-Ring-Magic-Prop-D25-5/32660807671.html?spm=2114.01020208.3.175.HpeuhN&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_10084_10083_10080_10082_10081_10060_10061_10062_10056_10055_10037_10054_10059_10032_10099_10078_10079_10077_10073_10100_10096_10070_10052_423_10050_424_10051,searchweb201603_2&btsid=4d444788-ffa1-4f5d-b2e3-89027769f0dc), and 20 mm metal washer on the other side.
 
pogos configuration - 5 pogos circle in the middle of the ring and 5 pogos around the first 5. should have enough space inside the ring magnet.

and we can add a threaded lid for waterproofing, something like [this](http://www.thingiverse.com/thing:1904270), but that looks like a lid.
```

---
## \#15 Posted by: mason Posted at: 2016-11-22T14:59:20.547Z Reads: 479

```
Soldering heat will be a big issue for the magnetic strength. I don't think this will work, though correct me if I'm wrong.
```

---
## \#16 Posted by: Hillso Posted at: 2016-11-22T15:23:54.760Z Reads: 495

```
magnet don't need to be close to the connector when soldering.
I don't know if it's comprehensible, but I painted the idea:
<img src="/uploads/db1493/original/3X/a/0/a01190e91547d3a430920dad8c19efbe3999a592.png" width="147" height="150">

I forgot about the female side of the connector. I haven't find any cheap female pogos. [those are 200 pcs](https://www.aliexpress.com/item/hot-sale-spring-pogo-pin-pogo-pin-connector-smart-watch-robot/32615580618.html?spm=2114.01020208.0.0.rEb3V7) :unamused:

[plan B](https://www.aliexpress.com/item/GETIHU-Quick-Fast-Charging-Data-Magnetic-Cable-For-iPhone-5-5s-5c-SE-6-6s-Plus/32721591620.html?spm=fLKTIe&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_10084_10083_10080_10082_10081_10060_10061_10062_10056_10055_10037_10054_10059_10032_10099_10078_10079_10077_10073_10100_10096_10070_10052_423_10050_424_10051,searchweb201603_2&btsid=37f0ee01-b183-49d9-84dc-f41622328eb9&aff_platform=aaf&sk=6mia6uvne%3A&cpt=1479825619853&af=cc&&aff_trace_key=5ef29800c05d4b3eac731cd1ea73747f-1479825619853-01706-6mia6uvne)?
```

---
## \#17 Posted by: Maxid Posted at: 2016-11-22T16:27:53.342Z Reads: 490

```
if you are soldering in way that the entire magnetic housing will get that hot, you are doing something wrong :D
```

---
## \#18 Posted by: B4Me Posted at: 2016-11-23T11:46:51.941Z Reads: 490

```
I was actually planning for building a wall mount, with build-in charger port, using pogo-pins 
http://www.larsenassociates.com/AriesCSPimages/AriesSpringProbesKelvin2008.jpg

And then when I hang my board, it will recharge if needed (and if I have told it so.. some logic/controller is neeeded)
```

---
## \#19 Posted by: Maxid Posted at: 2016-11-23T14:37:29.590Z Reads: 477

```
fun fact: the female jack can be bought in bulk on aliexpress for as cheap as 1.30€ per unit
https://de.aliexpress.com/item/New-Original-MagSafe-2-DC-Power-Jack-Borad-w-for-Apple-MacBook-Pro-Retina-15-A1398/32623222760.html

To test however I ordered a used DC board from an old macbook. Will let you know how it turns out. Cable part will be from a broken charger I have sitting in a drawer.
```

---
## \#20 Posted by: flatsp0t Posted at: 2016-11-23T16:15:34.423Z Reads: 464

```
Really interested how good it will handle "higher" current(8-10 Amps)
```

---
## \#21 Posted by: B4Me Posted at: 2016-11-23T16:18:43.318Z Reads: 446

```
How is the current and voltage rating on this connector ?
I mean, its not that nice if it burns the place down :slight_smile: 
due to overheated connectors
```

---
## \#22 Posted by: Maxid Posted at: 2016-11-23T16:21:50.176Z Reads: 454

```
You can't use it for 8-10 Amps - what kind of charger delivers that at 40V anyway?

2A should be fine since you can split it into using two pins (so 1A each). The Apple charger delivers 4A at 20V to fulfill the 80W rating - so the connector must be able to handle at least that.
```

---
## \#23 Posted by: B4Me Posted at: 2016-11-23T16:22:14.549Z Reads: 470

```
This seems like the pogopin used inside the magsafe... its only rated at max 1A :-/

https://ae01.alicdn.com/kf/HTB1wCCJJpXXXXbJXVXXq6xXFXXX4/200160384/HTB1wCCJJpXXXXbJXVXXq6xXFXXX4.jpg?size=45861&height=506&width=504&hash=9f5f8ffc35c2d64c7b423213eecfbc52
```

---
## \#24 Posted by: Maxid Posted at: 2016-11-23T16:23:15.339Z Reads: 452

```
And you have two (total of 4) you can use. Also since the Apple charger is 80W at ~20V it must be able to handle 4A.
```

---
## \#25 Posted by: B4Me Posted at: 2016-11-23T16:27:21.474Z Reads: 438

```
Exactly :)
this will be interresting :)

You could also just make your own , with a little more spacing between poles.. like 10mm in groups of two.. then you dont need to think of water shorting the poles :)
```

---
## \#26 Posted by: flatsp0t Posted at: 2016-11-23T16:29:33.553Z Reads: 433

```
Well, in theory, yes, but for science.
I have got an 8Amp 10s charger and even a 20Amp 12S charger for large packs.

Also, I want to see if it is sparky at higher Voltages.
```

---
## \#27 Posted by: B4Me Posted at: 2016-11-23T16:30:28.482Z Reads: 412

```
You could add a switch before the connector ? no sparks after contact
```

---
## \#28 Posted by: Maxid Posted at: 2016-11-23T16:32:55.818Z Reads: 409

```
I am not going to ride this in the rain. Sure you could make your own magnetic connector - but that is a lot of work and seems unnecessarily complex when you can use already existing parts. No reason to reinvent the wheel.

@flatsp0t could you link me to such a charger? I have never actually seen one.
At 40V you should not see a spark since there are no capacitors between the charger and the battery. So I think it should be fine. It is not like when you connect the VESC to the battery and the capacitors charge themselves.
```

---
## \#29 Posted by: brandon Posted at: 2016-11-23T16:38:54.793Z Reads: 387

```
I guess this only works if you have a bms :( damn balancing wires
```

---
## \#30 Posted by: Maxid Posted at: 2016-11-23T16:40:00.949Z Reads: 379

```
no - I am not going to use a BMS. With quality cells balancing is unnecessary and can be done occasionally (like once a year or something). Look at @whitepony's builds!
```

---
## \#31 Posted by: brandon Posted at: 2016-11-23T16:41:21.823Z Reads: 381

```
So in reality all I need to charge my zippys is the power wires and just occasionally power the cover off and balance them?
```

---
## \#32 Posted by: Maxid Posted at: 2016-11-23T16:42:14.780Z Reads: 380

```
Zippy's are not quality cells. Lipos in general are a different story. I am going to use 18650 cells.
```

---
## \#33 Posted by: B4Me Posted at: 2016-11-23T17:38:37.488Z Reads: 375

```
There should be a spark aswell there.. since a battery is also a capacitor.. but the ISR is higher in them compared to capacitors.. so you may be right about the sparks :)
```

---
## \#34 Posted by: flatsp0t Posted at: 2016-11-23T18:29:56.926Z Reads: 393

```
One From SuPower:
http://www.batterysupports.com/43v-44v-504v-20a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-442.html

They are only usable fo large e-bike or 8p MTB Packs.
```

---
## \#35 Posted by: FredSaberhagen Posted at: 2016-11-23T18:31:03.915Z Reads: 384

```
I think mellow is using something like this!  For waterproof charging
```

---
## \#36 Posted by: Maxid Posted at: 2016-11-28T12:48:24.515Z Reads: 399

```
Ok first heads up:

30V can be delivered (the max of my lab power supply) but the connector gets quite warm (I guess the controller chip is not designed for this type of voltage). Will see how it looks with 41V when my DROK charger is ready. Thickness of the female part (without the unnecessary PCB) is 7mm - so really nice for thin boards as all other plugs usually require much more space. The pins are even angled at 90° already :heart_eyes:

<img src="/uploads/db1493/original/3X/7/b/7b9adffb5a6b07906b4b1f0fdb6e158d6677960c.jpg" width="374" height="500">
```

---
## \#37 Posted by: Maxid Posted at: 2016-12-19T22:12:16.393Z Reads: 386

```
<img src="/uploads/db1493/original/3X/7/6/762587777b98b126baa29063e3fa81edfdabc454.jpg" width="375" height="500"/>
We'll see if that actually works tomorrow
```

---
## \#38 Posted by: sl33py Posted at: 2016-12-19T22:48:40.526Z Reads: 380

```
that is gorgeous!  I too am worried about over-amping those small wires and pcb... keep an eye on it, but so good looking!!!
```

---
## \#39 Posted by: Maxid Posted at: 2016-12-19T22:53:57.610Z Reads: 382

```
They are officially used for up to 4A (Apple 85W charger) - so nothing to worry about.
```

---
## \#40 Posted by: mmaner Posted at: 2016-12-20T02:52:18.747Z Reads: 384

```
I'm not a big fan of hubs, but damn that is so stealth.  I live it.  Awesome work.
```

---
## \#41 Posted by: JuniorPotato93 Posted at: 2016-12-20T05:09:35.317Z Reads: 384

```
@Maxid dude... 
 <img src="/uploads/db1493/original/3X/9/f/9ff74aaae7c4ff93b0539dd1311c1e5bc4f64c02.jpg" width="374" height="500">
```

---
## \#42 Posted by: Maxid Posted at: 2016-12-20T05:23:08.927Z Reads: 381

```
Finally someome noticed ;)
Was really happy when I found out that the switch fits nicely into the truck baseplate on the trucks that came with @jacobbloy's  motors
```

---
## \#43 Posted by: SirDiff Posted at: 2016-12-20T06:56:15.275Z Reads: 372

```
Cleanest look ever
```

---
## \#44 Posted by: Maxid Posted at: 2016-12-20T08:16:05.082Z Reads: 378

```
<img src="/uploads/db1493/original/3X/b/a/baf95caefcc18a7bf128927acff12cfad9d78d7a.jpg" width="375" height="500">Seems to work quite nicely
```

---
## \#45 Posted by: ajaynagra Posted at: 2016-12-20T10:18:53.795Z Reads: 375

```
yooo when i was falling asleep last night i was thinking of that switch idea
```

---
## \#46 Posted by: rwxr Posted at: 2016-12-20T11:22:50.273Z Reads: 372

```
@Maxid: Your magsafe port and the stealthy switch is friggin' awesome! 

Wall hanger charging sounds really sexy.
The problem would be the charging port. It needs to be easily connected without tension and pressure so it's not dependent on which angle you're hanging your board.
I mean the angle could change if your bottom wheels is touching the wall and you change the size of your wheels.
```

---
## \#47 Posted by: kyo Posted at: 2016-12-20T11:57:11.710Z Reads: 375

```
What ab spark? Is that switch antispark?
```

---
## \#48 Posted by: Maxid Posted at: 2016-12-20T11:59:47.307Z Reads: 376

```
there is a vedder anti spark switch inside the board.
<img src="/uploads/db1493/original/3X/d/2/d29e4eb3d73e963f86756611e99fbad3646c8c53.jpg" width="666" height="500">
Tight fit ;)
```

---
## \#49 Posted by: kyo Posted at: 2016-12-20T12:01:21.882Z Reads: 366

```
Kool!!!!!character
```

---
## \#50 Posted by: Eboosted Posted at: 2016-12-21T04:07:49.020Z Reads: 357

```
Can you guys share where you got the magnetic charger?
```

---
## \#51 Posted by: Maxid Posted at: 2016-12-21T06:09:48.983Z Reads: 354

```
The parts can be bought on ebay or aliexpress. Further up I even linked to an aliexpress store.
```

---
## \#52 Posted by: Eboosted Posted at: 2016-12-21T06:29:47.035Z Reads: 351

```
Thanks, how was shipping time on these sellers? Aliexpress usually takes around 40 days to deliver, hope I could find a USA seller on Amazon or eBay
```

---
## \#53 Posted by: Maxid Posted at: 2016-12-21T06:32:33.766Z Reads: 346

```
I bought mine from ebay as a used part from a broken macbook. It took like 2 days. Don't know how long it will take from china.
```

---
## \#54 Posted by: daanstoorvogel Posted at: 2016-12-21T08:15:32.600Z Reads: 345

```
that swicht tho ,Dude i am putting you up with the big boys in my book ! serious creativity
```

---
## \#55 Posted by: Esrapp21 Posted at: 2016-12-21T14:17:43.154Z Reads: 349

```
God damn that's slick!
```

---
## \#56 Posted by: Maxid Posted at: 2017-02-07T08:51:00.293Z Reads: 341

```
<img src="/uploads/db1493/original/3X/5/4/54e97eb96d435b85b59d9a50a91a6d2088e20c95.jpg" width="666" height="500">
```

---
## \#57 Posted by: Okami Posted at: 2017-02-07T09:58:08.739Z Reads: 344

```
<img src="/uploads/db1493/original/3X/5/a/5a4ce01d749078bcb348ea93765d62ea1f77bb17.jpg" width="690" height="387">

Not magsafe but at least will make things a lot easier :D
```

---
## \#58 Posted by: Maxid Posted at: 2017-02-07T10:30:34.421Z Reads: 346

```
Actually it was super easy to setup. Just connected the pins directly with the battery and changed the charger's output cable.
```

---
## \#59 Posted by: Okami Posted at: 2017-02-07T10:42:51.753Z Reads: 342

```
How many amps you gonna push through it? I remember from somewhere on this thread that there was 4 A mentioned. Correct?
```

---
## \#60 Posted by: Maxid Posted at: 2017-02-07T12:33:59.254Z Reads: 338

```
You could theoretically push 4 amps through it - personally my charger doesn't even have that. I charge with 2.5A
```

---
## \#61 Posted by: Pantologist Posted at: 2017-02-07T21:13:54.992Z Reads: 328

```
Just thought this [company](http://cfconn.manufacturer.globalsources.com/si/6008844589336/pdtl/Magnetic-connector/1125010466/Magnetic-DC-male-and-female-connector.htm) had some cool magnetic charging ports and connectors. 

Here's the Mellow [connector](http://rosenberger.de/ok/index.php?caller=search&logic=OR&uorder=number&nprop%5B10%5D=&lookfor=ROPD) for the swappable battery.
```

---
## \#62 Posted by: Surfer Posted at: 2017-02-20T11:57:17.991Z Reads: 327

```
Hi @Maxid, thanks to sharing this awesome idea. I'm in the process to set up my Magsafe charger too, I did with the parts of a old MacBook pro that is lying around. Maybe you or someone else wants to have the small plastic frame to hold it, I have one more available for free, just shipping.<img src="/uploads/db1493/original/3X/7/7/7791349cbe964f85ec94b6839da214a73c743661.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/d/d/ddc0bc374c66ea84c12d502c50a80b4ea6cc08f3.jpg" width="281" height="500">
```

---
## \#63 Posted by: DrM0nsta Posted at: 2017-08-07T16:01:01.786Z Reads: 277

```
I've also thought about doing this for my upcoming build! Nice to know it should work well, I'll be charging at 42V 2A so I should be fine, still within the 85W rating of the Magsafe 2 connector I have. Love the stealth switch you have too, I might have to do something like that for the headlights I plan on having :wink: Awesome build!
```

---
## \#64 Posted by: MaroonArcher Posted at: 2017-10-27T18:41:01.152Z Reads: 253

```
I am making a 14s6p battery for my longboard that's gonna have mountain wheels and dual motor. Would the magnetic charger work for since my battery will have a nominal voltage if 52v and a mac charge of 58v?? I don't mind using the standard plug in charger but I think that the magnetic would be sweet.
```

---
## \#65 Posted by: Maxid Posted at: 2017-10-27T18:55:22.721Z Reads: 243

```
1) what esc are you using with 14S?
2) No idea if it will work - it might but I have too little experience with such a high voltage to confidently say anything.
```

---
## \#66 Posted by: MaroonArcher Posted at: 2017-10-28T18:10:12.860Z Reads: 238

```
I am using a VESC
```

---
## \#67 Posted by: b264 Posted at: 2017-10-28T19:41:13.597Z Reads: 237

```
I would not use the Apple charger unless you know exactly what you are doing.  It sounds compatible from afar... but you'll risk junking your batteries or a big fire or both or worse.  The voltage on the charger would need to be very steady too with the max not fluctuating when the line voltage fluctuates.  I have no idea if apple does that in their charger or in the computer.

VESC is rated at 60V ... if you use 14S on a VESC you will probably have a junked VESC shortly, and will probably get tossed-off in the process.  That's not much wiggle-room
```

---
## \#68 Posted by: Maxid Posted at: 2017-10-28T19:58:54.146Z Reads: 238

```
A VESC is not made for 14S - you sound like you didn't do much research. Especially when dealing with such high voltages you need to know exactly what you are doing.
```

---
## \#69 Posted by: MaroonArcher Posted at: 2017-10-28T20:27:03.800Z Reads: 237

```
I do know what I'm doing. I read everything if you don't believe me here is the spec sheet for the VESC I use. It's torque boards VESC. Max voltage for 14s is 58.8v full charge and nominal is 52v. 

VESC BLDC ELECTRIC SKATEBOARD ESC FEATURES

Built in 5V BEC (Used to power your receiver.)
Voltage: 8V to 60V (Up to 14S LiPo Voltage)
Current: Up to 240A for a few seconds or 50A continous
```

---
## \#70 Posted by: b264 Posted at: 2017-10-28T21:02:15.508Z Reads: 242

```
[quote="MaroonArcher, post:69, topic:13458, full:true"]
I do know what I'm doing. I read everything if you don't believe me here is the spec sheet for the VESC I use. It's torque boards VESC. Max voltage for 14s is 58.8v full charge and nominal is 52v. 

VESC BLDC ELECTRIC SKATEBOARD ESC FEATURES

Built in 5V BEC (Used to power your receiver.)
Voltage: 8V to 60V (Up to 14S LiPo Voltage)
Current: Up to 240A for a few seconds or 50A continous
[/quote]

I understand that, but you're dealing with a reactive load which will feed back voltage into the driver circuit.  The magnetic windings in your motor will certainly pass the 60V mark and besides that, you never, ever, want to run any electronic device at 100% capacity.  50% is the gold standard
```

---
## \#71 Posted by: spannepacker Posted at: 2017-10-31T23:04:59.975Z Reads: 216

```
@Maxid How is the MagSafe connector holding up over time?
```

---
## \#72 Posted by: rok Posted at: 2018-01-11T23:29:43.941Z Reads: 196

```
[quote="Maxid, post:58, topic:13458"]
Just connected the pins directly with the battery and changed the charger's output cable.
[/quote]

Could we run it through BMS? I know that you don't use it but nevertheless for those who do?
```

---
## \#73 Posted by: MrHappy Posted at: 2018-01-11T23:36:43.800Z Reads: 196

```
yes

10chars
```

---
## \#74 Posted by: ivanflo Posted at: 2018-04-18T05:38:41.864Z Reads: 168

```
I’ve just picked up a used MagSafe charging port off eBay. Does anyone have any advice of how best to connect this to my BMS?

In terms of a reliable connection, is it easy to solder these thin wires? Should I solder directly to the bottom of the pcb? Is the little black connector a standard socket I might find at jaycar? 

Thanks,
```

---
## \#75 Posted by: Travo Posted at: 2018-05-23T15:02:29.794Z Reads: 151

```
Hey guys, I'm just researching what to get for my first build and came across this discussion page.  I was just wondering if anyone has a YouTube video or anything of the connections made and if this will work on a 10s battery 42v 2a. Thanks!
```

---
## \#76 Posted by: Maxid Posted at: 2018-05-23T15:24:22.391Z Reads: 151

```
I don't but it's easy. if you really need a video for this type of work you might want to reconsider doing a DIY board in the first place. High voltage batteries are no joke.
As I stated above somewhere the plug is rated for 4A - but the high voltage might release magic smoke from the controller chip. That does not matter however as i think you won't be using the cable to charge your macbook from that point on :D
```

---
## \#77 Posted by: ivanflo Posted at: 2018-05-27T10:24:59.034Z Reads: 139

```
any advice or images on how you soldered charge wires to the port side? i purchased a macbook magsafe port, but the wires coming off the little board are tiny. Should I solder my wires directly to the bottom of the board instead?
```

---
## \#78 Posted by: Maxid Posted at: 2018-05-27T11:09:01.481Z Reads: 128

```
Remove the PCB - you only want the connector itself. There should be 4 pins - you then use like the outer two for POS and the inner two for GND - that way you can flip the plug around and it will charge either way.
```

---
## \#79 Posted by: Travo Posted at: 2019-04-22T21:34:25.930Z Reads: 52

```
I think I'm going to add this magsafe to my board.  Just curious, could i just strip the wires of the 42v 2a power supply I use and wire the positive and negative charger as shown below. Let me know if this all looks correct and if any thing needs to be tweaked :grin: 
Links for the items:
[Magsafe Port](https://www.aliexpress.com/item/1-Piece-5Pin-DC-Power-Socket-Jack-Connector-for-Apple-MacBook-Pro-A1278-A1286-A1287/32947545124.html?spm=a2g0s.8937460.0.0.12a12e0eWBM2N9) -
[Magsafe Cable](https://www.aliexpress.com/item/DC-Cord-Cable-T-Plug-for-Magsafe2-Charger-Apple-Macbook-Pro-Air-45W-60W-85W-Notebook/32976461787.html?spm=a2g0s.8937460.0.0.12a12e0eWBM2N9) -
[BMS I use](https://www.aliexpress.com/item/10S-60A-active-bms-2017-new-Li-ion-smart-bms-pcm-with-android-Bluetooth-app-UART/32827750823.html?spm=a2g0s.9042311.0.0.27424c4deptVMm) -
[Power Brick](https://www.aliexpress.com/item/Wholesale-Balance-Scooter-Battery-Charger-42V-2A-84W-Li-ion-Power-Adapter-Self-Balancing-Scooter-Charger/32810333474.html?spm=a2g0s.9042311.0.0.27424c4dZlKdZH)
![wiring%20mag%20safe|500x500](upload://rar09BTAfkHhpEbQ5kxnf8HfVBj.jpeg)
```

---
