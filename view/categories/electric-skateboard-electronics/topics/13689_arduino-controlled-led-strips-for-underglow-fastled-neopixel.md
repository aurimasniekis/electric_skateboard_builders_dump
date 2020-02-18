# Arduino controlled LED Strips for Underglow-FastLED/ NeoPixel

### Replies: 9 Views: 4313

## \#1 Posted by: CaptainMerricka Posted at: 2016-11-26T06:55:02.133Z Reads: 194

```
Alright I would like to add some underglow lights to the board that have a fun pattern. (Not just fade and blink) I have no arduino experience so I am going to rely heavily on you guys for that. I have found 2 interesting code libraries that are supposed to run cool LED patterns. I think? 

 FastLED 
http://fastled.io/blog/
and NeoPixel by Adafruit.
https://github.com/adafruit/Adafruit_NeoPixel

These two webpages are what turned me on to this idea and I would like to see the fire pattern and the cylon pattern under the board as it scoots along. 2nd article has the cool videos.
http://www.tweaking4all.com/hardware/arduino/arduino-ws2812-led/
This second article expands on the first and has great example led pattern videos!
http://www.tweaking4all.com/hardware/arduino/adruino-led-strip-effects/

I need help picking an arduino or whatever board and getting this running.
```

---
## \#2 Posted by: CaptainMerricka Posted at: 2016-11-26T07:03:32.819Z Reads: 187

```
http://www.tweaking4all.com/wp-content/uploads/2015/11/LEDEffect-Cylon.mp4?_=10
http://www.tweaking4all.com/wp-content/uploads/2015/11/LEDEffect-RunningLights.mp4?_=16
http://www.tweaking4all.com/wp-content/uploads/2015/11/LEDEffect-Sparkle.mp4?_=14
```

---
## \#3 Posted by: saul Posted at: 2016-11-26T07:10:00.076Z Reads: 178

```
i'm almost done with my new lights.
it uses neopixels and microconroller to do tail/brake/turnsingals with the spare channel of a mini remote.

the adafruit lib has better support. a nano clone ($3-5) or a trinket/digispark($8/3) would work fine.

i'll probably sell a few plug and play kits once i've tested, not posting code yet because the _snakes_ are coming into esk8 sadly.
```

---
## \#4 Posted by: CaptainMerricka Posted at: 2016-11-26T09:55:19.180Z Reads: 172

```
From the NeoPixel Uberguide
https://learn.adafruit.com/adafruit-neopixel-uberguide/overview
RGB
30 LEDs: 9 Watts (about 1.8 Amps at 5 Volts).
60 LEDs: 18 Watts (about 3.6 Amps at 5 Volts).
144 LEDs : 43 watts (8.6 Amps at 5 Volts)

30 RGBW LEDs: 12 Watts (2.4 Amps at 5 Volts)
60 RGBW LEDs: 24 Watts (4.8 Amps at 5 Volts)
144 RGBW LEDs: 57 Watts (11.5 Amps at 5 Volts)
**The led needs its own power.**
If your microcontroller and NeoPixels are powered from two different sources (e.g. separate batteries for each), there must be a ground connection between the two.

When using a DC power supply, or an especially large battery, we recommend adding a large capacitor (1000 µF, 6.3V or higher) across the + and – terminals. This prevents the initial onrush of current from damaging the pixels. See the photo on the next page for an example.

Adding a 300 to 500 Ohm resistor  ohm resistor between your microcontroller's data pin and the data input on the NeoPixels can help prevent spikes on the data line that can damage your first pixel. Please add one between your micro and NeoPixels! Our NeoPixel rings already have this resistor on there<img src="/uploads/db1493/original/3X/d/c/dcb6c5be6a4fa6a1f2a4094d9fe3c5527e219bc2.jpg" width="690" height="404">

**Pro Tip:** NeoPixels don’t care what end they receive power from. Though data moves in only one direction, electricity can go either way. You can connect power at the head, the tail, in the middle, or ideally distribute it to several points. For best color consistency, aim for 1 meter or less distance from any pixel to a power connection. With larger NeoPixel setups, think of power distribution as branches of a tree rather than one continuous line.
<img src="/uploads/db1493/original/3X/8/b/8bdac984140358c6a131776200a1990f00b244d2.jpg" width="690" height="155">
```

---
## \#5 Posted by: emepror Posted at: 2016-11-26T16:16:48.621Z Reads: 144

```
check this out, never completely finished the project, but the leds change speed based off the board's speed: https://www.youtube.com/watch?v=sXrmD6p9eEo
```

---
## \#6 Posted by: CaptainMerricka Posted at: 2017-03-09T05:41:18.502Z Reads: 115

```
I've done it. The leds are running fast led or neopixel library. 
I need to re-up on my c programming to get my switches to work. I want a brightness selector based on a slide pot and a mode selector switch. I have a 10 position potentiometer from sparkfun but I have to figure out how to code it so each position determines the led pattern. 
https://youtu.be/jqfgupfd5NM
```

---
## \#7 Posted by: CaptainMerricka Posted at: 2017-03-09T05:41:47.854Z Reads: 115

```
<img src="/uploads/db1493/original/3X/c/7/c7f3a2329c8a8806afabdaa0270e011ff082f58c.JPG" width="640" height="480"><img src="/uploads/db1493/original/3X/7/6/7657f765be3e5a9e8f19f2913b79d0703b550b9c.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/0/6/06262a306851dcd542c0dc90f7a3a6e33a728f3c.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/a/3/a33d5f052cf4251060dab164ce9779cc2a8a9c54.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/c/4/c4b7d13e8b0e537243676ce6e798e46209a03ae6.JPG" width="640" height="480"><img src="/uploads/db1493/original/3X/d/0/d0e7687841cd8d902bc3d69f77bd0d4bfa056f59.JPG" width="375" height="500">
```

---
## \#8 Posted by: OLE370 Posted at: 2018-02-18T12:50:49.248Z Reads: 65

```
What type of Arduino do you use? I want to make the same with a Nano, but the Vesc library wants to have the Serial1 connection, but the Nano does not have it :/
```

---
## \#9 Posted by: dragopepper Posted at: 2018-02-19T06:30:45.100Z Reads: 47

```
For the future. You can use a esp6288 this is a arduino compatible microcrontroller with wifi. You can then control the strips with your phone. Or a esp 32 that controller have wifi and bluetooth. Theoretically you can write an app which shows your speed with a color code 😁
```

---
