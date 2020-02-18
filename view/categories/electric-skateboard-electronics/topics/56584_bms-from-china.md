# BMS from China?

### Replies: 13 Views: 769

## \#1 Posted by: pedro Posted at: 2018-05-24T10:30:26.676Z Reads: 159

```
Hello, i want know if bms from china (aliexpress, ebay, banggood) is good enough for electric skateboard.
and if you have do you have some problems?

thank you for yuour time ;)
```

---
## \#2 Posted by: Slak Posted at: 2018-05-24T10:52:07.298Z Reads: 158

```
Several times, I have read on this forum something like : "You can buy a cheap power supply but always take a good BMS anyway".

My own experience :
1) I bought a BMS from aliexpress last year (20 euros), it worked for a long time but then I used it a bit harshly (outside of the skate, without any case, so totally my fault I guess) and a resistor burnt.

2) 2 days ago, I ordered a cheap BMS from ebay just because I need one quickly but after the event I need one for, I will buy a good BMS from Bestech or BatterySupport.

My advice : Get a good BMS :)
```

---
## \#3 Posted by: rojitor Posted at: 2018-05-24T10:55:34.420Z Reads: 146

```
It is not a Matter of stores. Aliexpress has a lot of garbage and also very good bms. Depends on the model/manufacturer/seller...
```

---
## \#4 Posted by: pedro Posted at: 2018-05-24T11:14:59.453Z Reads: 127

```
Thank you, and another noob question, you can control output of bms like voltage and amp, or bms have to be a specific for your type of battery and your xP exemple: 12S1P
```

---
## \#5 Posted by: rojitor Posted at: 2018-05-24T11:35:50.812Z Reads: 118

```
It has to be specific for most cases. Some Smart bms can tweak parameters via pc or phone.
Depends on the bms. 10s 20a 6$ for example.... That's exactly what you've got.
The only choice available is bypass the bms. I do not recommend you that option if you are still unfamiliar with the bms world.
```

---
## \#6 Posted by: Blitz Posted at: 2018-05-24T11:41:05.036Z Reads: 113

```
@Deckoz runs powerful 13s builds and I think he runs like a 20$ bms from ebay.
```

---
## \#7 Posted by: pedro Posted at: 2018-05-24T13:29:47.566Z Reads: 91

```
thank you, i searching about bms. and i understood bms have a limited discharging, so, if the discharging (from battery to vesc) max is 20 A is useless have a VESC with max discharging 80A because my max will be 20A


like this
https://www.aliexpress.com/item/36V-BMS-for-12-series-of-battery-assembly/1196501778.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10151_10065_10344_10068_5722815_10342_10343_10340_5722915_10341_5722615_10696_10084_10083_10618_10304_10307_10301_5722715_5711215_10059_308_100031_10103_10624_10623_10622_5711315_5722515_10621_10620_10814_10815,searchweb201603_25,ppcSwitch_5&algo_expid=6a277655-54b3-4502-bd97-e128b3cbd2a5-0&algo_pvid=6a277655-54b3-4502-bd97-e128b3cbd2a5&priceBeautifyAB=0
```

---
## \#8 Posted by: rojitor Posted at: 2018-05-24T16:27:40.442Z Reads: 80

```
Exactly. That one could be used only bypassing the discharge. Or used like that with a very low performance.  Also make sure you understand the difference between lifepo4 and lipo/li ion.
They have different voltages so they are not compatible. That one you posted is lifepo4. Good for street legal ebikes.
```

---
## \#9 Posted by: Deckoz Posted at: 2018-05-24T16:32:30.956Z Reads: 75

```
I use cheap BMS as @Blitz said. But I bypass discharging, and use them for charge only. 

I don't use discharge bms for various reasons..
```

---
## \#10 Posted by: achatham Posted at: 2018-05-25T13:36:51.976Z Reads: 60

```
@Deckoz I'm new to bms's. I have a $9 bms from china and am really worried about using it.  I actually used this video https://youtu.be/_yrYG5skwvs to help me connect my power switch and vesc to it. Is this setup to bypass discharging? Sorry to sound like a noob!
```

---
## \#11 Posted by: DevinG Posted at: 2018-05-26T00:47:51.307Z Reads: 48

```
Where can i learn more about bypass? i gonna need a 12s  bms soon so i should probably research
```

---
## \#12 Posted by: Aeroquiv Posted at: 2018-05-26T05:16:40.229Z Reads: 44

```
All you got to do, is make sure that your charging wires are connected to the BMS. Either to the C- or the P- on your BMS depending on design, since some BMS's don't have separate charger/VSS ports. Then solder 2 ground wires from your battery to the BMS B- and another to your anti-spark/VESC. Then your P- or C- to charger port.
```

---
## \#13 Posted by: rojitor Posted at: 2018-05-26T13:42:40.885Z Reads: 35

```
Bypass means you take the discharge directly from the battery ignoring the bms. So you can use smaller/cheaper bms at full power.
Example of bypass:
https://youtu.be/yOnGAHu_odw
```

---
