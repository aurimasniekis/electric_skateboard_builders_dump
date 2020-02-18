# Custom li-ion pack ( turned out to be DIY spot-welder thread )

### Replies: 37 Views: 5012

## \#1 Posted by: IDVert3X Posted at: 2017-01-02T21:59:53.240Z Reads: 337

```
This topic was originally an request for custom buttery, it turned out to be DIY spot welder thread.
You can view the original version of this post by opening the history.

Now back to the DIY spot welder.

I've designed a hardware and written the firmware for custom battery spot welder project.
It's cheap, compact and gets the job done.

Schematic & PCB: https://easyeda.com/IDVert3X/MCU_controller_battery_spot_welder-b4ce75a4247b46baa9769568644e7ec7
Firmware: https://github.com/IDVert3X/TinySpotWelder

PCB design:

<img src="/uploads/db1493/original/3X/e/a/eafae539cfdb2cbc931afee40b3bda141f021aaa.png" width="405" height="500">

Right now, I have a working prototype on breadboard ( logic part ) & perfboard ( mosfets ).
I'm planning to switch to the PCB I designed soon.
```

---
## \#2 Posted by: Maxid Posted at: 2017-01-02T22:05:10.684Z Reads: 312

```
Shipping for dangerous goods will probably still be killer even inside of EU. You should make yourself a DIY Spotwelder and literally do it yourself.
```

---
## \#3 Posted by: ninja Posted at: 2017-01-02T22:47:36.183Z Reads: 300

```
This guy will do it and ship it, no problem :wink:

atomek1000@gmail.com

and you can use his calculator to now how much it will be! :

  http://users.pja.edu.pl/~s12888/batterycalc/
```

---
## \#4 Posted by: IDVert3X Posted at: 2017-01-02T23:00:18.862Z Reads: 290

```
Thank you very much for your helpful response.
```

---
## \#5 Posted by: ninja Posted at: 2017-01-02T23:01:44.056Z Reads: 271

```
You are welcome :smile:
```

---
## \#6 Posted by: Maxid Posted at: 2017-01-03T00:17:36.284Z Reads: 265

```
@IDVert3X

a 10S4P battery costs ~280€ with that guy.

40 25Rs from nkon.nl cost 131€ shipped to slovakia.
A DIY spot welder costs a maximum of 50€.

That would be 100€ cheaper than having it made plus you would have a spot welder for any additional builds in the future.
```

---
## \#7 Posted by: PXSS Posted at: 2017-01-03T00:50:44.766Z Reads: 246

```
Dont forget wires, nickel tabs, connectors. It can easily add up. I made that mistake lol
```

---
## \#8 Posted by: aigenic Posted at: 2017-01-03T05:34:30.319Z Reads: 238

```
Je hezké tu vidět aspoň někoho ze Slovenska :)
```

---
## \#9 Posted by: IDVert3X Posted at: 2017-01-03T08:37:26.989Z Reads: 251

```
[quote="Maxid, post:6, topic:15549"]
A DIY spot welder costs a maximum of 50€.
[/quote]

Even the transformer would be more expensive than 50 euros :smiley:
And then all the other parts, hours of work... yeah, not really worth it.
Also, I don't like doing things cheap-ass way, just so it works.
If I make something, it has to be reliable, safe and reasonable quality.

And no, DIY is not always going to be cheaper. That's a false economy.
Sunko 709A looks like a good option for low-cost spot-welder. 
I can have it for 220€ shipped, but then... yeah. Already over 300 euros :)
I will also have to buy those nickel strips ( hard to find 0.3mm ) and so on.
Gonna do some math and look for exact numbers.
If the complete is 300 euros a DIY 350, it might be worth to spend 50 euros more and have spot welder.

[quote="aigenic, post:8, topic:15549"]
Je hezké tu vidět aspoň někoho ze Slovenska :slight_smile:
[/quote]

Šikovné československé ručičky sa nájdu všade :)
```

---
## \#10 Posted by: Maxid Posted at: 2017-01-03T08:41:42.562Z Reads: 240

```
You don't know the Arduino Spot welder?
It works with a 12V car battery - no need for a transformer. The parts are like 20€ plus some for the PCB if you want to make it right.
There is no magic to do it right. My calculation was correct - I just built myself a 10S3P custom pack the same way.
You also can buy the nickel strips from nkon - tgey are not 0.3 but 0.15 if I remember correctly but you can always just add layers with the spot welder. Personally I soldered copper wire on top of the welded strips.
```

---
## \#11 Posted by: IDVert3X Posted at: 2017-01-03T08:51:50.091Z Reads: 236

```
Car battery is heavy and expensive thing ( 40+ eur, already over your 20 euros ).
The charger for car battery is also not free.
Then you have to get a pedal, also not cheap if you want it to be reasonable quality.
I have a lot of wires at home, so that's not an issue.
Then there is MCU, which is like $1 or like $3 for the Arduino Nano.
Electrodes ( huge copper pieces ), that are expensive ( at least where I live )
I can make PCBs at home, that's not an issue for me, it's almost free...
Then you need mosfets and other crap.
And even after that, it's not even as good as a premade one.
```

---
## \#12 Posted by: Maxid Posted at: 2017-01-03T09:01:58.014Z Reads: 224

```
What? You don't have a car battery at home? You can literally use the one from a car. You don't need a charger when you use a car battery. As electrodes you can simply use some 16sqmm copper wire - that should be easy to source. The Mosfets and diodes and stuff are ~20€. You can use any switch - I used a microswitch attached to the electrodes so I can trigger it with my finger: 2€.
And according to the guys at endless sphere this DIY spot welder is better than 2000USD spot welders and can even be used to spot weld pure copper!
```

---
## \#13 Posted by: Charster10 Posted at: 2017-01-03T09:05:21.951Z Reads: 214

```
Id go the diy route here...
```

---
## \#14 Posted by: IDVert3X Posted at: 2017-01-03T09:28:29.260Z Reads: 218

```
I don't have a car :smiley: No need for it right now. 
Driving license is still on TODO list too :D

But from what you guys say, I might consider making a spot welder after all...
```

---
## \#15 Posted by: Maxid Posted at: 2017-01-03T09:30:05.857Z Reads: 212

```
but someone in your family should have one no? I don't have my own car as well and just used the girlfriend's for an hour.
She wasn't too happy but as long as the car works afterwards it's fine :smiley:
```

---
## \#16 Posted by: okp Posted at: 2017-01-03T09:38:02.258Z Reads: 215

```
go DIY especially because you'll be proud of what you'll achieve !
```

---
## \#17 Posted by: IDVert3X Posted at: 2017-01-03T09:49:03.038Z Reads: 225

```
@Maxid
Yes, but noone will allow me to use their battery ( they think I'm gonna destroy it, lol ).
The battery is ~40 euros, cheapest charger is like ~30 euros.
There in Slovakia ( and Czech republic as well ) salaries suck compared to the rest of the world, but 60 euros for battery and charger really won't kill my me :D And I may recycle it in another project, so... :D

@unikboards
That's why I do most of the stuff DIY :D
But sometimes it really isn't worth it.
```

---
## \#18 Posted by: okp Posted at: 2017-01-03T09:55:54.521Z Reads: 220

```
yeah ! fully agree. Great thing about what we are all doing is that it develops our creatitivy and commitment. I would say that DIY is a metaphor for life ! 

the skills that we learn, develop are really applicable in our day to day activities. never ever give up !
```

---
## \#19 Posted by: IDVert3X Posted at: 2017-01-03T09:56:54.766Z Reads: 223

```
It's a lifestyle!
```

---
## \#20 Posted by: rwxr Posted at: 2017-01-03T10:28:22.592Z Reads: 219

```
Pre-built arduino welders are available from here now:

https://www.tindie.com/products/KaeptnBalu/diy-arduino-battery-spot-welder-prebuilt-kit/

All sold out but new ones will arrive around january 14th.
```

---
## \#21 Posted by: Maxid Posted at: 2017-01-03T10:32:02.530Z Reads: 205

```
With all the electronics you work with you surely have a lab power supply no? You can use that to charge the car battery. Also why not use one of your family's batteries and tell them that you buy them a new one if you destroy the original - which you will not have to do anyway.
```

---
## \#22 Posted by: IDVert3X Posted at: 2017-01-03T11:38:45.637Z Reads: 213

```
[quote="Maxid, post:21, topic:15549"]
With all the electronics you work with you surely have a lab power supply no?
[/quote]

Sure I do, it's a DIY MCU-controlled with quite a few useful functions...

[quote="Maxid, post:21, topic:15549"]
You can use that to charge the car battery.
[/quote]

...but I havn't implemented battery charging alghoritms. I could do that, but then... yeah, I'm lazy.
The firmware is already a mess ( I was learning C when I was coding it, it was one of my first projects that used microcontroller )  and I would have to rewrite the whole code for the device that I'm going to replace with the new, better one I'm working on for 7 months ( yes, I'm really, really lazy ) anyway... I will probably implement this in my new lab bench power supply once its finished, but that's going to take quite a while as it's not my priority right now.

And charging it manually ( aka watching if it's charged and disconnect it ) is not something I can afford to do.
Proper car battery charger is something I should have anyway.

[quote="Maxid, post:21, topic:15549"]
Also why not use one of your family's batteries and tell them that you buy them a new one if you destroy the original - which you will not have to do anyway.
[/quote]

Already tried, I was told to buy a new one and use it.
In the end, I might end up using the car battery for multiple projects so let's just buy one :)

---

Anyway, thanks for your help and advices, I appreciate you're trying to help!
```

---
## \#23 Posted by: IDVert3X Posted at: 2017-01-03T21:04:07.717Z Reads: 200

```
So, I was able to get an old car battery for free from my friend - hopefully it will do the job.
I also bought 4A car battery charger for 25 euros.
And finally, 40 Samsung 25R cells + some nickel strips from nkon.nl ( they really have great prices! ).

The pre-built welder @rwxr mentioned looks nice, but it's not available.
So I'm going to design my own as a plan B.

Will keep you updated :)
```

---
## \#24 Posted by: Eboosted Posted at: 2017-01-04T00:24:14.869Z Reads: 197

```
I'm going to this route.

https://www.youtube.com/watch?v=Gk3vrKc4Y1w&t=126s

But adding a push button like this guy

https://www.youtube.com/watch?v=UU7QC5Uby6M&t=2s

Easiest and most affordable spot welder ever
```

---
## \#25 Posted by: IDVert3X Posted at: 2017-01-04T10:42:27.809Z Reads: 193

```
Geez, just saw the first video....

No timing circuit
Too thin wires ( you should use 16mm2 or more )
Welding electrodes in a WOOD?

Geeez. Just... woooow. That's so bad...
Who on the Earth would do it like that? That's insane.

And the result? Those welds are terrible!
He is literally making holes in the nickel strip.
Geeeeeeez.
```

---
## \#26 Posted by: laikiux Posted at: 2017-01-04T11:02:08.324Z Reads: 196

```
I have designed simple spot welder. It uses arduino nano for timing, and solid state relay to activate the primary winding of the transformer.
<img src="/uploads/db1493/original/3X/8/e/8eae5db45a869026d3061f04ff705e6a84b0d76a.png" width="690" height="379">
<img src="/uploads/db1493/original/3X/e/e/ee4d7eae6b5d35496fc6fcf7fc2198bfe1b3a53c.JPG" width="669" height="499">
<img src="/uploads/db1493/original/3X/2/b/2b418990d7b6f9dc8bb79a8db9a05c521d3de09a.JPG" width="669" height="499">
```

---
## \#28 Posted by: IDVert3X Posted at: 2017-01-07T18:49:58.908Z Reads: 164

```
So, I finished the design, this time actually in a CAD.
I changed my mind and instead of using mini oled display, I'm gonna stick with 7 segment.
It draws much more current than the OLED display, but after some testing, I know 7805 can still handle it.
It will also make my life easier during the programming part of the development.

Missing components are ordered ( I already had most of the components at home ).

There is the schematic:

<img src="/uploads/db1493/original/3X/6/0/60ca630041671ff0f297979000c1110feb35e056.png" width="443" height="500">

I'm still not sure if I'm going to make a PCB for the whole thing or keep it simple and make a PCB just for the power switching part while keeping the logic part on the breadboard. Hmm... I'm gonna think about it once I start to design the PCB ( probably tomorrow ).
```

---
## \#29 Posted by: Eboosted Posted at: 2017-01-07T23:06:26.174Z Reads: 152

```
For some mortals as us, these diagrams are pretty difficult to follow. So, I'll stick with lead acid spot welding method shown on the previous youtube video, not the first but the last one.
```

---
## \#30 Posted by: IDVert3X Posted at: 2017-01-07T23:14:16.386Z Reads: 150

```
It's actually very simple diagram!
You have an programmed microcontroller ( I will open source the firmware as well ), that reacts to 2 inputs: button and pedal. Then, there is a shift register, which stores data about which segments of the display are active and also the one that enables the transistors that enables mosfets which then just create a path for the welding current. Then there is just a 5V linear regulator ( 7805, no reason to use buck converter there ) and a few passive components. Once I make it, I will post some pictures so you ( and others ) can see how simple it actually is!
```

---
## \#33 Posted by: Maxid Posted at: 2017-01-15T09:09:34.146Z Reads: 135

```
Did you also account for the TVS and Schottky Diode that are recommended to use with this type of spot welder?
```

---
## \#34 Posted by: IDVert3X Posted at: 2017-01-15T11:06:48.657Z Reads: 135

```
No need for them as there is no inductive load and input is a car battery ( 12V, will drop during weld ).
```

---
## \#35 Posted by: Maxid Posted at: 2017-01-15T11:09:26.053Z Reads: 132

```
Did you read the endless sphere topics about the arduino spot welder? There is quite a lot of avalanche current with a 12V battery.
https://endless-sphere.com/forums/viewtopic.php?f=14&t=83411
https://endless-sphere.com/forums/viewtopic.php?f=14&t=81400&start=550#p1218325
```

---
## \#36 Posted by: IDVert3X Posted at: 2017-01-15T11:52:20.255Z Reads: 128

```
I did not until now, but looks like they tested it in real world and found use for the diodes. From my calculations, the inductance should not be high enough to cause such a problems, also my real world tests on a prototype showed no problems, but okay, I will add these diodes just to be on a safe side.

I'm also going to improve the mosfet switching stage to something that can supply higher currents, because I found out that the mosfet switch time is too long.

Another problem I came up is the capacitance. 5V rail is super stable ( it has to be with 100u cap ), but the 12V rail falls before the mosfets get fully switched on. I will add high capacity capacitor to the new mosfet switching stage to keep the 12V rail stable enough during the weld.

I will implement all the changes soon.
```

---
## \#37 Posted by: IDVert3X Posted at: 2017-01-15T16:01:47.717Z Reads: 128

```
Just a quick update.

I have hard time looking for the diodes. Mostly because of "Stock level: 0 pcs" which is driving me crazy. Even if I find something that suits my needs, it's not in stock. I may look for it somewhere else, but ordering components from multiple distributors that I have no experience with is not really something I want.

List of [available schottky diodes](http://www.tme.eu/en/katalog/#id_category=112797&page=1&s_field=artykul&s_order=ASC&products_with_stock=on) on TME.eu
And the same for [transil diodes](http://www.tme.eu/en/katalog/#id_category=112804&page=1&s_field=artykul&s_order=ASC&products_with_stock=on).

Once I filter them, there is no diode in stock that would suit this project :/ .
Any advice? Maybe I will just ignore the diodes.

By the way, I was able to find some mosfet drivers and they are quite cheap.
Two of [these](http://www.tme.eu/en/details/ixdd604pi/drivers-integrated-circuits/ixys/) 4A 2-channels should get the job done.

I still need to source better electrodes somewhere.
Right now, I'm using 2.5mm2 solid core copper wire, I was unable to source anything thicker. It works, but it's not that great... 10mm2 solid core would be much better. I visited 7 ( !!! ) local electronics stores and none of them had anything bigger than 2.5mm2 so that might be hard to source as well.
```

---
## \#38 Posted by: Maxid Posted at: 2017-01-17T13:25:35.411Z Reads: 120

```
There are diodes in stock. The recommended ones are:
https://endless-sphere.com/forums/viewtopic.php?f=14&t=81400&start=550#p1219916

and TME.eu has for example:
http://www.tme.eu/de/details/5kp14a-dio/transil-einwegdioden-tht/diotec-semiconductor/5kp14a/
http://www.tme.eu/de/details/mbr4045pt-e3_45/universaldioden-tht/vishay/

the original design uses these mosfet drivers:
http://www.tme.eu/en/details/mcp14e10-e_p/mosfetigbt-drivers/microchip-technology/
```

---
## \#40 Posted by: usual Posted at: 2017-04-14T21:03:15.950Z Reads: 101

```
What about the other method?
```

---
## \#41 Posted by: Eboosted Posted at: 2017-04-20T05:26:09.807Z Reads: 85

```
So I got my arduino spot welder last week and today I made some welds, boy this thing is amazing, after soldering my last pack with a soldering iron, this thing simplify everything, it is really fast. 

<img src="/uploads/db1493/original/3X/7/3/739d07fd139e95872f00f46a1315c13cddb1b2ac.jpg" width="666" height="500">
```

---
