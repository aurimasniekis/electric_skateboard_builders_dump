# FlexiBMS - 0.2 HW under work - Flexible configuration and charging BMS

### Replies: 373 Views: 15619

## \#1 Posted by: SimosMCmuffin Posted at: 2018-02-11T14:23:32.045Z Reads: 740

```
Github Repo: https://github.com/SimosMCmuffin/FlexiBMS_hardware

**Connector poll on post #78** (http://www.electric-skateboard.builders/t/flexibms-poll-come-vote-on-key-design-choice-flexible-configuration-and-charging-bms/46117/78)

**First prototype KiCad project files released! #148** (http://www.electric-skateboard.builders/t/flexibms-first-prototype-kicad-project-files-released-flexible-configuration-and-charging-bms/46117/148)

**Licensing and my goals for the project #197** (http://www.electric-skateboard.builders/t/flexibms-license-discussion-come-give-your-feedback-flexible-configuration-and-charging-bms/46117/197)

So I've been working on my own BMS derivative from @raphaelchang (Raphael Chang's) Battman BMS (https://raphaelchang.com/#projects/bms). This is an announcement which I want to use to have a discussion with people about FlexiBMS and answer questions and listen to thoughts and ideas.

Anyway, who/what is this BMS for? (I'll update this list if I remember something missing from it)

* Supports 4S-12S battery stacks
* Easier and simpler charging for different battery configs with only single charger
** 12 V charger can charge 4S-12S configurations
** 15 V, 5S-12S
** 18 V, 6S-12S
** 21 V, 7S-12S
** 24 V, 8S-12S and so on
* Still supports Bulk chargers with built-in CC-CV feature. Faster charging for specific series cell battery pack configuration. (for example, a 42V 2A charger for 10S pack)
* Gives more flexibility to newcomers with their first battery packs to later change/upgrade their battery packs later without changing the BMS
* Adjustable limiting of charging power when using integrated boost charger
* Adjustable end-point voltages
* Support for multiple power switch types (momentary buttons or toggle switches)
* Balance current 100mA @ 4,20 Vcell
* Load Short-circuit detection (pre-charge voltage monitor and overcurrent detection during discharge)
* Overdischarge protection (can be pack voltage or individual cell voltage)
* Overcurrent protection
* Overcharge protection during charging (Load is still able to push current to battery for example during regen braking even if cell voltages exceed limits)
* Auto load cut off feature with configurable timeout
* Deep sleep mode for super-low standby current
* Battery storage discharge feature, for long time storage
* Audio warning and cues on configurable events (for example, cell voltage low warning when cell < 3,00)
* Status LED output for power-switch integrated or separate LEDs
* Bluetooth comms (HM-10) support for wireless diagnosis and monitoring of cell voltages and pack current during rides.
* Firmware flashing through USB via STM's built-in bootloader
* BMS configuration via USB on a graphical UI

The BMS is going to be built as 2 modules: Main module and a switch module. Main module is mandatory and will handle charging and battery pack voltage monitoring (pictured below), then if the user wants, they can add the switch module, which functions as a E-switch between the battery pack and the load and can measure discharge currents.

![image|690x339](http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/8/a/8abed220e9e642b9e4615057f76ee2559e0defd0_1_690x462.png)
![image|690x339](http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/4/149d73d6f86b279e8401a23cd3e4b141ed272007_1_690x462.png)
[details="Old concept photo:"]
![image|690x339](upload://a0BMfuHLE5gzoO9KTE0vFOxrljI.png)
[/details]


I have been testing my earlier prototype with my board's 10S5P pack and using the boost charger to charge the battery with a 16V replacement laptop power supply to 41,9 V (4,19V per cell)
![IMAG0857|690x389](upload://4uhlPJJlOdhXxdTih4YbkBjPrXZ.jpg)

Here are graphs of the pack voltage and charge current over the charging cycle:
![image|481x289](upload://w59SjODfg4CpXd4LvWSdmSQDKK1.png)
![image|478x289](upload://uJAdWKlB5ZxZzXVYOUWJh3CHZMB.png)
```

---
## \#2 Posted by: chomp Posted at: 2018-02-12T04:47:05.947Z Reads: 597

```
Very interesting. Bookmarked!
```

---
## \#3 Posted by: darkkevind Posted at: 2018-02-12T04:53:04.983Z Reads: 586

```
This is great, except we're all looking for a high current discharge BMS.... 60-120A.
```

---
## \#4 Posted by: b264 Posted at: 2018-02-12T06:37:05.909Z Reads: 564

```
Nah, most of us are only using the BMS for charging, not discharging
```

---
## \#5 Posted by: SimosMCmuffin Posted at: 2018-02-12T06:38:40.949Z Reads: 552

```
Noted.
At those currents you are most likely going to need to use a combination of multiple discharge FETs with a heatsink, a bit of a challenge/problem if you want to keep your design small.

I suppose as a concept it would be possible to split the BMS into two parts. Other one having most of the ICs and a separate module for the discharge FETs. That way you can have more flexibility in it's heatsinking design and what current it's rated continuous for.

Thoughts on this? Would rather have a big, one piece BMS unit with heftier current handling or a main BMS unit with changeable discharge module for different currents?
```

---
## \#6 Posted by: b264 Posted at: 2018-02-12T06:41:00.521Z Reads: 492

```
We'd rather have a BMS that only handles charging and is real small.  Also there can be an optional breakout board that plugs in to handle 120A discharge as well to those who don't bypass their BMS for discharging

That'd be awesome

And I see a microUSB on there at J1, does that mean charging from a phone charger?  Because that'd be awesome even if it was really, really slow
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2018-02-12T07:04:55.957Z Reads: 467

```
At this point the microUSB is only for PC comms and can't output 5V. It's regulated down to 3V3 for on-board logic, because I want the BMS to be able to be configured while only being connected to a PC without a battery. 

Now if it didn't need to be able to do that (you need to have battery connected to use USB), then I could put a 5V regulator from the battery to the USB.
```

---
## \#8 Posted by: b264 Posted at: 2018-02-12T07:06:44.050Z Reads: 454

```
No, I mean charge the battery from a phone charger, not charge a phone from the BMS
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2018-02-12T07:15:58.196Z Reads: 471

```
[quote="b264, post:8, topic:46117, full:true"]
No, I mean charge the battery from a phone charger, not charge a phone from the BMS
[/quote]

Ah, otherway around. ok.

As a concept, it's doable, but in practice I think it's going to be just too slow to be practical.

One of the main points of having the boost charger integrated into the BMS itself is the ability to buy and use inexpensive and small sized laptop chargers, which are easily carried around and can then just be plugged in to charge your board at 50+ Watts. Charging through USB in this case doesn't make enough sense to me.
http://www.ebay.co.uk/itm/Laptop-Charger-AC-Adapter-Rectangle-USB-Lenovo-IDEAPAD-G50-30/301827211694?epid=2255356376&hash=item46464dc1ae:g:4UEAAOSwwf5Zw9AA

Li-po chargers are also a bit cumbersome because they often need their own external DC supply, can often charge upto 6S only and then you need have the access to both power and balance connector to charge safely.
```

---
## \#10 Posted by: b264 Posted at: 2018-02-12T07:29:00.997Z Reads: 423

```
[quote="SimosMCmuffin, post:9, topic:46117"]
I think it’s going to be just too slow to be practical.
[/quote]

Picture 5 electric skateboards and you begin to notice how slow isn't a problem but sometimes preferred :stuck_out_tongue: 

For 1, yeah definitely too slow.  I mean we have fast charging options but flexible slow-charging options using stuff already in the home and office (and easy/light/cheap to carry in a backpack) is what we're missing.
```

---
## \#11 Posted by: SimosMCmuffin Posted at: 2018-02-12T07:43:04.721Z Reads: 411

```
[quote="b264, post:10, topic:46117"]
Picture 5 electric skateboards
[/quote]
I think at that point there are some other problems you need to be solving at that point :smile: 

Let me preface my perspective that I have done charge/discharge cycles on my board's 10S5P 600Wh battery pack and at 40 Watts it takes 15 hours (which it did). Discharge was done to 28 V and then charged back up to 41,9 V.

Now compared to USB 2, which can according to spec supply at max while using a dedicated charging port (DCP) 1,5 Amps at 5 V = 7,5 Watts + boost charger losses with big step up. I can't see it being viable, if charging a boosted board pack (~100Wh) would take over 13,3 hours at _best_.

It would start to make sense if you were using USB-C with power delivery mode which can provide 20 V @ 5 A = 100W and at that voltage the boost charger would also start to work quite efficiently.

EDIT: USB Battery Charging 1.2 (https://en.wikipedia.org/wiki/USB) support up to 5 A @ 5 V, but still 25 Watts (optimal) is not great and would need a pre-boost charger to first up the voltage for the boost charging circuit that I'm using. IMHO it's just not a good starting point for higher voltage battery charging.
```

---
## \#12 Posted by: b264 Posted at: 2018-02-12T07:55:23.143Z Reads: 371

```
Like I said, picture 5 electric skateboards that you use instead of a car, a couple on standby in case one breaks.  Because telling your boss you can't work because your skateboard broke is not okay, and polluting on the way to work is not okay either, and I don't want to deal with parking (like ebike).

There are definitely use cases; I'd like one right now :slight_smile: 

I'd say there are problems other people need to be solving, not me, because I don't emit greenhouse gases on the roadway...

Don't get me wrong, not adding the feature because it doesn't make sense is one thing, but saying nobody needs it just isn't true
```

---
## \#13 Posted by: SimosMCmuffin Posted at: 2018-02-12T08:06:37.695Z Reads: 358

```
[quote="b264, post:12, topic:46117"]
Don’t get me wrong, not adding the feature because it doesn’t make sense is one thing, but saying nobody needs it just isn’t true
[/quote]

Noted.
I'm not saying nobody would need it, but I'm advocating that there are better solutions, which would also fit better for more people (I'm guessing/assuming that most/more people would want faster charging). I'm seeing this case in this point in time, as a bit of a niche in a niche market.
```

---
## \#14 Posted by: Pimousse Posted at: 2018-02-12T09:26:37.472Z Reads: 356

```
Lithium batteries need to be charge at minimum 0.5C to protect them from bad chemical issues.
Micro-USB standard states a maximum of 2.1A current. That makes 5x 2.1A = 10.5W.
Not that much ;)

@SimosMCmuffin : did you write your own firmware ?
I'm still working on the Battman FW. My bench battery will be ready soon so the tests will start soon as well. :grin: 
I'll be more than curious to read how you coded some functions that was a pain for me (due to my lack of coding knowledge).
```

---
## \#15 Posted by: darkkevind Posted at: 2018-02-12T09:59:48.958Z Reads: 341

```
But that's because we can't find a decent small enough BMS that can handle high current right? 
We'd much prefer to let the BMS handle discharge too as it's much safer than relying on our VESCs right?
I can already find had decent small enough BMS' to handle charge only... :confused:
```

---
## \#16 Posted by: SimosMCmuffin Posted at: 2018-02-12T10:27:57.601Z Reads: 368

```
[quote="Pimousse, post:14, topic:46117"]
Lithium batteries need to be charge at minimum 0.5C to protect them from bad chemical issues.
[/quote]
This the first time I have heard of a minimum of 0.5C charge current for Lithium chemistry (this would mean I would have to charge my battery pack with ~8 amps...)
Can you link to where you read that? 

(https://www.orbtronic.com/content/samsung-35e-datasheet-inr18650-35e.pdf)
![image|690x125](upload://2OJH1ffWpLAgcwUAXBXo5rCi6qh.jpg)

Samsung charges at max 0.5C and then ramp down to 0.02C in the CV stage at which point they terminate the charging.

[quote="Pimousse, post:14, topic:46117"]
@SimosMCmuffin : did you write your own firmware ?
[/quote]
I write my own firmware for my own hardware. The current prototype has very basic firmware, mainly because it's only used to test the limitations of the hardware, so I need to able to perturb the behavior through serial Comms.

You can ask away, if you're pondering how I would code some function or a feature. I'll share my two cents.
```

---
## \#17 Posted by: TarzanHBK Posted at: 2018-02-12T10:41:55.411Z Reads: 327

```
A splitted design would be great.
Imagine a main board with like a 40A discharge and then add a second board according to your needs. Like a small addition for 60A, a medium one for 80A and a bigger one for 120A.
```

---
## \#18 Posted by: SimosMCmuffin Posted at: 2018-02-12T11:02:55.492Z Reads: 330

```
Running this through my head and thinking about the actual design challenges, it would make more sense to me to have the high side FETs and current measuring on the other module, with the main module not having any FETs on it. Mainly due to the problem of how to carry the current between both main and switch module if both of them have some high side FETs. It would be just easier to dedicate the switch module completely to the FETs.
```

---
## \#19 Posted by: TarzanHBK Posted at: 2018-02-12T11:07:03.972Z Reads: 331

```
or like that.
But it would be a problem if you want to handle charging if you want to bypass discharging wouldn´t it?
So you are required to take a second piece for that.
```

---
## \#20 Posted by: SimosMCmuffin Posted at: 2018-02-12T11:32:22.107Z Reads: 363

```
[quote="TarzanHBK, post:19, topic:46117"]
But it would be a problem if you want to handle charging if you want to bypass discharging wouldn´t it?
[/quote]

Can you reformat that sentence, because I can't figure out what exactly you mean with that?
When charger is detected -> shut off discharge FET and open charge FET.

Quick concept drawing of what is on what board:
![IMAG0859|689x390](upload://9TWTCeUPgAWIYCWbY28RxfQAygk.jpg)

You can carry through the board-to-board connector all the necessary signals and charger's charging current to battery.
```

---
## \#21 Posted by: TarzanHBK Posted at: 2018-02-12T11:37:20.501Z Reads: 321

```
sorry ;)
What i meant was that if you don´t have any fets on your main board, you definitely need to have a second board  with fets for charging.
Otherwise you´d have a small board with a 40A charge/discharge capacity, which is nice and small and enought for people to charge and bypass discharge. So that only people with higher loads need to get a second FET board.
```

---
## \#22 Posted by: SimosMCmuffin Posted at: 2018-02-12T11:46:48.070Z Reads: 317

```
If you just want to charge you don't need any FETs on the main board for that. So the main board alone could be used just for charging, if you're using the boost charger (controllable end-voltage). 

Bulk charger would present a problem, because that you can't disconnect if it for some reason was charging too fast. Then if you want more control add the Switch board and route the battery connections through it for more control.

I must say I'm a bit intrigued by this concept now...
```

---
## \#23 Posted by: SimosMCmuffin Posted at: 2018-02-12T12:18:13.252Z Reads: 349

```
I'm interested in hearing peoples thoughts on these two design/concept approaches.

**All-in-one BMS module:** 
Single board that has all the features on-board (as pictured in the first post). Battery connection is controlled. power button support. Supports both discharge and charge control and current measurement. Otherwise good approach, but non-ideal for people who want to just charge through the module under control and don't want to pay any more than necessary. Also non-ideal for high performance/current users. which the board can't support. Increasing current capability also increases price, which the charging only people are not interested in.

**Split board design**
BMS is split into mandatory _MAIN_ unit and optional _SWITCH_ unit. Main unit supports battery stack monitoring, charging  with it's dedicated charging FET and decreases entry point price for controlled charging with flexible battery configs. SWITCH unit allows for current measurement, load disconnection, power button control. Allows for flexibility in discharge current capability with bigger SWITCH units and optional heatsinking.

**Both boards support:**
 * Supports 4S-12S battery stacks
 * Easier and simpler charging for different battery configs with only single charger
 ** 12 V charger can charge 4S-12S configurations
 ** 15 V, 5S-12S
 ** 18 V, 6S-12S
 ** 21 V, 7S-12S
 ** 24 V, 8S-12S and so on
* Still supports Bulk chargers with built-in CC-CV feature, if you want faster charging for specific series cell battery pack configuration. (for example, a 42V 2A charger for 10S pack)
* Adjustable limiting of charging power when using integrated boost charger
* Adjustable end-point voltages
 * Balance current 100mA @ 4,20 Vcell
 * Overcharge protection during charging (Load is able to push current to battery for example during regen braking even if cell voltages exceed limits)
* Bluetooth comms (HM-10) support for wireless diagnosis and monitoring of cell voltages and pack current during rides.
 * Firmware flashing through USB via STM’s built-in bootloader
 * BMS configuration via USB on a graphical UI


This is not a definitive poll, but just to gauge peoples interest in what kind of BMS they would rather have?
[poll type=regular max=20 public=true]
* All-In-One BMS
* Split-Design BMS
[/poll]
```

---
## \#24 Posted by: bevilacqua Posted at: 2018-02-12T13:00:52.927Z Reads: 292

```
I think there are really only a few people who do 40A+ cont. 
Current peaks yes, but only a few seconds. 

Not even on hill climbs...
```

---
## \#25 Posted by: Pimousse Posted at: 2018-02-12T13:07:43.948Z Reads: 317

```
[quote="SimosMCmuffin, post:16, topic:46117"]
Can you link to where you read that?
[/quote]
I heard a lot from different people and also read that from here (in French, sorry) :
http://www.ni-cd.net/accusphp/theorie/charge/liion.php

[quote="SimosMCmuffin, post:16, topic:46117"]
Samsung charges at max 0.5C and then ramp down to 0.02C in the CV stage at which point they terminate the charging.
[/quote]
Of course, C rating for charging is meant for CC stage.

[quote="SimosMCmuffin, post:16, topic:46117"]
I write my own firmware for my own hardware. The current prototype has very basic firmware, mainly because it’s only used to test the limitations of the hardware, so I need to able to perturb the behavior through serial Comms.
[/quote]
That makes sense. Can't wait for the result !
Feel free to have a look at my code (not sure the latest version is commited yet) :
https://github.com/Peemouse/battman-firmware/tree/dev

I'm finishing assembling a 12S1P bench battery with unhealthy and healthy cells (to observe a bit better balancing process). I'll let you know if you're interested in.
```

---
## \#26 Posted by: SimosMCmuffin Posted at: 2018-02-12T13:21:15.778Z Reads: 298

```
http://lithiumbatteryresearch.com/Plating.php

> When the charging current is very high, as might occur during regenerative braking, the transport rate of Li+ ions to the graphite negative electrode exceeds the rate that Li+ can be inserted (intercalated) into the graphite. Under these conditions, Li+ may deposit as metallic Li, which can lead to a short circuit, degrading the battery's life and durability.

https://batteryworkshop.msfc.nasa.gov/presentations/1-Lithium_Plating_AZimmerman.pdf
![image|690x193](upload://8MLliWHAJDnCOyzli8q1E0Mc9Ik.jpg)

Quick look into the matter would suggest that plating occurs when charging current is too high, not low. Can you find any other sources confirming the low current plating?
```

---
## \#27 Posted by: Pimousse Posted at: 2018-02-12T13:52:45.798Z Reads: 272

```
Very interesting links !
I read them carefully, and no mention of low curremt causing plating.
I'll try to find more documention (or maybe find some specialists at work).
```

---
## \#28 Posted by: SimosMCmuffin Posted at: 2018-02-12T14:04:32.504Z Reads: 286

```
I just googled with "lithium charge current plating"
Those were one of the first hits.

https://trs.jpl.nasa.gov/bitstream/handle/2014/41485/08-0012.pdf?sequence=1

What I gather is that plating seems to incur at high charge rates and/or low temperature while charging.

http://www.upsbatterycenter.com/blog/lithium-plating/
> During this process, which is called intercalation, is when lithium plating takes place. There are two main reasons for this. One is the high charge current forcing the lithium ions to move at a faster reaction rate and accumulate in the surface of the anode (usually made of carbon compounds). Another reason is charging at low temperature. In this environmental condition, the reaction rate slows down thus affecting the intercalation of lithium ions.
```

---
## \#29 Posted by: Pimousse Posted at: 2018-02-12T14:27:53.853Z Reads: 266

```
Saw that article as well.
I'm focusing on plating under low charge current, but nothing really clear and studied like the over-charging.
But I still read during my search :

> The advised charge rate of an Energy Cell is between 0.5C and 1C

http://batteryuniversity.com/learn/article/charging_lithium_ion_batteries

Is it for another reason than lithium plating ?
Which one ?

Still searching. ;)
```

---
## \#30 Posted by: craj1031tx Posted at: 2018-02-12T15:43:18.510Z Reads: 261

```
So I saw that it only supports up to 6A for charging - won't that be a pretty big hindrance for braking situations? People commonly brake at between 12 and 20 amps on 12s packs, from what I've seen on the boards.

Also, since it doesn't look like we'll be getting this feature in our ESCs anytime soon, do you think it'd be possible to include a power shunt inside of a BMS for resistance heating circuit? So that we can brake at higher amps, regen charge up to a certain amperage ceiling, and then shunt the excess amperage off to a different circuit, that we can connect whatever we want to?

great design so far, and very impressive work!
```

---
## \#31 Posted by: SimosMCmuffin Posted at: 2018-02-12T15:58:26.909Z Reads: 239

```
[quote="craj1031tx, post:30, topic:46117"]
So I saw that it only supports up to 6A for charging
[/quote]
Where did you see or where did you get this number? I don't think I have mentioned that anywhere.
```

---
## \#32 Posted by: craj1031tx Posted at: 2018-02-12T16:01:18.349Z Reads: 233

```
It's in the "Features" section on his blog post:

"Boost converter circuit with adjustable voltage for CC/CV charging at up to 6A"

There are a lot of words in that post that I don't understand though, so maybe I misinterpreted this sentence and it can in fact support higher charge currents for braking events, and this statement only applies to wall charging...?
```

---
## \#33 Posted by: SimosMCmuffin Posted at: 2018-02-12T16:06:12.110Z Reads: 243

```
Ah, yes. Thanks for the context.

So the 6 Amps is the maximum input current for the boost converter, which you connect your charger into. As I mentioned in the original post, I have been testing the boost converter by charging my battery with a 16V replacement laptop power supply. The boost converter takes the 16V and then "boosts" it up to a controllable voltage, which allows me to charge my 10S battery pack from 29V to 41.9V.

It doesn't affect the max current the motor controller can pump back into the battery during regen braking through the discharge FET.
```

---
## \#34 Posted by: craj1031tx Posted at: 2018-02-12T16:43:41.238Z Reads: 238

```
Ahhh, OK, noted. Having a transformer on board is a really great feature, that would be fantastic. Thanks for clearing that up!
```

---
## \#35 Posted by: SimosMCmuffin Posted at: 2018-02-13T07:52:11.995Z Reads: 265

```
Ok, so I'm gonna do a concept PCB design for the split-design and post updates as I get more progression to get more thoughts. I spent a little time last evening fleshing out the idea, looked for components to actually execute it and made a better block graph for it how it would actually work wiring wise.
![IMAG0860|689x390](upload://hCsOvwHTyIK7RjGCBUiNkZvaeuT.jpg)

**I'd appreciate more votes on the POLL though!** (http://www.electric-skateboard.builders/t/poll-announcement-flexible-configuration-and-charging-bms/46117/23)
```

---
## \#36 Posted by: lox897 Posted at: 2018-02-13T10:48:44.901Z Reads: 252

```
Wow! Nice work! Keeping my eyes on this thread.
![u1|500x500](upload://d7xFgc0osA1pkHpUMroQ00IXcFb.jpg)
```

---
## \#37 Posted by: Pedrodemio Posted at: 2018-02-14T00:21:50.955Z Reads: 243

```
I also never saw that mentioned before, but saw a few times in forums that low charge current don’t do bad to the battery

This is the same when people say that float charging damages the battery (Lithium), true float damages because it switches again to CC after the CV phase, but keeping the CC until it goes exponentially to zero doesn’t have an influence on life

I think the best argument against the 0.5C recommendation is Tesla, take the S 100D, it comes with a 17.3kW charger, that’s approximately 0.2C, or even less since you can set lower in car, and I bet they are the company that have the most of real world data about 18650 batteries


@SimosMCmuffin do you think your firmware would be compatible with @raphaelchang hardware? Quite a few people including myself have a 100 USD dead weight

If you managed something in the same size as the original, I had the exactly space reserved for it in my board that’s is now occupied by an anti spark and cheap Chinese charge only BMS
```

---
## \#38 Posted by: SimosMCmuffin Posted at: 2018-02-14T06:55:29.195Z Reads: 256

```
[quote="Pedrodemio, post:37, topic:46117"]
If you managed something in the same size as the original,
[/quote]
Going to be tricky, Added to that is the fact that I have bigger components on the board due to the beef'd up boost converter (bigger inductor, double diodes and input/output el.caps). Okay, I don't have the discharge FETs or high current pathways, but I need the connector for the Add-on Switch-module. 

At this point, I can't really promise anything on the form factor as I don't have layout even mocked up to see what's the smallest area or shape I can go. Plus I don't actually have practical test data on the new board too see if the layout works properly IRL.

[quote="Pedrodemio, post:37, topic:46117"]
@SimosMCmuffin do you think your firmware would be compatible with @raphaelchang hardware? Quite a few people including myself have a 100 USD dead weight
[/quote]
Different microcontrollers. Battman has STM32F**303**CBT6, I'm planning on using STM32F**070**CBT6 + different peripheral connections, at least pin out wise.
What's the problem with the original firmware? Does it now work at all, or does it work badly? The thing is open source, so you could code your own basic firmware for it to make it work.
I'm going to prioritize my own firmware first and once that's working, then maybe port it with a basic feature set to the Battman, so people can at least get use out of their hardware.

EDIT: Could you take measurements of the Battman board? 
![image|690x257](upload://fP2qOuliHQ815EQQYD04woFcwpL.jpg)
```

---
## \#39 Posted by: Pimousse Posted at: 2018-02-14T08:38:46.287Z Reads: 253

```
The actual firmware allows us to use Battman only as a basic Vedder powerswitch.
I already code a lot of features now and I'm glad that @Pedrodemio will join the coding process :slight_smile:
The size of Battman is pretty compact but if I could rework it, I'd make it a bit bigger to allow more space between neg and pos battery and output leads (they are verryyyy close from each other :confused: )

![IMG_20171023_223238|666x500](upload://ePfYYd467nwvQa3byeJlEFjzKmr.jpg)

Making a small BMS is a real challenge. DieBieMS isn't small either, for good reasons I guess.
```

---
## \#40 Posted by: TarzanHBK Posted at: 2018-02-14T08:50:20.911Z Reads: 246

```
Yah these wires tend to shorts!
A cool BMS doesn´t have to be extremly small, i think the DieBieMs seems to have a great size. Others like my first China BMS are taller than my battery and are about 25cm long :smiley:
Smaller is of course nice to have, but it´s totally fine to have all the cool features and the size of a batterysupport bms.
```

---
## \#41 Posted by: SimosMCmuffin Posted at: 2018-02-14T10:15:23.138Z Reads: 229

```
I'm planning on putting the mounting holes of the same M5 screw terminal that DieBie uses into the terminal pads on the Switch-module, but also allowing the wires also to be soldered into the pads if the screw terminal isn't fitted. You know, as an option. Those screw terminals aren't exactly cheap.
https://media.digikey.com/Photos/Wurth%20Electronics%20Photos/7460408_sml.jpg
https://www.digikey.fi/product-detail/en/wurth-electronics-inc/7460408/732-3208-ND/2682499
```

---
## \#42 Posted by: Pimousse Posted at: 2018-02-14T10:38:22.012Z Reads: 219

```
IIRC, thos screw terminal need to be installed by pressing.
So you need the specific tool for this process. That might complicate the manufacturing thus higher cost.
```

---
## \#43 Posted by: SimosMCmuffin Posted at: 2018-02-14T10:43:08.502Z Reads: 234

```
They are press fit, so as long as the footprint for them is designed properly (hole size correct with plating) and hasn't been contaminated with solder they should work.
http://katalog.we-online.de/em/datasheet/7460408.pdf

EDIT: There are also other options available from Wurth
Surface-mount
![image|200x200](upload://A1wr8olXKIwGszhAZft4BATnLNK.jpg)
https://www.digikey.fi/product-detail/en/wurth-electronics-inc/7466005R/732-10900-1-ND/6644306
Though-hole
![image|200x200](upload://bQJyNfA2j8sOePzwvtmgBGABKPV.jpg)
https://www.digikey.fi/product-detail/en/wurth-electronics-inc/74650094R/732-10884-1-ND/6644295

But anyhow, I want at least to offer the possibility of using a screw terminal.
```

---
## \#44 Posted by: SimosMCmuffin Posted at: 2018-02-14T10:53:03.814Z Reads: 231

```
This new board is gonna be quite busy, not sure if I'm gonna have to increase size width wise, but current board outline is 65 x 35 mm. Will update more as this progresses.
![image|690x389](upload://7vppgqDz4LaWDs8qvS42gLJDszo.png)
```

---
## \#45 Posted by: Pedrodemio Posted at: 2018-02-14T12:45:28.186Z Reads: 229

```
Thanks, no worry’s, as @Pimousse said we are trying to make it work at least on basic, he already recoded a lot of stuff but I’m never messed with STM, so im trying to learn as we go

As soon as I got my hand on the BMS I will measure, it I’m not mistaken the height is the same or a little bit less than the Vedder anti spark
```

---
## \#46 Posted by: SimosMCmuffin Posted at: 2018-02-14T16:55:28.081Z Reads: 246

```
Well I got everything on the board, haven't routed anything yet though. There is still space for optimization (free space available as seen in the pictures around the MCU) and I need to re-wire some of the MCU pins around for better placement, but I don't think the board is going to get smaller because the connectors can't fit in.

Couple notes about the connectors:
**A**: Battery connection. Solderable, fits a XT60-connector or 2 terminal quick connect (pictured below)
**B**: Charger connection. Solderable or 3 terminal quick connect (pictured below,sizewise identical placeholder in the picture), can hookup both boost converter and bulk charge ports at the same time. (Bst_charger - GND - Blk_charger)
**C**: Bridge connector to Switch-module, 16-pin. Will carry charging current (not regen current) when using switch module, so no need to connect battery to the Main-module, expect for the XH-balance connector. 
_There is a key design decision to do with this connector that I will post about tomorrow for your guys' thoughts._
![image|200x200](upload://lCPP8lE06ItzSVuVGcuzTWSQwJp.jpg)![image|200x200](upload://1iVnPipMLe4S2prolfGsbV6tVn3.jpg)
![image|690x462](upload://8QkYuooCO4Ojgt84VS0tlBky490.png)
![image|690x305](upload://vpdtWMILNfP4zOd6KZZA79rXZ7h.png)
![image|690x462](upload://eTOMOccthxwD7OdUSAgfVrQmrgi.png)
```

---
## \#47 Posted by: Pimousse Posted at: 2018-02-14T17:15:20.090Z Reads: 218

```
Not sure about screw terminals.
The board will be exposed to shocks and vibration that may lead to unscrew the non-locked terminals.
In the industry we tend to replace them by spring terminal to lower the failure rate due to untighten screws. :)
```

---
## \#48 Posted by: SimosMCmuffin Posted at: 2018-02-14T17:28:50.181Z Reads: 213

```
These are the particular terminals I was looking at using
https://www.digikey.fi/products/en/connectors-interconnects/terminal-blocks-wire-to-board/371?k=OSTTE020104

[quote="Pimousse, post:47, topic:46117"]
In the industry we tend to replace them by spring terminal
[/quote]

It does say in it's properties "Screw - Leaf Spring, Wire Guard". I haven't used a lot of screw terminals in my own projects and not in anything with vibration, so I can't say if these would work? I'll wait for your opinion on them.
```

---
## \#49 Posted by: Pedrodemio Posted at: 2018-02-14T18:34:54.213Z Reads: 200

```
I just didn’t like the terminal block (B) in my opinion is wasted space, to the sides and up, would be better if the BMS could be 18mm thick with wires to fit in thinnest of the enclosures 

Also, what pitch are you using for the balance connector? Appears to be 2.54mm, the VESC uses 2mm and it makes a big difference with lots of pins
```

---
## \#50 Posted by: SimosMCmuffin Posted at: 2018-02-14T18:47:31.932Z Reads: 228

```
[quote="Pedrodemio, post:49, topic:46117"]
I just didn’t like the terminal block (B) in my opinion is wasted space, to the sides and up, would be better if the BMS could be 18mm thick with wires to fit in thinnest of the enclosures
[/quote]

The B connector in the 3D PCB picture is just a placeholder that has roughly the same size (not in vertical) as the one I'm going to be using, as pictured below:
![image|200x200](upload://o0vL5ljtR75u3vEB1oVi6PALYIc.jpg)
![image|500x500](upload://t57FuLlofR5yu3LtCYh0awVIhqn.jpg)
![image|500x500](upload://5QxSHP8uNZiTqHru98t2Y7LzpU3.jpg)
It's not very tall, in fact it's pretty compact. You can still not fit it and solder your charge port wires on.
https://www.digikey.fi/product-detail/en/on-shore-technology-inc/OSTTE030104/ED2741-ND/2351817

[quote="Pedrodemio, post:49, topic:46117"]
Also, what pitch are you using for the balance connector? Appears to be 2.54mm, the VESC uses 2mm and it makes a big difference with lots of pins
[/quote]
Balance connector is the standard Li-Po balance connector: JST's XH-series, 2.5 mm pitch.
```

---
## \#51 Posted by: PXSS Posted at: 2018-02-15T04:17:32.539Z Reads: 198

```
What boost converter are you planning to use? What are the specs? Sounds interesting :)
```

---
## \#52 Posted by: SimosMCmuffin Posted at: 2018-02-15T06:57:50.818Z Reads: 223

```
The overall setup is very similar to the Battman implementation, but having benchmarked it with thermal analysis (FLIR IR-camera) I found it to be running very hot. And that was with a lower max peak current, it would still easily reach over 100 Centigrade, sometimes even 140 C, not ideal longevity wise and having it in a closed battery enclosure next to the cells, didn't jive with me.

So I decided to lower the losses with it, to make it run cooler and allow a bit more current also. Biggest losses were the inductor's resistive losses and the diode loss. So I beefed up the inductor, that changed the nominal DC resistance of it from 74 mOhm -> 25.7 mOhm and changed the schottky diode from the 120V model to 60V model that has lower forward voltage at higher currents and also placed two of them side-by-side to spread the heat to a larger area to increase cooling.

Input and output capacitors were changed to electrolytic caps to reduce voltage ripple.

I also added an extra measure of security with a watchdog circuit that disables the boost circuit in case the MCU becomes unresponsive. Actually with the changes to the schematic that watchdog circuit would serve better at the charge FET to disable that in case the MCU becames unresponsive. This would then also protect in a case where the battery is being charged via a bulk charger... yea I'll make that change.

I have also placed a NTC temperature measuring point next to the boost converter, so I can monitor it's temperature in the MCU.
Battman:
![image|690x373](upload://1lgNXzyAI5gASHqQuZYS9a6Fqpa.png)
Mine:
![image|690x304](upload://yFCSh7xxjMGgTJh5AzLKuDiws6a.png)

I need to check one of the shunt resistor values at home before I can give any accurate performance numbers on my current prototype, but the charging test wtih my 10S5P battery pack indicated ~40 Watt average charging power with the 16V laptop charger as the input source.

EDIT:  I just checked the Battman boost converters output capacitor, which is a 180µF, 50V, so it might actually go atmospheric if you were to try to charge a 12S pack to full voltage (50,4V). I'm using a 100µ, 63V cap.
```

---
## \#53 Posted by: Pimousse Posted at: 2018-02-15T07:52:30.143Z Reads: 207

```
I think that what they call leaf spring is the part in red below :

![Capture|299x425](upload://2gx5ddCOt0dfnFOQopfWMxOd47u.PNG)

So the only tighten element is the screw.
And for such high current, I wouldn't rely on screw terminal.
In industry, part of electrical maintenance is to tighten screw of terminals and check all connections with thermal vision (iFLIR often :smile: ) because an untighten screw of a power cable will heat a lot and sometimes ignite the whole cubicle (or melt everything around in the best case).

This is only my industrial point of view which may not comply with electronics project.
If @JTAG chose this kind of component, I guess he knows the pros/cons and did this choice for good reasons. :)

[quote="SimosMCmuffin, post:52, topic:46117"]
EDIT:  I just checked the Battman boost converters output capacitor, which is a 180µF, 50V, so it might actually go atmospheric if you were to try to charge a 12S pack to full voltage (50,4V). I’m using a 100µ, 63V cap.
[/quote]

:open_mouth: :open_mouth:
Wait... I'm not far to test my Battman FW with a 12S, including charging/balancing feature.
Fu@$ ! That's a bit strange though because he tested it (there is a video of balancing on his YT channel).

Thanks for pointing the weakness of the Battman anyway !
I've put lot's of hope into it, I'm pretty disappointed.
Mostly after tens and tens of hours spent (wasted ?) into it. :disappointed_relieved:
```

---
## \#54 Posted by: SimosMCmuffin Posted at: 2018-02-15T07:56:29.798Z Reads: 188

```
[quote="Pimousse, post:53, topic:46117"]
And for such high current, I wouldn’t rely on screw terminal.
[/quote]

The terminals on the Main module are only used for charging so at max around 6 amps I would ball park. The terminal is rated for "Current	10A", so it is in spec. A loose connection is a loose connection and that is user error at that point, but you can still order your BMS without the screw terminals and just solder your wires directly to the board. It's just an option that I'm planning on, of course I'm going to test if they work and then based on the tests see if I continue supporting them or not.
```

---
## \#55 Posted by: b264 Posted at: 2018-02-15T09:34:34.090Z Reads: 183

```
[quote="Pimousse, post:42, topic:46117, full:true"]
IIRC, thos screw terminal need to be installed by pressing.

So you need the specific tool for this process. That might complicate the manufacturing thus higher cost.
[/quote]

Just put them in the package and let the user install them LoL
```

---
## \#56 Posted by: JTAG Posted at: 2018-02-15T10:46:35.729Z Reads: 177

```
ARE YOU CALLING MY BMS TO BIG :sob::sob::sob::sob::sob::sob:? You are right, it is kinda big... maybe :sweat_smile:. Well, with the current functionality if you want to keep it single sided it is a challenge to make it smaller.
```

---
## \#57 Posted by: JTAG Posted at: 2018-02-15T11:01:55.618Z Reads: 189

```
[quote="SimosMCmuffin, post:52, topic:46117"]
lso placed a NTC temperature measuring point next to the boost converter, so I can monitor it’s temperature in t
[/quote]

I am not sure whether I overlooked it or not; what cell voltage monitor are you using? The LTC I use has a build in watchdog and has GPIO's that reset (to a known state) when the uC stops communicating, I use this GPIO WD combination as an extra safety feature to disable / enable the charge / discharge ports (like you suggest to do as well). 

@Pimousse from past hobby projects and bug fixing of other projects I found that these type of screw terminal (if bought cheap or just in general) tent to introduce PCB traces / pads to break right next to the point where they are soldered (due to the extreme high mechanical stresses from the screw driver action and the mounting method, it is only a single pin in a small hole), so make sure to make a really beefy solder pad for these terminals. 

I use press fits just because they are really friendly during the assembly / disassembly process, also mechanically very very strong. But indeed, they are way to expensive xD.
```

---
## \#58 Posted by: SimosMCmuffin Posted at: 2018-02-15T11:28:40.522Z Reads: 182

```
[quote="JTAG, post:57, topic:46117"]
The LTC I use has a build in watchdog and has GPIO’s that reset (to a known state) when the uC stops communicating, I use this GPIO WD combination as an extra safety feature to disable / enable the charge / discharge ports (like you suggest to do as well).
[/quote]
Ah, I had completely forgotten about the battery stack monitor's watchdog! The particular model I'm using is LTC6803-3. I need to check it's watchdog pin functionality, I think it was open collector while active, so I could use it to pull down the gate of the activation FET for the charge FET. I could then ditch STWD100 watchdog IC.

[quote="JTAG, post:57, topic:46117"]
from past hobby projects and bug fixing of other projects I found that these type of screw terminal (if bought cheap or just in general) tent to introduce PCB traces / pads to break right next to the point where they are soldered (due to the extreme high mechanical stresses from the screw driver action and the mounting method, it is only a single pin in a small hole), so make sure to make a really beefy solder pad for these terminals.
[/quote]

Good to know. I'm gonna try them in the first iteration and if they feel/seem like complete nuggets I'm gonna abandon them and possibly look for another solution, but space is pretty limited.
```

---
## \#59 Posted by: JTAG Posted at: 2018-02-15T11:47:14.312Z Reads: 191

```
I was attempting to explain it but it got lengthy and messy. If you look in my schematic it is the "SAFETY" wire. The LTC is pulling it low when everything is ok, when there is nothing communicating is resets and goes high.

![image|690x367](upload://bCqebiiA8P4qhtKrAbEh41BXcJF.png)

And if high the fets wont allow the uC to enable the fet driver:

![image|690x415](upload://3hpWhUVQRPRm9ozIuSXyeByuV0Y.png)

Stupid but simple, should never be used. It did save me a couple of times during bebugging when I put a breakpoint somewhere and the LTC protected me from overcharging :P.
```

---
## \#60 Posted by: SimosMCmuffin Posted at: 2018-02-15T12:27:34.262Z Reads: 183

```
in my case I can't use the GPIO pin as the watchdog pin, because they float when logic high, which is the default state when reset or the watchdog runs out. I could replace the watchdog circuit with the WDTB pin from the LTC6803, so it pulls the gate low if the MCU hangs or doesn't communicate with the LTC6803. I could then drive the gate otherwise with the LTC6803's GPIO either on or off.
![image|690x411](upload://m6dGcR1pElCWfE0ozXN6DCrD4fp.png)
```

---
## \#61 Posted by: SimosMCmuffin Posted at: 2018-02-15T12:51:19.848Z Reads: 186

```
I came up with a simple solution that removed some unnecessary components and traces. On the LTC6803 GPIO and WDTB are connected together, with a pull-up. That connection is then passed to the Charge_FET control. If MCU hangs the WDTB is asserted and pulls the line low. Then when MCU controls the LTC6803 I can switch the GPIO pin to either pull the line down or let the pull-up pull it high.
![image|583x500](upload://aUwo6XP6qBQiF82h6atgXOWlatZ.png)
![image|550x500](upload://vd5aNd3FSw4ajtRcqjRkwuGSpGQ.png)
```

---
## \#62 Posted by: PXSS Posted at: 2018-02-15T12:54:07.669Z Reads: 171

```
Why not create a open source programmable charger instead? Why do we need all of this on board? 

I imagine this:
https://www.amazon.com/dp/B00B3C2Z52/ref=cm_sw_r_cp_api_vbyHAbFE6SG66
+
A boost converter module with nice lcd interface would be perfect to charge anything from 4-12s maybe even higher!

Then your BMS only gas to do the basics, protect from ov/uv/oc & balance when charging if dv>100mv between highest cell and lowest cell. It could be really small. You could make it even more modular and separate the balancing into a different module. In this scenario, you could have the balancer within the charger too and you're down to crucial protection components on board. 

I am really looking forward to this project regardless of the approach
```

---
## \#63 Posted by: Pimousse Posted at: 2018-02-15T13:04:31.705Z Reads: 176

```
[quote="JTAG, post:56, topic:46117"]
ARE YOU CALLING MY BMS TO BIG :sob::sob::sob::sob::sob::sob:? You are right, it is kinda big… maybe :sweat_smile:. Well, with the current functionality if you want to keep it single sided it is a challenge to make it smaller.
[/quote]
Sorry for that
I'm meant... bigger ? not big :grin:

Thank you guys for this electronics porn ! :slight_smile: 
WDTB on Battman is not used (at least, that's what I'm understanding).
Your safety feature is really smart JTAG !
```

---
## \#64 Posted by: SimosMCmuffin Posted at: 2018-02-16T07:56:25.058Z Reads: 200

```
Ok, key design choice time (Poll at the end). The module interconnector, AKA the connector that connects the Main- & Switch-modules together. I have **two styles** picked up and I'm going to explain the differences between them and then shortly go through the pros and cons with each approach. _(Switch-module design hasn't been started yet, so upcoming pictures are mock-ups_)

![image|690x389](upload://74rBlKxne9Od7vbZHTLnbEBRFVT.png)

Why aren't these two styles compatible with each other? It's because they flip the pin order in relation between them, as demonstrated below.
![image|690x261](upload://dfROhfaKaQK1aaUtQXw5Uv5fyTw.png)
![image|690x254](upload://5RpmsTg678mv6q1GmN34wGWBCcH.png)

----

Let's start with a closer look at **Style B** connector.
Male: (https://www.digikey.fi/product-detail/en/sullins-connector-solutions/SBH11-PBPC-D08-RA-BK/S9179-ND/1990072) 
Female: (https://www.digikey.fi/product-detail/en/sullins-connector-solutions/SFH11-PBPC-D08-RA-BK/S9204-ND/1990097)
![image|200x200](upload://68ihfD9aJnpkl4qt1NMAKKBKiOm.jpg)![image|200x200](upload://eytbzaUkP0LhtOHpVIluk2DiuF3.jpg)

Pros:
* Simplest and easiest way to connect the modules together

Cons:
* Wasted space as the board edges can't touch each other. Gap caused by the connector housing.
* No any kind of flexibility in positioning between the modules
![image|690x249](upload://cSHVFQNoWBuZssCHW5UQTlX6eUQ.png)

**Style A** connection:
Board side: (https://www.digikey.fi/product-detail/en/sullins-connector-solutions/SBH11-PBPC-D08-ST-BK/S9171-ND/1990064)
Connector side: (https://www.digikey.fi/product-detail/en/sullins-connector-solutions/SFH210-PPPC-D08-ID-BK/S9288-ND/2095297) or (https://www.digikey.fi/product-detail/en/sullins-connector-solutions/SFH11-PBPC-D08-ST-BK/S9196-ND/1990089)
![image|200x200](upload://pYVWXT2U9e2Iy89GUwNc8PdxZna.jpg)![image|200x200](upload://dHYsvDoX3sGaXoYRvrt5FxmAVMV.jpg)![image|200x200](upload://tVxtjGZgnyYm2yhBMHEJgaEGaU1.jpg)

Pros:
* Allows modules to be touching each other with a bridging PCB that has female headers on it. Almost no wasted space. (error in picture text, bridge PCB has female connectors)
![image|690x309](upload://upkYo2OqZXo5oN9FReUnED1G3DY.png)
* Option to use ribbon cable with IDC-connectors at the end allowing flexibility in positioning and different mounting angles between the modules. (Ribbon cable has to carry only charging current, which is carried by 4 wires in each direction)
![IMAG0861|690x442](upload://eu6nfFZ0nsoW1Yj9YrqdA5cVnbq.jpg)

Cons:
* Needs extra parts to connect modules.
* Needs a bit more vertical room
---
**There**. Short explanation between the connector styles, why they aren't cross-compatible and short pros & cons for both. I'll discuss about this with you or answer questions and update the Pros & Cons list if good points are made. Other connector suggestions are also welcomed.

I'm naming this project from this point onward under the alias **"FlexiBMS"**

----
**Poll below has it's voting descriptions mixed-up in contradiction to the info above, which are correct. Options should be:
Style A, Extra connector, allows for optimized space use, or more freedom on module positioning
Style B, Simple and easy, with a bit of wasted space**
[poll type=regular public=true]
* Style A, Simple and easy, with a bit of wasted space
* Style B, Extra connector, allows for optimized space use, or more freedom on module positioning
[/poll]
```

---
## \#65 Posted by: SimosMCmuffin Posted at: 2018-02-18T15:30:15.069Z Reads: 184

```
**OH CRAP! I just now noticed I have my poll options are mixed up. I'll fix the descriptions, if I can and holla to the voters to check their vote. Sorry for the mix-up**
![image|650x222](upload://y68OQ34MPQI6TPL5z6bjGdFux59.png)


**Update**. Board routing is done. I'm going to do some sanity checks to see if I have missed anything critical, but otherwise we're starting to look good for the first iteration prototype.

I'm also adding one more useful feature, which allows the module to put itself into deep shutdown state, essentially cutting it's power use almost completely for long term storage, so it doesn't drain the battery pack empty. The amount of time before the module disables itself will be configurable, for example, "if nothing happens in 15 days" -> "shutdown". Wake-up is done via  a pushbutton. You will also have to wake-up the module when you connect the battery pack, but it will then run on the shutdown timer.

![image|690x462](upload://iuaDkPBgQrKgqw12wJoDbiMA9L.png)
![image|690x462](upload://rqDeTqAuWgjAMlqVHxAB1SicG6r.jpg)

Sorry about this, but could following users check their voting choice on the post #64 poll, knowing that the connector descriptions were mixed-up
@Freddiecook @rene @bevilacqua @b264 @louwii @riva_00 @GrecoMan @JonathanLau1983 @TarzanHBK @ShutterShock
```

---
## \#66 Posted by: rene Posted at: 2018-02-18T16:56:14.067Z Reads: 169

```
I like the extra connector and voted what was stated in the vote option - not the intro.
```

---
## \#67 Posted by: b264 Posted at: 2018-02-18T20:57:44.075Z Reads: 176

```
I voted based on the image, not the text, for style A.  I'm still not sure exactly where the mixup was.  You should make a new poll so you can keep track of who voted again and who may not have understood

![image|690x261](upload://dfROhfaKaQK1aaUtQXw5Uv5fyTw.png)
![image|690x254](upload://5RpmsTg678mv6q1GmN34wGWBCcH.png)
```

---
## \#68 Posted by: JTAG Posted at: 2018-02-18T23:30:14.346Z Reads: 164

```
Is the schematic already published somewhere or should we wait :grin:?
```

---
## \#69 Posted by: ShutterShock Posted at: 2018-02-19T01:42:33.796Z Reads: 167

```
Oh yeah I voted based on the picture too.
```

---
## \#70 Posted by: SimosMCmuffin Posted at: 2018-02-19T06:28:55.107Z Reads: 161

```
Schematic is not yet released, but I intend to make it public once I complete the sanity checks on it. Probably on this week though.
```

---
## \#71 Posted by: SimosMCmuffin Posted at: 2018-02-19T06:32:25.579Z Reads: 159

```
Also @ShutterShock 
Did you vote based on, if the connector was vertical or horizontal like in the pictures?
```

---
## \#72 Posted by: ShutterShock Posted at: 2018-02-19T07:16:50.592Z Reads: 157

```
I was thinking vertical connector with a short ribbon cable, I think it is more flexible :slight_smile:
```

---
## \#73 Posted by: Pimousse Posted at: 2018-02-19T07:36:00.095Z Reads: 165

```
Style A is meant to allow stacking both boards ?
Erf, both stles have their pros and cons.
What about "Style C" with vertical pin but not crossed ?
Is the length between boards critical ?

Also I guess it's more convenient to have the USB port vertically like VESC 6.
Our enclosure are often messy, lot's of components/wires everywhere so it's not that easy to plug a USB cable on the side.
```

---
## \#74 Posted by: b264 Posted at: 2018-02-19T07:38:17.965Z Reads: 155

```
The connectors could always be unsoldered and changed if desired
```

---
## \#75 Posted by: Pimousse Posted at: 2018-02-19T07:40:27.563Z Reads: 153

```
Sure, but the PCB layout will changed between crossed and not crossed style, right ?
```

---
## \#76 Posted by: b264 Posted at: 2018-02-19T07:41:30.997Z Reads: 155

```
Yep, good call
```

---
## \#77 Posted by: SimosMCmuffin Posted at: 2018-02-19T07:43:43.033Z Reads: 173

```
**This ^^**

I'll make a new poll shortly with new images to demonstrate the styles clearly.
```

---
## \#78 Posted by: SimosMCmuffin Posted at: 2018-02-19T08:15:29.216Z Reads: 200

```
Okay. New connector poll time. with hopefully better pictures this time.

Here are our mock-up boards.
![image|497x500](upload://lLGr56nm31WgF5XoMTIAvru3l2s.png)

----
**Vertical connectors:**

![image|533x500](upload://mPrR3wAQTFJQcZY75D7osc2XcYn.png)
Boards can be right next to each other with a connector PCB, like so:
![image|302x500](upload://wpBhpKD8uGaUzBccK9IRtkLjMXB.png)
Or you can use a reasonable length ribbon cable to have some distance and angle between the boards, like so:
![image|617x500](upload://iqgb2iV9CHd3ZXWOAJppTg4ZMIa.png)
FYI, this is a ribbon cable:
![image|690x442](upload://d4I1m3AhihiWrDSTnXFKwsF3iYM.jpg)

----
**Horizontal connectors:**
![image|603x500](upload://3QYibxjK1riODIAvYiGvvsC9rza.png)
Simpler with no additional parts needed to connect the boards. There will be a gap left between the boards, like so:
![image|508x500](upload://fbBIcVN9PFjolauJdWtSK81S3dN.png)

---
**I would like to use:**
[poll type=regular public=true]
* Vertical connectors
* Horizontal connectors
[/poll]
```

---
## \#79 Posted by: Pedrodemio Posted at: 2018-02-19T12:07:18.790Z Reads: 179

```
@SimosMCmuffin I like where this is going, with the ribbon The flexibility increases a lot since you can cram the power board somewhere else

About the balance port, couldn’t it also be vertical? If reduces the footprint a bit but reduces the used space a lot since there are no wires going to the side
```

---
## \#80 Posted by: SimosMCmuffin Posted at: 2018-02-19T12:10:45.004Z Reads: 182

```
The vertical connector should just about fit without any changes. User choice?
![image|690x389](upload://bAHOP0fULXTN1jALNpyMtsudtTh.png)
```

---
## \#81 Posted by: Pedrodemio Posted at: 2018-02-19T12:11:17.817Z Reads: 174

```
Best of both worlds, since we touched the topic, a vertical usb would also be better suited for onboard programming

Thanks
```

---
## \#82 Posted by: SimosMCmuffin Posted at: 2018-02-19T12:15:28.889Z Reads: 168

```
I'm looking at the possibility of using double footprint for that as well, so it can fit either horizontal or vertical connector.

EDIT: Yes, it's possible to stack the footprints
```

---
## \#83 Posted by: TarzanHBK Posted at: 2018-02-19T12:49:19.637Z Reads: 166

```
I think it doesn´t matter much because you have the battery tabs on this side too - so a ballance connector this way shouldn´t use much more space.
```

---
## \#84 Posted by: SimosMCmuffin Posted at: 2018-02-19T13:04:18.867Z Reads: 175

```
I would call this board "somewhat" busy
![image|690x398](upload://9UkhKlcbaDVQgpYPwFUKOAallXB.png)
```

---
## \#85 Posted by: JTAG Posted at: 2018-02-19T14:40:59.192Z Reads: 169

```
Thanks, if you would like me to look at your schematic I would love to! Good work anyways ^^!

Am I overlooking the CAN transceiver or is it intentionally left out?
```

---
## \#86 Posted by: SimosMCmuffin Posted at: 2018-02-19T15:41:30.950Z Reads: 166

```
No CAN at the moment and there isn't space on the board to add it. I'm intending the main comms to be the HM-10 type bluetooth modules (serial bridges) during a ride, but I'm not explicitly saying that CAN can't be added in some future iteration, if people request it.

I think there is enough un-tested stuff on this iteration to do a board :wink:
```

---
## \#87 Posted by: Pedrodemio Posted at: 2018-02-19T16:29:21.956Z Reads: 165

```
With serial would be easy to hook it to an arduino or similar right? Having all info on the remote would be great, pack temperature, energy used, individual cell voltage
```

---
## \#88 Posted by: b264 Posted at: 2018-02-19T16:39:52.023Z Reads: 163

```
I would not overcomplicate version 1, let's see how it works first and how the community responds
```

---
## \#89 Posted by: SimosMCmuffin Posted at: 2018-02-19T16:40:40.905Z Reads: 160

```
It's a standard USART bus, RX and TX lines that work with a certain baudrate. Can be an arduino on the other end for example. The USART pins on the STM32 are also 5V tolerant, so 5V arduino won't blow them up, although if you're taking power also from the module, it's 3,3V.
```

---
## \#90 Posted by: SimosMCmuffin Posted at: 2018-02-19T16:57:34.400Z Reads: 164

```
Some info on the shutdown/wake-up logic on the board: 

I have implemented it in a way, that allows the MCU to shut off the 3V3 regulator (which consumes relatively large amount of current, even with no load) completely, which then also shuts down the 3V3 supply. **The MCU is not in hibernation, it is off**. In this state the module should use less than 100µA of current, which is about 90 times less than in normal standby mode. **The only way to wake-up the board is to use an on-board button**, which essentially re-latches the 3V3 regulator back online and the MCU can then keep itself powered up.

The reason I want this feature is to protect the battery from a deep discharge when for example putting it in winter storage or other such thing. I intend to add to software configuration to allow to set the time before the module goes to deep sleep and would also allow to discharge the battery to storage voltage after the module would turn itself off.

Thoughts?
```

---
## \#91 Posted by: b264 Posted at: 2018-02-19T17:08:53.435Z Reads: 158

```
Please, please make the default delay for entering sleep mode at least 10 hours.  That will still protect from deep discharges.  Also is it possible for it to be disabled if the charge port has power?

Certain commercial boards, ahem Evole, go into sleep mode after like 4 minutes or something, it's even happened at traffic signals before.  It's ridiculous, super-annoying, and dangerous
```

---
## \#92 Posted by: Pimousse Posted at: 2018-02-19T18:20:38.461Z Reads: 166

```
Great improvements ! I like the way you make it collaborative ! Thank you for that !
Few inputs :
- Please put the CAN !!! I think it's even better than UART as you can use the CAN forward command of the VESC to dial with the BMS using only the BLE of the VESC. I wouldn't add another BLE module just for BMS plus the one for the VESC although we can use the same one.
And it's not a big deal to integrate a communication between BMS and VESC to switch power off smoothly in case of low voltage on a cell or whole battery.
-Shut off mode is great ! As @b264 said, of course it needs to be hours unit for sure. Dn't you want to get inspiration from the Battman design for that ? I found the power management pretty well designed.

- May you tell the interface passing between 2 boards (main and power) ? Which signals are exchanged ?

So excited to see what's coming next ? :star_struck:
```

---
## \#93 Posted by: TarzanHBK Posted at: 2018-02-19T18:32:46.560Z Reads: 147

```
I think it´s difficult with power managment. If you have to push the button before it wakes up, what happens if you don´t know it shut down, start the board and want to drive? What happens when you plug the charger in?
```

---
## \#94 Posted by: SimosMCmuffin Posted at: 2018-02-19T19:02:12.213Z Reads: 169

```
@TarzanHBK

I'm meaning that shutdown mode is supposed to be entered after like 10 days, if the BMS hasn't been activated or plugged into a charger in that time. I did think about this and just found the idea annoying, if the time before shutdown is too short and you have to get hand-on to the module just to wake it up.

[quote="b264, post:91, topic:46117"]
Certain commercial boards, ahem Evole, go into sleep mode after like 4 minutes or something, it’s even happened at traffic signals before.  It’s ridiculous, super-annoying, and dangerous
[/quote]
I'm planning on auto power off feature, which allows to specify the time after which cut power off from load, if the measured current is too low. IE, if load current "<200 mA for 1 hour" -> "cut off load power". This is meant for if you accidentally forget to power off your board at the end of a ride, so the motor controllers or other loads don't drain the battery too much.

[quote="Pimousse, post:92, topic:46117"]
Please put the CAN !!! I think it’s even better than UART as you can use the CAN forward command of the VESC to dial with the BMS using only the BLE of the VESC. I wouldn’t add another BLE module just for BMS plus the one for the VESC although we can use the same one.

And it’s not a big deal to integrate a communication between BMS and VESC to switch power off smoothly in case of low voltage on a cell or whole battery.
[/quote]
I went for bluetooth as the first choice, because that I can implement by myself and it's simple. Running CAN comms through VESCs bluetooth is more complicated in that sense.

EDIT: I checked the STM32F070's datasheet and it doesn't have hardware CAN support

[quote="Pimousse, post:92, topic:46117"]
May you tell the interface passing between 2 boards (main and power) ? Which signals are exchanged ?
[/quote]
Swtich-module will have a BQ76200 gate driver for precharge and discharge FETs and a ISL28022 for current measurements. Then there is 3 analog signals for temperature, load voltage and ID voltage, which is meant to be used to detect what discharge current capable module is connected.
![image|690x337](upload://v4XUa7Uxd2cLEo5Q8jRkoDl6FMw.png)
```

---
## \#95 Posted by: TarzanHBK Posted at: 2018-02-19T19:28:28.654Z Reads: 147

```
Cool that sounds much better :slight_smile:
```

---
## \#96 Posted by: b264 Posted at: 2018-02-19T19:36:10.033Z Reads: 152

```
[quote="SimosMCmuffin, post:94, topic:46117"]
“&lt;200 mA for 1 hour”
[/quote]

I'm specifically suggesting making it ten hours+, not one hour.  Longer than a ride, workday, traffic signal, or full charge would be.  That will still accomplish your goal with less side-effects that you may not foresee
```

---
## \#97 Posted by: GrecoMan Posted at: 2018-02-19T19:40:44.761Z Reads: 150

```
I think 1 hour is good. if you’re sitting at a traffic light without any movement for an entire hour you should pick up your board and walk home. you’ll be fired from work for being that late.
```

---
## \#98 Posted by: SimosMCmuffin Posted at: 2018-02-19T19:43:26.049Z Reads: 151

```
This is just load cut off, not the shutdown state. You can just re-activate the load with the external switch. If you don't use the BMS or charge the board for 10 days, then it'll go into the shutdown state from which you can recover only by pressing the button on the module itself.
```

---
## \#99 Posted by: b264 Posted at: 2018-02-19T19:44:05.570Z Reads: 156

```
[quote="GrecoMan, post:97, topic:46117"]
I think 1 hour is good.
[/quote]

You think 1 hour is good.  Someone else might think ten minutes is good.  Or someone at Evolve might think 4 minutes is good and nobody will ever need more.  But either way, having it stay on longer won't hurt any of them at all but having it shut off early can inconvenience someone.  There is no ROI for making it short, other than ease of testing for the engineer designing it.  What if I want to watch the bluetooth signal while it's charging across the room?  (So can leave when it hits 95%)  Now you've just made that not possible for reasons that provide you no benefit at all.  What if the power is out and I'm using the lights on it to light up my house?

There are a zillion things that can come up and making it short when it provides no additional benefits other than safeguarding a deep discharge over periods of weeks or more is a mistake others have already made.  We don't need to repeat it.

Make it ten hours+
```

---
## \#100 Posted by: b264 Posted at: 2018-02-19T19:46:33.595Z Reads: 147

```
[quote="SimosMCmuffin, post:98, topic:46117"]
This is just load cut off, not the shutdown state.
[/quote]

I'm talking about both
```

---
## \#101 Posted by: GrecoMan Posted at: 2018-02-19T19:48:12.363Z Reads: 140

```
what’s the point of having a cutoff after it already destroys my battery? the whole point is to stop it from completely draining my battery if i forget

if you’re using the esk8 to light up your house i don’t think it would be a huge inconvenience to press a button every hour so it didn’t shut off 🤷‍♀️
```

---
## \#102 Posted by: b264 Posted at: 2018-02-19T19:49:50.836Z Reads: 143

```
It's not going to destroy your battery with idle current over ten hours.  Unless you're running like a 0.5Ah battery...
```

---
## \#103 Posted by: SimosMCmuffin Posted at: 2018-02-19T19:50:16.659Z Reads: 150

```
I'll make it configurable, you don't have to use it (no shutdown or load cut off time), but it's there for those who want it. I think it's perfectly reasonable feature. Set the time to something that makes sense to you.
```

---
## \#104 Posted by: Pedrodemio Posted at: 2018-02-19T22:42:32.086Z Reads: 155

```
@SimosMCmuffin
About the sleep state, what about making the power button 2 pole, and then it can also be used to wake up from sleep

If this delay is easily user defined them no problems, my boards are usually pretty well sealed with silicone after everything is working, and having to open it if get away from let’s say 2 weeks is a pain
```

---
## \#105 Posted by: SimosMCmuffin Posted at: 2018-02-20T06:29:28.572Z Reads: 162

```
Giving it some thought. I think it might better to just move the wake-up function completely to the external switch, but make it so that it can be just a normal off-mom switch or toggle off-on. Keep the switch simple as a single pole so you can use a following cheap switches for it:
https://www.ebay.co.uk/itm/Waterproof-Silver-12mm-LED-Momentary-Push-Button-latching-Switch-1NO-4Pin-Cool/192049157592?ssPageName=STRK%3AMEBIDX%3AIT&var=491866747727&_trksid=p2057872.m2749.l2649
OR
https://www.ebay.co.uk/itm/12-19mm-36V-LED-Power-Symbol-Metal-Momentary-Push-Button-Switch-For-Car-Boat/263292767049?ssPageName=STRK%3AMEBIDX%3AIT&var=562302410182&_trksid=p2057872.m2749.l2649

This would completely eliminate the need to be able to open the enclosure to wake-up the module and at the same time allow for the widest range of external switch types.

I'm gonna look into how to implement this.
```

---
## \#106 Posted by: b264 Posted at: 2018-02-20T06:32:45.532Z Reads: 136

```
If I could add, it's a really good idea if to power it off you have to hold the switch for X seconds.  That way if a stick or rock flies up and hits the switch it doesn't kill your brakes...
```

---
## \#107 Posted by: SimosMCmuffin Posted at: 2018-02-20T06:33:37.932Z Reads: 136

```
This is a planned software feature

EDIT: and also the load will be able to push current into battery through the Switch-module even if it's switched off, so braking is essentially never disabled.
```

---
## \#108 Posted by: b264 Posted at: 2018-02-20T06:34:00.246Z Reads: 133

```
the super debouncer
```

---
## \#109 Posted by: SimosMCmuffin Posted at: 2018-02-20T06:56:09.339Z Reads: 130

```
[quote="SimosMCmuffin, post:105, topic:46117"]
I think it might better to just move the wake-up function completely to the external switch, but make it so that it can be just a normal off-mom switch or toggle off-on
[/quote]

*Whlie still also enabling reading the state of the switch during battery power or usb power.
```

---
## \#110 Posted by: b264 Posted at: 2018-02-20T06:57:27.307Z Reads: 129

```
[quote="SimosMCmuffin, post:107, topic:46117"]
the load will be able to push current into battery through the Switch-module even if it’s switched off, so braking is essentially never disabled.
[/quote]

If the ESC is powered down, the output FETs won't be able to deliver the braking current to the battery
```

---
## \#111 Posted by: SimosMCmuffin Posted at: 2018-02-20T07:09:36.298Z Reads: 135

```
The ESC will function off of the motor's BEMF voltage and boost that voltage higher than the battery voltage allowing for braking to a lower speed, once the motor speed is too low then the ESC can't boost the voltage no more and it's DC bus voltage crashes and it shuts down.

If the ESCs DC bus voltage drops lower than the BEMF voltage, current will start to flow back into the DC bus through the FETs body diode. The motor starts to act as generator at this point.

EDIT: Try this: disconnect battery from an ESC, connect motor and spin it with a hand drill for example. The ESC will power up.
```

---
## \#112 Posted by: Pimousse Posted at: 2018-02-20T08:23:22.984Z Reads: 148

```
[quote="SimosMCmuffin, post:94, topic:46117"]
I checked the STM32F070’s datasheet and it doesn’t have hardware CAN support
[/quote]

Oh no. That's a pity.
I would love to have only one communication line for all the variables on the board.
That means one app (smartphone / smartwatch / smartwhatever) collecting and displaying all the data of your board (speed, current, cells voltage, real SoC, number of cycles...).
Also I think that acting directly on the ESC output as switch off (by sending STOP command or something) is safer than simply power off the whole ESC.
CAN forwarding has been implemented successfully by @rpasichnyk, @Ackmaniac and @emmaanuel on their own apps. Shouldn't a big deal, should it ?
I'll be pleased to contribute as well :slight_smile: (in the scope of my skills :smile: ) 

Thanks for the pinout explanation of the connector.
What the max current rating of those pins ?
I mean, what would be the max charge current allowed ?
```

---
## \#113 Posted by: SimosMCmuffin Posted at: 2018-02-20T09:11:43.553Z Reads: 152

```
On the future of CAN, I'm planning on skipping on it on this first iteration, mainly due to the fact that the MCU doesn't support it and if I were to change it, this would cause most likely a pretty big re-wiring job and atm there is no space for the CAN transreceiver or for the CAN connector. There is already a lot on the board that I want to test and see that the implementation works.

I can most likely fit the CAN in the future by changing MCU to one that supports CAN and the connectors to surface mount ones, which allows me to mount the CAN transreceiver underneath them then and share the USART pins with the CAN pins, so the connector can either go to a bluetooth module with the usart or to a another CAN device. That way it still supports CAN and Bluetooth directly.

[quote="Pimousse, post:112, topic:46117"]
Thanks for the pinout explanation of the connector.

What the max current rating of those pins ?

I mean, what would be the max charge current allowed ?
[/quote]
"Current Rating	3A" per pin on the connector.
https://www.digikey.fi/product-detail/en/sullins-connector-solutions/SFH11-PBPC-D08-ST-BK/S9196-ND/1990089

The reason why I put 4 parallel pins is to increase the current carrying capability through the connector. I'm speccing the parts for MAX 5 A charging current. Testing needs to be done to see how the ribbon cable behaves thermally with the max current.
![image|688x342](upload://568c0jpjC4hYdiwVvDAAfOmLbgh.png)
```

---
## \#114 Posted by: Pimousse Posted at: 2018-02-20T10:08:33.186Z Reads: 148

```
Thanks a lot for this constructive answer, love it.

[quote="SimosMCmuffin, post:113, topic:46117"]
On the future of CAN, I’m planning on skipping on it on this first iteration, mainly due to the fact that the MCU doesn’t support it and if I were to change it, this would cause most likely a pretty big re-wiring job and atm there is no space for the CAN transreceiver or for the CAN connector. There is already a lot on the board that I want to test and see that the implementation works.
[/quote]
That makes sense, definitely !
If you're not against adding it in the future, I'm in :grinning:

[quote="SimosMCmuffin, post:113, topic:46117"]
The reason why I put 4 parallel pins is to increase the current carrying capability through the connector. I’m speccing the parts for MAX 5 A charging current. Testing needs to be done to see how the ribbon cable behaves thermally with the max current.
[/quote]
So 4x 3A should theoretically allow a 12A charge but you limit to 5A, right ?
Isnt it too conservative ? We have to be careful with the ribbon cable though, that's right.

Thermal and electrical wize, I would advise (if the layout allows it), to put the GND at the other end of the connector. Thus you avoid accidental short-circuit (if 2 pins bent to each other) and also avoid having back and forth strong currents squeezed in the same side of the cable.
Like this :
![connectors|690x337](upload://48p1TpwWqGijyqkvbkOyNqHdgEC.png)

Thermal wize, (red wires are the ones that generate the most heat while charging) :
![thermal_ribbon|690x279](upload://tD78bJJV0HduaT3LHbSlKkfkwOz.png)

What do you think about his ?
```

---
## \#115 Posted by: SimosMCmuffin Posted at: 2018-02-20T10:34:35.478Z Reads: 138

```
[quote="Pimousse, post:114, topic:46117"]
So 4x 3A should theoretically allow a 12A charge but you limit to 5A, right ?

Isnt it too conservative ? We have to be careful with the ribbon cable though, that’s right.
[/quote]

I do believe that 5 Amps is quite plenty of current to push through, if you consider that a 10S pack with 5 Amps is 180 Watts of charging power already, but once again this isn't a hard limit. 7 Amps starts to close on some power handling capability of the charging current measurement shunt resistor.

Anyway the boost charger can't support this high _power_, but you could push something like that with a hefty bulk charger.

[quote="Pimousse, post:114, topic:46117"]
Thermal and electrical wize, I would advise (if the layout allows it), to put the GND at the other end of the connector. Thus you avoid accidental short-circuit (if 2 pins bent to each other) and also avoid having back and forth strong currents squeezed in the same side of the cable.
[/quote]

I would somewhat question the possibility of the pins touching each other, because it's on a 100 mil (2,54mm) pitch, so the pins aren't exactly side-by-side and I don't think you should be connecting the switch module while the battery is connected and the connector shroud should protect the pins from accidental bending. Fair point though, but I don't see any immediate danger in this config.

Having the BAT+ and GND high current pathways next to each other also decreases the loop area, which then lowers the EM noise. The more sensitive analog signals are somewhat shielded from the noise by the GND being in between them and the BAT+. Thermal wise it's not as optimal as the case you pointed, but I can't really say anything about it's performance yet, because I haven't tested it. I'll do a test today on my bench power supply to see how it behaves thermally with different currents.
```

---
## \#116 Posted by: Pimousse Posted at: 2018-02-20T11:02:43.059Z Reads: 130

```
[quote="SimosMCmuffin, post:115, topic:46117"]
Having the BAT+ and GND high current pathways next to each other also decreases the loop area, which then lowers the EM noise.
[/quote]

Good point !
Didn't think about that... :neutral_face:
If you can, try different length of ribbon cable.
I like this approach of experimenting stuff like that ! Great R&D !
```

---
## \#117 Posted by: SimosMCmuffin Posted at: 2018-02-20T11:14:37.821Z Reads: 145

```
I whipped up a quick test piece, as pictured below.
![image|690x389](upload://yfATSTKlHASKvBymqCm0bG68jjJ.jpg)

Tested with 10 Amps on the workplace's power supply and some heat was detected in the cable itself, but most in the connector, which was most likely due to the loosely fitting 4-pin male header connector (AKA not optimal connection).

I'll try to do another test with better connectors at home and post some IR-pictures from that.

EDIT: Ribbon cable is usually 28 AWG and with the 4 wires together it's equivalent to 23 AWG in surface area.
```

---
## \#118 Posted by: Pimousse Posted at: 2018-02-20T11:37:24.536Z Reads: 137

```
Awesome tests !
IR pictured will tell a lot ! I need one at home.
```

---
## \#119 Posted by: SimosMCmuffin Posted at: 2018-02-20T11:40:52.312Z Reads: 149

```
Just out of curiosity I was googling around and found an article testing 28 awg ribbon cable in power carrying use. Seems somewhat old, but I believe it's still relevant.
http://lss.fnal.gov/archive/test-tm/1000/fermilab-tm-1657.pdf
![image|648x396](upload://vKJKuE4FGpUe2lnBZfPPYT0d0Kt.jpg)
![image|641x277](upload://gSaQrPKhUl21eRubZZ6yGi3UnNk.jpg)
![image|690x330](upload://9P713vuEpKbmkQzVSRrTm89HjEL.jpg)
```

---
## \#120 Posted by: Pimousse Posted at: 2018-02-20T12:02:39.938Z Reads: 125

```
Fermilab???
Ahah you can trust these documents :smile: 

So I guess 5A would be OK (they say that in a 40C ambiant temperature you add 15 C so it 's still in the boundaries, isn't it ?
```

---
## \#121 Posted by: Pedrodemio Posted at: 2018-02-20T12:11:21.834Z Reads: 113

```
Instead of using the grey ribbon that is 28 awg you can use the colorful ones that is 24 and works just fine with most plugs

My current board I’m using 6 pins total in a ribbon to charge, by your test it might be a bit overkill, better safe than sorry. As soon as I get everything working I will give some long term feedback on how it handles the current with the heat from everything else plus being without air circulation inside the enclosure
```

---
## \#122 Posted by: Kug3lis Posted at: 2018-02-20T12:31:44.381Z Reads: 121

```
I haven't followed the whole topic, but it kinda looks like my BMS I am designing at the moment ;) Just I will be using block mosfets, isolated CAN + USB and no boosting circuit as I don't need it :)

But overall good work :) You work with KiCad? Because at first in 3D views I thought its Altium 18
```

---
## \#123 Posted by: SimosMCmuffin Posted at: 2018-02-20T12:39:14.796Z Reads: 127

```
I'm using KiCad. Moved to it from Eagle about a month ago, as the Autodesk acquisition with subsequent change to move into a subscription pay model didn't jive with me well. Decided to try KiCad once more and it's pretty darn good now and I much prefer it to Eagle now.

Are you going for what specific MOSFET for the discharge? FDBL86561-F085?
https://www.digikey.fi/product-detail/en/on-semiconductor/FDBL86561-F085/FDBL86561-F085CT-ND/5209201
```

---
## \#124 Posted by: Kug3lis Posted at: 2018-02-20T12:43:38.243Z Reads: 121

```
I will use case mounted MOSFET's, much easier to deal on higher currents. Plus I will have some copper busbars connecting 16 x xt90 connectors so it makes everything much easier. It's in SOT-227 case :slight_smile:

https://www.digikey.co.uk/product-detail/en/ixys/IXFN420N10T/IXFN420N10T-ND/2354436
```

---
## \#125 Posted by: Kug3lis Posted at: 2018-02-20T12:52:19.647Z Reads: 119

```
In the beginning of my PCB design I used Eagle, and then tried out Altium with really high level of tolerance to learn and now it's a bliss :D
```

---
## \#126 Posted by: JTAG Posted at: 2018-02-20T15:38:31.212Z Reads: 128

```
[quote="SimosMCmuffin, post:94, topic:46117"]
This is meant for if you accidentally forget to power off your board at the end of a ride, so the motor controllers or other loads don’t drain the battery too much.
[/quote]

Accidentally? Once you know you have auto power-off (like your design will have and mine has) you don't even care about turning it of. Once I arrive somewhere I just put my board somewhere and move on, it is so nice to never have to worry about turning off the board :grin:.
```

---
## \#127 Posted by: SimosMCmuffin Posted at: 2018-02-20T16:01:13.456Z Reads: 135

```
[quote="PatRocks, post:119, topic:34437"]
Update:  I did something really negligent a couple weeks ago. I left my board powered on for a day or two, and went out for a hard ride without checking my battery voltage. Started hitting my battery cutoff about a mile away from home, and when I got back I had 2 cells at about 2.86 volts. After freaking out for a few minutes I got my s*** together, and attempted to balance them back to good standing. At first I was having trouble balancing them, but they’re actually back in line with each other. I thought I had ruined about $1,200 worth of batteries, but for now they seem okay.
[/quote]
This is from another thread, but really case in point for the auto power off feature.
```

---
## \#128 Posted by: SimosMCmuffin Posted at: 2018-02-20T17:33:29.451Z Reads: 152

```
Okay, thermal test results for the 28 AWG ribbon cable. IR-images are taken with a FLIR ONE.

Below is the test setup presented. Bench power supply is ran in constant current mode with wires leading to the ends of the ribbon cable (I painted the cable partially black with a marker to see if it changed it's IR-emissivity, but it was unaffected).
![IMAG0863|690x389](upload://mesqhG75VUdkfjiERRHZy3petAR.jpg)

I tested the performance on one end with a run-of-the-mill 100 mil pin header and the other end got a cannibalized IDC-male connector with the shroud removed so I can plug it in. This was done to test to see if there is any contact differences/problems with otherwise seemingly identical pin headers.
![IMAG0866|690x431](upload://qOrhsJAfqxPajnqekCALSP07cbq.jpg)
![IMAG0864|459x433](upload://y4NYivqWQd7ijuvowySqBL2RO7I.jpg)![IMAG0865|573x430](upload://oEbZThCnPyPBPx61nxXVh3vRXuj.jpg)

----

**Thermal pictures for 5 Amps current:**
![Screenshot_20180220-184824|281x500](upload://tfVCrW4IDMwCClwYXZ7Ehx4NogZ.png)![Screenshot_20180220-184844|281x500](upload://k1g4oRMZlAtVN6xvp5KyYs22imB.png)
![Screenshot_20180220-184808|281x500](upload://6sZ62BFsE3tL5dkCRBEEtcxm4oW.png)

Cable temperature is no problem, only a very slight increase. Slight temp increase also at the contacts with the normal pin header running a bit hotter, which would lead me to assume a bit worse contact connection compared to the cannibalized IDC header. Maybe the 10 Amp test current will show a bigger difference.

----

**Thermal pictures for 10 Amps current:**
![Screenshot_20180220-183803|281x500](upload://mICQKGMSgNFud134Q2LGXeL7O76.png)![Screenshot_20180220-183949|281x500](upload://t3nGepfxRlmkMFSXZ4lOa8cJBUD.png)![Screenshot_20180220-183844|281x500](upload://4TuGTbR5bPsDf1pfofNVUOX7Vxo.png)![Screenshot_20180220-183915|281x500](upload://jUl8QHrmNkbxcGdQtwlNNfE5bpl.png)

Now we are starting to warm up! Middle point of the cable is around 48~50 C and the difference in the contact quality at the ends is showing up quite clearly. Cannibalized IDC header is running roughly about 10 C cooler than the normal pin header at 66 C. Again not critical or extreme temps, but I would start to get worried about the performance over a longer time as the contacts heat cycle at each end...

**Based on these tests, I conclude that 5 Amps current over 4 conductors is very doable and should last in use. Factoring in that the paired male and female headers from the same manufacturer will most likely also have a better fit overall.**
```

---
## \#129 Posted by: b264 Posted at: 2018-02-20T18:46:07.755Z Reads: 128

```
After seeing all that, I would unsolder the header and solder the ribbon cable directly onto the PCB after I got it.  So My vote is "I don't care, A or B" :rofl:
```

---
## \#130 Posted by: Pimousse Posted at: 2018-02-21T07:35:33.164Z Reads: 130

```
Wow !
That's a real scientific approach ! Thank you very much for these tests !
Also, I note that the heat really stays on the used wires and doesn't spray into the whole ribbon cable (plastic is not really a heat conductor).

Just for science, would you mind redoing these tests with the ribbon layout I posted (separate Bat+ and GND at each end) to see if there is a difference with your layout ?
```

---
## \#131 Posted by: SimosMCmuffin Posted at: 2018-02-21T08:48:28.308Z Reads: 147

```
[quote="Pimousse, post:130, topic:46117"]
Just for science, would you mind redoing these tests with the ribbon layout I posted (separate Bat+ and GND at each end) to see if there is a difference with your layout ?
[/quote]

Based on the test, I would speculate that there wouldn't be any real difference. I mean, I tested 4 side by side conductors and especially at the 5 Amp current the cable had no problem dissipating the heat. The warm zone was just around the current carrying conductors. So the results would otherwise be identical expect there would be another group of 4 conductors on the other side of the cable at the same temperature.

The insulation is also so thin between the conductors that it's not going to transmit heat well to the next conductor. So the heat should stay quite well around the hot conductor. 

Insulation thickness demonstrated by seeing my fingers through it against bright light.
![IMAG0867|282x500](upload://xdRx2RAYOfDjcHyO0xKw2Yq85u8.jpg)
```

---
## \#132 Posted by: Pimousse Posted at: 2018-02-21T10:42:18.274Z Reads: 139

```
[quote="SimosMCmuffin, post:131, topic:46117"]
The insulation is also so thin between the conductors that it’s not going to transmit heat well to the next conductor. So the heat should stay quite well around the hot conductor.
[/quote]

I would say : Less thickness = less thermal resistance, right ?
Anyway, with 5A, you're fine and if in this "worst" thermal case it's even good, it's better than having lot's of EM noises. :slight_smile:

So :
- 5A current through Ribbon cable : checked :white_check_mark: 

What's next ?:smiley:
```

---
## \#133 Posted by: SimosMCmuffin Posted at: 2018-02-21T12:57:26.212Z Reads: 132

```
I guess at this point the next step is for me to do sanity checks on the schematic and layout and once they look okay to me, release the files for public review and if no critical mistakes or errors are found, move into ordering the PCBs and building the first iteration prototype.
```

---
## \#134 Posted by: Pimousse Posted at: 2018-02-21T12:58:13.274Z Reads: 128

```
Count me in for beta testing ! :slight_smile:
```

---
## \#135 Posted by: Kug3lis Posted at: 2018-02-21T13:31:42.080Z Reads: 130

```
I would be interested in firmware, are you going to use some kind of Framework like mbed/arduino or just plain STM32Cube ?
```

---
## \#136 Posted by: SimosMCmuffin Posted at: 2018-02-21T16:48:53.222Z Reads: 127

```
I'm gonna go with a pretty simple state machine flow for the firmware. I'm gonna use at least the USB VCP driver from the CubeMX. I use AC6/STM32 workbench as the IDE. 

I don't see a need to use something like a RTOS, so I'm going to KISS it. I'm going to write my own libraries for the I2C-, USART- and SPI-buses.
```

---
## \#137 Posted by: SimosMCmuffin Posted at: 2018-02-22T08:28:58.892Z Reads: 146

```
Ok, I am almost done with the sanity check on the project, but I found a pretty critical footprint mistake with the module interconnector. Not a fatal error and I have come up with a backup plan.

So what's the problem? Well, I had been using a normal **UN**shrouded 2x8 100 mil pitch header as a placeholder on the board and going through all the footprints used on the board and checking their sizes I noticed the mistake I had done with the interconnector. It's shroud takes up quite a big area around the pins, as shown below.

![image|200x200](upload://pYVWXT2U9e2Iy89GUwNc8PdxZna.jpg)
![image|690x113](upload://frW68m3VqMI0hvHXPGcU1QZmpnj.png)
![image|457x500](upload://mQV1K3lMGF1YKNTwi860m7FTYPe.png)

Solution? 
We're going to use an unshrouded connector, just like in the picture above. I would have liked to use a shrouded connector, because it would have given the pins some protection mechanically and it was polarized so, you couldn't plug in the ribbon cable connector the wrong way around. 
I can 3D-print a protective shroud for the connector, if it's not used and I can add a silkscreen mark for the notch on the ribbon cable connector, but as you know, idiots usually find a way...

Male:
https://www.digikey.fi/product-detail/en/sullins-connector-solutions/PREC008DAAN-RC/S2012EC-08-ND/2774886
Female:
https://www.digikey.fi/product-detail/en/sullins-connector-solutions/PPTC082LFBN-RC/S7076-ND/810214
Ribbon:
https://www.digikey.fi/product-detail/en/sullins-connector-solutions/SFH210-PPPC-D08-ID-BK/S9288-ND/2095297
```

---
## \#138 Posted by: b264 Posted at: 2018-02-22T08:30:44.656Z Reads: 125

```
You could fill one of the female up with epoxy and leave off one of the male pins to polarise the connector
```

---
## \#139 Posted by: SimosMCmuffin Posted at: 2018-02-22T08:31:25.665Z Reads: 126

```
Otherwise good idea, except all 16 pins are used
```

---
## \#140 Posted by: Pimousse Posted at: 2018-02-22T08:50:39.206Z Reads: 137

```
IMHO, you'd better design an **idiot-proof** and **reliable** BMS.
So loosing the coding system and the mechanical holding system seems to be quite away from both goals.

You may want also to avoid extra work on the PCB such as adding epoxy here, cut a pin there as it will increase your workload and potentially mistake (you add a human failure risk).

OR

This can wait the next iteration. Maybe after the first one, you'll figure out that ribbon cables are not the way to go. ;)
```

---
## \#141 Posted by: b264 Posted at: 2018-02-22T08:53:42.006Z Reads: 126

```
This just made me realize

Instead of labeling the PCB  "B-" and "P-" if you mark it "batt+" and "load-" and "charge-" on the actual PCB itself if you have room, it will make things a lot easier for a lot of folks and there will be far less questions and mistakes
```

---
## \#142 Posted by: SimosMCmuffin Posted at: 2018-02-22T09:25:13.814Z Reads: 126

```
Changing the connector is not possible, because it simply does not fit onto the board without making the the board bigger. Let's go with the simpler unshrouded connector in the first iteration and see how it works, before doing board redesign. If we find problems with, then we'll see what the options are and go after improvements, but if it turns out to work ok, then we don't need to make the board any bigger than necessary.
```

---
## \#143 Posted by: SilentException Posted at: 2018-02-22T09:29:28.561Z Reads: 128

```
This project is great, just what the DIY community needs, a decent BMS. Thank you @SimosMCmuffin! 
There is one more feature I think it would be nice to have and that is smart discharge after X days. For example, if not using the board for 7 days, start the discharge to storage voltages ;)
```

---
## \#144 Posted by: SimosMCmuffin Posted at: 2018-02-22T09:31:57.972Z Reads: 132

```
[quote="SilentException, post:143, topic:46117"]
This project is great, just what the DIY community needs, a decent BMS. Thank you @SimosMCmuffin!

There is one more feature I think it would be nice to have and that is smart discharge after X days. For example, if not using the board for 7 days, start the discharge to storage voltages :wink:
[/quote]

[quote="SimosMCmuffin, post:90, topic:46117"]
The reason I want this feature is to protect the battery from a deep discharge when for example putting it in winter storage or other such thing. I intend to add to software configuration to allow to set the time before the module goes to deep sleep and would also allow to discharge the battery to storage voltage after the module would turn itself off.
[/quote]

Already planned.
```

---
## \#145 Posted by: SilentException Posted at: 2018-02-22T09:34:25.022Z Reads: 115

```
Thanks I looked and searched the thread but didn't see it. Nice!
```

---
## \#146 Posted by: Pimousse Posted at: 2018-02-22T09:52:49.945Z Reads: 119

```
Is there any other connector type that could allow to keep the tiny size and mistake-proof feature ?

What about having 2 different connectors : 1 for power and one for signal which could use smaller pin pitch and smaller footprint like a JST-ZH for instance ?

Just throwing some ideas
```

---
## \#147 Posted by: SimosMCmuffin Posted at: 2018-02-22T10:26:19.083Z Reads: 137

```
Going with KISS, I think it's better to keep the variety of used connectors to a minimum, just for inventory reason. Currently the balance connector is JST-XH, the external switch and LED is JST-XH and the bluetooth module connector is JST-XH. These are also connectors that are _quite_ easy to crimp yourself.

The pin header with the IDC ribbon cable is also an easy, neat, all-in-one package. At least for now. Will have to see how it works.
```

---
## \#148 Posted by: SimosMCmuffin Posted at: 2018-02-22T10:40:17.450Z Reads: 150

```
I can't really find anything else wrong with the project at this moment so here's the packaged KiCad project.

**google drive link removed, project files available @ https://github.com/SimosMCmuffin/FlexiBMS_hardware**

All components should have a manufacturer's part number associated with them, which can used to lookup specific components. Before sending the board to fab, silkscreen needs to be optimized.

EDIT: If you get missing library warning when opening the schematic, they should be non-critical.

1. KiCad can be downloaded from http://kicad-pcb.org/download/
2. Install everything as default options, no need to install Wings3D at the end of the installer.
3. Download the KiCad project files and extract the .Zip to a folder
4. Open KiCad and open project (CTRL+O) and navigate to the folder where you extracted the files.
5. A file ending in ".pro" should be in the folder. Open that and you have the project open
```

---
## \#149 Posted by: Pimousse Posted at: 2018-02-22T13:57:58.268Z Reads: 146

```
I'll do it ASAP !
Thanks a lot for sharing !
Could you commit file into Github ?
It's way easier to download/manage vesion files and contribution (like adressing issues or propose improvement) :slight_smile:
```

---
## \#150 Posted by: SimosMCmuffin Posted at: 2018-02-22T14:04:21.935Z Reads: 146

```
I'll try to set it up today.
```

---
## \#151 Posted by: SimosMCmuffin Posted at: 2018-02-23T18:54:08.073Z Reads: 146

```
Github Repo is up and running!
https://github.com/SimosMCmuffin/FlexiBMS_hardware
```

---
## \#152 Posted by: SimosMCmuffin Posted at: 2018-02-25T16:47:17.365Z Reads: 154

```
Silkscreen has been sorted out. I'm aiming to get the board sent to manufacturing today. I'll sort out the gerber files and commit the files soon.

I assume that anyone doesn't have anything critical to note from the github files?

![image|690x462](upload://jNoINNrfIwV9PcIriXA3kYs6nAI.png)
![image|690x462](upload://2WmTavUWNpNwv8FAwgAoq4kVMs7.png)
```

---
## \#153 Posted by: Pimousse Posted at: 2018-02-25T16:53:54.040Z Reads: 141

```
Dumb question : Are the led not too bright ?
I had this issue with Battman. I couldn't look at it, it made my eyes burn each time. :smile:
```

---
## \#154 Posted by: SimosMCmuffin Posted at: 2018-02-25T16:57:11.676Z Reads: 139

```
They should be "non-eye-damaging". Are you talking about the balance circuit Leds or the status Leds?
```

---
## \#155 Posted by: Pimousse Posted at: 2018-02-25T17:05:19.723Z Reads: 145

```
I didn't have the chance to see balance leds lighting :smile:
But status leds are really bright. And because they are close to each other you can't really see which one i on or not...

Same for RGB embedded. I don't really understand why not to externalize RGB light because once the BMS is enclosed, you don't see any leds anymore.

I found a cool button with RGB ring led on Adafruit and planned to desolder the embedded RGB led to power it instead.

https://www.adafruit.com/product/3350
```

---
## \#156 Posted by: SimosMCmuffin Posted at: 2018-02-25T17:17:40.320Z Reads: 148

```
I'm using very general LEDs as two status leds on the PCB itself, so they shouldn't be anything special brightness wise.

I'm planning on shipping these buttons with the board. I ordered couple of each to just see and test them and for the price they are pretty decent.

https://www.ebay.co.uk/itm/Waterproof-Silver-12mm-LED-Momentary-Push-Button-latching-Switch-1NO-4Pin-Cool/192049157592?ssPageName=STRK%3AMEBIDX%3AIT&var=491866747727&_trksid=p2057872.m2749.l2649

or
https://www.ebay.co.uk/itm/12-19mm-36V-LED-Power-Symbol-Metal-Momentary-Push-Button-Switch-For-Car-Boat/263292767049?ssPageName=STRK%3AMEBIDX%3AIT&var=562302410182&_trksid=p2057872.m2749.l2649
```

---
## \#157 Posted by: Pimousse Posted at: 2018-02-25T21:24:55.377Z Reads: 146

```
Oh ok.
I thought it could be a nice feature to have a RGB led to indicat whether the board is on/charging/faulty (ie, green, blue, red flashing).
Next iteration maybe ? :grin:
```

---
## \#158 Posted by: SimosMCmuffin Posted at: 2018-02-26T06:53:19.387Z Reads: 144

```
I was going to indicate the state of the board with the single colored Led via different kind of flashing styles and rhythms. 

RGB would be easier to distinct between states, because _colors_, but buttons with built-n RGB are not the cheapest... and you need more output pins on the MCU and on the connector.
```

---
## \#159 Posted by: keef Posted at: 2018-02-27T14:24:03.435Z Reads: 151

```
I've been looking at the raphael chang bms software since i also have one of the boards. I've been considering doing a rewrite in rust for fun. The lack of debugger connections has stopped me for now. I'd also be interested in helping out with software compatible for both bmses. 

I've taken a quick look at your schematic and really appreciate the debugging connections :slight_smile:

@Pimousse what's the current state of your firmware. Is it still the version on Github? I'm currently trying to get the serial connection working on linux
```

---
## \#160 Posted by: Pimousse Posted at: 2018-02-27T21:06:06.534Z Reads: 145

```
Well, I worked a lot on it, but I didn't try yet.
Since @SimosMCmuffin told us that the HW design of the Battman was limited (even dangerous), I stopped investing time on this project.

Just pushed my current working folder : https://github.com/Peemouse/battman-firmware/tree/dev
```

---
## \#161 Posted by: jbruce Posted at: 2018-03-09T03:14:43.977Z Reads: 132

```
Whats the expected price of these going to be? Do you need any beta testers?
```

---
## \#162 Posted by: SimosMCmuffin Posted at: 2018-03-09T07:02:45.608Z Reads: 151

```
[quote="jbruce, post:161, topic:46117"]
Whats the expected price of these going to be?
[/quote]

The BOM is looking at this moment roughly about 60€ for a _single_ main module and about 34€ for a batch of 100, but once I get the HW design tested and locked down I can move onto larger build batches, which will lower the component costs. 
I'll have to later look into if it makes more sense to fabricate and and furniture the boards with a third party, or whether to build them in my own space.

I also don't mind selling just the PCBs (+ possibly components) to those who want to assemble their own boards with the BOM available on github.
Honestly I don't want to nail down the price point to stone at this point in time, but I wouldn't expect less than 70€ once all the costs have been included.

[quote="jbruce, post:161, topic:46117"]
Do you need any beta testers?
[/quote]
I will most likely need/want at some point, once the module makes it through my own performance tests and I fix any obvious HW mistakes. Once that time comes I will inform about it in this thread and open up some kind of  application form for a limited amount of people. Modules might be provided free of charge, except for shipping and once the beta ends I will either let participants keep their modules for free-of-charge or pay for it with a discounted price for their help and effort.
```

---
## \#163 Posted by: banjaxxed Posted at: 2018-03-09T12:51:06.045Z Reads: 141

```
Hello there, I'm late and haven't read the thread completely yet but Ivam very interested if the footprint is this size & it does 12s, discharge protection, anti spark & eswitch can I get in on 1 or 2?

I will read the thread later when I have time thanks for your efforts in producing this
```

---
## \#164 Posted by: SimosMCmuffin Posted at: 2018-03-09T13:36:04.465Z Reads: 142

```
Sorry, the OP is not up to date with the current state of the project. I'll update it today, so it is up-to-date and new thread readers can more quickly understand what is being designed.

I would recommend starting to read from http://www.electric-skateboard.builders/t/flexibms-first-prototype-kicad-project-files-released-flexible-configuration-and-charging-bms/46117/23
```

---
## \#165 Posted by: TarzanHBK Posted at: 2018-03-09T15:23:11.844Z Reads: 141

```
sounds awesome - can´t wait to test one :grin:
```

---
## \#166 Posted by: banjaxxed Posted at: 2018-03-09T15:30:37.378Z Reads: 149

```
Thanks for the pointers, definitely want a split board here even better a stacked sandwich, I may try to make one or two.

Edit: I get it all now, the bms part is fully designed then we have the option on the switch side of the bosrd to size to discharge amps required, wonder what a pcb of the same size footprint could handle amps wise, also convenience to quickly swap out the switch board innovation 👌
```

---
## \#167 Posted by: Mike_Lemon Posted at: 2018-03-09T15:36:47.642Z Reads: 143

```
So at last what's up with this project? is there some demo vid of it somewhere?
```

---
## \#168 Posted by: SimosMCmuffin Posted at: 2018-03-09T16:14:32.298Z Reads: 138

```
PCBs are being manufactured at the moment.
```

---
## \#169 Posted by: Mike_Lemon Posted at: 2018-03-09T16:16:46.407Z Reads: 143

```
Hopefully this project will succeed. 

What would be the price for a 12S around 80A BMS setup? 

and how flat would it be?
```

---
## \#170 Posted by: SimosMCmuffin Posted at: 2018-03-09T16:33:36.062Z Reads: 154

```
This project is just beginning and is in prototype stage. I don't want to start promising any price points yet, because we haven't even tested the first prototype, which's PCBs are at the moment being manufactured. I'll be updating this thread as progress happens.
 
for more info, refer to this post at this point:
http://www.electric-skateboard.builders/t/flexibms-first-prototype-kicad-project-files-released-flexible-configuration-and-charging-bms/46117/162
```

---
## \#171 Posted by: Mike_Lemon Posted at: 2018-03-09T16:35:41.628Z Reads: 146

```
These prices look fine if you can ensure the quality over long period of time. Book marked.
```

---
## \#172 Posted by: SimosMCmuffin Posted at: 2018-03-15T16:16:47.919Z Reads: 162

```
Update.

Components ordered at the beginning of week and have now arrived.
![IMAG0876|690x389](upload://2jJINaE0j2A8NYZNpQyTmhCqhP0.jpg)![IMAG0877|690x389](upload://vCBlnZaNJpQbS7FFIf9SPXq9fwR.jpg)

PCBs are in the country and if lucky I'll be able to get them tomorrow, so I'll be able to assemble the first board and do basic functionality checks on it during this weekend.
```

---
## \#173 Posted by: SimosMCmuffin Posted at: 2018-03-16T19:49:15.064Z Reads: 163

```
Boards are here! 
I'm going to work on these during the weekend and try to progress towards functional prototype.
No component has been soldered yet to the boards in the pictures, I was just placing the bigger components.
![IMAG0878|690x389](upload://dXenGFj5K9BHoQpbJ5aUlI6Fu0V.jpg)
![IMAG0879|690x389](upload://eoKBX58ebjYSwj4QHngbtfBq6Nr.jpg)
![IMAG0880|690x389](upload://eFRqH7nO08jHLguj7kBQXXO9cnb.jpg)

The balance circuitry is very dense (as I designed it), I guess I'l just have to try and solder the components on or cry and solder them on :wink: 
![IMAG0881|690x364](upload://rf8pypY7vUktyAMCjGSrZUjzZLG.jpg)


Here is the size difference to the old pre-alpha prototype board, and as cliche as it might sound, I thought to myself "oh wow, this board is pretty small" when I got it out of the packaging.
![IMAG0885|626x500](upload://jl8S5nWnQHbUPR2Jgpp5Xt5ECEs.jpg)
```

---
## \#174 Posted by: banjaxxed Posted at: 2018-03-16T21:38:21.646Z Reads: 156

```
Nice is there rosin in your tears? 😂
```

---
## \#175 Posted by: SimosMCmuffin Posted at: 2018-03-16T22:03:20.377Z Reads: 161

```
I lick and scratch pine trees in the morning for my natural daily rosin dose.

Or if I'm about to crash, I go straight for the good stuff.
![IMAG0886|690x389](upload://hpWehyxu94N3dqXEIG4Y6xuP5FZ.jpg)

EDIT: It's a joke. Just in case somebody doesn't know or understand the context.
```

---
## \#176 Posted by: banjaxxed Posted at: 2018-03-16T22:04:02.812Z Reads: 160

```
Haha good one...pine fresh
```

---
## \#177 Posted by: riverside.rider Posted at: 2018-03-17T08:48:46.681Z Reads: 165

```
for the xt90 connector...just to let you know that there is a new type (already sold but not yet published) from Amass....perfect for PCB.let me know if you need the .stp file.....cannot upload it here..![xt90pw|690x474](upload://r1FHm3QV0cE5Cs9rGlLuRwACVXh.jpg)
```

---
## \#178 Posted by: SimosMCmuffin Posted at: 2018-03-17T11:59:05.626Z Reads: 161

```
Thanks for the tip!

I'll look into this once I start designing the Switch-module.
```

---
## \#179 Posted by: SimosMCmuffin Posted at: 2018-03-17T19:15:17.572Z Reads: 169

```
Board is assembled. Haven't tried to hello world the MCU yet, but that'll probably be the first thing tomorrow morning.
![IMAG0887|690x389](upload://mO9aCKKSRkCe5pJvBLD3IcqbYx7.jpg)
![IMAG0888|690x389](upload://847hdarFmjxLyKPFU9xHFNYrcWi.jpg)
![IMAG0890|690x389](upload://v5etWool6G6sUjHUQlbnGO5aAPS.jpg)
![IMAG0892|690x389](upload://uzpV6sZzHN55Y60XheLU2HIDemi.jpg)
![IMAG0891|690x389](upload://cnvorfK90x2aZ8ANUW1Z5sd2lsP.jpg)


There was a one major layout goof with the board. The footprint for the LTC6803-3 was incorrect with the wrong specific SSOP-package. The actual IC package was longer and wider than the footprint, but with the same pin pitch, so I managed to squeeze some of the components at the end just a bit further away and then bent the pins on the IC under it, enabling me to still solder it onto the board, although I wouldn't subject it to a lot of vibration with the fear of some of the solder points breaking loose. 
![image|501x413](upload://49YJZCab3MsEXU7cS1MLOfJfJGk.png)
![IMAG0889|690x389](upload://lMqtWhBxpUQkC3FCdOX1uJ8Vgxa.jpg)

Provided that everything is otherwise working on the board I can start testing and writing code for it. The layout will go into new iteration soon, which I have some improvements in mind and I'm gonna look into putting in the CAN-support as well.
```

---
## \#180 Posted by: scepterr Posted at: 2018-03-17T19:31:48.876Z Reads: 166

```
What if you trim the pins? Seems like enough pad beyond the ic
```

---
## \#181 Posted by: SimosMCmuffin Posted at: 2018-03-17T19:41:28.825Z Reads: 166

```
Well I did get IC soldered on, by bending the legs under it. The pads were far enough under it that you can't just trim the legs and try to solder it (pads are actually completely hidden beneath the IC, unlike shown in the illustrative picture). You need to have them go inwards for them to be able to reach the pads.

Other than that, the layout was fine and it will in any case get largely redone, because I need to change the MCU for one with a CAN support that people requested.
```

---
## \#182 Posted by: SimosMCmuffin Posted at: 2018-03-18T10:27:01.230Z Reads: 165

```
**It's alive!**
![Flexi01_blink|320x240](upload://h6aBhJLFhiuPhigi143uZHvTA9N.gif)

I'll now start to configure the peripherals and start connecting to the other ICs on the board.

EDIT: I have now tested and succesfully flashed the MCU via the USB bootloader, so the end-user, if they want/need to re-flash the firmware, they can do it with just a USB cable, no external programmer needed.
```

---
## \#183 Posted by: SimosMCmuffin Posted at: 2018-03-18T20:13:26.927Z Reads: 168

```
So, I was thinking today what my action plan will be for the next couple of weeks and what I need to achieve before I can progress to the next hardware iteration and have the next boards sent for fabrication with the goal to reach the beta test phase, hopefully by this summer.

I looked at the new MCU with the CAN support today and ended up with STM32F072C8T6 to replace the currently soldered STM32F070CBT6. Good thing is, as it's nearly identical model with the earlier one, the firmware should be pretty easy to port over, with basically just pin remaps, so I can already start developing the firmware features further than the basic functions with this board, but before I can work on the next hardware iteration with the new features, I need to code test functions for this board and test the performance of all the blocks, so I know they are functionally ok and don't need changing.

**So here's a priority list on how to progress for now:**

1. Implement basic firmware functionality to be able to test the board's performance and functionality
2. Design the next hardware iteration with new features and/or fix problems found with the earlier iteration and send boards for fabrication
3. While the boards are being fabricated (2-4 weeks), developed firmware features further with the current hardware with the portability in mind to the next iteration
4. Assemble new board and port old firmware and test the board's performance and functionality.
5. Repeat steps 2-4 until board ready for beta testing phase

---

I have been doing a long time test on how the **_pre-alpha_** prototype BMS has been draining the battery over the last 20+ days and have been logging the battery pack voltage. The test was started with a fully charged battery and has then just been left sitting with the BMS hooked up and I take voltage measurements roughly every 12 hours and enter them into a google sheet to generate the graph. I also measured the standby current with a multimeter and it seems to stay at pretty stable ~9 mA over the whole pack voltage (42-33 V). This test will continue on after this post and the google sheet updated.

The aim will be to lower this drain by at least a **factor of 2** in standby mode and by a **factor of 10** for the deep sleep mode for long time storage.

![image|602x374](upload://nDsqZgZvaMt7gvB0lQncutpxOU0.png)
```

---
## \#184 Posted by: SimosMCmuffin Posted at: 2018-03-20T17:11:54.429Z Reads: 165

```
Ok, the LTC6803 is not properly soldered on and it has intermittent connection problems, but I managed to test that the deep sleep wake-up via the external pushbutton works and that the MCU is able to turn itself off into the deep sleep mode.

I measured the following input currents @ 40V simulated battery voltage:
Deep sleep mode: 500µA
Standby mode: 7,3 mA (Can probably be reduced to < 7 mA, by powering all the ICs down and putting MCU into sleep mode)


So compared to the 9 mA standby current on the pre-alpha prototype.
[quote="SimosMCmuffin, post:183, topic:46117"]
The aim will be to lower this drain by at least a **factor of 2** in standby mode and by a **factor of 10** for the deep sleep mode for long time storage.
[/quote]
Current reduction factor of 10 for the deep sleep mode is easily achievable, but after looking at the relevant IC datasheets for the standby mode current. I don't think it's possible to realistically go lower than 6 mA, because the buck regulator alone with no load consumes about 4.8 mA, as shown in it's datasheet caption below. And also at very light loads (<20 mA), the buck converter has pretty bad efficiency. So, a factor of 2 reduction in current in standby use is simply impossible, but we can reduce it somewhat from the measured 7.3 mA still.

![image|690x207](upload://qy9QICzOCQByosWZMbClosuY6h9.png)

---

I have also confirmed with my earlier test board for the LTC6803-3 that the charge FET safety cut-off will work with a properly soldered IC. I was having weird behavior on the test module (Watchdog's open-drain couldn't pull itself completely down, but floated around 2,2V), but I'm very sure it's caused by the bad soldering job (due to wrong footprint), as it worked as intended with the standalone test module pictured below.
![IMAG0895|530x499](upload://j5xYfvjYZacSdPjJcQHMBE0W78t.jpg)

I have little doubt that there is anything wrong with the balance circuitry, due to it being pretty much identical to 
the ones used in earlier working prototypes, so I'm not sweating over that.

Now I need to test the current measurement, the boost charger circuit and some other small things and then I can start to work on the next hardware iteration.
```

---
## \#185 Posted by: Pedrodemio Posted at: 2018-03-20T18:37:25.072Z Reads: 156

```
http://www.electric-skateboard.builders/t/raphael-chang-bms-and-esc/8952/437?u=pedrodemio

The charging part is purely hardware to prevent this issue? I haven’t looked at the schematics
```

---
## \#186 Posted by: SimosMCmuffin Posted at: 2018-03-20T19:22:23.926Z Reads: 153

```
My module has complete hardware side protection against microcontroller hanging during charging.

If the microcontroller hangs while charging, even if it's enable_charging pin is left high, it also stops the communication with the LTC6803-3 battery stack monitor, which then causes it's watchdog to activate and the watchdog's open-drain output will pull the charging FET's gate low, cutting off the charging current.

When the MCU is operating normally it's keeping the LTC6803-3 in an active state during which it's watchdog output pin is floating and the MCU can pull-up or pull-down the charging FETs gate.

Along  with this, I'm planning on also running the MCU's internal watchdog, so it can recover from hang states, by resetting itself.
```

---
## \#187 Posted by: okashira Posted at: 2018-03-21T02:15:26.832Z Reads: 146

```
IMHO a good BMS should be below 20 microamps in deep-sleep/shutdown.
```

---
## \#188 Posted by: okashira Posted at: 2018-03-21T02:16:23.470Z Reads: 137

```
I think you replied to the wrong thread :)
```

---
## \#189 Posted by: Pedrodemio Posted at: 2018-03-21T02:38:04.058Z Reads: 146

```
No no, that’s on purpose since we were talking about @SimosMCmuffin Bms on batman thread

Edit: now I see, thanks, too many tabs open
```

---
## \#190 Posted by: okashira Posted at: 2018-03-21T02:53:58.204Z Reads: 156

```
I think 100uA is a bit much for deep sleep drain. It will kill the battery if someone parks their board after driving and leaves it for a month or so.

There are microcontrollers that can do 1uA with RTC and SRAM powered. The LTC6801 quiecient current is about 10uA.

It that a 20uA or so design is possible. that's with RAM powered and waking up every hour or so to take a measurment. :slight_smile:

Look at the STM32L4.
Low enough power you wont even need another DCDC and can power it directly from the LTC6803.
```

---
## \#191 Posted by: okashira Posted at: 2018-03-21T03:04:43.292Z Reads: 155

```
You can also consider a regular linear regulator or LDO for ultra low quiescent current.
With something like STM32L4 at low frequency and all your components optimized... (low leakage caps)
The poor efficiency wont matter.
```

---
## \#192 Posted by: SimosMCmuffin Posted at: 2018-03-21T07:19:01.671Z Reads: 157

```
Im doing a long time discharge test on my 10S5P (600 Wh) battery pack with my old BMS proto, which has standby current of ~9 mA from the battery, here's the current graph of it's effect
![image|602x374](upload://nDsqZgZvaMt7gvB0lQncutpxOU0.png)

It has almost been 30 days in _standby mode_. Then consider slowing this drain over 10 times for the deep sleep mode for 300+ days for the equivalent capacity. I think it's good enough. Could the deep sleep mode discharge be smaller? Yes, but this is already looking good enough approach.

[quote="okashira, post:438, topic:8952, full:true"]
No deep sleep? I though Raphael Chang specially added an external RTC so the MCU can be shut off and woken by the RTC, in fact I read he had specially measured the deep sleep drain at 10 microamps?
[/quote]

After looking closer at the Battman's RTC wake-up implementation and figuring out the logic behind it, it's pretty smart and I hadn't before realized how it exactly worked. But yes, it's a very good design that allows for very low quiescent current. Essentially only the LTC6803.

the MCU in sleep mode is not enough to reduce the input current a lot, because the buck regulator has such a high no-load current. Battman's implementation gets around this by completely cutting off the regulators from the battery via Q7, which causes the MCU to also shut off, but the RTC is using the Cell1 from the battery pack to power itself and periodically then enables the regulators back up.
![image|690x207](upload://5fRTJTk7h3Zo4kPxHSit30Ayyd6.png)

I feel like I was beaten in 4D chess game I didn't realize I was even playing :smile: At least I learned something new.

I'm gonna look at the possibilities on how to possibly implement something similar considering that there is hardware difference between the boards.

EDIT: Note, that the Battman's implementation does depend on having the balance connector on, so that the Cell1 is actually available. Mine implementation works with just the battery pack connected.
```

---
## \#193 Posted by: b264 Posted at: 2018-03-21T07:21:10.266Z Reads: 138

```
[quote="SimosMCmuffin, post:192, topic:46117"]
I feel like I was beaten in 4D chess game I didn’t realize I was even playing
[/quote]

This is my new favourite quote.
```

---
## \#194 Posted by: SimosMCmuffin Posted at: 2018-03-21T08:33:23.619Z Reads: 143

```
[quote="okashira, post:190, topic:46117"]
Look at the STM32L4.

Low enough power you wont even need another DCDC and can power it directly from the LTC6803.
[/quote]

I'm considering this. There is the LTC6803 5V output, which could be used to power just the MCU via a small LDO, the MCU (STM32L433CCT6) supply pins didn't seem to accept 5V directly after looking the datasheet. Then the MCU could power up the buck regulator directly if it needed to enable other circuits needing higher power.

I personally like this approach more then an external RTC IC. I'm gonna check the datasheet to see if the MCU has internal RTC capability, or if it needs an external 32kHz rock + does it need a high speed crystal for USB, or does it have an internal oscillator for that.
```

---
## \#195 Posted by: SimosMCmuffin Posted at: 2018-03-21T09:11:01.754Z Reads: 145

```
Direct quotes from the STM32L433 reference manual. RCC chapter

> **HSI48 clock**
> The HSI48 clock signal is generated from an internal 48 MHz RC oscillator and can be used
> directly for USB and for random number generator (RNG) as well as SDMMC. 
> **LSI clock**
> The LSI RC acts as a low-power clock source that can be kept running in Stop and Standby
> mode for the independent watchdog (IWDG), RTC and LCD. The clock frequency is 32 kHz. 

It seems that it wouldn't actually need any external crystals or oscillators to run USB and the RTC in low power mode.
```

---
## \#196 Posted by: SimosMCmuffin Posted at: 2018-03-21T18:45:35.860Z Reads: 159

```
@okashira I've been doing some measurements and comparisons between the Battman and Flexi 0.1 design and based on my tests I would say that the Battman has at least about 200 µA input current at 40 V battery voltage even at deep sleep mode.

Here's my evidence based on purely schematic design.
![image|606x500](upload://KQ7HiLeQCNpJlMlmBcrCnAEM4K.png)

The boost charger resistive divider will have with 40 V battery voltage:
40V - 0.7V (FET body diode) = 39.3V
39.3V / 207kOhm = 190 µA

There is also going to be some leakage through the FSV10120V schottky in the boost charger block to the LTC3873 boost controller. So I would say from design viewpoint, that there is no way for the Battman to have sleep drain of only 10 µAmps. Period.

Most of my quiescent currents also comes from voltage dividers, eliminating those somehow would have a decent effect on the deep sleep quiescent current.
```

---
## \#197 Posted by: SimosMCmuffin Posted at: 2018-03-22T07:34:49.522Z Reads: 160

```
I am posting this for the sake of transparency.

---

I have had multiple people contact(PM) me about the interest towards the FlexiBMS project, so I am compiling this message as a general reply in relation to the current project status at this point of time (22.3.2018).

Thank you for showing interest towards my project, I’m honored and also appreciate the outreach from the community in both user and vendor side. At this moment in time I’m planning on continuing the development of the project under my own control, but I welcome all feedback and discussion towards and about the project, preferably in the FlexiBMS forum thread itself (FlexiBMS - First prototype board assembled and firmware development started! - Flexible configuration and charging BMS). I’m neither accepting or refusing any possible collaborations or other offers at this time or for the perceivable future. For now the project is so WIP that I don’t want to tie myself down yet. I’ll continue working on it and updating the thread as things progress.

I am in thinking on changing the license of the project to something that would allow:

* Allow people to make their own derivative, based off of the files in the GitHub. I don’t want to stop innovation and want to enable the designs to work, as a launchpad toward their own unique/distinctive project/product.
* Allow the use of the Github files to make a copy of the hardware for their own personal use.
* To protect myself from someone who would link the Github repository directly to a chinese PCB fab and start flooding the market without receiving compensation.
* If/when this product becomes available. If I can’t meet the supply demands I’m open to allow other vendors to produce their own 1:1 batches with a reasonable license fee, so I can get compensation and people be able to get their product.

Personal message:
I want to do this for a living and make a living with it. I find this to be enjoyable and rewarding. I want to give people good products. I want to allow people to make their own derivatives based off of my work and be able to sell those. I want to protect myself from somebody flooding the market using 1:1 clone of my product without receiving compensation. In the case that I can’t supply the demand, I will allow for other vendors to produce their own batches under a reasonable license fee to help ease the possible supply problems (what good is a product you can’t get?).

---

Nothing has been set in stone yet, but these are my current thoughts, so I'm posting this here if people want to have a discussion.

In case you're wondering about how the license fee would work. I mean it as a small compensation per board (5-15 €). Maybe I see there is a supply problem and I can't meet the demand so I decide to allow the production of 200 boards with the aforementioned fee. Vendor X takes up the offer and we make a contract, they pay me license fee and then they are free to produce those 200 boards directly with the files available on github, they are also free to sell those boards at the price they see fit. I personally see this being the fairest to all sides on this issue: Me, Vendor and the end-user.

Thoughts, opinions?
```

---
## \#198 Posted by: b264 Posted at: 2018-03-22T08:07:02.206Z Reads: 145

```
[quote="SimosMCmuffin, post:197, topic:46117"]
link the Github repository directly to a chinese PCB fab and start flooding the market
[/quote]

[quote="SimosMCmuffin, post:197, topic:46117"]
Thoughts, opinions?
[/quote]

Require certain levels of QC to be met in order to use the license.  Some of the east Asian factories just pump stuff out without even testing to see if it works, hence the super low prices.  A bunch of junk on the market just looks bad on your design, even if it was the manufacturer being negligent.  Shipping defective units revokes licenses.



.
```

---
## \#199 Posted by: SimosMCmuffin Posted at: 2018-03-22T12:09:31.819Z Reads: 138

```
Good idea and point altogether. This can be bundled into the contract for the license fees.

I plan on doing my own visual check on the soldering job and then make an automated function/sanity check for the electronics that can quickly be run to test the circuitry.
```

---
## \#200 Posted by: mynamesmatt Posted at: 2018-03-24T05:24:24.172Z Reads: 136

```
How do i get my hands on one/buy one!!!???
```

---
## \#201 Posted by: bimmer Posted at: 2018-03-24T05:25:54.700Z Reads: 130

```
Do you need support? Like financial?
```

---
## \#202 Posted by: SimosMCmuffin Posted at: 2018-03-24T08:31:01.914Z Reads: 141

```
I'm not asking for donations/money at this point in time, because that is not the current limiting factor in the development. It is time. 

I work at a local engineering firm doing hardware, software and a little bit of mechanical design. I Work 8 hour days, 10 hours when you count in travel. Continuing doing the same thing when you get home is a bit rough and usually during the work days the progress is not huge every evening. Usually managing to test one specific thing. Weekends are much more productive. The pay is good, considering I graduated last year from university with bachelor's degree in embedded systems, but I have always been active on my free time, doing interesting projects while trying to incorporate new technologies into them and develop my skill and experience through that.

Here's a run down on how much an hardware iteration costs:
4 layer PCBs, 5-10 pcs - 38€
SMD stencils for bottom and top - 20€
Shipping PCBs and stencils - 55€
Components for a single test board ~ 70€

So I can do a whole round of iteration for around 200€, which is very cheap all things considered. The bigger loss in productivity is the turnover time for the PCBs, which is around 3 weeks, but at least now I can write firmware meanwhile I wait for the new boards to arrive.

I order my PCBs and stencils from **_SeeedStudio_** and components from _**Digi-key**_.
```

---
## \#203 Posted by: b264 Posted at: 2018-03-24T09:11:32.881Z Reads: 143

```
[quote="SimosMCmuffin, post:202, topic:46117"]
I Work 8 hour days, 10 hours when you count in travel
[/quote]

I certainly hope those extra 2 hours are spent on top of an esk8.  I hadn't truly lived life until my commute was on top of an esk8.  No, seriously.  I thought I knew what life itself was.  I didn't.
```

---
## \#204 Posted by: SimosMCmuffin Posted at: 2018-03-24T09:54:29.733Z Reads: 157

```
[quote="b264, post:203, topic:46117"]
I certainly hope those extra 2 hours are spent on top of an esk8.
[/quote]
I wish, but Finland isn't really the ideal esk8 country during the winter, especially with a single wheel drive (grip and torque limited) + the real possibility of turning into a human icicle. pic related.

![IMAG0897|690x389](upload://k03aJrVYZYAMHyazM8otfigthhw.jpg)

But I'm working on a new board iteration as well. Custom deck, dual rear drive, 10S6P watertight/resistant battery pack. And I have been prioritising more ruggedness and all-terrain capability more. Here's the raw board out of the mold. It's shape is based on the Trampa's HolyPro 35, but it's made out of finnish birch veneer, which also has it's contour limitations in the mold, AKA can't do super tight radii, so it's bit more rounded. It was made by one the mechanical designers at the office. You can find him @ https://www.instagram.com/pabloboards
![IMAG0894|690x389](upload://3yeovu1MaiJvTsDKQQRUcuAqcRo.jpg)

EDIT: I think he has managed to get it cut and sanded :smiley: Gonna have to make it rain on him!
![image|690x441](upload://uLzwPEmmesAhNJGdTyQLFvvwdW.jpg)
```

---
## \#205 Posted by: mikenyc Posted at: 2018-03-24T11:22:10.331Z Reads: 152

```
How long before frank sues? Lol
```

---
## \#206 Posted by: Lobap Posted at: 2018-03-24T12:08:00.857Z Reads: 153

```
Great work mate!

I'm in a kind of similar situation, 10-12h work per day then after reaching home keep doing same things... even for your own research, it's quite hard :frowning:

Anyway, your mechanical designer colleague, would ship a board to Spain? My name is also Pablo and they look awesome! I will send him an email.
```

---
## \#207 Posted by: SimosMCmuffin Posted at: 2018-03-24T13:58:56.707Z Reads: 160

```
Found a weird glitch in the hardware while debugging the BMS and it's making this very weird noise. I don't know what's causing this, so I'm just posting a short video of it in case you guys know where it might be coming from?
https://youtu.be/eTbzOaSlkPQ
```

---
## \#208 Posted by: SeanHacker Posted at: 2018-03-24T14:12:11.703Z Reads: 153

```
Hahaha!!! That's definitely a weird sound dude!
```

---
## \#209 Posted by: Pedrodemio Posted at: 2018-03-24T18:00:09.685Z Reads: 150

```
Damn, rick rolled

Can this be the default power on beep?
```

---
## \#210 Posted by: Winfly Posted at: 2018-03-24T18:04:54.984Z Reads: 151

```
em has been gotten. Noice one bro. Can you do a shooting star with it now
```

---
## \#211 Posted by: TarzanHBK Posted at: 2018-03-24T22:02:01.963Z Reads: 158

```
I like mine to have the Darth Vader theme later on :grin:
```

---
## \#212 Posted by: SimosMCmuffin Posted at: 2018-04-04T17:57:20.618Z Reads: 165

```
Oy! I'm writing an update over here!

I'm concluding the 1000 hour pre-prototype BMS standby power use test and below is the graph produced from it. If we assume the 9mA average discharge current over the whole 1000 hours period, then it would come to 9000mAh discharged.

This will be reference to which the future discharge tests will be compared to.
![image|690x414](upload://9ZR9FzYs3f11z8WkMU2MfBoyLpI.png)

As I have tested with the 0.1 HW version, it had roughly 600µA of standby current, but I have looked into the different options of lowering the consumption even more and I have couple ideas and options that I'll try.

Hardware testing has progressed into testing the boost converter's thermal performance. Bulk charging was also tested and temperature wise can handle 5 Amps continuous. Charging FET control needs a bit refining with resistor values, as quite a lot of heat is wasted currently.

![IMAG0919|690x438](upload://qrAagDMMjD4wai3YQjsJzTG49gs.jpg)

I2C and ADC functions have been implemented and the USB driver configured, so I can read and write to/from the module via a serial terminal. SPI will need to be implemented and tested once I get the next board iteration. Below is a capture from the data stream with short explanations for the values. I can manually write the DAC values through the terminal to control the end-point voltage for the boost converter and through that control current. Balance connector is not in use due to the footprint mishap with the LTC6803-3 and the intermittent connection problem.

![IMAG0920|690x489](upload://rMnHRyLK2YUonVtPEl3uoN7m0nI.jpg)

Here's a thermal image of the boost converter boosting 24V up to the 10S 39.7V (at that moment) battery pack in the picture.
100W 24V 4.2A in, 
96.8W 39.7V 2.44A out.
![Screenshot_20180404-202921|281x500](upload://eSrr07Q2bJblYM5YAFFxb39SqAY.jpg)

It's running still quite hot and I'm looking at a possibility to use a synchronous boost circuit to eliminate the diode losses. I'll probably make a standalone test board for the synchro boost circuit and test it with that.

Here's a couple more thermal pictures of the top and bottom of the board. I didn't note the power, but I'm assuming around 80 Watts.

![Screenshot_20180404-191737|281x500](upload://gvEghvGbdbLnSbd6SzVvXZ7Zr30.jpg)![Screenshot_20180404-191644|281x500](upload://95hmZfhmPjG4AwkqWwxnR7T4X16.jpg)

With those things tested, I'm starting the planning on the 0.2 HW iteration with quite a lot to change and improve upon. I have chosen the new MCU and mapped the peripheral pins on it. I'm changing the MCU series to the STM's L4 ultra-low power ARM, thanks to @okashira for suggesting the L4-series, which I then looked at and found to be a pretty good choice in fact.

![IMAG0898|585x500](upload://jqkzNwFbFSN0SJB6hQTimyFZnHE.jpg)

Off-topic:
Did anybody do anything interesting during easter? I bough a 12-pack of berlin donuts and ate 9 of them myself!

![IMAG0907|409x500](upload://iRDqHSm2UoOJXfZ6my3xMIyXYj4.jpg)
```

---
## \#213 Posted by: Kug3lis Posted at: 2018-04-04T17:59:09.172Z Reads: 158

```
I suggest to try out STM32CubeMX for assigning pins on mcu. It also lets you choose mcu based on your needs :)

http://thehackerworkshop.com/wp-content/uploads/2015/05/stm32cube-5.png
```

---
## \#214 Posted by: SimosMCmuffin Posted at: 2018-04-04T18:08:59.894Z Reads: 151

```
I have and do use CubeMX (have it integrated into the AC6 workbench), but I don't like to use it to map the peripheral pins, because you can't show all the possible peripherals for all pins at the same time, so I do it on the paper instead. I can show all the peripherals on all the pins and that helps me personally figure out faster the best combinations of which peripherals to use based on their location in relation to the other peripherals.
```

---
## \#215 Posted by: okashira Posted at: 2018-04-04T18:11:03.817Z Reads: 149

```
Nice. Glad you're trying the L4.
I think there may be a pin compatible L4 that swaps with he F3?
```

---
## \#216 Posted by: Kug3lis Posted at: 2018-04-04T18:11:29.542Z Reads: 147

```
Yeah that's a good point :) I normally map pins myself, as I don't like auto positioning :)
```

---
## \#217 Posted by: Kug3lis Posted at: 2018-04-04T18:13:04.237Z Reads: 140

```
I dont really think it would be pin compatible, but you have to check out which line and package you picking out ;)
```

---
## \#218 Posted by: SimosMCmuffin Posted at: 2018-04-04T18:13:10.692Z Reads: 143

```
Not with CAN support I don't think? I specifically chose the L433CCT6, because it had all the needed peripherals, while still being a low pin count. + low price.

And no external oscillator needed. RTC and USB can be run with internal oscillators.
```

---
## \#219 Posted by: okashira Posted at: 2018-04-04T18:17:04.678Z Reads: 141

```
Thanks for finding that on the battman design. Not surprised there is some issue.
Ultra low power design takes a lot of conscientiousness.
Maybe try to increase the resistor values or if necessary, add another FET to gate it when in sleep mode.
```

---
## \#220 Posted by: Kug3lis Posted at: 2018-04-04T18:20:51.933Z Reads: 138

```
Just a question, why you dont add diode inline of CHG fet to prevent current flowing back from the battery? Isn't this way you will prevent current leakage?
```

---
## \#221 Posted by: okashira Posted at: 2018-04-04T18:21:55.817Z Reads: 137

```
It's a voltage divider so you need the current flow?
no current flow no divider :-D
```

---
## \#222 Posted by: Kug3lis Posted at: 2018-04-04T18:23:05.576Z Reads: 136

```
What do you mean? If you talking about LTC voltage divider then it's for its output voltage or I am wrong?
```

---
## \#223 Posted by: okashira Posted at: 2018-04-04T18:24:44.769Z Reads: 139

```
Oh i assumed it was a voltage divider. No time to look closer at the moment.
```

---
## \#224 Posted by: Kug3lis Posted at: 2018-04-04T18:26:34.434Z Reads: 144

```
If I understand correctly its feedback loop for LTC to keep voltage right, so if you add diode next to CHR FET it will only allow charging via CHR terminal or you can use another FET back in back so that way if the switch is off nothing happens.
```

---
## \#225 Posted by: Kug3lis Posted at: 2018-04-04T18:37:22.586Z Reads: 141

```
Another suggestion is to drop LTC and use your MCU to boost :) http://www.st.com/content/ccc/resource/technical/document/application_note/ec/9c/b0/81/b5/12/4e/21/DM00108726.pdf/files/DM00108726.pdf/jcr:content/translations/en.DM00108726.pdf
```

---
## \#226 Posted by: SimosMCmuffin Posted at: 2018-04-04T18:51:47.234Z Reads: 145

```
I have considered both options earlier already. a Diode would block most of the "back-flow" current, but it would also introduce more heating when charging with either charger input and as can be seen, the board is already running hot enough. Drain-to-drain FETs are tricky due to the space problem + driving them both + doubling resistive losses in conducting mode. But as I said earlier I'm gonna look into the options and then gauge the feasibility of the implementations.
```

---
## \#227 Posted by: Pimousse Posted at: 2018-04-04T19:03:55.997Z Reads: 141

```
Thank you very much for keeping us updated !
That's a real and freaky R&D job !
```

---
## \#228 Posted by: SimosMCmuffin Posted at: 2018-04-09T13:06:19.850Z Reads: 149

```
Here's the current 0.1 -> 0.2 HW changelog, this also works as a reminder for myself and I can update and change this post to show how things are progressing. These changes haven't necessarily been done yet, but are in the works or waiting.

* External Led & switch + Comms connectors changed from THT JST-XH to SMT JST-PH (**done**)
* MCU changed from STM32F070CBT6 to STM32L433CCT6 (**done**)
* External oscillators removed due to being unnecessary with the new MCU (**done**)
* CAN support added to Comms connector, USART can be connected using solder bridges (**done**)
* Power delivery done via LTC6803-3's 5V linear output and 5V from the buck converter, which are then fed to a 3V3 LDO. Buck converter can be disabled when going into low-power state and keep MCU powered via the LTC6803-3 5V going to the LDO (**done**)
* LTC6803-3 footprint changed to the correct one (**done**)
* Balance circuit resistors changed from 0603 to 0402 package to save some space and give a bit more tolerance with the soldering (**done**)
* Buck regulator TVS protection diode switched from SMC to SMA to save space (**done**)
* Boost converter electrolytic caps upgraded to more fitting ones for the application (**done**)
* Ceramic capacitors added to the boost converter's input and output
* Ground plane partitioning to isolate the noisy, higher current areas from the analog and logic side
* Buzzer control pin moved to a DAC enabled pin
* ADC sense voltage dividers changed to higher resistance connections to decrease quiescent currents (**done**)

I decided against moving to the synchronous boost circuit for now, because it proved to be a real headache with the layout. It doesn't want to easily fit in to the board, so I'll probably do a standalone test board for it to test it out.
```

---
## \#229 Posted by: Kug3lis Posted at: 2018-04-09T16:22:31.721Z Reads: 144

```
[quote="SimosMCmuffin, post:228, topic:46117"]
0402
[/quote]

Did you mean imperial code right? Because metric 0603 is already small and if you go smaller it would be even bigger pain to solder :D

[quote="SimosMCmuffin, post:228, topic:46117"]
MCU always ON when battery connected via LTC6803-3 Vreg-pin and a 3V3 LDO (can only source 4 mA max)
[/quote]

Is it enough for MCU 4mA?
```

---
## \#230 Posted by: SimosMCmuffin Posted at: 2018-04-09T17:51:59.532Z Reads: 146

```
[quote="Kug3lis, post:229, topic:46117"]
Because metric 0603 is already small and if you go smaller it would be even bigger pain to solder :smiley:
[/quote]
The balance circuitry is so dense that the smaller footprint would actually give a bit more breathing room around the components themselves, so they don't as easily jump to the neighboring pad during soldering. It's already hard to place the components, because the tweezers ends feel so big :wink: . by having the smaller resistor package it would give a bit more breathing room around them, making placing them and the leds a bit easier.

The resistors are already in each others keep out areas with the 0603 package in KiCad, so they are really packed tight.

![IMG_7326|690x323](upload://yLs3N3Lip1Z3ULsCDD61lPtTyQL.JPG)

[quote="Kug3lis, post:229, topic:46117"]
Is it enough for MCU 4mA?
[/quote]
It's enough to keep MCU powered in it's ultra low power state. When going into standby mode, shutdown all other ICs and then disable the buck converter and it's LDO and switch to the LTC6803 LDO regulator to keep the MCU still powered. Going into the active state, activate buck converter and switch it's LDO on and then the LTC6803's one off.

This way I can keep the MCU powered up always when the battery is connected, so I can keep the RAM intact. Then check every now and then if the external button/switch is pressed or if a charger is connected and then switch to a active state.
```

---
## \#231 Posted by: Kug3lis Posted at: 2018-04-09T19:26:15.476Z Reads: 143

```
and your bleed resistor size is? If they are this small it would take forever to balance for e.g. 10Ah pack...
```

---
## \#232 Posted by: SimosMCmuffin Posted at: 2018-04-09T19:40:38.948Z Reads: 141

```
Bleed resistors are still on the other side of the board and it's a 0805 package with a decent power rating.
Bleed current should be a little less than100 mA, with ~80 mA through the 51 Ohm bleed resistor and ~16 mA through the LED.
```

---
## \#233 Posted by: SimosMCmuffin Posted at: 2018-04-10T19:45:38.217Z Reads: 145

```
Here's the plan on how to support both USART and CAN on the same connector pins:
![image|594x425](upload://kxPPbq3QpMnXPLOcyW8K65PtzXl.png)

By default CAN is used and the communication line should be fault tolerant, but the CAN transceiver can be disabled with software, so the pins can be switched to USART use, with the solder bridges bridged.

The +3V3 line is also software controlled, so the external device can be powered off, when going to standby state from active state for example. The +3V3 line isn't fault tolerant, so don't go connecting that to +5V power anywhere.
```

---
## \#234 Posted by: Pimousse Posted at: 2018-04-12T06:36:26.714Z Reads: 134

```
Regarding the balacing LEDs, are they really needed ?
Battman has also those leds but thie device (BMS)is meant to be embedded and enclosed, so no vision on any LEDs.

(That's basically why I wanted to externalize the main RGB led and use an Adafruit RGB led switch instead).

Anyway, thanks for the changelog, that sounds really amazing !
```

---
## \#235 Posted by: SimosMCmuffin Posted at: 2018-04-12T07:58:50.226Z Reads: 146

```
[quote="Pimousse, post:234, topic:46117"]
Regarding the balacing LEDs, are they really needed ?
[/quote]

Technically, no. Development wise, they are a nice thing to have.

In testing phase especially they are a good visual feedback on the behavior of the balance circuitry. I can just with a glance see if something should be balancing, but isn't or if something shouldn't be balancing, but is. If I can't visually inspect the state of the balance circuit I'll have to get in there with a probe head to measure voltages and that can be challenging, so you don't accidentally short something while you're poking in there. Then consider that it's another user that is having a problem and they can't just tell me if the Leds are on or off, which makes possible troubleshooting harder.

For everyone's information, _**I managed to break the microcontroller and the USB 3V3 regulator on the 0.1 test board**_, by accidentally connecting the oscilloscope probe head and ground the wrong way around on the battery lead terminals. Seems like the components didn't appreciate the -+40V Volts on them...
USB port on the PC was ok. So let's just say that 0.2 HW priority has been elevated.

[quote="Pimousse, post:234, topic:46117"]
That’s basically why I wanted to externalize the main RGB led and use an Adafruit RGB led switch instead
[/quote]

a Normal RGB led with discrete diodes is gonna be a challenge to figure out how the connectors should be done, because you need 3 signals wires and there isn't really room for bigger connectors. It would be much easier if there was a pushbutton with something like a WS281x  RGB led integrated, as you would only need 1 data signal to that.

EDIT:
+ we can only use the +3V3 line to power any external Leds, so the voltage is also limiting.
```

---
## \#236 Posted by: Pimousse Posted at: 2018-04-12T08:05:09.389Z Reads: 132

```
Can't you just look at at serial monitor (even better a simple program) to have all the balancing info ?
I'm agree that LEDs are very convenient for troubleshooting, but as you're looking for room, removing them help you this way.

[quote="SimosMCmuffin, post:235, topic:46117"]
It would be much easier if there was a pushbutton with something like a WS281x  RGB led integrated, as you would only need 1 data signal to that.
[/quote]
That was the first device I looked for. But no luck to find it.
Maybe by tweaking an RGB one by adding a ws2812 chip can be the solution.
```

---
## \#237 Posted by: SimosMCmuffin Posted at: 2018-04-12T08:07:49.585Z Reads: 135

```
[quote="Pimousse, post:236, topic:46117"]
Can’t you just look at at serial monitor (even better a simple program) to have all the balancing info ?
[/quote]

The problem is that the software might say the something is balancing for example, but it actually isn't. I can't verify the actual behavior from just the serial terminal. What if there is a bad solder joint in the balance circuitry and it can't actually balance, but the firmware might be physically unable to verify that.

But, yes for the fact that removing the Leds and their front resistors, would free up space from the board and the balancing circuitry could be packed in even tighter.
```

---
## \#238 Posted by: Pimousse Posted at: 2018-04-12T08:22:22.642Z Reads: 127

```
Oh yes, hardware wise, this is the only way to go. Sure.
Are you planning to remove them once your design will be validated ?
```

---
## \#239 Posted by: SimosMCmuffin Posted at: 2018-04-12T08:29:10.286Z Reads: 134

```
It depends on a couple factors.

Do we need more space on board for something else and the balance circuitry has been tested and proven to work? Then it's a possibility.

We don't need more space on the board and the balance circuitry has been tested and proven to work? Maybe just leave the Leds and their resistors un-populated in this case.

Balance circuitry non-proven or tested to work? I'd like to keep the Leds populated.
```

---
## \#240 Posted by: riva_00 Posted at: 2018-04-12T08:45:46.302Z Reads: 134

```
I think that you need to consider a few factors in regards to the LED's.

How good are they (so what do they provide).
How expensive are they (not just price but board space and such)
who do they target (n00bs, veterans or everyone)

Pimousse said that this meant to be embedded and enclosed, but is it? I'd personally cut a hole in my enclosure and put some perspex over to keep a seal and be able to see it, either that or have the lights travel up some fiber to the side of the enclosure.
The muffin could also use the design for more than just Esk8, what if someone bought it to charge LiPo/LiIon packs outside the case for testing. (i'm not great at circuitry so i don't know if this is a good idea).

Best validation i can think for the LED's is the fact the raspberry Pi has them. So many forum posts where the 1st thing someone asks is what LED's are lit, they're just so helpfull.
It seems you don't personally want them pimousse, but i'm guessing you're in the minority (just a guess though)
```

---
## \#241 Posted by: Pimousse Posted at: 2018-04-12T09:42:50.069Z Reads: 128

```
AFAIK, no build embedding a BMS has a transparent window to see any LEDS. Same for VESCs.
So, am I really the minority ?

Personnally, I see a BMS as a device that free your time/mind up by just plugging your board on a laptop-like charger and takes care about the battery for you.
Isn't it ? (ok, that's more sophisticated, I know)

Based on that statement, why would I check any kind of LEDs rather than the main one telling me if it's charging, dis/charged or even faulty ?

This is just a thought, to be argued for sure. :slight_smile: 

 @SimosMCmuffin : your 3 options make sense. Let see which way you'll take. ;)
```

---
## \#242 Posted by: SimosMCmuffin Posted at: 2018-04-12T10:05:24.487Z Reads: 131

```
[quote="Pimousse, post:241, topic:46117"]
your 3 options make sense. Let see which way you’ll take. :wink:
[/quote]

For the 0.2 HW, the Leds are staying in, because I couldn't test the balance circuitry, because I had the wrong footprint for the LTC6803-3, but managed to botch it on. The connections were unreliable so I didn't trust them enough to start testing the balance and sense connections.

[quote="Pimousse, post:241, topic:46117"]
Personnally, I see a BMS as a device that free your time/mind up by just plugging your board on a laptop-like charger and takes care about the battery for you.
Isn’t it ? (ok, that’s more sophisticated, I know)
[/quote]
FlexiBMS needs to be software configured for your setup, but I would recommend also testing at least by the cell charge voltage and balancing, before burying it inside the enclosure and forgetting about it.
```

---
## \#243 Posted by: Pimousse Posted at: 2018-04-12T12:31:00.856Z Reads: 134

```
[quote="SimosMCmuffin, post:242, topic:46117"]
FlexiBMS needs to be software configured for your setup, but I would recommend also testing at least by the cell charge voltage and balancing, before burying it inside the enclosure and forgetting about it.
[/quote]
Sure ! There is always a commissioning phase.
By this sentence, I meant the spirit of any BMS.
```

---
## \#244 Posted by: banjaxxed Posted at: 2018-04-12T21:02:29.657Z Reads: 132

```
I think the license will allow you to remove them and respace for minimalist concerns once @SimosMCmuffin is happy  no?

To me as a non-EE person who is only able to grasp half of what is going on in this thread I think it's just dandy
```

---
## \#245 Posted by: SimosMCmuffin Posted at: 2018-04-13T05:16:23.658Z Reads: 143

```
[quote="banjaxxed, post:244, topic:46117"]
I think the license will allow you to remove them and respace for minimalist concerns
[/quote]

Yes, because I would say it doesn't fall under the strict 1:1 clone, because they can't directly use the files from the Github, but will have to see if even I will remove them with further development.
```

---
## \#246 Posted by: SimosMCmuffin Posted at: 2018-04-16T16:27:57.054Z Reads: 151

```
Side topic, but today I got my first ever self-designed fully assembled PCBs that I designed in work for a customer! The boards were all designed by me, with couple feedback iterations between designs with the customer. I also sourced all the components to fit the customer's specifications. (Customer info has been removed for NDA purposes and I probably can't tell what the specific application of this board is).

![IMAG0967|690x404](upload://qUuF9IZ8y8KlvmBDrQEcEYBCNtg.jpg)
![IMAG0966|690x107](upload://4x5Ml9XI1zIr29IgPePsEX3irLG.jpg)
![IMAG0968_BURST004|690x287](upload://xePzlQIZZbDGOjCCt9PngbjQ0tT.jpg)
```

---
## \#247 Posted by: uigiroux Posted at: 2018-04-16T16:57:33.027Z Reads: 143

```
That looks incredible!
```

---
## \#248 Posted by: SimosMCmuffin Posted at: 2018-04-23T19:07:41.942Z Reads: 147

```
Update,

Slow progress last week, was working overtime on most days and bought Far Cry 5 and needed to finish before I could focus on anything else properly :blush: .Got a lot done on Sunday and today.

Everything is electrically connected on the board, but I need to go through and improve trace widths where needed. Wire pads need to be placed and I'm gonna try to do some separation between the high current and low current grounds for improved noise performance.

![image|690x381](upload://nqN3bGwvsc5L7SuHTRpOv5f0bzf.png)
![image|690x305](upload://6znBK9nFx4dQYdj40FGVAAYlt8k.png)
![image|690x305](upload://s9PqjNPb6Oz8ltDt5a4KuTfTkzQ.png)
```

---
## \#249 Posted by: banjaxxed Posted at: 2018-04-23T19:39:39.545Z Reads: 142

```
Looking great
```

---
## \#250 Posted by: SimosMCmuffin Posted at: 2018-05-11T18:59:38.499Z Reads: 140

```
Update,

Boards were ordered last weekend, I'll have them next week. Github repo has been updated with the 0.2 files ( https://github.com/SimosMCmuffin/FlexiBMS_hardware ), BOM still needs a review and I'll order the components.

Things are slowly progressing and I'll update again after I get the new board assembled.
```

---
## \#251 Posted by: Pimousse Posted at: 2018-05-15T13:15:06.848Z Reads: 140

```
Oh I missed the last update. Nice !
I would have suggested (but too late) to extend the PCB somehow under the JST connector to avoid too much stress in solder joint when plugging/unplugging balance plug.

Is it a real concern or not ?
Can't wait to see the assembled boards ! Keep the good work !
```

---
## \#260 Posted by: SimosMCmuffin Posted at: 2018-05-22T15:54:55.932Z Reads: 142

```
Update,

I have new boards and components. Assembly and testing will begin now.

![IMAG1003|690x276](upload://rFbC8aC8ciCMD1LdvFagEHe62OV.jpg)

[quote="Pimousse, post:251, topic:46117"]
I would have suggested (but too late) to extend the PCB somehow under the JST connector to avoid too much stress in solder joint when plugging/unplugging balance plug.
[/quote]
It's a 13 pin and through hole component, if the solder job is done properly it'll be **very** sturdy connector and won't care about little mechanical stress. I'd be more worried about the balance wires getting pulled out of their crimps.
```

---
## \#261 Posted by: SimosMCmuffin Posted at: 2018-05-22T19:12:57.722Z Reads: 140

```
First components soldered!

![IMAG1005|690x390](upload://2p1aP9Jnjfpq50ouWjtmuTmZRfH.jpg)

The board will slowly progress on a day-by-day basis and I'll drop updates, as things progress once again.
```

---
## \#262 Posted by: SimosMCmuffin Posted at: 2018-05-23T19:28:06.921Z Reads: 137

```
Double side action. LTC6803-3 and STM32L433 soldered + 5V and 3V3 lines checked.

![IMAG1006|690x389](upload://fGPIN5zrFfP25HU7o4S0idYYAhN.jpg)![IMAG1007|690x389](upload://wPNyrZajio6SkAQOD7wQuFfq5iJ.jpg)
```

---
## \#263 Posted by: Kug3lis Posted at: 2018-05-23T19:48:55.996Z Reads: 130

```
Hehe going to use same MCU for single group balancer :P Do you have maybe some measurements on current consumption?
```

---
## \#264 Posted by: SimosMCmuffin Posted at: 2018-05-23T20:04:09.746Z Reads: 129

```
Do you mean for charging or discharge?

Although I'm likely going to use the ISL28022 for both, but with different shunt resistors.
```

---
## \#265 Posted by: Kug3lis Posted at: 2018-05-23T20:08:45.862Z Reads: 132

```
No no I meant for MCU :) I will have 15 of them running so I am bit concerned :D
```

---
## \#266 Posted by: SimosMCmuffin Posted at: 2018-05-23T20:17:54.592Z Reads: 143

```
15 MCUs O_o ?!

Mental.

The current consumption is very dependent on the power and run mode. I would refer at this point to the STM32L433XX spec manual which has a **TON** of different current consumption specs for the different running modes at different operating conditions as shown below.

![image|690x301](upload://i0PIKGVtmkg8wmYCRk0xw8J7zs8.png)
![image|690x405](upload://3mLxqdYSWQTCUnprxEBdzLgowu9.png)
![image|460x500](upload://bZxD7diqr2kSn9NKlrGBKsi4hGH.png)
```

---
## \#267 Posted by: Kug3lis Posted at: 2018-05-23T20:21:04.117Z Reads: 138

```
Yeah I read datasheets, was just curious how they act in the field :)

Just to give more context I am building my battery as 15 x 12S1P groups each of them will have PCB on top with LTC6803 (cheap good balancer IC) + STM32L443 (STM32L0 eats more current than L4) also 6 temp sensors and 1 x AD8418 bidrectional current sensor :) All of them will be running as I2C slave and communicate to main MCU :slight_smile:

I want to keep track of all my 18650 cells and keep them in good balance I will also try to apply all those scientific methods for biggest cycle ratio and capacity :P
```

---
## \#268 Posted by: Deckoz Posted at: 2018-05-23T20:40:33.636Z Reads: 142

```
[quote="Kug3lis, post:265, topic:46117"]
15 of them running so I am bit concerned :smiley:
[/quote]

Why?

Just use max chip multiplexer ![09056-01|500x500](upload://gnmkg2KJD3as1pRTN68zaaCtF1k.jpg)
```

---
## \#269 Posted by: Kug3lis Posted at: 2018-05-23T20:42:20.716Z Reads: 133

```
For what? (I didn't got the point) I am using 15 MCU cause I want each block to independent from whole system, in case it goes bad or etc I could disconnect one block and still have working pack :)

It would be kinda modular but not hotplug style system :) Plus its easier to balance this way 15P pack :D
```

---
## \#270 Posted by: Deckoz Posted at: 2018-05-23T20:47:04.296Z Reads: 132

```
I figured you, we're using that many to monitor individual cells and didn't have enough pins. Not having separate 1p packs
```

---
## \#271 Posted by: Kug3lis Posted at: 2018-05-23T20:48:01.290Z Reads: 134

```
Yep I making separate 12S packs :)

![image|690x427](upload://jOZwnVMomETTuVuzh3gFrwsla5l.png)

This will be going on top of 2 floor 6 cell length group


Sorry @SimosMCmuffin for offtopic :P
```

---
## \#272 Posted by: fedestanco Posted at: 2018-05-23T20:50:31.701Z Reads: 130

```
[quote="Kug3lis, post:267, topic:46117"]
LTC6803 (cheap good balancer IC)
[/quote]
Good for sure. Not much cheap though. I remeber I paid something like 9.5€ each for the group buy. 15 of them will cost more than the battery itself ;) (probably not)
```

---
## \#273 Posted by: Kug3lis Posted at: 2018-05-23T20:51:54.411Z Reads: 126

```
I have them already from private works ;) Bought whole pallet for like 3 eur/ea
```

---
## \#274 Posted by: fedestanco Posted at: 2018-05-23T20:52:40.022Z Reads: 125

```
Man this is great news. Can you keep some for the next diebiems group buy?
```

---
## \#275 Posted by: Kug3lis Posted at: 2018-05-23T20:54:14.672Z Reads: 134

```
Lets move discussion to my topic :slight_smile:

http://www.electric-skateboard.builders/t/mark-48-landyachtz-evo-39-2018-fatboy-1-3-tb218-drivetrain-fatboy-solidcore-wheelhubs-6-5-trampa-aps-6374s-170kv-3-2kw-focbox-12s15p-panasonic-pf/54572/64
```

---
## \#276 Posted by: Pimousse Posted at: 2018-05-24T13:55:29.960Z Reads: 129

```
Just for curiosity, what is your assembling process ?
First LTC and MCU and power stages then you check by powering ?
I'm not an Electronics Engineer, but learning to become one :smile: so if you have some advices, I take them all !
```

---
## \#277 Posted by: JTAG Posted at: 2018-05-24T14:24:05.214Z Reads: 129

```
Part by part is for the WEAK :smiling_imp:.
```

---
## \#278 Posted by: Kug3lis Posted at: 2018-05-24T14:31:44.414Z Reads: 129

```
I start by soldering MCU with enough components to power it up so for e.g. VREG and MCU and etc if its recognized by programmer then I continue :D
```

---
## \#279 Posted by: SimosMCmuffin Posted at: 2018-05-24T14:50:42.299Z Reads: 139

```
I personally like to assemble everything in "blocks" (at least in non-tested designs). 

I started first with the voltage regulators and then confirmed that they were supplying the correct voltages, because if I hadn't and I had started with the MCU, DAC, CAN or any other ICs that are powered from those regulators. They might have blow if the regulators were badly soldered or faulty. This approach is about making sure the very basic things are okay before putting anything else on the board.

Second thing is figuring out the best order to start placing components based on their size and location. You don't want to put the tallest/highest things on first and trying to solder components on between high components. This is about just making the assembly progress easier and putting components on in a smart order. Although this approach is more relevant to tightly packed boards, as you might be space limited. With sparsely populated boards this isn't as much of an issue.

Also, hot air reflow soldering might look intimidating and difficult, but it really isn't. I personally thought this way too before I actually bought a 50 euro hot air station from ebay and started soldering on my first Quad-sided IC. I was more pissed off that I hadn't tried it sooner, so easy. SMD components all the way from there onwards for me. I bought some soldering paste and flux from digi-key like 3 years ago and I'm still using them. Might not be the most fresh things, but still solder and work fine. A decent basic soldering iron is also recommended as you'll have to clean up things every once in while, like solder bridges between component legs after hot air reflow with a bit too much solder paste.

Below are some pictures of my tools, which are very basic and affordable, but very capable once you learn how to solder and work them.

![IMAG1008|690x462](upload://8BBTyAhCAKchlrFnPNq9tK0vv9a.jpg)
![IMAG1009|690x389](upload://20tbfx6qsaBvBgiXSKCKTo988RL.jpg)
![IMAG1010|690x389](upload://datuUVfEvkQbtPjIFM16ktxBoaR.jpg)

Generally, try to come up with projects that motivate you to make things and try to incorporate some small new things always or often so your experience and skill field expands. That's how I've done it since trade school, just making stuff that interested me and trying new things.
```

---
## \#280 Posted by: Pimousse Posted at: 2018-05-24T14:57:30.169Z Reads: 127

```
Thank you so much for this amazing reply.
I knew that I'll arrive to the SMD game soon or later but you convinced me that it may be sooner than later :smile:
```

---
## \#281 Posted by: Kug3lis Posted at: 2018-05-24T15:26:45.861Z Reads: 130

```
Oh right I forgot about Vreg side first test to make sure it works correctly
```

---
## \#282 Posted by: SimosMCmuffin Posted at: 2018-05-26T17:05:23.239Z Reads: 140

```
More components have been soldered and MCU has been hello worlded.

Not quite sure, if the 0402 resistors in the balancing circuits made the assembly any easier compared to the more cramped 0603 resistors in the 0.1 .

![IMAG1011|571x499](upload://zSEbDAsxdKBKCzbbcKIrm3foT4g.jpg)
![IMAG1012|363x500](upload://9czhEB1H59MTMzEpfRP7gUuCzUC.jpg)
https://media.giphy.com/media/MnDTE2vtDdpj4bUh7s/giphy.gif
```

---
## \#283 Posted by: Kug3lis Posted at: 2018-05-26T18:07:30.081Z Reads: 133

```
Arent balancing resistor bit too small? how much current are you going to drain?
```

---
## \#284 Posted by: SimosMCmuffin Posted at: 2018-05-26T19:15:20.389Z Reads: 134

```
The actual power bleed resistors are the 0805s on the bottom side next to the FETs, balancing current should be around 90 mA.

Resistor current: 4.2V / 51Ohm = ~82 mA
LED current: (4.2V-1.7V) / 120 Ohm = ~20 mA

but the P-fets Rds(on) will add some more series resistance, so both currents will be a bit lower.
```

---
## \#285 Posted by: Kug3lis Posted at: 2018-05-26T20:05:22.905Z Reads: 126

```
Will it be enough to balance like >10Ah packs?
```

---
## \#286 Posted by: b264 Posted at: 2018-05-26T21:21:43.818Z Reads: 126

```
What about >50Ah packs?  LoL still 2A charge though so no worries
```

---
## \#287 Posted by: SimosMCmuffin Posted at: 2018-05-26T21:45:42.174Z Reads: 135

```
[quote="Kug3lis, post:285, topic:46117, full:true"]
Will it be enough to balance like &gt;10Ah packs?
[/quote]

If the cells are healthy, they won't start drifting a lot in use, so not a lot of balancing might be necessary to keep the pack in check after the initial balancing after building the pack. If it takes a lot of balancing time at the end of the charging , then that would indicate more that some of the cells are either damaged or not-up-to-the-task compared to the rest of cells. This was the case with my first DIY 4S5P pack of LG MJ1s. One particular series cell would always be the lowest voltage and warmest out of all the series cells, but for some reason reach the balancing voltage first. I concluded that there was something going on with those particular series cells.

Even if there is need to balance during charging, as long as the pack is otherwise relatively balanced, by the time you get to balancing you're already somewhere +95% SoC, so you're not losing much range if you don't let it balance and just head out for cruising.

The first working prototype will go into my 10S6P 35E pack build with nominal capacity of around 19,5 Ah, so I can give more detailed reports with it's performance on that. Can't see any real problems in this point in time.


[quote="b264, post:286, topic:46117, full:true"]
What about &gt;50Ah packs?  LoL still 2A charge though so no worries
[/quote]

What are you building :smiley:? xS+20P packs? Those are starting to be on another scale capacity wise and be more fitting for a bigger BMS as a whole when compared to compact Esk8 battery packs. 

Possible to still balance over time and monitor cell voltages via CAN, USART, bluetooth or USB.
```

---
## \#288 Posted by: SimosMCmuffin Posted at: 2018-05-27T19:12:07.267Z Reads: 139

```
More components soldered, programming has begun, LTC6803-3 has been tested and has been confirmed to be in working order.

![IMAG1013|690x472](upload://8hMP0U9RRyz7Dor9oVf9vON00O4.jpg)
![IMAG1014|614x500](upload://4QnmB6A5zKbuXmBkLwqSXGjMBxc.jpg)

Pretty much only the boost converter components aren't on yet.
```

---
## \#289 Posted by: SimosMCmuffin Posted at: 2018-05-28T19:35:06.501Z Reads: 133

```
Fully assembled!

![IMAG1015|602x500](upload://mvtfawMpbGP9hLdGgHQj8fpdVoA.jpg)
![IMAG1016|611x500](upload://zGuS5P3bSeG0a0VjPpszKdZ9u9n.jpg)

I suppose it's time to start testing and coding. 

Boost converter noise performance is going to be under particular supervision, because the 0.1 had **terrible** ringing at it's output, but the electrolytic capacitors have been optimized and a nice bunch of ceramic caps have been added to address the issue, but testing will confirm how it works.

PS. I'll try to sort out the BOM finally and update it to the repo.
```

---
## \#290 Posted by: uigiroux Posted at: 2018-05-28T19:37:41.155Z Reads: 126

```
Are you planning on making a production run of these?  I imagine many would sign up to buy this beauty! :heart_eyes:
```

---
## \#291 Posted by: SimosMCmuffin Posted at: 2018-05-28T19:48:38.489Z Reads: 133

```
Once I have tested it and if it has passed with no major or critical flaws I might do a hand assembled small batch that I will ship out (maybe free or not) to couple willing beta testers who preferably are esk8 power users and familiar with electronics, so they can test it and give feedback.


I refer back to a post on this particular issue couple months back
[quote="SimosMCmuffin, post:162, topic:46117"]
Do you need any beta testers?

I will most likely need/want at some point, once the module makes it through my own performance tests and I fix any obvious HW mistakes. Once that time comes I will inform about it in this thread and open up some kind of  application form for a limited amount of people. Modules might be provided free of charge, except for shipping and once the beta ends I will either let participants keep their modules for free-of-charge or pay for it with a discounted price for their help and effort.
[/quote]
```

---
## \#292 Posted by: Pimousse Posted at: 2018-05-28T19:50:44.664Z Reads: 126

```
Nice piece of art Simos !!!
And now good luck for the coding part !
I might be interested into particpating to the beta program ;)
```

---
## \#293 Posted by: SimosMCmuffin Posted at: 2018-05-28T19:59:32.149Z Reads: 121

```
[quote="Pimousse, post:292, topic:46117"]
Nice piece of art Simos !!!
[/quote]

Now let's hope it doesn't stay just as an art piece.

> the expression or application of human creative skill and imagination, typically in a visual form such as painting or sculpture, producing works **to be appreciated primarily for their beauty or emotional power.**
```

---
## \#294 Posted by: Pimousse Posted at: 2018-05-28T20:21:48.225Z Reads: 128

```
:smile:
Now you're done with the  "beauty" part.
Let's dive into the "emotional power" one. ;)
```

---
## \#295 Posted by: SimosMCmuffin Posted at: 2018-05-29T19:11:37.263Z Reads: 129

```
https://github.com/SimosMCmuffin/FlexiBMS_hardware

Repo has been updated with 0.2 HW finalized files with BOM now up-to-date and available in .csv and .pdf formats.

**PROJECT LICENSE UPDATED**
Project license changed from **GNU GENERAL PUBLIC LICENSE** to **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International**. This is because the project is more of a hardware one than a software one. If you have questions what this means in practice, or at least what I want it to achieve in practive, ask away.

I've also been doing some concept work on an open source remote with flexibility in it's configuration called FlexiRemote (Imaginative, I know right?). It would be based on an arduino nano and Nordic semiconductors nRF24L01 modules and the idea would be to allow the user to 3D-print the case for either thumbwheel with dead man switch or trigger control with switch. I'm also going to put a place for a 0.91" 128x32 OLED display. Charging will be done via the arduino nano's USB-mini connection.
```

---
## \#296 Posted by: Maxid Posted at: 2018-05-29T19:22:42.813Z Reads: 120

```
Why not go for a nodeMCU (or ESP8266 for that matter) - seems to be more performant and cheaper in the end.
```

---
## \#297 Posted by: b264 Posted at: 2018-05-29T19:27:27.271Z Reads: 127

```
Just to be clear to everyone, this license means you can use this design for free **ONLY** if you

A) Retain the original copyright notice
B) Publish any changes you make

So you can use it to make BMS, but not sell them, but if you make changes to the design you legally must publish the changes you made or you are not legally permitted to use this design.

Frequently called "copyleft" in the software world.  It's property of the public at-large and you're not allowed to steal it from the public.

[more information](https://creativecommons.org/licenses/by-nc-sa/4.0/)
```

---
## \#298 Posted by: SimosMCmuffin Posted at: 2018-05-29T19:37:40.427Z Reads: 124

```
[quote="b264, post:297, topic:46117"]
So you can use it to make BMS and sell them
[/quote]

What about the non-commercial part though?
"NonCommercial — You may not use the material for commercial purposes."

I understood this part that by default under this license somebody else would be breaking the license if they were to send the design files from the github as they are to fabrication for the purpose of selling the boards?
This if what I want to protect my work from.
```

---
## \#299 Posted by: b264 Posted at: 2018-05-29T19:55:20.714Z Reads: 124

```
Must have missed that part.  Edited.  Thanks :slight_smile:
```

---
## \#300 Posted by: mikenyc Posted at: 2018-05-29T19:56:18.465Z Reads: 122

```
[quote="SimosMCmuffin, post:298, topic:46117"]
“NonCommercial — You may not use the material for commercial purposes.”
[/quote]

how do you plan on enforcing this against a company like maytech?
```

---
## \#301 Posted by: ShutterShock Posted at: 2018-05-29T22:11:14.479Z Reads: 126

```
I would also be interested in participating in the beta program if it comes into being!
```

---
## \#302 Posted by: SimosMCmuffin Posted at: 2018-05-30T06:17:09.144Z Reads: 127

```
[quote="mikenyc, post:300, topic:46117"]
how do you plan on enforcing this against a company like maytech?
[/quote]
If there is a china seller that sees the potential of making money, I have little doubt that the license would actually stop them from copying the design as is and selling them, but at that point I could have a legal case against them, but I personally see the effectiveness of this being the same as trying to use your leaf blower to stop a tornado, it's just going to at best case, change it's course a little bit, but you're most likely just going to lose more money in the court case than what you would be gaining.

There is actually a quite recent case where something like this happened:
https://www.smh.com.au/business/small-business/flow-hive-stung-by-chinese-ripoffs-20170411-gviyzg.html

Only effective measure I see is to actually remove the github page or make it private, so it is no longer directly available to the public. Thieves usually are after the easy gains. Problem with this, as the earlier statement said, the project would disappear from the public eye and would be only known for example through this forum. But this I say goes against the idea of at least sharing the idea of what you're making and showing how it's done. I personally have used a lot of open source projects to learn and study electronic circuits and feel somewhat obligated to give back to the community.

It is a tricky question and hard problem to solve.
```

---
## \#303 Posted by: Pimousse Posted at: 2018-05-30T06:48:58.247Z Reads: 129

```
Hi @SimosMCmuffin,
I read your schematics (FlexiBMS.pdf) and issued you few (not so valued) comments. :slight_smile:

Thanks for the sharing.
I have some questions though :

- Charge connectors has 3 pins. Is it in order to be able to bypass BoostDAC (e.g. in case of use of a standard CCCV charger) ? Is that not so "dangerous" if the user don't connect to the right port ? Could it be a future improvement by adding a FET that bypass the whole BoostDAC thus letting only 2 pins on the charge connector ?
- I can't find the CAN chip although it's present in the BOM.

I keep studying your schematics. Quite interesting work, a lot to learn again, thanks ! :slight_smile:
```

---
## \#304 Posted by: SimosMCmuffin Posted at: 2018-05-30T07:13:48.715Z Reads: 120

```
If you looked at the "FlexiBMS140418.pdf" or "FlexiBMS.pdf"
they are dated on the 14.04.2018, so those are old schematics. I'll add the up-to-date schematics .pdf of the current ones today.

@moderators
Could it be possible to allow me to update the first post and the topic of this thread? They seem to have been time locked or locked by the mods.
```

---
## \#305 Posted by: Pimousse Posted at: 2018-05-30T07:22:44.735Z Reads: 122

```
Ok, so I don't go further till you upload the last version. ;)
```

---
## \#306 Posted by: SimosMCmuffin Posted at: 2018-05-30T07:33:58.912Z Reads: 132

```
FlexiBMS.pdf schematic is now up-to-date
https://github.com/SimosMCmuffin/FlexiBMS_hardware/blob/master/FlexiBMS.pdf

**Preliminary Beta-tester sign-up opened!**
If you're interested in joining the beta testing phase (if and when it might happen) you can officially list yourself in the following google sheet with some basic information.
https://docs.google.com/spreadsheets/d/1CItw3euHCguWo1JE4JJYVbNvmc4FKBdvPif63ELJipM/edit?usp=sharing
```

---
## \#307 Posted by: TarzanHBK Posted at: 2018-05-30T07:43:31.073Z Reads: 127

```
Done :slight_smile:
```

---
## \#308 Posted by: Pimousse Posted at: 2018-05-30T08:02:03.403Z Reads: 128

```
Me too. :upside_down_face:
Do you already have a cost estimate for the beta ? (could be announced by PM if you prefer).
```

---
## \#309 Posted by: Pedrodemio Posted at: 2018-05-30T13:07:24.933Z Reads: 127

```
What are the final dimensions? I would love to participate on the testing phase, but I think there is no way I can make it fit in my current build, if it’s no too thick maybe I can mount it at an angle to clear some other components
```

---
## \#310 Posted by: Pimousse Posted at: 2018-05-30T13:40:55.768Z Reads: 129

```
Also, could you provide a list of specs ?
Such as, max continuous current for discharge/charge (boost and bulk), Voltage min/max for boost, min cells setup...

(Sorry to rush you).
Still have a ton of questions regarding the HW (but most of them are for feeding my curiosity :innocent: ).
```

---
## \#311 Posted by: SimosMCmuffin Posted at: 2018-05-30T14:40:25.717Z Reads: 144

```
[quote="Pedrodemio, post:309, topic:46117"]
What are the final dimensions?
[/quote]
If horizontal connectors are **not** used (the 13 pin JST-XH balance connector) then dimensions are as follow. Bolt pattern 58x28mm for M3 bolts.
![image|690x210](upload://lqdd51146EAHl6Gorl6QwQRJNLi.png)
![image|690x462](upload://kfQQH5hJYlSA6Oc77oegEzr4rF4.png)

[quote="Pimousse, post:310, topic:46117"]
Also, could you provide a list of specs ?

Such as, max continuous current for discharge/charge (boost and bulk), Voltage min/max for boost, min cells setup…
[/quote]

Note: All voltages are for Li-Ion/Li-Po (3,6V or 3,7V nominal).

- Max continuous current for boost input current is yet unknown, as I need to test the boost converters thermal performance, it is also dependent on how hot of a board people want to run.
- Max continuous bulk charger current (or recommended max.): 5 A
- Min/max series cells: 4-12S for normal operation, possible to use 3S, but boost converter not usable, so have to use bulk.
- Voltage In Min for boost: Have to test for actual min, 9V is datasheet low limit, but 12V have been tested to work.
- Voltage In Max for boost: Recommended is # of series cells * 3V. So, 12V -> 4S, 15V -> 5S, 24V -> 8S. Main rule is that boost supply chargers voltage should not exceed battery voltage, otherwise current will just flow through the boost converter. Personally recommend 12V -> 4S-7S and 24V -> 8S-12S. These chargers are cheap on ebay for LED use. If higher charging power is needed, use a bulk charger.

You're gonna have to ask more for specific specs, because there are a LOT of possible specs I can list. Make list, if you could.
```

---
## \#312 Posted by: Pedrodemio Posted at: 2018-05-30T18:04:27.659Z Reads: 136

```
Thanks, I think I can't fit it, theoretically I have exactly 35mm between my Arduíno and the battery cells, need to open the board to check, but id have to use everything with vertical mount

The beta will include the switch board? if yes and depending on the price i may jump on board, removing the currently anti spark and re routing the wires it may fit

If not my next board will surely include one of these in the planning

![image|667x500](upload://gK2UgbOimgHN1eka4K6u0shVF2l.jpg)
```

---
## \#313 Posted by: SimosMCmuffin Posted at: 2018-05-30T18:16:36.237Z Reads: 131

```
Switch module is not designed yet. this beta will be for the main module.
```

---
## \#314 Posted by: Pimousse Posted at: 2018-05-31T14:00:37.565Z Reads: 129

```
Ah !
So if I understand well, the main module itself will act as a charger only, not managing discharge (but may tell the VESC to stop in case of cell or temperature fault through CAN comm.), right ?

And then, if we want to manage discharge, we just stack the power stage (That's where "FlexiBMS" makes sense :smile: ).
```

---
## \#315 Posted by: ron Posted at: 2018-06-01T23:21:55.811Z Reads: 134

```
Nice BMS ... 
Is it configurable at what time that passed the BMS is enabling the storage discharge mode?
And the configuration of the BMS is done only by PC?
And I love how either momentary or toggle switches are supported... A little detail but nice to be able to use momentary switches...

Thanks in advance.
A great project. Curious how the BMS is going to perform on everyday usage.
How much would it cost for the parts and the PCB overall? Couldn't find an estimate in this thread.
Ron
```

---
## \#316 Posted by: SimosMCmuffin Posted at: 2018-06-02T12:01:41.347Z Reads: 137

```
Basic LTC6803-3 library is functional and I'm doing balance tests
![IMAG1029|690x389](upload://vJhvJV1oAx1Kt3njK5xa3pDAx5D.jpg)

I'm trying to keep the code simple so it is easy to follow and understand what's going on
![image|510x500](upload://xjF9nlLxNzcCJOWsUR9tgHldTC8.png)

[quote="ron, post:315, topic:46117"]
Is it configurable at what time that passed the BMS is enabling the storage discharge mode?
[/quote]
Yes, the time for starting to balance/discharge towards storage voltage, which is also configurable, will be settable. probably in hours between 0-65535 hours, with 0 being disabled for example.

[quote="ron, post:315, topic:46117"]
And the configuration of the BMS is done only by PC?
[/quote]
Can also be done via USART or CAN also, but not implemented yet. You can use a for example a HM-10 bluetooth module and connect to it via smartphone and then read and configure parameters. I would still recommend doing the initial setup via USB and PC, but this point is a bit moot, as the BMS isn't out yet.
```

---
## \#317 Posted by: SimosMCmuffin Posted at: 2018-06-08T19:41:36.973Z Reads: 126

```
Update.

MAX5215 (DAC) and ISL28022 basic libraries created and tested.
Charging tested in both Bulk and Boost mode (manual control in boost for now).

![IMAG1032|539x500](upload://sHbCUxCFrCC5whcm0U3rOUiBm5j.jpg)

Thermal image of the boost converter with 5 Amps constant IN current shown below, temps settled around 88 C @ 23 C ambient.
Bulk charging tested with 5 Amps and the charging FET hovered around 77 C, no picture atm.
![Screenshot_20180608-212348|281x500](upload://zuCAnR51VDvQTBDAbXl3pOxxY2i.jpg)

I'm gonna start testing the charging on my actual battery pack and gonna get more pictures. Also going to start making a library for the necessary ADC functions.
```

---
## \#318 Posted by: TarzanHBK Posted at: 2018-06-11T10:20:57.687Z Reads: 115

```
this lipo looks puffy!
```

---
## \#319 Posted by: SimosMCmuffin Posted at: 2018-06-11T10:28:06.471Z Reads: 121

```
That Li-Po is an old workhorse of mine, which has now been retired for low current bench-top use. It's 3+ years old with a lot of abuse in RC planes and multirotors, so a little bit of puffing up is normal.

This week's goals are to write the ADC library and start working on the automated charging algorithm.
```

---
## \#320 Posted by: TarzanHBK Posted at: 2018-06-11T10:31:59.331Z Reads: 120

```
take in mind that we enclose this bms, so it might get a good amount hotter in shrinktube and packed with other stuff in ABS or Carbonfiber or other stuff kids use these days as enclosure ;)
```

---
## \#321 Posted by: SimosMCmuffin Posted at: 2018-06-11T10:36:31.100Z Reads: 129

```
I'm considering making a custom aluminium heatsink for the bottom side. I believe I can get the board run at decent temperature, if I'm able to spread the heat to a larger area, even in otherwise passive cooling.

I need to get the ADC library sorted out, so I can checking out the measurements from the NTC resistor next to the boost converter's inductor. That could be used to limit the charging power, so it stays under a certain temperature limit, but of course slows down the charging speed. I'l keep you guys updated.
```

---
## \#322 Posted by: b264 Posted at: 2018-06-11T16:23:18.652Z Reads: 123

```
[quote="TarzanHBK, post:320, topic:46117"]
we enclose this bms, so it might get a good amount hotter in shrinktube and packed with other stuff in ABS or Carbonfiber or other stuff kids use these days as enclosure
[/quote]

Don't forget some of us may use plenty of conformal coating as well ;-)
```

---
## \#323 Posted by: Pimousse Posted at: 2018-06-21T13:39:35.254Z Reads: 117

```
Hi @SimosMCmuffin, how is your BMS going ?
```

---
## \#324 Posted by: SimosMCmuffin Posted at: 2018-06-21T16:07:05.006Z Reads: 126

```
Slowly progressing.

Got the ADC library implemented and I'm now working on the automated charging algorithm and intend to get it working on some degree this weekend. 
I'm starting with the bulk charging first and implement the necessary logic flow for detecting the charger, checking if we have positive current flow towards the battery (for example if battery nearly full and charger at very close to battery's voltage then it might be hard to say if a charger is connected), main bulk charging algorithm, current max monitoring, cell monitoring and balancing, temperature monitoring, when to terminate charging, state machine implementation etc.

It's a bit involved, but gotta just start working on it, because it is probably the **most** important feature that needs to work right.
```

---
## \#325 Posted by: JTAG Posted at: 2018-06-21T19:06:26.316Z Reads: 126

```
Yep fun and loads of testing 🤐. And oh man the debugging 🙈. Luckily this is where all the fast and motivating progress is.
```

---
## \#326 Posted by: Pimousse Posted at: 2018-06-22T07:13:02.232Z Reads: 123

```
Wish you all the best for debugging.
I started by implementing all interlocks (over/under voltage, current, temperature...).
This helps to avoid some dangerous situations (like during PID tuning ;) ).
Again, feel free to check why I've coded for Battman..

And for the detection of end of charge, I remember that you should stop when going under 0.03C in CC mode (source : http://batteryuniversity.com/learn/article/charging_lithium_ion_batteries).
Thus, you can differentiate the end-of-charge from the charger disconnection.
```

---
## \#327 Posted by: banjaxxed Posted at: 2018-07-01T20:11:46.990Z Reads: 120

```
Still tuning in here to your forging of another option, not sure if you subbed JTAGs work on the DieBieMS project but it looks like he has managed to pull off push-to-start which is awesome of course.

presumably not a problem for the FlexiBMS project or is there an architectural blocker?

Keep it coming!
```

---
## \#328 Posted by: SimosMCmuffin Posted at: 2018-07-03T07:14:36.528Z Reads: 121

```
He implemented push-to-start on the BMS? Did he go into details on how he implemented it? How much pushing does the board need before activating, I have a couple of hunches how he might have done it.

Update:
Bulk charging has basic implementation, Boost charging has basic implementation.

Boost charging does need a heatsink for proper operation, otherwise the temperature monitoring cuts down the power by a sizable amount. I'm looking into getting something done for it. Thinking of having 4 mm aluminium plate milled from one side to remove some material from some areas so as not for it to touch other 
higher components. It would cover the whole backside.
```

---
## \#329 Posted by: banjaxxed Posted at: 2018-07-03T07:55:44.448Z Reads: 117

```
Here's the skinny 
https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/332?u=banjaxxed

Not sure how much push but suspect very little, a kick against the wheel provides the 5v needed to start the sequence. Can bus is used

Edit: FlexiBMS does not use CAN...but maybe there is still a way to hijack the can power rail and use it even if not using the CAN communication protocol...would be a nice hack
```

---
## \#330 Posted by: SimosMCmuffin Posted at: 2018-07-03T09:14:50.024Z Reads: 117

```
[quote="banjaxxed, post:329, topic:46117"]
Not sure how much push but suspect very little, a kick against the wheel provides the 5v needed to start the sequence. Can bus is used
[/quote]

So is this with software support from VESC or what does it use the CAN bus for? I can see the possibility on how to implement the push-to-start feature with the switch module.

[quote="banjaxxed, post:329, topic:46117"]
FlexiBMS does not use CAN
[/quote]

The 0.2 HW has CAN support. Unfortunately I can't edit the OP anymore to update the projects relevant information.
```

---
## \#331 Posted by: Pimousse Posted at: 2018-07-03T09:22:44.105Z Reads: 116

```
As far as I understand, it's only electrical related, no matter of communication.
When the wheel spins, 5V is generated on the VESC rail.
By using this 5V coming from CANbus wires (including 5V and GND), you may use this 5V to switch your BMS to discharge mode.
```

---
## \#332 Posted by: JTAG Posted at: 2018-07-03T09:36:17.122Z Reads: 118

```
Exactly. I do it trough an opto-coupler, to be safe (and be universal).
```

---
## \#333 Posted by: SimosMCmuffin Posted at: 2018-07-03T12:37:22.299Z Reads: 118

```
I would have first guessed that you're measuring the load-side voltage and when it rises high enough then switch to discharge mode based on that.
```

---
## \#334 Posted by: JTAG Posted at: 2018-07-03T12:50:50.254Z Reads: 120

```
Well, that is also an option but than your measurement system needs to be on, always. My BMS when off, is completely off (cant power itself up), it is to complex to explain how it works but that can be found in the schematics.
```

---
## \#335 Posted by: SimosMCmuffin Posted at: 2018-07-15T18:18:11.151Z Reads: 126

```
Heartbeat.
I've been on holiday from work and been testing and programming the boost charging along side cruising around a lot on my new board. Have been doing a lot of other stuff also, so not huge leaps in development, but some necessary solutions have been thought up for one thing. 

I have decided to prototype a heatsink that would cover the whole bottom side of the pcb with thermal pad transferring the heat away from the boost converter's schottky diodes and mosfet. Below are a couple test fitment mock-ups with a 3D-printed piece.

![IMAG1097|690x245](upload://cXhUWcC4XyaQLB5SP4dI5cMEwPz.jpg)

![IMAG1098|690x314](upload://sG9k1V1C5pBIvjwjF4PrmFCkF6R.jpg)

I have been charging (24V 7$ china brick supply) my new pack with 80 watts power and 70 degC temperature limit and it has been quite stable over the whole voltage range with a slight temperature raise towards the full pack voltage. Below is the temporary heatsinking solution attached to the inductor, which is not that intolerant of some extra heat. The diodes and mosfet on the bottom side have been around 77 degC with the onboard NTC reporting around 70-71 degC for the temperature.

![IMAG1099|690x398](upload://skFig4WBFRJC18WxlpOryHEg0QY.jpg)

I have designed the heatsink so that it would be easy to mill from a 4 mm aluminium plate.

![image|690x481](upload://6PZ2Rb8mIR7m4Yk4dCKJfP91rk3.png)

![image|690x377](upload://tIM0aRJRJxUSthQh6HpBiTCNrbL.png)

@Kug3lis You wouldn't be able to recommend anybody on this forum that could mill couple of these heatsinks for a payment?

Once this heatsinking issue has been solved. I believe I'm going to assemble couple more boards and send them out to a few of the testing volunteers, so we can get couple more people hands-on with it and perhaps start collaborating with the software development.
```

---
## \#336 Posted by: banjaxxed Posted at: 2018-07-15T21:53:47.074Z Reads: 113

```
Paging @LukePL & @Minim  as well
```

---
## \#337 Posted by: Minim Posted at: 2018-07-15T22:06:56.004Z Reads: 113

```
I can help you out with a test piece if you dont get help elsewhere. What is the external dimmensions of it (LxHxW)?

I would suggest that the pockets have radius tho as milling them with a 10mm will make a 5mm radius and 5mm 2.5mm and so on. Bigger=quicker cycle time and lower cost for you when you order a bigger batch.
```

---
## \#338 Posted by: LukePL Posted at: 2018-07-15T23:11:20.404Z Reads: 111

```
Thanks for mentioning but I have limited access to cnc right now but for @Minim should be a piece of cake ;)
```

---
## \#339 Posted by: SimosMCmuffin Posted at: 2018-07-16T11:31:33.078Z Reads: 117

```
External dimensions are 65x35x4 mm. 

![IMAG1100|638x500](upload://z3jWEX1txZoJvXtAfO5KeY0Gras.jpg)

I'm changing it slighty so it can be milled with a 10 mm bit. and I'll 3d-print to test it first.

![image|690x395](upload://cBPEs33ts5DjX3l7X4CdBI0U0To.png)
```

---
## \#340 Posted by: Kug3lis Posted at: 2018-07-16T11:45:53.498Z Reads: 110

```
We can make it too ;) Just send use the step file of what you want, don't forget that square holes are impossible so just add some radius :)
```

---
## \#341 Posted by: SimosMCmuffin Posted at: 2018-07-16T21:09:21.026Z Reads: 120

```
@Kug3lis @Minim

![IMAG1101|690x464](upload://6S6uAtDPHoGmc7wRivkcqyOwVwv.jpg)

I tested and fine tuned the geometry. Here's the .step file for the heatsink:
https://drive.google.com/file/d/1roijXmH9vJuJl88sKDpjGNRYAFCyrwT-/view?usp=sharing  

PM me, if you're interested in making 4 pcs of them and well discuss the payment and shipping.
```

---
## \#342 Posted by: SimosMCmuffin Posted at: 2018-07-18T17:10:11.480Z Reads: 120

```
Here's a little practical demo of boost charging.

https://www.youtube.com/watch?v=ZovcY_dLIog&feature=youtu.be
```

---
## \#343 Posted by: SimosMCmuffin Posted at: 2018-08-11T12:04:21.088Z Reads: 112

```
Update.

Heatsink tests have been going on during absence of smaller updates. Many thanks to @Minim for the CNC job and swift completion and shipping. Some dimensional tolerance was there, but not big enough to make the heatsink unusable. Double side adhesive thermal pad was used on the protruding square part seen below in the middle of the heatsink, which makes contact with the double diodes and the N-Mosfet of the boost converter.

![IMAG1126|646x500](upload://hjwLU5CRv1XcWOq7Tk85lWJryEG.jpg)
![IMAG0892_1|548x420](upload://rTFZxQ2MN4cwHEvrUtVxgkbYpCg.jpg)


![IMAG1116|620x500](upload://7CIbrPkgh6EgaXd6z4oLmgQcljC.jpg)
![IMAG1115|666x500](upload://2lvtAnIfjRNO5eZi8OitgnrS7eB.jpg)

Here are some charts made from a long pack chargings. 
Below is an open air log with the BMS hanging outside of the battery case, with no forced airflow over it.
![image|690x463](upload://sAZEP1E19mvluXgB76L5DLmktrT.png)

Log once the BMS was attached to the inside of my battery pack case. I was expecting little bit higher temps, as the plastic case in contact with the heatsink isn't exactly an ideal material to conduct heat, but it wasn't too extreme, I would rather just use lower max temp in the software to lower the running temp, with of course slower charging speed at the higher voltages, as you can see from the temperature climbing higher as the pack reaches higher voltage.
![IMAG1127|690x485](upload://A2yB0N5rMcPUL5rA7Cc3Coi0YyG.jpg)
![image|690x467](upload://uXFYUDgHmne5Qg29N28BXjcMv27.png)

So in general I would say that the BMS is now at a point, in which I will assemble couple more boards and send them out to the interested folks who signed up in the tester form. Hardware wise, I deem it usable, even though I still found couple things to fix or change.  I'm going to build the shopping list to digi-key this weekend and I'll see what things I already have in my inventory to avoid excess parts.

**BUT**, with the results of these tests, they have given me couple things to consider with future development and in what direction to take things.
```

---
## \#344 Posted by: Pedrodemio Posted at: 2018-08-11T12:38:28.003Z Reads: 108

```
Its coming along nicely

This temperature limitation only happens when using the buck converter right? Using an external charger the current can go higher without thermal throttle?
```

---
## \#345 Posted by: SimosMCmuffin Posted at: 2018-08-11T14:09:53.153Z Reads: 114

```
I decided to dedicate a separate post for the design choice conversation and other off topic ramblings, so it doesn't bloat the actual proper project update post above this one.

**Off-topic**
I've been thinking of building an e-bike. Why? My board is somewhat bulky and heavy for example to pop into stores for food trips, but too lightweight and small to trust into not being stolen even if locked into a bike rack. That alongside with wearing padding and a full face helmet doesn't make me want to go indoors either. I think the bike would be just a more usable platform for more things overall. It's also a more stable mechanical platform at higher speeds than a board :wink:. I've been using my board to commute to work and back for roughly couple months now, with each back-and-forth trip being 25km/15mi, so I have been spending about an hour every workday on my board. Plus the bike has built-in mudguards. I have had enough little drizzles and pours happen that I don't want to ride the board if the asphalt is noticeably damp, because it seems to manage to extract every single drop of muddy water from all possible nooks and crevices on the road, unless I want cruddy pant legs (which I don't).

The plan is to buy a normal bicycle and then do an electric conversion for it. I've been eyeing a particular bicycle model to use as the mechanical platform. It's a compact city cruiser with nice back rack, to either put batteries on or cargo and nice saddle - handlebar frame shape to perhaps build a dedicated battery pack into.
![image|690x482](upload://6qMCStiV9sLzsmb34yMaZzEyS1y.jpg)

It's a new area that interests me and works well into working my way into larger scale EVs.

---

I decided to build a monster USB powerbank from my more unknown mystery cells that I got when I extracted my first cells from some ebay laptop battery replacement packs. It's a 1S15P pack. Those white cells are actually re-sleeved by me because the original sleeves we're just in awful condition.

![IMAG1121|580x500](upload://mFRDmxbwhf49v1wcbNmr13P2qDo.jpg)
![IMAG1122|690x415](upload://lwDnSUWeOlxBwtfGotQ0mkB9T6J.jpg)

I then went to a local store and bought the cheapest USB powerbank they had and within 5 minutes of coming home had it disassembled in front of me. The plan was to take the charger / boost-charger PCB and use that as my first interface for the monster pack. The blue cell in the pictures is the one that came with the powerbank.
![IMAG1123|690x389](upload://bWkeCc5tgh5GO6zTgmtCDorjflw.jpg)

I decided to test the capacity of the pack, just so I actually know how much capacity it has (duh). I estimated the pack to be around 36000 mAh, with a single cell being around 2500 mAh and with 15 of them in parallel. Well that was a pretty good guess, because I got 35900 mAh from the discharge test, so pretty bang on :sunglasses: !

I also decided to dig out my solar panels to charge the pack during day time. The large panel in the picture below is a big 150 Watt panel, with a smaller 15 Watt one being sandwiched in the windows inner and outer panes behind it (shadow visible). Now this setup is woefully un-optimized, but I can't be bothered to actually attach the solar panel outside, as I now live in a flat without a balcony on the ground level. So craptastic placement + it's wired directly to the powerbank without a buck converter in between so horrible efficiency either way! But it is charging it and that's all that matters for now.
![IMAG1128|690x389](upload://cDEaEhbueSwNi9iyz10EYiCkCFI.jpg)

I'm thinking of designing a synchronous buck and boost converter, for self education/learning purposes. I'll bring this back up in the future development ponderings. Buck converter would be useful to make a MPPT (Maximum Power Point Tracking) charger for solar application and for higher power and efficiency battery pack charging (discussed further later). Boost converter would be for the USB powerbank to boost the voltage from the 1S15P Li-Ion pack for the 5V USB port.

---
**Project development ponderings**
_Thermal management and optimizing charging._

So, with the test results from the thermal performance of the BMS with the heatsink, I have come up with a couple observations. First of all, the heatsink works. It manages to pull a lot of heat from the boost converter section and more importantly keeps the mosfet and diodes cooler for longer lifetime. The inductor doesn't care as much about it's running temperature. Thermal images showed the inductor to run about 10-15 C hotter than the reported PCB temp.

The problem is that the heatsink can't really by itself get rid of the heat efficiently. It does provide a good thermal mass and surface area onto which you could couple some proper fanned heatsink to passively radiate the heat off, but considering that the BMS is meant to be integrated into the board's enclosure it would be very dependent on the material of the enclosure. Metal would work really well and spread out the heat, so that could work well, but wood, plastic or molded carbon fiber? It's gonna run hot and therefore limit the maximum charging power. Forced convection (aka. a fan) was also very effective and even at low airflow I could lower the charging temperature of the BMS quite easily by 20 Celsius, but trying to put fans into a tight enclosure seems like an absolute hassle.

So I've been thinking of removing the boost converter from the module and rather do the charging by using a commercial 51-60 V power supply connected to a high efficiency synchronous buck converter with easily adjustable output voltage and current. These two things are meant to reside outside of the enclosure as independent blocks. This could enable much higher power charging, because we wouldn't be as much limited by the tight space requirements that enclosures might have and could more easily incorporate cooling.

![image|500x500](upload://5gms8dahXf8BmPycdycy4zyhKIx.jpg)
![image|500x500](upload://mElvFwfHDk85WORdXHDCXqhdFDT.jpg)
_Images from Digi-Key_

Thoughts?
```

---
## \#346 Posted by: SimosMCmuffin Posted at: 2018-08-11T14:12:09.338Z Reads: 107

```
*Boost converter.

It is able to easily sustain 5 Amps of charging current when using the bulk charging rather than boost charging. Check my other post's end for the ideas to increase the charging power and eliminating the thermal barrier that we are hitting at the moment.
```

---
## \#347 Posted by: Pedrodemio Posted at: 2018-08-11T15:22:55.838Z Reads: 105

```
I'm all for removing the boost converter, even more if the board gets smaller, I just don't know if it's worth to design an external converter, chargers with CC/CV are pretty cheap these days, and ordering one with adjustable end of charge voltage is all that is needed

That being said, if you really are talking high power, then it could be interesting if we start to use non cc/cv charging algorithms that allows to charge a higher than 1C without increasing degradation, the problem is that it will be cell dependent and people could ruin their batteries

All that as learning exercise of course, I think that to most people on most days a boards that charges in 3 hours in good enought
```

---
## \#348 Posted by: Pimousse Posted at: 2018-08-12T11:06:58.941Z Reads: 103

```
To be honest, what I like in your project is the boost converter. It's the added-value we don't find in other BMS setups.
```

---
## \#349 Posted by: keef Posted at: 2018-08-12T12:11:56.706Z Reads: 103

```
I've been using meanwells constant current led drivers for charging (https://www.meanwell.com/webapp/product/search.aspx?prod=HLG-240H).
They've got versions with different voltage ranges and maximum power output and are silent. You just need one where the constant current range covers the batteries voltage range and the voltage adjust can be set to the end of charge voltage. What i'm currently missing is a bms which turns of charging after the battery is full and only trickle charges.

For me this appears to better than an integrated charger since I want an efficient high quality rectifier anyways and these are better suited to shed heat. It would be interesting to have low power(5-50w) charging integrated if one doesn't want to carry around the power brick and charging time isn't an issue. How much of your bom cost and pcb space is related to charging? Maybe those parts could be left unpopulated if it's significantly cheaper.
```

---
## \#350 Posted by: SimosMCmuffin Posted at: 2018-08-12T13:44:43.164Z Reads: 102

```
[quote="keef, post:349, topic:46117"]
I’ve been using meanwells constant current led drivers for charging
[/quote]
I was also looking at meanwell's desktop power supplies and battery chargers on Digi-key for the external buck converter idea.

But a good compromise with something like a:
https://www.digikey.fi/product-detail/en/mean-well-usa-inc/GC120A24-R7B/1866-1746-ND/7703241
Would actually be pretty ideal to be used with the current integrated boost converter idea, because it is a battery charger it has CC/CV, so if you're under the chargers nominal voltage you could hook it to the bulk charging port and skip the boost converter block with the BMS able to stop the charging once cell voltages hit high enough. Of course you can't exactly hit the 100% charge as we can't ramp down the current if we are operating in the CC region, but at least charge it pretty high. Then if you need to go higher then the charger's output, you can instead feed it into the boost charger and increase the voltage from there to the maximum of 12S full voltage. And now we can ramp down the current towards the end.

[quote="keef, post:349, topic:46117"]
How much of your bom cost and pcb space is related to charging?
[/quote]
I checked the current pricing on DK and it was about 15-16€, for a single run total being 70€, so the boost converter is about ~20% of the component cost at the moment. I would also estimate the PCB space cost to be about 20-25%

[quote="keef, post:349, topic:46117"]
It would be interesting to have low power(5-50w) charging integrated if one doesn’t want to carry around the power brick and charging time isn’t an issue.
[/quote]
You would still need to carry some sort of charger with you, but of course it doesn't need to be so huge, if you want to charge at lower power.
```

---
## \#351 Posted by: Pedrodemio Posted at: 2018-08-22T00:16:27.176Z Reads: 98

```
@SimosMCmuffin with all the changes, what are the current form factor? With and without the power board (I don’t remember if still is two pieces or just one board)

And that is gonna be the final size for the beta? I’m allocating space for it in my next build

Also, if I remember correctly there is no CAN for now right? After seeing all information about the battery being display on the phone with Metr in @JTAG one I think it would be really useful 

Thanks
```

---
## \#352 Posted by: Pimousse Posted at: 2018-08-22T05:37:13.426Z Reads: 102

```
[quote="Pedrodemio, post:351, topic:46117"]
, if I remember correctly there is no CAN for now right? After seeing all information about the battery being display on the phone with Metr in @JTAG one I think it would be really useful
[/quote]

I second that. Communicating with the VESC sounds obvious but UART port is often busy. CANbus may also bring the possibility to shut down smoothly dual setup, brodcasting on Canbus.
```

---
## \#353 Posted by: SimosMCmuffin Posted at: 2018-08-22T15:19:14.548Z Reads: 106

```
[quote="Pedrodemio, post:351, topic:46117"]
Also, if I remember correctly there is no CAN for now right? After seeing all information about the battery being display on the phone with Metr in @JTAG one I think it would be really useful
[/quote]

[quote="Pimousse, post:352, topic:46117"]
I second that. Communicating with the VESC sounds obvious but UART port is often busy. CANbus may also bring the possibility to shut down smoothly dual setup, brodcasting on Canbus.
[/quote]

Board has a CAN IC on it. Hasn't been tested though. You can select with the solder bridges between CAN or USART which one is connected to the 4 pin JST-PH connector, or solder in some jumper wires to them.

![IMAG1016_1|611x500](upload://xj8wB4uTNRbyPB5seHRiMuvkfXw.jpg)
![image|690x389](upload://3l94b7H8OetUjmeWvjck6qetdRo.png)
![image|569x412](upload://9SMrkAoB1GkBhV1gkwAY1Jygd87.png)

[quote="Pedrodemio, post:351, topic:46117"]
With and without the power board (I don’t remember if still is two pieces or just one board)
[/quote]

Size spoken earlier in this post. Add couple millimeters more for height for the heatsink. Switch-module is not prototyped yet, but I believe the module will add about 25-40 mm on the 16-pin header edge outwards.
https://www.electric-skateboard.builders/t/flexibms-0-2-hw-under-work-flexible-configuration-and-charging-bms/46117/311?u=simosmcmuffin

I have taken inventory and I have the digi-key cart done for the 2 extra boards, but some critical components are on backorder atm with the worst being the boost converter's mosfet, which has a bit of an exotic package.
```

---
## \#354 Posted by: TarzanHBK Posted at: 2018-08-24T09:10:22.091Z Reads: 95

```
What i have found interesting in the last weeks is how much of drifting different BMS are capable to compensate.

I had a small one that wasn´t able to bring a 3,8V drifted cell back to the other 4,05V cells.
I tested another one with one cell at 3,6V and others at 4,1V and it worked.

Would be a nice test of your Flexi, if you´ll let it try to get something like a 3,0V cell back to all other cells at 4,1V or something similar!
```

---
## \#355 Posted by: Pimousse Posted at: 2018-08-24T09:35:22.035Z Reads: 99

```
It depends on balancing current vs charge current.
If the BMS has too low balancing current, it may happen that the CCCV charger stops charging before the balance has been performed.
```

---
## \#356 Posted by: JTAG Posted at: 2018-08-24T09:47:06.443Z Reads: 97

```
The balancing should continue, even if the battery is charged. Only very few packs (ones with really good cells or many in parallel ) are balanced before the main charge current is disabled.
```

---
## \#357 Posted by: Pimousse Posted at: 2018-08-24T09:51:25.253Z Reads: 96

```
Probably but those chinese BMS are some kind of black box.
Some don't even have balance feature.

Wait...

@TarzanHBK : Could it be this issue ? No balance feature on your small BMS ?
```

---
## \#358 Posted by: TarzanHBK Posted at: 2018-08-24T12:20:52.715Z Reads: 96

```
no, it catches balancing again when i manually brought up the cell to 3,9V.
I found a few that stopped charging when the distance to each other is too far.
When you bring them closer again, they catch up and do their work, but that´s the problem with a few boards.
People ride them daily, and charge them only up to about 3,9V most of the time, so that there is no balancing happening and cells drift further over time.
So would be a good feature if a bms is able to take care of that, even if they are so far from eachother.
```

---
## \#359 Posted by: SimosMCmuffin Posted at: 2018-08-25T11:36:35.993Z Reads: 101

```
I'm using couple different parameters to configure the charging setup.

> uint16_t maxChargePower = 70,  //Max charging power in Watts
maxChargeTemperature = 60, //Max PCB tempperature in Celsius
temperatureHysteresis = 3, //Hysteresis for the measured temperature to either keep current power or decrease it
chargingState = 0, //Logic state for the charging state machine
maxChargeCurrent = 5000, //Absolute maximum charging current in mA
maxCellDifference = 3, //max allowed difference between cell voltages, used to discharge higher cells towards the lowest cell
terminationCurrent = 300, //Low end CV state charging current cut-off in mA
terminationCellVoltage = 4180, //Max voltage for any cell to reach in mV
terminationPackVoltage = 42000, //Max voltage for the pack to reach in mV
cellBalanceVoltage = 4165, //Start balancing after cell goes over this voltage in mV, if needed
packCellCount = 10; //How many series cells in the pack, I'm planning on adding a auto-detect feature for the cells at some point.

These parameters are at this point just global variables, but the intent is to pack them into a better variable form and then manipulate them through Gets() and Sets() and make a simple GUI for PC (or basically any other comms (USART, CAN)) to configure them and read log data from the BMS.

Then the actual charging algorithm is divided into couple different states.

> // chargingState descriptions:
	// 0: Waiting to detect charger
	// 1: Bulk charging algorithm
	// 2: Boost charging algorithm
	//
	//
	// 8: Rest balancing, stop charging and allow pack/cell voltages to stabilize, first wait 5 min and then balance if necessary or start charging again (not implemented yet, but shouldn't be too hard)
	// 9: Charging ended, waiting for charger to be disconnected so we can revert back to chargingState 0
```

---
## \#360 Posted by: Pimousse Posted at: 2018-08-25T13:17:53.729Z Reads: 94

```
As @JTAG, you should give VESC Tool a try to build your UI.
Vedder did an amazing job making it easy to custom.
```

---
## \#361 Posted by: SimosMCmuffin Posted at: 2018-08-25T13:31:37.370Z Reads: 95

```
Oh GOD!

They're starting to multiply!

![IMAG1137|668x499](upload://z4evu80XtwShBUZ97TdP6Q4nlHA.jpg)
```

---
## \#362 Posted by: SimosMCmuffin Posted at: 2018-08-25T18:46:38.832Z Reads: 99

```
Bottom sides fully populated. I'll continue on the top side tomorrow, try to get it mostly finished tomorrow.

![IMAG1138|690x372](upload://pEtf9MK0D1FOi38Cab8Jc1TW6ps.jpg)
```

---
## \#363 Posted by: SimosMCmuffin Posted at: 2018-08-26T11:00:20.623Z Reads: 102

```
Top sides populated apart from the biggest components. PMing the beta volunteer test group to talk about connector choices.

![IMAG1139|690x363](upload://3Cmd3vpdVLFDU0pduYHENbgWLw9.jpg)
```

---
## \#364 Posted by: SimosMCmuffin Posted at: 2018-08-27T06:12:44.300Z Reads: 101

```
The 2 new boards are going out to @Pimousse and @TarzanHBK  

If you're interested in volunteering for the testing and developing the BMS, you can add your information to the following google sheet from which I'll be choosing the next beta testers to get their modules. 

https://docs.google.com/spreadsheets/d/1CItw3euHCguWo1JE4JJYVbNvmc4FKBdvPif63ELJipM/edit?usp=sharing

No ETA for the next test batch has been planned at this time and will be dependent how we get the ball rolling from the start. We might also move onto 0.3 HW between now and then. I have a list of fixes and changes gathered from the 0.2 HW that I'll change for the next iteration.
```

---
## \#365 Posted by: Pedrodemio Posted at: 2018-08-27T17:16:36.912Z Reads: 99

```
Nice

I was going to fill but since I have no ETA to have my next board running it’s better to leave for those who can test right away 

On my current one unfortunately I can’t fit
```

---
## \#366 Posted by: SimosMCmuffin Posted at: 2018-08-27T17:34:30.627Z Reads: 105

```
Boards are assembled and I have hello world'd them, flashed the current firmware onto them and tested that the USB virtual COM port works. I will also test the charging just to make sure they are good to go, but that'll be a later objective.

![IMAG1150|436x500](upload://usIn014ADGtzYhYepfA0glqDdMH.jpg)
```

---
## \#367 Posted by: SimosMCmuffin Posted at: 2018-09-09T19:42:07.699Z Reads: 104

```
Update.

I have now tested both modules by using them to charge my battery pack during this week and they seem to be in working order. Plan is to get them shipped them to their respective testers next week.

![IMAG1164|690x428](upload://qj1RQvqpVzKFTS02BSBL3dFnm6W.jpg)
![IMAG1165|690x456](upload://lSVTV1EvOoBbGdlSw7nl8c9w2XC.jpg)


Beta tester user manual is also under work in google docs.

![image|690x311](upload://rHmTES6OP0P8ralfR6KaEB80xwn.png)

![image|635x500](upload://hxJm49tBwx9HQQffdm5uUAGgcDE.png)
```

---
## \#368 Posted by: Pimousse Posted at: 2018-09-09T21:03:15.032Z Reads: 106

```
Thank you for pushing test at a high lecel of R&D !
Can't wait to know how it performs !
```

---
## \#369 Posted by: Pedrodemio Posted at: 2018-11-26T01:43:14.629Z Reads: 91

```
Any more news?
```

---
## \#370 Posted by: SimosMCmuffin Posted at: 2018-11-26T21:06:52.545Z Reads: 89

```
Sorry for this particularly long silence since the last update.

**I would at this point declare the project to be on a hiatus**, because the boarding season has ended in Finland.
 
I am also personally taking a breather from the project at this point, as I was starting to burn out on it. I have been busy with customer projects at work and I didn't really feel like continuing doing the same thing at home that I had been doing for 8 hours at work. Had my own design electronics for the customer project in an official EMC-testing, which was an interesting experience and I tried to absorb as much info/experience as I could from it. 

I plan on picking this project back up next year when the weather start to move towards the start of the new season and I have planned upgrades for my esk8 as well for better usability regarding to charging and all-weather use.

I welcome @Pimousse & @TarzanHBK to share any negative or positive feedback/experience with their units, or even the possibility that they haven't used them since receiving them, which I also consider a possibility.
```

---
## \#371 Posted by: Winfly Posted at: 2018-11-26T21:18:34.636Z Reads: 87

```
Rip I really liked this project.
```

---
## \#372 Posted by: Winfly Posted at: 2018-11-26T22:40:37.611Z Reads: 88

```
I'll take some test units and see if I can figure something out
```

---
## \#373 Posted by: Pimousse Posted at: 2018-11-26T22:57:06.139Z Reads: 90

```
I would like to publicly apologize to not having tested the beta unit yet. You did an amazing work, pushed the tests hardly and had produced a couple of units with a ton of work. 
And finally the unit's still laying down in his box. :frowning: 

I hope being able to come back on this project soon.
The bad weather is the greatest reason to spend time coding and performing tests to prepare the Spring and the next season. :slight_smile:

You can't be more smart to take a break before burning a fuse in your head.
Believe me, blowing those fuses takes a lot of time to recover. :wink: 

@Winfly Why RIP ? This project isn't dead !
```

---
## \#374 Posted by: JTAG Posted at: 2018-11-27T00:33:21.201Z Reads: 87

```
Nooooooessssss why :sweat:. You were even writing a manual!

No pressure, it took me about 1.5 years to have a usable BMS... these things just take time.
```

---
## \#375 Posted by: SimosMCmuffin Posted at: 2018-11-27T07:12:58.657Z Reads: 92

```
@Winfly I don't personally see this project as dead, but I want to take a breather from it for the winter.

@Pimousse It's fine. If you have time, try connecting some 3S+ Lipo (if you have some lying around) with a XT60 discharge-plug and a balance connector to it (>**discharge plug first**<) and then via USB to a PC and seeing that you get serial terminal printout. Mainly to just check that the module is still okay.

@JTAG Had a mental 3 month tight deadline customer project at work, in which I was the only electronics designer. We were so tight with time that we couldn't order the final PCBs assembled, but I rather assembled the board's at home by hand with my own tools during couple long nights. And then we even needed to get them partially EMC-compliant to ship them around the world and not get them stuck in customs. Oh yea, and there were some hurdles with the compliance and had to prolong the pre-testing and the official tests as well. But we got them shipped in time and the customer was able to open their new location without any major hitches. Needless to say, I was a bit done with PCB stuff for a while... 

_Here are some pictures of some stuff._

![IMAG0045|690x389](upload://gos5RhhiDqsEVDs6nXtmFKEDMhe.jpeg) 
![IMAG0046|690x389](upload://o7nnSlR1AIFbh0qquMDT2TjYg7w.jpeg)
This is the EMC-testing chamber. The two antennas are for low and high frequency ranges, with the left one used for 30 MHz - 1000 MHz (we used mainly this one) and it is also able to turn 90 degrees on it's axis automagically to test both horizontal and vertical polarization. It also moves up and down from 1 meter height to 4 meters in 1 meter steps. Higher frequency one is for 1 GHz - 6 GHz.

https://youtu.be/TdpVyXpHNUg
Here's a short clip of our actual DUT without any critical identification marks showing (customer NDA) on the spin plate in the testing chamber. So the whole measurement process is automated. For our tests, the lower frequency starts and sweeps the frequency range from 30 MHz to 1 GHz at 1 meter height, measures horizontal and then vertical polarized emissions and then repeats this at heights of 2, 3 and 4 meters. After this the spin plate turns 45 degrees and the whole antenna orientation and moving routine is done again. This is repeated until a 360 total rotation is done. This whole process takes about 2-3 hours for the lower frequencies. Then if high emissions are detected at some orientations, polarizations and heights then more specific and accurate measurements can be queued from the control room and these might take even longer depending on the needed measurements. I think the cost for 2 work days measurements was about 5000 € and it wasn't even full compliance testing.


Here are some smaller size "plug-n-play" powerwall modules for 18650 cells that I prototyped, because I want to use my older 18650s for some energy storage. The idea for them came from [**jehugarcia**](https://www.youtube.com/watch?v=9YwErplHps8&t=384s) on YT, but I made some of my own changes to the design concept. So the idea behind the pack is that it's solderless assembly. You can just plug your 18650s into the holder and be done and then connect the modules together with crimpable connectors. One module has 4 cells in parallel and you can connect another module to that in parallel with a vertical connecting piece for easy expandability. You then use some heavier cabling with crimpable connectors to connect the parallel modules in series and leave the vertical connection piece out. The configuration shown below is 5S8P.

![IMAG0006|422x500](upload://vo1LK6rdW2r47kncRP811Yuyz6n.jpeg) 
![IMAG0004|303x499](upload://oLecVFkyAHAiNt23ZYMuuw5PeQM.jpeg) 
![IMAG0005|555x500](upload://2Qb8HNoMVcrrLAn7eujdvbCkEqD.jpeg)

I changed the crimp connector for side-entry ones, so the series connecting wires wouldn't protrude as far from the module stack, as compared to the pictures above. I have now bigger modules in assembly with 12 cells fitting into one, but I don't have pictures of those yet.
![IMAG0022|282x500](upload://nh2AExUzOuM2cMAyszg2ddgulAr.jpeg) 
![IMAG0021|282x500](upload://2Vcp3k53xEYqts4aYhhyc6beWxa.jpeg)


I have also converted an old fitness cycle to a generator and I have been charging that 18650 pack shown above with it and then charging all my rechargables from that (phone, flashlight, bluetooth headphones) using a car's USB charger (12-24V input). Plus I haven't been doing any good exercise after the weather started to prevent boarding.

![IMAG0056|690x389](upload://dlEB8x2A4kxASHU4xZ6ozgg0Io1.jpeg) 
![IMAG0055|690x389](upload://yHeIROAY99z6YQv5K6dKP6UMtZf.jpeg)
```

---
## \#376 Posted by: Winfly Posted at: 2018-11-27T07:16:29.942Z Reads: 87

```
Sorry i didn't mean it that way. I just wanted this completed really badly. I was following pretty closely until update were slow. figured you might be busy with something else important. anyways please take your time, we appreciate your effort into this project.
```

---
## \#377 Posted by: SimosMCmuffin Posted at: 2018-11-27T07:18:55.031Z Reads: 90

```
Thanks, appreciated :+1:
```

---
## \#378 Posted by: TarzanHBK Posted at: 2018-12-03T10:56:27.385Z Reads: 87

```
Same here unfortunately. I'm drowning in building batteries for People but haven't had the time to look closer at the bms. But im currently having a 10s4p pack with different loads due to a bad bms, so this might be a candidat to test your BMS a bit more. Goal is to get a testboard up for this this winter and run hell out of it as soon as the weather is suitable again.
```

---
## \#379 Posted by: okashira Posted at: 2019-04-10T20:44:01.896Z Reads: 58

```
@SimosMCmuffin 

Hows the current status?
I'd like to jump on.
If you have some extra boards, I'll buy some.
Any starting point on the code?
Did you get the STM32L4 going?
```

---
## \#380 Posted by: SimosMCmuffin Posted at: 2019-04-14T17:27:57.320Z Reads: 56

```
The development of this FlexiBMS fork has ended.

I started a new attempt and a approach a bit over month ago and have been documenting and having discussions on this thread over here:
https://www.electric-skateboard.builders/t/flexibms-lite-new-approach-to-get-past-vaporware-stage/85493
```

---
## \#381 Posted by: Jonisonvespa Posted at: 2019-08-07T15:19:09.137Z Reads: 36

```
hi 
wondered if this bms is now fully working no bugs, be interested if anybody has any boards for sale if it is
thanks
```

---
