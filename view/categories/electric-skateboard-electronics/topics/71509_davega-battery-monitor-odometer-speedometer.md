# DAVEga: Battery monitor, odometer, speedometer

### Replies: 1584 Views: 25882

## \#1 Posted by: janpom Posted at: 2018-10-17T08:36:32.750Z Reads: 1111

```
Here's a project that I've been working on for quite a while and that I'd like to share with this community since I feel like I owe you guys a lot.

![DSC01596|331x500](upload://fIbhJZXZuUdO4TbxfWrbeudiSXC.jpeg) 

It's a gadget that you plug into a VESC based controller to display some of the most important data, such as battery status, speed and distance travelled. It not only displays the data, but it also stores them and thus it doubles as an odometer. The design is Arduino compatible and thus the firmware can be easily customized without any special equipment.

I know that there have been a number of similar projects, but I wanted a display with nice graphics (instead of text only) and I wanted it to be compact. BTW, the graphics is inspired by @Pimousse's [smart ring](https://vimeo.com/265188386).  

I thought that the gadget would be best demoed in a video. So here it is. Please bear with my presentation skills. :smile:
https://youtu.be/u4e83JhVZNA

Some noteworthy features:
- uses both battery voltage and coulomb counter for estimating current battery capacity
- data retained after powering off and on again
  - updated in reasonable intervals so that the EEPROM doesn't get destroyed (should last for 10,000 km)
- automatic detection of battery fully charged => resets the coulomb counter
- odometer can be initialized to a custom value
- firmware customizable with [Arduino IDE](https://www.arduino.cc/en/Main/Software)
- low cost - less than $10 for the parts

I would like to hear your thoughts and suggestions. Also, please let me know if you'd like one. I will make the code available soon. I want to do a little bit of clean up first. I don't mind embarrassing myself as an DIY builder since I'm a noob, but I don't want to embarrass myself as a software engineer since that's what I've been doing for 20 years+ for living. :smile:

If there's interest, I think I could have professionally built PCBs made and collect the parts for DIY kits. It should be around $10 + shipping. I'm not looking to make money of this. I would love to spread these gadgets among people and it would be great if we can make them better together. For example, it would be helpful if someone designed an enclosure or a panel mount since I personally don't have much experience with that and I don't even have a 3D printer.

Update: There's [a post down there](https://www.electric-skateboard.builders/t/vesc-gauge-battery-monitor-odometer-speedometer/71509/36?u=janpom) that you can like if you'd like one of these.

Update 2: Beta-testing kits can now be ordered [here](https://www.electric-skateboard.builders/t/davega-first-batch-beta-testing/74208).
```

---
## \#2 Posted by: Grozniy Posted at: 2018-10-17T08:42:52.441Z Reads: 871

```
Might be good to incorporate it into @akhlut x things and mount above the front truck
```

---
## \#3 Posted by: brenternet Posted at: 2018-10-17T08:44:14.345Z Reads: 860

```
This is great. I personally wouldn't need something like this but it's clear you've put some good work in here.

Edit. Just watched your video and I'd be nuts not to find a way to incorporate this into a build for $10 right? Even if it's just sitting inside the enclosure gathering odometer readings it's worth the money
```

---
## \#4 Posted by: bigben Posted at: 2018-10-17T08:47:57.517Z Reads: 824

```
This looks very interesting. 
$10????
```

---
## \#5 Posted by: janpom Posted at: 2018-10-17T08:48:49.385Z Reads: 781

```
@Grozniy I'm not aware of the "x things". Could you post a link please.
```

---
## \#6 Posted by: Grozniy Posted at: 2018-10-17T08:49:36.815Z Reads: 757

```
https://www.electric-skateboard.builders/t/what-are-those-x-things-called/32370?u=grozniy
```

---
## \#7 Posted by: janpom Posted at: 2018-10-17T08:51:30.333Z Reads: 736

```
[quote="bigben, post:4, topic:71509"]
$10???
[/quote]

So the display is the most expensive part and you can get it for less than $5 from [AliExpress](https://www.aliexpress.com/item/ILI9225-2-0-Inch-UART-TFT-LCD-Display-Module-SPI-Interface-Colorful-Screen-Serial-Port-176x220/32792711665.html?spm=2114.search0204.3.15.65334a15WTmYzC&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_10059_10696_100031_5017615_10084_10083_10103_451_10618_5017515_452_10304_10307_10820_10821_5017415_10302_5017715,searchweb201603_2,ppcSwitch_5_ppcChannel&algo_expid=331b2bc4-1359-459c-8fb3-16bef1fdcf14-2&algo_pvid=331b2bc4-1359-459c-8fb3-16bef1fdcf14&priceBeautifyAB=0). The chip is around $2 and the USB-UART adapter also around $2. Other than that, it's just small and cheap parts.
```

---
## \#8 Posted by: brenternet Posted at: 2018-10-17T09:00:20.838Z Reads: 709

```
Everything about this is excellent...  except the name.

It needs an epic name, something Will Park industries would be willing to back.

As it's a personal helper of sorts and following the line of recent Amazon and Google naming activity I suggest calling this: Dave
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-17T09:11:10.927Z Reads: 691

```
that looks really great, especially for 10$ why not.
just interested, how the speed and battery voltage calculated?
if I change from 10s to 12s or the gearing the values need to be changed too.

how about water resistens? you think there is an option to get it as min splash proof?
```

---
## \#10 Posted by: Pimousse Posted at: 2018-10-17T09:20:12.899Z Reads: 681

```
Awesome tool !
Proud to be kind of inspiration ! Yours is crazy !
Coulomb counting and non-volatile variables (such as odometer, working hours, etc.) are defo added-value that we miss.
I'd love to see you hardware. Using a Nano (as you mention in your video) is a bit overkill compared to a simple Atmega 328.
I need to go this way for a SmartRing V2 less bulky.

Thanks for sharing and pushing it Open Source. :slight_smile:
```

---
## \#11 Posted by: Skunk Posted at: 2018-10-17T09:42:14.195Z Reads: 661

```
![1g6dnx|480x360](upload://rKG7aEyAF7nj83OrjxUFVovlL92.jpeg) 
Dude.... :+1::+1::+1:
```

---
## \#12 Posted by: Skunk Posted at: 2018-10-17T09:45:32.330Z Reads: 634

```
 would gladly pay a markup for one of these.
```

---
## \#13 Posted by: baxter Posted at: 2018-10-17T10:07:11.465Z Reads: 654

```
Love the design!

I think you have you have kicked a goal in term of feedback to the rider, especially for the cost of components.

I realise this argument is a bit premature, but aesthetically I do think the layout adjustment of the data could be worked on to improve the readability of the Speed graph readout, perhaps rotate the readout 90 degrees to use a landscape orientation for the screen instead of portrait? (because humans).  Regardless, I want one.

And while I can see you have used light blue square blocks on your prototype to demonstrate changes in speed, and green through red for battery capacity, I am sure an enterprising coder can make something a bit more nuanced and refined. 

Suggestion: using inspiration from a Honda S2000 tachometer for the speed graph :smile: 

![image|320x240](upload://ezgn8uCCNgFljWF3uqJqYGkcZsL.jpeg)
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-10-17T10:17:35.001Z Reads: 607

```
How are you going to do coulomb counting? Current clamp or transformer?
```

---
## \#15 Posted by: Skunk Posted at: 2018-10-17T10:47:49.626Z Reads: 596

```
I think it would be great to keep the profile of the device down. rather than mounting the board and Screen together. You can mount the board under the deck inside your enclosure and have a wire going to the screen mounted top side.
```

---
## \#16 Posted by: Andy87 Posted at: 2018-10-17T10:57:42.143Z Reads: 580

```
sandwich style...:sweat_smile: good idea!
```

---
## \#17 Posted by: janpom Posted at: 2018-10-17T11:10:25.975Z Reads: 624

```
Thanks all for the nice comments.

[quote="brenternet, post:8, topic:71509, full:true"]
Everything about this is excellent… except the name.

...

 I suggest calling this: Dave
[/quote]

Uh, OK. :sweat_smile: Is that a random pick or is there an obvious justification that I have missed? I agree it needs an enterprise level name and I have nothing against Dave, but just to give the opportunity to the others, are there any other suggestions? :smile:

[quote="Andy87, post:9, topic:71509"]
just interested, how the speed and battery voltage calculated?
if I change from 10s to 12s or the gearing the values need to be changed too.
[/quote]

Battery voltage is read directly from the VESC. So is the current motor erpm, which can be converted to speed. You need to provide your wheel size and gear ratio in the firmware config variables. The same goes for estimating the battery capacity from the voltage. You need to define the number of cells and you can even customize the discharge ticks, i.e. you can define which voltage corresponds to 100%, 50%, 0% etc. You can make it as finegrained as you want to. 

[quote="baxter, post:13, topic:71509"]
I realise this argument is a bit premature, but aesthetically I do think the layout adjustment of the data could be worked on to improve the readability of the Speed graph readout
[/quote]

Sure. We could have various skins. Landscape orientation is not a problem. If you or anyone else would like to design an alternative skin (as a 176x220 bitmap -- that's the display resolution), I'm happy to do the coding to make it work. Just note that the display resolution is low and complex shapes may not look very nice. That's why I'm using squares, rectangles and simple fonts with no anti-aliasing.

It would also be possible to display more VESC data, such as temperature, motor current, etc.

[quote="Kug3lis, post:14, topic:71509, full:true"]
How are you going to do coulomb counting? Current clamp or transformer?
[/quote]

The coulomb counting is done inside the VESC and I honestly don't know how it's done. I just read the values from the VESC using UART.

[quote="Skunk, post:15, topic:71509, full:true"]
I think it would be great to keep the profile of the device down. rather than mounting the board and Screen together. You can mount the board under the deck inside your enclosure and have a wire going to the screen mounted top side.
[/quote]

Yes, that's definitely possible. It's just a matter of having a cable between the headers and the display rather than plugging the display in directly.
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-10-17T11:18:16.262Z Reads: 555

```
[quote="janpom, post:17, topic:71509"]
The coulomb counting is done inside the VESC and I honestly don’t know how it’s done. I just read the values from the VESC using UART.
[/quote]

Did you read a single vesc or both of them? Because if you running dual you need to have both those values ;)
```

---
## \#19 Posted by: janpom Posted at: 2018-10-17T11:23:12.783Z Reads: 551

```
I read only one and multiply by the number of VESCs (config option). Is that a bad estimate? Reading from both with CANBUS forwarding is of course also possible with some extra work. I think that will be the V2.0. :)
```

---
## \#20 Posted by: janpom Posted at: 2018-10-17T11:40:12.629Z Reads: 556

```
[quote="Andy87, post:9, topic:71509"]
how about water resistens? you think there is an option to get it as min splash proof?
[/quote]

That's a matter of the enclosure, which I don't have and I'm not sure I can design it. But I guess if you can make one that's water-tight around the display, it should make the thing at least splash proof.
```

---
## \#21 Posted by: moon Posted at: 2018-10-17T12:40:55.306Z Reads: 487

```
I'm happy to design an enclosure with you
```

---
## \#22 Posted by: mmaner Posted at: 2018-10-17T13:01:29.867Z Reads: 498

```
@janpom This is impressive.  I am very interested.  Do you have a BOM available?  We should talk.  

If I had measurements I could model enclosures, including a waterproof gasket, for a lot of different decks for those that want to top mount.  I am thinking specifically about the LY Evo, Red Ember Caldera/Bludgeon & Hummie decks.
```

---
## \#23 Posted by: Pedrodemio Posted at: 2018-10-17T13:09:51.983Z Reads: 495

```
Nice one, may I ask how frequently you are saving to the EEPROM

I’m also implementing a odometer in my board and my intention was to use the ERPM to set when to save it

If ERPM is zero or close to zero save all stats to EEPROM, and only save again if the board moves and stop again, this way you never loose distabce
```

---
## \#24 Posted by: Andy87 Posted at: 2018-10-17T13:15:22.044Z Reads: 486

```
one for trampa decks please too ;)
```

---
## \#25 Posted by: mmaner Posted at: 2018-10-17T13:18:57.040Z Reads: 476

```
I don't have a trampa deck, likely I will never have a trampa deck.  If you want to get me measurements or send one for me to measure I'd be glad too.
```

---
## \#26 Posted by: bigben Posted at: 2018-10-17T13:20:59.253Z Reads: 461

```
Yes please to all of these!
```

---
## \#27 Posted by: Andy87 Posted at: 2018-10-17T13:22:56.871Z Reads: 478

```
here the measurements of the nose
https://www.trampaboards.com/manuals/96.pdf
if something missing you need, let me know.
```

---
## \#28 Posted by: mmaner Posted at: 2018-10-17T13:24:26.201Z Reads: 464

```
Will do.  Just need to get the measurements for the monitor, preferably one on hand, and I can get started.
```

---
## \#29 Posted by: Skunk Posted at: 2018-10-17T13:24:58.078Z Reads: 456

```
Yaaas. I knew you would be all over this
```

---
## \#30 Posted by: janpom Posted at: 2018-10-17T13:43:51.314Z Reads: 476

```
@moon @mmaner Cool! Thanks for offering to help with the enclosure. Here are my thoughts. It would be nice to have two types of mounts. One for mountain board with top mounted battery/ESC enclosures where you would mount to the lid of the enclosure. That wouldn't require full housing, only a panel mount, i.e. something [like this](
https://www.aliexpress.com/item/Power-Indicator-Battery-Meter-LYLCD/1547802368.html).

The second type would be for mounting on the front part of a deck, possibly as a part of the X thingy as @Grozniy suggests or in a full housing with mounting holes, i.e. something [like this](https://www.aliexpress.com/item/JUNTEK-VAT1300-100V-300A-Wireless-voltage-and-current-meter-Car-battery-monitoring-12V-24V-48V-battery/32867188239.html?spm=2114.search0104.3.2.3b3e2aebVatSfi&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_318_319_10696_450_10084_10083_10618_452_535_534_10304_533_10307_10820_532_10821_10302_204_10059_10884_323_10887_100031_320_10103_448_449,searchweb201603_2,ppcSwitch_0&algo_expid=dc583816-ea24-4995-87b7-df862c3c7531-0&algo_pvid=dc583816-ea24-4995-87b7-df862c3c7531&transAbTest=ae803_4). There are two options here. 1) Put the whole thing into the enclosure. 2) Only put the display into the enclosure and keep the PCB near the VESC.

What do you guys think? What dimensions do you want me to measure?
```

---
## \#31 Posted by: mmaner Posted at: 2018-10-17T13:45:41.381Z Reads: 473

```
I think separating the 2 pieces, while it increases the level of complication, lowes the risk of damage to half the unit and makes the enclosure a lot smaller.  

Ideally I need the full body measurements of the assembled unit, and the individual halves.

If you can PM me the BOM I can order the pieces and do the assembly here.  Or if you have an extra you can loan me Ill send it back when I'm done.
```

---
## \#32 Posted by: janpom Posted at: 2018-10-17T14:10:19.149Z Reads: 495

```
[quote="mmaner, post:31, topic:71509"]
I think separating the 2 pieces, while it increases the level of complication, lowes the risk of damage to half the unit and makes the enclosure a lot smaller.
[/quote]

In fact, it doesn't really make it a lot smaller unless you cut or bend the pins:
![IMG_1420|690x333](upload://OrW5lm5JA280Th6T5Gtg7e4Liy.jpeg) 

The display can be [purchased on Amazon for a more expensive price](https://www.amazon.com/Display-176x220-ILI9225-Peripheral-Interface/dp/B07HF7WVST/ref=sr_1_1?ie=UTF8&qid=1539784607&sr=8-1&keywords=176x220+display), but I guess then you won't need to wait for it for a month.

Other than that, the chip is the bulkiest part. It's the atmega 328 in the DIP package. I believe the vertical size is the same as any other DIP package MCU. If you cut a piece of perfboard in the same size as the display and put both the chip and the display on it, you should have a good idea about the assembled dimensions.

I currently only have a single prototype on a perfboard. It needs at least one tweak. The 4 pins used for connecting to the VESC need to be replaced with a 90 degrees 4 pin JST connector that I will have to order since I'm unable to get it locally. The pins don't work. The cable keeps sliding off.

I'm going to order professionally manufactured PCBs and put together assembly kits that I can send out to anyone interested for the cost of the parts and shipping. I can send one to you then as well. It will take a while though since I will be ordering from China to keep the costs down. If you're eager to start designing the enclosure in the meantime, I believe the display is the most critical part to have for that.
```

---
## \#33 Posted by: mmaner Posted at: 2018-10-17T14:12:19.409Z Reads: 449

```
I'll order the display so I can get started.  Id love to have one of the manufactured PCB's and assembly kits as well.  

Do you have a link to the atmega 328 in the DIP package?  I'll order one of those as well.
```

---
## \#34 Posted by: Battosaii Posted at: 2018-10-17T14:24:08.771Z Reads: 469

```
Looks pretty similar to this. 

https://www.electric-skateboard.builders/t/proton-digital-instrument-and-control-panel-touch-screen/58664

I have mine on order just waiting for him to finish them and ship em out.
```

---
## \#35 Posted by: Pimousse Posted at: 2018-10-17T14:26:50.663Z Reads: 536

```
That was also the way I planned to use.
At first, I thought about using FAULT_CODE_UNDERVOLTAGE (= power switch off), but it's a bit dangerous writing EEPROM whike powering down...
```

---
## \#36 Posted by: janpom Posted at: 2018-10-17T14:29:44.318Z Reads: 552

```
Alright, guys. Seems like there's at least a few people who'd like one of these gadgets. I'm going to order the parts and I need to know at least a rough number. Anyone interested, please like this post. I mean this particular post (not the first post in the thread). The cost should be around $10 + shipping. I won't be making money on this. I'll only ask you for what I paid for the parts and the shipping. Please note that the gadget hasn't gone through much testing, so please only sign up for the first batch if you don't mind being a guinea pig. I'll do my best to fix problems as they come up. The gadget assembly will require some easy DIP soldering. I will try to put together detailed instructions. Anyone should be able to do it. I can send a few assembled as well. I like to solder.  It's very relaxing. :slight_smile: 

Please don't like this post if you don't want the gadget kit. :smile:
```

---
## \#37 Posted by: Battosaii Posted at: 2018-10-17T14:31:30.625Z Reads: 530

```
Wow for $10 plus shipping I'm down. I can experiment with this and maybe use it on my second board.
```

---
## \#38 Posted by: Mich21050 Posted at: 2018-10-17T14:32:12.183Z Reads: 537

```
I would also be down for one :slight_smile:
```

---
## \#39 Posted by: janpom Posted at: 2018-10-17T14:33:05.154Z Reads: 540

```
[quote="Battosaii, post:34, topic:71509"]
Looks pretty similar to this.

![|20x20](/user_avatar/www.electric-skateboard.builders/wajdi/40/72535_1.png) [Proton- Digital Instrument and Control Panel Touch Screen](https://www.electric-skateboard.builders/t/proton-digital-instrument-and-control-panel-touch-screen/58664) [Esk8 Electronics](/c/electric-skateboard-electronics)
[/quote]

Oh that one looks very nice. I wasn't aware of it. Well, competition is always good. :slight_smile:
```

---
## \#40 Posted by: janpom Posted at: 2018-10-17T14:35:29.414Z Reads: 529

```
[quote="mmaner, post:33, topic:71509"]
Do you have a link to the atmega 328 in the DIP package? I’ll order one of those as well.
[/quote]

[Here's](https://www.amazon.com/Atmega-328P-PU-Arduino-Loader-ATMEL/dp/B01GWYUXP4/ref=sr_1_10?ie=UTF8&qid=1539786801&sr=8-10&keywords=atmega+328p) one that I quickly found on Amazon.
```

---
## \#41 Posted by: moon Posted at: 2018-10-17T14:36:55.338Z Reads: 466

```
I guess we don't need 2 people designing the same thing
```

---
## \#42 Posted by: Wraith Posted at: 2018-10-17T14:37:42.718Z Reads: 453

```
Just when I run out of likes for the day :sob:
```

---
## \#43 Posted by: janpom Posted at: 2018-10-17T14:40:24.652Z Reads: 472

```
[quote="Pedrodemio, post:23, topic:71509"]
Nice one, may I ask how frequently you are saving to the EEPROM
[/quote]

I think we had the same idea about this. I save after each 100 meters traveled (configurable) or whenever the board comes to a stop. In the latter case, I also check that at least X seconds elapsed since the last save. This is to prevent too frequent EEPROM writes in case the erpm indicate stop-go-stop-go sequences in a very quick succession for whatever reason (this is just a safeguard; I haven't really noticed that to happen when testing).
```

---
## \#44 Posted by: Battosaii Posted at: 2018-10-17T15:02:17.976Z Reads: 448

```
I'm still down for buying your kit and putting it together my self maybe I'll even like it better than the Photon one.
```

---
## \#45 Posted by: mmaner Posted at: 2018-10-17T15:11:55.148Z Reads: 446

```
Awesome, Ill get them ordered.
```

---
## \#46 Posted by: Pimousse Posted at: 2018-10-17T15:21:19.881Z Reads: 448

```
I would consider a higher cost.
You'll have to manage a ton of questions, remarks, support, especially every VESC FW update.
That deserves a bit more money ;)
```

---
## \#47 Posted by: brenternet Posted at: 2018-10-17T15:42:33.953Z Reads: 459

```
[quote="janpom, post:17, topic:71509"]
> I suggest calling this: Dave

Uh, OK. :smile: Is that a random pick or is there an obvious justification that I have missed? I agree it needs an enterprise level name and I have nothing against Dave, but just to give the opportunity to the others, are there any other suggestions? :smile:
[/quote]

I put the request for a name through a long and arduous testing panel of marketing experts and the answer was unanimous. Dave. 

It came to me in 3 seconds while drinking a coffee and watching someone wash my car, because while you're out there creating amazing content for our community and adding real value to this forum I'm too lazy to even wash my own car 🤣

I think this qualifies me though.
```

---
## \#48 Posted by: thisguyhere Posted at: 2018-10-17T15:49:59.704Z Reads: 419

```
i'd like one as well, where are you based?

also, for those running mono drives with bt module connected to uart, the vesc gauge would have to take its place, right?

for dual drives, plug the gauge into the controller without bt installed?
```

---
## \#49 Posted by: mmaner Posted at: 2018-10-17T15:52:31.016Z Reads: 416

```
I would assume so, but there are some programming changes you have to make to get both bluetooth devices to work.  I don't remember off the top of my head but Ill look it up and post it.
```

---
## \#50 Posted by: Pedrodemio Posted at: 2018-10-17T16:05:54.205Z Reads: 455

```
[quote="Pimousse, post:35, topic:71509, full:true"]
That was also the way I planned to use.
At first, I thought about using FAULT_CODE_UNDERVOLTAGE (= power switch off), but it’s a bit dangerous writing EEPROM whike powering down…
[/quote]

That could be, I saw a lot of people doing something similar using a big capacitor on the arduino input so it has time to complete the save, but I guess it only works if you are using an external 5v dc dc converter or the cap may have to be a lot bigger to keep both the logic of both VESC’s on for enough time


[quote="janpom, post:43, topic:71509"]
I think we had the same idea about this. I save after each 100 meters traveled (configurable) or whenever the board comes to a stop. In the latter case, I also check that at least X seconds elapsed since the last save. This is to prevent too frequent EEPROM writes in case the erpm indicate stop-go-stop-go sequences in a very quick succession for whatever reason (this is just a safeguard; I haven’t really noticed that to happen when testing).
[/quote]

Could be, at least in my head a lot less writes will happen doing just when stopping
I remember seeing that on FOC the erpm does not goes to zero when stoped, it swings a little bit, may need to pay atention to that

But either way, using your method you would need at least 10000 km to reach the eeprom limit, and from a test I saw they last way more than that
```

---
## \#51 Posted by: Andy87 Posted at: 2018-10-17T16:42:04.388Z Reads: 398

```
It’s way much more cheap. So why not?
```

---
## \#52 Posted by: Andy87 Posted at: 2018-10-17T16:44:58.337Z Reads: 422

```
Definitely down for one.
I don’t need it to perfect.
Speed and bat monitoring is the main thing i want to see without to watch my app or on a remote.
```

---
## \#53 Posted by: deucesdown Posted at: 2018-10-17T16:47:00.477Z Reads: 444

```
I suggest this UI

https://lostinatx.files.wordpress.com/2011/11/img_1118.png
```

---
## \#54 Posted by: janpom Posted at: 2018-10-17T18:52:11.494Z Reads: 435

```
[quote="thisguyhere, post:48, topic:71509"]
i’d like one as well, where are you based?
[/quote]

I'm in Czech Republic. I'm not sure if shipping to you guys in US is worth it. It will likely cost more than the parts. We'll figure something out.

[quote="thisguyhere, post:48, topic:71509"]
also, for those running mono drives with bt module connected to uart, the vesc gauge would have to take its place, right?
[/quote]

I'm afraid that's right.

[quote="thisguyhere, post:48, topic:71509"]
for dual drives, plug the gauge into the controller without bt installed?
[/quote]

I think so. I tested it plugged into both the master and slave VESC and both worked just fine. I didn't have the BT installed in the other one, but I can't see how that could change anything.
```

---
## \#55 Posted by: janpom Posted at: 2018-10-17T18:56:00.272Z Reads: 402

```
I was thinking about the name and while Dave surely sounds tempting, I think I'll call it VeGa. Sorry @brenternet. Thanks for the suggestion though! :smile:
```

---
## \#56 Posted by: moon Posted at: 2018-10-17T18:56:11.159Z Reads: 399

```
Whats more cheap? I am happy to design one either way
```

---
## \#57 Posted by: brenternet Posted at: 2018-10-17T18:57:52.724Z Reads: 403

```
You're dead to me.
```

---
## \#58 Posted by: thisguyhere Posted at: 2018-10-17T18:57:56.371Z Reads: 416

```
[quote="janpom, post:54, topic:71509"]
I’m in Czech Republic. I’m not sure if shipping to you guys in US is worth it. It will likely cost more than the parts. We’ll figure something out.
[/quote]

sounds like you're working with @mmaner to a get version working for him?  if that works out, we can probably assemble them here...?
```

---
## \#59 Posted by: mmaner Posted at: 2018-10-17T19:00:07.197Z Reads: 409

```
I'm just doing the model for now.  After that I'm going to try and get a working prototype, once @janpom gets his PCB's in. 

Once everything is settled, I'm sure we can work out a distribution arrangement with @janpom on his PCB's and/or kits.  Your prolly the guy to do that @thisguyhere
```

---
## \#60 Posted by: thisguyhere Posted at: 2018-10-17T19:01:45.224Z Reads: 394

```
sounds good mike, whatever i can do to help, let me know.  would love to try this.
```

---
## \#61 Posted by: totalgeek9224 Posted at: 2018-10-17T19:02:20.242Z Reads: 353

```
Love the collab going on here. I'd love to help in anyway possible!  Keep up the great work guys
```

---
## \#62 Posted by: Andy87 Posted at: 2018-10-17T19:02:36.842Z Reads: 360

```
I thought you speak about the proton or photon.
The other guy who made a display too...
Looks like I understood it wrong 🙈
```

---
## \#63 Posted by: moon Posted at: 2018-10-17T19:04:21.713Z Reads: 356

```
Yeah I was talking about designing a case for this, it looks like @mmaner is going to do it so I will leave it to him
```

---
## \#64 Posted by: Andy87 Posted at: 2018-10-17T19:07:50.700Z Reads: 365

```
Than forget about what I said...
Sorry for that.
```

---
## \#65 Posted by: mmaner Posted at: 2018-10-17T19:11:33.658Z Reads: 368

```
Im happy for you to do one too, its not a competition :slight_smile:
```

---
## \#66 Posted by: Skunk Posted at: 2018-10-17T19:14:54.443Z Reads: 364

```
More opinions are always a good thing
```

---
## \#67 Posted by: moon Posted at: 2018-10-17T19:16:57.930Z Reads: 361

```
Yeah ofc, I love open projects so let me know when you have critical dimensions and I will also try something. I think there are some dimensions online for the display.  I would probably design a case for the display and arduino so waiting for pcb aswell
```

---
## \#68 Posted by: mmaner Posted at: 2018-10-17T19:20:55.396Z Reads: 355

```
I think its going to have to be an inclusive model, meaning meaning both pieces actually cannot be split as there is button that needs to be accessible from the display section but connects to the arduino.
```

---
## \#69 Posted by: Skunk Posted at: 2018-10-17T19:20:57.194Z Reads: 351

```
@mmaner @moon whem making the mount, if you're going for over the truck like x things. Please keep in mind spacing for those who mount drop through. Maybe a small second piece to act as a riser so those that dont mount drop save the exta few mm of height.
```

---
## \#70 Posted by: mmaner Posted at: 2018-10-17T19:21:53.369Z Reads: 345

```
good idea, will make the gasket difficult, but I think it can be solved.
```

---
## \#71 Posted by: Skunk Posted at: 2018-10-17T19:23:08.836Z Reads: 336

```
Thanks bud
```

---
## \#72 Posted by: AreaKruzer Posted at: 2018-10-17T19:55:44.972Z Reads: 369

```
Hey janpom,

Great work so far. I was wondering if using a SMD Atmega2560(Arduino mega processor) would be good. 

The atmega have 4 uart ports. Meaning 2 vesc can feed data into it to do a coulomb counting and also possibly forward the data using another uart connected to the bt module 

Also instead of writing the data of the EEPROM, is it possible to write it onto a microSD? Of cos EEPROM, will write faster than a microSD,but at least microSD will be easier to replace as compared to the EEPROM, which is the chip itself.
```

---
## \#73 Posted by: Jake2k17 Posted at: 2018-10-17T20:18:53.086Z Reads: 352

```
This is pretty awesome man, nice job. Is there any way to convert the measurements to Imperial instead of metric?
```

---
## \#74 Posted by: janpom Posted at: 2018-10-17T20:36:04.671Z Reads: 369

```
I'm still thinking what would be the best way to distribute the parts. The main components are the PCB, display, chip, and USB-UART adapter. As for the latter three, we don't really save anything by me doing the distribution since everyone could order those themselves from AliExpress (or similar) with free shipping. For example:

- [display](https://www.aliexpress.com/item/ILI9225-2-0-Inch-UART-TFT-LCD-Display-Module-SPI-Interface-Colorful-Screen-Serial-Port-176x220/32792711665.html?spm=2114.search0104.3.8.3fc12510d3yVHc&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_318_319_10696_450_10084_10083_10618_452_535_534_10304_533_10307_10820_532_10821_10302_204_10059_10884_323_10887_100031_320_10103_448_449,searchweb201603_2,ppcSwitch_0&algo_expid=cc29c9d0-515b-4481-92b6-cf84a26d2a5c-1&algo_pvid=cc29c9d0-515b-4481-92b6-cf84a26d2a5c&transAbTest=ae803_4)
- [chip](https://www.aliexpress.com/item/ATMEGA328P-ATMEGA328P-PU-DIP-28-New-parts-best-price-and-short-lead-time/32824808024.html?spm=2114.search0104.3.96.79cfbf90oHec3C&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_318_319_10696_450_10084_10083_10618_452_535_534_10304_533_10307_10820_532_10821_10302_204_10059_10884_323_10887_100031_320_10103_448_449,searchweb201603_2,ppcSwitch_0&algo_expid=9550205c-1e81-49da-8007-229c64716265-16&algo_pvid=9550205c-1e81-49da-8007-229c64716265&transAbTest=ae803_4)
- [USB adapter](https://www.aliexpress.com/item/1PCS-CP2102-USB-2-0-to-TTL-UART-Module-6Pin-Serial-Converter-STC-Replace-FT232/32717057832.html?spm=2114.search0104.3.9.17102e7bLoEObF&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_318_319_10696_450_10084_10083_10618_452_535_534_10304_533_10307_10820_532_10821_10302_204_10059_10884_323_10887_100031_320_10103_448_449,searchweb201603_2,ppcSwitch_0&algo_expid=b3aed8e1-58e3-43cb-9f5a-3217d2348eda-1&algo_pvid=b3aed8e1-58e3-43cb-9f5a-3217d2348eda&transAbTest=ae803_4)

What remains are only small parts, such as
- 10k resistor
- 20pF and 100nF capacitors
- 16 MHz crystal
- diode
- pins / headers / JST connectors
- PCB spacers

Each you can get like 100 pieces for $1. Unfortunately, if you need just 1, it's about the same price. So it does make sense to make kits with these, but at the end of the day, the savings will likely be less than $5 per kit. Not sure if it's worth it.

The PCB is the only tricky one. I think it will be much more expensive if everyone orders their own. Please correct me if I'm wrong. And then if one person (me) orders all the PCBs to distribute to others, it makes sense to distribute at least the small parts as well. What do you guys think? I have never done this before so some advice would be much appreciated.
```

---
## \#75 Posted by: janpom Posted at: 2018-10-17T20:42:53.494Z Reads: 360

```
There are definitely many ways you can do this. I tried to keep it simple. SMD would be difficult to solder for some people (me included). MicroSD is a valid option, but why bother if the EEPROM lasts for 10,000 km after which you need to replace a $2 chip?

BTW, the display does have a MicroSD slot. I haven't looked into this, but maybe it's possible to wire it to the PCB and update the firmware to use it instead of the EEPROM.
```

---
## \#76 Posted by: janpom Posted at: 2018-10-17T20:47:31.130Z Reads: 389

```
[quote="Jake2k17, post:73, topic:71509"]
Is there any way to convert the measurements to Imperial instead of metric?
[/quote]

I don't have it implemented, but it's straightforward. I'm putting it on my todo list.

Though I would recommend that you guys really start rethinking this imperial units idea. :smile:

https://i.redd.it/2zvqpynr264z.png
```

---
## \#77 Posted by: deucesdown Posted at: 2018-10-17T20:58:29.684Z Reads: 373

```
[quote="janpom, post:76, topic:71509"]
imperial units
[/quote]

I used to feel this way, but amazingly, this blog post (and the comments) really made me think. Imperial has its advantages.

https://www.theenglishwoodworker.com/metric-vs-imperial/

I've now readjusted my stance, and have an absolute mess again. lol.
```

---
## \#78 Posted by: deucesdown Posted at: 2018-10-17T21:07:34.925Z Reads: 374

```
from comments in above,

[quote]
Base 12 and base 16 divide into more equal parts then base 10, metric only divides by 2 and 5. This means it is MUCH easier to think proportionally using imperial. Halves, quarters, eighths, thirds (in the case of inches) and sixteenths, easy in imperial, next to impossible in metric. I work in professional theater, I’ve seen dozens of designers from overseas, (metric using countries) that can’t see proportionally. Their designs tend to look like your looking at them through a warped lens.
You can work proportionally in metric, you just end up with some weird numbers, which as mentioned in this article, can be hard to locate on your layout tools, and aren’t standard sizes of materials or hardware.

I took a lot of physics in college, loved metric for that.
[/quote]

[quote]
The divisibility of 12 is a major advantage of inches and feet. 10 is only divisible by 5 and 2, but 12 is divisible 2,3,4,6 (and sort of 8). This makes measuring 1/4, 1/3, 1/2, 2/3, 3/4 of a length much easier with feet &amp; inches. Consider that there are 360 degrees in a circle for similar (but not quite the same) reasons. This is not accidental. Metric seems easier to us today in the age of digital calculators, but in the age of mechanical dividers and slide rules, 12 segments is superior. The imperial system is not arbitrary or random, as I had long suspected; it has a logic of its own.
[/quote]
```

---
## \#79 Posted by: Skunk Posted at: 2018-10-17T21:11:36.763Z Reads: 346

```
I would definitely prefer MPH,  but its not a deal breaker
```

---
## \#80 Posted by: thisguyhere Posted at: 2018-10-17T21:14:24.000Z Reads: 368

```
[quote="janpom, post:74, topic:71509"]
And then if one person (me) orders all the PCBs to distribute to others, it makes sense to distribute at least the small parts as well.
[/quote]

absolutely agree.  if you could source the parts, get the PCB printed, etc, then mail in bulk to one person in north america.

does not make sense for you to send these out individually across the ocean.

in terms of assembly, from your photo in the original post, looks like components are through-hole mounted?  if so, i can try assembling one and maybe take on the task of kitting them out for people on this side of the world.
```

---
## \#81 Posted by: mmaner Posted at: 2018-10-17T22:16:34.631Z Reads: 332

```
This @janpom, make the most sense to me.
```

---
## \#82 Posted by: Jake2k17 Posted at: 2018-10-17T22:19:52.632Z Reads: 316

```
Yeah, metric is easier, but living in the US, if you can’t beat them, join them
```

---
## \#83 Posted by: b264 Posted at: 2018-10-17T22:35:08.760Z Reads: 322

```
"MAH" is mega-amp-henries and "mAh" is milli-amp-hours

"km" is kilo-meter and "km/h" is kilometers per hour

Scientific units have certain conventions and standards for certain reasons, and if they aren't correct, then they are incorrect.  Science and math are universal and go beyond language barriers.
```

---
## \#84 Posted by: bsancken Posted at: 2018-10-17T22:49:24.357Z Reads: 332

```
I have everything other than the display and chip on hand so I would definitely be able to assemble my own!

(as for the pcb, if its 2 layer JLC can get 10 to the US for less than ~15USD, just an fyi) 
Otherwise, once you have good pcbs you could order them to be shipped from the factory to a distributer in the US to save postage for you being the MITM.

Also I second the imperial conversion and the ability for this to be connected in parallel with the serial output for BT or other arduinos (such as speed based underglow)!

Also(2) wondering about power draw from the 5v line on the VESC. Is it within a reasonable amount? How does it do in sunlight brightness wise?

Thanks!
```

---
## \#85 Posted by: Skunk Posted at: 2018-10-17T22:51:23.859Z Reads: 315

```
[quote="bsancken, post:84, topic:71509"]
How does it do in sunlight brightness wise?
[/quote]

That's a really good question.
```

---
## \#86 Posted by: Battosaii Posted at: 2018-10-17T22:53:44.051Z Reads: 301

```
That's a great question, 80% of my rides are at night but I would like to be able to see the screen in day time.
```

---
## \#87 Posted by: Skunk Posted at: 2018-10-17T22:56:49.571Z Reads: 294

```
Same, most my commute is night riding.
```

---
## \#88 Posted by: dareno Posted at: 2018-10-18T02:58:50.315Z Reads: 305

```
[quote="brenternet, post:47, topic:71509"]
I put the request for a name through a long and arduous testing panel of marketing experts and the answer was unanimous. Dave.
[/quote]

If I didn't already know and if there were no other clues, this right here would have absolutely and completely convinced me that you were an Englishman.
```

---
## \#89 Posted by: lrdesigns Posted at: 2018-10-18T03:33:43.083Z Reads: 321

```
Really cool man. I would be happy to get a kit, if it can be delivered for $25 then I think that is a great deal!

I like the feature set you have programmed, but there is just one other feature I would really want. I want to know if I got an error message during my ride. Even if it does not say what the error is I can at least know to connect my vesc to a PC before I switch off my board. @janpom If it's difficult or too time consuming to program this maybe its something that could be added later? 

Also I wouldn't mind having a go at designing a waterproof case. Even just for my own use. Will your final PCB have mounting holes, or should we just use the mounting holes on the LCD?
```

---
## \#90 Posted by: dareno Posted at: 2018-10-18T03:39:59.045Z Reads: 307

```
@janpom cool af idea and don't worry about the competition because that enclosure on the proton is naff.
@mmaner will make yours so much better.   (no pressure)   
@brenternet  I would have called it Alan
```

---
## \#91 Posted by: janpom Posted at: 2018-10-18T05:28:29.244Z Reads: 315

```
[quote="bsancken, post:84, topic:71509"]
Also(2) wondering about power draw from the 5v line on the VESC. Is it within a reasonable amount?
[/quote]

It draws between 90 and 100 mA, at least with my ESCapes.

[quote="bsancken, post:84, topic:71509"]
How does it do in sunlight brightness wise?
[/quote]

It's a cheap TFT display so you can't expect miracles on direct sunlight. It should still be better than OLED. Unfortunately, the brightness is not configurable with this particular one.

Maybe @mmaner or @moon could do some clever sunlight shielding on the enclosure. What do you guys think?
```

---
## \#92 Posted by: janpom Posted at: 2018-10-18T05:33:45.823Z Reads: 307

```
[quote="lrdesigns, post:89, topic:71509"]
I want to know if I got an error message during my ride.
[/quote]

It's definitely a good idea. I'm adding it on my todo list. The priority now though will be to make the kits, get the gadgets among people, test and fix any problems such that the basic functionality is working correctly. Then we can start adding more features. I hope that someone else will help with FW development. I'm currently between jobs with a plenty of time on hands but I'm starting a new job in November and then my time for this is limited.
```

---
## \#93 Posted by: janpom Posted at: 2018-10-18T05:54:27.439Z Reads: 290

```
After more thinking about the kits, here's my plan. I will get all the parts but the display. A few reasons for that. First, everyone can get the display from China with free shipping. We don't save money if I get them and distribute. It currently looks like there will be around 30 kits. I don't think that's enough for negotiating a bulk discount. Second, if I order 30 displays, that would be ~$150 and there's a risk I get hit by import taxes. Third, it will bring the kit cost down to ~$5 and I don't mind paying $150 for 30 kits without collecting advance payments, which will make things easier. I would be more reluctant to pay $300.

I hope this is OK. So if you're interested in the VeGa kit, **please go ahead and order the display now**. [Here's](https://www.aliexpress.com/item/ILI9225-2-0-Inch-UART-TFT-LCD-Display-Module-SPI-Interface-Colorful-Screen-Serial-Port-176x220/32792711665.html?spm=2114.search0104.3.8.3fc12510d3yVHc&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_318_319_10696_450_10084_10083_10618_452_535_534_10304_533_10307_10820_532_10821_10302_204_10059_10884_323_10887_100031_320_10103_448_449,searchweb201603_2,ppcSwitch_0&algo_expid=cc29c9d0-515b-4481-92b6-cf84a26d2a5c-1&algo_pvid=cc29c9d0-515b-4481-92b6-cf84a26d2a5c&transAbTest=ae803_4) one source. I haven't actually purchased mine from them so I can't give any references (I got mine locally for a much higher price). If anyone knows about a better source please let us know.
```

---
## \#95 Posted by: janpom Posted at: 2018-10-18T06:02:58.309Z Reads: 296

```
What would be the best way to go about the cables and connectors? Everyone will need a different cable length so some DIY will be necessary. An 8 pin JST PH connector is required for the VESC and I think I will use a 4 pin JST PH connector at the VeGa side. Only 4 wires (5V, GND, TX, RX) are needed. I could add the connectors to the kit, but I'm not sure about the wires. Would everyone be able to crimp their own wires? I could probably get pre-crimped wires and people can then extend them without crimping by cutting in the middle and soldering on an extension wire. Is that a good idea or am I overthinking this?
```

---
## \#96 Posted by: janpom Posted at: 2018-10-18T06:15:23.053Z Reads: 294

```
There are many displays available. I chose the 2.0" one because I liked the size and it's cheap. And it works. I suggest that we don't complicate things by trying to support other displays, at least for now. At the very least, the 2.2" one wouldn't fit into the enclosure that @mmaner and @moon are about to design for the 2.0". Also, I think the LED pin on the 2.2" would need to be connected to VCC while the corresponding N/C pin 2.0" does not connect to anything in the current PCB design.

Note that the 2.0" is also [available on Amazon](https://www.amazon.com/Display-176x220-ILI9225-Peripheral-Interface/dp/B07HF7WVST/).
```

---
## \#97 Posted by: janpom Posted at: 2018-10-18T07:26:38.678Z Reads: 292

```
I've just accidentally done some science. If you reverse polarity on the display you get the magic smoke. Tested for you. Now I have a new display to order. :frowning:
```

---
## \#98 Posted by: Skunk Posted at: 2018-10-18T07:28:18.136Z Reads: 295

```
:man_facepalming: :open_mouth: :dizzy_face:
```

---
## \#99 Posted by: mynamesmatt Posted at: 2018-10-18T07:41:43.047Z Reads: 308

```
you posted this yesterday. when's the group buy happening cmon fellas @mmaner @thisguyhere
lol. I really want one of these and i feel like it wouldn't be too difficult to design a pcb you can buy with all the parts so you can put it together yourself. An electronics store in here in australia does heaps of these solder-it-yourself kits. I think that'd be cool?
```

---
## \#100 Posted by: brenternet Posted at: 2018-10-18T08:08:33.496Z Reads: 303

```
And you would be incorrect 😄

I do live in England though.
```

---
## \#101 Posted by: Andy87 Posted at: 2018-10-18T08:29:04.156Z Reads: 302

```
could you please double check the new name...
It´s not DAVE...
you think VeGa will work non the less or people will refuse to
buy it as they think it is vegan food?
```

---
## \#102 Posted by: dareno Posted at: 2018-10-18T08:41:52.113Z Reads: 279

```
You've lived there far too long then.
```

---
## \#103 Posted by: Grozniy Posted at: 2018-10-18T09:30:35.674Z Reads: 279

```
@Minim might also have some input to incorporate the display above the baseplate
 https://www.electric-skateboard.builders/t/collaborative-design-of-a-x-truck-mount-thingy-with-give-a-way-for-fun/60237?u=grozniy
```

---
## \#104 Posted by: brenternet Posted at: 2018-10-18T11:43:09.299Z Reads: 286

```
I've discussed this with my extensive marketing team and they agree that Dave is still the best name for this device
```

---
## \#105 Posted by: akhlut Posted at: 2018-10-18T13:17:41.539Z Reads: 277

```
Schematic?
```

---
## \#106 Posted by: janpom Posted at: 2018-10-18T14:52:54.119Z Reads: 274

```
@akhlut [Here's](https://easyeda.com/honza.pomikalek/VESC-Gauge) the schematic and a draft of the PCB layout (the "PCB v0.1"). Any comments are welcome. My background is not in electronics. I'm a pure hobbyist so there's likely a lot of room for improvement in the design.
```

---
## \#107 Posted by: akhlut Posted at: 2018-10-18T15:03:07.199Z Reads: 277

```
Same.  I just like to play.
```

---
## \#108 Posted by: moon Posted at: 2018-10-19T01:33:26.691Z Reads: 283

```
Where can I find/buy/know what gaskets that will be good for this little project?
```

---
## \#109 Posted by: mmaner Posted at: 2018-10-19T01:38:01.174Z Reads: 284

```
I'm not sure yet, I haven't started yet, need measurements and it's likely to be a couple of weeks before the display and parts get to me. 

Once I have aRough XYZ values I can get an idea of what prr-made gaskets will for without much modification and then design the enclosure around that. 

It may be easier to make a change in the enclosure for a silicon bead instead. Still too early to tell.
```

---
## \#110 Posted by: Battosaii Posted at: 2018-10-19T01:53:59.577Z Reads: 283

```
Is the display available on Amazon? I don't mind paying a bit extra just so I don't have to order though a Chinese site and wait for shipping.
```

---
## \#111 Posted by: moon Posted at: 2018-10-19T01:56:13.781Z Reads: 281

```
https://www.amazon.com/Display-176x220-ILI9225-Peripheral-Interface/dp/B07HF7WVST/
```

---
## \#112 Posted by: Battosaii Posted at: 2018-10-19T01:57:36.793Z Reads: 273

```
I saw that one but I think it still comes from China so there is a long wait.
```

---
## \#113 Posted by: bsancken Posted at: 2018-10-19T01:57:48.005Z Reads: 274

```
Thats still weeks for shipping even though its on amazon...

*****
Ooops yah beat me to it!
```

---
## \#114 Posted by: moon Posted at: 2018-10-19T01:59:49.843Z Reads: 266

```
Oh didnt know that

I should have bought one from Taobao when I had the chance :persevere:
```

---
## \#115 Posted by: Battosaii Posted at: 2018-10-19T02:00:39.885Z Reads: 270

```
Found it with prime


HiLetgo 2.2" ILI9225 SPI Serial Port 176x220 TFT LCD Module with SD Socket Support 51/ARM/Arduino https://www.amazon.com/dp/B00LSG5HI0/ref=cm_sw_r_cp_apa_EQtYBbHMD4P7P

Edit I just noticed that link is the 2.2" display don't buy that one it's too big.
```

---
## \#116 Posted by: bsancken Posted at: 2018-10-19T02:01:33.509Z Reads: 268

```
Nope, already tried that, they flagged my post so I deleted it. Different screen/module!!
```

---
## \#117 Posted by: Battosaii Posted at: 2018-10-19T02:02:39.969Z Reads: 275

```
Yeah just noticed damn
```

---
## \#118 Posted by: lrdesigns Posted at: 2018-10-19T03:35:03.248Z Reads: 319

```
I was looking for some dimensions to get started on a case concept. I found [this.](https://github.com/Nkawu/TFT_22_ILI9225/tree/master/images) I assume this is accurate on the hole dimension and that the doughter PCB will have the same hole spacing? Apparently wrong, this is the 2.2" size.  

![image|594x432](upload://JizmA712twFP5d60uo5jXAeptC.jpeg) 

I went ahead and made a quick concept as small as I could make it. It uses a 3mm piece of Acrylic to cover the screen that should be epoxied to the case. Four M3 Socket heads hold it all together and compress an o-ring on the bottom for "water proof" ness. There is still a question about water proof buttons, for the communication cables I would just expoxy / hotglue where they come out the case. The bottom part I did not model yet.  The schematic from @janpom showed two buttons that's why there is two round holes on the side.  

Also I am sad to say its going to be too big to fit inside the truck bolt pattern. :roll_eyes:

![508|690x481](upload://a9XKkQ8IIIvCXBIFmFpSdDszqZM.jpeg) 

Bottom side where o-ring goes, then compress by bottom half part not shown. 

![509|690x481](upload://l2ydphOHFxNcajG4a5sG4D2dUtU.jpeg) 

PCB assembly. 

![511|690x481](upload://Abb6Ii1bMoeUJEm60jYXxUJ25Iy.jpeg) 

Cross section. 

![Cross%20Section|690x290](upload://ec9H55O3LmCMQNPTavuRsC9aGkO.jpeg)

All of the vertical dimensions for the PCB's are just a guess at this point.

Anyone know of some really small waterproof buttons?

*Thought. :thinking: Maybe the case does not need to be two parts with o-ring. Once you confirm it works, fully pot the inside with epoxy and use the 4 bolts to attach it to the deck. Well that is one way to get it done! :thinking: Actually you need to disassemble to re-program it if there is an update to the firmware, so fully potting it would not be good idea.
```

---
## \#119 Posted by: moon Posted at: 2018-10-19T03:38:06.116Z Reads: 281

```
Make it landscape? Thats what I am going to do if making it landscape is possible @janpom

I am probably going to have mine cnc aluminium - probably cost more than the electronics itself lol
```

---
## \#120 Posted by: Jc06505n Posted at: 2018-10-19T03:51:01.705Z Reads: 286

```
Please make it step-onable for us shortboarder 🙏🏾
```

---
## \#121 Posted by: Skunk Posted at: 2018-10-19T03:55:32.163Z Reads: 287

```
I think a different design that acts as a foot stop would be dope for my short board
```

---
## \#122 Posted by: janpom Posted at: 2018-10-19T07:03:31.820Z Reads: 305

```
That looks great, @lrdesigns! Unfortunately, the dimensions that you have are wrong. Those are probably for the 2.2" display. For the 2.0", the PCB outline dimensions are 62mm x 38mm.

Also, I'd like to have 3 buttons. Currently only 1 is used (for resetting the trip distance), but looking forward it would be nice to have more available so that menus can be implemented for basic config options.

I'm about to order the PCBs, but I'm still hesitating about the exact positions of the connectors, mainly the 6 pin header for the USB-UART.

Here's the layout that I currently have:

![56|690x441](upload://9EigS6NtwA6dB3f7L4X24EI2w5k.png) 

The DEBUG and VESC holes are meant for right angle JST PH connectors. However, they don't need to be soldered on. The DEBUG is only for development. And after discussing with @mmaner, we concluded that the cable leading to VESC would be best soldered directly on the bottom of the PCB so that it can be easily routed through the deck. No need for a connector.

So only the position of the USB-UART is critical. [6 pin right angle female headers](https://www.aliexpress.com/item/2-54mm-R-A-Single-Row-Female-2-40P-PCB-Board-Right-angle-Pin-Header-socket/32908650183.html?spm=a2g0s.9042311.0.0.3da24c4dikcoLF) will go there. This is for updating the FW. With the current position, the header would stick about 1mm out of the PCB and I'm not sure if that's a good thing.

I can see options there. (1) The header is accessible through the enclosure. Then it should probably stick out of the PCB more than 1mm. What about splash resistance then, though? Would there be some protective cover? Sounds complicated.  (2) You need to take the PCB out of the enclosure for programming. Annoying, but probably OK since it wouldn't be done too often. Then it's best if the header is flush with the PCB edge. Any thoughts on that?

BTW, since yesterday I have a fried display that I can send out to anyone interested. It may be handy for designing the enclosure.
```

---
## \#123 Posted by: janpom Posted at: 2018-10-19T07:07:50.770Z Reads: 265

```
[quote="moon, post:119, topic:71509"]
Make it landscape?
[/quote]

Yes, it's possible. We just need to figure out the layout. I found it much easier to lay things out in the portrait orientation.
```

---
## \#124 Posted by: lrdesigns Posted at: 2018-10-19T07:13:13.154Z Reads: 268

```
[quote="janpom, post:122, topic:71509"]
(2) You need to take the PCB out of the enclosure for programming.
[/quote]

I vote for this option. If you want to program it with the case on and don't care about water resistance you can just have a hole on the side large enough for the programer to fit?
```

---
## \#125 Posted by: janpom Posted at: 2018-10-19T07:20:26.931Z Reads: 272

```
Yes, I too think that's better. Let's keep it simple and we'll call it version 1. We can always iterate to make it more user friendly.

@mmaner, @moon: What do you guys think?
```

---
## \#126 Posted by: lrdesigns Posted at: 2018-10-19T10:13:13.625Z Reads: 296

```
I acidently designed a 2.2 inch enclosure if any one wants that? 

![image|666x500](upload://kamNW4FqoEsJVYH5Aj8qODYCQPS.jpeg) ![image|375x500](upload://cdcf6IGZyigqRFdCVYL71Y8ZDXV.jpeg) ![image|375x500](upload://ey0qbpMbjZDtvbp95YzY8wywenD.jpeg)
```

---
## \#127 Posted by: janpom Posted at: 2018-10-19T11:39:43.096Z Reads: 272

```
@lrdesigns That's neat. If I send you the dimensions for the 2.0" display, would you be able to adjust the model for it and share the file? I could then ask a friend to 3D print it for me and test the fit.
```

---
## \#128 Posted by: lrdesigns Posted at: 2018-10-19T11:43:18.017Z Reads: 270

```
Sure. The benefits of parametric modeling.
```

---
## \#129 Posted by: janpom Posted at: 2018-10-19T13:12:48.304Z Reads: 303

```
@lrdesigns, I hope this helps:
![ILI9225_TFT_dimensions|645x500](upload://28XByFSduuYMCuYhKqk19ZN8E55.jpeg) 

Also, the distance between the surface of the PCB and the surface of the display is 2.3mm and the pins on the left hand side come about 1mm above the surface of the PCB, so there's only ~1.3mm between the top of the pins and the surface of the display.

The center of all holes is 2.5mm from the two nearest edges (not apparent from the diagram for the holes at the right hand side). 

Photos:

![IMG_1424|690x381](upload://sSPBUhlDsfHZYjjwSO2B9wBaHcr.jpeg) 

![IMG_1425|627x500](upload://vcoZeA1nqn3uIE15CN0zVoKsr8B.jpeg)
```

---
## \#130 Posted by: brenternet Posted at: 2018-10-19T14:07:52.381Z Reads: 281

```
I love all the cooperation going into Dave, this is awesome.

Could someone make a bamboo enclosure please? All this aluminium and plastic is great but I'd totally fork out for a nice bamboo enclosure. Only have to buy the enclosure once right?
```

---
## \#131 Posted by: moon Posted at: 2018-10-19T14:08:36.366Z Reads: 273

```
Anything can be done :smiley:

I am just trying to figure out viewing angles atm
```

---
## \#133 Posted by: brenternet Posted at: 2018-10-19T14:11:47.002Z Reads: 272

```
Off topic, flagged. (Not really btw, when it actually gets flagged I don't want you to resent me)
```

---
## \#134 Posted by: Skunk Posted at: 2018-10-19T14:12:35.953Z Reads: 263

```
To late lol
```

---
## \#136 Posted by: Grozniy Posted at: 2018-10-19T14:21:34.647Z Reads: 256

```
They are on topic in the Secret Santa 2018 thread :stuck_out_tongue_closed_eyes:
```

---
## \#137 Posted by: moon Posted at: 2018-10-19T14:24:44.291Z Reads: 262

```
Could you try and modify it to make it so that that the screen is angled to like maybe 30 degrees (random number) so it would be easier to read the display when riding the board. 

Also has anyone thought that this would be a great "dashboard" maybe add a on/off switch and a charge port?
```

---
## \#138 Posted by: lrdesigns Posted at: 2018-10-19T14:26:55.548Z Reads: 279

```
[quote="moon, post:137, topic:71509"]
Could you try and modify it to make it so that that the screen is angled
[/quote] 

that was actually my first idea. But then I decided to try a minimum volume design first. Plus faster to model this way.
```

---
## \#139 Posted by: Grozniy Posted at: 2018-10-19T14:29:08.868Z Reads: 297

```
So something like this?
![g0KwHUE|660x337](upload://uvujxunt2zc2MKix1pgfH0BBsie.jpeg) 
Actually it would be possible to print a smartphone mount and attach to the trucks bolts. This way one could choose whatever app desired
Edit:
![smartphone-holder-new|500x500](upload://uj2mYMFr8VhSKwpP3qmVDRqIvB4.png)
```

---
## \#140 Posted by: moon Posted at: 2018-10-19T14:30:43.220Z Reads: 284

```
That wouldnt be hard but you would probably need to design it for a particular phone first

Oh lol. Now you look like an uber driver
```

---
## \#141 Posted by: Skunk Posted at: 2018-10-19T14:33:59.288Z Reads: 280

```
My luck i would be getting calls every time i ride or it would be dead.  Built in and powered by the board would be preferred for me at least.
```

---
## \#142 Posted by: Jc06505n Posted at: 2018-10-19T14:37:22.253Z Reads: 288

```
[quote="Grozniy, post:139, topic:71509"]
Actually it would be possible to print a smartphone mount and attach to the trucks bolts. This way one could choose whatever app desired
[/quote]


Sounds like a really fun way to lose a phone. While im all for cool things like this and the VEGA (i'm, even getting a proton myself), but I'm really worried about people not being responsible and looking down at the stuff at the wrong time (like looking own at 30mph). Dashboards on cars work because they're within your field of view and allow you to keep looking straight. Stuff like this should be considered more of a control panel rather than speedometer. Stuff like that should left to things like Helmets or Ar glasses, things that won't force you to snatch your eyes off the road for a second.
```

---
## \#143 Posted by: Skunk Posted at: 2018-10-19T14:42:14.143Z Reads: 283

```
We also don't have rearview mirrors or side mirrors. 
Quick glances are part of riding safety. 
Yeah don't stare at your feet,  but unless you're a complete nob i don't see this affecting safety.
```

---
## \#144 Posted by: janpom Posted at: 2018-10-19T18:58:20.582Z Reads: 286

```
[quote="Jc06505n, post:142, topic:71509"]
While im all for cool things like this and the VEGA (i’m, even getting a proton myself), but I’m really worried about people not being responsible and looking down at the stuff at the wrong time (like looking own at 30mph).
[/quote]

Yes, it's a good point. My main motivation for making the gadget was to get the odometer and battery monitor. I don't care that much about the speed and I only added it as a bonus. I'm already thinking of VeGa lite with a smaller display (maybe one of the 128x32 I2C OLEDs) that would only give you the battery status and traveled distance. One that would be small enough to mount on the side of a battery/ESC enclosure. First things first though.
```

---
## \#145 Posted by: spesh Posted at: 2018-10-19T22:49:22.330Z Reads: 267

```
If you do call this Dave I'll buy one.
```

---
## \#146 Posted by: mmaner Posted at: 2018-10-20T01:32:28.570Z Reads: 285

```
[quote="janpom, post:125, topic:71509"]
@mmaner, @moon: What do you guys think?
[/quote]

I agree, making ports waterproof is almost impossible.
```

---
## \#147 Posted by: pixelsilva Posted at: 2018-10-20T06:09:13.080Z Reads: 305

```
...and you will design my carbon footstop with the integrated casing (on top) for the **VeGa** batt, odometer, speedometer monitor!

![313_Footstop_2009_alpha_011|690x457](upload://ppxkSdbIFEWRT2LO0Me7LiH4zz6.jpg)

:point_up_2:
.
.
:point_down:

![image|690x481](upload://4simZFZqal8N9wAxDgkMM7mnm43.jpeg)
```

---
## \#148 Posted by: janpom Posted at: 2018-10-21T18:28:31.728Z Reads: 297

```
I realized we don't actually need any ports on the case and we can still update FW without taking the gadget out of the case. Programming as well as VESC communication is done over UART, so the two connectors connect to the same pins (and there's an extra reset pin for programming). We can simply solder a 5 conductor cable to the board and Y-split 4 of the wires. Here's how it looks:

![IMG_1427|664x500](upload://1Mo7RHN6PC7FMR099BDEck821PT.jpeg) 

Works like a charm.

The two JSTs go to VESC (it's supposed to be a single 8 pin JST that I currently don't have) and the dupont connector goes to the UART-USB adapter for FW update. (White = green. Don't ask. :smile: )

A simpler and cleaner alternative would be without the Y split. Instead, connect 4 wires to the 8 pin JST and the fifth reset wire to a 1 pin dupont. Then make an 8 pin JST to 4 pin dupont adapter and connect the 4+1 duponts to the USB-UART adapter for programming. Next time I'll do it that way.
```

---
## \#149 Posted by: brenternet Posted at: 2018-10-21T18:42:34.078Z Reads: 271

```
I think you and I make an overwhelming majority. I feel like a vote is needed.
```

---
## \#150 Posted by: brenternet Posted at: 2018-10-21T18:46:55.862Z Reads: 272

```
[quote="janpom, post:144, topic:71509"]
I’m already thinking of VeGa lite with a smaller display (maybe one of the 128x32 I2C OLEDs) that would only give you the battery status and traveled distance. One that would be small enough to mount on the side of a battery/ESC enclosure. First things first though.
[/quote]

If you did this perhaps all of the information could be cycled through a single button. That way a very small screen could be used and you could select what is important to you at the time.

I would probably have battery up but if you wanted to monitor you speed you could just push the button and get the speedo up. When you stop you could quickly cycle through odometer, voltage and the other options for that info if you need it.

I'd be more interested in that sort of display than a fat one with everything on.
```

---
## \#151 Posted by: mmaner Posted at: 2018-10-21T18:49:40.940Z Reads: 263

```
[quote="janpom, post:148, topic:71509"]
We can simply solder a 5 conductor cable to the board and Y-split 4 of the wires.
[/quote]

That is awesome!
```

---
## \#152 Posted by: sami Posted at: 2018-10-21T19:01:32.551Z Reads: 267

```
This thing looks AWSOME.... I can't wait to buy it/build it
```

---
## \#153 Posted by: janpom Posted at: 2018-10-22T06:18:08.328Z Reads: 296

```
I made a very crude enclosure from cardboard and tape, so that I can better test VeGa (aka Dave) while riding. Before, it would just be sitting in my battery box => no reading while riding.

It's not pretty but I think it will do.

![IMG_1430|666x500](upload://4ThzxOf5zqkMMC7Zj4SgAZGXjvV.jpeg) 

![DSC01614|690x460](upload://q65Rv41WSl27m6t46oPU7ASd7W1.jpeg)

![DSC01615|690x460](upload://4Ma9dnKmNSGAv3RXrYuTqqI7Pf2.jpeg)
```

---
## \#154 Posted by: Sebike Posted at: 2018-10-22T06:41:32.628Z Reads: 289

```
Only thing that's missing is

https://static1.jamaran.ir/servev2/YTgyYjY5ODJl/PBG64w6wfqErp47D1W9w0Jpfa8fpMiBcptkcLd6IQr4,/.jpg

Please! :smile:
```

---
## \#155 Posted by: totalgeek9224 Posted at: 2018-10-22T07:41:26.089Z Reads: 285

```
**THIS** is what is needed.
no one will care that you have a little screen that shows you VESC info, but watch people peer in curiosity when you're at work playing snake on your skateboard
```

---
## \#156 Posted by: lrdesigns Posted at: 2018-10-22T08:09:38.691Z Reads: 282

```
But you have to steer the snake by leaning the board! :rofl:
```

---
## \#157 Posted by: Vanarian Posted at: 2018-10-22T09:27:52.721Z Reads: 276

```
I'm totally up for it if you keep Dave haha sick little screen for data, top mounted it will look like future despite low res!
```

---
## \#158 Posted by: brenternet Posted at: 2018-10-22T09:50:34.028Z Reads: 273

```
[quote="janpom, post:153, topic:71509"]
test VeGa (aka Dave)
[/quote]

Yeaaaaaah. He's cracking boys. Dave is alive.

Your little mock up came out excellent. How do you think it'll hold up component wise to 100 miles of road shudder?
```

---
## \#159 Posted by: dareno Posted at: 2018-10-22T10:26:36.390Z Reads: 275

```
told you it was an english thing.

[quote="spesh, post:145, topic:71509, full:true"]
If you do call this Dave I’ll buy one.
[/quote]
```

---
## \#160 Posted by: janpom Posted at: 2018-10-22T12:35:07.312Z Reads: 272

```
VeGa is on GitHub: https://github.com/janpom/vega
```

---
## \#161 Posted by: sami Posted at: 2018-10-22T13:30:25.446Z Reads: 274

```
> The device is also known (or, rather, incorrectly referred to) as [Dave](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/8?u=janpom) by [some people](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/130?u=janpom), which is pretty annoying, especially since it seems to [begin to catch](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/145?u=janpom) and having to rebrand is no fun!

:rofl::rofl::rofl: @brenternet @spesh
```

---
## \#162 Posted by: brenternet Posted at: 2018-10-22T14:08:17.811Z Reads: 274

```
Technically the real name Dave was discussed before the assumed name vega. Which means an unnecessary re-brand has already happened
```

---
## \#163 Posted by: Silverline Posted at: 2018-10-22T15:26:33.475Z Reads: 260

```
Are you planning selling these as a complete kit ?? I would 100% be up for at least two.....
```

---
## \#164 Posted by: spesh Posted at: 2018-10-22T15:36:18.454Z Reads: 252

```
Pfft.. I'm welsh :p
```

---
## \#165 Posted by: totalgeek9224 Posted at: 2018-10-22T15:37:51.437Z Reads: 251

```
I mean, I think the right name is clear...
```

---
## \#166 Posted by: janpom Posted at: 2018-10-22T17:33:13.426Z Reads: 262

```
[quote="brenternet, post:162, topic:71509, full:true"]
Technically the real name Dave was discussed before the assumed name vega. Which means an unnecessary re-brand has already happened
[/quote]

I can't agree with that. The proposed name Dave was discussed and [rejected](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/55?u=janpom) by the executive board. As such, it has never come into official use and thus there can be no mention of any previous re-branding.
```

---
## \#167 Posted by: janpom Posted at: 2018-10-22T18:17:24.750Z Reads: 267

```
[quote="brenternet, post:158, topic:71509"]
How do you think it’ll hold up component wise to 100 miles of road shudder?
[/quote]

I'm not sure about the display. Other than that, it shouldn't be a problem as long as all the components are properly soldered. There are no sensitive parts. If your ESC survives the beating then so should Dave (that's just using the language of your tribe; it doesn't mean anything :smile:).
```

---
## \#168 Posted by: bsancken Posted at: 2018-10-22T18:19:20.557Z Reads: 254

```
[quote="janpom, post:167, topic:71509, full:true"]
[quote="brenternet, post:158, topic:71509"]
How do you think it’ll hold up component wise to 100 miles of road shudder?
[/quote]

I'm not sure about the display. Other than that, it shouldn't be a problem as long as all the components are properly soldered. There are no sensitive parts. If your ESC survives the beating then so should Dave 
[/quote]
Oh look! Called it Dave! Its official!
```

---
## \#169 Posted by: Jc06505n Posted at: 2018-10-22T18:21:51.060Z Reads: 249

```
[quote="janpom, post:167, topic:71509"]
that’s just using the language of your tribe; it doesn’t mean anything :smile:).
[/quote]


No fake news
```

---
## \#170 Posted by: janpom Posted at: 2018-10-22T18:24:12.256Z Reads: 271

```
[quote="Silverline, post:163, topic:71509, full:true"]
Are you planning selling these as a complete kit ?? I would 100% be up for at least two…
[/quote]

I could definitely make a few complete kits. However, I'm thinking of the first batch as a beta testing. I prefer to send the DIY kits to people with some knowledge of electronics and some experience with Arduino, i.e. people who will know what they are doing when assembling the kit (rather than just blindly following the assembly instructions), who won't damage their computer or their ESC by doing something stupid, and who are not afraid to experience and address problems. At this point, the gadget definitely can't be considered a well tested product. If you want something finished, I suggest that you wait a bit.
```

---
## \#171 Posted by: brenternet Posted at: 2018-10-22T19:07:07.885Z Reads: 272

```
Honestly, a solid $10 product with these features that's easy to fit around your build is amazing, you're doing good work here.
```

---
## \#172 Posted by: Vanarian Posted at: 2018-10-22T19:31:26.798Z Reads: 279

```
https://media.giphy.com/media/5By7NydSzyxIQ/giphy.gif
```

---
## \#173 Posted by: janpom Posted at: 2018-10-22T19:35:42.722Z Reads: 293

```
Today, I made a test ride with VeGa mounted to the front of my board. We had a sunny day so that was a perfect opportunity to test the display readability on sunlight. Here are my impressions:

- I mounted the gadget on the left side since it doesn't fit between the truck bolts. But it actually makes sense to have it more to the left since it's closer to the normal field of view (for goofy riders of course).
- The white on black is readable even or direct sunlight. I could always read the speed by taking a quick glance on the display.
- Taking quick glances on the display here and there doesn't feel risky at all if done at the right moment (no people, cars, obstacles around).
- The battery indicator (green to red squares) is easy to read. I like it a lot.
- The speed indicator (blue squares) is much harder to read. Blue on black doesn't work very well. Plus, I never actually even tried to look at it. I just read the number. So while it makes the design fancy it's not really useful.
- The numbers other than speed are a bit too small to be read easily while riding even out of direct sunlight. I had to at least slow down to read the voltage or trip distance. Leading zeroes make things worse. I have to get rid of those.
- I have a piece of matte foil covering the display. I'm not sure how much it affects the display readability, but it definitely doesn't improve it.
- Battery capacity tracking seems to work really well. The discharged Ah correlated nicely with the battery voltage. I arrived with near empty batteries -- 3.6 V per cell (LiPo) and with 1858 out of 8000 mAh remaining, so that's ~77% discharged when 80% is generally accepted as the usable battery capacity.
- I compared the distance and speed with GPS. Both were about 10% more than measured by GPS. I believe I just need to adjust my wheel size / gear ratio settings. I actually just measured my 8" MBS tire circumference and it's ~604mm when I had it set to 638mm (8 * 2.54 * PI), which partially explains the difference.

Overall, I'm very happy with the gadget. It's really nice that at any moment you have the distance, battery voltage and discharged mAh available since those combined give you a very good idea about the remaining range.

![IMG_1431|666x500](upload://isqOF6iN2DhAjZH6R1cFZ5ASdRC.jpeg) 

(never mind the filled blue squares; that's a bug I injected when cleaning up the code today; easy fix)

![PNG|281x500](upload://t3RYDHKLxwsURhYXejCz2ygsSBX.jpeg)
```

---
## \#174 Posted by: Kug3lis Posted at: 2018-10-22T20:01:08.156Z Reads: 281

```
I really like the idea of this stuff, and spent some time modifying one of my schematics which I have to utilise VeGa on ATmega32u4 which has USB integrated and make it as small as possible :)

Will start on PCB probably some time this week :) I have already forked the source and done some minor code changes. After I get lcd and test them I going to open PR.  It will help with the pain to configure it :) 

Probably will also add some headers for addressable RGBW strip and etc stuff (will require separate 5V power supply your DRV probably will die if you connect to it :laughing: ) 

![image|690x480](upload://o1o6p5ob17C5wyIRDx9JgjVwb75.png)
```

---
## \#175 Posted by: Kug3lis Posted at: 2018-10-22T20:12:10.013Z Reads: 258

```
Also had some thoughts maybe making into X plate with it... But looked up some water resistant small push buttons so nothing much exists... If anyone knows smaller than 12mm buttons send me the links :)
```

---
## \#176 Posted by: janpom Posted at: 2018-10-22T20:13:17.679Z Reads: 253

```
Cool! It's great to have an electronics guru on board. I'm looking forward to your updates.
```

---
## \#177 Posted by: Kug3lis Posted at: 2018-10-22T20:13:51.515Z Reads: 254

```
It's nothing special base circuit is like a standard for many arduino based boards :)
```

---
## \#178 Posted by: Holyman92 Posted at: 2018-10-22T20:30:50.378Z Reads: 251

```
can we still get these?
```

---
## \#179 Posted by: DilatedPupils Posted at: 2018-10-22T20:40:19.715Z Reads: 276

```
[quote="janpom, post:173, topic:71509"]
* The speed indicator (blue squares) is much harder to read. Blue on black doesn’t work very well. Plus, I never actually even tried to look at it. I just read the number. So while it makes the design fancy it’s not really useful.
* The numbers other than speed are a bit too small to be read easily while riding
[/quote]


What about eliminating the blue squares to make room for the other numbers to be bigger? Like the battery voltage.
```

---
## \#180 Posted by: Kug3lis Posted at: 2018-10-22T20:58:04.301Z Reads: 275

```
Quick mashup with KiCad, modified schematic added FRAM so you could store and write as my time as you want to it :)

![image|690x487](upload://3oJgZkvjpTtM7U5V3gm6Jm0X8Fg.png)
```

---
## \#181 Posted by: janpom Posted at: 2018-10-22T21:03:52.429Z Reads: 263

```
SMD components. That's cheating! :smile:

It's certainly nice to have a USB, so that you don't need an adapter. On the other hand, if you do use the adapter, then you don't need any ports. You just solder a 5 conductor cable to the PCB that you can use for both VESC and for programming. That makes designing the enclosure easier.
```

---
## \#182 Posted by: Kug3lis Posted at: 2018-10-22T21:04:49.936Z Reads: 261

```
It's just component to have a holes :) The same with 3 x button headers :slight_smile:

Also USB works with Arduino so you don't need any cables or etc :)
```

---
## \#183 Posted by: janpom Posted at: 2018-10-22T21:07:31.238Z Reads: 261

```
[quote="Kug3lis, post:182, topic:71509"]
It’s just component to have a holes :slight_smile: The same with 3 x button headers :slight_smile:
[/quote]

I see. I was actually wondering what those pins are for.

[quote="Kug3lis, post:182, topic:71509"]
Also USB works with Arduino so you don’t need any cables or etc :slight_smile:
[/quote]

Yeah sure, but you need to be able to access the USB connector.
```

---
## \#184 Posted by: Kug3lis Posted at: 2018-10-22T21:08:13.724Z Reads: 249

```
Cutout in the enclosure with plug for it :) We did same for vesc 4.12 enclosure :) Was working wonderfuly :)
```

---
## \#185 Posted by: janpom Posted at: 2018-10-22T21:10:34.179Z Reads: 248

```
[quote="DilatedPupils, post:179, topic:71509"]
What about eliminating the blue squares to make room for the other numbers to be bigger? Like the battery voltage.
[/quote]

I still have a weak spot for the blue squares. They may not be very useful, but I still like them. In fact, I don't think vertical space is a problem. I'd rather hit the horizontal space limitations first when trying to make the numbers bigger. I think we need a different font. The simple one used for the speed could work well.
```

---
## \#186 Posted by: janpom Posted at: 2018-10-22T21:12:26.481Z Reads: 242

```
Can you make it such that it's water resistant? The VESC is typically sitting in the battery enclosure so that's different.
```

---
## \#187 Posted by: brenternet Posted at: 2018-10-23T00:31:01.979Z Reads: 237

```
I believe he's referring to a top mount case for mtb/trampa decks. If so they are pretty exposed and taje a beating off road
```

---
## \#188 Posted by: mynamesmatt Posted at: 2018-10-23T00:42:17.002Z Reads: 241

```
i really. really want one of these
```

---
## \#189 Posted by: lrdesigns Posted at: 2018-10-23T01:51:47.069Z Reads: 247

```
@janpom can your code run on different screen sizes? Like 1.5 2.0 2.2 if the screen is same design like the 2.0 and 2.2 above that have the same model name? Or is it specific to the pixel count of the screen. Sorry I know nothing about how arduino outputs to screens.
```

---
## \#190 Posted by: AreaKruzer Posted at: 2018-10-23T05:00:36.181Z Reads: 241

```
the important thing for the screen to arduino is probably just the pixel count. the sizes of the screen dont really matter.
```

---
## \#191 Posted by: janpom Posted at: 2018-10-23T06:04:30.776Z Reads: 258

```
[quote="lrdesigns, post:189, topic:71509"]
Can your code run on different screen sizes?
[/quote]

Larger ILI9225 displays should work out of the box, but the pixel count is important. The picture would be aligned top left and there would be some empty space on the right and at the bottom. Smaller displays wouldn't work. At best, the picture would be trimmed.

However, the code is fairly modular and the display routines are decoupled from the rest of the code in the [vega_display](https://github.com/janpom/vega/blob/master/vega_display.h) module. Supporting any other display (even other than ILI9225) is a matter of re-implementing those 12 routines. Supporting larger/smaller ILI9225 displays then requires only relatively small code adjustments.
```

---
## \#192 Posted by: janpom Posted at: 2018-10-23T06:05:55.479Z Reads: 255

```
@lrdesigns Any progress on adjusting your enclosure for the 2.0" display? I would love to try it out.
```

---
## \#193 Posted by: janpom Posted at: 2018-10-23T06:47:47.379Z Reads: 284

```
Updating FW without even taking it off the board. :sunglasses:

![DSC01617|564x500](upload://3xNQ8i1KAlxE30PZDhfdOVuRnGZ.jpeg)
 
![DSC01618|690x460](upload://plXfrTZDzPLFcsDgvr8C8U1Ho5o.jpeg)
```

---
## \#194 Posted by: lrdesigns Posted at: 2018-10-23T06:51:07.922Z Reads: 283

```
[quote="janpom, post:192, topic:71509"]
Any progress on adjusting your enclosure for the 2.0" display?
[/quote]

Let me grab some :coffee: and have a look. Just needed to get a few free minutes at work. I guess I need to upload to thingiverse so you can download it?
```

---
## \#195 Posted by: janpom Posted at: 2018-10-23T06:53:56.452Z Reads: 276

```
Cool! Re sharing the files, do whatever works best for you. I'm flexible.
```

---
## \#196 Posted by: lrdesigns Posted at: 2018-10-23T07:53:40.823Z Reads: 279

```
OK I updated it based on the 2.0" drawing you provided. I hope it fits, not 100% sure it will yet. I removed the side holes, you can just drill some holes where its most convenient.  Modeled the bottom part now too. 

I don't suggest everyone download it yet as it has not been test fitted. But the 3D is [here.](https://www.thingiverse.com/thing:3171000/files)

![image|661x500](upload://rrsel8UnONEc3abUQmOCnPQH5xg.jpeg) 

![image|690x299](upload://cqpg4Q1VlNScFlVFwRvwThzJger.png) 

![image|689x500](upload://9RgGbAdvL8SGDQxMiuul7g85GSw.png)
```

---
## \#197 Posted by: janpom Posted at: 2018-10-23T08:27:18.633Z Reads: 265

```
Great, thanks a lot! I'll ask a friend to print it for me and will get some acrylic in the meantime. Can you please tell me the dimensions of the nuts and bolts?

I'm thinking that maybe the bottom plate could have the deck mounting holes inside rather than outside. You would mount the bottom plate to the deck first and only then cover it and secure with bolts. Anyway, the current is great for a test print and I can always do some cutting and drilling on it.
```

---
## \#198 Posted by: lrdesigns Posted at: 2018-10-23T08:48:21.589Z Reads: 277

```
M3 Socket head, 25mm long. To be used with nylock nuts. There is an issue though with 25mm they stick out a little and 20mm is too short. I need to adjust the design so it fits a standard size.

[quote="janpom, post:197, topic:71509"]
I’m thinking that maybe the bottom plate could have the deck mounting holes inside rather than outside.
[/quote]

Actually that is a good idea. :+1: I put two M4 counter sunk holes on the inside for direct mounting to the deck. I updated thingieverse. 

![image|597x500](upload://uB5KGRHyPkcpsBYIkXW5C1JQRrd.png)

![image|690x330](upload://4RCcgOybpdZ9N3RTkyDinAEjVfe.png)
```

---
## \#199 Posted by: pixelsilva Posted at: 2018-10-23T09:57:48.990Z Reads: 272

```
Wondering, why the enclosure lays flat? why the enclosure design doesn't count the fact that the rider will be positioned away on a diagonal visual posture, and the horizontal positioned screen (over the front truck plate) will not facilitate an easy read.

![New%20Project(3)|690x487](upload://1qUo5tZnDJvCNst4RPRI4qAj57j.jpeg)

Why not a slanted design? An enclosure with diagonal profile.... :point_up_2:
```

---
## \#200 Posted by: amazingdave Posted at: 2018-10-23T10:41:01.848Z Reads: 260

```
How far apart can the 2 pcb’s be? I’m not a fan of the chunky look, I’d like to have a slim display with the brains elsewhere if possible...
```

---
## \#201 Posted by: Andy87 Posted at: 2018-10-23T10:53:06.379Z Reads: 259

```
why not to safe the falt designe for all us who have a mountenboard and just use angled riser for those who want to mount it with an angle.
It´s even more easy to print and exchange it to different grades.
```

---
## \#202 Posted by: Skunk Posted at: 2018-10-23T10:53:44.738Z Reads: 254

```
[quote="amazingdave, post:200, topic:71509, full:true"]
How far apart can the 2 pcb’s be? I’m not a fan of the chunky look, I’d like to have a slim display with the brains elsewhere if possible…
[/quote]

This. I'd still use it either way. But slim would be nice
```

---
## \#203 Posted by: brenternet Posted at: 2018-10-23T11:43:51.333Z Reads: 250

```
+1 

Either screen slim or as I said before a much smaller screen with a button to cycle through options. I can't speak for others but I don't personally need to see all of the information all of the time.
```

---
## \#204 Posted by: lrdesigns Posted at: 2018-10-23T12:04:33.485Z Reads: 256

```
I made it flat just for speed of modeling. Didnt have much time between other jobs to work on it. Plus it makes even larger. Longer print time.  

@Andy87 this is genius.  
[quote="Andy87, post:201, topic:71509, full:true"]
why not have the flat design for all us who have a mountenboards and just use angled riser for those who want to mount it with an angle.
It´s even more easy to print and exchange it to different angles.
[/quote]

As to thickness. It could be much slimmer if you made it less robust and are willing to solder the two boards together. Soldering could get you maybe 3-4mm less. Change the screen protector from 3mm to 2mm/1mm/0mm. Don’t use a bottom plate and just bolt the top enclosure directly to board.

Also its better for the first sample to be too big then too small, once I have all the parts in hand it will be easier to shrink it down. At the moment it's just an educated guess.
```

---
## \#205 Posted by: janpom Posted at: 2018-10-23T15:09:23.874Z Reads: 234

```
You would have many wires to route. 8 for the display and another 1 for a button (another 3 if there are 3 buttons). So that's 9 to 11 wires in total.
```

---
## \#206 Posted by: Itsmedant Posted at: 2018-10-23T15:13:08.777Z Reads: 241

```
Just read through this thread, this thing is awesome!

I am super interested in getting one or helping in any way!
```

---
## \#207 Posted by: janpom Posted at: 2018-10-23T15:17:07.585Z Reads: 246

```
I purchased some 2mm plexiglass today (they only had 2mm and 4mm in the hardware store) and it seems plenty sturdy. I wouldn't be afraid to go even thinner for that small area. I currently have like 0.1mm foil. :smile:
```

---
## \#208 Posted by: amazingdave Posted at: 2018-10-23T15:41:23.614Z Reads: 287

```
A ribbon cable will sort that. I only need it to 15cm away....
```

---
## \#209 Posted by: janpom Posted at: 2018-10-23T17:58:19.281Z Reads: 300

```
Sure, I think that separating the two PCBs is a valid option. But then you actually don't need any VeGa PCB. Just buy the display, buttons, and Arduino Nano. Build an enclosure for the display and buttons, route cables to the Arduino ([here's](https://github.com/janpom/vega/blob/master/davega_display.cpp#L24) the pinout for the display and [here's](https://github.com/janpom/vega/blob/master/davega.ino#L121) the button pin -- you can change the latter). Connect VESC to Arduino. Upload the VeGa FW to the Arduino and you're done.

![12|690x368](upload://kNSsf7mMcpJo5EuQ8upOZ89v1g7.png)
```

---
## \#210 Posted by: janpom Posted at: 2018-10-24T09:08:35.054Z Reads: 318

```
I changed the fonts and made the numbers taller. This is a better utilization of the vertical space and should improve readability.

Before:
![IMG_1439|427x499](upload://rg6OwkHV9QWoI7SxD5OJJyh627P.jpeg)

After:
 ![IMG_1441|428x500](upload://4JZb2ZcJerUeoLbvWPgXE79BoHl.jpeg) 

With maximal values (except for voltage):
![IMG_1440|429x500](upload://2iNlwG2SgDqjWiCgChAbSZU34IF.jpeg)
```

---
## \#211 Posted by: janpom Posted at: 2018-10-25T10:07:40.985Z Reads: 304

```
PCBs arrived! That was super fast. I ordered them last Friday evening and they arrived today morning. That's less than 6 days for manufacturing and shipping from China! I'm impressed with JLCPCB. Also the quality looks pretty decent as fair as I can tell.

![IMG_1442|666x500](upload://zWv8YHmYydAtCgKXYp6WnwbePRV.jpeg) 

I had a few professionally re-branded specifically for @brenternet and @spesh. These will obviously be waaaaay more expensive since the re-branding costs need to be amortized!  

![IMG_1443|666x500](upload://80i7Cy8B6ARXGTkeZS8wdb71y2y.jpeg) 

The alignment with the display is near perfect. Unfortunately, the mounting holes are too small for M3 screws, but that's easily fixed with a bit of drilling.

![IMG_1444|690x497](upload://zlhIkKSBYxGG7iINLiZ1c98mzoo.jpeg) 

Here's how thick it will be assembled. It's 13mm (including the solder joins underneath the PCB).

![IMG_1445|690x229](upload://dNaF2w7wrDXrRDxb50DC9DZUvwo.jpeg) 

I haven't assembled any yet. Will do it now. I hope all works. :crossed_fingers:
```

---
## \#212 Posted by: Andy87 Posted at: 2018-10-25T10:13:55.677Z Reads: 266

```
so quick!  looks good!
```

---
## \#213 Posted by: brenternet Posted at: 2018-10-25T10:55:13.692Z Reads: 272

```
This is great :smiley:

I think I speak for the masses here, and if I don't my confidence should convince you otherwise (this is how I do business). We are all happy to pay a $700 premium for a correctly branded "Dave" model. 

I want that specific pictured one please.
```

---
## \#214 Posted by: amazingdave Posted at: 2018-10-25T11:00:11.245Z Reads: 261

```
Wow, what a quick turnaround! Looks great. I feel a kinship....
```

---
## \#215 Posted by: lrdesigns Posted at: 2018-10-25T11:21:29.861Z Reads: 259

```
Awesome! So fast. :heart_eyes: is that 13mm from the desk to the top of the display?
```

---
## \#216 Posted by: janpom Posted at: 2018-10-25T12:32:42.522Z Reads: 286

```
Hm, I never though of a premium package, but I do like the idea. After some thinking, let me present to you our premium features. The premium package will come with:

- Rebranding from VeGa to Dave, a name invented by [a panel of marketing experts](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/47?u=janpom) that has been repeatedly [asserted as being superior and more fitting](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/104?u=janpom).
![vega_premium_rebranding|690x149](upload://552JgprHs2SBqKLpDltAGrpuNPR.jpeg) 

- Extra big mounting holes that can accommodate M3 screws.
![vega_premium_holes|690x259](upload://i4Qmvcd39KHD0UPVaj0B9WC1kBz.png) 

- Spare 10k resistor!!!
![vega_premium_components|690x257](upload://1QWEgSOWLjubnVm783ro6inBZEH.png) 

- Premium packaging featuring an extra layer of bubble-foam for enhanced safety and extended bubble popping fun time.
![vega_premium_bubble_foam|690x257](upload://tAy0XavMNqAYPImPV6Ha67MF6n.png) 

Pricing:
- standard DIY package: $7 (no display included)
- premium DIY package: $700 (no display included)

The first to order the premium package, will also receive the first ever prototype as a bonus. The prototype is fully functional, except for the display that has been destroyed in course of the [research and development](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/97?u=janpom).

![IMG_1452|677x499](upload://2twSj0FeKn6BPYPhjW0MosR0153.jpeg) 

Due to high demand please expect a prolonged delivery time when ordering the premium package.
```

---
## \#217 Posted by: Mich21050 Posted at: 2018-10-25T13:22:05.660Z Reads: 272

```
Any idea when you will be able to sell kits? :smiley:
```

---
## \#218 Posted by: janpom Posted at: 2018-10-25T13:39:30.056Z Reads: 276

```
I ordered the parts from China with standard shipping to keep the costs low. (I only ordered the PCBs with DHL shipping so that I have them early to do some testing.) The packages should arrive in about a month.

I can also get all the parts locally (even the display), but for more expensive:
- [atmega chip](https://www.gme.cz/atmega328p-pu-sdip28-atmel) (~$4)
- [UART-USB adapter](https://www.gme.cz/prevodnik-usb-uart-reset-pin) (~$4)

All the small parts I can get pretty cheap even locally ($3-5 for everything). The PCB is $1. That's $12-$15 for the whole kit, excluding the display. With the parts from China it will be about $7 without the display (unless you want the premium package :smile:).

The displays I can get for ~$12 from [here](https://laskarduino.cz/displaje/230484-176x220-barevny-lcd-tft-displej-20-spi.html) if I order a few and spread the shipping cost.

I still haven't tested the PCBs though so this may be a bit premature. :slight_smile:
```

---
## \#219 Posted by: Grozniy Posted at: 2018-10-25T13:40:37.107Z Reads: 272

```
So now premium is 712?
```

---
## \#220 Posted by: janpom Posted at: 2018-10-25T13:43:58.541Z Reads: 269

```
You mean premium with the parts purchased locally? That would be premium premium. We don't even have that on our price list yet. I'll have to talk to our sales team about that.
```

---
## \#221 Posted by: janpom Posted at: 2018-10-25T14:01:51.575Z Reads: 265

```
[quote="lrdesigns, post:215, topic:71509"]
is that 13mm from the desk to the top of the display?
[/quote]

Yes, it's the full thickness including everything.
```

---
## \#222 Posted by: brenternet Posted at: 2018-10-25T14:39:29.321Z Reads: 257

```
700 I can do, I see the value. 712 I feel is just greedy and over the top.
```

---
## \#223 Posted by: moon Posted at: 2018-10-25T14:42:10.483Z Reads: 254

```
Shipping is free though
```

---
## \#224 Posted by: brenternet Posted at: 2018-10-25T14:45:33.836Z Reads: 249

```
ShIpPiNg Is AbSolUtEly **FREEEEEEEE**
```

---
## \#225 Posted by: spesh Posted at: 2018-10-25T15:06:43.045Z Reads: 246

```
Do people named dave get a discount?
```

---
## \#226 Posted by: Andy87 Posted at: 2018-10-25T16:04:42.935Z Reads: 245

```
Yeah for Dave’s it’s 800 without shipping... 👌
```

---
## \#227 Posted by: janpom Posted at: 2018-10-25T16:08:39.711Z Reads: 245

```
I'm happy to offer 10% discount off the Dave premium package to all Daves. If you order at least two, you get free shipping world wide.
```

---
## \#228 Posted by: DilatedPupils Posted at: 2018-10-25T16:20:50.291Z Reads: 245

```
Uh oh, Dave is gonna become the most popular name in the forum just to get the discount.

-Dave
```

---
## \#229 Posted by: brenternet Posted at: 2018-10-25T16:22:23.962Z Reads: 248

```
Sounds like a spooky sale 😂. None of this is lost on me haha
```

---
## \#230 Posted by: janpom Posted at: 2018-10-25T16:30:40.782Z Reads: 268

```
So I assembled one...

![IMG_1455|666x500](upload://9sOXVgNgkPAdBsHrNVGBOWLOOdl.jpeg) 

aaaaand...

It works! Yay!

![IMG_1456|666x500](upload://Dn6cAEbpRVwrI1FbjwiWXhlFNL.jpeg)
```

---
## \#231 Posted by: Skunk Posted at: 2018-10-25T16:33:09.701Z Reads: 256

```
Yep.  I want.  Must have.
```

---
## \#232 Posted by: Grozniy Posted at: 2018-10-25T16:37:01.643Z Reads: 260

```
I'm just considering the best investment: carvon or Dave premium :thinking:
```

---
## \#233 Posted by: Andy87 Posted at: 2018-10-25T16:37:53.541Z Reads: 257

```
What a question...
```

---
## \#234 Posted by: spesh Posted at: 2018-10-25T16:55:46.552Z Reads: 256

```
Dave premium of course
```

---
## \#235 Posted by: janpom Posted at: 2018-10-25T17:15:26.440Z Reads: 270

```
It turns out the PCB mounting holes are a perfect fit for M2 bolts. I thought that was a bug since the holes in the display's PCB are for M3 bolts. But... there's a very little space right to the display and the head of an M3 bolt doesn't fit there while a M2 bolt fits perfectly. I'm not sure if we can make any good use of that. Just FYI enclosure design team. @mmaner @lrdesigns @moon   

![IMG_1457|375x500](upload://sIkref1aqhRUCScOL8foISTLYCt.jpeg) 

![IMG_1458|666x500](upload://rLsDBVrMGIDVgnVCbCFd2pqF6Bq.jpeg)
```

---
## \#236 Posted by: mmaner Posted at: 2018-10-25T18:08:28.952Z Reads: 255

```
Im just about done with a tentative mode, trying to get some renders now.
```

---
## \#237 Posted by: brenternet Posted at: 2018-10-25T18:20:03.827Z Reads: 257

```
Flatter than Kate Hudson please.
```

---
## \#238 Posted by: Andy87 Posted at: 2018-10-25T18:28:05.019Z Reads: 255

```
Just as an idea, maybe you can implement a pop up in case there is a fault code.
Something like a red bar in the top or the down where the fault is written and will appear only in case there is a fault.
I know we limited by the display, so maybe there is some other kind of indication we can think about. I don’t know so much faults but it would be nice to have something as min for drv fault and abs over current.
```

---
## \#239 Posted by: mmaner Posted at: 2018-10-25T18:45:39.890Z Reads: 270

```
This is my initial version, I already see some changes I want to make but I think its good for a test run.

![MM%20vega%20lcd%20monitor%20v02%20case%20102518%20-%2001|606x500](upload://7GW7aAIhM08JCngCrkvCOVgNZlN.jpeg) 
![MM%20vega%20lcd%20monitor%20v02%20case%20102518%20-%2002|429x500](upload://5Fngki8d4dOIu1yLYJ1Brzmm9V9.jpeg) 
![MM%20vega%20lcd%20monitor%20v02%20case%20102518%20-%2003|690x471](upload://i660UBEdX5XBOnnOhbZWS6N0a0k.jpeg) 

    1.  There is a base plate that can be used to mount over X-Braces, in case anyone wants it.  
    2.  I am using passthrough columns to mount the electronics to the case using a 2mm hex head screw on top and bolt on the bottom, preferably with a rubber washer between the nut and PCB.  This keeps  aspace between the electronics and the deck, hopefully minimizing damage, and can be used for a neoprene pad or such.
    3.  I am using 1in coarse thread wood screws to mount the case to the deck, preferably a philips or hex version.  I'll go looking and see what specific screws I can find once I have a test piece printed.
    4.  There are 3 buttons on the side, Im assuming using standard 4.5mm momentary push buttons mounted to the inside of the case and the the printed buttons being glued to them during the assembly.
    5.  I have included a 1.5mm lexan/polycarbonate screen protector.  I have no clue where to get that, but I can probably cut a few at work if they are difficult to source.

Everything, other than the electronics and screws, is printable including the columns and base plate.  Thh base plate should probably be cut from aluminum, but I doubt an ABS or Nylon version would be much worse.
```

---
## \#240 Posted by: janpom Posted at: 2018-10-25T19:21:52.619Z Reads: 245

```
That looks pretty neat! I should get a 3D printer. I just have to think of some good arguments for my wife that we need one. I'm afraid that "I need to print a case for a gadget for my eMTB" wouldn't do.
```

---
## \#241 Posted by: Andy87 Posted at: 2018-10-25T19:26:56.246Z Reads: 241

```
They you need the printer for Dave.
I‘m sure she will understand that 😌
```

---
## \#242 Posted by: brenternet Posted at: 2018-10-25T19:29:28.360Z Reads: 246

```
Sex toys, just make sure you putty spray and fine grit sand them before use. Otherwise... ribbed, for her pleasure.
```

---
## \#243 Posted by: Vanarian Posted at: 2018-10-25T20:14:34.391Z Reads: 242

```
If you only plan to make cases, why not get a loyal Dave follower to print some for you?
```

---
## \#244 Posted by: ROFEN13 Posted at: 2018-10-25T21:46:17.654Z Reads: 230

```
This is so cool, and affordable... I need one!
```

---
## \#245 Posted by: mmaner Posted at: 2018-10-25T21:57:01.137Z Reads: 238

```
RE, my models posted above...

I am going to make a wedge version of the base plate.  That way if anyone wants to have the display angled up from the front, that is possible.  Just haven't done it yet as it will all change if my dimensions are off.
```

---
## \#246 Posted by: spesh Posted at: 2018-10-25T22:57:48.635Z Reads: 229

```
can you include a version with Dave written on the case please?
```

---
## \#247 Posted by: mmaner Posted at: 2018-10-26T00:05:00.906Z Reads: 235

```
I'll see what I can do 😀
```

---
## \#248 Posted by: brenternet Posted at: 2018-10-26T00:10:18.072Z Reads: 234

```
Real Mvp 🤣
```

---
## \#249 Posted by: lrdesigns Posted at: 2018-10-26T00:44:43.266Z Reads: 253

```
[quote="janpom, post:235, topic:71509"]
M2 bolt fits next to the LCD. I’m not sure if we can make any good use of that. Just FYI
[/quote]

It could be used to make a design where there is not 4 bolt holes at the top which could be more waterproof. 

[quote="janpom, post:221, topic:71509"]
13mm Yes, it’s the full thickness including everything.
[/quote]
Cool, I can make mine 4mm shorter on the top half, I got around 16mm at the moment and I think 2mm screen will be plenty. And make the base slimmer as I had a cutout for the through hole components legs to have room.

![IMG_0923|606x500](upload://4sv41zwIvwAKqlMoTxPowuPay92.jpeg) 

![IMG_0922|666x500](upload://suhqChILgPGNJcSKt6n3g04faoj.jpeg) 

![IMG_0926|666x500](upload://eMc8QDGEGFqlASzWc5KjSmBfrG8.jpeg)

I think its time I ordered the LCD. :smirk:
```

---
## \#250 Posted by: Static Posted at: 2018-10-26T00:48:18.911Z Reads: 230

```
SLA is so clean. Was that made on a form labs printer?
```

---
## \#251 Posted by: lrdesigns Posted at: 2018-10-26T01:05:37.752Z Reads: 229

```
Yes, its kinda cheating.
```

---
## \#252 Posted by: janpom Posted at: 2018-10-26T10:58:21.954Z Reads: 232

```
I have a big request for the enclosure designers. Would it be possible to make an adjustment such that the top part attaches to the bottom plate with some clip-on mechanism rather than with bolts? With my convertible Velcro Board, I need to be able to take VeGa off easily. Having to undo 4 bolts would add too much to the transforming time. Pretty please.
```

---
## \#253 Posted by: Skunk Posted at: 2018-10-26T14:45:22.921Z Reads: 240

```
https://www.amazon.com/BLACK-DECKER-Li2000-Rechargeable-Screwdriver/dp/B005LTNLDS/ref=sr_1_4?s=power-hand-tools&ie=UTF8&qid=1540565096&sr=1-4&keywords=electric+screwdriver
```

---
## \#254 Posted by: totalgeek9224 Posted at: 2018-10-26T15:06:58.286Z Reads: 237

```
So, Hows Dave coming along everyone?
```

---
## \#255 Posted by: mmaner Posted at: 2018-10-26T15:19:33.001Z Reads: 242

```
Now you do both or either...

![image|608x500](upload://oylDkeCx1HFX4YPKrmPGNObVepM.jpeg)
```

---
## \#256 Posted by: mmaner Posted at: 2018-10-26T15:24:39.366Z Reads: 239

```
...and then there's this :slight_smile:.

![image|690x299](upload://fvbnO3OBKojBCH1JP1fhsfolFka.jpeg)
```

---
## \#257 Posted by: thisguyhere Posted at: 2018-10-26T16:20:11.618Z Reads: 231

```
sorry i missed the boat on this one but why's it being called dave?
```

---
## \#258 Posted by: spesh Posted at: 2018-10-26T16:26:28.344Z Reads: 235

```
perfect :+1:
```

---
## \#259 Posted by: Skunk Posted at: 2018-10-26T16:27:42.202Z Reads: 235

```
@brenternet explain yourself
```

---
## \#260 Posted by: mmaner Posted at: 2018-10-26T16:30:56.533Z Reads: 248

```
![MM%20vega%20lcd%20monitor%20v02%20complete%20102618|500x500](upload://vVlGpLZQ3Naw1Dqodh5csuxq3Kk.jpeg)
```

---
## \#261 Posted by: Mich21050 Posted at: 2018-10-26T16:31:33.357Z Reads: 248

```
@mmaner That looks dope :smile:
```

---
## \#262 Posted by: janpom Posted at: 2018-10-26T17:47:13.442Z Reads: 249

```
Awesome! Thanks a lot for that. That was super quick. The whole case looks great! Have you tried printing it yet?
```

---
## \#263 Posted by: mmaner Posted at: 2018-10-26T17:48:59.423Z Reads: 246

```
not yet, I'm going to this weekend.  But I really need the display and perfboard to get a good fit and measure the hole tolerances.  The display and ATMEGA should be here next week,
```

---
## \#264 Posted by: janpom Posted at: 2018-10-26T17:56:34.551Z Reads: 229

```
Just PM me your address. I'll ship the whole kit to you on Monday. The premium version of course. :smile:
```

---
## \#265 Posted by: mmaner Posted at: 2018-10-26T18:04:06.199Z Reads: 222

```
I appreciate it.  Let me know what I owe you.
```

---
## \#266 Posted by: mmaner Posted at: 2018-10-26T18:05:34.134Z Reads: 222

```
Its apparently a british thing, started off as a joke but now people really wanna call it DAVE :slight_smile:.
```

---
## \#267 Posted by: brenternet Posted at: 2018-10-26T18:16:48.692Z Reads: 226

```
It's not a British thing! It's just the best name for this amazing device.
```

---
## \#268 Posted by: janpom Posted at: 2018-10-26T18:49:40.507Z Reads: 231

```
We could call it DaVeGa as a compromise. :smile:
```

---
## \#269 Posted by: mmaner Posted at: 2018-10-26T18:52:25.191Z Reads: 233

```
[quote="janpom, post:268, topic:71509"]
DaVeGa
[/quote]

This :arrow_up: :slight_smile:
```

---
## \#270 Posted by: brenternet Posted at: 2018-10-26T18:59:52.923Z Reads: 235

```
This could work. I'll speak to my people about getting a contract drawn up.

(My people are 4 and 1 years old and currently hanging off my legs)
```

---
## \#271 Posted by: janpom Posted at: 2018-10-26T19:19:29.921Z Reads: 246

```
It's worth considering that the re-branding cost savings would be substantial!

![IMG_1461|690x309](upload://gsDmz9s8iZivErCPII3euRynbEZ.jpeg)
```

---
## \#272 Posted by: mmaner Posted at: 2018-10-26T19:34:44.899Z Reads: 240

```
![image|690x231](upload://sqMSmkyNk4EltBSrmSesvuyNty4.jpeg)
```

---
## \#273 Posted by: janpom Posted at: 2018-10-27T16:18:06.225Z Reads: 236

```
If anyone would like only the PCB, I can get it to you for $3 shipped ($1 PCB, $2 shipping). It should work world wide. It's untracked for that price. Tracked is ~$5, which is not worth it given the PCB price. The components needed for the assembly should be easy to get. I can get all in the local electronics store over the counter.
```

---
## \#274 Posted by: bigben Posted at: 2018-10-27T16:20:33.804Z Reads: 232

```
Yes please. I’ll go for a few to the UK.
```

---
## \#275 Posted by: janpom Posted at: 2018-10-27T17:32:59.641Z Reads: 236

```
@bigben Please PM me your address and how many would you like.

The same goes for anyone else who would like PCBs only.

I expect it won't be before 2-3 weeks before I can ship full kits.

Just a reminder: The kits will come without the display. If you haven't ordered one yet, it maybe be a good time to do it since it will take a while until it arrives to you. [This](https://www.aliexpress.com/item/ILI9225-2-0-Inch-UART-TFT-LCD-Display-Module-SPI-Interface-Colorful-Screen-Serial-Port-176x220/32792711665.html?spm=2114.search0104.3.8.3fc12510d3yVHc&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_318_319_10696_450_10084_10083_10618_452_535_534_10304_533_10307_10820_532_10821_10302_204_10059_10884_323_10887_100031_320_10103_448_449,searchweb201603_2,ppcSwitch_0&algo_expid=cc29c9d0-515b-4481-92b6-cf84a26d2a5c-1&algo_pvid=cc29c9d0-515b-4481-92b6-cf84a26d2a5c&transAbTest=ae803_4) is the cheapest source I have found, but I don't have any experience with them, so I can't give any recommendations.
```

---
## \#276 Posted by: thisguyhere Posted at: 2018-10-27T17:40:23.426Z Reads: 240

```
[quote="brenternet, post:267, topic:71509"]
It’s just the best name for this amazing device.
[/quote]

still not a satisfying answer, but it's ok.

[quote="janpom, post:273, topic:71509"]
If anyone would like only the PCB, I can get it to you for $3 shipped
[/quote]

PM'd
```

---
## \#277 Posted by: bigben Posted at: 2018-10-27T17:48:44.492Z Reads: 242

```
Pmd back. If you need an enclosure for your board let me know and I’ll send one out to you. 
Think of it as a small thank you for what you’re doing for the community.
```

---
## \#278 Posted by: Kug3lis Posted at: 2018-10-27T17:50:09.783Z Reads: 241

```
I had idea to put also programmable RGB strip controller port but after running simple examples it used over 80% of memory on ATmega32u4 so I don't think it would fit together with main software. I will try to look either separate solution or into bigger flash mcu :P

Because those strips looks sick :P

https://youtu.be/OoyZ53-rQ94
```

---
## \#279 Posted by: janpom Posted at: 2018-10-27T18:52:21.445Z Reads: 255

```
@Kug3lis That looks cool. Is the speed / battery status somehow reflected in that?
```

---
## \#280 Posted by: janpom Posted at: 2018-10-27T20:17:19.337Z Reads: 269

```
Here's some info about the kit assembly, currently mainly for those who asked for the PCBs only.

This is the PCB layout:

![50|690x439](upload://9MJIfzm8eXtSbN20dX2vhuObT0b.png) 

Required components:
- ILI9225 2.0" TFT LCD Display
- ATMEGA328P-PU
- 16 MHz crystal
- 2x 20pF capacitor
- 100nF capacitor
- 1N4148 diode
- 10k resistor
- 3x button (only BTN1 currently used)
- 8 pin JST PH female connector (for the VESC)
- 5 or 6 pin right angle female pin header (for programming)
- USB-UART adapter (for programming)

Recommended:
- 8 pin JST PH male connector, 1 and 4 pin dupont female connectors
  - to make an 8 pin JST -> 5 pin dupont adapter for programming
  - update: maybe [this](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/294?u=janpom) is a better solution

Assembled PCB:
![38|690x441](upload://zW8spSw1zIIxU357mIcj24IZ4Es.jpeg) 

The VESC and DEBUG pads are for 4 pin JST PH connectors, but these are not needed. Better to solder on wires directly. VESC cable wires can be soldered either to the VESC pads plus the DTR (if you want to use the cable for programming as well) or to the 5 USB-UART pads.

In the local stores, I wasn't able to find small enough 20pF capacitors. The ones I found are taller than the chip (second tallest) and that increases the thickness of the whole thing.

![IMG_1467|690x448](upload://k07z6EbXIqceV1RAsgjFkwXDYw4.jpeg) 

Therefore I used SMD caps instead. If you need to do the same, I recommend the 0805 ones. Though smaller, they are easier to solder on than the 1206 since they fit in better.

Alternatively, it's possible to use the DIP caps and carefully bend them.

![IMG_1468|690x420](upload://nFyO53X3A13mAvMH4UFjt6LyjIi.jpeg) 

Be sure to **[burn a bootloader](https://www.arduino.cc/en/Tutorial/ArduinoToBreadboard) before soldering on the chip**.

[Here's](https://github.com/janpom/vega#configuring-and-installing-firmware) how to install the firmware.

Good luck!
```

---
## \#281 Posted by: janpom Posted at: 2018-10-27T20:51:37.998Z Reads: 262

```
Gerber files can be downloaded from https://easyeda.com/honza.pomikalek/VESC-Gauge.

- scroll down to "PCB v0.2" and click on "Open in Editor"
- select "Generate Fabrication File" from the menu:
  ![31|603x500](upload://4PIJfVxyI0Yl139bYPw7dUWtJbc.png) 

@thisguyhere
```

---
## \#282 Posted by: Indiangummy Posted at: 2018-10-27T21:01:55.515Z Reads: 256

```
[quote="janpom, post:280, topic:71509"]
10k resistor
[/quote]

Hey, does it matter what tolerance they are? I have some silver and gold ones in my parts kit from school and I was just gonna use those
```

---
## \#283 Posted by: janpom Posted at: 2018-10-27T21:06:36.910Z Reads: 246

```
It's just a pull up resistor. You can use pretty much any value close to 10k.
```

---
## \#284 Posted by: iTzDiego Posted at: 2018-10-28T03:36:58.904Z Reads: 240

```
What if you made this available to put to a custom remote instead? If that is possible

TAKE MY MONEY!
```

---
## \#285 Posted by: Jake2k17 Posted at: 2018-10-28T04:32:47.196Z Reads: 240

```
I’m definitely interested. Count me in.

 evaD
```

---
## \#286 Posted by: janpom Posted at: 2018-10-28T08:09:22.458Z Reads: 247

```
I'm afraid the display is a bit too big for that. Remotes with smaller displays already exist. The [Firefly](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543) has a small 128x32 display. A version with a bigger display [is being worked on](https://www.electric-skateboard.builders/t/solidgeeks-firefly-remote-with-bigger-screen-what-do-u-prefer-on-screen/70221).

At any rate, if anyone wants to make an Arduino based remote with the 2.0" LCD, I'm happy to help with adjusting the VeGa FW for it.
```

---
## \#287 Posted by: StefanMe Posted at: 2018-10-28T08:41:36.759Z Reads: 240

```
If u find an Display who ll fit in... 2 inch Huge for a remote. Any suggestions? 

The 0.96 inch display is more than enough. I mean... bigger screen is cool :). But also took a lot of power by rendering ect. U need all recourses u have for cycle time and calculating. My small 0.96.inch display needs around 45-50ms to refresh in the fastest possible mode. Double size screen could take a bit longer. We have to test it...
```

---
## \#288 Posted by: Superflim Posted at: 2018-10-28T08:55:11.095Z Reads: 233

```
Will these also be available like plug and play?
I wouldn’t trust myself to assemble such a kit...
```

---
## \#289 Posted by: janpom Posted at: 2018-10-28T08:55:19.521Z Reads: 238

```
IMO, what you have is just about the right display size for the remote and I like your GUI. Adding speed would be a nice feature. Maybe you could get rid of the "POWER" label and move the wifi and headlight indicators to that area. You could get rid of the small battery indicator, which is redundant. Then you have the right side of the display free for more info.

Note that you don't need to redraw the full display. You can only update what changed (e.g. speed). That way you can do much faster refresh rate. That's what I do on VeGa. Redrawing everything each time wouldn't be feasible.
```

---
## \#290 Posted by: janpom Posted at: 2018-10-28T09:01:00.046Z Reads: 228

```
Yes, I can assemble a few. It doesn't take much time and I kinda enjoy doing it. Note that you'll still need to do the wiring to the VESC so some soldering to the PCB is probably inevitable.

At any rate, as I said before, the first batch is meant for those who don't mind to be beta testers. There will likely be problems that will require some tweaking. If you want a plug-and-play version, it's best if you wait a little bit.
```

---
## \#291 Posted by: StefanMe Posted at: 2018-10-28T09:49:33.509Z Reads: 234

```
I have a button and u can switch through 4 different views with dirfferent informations. The section “Power” is the most important one for me at the moment because of my battery issues. There is also a long bar above the trigger jndicator I can’t see at the moment, because there is nothing connected.

Thanks for the tip with updating just sections who changed. I already into this... I expect them around -10ms. But 60ms total is allready perfect. At the beginning I was at around 130ms. 

But I am still seachring for a better display... maybe colored or with much more brightness liebe a Sharp reflective display from Adafruit. Any suggestions there?
```

---
## \#292 Posted by: janpom Posted at: 2018-10-28T10:40:17.883Z Reads: 242

```
There's a [smaller version](https://www.aliexpress.com/item/Free-Shipping-1-8-inch-TFT-touch-LCD-Module-LCD-Screen-Module-SPI-serial-51-drivers/32265119437.html) of what I use for VeGa, but it's probably still too big.
```

---
## \#293 Posted by: janpom Posted at: 2018-10-28T14:28:27.065Z Reads: 266

```
Some thoughts about wiring things up. Ideally, we would have a single cable going out of DaVeGa that we can connect either to VESC or to the USB-UART adapter for programming.

There are 5 pins on VeGa:
- 5V
- GND
- TX
- RX
- DRT

The VESC connects to the first 4. The USB connects to all.

Here's the pinout of the devices to be wired up (for the VESC, this is how my ESCapes look like; I think that other VESC derivatives have a different pin order, but that doesn't really matter):

![32|556x460](upload://1EdYnlnVC9fRSR4w7JkSSLAEsuQ.png) 

Now, one option is to simply split 4 wires and add two connectors. That's what I have done [here](https://www.electric-skateboard.builders/t/vega-battery-monitor-odometer-speedometer/71509/148?u=janpom). But, it's pretty annoying having to split 4 wires and you end up with the dupont connector dangling around all the time when it's only used rarely.

![07|591x500](upload://mDuilTn81MEbtQ3Mh27JWvHDg1E.png) 

An alternative would be to make an adapter. It's natural to go from more wires to fewer wires, i.e. from USB to VESC. But, that wouldn't be very reliable since the dupont connectors tend to slide off. Plus, the device that's plugged-in most of the time (the VESC) would go in via an adapter. Not ideal.

![53|690x318](upload://roQyYX4ObNRWhPrrvC3HS2WKAGB.png) 

We can go the other way around, but that means the DTR wire would need to be separate. It's not a problem to connect the 6 pin USB-UART to two (1+5 pin) dupont connectors. This would work just fine. We would end up with only a 1 pin dangling connector. No Y-splits needed.

![34|690x338](upload://fdtyQlV777PLrB0DREh43ri8x03.png) 

An even better option would be to connect all 5 VeGa pins to the VESC and then make a simple adapter to the 6 pin dupont without the stand-alone wire for DTR. I think that it should be OK to connect the DTR to one of the VESC's ADC pins. DTR is high (5V) in a normal state, but I believe the ADC pins are not used for anything by default. The only problem would be if the ADC is pulled low since that would reset the VeGa, but that shouldn't happen. Could someone with a better knowledge of the VESC HW please confirm this? @Kug3lis maybe? Thanks! I know this is a hackish solution, but it seems the simplest and most elegant.

![51|690x314](upload://fxDySorvE35IHWKkiFD1WSBh73d.png)  

Last but not least, it's not necessary to connect the DTR at all. Then we would need an extra button for resetting VeGa manually. It's not hard to reset manually at the right moment when updating the FW. Still, it's an extra button.
```

---
## \#294 Posted by: janpom Posted at: 2018-10-28T17:11:23.507Z Reads: 237

```
After more thinking, we could just do this:

![53](https://www.electric-skateboard.builders/uploads/db1493/original/3X/c/0/c009c0138a988cc9c9647f132814af9d240eddd1.png)

... but use JST XH instead of the dupont. The JST won't slide off and 2.54mm spaced pins of the USB-UART can be plugged into a female JST XH directly. It would still mean the VESC goes in via an adapter, but I guess that's fine.
```

---
## \#295 Posted by: janpom Posted at: 2018-10-28T18:53:49.021Z Reads: 253

```
For you guys out there on that retarded rollercoaster. :smile:

![48|690x53](upload://ql8qngvT110oNqIz6MSzFsu1sIS.png) 

![IMG_1474|331x500](upload://k2dsaIi8opVieEVC9FhSsCbcH7h.jpeg)  ![IMG_1473|354x500](upload://dRbDuz6okX2b1K2T3V6G6F6WQ7p.jpeg)
```

---
## \#296 Posted by: louwii Posted at: 2018-10-28T19:37:40.945Z Reads: 245

```
I'm just experimenting stuff with Arduinos and you clearly mastered the thing already. This is really inspiring as a creator and dev. Thanks for sharing everything with us!
```

---
## \#297 Posted by: janpom Posted at: 2018-10-28T20:35:17.628Z Reads: 250

```
@lrdesigns This one is for you. :slight_smile:

![IMG_1475|375x500](upload://wc0rklfwjxhahStiIN43ot1Q5Q2.jpeg)   

Fully implemented and [pushed to master](https://github.com/janpom/vega/commit/70584dee8c66f6b8275d9977ead2f40592caa55a).
```

---
## \#298 Posted by: Skunk Posted at: 2018-10-28T20:54:26.483Z Reads: 248

```
![thanksfromanerica|220x165](upload://v6LpTrWgcUTRpD5Jd54aiP6NjIC.gif) 
Thanks
```

---
## \#299 Posted by: totalgeek9224 Posted at: 2018-10-28T21:41:04.631Z Reads: 243

```
[quote="janpom, post:293, topic:71509"]
DaVeGa
[/quote]

This makes it official- Let the rebranding begin!
```

---
## \#300 Posted by: pixelsilva Posted at: 2018-10-28T21:51:32.455Z Reads: 235

```
I will design the logo guys.:wink:
```

---
## \#301 Posted by: janpom Posted at: 2018-10-28T22:10:00.521Z Reads: 238

```
I'm still not sure if I really like DaVeGa. It sounds kinda weird. In fact, I don't even know what the correct pronunciation is. That's something we should thoroughly discuss. :smile: Is it DaVeGa like "the vega" or is it more like "dave ga"? Or is it something completely different? @brenternet, what do your people say?
```

---
## \#302 Posted by: janpom Posted at: 2018-10-28T22:16:52.673Z Reads: 243

```
@pixelsilva A logo would be great! I propose something minimalistic. I like minimalism. Here's a draft to get you started. :smile: 

![davega_logo_v1|40x50](upload://cbTuc9AFQOyTJGhscpxL2EaYC6K.png)
```

---
## \#304 Posted by: pixelsilva Posted at: 2018-10-28T22:26:35.833Z Reads: 246

```
You took my words from my mouth! Yes, is gonna be minimalistic. You can clearly differentiate DAVE from VeGa thats for sure. I'll be back later...

![ShrillOblongCygnet-small|434x250](upload://7f75cqWsrEFOHXVCFPEzy4hPyOK.gif)
```

---
## \#305 Posted by: totalgeek9224 Posted at: 2018-10-28T22:34:26.191Z Reads: 237

```
I think that it should officially be known (and pronnounced) as Da- VeGa, but amongst us, we would know it as Dave-ga
Our own little inside joke

But of course, we need to hear from @brenternet's people
```

---
## \#306 Posted by: brenternet Posted at: 2018-10-28T22:38:48.430Z Reads: 231

```
They are napping at the moment but I'll run it past them after paw patrol tomorrow morning.
```

---
## \#307 Posted by: lrdesigns Posted at: 2018-10-29T00:26:13.145Z Reads: 231

```
![2l6tmr|500x274](upload://8EqED2KBGymrCSB1UDwNijLFYWd.jpeg)

I thought monday morning would be lame. But now it is AWESOME. Thanks @janpom
```

---
## \#308 Posted by: lrdesigns Posted at: 2018-10-29T00:34:40.504Z Reads: 236

```
If you update the firmware, say some new stuff comes out or bug fix etc, will you lose the total distance number?

Edit, you already thought of that. Thanks!

// Changing the EEPROM_MAGIC_VALUE (to any value different from the current, e.g. 42 -> 43) will reset
// the EEPROM to the values defined below. This is especially handy for pre-setting the total distance
// traveled (EEPROM_INIT_VALUE_TOTAL_DISTANCE).
#define EEPROM_MAGIC_VALUE 42  // [1, 255]

#define EEPROM_INIT_VALUE_VOLTS 0
#define EEPROM_INIT_VALUE_MAH_SPENT 0
#define EEPROM_INIT_VALUE_TRIP_DISTANCE 0  // meters
#define EEPROM_INIT_VALUE_TOTAL_DISTANCE 0  // meters
```

---
## \#309 Posted by: janpom Posted at: 2018-10-29T10:44:15.073Z Reads: 229

```
It's done! Re-branded: https://github.com/janpom/davega

Oh boy, that required [so many changes](https://github.com/janpom/davega/commit/19346eccd6c6bee0fea81d62ecf2b273e099804f). And that's only the firmware. Now on to the hardware. :sweat_smile:
```

---
## \#310 Posted by: totalgeek9224 Posted at: 2018-10-29T12:38:57.272Z Reads: 226

```
Alas! Let mass production begin!
```

---
## \#311 Posted by: brenternet Posted at: 2018-10-29T15:44:55.057Z Reads: 226

```
Amazing. Justice for the masses of 4 people pushing for this change!

All in good humour 😂. @bigben has been kind enough to order me one. Probably going to cnc a bamboo enclosure for it, will give you updates on how it goes.
```

---
## \#312 Posted by: janpom Posted at: 2018-10-29T17:12:20.310Z Reads: 234

```
I shipped all the packages today (@bigben, @lrdesigns, @bsancken, @SeanHacker, @Bokard). All but one went untracked with the Czech Post. It's not the carrier I have the best experience with, but at least the shipping didn't cost more than the packages themselves. This is a good science for shipping the kits later since it went to various parts of the world (US, EU, Hong Kong) and both tracked and untracked, so we'll see how fast and how reliable it is. Guys, please let me know once you have the packages. According to the Czech Post, they should arrive in about 7 days (which I don't really believe, especially with the one to Hong Kong, but we'll see). I'll of course re-ship if anything gets lost.

I don't have any more PCBs only to sell. The ones I have left I need to keep for the kits.

BTW, the kit parts I ordered from China are already coming in. I received the first two packages today. I may be ready to ship the whole kits soon.
```

---
## \#313 Posted by: Grozniy Posted at: 2018-10-29T17:34:46.592Z Reads: 226

```
Soon we'll have enough testing for you to sell be completes
https://goo.gl/images/iVbNZP
```

---
## \#314 Posted by: pixelsilva Posted at: 2018-10-29T18:39:11.456Z Reads: 226

```
This is amazing. I'm exited. Will be working on the logo today.:ok_hand:
```

---
## \#315 Posted by: LukePL Posted at: 2018-10-29T19:26:06.564Z Reads: 224

```
Those are great news! Where I can sign up for a kit?
```

---
## \#316 Posted by: janpom Posted at: 2018-10-29T19:43:49.780Z Reads: 220

```
For now only [here](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/36?u=janpom). I'll send more info when I have the kits ready to be shipped.
```

---
## \#317 Posted by: LukePL Posted at: 2018-10-29T19:45:56.265Z Reads: 225

```
I did that some time ago :) Thanks for awesome work!
```

---
## \#318 Posted by: Blix Posted at: 2018-10-29T20:44:53.096Z Reads: 242

```
...
![davegalogo5|498x500](upload://nlfuknAia263LWcETfg3119bboG.png) 
NOOO! IT'S:
![davegalogo6|498x500](upload://7eKXnPXq6d9Vgm5eev7mfD4KRHU.png)
```

---
## \#319 Posted by: Bokard Posted at: 2018-10-29T23:43:54.544Z Reads: 226

```
Really looking forward to these man ^^
```

---
## \#320 Posted by: Itsmedant Posted at: 2018-10-30T13:08:26.279Z Reads: 225

```
This project is turning out damn well guys!
```

---
## \#321 Posted by: rey8801 Posted at: 2018-10-30T20:36:25.050Z Reads: 228

```
@janpom man fantastic project! I am going to be a beta tester too. One question do you think is possible to put in parallel on the uart port either firefly remote or a bluetooth module? BEcause I have already both of the UART ports on the vesc busy and I was wondering whether is possible to connect it in parallel with the firefly remote. It also gets telemetry, I thought it may work together. What do you think? Thx a lot!
```

---
## \#322 Posted by: janpom Posted at: 2018-10-30T20:53:08.609Z Reads: 231

```
[quote="rey8801, post:321, topic:71509"]
man fantastic project! I am going to be a beta tester too.
[/quote]

Thanks! Cool!

[quote="rey8801, post:321, topic:71509"]
is possible to connect it in parallel with the firefly remote
[/quote]

I'm not an expert but since the UART communication is bi-directional, I doubt that would work. You would need an UART multiplexer. I'm afraid it won't be straightforward to setup, sorry.

It's not like the VESC is sending the telemetry all the time and you can just consume it. You need to request the data each time.
```

---
## \#323 Posted by: rey8801 Posted at: 2018-10-30T20:55:08.969Z Reads: 226

```
it's ok, no problem. I will use firefly as remote only. I do not really look at the screen anyway. Except for speed and battery sometime.
```

---
## \#324 Posted by: janpom Posted at: 2018-10-30T21:10:39.611Z Reads: 220

```
Thinking more about it, a VESC UART multiplexer would be a useful and a relatively simple project. I wonder why anyone hasn't done it yet. At least I haven't found any mentions of it on the forum.
```

---
## \#325 Posted by: Mich21050 Posted at: 2018-10-30T21:11:50.408Z Reads: 210

```
I absolutley love the design. Thank you for your work. :smile:
```

---
## \#326 Posted by: rey8801 Posted at: 2018-10-30T21:16:34.573Z Reads: 204

```
I think because all these additional "gadgets", as you call it, are rather new and up to now the 2 UART ports available on a dual setup were enough.
```

---
## \#327 Posted by: Kug3lis Posted at: 2018-10-30T21:17:56.476Z Reads: 211

```
I am at the moment trying to reimplement my multiplexer from linux to arm which works on packet level :) so you can connect vesc tools (multiple instances) bluetooth apps, remotes, lcd and shit to single port :)
```

---
## \#328 Posted by: janpom Posted at: 2018-10-30T21:24:35.456Z Reads: 210

```
Ha, here we go. :slight_smile:
```

---
## \#329 Posted by: Mikenopolis Posted at: 2018-10-30T21:37:41.834Z Reads: 228

```
[quote="janpom, post:76, topic:71509"]
![|490x500](https://i.redd.it/2zvqpynr264z.png)
[/quote]

As much as I see the stupidity of the system we use here in the US the calendar makes more sense. I mean do you guys SAY 30th of October 2018 or do you say October 30th 2018?
```

---
## \#330 Posted by: moon Posted at: 2018-10-30T21:40:18.710Z Reads: 217

```
I say 30th of october most of the time
```

---
## \#331 Posted by: Mikenopolis Posted at: 2018-10-30T21:45:52.321Z Reads: 219

```
![giphy|347x404](upload://t92zituXR2PyK1SpoLZdNebmrIv.gif)
```

---
## \#332 Posted by: moon Posted at: 2018-10-30T21:47:00.988Z Reads: 207

```
Its just how I think, I think day before month
```

---
## \#333 Posted by: thisguyhere Posted at: 2018-10-30T21:53:12.147Z Reads: 213

```
metric system is better.  end of discussion.

the US won't move to metric system because all of american industry is based on imperial.

all attempts to convert to metric was met with BURNING opposition by US industry as it'll cost BILLIONS to retool.

this is a classic example of making one's bed and then laying in it forever even though it fucking sucks.
```

---
## \#334 Posted by: Scream Posted at: 2018-10-30T22:07:51.340Z Reads: 208

```
Yeah even saying the month first is totally a US/imperial thing.
```

---
## \#335 Posted by: bsancken Posted at: 2018-10-31T07:16:35.267Z Reads: 214

```
[quote="janpom, post:324, topic:71509, full:true"]
Thinking more about it, a VESC UART multiplexer would be a useful and a relatively simple project. I wonder why anyone hasn't done it yet. At least I haven't found any mentions of it on the forum.
[/quote]
As I was reading that, I was thinking - Maybe your next project?? Lol Could be as simple as a small black box - UART in (with power) and 3 UART out. Nice simple pcb with no user input (assuming this is how it would work).

Will def. be needing one of these soon.. soo... lol
```

---
## \#336 Posted by: janpom Posted at: 2018-10-31T07:47:40.504Z Reads: 210

```
Yeah, I thought about that too. I wish I had more time for doing these things. :slight_smile:
```

---
## \#337 Posted by: pixelsilva Posted at: 2018-10-31T07:47:40.922Z Reads: 211

```
@Mikenopolis, thats the _"Me the great island, the rest a big gray spot"_ sindrome.
```

---
## \#338 Posted by: Andy87 Posted at: 2018-10-31T07:50:53.934Z Reads: 209

```
Same here 😂
I think and say how I write the date
```

---
## \#339 Posted by: Andy87 Posted at: 2018-10-31T07:56:14.175Z Reads: 217

```
Is it possible to pair more devices to one Bluetooth module?
If yes why not only using the information sent from the module for an app and our davega?
I know that then there other stuff like power supply etc needed, but no need for a multiplexer
```

---
## \#340 Posted by: janpom Posted at: 2018-10-31T22:14:50.641Z Reads: 220

```
But then davega would need a BT module too, which is not a trivial extension. Plus, as you mentioned, you still need a wired connection for the power supply, so using wireless in parallel with that is weird. It would make sense if the gadget is battery powered but then we're already talking about a significantly different device.
```

---
## \#341 Posted by: brenternet Posted at: 2018-10-31T23:29:28.894Z Reads: 226

```
![84667109|528x500](upload://7WufMywPNrN4cTgJ3jx6dLbF5s4.jpeg)
```

---
## \#342 Posted by: moon Posted at: 2018-10-31T23:51:01.293Z Reads: 224

```
Fahrenheit.... How does that even work
```

---
## \#343 Posted by: lrdesigns Posted at: 2018-11-01T00:27:41.634Z Reads: 220

```
You forgot to draw metric as a fist bump! :fist_right:
```

---
## \#344 Posted by: mmaner Posted at: 2018-11-01T01:12:36.767Z Reads: 225

```
[quote="moon, post:342, topic:71509, full:true"]
Fahrenheit… How does that even work
[/quote]

![PuNzp_d|640x413](upload://dhCysKatVhSvacED47tZ0kGFHHX.jpeg)
```

---
## \#345 Posted by: Battosaii Posted at: 2018-11-01T01:22:39.776Z Reads: 213

```
On paper metric sounds great but in the real world for professionals that use measuring tape for a living imperial makes more sense and is much more intuitive and easier to find exact measurements. Each system has it's ups and downs
```

---
## \#346 Posted by: lrdesigns Posted at: 2018-11-01T01:22:40.552Z Reads: 211

```
If your into cold or hot beverages, celsius is really useful. :coffee: :beer:
```

---
## \#347 Posted by: Battosaii Posted at: 2018-11-01T01:24:16.337Z Reads: 208

```
I water cool and over clock my pc's and I use Celcius to measure tempurature
```

---
## \#348 Posted by: Kug3lis Posted at: 2018-11-01T01:25:24.139Z Reads: 204

```
Explain how the fck it makes sense because 3mm is easier to understand than 1/8 of the inch

Also its easier to say 0.05mm than 1/500 of the inch
```

---
## \#349 Posted by: Battosaii Posted at: 2018-11-01T01:29:28.794Z Reads: 214

```
For a carpenter for example its much easier to find exact measurements on a measuring tape in feet than it is in CM. 

https://youtu.be/odVPwNgD8w4
```

---
## \#350 Posted by: lrdesigns Posted at: 2018-11-01T01:34:15.270Z Reads: 211

```
This metric VS imperial is really fun, but way off topic. :joy::rofl::joy::rofl:
```

---
## \#351 Posted by: Kug3lis Posted at: 2018-11-01T01:37:13.566Z Reads: 216

```
All the points he described is because he born and lived with the imperial unit system, while the rest of the world wood workers use metric without any issues. I never even heard (subscribed to many woodworkers) who would use imperial outside US.

Regarding measuring tape I have never had an issue finding something on metric tape it even has decimals (decimeter) markings in red.

![Image result for measuring tape](https://c1.staticflickr.com/1/892/27289592328_9c6f03e2fb_b.jpg)

Sorry for offtopic lets get back to topic :D
```

---
## \#352 Posted by: lrdesigns Posted at: 2018-11-01T01:44:19.199Z Reads: 206

```
I think we should split a new topic so we can keep arguing about it. I  mean passionately discussing. @moderators1

Guys there already is a thead. 

https://www.electric-skateboard.builders/t/imperial-vs-metric/56357?u=lrdesigns

Lets bring it back to life :man_scientist:
```

---
## \#353 Posted by: thisguyhere Posted at: 2018-11-01T02:53:23.735Z Reads: 211

```
going off topic ------

[quote="Battosaii, post:345, topic:71509"]
more intuitive and easier to find exact measurements
[/quote]

sorry, but i can't disagree enough.

performing fractions will never be easier than just converting in base 10.

the example the guy in the video said something about 5/32" being an actual measurement, while the same measurement in cm would be some number with four decimal places.  first, that's a dumb way to convert in to cm.  and if working in metric you wouldn't use that as a standard size.

anyway, back to the topic on hand.

back on topic ------
```

---
## \#354 Posted by: thisguyhere Posted at: 2018-11-01T02:56:03.233Z Reads: 219

```
[quote="mmaner, post:344, topic:71509"]
> Fahrenheit… How does that even work

![PuNzp_d|640x413](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/d/5d1a3555e1c518000306200687a5d7fec98a22a9.jpeg)
[/quote]

i read this on reddit the other day, but 

fahrenheit is asking how people feel
celcius is asking how water feels
kelvin is asking how an atom feels
```

---
## \#355 Posted by: spesh Posted at: 2018-11-01T05:18:10.595Z Reads: 206

```
I approve of the rebrand 👍
```

---
## \#356 Posted by: pixelsilva Posted at: 2018-11-01T08:34:43.889Z Reads: 206

```
@Battosaii ...

http://gifimage.net/wp-content/uploads/2017/06/wait-what-gif.gif
```

---
## \#357 Posted by: pixelsilva Posted at: 2018-11-01T08:40:02.617Z Reads: 213

```
[quote="Battosaii, post:345, topic:71509, full:true"]
On paper metric sounds great but in the real world for professionals that use measuring tape for a living imperial makes more sense and is much more intuitive and easier to find exact measurements. Each system has it’s ups and downs
[/quote]

Whaaattt??? ... 3/8 ... 5/16... 5' 9'' ... 32 inches ....18Oz ... you got to be kidding @Battosaii !!  .....yeah, _'imperial makes more sense and is much more intuitive'_ but in planet Pluto!
```

---
## \#358 Posted by: janpom Posted at: 2018-11-01T08:57:10.534Z Reads: 212

```
Just to bring the thread back on topic: I did some more accidental science yesterday which tested the durability of the DAVEga display. I drove over it with my board. And it survived! Yay! :slight_smile: 

You can read more about that [here](https://www.electric-skateboard.builders/t/new-discipline-eskate-kiting/72929) (at the end).
```

---
## \#359 Posted by: Andy87 Posted at: 2018-11-01T09:00:43.494Z Reads: 213

```
just ordered two displays. so from my site everything ready :sweat_smile::joy:
```

---
## \#360 Posted by: CarbonV Posted at: 2018-11-01T09:28:02.873Z Reads: 219

```
I ordered some PCB's as well as @janpom was already sold out :open_mouth:. They are in production now, I could easily send them via envelope to people in EU. I got 5 spare at the moment. If anyone wants some let me know! A symbolic dollar for the PCB same price as @janpom, shipping I'll need to look depending on where you live and if you want tracking. :slight_smile: 

![image|364x114](upload://t6wKyZUqPhySaLChF24jXxqVXMH.png)
```

---
## \#361 Posted by: JonathanLau1983 Posted at: 2018-11-01T09:51:39.027Z Reads: 214

```
PMed :smiley:

10 char
```

---
## \#362 Posted by: spesh Posted at: 2018-11-01T10:08:47.708Z Reads: 210

```
PM'd - better get in on this :slight_smile:
```

---
## \#363 Posted by: CarbonV Posted at: 2018-11-01T10:11:00.771Z Reads: 209

```
Last one of my spares is gone as well!
```

---
## \#364 Posted by: JonathanLau1983 Posted at: 2018-11-01T10:39:37.382Z Reads: 212

```
Anyone sourced multiples of the BOM and willing to sell some or all of the components?
Already ordered the LCD from AliExpress.
```

---
## \#365 Posted by: Sebike Posted at: 2018-11-01T11:01:20.613Z Reads: 208

```
I'm staying off topic here..
As I'm half/half, the swedish side of me sais the 30th of October, the hungarian half sais October 30th, so it's not really "rest of the world" when it comes to this, but in both cultures do we write the date as year.month.day when using numbers only.
```

---
## \#366 Posted by: spesh Posted at: 2018-11-01T11:07:07.296Z Reads: 210

```
Does anyone have a list of, say, mouser part numbers for the kit required?  the crystal options alone are mind boggling.
```

---
## \#367 Posted by: Battosaii Posted at: 2018-11-01T12:32:00.425Z Reads: 210

```
Makes perfect sense to me but then again I worked as a contractor for a while my whole world is fractions and it comes so easily I don't have to think.about it. 

Sorry to go off topic I didnt realize how passionate people could be about the subject.

Davega looks awesome.  Can't wait to get my hands on one.
```

---
## \#368 Posted by: bigben Posted at: 2018-11-01T13:13:29.942Z Reads: 223

```
![image|666x500](upload://3GNl7s8r9Lby0OAtiQlUVGoz9kF.jpeg) ![image|666x500](upload://tvoQDkqOjKK1i54twfFuM7otTNX.jpeg)
Arrived safe and sound. Now to source the parts. Like others, screens are on their way. Just the rest of it is a little confusing..
```

---
## \#369 Posted by: JonathanLau1983 Posted at: 2018-11-01T14:47:15.727Z Reads: 214

```
@janpom Your BOM says 20pF capacitors but one of your pics is showing you using 22pF. Presume they're okay to use too?

This ebay listing has the 16Mhz Crystal, and 2 x 20pF along with the ATMega328P
https://www.ebay.co.uk/itm/Atmega328P-PU-Arduino-Bootloader-16MHZ-Crystal-22pF-Capacitors-Atmega328p/132794820324?hash=item1eeb3026e4:m:m-HtOvcZkVKeHVChrjG_bwA:rk:2:pf:0
```

---
## \#370 Posted by: brenternet Posted at: 2018-11-01T14:59:27.212Z Reads: 210

```
That particular one will never see a single volt. Framing that for the mancave.

The day the people won
```

---
## \#371 Posted by: Kug3lis Posted at: 2018-11-01T15:00:03.642Z Reads: 209

```
yeah should work :)
```

---
## \#372 Posted by: JonathanLau1983 Posted at: 2018-11-01T15:17:23.922Z Reads: 209

```
These should work

100nF capacitor
https://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/5381310/

1N4148 diode
https://uk.rs-online.com/web/p/switching-diodes/7390290/
```

---
## \#373 Posted by: janpom Posted at: 2018-11-01T15:53:50.924Z Reads: 202

```
Note that you'll make it thicker if you use headers for the LCD. It's meant to be soldered on the PCB directly. If you want to use headers only for testing, I recommend that you get a few smaller ones, e.g. 3 pieces of 3 pin headers. These will be much easier to desolder if you decide to do so. Also, there are 11 pins on the display. 10 pin header won't work since pins at both ends need to be connected. 2x5 or 3x3 works though.
```

---
## \#374 Posted by: JonathanLau1983 Posted at: 2018-11-01T16:21:11.020Z Reads: 202

```
[quote="janpom, post:373, topic:71509"]
Note that you’ll make it thicker if you use headers for the LCD. It’s meant to be soldered on the PCB directly.
[/quote]

Ah I didn't realise, I'll remove them from the post.
```

---
## \#375 Posted by: JonathanLau1983 Posted at: 2018-11-01T17:32:01.441Z Reads: 207

```
Been thinking about the case and best way to get a seal to make it as water resistance as possible.

This is what I'm thinking of doing with a variety of nylon standoffs, bolts and nuts. Will be designing a case too once I get the PCB and LCD to fit my Trampa.

Btw, what's teh switch used for? Should it be included in the case design?

![image|677x500](upload://V2d1rtqcmegrWQcmTcAMKuLn9J.png)
```

---
## \#376 Posted by: pixelsilva Posted at: 2018-11-01T18:34:03.438Z Reads: 194

```
Don't worry man. just pulling your leg. :wink: :sweat_smile:
```

---
## \#377 Posted by: janpom Posted at: 2018-11-01T19:23:42.281Z Reads: 201

```
Switch? You probably mean the button. That's currently used for resetting the current trip. Including it in the case design would be a good idea.
```

---
## \#378 Posted by: janpom Posted at: 2018-11-01T21:57:51.591Z Reads: 208

```
Some chips came in today. I pre-programmed the FW on all to check that the bootloader is correctly burned and that the chips work OK. All worked fine. So far so good.

Here's Dave breadboard edition. :slight_smile: 

![IMG_1501|666x500](upload://mQGdCHGvOKD3rRcdZgwRvZVooW5.jpeg) 

I have simple labelling for chips. One white dot = bootloader burned. Two white dots = bootloader burned + FW pre-installed. So please don't be surprised if you receive a dotted chip. That actually means all is good. :smile:
```

---
## \#379 Posted by: bsancken Posted at: 2018-11-01T22:36:55.748Z Reads: 203

```
What is the UART connector that is used on Focboxes? I did a brief search bit didn't find a definite answer. 

(relevant to this thread for the UART connection, for those that would be making their own wiring harness)
```

---
## \#380 Posted by: deucesdown Posted at: 2018-11-02T04:39:04.306Z Reads: 199

```
JST PH 2.0mm
```

---
## \#381 Posted by: amazingdave Posted at: 2018-11-02T15:16:29.461Z Reads: 197

```
Am I too late to help with the beta test phase? I’ve got 2 screens on the way and am happy to populate a blank board.....
```

---
## \#382 Posted by: Kug3lis Posted at: 2018-11-02T15:17:35.621Z Reads: 193

```
Gerber files are online you can order pcb for few dollars from like http://allpcb.com/ https://jlcpcb.com/ for like under 10$ with shipping
```

---
## \#383 Posted by: janpom Posted at: 2018-11-02T18:17:35.405Z Reads: 192

```
Gerbers can now be downloaded from https://github.com/janpom/davega/tree/master/gerbers. The v0.3 has a few tweaks. See https://github.com/janpom/davega/blob/master/CHANGELOG_PCB
```

---
## \#384 Posted by: Pimousse Posted at: 2018-11-02T22:39:25.154Z Reads: 204

```
Hi @janpom, I'm digging into coulomb counting as well as SoC instead of voltage measurement.
I see that in your FW you define `VOLTAGE_WEIGHT` as 40% of the part of SoC in the computation.
WHy ? Coulomb counting isn't reliable enough ?

On my side, I'm planning to calculate the real usable capacity of the battery (like do smartphones IIRC) for a more accurate SoC.
Say you have a 10Ah rated battery but for protective purpose, you set a "high" cutoff. Perhaps, you could then only use 8Ah over 10.
If you detect a voltage corresponding to the cutoff end, you save the current total discharged mAh as the new (real) capacity of the battery.

What are your thoughts about this ?

Thanks Sir and again, really nice job done on this gadget ! Love it.
You actually kicked my ass to go further on my SmartRing :smile:
```

---
## \#385 Posted by: Kug3lis Posted at: 2018-11-02T23:26:28.407Z Reads: 210

```
Sorry and not, but I am not working anymore on the PCB, started working on RGB controller with Dave code, but it wasn't fitting on Arduino anymore, so I dropped the idea, and went bit more feature wise device on different platform. 

I moved to ESP32 platform which will let me fill up this device with tons of features like WiFi/Bluetooth/GPS/SD card/VESC integration/VESC data output for Firefly and other things.

WiFi for connecting to predefined list of AP or acting as AP to allow control settings, download logs, upload scripts, and provide TCP bridge for VESC tool.

Bluetooth with option to provide some fields from multiple VESC combined for that real battery consumption and etc not 2x.

Data logging to microSD card every time it powers up it will include GPS data if module is present and all other telemetry data.

Ws2812b (NeoPixel) control support.

LCD for outputing some telemetry data and custom screens.

and the most fun feature I think it is scriptability (small Javascript engine). Ability to create custom scenes for RGB/LCD and etc things with data from VESC/GPS and etc) 

![image|500x500](upload://4Fy5V9oO44tSz67gNK5hQGH57ib.jpeg) 

This is where I think we could cooperate with @janpom on providing best LCD experience as he has more experience in this.

I really would like to thank @janpom for triggering this idea and I would loved to cooperate with him on this project, as I am going to make it open source and provide ready to use kits + DIY kits

So I will try code in these days some basic feature set and come back for input regarding it :)

Sorry for over taking this topic with unrelated stuff, but I just wanted to share my idea and maybe in feature DAVE will also run inside it :D
```

---
## \#386 Posted by: janpom Posted at: 2018-11-03T14:11:44.674Z Reads: 206

```
Hi @Pimousse, first, thanks for the nice compliments!

About the `VOLTAGE_WEIGHT`, the 40% is pretty arbitrary. I just thought the Coulomb counter should have higher weight than the voltage.

As for reliability, I haven't done statistically significant amount of testing, but so far both voltage and Coulomb counting work as good SoC indicators for me. On my last ride, I ended up with 1235 out of 8000 mAh left and my LiPo batteries were almost completely flat based on voltage (total 12s voltage was 41V and one cell was below 3.3V when I then measured with my multimeter at home). 1235 is some 15% of 8000 so that's 85% of total capacity used. It's often said that the usable capacity of a battery is around 80% so this is more or less in line with that. Note that this is still with getting the readings from only one ESCape and multiplying by two.

I would be rather worried of doing automatic capacity calibration based on the cutoff voltage. The battery voltage tends be unstable. It drops under load. It may raise if you let the batteries rest for a bit after riding. I think the auto-calibrating logic would have to be rather clever to work reasonably well. From my current experience, this doesn't seem worth the trouble. But then again, my experience is still limited, so please take that with a grain of salt.

Glad to hear I made you make more progress on the SmartRing. The SmartRing looks really cool and I imagine the LEDs are much brighter and thus easier to read than the Dave display. The only thing I would be missing on it is the ability to do more accurate readings, such as exact voltage or exact distance traveled. That was actually the reason I started on Dave. There's unused round space inside of the SmartRing. If you could somehow squeeze an LCD display in there (maybe a smart watch round display?), that would be perfect!
```

---
## \#387 Posted by: janpom Posted at: 2018-11-03T17:19:44.948Z Reads: 197

```
@Kug3lis That sounds ambitious. I think you'll have significant feature overlap with the mobile apps that connect to VESC via bluetooth, such as Meter Pro. And with all the bells and whistles you're proposing, I imagine the price will easily grow beyond the Meter Pro price tag. IMO it will be tough to compete. This is not meant to discourage you though. It could still be a cool gadget.

I'm actually thinking of directing my next steps in the exact opposite direction. Reduce the features, make it even smaller and even cheaper. I like minimalism. :slight_smile:
```

---
## \#388 Posted by: janpom Posted at: 2018-11-03T17:43:34.478Z Reads: 198

```
Looking for some crowd wisdom regarding the Coulomb counter. Currently, the mAh counter starts at the full capacity and counts down. For example, with my 8000 mAh battery back, if I fully charge the batteries, the counter gets reset to 8000 and counts down as the battery discharges. The value around 1600 then indicates the batteries are almost flat because the usable battery capacity is only about 80%. I think this is kinda weird.

Wouldn't it be better to start counting from the usable capacity instead? In the example above it would mean the counter would start at 6400 mAh (80%) and count down to zero. Zero would then indicate (almost) flat batteries. It could potentially go to negative numbers if you push it, but that doesn't seem much of a problem to me. Note that the usable capacity [can already be configured](https://github.com/janpom/davega/blob/master/davega.ino#L40).

Related: What would be the best behaviour if you only partially charge the batteries? Currently, that use case is completely ignored. If you don't charge to at least 97% of max voltage (configurable), the mAh counter doesn't get reset and it will then show wrong values. That's not great, but then again, I didn't think many would charge batteries without going to fully charged and I didn't want to spend time implementing something nobody would use. Another reason was that I wasn't really sure what would be the best thing to do in such a case.

My best idea so far is this: If we detect batteries have been charged (voltage went up at least 1%, configurable), estimate the SoC from the voltage and set the remaining mAh accordingly. I'm slightly reluctant to implement this since there could be false positives that just mess up the Coulomb counter. For example, you end a ride with 48V and 6000 mAh. Then you switch the board off, let the batteries rest for a bit, switch it on again, the voltage will go up to 48.5, Dave will think the batteries got charged and will increase the mAh, e.g. to 6200 mAh, which is not what we want. Any thoughts about this?
```

---
## \#389 Posted by: Okami Posted at: 2018-11-03T19:33:24.749Z Reads: 196

```
U bring up interesting topic. 

I guess the only reliable way would be to have a feedback / connection with charger but i suppose this is not easily possible.

About the guess work.. I guess if it was possible to 'map' battery's state of charge based on what voltage it has, that would be great..

Though this would require to do a full charge and full discharge cycle and it would partly rely on voltage being linear to capacity left in watthours/amphours. 

Another thing I see here, is that temperature difference might throw off this 'reading' also..

As it can vary capacity of battery but i havent really tested this much, I guess in colder weather voltage would drop faster, so capacity should be decreased more drastically also..

Of course this is no problem for warm weather riders, as battery state should hold similar then, I think.

But might be considered if full battery is taken in summer and same values used in colder weather..

---

Thinking about this in details, it seems it is not as easy to get reliable estimate of battery life left, especially if one wants to guess who many miles / kilometers can u still do with remaining battery 

Ive thought about getting coulomb counter meter but havent it done yet.. for all i know u set max battery in amp/watthours. 

Then it just reduces that as u go.. then if one is clever enough he can deduct how much range he has left based on that

---

In conclusion.. I think it is best if user sets battery capacity himself, then the meter decreases from this count.. if u could set 20km of ride for full battery, then i guess it would be even possible to have 'estimated range left' also shown (50% battery left, 10km range).
```

---
## \#390 Posted by: janpom Posted at: 2018-11-04T22:00:52.409Z Reads: 194

```
Added a small update. Average cell voltage can now be optionally displayed instead of the total voltage. I personally don't have a good intuition of how my battery pack total voltage compares to SoC and end up dividing it by the number of cells in my head all the time. So the avg cell voltage will work much better for myself.

![IMG_1502|361x500](upload://fUKQPePBkD8yvIxpDbWq3mhu8kM.jpeg) 

Never mind the `rD6EC`. That's just the revision number. There will be the version number at that place for released FW versions.
```

---
## \#391 Posted by: brenternet Posted at: 2018-11-04T22:09:37.049Z Reads: 184

```
Out of interest I rarely charge my batteries to full. I stop at about 90%.
```

---
## \#392 Posted by: bigben Posted at: 2018-11-04T22:21:14.674Z Reads: 189

```
I am a relative simpleton when it comes to programming and the like, but. Would it be possible to configure the screen like this?![49|269x331](upload://rYhwVnsd2nRc8DVb9xGiCfeyQeR.png) 
Battery at the top and big speed?
(programming not my thing but look at my graphics skills)
```

---
## \#393 Posted by: janpom Posted at: 2018-11-04T22:38:13.112Z Reads: 186

```
That's good feedback. I'll think about how to best address such use case. There's a lot that could already be done with the available config options. For example, you could set your max voltage to 90% of the fully charged voltage and reduce the battery mAh in the settings as well, but that's a bit hackish. It wouldn't work correctly if you then occasionally charge to 100% instead of 90%. I'll figure something out.
```

---
## \#394 Posted by: janpom Posted at: 2018-11-04T22:40:51.686Z Reads: 184

```
Lovely! :smile: Yes, this is possible. I can make a skin like that. Do you insist on that particular font? :smile:
```

---
## \#395 Posted by: bigben Posted at: 2018-11-04T22:55:28.353Z Reads: 187

```
Has to be that bespoke font or it just won't work...:rofl:

The bar as in the real one could go around the edge but change from red to green as the battery discharged?
```

---
## \#396 Posted by: JonathanLau1983 Posted at: 2018-11-04T23:16:31.790Z Reads: 189

```
Average voltage is a smashing idea. Much harder to divide by 12 on the fly.
```

---
## \#397 Posted by: Blix Posted at: 2018-11-05T00:10:22.692Z Reads: 190

```
![davega9|690x443](upload://udsPWzt7ImZ5TUBknOyX8oxt0fl.png)
```

---
## \#398 Posted by: janpom Posted at: 2018-11-05T06:53:41.643Z Reads: 190

```
[quote="bigben, post:395, topic:71509"]
The bar as in the real one could go around the edge but change from red to green as the battery discharged?
[/quote]

How is that different from the current? Do you want all the cells to change color?
```

---
## \#399 Posted by: rpasichnyk Posted at: 2018-11-05T08:21:37.585Z Reads: 189

```
I recommend looking at DieBieMS https://github.com/DieBieEngineering/DieBieMS, because it does exactly what you are after. The easiest solution would be just to add it to your build and get state of charge % value via CAN. Or you can look at the source code how it's done and hopefully adjust so it works on your device without hooking up the DieBieMS.
```

---
## \#400 Posted by: janpom Posted at: 2018-11-05T09:01:18.626Z Reads: 194

```
First, thanks for chiming in, @rpasichnyk. 

[quote="rpasichnyk, post:399, topic:71509"]
The easiest solution would be just to add it to your build and get state of charge % value via CAN.
[/quote]

That might indeed be the easiest solution for me but then again not everyone has DieBieMS.

I believe DieBieMS has a complete control over the battery pack and it knows exactly when it's being charged so it's not a problem for it to keep track of the remaining mAh correctly. That's in contrast with Dave. Dave connects to the system via ESC and will typically be powered off when the battery pack is being charged. So it has to do some guesswork regarding the remaining mAh once it gets powered on and detects that the batteries have been charged. Unlike DieBieMS, it doesn't see the mAh coming in via the charger. It can only see the mAh coming out and in (recuperation) while riding.

Dave will work best for people who always charge their battery pack to 100%. Then it simply resets the Coulomb counter to the battery capacity. No guesswork needed.

It won't work so well for people who charge to less than 100% since then the Coulomb counter state will have to be estimated from the voltage after charging and that will lead to some inaccuracy. This will have to be accepted as a fact. Dave is just a simple device and I don't plan to make it more complicated. There more advanced (and more expensive) solutions for those who want more features, such as the DieBieMS and your Meter Pro.
```

---
## \#401 Posted by: brenternet Posted at: 2018-11-05T09:44:10.650Z Reads: 188

```
I can accept that, it was always the direction of this project to keep it simple and inexpensive.

Perhaps we could have a skin that ignores battery status and focuses on odometer and other features to maximise screen space. I'm alright with getting my battery info elsewhere.
```

---
## \#402 Posted by: janpom Posted at: 2018-11-05T09:46:38.038Z Reads: 183

```
Sure, that's possible. Or you could ignore the coulomb counter and only get SoC estimates from the battery voltage. That can already be configured.
```

---
## \#403 Posted by: Zentaria Posted at: 2018-11-05T09:58:31.668Z Reads: 180

```
Would be cool if this would be wireless, so I could Stick it into my remote.
```

---
## \#404 Posted by: b264 Posted at: 2018-11-05T09:59:36.969Z Reads: 183

```
[quote="Battosaii, post:349, topic:71509, full:true"]
For a carpenter for example its much easier to find exact measurements on a measuring tape in feet than it is in CM.
[/quote]

You must be smoking the good shit.  Metric is waaaay easier.  And this is coming from someone in Freedom Units Land.
```

---
## \#405 Posted by: brenternet Posted at: 2018-11-05T10:00:23.273Z Reads: 171

```
Don't bring this up again haha.

We're all different and were all special flowers
```

---
## \#406 Posted by: janpom Posted at: 2018-11-05T10:01:03.458Z Reads: 173

```
That probably won't happen any time soon. But then again, why not use the Firefly, or at least take the display and FW from it. It's open source.
```

---
## \#407 Posted by: Pimousse Posted at: 2018-11-05T10:17:13.811Z Reads: 191

```
Hi @janpom, nice to debate ideas about algorithm ! Love that !
Few inputs :

Ok, so first, I had a ride yesterday concluded by a reached cutoff end (3,5V/cell).
5 hours later, the battery was 3,7V/cell (average, some were 3,6V, but I know I have weaker cells).

:arrow_forward: This corroborates what you said about triggering a "real capacity" although I'm thinking to memorize the "low battery" status to avoid having the board going back into "yes, you're fine dude, go ahead for 10 km more !" after resting a bit.

Then, I charged my 12Ah back at home. I filled 10Ah in. 

:arrow_forward: Another stuff that corroborates your "80% real capacity" rule-of-thumb.

[quote="janpom, post:386, topic:71509"]
There’s unused round space inside of the SmartRing. If you could somehow squeeze an LCD display in there (maybe a smart watch round display?), that would be perfect!
[/quote]

Ahaha, funny you mentioned it ! I had the same thought and already had a quick search for a round screen, but no luck to find a ready-to-use display (I mean I2C/SPI display, not a raw one which will require to build a driver for hooking to Arduino).

Also, as you said
[quote="janpom, post:387, topic:71509"]
I like minimalism.
[/quote]
Me too, and the flat deisgn of the WS2812 ring is exactly what I want for keeping away this [KITT feeling](https://en.wikipedia.org/wiki/KITT#/media/File:KITT_Interior_at_Toronto_Auto_Show_2011.jpg).
Less is more. :slight_smile:

For more, bluetooth and @rpasichnyk 's app is the way to go.

Please, keep up the good work and share your feelings and algorithm thoughts, this is really interesting !
```

---
## \#408 Posted by: JonathanLau1983 Posted at: 2018-11-05T11:43:41.681Z Reads: 184

```
![image|690x460](upload://57mFqdS64jxMGmYPm6nRMRqsDFS.jpeg) 
Bring on the PCB
```

---
## \#409 Posted by: Pedrodemio Posted at: 2018-11-05T12:53:14.041Z Reads: 183

```
What I do for my board is use an expression extracted from a 0.2C discharge from https://lygte-info.dk/ and from initial resting voltage determine how much charge is left

For now I'm relying just on voltage, but you can easily determine the energy the same way and them start to subtract with the consumed Wh you get from the VESC

Also I only update the values when the current in or out of the battery is 0 for a few seconds to allow the voltage to come near resting voltage

Works like a charm
```

---
## \#410 Posted by: SeanHacker Posted at: 2018-11-05T15:50:49.849Z Reads: 187

```
So I bought an arduino uno locally (my first!) and I'm brand new in the arduino world so any help or advice is welcome. All my parts for davega should be here today or tomorrow (maybe the pcb too) and I can't wait. I figured I'd test uploading and practice on this uno to see how it goes. @janpom it looks like it's missing a header file for the display? Or am I missing something?
 
davega_display.h:23:28: error: TFT_22_ILI9225.h: No such file or directory
compilation terminated.
exit status 1
TFT_22_ILI9225.h: No such file or directory
```

---
## \#411 Posted by: janpom Posted at: 2018-11-05T19:08:58.020Z Reads: 190

```
@SeahHacker Ah, good catch. You need to install the TFT_22_ILI9225 library. You can get it from https://github.com/Nkawu/TFT_22_ILI9225 (Clone or download > Download ZIP). Here's [how to install](https://www.arduino.cc/en/Guide/Libraries#toc4).

I'll update the README file in davega repo.
```

---
## \#412 Posted by: SeanHacker Posted at: 2018-11-05T20:11:50.704Z Reads: 193

```
Nice. Thanks for being so responsive dude. 

Parts are coming in pretty quick thanks to Amazon prime. Just waiting for a few more things and I'll have everything I need. Another question. Can I test this out with the arduino uno? Or should I just wait for the PCB and the rest to get here?

![IMG_20181105_112433|665x500](upload://stU6TJkciISD0fDp4jZNcXCA4Gz.jpeg)
```

---
## \#413 Posted by: janpom Posted at: 2018-11-05T20:17:34.316Z Reads: 182

```
Sure, you can test it with the UNO. [Here's](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/209?u=janpom) how to wire it up. For starters, you can ignore the buttons and the VESC. Just connect the display to the UNO. The pins are the same as on the Nano.
```

---
## \#414 Posted by: Mich21050 Posted at: 2018-11-05T20:18:26.892Z Reads: 181

```
@janpom Do you still have some pcbs? :smile:
```

---
## \#415 Posted by: janpom Posted at: 2018-11-05T20:23:26.578Z Reads: 185

```
@Mich21050 Sorry, I don't have more to be sold alone. I need to keep enough for the kits. The kits could be ready to ship in a week or two.

@CarbonV might have a few PCBs to spare.
```

---
## \#416 Posted by: SeanHacker Posted at: 2018-11-05T21:53:18.209Z Reads: 187

```
![IMG_20181105_132726|375x500](upload://ziH8UPmdTpyq5dT1DcgMaQDik3g.jpeg)
```

---
## \#417 Posted by: janpom Posted at: 2018-11-05T21:56:45.014Z Reads: 174

```
Nice! :) Do you get anything on the display with the Dave FW? It should still draw the initial screen even if no ESC is connected.
```

---
## \#418 Posted by: SeanHacker Posted at: 2018-11-05T22:34:12.959Z Reads: 185

```
I just tried. I get white screen so far after upload. 

![IMG_20181105_143246|375x500](upload://kBaKhUsHn8dSZWIX6GZdIt3Rds3.jpeg)
```

---
## \#419 Posted by: janpom Posted at: 2018-11-06T06:49:06.445Z Reads: 179

```
Please double check you have it wired up correctly. The wiring that worked for your test sketch may be different from the wiring expected by Dave.
```

---
## \#420 Posted by: pixelsilva Posted at: 2018-11-06T07:03:13.613Z Reads: 181

```
Our friend @Battosaii running the less traveled Imperial System road...

https://media.giphy.com/media/TWiBZnJHDUZFe/giphy.gif
```

---
## \#421 Posted by: Bokard Posted at: 2018-11-06T13:20:22.488Z Reads: 189

```
![IMG_20181106_141807|375x500](upload://lWmHqB5Umm0NsshJ6iLwwspEAv4.jpeg)

😍😍😍
```

---
## \#422 Posted by: SeanHacker Posted at: 2018-11-06T23:20:57.259Z Reads: 194

```
Hey guys. I just got home and want to do some testing. But for some reason I can get this wiring correct. It's really bugging me. Can one of you treat me like a baby and point with arrows or something where I need to connect the wiring to this uno? I tried the nano diagram but it seems like the numbers are wrong. Maybe I'm just an idiot. Not sure. ;)

![IMG_20181106_145707|665x500](upload://cghJ7wmWuQGWytFMC9QuVVuEW9n.jpeg) 

On another note. I started prototyping a case (without any dimension at all) for this thing out of acrylic. I've never made anything like this and it was pretty fun. It's really ruff at the moment.

![IMG_20181106_151138|375x500](upload://z2RLGW8kqhDoohUXXQyKa5hRfcv.jpeg) ![IMG_20181106_151108|375x500](upload://aY7aIWfjCSY21RD91AhoH3hIKZz.jpeg) ![IMG_20181106_151044|375x500](upload://yxmfZCr19y1MvblcxkUmsHFaJmx.jpeg)
```

---
## \#423 Posted by: SeanHacker Posted at: 2018-11-07T01:24:46.575Z Reads: 189

```
Oh hi! :slight_smile: 

![IMG_20181106_172153|375x500](upload://pB0HH4q0nd54Lq4e4PpQ7iX0JYu.jpeg)
```

---
## \#424 Posted by: janpom Posted at: 2018-11-07T01:55:28.034Z Reads: 188

```
Yay! :wink:
```

---
## \#425 Posted by: SeanHacker Posted at: 2018-11-07T01:59:52.483Z Reads: 184

```
The rest of the stuff I ordered should be here Thursday or Friday and hopefully the pcb's too. Ordering a couple more screens so I can have one of these on all my boards. This little gadget is getting expensive on amazon. lol. This is pretty awesome dude. Thanks again!
```

---
## \#426 Posted by: lrdesigns Posted at: 2018-11-07T02:03:34.204Z Reads: 185

```
[quote="SeanHacker, post:422, topic:71509"]
Can one of you treat me like a baby and point with arrows or something where I need to connect the wiring to this uno?
[/quote]

Hey Sean, since you figured it out mind making a map for the rest of us dummies? I think many people have an uno laying around somewhere.
```

---
## \#427 Posted by: SeanHacker Posted at: 2018-11-07T02:18:21.511Z Reads: 190

```
No problem dude. 

CLK - 13
SDI - ~11
RS - ~9
RST - 12
CS - ~10

![uno_wiring|690x460](upload://vSaqIp9aoez9IDCGstFRI109v6T.jpeg)
```

---
## \#428 Posted by: lrdesigns Posted at: 2018-11-07T03:56:15.675Z Reads: 190

```
YES! :man_dancing: My LCD just came in!

![IMG_1118|666x500](upload://z8suvytoHmHwWzcIzui1fwgowgy.jpeg) 

The bolt holes on my case are too narrow on the width by about 2mm. So I double checked the [drawing janpom provided above](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/129?u=lrdesigns) against my CAD and it was my CAD that was off.  

Time for a design revision, also going to try to slim the overall thickness down.
```

---
## \#429 Posted by: janpom Posted at: 2018-11-07T08:51:34.198Z Reads: 181

```
@SeanHacker The pinout in your post is incorrect. Please correct it so that it doesn't confuse people.

It's best to retrieve the correct pinout [directly from the code](https://github.com/janpom/davega/blob/master/davega_display.cpp#L24). 

You clearly wired up correctly, but you made a few mistakes when writing it down:
- CS is 10 (not 9)
- SDI is 11 (not 10)
```

---
## \#430 Posted by: janpom Posted at: 2018-11-07T08:56:47.677Z Reads: 177

```
@bsancken @Bokard: Guys, have your PCBs arrived yet? They should have. @lrdesigns already received his in Hong Kong.
```

---
## \#431 Posted by: Bokard Posted at: 2018-11-07T08:58:20.237Z Reads: 170

```
Yeah just yesterday ^^
```

---
## \#432 Posted by: janpom Posted at: 2018-11-07T09:00:12.274Z Reads: 177

```
Ah, sorry. You actually posted the pics here. I lost track.

And @bsancken is actually in US, same as @SeanHacker, so it makes sense theirs haven't arrived yet. Hopefully they are coming soon. All that went to EU are already delivered and the one to Hong Kong as well. So far so good.
```

---
## \#433 Posted by: ARetardedPillow Posted at: 2018-11-07T11:15:24.265Z Reads: 170

```
Agh I'm late in the game, just started reading this thread now and I want this sooo bad, where do I start?
```

---
## \#434 Posted by: Andy87 Posted at: 2018-11-07T11:16:16.752Z Reads: 169

```
order some displays and add your like on the poll to get a set later
```

---
## \#435 Posted by: ARetardedPillow Posted at: 2018-11-07T11:16:59.536Z Reads: 174

```
I think this is a scam for likes!
```

---
## \#436 Posted by: Andy87 Posted at: 2018-11-07T11:18:29.020Z Reads: 182

```
https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/36?u=andy87
```

---
## \#437 Posted by: clistpdx Posted at: 2018-11-07T16:25:21.011Z Reads: 171

```
I scanned this thread but couldn't find an STL file anywhere. Has anyone posted a case for this yet? Or is @mmaner working on one but it's just not ready yet?
```

---
## \#438 Posted by: janpom Posted at: 2018-11-07T16:28:12.268Z Reads: 171

```
There's this by @lrdesigns: https://www.thingiverse.com/thing:3171000/files, but it's just a prototype. The dimensions probably need some adjusting.

@mmaner hasn't made the STL available yet. He's waiting to get Dave on hand so that he can adjust the dimensions as well.
```

---
## \#439 Posted by: mmaner Posted at: 2018-11-07T16:34:47.833Z Reads: 174

```
There is a couple posted, I'm waiting on components before I release mine as I'm not sure of the fit yet.  My components should start arriving today.
```

---
## \#440 Posted by: Bokard Posted at: 2018-11-07T17:26:10.316Z Reads: 171

```
I'm drawing something up too but waiting for the last few components
```

---
## \#441 Posted by: SeanHacker Posted at: 2018-11-07T23:35:50.897Z Reads: 188

```
PCBs made it here. Thanks again @janpom. This is going to be fun! Still just waiting for some parts to get here in the next day or so hopefully. :smile:

![IMG_20181107_150920|665x500](upload://9Gq0DIdVwh5N4qXjmzcUTtpW4H1.jpeg) 
![IMG_20181107_150920|665x500](upload://9Gq0DIdVwh5N4qXjmzcUTtpW4H1.jpeg) 

Also made some progress on a case but I think I'm just going to end up getting someone to 3D print me one when the boys come up with something. 

![IMG_20181107_151951|665x500](upload://soOkTX69hFVptSMFa6uY63JYFjx.jpeg) ![IMG_20181107_152716|665x500](upload://kZZkLA2HY3KAW1VgR6Fgw1lN1ny.jpeg) ![IMG_20181107_152556|665x500](upload://gpRU67ZpIis1wPIBKV8IvUGv8DN.jpeg)
```

---
## \#442 Posted by: lrdesigns Posted at: 2018-11-07T23:41:03.144Z Reads: 174

```
@clistpdx don’t download mine yet, wait till I confirm fitment. Just printing new version now. Probably couple more version till it’s good.
```

---
## \#443 Posted by: lrdesigns Posted at: 2018-11-08T01:51:31.210Z Reads: 183

```
Construction started! 

One thing I noticed was that the crystal hits the LCD IC, and the programming header hits the SD card slot. So if there is a V2, maybe these could move and the assembly could be about 2mm thinner. 
![image|690x230](upload://hboW5g3ucP6lKmQEEAsfwYrz9Ss.jpeg) 

First thing I did was drill out the 2mm holes to 3mm. The holes seem to line up pretty well with the LCD. 

![IMG_1133|666x500](upload://kC6FqeNnmtXuz76Z3iAG8jYKxq9.jpeg) 

![IMG_1135|666x500](upload://pdVyxH8xVYo1jfDbpOBKLjRaF0s.jpeg) 

![IMG_1136|666x500](upload://1Nt8uJnxFjPab26Pkhs4H7xYZyk.jpeg) 

![IMG_1134|375x500](upload://o1E8vJPthGYOSsRlJU3SjVJT8K1.jpeg)

Edit, Bugger! Just noticed my programing header is offset one hole. :pensive:
```

---
## \#444 Posted by: ARetardedPillow Posted at: 2018-11-08T03:46:36.777Z Reads: 179

```
Where do I pay?? Take my money dammit
```

---
## \#445 Posted by: janpom Posted at: 2018-11-08T08:10:35.555Z Reads: 179

```
@SeanHacker Cool that the PCBs arrived. So that's some 11 days for shipping to US. Good to know.

Nice work on the acrylic enclosure. I actually thought about doing the same, but then I went for cardboard instead. Not pretty, but easy to work with and it does the job.

What button is that? Is that rubber coating?
```

---
## \#446 Posted by: janpom Posted at: 2018-11-08T08:34:02.061Z Reads: 187

```
[quote="lrdesigns, post:443, topic:71509"]
Just noticed my programing header is offset one hole.
[/quote]

Yeah, I was about to tell you. It shouldn't be hard to desolder if you have a solder wick. I think I have sent you a spare header. If you can't desolder it as a whole, you can cut all the pins. Then you can desolder them one by one, which is much easier.

[quote="lrdesigns, post:443, topic:71509"]
One thing I noticed was that the crystal hits the LCD IC, and the programming header hits the SD card slot.
[/quote]

I'm aware of that. The crystal is already fixed in [v0.3](https://github.com/janpom/davega/blob/master/CHANGELOG_PCB):

![Selection_004|512x323](upload://gLYyq2IKQxTPFi2Y4R7sIpSBkob.png) 

The header is not a problem, IMO. It actually doubles as a spacer -- keeps the two PCBs parallel to each other. Also, you have a hair of space underneath the header.

The best way to solder it on is if you solder only a single pin first. Then take the PCB in your left hand, press the header firmly against the PCB and re-heat the soldered pin. Then let it cool while still pressing firmly. It won't move after that and you can solder the remaining pins next. That way you don't get any space under the header.

[quote="lrdesigns, post:443, topic:71509"]
So if there is a V2, maybe these could move and the assembly could be about 2mm thinner.
[/quote]

I don't believe that. You definitely don't have 2mm of clearance above the MCU. If the crystal is moved and the header is not soldered on (you can make a harness instead), you can maybe make it 0.5mm thinner, but no more than that.

The crystal only touches the plastic housing of the chip. It won't short anything. I still didn't like it so I moved it for the next version, but I honestly don't think it's a big deal.
```

---
## \#447 Posted by: Pimousse Posted at: 2018-11-08T10:23:07.350Z Reads: 173

```
Nice to see the progress !
It seems that there is a lot of space left on the PCB.
Would it be nice to add a NTC on the PCB for having the external temperature ? 
You probably have some spare ADC on the Atmega.
Just trhowing ideas for v0.3 :smile:
```

---
## \#448 Posted by: JonathanLau1983 Posted at: 2018-11-08T10:46:41.324Z Reads: 166

```
That sounds like a nice idea, I've got some 10k Thermistors kicking around.
```

---
## \#449 Posted by: SeanHacker Posted at: 2018-11-08T11:31:10.511Z Reads: 172

```
They're some breadboard buttons that my buddy gave me. He said he got them from Amazon. https://www.amazon.com/gp/aw/d/B06XT3FLVM?psc=1&ref=yo_pop_mb_pd_title
```

---
## \#450 Posted by: SeanHacker Posted at: 2018-11-08T22:17:29.823Z Reads: 186

```
Damn I hate waiting for these parts to come in. I really wanna use this thing already. 

Added a clear acrylic piece to cover the screen on my prototype enclosure. I just taped everything in, so that why its a little wonky looking. 

![IMG_20181108_134452|375x500](upload://lEDZBB2gTVGC9SDEg7rwIszx4zz.jpeg) ![IMG_20181108_141336|375x500](upload://32a5azivDkikszhvPLns4oJQQt7.jpeg)
```

---
## \#451 Posted by: janpom Posted at: 2018-11-08T22:23:24.380Z Reads: 179

```
Nice! In fact, the parts that you're missing are only needed to reset the chip while programming. You can program the chip using your arduino. Then you're good. The only problem is that once you solder on the display, it will be very difficult for you to solder additional components.
```

---
## \#452 Posted by: SeanHacker Posted at: 2018-11-08T23:02:44.410Z Reads: 184

```
I'm actually waiting for the chips to come in still. They were supposed to be here on Sunday but something happened. So from what it looks like they should be here tomorrow along with the rest of the components. 

Question. Its not bad to bend these 20pf capacitors like this is it?

![IMG_20181108_145459|375x500](upload://w8Cx3rgPxT8pCOEYHiBw32S4A4x.jpeg)
```

---
## \#453 Posted by: janpom Posted at: 2018-11-08T23:24:48.993Z Reads: 174

```
Aha, I remembered seeing the MCU with crystal and caps on one of the pics and I thought that one was from you, but I was wrong, sorry (it was from JonathanLau1983).

As for the capacitors, it's probably not ideal, but I have done the same with mine and haven't had any problems so far. I ordered [these](https://www.aliexpress.com/item/50PC-Monolithic-Capacitor-101-102-103-104-220-330-50V-100PF-1NF-10NF-0-1UF-22P/32865098104.html?spm=a2g0s.9042311.0.0.373e4c4d5j6dXp) for the kits, which are smaller and I hope they will fit without bending. You could also use SMD capacitors like [here](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/443?u=janpom).
```

---
## \#454 Posted by: janpom Posted at: 2018-11-09T08:56:15.815Z Reads: 172

```
@Pimousse Thanks for the idea. I prefer to keep it small, but I encourage anyone to experiment with add-ons. You could fork my PCB design on EasyEDA and add anything you want to it. Then order from JLCPCB. For 10 PCBs it's some $8 shipped if you don't mind waiting a bit.
```

---
## \#455 Posted by: BigBrit Posted at: 2018-11-09T09:02:09.529Z Reads: 177

```
Its not bad at all to bend the capacitors, it will have no effect to their operation
```

---
## \#456 Posted by: JonathanLau1983 Posted at: 2018-11-09T09:03:58.720Z Reads: 175

```
I'm probably going to blob on some hot glue to stop vibrations from potentially breaking their little legs.
```

---
## \#457 Posted by: Pimousse Posted at: 2018-11-09T09:09:42.678Z Reads: 174

```
You think you don't have not enough room for a NTC and another resistor on the actual size ?
That wouln't change the overall dimension. ;)
```

---
## \#458 Posted by: lrdesigns Posted at: 2018-11-09T09:17:44.578Z Reads: 172

```
Why do you need/want to know the temp of the DAVEga or the outside air? I want to know the temp of my motor or vesc which we already have with the fault notification. You could have current temp of motor and vesc with some software work, but the display might get crowded with too much info.
```

---
## \#459 Posted by: Pimousse Posted at: 2018-11-09T09:31:42.410Z Reads: 166

```
Oh, that was only thoughts.
Sure it requires to think about how this can be integrated with other data without messing UX up.
```

---
## \#460 Posted by: JonathanLau1983 Posted at: 2018-11-09T09:33:33.451Z Reads: 162

```
External temp sensor is more of a nicety.
So when your out and it's cold AF you know exactly how cold AF it is.
Beware black ice!
```

---
## \#461 Posted by: Andy87 Posted at: 2018-11-09T09:38:37.192Z Reads: 157

```
than we need peeping below 4degree too... :sweat_smile:
```

---
## \#462 Posted by: janpom Posted at: 2018-11-09T09:38:52.265Z Reads: 163

```
I meant "small" in terms of features, not necessarily physically small (though that's also a concern). Sorry for the ambiguity.

I like the UNIX system philosophy: Do one thing and do it well.
```

---
## \#463 Posted by: Pimousse Posted at: 2018-11-09T10:22:00.944Z Reads: 175

```
Ok, I get what you mean. You're right.
I would suggest to add it though on the PCB, not especially for external temp. but any kind of ADC measurement.
For instance, I hooked a NTC up in my battery box to the VESC ADC3 because I had the experience having very hot batteries after a continuous 10km uphill.
But nothing warned or stopped the VESC because of battery temperature (quite huge hazard !).
(Just throwing ideas, not forcing anything. :slight_smile: )
```

---
## \#464 Posted by: brenternet Posted at: 2018-11-09T10:42:36.532Z Reads: 177

```
As long as functionality is simple and doesnt detract from the main goal I'm all for it. A scrolling screen via small button would solve most of these issues. I have absolutely no idea if it can be implemented because I'm software impared but:

A general info screen, similar to the planned one now
A temp screen
A simplified speed screen
A simplified fault screen 
A simplified odometer screen

That way you could choose what is important to you at the time and when you stop for a break or beer or whatever you can scroll through all of them and look like a proper skateboard Aut.
```

---
## \#465 Posted by: janpom Posted at: 2018-11-09T11:48:29.915Z Reads: 171

```
The beauty of using the THT is that you can easily solder any additional sensors directly to the MCU pins.

I don't think it's worth it to make an designated space on the PCB for ADC add-ons since the size, number of pins, pin distance, etc would vary. However, I could route the unused ADC pins (and maybe the VCC and GND as well) to the border of the PCB so that the add-ons are easier to connect. These new pins could possibly replace the DEBUG pins, which I haven't even used myself yet and I actually don't think they are very useful after all.
```

---
## \#466 Posted by: janpom Posted at: 2018-11-09T11:59:30.875Z Reads: 175

```
Scrolling is complicated, but toggling between multiple screens with a button would be fairly easy and I do like the idea. In fact, I believe the display layout will be the most common thing people will want to customize. A good way to design this would be by making the display layout a pluggable module. People could then contribute various display layouts as plug-ins. The end-user would be able to select the layouts they like, register them all to their Dave FW and toggle between them with a button.

Since OOP (C++) is natively supported by Arduino, this would be easy to implement. It's a matter of defining a sharp interface for the display layout (which is already done to a large extent anyway) and have multiple implementations as class objects. Plus, class inheritance would come handy.
```

---
## \#467 Posted by: brenternet Posted at: 2018-11-09T12:00:29.885Z Reads: 169

```
I meant toggling haha. I don't need it to be fancy 🧚‍♂️
```

---
## \#468 Posted by: JonathanLau1983 Posted at: 2018-11-09T12:23:42.854Z Reads: 167

```
How about it switches between screens every couple second when stationary.
But when moving stays on speed/odometer screen.
```

---
## \#469 Posted by: SeanHacker Posted at: 2018-11-09T23:35:51.714Z Reads: 189

```
Alright. I think I have everything minus the 5 pin right angle. Those will be here tomorrow. I can't wait. 

![IMG_20181109_143716|375x500](upload://qAJqPlzP1UUKFXaE6FvcmKGTxkT.jpeg) ![IMG_20181109_152103|665x500](upload://dfR8iKSwm7n0DteRjhHlZIJygJJ.jpeg)
```

---
## \#470 Posted by: SeanHacker Posted at: 2018-11-09T23:54:30.294Z Reads: 185

```
Just noticed something. My screen seems to be different. These two guys are smashed against each other. I still have enough meat on the bone to solder. Is this going to be a problem @janpom?

![IMG_20181109_155250|375x500](upload://qI4PsMsIWnRw1DmYgMk3uBHRQqt.jpeg)
```

---
## \#471 Posted by: Skunk Posted at: 2018-11-10T00:08:11.237Z Reads: 184

```
Man these are really looking great.
Love seeing a community project like this.
We need way more things like this
```

---
## \#472 Posted by: janpom Posted at: 2018-11-10T19:00:07.715Z Reads: 182

```
@SeanHacker I looked at the pics of your display that you have posted. It's indeed different from mine. Is it 2.0" or 2.2"? Do the mounting holes align with the holes on the PCB?

I searched on AliExpress and found [this one](https://www.aliexpress.com/item/2-2-inch-Serial-port-TFT-screen-176X220-with-PCB-panel-ILI9225-LCD-color-display/32810066835.html?spm=2114.search0104.3.202.50fe3c97n0IzMc&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_319_317_10696_5728816_10084_453_454_10083_10618_10304_10307_10820_10821_537_10302_536_5733216_5733316_328_10059_10884_10887_5731016_100031_5733416_5730016_5733116_321_322_10103_5733516_5733616_5729016,searchweb201603_2,ppcSwitch_0&algo_expid=5ad3472b-de50-4950-bf57-4f8bdef19fc1-31&algo_pvid=5ad3472b-de50-4950-bf57-4f8bdef19fc1) that looks exactly as yours from the bottom. And that's the 2.2". If it worked with the Arduino, it should be all good, but if it's 2.2" it won't fit into the enclosures that @mmaner and @lrdesign are designing
```

---
## \#473 Posted by: mmaner Posted at: 2018-11-10T19:01:38.823Z Reads: 180

```
I got my display today, glad I didn't print a bunch. The display has a rim I didn't account for so I need to change the slot dimensions.
```

---
## \#474 Posted by: janpom Posted at: 2018-11-10T19:08:40.508Z Reads: 186

```
I have many updates. The most important is that the USB adapters arrived yesterday (the pile in the back) and with that I have all the major parts for the kits. I'm still waiting for crystals, resistors and capacitors, but those I can buy for cheap even in the local electronics shop, which I will do if it doesn't seem like the missing packages arrive in the next few days.

![DSC01651|587x500](upload://qYbqYmFVPEBxlaNnVyTlM3X9nAE.jpeg) 

I opened one of the USB adapters to inspect it. The quality doesn't look great. The USB connector is bent and there's some dirt on the PCB. You probably can't expect much for $1. I think I'll open and test all before shipping to people. It shouldn't take that long.

I'll start the thread for the first batch soon, maybe tomorrow.
```

---
## \#475 Posted by: SeanHacker Posted at: 2018-11-10T19:16:29.119Z Reads: 181

```
Yep. Looks like you're right. I ordered the 2.2". Dammit. Bought 3 of them too. lol. Probably just going to order some 2" later at some point. Let me know when you're selling your kits. I'll buy one or two from you also. ;)
```

---
## \#476 Posted by: janpom Posted at: 2018-11-10T19:25:21.245Z Reads: 182

```
I got these from a friend:

![IMG_1505|690x474](upload://y8n0OmAXGDq3Ah8Hi5lZsnZZ3vy.jpeg) 

It's just a test print and the print quality is pretty bad, but it was nice to be able to get hands on it and see how well Dave fits in. I like @lrdesign's design a lot. Simple and practical.

It would be nice to make it slightly slimmer, so that 20mm bolts can be used more easily. They work even with the current, but it's a very tight fit.

The space for 3mm protective glass seems a complete overkill to me. Even the 2mm acrylic I have purchased seems too much. I'm actually thinking if it wouldn't be best to go without any protective glass at all. It's not like the display is made of sugar and if it gets damaged, it gets damaged. It's 5 bucks.

If there's no protective glass it can be slimmer and it would be easier for people to make. Just print it, add bolts and nuts and done. No need to cut and glue glass. The display would probably be easier to read as well.

@lrdesigns, @mmaner: Any thoughts on without protective glass?
```

---
## \#477 Posted by: mmaner Posted at: 2018-11-10T19:33:56.433Z Reads: 178

```
[quote="janpom, post:476, topic:71509"]
If there’s no protective glass it can be slimmer and it would be easier for people to make.
[/quote]
im thinking the same thing.  the display looks tougher than i imagined it would be.
```

---
## \#478 Posted by: janpom Posted at: 2018-11-10T19:46:38.659Z Reads: 187

```
I've been using headers to connect my display to the PCB since the day one. Since I've been developing the thing, being able to access the PCB under the display was critical for me. I think it's actually a good feature to have for anyone. At the very least, you can easily replace the display if needs be.

The problem is that the headers add a lot to the thickness. I looked if there's something that could be done about it and turned there's a very simple solution. It's a matter of removing the yellow plastic and cutting the pins.

![IMG_1506|690x278](upload://fIhaZUZYdzXx0XJIDoqqONIGWSe.jpeg) 

It then still holds in the headers and allows for thin enough fit.

![IMG_1507|690x227](upload://bHVZwyvmcgKCrDM4uMczafqz1zI.jpeg)
```

---
## \#479 Posted by: janpom Posted at: 2018-11-10T19:52:35.173Z Reads: 179

```
[quote="SeanHacker, post:475, topic:71509"]
Let me know when you’re selling your kits. I’ll buy one or two from you also.
[/quote]

I'll post in here when I am. Note the kits will come without the display though, so you'll need to order the 2.0" anyway. Or you can just use the 2.2" for science. ;) You already have a nice enclosure for it anyway.
```

---
## \#480 Posted by: janpom Posted at: 2018-11-10T20:00:18.076Z Reads: 182

```
@SeanHacker One extra feature of the 2.2" display is that the brightness is customizable. You could add a jumper wire between the display LED pin and one of the PWM enabled pins on the MCU. Then in the Dave FW, specify that pin number [here](https://github.com/janpom/davega/blob/master/davega_display.cpp#L29) and adjust the brightness [here](https://github.com/janpom/davega/blob/master/davega_display.cpp#L31).
```

---
## \#481 Posted by: janpom Posted at: 2018-11-10T22:26:17.120Z Reads: 180

```
[Accepting orders](https://www.electric-skateboard.builders/t/davega-first-batch-beta-testing/74208)! :)
```

---
## \#482 Posted by: SeanHacker Posted at: 2018-11-12T02:36:15.202Z Reads: 173

```
@janpom

Can you post pics of your wiring to flash firmware to the board? For some reason all I get is "avrdude: stk500_recv(): programmer is not responding" when trying to flash the firmware from the programmer.
```

---
## \#483 Posted by: lrdesigns Posted at: 2018-11-12T04:28:04.411Z Reads: 186

```
[quote="janpom, post:476, topic:71509"]
Any thoughts on without protective glass?
[/quote]

I think it would be fine depending on your usage. The goal of my design is to be waterproof and robust. 3mm was overkill, now I have it with 2mm, but 1mm might be ok. The first iteration was quite thick overall as I was guessing many of the dimensions. 

I am hoping to laser cut some screens once the design is finalized. I just need to fix a friends laser cutter. 

The update now is 17mm thick for the top shell and 20mm bolts do fit now. 

![IMG_1237|375x500](upload://3qUDoE08o0ZllQAlxvkppfqE4VY.jpeg)
```

---
## \#484 Posted by: lrdesigns Posted at: 2018-11-12T06:43:27.541Z Reads: 187

```
Guys so excited!!

I figured out a way to test the LCD without soldering it on. I have not put on the external wires yet but really wanted to see if I could get it working and try the arduino stuff. I stuffed a tissue in the end which put pressure on all the pins for temporary testing. :grin:

![IMG_1240|666x500](upload://bpZVV2CvwwTY3v7aLV00UCh5PWr.jpeg) 

I had one issue compiling the sketch at first it said "davega_display.h" was not available. After I downloaded all the files the display.h was there but it was not in the davega folder. I moved all the extra files into there and it worked. I also needed to install the drivers for the programmer. 

![image|553x279](upload://9CuM8YLmFlddftuv7lVEX8LJfgt.png) 
![image|161x366](upload://lj52L2oTddjBLfy8AVqeqOZGlqn.png)
```

---
## \#485 Posted by: janpom Posted at: 2018-11-12T06:53:08.307Z Reads: 182

```
@SeanHacker It should be like this:

![IMG_1510|375x500](upload://cuDnQ2cbIILL1Zk2HAyRKw8R27G.jpeg) 

It would be best if you could post pics of how you have it wired up and I will try to tell you what's wrong with it.

Make sure you have the MCU and the diode correctly oriented.
```

---
## \#486 Posted by: janpom Posted at: 2018-11-12T07:01:34.286Z Reads: 180

```
@lrdesigns Awesome work! I purchased some female header pins for the display that I will ship with the next kits so that people don't have to use tissues. :smile:  I do like the creativity though! :smile:

[quote="lrdesigns, post:484, topic:71509"]
I had one issue compiling the sketch at first it said “davega_display.h” was not available. After I downloaded all the files the display.h was there but it was not in the davega folder. I moved all the extra files into there and it worked.
[/quote]

When you opened `davega.ino` for the first time, did it say something like it has to be located in a folder named `davega` and asked you if you wanted to move the file there?

[quote="lrdesigns, post:484, topic:71509"]
I also needed to install the drivers for the programmer.
[/quote]

Right. If you read the README file, the point 6 in [this section](https://github.com/janpom/davega/blob/master/README.md#configuring-and-installing-firmware) in particular, that shouldn't have caught you off guards. :wink:
```

---
## \#487 Posted by: bsancken Posted at: 2018-11-12T07:05:51.652Z Reads: 170

```
[quote="SeanHacker, post:482, topic:71509, full:true"]
@janpom

Can you post pics of your wiring to flash firmware to the board? For some reason all I get is "avrdude: stk500_recv(): programmer is not responding" when trying to flash the firmware from the programmer.
[/quote]

Are you on a Mac by chance? If not, just ignore me. (There is a known bug that results in that error. Super frustrating)
```

---
## \#488 Posted by: janpom Posted at: 2018-11-12T07:08:53.795Z Reads: 162

```
I'm not aware of that bug. I'm on a Mac and I have never seen the error with a correct set up. (I have actually seen it many times but always for a good reason. :smile:)
```

---
## \#489 Posted by: bsancken Posted at: 2018-11-12T07:18:03.706Z Reads: 168

```
I forget what the explanation was but I cannot flash arduinos from my 2017 mac (2010 works fine). 

From a full OS reinstall with neither the online ide or the full ide able to talk to various arduinos with correct settings...  Others do share the bug but it doesn't appear to be big enough to require a fix.

Just figured I'd ask.

Edit----

Also have received the PCB's Yesterday. Thanks!!  (figured I'd give this post some value lol)
```

---
## \#490 Posted by: janpom Posted at: 2018-11-12T07:21:24.948Z Reads: 172

```
That's good to know. Thanks for the info. Hopefully that's not the case for @SeanHacker since he did manage to install the FW to his Arduino UNO before.

Or did you mean flashing as when using the Arduino as ISP?
```

---
## \#491 Posted by: SeanHacker Posted at: 2018-11-12T12:41:12.873Z Reads: 180

```
No problem. Only picture I have on hand until I get home tonight. Hopefully everything's oriented correctly. 

![IMG_20181111_142217|665x500](upload://pyRtdttbF5YdFv5NBSVaWMxX28S.jpeg)
```

---
## \#492 Posted by: janpom Posted at: 2018-11-12T12:54:46.140Z Reads: 173

```
Yes, that looks good. Could you try connecting the display using @lrdesigns' tissue trick :smile: and see if anything shows up on the display when you power it on?

You can power it on with the USB-UART adapter or even with your Arduino. Just connect the GND and +5V using jumper wires.
```

---
## \#493 Posted by: janpom Posted at: 2018-11-12T12:56:26.345Z Reads: 167

```
@SeanHacker You seem to have quite a lot of solder on the MCU pins. Please double-check that nothing is shorted there.
```

---
## \#494 Posted by: SeanHacker Posted at: 2018-11-12T13:25:58.878Z Reads: 168

```
Yep. I was pretty heavy handed and partially drunk when I soldered this board in the picture. Lol. When I get home I have another one that's a lot better. I'll check everything when I get home tonight. Everything powered on, it showed white screen and I kept getting that error when trying to upload. Total noob at this so I'm pretty sure its user error my first time around. ;)
```

---
## \#495 Posted by: janpom Posted at: 2018-11-12T13:46:53.220Z Reads: 167

```
@SeanHacker Only now I realized you don't have the MCU from me so it hasn't been pre-programmed. The display obviously can't show anything but white screen then. Did the MCU come with the bootloader or have you burnt the bootloader yourself? If not, you won't be able to program it. Unfortunately, if it's already soldered on the PCB, you will have hard time burning the bootloader. It's not impossible, but I'm afraid it will be some hassle.
```

---
## \#496 Posted by: SeanHacker Posted at: 2018-11-12T14:01:23.134Z Reads: 162

```
The guy I bought from said "All microcontrollers tested, bootloader uploaded with sample arduino blink sketch on D9 (DIP#15)". But I have another board without that soldered on so I'll flash it before I solder just to make sure.
```

---
## \#497 Posted by: janpom Posted at: 2018-11-12T14:04:50.774Z Reads: 153

```
Ah, OK, good. Hopefully it's something else then. Try checking for shorts.

Also, it should be easy to verify that the blink is indeed uploaded and working correctly. Just power it on and check the pin 15 with multimeter.
```

---
## \#498 Posted by: clistpdx Posted at: 2018-11-12T16:51:43.027Z Reads: 164

```
[quote="SeanHacker, post:482, topic:71509"]
For some reason all I get is “avrdude: stk500_recv(): programmer is not responding”
[/quote]

I get that error off and on on my mac. I'm not positive, but I think sometimes I try a different USB cable, or a different USB port, reopen Arduino software, and then recheck the connection. Then it randomly starts working. I found a forum about it but no one seemed to have great solutions.
```

---
## \#499 Posted by: clistpdx Posted at: 2018-11-12T16:53:40.782Z Reads: 162

```
Oh, and one other thing, in Arduino software, where you choose what type of board you are connecting to, I had to choose "old bootloader" or something along those lines (I don't have my computer with me to send a screenshot right now). I think the Nano's I was using were chinese knockoffs with old software on them, and the "old bootloader" got past the  AVRdude error
```

---
## \#500 Posted by: janpom Posted at: 2018-11-12T17:06:20.978Z Reads: 161

```
True, I too had to use "old bootloader" with some MCUs where I didn't burn the bootloader myself. That could be it.
```

---
## \#501 Posted by: SeanHacker Posted at: 2018-11-12T17:07:46.862Z Reads: 163

```
Thanks @clistpdx and @janpom for the help. I'll be checking this out right when I get home tonight.
```

---
## \#502 Posted by: Vanarian Posted at: 2018-11-12T17:27:54.220Z Reads: 165

```
I'd actually love to test and report, but I don't have enough time on my hand to solder myself all the components. Would just be sitting there and it'd be ready to test after you've finished the first beta phase.
```

---
## \#503 Posted by: SeanHacker Posted at: 2018-11-13T04:35:46.329Z Reads: 182

```
Got home and still couldn't get the vega firmware to upload. Its gotta be these programmers or something. Uploaded to the chip on the uno (forgot to change the config to my board settings ;) ), took that chip out and soldered to a new board. Works now. 

I think these screens I have are defective. They flicker like crazy. Going to order a couple more and see. 

![IMG_20181112_195138|375x500](upload://uz0PM4DFQ3Q2a3bmm8WujeINGpB.jpeg)

![IMG_20181112_175029|665x500](upload://yrAf5tnlG1tm1TnCjhg2DdTLMSH.jpeg)
```

---
## \#504 Posted by: pixelsilva Posted at: 2018-11-13T05:47:54.438Z Reads: 170

```
Test, test, test....
```

---
## \#505 Posted by: janpom Posted at: 2018-11-13T07:11:07.150Z Reads: 164

```
@SeanHacker Nice progress! Can you update the firmware on the MCU using the USB adapter now that it's correctly programmed?
```

---
## \#506 Posted by: SeanHacker Posted at: 2018-11-13T12:22:00.573Z Reads: 165

```
I wasn't able to test last night, but I plugged it in this morning before work and it uploads just fine. :slight_smile:

I have one question though. How should I input my gearing correctly? I use #define GEAR_RATIO 2.5.1 and I get an error "too many decimal points in number"
```

---
## \#507 Posted by: janpom Posted at: 2018-11-13T14:31:55.462Z Reads: 171

```
@SeanHacker The `GEAR_RATIO` is the ratio between the wheel pulley teeth and motor pulley teeth count. For example, if it's 40:15, you would:

```
#define GEAR_RATIO 2.66667
```

or

```
#define GEAR_RATIO (40.0 / 15.0)
```

should also work -- the parentheses are mandatory in this case.

I realize this is somewhat confusing. I'll change this setting to two constants instead called:
- `WHEEL_PULLEY_TEETH`
- `MOTOR_PULLEY_TEETH`
```

---
## \#508 Posted by: janpom Posted at: 2018-11-13T21:20:07.129Z Reads: 164

```
done: https://github.com/janpom/davega/commit/9746e9ecccba519264c0825a736f08d8c0429c5b
```

---
## \#509 Posted by: janpom Posted at: 2018-11-13T23:18:07.894Z Reads: 173

```
Added a [new feature](https://github.com/janpom/davega/issues/13) to the FW. If you press and hold the button 2, the remaining mAh is estimated from current voltage and the Coulomb counter state is set accordingly. This will be handy for those of you who don't charge to 100%. Also good to have anytime mAh is showing the wrong value for whatever reason.

I'll do some more testing tomorrow and if all works, I'll go ahead and release v0.2, so that you guys that will be receiving your Dave kits shortly can grab it.
```

---
## \#510 Posted by: swimmydude Posted at: 2018-11-14T02:59:15.479Z Reads: 176

```
I think the only reason you say that is because you're just use to imperial. The main problem here is that switching over to metric would be difficult and tedious but in the long run it would be so so much easier. 

As someone who grew up using imperial (because that is what is used in United States unfortunately) and then had to use metric for school. Metric is my preferred way to use measurement, even at the detriment of myself because everyone and everything around me is using imperial. I say this even when I can't always envision the size of something in cm/m or the speed of something in kp/h or the temperature of something in Celsius. I still can accurately estimate something in imperial but I suppose I'll only get better with time.
```

---
## \#511 Posted by: SeanHacker Posted at: 2018-11-14T04:16:55.120Z Reads: 183

```
Didn't have much time today. But I have everything in its place and going to drill through my x-things and board to go for a first ride. Hoping for this weekend. First time doing anything like this. I loved everything about it so far. :slight_smile: 

![IMG_20181113_193641|665x500](upload://1MU9fEP0jau1Q8xomPzDfBUlv17.jpeg) ![IMG_20181113_193006|375x500](upload://2bW8zdlrH3WWIEEu7Ko1J0lANc5.jpeg) ![IMG_20181113_194035|665x500](upload://h0EO3xK5hgUDVTVHlEoQpVrJulC.jpeg) ![IMG_20181113_193235|375x500](upload://ot1pA1dWxlgTfpreovESYXa4wpb.jpeg)
![IMG_20181113_164813|665x500](upload://k3ibAZvyrGQaiDeCrgqyP82osNQ.jpeg)
```

---
## \#512 Posted by: lrdesigns Posted at: 2018-11-14T05:25:52.963Z Reads: 183

```
Confirmed the case fits now. Well the top half anyhow, just need to update the bottom half of the case then will upload to thiniverse. I have used a SLA printer so if your using FDM your tolerance will have to be on point or fitment will be tight. 

I got 4 wires for the Vesc and 4 wires for the buttons as they share ground. @janpom   I wonder if you can have just 3 wires for the buttons and share the vesc ground from the other 4 vesc wires? 
I am having the buttons external for now as I can more easily water proof that way, I don't have a specific button on hand yet and my case is so damn small any button will be a challenge to include. 

![Photo%20Nov%2014%2C%201%2008%2006%20PM|375x500](upload://f2vmAUD116HDQaCVUEHLOGsewqN.jpeg) 

![Photo%20Nov%2014%2C%201%2007%2038%20PM|666x500](upload://htu6KrU9X7w6IBA62uNQHGuHaNB.jpeg) 

![Photo%20Nov%2014%2C%201%2008%2055%20PM|375x500](upload://e2AIWpJ8kQro9Fb777zbzKx8Vm.jpeg) 

![Photo%20Nov%2014%2C%201%2009%2049%20PM|690x189](upload://8a847P9kmzAuqCfRt37e5n2oxS2.jpeg)
```

---
## \#513 Posted by: Mich21050 Posted at: 2018-11-14T05:31:51.649Z Reads: 176

```
Quick question: Whats the maximum length of the canbus cable? Because I want my display in the front but my vesc is in the back of my board :smile:
```

---
## \#514 Posted by: janpom Posted at: 2018-11-14T07:49:12.006Z Reads: 173

```
@lrdesigns Awesome work!

[quote="lrdesigns, post:512, topic:71509"]
I wonder if you can have just 3 wires for the buttons and share the vesc ground from the other 4 vesc wires?
[/quote]

Yes, that works. It's the same net.

[quote="lrdesigns, post:512, topic:71509"]
I am having the buttons external for now as I can more easily water proof that way, I don’t have a specific button on hand yet and my case is so damn small any button will be a challenge to include.
[/quote]

Do you have a plan as to where the buttons will go? On the battery enclosure?

Maybe the buttons could go on the right side of the case? The small tactile buttons could potentially fit between the two PCBs, facing right.
```

---
## \#515 Posted by: janpom Posted at: 2018-11-14T07:52:20.965Z Reads: 168

```
We'll have to find out. I ran it with ~40cm of a shitty cable with tiny conductor wires (must be like 30 AWG) and it worked just fine.
```

---
## \#516 Posted by: lrdesigns Posted at: 2018-11-14T07:56:57.089Z Reads: 175

```
![image|373x375](upload://5zquMd6jEPAuiagwa5gaCHPBs9I.jpeg) 

![IMG_1313|375x500](upload://cGVPujmtJJngeEaR0WPl1eT2XWU.jpeg) 

I added a DTR wire for programing externally over the vesc wires. Un-plug vesc first
```

---
## \#517 Posted by: mmaner Posted at: 2018-11-14T16:40:35.248Z Reads: 178

```
I've got 6 PCB's courtesy of @[janpom](https://www.electric-skateboard.builders/u/janpom) for anyone interested.

![IMG_20181114_103745_1542213519986|690x273](upload://s4C7v2GXJZWm7zvhVZopiZQvTY.jpeg) 

Make a donation of $1 or more to Donate to [Doctors Without Borders](https://donate.doctorswithoutborders.org/onetime.cfm?source=ADD180U0U01&utm_source=AdWords&utm_medium=ppc&utm_campaign=GooglePaid&utm_content=branded&gclid=CjwKCAiArK_fBRABEiwA0gOOc9WUKyhqOb-6jv-pFytSncaGl_I34mBCgn5PKIbYbbpbPo8klJssyhoCaRgQAvD_BwE&utm_expid=.ACVuR8QfQoWRpTdJzwfNnQ.0&utm_referrer=https%3A%2F%2Fwww.google.com%2F), this is @janpom's charity of choice, and send me $1 for shipping.  

[![image|288x90](upload://zGaJrVxEA3ytfJjteBdugvMcTsW.png)](https://donate.doctorswithoutborders.org/onetime.cfm?source=ADD180U0U01&utm_source=AdWords&utm_medium=ppc&utm_campaign=GooglePaid&utm_content=branded&gclid=CjwKCAiArK_fBRABEiwA0gOOc9WUKyhqOb-6jv-pFytSncaGl_I34mBCgn5PKIbYbbpbPo8klJssyhoCaRgQAvD_BwE&utm_expid=.ACVuR8QfQoWRpTdJzwfNnQ.0&utm_referrer=https%3A%2F%2Fwww.google.com%2F) 

_This is ONLY the PCB, not the kit.  I do NOT have the other components you will need to complete the DaVeGa._
```

---
## \#518 Posted by: mmaner Posted at: 2018-11-14T19:23:33.386Z Reads: 175

```
Got mine loaded up.  Thanks again @janpom, this is an incredible thing your giving to the community.

![IMG_20181114_125048|682x500](upload://cB52VRR9KqmK8YzeeKVmrmiW7Lk.jpeg)
```

---
## \#519 Posted by: mmaner Posted at: 2018-11-14T20:03:55.411Z Reads: 172

```
does anyone know if I can use a 4 pin momentary switch instead of a 2 pin, using soldered leads on 2 legs?  I have a million of them :slight_smile: .

https://www.amazon.com/GZFY-6x6x4-5mm-Momentary-Tactile-Button/dp/B01N6GU7TA/ref=sr_1_1?ie=UTF8&qid=1542225752&sr=8-1&keywords=6x6x4.5mm+Panel+PCB+Momentary
```

---
## \#520 Posted by: Kug3lis Posted at: 2018-11-14T20:15:08.416Z Reads: 169

```
Both sides are same :) 2 -> 2 Just use multimeter to check which ones are together
```

---
## \#521 Posted by: SeanHacker Posted at: 2018-11-15T00:16:44.326Z Reads: 166

```
Probably another dumb question @janpom or anyone who knows. Not sure what happened but I'm not able to get and data to DAVega. The first time I tried it worked fine. Hooked up to one of my boards tonight and nothing. Do we just wire this up to the vesc just like a Bluetooth module?  Or is something else needed for it to communicate?
```

---
## \#522 Posted by: Battosaii Posted at: 2018-11-15T00:51:03.653Z Reads: 167

```
You have to set the vesc to communicate through UART
```

---
## \#523 Posted by: SeanHacker Posted at: 2018-11-15T01:06:31.192Z Reads: 164

```
Yep. First thing I did before I hooked it up. I run Bluetooth modules in all my boards so it's already set.
```

---
## \#524 Posted by: Kug3lis Posted at: 2018-11-15T01:20:47.986Z Reads: 165

```
TX to RX and RX to TX right? You didnt connected RX to RX and TX to TX? :D
```

---
## \#525 Posted by: SeanHacker Posted at: 2018-11-15T01:41:15.957Z Reads: 172

```
Yep. Same as Bluetooth modules. That's why I'm having a hard time figuring this out. 

Don't mind the ghetto wiring for now until I make the long extension to reach the back of my deck. 

![IMG_20181114_173921|375x500](upload://sLeFZ3rtCGQiajHr3KuvVZh5Ece.jpeg)
```

---
## \#526 Posted by: Kug3lis Posted at: 2018-11-15T01:43:50.227Z Reads: 165

```
Swap red and green man... :D
```

---
## \#527 Posted by: SeanHacker Posted at: 2018-11-15T01:52:36.924Z Reads: 166

```
I'm going to switch them again and see. I hope you're right. I've done this so many times in two days that I don't even see the wires or their colors anymore. Fuck... :slight_smile:
```

---
## \#528 Posted by: SeanHacker Posted at: 2018-11-15T02:55:49.185Z Reads: 176

```
Nope. Didn't work @Kug3lis.  Switch them back and forth now and nothing. It looks like it's stuck where it's at from the only time I had it working. That one time I had some weird shit happen but didn't have any time to investigate. Just woke up the next morning thinking it would work like the last night and it doesn't. Probably something I'm overlooking. 

**When it worked**
https://www.youtube.com/watch?v=aDGbwaHC0QM

**Tonight when it didn't**
https://www.youtube.com/watch?v=GDMbCCSy3m4
```

---
## \#529 Posted by: SeanHacker Posted at: 2018-11-15T03:06:31.360Z Reads: 176

```
And yet. I have another question. Will this screen work for this project? I noticed the pin out is different and they have them at a store by my work. Figured I could give it a shot. They have them for $5.00.

https://www.amazon.com/gp/product/B07G2JYZK6/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#530 Posted by: mmaner Posted at: 2018-11-15T03:13:04.166Z Reads: 171

```
You might need to reload the Arduino project.  I think the display will work but you will need to create leads for the pins so they match the PCB.
```

---
## \#531 Posted by: SeanHacker Posted at: 2018-11-15T03:14:34.108Z Reads: 170

```
Nice. I'll see what I can dig up.
```

---
## \#532 Posted by: janpom Posted at: 2018-11-15T05:27:18.008Z Reads: 176

```
@SeanHacker Please be sure to:

1. Use the stable version of the FW. Grab the v0.1 from releases. Don't use what's in the master, especially not the very latest one. I haven't yet properly tested it.

2. Reset the EEPROM. Your numbers for the distances are way off. That could potentially cause some issues. Just change the EEPROM_MAGIC_NUMBER to a different value before uploading the FW.

3. Be sure to have your settings right. If something is too far off, there may be overflow/underflow errors.

4. Keep an eye on that blinking dot below the speed value. That's VESC data updates. Green is successful, red is failed. If it blinks red, you're not getting data from the VESC. Try increasing the UPDATE_DELAY when that happens, e.g. to 250.

I hope some of this helps. Please do get back if it doesn't.
```

---
## \#533 Posted by: janpom Posted at: 2018-11-15T06:42:16.643Z Reads: 166

```
No, that one has a different pinout. It would probably work with the Dave FW, but the PCB would have to be modified.
```

---
## \#534 Posted by: SeanHacker Posted at: 2018-11-15T13:59:05.679Z Reads: 170

```
I did everything you said and reset EEPROM, switched to v.01, and changed UPDATE_DELAY to 250. Everything looks better now without the screwy numbers. Still not getting vesc data yet. But when I get home tonight I'll screw around with it some more. Any other suggestions are always welcome. Thanks again!

![IMG_20181115_054053|375x500](upload://6nOGZdXr77A5zg7ISGfgjsejvg4.jpeg)
```

---
## \#535 Posted by: janpom Posted at: 2018-11-15T14:11:44.508Z Reads: 165

```
All should be good software wise now. If it's still not working, that must be a hardware problem. Please check that the TX, RX wires have a good connection and are not swapped. The VESC TX goes to the pin labeled TX on the PCB (which is connected to the RX pin on the MCU).
```

---
## \#536 Posted by: SeanHacker Posted at: 2018-11-15T14:13:06.359Z Reads: 165

```
Sweet. Sounds good. I'll swap the wires and check everything out. :sunny:
```

---
## \#537 Posted by: mmaner Posted at: 2018-11-15T14:18:34.201Z Reads: 169

```
[quote="janpom, post:535, topic:71509"]
The VESC TX goes to the pin labeled TX on the PCB (which is connected to the RX pin on the MCU).
[/quote]

I got this backwards :).  I assumed it would be like the HM-10 modules where they were reversed.
```

---
## \#538 Posted by: mmaner Posted at: 2018-11-15T21:17:51.094Z Reads: 186

```
OK, here's the enclosure.  If you wanna jump straight to the [STL's](https://www.thingiverse.com/thing:3218890), here ya go.

This is the actual print of the housing, its a low res print in PETG at 100% infill with a 4mm shell, you can stand on it so it's unlikely to break.

_DaVeGa Riser v2 Housing_

![MM%20DaVeGa%20Riser%20v2%20Housing%208|547x500](upload://DHS3lFHfpPumJ2xSZvhvupEl0m.jpeg) 

My renderings aren't great, I didn't have a lot of time as I was sneaking this in at work :slight_smile:.

![MM%20DaVeGa%20Riser%20v2%20Housing%201|547x500](upload://ooKIXO5w6vH4sjS42itaAPOK7aU.jpeg) 

![MM%20DaVeGa%20Riser%20v2%20Housing%202|547x500](upload://2qs6PNUg8mImpdxczn5u8EGHfll.jpeg) 

![MM%20DaVeGa%20Riser%20v2%20Housing%204|547x500](upload://dkt2yo04RTC1WFdbY8HhtibeOSq.jpeg) 


In the next 4 images you will see DaVeGa Riser v2 Housing A (pic 1) & B Pic 2 -4).  The only difference is the lock that fits in the the slot on the base.  DaVeGa Riser v2 Housing A has no lock, B has a lock.  The lock is for people that want to be able to remove the VeGa faster, by using only 2 screws.

![MM%20DaVeGa%20Riser%20v2%20Housing%203|547x500](upload://ft8Y5arRBGZWUOgCkVRo0bLEQTt.jpeg) 

![MM%20DaVeGa%20Riser%20v2%20Housing%205|547x500](upload://3biVKamVfbOYAJsOwdswSjiuSBM.jpeg) 

![MM%20DaVeGa%20Riser%20v2%20Housing%206|547x500](upload://d2UkQG9bezmVVNSwSAQHx9v0DaC.jpeg) 

![MM%20DaVeGa%20Riser%20v2%20Housing%207|690x440](upload://bB9i1eq6eDPKjzUlS0EkqMhQka4.jpeg) 

These are the different bases.  DaVeGa Riser v2 Housing Base A is easier to seal, has cutouts for truck mount hardware and has multiple mounting slot options (all of the mounting slots are chamfered for use with recessed screws).  Base B is made for people with using X-Braces or top mount trucks.  Both bases come in a version with a lock slot and without.

![MM%20DaVeGa%20Riser%20v2%20Housing%20Base%20A1|547x500](upload://uKvyM6DdOWjKc2bcc1esia8xQdC.jpeg) 

![MM%20DaVeGa%20Riser%20v2%20Housing%20Base%20A2|547x500](upload://taEYRztdPpuLeW9GiaQB3svvWDd.jpeg) 

![MM%20DaVeGa%20Riser%20v2%20Housing%20Base%20B1|547x500](upload://a6G5UNwdMgaJzsipNa87F2MdmsA.jpeg) 

![MM%20DaVeGa%20Riser%20v2%20Housing%20Base%20B2|547x500](upload://qdm5HT6mk0yOR1qnKQsJuBp6yBu.jpeg) 

Here's the links for the STL's if you want to print it.  Please post pics if you decide to print it, I love seeing my work in the wild :).  

https://www.thingiverse.com/thing:3218890

EDIT:  I forgot to mention a couple of things.  

1  There are slots for 3 buttons, but only 1 is through all, but the other 2 can be drilled out with a 4mm bit.  
2.  The housing goes to a 2mm shell at the top, this is to allow enough room for the hardware while keeping the housing as short as possible.  I used a lot of filets to increase the strength.  
3.  I made it wider than I originally planned so the housing could cover the truck hardware and sit outside of it in case people are using recessed bolts.
```

---
## \#539 Posted by: SeanHacker Posted at: 2018-11-15T22:51:43.866Z Reads: 170

```
Thanks for all the help guys. I finally got it working. I think the couple screens I got are screwed. They both blink and black screen when connected (even when connected to the uno). So I'll have to source some of the 2.0 screens from somewhere. Anyone know where to get them fast? 

![Screenshot_20181115-144823_Gallery|690x388](upload://mAtVg0zBfk6PwUA1x9q2ZyA4uEm.jpeg)
```

---
## \#540 Posted by: janpom Posted at: 2018-11-16T07:43:42.943Z Reads: 168

```
@mmaner Great work! Thanks a lot. One question: How do you attach the PCBs to the enclosure? It seems the mounting holes in the top part are supposed to be only used for screwing it to the bottom part, but the screws wouldn't go through the PCBs, correct?
```

---
## \#541 Posted by: mmaner Posted at: 2018-11-16T12:53:12.762Z Reads: 171

```
The screws pass all the way through the housing, electronics into the base. It's pretty snug. I plan on using a rubber sheet in the bottom since I'm not using headers. I printed a complete housing last night, I'll assemble it today and post pics.
```

---
## \#542 Posted by: amazingdave Posted at: 2018-11-16T12:56:06.233Z Reads: 171

```
I like a nice rubber sheep... 🐑
```

---
## \#543 Posted by: JonathanLau1983 Posted at: 2018-11-16T12:56:31.564Z Reads: 175

```
Very nice, I was starting to design something similar.
I've ordered two of these which to use just below the panel, it's going to be a tight fit. They're quite small, 8mm panel hole.
![image|418x354](upload://p1UUIm7DENpEpkREDciUfpuuTRd.jpeg)
```

---
## \#544 Posted by: Kug3lis Posted at: 2018-11-16T12:57:16.727Z Reads: 170

```
Those pretty long :/ I wanted to use something similar they are like 1-2cm length or something similar
```

---
## \#545 Posted by: JonathanLau1983 Posted at: 2018-11-16T13:01:58.722Z Reads: 170

```
Yeah, with pins it reach 15mm inside the enclosure. Might shorten or bend pins to make them fit better.
```

---
## \#546 Posted by: janpom Posted at: 2018-11-16T13:03:48.442Z Reads: 167

```
I see. The electronics gets attached to the base. Unfortunately, that doesn't make the quick release very helpful. I need to be able to quickly remove the top part AND the electronics. This is not to complain though. It's still a cool case. I can hopefully make some modifications to it myself. I don't think there's anyone else in need of the quick release. It doesn't seem a difficult modification. I just need to attach the electronics to the top part instead of the bottom.
```

---
## \#547 Posted by: moon Posted at: 2018-11-16T13:24:49.668Z Reads: 162

```
Have you got a step file for this?
```

---
## \#548 Posted by: lrdesigns Posted at: 2018-11-16T13:27:06.550Z Reads: 160

```
I have all the steps in the file. :wink:
```

---
## \#549 Posted by: moon Posted at: 2018-11-16T13:27:51.271Z Reads: 152

```
Sorry I am blind today, where is this file?
```

---
## \#550 Posted by: lrdesigns Posted at: 2018-11-16T13:28:54.033Z Reads: 166

```
Sorry Friday night 🍺’s. 

I can upload the 3D on Monday. There is a thingiverse page but the files are not good. Wait to the the next version. I printed on a SLA so tolerance is + .1 to .2mm
```

---
## \#551 Posted by: mmaner Posted at: 2018-11-16T13:44:14.281Z Reads: 168

```
If you use shorter screws in the back so they only pass through the housing and electronics, then a nuton the end, you should be able to use just 2 screws in the front to secure it.  I'll look at it again and see what I can come up with.  Im trying to figure out a slide lock mechanism, but its pretty difficult :slight_smile:.
```

---
## \#552 Posted by: janpom Posted at: 2018-11-16T13:48:10.041Z Reads: 166

```
You're kind, but please don't spend too much time on something that only one person (me) would ever make use of.
```

---
## \#553 Posted by: mmaner Posted at: 2018-11-16T14:02:28.441Z Reads: 162

```
Naw,I enjoy the process.  THis one is just particularly difficult :).
```

---
## \#554 Posted by: Friskies Posted at: 2018-11-16T16:26:23.101Z Reads: 161

```
You guys have done an awesome job with all the housing and trying to get it as small as possible. Just a though though... Why not just put the main board in the deck and run a ribbon wire up to to top for the screen on its own? Then you could have a way slimmer form factor ;) .
```

---
## \#555 Posted by: mmaner Posted at: 2018-11-16T16:30:17.571Z Reads: 162

```
its a lot of wires, makes the whole process more complicated.  It could be done, just not by most people.  The VESC cable is gonna be stretch for some folks.
```

---
## \#556 Posted by: Friskies Posted at: 2018-11-16T16:37:26.014Z Reads: 151

```
Fair enough. Once they get their head around this though it will be a fun little mod :stuck_out_tongue:.
```

---
## \#557 Posted by: janpom Posted at: 2018-11-16T17:02:12.153Z Reads: 152

```
It has [already been discussed](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/209?u=janpom) and I do think it's a valid option, though you have more wiring to do. The plus is you don't even need the Dave PCB. Use any Arduino instead. Arduino Nano would work nicely.
```

---
## \#558 Posted by: JonathanLau1983 Posted at: 2018-11-16T17:25:00.099Z Reads: 155

```
Harder to do on decks like Trampa
```

---
## \#559 Posted by: janpom Posted at: 2018-11-16T19:04:32.737Z Reads: 153

```
4 displays arrived from [e_goto Processors Store](https://www.aliexpress.com/item/ILI9225-2-0-Inch-UART-TFT-LCD-Display-Module-SPI-Interface-Colorful-Screen-Serial-Port-176x220/32792711665.html?spm=a2g0s.9042311.0.0.3da24c4dbQPK8W) today. I tested all. All work. Delivery to Czech Republic was almost exactly one month. Not particularly fast, but legit from my perspective. Note that @lrdesigns mentioned he had some trouble with them regarding shipping, though.
```

---
## \#560 Posted by: mmaner Posted at: 2018-11-16T19:21:52.955Z Reads: 159

```
Im seeing what you mean now bu the hardware not mounting to the enclosure.  I had assumed people would just hot glue it in place, but they may not be the best option.  I'll add some mounting slots for the PCB & Display board, but they are gonna be tiny screws as the slots on the PCB are tine.
```

---
## \#561 Posted by: mmaner Posted at: 2018-11-16T19:42:48.229Z Reads: 168

```
OK, you will probably need something like this.  It will also work for where the housing mounts to the base.

https://www.amazon.com/uxcell-Stainless-Phillips-Screws-Washers/dp/B01MYX5AOC/ref=sr_1_10?ie=UTF8&qid=1542397106&sr=8-10&keywords=M2+x+12mm+screw+%26+nut

![image|514x500](upload://nfnsua5ZEnuDrAg7SYlHX5beyCt.jpeg)
```

---
## \#562 Posted by: janpom Posted at: 2018-11-16T19:46:34.051Z Reads: 160

```
Perfect! Yes, I too was thinking M2 screws. Probably slightly longer than 12mm will be needed. IRRC, only Dave itself is 13mm.
```

---
## \#563 Posted by: mmaner Posted at: 2018-11-16T20:00:02.205Z Reads: 158

```
mine is measuring out 10, but im not using headers.  so prolly M2 x 15mm would be perfect.
```

---
## \#564 Posted by: mmaner Posted at: 2018-11-16T20:06:20.911Z Reads: 164

```
The STL's are updated...

https://www.thingiverse.com/thing:3218890
```

---
## \#565 Posted by: janpom Posted at: 2018-11-16T20:30:39.096Z Reads: 163

```
That looks great! I can't wait to get one printed.
```

---
## \#566 Posted by: janpom Posted at: 2018-11-16T20:45:43.035Z Reads: 163

```
@mmaner How about mounting the base plate to the deck using the bolts that hold the truck? Is that a bad idea? You wouldn't need to drill extra holes to the deck.
```

---
## \#567 Posted by: mmaner Posted at: 2018-11-16T20:53:19.157Z Reads: 159

```
I've done that in the past with voltmeter enclosures, the almost always break. I'm happy to make recessed truck bolt bases if anyone wants them tho.
```

---
## \#568 Posted by: janpom Posted at: 2018-11-16T20:59:52.546Z Reads: 163

```
I see. If it almost always broke, it's probably a bad idea. Let me try the base B then. I think I'll need bolts with smaller heads. The diameter of the ones I have is 12mm. The holes in the base plate seem smaller than that. Is that right?
```

---
## \#569 Posted by: mmaner Posted at: 2018-11-16T21:20:00.204Z Reads: 160

```
yeah, they are 10mm.  I can't make them bigger or they overlap, since Im trying to allow for old & new school patterns.
```

---
## \#570 Posted by: janpom Posted at: 2018-11-16T22:04:10.745Z Reads: 154

```
Makes sense. No problem at all. I'll just get smaller ones.
```

---
## \#571 Posted by: mmaner Posted at: 2018-11-16T22:06:00.955Z Reads: 159

```
i can make you a model for whichever truck mounting type you want with 10mm holes, just not both.
```

---
## \#572 Posted by: janpom Posted at: 2018-11-16T22:08:46.336Z Reads: 160

```
No worries. It looks like the current will fit just fine and if not, I can always make it fit with a little bit of filing. Thanks for the great work!
```

---
## \#573 Posted by: mmaner Posted at: 2018-11-16T22:10:48.918Z Reads: 159

```
No worries, glad to help.
```

---
## \#574 Posted by: janpom Posted at: 2018-11-16T22:18:21.100Z Reads: 172

```
So I can assemble 4 Daves per hour. Probably won't make living with this. :smiley: It's very satisfying though. 

![IMG_1520|690x407](upload://bq5LXpUesgu5CD9WihdxDouIZsZ.jpeg)
```

---
## \#575 Posted by: mmaner Posted at: 2018-11-17T01:51:21.655Z Reads: 191

```
So, im having an issue.  I cant seem to get any communications.  Ive tried 4 FocBox's (well, 2 of them are VESC-X's), I've swapped the TX & RX pins a few times.  Still nothing but the red blinking dot.  Any ideas?  @janpom, any insights?

![IMG_20181116_192533|375x500](upload://5a6eNB6OSktBPf6Y64NEQAB6h4O.jpeg) ![IMG_20181116_192526|375x500](upload://6xh60idBhgMXZljUQetzrXOxoRk.jpeg) ![IMG_20181116_192538|375x500](upload://q9B0UmSyAglY3XpzbomfGOZwGDv.jpeg)
```

---
## \#576 Posted by: janpom Posted at: 2018-11-17T07:45:08.322Z Reads: 174

```
@mmaner Assuming the FocBox pins are 5V, VCC, GND, ADC1, RX, TX, ADC2, you have the wires swapped on the picture. The connection should be:

5V - 5V
GND - GND
RX - RX
TX - TX

The pin labeled RX on the Dave PCB goes to the TX pin of the MCU. In other words, it does not label, which MCU pin it is but rather which VESC pin you should connect.

Since you mentioned you swapped the wires a few times, this is probably not the only problem.

Some questions:
- Which FW version are you using on your VESCs?
- Do you have the UART communication enabled?
- Is the UART baud rate set to 115200?
```

---
## \#577 Posted by: janpom Posted at: 2018-11-17T07:47:08.726Z Reads: 161

```
BTW, are there only 7 pins on the FocBoxes? I have 8 pins on my ESCapes and I'm including only 8 pin JST PH connectors in the kit. It looks like that won't work for some people.
```

---
## \#578 Posted by: deucesdown Posted at: 2018-11-17T13:39:11.332Z Reads: 160

```
Vesc4 designs including focbox have 7 pin. Vesc6 is 8 pin.

Escape also reverses the pins compared to original vesc6.

Fun stuff.
```

---
## \#579 Posted by: mmaner Posted at: 2018-11-17T14:28:26.480Z Reads: 166

```
I believe I'm running v0.1, but I'll need to check that. The baud rate is 115200. 

Yes, most v4 VESC's use a 7 pin just 2.0, I think all of them do. A lot of people use a 6 pin and skip the AD2 pin. 

I've got a funeral to go to then drive to Pennsylvania to pick up my kid. I likely won't be able to get back to this until Monday.
```

---
## \#580 Posted by: janpom Posted at: 2018-11-17T14:35:52.015Z Reads: 165

```
[quote="mmaner, post:579, topic:71509"]
I believe I’m running v0.1, but I’ll need to check that.
[/quote]

Yes, that's the Dave FW version. It's shown on the display. I asked about the VESC FW version though. Do you have the latest one (3.40)?
```

---
## \#581 Posted by: mmaner Posted at: 2018-11-17T15:30:03.577Z Reads: 159

```
Ahhh, no.  I'm running 3.54 on one and 4.02 on the other, bit @Ackmaniac.
```

---
## \#582 Posted by: janpom Posted at: 2018-11-17T15:40:37.230Z Reads: 161

```
Aha! That might be the problem. I don't know what changes there are in Ackmaniac's FW. I'll take a look at it.
```

---
## \#583 Posted by: janpom Posted at: 2018-11-17T15:41:45.644Z Reads: 157

```
@mmaner You don't happen to have a VESC with the standard FW, do you?
```

---
## \#584 Posted by: mmaner Posted at: 2018-11-17T15:54:34.987Z Reads: 155

```
Not at the moment, but I can prolly make that happen when I get back from PA.
```

---
## \#585 Posted by: janpom Posted at: 2018-11-17T16:03:07.615Z Reads: 159

```
That would be helpful, so that we know whether the problem is somewhere in Dave or it's just an incompatibility with Ackmaniac's FW.
```

---
## \#586 Posted by: mmaner Posted at: 2018-11-17T16:40:50.659Z Reads: 151

```
I hadn't thought about that, I default use Acks firmware. That's likely the cause.
```

---
## \#587 Posted by: mmaner Posted at: 2018-11-17T16:42:32.380Z Reads: 153

```
On another note... I've ordered a ton of filiment. Next week I'm gonna print housings for a few days for people that need them.
```

---
## \#588 Posted by: SeanHacker Posted at: 2018-11-17T16:48:55.164Z Reads: 156

```
I'm using ack's firmware (latest whatever that is) and it was working. I'll do some testing in a few minutes just to verify. 

Every screen I seem to order doesn't work right. I have to pinch the screen for them to work properly. Even picked up some nano's yesterday just to test and I get the same screen flickering.

@mmaner I would like to buy a case from you if possible. :slight_smile:
```

---
## \#589 Posted by: Mich21050 Posted at: 2018-11-17T16:54:24.633Z Reads: 156

```
@mmaner I would be in for one case :smile:
```

---
## \#590 Posted by: ROFEN13 Posted at: 2018-11-17T17:12:10.385Z Reads: 150

```
I just ordered 5kg of pteg filament as well and can help out if needed. I also have the dremel laser cutter coming soon, and can cut some cases if someone wants to create a file for me
```

---
## \#591 Posted by: mmaner Posted at: 2018-11-17T20:28:10.415Z Reads: 151

```
No buying, just pay shipping. I'll start printing Tuesday.
```

---
## \#592 Posted by: janpom Posted at: 2018-11-17T20:58:33.472Z Reads: 168

```
[quote="mmaner, post:581, topic:71509"]
I’m running 3.54 on one and 4.02 on the other
[/quote]

Hm, are you talking about https://github.com/Ackmaniac/bldc? Or are there any other FW mods? That repo is a bit strange. There are not many changes. It doesn't seem to be in sync with the latest Vedder's updates. There are no releases and I can see no other versions than 3.101 and 3.102. Where do you get the 3.54 and 4.02 from?
```

---
## \#593 Posted by: mmaner Posted at: 2018-11-17T21:10:01.574Z Reads: 162

```
I fat fingered it, driving. Sorry about that. It's 2.54 and 3.102.
```

---
## \#594 Posted by: janpom Posted at: 2018-11-17T21:58:38.217Z Reads: 167

```
DAVEga FW v0.2 released: https://github.com/janpom/davega/releases/tag/v0.2

BTW, you want the `davega-v0.2.zip` file, not the sources (unless you know what you're doing).
```

---
## \#595 Posted by: JonathanLau1983 Posted at: 2018-11-20T15:02:02.890Z Reads: 175

```
Switches have arrived, they're pretty small.
![image|666x499](upload://etzOYR22PBGlF6lH4KilqZ0Pc5m.jpeg) 

Enclosure is still work in progress, need to add bolt slots for attaching to board etc.
![image|665x500](upload://dmCMGshzU1D2lRqp4vyD8gxmSlT.png)
```

---
## \#596 Posted by: CarbonV Posted at: 2018-11-20T15:58:56.349Z Reads: 170

```
![IMG_20181120_163928|666x500](upload://dg9HyrytESluP7O12nVdqE1zAtN.jpeg)
Looking mint😎
```

---
## \#597 Posted by: janpom Posted at: 2018-11-20T16:00:03.142Z Reads: 162

```
Nice! You're the first to have the v0.3! :smiley:
```

---
## \#598 Posted by: moon Posted at: 2018-11-20T16:22:32.344Z Reads: 160

```
What are those switches for?
```

---
## \#599 Posted by: JonathanLau1983 Posted at: 2018-11-20T16:50:05.125Z Reads: 162

```
Going to hook up to Buttons 1 and 2. More of a futureproof thing.
Future firmware could use them to toggle things, maybe imperial to metric etc.
```

---
## \#600 Posted by: moon Posted at: 2018-11-20T16:50:48.069Z Reads: 158

```
Oh ok, it should look great, have you 3d printed that case?
```

---
## \#601 Posted by: JonathanLau1983 Posted at: 2018-11-20T16:51:30.275Z Reads: 162

```
Not yet, got the LCD already and waiting on a kit in the post from @janpom
```

---
## \#602 Posted by: janpom Posted at: 2018-11-20T17:53:03.083Z Reads: 166

```
Note that button 2 is already used in FW v0.2. It resets the mAh. Button 3 will be used for toggling between multiple screens. Coming soon.
```

---
## \#603 Posted by: Battosaii Posted at: 2018-11-20T18:45:12.937Z Reads: 162

```
Can't wait to put mine together :slight_smile:
```

---
## \#604 Posted by: bigben Posted at: 2018-11-20T18:52:39.616Z Reads: 188

```
What buttons have you guys been going for?
```

---
## \#605 Posted by: High-roller Posted at: 2018-11-20T19:54:54.791Z Reads: 188

```
Just got my screen, ready and waiting to get started!
```

---
## \#606 Posted by: janpom Posted at: 2018-11-20T20:28:55.959Z Reads: 191

```
I'm 1 PCB short for shipping ordered unassembled kits. I can ship an assembled one instead. Anyone interested?
@SourPlumGoose @Battosaii @spesh @venom121212
```

---
## \#607 Posted by: Battosaii Posted at: 2018-11-20T20:32:05.881Z Reads: 180

```
I wanted to do it my self and learn but if no one else takes it I will.
```

---
## \#608 Posted by: bigben Posted at: 2018-11-20T20:35:09.902Z Reads: 184

```
If you want me to send a pcb I can. I've only part assembled some of them.
```

---
## \#609 Posted by: janpom Posted at: 2018-11-20T20:43:13.667Z Reads: 190

```
Thanks @bigben, but I hope it won't be necessary.

I found one more PCB that has SMD caps pre-soldered. If nobody prefers the assembled kit but someone would rather avoid SMD soldering, I can send them this one.

![IMG_1524|690x468](upload://qbFFC8GNlMYrapZPQWASUxcTRKj.jpeg) 

Also thanks @Battosaii for offering to take the assembled one even if you don't prefer that. I hope we'll find someone else so that you can enjoy the assembly. :smiley:
```

---
## \#610 Posted by: JonathanLau1983 Posted at: 2018-11-20T21:06:39.294Z Reads: 174

```
[quote="janpom, post:602, topic:71509, full:true"]
Note that button 2 is already used in FW v0.2. It resets the mAh. Button 3 will be used for toggling between multiple screens. Coming soon.
[/quote]

What's button 1 used for?
```

---
## \#611 Posted by: mmaner Posted at: 2018-11-20T21:07:15.151Z Reads: 162

```
to reset the distance
```

---
## \#612 Posted by: 257 Posted at: 2018-11-20T21:14:25.354Z Reads: 160

```
Is that assembled kit you’re offering for those who have already requested a kit? If not I’ll jump on that and send you some $ :grinning:
```

---
## \#613 Posted by: janpom Posted at: 2018-11-20T21:23:56.704Z Reads: 159

```
Yes, it's for those who ordered a kit, sorry. I have 2 spares that I need to keep so that I have something to re-ship in case any packages are lost. Once everything is delivered, these spares can go as well. Please ask again in ~2 weeks.
```

---
## \#614 Posted by: 257 Posted at: 2018-11-20T21:25:03.003Z Reads: 154

```
Ah, no prob. I’ll check back :+1:
```

---
## \#615 Posted by: spesh Posted at: 2018-11-20T21:35:23.147Z Reads: 158

```
I'll take the assembled one @janpom , I've got too much shit to do anyway so might do me a favour haha :smiley:
```

---
## \#616 Posted by: janpom Posted at: 2018-11-20T21:37:28.245Z Reads: 160

```
Perfect! Thanks, @spesh.
```

---
## \#617 Posted by: venom121212 Posted at: 2018-11-20T21:52:27.172Z Reads: 158

```
Ah beat me to it. Oh well!
```

---
## \#618 Posted by: janpom Posted at: 2018-11-20T22:03:40.635Z Reads: 180

```
Alright guys, everything ready to be shipped tomorrow morning. These kits will go to:
- @new
- @SourPlumGoose (2 kits)
- @Battosaii
- @Spesh (assembled)
- @venom121212
- @Andy87  (assembled)
- @Darkie02 (assembled)
- @High-roller (assembled)
- @yelnats8j (assembled)

Now, it's slightly confusing with capacitors (again). Please pay attention.

- 22 pF capacitors - There are no THT, only SMD. It's the packaging with 3 capacitors.
- 100 nF capacitors - All packages should have 2 THT (one spare). Some packages also have 1 SMD. (I ran out of SMD ones so couldn't provide one for everybody.) Both THT and SMD work. If you have a choice, use whatever you're more comfortable with.

22 pf caps:

![IMG_1517|341x393](upload://fGjeqzC3jbs3gmXcG9C3qqDgycG.jpeg) 

100 nF caps:

![IMG_1523|252x499](upload://sWVrIZpSYgBFKHYklt7z5dzU78k.jpeg)
```

---
## \#619 Posted by: janpom Posted at: 2018-11-20T22:13:48.599Z Reads: 158

```
That's it for the batch 1. Now it's time to do some testing. I hope all goes well and we'll tweak a few things for the next batch.

I'm still thinking about how I'll do the batch 2. I did enjoy assembling Daves, but there's also a bunch of not-so-much-enjoyable tasks like completing the kits, packaging, filling out customs forms (especially this one!!!). I still have a ton of parts on hand, for which I'd like to find new owners, so something will definitely happen. Stay tuned.
```

---
## \#620 Posted by: JonathanLau1983 Posted at: 2018-11-20T22:41:28.130Z Reads: 155

```
How easy would it be implemented long press to reset things? So we could get more functionality from fewer buttons.
```

---
## \#621 Posted by: janpom Posted at: 2018-11-20T22:51:54.898Z Reads: 157

```
It's not hard. Nothing about how the buttons currently work is carved into stone. You can also customize it yourself. It's open source.

One problem, though, is the limited size of the flash memory on the MCU. The FW is already taking up some 80%, so there's no space for too many additional fancy features.
```

---
## \#622 Posted by: lrdesigns Posted at: 2018-11-21T01:29:08.882Z Reads: 178

```
Guys I have updated the thingiverse post as my design is workable now. Everything fits. It will still evolve but if you want to give it a go have at it. It might be challenging on the internal tollerances with a FDM printer as it was developed with a SLA printer. If you can adjust the wall offset in software maybe try that. 

https://www.thingiverse.com/thing:3171000

My DAVEga is ready to go and I wish I could just plug it into my Vesc, but that job is going to be a huge pain in the but. I have super extra water proofed them so it will require a lengthy disassebly and then I need to scrape silicone conformal coating of the pcb to get access to the pads. :pensive: :triumph: :cold_sweat: I have even removed the JST connectors from my vescs. 

Winter is dry season here though so I guess its an ok time to pull this shit appart. 

![File%20Jul%2011%2C%2010%2028%2050%20AM|666x500](upload://2DevYjrv9TczEytbyTEO4dgZIye.jpeg) 

It has a thick shrink wrap that is glued at both ends, then its glued into the enclosure. 

![IMG_1420|690x328](upload://ruyMPR0QwHs2oIKEeuyKviAH0WK.jpeg)
```

---
## \#623 Posted by: lrdesigns Posted at: 2018-11-21T01:50:17.007Z Reads: 167

```
[quote="JonathanLau1983, post:543, topic:71509"]
I’ve ordered two of these which to use just below the panel, it’s going to be a tight fit. They’re quite small, 8mm panel hole.
[/quote]

These look good, got a link?
```

---
## \#624 Posted by: Battosaii Posted at: 2018-11-21T03:36:13.984Z Reads: 165

```
Not to go off topic but I have found that bullet connectors soldered directly to the PCB tend to break off over time with vibration.
```

---
## \#625 Posted by: lrdesigns Posted at: 2018-11-21T03:46:29.947Z Reads: 171

```
I would agree if there is any mechanical stress on them its not a good idea. Even just wires that can vibrate off the end. But mine are supported by glue and heat shrink, then the wires exit through the enclosure. 
![File%20Jul%2017%2C%2012%2053%2055%20PM|666x500](upload://88o6MLwVCR4Rk96RYu2Mm7Ag5mX.jpeg) 
![File%20Jul%2017%2C%2012%2053%2036%20PM|666x500](upload://pwdG2tSGeR3077fonPdaxJDG9hO.jpeg)
```

---
## \#626 Posted by: High-roller Posted at: 2018-11-21T07:05:30.666Z Reads: 165

```
Hey, I couldn't find this earlier in the thread, but what do you do about dual motors connected with ppm? Is there a mode in the firmware where it simply multiplies the received info by 2, like with the Bluetooth monitor apps?
```

---
## \#627 Posted by: janpom Posted at: 2018-11-21T07:12:25.801Z Reads: 166

```
Yes. You set the number of vescs to 2 in the config.
```

---
## \#628 Posted by: JonathanLau1983 Posted at: 2018-11-21T07:35:47.975Z Reads: 170

```
[quote="lrdesigns, post:623, topic:71509"]
These look good, got a link?
[/quote]

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F273352943751
```

---
## \#629 Posted by: JonathanLau1983 Posted at: 2018-11-21T10:53:57.872Z Reads: 170

```
Parts have arrived!
Did a test print to check for sizing and hole spacing last night for the case. I'm going to ream the holes on the PCB to 3mm like the LCD, then use the nylon standoffs to stack it up.

Thanks @janpom ! 
![image|666x500](upload://4X786DnZXXAr5m7C9LF58ZOHH5H.jpeg)
```

---
## \#630 Posted by: amazingdave Posted at: 2018-11-21T12:30:48.922Z Reads: 167

```
It’s arrived!! Still waiting on my screens 🙁
```

---
## \#631 Posted by: Andy87 Posted at: 2018-11-21T12:31:33.147Z Reads: 161

```
For me the other way round 😅
Displays already here, the rest no...
```

---
## \#632 Posted by: janpom Posted at: 2018-11-21T15:27:44.304Z Reads: 164

```
I'm working on multiple screens that one will be able to toggle between. I will implement at least 3 different screen layouts to get a better idea about what the good API for screen layout plug-ins would be. Now it's good time for feature requests:

What would you change about the current screen layout? What other info would you like to have? Which info should be more prominent? What would your ideal screen look like?
```

---
## \#633 Posted by: mmaner Posted at: 2018-11-21T15:30:39.410Z Reads: 160

```
The battery percentage value small on top 1/3, speed large on bottom 2/3rds.  White text on a black background.  SImple and useful.
```

---
## \#634 Posted by: ROFEN13 Posted at: 2018-11-21T15:36:20.107Z Reads: 167

```
I would say distance as well, next to battery voltage on the top. But i like simplicity as well. Less distracting to do a quick check while riding.
```

---
## \#635 Posted by: janpom Posted at: 2018-11-21T15:46:02.385Z Reads: 167

```
Like this?

![screen-mmaner|176x220](upload://fbsiXHR2cTn825EO1IaQQrBNeIJ.png)
```

---
## \#636 Posted by: mmaner Posted at: 2018-11-21T15:46:21.107Z Reads: 158

```
Yeah, thats attractive.
```

---
## \#637 Posted by: janpom Posted at: 2018-11-21T15:48:21.196Z Reads: 160

```
That's too easy. :)

Any more challenging requests?
```

---
## \#638 Posted by: harrypzee Posted at: 2018-11-21T15:49:30.675Z Reads: 158

```
This is awesome. I definitely want one! What if instead of being a square, the display was circular? Then it could be much more speedometer looking.
```

---
## \#639 Posted by: janpom Posted at: 2018-11-21T16:03:28.455Z Reads: 171

```
![screen-ROFEN13|176x220](upload://nZudRGgv21gDQSPhjgY8PJ6Dysc.png) 

Not very pretty, but probably has the info you want.
```

---
## \#640 Posted by: mmaner Posted at: 2018-11-21T16:09:29.177Z Reads: 169

```
Thats awesome, I really like that.  Maybe make the battery go yellow at 50% and the speed go yellow after 25 mph?
```

---
## \#641 Posted by: deucesdown Posted at: 2018-11-21T16:10:53.663Z Reads: 165

```
I'm thinking (barely) out loud here, but some kind of voltage sag indicator would be useful...
```

---
## \#642 Posted by: JonathanLau1983 Posted at: 2018-11-21T16:12:26.876Z Reads: 164

```
Average cell value Voltage would be useful
```

---
## \#643 Posted by: janpom Posted at: 2018-11-21T16:24:49.570Z Reads: 165

```
Anyone cares about additional VESC telemetry data, such as motor temperature, MOSFET temperature, input/output current?
```

---
## \#644 Posted by: janpom Posted at: 2018-11-21T16:26:14.481Z Reads: 160

```
How about estimated range? (Would interpolate traveled distance using remaining battery capacity.)
```

---
## \#645 Posted by: mmaner Posted at: 2018-11-21T16:29:06.517Z Reads: 152

```
Estimated range would be great.  That's actually one the most important values that I use in the Ack app.
```

---
## \#646 Posted by: deucesdown Posted at: 2018-11-21T16:30:10.517Z Reads: 161

```
yes yes and yes :) I run ackmaniac app to see, in this order:
- fault codes
- top speed for ride
- max temps
- max/min currents (brakes too)
- min voltage (sag)
- wh/mile
- distance

First priority: is anything is blowing up. Second priority, how close am I to the limits.

If I could get a few of these it would free me from running the app on every ride. One less step...

I may be the weird one but I'm not that worried about range? My rides are along well known routes, and I know beforehand if my board can do it.

Oh I want to make clear, I'm not saying "please do these for me". I'm fine with whatever choices you've made and will continue to make.
```

---
## \#647 Posted by: janpom Posted at: 2018-11-21T16:35:35.382Z Reads: 162

```
Thanks, this is helpful. I'm thinking that one screen should be for details. You wouldn't use it while riding, but you may want to switch to it when you stop and check various info there. The values you mentioned would be a perfect fit.
```

---
## \#648 Posted by: billappleton Posted at: 2018-11-21T16:54:21.171Z Reads: 159

```
I wish elapsed time was on there. When I am done with a ride, I want to know how long, how far, top speed, and average speed.
```

---
## \#649 Posted by: venom121212 Posted at: 2018-11-21T17:09:58.607Z Reads: 161

```
Maybe a page with a stopwatch feature for timing laps?
```

---
## \#650 Posted by: ROFEN13 Posted at: 2018-11-21T17:29:19.626Z Reads: 161

```
These options are re all so cool! Multiple pages with different data would be awesome to have.
```

---
## \#651 Posted by: bigben Posted at: 2018-11-21T19:31:58.738Z Reads: 168

```
![58|390x500](upload://bgZq0RnoKQ4canFZindVHntxArp.png) 
So near but clearly pretty far...
Any tips anyone?
```

---
## \#652 Posted by: janpom Posted at: 2018-11-21T19:38:31.913Z Reads: 166

```
You have a bootloader on the MCU, right?
```

---
## \#653 Posted by: bigben Posted at: 2018-11-21T19:39:49.267Z Reads: 171

```
![image|375x500](upload://4IuDO7soR7QTZ0pcpUNODIGkfdk.jpeg) Well, the chip supposedly came pre installed with a bootloader.?
At this point I guess its a bit late to be finding out they lied..
```

---
## \#654 Posted by: janpom Posted at: 2018-11-21T19:43:07.082Z Reads: 161

```
Let's assume they didn't lie about the bootloader. Is the display soldered on the PCB or can it still be removed? If the latter, could you post a detailed picture of the PCB, ideally in good light and both sides.
```

---
## \#655 Posted by: bigben Posted at: 2018-11-21T19:46:57.546Z Reads: 160

```
Soldered on the screen..
just checking joints. there are a couple of suspect solder joints..
```

---
## \#656 Posted by: janpom Posted at: 2018-11-21T19:56:48.668Z Reads: 161

```
Oops. I should have told you to try to program the MCU before soldering the display on the PCB. Do you think you'll manage to desolder the display?

Unfortunately, there's a number of reasons it may not work and it will be hard to identify the culprit. It could be:
- no bootloader
- bad USB-UART adapter
- problem in the reset net (MCU doesn't get reset on the DRT signal)
  - you're sure you have the correct capacitor (100 nF?)
- bad connection/short anywhere on the PCB

If you have an Arduino, you could use it to program the MCU. It's a bit of a hassle, but it can be done. If that succeeded that would narrow down the issue quite a bit.
```

---
## \#657 Posted by: bigben Posted at: 2018-11-21T19:59:04.873Z Reads: 150

```
I have other a load of other usb-part adapters so I can rule that out. I can probably desolder the display..
```

---
## \#658 Posted by: SeanHacker Posted at: 2018-11-21T21:14:34.722Z Reads: 158

```
[quote="bigben, post:653, topic:71509"]
Well, the chip supposedly came pre installed with a bootloader.?
[/quote]

That's what the add on the listing I purchased from said too. I was getting that same error. But once I used an MCU with a bootloader it worked.

P.S- I was able to desolder the screen fairly easily with a solder iron some ceramic pliers.
```

---
## \#659 Posted by: bigben Posted at: 2018-11-21T21:20:45.571Z Reads: 147

```
I'll give it a go at the weekend. I'm away for work for a few days.
To be honest I was pretty excited to even see the screen light up..
```

---
## \#660 Posted by: janpom Posted at: 2018-11-21T22:17:05.586Z Reads: 151

```
@bigben One more idea. In the Arduino IDE, try selecting "Tools > Board > Arduino Nano" and then "Tools > Processor > ATMega328P (Old Bootloader)". Then upload the FW.
```

---
## \#661 Posted by: bigben Posted at: 2018-11-21T22:20:39.108Z Reads: 164

```
I did try that, same response sadly..
```

---
## \#662 Posted by: SeanHacker Posted at: 2018-11-21T22:51:37.732Z Reads: 171

```
Thanks for the idea for a different button. I have these and the black version at my work so I used one for the master and two recessed for things I don't want to push easily. 

![IMG_20181121_144714|665x500](upload://nzujU8NpU6MaO05Dfn6yssX1B0b.jpeg)
```

---
## \#663 Posted by: mmaner Posted at: 2018-11-21T22:56:56.122Z Reads: 165

```
that looks great
```

---
## \#664 Posted by: SeanHacker Posted at: 2018-11-21T23:24:47.622Z Reads: 161

```
Thanks man. I've literally been eyeballing everything. I'm only a month in on learning how to draw things up and use a lazer cutter at work. I've never really done anything like this before. I seriously can't wait to get a screen that works right so I can use this thing!
```

---
## \#665 Posted by: SeanHacker Posted at: 2018-11-21T23:27:15.852Z Reads: 155

```
That ui is sweet! Minimal looks so clean. But I still love what you have now. It reminds me of the 80's and arcade games from when I was a kid.
```

---
## \#666 Posted by: lrdesigns Posted at: 2018-11-22T02:17:23.309Z Reads: 175

```
[quote="deucesdown, post:646, topic:71509"]
* fault codes
* top speed for ride
* max temps
* max/min currents (brakes too)
* min voltage (sag)
* wh/mile
* distance
[/quote]

A page for all this would be pretty good. 


I think a simple display screen like this would be awesome, and easy to make a horizontal version. A horizontal orientation would make it much better to fit inside the truck bolts. The max / min detail info screen could still be vertical as there is no need to read that while riding. 
[quote="janpom, post:639, topic:71509"]
![screen-ROFEN13|176x220](https://www.electric-skateboard.builders/uploads/db1493/original/3X/a/8/a82557ffbebab3b20dc7ec4d9c1c0e57c2a9f0a4.png)
[/quote]
![image|690x409](upload://m1dmJaYAqjGSGj3Yk4M8LiGZ0Mx.jpeg) 

The red bar is only there if you get a fault.
```

---
## \#667 Posted by: janpom Posted at: 2018-11-22T06:58:09.512Z Reads: 166

```
I like that. I'll try to get it done over the weekend.
```

---
## \#668 Posted by: JonathanLau1983 Posted at: 2018-11-22T10:11:03.193Z Reads: 170

```
![image|666x500](upload://5uGizU92YoVEO9WMVeUQaDbQXqI.jpeg) 
![image|666x500](upload://iL15hij33kIjRkTYpYdHsC29rxf.jpeg) 
![image|666x500](upload://hGfuM64cKoVV7fY9NOcTMyH95s5.jpeg)
```

---
## \#669 Posted by: Grozniy Posted at: 2018-11-22T10:25:53.200Z Reads: 167

```
Só cute :smiling_face_with_three_hearts:
```

---
## \#670 Posted by: janpom Posted at: 2018-11-22T13:39:12.388Z Reads: 169

```
Looks great! Are those 3D printed spacers between the PCBs? How did you manage to squeeze to screw head next to the display? Are those M2 screws?
```

---
## \#671 Posted by: JonathanLau1983 Posted at: 2018-11-22T14:43:42.803Z Reads: 172

```
They are 3D printed spacers, I didn't have standoffs the size I wanted to use.
They're M3 bolts, no spacing issues.
```

---
## \#672 Posted by: janpom Posted at: 2018-11-22T14:47:32.824Z Reads: 173

```
I wasn't able to use M3 screws. Maybe you have ones with smaller heads. Could you please post the picture of the arrangement from the first picture in your previous post but taken from the top.
```

---
## \#673 Posted by: JonathanLau1983 Posted at: 2018-11-22T14:55:21.243Z Reads: 178

```
I don't have it on me, but I took this one yesterday, it's the same screws.
They're just M3 button head bolts.

![image|607x399](upload://am8q85blKoEdvHDptXvwM1TpZ0i.jpeg)
```

---
## \#674 Posted by: JonathanLau1983 Posted at: 2018-11-22T14:57:41.595Z Reads: 172

```
Oh, and the two holes on the opposite side to the LCD header pins is off by about 1mm. Needs to be closer to the edge, my bolts are going a bit of an angle at the moment.
```

---
## \#675 Posted by: SeanHacker Posted at: 2018-11-22T17:48:41.826Z Reads: 177

```
Alright guys. I finally got one of my screens to work perfectly. Just need some advice. The MPH is way off. I had to change to 2-3 Motor Pole Pairs to get it above 9MPH. But so far with my settings the speed maxes out at 9MPH. @janpom or anyone that can help. I have a dual setup with 6380 motors. What should my settings be in the config? Here's what I have so far. 

#define VESC_COUNT 2  // number of controllers: 1 = single, 2 = dual
#define MOTOR_POLE_PAIRS 7
#define WHEEL_CIRCUMFERENCE_MM 100
#define MOTOR_PULLEY_TEETH 16
#define WHEEL_PULLEY_TEETH 40 

https://youtu.be/V0ruKbMoNHY
```

---
## \#676 Posted by: janpom Posted at: 2018-11-22T17:53:54.766Z Reads: 174

```
@SeanHacker https://en.wikipedia.org/wiki/Circumference
```

---
## \#677 Posted by: banjaxxed Posted at: 2018-11-22T18:05:34.300Z Reads: 172

```
http://www.math.com/students/calculators/source/circle-solver.htm

100m wheel = 314.1592653589793mm circumference, I would be tempted to round that out.

Ps. this is awesome
```

---
## \#678 Posted by: SeanHacker Posted at: 2018-11-22T18:15:46.963Z Reads: 168

```
[quote="janpom, post:676, topic:71509"]
https://en.wikipedia.org/wiki/Circumference
[/quote]

[quote="banjaxxed, post:677, topic:71509"]
100m wheel = 314.1592653589793mm circumference, I would be tempted to round that out.

Ps. this is awesome
[/quote]

Thanks guys. I'm not sure what I was thinking. Up and running perfectly now. Going to drill into my X-Things and board to mount this gadget and go for a first ride when the rain is gone this weekend. I love this thing. I'll be posting a video soon. :slight_smile:
```

---
## \#679 Posted by: lrdesigns Posted at: 2018-11-23T09:12:02.343Z Reads: 166

```
@janpom I'm sure this information is in here somewhere but I can not figure it out. 

What are the exact Vesc settings you need to get this to work. I have dual vesc run on split PPM.

Your instructions on github for the DAVEga is really good but maybe add some points about the vesc setup. 

Is this all the settings I need to change?
![image|272x182](upload://uuWbZFFx1ZW5HJmYvsazw23BvNI.png) 

Baud rate? 
![image|530x40](upload://d4SHfsAi9agsGSjRufKTNnohCR3.png)
```

---
## \#680 Posted by: janpom Posted at: 2018-11-23T09:16:32.984Z Reads: 161

```
Good point. I'll add a section about VESC setup. I believe you only need to enable UART and set the baud rate to 115200. What you have looks correct. I don't think the CAN settings are relevant.
```

---
## \#681 Posted by: lrdesigns Posted at: 2018-11-23T09:30:53.504Z Reads: 165

```
Thanks, I tried CAN Status true and false. But my Baud was at 9600. Will try again on Monday.
```

---
## \#682 Posted by: janpom Posted at: 2018-11-23T22:12:19.565Z Reads: 176

```
Some progress on the horizontal layout.

![IMG_1525|666x500](upload://rDxZRi1oG0UPhGyFjXwpRaklSuy.jpeg) 

![IMG_1527|666x500](upload://iJMKHRjxQYu8ERu6NwduQJZJDba.jpeg)

![IMG_1528|666x500](upload://1MdHlrw3xcyZduuEedzMuOJanBu.jpeg)
```

---
## \#683 Posted by: JonathanLau1983 Posted at: 2018-11-23T22:32:32.854Z Reads: 167

```
Awesome work as always @janpom
Hope to have the time to get mine soldered together on Sunday. 
Changing the model to work in landscape too.
```

---
## \#684 Posted by: Mich21050 Posted at: 2018-11-23T22:34:49.516Z Reads: 172

```
Ok so after talking with @janpom about selling kits I would like to know if there's any interrest in kits right now. :smile:

Would you like a DAVEga kit:
[poll type=multiple min=1 max=1 public=true]
* Yes
* No
[/poll]
```

---
## \#685 Posted by: SeanHacker Posted at: 2018-11-23T23:12:51.212Z Reads: 172

```
Testing in doors while it's raining. I thought I might have some problems with the wires being sonlong but it works great. Still need to drill a whole through my deck and it will be perfect. :slight_smile:

https://www.youtube.com/watch?time_continue=1&v=Sj2YhWCjw7Q
```

---
## \#686 Posted by: ROFEN13 Posted at: 2018-11-24T00:03:51.537Z Reads: 164

```
I realllly like the horizontal display. I can't wait to get the kit and test it out for you!
```

---
## \#687 Posted by: SeanHacker Posted at: 2018-11-24T01:19:36.195Z Reads: 177

```
So close to finished now. Just need to do one minor revision to my enclosure and I'm finished. I seriously can't wait for the rain to leave to see how it holds up with vibration. 

![IMG_20181123_171550|375x500](upload://Adp2ik627Zw4YAOEhkKeTXPCrdI.jpeg) ![IMG_20181123_170800|375x500](upload://iRLX6XrV9FyMwvCSJlmATAGmHqH.jpeg)
```

---
## \#688 Posted by: SeanHacker Posted at: 2018-11-24T20:06:55.795Z Reads: 180

```
Forgot to put a list up of everything I needed for this project @pixelsilva and others. Keep in mind I planned on making 3-4 (maybe more) for my boards so I paid a bit more than usual and I wanted it fast. So I amazon prime and US ebay and had everything within a week or less. Patience will get you a ton more for way less $$$. I'm finally going for my first ride with this today. :slight_smile: 

**Buttons** (I got these for free from a friend. Buy these are the exact same ones.)
https://www.amazon.com/gp/aw/d/B06XT3FLVM?psc=1&ref=yo_pop_mb_pd_title

**JST**
https://www.amazon.com/2-0MM-Female-Single-Connector-Wires/dp/B01JG24NGE/ref=mp_s_a_1_3?ie=UTF8&qid=1543088918&sr=8-3&pi=AC_SX236_SY340_FMwebp_QL65&keywords=JST+PH+2.0MM+7+Pin&dpPl=1&dpID=41R5R2Cst1L&ref=plSrch

**Crystal**
https://www.ebay.com/itm/10pcs-16MHZ-16-000M-HZ-HC-49S-Crystal-Oscillator-Arduino-Raspberry-Breadboard-/231744679631?txnId=1621742042013

**20pf Capacitor**
https://www.ebay.com/itm/20pcs-20pF-NPO-Ceramic-Capacitor-1KV-1000V-5-USA-Seller-/132709069898?txnId=1523894114003

**1N4148 diode**
https://www.ebay.com/itm/10-x-1N4148-Diodes-DO-35-USA-SELLER-Free-Shipping-/173613544043?txnId=1929784759007

**MCU**
https://www.amazon.com/Fii-Atmega328P-PU-Replace-Arduino-Bootloader/dp/B075NRJFJ6/ref=mp_s_a_1_16?ie=UTF8&qid=1543089405&sr=8-16&pi=AC_SX236_SY340_FMwebp_QL65&keywords=Atmega328&th=1&psc=1

**10k ohm resistor**
https://www.ebay.com/itm/100pcs-10K-Ohm-Carbon-Film-Resistor-1-4W-25W-5/122898844268?hash=item1c9d578a6c:g:AXEAAOSwbWZafhbF

**100nf capacitor**
https://www.ebay.com/itm/1uf-Ceramic-Disc-Capacitor-50v-100nf-10pcs-SHIPS-TODAY/163073127306?hash=item25f7ea738a:g:CtAAAOSwf9ta-x7i
```

---
## \#689 Posted by: SeanHacker Posted at: 2018-11-25T01:13:52.788Z Reads: 166

```
https://youtu.be/BzeTtZPlO_4
```

---
## \#690 Posted by: mmaner Posted at: 2018-11-25T01:23:59.259Z Reads: 161

```
Great video, really nice demo.
```

---
## \#691 Posted by: SeanHacker Posted at: 2018-11-25T02:42:43.456Z Reads: 160

```
Thanks dude. I love this thing. Got some new ideas today that will cut it down to 1/3 of the size. I love having this on my board. No more pulling my phone out to check things. :slight_smile:
```

---
## \#692 Posted by: banjaxxed Posted at: 2018-11-25T03:14:55.335Z Reads: 166

```
Watch out for car bitch moves AKA didn’t see you
```

---
## \#693 Posted by: SeanHacker Posted at: 2018-11-25T03:54:43.268Z Reads: 163

```
[quote="banjaxxed, post:692, topic:71509, full:true"]
Watch out for car bitch moves AKA didn’t see you
[/quote]

All day, everyday!
```

---
## \#694 Posted by: janpom Posted at: 2018-11-25T08:37:05.120Z Reads: 177

```
Beautiful! It makes me so happy to see this actually being used. I'm jealous about the weather. It's all grey and rainy here.
```

---
## \#695 Posted by: janpom Posted at: 2018-11-25T17:27:15.168Z Reads: 189

```
Quick demo of the latest developments on the screen layouts and screen toggling.

https://youtu.be/bVz3w26C3og

https://youtu.be/uZS8LQG-Cjk

Each screen layout is now a separate module implementing the [`DavegaScreen`](https://github.com/janpom/davega/blob/multiple_screens/davega_screen.h#L32) interface. A simple example is the [`DavegaTextScreen`](https://github.com/janpom/davega/blob/multiple_screens/davega_text_screen.cpp#L27). The screen modules to be used are then registered [here](https://github.com/janpom/davega/blob/multiple_screens/davega.ino#L65). There can be any number of screens (as long as the program still fits into the flash memory) and the button 3 then toggles between them.

This is not yet in the master branch. I want to add a few final touches before merging, but if anyone wants to play with this, it's already possible.

Note the new [`DISPLAY_ORIENTATION`](https://github.com/janpom/davega/blob/multiple_screens/davega_config.h#L114) option. This is global. If you use a horizontal screen with vertical orientation (or vice versa), it likely won't look correct. There will be some cropping. The `DavegaTextScreen` currently works in either orientation though. The nice thing about this option is that you can easily rotate the screen by 180 degrees should you need that.
```

---
## \#696 Posted by: lrdesigns Posted at: 2018-11-26T06:11:11.271Z Reads: 188

```
@janpom great work on the horizontal version. Didnt think we would get it this soon.

I confirmed my DAVEga will talk to my Vesc. I got the green dot! YESS!

https://media.giphy.com/media/nXxOjZrbnbRxS/giphy.gif


![IMG_1458|375x500](upload://bzkUKucRK0EdloEMIrKgesgXkuK.jpeg) 

I only needed to change two settings on the vesk. App to use, PPM and UART. and. UART baud rate to 115200 bps. And connect the correct pins, which was a little confusing at first.

![image|308x34](upload://j6PPGkf8ZIMNBtTpZK9zUPmIYvu.png) 

![image|380x287](upload://ypTPp4O40SKea0zN2jcyBCDGRnX.png) 

Was tricky to find a really clear image of the pinout with google search but this one was pretty clear, although upside down as its a photo of the under side of the PCB. 

![image|647x272](upload://utcuszEXv2Iu3ykZDoSFT3dBKVz.jpeg) 

This is just temporary hook up to test it works. Some more work needs to be done for final installation. 

![image|681x500](upload://iIwDXhgstCvgYlvQI9cIKrlJELm.jpeg)
```

---
## \#697 Posted by: janpom Posted at: 2018-11-26T21:42:11.164Z Reads: 173

```
New screen layouts merged to the master branch. If anyone would like to test it, that would be much appreciated.

By default, the horizontal layout and the text layouts are used. It can be changed [here](https://github.com/janpom/davega/blob/master/davega_config.h#L129).
```

---
## \#698 Posted by: JonathanLau1983 Posted at: 2018-11-26T22:33:47.090Z Reads: 183

```
Awesome work as always @janpom

I've been making a new horizontal enclosure to work on my Trampa build. The holes for the LCD not being centred really bothered me, so I adjust the spacer on one side so it'll now be symetrical.
![image|689x487](upload://734coNYMsIqYlGZLU1wUjMsAlB1.png) 
![image|624x500](upload://nzgEW6WhbHJLq07JdSKvr4GnHSw.jpeg) 
![image|603x500](upload://sl2r988PGjOINISmmIG7aFJDfJP.jpeg)
```

---
## \#699 Posted by: billappleton Posted at: 2018-11-27T01:41:05.700Z Reads: 169

```
This is awesome. I want one productized not DIY. Is there a vendor here?
```

---
## \#700 Posted by: moon Posted at: 2018-11-27T01:44:30.927Z Reads: 170

```
Case or the whole assembly?
```

---
## \#701 Posted by: lrdesigns Posted at: 2018-11-27T02:23:04.624Z Reads: 182

```
@janpom 

I tried the horizontal version. I'm not sure if its how you structure the folder? But after I download the zip file and un-zip it. I will get an error unless I move all these files into the davga folder. Can you pre-do that on your end? 

![image|319x500](upload://c3Qi9lnK18qAeAU0mWwfsaPlVBS.png)

![image|690x254](upload://5bJfxMBhr3DxDuEsYLA2cAkANpJ.png)  

Looks cool :sunglasses: 

![IMG_1465|666x500](upload://nloaqvexSIuhnfJjfx2JyQOqyaQ.jpeg) 

I miss total distance though?
```

---
## \#702 Posted by: janpom Posted at: 2018-11-27T08:05:46.241Z Reads: 181

```
[quote="lrdesigns, post:701, topic:71509"]
I tried the horizontal version. I’m not sure if its how you structure the folder? But after I download the zip file and un-zip it. I will get an error unless I move all these files into the davga folder. Can you pre-do that on your end?
[/quote]

This is only a problem if you get the code from master. The release packages have the correct directory structure. I'll see what I can do about it. A quick fix is that you rename your `davega-master` folder to `davega`.

[quote="lrdesigns, post:701, topic:71509"]
I miss total distance though?
[/quote]

There's no space for everything. :) You can get the total distance from the text screen (button 3).

I could potentially squeeze three numbers to the right-hand side if I remove the labels. You would just need to remember what is what, which wouldn't be too hard.

If you create a mock-up of the layout that you would prefer (220x176 pixels), I can make it happen. It's really easy now with the screen layout modules.
```

---
## \#703 Posted by: JonathanLau1983 Posted at: 2018-11-27T11:44:16.317Z Reads: 185

```
Overnight print's finished, looks pretty good, symmetry FTW.

![image|666x500](upload://myjqrrkJtvKOJ6AHS7bX5ZTUHhC.jpeg)
```

---
## \#704 Posted by: Jc06505n Posted at: 2018-11-27T12:56:35.551Z Reads: 188

```
Danm this looks interesting ,

[quote="moon, post:700, topic:71509"]
whole assembly?
[/quote]

My lazy ass for one would love whole assembly
```

---
## \#705 Posted by: fafi.azucar Posted at: 2018-11-27T14:31:07.354Z Reads: 180

```
i'm late to the party, but would like to order 1 or 2 or 3😂
```

---
## \#706 Posted by: ROFEN13 Posted at: 2018-11-27T14:54:12.850Z Reads: 177

```
Can you publish the stl. I want to print this!
```

---
## \#707 Posted by: JonathanLau1983 Posted at: 2018-11-27T15:27:59.936Z Reads: 182

```
I need to bolt it together and offer it up to the board to ensure everything is aligned correctly then I'll upload it to Thingiverse.
```

---
## \#708 Posted by: SourPlumGoose Posted at: 2018-11-27T15:42:35.954Z Reads: 186

```
This looks so good. This is a NEED for my trampa. Good work sir!
```

---
## \#709 Posted by: SeanHacker Posted at: 2018-11-28T00:00:57.550Z Reads: 189

```
Damn you guys keep inspiring me. This looks awesome. Nice job dude. 

I decided to make a landscape enclosure now. This is what I have so far. Probably get it finished tomorrow hopefully. 

![IMG_20181127_155141|375x500](upload://39CGeG4FsSw45QrTxREqM92VLmV.jpeg)
```

---
## \#710 Posted by: yelnats8j Posted at: 2018-11-28T00:12:22.037Z Reads: 178

```
Cant wait to try this out 😁😁
```

---
## \#711 Posted by: clistpdx Posted at: 2018-11-28T02:08:35.818Z Reads: 181

```
![image|690x411](upload://hcFJ4J4OVhIADmyKBaTqLOIXOR3.jpeg) 
Here’s a side by side size comparison of the 2 stl’s thst have been posted here. @mmaner on the left and @lrdesigns on the right. I just did a quick PLA print in each to get a rough idea
```

---
## \#712 Posted by: lrdesigns Posted at: 2018-11-28T02:24:58.087Z Reads: 178

```
Nice! Id be interested to know if the dave will fit in mine from your printer. 

Im going to need to make mine bigger to accommodate some buttons. And I want to make a horizontal version.
```

---
## \#713 Posted by: Itsmedant Posted at: 2018-11-28T02:45:11.131Z Reads: 172

```
Can't wait till mine gets here, you guys are doing so much amazing work that this is going to be easy for me!

Seriously, the way this community jumps at the opportunity to help out on an amazing project like this is just phenomenal.
```

---
## \#714 Posted by: janpom Posted at: 2018-11-28T06:59:19.851Z Reads: 168

```
I love the efforts going into the enclosure development. Great work everyone. I think it's time to make space in my apartment for a 3D printer. I mean, it would be a shame to live in Czech Republic and not get the Prusa i3, right? :smiley:
```

---
## \#715 Posted by: Itsmedant Posted at: 2018-11-28T11:15:28.903Z Reads: 169

```
I think the release a Quad extruder recently! That would be a nice one to pick up.
```

---
## \#716 Posted by: mmaner Posted at: 2018-11-28T14:00:58.105Z Reads: 176

```
[quote="janpom, post:714, topic:71509"]
it would be a shame to live in Czech Republic and not get the Prusa i3, right? :smiley:
[/quote]

Yeah, I think it might even be illegal :slight_smile:.  For real tho, Prusa makes some solid badass equipment, you will enjoy it.
```

---
## \#717 Posted by: JonathanLau1983 Posted at: 2018-11-28T21:43:34.211Z Reads: 170

```
Any word on release for horizontal firmware yet @janpom ?
```

---
## \#718 Posted by: janpom Posted at: 2018-11-28T21:48:41.333Z Reads: 177

```
I'll probably release v0.3 in a few days. Until then, feel free to use the master version. It seems reasonably stable.
```

---
## \#719 Posted by: JonathanLau1983 Posted at: 2018-11-28T23:34:13.750Z Reads: 183

```
Got the PCB soldered tonight, but haven't soldered the LCD, use the tissue method. Board is a bit thicker than I originally thought so I will have to adjust my model.
![VescDisplay|304x252](upload://4EelPVINDUr7ZT9e3rayslH965R.gif)
```

---
## \#720 Posted by: SeanHacker Posted at: 2018-11-29T01:31:18.132Z Reads: 188

```
Landscape. Love it! :smile:

![IMG_20181128_154005|375x500](upload://yILJaBhg2dB9bKA58gJdbqjPXhb.jpeg)

![IMG_20181128_161628|665x500](upload://6NYw9IelhQqWJ3jT3LuDEbS5vgR.jpeg)
```

---
## \#721 Posted by: janpom Posted at: 2018-11-30T07:36:26.280Z Reads: 190

```
Installing buttons - lazy way:

![IMG_1536|458x500](upload://6Xs6uyzWYHxMUtcZQCjwDNcJTP9.jpeg) 

![IMG_1535|670x499](upload://p8ptgfP3W2EbqdRut3UlRGrQ05s.jpeg) 

Not extra pretty, but doesn't look terrible either. If we had like 1mm of square depression in the enclosure, so that the buttons could be sunk in a little bit, that would look much better and would make installing these cheap tactile buttons very easy. Just drill two holes, stick the button legs through, add a drop of epoxy, done. WDYT, @mmaner?

BTW, if you're wondering about the big bolt on the right hand side that's purely for decorational purposes... and to cover the hole. :smiley:
```

---
## \#722 Posted by: JonathanLau1983 Posted at: 2018-11-30T09:57:00.856Z Reads: 187

```
Nice one @janpom

Of the three buttons which do you think would be most used? I'm only going to be using two, and I'm not too worried about resetting distance travelled for example, which was switch 1 right?

I've printed what I think is the final version of my enclosure design, so I've now uploaded it to Thingiverse.
https://www.thingiverse.com/thing:3248802
```

---
## \#723 Posted by: Itsmedant Posted at: 2018-11-30T16:10:12.526Z Reads: 183

```
Ah crap, I forgot to order buttons....

I just looked, I ordered all of my stuff through aliexpress the other day and forgot the damn buttons.

Anyone got any extra I can buy a few off of?
```

---
## \#724 Posted by: clistpdx Posted at: 2018-11-30T16:31:22.868Z Reads: 197

```
[quote="lrdesigns, post:712, topic:71509"]
Id be interested to know if the dave will fit in mine from your printer.
[/quote]

![image|666x500](upload://7P9SDdJqWqZmLLVrJQAbVkXU1KZ.jpeg) 
The lcd board is soooo close to fitting. I can easily file down the corners by less than 1mm. But if you squared off the internal corners of your design (rather than rounded corners) it might accommodate a slightly greater tolerance
```

---
## \#725 Posted by: janpom Posted at: 2018-11-30T17:13:41.828Z Reads: 201

```
I have plenty and could ship some to you for free, but it would still take long to US.
```

---
## \#726 Posted by: janpom Posted at: 2018-11-30T17:19:15.377Z Reads: 211

```
Here's my take on the harness. I used a 5 conductor cable and put a JST-XH connector so that I can connect the USB adapter. Then I made an adapter from 5 pin JST-XH to 8 pin JST-PH to use for connecting to VESC. Works like a charm.

![IMG_1540|375x500](upload://e04xdm3eekMhvETFb1NL1oJmVz6.jpeg)

![IMG_1543|558x500](upload://fLFI6r2fWW9nl5SRoa7RHUOa1DX.jpeg) 

![IMG_1542|267x500](upload://q395GEAcRJl6nM0lVRqGdODMIvB.jpeg)

![IMG_1538|575x499](upload://3jbQjSzCkXT38oyoBsb4quWNG5o.jpeg)

![IMG_1539|405x500](upload://rs2zAYg031gfur8bt3Jk4yxxByh.jpeg)
```

---
## \#727 Posted by: janpom Posted at: 2018-11-30T17:31:15.983Z Reads: 206

```
[quote="JonathanLau1983, post:722, topic:71509"]
Of the three buttons which do you think would be most used?
[/quote]

The trip reset (button 1) seems the most important to me and will become even more important; see below. The screen toggle (button 3) would be the second most used for me and the coulomb counter reset (button 2) the least used. If you charge your batteries to 100% or don't care about the coulomb counter (set `VOLTAGE_WEIGHT 1.0`), then you may not need the button 2 at all.

About the button 1: I'm about to introduce the concept of session data. That's what you'll likely want to reset before each ride, such as:
- trip distance
- time elapsed
- time elapsed riding
- max speed
- avg speed
- max motor current
- min motor current (=max braking current)
- etc

The responsibility of the button 1 will then be to reset all the session data. In fact, it already does this, but the only session data item we currently have is the trip distance. :slight_smile: That's soon to be changed though.
```

---
## \#728 Posted by: swimmydude Posted at: 2018-11-30T18:28:49.064Z Reads: 184

```
I actually have a bunch myself and I'm located in US. If you just pay shipping, I'll give you some. I'm not sure what size is needed since I haven't received my packet yet.
```

---
## \#729 Posted by: Itsmedant Posted at: 2018-11-30T19:23:36.097Z Reads: 184

```
okay cool! Just let me know when it gets time for it! I'm going to be waiting a bit for all of my stuff too so I'm not in a super rush.
```

---
## \#730 Posted by: janpom Posted at: 2018-11-30T20:03:38.510Z Reads: 188

```
FW v0.3 released: https://github.com/janpom/davega/releases/tag/v0.3
```

---
## \#731 Posted by: SeanHacker Posted at: 2018-11-30T20:42:26.652Z Reads: 194

```
Great job dude!!! You're killing it. :smile: 

![IMG_20181130_124009|665x500](upload://i0ZNiTdpPYxNXkk0JjvqjqNmwng.jpeg)
```

---
## \#732 Posted by: fafi.azucar Posted at: 2018-11-30T22:30:25.866Z Reads: 195

```
when's the next phase?
```

---
## \#733 Posted by: SeanHacker Posted at: 2018-12-01T00:38:51.708Z Reads: 196

```
I was just scrolling through my old videos and realized that @janpom fulfilled something that I've wanted for a while, just couldn't find something that I liked. I fucking love this little thing!

**Back then...**
https://youtu.be/7lAlMHWferA

**Now...**
https://youtu.be/mouUeJYaPiE
```

---
## \#734 Posted by: banjaxxed Posted at: 2018-12-02T10:22:11.418Z Reads: 195

```
Thank you, too lazy and hung over from other voices fest to switch out carbonfil to TPU, but it came out nice, I have a Proton on backorder from some time ago, this probably has everything I realistically want.

Nice![IMG_9423|666x500](upload://ugBLdtcM3Z3u1J2ux1TlyTGttHw.jpeg)

Ps. 30% gyroid infill is so rock solid
```

---
## \#735 Posted by: skelstar Posted at: 2018-12-02T17:50:43.655Z Reads: 187

```
I immediately took notice of your part cooling fan assembly on your printer :)
```

---
## \#736 Posted by: banjaxxed Posted at: 2018-12-02T18:02:41.533Z Reads: 186

```
It does the job, no support under 70deg
```

---
## \#737 Posted by: janpom Posted at: 2018-12-03T20:26:52.337Z Reads: 194

```
Here's a version of the "simple horizontal layout" for those who prefer the vertical orientation. I also managed to squeeze in two more numbers. This is my favourite layout so far. I like the yellow on the speed. It will make me want to go fast in order to keep my Dave looking sexy. :smiley:

![IMG_1550|452x500](upload://x9gusHVEGYXTfxPbatqHQTEjcIu.jpeg) 

It looks much better live, especially in @mmaner's enclosure!
```

---
## \#738 Posted by: Andy87 Posted at: 2018-12-03T21:09:42.444Z Reads: 189

```
Today I made it through all the comments again.
Now I need only to read a bit more about how to flash the software. Which programs I need and which files from the GitHub are the once I need to select... as noob in this it looks for me always just a punch of file on one place. Which from them really necessary I didn’t understood 😅yet ☝️ 
Just to confirm that I got it right.
The speed is calculated by the gearing, right?
And the gearing parameters I have to change according to what I currently use on my build in the file I upload to the arduino?
```

---
## \#739 Posted by: Mich21050 Posted at: 2018-12-03T21:14:42.119Z Reads: 183

```
Ok so im also not really good at programming but you need the Arduino IDE Software, the davega firmware that you can download under releases on github. You also need to install the libraries that @janpom mentioned on his github readme. Once you got everything up and running you need to go to the config tab and fill in all the parameters.... :slight_smile:
The readme on github provides a pretty good overview of everything else that you need to to...
@janpom please correct me if I'm wrong :smile:
```

---
## \#740 Posted by: janpom Posted at: 2018-12-03T21:25:28.051Z Reads: 191

```
@Andy87 [Here's](https://github.com/janpom/davega#configuring-and-installing-firmware) the guidelines. If anything is unclear there, please let me know. I'll try to help and also update the README.
```

---
## \#741 Posted by: JonathanLau1983 Posted at: 2018-12-04T00:04:14.781Z Reads: 195

```
Here's my progress, just waiting on some multicore cabling to arrive to wire it properly but I've wacked it onto the board to see how it looks.
I've wired up buttons 1 and 3 as suggested.
@janpom when using button 1 to clear data, can there be something which flashes up? At the moment it's very hard to tell anything's happened, all I see is the green blinking box blink red once which is easy to miss.

https://www.youtube.com/watch?v=EovqvrPSGT4
```

---
## \#742 Posted by: Devilmycry Posted at: 2018-12-04T04:32:53.973Z Reads: 188

```
Where I can get this look a beautiful
```

---
## \#743 Posted by: janpom Posted at: 2018-12-04T05:57:45.712Z Reads: 196

```
You need to press and hold the button 1 for 3 seconds. The trip distance will gradually disappear. When you release the button it's reset.

Nice enclosure. Looks great!
```

---
## \#744 Posted by: lrdesigns Posted at: 2018-12-04T06:46:52.690Z Reads: 202

```
Found some time to solder some wires and a connector to my vesc. It works! 
https://media.giphy.com/media/5BWswJK1ZmPyAeVgMh/giphy.gif
```

---
## \#745 Posted by: amazingdave Posted at: 2018-12-04T09:42:09.147Z Reads: 198

```
I’m feeling so left out of all this!! Still waiting on my screens....
```

---
## \#746 Posted by: mmaner Posted at: 2018-12-04T16:56:47.920Z Reads: 199

```
I still cant get mine to work :sob:.  It powers on and shows the initial screen, but all I get is the flashing red dot and no VESC connection.  I  uploaded the standard 3.4 firmware to a pair of FocBox's.  Didn't change anything.  I've double checked my VESC cable (JST 2.0 7 pin).  Any ideas what I should start looking at?  I'll post some pics tonight when I get home.
```

---
## \#747 Posted by: JonathanLau1983 Posted at: 2018-12-04T17:07:49.800Z Reads: 198

```
Got a picture of your wiring?
```

---
## \#748 Posted by: mmaner Posted at: 2018-12-04T17:13:52.751Z Reads: 193

```
I don't, but I'm pretty sure its good.  Ill post pics when I get home tonight.
```

---
## \#749 Posted by: JonathanLau1983 Posted at: 2018-12-04T17:15:12.643Z Reads: 191

```
Only time I had the same issue was when one of my wires between the board and the Foxbox broke. So I now goop on some hot glue around the connectors.
```

---
## \#750 Posted by: mmaner Posted at: 2018-12-04T18:05:03.322Z Reads: 185

```
I haven't even mounted it on the board yet, In fact the display isn't even soldered to the PCB yet.  I didn't wanna do those until I was sure it worked.
```

---
## \#751 Posted by: Andy87 Posted at: 2018-12-04T18:43:17.277Z Reads: 193

```
So, unfortunatelly i have less time as i would like to have for our davega, but I started today with the first things.
I changed the colors of the wires in the jst plug which goes to the vesc. As i will try it out First with a focbox i looked up deep into my diy case and found one last 2mm 7pin jst 🙏 for the focbox side.
![image|690x419](upload://yrDspuNP039Vk4IcMVA4cUpoela.jpeg) 

![image|690x415](upload://bYPZ8VswV2Bj7lWqks3zcXI4ovl.jpeg) 

Soldering can be done only on the weekend, but as min now everything ready for it.

I had some 2.5mm standoffs for pcbs and they perfectly fit as spacer between pcb and display.
(Ok i needed a bit of drilling the holes out in the pcb... but besides perfect fit)

![image|690x390](upload://sYPe97gTDb1a5mxNbB6eiCqZPHH.jpeg) 

Is it ok if the pins from the displays are open like on the picture?

I also not sure, in my set there where 4puttons. On the pcb only three places to solder them on.
Is it just one spare or do I need it later as Boot reset or something like this?
```

---
## \#752 Posted by: SeanHacker Posted at: 2018-12-04T19:32:26.258Z Reads: 176

```
Have you selected UART and set the baud rate to  115200 by chance yet @mmaner?
```

---
## \#753 Posted by: Itsmedant Posted at: 2018-12-04T19:35:30.500Z Reads: 174

```
My screen shipped from aliesxpress at the end of last week. So everyone, solve all the problems so by the time mine gets here, it will be nice a documented on what not to do for me!
```

---
## \#754 Posted by: venom121212 Posted at: 2018-12-04T19:53:58.495Z Reads: 173

```
Same here haha
```

---
## \#755 Posted by: mmaner Posted at: 2018-12-04T20:08:24.185Z Reads: 172

```
Yes sir :slight_smile:
```

---
## \#756 Posted by: JonathanLau1983 Posted at: 2018-12-04T20:14:11.457Z Reads: 176

```
Tx pin going to Tx, Rx to Rx?
```

---
## \#757 Posted by: mmaner Posted at: 2018-12-04T20:51:23.736Z Reads: 181

```
I assume so, Ill have to check and see if I reversed them or not.  If I remember correctly, I tried it both ways.
```

---
## \#758 Posted by: janpom Posted at: 2018-12-05T07:24:53.870Z Reads: 182

```
I have two FOCBOXes now that @brenternet sent to me along with his Vera build, which I was kind enough to accept as a payment for the [correctly branded Dave](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/213?u=janpom) (though I still feel like it's a bit insufficient given the [complexity of the re-branding](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/211?u=janpom)).

I'll test the Dave with focboxes over the weekend and let you know if I find any issues.
```

---
## \#759 Posted by: lrdesigns Posted at: 2018-12-05T07:59:00.538Z Reads: 193

```
[quote="mmaner, post:746, topic:71509"]
I uploaded the standard 3.4 firmware to a pair of FocBox’s. Didn’t change anything.
[/quote]

I am running the latest @Ackmaniac firmware so it is not the firmware I don't think.  

I got the DAVEga temporarily mounted in my lunch box for its first real world test. :grin: Bit of tight fit, looks like a fire hazard. :flushed: 

![Photo%20Dec%2005%2C%203%2020%2040%20PM|666x500](upload://4474IW7g2QfehoDEGpfc29S7T7C.jpeg) 

![Photo%20Dec%2005%2C%203%2019%2045%20PM|666x500](upload://62ExMRRCdKVJfrK3nPXFdG8JLd5.jpeg) 

![Photo%20Dec%2005%2C%203%2023%2020%20PM|666x500](upload://pzIrPJIR4di8olFJb4HcxsuMBkg.jpeg)
```

---
## \#760 Posted by: janpom Posted at: 2018-12-05T08:49:59.832Z Reads: 181

```
[quote="Andy87, post:751, topic:71509"]
Is it ok if the pins from the displays are open like on the picture?
[/quote]

Yes, looks good.

[quote="Andy87, post:751, topic:71509"]
I also not sure, in my set there where 4puttons.
[/quote]

The fourth is just a spare.
```

---
## \#761 Posted by: lrdesigns Posted at: 2018-12-06T00:26:05.360Z Reads: 179

```
I have a  bug :spider: report. Mine will freeze if I pull too much amps. If I go really slow it does not freeze and not on the bench with wheels spinning free. Even on brakes with high load it will freeze, tested from top of hill. The only way to unfreeze is to reboot the vescs. 

![IMG_1538|666x500](upload://kPJU2mzbdV1EYuSb5LEcJ0rp7Nx.jpeg)

I am using the master horizontal version. So I am going to change to the V0.2 version and see if that is different. If not I will try the DAVEga in a different location. It's probably something to do with my setup being so crammed in will all the wires so close.
```

---
## \#762 Posted by: janpom Posted at: 2018-12-06T02:24:16.632Z Reads: 178

```
Dear Luke, 

Thank you for contacting the DAVEga technical support. I understand your Dave freezes when you pull too much power from your electric skateboard. My name is Jan and I will assist you with the problem.

First off, I want you to know that it makes me happy personally that you have lent us time on letting us know regarding this matter.

I have filed a support case for your issue under the number 000001. Please use this reference for any further contact regarding the problem.

Before I pass on the issue to the development team, let me try to get more insights. Could you please confirm whether you have tried turning the DAVEga off and on again without rebooting the VESC?

As a temporary workaround, you could try going slowly and not use your brakes. Alternatively, you could push your board around to further reduce the power drawn by the VESC and prevent the freezing issue. Please let me know whether this is an acceptable workaround.

Luke, I highly value the trust that customers like you place on us. Rest assured that we strive to provide you with excellent service.

Thank you for choosing DAVEga.

Sincerely,
Jan P.
DAVEga Technical Support
```

---
## \#763 Posted by: lrdesigns Posted at: 2018-12-06T02:29:33.727Z Reads: 163

```
Uahh customer service bots. 

Yes turn board on and off to reboot. Everything off.
```

---
## \#764 Posted by: janpom Posted at: 2018-12-06T02:38:25.097Z Reads: 175

```
Seriously though, this sounds like a hardware problem. What kind of VESCs do you have? Maybe the 5V power supply from the VESC gets unstable under high load. I haven't encountered this specific problem myself. I do remember that my Dave once started behaving strangely when my batteries got very low. First I thought that was a software issue (some overflow/underflow related to unexpectedly low value of the battery pack voltage), but I haven't been able to reproduce it, so I think that must have been a HW problem as well. It didn't really freeze though. Rather, the screen got distorted.

Maybe adding an electrolytic capacitor as a power supply buffer would help.

Could you please first try whether changing the location helps?

Also, I understand it completely freezes. The little green/red square doesn't blink, right?
```

---
## \#765 Posted by: lrdesigns Posted at: 2018-12-06T05:49:46.948Z Reads: 182

```
Yes a complete freeze, no blinking light. 

DAVEga firmware version and location did not fix it. I will try a power smoothing cap. My other theory is the wires I have extended for the buttons are picking up some RFI, like what happened with the unity. So will trim those if the cap dont  work. The button wires are about 12cm long.

https://www.electric-skateboard.builders/t/focbox-unity-official/64944/867?u=lrdesigns


Sometimes there is strange artifacts when frozen that are amusing. 

![Photo%20Dec%2006%2C%201%2024%2021%20PM|375x500](upload://twrpDbLMjMUW6T2tX76A4uTP2tq.jpeg) ![Photo%20Dec%2006%2C%201%2030%2019%20PM|375x500](upload://oit8uBHzZAFPRA4vYyev7exi4eu.jpeg) ![Photo%20Dec%2006%2C%201%2026%2027%20PM|374x500](upload://lyT881h82FLcCx3DTa0HI798ru9.jpeg) ![Photo%20Dec%2006%2C%201%2033%2043%20PM|374x500](upload://afVIVg9s0HFbQD6USsz9l6sb0D1.jpeg) 

Temporary mounting. :wink:

![Photo%20Dec%2006%2C%201%2028%2010%20PM|374x500](upload://8qEhXKG3gjLjU3gRBHkyHQODbRW.jpeg) ![Photo%20Dec%2006%2C%201%2029%2016%20PM|666x500](upload://A5UguQej3EjDKnO63Yt13a3r5On.jpeg) 


I much prefer the newer graphics with huge numbers.
```

---
## \#766 Posted by: janpom Posted at: 2018-12-06T07:21:14.663Z Reads: 165

```
This is great info, thanks. Nice mounting! Lends a very professional look to the board! :smiley: 

The smoothing cap is worth a shot. You could use the debug pins for it -- solder it between 5V and GND.
```

---
## \#767 Posted by: JonathanLau1983 Posted at: 2018-12-06T09:33:24.107Z Reads: 164

```
That's a good shout, might do the same just incase closer to the VESC end.
```

---
## \#768 Posted by: High-roller Posted at: 2018-12-06T17:03:09.259Z Reads: 166

```
@janpom could you please post links to the GitHub files and any assembly tips at the top of the thread so they'll be easier to find?
```

---
## \#769 Posted by: Mich21050 Posted at: 2018-12-06T17:04:50.615Z Reads: 166

```
https://github.com/janpom/davega
@High-roller
```

---
## \#770 Posted by: banjaxxed Posted at: 2018-12-06T19:40:13.692Z Reads: 159

```
Real support would have provided the workaround of going back to v0.2, keeping the LCD in landscape and turning your head sideways
```

---
## \#771 Posted by: lrdesigns Posted at: 2018-12-07T00:56:01.218Z Reads: 167

```
[quote="clistpdx, post:724, topic:71509"]
The lcd board is soooo close to fitting. I can easily file down the corners by less than 1mm. But if you squared off the internal corners of your design (rather than rounded corners) it might accommodate a slightly greater tolerance
[/quote]

Ohh yeah. I did file the corners on my DAVEga and LCD. The reason for the radius is there is concentric circles coming out from that corner, so that the o-ring groove can have a smooth corner and the wall thickness is even. 

I think your print quality is quite nice! 

![IMG_1580|666x500](upload://kurhJpVWWBWJvDJunBLqqaPthyJ.jpeg)
```

---
## \#772 Posted by: lrdesigns Posted at: 2018-12-07T05:37:36.039Z Reads: 164

```
Soldered in a 2200uF 25v cap, was all I had on hand. Its very large for the application. Didn't find a decent place to put it so its half way along the wires from vesc to DAVEga. 

I had just a few minutes on my lunch break, did a few up and down runs on a steep hill. So far it seems to have solved the issue. Thanks! @janpom 

 ![IMG_1581|666x500](upload://46SpQjUbTjzkXqkUDW78qrZyNEE.jpeg)
```

---
## \#773 Posted by: Andy87 Posted at: 2018-12-07T05:55:44.147Z Reads: 158

```
So the reason who cause the cut out was the too long signal wires?
Just to get it as noob ;)
So if you use signal wires longer than let´s say 25cm you will need an extra cap to  get a stable signal.
```

---
## \#774 Posted by: lrdesigns Posted at: 2018-12-07T05:59:15.644Z Reads: 157

```
I think it caused by unstable 5 volts from my vesc. Or noise in the 5v line. It might be the vesc, or the fact that I have soldered to the pads on the vesc directly, so it might not be the best connection, the negative pad is connected to a huge ground plane and is very difficult to get hot enough for a good solder joint. My vescs are maytech 4.12.
```

---
## \#775 Posted by: lrdesigns Posted at: 2018-12-07T06:31:23.119Z Reads: 163

```
[quote="janpom, post:702, topic:71509"]
If you create a mock-up of the layout that you would prefer (220x176 pixels), I can make it happen. It’s really easy now with the screen layout modules.
[/quote]

Something like this? I think it can all fit. Sorry I didn't make it the correct pixel size, though I could with a little more time.

The battery percentage could be smaller, you already have the battery bar so its just extra info.

![image|594x500](upload://4swPJKJNLQUV4PBsNYhNoBUdDp1.jpeg)
```

---
## \#776 Posted by: Andy87 Posted at: 2018-12-07T06:41:29.440Z Reads: 156

```
The FAULT is always visible? or only when a fault occures?
```

---
## \#777 Posted by: lrdesigns Posted at: 2018-12-07T06:42:19.893Z Reads: 152

```
Only when you get a fault. Otherwise how would you know you got one? :thinking:
```

---
## \#778 Posted by: Andy87 Posted at: 2018-12-07T06:49:12.729Z Reads: 152

```
if FAULT would change to the text like DRV of ABS over Current etc.
but that would be confuseing, that´s why I asked to be sure it´s not permanent.
```

---
## \#779 Posted by: lrdesigns Posted at: 2018-12-07T06:51:47.970Z Reads: 150

```
Yeah if it could list the actual fault that would be even cooler. Not sure how easy it is to do? This is just like the minimal information, let you know to check it. I guess you can see the full fault on the second info screen or plug vesc into usb before shutting your board down. 

But yeah, no red bars unless there is a fault, so its really obvious.
```

---
## \#780 Posted by: janpom Posted at: 2018-12-07T06:54:22.677Z Reads: 146

```
Looks good. I will implement it when I find some time.

If there's a fault, the fault code is displayed instead of the battery indicator. See [here](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/695?u=janpom) at 0:05.
```

---
## \#781 Posted by: janpom Posted at: 2018-12-07T06:58:53.420Z Reads: 146

```
Great that it seems to help. Please do some more testing and let us know if the problem is really gone (don't forget to use reference number 000001 :smile:). If it is, I will make space for the cap on the next version of the PCB. Seems like a good thing to have there.
```

---
## \#782 Posted by: janpom Posted at: 2018-12-07T07:31:36.951Z Reads: 151

```
@lrdesigns Could also please test if a smaller cap would still work. The biggest I can fit between the PCB and the display would be something [like this](https://www.aliexpress.com/item/16v-22uf-Axial-Electrolytic-Capacitor-5x13mm-100pcs-Hongkong-post-tracking-number-Free-Shipping/2047158667.html?spm=2114.search0104.3.270.2bd624f5P1pDwK&ws_ab_test=searchweb0_0,searchweb201602_3_10065_10068_319_317_10696_10084_453_454_10083_10618_10304_10307_10820_10821_538_537_10302_536_10059_10884_10887_100031_321_322_10103,searchweb201603_2,ppcSwitch_0&algo_expid=bd38894c-8fa7-4cf0-9a71-64c5176fa236-41&algo_pvid=bd38894c-8fa7-4cf0-9a71-64c5176fa236) (22 uF, eletrolytic axial), so that would be 100 times lower capacity than what you're using now.
```

---
## \#783 Posted by: janpom Posted at: 2018-12-07T13:42:45.090Z Reads: 164

```
@mmaner I tested Dave with my new focboxes today and it worked fine with both. I used the standard 3.40 FW and pretty much default settings.

Here's how it should be correctly wired up.
- TX-TX
- RX-RX

![IMG_1559|375x500](upload://ivVkpupOf411VyT71KHjj2s5UWx.jpeg)  

I'm guessing the problem is in the TX/RX wires. Please double-check for any loose connection or even bad solder joins on the PCB. I hope you can make it work! :crossed_fingers:
```

---
## \#784 Posted by: mmaner Posted at: 2018-12-07T13:45:47.407Z Reads: 159

```
I am pretty sure mine is wired up the same way.  I've been really busy all week at works, so haven't had time to work on this more but I will be working on it saturday.  Ill double check my wiring and solder connections.  Thanks
```

---
## \#785 Posted by: lrdesigns Posted at: 2018-12-07T14:55:15.726Z Reads: 163

```
[quote="janpom, post:762, topic:71509"]
As a temporary workaround, you could try going slowly and not use your brakes. Alternatively, you could push your board around
[/quote]

What are you insane? 

https://giphy.com/gifs/nzFhajbsYJhDO
```

---
## \#786 Posted by: lrdesigns Posted at: 2018-12-07T15:03:00.724Z Reads: 164

```
Works! 
![image|667x500](upload://9gJ8hSTofl4y5e0uHsP2UWMJYLs.jpeg)
```

---
## \#787 Posted by: Mich21050 Posted at: 2018-12-07T19:55:24.220Z Reads: 166

```
Ok so just a quick note:
If you experience this:
![20181203_171442|281x500](upload://htYt5OiHGLGm4mLz61biKXXP78z.jpeg) 
You just need to change the last parameters in the config to the following:
![Unbenannt_davega|289x187](upload://oSAASEe4qdmoMTw03Lb49TmmGAg.png) 
@janpom Thank you again for your patience and help :slight_smile:
Also my vesc cables are 60cm long and I don't experience any problems (I'm using a hk vesc) :slight_smile:
```

---
## \#788 Posted by: lrdesigns Posted at: 2018-12-08T05:40:59.396Z Reads: 168

```
@janpom tried 100uF cap and 90cm wire extension. Wire is very thin and un-shielded. Cap is near vesc while davega is at the other end. Seems to work fine after one short ride. 

![image|375x500](upload://5ZYBEXNvMyMPvmouLjQRUvhUbBC.jpeg) 

![image|375x500](upload://mh60CNVIwDvWUHKtxlbZ2sz4CtY.jpeg)
```

---
## \#789 Posted by: janpom Posted at: 2018-12-08T07:16:23.109Z Reads: 159

```
Perfect! This is exactly the kind of testing that was much needed. Thanks a lot!
```

---
## \#790 Posted by: Andy87 Posted at: 2018-12-08T17:59:09.537Z Reads: 164

```
It’s on... 🙌
As total noob and first time arduino user i can say @janpom you github description is super clear. I didn’t have had the right usb driver installed but even those where linked in the description.
I had to modify the tissue mode a bit to get the display working, but besides it’s no as min showing something.

![image|375x500](upload://rKdxf08fEmpzCFHRCrL0zORzMO8.jpeg)  

The only thing which is not working now is to switch between displays.
Did I forgot to enable that in the parameters?
Or is something wrong with my switches?


PPS: @janpom my smart bms arrived today. Seems like it is for 12s LiIon 
![image|375x500](upload://pYWwZZsAVhF8EXPDIlqJUnOk8Mn.jpeg)
```

---
## \#791 Posted by: janpom Posted at: 2018-12-08T18:08:40.901Z Reads: 157

```
@Andy87 Great! I'm glad you made it working. It seems like you're actually not getting data from the VESC (it's showing 0% battery). That's the reason you can't toggle between screens. This is actually a minor bug that I plan to fix at some point. Dave is stuck in the initialization phase until it gets the first reading from the VESC and in this phase it's not possible to switch screens. You're probably in the same stage as @mmaner now. You'll want to check your RX/TX wires and your VESC UART settings (UART enabled, baud rate set to 115200).
```

---
## \#792 Posted by: Mich21050 Posted at: 2018-12-08T18:08:42.856Z Reads: 154

```
The buttons will only work when its connected to the vesc :slight_smile:

@janpom sorry... its your awesome device. :slight_smile:
```

---
## \#793 Posted by: janpom Posted at: 2018-12-08T18:12:02.045Z Reads: 163

```
[quote="Andy87, post:790, topic:71509"]
PPS: @janpom my smart bms arrived today. Seems like it is for 12s LiIon
[/quote]

Cool! I'm still waiting for mine. I wonder what I'll get. :D The seller responded to my message and assured me they would send me the right thing. (We're in the wrong thread with this. Sorry for off-topic everyone.)
```

---
## \#794 Posted by: Andy87 Posted at: 2018-12-08T18:45:19.291Z Reads: 162

```
🙈 i just realized 5min after I wrote the last post that it need to be a connection problem 😅
Swapped rx/tx and it’s functioning.
Fault code indicator works too 👌🙈
![image|375x500](upload://s8PXn0dJ426ZIj13WnfcTA9vdZa.jpeg) 

Strange thing, I knew there is a vault on the focbox but it wasn’t show in the terminal which fault.
```

---
## \#795 Posted by: janpom Posted at: 2018-12-08T23:33:13.718Z Reads: 155

```
Does anybody know where to get some small axial electrolytic capacitors with a reasonable capacity (5V rating sufficient)? I spent quite a bit of time looking on ebay, banggood, aliexpress, but couldn't really find anything suitable. The diameter has to be 5mm or less. The best thing I have found so far is [this](https://www.gme.cz/cea-22u-40v-vis-asm-4-5x10) in my local electronics store. The dimensions are just about perfect. The 40V rating is unnecessary though. I wish there was more capacity instead. They are also a bit expensive. 17 CZK is almost $1.
```

---
## \#796 Posted by: b264 Posted at: 2018-12-09T00:00:12.639Z Reads: 153

```
Do Digikey or Aliied Electronics carry them?
```

---
## \#797 Posted by: clistpdx Posted at: 2018-12-09T00:01:15.731Z Reads: 154

```
What amount of capacitance are you wanting in the cap? I see [10uF ones here](https://www.ttiinc.com/content/ttiinc/en/apps/part-detail.html?mfrShortname=NIC&partsNumber=TVX1H100MAD&customerPartNumber=&minQty=50&customerId=), or [22uF ones here](https://www.ttiinc.com/content/ttiinc/en/apps/part-detail.html?mfrShortname=NIC&partsNumber=TVX1E220MAD&customerPartNumber=&minQty=50&customerId=). Or on mouser.com they show [77 axial caps](https://www.mouser.com/Passive-Components/Capacitors/Aluminum-Electrolytic-Capacitors/_/N-75hqt?P=1yzxn99&Keyword=electrolytic+capacitors+axial&FS=True) with 5mm diameter.
```

---
## \#798 Posted by: janpom Posted at: 2018-12-09T04:25:03.808Z Reads: 158

```
The mouser filters are great. I found [this guy](https://cz.mouser.com/ProductDetail/Vishay-BC-Components/MAL202124101E3?qs=sGAEpiMZZMu3dWSqd4Tl0IrB%252bE%2fYPbXzdcGGOLzGjbQ%3d) there, which is a perfect fit, if still a little pricey.
```

---
## \#799 Posted by: kalebludlow Posted at: 2018-12-09T04:50:06.668Z Reads: 163

```
Skimmed through the last month's worth of comments and couldn't find an answer, so I'm wondering if there are still kits or preassembled for sale?
```

---
## \#800 Posted by: swimmydude Posted at: 2018-12-09T08:57:01.696Z Reads: 165

```
Currently, I don't think so. It's still going through the beta testing phase. Though I'm sure if you really wanted to, someone might have the pieces needed.
```

---
## \#801 Posted by: janpom Posted at: 2018-12-09T09:19:32.972Z Reads: 171

```
So I've been thinking about how to do the second batch. I'm already preparing for it. I'm awaiting 50 new MCUs.

It seems that many would prefer an assembled kit, but then again this is an DIY forum and I'm sure many will prefer to assemble the Dave on their own as well. I don't want to offer multiple options since dealing with orders is already time consuming even if I make it as simple as possible. I would like to have one standard package with one price for everyone, so that I can prepare sealed envelopes to be shipped and whenever someone orders one, I just stamp on their address and take it to the post office. Also, though the untracked shipping worked well so far, many packages got delayed and people got nervous about not knowing where their package is.

With this in mind, here's how I would like to go about the batch 2. Each package will have two Daves, one assembled and one kit. That way, everyone will get at least one functional and everyone will have a chance to build another one, either to keep as a spare or to give to a friend. Having the assembled one on hand will then provide a template and should make the assembly easier. The price will be higher, which will the $5 for tracked shipping not sound so ridiculous compared to the value of the package.

I plan to set the price at $25. This includes $5 shipping, accounts for PayPal fees and exchange rate losses (since apparently not everyone wants/manages to pay as F&F and sometimes the money paid gets converted to CZK for no obvious reasons), the costs of the parts (I'll be adding electrolytic caps to the next generation to protect against volatile power supply that @lrdesigns has experienced, so that's minor extra cost) and if I'm lucky there will be $1-2 left for myself, so that I can tell my wife I'm actually making money on this! :laughing:

Also, @Mich21050 volunteered to help with completing, assembling, and distributing kits for no charge, which I really appreciate, but at the same time I think it would be nice to leave some padding in the price for him as tips. He's a young fella and I'm sure he'll make good use of a few extra bucks.

With the displays, that will be $35 for 2 Daves, or $17.5 for one, which is quite a bit more than the $10 that I promised, but hopefully still affordable for everyone who wants one... eh, I mean, two. :smiley:

I would like to get your thoughts on this, guys.
```

---
## \#802 Posted by: ROFEN13 Posted at: 2018-12-09T09:25:59.254Z Reads: 152

```
$35 for two of these is still amazingly low for what it is. The only other option for something like this is the photon control panel, which does have more features, but that is $115.
```

---
## \#803 Posted by: Skunk Posted at: 2018-12-09T09:29:57.609Z Reads: 156

```
Sounds good to me.
```

---
## \#804 Posted by: amazingdave Posted at: 2018-12-09T09:30:10.984Z Reads: 156

```
That is still incredibly cheap for a 2 pack. The one built and one kit is a good idea.
```

---
## \#805 Posted by: bigben Posted at: 2018-12-09T09:34:08.044Z Reads: 156

```
Fantastic pricing. These will be on every new build for sure.
```

---
## \#806 Posted by: kalebludlow Posted at: 2018-12-09T09:49:46.517Z Reads: 155

```
Definitely a must buy
```

---
## \#807 Posted by: ElectricCoast Posted at: 2018-12-09T10:26:14.049Z Reads: 155

```
I think the pricing is amazing and I'd purchase a couple.
```

---
## \#808 Posted by: 257 Posted at: 2018-12-09T19:29:54.808Z Reads: 152

```
Great idea including a complete and a kit! Building with a template would be very helpful for me. 

Thank you for developing this awesome thing :smiley:
```

---
## \#809 Posted by: SeanHacker Posted at: 2018-12-09T19:38:50.678Z Reads: 159

```
[quote="janpom, post:801, topic:71509"]
$17.5 for one, which is quite a bit more than the $10 that I promised
[/quote]

It's really not much more considering they get an already assembled unit. I can almost guarantee people would pay a bit more for something like this. I like your style though dude. I'm super impressed at what you've done so far and I can't imagine not having my Dave on my board.  

P.S- I'll buy a two pack whenever you have them. Maybe a couple two packs. I have plans for a couple other boards this winter. This option will make it way easier. Thanks again for everything you've done so far!

![IMG_20181203_090727|665x500](upload://81j4R8UhjJYRpzZ4di6DStvl47c.jpeg)
```

---
## \#810 Posted by: venom121212 Posted at: 2018-12-09T19:49:41.148Z Reads: 152

```
That looks really great man. Mind showing a pic of the mounting/routing underneath if/when it's convenient?
```

---
## \#811 Posted by: lrdesigns Posted at: 2018-12-10T01:14:59.595Z Reads: 149

```
Even $20 is crazy cheap for a fully assembled one, that includes shipping and paypal fees? Get outta here. 

After a few rides its really fun / nice but @janpom I am REALLY excited to have min/max information on the second or third screen. Any chance we can get that before xmas? :christmas_tree:  

I really would like to know min / max amps (battery), min voltage (sag) and max speed.
```

---
## \#812 Posted by: mmaner Posted at: 2018-12-10T01:19:04.923Z Reads: 156

```
I finally got off my ass and got mine finished and installed. I still need to make some adjustments to my model, I need better soacing for the button holes and an imset on the inside for the micro momentary buttons. 

https://youtu.be/N3Xu8UC1xj4

This thing is frikkin awesome.
```

---
## \#813 Posted by: SeanHacker Posted at: 2018-12-10T01:21:56.457Z Reads: 152

```
Yep. I'll grab some shots tomorrow for you.
```

---
## \#814 Posted by: clistpdx Posted at: 2018-12-10T04:12:56.614Z Reads: 154

```
Do you have a button to suggest that fits your cutouts? All I've got are square buttons, but can't seem to locate circular ones that fit your design
```

---
## \#815 Posted by: mmaner Posted at: 2018-12-10T04:14:23.991Z Reads: 158

```
My buttons are square too, just hot glue them in place, print a small round plug (slightly smaller than the slot) and glue it to the button. 

I'll update my model tomorrow or Tuesday with better soacing and button plugs.
```

---
## \#816 Posted by: lrdesigns Posted at: 2018-12-10T04:40:39.411Z Reads: 163

```
I am working on an angled base for my case. So that there is room for buttons. Currently its just 3M double taped to my surfrodz reinforcing plate. There is holes so I can still undo the trucks if need be. 

Using the smallest waterproof switch I could find, it has a 8mm hole and 12mm head. Same one as @JonathanLau1983 found. [Ebay](https://www.ebay.com/itm/2pcs-8mm-Mini-Micro-2Pin-Metal-Waterproof-Momentary-Push-Button-Switch-TEUS/142899473216?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649) - [Aliexpress.](https://www.aliexpress.com/item/1pc-8mm-Momentary-Metal-Stainless-Steel-Horn-Doorbell-Bell-Push-Button-Switch-Waterproof-Car-Auto-Engine/32822845113.html?spm=a2g0s.13010208.99999999.265.799f3c00R2hJW6)  

![image|690x326](upload://4ROFr46AfpNh1aaGBo8DnNV1oDg.jpeg) 

![image|653x500](upload://zOv37iF5JElPj9K4otxX22bM44h.jpeg) 

![image|578x500](upload://fjfOZvLZq6DoPv270aZUckZeLKU.jpeg) 

![image|632x500](upload://jCLGfviUpQUk2Oqwwk1xXoONhmX.png)
```

---
## \#817 Posted by: SeanHacker Posted at: 2018-12-10T04:41:34.822Z Reads: 154

```
I want that dude...

It's beautiful!!!
```

---
## \#818 Posted by: janpom Posted at: 2018-12-10T07:03:18.018Z Reads: 153

```
[quote="mmaner, post:812, topic:71509"]
I finally got off my ass and got mine finished and installed.
[/quote]

Great! Have you been able to figure out why it didn't work before?
```

---
## \#819 Posted by: lrdesigns Posted at: 2018-12-10T08:45:41.975Z Reads: 152

```
@janpom I got a question about the buttons, is it possible to have the 3rd or additional button in software (optional) so we only need two physical buttons? Like maybe a long press of both buttons gives you the 3rd button press?   

My reason to want such a feature is to save space, as the waterproof buttons take up a lot of volume and makes the case tricky to design. Also these little waterproof buttons are like $1 - $1.50 each. Which for a momentary switch is pretty expensive.

The only thing I like about 3 buttons is it looks better than two. With two you can end up with a funny looking face by accident.
```

---
## \#820 Posted by: tm0587 Posted at: 2018-12-10T08:59:39.054Z Reads: 151

```
I'm lazy, so I'll be more than happy to pay $40 for 2 assembled units, with the additional $5 going to @Mich21050 for assembling the second unit (i hope that's a fair labor cost).
```

---
## \#821 Posted by: mmaner Posted at: 2018-12-10T12:53:30.009Z Reads: 152

```
[quote="janpom, post:818, topic:71509"]
Great! Have you been able to figure out why it didn’t work before?
[/quote]

It think it was something to do with the display not being permanently connected. I'm really not sure. The display is soldered to the PCB now, it works flawlessly.
```

---
## \#822 Posted by: Gerrycorrado Posted at: 2018-12-10T12:59:21.442Z Reads: 152

```
Same here!
You can already put me down for a set (as long as there is at least 1 ready out of the box :slight_smile: )
```

---
## \#823 Posted by: clistpdx Posted at: 2018-12-10T16:50:32.468Z Reads: 155

```
[quote="lrdesigns, post:816, topic:71509"]
Using the smallest waterproof switch I could find, it has a 8mm hole and 12mm head.
[/quote]

I found [this button with a faster shipping](https://www.aliexpress.com/item/8mm-Mini-1NO-2-Pins-Metal-Momentary-Push-Button-Electric-Switch-3A-250V-For-Car/32884574725.html?spm=a2g0s.9042311.0.0.40d04c4dASNsEH) option inside the US. Bought 6 for $10 shipped.
```

---
## \#824 Posted by: JonathanLau1983 Posted at: 2018-12-10T17:04:36.204Z Reads: 162

```
![image|690x437](upload://6ppTgPZh4UMCsJklqMWWLKjGzaX.png)
```

---
## \#825 Posted by: Andy87 Posted at: 2018-12-10T17:27:13.058Z Reads: 163

```
So, Dave is in da house 
![image|375x500](upload://sJbDjyOKwx7znpaHnzVAzppx2yj.jpeg) 

Sure it will need some sanding and finishing, but that’s for now the new home of my speedometer.
Together with the two focboxes close by and will be top mounted on the battery pack between my legs.
```

---
## \#826 Posted by: mmaner Posted at: 2018-12-10T19:51:38.478Z Reads: 161

```
Here's v3 of my DaVeGa riser. 

https://www.thingiverse.com/thing:3274207

It has 2 button slots for use with [these buttons](http://a.co/d/8bvRQCk), a standard 6x6x4.5 momentary switch.   It has 2 button holes with button covers, use super glue to secure the button cover to the buttons.
```

---
## \#827 Posted by: janpom Posted at: 2018-12-10T20:07:44.464Z Reads: 156

```
[quote="lrdesigns, post:811, topic:71509"]
I am REALLY excited to have min/max information on the second or third screen. Any chance we can get that before xmas?
[/quote]

I already started on it. I should be able to finish it in one or two hours. I'm just having hard time to find that time since either there's other things or I'm too tired to code in the evening. I think I'll make it before Xmas though.
```

---
## \#828 Posted by: janpom Posted at: 2018-12-10T20:12:24.293Z Reads: 158

```
[quote="lrdesigns, post:819, topic:71509"]
I got a question about the buttons, is it possible to have the 3rd or additional button in software (optional) so we only need two physical buttons?
[/quote]

I don't see a good and easy way to do that. One problem is that I don't have the buttons connected to the interrupt enabled pins on the MCU (that was a mistake), so I have to detect the button-press in a clunky way.

One easy thing I could do, though, is that the button 1 would reset the session data AND the coulomb counter (if enabled by a preference). That would make the button 2, which only resets the coulomb counter almost redundant. You wouldn't be able to reset coulomb counter without resetting the session data as well (trip distance, min/max values), but I guess that's not a big deal.
```

---
## \#829 Posted by: lrdesigns Posted at: 2018-12-10T23:50:08.480Z Reads: 154

```
[quote="janpom, post:828, topic:71509"]
One easy thing I could do, though, is that the button 1 would reset the session data AND the coulomb counter
[/quote]

That sounds pretty good to me. :+1: 

.
.
.
Just thinking here :thinking: an option of auto reset on full charge would be nice for some people.
```

---
## \#830 Posted by: Battosaii Posted at: 2018-12-10T23:54:25.596Z Reads: 147

```
Hmm yeah but braking while in the 90%+ range may cause the battery to momentarily hit 100% and reset the data. Maybe if there was a time delay for the reset.
```

---
## \#831 Posted by: venom121212 Posted at: 2018-12-11T00:25:09.135Z Reads: 149

```
Or if your pack is older and displays 0.something under your max voltage set. I suppose it would take the reading from the charger still at max voltage.
```

---
## \#832 Posted by: clistpdx Posted at: 2018-12-11T00:34:18.711Z Reads: 145

```
Sorry, what I meant to say was not that they were shipping from the US, but rather they offer a 12-20 days shipping option to the US. The effect is that they arrive 10-30 days sooner than others with different shipping options.
```

---
## \#833 Posted by: clistpdx Posted at: 2018-12-11T00:39:06.192Z Reads: 153

```
[quote="mmaner, post:826, topic:71509"]
Here’s v3 of my DaVeGa riser.
[/quote]

The thingiverse page still shows 'v2' in your newer design's title/headline
```

---
## \#834 Posted by: lrdesigns Posted at: 2018-12-11T01:16:11.414Z Reads: 155

```
I did find illuminated ones for those who need more bling. But I did not like the way they look like [robot nipples.](https://www.aliexpress.com/item/8MM-high-head-with-LED-3V-1-8V-Metal-Button-Switch-Momentary-push-button-auto-reset/32948881040.html?spm=a2g0s.13010208.99999999.277.52943c0012a4bP) 

and are $1.80 each. 
![image|198x184](upload://dqd4Oi3jbmlC2SiLxbjRyez67BC.jpeg)
```

---
## \#835 Posted by: swimmydude Posted at: 2018-12-11T01:18:22.312Z Reads: 153

```
HAHAHA! Get @brenternet in here cause he's going to need some replacement nips. Might as well upgrade and get some bling bling.
```

---
## \#836 Posted by: SeanHacker Posted at: 2018-12-11T01:23:02.413Z Reads: 158

```
Wish I would've known you needed some of these. I can get a ton of different buttons kinda like this at work for free or basically free. Some have screw in terminals, LEDs, ect. 

![IMG_20181210_171914|375x500](upload://9gXJwRs5xsZhDqyr3F60VC2hrw3.jpeg) ![IMG_20181210_171952|375x500](upload://ezao4sZWJvYuqZgriYPXcrKsPgE.jpeg)
```

---
## \#837 Posted by: mmaner Posted at: 2018-12-11T03:08:22.963Z Reads: 151

```
I renamed it, I should really learn to proof my own typing 😀
```

---
## \#838 Posted by: b264 Posted at: 2018-12-11T03:47:34.472Z Reads: 149

```
I actually like the DaVeGa name a LOT better.  @janpom you should adopt it LoL
```

---
## \#839 Posted by: janpom Posted at: 2018-12-11T06:54:26.556Z Reads: 152

```
[quote="lrdesigns, post:829, topic:71509"]
Just thinking here :thinking: an option of auto reset on full charge would be nice for some people.
[/quote]

 Glad that you think so because it's already implemented. You guys should really read through all the config options. :smiley:
```

---
## \#840 Posted by: janpom Posted at: 2018-12-11T07:03:48.176Z Reads: 154

```
[quote="Battosaii, post:830, topic:71509, full:true"]
Hmm yeah but braking while in the 90%+ range may cause the battery to momentarily hit 100% and reset the data. Maybe if there was a time delay for the reset.
[/quote]

That's a very good point. I never thought of that. It would only reset the coulomb counter, not all the session data. It would still be wrong though. I wonder what are the odds of that happening and if it's worth worrying about.

There's a configurable minimal voltage raise to assume the battery has been charged. You could always set it to high enough value to prevent this brake-reset problem. The autoreset may then not happen if you started charging from half full, but then you just reset manually.
```

---
## \#841 Posted by: janpom Posted at: 2018-12-11T07:05:06.422Z Reads: 146

```
[quote="janpom, post:839, topic:71509"]
Glad that you think so because it’s already implemented.
[/quote]

Or did you mean complete session reset? Not just the coulomb counter?
```

---
## \#842 Posted by: lrdesigns Posted at: 2018-12-11T07:16:46.465Z Reads: 144

```
Yeah I mean all session data except for total distance. Same as the button 1-2 combination.
[quote="janpom, post:828, topic:71509"]
session data AND the coulomb counter
[/quote]
```

---
## \#843 Posted by: janpom Posted at: 2018-12-11T09:23:43.194Z Reads: 147

```
I see. Currently only coulomb counter is automatically reset on full charge, but I could add an option for resetting all session data on full charge. Total distance is not (won't be) included in the session data and it will only be possible to reset it by updating FW (same as now).
```

---
## \#844 Posted by: SourPlumGoose Posted at: 2018-12-11T16:34:31.915Z Reads: 146

```
PM'd regarding these buttons :grimacing:
```

---
## \#845 Posted by: clistpdx Posted at: 2018-12-11T17:54:11.032Z Reads: 151

```
[quote="SeanHacker, post:836, topic:71509"]
I can get a ton of different buttons kinda like this at work for free or basically free.
[/quote]

Sweet. I'll remember that next time :)
```

---
## \#846 Posted by: lrdesigns Posted at: 2018-12-12T07:49:45.977Z Reads: 156

```
@janpom after all that I figured out a way to fit 3 buttons on mine. But the two button option is still a good idea I think for more minimal builds. But I like the way three looks much better than two. 

![image|690x370](upload://di9TgkWLhdYDiZcNFJ9qqMFbnAh.jpeg) 

![image|690x458](upload://f6MBSMRJ4hQSQHLzFvTIds3mSmu.jpeg) 

![image|690x460](upload://opFU5sDqEG6njAQ5JwtK7H1icIS.png) 

![image|690x440](upload://wxCMhZklWySOSLRyjaPtmvDbJMs.png) 

![image|689x339](upload://6nCS4KDvbkEIOYfxAyxn66vvYnM.png) 

After I confirm it all fits then I will upload new version to thingiverse.
```

---
## \#847 Posted by: janpom Posted at: 2018-12-12T07:57:06.496Z Reads: 147

```
Looks cool! If I may have one suggestion, I would put the DAVEga inscription on the spacer rather than on the enclosure so that it's correctly oriented.
```

---
## \#848 Posted by: b264 Posted at: 2018-12-12T08:02:57.472Z Reads: 147

```
So is this pronounced dă'-vē"-găh or is it pronounced dāv-gē"-ā'

In other words, da-ve-ga or dave-G A
```

---
## \#849 Posted by: Andy87 Posted at: 2018-12-12T08:17:02.972Z Reads: 146

```
I vote for Dave full stop GA and ga like you would say it in German ... sounds way better 😌
```

---
## \#850 Posted by: janpom Posted at: 2018-12-12T08:18:03.136Z Reads: 145

```
That's still an open problem. A bit like P=NP? ... only harder. :smile:
```

---
## \#851 Posted by: lrdesigns Posted at: 2018-12-12T08:30:09.361Z Reads: 145

```
I have been saying dave Ga but it think that sounds a bit special. 

da-ve-ga sounds more classy.
```

---
## \#852 Posted by: b264 Posted at: 2018-12-12T08:33:56.309Z Reads: 149

```
If it's still an open problem, then a quick poll should gather some information:

[poll type=regular public=true]
* dă’-vē"-găh (Davega.)
* dāv-gē"-ā’ (Dave.G.A.)
* dāv"-găh' (Dave.Ga.)
[/poll]
```

---
## \#853 Posted by: banjaxxed Posted at: 2018-12-12T08:59:26.842Z Reads: 143

```
You wouldn't happen to be a button pusher now would you 😁
```

---
## \#854 Posted by: janpom Posted at: 2018-12-12T09:12:31.779Z Reads: 147

```
That's very scientific. I wonder if the same would work for P?=NP. :smile:
```

---
## \#855 Posted by: SeanHacker Posted at: 2018-12-12T13:24:57.902Z Reads: 147

```
Haha. Nope. Got too much on my hands at the moment to be slanging buttons. ;)

@clistpdx is local so I would've just skated them over.
```

---
## \#856 Posted by: b264 Posted at: 2018-12-13T19:40:54.355Z Reads: 149

```
85% of the votes for `dă’-vē"-găh (Davega.)` but OP @janpom voted for `dāv"-găh' (Dave.Ga.)`

I'm going to call it "Davega" (dă’-vē"-găh)  LoLz

I like how @mmaner stylized it DaVeGa
```

---
## \#857 Posted by: mmaner Posted at: 2018-12-13T19:46:08.499Z Reads: 147

```
I dont give a shit :slight_smile:.
```

---
## \#858 Posted by: lrdesigns Posted at: 2018-12-14T08:31:13.604Z Reads: 160

```
![image|467x500](upload://rduPyesfCQNY6KG3BQyqryeG0v0.jpeg)
 
[JST 1.5mm 5 pin aliexpress.](https://www.aliexpress.com/item/10Pcs-ZH-1-5mm-2-3-4-5-6-7-8-9-10-Pin-Single-JST/32880466568.html?spm=a2g0s.9042311.0.0.49994c4dU9yncj) I was looking for a small connector with 5 pins. Pretty small compared to a 6s connector (7pin). 

![image|666x500](upload://rdfhWJbFI2YmQxnjqMgrCPTo2Zd.jpeg) 

![image|375x500](upload://7o9NHPkAyyE140yjO1Vd1qCwNIf.jpeg) 

![image|375x500](upload://pIN9qqh0KTAtRBBd2OuefrQvave.jpeg) 

![image|375x500](upload://tm8AuvIZHmi3VC22JQZ2DEww1DZ.jpeg) 

![image|375x500](upload://tIyHv58N01lf9QhX1AiD61dhksw.jpeg)  

![image|666x500](upload://deRarKVOUGbqGy88f3Q3lSwrFtI.jpeg) 

![image|375x500](upload://9hnJwJMxGDRDne0cOqWglB4KfnD.jpeg)

Still waiting on buttons. I think it looks nice though.
```

---
## \#859 Posted by: JonathanLau1983 Posted at: 2018-12-14T11:46:57.536Z Reads: 145

```
Awesome enclosure!
```

---
## \#860 Posted by: Itsmedant Posted at: 2018-12-14T15:53:33.746Z Reads: 144

```
What gauge wire are you guys using to extend this back to the VESC?

I got my kit in the other day so I want to get any other supplies I need.

As far as the caps, I'm not sure I can soldering these SMD caps that came with it, I may just get some of the button style caps and try those out too.
```

---
## \#861 Posted by: Skunk Posted at: 2018-12-14T15:56:56.899Z Reads: 145

```
I really like the way your mount turned out.
```

---
## \#862 Posted by: janpom Posted at: 2018-12-14T15:57:03.058Z Reads: 144

```
[quote="Itsmedant, post:860, topic:71509"]
As far as the caps, I’m not sure I can soldering these SMD caps that came with it, I may just get some of the button style caps and try those out too.
[/quote]

Come on, you can do it. I managed to do it and I only started to learn how to solder like 6 months ago. :smile:
```

---
## \#863 Posted by: Itsmedant Posted at: 2018-12-14T16:02:03.091Z Reads: 137

```
I'll try it! Any suggestions? Just hold it down and hope the solder flows!?

I ordered the caps I needed, I'll try the smd's first, only cause you have so much blind faith in me!
```

---
## \#864 Posted by: janpom Posted at: 2018-12-14T16:08:30.075Z Reads: 146

```
Here's what worked for me:
- Put some solder on one pad. Just enough so that it doesn't block the cap from being inserted between the pads.
- Place the cap between the pads and hold it in place with tweezers.
- Reflow the solder. It should stick to the cap. One side done.
- Do the other side. The cap should no longer move, so it's easy.
```

---
## \#865 Posted by: Itsmedant Posted at: 2018-12-14T16:16:40.212Z Reads: 144

```
Sounds simple enough!

What about wire guage? Whats the best type of wire to use to extend from the front of my board to the back?
```

---
## \#866 Posted by: janpom Posted at: 2018-12-14T16:18:52.215Z Reads: 146

```
I made it work with really shitty cable, so I'd say it doesn't matter. You definitely don't need thicker than 24 AWG and much thinner will likely be OK.
```

---
## \#867 Posted by: Itsmedant Posted at: 2018-12-14T16:20:19.624Z Reads: 145

```
Cool, thats what I thought it was, just wanted to make sure. Its not carrying a huge load of power through it so it should be fine!

I'm hoping to have this ready to go at the same time I finish my battery so I can get everything plugged in and programmed all at once!
```

---
## \#868 Posted by: janpom Posted at: 2018-12-14T16:21:02.369Z Reads: 147

```
It draws less than 100 mA from the ESC.
```

---
## \#869 Posted by: lrdesigns Posted at: 2018-12-17T04:01:09.394Z Reads: 157

```
Buttons came in, woo Monday just got a bit better. 

![IMG_1772|666x500](upload://ekwbxTbejDmAU54TscEfW9GhXqn.jpeg) 

![IMG_1773|666x500](upload://wx2AFv0L1wi2FtjBMHO1r3MXiun.jpeg) 

![Photo%20Dec%2017%2C%201%2054%2031%20PM|375x500](upload://8c0TAAkW6BeFExBnn86WBRI4Aev.jpeg) 

![Photo%20Dec%2017%2C%202%2007%2037%20PM|375x500](upload://997P5RECEkj2zOKi34xG65iqqSk.jpeg) 

Encase in hotglue for vibration control and water proofness. 

![Photo%20Dec%2017%2C%201%2056%2001%20PM|666x500](upload://cbmw3NFxAiCBTNWsQnfXiurgaAa.jpeg) 

Always check it works before bolting it back together. All good! :+1: 

@janpom your probably getting sick of my feature requests. But I got one more. In the horizontal screen I really would like to swap out battery % with average cell voltage. Only one decimal place so it still fits in the same area. Average cell voltage is the only critical number for me while monitoring voltage sag.  The % number can be misleading and its easy to make it wacky by changing the config. But cell voltage should always be "accurate".
```

---
## \#870 Posted by: banjaxxed Posted at: 2018-12-17T09:31:10.542Z Reads: 146

```
And don’t forget to flux on, flux off!

I.e. let it do the work of flowing the solder and avoiding bridges then get get rid of it with IPA, as its corrosive
```

---
## \#871 Posted by: Jumpman Posted at: 2018-12-17T10:35:16.334Z Reads: 142

```
I used the same method as @janpom.  If you end up with solder under the cap, or your tweezers are too slippery, then what I found helped was to hold the cap down with the tip of my thumb nail.
```

---
## \#872 Posted by: uigiroux Posted at: 2018-12-17T10:50:13.164Z Reads: 147

```
Is it still possible too order one of these, or is that over?  Also, is it possible to order this fully assembled?
```

---
## \#873 Posted by: janpom Posted at: 2018-12-17T11:47:37.864Z Reads: 147

```
@uigiroux See [here](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/801?u=janpom). It will probably happen late January or early February.
```

---
## \#874 Posted by: Itsmedant Posted at: 2018-12-17T18:04:34.015Z Reads: 145

```
My davega is going to be a bit delayed everyone, I'm finally getting the last of my parts for my build so I gotta focus on getting this board built before the snow starts falling here!

Then I'll get the Davega built!
```

---
## \#875 Posted by: uigiroux Posted at: 2018-12-19T04:14:37.097Z Reads: 140

```
Please put me down for a set of 2.  Love the idea of having one assembled as a guide!  So cool :heart_eyes:
```

---
## \#876 Posted by: janpom Posted at: 2018-12-19T08:11:17.266Z Reads: 152

```
I'm trying to decide whether the assembled kit should come with the headers for the displayed soldered on the PCB. I think it would be a good idea since (1) it would make testing easier and (2) it would be truly plug-and-play; no need to solder anything.

The downside is that the headers make the Dave slightly thicker. If you shorten the display pins, the difference is negligible (about 1 mm thicker than without headers), so IMO it's not a big deal.

Since nobody is integrating Dave directly into the deck, I don't see a problem with having an extra 1 mm of thickness. It may require modifying the existing enclosures though. I believe the @mmaner's one should work fine without modifications. I had one printed and I'm using it without the headers, but there's still some extra space. I'm not sure about the @lrdesigns' one. Do we have some headroom there?
```

---
## \#877 Posted by: lrdesigns Posted at: 2018-12-19T08:15:30.768Z Reads: 138

```
1mm might squeeze in, or I could modify the base a little. A header for the LCD will sure make it easier to test etc. Will it be ok with heavy vibration from skating?
```

---
## \#878 Posted by: janpom Posted at: 2018-12-19T08:19:09.500Z Reads: 143

```
[quote="lrdesigns, post:877, topic:71509"]
1mm might squeeze in, or I could modify the base a little.
[/quote]

That would be great. Thanks!

[quote="lrdesigns, post:877, topic:71509"]
Will it be ok with heavy vibration from skating?
[/quote]

In the enclosure it will still be held in place with bolts so that should be fine.
```

---
## \#879 Posted by: lrdesigns Posted at: 2018-12-19T08:24:50.124Z Reads: 141

```
[quote="janpom, post:878, topic:71509"]
In the enclosure it will still be held in place with bolts so that should be fine.
[/quote]

I guess you could add a bit of hotglue to the header when you do the final installation for extra vibration proofing.
```

---
## \#880 Posted by: mmaner Posted at: 2018-12-19T12:53:53.242Z Reads: 148

```
I've redesignd mine a bit. I changed the button locations and made a new base. I printed it last night, haven't installed it yet. I'll get some pics soon. 

But, it ises 5mm standoffs so I can add in some shorter standoffs for people using the soldered header. There's about 10mm to play with in the new base
```

---
## \#881 Posted by: mmaner Posted at: 2018-12-19T14:14:26.357Z Reads: 159

```
New Base, the housing sits inside and uses spacers to set the height required.

![image|649x500](upload://g7UXiUQh1ekfCQPIurcxtuf8XJM.jpeg) 

It looks like this when its put together.

![image|648x500](upload://wRgGo0KiTnYkcZswxm0eZ4iOWu1.jpeg) 

The idea is the base screws to the deck, the housing screws to the base.  You have room for anti-vibration mat and cabling plus the cutout in the base leaves room for braces and truck hardware.

I also re-arranged the buttons to make them easier to use.  The last thing I have to do is make a version of the housing with snap-in slots for mini tactile buttons.  Once those are in place you can pop the buttons in place, put a drop of hot glue on them and they should stay in place forever.  The buttons tops are pretty simple, they print with the housing, you just pop them out of the support material and a drop of superglue on the bottom and you are good to go.

Here is an actual print but its not completely installed yet.

![IMG_20181219_071158_1545228842124|633x500](upload://390Zbu4f23LhNmeijAWT4sPCdKN.jpeg)
```

---
## \#882 Posted by: venom121212 Posted at: 2018-12-19T14:49:29.192Z Reads: 154

```
Any chance my kit is still coming? I fear it is lost in the holiday mail.
```

---
## \#883 Posted by: janpom Posted at: 2018-12-19T15:03:51.770Z Reads: 151

```
None was lost so far. It's likely only delayed. It's a bad time for shipping anything. I have no more spares, so please wait and if it doesn't arrive before the new year, I  will refund your payment.
```

---
## \#884 Posted by: ROFEN13 Posted at: 2018-12-19T15:30:14.304Z Reads: 148

```
Mine took a month to as arrive. @janpom i will send the spare if his doesnt arrive instead of you refunding.
```

---
## \#885 Posted by: venom121212 Posted at: 2018-12-19T15:31:22.763Z Reads: 143

```
Thank you both. No rush just checking. Happy to be receiving this awesome component regardless.
```

---
## \#886 Posted by: Battosaii Posted at: 2018-12-19T15:33:17.137Z Reads: 141

```
I'm in the same boat I check the mail eagerly everyday.
```

---
## \#887 Posted by: yelnats8j Posted at: 2018-12-19T15:38:26.586Z Reads: 146

```
Same i cant wait to get it.
```

---
## \#888 Posted by: mmaner Posted at: 2018-12-19T17:34:01.779Z Reads: 163

```
I made some tweaks so everything fits together nicely.  I am doing the final print tonight, if everything goes correctly I will post the models tomorrow.  

I did some renders, I mostly never do that :slight_smile:.

![DaVeGa%20Riser%20v3%20render%2001|500x500](upload://bbaKLbJsMJlo0bSMVqm15ziCYuk.jpeg) ![DaVeGa%20Riser%20v3%20render%2002|500x500](upload://jdpvjlCb8du6BqGNcqgn2dWZSUk.jpeg) ![DaVeGa%20Riser%20v3%20render%2003|500x500](upload://oGWGrqA5OPgNp7WruOZhvwKrvM4.jpeg) ![DaVeGa%20Riser%20v3%20render%2004|500x500](upload://skZdwJBd1nNdnUZxNimRqg1eMXn.jpeg)
```

---
## \#889 Posted by: swimmydude Posted at: 2018-12-19T17:39:16.597Z Reads: 149

```
I'll he assembling mine sometime this week maybe, but definitely before the weekend is over. I'm still in limbo with my build waiting on my second mount and Unity. What I'm currently working on is my remote and it seems to be functioning thus far but I'm having slight issues figuring out the coding on its receiver. But my question is since my remote and DaveGa are basically doing the same thing, are they going to be fighting for slots to plug into on my Unity? I know there's not much point on having both, but things were already in motion. I already ordered parts and was working on my Firefly remote then saw that I could assist on the beta testing on this.

If slots are limited, I don't know if splicing them together to fit one slot would work either? Even if I soldered some diodes on there?
```

---
## \#890 Posted by: Itsmedant Posted at: 2018-12-20T00:38:16.636Z Reads: 146

```
My screen finally came in! Just waiting on a few more things and I'll get it going!
```

---
## \#891 Posted by: mmaner Posted at: 2018-12-20T00:55:49.288Z Reads: 147

```
I'm getting crazy speeds shown. I think I've figured it out though. 

I'm using carvon torque drives, they have 14 pole pairs and I have the DaVeGa configured for 7. I assume if I change it to 24 that will resolve my issue?
```

---
## \#892 Posted by: JonathanLau1983 Posted at: 2018-12-20T01:05:50.885Z Reads: 142

```
I wasn't sure about this too, but thought 7 pole pairs meant 14 poles total which matches my motors. 
Hopefully @janpom can answer this
```

---
## \#893 Posted by: brenternet Posted at: 2018-12-20T01:14:08.618Z Reads: 134

```
Gents, I'd like to mount my dave-ga (Yes) under my deck in the enclosure under something clear.

I like the idea of using it as a battery meter/odometer but don't need to look at it while I'm riding. Am I the only one?

If I did that is there going to be a single button function scroll?
```

---
## \#894 Posted by: sayekim Posted at: 2018-12-20T07:16:10.537Z Reads: 133

```
28 would be the magic number. Not 24. I have it set to 28 on metr too.
```

---
## \#895 Posted by: janpom Posted at: 2018-12-20T07:36:58.796Z Reads: 133

```
Probably 14, not 28. It's 14 pole pairs or 28 poles. In DAVEga, you enter the number of pairs. I suppose the 24 in @mmaner's post is just a typo and he actually meant to write 14.
```

---
## \#896 Posted by: bigben Posted at: 2018-12-20T07:38:44.607Z Reads: 137

```
You are the only one.
```

---
## \#897 Posted by: JonathanLau1983 Posted at: 2018-12-20T09:55:33.279Z Reads: 148

```
Top tip, hit the 3D printed enclosures with truck bed liner spray.
![image|666x500](upload://4EXBrEswzTpfytqdXttlVWpcEK1.jpeg)
```

---
## \#898 Posted by: janpom Posted at: 2018-12-20T11:14:02.339Z Reads: 148

```
Maybe then you don't need any button at all?

I now have some small ATMEGA328P-AU chips and 128x32 OLED displays that I would like to use for creating a mini version of DAVEga exactly for your type of use case. The problem is there's more projects than spare time, so I don't know when this will be available.
```

---
## \#899 Posted by: brenternet Posted at: 2018-12-20T11:19:27.306Z Reads: 148

```
I've got time 😁 no rush here.

Just try do it while the weather is bad because when spring hits you're going to be on that falcon all day!
```

---
## \#900 Posted by: janpom Posted at: 2018-12-20T12:10:40.746Z Reads: 158

```
100 uF smoothing caps just arrived from mouser. The size looks good. Now I have 100 kits to make. Great. :sweat_smile:

![image|448x500](upload://dMkQG3PvUzQ0416N9lbBscqqLWP.jpeg)
```

---
## \#901 Posted by: mmaner Posted at: 2018-12-20T14:37:59.248Z Reads: 158

```
Per Carvon the Carvon v4 TD's have 14 pole pairs, 28 poles/magnets.  I changed the pole pairs setting in the DaVeGa config to 14 and the issue is resolved.
```

---
## \#902 Posted by: janpom Posted at: 2018-12-20T20:07:46.521Z Reads: 164

```
A few pics of Dave on my eMTB in @mmaner's enclosure (the older version, which is still pretty cool though).

![DSC01693|690x295](upload://fu98qQj5IoZMJayxwy89sgH4j4z.jpeg)

![DSC01716|690x399](upload://3zRAeXujmJV9aKTTOqm68VhoSJM.jpeg) 

![DSC01711|690x460](upload://b5bwg2s8JPcZmUcxRyhaM8LEhe2.jpeg)
```

---
## \#903 Posted by: mmaner Posted at: 2018-12-20T20:33:10.865Z Reads: 150

```
Looks awesome.  You'll like the latest revision of the housing, there are slots for the momentary buttons, makes it a lot easier to mount.  Plus I've included blanks if you want to only use 2 buttons like I am.
```

---
## \#904 Posted by: janpom Posted at: 2018-12-21T21:21:58.299Z Reads: 155

```
Guys, I'm going to make changes to the PCB and order some for the batch 2. Planned changes:
- remove the DEBUG pins
- add the 100uF axial capacitor (in place of the DEBUG pins)
- adjust the distance between holes for 22pF capacitors
- route the buttons to interrupt-enabled MCU pins

Apart from that I'm considering the following (not yet decided):
- flip the 4pin JST-PH connector so that it faces inwards the PCB
  - this is so that the cable can be routed from between the PCB and the display to either side
- use pads instead of holes for buttons
  - we then need to decide on which side of the PCB they will go though
  - or we could put them on both sides and connect them with an auxiliary hole

Any thoughts about the latter? Is there anything else you'd like changed?

Please note that most of you have the v0.2, but v0.3 already exists that has the [following changes](https://github.com/janpom/davega/blob/master/CHANGELOG_PCB). Those will be retained for v0.4.
```

---
## \#905 Posted by: mmaner Posted at: 2018-12-21T21:23:47.131Z Reads: 144

```
I don't know if anyone will care, but would it be possible to add a positive and negative passthrough to drive an LED for button 1?
```

---
## \#906 Posted by: janpom Posted at: 2018-12-21T21:31:34.040Z Reads: 143

```
What would that be good for? Do you want to have a LED that lights up when you press the button?
```

---
## \#907 Posted by: mmaner Posted at: 2018-12-21T21:40:13.811Z Reads: 144

```
Just have an LED to show power.  Normally the power switch is used to show power, which is typically on the side of the enclosure.  This way it'll be on the top of the board.

Like I said, not a big deal, just a thought.
```

---
## \#908 Posted by: janpom Posted at: 2018-12-21T21:43:31.942Z Reads: 144

```
Hm, you would have the Dave display to power on when you power on the board. Isn't that sufficient indication? I'm not saying no. I'm just trying to understand the use case.
```

---
## \#909 Posted by: mmaner Posted at: 2018-12-21T21:44:52.924Z Reads: 147

```
I agree, its just an attractiveness thing.  Its not at all important and doesnt really serve any purpose other than looking pretty :).
```

---
## \#910 Posted by: janpom Posted at: 2018-12-21T21:47:49.050Z Reads: 142

```
Alright. I don't quite understand how it relates to buttons, though. You could just connect the LED to any 5V and GND on the PCB. Plus, you would need a current limiting resistor in series with the LED. I could make space for the resistor directly on the PCB to make this easier. There's definitely space for it. I can even add two dedicated pads for the LED.
```

---
## \#911 Posted by: janpom Posted at: 2018-12-21T21:54:12.863Z Reads: 140

```
Oh, you mean a backlight for the button, right? Sometimes I'm slow in understanding things. :smile:
```

---
## \#912 Posted by: mmaner Posted at: 2018-12-21T22:00:45.140Z Reads: 147

```
Yes, just to light a 10mm momentary switch that has a built in LED.
```

---
## \#913 Posted by: mmaner Posted at: 2018-12-21T22:02:24.203Z Reads: 153

```
Something like this...

https://www.amazon.com/button-switchtoggle-Waterproof-Momentary-Modified/dp/B074WXYSPH/ref=sr_1_3?ie=UTF8&qid=1545429660&sr=8-3&keywords=10mm+momentary+switch
```

---
## \#914 Posted by: janpom Posted at: 2018-12-22T21:52:12.342Z Reads: 157

```
@lrdesigns How about this?

![IMG_1583|674x500](upload://8gVFPFNPItBvZGHclIsU3gRqMPC.jpeg) 

Would everyone be OK with this for the horizontal layout? Or is there anyone who prefers the previous one with only two numbers on the right hand side and slightly bigger fonts?

If anyone prefers battery % instead of volts, I can make that a config option.
```

---
## \#915 Posted by: JonathanLau1983 Posted at: 2018-12-22T21:54:16.907Z Reads: 151

```
Looks awesome @janpom. 
I don't think battery % I necessary considering the coloured bars beneath. Average voltage makes good sense.
```

---
## \#916 Posted by: bigben Posted at: 2018-12-22T22:59:15.279Z Reads: 149

```
Top speed on the trip would be a handy one to squeeze in?
```

---
## \#917 Posted by: bigben Posted at: 2018-12-23T10:56:33.110Z Reads: 157

```
![image|666x500](upload://5PggIVmpTOxpEWfx2wDXJlJQglg.jpeg) ![image|375x500](upload://iNco4GW7akzcOhl5MQAHy0lCCL3.jpeg) 
Does it look like I’m getting closer on this attempt?
@janpom
```

---
## \#918 Posted by: bigben Posted at: 2018-12-23T12:56:58.105Z Reads: 159

```
![image|375x500](upload://VIYNAzdJyQn2xR4AiaBmdNOgv4.jpeg)
```

---
## \#919 Posted by: bigben Posted at: 2018-12-23T17:39:50.619Z Reads: 153

```
It's up and running. Displaying voltage but no speed? I know I'm missing something obvious.. As always.
```

---
## \#920 Posted by: mmaner Posted at: 2018-12-23T17:45:56.748Z Reads: 155

```
You just need to go faster 😀
```

---
## \#921 Posted by: JonathanLau1983 Posted at: 2018-12-23T17:55:20.357Z Reads: 153

```
Stupid question, but you running sensored motors?
```

---
## \#922 Posted by: bigben Posted at: 2018-12-23T18:03:24.419Z Reads: 153

```
No.. Stupid persons answer?
```

---
## \#923 Posted by: JonathanLau1983 Posted at: 2018-12-23T19:49:28.114Z Reads: 147

```
Well I assumed the VESC used the hall sensors to determine rotation speeds, so I think this only works with sensored setups.
```

---
## \#924 Posted by: bigben Posted at: 2018-12-23T20:00:40.966Z Reads: 143

```
Doh. I'll have to stick it on another build..
```

---
## \#925 Posted by: deucesdown Posted at: 2018-12-23T20:07:06.282Z Reads: 135

```
Speed is calculated from erpm which is how vesc controls the motor. No sensor required for speed readings.
```

---
## \#926 Posted by: bigben Posted at: 2018-12-23T20:10:03.664Z Reads: 141

```
Phew so must be missing something in the settings in either the arduino or vesc tool.
```

---
## \#927 Posted by: janpom Posted at: 2018-12-23T20:56:03.786Z Reads: 146

```
It's unlikely it has to do with VESC settings. I assume you're an order of magnitude off somewhere in the Dave settings. As a result the calculated speed is up to 0.5 km/h, which is displayed as 0.

It could be the wheel circumference, gear teeth, number of motor pole pairs.
```

---
## \#928 Posted by: janpom Posted at: 2018-12-23T20:58:32.697Z Reads: 147

```
@bigben What's your values for the following options:
```
MOTOR_POLE_PAIRS
WHEEL_CIRCUMFERENCE_MM
MOTOR_PULLEY_TEETH
WHEEL_PULLEY_TEETH
```
?
```

---
## \#929 Posted by: bigben Posted at: 2018-12-23T20:59:19.129Z Reads: 145

```
I set it as circumference 283 for 90mm, 1-1 for teeth as it's direct drive. Pole pairs 7.(not sure at all on this one as it's carvon. 2.5
```

---
## \#930 Posted by: janpom Posted at: 2018-12-23T21:03:29.205Z Reads: 146

```
That sounds OK. Not sure about carvon 2.5 poles count, but I doubt you're an order of magnitude off. You should be seeing some speed indication as long as you're getting data from the VESC.

You said the voltage is displayed correctly. The small blinking box underneath the speed indicator is green?
```

---
## \#931 Posted by: bigben Posted at: 2018-12-23T21:06:20.404Z Reads: 145

```
Voltage shows correctly but theres a quickly flashing red box.
```

---
## \#932 Posted by: janpom Posted at: 2018-12-23T21:11:12.123Z Reads: 140

```
If it's red, then you're not receiving data from the VESC. The voltage shown is the last seen value (it's persisted). Did you set the `EEPROM_INIT_VALUE_VOLTS` and now it's showing whatever you put there or did you leave it at 0?

If the latter and there's non-zero voltage shown, that means you did have a working VESC connection at some point, but you have lost it now. In that case you'll want to check your wires for a loose connection.
```

---
## \#933 Posted by: bigben Posted at: 2018-12-23T21:33:14.042Z Reads: 136

```
Strangely now I don't seem to be able to get anything. It lights up and shows the screen, just has no readings at all! I've managed to get 2 Dave's to this stage..
```

---
## \#934 Posted by: bigben Posted at: 2018-12-23T21:55:11.704Z Reads: 135

```
Using Ackmaniac software if this would have any bearing on what is happening.. Or more like not happening.
```

---
## \#935 Posted by: janpom Posted at: 2018-12-23T22:03:25.415Z Reads: 143

```
I don't use Ackmaniac's FW, but @lrdesigns [does and runs Dave with no problem](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/759?u=janpom).

The strange thing is that it seems you did have it working for a while. If that's the case, it must be a HW problem. Probably something with the RX/TX wires.
```

---
## \#936 Posted by: bigben Posted at: 2018-12-23T22:15:16.928Z Reads: 147

```
RX and TX aren't reversed like a bluetooth module are they?
```

---
## \#937 Posted by: janpom Posted at: 2018-12-23T22:30:53.464Z Reads: 151

```
No, you should connect the VESC RX to the pad labeled RX on the Dave PCB. Same for TX.
```

---
## \#938 Posted by: janpom Posted at: 2018-12-24T22:13:55.001Z Reads: 158

```
This may still be before Xmas for some of you. ;)

![IMG_1596|635x500](upload://qhR6z13JjWTy0L5y12gCAdiSja9.jpeg) 

New session data items:
- min total voltage
- max speed
- time elapsed
- time riding

Available from the [session_data](https://github.com/janpom/davega/tree/session_data) branch for the inpatient ones (note that I only just finished coding this and it went through minimal testing). Apologies for the lame time output. This will soon get an update to get properly formatted HH:MM:SS. While it may look trivial, it's somewhat tricky to do now without exceeding the available flash memory (already at 97%). I will have to do some optimisations before adding more features.

WARNING: **This update resets the EEPROM**, so be sure to take a note of your total traveled distance before installing and enter it as the `EEPROM_INIT_VALUE_TOTAL_DISTANCE` in the config.

Merry Christmas everyone!
```

---
## \#939 Posted by: deucesdown Posted at: 2018-12-26T15:11:54.977Z Reads: 153

```
@janpom do you think you can keep a list of compatible firmwares somewhere? Maybe in the readme.md in github, since Discourse blocks editing old posts (grr).

For example I'm running mostly 2.54 (ackmaniac, BLDC-Tool), and some 2.18 (vanilla BLDC-Tool). I have a Enertion R2 which has custom firmware version 2.80. According to https://enertionboards.zendesk.com/hc/en-us/articles/360000673895 Enertion also has 23.40.

Personally I've not tried the Vesc-Tool firmwares yet, of which there's an Ackmaniac version.

And now Enertion Unity has a new packet format:

https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/121

We can report what works and what doesn't, but I'd be nice to have a central place track it all.
```

---
## \#940 Posted by: janpom Posted at: 2018-12-26T17:55:00.086Z Reads: 146

```
Sure, I can add a section to the README file. It's a great idea. Personally, I have only tested the VESC FW 3.40 (the latest version). If anyone is successfully running DAVEga with another FW, please let me know and I will add it to the list.

I'm not sure if tracking the hardware known to work is worth the time. I'm guessing that any VESC based controller should work as long as it's running compatible FW and has UART enabled. Right?
```

---
## \#941 Posted by: b264 Posted at: 2018-12-26T18:12:04.874Z Reads: 152

```
Yes&ZeroWidthSpace;
```

---
## \#942 Posted by: janpom Posted at: 2018-12-27T18:38:46.316Z Reads: 164

```
Here's the draft of the new PCB layout. I think it's about time to call it v1.0 so I did. :slight_smile: 

Changes to v0.2:
- removed DEBUG pins
- added 100uF axial capacitor (for a more stable power supply)
- added pads for a LED and a current limiting resistor (as per @mmaner's request; can be left unused)
- brought pads for the 20pF caps closer together (so that the [THT caps](https://www.aliexpress.com/store/product/50PC-Monolithic-Capacitor-101-102-103-104-220-330-50V-100PF-1NF-10NF-0-1UF-22P/630494_32865098104.html?spm=2114.10010108.1000023.124.15bc7bd4eP3Kni) I have on hand fit)
- moved the crystal so that it doesn't rub against the chip on the display above
- moved USB-UART further from the edge so that the headers are flush with the edge
- moved the right side mounting holes a hair to the right

![57|690x418](upload://ns1pZnpt5SXiDtdvGDYqNf5V0G5.png) 

I'm about to have these manufactured. If anyone would like any more changes speak now or forever hold your piece.
```

---
## \#943 Posted by: b264 Posted at: 2018-12-27T18:42:10.769Z Reads: 156

```
I would relabel "VESC" as "ESC" or "ESC UART" to stave off the trademark wrath nastygrams
```

---
## \#944 Posted by: janpom Posted at: 2018-12-27T18:46:21.995Z Reads: 155

```
That would be kinda wrong though since it doesn't work with any ESC, only with VESC derivatives running the (modified) VESC FW. I wish there was a better short term for these.
```

---
## \#945 Posted by: mmaner Posted at: 2018-12-27T19:10:15.107Z Reads: 150

```
I don't have it in front of me or I would measure.  But the screw holes in the display are M2 I think. do you think making the screw holes in PCB match would be advisable?
```

---
## \#946 Posted by: JonathanLau1983 Posted at: 2018-12-27T19:25:03.375Z Reads: 152

```
My LCD had M3 holes, I had to drill out my PCB to match.
```

---
## \#947 Posted by: janpom Posted at: 2018-12-27T19:37:21.830Z Reads: 153

```
The display PCB holes are indeed M3 while the Dave PCB holes are M2. I could extend them to M3, but I'm not sure if I can align them perfectly and if I don't, the M3 screws going through will be slightly angled. Maybe better to keep M2 and use M2 screws? I'm open to suggestions.
```

---
## \#948 Posted by: mmaner Posted at: 2018-12-27T19:40:13.103Z Reads: 151

```
I'm just making a suggestion, it doesn't stop it the assembly at all.  It might be better to leave them as M2.
```

---
## \#949 Posted by: janpom Posted at: 2018-12-28T19:53:53.785Z Reads: 149

```
I'll leave M2. Changing M2 hole to M3 hole is a matter of one minute with a drill. The same is not true for shrinking M3 hole. :smile:
```

---
## \#950 Posted by: janpom Posted at: 2018-12-29T14:27:28.341Z Reads: 159

```
![image|669x500](upload://uVEklEDn5RFxQbxQL3Gxw7XxKiS.jpeg) 

MCUs arrived. I should start mining bitcoins with so much processing power on hand. :smiley:
```

---
## \#951 Posted by: janpom Posted at: 2018-12-29T15:23:00.696Z Reads: 159

```
Display headers arrived.

![image|538x500](upload://3V1ZyOcgSyD2CTG0ux26bY6mgB0.jpeg) 

... but a wrong size. Dammit! :man_facepalming:

![image|690x454](upload://ac1vawY0TScikKNa280IkrV05ro.jpeg) 

Anyone needs 11pin 2.0mm female headers? I have a lot. :smiley:
```

---
## \#952 Posted by: janpom Posted at: 2018-12-29T20:40:58.322Z Reads: 159

```
Today I fixed bugs in the session data code, ensured time is properly formatted and added avg speed. It's now merged to master and released as [v0.4](https://github.com/janpom/davega/releases/tag/v0.4). Enjoy.

![IMG_1600|690x498](upload://r2aTmOSVA3bRBNF4AukIOcqONUo.jpeg)
```

---
## \#953 Posted by: janpom Posted at: 2018-12-29T22:27:18.674Z Reads: 157

```
Gerber files for PCB v1.0 are now available: https://github.com/janpom/davega/tree/master/gerbers

I reverted the button re-routing at last to retain backwards compatibility with the FW. After some experiments with pin change interrupts (that work on all ATMEGA328 pins), I figured these will do for future developments. No need to use the pins with full interrupt capabilities. (If this doesn't make sense to you, don't worry. :smile:)

Here's also the [BOM with the purchase links](https://docs.google.com/spreadsheets/d/1GwQCfm-0AdgQenQ-uo58yl8oYM9hIg8REw0B3hwU51c/edit?usp=sharing) that I use in case anyone wants to order everything on their own.

I'm going to order the PCBs right now. I should be ready to start shipping first kits in about 3 weeks time. I will start a thread for batch 2 shortly before that. As mentioned before, there will be a package with 2 kits, one assembled and one unassembled for $25 including world wide tracked shipping. [DISPLAY](https://www.aliexpress.com/item/ILI9225-2-0-Inch-UART-TFT-LCD-Display-Module-SPI-Interface-Colorful-Screen-Serial-Port-176x220/32792711665.html) **NOT** INCLUDED. If you have special needs (maybe you want more than 2 kits or maybe you only want assembled ones) please talk to @Mich21050. He might be handling custom orders if there's enough interest.
```

---
## \#954 Posted by: totalgeek9224 Posted at: 2018-12-30T09:35:55.480Z Reads: 145

```
Why not just then use VESC™
```

---
## \#955 Posted by: b264 Posted at: 2018-12-30T09:57:49.119Z Reads: 145

```
Hey, y'all can do whatever you want :blush:

That's just my recommendation is all

It's easy to change web apps later if needed and all the digital stuff, but not scrap a whole batch of PCBs because of one letter on the silkscreen
```

---
## \#956 Posted by: Mich21050 Posted at: 2018-12-30T10:00:23.979Z Reads: 152

```
Thats a little bit complicated but it's about copyright open source and so on.. It's not really clear what is legally allowed and what not...
```

---
## \#957 Posted by: b264 Posted at: 2018-12-30T10:18:25.009Z Reads: 153

```
[quote="Mich21050, post:956, topic:71509, full:true"]
Thats a little bit complicated but it’s about copyright open source and so on… It’s not really clear what is legally allowed and what not…
[/quote]

This is exactly why I wouldn't put it on the PCB silkscreen.  But :man_shrugging:

You could have it in the digital documentation all day long
```

---
## \#958 Posted by: totalgeek9224 Posted at: 2018-12-30T10:22:00.334Z Reads: 144

```
I see, then maybe not write VESC but rather ℣esc? ;)
```

---
## \#959 Posted by: Mich21050 Posted at: 2018-12-30T10:23:25.014Z Reads: 145

```
Thats exactly what I meant.. :wink:
I wouldn't put it anywhere.. not even digital... :slight_smile:
```

---
## \#960 Posted by: Skunk Posted at: 2018-12-30T10:23:48.891Z Reads: 143

```
Davesc ? Lol
```

---
## \#961 Posted by: b264 Posted at: 2018-12-30T10:26:42.392Z Reads: 144

```
What I mean is you can change the digital assets at any time but not so much a PCB silkscreen.  It's a like a tattoo.
```

---
## \#962 Posted by: Mich21050 Posted at: 2018-12-30T10:27:58.907Z Reads: 144

```
Yes and I'm not 100% sure but I think you would have to recall all pcbs (that you sold)and change them...  :slight_smile:
@b264
```

---
## \#963 Posted by: janpom Posted at: 2018-12-30T14:01:41.108Z Reads: 150

```
Yeah, we could put V-youknowwhat and AT-youknowwhat-328. Come on guys. I would be really surprised if there was a legal problem with writing VESC on a PCB where it clearly means "plug VESC here". It would be against common sense. And even if there was a legal issue, Vedder would have to be one hell of an asshole to go after it, which I believe he's not.
```

---
## \#964 Posted by: mmaner Posted at: 2018-12-30T14:18:28.648Z Reads: 150

```
I kind of agree with you but Frank from Trampa commonly sicks his lawyers on people for using the term VESC. 

Your right, it would be silly for anyone to care, but he apperantly does and has gone after people in the past.
```

---
## \#965 Posted by: Mich21050 Posted at: 2018-12-30T14:20:03.944Z Reads: 145

```
It wasn't meant to offened you or anything. I just wanted to note it..  :slight_smile:
```

---
## \#966 Posted by: janpom Posted at: 2018-12-30T15:32:56.395Z Reads: 143

```
[quote="mmaner, post:964, topic:71509"]
I kind of agree with you but Frank from Trampa commonly sicks his lawyers on people for using the term VESC.
[/quote]

He doesn't want "VESC" to be used on VESC derivatives = competing products, which is understandable. This is a completely different situation though. Asking me to remove VESC from the Dave PCB would be like asking the admins of this forum to remove all mentions of VESC from all posts.
```

---
## \#967 Posted by: totalgeek9224 Posted at: 2018-12-30T15:36:02.330Z Reads: 142

```
@trampa could you provide some insight here? Do we need to be worried, or do we have your blessing?
```

---
## \#968 Posted by: mmaner Posted at: 2018-12-30T15:37:10.193Z Reads: 138

```
I agree, I mean I totally agree. All I'm trying to do is add a little bit of perspective to whatever you decide. It's not so much Ben as it is Frank that shoots first and asks questions later. I feel like you will be fine, but maybe shoot him a PM to make sure.
```

---
## \#969 Posted by: Itsmedant Posted at: 2018-12-30T16:30:32.233Z Reads: 137

```
Gonna try and populate my DaveGa today....or build my battery....or clean my damn garage all the way. Crap, got too much to do and to little time to do it!
```

---
## \#970 Posted by: yelnats8j Posted at: 2018-12-30T16:33:13.188Z Reads: 136

```
Is anyone else still waiting for it?
```

---
## \#971 Posted by: banjaxxed Posted at: 2018-12-30T16:34:16.690Z Reads: 140

```
Thanks @janpom I ordered some pcbs a week ago, not sure when I’ll make a couple but the BOM is really handy
```

---
## \#972 Posted by: Battosaii Posted at: 2018-12-30T18:35:41.785Z Reads: 146

```
I am still why?
```

---
## \#973 Posted by: trampa Posted at: 2018-12-30T19:20:45.582Z Reads: 154

```
What you need to know can be found here:
https://vesc-project.com/trademark_policies

You can't use the VESC Trademark for/on your product. You can make fair use of the TM as stated in the TM policies. 

Fair use is for example using the TM in your product description to point out compatibility with VESC Software:

_XYZ, compatible with VESC®* Software/Firmware_

_* VESC is a registered TM owned by Benjamin Vedder._
```

---
## \#974 Posted by: venom121212 Posted at: 2018-12-30T19:35:30.533Z Reads: 154

```
Me :cry: my mailbox can't take the wear on the hinges any more
```

---
## \#975 Posted by: clistpdx Posted at: 2018-12-30T22:40:45.914Z Reads: 155

```
[quote="trampa, post:973, topic:71509"]
What you need to know can be found here:
[https://vesc-project.com/trademark_policies ](https://vesc-project.com/trademark_policies)
[/quote]

Looks like it specifically forbids use on a circuit board:
"A trademark should not be used on/for Products (e.g. circuit boards, hardware, services)"
```

---
## \#976 Posted by: janpom Posted at: 2018-12-30T22:56:37.583Z Reads: 152

```
Yeah, I saw. My impression is still that the intention is to protect against VESC derivatives being called VESCs, such as the original FOCBOX. So while putting VESC on the PCB violates the trademark policies, I can't see why anyone should mind that since the use is clearly in the context of "plug VESC here" as opposed to "this is a VESC thing".

I already ordered the PCBs. I will write an email to Vedder to ask him if the use of the trademark  is OK. I'm convinced he won't have anything against it, especially since this is a non-commercial open source project.

Gosh, I guess I will take @b264's advice next time. I don't have time for dealing with nonsense legal issues.
```

---
## \#977 Posted by: Jc06505n Posted at: 2018-12-30T23:33:10.912Z Reads: 151

```
[quote="janpom, post:976, topic:71509"]
My impression is still that the intention is to protect against VESC derivatives being called VESCs, such as the original FOCBOX.
[/quote]

While I’m not with Trampa, it goes a bit beyond just VESC’s. Think of it as Nintendo. Their trademark not only allows them grounds to pursue anyone who dares tries to name a similar product of the same name , but to ensure that unwanted accessories arent associated all Willy milky with their product. Gives them the ground to say “err no” legally.
```

---
## \#978 Posted by: mmaner Posted at: 2018-12-31T01:56:34.607Z Reads: 149

```
The difference in this case is that both products are open source.
```

---
## \#979 Posted by: High-roller Posted at: 2019-01-01T15:17:55.104Z Reads: 161

```
My screen finally came!
I'm going to put in some pins I've bent 90° in order to make attaching the bootloader easier:
![IMG_20190101_170639|375x499](upload://rQGsUc6F93Q1RBEPiyOm6HT0LpL.jpeg) 
I've already started working on a matching case for it.
![15463557697902597728224372433455|666x500](upload://zKZ2JAtuJDhPHbp18FPPpL74IMm.jpeg) 
I'm probably going to go with the landscape view so I want to put the buttons on the same side in order to keep the footprint as comfortably small as possible.
```

---
## \#980 Posted by: janpom Posted at: 2019-01-01T22:05:44.284Z Reads: 159

```
![dave_pf_2019|500x500](upload://wYJnYfaBAElyrqZcsszwmdhlJhN.png)
```

---
## \#981 Posted by: janpom Posted at: 2019-01-02T18:35:39.640Z Reads: 165

```
Christmas came late this year. This beauty arrived today.

![DSC01778|690x460](upload://i8t5jnqun8iMCnWGlx3vrASOq1i.jpeg) 

It's absolutely fantastic. Quite an upgrade from my $5 HobbyKing soldering iron. No more coffee breaks until the tip heats up. :smiley: Now I feel well prepared for assembling some Daves.

I had to test it and since I just had no useful soldering to do, here's one more PF.

![DSC01779|690x200](upload://h1McNdaZ1IMmbPUFTkg4p0wEa7q.jpeg)
```

---
## \#982 Posted by: mmaner Posted at: 2019-01-02T20:43:52.204Z Reads: 158

```
Do you have a link to that. I likey 😀.
```

---
## \#983 Posted by: Itsmedant Posted at: 2019-01-02T20:45:33.299Z Reads: 158

```
https://www.amazon.com/UY-CHAN-Programmable-Pocket-size-Acceleration/dp/B01MDTO6X7

Looks like this is it.

I'm interested.....time to do some research! It would be nice to get rid of the big soldering station I have.
```

---
## \#984 Posted by: moon Posted at: 2019-01-02T20:46:22.815Z Reads: 151

```
Ive got one with a bc2 tip, it's good for small things
```

---
## \#985 Posted by: Itsmedant Posted at: 2019-01-02T20:47:35.861Z Reads: 147

```
Oh shit....you can run these off of a Lipo?!
```

---
## \#986 Posted by: moon Posted at: 2019-01-02T20:52:50.512Z Reads: 148

```
Yeah and laptop charger
```

---
## \#987 Posted by: janpom Posted at: 2019-01-02T21:09:14.784Z Reads: 158

```
I got mine from [Banggood](https://www.banggood.com/MINI-TS100-Digital-OLED-Programmable-Interface-DC-5525-Soldering-Iron-Station-Built-in-STM32-Chip-p-984214.html?cur_warehouse=CN) for a good price, but I waited 2 months. You can buy replacement tips [here](https://www.banggood.com/MINI-Original-Replacement-Solder-Tip-For-TS100-Digital-LCD-Soldering-Iron-p-984215.html?ID=517509&cur_warehouse=CN). I got the BC2 and D24. Both are very nice. The soldering iron comes with the B2 tip, which I like the best for PCB soldering. People say that you don't get a good heat transfer with conical tips, but with TS100 that's no problem at all.

I got [this DC adapter](https://www.banggood.com/9-24V-3A-72W-ACDC-Adapter-Switching-Power-Supply-Regulated-Power-Adapter-Supply-Display-EU-Plug-p-1250656.html?cur_warehouse=CN), which works nicely with the soldering iron, since you can easily turn it on and off (you can't turn the soldering iron off in any other way then by cutting off the power supply).

There are many TS100 reviews on youtube and it's nothing but praise.

Update: I just found out it's also [available from HobbyKing](https://hobbyking.com/cz_cz/soldering-iron-ts100-bc2.html).
```

---
## \#988 Posted by: mmaner Posted at: 2019-01-02T21:09:55.587Z Reads: 156

```
Bookmarked 😀
```

---
## \#989 Posted by: deucesdown Posted at: 2019-01-02T22:24:36.939Z Reads: 162

```
Good stuff, get the "pro kit" version -- it comes with the non-useless larger chisel tip among other things.

https://www.youtube.com/watch?v=HgrB5P-rDLw

https://www.youtube.com/watch?v=83STpUXHilk

https://www.youtube.com/watch?v=ao39bPEyok4

https://www.youtube.com/watch?v=71R8OksmpWw

https://www.youtube.com/watch?v=EEYt2jTTVdE
(Dave craps on the TS100 too much, it's also good)

Summary:
- ts100 is older/cheaper, plastic case runs off dc power (can run off lipo)
- ts80 is newer, metal case, usb-c, can run off a good usb-c charger or a battery bank (no lipo). less power rating, but more power delivered
- ts100 has more tips available
- ts80 better ergonomics
- both are very good, surprisingly so. spanks all older tech non-cartridge-tip soldering stations.

@mmaner I did ninja edit adding a bunch more crap :slight_smile:

EDIT corrected as per janpom, ouch lol
```

---
## \#990 Posted by: janpom Posted at: 2019-01-02T22:55:46.637Z Reads: 149

```
I think you have TS80 and TS100 the other way around in your summary.

We're getting a bit too much off-topic. If more people would like to discuss TS80 and TS100, I suggest that we move it to another thread.
```

---
## \#991 Posted by: b264 Posted at: 2019-01-02T23:12:14.832Z Reads: 149

```
You'll have to pry my Weller WESD51 out of my cold, dead hands because I'm not giving it up ;-)
```

---
## \#992 Posted by: deucesdown Posted at: 2019-01-02T23:27:31.873Z Reads: 149

```
Your Weller's safe! Can be beat but not by a large margin.

Thanks janpom for the correction, and this is my last post on the soldering irons, but you started it! ;)
```

---
## \#993 Posted by: moon Posted at: 2019-01-03T00:27:19.931Z Reads: 148

```
@moderators split topic

@deucesdown what did you say about chisel tips, anything good enough to do XT90 etc
```

---
## \#994 Posted by: deucesdown Posted at: 2019-01-03T02:12:19.890Z Reads: 164

```
Sigh ok last one for real. :slight_smile:

TS80 is the stronger one.

https://www.aliexpress.com/item/Mini-TS80-Portable-Electric-Soldering-Iron-Adjustable-Temperature-Digital-Solder-Station-OLED-Display-USB-Type-C/32904980528.html

There are 3 variants here. The "Pro Kit" one has a different tip, medium chisel vs the conical on the other 2 variants. TS-D25. For that alone the Pro Kit is the only one worth considering. The kit versions also come with a flexible silicone-like wire, which is really nice for soldering and hard to get otherwise. The tip selection and aftermarket tips for the TS80 is not that good.

I found ebay (wait for 15% coupon) or aliexpress are the cheapest.

I just plugged mine into the wall with the provided power brick, and it took a few seconds longer than my main irons, but XT90 + 10awg no real problem.

The TS100 is not has powerful, but has a much bigger selection of tips, and the TS-C4 tip is quite a bit larger, so might do a similar job. You need to feed it I think at least 19v 3a or so for max power.

For really big stuff I like the 100w Weller pencil. Like battery pack serial connections, quick in and out if space permits. This thing has crazy thermal mass and is temperature controlled tip technology. It's worth having.

https://www.amazon.com/Weller-W100PG-Farenheit-Soldering-Degree/dp/B07C43TSFK/

These cute irons are really nice, but I'm always using my used industrial/commercial irons. Pace and Metcal stuff after patient shopping on ebay. Hint, Pace has much nicer consumables cost and similar performance.

They're fantastic though, if you have to bring the iron to the board.

![IMG_20190102_211511|666x500](upload://l8iQuANbgQILBoDOgE9Muh3nldV.jpeg) 

Left to right: biggest Metcal tip, Weller 100w, biggest ts80 tip.
```

---
## \#995 Posted by: High-roller Posted at: 2019-01-06T15:02:28.968Z Reads: 151

```
[quote="janpom, post:576, topic:71509"]
@mmaner Assuming the FocBox pins are 5V, VCC, GND, ADC1, RX, TX, ADC2, you have the wires swapped on the picture. The connection should be:

5V - 5V
GND - GND
RX - RX
TX - TX
[/quote]

Is this accurate for the flipksy mini fsecs? I'm about to star soldering and I don't have many spares if I screw up.
```

---
## \#996 Posted by: pookybear Posted at: 2019-01-06T16:39:59.141Z Reads: 148

```
I have the ts100. I use it all the time for my RC soldering needs.

Link to the awesome firmware. Lots of cool safety features and more:

https://github.com/Ralim/ts100
```

---
## \#997 Posted by: janpom Posted at: 2019-01-06T18:07:26.443Z Reads: 144

```
That should hold true for any VESC, or more generally, for any UART device.
```

---
## \#998 Posted by: Battosaii Posted at: 2019-01-07T19:27:44.822Z Reads: 152

```
Just got my Davega kit, funny thing is that it came with a 3d printed enclosure I got from a special someone. It was such great luck I was not expecting that lol.

I'll start assembly tonight.
```

---
## \#999 Posted by: High-roller Posted at: 2019-01-08T12:53:57.209Z Reads: 158

```
![15469519927414407826616552233229|666x499](upload://uUZwQ24HPVfSKuxj4nezi0LyD6M.jpeg) 
It's getting there...
```

---
## \#1000 Posted by: lrdesigns Posted at: 2019-01-10T02:02:43.356Z Reads: 158

```
I finally got some free time to post the new case design with angled riser that includes space for 3 waterproof buttons. 

I have only used it in light rain so far but it has been working perfect. Once wet :cloud_with_lightning_and_rain:  season hits I will be adding some coating to the pcbs and a thin coat of silicone around the lip seal. 

It also makes a good foot stop.

![IMG_1854|666x500](upload://hHwAvn3k94sKMvZ7dYle8NvCjNv.jpeg) 

https://www.thingiverse.com/thing:3171000
```

---
## \#1001 Posted by: Andy87 Posted at: 2019-01-11T17:33:28.912Z Reads: 155

```
@janpom is there an easy sw setting to switch the horizontal view 180degree?
It’s not a big deal, but the uart wires would than come out on direction where my focbox is sitting.
Otherwise I would need to route the wires under the pcb to the other side.
If it’s not possible, no problem, just thought I to ask. Maybe it’s an easy thing of just change a variable or so.
```

---
## \#1002 Posted by: SeanHacker Posted at: 2019-01-11T17:37:21.200Z Reads: 151

```
Yep. You can change the orientation in the davega.config here https://github.com/janpom/davega/blob/master/davega_config.h

Line:
// 0=portrait, 1=right rotated landscape, 2=reverse portrait, 3=left rotated landscape
#define SCREEN_ORIENTATION 0
```

---
## \#1004 Posted by: Andy87 Posted at: 2019-01-11T17:53:10.224Z Reads: 143

```
Thx! That’s great!
```

---
## \#1005 Posted by: Andy87 Posted at: 2019-01-13T10:02:30.752Z Reads: 146

```
What a nice project!
Sorry for the question.
Found the fault.
```

---
## \#1006 Posted by: lrdesigns Posted at: 2019-01-14T06:39:38.117Z Reads: 158

```
@janpom thanks so much for incorporating all my feature requests and doing an awesome job of both software and hardware. :clap::clap::clap:  Average cell voltage is really helpful for me. :ok_hand:

![IMG_2043|666x500](upload://lP6TYI6h0ulpeV6mN3SZ2ddQJdp.jpeg)  

There is one feature sorely lacking though, when your going faster and faster and then the speed number turns red, I think it needs to shoot lasers out the front to create a virtual highway and play  _**HIGH WAY TO THE DANGER ZONE**_ really loud!  A red glow under the board might be nice too but that's more of a personal choice. :laughing:

![IMG_2044|544x500](upload://7CwMgfiRxITyy9bQvikCO0pthLS.jpeg) 
![image|545x429](upload://5NDZ7CeWCehSL9jPttUB1uJHQRR.jpeg) 

https://youtu.be/kUsFWO08CO0
```

---
## \#1007 Posted by: Andy87 Posted at: 2019-01-14T06:58:16.639Z Reads: 151

```
that was really a great idea with the average cell voltage.
just installed V4 yesterday and set it up with average cell voltage.
```

---
## \#1008 Posted by: janpom Posted at: 2019-01-14T07:28:54.417Z Reads: 148

```
OK, I'm adding that on the backlog. :smiley:

I see I should adjust the formatting for total km once it gets over 999.
```

---
## \#1009 Posted by: janpom Posted at: 2019-01-14T07:31:09.858Z Reads: 148

```
I will make the avg cell voltage the default in the next version. I personally prefer it too and I believe that most people have a better intuition of how a single cell voltage relates to the SoC rather than the total battery pack voltage.
```

---
## \#1010 Posted by: lrdesigns Posted at: 2019-01-14T07:50:06.065Z Reads: 152

```
[quote="janpom, post:1008, topic:71509"]
I see I should adjust the formatting for total km once it gets over 999.
[/quote]

yeah, there is a weird half a character after the 4th number. Oh I see its a .  decimal and part of a another character. 

Personally for total trip distance I dont need any decimal place just whole KMs.
```

---
## \#1011 Posted by: janpom Posted at: 2019-01-14T07:56:46.598Z Reads: 149

```
Yeah, I'll just switch from 1 decimal to 0 decimal once the count gets over 999.9. I hope that 9999 is then a reasonable max. I think it will have to overflow to 0 after that, just like the good old mechanical car odometers. :smiley:
```

---
## \#1012 Posted by: venom121212 Posted at: 2019-01-15T19:28:21.815Z Reads: 143

```
Anybody playing around with a flushmount screen for a top box enclosure? If not, I'm about to start. I don't have my  davega assembled yet though so I don't have button spacing measurements.
```

---
## \#1013 Posted by: b264 Posted at: 2019-01-15T19:32:05.167Z Reads: 152

```
[quote="janpom, post:1011, topic:71509"]
Yeah, I’ll just switch from 1 decimal to 0 decimal once the count gets over 999.9. I hope that 9999 is then a reasonable max. I think it will have to overflow to 0 after that, just like the good old mechanical car odometers. :smiley:
[/quote]

"1E04" is 10,000
"23E3" is 23,000
"13E3" is 13,000
"6E06" is 6,000,000
"9E99" is 9,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000,000

et cetera

So you could go all the way up to nine-tenths of a googol that way in only 4 characters.
```

---
## \#1014 Posted by: janpom Posted at: 2019-01-16T16:11:50.570Z Reads: 145

```
@b264 OK, now I'm having hard time figuring out whether you're trying to be genuinely helpful or you're trolling or it's a mixture of both. :slight_smile:
```

---
## \#1015 Posted by: janpom Posted at: 2019-01-16T16:15:39.601Z Reads: 152

```
1E04 would have to indicate "somewhere between 10000 and 15000", which honestly doesn't seem very helpful. I personally would much rather have it overflow. :slight_smile:
```

---
## \#1016 Posted by: Jc06505n Posted at: 2019-01-16T16:18:08.099Z Reads: 148

```
Nha he’s jsut tryna help out with presenting big numbers in 4 chars
```

---
## \#1017 Posted by: deucesdown Posted at: 2019-01-16T16:56:28.681Z Reads: 138

```
hehe you can display the value in hex :) FFFF == 65535
```

---
## \#1018 Posted by: janpom Posted at: 2019-01-16T20:43:56.752Z Reads: 138

```
You guys remind me of our UX team. :smiley:

How about this, though: We let it overflow but we change the color after each 10,000. It will start white, then change to yellow, then orange, then green. See the pattern? And after mere 80,000 you gain your black DAVEga belt! The minor downside is that the meter gets slightly hard to read at that point. Also, the black DAVEga belt will be somewhat harder to achieve in US/UK, which is just another evidence that the metric system is superior! :smiley:
```

---
## \#1019 Posted by: b264 Posted at: 2019-01-16T22:30:07.303Z Reads: 131

```
If you can succeed in convincing my fellow citizens that the metric system is better, I'll buy you dinner.  It's mainly the construction industry that's holding our entire country back with that crap.
```

---
## \#1020 Posted by: banjaxxed Posted at: 2019-01-16T22:42:24.729Z Reads: 135

```
@b264 is Vulcan, make what you want of it!
```

---
## \#1021 Posted by: lrdesigns Posted at: 2019-01-17T00:51:55.947Z Reads: 151

```
Hey @janpom what is your future plans for the info screen?  

![image|442x322](upload://5aEti7m6cMjC5RfLHZMijmKb1h3.jpeg) 

I find the font size so small that it's quite hard to read, I would rather less info in larger font.  Some of the info is duplicate of what is on the main screen so that could be removed. Current speed seems not useful as you can't look at this tiny text and read it while riding. 

There are two bits of info I was really looking forward to having on this screen, Battery max & min/regen amps. Are these hard to implement?
```

---
## \#1022 Posted by: janpom Posted at: 2019-01-17T06:49:34.001Z Reads: 147

```
I can definitely make the list of items and the font size configurable. I'll look into the battery amps. Shouldn't be hard to add and I agree that's a good piece of info to have.
```

---
## \#1023 Posted by: High-roller Posted at: 2019-01-17T09:10:33.549Z Reads: 157

```
![IMG_20190117_110529|375x499](upload://kBAioUvPK2gLF9t9sJj4Bga0BVL.jpeg) ![IMG_20190117_110556|666x499](upload://9zvuDk1Goe8veNZUmmlPQWuRbC1.jpeg) 
My first iteration is done! Once I receive the waterproof buttons I ordered I'll make a nicer one but this works for now. Easy access to the programming port, and I can adjust the viewing angle if I need to.
Now if the post office would just let me have my battery enclosure I could do test ride in the next few days.
```

---
## \#1024 Posted by: lrdesigns Posted at: 2019-01-17T09:13:18.434Z Reads: 155

```
What the hell is this? An eskate for mars?

Those tires are out of this world!
```

---
## \#1025 Posted by: High-roller Posted at: 2019-01-17T09:15:04.276Z Reads: 160

```
Thanks! Yeah, I keep getting that. I have the beginnings of a build thread for it but it's taken a while to get it all together.
https://www.electric-skateboard.builders/t/swing-arm-sensation-wip-madeus-maximus-aka-the-height-of-insanity-bmw-streetcarver-trucks-29-jetspud-dual-diagonal-6374-flipsky-minifsesc-4-20-battery-tbd/75118
```

---
## \#1026 Posted by: High-roller Posted at: 2019-01-17T09:18:15.354Z Reads: 158

```
[quote="lrdesigns, post:1024, topic:71509"]
An eskate for mars?
[/quote]

Hmm, now that you mention it...
...aaaand there goes my next paycheck on a third build.
```

---
## \#1027 Posted by: janpom Posted at: 2019-01-18T08:01:05.755Z Reads: 166

```
Look what just arrived.

![IMG_1614|383x500](upload://2l0bopWYBSVXv9OfI25APxRlpOb.jpeg) 

![IMG_1616|690x469](upload://gw4hzZRki2Rc5w8jSLko2zNpqou.jpeg) 

Quick test if everything fits.

![IMG_1617|690x457](upload://fk3Va8MDIjjwP9bTjj04bDbCz6b.jpeg) 

I'll assemble one tonight. If it works, I'll be good to start the 2nd batch.
```

---
## \#1028 Posted by: lrdesigns Posted at: 2019-01-18T09:11:25.505Z Reads: 159

```
Is that like 100 boards?
```

---
## \#1029 Posted by: janpom Posted at: 2019-01-18T10:07:39.706Z Reads: 164

```
Good guess. :slight_smile:
```

---
## \#1030 Posted by: janpom Posted at: 2019-01-18T22:52:56.432Z Reads: 164

```
So I assembled one and all works!

![IMG_1624|690x466](upload://bW69yM7EfsDi2VVucAURGaiWxry.jpeg) 

The 100 uF capacitor is pretty big. It's slightly taller than the MCU. Still not taller than the display headers. If someone will want to make it really really low profile with no display headers and no JST connector, they will have to either leave out the capacitor (it's not a critical component) or solder it outside of the PCB. This is the only problem I have found so far and it's pretty minor.

![IMG_1627|690x187](upload://pJV1XGzA3a0bSaiDectzpqbi9yG.jpeg) 

![IMG_1628|690x145](upload://q2sxCWZwglTeJJncPwCcYPZHoa7.jpeg)
```

---
## \#1031 Posted by: b264 Posted at: 2019-01-18T22:55:01.563Z Reads: 160

```
Maybe using two 47μF capacitors that are thinner would work also, or just a 47μF
```

---
## \#1032 Posted by: janpom Posted at: 2019-01-18T23:08:18.330Z Reads: 164

```
Unfortunately I haven't found any thinner axial electrolytic capacitors. The thinnest that mouser has are 4.5mm diameter. Capacitors of various capacitance are available in this size and the 100uF is the highest, so that's what I ordered. It's [this one](https://cz.mouser.com/ProductDetail/Vishay-BC-Components/MAL202124101E3?qs=sGAEpiMZZMu3dWSqd4Tl0IrB%252bE%2fYPbXzdcGGOLzGjbQ%3d). In reality it's slightly more than 4.5mm. I measured closer to 5mm.

We could use radial instead of axial and bend the legs, but I don't like that. Plus I haven't even checked if a thinner radial is available.

Edit: Found [this](https://cz.mouser.com/ProductDetail/Nichicon/UVR1A101MDD6?qs=UBiR96IgLrSPbXe39cac9Q%3d%3d) for radial. Also 100uF but only 4mm diameter.
```

---
## \#1033 Posted by: b264 Posted at: 2019-01-18T23:19:00.050Z Reads: 163

```
I agree with not bending legs when extreme vibrations are involved
```

---
## \#1034 Posted by: b264 Posted at: 2019-01-18T23:19:15.510Z Reads: 161

```
How about surface mount ceramic?
```

---
## \#1035 Posted by: totalgeek9224 Posted at: 2019-01-19T07:01:25.984Z Reads: 162

```
Not sure if this is a design no-no, but how about a cutout for the Cap that would allow it to go through the pcb narrowing down the top profile?
```

---
## \#1036 Posted by: janpom Posted at: 2019-01-19T09:32:06.841Z Reads: 166

```
Interesting idea. I like that. Should be easy to do with a bit of drilling and filing for those who want to narrow down the profile.
```

---
## \#1037 Posted by: janpom Posted at: 2019-01-19T09:33:15.018Z Reads: 168

```
All set. Time to make some Daves. :slight_smile: 

![DSC01818|690x460](upload://sYzKXYV8z6nAaWk7lZAZYzMx2xY.jpeg) 

![DSC01819|690x460](upload://ukJgGslUMyE8zStuQow5O8LtbDh.jpeg)
```

---
## \#1038 Posted by: JonathanLau1983 Posted at: 2019-01-22T16:55:30.780Z Reads: 161

```
@janpom I'm looking at updating to fimrware 0.4 tonight or tomorrow and I've just been reading your notes. It's a new build which hasn't got any miles on it yet, so should I just change the EEPROM_MAGIC_VALUE value to something new? Any arbitrary number?
```

---
## \#1039 Posted by: janpom Posted at: 2019-01-22T18:37:33.291Z Reads: 162

```
Correct. Note that the 0.4 has a different magic number than the previous versions so chances are you don't need to touch it at all.
```

---
## \#1040 Posted by: janpom Posted at: 2019-01-25T21:42:37.288Z Reads: 165

```
https://www.electric-skateboard.builders/t/davega-second-batch/82070
```

---
## \#1041 Posted by: TUTOS_BRICOLAGES Posted at: 2019-01-26T09:44:37.463Z Reads: 167

```
hello, I wanted to thank janpom and other guys Who haveWho participated in the project, For all the work on the DAVEga, a big thank you!
I am a French and I made a video on DAVEga on my Youtube channel On which I already made an electric skateboard and an electric scooter with an esk8 engine to go to 45kph, I have for the moment to install the DAVEga on my electric scooter, the link if the video : https://youtu.be/x95_16zzV8s 

![IMG_20190122_164037|666x500](upload://twEeIGHaS1rQ7aFmEWwn4kGLg0L.jpeg)
```

---
## \#1042 Posted by: janpom Posted at: 2019-01-26T14:01:35.565Z Reads: 165

```
Cool! Great to see someone build it with the Nano. I also love the plastic box idea. So simple and seems to work great. Thanks for sharing the vid. I wish I spoke some French. :slight_smile:
```

---
## \#1043 Posted by: TUTOS_BRICOLAGES Posted at: 2019-01-26T14:16:29.009Z Reads: 162

```
thanks, for the plastic box, it's because I do not have a 3d printer and it turned out to be a good idea.
```

---
## \#1044 Posted by: JonathanLau1983 Posted at: 2019-01-26T16:02:06.806Z Reads: 168

```
@janpom Could we get motor temperature added to the screen with all the info listed? Not so important in winter, but in summer it would be useful. 
Thanks!
```

---
## \#1045 Posted by: janpom Posted at: 2019-01-26T16:13:14.801Z Reads: 173

```
OK. [I added it on the backlog](https://github.com/janpom/davega/issues/21). I may need to make the items on the text screen configurable first though because if I add one more item, I'm afraid it already won't fit on screen with the horizontal layout. It's pretty straightforward. I just need to find some time for it.
```

---
## \#1046 Posted by: b264 Posted at: 2019-01-26T16:20:29.395Z Reads: 168

```
Rule of mine is any post with github link gets automatic "like"
```

---
## \#1047 Posted by: JonathanLau1983 Posted at: 2019-01-26T21:27:10.537Z Reads: 169

```
Nice one, thanks!
```

---
## \#1048 Posted by: janpom Posted at: 2019-01-28T08:01:49.285Z Reads: 176

```
I got this beauty as a gift from @lrdesigns. :heart_eyes: 

![DSC01838|617x500](upload://gNhMx7eWGtVUWWPx3zeHSOkBZzy.jpeg) 

![DSC01837|593x500](upload://5TYj2amcjJ3iUadW0wa0UoobegJ.jpeg) 

Thanks a lot, Luke. I'm not sure if the angle won't be too much for my falcon, but this is definitely going on a build, even if I have to start a new one for it. :smiley:
```

---
## \#1049 Posted by: banjaxxed Posted at: 2019-01-28T09:30:58.911Z Reads: 167

```
Noice. Looks molded but must be sanded. I've printed out one of these as well and loving the form/function
```

---
## \#1050 Posted by: lrdesigns Posted at: 2019-01-28T09:32:19.516Z Reads: 168

```
No sanding, SLA printing. Comes right outa the printer like that.
```

---
## \#1051 Posted by: banjaxxed Posted at: 2019-01-28T09:38:26.802Z Reads: 172

```
Ah yes SLA, makes sense 👍

Here's a CarbonFill lower with a Graphene top, will need some post-processing since the Graphene has to be dialled in. I'm aware both materials are conductive ![IMG_9448|666x500](upload://zSSsDTmKa5nD7eRRr1zuJjUnlHH.jpeg)
```

---
## \#1052 Posted by: venom121212 Posted at: 2019-01-28T13:27:49.813Z Reads: 168

```
I was an early backer of the peachy printer because I love the idea of SLA. Lost my money and never got the product from Kickstarter :expressionless:
```

---
## \#1053 Posted by: Jaydawg56 Posted at: 2019-01-28T14:00:12.972Z Reads: 170

```
When do you think you’ll open this up to more folks? A little late but can definitely solder and assemble pretty easily. Thanks!
```

---
## \#1054 Posted by: venom121212 Posted at: 2019-01-28T14:09:34.747Z Reads: 169

```
Already did. Search this thread
```

---
## \#1055 Posted by: SeanHacker Posted at: 2019-01-28T14:55:48.819Z Reads: 170

```
https://www.electric-skateboard.builders/t/davega-second-batch/82070
```

---
## \#1056 Posted by: janpom Posted at: 2019-01-28T20:03:47.747Z Reads: 161

```
Unfortunately I can't edit the original post any more, otherwise I would put the 2nd batch link there so that it's easier to find.
```

---
## \#1057 Posted by: SeanHacker Posted at: 2019-01-28T23:43:55.232Z Reads: 165

```
Dude. He does some great work. This thing is beautiful!!! @lrdesigns you killed it! Thanks!!!

![IMG_20190128_144504|665x500](upload://pepRdPmnyI20jDDOSNYj1CnK8ad.jpeg)
```

---
## \#1058 Posted by: lrdesigns Posted at: 2019-01-29T01:21:05.166Z Reads: 162

```
@banjaxxed your print looks quite good for FDM, the design was never intended to be printed in FDM, how did it go with the overhangs, and there is some thin wall where the bolt holes go past the LCD?
```

---
## \#1059 Posted by: briman05 Posted at: 2019-01-29T01:41:39.881Z Reads: 159

```
That is top notch it looks awesome.
```

---
## \#1060 Posted by: ZachTetra Posted at: 2019-01-29T02:20:52.203Z Reads: 160

```
Does anyone know if it will work with the MayTech dual 50A ESC?  It’s based on the VESC 4.12 so I assume it will
```

---
## \#1061 Posted by: lrdesigns Posted at: 2019-01-29T02:23:04.322Z Reads: 158

```
If it has a spare uart port and uses standard firmware it should.
```

---
## \#1062 Posted by: ZachTetra Posted at: 2019-01-29T02:27:56.352Z Reads: 156

```
If it’s one of the 2 6 pin ports then it seems so, does it matter which side it’s connected to on a dual ESC?  (Can I plug in 2?)
```

---
## \#1063 Posted by: janpom Posted at: 2019-01-29T05:59:59.272Z Reads: 150

```
It doesn't matter and yes, you can plug-in two.
```

---
## \#1064 Posted by: banjaxxed Posted at: 2019-01-29T09:35:16.325Z Reads: 155

```
I didn’t use support on the bottom, where this was a problem was the cable holes through the slant, a little bit of droop there but not bad and not seen the blowers and the filament helped. I got a little lucky 

I saw the thin wall around the bolt hole, I may need to dress those up a bit as they were touched by plate build support
```

---
## \#1065 Posted by: Skunk Posted at: 2019-01-29T09:37:30.131Z Reads: 159

```
What you can do if find the post # and change the title of the thread and add the post # so it's quicker to find
```

---
## \#1066 Posted by: janpom Posted at: 2019-01-29T10:27:33.213Z Reads: 165

```
Installed! More buttons ordered. I only had one.

![IMG_1641|666x500](upload://xptBgofP2iLfLXIFo8OnCGZGx0l.jpeg)

![IMG_1638|666x500](upload://mF25tYNUmVOJx6NFTO7VzdCCpYN.jpeg) 

Connected to VESC.

![IMG_1639|666x500](upload://xwY66E5bvpNu9B6MxyJJeRdqmGZ.jpeg)

![IMG_1640|666x500](upload://3lp6WIvmh744wWqizJhMgMb2RwF.jpeg)

Testing the view angle on falcon. It's not perfect, but not too bad either. I can still read the display while standing on the board with no problems.

![IMG_1642|375x500](upload://47CyH4FW6QRUviycu3a1PhXIf6H.jpeg)

I love how easy it is to use the enclosure. And it looks great. Thanks again @lrdesigns.
```

---
## \#1067 Posted by: lrdesigns Posted at: 2019-01-29T12:51:58.901Z Reads: 156

```
Will it work if you flip it upside down, buttons on rider side?
```

---
## \#1068 Posted by: janpom Posted at: 2019-01-29T13:10:02.882Z Reads: 157

```
I tried that and I don't think that would work well. The enclosure angle is greater than the board tip angle so if you flip it the display is facing slightly away from the rider. It looks weird and I think reflections would be a problem.

The enclosure is actually a great fit for the board tail since the tip there is angled slightly down. I guess I'll just have to learn riding backwards. :smiley:
```

---
## \#1069 Posted by: SeanHacker Posted at: 2019-01-29T21:19:37.631Z Reads: 157

```
Any of you guys in the USA have an extra screen you want to sell me. Fucking stepped on my only 2 inch screen. I have a ton of 2.2" ones but they won't fit in my @lrdesigns enclosure. :sob:

Edit: I said fuck it and ordered from ALi. Paid twice as much as the screens for faster shipping. I seriously can't be out my DAVega's. I need them now. :)
```

---
## \#1070 Posted by: janpom Posted at: 2019-02-06T22:10:53.960Z Reads: 163

```
I finally found some time and energy to do more developments. I added more items to the text screen.

- MOSFET temperature
- motor temperature
- motor current
- battery current
- duty cycle

I originally only wanted to add the motor temperature as per a request from @JonathanLau1983, but since I was already at it I thought I could just as well add a little more stuff since it was pretty straightforward.

Note that you have to have the motor NTC connected to the VESC, otherwise you'll get rubbish negative numbers for the motor temperature (as shown at the picture :slight_smile:).

Temperatures are in Fahrenheit when imperial units are on.

 ![IMG_1650%202|362x499](upload://pxONXNFOfIe2M0I1EQPdYmCsc3K.jpeg) 

Since there's already more items than the text screen can accommodate, you can now configure which ones you want to see. Here's the relevant excerpt from the config (mind the trailing backslashes, which are mandatory):

```c
// Information to be displayed on the text screen. Only relevant if TEXT_SCREEN_ENABLED is set.
// Available options:
//    TSCR_FW_VERSION
//    TSCR_MOSFET_TEMPERATURE
//    TSCR_MOTOR_TEMPERATURE
//    TSCR_MOTOR_CURRENT
//    TSCR_BATTERY_CURRENT
//    TSCR_DUTY_CYCLE
//    TSCR_TOTAL_VOLTAGE
//    TSCR_MIN_TOTAL_VOLTAGE
//    TSCR_AVG_CELL_VOLTAGE
//    TSCR_BATTERY_CAPACITY_MAH
//    TSCR_BATTERY_CAPACITY_PERCENT
//    TSCR_TRIP_DISTANCE
//    TSCR_TOTAL_DISTANCE
//    TSCR_SPEED
//    TSCR_MAX_SPEED
//    TSCR_AVG_SPEED
//    TSCR_TIME_ELAPSED
//    TSCR_TIME_RIDING
//    TSCR_FAULT_CODE
#define TEXT_SCREEN_ITEMS { \
    TSCR_TOTAL_VOLTAGE, \
    TSCR_MIN_TOTAL_VOLTAGE, \
    TSCR_AVG_CELL_VOLTAGE, \
    TSCR_BATTERY_CAPACITY_MAH, \
    TSCR_BATTERY_CAPACITY_PERCENT, \
    TSCR_TRIP_DISTANCE, \
    TSCR_TOTAL_DISTANCE, \
    TSCR_SPEED, \
    TSCR_MAX_SPEED, \
    TSCR_AVG_SPEED, \
    TSCR_TIME_RIDING, \
    TSCR_FAULT_CODE, \
}
``` 

I believe that someone (@lrdesigns?) has asked for a bigger font. There's now an option for that as well (though I would call it rather experimental :slight_smile:). It's only recommended for the horizontal layout. Note that some items may overflow the right border. It's easy to adjust (shorten) the labels in the code (`davega_text_screen.cpp`). I may move the labels to the config at some point if there's interest.

![IMG_1651%202|690x454](upload://4qRq2rUTw5fqaNR6Um7kZw0sWSL.jpeg)
```

---
## \#1071 Posted by: yelnats8j Posted at: 2019-02-06T22:17:04.375Z Reads: 157

```
![15494913813386943424577620272635|375x500](upload://clWDH0y4uqJcm2KnqHbSlifjEK7.jpeg)

YAYAYAYYAYAY IT CAME
```

---
## \#1072 Posted by: JonathanLau1983 Posted at: 2019-02-07T16:51:56.083Z Reads: 156

```
Thanks for the update @janpom! 

[quote="janpom, post:1070, topic:71509"]
Temperatures are in Fahrenheit when imperial units are on.
[/quote]

We use mph in the UK and Celcius for temperature, so anyone using the new firmware will need to swap the logic around for the temperature calculation.
```

---
## \#1073 Posted by: JonathanLau1983 Posted at: 2019-02-07T17:25:55.033Z Reads: 147

```
Either manually changing the code or whether we introduce Imperial, Metric and UK as options.
We do like to be difficult, just look at Brexit.
```

---
## \#1074 Posted by: janpom Posted at: 2019-02-07T19:16:57.765Z Reads: 146

```
[quote="JonathanLau1983, post:1072, topic:71509"]
We use mph in the UK and Celcius for temperature
[/quote]

You guys in UK and US are hopeless when it comes to units. :smiley:

I can just add another config option for the temperature units. That's easy. Will put kids to bed and I'm right on it.
```

---
## \#1075 Posted by: yelnats8j Posted at: 2019-02-07T19:18:16.801Z Reads: 146

```
[quote="janpom, post:1074, topic:71509"]
UK and US are hopeless
[/quote]

Tell me about it I miss living in a metric country
```

---
## \#1076 Posted by: b264 Posted at: 2019-02-07T19:40:35.537Z Reads: 149

```
[quote="janpom, post:1074, topic:71509"]
You guys in UK and US are hopeless when it comes to units.
[/quote]

The construction industry is holding us back.  Engineering is already almost totally metric or at least metric-friendly.  Most of the construction workers, especially union ones, would rather break into your house at night and murder you, rather than be told what a millimeter is.

We have huge home improvement stores here called "Home Depot" and "Menards" and they think metric is some sort of joke.  I went to buy a tape measure and they had 80+ different models -- not a single one had metric on it.  I had to tell them to eat my shit and ordered one online right in front of them.  If they go out of business, we will know why and I won't feel bad for them.
```

---
## \#1077 Posted by: JonathanLau1983 Posted at: 2019-02-07T19:42:58.587Z Reads: 149

```
You the man!
```

---
## \#1078 Posted by: janpom Posted at: 2019-02-07T20:18:49.067Z Reads: 147

```
done (https://github.com/janpom/davega/commit/d9425aba3ae16d9b9dc623bb653c54dfd3618238)

edit: And [now](https://github.com/janpom/davega/commit/a0f70e56d865c84d97d352af99d7ab578f1a08f9) it even actually converts the values to Fahrenheit rather than just changing the name of the units. :sweat_smile:
```

---
## \#1079 Posted by: venom121212 Posted at: 2019-02-07T22:50:56.504Z Reads: 145

```
Finally somebody who truly understands my pain. I'm not great at metric yet but it is so much more simple. It's like it was designed to make sense.
```

---
## \#1080 Posted by: moon Posted at: 2019-02-07T23:41:47.400Z Reads: 143

```
I have terrible and imperial but somethings of metric Im too used to like mph
```

---
## \#1081 Posted by: StickyBlue Posted at: 2019-02-07T23:46:18.120Z Reads: 139

```
Aviation is also terrible with units

Pay for POUNDS (not fluid ounces) of fuel, but instruments commonly display Liters/minute fuel flow
```

---
## \#1082 Posted by: Indiangummy Posted at: 2019-02-08T01:19:08.069Z Reads: 144

```
[quote="venom121212, post:1079, topic:71509"]
It’s like it was designed to make sense
[/quote]

That's cause it was! xd.
```

---
## \#1083 Posted by: lrdesigns Posted at: 2019-02-08T01:29:51.673Z Reads: 146

```
[quote="b264, post:1076, topic:71509"]
80+ different models – not a single one had metric on it.
[/quote]

That is crazy! Almost every tape measure around here has both on it.
```

---
## \#1084 Posted by: venom121212 Posted at: 2019-02-08T02:01:57.851Z Reads: 149

```
I can confirm. I went to both of our major hardware stores and found exactly one tape measure that had metric. 

The metric was a conversion table on the back of the reel...
```

---
## \#1085 Posted by: Indiangummy Posted at: 2019-02-08T02:20:01.581Z Reads: 150

```
Just received it. Thanks so much for this @janpom
![20190207_211839|690x335](upload://dd3pIwd8E20xudy8QwqJgrwwnE9.jpeg) 

Now just waiting on the screen. I ordered during Chinese new year so I'm not expecting it for a while.
```

---
## \#1086 Posted by: janpom Posted at: 2019-02-10T18:43:24.396Z Reads: 144

```
[quote="ROFEN13, post:11, topic:74270, full:true"]
Im having trouble installing the V.4 firmware. I soldered both board (Both ATmega chips have 2 dots from you on them). I followed the steps on GitHub and installed the library and driver but it get stuck uploading. Just a flashing red dot in the middle of the DAVEga display.
Both USBs you seny and boards have the same issue. Did I miss something? Thanks for your time!
[/quote]

@ROFEN13 What do you select as "Port" in the Arduino IDE? Please share the console output (the last ~10 lines) from when the FW upload gets stuck. Detailed pictures of the board (without the display) would be helpful. Ideally both sides.
```

---
## \#1087 Posted by: ROFEN13 Posted at: 2019-02-10T19:04:29.070Z Reads: 152

```
Hopefully I've done something dumb and just overlooked something!
The only port available is "Com 7" (windows)

![20190210_135405|666x500](upload://vLtEVBGUou6i1OUI2u3VjVk8OV2.jpeg) ![20190210_135325|666x500](upload://pXY2LKAdxoJG9bb4o6eWx2bGmPx.jpeg) 

C:\Users\Trevo_000\Downloads\davega-v0.1\davega-v0.1.ino:192:20: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]

             return "unexpected fault code";

                    ^

C:\Users\Trevo_000\Downloads\davega-v0.1\davega-v0.1.ino: In function 'void setup()':

C:\Users\Trevo_000\Downloads\davega-v0.1\davega-v0.1.ino:215:38: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]

     display_set_fw_version(FW_VERSION);

                                      ^

C:\Users\Trevo_000\Downloads\davega-v0.1\davega-v0.1.ino: In function 'void loop()':

C:\Users\Trevo_000\Downloads\davega-v0.1\davega-v0.1.ino:276:42: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]

         display_set_fw_version(FW_VERSION);

                                          ^



sketch\vesc_comm.cpp: In function 'vesc_comm_fault_code vesc_comm_get_fault_code(uint8_t*)':

sketch\vesc_comm.cpp:179:26: warning: invalid conversion from 'uint8_t {aka unsigned char}' to 'vesc_comm_fault_code' [-fpermissive]

     return vesc_packet[55];
```

---
## \#1088 Posted by: janpom Posted at: 2019-02-10T19:14:48.894Z Reads: 152

```
[quote="ROFEN13, post:1087, topic:71509"]
The only port available is “Com 7” (windows)
[/quote]

I you unplug the USB-UART adapter, does that port disappear from the options?

The diode is reversed on the board with no display headers. The black end must be on the left hand side. I suppose this is not the one you have tested though, right?

When you power it on, the display is rendered correctly? Have you tried connecting it to a VESC?

The console output that you provided are only warnings. That shouldn't be the last thing you see before the FW starts uploading. There should be something like:

```
avrdude: Version 6.3-20171130
         Copyright (c) 2000-2005 Brian Dean, http://www.bdmicro.com/
         Copyright (c) 2007-2014 Joerg Wunsch

         System wide configuration file is "/Users/xpomikal/Library/Arduino15/packages/arduino/tools/avrdude/6.3.0-arduino14/etc/avrdude.conf"
         User configuration file is "/Users/xpomikal/.avrduderc"
         User configuration file does not exist or is not a regular file, skipping

         Using Port                    : /dev/cu.SLAB_USBtoUART
         Using Programmer              : arduino
         Overriding Baud Rate          : 115200
```
```

---
## \#1089 Posted by: Mich21050 Posted at: 2019-02-10T19:19:27.793Z Reads: 145

```
Diode is reversed.. And some solder joints look cold.  :slight_smile:
Did you install the uart driver?
![15498264414095403510395705885687|375x500](upload://yoQgAIm1MiJcSbKvUkePb5a8v9z.jpeg)
```

---
## \#1090 Posted by: ROFEN13 Posted at: 2019-02-10T19:42:45.051Z Reads: 142

```
I checked in system management and Com 7 is the port designated with uart driver. It does disappear when unplugged. Everything on the screen appears as it should when in the computer, I haven't tried it connected to the vesc yet, I was trying to configure it to my board first
That is the last thing that appears before it stops....

"C:\Users\Trevo_000\Desktop\davega-v0.4\davega-v0.4.ino:86:44: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]

Sketch uses 25700 bytes (83%) of program storage space. Maximum is 30720 bytes.
Global variables use 1102 bytes (53%) of dynamic memory, leaving 946 bytes for local variables. Maximum is 2048 bytes.

An error occurred while uploading the sketch"
```

---
## \#1091 Posted by: janpom Posted at: 2019-02-10T19:52:07.339Z Reads: 138

```
It would be helpful if you could try connecting it to VESC. If that works, it means the serial connection is functional. That's used both for VESC communication and for FW update. There could be a problem in the RESET net -- that's the diode, resistor, and the 100n cap. Its purpose is to reset the MCU before the FW upload.

One more thing. In your Arduino IDE preferences, please turn the "Show verbose output during:" for both compilation and update. Then please send the console output again. It should have more details.
```

---
## \#1093 Posted by: b264 Posted at: 2019-02-10T20:04:44.478Z Reads: 136

```
The diode (1N4148) is backwards on one of those (the top one in the photo).  Direction is critical.
```

---
## \#1094 Posted by: ROFEN13 Posted at: 2019-02-10T20:14:50.867Z Reads: 144

```
I reversed the Diode so both DAVEgas are correct now. This is the error I get.

avrdude: Version 6.3, compiled on Jan 17 2017 at 12:00:53
         Copyright (c) 2000-2005 Brian Dean, http://www.bdmicro.com/
         Copyright (c) 2007-2014 Joerg Wunsch

         System wide configuration file is "C:\Program Files (x86)\Arduino\hardware\tools\avr/etc/avrdude.conf"

         Using Port                    : COM7
         Using Programmer              : arduino
         Overriding Baud Rate          : 57600
avrdude: stk500_getsync() attempt 1 of 10: not in sync: resp=0x08
avrdude: stk500_getsync() attempt 2 of 10: not in sync: resp=0xa0
avrdude: stk500_getsync() attempt 3 of 10: not in sync: resp=0xfc
avrdude: stk500_getsync() attempt 4 of 10: not in sync: resp=0x00
avrdude: stk500_getsync() attempt 5 of 10: not in sync: resp=0x20
avrdude: stk500_getsync() attempt 6 of 10: not in sync: resp=0xfc
avrdude: stk500_getsync() attempt 7 of 10: not in sync: resp=0x08
avrdude: stk500_getsync() attempt 8 of 10: not in sync: resp=0x20
avrdude: stk500_getsync() attempt 9 of 10: not in sync: resp=0xfc
avrdude: stk500_getsync() attempt 10 of 10: not in sync: resp=0x08

Thanks for your help everyone! I will check the connection with the Vesc later today.
```

---
## \#1095 Posted by: janpom Posted at: 2019-02-10T20:18:44.991Z Reads: 136

```
[quote="ROFEN13, post:1094, topic:71509"]
Overriding Baud Rate : 57600
[/quote]

This looks wrong. Should be 115200. What do you have in `Tools > Board` and `Tools > Processor`?
```

---
## \#1096 Posted by: ROFEN13 Posted at: 2019-02-10T20:22:28.275Z Reads: 134

```
Adurino nano and atmega328p
I saw that the baud rate wasnt right but didnt know how to change it....

Same exact readout on both boards (After it has been fixed).
```

---
## \#1097 Posted by: janpom Posted at: 2019-02-10T20:31:45.607Z Reads: 141

```
`Tools > Board > Board Manager...` then find `Arduino AVR Boards` (should be at the top). What version do you have? If not the latest, try installing the latest.
```

---
## \#1098 Posted by: ROFEN13 Posted at: 2019-02-10T20:37:10.047Z Reads: 140

```
Well guess what.... it worked! Hahaha thank you so much!! Im glad it was vecause I overlooked something dumb![15498309610667532707130882520364|666x500](upload://5IgzwKAV2noh3R9eeywytOBCX71.jpeg)
```

---
## \#1099 Posted by: janpom Posted at: 2019-02-10T20:39:35.335Z Reads: 145

```
Great!
10c
```

---
## \#1100 Posted by: TUTOS_BRICOLAGES Posted at: 2019-02-11T15:32:42.362Z Reads: 152

```
![IMG_20190210_184700_776|500x500](upload://jwpFVbhfyMus3S1LISFHjEf13sG.jpeg) ![IMG_20190210_184700_778|500x500](upload://f4UaDA0bEnn4NciTZQcIPHWu6oF.jpeg) 

a new DAVEga installed! on my esk8 this time!
```

---
## \#1101 Posted by: janpom Posted at: 2019-02-15T15:59:51.421Z Reads: 147

```
@mmaner I am about to get the latest version of your enclosure printed. I'm trying to wrap my head around the buttons. I understand that the printed caps should be glued to the buttons, but what exactly is the idea for holding the buttons in place?

I really like the [metal panel mount buttons](https://www.aliexpress.com/item/1pc-8mm-Momentary-Metal-Stainless-Steel-Horn-Doorbell-Bell-Push-Button-Switch-Waterproof-Car-Auto-Engine/32879072096.html) that @lrdesigns uses. They look great and are easy to install. I'm afraid they are slightly too big for your enclosure. Any ideas for a simple mod that would allow using those? Thanks.
```

---
## \#1102 Posted by: mmaner Posted at: 2019-02-15T16:22:58.932Z Reads: 144

```
There are recesses on the inside of the case that hold the buttons in place, I just use a little hot glue to keep them from moving. I wish I could find some 6 or 8 mm momentary switches to use.
```

---
## \#1103 Posted by: ROFEN13 Posted at: 2019-02-15T16:30:23.804Z Reads: 152

```
Hey everyone. Another issue. It isnt reading from the vesc. I have 
Rx to rx
Tx to tx
Ground to ground
5v to 5v
Both Davegas have the same problem and it happens to both vescs. 
Baud rate is 115200
![20190215_111641|375x500](upload://AfCZEmWp1lARVXLSNjickBoNREl.jpeg) 
Thanks again all.
```

---
## \#1104 Posted by: Jaydawg56 Posted at: 2019-02-15T16:40:33.028Z Reads: 143

```
Do you mean you have TX to TX on both sides (VESC and DAVE) or is it implied you mean you have a TX to RX (VESC to DAVE)?
```

---
## \#1105 Posted by: ROFEN13 Posted at: 2019-02-15T16:46:56.724Z Reads: 150

```
[quote="janpom, post:576, topic:71509"]
[mmaner](/u/mmaner) Assuming the FocBox pins are 5V, VCC, GND, ADC1, RX, TX, ADC2, you have the wires swapped on the picture. The connection should be:

5V - 5V
GND - GND
RX - RX
TX - TX
[/quote]

Same as this.
```

---
## \#1106 Posted by: Tinp123 Posted at: 2019-02-15T17:14:40.060Z Reads: 146

```
1. App Settings; General; App to Use:  **PPM and UART**

Did you do this? 
I did setup yesterday and it works great!
```

---
## \#1107 Posted by: mmaner Posted at: 2019-02-15T17:16:44.671Z Reads: 148

```
I can print you the enclosure and mount the buttons and send it to you if you like, I have all the pieces on my bench.  It will take awhile to get to you.
```

---
## \#1108 Posted by: Mich21050 Posted at: 2019-02-15T17:32:40.774Z Reads: 142

```
I could print it for you.. :slight_smile: I still owe you something :wink: :slight_smile:
@mmaner just offering it bc. I'm within the EU.. :slight_smile:
```

---
## \#1109 Posted by: ROFEN13 Posted at: 2019-02-15T17:33:32.821Z Reads: 140

```
Yeah i did
```

---
## \#1110 Posted by: mmaner Posted at: 2019-02-15T17:40:12.679Z Reads: 137

```
Cool, no worries, I can send the buttons if they are difficult to source there.
```

---
## \#1111 Posted by: janpom Posted at: 2019-02-15T19:57:17.620Z Reads: 141

```
[quote="mmaner, post:1107, topic:71509"]
I can print you the enclosure and mount the buttons and send it to you if you like, I have all the pieces on my bench.
[/quote]

That's very nice of you. Thanks for the offer, but shipping from US to EU costs arm and leg. It's not worth it. I can ask a friend to print it for me.

Could you please just share the link for the correct buttons? I'm sure it's somewhere in this thread, but I can't find it. There's too much stuff already.
```

---
## \#1112 Posted by: janpom Posted at: 2019-02-15T19:58:52.241Z Reads: 141

```
[quote="Mich21050, post:1108, topic:71509"]
I could print it for you
[/quote]

Thanks, Michael. I appreciate the offer, but it won't be necessary.
```

---
## \#1113 Posted by: mmaner Posted at: 2019-02-15T20:17:24.925Z Reads: 137

```
Sure, here ya go.

100 Pcs GZFY 6x6x4.5mm Panel PCB Momentary Tactile Tact Push Button Switch 4 Pin DIP https://www.amazon.com/dp/B01N6GU7TA/ref=cm_sw_r_cp_apa_i_d5XzCbRX9H3ES
```

---
## \#1114 Posted by: janpom Posted at: 2019-02-15T20:47:14.413Z Reads: 132

```
Oh, it's these? I have a ton of them. :slight_smile: Thanks!
```

---
## \#1115 Posted by: ROFEN13 Posted at: 2019-02-15T22:04:54.071Z Reads: 140

```
I have the green dot!
Incase anyone is wondering, i didnt update to the new ACKMANIC firmware (3.xx, I was still 2.54). It will not work on the old firmware (I may have missed this if was already posted in the thread). I installed the new firmware on one vesc, and the DAVEGA connected. 
I just really didnt want to redo all my settings on the new software, but I guess I am now! The DAVEGA is worth it. I am excited to test it out!
```

---
## \#1116 Posted by: ROFEN13 Posted at: 2019-02-16T02:16:06.194Z Reads: 146

```
One more thing, sorry for clogging this up... hopefully it will help someone in the future....
My speed was off by a factor of 3 (I use mph)
3 mph on the DAVEga is really 9 mph
5 is really 15
8 is really 32
I verified this with gps. It was easy to do the calculations while riding but Im not sure what setting I messed up. I have 97mm wheels, 18t motor pulley,  36t wheel pulley, 7 pair poles
Can I just multiply a setting by 3 to get the correct speed and call it done? I will look through the code again tomorrow to see if there is a typo but wanted to out it out here as well.
```

---
## \#1117 Posted by: janpom Posted at: 2019-02-16T08:07:28.678Z Reads: 137

```
I bet everything is actually off by a factor of PI since you set the `WHEEL_CIRCUMFERENCE_MM` to the wheel diameter. Change the 97 to 305 and you should be good.
```

---
## \#1118 Posted by: banjaxxed Posted at: 2019-02-16T08:54:06.613Z Reads: 148

```
Meme time, kind of![image|638x479](upload://sGReLdTQ3NK4IHNUXXoeyHjh99K.jpeg)
```

---
## \#1119 Posted by: ROFEN13 Posted at: 2019-02-16T12:44:44.164Z Reads: 142

```
Haha that makes sense. Go me. Thanks so much for all this @janpom! You're my hero!
```

---
## \#1120 Posted by: ROFEN13 Posted at: 2019-02-16T12:48:21.891Z Reads: 138

```
Yep, I teach high school math and when I explain this to my students, I either get the look "huh? WTF? That isnt true" or "what a nerd"
I just wasnt paying attention when I input that number.
```

---
## \#1121 Posted by: banjaxxed Posted at: 2019-02-16T12:51:40.696Z Reads: 140

```
The irony is so rich, perfect to introduce the concept to students, next time they will listen if they can also enjoy the irony 😁
```

---
## \#1122 Posted by: janpom Posted at: 2019-02-18T22:03:50.536Z Reads: 144

```
v0.5 released: https://github.com/janpom/davega/releases/tag/v0.5
- configurable text screen
- new text screen items
  - MOSFET temperature
  - motor temperature
  - motor current
  - battery current
  - duty cycle
- configurable text screen font size
- total km (miles) displayed correctly when greater than 1000
- WHEEL_CIRCUMFERENCE_MM replaced with WHEEL_DIAMETER_MM
- SHOW_AVG_CELL_VOLTAGE is true by default
```

---
## \#1123 Posted by: janpom Posted at: 2019-02-18T22:14:58.564Z Reads: 135

```
Plans for future developments: 
- battery odometer (total Wh discharged; should be a good indicator of battery health)
- estimated range
- multiple text screens (there's already too many items to fit on one screen, especially with horizontal layout) 

Any other feature requests?
```

---
## \#1124 Posted by: venom121212 Posted at: 2019-02-18T22:19:55.744Z Reads: 133

```
Stopwatch feature would be cool if possible?
For clocking lap times or total ride time
```

---
## \#1125 Posted by: janpom Posted at: 2019-02-18T22:22:02.644Z Reads: 131

```
Ride time is already available. Lap times? Really?
```

---
## \#1126 Posted by: venom121212 Posted at: 2019-02-18T22:24:29.980Z Reads: 131

```
So by feature requests you meant only if you like them too? Got it thanks :neutral_face:
```

---
## \#1127 Posted by: janpom Posted at: 2019-02-18T22:29:15.882Z Reads: 130

```
No, sorry. :smiley: That wasn't meant to sound dismissive. I just don't understand it. I was trying to imagine how it would work. Considering your Dave is mounted at the tip of your board, completely out of your hands reach, would you seriously try to press a button to get a lap time?
```

---
## \#1128 Posted by: Jc06505n Posted at: 2019-02-18T23:14:31.182Z Reads: 135

```
Probably by just clicking start and then deducing the time taken to start (applicable for races) but not fully accurate. Maybe via detecting like metr does ?
```

---
## \#1129 Posted by: venom121212 Posted at: 2019-02-19T00:05:58.467Z Reads: 136

```
No hurt feelings :yum:
Yeah lap was a bad term to use. I have a big loop around my lake I like to ride and would like to generally time how long it takes (not concerned about stop and start time). Most people have it on their phone already though or their watch.

I'd love to get Davega synced into a remote somehow
```

---
## \#1130 Posted by: bsancken Posted at: 2019-02-19T00:11:11.353Z Reads: 141

```
[quote="venom121212, post:1129, topic:71509, full:true"]
I'd love to get Davega synced into a remote somehow
[/quote]
Since it was mentioned ~ If we want to add a remote connection into this too, I'll be needing someone to DIY up a CAN bus splitter or Multiplexer (has to be active from my understanding)! Need to connect bluetooth, remote, and the connection between the 2 vescs... Would love to be able to add in a lighting controller too :wink:
```

---
## \#1131 Posted by: lrdesigns Posted at: 2019-02-19T01:25:11.766Z Reads: 149

```
[quote="janpom, post:1122, topic:71509"]
v0.5 released:
[/quote]

Awesome! Time to update my davega. I still need to make a cable/adapter so I can program it externally and not take it out of the case. 

I've done 430 km's since installing the davega and loved every ride with it. :heart_eyes:

The data I most use is average voltage and speed. Since I ride 1p lipo I like to keep a really close eye on average voltage, the only thing that is little annoying is the font is a bit small to easily read while riding

![IMG_2419|666x500](upload://oXcbc3RLGELFR7hbb90sSyJ4gLq.jpeg) 

One other mild annoyance is the speed when its changing color, I can see the color of the number scan across left to right, which can be quite distracting. If you stay on the color change speed it can flicker quite a bit. It's like a colorful strobe. I don't think you can change that though? I think that is just how the LCD works?
```

---
## \#1132 Posted by: lrdesigns Posted at: 2019-02-19T01:33:03.440Z Reads: 149

```
[quote="janpom, post:1123, topic:71509"]
Any other feature requests?
[/quote]

Let me just say first that this request is just a nice to have and I don't think it should get any priority. 

It would be called something like "commuter mode" and would combine a trip counter with automatic trip reset on full charge, or 2x full charge if you charge both at home and work. 

Before the davega I used to do a trip counter manually with a marker on my battery enclosure. The reason is so I can calculate how many "trips" X "saved taxi money" so I can justify spending more money on eskate parts. :stuck_out_tongue_closed_eyes: Or help with wifey negotiations.  :thinking::rofl:

My previous trip counter. :wink:

![IMG_2429|666x500](upload://v9HbiIBVWq3UiumAWNeW41VyFHI.jpeg)

I have not updated my trip counter since getting the davega as I have distance traveled now, but I don't really have a trip counter anymore.

*Edit. Just updated to 0.5v and the text page is looking much nicer!! :+1::eyeglasses: 
Can I make a suggestion, put the numbers on the left side, then the text label on the right side. 
Also some instructions on how to customize the text page inputs, took me a bit of trial and error to figure it out. 

![IMG_2430|666x500](upload://twraUkfzhyXfWsyHXGU5pPxW99C.jpeg) 


There is one big feature request that I **REALLY** want and have been waiting for since the beginning. 
Max battery amps
Min battery amps
Max Motor amps
Min Motor amps

If davega gets this it pretty much does everything I would want it to do. 
:pray: :pray: :pray: :pray:
```

---
## \#1133 Posted by: janpom Posted at: 2019-02-19T08:34:21.774Z Reads: 142

```
[quote="lrdesigns, post:1131, topic:71509"]
I like to keep a really close eye on average voltage, the only thing that is little annoying is the font is a bit small to easily read while riding
[/quote]

I may have a solution for you. :wink:

![image|667x500](upload://eWt39STd8dXtyYT8HhDgcGthHs.jpeg)
```

---
## \#1134 Posted by: mishrasubhransu Posted at: 2019-02-19T09:06:04.967Z Reads: 142

```
:D
![image|690x164](upload://spCz4dpCmGKEOORqCY8nZ21dMw2.png)
```

---
## \#1135 Posted by: lrdesigns Posted at: 2019-02-19T09:32:45.962Z Reads: 137

```
Can I haz linky link? 
https://media.giphy.com/media/3oxHQfvDzo7VhSRy8M/giphy.gif
@janpom is this LCD going to work with current firmware?
```

---
## \#1136 Posted by: janpom Posted at: 2019-02-19T09:42:53.303Z Reads: 138

```
Here's the [link](https://www.aliexpress.com/item/2-8-240x320-SPI-TFT-LCD-Serial-Port-Module-With-PCB-Adapter-Micro-SD-ILI9341-5V/32889801161.html), but no, it won't work with Davega. I actually purchased it to experiment with micropython on ESP32 since there's no micropython library for the ILI9225 driver (used on the standard Davega display).

[This one](https://www.ebay.com/itm/2-2-TFT-LCD-Color-Display-Screen-Module-176x220-for-Ar-Mega2560-ILI9225-IC/113226293641) should work with Davega out of the box, but it's 2.2" so only 10% bigger than what we normally use.
```

---
## \#1137 Posted by: janpom Posted at: 2019-02-19T09:47:09.467Z Reads: 147

```
LOL. I made exactly the same purchase, only a few cents cheaper. ;)

![image|500x500](upload://nWGkgRXIimWi5QzchZuMYGzncdh.jpeg)
```

---
## \#1138 Posted by: mishrasubhransu Posted at: 2019-02-19T09:53:09.401Z Reads: 139

```
I was going to build DAVEga myself but thought a bigger screen would be better. Of course would have to modify the firmware. I already checked that there are Arduino libraries for ILI9341 chip.
```

---
## \#1139 Posted by: janpom Posted at: 2019-02-19T10:02:13.928Z Reads: 140

```
Sounds good. It shouldn't be that hard. For the most part, you'll need to add a custom implementation of the [`DavegaScreen`](https://github.com/janpom/davega/blob/master/davega_screen.h) interface. The only problem is that the `init()` method currently depends on the `TFT_22_ILI9225`, but that could be fixed with some code refactoring. I wanted to do that anyway since I'd like to support the small 128x32 OLED display for "Davega Mini". I'll try to prioritize this so that you can reuse as much code as possible. Contributing back to the Davega repo would then be much appreciated.
```

---
## \#1140 Posted by: mishrasubhransu Posted at: 2019-02-19T10:12:08.535Z Reads: 132

```
Sounds good. I'll make a pull request when done.
```

---
## \#1141 Posted by: amazingdave Posted at: 2019-02-19T10:26:42.640Z Reads: 137

```
Like the sound of the mini.....
```

---
## \#1142 Posted by: banjaxxed Posted at: 2019-02-19T13:10:56.136Z Reads: 142

```
Maxi v6 😄![image|690x388](upload://ub3vd5UqJebpcPheSGAIcVWuuUa.jpeg)
```

---
## \#1143 Posted by: janpom Posted at: 2019-02-19T22:33:45.466Z Reads: 143

```
@mishrasubhransu I have done the refactor. It's in the [display_refactor](https://github.com/janpom/davega/tree/display_refactor) branch.

As a quick exercise, I tried implementing a very basic screen for a SSD1306 based 128x32 OLED display. [Here's](https://github.com/janpom/davega/commit/5bf124cdb6d8572699983b6b5258442c78a6f7c2) the commit. It should give you a useful template for implementing the ILI9341 screen(s). I hope it makes sense. Ignore the changes in `davega_util`. Those shouldn't have been a part of this commit. Feel free to get back with any questions.

Here's some pics from testing:

![IMG_1672|690x465](upload://j5eXgG93xNw70ZjwkViKuNNVrUN.jpeg) 

Small HW hack (putting the NC pins to a good use) :wink:

![IMG_1673|665x499](upload://2p9jtSDkY3DWMwetdmDlMc0mjXn.jpeg)
```

---
## \#1144 Posted by: lrdesigns Posted at: 2019-02-20T01:28:28.167Z Reads: 140

```
Tested it last night, I think it's a big improvement over the previous version. :+1::sunglasses:

The instantaneous values are not very useful though, I can't read them while riding and are gone when I stop. Though they could be useful for bench testing / dyno testing / or if you mounted the davega in go kart or something like that where the screen is close to your face. 

The non - instantaneous values work good and provide useful information. It is cool to check on mosfet temp when I stop at an intersection. Capacity is quite nice to check at the end of a ride. 

![IMG_2438|666x500](upload://mcIdN2xRwzCRCnEoQWmcozyZwAt.jpeg)
```

---
## \#1145 Posted by: mishrasubhransu Posted at: 2019-02-20T01:30:15.984Z Reads: 140

```
I think an absolute ride max and a rolling max(max in 30 seconds or so) are valuable information. 

Remaining capacity is nice, nicer is an estimate of ride distance left based on the average Wh/km. The new VESC app does that.
```

---
## \#1146 Posted by: lrdesigns Posted at: 2019-02-20T06:26:24.090Z Reads: 141

```
I modified the labels and put the numbers on the left. :smile: I think its easier to read if the numbers are on left especially if your comparing two similar items, like motor amps and battery amps. 

![IMG_2448|634x500](upload://kO5d57vqNrDoI05ou6c7kZq1Ld.jpeg)
```

---
## \#1147 Posted by: janpom Posted at: 2019-02-20T08:02:32.850Z Reads: 145

```
I like that. I'm thinking that aligning all the numbers at the decimal point would improve readability. The labels could maybe be right aligned. Something like this:

```
  38.94 km/h   max speed
  17.43 km/h   avg speed
   0.14 A     motor amps
   0.00 A   battery amps
  43.70 V  min pack volt
   4.10 V    avg voltage
3961.00 mAh     capacity
  29.00 °C     VESC temp
NONE          fault code
```

or maybe labels on the left are actually better if everything is aligned nicely:

```
max speed      38.94 km/h 
avg speed      17.43 km/h   
motor amps      0.14 A     
battery amps    0.00 A   
min pack volt  43.70 V  
avg voltage     4.10 V    
capacity     3961.00 mAh     
VESC temp      29.00 °C     
fault code          NONE          
```
```

---
## \#1148 Posted by: lrdesigns Posted at: 2019-02-20T08:26:36.326Z Reads: 129

```
I'm more a fan of left side numbers but let's see what other think about it. Spacing will an issue in large font mode, will probably need more abbreviated labels.
```

---
## \#1149 Posted by: b264 Posted at: 2019-02-20T09:22:24.185Z Reads: 136

```
[quote="lrdesigns, post:1148, topic:71509"]
will probably need more abbreviated labels.
[/quote]

A lot of it is duplicative, so that should be really easy

km/h means "speed" so
`38.94 km/h :max speed` = `38.94 km/h :max`

A means Amperes so
`0.14 A :Motor amps` = `0.14 A :Motor`

V is a measure of voltage so
`43.70 V :min pack volt` = `43.70 V :min pack`
```

---
## \#1150 Posted by: Bbaldrickk Posted at: 2019-02-24T02:52:31.424Z Reads: 133

```
Hi ive built a screen using an arduino nano and a 2.2 inch screen that ive got connected to a flipsky 6.6 dual vesc. But im having a problem with connection the data led is flashing away on the nano so pretty sure there is a signal there screen is stuck on first screen with red flashing and buttons not working im running the latest stock vesc firmware .48 is this compatible or do i need to roll back to an older firmware.


Edit: I have about a meter of shielded usb cable to connect from vesc to nano could this be too long ?
```

---
## \#1151 Posted by: janpom Posted at: 2019-02-24T07:43:32.853Z Reads: 129

```
Hi, I don't believe it works with the latest VESC FW. Try downgrading to 3.40.
```

---
## \#1152 Posted by: Pimousse Posted at: 2019-02-24T07:54:55.228Z Reads: 129

```
I did the check for SmartRing : 3 FET temperatures have been added at tthe end of COMM_GET_VALUES.
Depending on your library, if end of packet is ignored, that could work.
(Did'nt test it though, I switched to COMM_GET_VALUES_SELECTIVE)
```

---
## \#1153 Posted by: janpom Posted at: 2019-02-24T08:27:55.213Z Reads: 135

```
The problem is that I do check the CRC and that's probably trimmed. So I suppose it doesn't work out of the box. The COMM_GET_VALUES_SELECTIVE sounds like the way to go.
```

---
## \#1154 Posted by: Pimousse Posted at: 2019-02-24T08:38:58.171Z Reads: 135

```
Is the CRC dependant of the payload content in your library ?
The one I used (forked from @solidgeek) don't care about the payload content as long as the calculated CRC matches the read one.

Need to give a try though.

COMM_GET_VALUES_SELECTIVE is really great and should avoid bringing big update each time.
COMM_GET_VALUES_SETUP(_SELECTIVE) may gain your interest for coulomb counting also ! :+1:
```

---
## \#1155 Posted by: janpom Posted at: 2019-02-24T10:00:07.155Z Reads: 131

```
[quote="Pimousse, post:1154, topic:71509"]
Is the CRC dependant of the payload content in your library ?
[/quote]

Hm, I can't see how a library has a choice in that. The CRC is computed from the payload so if you don't have the payload you can't compute the CRC. Am I missing something?
```

---
## \#1156 Posted by: janpom Posted at: 2019-02-24T10:02:43.894Z Reads: 129

```
[quote="Pimousse, post:1154, topic:71509"]
COMM_GET_VALUES_SETUP(_SELECTIVE) may gain your interest for coulomb counting also
[/quote]

I probably won't use it because of backwards compatibility (I don't want to implement features that would only work with the latest VESC FW), but it looks pretty neat. Thanks for pointing it out.
```

---
## \#1157 Posted by: Pimousse Posted at: 2019-02-24T10:35:02.405Z Reads: 136

```
Sorry, I wasn't clear enough.
I meant, the CRC computation doesn't care of the meaning of each byte of the payload. It computes it based on the values.

So once the CRC is checked and verified, the library pushes the payload to the parsing process.
During it, if you don't parse all the packet and ignore the end, there is no difference between FW3.40 and FW3.48. The only difference between both is some values added at the end of the payload.

Not sure I'm clear enough in my explanation.
Sorry for that.
```

---
## \#1158 Posted by: Bbaldrickk Posted at: 2019-02-24T13:09:15.314Z Reads: 128

```
Really wish i understood what you guys are talking about 🤯 as it sounds like you know how to get it running on .48 and id much rather stay on that than use the older firmware
```

---
## \#1159 Posted by: Wainecaplin Posted at: 2019-02-24T14:15:02.694Z Reads: 125

```
I really need this to run on .48 aswell because im running a 75 300 vesc i have to run that firmware  please help
```

---
## \#1160 Posted by: janpom Posted at: 2019-02-24T15:16:08.152Z Reads: 128

```
It will definitely be done. You just have to give me some time guys. I have a full time job and two kids. :slight_smile:
```

---
## \#1161 Posted by: janpom Posted at: 2019-02-24T15:23:23.537Z Reads: 131

```
Right, makes sense. The problem is that with Arduino you have the 64 bytes UART message limit and even with FW 3.40, the last byte of the response to GET_COMM_VALUES gets trimmed. That's not a problem though since that's the "message termination" byte and it's not at all important. However, with more bytes added to the payload more bytes at the end of the message will be trimmed, namely the CRC bytes. You should still be able to parse the message and maybe even compute the CRC. You just won't have anything to compare it to.
```

---
## \#1162 Posted by: Pimousse Posted at: 2019-02-24T18:45:05.221Z Reads: 131

```
With @Solidgeek 's library, Arduino can handle packets >63 bytes (by emptying the buffer while receiving data).

But anyway, old story now with COMM_GET_VALUES_SELECTIVE (unless you need a big amount of data, this command reply back also with the 32 bit mask after COMM_PACKET_ID, so only 53 useful bytes).
```

---
## \#1163 Posted by: janpom Posted at: 2019-02-24T19:12:08.146Z Reads: 138

```
[quote="Pimousse, post:1162, topic:71509"]
With @Solidgeek 's library, Arduino can handle packets &gt;63 bytes (by emptying the buffer while receiving data).
[/quote]

Ah, I looked at the code and also read up a little bit on the 64 bytes limit since I didn't understand the code at first. It's actually pretty straightforward. You just need to wait a bit for the data. Something like:

```
while (Serial.available())
  Serial.read()
```

will only read what's in the buffer. However, something like this will read all:

```
long start = millis();
int timeout = 100;
while (millis() - start < timeout) {
  if (Serial.available())
    Serial.read();
}
```

Good to know. Maybe an easier way for me to support the 3.48. Thanks!
```

---
## \#1164 Posted by: janpom Posted at: 2019-02-24T20:43:26.887Z Reads: 131

```
@Bbaldrickk @Wainecaplin I spent a little bit of time on the Dave FW today. [This version](https://github.com/janpom/davega/tree/64b_limit) might work with VESC 3.48. I haven't had time to test it with 3.48. I merely verified that it still works with 3.40. IMO there's a pretty good chance it will work with 3.48 though. :slight_smile: If you don't mind being guinea pigs, please give it a try. It definitely won't break anything. In the worst case it just won't work. One thing you could try in that case is going to `vesc_comm.h` and changing

```
#define PACKET_MAX_LENGTH 70
```

to a higher value than 70, say 80.
```

---
## \#1165 Posted by: Bbaldrickk Posted at: 2019-02-24T21:08:34.335Z Reads: 129

```
Wow thanks for the swift work will download and give it a go ill let you know how it goes. 😁
```

---
## \#1166 Posted by: solidgeek Posted at: 2019-02-24T21:46:50.157Z Reads: 130

```
Yeah it is pretty straight forward, just read the bytes as fast as they come and the buffer will never overflow :-) Nice project by the way :+1:
```

---
## \#1167 Posted by: Wainecaplin Posted at: 2019-02-24T21:49:59.021Z Reads: 134

```
Thankyou i will give it ago
```

---
## \#1168 Posted by: Bbaldrickk Posted at: 2019-02-24T22:51:52.151Z Reads: 137

```
Ok so ive had a go and still cant get a connection i have changed the setting to 80 aswell as you suggested with no luck and tripple checked my connections swapped tx and rx several times just incase with no joy 😞
```

---
## \#1169 Posted by: janpom Posted at: 2019-02-25T07:49:25.017Z Reads: 134

```
OK, thanks for testing. I'll try to find some time to do some testing/debugging myself this week.
```

---
## \#1170 Posted by: Wainecaplin Posted at: 2019-02-27T10:55:11.296Z Reads: 135

```
@janpom i also tried that aswell with no luck ill try anything you put to me no problem thankyou for your help could it be that i am using a mini arduino and not your circuit ?
```

---
## \#1171 Posted by: janpom Posted at: 2019-02-27T11:00:48.236Z Reads: 145

```
No, that's definitely not it. My circuit is basically a barebone Arduino as well. I suppose it's just that my latest FW update doesn't really fix things for VESC FW 3.48. I hope to find some time for it tonight. Thanks for the feedback.
```

---
## \#1172 Posted by: janpom Posted at: 2019-02-27T20:17:17.653Z Reads: 147

```
@Wainecaplin @Bbaldrickk  I have some good news, which however may actually be bad news for you. I just installed the 3.48 on my ESCapes and my Dave with the v0.5 that's permanently connected immediately stopped working (as expected). Then, however, I connected my other Dave with the FW from the [`64b_limit`](https://github.com/janpom/davega/tree/64b_limit) branch and that one just worked. So I'm afraid the problem must be something at your end.

Make sure your TX/RX wires are correctly connected and that you have your VESCs [correctly configured](https://github.com/janpom/davega/tree/64b_limit#configuring-the-esc). Fingers crossed. May you see the [green square](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/980?u=janpom) soon. :slight_smile:   

I'll soon release DAVEga v0.6, which will be VESC 3.48 compliant (while retaining compatibility with older VESC FWs).
```

---
## \#1173 Posted by: Wainecaplin Posted at: 2019-02-27T20:46:26.498Z Reads: 142

```
Thankyou i will givw it a try asap
```

---
## \#1174 Posted by: janpom Posted at: 2019-02-27T22:36:52.294Z Reads: 162

```
[DAVEga v0.6](https://github.com/janpom/davega/releases/tag/v0.6) is out.
```

---
## \#1175 Posted by: Bbaldrickk Posted at: 2019-02-28T09:53:47.816Z Reads: 168

```
Well it works 😁😁😁 not sure exactly what happened as all i done was re download last night flashed and it worked straight away. ![20190222_002615|243x500](upload://sB9Jh4zH4T4DjQySswzy6NPgiBf.jpeg)
```

---
## \#1176 Posted by: janpom Posted at: 2019-02-28T11:12:17.630Z Reads: 161

```
Nice! I like the color choice for your enclosure. And the buttons are cool as well. Are they printed?

The deck a trucks look familiar. ;)
```

---
## \#1177 Posted by: hiboute Posted at: 2019-02-28T11:23:37.706Z Reads: 164

```
Hello all,

I’ve just received my screens from aliexpress and tried to install the davega. 
But the screens keeps beeing white. Can someone please assist me? 
I’m on the 1.0 hardware received from janpom.
![image|375x500](upload://AqKFEFgFaj1YrXhBRWtmBoM58kY.jpeg) ![image|375x500](upload://AOLZjQOcWcNcbSBbiVe02XPosW.jpeg) ![image|375x500](upload://oX2F3Pih9vLpVybAU1ynJG9oN5N.jpeg) ![image|375x500](upload://jvmJGtN6BMoUDuV3aexwDbFbYVi.jpeg) ![image|375x500](upload://u18Uprvn5LMMosMk5MZwDCqOK3q.jpeg)
```

---
## \#1178 Posted by: Bbaldrickk Posted at: 2019-02-28T11:36:06.462Z Reads: 153

```
Yeh i hacked and slashed the irdesighn case to fit a 2.2inch screen and to suit my needs![20190222_000538|243x500](upload://ct7XyDW3m5GDJ5jKufbnDY1QZK9.jpeg)
```

---
## \#1179 Posted by: janpom Posted at: 2019-02-28T11:37:54.593Z Reads: 148

```
Hi, sorry, I got your message but haven't had time to respond yet. This is weird since I have tested all boards before shipping. Did the package look like it might have got some beating?

Have you tested if you can update the FW? If not, please try that first. If that works, it's probably a bad display. If it doesn't work, the board is probably broken and it's not worth debugging. I can just send you another one.
```

---
## \#1180 Posted by: janpom Posted at: 2019-02-28T11:40:00.018Z Reads: 146

```
Wow, that's neat! Would you share the stl files with us?
```

---
## \#1181 Posted by: hiboute Posted at: 2019-02-28T11:43:31.561Z Reads: 143

```
No the package was fine. 
I’ve ordered 3 display (one was broken), they all display white.

I did try to upload the firmware but still have the issue.
```

---
## \#1182 Posted by: janpom Posted at: 2019-02-28T11:44:07.108Z Reads: 136

```
Just to be clear: The FW upload was successful?
```

---
## \#1183 Posted by: hiboute Posted at: 2019-02-28T11:49:41.933Z Reads: 146

```
![image|666x500](upload://xMsWC7zqE1mKXEC1Q1TsYHXlam4.jpeg) 

Tryied again, i have this error now
```

---
## \#1184 Posted by: Mich21050 Posted at: 2019-02-28T11:51:10.304Z Reads: 144

```
Did you install the driver? Did you select the right com port/board? Did you solder/buy the parts yourself?
```

---
## \#1185 Posted by: janpom Posted at: 2019-02-28T11:57:10.778Z Reads: 146

```
When you tried installing the FW before, did it work without this error? Please double-check your Arduino IDE settings are correct as @Mich21050 suggests. https://github.com/janpom/davega#configuring-and-installing-firmware

If you can't get the FW updated, that's likely a bad board. I believe you have the DIY kit as well, right? Do you think you could try assembling that one and see if you can get it working? That way we would rule out there's a problem in the display or in the Arduino IDE setup.
```

---
## \#1186 Posted by: hiboute Posted at: 2019-02-28T12:22:33.403Z Reads: 141

```
Ok i will build the diy kit and keep you posted. Thank you
```

---
## \#1187 Posted by: Bbaldrickk Posted at: 2019-02-28T14:28:59.208Z Reads: 141

```
Yeh when I get some time ill put it up on thingiverse as a remix
```

---
## \#1188 Posted by: kalebludlow Posted at: 2019-02-28T22:14:53.419Z Reads: 140

```
Have tried uploading the sketch, but am getting the error 

'avrdude: ser_open(): can't open device "\\.\COM9": Access is denied.'

Any idea?
```

---
## \#1189 Posted by: Mich21050 Posted at: 2019-02-28T22:16:50.518Z Reads: 132

```
Are you sure you selected the right com port? Did you install the driver which is mentioned on @janpom 's github? You could try running Arduino Ide with administrative privileges.. :slight_smile:
```

---
## \#1190 Posted by: kalebludlow Posted at: 2019-02-28T22:24:39.205Z Reads: 130

```
Restarted PC and it worked without issue. Thank you for your help
```

---
## \#1191 Posted by: hiboute Posted at: 2019-02-28T22:36:32.010Z Reads: 131

```
so i finish soldering the diy kit. Same issue on both pcb.
I’ve installed ubuntu, and tryied to upload from there, same problem.

avrdude: stk500_recv(): programmer is not responding

I really don’t understand...
```

---
## \#1192 Posted by: janpom Posted at: 2019-02-28T23:06:00.656Z Reads: 135

```
Maybe try the other USB-UART adapter. Do you have any regular Arduino on hand?
```

---
## \#1193 Posted by: hiboute Posted at: 2019-02-28T23:12:59.234Z Reads: 142

```
I tried both.

No, but from i can read online, it is probably that there is no bootloader.

Possible?

If so, what do i need to install it?
```

---
## \#1194 Posted by: venom121212 Posted at: 2019-03-01T00:37:50.680Z Reads: 138

```
Finally got my DAVEga assembled and am setting up the config file.

With the Foxbox Unity:
`Vesc_Count = 1?`
`Motor_Pole_Pairs = ?'`
```

---
## \#1195 Posted by: b264 Posted at: 2019-03-01T04:49:26.378Z Reads: 140

```
Which motors do you have?
```

---
## \#1196 Posted by: janpom Posted at: 2019-03-01T10:04:22.355Z Reads: 141

```
[quote="hiboute, post:1193, topic:71509"]
No, but from i can read online, it is probably that there is no bootloader.
[/quote]

No way. The MCU on the board that I assembled definitely has a bootloader. I pre-installed the FW on all boards I have shipped. That wouldn't work without the bootloader.

I haven't verified if the MCUs on in the DIY kits do have the bootloader installed but all the MCUs came from the same batch and they all had bootloaders. So while I can't guarantee it has a bootloader I would be really surprised if it didn't.

You can burn a bootloader using an Arduino but since the MCU is already soldered on the board, it would be a bit of a hassle. As I said, though, I don't believe this is actually the problem.
```

---
## \#1197 Posted by: hiboute Posted at: 2019-03-01T10:25:44.557Z Reads: 133

```
Alright, so maybe an issue with CP2102 devices? i will try to remove and reinstall the driver.
```

---
## \#1198 Posted by: janpom Posted at: 2019-03-01T11:09:24.452Z Reads: 136

```
While trying to install the FW, do the RX/TX LEDs on the USB-UART adapter flash?
```

---
## \#1199 Posted by: janpom Posted at: 2019-03-01T11:13:47.096Z Reads: 137

```
I'm actually not even sure it will work correctly with the Unity. I will have to look into that. I currently don't have one to test with but I pre-ordered one and it was due to shipping in February, so hopefully I will get it soon.

Have you been able to get the green square with the Unity?
```

---
## \#1200 Posted by: hiboute Posted at: 2019-03-01T11:53:14.330Z Reads: 127

```
only one blink of the TXD at each try.
```

---
## \#1201 Posted by: janpom Posted at: 2019-03-01T11:59:07.749Z Reads: 120

```
That sounds like it's working correctly. One more idea. Try [this](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/1097?u=janpom).
```

---
## \#1202 Posted by: hiboute Posted at: 2019-03-01T12:01:26.318Z Reads: 124

```
1.6.23

10 char
```

---
## \#1203 Posted by: janpom Posted at: 2019-03-01T12:14:00.084Z Reads: 129

```
OK, good. Could you please send the full console output from the FW upload (you can leave out the initial compile part)?

Before you run the FW upload, please go to your Arduino IDE preferences and set the “Show verbose output during:” for both compilation and update.
```

---
## \#1204 Posted by: hiboute Posted at: 2019-03-01T12:28:50.521Z Reads: 145

```
avrdude: Version 6.3-20171130
         Copyright (c) 2000-2005 Brian Dean, http://www.bdmicro.com/
         Copyright (c) 2007-2014 Joerg Wunsch

         System wide configuration file is "C:\Program Files (x86)\Arduino\hardware\tools\avr/etc/avrdude.conf"

         Using Port                    : COM4
         Using Programmer              : arduino
         Overriding Baud Rate          : 115200
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 1 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 2 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 3 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 4 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 5 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 6 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 7 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 8 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 9 of 10: not in sync: resp=0xfc
avrdude: stk500_recv(): programmer is not responding
avrdude: stk500_getsync() attempt 10 of 10: not in sync: resp=0xfc

avrdude done.  Thank you.

Problème de téléversement vers la carte. Voir http://www.arduino.cc/en/Guide/Troubleshooting#upload pour suggestions.
```

---
## \#1205 Posted by: janpom Posted at: 2019-03-01T13:21:01.152Z Reads: 145

```
Thanks. I don't really have any other ideas. This looks as though the board is not working. I will just send you a replacement. I can also configure it for you in case you still had problems updating the FW. I'm currently waiting for supplies but they should arrive any day now.
```

---
## \#1206 Posted by: hiboute Posted at: 2019-03-01T14:13:50.007Z Reads: 148

```
Ok thank you. I have pm you.
```

---
## \#1207 Posted by: 702vegas Posted at: 2019-03-04T17:37:36.347Z Reads: 147

```
I had the white screen too. But i reinstalled the cp driver and reselected the com port and then it worked for me
```

---
## \#1208 Posted by: janpom Posted at: 2019-03-06T21:42:02.449Z Reads: 155

```
Here's how to save the day if you assemble a DAVEga before burning a bootloader on the MCU first. Note that **this should never happen to you if you have a kit from me** since all MCUs come with a bootloader.

I tried to do it today on a board that doesn't work. I thought that maybe the MCU doesn't have the bootloader since there wasn't any other apparent reason. It didn't work so the MCU is probably dead. I tried doing the same on a good board first to test that I'm doing it correctly and that did work.

So here's how to. Fortunately, the display headers connect to the right pins and we can leverage that.

1. Take an Arduino and upload the "Arduino ISP" to it (File > Examples > Arduino ISP > Arduino ISP). For Arduino UNO this should work out of the box. I used Arduino Pro Micro, for which I needed to slightly modify the code. I made it available [here](https://gist.github.com/janpom/9392cd185792685f6e3d20047587b0d2).

2. Connect the Arduino to the display headers as follows:
- 5V -> VCC
- GND -> GND
- on Arduino Pro Micro
  - pin 15 -> CLK
  - pin 14 -> RST
  - pin 16 -> SDA
- on Arduino UNO
  - pin 11 -> SDA
  - pin 12 -> RST
  - pin 13 -> CLK

3. Connect pin 10 (both UNO or Micro Pro) to the reset pin. Tthis one requires a hook clip or you can temporarily solder a jumper wire to the pin.

4. In the Arduino IDE, Tools:
- Board: "Arduino Nano"
- Processor: "ATmega328P"

5. Tools > Burn Bootlader

![IMG_1693|666x500](upload://eN8kwPF7TSSzOSRMJAHKZUQvoaM.jpeg) 

![IMG_1695|666x500](upload://mD5t9BsTzAiXu2deSpS70eafrfE.jpeg) 

![IMG_1694|666x500](upload://qmVeI800owVKZzOlLF330iwCDg1.jpeg)
```

---
## \#1209 Posted by: janpom Posted at: 2019-03-08T15:17:03.622Z Reads: 143

```
@hiboute I just received the package from you. I have some good news. The DAVEga that you have assembled does work. Only the display headers don't have a good contact. Maybe one of them was a bad piece or you put too much head on it while soldering and that has slightly deformed it. At any rate, I can easily fix that and ship it back to you.

The one that I have assembled is a bit of a mystery. I plugged it into the computer and tried uploading the FW to it. That worked just fine. After that I plugged in the display and at that point it stopped working. I can't even upload the FW on it anymore. The MCU seems completely dead now. Very strange. I'll send you a new piece.

I'll PM you about how you want the FW pre-configured. You clearly have some problem with your Arduino IDE setup and I don't know how to fix that.
```

---
## \#1210 Posted by: hiboute Posted at: 2019-03-08T15:34:17.453Z Reads: 137

```
Thank you for looking at it. 
I really appreciate it.
```

---
## \#1211 Posted by: pookybear Posted at: 2019-03-08T15:42:10.657Z Reads: 136

```
Are there any kits left?
```

---
## \#1212 Posted by: janpom Posted at: 2019-03-08T16:36:59.717Z Reads: 133

```
I should have more soon. I'm waiting for the supply of MCUs and it seems to be stuck at customs. :(
```

---
## \#1213 Posted by: pookybear Posted at: 2019-03-08T16:39:28.977Z Reads: 133

```
Thanks. I'll keep an eye out. Do I need to be on a list? Google form?
```

---
## \#1214 Posted by: janpom Posted at: 2019-03-08T23:14:22.416Z Reads: 139

```
Just PM me your name and address please.
```

---
## \#1215 Posted by: 702vegas Posted at: 2019-03-11T01:58:32.788Z Reads: 143

```
Made a simple case![20190310_185442|238x499](upload://kbhscxKRssHqOV6wf79ZWbIprI8.jpeg)
```

---
## \#1216 Posted by: lrdesigns Posted at: 2019-03-13T00:56:33.517Z Reads: 136

```
[quote="janpom, post:1123, topic:71509"]
Any other feature requests?
[/quote]

Just an idea, if the large speed number could be switched out for battery amps that would be really cool. As a firmware setting option would be ok, but what would make it super awesome if they could be switched with some button combination.
```

---
## \#1217 Posted by: janpom Posted at: 2019-03-13T06:48:41.615Z Reads: 132

```
It could be done as another screen layout. You could then toggle between them with the button 3. It's fairly straightforward. The question is if it fits in the flash memory. I'll give it a try.
```

---
## \#1218 Posted by: taz Posted at: 2019-03-13T15:02:25.095Z Reads: 135

```
[quote="Wainecaplin, post:1159, topic:71509"]
im running a 75 300 vesc
[/quote]

Are you running it on an esk8?
```

---
## \#1219 Posted by: Wainecaplin Posted at: 2019-03-13T15:18:17.483Z Reads: 138

```
On a goped but the trampaboards vesc was faulty so im hopfully getting a replacment soon
```

---
## \#1220 Posted by: janpom Posted at: 2019-03-13T21:37:57.361Z Reads: 143

```
[quote="lrdesigns, post:1216, topic:71509"]
if the large speed number could be switched out for battery amps that would be really cool
[/quote]

Here's a quick demo of what I have done: https://www.youtube.com/watch?v=cfFPBYKwKnQ

It works for the horizontal mode as well. You can select which display types you want in the config. Here's what I had for the demo. Comment out `...WITH_MOTOR_CURRENT_ENABLED` if you only care about battery amps.

```
// Screens. Uncomment the ones you want enabled.
//#define DEFAULT_SCREEN_ENABLED 1
//#define SIMPLE_HORIZONTAL_SCREEN_ENABLED 1
//#define SIMPLE_HORIZONTAL_SCREEN_WITH_BATTERY_CURRENT_ENABLED 1
//#define SIMPLE_HORIZONTAL_SCREEN_WITH_MOTOR_CURRENT_ENABLED 1
#define SIMPLE_VERTICAL_SCREEN_ENABLED 1
#define SIMPLE_VERTICAL_SCREEN_WITH_BATTERY_CURRENT_ENABLED 1
#define SIMPLE_VERTICAL_SCREEN_WITH_MOTOR_CURRENT_ENABLED 1
#define TEXT_SCREEN_ENABLED 1
```

I still only get data from one VESC. The battery current readings are multiplied by the `VESC_COUNT` config option. I don't multiply the motor current readings though. In other words, it shows the total battery current (approximately) and the connected motor current (which should be roughly the same as any other motor current). This seemed like the most intuitive way of doing it, but I don't feel strongly about it and I'm open to discussion.

We only have 2 digits for the value. While that's enough for speed (I don't expect many people to go over 100 kph), it may not be enough for current (I guess some people do make 100A+ occasionally). I didn't want to bother with adding the third digit, so there's color coding instead. Any value between 100-200 amps is displayed in yellow. Any value over 200 amps is displayed in red. The leading digit is trimmed.

For example, 125 amps would be displayed as 25 in yellow. 235 amps would be displayed as 35 in red. (335 amps is also displayed as 35 in red, so you can't distinguish that from 235, but I don't expect this to be a problem for anyone... except maybe @FullMetal_Machinist :laughing:). 

The code is in the [`display_current`](https://github.com/janpom/davega/tree/display_current) branch. 

Nice idea @lrdesigns. I'm definitely going to use this myself.
```

---
## \#1221 Posted by: FullMetal_Machinist Posted at: 2019-03-14T07:40:09.168Z Reads: 126

```
It is true that i do intend to run some 350 motor amps.
However this is per motor, on 4 motors combined it will be 1400 amps. You will run out of colors.
Two more digits please!
This is when more than one vesc are supported.
Battery total current limited to about 600 amps. 
Only meter i am interested in for now is ordinary voltage meter, keeping everything as simple as possible.
```

---
## \#1222 Posted by: lrdesigns Posted at: 2019-03-14T08:48:54.001Z Reads: 129

```
[quote="FullMetal_Machinist, post:1221, topic:71509"]
However this is per motor, on 4 motors combined it will be 1400 amps
[/quote]

:exploding_head:

@janpom the new screens with amps is really awesome!! And super quick development. Can't wait to try it.
```

---
## \#1223 Posted by: kalebludlow Posted at: 2019-03-19T22:28:09.523Z Reads: 123

```
Do any of the current enclosure designs take into account the extra thickness of the header on the screen? I tried the LRdesigns one and it wasn't thick enough so I hope there is one that will work
```

---
## \#1224 Posted by: janpom Posted at: 2019-03-19T22:42:31.989Z Reads: 123

```
Maybe you just need to trim the display header pins?
```

---
## \#1225 Posted by: lrdesigns Posted at: 2019-03-20T01:09:47.986Z Reads: 128

```
Which pins exactly could you point them out with an image? The pins on the top lcd side? My case has some room for them, but only if inserted the right way around, like try flipping the davega 180deg. 

If it really don't fit I would like to try and adjust my case design.
```

---
## \#1226 Posted by: kalebludlow Posted at: 2019-03-20T21:20:59.351Z Reads: 140

```
![IMG_20190321_081744|666x500](upload://pY3QDF7qT3J4hNeSoByX9ARKhOw.jpeg) 
![IMG_20190321_081753|666x500](upload://fQoCgJzoqWsNGSpRQXhJTVqbQ1c.jpeg) 
![IMG_20190321_081816|666x500](upload://ns82VVFwN13sIk3aGtqcHz8xSlI.jpeg) 

@janpom I have already trimmed down the pins a bit, but don't wanna go much further incase they lose contact in the header.

@lrdesigns The screen is oriented the correct way in the case. The issue could be a bad print as the case didn't really come up well. I'm still kinda new to printing so need to work on that more
```

---
## \#1227 Posted by: SeanHacker Posted at: 2019-03-20T21:27:43.454Z Reads: 137

```
I cut off this yellow plastic in order to get everything to fit right. 

![IMG_20190321_081816|690x213](upload://eICwXiG8rvoTliKYNfIqQwGYbW5.jpeg)
```

---
## \#1228 Posted by: kalebludlow Posted at: 2019-03-20T21:28:22.000Z Reads: 139

```
How exactly did you go about doing that?
```

---
## \#1229 Posted by: SeanHacker Posted at: 2019-03-20T21:29:13.344Z Reads: 138

```
Just a razorblade. You'll see that you can almost just pull it off with pliers. Just go slow and take your time. Start cutting at the base and you can kinda pry up at the same time.
```

---
## \#1230 Posted by: b264 Posted at: 2019-03-20T22:07:54.088Z Reads: 137

```
I don't have a Devega, but similar connectors are easy to pull the plastic off if you snip them with wire cutters first between the pins, then each individual one you can can pull off with hemostats.
```

---
## \#1231 Posted by: janpom Posted at: 2019-03-21T00:17:31.269Z Reads: 142

```
^ this. It's a bit of a hassle, but not really hard to do.
```

---
## \#1232 Posted by: lrdesigns Posted at: 2019-03-21T00:35:42.724Z Reads: 145

```
@kalebludlow I was talking about trimming the top side of the pins not the bottom. There is relief for them in the case but this may help the davega sit all the way in. 

![image|487x240](upload://vftrrXIQ1YsDJCzBcCXtprivdVG.jpeg)  

I see there is some shrinkage on the top of the case, it  could making the distance a bit shorter. Is this abs? If yes then I would switch to a less shrinky plastic like PLA. 

![image|690x267](upload://p1C8c4mKINJ9YCBr5NMPDQlzqkV.jpeg) 

My case was not designed for easy printing on a FDM printer. I think its very challenging on anything but a perfectly tuned FDM printer. Looking at @banjaxxed print above, that's pretty much the quality to aim for.
```

---
## \#1233 Posted by: 702vegas Posted at: 2019-03-26T18:04:12.174Z Reads: 136

```
Question. When connected to pc. I get everything on the davega screen. But connected to the board it powers on to a black screen. I did changed the baud and pwm uart. Am i missing something?
```

---
## \#1234 Posted by: janpom Posted at: 2019-03-26T18:46:31.907Z Reads: 136

```
Sounds like the 5V/GND wires are not correctly connected to the VESC.

The display goes all white when powered on. If it's all black it's likely not powered on. I recommend that you take a multimeter and do some measuring on the PCB between the 5V and GND rail.
```

---
## \#1235 Posted by: 702vegas Posted at: 2019-03-26T20:25:47.494Z Reads: 131

```
Will check. I just went of flipsky layout
```

---
## \#1236 Posted by: janpom Posted at: 2019-03-31T17:05:31.033Z Reads: 131

```
@hiboute I managed to fix your Dave! It had a bad crystal.

I was assembling some Daves today and one didn't work, which was really strange because I was pretty sure I have done everything correctly and I tested the MCU before the assembly. There's not that many components, so it wasn't that hard to find the bad one.

Then I thought what if your Dave had the same issue. Fortunately I didn't throw it to the bin, so I digged it out of my dead electro box and tried replacing the crystal there as well and voila, works like a charm. I can ship it to you if you have any use for it.

It looks like the batch of crystals I purchased had at least 2 bad pieces. I will have to test the crystals before including in the kits from now on.
```

---
## \#1237 Posted by: PickSix24 Posted at: 2019-03-31T17:11:20.594Z Reads: 130

```
@janpom is it possible to order one ?
```

---
## \#1238 Posted by: hiboute Posted at: 2019-03-31T17:18:50.593Z Reads: 131

```
Well, you already replace the oned i've sent you and they work great. Please give it to someone who would like to join the project!
```

---
## \#1239 Posted by: janpom Posted at: 2019-03-31T17:50:24.458Z Reads: 129

```
I could send to you the @hiboute's one and if you don't mind refurbished. :) It works just fine. Please PM me if you're interested.
```

---
## \#1240 Posted by: PickSix24 Posted at: 2019-03-31T18:22:44.055Z Reads: 134

```
Sounds good I’ll PM you
```

---
## \#1241 Posted by: venom121212 Posted at: 2019-04-01T01:07:46.044Z Reads: 132

```
Hey man, just checking if you've made any progress with unity integration. I want my davega working Sooo badly!
```

---
## \#1242 Posted by: janpom Posted at: 2019-04-01T05:21:54.780Z Reads: 132

```
I have one Unity on hand and I think I know what needs to be updated in the DAVEga FW. Now I just need to find some time to do it.
```

---
## \#1243 Posted by: SeanHacker Posted at: 2019-04-01T05:31:34.656Z Reads: 132

```
@janpom Are you always this cool? I swear I've told all my friends and family about you. You are the epitome of what open source is. Love it dude!
```

---
## \#1244 Posted by: janpom Posted at: 2019-04-01T05:54:27.569Z Reads: 135

```
Hehe, you guys exaggerate. It's really nothing. Compare to, say, how much time Vedder must have put into the VESC and you'll see how small the DAVEga is.
```

---
## \#1245 Posted by: b264 Posted at: 2019-04-01T05:56:01.221Z Reads: 131

```
People ***drastically*** underestimate the amount of time it took to write the VESC 2.18 firmware.
```

---
## \#1246 Posted by: MrMM Posted at: 2019-04-01T15:12:57.862Z Reads: 142

```
Just wanted to say thanks to @janpom for awesome idea and all your work!
I've uploaded code to arduino nano, using "current" branch. Seems to work with 2.2 screen, but I haven't had a chance to connect it to vesc yet. Should buttons work (to change screens) without vesc connected? I have them wired to pins A2, A3 and A4, of course I updated davega.ino with these pins before uploading it to arduino.
Is here someone less busy 😉 than janpom, who also knows programming well enough to make some little changes in what parameter is displayed on the screen with battery current? I'd be very happy, if someone could replace trip and total miles with mah used and motor temp. I don't need to see the speed or mileage at all, as in my case vesc is mounted on electric bike (with different gears being used, so the speed shown will never be true).
Thanks.
```

---
## \#1247 Posted by: janpom Posted at: 2019-04-01T17:25:48.871Z Reads: 138

```
Hi, thanks for the nice compliments. The buttons don't work until you connect to a VESC.

I'll send you some guidelines on how to customize the screens later.
```

---
## \#1248 Posted by: MrMM Posted at: 2019-04-01T17:50:18.590Z Reads: 159

```
Thank you, I'd really appreciate it. I've already connected DaVeGa to VESC and all worked first time 😁 My friend calls me cheater after we went for a ride today, for using my 2.8kW mid drive I've built from scratch on single track, but when I have shown him DaVeGa screen, he was speechless lol
```

---
## \#1249 Posted by: janpom Posted at: 2019-04-01T21:18:40.414Z Reads: 162

```
Alright, guys. It's time to teach you some fishing since I don't have enough fish for everyone.

Currently, there are 4 DAVEga screen layouts:

- default
  
![DSC01596|331x500](upload://fIbhJZXZuUdO4TbxfWrbeudiSXC.jpeg) 

- simple vertical

![IMG_1550|452x500](upload://x9gusHVEGYXTfxPbatqHQTEjcIu.jpeg) 

- simple horizontal

![IMG_1583|674x500](upload://8gVFPFNPItBvZGHclIsU3gRqMPC.jpeg) 

- text

![IMG_1596|635x500](upload://qhR6z13JjWTy0L5y12gCAdiSja9.jpeg) 

The layouts to be used can be configured [here](https://github.com/janpom/davega/blob/master/davega_config.h#L130) and then you can toggle between them with button 3. Normally you'll want to enable 2 layouts: the text and one of the graphical ones. It doesn't really make sense to enable more than 2 though you could.

The code is modular and each screen layout is one class:
- [davega_default_screen.cpp](https://github.com/janpom/davega/blob/master/davega_default_screen.cpp)
- [davega_simple_vertical_screen.cpp](https://github.com/janpom/davega/blob/master/davega_simple_vertical_screen.cpp)
- [davega_simple_horizontal_screen.cpp](https://github.com/janpom/davega/blob/master/davega_simple_horizontal_screen.cpp)
- [davega_text_screen.cpp](https://github.com/janpom/davega/blob/master/davega_text_screen.cpp)

You can customize existing layout by editing its class. (You can even add your own new layout. Just use any of the existing layouts as a template. This is not completely straightforward so I only recommend it to people with some coding experience.)

Now, let's have a look how to get basic things done. To display a value, you'll want to do two things:
1. create a label for it
2. display the actual value

Say that we want to modify the simple vertical screen such that it shows BATTERY AMPS instead of TRIP KM.

First, we'll go to the [`reset()`](https://github.com/janpom/davega/blob/master/davega_simple_vertical_screen.cpp#L27) method where the labels are drawn. We'll want to change the following line:

```
_tft->drawText(0, 130, _config->imperial_units ? "TRIP MI" : "TRIP KM", COLOR_WHITE);
```

to the following:

```
_tft->drawText(0, 130, "BATTERY AMPS", COLOR_WHITE);
```

By that we're simply saying to write the text `BATTERY AMPS` in white color at coordinates [0, 130]. In the original, the ternary expression may look scary:

```
_config->imperial_units ? "TRIP MI" : "TRIP KM"
```

This simply says: write `TRIP MI` if the `_config->imperial_units` flag is true; write `TRIP KM` otherwise.

Second, we'll go to the [`update()`](https://github.com/janpom/davega/blob/master/davega_simple_vertical_screen.cpp#L44) method where the values are displayed. The `reset()` is only called at the screen layout initialization whereas the `update()` is called periodically several times a second.

There we'll want to locate the following code, which displays the trip distance:

```
    // trip distance
    dtostrf(convert_distance(data->trip_km, _config->imperial_units), 5, 2, fmt);
    tft_util_draw_number(_tft, fmt, 0, 140, progress_to_color(data->session_reset_progress, _tft), COLOR_BLACK, 2, 6);
```

and change it to something like this:

```
    // battery amps
    dtostrf(data->battery_amps, 5, 1, fmt);
    tft_util_draw_number(_tft, fmt, 0, 140, COLOR_WHITE, COLOR_BLACK, 2, 6);
```

Now, let me explain what all of that means. The first line is just a comment. On the second line, we convert the float value `data->battery_amps` to a string value in `fmt`

```
    dtostrf(data->battery_amps, 5, 1, fmt);
```

The 5 is the total number of characters including the decimal point; the 1 is the number of decimal places. For example, the value of

`123.4466666666`

would be formatted as

`123.4`

That's 5 characters and 1 decimal point precision. If the value is less than 100, there will be leading spaces. For example:

`5.339999999999`

would be formatted as

`__5.3`

(two leading spaces). This ensures the value is right-aligned.

On the third line, we display the value stored in the `fmt` variable.

```
tft_util_draw_number(_tft, fmt, 0, 140, COLOR_WHITE, COLOR_BLACK, 2, 6);
```

The parameters are as follows:
- `_tft` - reference to the display instance (don't worry about it)
- `fmt` - the string to display
- `0` - x coordinate
- `140` - y coordinate
- `COLOR_WHITE` - text color
- `COLOR_BLACK` - background color
- `2` - number of pixels between characters
- `6` - font size

In the original code, instead of `COLOR_WHITE` for text color, there's the following expression:

```
progress_to_color(data->session_reset_progress, _tft)
```

This is to dim the text when the session data is about to be reset. As you press and hold the button 1, the `data->session_reset_progress` value will gradually increase from 0.0 to 1.0 and the `progress_to_color()` function translates the value into appropriate color (higher = darker). Once the `data->session_reset_progress` reaches the value of 1.0, the session data is reset and the value becomes completely black. You don't need to worry about this. It's just to explain what's going on.

The last thing you need to know is what values are available in the `data`. You'll find the list [here](https://github.com/janpom/davega/blob/master/davega_data.h#L42). For example:

```data->speed_kph```

will give you the current speed in km/h. Session data can be accessed using double dereference. For example, this is how to get the max speed in km/h:

```data->session->max_speed_kph```

The list of values available in the session is [here](https://github.com/janpom/davega/blob/master/davega_data.h#L25).

I hope this is helpful and I'm looking forward to seeing many customized screen layouts. :slight_smile:
```

---
## \#1250 Posted by: MrMM Posted at: 2019-04-02T00:42:37.960Z Reads: 140

```
Sir, you are a Legend! Thank you for that explanation. I've been going through every line of your code and I had basic understanding what relates to what. But as I haven't had a chance to learn even the basic of programming, I was pretty sure I will screw it up. Now it looks much clearer 😊
```

---
## \#1251 Posted by: PickSix24 Posted at: 2019-04-02T00:50:14.163Z Reads: 145

```
Can’t wait to get mine and set it all up !! @janpom how’s the unity support going ?
```

---
## \#1252 Posted by: janpom Posted at: 2019-04-03T20:00:27.809Z Reads: 149

```
@venom121212 @PickSix24 Here's a picture for you that you might like. :slight_smile:

 ![DSC01892|641x500](upload://d2hAbJwGp5tJd8M9pZKouiuXxV0.jpeg)
```

---
## \#1253 Posted by: janpom Posted at: 2019-04-03T20:26:14.881Z Reads: 147

```
Here's the [`unity_support`](https://github.com/janpom/davega/tree/unity_support) branch for the impatient ones. Note that the Dave FW has to be specifically compiled for the Unity. To enable that, you currently need to uncomment the [following line](https://github.com/janpom/davega/blob/unity_support/vesc_comm.h#L25). I'll try to make a config option for that instead before merging to master. It's unfortunately not completely trivial.

Also, you will want to set the `VESC_COUNT` config option to 1 with the Unity unless you actually have more than 1 (e.g. 2 for dual Unity for 4WD). There's a note in the config.
```

---
## \#1254 Posted by: venom121212 Posted at: 2019-04-05T18:14:53.196Z Reads: 141

```
Oh no! 404. 

Hopefully that means you're merging into the master :smiley:
```

---
## \#1255 Posted by: janpom Posted at: 2019-04-05T18:20:49.596Z Reads: 138

```
Already merged. I also moved enabling Unity to the config. You no longer need to touch any other files. (I spent 2 bloody hours getting that working. Totally not worth it. I hate C++.)
```

---
## \#1256 Posted by: venom121212 Posted at: 2019-04-05T18:46:49.694Z Reads: 139

```
You are the best! I can't wait to get this working
```

---
## \#1257 Posted by: venom121212 Posted at: 2019-04-05T19:12:02.455Z Reads: 140

```
I don't see an option for unity in the config tab. This is in the main v0.6 release found [here](https://github.com/janpom/davega/releases/tag/v0.6)?
```

---
## \#1258 Posted by: janpom Posted at: 2019-04-05T19:44:10.260Z Reads: 145

```
It's not yet released. You have to grab the master version. Will make a release soon. I'd like to do a few more changes and maybe finally call it v1.0.
```

---
## \#1259 Posted by: janpom Posted at: 2019-04-06T09:17:55.605Z Reads: 149

```
I have done some reformatting of the text screen following the suggestions from @lrdesigns and @b264. IMO it looks cleaner and is easier to read now. I hope you guys like it. (Never mind the motor temp. That's what you get if you don't have motor temperature sensor.)  

![IMG_1797|307x500](upload://dqx1JvDhCUvLHFuzCAWgNOUh3oY.jpeg)
```

---
## \#1260 Posted by: Romain Posted at: 2019-04-06T15:53:19.401Z Reads: 145

```
Hi

I am In South Africa and interested in your project. 
Still trying to figure out how to get a unit from you so please advise.

Would your display support the flipsky vescs?

Regards
```

---
## \#1261 Posted by: janpom Posted at: 2019-04-06T17:57:30.318Z Reads: 144

```
@Romain, see here: https://www.electric-skateboard.builders/t/davega-second-batch/82070

And yes, it will work with fipsky as well as any other VESC.
```

---
## \#1262 Posted by: jmasta Posted at: 2019-04-09T03:35:40.190Z Reads: 141

```
This is awesome
```

---
## \#1263 Posted by: gmurad Posted at: 2019-04-09T12:18:48.690Z Reads: 143

```
Tried search but couldn't find the answer. Did anyone find a faster shipping source for the LCD screen? DHL shipping to Canada is $30 from Aliexpress
```

---
## \#1264 Posted by: janpom Posted at: 2019-04-09T12:24:18.969Z Reads: 145

```
If I were you I would just order from AliExpress now with standard shipping. It normally arrives in less than a month (at least to Czech Republic) and I don't think you'll get the kit much faster anyway. You'll have hard time finding a faster source for the display without paying a lot extra.
```

---
## \#1265 Posted by: PickSix24 Posted at: 2019-04-09T12:48:24.229Z Reads: 141

```
Can’t beat this for speed 
https://www.amazon.com/gp/aw/d/B07HF7WVST?psc=1&ref=ppx_pop_mob_b_pd_title
```

---
## \#1266 Posted by: lrdesigns Posted at: 2019-04-09T12:54:07.076Z Reads: 145

```
![image|375x500](upload://mkY20XSq9pE2Nx7E0oInKRbdtRY.jpeg) 

![image|666x500](upload://d3HC6PEqKk1Teu2sLojRHa11uBu.jpeg) 

![image|375x500](upload://fVdBpjOl7KLxtNjVwB2hGaLuNX3.jpeg)

:heart_eyes:
```

---
## \#1268 Posted by: gmurad Posted at: 2019-04-09T12:54:56.880Z Reads: 139

```
Thank you! I ended up just getting from Aliexpress as I would also have to wait for the the parts from janpom and he said the time will more or less align. Good link to have in the thread for people in the US tho.
```

---
## \#1269 Posted by: PickSix24 Posted at: 2019-04-09T13:05:19.103Z Reads: 135

```
Quit teasing... 🤣🤣 i should have mine in a few days
```

---
## \#1270 Posted by: janpom Posted at: 2019-04-09T13:11:00.946Z Reads: 134

```
I'm actually surprised we're not seeing more Dave pics. I went over my records yesterday and I already shipped close to 100 kits. I should think of a bonus to ship with the 100th. :slight_smile:
```

---
## \#1271 Posted by: venom121212 Posted at: 2019-04-09T13:16:07.972Z Reads: 136

```
V1.0 FW and I'll have it working today :grin:
```

---
## \#1272 Posted by: MrMM Posted at: 2019-04-10T18:19:38.637Z Reads: 135

```
I've successfully 😄 changed screen layout, so it would show what's important for me on my ebike 😊 Thanks again for clear explanation 👍 I've made temporary housing, visible scratches are on polycarbonate piece on top of the screen. 
![20190410_191528|500x500](upload://ugw9yFcKOeGkHbIoDW3oN15SZ8G.jpeg)
```

---
## \#1273 Posted by: janpom Posted at: 2019-04-10T20:57:37.990Z Reads: 125

```
Looks good! I'm glad I didn't write the DAVEga coding crash course in vain.
```

---
## \#1274 Posted by: Andy87 Posted at: 2019-04-11T07:33:09.338Z Reads: 125

```
That’s amazing! Looks like a successful family business! You already took your children out of school to work 24/7 in the home production? 😜😜😜
```

---
## \#1275 Posted by: janpom Posted at: 2019-04-11T09:38:26.442Z Reads: 127

```
School? What do you mean? I merely shortened their shifts in the mines.
```

---
## \#1276 Posted by: Andy87 Posted at: 2019-04-11T09:48:06.669Z Reads: 126

```
But seriously. Good to see that this is going so well. Really a cool project and i‘m sure you made a lot of people happy with it. Me included 👍
```

---
## \#1277 Posted by: MrMM Posted at: 2019-04-11T13:48:12.156Z Reads: 128

```
My first one apparently was too easy to make, after all... This is much better. Now the biggest mystery to me is how to program another option, which is power output in Watts.. ![20190411_113535|281x500](upload://h1wgk3AzznNtBXF1RrwFxyTf8LH.jpeg)
```

---
## \#1278 Posted by: janpom Posted at: 2019-04-11T13:55:47.546Z Reads: 123

```
You're getting good at this! :slight_smile: If you're after the power drawn from the battery, that would simply be the amps * volts. I don't think you can currently get the watts for the motors from the VESC, only amps.
```

---
## \#1279 Posted by: MrMM Posted at: 2019-04-11T14:41:05.690Z Reads: 125

```
Thank you 🙂 Well, I'm confused with this... Rpm were not too difficult, as there's "get" message, which returns erpm (I think so). I've added "divide by 7" ( / 7) in two places to get rpm from erpm: in simple vertical screen, 
`dtostrf(data->rpm / 7`
and in text screen, added 
`SCR_RPM _write_numeric_line(data->rpm / 7`
But I have no idea what function should I use for power,
`float power = voltage * battery_amps; ` ?
And what to write in SCR_ line in text screen? And should I add float power in other files too? Like in the list in data.davega? Time to learn.... Lol
```

---
## \#1280 Posted by: janpom Posted at: 2019-04-11T15:15:34.039Z Reads: 122

```
`data->voltage * data->battery_amps`
```

---
## \#1281 Posted by: MrMM Posted at: 2019-04-11T15:44:40.861Z Reads: 131

```
Is it simple as that? 😅 So in `davega_simple_vertical_screen.cpp`
should I create label:
`_tft->drawText(x, y, "WATTS", COLOR_WHITE);`
and 
`dtostrf(data->voltage * data->battery_amps, 4, 0, fmt);
    tft_util_draw_number(_tft, fmt, x, y, COLOR_WHITE, COLOR_BLACK, 2, 6);`

But how to make it shown in text screen? Like that? 
`case SCR_WATTS:
                _write_numeric_line(data->voltage * data->battery_amps, "W", "power", i);
                break;`

And in `davega.screen.h`? 
`typedef enum {
	SCR_WATTS, `

In `davega.data.h`? 
`typedef struct {
	float watts; `

In `davega.config.h`? 
`#define TEXT_SCREEN_ITEMS { \
    SCR_WATTS, \ `

I apologise @janpom, I won't bother you again with my noob questions 😅🤯😳🤐
```

---
## \#1282 Posted by: janpom Posted at: 2019-04-11T17:24:04.703Z Reads: 133

```
That's all correct, except the `davega_data.h` edit would be redundant since you don't set or use the `data->watts` anywhere.

It would make sense if you set:
```
data.watts = data.voltage * data.battery_amps;
```
somewhere in the `loop()` function in `davega.ino` (before calling `scr->update()` but after setting both `data.voltage` and `data.battery_amps`).

Then you would be able to use `data->watts` instead of `data->voltage * data->battery_amps`.  It doesn't really have any advantage over using `data->voltage * data->battery_amps`, though. It's just an alternative way for achieving the same goal.
```

---
## \#1283 Posted by: janpom Posted at: 2019-04-11T18:26:02.054Z Reads: 130

```
[DAVEga v1.0](https://github.com/janpom/davega/releases/tag/v1.0) is out!
```

---
## \#1284 Posted by: venom121212 Posted at: 2019-04-11T18:32:24.494Z Reads: 134

```
https://giphy.com/gifs/dancing-adventure-time-bmo-pO4UHglOY2vII

Thank you!
```

---
## \#1285 Posted by: PickSix24 Posted at: 2019-04-11T21:48:29.592Z Reads: 132

```
Got mine today ! Gonna try and set everything up for unity tonight 

![image|375x500](upload://1EVenlbUwendD7OB5Sb7oJgftZV.jpeg)
```

---
## \#1286 Posted by: lrdesigns Posted at: 2019-04-12T00:27:25.940Z Reads: 132

```
[quote="janpom, post:1283, topic:71509"]
[DAVEga v1.0 ](https://github.com/janpom/davega/releases/tag/v1.0) is out!
[/quote]

Perfect timing! 

I was planning to update my settings today as I have changed gear ratio and wheel size. My speed has been wrong for 3 days. 

Thanks @janpom
```

---
## \#1287 Posted by: PickSix24 Posted at: 2019-04-12T02:16:36.823Z Reads: 129

```
I’m definitely not a code wiz.... hopefully I got these settings right lol. Gonna flash mine in a bit. Wish me luck !!
```

---
## \#1288 Posted by: SeanHacker Posted at: 2019-04-12T02:17:44.907Z Reads: 133

```
It's beautiful. Thanks dude!

![IMG_20190411_153619|666x500](upload://kvNyPMnksr2D5vQVvYrIE0QO4Qz.jpeg)
```

---
## \#1289 Posted by: lrdesigns Posted at: 2019-04-12T03:44:26.699Z Reads: 133

```
So awesome, now I have 4 screens to choose from!

![Davega%201|666x499](upload://nAIaQaD2PtJVbAYUzkXVpQ9PuXf.jpeg)
```

---
## \#1290 Posted by: PickSix24 Posted at: 2019-04-12T03:49:16.958Z Reads: 133

```
Got this error 
![image|374x500](upload://mpF2FqF6gEO6AbfC67Zn4xG4UJW.jpeg)
```

---
## \#1291 Posted by: SeanHacker Posted at: 2019-04-12T03:54:17.119Z Reads: 130

```
Look in you davega directory and make sure it's there. (the davega_config.h)

![Screenshot%20from%202019-04-11%2020-54-56|690x446](upload://AqibyKeiHebaf2SkPXAW3NTefdS.png)
```

---
## \#1292 Posted by: PickSix24 Posted at: 2019-04-12T04:06:02.872Z Reads: 132

```
Hmm still getting the error. Here’s what I got , saved in my Documents/Arduino 

![image|374x500](upload://4WuarcTKzDODgJ8CbjBRxO6LTwF.jpeg)
```

---
## \#1293 Posted by: PickSix24 Posted at: 2019-04-12T04:07:56.262Z Reads: 119

```
Think I figured it out. I wasn’t in sketchbook
```

---
## \#1294 Posted by: PickSix24 Posted at: 2019-04-12T04:14:40.706Z Reads: 130

```
![image|375x500](upload://VurM0cxPHhJohNPhamRv8dHrGs.jpeg)

First hurdle, got it programmed ! 
Now I have my buttons wired up, but they don’t seem to do anything. I couldn’t find an explanation of each button function. Do these need to be programmed?
```

---
## \#1295 Posted by: Mich21050 Posted at: 2019-04-12T04:53:46.059Z Reads: 129

```
The button's only work when the davega is connected to a vesc. \
@PickSix24
```

---
## \#1296 Posted by: PickSix24 Posted at: 2019-04-12T04:59:10.495Z Reads: 122

```
Awesome thanks !
```

---
## \#1297 Posted by: lrdesigns Posted at: 2019-04-12T07:41:17.998Z Reads: 131

```
@janpom I found a potential bug in 1.0. On the motor or battery amp screen when I go from full speed to hard break I get some random graphical errors. It does not happen on the speed screen or the text screen. Also if I cycle through the screens it goes away.  The error is very repeatable on the bench but less so on the ground. I need more road testing to see if it really is a big issue or not. Will let you know. 

![IMG_3204|666x500](upload://rmjX9fYNuoJBa5snOGs5mJy7zg.jpeg)
```

---
## \#1298 Posted by: janpom Posted at: 2019-04-12T07:48:29.561Z Reads: 127

```
I noticed something similar when testing. It happens very randomly and I haven't been able to consistently reproduce it. Also, I have only seen it happen when using all four screens. The only reason I can think of is that the MCU is low on memory. There's only 2 kB of RAM on the ATMEGA-328. Could you please try disabling at least one of the screens? That should free up some memory. Please let me know if that helps. Thank you.
```

---
## \#1299 Posted by: PickSix24 Posted at: 2019-04-13T07:02:52.616Z Reads: 124

```
![image|375x500](upload://m7OEl5JYM3D4bdQDRcywisrmAOh.jpeg) 

Got it working ! So awesome
```

---
## \#1300 Posted by: bsancken Posted at: 2019-04-13T07:09:58.540Z Reads: 130

```
Dual Vescs? for the 2 uart sources?
```

---
## \#1301 Posted by: PickSix24 Posted at: 2019-04-13T08:21:22.796Z Reads: 138

```
Nah , I’m Unity all the way
```

---
## \#1302 Posted by: janpom Posted at: 2019-04-13T10:25:21.398Z Reads: 149

```
_Edit: After writing it all down and taking all the pictures I realized that the 4P connectors are different from the batch I ordered earlier. The guidelines below assume the 4P connector looks as follows_ 

![IMG_1834|690x255](upload://d7wCoJAoYU9UEbJHnZ8euy4Bk3K.jpeg) 

_which is apparently not the case for some of the kits I distributed. So as a preparation step you will want to unpin the wires from the housing and plug them back so that it looks as on the picture above. Then on the pictures below, let's pretend this has already been done. :sweat_smile:_

_At the end of the day, the Dave has to be connected to the VESC as follows (5V-5V, GND-GND, RX-RX, TX-TX):_

![IMG_1835|366x500](upload://uwjCJvnNJ90V8spC6kZrLzriHFk.jpeg) 

_Sorry for the confusion! I will update the guidelines later._

... 

I realized that maybe it's not completely obvious how to get from here:

 ![IMG_1824|690x302](upload://hQMCZiNFsIBclyYNVfdBDmf2uzd.jpeg) 

to here:

![IMG_1829|690x166](upload://oMs3cL02AzITrgjCv0uZeSLmYrq.jpeg) 

so here's how to make the DAVEga-VESC cable. If you have crimping pliers and JST-PH crimps, that's ideal. I guess that most people don't though. No worries. You can do it just with a soldering iron as well.

First, you will want to unpin the wires from one of the 4P housings. I do it with a very small screwdriver. A needle should also work. You will want to lift the piece of the plastic that holds the crimp. Then you can unplug the wire.

![IMG_1825|690x275](upload://vks6klJcFyqbM53v0nYM2dDwWED.jpeg)

You can be rough with the housing since you won't need it. Be careful not to damage the crimps though. 

You will get four crimped wires.

![IMG_1826|690x348](upload://w1nd7oEvhPXvENajXElN3zTF0NX.jpeg)

Now, depending on your VESC type, you will want to take either the 7 pin or the 8 pin JST-PH housing (both come with the kit) and plug in the wires correctly. Check your VESC UART connector. The color mapping is as follows:

- red - 5V
- black - GND
- white - TX
- yellow - RX

Here's what it looks like for FOCBOX (and Unity). I believe this is the most common pinout.

![IMG_1827|690x459](upload://qgt89TDq39Aa4aJ8PBvnxAXLA9l.jpeg)

If you happen to have @stewii's ESCapes, you will want to have the wires plugged into the housing as follows (completely different from FOCBOX):

![IMG_1828|666x500](upload://sGTmaqL2qQF7osYwCpeBNdvj8zq.jpeg) 
 
Then you simply solder the 4P and 7P (or 8P) parts together (I didn't have white heatshrink :slightly_smiling_face: ):

![IMG_1829|690x166](upload://oMs3cL02AzITrgjCv0uZeSLmYrq.jpeg) 

Depending on where you want to install your Dave, this will likely be too short, so you will want to use an extension.

You can either use a 4 conductor cable:

![IMG_1830|666x500](upload://5ZWXEDDk1uIqKd2oWzimJpGYqNh.jpeg) 

or 4 individual wires. 26 AWG is ideal but anything in the 20-28 AWG range is usable. Here's what the end result should look like.

![IMG_1831|666x500](upload://6HZ58gt7aaFK2JTtLKO58J8k8e.jpeg) 

Also, you don't have to use the 4P connector but instead solder to the Dave PCB directly.

![IMG_1832|666x500](upload://mlWAXpsKw31CKJRzNS2vfNLqr1k.jpeg)

It doesn't matter whether you solder on the VESC port or on the USB-UART port. These are the same rails. You can actually easily see on the PCB how the pins are connected (RX=RXD, TX=TXD, etc). 

![IMG_1833|666x500](upload://g2QZU2psCrSZhjhtIBJvg0xQk7G.jpeg) 

So feel free to solder on the USB-UART if that's easier for you. It all comes down to what kind of enclosure you use and how you route your wires.

See also [here](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/726?u=janpom) for how to make a more advanced harness that can also be used for updating the FW.
```

---
## \#1303 Posted by: b264 Posted at: 2019-04-13T16:20:46.871Z Reads: 132

```
This post :arrow_up: should be linked directly from the github readme so you don't have to read 1295 posts to find it :-)
```

---
## \#1304 Posted by: janpom Posted at: 2019-04-13T16:50:18.183Z Reads: 135

```
![33|562x500](upload://vlBG37E7UwoA3qUM3Oqy4NvjE6B.png)
```

---
## \#1305 Posted by: hiboute Posted at: 2019-04-14T16:22:34.787Z Reads: 132

```
I had to revert back from 1.0 to 0.6.   i was gaining 1269 km at each startup of the Arduino.
```

---
## \#1306 Posted by: janpom Posted at: 2019-04-14T17:46:46.878Z Reads: 135

```
Can I have more details please? When you say "gaining", do you mean the odometer was at 1269 km after the first startup; at 2538 km after the second startup, etc? Is it the "total km" or the "trip km" or both?

Is anyone else seeing something similar with v1.0? It works fine for me and there haven't been any code changes since v0.6 that should affects this. Weird.
```

---
## \#1307 Posted by: MrMM Posted at: 2019-04-14T19:25:22.821Z Reads: 143

```
I hope it's not spamming... 😜 My final version 😁
![20190414_202040|405x500](upload://i9Dg4TADzxWXWd21QM6ceaM5HFu.jpeg)
```

---
## \#1308 Posted by: b264 Posted at: 2019-04-14T20:23:14.361Z Reads: 136

```
"MAH" is mega-amp-henries

"mAh" is milli-amp-hours
```

---
## \#1309 Posted by: hiboute Posted at: 2019-04-14T20:28:50.740Z Reads: 138

```
Sent you a video of the issue
```

---
## \#1310 Posted by: MrMM Posted at: 2019-04-14T20:44:16.550Z Reads: 138

```
Yes, you're right 😆 Actually I'm perfectly aware of it. Because the screen is so small and I squeezed 6 different values showing on this display, I decided to go full capital letters. Just my personal choice, I don't encourage anyone to do the same...
```

---
## \#1311 Posted by: bsancken Posted at: 2019-04-14T23:05:08.972Z Reads: 135

```
As long as you understand you own version lol Looks great!
```

---
## \#1312 Posted by: b264 Posted at: 2019-04-14T23:16:58.688Z Reads: 136

```
Science doesn't work that way.  It's either correct, or it's incorrect.
```

---
## \#1313 Posted by: MrMM Posted at: 2019-04-15T10:43:03.510Z Reads: 131

```
If you look at original layout on "default" screen, you'll see displayed capacity with capital MAH too 😄 Looks like no one complained about it earlier? 😉
```

---
## \#1314 Posted by: janpom Posted at: 2019-04-15T10:47:19.777Z Reads: 136

```
Actually, he did. :smile:

https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/83?u=janpom
```

---
## \#1315 Posted by: MrMM Posted at: 2019-04-15T10:49:31.742Z Reads: 135

```
Haha, anyway I'm not bothered, if it's about calculations, then indeed it is important. But on the display, when we all know what it shows anyway... 😜
```

---
## \#1316 Posted by: b264 Posted at: 2019-04-15T17:37:45.723Z Reads: 133

```
The people who lost billion dollar spacecraft weren't worried either about the "silly shit".  Science doesn't give a flying fuck what anyone thinks.  What's correct is correct, and what isn't, isn't.  Feelings are not taken into consideration.

Building an electric skateboard is being an engineer on the side.  Engineers use science.
```

---
## \#1317 Posted by: Mich21050 Posted at: 2019-04-15T17:42:47.856Z Reads: 137

```
But that's not the way science/electricity works. I just can't say this:
![15553500841624207278432480462397|281x500](upload://oLGW5o2Y2dGcuxWB6Pz4vhZ764F.jpeg) 

Is right just because I know there's one 0 missing so we all know that. It's to put it simply not correct.
```

---
## \#1318 Posted by: MrMM Posted at: 2019-04-15T18:03:12.615Z Reads: 135

```
Guys I think you've forgot something. This is about display, which only shows the numeric value. It could not have mAh or MAH at all, just "remaining" and it still would be fine. Because it could be showing "mAh", "MAH" or "cheeseburgers" it doesn't matter, as displayed value is not further processed in any way. And furthermore, it is not critical to show capacity left, considering that config consists of calculating it from VESC meter and battery voltage and it could be not 100% accurate everytime, as it depends or discharge profile and one could use Li-ion and one could use LiFePO4 etc.. You mainly need to see voltage of your battery if you don't rely only on LVC. I configured what to show where on the screen and it is for ME, not you or you. And I'm not making displayed value shorter by one or two digits! I'm not selling my display, I'm not sharing it with anyone and I'm the only one person who rides my mountain bike with custom, 3kW mid drive I built from scratch.
```

---
## \#1319 Posted by: b264 Posted at: 2019-04-15T18:07:48.992Z Reads: 131

```
You should never get a job as an engineer, because you will fail horribly.

Also you should read what I wrote.  I didn't forget anything.
```

---
## \#1320 Posted by: MrMM Posted at: 2019-04-15T18:17:02.310Z Reads: 129

```
I did, and I never aspired to be one. I admit that seeing someone getting frustrated over such a thing, which doesn't affect anyone else and is purely personal matter, is sometimes funnier than you think 👍 I never said I would do the same if I was distributing my layout to other people.
```

---
## \#1321 Posted by: b264 Posted at: 2019-04-15T18:20:33.435Z Reads: 128

```
I'm not frustrated, I'm rolling my eyes at you.  It's like when a teenager thinks they know more than you do, but clearly they are a huge dumbass to everyone, but only they can't see that.  You're the teenager here.

And you just can't stop showing everyone.
```

---
## \#1322 Posted by: MrMM Posted at: 2019-04-15T18:22:35.682Z Reads: 127

```
Just LOL, shall I also show you how I tie my shoelaces so you can tell me how to do it correctly?
```

---
## \#1323 Posted by: b264 Posted at: 2019-04-15T18:24:13.996Z Reads: 129

```
You're letting it leak out some more.

How you tie your shoelaces only affects you.  There are also multiple correct ways to tie them.

See, you're the teenager here.  We're rolling our eyes at you.
```

---
## \#1324 Posted by: yelnats8j Posted at: 2019-04-15T18:24:42.549Z Reads: 128

```
[quote="b264, post:1321, topic:71509"]
You’re the teenager here
[/quote]

At this point he is like a 10 year old. Cant learn how to stop arguing.
```

---
## \#1325 Posted by: MrMM Posted at: 2019-04-15T18:27:09.891Z Reads: 129

```
No, you still can't see that what I set on MY display only affects ME?
```

---
## \#1326 Posted by: b264 Posted at: 2019-04-15T18:28:35.123Z Reads: 130

```
It's leaking more.
```

---
## \#1327 Posted by: MrMM Posted at: 2019-04-15T18:31:16.849Z Reads: 148

```
Oh man, I feel sorry for you. Because your point of view is about being correct while using SI, my point of view from start is that my display can show whatever I want as it's totally personal thing which doesn't affect anyone, but me... Keep it going lmao
```

---
## \#1328 Posted by: Mich21050 Posted at: 2019-04-15T18:45:38.630Z Reads: 155

```
[quote="MrMM, post:1320, topic:71509"]
I did, and I never aspired to be one
[/quote]

The fucking stop acting like you are one.. jeez... @b264 just wanted to indicate that something is wrong on your display but instead of correcting or acknowledging it, you decided to be cocky nonetheless.\
And as I tried to point out earlier you can just go ahead and say it's just for personal use and because of that it's correct. Science doesn't work that way. Why do you think do we have SI units??
```

---
## \#1329 Posted by: lazarus Posted at: 2019-04-15T18:51:21.568Z Reads: 151

```
Wow you guys get really intense about your units. Anyone wanna port VESC to Ada or at least C++ so we can use safe unit types?
```

---
## \#1330 Posted by: MrMM Posted at: 2019-04-15T18:53:38.202Z Reads: 163

```
Yeah @Mich21050 and this was my reply, if you fucking didn't see it
[quote="MrMM, post:1310, topic:71509"]
Yes, you’re right :laughing: Actually I’m perfectly aware of it. Because the screen is so small and I squeezed 6 different values showing on this display, I decided to go full capital letters. Just my personal choice, I don’t encourage anyone to do the same…
[/quote]

[quote="Mich21050, post:1328, topic:71509"]
decided to be cocky
[/quote]
When after I acknowledged it, @b264 kept acting like "you have to fucking change it to mAh, no matter what". 
Your only advantage in this discussion is fact, that my English is not as fluent as yours.
```

---
## \#1331 Posted by: spei Posted at: 2019-04-15T19:00:44.064Z Reads: 155

```
Reading @MrMM and @b264 little 'argue' made me remember [this article](https://www.nytimes.com/1983/07/30/us/jet-s-fuel-ran-out-after-metric-conversion-errors.html) xD
```

---
## \#1332 Posted by: SeanHacker Posted at: 2019-04-15T19:02:09.798Z Reads: 173

```
On the same topic guys. I don't use MAH or mAH. I use penises because of... uh... science. Just let the man do what he wants with his display. No need to get hardcore about it. He even stated it's just his personal preference for his display.  

![IMG_20190411_153619|666x500](upload://tzoyruMiWdUn0b5wxxcLW2AYIN0.jpeg)
```

---
## \#1333 Posted by: janpom Posted at: 2019-04-15T19:04:30.084Z Reads: 268

```
@b264 @MrMM Guys, would you mind taking this argument to a different thread. Cheers.
```

---
## \#1334 Posted by: Riako Posted at: 2019-04-15T23:31:50.880Z Reads: 267

```
[quote="Riako, post:425, topic:88821"]
![Capturefsd|690x415](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/5/d/5d4ea60f346685ed46b95adc559097d5af6e8eec_2_690x415.jpeg)
[/quote]

You inspire compagny !!!
```

---
## \#1335 Posted by: brenternet Posted at: 2019-04-15T23:33:26.589Z Reads: 264

```
@janpom did they speak to you first?  

https://flipsky.net/collections/new-accessories/products/led-screen-module-base-on-davega-and-vesc
```

---
## \#1336 Posted by: mishrasubhransu Posted at: 2019-04-15T23:36:03.501Z Reads: 260

```
wow! that was crazy fast. So they are actively following what's going on here.
```

---
## \#1337 Posted by: SeanHacker Posted at: 2019-04-16T00:21:43.296Z Reads: 257

```
@janpom I think I said something along the lines about this kinda thing happening early on in this thread. I knew the affordable price, usability, and ease of use would be something that others would want. You killed it. ;)
```

---
## \#1338 Posted by: b264 Posted at: 2019-04-16T00:23:44.217Z Reads: 256

```
But there are no links to that?  What company?
```

---
## \#1339 Posted by: Riako Posted at: 2019-04-16T00:24:27.523Z Reads: 255

```
https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/1335?u=riako
 ^^ just under my post ;P it's Flipsky
```

---
## \#1340 Posted by: b264 Posted at: 2019-04-16T00:26:20.870Z Reads: 252

```
Is that @lrdesigns's design?
```

---
## \#1341 Posted by: venom121212 Posted at: 2019-04-16T00:29:24.718Z Reads: 249

```
It surely looks like it's one of the ones on thingiverse
```

---
## \#1342 Posted by: SeanHacker Posted at: 2019-04-16T00:30:38.572Z Reads: 248

```
https://flipsky.net/collections/new-accessories/products/led-screen-module-base-on-davega-and-vesc
```

---
## \#1343 Posted by: lrdesigns Posted at: 2019-04-16T00:31:46.410Z Reads: 246

```
They where even inspired by my case design. HAHA. 

@janpom I had some time to characterise the graphical error I have with brakes on the amp screens. 

- It only happens on the amp screens when using the brakes.
- Never during acceleration or speed screen or text screen. 
- It will happen at any brake level, ie slow as a turtle and soft brakes or hard with speed.
- The number of amps it shows always goes directly to 25amps. No other number will show. My vesc brake setting is only  -17 for battery and -45 for motor. 

You might be right that its a memory issue but why would it only be on the brakes on those screens? Seems weird. 

I will try with less than 4 screens when I get a chance might be a few days, my remote got stolen. :persevere:

- One other thing I think would be nice for the amp screens is that when pushing the brakes you get a different color on the amps, or at least a - symbol.
```

---
## \#1344 Posted by: SeanHacker Posted at: 2019-04-16T00:34:04.055Z Reads: 246

```
[quote="lrdesigns, post:1343, topic:71509"]
* t only happens on the amp screens when using the brakes.
* Never during acceleration or speed screen or text screen.
* It will happen at any brake level, ie slow as a turtle and soft brakes or hard with speed.
* The number of amps it shows always goes directly to 25amps. No over number will show. My vesc brake setting is only -17 for battery and -45 for motor.
[/quote]

Same here. I've been testing myself and see everything you mentioned. I've got it down to 2 screens and get the same results.
```

---
## \#1345 Posted by: gmurad Posted at: 2019-04-16T01:35:49.410Z Reads: 246

```
That’s a pretty fair price at $35 all assembled. Now if only they copy one of the diy remotes with telemetry...
```

---
## \#1346 Posted by: Tim231 Posted at: 2019-04-16T01:45:06.514Z Reads: 250

```
![image|230x500](upload://z9kII9dmgfklEoTVaqan3yoZL3c.jpeg) ![image|230x500](upload://r7S83XbYrBgfF9l9SKmH8EoSbOi.jpeg) 
Would I be able to splice the wires together from these two In the pictures and still get accurate readings from both I already have the Bluetooth module.
```

---
## \#1347 Posted by: bsancken Posted at: 2019-04-16T01:50:22.923Z Reads: 248

```
I wish that were how it worked! From my understanding that will not work reliably. I have been asking/hoping for someone to develop a UART multiplexer but so far nothing...

Please others correct me if I am wrong or if there is another way( other than multiple VESCs)
```

---
## \#1348 Posted by: Ricco Posted at: 2019-04-16T04:19:31.432Z Reads: 239

```
Ive actually started developing a UART Splitter based based on your request for one :stuck_out_tongue: It is definitely a much needed device. If all goes well with testing, you shouldnt have to wait too much longer for one :slight_smile:
```

---
## \#1349 Posted by: mackann Posted at: 2019-04-16T05:24:53.588Z Reads: 235

```
It was me who told them the idea. They where asking me for ideas on things they could make for eskate with low parts cost. But I didn't think they would just copy it. Haha we will se alot of fun things if they make all the things I told them that they could make 😁😂
```

---
## \#1350 Posted by: DEEIF Posted at: 2019-04-16T05:26:36.582Z Reads: 230

```
Now we wanna know what you told them to make😃
```

---
## \#1351 Posted by: b264 Posted at: 2019-04-16T05:29:01.123Z Reads: 233

```
[quote="DEEIF, post:1350, topic:71509, full:true"]
Now we wanna &ZeroWidthSpace;know what you told them to make😃
[/quote]

:arrow_up:&ZeroWidthSpace;

We need a "Flipsky copies..." thread
```

---
## \#1352 Posted by: Andy87 Posted at: 2019-04-16T05:32:06.659Z Reads: 232

```
I hope you also told them to honor the guy who made all the work...
```

---
## \#1353 Posted by: mackann Posted at: 2019-04-16T05:37:14.802Z Reads: 231

```
I told them: this open source project you could make something simular, it will probely be popular if it comes pre assembly. But please design it by yourself and if you use any others work i suggest you honor or pay them.
```

---
## \#1354 Posted by: b264 Posted at: 2019-04-16T05:50:02.402Z Reads: 230

```
[quote="mackann, post:1353, topic:71509"]
But please design it by yourself and if you use any others work i suggest you honor or pay them.
[/quote]

To a Chinese company, this translates as

[quote]
Steal this and do nothing for the original author
[/quote]

...because their intellectual property laws are so world-class over there.
```

---
## \#1355 Posted by: banjaxxed Posted at: 2019-04-16T06:23:46.784Z Reads: 227

```
How much cash do you think they put Vedder’s way each month? 

I think Jan could get just as much 😉
```

---
## \#1356 Posted by: lrdesigns Posted at: 2019-04-16T06:48:23.745Z Reads: 224

```
[quote="SeanHacker, post:1344, topic:71509"]
I’ve got it down to 2 screens and get the same results.
[/quote]

Which two screens?
```

---
## \#1357 Posted by: mackann Posted at: 2019-04-16T06:48:47.977Z Reads: 227

```
Well at least they did name it after him and did give a url to the github
```

---
## \#1358 Posted by: b264 Posted at: 2019-04-16T06:50:56.965Z Reads: 231

```
Here comes @janpom

![Screenshot%20from%202019-04-16%2001-49-51|113x39](upload://ovU2IbN4XMhU1n2ZrqaC9HDcCk3.png)
```

---
## \#1359 Posted by: janpom Posted at: 2019-04-16T06:58:53.229Z Reads: 236

```
Achievement unlocked! Getting copied by a Chinese company. :laughing:

@mmaner must be mad they didn't choose his enclosure design over @lrdesigns. :slight_smile:

Well, the FW is open source. It's perfectly legit that they use it and sell it as long as they keep any code updates open source... which they actually have to, not just for legal reasons, but mainly for technical reasons. People need the source code to be able to configure the device. I wonder if we'll see any new features or bug fixes from Flipsky.

This is also great timing since I just ran out of parts for making more kits and I wasn't even sure if I wanted to make more. I made over 100 by now and it's not that much fun anymore. I think I've been making like $2/hour on this (not including the FW development time) so it's not really like Flipsky is putting me out of business. :laughing: In fact, it's great that somebody will keep distributing the HW. 

The only thing that makes me mad is the way they executed this.

First, the way they have done it is pretty lame. There's misleading info in the item description, e.g. the 5c about pressing the button 3. That's just plain wrong. They also link an old version of the code and they link the source code rather than the release file. Last but not least, the cable seems too short. It will likely require an extension on most boards.

Second, they didn't talk to me or Luke about what they are about to do. At the very least, it would have been polite. "Guys, we'd like to make a product based on your open source design. Is that OK? Any comments or suggestions?" I'd happily give them my blessing and even spend some time making sure they don't screw it up...

Anyway, time to make progress the new DAVEga+. :slight_smile: 

![IMG_1837|666x500](upload://pqxycZQSFuJptofMDsSH9m5TuHY.jpeg)
```

---
## \#1360 Posted by: janpom Posted at: 2019-04-16T07:01:54.910Z Reads: 230

```
@lrdesigns This is great info. That will likely be an underflow bug in handling the amp values. I think I don't account for a negative value there, which is of course a problem when breaking. It should be an easy fix. I'll try to look at it toning.

... or, shall we file a bug report at Flipsky? :wink:
```

---
## \#1361 Posted by: bsancken Posted at: 2019-04-16T07:10:45.586Z Reads: 228

```
[quote="Ricco, post:1348, topic:71509, full:true"]
Ive actually started developing a UART Splitter based based on your request for one :stuck_out_tongue: It is definitely a much needed device. If all goes well with testing, you shouldnt have to wait too much longer for one :slight_smile:
[/quote]
I will definitely be interested in testing(and/or assembling!)!! I can even make this relevant to this thread by saying this could be used for a "DAVEga-dashboard" or even larger DAVEga+ cluster up front! ;)
```

---
## \#1362 Posted by: janpom Posted at: 2019-04-16T07:17:07.600Z Reads: 224

```
The DAVEga+ will be using the ESP32 MCU, which has built-in bluetooth. One of the features I have in mind is to do it such that it show the telemetry on the display but it also relays it over BT so that a mobile app can retrieve it.
```

---
## \#1363 Posted by: Okami Posted at: 2019-04-16T07:17:53.410Z Reads: 224

```
@janpom mh bigger display is nice. How much modification to pcb parts, if any would be needed?

I guess code also changes a bit due to different display / size or it stays the same mostly? (Other than pixel size - letter size, i guess)

Ok got the answer, i guess :D esp module would be way different level
```

---
## \#1364 Posted by: janpom Posted at: 2019-04-16T07:23:02.606Z Reads: 218

```
It's a completely different design. I'm doing it on ESP32 and in Micropython. I'm basically starting. It will take a few months until I have something to show. I have a lot of ideas and very excited about the project. I wish I had more time for it. I hope this will go quickly though since I'm much more efficient in Python than in C++.
```

---
## \#1365 Posted by: b264 Posted at: 2019-04-16T07:29:31.048Z Reads: 217

```
[quote="janpom, post:1360, topic:71509"]
or, shall we file a bug report at Flipsky?
[/quote]

LoLz :rofl:

They can't innovate; they produce carbon copies.
```

---
## \#1366 Posted by: Andy87 Posted at: 2019-04-16T07:33:30.828Z Reads: 210

```
somebody else told Flipsky what they could do and they just made that. That tells me that they have absolutely no idea what they are producing.
```

---
## \#1367 Posted by: SeanHacker Posted at: 2019-04-16T10:29:40.541Z Reads: 206

```
[quote="lrdesigns, post:1356, topic:71509"]
Which two screens?
[/quote]

Speed and Battery amps.
```

---
## \#1368 Posted by: SeanHacker Posted at: 2019-04-16T10:42:11.368Z Reads: 209

```
[quote="mackann, post:1349, topic:71509"]
It was me who told them the idea.
[/quote]

Bummer. It's too bad you chose to tell a company that produces complete dogshit parts. I can't think of one product that they make that is worth using with the exception of the DAVEga now. Haha
```

---
## \#1369 Posted by: janpom Posted at: 2019-04-16T10:44:45.764Z Reads: 206

```
[quote="SeanHacker, post:1368, topic:71509"]
with the exception of the DAVEga
[/quote]

That's yet to be seen. I'm tempted to order one to see what they have done. :smile:
```

---
## \#1370 Posted by: b264 Posted at: 2019-04-16T10:54:55.471Z Reads: 203

```
You should be getting one free, that's a fucking fact.
```

---
## \#1371 Posted by: SeanHacker Posted at: 2019-04-16T10:57:08.873Z Reads: 203

```
[quote="janpom, post:1369, topic:71509"]
I’m tempted to order one
[/quote]

Haha. Don't waste your $$$. With their track history it'll probably just break or not work properly.
```

---
## \#1372 Posted by: mmaner Posted at: 2019-04-16T11:58:54.928Z Reads: 203

```
[quote="janpom, post:1359, topic:71509"]
@mmaner must be mad they didn’t choose his enclosure design over @lrdesigns. :slight_smile:
[/quote]

Naw, I'm good. His easier to print and assemble. It must feel good to see your creation picked up for manufacturing though. Gratz
```

---
## \#1373 Posted by: janpom Posted at: 2019-04-16T12:13:16.702Z Reads: 211

```
I actually like yours. It works better for my boards since they both have the deck tips tilted and I don't need more tilting added by the enclosure. I also prefer the vertical layout. If Flipsky asked me, I would have advised them to offer both options... and make the cable longer... and provide correct product description. Those guys... I first felt rather optimistic about them getting the HW part right since it's so simple that it's really hard to mess up but now that I see how they managed to mess up even the simplest things I'm really not so sure anymore. Is anyone ordering one for science?
```

---
## \#1374 Posted by: Andy87 Posted at: 2019-04-16T12:45:24.463Z Reads: 212

```
[quote="janpom, post:1373, topic:71509"]
Is anyone ordering one for science?
[/quote]

maybe our flipsky incognito agent mr. @mackann can organize something for you for free???:thinking:

@janpom what your children now going to do without job? they need to go back to school? what a bummer....
```

---
## \#1375 Posted by: mackann Posted at: 2019-04-16T12:53:49.634Z Reads: 206

```
Haha I have nothing togheter with them, they just asked me about some nice product tips and I told them a few. Its not like it was a secret this topic. But yes I agree they should send you one for free atleast
```

---
## \#1376 Posted by: Andy87 Posted at: 2019-04-16T12:55:43.227Z Reads: 207

```
i meant more or less, maybe you have some connections or closer contact with people at flipsky than we have and could bring that topic up.
```

---
## \#1377 Posted by: briman05 Posted at: 2019-04-16T13:02:11.681Z Reads: 209

```
What you should do is buy one of flipsky's check it out and see if it has all the bug which it probably does cause it is linking the older files.  And then say hey you copied my idea and it would be nice to atleast mention me  for all my work but I found these bugs.  And let them figure them it out.  I think with the 4.20 modifications they are sending some to the guys who found the cut out problem for testing.  Maybe they can do the same for you.
```

---
## \#1378 Posted by: mackann Posted at: 2019-04-16T13:10:29.997Z Reads: 207

```
I did, but she told me a few days ago she quit the job
```

---
## \#1379 Posted by: janpom Posted at: 2019-04-16T14:56:00.109Z Reads: 203

```
[quote="Andy87, post:1374, topic:71509"]
@janpom what your children now going to do without job? they need to go back to school? what a bummer…
[/quote]

I guess I'll need to extend their temporarily shortened mine shifts back to 19 hours. :thinking:
```

---
## \#1380 Posted by: linsus Posted at: 2019-04-16T15:00:25.240Z Reads: 199

```
Null, 10 char
```

---
## \#1381 Posted by: janpom Posted at: 2019-04-16T21:04:50.444Z Reads: 206

```
@lrdesigns @SeanHacker This is fixed now: https://github.com/janpom/davega/releases/tag/v1.0.1

The problem was that I used unsigned integer for battery/motor amps so a small negative value would be interpreted as a high positive value (e.g. -1 => 255) and the third digit is unaccounted for. It would be written over the numbers on the screen right hand side. That's the "distortions".

I don't have space for a negative sign, so there's colour coding (again). Values below zero are displayed in red, e.g. red 10 = -10. Values above 100 are yellow and above 200 are purple. For example, yellow 55 = 155, purple 99 = 299. Whoever gets amp values below -99 or above 299, they need to wait for Flipsky to fix this for their "LED Screen Module base" in a better way. ;)
```

---
## \#1382 Posted by: SeanHacker Posted at: 2019-04-16T21:22:29.857Z Reads: 207

```
[quote="janpom, post:1381, topic:71509"]
This is fixed now
[/quote]

I love you!

I'll be able to test when I get back home tonight. Thanks dude!
```

---
## \#1383 Posted by: SeanHacker Posted at: 2019-04-17T21:17:43.025Z Reads: 191

```
Nice job on the update dude!!!
```

---
## \#1384 Posted by: janpom Posted at: 2019-04-17T21:33:06.682Z Reads: 193

```
Thanks! This should be a mandatory update for everyone.
```

---
## \#1385 Posted by: SeanHacker Posted at: 2019-04-17T22:35:03.916Z Reads: 196

```
Haha. It actually got me for a second.
```

---
## \#1386 Posted by: venom121212 Posted at: 2019-04-18T01:52:28.180Z Reads: 193

```
That... Is so great
https://giphy.com/gifs/cartoonhangover-animated-artists-on-tumblr-illustration-ToMjGpyO2OVfPLpoxu8
```

---
## \#1387 Posted by: lrdesigns Posted at: 2019-04-18T02:03:03.784Z Reads: 190

```
Thanks so much for the quick fixes and cool additions to the firmware!
```

---
## \#1388 Posted by: SeanHacker Posted at: 2019-04-18T02:15:03.189Z Reads: 189

```
[quote="lrdesigns, post:1387, topic:71509"]
@SeanHacker ruined the surprise. :expressionless:
[/quote]

Story of my life... :sob:
```

---
## \#1389 Posted by: janpom Posted at: 2019-04-18T06:14:52.358Z Reads: 181

```
The v1.0.1 has the important motor/battery amps bug fix. I highly recommend that everyone installs this version!
```

---
## \#1390 Posted by: Andy87 Posted at: 2019-04-18T06:19:33.148Z Reads: 182

```
that´s great!
Just imagine the Flipsky engineers uploading this for the first time :joy::joy::joy:
```

---
## \#1391 Posted by: b264 Posted at: 2019-04-18T06:24:21.001Z Reads: 188

```
They're screwed because they don't have any Software Engineers, only Photocopy Engineers.  They probably cannot fix this.
```

---
## \#1392 Posted by: Andy87 Posted at: 2019-04-18T06:27:07.842Z Reads: 175

```
Maybe to add something like "Flipsky, send nu*es!!!" in the end @janpom :smirk::joy:
```

---
## \#1393 Posted by: janpom Posted at: 2019-04-18T06:44:14.565Z Reads: 176

```
I'm sure Flipsky DAVEga will be a great success. They didn't even make a typo in the product title. Oh wait.
```

---
## \#1394 Posted by: lrdesigns Posted at: 2019-04-18T06:46:33.897Z Reads: 176

```
Delete all spoilers till after easter!
```

---
## \#1395 Posted by: janpom Posted at: 2019-04-18T06:49:15.989Z Reads: 183

```
@mmaner Is it possible to temporarily hide (or move to another secret thread) everything from Sean's post [here](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/1383?u=janpom)?
```

---
## \#1396 Posted by: venom121212 Posted at: 2019-04-18T11:51:55.188Z Reads: 193

```
@Andy87
https://giphy.com/gifs/meme-adventure-time-jake-the-dog-wVt0wS52vBagM

 I love my davega!

I can't wait to install it. I've been busy riding and spring time choring to get it physically installed. 

https://giphy.com/gifs/adventure-time-work-jake-the-dog-Ebys71phzQQx2

Today shall be the day!
```

---
## \#1397 Posted by: mmaner Posted at: 2019-04-18T12:43:04.497Z Reads: 183

```
Not temporarily, the individual post will have yo go to a new thread or an existing thread.
```

---
## \#1398 Posted by: Andy87 Posted at: 2019-04-18T12:48:49.941Z Reads: 171

```
we can flaaaag it aaaall away :rofl:
```

---
## \#1399 Posted by: Arzamenable Posted at: 2019-04-18T18:19:16.834Z Reads: 173

```
I ordered one yesterday for science. Will report in with pics.
```

---
## \#1400 Posted by: SeanHacker Posted at: 2019-04-18T19:26:59.753Z Reads: 170

```
What post? ;)
```

---
## \#1401 Posted by: janpom Posted at: 2019-04-18T19:35:08.680Z Reads: 170

```
Hehe, OK, I'm following in your footsteps. ;)

I feel like Winston Smith. :smile:
```

---
## \#1402 Posted by: janpom Posted at: 2019-04-18T20:06:51.574Z Reads: 165

```
@lrdesigns Your turn now. ;)
```

---
## \#1403 Posted by: Scream Posted at: 2019-04-19T05:12:28.134Z Reads: 163

```
I ordered one before I read this discussion. Assumed there was some sort of collaboration. Honestly flipsky is probably the easiest way for me to get the various components in NZ.

Not even sure how I’m gonna mount it on my tiny board. Might have to save it for my next build.
```

---
## \#1404 Posted by: bsancken Posted at: 2019-04-19T05:23:56.461Z Reads: 166

```
Wrist mounted DAVEga?? lol Solution for those who don't have room on their board! ;)
```

---
## \#1405 Posted by: janpom Posted at: 2019-04-19T07:35:59.625Z Reads: 170

```
That's all good. If you could then send us some pics of the internals that would be great. I'm very curious how they have done it. If it's just Arduino Nano inside or they have created something custom. I bet it's the Nano since they don't mention the USB-UART anywhere so they probably rely on the MicroUSB on the Nano for FW update/customization.

BTW, don't forget to upgrade to the latest firmware! :slight_smile:
```

---
## \#1406 Posted by: Scream Posted at: 2019-04-19T08:06:39.615Z Reads: 171

```
Will do. Thanks!
```

---
## \#1407 Posted by: 702vegas Posted at: 2019-04-20T02:56:21.833Z Reads: 173

```
got mine to turn on. had to downgrade. its displaying everything but im not getting response when throttling just stays at 0. what should i look at.
```

---
## \#1408 Posted by: PickSix24 Posted at: 2019-04-20T03:43:20.764Z Reads: 171

```
I feel like my mileage is being recorded inaccurately, a little too much. I have my gear ratio and wheel size correct. If I were to track mileage with gps and compare. How would I go about correcting it ? Also using unity if it matters.
```

---
## \#1409 Posted by: mishrasubhransu Posted at: 2019-04-20T04:23:02.033Z Reads: 173

```
Make sure that the number of magnets are correct. Default of 14 is not correct for all motors.
```

---
## \#1410 Posted by: PickSix24 Posted at: 2019-04-20T04:27:35.365Z Reads: 176

```
I’m running these 
https:///collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv

Not sure what the setting should be
```

---
## \#1411 Posted by: janpom Posted at: 2019-04-20T05:17:37.826Z Reads: 173

```
You can adjust your wheel size to compensate. For example, if you are getting 0.9 times the mileage recorded by the GPS, divide the wheel size by 0.9.
```

---
## \#1412 Posted by: janpom Posted at: 2019-04-20T05:19:22.512Z Reads: 171

```
Which version does work for you and which doesn't? What kind of ESC do you have?
```

---
## \#1413 Posted by: 702vegas Posted at: 2019-04-20T06:11:50.166Z Reads: 163

```
flipsky 6. downgraded to 38.
```

---
## \#1414 Posted by: janpom Posted at: 2019-04-20T11:35:20.867Z Reads: 162

```
Ah, you mean you had to downgrade the VESC FW. I though you were talking about the DAVEga FW. Currently VESC FW up to 3.40 is known to be compatible. Looking to the VESC changelog, 3.42 should still work but not 3.43 and later. I'll add an issue for this and fix it soon.
```

---
## \#1415 Posted by: 702vegas Posted at: 2019-04-20T16:58:30.434Z Reads: 156

```
any idea where to start to get it to communicate with the board?
```

---
## \#1416 Posted by: 702vegas Posted at: 2019-04-20T17:38:14.090Z Reads: 159

```
also just upgraded davega fw. and went back to 3.4 on esc but went back to white screen again.
```

---
## \#1417 Posted by: janpom Posted at: 2019-04-20T17:39:45.724Z Reads: 161

```
If you have a white screen, that's a hardware issue. Make sure the display pins have a good contact with the PCB.
```

---
## \#1418 Posted by: 702vegas Posted at: 2019-04-20T19:04:05.698Z Reads: 162

```
I had display when i downgraded to 3.8 so not sure
```

---
## \#1419 Posted by: janpom Posted at: 2019-04-20T19:16:57.669Z Reads: 156

```
The screen is normally rendered even if the DAVEga is not connected to a VESC. If you get a white screen, that has nothing to do with the VESC FW version. It's a DAVEga problem. What hardware do you have? I don't think you purchased a kit from me.
```

---
## \#1420 Posted by: PickSix24 Posted at: 2019-04-20T19:20:08.267Z Reads: 158

```
Ok so I traveled 1 mile and the Dave is saying 1.73 traveled. What should I set wheel size to if I have 200mm wheels ?
200 / .73 ?
```

---
## \#1421 Posted by: janpom Posted at: 2019-04-20T19:37:43.440Z Reads: 158

```
200 / 1.73 = 116 mm

That's a significant difference. You must have the gear ratio or the number of motor poles set incorrectly. It doesn't matter though. If you reduce the wheel diameter 1.73 times, all should work correctly.
```

---
## \#1422 Posted by: PickSix24 Posted at: 2019-04-20T19:45:17.247Z Reads: 167

```
I’ll try that. I’m using these motors and left the motor poles at default 
https:///collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv
```

---
## \#1423 Posted by: 702vegas Posted at: 2019-04-20T22:15:32.729Z Reads: 163

```
i didnt. another local eskater purchased the kit and she gave me the other one to play around with
```

---
## \#1424 Posted by: janpom Posted at: 2019-04-21T01:18:52.063Z Reads: 166

```
I see. Did you use the display headers or did you solder the display directly to the PCB? Did you adjust the lengths of the display pins? Again, you will want to make sure there's a good contact between the display pins and the PCB. It's best to verify that with a multimeter.
```

---
## \#1425 Posted by: 702vegas Posted at: 2019-04-21T02:50:12.962Z Reads: 168

```
Display direct to pcb
```

---
## \#1426 Posted by: janpom Posted at: 2019-04-21T09:07:54.086Z Reads: 171

```
When you try to update the FW on DAVEga, does that work now?
```

---
## \#1427 Posted by: 702vegas Posted at: 2019-04-21T23:03:21.533Z Reads: 175

```
I did update but it was white. Just wondering if its flipsky
```

---
## \#1428 Posted by: gmurad Posted at: 2019-04-23T12:06:09.193Z Reads: 181

```
My kit arrived yesterday (only 13 days after ordering it)! Screens from Aliexpress will get here on Monday.
```

---
## \#1429 Posted by: Bobby Posted at: 2019-04-25T05:29:05.705Z Reads: 180

```
![image|281x499](upload://tvNHlMJneEusr7ylRywNOeQnK9x.jpeg) 

Flipsky has davega for $35!!!! Are you a part of this @janpom?
```

---
## \#1430 Posted by: bsancken Posted at: 2019-04-25T05:41:53.080Z Reads: 168

```
Read up in the tread. Already been discussed [here](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/1334?u=bsancken) and brought up on a sister thread [here](https://www.electric-skateboard.builders/t/new-pro-verson-flipsky-vesc/90799/2?u=bsancken)! :slight_smile:
```

---
## \#1431 Posted by: Bobby Posted at: 2019-04-25T05:52:03.815Z Reads: 169

```
Thanks bud! Hard to keep up with all the posts sometimes
```

---
## \#1432 Posted by: janpom Posted at: 2019-04-25T06:08:51.297Z Reads: 167

```
Ken from Flipsky actually got in touch a few days back and offered a small donation from each sold piece. They will also be sending me a sample for feedback. I'll keep you posted.
```

---
## \#1433 Posted by: Bobby Posted at: 2019-04-25T06:56:48.558Z Reads: 169

```
Please do! I love this forum and all the wonderful people in it!!! I will feel a lot better ordering one if I know you’re getting a small cut. I will wait on ordering until then 👍🏼
```

---
## \#1434 Posted by: mackann Posted at: 2019-04-25T11:37:54.219Z Reads: 168

```
Great to hear!
```

---
## \#1435 Posted by: deucesdown Posted at: 2019-04-26T01:12:08.574Z Reads: 168

```
Papa did I do good? Display shows stuff!

![IMG_20190425_210823|374x500](upload://9VnG2uvSZmcNYEihNRX0dCNttky.jpeg) 

Hm. Gulp.

![IMG_20190425_210812|374x500](upload://dkeOxFGyH3b7Bce6DQkY6R4YGGs.jpeg) 

Aaaah okay! :slight_smile:

This is my second arduino thing, with the first being "blink". I even burned a bootloader. Thanks papa @janpom for the gentle introduction to arduino. I don't feel guilty anymore for watching AvE videos. :slight_smile:

bootloader + firmware + display tested, I can get to soldering.

Ha I just noticed the PSU is bumping the 100mA limit I set. Gulp I had it set to my board's charging voltage at 53v when I plugged it in -- thankfully with output turned off. Seems to run at about 125mA at 5v.
```

---
## \#1436 Posted by: Arzamenable Posted at: 2019-04-27T00:39:25.835Z Reads: 168

```
Non-contributing leech here, checking in for science: 

![image|395x499](upload://5IpNlLWnnhbGiBKtBjE6pAeFcBk.jpeg) ![image|375x500](upload://j53GvuL5bLfhgJU9fryQZq5wogN.jpeg) ![image|427x500](upload://b9YZAQKeRC8RvoZrat4atm6Wj0W.jpeg) ![image|593x500](upload://bAXUevkwFj58DThDKgFg0NBrlzC.jpeg) ![image|509x499](upload://mCayDWQ6fffhE6oqYfTDIXm8Pnq.jpeg) ![image|638x500](upload://3tA6hdJLQR2KVbT7lZdmv9GnXiO.jpeg) 

Need to read thread and set up, brb.
```

---
## \#1437 Posted by: janpom Posted at: 2019-04-27T05:59:07.533Z Reads: 163

```
Interesting. So there's both 7pin and 8pin connectors? That seems unnecessary since the 7pin can be plugged into the 8pin port just fine. @Arzamenable, does it look like that when you install it on your deck front tip the wires will reach the VESC?
```

---
## \#1438 Posted by: Scream Posted at: 2019-04-29T01:57:36.318Z Reads: 166

```
I got mine from Flipsky today

![image|375x500](upload://37y2qT35Wky6bHoDtK1llboQgBA.jpeg) ![image|375x500](upload://oCs5MJ7u9H10Rs5ipDqAyWyA0gl.jpeg) 

Definitely feels like a return to “old” flipsky styles. Stuff in a bag, wrapped in bubble wrap, in a plain brown box. Gets the job done for sure, but I thought we were turning a corner with the VX1 remote (branded packaging etc)

Case feels robust. I don’t have much experience with 3d printing, but if this is a 3d printed part I would be comfortable using more 3d printed parts in future builds. I always expected 3d printed stuff would feel kinda like hot glue after it sets. I kinda like how it’s this neutral, matte white. Looks and feels like it will be easy to customise with paint.

The case is not able to be easily dissembled. I wanted to take photos of the internals, but I’ll need to wait until I’m home and have the time and tools to carefully prise it open. Maybe there’s no need since @janpom will receive his test unit soon. Also there’s this video on their website now which shows the internals from 3:21:

https://youtu.be/jM5X4riDr6E

Pretty bummed to find out I need a FTDI232 serial converter to load the firmware. I haven’t really been following the DAVEga development in detail, so I wasn’t aware of this. I don’t mind the extra step, it’s just it wasn’t super apparent from the flipsky site. Since I ordered they have updated their site with an option to include this with the purchase. It would have been nice if in good faith they sent the converter out with earlier orders. Now I’m gonna have to wait for a converter to come from aliexpress.

It looks like the guts are an ATmega328pIf I can get into the case, is there any reason why I couldn’t just load the firmware via the micro usb on that board?

Here’s a photo of the instructions that come with it:

![image|375x500](upload://hc8YmzcIosVsa2befUvS8EoPoC1.jpeg) ![image|375x500](upload://gkd66IJaYttnn8vYsnz3zBbN0Cz.jpeg)
```

---
## \#1439 Posted by: lrdesigns Posted at: 2019-04-29T02:25:42.915Z Reads: 165

```
[quote="Scream, post:1438, topic:71509"]
I don’t have much experience with 3d printing, but if this is a 3d printed part I would be comfortable using more 3d printed parts in future builds.
[/quote]

Pretty sure this is powder based SLA printing. It's maybe the most cost effective way to print if your doing short run production because there is no supports and you can fill the entire print volume with parts stacked on top of each other. Downsides is it usually only comes in white and has a rough sandstone like texture that may not be appropriate for some applications. 

 ![image|690x442](upload://w1s1wm62SSQfwowvo1MJ0Oj4915.jpeg)
```

---
## \#1440 Posted by: venom121212 Posted at: 2019-04-30T20:35:37.994Z Reads: 162

```
![image|281x499](upload://4v00jrHYkZup1aVYxsV6ZqCUkQj.jpeg) 

DAVEga and Unity... Working in perfect... Harmony

And because I'm sure someone will notice: I already updated to v1.0.1
```

---
## \#1441 Posted by: janpom Posted at: 2019-04-30T20:45:36.520Z Reads: 159

```
Good for you. v1.0.1 is the best DAVEga FW version. Everyone should upgrade to it! :smile:
```

---
## \#1442 Posted by: venom121212 Posted at: 2019-04-30T21:51:44.619Z Reads: 158

```
Ahh one hiccup I ran into. I'm getting battery data and tripometer data but no speed feedback when throttling. Where shall I start investigating?
```

---
## \#1443 Posted by: janpom Posted at: 2019-04-30T22:01:49.685Z Reads: 160

```
Check your wheel size and gearing settings.

Hm... but the trip distance meter functions correctly? Does it get incremented at expected rate or is it more like if you were traveling below 0.5 mph?
```

---
## \#1444 Posted by: venom121212 Posted at: 2019-04-30T22:15:54.393Z Reads: 159

```
In the first photo I posted I was on 1.0 firmware and it was logging that trip distance and amp draw. After the update, it isn't responding. Most likely something I did in the settings. I'll report back in a bit.
```

---
## \#1445 Posted by: gmurad Posted at: 2019-04-30T22:30:35.382Z Reads: 158

```
Speaking of Unity, has someone figure out how to connect DAVEga to the unexposed UART port (in lieu of the bluetooth module)?
```

---
## \#1446 Posted by: PickSix24 Posted at: 2019-04-30T22:48:00.704Z Reads: 162

```
That’s what I’m doing. Let me see if I still have the pinout somewhere
```

---
## \#1447 Posted by: gmurad Posted at: 2019-04-30T22:49:50.555Z Reads: 168

```
Oh nice! Did you need to do firmware modification to the unity? I think that's what Sofu had to do but for a Feather remote not a DAVEga
```

---
## \#1448 Posted by: PickSix24 Posted at: 2019-04-30T22:52:23.155Z Reads: 173

```
Yes, the the Dave and the feather both use the same baudrate so it works. Here’s a screen grab from Sofu’s build. 
![image|230x500](upload://nBQERXFU8xpyVbxeeA896tXZGMU.jpeg) ![image|230x500](upload://A2cXp67ImIIMkFov9siLAZuyjS7.jpeg)
```

---
## \#1449 Posted by: PickSix24 Posted at: 2019-04-30T22:53:25.685Z Reads: 167

```
I’m currently using a feather remote and a Dave. Works perfect.
```

---
## \#1450 Posted by: gmurad Posted at: 2019-04-30T23:21:31.298Z Reads: 164

```
Thanks. I was hoping no firmware changes were needed. This message is from Feb 1st and I wonder if there are updates to the Unity firmware since then (I see constant development here https://github.com/EnertionBoards/bldc).
```

---
## \#1451 Posted by: PickSix24 Posted at: 2019-04-30T23:35:43.171Z Reads: 165

```
I can’t speak on the most recent firmware but I haven’t had any issues with the one linked by sofu.
```

---
## \#1452 Posted by: kalebludlow Posted at: 2019-05-01T00:07:44.124Z Reads: 171

```
This would be a question for @Deodand
```

---
## \#1453 Posted by: pookybear Posted at: 2019-05-01T20:05:00.179Z Reads: 164

```
Is the 5 pin jst-xh connector 2.54mm pitch? I'm making a cable for the DaVega.
```

---
## \#1454 Posted by: janpom Posted at: 2019-05-01T20:06:41.850Z Reads: 166

```
Which connector? JST-XH is indeed 2.54mm pitch.
```

---
## \#1455 Posted by: pookybear Posted at: 2019-05-01T20:09:11.450Z Reads: 170

```
Sweet. Thanks. I'm making an "advanced cable" based on your post [here](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/726?u=janpom). Easier to update the unit without opening the DaVega enclosure.
```

---
## \#1456 Posted by: venom121212 Posted at: 2019-05-02T20:36:46.136Z Reads: 174

```
![image|559x46](upload://A7UXBUKuoOsLmFP8KZIaAw4sJUc.png) 

It's not like you didn't literally write it in the instructions :sweat_smile:

https://www.youtube.com/watch?v=BnUQ103_WpE
```

---
## \#1457 Posted by: venom121212 Posted at: 2019-05-02T20:57:05.594Z Reads: 174

```
![20190502_165443|281x500](upload://vhxx7qmpq2xOOjMeDiFb5Ldovph.jpeg)

Most excellent!
```

---
## \#1458 Posted by: janpom Posted at: 2019-05-06T20:53:32.363Z Reads: 169

```
Two birds with one stone. Testing the [Cheap FOCer](https://www.electric-skateboard.builders/t/cheap-focer-vesc-compatible-4-12-redesign/81344?u=janpom) with Flipsky DAVEga. :smile: 

![DSC02168|690x460](upload://2eWtbgnxvxp8N7OTHdFJ120IeNx.jpeg)
```

---
## \#1459 Posted by: pookybear Posted at: 2019-05-07T06:22:16.171Z Reads: 173

```
Inquiring about these:

* Is it normal to see zero speed as soon as you let go of the throttle? I would think it would gradually count down the speed.

* Is it frowned upon when you try to reconfigure the unit while its connected to vesc? Meaning JST is plugged in the UART port and you connect the USB dongle to your laptop to change the settings. Power is off on the board of course.

I tried the latter and it gave me DRV fault error. I got scared and unplugged the USB. Turned on my board and it still works. No fault codes.
```

---
## \#1460 Posted by: janpom Posted at: 2019-05-07T07:46:18.752Z Reads: 175

```
[quote="pookybear, post:1459, topic:71509"]
Is it normal to see zero speed as soon as you let go of the throttle?
[/quote]

Definitely not. I bet you're looking at the motor amps or battery amps rather than on the speed. Those do drop to 0 as soon as you let go of the throttle.

[quote="pookybear, post:1459, topic:71509"]
Is it frowned upon when you try to reconfigure the unit while its connected to vesc?
[/quote]

I haven't tried that myself but I imagine it can be problematic since the ATMEGA-328 PU only has one UART port that's used for both programming and connecting to VESC. So if you connect the USB-UART adapter to the Dave while it's connected to the VESC you're effectively connecting it to both Dave and VESC. The fact that the VESC is powered off may not be relevant. The UART adapter has 5V to power the target device and so it probably actually powers on the VESC MCU. IMO you don't want to do this.
```

---
## \#1461 Posted by: pookybear Posted at: 2019-05-12T17:59:32.383Z Reads: 169

```
@janpom 

Just stopping by to give you a massive thank you for making this. It's pretty bad ass!

![Attach177950_20190512_104009|299x500](upload://9PJpBYjbvLX3q2kkpju1zmPEdSK.jpeg)
```

---
## \#1462 Posted by: janpom Posted at: 2019-05-14T20:08:04.288Z Reads: 161

```
I had a dull moment this afternoon so I assembled one kit and got it recorded. After reviewing the video I feel like I probably won't make a career as a youtuber. :laughing: I hope it still helps someone.

https://youtu.be/QPjD0Zebh9U
```

---
## \#1463 Posted by: gmurad Posted at: 2019-05-19T22:55:43.151Z Reads: 157

```
Thanks for this video. Just assembled one by copying the video.

After assembling and turning it on via USB the 3 buttons didn't do anything went pressed. Is that normal?
```

---
## \#1464 Posted by: pookybear Posted at: 2019-05-19T22:58:16.515Z Reads: 153

```
Is it connected to your Vesc?
```

---
## \#1465 Posted by: gmurad Posted at: 2019-05-19T22:58:53.697Z Reads: 155

```
No, just connected via USB.
```

---
## \#1466 Posted by: pookybear Posted at: 2019-05-19T23:10:12.323Z Reads: 156

```
I believe there is a post here stating that it needs to be connected to Vesc. When I was setting up mine, nothing happened also when I pressed the buttons. As soon as I connected them, they worked.
```

---
## \#1467 Posted by: gmurad Posted at: 2019-05-19T23:34:00.136Z Reads: 163

```
Thanks for the info.

How did your @lrdesigns's mount? Did you also use double sided tape? I just printed mine but realized this is for surfrodz and I'm using TB trucks or Caliber IIs... I guess it's time to learn a bit of 3d modeling and remix it.

It printed with no issue on PETG
![image|690x335](upload://b94TbmpgZnJ0xcYjvXfe42FURJL.jpeg)
```

---
## \#1468 Posted by: pookybear Posted at: 2019-05-19T23:51:15.962Z Reads: 159

```
I did use double sided tape so the screen doesn't flop around. It was place under the screen opposite to where screen port is. The screen connector prongs were cut a little to get it to work w that enclosure. Otherwise, I can't screw the lid. 

Hope this helps
```

---
## \#1469 Posted by: PickSix24 Posted at: 2019-05-20T00:20:10.064Z Reads: 156

```
This is correct, buttons don’t work until connected to vesc
```

---
## \#1470 Posted by: lrdesigns Posted at: 2019-05-20T01:53:25.525Z Reads: 156

```
It’s not for any particular truck, so long as your using the old school bolt pattern. The longer of the two patterns. Then the bolt heads can be accessed through the print, but they are not holding it down. 

The case is just meant to be stuck down with high quality double tape.
```

---
## \#1471 Posted by: lrdesigns Posted at: 2019-05-20T03:07:57.518Z Reads: 153

```
@pookybear err the davga logo is meant to be on the right side, its not meant to fit like that. It will fit together much better if you turn the top half 180 deg. There is a locating feature that is meant to make the orientation more obvious, I guess it's not that effective.
```

---
## \#1472 Posted by: pookybear Posted at: 2019-05-20T03:23:22.222Z Reads: 159

```
![15583225155911025321577|375x500](upload://pShqFZdnnSA0OmIccb3coZnhyLv.jpeg) 

You mean this notch?
```

---
## \#1473 Posted by: pookybear Posted at: 2019-05-20T03:23:39.288Z Reads: 150

```
Crap. I see it now
```

---
## \#1474 Posted by: lrdesigns Posted at: 2019-05-20T03:25:54.872Z Reads: 151

```
Yes, lol. Surprising you got shut.
```

---
## \#1475 Posted by: pookybear Posted at: 2019-05-20T03:42:54.610Z Reads: 153

```
Gorilla grip brah. LOL
```

---
## \#1476 Posted by: pookybear Posted at: 2019-05-20T03:51:24.875Z Reads: 161

```
@lrdesigns
 
![1558324234918467087694|666x500](upload://2rwXAgOASKwkjwVSgfoQpvjufRG.jpeg)
```

---
## \#1477 Posted by: slade Posted at: 2019-05-26T04:13:42.010Z Reads: 154

```
So I was looking into info about the ili9225 display driver chips that the 2 inch screens it uses, and it seems like the max resolution they support is only 176x220. I'm itching to try and make a DAVEga using a 2.8", 320x240 resolution screen and an arduino nano (the extra display size is definitely worth it). I just ordered the parts and I'll reply to this once it all comes in and I make progress porting over the display code to work with ili9341 display drivers. Will be a couple weeks till all parts arrive :)
```

---
## \#1478 Posted by: janpom Posted at: 2019-05-26T05:31:21.458Z Reads: 153

```
Sounds good. You may want to check this for an example of enabling a screen with a different driver: https://github.com/janpom/davega/commit/5bf124cdb6d8572699983b6b5258442c78a6f7c2

Note that the new DAVEga that we're currently working on together with @lrdesigns will use exactly the display that you mention. Plus, it will come in a nice aluminum case and with a lot of new features. You may just as well want to wait for that one. It should be available around August.
```

---
## \#1479 Posted by: slade Posted at: 2019-05-26T06:43:54.354Z Reads: 156

```
Good to hear! By chance, have you taken a look at this optimized version of the ili9341?  
  
https://www.youtube.com/watch?v=rL_2_D3cgFg  

I used it in a previous project involving some custom animations and it was a godsend for my performance.
```

---
## \#1480 Posted by: 0Z3M0 Posted at: 2019-05-26T21:04:36.504Z Reads: 150

```
Hey guys, noob question,
Is there like a parts list or something and where can I get the PCB from?
```

---
## \#1481 Posted by: venom121212 Posted at: 2019-05-26T22:33:46.383Z Reads: 153

```
https://github.com/janpom/davega/blob/master/README.md

All info needed is on the github
```

---
## \#1482 Posted by: 0Z3M0 Posted at: 2019-05-27T16:36:21.683Z Reads: 143

```
Thank you :grinning:
```

---
## \#1483 Posted by: Mudders Posted at: 2019-06-05T20:49:35.418Z Reads: 136

```
@janpom or anyone, im an old guy trying really hard here to get my dga going, ive followed the instructions but i get this and my dga has a white screen :frowning:

Any help much appreciated

![20190605_214624|690x335](upload://urDkes7VZNc3fKuFWBABrExDIgN.jpeg)
```

---
## \#1484 Posted by: janpom Posted at: 2019-06-05T21:13:57.227Z Reads: 136

```
Looks like the compiler is having hard time compiling your code. This may be a bug in the compiler. It's not unheard of. You could try a different version of Arduino IDE and see if that helps.

Have you done any changes to the code (including the config) before trying to compile? If you did, please try to compile the vanilla code first. If that works, please provide the code changes you have made. I suppose you have only touched the `davega_config.h` so ideally send that file.
```

---
## \#1485 Posted by: Mudders Posted at: 2019-06-05T22:13:57.953Z Reads: 136

```
Thanks @janpom, i trued a different ide and its working great :slight_smile:
Your opening message had me slightly worried for a second :smile:   

![20190605_231044|690x335](upload://lJGyjr5U8lwVRnpyl1jcJIbxXN8.jpeg)
```

---
## \#1486 Posted by: Mudders Posted at: 2019-06-08T12:57:28.467Z Reads: 139

```
I finally soldered the switches up and connected it to the unity, set the baud rate in the app and applied it and while the screen lights up correctly the buttons appear to do nothing and the screen does not show any live data, what have I missed please?

here is my config file, sorry I do not know how to show it any other way..

[code]
/*
    Copyright 2018 Jan Pomikalek <jan.pomikalek@gmail.com This file is part of the DAVEga firmware.

    DAVEga firmware is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    DAVEga firmware is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with DAVEga firmware.  If not, see <https://www.gnu.org/licenses/>.
*/

#ifndef DAVEGA_CONFIG_H
#define DAVEGA_CONFIG_H
#define NOEASTER
// To compile for FOCBOX Unity, uncomment the following line.
#define FOCBOX_UNITY 1

#define VESC_COUNT 1  // number of controllers: 1 = single, 2 = dual (set to 1 for FOCBOX Unity unless you have more than 1)
#define MOTOR_POLE_PAIRS 7
#define WHEEL_DIAMETER_MM 110
#define MOTOR_PULLEY_TEETH 15
#define WHEEL_PULLEY_TEETH 39

// Affects the speed indicator. If MAX_SPEED_KPH is exceeded, no major disaster will happen.
// The speed indicator will merely indicate the current speed as the max speed (all blue rectangles
// filled). It will still show the correct number though.
#define MAX_SPEED_KPH 50

// Set to true to display the distance in miles and the speed in mph.
#define IMPERIAL_UNITS true

// Set to true to display the temperature in Fahrenheit instead of Celsius.
#define USE_FAHRENHEIT false

#define BATTERY_S 12  // number of battery cells
#define BATTERY_MAX_MAH 8000  // battery capacity in mAh
#define BATTERY_USABLE_CAPACITY 0.8  // [0.0, 1.0]

// If SHOW_AVG_CELL_VOLTAGE is true, average cell voltage is displayed instead of the total battery
// pack voltage (total voltage is divided by the number of cells).
#define SHOW_AVG_CELL_VOLTAGE true

// The two options below are for detecting that battery has been fully charged (in which case
// we reset the available mAh to the max value). We think that the battery has been fully charged
// if the voltage has increased at least a little bit since the last remembered state AND the
// battery voltage is close to the max value (which is the last value in DISCHARGE_TICKS, see below).

// How much the battery voltage must increase since the last remembered state so that
// so that we think the battery has been charged.
#define FULL_CHARGE_MIN_INCREASE 0.01  // [0.0, 1.0]

// Minimal percentage of the max battery voltage to consider the battery fully charged.
// Example: With 0.97, if the max voltage is 50.4 V, then 48.888 V or more is considered fully charged.
#define FULL_CHARGE_THRESHOLD 0.97  // [0.0, 1.0]

// The DISCHARGE_TICKS can be used for configuring the battery discharge profile. The first value in the
// array is the voltage for fully discharged and the last value is the voltage for fully charged. The
// array may contain any number of values representing equidistant points of the discharge curve. For
// example, with 5 values, the voltages will be interpreted as 0%, 25%, 50%, 75%, and 100% of the battery
// capacity respectively.
#define DISCHARGE_TICKS { \
    3.5 * BATTERY_S, \
    3.67 * BATTERY_S, \
    3.73 * BATTERY_S, \
    3.76 * BATTERY_S, \
    3.80 * BATTERY_S, \
    3.83 * BATTERY_S, \
    3.86 * BATTERY_S, \
    3.90 * BATTERY_S, \
    4.0 * BATTERY_S, \
    4.2 * BATTERY_S, \
}

// Remaining battery capacity can be estimated from the battery voltage
// and from the VESC coulomb counter (number of mAh spent). The VOLTAGE_WEIGHT is
// the weight of the battery voltage in the calculation. (1.0 - VOLTAGE_WEIGHT) is
// then the weight of the coulomb counter.
//
// In particular,
// 1.0 = only use battery voltage for estimating remaining capacity.
// 0.0 = only use coulomb counter for estimating remaining capacity.
#define VOLTAGE_WEIGHT 0.4

// Changing the EEPROM_MAGIC_VALUE (to any value different from the current, e.g. 42 -> 43) will reset
// the EEPROM to the values defined below. This is especially handy for pre-setting the total distance
// traveled (EEPROM_INIT_VALUE_TOTAL_DISTANCE).
#define EEPROM_MAGIC_VALUE 43  // [1, 255]

#define EEPROM_INIT_VALUE_VOLTS 0
#define EEPROM_INIT_VALUE_MAH_SPENT 0
#define EEPROM_INIT_VALUE_MAX_SPEED 0
#define EEPROM_INIT_VALUE_MILLIS_ELAPSED 0
#define EEPROM_INIT_VALUE_MILLIS_RIDING 0
#define EEPROM_INIT_VALUE_MIN_VOLTAGE 60
#define EEPROM_INIT_VALUE_TRIP_DISTANCE 0  // meters
#define EEPROM_INIT_VALUE_TOTAL_DISTANCE 0  // meters

// After how many meters traveled should the distance (and other values) be stored to EEPROM.
// The EEPROM lasts for 100,000 write cycles. With EEPROM_UPDATE_EACH_METERS=100, the EEPROM
// should last for 10,000 km. If the value is set lower, the EEPROM will die earlier.
// Note that EEPROM is also updated whenever the board comes to a stop (see below), so regardless
// of how EEPROM_UPDATE_EACH_METERS is set, there won't be missed meters unless DAVEga is accidentally
// reset before saving to EEPROM (which shouldn't happen under normal circumstances).
#define EEPROM_UPDATE_EACH_METERS 100

// If the board comes to stop, update EEPROM, unless it was already updated in less than
// EEPROM_UPDATE_MIN_DELAY_ON_STOP millis when the board stopped. This shouldn't happen
// under normal circumstance and is mainly a safeguard against destroying EEPROM in case
// unexpected oscillating speed readings are retrieved from the VESC.
//
// The EEPROM will still be updated if it was previously updated in less than
// EEPROM_UPDATE_MIN_DELAY_ON_STOP due to EEPROM_UPDATE_EACH_METERS. (Otherwise, meters would be missed.)
#define EEPROM_UPDATE_MIN_DELAY_ON_STOP 10000

// Hold button 1 for this time to reset session data.
// Hold button 2 for this time to reset the Coulomb counter.
#define COUNTER_RESET_TIME 3000  // ms

// This corresponds (more or less) to how often data is read from VESC.
#define UPDATE_DELAY 50  // ms

// 0=portrait, 1=right rotated landscape, 2=reverse portrait, 3=left rotated landscape
#define SCREEN_ORIENTATION 3

// Screens. Uncomment the ones you want enabled.
//#define DEFAULT_SCREEN_ENABLED 1
#define SIMPLE_HORIZONTAL_SCREEN_ENABLED 1
//#define SIMPLE_HORIZONTAL_SCREEN_WITH_BATTERY_CURRENT_ENABLED 1
//#define SIMPLE_HORIZONTAL_SCREEN_WITH_MOTOR_CURRENT_ENABLED 1
//#define SIMPLE_VERTICAL_SCREEN_ENABLED 1
//#define SIMPLE_VERTICAL_SCREEN_WITH_BATTERY_CURRENT_ENABLED 1
//#define SIMPLE_VERTICAL_SCREEN_WITH_MOTOR_CURRENT_ENABLED 1
#define TEXT_SCREEN_ENABLED 1

// Information to be displayed on the text screen. Only relevant if TEXT_SCREEN_ENABLED is set.
// Available options:
//    SCR_FW_VERSION
//    SCR_FAULT_CODE
//    SCR_MOSFET_TEMPERATURE
//    SCR_MOTOR_TEMPERATURE
//    SCR_MOTOR_CURRENT
//    SCR_BATTERY_CURRENT
//    SCR_DUTY_CYCLE
//    SCR_TOTAL_VOLTAGE
//    SCR_MIN_TOTAL_VOLTAGE
//    SCR_AVG_CELL_VOLTAGE
//    SCR_BATTERY_CAPACITY_MAH
//    SCR_BATTERY_CAPACITY_PERCENT
//    SCR_TRIP_DISTANCE
//    SCR_TOTAL_DISTANCE
//    SCR_SPEED
//    SCR_MAX_SPEED
//    SCR_AVG_SPEED
//    SCR_TIME_ELAPSED
//    SCR_TIME_RIDING
#define TEXT_SCREEN_ITEMS { \
    SCR_FAULT_CODE, \
    SCR_MOSFET_TEMPERATURE, \
    SCR_MOTOR_TEMPERATURE, \
    SCR_MOTOR_CURRENT, \
    SCR_BATTERY_CURRENT, \
    SCR_DUTY_CYCLE, \
    SCR_TOTAL_VOLTAGE, \
    SCR_MIN_TOTAL_VOLTAGE, \
    SCR_AVG_CELL_VOLTAGE, \
    SCR_BATTERY_CAPACITY_MAH, \
    SCR_BATTERY_CAPACITY_PERCENT, \
    SCR_TRIP_DISTANCE, \
    SCR_TOTAL_DISTANCE, \
    SCR_SPEED, \
    SCR_MAX_SPEED, \
    SCR_AVG_SPEED, \
    SCR_TIME_ELAPSED, \
    SCR_TIME_RIDING, \
}

// Big font is only recommended for landscape orientation. 9 lines fit on the screen then.
// Some items overflow the right order. You may want to adjust the labels in davega_text_screen.cpp.
#define TEXT_SCREEN_BIG_FONT false



#endif //DAVEGA_DAVEGA_CONFIG_H
[/code]
```

---
## \#1487 Posted by: pookybear Posted at: 2019-06-08T13:11:49.546Z Reads: 130

```
Do you have PPM and UART enabled? Check your tx and RX pins.
```

---
## \#1488 Posted by: pookybear Posted at: 2019-06-08T13:20:06.372Z Reads: 130

```
Right and middle buttons reset your "text" screen stats when you hold it for a few seconds while left button toggles your screen type (you only have two set- max is 4 I believe).
```

---
## \#1489 Posted by: Mudders Posted at: 2019-06-08T13:20:23.987Z Reads: 124

```
Check where @pookybear? #noobsoz
```

---
## \#1490 Posted by: pookybear Posted at: 2019-06-08T13:22:14.089Z Reads: 121

```
Your cable pins that connect from DaVega  to your unity's uart port.
```

---
## \#1491 Posted by: Mudders Posted at: 2019-06-08T13:24:16.581Z Reads: 139

```
Ahh yes, they are connected.

![20190608_142349|243x500](upload://uyvCSuJbhvHHnpqWbRMTI1c2S6a.jpeg)
```

---
## \#1492 Posted by: Mudders Posted at: 2019-06-08T13:25:31.480Z Reads: 138

```
![20190608_142457|243x500](upload://4mYdNbRWONv5rzQnyTmIMYRHNPJ.jpeg)
```

---
## \#1493 Posted by: pookybear Posted at: 2019-06-08T13:26:30.894Z Reads: 137

```
I don't remember whether

* Rx to RX
* Tx to TX 

Or

* Rx to tx
* Tx to RX
```

---
## \#1494 Posted by: Mudders Posted at: 2019-06-08T13:31:41.728Z Reads: 138

```
I switched the white and yellow wires at the unity and the screen just showed white.

The information just doesnt seem to be getting through for some reason :-(
```

---
## \#1495 Posted by: pookybear Posted at: 2019-06-08T13:33:49.324Z Reads: 136

```
Do you at least see your battery voltage on the screen?
```

---
## \#1496 Posted by: Mudders Posted at: 2019-06-08T13:34:52.935Z Reads: 137

```
No, no info, it lights up correctly but no info at all, just 0.00
```

---
## \#1497 Posted by: pookybear Posted at: 2019-06-08T13:37:44.592Z Reads: 136

```
One last thing. I assume the white wires to left on the pic aren't connected to anything while your 4 multi colored wires are connected to the unity.

Edit:

I'm dumb. I think those are for the switches.
```

---
## \#1498 Posted by: pookybear Posted at: 2019-06-08T13:43:34.468Z Reads: 138

```
Sorry man. I'm out of ideas. The only thing I could think of is to reflash the firmware. It could be corrupted? It could also be that maybe the new unity firmware is not compatible w the current DaVega version?

I'm using vesc6.
```

---
## \#1499 Posted by: Mudders Posted at: 2019-06-08T13:44:22.830Z Reads: 140

```
Yeah, they are the switches. I continuity checked every cable including switches and all seems good, i dont understand why i get no info :cry

![20190608_144127|243x500](upload://eKHoODGqMsm0y2JzActHcHB2Bfv.jpeg)

![20190608_144141|690x335](upload://solSl2mJUahsj0xRnc3AK6dtQAm.jpeg)
```

---
## \#1500 Posted by: pookybear Posted at: 2019-06-08T13:48:43.331Z Reads: 128

```
In Vesc tool, you have ppm and Uart enabled right? I didn't get a confirmation from you earlier.
```

---
## \#1501 Posted by: Mudders Posted at: 2019-06-08T13:52:02.919Z Reads: 130

```
In the app i set uart mode to 115200 baud, but thats it. Ppm mode is forward/brake. Is there another PPM setting? Should i use the vesc tool? Ive not tried that yet...
```

---
## \#1502 Posted by: pookybear Posted at: 2019-06-08T13:53:03.257Z Reads: 134

```
Yes. You should check it. Vesc tool.
```

---
## \#1503 Posted by: Mudders Posted at: 2019-06-08T13:54:00.212Z Reads: 136

```
Cool ok, ill go have a look (optimistic smiley)
```

---
## \#1504 Posted by: pookybear Posted at: 2019-06-08T13:58:27.382Z Reads: 135

```
I know it's a given but make sure you use unity's Vesc tool.
```

---
## \#1505 Posted by: Mudders Posted at: 2019-06-08T14:00:55.580Z Reads: 136

```
Here right? Which option?

![20190608_145951|690x335](upload://rgJl3Wye4Kl11YXWQ9GBX0T0uB5.jpeg)
```

---
## \#1506 Posted by: pookybear Posted at: 2019-06-08T14:01:36.897Z Reads: 132

```
To the left, hit general under app
```

---
## \#1507 Posted by: Mudders Posted at: 2019-06-08T14:04:05.066Z Reads: 137

```
Yep

![20190608_150335|690x335](upload://iTtA7fkxj9VG2gR0AMJVEXaEt3f.jpeg)
```

---
## \#1508 Posted by: pookybear Posted at: 2019-06-08T14:04:34.914Z Reads: 135

```
![15600026458381126987241|666x500](upload://ishFVxIY81QdPBnGDDNxh3VA7g0.jpeg)
```

---
## \#1509 Posted by: Mudders Posted at: 2019-06-08T14:05:48.578Z Reads: 133

```
I need to get me that vesc tool...


Loading...
```

---
## \#1510 Posted by: pookybear Posted at: 2019-06-08T14:06:30.263Z Reads: 132

```
Unity Vesc tool should have that. You are just not under the correct area
```

---
## \#1511 Posted by: pookybear Posted at: 2019-06-08T14:08:46.118Z Reads: 133

```
* Under APP settings
* General
* First option to the right
* Choose PPM and UART
* Hit write
```

---
## \#1512 Posted by: Mudders Posted at: 2019-06-08T14:14:14.150Z Reads: 134

```
Got it, thanks for your help but dave is still the same :-(
```

---
## \#1513 Posted by: pookybear Posted at: 2019-06-08T14:15:18.149Z Reads: 133

```
Unplug battery. Wait 30 secs and plug it back in.
```

---
## \#1514 Posted by: Mudders Posted at: 2019-06-08T14:15:22.517Z Reads: 143

```
![20190608_151434|690x335](upload://1EFGRhgUBcKwCmEfoeAnyhdotuz.jpeg)
```

---
## \#1515 Posted by: pookybear Posted at: 2019-06-08T14:21:08.246Z Reads: 137

```
Turn off unit. Wait 10 secs. Turn it back on. Also make sure in Vesc tool it kept the ppm and Uart settings.

It's a good habit that you hit read settings first before you change and write new parameter settings in the Vesc tool. This sh!t got me a few times :see_no_evil:
```

---
## \#1516 Posted by: Mudders Posted at: 2019-06-08T14:22:02.527Z Reads: 131

```
No joy im afraid, i connected back to the vesc tool and read the settings to check and it is ppm and uart
```

---
## \#1517 Posted by: pookybear Posted at: 2019-06-08T14:22:14.189Z Reads: 129

```
If this doesn't work, Im out of tricks for you. Time to bring in the big guns? @janpom ?
```

---
## \#1518 Posted by: janpom Posted at: 2019-06-08T14:58:11.135Z Reads: 133

```
Hey guys. Thanks @pookybear for trying to help. 

[quote="Mudders, post:1494, topic:71509"]
I switched the white and yellow wires at the unity and the screen just showed white.
[/quote]

That shouldn't happen. If your TX/RX is swapped, the screen should still be rendered correctly. The indicator rectangle in the bottom part of the screen will blink red. The red indicates that the communication with the VESC is not working. That can either be a software problem (misconfigured VESC) or a hardware problem (TX/RX swapped or a continuity problem). The rectangle will turn green when the connection is established.

I suggest that you try swapping TX/RX again. If that gives you a while screen; try powering off and on again.
```

---
## \#1519 Posted by: janpom Posted at: 2019-06-08T15:02:11.423Z Reads: 144

```
[quote="Mudders, post:1491, topic:71509"]
![20190608_142349|243x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/d/6/d627e1fc177ea852efe3b8afb9f0b7a3762d0866_2_243x500.jpeg)
[/quote]

[quote="Mudders, post:1492, topic:71509"]
![20190608_142457|243x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/e/1ea1726735aeeb17fa0c297f3b9e3e1676045dc3_2_243x500.jpeg)
[/quote]

If the colors match, then you have RX/TX swapped. It should go:
RX-RX
TX-TX

Also, you have the red wire on the DAVEga PCB connected to GND and the black to 5V whereas on the VESC you have red on 5V and black on GND. I suppose you connect red on black and black on red. Correct?
```

---
## \#1520 Posted by: Mudders Posted at: 2019-06-08T15:47:43.389Z Reads: 134

```
Thanks for replying @janpom, i did as you said and switched the tx/rx at the unity, power cycled and still get a white screen.

All the wire colours run inline, nothing crossed!
```

---
## \#1521 Posted by: Mudders Posted at: 2019-06-08T15:53:35.969Z Reads: 134

```
I see what you are saying @janpom, i made the noob mistake of using wire colours instead of whats printed on the board... doh
```

---
## \#1522 Posted by: janpom Posted at: 2019-06-08T16:01:02.899Z Reads: 146

```
[quote="Mudders, post:1521, topic:71509"]
i made the noob mistake of using wire colours instead of whats printed on the board
[/quote]

I'm not sure what this means. Please double check that the wires go:
- 5V-5V
- GND-GND
- TX-TX
- RX-RX

If the wires are connected such that the colors match, then on the Dave PCB, the colors here:

[quote="Mudders, post:1491, topic:71509"]
![20190608_142349|243x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/d/6/d627e1fc177ea852efe3b8afb9f0b7a3762d0866_2_243x500.jpeg)
[/quote]

should be (left to right) red, black, yellow, white.
```

---
## \#1523 Posted by: Mudders Posted at: 2019-06-08T16:11:16.752Z Reads: 151

```
Yep got it, all working now, many thanks for your patience @pookybear and @janpom.

  I made the mistake of just plugging the supplied connector in and taking a picture for reference...

![20190608_082715|243x500](upload://2sw7cM9wFrq2m24mqqLaXnjp5Po.jpeg) 

Then desoldered the connector from the board and soldered the wires in the same order, wrongly assuming that the coloures of the wires were correct, thats my noob mistake!

Wires switched to the correct order and whaddya know, all good!

![20190608_170957|243x500](upload://rSbYYdsuhBEBEhs9wO7aRb5DUtO.jpeg) 

One down one to go....
```

---
## \#1524 Posted by: janpom Posted at: 2019-06-08T17:17:11.093Z Reads: 147

```
[quote="Mudders, post:1523, topic:71509"]
Then desoldered the connector from the board and soldered the wires in the same order, wrongly assuming that the coloures of the wires were correct
[/quote]

Yeah, I know the colors on the supplied connectors are confusing. Sorry about that. I had ones with different order of colors in the first batch. I got different ones for the second batch and haven't noticed that until it was late. I talk about that here: 

https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/1302?u=janpom
```

---
## \#1525 Posted by: Mudders Posted at: 2019-06-08T20:25:08.255Z Reads: 133

```
Its all good man, i have learned a lesson today and no harm done :slight_smile:
```

---
## \#1526 Posted by: Mudders Posted at: 2019-06-16T22:08:39.392Z Reads: 137

```
I'm ready for another lesson @janpom!!

I took dave his first outing today,  i live this little gizmo,  but i have a problem i want to fix.

The speed is spot on, but the trip milage is around 50% more than it should be, what do i adjust to tune it??
```

---
## \#1527 Posted by: janpom Posted at: 2019-06-16T22:14:47.326Z Reads: 138

```
That shouldn't happen. If the speed is correct, the mileage should be correct as well. What VESC FW version do you have?
```

---
## \#1528 Posted by: Mudders Posted at: 2019-06-16T22:24:13.335Z Reads: 139

```
Im on unity 23.43
```

---
## \#1529 Posted by: Mudders Posted at: 2019-06-16T22:28:15.769Z Reads: 142

```
Tomorrow i will go exactly 1mile according to my phone gps, and see what dave reads. I was out with a couple of evolve boards and our speeds matched perfectly.

![20190616_192925|243x500](upload://ble9lXz421wFZj8mPnKYk3oSMq3.jpeg)
```

---
## \#1530 Posted by: janpom Posted at: 2019-06-16T22:32:05.694Z Reads: 144

```
OK, thanks. That should be helpful for debugging. It could be something with Unity. I haven't done thorough testing with it. It could be that it reports different numbers under `tachometer` than the standard VESC FW though that would be pretty weird. BTW, are you sure you're not on metric units and interpreting kilometers as miles?
```

---
## \#1531 Posted by: Mudders Posted at: 2019-06-16T22:39:31.695Z Reads: 150

```
No,  I'm set for miles coz kms mean nothing to me!

![20190609_193311|243x500](upload://eVP9iGS6NTsT4sQlc523oocPntP.jpeg)
```

---
## \#1532 Posted by: Mudders Posted at: 2019-06-17T21:08:53.409Z Reads: 153

```
@janpom , here is the best logging I can do...!

![Screenshot_20190617-220329_Runtastic|243x500](upload://mkkf07S9UFyih10wRmeKTaB27Yl.jpeg) 


![20190617_220341|243x500](upload://3DhKjwIDEFFHWSfRC94sNeONQV9.jpeg)
```

---
## \#1533 Posted by: Mudders Posted at: 2019-06-17T21:11:44.764Z Reads: 149

```
Also...

![Screenshot_20190617-215719_Runtastic|243x500](upload://nfNGdDoTpXJLN4mFytD96TNIbEt.jpeg) 

![20190617_215732|243x500](upload://eo1RcEG1OGRBPnV9NrADeZju7lI.jpeg)
```

---
## \#1534 Posted by: janpom Posted at: 2019-06-17T21:43:30.791Z Reads: 151

```
Thanks. This is very strange. The thing is that the computation of speed and distance uses the same code. If there was a bug, both should be wrong. Yet you're saying that your speed is correct and only the distance is off.

Simplifying things a little bit, we get the "RPM" and "tachometer" from the VESC where "tachometer" is the total number of motor revolutions. There's a routine `revolutions_to_meters` that converts the number of motor revolutions to meters using the information about wheel size and gearing. Then:

```
speed_in_kph = revolutions_to_meters(RPM) / 1000 * 60
distance_in_km = revolutions_to_meters(tachometer) / 1000
```

And we just multiply by 0.621371 to get the speed in mph and distance in miles.

There's very little room for error here. Sure, the `revolutions_to_meters` routine could have a bug but then that would cause both speed and distance to be off. I'm running out of ideas.

Guys, is there anyone else using Dave with Unity? @venom121212 @PickSix24? Is everything working as expected?
```

---
## \#1535 Posted by: esk8_hui Posted at: 2019-06-17T23:36:44.738Z Reads: 146

```
I also have 50% more trip odometer reading and slightly higher speed reading.

Here are my config:

#define VESC_COUNT 2
#define MOTOR_POLE_PAIRS 7
#define WHEEL_DIAMETER_MM 203
#define MOTOR_PULLEY_TEETH 14
#define WHEEL_PULLEY_TEETH 66

In reality I use 8 inch tiers with 14T and 66T pulley and 2 VESC 6 from trampa
```

---
## \#1536 Posted by: venom121212 Posted at: 2019-06-18T12:08:04.423Z Reads: 146

```
I had similar results with the davega reading a longer travel distance than I felt was correct but I figured a bit of error was OK.

I unfortunately broke the 3d printed case holding my davega in Colorado while riding on the dirt track so I had to yank the wires to keep riding quickly. I'm looking to order a new davega for my second build though, I really love the product.
```

---
## \#1537 Posted by: PickSix24 Posted at: 2019-06-19T03:05:40.871Z Reads: 144

```
I initially noticed the issue with the mileage being off, I honestly forget what was recommended to fix it, but I made the correction and checked against a gps app. Now I’m thinking I should go back and verify speed... 🤣
```

---
## \#1538 Posted by: Eskate444 Posted at: 2019-06-19T03:41:52.929Z Reads: 147

```
Hi guys if anyone has a full complete setup for this on sale, i would love to buy it.
```

---
## \#1539 Posted by: janpom Posted at: 2019-06-19T20:25:07.925Z Reads: 141

```
New DAVEga is coming soon. I'm just finishing the first functional prototype and will be shipping it to @lrdesigns for test fitting into the enclosure. If all goes well, we should be able to start distributing by the end of August.
```

---
## \#1540 Posted by: esk8_hui Posted at: 2019-06-19T20:34:03.754Z Reads: 139

```
Cant wait! Maybe in the future we can have one with Bluetooth so we don't have to do the wiring.
```

---
## \#1541 Posted by: slade Posted at: 2019-06-19T20:50:27.762Z Reads: 135

```
:tada::tada::tada:  
Awesome, good job! Does this new change to the enclosure come with support for larger screens?
```

---
## \#1542 Posted by: janpom Posted at: 2019-06-19T22:05:00.294Z Reads: 137

```
It will have wifi for FW updates. You will still need to wire it to the VESC. While the communication could be done wirelessly, it also needs to be powered somehow.
```

---
## \#1543 Posted by: janpom Posted at: 2019-06-19T22:10:18.627Z Reads: 135

```
It will come with 2.8" 320x240px ILI9341 screen. 2.4" and 3.2" are available with the same driver and resolution. These will work out of the box. The enclosure will be available only for 2.8" though, at least initially.
```

---
## \#1544 Posted by: mmaner Posted at: 2019-06-19T22:12:58.015Z Reads: 137

```
I need 1, let me know how to pay :slight_smile:
```

---
## \#1545 Posted by: slade Posted at: 2019-06-20T01:33:07.037Z Reads: 136

```
Is this already checked into the github repo? Like the existing code there will handle ILI9341 fine as is?
```

---
## \#1546 Posted by: janpom Posted at: 2019-06-20T07:49:45.991Z Reads: 141

```
No, this is a complete rewrite for the ESP32 platform and I currently don't intend to make the code opensource. I implemented a menu that you'll be able to use to configure the device. No more need to configure and compile the FW. The FW updates are done over the air using WiFi. You shouldn't ever need to connect the new DAVEga to your computer.

BTW, have I mentioned the enclosure will be anodized aluminum and will double as the X-thingie? ;)
```

---
## \#1547 Posted by: hexakopter Posted at: 2019-06-20T11:37:38.323Z Reads: 146

```
[quote="janpom, post:1543, topic:71509, full:true"]
It will come with 2.8" 320x240px ILI9341 screen. 2.4" and 3.2" are available with the same driver and resolution. These will work out of the box. The enclosure will be available only for 2.8" though, at least initially.
[/quote]


I see some ILI9341 based screens come with touch functionality.:sunglasses: Are you using one of those?
```

---
## \#1548 Posted by: janpom Posted at: 2019-06-20T11:49:28.549Z Reads: 144

```
Many of these displays can be had with or without the touch functionality. I have considered it for a long time and I decided against the touch display at last. You don't need to interact with the device that much for the touch display to be worth it. You configure it once and you update the FW maybe once in a month. The only interaction you'll want to do more frequently is resetting the session data or toggling between screens and that's easy to do with buttons (maybe easier than having the touch functionality). Plus, you keep the display clean by not having to touch it.

The new DAVEga will come with 3 buttons. Most of the configuration can be done conveniently with the buttons. The only exception is entering your WiFi password. That one is a bit annoying but you only do it once and it doesn't take more than a minute.
```

---
## \#1549 Posted by: venom121212 Posted at: 2019-06-20T12:02:58.651Z Reads: 143

```
The desire is strong!

My 3d printed case snapped on the dirt track in Colorado. I am definitely keeping an eye out for Dave2
```

---
## \#1550 Posted by: hexakopter Posted at: 2019-06-20T20:49:48.810Z Reads: 147

```
Makes sense. Haven't thought a lot about it actually not being that useful for our application. Was just surprised that you can get such a touch display for that few bucks.
```

---
## \#1551 Posted by: AlMcCal Posted at: 2019-07-30T02:15:09.342Z Reads: 144

```
First just want to say thanks to everyone for putting so much time into this community, it’s really amazing. Quick question here: I’ve got a dga built into my new scooter project and It’s showing the green dot, but it only displays random speed values which change with every signal refresh and 0v on the battery. I flashed new firmware several times on the dga. On my focbox: uart is enabled, baud rate is correct at 115200, and I’m running vesc firmware 2.18. The dga is a v0.2 PCB but @janpom added the 100uF cap so it should be the same as a v1.0. Any ideas?![IMG_8656|667x499](upload://2t2LgmemvOIvk0VYDWJEkfERSdW.jpeg)
```

---
## \#1552 Posted by: Pimousse Posted at: 2019-07-30T13:04:40.817Z Reads: 146

```
Good to hear !
I played a bit with ESP32, it's an amazing chip ! (The OTA FW upload is amazing !).
Do you go SMD design or you'll keep a DIY-friendly through-hole design ?

BTW, I couldn't resist to add a Davega in my cart when I purchased some VESC on Flipsky.
I'd like to try integrating DieBieMS comm for displaying cell voltages. :+1:
```

---
## \#1553 Posted by: janpom Posted at: 2019-07-31T10:13:57.587Z Reads: 139

```
I'm afraid the problem is likely the incompatibility with the VESC FW 2.18. That's pretty old. It probably isn't difficult to fix at the DAVEga end but I'm not sure when I can find the time to get it done since I'm busy working on the new DAVEGA (https://forum./t/davega-x-gauging-interest/5203). Could you just upgrade your VESC FW to at least v3.38?
```

---
## \#1554 Posted by: janpom Posted at: 2019-07-31T10:19:13.499Z Reads: 144

```
[quote="Pimousse, post:1552, topic:71509"]
Do you go SMD design or you’ll keep a DIY-friendly through-hole design ?
[/quote]

No SMD. It's actually very simple. The new project is executed completely differently though. It will be delivered as a finished product rather than DIY kit.

[quote="Pimousse, post:1552, topic:71509"]
I’d like to try integrating DieBieMS comm for displaying cell voltages.
[/quote]

That's great. I'd also like to get that done for the new DAVEGA at some point. I'm using the DieBieMS for my new build.

Please do keep us posted on how it goes!
```

---
## \#1555 Posted by: annihil8ted Posted at: 2019-08-01T21:02:14.463Z Reads: 132

```
[quote="janpom, post:1554, topic:71509"]
I’d also like to get that done for the new DAVEGA at some point. I’m using the DieBieMS for my new build.
[/quote]

That would be amazing. :smiley:  That is my current setup too. 

I see the new DAVEga is priced higher than the original DAVEga. For those that want to save a couple of dollars, will you make the older version available still?
```

---
## \#1556 Posted by: janpom Posted at: 2019-08-02T10:59:28.777Z Reads: 137

```
[quote="annihil8ted, post:1555, topic:71509"]
For those that want to save a couple of dollars, will you make the older version available still?
[/quote]

Probably not. It's hard to compete with the Flipsky prices. You can also always make one using Arduino Nano: https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/209?u=janpom. Someone even made a nice enclosure for that version though I'm not sure if they ever made the stl files available. You may want to do some digging in the DAVEga thread.
```

---
## \#1557 Posted by: janpom Posted at: 2019-08-02T11:02:24.345Z Reads: 136

```
@Bbaldrickk has made the enclosure: https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/1175?u=janpom. It's pretty neat.
```

---
## \#1558 Posted by: Flasher Posted at: 2019-08-13T13:51:08.056Z Reads: 128

```
If I want to place the davega on the slave side, can I have my master set to ppm and my slave set to uart?
```

---
## \#1559 Posted by: BallsAndWeiners Posted at: 2019-08-13T14:16:33.439Z Reads: 128

```
Yes you can.
```

---
## \#1560 Posted by: Flasher Posted at: 2019-08-13T23:03:35.154Z Reads: 130

```
Cool now my problem is with the davega itself :frowning:
https://youtu.be/jua_dYM1g4M
```

---
## \#1561 Posted by: AlMcCal Posted at: 2019-08-14T03:42:27.052Z Reads: 127

```
Updating the VESC fixed the issue, thanks!
```

---
## \#1562 Posted by: pookybear Posted at: 2019-08-29T22:27:15.066Z Reads: 113

```
@janpom 

Hey. I'm helping my buddy setup his DaVega he bought from flipsky. It comes w v0.6. I'm trying to upload the newest but its giving me "avr errors". Any idea how to fix this? TIA

![1567117597283297852455|666x500](upload://4Oo2OSkki5JKmayaK9q7xFNR4C0.jpeg)
```

---
## \#1563 Posted by: janpom Posted at: 2019-08-31T06:18:06.507Z Reads: 111

```
That's probably a hardware problem. Could be a bad UART adapter, bad wire, or just incorrectly plugged in adapter.

The device itself works correctly? Have you tried connecting it to the VESC? Did you get any readings from it?
```

---
## \#1564 Posted by: RobPBody Posted at: 2019-09-05T22:41:17.175Z Reads: 105

```
Hey, I was wondering what are some things I can try to do to get correct MPH? I put in my wheel and pulley info, but I"m getting top speed of 14MPH which i know isn't accurate (To low).
```

---
## \#1565 Posted by: Flasher Posted at: 2019-09-05T23:32:50.055Z Reads: 109

```
Did you fix it? I had the same problem earlier this week. I found out it was trying to pull data from the esc. When I plugged the adaptor in my PC, it turned on the esc for some reason (killswitch to battery removed). Try unplugging the uart while updating
```

---
## \#1566 Posted by: pookybear Posted at: 2019-09-06T00:03:30.931Z Reads: 110

```
Haven't had a chance to dissect it. It's on my list to do this weekend.
```

---
## \#1567 Posted by: pookybear Posted at: 2019-09-06T00:05:12.213Z Reads: 112

```
Yea, don't do that. Make sure when you update, DaVega needs to be disconnected from Vesc or it will throw Drv errors. Been there done that.
```

---
## \#1568 Posted by: janpom Posted at: 2019-09-06T06:19:52.249Z Reads: 116

```
[quote="RobPBody, post:1564, topic:71509"]
I was wondering what are some things I can try to do to get correct MPH
[/quote]

Check motor poles and/or pulley teeth settings. These affect the speed.

If you can't find a problem in your setup, a quick fix is to multiply the wheel size by a correcting factor. For example, if your MPH readings are 0.5 times (one half) of the actual, just multiply the wheel size by 1/0.5, i.e. by 2.
```

---
## \#1569 Posted by: pookybear Posted at: 2019-09-07T20:52:20.446Z Reads: 120

```
@janpom
@Flasher  

Flipsky:

Front

![15678892925842025458799|375x500](upload://npKDMGJLRLqPRnh6g4B8aLiaOw3.jpeg)
Back
 
![15678893256151331373269|666x500](upload://rEUA7kLr7OywftnUfwoMqN2xNXG.jpeg)

DaVega:

Front:

![1567889376296156523681|375x500](upload://cxyvzPowNQgTZHT4PfcDTAJ32VS.jpeg) 

Back:

![15678894104691025824370|666x500](upload://1fb694nFv1o6chLa00jjtt69Ogs.jpeg) 

I switched the boards. It works now! Is it normal to have a lot of missing board "components" on the flipsky vs the davega. When I saw this, I was like wtf?

[quote="janpom, post:1563, topic:71509, full:true"]
That's probably a hardware problem. Could be a bad UART adapter, bad wire, or just incorrectly plugged in adapter.

The device itself works correctly? Have you tried connecting it to the VESC? Did you get any readings from it?
[/quote]
```

---
## \#1570 Posted by: janpom Posted at: 2019-09-08T06:15:06.941Z Reads: 114

```
They didn't put the 100 uF power smoothing capacitor. Other than that, they just replaced the THT components with SMD, which are a lot smaller.
```

---
## \#1571 Posted by: UgloBuglo Posted at: 2019-09-16T08:48:50.376Z Reads: 109

```
New poster here, so please bear with me.
I just started looking into the DAVEga, will try to use it in a e-Scooter I am restoring and wanted to check one thing before continuing on.
I'm going through the settings, and the way to set up a direct drive motor would be to set **MOTOR_PULLEY_TEETH** and **WHEEL_PULLEY_TEETH** to the same value, right? Like **1** for both?

Or are there some other parameter I am missing?
```

---
## \#1572 Posted by: janpom Posted at: 2019-09-16T12:00:24.141Z Reads: 107

```
[quote="UgloBuglo, post:1571, topic:71509"]
I’m going through the settings, and the way to set up a direct drive motor would be to set **MOTOR_PULLEY_TEETH** and **WHEEL_PULLEY_TEETH** to the same value, right? Like **1** for both?
[/quote]

Yes, exactly. Any value will do as long as it's the same for both.
```

---
## \#1573 Posted by: Stan8 Posted at: 2019-10-23T20:38:32.322Z Reads: 84

```
So is the flipsky one a lot worse? I was looking at the mainstream X model, but I was also trying to find other brands that makes them for maybe a bit less.
```

---
## \#1574 Posted by: janpom Posted at: 2019-10-23T20:55:22.209Z Reads: 87

```
[quote="Stan8, post:1573, topic:71509"]
So is the flipsky one a lot worse?
[/quote]

I'm not sure if you're asking "Flipsky module" vs "my open source module" or it's "Flipsky module" vs "DAVEGA X". If the former, they put lower quality display which has annoying flickering and their housing IMO is worse than any of the [community contributed](https://github.com/janpom/davega#enclosures) that you can 3D print. Other than that, there's not much difference.

If the latter, DAVEGA X is way more advanced than the Flipsky module. It has aluminum housing and the baseplate doubles as X bracket. The screen is larger (2.8" vs 2.0"). The firmware has a lot of features that are not available in the open source firmware, such as estimating range, calculating consumption (Wh/km), configuring via menu, parts lifespan tracking... to name just a few. I'm now also actively developing the DAVEGA X fw whereas the OS fw is on hold and I doubt we'll see any pull requests from Flipsky any time soon.
```

---
## \#1575 Posted by: Stan8 Posted at: 2019-10-23T21:21:07.601Z Reads: 86

```
Thank you so much for this fast reply! I am currently looking forward into this product as it is so cool! Though I also need to see if I could get my hand on an uart splitter as I have both of my ports already used.
```

---
## \#1576 Posted by: Chricious Posted at: 2019-12-01T12:20:49.090Z Reads: 65

```
What's the current status?
```

---
## \#1577 Posted by: rey8801 Posted at: 2019-12-07T16:31:42.932Z Reads: 61

```
Nice how did you made the case for the Davega? I am also going to use it for a escooter
```

---
## \#1578 Posted by: steresis Posted at: 2019-12-08T15:17:44.781Z Reads: 59

```
I have build my own version V0.3 pcb DAVEga with cnc milling methode. Uploaded bootloader and software from Arduino IDE. Configure interface for horizontal display... All seems well.
But when I connect to my VESC V4.20 (flipsky) with 3.63 FW (ADC+UART - Baudrate:115200 Bps).   Display have good interface but communication doesn't work all value stay at 0.

The little red quare is still blinking. I try to invert RX and TX... And this time the little red square stop to blink and stay lit but do not passed to green.

I have tryed to plug simple arduino with flying wires to display  and connect to VESC, but obtain exact same issue... Does anybody allready had the same trouble and resolved it?

I already read lots of tread about DAVEga but did not found solution yet. Thank you in advance for your reply !
When solved it, I will post some pictures to show the result
```

---
## \#1579 Posted by: janpom Posted at: 2019-12-08T17:40:19.372Z Reads: 53

```
The latest updates to VESC FW added backwards incompatible changes to communication. Try downgrading the VESC firmware to somewhere around 3.40 and see if that works.

If it does, you can try asking Flipsky if they want to make the OS DAVEGA FW updates to make it work with the latest VESC FW. It would be kinda nice since they (unlike me) are making money on it.
```

---
## \#1580 Posted by: steresis Posted at: 2019-12-08T19:12:43.394Z Reads: 55

```
You have totaly right ! I go back to VESC Fw 3.58 (VESC-Tool 1.16) and It works ! 
I don't have all previous version VESC of firmware, so maybe some other Firmware between 3.58 and 3.62 could works ?
So the trouble "come" from new VESC firmware...
```

---
## \#1581 Posted by: rey8801 Posted at: 2019-12-08T22:45:24.503Z Reads: 57

```
Thanks @janpom for this project. Only found now the time to put it together. I had an older v.0.3 version but I added the 100uF capacitor so should be similar to the v1.0 😉

![IMG_20191208_234233|690x318](upload://5QfjpNKIVRy9JDFiVFVpVqiobDZ.jpeg) ![IMG_20191208_233332|230x500](upload://k89SHx0m76lUjYX0yIlJzcTSf3o.jpeg)
```

---
## \#1582 Posted by: janpom Posted at: 2019-12-08T23:30:17.223Z Reads: 55

```
Cool! Nicely done. :+1:
```

---
## \#1583 Posted by: rey8801 Posted at: 2019-12-08T23:31:47.508Z Reads: 52

```
did you write somewhere what the 3 buttons do? I know they change the screen, but 3 sounds like a lot of function or you do not need all of them? Thx
```

---
## \#1584 Posted by: janpom Posted at: 2019-12-08T23:37:56.168Z Reads: 55

```
One changes screens, one resets the current trip distance, and one resets the coulomb-counter. Coulomb-counter is auto-reset when you charge the battery so you don't really need that button.

With some code changes, the buttons could be reduced to just one when a short press switches the screen and press-and-hold resets the trip distance.
```

---
## \#1585 Posted by: rey8801 Posted at: 2019-12-08T23:38:48.878Z Reads: 57

```
crystal clear thanks :grin:
```

---
## \#1586 Posted by: AlMcCal Posted at: 2019-12-10T03:23:08.233Z Reads: 56

```
I designed the case in Onshape, and printed it on a Formlabs SLA printer.
```

---
## \#1587 Posted by: rey8801 Posted at: 2019-12-10T07:51:45.404Z Reads: 54

```
Ah ok cool! So basically is a sleeve, you place the davega inside adn then slide the whole thing on the handlebar?
```

---
## \#1588 Posted by: Shaz Posted at: 2020-01-20T20:44:23.162Z Reads: 32

```
when i try and upload the sketch, i get the following error:

**avrdude: verification error, first mismatch at byte 0x02ad**

**0x0b != 0x0f**

**avrdude: verification error; content mismatch**

avrdude: verification error; content mismatch

any ideas?
```

---
## \#1589 Posted by: janpom Posted at: 2020-01-21T11:40:14.299Z Reads: 30

```
Did you follow the steps here: https://github.com/janpom/davega#configuring-and-installing-firmware?

CP2012 drivers installed?
```

---
## \#1590 Posted by: janpom Posted at: 2020-01-21T11:41:50.112Z Reads: 30

```
Is that a DAVEGA from me with the CP2012 adapter or one from Flipsky? AFAIK, they provide it with another USB adapter.
```

---
## \#1591 Posted by: Shaz Posted at: 2020-01-21T16:27:25.924Z Reads: 26

```
Flipsky. I know they typically use the FT232RL FTDI adapter, so will check again if i have the correct adapter and drivers installed
```

---
