# \[Arduino Project\] Percentage based voltage display using 16 x 2 LCD

### Replies: 22 Views: 6883

## \#1 Posted by: Okami Posted at: 2017-01-13T23:50:23.340Z Reads: 179

```
Hi there! I started off this topic based on ideas and other info I collected in this thread:

http://www.electric-skateboard.builders/t/ways-to-tell-you-should-start-to-think-about-going-home-voltage-monitoring/

So, anyways, I came up with an idea to use arduino nano and a simple ''voltage divider'' - consisting of 2 resistors for bringing the voltage down. I assume I can be lucky that I still use 6s system, so my max voltage will be only 24.6v (4.1v x 6cells).
 _Not 4.2v, because im not using lipos and I charge li-ions only till 4.1v._
 
So, anyways, **it looks like I will get 0.025v precision? Is this right? Can you @saul or @IDVert3X step in and comment onto this?** 

I derive this 0.025v precision because I've heard you can only use 1024 bit precision when measuring through analog pin. This way, I assume, I need to divide 25v / 1024 = 0.0244 v 

---
The following idea is as follows: **1008 bit will serve as 100%**
(24.6v = 25v - 24.6 = 0.4v )  
(0.4v / 0.0244 = 16.393  bits)

1024 - 16.4 = ~1008 bits

---
The lowest point will be around 3.45v per cell or 20.7v for total pack voltage! In bits, this should correspond to 848 bits. (1024 - 176).

As I can see from this, a big range of bits dont get used up this way, so I might as well use just
a single cell group voltage to determine the left percentage of the battery! 

This way I wont have to do the math so much and I will achieve even better accuracy, even better, it should be possible to use for higher voltages too! Of course, the pitfall is that it relies on just one parallel group of batteries, to determine the whole pack's voltage..

But as I also have a wattmeter installed, I think I wont need a backup plan/voltage meter for total pack's voltage..

--

Ok so I hope that my logic is correct, the hardest part will be to program the lcd.. I will look up some tutorials and will post some more info + some code, once I have researched a bit more

----

On a side note, I also considered it would be cool, if there was a chance to make a **arduino based coulometer / wattmeter,** which collects ah/wh stats and of course, measures current! 

Though, the simple models which are available, seems to be able to measure only up to 3A of power.. way too low for something useful + they use resistors and _perhaps_ dissipate heat as they measure it!

 It was said in the manual of MAX471, that it is possible to use ''external sense resistors''. 
http://www.qsl.net/n9zia/28vdc/MAX471-MAX472.pdf

But im not entirely sure will it be a reliable method of measuring current + what are the limits + cost factor, too!

--

Before that, I still need to make my simple percentage display unit, so wish me luck to finish it and make something useful out of this!

--

Some little background info on voltage measuring for arduino:
http://henrysbench.capnfatz.com/henrys-bench/arduino-voltage-measurements/arduino-25v-voltage-sensor-module-user-manual/
```

---
## \#2 Posted by: IDVert3X Posted at: 2017-01-14T00:02:35.280Z Reads: 149

```
ATMega328P in Nano has 10bit ADC.
That means the value can be between 0-1023.
Value != number of bits.

Using arduino for this is pointless and just makes it bigger. 1602 display is too huge as well. You can just use ATTiny85 microcontroller or something similar and mini oled display. ATtiny has 3 ADC pins that can measure voltage in 10bit resolution. You can measure the current using shunt, but you will need an amplifier to amplify the signal from the shunt. 10 bit resolution might be not enough to cover 0-100A range with precise... So you will need an external ADC with at least 16 bit resolution. Firmware is pretty straight forward, you can either write it in C or in ASM. Or in binary if you are crazy enough. You will need a USBasp programmer tho. You can source this on eBay for 2 bucks.

I will provide more info, recommendations and schematics tomorrow once I get on my desktop. Its uncomfortable to write long text and attach links on a cell phone :)

E: sure you can use arduino instead of the "raw" microcontroller if size doesnt matter and you dont plan making PCB for it ( which you will have to if you want to measure the current as you need a few additional components )
```

---
## \#3 Posted by: Okami Posted at: 2017-01-14T00:20:21.167Z Reads: 140

```
@IDVert3X Cool thanks for input!

Well, I just listed there what was at hand! I would like to incorporate the 16x2 display, as I thought it might be able to offer a lot bars for voltage left, as the display is pretty wide!

Im riding a mountainboard, so I dont need to put inside of the empty space of the truck plate. 

--

I do appreciate the input about going with smaller size, to do the same job! I know Attiny is quite handy but it just comes to the fact I still have not ordered it, no matter how useful it might sometimes be!

--

Im deciding on how much bars / resolution should I choose. Once Im ready with the design of the the lcd display functions, I will update. 

thanks for clarifying once again! Ok so 1023 is not bits but just values! A bit rusty with arduino, so I hope with the help of you guys I will make this possible!

I also intend to include some mild audio signals for signaling when battery is at certain voltage.. Will have to think about it more as I have to consider the voltage drop.. so it does not beep / sound all the time to get annoying..

--

Will leave the shunt idea alone for now.. I do hate a bit that for the price of signle 50A shunt, you can get a decent wattmeter/powermeter, which has display, cables and the functionality.. all included in single unit (with case, too)
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-01-14T00:27:48.544Z Reads: 119

```
I would recommed to use arduino because it would be easier to understand for the most here. I also don't like the 16x2 display becasue it has a very limited space. Better would be the SSD1306 that i showed in my video because you could easily programm each pixel and have 21x8 characters space. You could also use a arduino nano which is much smaller or a ESP8266 like a Wemos Mini D1 which would be cheap as 4 dollars. And they come with Wifi. Maybe useful later on. Or go with a fancy ESP32 which would also provide BLE and multiple ADC channels.
So if we want to have all the possibility's i would recommend the ESP32. But the first boards are only out now and the cheapest price you can get is around 18€.
```

---
## \#5 Posted by: Okami Posted at: 2017-01-14T00:34:31.950Z Reads: 127

```
[quote="Ackmaniac, post:4, topic:16067"]
Better would be the SSD1306
[/quote]

Ok, I will look into this and consider can I get anything soon and with a decent price.. Is it hard to program the pixels? The best would be, if there was a seperate program / ''calculator'' to generate the code for the image.. is there such a tool available?

I know how big pain it was to program led matrix manually, so I would like to have some tools available, if I have to program such wide display space alone..

 168 pixels (21 x 8) does sound good.. im not entirely sure how much ''native'' pixels 16x2 had but perhaps there are some other benefits in using oled type display for this..so will definately take a look and also start to plan which display is easier to program for my needs.. wouldnt like to set back this project only because I can get regular voltmeter with some bars for about 5eur / 6 usd..

--

If we go that far (wifi compatibility) then I think it would be a **''must''** to develop an independent gps / accelerometer device, which can log and store some more info, including current reading ability.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-01-14T00:37:20.659Z Reads: 128

```
The pixels are 128x64, With that you can display normal ext with 21 characters and 8 lines.
Hers is the libary for programming.
https://github.com/adafruit/Adafruit_SSD1306
```

---
## \#7 Posted by: Okami Posted at: 2017-01-14T01:42:30.971Z Reads: 120

```
I think for the beginning I will do with 16 x 2

This sort of ''pattern'' would suit me quite ok!

<img src="/uploads/db1493/original/3X/8/7/878e1c3967acfec58e040a104d604857851b41f1.jpg" width="443" height="180">

I might redesign the bar layout / look, but this is how I imagine it could look.

16 bars over ~~1v voltage apmplitude (3.1v - 4.1v) will be quite good I think! 

This should give me an increments of 0.062 (~0.07v), so basically:
3.07 - 3.14 - 3.21 - 3.28 - 3.35 - 3.42 - 3.49 - 3.56 - 3.63 - 3.7 - 3.77 - 3.84 - 3.91 - 3.98 - 4.05-4.11
[1]      [2]       [3]     [4]      [5]     [6]      [7]      [8]     [9]    [10]   [11]    [12]    [13]    [14] [15]  [16] 
---
This way I should be able to see the voltage drop quite accurately too!

I just want to figure out what to do with the percentage.. 

I dont want **that percents / % numbers ''jerk'' around all the time**, perhaps the percentage could be displayed only every minute on the display not constantly like with the graph bars..

Have to come up with a with a way how take load into consideration and show the ''real voltage'' or at least an approx one with some sort of delay..

---
Btw here is a tool to make custom chars for these displays:

http://www.quinapalus.com/hd44780udg.html

---
```

---
## \#8 Posted by: saul Posted at: 2017-01-14T06:37:05.149Z Reads: 99

```
since this is on the board, i think the oled would handle vibration better. less than $10 each for 1" version. and the adafruit lib can do text and graphics already. pretty cool.

a attiny could be nice for a micro meter. but I would use a nano and instead just hook the balance plug to each analog pin, works for up to 8s and you can have cell voltage then calculate a more complete pack voltage.
wait, only 6s with an i2c screen, but 8s with spi :nerd:


to keep the display from going crazy, just need to average the readings  and measure only every few seconds...
maybe have multiple modes so you can see voltage sag when climbing hills.

for range estimate a hall sensor tach like a bike computer should be pretty simple, just need to stick a magnet on the wheel....
```

---
## \#9 Posted by: Ackmaniac Posted at: 2017-01-14T09:23:21.433Z Reads: 93

```
You can get the display here for like 4$.
https://de.aliexpress.com/item/Free-shipping-1Pcs-128X64-OLED-LCD-LED-Display-Module-For-Arduino-0-96-I2C-IIC-SPI/32595045366.html?spm=2114.13010608.0.0.twPcto
```

---
## \#10 Posted by: IDVert3X Posted at: 2017-01-14T11:21:10.567Z Reads: 96

```
No. ATMega328P analog pins can handle only up to 5V, 1S is 4.2V. Second cell vs ground is already 8.4V, this will destroy the microcontroller. You need another circuitry to be able to monitor each cell.
```

---
## \#11 Posted by: Okami Posted at: 2017-01-14T11:55:14.663Z Reads: 99

```
I think with six analog pins it is possible to monitor each cell group of 6s battery. So i think this is not as bad idea..

Dont know will I implement this but will see.

As for the display durability - i think lcd is fine, i will probably try to find or make an enclosure for it. My wattmeters lcd display.is doing just fine with its enclosure.

I know that oled display would offer some more possibilities but for now I think I could leave its use for remote controller with a display and also speedometer functionality.

I really would love to see a community developed standalone speedometer for eboards. I know some ppl have done this along with vesc but would be great to make the same for regular escs. Mountainboards are especially in this zone right now, i think.
```

---
## \#12 Posted by: IDVert3X Posted at: 2017-01-14T12:17:53.543Z Reads: 86

```
The voltage between ground and 2nd cell is 8.4V which is more than 5V limit of ADC. 3rd cell is 12.6V, much more than 5V limit. You will need comparators if you want to monitor more than just a first cell.
```

---
## \#13 Posted by: Paulf Posted at: 2017-01-14T12:48:44.336Z Reads: 89

```
I've been monitoring the first cell for a while and it works just fine
Otherwise you just need a few resistors in order to make tension bridges 
The only thing is that with this approach, you'll need to cut ground in order to turn off your board otherwise you might damage your mcu
```

---
## \#14 Posted by: Okami Posted at: 2017-01-14T13:28:49.715Z Reads: 84

```
Got your point now.. somehow forgot in this manner that ''safe'' voltage is only for the 1st parallel group.. after that (2s) the voltage is 8.4 at max.. as you say
```

---
## \#15 Posted by: Okami Posted at: 2017-01-14T14:13:00.757Z Reads: 76

```
How do you ouput the voltage you get? Do you use a display or just simple leds?
```

---
## \#16 Posted by: Paulf Posted at: 2017-01-14T18:20:49.132Z Reads: 67

```
I've done both
On my first board u had a single led a the front and the speed of the blink was telling me what de percentage was
That was very nice because you can see the led while riding
On my second board, I've used the exact same 16 by 2 display you have.  its really cool too because I've added max speed, distance,  voltage, Ah drawn, everything...  and I can choose what I want to see with my remote
The only downside is you can't see all this data while you're riding because its under my board and even if it was on top, it would be way too small...
```

---
## \#17 Posted by: Okami Posted at: 2017-01-14T20:36:40.349Z Reads: 66

```
Sounds cool. I assume u used vesc to get telemetry (speed) and other data (ah drawn) right ?

What connection did you use? (Bluetooth) ?
```

---
## \#18 Posted by: Paulf Posted at: 2017-01-14T20:56:03.842Z Reads: 77

```
I had no vesc on my first board so I just used the first cell of my battery,  a resistor and the analog input of an atmega! 
On my current board I'm using uart between the vesc and an atmega in order to retrieve all this telemetry 

I think both the methods I've used are fine but there serving different purposes, if you just want something easy and that just works, a led on top of the board and monitoring the battery percentage with the first cell voltage is perfectly fine

If you want to be able to access all the data without having to connect your phone over Bluetooth or anything,  an atmega,  uart with the vesc and a Lcd screen is real cool!
```

---
## \#19 Posted by: Okami Posted at: 2017-01-14T21:08:00.246Z Reads: 83

```
@Paulf  So for vesc based output screen - did you wire all of it up? I did not quite get the idea I think - did you have an oled screen on the front (for telemetry / spent wh) and then with the remote you were able to switch the data on the screen? 

Or the screen was on the remote itself?

If you got any pics, would be cool to see how it looks! If you still have them and are willing to share!

Otherwise.. I understand you get info from vesc through uart then to arduino (all wired, not wireless I assume) and then you output to the screen.. I did not quite get the idea how exactly are you able to switch the mode on the screen with your remote :) do you just use a channel on the receiver for receiving a signal and then you send it to the arduino through wires?
```

---
## \#20 Posted by: saul Posted at: 2017-01-14T21:12:12.228Z Reads: 77

```
yes, but you can just have a voltage divider for each cell. resistors are cheap.
```

---
## \#21 Posted by: Paulf Posted at: 2017-01-14T21:18:11.995Z Reads: 81

```
<img src="/uploads/db1493/original/3X/b/d/bd8c70f19d52b0c71dfeae15c66c671a3d06f637.jpg" width="375" height="500">
(scrap enclosure for now...) 
So im indeed retrieve g the data as you said 
The things g is that I've also made a custom Co t roller with you can check here http://www.electric-skateboard.builders/t/how-do-build-a-wii-nunchuck-remote/4508/19?u=paulf
This remote involves another atmega on my board which gets data from the remote and sends instructions to the vesc through ppm but which also sends left/right commands to my oder atmega (the one retrieving telemetry from the vesc and driving the lcd)  with changes the info displayed according to the instruction received
I guess this could be more easily doable with only one atmega retrieving data from the vesc, driving the Lcd and getting Inputs from the second channel of a remote... 
I'm quite bad at explaining... I should make a diagram when I get time...
```

---
## \#22 Posted by: Okami Posted at: 2017-01-14T23:15:20.989Z Reads: 73

```
Ok, will have to look into this (making your own controller) at some later point in time!

Anyways, quite a good project! Im glad you have done such a thing at such age already :) I found about electronics only when I was about 19-20yrs old anyways..

So far I understand that you just have there more than a couple (2+) arduino's on the board, doing all the communication/function work for you :)

--

As for the project itself (lcd display + battery voltage monitor) I hope to get something working tomorrow, not sure how far will I get but will try to come at least with some results..
```

---
