# Lion &#124; Sk3 6374 192kv &#124; 10s2p 25R battery &#124; 90mm 33T/14T &#124; VESC

### Replies: 23 Views: 1757

## \#1 Posted by: usual Posted at: 2017-04-12T19:47:34.244Z Reads: 194

```
Now it's finally time.
I'm not completely sure, if I forgot something or if the wiring is right.
 Soooo... here are my parts:

Board
* Deck:[ Jucker Hawaii New Hoku Flex 2](https://www.juckerhawaii.com/JUCKER-HAWAII-longboard-komplett-NEW-HOKU-Flex-2)
* Trucks: Caliber II
* Wheels: 90mm 74A Stickies

Motor
* [Sk3 6374 192kv motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html)
* Carbon Motormount 
* 40T/15T Pulleys
* VESC
* 10s3p 18650 HE2 Li-Ion
* [LCD: TE619](http://www.ebay.de/itm/12V-Batterie-Tester-Kapazitat-LCD-Panel-Blei-Saure-Acid-Akku-24-36-48V-TE619-/262845284281?hash=item3d32ccbfb9:g:hx8AAOSwB-1YnMPp)
* [Charger](http://www.ebay.de/itm/Ladegerat-Netzteil-Charger-42V-2A-fur-36V-Pedelec-E-Scooter-mit-Rundstecker-/282274916160?hash=item41b8e56740:g:NjAAAOSw-4BXbPmN) + [Charging Port](http://www.ebay.de/itm/Mini-Xlr-3-Pin-Audio-Cable-Steckverbinder-Male-Stecker-Buchse-Female-/331692874590?var=&hash=item4d3a6f9b5e:m:mhnDKZRSb27BxIVOj9UodVQ): 
* Remote: eSk8 Mini Remote 
* BMS

Wiring etc.
* shrinktubes
* 12 awg red/black 1m cable
* 22 awg wires
* Nickel sheets
* XT90s
* 3 x XT60
* Balance Port
* Enclosure



<img src="/uploads/db1493/original/3X/f/1/f188e6eb671fe27341f6e9e26c70825b381bded7.jpg" width="641" height="500">



Couple questions: 
1) Which deck would be better?
2) 33T/ 13T or 14T or 15T?
3) Would 83mm wheels be better for 33T pulley?
4) Is this charger and charger port right? When yes, how do I connect the XLR male Port?
5) How do I charge the battery without a charge port (so the xt60 connectors)?
6) Do I need a Turnigy HV SBEC 5A Switch Regulator? When yes, why and how should I wire it up? 

I weight round about 63 kg how fast would this setup be and what would be the range?
```

---
## \#2 Posted by: TranxFu Posted at: 2017-04-12T19:52:41.226Z Reads: 182

```
That way your LCD will be always on. I'd wire it in after the loop key. Its personal preference but it would bother me if it is always on.

-< 
1. I'd prefer the Hoku Flex :) 
2. & 3. Use one of the many gearing calculator tools and choose depending on your preference. 
4. The charger works. Personally I'd go for a D/C plug. When using those 3 pins just get a diagram and find out which is ground/positive and wire it in. When using a BMS you will have to look for its specific wiring diagram too, to know where to wire the charging port in. 
5. You can also use an xt connector to charge the batteries. Many people here use quality 18650 cells without a BMS and use a regulating charger to charge them up to 41v only. It preserves the cells.
```

---
## \#3 Posted by: usual Posted at: 2017-04-12T21:30:53.615Z Reads: 169

```
First of all, thank u very much!

I think I go 13T, 47,5 km/h doesn't sound so scary compated to 14/15T.

What if I replace the LCD with [this](http://www.ebay.de/itm/Digital-Batterie-Balancen-LCD-Voltage-Akku-Power-Analyzer-Watt-Meter-60V-100A/380950291989?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D41821%26meid%3De5c2bc807d4a4b1daff3240875babf2b%26pid%3D100005%26rk%3D5%26rkt%3D6%26mehot%3Dag%26sd%3D222265153944), looks much nicer to me.

Can you recommend one cheap regulating charger?
I found one for 75 €, are they really so pricey or am I searching wrong? 😒

------------
Or... I'll go with BMS, much easier. Is this [BMS](http://www.ebay.de/itm/10S-36V-BMS-40A-Li-ion-Lithium-Battery-Cell-Protection-Module-Balanced-Charge-/252844029827?hash=item3adeadb783:g:BsAAAOSw4A5YnbzF) right?
```

---
## \#4 Posted by: Smorto Posted at: 2017-04-12T22:17:01.654Z Reads: 157

```
Changing the LCD won't do anything in terms of it being on. What @TranxFu is saying is that the LCD will always be on in your current configuration. I recommend putting it **after** the loop key as well so that way it only comes on when your board is on.
```

---
## \#5 Posted by: SirDiff Posted at: 2017-04-12T23:01:15.517Z Reads: 143

```
Don't go lower than 14 teeth on the motor, otherwise the belt will skip sometimes. If you want more torque and lower speed, just increase the teeth on the wheel pulley
```

---
## \#6 Posted by: usual Posted at: 2017-04-12T23:33:18.010Z Reads: 141

```
Thanks for that! I will go 83mm 33T/15T:grin:
```

---
## \#7 Posted by: usual Posted at: 2017-04-12T23:34:19.909Z Reads: 143

```
<img src="/uploads/db1493/original/3X/5/f/5f4908660f92f56e313e55ecf97792e428a3b7f1.png" width="516" height="481">
```

---
## \#8 Posted by: Namasaki Posted at: 2017-04-12T23:39:52.951Z Reads: 136

```
did you already purchase the 25R batteries?
```

---
## \#9 Posted by: Smorto Posted at: 2017-04-12T23:45:57.695Z Reads: 136

```
The one further to the right, **after** the loop key that way it only turns on when your system does.
```

---
## \#10 Posted by: usual Posted at: 2017-04-12T23:50:23.840Z Reads: 134

```
Not yet, I wait a little because of easter.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-04-12T23:57:43.919Z Reads: 131

```
I use Lipos myself but I have heard that 25r cells are bad about voltage sag.
30Q cells are suppose to be better even though there discharge spec seems lower.
```

---
## \#12 Posted by: SirDiff Posted at: 2017-04-13T05:34:07.382Z Reads: 124

```
15/33 will give you a lot of speed though. Can't you add teeth on the wheel pulley?
```

---
## \#13 Posted by: TarzanHBK Posted at: 2017-04-13T09:29:57.336Z Reads: 118

```
another thing to mention is a 10s2p with either 25r or 30Q cells is really low.
10s3p is minimum to go, better is a 4p configuration.
Otherwise your cells will have a hard time and wear out soon.
```

---
## \#14 Posted by: usual Posted at: 2017-04-13T23:07:17.876Z Reads: 98

```
What about HE2 cells? Are they any good? They're pretty cheap tho, and the specs are the same as 25R.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-04-13T23:11:43.188Z Reads: 94

```
I'm not sure but I think from what I've heard that they're better than 25r's
Seems like 30Q are best from what I've heard
Also Like @TarzanHBK said, you can't do a 10s2p with 18650. You will need at least 4p
```

---
## \#16 Posted by: Guacamoleface Posted at: 2017-04-13T23:16:35.232Z Reads: 97

```
Yeah as mentioned before I wouldnt go below 10s3p, Preferly 10s4p. Or if its a space issue it might be worth going with less serial connections for more parallels to increase the discharge rate. Just a thought! 
Not much experience with anything else than my own 10s4p tho..
```

---
## \#17 Posted by: usual Posted at: 2017-04-13T23:19:54.018Z Reads: 96

```
I'm considering 10s3p with he2 or 10s2p with vtc5. What you think, would be better?
The he2's are 1,10€ cheaper per cell than the 30Q's.
```

---
## \#18 Posted by: usual Posted at: 2017-04-13T23:23:04.480Z Reads: 96

```
I go with 10s3p after researching a bit more. Thanks for that!
```

---
## \#19 Posted by: Namasaki Posted at: 2017-04-14T03:31:38.631Z Reads: 95

```
I'm not sure about HE2 cells and I know nothing about VTC5 cells.
If pack size is a concern I would take a look at A123 Lifepo4 cells. 
They are supposedly the real deal with 70a discharge per cell
Full charge voltage is 3.6v so a 12s2p would give you 5ah with 43.2v full charge and 140a continuous current.
They have much higher cycle life than Li-ions as well.
The only other option I know of to have high power in a compact system is with Lipo packs.
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-04-14T09:35:13.145Z Reads: 92

```
He2 or he4 are perfectly fine to use. Esk8.de and chaka are using them
```

---
## \#21 Posted by: willpark16 Posted at: 2017-04-16T01:32:08.254Z Reads: 77

```
I've got some he2 that I can give u for cheap to play around with
```

---
## \#22 Posted by: usual Posted at: 2017-04-16T10:56:53.622Z Reads: 77

```
How many do u have? And how much would it be?
```

---
## \#23 Posted by: willpark16 Posted at: 2017-04-16T17:55:40.892Z Reads: 68

```
30 I can give em to u for 3 bucks a cell?
```

---
