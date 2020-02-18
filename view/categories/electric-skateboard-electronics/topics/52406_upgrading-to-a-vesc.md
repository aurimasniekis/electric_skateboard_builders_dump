# Upgrading to a VESC

### Replies: 29 Views: 1290

## \#1 Posted by: ShakeNBake7000 Posted at: 2018-04-16T07:43:23.091Z Reads: 139

```
So I've been using a cheap race car ESC for over a year and I want to upgrade, I'm in the process of getting a BMS and wanted to use a proper VESC with my new setup.
Any recommendations? I can't really tell the difference between the VESC's, just need a reliable one that I can program and maybe have a port for a Bluetooth adapter like this one:
https://miamielectricboards.com/shop-1/vesc-bluetooth-adapter
Currently using two 3s 8000mAh batteries in series.
Any help appreciated
Thanks
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2018-04-16T10:25:37.075Z Reads: 113

```
Focbox is the one I would buy for dependability. Opinions vary on other versions of vesc.

You can backorder one here.

https://longhairedboy.com/collections/all/products/focbox-electric-skateboard-motor-controller

Or they are in stock right now here.

https://buildkitboards.com/collections/speed-controllers/products/focbox
```

---
## \#3 Posted by: ShakeNBake7000 Posted at: 2018-04-16T10:58:28.028Z Reads: 94

```
That's a little higher than my current budget, are they worth it? I was hoping to spend 100$ max for a VESC.
Any cheaper suggestions? if the 50 bucks make a big difference than I'll buy it.
Thanks for the response
```

---
## \#4 Posted by: RedEagle Posted at: 2018-04-16T11:01:07.189Z Reads: 90

```
If that's your budget then maytech vescs are what you're looking for. They work just as fine as all the others but they are less fault tolerant which means you have to handle them with care.

Otherwise just get a car esc or something.
```

---
## \#5 Posted by: i2oadsweepei2 Posted at: 2018-04-16T11:08:21.962Z Reads: 89

```
To me they are worth it. Focbox's have upgraded components Iike direct fets. However I don't know enough about the differences to explain them properly. Hopefully someone else with more knowledge about the differences and what they mean for you will explain it.

There are many many people using the $100 vescs as well with no issues. Some say most people have issues on the bench when testing by pulling full throttle with no load and damaging them. All vesc act differently on the bench then they do on the ground under load. My opinion is just my personal preference. Hope that helps in some small way.
```

---
## \#6 Posted by: RedEagle Posted at: 2018-04-16T11:17:17.260Z Reads: 82

```
The build quality of the focbox is very high overall. It's got direct fets as stated above and the design is based on the discontinued vesc 5. The vesc from esk8.de is the same quality, if not higher.

I've got some maytech vescs for sale if you want some.
```

---
## \#7 Posted by: ShakeNBake7000 Posted at: 2018-04-16T11:27:47.483Z Reads: 75

```
I live in Israel, and shipping here costs more than the vesc lol, when I buy parts I try to look at some sites that have relatively cheap worldwide shipping, so sadly I can't buy from you.
Will look more into the maytech, thanks
Another question, do you know if its possible to buy the raptor 2 board separately? or any other board that already has a prebuilt space for the electronics? I'm using a flimsy lunch box right now and it makes the board look way worse than it can be.
Thanks
```

---
## \#8 Posted by: leonsc Posted at: 2018-04-16T11:33:40.057Z Reads: 71

```
https://hobbyking.com/en_us/turnigy-skateboard-esc.html cheap and should not be to much shipping wise
```

---
## \#9 Posted by: ShakeNBake7000 Posted at: 2018-04-16T11:35:43.038Z Reads: 78

```
Yeah hobbyking is good for shipping here, point is, is it worth the extra 70$ to get the focbox or not?
I'll be using the vesc for at least a year if not more, i wanna make sure it lasts
Edit: and cool features are more than welcome
```

---
## \#10 Posted by: RedEagle Posted at: 2018-04-16T11:39:27.926Z Reads: 78

```
This could be an option.

https://www.electric-skateboard.builders/t/lacroix-board-co-wood-and-cf-deck-segmented-flex-carbon-fiber-enclosure-group-buy/49051

Or just get an enclosure from @psychotiller or @bigben.

If that also doesn't work you can make one yourself.

https://www.electric-skateboard.builders/t/thermoforming-a-kydex-battery-enclosure/8642
```

---
## \#11 Posted by: ShakeNBake7000 Posted at: 2018-04-16T11:49:28.585Z Reads: 69

```
Looking for more of a cruizer than a longboard (snap back, shorter), I'll try to find something in the forums that matches what I want.
I'm looking for a new board either way so the enclosures won't work, or maybe ill get a normal board and get one of those enclosures with it, need to think about it.
One last question, I still don't fully understand what other parts do I need to run a full discharge/charge BMS system.
Sorry for so many questions you've just been so helpful I thought id try to figure some other stuff out.
Thanks for all the help
```

---
## \#12 Posted by: pat.speed Posted at: 2018-04-16T11:58:38.600Z Reads: 63

```
Just the bms and charger, maybe a jst connector. Apart from that you should be able to just plug the bms into the battery and then plug in the charger. You might also need a charge port and power switch for your board if you don’t already have one
```

---
## \#13 Posted by: ShakeNBake7000 Posted at: 2018-04-16T12:03:29.509Z Reads: 63

```
Will these do?
https://miamielectricboards.com/shop-1/120amp-12s-power-switch
https://miamielectricboards.com/shop-1/mountable-charging-adapter

and what kind of charger do i need? i already have this:
https://hobbyking.com/en_us/hobbyking-105w-15v-7a-switching-dc-power-supply.html
will it work?
thanks
```

---
## \#14 Posted by: pat.speed Posted at: 2018-04-16T12:16:29.852Z Reads: 53

```
The first two will work fine, but that charger will only work for charging with a balance charger not a bms. If using a bms you need a charger that outputs the same voltage as your fully charged battery, for 10s- 42v charger, 12s- 50.4v charger and so on
```

---
## \#15 Posted by: ShakeNBake7000 Posted at: 2018-04-16T12:18:38.882Z Reads: 51

```
And can I use a charger with more V than my pack in case I upgrade in the future? or does it have to be exact? because I have 6s right now and i might upgrade some time.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-04-16T12:22:10.528Z Reads: 52

```
No, not that I know of as. For 6s you will need a 25.2v charger. These can be had for cheap from banggood if I remember right
```

---
## \#17 Posted by: ShakeNBake7000 Posted at: 2018-04-16T12:30:20.634Z Reads: 54

```
Alright, thank you for the help, one final question for real this time 

Do you have a certain bms you can recommend? just need something that will get the job done and won't fry after a month, been looking around for a while and can't really decide on which one to get

Edit: this should do right?
https://www.banggood.com/25_2V-2A-Smart-Charger-For-21_6V-22_2V-25_2V-Li-ion-Li-Po-Lithium-Battery-US-Plug-p-1167937.html?rmmds=search&cur_warehouse=CN
```

---
## \#18 Posted by: RedEagle Posted at: 2018-04-16T17:09:41.408Z Reads: 43

```
[quote="ShakeNBake7000, post:11, topic:52406"]
Looking for more of a cruizer than a longboard
[/quote]

Arbor Vugenhausen and Jet Spud are the first that come to mind.

[quote="ShakeNBake7000, post:11, topic:52406"]
or maybe ill get a normal board and get one of those enclosures with it, need to think about it.
[/quote]

@psychotiller can do custom enclosures. Not sure about @bigben though.

[quote="ShakeNBake7000, post:11, topic:52406"]
I still don’t fully understand what other parts do I need to run a full discharge/charge BMS system.
[/quote]

Balance wires, balance connectors, BMS, charge port & fuse/antispark. I highly recommend a coulomb meter to go with it.
```

---
## \#19 Posted by: RedEagle Posted at: 2018-04-16T17:15:46.810Z Reads: 38

```
[quote="ShakeNBake7000, post:17, topic:52406"]
Do you have a certain bms you can recommend?
[/quote]

Supower & bestech make good bms's. You can also find good one's on aliexpress & banggood but you have to know what you're looking for.

[quote="ShakeNBake7000, post:17, topic:52406"]
this should do right?

      www.banggood.com

25.2V 2A Smart Charger For 21.6V 22.2V 25.2V Li-ion Li-Po Lithium Battery US...

Only US$12.80, buy best 25.2V 2A Smart Charger For 21.6V 22.2V 25.2V Li-ion Li-Po Lithium Battery US Plug sale online store at wholesale price.US/EU warehouse.
[/quote]

That one will do fine for 6s. you can hook it up directly to the battery but I would highly recommend you connect it to a bms for charging.
```

---
## \#20 Posted by: ShakeNBake7000 Posted at: 2018-04-16T18:20:14.278Z Reads: 32

```
Wow. thank you.
The jet spud looks great for what I want, and it's not that expensive either, might get that soon.
Is a Coulomb meter just a voltage meter? or is there a difference? will one of those cheap ones work?
https://www.banggood.com/330V-DC-0_4-Inch-Voltmeter-Board-LED-Amp-Digital-Volt-Meter-Gauge-p-1044595.html?rmmds=search&cur_warehouse=CN
And about a bms, unlike the vesc I want the cheapest one that won't fry after a month, don't need any features or anything, just simpler charging.
But why does this bms cost three euros while others cost a 100?
https://www.banggood.com/PCB-BMS-6S-15A-24V-Battery-Protection-Board-For-18650-Li-ion-Lithium-Battery-Cell-p-1162772.html?rmmds=search&cur_warehouse=CN
From what I understand, its a 6s bms with more amps than my battery can charge at, and its dirt cheap.
```

---
## \#21 Posted by: RedEagle Posted at: 2018-04-16T18:28:37.290Z Reads: 27

```
A coulomb meter can do much more than read voltage. The one you linked is too low specced, only 30v. 

That bms can only discharge 15a. That's why it's so cheap. You can use it, but only for charging. 
More expensive bms's have a higher discharge, overvoltage protection, undervoltage protection etc.

Edit: Try to use the reply button :) 
Otherwise I can't know that you replied to me.
```

---
## \#22 Posted by: ShakeNBake7000 Posted at: 2018-04-16T18:39:35.396Z Reads: 27

```
Oh lol my bad, I clicked the reply to the entire thread and not you.
Anyway, how many amps do I want for a decent charge? I don't know what to base my search on as i know nothing about it

[quote="RedEagle, post:21, topic:52406"]
A coulomb meter can do much more than read voltage. The one you linked is too low specced, only 30v.
[/quote]
Talking about something like this?
https://www.banggood.com/DC-8-80V-50A-High-Precision-LiFePO-Lithium-Lead-Acid-Battery-Tester-Coulomb-Counter-p-1120272.html?rmmds=search&cur_warehouse=CN

Still getting the hang of the website
```

---
## \#23 Posted by: ShakeNBake7000 Posted at: 2018-04-16T18:55:25.896Z Reads: 25

```
I clicked reply on your message and still didn't show it as a reply, not sure why
```

---
## \#24 Posted by: RedEagle Posted at: 2018-04-16T18:57:10.559Z Reads: 24

```
Yes, now you're talking. Are you planning to go lion or lipo? Sometimes it doesn't show the reply idk why. You did reply to my comment and not the thread though.
```

---
## \#25 Posted by: ShakeNBake7000 Posted at: 2018-04-16T18:58:29.110Z Reads: 22

```
Not sure what lion is but my batteries are lipo if that's what you're asking
```

---
## \#26 Posted by: ShakeNBake7000 Posted at: 2018-04-16T18:58:43.988Z Reads: 22

```
again, did not reply for some reason
```

---
## \#27 Posted by: RedEagle Posted at: 2018-04-16T19:02:35.260Z Reads: 19

```
It did show as a reply in my notifications. As long as you click the right button everything will be fine. 5ah is a good start. Average consumption is 10Wh/km/mi.
```

---
## \#28 Posted by: ShakeNBake7000 Posted at: 2018-04-16T19:38:02.251Z Reads: 16

```
You asked if im planning to go lion or lipo, can you explain just so i understand what were talking about? i thought it was a type of battery, mine are lipos
```

---
## \#29 Posted by: RedEagle Posted at: 2018-04-16T20:42:48.373Z Reads: 17

```
You're right. They are two different types of battery chemistry. Lithium ion and lithium polymer.
```

---
