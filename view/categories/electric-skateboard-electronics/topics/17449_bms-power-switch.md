# Bms Power Switch

### Replies: 25 Views: 3670

## \#1 Posted by: IsTalo Posted at: 2017-02-09T16:12:09.692Z Reads: 297

```
Hi, I was looking to buy some mosfets and make my own Power Switch. But I read that some Bms have power switch and I questioned my self, can I put a power switch in my Bms without all that Mosfets and things that have in a Anti-Spark Power Switch? Look at the bms <img src="/uploads/db1493/original/3X/4/e/4e3edef377cd943cf0c7b3d1646d9e2ac4d83b46.JPG" width="400" height="238"><img src="/uploads/db1493/original/3X/b/b/bb60fc124be65486decb78c878de4dc8ac777bba.JPG" width="400" height="299">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-02-09T17:04:26.386Z Reads: 272

```
I don't think so
Besides, that is only 20a BMS. 
You are going to need to bypass it on discharge and use it only for charging.
And by the way, the wiring diagram. 
The numbers on the balance wires are backwards. 
The cells count from the negative side of the battery
1-2-3-4-5 with the red balance wire being cell 6
```

---
## \#3 Posted by: IsTalo Posted at: 2017-02-09T17:19:51.103Z Reads: 260

```
Yeah, but if I put a Power Switch without all that anti spark mosfets, it would work?

Right here is the squematic of the Bms<img src="/uploads/db1493/original/3X/4/2/4272c298a5c055de2889009e7e0e2b27eb68efe3.PNG" width="684" height="500">
```

---
## \#4 Posted by: faithfulpuppy Posted at: 2017-02-09T17:33:04.714Z Reads: 226

```
i hope you're joking, that schematic shows a switch that doesn't do anything except short the battery
```

---
## \#5 Posted by: PXSS Posted at: 2017-02-09T19:07:54.980Z Reads: 214

```
Thats how you turn it off! 
Permanently
```

---
## \#6 Posted by: IsTalo Posted at: 2017-02-09T19:20:25.336Z Reads: 211

```
Sorry, a guy on this forum said to Me do this way, what is wrong? Or are u talking about the Bms Squematic?
```

---
## \#7 Posted by: IsTalo Posted at: 2017-02-09T19:20:55.117Z Reads: 213

```
Why? It will blow my Battery?
```

---
## \#8 Posted by: boards Posted at: 2017-02-09T20:03:05.927Z Reads: 205

```
Consider: if the circuit is closed at your switch, what is the most direct path from the + to - terminal of the battery.
```

---
## \#9 Posted by: IsTalo Posted at: 2017-02-09T20:05:14.872Z Reads: 198

```
I Understand it, but my diagram is correct? The one that is Colored okay?
```

---
## \#10 Posted by: lox897 Posted at: 2017-02-09T22:14:52.435Z Reads: 190

```
It isn't correct. You're connecting the + and - poles together
```

---
## \#11 Posted by: IsTalo Posted at: 2017-02-09T22:18:50.945Z Reads: 182

```
Noooo, positive will pass under the Negative one
```

---
## \#12 Posted by: lox897 Posted at: 2017-02-09T23:52:00.063Z Reads: 173

```
I'm talking about the switch. You are still connecting a + and - together
```

---
## \#13 Posted by: IsTalo Posted at: 2017-02-10T00:48:12.304Z Reads: 169

```
I'm sorry, where I'm doing it, there is no switch in my diagram
```

---
## \#14 Posted by: lowGuido Posted at: 2017-02-10T01:39:40.991Z Reads: 171

```
threads like this make me giggle.

these are the ones that directly precede the "I connected my battery and there was a big spark and now nothing works threads"

and then the "don't buy this switch it killed my battery" threads

seriously.. you diagram is wrong. the "out to switch" causes a direct short of the battery.

smoke then fire.
```

---
## \#15 Posted by: benwong Posted at: 2017-02-10T02:10:28.709Z Reads: 172

```
i think you don need a switch for BMS, but for your ESC.. just a key loop will solve..
```

---
## \#16 Posted by: Pantologist Posted at: 2017-02-10T02:15:09.591Z Reads: 172

```
You have a few options here instead of making it work against all odds....

* Buy an antispark switch
* Buy a smart BMS or BMS with a switch circuit built in
* Make a simple XT 90 loop key
```

---
## \#17 Posted by: Eboosted Posted at: 2017-02-10T07:21:34.547Z Reads: 167

```
@IsTalo, everyone is wrong, the schematic is correct.

They are confussing the "Out-To-Switch" with an "on/off switch", when it's just an switch with positive and negative poles which would to connect to the ESC and then to the VESC.

Here is my diagram if you want to connect the BMS for charging only (recommended)

<img src="/uploads/db1493/original/3X/4/f/4f4a513277df8cc5ebdab90c5925dd0be7bed7f7.png" width="690" height="419">
```

---
## \#18 Posted by: benwong Posted at: 2017-02-10T07:29:50.094Z Reads: 156

```
tat is the greats diagram. 
I think @IsTalo should draw out the whole system. we only know understand "Out of Switch" meaning..haha.  

BTW @Eboosted, i have a problem on integrate BMS to my setup, are you connect balance lead to BMS first or main power wire first?
```

---
## \#19 Posted by: Eboosted Posted at: 2017-02-10T07:53:51.595Z Reads: 155

```
O didn't get your question very well. 

In order to fit a BMS you must connect BMS B- to battery negative, BMS P- to charger negative pole and balance leads to all possitive pole en each pack
```

---
## \#20 Posted by: adilism Posted at: 2018-03-19T09:36:57.379Z Reads: 94

```
Hey guys! So I ordered [this](https://ru.aliexpress.com/item/10S-60A-active-bms-2017-new-Li-ion-smart-bms-pcm-with-android-Bluetooth-app-UART/32827750823.html?spm=a2g0s.9042311.0.0.xKvXyj) BMS from AliExpress for a 10s3p 30Q. I was wondering if it's possible to solder [this](https://ru.aliexpress.com/item/1pc-16mm-Locking-Metal-Stainless-Steel-Latching-Power-Push-Button-Switch-LED-5V-12V-24V-36V/32825467707.html?ws_ab_test=searchweb0_0,searchweb201602_3_10152_10151_10065_10344_10068_10342_10343_10340_10341_10696_10084_10083_10618_10307_5711215_10313_10059_10534_10682_10681_10683_100031_10103_10624_10680_10623_443_10622_10621_10620_10125-normal#cfs,searchweb201603_25,ppcSwitch_5&algo_expid=fd3e0694-9f7c-4f9b-99a6-ac260f4c446e-4&algo_pvid=fd3e0694-9f7c-4f9b-99a6-ac260f4c446e&priceBeautifyAB=0) switch onto it (the 36v version, right?). Also attaching a wiring diagram from the Ali website below. ![10-s-60a-Active-BMS-2017-Li-Ion-Smart-BMS-pcm-Android-Bluetooth-App|600x484](upload://O0otrJZmTSZMbMksdHg7spNG7j.jpg)

Appreciate all the help!
```

---
## \#21 Posted by: Giga Posted at: 2018-04-25T10:47:42.660Z Reads: 76

```
Hey, 
how did it work out?
I am considerating getting a similar one: [12s Smart BMS](https://www.aliexpress.com/item/12S-100A-smart-board-lipo-lithium-Polymer-BMS-PCM-PCB-battery-protection-board-for-18650-Li/32848466970.html?spm=2114.search0104.3.119.7e1e7328SfFYQ2&ws_ab_test=searchweb0_0,searchweb201602_5_10320_10152_10321_10065_10709_10151_10344_10068_10342_10547_10343_10322_10340_10548_10341_10697_10193_10696_10194_10084_10083_10618_10304_10710_10307_10302_10180_10059_10184_308_100031_10319_10103_441_10624_10623_10622_10186_10621_10620,searchweb201603_19,ppcSwitch_5&algo_expid=e0fe8c71-caa0-4e0f-9a69-0a48c7d24286-18&algo_pvid=e0fe8c71-caa0-4e0f-9a69-0a48c7d24286&transAbTest=ae803_2&priceBeautifyAB=0)

Did yours already arrive? 
Could you test it?
```

---
## \#23 Posted by: adilism Posted at: 2018-06-05T14:05:28.366Z Reads: 67

```
Sorry for a long reply. I got the 10s 60a version a while ago and was waiting for the battery pack to be build by local welders. Everything works well, including the app. BMS balances the cells and measures the incoming and outgoing current, as well as the temperature. It also shows each cell voltage separately as they discharge. IOs version is still in development and only does monitoring, but will likely be improved in the coming months. The Android version is a lot more sophisticated, it allows you to program the BMS and cut the power from the battery to the VESC to 0v, supplying power to BT only, so you can power it back without other switches. Although the guys here don’t recommend this kind of switch solution for safety reasons (since there is some current flowing and the battery is not physically switched off), so I will likely be getting a Luna on/off switch as well and use the BT power switch as anti-theft protection.
```

---
## \#24 Posted by: IsTalo Posted at: 2018-06-10T21:54:13.897Z Reads: 59

```
How many balancing pins was in the Bms?
```

---
## \#25 Posted by: adilism Posted at: 2018-06-11T19:22:52.916Z Reads: 47

```
If you mean balancing cables, it has 11, first for the "-", the rest for cells.
```

---
## \#26 Posted by: adilism Posted at: 2018-06-11T19:26:06.035Z Reads: 46

```
Just tried the BMS in-built on/off switch function with beta iOS app and kinda regret getting the luna cycle on/off switch now :smiley:
```

---
