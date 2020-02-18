# 400€ Build &#124; ebay Deck &#124; SK3 149kv 20/28t &#124; 6S Lipo &#124; 150A Car ESC

### Replies: 28 Views: 6666

## \#1 Posted by: Maxid Posted at: 2016-06-07T07:29:04.919Z Reads: 436

```
Hi guys,

after riding my build for a couple of weeks now I wanted to show it to you and get some (hopefully nice) feedback.
It all started with a lot of reading here, on endless sphere and in a German esk8 forum.
Due to limited funds and the not so perfect supply in Germany I basically did as much myself as I possibly could. So I made the mount myself (first out of 12mm PVC and then after it broke out of 10mm aluminium), modified industrial pulleys to fit, used a friends 3D printer for small stuff and put it all in a Tupperware box under a cheap ebay deck.

My goal was to create a commuter board - so size was also an issue. I wanted to keep it as short as possible so that I could still carry it and settled on a 40inch bamboo deck with a 67cm wheelbase. I cut the kicktail off. It has almost no flex - so perfect for this kind of thing. The deck was 34€ including shipping.
https://images-na.ssl-images-amazon.com/images/I/31e-A0N7PhL.jpg

My Hobbyking order then included an SK3 149kv motor, 2x3S Turnigy 5000mAh batteries, an X-Car beast 150A ESC, a Reaktor 250W charger and XT90S plugs -> ~200€
I should have ordered a programming card with the ESC as the settings are not perfect - but it works. I removed the plastic housing and cut the fan to make it silent and reduce the height of the ESC. No problems so far with overheating!

The remote is a badwolf mod GT2B for which I only had to pay for the actual remote -> 25€

As you can see in [my other thread](http://www.electric-skateboard.builders/t/motor-mount-sliding-on-truck-what-can-i-do/3445/25) I had some problems with the selfmade motor mount but this should be solved now.

The pulleys and the belt I got from industrial supplier [hug](http://www.hug-technik.com/shop/).
I [calculated](https://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii) the theoretical top speed and settled on a 20/28t gearing.
To fit the motor shaft and the 80mm Kegel wheels I had to use a lathe and drill press. Basically I only made the center holes wider and drilled 5 holes in there for M6 screws to hold the wheel. M6 fits through the kegel rim without any drilling necessary. A grub screw holds the motor pulley in place with a filed flat spot on the shaft -> ~14€ for 9mm belt and both pulleys

For the longboard parts I settled on the popular stuff: 44° 180mm Caliber II trucks and Orangatang 80mm wheels -> 118€

This brings the total to ~400€.

Over the weekend I put a [battery indicator](http://www.ebay.de/itm/Digital-LCD-Indicator-Battery-capacity-Tester-F-Lead-acid-Lithium-Cell-LiPo-12v-/281522190751) in there as well which works quite nicely with the semi transparent plastic lid of the box.
For the electronics I put a selfmade 2x3S y-cable in and connected the balance leads to a selfmade D-Sub 9 connector (similar to what @oriol360 showed). That way I still have to open the case to charge but it is less of a hassle. Range is ~10-15KM - at full speed obviously less but I have only ever ridden it once at its top speed of ~40km/h (38 according to the GPS but the batteries were already a little lower than 4.1V at the time I reached that). I charge them as soon as they drop below 3.7V and up to 4.1V at 0.5C to keep them healthy.

For a power switch I was lucky that the Beast ESC has its own small switch. I cut the red +line and soldered a [flip switch](http://www.ebay.de/itm/Wippenschalter-I-0-Kippschalter-Taster-Rocker-Switch-Druckschalter-Snap-In-/161792271522?var=&hash=item25ab9224a2:m:m6pX0DnO-TvMKfp_8cpExlg) in series that I could place through the box. this is also where I connected the voltage meter (the ESC switch lines are provided with the full battery voltage :thumbsup:) so that it does not drain the batteries when the board is turned off.

<img src="/uploads/db1493/original/2X/8/8a89a123a6806597b5698be12c5634a19514c410.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/e/ee59e10f0154f43ac3eb98aa51209356eb130fdf.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/9/94b32487f358db37204143646e80efe949589f65.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/4/4063956ba52d718144c14c0475de7bc4068b3b65.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/b/b2d4c2335b5cd59d006fd7e8acc330eb298859cc.jpg" width="375" height="500">
```

---
## \#2 Posted by: BoardAdmin Posted at: 2016-06-07T08:12:10.860Z Reads: 382

```
Nice Board! 
Where in Germany do you live?
```

---
## \#3 Posted by: Maxid Posted at: 2016-06-07T08:13:11.185Z Reads: 380

```
Thanks!
[quote="BoardAdmin, post:2, topic:4386, full:true"]
Where in Germany do you live?
[/quote]
Close to Stuttgart.
```

---
## \#4 Posted by: BoardAdmin Posted at: 2016-06-07T08:14:17.340Z Reads: 365

```
Me to, i live very close to metzingen and Reutlingen
```

---
## \#5 Posted by: flatsp0t Posted at: 2016-06-07T12:17:24.893Z Reads: 351

```
Hey, i am from Schwäbisch Gmünd
```

---
## \#6 Posted by: flatsp0t Posted at: 2016-06-07T12:18:07.029Z Reads: 341

```
Nice work!
```

---
## \#7 Posted by: Maxid Posted at: 2016-06-07T18:32:09.282Z Reads: 333

```
@longhairedboy you recommended a similar voltmeter in one of your threads and I was just wondering if you know how they actually compute the capacity. What voltage is "0%" and can one change the thresholds somehow?
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-06-07T18:42:41.186Z Reads: 326

```
as far as i know, you cannot modify them to calculate the voltages differently. But based on what i've seen, they calculate based on the standard thresholds for lithium-ion, which is a 3.6v nominal per cell group. the 18650s i use have a max of 4.2v and a min cutoff at 2.6v, so i expect that's more or less standard and that it falls in line with that. I have seen the meter read 1% when the BMS cuts off power, and it usually takes a little longer past 100% to get the charger LED to turn green, meaning when the BMS cuts off for high voltage. 

All of that is to say they seem to be operating within a safe margin of the cells actual capacity, but all it is is a monitor. Even if they are measuring based on 3.7 nominal such as a lipo pack, the BMS if set to lipo will still cut charge/discharge like it is supposed to, but if you're using them without a BMS, i think you'll be fine because like i said they seem to work within a safe margin and if set correctly will tell you when its time to get off the board and turn it off.
```

---
## \#9 Posted by: Maxid Posted at: 2016-06-07T18:51:17.345Z Reads: 301

```
thanks - was just wondering if there is actually a way to like set them to show 100% at 4.1V and 0% at 3.5V (or similar).
But I guess I just have to wait and see and measure how the reading corresponds to the actual voltage.
```

---
## \#10 Posted by: Johan Posted at: 2016-06-09T21:54:47.717Z Reads: 279

```
How did you wire the lcd battery display?
```

---
## \#11 Posted by: Nooby Posted at: 2016-06-10T04:18:12.302Z Reads: 273

```
I am from Kirchheim unter Teck xD
```

---
## \#12 Posted by: Maxid Posted at: 2016-06-10T14:57:56.848Z Reads: 271

```
[quote="Johan, post:10, topic:4386, full:true"]
How did you wire the lcd battery display?
[/quote]

<img src="/uploads/db1493/original/2X/1/1b6dd37700772540e80daab3cd48ca3ccc2ef4b9.PNG" width="690" height="368">
```

---
## \#13 Posted by: Johan Posted at: 2016-06-10T15:21:04.525Z Reads: 257

```
That's really clever! Thanks for the answer.
```

---
## \#14 Posted by: Chilt Posted at: 2016-06-10T20:21:44.669Z Reads: 251

```
Where did you get the remote from? Thanks in advance.
```

---
## \#15 Posted by: Maxid Posted at: 2016-06-10T20:26:48.584Z Reads: 238

```
It is in the text: a badwolf mod gt2b
```

---
## \#16 Posted by: Chilt Posted at: 2016-06-10T20:27:57.121Z Reads: 235

```
Sorry I didnt know what that was :joy:!
```

---
## \#17 Posted by: hexakopter Posted at: 2016-06-10T20:29:26.630Z Reads: 230

```
I think it is this [thing](http://www.hobbyking.com/hobbyking/store/__31671__HobbyKing_174_8482_HK_GT2B_3CH_2_4GHz_Transmitter_and_Receiver_w_Rechargable_Li_ion_Battery.html) in a 3D printed case.
```

---
## \#18 Posted by: offir Posted at: 2016-06-14T10:39:57.588Z Reads: 221

```
how far/distance/time can you skate with these lipo 5a 3c in series?
```

---
## \#19 Posted by: Maxid Posted at: 2016-06-14T11:00:23.455Z Reads: 222

```
[quote="offir, post:18, topic:4386, full:true"]
how far/distance/time can you skate with these lipo 5a 3c in series?
[/quote]

http://www.electric-skateboard.builders/t/ride-time-how-long-can-you-ride/1316/78?u=maxid
```

---
## \#20 Posted by: SFrider Posted at: 2016-07-04T21:50:08.151Z Reads: 198

```
Hi,
I am a new builder/user to this forum and I am very excited to be getting into such a fun project.  I live in SF where there are plenty of hills and weigh about 145-150 lbs and was wondering what components I needed.  I will be running a single motor with the VESC, with 2x 4s 5000mah 20c Lipo in series.  I bought DIYelectricskateboard's 16T/36T motor mount kit as well.  SO what I don't know is what motor I need (been told 230kv is good) and does anyone have suggestions for a comparable but cheaper alternative to DIYelectricskateboard's on/off antispark switch.
```

---
## \#21 Posted by: JLabs Posted at: 2016-07-06T01:08:07.096Z Reads: 182

```
Xt90 anti spark is the way to go. Do a quick search on the forum and lots will come up, I would say almost everyone uses them because it's about $5
```

---
## \#22 Posted by: fc_key Posted at: 2016-07-06T09:03:43.063Z Reads: 178

```
Wuoah such a nice board for such a low price thats pretty awesome :heart_eyes:

I got some question to this project, do you have some ride data like speed and the distance you can hit in one charge? You would help me a lot to build myself a board, what trucks did you use? How stable is the board on a high speed :slight_smile:

Thank you for your answer :raised_hands:

Friendly greetings fc_key
```

---
## \#23 Posted by: Maxid Posted at: 2016-07-06T16:39:04.807Z Reads: 171

```
dude everything you asked for is in the comments or text.
I linked to the distance for a charge just two posts above yours.
Also the trucks are specified in the initial post (Caliber 44°).
Top Speed is 40km/h and it is pretty stable (although I can not compare to other boards)
```

---
## \#24 Posted by: offir Posted at: 2016-07-11T13:50:05.976Z Reads: 158

```
thank you maxid!
```

---
## \#25 Posted by: Mossi Posted at: 2017-08-02T09:29:33.431Z Reads: 59

```
Hey nice board! I have basically the same setup but without the extra switch and volt meter, which I just got in the mail but now I'm wondering about how to wire the switch. I thought you should wire it up in parallell to the esc switch? But you say that you connected both + and - from the new switch to the red esc wire? How does that work? A bit cofused about what is what since the esc has three wires.
```

---
## \#26 Posted by: Maxid Posted at: 2017-08-02T10:26:50.993Z Reads: 58

```
if you connect in parallel there would be no benefit of having the second switch.
You need to connect in series so that the new switch can actually break the circuit.
The ESC has three wires (GND, POS and a signal wire for the small button). You only want to disconnect the red POS wire as otherwise the current would just travel over the signal line when you disconnect GND.
```

---
## \#27 Posted by: Mossi Posted at: 2017-08-02T10:35:49.852Z Reads: 56

```
Alright, thanks for the fast answer! So both of the new switch wires go to the red esc wire.
```

---
## \#28 Posted by: Maxid Posted at: 2017-08-02T10:45:35.004Z Reads: 58

```
yup you connect them in series to the other switch breaking the POS line just like what I showed in the diagram
```

---
