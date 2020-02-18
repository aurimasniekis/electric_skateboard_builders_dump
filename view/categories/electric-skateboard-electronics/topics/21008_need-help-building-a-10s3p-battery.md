# Need help building a 10S3P battery

### Replies: 18 Views: 1341

## \#1 Posted by: tueboard Posted at: 2017-04-14T16:18:34.522Z Reads: 224

```
hi,

i want to build a 10S3P battery for a dual rear drive + 2 VESC, but i'm not sure about all the components, can you help me (i'm from spain, europe)

[30x cells Samsung INR18650-25R 2500mAh - 20A](https://eu.nkon.nl/samsung-18650-inr18650-25r.html)

[DC Jack 5.5 - 2.1](http://www.ebay.es/itm/172617223457?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)

[DC Socket 5.5 - 2.1](http://www.ebay.es/itm/131988840968?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) 

[DC Screw Hat Waterproof 5.5 - 2.1](http://www.ebay.es/itm/132019062633?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT)

[power switch](http://www.ebay.es/itm/SmartSwitch-12V-24V-18mm-IP67-Steel-LED-Illuminated-ON-OFF-POWER-Button-Switch-/142264810878?var=&hash=item211fa4bd7e:m:mf8-GLW1A4yZn1Lhe1Swh_w)

[12 awg cable](http://www.ebay.es/itm/12-AWG-3m-Escala-Cable-De-Silicona-Flexible-Trenzado-Cobre-Cables-/112354435387?hash=item1a28d8a13b:g:fCsAAOSwxKtYBcj7)

[battery indicator](http://www.ebay.com/itm/2016-Battery-Capacity-Tester-Indicator-for-12V-24v-36v-48v-CAR-Lead-acid-lithium-/172143986261?hash=item281494c655)

[nickel strips](https://es.aliexpress.com/store/product/100pcs-lot-0-15mm-x-7mm-x-100mm-Quality-low-resistance-99-96-pure-nickel-Strip/1758634_32333149144.html)

any of those chargers are valid? or can you recommend me another one? 

[charger 4A](https://es.aliexpress.com/store/product/High-Quality-36V-42V-4A-Li-ion-Battery-Charger-E-bike-fast-charger-Aluminum-housing-charger/313864_422328869.html)

[charger 2.5A](https://es.aliexpress.com/store/product/36V-42V-2-0-2-5A-Lithium-Battery-Charger-High-quality-E-bike-charger/313864_455606765.html)


any of those bms are valid? or can you recommend me another one?

[bms 1](http://www.ebay.com/itm/221769582503)

[bms 2](https://es.aliexpress.com/store/product/36V-2000W-Lithium-Battery-BMS-PCB-10S-42V-Electric-Bicycle-Battery-BMS-60A-continuous-120A-peak/1263529_32459655141.html)

**some questions...**

1- why some people prefer to use the bms only for charge but no for discharge ? the cells can unbalance easier if you do that, right?

2- can someone provide me a 10S3P battery Scheme picture or tutorial?

3- it's bad for the battery lifespan to charge at 4A?

4- for this kind of battery is better to use a power switch or a xt60-xt90 anti-spark?

5- the DC jack size or type can influence in the charging thime?

6- which is the avg range and charging time of 10S3P?

thank you
```

---
## \#2 Posted by: TranxFu Posted at: 2017-04-14T16:40:18.765Z Reads: 206

```
-Maybe get 30Q cells for a slightly higher price. 25R cells are proven to not be that efficient overall. 
-Better get the DC plugs/jacks with 2.5mm. 
https://www.amazon.de/Stück-DC-Einbaubuchse-Stift-metallausf-Lötfahnen/dp/B00CI6ISMG/ref=sr_1_5?ie=UTF8&qid=1492187661&sr=8-5&keywords=Hohlstecker+buchse

-Switch is your preference.
-Chargers are both good. I'd prefer a regulating one so you can tune it down to approx. 41v. It preserves the life of the cells.
-Dont know about BMS since me and a lot of other experienced members don't use one with quality 18650s



----------


1- first, it is cheaper if you get an low amp BMS. Second, the VESC has discharge and undercurrent protection.

2- Look up 10s3p/10s4p diagrams in the search function :) or even google.

3- At 10s3p, 4A is good to go. I'd not go above. I'd rather go below.

4- Preference. I'd go with a power switch + fuse. I don't know how to wire an LED Button in when using XT60,90

5- Connections/plugs/chargers that can handle higher amps might be better. But I don't think it matters at 2-4A. They might not get hot/warm that fast.
```

---
## \#3 Posted by: OskarCastrone Posted at: 2017-04-14T17:28:00.622Z Reads: 187

```
Hi

I think @TranxFu have answered your questions very well.  

About the charging port; I think you can go ahead and safely use the one you have linked to in your post. I dont know have many amps it is rated for, but I dont think it is going to be a problem. 

I am using [these guys](http://www.ebay.com/itm/5pcs-Waterproof-5-5-x2-1mm-DC-Socket-Power-Jack-Plug-Female-Mount-Connector-CATB-/351632441235?hash=item51deed3f93:g:G2QAAOSw1S9WhAD0) and they have been working great. I sometimes charge the battery with my 5.5a charger, which also works fine with this charging port. It gets a little bit warm but not hot at all. 

About the BMS; I would definitely advise you to buy a BMS from Bestech. You have to order at least 2 per order, but they are great and reliable. They also offer a BMS with a build in power switch. Therefore you wont have to buy an additional power switch! 

I am willing to assemble the whole setup if you like. I have a spot welder and everything. I can make the pack exactly as you like it. I can also solder on a display, charging port etc. 
It is just an offer. I am still here to help if you want to build the pack yourself :-)
```

---
## \#4 Posted by: PXSS Posted at: 2017-04-14T17:56:33.435Z Reads: 172

```
[quote="tueboard, post:1, topic:21008"]
1- why some people prefer to use the bms only for charge but no for discharge ? the cells can unbalance easier if you do that, right?
[/quote]
Yes, it is easier for cells to go out of balance and get damaged that way. I recommend you get a BMS you can use while discharging too in order to protect your pack.

[quote="TranxFu, post:2, topic:21008"]
it is cheaper if you get an low amp BMS. Second, the VESC has discharge and undercurrent protection.
[/quote]

The discharge protection will protect the battery from discharging below a voltage. If the cells are out of balance, it won't prevent from individual cells going below 2.5v and potentially to 0v. For example, @Eboosted's setup.


  [quote="tueboard, post:1, topic:21008"]
2- can someone provide me a 10S3P battery Scheme picture or tutorial?
[/quote]
search function


[quote="tueboard, post:1, topic:21008"]
3- it's bad for the battery lifespan to charge at 4A?
[/quote]

4A is fine, look up the spec sheet for the cell youre using.


[quote="tueboard, post:1, topic:21008"]
5- the DC jack size or type can influence in the charging thime?
[/quote]

A tiny tiny bit. the less resistance they have, the less heat you will generate and the less energy you will waste. But we're talking tiny tiny tiny amounts.


[quote="tueboard, post:1, topic:21008"]
6- which is the avg range and charging time of 10S3P?
[/quote]

Depends on the cells you use. 25Rs are meh.
```

---
## \#5 Posted by: tueboard Posted at: 2017-04-14T18:54:03.268Z Reads: 149

```
first of all thank you all for your answers!

@PXSS if you discharge the battery by bms, you must to disable the vesc cutoff?

@TranxFu regulating charger is a balance charger?

@OskarCastrone do you prefer this one? thanks for your help but i want to build by myself :)
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#6 Posted by: PXSS Posted at: 2017-04-14T18:56:06.801Z Reads: 147

```
[quote="tueboard, post:5, topic:21008"]
if you discharge the battery by bms, you must to disable the vesc cutoff?
[/quote]

No. They add up. Which is good since you have two safeties. The first when your ESC reaches it's cutoff and if that fails, your BMS.
```

---
## \#7 Posted by: OskarCastrone Posted at: 2017-04-14T19:11:30.526Z Reads: 145

```
Yep, that is the BMS I use. 
You can also get this BMS with a 60a discharge if you ask them :slight_smile:
A good tip is to remove the screws in the corners and fold it open. In that way the BMS gets a lot thinner.
```

---
## \#8 Posted by: tueboard Posted at: 2017-04-14T21:00:50.716Z Reads: 138

```
@PXSS which 18650 cells do you recommend? LG HG2? other? and why? thanks
```

---
## \#9 Posted by: PXSS Posted at: 2017-04-14T21:13:58.134Z Reads: 144

```
30Q
More capacity = Higher Range
Less Internal resistance = Less heat, less wasted energy (more range), more power. 
Not that expensive. 

25R/HG2 are old cells. They were good back in 2014... 30Q got released a year later and is a better cell overall
```

---
## \#10 Posted by: tueboard Posted at: 2017-04-24T23:45:03.946Z Reads: 130

```
This socket is ok?  It looks very small 

<img src="/uploads/db1493/original/3X/a/4/a451268ae4a81a900b821691dab2bc56bec656f8.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/c/c/cc5aa893008971025fbc790ef6442e10468a18ed.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/6/d/6dd822970dab7257a27056b03b3ab3cb8d00eff1.jpg" width="375" height="500">
```

---
## \#11 Posted by: mmaner Posted at: 2017-04-25T13:53:27.045Z Reads: 110

```
Thats the same one I use.
```

---
## \#12 Posted by: Okami Posted at: 2017-04-25T14:18:47.053Z Reads: 108

```
@mmaner  At how much amps do you charge?

These legs do look tiny.. Though it might be okay for 5amps but im not good for these kind of things to calculate max amps per metal surface/part
```

---
## \#13 Posted by: mmaner Posted at: 2017-04-25T14:20:06.600Z Reads: 107

```
I charge at 2 amps, all of my 10s chargers are only 2 amps.
```

---
## \#14 Posted by: Okami Posted at: 2017-04-25T14:21:11.893Z Reads: 106

```
@mmaner  yeh, 2amps are okay I think, cell phone chargers also doenst have very big metal surface but they stilll manage 1-2A
```

---
## \#15 Posted by: tueboard Posted at: 2017-04-25T14:25:48.202Z Reads: 101

```
@mmaner @okami thanks for the reply, it's 2.5mm dc socket and i've a 4A charger
```

---
## \#16 Posted by: Okami Posted at: 2017-04-25T14:29:33.932Z Reads: 103

```
@tueboard yeh I think some time ago when I looked into this, the max they were rated at was 5A

Probably the best way to check is to see wheneve it gets warm or not.. though at 4A it might be okay, 10A probably wouldnt bet that good.. 

but as said earlier, im not really having much experience, only what Ive seen on videos and just some general sense on what seems logical to be used for such currents
```

---
## \#17 Posted by: tueboard Posted at: 2017-05-05T21:33:21.164Z Reads: 97

```
So i got all this stuff
<img src="/uploads/db1493/original/3X/c/f/cf056f12ea23f79e8dcc4c0b4844f222c754b054.jpg" width="666" height="500">

And some questions too :slight_smile: 

1- Do you think that this nickel strip can work or its too small (0.15mm x 7mm)? How many layers i need?
<img src="/uploads/db1493/original/3X/9/3/93feea5fcba0cdc66154dcc340a228021962a43e.jpg" width="375" height="500">

2- do you think that i need washers to cover each 30Q battery positive end?
<img src="/uploads/db1493/original/3X/7/d/7dfcafb3bbff0a349a7cec76fa8848776329efa0.jpg" width="375" height="500">

Thanks
```

---
## \#18 Posted by: PXSS Posted at: 2017-05-05T23:44:30.511Z Reads: 91

```
Definitely on the washers if you've never done this before. Samsungs have the casing at the same height as the positive and their protection is easy to melt through.
```

---
