# China board remote / remote monitoring mods wifi -arduino(own,meepo,koowheel, etc)

### Replies: 14 Views: 358

## \#1 Posted by: TxFlatRoller121 Posted at: 2018-12-10T18:28:40.332Z Reads: 84

```
anyone used Arduino modules to setup a Wirelss OLED mini screen into there controller? ! . just wondering 
i am thinking about figuring out a way how i could build this out. 
i think i could use 2 arduino nanos along with 2 WiFi module powered by 2 18650 lipos should not be to difficult anyone done anything like this ?
```

---
## \#2 Posted by: skelstar Posted at: 2018-12-10T18:54:30.219Z Reads: 79

```
Don't use nanos + wifi module: look at using ESP32 (or ESP8266) they have wifi built in (ESP32 has BLE too).

Yes I have done it (as have many). I don't use wifi/BLE though, I use nRF24L01 modules (as do others).

There are _many_ threads. _So many threads_.
```

---
## \#3 Posted by: TxFlatRoller121 Posted at: 2018-12-10T19:16:18.163Z Reads: 67

```
i know there are alot of threads for Vesc but i have yet to find anyone who has modded a china controller and integrated a LCD screen screen like i am talking about doing . please link me to a china controller build for ESC and hub motors .
```

---
## \#4 Posted by: skelstar Posted at: 2018-12-10T19:17:50.591Z Reads: 66

```
Fair enough. I didn't read your first post thoroughly enough.

ESP32/ESP8266 recommends still stand though :) (although they won't be as small as a nano but have the wifi built in).
```

---
## \#5 Posted by: TxFlatRoller121 Posted at: 2018-12-10T19:21:48.283Z Reads: 60

```
right on will look into those modules . thinking i will 3d print a test controller 1st and modify based on that. what i plan on trying to do  is a copy the controller housing design and create 1 new 3d printed half of the case that will have the led screen cutout built into it along  and a spot for the modules and small micro lipo battery setup and the cutouts for the oem controller leds and stuff .
```

---
## \#6 Posted by: skelstar Posted at: 2018-12-10T19:27:49.375Z Reads: 50

```
18650s might be overkill. I'm using (I think) 380mA lipos which are fine for a journey (and more probably). They are tiny compared to an 18650.
```

---
## \#7 Posted by: skelstar Posted at: 2018-12-10T19:29:05.143Z Reads: 46

```
This is the controller that I built: https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/5168?u=skelstar ... and only about half of the enclosure is full.
```

---
## \#8 Posted by: TxFlatRoller121 Posted at: 2018-12-10T19:31:54.215Z Reads: 47

```
yeah actually i have a bunch of micro lipos from my tinywhoop( micro fpv racing drones) some 300-and 500 mah. cool remote ya got modded there love me some SNES! what really got me thinking about this was this remote ... which i bet my $ the
 china companies all catch on and the next round of boards and remotes will be like this .. https://www.electric-skateboard.builders/t/solidgeeks-firefly-remote-with-bigger-screen-what-do-u-prefer-on-screen/70221
```

---
## \#9 Posted by: skelstar Posted at: 2018-12-10T19:44:55.247Z Reads: 44

```
I think I have that OLED in the end of my remote (128x32px). Not as much detail though, but I don't want too many things to read at speed anyway.

All the internals of my remote are my own doing though: wrote the code from scratch and there is another module in/on the board that talks to the VESC via UART. _Fun_.
```

---
## \#10 Posted by: TxFlatRoller121 Posted at: 2018-12-10T19:50:57.576Z Reads: 40

```
another build with a mini LCD https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/804. still not a china remote!
```

---
## \#11 Posted by: skelstar Posted at: 2018-12-10T19:59:12.788Z Reads: 38

```
So you still want to use the "China Remote" electronics for controlling, but you want to get the "values" out of it to the display? Or do you plan to read the values from the VESC and transmit to your module in the remote which will display some figures (easier option, but messy)?
```

---
## \#12 Posted by: TxFlatRoller121 Posted at: 2018-12-10T20:07:11.305Z Reads: 38

```
yes exactly i want to be able to get the "values " and transmit them between the 2 arduinos +wifi modules to the display on the controller  that will be the plan. and basically i want to be able to see the battery voltage output,maybe time, and speed ( via hall-way sensor add on) and dont get me wrong ! i know this is kind of extra esp considering all the apps for cycling and stuff easily track all that but still. its good to know
```

---
## \#13 Posted by: skelstar Posted at: 2018-12-10T20:14:02.841Z Reads: 37

```
You could use Wifi. I discounted wifi/BLE in my controller because having a strong/solid/dependable signal for controlling the board is kind of important, but if you're just showing data, then it would be fine. 

You could have an "offline" indicator if the controller doesn't hear from the board for more than 1 second or something.

I'm not sure finding a thread specifically about what you want to do is super important. The threads about remotes that do everything (like the one you linked earlier) are going to tell you what you (I think) want to know.

Trial and error is going to tell you more.
```

---
## \#14 Posted by: skelstar Posted at: 2018-12-10T20:14:46.586Z Reads: 36

```
_ps_ - U8Lib (I think) for a good library to write to the OLED.
```

---
