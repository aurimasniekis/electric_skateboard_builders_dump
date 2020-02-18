# Is my schematic right?

### Replies: 14 Views: 1533

## \#1 Posted by: pau Posted at: 2017-05-07T14:08:21.014Z Reads: 125

```
hey,
this is my firt build. 
is ervery thing all right?

what should i do with the 2 negatives wires from the balance wire? nothing? or connect them to the ground?
do i need a anti spark switch?
is that the best switch location in that schematic?
can i use that charger 24V and 4Ah output for 6s lipo



here is my electronic part list.
2x motor 5055 190kv [link](diy-electric-skateboard-kits-parts/electric-skateboard-motor-5055-190kv/)
2x vesc [link](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)
bms 10A charge / 10A discharge [link](https://hobbyking.com/en_us/6s-li-ion-10a-pcm.html?___store=en_us) i want to bypass the bms
2 3s lipo 5Ah or 8Ah [5Ah](https://hobbyking.com/de_de/zippy-compact-5000mah-3s-25c-lipo-pack.html?___store=de_de) [8Ah](http://www.ebay.de/itm/RC-ZIPPY-Flightmax-8000mAh-3S1P-30C-/221559238641)
charger 24v and 4 Ah [link](https://www.amazon.de/Netzteil-Ladeger%C3%A4t-Monitor-Radiowecker-Festplatte/dp/B01I4YDNUW/ref=sr_1_1?ie=UTF8&qid=1494061445&sr=8-)
anti spark switch [link](http://www.hellray.de/shop/#!/Vedder-SparkProtectionSwitch-mit-Sicherung-new-Version-made-by-eSk8-de-kostenloser-Versand-Free-Shipping/p/59817445/category=15255004)
voltmeter [link](https://hobbyking.com/en_us/in-line-voltage-and-amperage-meter.html)

<img src="/uploads/db1493/original/3X/9/c/9c7c43b14c0d5f2c8d78dd391e07564f45547d70.png" width="690" height="424">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-07T15:15:26.316Z Reads: 105

```
Your diagram is showing extra battery cells.
```

---
## \#3 Posted by: pau Posted at: 2017-05-07T15:27:35.801Z Reads: 101

```
why? 
sorry
i dont know what you mean
```

---
## \#4 Posted by: IsTalo Posted at: 2017-05-07T16:09:31.255Z Reads: 94

```
Man, 6s normally have 7 balance cables, 6 for the positive of each cell and 1 for the negative of the battery!
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-07T16:20:34.380Z Reads: 87

```
your volt meter needs two cables going in and out since it's inline. It's also not suitable because it supports 30a current max.
```

---
## \#6 Posted by: pau Posted at: 2017-05-07T17:39:41.345Z Reads: 73

```
hey but there only 6 pins
[link](https://hobbyking.com/media/file/845847974X4580138X47.pdf)
as you can see
```

---
## \#7 Posted by: IsTalo Posted at: 2017-05-07T17:51:48.919Z Reads: 69

```
The first dot is the negative one
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2017-05-07T17:53:43.531Z Reads: 70

```
Like this
<img src="/uploads/db1493/original/3X/7/8/7898d6745efcc893602079718c28241410ebd56e.jpg" width="690" height="253">
```

---
## \#9 Posted by: pau Posted at: 2017-05-07T17:54:16.106Z Reads: 67

```
why do i need more then 30A.
the voltmeter is parallel to the batteries. and the voltmeter has a high internal resistance. the greater the resistance, the lower the current is.
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2017-05-07T17:56:43.870Z Reads: 64

```
This is a power meter, it also measures the current flowing through it, so at >30 battery amps you're going to melt it. How would it measure power with only the voltage?
```

---
## \#11 Posted by: pau Posted at: 2017-05-07T18:17:14.588Z Reads: 60

```
is this one right? [link](http://www.ebay.de/itm/Neu-DC-3-0-30V-Wasserdicht-Blau-LED-Digital-Voltmeter-Spannungsanzeige-Prufer/302174551836?_trksid=p2047675.c100010.m2109&_trkparms=aid%3D555018%26algo%3DPL.SIM%26ao%3D1%26asc%3D43785%26meid%3D95f586563d2b4933b5ce6e81d4b3845d%26pid%3D100010%26rk%3D3%26rkt%3D6%26sd%3D112399282177)
details: 
No power supply required
Measuring voltage: DC 3.0-30V blue
Working current: <20mA
Display: Three-digit 0.4 \ "LED, blue color
Refresh speed: Approx.500mS / time
Highest input: DC 30V (higher than 30v has the risk of burning)
Minimum input: DC 3.0V (below 3.0V, measurement inaccurate or not show
Minimum resolution: 0.01 V (<10 V) /0.1V (> 10 V)
Resolution: 1% + 1 digit
Working temperature: -10 ℃ ~ 65 ℃
Size: about 40mm x 25mm x 23mm (L * B * H)
Mounting hole size: Approx.37 * 20mm
LED Color: Blue color
```

---
## \#12 Posted by: pau Posted at: 2017-05-07T18:40:17.339Z Reads: 50

```
here is an update of my schematic.
but i think it is worng for this type on balancer/bms
<img src="/uploads/db1493/original/3X/b/a/ba780c130f5e95143fb51679a3b2c84a6b47054f.png" width="690" height="424">
```

---
## \#13 Posted by: pau Posted at: 2017-05-07T19:16:52.130Z Reads: 44

```
hmm maybe your schematic is wrong.
as you can see on that picture. the balancewire has only 6 ports. [link](https://hobbyking.com/en_us/6s-li-ion-10a-pcm.html?___store=en_us)

and here is on thread 
where they have the same problem
[link](https://www.electric-skateboard.builders/t/battery-management-system-zippys/10772/67?u=pau)
```

---
## \#14 Posted by: SimosMCmuffin Posted at: 2017-05-07T20:36:17.793Z Reads: 40

```
It has 7 pins on the connector.
B-
B1
B2
B3
B4
B5
B6
<img src="/uploads/db1493/original/3X/1/0/10e0e58e618780dc360791a1e625d93b34708a8b.jpg" width="332" height="270">
```

---
