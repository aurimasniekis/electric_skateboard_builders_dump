# Charging 12s&hellip; from USB

### Replies: 42 Views: 1805

## \#1 Posted by: SuperSaiyanCaleb Posted at: 2018-05-24T07:57:31.694Z Reads: 264

```
Before you say it, yes, I know it would take a loooong time.  But I'm planning to DIY a board with a 12s lipo battery, and I'm interested in having the option to slow charge it from a 5V power source like USB.  (Of course I'm also planning on having faster options like a balance charger or BMS.)  But in the event that I'm staying the night some place and only happen to have a USB charger, I'd love the option to be able to at least partially charge the board that way.

My two first thoughts were to either charge one cell at a time using a 1s charger that takes 5V, or to boost the 5V to the ~50V that a 12s charger would require.  But in the former case, I'm not sure of a simple way to cycle the charging between cells without manual intervention, and in the latter case, I'm not sure if there are any chargers that won't attempt to draw too much current so as to overwhelm the boost circuitry and/or the underlying 5V power supply.  Any ideas on a simple-ish way that I could accomplish this?
```

---
## \#2 Posted by: Luuke Posted at: 2018-05-24T08:14:46.211Z Reads: 248

```
Just use a DC DC step up module to 50V.
Lets say you use a 5V 1A charger, that would lead to less (cause of the losses) then 50V 0.1A. This could be done easily but is very slow!
```

---
## \#3 Posted by: b264 Posted at: 2018-05-24T08:17:12.678Z Reads: 245

```
I'd also be interested in this for 10S
```

---
## \#4 Posted by: Acido Posted at: 2018-05-24T09:59:14.943Z Reads: 231

```
Boosting 5 to 50 would be super inneficient and super slow
```

---
## \#5 Posted by: Slak Posted at: 2018-05-24T10:44:28.330Z Reads: 222

```
But, is there any problem charging at 0.1A ? Slow ok, but is it bad for the battery (longer charge --> more time to heat a lot) to charge during several hours at 0.1A (I mean more than 5h for example ) ?
```

---
## \#6 Posted by: petter Posted at: 2018-05-24T11:11:11.412Z Reads: 214

```
No, slower charge times are actually better for the battery. 

Though.. The usb standard puts the maximum current(after requesting "high" current) at 500mA. This is for a proper USB port atleast, like a computer, laptop, router or similar. If you use a charger with higher specs, some go up to 2~2,5 amps, or for usb 3 there are different rules where you can even get higher voltage. 

All of these things demand more out of your "charger" or usb-converter. If you want to make a version that will always work with any usbport, your charge current would likely be less than 50mA, maybe 40 or 30 mA. From there, you will have a charge time of several hundred hours. 

So im a bit dissapoint to have to inform you that it's not very feasible or useful.. maybe if you have a 2A USB charger you could get 200-300 Wh charge over two days or 30 hours, but for that to be reliable you'd probably have to bring the charger with you.. And then you might just as well bring a proper charger for the board?


However, something that might be along the lines of 'charge with what you got' could be this: http://www.faradaymotion.com/faraday-motion-web-shop/31-battman-intelligent-bms-4-12s-builtin-chargerswitch.html
https://raphaelchang.com/#projects/bms

Not for the faint of heart, but possibly it would work with pretty much any old laptop power brick or similar adapters.
```

---
## \#7 Posted by: Slak Posted at: 2018-05-24T11:18:33.637Z Reads: 192

```
Did you finish the Battman BMS firmware ? Because last time I heard about it, buyers had to deal with it by themselves as RaphaelChang didn't answer anymore (at the time at a least, few months ago). Hardware was working but firmware was basic or unfinished.
```

---
## \#8 Posted by: petter Posted at: 2018-05-24T11:25:13.087Z Reads: 185

```
Nope, i haven't heard any news of it.. it's very interesting though. i figured since you can buy it there, it should at least work? But it might also be a real PITA!

though if it wasn't so expensive i'd probably buy one and get it up to speed myself, it's a real interesting project.

I mentioned USB3 above, and thats sort of in the same boat.
http://www.usb.org/developers/powerdelivery/
Lots of potential, but have you heard anything of this? i don't think i have heard of any devices using or providing the 20V they talk about. if they did, 100W would be good enough to use as your only charger!
```

---
## \#9 Posted by: Pedrodemio Posted at: 2018-05-24T11:28:56.574Z Reads: 172

```
The @JayKay e-trucks charge via PD
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2018-05-24T12:09:46.658Z Reads: 167

```
high currents heat up the battery, whether it's while charging or discharging. Low currents are no problem.

But speaking of actually range gained from charging with for example the 5V 1A and assuming a 100% efficiency, it's just 5Wh every hour. Even efficient boards use around 10Wh / km of energy, so you're getting 0.5km/0.3mi of range for a hour of charging and even if left to charge overnight it is still almost nothing.

the 5V to 50V DC-DC converter is also pretty exotic and would likely need a 2 step-up converters, which also reduce the conversion efficiency even more.

Note. got interrupted by colleagues while writing this reply, so sorry if there is some repeated info.
```

---
## \#11 Posted by: Pimousse Posted at: 2018-05-24T12:58:24.134Z Reads: 142

```
(Off topic, sorry)
Forget Battman project. It's dead.
I bought 2 boards from him, without any usable features coded (beside only the antispark switch).
I spent few dozen (maybe hundred) of hours coding all the BMS features to avoid using those expensive boards only as door stoppers.
Then @SimosMCmuffin came and told us that the Hardware is undersized for what it pretends to achieve and can even be dangerous (over-heating).

At least, I learned a lot of C coding. :roll_eyes:
```

---
## \#12 Posted by: DeathCookies Posted at: 2018-05-24T13:04:44.557Z Reads: 128

```
Its a pitty to hear....
```

---
## \#13 Posted by: Sebike Posted at: 2018-05-24T13:24:53.938Z Reads: 126

```
So one could actually plug the board in, leave for a vacation, come home after a week or so to a half full, half empty battery. Sounds amazing! :rofl::wink:
```

---
## \#14 Posted by: Giga Posted at: 2018-05-24T13:55:10.986Z Reads: 127

```
[quote="petter, post:8, topic:56576"]
I mentioned USB3 above, and thats sort of in the same boat.

http://www.usb.org/developers/powerdelivery/

Lots of potential, but have you heard anything of this? i don’t think i have heard of any devices using or providing the 20V they talk about. if they did, 100W would be good enough to use as your only charger!
[/quote]

I have a 60W (Laptop or Phone) USB-C charger. It changes voltage between 5V, 9V, 15V and 20V automatically. But then you need another stepup or bms I guess....

other thing with easy solution: 

https://www.ebay.com/itm/MICRO-USB-5V-1A-Lithium-Battery-Charging-Module-Lipo-Charge-Board-Protection/182712292766?epid=2081582587&hash=item2a8a80559e:g:RQMAAOSw8IJZjRug
for each cell (maybe even at balancer lead as second charging solution) and then a multi usb hub/charger like this
https://www.ebay.com/itm/Fast-Charging-Desktop-Station-8Port-USB-HUB-Travel-Home-Wall-Charger-Smart/163031438037?hash=item25f56e52d5:m:md5ae-V4ONNCqittjmbmkHg

so you have at least 1AH per cell.
```

---
## \#15 Posted by: petter Posted at: 2018-05-24T13:56:02.960Z Reads: 110

```
Haha, yeah i'm not surprised! I had a laugh when i read about the balancing resistors, how he sounded surprised when they got hot.. though i have not looked further into the power switch and the charging, i don't really see why it would not work. At least for the balancing that would be an easy fix with lower currents.

How far did you get? it would be very interesting to have a BMS with eswitch, that does not cut brakes on high voltage and that has communication possibilities with a vesc.. Programmable number of cells and voltage levels would be very nice as well. From an oem standpoint, you both want to protect the battery at all times but also never cut the power leaving the rider in a possible headstand. Not sure how for example the raptor 2 does this but only using the vesc with an LVC "gives" the user a possibility to kill an unbalanced battery. this is also made worse if a dumb BMS is used, if it does not balance for example if the user never charges the board fully.

edit: @Giga, yeah its one of those i was thinking of. that sounds like its using usb PD mode 4, 60W. Or up to mode 4 maybe, i am by no means the person to ask about this. i know a fair bit about usb 2 but usb3.. Either way, the hardest part about possibly using an usb3 power source is that it will not give you much juice without the cennecting device negotiating for it. This also happens in usb2, but the low power levels makes it much simpler and there is a sort of standard of requesting more power with certain voltages on the data pins. The normally allowed current on those usb ports is only 100mA, but since it's not defined what they should do if a unit uses more than that, usually nothing is done about it even if a unit has not done any request for more power.

But since in usb3 the voltages also changes, possibly damaging units that cannot handle it, i expect that the negotiation is more strict and that you cannot get access to that power without a full usb3 control circuit handling the communication. I can very much see such a unit becoming available on ebay for example, just a pcb with a possible jumper for voltage and power out pads, but i have not seen any nor expect to really see any until usb3 becomes way more popular... which also fits with that even if you could whip up this usb3 charge port on the board, odds are that there won't be a usb3 charger where you are staying. maybe next year there will though!
```

---
## \#16 Posted by: Pimousse Posted at: 2018-05-24T14:03:52.500Z Reads: 100

```
I wrote BMS features (charging, faults and warnings management), LTC auto-diagnostic, modified the PC interface to display faults and parameters that I added.

I also started to implement VESC comm. through CAN to, as you said, tell the VESC to stop driving motor smoothly, and if overcurrent is still there (e.g. short on wires), then switch power off.
But I let this project at this point and gave up.

That's a pity because I saw so many great stuffs to do with this Battman/VESC duo ! :(
```

---
## \#17 Posted by: petter Posted at: 2018-05-24T14:16:02.515Z Reads: 99

```
Wow, sounds like you made it really far! 

Also yeah, C-coding is a pretty useful skill.. some even get paid for it ;)

Did you get a chance to try using battman for real? did you run into any of these heat issues yourself? 
(My guess is, balancing got very hot, charge circuit possibly when using high current, switch quite OK?)
```

---
## \#18 Posted by: Giga Posted at: 2018-05-24T14:25:17.566Z Reads: 107

```
[quote="petter, post:15, topic:56576"]
Either way, the hardest part about possibly using an usb3 power source is that it will not give you much juice without the cennecting device negotiating for it.
[/quote]

Well, I guess it is not really that hard...:
https://www.crowdsupply.com/goarks/usb-c-thru
or this

https://blog.adafruit.com/2017/01/05/fusb302-breakout-board-usb-power-delivery-phy/

or this

https://www.tindie.com/products/ReclaimerLabs/usb-type-c-power-delivery-phy-breakout-board/

they all claim to get up to 20V, 5A...
I guess it cant be that hard to get them from default 5V 2A to 20V 5A...since they are really made for that...

EDIT: there is even a git example how to do it with the last one:
https://github.com/ReclaimerLabs/USB_PD

https://www.tindie.com/products/ReclaimerLabs/usb-c-explorer/
```

---
## \#19 Posted by: petter Posted at: 2018-05-24T14:28:01.712Z Reads: 99

```
Haha, damn. I stand corrected! Thanks!

Edit, that last one seems like the easiest to use, though pretty pricey.. it does seem like the other options will require some more work/extra bits around them, with an arduino or similar. might not be a bad thing in the end since you probably need something to see to that the charger waits for the full 20V to be available before starting up, but it does add complexity

Edit again, i'd suggest this one! [PD buddy](https://www.tindie.com/products/clayghobbs/pd-buddy-sink/)
```

---
## \#20 Posted by: Pimousse Posted at: 2018-05-24T14:32:03.382Z Reads: 100

```
I built a 12S1P pack using old an brand-mixed cells (in order to have a high drift behaviour and thus highlight the balance skill of this BMS). But I read @SimosMCmuffin just before connecting it to the Battman.
AFAIK, the heat isue was on the Step-up/down converter (the coil itself).

[quote="petter, post:17, topic:56576"]
Also yeah, C-coding is a pretty useful skill…
[/quote]

Yeah, C coding wasn't a waste as I'm now able to write my own VESC firmware for adding more features. :)
```

---
## \#21 Posted by: petter Posted at: 2018-05-24T14:34:02.369Z Reads: 97

```
Great! Then i know who to ask for vesc features ;)

I'd do it myself but you know.. time and stuff.

yeah the converter is not a terrible idea but in order to deal with similar power levels, it would really need bigger components. Not quite sure why raphael seems to want to make everything so small? But for looking into usb3 a converter will probably be needed, and some smarts.. There are ofc other ways to get the same function but it's always nice to have a brain box in there somewhere.

Also, in this size, balancing cells is for sure something that battman could do but in order to deal with the heat, it could take a looong time for an extreme case. Though i don't see this as a problem, since it can keep doing the balancing and protect the cells at the same time, so even if you plug in a pack that has one cell at 0% and one at 70%, charge for an hour and go riding? it's only managed to balance a bit say it's at 100% and 35%, the charge will stop at 100% and the ride at 0% for each cell respectively. After, the balancing continues so the next time it will have sorted it.
```

---
## \#22 Posted by: SuperSaiyanCaleb Posted at: 2018-05-25T01:02:46.049Z Reads: 83

```
I considered using one or more of those TP4056 modules.  The issue with using more than one is that they have a common ground on the input and output sides, which means each module would require an isolated power source unless the individual cells of the battery can be separated while charging.  (And if I use 3s or 4s lipo packs to construct my 12s battery, there's basically no way I can isolate all the cells from each other.)

This was what led to my idea that I could use one module and cycle between individual cells.  But I'm not sure if there are any easy ways to make that happen automatically...
```

---
## \#23 Posted by: SuperSaiyanCaleb Posted at: 2018-05-25T01:06:07.456Z Reads: 77

```
> Just use a DC DC step up module to 50V.
> Lets say you use a 5V 1A charger, that would lead to less (cause of the losses) then 50V 0.1A. This could be done easily but is very slow!

Are there any 12s BMS or balance chargers that can be set to only draw 0.1A?
```

---
## \#24 Posted by: SuperSaiyanCaleb Posted at: 2018-05-25T01:15:42.921Z Reads: 78

```
[quote="SimosMCmuffin, post:10, topic:56576"]
But speaking of actually range gained from charging with for example the 5V 1A and assuming a 100% efficiency, it’s just 5Wh every hour. Even efficient boards use around 10Wh / km of energy, so you’re getting 0.5km/0.3mi of range for a hour of charging and even if left to charge overnight it is still almost nothing.
[/quote]

[quote="SuperSaiyanCaleb, post:1, topic:56576"]
Before you say it, yes, I know it would take a loooong time.
[/quote]

Also to be fair, many USB power supplies are able to supply 2A or more of current.  Computers aren't the only power sources with USB ports.  But even charging at just 5 watts overnight, that would still add about 2 miles of range.  Considering I live within a couple miles of several friends' houses that I stay the night at, this still seems like a useful function to have for me.
```

---
## \#25 Posted by: lrdesigns Posted at: 2018-05-25T03:13:58.050Z Reads: 74

```
Use 12 of these if you want to charge from a 5v sorce. 
Could charge at decent speed if you can find a 5v 12amp power supply!
![image|459x385](upload://eegX4UmvHJoqSmpoNcxATsYAjkg.jpg)
```

---
## \#26 Posted by: b264 Posted at: 2018-05-25T03:16:49.928Z Reads: 70

```
For everyone that says "it will be slow"

OP noted that in the first post ... and those of us that want this are okay with that .. or may even prefer it...for reasons outside the scope of this thread.

Who cares how slow it is.  We're talking about how to make it happen ...
```

---
## \#27 Posted by: b264 Posted at: 2018-05-25T03:18:26.033Z Reads: 72

```
[quote="lrdesigns, post:25, topic:56576"]
Use 12 of these if you want to charge from a 5v sorce.
[/quote]

I don't think you can use 10 or 12 TP4056 modules because the cells are 10SxP and 12SxP -- not 1S10P or 1S12P

The cell negatives all have to be connected together to use those.
```

---
## \#28 Posted by: SimosMCmuffin Posted at: 2018-05-25T06:57:26.160Z Reads: 71

```
[quote="SuperSaiyanCaleb, post:24, topic:56576"]
But even charging at just 5 watts overnight, that would still add about 2 miles of range.  Considering I live within a couple miles of several friends’ houses that I stay the night at, this still seems like a useful function to have for me.
[/quote]

Fair enough. My personal needs might have skewed the usefulness of this charge speed, as my work trip in one direction is a bit over 7 miles, so it just wouldn't have made sense to me, but now that you mentioned your scenario with a bit more detail. I can start to see why you could get actual use out of it.
```

---
## \#29 Posted by: b264 Posted at: 2018-05-25T07:22:06.149Z Reads: 69

```
The other factor nobody considers is multiple boards.  What if I have 5 boards ready to go and I want to slow-charge the one I just got back on over multiple days?  The OP noted in first post that "slowness" is not what the thread is about, but more so how can this be accomplished.  There are so many off-topic reasons.  Solar charging.  Compatibility with everything else that uses USB.  Availability of charging locations.

But "how" is the major thing.
```

---
## \#30 Posted by: Slak Posted at: 2018-05-25T08:44:03.170Z Reads: 69

```
[quote="SuperSaiyanCaleb, post:24, topic:56576, full:true"]
But even charging at just 5 watts overnight, that would still add about 2 miles of range.  Considering I live within a couple miles of several friends' houses that I stay the night at, this still seems like a useful function to have for me.
[/quote]

Are you implying you will let your board charge during the night while you are asleep ? If the answer is Yes, you may be put yourself and your friend's house at risk, fire risk.
```

---
## \#31 Posted by: petter Posted at: 2018-05-25T09:02:06.019Z Reads: 69

```
Well, there is slow, like the op noted, and then there is slow. Like i stated above, in order to comply with usb 2 specs, it might take more than a week to charge a 400wh board. 

(And while it might be nice to get enough juice to get home again, somewhere i'd guess if it's close you might have the capacity to make a round trip anyways and if it's long you could bring your normal charger.. But thats beside the question :wink:  )

if you just want to charge your board, one of these [boost converters](https://www.ebay.com/itm/DC-DC-4-5-32V-to-5-52V-XL6009-Boost-Step-up-Module-Power-Supply-LED-Voltmeter-/262401090345) will probably get you close. Though i'm not quite sure how they would perform with such a big voltage boost, or what they would do with such a limited current input to such a "high" output current. But assuming you find a module that does manage to produce the voltage you need then my guess is that it will just work. Otherwise it's pretty simple to create a constant current circuit. 

This is also assuming that you first do some testing to verify that you wont burn up the usb you connect to and that you have a BMS.. though the bms is more a style point here, since the actual chance of the battery getting full are slim. But it should nonetheless be there.

But still, if you want to be able to charge anywhere, id probably go for supporting most 12-24V wall warts instead, it's almost the same circuit and odds are that it will get you ALOT more charge.
```

---
## \#32 Posted by: Luuke Posted at: 2018-05-25T09:26:13.754Z Reads: 70

```
This WRONG! you can not use one single 5V power supply!
That would shorten your Battery!

You would need 12 individual 5V 1A power supplys.
See my post for a 10S version:
https://www.electric-skateboard.builders/t/first-build-mono-6374-vesc-10s3p-bms-90mm-flywheel/37257/14?u=luuke
```

---
## \#33 Posted by: riva_00 Posted at: 2018-05-25T10:51:23.892Z Reads: 66

```
@SimosMCmuffin
What if you had this: -

https://www.ebay.co.uk/itm/ORICO-6-Amp-4-Port-Multi-USB-Wall-Charger-UK-Plug-Power-Adapter-for-iPhone-iPad/291258871850?epid=2271459604&hash=item43d061b02a:g:wR8AAOSwKkhZrc-9

or this: -

https://www.ebay.co.uk/itm/36W-7-2A-4-Port-Fast-Multi-USB-Wall-Charger-Power-Adapter-UK-Plug-Android-iPhone/382178132956?var=651029667537&hash=item58fb9783dc:m:mZ_-zAt7QmZ8M5dwrgqcU-w

I'm certainly no electrical engineer, but could you use one of those, plug it into the wall and connect say 3 usb cables from it to something that combines the power output from those 3 cables? So assuming you then get 30W, based on your previous statement of 5Wh achieving (approx) 0.5KM/0.3m every hour, this could do something like 3.0km/1.8m every hour.
Above is assuming 100% efficiency though, however even if i halved those numbers it's still viable for charging at work as part of a commute.
I also think i could probably find a larger watt USB charger, however the ones above are cheap and compact.
```

---
## \#34 Posted by: SimosMCmuffin Posted at: 2018-05-25T11:45:06.870Z Reads: 63

```
[quote="riva_00, post:33, topic:56576"]
2.4A per Port
[/quote]

The  beefier A-type -connectors can usually deliver rated maximum of 2.5 Amps, so you would still be at 12.5W and not sure if the ports could be paralleled up, but then you would have to make a custom USB cable anyway that could handle the current.

The biggest limiting factor with using normal USB to charge is the low voltage that needs to get boosted very high, but USB type C connector with PD would start to make sense, but needs communication ICs  to be able to charge at higher voltages. And of course an USB PD capable charger, which then I would already ask why not carry a dedicated charger for the board? Put a 5V buck regulator on the board and charge your USB devices from that :smiley:
```

---
## \#35 Posted by: riva_00 Posted at: 2018-05-25T12:53:38.113Z Reads: 65

```
I have a scenario in my head that you need to help make happen...

I get into work on my board, everyone looking dreamily at me wishing they skated in.
Then i ask to "borrow" USB chargers off people, claiming i forgot mine.
I combine them all in my PC and maybe the one next to mine (he'll never know).
I can then charge the board back up enough to razz around the park at lunch, harassing dogs and such.

Yeah sure i can do that with a charger, but the stupid ponces need a sticker on the brick that says it's passed a safety test, and the guy that does that isn't in till August or something.

Make this thing Muff master Simos, you know you want to.
```

---
## \#36 Posted by: petter Posted at: 2018-05-25T14:37:37.027Z Reads: 62

```
Yeah, that's kind of my thoughts aswell.. If anyone wants to try charging from one usb, then by all means get a boost converter like the one i linked above. Same problem with the high current usb chargers like @riva_00 linked. Sure it can be done, but then you'd need to bring that charger instead. If you want portable, something like [this](https://www.alibaba.com/product-detail/50-4V-54-6V-58-8V_60725956350.html?spm=a2700.details.maylikever.4.232078fbiTLfLs) is also pretty small. And slowish. ;) you could go for one with even lower current too if you can find one?

For the single cell chargers like the one @lrdesigns showed, the question is not only if you have different chargers, you also need chargers that have an isolated ground, otherwise it will cause a short anyways. BUT, if you wanted to go down that slightly silly route or ten chargers, you could also just series them to get one 50V, 1A source and (maybe) add some current limit in order not to overload them. But for cheap(also for not-so-cheap) usb chargers it's very common that they drop in voltage under load, meaning that the current would regulate itself. That would be one UGLY usb cable though! And you'd be pretty guaranteed to fry something sooner or later when you plug it into the wrong port.

Btw @riva_00, would they not be more upset if you plug in a wire mess diy abortion of a usb charger than if you just smuggle you normal charger in?
```

---
## \#37 Posted by: SimosMCmuffin Posted at: 2018-05-28T06:12:48.156Z Reads: 52

```
This could be a fitting boost converter controller
http://www.ti.com/lit/ds/symlink/tps43060.pdf

4.5 - 38 V input voltage, 58 V output max, depending on switching frequency very closely capable of 90% duty cycle.

Not starting on designing this yet though, I have some other higher priority projects in the pipeline.

Also, I might be designing an evaluation version of this for myself, but it could be tested for the topic's use case.
```

---
## \#38 Posted by: jadatmag Posted at: 2018-05-28T09:17:40.895Z Reads: 48

```
With USB Power Delivery over USB type C, surely any skateboard van be charged overnight.

The Macbook Pro charger deliveres 87 watt over USB type C.
```

---
## \#39 Posted by: SimosMCmuffin Posted at: 2018-05-28T11:52:56.087Z Reads: 48

```
Sure, except that USB C with PD brings with it completely new can of worms to contend with and we still need to most likely boost the voltage higher for +6S packs. PD is a pain to implement, because it needs PD specific implementation and communication between charger and load.
```

---
## \#40 Posted by: petter Posted at: 2018-05-28T13:29:22.384Z Reads: 43

```
Well, if we're talking a custom board then might as well support PD.. the code and ics used in the tindie boards looked simple enough, outside of that that is needed is to be able to set charge(if thats desired to be a feature) current and a enable signal to the boost circuit. Maybe it would even be possible to have a usb3 PD charger with support for snail charge on usb2?? THAT would be COOL. 

i looked at the tps43060, looks nice except for the package.. any reason you chose that over others? Switching regulator design is certainly not my expertise but it's pretty damn interesting
```

---
## \#41 Posted by: SimosMCmuffin Posted at: 2018-05-28T16:12:57.038Z Reads: 40

```
[quote="petter, post:40, topic:56576"]
i looked at the tps43060, looks nice except for the package… any reason you chose that over others?
[/quote]

I didn't choose it because of the package (although it's nice it has a small footprint). I chose it because it had the features I was looking for in a boost converter. Synchronous, current mode, Wide Vin voltage with emphasis on the low voltage, over 12S capable output voltage support, cheap. The package could have been almost anything, as long as it would be something compact.
```

---
## \#42 Posted by: petter Posted at: 2018-05-28T19:45:51.704Z Reads: 34

```
Nice.. Not a chance that i'd manage to solder that but it will be interesting to see the result! Like you say, it's nice n small
```

---
