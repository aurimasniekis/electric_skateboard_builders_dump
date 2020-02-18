# Calling VESC UART Arduino experts

### Replies: 21 Views: 2680

## \#1 Posted by: evoheyax Posted at: 2018-01-03T18:51:23.239Z Reads: 266

```
Trying to get vesc data from the UART port, but I am for some reason getting the same data that it sends for the command.

So for example, a COMM_GET_VALUES command is sent in a packet with this data: 2 1 4 64 132 3 0
And when it detects a packet, it finds a packet with this data: 2 1 4 64 132 3 0
So essentially, I'm picking up the packet I'm suppose to be sending and never getting the right response back. I confirmed with my bluetooth app and I get the same packet sent for the COMM_GET_VALUES command, but I actually get good data back.

I'm using an ardunio Mega 2560, VESC Rx to Mega Tx, VESC Tx to Mega Rx.

Also using this library: https://github.com/R0b0shack/VESC-UART-Arduino/tree/Arduino-Mega-with-debugging-code

I tried the RollingGecko library, but I couldn't get past the many compiling errors, even after many hours of debugging.

Any help is much appreciated!
```

---
## \#2 Posted by: Stevemk14ebr Posted at: 2018-01-03T19:24:35.436Z Reads: 233

```
It may be possible that unrecognized values are echoed back. Perhaps your boad rate is incorrect.
```

---
## \#3 Posted by: evoheyax Posted at: 2018-01-03T19:40:18.392Z Reads: 222

```
I have the buad rate set to 9600 on both the vesc and when I open the serial connection on the arduino. Should I have it set to a different value?
```

---
## \#4 Posted by: Stevemk14ebr Posted at: 2018-01-03T19:41:15.034Z Reads: 217

```
it was just a guess i am not sure, try a few different baud rates.
```

---
## \#5 Posted by: skelstar Posted at: 2018-01-03T19:54:30.698Z Reads: 207

```
Try looking at this library: https://github.com/bastianraschke/ESP8266VESC

I am using ESP32(s) (and/or ESP8266) and I couldn't get RollingGecko's library to compile either (I'm not very good at this stuff and I'm lazy).
```

---
## \#6 Posted by: SORRENTINO Posted at: 2018-01-03T20:01:15.953Z Reads: 191

```
I would try a different value just for shits and giggles. ( 115200 )
```

---
## \#7 Posted by: evoheyax Posted at: 2018-01-03T21:49:14.936Z Reads: 177

```
Tried 115200 on both, but no luck :(

@skelstar Thank you. I'll check it out and try it.
```

---
## \#8 Posted by: ZackoryCramer Posted at: 2018-01-03T23:35:57.570Z Reads: 172

```
make sure you are using UART mode on VESC and the UART band width is the same on the VESC
```

---
## \#9 Posted by: Der6FingerJo Posted at: 2018-01-04T00:39:36.317Z Reads: 167

```
I honestly can't imagine whats wrong with the RollingGecko library. For me it has always been using the example sketch without any problems. Maybe you could try reinstalling arduino?
Also, are you using the latest VESC 6 Branch of Rolling Gecko? It's also for 4.12 HW running 3.x firmware.
```

---
## \#10 Posted by: evoheyax Posted at: 2018-01-05T01:10:54.749Z Reads: 150

```
I'm not trying th latest branch, I will try that.

With the RollingGecko, first I got this:

Arduino/libraries/VescUart/VescUart.h:45:21: fatal error: arduino.h: No such file or directory #include "arduino.h" 

Then, If I removed that include, I get:

Arduino/libraries/VescUart/VescUart.cpp:18:
Arduino/libraries/VescUart/local_datatypes.h:25:2: error: 'boolean' does not name a type
boolean valUpperButton;

I tried changing that to bool, and I got some other error.
```

---
## \#11 Posted by: Stevemk14ebr Posted at: 2018-01-05T01:33:36.991Z Reads: 140

```
you can't just remove includes. You need to figure out why that include wasn't found, it should be installed with standard arduino installation. Unfortunely in C solving one error can allow the compiler to get further along until it hits an error it didn't before, so playing bug wack-a-mole is not the right strategy.
```

---
## \#12 Posted by: evoheyax Posted at: 2018-03-28T23:44:59.500Z Reads: 114

```
Still trying to get a library to work.

I think my wiring is the issue.

Currently, I am trying the RollingGecko library to work again. But all I get is "Failed to get data".

Baud rates are both 115200 on vesc uart and arduino serial. Using a mega, with Searial1 for the VESC connection.

I'm just linking Rx to Tx and Tx to Rx. Do I need to connect any other cables? I tried with firmware 2.16 and 2.54, neither work.
```

---
## \#13 Posted by: evoheyax Posted at: 2018-03-29T00:40:13.272Z Reads: 111

```
So finally figured it out. Hopefully this helps others with the same issue. You need to connect the ground of the uart to the arduino ground, in addition to the tx->rx and rx->tx.
```

---
## \#14 Posted by: Kal-El_basically Posted at: 2018-10-31T18:52:51.476Z Reads: 73

```
Hi, Im also new to the VESC community and I was wondering if it was possible to make an arduino controlled VESC using Blynk's APP UI to control the arduino over wifi connectivity (if that makes sense). I know using a phone as a speed controller is a "bad idea" but this is really just a proof of concept and I dont know if I'll be using it in the future. If anybody could help we with figuring this out that would be great.
```

---
## \#15 Posted by: skelstar Posted at: 2018-11-01T19:04:19.852Z Reads: 68

```
Definitely possible. You would have to make a unit that would be on the board connected to the VESC and it would communicate via UART.

Wifi can be a bit flakey... I found (and I've been told I'm wrong) that there was a bit of latency/delay with wifi. Now using nRF24L01 2.4GHz radios (super cheap).
```

---
## \#16 Posted by: Kal-El_basically Posted at: 2018-11-01T20:49:12.647Z Reads: 60

```
My main criteria for the project is using an Arduino and having the board being mainly controlled from my phone. If I use a nRF24L01 2.4GHz radio will I still be able to connect to the Blynk IOS app? I would prefer not to write my own app that allows for full control if I can use Blynk.
```

---
## \#17 Posted by: skelstar Posted at: 2018-11-01T23:59:30.270Z Reads: 59

```
Blynk (or at least your phone does) needs Wifi. The nRF, is that what your remote is using? You can out the VESC into PWM/UART mode and control it and talk to it using Arduino. Fairly certain that is right.

Is that what you mean?
```

---
## \#18 Posted by: Kal-El_basically Posted at: 2018-11-03T16:21:14.873Z Reads: 54

```
I basically want to substitute the nRF24L01 controller with a project on the Blynk app on my phone. My question is will this be possible. If so, how can I combine the Blynk codes with the vesc/uart/arduino codes so the information goes from my phone to the Arduino which acts as a main transmitter to the VESC and in turn controls my motor?
```

---
## \#19 Posted by: skelstar Posted at: 2018-11-04T05:47:09.335Z Reads: 51

```
I'm finding it difficult to understand everything you've explained.

To put it simply: you could have your phone (Blynk) talk to an Arduino (connected physically to the VESC, on the board) which can (at the same time) talk to the VESC and pass on the commands/information that originated in the Blynk app.

So technically possible. I'm sure I had a play with doing this at one stage.

You're going to have to work out how to do this by experimenting TBH.

hint: get an ESP32 if you don't already have one. Aliexpress.com, TTGO store.

Have fun!
```

---
## \#20 Posted by: Kal-El_basically Posted at: 2018-11-05T17:22:05.736Z Reads: 45

```
Thanks for the feedback. Btw, what makes you recommend an ESP32 over an arduino, Im unfamiliar with board so what specifically would make it "better" for my project?
```

---
## \#21 Posted by: skelstar Posted at: 2018-11-05T17:25:05.939Z Reads: 46

```
ESP32 is an Arduino compat board. It's very fast. Built in Wifi/Bluetooth, multiple UARTs. Lots of features... and it's _dual core_ (which you may not need), which means it can run two separate threads (google ESP32 FreeRTOS).

It's a bit of a step up. Maybe get comfortable with getting what you want done on something you're familiar with and then look at implementing on an ESP32. Maybe.
```

---
