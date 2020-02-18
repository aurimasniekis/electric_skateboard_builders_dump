# LED headlights &amp; indicators with VESC &amp; Nunchuk control

### Replies: 24 Views: 5507

## \#1 Posted by: Moja Posted at: 2015-11-03T07:37:44.267Z Reads: 482

```
 I would like to set up some functional lighting on my board for riding on the roads at night. I'd like to set up a powerful floodlight on the front, brake lights (potentially responsive to braking) and possibly indicators. 
 
Here is Vedder's setup, how was it done and what parts would people suggest for a practical 6 lights setup (front, rear, 4 indicators)? 

https://www.youtube.com/watch?v=G8f0xg7DNmM
```

---
## \#2 Posted by: RandV Posted at: 2015-11-05T16:53:33.491Z Reads: 453

```
Also Onloop was thinking about launching a LED light panel but I don't know what happened to that.

https://endless-sphere.com/forums/viewtopic.php?f=35&t=62643
```

---
## \#3 Posted by: onloop Posted at: 2015-11-05T22:13:37.542Z Reads: 426

```
I have no idea how vedder did that... i never saw any instructions...
```

---
## \#4 Posted by: Moja Posted at: 2015-11-06T08:13:29.721Z Reads: 406

```
I assume he used the UART app to configure the setup, thats all I know. If anyone knows any good reference articles on UART programming I'd love to have a good read.
```

---
## \#5 Posted by: evoheyax Posted at: 2015-12-21T20:12:25.932Z Reads: 388

```
If you listen closely near the beginning, he mentions that (by showing the UART port) is connected to the hall sensor, which is connected to the lights. How he did the turn signals, I have no idea, but the Hall sensor explains how the brake lights work.

I am leaning towards a tx controlled brake and headlight system.

This in particular looks promising, as it appears to be bright and is powered by the tx and can be controlled by the tx.

http://www.amazon.com/gp/product/B00C1BZT3E/ref=ox_sc_imb_mini_detail?ie=UTF8&psc=1&smid=ATVPDKIKX0DER

I can't say for 100% this works, as I have yet to test it. But I think a tx controlled brake/headlight system will be easier then using the VESC to do it, as it appears you need sensored motors, which most of us are not using, requiring more modification than using a tx system.
```

---
## \#6 Posted by: longhairedboy Posted at: 2015-12-21T20:33:53.667Z Reads: 345

```
Would these wire into the C channel on the receiver and use it as a toggle? If so, that's pretty much exactly what i've been looking for.
```

---
## \#7 Posted by: evoheyax Posted at: 2015-12-21T21:57:50.925Z Reads: 343

```
It seems like it plugs into either 1 or 2 channels. there's many kits like this that have even turn signals, but they all have very few leds that would be quite useless for an electric board.

I am ordering one today and will try it out after Christmas. Hopefully, this provides a basic headlight and brake light system.
```

---
## \#8 Posted by: longhairedboy Posted at: 2015-12-22T00:47:30.564Z Reads: 332

```
couldn't they be hacked to increase the number of lights?
```

---
## \#9 Posted by: evoheyax Posted at: 2015-12-22T15:58:10.918Z Reads: 337

```
I would assume so, but I do not know what would need to be done to do so. I may check out one of these kits. The problem is these kits are hard to find. The more popular one i've seen is this one:
http://www.ebay.com/itm/RC-Car-Truck-Lighting-12-LED-kit-system-2-4ghz-Tx-compatible-PPM-FM-NEW-/191483899815?hash=item2c95546fa7:g:XtsAAOSwo0JWGWu8

They make an 8, a 12, and a 16 led system. They seem solid, but no matter where I looked, they were mostly sold out, and if not, have to be shipped from china and have 1-2 months of shipping time, something I don't have right now. I want to get my electrical system ready by the end of the year.
```

---
## \#10 Posted by: longhairedboy Posted at: 2015-12-22T21:26:11.593Z Reads: 333

```
i definitely want headlights and taillights on my builds eventually. Even if its just marker lights i'd be happy. I have some ideas involving EL wire also. 

I've seen some interesting ideas involving all the LED circuits and batteries being inside the 1/2" risers, which would be very convenient despite having to turn them on via switch instead of remote. I'm sure I could rig up a non-pcb solution with 3 AAA bateries and a slide switch and still have it be clean, but that's not a true brake light system. 

also bluetooth audio. I suspect some Altech Lansing electronics are going to get re-puprosed at some point for one of my future ridiculous over-builds.
```

---
## \#11 Posted by: Pablo_702 Posted at: 2016-06-18T19:57:57.247Z Reads: 290

```
I would call this board the hammer head shark
```

---
## \#12 Posted by: Skitzor Posted at: 2016-07-15T11:39:38.739Z Reads: 270

```
I'm really looking into this. I'm waiting for a replacement VESC, so I can't ride at the moment, but I got my new WINNING remote in the mail, with 2 channels. I'm thinking about using the second channel (which is controlled by a simple switch) for lights on/off. But it seems it's only switching a 3.3V signal on the receiver side. 

I probably could get an arduino 3.3V relay and switch on a 12V circuit for the Led lights, but this already takes up too much room to my liking, anyone got any better idea's? Or a link for some documentation on this?

Second I want to look into, since my rear lights feature indicators and a brake light, how to get this signal out of the VESC. I dont care about the indicators, though it would be nice. But all this without using any of those RC-pre-made kits. Since I want decent lighting and already bought those, it's just a matter of getting the signal out...
```

---
## \#13 Posted by: PB1 Posted at: 2016-07-15T13:28:05.281Z Reads: 265

```
Hello @Skitzor, I've ordered one of these Receiver Controlled Switches. No experience yet. 
http://www.hobbyking.com/hobbyking/store/__46040__Turnigy_Receiver_Controlled_Switch.html

The switch can be controlled by channel 2 directly and switches up to 30V and 10A. 

Search for brake light here in the forum, this has been discussed already somewhere.
```

---
## \#14 Posted by: quinnyt2015 Posted at: 2016-09-21T09:48:04.541Z Reads: 222

```
Has anyone figured out how to do this yet?
```

---
## \#15 Posted by: Carvin_Ginger Posted at: 2016-09-24T15:36:24.788Z Reads: 227

```
http://www.electric-skateboard.builders/t/winning-remote-2nd-channel-for-led-lights-on-off-vesc/10082
```

---
## \#17 Posted by: jdnicholson Posted at: 2017-07-05T00:02:00.628Z Reads: 174

```
I have done this with RC planes and cars before. You either need to buy a set of lights with a built in controller or a receiver controller switch like @PB1 said. I have also used one of these in the past. 
https://hobbyking.com/en_us/dr-mad-thrust-electronic-on-off-switch.html

I'm not fussed about indicators or brake lights at this stage, I just want to be able to toggle them on/off.

The controller can be the tougher thing. My Nano X does not have a switch for the 2nd channel so I'm gonna have to figure out a way to maybe use the mirror button on the side somehow.  I use my board to commute so it would be so good to be able to remotely turn off and on my lights.
```

---
## \#18 Posted by: dannlh Posted at: 2017-10-30T21:01:49.044Z Reads: 149

```
HI!

New here, and I am interested in the LEDs on the board. Looks really cool. 

So...Ok, 

Here's a summary of what I can gather from the video. 

Vedder used **ws8212b LED** strip with waterproof silicon wrap around it. I'm familiar with it, because I have used it for under bar lighting. 

This kind of strip uses 1 power, 1 ground and 1 data line. On Vedder's controller, he hooked up to GND, H1 and 5v from the hall/temp connector. **Look on the bottom of your esc for labeling**.  


connector
  _______.      
| .  .  .  .  .  .   |   
____________.
edge of board

gnd, h3, h2, h1, temp, 5v

So in this case, it would be connected to the 1st, 4th and 6th pins for the **gnd, h1, and 5v**. (DON'T SCREW THIS UP!!!)

Also in his system, he has exactly 14 LEDs. 7 in front and 7 in back. These LEDs are serial devices, so the data is sent through each device on to the next one. Pinouts for these LEDs are **V+, Gnd, Data IN, Data Out**. Make sure you **connect the H1 to the Data In** connection on the first LED! Do not connect it to the Data Out. If you do the strip will do nothing.

You can test this by buying a strip of these LEDs (1M for example) and just hook up the whole strip. (or buy them as individual LED modules and solder three wires wires between each one.)  The first 14 should light up and the rest will be ignored if you have extras. On the strips there are cut marks on the LED tape to show the correct place to cut it between LEDs. 

If you notice in the video, Vedder uses a black and a white cable both going to the near strip of LEDs (one at each end of the led strip)  and the white cable then goes to the other strip of LEDs at the other end of the board from the near strip. 

Cabling is like this: 
ESC-------black-------LEDLEDLEDLEDLEDLEDLED---------white---------LEDLEDLEDLEDLEDLEDLED

The only thing I'm wondering now, **is the code in the existing firmware for this?!**

I have some ws2812b modules and ws2812b tape around here. When I get a chance I will test it out. Just building my first board for my son who is in college. 

Dannlh

edit: 
I forgot to mention Each ws8212b LED is RGB addressable with a value of 0-255 (off to full on) for each of the colors. Because they're addressable it means that any one led can be set to any color without affecting the rest of them. e.g. blinking an LED for a turn signal... or turning your running lights purple if you want to.

And I did find 8211( a relative of the 8212 - only difference is the 8211 requires a clock line ) code in the system. I just need to see if anything needs to be done to enable it or if its already in the config utility somewhere.
```

---
## \#19 Posted by: saul Posted at: 2017-10-31T05:43:58.789Z Reads: 135

```
I've been working on these for a while. 
they will be available as a plug and play and diy kit soon.

detail on this thread...
http://www.electric-skateboard.builders/t/brake-lights-and-turn-signals-finally-for-any-esc/15888
```

---
## \#20 Posted by: dannlh Posted at: 2017-11-02T15:55:30.541Z Reads: 124

```
@saul are you using the ws8211 code already in the VESC firmware? Or is  your design 100% independent of the vesc?
```

---
## \#21 Posted by: saul Posted at: 2017-11-03T00:30:10.470Z Reads: 130

```
[quote="dannlh, post:20, topic:400"]
are you using the ws8211 code already in the VESC firmware? Or is  your design 100% independent of the vesc?
[/quote]

it is independent of the esc. (it does get power from the esc) you can use it on rc cars/drones/ anything with ppm/pwm signal.

the method vedder used with the vesc requires hardware modification. maybe vesc6 has easier way but I am still using 4.1x
```

---
## \#22 Posted by: dannlh Posted at: 2017-11-03T01:35:04.648Z Reads: 120

```
Any notes on what those modifications were? I'm still looking.
```

---
## \#23 Posted by: saul Posted at: 2017-11-03T01:42:24.292Z Reads: 124

```
i forget where i found that info. i think in one of his videos.
if you really want to do it with the vesc i would ask on vedders fourm. he is quick to respond if you ask clear questions.
```

---
## \#24 Posted by: stewii Posted at: 2017-12-03T05:09:15.438Z Reads: 114

```
Hi. I found this’ll thread while digging about this same subject. 
 If you are on vesc 4.x and you want to connect the data pin to hall2 pin you have to remove R12 and C6, change R9 with a zero ohm resistor and finally add a pull up resistor ( 2.2k is fine ) to 5V. 
Then you can edit the conf general.h and compile.  Or just upload the ws2811.bin version of your firmware ( haven’t done this way and you probably can’t edit the number of LEDs ). 

On the vesc6 , which is the one I am using , you don’t need any hardware modification  you just need to edit a couple of files to make it compatible. 


<img src="/uploads/db1493/original/3X/f/2/f2f02f3f4b8614fbae089536aa9d0c32a832594e.png" width="281" height="499">
```

---
## \#25 Posted by: Ash Posted at: 2019-11-15T16:13:23.372Z Reads: 4

```
Hi Stewii, I have tried to implement this, but it does not work.

**Things I have done:**

* Flashed default WS2811.bin
* I have removed the filters on the hall sensor port and added 2.2k pull up resistor to 5v on H2 pin.
* I have replaced r8,r9,r10 with 0 ohm resistor.
* For my remote, I am using custom nun-chuck nrf24l01.
* The ws2812 leds are getting powered from external 5v source, but same ground reference.

**Observation:**

* 800khz signal is being produced on H2 pin but does not work.( the signal is constant and does not change).
```

---
