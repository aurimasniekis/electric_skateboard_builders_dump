# Need Help finding/deciding parts - Project FrozenFury

### Replies: 13 Views: 1204

## \#1 Posted by: FrozenFury Posted at: 2016-08-08T07:07:58.458Z Reads: 147

```
[1.	Deck – 106.99 (Bamboo Raven)](http://www.funboxdist.com/store/completes/)
•	Material: Bamboo / Hard Rock Maple
•	Length: 38″ x 9″
•	Wheel Base: 25.75″
•	Type: Top Mount Double Kick
•	Trucks: 180mm Black RKP Trucks
•	Wheels: 70mm 80A Longboard Trans Blue Wheels
•	Bearings: ABEC 9 Bearings w/ Spacers
•	Hardware: 1.25″ Skateboard Hardware
•	Grip Tape: Black Super Grip Tape

[2.	Motor – 79.26](http://www.hobbyking.com/hobbyking/store/__35029__Turnigy_Aerodrive_SK3_6364_245kv_Brushless_Outrunner_Motor_US_Warehouse_.html)
•	Turnigy Aerodrive SK3
•	245kv Brushless Outrunner Motor

[3.	Motor Mount – 72.99](http://miamielectricboards.com/shop-1/enertion-motor-mounts)
•	Enertion Motor Mount

[4.	Battery – 108.00](http://www.hobbyking.com/hobbyking/store/__14083__ZIPPY_5000mAh_3S1P_20C_Hardcase_Pack_.html)
•	ZIPPY 5000mAh 3S1P 20C Hardcase Pack (4)
•	Balance Plug: JST-XH
•	Discharge Plug: 4mm Bullet-connector

[5.	BMS – 29.00](http://www.batterysupports.com/22v-24v-6s-30a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-475.html)
•	22V 24V 6S 30A 6x 3.6V Lithium ion LiPo Battery BMS PCM PCB

[6.	Charger – 21.49](https://www.amazon.com/Battery-Balance-Charger-Li-ion-Batteries/dp/B005EF15Q4)
•	iMAX B6 OEM Battery Balance Charger For 1-6 cell Lipo, Li-ion, LiFe (A123), Pb, 1-15 cells NiCd and NiMH Batteries

[7.	Charger Adapter – 11.99](http://miamielectricboards.com/shop-1/ez)
•	Simple Charging Port Adaptor
•	Balance Leads: 4S/6S/8S JST-XH plug
•	Charger Leads: Deans Connector
•	Request XT-90 Anti-Spark connectors and battery leads

[8.	ESC – 70.00](diy-electric-skateboard-kits-parts/single-motor-120a-6s-esc/)
•	TorqueBoards 120A 6S ESC

[9.	Programming Card – 15.00](diy-electric-skateboard-kits-parts/torqueboards-esc-programming-card/)
•	TorqueBoards ESC Programming Card

This is my build as of now. I have a couple of questions that I'm unsure about. 
- What pulleys, timing belts, and other mechanical parts do I need for this setup?
- Where can I find an on/off switch and battery voltage meter?
- What wiring, connectors, or leads do I need (assume that I have the on/off switch and battery voltage meter)? If possible, can you diagram how the wiring would work? 
- Any recommendations on a sleek electronic enclosure?
- Is there anything that I am missing?

Thanks in advance.
```

---
## \#2 Posted by: lox897 Posted at: 2016-08-08T07:50:45.797Z Reads: 128

```
How are you going to use those trucks and wheels? You should get calibers and abec or orangatang (or clones).

Buy belts and pulleys from Enertion. They have the right stuff.

1. You can make your own switch with an xt90 antispark. Look on ebay for the volt meter.
2. 10 AWG for battery and 12 AWG for motor.
Text diagram:
Battery > Switch > Volt Meter > ESC > Motor
3. Check out @psychotiller enclosures
```

---
## \#3 Posted by: psychotiller Posted at: 2016-08-08T12:06:05.720Z Reads: 117

```
I also have mounts that fit the black rkp trucks perfectly.
```

---
## \#4 Posted by: FrozenFury Posted at: 2016-08-08T17:36:17.727Z Reads: 90

```
Sweet! 

Which mount on your website is for the black rkp trucks?
Also which enclosure of yours should I use if I want to put four ZIPPY 5000mAh 3S1P 20C Hardcase Packs in it? The dimensions are [here](http://www.hobbyking.com/hobbyking/store/__14083__ZIPPY_5000mAh_3S1P_20C_Hardcase_Pack_.html)

Thanks!
```

---
## \#5 Posted by: FrozenFury Posted at: 2016-08-08T17:42:53.916Z Reads: 83

```
Do you reccomend that I not buy the complete skateboard and instead buy the parts separately and assemble myself? I was thinking about doing that but it came out to be more expensive than if I just bought the board myself, so I refrained from doing so.

 If I use @psychotiller mounts, would it work with the trucks and wheels from the board I linked?

1. How do I make my own switch with an XT90 AntiSpark? Would [this volt meter](http://www.ebay.com/itm/172143986261?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) work?
2. Can I get [this](https://www.amazon.com/Hilitchi-30feet-Black-Gauge-Silicone/dp/B018GHMME0/ref=sr_1_2?s=car&ie=UTF8&qid=1470677977&sr=1-2&keywords=10+AWG) for the wires? Also where do I put the antisparks in the text diagram and do I need any connectors?

Thanks again!
```

---
## \#6 Posted by: ikjahaa Posted at: 2016-08-08T18:05:18.143Z Reads: 74

```
you don't need a "special" anti-spark switch.
just get a switch that is rated for your numbers.

if you are going 12S total, that would be a switch for 4.2*12=50.4V DC and about 40 to 50 Amps.
```

---
## \#7 Posted by: FrozenFury Posted at: 2016-08-08T18:10:02.106Z Reads: 75

```
If I'm doing 6S total, what anti spark switch would I get? I tried doing the math and googling it to buy the switch, but nothing showed up.
```

---
## \#8 Posted by: ikjahaa Posted at: 2016-08-08T18:17:53.592Z Reads: 76

```
Well, in that case you could use the same setup as me....

I used this switch : 
[DPDT On-Off-On 20A 30V DC switch](http://www.digikey.be/product-search/en?keywords=360-1931-ND) 

<img src="/uploads/db1493/original/2X/3/36ad7d9d357444a85c70cefd078f88084e29dea5.png" width="690" height="278">

This way i split the load across the two poles, 40Amps combined.
Also when I select to charge my batteries, they're cut-off from my esc. ( not entirely necessary thought) If you don't want this feature then you can simply get a DPST switch. ( why Double-Pole ? --> high amp rated switches are indeed hard to find, so splitting the amps make it easier :slight_smile: )

Edit, updated the schema....
```

---
## \#9 Posted by: FrozenFury Posted at: 2016-08-08T19:46:42.941Z Reads: 66

```
Thanks!

Where do I find the poles, and triggers? Also for the wiring, do I use 10 AWG? I'm a complete amateur and don't know where to get these parts. Please help.
```

---
## \#10 Posted by: lox897 Posted at: 2016-08-08T20:13:00.152Z Reads: 65

```
[quote="FrozenFury, post:5, topic:7295"]
If I use @psychotiller mounts, would it work with the trucks and wheels from the board I linked?


How do I make my own switch with an XT90 AntiSpark? Would this volt meter work?
Can I get this for the wires? Also where do I put the antisparks in the text diagram and do I need any connectors
[/quote]

Ask @psychotiller

1. How to make antispark switch: http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
That volt meter will work.

That wire looks good. You will need to change some connectors by soldering. Get XT90 (because you need it for the switch) and 5.5mm connectors. IMO, they are the easiest to solder.
```

---
## \#11 Posted by: ikjahaa Posted at: 2016-08-08T20:37:18.850Z Reads: 62

```
The switch will have numbers next to the connectors, the datasheet will state what connects to what. 
Or even easier, use a multimeter to find the switch states.

Yea 10 awg is  suitable for applications up to 52 amps
```

---
## \#12 Posted by: psychotiller Posted at: 2016-08-09T01:41:52.236Z Reads: 57

```
http://psychotiller.com/product/ripba-axle-set-mount-60 Will work with your trucks, but you are going to find it a little more difficult to use the 70mm wheels. Those are a little small for E-board pulleys.
```

---
## \#13 Posted by: psychotiller Posted at: 2016-08-09T01:46:08.512Z Reads: 56

```
Those batteries are tall...I could make you a custom enclosure for 4 of those side by side for $80, but I don't have a ready made model.
```

---
