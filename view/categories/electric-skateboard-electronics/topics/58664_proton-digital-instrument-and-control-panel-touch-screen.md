# Proton- Digital Instrument and Control Panel Touch Screen

### Replies: 351 Views: 9577

## \#1 Posted by: Wajdi Posted at: 2018-06-12T17:34:09.394Z Reads: 796

```
Hey guys,

Our Vesc powered electric skateboards are very powerful, with a lot of functionalities under the hood. 
What we were missing is way to take full control of these features at a finger tip, without the need of carrying and accessing extra hardware like smartphones.

Just like cars have instrument cluster, electric skateboards can have one too.

Introducing Proton Panel - a digital instrument and control panel that turns your ordinary skateboard into an advanced piece of machinery. ( as seen on https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/5570?u=wajdi)

Proton Panel is standalone, with a new custom hardware and software design, only requires one connection to the Vesc.

![1|625x500](upload://rxqjWQjc8P8ekpZXb7bp1QEZWQr.jpg)
![Longboard_2018-Jun-20_05-40-36AM-000_CustomizedView9780571581|690x480](upload://q2U0StXA3g0VoyHrVD5mm8cANV4.jpg)
![3|625x500](upload://wwX9P4ar2yxwIPRpdaZ116Yaskb.jpg)
![Longboard_2018-Jun-11_12-15-29AM-000_CustomizedView29942209180_jpg|625x500](upload://ePKLbjFnjR7LpwPptub3fecGeEz.jpg)![Longboard_2018-Jun-11_12-46-51AM-000_CustomizedView8771056540|625x500](upload://1Tz9f3bQBamtRmD2gZiPUnFOGT3.jpg)

**Some of the key features:**

* Touch screen - 240x320 2.8" 
* Real time telemetry right at your sight all the time ( Speedometer, battery voltage, temperature, traveled distance..)
* Built in USB charger
* Menu with different settings and options to adapt to your own configuration.
* Dual UART port for dual Vesc support
* Firmware updates through built-in micro USB, always up to date with latest Vesc changes. 
* Built in LEDs driver with touch color picker, effects, front and back lights
* Easy to access and configurable riding preset modes.
* Benchmark mode 
* Configurable sound alerts for low voltage, power on, ...
* Miles/Km units
* Ultra fast refresh rate
* Does not require the Photon remote or receiver, works with any standard remote

**Current Status:**

I have been working on this project for the past few months, I have built and tested prototype units with great success. Right now I finished most of the hardware design, still adding and improving on the software, if you want a feature added or have any suggestion please let me know.

**Price and release date:**
Since this is still a work in progress, I don't have a price set yet. I'm going to have the PCBs fabricated and assembled by a manufacturer to reduce the production time, handle large quantities, and offer the best hardware quality. I have a PCB manufacturer ready and they will quote me a production price once I get the design finalized. I estimate this project to be ready in about 1.5 months from now.

Thank you for reading through, I hope this can be useful for the community!
```

---
## \#2 Posted by: brenternet Posted at: 2018-06-12T17:51:24.845Z Reads: 649

```
Well.. this is interesting. Telemetry for those of us who don't like thumb controls as much ;)

Does is store total mileage? If so how is it doing that?
```

---
## \#3 Posted by: Wajdi Posted at: 2018-06-12T17:53:25.679Z Reads: 643

```
@brenternet Yes it stores total mileage, and it can be reset anytime from the menu. It is stored in the MCU flash, stays saved even after power cycle.
```

---
## \#4 Posted by: moon Posted at: 2018-06-12T17:54:36.619Z Reads: 630

```
What display are you going to use? Is it good enough in sunlight and weird viewing angles
```

---
## \#5 Posted by: brenternet Posted at: 2018-06-12T17:55:56.184Z Reads: 605

```
Very useful. What is the overall size of the enclosure/case and is this the design you've settled on?
```

---
## \#6 Posted by: Wajdi Posted at: 2018-06-12T18:04:54.050Z Reads: 589

```
@moon I'm using the widely available 2.8"  240x320 Tft display, the touch screen actually helps reducing glare. It is pretty bright. Almost all 2.8" displays share the same screen, just re-branded.
The display is clearly visible when viewed from above or normal standing position.
@brenternet The enclosure dimensions are about 90 mm x 66 mm x 12 mm, just enough to hold the hardware in. There might be minor changes, but nothing major.
```

---
## \#8 Posted by: Battosaii Posted at: 2018-06-12T18:10:09.020Z Reads: 545

```
That looks really cool but flipping the deck upside down on the ground on purpose or by accident looks like it can damage or scratch the screen. I often put my boards in strange position at home or in the car.
```

---
## \#9 Posted by: Wajdi Posted at: 2018-06-12T18:12:11.233Z Reads: 541

```
Screen will actually be more protected than on the rendering photos, it stays under the frame slightly with enough bezel to prevent direct contact.
```

---
## \#10 Posted by: SuperBen Posted at: 2018-06-12T18:14:01.279Z Reads: 524

```
Following, this is an awesome idea and the larger screen should be nice and easy to see on the front truck
```

---
## \#12 Posted by: Mobutusan Posted at: 2018-06-12T18:16:05.228Z Reads: 517

```
Cool project. You could also add an integrated raised foot stop/screen protector to the front of the frame/bezel. Keep the screen from getting stepped on too.
```

---
## \#13 Posted by: Wajdi Posted at: 2018-06-12T18:18:20.625Z Reads: 503

```
As crazy as it sounds, I have actually rode my board in a very rough environment without doing a single damage to the device. I dropped my board several times as well, no issues. The design is very simple and rigid.
Think about how complicated your VESC electronics are, yet they still survive.
```

---
## \#14 Posted by: Deckoz Posted at: 2018-06-12T18:18:29.513Z Reads: 494

```
I was actually going to suggest using a metal base plate, with threaded bumpers that stick up 1/2" or so on the four corners of the screen. So it can't get smashed when I run into a bridge and flip my board over trying to do an electric Casper slide. Haha
```

---
## \#15 Posted by: Ebisane9 Posted at: 2018-06-12T18:18:39.559Z Reads: 472

```
I actually like this, no need for voltage display on the enclosure. Could call for larger battery configs in small enclosures perhaps.

Edit: Any idea of an ETA? and will this be connected to the ppm port? if so what about users using split ppm who happen to be using both ports for monitoring. the data registered would only show for one vesc if not by canbus right? @Wajdi
```

---
## \#16 Posted by: Wajdi Posted at: 2018-06-12T18:20:48.031Z Reads: 459

```
@Mobutusan @Deckoz Cool ideas :smiley:  There are several ways one can customize this.
```

---
## \#17 Posted by: Deckoz Posted at: 2018-06-12T18:21:57.797Z Reads: 470

```
[quote="Ebisane9, post:15, topic:58664"]
if so what about users using split ppm who happen to be using both ports f
[/quote]

He had mentioned 1.5 months.

But it will be a uart device like Bluetooth to aquire vesc telemetry packets. Ppm still functional.
```

---
## \#18 Posted by: Ebisane9 Posted at: 2018-06-12T18:25:04.730Z Reads: 451

```
excitement had me skipping over.
Thanks @Deckoz and @Wajdi. I meant UART. for split ppm we only get telemetry per vesc, well at least with ios apps we don't get the "double values" option. This would read telemetry for only one vesc, meaning two for one board. which is ridunculous.
```

---
## \#19 Posted by: brenternet Posted at: 2018-06-12T18:25:26.608Z Reads: 452

```
@Wajdi Would there be a chance now that this has been created for collecting telemetry that you would consider building a simple, ergonomic, no need for modding, reliable, preferably trigger based, molded remote to go with it? You clearly have the skills and I think it's clear the market is there.

Do your bank balance a favor and put some time into a project like this, for the love of eskate!
```

---
## \#20 Posted by: Wajdi Posted at: 2018-06-12T18:35:26.047Z Reads: 458

```
@Ebisane9 Dual vesc setup is supported. The monitor does in fact have two UART ports, to connect to both vescs at the same time. 
@brenternet Thanks for the suggestion, I will try :smile:
```

---
## \#21 Posted by: Jc06505n Posted at: 2018-06-12T18:38:34.312Z Reads: 453

```
Ouff, Thinking this could work with the Jet Spud... very tempting. Is there any kind of hardware device that would allow two devices to be plugged into the VESC's UART? or maybe the ability to connect via Bluetooth? (hint hint METR application support)
```

---
## \#22 Posted by: brenternet Posted at: 2018-06-12T18:41:27.854Z Reads: 428

```
No screens, no bells or whistles! Just make it look good and work!
```

---
## \#23 Posted by: Wajdi Posted at: 2018-06-12T18:41:28.392Z Reads: 393

```
@Jc06505n I thought about this when I was designing it, thats why I added a secondary UART port on the panel. That way you can connect your Bluethooth module to it, or whatever needs access to UART.
```

---
## \#24 Posted by: Jc06505n Posted at: 2018-06-12T18:46:08.471Z Reads: 375

```
Ohhhhh you sexy genius. Would the port be on the side , inside, under? This is def a forsure buy.
```

---
## \#25 Posted by: Wajdi Posted at: 2018-06-12T18:47:47.651Z Reads: 377

```
Both ports will be on the side for easy access :+1:
```

---
## \#26 Posted by: i2oadsweepei2 Posted at: 2018-06-12T18:48:12.352Z Reads: 382

```
I would use this while riding and use my metr module for records and making over layed videos. I’m assuming this could be connected to my slave vesc and it won’t interfere with my metr pro module?

Anyway long way to go here. Watching 👍
```

---
## \#27 Posted by: Acido Posted at: 2018-06-12T18:50:20.663Z Reads: 371

```
Tell me its waterproof and i will buy one :D
at least partly like splashes
```

---
## \#28 Posted by: Wajdi Posted at: 2018-06-12T18:52:56.033Z Reads: 366

```
@i2oadsweepei2 Yes it will work on your slave vesc, it won't interfere with  your metr pro module because its connected to your other vesc.

@Acido No waterproofing so far, however feel free to mod it the way it suits you.
```

---
## \#29 Posted by: High-roller Posted at: 2018-06-12T18:57:10.267Z Reads: 372

```
Let me see if I have this right- can I connect my vescs to the computer through this to enter my initial settings, motor detection, etc? Do I even need to or is it powerful enough to run a vesc-tool by itself?
```

---
## \#30 Posted by: Wajdi Posted at: 2018-06-12T19:00:30.353Z Reads: 379

```
@High-roller I believe initial setup such as motor detection and limits aren't frequently changed and should be done only once. This device is meant to be used for everyday needs, switching between different riding modes fast and easy. Therefore it wont have initial setup built in.
```

---
## \#31 Posted by: zyphaz Posted at: 2018-06-12T19:09:43.342Z Reads: 366

```
I question how useful the live statistics will be, down on the board and not directly in my FoV.   Still I want one badly, oh so badly I want one!
```

---
## \#32 Posted by: TheMachine Posted at: 2018-06-12T19:42:01.101Z Reads: 373

```
Car gagues often have the same problem (don't want to be looking at the gagues at WOT).  A rolling histogram is great for this, as it lets you see the last few minutes/seconds/whatever clearly and quickly.
```

---
## \#33 Posted by: zyphaz Posted at: 2018-06-12T19:56:52.682Z Reads: 364

```
A rolling histogram as the speedo/amps/etc wouldn't photograph as well, but as mentioned it'd be worlds more useful.
```

---
## \#34 Posted by: Acido Posted at: 2018-06-12T19:57:01.142Z Reads: 376

```
yeah but looking on a car gauges is much easier and safer than on a skate :smiley:

We need something like Ironman has in our full face helmets ![Iron_Man_Mark_VII_HUD_design_By_Jayse_Hansen_1400|690x388](upload://wskUnHNCwiwkhi956Ty841pp2Ol.png)
```

---
## \#35 Posted by: Jc06505n Posted at: 2018-06-12T20:04:09.287Z Reads: 369

```
[quote="Wajdi, post:28, topic:58664"]
No waterproofing so far, however feel free to mod it the way it suits you.
[/quote]


Ouff, waterproofing is important for any external electronic equipment for our boards. Especially when one can get caught in the rain, or trying to clean their boards. Would be a hassle to unscrew every time you need to hose it down. Waterproofing should be an aim for ESK8 by now.
```

---
## \#36 Posted by: Wajdi Posted at: 2018-06-12T20:17:10.400Z Reads: 347

```
Waterproofing wont be difficult to be honest, there are no buttons so less things to worry about. Perhaps if someone has idea on how to cheaply mass waterproof this things I'm a taker :smiley:
```

---
## \#37 Posted by: anorak234 Posted at: 2018-06-12T20:19:11.124Z Reads: 350

```
Integrated rubber gaskets sandwiched at the edge of the display and between the area on the bottom of the unit and the board - sealing all electronics. Just find the right length and then use small amounts of glue to keep it in place - but make sure when pressure is applied that it keeps a full seal. Also if you’re going to 3d print this one, it’d be better to plastidip all of it and then put the gaskets for 100% waterproofing.
```

---
## \#38 Posted by: strattos Posted at: 2018-06-12T21:12:58.895Z Reads: 342

```
It exists, kinda there's a company Aecon that makes goggles and glasses that run android and have a display.

Definitely considered ripping it out of my goggles to try and Jimmy rig my pass, but I should probably finish my boards first lol.
```

---
## \#39 Posted by: TheMachine Posted at: 2018-06-12T22:59:02.705Z Reads: 332

```
For sure this you'd still need to stop to look at.

The projector tech is there, it's about hacking it into a helmet.  Anyone have a Google Glass that still works?
```

---
## \#40 Posted by: Toughook Posted at: 2018-06-15T13:04:51.970Z Reads: 318

```
Oakley make Goggles with heads-up dsiplay inside. Granted you'd look a bit daft wearing them in the summer, butthe tech is out there already :)
```

---
## \#41 Posted by: banjaxxed Posted at: 2018-06-15T15:26:11.641Z Reads: 333

```
It's really nice. After all the phone developments and the no doubt incoming wristwatch ports of all the apps I'd been looking at board based meyers and meh

But this is slick, sell it at a price to make it ubiquitous on most boards huh and not just the prized board?

Nice job
```

---
## \#42 Posted by: Jc06505n Posted at: 2018-06-17T14:08:29.300Z Reads: 343

```
Anyway for a SD port to be added to save lifetime telemetry (I.e lifetime odometer).


The data could be compiled to see data that we usually don’t get to observe Over the course of a VESC’s lifetime, such as the hottest its ever been , the average Wats consumption over its lifetime, the amount of faults, top lifetime speed , displacement travels etc.

Edit: or even Bluetooth Capabilites (one might say this is redundant since it already has a UART port for Bluetooth Mods, but it would skip the Need for an SD Port )that’ll allow Lifetime Data to be wirelessly transferred to a webpage similar to the mertr page that visually displays thedata. People like @Ackmaniac could allow for the data to be transferred and displayed on their app.
```

---
## \#43 Posted by: Kug3lis Posted at: 2018-06-17T14:50:03.103Z Reads: 311

```
This is on what I am working myself, but instead of writing hardcore data logging on small MCU I will run fully fledged data collection/aggregation system on normal platform with correct tools for the job :) Because to implement all of this on embedded MCU is a bit painful.

I like the idea of this product, I would suggest to use OLED screen as it would be better with readability and viewing angles :P
```

---
## \#44 Posted by: mikenyc Posted at: 2018-06-17T17:12:21.717Z Reads: 305

```
Why don’t you just write an iOS or android app that takes this information over Bluetooth?  There are apps that show real time information already, why don’t you just make an app that takes that same information and store it?
```

---
## \#45 Posted by: Jc06505n Posted at: 2018-06-17T18:16:08.471Z Reads: 313

```
Cause that means you always have to have your phone with you on every ride (The VESChas a limit t how many writes can be stored on its EEPROM, )  , It wouldn’t be lifetime stats per day, but the culmination of everytime you remembered to record your ride or take your phone with you. 

Since his thing is always going to be on your Board AND it’s conencted directly to the UART. Its  In the position to act as a lifetime Odometer/Stat holder in addition to its duties. Sure you can make the VESC do It, but again , it has a limit to how many writes it can do to its EEPROM.
```

---
## \#46 Posted by: Wajdi Posted at: 2018-06-17T18:27:07.939Z Reads: 295

```
@Jc06505n I agree, the display has an SD card slot already integrated. We can use it to store lifetime information on the board, and perhaps do a lot more things with it.
```

---
## \#47 Posted by: mikenyc Posted at: 2018-06-17T18:28:44.297Z Reads: 295

```
I would have thought that most people carry a phone with them all the time 🤷🏻‍♂️
```

---
## \#48 Posted by: Jc06505n Posted at: 2018-06-17T18:39:34.064Z Reads: 291

```
Awesome! Make this think Waterproof (or a case for it) and it’s a sure buy
```

---
## \#49 Posted by: Jc06505n Posted at: 2018-06-17T18:40:44.316Z Reads: 291

```
Even then I forget to turn in a tracking app or I’m too much in a hurry to. Such a feature would bypass any mistakes like that.
```

---
## \#50 Posted by: wafflejock Posted at: 2018-06-17T18:51:23.304Z Reads: 310

```
Biggest problem with doing any sort of remote is having the hardware certified to sell it legally in the US and around Europe.  The rules are strange in the US basically any intentional radiator and from what I gather basically anything with an inductor has to be fcc certified which is at least $10k from what I've read, which basically restricts it to mass production to dilute that cost.  The plastic housing can be made at scale (10k units) for $2-3 a piece with injection molding but again big up front cost of getting the master mold made by someone who knows how to design those for injection molding.  Best idea I could come up with to make this at all feasible for our relatively small market is doing kits with some assembly required and links to known good vendors for getting the radios (in the US at least you can make up to 5 devices for testing I believe, adafruit has a write up on legality with radios).  Probably 3d printing the cases either in house or using 3d print services to avoid mold making costs.

---

Also looks nice regarding the OP, would be curious how the screen holds up over the longer term.  Have seen some TFT displays on desk phones that get terrible over time but I'm unsure the root cause of that (maybe just crappy screens)
```

---
## \#51 Posted by: Exigent Posted at: 2018-06-26T22:26:58.938Z Reads: 291

```
**If possible**
You may wish to consider making it easy to replace just the screen. 
A replacment screen as a product also might be a good idea.
```

---
## \#52 Posted by: Exigent Posted at: 2018-06-26T22:39:38.920Z Reads: 294

```
I can understand not claiming "waterproof" or adding that expense.
One has to be careful on any "waterproof" claims as doing so can be a **major** legal issue in some countries when it comes to product claims.
```

---
## \#53 Posted by: uigiroux Posted at: 2018-07-02T18:47:44.755Z Reads: 287

```
I know we discussed this before, but have you thought about adding active GPS where it shows directions that it gets from your phone?  Also, will this have a power on button, so we wouldn't need to add one on the side?  Just like how this will make a voltage meter not needed anymore, it'd be great if we could also get rid of the on / off button / switch.  That'd be great if we didn't have to think about installing any of those things anymore and could just do it all with this.  Also, any chance you could incorporate a USB charge port, or 2?

With this will we not need a Bluetooth transmitter like meter since it shows the same telemetry via the UART cable?
```

---
## \#54 Posted by: Friskies Posted at: 2018-07-03T05:47:25.432Z Reads: 277

```
This kind-of seems pointless. Most people will be buying the new Bluetooth modules anyway as you can use them with the vesc tool. Good idea but if your board has Bluetooth already then you might as well use the integrated chip in the phone. I can see this being really useful for telemetry and battery monitoring but I already have that with my photo remote :stuck_out_tongue:
```

---
## \#55 Posted by: Jc06505n Posted at: 2018-07-03T05:55:23.465Z Reads: 276

```
My goal is to use this a “Main Control” unit of the board. It’ll allow me to record data whenever I ride and switch modes with ease. Wonder if I.T would be possible to implement a “lock down mode”. Makes it so if I choose, Upon the next start up , a password has to be put it and if incorrect a # of times , the motors are locked up and unridable unless the right password is put in. Won’t stop a thief from taking It but It  Sure as hell make it less valuable to them
```

---
## \#56 Posted by: Wajdi Posted at: 2018-07-03T14:39:36.651Z Reads: 286

```
@uigiroux
 Adding a USB charging port is possible. I think it will make a great addition to this control panel. 

I have looked into turn by turn navigation, but its not easy to implement. It will still require a smartphone phone to calculate navigation, and then we need to somehow send directions over bluetooth to the control display. I couldn't find an API from google maps that allows this.

I'm still thinking about a smart turn on/off system PS4 style. Nothing official yet tho.

@Jc06505n Implementing a password lock is easy, but I don't think it will have any security weight as is. To properly lock it we would need to somehow lock the firmware on the VESC. But even that can be bypassed by reflashing it. Sure it will make it harder, but still bypassable.
```

---
## \#57 Posted by: banjaxxed Posted at: 2018-07-03T15:22:34.068Z Reads: 302

```
It's possible but maybe no API as you say
https://github.com/komoot/BLEConnect
![image|612x500](upload://8nABNxiU0nJ28COWYXfcIi0QvyE.jpg)

It would kickass that's for sure

Maybes
http://www.akexorcist.com/2015/12/google-direction-library-for-android-en.html

@JTAG is using the 5v rail of the VESC to turn on the BMS and ergo the esk8. When you turn the motor manually it creates the current, which in turn can be used to turn something on - like the main battery
```

---
## \#58 Posted by: uigiroux Posted at: 2018-07-03T15:50:33.423Z Reads: 290

```
Awesome!  That would be great to have that on there.  One thing I also just thought of.  This thing with a USB charging port and possibly being able to turn it on from there kinda makes this like an all in one solution to everything you could add to a board, but I was just thinking, would it also be possible to add a charging port, for the battery, maybe next to the USB charging port?  That would literally make this an all in one solution, and be the only thing one would need to hook up to operate every aspect of the board!  On/off control, battery charging power, and USB charging port, along with display that shows all telemetry and battery status, this would be perfect!! :heart_eyes:
```

---
## \#59 Posted by: Wajdi Posted at: 2018-07-05T10:03:37.931Z Reads: 303

```
![Longboard_2018-Jun-20_05-40-36AM-000_CustomizedView9780571581|690x480](upload://q2U0StXA3g0VoyHrVD5mm8cANV4.jpg)

Almost done finishing LED control settings
* Different effect modes will be available.
* Color picker 

![Longboard_2018-Jun-20_05-40-36AM-000_CustomizedView9780571581|690x480](upload://jIZsKVLIADMwczp4lKzJSsyGjsB.jpg)

Endless ride or push assist implementation, I posted a while back on some other thread.
* “Assist.” Controls how long the power assist will last in seconds. Default to 30 sec.
* “Threshold” Controls the activation threshold, after pushing and reaching this speed, power assist will kick in.
* “Deceleration” This controls the rate at which the deceleration decay happens. For example at 30 rotations per seconds as the mellow boards have it implemented.

Development and testing are almost done, I will be finalizing project files for manufacturing soon.
I anticipate to start pre-orders by Mid July, and start fulfilling orders by August.
```

---
## \#60 Posted by: Friskies Posted at: 2018-07-05T11:40:50.681Z Reads: 292

```
Annnnd now I want one...
```

---
## \#61 Posted by: Jc06505n Posted at: 2018-07-05T11:48:31.398Z Reads: 291

```
How does wiring work in regards to the cable such as length? I can see it working with the tunnel risers by drilling a hole in the middle of the truck holes and routing it to the enclosure.
```

---
## \#63 Posted by: SeanHacker Posted at: 2018-07-05T13:16:54.736Z Reads: 287

```
Just tell me a price and I'll most likely be buying 2 or 3. This is going to be awesome! Thanks @Wajdi for the cool shit you've been bringing to the table here.
```

---
## \#64 Posted by: uigiroux Posted at: 2018-07-05T13:51:29.427Z Reads: 272

```
USB charging port?
On/off switch? 
Battery charger port? 
:smile:. :smile: :smile:
```

---
## \#65 Posted by: Wajdi Posted at: 2018-07-05T15:19:44.349Z Reads: 273

```
@uigiroux
USB charging port will be available.
Regarding battery charger port and On/Off switch it will be hard to fit those on the device, they are more BMS related. Maybe a case mod for those interested.
Pricing: An approximate price will be posted in about a week.
```

---
## \#66 Posted by: uigiroux Posted at: 2018-07-05T15:22:33.006Z Reads: 273

```
That's great, thanks so much for implementing the USB port, I think that'll be a great addition to the unit!  Definitely put me down for one :smile:
```

---
## \#68 Posted by: Wajdi Posted at: 2018-07-20T17:17:47.409Z Reads: 270

```
Almost there, I will try to finilize the design tonight and approximate the production cost.
```

---
## \#70 Posted by: uigiroux Posted at: 2018-07-23T17:26:40.475Z Reads: 274

```
Another question.  I had been planning on getting a Bluetooth set like the metre pro for telemetry on my phone.  Would this provide the same things, thus making the need for a Bluetooth module obsolete, in a sense?  Cause if they both do the same thing, I'd rather have this, then have to get the Bluetooth module and then always have a smart phone with me to be able to use it...
```

---
## \#71 Posted by: uigiroux Posted at: 2018-07-25T18:26:38.382Z Reads: 264

```
Any updates...?
```

---
## \#72 Posted by: Mich21050 Posted at: 2018-07-25T19:40:56.976Z Reads: 266

```
@Wajdi Anything new? :smiley:
```

---
## \#73 Posted by: Wajdi Posted at: 2018-07-25T20:34:08.093Z Reads: 278

```
I have been working on implementing a built in DC DC buck converter to easily and efficiently step down battery voltage, offer a high current power source for LEDs and to power the USB charger. It should handle an input range up to 55V and output both 12v and 5v rails. 

I have been debating whether to have this built in or just leave it as an external component for everyone to use their own.
```

---
## \#74 Posted by: uigiroux Posted at: 2018-07-25T21:22:54.913Z Reads: 272

```
I'd definitely prefer it built in personally.

Would leaving it external mean having it wired up, but not mounted on the Proton, so we could use the USB ports from in the enclosure and mount it where we want?  That would also be nice..  Any way to do both?
```

---
## \#75 Posted by: Friskies Posted at: 2018-07-26T05:15:28.239Z Reads: 253

```
The external component would be great.
```

---
## \#76 Posted by: Wajdi Posted at: 2018-07-26T09:10:31.756Z Reads: 250

```
Everything will be the same except the buck converter module will be external.

Upon further thinkering, I think leaving it as an external module is better because it will be easier to replace it in case it blows up instead of loosing the whole control panel. They also tend to get very hot under load, especially when using high voltages like 10 and 12s. It will also makes it easy to upgrade it in case more power is needed.
```

---
## \#77 Posted by: uigiroux Posted at: 2018-07-26T11:44:15.790Z Reads: 245

```
Ok yeah that's certainly a smarter way to do it.  So then it would have those external and we would basically run them into our enclosure to mount, correct?
```

---
## \#78 Posted by: Wajdi Posted at: 2018-07-26T12:08:32.358Z Reads: 237

```
Yes that’s correct, the buck converter can be placed inside the enclosure to save space.
```

---
## \#80 Posted by: Wajdi Posted at: 2018-07-27T09:47:37.917Z Reads: 250

```
I’m trying to finalize the hardware as much as possible to give an accurate estimate, at the same time finding ways to keep the production cost at a minimum. I should have an estimate in the next 48 hours.
```

---
## \#81 Posted by: Wajdi Posted at: 2018-08-01T16:11:58.434Z Reads: 258

```
Updated renderings with USB chargers.
![47%20PM|690x321](upload://o9RRvqZFXzaGJKAbK8QBZ9zg5fI.jpg)
![57%20PM|690x322](upload://sNuXYfUOJtQxOyp4xTyOI7u7eJK.png)![54%20PM|689x321](upload://lOHrhFJ5MHh7jE9Kb1XolEasboz.jpg)![17%20PM|690x322](upload://n7DRAIFK8UsDmUl6nuy6NDu82uC.jpg)![15%20PM|689x323](upload://7TW5AA0dgUwkh0sA0qBWjHEvJRc.jpg)

Buck converter module will be an additional add-on, it is only needed if you want to use the USB chargers and drive LEDs, otherwise, the control panel can be fully powered using the UART cable.

Estimated production price will be based on how big is the batch. Coming up soon.
```

---
## \#82 Posted by: uigiroux Posted at: 2018-08-01T16:16:10.749Z Reads: 253

```
Dude that looks amazing!  Will there be water proof covers for the USB chargers? Or just covers in general that'll fit flush against the instrument panel?

I noticed on the top left there is a large empty area next to the display.  Will there be buttons or something there?  Otherwise wouldn't the display be centered?  Can't wait for more info on this :heart_eyes:

Also, where do the wires that will run to the vesc or battery come out from?  The bottom would be ideal for easy concealment.

I know you didn't want to make this have a on/off button and charger port, but would it be possible to create a case for this that is a bit extended and empty so we could put our own on /off button and charger port in the module without having to put another thing on the other side of the board.  That way this could be truly a all in one device.
```

---
## \#83 Posted by: Wajdi Posted at: 2018-08-01T16:25:16.076Z Reads: 253

```
@uigiroux Thanks! I think it should be easy to make it water resistant using USB covers, and put some sort of a rubber seal at contact area with the deck.

About the display offset, thats because of the dimensions of the screen
![GVXXXXXuapXXq6xXFXXXy|323x230](upload://el4rrOco7jL2gOpzoDQCWzgYEon.jpg)

Wires will run through a bottom tunnel.
```

---
## \#84 Posted by: uigiroux Posted at: 2018-08-01T16:28:40.863Z Reads: 252

```
Can you give a detailed description of all this will be able to do again please?
```

---
## \#85 Posted by: i2oadsweepei2 Posted at: 2018-08-01T16:31:04.714Z Reads: 253

```
I believe most of it is in the first post. He just updated it four days ago. Let’s let him work.
```

---
## \#86 Posted by: uigiroux Posted at: 2018-08-01T16:35:40.797Z Reads: 256

```
I know the original functions were listed in the first post, but as there has been quite a few new features and developments, I was wondering if there was new features or ones that may not have been listed originally. :slight_smile:
```

---
## \#87 Posted by: Wajdi Posted at: 2018-08-01T16:50:05.592Z Reads: 256

```
There is an alternative 3.2 inch lcd with the same pixel resolution of 320x240, however I don't think if it's worth the change. 
![HTB1H37hQFXXXXcJXFXXq6xXFXXXA|500x500](upload://7okwPFZcczsCzVD0W5i7bvNrhV7.jpg)
```

---
## \#88 Posted by: uigiroux Posted at: 2018-08-01T16:53:03.799Z Reads: 246

```
I see that this can work with a single or dual VESC, but what if you're running 4WD?
```

---
## \#89 Posted by: Wajdi Posted at: 2018-08-01T16:56:18.776Z Reads: 253

```
You can have them connected on CAN bus, and plug the masters to the controller.
```

---
## \#90 Posted by: Wajdi Posted at: 2018-08-04T14:24:23.665Z Reads: 264

```
I rearranged the USB ports to make the design slimmer.

![10%20PM|689x324](upload://3QTOHhEIrLKtKm6gOOhVZhOBGIH.jpg)

New Design.
![04%20PM|690x161](upload://2hULxTUh26gWZv6jhBxMPy2MIx2.png)

Old Design
![14%20PM|690x168](upload://nLpgkrtLZ8CgJT6q2DtbZGaXwiX.png)
```

---
## \#91 Posted by: kylem21 Posted at: 2018-08-04T14:55:27.689Z Reads: 254

```
Looks great! What kind of cable would be used to connect this to the UART ports on the vescs? Just two JST cables?
```

---
## \#92 Posted by: uigiroux Posted at: 2018-08-04T15:20:26.204Z Reads: 253

```
Love this! Were you able to get a production estimate?
```

---
## \#93 Posted by: Wajdi Posted at: 2018-08-04T15:33:58.505Z Reads: 245

```
@kylem21 Yes regular JST cables as usual.
@uigiroux Almost there, I will post an estimate using different batch quantities.
```

---
## \#94 Posted by: uigiroux Posted at: 2018-08-06T18:20:02.033Z Reads: 244

```
Lol, just dying to learn more about this!  Just love the idea so much! :heart_eyes:
```

---
## \#95 Posted by: mackann Posted at: 2018-08-09T21:05:03.941Z Reads: 253

```
Wow, this look so great! Cant wait to get one of this!
```

---
## \#96 Posted by: ElskerShadow Posted at: 2018-08-10T10:36:58.202Z Reads: 245

```
Jumping late here, very exciting news !
```

---
## \#97 Posted by: Skunk Posted at: 2018-08-10T11:21:01.440Z Reads: 247

```
Very cool.  
So it's using the truck hardware for mounting it looks like. Any thoughts on making a spacer or mounting bracket for decks mounted drop through? And how that might affect the wire placement? 
Also I'm guessing it's safe  to assume the case is being made strong since the hardware for the skateboard trucks needs to be torqued down fairly hard.
```

---
## \#98 Posted by: uigiroux Posted at: 2018-08-10T12:23:04.491Z Reads: 260

```
I was wondering about this too.  For regular mounting, I was wondering if the top side screws could be the type that are hollow and allow for another screw to screw into the top of that screw.  So you would mount your trucks like normal, then just screw over the top of that the Proton, and they'd attach into the trucks screws.

Like this, but with the proper types of screws, not these. 

![Screenshot_20180810-072518_Chrome|502x500](upload://tS2OazRXRGhfUyctLWPiCEXsuLT.jpg)

Though a special type of mounting plate for drop through style trucks would also be very useful too.  One thing that worries me that Hummie said about the decks, is that the tips of the ends of the board often split open when they hit something. So I was wondering if a bash guard for the fronts of these could be made which also acts as a mounting plate for the top of the board.
```

---
## \#99 Posted by: Wajdi Posted at: 2018-08-10T12:42:21.833Z Reads: 243

```
@Skunk Drop through decks should be no different, if not favorable. Because you can insert the wiring through the deck without the need to drill. 
A tunnel riser might be needed, something similar to this https://www.electric-skateboard.builders/t/official-riptide-sports-custom-esk8-tunnel-riser-group-buy-last-chance-at-discounted-price/57359.

In regards to the case hardware, a washer can be used to spread the force, it should work fairly well.  

@uigiroux That should also work.
```

---
## \#100 Posted by: uigiroux Posted at: 2018-08-10T12:47:48.027Z Reads: 237

```
Do you have estimates on price yet please???
```

---
## \#101 Posted by: Wajdi Posted at: 2018-08-10T12:48:58.639Z Reads: 232

```
I submitted the design and I'm waiting for the quotes.
```

---
## \#102 Posted by: SeanHacker Posted at: 2018-08-10T12:51:42.448Z Reads: 238

```
Damn dude. You've asked this a million times already in this thread. Do you not think @Wajdi will release a price once he has one?
```

---
## \#103 Posted by: ElskerShadow Posted at: 2018-08-10T16:28:04.374Z Reads: 239

```
Classic shit from him hahaha
```

---
## \#104 Posted by: Riako Posted at: 2018-08-10T16:34:45.855Z Reads: 244

```
Gorgeous idea !! I missed a lot here, just seeing your pics before !
This is crazy good work, thanks for us :blush:
 Tracking mode on :smile:
```

---
## \#105 Posted by: Skunk Posted at: 2018-08-10T17:07:06.351Z Reads: 238

```
[quote="Wajdi, post:99, topic:58664"]
Drop through decks should be no differe
[/quote]
  The top of the deck would not be flat when mounted on a drop through. (Unless you're not mounting drop) you would be mounting it directly to the trucks baseplate and any overhang would have a gap between display and deck.
```

---
## \#106 Posted by: uigiroux Posted at: 2018-08-10T17:17:54.396Z Reads: 238

```
This was my thinking too.  It seems for a drop through deck setup you'd need some sort of plate that would fit around the top of the trucks that are above the deck so that the Proton could be mounted on a flat surface.  Otherwise, as you said, there would be a gap between the module and the deck since it'd be raised up from the drop through trucks.
```

---
## \#107 Posted by: Wajdi Posted at: 2018-08-10T17:29:56.045Z Reads: 227

```
I was thinking about top mounting the trucks on a drop through deck.
```

---
## \#108 Posted by: Friskies Posted at: 2018-08-11T06:13:36.545Z Reads: 232

```
I think there are only a handful of setups that actually support drop through anyway. Most people here will be top mounted for obvious reasons.
```

---
## \#109 Posted by: Wajdi Posted at: 2018-08-29T20:34:52.305Z Reads: 249

```
Hey guys,

I finally managed to get a production quote for the controller, pre-orders will have a **discounted price of $99** for a **limited time only**, **instead of $117**.

**_Now available on https://eboardshop.net_**

![35874743-0d87-4674-8c17-018c882b9089|589x444](upload://4LTkmBLmNXMbXNhuExKyglMJF64.PNG)![aa327104-5d04-4da9-ab1e-f11a73ec31bc|690x316](upload://qXA9YtCgLU8tsf7ZeCmLn9otpij.PNG)![Longboard_2018-Aug-25_03-35-15PM-000_CustomizedView14167382991|690x420](upload://4oeb20QilZlNlHOw9m3TuCBezrx.png)![a32166cf-2107-4e0d-a064-41e510ab4f3b|625x500](upload://73ftnuFceShnfUMIdUHgJQEWWjs.jpg)

Pre-orders will be shipped in about 24-26 days. 
In order to power the USB chargers and LED drivers, an external 5V buck converter is needed. They are generally cheap and can be bought for about $3-5.

I'm making a demo video, it should be up in a few days.
```

---
## \#110 Posted by: Jc06505n Posted at: 2018-08-29T20:40:57.257Z Reads: 235

```
Welp, there goes my paycheck
```

---
## \#111 Posted by: uigiroux Posted at: 2018-08-29T20:46:38.719Z Reads: 234

```
Well that's probably the fastest I've ever acted towards making an Esk8 purchase, lol.  This looks amazing, can't wait!!!  :heart_eyes:
```

---
## \#112 Posted by: Silverline Posted at: 2018-08-29T21:02:17.724Z Reads: 234

```
Does it need UART connections between vesc and proton ?
```

---
## \#113 Posted by: Wajdi Posted at: 2018-08-29T21:04:12.111Z Reads: 233

```
Yes, a UART cable will be provided.
```

---
## \#114 Posted by: mackann Posted at: 2018-08-29T21:14:01.055Z Reads: 232

```
Ordered one :) can you link any converter you could recommend?
```

---
## \#115 Posted by: Silverline Posted at: 2018-08-29T21:14:30.043Z Reads: 225

```
Thanks. Looking forward to the video
```

---
## \#116 Posted by: kylem21 Posted at: 2018-08-29T21:50:11.083Z Reads: 227

```
If you are running a dual setup, can we just connect to the master and get full functionality?
```

---
## \#117 Posted by: Wajdi Posted at: 2018-08-29T22:02:54.742Z Reads: 228

```
@mackann Thank you for your support :slightly_smiling_face:  There are several step down converter available, I didn't test one specifically but you generally should look for one that has input range similar to your battery voltage, outputs 5V, and offer around 2-3A of current. Here is an example https://www.ebay.com/itm/10V-50V-to-5-35V-DC-Buck-Module-Step-Down-Converter-synchronous-rectification/142322471378?hash=item21231491d2:g:CfUAAOSwTM5Y0lMG
@kylem21 Yes, you can just connect the master.
```

---
## \#118 Posted by: uigiroux Posted at: 2018-08-29T22:31:28.888Z Reads: 222

```
This is probably a long shot, but is there a way to make like a rubber plug/cover for the USB ports to slightly protect them from water and such?
```

---
## \#119 Posted by: Jc06505n Posted at: 2018-08-29T22:32:06.167Z Reads: 232

```
That sorta things been around since the usb existed, search around and I’m sure you’ll find them.

Less than 10 seconds of searching ![image|281x500](upload://swEZSwuqcDs89GlI08xchoKMBbp.jpg)
```

---
## \#120 Posted by: uigiroux Posted at: 2018-08-29T22:32:43.106Z Reads: 226

```
Well yes I realize that, but one that is specific to this design is what I mean.
Haha, ok ok I get it.  I'm being lazy. :blush:
```

---
## \#121 Posted by: Jc06505n Posted at: 2018-08-29T22:34:44.064Z Reads: 219

```
His design is just two USB ports. Nothing special about the integrals , nor would it costly make sense to have someone manufacture or make a 2 tab usb cover
```

---
## \#122 Posted by: uigiroux Posted at: 2018-08-29T22:36:50.389Z Reads: 226

```
I don't know how to get that done, lol.  Would you know how to get one of those made??
```

---
## \#123 Posted by: Brdchris Posted at: 2018-08-29T23:08:21.320Z Reads: 226

```
Needs Bluetooth and to be rechargeable
```

---
## \#124 Posted by: Wajdi Posted at: 2018-08-29T23:21:34.962Z Reads: 232

```
@uigiroux They are already made and available online, you can get a dozen for around $3-4 https://www.ebay.com/itm/10pcs-Black-PC-Laptop-USB-Plug-Cover-Stopper-Rubber-Soft-Silicon-Dust-Cap-H-P/142774376695?epid=2274495062&hash=item213e0418f7:g:YGoAAOSw3GtZxh1B
Or 5 for about $1 from china. https://www.ebay.com/itm/5-Black-RUBBER-SILICONE-ANTI-DUST-USB-PLUG-COVER-STOPPER-for-Computer-Laptop-/151535506013?_trksid=p2349526.m4383.l4275.c10#viTabs_0

@Brdchris Not sure why it needs to be rechargeable :thinking: It is powered directly when you turn on your board. Not sure why it needs Bluetooth either.
```

---
## \#125 Posted by: Jc06505n Posted at: 2018-08-29T23:46:26.362Z Reads: 221

```
To add in to what @Wajdi is saying , this is not a wireless device. It’s a terminal

Edit , ah I see what you meant now, I agree, it’s better off wireless and connected via a receiver. 

@Wajdi, would it be impossible to make a version of this thatbuses an Arduino Nano like the firefly remote does ?
```

---
## \#126 Posted by: Wajdi Posted at: 2018-08-30T00:21:32.587Z Reads: 219

```
@Jc06505n I still don't understand the purpose of your request, this controller has its own MCU, it does not need an external arduino.
```

---
## \#127 Posted by: Brdchris Posted at: 2018-08-30T00:23:40.152Z Reads: 211

```
We are asking what it would take to make it totally wireless. Internal battery and Bluetooth support. I would pay $30 more for that. As it stands I don’t think I want it. Purely because I don’t want to drill more holes. I love everything else about it.
```

---
## \#128 Posted by: Wajdi Posted at: 2018-08-30T00:50:45.154Z Reads: 219

```
I see your point, however it is far from what this project was initially designed for. Adding an internal battery would require additional charging hardware, power consumption would be an issue as well due to the large display and fast refresh rate. Bluetooth or nrf module would also increase the power consumption, resulting in a poor battery lifetime, requiring a lot of more hardware components and an additional receiver.

This controller is supposed to be lightweight, with minimal dependencies to get going. Its a plug in once and forget it.

There are a lot of ways to get around drilling the board. Since the Proton controller is self powered from the UART cable, there is only one cable that needs to be routed, and it is flat.
It can be wrapped from the side with minimal exposure. Depending on your board design, it can be hidden underneath the grip tape.
```

---
## \#129 Posted by: LEE Posted at: 2018-08-30T02:07:21.932Z Reads: 218

```
Can I expose the design on the back side? I would like to confirm the mounting position of UART etc. Also, when a UART cable is included, how long is it?
```

---
## \#130 Posted by: Wajdi Posted at: 2018-08-30T03:02:00.268Z Reads: 228

```
UART 1 and UART 2 ports at the bottom.
![24%20PM|425x500](upload://7ksscAHZknLctj4gxcp6lP0S9cZ.png)

UART cable will be 50cm long, thats about 19.68 inches.
```

---
## \#131 Posted by: LEE Posted at: 2018-08-30T03:37:25.942Z Reads: 227

```
There are two UARTs, how do you use the second UART?
```

---
## \#132 Posted by: Wajdi Posted at: 2018-08-30T03:40:22.189Z Reads: 225

```
Generally, you would only use one, connected to the master. The other one can be used if you are running two separate VESCs not connected through CAN bus.
```

---
## \#133 Posted by: kylem21 Posted at: 2018-08-30T03:40:52.099Z Reads: 224

```
Can you recommend an extension about 20inches to lengthen the uart cable
```

---
## \#134 Posted by: Wajdi Posted at: 2018-08-30T03:42:44.217Z Reads: 224

```
@kylem21 The longest I have been able to find so far is about 19.68 inches, I'm still looking for longer. If not we can connect two cables together.
```

---
## \#135 Posted by: LEE Posted at: 2018-08-30T04:01:26.435Z Reads: 223

```
If you use two UARTs, is the speed the average of the two UART data?
Is there a function to see output ampere etc. individually?
```

---
## \#136 Posted by: Wajdi Posted at: 2018-08-30T04:18:56.813Z Reads: 225

```
@LEE If you have both UARTs connected, then yes, the speed will be the average of the two. Amps consumption can be either set to display the total combined value of the two, or the individual reading. If you have any suggestions or requests please let me know, future software updates are easy to install.
```

---
## \#137 Posted by: DilatedPupils Posted at: 2018-08-30T06:38:28.389Z Reads: 218

```
Would it be possible to have an eMTB version? Only the mounting holes would be different I guess. And would the length of the wires connecting it to the vesc have any effect?
```

---
## \#138 Posted by: Andy87 Posted at: 2018-08-30T08:27:01.733Z Reads: 215

```
I know I can make my own UART cable or mount it somewhere else, but just to calculate for a mountain boards it´s min 80cm from the back to the front, so it will not be long enough for sure.
Are there some signal problems with that long not shielded cables?
```

---
## \#139 Posted by: banjaxxed Posted at: 2018-08-30T11:02:10.919Z Reads: 210

```
Nice I put in an order 🤫
```

---
## \#140 Posted by: Wajdi Posted at: 2018-08-30T16:44:26.512Z Reads: 214

```
@DilatedPupils Sure, if you happen to have the measurements for the eMTB mounting holes, please post it and i will add a version for it.

@Andy87 Regarding UART data over long cable, if running directly from the tx and rx pins then there might be an issue with voltage drop and noise. To solve this, I'm converting UART to RS485, which can run reliably over a couple meters long cables ( up to 1200meters ), this allows the data to flow over long distance reliably without errors.

The modules I'm using are MAX485, they convert TTL to RS-485 easily.
```

---
## \#141 Posted by: Ricco Posted at: 2018-08-30T17:48:13.914Z Reads: 211

```
What software do you use for your renderings. They look beautiful :heart_eyes:
```

---
## \#142 Posted by: Wajdi Posted at: 2018-08-30T18:06:38.197Z Reads: 225

```
@Ricco Fusion 360 :slightly_smiling_face: 
@DilatedPupils
I found the following template for Trampa's mounting holes:
![image|443x335](upload://hM4BfunShicMvjth3G1rIkexVYv.png)

It seems like it already fits the controller:

![11%20PM|684x500](upload://2tUZHeOgAsOfgNCCvv2c13xLSP2.jpg)
```

---
## \#143 Posted by: Wajdi Posted at: 2018-08-30T23:58:00.049Z Reads: 223

```
Some dimensions on mm.
![23%20PM|661x500](upload://f8AfxTvtjCwEStynxN40jL9K7FJ.png)
```

---
## \#144 Posted by: Battosaii Posted at: 2018-08-31T01:13:41.977Z Reads: 215

```
Hmm does it need to be connected to all the Vesc? Im building a 4wd and I'm gonna use split PPM with Focbox would i still be able to use this?
```

---
## \#145 Posted by: Wajdi Posted at: 2018-08-31T01:25:52.287Z Reads: 219

```
Yes you can still use it, it doesn’t have to connect to all your vescs, only the master is enough to report data.
```

---
## \#146 Posted by: Andy87 Posted at: 2018-08-31T04:54:33.503Z Reads: 221

```
The problem that the screws for the springs stay out of the deck. Depending on how tight you screw it, between 2-8mm I would say.
This in outer or inner position.
So in this case we would need to mount some spacer under (or neoprene tape etc.)
![image|595x500](upload://1OnafUSlBiy5Pvmzkf1TUQELEoS.jpeg)
```

---
## \#147 Posted by: Battosaii Posted at: 2018-08-31T09:29:09.276Z Reads: 218

```
one last question, i have an Evo i want to use this on problem is this is really wide 102mm wide and i dont think the evo is that wide and id probably have it sticking out of the sides i just cant picture how much it will stick out.
```

---
## \#148 Posted by: uigiroux Posted at: 2018-08-31T12:01:00.858Z Reads: 219

```
This is probably a bad idea but I'll throw it out there anyway.  Since the Evo has a steep drop in the front under side, maybe you could mount it there...? We likely won't be looking at it while riding, well,, quick glances at least, but you'd still be able to utilize the touch screen and all it's features.  Just couldn't see the speed as your riding.  Lol, less than optimal, but it's a thought.
```

---
## \#149 Posted by: Battosaii Posted at: 2018-08-31T12:13:27.659Z Reads: 219

```
I want a fancy way of checking my battery levels while I ride.
```

---
## \#150 Posted by: Jc06505n Posted at: 2018-08-31T12:22:19.914Z Reads: 216

```
Wouldn’t a remote or at the very least a watch be adequate for that? Sounds like a bad idea to draw your attention away from the road to look at a display done at you. 

That’s why for me I’m mounting it behind me and using it to change modes and store telemetry while i let other tools (like a remote or watch) give me quick data
```

---
## \#151 Posted by: Skunk Posted at: 2018-09-03T14:45:08.331Z Reads: 209

```
Deadline for preorder? I'm indecisive as hell. (And broke atm)
```

---
## \#152 Posted by: Battosaii Posted at: 2018-09-03T17:06:10.592Z Reads: 208

```
I ordered one but just measured my deck and its 90mm wide and this device is 101mm wide so I'll have quite a bit of overhang. Not sure if I can trim the extra of if it's too much.
```

---
## \#153 Posted by: Wajdi Posted at: 2018-09-03T17:28:44.398Z Reads: 216

```
@Andy87 A spacer in this case would solve the problem, I can help you with that.
@Skunk I'm performing some final testings on my prototype right now, once everything is done I will submit a batch order to the fab. I don't know exactly when that will be, but my guess is sometime this week.
@Battosaii The controller case can be trimmed down, I will try to reduce its size today. The actual circuit board is only about 87mm.
```

---
## \#154 Posted by: FredXanadu Posted at: 2018-09-04T14:20:34.602Z Reads: 207

```
F... i did the same, i ordered the proton , what the trick to set tup the proton on the Evo ?
```

---
## \#155 Posted by: Battosaii Posted at: 2018-09-04T14:38:39.349Z Reads: 210

```
https://www.electric-skateboard.builders/t/proton-digital-instrument-and-control-panel-touch-screen/58664/153?u=battosaii

He says it right there we should be okay.
```

---
## \#156 Posted by: Wajdi Posted at: 2018-09-04T15:14:54.065Z Reads: 214

```
@FredXanadu I cropped the sides of the enclosure, it is now around 92-93mm.
![52%20AM|611x499](upload://7a8p5yzcwrPRtfv8R766uWos1Vn.png)
```

---
## \#157 Posted by: uigiroux Posted at: 2018-09-04T15:15:29.567Z Reads: 206

```
Anyone know if this will this fit on Hummies deck?
```

---
## \#158 Posted by: Wajdi Posted at: 2018-09-04T15:16:04.805Z Reads: 204

```
@uigiroux What are the dimensions of that deck?
```

---
## \#159 Posted by: uigiroux Posted at: 2018-09-04T15:16:32.927Z Reads: 204

```
Would the screen be centered though if it was modified this way?

Not sure off hand...  Can't really check atm, was hoping someone knew..
```

---
## \#160 Posted by: Wajdi Posted at: 2018-09-04T15:26:15.736Z Reads: 207

```
Yes I will try to center the screen.
```

---
## \#161 Posted by: FredXanadu Posted at: 2018-09-04T15:49:01.873Z Reads: 198

```
Still missing 3mms... :(
```

---
## \#162 Posted by: Wajdi Posted at: 2018-09-04T15:49:41.519Z Reads: 199

```
Still not done yet :grinning: I will get there.
```

---
## \#163 Posted by: Toughook Posted at: 2018-09-04T16:01:53.036Z Reads: 207

```
The device looks cool, but because I am (and I suspect many other leisure-time-engineers on here are too) quite OCD in disposition.... a screen off center just looks wrong.

I understand, having read your earlier posts, why it turned out this way, but whilst I'd have a device this useful on my board, it would bug the hell out of me if asymmetrical.

Just my two cents
```

---
## \#164 Posted by: Wajdi Posted at: 2018-09-04T16:05:14.863Z Reads: 219

```
@Toughook Rest assured it will be centered and symmetrical. Those rendering are using an older version of the display. I will update the renderings today.
New one 
![HTB1KTByB2iSBuNkSnhJq6zDcpXaN|500x500](upload://nx7asRWg6tpDhh3xOFShxTBNj02.jpg)
```

---
## \#165 Posted by: Socalscare Posted at: 2018-09-04T16:54:10.052Z Reads: 210

```
Something else to add to my first build!!! Man this forum is getting expensive !!!!!  😊
```

---
## \#166 Posted by: Toughook Posted at: 2018-09-04T17:12:58.467Z Reads: 209

```
Cool ! Glad you're changing it, you'll sell loads more I reckon, and I might well be one of them.... 😀
```

---
## \#167 Posted by: Pedrodemio Posted at: 2018-09-06T21:08:29.467Z Reads: 203

```
As soon I receive my deck I will make a detailed CAD model of it, if want I can share it so you can make a version that fits perfectly
```

---
## \#168 Posted by: Battosaii Posted at: 2018-09-06T21:20:29.778Z Reads: 200

```
Hmm 93mm is about 1.5mm over hang each side thats not too bad but flush would be nice.
```

---
## \#169 Posted by: Wajdi Posted at: 2018-09-06T23:10:30.913Z Reads: 201

```
@Pedrodemio Cool thanks!
@Battosaii I will try to make that happen. I recently upgraded the display from 2.8" to 3.2", that made the screen centered and improved visibility due slight increase in size.
```

---
## \#170 Posted by: Goonman Posted at: 2018-09-09T08:16:20.808Z Reads: 200

```
You are a freakin genius. I wondering how I was going to incorporate a volt meter and ammeter on my board. Thinking there was no hope. Now I have seen this awesome bit of gear I am wondering if it will calculate and display watts and Watt hours. So if you know that you have 200wh of battery from full it will give you a more accurate picture of usage. Have you seen cycle analyst?
```

---
## \#171 Posted by: Goonman Posted at: 2018-09-09T08:16:50.303Z Reads: 198

```
PS 
Take my money!
```

---
## \#172 Posted by: Wajdi Posted at: 2018-09-10T15:26:09.711Z Reads: 202

```
Thank you @Goonman. Yes Absolutely, from the main screen you will have the possibility to cycle through what data you want to be displayed, including Wh.
```

---
## \#173 Posted by: Dayum Posted at: 2018-09-12T00:01:45.398Z Reads: 203

```
I saw this listing on this website.  I'm trying to figureout how does this device hook up to lets say a Lacroix board or a Evolve Bamboo GTX board's electronics.

https://eboardshop.net/product/proton-control-panel/
```

---
## \#174 Posted by: Battosaii Posted at: 2018-09-12T00:55:57.865Z Reads: 207

```
This product is designed to work with Vesc based esc's so it will not work with an Evolve board. The LaCroix board does use Vesc based esc's but the truck mounting points are different since it uses mountain board trucks. You attach the device with truck hardware and you plug in the uart cable to the master Vesc.
```

---
## \#175 Posted by: Kug3lis Posted at: 2018-09-12T01:15:39.159Z Reads: 200

```
[quote="Battosaii, post:174, topic:58664"]
mounting points are different since it uses mountain board trucks
[/quote]

iirc MBS has longboard style mounting hole pattern..
```

---
## \#176 Posted by: Dayum Posted at: 2018-09-12T01:26:44.970Z Reads: 191

```
I'm new to the esk8 modding community.  So what you saying is I will have to connect a wire from the Proton Control unit to a connector inside the battery enclosure that's housing the VESC component that has a UART connector?

As for the truck hardware I'm not too worried about it.  I'll just use double sided velcro mounting.
```

---
## \#177 Posted by: Battosaii Posted at: 2018-09-12T01:33:59.972Z Reads: 184

```
yes thats exactly it. i plan on making a small hole in the deck just enough to fit the uart wires so i can run the wire under the deck into the enclosure. 

and as @Kug3lis pointed out this will work with a lacroix because they use MBS hardware.
```

---
## \#178 Posted by: Dayum Posted at: 2018-09-12T01:42:05.718Z Reads: 179

```
Have you pre-order this unit yet?
```

---
## \#179 Posted by: Battosaii Posted at: 2018-09-12T01:43:28.426Z Reads: 178

```
I did preorder it, i like the concept.
```

---
## \#180 Posted by: Dayum Posted at: 2018-09-12T01:47:37.696Z Reads: 179

```
How do you power it?  It is drawing power off the UART connection to the VESC electronics?  Or do I have to somehow splice into the battery pack to get power for the unit?
```

---
## \#181 Posted by: FourteeOZ Posted at: 2018-09-12T01:56:25.666Z Reads: 187

```
I will definitely Pre-Order this if there is any news that it will fit Hummies deck.
```

---
## \#182 Posted by: Wajdi Posted at: 2018-09-12T02:09:11.148Z Reads: 188

```
@Dayum It is self powered from the VESC, no need for external power. Unless you want to drive LEDs and use the USB chargers.
@FourteeOZ Do you have the dimensions of that deck?
```

---
## \#183 Posted by: Dayum Posted at: 2018-09-12T02:35:27.939Z Reads: 185

```
@Wajdi  Sorry for the noob question but when you say power the LEDs are you talking about the backlight for the LCD screen?  I understand the USB chargers part.  Where you recommend tapping 5v+ from?
```

---
## \#184 Posted by: Wajdi Posted at: 2018-09-12T02:48:02.523Z Reads: 183

```
@Dayum, No the backlight and everything related to the control panel is self powered from the UART cable, what I meant by LEDs was adding LED strips for lightning effects.
```

---
## \#185 Posted by: Dayum Posted at: 2018-09-12T02:53:42.117Z Reads: 188

```
@Wajdi Gotcha, so literally LED accented lighting for the board.  Thanks for the clarification.  I'll be pre-ordering end of this weekend.
```

---
## \#186 Posted by: Wajdi Posted at: 2018-09-12T02:55:44.198Z Reads: 190

```
You are welcome, let me know if you have any more questions :slightly_smiling_face:
```

---
## \#187 Posted by: FourteeOZ Posted at: 2018-09-12T03:10:40.312Z Reads: 191

```
I do not have time to go through the thread as I am at work, but somewhere around post 1410 https://www.electric-skateboard.builders/t/new-wood-carbon-decks-group-buy-round-3-110-shipped-us/43245/1410 are the pics of the round 3 double cut outs. Further down hummie says it is 120mm across the truck mounts.
```

---
## \#188 Posted by: Wajdi Posted at: 2018-09-12T03:18:38.717Z Reads: 192

```
If its 120mm across the truck mounts then it should absolutely fit.
```

---
## \#189 Posted by: mackann Posted at: 2018-09-19T18:30:08.615Z Reads: 189

```
Do you have any news about shipping for the pre-orders?
```

---
## \#190 Posted by: Wajdi Posted at: 2018-09-23T00:37:44.388Z Reads: 201

```
Received a prototype board today, going to test it and I will be posting updates :+1:

![IMG_1196|375x500](upload://9o8m2Llb3RoaTGD954z04O965A5.jpeg)
```

---
## \#191 Posted by: Battosaii Posted at: 2018-09-24T14:54:32.344Z Reads: 198

```
Looks really nice can't wait to see it up an running.
```

---
## \#192 Posted by: FredXanadu Posted at: 2018-09-25T14:10:31.979Z Reads: 196

```
Hello, What about the final size ? Do you think it's gonna finally fit on an Evo deck ?.
```

---
## \#193 Posted by: Battosaii Posted at: 2018-10-03T03:59:24.870Z Reads: 189

```
Any updates on the final dimensions?
```

---
## \#194 Posted by: pixelsilva Posted at: 2018-10-03T11:04:31.456Z Reads: 194

```
![New%20Project(1)(1)(1)|690x487](upload://1OznNvtyjAVUDZykZJEZ7wq5Mlf.jpeg) 

@Wajdi, do you think is possible to trim the control panel even more, like this? In my case I have no use for the curvy case profile. My deck comes with narrow drop-thru front and rear ends so reducing excesive panel real state is a must.
```

---
## \#195 Posted by: uigiroux Posted at: 2018-10-03T13:02:11.782Z Reads: 179

```
What would modifying the case like that actual do though?  I can understand wanting to do that if it was something in your enclosure since that space is extremely limited, but if you're just mounting this as intended, then changing the screw holes to be less curvy as you said, it looks like all that would change is purely aesthetic.   :confused:
```

---
## \#196 Posted by: topcloud Posted at: 2018-10-03T13:17:02.092Z Reads: 176

```
many of us plan to print our own enclosures for the Proton Cockpit.
```

---
## \#197 Posted by: Battosaii Posted at: 2018-10-03T16:49:21.357Z Reads: 177

```
Nice yet another reason yo buy a printer. 

I just want something that will look nice on an Evo
```

---
## \#198 Posted by: Wajdi Posted at: 2018-10-03T20:41:39.375Z Reads: 193

```
Its at 94.4mm x 60mm right now. Thats with the bigger screen and centered design.

I will also share the enclosure stl files, so that anyone can work, print and modify it as they wish.

![01%20PM|599x500](upload://eoPVmfHvDvTitUihAclrPt6O62N.jpeg)
```

---
## \#199 Posted by: Jc06505n Posted at: 2018-10-03T20:42:53.935Z Reads: 180

```
Nice, what's the status on progress?
```

---
## \#200 Posted by: pixelsilva Posted at: 2018-10-03T20:44:41.771Z Reads: 187

```
No, I just eliminated some excess case curvy profile that is not neccesary to me. Drop-thru front ends are already smaller on most decks. That curvy profile is uneccesary if the only thing you need is the four holes to attach the thing. So, the smallest case footprint should be the size of the whole screen/circuit board. That should be the smallest size for the control panel. Excessive plastic case around interfere (overlaps) most deck's front end profiles.
```

---
## \#201 Posted by: uigiroux Posted at: 2018-10-03T21:48:28.972Z Reads: 185

```
Right on, that makes sense.  I imagine the best way for you to get the profile you want would be to print off a design of your own...
```

---
## \#202 Posted by: pixelsilva Posted at: 2018-10-04T01:59:22.462Z Reads: 183

```
Yeah, thats seems to be the case, @Wajdi is providing the STL files so anyone could go and print their own personalized enclosure.
```

---
## \#203 Posted by: Battosaii Posted at: 2018-10-09T00:10:57.705Z Reads: 188

```
if the PCB is 87mm would it be possible to make a 90mm wide enclosure for Evo guys and other similar style decks?
```

---
## \#204 Posted by: Wajdi Posted at: 2018-10-14T22:06:42.125Z Reads: 196

```
Been working on the UI and improving touch controls, will fit everything inside the casing soon.

![IMG_1372|666x500](upload://eMFNXZwIgMkzQC8hZ6RX4fu8Yu4.jpeg) ![IMG_1373|666x500](upload://o2J5u7nUesZOU5totoCMfyU6npd.jpeg) ![IMG_1374|666x500](upload://iFL3HhL0TnnimTGQtMZ8VKQmhZU.jpeg)
```

---
## \#205 Posted by: Jc06505n Posted at: 2018-10-14T22:09:21.220Z Reads: 189

```
Nice, Any eta of a Timeline?
```

---
## \#206 Posted by: Wajdi Posted at: 2018-10-14T22:21:27.593Z Reads: 191

```
@Jc06505n I made some changes to the prototype PCB I received, and will be finishing v0.1 of the software by Wednesday. I will have the first batch manufacturing start in about 1 or 2 days.
```

---
## \#207 Posted by: uigiroux Posted at: 2018-10-15T00:18:15.224Z Reads: 185

```
Wow, you're killin it with these products you're designing.  I can't wait to get one of these! Won't ever have to hook my board up to a computer.  Instantly being able to change settings so easily...  Love it! :heart_eyes:
```

---
## \#208 Posted by: Battosaii Posted at: 2018-10-22T12:43:50.794Z Reads: 188

```
Any updates? Im excited about having a instrument cluster on my board.
```

---
## \#209 Posted by: Wajdi Posted at: 2018-10-23T05:45:49.905Z Reads: 196

```
A quick update, a couple images of the 3.2 inch touch display inside the enclosure. Silver filament is what I have left for the moment, I will be printing black on Wednesday :slightly_smiling_face:

I will be posting an in-depth showcase tomorrow showing it in action! 
* Touch commands are all set
* Real time graphs and data are implemented
* Support for latest Vesc FW 3.40 is done.
* Dual UART port for dual setup or to forward Photon receiver/Bluetooth modules

![IMG_1403|375x500](upload://m3VB5XjQ8akEjjg5XD5Y9w8DzYg.jpeg) ![IMG_1404|375x500](upload://hCMG1rVNbff8LyJmq4jZpmCG4Ir.jpeg) ![IMG_1406|375x500](upload://dBdmqo67MAdi6VrMvUCEtfbHYAz.jpeg)
```

---
## \#210 Posted by: Battosaii Posted at: 2018-10-23T05:51:12.781Z Reads: 183

```
That looks awesome.

Edit: I wonder if the display mounted flat would cause glare.
```

---
## \#211 Posted by: Wajdi Posted at: 2018-10-23T06:02:37.260Z Reads: 191

```
I will share the display enclosure once finished, it can be adjusted easily to be tilted or modified to any shape/design.
```

---
## \#212 Posted by: Wajdi Posted at: 2018-10-27T17:10:43.627Z Reads: 195

```
I spent a significant time yesterday finishing up the software design and calibrating most of the touch screen commands, I also printed the case to test the fitting, and it was near perfect. 

![IMG_1444|375x500](upload://lofMay2iKCswNOATmbYXOLVvyK9.jpeg) 
![IMG_1446|375x500](upload://aoz02WRCKDE2iMIQxePZFEJ54mp.jpeg) 
![IMG_1450|658x499](upload://8ftnCjBWeKxyr5BOCvgqQmlv52J.jpeg) 
![IMG_1451|375x500](upload://vEGCnmuk2I3SGHGt0VgDU9j0Mmm.jpeg) 
USB chargers are not yet fitted in this picture.
![IMG_1455|461x500](upload://lPd6wGq41iDsHRcfUW3khMJ61YX.jpeg) 
![IMG_1456|500x500](upload://w39ID1MGL92Emv6pIJSci6aw1Su.jpeg) 
![PNG|500x500](upload://jfjeNZC8aTsK7FZYS3UDi1BaMlr.jpeg)
```

---
## \#213 Posted by: Battosaii Posted at: 2018-10-27T17:22:02.906Z Reads: 187

```
Daaaaaaamn thats so nice looks increabible. Do you expect shipping sometime next month?
```

---
## \#214 Posted by: Wajdi Posted at: 2018-10-27T17:39:56.375Z Reads: 180

```
Yes it should be well ready by next month, going to finalize everything this weekend and start production afterwards. I'm also making a small demo video.
```

---
## \#215 Posted by: Battosaii Posted at: 2018-11-12T20:24:08.249Z Reads: 175

```
Any updates my board is now done and this is the last piece lol.
```

---
## \#216 Posted by: FredXanadu Posted at: 2018-11-12T20:31:53.622Z Reads: 175

```
hello @Wajdi, for the V2, why not implant a charging port on the proton ?
Maybe instead of 2 Usb port, we can have 1 usb and 1 charging port.
What do you think ?
```

---
## \#217 Posted by: Battosaii Posted at: 2018-11-12T20:36:09.607Z Reads: 184

```
Adding a charge port would be easy but I wouldn't want a charge port on top of my deck.
```

---
## \#218 Posted by: FredXanadu Posted at: 2018-11-12T20:45:45.437Z Reads: 181

```
the new trend is, no hole on the enclosure :slight_smile:
```

---
## \#219 Posted by: Battosaii Posted at: 2018-11-12T20:57:30.817Z Reads: 184

```
I have button and charge port on the enclosure nothing else I think it's pretty clean
```

---
## \#220 Posted by: mackann Posted at: 2018-11-19T20:39:22.532Z Reads: 184

```
Any update?
```

---
## \#221 Posted by: Battosaii Posted at: 2018-11-22T03:11:28.025Z Reads: 191

```
Any updates on the production? @Wajdi
```

---
## \#222 Posted by: Wajdi Posted at: 2018-11-22T03:48:46.082Z Reads: 194

```
I already started production, going to start delivering in about 3 weeks. 
Demo video is almost done, waiting for sunlight to finish recording.
```

---
## \#223 Posted by: Wajdi Posted at: 2018-11-23T02:37:41.404Z Reads: 200

```
Update: quick demo video showcasing the Proton control panel as promised, enjoy :slight_smile:

https://youtu.be/Ag4mpMdqHmk
```

---
## \#224 Posted by: harrypzee Posted at: 2018-11-23T02:45:44.749Z Reads: 196

```
Woah, I thought of this exact thing a few weeks ago! That’s what I love about this hobby, I have an idea and it turns out someone is already working on it. I definitely am interested in preordering.
```

---
## \#225 Posted by: kylem21 Posted at: 2018-11-23T03:40:36.551Z Reads: 192

```
Looks good! How far out you think you are of implementing the endless ride?
```

---
## \#226 Posted by: Wajdi Posted at: 2018-11-23T17:31:06.785Z Reads: 190

```
I had endless ride implemented a while back. I will post a demo video of it sometime this week when I fix my board battery. Btw Black friday sale is live with 20% off :grinning:
```

---
## \#227 Posted by: Battosaii Posted at: 2018-11-24T18:42:01.075Z Reads: 184

```
I'm so excited wooo
```

---
## \#228 Posted by: Badger1666 Posted at: 2018-11-25T12:47:54.171Z Reads: 190

```
I have ordered one of these to use on my scooter build , the question is . Will the uart still work @ 1.2m ,if i use a shielded cable
```

---
## \#229 Posted by: Battosaii Posted at: 2018-11-29T16:56:59.990Z Reads: 189

```
Shouldn't be a problem. Especially if they are shielded.
```

---
## \#230 Posted by: pixelsilva Posted at: 2018-11-29T17:48:19.950Z Reads: 186

```
Wow!!  ...double Wow!! :open_mouth: Amazing development @Wajdi
```

---
## \#231 Posted by: Battosaii Posted at: 2018-12-09T15:16:19.947Z Reads: 186

```
any updates?

do you have an instagram?

im going to assume these will now be for next year?
```

---
## \#232 Posted by: Wajdi Posted at: 2018-12-15T01:19:12.064Z Reads: 181

```
Im receiving the PCBs next week, fab just contacted me with some questions before assembly, they said I should receive them by next week, I will start shipping pre-orders right away. :+1:
```

---
## \#233 Posted by: banjaxxed Posted at: 2018-12-19T09:26:30.091Z Reads: 178

```
Hey @Wajdi did you get the pcbs in yet? Presumably pre-populated and just need a f/w upload and quick test? Looking forward to them
```

---
## \#234 Posted by: banjaxxed Posted at: 2018-12-24T13:18:49.675Z Reads: 179

```
Happy Christmas @Wajdi let's get things rolling in 2019
![tumbleweed|509x339](upload://p3HJsMZ6mBGkG0xer0owtBH6262.jpeg)
```

---
## \#235 Posted by: ElskerShadow Posted at: 2018-12-24T22:50:27.628Z Reads: 174

```
It was the same story with the photon, was to be expected ;)
```

---
## \#236 Posted by: kylem21 Posted at: 2018-12-24T23:29:01.671Z Reads: 174

```
I’m looking to sell my preorder  if anyone’s interested. Asking for $105. Shipping within US is already paid for, I’ll just ask to switch shipping address.
```

---
## \#237 Posted by: Battosaii Posted at: 2018-12-26T19:41:06.416Z Reads: 173

```
You could ask for a refund, I ordered in September and the website said expected to start shipping within 25 days. Well now we're almost on January and still nothing. 

I will wait for it cause I want it and I don't mind waiting but I understand.
```

---
## \#238 Posted by: kylem21 Posted at: 2018-12-26T21:05:13.826Z Reads: 171

```
Yeah I’ve kind of just lost interest now that my builds been complete for a couple months without the panel, I’ll probably try to get the refund but I figured I’d give someone a chance at the early preorder price
```

---
## \#239 Posted by: Wajdi Posted at: 2018-12-28T03:31:28.196Z Reads: 179

```
![IMG_1670|375x500](upload://ibDA8AbULpbxXWXWP5eJ0CSWse3.jpeg) 
![IMG_1681|375x500](upload://9A1SxJF9gDecbpNhAVIuFJapcF8.jpeg) 
![IMG_1684|375x500](upload://l24MWiREGZkCU99p2j76TxjkiNO.jpeg)

Packages arrived today, fab took extra long time. I have everything ready right now, and I'm expecting the custom long UART cables to be here shortly as well.
I will be packing those up and sending out orders asap. :+1:
```

---
## \#240 Posted by: Battosaii Posted at: 2018-12-28T03:41:07.239Z Reads: 168

```
Sweet can't wait to see it
```

---
## \#241 Posted by: Frenchy Posted at: 2018-12-28T03:57:41.615Z Reads: 167

```
I remember reading early you we're trying to get it to fit your Evo. did he manage to get it to fit nicely
```

---
## \#242 Posted by: Jc06505n Posted at: 2018-12-28T04:09:08.300Z Reads: 169

```
Awesome @moon any interest in creating cases for these like for DaveGa? These have less buttons (I think none) and seem to be of a similar screen
```

---
## \#243 Posted by: Battosaii Posted at: 2018-12-28T04:09:16.298Z Reads: 169

```
Last I checked the enclosure was about 1mm wider than the deck so it will have .5mm overhang each side. Shouldn't be too bad maybe a little sanding can fix that.
```

---
## \#244 Posted by: Battosaii Posted at: 2018-12-28T04:10:37.780Z Reads: 160

```
It's a bigger screen and it's touch screen. It does come with an enclosure but I'm sure there will be design changes or diyers that make their own.
```

---
## \#245 Posted by: Jc06505n Posted at: 2018-12-28T04:11:58.801Z Reads: 162

```
Yeah. , I just wish there was bug interest in custom cases like there is for Dave , but I’m hype to put this on the orca
```

---
## \#246 Posted by: moon Posted at: 2018-12-28T04:12:39.756Z Reads: 166

```
Just that less people will end up having this so making a special case might not be worth it
```

---
## \#247 Posted by: banjaxxed Posted at: 2018-12-28T11:13:18.416Z Reads: 159

```
I’ll be looking at the design for sure, @Wajdi can you release a cad to make it easier to mod the case, it may make it a more interesting proposition if there are some good case variations ie just keep the electronics proprietary 

For instance I would like to add a 5.5 charger port for a 13s HAYA build, fusion file if you can

thanks
```

---
## \#248 Posted by: Battosaii Posted at: 2019-01-08T19:50:36.272Z Reads: 160

```
Hello any updates on this yet? It's 2019 I want a screen on my board haha.
```

---
## \#249 Posted by: banjaxxed Posted at: 2019-01-08T19:59:29.774Z Reads: 167

```
Arizona comms sadly![tumbleweed|509x339](upload://p3HJsMZ6mBGkG0xer0owtBH6262.jpeg)
```

---
## \#250 Posted by: mackann Posted at: 2019-01-09T06:52:08.848Z Reads: 162

```
Just got my display shipped!
```

---
## \#251 Posted by: mackann Posted at: 2019-01-09T08:24:15.304Z Reads: 164

```
Will this display work with Unity? I gues it needs a firmware update for it? @Wajdi
```

---
## \#252 Posted by: Battosaii Posted at: 2019-01-09T20:24:20.877Z Reads: 162

```
When did you order it? I ordered near the end of August.

And it should work with a unity. It's not that much different than a focbox. I'll be getting a Unity Friday and I'll try it as soon as my display ships.
```

---
## \#253 Posted by: Jc06505n Posted at: 2019-01-09T20:29:15.503Z Reads: 162

```
the UART protocols are slightly different. If @Wajdi doesn't account for it , telemetry wont work.
```

---
## \#254 Posted by: mackann Posted at: 2019-01-09T20:37:47.056Z Reads: 159

```
August 29, like @jc06505n says it's need a firmware fix to work
```

---
## \#255 Posted by: Wajdi Posted at: 2019-01-09T20:51:49.801Z Reads: 172

```
Hey guys,

I created shipping labels for all the Proton pre-orders, if you did not get your tracking number, let me know and I will send it to you.
About Unity compatibility, I'm looking into the source code right now, and I will make it compatible either initially or through a firmware update once shipped.

I will also post the enclosure files so anyone can modify to their liking 

![IMG_1755|375x500](upload://6UfGUdDt1imMTMoDEWpPJvDJ95s.jpeg) ![IMG_1756|375x500](upload://2412ptvSeREpkckhYvsdu2is3zs.jpeg) ![IMG_1757|375x500](upload://cOBtanHcUsY1VS64Oq35r0MFzDz.jpeg)
```

---
## \#256 Posted by: Battosaii Posted at: 2019-01-09T20:54:20.875Z Reads: 164

```
@Wajdi I did not get my tracking number yet
```

---
## \#257 Posted by: Wajdi Posted at: 2019-01-09T20:58:03.117Z Reads: 162

```
Pm your order number and I will send it to you :+1:
```

---
## \#258 Posted by: Jc06505n Posted at: 2019-01-09T21:03:25.798Z Reads: 163

```
Got it , make sure you guys check spam
```

---
## \#259 Posted by: Mich21050 Posted at: 2019-01-09T21:09:24.468Z Reads: 165

```
Ok so kind of an odd question but I think I somewhere read that the proton has an uart splitter... If so how did you realize that? I'm working on one right now and was just wondering :slight_smile:
```

---
## \#260 Posted by: Battosaii Posted at: 2019-01-09T21:17:36.636Z Reads: 163

```
Thanks I actually checked and it's there in the spam I'm so excited!!
```

---
## \#261 Posted by: Wajdi Posted at: 2019-01-09T21:35:30.210Z Reads: 164

```
@Mich21050 Pretty easy, just make sure that your microcontroller supports two serial ports, then you just forward commands from one port to the other in a FIFO order.
```

---
## \#262 Posted by: Wajdi Posted at: 2019-01-09T21:39:13.012Z Reads: 171

```
Picture with USB charging ports in:
![IMG_1758|375x500](upload://ncFszsgNuzVQMwDzi05xQ6pZdwx.jpeg)
```

---
## \#263 Posted by: louwii Posted at: 2019-01-09T21:52:40.964Z Reads: 166

```
Interesting project. What's funny is that another community member is working on quite the exact same thing, but has open-sourced it: https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509

Would be cool to have a comparison between them. DAVEga is more for the DIYers I imagine, as it doesn't have a touch screen, everything needs to be programmed first, then the unit needs software flashing.

It's a cool project though, it's nice to see "new" products coming out.
```

---
## \#264 Posted by: banjaxxed Posted at: 2019-01-09T21:58:46.199Z Reads: 164

```
Got my number thanks for releasing everything dude
```

---
## \#265 Posted by: Wajdi Posted at: 2019-01-09T23:00:13.145Z Reads: 163

```
Tested with the custom made 1 meter long uart cable (~ 39.37 ") with no problems! I was worried about voltage attenuation and packets loss but it worked perfectly!
```

---
## \#266 Posted by: Mich21050 Posted at: 2019-01-10T06:40:31.774Z Reads: 163

```
I know I'm a little late for the party but if I order right now when would I get it? :slight_smile:
```

---
## \#267 Posted by: Wajdi Posted at: 2019-01-10T15:53:38.534Z Reads: 161

```
Yes, I have it available in stock.
```

---
## \#268 Posted by: Wajdi Posted at: 2019-01-16T05:58:45.071Z Reads: 167

```
I released the enclosure file on thingiverse https://www.thingiverse.com/thing:3359442
Feel free to modify it to your liking. If you made improvements please do share with the rest of us :slightly_smiling_face: , we still need to figure out what would be the best base plate design, right now I only have the top cover done.

I will include the 3D printed top cover with current pre-orders, but it will still need a base plate.

![IMG_1785|666x500](upload://fAumqea5K5Xf6ZqzKq5XMpRzKUm.jpeg) ![IMG_1788|375x500](upload://6eIUF41VgLNjavABAlGwHOMWujr.jpeg) ![IMG_1795|375x500](upload://dgAA5vXjEHD7F5qY9WG3coL3mzv.jpeg) ![IMG_1796|375x500](upload://38Yr24kc5eiTPtwlqqmNqTSNxMD.jpeg) 

I have them ready to be dropped off.
```

---
## \#269 Posted by: mackann Posted at: 2019-01-16T07:16:48.070Z Reads: 158

```
So you will ship preorders without a baseplate?
```

---
## \#270 Posted by: banjaxxed Posted at: 2019-01-16T10:59:26.594Z Reads: 157

```
Great a mod so as to not cut the deck for non drop decks will be a good one thanks
```

---
## \#271 Posted by: Wajdi Posted at: 2019-01-16T14:27:41.656Z Reads: 162

```
It will have a basic bottom rectangular cover.
```

---
## \#272 Posted by: Wajdi Posted at: 2019-01-19T21:52:08.955Z Reads: 169

```
Here is what’s included in the package kit
![image|666x500](upload://mJ8Zx3BUiOtFuZouPLE7cc1KhGJ.jpeg) 

Endless ride is still experimental and is not activated yet in this first release. If anyone wants to be a tester let me know and I will send you a firmware update that enables it.
```

---
## \#273 Posted by: Mich21050 Posted at: 2019-01-19T22:08:27.230Z Reads: 163

```
Any plans on releasing the source code? :smile:
```

---
## \#274 Posted by: banjaxxed Posted at: 2019-01-19T22:25:44.396Z Reads: 157

```
Haha you are having a laugh
```

---
## \#275 Posted by: Mich21050 Posted at: 2019-01-19T22:26:29.703Z Reads: 156

```
Yeahh still worth a shot :joy:
```

---
## \#276 Posted by: Wajdi Posted at: 2019-01-19T22:31:36.692Z Reads: 159

```
Not for now, but I have that in my to consider list :slightly_smiling_face:
```

---
## \#277 Posted by: Battosaii Posted at: 2019-01-22T01:43:38.051Z Reads: 159

```
Tracking number says mine comes in tomorrow, id love to beta test the endless ride mode. Thats the one and only feature i liked about mellow.

btw is that a nintendo 3ds stylus?
```

---
## \#278 Posted by: Wajdi Posted at: 2019-01-23T00:22:22.480Z Reads: 152

```
Looks similar but I'm not sure if its the same one used in the Nintendo :slightly_smiling_face:
```

---
## \#279 Posted by: Battosaii Posted at: 2019-01-23T00:28:20.611Z Reads: 155

```
I was going to use this on my Evo deck but the uart plug goes straight down so if you don't have a hole under where it goes then you need to drill it out. 

I'm going to try it on my drop through arbor evolve set up.
```

---
## \#280 Posted by: Battosaii Posted at: 2019-01-23T00:47:52.995Z Reads: 162

```
So I got home and saw my kit. Eagerly wanting to install it I ran into my first problem.

There's not enough space on the enclosure for the screws. The thread of the screw skimms across the side of the enclosure barely fitting and that leave no space for the head of the screw to go down. 

![20190122_194402|666x500](upload://thc3e3b5QiMEK5ByfUpmNR0bak.jpeg) 

![20190122_194336|666x500](upload://nPBFbU0mQUs5uqZGRfyRHvgB9vU.jpeg) 

I can try to force the screws down but I'm afraid of snapping the enclosure. 

What should I do @Wajdi
```

---
## \#281 Posted by: Jc06505n Posted at: 2019-01-23T01:00:58.909Z Reads: 157

```
I wonder if modifying the davega files would work, it's a bigger screen but just scaling it to that and closing off the holes should be enough right? or maybe we need to throw money at @moon
```

---
## \#282 Posted by: moon Posted at: 2019-01-23T01:02:24.584Z Reads: 155

```
I can try something but I'm completely out of the loop
```

---
## \#283 Posted by: Battosaii Posted at: 2019-01-23T01:03:23.203Z Reads: 151

```
The pcb shape is also very different than the davega it's not just the screen. 

I'm having an issue with enclosure I may just velco the thing on lol
```

---
## \#284 Posted by: Jc06505n Posted at: 2019-01-23T01:06:05.669Z Reads: 151

```
ooooh I assumed that it was just a bigger screen, that does complicate things
```

---
## \#285 Posted by: Battosaii Posted at: 2019-01-23T01:07:21.703Z Reads: 153

```
I'm seriously going to Velcro this thing down lol
```

---
## \#286 Posted by: Wajdi Posted at: 2019-01-23T01:09:21.729Z Reads: 151

```
Whats the size of those screws? I will try to modify the enclosure to accommodate for that.
```

---
## \#287 Posted by: Battosaii Posted at: 2019-01-23T01:13:24.611Z Reads: 151

```
Normal 10/32 screws. I use flat headed screws cause counter sunk can cause deck splitting.
```

---
## \#288 Posted by: Wajdi Posted at: 2019-01-23T01:34:01.489Z Reads: 152

```
Ok, I will see how to make that fit. In the mean time, you can probably try to put your screws in reverse, head down, and nut up, with some washers.
```

---
## \#289 Posted by: Battosaii Posted at: 2019-01-23T03:59:20.058Z Reads: 152

```
cant seem to get info to show on display is there anything special i need to do?
```

---
## \#290 Posted by: Jc06505n Posted at: 2019-01-23T03:59:54.527Z Reads: 152

```
Did you change the baudrate?
```

---
## \#291 Posted by: Battosaii Posted at: 2019-01-23T04:00:41.838Z Reads: 151

```
i put it at 115200 is that correct?
```

---
## \#292 Posted by: mmaner Posted at: 2019-01-23T04:05:29.903Z Reads: 151

```
If you want to send me the dimensions I can make my DaVeGa design fit.
```

---
## \#293 Posted by: Wajdi Posted at: 2019-01-23T04:14:44.778Z Reads: 154

```
Yes that's correct, did you change app control to UART? 
Also there are two UART ports, you have to use the master port, which is the one on the left when screen is facing up.
```

---
## \#294 Posted by: Jc06505n Posted at: 2019-01-23T04:27:42.034Z Reads: 149

```
If your using the unity it might not work since the code for telemetry is different.
```

---
## \#295 Posted by: Battosaii Posted at: 2019-01-23T04:29:45.688Z Reads: 148

```
I'm using it on Focbox I know they don't work with unity yet. 

But yeah have it set to ppm and uart use and baud to 115200 and I get no info on the screen.
```

---
## \#296 Posted by: Wajdi Posted at: 2019-01-23T04:35:18.193Z Reads: 148

```
Did you try the other UART port? which port are you using?
```

---
## \#297 Posted by: Battosaii Posted at: 2019-01-23T04:47:09.946Z Reads: 146

```
I've tried both and have tried 4 different Focboxes.
```

---
## \#298 Posted by: Wajdi Posted at: 2019-01-23T04:47:56.719Z Reads: 151

```
What firmware version is your Focbox running?
```

---
## \#299 Posted by: Wajdi Posted at: 2019-01-23T04:56:28.040Z Reads: 164

```
[quote="Battosaii, post:297, topic:58664, full:true"]
I’ve tried both and have tried 4 different Focboxes.
[/quote]


The port to use has to be the master, the one on the left when facing up, after setting the app  to UART, make sure you hit the apply button.
Once all done, you need to power cycle while the Proton is connected. On next boot up it should start communicating.

![IMG_1795-2|375x500](upload://heHXK0fdSjQ2Fe3Rn1gP9ekHgAA.jpeg)


**One more thing**: When turned on, press the settings menu button, then go back to main screen, it should force it to work, let me know if this solves it.
```

---
## \#300 Posted by: Battosaii Posted at: 2019-01-23T12:35:48.323Z Reads: 155

```
I've done that a few times and I have the uart plugged into the right port. Once I get home from work I'll try again.

I was going to try it out on the night ride tonight but the deck won't be finished so even if it works I won't be able to use it till.next weeks ride.
```

---
## \#301 Posted by: Battosaii Posted at: 2019-01-23T12:38:47.629Z Reads: 152

```
They are running ackmaniac firmware and tool, could that be the issue?
```

---
## \#302 Posted by: Wajdi Posted at: 2019-01-23T16:21:04.575Z Reads: 154

```
It could be, I only tested on official firmware. Btw they should also be compatible with Unity, give it a go and let me know if its works, I haven't tested Unity because I don't have one, but it should work.
```

---
## \#303 Posted by: Battosaii Posted at: 2019-01-23T16:44:28.723Z Reads: 148

```
Ok I'll try on unity if it works then it's the ackmaniac on the regular Focboxes that's not working with the screen.
```

---
## \#304 Posted by: Jc06505n Posted at: 2019-01-23T19:52:16.141Z Reads: 150

```
[quote="Wajdi, post:23, topic:58664"]
I thought about this when I was designing it, thats why I added a secondary UART port on the panel. That way you can connect your Bluethooth module to it, or whatever needs access to UART.
[/quote]


Just got mine, is this still true? Can i plug in the metr mod into the second uart port ?
```

---
## \#305 Posted by: Wajdi Posted at: 2019-01-23T21:07:10.476Z Reads: 145

```
Yes, the second port will forward whatever serial commands are sent through it to the Vesc. On the video showcase I posted earlier in this thread, I had the Photon receiver connected the second port, and it forwarded all commands to the Vesc.
```

---
## \#306 Posted by: mackann Posted at: 2019-01-23T21:18:35.046Z Reads: 147

```
This is such a great feature!
```

---
## \#307 Posted by: Jc06505n Posted at: 2019-01-23T21:28:14.937Z Reads: 158

```
Awesome, think I'm gana try out different designs. First ganna alter the STL above and take a look at the davega designs 

Think I'm going to follow @lrdesigns path with what he did for the davega

Here's the dimensions for the screen pcb: 

![image|322x500](upload://57gWswKn9DYKDrRndGI8f3viJUe.png)

Edit: On second thought, @lrdesigns, you mind if i try to remix the [case you made for the davega](https://www.thingiverse.com/thing:3171000/files)?  

It looks amazing , and I have absolutely no experience in 3d design but i want to see how far I'll get.
```

---
## \#308 Posted by: banjaxxed Posted at: 2019-01-23T22:18:59.947Z Reads: 158

```
Better get to work, there's a bit!

![image|608x499](upload://8LBEA5njoJDdWXpSGmJEGBzioGx.jpeg)
```

---
## \#309 Posted by: lrdesigns Posted at: 2019-01-24T03:55:36.644Z Reads: 155

```
I would like to give it a go but I am super busy right now. Where do I find a model or shape of the pcb?
```

---
## \#310 Posted by: Jc06505n Posted at: 2019-01-24T04:06:57.733Z Reads: 162

```
Shit that’s a big difference , I was just planning on taking out the buttons and enlarging the screen space

Oh boy. 

[quote="lrdesigns, post:309, topic:58664"]
Where do I find a model or shape of the pcb?
[/quote]

I think I got the dimensions of the pub for the screen above but I’m sure @Wajdi can provide what you need.
```

---
## \#311 Posted by: Wajdi Posted at: 2019-01-24T05:06:53.126Z Reads: 150

```
Enclosure is on Thingiverse https://www.thingiverse.com/thing:3359442
I also added STEP file for the electronics.
```

---
## \#312 Posted by: banjaxxed Posted at: 2019-01-24T09:24:58.358Z Reads: 153

```
That's a welcome addition.

I'm waiting for @lrdesigns version, the DaveGA treatment is really sweet.

@Wajdi you can see Luke is a design professional and a highly skilled one to boot. 

Can I be as bold to say to consider the inducement of a Proton to *ahem* check fitment of any forthcoming design. A sexy case is important for both form and function and gets the Proton seen to a wider audience, so your work can be fully appreciated.

![image|531x500](upload://adQTvXgzmtPCPDw9pnNIwL1IpIN.jpeg) 

:)
```

---
## \#313 Posted by: Wajdi Posted at: 2019-01-27T01:40:37.542Z Reads: 153

```
Thanks to the help of @Battosaii testings I was able to fix Focbox Unity compatibility and released MonitorV0.11.
It can downloaded from here: http://forum.eboardshop.net/t/firmware-update-download/59
```

---
## \#314 Posted by: Battosaii Posted at: 2019-01-27T01:45:20.581Z Reads: 157

```
![20190126_200133|666x500](upload://m8it4ug4EVTUxXxSuXLpDMTTeMO.jpeg) 

Looks so nice to.
```

---
## \#315 Posted by: banjaxxed Posted at: 2019-01-29T13:15:13.720Z Reads: 155

```
Got my parcel thanks, looking forward to testing it

Hopefully a 3D design guru makes something sexier for this kit

Not sure if you are plannning a v2 design of the PCB but it would be really nice to reposition the UART headers to the edge of the board near the USB and attach 90deg angled headers instead if possible.

Then the stl could be modified to also have a socket for that, the net result is a flat underside and lower profile overall. I am thinking of mounting one on the HAYA deck with Focboxes and Hummie hubs but I do not want to cut the deck at all so I will try making a hollow 'riser' for the existing case supplied, slightly angled, but tall enough the allow for USB cables to not be interfered and for the UART of course to have enough clearance 

Just a thought!
```

---
## \#316 Posted by: banjaxxed Posted at: 2019-01-29T22:41:01.028Z Reads: 151

```
Same problem with typical M5 countersunk skate bolt here. The holes at the rear seem to have a tab where the bolt would touch the sidewall, these 'tabs' break-off with a very small portion of bolt head entering the enclosure.

I made a test interface to avoid deck modification but unable to put them together with the front bolts as is. Upside down bolts would not not be my first choice, will have a go at modding the enclosure so you can bolt it in typical fashion

Edit: Tried really hard but failed, waiting on the gurus
```

---
## \#317 Posted by: banjaxxed Posted at: 2019-01-31T17:58:43.537Z Reads: 147

```
@Wajdi can you please post the stp you have. I am no 3D guru but I need a better case to mount this.

The stl is too hard to modify....please! It's useless to anyone with the proprietary electronics, nothing to lose

Too many faces when a mesh is imported, you quickly gets errors like this and lots of inconsistencies

![image|681x500](upload://bmaqfx5dgbdAkB6w0Eu0Oulf00C.png) 

Maybe the gurus know how to deal with this, but your average Proton buyer is waiting for a case design that is structurally strong and supports M5 typical skate bolts the normal way...it's a skateboard after all.
```

---
## \#318 Posted by: Friskies Posted at: 2019-02-01T00:28:40.750Z Reads: 139

```
Silly question here but why can't you just not use countersunk hardware? I don't know many bits of plastic that can handle that kind of force.
```

---
## \#319 Posted by: banjaxxed Posted at: 2019-02-01T12:25:19.407Z Reads: 137

```
Appreciate it!
```

---
## \#320 Posted by: Wajdi Posted at: 2019-02-01T16:53:37.009Z Reads: 142

```
Sorry for the late reply, I thought I published the .step files of the case as well, but I guess I did not, I updated the thingiverse file. I'm working on two part sliding design, where you can securely bolt the bottom part, and slide the top part that contains the display on it. Should solves the mounting issues due to size restrictions.
```

---
## \#321 Posted by: banjaxxed Posted at: 2019-02-01T23:45:38.289Z Reads: 140

```
getting there, thanks @Wajdi and @lrdesigns 

![image|658x500](upload://1dCEa8N1w8bCAAMdbkJMttJHfAE.jpeg)
```

---
## \#322 Posted by: Wajdi Posted at: 2019-02-01T23:49:07.234Z Reads: 137

```
I love it!
```

---
## \#323 Posted by: banjaxxed Posted at: 2019-02-02T13:19:07.716Z Reads: 136

```
First print didn’t fit back to the drawing board later tomorrow
```

---
## \#324 Posted by: Battosaii Posted at: 2019-02-03T00:50:01.529Z Reads: 137

```
Your awesome man.
```

---
## \#325 Posted by: totalgeek9224 Posted at: 2019-02-03T09:28:13.074Z Reads: 138

```
Love the modification! Will you have enough clearance for those USB's?
```

---
## \#326 Posted by: banjaxxed Posted at: 2019-02-03T13:33:40.047Z Reads: 139

```
Thanks, trying print No. 3 now. 

Yes I did factor in that a USB cable needs to be attached. A regular male USB *should* be ok but I have not modeled it in. Nothing like a test fit but I will of course try this and alter the angle as necessary.

The USB should point inboard(?), not even sure you can change the rotation of the screen in firmware. For rain ingress this is desirable. I have so far completely forgotten about the mini usb on the rear, something need to happen for that too.

So far only done the top section, the bottom will need to be printed and tested after I get the screen right.
```

---
## \#327 Posted by: banjaxxed Posted at: 2019-02-03T14:59:49.451Z Reads: 133

```
@Wajdi I’m a little confused on the buck wiring proton <>leds<>usb, can you draw a diagram of how that wires up assuming that you want all that function at the same time, for instance with 12v/24v led and your typical usb voltage as well. So two different voltages, is there a step-down on-board? I only noticed the two solder pads on bottom of the pcb
```

---
## \#328 Posted by: Wajdi Posted at: 2019-02-05T01:24:57.589Z Reads: 131

```
@banjaxxed The board doesn't have built in step down voltage regulator, you have to use an external one. So far only one voltage source input is supported, if you want to use the USBs then that input voltage should be around 5V. 
For the LEDs, I can add a new software button that acts as a digital switch, and use one of the led's data pin as a digital on/off.

For example if you have a fixed front light LEDs, that operate on 12/24 v, then you can simply use a power transistor connected to a digital pin on the board, and toggle them On/Off.
```

---
## \#329 Posted by: banjaxxed Posted at: 2019-02-05T11:12:51.644Z Reads: 131

```
Gotcha. Ok I understand, there is only one external power feed to the PCB, the probability is that USB is really desirable since the inputs are there, so a 5v step-down to feed those to the PCB point.

Then for LED lighting, just so I understand correctly -
Assuming 12v RGB LEDs are used -
Use another step-down buck to provide 12v directly to the power wires directly on the LEDS and control them by wiring the colour control wires of the LEDs via the plug on the pcb?

Might be my understanding of RGB LED lighting
```

---
## \#330 Posted by: banjaxxed Posted at: 2019-02-05T13:30:48.624Z Reads: 132

```
https://www.thingiverse.com/thing:3406021
```

---
## \#331 Posted by: Battosaii Posted at: 2019-02-05T17:15:42.616Z Reads: 129

```
OMG I want that now I need to find someone to print it for me.
```

---
## \#332 Posted by: Mich21050 Posted at: 2019-02-05T17:26:33.486Z Reads: 124

```
Where are you located? I might be able to print it for you :slight_smile:
```

---
## \#333 Posted by: Battosaii Posted at: 2019-02-05T17:29:02.002Z Reads: 124

```
I live in Miami, FL :slight_smile:
```

---
## \#334 Posted by: Mich21050 Posted at: 2019-02-05T17:29:34.373Z Reads: 123

```
Sorry I'm in the EU so shipping would be pretty expensive :slight_smile:
```

---
## \#335 Posted by: Battosaii Posted at: 2019-02-05T17:30:01.803Z Reads: 124

```
Thank you anyway :)
```

---
## \#336 Posted by: Mich21050 Posted at: 2019-02-05T17:32:05.146Z Reads: 127

```
Cheapest option would be 10€.
```

---
## \#337 Posted by: 701Superjet Posted at: 2019-02-06T01:00:18.821Z Reads: 130

```
@Wajdi Is the SD card slot set up to keep the total odometer count? Also id love a settings option for the live data screen to pick what is displayed on the graph.
```

---
## \#338 Posted by: Wajdi Posted at: 2019-02-09T15:34:39.265Z Reads: 127

```
@701Superjet Total odometer count can be saved without the need of an SD card, in the next update I will enable an option to activate it and to reset the count if needed.
Regarding the live graph, by picking you mean touching a point on the graph and display the values at that point?
```

---
## \#339 Posted by: mackann Posted at: 2019-02-09T17:07:53.831Z Reads: 128

```
Did you ship it with unity support or is a firmware update needed?
```

---
## \#340 Posted by: Jc06505n Posted at: 2019-02-09T17:46:13.098Z Reads: 131

```
[quote="Wajdi, post:313, topic:58664"]
Thanks to the help of @Battosaii testings I was able to fix Focbox Unity compatibility and released MonitorV0.11.
It can downloaded from here: [http://forum.eboardshop.net/t/firmware-update-download/59 ](http://forum.eboardshop.net/t/firmware-update-download/59)
[/quote]


Ten Jasons
```

---
## \#341 Posted by: Battosaii Posted at: 2019-02-09T19:16:11.323Z Reads: 131

```
I think he was asking if it will be shipped with the already updated firmware.  Either way it was pretty easy to do my only gripe was and is with any of these types of software was that it only works on Windows so I have a dual boot windows 10 on my MacBook pro.
```

---
## \#342 Posted by: 701Superjet Posted at: 2019-02-09T20:04:04.540Z Reads: 133

```
Ok awesome! For the graph I was thinking more along the lines of picking what is displayed since it is a small screen. For example you could select to have speed and motor amperage displayed. Or maybe battery amps and motor amps. Would be nice to display whatever you need but only display a couple options at a time. 

I have printed out a prototype of a mount for dropthrough trucks. I think it's going to work great. Just making some small adjustments now to make it better. I plan to publish it for everyone after the weekend.
```

---
## \#343 Posted by: 701Superjet Posted at: 2019-02-10T17:47:14.395Z Reads: 137

```
Drop through mount.![IMG_20190210_113401|666x500](upload://aBNGzUDjCNWYdQ1bWsx3pTLMQbu.jpeg) ![IMG_20190210_113417|666x500](upload://80q0Qv9841LX5snoE5CUlvtAw0F.jpeg) ![IMG_20190210_113305|666x500](upload://9lEDOA3jy3v1n2WuuDsvgQe98wb.jpeg) ![IMG_20190210_113340|666x500](upload://kDSyYaLRkSGendOHHQoCZJRDIKA.jpeg)
```

---
## \#344 Posted by: Wajdi Posted at: 2019-02-10T18:28:59.469Z Reads: 134

```
Looks awesome! Thanks for sharing.
Regarding your live graph request, I see what you mean, I will add that to the list of the next update.
So far I have this planned for the next update:
* Ability to rotate display 180 degrees
* Improved battery percentage calculation
* Pick what live graph values you want to monitor
* Add an option for persistent trip counter / add reset button
```

---
## \#345 Posted by: Farklinsburg Posted at: 2019-02-18T01:11:03.182Z Reads: 136

```
@701Superjet love your enclosure. Great job. Any chance of making the sti files available?
```

---
## \#346 Posted by: 701Superjet Posted at: 2019-02-18T03:06:45.501Z Reads: 136

```
Thank you! I put quite a bit of time into this. You can download the files here.

https://www.thingiverse.com/thing:3435535

Id appreciate any feedback. I would also appreciate any donations for my hard work if anyone feels like doing so.
```

---
## \#347 Posted by: Resonant Posted at: 2019-03-19T09:00:27.767Z Reads: 118

```
Any cases for this on a trampa?
```

---
## \#348 Posted by: banjaxxed Posted at: 2019-03-24T02:52:42.895Z Reads: 113

```
@Wajdi what’s the pinout  and connector spec for the led?
```

---
## \#349 Posted by: 701Superjet Posted at: 2019-03-24T12:27:26.686Z Reads: 113

```
![Screenshot_20190324-072614|327x500](upload://nQ2xKge5lq0pSvzLJwdTRyF1Ugb.jpeg)
```

---
## \#350 Posted by: banjaxxed Posted at: 2019-03-24T12:54:51.647Z Reads: 120

```
Thanks, do you know the exact connector used on the pcb?

Looking for led dummy guide really, plan is to just power board by a DC buck to 5v and power both the USB ports AND the LEDs. 

Idea being front and rear non-cosmetic lights will either be self powered or run through a separate buck

@Wajdi any chance you can shine some light on this? Maybe I missed something in vids or docs
```

---
## \#351 Posted by: Wajdi Posted at: 2019-06-04T22:23:16.933Z Reads: 95

```
Hi,

Sorry for the late response, I just released an update v0.13 that solved an issue with LED driver.
Here is how you connect the led strip:

![IMG_2448|375x500](upload://ayKQQgQlzeZ5UYyypv4YxZPYbTT.jpeg) 
(This is a proto pcb)

And here is a quick video of it in effect:
https://youtu.be/r2goMJz_wp8

Monitorv0.13 is available for download here https://forum.eboardshop.net/t/firmware-update-download/59

Let me know if you need any help!
```

---
## \#352 Posted by: banjaxxed Posted at: 2019-06-05T03:46:31.776Z Reads: 88

```
Thanks for the heads up @Wajdi I guess you updated the thread in the other place too. I’m trying this as soon as I can cheers
```

---
## \#353 Posted by: Flasher Posted at: 2019-06-10T19:14:44.189Z Reads: 78

```
Has anyone tried rerouting a 5v pin from the vesc to give current to the proton for use with LEDs? And if you have, what's the max output you can get from it? I don't own the panel yet so planning ahead in the meanwhile
```

---
## \#354 Posted by: Flasher Posted at: 2019-06-14T21:19:43.709Z Reads: 69

```
@Wajdi hey there got any updates on order? And maybe you can answer my previous question (previous post)
```

---
## \#355 Posted by: KingB Posted at: 2019-08-05T23:33:25.900Z Reads: 58

```
Just an idea regarding the waterproofing... I recently bought I waterproof iPad case. The ipad lacks buttons and is also a touch screen (obviously). There is a rim around the iPad on the screen that doesn’t actually register anything as a touch. It will recognize your finger but there is nothing is there on that part of the screen to open. The enclosure is plastic similar to ABS but when the front and back side clamp down around the iPad I noticed all that makes it “waterproof” from the screen is a 1-2mm rubber lining that lightly squeezes against the screen providing a seal protecting the rest of the iPad. I used to run my own business outside and needed the water proofing but didn’t want some piece of crap plastic bag feeling screen protector with a case. This allowed me to still touch the actual screen itself while maintaining a waterproof feature from drops and rain.. trust me I put it through it’s paces. Haha my screen go so wet it was actually hard to use and sometimes would not register my touch but everything else stayed perfectly dry. I even bought it at Walmart so I’m sure you could roll through your local store and find something similar but that wouldn't cost more than a few bucks per unit and maybe take two min to install if you applied it to the case first and then fit in the screen nice as snug against it during install, which seeing the unit (which I am buying) I don’t see how this wouldn’t already work with the screens tight looking fit already. It was fairly light and pretty squishy rubber that actually felt almost similar to welders glue after it dries. As for holding up against a full pressure water hose??? Ehh idk but that still wouldn’t have gotten enough water in there to damage anything I don’t think... the rain was Kentucky torrential downpour btw.. lol nothing you would want to stand outside for more the 60 seconds in especially with electronics but I had a job to do so....  anyways hope this helps and hope you will give it a try. I plan on buying a unit and was thinking about applying a tiny bit of welders glue around the edges because it dries like rubber and can easily be pulled off without damaging stuff. I use it on foam planes and apply it and remove it all the time without damage. I’ll be anxious to hear if you try something like this and how it works!
```

---
## \#356 Posted by: KingB Posted at: 2019-08-05T23:36:30.877Z Reads: 55

```
@Flasher I recently heard he is expecting shipment in September for his next batch.
```

---
## \#357 Posted by: atlasdev Posted at: 2019-09-22T21:13:34.931Z Reads: 42

```
Hi @Wajdi,

I've send an email a while ago, but I haven't received any response yet. I have a problem with my motor making a noise when not touching the remote, and telemetry which doesn't work. Can you please respond to my email?

Thanks!
```

---
