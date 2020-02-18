# Esk8Lightuino - Arduino for Esk8

### Replies: 16 Views: 2127

## \#1 Posted by: Kug3lis Posted at: 2019-05-05T23:12:20.523Z Reads: 217

```
Hey guys, just finishing working on a small project, which I was wanted to finish for a long time. Originally it was intended just for RGB light control, but because of space requirement I ended up with pretty beefy MCU I decided just to make a board with all outputs and inputs routed out.

Short description this is motherboard for Arduino Pro Micro module which routes out connections and makes it easy to use and connect things together. I am releasing everything open source. Its uses are to connect rf receiver, vesc as inputs for data throttle position, rpm, voltage, current and etc data and use it to control addressable RGB led strips like WS2812, relays, use inputs for temperature, potentiometers, voltage, current or etc... Also connect NRF24 module for remote connection to ur helmet, backpack or etc? Also, you can connect TFT/LCD screens like @janpom DAVega LCD screen and etc things (use ur imagination) 

# Features:

* Powered by Arduino Pro Micro module with USB connection (no usb - serial cables)
* 2 x PPM Inputs
* 1 x UART (VESC connection)
* 4 x 3 pin (IO, 5V, GND) (Used for relays, potentiometers, led buttons, temperature sensors and etc it can be logic input, logic output, few of them can do PWM output and all can do ADC input)
* 1 x SPI + 3 external control pins for LCD additional pins or NRF24 control signals (These pins are also can be switched off and used as normal input/output pins through the main connector)
* 10 x Input/Output + GND pins
* Power supplied by PPM/Uart or 6V-16V input (it powers only MCU everything else will require external voltage converter)

# Software side:

I am going to finish writing library for Arduino which will include PPM reading, VESC data fetching, all the pins defined as constants no reverse looking and few other functionalities. Also, I will provide a few sample projects and maybe even code generator which would peace code from blocks.

# Hardware:

The board is designed using Kicad the files will be hosted in [Github](https://github.com/esk8lightuino). For those who just want a finished thing assembled or kits will be available to buy from @3DServisas [online store](https://shop.3dservisas.eu) 

![Esk8Lightuino_back|533x500](upload://lS9UqVvaJOT5UdXOWD9EOzjZ66h.png)

![Esk8Lightuino_front|533x500](upload://9QWLNEjGPlbbH6cYWIN3KSsBoD9.png) 

Here are a few other components which would ease playing with this we will try to keep stock of these in store too:

* 5V 3A DC/DC regulator https://www.aliexpress.com/item/1PCS-High-Quality-3A-Adjustable-DCDC-LM2596-LM2596S-input-4V-35V-Output-1-23V-30V-dc/32280431843.html
* Pre-crimped 2, 3, 4 pin connectors https://www.aliexpress.com/item/10PCS-20CM-Single-head-DUPONT-LINE-DUPONT-connector-plug-with-cable-jumper-wire-2-54MM-PITCH/32906121697.html
* Relay board (Control your 12V/24V lights or any other higher load) (uses 3 pin connector) https://www.aliexpress.com/item/Free-Shipping-1PCS-5V-low-level-trigger-One-1-Channel-Relay-Module-interface-Board-Shield-For/32519570562.html
* Arduino Pro Micro (yet to verify if correct & works) https://www.aliexpress.com/item/1pcs-TENSTAR-ROBOT-With-the-bootloader-Black-Pro-Micro-ATmega32U4-5V-16MHz-Module-controller-Mega32U4-mini/32849563958.html or if you want trusted one from SparkFun https://www.sparkfun.com/products/12640


# Examples:

Few usage examples:

* Using PPM input from receiver to make a brake lights from WS218 strip controlled intensity and etc.
* Use PPM input and a second channel for Mini/Nano-X for brakes and light turn on
* Use external buttons or button and pots to control different light scenes for multiple RGB strips.

Here are some real-life examples:

Some random RGB strip light patterns:

https://media.giphy.com/media/ef4EzlngZhWzGQZ40x/giphy.gif

Using PPM input for Acceleration RBG lighting and Red brake light. When Nano-X second channel button is held for 5s turn on night mode which turns on "front light relay" and puts the RGB strip into a tail light mode when nothing is done on the throttle"

https://imgur.com/0iCT5kh

I will be posting some more examples later on :) Still trying to figure out how to provide everything as custom Arduino board with libraries integrated but still extending original Arduino core...
```

---
## \#2 Posted by: Kug3lis Posted at: 2019-05-05T23:36:51.913Z Reads: 191

```
Another a bit older example:

https://streamable.com/3xanf
```

---
## \#3 Posted by: MD84 Posted at: 2019-05-06T02:36:49.839Z Reads: 179

```
I like this. The plug and play simplicity is attractive. I set up some ws2812b strips with an Arduino nano. Using the mini remote steering channel as a ppm input to the Arduino. The fastled library is quite good. 

https://youtu.be/KuqDIZko4JQ
```

---
## \#4 Posted by: Resonant Posted at: 2019-05-06T05:03:40.601Z Reads: 159

```
Thank god, brake lights and RGB lights combined. The uses. Finally. And you made it so there were more capabilities than just that... mad. Gonna need me one of these.
```

---
## \#5 Posted by: MD84 Posted at: 2019-05-06T11:48:50.167Z Reads: 135

```
Having the main battery data point available with rgb would be sweet. You could switch to battery indicator mode and have a color gradient showing real time battery state. Green is good orange is meh red is low, flashing red uh oh
```

---
## \#6 Posted by: Kug3lis Posted at: 2019-05-24T14:37:59.145Z Reads: 90

```
I will be ordering prototypes next week for this project.

Here is prototype RGB strip inlay for our enclosure

![image|667x500](upload://9owSPQrnlmfVd0nqA2VRDBT6u12.jpeg) 

Running examples for RGB strip

https://aurimas.niekis.lt/uploads/2019-05-24%2014.20.04.noSound.MOV
```

---
## \#7 Posted by: walleywalker Posted at: 2019-07-10T19:19:10.517Z Reads: 67

```
Bump. This this ever transpire into anything? It's an awesome project

Really looking to learn from the code masters here about how to read and interpret throttle position signals and stuff to an Arduino.
```

---
## \#8 Posted by: Kug3lis Posted at: 2019-07-10T21:45:46.703Z Reads: 66

```
It's kinda in trial

![image|375x500](upload://q0qhmSPTKl5uG6s88Ub3ugQ8bGQ.jpeg) ![image|666x500](upload://3sYBnFWjf8Lf2C9jgHh37p41KAk.jpeg)
```

---
## \#9 Posted by: Kug3lis Posted at: 2019-07-10T21:48:28.357Z Reads: 57

```
For fastled lib it's plenty of space but I tried neopixel with ws2813fx and it's enough just for demo mode 2 strips will thinking make a bigger with esp32 should maybe be enough
```

---
## \#10 Posted by: walleywalker Posted at: 2019-07-17T20:32:19.339Z Reads: 50

```
Any hope that you could impliment this fork into the FastLed library for RGBW strips? 

https://github.com/coryking/FastLED
```

---
## \#11 Posted by: walleywalker Posted at: 2019-07-21T08:16:18.533Z Reads: 41

```
@Kug3lis Will this work with UART controllers or only PPM?
```

---
## \#12 Posted by: Kug3lis Posted at: 2019-07-21T21:00:56.292Z Reads: 33

```
I think anything can be implemented as its simple Arduino base, I have it working for few rides till wire broke of and managed to send 12V back to arduino so my Arduino Micro fried...

I think this can work with both PPM and UART, just don't know right if to use Arduino micro as base as it lacks flash for something bit more useful if you want to do some animations..
```

---
## \#13 Posted by: walleywalker Posted at: 2019-07-21T21:11:49.772Z Reads: 33

```
I see. I suppose I'm still learning. Regardless you should always be able to read the PPM signal (throttle position) from the VESC through CAN by the COMM_GET_DECODED_PPM command right?   This allowing for brake light enabling? 

There is always [this](https://hohmbody.com/flickerstrip/lightwork/?id=790) fantastic generator which kicks out R,G,B signals into PROGMEM which can buy you a bit more memory, or is that what you were already doing?
```

---
## \#14 Posted by: Kug3lis Posted at: 2019-07-21T21:15:21.423Z Reads: 33

```
Oh yeah you can do this static, but I was looking into some dynamic effects like effect speed changing based on throttle position and etc, but you know simple stuff is enough. FastLed with 5 strips was like 40% of flash used without any animation, 2 strips using WS2812FX with NeoPixel lib was like 95%. I even grabbed Fadecandy board for my project just it arrived too late and my project failed so I didn't used...
```

---
## \#15 Posted by: walleywalker Posted at: 2019-07-21T21:25:36.570Z Reads: 32

```
That fadecandy development is insane. I'd never seen that until now. 

That takes some serious programming know-how it appears - That's light-years a head of me.  Cant wait to see the project develop further!
```

---
## \#16 Posted by: Kug3lis Posted at: 2019-07-21T21:59:41.828Z Reads: 30

```
Yeah but fadecandy is just bridge between pc and rgb strip also one channel is max 64 led so I would need to split my strips for board and etc
```

---
