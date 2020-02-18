# Synchronized lighting for VESC

### Replies: 99 Views: 5975

## \#1 Posted by: ju_mpe_r Posted at: 2018-01-27T13:59:41.897Z Reads: 606

```
Hi, there! :upside_down_face:
This is my first post here so...
First of all, I want to thank Benjamin Vedder for his great project and @Onloop for this kind place.
Also great thanks to @WhitePony for his very detailed and helpful build process posts.
And all of you, guys, for that large community.

Now, closer to the topic...
I spent some time to realize my friend's idea of underbody synchronized lighting,
it's hard to explain and better to see once than read a hundred times.

https://www.youtube.com/watch?v=jkwX-VA8xU0

**don't forget to set stepdown converter to +5volts**
![synchronized_lighting|690x463](upload://xK5sCI37PNoqjFCSGOuEcKNdkQ0.jpg)

---
You can find all instructions to try this at home here -> https://github.com/ju-mpe-r/synchronized_lighting_for_vesc
```

---
## \#2 Posted by: colinphotovideo Posted at: 2018-01-27T15:01:37.016Z Reads: 532

```
Very nice haha I like the police lights
```

---
## \#3 Posted by: ducktaperules Posted at: 2018-01-27T15:38:44.522Z Reads: 524

```
This looks great. I have been planning to do this for a while now but it seems like you beat me to it. Cant wait to try it out :)
```

---
## \#4 Posted by: akhlut Posted at: 2018-01-27T15:42:31.591Z Reads: 517

```
I have a WS2812strip...looks like I'm going to have to grab an apa102 one instead.

Is the strip sealed, and if so where did you get it?

/edit: [nevermind](https://www.amazon.com/gp/product/B01DIJHZKM/ref=ox_sc_act_title_1?smid=A2A7Y0JQLDHNKF&psc=1)
```

---
## \#5 Posted by: Sapphirinia Posted at: 2018-01-27T17:09:08.343Z Reads: 486

```
Oh, I really need to do this!
```

---
## \#6 Posted by: scepterr Posted at: 2018-01-27T19:57:48.768Z Reads: 458

```
It should be able to work with ws2812 with minor tweaking
```

---
## \#7 Posted by: akhlut Posted at: 2018-01-27T20:07:02.624Z Reads: 439

```
Yeah, i need to look at the code.  But the strip I already have isn't sealed...might as well get the right stuff.
```

---
## \#8 Posted by: XIII Posted at: 2018-01-27T21:51:18.445Z Reads: 418

```
interested in the ws2812 adaptations aswell. 

These minor tweaks... In what lib should I be looking for changes? 

nice project !
```

---
## \#9 Posted by: Sapphirinia Posted at: 2018-01-28T00:11:59.813Z Reads: 393

```
Order 2 lol
```

---
## \#10 Posted by: ju_mpe_r Posted at: 2018-01-28T02:01:28.905Z Reads: 417

```
[quote="colinphotovideo, post:2, topic:44795"]
very nice haha I like the police lights
[/quote]
Thanks! Full hue also gonna be cool, but because of winter I cant record outdoor video to show that you can skate the rainbow :slight_smile:



[quote="ducktaperules, post:3, topic:44795"]
This looks great. I have been planning to do this for a while now but it seems like you beat me to it. Cant wait to try it out :slight_smile:
[/quote]
Thanks, man! Just enjoy the result of idea! :wink:



[quote="akhlut, post:4, topic:44795, full:true"]
I have a WS2812strip…looks like I’m going to have to grab an apa102 one instead.
Is the strip sealed, and if so where did you get it?
/edit: nevermind
[/quote]
I attached links to components at github project page. And yeah, you need APA102 because of some limitations of ws2812



[quote="scepterr, post:6, topic:44795, full:true"]
It should be able to work with ws2812 with minor tweaking
[/quote]
At first I tried to accomplish this project with ws2812, but it's too slow because this strip is very time dependent - ws2812 library disables interrupts to write to the strip and enables it back, so with uart interrupts this all takes too much time... I dont say this is impossible, but sure, to get it work you will need to write your own libraries on vanilla C. One for Arduino uart setup and communication and second for updating ws2812 strip, so I decided that I don't want to waste time on this. :sweat_smile:


[quote="Sapphirinia, post:9, topic:44795, full:true"]
Order 2 lol
[/quote]
:smiley: :+1: Will be glad to help - ask if you will have any questions.

[quote="XIII, post:8, topic:44795, full:true"]
interested in the ws2812 adaptations aswell.
These minor tweaks… In what lib should I be looking for changes?
nice project !
[/quote]
Thanks! But I dont think that changes will be minor, man. Please, see my answer to @scepterr
```

---
## \#11 Posted by: ZackoryCramer Posted at: 2018-01-28T02:04:35.596Z Reads: 324

```
Wire an MPU 6050 to arduino, do some coding and get turning head lights! :grinning: (have the leaning side led brighter)
```

---
## \#12 Posted by: scepterr Posted at: 2018-01-28T02:07:25.117Z Reads: 330

```
Have you used the Teensy before?
It should be able to do everything in an even smaller package. I use them to drive 4000+ ws2812 led video displays 😋

https://www.pjrc.com/teensy/index.html

https://www.pjrc.com/teensy/td_libs_OctoWS2811.html
```

---
## \#13 Posted by: ju_mpe_r Posted at: 2018-01-28T09:24:38.902Z Reads: 317

```
[quote="scepterr, post:12, topic:44795"]
Have you used the Teensy before?
It should be able to do everything in an even smaller package. I use them to drive 4000+ ws2812 led video displays :yum:
[/quote]
No, have not tried it yet, but thanks for info, man! :wink:
In comparison arduino with teensy, cost of overall project will be more, even  with ws2812 instead of apa102.
```

---
## \#14 Posted by: akhlut Posted at: 2018-01-30T02:37:49.447Z Reads: 292

```
OK!

Time to own up to my lack of skill.  

How do I compile and flash this to the nano?  I have a pro mini (5V 16MHz) that should work.  

I have everything on-hand, just need to get the FW on there.

Thanks in advance!
```

---
## \#15 Posted by: scepterr Posted at: 2018-01-30T02:46:28.287Z Reads: 279

```
Get the Arduino ide installed
https://www.arduino.cc/en/Main/Software
```

---
## \#16 Posted by: akhlut Posted at: 2018-01-30T02:48:27.827Z Reads: 279

```
I did, but it's complaing about .ino and .pde being the only valid file types.  :/
```

---
## \#17 Posted by: scepterr Posted at: 2018-01-30T02:55:40.664Z Reads: 288

```
I'm setting up the PC I'm on now I'll see what's up
```

---
## \#18 Posted by: akhlut Posted at: 2018-01-30T03:14:47.841Z Reads: 303

```
OK, got it to compile.

Opened a new sketch, then copied the contents of main.cpp into it.  Saved the sketch.

Moved the folders in /lib to the arduino library folder, then had to install the fastgpio and the apa102 libraries.

compiled OK.  need to test tomorrow.
```

---
## \#19 Posted by: scepterr Posted at: 2018-01-30T03:17:59.626Z Reads: 294

```
Yep that's it 😋
Readme definitely needs an update 😉
```

---
## \#20 Posted by: ju_mpe_r Posted at: 2018-01-30T09:09:13.274Z Reads: 290

```
:sweat_smile: Sorry, man, Im just forgot about description for compile process in Arduino IDE. Added to readme. Thanks man. :+1:

Keep me informed and dont forget to play with **const uint8_t WHEEL_SIZE_RATIO = 15**;
```

---
## \#21 Posted by: akhlut Posted at: 2018-01-30T16:07:58.145Z Reads: 279

```
Quick questions!

Your picture his the plug going into the debug header, but shouldn't it be going into the uart header?

I have yet to play with @Ackmaniac's firmware and an HM10 module, but I think using the UART port will make users choose one or the other.  Can this firmware simply sniff the green Tx line for state changes if a bluetooth module is installed?

/edit

How could I add a second strip - one on each side of the board - that have duplicate functionality?
```

---
## \#22 Posted by: ju_mpe_r Posted at: 2018-01-30T18:39:36.767Z Reads: 282

```
Ah... You right, the picture was wrong! Shame on me) I corrected this. Thank you.

The best option to work with bluetooth module and arduino on the same VESC uart is take arduino with two uarts. And connect arduino to VESC uart and bluetooth module to second uart of arduino, but this will need some code rework.

To add second APA102 led strip just connect it in parallel with first one to the **d11** and **d12** and **gnd** arduino pins(You, also, will need second LM2596HVS converter for second strip because one of this can take only 3A current.)
```

---
## \#23 Posted by: akhlut Posted at: 2018-01-30T19:53:59.147Z Reads: 281

```
That's good news!  The second APA strip shouldn't be a problem.  I have one of these to supply the 5V.
https://hobbyking.com/en_us/yep-20a-hv-2-12s-sbec-w-selectable-voltage-output.html
```

---
## \#24 Posted by: akhlut Posted at: 2018-01-31T16:04:22.143Z Reads: 280

```
OK!  So I got this up and running last night.  Works great!

Some notes:

1) I went and [zipped up the sketch and libraries](https://drive.google.com/file/d/0B6yPgtXXa9tXV0UzUWdIRGJ5MDhsdmFMSkMxd2NpU0lJZ2cw/view?usp=sharing).  Simply upload this zip file to the on-line arduino IDE, [Arduino Create](https://create.arduino.cc/).  Should compile right away and the FASTGPIO and APA102 libraries are already available.  Works great and web access is nice!

2) My arduino pro mini would not upload when connected to the TxRx of the VESC, even with the VESC powered down.  I had to break these connections to get it to upload.  Not the end of the world, just something to be mindful of.

3) I had trouble getting the police_pallete to work.  My LED strip is 29 modules long, so I changed             
         'static const uint16_t CURRENT_PALLETE_WIDTH =29;'  I modified police_pallete too.

      const hsv_color police_pallete[80] PROGMEM = {
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
   };
It works well now.  
RESPECT MAH AUTHORITAH!
![identities-cop-cartman|690x388](upload://7Db0KqvYuyTXK8509CT3nzQLNRL.jpg)
Should CURRENT_PALLETE_WIDTH = LED_COUNT?

Also, I had a thought about how to avoid using UART entirely.  Could we attach the output of two of the motor hall sensors to INT0/1 to get the motor position? This might mess with FOC, but I'd bet that it wouldn't.
```

---
## \#25 Posted by: ju_mpe_r Posted at: 2018-01-31T22:04:00.681Z Reads: 261

```
[quote="akhlut, post:24, topic:44795"]
My arduino pro mini would not upload when connected to the TxRx of the VESC, even with the VESC powered down.  I had to break these connections to get it to upload.  Not the end of the world, just something to be mindful of.
[/quote]
Hmm, interesting, because I was able to upload firmware when VESC is powered down... Thanks for info, man, I must add these instructions to Github readme.

[quote="akhlut, post:24, topic:44795"]
I had trouble getting the police_pallete to work.  My LED strip is 29 modules long, so I changed

’static const uint16_t CURRENT_PALLETE_WIDTH =29;’  I modified police_pallete too.
[/quote]

You don't need to set **CURRENT_PALLETE_WIDTH** to **LED_COUNT**.
**CURRENT_PALLETE_WIDTH** must be equal to pallete elements, for example, if you want to create new pallete with 3 elements:
const hsv_color pallete_name[3] PROGMEM = { 0, 240, 0 };
or
const hsv_color another_pallete_name[6] PROGMEM = { 0, 240, 0, 240, 0, 240, };
so **CURRENT_PALLETE_WIDTH** must be equal to number in **[ ]** brackets and count of values in **{ }** brackets. :slight_smile:

Instead of this set **#define LED_COUNT** to number of leds on your strip(in **led_strip_apa102.h** file). And don't forget change **#define LED_STRIP_BRIGHTNESS** to **31** in the same file.

[quote="akhlut, post:24, topic:44795"]
Also, I had a thought about how to avoid using UART entirely.  Could we attach the output of two of the motor hall sensors to INT0/1 to get the motor position? This might mess with FOC, but I’d bet that it wouldn’t.
[/quote]
That's interesting idea, man, I think it's possible, but only for sensored motors :roll_eyes:

Do you have single motor board?

Also, are you using old firmware on your VESC?
I'm asking, because I tried to use HM-10 bluetooth module(with many apps at google play) and can't get any data back, because of outdated protocol I think...

p.s. Could you, please, record a video? I have too many snow on the streets in my country now, so I can't get joy of this.:sweat_smile:
```

---
## \#26 Posted by: akhlut Posted at: 2018-01-31T23:32:35.838Z Reads: 226

```
It just snowed here last night, so ice and salt and water everywhere.  :(  

I can take a quick vid of it on the bench in my disaster of an office/workshop.

I'll play with the settings tonight and document what I do and how it works.

I'm running the lastest vesc firmware from vedder - I need to dig out my HM10 module and flash the ackmaniac FW and see if I can get it working.

Yeah, sensored motors only, but I'm running @12S and the cord is just dangling there.
```

---
## \#27 Posted by: GrecoMan Posted at: 2018-02-01T02:05:07.482Z Reads: 211

```
you seem like a busy guy 😜
```

---
## \#28 Posted by: akhlut Posted at: 2018-02-01T02:15:27.570Z Reads: 220

```
Yeah, i get around.  Problem is the CNC is stuck at work and i have a few hours at night to kill when I'm home.  :slight_smile:  i got the G-code sorted for your cuts, but had to tweak some operations for the trucks mount.  Geometry is unchanged, but i need to pocket a large area to prevent a rouge piece from coming free and breaking the bit which has happened before.  I'm going in a few hours early tomorrow to try and bang out your parts.
```

---
## \#29 Posted by: GrecoMan Posted at: 2018-02-01T02:43:20.224Z Reads: 213

```
haha no worries bro. just teasing you because teasing is fun 😉
```

---
## \#30 Posted by: bsancken Posted at: 2018-02-02T06:40:04.277Z Reads: 209

```
Also interested in using my bluetooth AND an arduino on that serial line...
```

---
## \#31 Posted by: scepterr Posted at: 2018-02-03T15:07:00.390Z Reads: 205

```
Got it up and running on a couple Arduinos, it's rather sweet. A thought, would it be possible intercept brake signal(from ppm maybe) and flash red
Will try to grab a video over the weekend 😋
Btw, I'm using the 144led/m strip
```

---
## \#32 Posted by: akhlut Posted at: 2018-02-03T15:20:03.967Z Reads: 226

```
I already have a script running that reads a button press on channel 3.  Hoping to use a button press to turn the lights on and off as I don't want them on during the day.

I bet we could attach channel 2 to to INT1 and get throttle position, but that would eat up all the hardware interrupts and I'm thinking that reading hall sensors is the way to go to get around UART.

Here's the script:

#define BUTTON_SIGNAL_IN 0 
#define BUTTON_SIGNAL_IN_PIN 2
#define NEUTRAL_BUTTON 1500
volatile int nButtonIn = NEUTRAL_BUTTON;
volatile unsigned long ulStartPeriod = 0;
volatile boolean bNewButtonSignal = false;

void setup()
{
  attachInterrupt(BUTTON_SIGNAL_IN,calcInput,CHANGE);
  Serial.begin(9600); 
}

void loop()
{
 if(bNewButtonSignal)
 {
   if(nButtonIn > 1500){
   Serial.println("ON");
   }
   else{
   Serial.println("OFF");
   }
   bNewButtonSignal = false;
 }
}

void calcInput()
{
  if(digitalRead(BUTTON_SIGNAL_IN_PIN) == HIGH)
  { 
    ulStartPeriod = micros();
  }
  else
  {
    if(ulStartPeriod && (bNewButtonSignal == false))
    {
      nButtonIn = (int)(micros() - ulStartPeriod);
      ulStartPeriod = 0;
      bNewButtonSignal = true;
    }
  }
}

[Code Source](http://www.instructables.com/id/Rc-Controller-for-Better-Control-Over-Arduino-Proj/)
```

---
## \#33 Posted by: scepterr Posted at: 2018-02-03T15:21:57.979Z Reads: 186

```
I was actually just thinking, why not use ppm for everything? And/or why not put a sensor on the Arduino to sense the road moving by or motor/wheel spin? Can be vesc/ESC independent then
```

---
## \#34 Posted by: akhlut Posted at: 2018-02-03T15:34:18.354Z Reads: 195

```
Essentially yes.  We want to see what the motor or wheels are doing so that the lights are synched to the actual motion of the board.  Polling the VESC via UART gives that, but there are other ways of getting that info.

I think that reading a hall sensor is most likely the easiest way as the motors have the hardware built-in and the VESC is simply reading the values.  If we can sniff a single hall line we should be able to determine the RPM of the motor without interfering with FOC.  

I'm thinking of making a PCB to knit all these ideas together for testing.
```

---
## \#35 Posted by: scepterr Posted at: 2018-02-03T15:45:32.481Z Reads: 196

```
Yeah but that assumes having hall sensors..I have em, you have em, not everybody does though 🤔
And right now it's vesc only
Is it vesc6 compatible?
```

---
## \#36 Posted by: akhlut Posted at: 2018-02-03T15:48:36.893Z Reads: 203

```
True.  Maybe have a code base that allows for different control methods?  

* Trigger Monitor
* Hall Monitor
* UART Monitor
```

---
## \#37 Posted by: scepterr Posted at: 2018-02-03T15:50:50.323Z Reads: 213

```
I just got these awesome lipo charge+boost boards, will be making mine independently powered
![IMG_20180201_140349|666x499](upload://2KkxzA0K82h5QpxolXxImXoDUAB.jpg)
![Screenshot_20180203-105231__01|461x499](upload://qFIx5qCak2eSo7JxIQTFYX9Ksmm.jpg)
```

---
## \#38 Posted by: krloz Posted at: 2018-02-03T16:11:37.416Z Reads: 211

```
[quote="akhlut, post:34, topic:44795"]
I think that reading a hall sensor is most likely the easiest way
[/quote]

Wouldn't reading the ppm be kind of easier.  Just use a y servo cable to split the signal to vesc and arduino. Maybe drop an optocoupler before getting to the arduino to be safe. Arduino already has libraries to read the servo signal
That's what I was planning on doing on the future at least
```

---
## \#39 Posted by: scepterr Posted at: 2018-02-03T16:13:32.990Z Reads: 207

```
The only thing with ppm to take into consideration I think are the calibration values used by the vesc, there should be a way to input them , min, max, deadband
```

---
## \#40 Posted by: akhlut Posted at: 2018-02-03T16:32:38.629Z Reads: 235

```
Hmmmmm...

https://www.adafruit.com/product/2995

https://cdn-learn.adafruit.com/assets/assets/000/046/245/original/adafruit_products_Feather_M0_Bluefruit_v2.2-1.png?1504885440
```

---
## \#41 Posted by: scepterr Posted at: 2018-02-04T02:08:56.778Z Reads: 219

```
Put some bits together 😋
https://youtu.be/1gyEk7ZSpgA
![IMG_20180203_211122|514x499](upload://3DARtQhTp7ZmqTI7N2LFZ36LNSi.jpg)
![IMG_20180209_235428|690x315](upload://o7I2VnxCZyVcAXHaLZPBLdqv2l7.jpg)
```

---
## \#42 Posted by: akhlut Posted at: 2018-02-04T14:36:39.565Z Reads: 205

```
Beautiful!

I need to get mine installed.  Using 1/2" 3m dual lock to mount the strips.  Waiting on silicone end caps to keep them dry.

Curious, how many leds are are you pushing?
```

---
## \#43 Posted by: scepterr Posted at: 2018-02-04T16:12:17.123Z Reads: 196

```
72 led on each strip, 144led/m
```

---
## \#44 Posted by: akhlut Posted at: 2018-02-04T16:17:22.129Z Reads: 200

```
Did you run into compile issues?  My arduino was complaining that it was running out of memory the longer the strip got.
```

---
## \#45 Posted by: scepterr Posted at: 2018-02-04T16:17:48.964Z Reads: 195

```
No issues, about 500bytes left
```

---
## \#46 Posted by: akhlut Posted at: 2018-02-04T16:18:41.440Z Reads: 198

```
Ok.  Im only running 29 on a side.  It would be nice to have higher density.  What strip are you running?
```

---
## \#47 Posted by: scepterr Posted at: 2018-02-04T16:23:24.510Z Reads: 198

```
MOKUNGIT APA102 LED Strip Lights 3.2ft/1m APA102-C 144 LEDs 5050 RGB Individually Addressable RGB Full Color Magic LED Strip DC5V Black PCB Waterproof IP65 
https://www.amazon.com/dp/B019NZREYM/ref=cm_sw_r_cp_apa_KnZDAbRXPRTEZ
```

---
## \#48 Posted by: krloz Posted at: 2018-02-04T17:32:48.424Z Reads: 194

```
Sometimes fake Chinese arduino carry less memory than advertised.  Don't know if you're is but that could be causing it
```

---
## \#49 Posted by: scepterr Posted at: 2018-02-05T00:59:16.648Z Reads: 196

```
Possibly silly question, I don't need the gnd line if I'm not powering from vesc right?
```

---
## \#50 Posted by: Pedrodemio Posted at: 2018-02-05T01:11:59.853Z Reads: 200

```
Great work, I was planning to do something similar, on the build I’m working right now I have leds embedded in the enclosure in 4mm holes that are filled with acrillic resin, so when they are off you can’t see. The programming part I left for when i finish the built, not anymore

Thanks
```

---
## \#51 Posted by: akhlut Posted at: 2018-02-05T01:41:13.455Z Reads: 194

```
Maybe...id keep it in case of transients.
```

---
## \#52 Posted by: scepterr Posted at: 2018-02-05T01:43:07.205Z Reads: 201

```
I'll do one with and one without, see if there's any diff
![IMG_20180204_204527|690x286](upload://87mV7dw8o9KFgjqSESLDqfnVRk3.jpg)
```

---
## \#53 Posted by: bsancken Posted at: 2018-02-05T03:01:54.379Z Reads: 197

```
You're pulling the ground from the same battery ground as the vesc, right? so there's still a common ground there with the battery to filter it.
```

---
## \#54 Posted by: scepterr Posted at: 2018-02-05T03:03:42.519Z Reads: 190

```
No I'm using an independent battery for the Arduino and leds
```

---
## \#55 Posted by: bsancken Posted at: 2018-02-05T03:05:25.409Z Reads: 180

```
Ahh, my bad, didn't see that. I'll be putting this together in an hour or 2 hopefully!
```

---
## \#56 Posted by: scepterr Posted at: 2018-02-05T03:07:03.125Z Reads: 184

```
I'm making it as plugnplay as possible to any existing setup, don't have to mess with the board battery or anything just plug in uart and go
With a switch on the battery, could even be a ppm controlled switch and use your remote for on/off
```

---
## \#57 Posted by: ju_mpe_r Posted at: 2018-02-05T10:19:53.904Z Reads: 189

```
[quote="scepterr, post:49, topic:44795, full:true"]
Possibly silly question, I don’t need the gnd line if I’m not powering from vesc right?
[/quote]

no, you need arduino with vesc common ground to get right uart signals.
```

---
## \#58 Posted by: ju_mpe_r Posted at: 2018-02-05T10:33:29.314Z Reads: 202

```
[quote="scepterr, post:56, topic:44795, full:true"]
With a switch on the battery, could even be a ppm controlled switch and use your remote for on/off
[/quote]

You can use ttp223 sensor module in switch mode(with mosfet) on battery enclosure for this or even try to use it through deck ;)
https://www.youtube.com/watch?v=rcp-eIQ44I0
```

---
## \#59 Posted by: akhlut Posted at: 2018-02-07T04:32:19.589Z Reads: 200

```
Is there a way to change the direction of the lights?

Mine are moving opposite to the direction of travel.

https://youtu.be/-SS4X4zkaE4
```

---
## \#60 Posted by: bsancken Posted at: 2018-02-07T07:10:00.026Z Reads: 192

```
OMG I love those enclosures! 3d printed? I'd imagine invert the variable that deals with which step in the palette array?
```

---
## \#61 Posted by: akhlut Posted at: 2018-02-07T20:27:23.144Z Reads: 185

```
Yeah, the walls and interface plates (board to enclosure) are 3D printed.  There is a CNC'd aluminum base plate and CNC'd acrylic covers.
```

---
## \#62 Posted by: akhlut Posted at: 2018-02-07T21:14:58.708Z Reads: 191

```
@ju_mpe_r

changing the led direction of travel...

_color_shifting.cpp_
_#include "color_shifting.h"_
_#include "led_strip_apa102.h"_
_#include "color_palletes.h"_



_extern "C" {_
_#include "vesc_uart.h"_
_};_



_void update_strip_colors(void) {_
_uint32_t current_tacho_value;_
_uint32_t pallete_travel;_
_current_tacho_value = bldc_get_tachometer_value();_
_pallete_travel = current_tacho_value / WHEEL_SIZE_RATIO;_
_for (uint8_t i; i < LED_COUNT; i++) {_
_led_strip_colors[i] = get_pallete_color(pallete_travel  + i);_
_}_
_update_strip();_
_}_

Just change 
    **led_strip_colors[i] = get_pallete_color(pallete_travel  + i);**
to
    **led_strip_colors[i] = get_pallete_color(pallete_travel  - i);**
?
```

---
## \#63 Posted by: ju_mpe_r Posted at: 2018-02-07T21:25:49.918Z Reads: 179

```
yeah, this is fastest solution ;)
but I'm trying to implement this setting based on condition right now...:sweat_smile:
```

---
## \#64 Posted by: akhlut Posted at: 2018-02-07T21:27:30.798Z Reads: 178

```
Awesome!  

I'm loving the lights man!  And making/customizing the palletes is great!
```

---
## \#65 Posted by: ju_mpe_r Posted at: 2018-02-07T21:30:08.841Z Reads: 178

```
Thanks man!
And big thanks for the video! :pray:

p.s. What is your **WHEEL_SIZE_RATIO** value on the video?
```

---
## \#66 Posted by: akhlut Posted at: 2018-02-07T21:30:53.537Z Reads: 195

```
const uint8_t WHEEL_SIZE_RATIO = 10;

I kinda want the lights to blink fast, just like the po-po.

my modified police pallete:

/* POLICE PALLETE */
   const hsv_color police_pallete[460] PROGMEM = {
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      0, 0, 0, 0, 0, 0, 0, 0, 0, 0,
      240, 240, 240, 240, 240, 240, 240, 240, 240, 240,
    
   };

also, resorted to a hardware solution to turn the lights on and off.

https://www.amazon.com/gp/product/B012W6RJ5I/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#67 Posted by: ju_mpe_r Posted at: 2018-02-07T21:35:59.606Z Reads: 184

```
[quote="akhlut, post:66, topic:44795"]
I kinda want the lights to blink fast, just like the po-po.
[/quote]
:smiley: After that answer everything is fine :wink:

p.s. Thanks for sharing your pallete, I'll add it to project ;)
```

---
## \#68 Posted by: scepterr Posted at: 2018-02-10T05:02:39.943Z Reads: 185

```
I wonder if this can be ported to the photon remote...it already supports ws2812.. 
@ju_mpe_r  @Wajdi what do you think?
```

---
## \#69 Posted by: scepterr Posted at: 2018-02-11T00:05:01.867Z Reads: 190

```
@ju_mpe_r I think some options could be added to standby, something like this

https://thumbs.gfycat.com/AdorableSlightBarnswallow-max-1mb.gif
```

---
## \#70 Posted by: Wajdi Posted at: 2018-02-11T03:19:18.319Z Reads: 179

```
Very cool, I like the idea of synchronizing light to movement by distance. I will work on adding that to the list of effects.
```

---
## \#71 Posted by: ju_mpe_r Posted at: 2018-02-12T12:34:05.913Z Reads: 180

```
[quote="scepterr, post:69, topic:44795, full:true"]
@ju_mpe_r I think some options could be added to standby, something like this
[/quote]

Yeah!
I like this idea and it's not hard to implement, but don't know when I will have time for that.
```

---
## \#72 Posted by: ju_mpe_r Posted at: 2018-02-14T02:43:09.852Z Reads: 175

```
I don't like that the idea will be used in not open source project. But I understand that can't do anything with this. So...
```

---
## \#73 Posted by: Ishayc Posted at: 2018-06-15T07:15:13.132Z Reads: 150

```
Maybe someone has a clue why changes I make that’s not in the main.ino file(like led_count) doesn’t work?
```

---
## \#74 Posted by: Ishayc Posted at: 2018-06-15T10:58:20.037Z Reads: 145

```
nvm got it to work.
Another question - I can't seem to make it work with @Ackmaniac 's 2.54 version only the new one.   Any idea?
I set the baud rate to 115200 on both versions.
```

---
## \#75 Posted by: ARetardedPillow Posted at: 2018-07-29T15:57:08.043Z Reads: 131

```
I can't get it to work for some reason, seems like the arduino doesn't read the UART signals from vesc at all
```

---
## \#76 Posted by: akhlut Posted at: 2018-07-29T16:12:18.630Z Reads: 130

```
Did you change vesc to ppm and uart?
```

---
## \#77 Posted by: ARetardedPillow Posted at: 2018-07-29T16:13:46.430Z Reads: 131

```
Yea I checked everything, bluetooth works fine aswell
```

---
## \#78 Posted by: akhlut Posted at: 2018-07-29T16:18:40.992Z Reads: 130

```
BT?  Might not work with BT.

@ju_mpe_r?
```

---
## \#79 Posted by: ARetardedPillow Posted at: 2018-07-29T16:20:35.978Z Reads: 128

```
Oh no. I plugged in bt just to make sure the vesc send UART signal, I tried it without the BT
```

---
## \#80 Posted by: ARetardedPillow Posted at: 2018-08-20T15:19:28.891Z Reads: 128

```
Does not work with Ack 2.54, does work with 3.102 though.

Also, would this work for SK9822? I can't find apa102s on amazon that are waterproof and have black pcbs
```

---
## \#81 Posted by: ZachTetra Posted at: 2019-01-14T14:37:19.765Z Reads: 110

```
How much money would someone make and ship one of these (electronics with software but not the lights)?  And will it work for any ESC (I've got the MayTech 50A dual)?
```

---
## \#82 Posted by: ARetardedPillow Posted at: 2019-01-14T14:48:33.556Z Reads: 111

```
Its not that hard/expensive to build and program, the whole system without the lights costs 5$ at most
```

---
## \#83 Posted by: ZachTetra Posted at: 2019-01-14T14:49:19.002Z Reads: 109

```
Including the step down and other circuitry?
```

---
## \#84 Posted by: ZachTetra Posted at: 2019-01-14T14:50:05.403Z Reads: 111

```
I really want something like that but I don't have any experience in these electronics
```

---
## \#85 Posted by: Mudders Posted at: 2019-03-03T21:06:18.085Z Reads: 103

```
I'd like to have a go at this, with no prior experience at all with kinda stuff. 

If i order the shopping list in the OP, i guess itll work with the unity?
```

---
## \#86 Posted by: Songsta Posted at: 2019-03-09T15:37:02.232Z Reads: 97

```
I’m really keen to try this. Is it possible to run the power for this directly from one of the Vesc 6 ports? I’m struggling to find the necessary voltage step down converter in South Africa.
```

---
## \#87 Posted by: Bor.inc Posted at: 2019-03-10T20:47:29.502Z Reads: 95

```
You can try it but I dont recommend it, maybe it can work well but the main problem is that the vesc isnt capable of supplying a lot of juice from his 5v port.

I know someone that blew his vesc because he had too big of a light connected to his vesc so maybe try to find another solution (iknow its probably hard)
```

---
## \#89 Posted by: Jonhson Posted at: 2019-05-16T15:07:40.617Z Reads: 71

```
    This is the first time I used this scheme.There are any problems that I don't  understand.When ATmega328 communicate with VESC electronic speed controller to get motor information by UART , I found that there are no CRC datas in each package.So VESC electronic speed controller cannot feed back to ATmega328, and the RGB light belt cannot flicker normally.I do not know how to modify the program source code, please advise, thank you!
```

---
## \#90 Posted by: RedBaron Posted at: 2019-05-16T19:31:24.493Z Reads: 68

```
I love this, especially the police scheme.
```

---
## \#91 Posted by: TheAwkwardLlama Posted at: 2019-05-21T16:22:19.488Z Reads: 64

```
Has anyone gotten this to work with the Unity? 

I have mine put together and everything is loaded up. The lights are stuck in stand by mode no matter how much the motors move.
```

---
## \#92 Posted by: Ricco Posted at: 2019-05-21T17:07:32.285Z Reads: 65

```
Do you have experience with Arduino coding? I know that the Unity has a different response for the COMM_GET_VALUES UART command, so though I'm not completely familiar with how the code for this is written i would bet that you need to change how the data from that packet is parsed (which bytes are stored in which variables)
```

---
## \#93 Posted by: TheAwkwardLlama Posted at: 2019-05-21T17:19:38.696Z Reads: 62

```
I only know enough to edit whats needed when instructions are present lol. But thanks a lot for the tip. I'm going to try and look into it more.
```

---
## \#94 Posted by: Ricco Posted at: 2019-05-22T03:39:08.870Z Reads: 57

```
No problem :) after taking a look at the code, it looks like you can update which bytes are taken from a COMM_GET_VALUES packet in the "bldc_interface.c" file of the VESC UART library used. Look at the "bldc_interface_process_packet" function. Just check what bytes are sent by the Unity by looking at the "commands.c" file of enertion's unity FW and update them accordingly :slight_smile:
```

---
## \#95 Posted by: TheAwkwardLlama Posted at: 2019-05-22T16:06:11.403Z Reads: 52

```
https://giphy.com/gifs/carl-sagan-mbhseRYedlG5W

You're awesome! I'll look through everything today or tomorrow and see what I can do. :star_struck:
```

---
## \#96 Posted by: Bbaldrickk Posted at: 2019-07-21T15:59:04.066Z Reads: 43

```
Has anybody got this working on the latest vesc firmware cant seem to get it working I have tx and rx correct but lights wont move
```

---
## \#97 Posted by: willumpie82 Posted at: 2019-07-22T06:15:55.620Z Reads: 42

```
This is an awesome project!

Since I have both my uarts (dual VESC) in use (Flipsky VX1 and Metr.pro) would this board also work when I connect just the RX in parralell with the metr.pro?
```

---
## \#98 Posted by: bsancken Posted at: 2019-07-22T06:18:37.814Z Reads: 42

```
Btw - Just got mine, Still in beta but sounds like you could use this for future addons..

https://www.electric-skateboard.builders/t/uart-splitter-for-vesc-based-escs/94552
```

---
## \#99 Posted by: Pimousse Posted at: 2019-07-23T07:09:07.908Z Reads: 39

```
Could work but you need a modified library.
```

---
## \#100 Posted by: Bbaldrickk Posted at: 2019-07-24T09:26:50.815Z Reads: 31

```
Am I missing something so glaringly obvious that nobody even wants to mention it:crazy_face:
```

---
