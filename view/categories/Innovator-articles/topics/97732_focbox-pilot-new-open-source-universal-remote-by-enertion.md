# FOCBOX Pilot &#124; New open-source universal remote by Enertion

### Replies: 79 Views: 4322

## \#1 Posted by: Deodand Posted at: 2019-07-02T18:25:59.633Z Reads: 657

```
![image|690x174](upload://710mTLVWXZaLFTb7TDe4ZSjLC3Q.png) 

Hello, we at Enertion Boards wanted to give you guys an early look at the remote we have been developing over the past year. Feel free to skim through this lengthy write up and give some feedback! 

Please forgive the rough print quality of our prototype, we've been rapidly iterating and are waiting on higher resolution prints to arrive before getting molds made. Please also note this is a prototype, we will continue sharing updates as the design is finalized. Here's a few renders to give you an idea where we are headed aesthetically: 

![front|281x500](upload://5IFnIAEtT0A9USrSE5COia01e3X.jpeg) ![standing%20up|281x500](upload://bIltmhPxJsNPjXaxduyMbaS1FHr.jpeg) 

![screen|690x388](upload://lM6URc2x4gWxovsPYGkZtvm7DtY.jpeg) 

**Throttle Design**

A remote is first and foremost the control of that (hopefully)  powerful beast sitting under your feet. A bad throttle can make it seem challenging to tame that power, and at it's worse can create dangerous situations during an accidental slip of the finger. Even more dangerous can be situations where electromechanical interfaces break down such as the oft-used but sometimes fragile potentiometer. Just this week in Denver we were unfortunate enough to witness a potentiometer failure that caused the throttle to lock up; launching a board uncontrolled into a curb damaging itself and (fortunately) nothing else. 

![IMG_20190614_165224|375x500,100%](upload://lHWjqwUkdXw2KEsnTMUYEKbOXCS.jpeg) 

We did a complete overhaul of the design to increase the tactile feedback and throw of the throttle. Strong neodymium magnets are used to provide ramping force feedback as you lay into the throttle. The changing magnetic field is also used as the sensing element for throttle position, which means the electronics are completely solid state. Because the magnets are strong enough to provide the spring force for the throttle they are also quite robust to incidental magnetic interference. Additionally, multiple embedded 3-axis hall senors combined with intelligent filtering ensure reliable and high-precision feedback of throttle angle. 

This all adds up to a premium throttle feel that meets the demanding requirements of even the most powerful high-end builds. 

**Telemetry & Durability, can we have both?**

We had *many* long discussions on what form of telemetry was best for our remote. Most remotes seem to be using OLEDs which can be difficult to see in sunlight, and testing showed them to be fragile when dropped. We also investigated E-ink displays and found similar problems with fragility. The most robust remotes seem to use the ever-reliable LED, which can be great for at-a-glance information on current battery levels etc. but the flexibility of what data can be displayed is limited and often not intuitive.  

![IMG_20190614_165345|666x500](upload://cdZz3o6d5gECTU9VkEdQ2tiR6Ta.jpeg) 

Ultimately we decided to for a more retro-style 0402 LED matrix, this allows for the display of numerical and text-based telemetry and is significantly more durable than any OLED screen we have tested thus far. It's shockingly bright when you crank up the brightness to max.  It also has the advantage of looking pretty cool when you scroll logos across it:

![](https://media.giphy.com/media/UVBW5rsSVveD60FWsL/source.gif)

To augment the telemetry data and offer more stylized output of data (battery, speed, throttle, current etc.)  we included a remap-able and customizable RGB bar. It has been suggested by leading experts that the RGB can improve performance of your board by 236%

![](https://media.giphy.com/media/VgaJYxmm20lS5q0fxi/source.gif)

Additionally there is a vibration motor for some tactile feedback. 

**Battery**

Nobody wants a remote that has to be recharged after every ride, or to use disposable batteries which generate harmful e-waste that is tedious to dispose of properly. The remote is slated to contain a 2Ah rechargeable lithium battery. Testing has shown the battery lasts over 30 hours with radio on full power and screens displaying at medium brightness. We'll continue testing as the firmware matures to get a more true-to-final estimate of battery life. Additionally we are upgrading to the durable USB C so no more torn off charge ports (unless you are really strong).

![IMG_20190614_164526|666x500](upload://oehEidZfqD2cDreVrDlWv603YiT.jpeg) 

**Wireless Stuff**

If you look around it seems a portion of remotes are moving to BLE modules, and leveraging the ESB (shockburst) protocol from Nordic. Many here on the forums have reported back mixed results with this protocol (it's what nrf24s use as well, think nunchuck remotes). Investigating further I realized it takes someone extremely well-versed in RF implementations to create a robust and reliable connection in interference ridden environments with this technology, and I'm fairly certain that is why results are such a mixed bag. 

Let's get into some nerdy bits so I  don't just sound like I'm pulling this from thin air. The [shockburst protocol](https://devzone.nordicsemi.com/nordic/nordic-blog/b/blog/posts/intro-to-shockburstenhanced-shockburst) leverages [GFSK modulation](https://en.wikipedia.org/wiki/Frequency-shift_keying), or Gaussian Frequency Shift Keying. This means it uses a fairly narrow band of frequencies to transmit data. If a strong interference shows up within the same bandwidth it can corrupt the signal, and in cities this can happen all too often. The common way to improve performance is to do Frequency-Hopping to spread the transmission spectrum randomly across a pre-set number of independent frequencies. This can get **pretty** complicated  and from my exploration it seems easy to implement incorrectly. 

We chose instead to go with a newer chip, namely the [SX1280](https://www.semtech.com/products/wireless-rf/24-ghz-transceivers/sx1280) . It was specifically designed for low-data rate and long range wireless links. The SX1280 contains some  integrated proprietary protocols that handle some of the heavy lifting for robust spread-spectrum transmission. These protocols should be less susceptible to the narrow-band interference you can encounter skating around big cities. As an illustration, with FLRC protocol on the sx1280 at an effective data-rate of 130 kbs you get a frequency spread of 300 kHz , by contrast GFSK is spread across 0.3 kHz. 

Let's look at a couple specs to see how it stacks up vs the newest [NRF52840](https://www.nordicsemi.com/-/media/Software-and-other-downloads/Product-Briefs/nRF52840-product-brief.pdf?la=en&hash=CE0FDDC1D5B83F5BB5DC5F031AF0A05ADA41D921) from Nordic. The easiest of these specs to understand are transmit-power, and receiver-sensitivity, both of which contribute to the robustness of the wireless link. You want a large dBm number for transmitting and small dBm for receiving.  The transmit-power of the sx1280 is 12.5 dBm vs the 8 dBm of the NRF52840. Decibels can be a bit confusing but in simple terms this means the sx1280 transmits a signal that's about 2.8 times more powerful than the latest NRF module (if its an NRF52832 that number is much higher still). Reciever-sensitivity is a bit more involved as varies depending on which protocol you implement with the sx1280, but using a handy calculator tool a 10ms on air 20 byte LoRa packet has a sensitivity around -109 dBm, and if you instead go for the FLRC protocol you can achieve a sensitivity of around -106 dBm. The NRF falls short here as well, the highest listed sensitivity in the datasheet is BLE long-range with a sensitivity of -103 dBm. But even with that best case scenario the receiver should detect signals that are 4x weaker in LoRa mode and half as strong in FLRC. In terms of range since we don't use a directional antenna, if we use LoRa we can say the module is:

    sqrt(2.8*4) = ~3.3 times the range

And in FLRC

    sqrt(2.8*2) = ~2.3 times the range

Now you're probably thinking "I'm standing right on top of the skateboard why do I want more range?", the answer is pretty straightforward. The difference between the transmit-power and receiver-sensitivity is called link-budget, and increasing distance is only one of many things that can negatively impact this value. Every bit of carbon-fiber in you're enclosure, every 2.4 Ghz network in your surroundings, even the sunlight or EMI thrown off by nearby electronics subtracts away from this number. With all of these negative factors you want to be sure that your remote is as reliable as possible to ensure your own safety. This isn't the whole story, and many other factors come into play to get more true to real-world range comparisons but I think we can all agree this section is already too long.

The combination of spread-spectrum transmission, increased transmission-power, and receiver-sensitivity should yield a remote that never  drops out on you while riding. Early testing has shown these modules seem to live up to the hype, but we are in the process of finalizing the design to prepare for beta-testing to ensure the connection holds in even the most interference ridden environments. Including those with many co-located remotes. 

**Mechanical Bits**

![explode|690x388](upload://qg3mLtpafbWdcvUdabCs7DZvUbw.jpeg) 

In terms of ergonomics, we wanted a design that could be held comfortably in either hand and would allow all buttons to remain accessible. We also wanted the design to be resistant to dust and contaminants.  To achieve this, the remote will feature a semi-transparent silicone gasket running the entire perimeter of the shell which seals in the electronics.  We will also be adding a loop for a wrist lanyard.

![](https://media.giphy.com/media/UuqIokzUqpouE9QaBJ/source.gif)

For the receiver side we will have a small module with an integrated CAN interface alongside PPM.  You will be able to connect to the FOCBOX app and customize the remote through CAN forwarding or connect to the computer through USB. We'll share more information here as the firmware evolves. 

**Open-Source Firmware**
 
We've talked at length about customization, because everyone has different ideas on what the perfect remote looks like. One of the reasons Vedder's work has been so popular in the community is the breadth of customization he allowed. The open source nature of his work enabled others to contribute their own designs, tweaks, and customization. The FOCBOX Unity further built upon this by simplifying the setup and ease-of-use of some of these tools and we intend to continue pushing forward these efforts with continued support and contributions from the community. 

We are excited to say we will be releasing the FOCBOX Pilot firmware open-source to allow the community to add their own customization and tweaks. I also had the pleasure of meeting up with @DerelictRobot and @Jonner while in Colorado, who are both doing a lot of cool and diverse work in the e-skate remote space. We talked at length on the topics of remote safety and reliability, and we all agreed having more collaboration to review the designs, architecture and code of this critical system would be a win for everyone involved.

We have begun working together to develop a small low-cost open-source development board consisting of the radio, micro-controller, and power regulation architecture including a single cell li-ion/lipo charge/discharge. This will be available for anyone seeking to develop their own remote and leverage the existing drivers and routines integrated within the firmware. While other developer platforms (like the adafruit feather) exist, they are not targeted specifically at e-skate remotes and the provided examples aren't intended for use within a system controlling a rocket under your feet. We hope together to develop a powerful codebase for other experienced developers looking to design a custom remote implementation while keeping the system simple enoguh that this platform can also be leveraged by hobbyists to build unique mechanical remote designs leveraging standard supported components.
```

---
## \#2 Posted by: Shaun Posted at: 2019-07-02T18:30:13.268Z Reads: 557

```
Nice one guys! Personally, I’m not a massive fan of the design - I think it looks like a Stanley knife.
```

---
## \#3 Posted by: venom121212 Posted at: 2019-07-02T18:34:51.990Z Reads: 554

```
I think it looks great Jeff
```

---
## \#4 Posted by: Blasto Posted at: 2019-07-02T18:36:20.465Z Reads: 547

```
We’d figured not everyone would keen on the design. Huge reason why we wanted to open source and collaborate with others. Get a nice safe protocol out, and derive from there
```

---
## \#5 Posted by: Jonner Posted at: 2019-07-02T18:44:56.535Z Reads: 522

```
I'm excited to be collaborating on this project.
```

---
## \#6 Posted by: Winfly Posted at: 2019-07-02T18:47:12.765Z Reads: 497

```
Put me down for one
```

---
## \#7 Posted by: dareno Posted at: 2019-07-02T18:49:22.264Z Reads: 483

```
Magnets are a clever idea.  I personally love that design, (I'm deliberately not using the term form factor because it makes vomit)   The name is pure genius.  Thats the level of my technical knowledge and input lol.  
The front trigger is what?  A dead man switch?
```

---
## \#8 Posted by: Deodand Posted at: 2019-07-02T18:52:28.521Z Reads: 471

```
I'll be making it selectable from a drop down:

- dead-man
 - cruise control
 - screen-go-brighter
 - nothing
 - insert someone elses better idea here
```

---
## \#9 Posted by: davidbonde Posted at: 2019-07-02T18:54:46.598Z Reads: 457

```
Had a change to hold the prototype in Colorado. The magnet thing felt really good! For me the most important thing in a remote is the feel of it and the feel of the trigger. This is very promising!
```

---
## \#10 Posted by: niuva Posted at: 2019-07-02T18:58:22.941Z Reads: 454

```
That magnet mechanism for the throttle seems interesting indeed. I'm so tired of crappy potentiometers (including gamepad analogsticks) and spring loaded hall effect mechanisms.

I can already imagine the feeling of pushing it - the closer to the limit you get the more resistance the magnets provide.

The lights on the palm side do feel a bit redundant on the design though, since they will be covered whenever the controller is being held?

Will the enclosure design also be open source, or only the software side of the controller?
Really looking forward to getting my hands on the code.
```

---
## \#11 Posted by: sofu Posted at: 2019-07-02T19:03:07.554Z Reads: 423

```
Awesome job @Deodand, can't wait to work together on this :blush:
```

---
## \#12 Posted by: meesie Posted at: 2019-07-02T19:03:20.435Z Reads: 420

```
I hope it lives up to what’s advertised. It looks and sounds cool!

I really really hope it doesnt have 1 relatively big drawback like all remotes have.

All remotes are either very reliable but too bulky, or they are reliable and small but only last an hour. Or their battery is good, they’re small but then they’re unreliable asf.... or they’re bajeezus expensive!

I hope this remote you’re working on will tick all of the boxes and come at a reasonable price
```

---
## \#13 Posted by: akhlut Posted at: 2019-07-02T19:05:24.660Z Reads: 413

```
Hell yes!

That magnetic spring feels SOOOOOOOOOO good!

Jam-packed with great ideas and expandable for more!  

I'm ready for this.
```

---
## \#14 Posted by: Halbj613 Posted at: 2019-07-02T19:08:08.777Z Reads: 393

```
What is shipping time going to be like
```

---
## \#15 Posted by: DerelictRobot Posted at: 2019-07-02T19:08:41.253Z Reads: 393

```
Everything is _terrible_ Jeff. Gosh.

Looking forward to helping create a unified & safe remote technology platform! Off to a great start.
```

---
## \#16 Posted by: walleywalker Posted at: 2019-07-02T19:10:22.153Z Reads: 387

```


Excellent! Might I suggest you have the remotes molded in a bright color as the design could be mistaken for a firearm.
```

---
## \#17 Posted by: bsancken Posted at: 2019-07-02T19:19:22.768Z Reads: 380

```
That look cool! Just how long do we actually have to wait... lol
```

---
## \#18 Posted by: CarlCollins Posted at: 2019-07-02T19:21:53.049Z Reads: 387

```
I really like the design and would definitely want to try it but I wish there was a minimal battery indicator on it so we will be aware that how much charge battery of remote have. :slight_smile:
```

---
## \#19 Posted by: akhlut Posted at: 2019-07-02T19:26:43.478Z Reads: 402

```
![image|575x464](upload://qELLefIuIVMzk4VikbyvkNn9daH.png)
```

---
## \#20 Posted by: dareno Posted at: 2019-07-02T19:33:08.979Z Reads: 396

```
[quote="Deodand, post:8, topic:97732"]
* dead-man
* cruise control
[/quote]

These 2 things to me are synonymous.  

I don't personally like a dead man switch on a remote.  I frequently let my remote hang from the lanyard on hills etc.  If the deadman switch activates some sort of brake failsafe then I'd hate it.  It would catch me out eventually.  Programmable function for it is cool though.  
I like simple.  If its not absolutely necessary then it doesn't go on my rig.  The only part that can not fail is the part thats not there.  Stole that from someone.
```

---
## \#21 Posted by: FranciscoV Posted at: 2019-07-02T19:36:53.397Z Reads: 379

```
I see deadman as being kinda not needed.    Instead I love what Hoyt st did with their remote where you can basically deactivate it by double clicking the power button
```

---
## \#22 Posted by: niuva Posted at: 2019-07-02T19:38:00.005Z Reads: 374

```
No idea how they plan on implementing deadmans switch, but at least on the remotes I've previously had it on it doesn't slam the brakes when you let go of the deadmans switch. Instead it doesn't let you throttle up without it being held down. Brakes work without it. 

Deadmans switch personally for me is a must. There have been so many times when I've launched my board as a projectile because my throttle got caught in my clothing as I was fiddling around with something else. Now I have skidmarks in my apartments floor that wont wash off.

Deadmans switch also adds a very welcome layer of safety in case of the throttle erroring out for some reason. (bug in the firmware or faulty hall sensor hardware)

But then again - it's open source. Pretty sure you could make it turn on your coffee maker somehow.
```

---
## \#23 Posted by: Bjork3n Posted at: 2019-07-02T19:38:34.606Z Reads: 357

```
Guys dont worry! It will be avalible 2023, they will get it right at the 5th batch. :sweat_smile:

Its a sweet looking remote for sure, nice work.
Keep it up :)

Deadman switch is ok , but then i would like the possibilty to turn it off, like the evolve remote.
```

---
## \#24 Posted by: FranciscoV Posted at: 2019-07-02T19:41:43.630Z Reads: 345

```
Aww 2023!?    Really!!??.   I need a remote now 😞
```

---
## \#25 Posted by: meesie Posted at: 2019-07-02T19:42:47.234Z Reads: 339

```
You have a point there, though i didn’t mean cheap. Also i didn’t say fast 😜
```

---
## \#26 Posted by: str8_Clutch Posted at: 2019-07-02T20:19:59.858Z Reads: 342

```
Nice work! Had the chance to see this thing at the esk8 convention in Denver! Love the innovation you guys are doing to push the industry further. Can’t wait to have one for myself.
```

---
## \#27 Posted by: barajabali Posted at: 2019-07-02T22:27:25.733Z Reads: 322

```
Awesome work @Deodand
```

---
## \#28 Posted by: Schulerbible Posted at: 2019-07-02T22:33:56.937Z Reads: 320

```
Use a magnetic usb charge port. Ican forsee this will be the first thing falling off. Or use glue to lock it down!
```

---
## \#29 Posted by: CarlCollins Posted at: 2019-07-02T22:41:31.905Z Reads: 319

```
I think now it will be USB-C so the issue with charge port will be fixed and gone for good :slight_smile:
```

---
## \#30 Posted by: Ixf Posted at: 2019-07-02T22:42:44.386Z Reads: 318

```
Love it! can't wait!
```

---
## \#31 Posted by: Devilmycry Posted at: 2019-07-03T00:28:57.498Z Reads: 310

```
Look beautiful love it 
Just the dead man really don’t like this 
Good job 🍾🍾🍾🍾
```

---
## \#32 Posted by: Genex Posted at: 2019-07-03T00:56:55.238Z Reads: 314

```
This is great; I love the idea of a dedicated RF board developed for esk8.  There are tons of options out there but having to repackage stuff like the GT2B just isn't reasonable, and there are no good open source options.

Do you plan to sell the PCB's alone, and if so do you have an idea of availability and price?

I've got a project that could **REALLY** use this kind of board; excited to see where it goes :)
```

---
## \#33 Posted by: Deodand Posted at: 2019-07-03T01:18:19.962Z Reads: 311

```
Thanks for your interest and enthusiasm! I'd like to organize a small run of them, they should be reasonably cheap so sitting on a small amount of stock shouldn't be too big of a deal... I'll share more when I know more :slight_smile:
```

---
## \#34 Posted by: Deodand Posted at: 2019-07-03T01:20:15.436Z Reads: 301

```
@Devilmycry Just to be clear the Deadman trigger can be fully disabled if it's not your cup of tea. It's not something I personally prefer either, but I did ram by board into @Blasto's ankle in Colorado so maybe I can't be trusted without one :smile:
```

---
## \#35 Posted by: Roan_Psyko Posted at: 2019-07-03T01:26:05.299Z Reads: 297

```
Great work Jeff! Super excited to get my hand on one and keen to see what the community does with it.
```

---
## \#36 Posted by: DrUnreliable Posted at: 2019-07-03T03:46:04.658Z Reads: 303

```
BLE with a solid protocol and chip. Good

LED array. Good

Customisable dead man. Good

Design. Schweet. Stanley knife haters be damned. It 
looks like a pilot control device to me. 

LEDs where your hand is, cool but I think hard to get value from as I won't be able yo watch under my hand when riding, just be wasting precious juice. And is a bit overkill as battery indication goes.
Perhaps a single LED pixel for battery would suffice?

Ya done good, please sell me one soon.
```

---
## \#37 Posted by: jasonbhuynh Posted at: 2019-07-03T04:44:01.507Z Reads: 290

```
Oof, is there a timeline for this? I'd certainly like to get in on it
```

---
## \#38 Posted by: deucesdown Posted at: 2019-07-03T05:29:44.306Z Reads: 315

```
Lovely. Looking forward to this.

[quote="Deodand, post:8, topic:97732"]
insert someone elses better idea here
[/quote]

Momentary or latching (configurable) to control a 2nd ppm channel, or a relay. For horns, lights, etc.

[quote="Deodand, post:1, topic:97732"]
For the receiver side we will have a small module with an integrated CAN interface alongside PPM
[/quote]

no UART, and instead CAN? Interdasting...

[quote="Deodand, post:1, topic:97732"]
The remote is slated to contain a 2Ah rechargeable lithium battery.
[/quote]

Please source good quality stuff, that won't puff after 10 cycles. Maybe even 1x18650, which are highly evolved now (tough, abuse tolerant, very high capacity).
```

---
## \#39 Posted by: evoheyax Posted at: 2019-07-03T05:56:41.479Z Reads: 310

```
Love to see the work. We need more remote options!

As always, impressed with your knowledge and ability to innovate Jeff!
```

---
## \#40 Posted by: ShutterShock Posted at: 2019-07-03T06:09:38.435Z Reads: 305

```
Very cool, looking forward to seeing this in person.  It would be great to have another reliable remote on the market!
```

---
## \#41 Posted by: L3chef Posted at: 2019-07-03T07:16:18.200Z Reads: 296

```
My body is ready ! Awesome work guys
```

---
## \#42 Posted by: 12meterkuk Posted at: 2019-07-03T09:20:08.595Z Reads: 287

```
You mean your wallet... 😂
```

---
## \#43 Posted by: venom121212 Posted at: 2019-07-03T11:55:20.449Z Reads: 276

```
https://giphy.com/gifs/adventure-time-12oQNsLa6CccDu
```

---
## \#44 Posted by: L3chef Posted at: 2019-07-03T12:10:30.404Z Reads: 271

```
Nope :joy:
```

---
## \#45 Posted by: Tangent Posted at: 2019-07-03T13:29:30.806Z Reads: 270

```
I love the idea of of using magnets to offer resistance, super novel and innovative, this is a definite GET for that alone, so much easier to modulate pressure than position, very very interested to see what it feels like in the hand. The rest of it looks super cool as well.. Talk about up staging Trampa.. My body is also ready👍
```

---
## \#48 Posted by: FranciscoV Posted at: 2019-07-03T14:12:46.542Z Reads: 261

```
Haha.   This is the third time I try but.   

Good one 😂
```

---
## \#49 Posted by: Devilmycry Posted at: 2019-07-03T14:44:09.126Z Reads: 258

```
Ok cool thank 🥂
```

---
## \#50 Posted by: Chupacabra Posted at: 2019-07-03T15:29:42.218Z Reads: 260

```
Love the design and the concept. Can’t wait to get my hands on this controller.
```

---
## \#51 Posted by: Ricco Posted at: 2019-07-03T17:08:31.559Z Reads: 253

```
This design is very impressive, but what's more impressive are the detailed explanations given for all of the design choices made. I really appreciate this because it opens peoples eyes to issues they didnt know were there and would not have thought to look for in other remote designs.
```

---
## \#52 Posted by: thisguyhere Posted at: 2019-07-03T17:16:25.579Z Reads: 247

```
what if one's primitive monkey brain can't get a handle on using thumb throttles?
```

---
## \#53 Posted by: deucesdown Posted at: 2019-07-03T17:24:11.160Z Reads: 247

```
Have you tried thumbwheels with longer throw? I find nano-x twitchy but get along fine with the ownboard remote. I prefer trigger for control but thumb works better with gloves and going in and out of pockets.
```

---
## \#54 Posted by: thisguyhere Posted at: 2019-07-03T18:12:43.436Z Reads: 244

```
yea i keep hitting the trigger accidentally and getting jolted.  

so thumb control's better for that reason but i just can't get the articulation i get with the trigger.
```

---
## \#55 Posted by: Toughook Posted at: 2019-07-03T19:58:40.034Z Reads: 242

```
You had me at 236% 😍
```

---
## \#56 Posted by: Launchy21 Posted at: 2019-07-03T21:10:27.390Z Reads: 245

```
Does the Pilot need recalibration like the Nano-X does? This is my biggest QoL annoyance with this board and I'd really like to see that changed - I mean, even two completely different brands like Boosted and Backfire don't need calibration, so I'd love to see Enertion go that same route.
```

---
## \#57 Posted by: niuva Posted at: 2019-07-03T21:24:17.236Z Reads: 246

```
IIRC the Nano X used a potentiometer and the pilot does not. Instead it uses multiple Hall sensors, so I'm fairly certain no recalibration is needed.
```

---
## \#58 Posted by: Deodand Posted at: 2019-07-03T23:02:00.665Z Reads: 243

```
Absolutely will not need re-calibration after every power cycle.
```

---
## \#59 Posted by: Launchy21 Posted at: 2019-07-03T23:49:09.414Z Reads: 244

```
Thank goodness! This remote is shaping up to be a SOLID upgrade!
How about the materials? The render makes it look like a plastic/rubber build - how does it differ from the Nano-X or has that yet to be determined? I wonder how an aluminum remote with rubber contours would feel...
```

---
## \#60 Posted by: Friskies Posted at: 2019-07-04T12:28:06.377Z Reads: 244

```
I will sell my first born child for a Dev kit @Deodand
```

---
## \#61 Posted by: meesie Posted at: 2019-07-05T10:53:03.552Z Reads: 243

```
[quote="deucesdown, post:38, topic:97732"]
Momentary or latching (configurable) to control a 2nd ppm channel, or a relay. For horns, lights, etc
[/quote]

![image|360x328](upload://kvzviiBnagFW4WH4Tz8ORMwjsqo.jpeg)

as for my own input, i'd like to have rubber-like material on the "trigger." my thumb always slips back on those plastic triggers, especially in warm weather. do more people experience this?
```

---
## \#62 Posted by: Zaphod Posted at: 2019-07-08T01:05:19.052Z Reads: 230

```
I'm surprised that people are hating on the aesthetic. I think it looks amazing. The only way to one up this for me would be a power-glove form factor so you can wear slide pucks and throttle by clenching fingers.
```

---
## \#63 Posted by: baxter Posted at: 2019-07-08T11:45:41.319Z Reads: 217

```
Fully support what you are trying to achieve @Deodand !

I would have thought enertion as design leader might want to consider other forms of remote controls. Technical improvements aside, the proposed (initial) form factor seems a little derivative of the nano-x, and should support other form factors

Here's a very basic concept I prepared earlier based on a slot car remote (perhaps skip forward to post 15). The linear slide would require less articulation of the thumb, than existing thumb trigger remotes. 

https://www.electric-skateboard.builders/t/esk8-remote-control-concept/21898

I was thinking in addition to the 18650 battery, maybe put two digital readouts parallel to the potentiometer , on each side of the remote (for left and right handed operation), so the rider can look into the fist of their hand to see speed/data etc.

![image|533x312](upload://4F342mN7Vdu7kdIPuy5JH52Ik8K.jpeg)
```

---
## \#64 Posted by: drone001 Posted at: 2019-07-09T00:36:35.299Z Reads: 202

```
siiiiick!!! damn Jeff that's bad ass bruh.
```

---
## \#65 Posted by: billappleton Posted at: 2019-07-09T05:34:36.082Z Reads: 199

```
What kind of special connection to Unity? That’s the point, right?
```

---
## \#66 Posted by: Deodand Posted at: 2019-07-09T20:20:33.102Z Reads: 188

```
It will connect to the Unity via CAN interface to provide a mroe reliable connection than UART.
```

---
## \#67 Posted by: cubed Posted at: 2019-07-09T20:25:20.974Z Reads: 197

```
Couple of questions;

* Will this work with the original focbox?
* Would it be possible to pair it to a phone or other bluetooth devices to add other functionality (directions via google maps, led color control on the board)?
* Potential release date?
```

---
## \#68 Posted by: mikenyc Posted at: 2019-07-09T20:34:11.971Z Reads: 196

```
what about 4wd set ups?
```

---
## \#69 Posted by: Deodand Posted at: 2019-07-09T21:50:07.199Z Reads: 203

```
[quote="mikenyc, post:68, topic:97732, full:true"]
what about 4wd set ups?
[/quote]
CAN is a parallel bus so we will include a dual port to support 4WD

[quote="cubed, post:67, topic:97732"]
Will this work with the original focbox?
[/quote]

Currently working on firmware, plans are to support both Unity and singles. Might see more complete support for unity at first simply because I have more control over that firmware. 

[quote="cubed, post:67, topic:97732"]
Potential release date?
[/quote]

We still need to do a second alpha run and then a larger beta run before starting production. I'd estimate 2 months if we worked REALLY fast but realistically it will probably take longer to fully test and vet everything. 

[quote="cubed, post:67, topic:97732"]
Would it be possible to pair it to a phone or other bluetooth devices to add other functionality (directions via google maps, led color control on the board)?
[/quote]

There will be support for customization settings via the app, probably not turn by turn (at least not at first)  don't really want to encourage anyone to take eyes off road to look at display frequently while riding and the remote won't have a speaker. 

[quote="baxter, post:63, topic:97732"]
Here’s a very basic concept I prepared earlier based on a slot car remote
[/quote]

Unfortunately we don't currently have the engineering resources to reliably launch multiple remote types without outside assistance. The goal with the  open source design is to create a platform that makes it easier to design other unique remotes.
```

---
## \#70 Posted by: billappleton Posted at: 2019-07-09T22:03:54.560Z Reads: 192

```
that's good, but seems like an opportunity for advanced battery levels, range, temperature, rpm, distance traveled, etc.
```

---
## \#71 Posted by: skatardude10 Posted at: 2019-07-09T22:23:11.937Z Reads: 191

```
I'd love to get in on the beta test for this. Ever since swapping my Nano-X over to my Haya (dirty wiring, 8awg pulling 160 amps all over the place back and forth (filtered with a capacitor bank before ESCs) I've been experiencing numerous cutouts, boards throttling/braking randomly, lost connections, etc. It hurts. Lol.

Short of just removing my receiver from inside the board or really doing some magic with the wiring to reduce inductance, I'm not sure what to do.
```

---
## \#72 Posted by: cubed Posted at: 2019-07-09T23:49:17.017Z Reads: 188

```
Let me know when the beta test happens! Id be happy to be a part of it, thanks!
```

---
## \#73 Posted by: deucesdown Posted at: 2019-07-10T00:37:03.596Z Reads: 193

```
Dedicated battery pack for the receiver? I know space is tight though.
```

---
## \#74 Posted by: Launchy21 Posted at: 2019-07-16T20:06:52.469Z Reads: 187

```
How do you turn this remote on? What sort of power switch is it going to use? 
Will this remote be able to turn the board on and off remotely? 
I'm so curious!!
```

---
## \#75 Posted by: tomiboi Posted at: 2019-07-16T21:55:59.775Z Reads: 191

```
A lot of really awesome ideas. The thumbwheel looks legit. I love the lights. How about wood or bamboo for the outer panels? Make it feel real nice.
```

---
## \#76 Posted by: Jomant Posted at: 2019-07-19T13:04:55.450Z Reads: 184

```
PleAse make sure that the Type C has a reenforced bracket which is held with screws and hot glue. Don't like to see a type c socket rattle inside this nice looking remote. Plus make a elite edition out of aluminum oxidate in Black and charge me $100 more. Even more durable.
```

---
## \#77 Posted by: WAVMOB Posted at: 2019-07-19T13:30:32.534Z Reads: 191

```
A deadman switch would make it safer. There were times on my Raptor I reached with my remote hand to adjust my helmet strap and accidentally accelerated even though my thumb was off the remote itself but the throttle got pushed by the helmet strap or jus t anything in the way.

The LEDs could serve as a good flashlight since it would face forward if we just dropped our arms to its naturally rested position and would face upcoming traffic.

Great design!!!
```

---
## \#78 Posted by: jadatmag Posted at: 2019-09-06T13:00:34.087Z Reads: 153

```
This still alive?
```

---
## \#79 Posted by: Richcan Posted at: 2019-10-01T12:57:29.743Z Reads: 128

```
I found the nano remote to big in the palm? Does not grip comfortable compared to my meepo classic remote with the finger hole. I’ve passed it around to friends they all said the same. If it was more slim would be better?
```

---
## \#80 Posted by: MikEeee Posted at: 2019-11-01T06:18:37.317Z Reads: 91

```
Look Im no scientist  but I think we are all thinking the same thing, An sk8 remote that resembles an expensive piece of equipment because just like a smartphone no one wants to hold a flimsy piece of plastic they want a real phone with heavy materials like glass and metal which doesn't exist currently  its a shame if you ask me. Reliability  is also a big problem I can't speak much  in this regard but it needs some sort Saftey mechanism to improve safety, and pls for the love of god no one wants a RGB ULTRA VIS Gmr vibe  a speed omiter  and bttry % display
```

---
## \#81 Posted by: Halbj613 Posted at: 2019-11-01T07:09:30.544Z Reads: 89

```
Thank you for telling them what all of us wanted after reading about esk8 for 5 minutes
```

---
