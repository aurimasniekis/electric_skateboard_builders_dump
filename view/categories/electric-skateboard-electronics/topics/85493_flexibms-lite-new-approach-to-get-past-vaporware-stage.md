# FlexiBMS Lite - New approach to get past Vaporware stage

### Replies: 269 Views: 6386

## \#1 Posted by: SimosMCmuffin Posted at: 2019-02-26T19:01:23.469Z Reads: 608

```
Hey, It's been a while since I've been active in the forums, but spring is finally approaching Finland. Roads are finally starting to loose their ice coatings, the air is warming and the light time outside is getting longer, so I feel like it's to become active again (3D printing some mudguards for my board atm, so I can get on the roads once the ice melts).

I would first like to have a look-back on my first approach for a BMS for the esk8 community (https://www.electric-skateboard.builders/t/flexibms-0-2-hw-under-work-flexible-configuration-and-charging-bms/46117) and identify the problems with it and how to solve them at least partially with the focus being on developing something functional that can be shipped.

The problem can be summarized as "Trying to do too much cool stuff at once" this caused high component cost, while hamstringing performance of the board as a whole. Even though the BMS was functional it had multiple tripping points on it's way for mass-production.

So my solution will be to simplify/streamline and cut back features to bring down the component cost, lower assembly costs and make the board more sensible as a whole. I will list below some of the changes and the reasons for them:

- **Design ethos/focus should be aimed at the layman esk8 hobbyist and battery builders**
BMS doesn't need to loaded with all the imaginable features, because the layman esk8 user doesn't need them or will never in the most cases use them. Most people just want to charge their battery safely and don't need to have all their components interconnected. They need something simple, flexible (series cell count wise), reliable and affordable.


- **Remove the whole boost SMPS block**
It was a cool idea IMO, but now in hindsight it really didn't make sense. Thermal limitations were the biggest problem, plus it was quite expensive as a block. Easiest solution for this is to externalize this feature to the charger, and even with it, you would still have needed an external power source. Higher charging power ceiling as well due to heat generation being much lower on the board itself. You can get decent battery chargers (CC/CV) from china for good price these days.

- **Remove extra module connector**
Save costs, KIS

- **Cheaper MCU**
Moving from STM32L433 to STM32L052, lots of unneeded peripherals. Cuts MCU cost roughly in half from 5€ to 2,5€

- **Cheaper 5V buck SMPS**
Moving from MAX17502 (1 Amp) to MAX15062 (0.3 Amp). Overkill, price and size.

- **Higher balance current**
With more board space available and less heat generation due to no SMPS block, we can switch to bigger package bleed resistor and increase balance current from ~90 mA to ~140 mA.

- **Cheaper current sense circuitry**
ISL28022 is a really good IC, but maybe a bit overkill. I'm testing with a INA180 for price cutting.

- **Full blocking charging switches**
Problem with the earlier implementation was that battery voltage was always present at the bulk charger connector (flowed through the P-channel body diode). This was a safety concern for me personally. Charging switches are now 2 n-channel mosfets with common drain, controlled by BQ76200, enabling a fully blocking setup.

- **CAN and USART removed**
Cheaper MCU doesn't have CAN support. Maybe USART can have some solder pads, but no connector. **Opinions welcome**.

So what are the planned BMS' features?
- **3S-12S series cells support**
Flexible series cells support
- **140 mA balance current**
Higher balance current
- **9 A max charging current**
Higher maximum charging power
- **Pack temperature NTC probe for thermal monitoring**
Solder pads or a dedicated connector.
- **USB connectivity for parameter configuration and charging monitoring**
Configurable parameter: Max charging current, charging end current, max cell voltage, cell balancing behavior, temperature limits.
- **Buzzer for audio signaling**
_Interested in opinions on implementation_
- **On board status LED**
_Interested in opinions on implementation_
- **Smaller PCB**
With a lot of components removed, I can shrink the board down further.


I'm planning on splitting the FlexiBMS into a **Lite and Basic** versions, with Basic being more feature rich and Lite being the no-bells-and-whistles version meant for battery pack builder integration/basic functionality for controlled charging.

Layout WIP picture.
![image|690x421](upload://oHrYb2qgf8vVXNqmk9TB0Za0B4H.jpeg) 

Currently when I've been sourcing the components from Digi-Key with the planned amount for 100 boards and the total is standing a bit over 2000€ or 20€ per board, which is MUCH lower than with the earlier approach and is something that even I feel safe to pull a trigger for ordering.

**I aim the sell price to be between 40€-60€**

And as always I welcome comments and questions from the community and invite everybody to the conversation.
```

---
## \#2 Posted by: Blasto Posted at: 2019-02-26T19:19:10.072Z Reads: 489

```
[quote="SimosMCmuffin, post:1, topic:85493"]
**CAN and USART removed**
Cheaper MCU doesn’t have CAN support. Maybe USART can have some solder pads, but no connector. **Opinions welcome** .
[/quote]

I would keep CAN, go for STM32L0 ?

[quote="SimosMCmuffin, post:1, topic:85493"]
**Higher balance current**
With more board space available and less heat generation due to no SMPS block, we can switch to bigger package bleed resistor and increase balance current from ~90 mA to ~140 mA.
[/quote]

would be careful here, those resistors will get real hot even when only pulling 1/2W

[quote="SimosMCmuffin, post:1, topic:85493"]
Buzzer for audio signaling
[/quote]

probably useless inside an enclosure, especially it's a pretty big component
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2019-02-26T19:47:24.614Z Reads: 442

```
[quote="Blasto, post:2, topic:85493"]
I would keep CAN, go for STM32L0 ?
[/quote]

[quote="SimosMCmuffin, post:1, topic:85493"]
**Cheaper MCU**
Moving from STM32L433 to STM32L052, lots of unneeded peripherals. Cuts MCU cost roughly in half from 5€ to 2,5€
[/quote]
Only STM32L4's have CAN connectivity (re-checked).

[quote="Blasto, post:2, topic:85493"]
would be careful here, those resistors will get real hot even when only pulling 1/2W
[/quote]
Will have to check thermal performance once I have the first prototypes on hand.

[quote="Blasto, post:2, topic:85493"]
probably useless inside an enclosure, especially it’s a pretty big component
[/quote]
This was one of the concerns with the buzzer implementation. It's cheap though, only 29 cents in volume, but quite large size-wise. Could maybe even shrink down the board further without it. My other question is how should the audio warning be implemented if there isn't a button on the board or externally to clear warning states? Play warning tune for couple seconds and repeat after couple of minutes if warning state is still true, let's say for example cell undervoltage.

And considering the BMS might wrapped in a kapton layer and inside a foam padded enclosure (pic below)... Not sure if you need the status LED for the same reasons...
https://www.electric-skateboard.builders/uploads/db1493/original/3X/7/0/70d6395476a2a171260979970b0e8ec8a7d768dd.jpeg
```

---
## \#4 Posted by: Blasto Posted at: 2019-02-26T19:48:33.658Z Reads: 358

```
My mistake! i meant STM32F0
```

---
## \#5 Posted by: Surfer Posted at: 2019-02-26T19:48:50.335Z Reads: 355

```
I like the idea to connect a Bluetooth module to the BMS and get the info in my phone, even if it's only monitoring I'm happy with it
```

---
## \#6 Posted by: ducktaperules Posted at: 2019-02-26T20:09:13.712Z Reads: 359

```
I feel like uart connection to the VESC is a fer better idea the BMS having its own bluetooth module, most peoples VESC already has some type of wireless module built in and support relaying BMS information to phone apps.

Additionally a small charge only BMS paired with a Focbox Unity which already has antispark built in could be super low cost and easy settup configuration.
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2019-02-26T20:10:26.465Z Reads: 363

```
What would you say about the idea of the Lite being the barebones version and then making the Basic, bigger and more expensive with better connectivity?

[quote="SimosMCmuffin, post:1, topic:85493"]
I’m planning on splitting the FlexiBMS into a **Lite and Basic** versions, with Basic being more feature rich and Lite being the no-bells-and-whistles version meant for battery pack builder integration/basic functionality for controlled charging.
[/quote]
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2019-02-26T20:12:36.866Z Reads: 345

```
So would say it would make sense to have the bare-bones charge-only Lite version, and then a Basic version with better connectivity?

[quote="SimosMCmuffin, post:1, topic:85493"]
I’m planning on splitting the FlexiBMS into a **Lite and Basic** versions, with Basic being more feature rich and Lite being the no-bells-and-whistles version meant for battery pack builder integration/basic functionality for controlled charging.
[/quote]
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2019-02-26T20:20:40.912Z Reads: 345

```
By the way, here are some of the cheap series cell specific chargers that I mentioned:

6S
https://www.aliexpress.com/store/product/25-2V-3A-Charger-6S-22-2V-Li-ion-electric-bike-battery-22-2V-Lithium-Battery/1728275_32840379224.html?spm=2114.12010612.8148356.14.4a0523e1ZuCgMP

7S
https://www.aliexpress.com/store/product/29-4V-3A-Charger-7S-24V-Li-ion-electric-bike-battery-24V-Lithium-Battery-Charger-Input/1728275_32840367637.html?spm=2114.12010612.8148356.16.68ad23e1B8tqzC

8S
https://www.aliexpress.com/store/product/33-6V1-8A-battery-charger-8S-33-6V-charger-output-33-6V1-8A-33-6V1-8A/1728275_32761610145.html?spm=2114.12010612.8148356.12.1ba723e1VJUHOg

9S
https://www.aliexpress.com/store/product/37-8V-2A-Charger-9S-33-3V-Li-ion-electric-bike-battery-33-3V-Lithium-Battery/1728275_32838696113.html?spm=2114.12010612.8148356.16.443723e1MICRId

10S
https://www.aliexpress.com/store/product/42V3A-Charger-10S-36V-Li-ion-Battery-Charger-Output-DC-42V-Lithium-polymer-battery-Charger-Free/1728275_32763152800.html?spm=2114.12010612.8148356.4.16dc23e1fhKOnJ

11S charger seems to be a bit exotic

12S
https://www.aliexpress.com/store/product/50-4V-1-5A-Charger-12S-44-4V-Li-ion-electric-bike-battery-44-4V-Lithium/1728275_32839194001.html?spm=2114.12010612.8148356.16.7c2d3accAeP3gl
```

---
## \#10 Posted by: ducktaperules Posted at: 2019-02-26T20:33:13.547Z Reads: 298

```
I think you need some sort of power switch in your system somewhere to shutdown in fault conditions.
If there was a "lite" charge only version with no large (expensive) power switching then adding UART (basically free) allows you to send shutdown command to Unity or similar with built in antispark. 

Im not aware of another bms that works this way. it could result in a very low cost BMS with lots of features that is perfect for easy DIY builds. 

Then for the "power users" a variant with high current power switching, bluetooth, CAN and all the fancy stuff built in. But honestly not everyone needs these things and there are lots of products that already offer these features. what we seem to be missing at the moment is a cheep, simple reliable BMS for the new generation of more integrated VESC's that is arriving.
```

---
## \#11 Posted by: Friskies Posted at: 2019-02-26T20:37:20.570Z Reads: 288

```
I would keep CAN or build in wifi or bluetooth. - ditch the buzzer and just go with an led that can show charging states eg: charging->balancing->chargedandbalanced.

I think the trick will be just giving a good compact BMS with solid specs and some connectivity but importantly shows the info quickly and simply.
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2019-02-26T21:10:13.348Z Reads: 290

```
& @Friskies 
[quote="ducktaperules, post:10, topic:85493"]
I think you need some sort of power switch in your system somewhere to shutdown in fault conditions.
If there was a “lite” charge only version with no large (expensive) power switching then adding UART (basically free) allows you to send shutdown command to Unity or similar with built in antispark.
[/quote]

Good point. If the buzzer is ditched, there is ample space for a dedicated USART connector, which can be hooked up to a VESC-derivative or used to disable an independent E-switch, if it supports low-voltage fault signal.

CAN would cost roughly 2€ in components to implement (transreceiver + STM32L4). Worth it?
```

---
## \#13 Posted by: Acido Posted at: 2019-02-26T21:16:51.051Z Reads: 265

```
This looks amazingly small!
Good work, after some time passes and people prove its reliable, I will recommend it to my battery customers to support forum members :)

This probably is answered in the other thread, but does this bms balance all the time or only when charging?
```

---
## \#14 Posted by: rpasichnyk Posted at: 2019-02-26T21:18:28.583Z Reads: 248

```
Please keep CAN :slight_smile:
```

---
## \#15 Posted by: Arek Posted at: 2019-02-26T21:23:03.144Z Reads: 244

```
So this BMS is not passing the main power and just monitoring/balancing the cells?

And yes pls keep CAN
```

---
## \#16 Posted by: SimosMCmuffin Posted at: 2019-02-26T21:37:52.462Z Reads: 259

```
[quote="Acido, post:13, topic:85493"]
This probably is answered in the other thread, but does this bms balance all the time or only when charging?
[/quote]

I don't see any reason why it couldn't balance when not charging. At that point it's just firmware implementation question. It's going to have to monitor cell voltages anyway to look for un-balance, under- and overvoltage conditions.

[quote="rpasichnyk, post:14, topic:85493"]
Please keep CAN :slight_smile:
[/quote]

[quote="Arek, post:15, topic:85493"]
And yes pls keep CAN
[/quote]

I'll look into integrating it tomorrow.

[quote="Arek, post:15, topic:85493"]
So this BMS is not passing the main power and just monitoring/balancing the cells?
[/quote]

This planned Lite model won't have a discharge path mosfet control, but is rather just used to control charging via external charger and then monitor cells and communicate via USART or CAN.

The Basic model could have discharge path control mosfets integrated onto it.
```

---
## \#17 Posted by: Arek Posted at: 2019-02-26T21:48:03.633Z Reads: 246

```
[quote="SimosMCmuffin, post:16, topic:85493"]
This planned Lite model won’t have a discharge path mosfet control, but is rather just used to control charging via external charger and then monitor cells and communicate via USART or CAN.
[/quote]

OMG THIS IS WHAT I DESIGNED IN MY HEAD LIKE A MONTH AGO :smiley: 
... after I realised that I won't get DieBieMS and that I wasn't happy with the discharge current limitations anyway.

Can I go in as a prototype tester/builder(that's my actual work)?
I can solder down to 0402 no problem or whatever uC package.

Make sure you design it to alarm the VESC/Unity through CAN when one section is low on voltage and trigger shut down in the ESC
```

---
## \#18 Posted by: SimosMCmuffin Posted at: 2019-02-27T09:03:38.500Z Reads: 252

```
Here's a updated block diagram for the board

![image|690x379](upload://s4IQNhvSzN6T5YKMNEwcobjHDgb.png)   

I'm planning on keeping the MCU always powered on via the LTC6803 5V regulator output dropped down to 3V3 via linear. This is a low power supply, about 4-6mA max and power all the other devices through the 5V buck smps and another 3V3 linear. I can then shut them down by disabling the 5V buck while still leaving the MCU powered.

I also checked the STM32L431 datasheet and discovered for my delight that most of the I/Os are 5Volt tolerant, so I can for example use 5 Volt CAN ICs without level translator between the CAN and MCU.
```

---
## \#19 Posted by: Komamtb Posted at: 2019-02-27T09:22:47.374Z Reads: 233

```
Not 13s capable? A button integration would be sweet. Side note, someone could thing of a design for a bms and antispark in a single unit maybe. With simplified connections.
```

---
## \#20 Posted by: SimosMCmuffin Posted at: 2019-02-27T09:32:32.959Z Reads: 248

```
[quote="Komamtb, post:19, topic:85493"]
Not 13s capable?
[/quote]
Isn't 13S a bit exotic? 12S should be plenty high for the majority of the users. Implementation costs also jump a LOT when moving past 12S if you also want balancing.

[quote="Komamtb, post:19, topic:85493"]
A button integration would be sweet.
[/quote]
What would this button be used for? If it's mean for the anti-spark switch, then why not wire the switch directly onto that?

[quote="Komamtb, post:19, topic:85493"]
Side note, someone could thing of a design for a bms and antispark in a single unit maybe. With simplified connections.
[/quote]
This is the Lite version, Basic version would most likely be bigger in size and include integrated discharge path control switches.


**SIDE NOTE**
I have taken couple days free from work and I intend to use the rest of the week to design the first iteration of this BMS, so I will be available on the forum for the rest of the week.
```

---
## \#21 Posted by: pjotr47 Posted at: 2019-02-27T10:38:40.207Z Reads: 220

```
That BMS looks really small. That would be something awesome for my costumers who want charge only battery packs :yum:
```

---
## \#22 Posted by: b264 Posted at: 2019-02-27T11:03:32.935Z Reads: 221

```
I love all of this!!  

Well except:
[quote="SimosMCmuffin, post:1, topic:85493"]
Problem with the earlier implementation was that battery voltage was always present at the bulk charger connector (flowed through the P-channel body diode). This was a safety concern for me personally. Charging switches are now 2 n-channel mosfets with common drain, controlled by BQ76200, enabling a fully blocking setup.
[/quote]

OMG no!  Some folks plug their battery gauges into the charge ports.  I'm not sure the reason to do this is worth the cost and reduced functionality.

Overall I love the approach though.

I'd like to add that the #1 reason off-the-shelf BMS aren't adequate for esk8 -- besides obvious reasons like discharge current too low -- is that they don't have roll-to-start.

I think you should look at it from that perspective.  What do we need that a regular BMS doesn't provide?  Roll-to-start is like the only thing... and maybe auto-poweroff after 1 hour of no activity.  That'd allow you to not even have a power switch on your skate.... just put it on the ground and skate.  And step off it when you're done.
```

---
## \#23 Posted by: b264 Posted at: 2019-02-27T11:04:58.210Z Reads: 197

```
That [10S charger you linked](https://forum./t/pictures-and-nothing-else/79/55?u=b264) is a piece of shit.  I've had more than one fail one.  The only chargers I've ever had fail.
```

---
## \#24 Posted by: Pimousse Posted at: 2019-02-27T11:07:13.682Z Reads: 209

```
Like for the precedent FlexiBMS project, I really like your approach.
CAN comm is really needed IMHO. @rpasichnyk proved it this the DieBieMS integration into Metr app.

However, not sure that the current COMM protocol coded into VESC FW supports commands such as "Stop", mostly for the Master one.
But, this is something really interesting and it's worth to PR it to Vedder. :slight_smile:
```

---
## \#25 Posted by: SimosMCmuffin Posted at: 2019-02-27T11:25:28.622Z Reads: 215

```
[quote="b264, post:22, topic:85493"]
I’d like to add that the #1 reason off-the-shelf BMS aren’t adequate for esk8 – besides obvious reasons like discharge current too low – is that they don’t have roll-to-start.
[/quote]

How is roll-to-start usually implemented? Motor controller senses wheel rotation and sends a command to e-switch to turn on?

[quote="b264, post:22, topic:85493"]
OMG no! Some folks plug their battery gauges into the charge ports. I’m not sure the reason to do this is worth the cost and reduced functionality.
[/quote]
They do? Well I mean I can just take the other N-channel FET off and voltage would be able to go to to the charger input. Problem is that I need to have charger_sense circuitry to detect when a charger is plugged in and the current implementation is done as a resistive divider, which would cause extra quiescent current draw from the battery when not charging if the FETs are not in a fully blocking config.

Otherwise I would need to go for P-channel and N-channel setup for the sense circuit for it to be able to completely disable the quiescent current draw.

[quote="b264, post:22, topic:85493"]
I think you should look at it from that perspective. What do we need that a regular BMS doesn’t provide?
[/quote]
Aren't the most used BMS' the bestech ones? I mean they are pretty purely hardware configured for a fixed series cell configs. I guess flexibility with one single BMS board in small package.
```

---
## \#26 Posted by: b264 Posted at: 2019-02-27T11:28:37.403Z Reads: 194

```
[quote="SimosMCmuffin, post:25, topic:85493"]
How is roll-to-start usually implemented? Motor controller senses wheel rotation and sends a command to e-switch to turn on?
[/quote]

Any two of the three motor phase leads are sent to the BMS, when they have an AC voltage on them, the BMS turns on.  Each time an AC voltage is registered, turn-off-time is set to one hour from right now, because it means the motor is turning.
```

---
## \#27 Posted by: SimosMCmuffin Posted at: 2019-02-27T11:58:45.865Z Reads: 194

```
[quote="b264, post:26, topic:85493"]
Any two of the three motor phase leads are sent to the BMS, when they have an AC voltage on them, the BMS turns on. Each time an AC voltage is registered, turn-off-time is set to one hour from right now, because it means the motor is turning.
[/quote]

Has this ever been implemented in a BMS? Pretty exotic to bring two motor phases to the BMS, just wiring wisem you'll have to split your motor connections before the motor controller. Maybe Mellow have done it, because their motor controller and BMS is on the same board, but I would still hazard a guess that the motor controller sends a signal to the BMS.
```

---
## \#28 Posted by: akhlut Posted at: 2019-02-27T12:14:38.712Z Reads: 182

```
Honestly, a can bus powered cell voltage monitor is what we need.  Roll your own BMS are great, but something that lets us monitor what a generic bms is doing is the missing link.  

Dont compete with china.  Find a nieche and exploit that, and right now thats a dead zone with only high cost options.  Nothing against them, but the number of people using d140 bms is at least an order of magnitude larger.
```

---
## \#29 Posted by: b264 Posted at: 2019-02-27T12:14:44.690Z Reads: 181

```
Lots of antispark do this.  Which is basically only because the BMS is incapable.
```

---
## \#30 Posted by: Klaerke91 Posted at: 2019-02-27T12:35:42.699Z Reads: 184

```
@JTAG is doing it via canbus. 

dont know how.

https://www.electric-skateboard.builders/t/diebiems-v0-8-2nd-batch-total-48pcs-closed/58327/289
```

---
## \#31 Posted by: SimosMCmuffin Posted at: 2019-02-27T12:49:58.353Z Reads: 183

```
[quote="Klaerke91, post:30, topic:85493"]
@JTAG is doing it via canbus.

dont know how.
[/quote]

To be specific I'm not sure the CAN comms are even needed, it just flips ENABLE signal on the BMS. Although he might be doing some extra comms on the CAN.

It's pretty much as I guessed in the first place. As the motor is spun up, it generates voltage on the ESC, which then wakes up. It then wakes-up the BMS and starts CAN communication.

So the motor powers the ESC long enough to inform the BMS to wake-up.

[quote="SimosMCmuffin, post:25, topic:85493"]
How is roll-to-start usually implemented? Motor controller senses wheel rotation and sends a command to e-switch to turn on?
[/quote]
```

---
## \#32 Posted by: JTAG Posted at: 2019-02-27T12:50:26.688Z Reads: 169

```
Push to start 😍😍 best thing I have ever done to my board.
```

---
## \#33 Posted by: SimosMCmuffin Posted at: 2019-02-27T12:51:48.247Z Reads: 160

```
Does the "EnableRequest" through the opto-isolator switch on the discharge path or do you also do some extra data on the CAN for that?
```

---
## \#34 Posted by: JTAG Posted at: 2019-02-27T12:55:58.421Z Reads: 168

```
No it is indeed just a turn on signal, its the 5V that is being created by the motor back emf ( by the buck converter in the esc), wasn't my idea ( someone in the thread came up with the idea ( don't remember who exactly but he / she deserves the credits ), I just tuned my power on state firmware for a better user experience ). 

There is no smart BMS implementation to the VESC yet, I am now tuning / making the charge and discharge throttling mechanism so it is hopefully not far away.
```

---
## \#35 Posted by: SimosMCmuffin Posted at: 2019-02-27T13:02:27.012Z Reads: 176

```
Any personal opinions on @b264 's proposed way to implement it?

[quote="b264, post:26, topic:85493"]
Any two of the three motor phase leads are sent to the BMS, when they have an AC voltage on them, the BMS turns on. Each time an AC voltage is registered, turn-off-time is set to one hour from right now, because it means the motor is turning.
[/quote]

IMO it's a bit redundant and silly wiring wise. Motor is already connected to the ESC, so just get a enable signal from that.

And either way this is a bit redundant topic for the Lite version, as it won't have disharge path mosfets integrated onto it. Why not just wire a 5V supply from the ESC to an independent e-switch in this case?
```

---
## \#36 Posted by: JTAG Posted at: 2019-02-27T14:23:27.248Z Reads: 171

```
So you are going to make this BMS charge only? Then there is also no need for push to start. And there are many ways to do push to start, the 5V BMS enable was just a very minimal effort implementation for mine, just a solder blob behind a connector if you are very lazy.

What are you going to do when someone drains the battery pasts its (most likely lower) limit? Because this will definitely happen :sweat_smile:. If you cant prevent lower limit discharge it is only half of a BMS :zipper_mouth_face:.
```

---
## \#37 Posted by: deucesdown Posted at: 2019-02-27T14:50:08.237Z Reads: 191

```
[quote="akhlut, post:28, topic:85493, full:true"]
Honestly, a can bus powered cell voltage monitor is what we need. Roll your own BMS are great, but something that lets us monitor what a generic bms is doing is the missing link.

Dont compete with china. Find a nieche and exploit that, and right now thats a dead zone with only high cost options. Nothing against them, but the number of people using d140 bms is at least an order of magnitude larger.
[/quote]

This right here. If you really think about what we want from charge only bms -- really think about it:

- 30q and other high quality 18650 tend to stay in balance
- charging to 100% (101.9% really with typical bms 4.25v cutoff) is not good for the cells
- most boards have ridiculous capacity, thus don't need to charge to 100%
- not charging to 100% means no balancing
- it's additional wear and tear to balance your cells on each charge via bms (for high cells overcharge slightly, then drain, repeat until low cells catch up)
- typical bms gives no indication what it's doing (is it balancing? which cell? is it stopping charge? what's it doing?? is it running correctly or broken?).
- it's a pain in the rocks to measure cell voltages once everything is installed

I think a more reasonable strategy is:
- bulk charge to 4.1v/cell
- have easy way to check voltage
- don't balance charge
- if when you check the cells are badly out of balance, take board apart to fix.
- if slightly out of balance to the point where bulk charging to 4.1v/cell is a bit scary, take pack out of board and fix the unbalance (probably tp4056 boards on low groups is the way to do this efficiently)

So yeah I'm with @akhlut. There are plenty of small charge-only 12s bms. There are no compact cell voltage monitors with indicators (display/bluetooth/canbus). And not many 13s bms.

But @SimosMCmuffin I love the project! Probably we're talking about a whole different thing. 

[quote="SimosMCmuffin, post:18, topic:85493"]
I’m planning on keeping the MCU always powered on via the LTC6803 5V regulator output dropped down to 3V3 via linear. This is a low power supply, about 4-6mA
[/quote]

A typical pack, 4p 30q, is 12ah. 12ah / .006a == 2000h. 2000h/24h == 83.3 days, which means we need a loud caution label, and cannot build the bms into the pack. Must be disconnected for medium to long term storage. Can you put a little switch on it?
```

---
## \#38 Posted by: JTAG Posted at: 2019-02-27T15:14:50.173Z Reads: 170

```
Not so sure about this.........
```

---
## \#39 Posted by: SimosMCmuffin Posted at: 2019-02-27T16:02:17.308Z Reads: 193

```
[quote="deucesdown, post:37, topic:85493"]
A typical pack, 4p 30q, is 12ah. 12ah / .006a == 2000h. 2000h/24h == 83.3 days, which means we need a loud caution label, and cannot build the bms into the pack. Must be disconnected for medium to long term storage. Can you put a little switch on it?
[/quote]

I meant that the LTC6803 5V regulated output can only supply a **max** of 4-6 mA, which means I can't really power anything hungry from it. The MCU in running state is around 1-6 mA (dependent on clock speed) and in low-power state needs only 10-200 µA (depending on sleep mode) and rest of the devices can be turned off by disabling the 5V buck SMPS.

![image|690x202](upload://3f5UREknW6zDH5PSxKy4YFzvtV3.png) 

[quote="deucesdown, post:37, topic:85493"]
So yeah I’m with @akhlut. There are plenty of small charge-only 12s bms. There are no compact cell voltage monitors with indicators (display/bluetooth/canbus). And not many 13s bms.
[/quote]
@akhlut 
Can you link to these BMS'? Something that supports CANbus? Has an actual battery management ICs and not just independent cell level logic gate discharge implementation?

[quote="deucesdown, post:37, topic:85493"]
I think a more reasonable strategy is:

* bulk charge to 4.1v/cell
* have easy way to check voltage
* don’t balance charge
* if when you check the cells are badly out of balance, take board apart to fix.
* if slightly out of balance to the point where bulk charging to 4.1v/cell is a bit scary, take pack out of board and fix the unbalance (probably tp4056 boards on low groups is the way to do this efficiently)
[/quote]
I don't think the layman user wants to keep checking on their battery to check if it's balanced and especially disassemble their board to get to the battery if it does need balancing...
```

---
## \#40 Posted by: deucesdown Posted at: 2019-02-27T16:20:16.614Z Reads: 179

```
[quote="SimosMCmuffin, post:39, topic:85493"]
keep checking on their battery to check if it’s balanced
[/quote]

Anything else is blind faith.

I know we're getting off-topic so I'll try to shut up :slight_smile:
```

---
## \#41 Posted by: amazingdave Posted at: 2019-02-27T16:22:04.283Z Reads: 165

```
This is great. For my money I want small, charge only, canbus for metr connection and user configurable charge termination/ balance. Balancing is a must.....

No faith needed with can and metr.
```

---
## \#42 Posted by: SimosMCmuffin Posted at: 2019-02-27T16:25:37.833Z Reads: 165

```
[quote="amazingdave, post:41, topic:85493"]
This is great. For my money I want small, **discharge only**, canbus for metr connection and user configurable charge termination/ balance. Balancing is a must…
[/quote]

Did you mean _charge only_??
```

---
## \#43 Posted by: amazingdave Posted at: 2019-02-27T16:28:13.631Z Reads: 158

```
I did....

10
```

---
## \#44 Posted by: Friskies Posted at: 2019-02-27T16:28:44.770Z Reads: 160

```
I don't know anybody that wants to take their pack apart and charge everything manually. It pretty much defeats the purpose of having a BMS?????
```

---
## \#45 Posted by: SimosMCmuffin Posted at: 2019-02-27T16:31:41.500Z Reads: 177

```
@amazingdave @deucesdown @akhlut
Talking about Metr  

[quote="amazingdave, post:41, topic:85493"]
canbus for metr connection
[/quote]

[quote="deucesdown, post:37, topic:85493"]
There are no compact cell voltage monitors with indicators (display/bluetooth/canbus).
[/quote]

[quote="akhlut, post:28, topic:85493"]
Honestly, a can bus powered cell voltage monitor is what we need.
[/quote]

https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/1

Is the Canbus meant to connect the BMS to the VESC/derivative and then from there with USART to Metr and then over bluetooth for status monitoring on your phone?
```

---
## \#46 Posted by: Pimousse Posted at: 2019-02-27T16:46:33.994Z Reads: 162

```
Yes.
Metr Pro issues command to DieBieMS through CANbus (Bluetooth to Metr Pro -> UART to VESC -> CAN to DBMS).
If you design commands the way as this is coded into DBMS, it would be compativle straight forward with Metr Pro (I assume).
```

---
## \#47 Posted by: akhlut Posted at: 2019-02-27T16:52:10.607Z Reads: 163

```
The DieBieMS for one.  It's great, but spendy, large and not readily available.

there are a crop of smart BMS from China.  I've seen a few that have cell monitoring but can't remember the names.
```

---
## \#48 Posted by: Pedrodemio Posted at: 2019-02-27T16:55:53.476Z Reads: 172

```
Nice to hear back from you @SimosMCmuffin

* One more vote for keeping CAN if integration with Metr is to happen, also since it's charge only, you can use software to cut power to the motors instead of cutting power to all electronics

* Current sensing module I think it's not needed, VESC already do it, and with the new firmware it's even more integrated when using multiple VESC's, the downside is that charging current is not monitored, if you want the BMS to now discharge current and energy used is just a matter of requesting the VESC data via CAN

* about the full blocking, how does it work? is there any way to make the charge port live when the board is turned on? or at least make it configurable by a jumper or something? I see a lot of uses for using the board as a portable battery, such as powering a computer and etc

* size, most compact charge low current BMS's are 60x30mm, if possible this would be the perfect size

And put me up from one, I have space reserved for it since your last iteration
```

---
## \#49 Posted by: deucesdown Posted at: 2019-02-27T17:15:32.729Z Reads: 155

```
[quote="Friskies, post:44, topic:85493"]
take their pack apart and charge everything manually
[/quote]

999 out of 1000 times you just bulk charge as normal, but to 90% not 100%. The telemetry would let you know this is safe. "know" is the key concept. Just because you have BMS installed, do you think your pack is perfectly healthy? Does the BMS let you know if something is amiss? Do you just assume it is?
```

---
## \#50 Posted by: amazingdave Posted at: 2019-02-27T17:17:47.535Z Reads: 144

```
If I can see the p groups in metr I’m going to be happy for a month between inspections...
```

---
## \#51 Posted by: SimosMCmuffin Posted at: 2019-02-27T17:24:23.601Z Reads: 162

```
[quote="Pedrodemio, post:48, topic:85493"]
the downside is that charging current is not monitored
[/quote]

The INA180 is used to monitor charging current. Protection from overcurrent and allows setting cut-off current at the end of charge.

[quote="Pedrodemio, post:48, topic:85493"]
about the full blocking, how does it work? is there any way to make the charge port live when the board is turned on?
[/quote]

This is a fully blocking switch setup. in this case it's 2 N-channel mosfets either in common-drain or common-source configuration.

Here's an equivalent circuit with switches with a "body diode" instead of mosfets, but take one away and your switch can only stop the flow of current in one direction.
![image|690x270](upload://581BQ8vixv4pVnXPKzufbDmyQfE.png) 
![image|690x246](upload://ve2SwGaYNsQkpcmzD4cob4Hk8K5.png)

It can be opened up through firmware, but how to communicate that to the BMS when to do it, is the real question.
```

---
## \#52 Posted by: SimosMCmuffin Posted at: 2019-02-27T17:32:06.969Z Reads: 151

```
Ooh, just found an interesting IC for power saving use:

![image|690x283](upload://tfO0kPRiLUChROZDvbmQ1tYw3bd.png) 

http://www.ti.com/lit/ds/symlink/tpl5010.pdf

Gonna dig through this datasheet....
```

---
## \#53 Posted by: Pedrodemio Posted at: 2019-02-27T17:46:08.842Z Reads: 148

```
Understood, if you were integrating a switch it should be easy, something like hold the button for 10 seconds

And about the current drain, give the drama from the past week about switches drawing to much current when idle, in my opinion in no way a switch or BMS should be able to to kill a board if left connected in a reasonable amount of time

Isn't any way to make the BMS only active when charging and when the board is on? Such as connecting it after the main switch and using a transistor to turn it on?

Lets say for example a 300 Wh battery left with 20% charge should no be dead after 6 months
```

---
## \#54 Posted by: SimosMCmuffin Posted at: 2019-02-27T18:16:45.748Z Reads: 159

```
IMO the solution is to maximize sleep states when not charging to minimize quiescent draw. On the other hand you need to have something active to check every now and then if any comms or if a charger is detected or enable signal from ESC is detected.

The first BMS' problem to the quiescent current were all the resistive voltage dividers, which pulled multiple hundred microAmps from the battery regardless if the MCU was even soldered onto the board. That's why I'm a bit hesitant to change the charging mosfets away from the fully blocking setup. IMO better idea to allow for the roll-to-start function to signal that system is active and then open the charging switches so, if somebody wants voltage from the battery on the charger plug then it can be activated with the roll-to-start. (EDIT: Or just ESC normally powered up)

I personally would prefer to not put any buttons on the BMS, because some people essentially integrate the BMS into their pack by wrapping the whole thing up.

ST's L-series MCUs can go into reaaaaaally low-power states (attached some datasheet tables from current consumption from normal run states to the deep low-power states)

![image|690x460](upload://fQMOLtEmhTfpJlrGxf6qJQ7gh7h.png) 
![image|690x473](upload://186LmZUVWf5nIEphGDdz1yupcNJ.png)
```

---
## \#55 Posted by: Pedrodemio Posted at: 2019-02-27T18:22:04.508Z Reads: 134

```
The micro controller yes, but what about the voltage regulator that powers it? genuinely asking
```

---
## \#56 Posted by: Friskies Posted at: 2019-02-27T18:23:01.829Z Reads: 131

```
Thats not a battery management system. Its a battery monitor.
```

---
## \#57 Posted by: SimosMCmuffin Posted at: 2019-02-27T18:41:07.413Z Reads: 152

```
When a battery is connected to the BMS the LTC6803 is powered but stays on standby mode until SPI communication happens. The IC has a linear 5V voltage regulator output. So if it's loaded 2 mA, it should pull 2 mA from the battery. This is then passed through 3V3 linear regulator to power the MCU.

EDIT: So if the MCU is in low-power state with few ten microAmps of current use, that's how much should be pulled from the battery + LTC6803's standby current.

![image|441x348](upload://lLyRr6qlODVQ7Mp6kUDn0vWMN3u.png) 

![image|421x213](upload://uuSgeX7do5PPOo0Qdd43A5W2ipF.png) 

![image|550x278](upload://2jA3kjle1fywn5HjkWW2DfEjSdZ.png) 

(LTC6803-3 datasheet)
https://www.analog.com/media/en/technical-documentation/data-sheets/680313fa.pdf
![image|519x500](upload://ffC7fJ0FCCOrshlg5ax8XpS6Lyx.png)
```

---
## \#58 Posted by: haand22 Posted at: 2019-02-27T18:47:26.396Z Reads: 141

```
Awesome bms! Would definitely buy one once available. However, I would really want to see them with a better connector. Something graded for automotive industry or similar.
```

---
## \#59 Posted by: Friskies Posted at: 2019-02-27T18:48:43.417Z Reads: 144

```
Do you actually even want roll to start on a charge only BMS though?
```

---
## \#60 Posted by: Surfer Posted at: 2019-02-27T18:56:59.122Z Reads: 150

```
Yeah I will love it, and auto switch off included, no more power switch.
 My 2 cents:
Small footprint
At least up to 12s 
Charge only
Cell monitoring
CAN communication with metr.app
Push to start/ adjustable auto switch off.
Good quality components and a beer or two for the creator.
No need to be too cheap, this hobby has so many options to go in a cheap way.
That's all I want, and I will be very very happy.
```

---
## \#61 Posted by: SimosMCmuffin Posted at: 2019-02-27T19:09:46.516Z Reads: 147

```
[quote="haand22, post:58, topic:85493"]
However, I would really want to see them with a better connector.
[/quote]

Do you have any proposals? Mooost likely it's not going to fit onto the board, but I'll look through your proposals.
```

---
## \#62 Posted by: SimosMCmuffin Posted at: 2019-02-27T19:20:50.959Z Reads: 154

```
I just checked the pin out on the MCU and I can get USART_TX/RX and I2C_SDA/SCL from the same pins, so I can connect them both to the 4 pin header and switch between them in firmware. You can then config the pins to use the I2C interface and connect one these cheapie OLED screen onto it, it can be then used to monitor the cell voltages directly.

![image|427x381](upload://yJ8Ccajy7ydm6DTBEY9577m1i4k.jpeg) 
https://www.aliexpress.com/item/0-91-Inch-128x32-IIC-I2C-White-Blue-OLED-LCD-Display-DIY-Module-SSD1306-Driver-IC/32879702750.html
```

---
## \#63 Posted by: SimosMCmuffin Posted at: 2019-03-01T09:50:59.795Z Reads: 146

```
**Off-topic**
Something interesting happened last night. Got a whatsapp message from my old employer/customer asking how much would my monthly salary have to be for me to come to do R&D for them... I scheduled a meet for coffee tomorrow to talk things through about this. Maybe I can leverage for a raise with this.

I'm just really surprised, did not expect this.
```

---
## \#64 Posted by: SimosMCmuffin Posted at: 2019-03-01T17:13:21.351Z Reads: 145

```
**Update.**
Board is routed, but I'm not ordering the PCBs yet, I need to sanity check the schematic side for anything obvious. I'm also gonna experiment with changing the layout to find something a bit more optimal, but I'm taking a snapshot of the current layout in case I can't successfully optimize it, so I can at least order the first boards at the change of the week.

Would have updated some smexy raytraced 3D-renders, but it appears that the forum's server has ran out of space for images :sweat_smile: . I'll add them later to this post when the issue resolved (assuming it's soon).

> No space left on device @ io_write - /var/www/discourse/public/uploads/db1493/original/3X/7/0/70ee714019eea3c91e0ac9ae0b24b97061d4e118.jpeg

**EDIT:**
**We got Pics!!**
[url=https://ibb.co/KbkbXgW][img]https://i.ibb.co/ZGPGVrx/image.png[/img][/url]
[url=https://ibb.co/1rByf4W][img]https://i.ibb.co/jyq0vjX/image.png[/img][/url]
```

---
## \#65 Posted by: banjaxxed Posted at: 2019-03-01T18:25:47.367Z Reads: 143

```
[quote="SimosMCmuffin, post:20, topic:85493"]
Isn’t 13S a bit exotic?
[/quote]

Since @Deckoz popularized it, there has been a few builds for sure, I’ve one in the works that this design would have been perfect for 👍
```

---
## \#66 Posted by: haand22 Posted at: 2019-03-01T21:52:45.551Z Reads: 146

```
One could use something like this:
https://www.alibaba.com/product-detail/High-Quality-IP68-Circular-Waterproof-Male_1987076125.html
I don't know. I'm just not a fan of these sketchy pin-connectors that may come loose at any time. An other solution is just to leave some holes for the cables to be soldered into.
```

---
## \#67 Posted by: SimosMCmuffin Posted at: 2019-03-01T22:12:26.239Z Reads: 145

```
That is a inline wire connector, not a board header.

JST's XH-series is pretty good connector for it's size and price. It has detent locking, so unless it's pulled away from the connector, I don't see the probability of it coming loose likely.
http://www.jst-mfg.com/product/pdf/eng/eXH.pdf

I'm planning on ordering the boards without any through hole components, which would be the wire connectors. People can then specify when they order, what connectors they want pre-soldered. If you don't want to use that particular connector, then you can solder your own wires onto the board and crimp your own connectors.
```

---
## \#68 Posted by: Pedrodemio Posted at: 2019-03-02T04:09:39.247Z Reads: 138

```
Looking good, what are the dimensions so far? Excluding the connectors
```

---
## \#69 Posted by: SimosMCmuffin Posted at: 2019-03-02T08:58:07.156Z Reads: 143

```
62,5 x 26,5 mm

[url=https://ibb.co/0CFsKsb][img]https://i.ibb.co/D98rYr2/image.png[/img][/url]
```

---
## \#70 Posted by: Pedrodemio Posted at: 2019-03-02T14:58:31.838Z Reads: 137

```
Perfect

A suggestion, use a vertical mounted USB connector, most board won’t be able to reach it once installed as it is
```

---
## \#71 Posted by: SimosMCmuffin Posted at: 2019-03-02T17:55:20.614Z Reads: 139

```
I might do the same move as with the earlier board. Make it possible to mount either one.
```

---
## \#72 Posted by: Arek Posted at: 2019-03-02T19:41:21.530Z Reads: 139

```
I really wish you would work with @deodand and make lite version alarm Unity through CAM about cell/pack low voltage and first enable limited power mode and when voltages are critically low complete shutdown of Unity.
This would let us use all the current pack can output and at the same time do it safely.
```

---
## \#73 Posted by: SimosMCmuffin Posted at: 2019-03-03T09:41:31.795Z Reads: 139

```
I don't see why that couldn't be made reality. Mainly it's just getting both parties to agree on the messaging protocol and then implementing it.

Or if one party has already implemented the messaging protocol, then it will be just making sure your device conforms to it.
```

---
## \#74 Posted by: Darkie02 Posted at: 2019-03-03T10:20:31.469Z Reads: 142

```
As the layman am I right in thinking the features each the vershion will have

FlexBMS Light 
Seprat cell voltage monitoring,
CANbus,
Active cell balancing in use.

FlexBMS Basic
Same as light +
Discharge protection

I’m sure things have been mentioned that have just gone over my head that I missed will try to work out what thay are. but looks as tho it be very popular for a lot of diy builds


Im on the side of defiantly want CAN with it linking to Metr pro app to see cell voltage. Been able to set min cell voltage cut off instead of a overall battery pack min. Is this some thing that could be set by consumer later or would it have to be pre set in manufacturing?

Not sure how the screen links in to it is that throu canbus as well?
```

---
## \#75 Posted by: SimosMCmuffin Posted at: 2019-03-03T12:35:30.734Z Reads: 144

```
Here's a rendering with both horizontal and vertical connectors. They can be soldered in any configuration, so you can optimize your connector orientation for your use environment.

[url=https://ibb.co/Q95s6jy][img]https://i.ibb.co/kKdYh6N/image.png[/img][/url]

[quote="Darkie02, post:74, topic:85493"]
Im on the side of defiantly want CAN with it linking to Metr pro app to see cell voltage. Been able to set min cell voltage cut off instead of a overall battery pack min. Is this some thing that could be set by consumer later or would it have to be pre set in manufacturing?
[/quote]
CAN is confirmed, USART/I2C is confirmed and a opto-isolated enable signal is confirmed.
I plan on first making a simple configuration interface via the USB and Serial terminal for the relevant charging and fault limits. Then in the future maybe try to integrate the configuration onto the VESC tool or metr app.
```

---
## \#76 Posted by: SimosMCmuffin Posted at: 2019-03-03T18:12:14.081Z Reads: 143

```
Deadline is approaching and @ducktaperules offered an extra set of eyes to check the schematic and layout. 0.1 HW files are at the moment ready-to-order and I'm just waiting for the green light from him. 

[url=https://ibb.co/fv9rxLM][img]https://i.ibb.co/VmxMq5V/image.png[/img][/url]
[url=https://ibb.co/BnPNqmG][img]https://i.ibb.co/hYMfDkc/image.png[/img][/url]
```

---
## \#77 Posted by: SimosMCmuffin Posted at: 2019-03-03T20:04:39.935Z Reads: 138

```
Boards have been ordered.

I'm gonna clean up the BOM and order the parts meanwhile. Maybe I'll comment about the component costs and quoted assembly costs once I get the shopping cart sorted.
```

---
## \#78 Posted by: pjotr47 Posted at: 2019-03-03T21:38:29.631Z Reads: 137

```
Nic! Keep the good work. The thing about unity and communication between bms would be awesome.
```

---
## \#79 Posted by: SimosMCmuffin Posted at: 2019-03-04T14:52:23.428Z Reads: 141

```
Here's a pie chart of how the component cost is spread between the component categories in case anyone is interested.

![image|686x500](upload://73qO70aeriDquZwBQWnU5Gc6iit.png)
```

---
## \#80 Posted by: Gerrycorrado Posted at: 2019-03-04T15:06:03.720Z Reads: 138

```
Bla bla bla bla
We only want to know: did you get a raise?!
```

---
## \#81 Posted by: SimosMCmuffin Posted at: 2019-03-04T16:29:48.161Z Reads: 138

```
[quote="Gerrycorrado, post:80, topic:85493, full:true"]
Bla bla bla bla We only want to know: did you get a raise?!
[/quote]

Not yet. Had some coffee with the old colleague and talked about more normal and mundane stuff first recent events on both of our ends. They are currently looking for investors and they had asked how much a HW oriented employee would cost in a year. He then told me that he proceeded to send me that whatsapp message right after that, which would partially explain that the message came at 10 in the evening. Told me that he had been working a "little" longer days recently.

Anywhoo, I told my current wages and fringe benefits and said that was the baseline to go higher from. They had been developing and manufacturing consumer level desktop printers before, but they are moving now onto more industrial printing applications. They currently have an industrial robot arm with a printhead and they are developing their own software and hardware solutions around that (He had a picture of him riding said arm). I said that I was interested in coming back to them after hearing all this.

No dates were set in stone, but within the next half a year, depending on when they can secure more funding. I said I was going to inform my current employee as well of the developments and we agreed to keep in touch.

**TLDR**

Pre-emptive move to contact me, so they can give a better cost prediction for investors about how much I would cost annually. "Putting the gears in motion", so to speak.
```

---
## \#82 Posted by: Arek Posted at: 2019-03-04T21:37:32.318Z Reads: 134

```
Nice layout!
Took a look myself and I can't find any issues, at least any major.
Don't like how R12's pad is merged with B- pad, you'll get it bridged with soldered cable and any forces applied to it will stress that resistor and could cause it to crack.

Also if Q1+Q2 will be getting too toasty you can remove those thermal reliefs in the next HW revision and get some heat sinked into the massive pads and cables.
```

---
## \#83 Posted by: Darkie02 Posted at: 2019-03-05T08:31:59.466Z Reads: 138

```
Had a couple of ideas for you to consider. I’m not experienced in designing or making PCB so thay might be a useless thoughts that you might have good reasons to dismiss. I really like the press for terminals on the batt + - expensive for what thay are but a nice finish and easy to to remove large cables later with out over heating the board. ![image|464x500](upload://bBBzudw02ZFDmZb89V0Y0VNkWgH.jpeg) https://image.made-in-china.com/44f3j00ZUlEnaRBAwky/Press-Fit-Power-Clamps-Flexible-or-Elastic-Press-Fit-Technology.jpg

Tho I don’t know how useful it be on the light version as it’s not carrying the power to the VESC you wouldn’t need 10awg cable.

Also thinking how much room in a encloser the plugs would need each side could one be spun around after if you wanted all the cables to come off one side? This is a really tiny BMS so compacked mabe it just looks as tho the the cables coming off would use up more room than the board it’s self and in reality it’s not worth even considering. 

It’s looking as tho it’s becoming a reality parity quick when might you be taking pre orders? (APS BMS Just dies on me after 4 months so need to decide what to do about replacing it)
```

---
## \#84 Posted by: SimosMCmuffin Posted at: 2019-03-05T11:13:45.529Z Reads: 138

```
[quote="Darkie02, post:83, topic:85493"]
I really like the press for terminals on the batt + - expensive for what thay are but a nice finish and easy to to remove large cables later with out over heating the board.
[/quote]

[quote="Darkie02, post:83, topic:85493"]
Tho I don’t know how useful it be on the light version as it’s not carrying the power to the VESC you wouldn’t need 10awg cable.
[/quote]

Lite version is not going to have these, due to only having charge path control (no crazy currents). Basic version is shaping up to be board size wise bigger and with discharge path control comes the need to think about the wire connections. Good point bringing up the heat stress if you need to solder heavy gauge wire directly onto a solder pad.

I have looked earlier at  Wurth electronics' "REDCUBE WP" series screw terminals (the same ones as in the picture above) at Digi-Key, link below to the connectors.

https://www.digikey.fi/products/en/connectors-interconnects/terminals-screw-connectors/396?k=&pkeyword=&sv=0&s=56728&s=56729&s=56718&s=56719&s=56720&s=56721&s=56722&s=56723&s=56724&s=56725&s=56726&s=56727&sf=0&FV=1f140000%2Cffe0018c&quantity=&ColumnSort=0&page=1&stock=1&pageSize=25

[quote="Darkie02, post:83, topic:85493"]
It’s looking as tho it’s becoming a reality parity quick when might you be taking pre orders? (APS BMS Just dies on me after 4 months so need to decide what to do about replacing it)
[/quote]

I'm going to be pushing this project forward with a lot of effort. Priority on getting the board's basic functionality going and being able to configure the critical parameter's for charging use. _No one wants a non-functional paper weight_. And is a very bad idea to start shipping product if this is the FW state.

I'm focusing atm on making a basic bootloader that allows to flash the firmware through the USB connection alone, while still keeping the implementation simple. This way, as more software features get implemented and fixed you can easily upgrade to the latest firmware. This is one of the biggest priorities for me.

Once hardware gets mature enough to be considered shippable. I'm going first do a small 8-10 board assembly test batch to see how the PCBA workshop performs and iron out any manufacturing file deficiencies. I'm currently looking at a few china workshops like:  
https://www.pcbway.com/Home/Index?code=f   
and   
https://www.seeedstudio.com/fusion_pcb.html (I have ordered PCBs from here before)

With more options from this list:  
https://www.eevblog.com/wiki/index.php?title=PCB_Assemblers#China_Based

If anybody has anybody has any experience working with Chinese PCBA workshops, I'm all ears.
```

---
## \#85 Posted by: Surfer Posted at: 2019-03-05T11:26:24.998Z Reads: 128

```
@Samau18  
10 skirrels
```

---
## \#86 Posted by: Samau18 Posted at: 2019-03-05T14:42:02.096Z Reads: 131

```
Can certainly take a look when the board is ready.  My only request is that there will be automatic testing tools to go with it =]. 

Sam
```

---
## \#87 Posted by: SimosMCmuffin Posted at: 2019-03-05T20:15:07.058Z Reads: 139

```
Here's the planned bootloader flow chart, that I know I can implement in a timely fashion.
![image|690x438](upload://fqhaTdgYjzFlZwRUdpPnLsthjQW.png)
```

---
## \#88 Posted by: Arek Posted at: 2019-03-05T20:46:20.249Z Reads: 138

```
[quote="Samau18, post:86, topic:85493"]
there will be automatic testing tools to go with it
[/quote]

The least fun part of designing a product :smiley:
```

---
## \#89 Posted by: SimosMCmuffin Posted at: 2019-03-06T07:24:23.100Z Reads: 136

```
Do you own your own PCBA assembly line or did you order the DieBieMS boards assembled from somewhere else?
```

---
## \#90 Posted by: Samau18 Posted at: 2019-03-06T07:36:47.313Z Reads: 139

```
We order parts, sent them off to be SMT-ed by SMT house (We can do it in house with our Juki too, but not very cost effectively at the current bms quantities)

Manual installing items (press-in connector, fuse) and testing are done in house.
```

---
## \#91 Posted by: SimosMCmuffin Posted at: 2019-03-11T16:32:52.327Z Reads: 142

```
Boards and components came today. Gonna start assembling today in sections and testing that everything is looking good.

![IMAG0182|690x200](upload://2L7nprKCcXh9j00m808bAshvTAS.jpeg) 
![IMAG0183|690x389](upload://9jHuPJJaxJ2V8vEB4S9JTY08SRt.jpeg)
```

---
## \#92 Posted by: Pedrodemio Posted at: 2019-03-13T04:56:29.991Z Reads: 140

```
@SimosMCmuffin and had an idea that maybe more people find useful 

Is possible to have a pin supply 5v when the board is charging? I would use it to power my arduino without actually powering the board on and use my battery charge leds indicate that the board is indeed being charged, something similar how boosted does
```

---
## \#93 Posted by: SimosMCmuffin Posted at: 2019-03-13T18:55:57.177Z Reads: 141

```
[quote="Pedrodemio, post:92, topic:85493"]
Is possible to have a pin supply 5v when the board is charging?
[/quote]
Unfortunately, no 5V is readily available off the board. 3V3 is available from the USART/I2C connector, which arduino can be run from, but can't say if your other devices with the arduino will be able to run from it.

Do note, that the max current from the 5V buck is 300 mA absolute maximum (datasheet), minus what is already being used by the BMS components.

If you reaally need 5V, then probably the easiest place to get it from would be the either to solder a jump wire to the capacitor next to the CAN transreceiver and a dab of hot glue to give the wire some mechanical support.
![image|675x500](upload://kPKa4x1GQ0grmiZ0m8x5Ay9n4ME.jpeg) 
Or straight onto the 5V buck controllers inductor output side, or output capacitor.
![image|548x499](upload://s3zE472bKiBmu7a2j706cRGpetp.png) 

I'll see if I can add an open pad somewhere for the 5V, so users can more easily get the 5V out of the BMS.

---

**Progress on the board assembly and testing**

I've been busy testing the voltage regulation and current consumption on the board from the 5V buck and through the LTC6803's linear regulator. MCU is alive and I've been doing some low power mode testing. I want to test and confirm the current consumption for the MCU, so I haven't assembled the rest of the board yet, meaning I can isolate all the power draw to the 5V buck or the MCU.

Started from around 3.3 mA on the basic settings with USB turned on with a couple of the internal oscillators going. Disabled the USB and it's oscillator and turned the main oscillator from 16MHz down to 100kHz. Went into lower internal voltage regulator mode and then went into low-power-run mode. 

After this my multimeter showed around 150 µA, but I don't know how accurate it is at very low currents. I also noticed that the 3V3 linear regulator for the MCU has a quiescent current of 150 µA at zero output current, sooo the current consumption mighty be largely, because of that at the moment (Graph from it's datasheet below). I have already found a drop-in replacement regulator, with 5µA spec'd quiescent current. 

![image|675x500](upload://519ejgqisRCotzACTW3lpqEuGID.png) 

I'm gonna do more current measurements tomorrow at work with better equipment.

So in that line I have already found a couple HW related things I want to change around, but nothing major so far.

![IMAG0186|690x284](upload://3NLiJ1CMF8PCuhwz69mbnzWJ112.jpeg) 
![IMAG0188|690x241](upload://ln4sbc8Wqn9WADvjtgB3l37E4aW.jpeg)
```

---
## \#94 Posted by: Pedrodemio Posted at: 2019-03-13T19:43:34.102Z Reads: 138

```
Thanks, or alternatively, pads to drive some leds directly would also work, I have and SOC "algorithm" that I use on the Arduíno that could merge with the firmware if you have interest, i don't know if you have pins remaining on the micro controller
```

---
## \#95 Posted by: SimosMCmuffin Posted at: 2019-03-14T07:35:35.851Z Reads: 141

```
Is there a reason you couldn't interface via USART or I2C?

---

Here's a pic me (or my hands at least) testing the current consumption in my workplace's lab. Current hovered around 145 µA and the lab multimeter used was Keysight 34461A. I'm quite surprised how close my 20 dollar chinese multimeter (an8008, approved by Dave from eevblog) showed to this amount. I'll see if I can add the better suited linear reg to our HW team digi-key order list, I don't personally see any big enough orders in the near days to make the order myself (free shipping after 50€ items). So far the current consumption seems pretty promising, but I'll  say for certain after I get to test the new linear reg.

![IMAG0190|338x500](upload://2mYUu4EARKUAMnmcBGt5kHgjGbE.jpeg)
```

---
## \#96 Posted by: Pedrodemio Posted at: 2019-03-14T12:26:18.467Z Reads: 137

```
[quote="SimosMCmuffin, post:95, topic:85493"]
Is there a reason you couldn’t interface via USART or I2C?
[/quote]

It’s possible, I don’t even need any the data of the BMS, just a way to power the board or just the logic part when the charger is plugged 

Thanks
```

---
## \#97 Posted by: SimosMCmuffin Posted at: 2019-03-18T18:37:00.093Z Reads: 145

```
Started assembling and testing the sense and balance circuitry on the weekend. 

Discovered some weird behavior on the cell voltage measurements on Sunday. Otherwise cell voltages were okay, but the top most cell was always 40-70 mV under actual amount and was fluctuating slightly, where as all the other cell voltages were rock-solid and on point. I tested with 3, 4, 5, and 6S batteries and it was always the top cell measurement that exhibited this behavior. Due to the problem always persisting with the top cell and all lower cells showing correct numbers, this lead me to believe the sense circuitry itself was okay, but there is something weird going on the supply side on the LTC6803. 

Tried isolating the MCU's 3V3 supply, which seemed to fix the problem. Meaning there is something funky going on with the 6803's 5VREG output while USB is connected. Problem seemed to get fixed by placing a diode on the 5VREG line between the MCU 3V3 linear regulator. USB comms showed correct and steady results for the top most cell measurement after that. Board now officially has it's first hot bodge component placement as pictured below  (had to scrape off soldermask and cut a trace and then solder the diode inline onto the naked trace :wink:)

I still want to check the measurement results without the USB connected by passing the cell measurement results through an Arduino via USART.

Once I have results from that, then I'll start testing the actual balancing. Mainly interested in the thermal behavior, currently current bleed resistors are 33 Ohm, as can be seen on the lower picture. At 4.15V this should give ~125 mA balance current.

**Note**

I believe I'll be able to get the standby current use below 100µA, but I still don't have the better suited linear regulator on hand yet, so I can't affirm it 100%. In theory this should give for example a 1 Ah (very small) battery a storage life of ~400 days, or 2.4 mAh daily.


![IMAG0192|690x452](upload://8S8pf2Th6BjLQtVl2QPL7m1wVE8.jpeg) 

![IMAG0193|579x500](upload://2d1yTmXRbMK3qUl6rjyg5EfkBjL.jpeg) 

---

**Off-topic**

Assembled this thing also on the weekend (battery not yet soldered in). Kudos to @MasterCho for Thingiverse files and @Smorto (https://www.electric-skateboard.builders/t/gt2b-mastercho-chozen-mod-full-length-tutorial-how-to/16005?u=simosmcmuffin) and  @Mikenopolis (https://www.electric-skateboard.builders/t/gt2b-mod-video-tutorial-chozen-remote-case/37668?u=simosmcmuffin) 
![IMAG0194|690x447](upload://5nYy6g0eYiYqQi4IYcIhLMiTlhU.jpeg)


---
**EDIT:**

Also, experimented with the super low-power modes on the MCU and did a beginner's error. Put the MCU in stop mode 2, which stops the CPU clock. 

Have a guess, if I could get my ST-LINK to connect to it after that? No. Problem really was that I don't have RESET broken out to a test pad, because normally you can call software system reset with just the SWCLK and SWDIO, but guess if that still works when the CPU is internally stopped in a low-power stop mode? Nah. So every time the MCU booted up it directly ran itself to stop mode in couple milliseconds. Not really enough time to start debugging run from the ST-LINK and flash a new firmware to it :smile::sweat_smile: . 

Fun. Times. 

In the end I solved the problem by soldering a sneaky hook-up wire directly onto the QFN package's 
RESET pin pad (which doesn't extend out anywhere from below the package). Well got it done. Got reset working so I could get the debugging session started and flash a new firmware. Didn't even have RTC running the auto wake-up in the background, so it really was a sleeping beauty at that point. Even considered desoldering the whole MCU and just plonking down a new one.

Well, you learn best from these kinds of mistakes...
```

---
## \#98 Posted by: Pedrodemio Posted at: 2019-03-18T18:50:52.123Z Reads: 138

```
Good progress

I think your best bet with cell balancing is to limit how many cells should be allowed to balance simultaneously with a temp sensor near the resistors should it get too hot in a extreme situation
```

---
## \#99 Posted by: rpasichnyk Posted at: 2019-03-18T20:37:28.156Z Reads: 131

```
It was interesting to read about developments :nerd_face: Thanks for documenting!
```

---
## \#100 Posted by: ducktaperules Posted at: 2019-03-19T14:17:39.056Z Reads: 129

```
[quote="ducktaperules"]
you haven’t broken out the reset pin
[/quote]

[quote="SimosMCmuffin"]
I do believe you only need Reset if you map the pins to GPIO. My earlier board was running debugging fine with only SWCLK and SWDIO.
[/quote]

I always try and breakout these sorts of pins to a test pad even if you dont think you will need them just for situations like this. 

Otherwise the boards look great. Did you solder them by hand or did you reflow them? they look very tidy.

To be honest if adding 1 diode is the only change you need to make then that's pretty good going. Cant wait to see further progress with this. Also Im surprised by just how small the board looks in your photos. Cant wait to have one of these in my board :smile:
```

---
## \#101 Posted by: SimosMCmuffin Posted at: 2019-03-19T17:18:53.719Z Reads: 133

```
Here is a FLIR video of the first balancing action. Charging a 6S battery with all the lower 5 cells crossing over balancing voltage, which in this case was 4,160 V. It's running too hot for my taste, especially under continuous balancing, which is compounded if the cells that need balancing are all next to each other. I can use the internal temperature measurements of the LTC6803 and MCU to determine the board temperature on a rough scale.

https://youtu.be/dpaqirpvOUk

![Screenshot_20190319-185628|281x500](upload://fJx6i1qKMg5j2mJZdd04R4QZQ3O.jpeg) 

Recorded on a FLIR ONE (first gen, not available anymore) a very worth it purchase for debugging and troubleshooting electronics and anything thermal related.
![IMAG0195|690x386](upload://vbiNaPd3Wbnj6WkqLWktGfHUBJc.jpeg)
```

---
## \#102 Posted by: Darkie02 Posted at: 2019-03-20T09:06:46.444Z Reads: 129

```
As long as the board is not thicker than a 18650 battery it wouldn’t affect any one is it possible to add a heat sink or drop it in to a mettle case as a upgrade so it would never become a limiting factor? Having a case mounted heatsink is some thing I do check if any things not feeling right just put my hand on it and it gives a piece of mined I’m not frying my foxbox on a long hill.
```

---
## \#103 Posted by: Pimousse Posted at: 2019-03-20T10:03:55.474Z Reads: 125

```
Again, I love your R&D approach. Nothing's left random.

[quote="ducktaperules, post:100, topic:85493"]
To be honest if adding 1 diode is the only change you need to make then that’s pretty good going.
[/quote]
I second that ! Nice job !
```

---
## \#104 Posted by: SimosMCmuffin Posted at: 2019-03-20T15:03:17.274Z Reads: 128

```
[quote="ducktaperules, post:100, topic:85493"]
Otherwise the boards look great. Did you solder them by hand or did you reflow them? they look very tidy.
[/quote]

Hand soldering. Hot air reflow station and soldering iron if needed.

[quote="Pimousse, post:103, topic:85493"]
Again, I love your R&amp;D approach. Nothing’s left random.
[/quote]

Gotta test to know.

[quote="Darkie02, post:102, topic:85493, full:true"]
As long as the board is not thicker than a 18650 battery it wouldn’t affect any one is it possible to add a heat sink or drop it in to a mettle case as a upgrade so it would never become a limiting factor? Having a case mounted heatsink is some thing I do check if any things not feeling right just put my hand on it and it gives a piece of mined I’m not frying my foxbox on a long hill.
[/quote]

It's a possibility, but IMO a pain in the ass (had a heatsink on the first one). I'll rather just go for lower balancing current, which lowers the heat generated and allows more time for the heat to spread and conduct away. Seems like a bit of an unnecessary complication, considering it would only be cooling the balancing resistors. Much more likely for the heatsink to happen with the version that has discharge path control also.
```

---
## \#105 Posted by: SimosMCmuffin Posted at: 2019-03-21T06:36:07.840Z Reads: 136

```
Got the charging cut-off and the battery voltage sense circuit assembled.

![image|690x273](upload://2uddwHdP6DWLw9uCxHfe3UPQG9M.png) 

I didn't get to test the actual charging through this circuit yet, as I started figuring out why I was getting a little too low reading from the battery voltage sense circuit.Connected my ~12,50 V battery, analog pin voltage was around 491 mV, hmmm, checked with a calculator what the ideal voltage should be, 512 mV... These would translate to 11,90 V and 12,49 V respectively. That's actually quite a lot lower. Why though :thinking:?

Even weirder was that the lower N-fet seemed to be conducting with a gate voltage at 0V. What? Well after some multimeter voltage measuring and checking schematic and fet datasheets turns out I had accidentally put the fets in the schematic the wrong way around, part model wise. P-fet was on the high-side and N-fet on the low side, this is correct in the schematic, but I had somehow mixed up the actual 2N7002 and BSS84PW fet types. 2N7002 is the N-channel that should be on the low side and BSS84PW is the P-channel that should be on the high-side and as you can see from the schematic capture below, I have them wrong way around. 

![image|479x500](upload://mJhmfkJGEiBfg2WUc7imVopyesc.png) 

Well I was able to find substitute fets from my parts bin and got the circuit working as intended (correct fet types, pin outs and voltage capability). Got the measured and AD-converted result within a couple of LSB too, nice. This mix-up is easy to fix for the next iteration.

Next mistake I found when I started writing the software configurations for the ADC. More specifically when I started to map the analog read pins to the correct channels for the ADC. Anybody notice in the picture below any problems with using the PB2 (CHARGER_SENSE) pin as an analog input?

![image|690x153](upload://2Kec23E4wp6RAhIEHB30FyatJUx.png) 

Well... It's not mappable as an analog channel for ADC.... Guess I'm not testing that then. At least the fix will be easy to make for the next iteration. Otherwise the circuit is identical to the battery voltage sense one, so I don't see why it wouldn't give as accurate readings. PB1 and PB2 will be easy to flip around and get that CHARGER_SENSE to a ADC input channel. Easy-Peasy re-trace as shown below.

![image|690x374](upload://jaIU6LDyke12oPiViyhdRZ5289L.png) 

I'll start testing the charging circuit today and then move onto the current sense once that works. Some new board pictures below with a standard XT60 for size comparison (sorry, no standard banana this time).

![IMAG0196|690x457](upload://5eBf1Pfq724rZayJaNdLtgVI6gs.jpeg) 

![IMAG0197|690x466](upload://7gnLJaAmcydRopJngsVm03MEkTa.jpeg)
```

---
## \#106 Posted by: SimosMCmuffin Posted at: 2019-03-22T18:33:01.720Z Reads: 131

```
Charging current tests done and I've got results. 

I used a simple test setup shown below. I'm supplying current from the BMS' charger side with my bench top configurable power supply and on the battery side of the BMS is a configurable DC load. I don't need to use an actual battery in the test setup like this. Voltage is not a critical variable in this test as I'm interested only in the thermal performance in relation to the current.

![IMAG0198|690x370](upload://qkUdzQUDkzeu03Twf0BQdDIHKc7.jpeg) 
![IMAG0199|690x389](upload://f6zHHwiJhdaTHV6V9v0r5wBOd78.jpeg) 


**The tested currents were: 2, 3, 4, 5, 6 and 7 Amps.** For each current test the BMS was left to run for couple of minutes, allowing the thermals to stabilize after which a FLIR image was taken with FLIR ONE. a FLIR image was taken from the bottom side of BMS on currents 5 and 7 Amp.

I also measured the voltage from the following points (shown below) to measure and calculate the losses happening specifically in the MOSFETs for each test current and after letting thermals stabilize.

![IMAG0203|690x281](upload://diAgyFq3zHVta32jNhZKfHSQLzr.jpeg) 

    Test current: 2 A
    Voltage drop: 53 mV
    Resistance: 26,5 mOhm
    Power loss: 106 mW

![Screenshot_20190322-162206|281x500](upload://r14y6k6NmUzUzlZK5wl8diuoPNm.jpeg) 

    Test current: 3 A
    Voltage drop: 82 mV
    Resistance: 27,3 mOhm
    Power loss: 246 mW

![Screenshot_20190322-162619|281x500](upload://wBPzLbo9ghYnCo5pVkoTnf3PX6t.jpeg) 

    Test current: 4 A
    Voltage drop: 115 mV
    Resistance: 28,8 mOhm
    Power loss: 460 mW

![Screenshot_20190322-163014|281x500](upload://nmkJi47UouHLRgBIBzasQOgrnn7.jpeg) 

    Test current: 5 A
    Voltage drop: 151 mV
    Resistance: 30,2 mOhm
    Power loss: 755 mW

![Screenshot_20190322-163519|281x500](upload://b2lS4JzDU2k6XWts2mpiZd6EtEm.jpeg) 
![Screenshot_20190322-163541|281x500](upload://ycqkDQakqvSn8iNPY94N8fm9Rhr.jpeg) 

    Test current: 6 A
    Voltage drop: 196 mV
    Resistance: 32,7 mOhm
    Power loss: 1176 mW

![Screenshot_20190322-163902|281x500](upload://19LOubQhYT1Wbe3oDllir7rtKqo.jpeg) 

    Test current: 7 A
    Voltage drop: 260 mV
    Resistance: 37,1 mOhm
    Power loss: 1820 mW

![Screenshot_20190322-164345|281x500](upload://gRal78GjOYbedsY0iGhZ8H5J0sI.jpeg) 
![Screenshot_20190322-164413|281x500](upload://fQ7W2lHSXc9TzgkEq9ptnIvUYeh.jpeg) 



Here are the results of all the current tests collected to a google sheet and a couple of charts drawn from them.

![image|690x436](upload://j50t3ijKy9FTU5kYgWIztSq9wnm.png)

---


From the charts can be seen the effects of the increasing temperature alongside increasing current. Voltage vs. Current and Resistance vs. Current should technically be linear, but as the mosfets heat up their Rds(on) resistance increases, therefore producing more voltage loss as the current increases. This is then magnified even more in the Power Loss vs. Current, as it already rises in the square of the current. 


**Conclusion:**

With these MOSFETs, I wouldn't personally go above 5 Amps for the charging current, as things start to get real toasty above 5 Amps. Far cry from the 10 Amps I envisioned in the beginning. So what's the game plan? **I'll throw a poll at the end of this post** to get some feedback on what the forum members think is high enough as the supported charging current.

To achieve higher charging current the MOSFETs should be optimized for as low as possible Rds(on) resistance, to minimize conduction losses -> minimize heat generation. Switching speeds are not critical as the MOSFETs are not run with PWM, but are rather just closed or opened for extended periods. Other 2 important attributes then are package size and cost.

Once I get some votes on the poll below and see what people would want, I can then start to check possible options for the mosfets and then discuss about the cost with them. One consideration though is how high of a charge current should the Lite version support, if it's meant to be the lighter, smaller and cheaper option.


---

**How many amps do you think the BMS should support as a maximum charge current? (Lite version)**
[poll type=regular results=always public=true]
* 5 A is enough
* 6 A
* 7 A
* 8 A
* 9 A
* 10 A
[/poll]
```

---
## \#107 Posted by: Surfer Posted at: 2019-03-22T19:31:17.553Z Reads: 122

```
The mostly common used charger is 4 amps, 6 and 8 is a bit more expensive but our batteries are ready to handle 8 charging amps just fine. Other point with 5+ amps is the connector, the most common is power jack 2,1x5,5mm this doesn't handle a lot more than 4 amps. Actually I have 8 amps charger and I keep charging to 5 because I didn't find a nice and small connector up to 8. I think most of the beginner builders they will no go above 5 amps easily. I rather prefer 8 amps but seems logic for a lite version up to 5. 

Edit: I want to vote 5 by mistake I did 6 and can't change it :smile:
```

---
## \#108 Posted by: Pedrodemio Posted at: 2019-03-22T19:56:18.631Z Reads: 121

```
Looking great

Just a suggestion for the MOSFET

https://www.digikey.com/product-detail/en/toshiba-semiconductor-and-storage/TPW1R306PLL1Q/TPW1R306PLL1QCT-ND/6188444

It was the best I could find for a reasonable price for my antispark switch
```

---
## \#109 Posted by: pjotr47 Posted at: 2019-03-22T20:16:36.486Z Reads: 122

```
I am charging my board at this moment with 8A and want to go to 10 or 12A :see_no_evil:
```

---
## \#110 Posted by: Darkie02 Posted at: 2019-03-22T21:26:44.113Z Reads: 123

```
Voted 6a because.
Most common battry q30.
spec sheet standard charge 1.5a.
Most common battry config 10s4p.
4 Q30 in parallel standard charge 6a.
```

---
## \#111 Posted by: SimosMCmuffin Posted at: 2019-03-23T15:29:56.599Z Reads: 122

```
[quote="pjotr47, post:109, topic:85493"]
I am charging my board at this moment with 8A and want to go to 10 or 12A :see_no_evil:
[/quote]

What's your pack configuration and what cells?

[quote="Pedrodemio, post:108, topic:85493"]
Just a suggestion for the MOSFET

[https://www.digikey.com/product-detail/en/toshiba-semiconductor-and-storage/TPW1R306PLL1Q/TPW1R306PLL1QCT-ND/6188444 ](https://www.digikey.com/product-detail/en/toshiba-semiconductor-and-storage/TPW1R306PLL1Q/TPW1R306PLL1QCT-ND/6188444)
[/quote]

Might be a overkill and a bit pricy (@ volume 1,4 € ea.) compared to the 20 cents (@ volume) per piece for the current 5 Amp continuous ones.

https://www.digikey.fi/product-detail/en/diodes-incorporated/DMT6004LPS-13/DMT6004LPS-13DITR-ND/5699713

This is a bit more reasonable. Should be able to do the 10 Amps or very close at least. 

[quote="Surfer, post:107, topic:85493"]
The mostly common used charger is 4 amps, 6 and 8 is a bit more expensive but our batteries are ready to handle 8 charging amps just fine. Other point with 5+ amps is the connector, the most common is power jack 2,1x5,5mm this doesn’t handle a lot more than 4 amps. Actually I have 8 amps charger and I keep charging to 5 because I didn’t find a nice and small connector up to 8. I think most of the beginner builders they will no go above 5 amps easily. I rather prefer 8 amps but seems logic for a lite version up to 5.

Edit: I want to vote 5 by mistake I did 6 and can’t change it :smile:
[/quote]

Yea, the common 2.1x5.5 / 2.5x5.5 mm DC connector will become the limiting factor after 4 or 5 Amps. 

**Anybody** have any good charger connector ideas/recommendations capable up to 10 Amps?

[quote="Darkie02, post:110, topic:85493, full:true"]
Voted 6a because. Most common battry q30. spec sheet standard charge 1.5a. Most common battry config 10s4p. 4 Q30 in parallel standard charge 6a.
[/quote]

Thanks for the feedback.
```

---
## \#112 Posted by: Pedrodemio Posted at: 2019-03-23T16:24:08.168Z Reads: 110

```
Sorry, completely forgot you are aiming for just 10 A

About the charger connector, at 10A XT30 starts to make sense and really easy to find, unfortunately not waterproof
```

---
## \#113 Posted by: Surfer Posted at: 2019-03-23T16:39:03.929Z Reads: 107

```
Here is the nicest power jack I could find, they can handle 11 amps, not crazy expensive but it's bigger than it looks in pictures.
http://www.switchcraft.com/Category.aspx?Parent=943
```

---
## \#114 Posted by: Pimousse Posted at: 2019-03-23T17:31:34.328Z Reads: 113

```
[quote="SimosMCmuffin, post:111, topic:85493"]
**Anybody** have any good charger connector ideas/recommendations capable up to 10 Amps?
[/quote]

XT30 is the best option for me.
It's really thin for the current supported !
```

---
## \#115 Posted by: rojitor Posted at: 2019-03-23T17:55:58.118Z Reads: 115

```
I use Anderson for high current. 45amps rated. Even more amps capable.
```

---
## \#116 Posted by: SimosMCmuffin Posted at: 2019-03-23T20:36:25.339Z Reads: 117

```
[quote="Pimousse, post:114, topic:85493"]
XT30 is the best option for me. It’s really thin for the current supported !
[/quote]

[quote="Pedrodemio, post:112, topic:85493"]
About the charger connector, at 10A XT30 starts to make sense and really easy to find, unfortunately not waterproof
[/quote]

Should have ordered couple of the XT30s from the hobbyking when I bought the GT2B for the Chozen remote mod. I even ordered some MT60 3-phase motor connectors just to check them out...

Maybe I'll make a small XT30 panel adapter PCB, which can be easily then installed onto an enclosure. Backside of the connector can be filled with hot glue or your goopy filler of choice, so water can't enter the enclosure through the connector. Although grime and dust will accumulate in the open front area and onto the contacts... not good.

Well at least there is no need for anti-spark connectors thanks to the fully blocking charging switch setup. No inrush really in either direction at least when plugging in the charging connector. But the dirt accumulation can be problem...
```

---
## \#117 Posted by: Darkie02 Posted at: 2019-03-23T20:48:46.311Z Reads: 115

```
I just put a spare XT30 socket in the hole stops dirt getting in . Keep meaning to 3D print a little plug to push in at some point but still haven’t got around to making one yet
```

---
## \#118 Posted by: SimosMCmuffin Posted at: 2019-03-23T20:52:40.162Z Reads: 118

```
https://www.thingiverse.com/thing:2900417

EDIT: also

https://hobbyking.com/en_us/xt30-plug-fixed-mount-board.html
```

---
## \#119 Posted by: Darkie02 Posted at: 2019-03-24T07:43:11.273Z Reads: 117

```
Them caps go over plug and mine only sticks out a few mm on the board. So need to design some thing to go inside the male plug.

Edit
Prefer this type of clamp leaves less sticking out the case ![image|664x500](upload://ziNNqGIUWt2SCha64BmeNXV3HlE.jpeg)
```

---
## \#120 Posted by: SimosMCmuffin Posted at: 2019-03-24T10:35:08.067Z Reads: 120

```
So, after looking at the poll results and at the comments. I have decided to go for the **10 Amp** charge.

Based on the test results. I would aim the temperature for the MOSFETs to be max ~50-60 Celsius @ 10 Amp. For the current MOSFETs this area currently resides in between the 4 and 5 Amp test currents  temperature wise. The effective resistance on the MOSFETs was around 14.5-15.0 mOhm (per mosfet, note 2 back-to-back in circuit) with a power loss of 250-300 mW in each mosfet. 

Below is a chart from the MOSFET datasheet showing the Rds(on) behavior according to Id drain current and package temperature and I have marked the location the mosfet is operating in at the 4-5 Amp test currents.

![image|520x500](upload://okKheYgNuHFhYHFhsJOZVsprhRS.png) 
https://www.digikey.fi/product-detail/en/diodes-incorporated/DMT6016LSS-13/DMT6016LSS-13DICT-ND/4967052

So to be able to double the current we need to cut the Rds(on) at least to a quarter of what it is to maintain the power loss at the same level. So the beefier MOSFETs can have a maximum Rds(on) of around 3.5 mOhm @ 10 Amps and 50 Celsius.

Digi-key part filtering based on these criteria and then sorting by the cheapest lead me to the following MOSFET. Datasheet inspection shows that this MOSFET should be able to achieve 2.7-2.8 mOhm Rds(on) @ 50 Celsius with 25 Amps of current, which is higher then what we are even aiming so the effective Rds will likely be even lower then what I have circled on the graph below. The power loss @ 10 Amps should roughly be around 250-300 mW, essentially the same as the in the old MOSFETs @ 4-5 Amps.

![image|532x451](upload://pGJ7RGoFO8gt3hsrWwRHsdSDpuU.png) 
https://www.digikey.fi/product-detail/en/diodes-incorporated/DMT6004LPS-13/DMT6004LPS-13DITR-ND/5699713

One thing that will also cause more losses at higher currents will be PCB trace resistance, which will start to be a consideration at these higher currents, this so far has been purely about the conduction losses in the MOSFETs. Quick calculations with trace calculators show roughly a 20 Celsius increase in the traces at @ 10 Amps with the current trace sizes.

So what's the cost difference?: Price @ volume: old FETs: 0.2€ ea. new FETs: 0.6€ ea.

**Worth it? (Component cost)**
[poll type=regular results=always public=true]
* 5 Amp capability baseline cost 0.4€
* 10 Amp capability +0.8€ -> 1.2€
[/poll]
```

---
## \#121 Posted by: Friskies Posted at: 2019-03-24T10:44:53.838Z Reads: 114

```
That difference in cost is negligible. I don't see why you wouldn't :P
```

---
## \#122 Posted by: banjaxxed Posted at: 2019-03-24T11:03:03.797Z Reads: 115

```
Agreed, this is a core aspect, unless you’re building to sell commercially that € value does not make any difference, even to the tweens
```

---
## \#123 Posted by: pjotr47 Posted at: 2019-03-25T21:41:03.873Z Reads: 115

```
[quote="SimosMCmuffin, post:111, topic:85493"]
What’s your pack configuration and what cells?
[/quote]

12s4p with sanyo 20700B.

Next battery will be a 12s7p with samsung 30q charging with 12A :wink:
```

---
## \#124 Posted by: Darkie02 Posted at: 2019-03-25T23:23:07.205Z Reads: 116

```
Rated to 10a 50v 

![image|200x200](upload://ysg4RfYimirLCIkyA9e709iaqL9.jpeg) 

https://www.digikey.co.uk/product-detail/en/globtek,-inc/JACK-C-PC-10A-RA(R)/1939-1086-ND/8597889?utm_adgroup=&mkwid=sVwLkHM8h&pcrid=338202715904&pkw=&pmt=&pdv=m&productid=8597889&slid=&gclid=CjwKCAjw-OHkBRBkEiwAoOZqlxYiuIjVyD5IeprOM9wuapNjI3-8DHHHzucjB-3oeAC3-dLUm_xwmhoCKkMQAvD_BwE



60v 10A/30A/40A magnetic connector 
Tho I think you need to make some kind of time delay circuitry with the data pins as it’s not hot plugerble not worked it out but been toying with the idea tho it’s quite chunky and expensive.
![image|243x100](upload://tHiUcoQ9yaXDaEC2eiu6ALftdzb.jpeg) 
https://www.rosenberger.com/0_documents/de/catalogs/ba_automotive/AUTO_RoPD_Flyer_2016.pdf
```

---
## \#125 Posted by: SimosMCmuffin Posted at: 2019-03-27T18:19:27.719Z Reads: 118

```
Work (at the office) has been just downright depressing and I have become void of feelings and energy...

Anyhoo...

**Tested the charging current sense circuit.** I was getting a little too high of an output from the INA180 current sense amplifier, roughly 5-7% more than supposed (@ 2 Amps was getting ~536 mV, should be ~500 mV). Checked the datasheet to see what the internal error can be at maximum, which was about 2%. 

I'm 90% sure of what's causing this though, which is sloppy ground flood design in the sense circuit. The sense traces have extra ground return current going through them, which causes the extra sensed voltage, which then gets amplified and results in the erroneous output voltage. Essentially the 5 mOhm current shunt resistor is fine, but there is extra resistance from the sense traces and is therefore something like 5+0.25 mOhm and because ground current is flowing through this small trace it's causing that little extra voltage drop and therefore it's showing too high of an output.

Fix will be to isolate the sense traces from the GND planes/pours with some keepout areas. If the charging current can't return through the via the sense trace, it will just measure the voltage drop over the shunt resistor.

---

**Also got the better 3V3 linear regulator (and 47 Ohm bleed resistors)** and retested the current consumption in the low-power-run mode. **Got 50-60 µAmps in a sawtooth pattern, which I'm tempted to average to 55 µA!** I'm very happy that the consumption is able to go so low, while still staying in running state. I'll post a pic of measurement with the office's benchtop multimeter.
```

---
## \#126 Posted by: Pedrodemio Posted at: 2019-03-27T18:25:34.723Z Reads: 116

```
Great news about the consumption :grinning: 

I was thinking about how this BMS could make easier to use external range extenders without a DC-DC converter

In the current state how would the BMS would react in this scenarios?

1 - external battery with higher voltage than the internal, and with a voltage difference large enough to cause a current flow higher than 10A. Would it just cut the charge until unplugged?

2- external battery lower than the internal battery. If I recall from the last topic it won’t allow reverse current through the charge port, so nothing would happen until the board battery discharged to an equal or less voltage?
```

---
## \#127 Posted by: SimosMCmuffin Posted at: 2019-03-27T18:50:19.792Z Reads: 118

```
[quote="Pedrodemio, post:126, topic:85493"]
1 - external battery with higher voltage than the internal, and with a voltage difference large enough to cause a current flow higher than 10A. Would it just cut the charge until unplugged?
[/quote]

Correct. If the current stays under the configured max charging current (10 A max) and above the end of charging current then everything should be peachy.

[quote="Pedrodemio, post:126, topic:85493"]
2- external battery lower than the internal battery. If I recall from the last topic it won’t allow reverse current through the charge port, so nothing would happen until the board battery discharged to an equal or less voltage?
[/quote]

It's a fully blocking setup, so if it's turned off then current can't flow in either direction (while bq76200 gate driver is still powered). Reverse charging current, aka, discharge current can't be measured with the INA180 in the charging path. Most likely a beginning state to start charging is the "Charger Voltage" >= "Battery Voltage" and then monitor the current, if the current is negative then it will most likely be measured as zero charging current (haven't tested yet) and the charging will be turned off.
```

---
## \#128 Posted by: Pedrodemio Posted at: 2019-03-27T19:33:44.745Z Reads: 115

```
Perfect, this will make a no brainer to plug an external battery, initially I would use another micro controller to check the diference between packs and calculate what the current would be, and if within acceptable margin turn on a MOSFet to enable charging
```

---
## \#129 Posted by: SimosMCmuffin Posted at: 2019-03-29T09:25:44.548Z Reads: 121

```
Current consumption in Low-Power-Run state @ 100 kHz, so we are still running code, albeit slower and with certain peripherals disabled, but still executing code ( empty while(1) loop in the measurements ). Could go even lower in Stop Modes, but gonna have to check how implement in a smart way (wake-up period wise).

![IMAG0207|690x442](upload://bnfk9tmNRvdVnbBNTiN8GvByEfi.jpeg) 

https://media.giphy.com/media/SILI7okOcKnPM2Fh6X/giphy.gif
```

---
## \#130 Posted by: Surfer Posted at: 2019-03-29T10:36:42.122Z Reads: 121

```
Wow! is tiny than I thought! Congrats buddy
```

---
## \#131 Posted by: Arek Posted at: 2019-03-31T23:41:25.726Z Reads: 122

```
Was thinking about buying that maynuo electronic load, do you recommend it? :stuck_out_tongue:
```

---
## \#132 Posted by: SimosMCmuffin Posted at: 2019-04-01T07:26:11.954Z Reads: 124

```
For what it is (a copy of BK precision DC load) I'm happy with it. Displayed current and voltage readings are reasonably accurate.

One weird thing that I have detected in my use, is that the battery capacity measurement for some reason seems to be running a little too slow on the time scale. For example, the load current is 100 mA (verified by my multimeter), DC load shows around 100,8 mA, so it should be registering the correct current, but after a hour of discharge time the used capacity shows only 97 mAh on the DC load, as if the meters time keeping is running a bit slower.

I have compensated by taking timestamps of the time and current and from that calculated the real used capacity.

Apart from that it's been good enough for my use. Personally I would upgrade or buy the 300W version, if I were to get one today. Makes getting a bit more truthful capacity measurements easier and helps locating problem spots thermal wise in battery packs.

---

I'm currently fine tuning the opto-isolator front resistor. The original 4k7 one was running pretty hot with 43 Volts at 60+ Celcius. 10k was a bit better at 45 C, but I think I'm gonna go a bit bigger than that.

I also tested the current consumption at 43 Volts and it slightly increased to 65 µA, but it was still very cozily under the aimed amount.
```

---
## \#133 Posted by: Arek Posted at: 2019-04-01T09:53:57.745Z Reads: 123

```
Thanks mate.
I guess that the oscillator of the main uC is off, perhaps you could try to alter the capacitance of one of them to correct it?
For that you need a frequency counter.
```

---
## \#134 Posted by: SimosMCmuffin Posted at: 2019-04-05T10:12:04.448Z Reads: 129

```
**Update:**

...I went on a tangent... a deep one... Like I have a bad habit of doing :sweat_smile:

_Long story about the escalation from a simple start following_

bms hasn't progressed much, so what have I been doing?Well *record scratch*... It all started when a colleague couple weeks ago went to go eat at a local mall on his lunch break. He then popped by an electronics/hobby/hardware/misc store (Clas Ohlson) on his way back, because they had a deal going there. For **ONE** euro you could buy this small, simple and cute DIY bluetooth speaker kit (shown below). He bought **5**.

https://images.clasohlson.com/medias/sys_master/9630741168158.jpg 
https://images.clasohlson.com/medias/sys_master/9630741299230.jpg

He bought one for the office and I'm sure I looked like an excited manchild when I was assembling it (we were all making good jokes and times about it). I thought it was pretty dope, as a concept and for the price one couldn't complain. You could power it via USB or 3 AA batteries.

Here it starts... The sound was quite tinny, no doubt in large part for the cardboard case having more holes in it than a traffic sign in Alabama. Ok, I can make a better box for it to improve the low end. Hmm... 3 AA batteries should actually be operating pretty near lithium cell voltages, let me just try it with a single 18650 cell, oh it works no problem. How much power does it use?, *does some current use measurements* oh this thing should last like at least 15+ hours on a single cell with decent volume... This could actually be made into a pretty sweet portable boombox with some effort...

I even looked up the ICs on the control board. Bluetooth comms were handled by Beken BK3254 ( https://oss.aliyuncs.com/netmarket/29bc7cac-8266-45bf-b2b0-f152227ba546.pdf ) and the 2 drivers were then driven by 2 MIX2052 mono channel class D amplifiers ( http://www.pluschiptech.com/web/userfiles/download/MIX2052_Prilimineary_datasheet_V1.0.pdf )

![IMAG0239|690x459](upload://SildWGE7jshWT1LdVbLL4kBguz.jpeg)
![IMAG0232_1|427x315](upload://cxSyJ5JVcoRJ1MQj50fcmyFZF68.jpeg) 
 

After looking at how simple the class D amp circuit was, I went onto Digi-Key to check what they had. There are many low-power class D amp ICs that can work off of a single lithium cell. Hmm... I have always been interested in getting into some audio stuff, but it has always seemed just a bit too complicated to get started, but with a single IC and just 5 external components I could have the equivalent amplification as on the original board.... So I then started designing my first audio amp board... There was also some escalation on the design too and in the end it ended up getting a op-amp low-pass circuit in front of the audio amp (haven't really worked with op-amps before, so I saw this as a good opportunity to start tinkering with them). I also LTspice simulated the low-pass behavior.

![image|690x379](upload://yLtYhYcumWeTj91PsQ1Pw564o8Q.png) 
![image|683x500](upload://rCZKA6wKMxDk4l0K6AeCaI76q7i.jpeg) 
![image|618x500](upload://rZc93hNJBVOxh3BbK3ujvSIV24r.jpeg) 

But of course, things must escalate more... I then decided that I want to charge the 1S lithium cell battery via USB and it should be protected against overdischarge, so I then started designing a single cell BMS... Which ended coming out like this.

![image|623x500](upload://rT4Radn3dX4OyALANgUOmjMyHZP.png) 
![image|519x500](upload://1zm6zXsYzXzzkFqq5Mxwm1zwY8x.jpeg) 

So... This 1 euro bluetooth speaker has already been escalated to 2 custom PCBs... Well we can go  further than that! I then spent couple next days designing a new enclosure that fit all the original parts.

![image|690x424](upload://khyIg3xw8JNia4aCqlpudTYGrDA.png) 
![image|690x420](upload://fMx1ZEl3Spb37FXQHwtmnOvumrO.png) 

I then spent couple days 3d-printing the parts and shown below is the assembled package.

![IMAG0215|690x475](upload://9K8oAfnJ8MXumMfeuwVJh82qL4t.jpeg) 
![IMAG0216|637x500](upload://eXovmM1z1yIG6AyvkADGsyuttmQ.jpeg) 
![IMAG0217|654x500](upload://2zWOEQc00JBlLs9biJlDmdE5X2I.jpeg) 
![IMAG0218|690x437](upload://31SRV7ksbE3CkfDneN3tKR9Tv09.jpeg)

There was still a small problem, it was still sounding pretty tinny (all original parts still). Hmm... I remember that Digi-Key does have some decent Peerless speakers... I guess I'll just have little look... Oh those ones are quite cheap (7,5 € ea.), how will they work in a small enclosure though... Guess I'll boot-up Winisd and simulate their behavior with the speaker parameters... ( http://www.loudspeakerdatabase.com/Peerless/PLS-65F25AL04-04 ). I also spent quite a lot of time just reading about speaker parameters, trying to understand their impact on the speaker behavior in different enclosures and testing my expectations through simulation.

![image|690x489](upload://oLmNuFiRXPSTEyk2DF6uY8gUEN6.png) 

Oh these ones could go decently low in quite a small volume vented enclosure... Guess I'll order couple of those! After looking at the first enclosure for some time I decided I wanted to make a better one. I also needed to optimize the printing process at the same time. I approached the new enclosure from a different perspective.

![image|690x428](upload://fmvTqotQcuYkq4Jo6ouYp1049Cw.png) 

And you know what. I'm pretty darn happy with it at the moment and I think it's pretty cool.

![IMAG0227|615x500](upload://1xMrItfr0hjlQNVCRKDDFDSkKxb.jpeg) 
![IMAG0228|658x500](upload://qM6TiuowMIjVViZW7CvRckbeWXq.jpeg) 
![IMAG0229|608x500](upload://91bGMs2J3poarAyBVTMBrgxSeue.jpeg) 
![IMAG0230|689x390](upload://5KQdLWyoea0O6SHAevmXQ3OKnnw.jpeg) 
![IMAG0231|506x500](upload://wD67QNmhqoJQLC8bD7lrRpMqIHC.jpeg) 
![IMAG0232|690x498](upload://dTkn0CZ5ngJY0woOuNc8hNEfElH.jpeg) 
![IMAG0233|689x390](upload://9spmkreymQHpcLtJTUz1Xqljux8.jpeg) 
![IMAG0234|690x389](upload://17dZ18Hl6bDKAf1FlcTE0dGSblg.jpeg) 
![IMAG0235|671x500](upload://7NJi9PDOQh6Cqxvyp69MpCrsCl0.jpeg) 
![IMAG0236|604x499](upload://b8g2AcglmUqEEndPg2gCU6ry65C.jpeg) 
![IMAG0237|690x476](upload://ZcMhyaiy8X4ytEHY0mFmoRcaDf.jpeg) 
![IMAG0238|547x500](upload://1Q1mY3eTDeHrMeqFGIjzXlQqret.jpeg) 

It has good low-end for being a very portable speaker and is quite loud. Not gonna burst ear drums, but loud enough for indoor use. Once I get my custom amp boards I can tame the top-end a little bit down. But only original part left in the speaker is the bluetooth and amp PCB + speaker wires. I even changed the volume knob.

But this was my escalation story about how a "1" euro cardboard bluetooth speaker kit turned into tens of hours of development, studying, simulation and design hours... But I feel content and satisfied... for now...

**TLDR**: I got captivated by a 1 euro bluetooth speaker kit and spent tens of hours making "improvements" to it.

----

On BMS end of things... The only real thing left to do is to test the CAN bus. Opto-isolator has been tuned and tested to work from 2.8 - 50 V control signals without leaving the front resistor dissipate any crazy amounts of heat.

I'm gonna write the testing CAN libraries on the weekend and then test the comms in the office with a PC CAN adapter.

We are essentially on the final straight in the development for the 0.1 HW iteration. I have quite a list of bullet points collected on things that need changing to 0.2 and I will start implementing them once the CAN is tested and confirmed working.
```

---
## \#135 Posted by: Pedrodemio Posted at: 2019-04-05T11:49:54.055Z Reads: 123

```
Now that you got bitten by the DIY audio bug you won’t let go, soon you will have speakers bigger than your fridge in your living room 😁, speaker drivers everywhere and etc 

The pleasure of building a speaker and it sounding good or even better than any other you heard is priceless 

If you really wanna go down the rabbit hole check out Horneresp (http://www.hornresp.net), way more advanced simulation capabilities and some crazy designs are possible

A calibrated microphone is also a must 

This is one I’m working for the last year, already changed a lot of things without even finishing the first version, from passive to active and dsp driven crossover, countless Bluetooth modules

(Tweeter disconnected on this video and distortion from my phone)
https://instagram.com/p/BmT6LRGl9RR/

On the BMS, on what version you would think to start getting beta testers?
```

---
## \#136 Posted by: SimosMCmuffin Posted at: 2019-04-09T17:40:35.727Z Reads: 122

```
[quote="Pedrodemio, post:135, topic:85493"]
On the BMS, on what version you would think to start getting beta testers?
[/quote]

Once I get the obvious HW related problems fixed, then probably after I get the first small test batch from a chinese PCB+Assembly house to see if there are any problems with the DFM/MFG files.

When will that be? Can't say, because I don't know.
```

---
## \#137 Posted by: SimosMCmuffin Posted at: 2019-04-14T19:55:51.644Z Reads: 132

```
Finally have some intelligent life on the CAN bus!

Full CAN frame with 8 bytes of 0x55 (every bit changes state) at the correct baudrate (500kHz)
![IMAG0250|690x389](upload://23JntDVhd1n5cOTeAOO3Yoe9cBE.jpeg) 

Some things that have been going on in the background:

* Boarding season started 2 weeks ago, then was immediately cut off as winter made a comeback like the baddie from some bad horror film
* My car battery gave it's last breath of life when it decided that it wasn't able to give enough current to even turn the engine over on a cold winter comeback morning
* ...public buses...*shudder*...
* My 3D-printers ATX-power supply crapped out, but I fished another one out of my old gaming rig
* I _think_ I got the worst of the audio bug out for now (check couple posts back for reference). Got the mono D-class PCBs assembled and tested and figured out some basics from those tests
* STM32 Workbench decided to completely implode on me. Luckily I was able to get backups of all of my projects on it. Installed the newest one and got it set up and working, my old projects couldn't be imported back easily though, so I now have only the FlexiBMS_lite on there
* Had to do some studying on how the CAN bus works and especially how the registers are implemented in the STM32, but I have a pretty good grasp on it now
* Got my Metr Pro hooked up and finally got to do a test ride with it

As for what's next for the project. I think it's time to start working on the 0.2 HW. Everything is pretty much tested on the HW side and all the found problems have been noted up. So I'm gonna start doing the PCB revisions next week and then once I get the boards ordered, intend to clean up all the written test code and start building more functionality onto it.



I'm gonna post a list of all the HW changes I have written down in the coming days and expect a lot of pictures.

---
**CAN bus technical discussion**

_CAN bus grounding? Is it necessary, or will it create mustard gas :thinking:?_

Let's take a look at connecting multiple VESCs together, it's a surprisingly opinion dividing topic on how it's best to connect them together. Hence there is a thread with nearly 300 replies on this particular matter:
https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461

But this isn't about that PPM Y-split vs. CAN discussion. This is about that third signal wire that is awkwardly hanging around like your old Ex (_GND_) in the background as you're going on a date with your new girl (_CANH & CANL_)... Sometimes you just wonder if you would've been better staying with her or if you should try to ask her to a threesome...

So, innuendos aside. **There are 3 possible ways to do grounding in CAN bus** associated communication and all can be summarized easily in this easy-to-understand memetic image.


[details="Image"]
![image|690x386](upload://jwjHfCICzyEYBlNkqx3OTioNed.jpeg) 
[/details]


In practice, all CAN transreceivers need to be in within a certain range for common-mode voltage swing, AKA in relation to ground. Even though the data carrying signals CAN HIGH and CAN LOW are differential for better signal integrity and noise immunity.

In the official CAN Bus standard (ISO 11898-2) this common mode offset-voltage is specified as:
![image|641x39](upload://k514QsWi7VwqAYZXNurDeNz1ayv.png) 

But available ICs can support much larger common mode offset voltages like the TJA1051 at +-30V:
![image|690x174](upload://dVm5z3HSmJD02MGKAovzJ2nRgSK.png) 

But I think it makes more sense to look at the question with the 3 possible grounding strategies:
* No CAN ground
* Weak CAN ground
* Strong CAN ground

Then ask the question how far can the Grounds of 2 or more CAN transceivers be offset at worst case or at least in normal operation: 

If there should be no reason for large ground offsets, there is no need for dedicated CAN ground. The shared system ground will be good enough. This in my opinion mirrors the most common use case in esk8ing with 1 battery pack powering all ESCs and therefore supplying a strong ground with the power lead harrness. Pictured below is my board's VESC setup with a clearly strong system grounding, meaning there is no need for the CAN ground connection between the VESCs (and in fact should not be used to avoid ground loops).

![IMAG1109|690x389](upload://3Rd1tZQCO82h8qExE2GKFFAgUEl.jpeg) 

Strong CAN grounding should be used if multiple ESCs were powered from 2 or more separate battery packs, AKA pack #1 only powers ESC #1 and pack #2 only powers ESC #2, as in this case there is no common ground shared between the 2 CAN trans-receivers on the ESCs, causing them to be floating in relation to one another. The better place to do this grounding would be to connect the ground of the battery packs together in my opinion. A strong grounding can be used, because the ESCs don't share the ground currents and this goes for multiple floating devices, they need to be tied together in some way.

Weak grounding should be used if the devices share a common ground, but for one reason or another can exhibit large ground voltage swings. Strong grounding can cause large ground currents to travel through the CAN's Ground if that pathway is presenting a lower impedance to the system ground. Weak CAN Ground will present much larger grounding impedance to lower the possible ground currents to a much lower level, and therefore lowering the voltage drop on the CAN Ground line, more likely staying within the maximum offset voltage. I'm not quite sure if the better idea would be to add a resistor in-line to the CAN Ground wire, or between the CAN transceiver's ground pin and device ground.

But there. That went on a bit longer than I intended, but hopefully what I wrote made sense and that I had correctly understood what I had read and studied.
```

---
## \#138 Posted by: Komamtb Posted at: 2019-04-16T11:04:31.925Z Reads: 125

```
I assume it's not an issue to charge with a less of a current? 12s 10a chargers don't come cheap.
```

---
## \#139 Posted by: Friskies Posted at: 2019-04-16T12:44:17.416Z Reads: 121

```
Not a problem at all. It just means that your charge time will be longer. In saying that max charge rate depends on your pack configuration anyway.
```

---
## \#140 Posted by: SimosMCmuffin Posted at: 2019-04-16T14:09:20.063Z Reads: 130

```
Changelog 0.1 -> 0.2 HW iteration:

* **Connect BOOT0 pin to GND** (pin left floating read as a logical "1", causing weird behavior in boot, band aid fix done by writing nSWBOOT0 to "0") 
* **Capacitor values for MCU and linear regulators 1µF**
* **MCU linear regulator switch from AP2210N-3.3 to TS9011SCX** (for lower quiescent current consumption)
* **Breakout pad for 5V**
* **Reset breakout pad**
* **Finetune LTC6803 footprint** (increase pad length slightly)
* **Add BAS20 diode to the LTC6803's linear voltage regulator output**
* **Lower balancing current** (change resistors from the initial 33R to 47R due to thermal performance. Balance current changing from 125mA to 88mA)
* **Fix Q3 and Q4 mix-up at the battery Vsense** (accidentally put the wrong fet types the wrong way)
* **Change charger sense pin to one with analog connection** (fix already described on post #105)
* **Change opto-isolator footprint to correct one** (used a bit too big one)
* **Charging FET change from DMT6016LSS-13 to DMT6004LPS-13** (in effort to achieve 10A sustained continuous charging current)
* **Charging current sense trace isolation** (currently the sense trace shares ground return currents, causing higher than real current measurement results)

That is everything I have noted in my hardware assembly, testing and discussion in this thread. Most of these changes are quite minute, not really needing huge layout changes on the board, so implementing these changes/fixes shouldn't take that long.

If somebody has questions about the change list, this would be the best idea to present them.
```

---
## \#141 Posted by: SimosMCmuffin Posted at: 2019-04-23T17:39:18.964Z Reads: 130

```
Remembered one thing I hadn't test yet, which was the RGB indication led on the board. Made couple short clips of it in action.

![gif|480x270](upload://fxvgc6q0Y3DhGu4SMSTrw4oQyuW.gif) 
https://giant.gfycat.com/CarelessMarvelousIchthyosaurs.webm

I have finished the 0.2 HW changes and I'm going to order the new PCBs this week.

![image|690x458](upload://jmS97zzBZTwHgfDChrY6gFhhsv.jpeg)
```

---
## \#142 Posted by: Darkie02 Posted at: 2019-04-24T07:49:17.924Z Reads: 121

```
How thick is the BMS with plugs and sockets?

I’m thinking having cables coming out both sides uses a lot of room up compared to how small the BMS is. 
Is it possible to raise up and spin the connectors on one side 180 deg with out the thickness exceeding 18mm (diameter of a 18560 cell) this would allow cables to be routed down 1 side layered on top of the other ones. Reducing the space you would have to dedicate to the BMS inside a build ones it’s has all its connections attached.

It’s just a idea and I have no idea if this would cause to much mechanical stress or heating issues by doing some thing like that or if it need covering with fish paper or some thing so resistors don’t melt and short cables. Or any other issue that may arise from doing that others might foresee.  

Edit:
This would all depend if you place you BMS next to or on top of your battery I suppose.
```

---
## \#143 Posted by: Friskies Posted at: 2019-04-24T19:42:28.505Z Reads: 120

```
@SimosMCmuffin this legitimately looks amazing. The layout and design in general looks.awesome! I'm so thirsty for one of your finished products.

@Darkie02 the connectors are place like that so that there Is a battery side and a board side. All the relevant battery connectors are on one end - balance and power. And the other side is all the external inputs and outputs -can charge leads etc. Makes a lot of sense to be like this if you ask me.
```

---
## \#144 Posted by: SimosMCmuffin Posted at: 2019-04-25T06:56:26.083Z Reads: 126

```
[quote="Friskies, post:143, topic:85493"]
@SimosMCmuffin this legitimately looks amazing. The layout and design in general looks.awesome! I’m so thirsty for one of your finished products.
[/quote]

Appreciated.

[quote="Friskies, post:143, topic:85493"]
@Darkie02 the connectors are place like that so that there Is a battery side and a board side. **All the relevant battery connectors are on one end - balance and power. And the other side is all the external inputs and outputs -can charge leads etc.** Makes a lot of sense to be like this if you ask me.
[/quote]

^This

@Darkie02 The board should be under or just about 18mm thickness even if you're using the vertical connectors and have the JST-XH balance connector plugged in with wires connected. You might need to bend the wires of on the XH quite tightly though.

If space is on super premium then you can remove connectors (or order the board without them) and solder your wires directly onto the board.

Below are top and bottom pictures of the board with the connectors named. Feel free to ask, if there is still something unclear.

![image|690x350](upload://6Nrl9e947JTz1a3MeDhXVc3qrMb.jpeg) 

![image|690x350](upload://tYKaNknjUP5hejA1b0G6w0ws2HH.jpeg)

EDIT: I'm gonna finish the board today and order the PCBs
```

---
## \#145 Posted by: Winfly Posted at: 2019-04-25T07:25:39.109Z Reads: 118

```
As always, I love this project and has been following since the beginning of the Full version. Can't wait to use it once it is finished.
```

---
## \#146 Posted by: SimosMCmuffin Posted at: 2019-04-25T16:31:47.516Z Reads: 119

```
0.2 PCBs have been ordered.

Also noticed this very interesting update email in my mailbox from Seeedstudio, I might take a further look into this.

http://www.seeedstudio.com/blog/2019/04/23/free-assembly-for-5-pieces-only-at-seeed-fusion/
```

---
## \#147 Posted by: SimosMCmuffin Posted at: 2019-05-03T19:28:05.343Z Reads: 120

```
PCBs are here. No major difference in the looks, but I also got some XT30s and I would say they are pretty ideal and just so cute next to their XT60 big brother.

![IMAG0270|690x447](upload://3TW0Ox5FZvMTEmd0WqoWdTX92Hx.jpeg) 
![IMAG0271|690x460](upload://5e7xxa9nHUqmQJFo1CRXFwDfH7B.jpeg) 

I'm gonna do inventory on the components tomorrow and order what I'm missing for the next week. I think I might be able to start the assembly, but won't be able to finish it this weekend.
```

---
## \#148 Posted by: ducktaperules Posted at: 2019-05-03T21:53:22.907Z Reads: 116

```
This is looking great. cant wait to get my hands on one of these :slight_smile:
```

---
## \#149 Posted by: Darkie02 Posted at: 2019-05-04T08:22:31.609Z Reads: 118

```
Don’t know if it would work with the lay out but I quite like these.

![image|500x500](upload://my2OGOZxvdAntse34GcWDM0yr34.jpeg) https://ae01.alicdn.com/kf/HTB1ra_.KFXXXXbMXVXXq6xXFXXXY.jpg
```

---
## \#150 Posted by: SimosMCmuffin Posted at: 2019-05-05T16:10:11.110Z Reads: 114

```
Got the parts ordered and I'm working on the code at the moment. Cleaning up the functions and making things more clear and efficient to run.
```

---
## \#151 Posted by: SimosMCmuffin Posted at: 2019-05-05T20:30:32.655Z Reads: 120

```
Decided to do some destruction as a way to end the weekend.

![IMAG0272|631x500](upload://gHBDLcrVpcZTNP1SZLrzQXJYWQ5.jpeg) 
![IMAG0273|440x500](upload://hTCSpO8dplg35GmdChXWVOt9g1z.jpeg) 
![IMAG0274|690x241](upload://82dtAjXC1RhtY5wFAU2uNfB2fvV.jpeg) 
![IMAG0275|690x442](upload://uT2iD03OpNWtnATCF0dHbxTb2f1.jpeg) 
![IMAG0276|524x500](upload://yCYIWQsvQWt9GLhXjjhfrjDLifg.jpeg) 
![IMAG0277|525x500](upload://kUmYRZtKc774nc91Le9QRCEETvk.jpeg) 

Solder joints failed on the vertical one, while the horizontal one tore the copper pads off of the board. It did take some torque to get these off. The XT30s themselves were alright and still connected nicely after this.

Note:
No 0.2 PCBs were hurt in the making of these photos. Only old 0.1 boards.
```

---
## \#152 Posted by: SimosMCmuffin Posted at: 2019-05-09T18:54:26.850Z Reads: 123

```
Got the missing components yesterday and assembled the board this morning.

![IMAG0279|690x468](upload://o4afNpHji2sQDjxJgsx76WtHjNr.jpeg) 
![IMAG0280|690x443](upload://9fitqLPijidcjRzQ4C7S5MGlaba.jpeg) 
![IMAG0281|690x472](upload://nwu5KX6MUOPnWLfMbiw2KUQTTko.jpeg) 

I then decided to test the max charging current. The board was allowed to thermally settle for 5 minutes before taking the FLIR images. Room ambient temperature was around 21 C. I did not measure the voltage loss over the mosfets this time, because I forgot, but the thermal images show the thermal behavior at least for the power loss in them.

6 Amps
![Screenshot_20190509-204920|281x500](upload://lmqP601ZkH6OFUjHShFwCc83cup.jpeg) 

7 Amps
![Screenshot_20190509-205334|281x500](upload://bjNngY9oH6WjaaHecP1a2d3MIF0.jpeg) 

8 Amps
![Screenshot_20190509-205623|281x500](upload://tPrBQISdXJ7poE0QondW3EaxTim.jpeg) 

9 Amps
![Screenshot_20190509-210148|281x500](upload://wSnC01G6DE3Uc7sC7TzWpguLKts.jpeg) 

10 Amps
![Screenshot_20190509-210706|281x500](upload://a6cBGYnnaBSpzzpijUXCYjLDvqI.jpeg) 

11 Amps
![Screenshot_20190509-211241|281x500](upload://ir2u7z4A2L6AYdy26EwjhrGbTc3.jpeg) 

With these thermal results I'm gonna say that it will do continuous 10 Amps. I also checked the current measurements from the improved current shunt sense circuit and it was within 1-2% of the indicated current from the power supply (not lab/reference grade indication), so I'm gonna say that it's also good to go.
```

---
## \#153 Posted by: totalgeek9224 Posted at: 2019-05-19T10:44:34.526Z Reads: 109

```
Any news on this project? :)
```

---
## \#154 Posted by: SimosMCmuffin Posted at: 2019-05-19T17:31:23.611Z Reads: 113

```
No big updates. 

Haven't had a lot of time to do coding, but because the hardware is starting to look fully functional I'm beginning to look into getting the prototype assembly batch under way. At least getting the real cost quotes from a couple of PCB/assembly houses and getting their feedback on the manufacturing files. I also need to think about the flashing and testing jig, so I can reduce the flashing prep & calibration steps.

Been a bit busy at work, as the customer PCB I'm doing the HW design for is supposed to be ready and sent to the fab shop for volume production next Tuesday (that's my excuse at least) + they wanted some changes to it on Thursday. I'm also writing the most basic firmware functionality into it for this beginning milestone.

I have been also thinking and planning about how to structure the code, so that it wouldn't start snowballing into a obfuscated mess of uncommented & confusing spaghetti monster. I'm not the most efficient or best code monkey, as I would say my skills are more on the hardware side.
```

---
## \#155 Posted by: Winfly Posted at: 2019-05-19T17:35:10.312Z Reads: 111

```
I'm signing up for testing if you need any.
```

---
## \#156 Posted by: totalgeek9224 Posted at: 2019-05-19T17:51:42.290Z Reads: 113

```
Seconded. Would love to aid this project in any way possible
```

---
## \#157 Posted by: SimosMCmuffin Posted at: 2019-05-19T17:58:13.008Z Reads: 112

```
Thanks guys.

Personally I currently see the biggest risk against getting the BMS shippable to testers being the code at the moment, but I suppose at this point as I don't have any products to sell yet it's just how it will be. Once I can get some additional income I can maybe start looking into getting someone dedicated for the SW side or look into other solutions.
```

---
## \#158 Posted by: totalgeek9224 Posted at: 2019-05-19T18:03:26.036Z Reads: 111

```
Maybe someone from the community could help with the SW? How easy is it to flash onto the boards? If it's easy, then as the software improves, users can easily reflash.
```

---
## \#159 Posted by: SimosMCmuffin Posted at: 2019-05-19T18:27:22.093Z Reads: 115

```
You can reflash with a cheap 2$ ST-link clone. In fact I use one to flash and debug.

![IMAG0284|690x287](upload://d5nKatBENq3o4D7IWJOwGii5alb.jpeg) 
![IMAG0285|690x473](upload://mPWwG4E8kwaNggUv6sQAeDJnORl.jpeg) 

The 4 test pads on the bottom are 3V3 & GND for power and SWDIO & SWCLK for serial wire connections. Reset test pad is also available on top side (no space on bottom side). I plan on building a jig with pogo pins that I can just insert the board into and it will make the connections to the test pads for production flashing and testing. Probably gonna have pogo pins on top and bottom.
```

---
## \#160 Posted by: SimosMCmuffin Posted at: 2019-06-02T11:58:46.047Z Reads: 113

```
Update.

We are charging!

![IMAG0295|690x389](upload://5B5UHcwdmAUvFTtE1LYIu8YM5My.jpeg) 

First charges going through the BMS now, got the FW sorted out so I can implement the basis for the charging control, not finished but ready for testing as I am doing atm. 

I'm going to now focus on getting the prototype PCB+assembly test batch underway, alongside a debug/flashing jig, so I don't need to use or attach the dangling debug wires onto the BMS.

On the FW side, I think I'm going to implement a communications frame for the USB-UART interface, so I can change the parameters on the fly. After this would be making the EEPROM simulation, so I can save the parameters to flash memory for non-volatile storage.
```

---
## \#161 Posted by: ducktaperules Posted at: 2019-06-02T12:44:06.868Z Reads: 111

```
If you want anyone else to help with testing one of these then let me know. I have spare 12s packs that i could use and have a programmer to upload new firmware's if/when you make changes. Also willing to cover the hardware cost.
```

---
## \#162 Posted by: janpom Posted at: 2019-06-02T19:28:19.049Z Reads: 111

```
I also volunteer for testing. I like the project a lot. This is exactly the kind of BMS I'd like to use. I'm a software engineer and could help out a little bit with the code. I'm pretty swamped at the moment, so I don't think I can contribute a lot of code but I could do a code review and/or help debug things. I guess that's only relevant if you plan to make the code open source, which I'm actually not sure about.
```

---
## \#163 Posted by: SimosMCmuffin Posted at: 2019-06-03T11:19:24.563Z Reads: 109

```
Made the little debug connector for the test pads using spring loaded pogo pins for the connections. Gonna check the MFG files today and send them for cost quotes from  a couple of fab houses.

https://www.digikey.fi/products/en?keywords=ed8184
![image|500x500](upload://hLKKnJAYkFnpATWbyLd4xbgkWsG.jpeg) 
![image|617x500](upload://7Osj69dYIDOVHtb0zEabMyUmeh7.jpeg) 

@ducktaperules will do once I start getting hardware from the fab houses.

@janpom Appreciate the offer, but I'd rather say that I'm looking for someone dedicated to take-over the FW/SW development, because my roots are in the HW arena and my personal code development and train of thought is highly un-ideal for collab code development. I'm a bit embarrassed to say that, but I think say that it's a more realistic statement knowing myself. It's my personal shortcoming.

I can take care of HW development, testing, sourcing and manufacturing, that's where I'm comfortable at and I feel that the project could proceed more efficiently with a dedicated SW/FW developer/leader to develop/manage the open-source code. I'm not demanding anyone to step up and take the whole weight of the code development on their shoulders, but rather help me at least setup the environment for the open-source SW development and help manage it.

I mean, the HW team at the office is working at the office next to a part of the SW team, but I don't know what the SW team is doing most of the time. I'm atm busy with a new customer project that I'm handling the whole development process for apart from EMC testing (papa bless our HW team leader :pray:). I'm designing the HW, making the MFG files, communicating the the fab house and the customer about sourcing and testing and writing the standard SW that the devices will at the beginning be shipped out. 

There are already more features requested from the customer side and we have now included a 
semi-dedicated SW guy for the project, but the problem is that I don't follow the same coding guides as the SW team is following, so most of my code is likely going to be thrown out and at that I feel that the SW guy should just take over the code development. I'm comfortable with low-level code and even starting to do stuff through a HAL makes my head spin, as I feel that it's obfuscating the code for me.

If someone wants to step-up for the code development manager/leader, I believe we can workout some sort of payment deal if/when the BMS starts to ship. Log your hours and then get % of sales profits until you've gotten your payment fulfilled or some sort of other deal.

I'm a 27 old guy who wants to work as an entrepreneur, build and sell cool stuff, so I'm still learning new things. Accounting, salary and possible employees are still new things on the entrepreneur side. Life is so much easier when you are employed and those things are largely taken for you, but I'm often bored and frustrated at my job and I want to start steering my career towards my company. I also want to get more going on mechanical products, but don't have the equipment and space at the moment.

Maybe that went a bit on the venting side, but I think a lot of real talk/writing was done.

Papa bless ya all :pray::weary::100:
```

---
## \#164 Posted by: janpom Posted at: 2019-06-03T11:28:30.663Z Reads: 105

```
I think I would really enjoy working on it, but unfortunately I don't have the time now since I'm already juggling a full time job and a project of my own. I might be available in November, but I hope you can find someone else earlier since I really want this BMS. :slight_smile:
```

---
## \#165 Posted by: totalgeek9224 Posted at: 2019-06-03T12:00:00.706Z Reads: 104

```
Maybe @JTAG would be willing to contribute?
```

---
## \#166 Posted by: JTAG Posted at: 2019-06-03T12:18:48.464Z Reads: 105

```
The hardware could have been made compatible with the firmware, but it isn't :frowning:. Now its a pain to match it and keep it mainline. So I am afraid its hard to do.
```

---
## \#167 Posted by: janpom Posted at: 2019-06-03T12:23:59.559Z Reads: 105

```
How hard would it be to make the hardware compatible? Isn't that less effort than developing the FW from scratch?
```

---
## \#168 Posted by: SimosMCmuffin Posted at: 2019-06-03T16:45:45.218Z Reads: 101

```
Way too different HW for easy port. Different MCUs too.

I think for now the more realistic approach would be that I'll get the manufacturing sorted and then write the FW to be usable for a start. Then as the first BMS' get shipped out to testers, see if somebody has time to to start improving or making a clean start.
```

---
## \#169 Posted by: SimosMCmuffin Posted at: 2019-06-04T16:25:23.556Z Reads: 111

```
A good learning opportunity came up at the office.

I decided to embrace the SW collab coding experience and try to absorb as much as possible of how to do collaborative coding. We setup the Git environment today for the customer project with the SW guy and I admitted that I'm a bit new to this, so expect that I will be asking some questions about the process along the way.

---

On Monday I also found some weird behavior while charging via the BMS. Something was causing the USB comms to freeze when the FET bridge switched on to start the charging. Windows didn't play the unplugged USB device sound so it didn't disconnect on the PC end and it still showed the COM port in the device manager, but the serial communication froze (no more data coming to terminal), so clearly something weird was happening there. 

I'm not also sure if it's the MCU's USB driver getting stuck in a some sort of error state, but disconnecting and connecting the USB cable into the BMS and re-starting the serial terminal got it back going. Un-plugging USB makes the MCU's SW shutdown the USB driver and restart it when USB 5V comes back present, so possibly that clears any error states. the MCU still continued normal operation apart from the USB hiccup.

Talked about it with my colleagues in the HW team about the possibility of some kind of ground loop effect happening on the switching moment, but they didn't have any clear-cut answers on that. Really the only thing was to start measuring around and see if the USB voltages jump around during the switching moment. I also noted that the disconnect only happened when the 10S battery pack was under 39-40 Volts, but not above that. Maybe the charger gave a bigger current spike when the voltage difference was bigger and it got smaller as the pack filled up and the voltage difference got lower.

So I decided to check the current waveform from the brick charger I was using and oh my god... Below is an image from the current waveform measured with differential pair, what you want to look at is the purple line, which is the math result for probes 1 and 2. HUGE oscillation in the current at a 4 kHz frequency (which also explains the annoying whine coming from the charger). The voltage scaling for the purple line is 200mV/grid and the current sense OP-amp sensitivity with the used shunt resistor is ~250mV/Amp. The charger has nominal charging current of 2.2 Amps, too bad the current is oscillating from ~1-3.2 Amps (well there's that ~2.2 A average)! No wonder the serial terminal showed the charging current oscillating/jumping between 2000-2300 mA, it was correct and the 16x oversampling done in the ADC brought to those numbers! I decided to stop using the charger after that.

![IMAG0297|690x389](upload://bV8Yh1z8t8WvbzMxzmmD1ihqb66.jpeg) 

I then decided to compare it against my current workhorse charger and the difference was just clear as night and day. Again pay attention to the purple line. Sooooo much smoother power delivery compared to the one above. The serial terminal current value now only lives at around +-15 mA, which seems accurate with some measuring noise. Couldn't get the USB to disconnect with my charger setup.

![IMAG0298|690x389](upload://alMlZ80zQ1cFNSt3SNERucNybIs.jpeg) 
![IMAG0268|690x341](upload://5LPFH5QsTBPfzpZT3uhmI0DXJe8.jpeg)

So I don't think I'm going to implement any changes to the USB connection for now, as I would chalk this up to the brick charger being just bad quality. Gonna have to see if anybody else has this problem when I ship the first test boards out. 

Note, it was not a chinese cheapo charger, but a brand name device (link below)

https://www.digikey.fi/product-detail/en/mean-well-usa-inc/GC120A48-R7B/1866-1748-ND/7703243
```

---
## \#170 Posted by: Hummie Posted at: 2019-06-04T17:09:12.569Z Reads: 100

```
How will the fluctuating voltage and current effect the charging temporarily or battery long term
```

---
## \#171 Posted by: Darkie02 Posted at: 2019-06-04T17:42:00.446Z Reads: 104

```
[quote="SimosMCmuffin, post:169, topic:85493"]
Note, it was not a chinese cheapo charger, but a brand name device
[/quote]

Now I’m wondering what my go to option in charging and power supply’s are like. I always gone with what I know others people have tried and tested and just believed thay were quality. any idea on the ones in the link below?

https://www.meanwell-web.com/content/files/pdfs/productPdfs/MW/HLG-320H/HLG-320H-spec.pdf
```

---
## \#172 Posted by: Hummie Posted at: 2019-06-04T18:11:58.619Z Reads: 105

```
Ac Ripple in the dc charge no good.    https://reader.elsevier.com/reader/sd/pii/S030626191630808X?token=D7FCBE14A5C1F0DD1F86672E27FA4B33FA9E29F6972C027AE12FA9C6AA0BED3249CD8B7ED886ACD88F053AD2F0478BBE    But maybe if u turned all the lights on or off in the building ur charging it could be smoother. Maybe there’s a mod.  I’d think be easy to smoothen w bigger bits installed. Caps n coils.
```

---
## \#173 Posted by: SimosMCmuffin Posted at: 2019-06-04T18:33:08.019Z Reads: 111

```
I am using one of Mean Well's LED drivers for my DIY ceiling light with dimming control and haven't had any problems with it.
"HLG-150H-15B" to be exact

https://www.digikey.fi/product-detail/en/mean-well-usa-inc/HLG-150H-15B/1866-2360-ND/7703916

Thing is able to go bright AF (low-medium power in pic), there is an external potentiometer in the middle of the bottom part, so I can adjust the brightness. The center part is my custom 3D-printed part.

![IMAG0299|690x389](upload://eXSvjkN7eaZKH4mvi3ezGuMWMOO.jpeg)

As a basis I don't see a problem using a LED driver to charge battery packs especially if other people have reported success with the particular model, but these days I will usually test the performance of power supplies to validate the datasheet numbers. 

I'm just disappointed in the "GC120" battery charger series' performance in particular from them (the terrible current waveform earlier was from that), I mean my custom charger/PSU uses a Mean Well PSU (ENP-360-48) to feed the DPS5015 buck converter and seems like a decent item.

![IMAG0300|690x389](upload://6ObPEqRDyyctk6TtwSctOjcp0dv.jpeg) 

General opinion of Mean Well power supplies in the HW team is that they have often been a problem component in EMC compliance.

I think the quality is just very series dependent if they're good or not, but they are one of the cheaper PSU brands on the market.
```

---
## \#174 Posted by: ducktaperules Posted at: 2019-06-05T10:35:30.992Z Reads: 111

```
i have just brought one of these which arrived yesterday so once i get a chance to test it i will report back :slight_smile:
```

---
## \#175 Posted by: SimosMCmuffin Posted at: 2019-06-05T17:03:14.661Z Reads: 111

```
I'm also interested how the voltage and current waveforms look like under load,
```

---
## \#176 Posted by: SimosMCmuffin Posted at: 2019-06-09T16:50:44.334Z Reads: 112

```
Getting the ball rolling.

![image|595x500](upload://nqaHLVrhxHu5JtXq9MzhJWzr2Dm.png) 

Note, that is not the final price for the prototype batch, doesn't have the LTC6803 for example included yet, as their automated BOM reader couldn't get the prices for a couple of components. They say they'll give the correct final quote within a working day.

First time I'm ordering assembled boards from China. And this isn't exactly the easiest starting point board complexity wise, but you have to take the first step at some point.

----

Friday was a pretty interesting day at work. Went to the local pcb assembly service provider and saw the first boards getting assembled for the customer project and the fine tuning with the paste application machines and pick-n-place machine. Only assembled 1 panel first (4 boards per panel), which we then checked that it came alive (checked voltage regulators and tested flashing the MCU). Seeing that everything seemed to be in order we gave the okay for the assembly line to run the rest of the batch (50 panels in total for 200 assembled boards).

After that it was time for quick software tuning, as the board's hardware setup had changed, to make sure the basic functions were working. Then we went to see the production line test jig house upstairs of the from the assembly space/hall. Their device's job is to flash the customer board and run a hardware test on it to see that everything works. I then spent roughly 4 hours with the test jig makers getting the tester code to work with the test mode running on the customer board. One of the original measuring setups didn't work out-of-the-box so there was some trial-and-error testing couple different measuring circuits to determine if the customer board was working properly. Luckily at the end of the day, we found a workable measuring setup that could be used to test the correct function of the specific part of the board that was the problem.

Can't post a picture of our test jig, but here's a couple close ones in appearance from the tester company's website.

http://www.testnova.com/galleries/gallery1/galleryimage_12.jpg 
http://www.testnova.com/galleries/gallery1/galleryimage_19.jpg

Essentially it's a bed of nails. You put the board into the jig and then pull lever and it then closes the top part downwards pushing the board onto the test nails coming through the bottom of the tester. The nails then make a contact onto the test pads on the bottom of the DUT (Device Under Test) board. In the bottom part of the tester is a whole assortment of measuring and testing devices, which are then connected to the nails.

The testing device was then connected via an USB to a PC that was running the testing company's own proprietary testing software with their own developed testing script language. After putting a board onto the jig and closing it, you would scan a QR code sticker put onto the board and the test software from there would automatically start the testing sequence, the QR code is used to track the manufacturing day and batch of the board and will be put into a database. There are multiple steps in the script and they are given a PASS or a FAIL depending on if the device passes the particular test. 

for example the couple first steps on the script was:
- current consumption after powering-up
- flashing firmware to MCU
- getting baseline numbers from multiple outputs.

All these numbers needed to be withing a certain range or they would fail the test.

It was **QUITE** a stressful day, as I was the guy who had designed the boards, made the manufacturing files and done the software, so the whole stack was sort of resting on my shoulder. There wouldn't be anyone else to point blame to except me if something was **FUBAR** design wise. But stressing doesn't really achieve anything so I just took everything as it came and looked at the problem situations through a chill mood.

_I did then go and buy a 1.2kg (~3 pound) strawberry gateau cake and ate it by myself on Saturday :blush::yum::joy::pray::100:_
```

---
## \#177 Posted by: Friskies Posted at: 2019-06-09T17:54:21.837Z Reads: 105

```
Nothing beats buying yourself a cake and eating it too. Well done mate. Let me know when they are ready to buy and I will throw my money at you :stuck_out_tongue:
```

---
## \#178 Posted by: pjotr47 Posted at: 2019-06-09T21:02:41.357Z Reads: 113

```
Yowdie guys,

It is not fully about this bms, but I think it can do something good.
At this moment some off us are using charge only bms's. That means that the power from the cells go most off the time to a antispark.

Due this and not setted correct cut off voltage you can kill the cells. Or due a bad cell group you can kill also such a group.

Those charge only bms's have most off the time also a output. When a group or the total voltage is below the cut off it will cut the output voltage to around 0v.

Should there be a possibilty to create a small controller to set between the output and the antispark. So the antispark should power off or you don't even gonna have the chance to power it on.

I hope you understand what I mean
```

---
## \#179 Posted by: janpom Posted at: 2019-06-09T21:29:40.136Z Reads: 108

```
Makes sense. A better and a more generally applicable approach would be to signal directly to VESC. The VESC would then be able to shut down in some reasonable way (without throwing you off the board). That would of course require updates to the VESC FW but doesn't seem hard to do.
```

---
## \#180 Posted by: Pedrodemio Posted at: 2019-06-09T23:39:27.479Z Reads: 110

```
This. there is no reason for the BMS cut power to the entire board

If we get low voltage on a cell, make the thing beep like crazy and tell the vesc to only allow braking
```

---
## \#181 Posted by: Friskies Posted at: 2019-06-10T04:55:57.592Z Reads: 110

```
This isn't something that just the BMS can do. You would need to re-write Vesc firmware too. Whilst I think that it's a great idea I think it is a bit much to ask for in this particular case. Also charge only BMS are wired to bypass the BMS completely when discharging; they don't do any kind of cut off when the board is operating. This is done by most riders as they normally prefer dead cells than broken bones.

In saying that this unit should be compatible with the Metr app and I was going to ask this anyway. @rpasichnyk is it possible to create an alert option for this BMS/diebie that can alert your phone/watch when there is a P group voltage varience above a set value?
```

---
## \#182 Posted by: Pedrodemio Posted at: 2019-06-10T18:47:28.697Z Reads: 104

```
Yeah, is one more complication

For me personally if the BMS balances the cells, and beep following some pattern (one beep low voltage, two beeps one cell bellow the average, etc) is already perfect, if it manages to tap into the CAN bus and show cell voltages in Metr is a plus
```

---
## \#183 Posted by: SimosMCmuffin Posted at: 2019-06-13T09:22:47.427Z Reads: 107

```
Seeed has now completed their BOM sourcing and shown below is the finalized quote for the 5 boards. I'll confirm and pay the order today.

![image|690x406](upload://8NQHxEJhOWX6ypYa5E8M4dGFjtQ.png) 

---

I don't personally see a problem implementing the cell voltage broadcasting on the CAN bus on the BMS end, but I haven't looked into implementing the VESC end FW changes and then adding the support Metr.
```

---
## \#184 Posted by: rpasichnyk Posted at: 2019-06-13T12:31:52.113Z Reads: 115

```
[quote="SimosMCmuffin, post:183, topic:85493"]
but I haven’t looked into implementing the VESC end FW changes
[/quote]


If you keep the same packet structure as DieBieMS and assign yourself same CAN ID (10), it will just work :+1:
```

---
## \#185 Posted by: SimosMCmuffin Posted at: 2019-06-13T17:45:28.743Z Reads: 122

```
**Charger/charging related update:**

Received a Digi-Key order today and in it I got Mean Well's ELG-series LED driver that I wanted to try/test for battery charging after being disappointed in the GC120-battery charger serie. Shout out to @Darkie02 for the idea.

Specific model name is "ELG-150-54A", good for 10-13S packs voltage range wise. A-models have two trimpots to set the CC current and CV voltage.

https://www.digikey.fi/product-detail/en/mean-well-usa-inc/ELG-150-54A/1866-1491-ND/7702969

![image|690x367](upload://t3iZoKlz2ucQIqAQ8JCfgu9TQcV.png) 

The charger comes without any connectors on the input or output side, just tinned wire leads, so I connected an IEC-mains connector that I have many cables available for the input side and soldered a XT60 to the output end.

![IMAG0309|690x424](upload://zd8DI7uOLv8cJthrwHrgrGvtV9G.jpeg) 
![IMAG0311|690x395](upload://pm0U0fal7o1LkcX06G7jmd0TlbH.jpeg) 

Charging.
![IMAG0306|690x389](upload://tvZr6FnloFmuIMei9iAHT6lsYnW.jpeg)

The two trimpots for the CC and CV control are located on the bottom side and the holes have a rubber plugs for ingress protection. The trimpots are located at the bottom of those access holes, which are surprisingly deep.
![IMAG0307|690x423](upload://pLioioqZnVGnL4CAFFkSdQbx8Hb.jpeg) 

So how's the actual performance? Very impressive actually. Very little noise on current or voltage waveforms on the output. Differential measurement, purple line shows the actual current waveform.
![IMAG0308|690x389](upload://1F6e0LQEKJBGuSxzKoezwxUrD8e.jpeg) 

FLIR image of the full metal case at around 38 Volts @ 2.6 Amps (~100 Watts). Case feels hot to the touch as the metal case transfers heat well.

![Screenshot_20190613-195248|281x500](upload://i7sXuUuETy9aLcPT7ThjcuBfV37.jpeg) 

Personally I would say that this LED driver is good for charging use. Just make sure that your charging controller/BMS **CAN** cut the charging if you're operating in the CC region.

My particular unit's CV range via the trimpot was 45-59 Volts and CC range was 1,1 - 3,1 Amps

**EDIT:** I managed to get the output current to start oscillating (**bad**). After setting the output current to around 2 Amps and starting the charging, I noticed that the output current started oscillating. If I changed the CC current while charging, it would stabilize, but after un-plugging and re-plugging the charger back it started to oscillate again. It exhibits this behavior within a certain CC current range which for me seems to be about 1,1-2,5 Amps. So if I crank it to the minimum CC current of ~1,1 Amps it's stable and if I put it above 2,5 Amps it's also stable. Changing the CV voltage had no effect. **Just a heads up.**

![IMAG0312|690x389](upload://3iawS0d2gsJHW9mK4I8OMKPteSm.jpeg)
```

---
## \#186 Posted by: ducktaperules Posted at: 2019-06-15T22:40:51.399Z Reads: 111

```
This is super interesting. How much oscillation is occurring? I can't see any scale or reference for the current trace on your scope?

I recieved my meanwell led driver last week and it seems to have been doing well so far. The cables are a little short but apart from that it's good. I got the 7A version and my BMS is happy with it at both the highest and lowest current settings. The current output seems stable when viewed from my BMS app but I can't imagine that's got a good sample rate. You've got me curious now to see if I can get mine too oscillate so I may try and stick a scope on it if I get some free time next week.
```

---
## \#187 Posted by: deucesdown Posted at: 2019-06-16T06:40:06.805Z Reads: 108

```
@Hummie waveforms
```

---
## \#188 Posted by: SimosMCmuffin Posted at: 2019-06-16T09:19:22.712Z Reads: 111

```
The purple waveform for the math function has 200mV/grid voltage scaling, so I would estimate that the current waveform voltage is jumping between ~380 to 720mV. Current measuring sensitivity is 250mV/A, so current is jumping between 1,5 - 2,9 Amps.

My BMS' ADC configuration currently has 16x oversampling and 16x division done on the hardware. 4 MHz ADC clock, 12-bit sample depth. This gives us ADC clock period of 250ns, 12-bit conversion time = 12,5 ADC clocks and I'm using sample time of 92,5 ADC clocks, so 105 ADC clocks in total for the whole sampling + conversion. 1 sample + conversion time is ~26µs, so the whole sequence would be 420µs (:pray: ayoooo) and then those samples would get averaged.

[quote="ducktaperules, post:186, topic:85493"]
I recieved my meanwell led driver last week and it seems to have been doing well so far.
[/quote]
What model and where did you get it from?
```

---
## \#189 Posted by: ducktaperules Posted at: 2019-06-16T20:44:21.166Z Reads: 109

```
I got the HLG-320H-48A and i just got it from Amazon so it would be here next day.

![IMG_20190616_213302|666x500](upload://kRV0kmsszxN7tAG381FmGj1xiez.jpeg) 

One things that annoys me is that the cable is to short for it to sit on the ground.

[quote="SimosMCmuffin, post:185, topic:85493"]
CC range was 1,1 - 3,1 Amps
[/quote]

Seems like i also get slightly larger CC range that the "rated spec". Im measuring from 2.8A up to around 7.6A.

![Screenshot_20190616-213505|281x500](upload://kpl47eZem9I5H8sVcFP6EmS7X7h.jpeg) 
![Screenshot_20190616-213436|281x500](upload://uAVRL9MAVZ8xzhWkrQw3F6cCh0A.jpeg)
```

---
## \#190 Posted by: SimosMCmuffin Posted at: 2019-06-17T07:02:44.431Z Reads: 103

```
Maybe I should order one of them as well.... a bit pricy though.

https://www.digikey.fi/product-detail/en/mean-well-usa-inc/HLG-320H-48A/1866-2490-ND/7704048

I think I'll order the 150 Watt one instead for testing.

https://www.digikey.fi/product-detail/en/mean-well-usa-inc/HLG-150H-48A/1866-2377-ND/7703933

Might be that the HLG-series' current control loop is a little bit different compared to the ELG-series resulting in a more stable current behavior.
```

---
## \#191 Posted by: SimosMCmuffin Posted at: 2019-06-17T18:06:48.408Z Reads: 105

```
Would anybody happen to be able to recommend Trampa mountainboard truck compatible motor mounts? Let's just say a little something something happened on the way back from work today...

![IMAG0313|690x389](upload://vXXf6srwdbBaLr8iha9hXkun6TI.jpeg)
![IMAG0314|690x389](upload://7BDYG4Q9RnyVhjOHvpWicDPMB9A.jpeg) 
![IMAG0315|690x389](upload://wMhc0OyQU9Hbmyq7NGzpb3omwJX.jpeg) 

Luckily I was able to come to a controlled stop, so I'm fine. Motor mounts were from @UnikBoards  and probably had 4000+km on them. Hadn't really checked them over closely at any point so no idea when the metal had started to fatigue. I checked my email for the date when I had purchased them and it was on May 2017, there was also a notification email from them/him:

    Nov 29, 2017,
        
    Hello

    We had a return on a faulty engine mount (twisted with use)
    Take the time to watch and inform me if this is the case for you. A standard exchange will be done directly.

    Sorry for the disagreement

Had completely forgotten about that.

![IMAG0318|690x389](upload://mZpIHAN5Q4JK1cP1s1dN0SBhWo6.jpeg) 

Motor seems to be fine, except that I'll have to to true the rotor bell, as it's currently a bit offset angle wise causing it to rub against the stator teeth. Also cleaned it when I had it apart.
```

---
## \#192 Posted by: Arek Posted at: 2019-06-22T20:19:15.861Z Reads: 102

```
@Idea is the man, look at this mechanical porn!:
 ![IMG_20190212_231500|690x388](upload://k0ZUD4XC4D708qyLZMFM5bbMSIn)

@ducktaperules For mine I 3D printed some handling-friendly covers also replaced original cables for longer ones:
![IMG_20190622_212804|690x388](upload://jpTS3VYtQgNPk8FNttTPDTBxSl6.jpeg)
```

---
## \#193 Posted by: SimosMCmuffin Posted at: 2019-06-23T11:16:55.002Z Reads: 101

```
I ordered a set from @Marsl187

https://www.electric-skateboard.builders/t/motor-mount-for-trampa-spring-trucks-infinity-vertigo-hypa-pulleys/96708 

----

I also finished prototyping the test jig for the SWD connector.

![IMAG0321|690x389](upload://3NJfVzoBey7S77mN1TuFcLuyUXw.jpeg) 
![IMAG0326|690x391](upload://h29U9f88hQNbddXoP6k6oCheeSZ.jpeg) 
![IMAG0322|690x411](upload://lLNs5KZjhuh53CPiqkSwYoc4eET.jpeg) 
![IMAG0323|690x446](upload://hLbbTmYJKgAiZo5Ti9G9qX5ULHG.jpeg) 
![IMAG0324|690x336](upload://mE6IjoMWiXsJcqXzdrQJwLTkiB2.jpeg) 
![IMAG0325|690x433](upload://qBYlQS2AfqzLaIGQWeRXDe2V2xY.jpeg) 

Simple enough and seems to work. Maybe need to put Nyloc nuts on the backside for the holding tabs, as the bolts start to work themselves loose when you turn the tabs back-and-forth.
```

---
## \#194 Posted by: Darkie02 Posted at: 2019-06-25T09:13:56.189Z Reads: 88

```
[quote="SimosMCmuffin, post:190, topic:85493"]
I think I’ll order the 150 Watt one instead for testing.
[/quote]

Any update on testing and your verdict on the HLG or as work got in the way of playing again? 🤔 has any one made a esk8 national holiday yet for more building time.
```

---
## \#195 Posted by: SimosMCmuffin Posted at: 2019-06-25T10:43:52.846Z Reads: 89

```
Funny thing.

I literally submitted my digi-key order 2 minutes ago with the HLG-150H-48A and then popped in here to check if I had any new notifications, so yes I'll making a post about it at some point soon.
```

---
## \#196 Posted by: Colydog Posted at: 2019-06-28T05:04:07.911Z Reads: 93

```
Bit of background I'm an electrical engineer but I work mostly in PLCs, contractor logic and high voltage transmission, so my solid state electronics knowledge isn't that crash hot. 

My question is what is the fundamental difference between this BMS and say a D140, that allows it to be so much smaller and pack in so many more features, than other BMS on offer? 

This thing looks like the holy grail of charge only BMS and I'd be really interested to help develop it if I can.   

Thanks 
Colin
```

---
## \#197 Posted by: SimosMCmuffin Posted at: 2019-06-28T11:52:40.605Z Reads: 95

```
[quote="Colydog, post:196, topic:85493"]
what is the fundamental difference between this BMS and say a D140
[/quote]

For reference, I assume you mean the Bestech D140 BMS 
https://buildkitboards.com/products/bestech-d140-charge-only-bms

[quote="Colydog, post:196, topic:85493"]
My question is what is the fundamental difference between this BMS and say a D140, that allows it to be so much smaller and pack in so many more features, than other BMS on offer?
[/quote]

After taking a look at the product pictures for the D140, I have couple of notes that I made on the key design differences.

---

The D140 BMS is very, very simple. No programmable logic, everything is passive/non-programmable. Around 9-11 unique components, most likely super cheap price wise, I'm guessing around 2$ for all the passives/non-programmables, 1$ for the FETs and couple cents for the connectors. It's built down to price and then made in big volumes. Pretty sure they have good margins on it, or at least re-seller has.

One sided component placement. Con, this means that you need more board size/space to be able to fit an equivalent amount of parts. Pro, cheaper assembly costs, due to needing to run board through SMD line only once, where as dual side component placement board needs to be run twice through an assembly line, once for each side. Interestingly they still opted to use through-hole FETs... I guess labor is cheap(er) in China.

Lack of good competition on the low-end BMS market (or higher end for that matter). Why try harder if you don't have anyone to compete against and/or your product is selling well.

It's a cookie cutter copy topology from their other designs.

Low-side load switch topology.

No comms of any sort. No any sort of indication of charging or balancing on the board either, or at least I didn't spot any led anywhere.

---

The approach for the design of the FlexiBMS Lite was not price driven, but rather feature driven. When I started this thread I had an idea in my head for the feature set that I then presented to the forum for feedback. From there the design changed and evolved along the feedback and feature discussion. 

Once the wanted features were selected and "locked in" I then started to check what the most economical approach component selections wise was to still fulfill the wanted features. Alongside the component selection I'm doing the schematic and layout design and seeing how much board space I have and If I can fit everything or even shrink the board down in size.

My BMS has a lot of high performance components with a good feature set. The board is designed from the get-go with semi-high integration density and uses a 4-layer PCB to be able to route everything. There is just a different design ethos between these two boards, mine is feature driven without so much priority on price, where as their's is minimal features with priority on minimal cost.

I want to make a cool product, not necessarily the most profitable one, but I think making cool things will always draw *some/more* attention/customers then just making a dime-a-dozen product.
```

---
## \#198 Posted by: SimosMCmuffin Posted at: 2019-06-30T15:15:55.339Z Reads: 94

```
Got the **Mean Well HLG-150H-48A LED driver** and did a number of tests on it. It's outer dimensions are all a bit bigger compared to the equivalent power ELG-serie driver.

![IMAG0343|690x445](upload://rF70TDnaWdrclR6tsl1QHbcXxmm.jpeg) 

![image|690x470](upload://pq7GIksfnkNuCMl01TAQTJ53Vj7.png) 

Measured ranges on the Vo & Io trimmers for open voltage and output current were (measured with Maynuo M9711 DC load):
- Vo: 41,6 - 53,6 V
- Io: 0,99 - 4,00 A

Made a little IEC-power cable adapter with a built-in power switch for easy on-off control.

![IMAG0337|690x485](upload://ryJFLvcAceiKjr6dlqM47RCAIpD.jpeg) 
![IMAG0338|690x461](upload://rPszaR6EoUcqwrI7RHH4vQJv3n7.jpeg)
![IMAG0339|690x483](upload://gHTQlJrs8O3Ez1SeqkkitdHqRoX.jpeg) 
![IMAG0341|690x246](upload://j7T7ZC4qxW4lUOyElKGUXEN52f8.jpeg) 
![IMAG0342|690x444](upload://gxiLv9nc28rtXwBKSOi5vta6lCE.jpeg) 

Onto the measurements and oscilloscope current waveforms. The sensitivity/division for the current/purple waveform is 200mV/div and the current measuring circuit outputs at 250mV/A sensitivity. I have also noted the measured current values for the waveform on the serial terminal, these ADC results are calculated with a 16x oversampling & ~420µs sampling + conversion total time for all 16 samples.

I started measuring from the lowest possible Io current and then increased the current for each measurement seeing if there were any possible oscillating current ranges anywhere. I did not observe the same current oscillation behavior as with the ELG-driver with starting the charging in certain current ranges. 


1. Minimum current setting. 1,05 - 1,30 A. *not stable* due to current being so low and can be seen clearly turning the output on and off, resulting in the choppy current waveform jumping between ~ 0,4 - 1,7 A

![pic_236_3|690x414](upload://bUihSei6XPlbV8TzfGLNOdC8gQM.png)

2. 1,33 - 1,70 A. Still not completely stable, but the current is clearly starting to stabilize.

![pic_236_4|690x414](upload://c6tete9iDS2AzZTzACRVPn00CvC.png) 

3. First stable current. 1,83 - 1,92 A

![pic_236_2|690x414](upload://w5jy58laSzZR32nJvJ3QdTcUTgS.png) 

4. 2,45 - 2,53 A

![pic_236_5|690x414](upload://3snN8HhXw8HqgyHntXbFJZRBNzz.png) 

5. 2,96 - 3,06 A

![pic_236_6|690x414](upload://g5n2PJOSPnRMypAvfLcWmYhUeJK.png) 

6. 3,49 - 3,59 A

![pic_236_7|690x414](upload://mWo53Jg0OVpFl2pNCipEKQC2SD8.png) 

7. 3,94 - 4,03 A

![pic_236_8|690x414](upload://30DUGa6ED3VAhzp0cjMlntyUbSE.png) 

8. Current waveform when limited by Vo output voltage, slight oscillation can be seen but it's pretty tame in amplitude (~300-400mA) and low in frequency (~110Hz), so I don't see this as a problem.

![pic_237_1|690x414](upload://msQhQRclXIIHthDIE31ZToK0jsG.png) 

FLIR image after charging at 160+ Watts for 15 minutes (4 A @ 40+ Volts), runs cooler compared to the ELG-serie as that was externally at 50C with only ~110 Watts of power. Note the caveat that the ELG-driver was meant for one step higher voltages, so this isn't pure apples-to-apples comparison in that sense.

![Screenshot_20190630-170006|281x500](upload://f3r4GAjIpOoJhX1xy285ELAapKj.jpeg) 
![Screenshot_20190630-170021|281x500](upload://x2Un8Ne0v6jZYg6aAlzoaKyv4Qd.jpeg) 

**Summary**

I'm glad that I decided to test this charger, as it will become my go-to charger based on my testing results. Current output behavior was good apart from the chopping action at minimal output currents. Thermally it seems to perform superiorly in terms of actual output power when compared to the ELG-driver that I tested earlier, even though both are rated for 150 Watts of power. Although you might not necessarily want to push that 4 Amps if you're on 11S or 12S packs, but seems to perform fine with 10S.

I think it's possible to add a feature to the FlexiBMS for detecting charging current oscillations, so you can see if your charging is outputting clean current and protect your batteries from bad chargers or at least be informed that the current is oscillating.

--- 

*Off-topic*

Got mah new motor mount kit from @Marsl187 , I'm still waiting for my new gears and belts, so a little break for now from boarding. Kit seems to be good quality and well priced for the 130€ that I paid for the parts and shipping in total. I gave him some feedback on the design to improve them in case he wants to start making more of them in the future.

![IMAG0330|690x389](upload://hmAHzcDWLcxkREU1SaoAaYt5ebj.jpeg) 
![IMAG0331|690x389](upload://8SW3qWHTs2EDvRIbv2RPdiVW59Z.jpeg) 
![IMAG0333|690x389](upload://4rRDmv217AKORMKAjZX6kKb2JFM.jpeg)
```

---
## \#199 Posted by: totalgeek9224 Posted at: 2019-06-30T18:59:00.749Z Reads: 87

```
Love the design and through testing. May be worth integrating a fuse in that print of yours, just to ensure the longevity of the driver.
```

---
## \#200 Posted by: Darkie02 Posted at: 2019-07-01T07:08:20.927Z Reads: 87

```
As a thort is it possible to implement a fuse on the charge side. in case any one shorts the charge plug. Iv been using a automotive 7.5A 58v mini blade fuse and just stuffing it in the case.

![image|281x500](upload://yw30F19QPuivyAf6YMyuPUqRIeu.png) ![image|281x500](upload://mlz5ps8AWs7A3MGdvkJLSLo60sK.png) ![image|281x500](upload://m7CAhgWyQ4TaxhaeZdL5zi4Y4p8.png) 

Or software to limit the input max voltage and amps of the charge? 

Seen people talk about using there 12s charger on the 10s board by mistake or dropping a coin and shorting out the charge point with a huge flash.
```

---
## \#201 Posted by: totalgeek9224 Posted at: 2019-07-01T08:46:44.350Z Reads: 85

```
A fuse on the charge side should be implemented nonetheless, what I was rather suggesting was a fuse before the charger, to alleviate any possible issues due to power surges or something similar
```

---
## \#202 Posted by: Darkie02 Posted at: 2019-07-01T09:45:30.316Z Reads: 81

```
I’m getting a little confused 

Fuse in the 3d print I think is irrelevant to some people as some countries have fuses in the mains plugs. Those that don’t i was under the impression that the sockets are rated to the supply circuit protection at the board. A fuse is  officially only needed on the supply to be rated to protect the cable to the the device not the device it’s self according to my local standards.

Fuse on the load side of the charger is not needed as the HLG has overload and short circuit protection built in.

Fuse on the charge input side of the board close to the battery as possible is what I was referring to most BMS have full battery voltage at the charge terminals all the time unprotected so a short there will cause the battery to overload and thermal runaway. Same if some one plugs in a way to powerful charger for the battry.
```

---
## \#203 Posted by: SimosMCmuffin Posted at: 2019-07-01T12:26:11.396Z Reads: 81

```
[quote="Darkie02, post:200, topic:85493"]
Or software to limit the input max voltage and amps of the charge?

Seen people talk about using there 12s charger on the 10s board by mistake
[/quote]
I have already implemented a basic max charging current limitation, which if crossed will shut off the charging fets, same for minimum/termination current. I'm currently checking if a charger is connected by measuring the charging port voltage and if it's higher than 0.5V then it means there is something connected, but should be no problem to also add a check that it isn't over a certain voltage.

Technically the charging port voltage should be at minimum near the battery pack voltage or lower than the specified max voltage. Then before switching on the charging FETs, check that cell voltages are ok and no breaks are detected on the balancing connector. Once those are true then we start charging and monitoring current and following their limits alongside monitoring cell voltages and balancing if possible/necessary.

[quote="Darkie02, post:200, topic:85493"]
or dropping a coin and shorting out the charge point with a huge flash.
[/quote]
This can't be protected against on the BMS, but the charger side fuse would help in this case. If this happened during charging the BMS would probably turn off the charging FETs due to either  minimum or maximum current limit being crossed, with the presumption that nothing blows up from the high currents.

I'm with @Darkie02 that the charger front side fuse seems a bit excessive. This being a LED driver it's meant to be installed once into a lighting fixture/installation and is meant to being able to take the powering on/off that you do when turning on the lights. There are no extra fuses, except what you have on your fuse board, or also in your power cables like in UK, but most likely it would be wired directly to the fuse board in permanent installations.
```

---
## \#204 Posted by: ducktaperules Posted at: 2019-07-01T15:23:43.384Z Reads: 72

```
It would be awesome if the bms had the ability to limiting current from the power source. This would mean that almost any powersuply could be "slowed down" to charge at any desired rate.

Also it might allow you to charge from other power sources such as other battery packs without needing a buck/boost type setup.

Additionally by monitoring the pack voltage and controlling charge current you can implement any desired charge curve, including adding features like stopping at 80% capacity whilst charging overnight then just topping it up to 100% less than an hour before you leave for work :slight_smile:
```

---
## \#205 Posted by: deucesdown Posted at: 2019-07-01T19:39:02.252Z Reads: 75

```
That sounds like a high energy cc/cv supply with a remote interface. :) maybe a very low current version could fit, for size and heat?

I'm gonna stop myself from a full thread derail, but maybe a dph5005 with bluetooth, with screen and controls removed, mounted inside between battery and charge port...
```

---
## \#206 Posted by: SimosMCmuffin Posted at: 2019-07-02T07:56:09.367Z Reads: 83

```
[quote="ducktaperules, post:204, topic:85493"]
It would be awesome if the bms had the ability to limiting current from the power source. This would mean that almost any powersuply could be “slowed down” to charge at any desired rate.
[/quote]

Don't think that is going to be a feature on the Lite version, because it isn't easy to implement. You need to go either active with a buck-topology or passive with current limiting resistors. Active needs more components and board space where as the passive needs less, but will generate more extra heat due to dissipating "excess" current. I've been through this with the first FlexiBMS iteration that had the boost-converter on it. Limiting factor for the power was the generated heat.

Would be more sensible to make a dedicated charge current regulator board for the charge port front side that you could add-on later.

[quote="deucesdown, post:205, topic:85493"]
but maybe a dph5005 with bluetooth, with screen and controls removed, mounted inside between battery and charge port…
[/quote]

That would probably be the easiest solution.
```

---
## \#207 Posted by: SimosMCmuffin Posted at: 2019-07-10T09:20:46.069Z Reads: 82

```
PCB assembly order update.

Me:

    Mon, Jul 8

    Hey,

    What's the status on fusion pcb+assembly order XXXXXXXXXXXXX ?
    Are the design files ok?
    Have you been able to procure the components? 

    Do you have any estimate when you would be able to populate and ship the boards?

Reply,

    Tue, Jul 9

    Dear Simo，

    I just looked into your latest order status, which shows that we have successfully received all the components. And I have stretched my very best to require our workers in the assembly line to finish the assembling by July 16. Hopefully, they can keep up the schedule and do not cause further delay. 

    If the proposed deadline is too late for you, please contact me directly and I will try if I can help you set up an earlier schedule for the production.

    Sincere gratitude in advance for your understanding and support.

    **Best Regards,**

    <b>Cecilia
    Seeed Fusion Support Team

Me:

    Wed, Jul 10

    Thanks Cecilia for the update.

    I was more interested in just what the current schedule was looking like and if you're able to assemble the boards on the 16th that would be great!

    Thanks for your help,
```

---
## \#208 Posted by: glyphiks Posted at: 2019-07-10T10:18:18.677Z Reads: 80

```
That's great news.definitely keen on trying out this BMS
```

---
## \#209 Posted by: totalgeek9224 Posted at: 2019-07-18T20:50:20.897Z Reads: 75

```
Any updates? This is one of the few reasons i come back to this forum :p
```

---
## \#210 Posted by: SimosMCmuffin Posted at: 2019-07-19T10:01:17.075Z Reads: 75

```
I sent Cecilia an email asking for a status update on the order.

Seeedstudio's webpage still shows order status as "Processing".
```

---
## \#211 Posted by: totalgeek9224 Posted at: 2019-07-19T10:40:04.604Z Reads: 75

```
Darn. How about on the software side of things?
```

---
## \#212 Posted by: SimosMCmuffin Posted at: 2019-07-19T13:07:31.832Z Reads: 80

```
Got a reply back from Seeed.
 
    Dear Simo,

    I am so sorry that there might be further delay on the boards, and we have started the assembling already.

    If everything went smoothly, I expect that we will be able to dispatch them soon.

    **Best Regards,**

    <b>CECI
    Seeed Fusion Support Team

[quote="totalgeek9224, post:211, topic:85493, full:true"]
Darn. How about on the software side of things?
[/quote]
I'm gonna start implementing the USB serial configuration comms today, so it's possible to update the non-volatile parameters through serial terminal. I'm probably gonna implement a simple interface that can then be expanded upon later.
```

---
## \#213 Posted by: totalgeek9224 Posted at: 2019-07-22T21:52:11.517Z Reads: 75

```
In other news, Somone from the other forum posted [this](https://www.aliexpress.com/item/32922633046.html?srcSns=sns_Copy&tid=white_backgroup_101&mb=Me1ZJaxPrpPWbOg&tt=sns_Copy&aff_platform=default&cpt=1563831916008&sk=cl49ywv6&aff_trace_key=e89bf5eb7d8d499c8021ad6907889f50-1563831916008-04910-cl49ywv6&businessType=ProductDetail&platform=AE&terminal_id=17f230c0017541818839afccef0802c8). I wonder what its wave profiles will be like and how something like it would perform with this BMS.
```

---
## \#214 Posted by: SimosMCmuffin Posted at: 2019-07-27T20:18:46.212Z Reads: 84

```
Update.

I've been working on implementing the BMS's configuration through the USB serial connection and I've gotten the basic features implemented. I'm still gonna add some more flesh to it, but here's what's going on right now. I've implemented a GRBL-style (https://github.com/grbl/grbl/wiki/Configuring-Grbl-v0.9) lightweight, but functional configuration interface. I've used the GRBL firmware on one of my custom tabletop CNC routers (running arduino Due with a stepper shield) and then adapted that approach to the BMS.

**(NOTE, forum doesn't allow to place single dollar character in the text, it hides it, but putting 2 of them back-to-back shows both of them $$, check the screenshots for the commands)** 
Sending a "$$?" or just $ through the serial terminal prints out the commands available.
![image|690x362](upload://oS3YkfO5jpORpUPOoqYAaXV2S3.png) 

"$$" will print out the configurable parameters, their values and descriptions. I'm gonna rewrite the description to be clearer, but at least there is something for all currently configurable parameters.
![image|690x363](upload://hV7nsGxAEmlaSJuLOQRguBvxvbU.png) 

Writing new values is done with "$xxx=yyy" where you check the parameter ID through the "$$" menu and then essentially assign a new value to, in the picture below the example write is "$0=10", which writes the packCellCount to be 10 and it then echoes back the new written value.
![image|690x305](upload://a93SGsO0DHtrPVlQVqUgUX2CTSt.png) 

The EEPROM Save and Load functions are working, but I'm gonna add some info text to them for feedback.

The interface is usable through pretty much any serial terminal, with the Arduino IDE terminal shown below.

![image|639x500](upload://98E3K1TOvTrafieuPOFfCvoKl25.png) 

![image|500x500](upload://swyJDzmtdoJIXQGApaaN8mXMOAh.png) 

I'm planning on implementing this simpler interface first and then in the future start looking into integrating the configuration interface into the VESC tool, like DieBieMS does. Feedback and thoughts are welcome based on the info above.

---
PCB assembly status is still unfortunately unknown, I'll email Seeed again on Monday for a status update, but their site still shows the order status as "Processing". Future plan is once I get the order finally to me, I'm gonna quality check the boards and see that they are okay, then send 4 of them to interested testers, once I get green lights at least for the HW then I think I'm gonna go for a bigger batch to get the ball rolling. I'm thinking 15-25 pieces through a bigger PCB assembly provider, I'm currently planning on PCBway.

I think I might be able to start shipping the BMS on the start of next year and I'm planning on taking my trade name out of hibernation and putting up an online store for sales.

This is of course with the assumption that nothing major comes up.

----
Personal note

Man it took couple of days to get the ball rolling on the coding. Have a bad habit of procrastination especially when I should start something new, essentially getting the ball rolling in the beginning. Once I get started then it usually starts to pick up more speed and the last 3 days have been actually been enjoyable 8 hour coding days and I feel like i've gotten a lot accomplished! Gonna try to keep this ball rolling as I'm up to speed now.

----
[quote="totalgeek9224, post:213, topic:85493"]
In other news, Somone from the other forum posted [this ](https://www.aliexpress.com/item/32922633046.html?srcSns=sns_Copy&tid=white_backgroup_101&mb=Me1ZJaxPrpPWbOg&tt=sns_Copy&aff_platform=default&cpt=1563831916008&sk=cl49ywv6&aff_trace_key=e89bf5eb7d8d499c8021ad6907889f50-1563831916008-04910-cl49ywv6&businessType=ProductDetail&platform=AE&terminal_id=17f230c0017541818839afccef0802c8). I wonder what its wave profiles will be like and how something like it would perform with this BMS.
[/quote]
Would be interesting to test. Little bit questioning that 1000W rating tho' when the current is adjustable between 2-12A? it would make sense for the 20S+ Li-ion voltage ones, but how does it function at the lower voltages?...
```

---
## \#215 Posted by: SimosMCmuffin Posted at: 2019-07-30T11:32:00.686Z Reads: 85

```
Got a reply from Seeed:

    I just got the latest news from our engineer, and she told me that the boards are done with assembling, however, they did not pass the final quality inspection, which need to have those boards returned for little bit of tweaking.

    Can you give us more time and we will dispatch them as soon as possible.

    Best Regards,
    Ceci
    Seeed Fusion Support Team

So it would appear that they have run the boards through their assembly line, but have then bounced at the inspection booth. 

This could be anything between tombstoned resistors or capacitors, diodes placed the wrong way around or solder bridges, but unfortunately I didn't get the specific reason for the QC failure, because this is important for me to know, if for example it's something in the component placement, solder mask openings or solder paste sizes. Essentially if it's anything I can affect with the PCB design and component selection. Other possibility is that they didn't have the assembly line machines dialed/fine-tuned in for this specific board and component run.

I recently (couple months ago) visited a local fab house that we were using our customer product. We visited with me and my HW team leader from our design office along with 3 customer reps. I was the one who had designed the PCB, so I was pretty anxious to see the first PCB being populated. Their smaller assembly line that these boards were being run through (200 pieces for this batch) had the following setup:

Input board rack -> Stencil solder paste applicator (auto) -> Solder paste inspection (auto) -> Pick&Place machine (auto) -> Inspection station (manual) -> Re-flow oven (auto) -> Output board rack

So the panel had 3 PCBs on it, but on the very first test, only one of the PCBs were populated and then they did a complete manual inspection on the board at the inspection station. Biggest thing was that all diodes were the correct way around and that none of the components had shifted in position. I immediately got feedback on couple of things that I could fix/change for the volume production design. Other than that, it looked all good, so we then gave the green light for running the rest of the boards. We then hopped onto setting up the production PCB tester that flashed and tested the HW to check that HW worked as was supposed to. I think the boards were all done 2-4 hours later.

This is the biggest hurdle with doing fabrication somewhere where you can't personally go to check on the process and get immediate feedback.

But hopefully they'll be able to ship the boards this or next week, so I can then also check the boards over myself.
```

---
## \#216 Posted by: Komamtb Posted at: 2019-07-30T12:06:21.026Z Reads: 81

```
Good to hear all the updates! Patiently waiting..
```

---
## \#217 Posted by: SimosMCmuffin Posted at: 2019-07-31T17:49:17.730Z Reads: 80

```
Good news, I just got confirmation email and text messages from DHL, informing me of a package from Seeed. Estimated delivery is on Friday the 2nd this week.

---
On the other news, I don't how I did it, but I messed up my sleep schedule something major over the last two days. Been feeling like an absolute daylight zombie today and yesterday. Gonna try to get this sorted, feeling awful :persevere::tired_face:
```

---
## \#218 Posted by: totalgeek9224 Posted at: 2019-08-01T10:09:10.311Z Reads: 81

```
The good news is indeed great! Can't wait to see her w it comes out

On the other hand, I hope you salvage your sleep schedule soon, noone likes feeling like a daylight zombie.
```

---
## \#219 Posted by: banjaxxed Posted at: 2019-08-01T13:52:18.407Z Reads: 81

```
[quote="SimosMCmuffin, post:214, topic:85493"]
forum doesn’t allow to place single dollar character in the text, it hides it
[/quote]

\$

precede the 'special' character with a backslash and it will not be interpreted

Also code blocks are not difficult

https://forum.digikey.com/t/an-unofficial-discourse-user-reference-guide/1125#heading--CodeFormatting

```
function foo(bar){
     return bar+1;
}
```
```

---
## \#220 Posted by: SimosMCmuffin Posted at: 2019-08-02T18:48:58.381Z Reads: 81

```
Boards are here!

![IMAG0464|690x456](upload://vIwdf2wergB4sQc0CKuBXhjatAc.jpeg) 
![IMAG0467|690x445](upload://o0uYIFMy2X2spKdwRVbaNbIS72U.jpeg) 

Quality wise, there is room for improvement, but understanding that it's only 5 boards, I doubt they have a lot of resources to dedicate for a run in case of problems. I have so far looked over them quickly, but I almost immediately found something that I need to do rework to fix.

CAN IC pins in short circuit by solder bridge.
![IMAG0463|690x457](upload://jsfgNhgTwh1nCQBvbQmrBrlZtmQ.jpeg) 
Weird scratches on the board, exposing copper underneath solder mask. Maybe they were trying to remove solder bridges?

![IMAG0466|354x241](upload://2IAFZYzplpZXlMXKba8zufkFN7d.jpeg) 

I'm gonna look the boards over tomorrow and make a list of all the shortcomings. 

Also writing code, got the charging algorithm updated today and got the first tentative charges going, need to keep working at it and clean it up afterwards, looks like absolute code vomit atm. I need to add a live status mode for the Comms, so I can monitor the current runtime state more easily. Also found and fixed a bug/feature in the EEPROM/FLASH library, that should have worked in a way that once the flash pages dedicated for the non-volatile parameters filled up, it should have erased the first page, written the new non-volatiles and then erased the other pages, but instead it didn't write after the page erases causing the non-volatile memory to be just 1s and then the parameters would always revert to their default values, because the load function didn't find anything saved in the memory, which there wasn't. But I got that fixed.
```

---
## \#221 Posted by: totalgeek9224 Posted at: 2019-08-04T16:09:22.322Z Reads: 75

```
What are the dimensions for the board?

Im glad to see that they've arrived, although its a shame about the quality misshaps. But great to see you continuing the development of the code. For sure i cant wait to get my hands on one of these to put in my build! (just got to get the build going :P )
```

---
## \#222 Posted by: SimosMCmuffin Posted at: 2019-08-04T18:02:36.446Z Reads: 77

```
PCB XY-dimensions are 62.5x26.5 mm and mounting hole pattern is 57x21 mm.

[quote="totalgeek9224, post:221, topic:85493"]
But great to see you continuing the development of the code.
[/quote]
Yea, there are still a lot of features I want to add, for example I'm working on a fault flag system, so you can query them through the USB serial connection, in case you get a red error indicating status light.

    typedef enum
    {
    	fault_lowPackVoltage = 0,
    	fault_highPackVoltage,
    	fault_lowCellVoltage0,
    	fault_highCellVoltage0,
    	fault_lowCellVoltage1,
    	fault_highCellVoltage1,
    	fault_lowCellVoltage2,
    	fault_highCellVoltage2,
    	fault_lowCellVoltage3,
    	fault_highCellVoltage3,
    	fault_lowCellVoltage4,
    	fault_highCellVoltage4,
    	fault_lowCellVoltage5,
    	fault_highCellVoltage5,
    	fault_lowCellVoltage6,
    	fault_highCellVoltage6,
    	fault_lowCellVoltage7,
    	fault_highCellVoltage7,
    	fault_lowCellVoltage8,
    	fault_highCellVoltage8,
    	fault_lowCellVoltage9,
    	fault_highCellVoltage9,
    	fault_lowCellVoltage10,
    	fault_highCellVoltage10,
    	fault_lowCellVoltage11,
    	fault_highCellVoltage11,
    	fault_highChargerVoltage,
    	fault_highChargingCurrent,
    	fault_lowBMStemp,
    	fault_highBMStemp,
    	fault_lowNTCtemp,
    	fault_highNTCtemp,
    	fault_numberOfElements
    }_fault_ID;

Then there is a lot of implementation specific coding and testing, so that everything functions in a logical order and fashion.

I did do a mistake though and bought Oxygen Not Included on Steam and I'm completely hooked. Reminds me the time I got hooked on factorio... So many interesting mechanics and challenges...
https://store.steampowered.com/app/457140/Oxygen_Not_Included/
```

---
## \#223 Posted by: janpom Posted at: 2019-08-04T18:37:36.786Z Reads: 75

```
[quote="SimosMCmuffin, post:222, topic:85493"]
PCB XY-dimensions are 62.5x26.5 mm
[/quote]

That's great. So tiny! If it works and it has CAN, this is going to be a killer.
```

---
## \#224 Posted by: totalgeek9224 Posted at: 2019-08-04T18:42:35.524Z Reads: 74

```
[quote="SimosMCmuffin, post:222, topic:85493"]
I did do a mistake though and bought Oxygen Not Included on Steam and I’m completely hooked.
[/quote]
been there, done that, and let me tell you, its a hell of a wormhole, especially with all of the new content they've added. Hope you have a blast playing it!
```

---
## \#225 Posted by: SimosMCmuffin Posted at: 2019-08-05T17:10:20.886Z Reads: 74

```
Summary of things to fix on the 5 boards.

1. 
- Solder bridge between LTC6803's pins
- Very little solder paste on MAX15062 pins

2.
- Solder bridges on the CAN IC

3.
- Clean crusty solder finish on LTC6803's pins

4.
- Reflow MAX15062 for questionable position

5.
- Reflow MAX15062 for mis-alignment

Overall rating 3/5 for low-cost small volume prototype run. Need to fix couple of things, as outlined above. All resistors, capacitors, diodes and lower pitch components visually looking good.

- 1/5 - unusable as is, need to rework whole board
- 2/5 - some components correctly placed, need to do rework, but partially
- 3/5 - overall good, but problems with challenging components, little or no rework needed
- 4/5 - all components correctly on, no need for rework, not the best finish or alignment (crusty)
- 5/5 - all components correctly on, correct paste amounts and excellent component placement and finish

Gonna fix the boards tomorrow.
```

---
## \#226 Posted by: SimosMCmuffin Posted at: 2019-08-19T14:22:29.142Z Reads: 68

```
Got the charging algorithm adapted, so it's working again, mostly. Need to fine-tune things alongside testing. Found for example weird stability issue with the LTC6803 that manifests as incorrect cell voltage measurements when an USB-cable wasn't connected, but was fixed by connecting an USB-cable. Not yet sure if it's grounding or power supply issue, but I have ideas where to start testing for a fix.

I have also fixed the 5 boards, but have not yet power-tested them. Need to get the firmware sorted into a basic stable functioning state first.

I have also opened communications with an US based start-up company for designing a high voltage, cascadable car/energy storage scale BMS. We're still in the process of doing the HW block diagram for the Proof-of-Concept prototype.
```

---
## \#227 Posted by: Wisp Posted at: 2019-08-19T22:05:02.865Z Reads: 66

```
When the time is right it communication with Davega could be implemented (like the smart BMS), no? :star_struck:
```

---
## \#228 Posted by: janpom Posted at: 2019-08-20T08:50:05.466Z Reads: 64

```
I think so, provided there's CAN and communication can be relayed by VESC the same way as with DieBieMS.
```

---
## \#229 Posted by: SimosMCmuffin Posted at: 2019-08-21T16:32:41.806Z Reads: 64

```
Did a hotfix for the LTC6803 measurement error. Looks like it's 5V VREG output really doesn't tolerate any extra load on it (and I'm powering the MCU currently from it...), so I'm gonna have to do another HW iteration for the board. I have shown below the current power supply scheme and then what I propose for the 0.3 HW revision. I found a nice linear regulator for the MCU.
![image|690x467](upload://e69lKCCt0eLqrDVBDLMzLuzilyq.png)
```

---
## \#230 Posted by: SimosMCmuffin Posted at: 2019-08-27T09:38:43.609Z Reads: 72

```
I ordered 0.3 HW boards today.

Changelog 0.2 -> 0.3:
- Added a small pull-down resistor to INA180 shunt op-amp output to pull it to ground, if IC un-powered
- Added a protection/fuse resistor to CAN ground, in case battery negative lead gets cut, then all current would try to return through CAN ground, but will blow resistor now, instead of burning CAN GND wire
- Moved traces from between LTC6803 pins
- Switched MCU supply to dedicated 3V3 linear regulator (RT9068), removing it from loading LTC6803's 5V VREG output, which caused measurement inaccuracies
- Improved LTC6803 power decoupling
- Changed couple diodes related to MCU power supply to work with new regulator
```

---
## \#231 Posted by: SimosMCmuffin Posted at: 2019-09-15T12:52:36.212Z Reads: 68

```
**Update**

Got the 0.3 HW boards (last week) and components (this week) and assembled one this weekend. Did some analysis on the quiescent current consumption and after couple of code tweaks, got it to **~80 µA** in the low-power run state (not stopped state). There is the possibility of optimizing into a Stop 2 mode for the power-saving, which could (according to datasheet) lower the quiescent current another ~30-50 µA, but this is a sleep state, so can't run any code during this.

I still need to test that the power supply scheme change fixed the cell voltage measurement error, but this setup should actually improve the measurement accuracy performance in all states compared to before, but need to verify this.

![IMAG0499|624x500](upload://pR2JqN3uflSqoNrcgoFIpNLI7dA.jpeg) 

![IMAG0500|563x500](upload://vhHhNxAuB7rMIQ0uf70fTHQJ1ZA.jpeg)
```

---
## \#232 Posted by: SimosMCmuffin Posted at: 2019-09-18T08:47:52.226Z Reads: 63

```
**Update**

Have been using the 0.3 board to charge my pack on the start of the week and I've been testing it's performance. 

I started with just comparing the cell measurement results between the 0.2 and 0.3 boards. Both showed steady numbers for all the cell measurements, but the 0.2 board showed slightly lower voltages for all cells, namely about 2-3 mV lower compared to the 0.3 board. So I used my multimeter to manually check the cell voltages to compare against the boards measurements. The DMM showed identical numbers to the 0.3 board, but a doubt started to rise within in about one thing. How accurate are my DMM's voltage measurements? I need to calibrate/verify it's readings before I can say whether the results are good or not.

Brought the DMM to office to compare against better and more expensive equipment. So I hooked up my chinese Aneng AN8008, a Fluke 179 and a Keysight 34461A benchtop DMM to a low noise voltage source and tested couple different voltage measurements on different ranges to see how accurate the indicated measurements were. The Keysight is probably the most accurate DMM, so it's an accurate enough reference to compare the AN8008 results against.

![IMAG0502|282x500](upload://qTsm3Ma30TGpDfVQbv14A5ywRmm.jpeg) 

![IMAG0503|282x500](upload://hybUPrNyWQEYW2s2tm0rN7nsqVY.jpeg) 

![IMAG0504|282x500](upload://iitRiZkDx0ouvUsutzawhnt1wXo.jpeg) 

The measurements seemed to be within 1 least significant indicated number. All the DMMs had some noise on their indicated least significant numbers, but that's normal as the voltage source was not a voltage *reference*, but just quite clean DC output. So with that test I could trust the steady DC voltage measurement were pretty spot on in the 3.000 - 4.200 V range, which was the range I was interested in due to wanting to verify the Li-Ion cell voltages.

*So what is the result?*

Well my DMM is showing **identical** numbers to one measured by the LTC6803 on the 0.3 board and I have verified that the DMM is accurate withing +-1 mV in the used voltage range, so all I can say is that I'm pretty darn happy about it's performance! Also not bad for a 22€ DMM.

I suspect on the 0.2 board that the MCU is loading down the LTC6803's VREG enough that it disturbs the measurement results, even though they are steady, they show consistently 2-3 mV less then the 0.3 board results. But that is really what I wanted to fix for the 0.3 iteration, by completely supplying the MCU through a separate regulation, removing it's influence on the LTC6803's VREG output.

-----

**Future moves and HW RC (Release Candidate)**

**I'm moving to a ramp-up stage on the development**. I did very slight changes to the HW and with that I'm moving onto 0.4/RC1 HW (Release Candidate). I feel like the HW is now mature enough and the SW is usable enough (still under development) to start considering doing a development batch of 10 boards meant for distributing to HW testers and SW developers. ***I will be opening a sign-up form for testers and developers in the coming days. Link to it will be posted on this thread along with more info.***

I have ordered components for a couple hundred euros for the upcoming developer build, which I I'm going to hand assemble, so I have the best/personal control over quality. I can also test the hand assembly time for larger batches, so I can compare the time/cost ratio for future production batches. The 0.4/RC1 gerbers are ready and I'm planning on ordering the boards next week. I want to test couple extra connector options for the XH and PH connectors on the board before ordering the 0.4 boards.

-----

**Other BMS news, FlexiBMS HV**

I've been doing HW design with an American start-up company for a *high voltage* variant of the FlexiBMS for a bit over a month now. They contacted me through PMs on this forum, commenting about this Lite thread and expressing interested for the Lite and a HV version. I'm not on a payroll, I'm working rather for the possible future sales, we have been discussing and planning for me to give them a license allowing them to use the HW design (single-time payment) and then a small commission fee for every unit sold.

So what's this HV version about then?

* LTC680**4** battery stack monitor (newer gen. to the LTC6803)
* Master/Slave topology
* Cascadable design for chaining multiple packs together in series (they are going for 8 units -> 96S)
* True isolated connections between LTC6804's
* Isolated external charging contactor control on Master module
* CAN-bus on Master module

What application is the HV meant for?

Higher voltage use, EVs, power storage. The real point is that you can connect multiple packs together in series for larger S-configurations and be able to measure all series cell voltages and balance them if necessary. They for now have been talking about using them in recycled Tesla model S packs for re-use and want a BMS for that.

It's not meant for the small scale as the Lite is (3S-12S) and is not an All-In-One, but for bigger pack configurations (12S+) where you need to start designing your system as a distributed one.
```

---
## \#233 Posted by: janpom Posted at: 2019-09-18T08:56:03.376Z Reads: 60

```
Great progress! I'd be happy to do some testing. I can also do a code review for you and/or help build the integration with VESC and other devices like Metr or my DAVEGA. This would be best done by implementing the same communication protocol as DieBieMS uses since that one is already supported by Metr and is going to be supported by DAVEGA soon as well.
```

---
## \#234 Posted by: Friskies Posted at: 2019-09-18T10:18:12.948Z Reads: 61

```
It's awesome watching the progress of this BMS. I'll be sending money your way when they are available. Awesome work!!!
```

---
## \#235 Posted by: Pedrodemio Posted at: 2019-09-18T16:56:51.268Z Reads: 61

```
Nice to hear that, so in the future we will be able to read all BMS data on DAVEGA? And maybe the other way around? configure DAVEGA through Metr
```

---
## \#236 Posted by: ducktaperules Posted at: 2019-09-18T22:17:12.014Z Reads: 62

```
This is looking awesome. This is mostly the only thread i come back here for these days. cant wait till you have RC1 builds to send out. Id be happy to help do some testing when the time comes.
```

---
## \#237 Posted by: janpom Posted at: 2019-09-19T07:20:41.480Z Reads: 61

```
[quote="Pedrodemio, post:235, topic:85493"]
so in the future we will be able to read all BMS data on DAVEGA
[/quote]

Not sure about the "all" part but you'll definitely be able to read the most important DieBieMS data (e.g. individual cell voltages) on DAVEGA X pretty soon. It's high on the TODO list now.

[quote="Pedrodemio, post:235, topic:85493"]
configure DAVEGA through Metr
[/quote]

This is less likely though not completely out of question. It would definitely be possible technically once DAVEGA X has CANBUS. We would need to coordinate with @rpasichnyk. We have already been working together a little bit -- me testing his Metr Unity module and him and @hexakopter testing the DAVEGA X -- so we'll see what happens. 

If you have any more questions please ask in https://forum./t/davega-x-gauging-interest/5203 so that we don't hijack this thread.
```

---
## \#238 Posted by: SimosMCmuffin Posted at: 2019-09-19T18:40:36.048Z Reads: 59

```
Did a final check on the CAN bus functionality today. Implemented an echo function that waits for the CAN to receive any message on the bus and then sends it back to the bus with the same info. Worked without problem.

![IMAG0506|690x335](upload://5eqhHQMMaf0xMbVXzSxis5CLWD6.jpeg) 

The upper received messages were test messages for testing RX at first and checking that the filtering settings were working. Then I changed to actually using the echo function and sent the message shown on the bottom half and it was then received back to the CAN analyzer.

![IMAG0507|690x389](upload://4caNnv2VdikDk8hbXYl0h66fS02.jpeg) 

-----
I also updated the programming jig a little bit. Testers will be sent one, so if we have SW updates, we can flash them before the bootloader and "live flashing" are implemented. *You are gonna have to supply your own programmer though.*

![IMAG0508|689x390](upload://nmWxbYPogvpiaDldL7iXL8XQXZ9.jpeg) 

![IMAG0509|689x390](upload://5FruzqK6ggteAUvBEn3RN2OqF3k.jpeg) 

![IMAG0510|689x390](upload://2nGmamuzjbbzGwZZUB04gW53Xdd.jpeg) 

![IMAG0511|689x390](upload://vLZl5TWZfzMWvybeBnmv5pM6QCn.jpeg) 

-----
I also tested how JST's XA and PA series fit onto the board. They are essentially *almost* identical to the XH and PH series, but instead of the detent lock they actually have a locking ramp, so they can't be disconnected unless you press on the tab and pull, or the wires break.

![IMAG0513|690x379](upload://hMXnIsYuaLSPUrZ2pslyaDcyAJZ.jpeg)
```

---
## \#239 Posted by: nickw1881 Posted at: 2019-09-20T06:05:56.952Z Reads: 55

```
Is the software foss? Or is it secret?
```

---
## \#240 Posted by: Darkie02 Posted at: 2019-09-20T07:25:19.204Z Reads: 54

```
[quote="janpom, post:233, topic:85493"]
same communication protocol as DieBieMS uses since that one is already supported by Metr and is going to be supported by DAVEGA soon
[/quote]


Hoping so to this will then start to be a standard for eSk8 in my eyes.
```

---
## \#241 Posted by: SimosMCmuffin Posted at: 2019-09-20T07:41:30.461Z Reads: 52

```
I'll throw it up on github at some point soonish. Need to clean up the commented code lines and comments.
```

---
## \#242 Posted by: Pimousse Posted at: 2019-09-20T08:44:54.052Z Reads: 54

```
All these improvements are awesome ! Congrats @SimosMCmuffin !

We should definitely work on a PR for integrating a standard BMS communication into VESC FW for a better interaction between both. :slight_smile:
```

---
## \#243 Posted by: SimosMCmuffin Posted at: 2019-09-20T08:50:21.067Z Reads: 54

```
Has there been development for a generic/standard BMS CAN communication for VESC with DieBieMS's or has it just been DieBie's side implementation?
```

---
## \#244 Posted by: Pimousse Posted at: 2019-09-20T08:55:36.826Z Reads: 56

```
No, at least I'm not aware of this.
That was my top priority when I jumped into the DieBieMS adventure but I couldn't find details to successfully compile the code (I tried tho but I bricked my DBMS, rescued by a ST-Link :neutral_face: ).

If you're interested, I can work on a draft of features that may be interesting to develop for such VESC-BMS wedding. :slight_smile:
```

---
## \#245 Posted by: SimosMCmuffin Posted at: 2019-09-20T09:14:00.837Z Reads: 56

```
Maybe just a more general look at what possible messages could be used in a generalized BMS CAN communication. Then maybe add to that more VESC specific messages.

Here's little sneak-peek picture of the FlexiBMS HV:

![image|690x339](upload://7hqJnFxIRVnbP89BYfWHKOWsIHo.jpeg)
```

---
## \#246 Posted by: Pimousse Posted at: 2019-09-20T09:15:56.513Z Reads: 56

```
[quote="SimosMCmuffin, post:245, topic:85493"]
Maybe just a more general look at what possible messages could be used in a generalized BMS CAN communication. Then maybe add to that more VESC specific messages.
[/quote]

 Yes, this is exactly what I meant. :+1:
```

---
## \#247 Posted by: SimosMCmuffin Posted at: 2019-09-20T09:20:58.839Z Reads: 53

```
That would actually be pretty ace thing to do. What are you planning on using to draft the standard?
```

---
## \#248 Posted by: SimosMCmuffin Posted at: 2019-09-20T09:28:36.757Z Reads: 58

```
I'm looking into an idea I had about it being possible to turn the opto-isolated **INPUT** into an opto-isolated **OUTPUT**. Will need to flip the opto-IC around and changing some resistors, but would be doable and don't need to do anything if you don't want to change it, so it's just a configuration possibility.

Below is the change from the current implementation to the one I'm proposing that would allow you to turn from an INPUT to an OUTPUT. I'll see how tight the board space will be for the additional resistors.

![image|541x500](upload://k4DlAx3WxPIYejuGC2khSiRP602.png)

EDIT: Donzo

![image|690x339](upload://tO6oHrubEgkJnqK8ULNu3jfnOTi.png)
```

---
## \#249 Posted by: totalgeek9224 Posted at: 2019-09-20T10:50:06.641Z Reads: 55

```
as always, this is looking really good. i like the idea of using JST XA's and PA's instead of XH and PH
```

---
## \#250 Posted by: SimosMCmuffin Posted at: 2019-09-20T11:07:15.788Z Reads: 58

```
I have been thinking about different variations of the FlexiBMS that I'm wanting to make. Currently the closest thing to getting ready-to-ship is the **Lite**-version and I suppose **HV** is currently following somewhere behind (no boards made or tested yet). 

Along those two I've been tossing  around the idea of FlexiBMS **Pro** in my head, which would be based on the Lite, but offer discharge path control alongside better specs in comparison to the Lite, more beefy capability. **Maybe up-to 15S or even 18S support...** Nothing concrete done yet, but rather been just looking around at ICs and possible implementations.

I've also been thinking of a more cost-effective simpler design, which should price wise sit somewhere below half the price (component wise) compared to the FlexiBMS Lite. Essentially a more cost-effective option for just charging and not needing CAN for example or other "flairs". Stripping out anything else in relation to just pure charge control. The problem naming wise is that the battery stack IC that I'm planning to use doesn't support such a large range of S-configurations for the pack, so in that regard I don't think the name FlexiBMS would suit it... **There would be 2 or 3 versions of this BMS for different S-configurations and I'm open to hearing any name ideas for a more economic line of BMS'.**
```

---
## \#251 Posted by: Pimousse Posted at: 2019-09-20T11:41:37.588Z Reads: 57

```
Well. I'm not a HW or SW engineer so if there is a regular way to do it, please tell me.
I was planning a basic Word spec document that would be a good base (which is more what I do daily as now as process control engineer).

What are your thoughts about this ?
```

---
## \#252 Posted by: janpom Posted at: 2019-09-20T11:44:24.872Z Reads: 57

```
Sounds good to me. It doesn't need to be formal as long as it makes sense. I guess this could be as simple as describing the essential parts of the DieBieMS communication protocol.
```

---
## \#253 Posted by: Pimousse Posted at: 2019-09-20T11:53:08.978Z Reads: 58

```
DieBieMS doesn't really interact with the VESC. It shares the same protocol as VESC but that's all AFAIK.

Alright, let me a week to write something up.
```

---
## \#254 Posted by: Surfer Posted at: 2019-09-20T14:04:07.272Z Reads: 58

```
**Maybe up-to 15S or even 18S support…**
This will open to used it also in a Onewheel and euc's wich is awesome, and there are a lot in the wild
```

---
## \#255 Posted by: SimosMCmuffin Posted at: 2019-09-21T18:12:18.061Z Reads: 57

```
**Here's a link to the FlexiBMS Lite 0.4/RC1 Tester Application:**

https://forms.gle/TpVjBbVNobmsMhqp7

Submitted forms can be edited later. Although not sure how it functions, if you're not logged into a google account.
```

---
## \#256 Posted by: totalgeek9224 Posted at: 2019-09-21T18:25:22.440Z Reads: 57

```
god, i was filling in the form when i realised, as much as i want one of these, i probably wouldnt be able to give you the feedback that would be needed. :( Cant wait to see how this goes though
```

---
## \#257 Posted by: SimosMCmuffin Posted at: 2019-09-21T19:04:26.271Z Reads: 58

```
You can fill the application without expertises marked or say so in the extra info section, so you're just an interested person.
```

---
## \#258 Posted by: sayekim Posted at: 2019-09-23T14:15:11.591Z Reads: 50

```
Will there also be a roll to start version of this bms with auto off?

This next to cell monitoring is what I’d like to have.
```

---
## \#259 Posted by: SimosMCmuffin Posted at: 2019-09-23T16:08:58.292Z Reads: 53

```
The Lite-version will not have push-to-start, as it doesn't have discharge path control, but the Pro-version will have it. Once we get some tester feedback, experience and development done on the Lite, AKA get ready to sell, then the development on the Pro version will start.

[quote="SimosMCmuffin, post:250, topic:85493"]
Along those two I’ve been tossing around the idea of FlexiBMS **Pro** in my head, which would be based on the Lite, but offer discharge path control alongside better specs in comparison to the Lite, more beefy capability. **Maybe up-to 15S or even 18S support…** Nothing concrete done yet, but rather been just looking around at ICs and possible implementations.
[/quote]
```

---
## \#260 Posted by: SimosMCmuffin Posted at: 2019-09-23T17:13:42.011Z Reads: 53

```
Finished the first manual version of the multi S-configurable pack tester board. 4 cells in series in one board, can chain them together, sense wires coming from all cells, can select what cell is the positive terminal cell and can disconnect sense wires per cell basis.

This is gonna make testing different cell configurations so much easier.

![image|648x500](upload://7UOfTzDi9Y33md4JSv9Xo6PK5zS.jpeg) 

Gonna use these spring steel battery clips that I've been using for my portable devices. Below is a 1S4P pack.

![IMAG0516|651x500](upload://aVQrKqPK7CNHKo5prTgEU4PPeJ4.jpeg) 

![IMAG0517|690x383](upload://4wU5x8hZzyQHGna4eHCUQmRPRGu.jpeg) 

I'm planning on ordering the 0.4/RC1 boards on this wednesday, think I'm gonna go for 20 pieces.
```

---
## \#261 Posted by: janpom Posted at: 2019-09-26T10:56:29.813Z Reads: 49

```
I just want to say it's very hard for me to resist the temptation to sign up as a tester. This is a very exciting project. I was already half way filling up the form but then I stopped for a while to think about when exactly will I do the testing and I remembered how I hardly had time to sleep in the last couple of week. So I closed the form again. I may still be available in a couple of months things once I'm less busy with the DAVEGAs and maybe reduce the hours in my job.
```

---
## \#262 Posted by: Pimousse Posted at: 2019-09-26T11:49:00.743Z Reads: 50

```
Same for me. I already have your last prototype for an PV project but no time for it.
That would be unfair to take a slot.
```

---
## \#263 Posted by: glyphiks Posted at: 2019-09-26T14:34:08.556Z Reads: 52

```
Signed up. Pretty keen to help get this going 👍
```

---
## \#264 Posted by: walleywalker Posted at: 2019-09-26T15:07:39.624Z Reads: 56

```
Could the boards be used to test a 3P configuration? If so sign me up for some!
```

---
## \#265 Posted by: SimosMCmuffin Posted at: 2019-09-26T17:23:56.941Z Reads: 50

```
Can you be a bit more specific in the 3P specification? Are you planning on running 3 Li-Pos in parallel or building a xS3P pack with 18650s?
```

---
## \#266 Posted by: walleywalker Posted at: 2019-09-26T17:39:26.588Z Reads: 55

```
Assuming these can daisy chain, I'd be interested in using them to test a 12S3P setup with 18650 cells before spot welding them in their final layout.
```

---
## \#267 Posted by: SimosMCmuffin Posted at: 2019-09-26T18:34:46.021Z Reads: 57

```
Unfortunately this variant of the BMS can't be daisy-chained, but out of curiosity how were you exactly planning on connecting them with your packs to test them, because I still can't quite figure out the any way that makes sense to me. How are you're planning on connecting them?
```

---
## \#268 Posted by: SimosMCmuffin Posted at: 2019-09-26T18:50:30.309Z Reads: 56

```
# !NOTICE!

**This project thread is moving over to  forum. Please continue the conversation over there, thank you.**

**New project thread can be found @ https://forum./t/flexibms-lite-flexible-configuration-bms-w-can-bus-tester-application-open/8801**

**Major updates on the project will still be posted on this thread too, but all the smaller updates and discussions will be continued at the  forum's project thread at the link above**

**Link to the new project thread will be posted on every major update messages**


___--MCmuffin___
```

---
## \#269 Posted by: walleywalker Posted at: 2019-09-26T19:00:55.522Z Reads: 55

```
I guess I just realized that the board is only setup for a series connection, so you're right this wouldn't work for me
```

---
