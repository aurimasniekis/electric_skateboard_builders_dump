# How to charge permanent mounted battery

### Replies: 39 Views: 8508

## \#1 Posted by: ikjahaa Posted at: 2016-02-07T14:07:16.382Z Reads: 457

```
Hello,
I would like to have my lipo permenatly fixxed to my board, just like the boosted board has. I currently have a 12AWG wire running through the wood of my deck from the back tructs to the front. Now I would like to solder the charge leads of my lipo to those wires and somehow "split" the charge leads from the lipo so i can charge it without having to dismount them.

I was thinking of using a switch that would close the connection from my battery to the wires running to the esc and opening the connection from the charge port to my lipo's charge leads ? Would this be a viable solution or is there something better I can/should do ?
If not, what switches should I use ?

Lipo: http://www.hobbyking.com/hobbyking/store/__9183__Turnigy_5000mAh_3S_25C_Lipo_Pack.html
VESC: http://www.enertionboards.com/electric-skateboard-parts/vesc-motor-controller/
```

---
## \#2 Posted by: paragon Posted at: 2016-02-07T15:57:44.378Z Reads: 452

```
not to sure, but i think a loop key switch and connecting a bms may be an alternative to exposing your balance plugs.
```

---
## \#3 Posted by: Kaly Posted at: 2016-02-07T15:58:40.213Z Reads: 448

```
hello 

first what battery configuration are you going to use?
and what charger are you going to use?

this is how i have my batteries, i used 4-3S pack and configured this  into 2-6S packs. this configuration can be use in 2 different mode (6S and 12S) via a DTDP switch. the yellow xt90 connector is for a anti-spark key loop, this prevent the charging current from getting to the esc.

<img src="/uploads/db1493/original/2X/5/579c354e67b50ad4a2e907f6d64393483bed253d.JPG" width="375" height="500">

i included the charging port, the balance and the volt meter with a 3.4V alarm port into the enclosure , for this i just solder a jst connector to the balance lead and installed a  micro on/off switch on to the negative wire of the extension balance lead that goes to the volt meter. 

<img src="/uploads/db1493/original/2X/1/175ea8fbfb3425a0c4ac7edc5bb87d75d4486a8d.JPG" width="666" height="500">
```

---
## \#4 Posted by: ikjahaa Posted at: 2016-02-07T16:31:58.393Z Reads: 431

```
Well, I would like to start with a single 3S pack to which I'll probally add another 3S pack in the near future.
I'm going to use the VESC cutoff settings to disable the board if my batteries aren't providing enough voltage, So i wont need the voltmeter/alarm port. The ballance wires are only needed for charginf so I have no problem with those..

I do however like that DTDP switch, It gave me the idea to use a 2 way switch or something (if those exist)
State A : lipo wires connect to charger wires
State B: lipo wires connect to esc wires
<img src="/uploads/db1493/original/2X/e/e3bc29a203397df3f6f9d6b4b70a583b058318e5.png" width="589" height="354">
The only problem i have with this solution are sparks ?

ps. Sorry for my crappy paint skills
```

---
## \#5 Posted by: Kaly Posted at: 2016-02-07T16:46:55.868Z Reads: 412

```
For the spark check this 
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
```

---
## \#6 Posted by: ikjahaa Posted at: 2016-02-07T16:59:44.482Z Reads: 404

```
I updated my sketch.
I would prefer to use a switch over a loop key, because i'm afraid that I might plug in the charger without pulling out the loop key first. With this switch solution, It doesnt matter. Your charger will not find the batteries if you didnt switch it to charge mode.
```

---
## \#7 Posted by: ikjahaa Posted at: 2016-02-07T17:37:27.452Z Reads: 386

```
[quote="Kaly, post:3, topic:1261"]
DTDP switch
[/quote]

How did you know howmuch amps the switch had to be able to handle ?
if batteries provide 5000mah @ 20C, would that mean my switch needs to be able to handle 100amps ?
```

---
## \#8 Posted by: Kaly Posted at: 2016-02-07T20:25:44.376Z Reads: 371

```
Check the switch rating and get the watts 
W=v*a
And check how much watt you are going to be using
```

---
## \#9 Posted by: ikjahaa Posted at: 2016-02-07T20:39:38.617Z Reads: 362

```
[quote="Kaly, post:8, topic:1261"]
check how much watt you are going to be using
[/quote]
using by ? the esc, motor or charger ?
```

---
## \#10 Posted by: Kaly Posted at: 2016-02-07T21:57:51.340Z Reads: 356

```
Your whole setup 
If you are using 6s that's 22.2V x 35 amps that will be 777 watts
```

---
## \#11 Posted by: ikjahaa Posted at: 2016-02-07T22:01:06.670Z Reads: 346

```
how did you get those 35 amps?
```

---
## \#12 Posted by: onloop Posted at: 2016-02-07T22:19:46.263Z Reads: 349

```
There are not many switch options that can work.

1. Vedder antispark
2. @lowGuido has a breaker that is an actual switch.
3. @torqueboards has an anti spark switch.
4. Buy a space cell ;)

A simple loop key is a good cheap option but not very elegant.
```

---
## \#13 Posted by: ikjahaa Posted at: 2016-02-07T23:01:08.132Z Reads: 345

```
I am not trying to switch my esc off, well not directly.
I want to be able to select the circuit. Battery to ESC or battery to charger.
(battery to charger = switching esc off indirectly)

Currently i'm looking into heavy duty SPDT switches, which shouldn't spark since they are designed for such purposes.
```

---
## \#14 Posted by: Kaly Posted at: 2016-02-08T00:38:39.286Z Reads: 337

```
[quote="ikjahaa, post:11, topic:1261, full:true"]
how did you get those 35 amps?
[/quote]


On my previous built I installed a watt meter and keep a log. 
 from this normal real world data use I determine the average watt use by the eBoard with a load of my weight.
```

---
## \#15 Posted by: laurnts Posted at: 2016-02-08T01:39:12.057Z Reads: 320

```
I am using this rocker switch.
https://www.conrad.nl/nl/marquardt-19323112-wipschakelaar-250-vac-16-a-2x-uitaan-ip65-vergrendelend-1-stuks-700093.html13

It's not a SPDT but a DPDT. The reason I go for DPDT is that I could hook up both poles to be able to support double current draw.
```

---
## \#16 Posted by: onloop Posted at: 2016-02-08T01:40:46.975Z Reads: 331

```
if you isolate the ESC with a switch you are essentially switching the battery to the Charge circuit, aren't you?

Normally people use a switch to simply isolate the ESC from battery. It's to turn your board off. You can actually charge your battery whether the ESC is isolated or not.

So what exactly are you trying to do?
```

---
## \#17 Posted by: laurnts Posted at: 2016-02-08T03:36:20.487Z Reads: 335

```
[quote="ikjahaa, post:13, topic:1261"]
How-To: Anti-Spark XT-90 Loop Key
[/quote]

In my thread I specifically posted how to do Antispark with 100 Ohm resistor. It's cheaper than getting your self an XT90 anti spark. Basically what Antispark does is limiting the current draw of your ESC capacitors when all circuits are connected. By providing a small resistance, it can't draw that much amps in short period of time, hence there is no spark. But afterwards, you would need to connect the bigger power connector. Here is a simple diagram of an antispark
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/a/a1196c8f5a859e59cb3fb605690d0da69dc35d6c_1_690x450.JPG

So you connect the auxiliary first (no sparking already), then connect the power connector. That simple.
With the XT90 loop key tutorial, it's all happening in 1 process as you plug the XT90 together (male and female).

---

But I got to say the way you think it's abit strange. Why do you want to have such connections? Either to battery / to charger.
The safest way is just to disengage the battery from the ESC completely and make separate cable port for charging (branch it / parallel it from the battery). I believe you would like to install the balancing charger and or powersupply within your electric longboard as well. If that is the case, then you should look for a BMS. BMS is just much smaller and does what balancer does without the bulk of box, displays and other charging features. 

---

I recommend you to read my build, I hope I would shine some light for you. My build components have quiet high similarities as yours. If I am correct with what I mention above, then you should read it!
http://www.electric-skateboard.builders/t/project-lacr-globe-the-maiden-deck-enertion-single-drive-propulsion-turnigy-sk3-6364-190-kv-vesc-4-10-turnigy-sentilon-100a-24v-10ah-zippy-flightmax-lipo-packs/
```

---
## \#18 Posted by: ikjahaa Posted at: 2016-02-08T16:50:39.470Z Reads: 301

```
[quote="onloop, post:16, topic:1261"]
Normally people use a switch to simply isolate the ESC from battery. It's to turn your board off. You can actually charge your battery whether the ESC is isolated or not.
[/quote]

This wouldn't harm the esc ?
```

---
## \#19 Posted by: ikjahaa Posted at: 2016-02-08T17:16:39.507Z Reads: 301

```
[quote="laurnts, post:17, topic:1261"]
The safest way is just to disengage the battery from the ESC completely and make separate cable port for charging (branch it / parallel it from the battery).
[/quote]

Yes, but what if you would start charging and forget to unplug the loop-key which disengages the battery to esc connection ?
```

---
## \#20 Posted by: Sebastiaan Posted at: 2016-02-08T17:44:55.059Z Reads: 301

```
You could use this, it has a switch integrated in the circuit, easy !

http://alienpowersystem.com/shop/rc-ev-accessories/electronics/alien-antispark-power-switch-2-14s-120amp-max/
```

---
## \#21 Posted by: ikjahaa Posted at: 2016-02-08T17:47:39.797Z Reads: 282

```
This is the same as a loop-key, just prettier.
```

---
## \#22 Posted by: laurnts Posted at: 2016-02-08T18:34:28.212Z Reads: 294

```
You could also forgot to switch off the switch in that sense. But if safety is your concern than you would also would like to consider the safety of battery shorts. I use switches to cut off power from battery from any source, wether it's from esc / charging cable. If you would like to add extra layer of protection, then you might want to add extra switch in your circuit for charging mode next to the adapter plug. Hence you would always see that switch every time you're about to charge your board that make sure that no electricity come to the esc.

---

For me I just simply branch out battery output into 2. 1 for esc and 1 for charging. The one for esc has a power switch / loopkey with it.

---

If you would like to go the extra mile for safety, you could instal a relay / mosfet switch within your charging cable.
Hence if the charging cable has power going through the cable, it will power up the relay / mosfet switch and cut off the connection from battery to esc. I am not an electrical engineer, so I can't help you build such thing. But pretty sure some one here are able to make such smart system.
```

---
## \#23 Posted by: Hummie Posted at: 2016-02-08T18:53:05.149Z Reads: 280

```
I was obsessed with finding a switch and then decided the xt90s plug is simple enough.  

I charge everything at once to 50 volts.  All these wire connections i have since heatshrinked over and sealed not to be taken apart again.  One big plug to charge or turn it on.  <img src="/uploads/db1493/original/2X/1/1e73f75db89b3e74e90881064663a20045110657.jpeg" width="500" height="500">


Here I'm charging with the bulk charger which has a watt meter in-line telling me the voltage and amps going in and with a balancer on the side
```

---
## \#24 Posted by: laurnts Posted at: 2016-02-08T19:05:53.442Z Reads: 271

```
For anyone else looking for 3PDT switch so you can't accidentally power up the ESC while charging, this is an option.
http://nl.mouser.com/ProductDetail/NKK-Switches/SW3833/?qs=sGAEpiMZZMtNT9UGfLL4eEXUF0YHaQ0QQUQGD5zP87o%3d

You don't need loopkey / antispark for it as it could handle pretty big amps easily. Only limited to 30V DC, hence it's about 8S top.
```

---
## \#25 Posted by: longhairedboy Posted at: 2016-02-08T19:13:10.784Z Reads: 272

```
i use the solid state switch from  on my 6S beteen the battery mains and the ESCs. This is how they are supposed to work. It won't hurt anything for sure. 

Also, a BMS and laptop style charger is probably the best solution for onboard charging. Otherwise you'll have to figure out some kind of multipin connector solution for your balance leads and discharge leads for using a standard lipo/li-ion charger.
```

---
## \#26 Posted by: ikjahaa Posted at: 2016-02-08T19:15:06.651Z Reads: 273

```
You can also buy a DPDT switch, with On-Off-On states.
My wiring setup so far....

<img src="/uploads/db1493/original/2X/2/2526077818d685ad2b3945c4e33cd3e74071c83c.png" width="690" height="212">
```

---
## \#27 Posted by: ikjahaa Posted at: 2016-02-08T19:15:47.260Z Reads: 268

```
[quote="longhairedboy, post:25, topic:1261"]
BMS
[/quote]
what does this abbreviation stand for ?
```

---
## \#28 Posted by: laurnts Posted at: 2016-02-08T19:17:57.602Z Reads: 263

```
ON Off ON State means 3PDT and not DPDT. DPDT only has ON and ON.
This switch is suitable for you. It has DC rating, has the Amps and has the switching state.

http://nl.mouser.com/ProductDetail/NKK-Switches/SW3833/?qs=sGAEpiMZZMtNT9UGfLL4eEXUF0YHaQ0QQUQGD5zP87o%3d

Hefty Price tag of 30 euro, but considering it's a specialize switch, it's cheap.
At least cheaper than the electronic mosfet switch that you can be sure it has total power cut off.

BMS stands for Battery Management System
```

---
## \#29 Posted by: longhairedboy Posted at: 2016-02-08T19:24:16.760Z Reads: 259

```
Battery Management System, i believe. ITs a circuit board that keeps your pack's cells balanced, allows the pack to be charged using a laptop style charger, protects from over charge and discharge, and generally makes things a lot more convenient. 

The only caveat is finding the right one for your needs. i'm still digging around for the perfect one for my needs, but since i've been playing around with ripped open space cells, i can totally see myself finding one for use with standard lipo packs. my next lipo build is definitely going to have one.
```

---
## \#30 Posted by: ikjahaa Posted at: 2016-02-08T19:25:36.188Z Reads: 271

```
A DPDT with on-off-on state is a 3PDT switch without the thrid pole wiring sticking out :smile:
```

---
## \#31 Posted by: longhairedboy Posted at: 2016-02-08T19:32:33.347Z Reads: 273

```
speaking of BMSs... i think i just found the mysterious 50amp space cell BMS on ebay. there's also a 44.4v (that's 12S folks) version on there as well. its $30 USD.

http://www.ebay.com/itm/37V-42V-10S-50A-Lithium-ion-Li-ion-LiPo-NMC-Battery-BMS-PCB-System-Ebike-36V-/121812804086?_trksid=p2141725.m3641.l6368

this makes me want a spot welder BADLY. I've already found LG HE2s for less than $5 each, which means you can build a 12S 4P for almost $100 less than a space cell retails. 

Sorry, didn't mean to derail the thread with my stream of conciousness. Please continue...
```

---
## \#32 Posted by: lox897 Posted at: 2016-02-09T07:16:48.473Z Reads: 258

```
Hey @longhairedboy 
Where did you find those LG HE2s?
JP Spot Welder looks like a good option or if you want to only use 0.15mm max Sunkkos are good.
```

---
## \#33 Posted by: longhairedboy Posted at: 2016-02-09T12:01:59.803Z Reads: 256

```
liionwholesale.com 

http://liionwholesale.com/collections/batteries/products/lg-he2-18650-battery-genuine-tested-20a-2500mah-flat-top-wholesale-lot?variant=1038173256&refer1=adw&campaign=he2wholesale&gclid=CNyvmKTQ6soCFUUfhgodokUBmw

they have other cell types too, very interesting high capacity cells that might be worth exploring.
```

---
## \#34 Posted by: Pablo_702 Posted at: 2016-06-28T23:53:24.915Z Reads: 211

```
im asking around the same question. how did you permanently fixed thos econector to your enclousure? im trying to see if theres any other ideas besides epoxy
```

---
## \#35 Posted by: Kaly Posted at: 2016-06-29T01:55:48.916Z Reads: 218

```
I use epoxy for fixing the connectors, what you need to do is create a base for the epoxy not to separated from the enclosure. 

My process is like this, I have 1/8 thick abs and create a 3 layer base plate with an U shape where I can stick the connector, shown here made out of foam to illustrate <img src="/uploads/db1493/original/2X/c/ce1bba2b5feb2fc43ebed290ba7672de21faa619.jpeg" width="690" height="388">

I cover each layer with the epoxy so they can form a strong base for the connector and stack them onto the connector in this manner. 

<img src="/uploads/db1493/original/2X/a/a827a4cf3fa524743895677c9f35e2b3fa23f866.jpeg" width="690" height="388">

<img src="/uploads/db1493/original/2X/d/dcafa9bfaec57efa4cb71f91d28759cf1d8b0cbf.jpeg" width="690" height="388">

So in short.
- make the orifice where you want to position the connector. 
- make 3 base plate out of abs plastic with a opening for the connector, remember to sand the surface for better adhesion. 

- position connector and use tape on the terminal side to prevent epoxy from getting in. 

- apply 5 min epoxy to connector and to baseplate one at the time. Be generous with the epoxy. 

- hold in place for 5-6 min until epoxy sets and you are done. 

For the balancing ports. 
- make a groove on the location you want to position the port. Make sure is just the same size of the wire flaten together. 

- cut the wires and insert them through the opening and solder the wires on the other side. 

- apply a little bit of epoxy to the wire and the opening and push the connector onto the epoxy, covering the opening and fixing the connectors in place.

 <img src="/uploads/db1493/original/2X/e/e6b21fa0c14a4ea8c3d83299431e71b23141a9fa.jpeg" width="690" height="388">
```

---
## \#36 Posted by: Pablo_702 Posted at: 2016-06-29T02:00:11.991Z Reads: 213

```
Thank you i will try this
```

---
## \#37 Posted by: paulus_germanus Posted at: 2017-03-25T17:09:36.404Z Reads: 129

```
[quote="Kaly, post:3, topic:1261"]
IMG_7002.JPG2448x3264 1.22 MB
[/quote]

These wheels are massive and beautiful, Bro - could tell me the name of them plz so that I could find myself some? I'm asking cuz ima new to the esk8 game. Thx a million
```

---
## \#38 Posted by: Kaly Posted at: 2017-03-25T20:12:58.267Z Reads: 130

```
This is the link 
http://shop.mbs.com/accessories-492/mountainboard-wheels/mbs-all-terrain-longboard-wheels.html

Currently not a available
```

---
## \#39 Posted by: paulus_germanus Posted at: 2017-03-25T22:10:29.783Z Reads: 122

```
Awesome! Thank you! I'll keep looking and eventually find them somewhere :slight_smile:
```

---
