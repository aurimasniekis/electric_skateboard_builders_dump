# Raphael Chang BMS and ESC

### Replies: 452 Views: 32973

## \#1 Posted by: boards Posted at: 2016-09-05T06:34:21.861Z Reads: 1041

```
This guy made his own ESC and BMS. (Probably helped getting an internship at BB lol)

The BMS actually looks pretty nice http://raphaelchang.com/projects/bms/ https://github.com/raphaelchang/battman-hardware and seems close to functional. It has push button for power. Another thing to look out for I guess.

The ESC still seems reliant on a magnetic encoder, but might become interesting.
```

---
## \#2 Posted by: lox897 Posted at: 2016-09-05T07:03:15.158Z Reads: 919

```
Looks really nice. His ESC looks really good as well. I wonder if it performs as well, if not better than the VESC. Do you think he is on the forum?

EDIT: I have sent an email to him inviting him to the forum
```

---
## \#3 Posted by: boards Posted at: 2016-09-05T07:12:47.921Z Reads: 890

```
I doubt he's on the forum. He's moved away from the DRV8302 in his designs, so it can't be that bad. (Crossing fingers for eventual reliable FOC).

Looking at his stuff makes me realize I need to be more ambitious with being a robotics student LOL.
```

---
## \#4 Posted by: Ulfberht Posted at: 2016-09-05T21:48:32.797Z Reads: 808

```
Very interesting. You know he used to work for Boosted Boards. :wink:
```

---
## \#5 Posted by: michaeld33 Posted at: 2016-09-05T21:56:28.759Z Reads: 790

```
Damn this is sweet. The ESC is nice too!
```

---
## \#6 Posted by: JLabs Posted at: 2016-09-05T22:03:38.414Z Reads: 764

```
Way cool, he defiantly needs to join the forum!
```

---
## \#7 Posted by: treenutter Posted at: 2016-09-06T03:27:19.780Z Reads: 736

```
This is exciting. Looks like another viable ESC option for us.
```

---
## \#8 Posted by: akira Posted at: 2016-09-06T11:59:01.716Z Reads: 717

```
Great !
The BMS is last bit of element that was not DIY on my project !!
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-09-06T13:55:26.702Z Reads: 700

```
I will be following this. Good stuff!
```

---
## \#10 Posted by: HTownBomber Posted at: 2016-09-06T14:21:07.039Z Reads: 697

```
Looks kinda like he's trying to build a better, faster Boosted. BMS looks interesting as it's tailor-made for 12s LiFePO4.   

I'd be very interested in an ESC designed specifically for FOC, especially if it can handle high amps better than the VESC. Amazing to see guys do this kinda work in their free time and share their design open-source.
```

---
## \#11 Posted by: sl33py Posted at: 2016-09-06T18:50:52.377Z Reads: 703

```
Guy has some amazing skill obviously.  Definitely check out his other projects.  Cool Cap spot welder too!

Be great to have him join and contribute here.
```

---
## \#12 Posted by: DougM Posted at: 2016-09-06T19:05:11.388Z Reads: 751

```
This is very intriguing - I'm going to take a look at it since I've given up on the chinese BMS vendors.
```

---
## \#13 Posted by: raphaelchang Posted at: 2016-10-11T05:24:51.139Z Reads: 722

```
Thank you everyone for inviting me to this forum, and thanks for all the positive comments! Sorry for taking so long to reply to this thread, school has been very busy for the last month.

First, a bit about me: I’m a student at MIT and I enjoy designing and building electromechanical systems. I was originally developing an ESC and BMS just for my own skateboard, to build a skateboard with fully custom parts. Over the last year, however, they became more independent projects. Since there seems to be quite a bit of interest in them in the DIY community, I am interested in developing and releasing them to the DIY community for others to use. This will take some more development to make them work with different system requirements; I have a rough timeline below.

Here's a small preview of the two boards, the ESC ("Infinity") and the BMS ("Battman"). They're still under development, so some of these specifications may change as I do more testing and iterating.

**Infinity ESC**
Development progress: [http://raphaelchang.com/projects/brushless-esc/](http://raphaelchang.com/projects/brushless-esc/)
GitHub: https://github.com/raphaelchang/infinity-hardware (PCB), https://github.com/raphaelchang/infinity-firmware (Firmware)
<img src="/uploads/db1493/original/3X/4/3/43d02ec9a73c97307e2d23b496dfb853aa9967ba.PNG" width="350"><img src="/uploads/db1493/original/3X/b/6/b6249928dd027236ad5d93d16112a8936fa07a2f.jpg" width="350">

Features:

* 8V-50V operating voltage (3S-12S LiPo)
* 80A continuous, 100A peak (may change with more testing)
* Sensored and sensorless (in development) field-oriented control
* DirectFET MOSFETs for better heat dissipation
* Discrete 3A MOSFET drivers with 100V tolerance (no DRV)
* 3 discrete current amplifiers for improved current measurement
* Separate gate drive and logic level buck converters for reliability
* CAN, UART, I2C, SPI, PPM, USB for communication (Nunchuk, NRF, etc.)
* STM32F4 with bootloader buttons for programming without ST-Link
* Node.js web application for cross platform GUI configuration
* Bulk capacitor mounted to PCB
* 2"x1.5" PCB size

**Battman BMS**
Development progress: [http://raphaelchang.com/projects/bms/](http://raphaelchang.com/projects/bms/)
GitHub: https://github.com/raphaelchang/battman-hardware (PCB), https://github.com/raphaelchang/battman-firmware (Firmware)
<img src="/uploads/db1493/original/3X/a/f/afbe98d1019d2f924338baace0ebdfcf24a49e4f.PNG" width="550">

Features:

* Supports 4 to 12 cell LiPo and LiFePo4 battery packs
* 100A continuous, 150A peak discharge current (may change)
* Cell voltage monitoring and ~100mA balancing with LTC6803 IC
* Bidirectional current monitoring with overcurrent protection and SOC tracking (planned)
* Boost converter circuit with adjustable voltage for CC/CV charging at ~3A
* Pre-discharge circuit to limit inrush current
* External push button (momentary) switch to turn on BMS and rest of system
* Complete shutdown to preserve battery when not in use
* STM32F3 with UART, I2C, CAN communication and WS2812 LED support
* GUI for configuration
* Flash memory to log battery usage data during rides
* Optional CAN communication with Infinity ESC for smarter protection (planned)
* 3.5"x1" PCB size

As these are personal projects, I have to balance the time I spend on them with schoolwork and other things, so it will take a while before they're ready for use. Still, I'm spending quite a bit of time on them, as well as working with a few friends to develop various aspects in parallel. I'm estimating a few more months of development, so early 2017 is what I am aiming for right now. Infinity is a little further along than Battman, so it might be ready first.

Any questions and comments are appreciated, and I'll definitely post more details and any important updates here. Stay tuned!
```

---
## \#14 Posted by: Jinra Posted at: 2016-10-11T06:01:24.320Z Reads: 627

```
Sounds like this will give the VESC a run for it's money, can't wait to see this in action!
```

---
## \#15 Posted by: Eboostin Posted at: 2016-10-11T06:09:25.605Z Reads: 622

```
Thank you for joining and sharing your work. Both the esc and bms are very interesting, especially the BMS as I have not personally seen one as powerful that is that small. That PCB size seems to apply to 10A discharge BMS.
```

---
## \#16 Posted by: Pantologist Posted at: 2016-10-11T12:43:39.892Z Reads: 624

```
Would you consider integrating a receiver or Bluetooth module in either the BMS or ESC? I forgot what built in radio the Vesc 6.0 will have but doing something similar would be great.

For the BMS could you add a little fuse standoffs so we don't have to have a separate fuse unit. 

Check out JTAG's BMS project. http://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/67?u=pantologist
```

---
## \#17 Posted by: caustin Posted at: 2016-10-11T12:49:04.255Z Reads: 596

```
Welcome, awesome stuff!!
```

---
## \#18 Posted by: raphaelchang Posted at: 2016-10-11T21:40:52.547Z Reads: 608

```
I have considered integrating a Bluetooth module into the BMS and ESC, but I decided that it would be better to design an external module that would be plug and play into one of the JST connectors. This way, I can keep the boards compact (wireless modules tend to require many parts + antenna space) and people who don't care about having Bluetooth don't have to pay for the extra components.

I do have surface mount fuses on the BMS right now (a few in parallel). If they turn out to be problematic at high currents I will consider switching to standard fuses, but it could be difficult with size constraints.

I have actually seen the DieBieMS before, but I did not know it originated here. We seem to have a lot of features in common, it would be awesome for both projects to co-exist in the community.
```

---
## \#19 Posted by: DougM Posted at: 2016-10-11T23:18:55.771Z Reads: 586

```
I think this is a good decision - I personally use XBee and am looking forward to giving your designs a try and would much rather have a serial connection than to have to hack in a nonstandard radio.

Thank you very much for open sourcing the project!
```

---
## \#20 Posted by: Glenn Posted at: 2016-10-12T03:51:35.280Z Reads: 575

```
I want this for my next build
```

---
## \#21 Posted by: smurf Posted at: 2016-10-12T04:48:19.535Z Reads: 547

```
I would like to know what's going on inside the BMS if it's working or not. What I would love to see is the BMS & 2 ESCs on one PCB in a box.
```

---
## \#22 Posted by: Pantologist Posted at: 2016-10-12T05:04:48.587Z Reads: 532

```
I'd rather have the BMS housed with the battery like in most builds and prebuilt boards. 

A Dual ESC PCB can easily be done. All you need is to attach the two PCBs to one piece of acrylic or something either next to each other or on top of each other.
```

---
## \#23 Posted by: sl33py Posted at: 2016-10-12T07:27:53.756Z Reads: 529

```
Welcome to the forum @raphaelchang!  Great to see these projects take shape.  Looking forward to trying them both out when they are ready!

Good luck at MIT and hope to see you on here when time permits!
```

---
## \#24 Posted by: rpn314 Posted at: 2016-10-12T07:34:07.419Z Reads: 531

```
AHHHHH!! On my toes already! Must have BMS.

/Outburst

Glad to have you @raphaelchang
```

---
## \#25 Posted by: TarzanHBK Posted at: 2016-10-12T08:53:45.690Z Reads: 530

```
would be good to have liion support on that bms - that´s what most people use here :slight_smile:
```

---
## \#26 Posted by: thisrealhuman Posted at: 2016-10-12T10:20:14.770Z Reads: 541

```
Nice looking bms you got there.

<img src="/uploads/db1493/original/3X/8/5/8575393cb8fbbd9e5778a1a9d5eec615fc375fca.jpg" width="430" height="253">

Welcome to the community!
```

---
## \#28 Posted by: rpn314 Posted at: 2016-10-12T12:36:25.426Z Reads: 522

```
From a BMS perspective I think li-ion and li-po should be pretty much the same, so I think this would already work just fine with li-ion packs as well. Can anyone confirm that or am I just spouting lies in my excitement? :smiley:
```

---
## \#29 Posted by: 2-alex-2 Posted at: 2016-10-12T13:29:02.413Z Reads: 509

```
Lipo have a higher low cutoff than lion so would require some adjustments if possible maybe with small surface mounted push button.
```

---
## \#30 Posted by: Maxid Posted at: 2016-10-12T14:57:30.710Z Reads: 495

```
they are both rated at 4.2V per cell - not sure what the higher cut-off is you are talking about.
```

---
## \#31 Posted by: DougM Posted at: 2016-10-12T15:32:51.509Z Reads: 493

```
Also, it would be great to bring out a couple of GPIO's so we can add native deadman and headlight functionality.
```

---
## \#32 Posted by: 2-alex-2 Posted at: 2016-10-12T15:38:24.120Z Reads: 489

```
Lol edited it mean a higher low voltage cutoff.
```

---
## \#33 Posted by: Toleg Posted at: 2016-10-12T15:43:59.648Z Reads: 477

```
Yeah, INSTANT NEEEEEEEEEEEEEEEEEDDDDDDDDDDDDDDDDD :)
```

---
## \#34 Posted by: raphaelchang Posted at: 2016-10-13T00:18:46.394Z Reads: 482

```
Thanks everyone for the welcomes! The BMS will support lithium ion (LiPo in particular) batteries. It does have a higher low voltage cutoff (and higher voltage in general) compared to LiFePo4 so it will be a configuration option in the GUI. I'm thinking of doing something like "auto-detect" where you can just plug in the balance connector and the BMS will be able to determine the battery type and number of cells by looking at the voltages at the balance connector.

There are two GPIOs brought out right now, in addition to 3.3V and 5V power for lights, LEDs, buzzers, etc. The GPIOs also support I2C and UART as well as WS2812 driving.
```

---
## \#35 Posted by: Hummie Posted at: 2016-10-13T02:51:28.250Z Reads: 473

```
Can u make a program to send voltages to ur phone?  There's so many complications with an automated bms, if u can just send all the voltages to ur phone u can simply become the bms.  That's what I'd rather do.  As long as there's a low voltage cut-off for the pack.
```

---
## \#36 Posted by: raphaelchang Posted at: 2016-10-13T03:12:27.511Z Reads: 467

```
With a Bluetooth add-on that could be possible. The BMS also balances and protects against over-current and over-charging though, which you can't really do from a phone. I agree that having an app to monitor the state of charge and other battery stats would be nice though.
```

---
## \#37 Posted by: TarzanHBK Posted at: 2016-10-13T06:46:53.791Z Reads: 463

```
thats awesome! Also really cool if people like to use some uncommon packs like 7s or 9s, if the bms is auto detecting :slight_smile:
```

---
## \#38 Posted by: oneafrikan Posted at: 2016-10-13T13:10:20.812Z Reads: 485

```
My 2p - create a tip jar for folks to send you cash. I know quite a few here would. Then it becomes easier to spend time on something you clearly enjoy doing. Could end up a product / license for you in the end. 

Awesome work man!
```

---
## \#39 Posted by: raphaelchang Posted at: 2016-10-15T06:04:36.726Z Reads: 519

```
All this excitement made me realize I should post updates on here more often :) so here goes.

Just finished routing some changes for the next iteration of the BMS, which has slightly higher balance current and an added buzzer. I've sent out the first version to OSHPark, so they should be here in a week (can't wait!). I'm liking the compact size of this board, 3.25 inches wide without the mounting hole tabs which add ~0.2 inches to each side, and 1 inch tall. I think it'll fit nicely with most battery pack layouts. The short height might even allow it to be mounted sideways on the side of a battery.

Here's the current layout of the board (with pretty CAD models):
<img src="/uploads/db1493/original/3X/c/d/cd4c52e7190f9b9a44d18780464e00bfd732e14e.PNG" width="690" height="204">
<img src="/uploads/db1493/original/3X/d/8/d89c53626596f9a4f1de517cc89b84b4f5fc7f86.PNG" width="690" height="273">
<img src="/uploads/db1493/original/3X/b/2/b2e55e55226a1041df80f51eb6d2f19872e6be11.PNG" width="690" height="205">
<img src="/uploads/db1493/original/3X/d/a/da48edf965d842f96363c1f3a8cdb7c16ddd72d3.PNG" width="690" height="289">

@oneafrikan Thanks for the advice! I will definitely consider. College student budgets don't work too well with such an expensive hobby :P

Now while I'm waiting for the boards, time to go back to firmware development for the ESC...
```

---
## \#40 Posted by: raphaelchang Posted at: 2016-10-21T19:32:22.099Z Reads: 497

```
PCBs arrived!
<img src="/uploads/db1493/original/3X/d/b/db3a1fee7b0ac6cf85ead50699fbe8ec6635b27a.jpg" width="666" height="500">
Time to solder...
```

---
## \#41 Posted by: Jinra Posted at: 2016-10-21T19:41:31.931Z Reads: 479

```
I'm almost done with my build but my BMS seems to be DOA. I would love a BMS in this form factor, good luck!
```

---
## \#42 Posted by: IDVert3X Posted at: 2016-10-21T19:44:07.529Z Reads: 474

```
Looks great!
I was just wondering: in the specs, you say 3A max charge current.
Isn't it too low to be used with regenerative breaking?
```

---
## \#43 Posted by: raphaelchang Posted at: 2016-10-21T19:49:21.319Z Reads: 473

```
@IDVert3X the charge current spec refers to the charging circuit (the boost converter), which is used when you plug in a power supply to charge your batteries. It can handle a much larger reverse current coming from the output (to the ESC), which happens in regenerative braking.
```

---
## \#44 Posted by: IDVert3X Posted at: 2016-10-21T19:51:06.626Z Reads: 475

```
Thanks for your fast reply!
Then it looks like a perfect solution for my next project!
```

---
## \#45 Posted by: Pantologist Posted at: 2016-10-21T20:00:47.669Z Reads: 464

```
Awesome! You are doing them by hand or do you have access to a hot air station at least?
```

---
## \#46 Posted by: TheCheat Posted at: 2016-10-21T20:01:36.531Z Reads: 462

```
Regarding the ESC, I know for a fact I'd buy into an FOC ESC with higher max current. The VESC is 80(?) amps if I'm not mistaken.
```

---
## \#47 Posted by: raphaelchang Posted at: 2016-10-21T20:03:30.403Z Reads: 451

```
I have a hot air station, so I just reflow the parts one region at a time.
```

---
## \#48 Posted by: SORRENTINO Posted at: 2016-10-21T20:04:38.298Z Reads: 440

```
Cant wait to try out the esc. Thats what im waiting for. No DRV and 80amps constant sounds like a winner to me!
```

---
## \#49 Posted by: raphaelchang Posted at: 2016-10-21T20:06:10.145Z Reads: 443

```
The ESC uses DirectFETs and has a pretty neat power stage layout, so I do think it will be able to handle higher current. I will post more updates/info about the ESC soon...
```

---
## \#50 Posted by: SORRENTINO Posted at: 2016-10-21T20:07:57.118Z Reads: 442

```
Are you going to post gerbers and bom for esc for us to test the esc eventually?
```

---
## \#51 Posted by: raphaelchang Posted at: 2016-10-21T20:14:08.950Z Reads: 435

```
The gerbers and BOM are already in the repo, but the firmware isn't quite ready for testing yet. I will let you guys know!
```

---
## \#52 Posted by: SORRENTINO Posted at: 2016-10-21T20:20:47.757Z Reads: 426

```
ahhh ok thanks!
```

---
## \#53 Posted by: Michael319 Posted at: 2016-10-21T21:01:14.082Z Reads: 425

```
Super hyped for the ESC! We need something to compete with the VESC. It will make both products better in the end.
```

---
## \#54 Posted by: JLabs Posted at: 2016-10-21T21:22:42.329Z Reads: 419

```
Great work! Cant wait to see it up and running!
```

---
## \#55 Posted by: Pantologist Posted at: 2016-10-21T21:31:07.780Z Reads: 425

```
So for the surface mount fuses, they seem to be great for space saving but you have to solder a new set to replace a blown fuse. That sounds like a pain if you accidentally go over the current rating.

The DieBie's two standoffs allow for Littlefuses to be used and easily replaceable. They will only increase the height by a few millimeters for a lot more functionality. 

Just a suggestion. ;)
```

---
## \#56 Posted by: raphaelchang Posted at: 2016-10-21T21:44:17.825Z Reads: 429

```
I did consider (very hard) to use standoff fuses, but the ones that I could find that could handle 150A were all huge and would make the PCB a lot bigger.

All the surface mount fuses in parallel should be able to handle 150A with no problem; the fuses should never blow under normal operation as the BMS should be able to protect itself before that. The fuses are intended to only be a last resort protection feature in case something like a battery short happens. It's not designed to be regularly replaced.

Of course, I'm open to any suggestions, as I know this isn't an ideal solution.
```

---
## \#57 Posted by: Pantologist Posted at: 2016-10-21T21:51:06.516Z Reads: 419

```
Oh Okay as long as it can cutoff load or the battery in time I that solves it.
```

---
## \#58 Posted by: Kaly Posted at: 2016-10-22T00:10:48.958Z Reads: 425

```
@raphaelchang on the same line of the fuse conversation above. How will this BMS behave in the case of a motor or esc short ?
```

---
## \#59 Posted by: Pantologist Posted at: 2016-10-22T00:30:13.996Z Reads: 437

```
If I am not mistaken, the fuses are inline with the negative side of the battery terminal on the board. Shouldn't it pop if there is a short either with the battery terminals or ESC?
```

---
## \#60 Posted by: raphaelchang Posted at: 2016-10-22T01:09:22.919Z Reads: 453

```
The fuses are inline at the negative terminal of the battery connection, so all current coming out of the battery returns through the fuses. If the BMS software does not turn off the discharge FET fast enough (in case of ESC/motor short) the fuses will blow (after a few milliseconds at >150A). Since motor overcurrent events are usually inductive, the current won't increase at a very fast rate, so the BMS should be able to respond in time to shutoff the load before the fuses blow.
```

---
## \#61 Posted by: cmatson Posted at: 2016-10-22T02:55:56.154Z Reads: 445

```
My BMS has also died.. would totally buy yours in a heart beat once you decide to sell them!
```

---
## \#62 Posted by: raphaelchang Posted at: 2016-10-22T09:02:05.296Z Reads: 446

```
After 10 hours of soldering...
<img src="/uploads/db1493/original/3X/f/c/fc62823b03b5c3df4fed3da1606619a6f0083b5c.jpg" width="666" height="500">
```

---
## \#63 Posted by: akira Posted at: 2016-10-22T09:38:10.069Z Reads: 432

```
Sweet !!
Are you using a hot air station or a reflow oven ?
```

---
## \#64 Posted by: aldopopp Posted at: 2016-10-22T10:11:27.812Z Reads: 431

```
He already replied, hot air station ;)
```

---
## \#65 Posted by: akira Posted at: 2016-10-22T10:13:08.675Z Reads: 431

```
Sorry for the repeat. 
It is just that I was messing up with my hot air station yesterday to solder a poor vedder antispark !!!
Amazing what the same tool can do when used by skilled hands !!
```

---
## \#66 Posted by: chipoi84 Posted at: 2016-10-22T14:32:42.291Z Reads: 430

```
Hi, can you tell me the cost of all of the components including the pcb?
```

---
## \#67 Posted by: Pantologist Posted at: 2016-10-22T14:55:04.684Z Reads: 423

```
The BOM and Gerber files are in the GitHub. BOM is the Bill of Materials so you can use that to find the components and their prices.

From OshPark the PCBs will be around $12 each for the Infinity and BMS PCBs
```

---
## \#68 Posted by: chipoi84 Posted at: 2016-10-22T15:07:44.956Z Reads: 421

```
Found it. I couldn't find it before because the list of materials is in "Battman.XLS" file instead of BOM.
```

---
## \#69 Posted by: raphaelchang Posted at: 2016-10-22T19:36:51.301Z Reads: 418

```
The BOM prices are currently (on mouser) ~$120  for the ESC and ~$100 for the BMS. The ESC price drops to ~$90 and the BMS price drops to ~$80 at 10 though, so ordering in bulk would make it much cheaper.
```

---
## \#70 Posted by: Hummie Posted at: 2016-10-22T22:16:52.779Z Reads: 420

```
School can wait make these!
 It looks like the capacitor is siting on the fet wouldn't that cook it?
```

---
## \#71 Posted by: raphaelchang Posted at: 2016-10-23T00:47:39.034Z Reads: 422

```
It's very close, but the contact area is very small/not touching.

School is already waiting :)
```

---
## \#72 Posted by: Michaelinvegas Posted at: 2016-10-23T03:03:58.305Z Reads: 427

```
We just want innovators to be slaves for ESk8 .... it's a sickness lol
```

---
## \#73 Posted by: EMC75 Posted at: 2016-10-23T03:11:53.115Z Reads: 421

```
Read up on your site earlier today about all the iterations you went through to get to a working and more reliable ESC. 
Not sure where you find the time to get this all done. Absolutely amazing work!
```

---
## \#74 Posted by: raphaelchang Posted at: 2016-10-23T08:25:04.623Z Reads: 426

```
While I'm bringing up the new BMS, here's a list of significant features I've added for the next version (I tend to start designing the next iteration before the previous version arrives):

* Increased balance current to ~100mA
* Buzzer for notification
* Real-time clock and calendar IC with alarm to periodically wake up BMS (for battery storage discharge, other functions?). Powered by lowest cell, so as long as balance connector is plugged in, the RTCC will be tracking time.
* Switchable gain on current sense amplifier for increased resolution during low current while allowing for high current measurement (better SOC calculations)
* Reduced sleep supply current to <10uA (battery pack voltage dividers, which consumed 100-200uA before, are now disconnected in sleep mode)
```

---
## \#75 Posted by: IDVert3X Posted at: 2016-10-23T09:27:33.479Z Reads: 405

```
What about a watch battery for the RTC?
It's quite common solution, I use it in many projects and the battery lasts forever...
```

---
## \#76 Posted by: webst Posted at: 2016-10-23T11:40:16.724Z Reads: 393

```
Then think how many forevers would it last on 10s4p power bank. It's just another component that you already have there in abundance.

Edit: removed double "would"
```

---
## \#77 Posted by: IDVert3X Posted at: 2016-10-23T12:05:51.371Z Reads: 401

```
That's right, but if you do maintenance and you disconnect balance connector, RTC will reset and you have to reconfigure it again.
```

---
## \#78 Posted by: webst Posted at: 2016-10-23T14:13:03.676Z Reads: 403

```
What kind of battery maintenance do you have in mind? Why would I ever want to disconnect part that once connected becomes integral part of battery bank?
```

---
## \#79 Posted by: Pantologist Posted at: 2016-10-23T14:26:37.994Z Reads: 402

```
I guess it depends on how you have your BMS placed in your enclosure. A properly made battery pack with integrated BMS won't need to be disconnected.
```

---
## \#80 Posted by: Michael319 Posted at: 2016-10-23T15:16:46.914Z Reads: 407

```
http://hackaday.com/2016/10/22/supercapacitor-uses-no-carbon

You should use supercapacitors! Lol
```

---
## \#81 Posted by: IDVert3X Posted at: 2016-10-23T15:56:10.312Z Reads: 415

```
[quote="Michael319, post:80, topic:8952"]
You should use supercapacitors! Lol
[/quote]

Supercapacitors are really cool, I have few of them at home, BUT they have:

+ terrible leakage current
+ bad capacity to size ratio

In human speech: they will self-discharge pretty quickly ( few days ) and the pack needs to be huge.

@webst
When you need to change puffy or old LiPo ( ~200 charge cycles ? ), rearrange things etc.
But yeah, those are things that don't happen often...
```

---
## \#82 Posted by: raphaelchang Posted at: 2016-10-23T17:56:15.212Z Reads: 401

```
I'm running out of space on the board to add more stuff :P

I think that since most of the time your balance connector is plugged in, this will be fine for most situations. In case of maintenance, it should be really easy to reset the time (i.e. click a button in the GUI to sync it to your computer). If a phone is connected through Bluetooth, it could even sync automatically through the phone when it detects that it's been reset. Either way, this is only required if you care about the actual time; the alarm feature should keep working regardless.
```

---
## \#83 Posted by: Michaelinvegas Posted at: 2016-10-23T18:10:45.677Z Reads: 400

```
[quote="raphaelchang, post:82, topic:8952"]
I'm running out of space on the board to add more stuff :stuck_out_tongue:
[/quote]

Does that mean the DJ mixer is out?
```

---
## \#84 Posted by: Pantologist Posted at: 2016-10-23T19:43:06.566Z Reads: 392

```
Have you considered making a led SOC gauge or on and off switch unit for the BMS? Maybe even have a Bluetooth chip on the same PCB so you can read data from the BMS and ESC?
```

---
## \#85 Posted by: raphaelchang Posted at: 2016-10-23T19:59:10.677Z Reads: 396

```
I've been thinking about a lot of different plug and play modular PCBs to connect to the BMS and ESC. SOC gauge and power switch would be simple, another idea is to have a Bluetooth "sniffer" on the CAN bus to intercept messages from both the BMS and ESC and send them out.
```

---
## \#86 Posted by: Stef Posted at: 2016-10-23T20:45:36.972Z Reads: 394

```
Hi Raphael! I enjoyed reading about your projects on your website. Great to see passionate students working on technology that I think is important for a sustainable future, as well as a fun one! There is a lot of demand for better and more ESC options for electric skateboards in a growing esk8 community.

I will be at MIT during the spring semester+summer as a visiting graduate research student, would enjoy meeting up, seeing your work and sharing ideas. My background is precision mechanical and mechatronics.
```

---
## \#87 Posted by: Pantologist Posted at: 2016-10-23T20:45:47.396Z Reads: 411

```
It would be awesome if you could put them all on one external PCB, that would be fantastic and very space saving. 

For the power switch I was thinking having a long press 4-8 seconds to be the on and off toggles and a single press, 1-3 seconds having the SOC gauge display. 

Also while the BMS is connected to a charger and charging the SOC gauge will blink indicated that the battery is charging. 

Having a "smart" SOC gauge would be great since we really don't have something like this for the community. 

Here's a table from Bestech.
https://i.snag.gy/wAFpdg.jpg
```

---
## \#88 Posted by: raphaelchang Posted at: 2016-10-23T20:58:06.036Z Reads: 392

```
I think a PCB with a button and 5 WS2812 LEDs would work for this (would also allow for different color SOC displays). The button timing (and other customizable features) would be configurable through USB. Seems like a pretty simple PCB, I could put one together sometime.
```

---
## \#89 Posted by: webst Posted at: 2016-10-23T21:12:30.150Z Reads: 381

```
Don't you all think that 5$ 1,3"OLED screen with 128X64 resolution and I2C and SPI would be much better? I see it like this:
1. Bluetooth and iOS/Android app + Leds - best option but app to maintain etc.
1. OLED - you can do without phone app, cheaper, faster, if you want to analyse more data connect computer
2. Leds only - too easy

edit: changed 3$ 0,96" to 5$ 1,3", I just run my 0'96" oled screen and it's too small even for remote
```

---
## \#90 Posted by: jackw Posted at: 2016-10-23T21:18:52.883Z Reads: 377

```
Why not the option for both like it has been said? On separate boards. That way the easier LED option can be utilised for the people whom this would suit best and the OLED/LCD could come later as I would assume that would take a lot more development.
```

---
## \#91 Posted by: Pantologist Posted at: 2016-10-23T21:21:19.612Z Reads: 392

```
Yeah you can do either one. You don't have to change the original PCBs at all. Just looking at a set of LEDs would be easier to read and more simple. Also with LEDs you can actually easily make them water resistant or seal them somehow. It would be harder to do with a screen I think. 

I just want a simple solution. Looking at app vs a small screen on the board would be easier also.
```

---
## \#92 Posted by: webst Posted at: 2016-10-23T21:28:56.898Z Reads: 396

```
But app needs to be maintained, new os revision might make it obsolete. Using OLED screen with easily accessible libraries is easiest option to have it all from both worlds. You can have all data you need on this little screen protected by piece of plexi. Just take a look at possibilities:

http://g03.a.alicdn.com/kf/HTB1yHi4IpXXXXcVXpXXq6xXFXXX3/Free-shipping-0-96-inch-128x64-Yellow-Blue-oled-display-module-LM096-128064-oled-led-lcd.jpg
```

---
## \#93 Posted by: Stef Posted at: 2016-10-23T23:26:24.243Z Reads: 396

```
I like the idea of having a little screen on the board that is multifunctional for configuring the ESC&BMS, as well as functioning as SOC(with charging info) and speed gauge. With charging info you could think of confirming its charging or done charging, showing time left till full charge and the projected range in km or miles on the current charge. It would be even more awesome if the input device would be the remote, the throttle would make for a great scroll wheel!

Current SOC gauges also dont give an accurate representation of the range that is left, due to the non-linearity between the volts in the pack VS the Wh in the pack. This should be easy to solve unless different lipo cells have wildly different voltage to Ah-left curves.

The next big step for a SOC gauge would be displaying the projected left-over range in miles or kilometers. This would require GPS along with the battery voltage for it to become accurate without requiring user input. Alternatively you could calculate the traveled distance based on motor RPM and user input on wheel diameter+drive ratio. When making a production board the user input is not required as the drive ratio and wheel diameter are known. I think this only has significant added value when boards get enough range so that it can be used multiple days on a single charge and users lose track of how far the remaining charge can bring them.

I think the most important improvements are to be made in the ESC. I personally just want the smoothness and quietness of a VESC without all its drawbacks:

* Reliability is still an issue whilst it actually being quite expensive.
* Lack of housing sucks in terms of durability and ease of install (VESC X is great but quite expensive)
* Requiring careful configuration on a pc before it can be used. Note that I think config options are great, don't get rid of them, but if it already works from the box and the config options are easy to use then its much better!
* 60A continuous limit is a bit on the low side, forces you to go beyond 6S to get more than 1300W power out of a single drive which typically makes your build more expensive.
* The ERPM limit is a bit of a pain too, it limits the KV of the motor you can use based on the voltage you're running. This along with the 60A limit really couples your choice of motor+battery+drive ratio+charging system to achieve a certain performance level whilst working in the reliable limits of the VESC. 

Sorry if this was TL:DR :sweat_smile:
```

---
## \#94 Posted by: webst Posted at: 2016-10-24T20:00:38.104Z Reads: 382

```
I thought this thing through and why bother with BMC or ESC LCD while there should be and could be only one LCD on a remote. I deliberately exclude phone app as it should be something extra. Basic info info should be in your hand. I quickly made a mockup of how 5$ 1,3" 128x64px screen could look like:

<img src="/uploads/db1493/original/3X/e/0/e0adeb91c540b513a2629b170fbcb2c5bfc7e118.png" width="128" height="64">

Also there should be, built into BMS or standalone, way to use this huge battery as power bank so you could charge your remote while riding or just use single wall outlet while charging both.
```

---
## \#95 Posted by: Stef Posted at: 2016-10-25T00:35:09.969Z Reads: 375

```
Turns out some people on the forum are already experimenting with telemetry on the controller:

http://www.electric-skateboard.builders/t/ultimate-vesc-controller/6014
```

---
## \#96 Posted by: Pantologist Posted at: 2016-10-31T04:22:24.519Z Reads: 364

```
Now that I think about it @raphaelchang, the + and - terminals for Load, battery and charging seem awfully close to each other. Is that safe for voltages of around 50V if someone was to use a 12S Lipo config? I feel like they could arc or easily be shorted together if the soldering job is not that great or if while soldering, the two make contact with each other. If you widen the PCB by a few MM, it should allow for better spacing between + and - pads.
```

---
## \#97 Posted by: raphaelchang Posted at: 2016-10-31T04:52:55.671Z Reads: 363

```
I've increased the spacing between the pads a bit in the next version. IPC standards ([http://www.smpspowersupply.com/ipc2221pcbclearance.html](http://www.smpspowersupply.com/ipc2221pcbclearance.html)) say that 0.1mm should be safe for 20V (charging pads) and 0.6mm should be safe for 50V (battery + output pads), and the standards are usually pretty conservative. The pads are also pretty wide for even 10 AWG wire, so it shouldn't be hard to solder the wires at a safe distance from each other. Also, I don't think you should ever solder live wires regardless of how far away they are from each other; it's too easy to get out of your control and fry everything in its way (personal experience).
```

---
## \#98 Posted by: Pantologist Posted at: 2016-11-06T19:18:36.668Z Reads: 369

```
So is this the final update to the PCB? 

How are the BMS units you made working out for ya?

[quote="raphaelchang, post:97, topic:8952"]
say that 0.1mm should be safe for 20V (charging pads)
[/quote]

Shouldn't you space the charging pads a bit more since most people will be using batteries in the 30-50V range?
```

---
## \#99 Posted by: DanButcher Posted at: 2016-11-06T21:28:22.937Z Reads: 362

```
Did you consider using ESP8266 Wi-Fi module? It is arduino compatible, got possibility to use it as an access point (nodemcu). You can easly setup server with all necessary informations, also this device is capable of pwm. Easy to implement with your esc as an wirelesss communication protocol and controller. And fully functional board cost just 3$.
```

---
## \#100 Posted by: raphaelchang Posted at: 2016-11-07T08:58:52.032Z Reads: 396

```
@Pantologist  The version I am currently working with is not the final version, I've just sent out the next version that adds buzzer + RTCC + improved current sensing. I am continuing to develop firmware to get everything working. I've found a few problems with the current units, which I've fixed in the next version that I just sent out. So far, the cell voltage reading circuit and the charging circuit are working. I'm working on other core features like balancing, current sensing, etc., as well as interfacing it with a GUI. I'll try to post an update showing stuff working soon.

The idea of the charging circuit is that you only have to supply a lower voltage (12-24V) such as from a laptop power supply, and the circuit will boost the voltage to the right voltage for any battery pack. This removes the need for custom voltage power supplies, and allows for adjustment of charge current and voltage on the fly. It also allows for CC/CV charging with any power supply vs. having to find a power supply with the exact voltage if you want to do CV charging. However, if you still want to use your power supply to directly charge your battery, there is the option of bypassing the charge circuit and directly connecting a charger (up to 40V for now) to the battery. Since it has to support 40V, I can space out the pads a bit more, but I don't think it will be a big concern.

@DanButcher What would be the advantage of a Wi-Fi module vs. something like Bluetooth for wireless connectivity? Wi-Fi is usually used for providing internet or networking between multiple devices, so I'm not sure what types of applications you had in mind with putting Wi-Fi on an ESC. However, as long as the chip you referred to has I2C, SPI, or UART capability, it would be possible to design a plug-and-play board to communicate with the ESC.

Speaking of Bluetooth, I've decided that the most elegant way to have both the ESC and BMS send data to a phone via Bluetooth is to put a CAN "sniffer" on the CAN bus. Since both the ESC and BMS will be sending data to each other over CAN already, the sniffer can just intercept these messages and forward them over Bluetooth for an app to display. This way, you only need one Bluetooth board to send data from both boards to the phone, and it requires minimal software changes on the ESC and BMS to work. Being on the CAN bus also keeps it from using any additional connectors on either board.

The NRF51822 BLE chip is meant to run custom firmware, so my current plan is to design a board with a CAN transceiver -> SPI interface -> NRF51822 chip, and program firmware onto it to read from the CAN bus and send over Bluetooth. This allows for other cool features in the future too, like over-the-air firmware updates to both the ESC and BMS and wireless configuration of both boards from a computer. I just started designing this PCB (I don't have much RF experience), so I'll probably be developing it slowly in parallel with the two main boards.
```

---
## \#101 Posted by: DanButcher Posted at: 2016-11-07T09:22:33.713Z Reads: 389

```
Yes this board  is capable of ADC, I2C, SPI and UART. Connection should be more stable, you can use this board as all in one solution ( wieless controller, phone app comunication module, pc communication module). 
In same time this board can send information to your phone and pass pwm signal from wireless controler to esc. Even wireless controler can be based on second esp8266 board and anybody could create his own controller for around 8$.
http://www.nodemcu.com/index_en.html

This board can do all things that you want to do over bluetooth and even much more. Huge community with ready to go solutions.

Example:
http://diydrones.com/profiles/blogs/wifi-telemetry-with-cheap-3-esp8266
https://www.youtube.com/watch?v=nz7vJ0woE0Y
https://github.com/lephiloux/esp8266-rc
```

---
## \#102 Posted by: bliz Posted at: 2016-11-07T14:48:01.235Z Reads: 378

```
Hi, the esp8266 can be very good for a remote system (it can also be a nice 3rd circuit with bsm and esc for more flexibility and to keep bms for bms only)

Ex, with wifi and some security, you can alway add bluetooth module or use only wifi. The board can work as ap, receive information with the esp8266 remote module for the control, and send periodically information like speed or power (temperature and more) to the remote or on a phone ect.

It's also possible to add a 128*64 oled display on board and/or remote, a gps :p, light control ect ^^

My first post here but i read this forum since a moment and you do a really great work on bms and esc !!!!!
```

---
## \#103 Posted by: Hummie Posted at: 2016-11-07T15:08:45.510Z Reads: 356

```
Looking forward to your end results.  How many watts would it be able to charge at?

How much power would the bms and esc consume? I like the idea of leaving the board permanently on and knowing the battery state constantly.
```

---
## \#104 Posted by: DougM Posted at: 2016-11-07T16:09:16.723Z Reads: 357

```
I would advocate for the communications method to be an add-on module, mostly because I want to stick with XBee.  The ESP8266 has been replaced with the ESP32 IIRC, so even though they are cheap they are probably near end of life.
```

---
## \#105 Posted by: alexmarin99 Posted at: 2016-11-07T16:29:30.865Z Reads: 347

```
This looks very very interesting!
How would you compare this ESC vs the VESC by Vedder in real world? How does it ride?
```

---
## \#106 Posted by: DanButcher Posted at: 2016-11-07T16:49:22.572Z Reads: 348

```
Well ESP32 IIRC got both wi-fi and bluetooth, code from ESP8266 in most of cases should be compatible with ESP32 IIRC. Still XBee is less powerfull and more expensive than ESP. So why would you want to stick with XBee?
```

---
## \#107 Posted by: Stevemk14ebr Posted at: 2016-11-07T16:56:39.286Z Reads: 349

```
I've actually done development on esp8266 and I can tell you it is a pain in the ass. The xbee modules have significantly better firmware and libraries. I had to recompile, reflash, and write my own library when using the esp. Xbee worked out of the box
```

---
## \#108 Posted by: DougM Posted at: 2016-11-07T17:05:34.871Z Reads: 352

```
[quote="Stevemk14ebr, post:107, topic:8952"]
Xbee worked out of the box
[/quote]

This.  

XBee just works.  And the range is fantastic, even at medium power levels I held the controller in my hand and sent the neighbor kid all the way to the end of the block and back without losing signal.
```

---
## \#109 Posted by: DanButcher Posted at: 2016-11-07T17:33:58.801Z Reads: 349

```
@Stevemk14ebr Indeed you need to flash nodeMCU to ESP, right now there is a lot of libraries. Do you think that without Xbee explorer  or shield this device will be as powerfull as ESP8266? 


@DougM Range of ESP8266 is also fantastic ( 300m+ only with pcb antena)

I'm not saying that Xbee is not a good idea but simply ESP8266 is standalone MCU and out of the box give you more possibilities. I know that Xbee will be easier to setup.

@Stevemk14ebr and @DougM both Xbee and ESP8266 got pros and cons.

ESP8266 features:
32-bit RISC CPU: Tensilica Xtensa LX106 running at 80 MHz*
64 KiB of instruction RAM, 96 KiB of data RAM
External QSPI flash - 512 KiB to 4 MiB* (up to 16 MiB is supported)
IEEE 802.11 b/g/n Wi-Fi
Integrated TR switch, balun, LNA, power amplifier and matching network
WEP or WPA/WPA2 authentication, or open networks
16 GPIO pins
SPI, I²C,
I²S interfaces with DMA (sharing pins with GPIO)
UART on dedicated pins, plus a transmit-only UART can be enabled on GPIO2
1 10-bit ADC
```

---
## \#110 Posted by: DougM Posted at: 2016-11-07T17:40:46.698Z Reads: 334

```
@DanButcher We totally agree then :-)  

My request isn't for XBee, my request is for modularizing the radio, so we have a choice.
```

---
## \#111 Posted by: raphaelchang Posted at: 2016-11-08T03:34:17.817Z Reads: 356

```
The point of making the radio chip separate from the main PCB (modular) was so that people were not restricted in their choice of a radio module. The ESP looks similar to the NRF chip, in that it is an SOC and requires firmware to be loaded. It should be possible to do something very similar to what I described (the CAN sniffer) with this chip. I am still going to stick with the NRF chip for my design for now, as it seems like this chip is the most common solution for Bluetooth (also, VESC 6.0 uses it). Also, with Bluetooth, it would be possible to do over-the-air firmware updates, whereas if the phone was connected to a WiFi hotspot it would not have internet to download the firmware.

@Hummie The charging circuit is able to charge at up to 240W (40V at 6A), but this is not a very useful number as it is a boost converter, so the max current depends on the input voltage. For example, boosting from 20V to 40V with 6A input would only output 3A at 40V, which is 120W. Regardless, I've specified the numbers so that it is possible to charge at a reasonable rate for any battery voltage.

@alexmarin99 I haven't tried my ESC in the real world, but it should feel the same (but with higher current limits) because it's just current/torque control.
```

---
## \#112 Posted by: raphaelchang Posted at: 2016-11-11T09:56:14.165Z Reads: 349

```
A quick video showing the BMS turning on the ESC using a power switch (the startup tune comes from the ESC, which I added just for fun and won't be there by default): 
[https://youtu.be/C7EROdycZ5Y](https://youtu.be/C7EROdycZ5Y)
```

---
## \#113 Posted by: DeathCookies Posted at: 2016-11-11T10:22:55.489Z Reads: 347

```
Can you add a BOM?

You are using 50ma for balancing. That sounds awfully long?

Do you have a feature to balance by a mouse click (Manually not every time)?
Can the charging current be increased? Imagine a 6P config (3A * 6P = 18A capacity). Charging it with 6A  1/3C would take 3 hours.
```

---
## \#114 Posted by: Maxid Posted at: 2016-11-11T11:27:30.214Z Reads: 342

```
Awesome work - I like where this is headed. Just please remove that startup sound :slight_smile:
It is one of the things that I don't like on my car ESC - just raises unnecessary attention.
```

---
## \#115 Posted by: DanButcher Posted at: 2016-11-11T11:45:41.533Z Reads: 336

```
I think that Raphael design this for electric skateboard, such huge battery(6p) would fit probably only in mountainboard,e-bike,e-scooter.
```

---
## \#116 Posted by: DanButcher Posted at: 2016-11-11T11:47:33.119Z Reads: 337

```
I think that this sound checks if frequency is generated properly.
```

---
## \#117 Posted by: korryh Posted at: 2016-11-11T15:56:19.260Z Reads: 341

```
Can you make it play the imperial march from starwars or at least be able to turn the beep off
```

---
## \#118 Posted by: raphaelchang Posted at: 2016-11-11T18:03:11.203Z Reads: 351

```
All this hate on startup tunes :P (I'm not a fan either). I did it just for fun, it will be configurable (default off) and you will even be able to write your own tune.

@DeathCookies The BOM is in the repository. The balancing is 100mA. You actually don't need that much balance current, as (hopefully) your cells are never that unbalanced in the first place, especially if you are balancing regularly. Charging your 18Ah pack at 1C is 18A, which is a ridiculous amount of power for a PCB of this size. I don't think you can easily find 18A power supplies either. However, you can choose to "bypass" the charging circuit, in which case the current is limited by only a 10A diode, so you could charge at 10A if you find such a power supply.
```

---
## \#119 Posted by: Pantologist Posted at: 2016-11-11T18:35:23.847Z Reads: 343

```
I know this is the version without the larger spacing, but even with increased spacing I feel like that the + and - pads are way too close. 

When soldering the battery tabs it seems way too easy to accidentally short out the battery. 

I'm probably getting annoying at this point. :grin:
```

---
## \#120 Posted by: SORRENTINO Posted at: 2016-11-11T18:45:42.308Z Reads: 337

```
Quite common to have these not that far apart. I come from drone building and the pdb spacing for wires is ridiculously close. Nothing a soldering iron cant fix with a swipe across the spacing to de-bridge any solder.
```

---
## \#121 Posted by: Pantologist Posted at: 2016-11-11T18:49:56.778Z Reads: 332

```
But with battery + and - connections, you will be shorting them right? Also drones aren't running at 20v to 50v. Arcing can happen at around 50v if I am not mistaken.
```

---
## \#122 Posted by: raphaelchang Posted at: 2016-11-11T18:52:40.126Z Reads: 325

```
Are you talking about soldering the battery tabs on directly? That sounds like something you would need a custom PCB design for (the pad locations would be to match up to your battery exactly). The pads here are designed for wires to be soldered on before connecting the battery. Moving them far apart to allow for safe soldering of live wires would require a complete redesign. I can space them out even more, but i still don't think it's a good idea to solder things live.
```

---
## \#123 Posted by: SORRENTINO Posted at: 2016-11-11T18:54:06.787Z Reads: 327

```
We have a couple drones that run 6s. Solder wont stick to the pcb so running the iron across the spacing make the solder wick back into the solder on the pads. Im pretty sure Raphael addressed the arching thing and spaced them out enough for no arch to occur.
```

---
## \#124 Posted by: DeathCookies Posted at: 2016-11-11T18:56:16.182Z Reads: 332

```
You are right. It is called Battman.xls . I searched for BOM :smiley:

This here does have a lot of power?!
https://www.amazon.com/gp/product/B01GFVI6R6/ref=pd_sbs_23_4?ie=UTF8&pd_rd_i=B01GFVI6R6&pd_rd_r=GPZNM1HGSVPB8RH87F1T&pd_rd_w=kg1KU&pd_rd_wg=KtrTJ&psc=1&refRID=GPZNM1HGSVPB8RH87F1T
```

---
## \#125 Posted by: Maxid Posted at: 2016-11-11T19:53:01.411Z Reads: 326

```
this thing will never ever be able to charge at 18A. It says 900W but check the German amazon website and you will find a review of a guy telling exactly this. Also you would still need an actual power supply supplying the DC voltage.
```

---
## \#126 Posted by: smurf Posted at: 2016-11-11T20:21:51.578Z Reads: 320

```
I have a  adjustable 32-40V 15A power supply for my drok coming on the slow boat from China right now
```

---
## \#127 Posted by: Maxid Posted at: 2016-11-11T20:25:22.543Z Reads: 321

```
There will be losses (quite large ones) so with a 15A supply you will not be able to actually charge with 15A.

What kind of boards are you guys riding anyway that you could ever need such a charging current?
```

---
## \#128 Posted by: smurf Posted at: 2016-11-11T20:35:23.743Z Reads: 319

```
6 parallel charging at 1.75 equals 10.5
And some battery's can be fast charged at 2A
```

---
## \#129 Posted by: Maxid Posted at: 2016-11-11T21:19:47.794Z Reads: 319

```
Who actually uses 6P batteries and needs to charge them as quickly as possible? Also fast charge usually means more than 4A per cell not just 2A. You can safely charge at 1C although slower is always better to get healthier cells for longer.

Assuming 10S6P that would result in something like 540Wh up to 650Wh. That gives you more than 50km in range - who needs to honestly fast charge after a 50km ride?
```

---
## \#130 Posted by: 2-alex-2 Posted at: 2016-11-11T21:23:11.575Z Reads: 314

```
So my 6s4p hg2 are 4a max charge so your saying I can actually use this bms to charge at 16a because of the 4p ?
```

---
## \#131 Posted by: Maxid Posted at: 2016-11-11T21:33:17.383Z Reads: 322

```
I don't know the max charge current of @raphaelchang s BMS but in general you can. Parallel cells "add" the individual max charge current to give you the actual max current for the pack. However as I said you should always charge as slow as possible to keep them healthy for longer.
```

---
## \#132 Posted by: 2-alex-2 Posted at: 2016-11-11T21:38:14.383Z Reads: 319

```
Yea I understand as seen a 5a charger but wasn't sure as max was 4a and my bms can only handle 5a but I do like these bms and esc just hope they are a sensible price.
```

---
## \#133 Posted by: SageTX Posted at: 2016-11-11T22:41:55.530Z Reads: 330

```
[quote="raphaelchang, post:118, topic:8952"]
you will even be able to write your own tune.
[/quote]

Make it the Batman tune by default "na na na na na na na na, na na na na na na na na"
```

---
## \#134 Posted by: raphaelchang Posted at: 2016-11-12T05:37:50.214Z Reads: 347

```
Let me try to explain the charging circuit with a little more detail. The circuit is a boost converter with a current limit on the input (as most boost converters do) of 6A. By conservation of power, the product of input voltage and input current must equal the product of output voltage and output current (minus efficiency losses). For example, if you supply 24V and want to charge a 48V battery, 24V*6A = 144W, so you are limited to 144W/48V = 3A at the output. Therefore, the closer your input voltage is to your desired output voltage, the closer to 6A you will be able to charge at.

There is also the option of bypassing the boost converter and charging the battery directly with the power supply, the traditional method. To explain this, this is the schematic of the charging circuit. C+ is the input supply and CHG+ is the output to the battery. The boost controller IC is on the left and a DAC is on the right.
<img src="/uploads/db1493/original/3X/2/a/2a64ab32ba5f8acea1c902245f5eb79d20bc6d13.png" width="500">

Using the DAC, the circuit is able to adjust the output voltage of the boost converter by injecting a voltage into the feedback pin of the IC. Normally, the desired voltage would be higher than the input, so the controller would be switching the MOSFET to boost the voltage up. However, when the bypass option is selected in the configuration, the firmware will make the DAC force the boost converter to output a very low voltage, lower than the supply, which the converter cannot do. Therefore, it keeps the MOSFET off, and the circuit simply becomes C+ -> inductor -> diode -> CHG+. This simple current path allows for a higher current because the controller isn't involved. The charge current will be the current rating of the power supply, but the ratings of the inductor and diode mean that the current should not exceed 8-10A.

Currently there is a limitation in the boost controller IC that limits the input to 42V, so any battery pack that is more than this will require the use of the boost converter. Using the boost converter means that you can have CC/CV charging with any input supply because the voltage can be controlled accurately, whereas if you bypass the circuit, you can only have CV charging if your power supply is exactly the CV voltage of the pack. If you plug in a higher voltage supply, the BMS will simply cut off the charging (with another MOSFET) when the battery pack reaches its max voltage, so you will only have CC charging.

Long explanation, but I hope this clears things up a bit for those who are curious.
```

---
## \#135 Posted by: JTAG Posted at: 2016-11-12T15:49:21.012Z Reads: 333

```
[quote="raphaelchang, post:134, topic:8952"]
This simple current path allows for a higher current because the controller isn't involved. The charge current will be the current rating of the power supply, but the ratings of the inductor and diode mean that the current should not exceed 8-10A.
[/quote]

The diode will dissipate quite a bit of power. at about 10 amps this could easily be close to 8W (0.8V diode drop). I have the same limitations in my BMS design. There is just no easy and cost effective was of solving this.
```

---
## \#136 Posted by: raphaelchang Posted at: 2016-11-21T03:31:35.271Z Reads: 333

```
Here's a bit of suspense for you guys:
https://youtu.be/9_kyLGOOu24
```

---
## \#137 Posted by: rpn314 Posted at: 2016-11-22T20:29:06.223Z Reads: 329

```
Now you're just teasing :)
```

---
## \#138 Posted by: Pimousse Posted at: 2016-11-23T08:07:21.269Z Reads: 332

```
Wow, it looks ridiculously small !!
Great job !!

Wires seem to be soldered very close.
At least for my soldering skills...
```

---
## \#139 Posted by: raphaelchang Posted at: 2016-11-24T04:36:15.022Z Reads: 333

```
Cell balancing:
https://www.youtube.com/watch?v=VIm5HILlGs0
```

---
## \#140 Posted by: TeleRando Posted at: 2016-11-24T04:51:01.838Z Reads: 332

```
Sign me up!!!

Boom!
```

---
## \#141 Posted by: WrinklyWink Posted at: 2016-11-24T09:05:06.711Z Reads: 330

```
[quote="Maxid, post:129, topic:8952, full:true"]
Who actually uses 6P batteries and needs to charge them as quickly as possible? Also fast charge usually means more than 4A per cell not just 2A. You can safely charge at 1C although slower is always better to get healthier cells for longer.

Assuming 10S6P that would result in something like 540Wh up to 650Wh. That gives you more than 50km in range - who needs to honestly fast charge after a 50km ride?
[/quote]
in [Exhibit A](http://www.nkon.nl/sk/k/30q.pdf) we have a spec sheet for Samsung 30Qs. on page 3/17, it states max charging current at 4 Amps and standard charging current at 1.5 Amps. Then look at page 8/17 and 9/17. With 4 Amps charging it reduces to 72-74% capacity with 250-300 cycles.

in [Exhibit B](http://www.batterysupports.com/43v-44v-504v-20a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-442.html) we have a 20 Amp 12S charger available for sale and shipment now.

With a 12s6p pack 20 Amps would spread over 6 batteries width so: 3.3 Amps per a cell.

You would hurt the life of the battery somewhat with these aggressive charging currents, however it is well within safety spec. Still can be nice as an option to fill those batteries 5 times faster than a 4A charger.

Anyways my point is I'm starting to prefer the idea of small capacity but rapid charge ability, and there are batteries out there which welcome such behavior albeit at an expense of capacity. This would make for a small quick commute board, which lives by the charger constantly.


[quote="raphaelchang, post:139, topic:8952, full:true"]
Cell balancing:
[/quote]

I'm looking forward to purchasing this in the future. Do you have a sort of time-frame? I searched the entire post for words like "date" and "when" but nothing applicable came up. If you don't have a timeline that's also fair. Some times food has to be prepared accordingly, so I understand. Like TeleRando.. sign me up!
```

---
## \#142 Posted by: Maxid Posted at: 2016-11-24T09:18:39.336Z Reads: 314

```
Not sure what you are trying to tell me here :confused:
What does all that have to do with my post?
```

---
## \#143 Posted by: raphaelchang Posted at: 2016-11-25T00:43:49.691Z Reads: 306

```
I'm working hard on finishing this and am a bit ahead of my predicted timeline, so I *might* be ready for beta testing by January next year.
```

---
## \#144 Posted by: TarzanHBK Posted at: 2016-11-25T09:15:29.761Z Reads: 306

```
did you already calculated costs for this masterpiece?
```

---
## \#145 Posted by: raphaelchang Posted at: 2016-11-25T10:10:26.371Z Reads: 297

```
It looks to be about $105-110 in components right now, but I do plan to sell it so if there are enough orders the price should be around $100 each.
```

---
## \#146 Posted by: smurf Posted at: 2016-11-25T10:26:23.613Z Reads: 297

```
I think your gonna get enough orders
```

---
## \#147 Posted by: akira Posted at: 2016-11-25T10:43:52.880Z Reads: 310

```
Hi Raphael,
Do you plan to release the sources (gerber and firmware) ?
```

---
## \#148 Posted by: hexakopter Posted at: 2016-11-25T10:57:36.147Z Reads: 303

```
Do you have read the thread? :slight_smile:
There are links to his [GITHUB](https://github.com/raphaelchang) everywhere.

Incredible how fast the development goes @raphaelchang. :grin: Thumbs up. This will become THE "small killer BMS". Btw the Node Dashboard is not working for me. If I understand it correct I have to go to the battman-dashboard folder in the terminal and then just type "npm start". But that is not working for me. I am on OSX like you.
Have installed the latest Node including npm.
```

---
## \#149 Posted by: akira Posted at: 2016-11-25T11:16:15.242Z Reads: 297

```
I had when the thread started. But since Raphael said that he was willing to sell it, he might choose to keep the sources for the final version that he would sell himself. That is commonly done, no judgement of any kind from me.
```

---
## \#150 Posted by: raphaelchang Posted at: 2016-11-25T11:21:21.316Z Reads: 300

```
I have no plans to do that. This is a fully open source project, so I will keep everything up to date in the repos. The only requirement (by the license) is that if anyone modifies it they must make it open source as well.
```

---
## \#151 Posted by: TarzanHBK Posted at: 2016-11-25T11:29:14.016Z Reads: 292

```
i´ll probably be down for 2 chang BMS! I hate these big 10s 80A bricks
```

---
## \#152 Posted by: akira Posted at: 2016-11-25T11:37:28.143Z Reads: 288

```
Thumbs up for your open-source development. 
This is extremely appreciated. I will probably try to build one myself (for the fun of it) and donate for the dev.
Great work !
```

---
## \#153 Posted by: chinzw Posted at: 2016-11-25T18:47:10.582Z Reads: 285

```
Def buying one if you decide to sell them!
```

---
## \#154 Posted by: Eboostin Posted at: 2016-11-25T20:08:58.633Z Reads: 282

```
Are you saying that charging at 4A reduces the number of available battery cycles by ~25%?
```

---
## \#155 Posted by: hexakopter Posted at: 2016-11-25T20:46:29.035Z Reads: 303

```
Raphael helped me solving my problem with the GUI. Thanks for that.

I have done a Mouser list with all the parts available there. I have put exactly the number of pieces needed into the shopping list, also when for example 10 resistors would be cheaper when you need just five. You can find it [here](http://www.mouser.de/ProjectManager/ProjectDetail.aspx?AccessID=80114e51eb). (without engagement)
Mouser don't have the JST jacks/ the sunLED RGB-LED and the very expensive Battery Monitor IC (around 17$) available. (this parts are available on digikey) Don't forget that the mouser price of 77,6€ are without 19% taxes and a four layer PCB isn't cheap. Also notice that Raphael is still in the improvement phase, so this calculation I did for me is not matching the final layout.

@raphaelchang Do you think the 50V caps are specced well? I just ask because a full 12s Lipo is 50.4V and we saw with the VESC, that this "very close or underrated" specs can make problems. When you look the capacity close to the max rated voltage it is a lot lower than the stated capacity. This effect is even bigger because of your 0402 selection.

Are you planing to sell the part sets or the complete build BMS? (So you have a pick and place machine somewhere available, because hand soldering that much 0402 components would be a pain in the a** for several PCBs)

Do you have plans to make that beauty also work together with the VESC from Benjamin Vedder over CAN or is it mostly for your Infinity hardware?
Thanks for everything.
```

---
## \#156 Posted by: raphaelchang Posted at: 2016-11-25T21:43:02.864Z Reads: 297

```
I've updated the BOM to reflect the latest design. The PCB is around $12 each on OSH Park. The total price will come to around $120 if you decide to assemble it yourself. Also, there's another store called [Arrow Electronics](https://www.arrow.com/en/products/ltc6803ig-3pbf/linear-technology) which sells the LTC6803 for only $13, but it is often out of stock. They have a lot of parts that are cheaper than Mouser and Digikey though.

Most of the 50V caps are not used for the battery voltage. The one that is 50V on the battery line is a high quality electrolytic capacitor, which does not have this problem. Thanks for noting this though, I went back and checked all the caps to make sure.

I'm definitely not planning to hand solder all the boards :slight_smile: (I've almost had enough of that).  I am planning to outsource it in bulk to a PCB fab for assembly, and set up a system here for quality testing. The quality will be higher and the cost will be lower this way.

Working with the VESC would require changing his firmware, so I am first getting it to work wth my ESC. The interface is over CAN though, so it should work with either ESC if the firmware is set up. However, once both boards are ready, I'm planning on adding a lot of integrated features that would make the system a lot more advanced if both my BMS and ESC were used together (i.e. simultaneous firmware updates, unified app, etc.).
```

---
## \#157 Posted by: hexakopter Posted at: 2016-11-25T23:16:46.320Z Reads: 303

```
[quote="raphaelchang, post:156, topic:8952"]
Also, there's another store called Arrow Electronics which sells the LTC6803 for only $13, but it is often out of stock. They have a lot of parts that are cheaper than Mouser and Digikey though.
[/quote]
I have no experience with them. Will check them out. Was thinking they are expensive or was that in the past or has to do with the shipping to europe?

[quote="raphaelchang, post:156, topic:8952"]
Most of the 50V caps are not used for the battery voltage. The one that is 50V on the battery line is a high quality electrolytic capacitor, which does not have this problem. Thanks for noting this though, I went back and checked all the caps to make sure.
[/quote]
Good to know. I haven't checked what they are used for, just noticed the 50V in this 0402 package and was thinking it is used for battery voltage. :blush:
[quote="raphaelchang, post:156, topic:8952"]
I'm planning on adding a lot of integrated features that would make the system a lot more advanced if both my BMS and ESC were used together
[/quote]
That sounds amazing. I know how komplex Field Oriented Control is and the step to sensorless FOC is even a lot bigger, but I think that is needed so eBike and eSkateboards could use it. I think adding a magnetic encoder isn't possible for most people. But I read on your [website](http://raphaelchang.com/projects/) that you already are working on sensorless support. Really cool. :sunglasses:
```

---
## \#158 Posted by: DeathCookies Posted at: 2016-11-28T07:31:49.133Z Reads: 307

```
[quote="hexakopter, post:155, topic:8952"]
Mouser don't have the JST jacks/ the sunLED RGB-LED and the very expensive Battery Monitor IC (around 17$) available. (this parts are available on digikey) Don't forget that the mouser price of 77,6€ are without 19% taxes and a four layer PCB isn't cheap.
[/quote]

[quote="raphaelchang, post:156, topic:8952"]
I've updated the BOM to reflect the latest design. The PCB is around $12 each on OSH Park. The total price will come to around $120 if you decide to assemble it yourself.
[/quote]

It would be better to buy huge amounts from mouser. If you will buy one circuit you will always pay 20-50% more than you would pay for 10 circuits each.

I have updated the qunatity of your shop link @hexakopter to ten and the result ist 564,33. That would be only 56€ for one set instead of 77,60€
Maybe we should make a group buy and get it somewhere assembled.
```

---
## \#159 Posted by: hexakopter Posted at: 2016-11-28T08:12:23.455Z Reads: 298

```
@DeathCookies Don't forget the expensive Battery Monitor IC and PCB price.
I have done a VESC group buy last time and I can tell you that it is a lot of work and hassle.
```

---
## \#160 Posted by: hexakopter Posted at: 2016-11-28T18:12:53.018Z Reads: 289

```
[quote="raphaelchang, post:13, topic:8952"]
120A continuous, 150A peak discharge current (may change)
[/quote]


Just something I noticed today. You have the IRF7749L1 as your discharge FET. How should that thing be able to let through 120A continuous current when it isn't cooled? Isn't something about the half more realistic, so around 60-70A? Or was your number calculated for using two FETs in parallel, but then because of the size you only choose one FET?
```

---
## \#161 Posted by: raphaelchang Posted at: 2016-11-28T18:27:21.009Z Reads: 281

```
Correct, I chose to use one FET because of size. A more realistic continuous current is 80-100A (slightly more than an ESC because it's not switching), but that is still enough for most people. Still need to evaluate that though.
```

---
## \#162 Posted by: Pimousse Posted at: 2016-11-29T14:59:40.003Z Reads: 281

```
Isn't it better to have redundancy with the FET ?
I encountered and also saw guys having issues with powerswitch and their FETs.
If FET fails (in blocking position) during braking, it also blows the VESC... :/

I'm really interested into your project, but this point scares me a bit and can't stop to think that a XT90s stays the most reliable on/off method.

What do you think about this point ?
```

---
## \#163 Posted by: raphaelchang Posted at: 2016-11-29T22:39:08.374Z Reads: 283

```
I think this is a valid point, but I am hesitant to make the change until I evaluate it under real conditions and decide that it is necessary. I don't want to increase the board size and add $5 to the cost without good reason.

Can you show me some specific issues people had with their FETs? If a FET fails open, there is still a reverse diode inside it that will allow regen current from the VESC to flow. If that diode blows as well, I have a TVS diode that will absorb the energy from the resulting voltage spike, so the VESC will still be protected. The concerns I have with 1 vs. 2 FETs are more for power dissipation reasons than redundancy.
```

---
## \#164 Posted by: JTAG Posted at: 2016-11-29T22:56:24.280Z Reads: 284

```
Double FET wont help, 98% of the FET's fail in dead short and only during switching.
```

---
## \#165 Posted by: Pimousse Posted at: 2016-11-30T11:10:19.803Z Reads: 287

```
Let me find the guy who blow his VESC because of the powerswitch failure.
It was during a braking, not while switching on/off.
```

---
## \#166 Posted by: raphaelchang Posted at: 2016-11-30T17:21:40.550Z Reads: 292

```
A power switch or connector failure will kill the VESC during braking, as there is no backup path for current to flow. In contrast, a MOSFET failure could actually have more redundancy. As @JTAG mentioned, MOSFETs do tend to fail in shorts, and they also have a body diode to allow reverse current. I think he also meant that MOSFETs usually fail only when switching fast (like in an ESC) because the transition period is when it sees the most load. When it's on or off, it's just a simple low/high resistance resistor.
```

---
## \#167 Posted by: ikjahaa Posted at: 2016-11-30T22:29:51.085Z Reads: 298

```
just letting you know, im loving your project !!
If you were able to provide me with an out-of-the-box, ready-to-use set of esc and bms ( no soldering ) then i'd defenatly be down for a set. 

keep us updated, love reading this post.

Regards :slight_smile:
```

---
## \#168 Posted by: treenutter Posted at: 2016-11-30T22:32:03.668Z Reads: 295

```
Looks great! nice work @raphaelchang we're all looking forward to seeing your progress!
```

---
## \#169 Posted by: raphaelchang Posted at: 2016-12-03T02:16:53.673Z Reads: 299

```
I have a few more logistics-related updates. BMS progress is going faster than anticipated, and I'm expecting to need beta testers in a month or so. Please **message me** if you are interested in testing the BMS. I'm looking to acquire around 50 initial units for testing, and the price will be around $110-120 for the initial units (slightly higher because of the lower quantity, exact cost will depend on how much interest).

As for the ESC, I haven't worked on it much because of the BMS, so it will still be a while. I'll hopefully have more updates on that soon.

On a side note, if you'd like to further support my development, I've created a donation link [here](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=AMHGZHZVS6X8S&lc=US&item_name=Battman%20BMS%20and%20Infinity%20ESC&item_number=1&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted). Everything will go towards prototyping costs (I'm basically buying a new BMS/ESC every time I make a new hardware version).
```

---
## \#170 Posted by: WrinklyWink Posted at: 2016-12-04T14:03:18.903Z Reads: 291

```
After ~200 cycles for the samsung 30q batteries.
```

---
## \#171 Posted by: Eboostin Posted at: 2016-12-04T17:49:48.761Z Reads: 289

```
I looked at the spec sheet and it is on a per battery basis. So a 4P pack charged at 4A, would that be 1A per cell or does each cell in parallel get the the full 4A. 

I have a few large packs and want to make sure they last as long as possible.
```

---
## \#172 Posted by: WrinklyWink Posted at: 2016-12-05T00:28:16.973Z Reads: 283

```
[quote="Eboostin, post:171, topic:8952"]
So a 4P pack charged at 4A, would that be 1A per cell or does each cell in parallel get the the full 4A.
[/quote]
1Amp per Cell.
Make sure the voltage matches
```

---
## \#173 Posted by: Pedrodemio Posted at: 2016-12-05T11:02:04.609Z Reads: 282

```
Great project, already signed up as beta tester

Two things that I remember I saw on the discussion:

- about the limits of the battery (maximum voltage, minimum voltage, etc) I thinks is better to leave everything numerically customizable instead of presets
- the low voltage cut-off be load dependent, it's something the vesc lacks. Since we push the battery's to the limit, we have significant voltage sag, so at most times there's still plenty of energy left but we hit the cut off. The strategy would be the BMS know the internal resistance and calculate the voltage drop due to the current flow, this could be measured or just a crude estimation, would be better than nothing

Edit:
And about the battery capacity display, a option with just simple leds, not ws2812, would be interesting, the way boosted uses, compact and simple to design, i don't know how many pins you have left, but nothing that a multiplexer can't do
```

---
## \#174 Posted by: raphaelchang Posted at: 2016-12-05T17:32:55.758Z Reads: 279

```
All numbers are customizable in the dashboard. Calculation of voltage sag is possible, but I thought that the purpose of the low voltage cutoff is to keep the voltage from dropping to damaging levels even under load. Another way would be to only measure cell voltages when the current draw is low enough.

There are two accessory pins, but they support I2C so you could use an LED driver.
```

---
## \#175 Posted by: SORRENTINO Posted at: 2016-12-05T17:46:39.189Z Reads: 279

```
What would calculating the voltage drop even help with? End of day you should never go below a certain voltage per cell even when under load.
```

---
## \#176 Posted by: Pantologist Posted at: 2016-12-05T17:54:59.198Z Reads: 277

```
It would make battery SOC more accurate. I think the method is called columb counting or something like that. 

Inboard even experiences early battery cutoff because the voltage sag is so high with their battery. Their battery readings are also of because they are simple meters based in voltage readings.

Having your board cut off from hard acceleration is not fun. This would change that.
```

---
## \#177 Posted by: SORRENTINO Posted at: 2016-12-05T17:57:32.839Z Reads: 272

```
So would it gradually cutoff since it can calculate the sag before hand instead of the instant cuttoff?
```

---
## \#178 Posted by: Pedrodemio Posted at: 2016-12-05T18:21:37.152Z Reads: 298

```
[quote="raphaelchang, post:174, topic:8952, full:true"]
All numbers are customizable in the dashboard. Calculation of voltage sag is possible, but I thought that the purpose of the low voltage cutoff is to keep the voltage from dropping to damaging levels even under load. Another way would be to only measure cell voltages when the current draw is low enough.

There are two accessory pins, but they support I2C so you could use an LED driver.
[/quote]

Nice, from what i read i thought it would be predefined configuration. So it's easy to put just a few leds

From all i've read across the years, the problem is rest voltage too low, no problem going low during heavy current draw, it's actually desirable if you want to get most energy out of the battery

watch from 16:30, it shows the diference in booth methods

EDIT: and about measuring only when there is no load will bring more problems than solve, becouse the battery is no a pure resistive load, it take a long time to the battery voltage stabilze, see the first part of the video

https://www.youtube.com/watch?v=p54wVWxFZ6Q


Would be a lot of trouble adding one of these?

http://www.ti.com/product/bq34z100-g1/description

More work on the hardware side, but less in making a SOC algorithm


[quote="Pantologist, post:176, topic:8952, full:true"]
It would make battery SOC more accurate. I think the method is called columb counting or something like that. 

Inboard even experiences early battery cutoff because the voltage sag is so high with their battery. Their battery readings are also of because they are simple meters based in voltage readings.

Having your board cut off from hard acceleration is not fun. This would change that.
[/quote]

That's it, the problem i see with pure coulomb counting is drift over time and not knowing whats the full capacity of the battery, the series of the video i posted above shows the main advantages of each method
```

---
## \#179 Posted by: raphaelchang Posted at: 2016-12-05T20:36:38.660Z Reads: 282

```
That's a very fancy algorithm. All the hardware should be there to implement it in software (if I can understand it).

I still think a low voltage cutoff for a cell should be there as a matter of absolute protection. It can be set lower than the 0% voltage, just to protect the cells. SOC tracking is more for user information (as in, a 0% SOC should not shut off the battery, only tell the user that the battery is empty, maybe with a warning).
```

---
## \#180 Posted by: Pedrodemio Posted at: 2016-12-05T22:37:00.057Z Reads: 279

```
Maybe that will work as a safe guard, at least on the beta units
I wil look on your code this weekend and start to think on how to implement something similar to the TI algorithm
```

---
## \#181 Posted by: PXSS Posted at: 2016-12-07T11:47:25.202Z Reads: 285

```
the way we measure SOC on our batteries at work is by measuring power draw every x seconds and integrating over time in order to get an accurate measure of energy used. Depending on the cell, the user could set up maximum capacity through software. For example a 10S4P NCR18650GA pack has a total of 504Wh, so the SOC percentage would be the 504Wh- integral of power over time.

This can be dangerous though. Batteries are not meant to go under a certain voltage level or permanent damage will happen. At higher current draws, the nominal energy of the cell is lower and pulling the rated amount can over discharge and kill your cells. We remedy this by having discharge curve models of cells at different current and temperature levels which we translate to maximum energy tables to reference when and use as our max capacity.

The simple way to do it is add a 10% margin to the rated energy and go by either that or low voltage cutoff. 

Cheers
```

---
## \#182 Posted by: aldopopp Posted at: 2016-12-07T13:33:23.316Z Reads: 273

```
(off topic) what job do you have?
```

---
## \#183 Posted by: PXSS Posted at: 2016-12-07T14:37:18.674Z Reads: 273

```
Aerospace Engineer at a small UAV company called Area-I but since we're so small (15 engineers) we are pretty well versed in several other areas. 

PM for more info. Dont want to drag the thread too far off topic.
```

---
## \#184 Posted by: WrinklyWink Posted at: 2016-12-21T06:32:02.406Z Reads: 271

```
So a couple questions from this:
[quote="raphaelchang, post:100, topic:8952"]
However, if you still want to use your power supply to directly charge your battery, there is the option of bypassing the charge circuit and directly connecting a charger (up to 40V for now) to the battery.
[/quote]

Would this mean that even though the BMS can do 12s (with its built in converter) it can only do up to 9s with CV?

[quote="raphaelchang, post:100, topic:8952"]
(up to 40V for now)
[/quote]

will there be a chance of using up to a 12s supply? A LOT of people have 10s chargers, they wouldn't work with this BMS, correct?

lastly, if using CV direct, will the circuit still balance the battery?
```

---
## \#185 Posted by: raphaelchang Posted at: 2016-12-21T19:34:03.664Z Reads: 262

```
[quote="WrinklyWink, post:184, topic:8952"]
Would this mean that even though the BMS can do 12s (with its built in converter) it can only do up to 9s with CV?
[/quote]

The built in converter is what allows it to do CV at any battery voltage. The limit I was referring to was the voltage limit of the charger input, which is now 50V, so there is no problem.

[quote="WrinklyWink, post:184, topic:8952"]
will there be a chance of using up to a 12s supply? A LOT of people have 10s chargers, they wouldn't work with this BMS, correct?
[/quote]

Yes, I have changed the design to allow for 50V power supplies.[quote="WrinklyWink, post:184, topic:8952"]
lastly, if using CV direct, will the circuit still balance the battery?
[/quote]

The BMS will balance the cells regardless of the charging method. It tries to balance them before the CV stage begins.
```

---
## \#186 Posted by: DeathCookies Posted at: 2016-12-21T20:09:51.687Z Reads: 253

```
[quote="raphaelchang, post:185, topic:8952"]
The BMS will balance the cells regardless of the charging method.
[/quote]

Is a software feature possible to set up the "cell balancing interval"?

e.g. i wanna say that the bms should only balance cells if the drift between them is higher than 0,5V or 0,05V

That feature would be awesome :heart_eyes:
```

---
## \#187 Posted by: Maxid Posted at: 2016-12-21T23:27:52.541Z Reads: 246

```
Why would that be awesoms? What do you need that for?
```

---
## \#188 Posted by: raphaelchang Posted at: 2016-12-21T23:51:11.491Z Reads: 260

```
Yes, that value is software configurable. It's not really useful to change it dynamically, but different people may have different requirements for their batteries.
```

---
## \#189 Posted by: Garfield Posted at: 2016-12-22T12:16:56.200Z Reads: 277

```
@raphaelchang
Great work I´m searching for an BMS for my project. I´m undecided if your BMS or the DieBieMs from JTAG is the right one for me.

I´m working on an self balancing scooter and plan to use either one 10s2p 5000mAh or two 10s1p 5000mAh battery packs (power both ESCs with one battery pack or power the left and right hub motor/wheel independent). The scooter uses brushless hub motors with 36V 60A max rating and I drive the motors with an VESC each.
My dream is to have an BMS which could send the following data back to my MCU over SPI/UART/CAN:
- state of charge
- individual cell voltage
- actual discharge current
- actual charge current
- temperature of the hot spots on the PCB
- temperature of the battery

Could you please give an short feedback of what should be possible with the beta testing BMS?
I know your BMS could do some of the feautures (I think except the temperatures).

I have a few more questions to you.
Is it possible to use your BMS with only a 10s LiPo pack?
Is it possible to use WS2812 to indicate charge status and an digital interface to an MCU (SPI, UART, CAN) at the same time?
Your BMS could charge and balance your 12S pack does the software automatically recognize a 10s pack and could this be charged also?

Thank you very much.
Best regards,
Garfield
```

---
## \#190 Posted by: raphaelchang Posted at: 2016-12-22T14:14:15.890Z Reads: 263

```
All of your listed features are possible on the current hardware (including both temperatures). Some features aren't implemented in software yet, but it should be easy to update the firmware on the beta testing version.

It is possible to use it with any cell configuration (4S-12S), including charging and balancing. Everything is configurable through a dashboard (like the VESC).  If you want to connect it to WS2812s, you will have to use CAN to communicate with your MCU. The I2C/UART/WS2812 pins are designed to be used for display peripherals (LCD, LEDs, etc.) so they are mutually exclusive. The CAN bus is designed for inter-PCB communication.
```

---
## \#191 Posted by: PXSS Posted at: 2016-12-22T15:23:27.514Z Reads: 255

```
Sign me up for Beta testing on both BMS and ESC. I also have all the tools to do my own assembly if it helps.
```

---
## \#192 Posted by: Michael319 Posted at: 2016-12-22T16:58:20.597Z Reads: 261

```
I would love to do some beta testing on the ESC
```

---
## \#193 Posted by: raphaelchang Posted at: 2016-12-22T17:35:44.850Z Reads: 266

```
The ESC isn't quite ready for beta testing yet, but I'll let you know!
```

---
## \#194 Posted by: DeathCookies Posted at: 2016-12-22T20:27:08.535Z Reads: 279

```
[quote="Maxid, post:187, topic:8952, full:true"]
Why would that be awesoms? What do you need that for?
[/quote]

Normally your new 18650 cells wont drift very much! Especially if you have them in parallel. @whitepony is riding without bms and he does not have battery voltage cell drift at all....


The problem is that a normal BMS would balance the cells every charge cycle. And i mean every cycle... You just have 1500 charge cycles and waste some on unnecessary  balancing. I want to avoid that and extend the life time of my batteries. 
So I want to set up that the BMS should only balance the cells if it is really required (more than 0,5 or 0,05).
```

---
## \#195 Posted by: Maxid Posted at: 2016-12-22T21:10:12.307Z Reads: 286

```
Sorry but AFAIK:
https://i.imgflip.com/ur7ip.jpg
```

---
## \#196 Posted by: Garfield Posted at: 2016-12-22T21:26:51.457Z Reads: 284

```
Is it possible to use two LiPos each with one BMS connected in parallel?
I mean one 10s1p LiPo with BMS and an second LiPo 10s1p with BMS and those two packs then paralleled.
I didn't see any reason against it. So if I'm not mistaken count me in for two beta test BMS.

@DeathCookies The balancing is working in the way that the energy which initially should charge the full (highest voltage) cell is dissipated in heat in the balancer. So the full cell doesn't see any charge/discharge while the balancing is on.
The cells which have a little lower voltage are charged until these are also full (and then balanced) and if all cells are full the charging is stopped.
So the balancing only ensures that every cell is individually charged to the max cell voltage and the balancing doesn't add any charge/discharge cycle to your cells. So if you prefer to charge unbalanced you gain no charge/discharge cycle. So it doesn't matter if the balancer is starting at 0.5V or 0.005V or even 0.0V difference of the cells.
I hope you could understand my explanation.
```

---
## \#197 Posted by: Hummie Posted at: 2016-12-22T21:56:23.403Z Reads: 277

```
why do you see balancing as wasting energy?  if the cells are balanced every time when charging you will have more energy as each cell will be filled to whatever voltage you decide.  for longest cell life a bms makes sense also.  for convenience and simplicity going without works but you will likely have to add a bit of buffer into the max charge voltage to be safe.  Or don't and have cells not being charged to the optimum voltage for greatest energy holding and longest life.
```

---
## \#198 Posted by: DeathCookies Posted at: 2016-12-22T23:15:33.876Z Reads: 279

```
@Garfield @Hummie thanks for the clarification.
```

---
## \#199 Posted by: DeathCookies Posted at: 2017-01-13T11:58:57.883Z Reads: 272

```
Well, The description on @raphaelchang website says 
" This video shows the BMS balancing cells while charging. When one cell reaches a voltage close to the fully charged voltage, it discharges all the higher cells that are a threshold above the lowest cell and continues charging."

That means that the higher voltage  cells get discharged to get balanced to the other cells. @Garfield you have said that the Full cell does Not get energy, it gets dissipated by heat... 

This does Not Match raphaels description. Could you tell me what this BMS actually do?
```

---
## \#200 Posted by: IDVert3X Posted at: 2017-01-13T13:01:14.160Z Reads: 272

```
[quote="DeathCookies, post:199, topic:8952"]
That means that the higher voltage  cells get discharged to get balanced to the other cells
[/quote]

That's how all BMS with balancing function works :)

[quote="DeathCookies, post:199, topic:8952"]
Full cell does Not get energy, it gets dissipated by heat
[/quote]

If this was a truth, we would not need a over-charge protection.
It will charge even further until it fails ( catastrophically ).
```

---
## \#201 Posted by: Garfield Posted at: 2017-01-13T15:30:55.205Z Reads: 263

```
Okay it was a bit unclear.
With "it gets dissipated by heat" I mean an resistor (in the BMS) parallel to the cell is switched on and discharges the full cell (which generates heat) OR these discharge resistor is a sink for the charge current and the charge current is heating up these resistor.

@DeathCookies 
If these resistor and MOSFET/TRANSISTOR is powerful enough the charger doesn't have to stop charging while balancing and if the resistor isn't powerful enough the charger hast to stop/slow down charging until balancing is finished. I didn't know whether of this is used in raphael's BMS but from the description in the video I assume that charging is stopped while balancing.

It is not meant that the full cell heats up itself which would be catastrophically here you are right.
Sorry for the not fully clear description.

I hope it is clear now if not please feel free to ask.
```

---
## \#202 Posted by: DeathCookies Posted at: 2017-01-13T17:37:52.586Z Reads: 261

```
[quote="Garfield, post:201, topic:8952"]
With "it gets dissipated by heat" I mean an resistor (in the BMS) parallel to the cell is switched on and discharges the full cell
[/quote]

That means that i will reduce the life cycle of a 18650? because the cell gets discharged a little bit when it is full just to get charged again until all batteries are at the desired end voltage.

Then this is the reason why i wanted to set up the balancing interval in the first place.
```

---
## \#203 Posted by: IDVert3X Posted at: 2017-01-13T17:48:43.760Z Reads: 253

```
No. Its generally better to keep them balanced :)
```

---
## \#204 Posted by: Okami Posted at: 2017-01-13T17:56:28.615Z Reads: 258

```
@DeathCookies im not a scientist.. but do you think that this discharge harms the cell (while balancing)?

 I think we should be more worried about the regen function, which seems to be putting energy back into the cells.. as soon as they had released it to the motors/esc and other electronics :)
```

---
## \#205 Posted by: DeathCookies Posted at: 2017-01-13T17:56:52.723Z Reads: 264

```
I think you are right but the cells dont drift much at all. At least @whitepony seems not to need a BMS but the cells are balanced quite well since a long period! If you have a efficient setup and a good battery which can handle the required constant output (and when it has many cells in parallel) they dont tend to drift very quickly. So why should i balance them every time if they do not really need to be balanced. 

e.g.
cell 1: 4,05V
Cell 2: 4,00V

but it should balance if the voltage difference is more than 0,2V:
Cell 1: 3,9V
Cell 2: 4,1V


  

@raphaelchang i will beta test this BMS if you enable a software feature where i can set up a voltage difference for the balancing interval
```

---
## \#206 Posted by: SORRENTINO Posted at: 2017-01-13T18:14:55.905Z Reads: 252

```
1. Your over thinking this. 2. All it takes is one battery cell to go bad regardless of health and you'll be sorry. 3. Is this all because you want to charge faster?
```

---
## \#207 Posted by: DeathCookies Posted at: 2017-01-13T18:16:32.354Z Reads: 247

```
It is about longlivity. This is over thinking but why not. It would be a nice feature to have....
```

---
## \#208 Posted by: SORRENTINO Posted at: 2017-01-13T18:16:42.732Z Reads: 247

```
Also a cell might not be off that much but have you thought about the Ir changing in the cells? this could cause some cells to charge faster then others even if they are the same voltage.
```

---
## \#209 Posted by: SORRENTINO Posted at: 2017-01-13T18:18:29.268Z Reads: 246

```
I think its very unlikely that balance charging the cells has any negative effect on the longevity of them. We would have probably seen testing by now that supported your thought if it was true. imo atleast
```

---
## \#210 Posted by: DeathCookies Posted at: 2017-01-13T18:29:04.501Z Reads: 252

```
if the resistance is changing it will indeed charge faster/slower. Then the bms would always balance charge because the voltage difference is always to high.

[quote="SORRENTINO, post:209, topic:8952"]
I think its very unlikely that balance charging the cells has any negative effect on the longevity of them. We would have probably seen testing by now that supported your thought if it was true.
[/quote]

One cell has approximately 1000 charge cycles. If you balance charge you are going to charge/decharge/charge the cell multiple times in one charge cycle. Then you will have about 1,01 charge cycle for each cell by charging the complete pack. Therefore you will only get about (1000/1,01=) 990 cycles

Again: This is overthinked but why not?
```

---
## \#211 Posted by: IDVert3X Posted at: 2017-01-13T19:11:55.473Z Reads: 244

```
Look,  I dont use BMS for liions either, but if you have balancing function, its pointless to not use it. It will improve the lifespan, not the oposite way. Im not going to explain why, use google if you are interested. There are some studies on that topic.
```

---
## \#212 Posted by: Okami Posted at: 2017-01-13T20:05:45.545Z Reads: 268

```
@DeathCookies Well unless you gonna "race" your batteries, I think these 10 cycles out of the battery life wont matter!

 You will still witness capacity fade anyways.. I think for such ''consumers / commuters'' as us.. it does not make such a big impact if we lose a bit of percentage in the long run (like 3+ years).. as by that time the batteries should have outweighted the cost of using other alternative transports, some of which migh use oil anyways..

I think you are a bit overdoing it / on an extreme with this.. I do understand your interest in longterm reliability but I think as soon as you dont intend to buy a car battery, which might really need to last at least 10 years.. then this is not so much a concern.. especially if you can try to replace the batteries at later stage anyways and it is not a maintaince intensive job :)

---

[quote="DeathCookies, post:210, topic:8952"]
One cell has approximately 1000 charge cycles. If you balance charge you are going to charge/decharge/charge the cell multiple times in one charge cycle. Then you will have about 1,01 charge cycle for each cell by charging the complete pack. Therefore you will only get about (1000/1,01=) 990 cycles

Again: This is overthinked but why not?
[/quote]

I think if you dont like balancing cells all the time, your best option is just to get balance function turned off (if it can be turned off, other just get a different bms)..

This way.. you will be able to ''bulk charge'' as you wish.. and just balance the cells from time to time.. if they do need balancing at all.. (@whitepony experience)
```

---
## \#213 Posted by: raphaelchang Posted at: 2017-01-14T01:22:35.345Z Reads: 252

```
The balance threshold feature is really easy to implement, so I have already implemented it, regardless of whether you really need it. Some threshold is always needed anyways, otherwise the balance routine will never end because the voltages can never be perfectly equal.
```

---
## \#214 Posted by: PXSS Posted at: 2017-01-14T08:56:50.040Z Reads: 270

```
@DeathCookies post 202. is right on this one. The cells do not lose longevity by being discharged near full capacity. The cells lose longevity by being charged near full capacity also the longer the cells remain near full capacity, the lower their lifespan. This is due to the chemistry of the cells. The chemical reaction while charging produces more oxides at high voltage state which reduce the amouny of charge a cell can hold. Over several cycles this adds up into reduced capacity, this is actually the reason why the more cycles your cells have, the lower the capacity. Even though the chemical reaction is mostly reversible, it is not 100% reversible. 

So the longer your cells remain near 4.2V charging, the more you are harming them. That's why spec sheets state that you need to have a timer to stop balancing after 2 hours in cv mode regardless of how closely your cells are balanced or how close to 4.2V your pack is. 

@IDVert3X, post 203. the reason it is a good udea to keep them balanced is so you can get the most capacity out of the pack. Nothing to do with health. If your BMS detects any cell at 2.5V it will shut down regardless of other cells being at 2.8V. By keeping them balanced, you assure that the voltage difference between them remains as low as possible and you are not wasting any energy. 

On non-BMS setups, only the total voltage of the pck is read, so in this case it is important to keep them balanced as when your ESC sees 10V on a 4s pack, it means that each cell is at 2.5V or nearly there. If unbalanced, you could have drained a cell beyond 2.5V and reduced its longevity. Again soec sheets usually state what is the minimum voltage on the cell where you should not try to recharge the cell (usually under 2V for 18650 cells)

@Okami, post 204, balancing if not done right is harmful. Read above.  

@SORRENTINO, post 206,208-209, you are exaggerating. He is talking about a 0.05V difference. If he has a dead cell and properly adjusted his voltage cutoffs, this system is completely safe, his cells will charge faster and his cells will last longer. 

 If a cell has higher Ir and does charge faster, they will be out of balance by a proportional amount. If they are not that far off, then the Ir is not that far different. V=I*R. Simple as that. A cell that is going bad will get balanced whenever it needs to be balanced. Again as long as your low voltage cutoff is reasonable, no risk and dare I say his bad cell will last longer than if it were being balanced every cycle as it would spend less time near full capacity. 

@DeathCookies, post 210, the cells are usually rated for ~300 cycles above 70-80% original capacity not 1000. Look up the spec sheet of the particular cell you use.  


@IDVert3X, post 211, you'll have to explain why, because that is wrong unless you are using the cells to their full range of 4.2V-2.5V without a BMS. 

@Okami. Post 212. Why is it overdoing it when it's such a simple change that will make his batteries healthier?
```

---
## \#215 Posted by: IDVert3X Posted at: 2017-01-14T10:25:17.678Z Reads: 259

```
Ok, I will explain. I do not need BMS in most cases, low and high voltage cutoffs are enough and these can be easily programmed into the microcontroller which I almost always have in my project on the main logic board, its just matter of adding a mosfet and one more trace + voltage divider. This works fine for me as my liions cells almost dont drift at all, I use the range of 2.8-4.1V per cell. For lipos, I use proper BMS with per cell monitoring, balancing etc.
```

---
## \#216 Posted by: benwong Posted at: 2017-01-14T10:38:16.348Z Reads: 264

```
sorry guy, abit out of topic, is there any sequence to hook up bms wiring to lipo battery?
Balance lead connect first or main power wire connect first?
```

---
## \#217 Posted by: PXSS Posted at: 2017-01-14T10:46:06.650Z Reads: 262

```
So why do you think balancing every cycle will improve lifespan? If your cells are limited between 2.8 and 4.1v?
```

---
## \#218 Posted by: WrinklyWink Posted at: 2017-01-14T12:52:32.558Z Reads: 282

```
[quote="DeathCookies, post:210, topic:8952"]
One cell has approximately 1000 charge cycles. If you balance charge you are going to charge/decharge/charge the cell multiple times in one charge cycle. Then you will have about 1,01 charge cycle for each cell by charging the complete pack. Therefore you will only get about (1000/1,01=) 990 cycles

Again: This is overthinked but why not?
[/quote]

Actually that isn't overthinking in the future sense. If we are to overcome lion's limitations we have to be thinking exactly like this and more. At the threshold of where degrading occurs with possibility dynamic means of charging, as one possible idea. The largest most successful discoveries of mankind has been during the close examination of two repelling problems. In fact this goes for all successful discoveries. The fact that you're asking yourself these questions means you are still considering variables that other people have overlooked or passed as unimportant. Again through the history of discovery the reward for this behavior goes with possibly finding a never explored solution. Like diamonds in the rough.
People might find you unrelevant or off topic, but you have a gem for discovery because of this thinking. kudos for being persistent.
```

---
## \#219 Posted by: Okami Posted at: 2017-01-22T20:59:05.878Z Reads: 268

```
I think we also should start by pointing out to beginners that if they want to keep their cells alive for longer.. they should not charge the board till 4.2v.. and then keep it for a half a year charged that way either..
```

---
## \#220 Posted by: Pimousse Posted at: 2017-02-06T19:15:16.661Z Reads: 271

```
Hi Raphael,

How is going the prototypes production ?

As you mentioned that a couple of pin are available, I have some ideas coming.
Is at least one of them which is PWM ?
Do we have few computational resources left ?
I bought a couple of Neopixel rings (using WS2812) and play a bit with :

https://youtu.be/MnKQRo1I4bA
(gradient color from green to red and numbers of leds according to the capacity left, switch in blue when charging).
I have some ideas left to improve the deisgn and add feature.
The code isn't so heavy (10-20% for program and RAM).
```

---
## \#221 Posted by: Okami Posted at: 2017-02-06T19:18:45.645Z Reads: 266

```
@Pimousse This is pretty cool! Will you share your results when it is gonna be more finished? Is there a place where to check up on your work or all the stuff is gonna be inserted here?

I also got 8piece RGB led ring (ws2812) ordered.. so it was awesome to look at what you have achieved with yours! 

It looks like you got 12rgb leds on yours.. but that does not spoil the ''fun'' that I'll get only 8, I think..

Non the less, the color effects look awesome! Cant wait to get my hands on one of these and start ''experimenting'' too :slight_smile:

---

Can you somewhat describe what your ''algorithm'' for capacity will be?

Will you rely on one cell's voltage or you maybe even have some sort of current sensor / shunt for your board?

..

My version will probably consist of 1cell reading for better accuracy.. 8 leds (in my case), could symbolize the 8 ''mayor steps'' in voltage.. EG - Full on - 4.1-4.2v, Empty - 3.4-3.5v
Then.. the colors might as well ''help out'' by indicating ''Low - Med - High'' Range.. Green / blue for ''High'', Yellow for ''Mid'' and Red for ''low''
```

---
## \#222 Posted by: Pimousse Posted at: 2017-02-06T19:29:27.254Z Reads: 273

```
My inputs are pretty simple :
1x uint8_t for capacity (0-100)
1x bool for charging state (TRUE=charging)

And... that's all !

I have to clean my code because some part are hard-coded to be used with 12 leds.
But once it's clean, you'll just have to define the number of led at the beginning.

I only use 0-100% for the capacity because I guess you already compute calculations for BMS protection.
It avoids to specify twice the same values (100% and 0% voltage).
```

---
## \#223 Posted by: Pantologist Posted at: 2017-02-06T20:33:50.314Z Reads: 263

```
Nice! This is like what Mellow is using. Seems that it takes up lots of space though. Are there smaller neo pixel rings?
```

---
## \#224 Posted by: raphaelchang Posted at: 2017-02-06T20:56:46.440Z Reads: 258

```
There is a pin that can be used to drive WS2812 LEDs. I've been trying to get the code to work on the STM32F3, but still having a bit of trouble. 

There is a current sensor to do state-of-charge calculations for capacity. I haven't implemented the algorithm yet, but it will probably be a combination of coulomb counting and voltage tracking.
```

---
## \#225 Posted by: Pimousse Posted at: 2017-02-06T21:18:27.250Z Reads: 265

```
6066 bytes for program
219 for RAM

I bought this one :
https://www.adafruit.com/products/1643

From Adafruit, it's the smallest one.
But there are surely plenty of other brands and maybe you can find a smaller one.
```

---
## \#226 Posted by: Okami Posted at: 2017-02-06T21:18:39.331Z Reads: 266

```
Oh cool, didnt know your bms has capacity meter / current sensor.. this opens a wide range of possibilities / opportunities, I think!

Though - is it capable enough to measure discharge current also?
```

---
## \#227 Posted by: Pantologist Posted at: 2017-02-06T21:25:04.411Z Reads: 275

```
I have these individual ones to make a nice bar style config. I also have 60 leds per meter strips of neo pixels, that might be better. 

I found this, Might be cool to have battery capacity status for the outer leds and the inside led for error codes.

https://www.adafruit.com/products/2226
```

---
## \#228 Posted by: Pedrodemio Posted at: 2017-02-07T18:08:04.822Z Reads: 267

```
[quote="raphaelchang, post:134, topic:8952"]
as most boost converters do) of 6A. By conservation of power, the product of input voltage and input current must equal the product of output voltage
[/quote]

@raphaelchang I've been searching for a power supply  to use for when the BMS arrive, it's a rule that the input voltage must always be lower than the battery or the converter can act as a step down? on Ali Express there are some nice power supply's at 32V 6A that would bring the charge time down a lot
the other option that I've found are 28V bricks that leave a safety margin
```

---
## \#229 Posted by: raphaelchang Posted at: 2017-02-07T20:01:36.817Z Reads: 263

```
It doesn't step down, but you can still use a higher voltage power supply. It will just act as if you plugged it into the battery directly (the supply's current limit will be activated).
```

---
## \#230 Posted by: Pantologist Posted at: 2017-02-07T20:06:03.096Z Reads: 258

```
Just to confirm. If using a Boosted charger with 12S A123 cells will the BMS allow the 43.2V 2.9A current from the charger?
```

---
## \#231 Posted by: Pedrodemio Posted at: 2017-02-07T20:13:12.798Z Reads: 265

```
Thanks, i will go to lower voltage since i don't put much faith on the current limiter of these cheap power supply

@raphaelchang i was reading your site again, on this final version the max charging current is still 3A or it went back to 6A?
```

---
## \#232 Posted by: raphaelchang Posted at: 2017-02-07T21:39:14.295Z Reads: 269

```
If you're not using the boost converter, there isn't really an absolute current limit for charging.

@Pantologist You can use the Boosted charger with the BMS.
```

---
## \#233 Posted by: Pedrodemio Posted at: 2017-02-07T22:00:50.771Z Reads: 264

```
I mean when using the boost converter
```

---
## \#234 Posted by: raphaelchang Posted at: 2017-02-07T22:34:56.305Z Reads: 269

```
It depends on your input voltage level, the higher ratio you're boosting up to, the lower the current. It should be roughly 6A divided by the ratio.
```

---
## \#235 Posted by: Pedrodemio Posted at: 2017-02-08T14:17:51.008Z Reads: 279

```
Got it, so it was just like before, the input current limited at 6A and the output by conservation of power

With respect of how the charging part work, i can plug in a 19v power supply and it will use the boost converter to charge, and i can plug a proper cc/cv charger. Does the transition between the two modes happen automatically or i have to set the desired mode on the configuration app?
```

---
## \#236 Posted by: hexakopter Posted at: 2017-02-23T22:09:51.926Z Reads: 268

```
Is the order placed now @raphaelchang?
```

---
## \#237 Posted by: raphaelchang Posted at: 2017-02-24T02:59:12.736Z Reads: 273

```
It has been placed, just waiting for a confirmation on the design before manufacturing begins.
```

---
## \#238 Posted by: hexakopter Posted at: 2017-03-10T16:49:31.052Z Reads: 277

```
What is the status right now? I think we are now in the time frame of the delivery from the beginnings time schedule. Thanks.
```

---
## \#239 Posted by: fraannk Posted at: 2017-03-10T18:22:24.518Z Reads: 280

```
I am soooo excited for this :D
```

---
## \#240 Posted by: Titoxd10001 Posted at: 2017-03-10T19:18:57.476Z Reads: 285

```
What will we need to get started using your bms? (wires, connectors, switches, charge port)

Also does your bms support 11s?
```

---
## \#241 Posted by: raphaelchang Posted at: 2017-03-10T23:30:09.821Z Reads: 284

```
Apologies for the lack of updates. Production got a bit delayed because of a design issue I found + DFM issues at the manufacturer, so they've just started making the boards. They're estimating 4 weeks from now for completion.

You'll need wires from your battery to the BMS, from the BMS to the ESCs, a charger connector, wires from the charger connector to the BMS, a JST-XH balance connector from the battery (with # cells + 1 wires), and a momentary switch. It supports batteries from 4S to 12S.
```

---
## \#242 Posted by: Pedrodemio Posted at: 2017-03-11T04:33:33.586Z Reads: 276

```
Raphael, another doubt,

Your design use just on directFET to switch the power, is that enough? How many amps this just one FET can handle?

I saw some anti spark switches that use 3 direct FET's in parallel 

Thanks
```

---
## \#243 Posted by: raphaelchang Posted at: 2017-03-11T05:24:16.510Z Reads: 275

```
Should be 80-100A, but it will get hot. Keep in mind that this is battery current though, so it will usually be less than the motor current. If it becomes too problematic for many people I can add a second one (at the expense of size + cost).
```

---
## \#244 Posted by: Pimousse Posted at: 2017-03-11T06:18:56.254Z Reads: 273

```
What is the failsafe position of the DirectFET ?
I had troubles with Vedder's antispark, MOSFET failed in ON position.
```

---
## \#245 Posted by: raphaelchang Posted at: 2017-03-14T15:41:56.227Z Reads: 274

```
It's the same as any MOSFET, the failure position isn't really predictable. I haven't been able to kill a DirectFET though.
```

---
## \#246 Posted by: DougM Posted at: 2017-03-14T23:52:41.563Z Reads: 283

```
That's encouraging.  Did you try and kill a bunch of other FETs before you landed on the DirectFET or did you happen upon it by luck?
```

---
## \#247 Posted by: fraannk Posted at: 2017-03-15T09:30:05.939Z Reads: 285

```
I'm not entirely sure which kind of charger I'll need for this BMS. I have a 8S setup, would I need a 33,6V charger, or would the BMS be able to charge the batteries with, let's say a 25V charger?
```

---
## \#249 Posted by: Pantologist Posted at: 2017-03-15T20:35:02.593Z Reads: 291

```

You could use a lower voltage power supply and the Boost converter will boost the voltage to the required voltage for charging.

<img src="/uploads/db1493/original/3X/0/3/0316fc5f84cfa1401b80d4f031460ff1a375cf34.png" width="646" height="500">
```

---
## \#250 Posted by: raphaelchang Posted at: 2017-03-15T20:49:17.967Z Reads: 281

```
I'm no longer using that IC. I'm using [this one](http://cds.linear.com/docs/en/datasheet/3873fb.pdf) now. You can use a lower voltage charger, which will use this circuit, or you can use an 8S charger, and this circuit will be bypassed.
```

---
## \#251 Posted by: Titoxd10001 Posted at: 2017-03-23T23:57:19.425Z Reads: 284

```
What are the 2 pin and 5 pin connectors for and are they included. 

Also I can use a 10s charger to charge a 11s or 12s pack? I'm able to change end voltage to say 4.1 per cell or how does that work?
```

---
## \#252 Posted by: raphaelchang Posted at: 2017-03-25T23:47:33.486Z Reads: 287

```
The 5 pin connector is for connecting accessories. It has two pins that can be used for I2C/UART, and 5V and 3.3V supplies. One of the 2 pin connectors is for connecting the required momentary switch, and one of them is for CAN.

You should be able to use a 10S charger for a higher voltage pack and be able to configure the end voltage.
```

---
## \#253 Posted by: fraannk Posted at: 2017-03-28T08:05:33.677Z Reads: 284

```
Would it also be possible to use a 10S charger for lets say 8S batteries?
```

---
## \#254 Posted by: TSG_AU Posted at: 2017-03-28T17:33:34.297Z Reads: 282

```
Hey @raphaelchang, what IDE do you use for firmware development?
```

---
## \#255 Posted by: trampalovesshekels Posted at: 2017-03-28T18:27:24.245Z Reads: 279

```
emacs but its not for kids :underage:
```

---
## \#256 Posted by: chinzw Posted at: 2017-03-31T06:25:11.280Z Reads: 272

```
Any news from the manufacturer?
```

---
## \#257 Posted by: raphaelchang Posted at: 2017-04-02T02:53:09.294Z Reads: 284

```
@fraannk Yes, it'll just behave like a normal power supply connected straight to a battery, with CC charging only.

@TSG_AU I use vim.

@chinzw They're still manufacturing and assembling the boards; they finished asking me about DFM problems last week and are currently obtaining parts for assembly.
```

---
## \#258 Posted by: flatsp0t Posted at: 2017-04-02T13:43:33.723Z Reads: 282

```
Now that it is being Manufactured, can you tell me the final measurements so i can plan my enclosure?
```

---
## \#259 Posted by: okashira Posted at: 2017-04-03T08:08:59.718Z Reads: 284

```
Very interesting you use a free IDE --- and a crazy expensive suite (altium designer) for the PCB. I guess you get to use it through your university. :)
```

---
## \#260 Posted by: Pedrodemio Posted at: 2017-04-03T11:57:27.912Z Reads: 285

```
@raphaelchang another doubt, does the circuit have a soft latch or I have to use a latching switch?
```

---
## \#261 Posted by: chinzw Posted at: 2017-04-03T15:31:34.108Z Reads: 285

```
@Pedrodemio it uses a momentary switch for the on/off
```

---
## \#262 Posted by: Pedrodemio Posted at: 2017-04-03T15:48:07.436Z Reads: 281

```
Thanks, that's better since they are less bulky
```

---
## \#263 Posted by: raphaelchang Posted at: 2017-04-05T23:00:16.978Z Reads: 278

```
There's a STEP file on the Github, which contains the hole locations and board size.
```

---
## \#264 Posted by: Pimousse Posted at: 2017-04-16T20:02:01.760Z Reads: 288

```
Hi Raphael,

Any news since the last 2 weeks ?
I think it's REALLY important that you update us often.
It helps us to feeling that the project is still alive and we didn't waste a consequent amount of money.
;)
I still can't finish a build (started in June 2016), your BMS is the last part missing.
And warm and sunny days are arriving :slight_smile:

Thank you !
```

---
## \#265 Posted by: raphaelchang Posted at: 2017-04-17T20:41:55.666Z Reads: 292

```
Apologies for the lack of updates. I've just emailed the manufacturer asking for a status update, will post again when I get a reply.
```

---
## \#266 Posted by: chinzw Posted at: 2017-04-18T04:16:33.074Z Reads: 297

```
Thanks for the reply, keep us updated. Im in the same boat as pimouse, bms is all that's left
```

---
## \#267 Posted by: raphaelchang Posted at: 2017-04-21T08:11:09.192Z Reads: 296

```
Just got photos from the manufacturer of the assembled boards. Once I check everything and confirm with them, they'll ship the boards to me, which should take 1-2 weeks.
<img src="/uploads/db1493/original/3X/1/c/1c58c3896b6ba7f17782cb970cfb86398aa68797.jpg" width="680" height="500">
<img src="/uploads/db1493/original/3X/0/7/07955412c89d0bc70a8c906d82e5d9206ace06df.jpg" width="690" height="472">
```

---
## \#268 Posted by: fraannk Posted at: 2017-04-21T08:24:33.996Z Reads: 289

```
Looks awesome!!
```

---
## \#269 Posted by: webst Posted at: 2017-04-21T08:42:24.031Z Reads: 292

```
Is it possible to buy one?
```

---
## \#270 Posted by: Pimousse Posted at: 2017-04-21T11:27:57.479Z Reads: 293

```
Good news !!
So only one DirectFET ?
Do you plan to release documentation as well (specs, features, communication protocol, software...) ?
I'd like to see how manage to communicate with the VESC and OLED screen (or WS2812 as I mentioned before)

Thank you, we're close to touch it !! Can't wait ! :smile:
```

---
## \#271 Posted by: chinzw Posted at: 2017-04-21T15:42:33.766Z Reads: 290

```
@raphaelchang they look awesome! Can't wait to start playing around with this!
Edit: will we be needing heatsink for the directFET? I can probably CNC mill a few if needed.
```

---
## \#272 Posted by: longhairedboy Posted at: 2017-04-21T16:09:43.656Z Reads: 287

```
so when can i get some?
```

---
## \#273 Posted by: Pantologist Posted at: 2017-04-21T16:41:55.106Z Reads: 287

```
I don't think he is taking more Beta orders. Hopefully after the beta run we can get more manufactured for cheaper.
```

---
## \#274 Posted by: webst Posted at: 2017-04-21T18:51:28.135Z Reads: 292

```
I can arrange EU production of resonable batch.
```

---
## \#275 Posted by: longhairedboy Posted at: 2017-04-21T19:19:23.856Z Reads: 286

```
somehow i missed the whole beta thing. Dammit.
```

---
## \#276 Posted by: Pantologist Posted at: 2017-04-21T19:32:27.428Z Reads: 290

```
I missed it because I was broke paying for college ☹️
```

---
## \#277 Posted by: smurf Posted at: 2017-04-21T21:35:28.341Z Reads: 289

```
I'm ok missing the beta version. But I'm in on the next batch
```

---
## \#278 Posted by: JTAG Posted at: 2017-04-21T21:48:07.480Z Reads: 288

```
47R 0805 balancing resistors :open_mouth:? those must be special ones :blush:. looks awesome!
```

---
## \#279 Posted by: thisrealhuman Posted at: 2017-04-22T08:31:11.270Z Reads: 287

```
This is going to change the world. Like a computer mouse,  or the plastic shoelace tabs. Thank you testers, on behalf of the future!
```

---
## \#281 Posted by: Rollbrett Posted at: 2017-04-27T05:52:00.792Z Reads: 286

```
BMS's are usually advertised separately for either Lipo or lion, but is there an actual difference in hardware or software?
I was wondering because I'm probably going to switch to LiIon sooner or later and it'd be nice to use this BMS for Li-Ion's as well.
Would that be possible? (maybe via a software update?)
```

---
## \#282 Posted by: chinzw Posted at: 2017-04-27T15:19:50.685Z Reads: 286

```
Its the same thing, you should be able to use this bms with any type of battery, since its programable and you can change the voltage ranges.
```

---
## \#283 Posted by: chinzw Posted at: 2017-05-03T15:48:28.016Z Reads: 281

```
@raphaelchang any news?
```

---
## \#284 Posted by: chsknight Posted at: 2017-05-03T16:30:16.960Z Reads: 285

```
I missed the beta?! Noooo....

God speed on this project.  I really need a smaller BMS.
```

---
## \#285 Posted by: longhairedboy Posted at: 2017-05-03T17:03:30.462Z Reads: 286

```
i need like 10s of them now.
```

---
## \#286 Posted by: SilentException Posted at: 2017-05-03T17:07:20.630Z Reads: 292

```
I would also be interested in beta testing of one, two. If you do get any extras...
```

---
## \#287 Posted by: oyta Posted at: 2017-05-03T19:13:35.796Z Reads: 293

```
Let me know if you ever start up. I may be interested!
```

---
## \#288 Posted by: yakjock Posted at: 2017-05-04T11:01:12.236Z Reads: 290

```
I would be interested too as I am piecing together my first build.
```

---
## \#289 Posted by: Pimousse Posted at: 2017-05-10T08:00:36.880Z Reads: 289

```
Any news now ?
```

---
## \#290 Posted by: petter Posted at: 2017-05-11T13:43:55.468Z Reads: 296

```
Also interested in this! Looks really good so far, loving the boost converter idea even if it's not the most energy efficient. Imagine that you battery bites the dust for some external reason, and you have a spare battery that's a different cellcount for example, you can still just switch it out and go on, the battery will still be protected and super easy to charge!
```

---
## \#291 Posted by: raphaelchang Posted at: 2017-05-12T08:40:26.240Z Reads: 294

```
Sorry for the delay everyone, I just received the boards this week, but I'm very busy this next week because of finals. I'll post a more detailed update in about a week.
```

---
## \#292 Posted by: eitan Posted at: 2017-05-12T08:56:34.589Z Reads: 298

```
Thanks for the update but more importantly good luck on finals - the BMS can wait.
```

---
## \#293 Posted by: longhairedboy Posted at: 2017-05-12T14:32:31.818Z Reads: 297

```
<img src="/uploads/db1493/original/3X/e/7/e796ca7cc719fac0468af6b031b7346c2fcb2faa.jpg" width="196" height="257">
```

---
## \#294 Posted by: chinzw Posted at: 2017-05-12T15:18:59.661Z Reads: 290

```
Good luck on your finals! We can wait another week :slight_smile:
```

---
## \#295 Posted by: WrinklyWink Posted at: 2017-05-16T05:40:56.856Z Reads: 288

```
should i be nervous that the negative and positive leads are so close to each other? what is the clearance between them?

I feel like i would need to apply hot glue insulation, because the tiniest bit of metallic dust or water droplet could short the two.

Then again, if this thing can do 100 Amps then surely the glue would remelt. :thinking:
```

---
## \#296 Posted by: smurf Posted at: 2017-05-16T07:06:35.076Z Reads: 292

```
https://www.amazon.com/MG-Chemicals-Silicone-Modified-Conformal/dp/B008O9YIV6/ref=sr_1_5?ie=UTF8&qid=1494918296&sr=8-5&keywords=mg+chemicals
```

---
## \#297 Posted by: Pantologist Posted at: 2017-05-17T12:20:09.322Z Reads: 288

```
I said the same thing. You just have to make sure they are soldered correctly and have insulation of some kind. Not sure about the dimensions of the pads but maybe you could surface solder a XT60 instead of wires.
```

---
## \#298 Posted by: chinzw Posted at: 2017-05-24T22:34:42.323Z Reads: 286

```
@raphaelchang hey dude, any news on the boards? We're all eager to give them a go.
```

---
## \#299 Posted by: raphaelchang Posted at: 2017-05-25T04:58:34.355Z Reads: 285

```
Sorry for the delay. I just ordered ESD bags and shipping boxes so I hope to ship them next week. 

Even though the hardware is good, there are still quite a few bugs and missing features in the firmware that need attention before the BMS is usable. I'm busy with an internship this summer and might not have enough time to develop the firmware, so I'd appreciate any contributions to the firmware once you have the boards. Pull requests for the issues on GitHub (https://github.com/raphaelchang/battman-firmware/issues) would be great.

Meanwhile, I'll try to develop the firmware a bit more after shipping the boards. Once they arrive, you'll be able to flash the latest firmware onto the boards (instructions later).
```

---
## \#300 Posted by: itsmikeholland Posted at: 2017-05-26T01:11:40.441Z Reads: 280

```
i need this! theres no more to beta test?
```

---
## \#301 Posted by: chinzw Posted at: 2017-05-26T03:47:47.350Z Reads: 280

```
I'll have some spare time this summer so ill try and go through your code to get acquainted, and ill help out as much as i can.
```

---
## \#302 Posted by: jackw Posted at: 2017-05-28T12:40:45.362Z Reads: 270

```
Will these be available to buy at any time? Would be perfect to finish a build I'm working on 😩
```

---
## \#303 Posted by: chinzw Posted at: 2017-06-06T16:44:46.458Z Reads: 261

```
@raphaelchang hey raphael, any news? did you manage to ship the bms?
```

---
## \#304 Posted by: raphaelchang Posted at: 2017-06-07T00:50:26.210Z Reads: 263

```
Still making shipping labels, 30 boards is a lot to ship :slight_smile:
```

---
## \#305 Posted by: hexakopter Posted at: 2017-06-09T12:01:59.972Z Reads: 261

```
Great to see that it is going forward. I think it would be useful that we receive the boards before the Paypal insurance is running out. So that we really receive something and not canceling shortly before the insurance is gone.
```

---
## \#306 Posted by: Pedrodemio Posted at: 2017-06-09T13:09:59.628Z Reads: 268

```
@raphaelchang one of the thinks I plan to use my board is to power things (notebook, phone, etc) thru the charging port, with an external DC-DC converter obviously, in the current firmware, does the charge port allow a reverse current? And can I do this with the BMS off?

Thanks
```

---
## \#307 Posted by: raphaelchang Posted at: 2017-06-09T16:31:27.485Z Reads: 266

```
@hexakopter yes, I believe that the insurance runs out after 180 days, which is in July. They will be shipped by then.

@Pedrodemio I don't really understand your question. The charge port doesn't allow current to flow from the battery to the charge port.
```

---
## \#308 Posted by: Pedrodemio Posted at: 2017-06-09T16:45:36.697Z Reads: 267

```
That's what I would like to know, is this a hardware or software limitation ?
```

---
## \#309 Posted by: chinzw Posted at: 2017-06-20T17:27:37.451Z Reads: 261

```
@raphaelchang hey dude, any updates? its been a while
```

---
## \#310 Posted by: raphaelchang Posted at: 2017-06-22T23:33:56.174Z Reads: 251

```
I'm starting to ship them out a few at a time, I'll let you know when yours is shipped. Hopefully everything will be out by the end of next week.
```

---
## \#311 Posted by: SilentException Posted at: 2017-06-22T23:42:12.961Z Reads: 253

```
Do you have any extras? I know, it's a stretch but contact me if you do :)
```

---
## \#312 Posted by: sprocket12 Posted at: 2017-06-23T22:34:13.279Z Reads: 248

```
Ditto!  I failed to see this thread and have 32- 26650's going into a pack now.  I'm interested in implementing immediately!  I'll buy an extra if available...

-
```

---
## \#313 Posted by: chinzw Posted at: 2017-06-23T22:52:34.099Z Reads: 243

```
@raphaelchang please keep us posted, all i'm missing for my new build is the bms.
```

---
## \#314 Posted by: raphaelchang Posted at: 2017-06-23T23:07:11.511Z Reads: 247

```
Keep in mind that the only reliably working feature in the BMS firmware is the power switch and charging, so I wouldn't rely on it having other features immediately if you need them for your build.
```

---
## \#315 Posted by: Pedrodemio Posted at: 2017-06-23T23:31:36.507Z Reads: 254

```
Does the charging includes balancing? If it's switching on and off and balancing/charging that's ok as a start, and the GUI is working for some basic configuration?

Could you list what needs to be done? In a week I will have a little bit of free time and could help implementing what's left
```

---
## \#316 Posted by: chinzw Posted at: 2017-06-25T21:19:09.525Z Reads: 253

```
@raphaelchang does it have the basic BMS functionalities? Charging and balancing ? If so that should be enough to get started.
```

---
## \#317 Posted by: Titoxd10001 Posted at: 2017-07-07T07:58:07.219Z Reads: 247

```
Where are the updates. No photos or any mention of anyone receiving a bms. Not cool
```

---
## \#318 Posted by: Titoxd10001 Posted at: 2017-07-07T08:09:49.956Z Reads: 242

```
180 days is coming up for me next week. Check your transaction date fellas
```

---
## \#319 Posted by: Pedrodemio Posted at: 2017-07-07T14:03:28.384Z Reads: 247

```
Mine has been shipped, but it will take a while to arrive
```

---
## \#320 Posted by: Pimousse Posted at: 2017-07-07T18:18:49.044Z Reads: 249

```
Mine is at the post office.
I'll grab it tomorrow morning ;)
```

---
## \#321 Posted by: Pimousse Posted at: 2017-07-08T07:26:31.803Z Reads: 257

```
Got it !
<img src="/uploads/db1493/original/3X/4/6/46a282ce0bef20c913529b3d277871acf6534c73.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/3/e/3e9452031e06bb0663d0e66e6721544f7f868874.jpg" width="666" height="500">
But I had to pay 39€ for VAT and customs fees !! :frowning:
That starts to be a lot of money for a BMS !

@raphaelchang : what's the type of connectors ? Need to order them.
```

---
## \#322 Posted by: Okami Posted at: 2017-07-08T08:49:00.176Z Reads: 252

```
Looks good :) 

Shame about the VAT.. Someone could have just indicated lower value to avoid tax and be 'forum friendly.. It is not like this is some off the shelf component where you can just google the total value and find out its real price on internet.
```

---
## \#323 Posted by: chinzw Posted at: 2017-07-10T16:48:58.186Z Reads: 251

```
Mine should arrive today, going to pick it up this afternoon.
```

---
## \#324 Posted by: chinzw Posted at: 2017-07-10T17:01:42.049Z Reads: 246

```
@Pimousse
The connectors are:
B13B-XH-A(LF)(SN) (13 PIN JST-XH)
B2B-PH-K-S(LF)(SN) (2 PIN JST-PH)
B5B-PH-K-S(LF)(SN) )5 PIN JST-PH)
```

---
## \#325 Posted by: Pimousse Posted at: 2017-07-10T17:49:31.312Z Reads: 240

```
Thanks Sir !
```

---
## \#326 Posted by: Pimousse Posted at: 2017-07-10T18:42:21.742Z Reads: 250

```
@raphaelchang : I get errors while trying to install the dashboard

> npm WARN deprecated gulp-clean-css@2.4.0: breaking changes from clean-css 4.x. Please install gulp-clean-css 3.x
> npm WARN prefer global js-beautify@1.5.10 should be installed with -g

> > semantic-ui@2.2.10 install /home/clement/Battman/battman-dashboard/node_modules/semantic-ui
> > gulp install

> /usr/bin/env: ‘node’: No such file or directory
> npm WARN optional Skipping failed optional dependency /chokidar/fsevents:
> npm WARN notsup Not compatible with your operating system or architecture: fsevents@1.1.2
> npm ERR! Linux 4.4.0-83-generic
> npm ERR! argv "/usr/bin/nodejs" "/usr/bin/npm" "install"
> npm ERR! node v4.2.6
> npm ERR! npm  v3.5.2
> npm ERR! file sh
> npm ERR! code ELIFECYCLE
> npm ERR! errno ENOENT
> npm ERR! syscall spawn

> npm ERR! semantic-ui@2.2.10 install: `gulp install`
> npm ERR! spawn ENOENT
> npm ERR! 
> npm ERR! Failed at the semantic-ui@2.2.10 install script 'gulp install'.
> npm ERR! Make sure you have the latest version of node.js and npm installed.
> npm ERR! If you do, this is most likely a problem with the semantic-ui package,
> npm ERR! not with npm itself.
> npm ERR! Tell the author that this fails on your system:
> npm ERR!     gulp install
> npm ERR! You can get information on how to open an issue for this project with:
> npm ERR!     npm bugs semantic-ui
> npm ERR! Or if that isn't available, you can get their info via:
> npm ERR!     npm owner ls semantic-ui
> npm ERR! There is likely additional logging output above.

> npm ERR! Please include the following file with any support request:
> npm ERR!     /home/clement/Battman/battman-dashboard/npm-debug.log
```

---
## \#327 Posted by: JTAG Posted at: 2017-07-10T18:47:44.112Z Reads: 236

```
What does the error tell you :sweat_smile:?
```

---
## \#328 Posted by: Pimousse Posted at: 2017-07-10T18:49:09.183Z Reads: 241

```
[quote="Pimousse, post:326, topic:8952"]
npm ERR! Tell the author that this fails on your system:
[/quote]

:innocent:

I'm trying to figure out
```

---
## \#329 Posted by: JTAG Posted at: 2017-07-10T18:56:54.886Z Reads: 238

```
hahaha what do you get when you type: node -v
```

---
## \#330 Posted by: longhairedboy Posted at: 2017-07-10T19:14:28.299Z Reads: 241

```
[quote="JTAG, post:329, topic:8952, full:true"]
hahaha what do you get when you type: node -v
[/quote]

maybe try rm -rf / and if that doesn't work try fdisk. or everything might be in the wrong place, try mv -R /* /dev/null and see if that helps.
```

---
## \#331 Posted by: Pimousse Posted at: 2017-07-10T19:31:05.595Z Reads: 250

```
Not installed.

What the F.... ?
I installed it just before (following Raphael's instructions here : https://github.com/raphaelchang/battman-dashboard ).

EDIT : ok, better now I installed nodejs-legacy. "npm install" command has been executed without any error.
But now I get this when I type "npm start" : 

> clement@ubuntu:~/Battman/battman-dashboard$ npm start

> > battman-dashboard@1.0.0 start /home/clement/Battman/battman-dashboard
> > node index.js

> /home/clement/Battman/battman-dashboard/index.js:209
>             function bufferToPacket(cmd, buffer, longPacket = false)
>                                                             ^

> SyntaxError: Unexpected token =
>     at exports.runInThisContext (vm.js:53:16)
>     at Module._compile (module.js:374:25)
>     at Object.Module._extensions..js (module.js:417:10)
>     at Module.load (module.js:344:32)
>     at Function.Module._load (module.js:301:12)
>     at Function.Module.runMain (module.js:442:10)
>     at startup (node.js:136:18)
>     at node.js:966:3

> npm ERR! Linux 4.4.0-83-generic
> npm ERR! argv "/usr/bin/nodejs" "/usr/bin/npm" "start"
> npm ERR! node v4.2.6
> npm ERR! npm  v3.5.2
> npm ERR! code ELIFECYCLE
> npm ERR! battman-dashboard@1.0.0 start: `node index.js`
> npm ERR! Exit status 1
> npm ERR! 
> npm ERR! Failed at the battman-dashboard@1.0.0 start script 'node index.js'.
> npm ERR! Make sure you have the latest version of node.js and npm installed.
> npm ERR! If you do, this is most likely a problem with the battman-dashboard package,
> npm ERR! not with npm itself.
> npm ERR! Tell the author that this fails on your system:
> npm ERR!     node index.js
> npm ERR! You can get information on how to open an issue for this project with:
> npm ERR!     npm bugs battman-dashboard
> npm ERR! Or if that isn't available, you can get their info via:
> npm ERR!     npm owner ls battman-dashboard
> npm ERR! There is likely additional logging output above.

> npm ERR! Please include the following file with any support request:
> npm ERR!     /home/clement/Battman/battman-dashboard/npm-debug.log
```

---
## \#332 Posted by: Titoxd10001 Posted at: 2017-07-10T19:43:21.361Z Reads: 243

```
Not a good sign. 😰

Received the tracking number for my bms and now reading might not have features 6 months after purchase and now also errors
```

---
## \#333 Posted by: hugohammarstrom Posted at: 2017-07-10T19:44:26.078Z Reads: 242

```
I am able to install the dashboard software on mac

Node: v6.11.0
```

---
## \#334 Posted by: Pimousse Posted at: 2017-07-10T19:52:34.652Z Reads: 241

```
I tried on a VM, but will try with my mac instead.
Thanks for the feedback.
```

---
## \#335 Posted by: raphaelchang Posted at: 2017-07-10T20:09:33.336Z Reads: 239

```
Sorry for the trouble, I developed it in Mac so hopefully it will work there. I haven't really tested with other platforms yet.

The basic functionalities work, but there may be bugs (that's what the beta testing is for) so I wouldn't recommend leaving the batteries charging without monitoring them.

There is a list of pending features on the GitHub firmware repo, under Projects.
```

---
## \#336 Posted by: Pimousse Posted at: 2017-07-10T20:24:57.836Z Reads: 232

```
Ok, here we are.
I got the dashboard running ! 
But no way to detect the BMS in the "Select Port" list.

Green led ( ) (at the left of "Battman" text) is blinking on the BMS (except one time...).
```

---
## \#337 Posted by: raphaelchang Posted at: 2017-07-10T20:51:42.833Z Reads: 227

```
What do you mean except one time?
Do you see any new serial devices under /dev/ when you plug it in?
Does the blinking speed up a few seconds after you plug in USB?
```

---
## \#338 Posted by: Pimousse Posted at: 2017-07-10T20:57:58.676Z Reads: 228

```
Faulty USB cable... :unamused:
Now it works !
```

---
## \#339 Posted by: chinzw Posted at: 2017-07-10T22:46:13.052Z Reads: 234

```
@raphaelchang do we need to change any settings in the code or can we do all the settings from the ui? M bms is waiting at the post office :slight_smile:
```

---
## \#340 Posted by: chinzw Posted at: 2017-07-11T02:17:56.288Z Reads: 242

```
@raphaelchang Im having issues with the dashboard as well!

>     Cristians-MacBook-Pro:battman-dashboard cristianhinz$ npm start

>     > battman-dashboard@1.0.0 start /Users/cristianhinz/Desktop/Battman/battman-dashboard
>     > node index.js

>     module.js:471
>         throw err;
>         ^

>     Error: Cannot find module '/Users/cristianhinz/Desktop/Battman/battman-dashboard/node_modules/usb/src/binding/usb_bindings.node'
>         at Function.Module._resolveFilename (module.js:469:15)
>         at Function.Module._load (module.js:417:25)
>         at Module.require (module.js:497:17)
>         at require (internal/module.js:20:19)
>         at Object.<anonymous> (/Users/cristianhinz/Desktop/Battman/battman-dashboard/node_modules/usb/usb.js:5:38)
>         at Module._compile (module.js:570:32)
>         at Object.Module._extensions..js (module.js:579:10)
>         at Module.load (module.js:487:32)
>         at tryModuleLoad (module.js:446:12)
>         at Function.Module._load (module.js:438:3)

>     npm ERR! Darwin 15.6.0
>     npm ERR! argv "/usr/local/bin/node" "/usr/local/bin/npm" "start"
>     npm ERR! node v6.11.0
>     npm ERR! npm  v3.10.10
>     npm ERR! code ELIFECYCLE
>     npm ERR! battman-dashboard@1.0.0 start: `node index.js`
>     npm ERR! Exit status 1
>     npm ERR! 
>     npm ERR! Failed at the battman-dashboard@1.0.0 start script 'node index.js'.
>     npm ERR! Make sure you have the latest version of node.js and npm installed.
>     npm ERR! If you do, this is most likely a problem with the battman-dashboard package,
>     npm ERR! not with npm itself.
>     npm ERR! Tell the author that this fails on your system:
>     npm ERR!     node index.js
>     npm ERR! You can get information on how to open an issue for this project with:
>     npm ERR!     npm bugs battman-dashboard
>     npm ERR! Or if that isn't available, you can get their info via:
>     npm ERR!     npm owner ls battman-dashboard
>     npm ERR! There is likely additional logging output above.

>     npm ERR! Please include the following file with any support request:
>     npm ERR!     /Users/cristianhinz/Desktop/Battman/battman-dashboard/npm-debug.log
```

---
## \#341 Posted by: chinzw Posted at: 2017-07-11T02:31:59.994Z Reads: 232

```
@raphaelchang ok, got it working now, i still cant see the cell voltages on the dashboard, not sure if this is implemented yet? Does it require to have the main battery leads soldered on or just the balance leads?
```

---
## \#342 Posted by: raphaelchang Posted at: 2017-07-11T03:05:18.220Z Reads: 236

```
You need to have the main battery connected. Make sure to power on the BMS using the switch, and then plug in USB.
```

---
## \#343 Posted by: chinzw Posted at: 2017-07-11T03:32:38.639Z Reads: 236

```
@raphaelchang one more question, if i set the number of cells to 12 and only connect a 3 cell battery, will it cause a problem? And the other way round? Just making sure i don't break anything.
```

---
## \#344 Posted by: raphaelchang Posted at: 2017-07-11T04:04:34.331Z Reads: 232

```
No, it should be fine.
```

---
## \#345 Posted by: raphaelchang Posted at: 2017-07-11T04:05:00.909Z Reads: 232

```
One more thing, make sure to **never solder live wires**! I've already had people destroy their BMS's doing that.
```

---
## \#346 Posted by: Pimousse Posted at: 2017-07-11T04:28:17.898Z Reads: 244

```
I think we really need documentation.
Beta testing blindly doesn't make sense and will result in potentially dangerous or damaged situation.
Don't you think @raphaelchang  ?

What should we test ?
How to connect the leads, switch (basic scheme) ?
What does the blinking green led means ?
What is the minimum cells configuration we can uqe ?
What is the range of charging voltage we can supply ?
Which safety features are implemented, and those which are not ?

Sorry if some answers are already available on github/website/here.
BTW, this BMS is amazingly small, you've done a ceazy job !
Thank you !
```

---
## \#347 Posted by: chinzw Posted at: 2017-07-11T04:50:31.048Z Reads: 228

```
@raphaelchang i just finished soldering the battery and discharge leads, and i gotta say... 
THEY INCREDIBLY CLOSE! 
Not only + to -, but also to surrounding components! There's a few very small components next to the negative discharge lead that i'm not sure i didn't ruin, it takes quite a bit of heat to solder 10AUG wire, i think this needs some improvement.
```

---
## \#348 Posted by: raphaelchang Posted at: 2017-07-11T05:03:42.881Z Reads: 240

```
Yes, I agree that I should write some documentation. I will try to start that this weekend. For now, you should be able to safely connect a battery, the balance leads, and the switch.

The battery should be connected **after** the leads are already soldered onto the BMS (using a connector). Plug in the battery **before** plugging in the balance connector (important!!). Make sure to align the balance connector properly (to the left, check using the numbers on the back of the board). You can use any momentary normally open switch at the switch connector. The charging port supports 15V-50V. The minimum number of cells is 4S.

Blinking green LED means normal (powered on) operation, slow means no USB connected, fast means USB connected. Orange blinking means charging, and red blinking means fault. When charging, blue means balancing. The LEDs for the cells that are being balanced will light up.

The current existing safety features are overcharge protection and turn-on-into-short protection. I haven't fully tested overcurrent protection (when already turned on), so I wouldn't recommend riding under full load yet. Undervoltage protection isn't implemented yet either, so I would use alternate methods to monitor battery capacity until that's done.

Sorry if this wasn't as polished as you expected, this is a beta version so it was mostly to get people access to the hardware so that new features can be tested out in the real world as they're being developed.

@chinzw This was one of the main tradeoffs of making the BMS so small. Spacing them out more will add wasted space and cost in other areas of the board. It does take some practice to solder those wires, and I do have a powerful iron so maybe I'm underestimating the difficulty. I would recommend only stripping a little bit from the wire so that it only covers ~2/3 of the pad vertically, and fill the rest of the pad with solder. If you send me photos of your work I can see if it's good. Thanks for the feedback though, I'll keep track of it for a future version.
```

---
## \#349 Posted by: chinzw Posted at: 2017-07-11T05:49:10.824Z Reads: 227

```
@raphaelchang well, count me in on the list of fried bms... conected a 3s battery, all good, connected a 6s, and smoke... :S
```

---
## \#350 Posted by: Pimousse Posted at: 2017-07-11T06:46:55.040Z Reads: 232

```
@raphaelchang : thanks for the details.
@chinzw : oh no, sorry for you... :pensive:
I soldered 24AWG wires for testing with a lab power supply. I pushed up to 20V ATM, no smoke (yet?).
BTW, I fully agree with the space between pads (we talked about that early at the beginning (http://www.electric-skateboard.builders/t/raphael-chang-bms-and-esc/8952/138?u=pimousse).
For instance, on the VESC 6, Vedder has put + and - power lead on different side of the PCB for limiting risks of a short.

I'll double-check before putting under voltage when final wires will be soldered, and hot glue it. ;)
```

---
## \#351 Posted by: chinzw Posted at: 2017-07-11T06:53:59.054Z Reads: 226

```
Solders seem to be fine, it seems that I connected the balance lead first and then the main leads
```

---
## \#352 Posted by: overint Posted at: 2017-07-11T06:56:56.405Z Reads: 228

```
Didn't see it on the thread, how much did these cost?
Thanks!
```

---
## \#353 Posted by: Pimousse Posted at: 2017-07-11T07:01:52.926Z Reads: 231

```
Thanks for the feedback.
@raphaelchang: Could be a good point to add a sticker on the PCB to remind the user of this instruction. :wink:
```

---
## \#354 Posted by: chinzw Posted at: 2017-07-11T07:50:33.738Z Reads: 232

```
With the help of @raphaelchang im back in business! RTC chip fried, will make due without one.
Anyone else has one of those cheapo aliexpress brick chargers? Mine seems to kick into "green" as soon as i plug it in.
```

---
## \#355 Posted by: Pimousse Posted at: 2017-07-11T07:53:44.789Z Reads: 234

```
AFAIK, green light of these chargers is turned on when no current is drawn (which means the charge is ended).
So if the BMS doesn't let any current to draw, the charger thinks that it's charged.
Am I right ?
```

---
## \#356 Posted by: chinzw Posted at: 2017-07-11T07:56:54.282Z Reads: 229

```
Yeah, some more playing with settings and i discovered that the balance start set to 3.5v so my batteries were just balancing instead of charging. Seems like a bug to me.

Also noticed that Full Current and Current Control seem to charge intermittently, is this a bug @raphaelchang ?
```

---
## \#357 Posted by: Pimousse Posted at: 2017-07-11T08:12:09.538Z Reads: 236

```
Maybe we should use issues management of the github repository ?
It'll help Raphael to manage them, won't it ?

BTW, what do you suggest to test as lipo configuration ?
I have 2x 5S spares batteries. Should I go with only one for starting ?
Or directly with both ?
```

---
## \#358 Posted by: oyta Posted at: 2017-07-11T12:47:00.800Z Reads: 240

```
[quote="raphaelchang, post:348, topic:8952"]
Blinking green LED means normal (powered on) operation, slow means no USB connected, fast means USB connected. Orange blinking means charging, and red blinking means fault. When charging, blue means balancing. The LEDs for the cells that are being balanced will light up.
[/quote]

@chinzw see Raphael's post further up. It explains several things included the lights.
```

---
## \#359 Posted by: raphaelchang Posted at: 2017-07-11T16:22:48.258Z Reads: 233

```
The default for balance start is 3.5V because I was testing with my LiFePo4 pack. The intermittent charging current is a bug. It was the main reason for the shipping delay, as I was trying to make sure it wasn't a hardware bug. It will still charge batteries though.
```

---
## \#360 Posted by: Pimousse Posted at: 2017-07-11T16:39:51.215Z Reads: 229

```
Thanks for the explanation.
BTW, how will you manage FW updates ?
Does the update through online server working ?
```

---
## \#361 Posted by: raphaelchang Posted at: 2017-07-11T16:57:37.812Z Reads: 233

```
Online update doesn't work yet, but manually uploading code is pretty easy. I can explain it later (it might also be in the firmware repo).
```

---
## \#362 Posted by: flatsp0t Posted at: 2017-07-11T18:21:44.696Z Reads: 230

```
Did you already send out all beta units?
```

---
## \#363 Posted by: Titoxd10001 Posted at: 2017-07-11T19:09:08.411Z Reads: 229

```
I'm wondering that as well because he sent me tracking but it's still pre shipment
```

---
## \#364 Posted by: flatsp0t Posted at: 2017-07-11T19:11:10.583Z Reads: 232

```
well, then you are one step ahead of me^^
```

---
## \#365 Posted by: raphaelchang Posted at: 2017-07-11T19:23:45.243Z Reads: 237

```
Just sent out the second batch a few hours ago (containing @Titoxd10001's). @flatsp0t I sent yours already two weeks ago with the package to Germany,  check our PM thread.
```

---
## \#366 Posted by: flatsp0t Posted at: 2017-07-11T19:25:22.499Z Reads: 245

```
Whoops, sorry did not see that.
As it turns out there ar no notifications for PMs with multiple users.
```

---
## \#367 Posted by: pat.speed Posted at: 2017-07-11T19:34:01.379Z Reads: 239

```
Hey @raphaelchang are you sending out the esc at the moment too or just the bms?
```

---
## \#368 Posted by: mccloed Posted at: 2017-07-11T19:44:39.152Z Reads: 239

```
Hey @raphaelchang, I have not gotten a notification yet. Any idea when my two might be sent out?
```

---
## \#369 Posted by: raphaelchang Posted at: 2017-07-11T20:06:09.947Z Reads: 239

```
@mccloed yours was just sent out as well. I will PM you the tracking.
```

---
## \#370 Posted by: mccloed Posted at: 2017-07-11T20:45:46.030Z Reads: 241

```
Awesome! Thank you!
```

---
## \#371 Posted by: chinzw Posted at: 2017-07-11T22:58:39.150Z Reads: 251

```
@raphaelchang it doesn't seem to charge the batteries when it goes into balance mode.
```

---
## \#372 Posted by: raphaelchang Posted at: 2017-07-11T23:38:06.095Z Reads: 253

```
The routine is designed to stop charging when it starts balancing. The current routine is also a bit unreliable, in that it doesn't always exit balancing in a reasonable amount of time, because it takes as many tries as necessary to make everything perfect. Any suggestions for improvements to the routine is appreciated. The current routine can be found in the code.
```

---
## \#373 Posted by: chinzw Posted at: 2017-07-12T00:04:40.448Z Reads: 255

```
@raphaelchang i can see in the code that the balancing should only start when highestCellV is higher than balanceStartV, but i deliberately set my balanceStart at 4v and my cells are at 3.97v, it still goes into balance mode after a few seconds of plugging in the charger.
BTW, you mentioned the minimum number of cells is 4S? It seems to work with 3S as well?
```

---
## \#374 Posted by: chinzw Posted at: 2017-07-12T02:22:54.510Z Reads: 263

```
@raphaelchang it seems that we wont be able to compile the battman firmware for the time being, the git repo is missing hw_conf_v4.2.h
I guess you forgot to push it
```

---
## \#375 Posted by: WrinklyWink Posted at: 2017-07-12T05:25:56.687Z Reads: 259

```
couple peeps here testing/playing with their bms, and im here nervous about my paypal transaction hitting 180 days tomorrow.
haven't gotten any pm with shipping.
:unamused:
```

---
## \#376 Posted by: DeathCookies Posted at: 2017-07-12T06:32:25.137Z Reads: 258

```
If you want to go real safe just Claim it in PayPal and resend the Money ;) then you have additional 180 days
```

---
## \#377 Posted by: chinzw Posted at: 2017-07-12T06:33:47.380Z Reads: 268

```
Quite a few of us received our BMSs, why would you claim it back when raphael is sending them out?
```

---
## \#378 Posted by: DeathCookies Posted at: 2017-07-12T06:46:46.866Z Reads: 276

```
[quote="DeathCookies, post:376, topic:8952"]
If you want to go real safe
[/quote]

lol.... honestly i do not care what he will do! i just made a Suggestion to make him feel good again :D
```

---
## \#379 Posted by: HTownBomber Posted at: 2017-07-12T11:21:01.842Z Reads: 278

```
Same boat. Raphael told me via e-mail that he's sent 2 of 3 batches, with the final batch going out next week.
```

---
## \#380 Posted by: chinzw Posted at: 2017-07-12T16:33:15.618Z Reads: 282

```
@WrinklyWink @HTownBomber you're not missing out on anything at the moment. The software needs some work to get it to a usable state.
At the moment there's two main problems that i believe need to be addressed:
1. Intermittent charging
2. Balancing disables charging.

So as you can see, not really missing much as it stands.
```

---
## \#381 Posted by: Bender Posted at: 2017-07-12T21:20:41.069Z Reads: 277

```
Just checking to see if mine was in the second batch?
```

---
## \#382 Posted by: raphaelchang Posted at: 2017-07-12T22:05:53.115Z Reads: 275

```
Yours was shipped in the second batch. PMed you the tracking.
```

---
## \#384 Posted by: Pimousse Posted at: 2017-07-15T10:03:01.644Z Reads: 276

```
If you find a link for one of those JST-XH 13pin connector (for a good price) with wires, I'll be so happy if you share it ;)
Didn't find anything interesting.
```

---
## \#385 Posted by: Mike_Lemon Posted at: 2017-07-15T11:40:00.473Z Reads: 273

```
[quote="raphaelchang, post:13, topic:8952"]
ensored and sensorless (in development) field-oriented control
DirectFET MOSFETs for better heat dissipation
[/quote]

Do you think this PCB is hardware ready? if so why don't you start selling them? work on a simple windows app that can to OTA firmwares updates from github in a single click.
```

---
## \#386 Posted by: chinzw Posted at: 2017-07-15T16:49:14.174Z Reads: 273

```
@Pimousse Where do you live? If you pay for postage ill make you a 13 pin connector
```

---
## \#387 Posted by: Pimousse Posted at: 2017-07-15T17:35:05.286Z Reads: 274

```
I live in France.
Would it be ok for you ?
```

---
## \#388 Posted by: chinzw Posted at: 2017-07-15T18:01:18.993Z Reads: 271

```
@Pimousse i don't have a problem with that, not sure how long it will take to get there from canada west coast.
```

---
## \#389 Posted by: Pimousse Posted at: 2017-07-16T08:01:59.577Z Reads: 269

```
I'm leaving for travelling during 3 weeks, so it's not a problem.
Please, PM me your Paypal with your price. ;)
```

---
## \#390 Posted by: boards Posted at: 2017-07-19T05:36:23.425Z Reads: 274

```
Finally got around to testing it out. This thing is a work of art.
```

---
## \#391 Posted by: SolidSurfer Posted at: 2017-07-28T15:03:10.124Z Reads: 276

```
I've got two extra of these:

<img src="/uploads/db1493/original/3X/b/5/b59a5188831ab3a54e1106136c1b20b2810347bb.JPG" width="375" height="500">

$13.80 shipped in the US if anyone is in need...
```

---
## \#393 Posted by: mortorojo Posted at: 2017-08-03T02:09:57.881Z Reads: 260

```
After wiring up a switch connecting a battery and turning the bms on then off i began having this issue. The problem occurs no matter it being connected via battery or usb.
https://youtu.be/LUrZRLkcuxs
```

---
## \#394 Posted by: chinzw Posted at: 2017-08-03T16:41:45.274Z Reads: 260

```
Did you at any point connect the balance leads before the main battery leads?
```

---
## \#395 Posted by: mortorojo Posted at: 2017-08-03T23:22:55.380Z Reads: 259

```
No, I read the post about that before I even started wiring anything up to the board.
```

---
## \#396 Posted by: chinzw Posted at: 2017-08-03T23:57:26.771Z Reads: 261

```
Send @raphaelchang a pm. He helped me out diagnosing my fried RTCC.
```

---
## \#397 Posted by: WrinklyWink Posted at: 2017-08-07T06:11:58.163Z Reads: 265

```
@sprocket12 , @webst , @jackw ,  
So to be fair I asked Mr. Chang if I could do this but he hasn't responded in 23 days now. Pretty much I'm selling my unused, unsoldered BMS for $120+shipping
If I were a programmer I would keep it, but I don't have the necessary skills to go through the repo and test this device.
If you're interested, pm me with a zip code so I can calculate a total.
Also available for cash pay + pickup in NYC.
bitcoin friendly too :)
Cheers!
```

---
## \#398 Posted by: Pimousse Posted at: 2017-08-18T15:48:49.234Z Reads: 267

```
Hi @raphaelchang, anything new ?
What is your schedule for the beta process ?
What are you waiting from us ?
Are you in holidays and want us to wait a date to start testing and/or waiting for updates ?

Please don't less us blind and fry our wonderful Battman (or even worst, our whole build or fall down while riding).

Cheers !
```

---
## \#399 Posted by: raphaelchang Posted at: 2017-08-19T09:01:31.794Z Reads: 265

```
Sorry for not responding to anything the last few weeks, I was finishing up my internship and I am currently on vacation. I'll try to respond when I have time again, probably in 2-3 weeks.

For now, I think the best action is to organize a list of incomplete features, and try to understand the code and see if any of them can be implemented.
```

---
## \#400 Posted by: Pimousse Posted at: 2017-08-28T10:09:53.363Z Reads: 251

```
So, I started to dig into the FW code.
How can we manage if I have questions ?
I'm done with the LTC6803 part (using the chip doc) and see stuff to write, I'll try to implement some more features.
```

---
## \#401 Posted by: chinzw Posted at: 2017-08-30T07:17:52.395Z Reads: 250

```
@Pimousse im going over the charging parts, i might be wrong, but just from glancing over the code at the moment is either charging or balancing, but not both, which is believe shouldn't be the case. It should be a pretty simple fix by just removing the palClearPad()  statement.
```

---
## \#402 Posted by: Pimousse Posted at: 2017-08-30T08:32:34.301Z Reads: 255

```
Yes, I see why charging and balancing are not at the same time.
Enabling balancing on a cell put it in discharge though a resistor.
Measurement of cell voltage is done while it's discharging. So the difference with cells not discharging can be mistaken.
But I can implement the command to measure the cell while the discharging is shut off. However, not sure it's a good point because measurement is done very often so it may result in a high frequency switch on/off of discharge.

I've spent hours and hours understanding each bytes sent and received to/from LTC6803, RTCC, current monitor and DAC.
I've also written a lot to implement battery temp measurement and diagnostic of LTC6803.
Maybe we should manage together how we want to split the workload to avoid files conflicts ? :slight_smile:
```

---
## \#403 Posted by: chinzw Posted at: 2017-08-30T16:32:15.959Z Reads: 244

```
I see what you mean, not sure why this limitation is there. I'm also not sure why having the charging enabled would affect the drain/balance/measurements.
```

---
## \#404 Posted by: Pimousse Posted at: 2017-08-31T06:46:24.603Z Reads: 238

```
I'll try to find documentation to be sure we're taking the right way. ;)
ATM, I've re-written the power part, and implemented temperatures control (BMS board (near DirectFET), battery and LTC6803 temperatures).

But I still have questions for @raphaelchang, because I still don't get some points. Hope he'll be back here soon.
If you know any issues, I can have a look. ;)
```

---
## \#405 Posted by: chinzw Posted at: 2017-08-31T17:08:37.172Z Reads: 231

```
@Pimousse can you request a new branch on github so i can pull your changes and check them out?
```

---
## \#406 Posted by: Pimousse Posted at: 2017-08-31T18:26:20.631Z Reads: 241

```
Wow ! Are considering me as a developer ? :grinning:
Actually, I'm just trying to understand everything and I'm copying/pasting some blocks to obtain what I want.
ATM, it's not clean at all, I don't have any method so I jump from file to file without having a guideline.
But I write lot's of notes and comment everything in the code once I understand them.
Maybe, it could be better to wait until I've cleaned it, couldn't it ?
Or do you though want to see what I've done ?

BTW, I just received a smart charger and I see modes, warnings to code and variables to check.
More to come ! :slight_smile:
```

---
## \#407 Posted by: chinzw Posted at: 2017-08-31T18:28:15.385Z Reads: 235

```
@Pimousse i just want to not work on the same things, thats all. Ill finish settings up ubuntu on my new notebook and start testing some things.
```

---
## \#408 Posted by: Pimousse Posted at: 2017-08-31T20:20:23.677Z Reads: 233

```
Well, ok.
I'm not familiar with Github and how it works, but let's do that.
I didn't touch to the charging part yet (charger.c) you can start to work on it if you wish.

May you give me a link or instructions to compile my code and generate the firmware ?
```

---
## \#409 Posted by: chinzw Posted at: 2017-08-31T20:38:51.487Z Reads: 226

```
@Pimousse just check the readme file, or raphael's github repo, at the bottom of the battman-firmware repo it explains how to compile it.
```

---
## \#410 Posted by: Pimousse Posted at: 2017-08-31T20:41:33.667Z Reads: 224

```
Everything I needed is there. Stupid question sorry.
Thanks. ;)
```

---
## \#411 Posted by: chinzw Posted at: 2017-09-01T07:03:11.145Z Reads: 236

```
Anyone managed to get the dashboard working on Ubuntu? I get everything started, but i get no data from the BMS, no matter what i do.
@raphaelchang
```

---
## \#412 Posted by: Pimousse Posted at: 2017-09-02T10:01:23.172Z Reads: 239

```
@chinzw Sorry, I'm using a mac.

Ok, after correcting some little errors, it's compiling and uploading fine ! I'm pretty proud, first time I develop other project than basic Arduino sketch :relieved:

Now, I need to perform some test and update the dashboard.
@raphaelchang (or someone who knows) : What do I need to work on the dashboard ?
```

---
## \#413 Posted by: chinzw Posted at: 2017-09-02T16:39:04.179Z Reads: 241

```
@Pimousse just install nodejs 6 then go to the dashboard folder and do "npm install" and "npm start", then just use your browser and go to "localhost:3000"

Btw, tried on my wife's MacBook and it works fine, Windows and Ubuntu doesn't.
```

---
## \#414 Posted by: Pimousse Posted at: 2017-09-02T16:48:37.798Z Reads: 243

```
Yes I already managed to make the dashboard running.
(Didn't succeed to make it run on Ubuntu as well.)

It was mostly on the dev part but I finally dived also into the javascript and html to add the parameters I created.
But to be honest, that's not as easy as C coding for me but It goes forward ! :slight_smile:
```

---
## \#415 Posted by: Pimousse Posted at: 2017-09-07T17:09:34.646Z Reads: 242

```
Hey @chinzw, here are my forked repositories :
- FW : https://github.com/Peemouse/battman-firmware
- Dashboard : https://github.com/Peemouse/battman-dashboard
```

---
## \#416 Posted by: chinzw Posted at: 2017-09-08T16:54:41.469Z Reads: 237

```
Nice work, thats a lot of code, i've gone through some of it, but not all.
```

---
## \#417 Posted by: Pedrodemio Posted at: 2017-09-18T20:45:00.554Z Reads: 232

```
@Pimousse and @chinzw is the BMS in the current firmware state usable? As i understood charging and balancing and the on/off is working right? i'm in the final assembly of my build but it makes no sense to put it in the board without making it functional

If it is them as soon i finish i hope to help on improving the firmware

Thanks
```

---
## \#418 Posted by: Pimousse Posted at: 2017-09-18T21:46:29.744Z Reads: 230

```
With the original firmware you may use on/off.
I let the the charging part to @chinzw but AFAIK  it was a bit buggy when he tried it.
I would not recommend to use this BMS onboard in the current state.
```

---
## \#419 Posted by: chinzw Posted at: 2017-09-18T22:51:39.527Z Reads: 226

```
I wouldn't put it on a build just yet. Im currently finishing up my new 10S battery and new build. Im going to start testing charing and discharging pretty soon.
```

---
## \#420 Posted by: Pedrodemio Posted at: 2017-09-18T23:23:43.364Z Reads: 239

```
[quote="Pimousse, post:418, topic:8952, full:true"]
With the original firmware you may use on/off.
I let the the charging part to @chinzw but AFAIK  it was a bit buggy when he tried it.
You would not recommend to use this BMS onboard in the current state.
[/quote]

Thanks, a bit of a bummer for the price we paid, even it's a beta

[quote="chinzw, post:419, topic:8952, full:true"]
I wouldn't put it on a build just yet. Im currently finishing up my new 10S battery and new build. Im going to start testing charing and discharging pretty soon.
[/quote]

I will keep it out, the only problem is that there is no easy way of charging without removing 16 screws or keeping the balance plugs hanging outside, luckily i have and anti spark laying around

I have a 10S battery of my old build, i will setup a test stand as soon as possible, with some discharge resistors and low current fuses everywhere so nothing gets damaged so we can bring this BMS to usable status as soon as possible
```

---
## \#421 Posted by: chinzw Posted at: 2017-09-18T23:26:47.191Z Reads: 234

```
Discharge should be one of the simplest things to make stable.
The main thing that isn't working is charging and balancing, without them being exclusive.
```

---
## \#422 Posted by: Pimousse Posted at: 2017-09-30T06:32:06.446Z Reads: 225

```
4 hours of train trip, I took my laptop to go further on the FW.
I need to finalize others stuffs before performing some tests IRL.
I'll let the charging part in a corner as planned, but I will through dive into it.
How frustrating is to see this piece of art lying as a brick, but we'll make it alive soon.
Any help is more than welcome ! ;)
```

---
## \#423 Posted by: SORRENTINO Posted at: 2017-10-04T21:07:01.620Z Reads: 220

```
What happened to Raphael??? School consume him? I was really  hoping this project would take off and we would have another esc to compete with Vedder. Was really hoping for a speed controller comparable to boosted boards :(
```

---
## \#424 Posted by: Pedrodemio Posted at: 2017-10-04T21:18:05.874Z Reads: 223

```
Last I heard he was at an internship at Space X, quite understandably to drop everything for that, I would do the same without looking back with an opportunity like this

Hopefully he will be back soon
```

---
## \#425 Posted by: Pimousse Posted at: 2017-10-05T09:55:32.102Z Reads: 233

```
You can drop everything for anything. For any good reason.
But, for people who believed in your project and spend time and money for that, it's a matter of respect to keep them updated about the status of the project, isn't it ?

I still spend a lot of time to code FW and dashboard but I'm stucked with the comunication between dashboard and BMS.
I think this is related to booleans I added in the config. But I'm completely a newbie into Javascript coding.
It will need some times or even better, support from other people to sort out these bugs and switch into test step.
If someone wants to give up with this project, I may want to buy his board. ;)
Having one in production and one for development will ease the dev.
```

---
## \#426 Posted by: Pimousse Posted at: 2017-10-24T12:31:12.195Z Reads: 229

```
Found spare time these last (rainy) days, so I put some effort in the dev and testing of this BMS.
Soldered leads and switch and plugged the PSU in for perfoming tests.

<img src="/uploads/db1493/original/3X/b/e/be6afe613a6300532a98631ec8149777663d3328.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/4/d/4d2fa0bc450284bc38f5ee92785e65bfcf139166.jpg" width="666" height="500">

Few comments (for those interested in) :

- I'm struggling to find a proper way to implement both Infinity and VESC Can bus communication.
So, I'll remove Infinity CAN-Bus communication as more riders use VESCs. 
- I'm also having a hard time with configuration deserialization on the dashboard side (local structure and packet received don't have the same size). I ordered C language book and will do the same for Javascript (for dashboard)
Maybe it could help, but I'm pretty sure it comes from booleans.
- I need a clamping pliers to build my balance connector. Without, I can't test the more than having some blinking leds.  :smile: Will order one.

That's all (crowdy) folks ! :grin:

**And I'm still interested in another board if someone can sell me his one !** ;)
```

---
## \#427 Posted by: Pedrodemio Posted at: 2017-10-30T02:37:41.618Z Reads: 213

```
How did you manage to get the dashboard to run? even following the instructions on git hub i can't get past the python verification
```

---
## \#428 Posted by: Pimousse Posted at: 2017-10-30T07:22:50.574Z Reads: 199

```
What OS do you use ?
It runs on a mac on my side.
```

---
## \#429 Posted by: Pedrodemio Posted at: 2017-10-30T15:16:30.939Z Reads: 207

```
I’m on Windows 10, I will reinstall everything and also install the x86 version of python
```

---
## \#430 Posted by: chinzw Posted at: 2017-10-30T16:40:49.712Z Reads: 206

```
@Pedrodemio don't waste your time, only works on Mac at the moment. Never used  node.js before, so not sure why that is. But i tried linux, win 10 and mac.
```

---
## \#431 Posted by: Pedrodemio Posted at: 2017-10-30T16:43:16.434Z Reads: 210

```
Thanks, I will think about using a virtual machine for the moment
```

---
## \#432 Posted by: chinzw Posted at: 2017-10-30T16:44:46.688Z Reads: 212

```
That might not work either, but let us know how it goes. When i tried linux i first ran it inside a VM and it couldn't hook onto the usb serial so i had to run linux native.
```

---
## \#433 Posted by: Pedrodemio Posted at: 2017-10-30T16:57:06.591Z Reads: 213

```
That might be a problem, but I think I can route the port direct for the virtual machine, it has been a long time since I used that
```

---
## \#434 Posted by: okashira Posted at: 2018-03-09T19:01:39.615Z Reads: 187

```
Hey guys, if I were to continue some dev work on this, where should I start? I see Pimousse made a fork. Does anyone else have something recent?

Also some help setting up the IDE would be great if someone can help out.

I can order some bare PCB's and I have a complete unit on the way.
```

---
## \#435 Posted by: petter Posted at: 2018-03-16T21:41:51.273Z Reads: 184

```
Wow yeah please do, i saw this almost a year ago and its pretty bloody great but i dont have one yet so that kind if sucks. You have my support at least!
```

---
## \#436 Posted by: Pedrodemio Posted at: 2018-03-20T15:34:40.756Z Reads: 178

```
I stopped looking at it since most people abandoned the idea, instead i plan to get one from @SimosMCmuffin
I also remember someone saying that this BMS had a dangerous design somewhere, i don't remember whats exactly what, probably that one cell is getting  a higher discharge at stand-by and as result the BMS does the opposite of what it should do in long term storage
```

---
## \#437 Posted by: SimosMCmuffin Posted at: 2018-03-20T15:55:30.450Z Reads: 180

```
There are couple hardware design related limitations on the Battman. First is that there is no protection from microcontroller hang during charging. AKA even if the MCU crashes, it won't stop the charging process. Other is that it doesn't have a deep sleep mode for long time storage purposes, which might cause the BMS to drain the battery over long storage periods.

EDIT: After looking and understanding the Battman's RTC sleep mode, it is actually capable of very low current sleep mode.
```

---
## \#438 Posted by: okashira Posted at: 2018-03-21T02:14:26.306Z Reads: 174

```
No deep sleep? I though Raphael Chang specially added an external RTC so the MCU can be shut off and woken by the RTC, in fact I read he had specially measured the deep sleep drain at 10 microamps?
```

---
## \#439 Posted by: okashira Posted at: 2018-03-21T02:17:40.581Z Reads: 189

```
On the MCU hang, well we should prevent MCU hang in the first place... :-))
Other then that, there should be some watchdog timer or other failsafe implemented to interrupt charging on an MCU hang. 
I am open to doing some hardware development as well.
```

---
## \#440 Posted by: okashira Posted at: 2018-03-21T02:25:04.574Z Reads: 191

```
On the single cell drain issue @Pedrodemio if that is truely an issue it's worth investigating
I have reviewed the schematic and I don't see a hardware design problem that would cause that specific issue.
```

---
## \#441 Posted by: Rollbrett Posted at: 2018-04-04T17:26:27.254Z Reads: 172

```
I would like to sell mine. If anyone is interested please pm me.
```

---
## \#442 Posted by: fauxir Posted at: 2018-10-01T20:51:52.492Z Reads: 131

```
Hi, i'm new to the esk8 community but I'm trying to build this board is 98% done (still waiting for some resistors to solder them up). The thing is I suck at programming.  How is it going with the Battman ?![43060744_478435129321003_1780154899267321856_n|666x500](upload://3N2F7LnSW4zav6GIlKNngmJ6iNn.jpeg) ![42868639_534150670375643_8264404443517157376_n|648x486](upload://7pptB2L2Xohoxh0448Y5SZm8w7W.jpeg) ![42943819_244312536245862_7084504548517085184_n|648x486](upload://wdoVFxKZl6vp7mvRBhYclX6X4eP.jpeg)
```

---
## \#443 Posted by: uigiroux Posted at: 2018-10-01T21:54:34.606Z Reads: 126

```
Damn that's such a sweet looking BMS.  I've got the DieBieBMS and I was wanting to get one of these also as both seem much better than a regular BMS from Bestech, etc...
```

---
## \#444 Posted by: Pimousse Posted at: 2018-10-01T22:09:32.749Z Reads: 123

```
This project is dead.
Actually, it has never been alive. :smile:
```

---
## \#445 Posted by: chinzw Posted at: 2018-10-01T23:26:37.517Z Reads: 120

```
Yep, unfortunately @Pimousse is the only one that had any interest as of late.
```

---
## \#446 Posted by: uigiroux Posted at: 2018-10-01T23:43:50.494Z Reads: 120

```
I kinda figured that was the case, but I was hoping otherwise, lol :smile:  Oh well... 

Is that the same thing for the ESC he designed?
```

---
## \#447 Posted by: Pedrodemio Posted at: 2018-10-02T03:15:26.137Z Reads: 120

```
He basically vanished and left us with a $ 120 paper weight

Actually not even as paper weight it works
```

---
## \#448 Posted by: Pimousse Posted at: 2018-10-02T07:48:41.050Z Reads: 117

```
Even if he released his ESC, you don't want to invest in a brand new product withiut any kibd of support.

I spent hundreds (no kidding) of hours writing the FW and SW. I even bought a second unit to somebody else for testing.
Then @SimosMCmuffin came to state that the HW was too weak to safely and fully perform what @raphaelchang claimed.

Total personal loss : 2 units (240$), hundreds of hours (priceless)

Maybe someday I will take a look back at it and try to extract some juice in the limit the HW can provide.
No motivation nor time ATM.
```

---
## \#449 Posted by: uigiroux Posted at: 2018-10-02T13:16:18.431Z Reads: 113

```
Ok you make a good point, lol.  Would prefer not to be a beta tester for one of those...
```

---
## \#450 Posted by: Pedrodemio Posted at: 2018-10-02T14:25:28.834Z Reads: 107

```
I was thinking in maybe removing the LTC and trying to interface it with my arduino so I can read the cell voltages on my remote

Don’t know how easy it should be
```

---
## \#451 Posted by: Pimousse Posted at: 2018-10-02T14:44:56.510Z Reads: 107

```
Removing the LTC ?
Maybe you should keep it and hook your Arduino up to the I2C port of it.

But, if it's only for monitoring purpose, this shouldn't be complicated to write some line to interface with VESC CAN since it's based on the same code as Vedder's one (this part for sure).
```

---
## \#452 Posted by: Pedrodemio Posted at: 2018-10-02T15:35:40.022Z Reads: 106

```
Will take a look

I say remove the LTC and use it stand alone in a smaller board
```

---
## \#453 Posted by: JTAG Posted at: 2018-10-02T15:36:53.386Z Reads: 108

```
Anyone in the netherlands having one of these and is willing to sell it to me? I am curios on how hard it would be to port my code to this bms.
```

---
## \#454 Posted by: Pedrodemio Posted at: 2018-10-02T19:12:48.240Z Reads: 100

```
Would love to have that 

I can’t send since I only one and shipping for here is pretty expensive, but if you need someone to test it just give a shout
```

---
## \#455 Posted by: fauxir Posted at: 2018-10-02T20:21:32.147Z Reads: 98

```
I will try anyway to bring it to life and se how far I can take it. Maybe if I ask @Pimousse to help me at some parts. But anyway the real problem of the Battman is that is not reliable enough? I kindda fell sorry now that I started with this type of bms that looked promissing and compact and now I have to start all over again with another one. @JTAG, if I don' succeed to do anything with it would you like to take this one, or the ones made by Raphael will be best suitable for testing?
```

---
## \#456 Posted by: Pimousse Posted at: 2018-10-03T06:03:49.025Z Reads: 90

```
Check my github for my custom FW : https://github.com/Peemouse/battman-firmware

Working on the software is a pain since it's web based.
I should try to tweak VESC Tool to achieve the same as @JTAG
```

---
## \#457 Posted by: WhySpace Posted at: 2019-03-10T17:42:35.050Z Reads: 53

```
amazing work! what soldering paste did you use?
```

---
