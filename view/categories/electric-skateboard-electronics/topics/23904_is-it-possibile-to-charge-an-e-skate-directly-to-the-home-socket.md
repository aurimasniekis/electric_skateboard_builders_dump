# Is it possibile to charge an e-skate directly to the home socket?

### Replies: 90 Views: 4525

## \#1 Posted by: edoardo Posted at: 2017-05-25T21:19:05.365Z Reads: 340

```
Some factory-made electric skateboard can be charged directly from the power plug of our home ( EU in my case ).
Instead I have to take Lipo battery from the longboard and charge it with the Imax b6 charger ( or others ).

There's a way to avoid this intermediate steps and connect "power cable" from the e-skate directly into home socket?
```

---
## \#2 Posted by: Okami Posted at: 2017-05-25T21:31:01.642Z Reads: 328

```
yes, if you integrate the charger on your eboard.. or have 230v battery lol

People usually integrate Bms module (battery protection circuit) so that they can charge with just one plug, not 2 - balance cable + main plug (+ / - )

A way more clever charging would be with induction (wireless) but right now the technology is not really there yet.. so it would probably be waay expensive to do this way, it would still take a lot of time and heat would be involved (wouldnt be that good for batteries, if directly translated to them)

--

I think it is possible to order some similar modules as b6, they are smaller and just more 'dumb', meaning you wont get a lot of customization, but you could easily install them on eboard and just plug in the mains cord into them, so they can do their work and convert the voltage/charge the batteries.
```

---
## \#3 Posted by: edoardo Posted at: 2017-05-25T22:39:47.077Z Reads: 301

```
[quote="Okami, post:2, topic:23904"]
People usually integrate Bms module (battery protection circuit) so that they can charge with just one plug, not 2 - balance cable + main plug (+ / - )
[/quote]

Anyway they have to charge the board ( with only 1 cable ) with a charger like Imax, right?
```

---
## \#4 Posted by: Jebe Posted at: 2017-05-25T22:42:40.349Z Reads: 280

```
nope - use a 36volt laptop style charger - it converts your domestic voltage to the voltage of your battery.
The on board battery BMS (battery monitoring system, aka battery murdering system) monitors the individual cells and keeps them balanced.
```

---
## \#5 Posted by: Jebe Posted at: 2017-05-25T22:44:57.513Z Reads: 279

```
something like this
http://www.ebay.com.au/itm/Electric-Skateboard-36-Volt-Universal-Battery-Charger-/112019530457?hash=item1a14e262d9:m:mrGwBevauUxlCX6-gXBqx3Q

there are definitely cheaper ones than this and you have to select according to your cell type.
```

---
## \#6 Posted by: edoardo Posted at: 2017-05-25T22:49:04.533Z Reads: 266

```
Is it possibile to make all of that with my Turnigy Lipo 6s1p ? 

If it's so I have to:
- cut the balance plug of my battery
- properly solder each cable in a BMS module 
- properly solder "+" and "-" plug
- get output (?) 
- and charge with a 22.2v laptop style charger? 

Thank you and sorry for the doubts but I'm a beginner! :sweat_smile:
```

---
## \#7 Posted by: Jebe Posted at: 2017-05-25T22:55:45.429Z Reads: 250

```
I don't know sorry - I don't use lipos.
I think it's been done - try the search function.
If you cut the enclosure to fit the lipo bms cable you could connect the imax bms connections straight to it and not have to remove it from the enclosure.
Search bud, I think @dunkirk did this on his vanguard build.
```

---
## \#8 Posted by: edoardo Posted at: 2017-05-25T22:57:36.756Z Reads: 233

```
That's more simple with a custom battery pack right?
```

---
## \#9 Posted by: Jebe Posted at: 2017-05-25T22:58:20.010Z Reads: 234

```
yes but making the custom pack isn't ! :stuck_out_tongue:
```

---
## \#10 Posted by: edoardo Posted at: 2017-05-25T23:06:45.778Z Reads: 226

```
This could be fine? 
http://www.ebay.it/itm/6S-15A-BMS-Protection-PCB-Board-For-6-Packs-Li-ion-Lithium-18650-Battery-Cells-/122466464950?hash=item1c8391f4b6:g:UIIAAOSw3u1ZAZXb

Which plug end can I use? ( I come from EU )
```

---
## \#11 Posted by: sayreul Posted at: 2017-05-25T23:07:07.646Z Reads: 219

```
Yes 
You can do this with your lipo 

You can use à BMS just to control charge / or to control charge and discharge
```

---
## \#12 Posted by: sayreul Posted at: 2017-05-25T23:08:22.938Z Reads: 211

```
If you buy this BMS (15A) you can only use for charge 
You need at leat 60a BMS for discharge
```

---
## \#13 Posted by: edoardo Posted at: 2017-05-25T23:08:33.549Z Reads: 201

```
Good to know! Have you already done it?
```

---
## \#14 Posted by: edoardo Posted at: 2017-05-25T23:10:57.366Z Reads: 217

```
This ? 
http://www.ebay.it/itm/6s-24v-Li-ion-Lithium-Cell-60A-18650-Battery-Protection-BMS-PCM-Board-w-Balance-/282140999613?hash=item41b0e9ffbd:g:fFwAAOSwMtxXtY3K
```

---
## \#15 Posted by: Okami Posted at: 2017-05-26T00:00:19.319Z Reads: 209

```
There's also this solution:

https://www.electric-skateboard.builders/t/miami-electric-boards-diy-charger-how-to/4242

Though I wouldnt recommend if you havent soldered small wires before, it can be a bit messy and you need to make 100% sure you solder the right wires to the right pins.

--

As for the bms, from text it looks it might be okay but maybe wait till someone else jumps in.

@Namasaki will probably tell you that getting ebay bms modules is not great idea.. but ok they might work, if you monitor the actual state of your batteries once in a while ( I think)
```

---
## \#16 Posted by: Namasaki Posted at: 2017-05-26T01:24:28.339Z Reads: 198

```
[quote="Okami, post:15, topic:23904"]
@Namasaki will probably tell you that getting ebay bms modules is not great idea.. but ok they might work, if you monitor the actual state of your batteries once in a while ( I think)
[/quote]


You are absolutely correct @Okami
I would never recommend  using a cheap bms from eBay or any other supplier.
Especially to someone who has invested a lot of money and time building a Li-ion battery pack.
I just can't see risking an expensive battery pack to save a couple bucks on the bms.
```

---
## \#17 Posted by: Hummie Posted at: 2017-05-26T02:13:22.362Z Reads: 189

```
Or just get a laptop style charger (some can be really fast high power) and a 10$ discharge balancer and be done.
```

---
## \#18 Posted by: edoardo Posted at: 2017-05-26T07:16:01.338Z Reads: 179

```
[quote="Namasaki, post:16, topic:23904"]
You are absolutely correct @OkamiI would never recommend  using a cheap bms from eBay or any other supplier.Especially to someone who has invested a lot of money and time building a Li-ion battery pack.I just can't see risking an expensive battery pack to save a couple bucks on the bms.
[/quote]

Where you recommend to buy a BMS?

Which plug end of the e-skate can I use? ( I come from EU )
```

---
## \#19 Posted by: sayreul Posted at: 2017-05-26T08:07:58.321Z Reads: 173

```
you can buy a good BMS here 
http://www.batterysupports.com

<30A for charge only, 60A for charge and discharge (the BMS help you to protect your lipo during discharge (cut of) )

you will need to buy a "laptop style" charger but you can use any connector for charge (DC 2.1 5.5 is very common)

you can also change the cable with socket plug to adapt to your country
```

---
## \#20 Posted by: edoardo Posted at: 2017-05-26T09:01:10.904Z Reads: 168

```
Which good waterproof connector can I choose?
```

---
## \#21 Posted by: edoardo Posted at: 2017-05-26T09:23:38.102Z Reads: 158

```
I was thinking... 
Can I bought this https://goo.gl/w6zvIY to only charge battery and discharge it with my Imax B6 ? 

ps: Why and when I need to discharge battery? :sweat:
```

---
## \#22 Posted by: sayreul Posted at: 2017-05-26T09:49:36.578Z Reads: 160

```
discharge is when you use your eskate 
your BMS can control the discharge to check and avoid battery cells to go under 3.3v

the vesc do the same  - so you can use your BMS to control only charge 

but it is better to avoid cheap BMS if you want a good balance charge of your cells
```

---
## \#23 Posted by: edoardo Posted at: 2017-05-26T09:54:19.038Z Reads: 158

```
[quote="sayreul, post:22, topic:23904"]
the vesc do the same  - so you can use your BMS to control only charge
[/quote]
I doesn't have VESC, I've a ESC X-car beast 120A , do it the same?

[quote="sayreul, post:22, topic:23904"]
but it is better to avoid cheap BMS if you want a good balance charge of your cells
[/quote]
It seems clear, but I have to spend another 40 euro for the BMS ... It's not very cheap for a student :sweat_smile:

whatever thanks for the tips!
```

---
## \#24 Posted by: sayreul Posted at: 2017-05-26T10:04:11.651Z Reads: 143

```
Check if you can setup a cut of for your esc

You can try the eBay BMS -- up to you ;)
```

---
## \#25 Posted by: edoardo Posted at: 2017-05-26T10:26:27.807Z Reads: 138

```
[quote="sayreul, post:24, topic:23904"]
Check if you can setup a cut of for your esc
[/quote]
> [...]
> _Multiple protection features_: Low voltage cut-off protection 
> [...]

And:

> **Customized Voltage cutoff**: you can select a starting cutooff voltage of 4,5,6,9 or 12 volts. Then using the up/down to the right of the voltage you can increase the voltage stepping up 0.1V between the selectable settings.
> ( when using any Lithium batteries, they must not be discharged to less than 3.0v per cell )
```

---
## \#26 Posted by: TarzanHBK Posted at: 2017-05-26T10:32:32.291Z Reads: 127

```
don´t rely on the ESC cutout. They only check the sum Voltage of all cells. So if you have one or two drifting cells it´s likely that they will discharge to much before toggling the ESC cutoff.
```

---
## \#27 Posted by: edoardo Posted at: 2017-05-26T10:38:20.336Z Reads: 127

```
[quote="TarzanHBK, post:26, topic:23904, full:true"]
don´t rely on the ESC cutout. They only check the sum Voltage of all cells. So if you have one or two drifting cells it´s likely that they will discharge to much before toggling the ESC cutoff.
[/quote]
Ok, thanks. What do you thing about eBay BMS ?
```

---
## \#28 Posted by: Okami Posted at: 2017-05-26T10:54:11.220Z Reads: 134

```
I think you should just buy the cheapest you can afford now and go with it.. 

A lot of people dont use the bms in the first place ;)

---

On the topic of your choosen BMS, look at this:

Lampshift maximum discharge current: 15A
**Instantaneous discharge current: 25A**
Charging voltage: 25.5V
Charging current: 15A (MAX)
Overcharge detection voltage: 4.28 ± 0.05V
Overcharge protection delay: 0.1S
Overcharge release voltage: 4.08 ± 0.05V
**Over discharge detection voltage: 2.55 ± 0.08V**
Overdischarge detection delay: 0.1S
The overdischarge release voltage: 2.9 ± 0.1V
Overcurrent detection voltage: 150mV
Overcurrent detection delay: 9MS
Overcurrent protection current: 30 ± 3A
**Overcurrent protection release condition: Disconnect the load**
Short circuit detection delay: 250uS

It seems like this BMS wont work very good for you.

Just search for one which is - Charge Only, and use a seperate monitoring circuit (device) to know the lipo pack voltage.

You dont want that your bms just disconnects after it has reached certain voltage or amps also. You might loose power in situations where u maybe most need it and it can happen accidentally.

---


So just be extra careful when you use your cells afterwards and please install a seperate battery monitoring circuit!

It costs like 5$ extra but I would advise to get a better one, at least for 20$ or so.


I can recommend this one, but it is a bit pricy, otherwise please seek similar options (which still work reliably)

https://www.banggood.com/ISDT-BC-8S-Battery-Checker-with-Two-85dB-Buzzer-for-LiPo-LiHv-LiFe-LiIon-Batteries-p-1128253.html?rmmds=search

--

Cheapos are these but I hate buzzers and mine didnt work correctly.. so I would just buy the better one
https://hobbyking.com/en_us/cell-checker-with-low-voltage-alarm-2s-8s.html
```

---
## \#29 Posted by: Okami Posted at: 2017-05-26T10:59:44.060Z Reads: 120

```
One more option (the one I gave u in the beginning:

https://hobbyking.com/en_us/turnigy-b6-compact-50w-5a-automatic-balance-charger-2-6s-lipoly.html

Though, havent tried these, so you should find out how reliable they are, u would still need a laptop powersupply, in the needed voltage range.. and u would need to glue the connectors into the charger.

<img src="/uploads/db1493/original/3X/0/8/08b008e580f6a8f27548645b983ff7c471572e96.png" width="565" height="414">
```

---
## \#30 Posted by: TarzanHBK Posted at: 2017-05-26T10:59:49.352Z Reads: 113

```
can work, can fail - some are better than others...
If you wanna be safe, spend a few bucks more and get a good one from batterysupport or bestech.

You use 6s normally because it´s cheap. Therefor, easiest thing is to use a imax b6 - cheap too and works really well.
If you like to add more comfort to it, get the miami VGA charging solution. You could build one on your own.
If you want to spend a bit more and really wanna use the laptop charging style, I´d recommend getting a BMS only for charging, because I don´t know any affordable BMS that is able to deliver the Amps you need on 6s. 60A is not enough in my opinion. If you wanna go that route, search for bypassing BMS here on the forum.
Also make sure, no matter which method you choose, to monitor your cells. Use a low voltage alarm or some other solution.
```

---
## \#31 Posted by: edoardo Posted at: 2017-05-26T11:25:54.642Z Reads: 111

```
But In this case sometimes I have to check manually the voltage of each cells ?

[quote="Okami, post:28, topic:23904"]
So just be extra careful when you use your cells afterwards and please install a seperate battery monitoring circuit!

It costs like 5$ extra but I would advise to get a better one, at least for 20$ or so.

I can recommend this one, but it is a bit pricy, otherwise please seek similar options (which still work reliably)
[/quote]
I already have this https://hobbyking.com/it_it/hobbykingtm-lipo-voltage-checker-2s-8s.html, it has the same duty?
```

---
## \#32 Posted by: Okami Posted at: 2017-05-26T11:30:38.999Z Reads: 106

```
yes, u can use that one, no problem, just make sure it is somewhat accurate and now when to stop riding the board..

At what level/voltage per cell have u put it?

When do u stop riding your eboard?
```

---
## \#33 Posted by: edoardo Posted at: 2017-05-26T11:35:33.386Z Reads: 101

```
[quote="Okami, post:29, topic:23904"]
https://hobbyking.com/en_us/turnigy-b6-compact-50w-5a-automatic-balance-charger-2-6s-lipoly.html
[/quote]
That's a good ( and simple ) idea... I have to glue the connector to avoid disconnection during riding?

[quote="TarzanHBK, post:30, topic:23904"]
If you wanna go that route, search for bypassing BMS here on the forum.Also make sure, no matter which method you choose, to monitor your cells. Use a low voltage alarm or some other solution.
[/quote]
I don't understand this part. Sorry can you explain me more? :confused:
```

---
## \#34 Posted by: TarzanHBK Posted at: 2017-05-26T11:42:07.917Z Reads: 95

```
You can use a cheaper BMS, like a 6s 10A BMS, but then you can´t discharge through it, because of the 10A Limit. So you have to bypass it. How do you do it? Search for "bypassing BMS" here on the forum.
```

---
## \#35 Posted by: edoardo Posted at: 2017-05-26T12:01:08.440Z Reads: 92

```
All topic that I found are about VESC and BMS so they are protected by undervolts.
I don't have a VESC...
```

---
## \#36 Posted by: Namasaki Posted at: 2017-05-26T12:25:43.429Z Reads: 95

```
[quote="edoardo, post:18, topic:23904"]
Where you recommend to buy a BMS?
[/quote]
http://bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#37 Posted by: Okami Posted at: 2017-05-26T12:25:56.630Z Reads: 102

```
He means that if you buy one of these cheap bms, use it 'In Charge mode' only.

Usually people hook up their bms in a way that it both helps to 'Charge' and also protects cells while 'Discharging.

I think you just need to make a parallel Port / Cables to your existing batteries, then attach Charge only bms to that side of wires, and you should be good to charge through BMS (also u will need to connect balance wires, so the bms knows the voltage level of each cell group).

U should now decide which route is best for you..

---

1) If you choose to go with 'portable battery charger', then you will need to carry 'dead weight' around with you and you will also need laptop power supply to charge it

2) If you choose to go with bms, the weight is less but u will need to make an enclosure to protect the bms module from the elements (or just put it inside of the box, with batteries)..

Here u also gonna need the **right voltage power supply**, but you will need to buy a special one, which suits the battery voltage directly. At least I dont know can you really attach 12v to 24v bms and expect it to charge up the batteries. Im pretty sure these low cost modules dont have step up converters there..


Ok I hope this makes it a bit more clear now.

So yes, route 1) just 50W charging module + laptop power supply of about 11-12v (70W recommended)
2) Chinese Bms with possible future faults (not balancing cells), disconnecting etc, which needs extra protection (from elements and shorts) + Proper voltage power supply (possibly ~25.2v) 

U can look up how much such power supply costs.

In both cases u also need to buy parallel cable for your existing connection, unless you want to do it by hand and solder new cables to the existing ones.

---

What power suplly are u using now for your b6 charger?

How many volts it is?
```

---
## \#38 Posted by: Okami Posted at: 2017-05-26T12:31:25.854Z Reads: 91

```
Extra info - Sometimes it might be a pain to connect batteries to BMS.. Ive seen shorts, smoke and other nasty stuff coming up.. be sure you already now understand which cables go where.

IF I were you, I would just buy that small B6 module I showed you and would hope it does not break because of vibration..

Then yes, just plug in the cables like you now do for your imax b6 and and glue the cables to the box, and in theory it should select the right battery voltage and start charging once you attach a cable of 12v from your laptop power supply (most easiest solution)

Look it up in more detail, im pretty sure people are using it on youtube etc.. for reviews and so on.
```

---
## \#39 Posted by: edoardo Posted at: 2017-05-26T12:37:10.146Z Reads: 91

```
I don't understand a thing.

[quote="sayreul, post:19, topic:23904"]
&lt;30A for charge only, 60A for charge and discharge (the BMS help you to protect your lipo during discharge (cut of) )
[/quote]
[quote="TarzanHBK, post:30, topic:23904"]
I´d recommend getting a BMS only for charging, because I don´t know any affordable BMS that is able to deliver the Amps you need on 6s.
[/quote]

The two opinions are contradictory. If I invest money to bought a decent BMS ( http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html ) can I use it for charge and discharge?
```

---
## \#40 Posted by: Okami Posted at: 2017-05-26T12:41:25.541Z Reads: 95

```
I would say - get this one and save yourself a trouble

<img src="/uploads/db1493/original/3X/8/a/8a87d24d64d6fb48249e7feec54f83c51163621d.png" width="565" height="414">

They even include the cables:

<img src="/uploads/db1493/original/3X/7/1/71473ede0ff8d3a089daaf42bafd94bf6f31af34.png" width="331" height="273">


**Extra Weight** to your board:
**265g** + some cables

**--**

**Costs about 12Eur** _and comes from europe. u will wait a month or so just to get the bms, then you gonna need to solder the cables or connectors._

_With this thing you just plug everything in, make sure it does hold in place, and attach the right voltage as I said_

_It looks like it works from:_

----
**11 - 18v**
So you can use 15-16v power bricks from laptops without a problem and it will be even better than 12v power bricks.
```

---
## \#41 Posted by: TarzanHBK Posted at: 2017-05-26T12:44:09.384Z Reads: 87

```
You can.
The thing is: With 6s (22,2V) you need much more current to get the needed Watts to move.
So with 10s (36V) and 60A you get: 36V x 60A = 2160W max, which is good.
On 6s: 22,2V x 60A = 1332W which might be ok for most cruising, but you get problems on hills if you´re not a featherweight.
If you´d use this BMS it´s gonna be your bottleneck in the system, which slows everything down.
To overcome that, don´t use it for discharging.
```

---
## \#42 Posted by: edoardo Posted at: 2017-05-26T12:49:05.606Z Reads: 89

```
[quote="TarzanHBK, post:41, topic:23904"]
To overcome that, don´t use it for discharging.
[/quote]
How can I do it? Reading other threads I don't understand...

I want to have clear all possibilities to decide. :)
```

---
## \#43 Posted by: TarzanHBK Posted at: 2017-05-26T12:51:57.733Z Reads: 85

```
https://www.electric-skateboard.builders/t/bypass-bms-with-overcharge-detection-how-that-works/22582
You´ll find the right diagramm on the bottom of the post, just do some reading before you decide
```

---
## \#44 Posted by: Namasaki Posted at: 2017-05-26T13:36:23.183Z Reads: 90

```
[quote="edoardo, post:39, topic:23904"]
The two opinions are contradictory. If I invest money to bought a decent BMS ( http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html ) can I use it for charge and discharge?
[/quote]

Yes you can. And charging/discharging is the best option because it provides the most protection for your battery and system. 

Bypassing is also an option but it is a compromise because it circumvents short protection, over discharge protection and overcharging from regenitive braking protection.
```

---
## \#45 Posted by: edoardo Posted at: 2017-05-26T14:49:38.927Z Reads: 84

```
[quote="TarzanHBK, post:41, topic:23904"]
On 6s: 22,2V x 60A = 1332W which might be ok for most cruising, but you get problems on hills if you´re not a featherweight
[/quote]
1332 watts is anyway my "max power" because my [turnigy sk3 280kv](https://hobbyking.com/it_it/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html) can handle up to 60A. 
So if I use a 6S 60A BMS is good enough to discharge, right?
```

---
## \#46 Posted by: Okami Posted at: 2017-05-26T14:56:32.171Z Reads: 87

```
yeh it is. 

I hope no problems meet you when you gonna go the bms route ;)
```

---
## \#47 Posted by: edoardo Posted at: 2017-05-26T15:14:31.619Z Reads: 92

```
I tried to do this diagram, but I think I miss something .. eg where and how do I use the anti-spark connector ??

http://i.imgur.com/KjZ45CU.jpg

Thanks for patience! :blush:
```

---
## \#48 Posted by: edoardo Posted at: 2017-05-27T12:19:16.447Z Reads: 84

```
@Okami @sayreul @TarzanHBK Can someone help me?
```

---
## \#49 Posted by: Namasaki Posted at: 2017-05-27T12:38:53.973Z Reads: 86

```
The anti-spark connector goes between the power source and the ESC. 
The voltage meter goes between the anti-spark connector and the ESC
```

---
## \#50 Posted by: edoardo Posted at: 2017-05-27T13:07:15.245Z Reads: 87

```
And now how I connect the charge plug? 


<img src="/uploads/db1493/original/3X/e/2/e29f4c79fd6656992227c23532685113e69444ac.jpg" width="690" height="348">
```

---
## \#51 Posted by: Tuomalar Posted at: 2017-05-27T13:59:49.182Z Reads: 86

```
Black between bms and esc and red between anti-spark and battery
```

---
## \#52 Posted by: Namasaki Posted at: 2017-05-27T14:03:49.048Z Reads: 82

```
The voltage meter will have  red and black wires that connect to the red and black wires between the ESC and power source
```

---
## \#53 Posted by: Smorto Posted at: 2017-05-27T14:32:09.284Z Reads: 84

```
This would be my BMS diagram. Feel free to take a look.

https://docs.google.com/drawings/d/1tXLadrh44pFh265D3_fWR32QnZEoWXcDMkGyta21g6Q/edit
```

---
## \#54 Posted by: Hummie Posted at: 2017-05-27T14:34:07.783Z Reads: 84

```
Can't u put the voltmeter, bms, and antispark in any order between the battery and esc
```

---
## \#55 Posted by: Namasaki Posted at: 2017-05-27T15:17:30.701Z Reads: 86

```
You want the switch or key to turn on the meter and ESC. 
And the ability  to charge the battery through the BMS without turning on the rest of the system
```

---
## \#56 Posted by: edoardo Posted at: 2017-05-27T17:37:16.495Z Reads: 85

```
[quote="Tuomalar, post:51, topic:23904, full:true"]
Black between bms and esc and red between anti-spark and battery
[/quote]
[quote="Namasaki, post:52, topic:23904, full:true"]
The voltage meter will have  red and black wires that connect to the red and black wires between the ESC and power source
[/quote]
Is that right?

<img src="/uploads/db1493/original/3X/0/9/0977bb0cf8af4b2e3bb112dceee9dbf64fce05bf.jpg" width="690" height="356">

[quote="Smorto, post:53, topic:23904"]
This would be my BMS diagram. Feel free to take a look.
[/quote]
Thanks, I'll take a look! ;) 

[quote="Namasaki, post:55, topic:23904, full:true"]
You want the switch or key to turn on the meter and ESC. And the ability  to charge the battery through the BMS without turning on the rest of the system
[/quote]
I want to use the ESC's button to turn on the system.
And yes I want the ability to charge the battery through the BMS without turning on the system.
```

---
## \#57 Posted by: edoardo Posted at: 2017-05-27T17:56:33.524Z Reads: 69

```
You use the BMS only to charge the batteries right?
```

---
## \#58 Posted by: Tuomalar Posted at: 2017-05-27T19:07:54.704Z Reads: 67

```
Looks fine to me. @Namasaki can confirm?
```

---
## \#59 Posted by: Namasaki Posted at: 2017-05-27T19:10:04.713Z Reads: 67

```
Yes, your diagram is looking better with every update.
```

---
## \#60 Posted by: Namasaki Posted at: 2017-05-27T19:11:48.096Z Reads: 73

```
There is one detail that you still have to address and that is the balance wire connection between the battery and the bms. 
You can't just plug the jst connector from the battery into the bms. 
The bms will come with its own connector and wires. 
And the bms will only use balance 6 wires whereas the battery has 7 balance wires.
I'd first  like to see if you can figure it out but if you can't, don't worry, we will tell you what to do.
```

---
## \#61 Posted by: edoardo Posted at: 2017-05-27T19:30:30.777Z Reads: 74

```
I have a question, "_anti-spark switch_" for me means this:

<img src="/uploads/db1493/original/3X/4/f/4fa5290ee6c876b5498e73e3ea45e01517c8ca61.jpg" width="244" height="245">

Is this necessary? Consider that: 
[quote="edoardo, post:56, topic:23904"]
I want to use the ESC's button to turn on the system.And yes I want the ability to charge the battery through the BMS without turning on the system.
[/quote]


----------

[quote="Namasaki, post:60, topic:23904, full:true"]
There is one detail that you still have to address and that is the balance wire connection between the battery and the bms. You can't just plug the jst connector from the battery into the bms. The bms will come with its own connector and wires. And the bms will only use balance 6 wires whereas the battery has 7 balance wires.I'd first  like to see if you can figure it out but if you can't, don't worry, we will tell you what to do.
[/quote]
Maybe I should not use a cable from the JST battery? But which of them? ...
```

---
## \#62 Posted by: Namasaki Posted at: 2017-05-27T19:52:40.874Z Reads: 70

```
The Lipo has only 6 cells but there are 7 balance wires. 
What would you guess the extra wire is for?
```

---
## \#63 Posted by: edoardo Posted at: 2017-05-27T20:24:48.755Z Reads: 72

```
To consider each cell's voltage as one ( the sum ) ?
```

---
## \#64 Posted by: edoardo Posted at: 2017-05-27T20:38:03.081Z Reads: 69

```
I know that each lead of balance cable is connected to:
- main leads ( + , - )
- middle link betwheen cells

So for example: 6 cells make 7 cable , 5 in the middle and 2 main leads.

Right?
```

---
## \#65 Posted by: Namasaki Posted at: 2017-05-27T21:03:35.730Z Reads: 71

```
The 6 color wires go to the pos side of each cell. 
The red wire on the edge of the connector is always the last cell in series. In this case its cell 6. 
The black wire on the opposite edge is always a ground wire. 
You omit the black ground wire when connecting to a Bestech or Battery Supports bms.
```

---
## \#66 Posted by: edoardo Posted at: 2017-05-27T21:10:53.126Z Reads: 72

```
But after this mod I'll not be able to charge the battery with my Imax B because of soldering leads of balance cable??
```

---
## \#67 Posted by: SageTX Posted at: 2017-05-27T22:09:54.996Z Reads: 69

```
Correct. However i used a balance lead extension and soldered those to the wires from the BMS lead. Then just plugged the battery's lead into that.  
That way i could still balance them _if_ I ever wanted to. However I never have. But it still makes it easier to replace a battery if ever needed.
```

---
## \#68 Posted by: Namasaki Posted at: 2017-05-27T23:03:17.986Z Reads: 65

```
I'm with @SageTX
That is the solution that I used on my builds and in my opinion, it's the best solution.
```

---
## \#69 Posted by: Smorto Posted at: 2017-05-28T00:41:01.269Z Reads: 67

```
No, this was a digram using the BMS for charging as well.
```

---
## \#70 Posted by: edoardo Posted at: 2017-05-28T08:51:57.189Z Reads: 70

```
I like this solution, thank you very much! So I have to create a balance lead extension without the black wire ( ground ) in order to connect the JST-HX ( 7 wire - 7 pin ) from my battery to the new balance lead ( 6 wire - 7 pin ) of the BMS, all right?
Are these good?? : http://amzn.to/2qvRdat 

@Namasaki Can you answer to this question please? 
[https://www.electric-skateboard.builders/t/is-it-possibile-to-charge-an-e-skate-directly-to-the-home-socket/23904/61?u=edoardo](https://www.electric-skateboard.builders/t/is-it-possibile-to-charge-an-e-skate-directly-to-the-home-socket/23904/61?u=edoardo)
```

---
## \#71 Posted by: BigBoyToys Posted at: 2017-05-28T09:25:41.886Z Reads: 65

```
Yes, search BMS on the forum. If you add a bms to your board youll be able to charge from a wall socket. Its basically putting your imax charger inside the board :)
```

---
## \#72 Posted by: edoardo Posted at: 2017-05-28T12:13:14.768Z Reads: 74

```
Sorry but I did not understand how you implemented these parts:

<img src="/uploads/db1493/original/3X/c/d/cd8fcf50e838b4f7d1762b45b71b0f8e09ffb516.jpg" width="579" height="500">

XT60 has to pin ho how do you connect three of this in that way?
```

---
## \#73 Posted by: Smorto Posted at: 2017-05-28T12:49:30.249Z Reads: 77

```
It is a parallel connector or splitter like this one I made. All it does is turn one XT60 into 2 XT60s.

<img src="/uploads/db1493/original/3X/1/e/1e4b070285db7020d41694e0ea510e3df627b773.jpg" width="690" height="459">

You can also find them online for cheap, tho these have wires and are backwards (male where female should be and vice versa). I recommend making your own which is easier,  smaller, and cheaper.
https://www.amazon.com/Dimart-Parallel-Connector-Extension-Splitter/dp/B01ALERNYA/ref=sr_1_5?s=toys-and-games&ie=UTF8&qid=1495975600&sr=1-5&keywords=XT60+parallel+y+cable

The second place you circled I simply soldered the voltage meter onto the XT60 along with the main power leads.

<img src="/uploads/db1493/original/3X/e/d/ed38cae5919a3cdd42ed2fd3adb093d6fc5c9503.jpg" width="690" height="459">

<img src="/uploads/db1493/original/3X/4/d/4dff62683fab9cc6fb87e28464b2139114a22e0f.jpg" width="690" height="459">
```

---
## \#74 Posted by: edoardo Posted at: 2017-05-28T13:53:40.355Z Reads: 71

```
Now it's clear. Thanks!

My voltage meter has JST-HX connector ( is used with my LiPo battery ), I have to buy another one with red/black wires?
<img src="/uploads/db1493/original/3X/8/4/84674246aa2e96b1ab257cb31e01bdc3a386ab9f.png" width="393" height="337">
```

---
## \#75 Posted by: Smorto Posted at: 2017-05-28T16:48:44.343Z Reads: 65

```
Yes you should, those lipo checkers usually drain power from one cell which leads to uneven cells.
```

---
## \#76 Posted by: edoardo Posted at: 2017-05-28T19:04:35.569Z Reads: 64

```
Could you suggest one of these from AliExpress?
```

---
## \#77 Posted by: SageTX Posted at: 2017-05-28T19:57:54.703Z Reads: 63

```
Yes. That's a plan.
And yes those are fine.
```

---
## \#78 Posted by: Smorto Posted at: 2017-05-29T00:20:41.403Z Reads: 65

```
https://nl.aliexpress.com/item/No-Wires-XT60-Parallel-Battery-Connector-for-Turnigy-Zippy-XT-60/32581075055.html?spm=2114.010208.3.50.oBpO16&ws_ab_test=searchweb0_0,searchweb201602_3_10152_5010012_10065_10151_10130_10068_10136_10137_10157_10060_10138_10155_10062_10156_437_10154_10056_10055_10054_10059_303_100031_10099_10103_10102_10096_10147_10052_10053_10107_10050_10142_10051_5020012_10084_10083_10080_10082_10081_10178_10110_519_10111_10112_10113_10114_10182_10185_10078_10079_10073_10123_142-10102,searchweb201603_2,ppcSwitch_5&btsid=4cf52aa6-e82f-480a-b1e9-4228faa8022b&algo_expid=05602804-35e0-4978-af1c-4884cda66470-6&algo_pvid=05602804-35e0-4978-af1c-4884cda66470
```

---
## \#79 Posted by: edoardo Posted at: 2017-05-29T06:39:54.656Z Reads: 62

```
Sorry but I meant to suggest a voltmeter ( 2 wire ) from AliExpress with a right voltage range and precision.
```

---
## \#80 Posted by: edoardo Posted at: 2017-05-29T10:56:31.746Z Reads: 60

```
This charger ( https://goo.gl/kFJwtD ) will work fine with this BMS ( https://goo.gl/1kpBcP ) ?
 
And 4A is a reasonable way to charge a 4500mAh 22.2V 6s1p LiPo battery?
```

---
## \#81 Posted by: Smorto Posted at: 2017-05-29T13:07:12.895Z Reads: 62

```
Ahhh sorry, misunderstanding.

Something like this should work, though if you just search for "voltage meter" in the search bar and choose something that fits your voltage it should be fine.

https://nl.aliexpress.com/item/Portable-Digital-Voltmeter-DC0-100V-Red-Light-LED-Panel-Voltage-Meter/1831150751.html?spm=2114.010208.3.285.hMyAkJ&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10130_10068_5010013_10136_10137_10157_10060_10138_10155_10062_10156_437_10154_10056_10055_10054_10059_303_100031_10099_10103_10102_10096_10147_10052_10053_10107_10050_10142_10051_5020013_10084_10083_10080_10082_10081_10178_10110_519_10111_10112_10113_10114_10182_10185_10078_10079_10077_10073_10123_142,searchweb201603_2,ppcSwitch_5&btsid=39790f67-9b8a-412a-adb3-ca5eb1dfc34a&algo_expid=6c5c5b5b-41ee-4032-b342-030aaf2e29fe-38&algo_pvid=6c5c5b5b-41ee-4032-b342-030aaf2e29fe
```

---
## \#82 Posted by: edoardo Posted at: 2017-05-29T14:26:17.909Z Reads: 59

```
Can U help me also in this question? 
https://www.electric-skateboard.builders/t/is-it-possibile-to-charge-an-e-skate-directly-to-the-home-socket/23904/80
```

---
## \#83 Posted by: sayreul Posted at: 2017-05-29T14:38:49.090Z Reads: 58

```
yes it should be ok
```

---
## \#84 Posted by: Smorto Posted at: 2017-05-29T17:03:57.689Z Reads: 56

```
Yes 4A is almost 1c for your batteries so it will be fine.
```

---
## \#85 Posted by: rojitor Posted at: 2017-05-31T22:18:20.592Z Reads: 51

```
Lipo is the most dangerous chemistry available. I would not put my faith on a bms. You can "bulk" charge your lipo and then balance once every 5 or 10 times. You will save some time while keeping  it safe. The only thing you must do is leave a reasonable margin of security. Lipo cells charge to 4.2 for bulk charge you should do 4.10 or 4.15 tops. As long as you balance it often you are safe. I have been doing it for years. No problem.
```

---
## \#86 Posted by: edoardo Posted at: 2017-05-31T22:33:00.722Z Reads: 50

```
[quote="rojitor, post:85, topic:23904"]
The only thing you must do is leave a reasonable margin of security. Lipo cells charge to 4.2 for bulk charge you should do 4.10 or 4.15 tops.
[/quote]
So I have to check manually voltage at the end of charge through BMS ?
```

---
## \#87 Posted by: rojitor Posted at: 2017-05-31T23:00:09.603Z Reads: 55

```
If you bulk charge you do not need bms.
You plan to charge 6s right?
4.2 x 6= 25.2v this is the usual voltage 
4.10 x 6= 24.6v
4.15 x 6= 24.9
You just need a charger with 24.6-24.9v output and solder bullets
You balance your lipo and you use the bulk the next time. You check the voltage when done with one of Those lipo voltage checkers. You should see 4.10-4.15 per cell. You can use it 5-10 times. As soon as you see one of the cells goes rogue you balance again....And so on. At least one balance every 10 charges. This way is cheaper and safer than bms. (Unless you spend hundreds on a GOOD bms).
The use of a buzzer is advised  too.
```

---
## \#88 Posted by: rojitor Posted at: 2017-05-31T23:13:12.258Z Reads: 55

```
Some sellers can modify the voltage of the charger by request. If you can't find it you can use a buck converter.
The 12 volt power supply of your lipo charger will do.
Connect it to one of these
[OOTDTY Pantalla Digital DC-DC Step Up Step Down Buck Boost Junta Módulo de Potencia Del Convertidor  http://s.aliexpress.com/aUba6Jfi  (from AliExpress Android)](OOTDTY Pantalla Digital DC-DC Step Up Step Down Buck Boost Junta Módulo de Potencia Del Convertidor  http://s.aliexpress.com/aUba6Jfi  (from AliExpress Android))
```

---
## \#89 Posted by: Hummie Posted at: 2017-06-01T01:32:50.925Z Reads: 60

```
Every bulk charger I've ever gotten has a little screw to adjust voltage.   Definately worth wiring in a wattmeter <img src="/uploads/db1493/original/3X/8/1/817b1700eaccfcd905196b35823c0aa667714c94.png" width="333" height="500">
Rare that I hear someone say it's safer but potentially.   The benefit of charging at high wattage is a huge time saver and if ur using lipos u likely can
Much simpler and cheaper. And get an xt90s plug and ur done. <img src="/uploads/db1493/original/3X/a/e/aef09979360a6c81fa01b799ece0d6f1a6f1f5c1.png" width="333" height="500">
```

---
## \#90 Posted by: rojitor Posted at: 2017-06-01T09:52:11.770Z Reads: 54

```
That depends on the lipo C rate and the amps delivered by the bulk charger. lipo can usually take high C for charge while chargers are usually slow. No problem as long as you do not exceed the recommended C charging speed.
<img src="/uploads/db1493/original/3X/5/5/5548ae39124490bb826a75cf1866e638b090df8d.jpg" width="690" height="475">
Some chargers are easy to modify just by adjusting two screws. voltage and amperage. Any multimeter can measure the changes. It is a fast and easy mod. Nevertheless i think he can find some charger 24-24.9v out of the box. Buck converters are available at any electronics store too.
```

---
