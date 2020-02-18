# Battery Indicator in Controller?

### Replies: 23 Views: 3742

## \#1 Posted by: Raf Posted at: 2016-07-29T17:41:44.987Z Reads: 256

```
Hey guys,

I was wondering if there was a way of indicating how much battery is left in the board, on the controller. Like the boosted board controller. You can see how much battery is left with the lights and i was wondering if this was possible to do with any controller and how does it work?

After seeing this batter indicator, i thought it would look great in a controller

http://www.ebay.co.uk/itm/6v-12v-24v-LED-battery-Alternator-monitor-level-meter-gauge-lamp-indicator-C-/190476821879?hash=item2c594da577:g:1qcAAMXQVERSqKaK


Thanks
```

---
## \#2 Posted by: Hillso Posted at: 2016-07-29T17:55:04.937Z Reads: 246

```
maybe arduino and bluetooth module http://www.electroschematics.com/9351/arduino-digital-voltmeter/

"The analog sensor on the Arduino board senses the voltage on the analog pin and converts it into a digital format that can be processed by the microcontroller. Here, we are feeding the input voltage to the analog pin (A0) using a simple voltage divider circuit comprising resistors R1 (100K) and R2 (10K). With the values used in the voltage divider it is possible to feed voltage from 0V to 55V into the Arduino board. The junction on the voltage divider network connected to the the Arduino analog pin is equivalent to the input voltage divided by 11, so 55V ÷ 11 = 5V. In other words, when measuring 55V, the Arduino analog pin will be at its maximum voltage of 5V. So, in practice, it is better to label this voltmeter as “0-30V DVM” to add a safety margin!"
```

---
## \#3 Posted by: Raf Posted at: 2016-07-29T18:09:42.300Z Reads: 223

```
wow LOTS of detail haha a lot of which i don't understand, will have to read over it a few times. Thanks for this. Do you have a simple/dummy explanation
```

---
## \#4 Posted by: Hillso Posted at: 2016-07-29T18:14:29.174Z Reads: 213

```
2 arduinos and 2 bluetooth modules, 1 arduino on board measuring the voltage and 1 bluetooth module transmitting, 1 bluetooth on remote receiving and arduino displays the voltage on screen \ precentage on leds.

the circuit divides the voltage by11 so for example 55V = 5V
```

---
## \#5 Posted by: Pantologist Posted at: 2016-07-29T18:16:01.637Z Reads: 204

```
How did you get that it divides by 11? From the resistors? 

If you have 12 cells would you divides the voltage by 12?
```

---
## \#6 Posted by: Hillso Posted at: 2016-07-29T18:18:14.585Z Reads: 190

```
It is written in the site:

[quote="Hillso, post:2, topic:6826"]
The junction on the voltage divider network connected to the the Arduino analog pin is equivalent to the input voltage divided by 11, so 55V ÷ 11 = 5V.
[/quote]
```

---
## \#7 Posted by: Raf Posted at: 2016-07-29T19:21:58.533Z Reads: 161

```
i found this on their website....

http://www.electroschematics.com/6868/12v-battery-level-indicator-circuit/

exactly what i was talking about. Just need to research more and figure out how to fit it in a controller haha. Thank you for directing me towards arduino. Had never heard of it before but now i will do as much research as i can
```

---
## \#8 Posted by: Hillso Posted at: 2016-07-29T19:27:59.971Z Reads: 149

```
but your board battery is much higher than 12V
```

---
## \#9 Posted by: Raf Posted at: 2016-07-29T19:33:00.689Z Reads: 146

```
yeah 42V :/
```

---
## \#10 Posted by: Hillso Posted at: 2016-07-29T19:44:38.004Z Reads: 147

```
why not use the circuit in my link?
btw you can also read board voltage on your phone if you use bluetooth module
```

---
## \#11 Posted by: Raf Posted at: 2016-07-29T19:46:52.579Z Reads: 137

```
I still don't really understand this too much. I will read more into the circuits. And i saw the bluetooth phone voltage reader and its awesome, i'd just like a boosted style one on the controller as its simple and looks good :slight_smile:
```

---
## \#12 Posted by: Hillso Posted at: 2016-07-29T19:49:19.728Z Reads: 130

```
the circuit is less importent to understand. if you have questions on the arduino and the bluetooth modules subject I can answer (maybe, i'm just a beginner too)
```

---
## \#13 Posted by: Raf Posted at: 2016-07-29T19:53:47.178Z Reads: 120

```
ahh okay thank you. Its just this is the first time I've ever seen the arduino so i have 0 idea about ti haha but if you have any pages or info sites that will help me understand it better, I'd be more then happy to read them.
```

---
## \#14 Posted by: Hillso Posted at: 2016-07-29T20:07:37.805Z Reads: 120

```
I don't know how to explain, but it's fiarly simple once you have it and trying to play with it. if you want to learn I suggest you to buy [arduino](http://www.aliexpress.com/item/UNO-R3-CH340G-ATmega328P-compatible-for-Arduino-UNO-R3/32523366108.html?spm=2114.01010208.3.1.PmMklK&ws_ab_test=searchweb201556_7,searchweb201602_2_10057_10056_10055_10037_10049_10033_10059_10058_10032_10017_405_404_10040_10060_10061_412,searchweb201603_8&btsid=57f3d899-ba0d-4401-8483-5e47e1c94531) (or [nano](http://www.aliexpress.com/item/Nano-CH340-ATmega328P-MicroUSB-Compatible-for-Arduino-Nano-V3/32572612009.html?spm=2114.01010108.3.11.uQRXAM&ws_ab_test=searchweb201556_7,searchweb201602_2_10057_10056_10055_10037_10049_10033_10059_10058_10032_10017_405_404_10040_10060_10061_412,searchweb201603_8&btsid=1f3bcc56-9a33-4178-905f-2f7d204d7be2))  or one of the [kits](http://www.aliexpress.com/w/wholesale-arduino-kit.html?spm=2114.01010208.0.46.mf7p6r&initiative_id=SB_20160729215721&site=glo&g=y&shipCountry=IL&SortType=total_tranpro_desc&SearchText=arduino+kit) 

basicly you have many ports and you can commend: when port 1 get voltage (button connected to port1) turn on port 2 (port 2 connected to led), so when you press the button the led turns on.

nice English I have

the main code will be something like this: 

if (digitalread(1) == 1) { 
   digitalwrite(2,ON)
   }

pin 1 is button, pin 2 is led
```

---
## \#15 Posted by: Raf Posted at: 2016-07-29T20:41:24.981Z Reads: 115

```
ahh okay, so you get a board and its based on codes that tell it what to do?
```

---
## \#16 Posted by: cjoliver Posted at: 2016-07-29T22:18:12.637Z Reads: 114

```
Battery of controller or the board itself? There would be no practical way of connecting the VESC battery to a microcontroller directly. However the VESC supports UART and gives you the input voltage from the battery, more than enough to tell you your current battery level
```

---
## \#17 Posted by: Raf Posted at: 2016-07-29T22:20:22.684Z Reads: 109

```
no, i would like the battery on the board indicated on my controller. That way i can just check the controller and see how much juice is left in the board
```

---
## \#18 Posted by: cjoliver Posted at: 2016-07-29T22:21:54.209Z Reads: 114

```
Then what I said still helps..

I'm hoping to start a controller project once all my parts come in
```

---
## \#19 Posted by: Raf Posted at: 2016-07-29T22:26:02.894Z Reads: 118

```
ahh nice, what is the project you are doing? this one? 

and with that UART that indicated the voltage, could you somehow transfer this to the controller?
```

---
## \#20 Posted by: cjoliver Posted at: 2016-07-30T02:44:55.665Z Reads: 119

```
This project kinda explores the ideas you're talking about 

http://www.electric-skateboard.builders/t/ultimate-vesc-controller/6014
```

---
## \#21 Posted by: Raf Posted at: 2016-07-30T09:57:32.621Z Reads: 107

```
thank, will check it out
```

---
## \#22 Posted by: Raf Posted at: 2016-07-30T14:35:01.624Z Reads: 93

```
http://www.electroschematics.com/11124/36v-battery-level-indicator/

this one is better
```

---
## \#23 Posted by: vitormhenrique Posted at: 2016-07-30T15:07:51.971Z Reads: 83

```
Quick update, I'm still testing different radios, encryption, data speed communication and reliability. 
I think this weekend PCB is going to be done!
```

---
