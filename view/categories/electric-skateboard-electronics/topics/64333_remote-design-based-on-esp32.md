# Remote design based on ESP32

### Replies: 56 Views: 2902

## \#1 Posted by: dimach Posted at: 2018-08-09T11:27:27.854Z Reads: 252

```
HI Guys,

I'm impressed by the work this community did on creating remotes based on arduino/avr. I like them, but I would like a simpler solution using ESP32. Specifically you can get dev board which basically has everything need but accelerator control.

This is the board 
https://www.ebay.co.uk/itm/ESP32-Development-Board-WiFi-Bluetooth-CP2102-18650-Battery-0-96-inch-OLED/162659059377?hash=item25df3c46b1:g:06QAAOSwn3Vasxcg

For communication we can do UDP over wifi OR ESP supports interesting p2p communication using ESPNow protocol.

I can do coding/3d design/electronics and looking for collaborators on this project.

This could be an easy to assemble and a cheap remote solution.
```

---
## \#2 Posted by: moon Posted at: 2018-08-09T11:58:16.009Z Reads: 236

```
Sounds like a neat idea
```

---
## \#3 Posted by: moon Posted at: 2018-08-09T11:58:54.344Z Reads: 236

```
![image|500x500](upload://nhYg1Vbvp9EdMimPtq0WNX8SV56.jpg)
```

---
## \#4 Posted by: Jc06505n Posted at: 2018-08-09T12:02:11.492Z Reads: 225

```
How strong is the connection as the current problem with most remotes is that they’re either butt ugly , or are susceptible to interference. 

A plain Firefly with only  LED’s and a multi-button would be nice
```

---
## \#5 Posted by: moon Posted at: 2018-08-09T12:07:56.331Z Reads: 214

```
There is a ESP8266 version, is that better? I think someone made a ESP8266 remote before

https://www.electric-skateboard.builders/t/oled-remotes-under-development-please-leave-suggestions/22055
```

---
## \#6 Posted by: dimach Posted at: 2018-08-09T13:44:53.973Z Reads: 195

```
esp8266 is the older version. ESP32 is the new version of this controller and this dev board has battery/charger/wireless/oled/few buttons. Perhaps hall sensor and case is all whats needed. 

I agree stability needs to be tested. My feeling is that using wifi/tcp is a bad choice but UDP should work. The ESPNow is probably even better. I managed to find some reports from RC world.

More testing is needed, hence looking for like-minded people to do it together.
```

---
## \#7 Posted by: dimach Posted at: 2018-08-09T14:45:12.732Z Reads: 186

```
This is funny, but ESP32 even includes a hall sensor!!!
https://techtutorialsx.com/2017/07/16/esp32-arduino-internal-hall-sensor-measurements/
```

---
## \#8 Posted by: moon Posted at: 2018-08-09T14:51:20.682Z Reads: 175

```
Nice sorry I didn't know that ESP32 was the new version :slight_smile:

The dimensions of the pcb, are they a bit too tall?

edit doesnt matter
```

---
## \#9 Posted by: visnu777 Posted at: 2018-08-09T15:05:26.126Z Reads: 182

```
I'm in :slight_smile: 

https://www.electric-skateboard.builders/t/building-stealthy-eskateboards-from-regular-skateboard-decks-mini-logo-paris-truck-dual-diyeboard-90mm-hubs-integrated-enclosure-10s3p-n-e-s-e-2x-flipsky-esc/59906/25?u=visnu777
```

---
## \#10 Posted by: skelstar Posted at: 2018-08-09T17:59:20.347Z Reads: 161

```
I have built my remote using ESP32. Tried ESP-Now, Wifi, BLE but they were all a bit slow (BLE connection was a pain, but worked). Ended up using an ESP32 with nRF24L01. More wires but a lot more reliable.

ESP32 has _two cores_ which I HIGHLY recommend getting you head around. Google "ESP32 FreeRTOS" maybe. I might see if I can find you a link somewhere.

RTOS/dual cores means that you can have one core (or thread?) reading buttons etc (timing critical) and the other core talking to the board... completely independantly. 

I had real issues with how much stuff the ESP32 was having to do, and I was reading a digital encoder at the same time.
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-08-09T18:02:57.711Z Reads: 148

```
You are using MCU resources incorrectly... 8-bit AVR can do all that stuff without even sweating.

P.S. How are you splitting load between cores?
```

---
## \#12 Posted by: skelstar Posted at: 2018-08-09T18:12:28.509Z Reads: 153

```
One core had interrupt handlers on two pins reading a digital encoder. The other core was sending data through the nRF24L01. 

I don't think I was doing anything incorrectly. It was about timing-critical tasks. If the MCU was busy updating a display/sending data then it was missing encoder pulses.
```

---
## \#13 Posted by: skelstar Posted at: 2018-08-09T18:14:48.344Z Reads: 145

```
I'll admit that for "trigger" style remotes that dual-core (FreeRTOS) might be overkill. Still think it's elegant though.
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-08-09T18:17:42.669Z Reads: 150

```
Just to bring in the context, 8051 handles W16 engine, with 4 precision rotary encoders, 16 injectors (PWM based) over 20 sensors communicate through CAN and final nail everything was fit inside 64K rom, 2 external interrupts, and just 2 timers :D 

Check your code for blocks, something is blocking interrupts I don't remember if ESP32 has jtag or etc debugger to see what your code is doing.

P.S. don't use those Arduino style SDK those SDK are just for simple simple task
```

---
## \#15 Posted by: Andy87 Posted at: 2018-08-09T18:22:17.924Z Reads: 137

```
I understand just 5% of what you guys say....but sounds very interesting...continue reading 😜
```

---
## \#16 Posted by: skelstar Posted at: 2018-08-09T18:22:24.984Z Reads: 142

```
Sure. You might be right. I'm a c# developer, not a c++ dev. Dual cores works for me... I like the idea of abstracting tasks away from each other... especially in a hardware sense.

p.s. you're probably right re: Arduino SDK. I fairly short of time so Arduino is just going to have to work for now.
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-08-09T18:23:08.683Z Reads: 143

```
It's easy to develop something on ready made platform :)

Also I think my computer in my Mark48 project is overkill compared to your remote :D
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-08-09T18:25:12.887Z Reads: 132

```
Also lets not forget Apolo 11 Main CPU :joy:
```

---
## \#19 Posted by: dimach Posted at: 2018-08-09T18:31:58.117Z Reads: 139

```
Agree it's strange you had performance issues. 

What did you use encoder for? Did you try to use internal hall sensor for trigger? It's just  adc conversion.

I want to play with ESP now. Someone on arduino forum reported less than ms for packet send/receive cycle ...
```

---
## \#20 Posted by: skelstar Posted at: 2018-08-09T18:40:16.122Z Reads: 144

```
I was going to write a post about the encoder idea but I am using the encoder as the throttle, pulses increment/decrement a counter and the remote talks to the board as a 'nunchuk' remote ... essentially a position-less throttle I guess. 

Might not be the best solution, a few design/safety decisions had to be figured out, but cruising/throttle response is super smooth.
```

---
## \#21 Posted by: Caanon Posted at: 2018-08-09T20:33:25.121Z Reads: 138

```
I actually *just* completed my recently build doing exactly this, except with a pair of ESP8266s. Nunchuck talks I2C to remote box w/[Feather Huzzah ESP8266](https://www.adafruit.com/product/2821) in it. That in turn talks WiFi to board's ESP8266 which checks data packets via CRC, then relays the info to the VESC via UART.

![img](https://lh3.googleusercontent.com/av6N6tu77jWhwycEXpTtE9b-BRQbi_kZmSmgAsvTnkhYD4Nh5jpAeOovvwncxYKVLDYOG_uEYXufsP1fWzN8MkOHA5XfV4jYD5Zo4tp_4bdU9vK1Zqt0JP5ldOc6hrMCBlkUwo2tE-HOqmU9uTKPd1aOTxKBWBeyzr2FPftlFNjFiLadVG46O6yYUs4ZRUwnzeVokQ-EA7r1k_UAZ8EHGzGsRLkoCJCP1IjEqVYM6ZG1otm8UKA3OY-tODI6PbyTKZvonMkxVWfdnE4e1WFm4xeALRC0XvZlGVLX8ThiDZx-Dysa-_0t0yz5a750R2QciLSf3w6ShVI-HbBgqCiXvGD-DEW7R7DkG4lUSVrvP-vkf7Enq6i-ykYeEnlCq3MoArN5wjB1w5Vmeztm1IVmdBVeuTj5uqbt2jLIHsdaHsijCb6IHtd3LCOvZRCwp0-8zk6LWcgeeTRrHcyki8g353FLn9w5dzJZIO-9I7SkENRLZ-RSTfRPAy8A4WUq2I4Y2sHqSTgSS1Dx0KsSqyfbOdz6Ng-Off18X0STJL0nZ49MPgbLeViNwcFXn4KvaxyFELCDBhYdIb0Fmk7ZHlKXAJJfsQ0kg3Vym7mzTOcx=w1533-h2044-no)

![img](https://lh3.googleusercontent.com/92BLQxWC7nr8W9JcxXxTG7t88KcunlxiBlkxkykIo7jRdxAU6oTsBoXGTPpd7SyTfZDiLaJ-VzMaTnKoYnxAP-I53x6z917vgfKJPe5RcRV4qNSkfCBKzoM5hfIoQSnJa8NLhjzA3mwvMfgIniuCSc5WUTxHFbzkQV3BZ_WrzFOVU0TYivk1IUEWHIqej4QYYsBHc5qcow1ngUmQ0qHfeUsoJ1gZaMC7rhcaRQLBDTpXAnnQkWByL2gjf3G9l30dcM8RGgKaMNkdwflwuFh_ZjUQ_NfgI-m-bzNrNBc555ghOXwj_O4uOT3tmRxo3FGmJHIpQDmhUHaoeQhWLfbS4AbgAmbNnQoFFUelw8JIU3KryVL4keoo2fwRcnsLY9OvQ6oHMoSc1jMM3rc-4VIwRZyi5ONoqez2rcJTt2wZLUfwrMXEKjIEZBnXb0xj3y2kEIDYNtme-Uy2u0xAH2BTcXBVWoXesgpnqAxjHMlNmhZUQaqU6toNN9p_bV7I75ydAJWQ5fHEGmcKlWStTX5IsWQw9uh_xxKFW3ilS-D4oxtqhIxEtnfv3-bZsglngnySDph4cnTGBbT9_x6xqZHzcSMHgrR44Kj-e-QPCv1u=w1533-h2044-no)
```

---
## \#22 Posted by: dimach Posted at: 2018-08-09T21:25:35.554Z Reads: 119

```
How is it working for you, Caanon? Responsive, no lags over wifi?

Not sure what you mean by CRC? Do you use tcp socket?
```

---
## \#23 Posted by: Kug3lis Posted at: 2018-08-09T21:35:42.154Z Reads: 123

```
@cannon, if you already using TCP/IP package is not worth double check the integrity of the message as underlying network layer does it for you. It's more for low level communications like UART, CAN, SPI, I2C, Raw RF and etc.
```

---
## \#24 Posted by: Mjkl Posted at: 2018-08-09T21:45:43.160Z Reads: 122

```
If I read this thread correctly you're handling encoder signals as interrupts which is bogging down the Microcontroller and makes it possible to miss pulses when interrupts are deactivated.

It would be better to employ hardware (timer/counter registers) to keep count so you never miss a pulse. Every Microcontroller has these (it also used them to keep track of time with a pulsing crystal) 

On a teensy (nxp Microcontroller) I used for a university project they were called  flextimers and could even decode quadrature signals flawlessly and since it's hardware it's costing you zero computing time to handle encoder input. 

If you look up the manual of manufacturer (usually 2000-3000 pages) of the Microcontroller you will usually find descriptions and application notes on how to do this.

If you still need interupts to handle certain encoder positions you can usually lower the maximum count of the register to a certain integer so the counter with reset on reaching this number. This will trigger an overflow interupts which can then be handled in your code.

I'm on my phone right now but will look into the esp32 manual and point you to the right page
```

---
## \#25 Posted by: Caanon Posted at: 2018-08-09T22:03:19.731Z Reads: 110

```
@Kug3lis Doesn't mean I trust the TCP/IP stack code running underneath :slight_smile: Espressif's code has gotten better in the last few years, but I've hit a number of facepalm-worthy bugs in their SDKs in the past that I'd rather err on the side of caution.
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-08-09T22:04:27.788Z Reads: 107

```
But CRC gives you same face palm protection as espressif could give :D

EDIT: also you code shouldn't depend on one packet ;) You should send at least 10 updates and take some kind of average or etc otherwise you can have spikes on duty which can kill your esc mosfet drivers :D
```

---
## \#27 Posted by: Caanon Posted at: 2018-08-09T22:08:16.972Z Reads: 103

```
@dimach Pretty well, actually. You need to call setNoDelay to disable the Nagle algorithm, otherwise it waits for a larger packet size before broadcasting.
```

---
## \#28 Posted by: Caanon Posted at: 2018-08-09T22:17:19.837Z Reads: 107

```
@Kug3lis Erm... not if you ensure the CRC function is adequately unit tested? And I think you're confusing "packet" with "sample"; you can transmit multiple samples in a single packet. 

Still, agreed that the signal does need to be smoothed: I Kalman filter the received signal board-side before sending it to the VESC.
```

---
## \#29 Posted by: Kug3lis Posted at: 2018-08-09T22:24:38.515Z Reads: 108

```
Nah, I am just saying that CRC is just CRC ;) and I do not confuse packet with sample, in my demo code I am sending values 100th/s to receiver and there doing all calculation of actual value, my code can lose signal, drop packets, invalid packets and etc without a single problem occurring in the end signal. 

So I just calculate throttle position based on calculation and dump live values to the receiver as fast as possible. In the receiver side, I get at least 20 packets, get all the values to apply filtration and safety features and then just send that value to the output. It works nicely on a breadboard, but I think I will be switching to B5 with game controller service or etc using NRF52 MCU :) 

I have worked with many communication protocols, mostly over UART, RS485, RF in industrial applications, so I never trust a packet you wouldn't believe how much trash you can pick up in 5m cable in industrial application.
```

---
## \#30 Posted by: Mjkl Posted at: 2018-08-10T06:07:26.405Z Reads: 109

```
@skelstar

Unfortunately the ESP32 Has no fancy counter module to do for instance quadruture signals straight of the box according to the reference manual.

However, i did find this thread on the esp32 forum if you're interested in pursuing  this

https://www.esp32.com/viewtopic.php?t=4983
```

---
## \#31 Posted by: Skyng22003 Posted at: 2018-08-10T07:48:05.509Z Reads: 107

```
I've been working on a open source electric skateboard platform for a few years now and have designed a encoder based remote based on the DA14580 and DA14583 currently linked up to the skateboard controller running esp32 via Bluetooth, I currently use it as a daily driver, connection is stable but the encryption and pairing isn't sorted out yet.
![IMG_20180810_083851|375x500](upload://ubmwLfXAx2ItruOZrVd3FOBIUDu.jpg)
```

---
## \#32 Posted by: Skyng22003 Posted at: 2018-08-10T07:55:46.361Z Reads: 105

```
![IMG_20180810_084137|375x500](upload://nbUpvFCaZlYBfC4wGc4E1a72cH1.jpg)
Here's an earlier prototype based on the DA14580 with external flash, I'm happy to share the code and schematics, however it's still beta ish. Response times are around 50ms I think. It's using the BLE 4.2 protocol so it's possible to use a 90mAH battery.
```

---
## \#33 Posted by: dimach Posted at: 2018-08-10T08:57:09.306Z Reads: 98

```
What do you use for receiver? ESP32 I assume. How do you power it?

I need to find 10S -> 3.3v converter. Must of them don't go above 36v.
```

---
## \#34 Posted by: Kug3lis Posted at: 2018-08-10T09:16:52.109Z Reads: 96

```
your esc normally provides 5V
```

---
## \#35 Posted by: Skyng22003 Posted at: 2018-08-10T12:04:42.369Z Reads: 91

```
The VCC on the VESC Board should give you 3.3V as the STM32F4 processor on the VESC runs on 3.3v.
Schematic from VESC below, This regulator which takes the regulated 5v generated from the DRV8301 is capable of handling 800ma, which should be enough to power the ESP32
![3v%20diag|470x247](upload://lQuhDUzB6ykwifQR12Qd4WBPqwu.jpg)
```

---
## \#36 Posted by: Skyng22003 Posted at: 2018-08-10T12:14:08.549Z Reads: 88

```
Yeah, so the receiver is a ESP32 and talks to the VESC via UART. On my own setup I use the LT8640 which provides power to the VESC micro-controllers and the ESP32s and can handle up to 42v input and outputs 3.3v up-to 5A.

I have a custom VESC board with a LIPO charger, LT8640 and 2 VESCs, I might create a separate post to see if anyone is interested to test the whole platform.
```

---
## \#37 Posted by: dimach Posted at: 2018-08-10T13:19:32.359Z Reads: 89

```
This is impressive. Do you have PCB built? I'm not that advanced in EE hence I'm looking for easier option)

I've tested built in hall sensor in ESP32 and it works ok. So perhaps that dev board, 3d printed case and couple of magnets is all what's needed for transmitter.
```

---
## \#38 Posted by: Skyng22003 Posted at: 2018-08-10T15:09:13.491Z Reads: 90

```
Thanks, I don't think a hall sensor is a good idea for this application, you can't detect the direction the wheel is going in. The resolution will also not be great, you would need really small magnets and/or a really big wheel. Much better to stick with a rotatory encoder, like the ones used in computer mice. 

How are your soldering skills? I can send you a couple PCBs for the price that it cost to make + shipping.
You would need to solder your own components.

You can then either design your own enclosure or I can get a set printed for you, this will require industrial SLA/SLS printers (I got this done in China), even the SLA printer from Form Labs is not accurate enough and you end up needing to do lots of sanding.
```

---
## \#39 Posted by: ervinelin Posted at: 2018-08-10T15:16:02.009Z Reads: 88

```
I bought the ESP board, just never got down to putting everything together.. If you can do the coding I can try to do up the remote casing... (see my DIY trigger remote thread)
```

---
## \#40 Posted by: dimach Posted at: 2018-08-10T15:49:06.335Z Reads: 83

```
Thanks for the offer. Are there many small components? My fingers are too large for SMD components, but I have decent soldering station. 

I still hope to create something that can be easily put together and if I can pull this off with this devboard it could be easy to replicate.

From my testing if you use two magnets of opposite polarity you can position them above the chip so it gives positive and negative reading depending on the direction. I hope to do more testing next week.
```

---
## \#41 Posted by: Kug3lis Posted at: 2018-08-10T15:51:29.100Z Reads: 75

```
You have two magnets one normal and another flipped so you have one coming with N another with S that's how boosted works iirc
```

---
## \#42 Posted by: dimach Posted at: 2018-08-10T15:52:15.734Z Reads: 75

```
Which one you have? I want to design enclosure for this dev board and fit in trigger with two magnets above the chip.
Don't have much time to work on this until next week and I didn't receive my vesc controllers yet. Though constant failures on my Chinese controller will force me to work harder on this!)
```

---
## \#44 Posted by: Skyng22003 Posted at: 2018-08-10T16:04:56.960Z Reads: 74

```
I see, I was thinking more of a digital counter with infinite scrolling. All of them are going to be SMD components mostly 0603 and some 0402. You would probably need twzeers.
```

---
## \#45 Posted by: Skyng22003 Posted at: 2018-08-10T16:05:42.927Z Reads: 72

```
I see, I was thinking more of a digital counter with infinite scrolling. The one that I made is an infinite scrolling wheel, much like a mouse.
```

---
## \#46 Posted by: Kug3lis Posted at: 2018-08-10T16:08:06.249Z Reads: 72

```
There is already existing one I think it's called Firefly remote or etc with 3d printed case it uses hall sensor, and it's more precise than potentiometer...  I wouldn't much use rotary encoder as you don't have exact position just movement, if you skip some steps you screwed :D
```

---
## \#47 Posted by: Skyng22003 Posted at: 2018-08-10T16:17:14.491Z Reads: 75

```
I don't think you would need an exact postion.

Mine has a safety button, you can only accelerate or brake when you hold the safety button.

When the safety button in not held, the skateboard goes into coast mode, and the acceleration or braking is reset.

Having a infinte scroll wheel means that you don't have to keep the throttle at certain position and is immune to sudden acceleration or braking if your fingers are bumped out of position.

In addition you can also have very fine control over the acceleration and braking, as you don't have to map the throttle/brake to 180 degress.
```

---
## \#48 Posted by: ervinelin Posted at: 2018-08-10T17:03:37.222Z Reads: 73

```
[Mine is this..](https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231)

Never got down to using the esp because my remote works just fine as it is...
```

---
## \#49 Posted by: dimach Posted at: 2018-08-10T17:28:42.642Z Reads: 74

```
Yours is cool! I'm just being way too lazy at connecting wires!)
```

---
## \#50 Posted by: ervinelin Posted at: 2018-08-10T17:55:16.835Z Reads: 71

```
Yup I know the feeling which is why I bought the esp board as well... But I really don't have the time to learn how to code it...
```

---
## \#51 Posted by: dimach Posted at: 2018-08-11T04:46:46.842Z Reads: 65

```
If arduino is used, it's not hard at all. I do plan to use your fw as a base. You guys have done a lot already and this shouldn't be hard to adopt for esp
```

---
## \#52 Posted by: Skyng22003 Posted at: 2018-08-11T08:52:28.074Z Reads: 63

```
The ESP32 supports the Arduino core, so most of the code can be ported directly from the Arduino Nano, even communications like I2C work straight out of the box. Display libraries such as the U8glib also work. The only thing you would need you to get working is the Bluetooth or if you are using the NRF modules there would be no issue as SPI also works straight out of the box. WIFI is a power hog and you don't really need that much bandwidth. I would go for Bluetooth as the NRF modules have no encryption if I remember correctly. I have just managed to get Bluetooth pairing and encryption to work so I can help with that.
```

---
## \#53 Posted by: joshgarde Posted at: 2018-08-12T09:24:05.820Z Reads: 63

```
I just got my ESP32 dev board in the mail this week and I'm currently experimenting with using off the shelf bluetooth game controllers for my remote with the ESP32 as the receiver. It seemed like an interesting challenge for myself and a way to get away with using cheap, easily replaceable hardware (not to mention I have a lot of time to kill waiting for cash for my other esk8 gear). I'm using the ESP-IDF framework and it's been interesting playing around with it.
```

---
## \#54 Posted by: ervinelin Posted at: 2018-08-12T10:25:16.148Z Reads: 63

```
Sounds good.. let me go dig out my board and see how I can design a casing around it
.
```

---
## \#55 Posted by: skelstar Posted at: 2018-08-12T18:17:16.030Z Reads: 60

```
FWIW I'm using the "infinte-scrolling" encoder (if I hadn't mentioned already) and it's true that you don't know what the position is, but as I have it set up as a nunchuk remote, I:
- increment/decrement a value from 127 to -127 (from memory, or was it 0-255?)
- have a deadman switch that if I let it go, the throttle immediately goes back to 0 (or idle)
- if I click the encoder it also goes back to 0
- brakes still work if deadman switch is released
- only clicking the encoder button will 0 if brakes are on

The feature/reason why I am using an encoder is that the throttle is _very_ smooth (depending on the granularity of the mapping of pulses to "throttle steps"). I hated how twitchy potentiometers were in the traditional style of controller. Constant cruise-control FTW.

*It's not "ideal", this won't be for everyone*

I haven't had any moments yet. I spend a lot of time thinking about how to make it safe. You do have to train yourself to take your finger off the deadman switch if you want to brake quickly.

I have a screen (OLED 128x32px) in my remote that shows me board-battery voltage. Next I'll implement some way of changing throttle-response settings through the remote. It will just change the throttle curve.
```

---
## \#56 Posted by: Skyng22003 Posted at: 2018-08-16T20:16:59.544Z Reads: 53

```
Been working on the code for this ESP32 remote coded on the ESP32 Arduino Platform 

I've now got passcode pairing to work with MITM support see photos below

The only inconvenience right now is the first time a remote is paired with a receiver, you would need to enter the randomly generated passcode on the receiver over a USB connection over serial. This only has to happen once as the pairing keys are stored in the ESP32 flash which will survive a reboot/power down but not a firmware flash

Going to try and get navigation working with magnet and safety button as input

Let me know if there are any specific requests? Is the plan to just have one button?

![IMG_20180816_205835|666x500](upload://4py2IEOuvLYe4zlp7pR0JzEGeVl.jpg)
![IMG_20180816_205950|666x500](upload://f1QQbRvqAgdecpni0yJFuAGXbpC.jpg)
![Screenshot_20180816_210657|251x500](upload://pNZzEXhxoPTJ3IJ9u37a3YP0CHP.jpg)
```

---
## \#57 Posted by: Skyng22003 Posted at: 2018-08-16T20:20:40.175Z Reads: 51

```
I'll be modifying some code from my current receiver which can communicate with the VESC over serial to operate on a single ESP32 board, see my other thread.
 [https://www.electric-skateboard.builders/t/open-source-electric-skateboard-platform/64535/13](https://www.electric-skateboard.builders/t/open-source-electric-skateboard-platform/64535/13)
```

---
