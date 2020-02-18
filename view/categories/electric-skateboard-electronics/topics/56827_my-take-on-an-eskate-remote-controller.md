# My take on an eskate remote controller

### Replies: 68 Views: 3635

## \#1 Posted by: ofekp Posted at: 2018-05-26T09:57:06.466Z Reads: 497

```
As far as I know this is a first, but please let me know if I am wrong.
I never seen someone making this concept of a remote. It is a prototype and can be largely improved with 3D printing, at least the aesthetics of it, but it functions great.

Remote Controller Features:
- UART connection to a VESC over Bluetooth, only a Bluetooth module is needed to connect to the VESC, with no additional hardware.
- Board battery voltage and speed on a tiny side display
- Speaker for indicating connection to the board
- The speaker also beeps when connection is lost (did not happen but functionality works when I power down the board while leaving the remote on)
- Charging through mini USB port (this is a power bank mod after all)
- Throttle and braking FSR function according to rider applied force
- Comfortable for usage with gloves
- No moving parts whatsoever


https://i.imgur.com/FF3M906.jpg

Remote in action:
https://www.youtube.com/watch?v=TJ6FgYh-Vco

More images (from before I used bolts to mount the top) and a look into the insides:
[ESK8 FSR Remote Controller Prototype](https://imgur.com/a/fKD2m)

I want to know what you think :slight_smile:
```

---
## \#2 Posted by: chocol4te Posted at: 2018-05-26T11:35:55.728Z Reads: 434

```
Really interesting! The solid state seems a lot safer, you don't want a crushed remote to be stuck on max throttle. Have you tried thumb wheel and forefinger trigger style remotes and if so, could you give a run down of the differences (comfort, precision, etc)? Would you recommend this over the other types?
```

---
## \#3 Posted by: ofekp Posted at: 2018-05-26T11:47:23.808Z Reads: 421

```
I have not tried the opposing thumb and index finger sensors configuration since it is harder to implement with no 3D printer. Although, this configuration is awesome and I am able to controll my speed to my liking and it is very intuitive to use. The preceision is actually better than can be seen in the video when the board is under load.
That said, I admit I never tried a different remote for a long period of time.
I think there are may configuration to be explored with this design, like opposing, or maybe thumb on front and index on the top face which I wanted to do but had the powerbank charge inlet there..
```

---
## \#4 Posted by: chocol4te Posted at: 2018-05-26T11:51:42.478Z Reads: 378

```
I've been working on some new remote internals, using a better radio, 1.5inch OLED, faster MCU and some firmware written in Rust instead of C. I'd really like to try this kind of user input, perhaps something like the Boosted remote but a pressure sensor where the wheel would be?
```

---
## \#6 Posted by: ofekp Posted at: 2018-05-26T12:02:10.547Z Reads: 352

```
yeah I like this, you can use smaller FSR sensors so that the rider will not have to move his finger to much to change from throttle to brake, but make sure it usable with a glove.
You better equip yourself with a 3D printer, otherwise you’re in for a lot of exploring on how to mount those FSRs to the remote.
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2018-05-26T13:01:49.525Z Reads: 338

```
This looks really interesting, never thought about FSR Sensors in a remote!

Also i'm curious about the Bluetooth module. I used one back then with a nunchuck style remote and found it to be really unreliable. Like random dropouts or just stopping to work. Which one are you using? And what kind of protocol? I used some serial.write commands in an endless stream with codewords inbetween and it didn't work too well. Since then i switched to nrf24l01 with a proper antenna and i never had issues and the data handling is also way better.
```

---
## \#8 Posted by: davewood1982 Posted at: 2018-05-26T13:24:51.404Z Reads: 313

```
Interesting, So how practical  would the sensors be? People have different sized fingers and thumbs, theres a fair difference between a 15/16yr olds thumb and a fully grown man in his 30 or 40s, what about men and women. Make them sensor pads too small and it will be impossible for some people to use,Too large and id of thought it could be quite dangerous?
```

---
## \#9 Posted by: ofekp Posted at: 2018-05-26T13:43:09.888Z Reads: 310

```
Yeah, so far, it looks like I am the first to think of that :wink:

I am using the simple HC-05, two of them, one is a slave and one is master.
The process of binding the two is a bit annoying, but once you do that they connect rather quickly and it is hard to get them to disconnect, I had one disconnection in a long time which might have been caused because the remote was not fully charged, and I have to go several meters away from the board before they unbind.

I am communicating with the VESC through UART so I am using [VescUart](https://github.com/RollingGecko/VescUartControl/blob/master/VescUart.h) library to send the commands over Bluetooth to the other BT module that is directly connected to the VESC.

The remote does all the lifting here using an Arduino Nano so it was easy to update the software, only the remote needed to be updated, plus it was easier to maintain and debug than when I had two Arduinos.
Fitting it all inside this power-bank was hard, though.

Connecting through the UART has many benefits, one of them is being able to get the voltage and RPM from the VESC, I then display them on tiny screen and this is how I know when to stop riding.

I have not cracked the RPM to speed formula yet, pretty sure I had it wrong somewhere in my formula lol. Perhaps the rpm the VESC is sending is not accurate or perhaps it is actually erpm, anybody knows?
```

---
## \#10 Posted by: ofekp Posted at: 2018-05-26T13:47:40.432Z Reads: 267

```
I think women and men will be able to use this configuration as is. I let a kid try this once and he seemed to have no problem controlling it he was 15+- not sure how it will be for younger kids, though.
Also gave it to multiple people that had no other experience in eboards before and they all seemed to be handling it quite well, so I guess it is intuitive enough.
```

---
## \#11 Posted by: Der6FingerJo Posted at: 2018-05-26T14:10:10.468Z Reads: 243

```
I used HC05's too but it was garbage. But hey, maybe I just didn't win in the silicone lottery. 

The Vesc sends eRPM out of the UART, you can find the formulas in rollinggeckos ArduBiardControl or Solidgeeks remote in GitHub :smiley:
```

---
## \#12 Posted by: ofekp Posted at: 2018-05-26T14:20:11.988Z Reads: 242

```
Thanks! Finally I will correct my formula :slight_smile:

I guess this can be used with radio and two arduinos too, but I like that I have only one Arduino, I found that this is the point of faliure most times, when you have two of these you have to use SoftwareSerial and this is when things really start to get messy :face_with_head_bandage:
```

---
## \#13 Posted by: Der6FingerJo Posted at: 2018-05-26T14:34:31.955Z Reads: 241

```
Oooooh now i get it. Hey that's pretty cool to only use one arduino, makes sense. This would also be very possible with nrf24l01 modules so if you ever have any connection problems you could try those as well.

Oh and actually i used a Arduino Mega on my old board so no software serial, but i agree that it's a bit more messy than with one arduino only.
```

---
## \#14 Posted by: ofekp Posted at: 2018-05-26T14:58:28.736Z Reads: 224

```
Great idea, how much more reliable were they in your case? It is also serial I2C right?
```

---
## \#15 Posted by: Der6FingerJo Posted at: 2018-05-26T15:00:45.681Z Reads: 239

```
Well, i went from occasional hiccups on bluetooth (like every 5km or so) to absolutely no problems at all over ~400km on nrf24. They are communicating using SPI (i believe) and there are plenty of libraries available to make it easy.
```

---
## \#16 Posted by: ofekp Posted at: 2018-05-26T16:11:58.906Z Reads: 238

```
I will give it a try :+1:
```

---
## \#17 Posted by: ofekp Posted at: 2018-05-26T16:35:55.652Z Reads: 242

```
Can you use this without the antenna too?
```

---
## \#18 Posted by: Der6FingerJo Posted at: 2018-05-26T16:39:32.407Z Reads: 253

```
There are smaller modules with a PCB antenna but I can't say anything about those. IMO a dedicated antenna should be on every vehicle that relies on radio communication.
```

---
## \#19 Posted by: ofekp Posted at: 2018-05-26T17:42:31.503Z Reads: 252

```
how do you connect the nrf24l01 to the VESC directly? Looks like there's only UART.. but the nrf24l01 is using SPI.
```

---
## \#20 Posted by: Der6FingerJo Posted at: 2018-05-26T17:46:12.458Z Reads: 247

```
The vesc 6 has an inbuilt nrf and I believe you can hook it up to vesc 4 too. Hast to be on the uart port as well, those pins can have different functions depending on settings.
```

---
## \#21 Posted by: ofekp Posted at: 2018-05-26T17:54:43.888Z Reads: 238

```
So if I use VESC4.12 I won't need to flush a new hardware and no need to buy SPI to UART modules right?
```

---
## \#22 Posted by: Der6FingerJo Posted at: 2018-05-26T17:56:32.574Z Reads: 204

```
Nope probably not. Just Google for VESC and Nrf, I'm sure you'll find something
```

---
## \#23 Posted by: ofekp Posted at: 2018-05-26T18:01:17.383Z Reads: 204

```
Will make the next remote with this module cuz it sounds good :slight_smile:
Now I need to think how to hide the antenna :wink:
```

---
## \#24 Posted by: Der6FingerJo Posted at: 2018-05-26T18:55:56.554Z Reads: 209

```
Best way is to decase a WiFi antenna, they are pretty slim after that.
```

---
## \#25 Posted by: chocol4te Posted at: 2018-05-27T11:52:36.709Z Reads: 216

```
Oooh, this is interesting:

https://www.adafruit.com/product/178

Thoughts? Seems like a nice middle ground; still no mechanical parts, but a more familiar interface. They do a 25mm one which seems about right.

In terms of comfort on long rides, I don't know what would be better. FSR means no need to move thumb to change speeds which is good, however pressing down for a long time might be uncomfortable.
```

---
## \#26 Posted by: ofekp Posted at: 2018-05-27T13:00:15.102Z Reads: 198

```
I like what you got
```

---
## \#27 Posted by: sunnyD Posted at: 2018-05-27T15:39:30.737Z Reads: 190

```
I like this idea very much, let me see what i can do with that sensor.
```

---
## \#28 Posted by: ofekp Posted at: 2018-05-27T16:05:46.414Z Reads: 196

```
I knew I would spark more innovations from this :slight_smile:
This is very good, I thought of it before but could not find anything like that. I imagine it will be weirder to use maybe, but if you place it correctly than it could be great.

For example I thought of the boosted remote with this strip on the top instead of the roller this could work well as long as the active region on the strip is not too long.
```

---
## \#29 Posted by: chocol4te Posted at: 2018-05-27T16:55:58.574Z Reads: 197

```
Last exam is on the 25th, I gotta concentrate and not start CAD mockups! :smiley:
```

---
## \#30 Posted by: Nemesis Posted at: 2018-05-27T17:49:30.336Z Reads: 199

```
@ofekp Im wondering, is it possible the sensors could be used as multi function buttons? for example hold both for 4 seconds to power on or off/sleep mode?

Ps i really like the robust look of this keep it going bro.. bookmarked :slight_smile:
```

---
## \#31 Posted by: ofekp Posted at: 2018-05-27T18:37:07.297Z Reads: 204

```
Happy you like this :smile:
The answer is YES! In the code I am already planning on pressing both sensors for a few seconds to turn on the lights (which I haven't yet started to build, so no point in doing it now :laughing:)
I would not, however use it for too many options, this gets dangerous the more you add to it because if you have a bug in your code and you accidentally put your fingers the wrong place during a ride you can get, well I don't need to tell you what you can get...

In any case, as long as you don't overload this too much this is possible.

Note, though, that if you are connected to the VESC directly, which I recommend you will, you will have to place your code that flicks the lights on inside your VESC, I do not yet know how to achieve that. But I know for fact this could be done.
This is how I know that:
https://www.youtube.com/watch?v=G8f0xg7DNmM

If someone does know how, please share.
```

---
## \#32 Posted by: skelstar Posted at: 2018-05-28T01:00:56.584Z Reads: 180

```
Very cool! I have my own take on the traditional potentiometer-based remote (which I will share soon), but hadn't thought of using one of these. Have ordered a couple of AliExpress (hope you don't mind inspiring me to try).
```

---
## \#33 Posted by: faithfulpuppy Posted at: 2018-05-28T01:11:39.614Z Reads: 163

```
This is super dope! I'm working on my own controller design right now too, seeing innovation in eboards is so exciting!
```

---
## \#34 Posted by: ofekp Posted at: 2018-05-28T06:31:39.360Z Reads: 164

```
The whole point is to get you inspired. Please do.
Show us what you got!
```

---
## \#35 Posted by: ofekp Posted at: 2018-05-28T06:35:09.750Z Reads: 155

```
I agree!
I have been using this for a long time now and I am super glad to share this idea and inspire others to try :smile:
```

---
## \#36 Posted by: skelstar Posted at: 2018-05-29T19:44:02.735Z Reads: 149

```
Was thinking about these FSR sensors when I was walking to work this morning (wet roads = no board :( ):
the sensor wouldn't have to mount to a flat surface would they? I'm just thinking about a 2D surface, not 3D. Not necessarily a radical curve either.
```

---
## \#37 Posted by: ofekp Posted at: 2018-05-29T21:10:04.053Z Reads: 162

```
Most of those come with sticker on the back so you can stick them on a flat surface.
If you do not put them on a flat surface you will have nothing to press them against (Newton's third law blah blah blah) which won't do you much good.
You need to find a way to mount them on a surface and then cover them with another, much like I did. If you do have access to a 3D printer you're in luck, I used aluminum which was easy enough to process.
But yes, the ones I use can, and, in fact, should be pressed against a flat 2D surface.
```

---
## \#38 Posted by: skelstar Posted at: 2018-05-29T21:25:58.995Z Reads: 166

```
I was imagining one of those nano-remote type arrangements with the hole that you stick your finger in, and the FSR would stick to the inside of the hole. 

If the buttons on the top of the remote were a bit 'awkward' then mounting it into the hole might be a bit more comfortable.
![image|487x417](upload://r12MZ6u2jQ6KZcM2YmJ2NEbAxjU.jpg)

I appreciate that the footprint of the FSR might be significantly bigger than the depth of the hole (in the nano-remote at least). If I were to 3D printer something then you could make the hole deeper.

Wish I could help you out 3D printer-wise. I'm in New Zealand and I imagine I'm a _very_ long way away from you (freight-wise).
```

---
## \#39 Posted by: ofekp Posted at: 2018-05-31T08:50:19.606Z Reads: 163

```
There are many different kinds of FSR sensors with smaller diameter that could fit your design, e.g.
https://www.ebay.com/itm/Force-Sensor-FSR400-Sensitive-Resistor-Force/282810402815?_trkparms=aid%3D555018%26algo%3DPL.SIM%26ao%3D2%26asc%3D44040%26meid%3D82ad88a1b90e480abc59a8915e9cc43b%26pid%3D100005%26rk%3D1%26rkt%3D12%26sd%3D202261960276%26itm%3D282810402815&_trksid=p2047675.c100005.m1851

Also, check out the other suggestion made by @chocol4te in this thread for a different kind of [Robbon Sensor](https://www.electric-skateboard.builders/t/my-take-on-an-eskate-remote-controller/56827/25?u=ofekp)

This may fit on top and will fit the remote profile well IMO. But mods will need to be made to make it fit nicely.

Thanks for trying to help with 3D printing, it is just two planes and like 24 hours of flight :wink: LOL I will get myself one of these eventually and will make this remote even greater!
```

---
## \#40 Posted by: kuphjr Posted at: 2018-05-31T14:56:25.841Z Reads: 149

```
I would definitely be interested in purchasing a couple of these if you get all the kinks worked out.  I would love being able to have my speed right on my remote!  I would need a speedometer on the side that would show speeds up to 40mph though.
```

---
## \#41 Posted by: ofekp Posted at: 2018-06-02T10:09:02.757Z Reads: 142

```
you'll need to elaborate on "kinks"
The remote can show any speed up to 99Km/h, but boy, 40mph... please wear a helmet and gloves at least.
```

---
## \#42 Posted by: kuphjr Posted at: 2018-06-04T16:22:32.346Z Reads: 126

```
Yes, I always wear motorcycle helmet, gloves, pants and jacket when I go that fast.  I'm certainly not the first person on the forum to do it lol.

By kinks I just meant that I didn't want to buy anything that doesn't work very well yet.  I just wasn't sure if this was your final design or if you are still working on it and improving things since you mentioned it was a prototype in your first post.
```

---
## \#43 Posted by: kuphjr Posted at: 2018-06-04T16:24:11.709Z Reads: 122

```
Not insinuating your remote doesn't work well, but I know as with any DIY project it sometimes takes a few tries to work out any potential flaws or improvements that can be made.
```

---
## \#44 Posted by: TheFluffiest Posted at: 2018-06-04T17:01:26.122Z Reads: 121

```
I think you may have stumbled upon something revolutionary...

If you put that on a slide glove, you could allow the use of a slide puck on both hands! I know people have been trying to integrate remotes into gloves for awhile, I think this may be the solution!
```

---
## \#45 Posted by: ofekp Posted at: 2018-06-08T18:37:32.582Z Reads: 122

```
Thanks, glad you like it,
I thought of this idea :slight_smile: I still prefer the remote, for now, but yeah this can totally be done.
I would have used a smaller battery though, this one lasts way too long and can be made smaller.
I do admit it was a test of my ingenuity to fit that all in that power bank, but if there's a will there's a way!
If you do plan to attempt this do let me know.
```

---
## \#46 Posted by: ofekp Posted at: 2018-06-08T18:43:22.988Z Reads: 123

```
It took a few iteration to get to this, a lot of things did not work on the way.
As I explained above, software serial made my life miserable along the way. I had to do many software changes before it worked as well as it does now, and as I said before too, I do not plan to stop here. You're right, I do not know if I can sell it this way because I would like to make the casing nicer, but functionality wise I am very happy. Will give the nrf24l01 that @Der6FingerJo suggested as it sounds powerful and I do want this to be as safe as possible.
```

---
## \#47 Posted by: Der6FingerJo Posted at: 2018-06-08T19:05:51.206Z Reads: 115

```
Be sure to use some capacitors on the power input of the Nrf, the Arduino step down will struggle with the load!
```

---
## \#48 Posted by: Hummie Posted at: 2018-06-08T19:14:33.763Z Reads: 120

```
i saw the video but haven't read the the whole thread.  how do you control degrees of throttle and brake?  if i wanted to slam on the brakes vs slowly.  is it like cruise control for the throttle?
```

---
## \#50 Posted by: ofekp Posted at: 2018-06-08T20:22:25.833Z Reads: 131

```
Thanks for the advise :slight_smile:
What capacitor do you use (Farad)?

Like that?
![image|222x120](upload://2MP4dBG62YB8Tg5xlcXZ2B8TTR3.png)
http://www.reuk.co.uk/wordpress/electric-circuit/smoothing-capactitors/

Thanks!!
```

---
## \#51 Posted by: ofekp Posted at: 2018-06-08T20:23:01.101Z Reads: 128

```
That’s the thing, those sensors know how hard you press.
Totally controllable and very intuitive.
```

---
## \#52 Posted by: Der6FingerJo Posted at: 2018-06-08T20:25:37.940Z Reads: 127

```
Actually only one I had laying around. Maybe 470 microFarad
```

---
## \#53 Posted by: wafflejock Posted at: 2018-06-08T20:38:10.994Z Reads: 133

```
@ofekp check out @solidgeek's remote and code if you haven't already I also made my own remote with basically bare minimum code here: https://github.com/shusain/eskatecontroller

For mine I'm using an arduino pro-mini on both the transmitter and receiver side.  Things are stable and work well regarding the arduino's so long as you are powering them correctly given the clock rate on the arduino you're using.  Regarding the capacitors for the NRF chips believe .1 and 10microFarad is recommended (I used a 100microFarad one and it does seem to help to keep the nrf chip itself stable), more info here: https://arduino-info.wikispaces.com/Nrf24L01-2.4GHz-HowTo

I did an arduino+nrf on the transmitter and receiver side and have PCBs to connect the arduino to the nrf chips that work for both the transmitter and receiver (if interested in trying those out send me a PM with where you're at and can see what shipping would be, they only cost me a couple dollars a piece to get 100 made, but I have plenty of extras for anyone experimenting).  The nrf with the antenna on the board work well for at least 30ft away the ones with external power amplifier (PA) and antenna can go for at least a city block (as far as I could see my RC car from).

---

One thing to note, I don't know anything about the FSR sensors but using a potentiometer in my controller and every once in a while I have to replace it or recalibrate things due to drift or things getting messed up with the potentiometer (think humidity changes effect it).  Luckily the 'safe start' on the VESC and other config basically stops it from getting too horribly dangerous.  I'll likely switch over to using linear hall sensor and magnets similar to solid geeks build.
```

---
## \#54 Posted by: ofekp Posted at: 2018-06-08T21:27:54.824Z Reads: 114

```
That's a neat project, I should really get myself a 3D printer :slight_smile: 
https://arduino-info.wikispaces.com/Nrf24L01-2.4GHz-HowTo - Lot's of info that I will use on the next remote :+1: 
 Seems like those NRFs are the way to go, but I am really trying to avoid using an Arduino as an SPI to I2C/UART converter.

I did find this post http://reboot.love/t/vesc-mods-for-robotics-use/107
It kinda says there's a flag that can be changed to get the SPI working on the VESC  (if I am not mistaking, I think the rest of the code in the GitHub link he shared is unrelated stuff). It does require HW flush and all the pain that comes with it (I imagine) but I think this is worth it 100%.

hall sensor sound much better and should not be susceptible to weather, although, regular potentiometers should not be that sensitive either, no?
```

---
## \#55 Posted by: wafflejock Posted at: 2018-06-08T21:36:29.812Z Reads: 109

```
Yah the potentiometer was good for a long time but recently when the weather changed here it started acting weird unless I put pressure on it, maybe case of just crappy component or something along those lines just figured I'd put it out there as something to consider.  Regarding using the nrf directly on the vesc that sounds like it should work I just didn't want to deal with modifying the firmware and trying to keep a patch up to date (if it's just a matter of uncommenting a line perhaps not a big deal). Nice thing about using an Arduino on the receiver side is can bake some extra logic in there like my time out code (vesc also has a timeout though for no signal received, so maybe doesn't matter).  Only issue I've had was things going ghost Rider on me when only the mosi pin for SPI got disconnected and the throttle floated high.  I worked around that issue by only ever sending 1-254 instead of 0-255 so if it floats high or low I know it's a bogus value and ignore it (go idle)
```

---
## \#56 Posted by: ofekp Posted at: 2018-06-08T21:50:02.791Z Reads: 111

```
I had a version where the Arduino on both side was OK, but since then I added a screen and wanted to communicate with the VESC to get data. As I was adding more functionality, the system was now using two way communication so I needed to use Software Serial (Arduino Nano has only one HW serial) and that got all kinds of weird things going on.
Debugging those issue can be hard, when I had the Arduino connected in one previous version (with Software Serial) I got weird behavior where every once in a while the brakes would engage. Actually fell once due to this on slow test speed luckily. And on other dev version I had the throttle engaging randomly, scary stuff right there. I slowly learned that less is more.
As for the other changes I would like to do, I can get them programmed on the VESC too. I agree it is easier when you already have an Arduino connected to the board, but again, I think it is worth the effort of loading all this stuff into the VESC itself.
If you are using a more powerful Arduino than mine (Nano) you might have more HW serials and you might be OK because of that, keep using the HW, can't stress that enough.
```

---
## \#57 Posted by: wafflejock Posted at: 2018-06-08T22:09:55.140Z Reads: 105

```
Gotcha saw the mention of software serial earlier but didn't grok why you were using it originally.  The pro mini are just missing the ftdi and USB connections so saves some space and the ones I have are setup for 8MHz and 3.3V (easier to power off 1S lipo without boost), instead of 16MHz and 5V for the typical Arduino.  Ultimately looking at the data sheet for the particular atmega chip on a given Arduino board is the best way to know what it has available.

Anyhow I'm just using the metr Bluetooth module (new version just made I have the old one but will probably upgrade it) for getting data from the VESC but makes more sense with what you want to do to have the direct connection.  @solidgeek has "telemetry" data from the VESC sent to it as well so maybe can look over his code too for some ideas of how to do it.  I noticed in my testing the response on the 8Mhz Arduino is better when I removed all the serial debugging after things are working.
```

---
## \#58 Posted by: TheFluffiest Posted at: 2018-06-08T22:27:54.363Z Reads: 99

```
I certainly don't have the electrical or programming skills to do that unfortunately, although it would be a pretty cool thing to learn!
```

---
## \#59 Posted by: skelstar Posted at: 2018-06-19T00:27:04.960Z Reads: 101

```
Hey, lots of reading that I haven't done but I'm doing something similar to what you're doing but not with an FSR (ie arduino in remote -> nrf24L01 -> arduino on the board translating commands for the VESC), and I was using an ESP32s.

I was having issues with the code doing a lot of things at once (mostly in the remote) and remembered that the Esp32 has two cores (actually three). It's _totally_ worth reading about it. Now one core is responsible for reading buttons, and the other core is responsible for talking to the board.

It's. So. Fast.

Also the ESP32 has multiple hardware serial ports :)
```

---
## \#61 Posted by: ofekp Posted at: 2018-06-21T20:57:10.795Z Reads: 98

```
It’s mostly used for IOT since it has Wi-Fi, don’t you think this is an overkill?
Are you using the WiFi capability?
I like the fact that it has multiple cores, though.
```

---
## \#62 Posted by: wafflejock Posted at: 2018-06-21T21:03:27.456Z Reads: 103

```
Yeah I really need to get some ESP8266 based stuff to see how it works in practice myself.  I've heard there can be issues with latency from the wifi but I wonder if that is just if using TCP and UDP would be sufficient... anyway I never tried myself and given I'm running the Arduino's at 8MHz and still works fine I kind of feel like it shouldn't be that bad to do on a much more powerful chip, that said you do have to feed it more energy so there is that down side.  I've had lots of luck I guess with the NRF chips, it did take me quite a bit of failing at first but have had a pretty solid setup for a couple of years now so for now just not fixing something that isn't broken.
```

---
## \#63 Posted by: skelstar Posted at: 2018-06-21T21:49:54.493Z Reads: 101

```
I'm not using the Wifi capability. 

Plan to (this weekend) use wifi and use [Blynk](https://www.blynk.cc) so that I can see some data on my phone that I don't need in real-time/in-flight.
```

---
## \#64 Posted by: skelstar Posted at: 2018-06-21T21:53:08.795Z Reads: 96

```
I tried UDP, TCP and had latency issues (maybe I wasn't doing it right). Tried websockets last weekend but my arduino IDE setup was causing issues. Using these technologies are really only so I can get rid of the RF24 chip/board in my remote.

ESPNow is another thing I tried (I think it's a websocket)... and BLE, but the BLE/BT stack wasn't mature with ESP32 at the time (and probably still not there).
```

---
## \#66 Posted by: ofekp Posted at: 2018-06-23T09:26:08.355Z Reads: 84

```
Why do you want to remove the NRF24? Is it causing you issues?
You plan to have a WiFi based communication?
```

---
## \#67 Posted by: skelstar Posted at: 2018-06-23T20:17:11.495Z Reads: 84

```
Umm... I had some teething problems with nRF24 initially (hardware, not software) and I like the idea of having one less board in my remote (space, complexity). Seems to me that it is the best option (aside from the space needed).

nb: wifi seems to have too much latency in my short investigations.
```

---
## \#68 Posted by: ofekp Posted at: 2018-06-25T08:16:00.826Z Reads: 78

```
I think WiFi is not a common thing in real time remote controlers for a reason. I would stick with BT or RF. And I completely agree, having as less HW as possible is generally the best thing you can to your setup. I have said that many times throughout this post and it can't be said enough times. Having only one arduino in my remote while keeping the board "stupid" by connecting a BT module directly to the VESC made my setup stable.
```

---
## \#69 Posted by: skelstar Posted at: 2018-06-25T18:45:21.292Z Reads: 75

```
BT straight to the board. Hmmm... interesting (I haven't read all the posts sorry).

I _do_ have the option of doing some cool stuff on the board if I have an ESP32 between the remote and the VESC (lights, status indicators, tilt-sensors) but I might have to consider the advantages.

I'm guessing signal strength could be more critical with BT over RF.

Anyway :)
```

---
## \#70 Posted by: chocol4te Posted at: 2018-07-16T12:47:41.631Z Reads: 65

```
Okay, exams finished and I've been able to start in earnest. 

Here's where I am at:

[![](https://thumbs.gfycat.com/RevolvingInfiniteIrishwaterspaniel-size_restricted.gif)]()

[![](https://thumbs.gfycat.com/ZigzagHandyAtlanticsharpnosepuffer-size_restricted.gif)]()

[![](https://thumbs.gfycat.com/NiceAnimatedAmazondolphin-size_restricted.gif)]()


CC1101 radios are working - they use a lower, less cluttered frequency (lots of stuff runs on 2.4GHz meaning NRF-based remotes will be more susceptible to interference) that should result in far fewer drop outs and a more reliable remote. The SoftPot is also working as shown in the last gif (top line on display is throttle input percentage)
```

---
## \#71 Posted by: ofekp Posted at: 2018-07-16T20:27:19.203Z Reads: 57

```
Ideas can change the world :slight_smile:
I am glad to have a part in this, this looks awesome indeed.
You have 3D printer right?
Would love to compare the ride feel between this and the two FSRs I use :)
I see you use two Nanos, I hope to have this solved by connecting just one Nano in the remote and a NRF (SPI) connected directly to the VESC. BTW if you're using VESC6.0 it should be supported out of the box.
```

---
## \#72 Posted by: sunnyD Posted at: 2018-07-16T22:51:07.916Z Reads: 45

```
Niiiiiiiice. This looks incredible!
```

---
