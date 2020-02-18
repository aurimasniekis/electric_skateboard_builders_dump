# New Open Source Antispark Switch

### Replies: 177 Views: 3659

## \#1 Posted by: Pedrodemio Posted at: 2019-01-26T14:33:59.848Z Reads: 492

```
I'm in need of new antispark switch, and most of the switches are either too expensive or will suffer the same failures

As pointed by @b264 the main problem is the inrush current killing the MOSFET's as time goes on

Here are the requirements:

* all componentes from https://lcsc.com/ , this way we can get everything on the same shipping as the PCB from https://jlcpcb.com/ for ridiculously low prices *
* no micro controllers
* 100A continuous
* pre charge circuit
* up to 12S
* max size (need to look at my board what can fit, I think 30x50mm)

*the MOSFET's may need to come from another place

Any help appreciated, never designed anything for power switching and  higher voltage like this, only done mostly low power audio stuff

What I have so far is two candidates for the main MOSFET's:

* HY4306B6 from HuaYi Microelectronics - [datasheet](https://datasheet.lcsc.com/szlcsc/HY4306B6_C133391.pdf)
* NCEP85T25D from Wuxi NCE Power Semiconductor - [datasheet](http://ncepower.com/Upload/SGT/NCEP85T25Ddatasheet-14384485438.pdf)

I need to research more if they should be trusted, but from all the specs they look really similar to the IRFS7350

For the pre-charge the plan is to use a 555 timers (or maybe two if needed)

​

​
```

---
## \#2 Posted by: b264 Posted at: 2019-01-26T14:52:41.679Z Reads: 432

```
I'm working on a way, but so far can't eliminate the MCU from the design... it may be better to just use an [ATtiny10](https://lcsc.com/product-detail/MICROCHIP_MICROCHIP_ATTINY10-TSHR_ATTINY10-TSHR_C128438.html) or something rather than try to come up with an elaborate analog circuit
```

---
## \#3 Posted by: Pedrodemio Posted at: 2019-01-26T14:58:41.265Z Reads: 424

```
If I can't find a away I may go that route, I would rather avoid it to open it to as much people as possible

About the linear region operation, more FET's in parallel would help alleviate the problem? I say that because I've never blown my Vedder antispark, it has been in two board so far with a lot of mileage, it's only a matter of time? I need to study more on the subject
```

---
## \#4 Posted by: DeathCookies Posted at: 2019-01-28T17:51:54.890Z Reads: 399

```
The problem is that sometimes the user cannot See on the switch whether it is Turned off or on. Then it can Happen easily that the as switch is connect to the system in Turned on State which kills it. Most commonly
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-01-28T17:58:32.460Z Reads: 391

```
Arrow.com offers free shipping on every order no minimum purchase.

Would you be able to source parts from there?

Also, the whole inrush current problem is solved with the LTC7004.
https://www.analog.com/media/en/technical-documentation/data-sheets/LTC7004.pdf

page 11 of the datasheet.

https://easyeda.com/editor#id=|602dc2b7711e4c16b88d2f5de19e1ff6|42d88dfcf3ce4bfd8d401d1ee3b6d229
this is what I have been using.
It will charge 3mF without exploding, haven't tested 6mF, but it should survive, the RC timing circuit has a 300milisecond rise time.
NOTE: you need to bypass the ground plane with blue wires, (that is connect negative to negative) there are too any traces that impede the ground plane.

edit: oh bleh, the pcb is too wide, if you change the PTH parts to SMD and move the header, it *might* fit in 30x 50mm.

And maybe use the TPW1R306PL,L1Q instead of the IPB014N06NATMA1, you could fit three and still make it smaller.

Including the PCB shipping cost, it cost me about $70 to make three of these (well two, I screwed up the pins on one of the ltc7004s, but I can just order more from Arrow with free 1 day shipping).
```

---
## \#6 Posted by: Indiangummy Posted at: 2019-01-28T18:02:19.431Z Reads: 347

```
wooo, nice find. thats super interesting.

Edit; this is what @Gamer43 is referring to 
![06%20PM|539x500](upload://aJet8FaPcBSVwMNcWrE4i2nGaZX.png)
```

---
## \#7 Posted by: Gamer43 Posted at: 2019-01-28T18:06:19.773Z Reads: 315

```
Implementation is continued on the next page :).
```

---
## \#8 Posted by: Pedrodemio Posted at: 2019-01-28T18:17:10.066Z Reads: 311

```
@Gamer43 I took a look at them and really liked, what kills here is shipping, Mouser, Farnell and Digikey were all in the 40 USD no mater how little I ordered 

Really nice find of the LTC7004, I was giving up and just adding more MOSFET's to the Vedder switch, and you already having and schematic made my day

Thanks a lot, I will definetely look into it

Making a new PCB and changing the components are no problem, will post here once I have more compact layout
```

---
## \#9 Posted by: Gamer43 Posted at: 2019-01-28T18:28:36.468Z Reads: 308

```
Glad I could help. :)

Some passive values may need some tweaking, just realized I didn't quite follow the datasheet recommendations exactly... (i.e. the rise time may have been significantly longer than 300 miliseconds....)
Actually, nvm, what happened was I changed some values on the fly and didn't update them in the schematic.

Also, is Arrow still charging shipping for you?
I remember when I ordered parts internationally, they still offered a free option.
```

---
## \#10 Posted by: Pedrodemio Posted at: 2019-01-28T18:36:29.841Z Reads: 279

```
No, Arrow gives me free shipping, and a way better selection of components than LCSC

I will take a good look before ordering anything

I'm a bit lost on the connection to the switch on the header 1, the switch itself connects to pins 5,4 and 2 and an LED to 1 and 3?
```

---
## \#11 Posted by: Gamer43 Posted at: 2019-01-28T18:38:42.734Z Reads: 279

```
[quote="Pedrodemio, post:10, topic:82154"]
I’m a bit lost on the connection to the switch on the header 1, the switch itself connects to pins 5,4 and 2 and an LED to 1 and 3?
[/quote]

My apologies, I didn't label them in the schematic,
pin 1 is Normally Closed
pin 2 is Normally Open
pin 3 is Common
pin 4 is LED cathode
pin 5 is LED anode.
```

---
## \#12 Posted by: b264 Posted at: 2019-01-28T18:58:00.865Z Reads: 256

```
This is why I would want an auto powerdown after like 8 hours of inactivity
```

---
## \#13 Posted by: Pedrodemio Posted at: 2019-01-28T19:39:14.259Z Reads: 262

```
I was gonna ask if it's not a good idea to have a pull down resistors but it's build in

Thanks for the diagram

do you think that 3 TPW1R306PLL1QCT would be enough for the 100A goal? price wise they are cheaper than the IRFS7530 and llower Rdson

Another challenge I"m looking at is finding the right fuse, ideally I would like to mount it on the PCB, but once we go to higher current the automotive fuses start to get too big

I remember Batman from @raphaelchang used tiny PCB fuses in parallel, I may go that route
```

---
## \#14 Posted by: Gamer43 Posted at: 2019-01-28T20:05:32.559Z Reads: 246

```
They should be able to handle 100A but at those currents you also need to make sure the pcb traces can handle it as well. The entire PCB will need cooling if those currents are sustained. Cooling can be passive, like with a modest heatsink.

What I use for fuses is I inline an autolink fuse using ring terminals and bolts in my wiring. Trying to incorporate it on a pcb becomes too cumbersome.
```

---
## \#15 Posted by: Pedrodemio Posted at: 2019-01-28T20:11:15.247Z Reads: 236

```
I'm thinking is ditching the Toshibas since they are really small to work with

I'm really really space constrained that is hard to fit any of the common fuse types

So far I've found this one form Littlefuse that I really liked, but expensive

https://www.arrow.com/en/products/0881080.ur/littelfuse
```

---
## \#16 Posted by: deltazeta Posted at: 2019-01-28T20:21:26.438Z Reads: 238

```
Spent a lot of time thinking about this after @b264 explained the issue. Ended up going with a mcu attiny85 to control everything.

https://easyeda.com/ninetailfox97/fused

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words/2992/8860?u=deltazeta
```

---
## \#17 Posted by: Gamer43 Posted at: 2019-01-28T20:23:47.168Z Reads: 241

```
They have the same footprint as an SOIC-8, and unlike the DFN MOSFETs from ON Semi, they actually have leads, you shouldn't have a problem working with them; I used a standard soldering iron to switch out the MOSFETs on a FSESC 4.20 with them a little while back.

Are you sure you wouldn't be able to inline something like this? https://www.arrow.com/en/products/142.5631.6152/littelfuse
It has almost the same profile as 10 gauge wire once everything is bolted together.
```

---
## \#18 Posted by: b264 Posted at: 2019-01-28T20:32:13.949Z Reads: 226

```
@deltazeta Do you have the firmware for that?  Is it on github?
```

---
## \#19 Posted by: deltazeta Posted at: 2019-01-28T21:14:01.947Z Reads: 217

```
will upload once i'm back from class
```

---
## \#20 Posted by: Pedrodemio Posted at: 2019-01-28T22:37:35.667Z Reads: 238

```
[quote="Gamer43, post:14, topic:82154"]
They should be able to handle 100A but at those currents you also need to make sure the pcb traces can handle it as well. The entire PCB will need cooling if those currents are sustained. Cooling can be passive, like with a modest heatsink.
[/quote]

At least in my case it will be only peak, I doubt it will sustain anywhere near that

@deltazeta  will take a look in what you did, thanks

[quote="Gamer43, post:17, topic:82154"]
They have the same footprint as an SOIC-8, and unlike the DFN MOSFETs from ON Semi, they actually have leads, you shouldn’t have a problem working with them; I used a standard soldering iron to switch out the MOSFETs on a FSESC 4.20 with them a little while back.
[/quote]

Nice to hear that, I can use an SOIC-8 and just extend the pad to the bottom of it? Couldn't manage to find any component in EasyEDA that has the same package

The Midi ones I may manage to fit, even more if I go with the Toshiba ones that are slim
```

---
## \#21 Posted by: Gamer43 Posted at: 2019-01-29T00:45:22.660Z Reads: 230

```
[quote="Pedrodemio, post:20, topic:82154"]
> They should be able to handle 100A but at those currents you also need to make sure the pcb traces can handle it as well. The entire PCB will need cooling if those currents are sustained. Cooling can be passive, like with a modest heatsink.

At least in my case it will be only peak, I doubt it will sustain anywhere near that
[/quote]

Oh, they'll handle that no problem, then.

[quote="Pedrodemio, post:20, topic:82154"]
Nice to hear that, I can use an SOIC-8 and just extend the pad to the bottom of it? Couldn’t manage to find any component in EasyEDA that has the same package

The Midi ones I may manage to fit, even more if I go with the Toshiba ones that are slim
[/quote]

Actually, since the drain and source pins are contiguous on opposite sides (aside from the gate pin) simple rectangular pads should work with the right spacing. 
If not, they fit perfectly in the same footprint as the NTMFS5C628NL, which I believe is "DFN5 5x6mm" or "SO-8FL".
What you can do in easyEDA is place the NTMFS5C628NL and simply solder the TPW1R306Pl,L1Q in its place.

I know this because before I switched out the NTMFS5C628NL in my FSESC 4.20, I double checked the package drawings and soldered in the TPW1R306PL,L1Q. 
The FSESC 4.20 works better than ever xD.
```

---
## \#22 Posted by: Pedrodemio Posted at: 2019-01-29T02:58:32.432Z Reads: 202

```
That’s a valuable tip, I was going to do the package from scratch
```

---
## \#23 Posted by: deltazeta Posted at: 2019-01-29T05:05:14.106Z Reads: 222

```
@b264 @Pedrodemio here's the firmware for the attiny85

https://github.com/dzhang97/Antispark/blob/master/antispark.c
```

---
## \#25 Posted by: Blasto Posted at: 2019-01-29T17:17:20.660Z Reads: 198

```
Design and testing tip, while adjusting fet gate timer, do all your tests with a single fet. That single fet must be able to take the inrush, to wich will be greatly reduced by the gate cap. While testing at the max voltage, use batteries, not a power supply.

Adding // fets will improve the reliability and reduce the Rdson
```

---
## \#26 Posted by: Pedrodemio Posted at: 2019-02-03T22:01:32.676Z Reads: 195

```
Thanks Blasto, will see to it

I didn't have much to work but was thinking, how does the LTC7004 current limiter is better than the Vedder implementation? Would’t we be also operating in the linear region as @b264 explained?

If yes, one way I thought to overcome that is to set the ramping time to a few seconds, but have another MOSFET with a current limiting resistor inline that turns immediately and a few seconds later it’s turned off by 555 timer, the majority of the current would pass by the limited current

Or maybe go back to my initial idea of using two 555 timers, one that turns the current limited MOSFET immediately and turn it off after a few seconds and then another 555 turn all the mains MOSFETs on after a few seconds


  https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967/4?u=pedrodemio
```

---
## \#27 Posted by: AlexBE Posted at: 2019-02-03T23:33:44.912Z Reads: 189

```
I don't think there is a problem operating in the linear region as long as you design the circuit correctly to not exceed the maximum ratings for the FET. Every product I have designed that uses a FET to switch power simply ramps the FET slowly enough to not exceed ratings. Don't use 555 timers, they will make the problem worse, just use a resistor and capacitor on the gate and get the values right to not exceed the current rating of the FET.

Quickest way is to just do a spice simulation. Let me know if you need help with this.
```

---
## \#28 Posted by: Pedrodemio Posted at: 2019-02-04T15:10:51.451Z Reads: 185

```
Nice, would gladly accept some help, I have an idea how to do it but trust more in someone else

The LTC7004 datasheet has some formulas to calculate the rise time but I doesn't take the current into account

On the spice we would just put a transistor being turned on by an RC network while powering a capacitance equal or greater than both VESC's combined and watching how high the current gets?
```

---
## \#29 Posted by: Kug3lis Posted at: 2019-02-04T15:19:07.439Z Reads: 187

```
My only suggestion for whole this project is not to put mosfet into linear mode they burn instantly doesn't matter how many 2,3,4 you will put in parallel inrush currents are thousands of amps for few tens of ms you can check your mosfet SOA and will see that these inrush will kill it instantly.

![image|656x375](upload://thEE2miUMwdiKgjRv6PXevxicqU.png)
```

---
## \#30 Posted by: Pedrodemio Posted at: 2019-02-04T15:51:17.199Z Reads: 175

```
That part I understood, but wouldn't the soft turn on of the LTC7004 with an adequate rise time make the current low enough? Or since an empty capacitor is almost a short, no matter how long the ramp up is the current would still be big?
```

---
## \#31 Posted by: Kug3lis Posted at: 2019-02-04T16:01:16.492Z Reads: 171

```
LTC7004 by slowing down opening will put Mosfet into linear mode
```

---
## \#32 Posted by: deucesdown Posted at: 2019-02-04T16:07:16.275Z Reads: 173

```
[quote="AlexBE, post:27, topic:82154"]
Don’t use 555 timers, they will make the problem worse
[/quote]

Sorry can you help educate a noob? A resistor with a timer would be an effective current limiting precharge circuit for the capacitors, no?
```

---
## \#33 Posted by: Blasto Posted at: 2019-02-04T17:09:30.621Z Reads: 181

```
what i don't like about LTC7004 is the external Vcc that is required (15V MAX)

if you are able to work with that, i'm sure you can it can be done

did a little sim for fun, not sure how accurate it is

![image|690x476](upload://mH2WxhUePAPlxSppCl5HLMqRFp7.png) 

like @Kug3lis said, you need to look at the SOA curve of your chosen fet
```

---
## \#34 Posted by: Blasto Posted at: 2019-02-04T18:06:18.496Z Reads: 181

```
same circuit but removing the gate cap, you can see the monster current spike, insta blow

![image|690x470](upload://fE2TADP39clGifd0Kk2XT2A2lkt.png)
```

---
## \#35 Posted by: Gamer43 Posted at: 2019-02-04T19:00:11.175Z Reads: 184

```
[quote="Pedrodemio, post:28, topic:82154"]
The LTC7004 datasheet has some formulas to calculate the rise time but I doesn’t take the current into account
[/quote]
There should be formulas for calculating inrush current, if not, assuming you know the rise time, the inrush current will be (Load Capacitance * System Voltage ) / Rise-Time.
For example, system voltage of 40V, load capacitance of 3,000uF, Rise-Time of 100ms, inrush current will be
3,000uF * 40V / 100ms = 1.2A.

[quote="Kug3lis, post:29, topic:82154"]
inrush currents are thousands of amps for few tens of ms you can check your mosfet SOA and will see that these inrush will kill it instantly.
[/quote]

The purpose of the RC timing circuit is to limit this inrush current from the hundreds of Amperes to something more manageable such as a couple amperes or even less than an ampere. In this case, since the rise time is significant, the circuit just needs to not exceed the maximum power dissipation of the MOSFET, which in this case is 170W.

From the above example, the peak power dissipation will be 50W (40V * 1.2A).

[quote="Blasto, post:33, topic:82154"]
what i don’t like about LTC7004 is the external Vcc that is required (15V MAX)
[/quote]
It has a very low quiescent current, less than 1mA, something like the ZXTR2112F-7 provides a 12V supply without issue. 
https://www.digikey.com/product-detail/en/diodes-incorporated/ZXTR2112F-7/ZXTR2112F-7DICT-ND/5371921


In order to implement automatic turnoff, bi-directional current sensing and some kind of timing element is required. This is most easily realized with a current sense amp and a microcontroller. It can be done using a current sense amp and window comparator with timing circuit, but that is really annoying to design.

Unfortunately all of the LTC700x series chips with current sensing only have unidirectional current sensing, not sure how it would behave with negative load current.
But, if the on-chip current sense amplifier recovers without a problem from negative saturation, then using the LTC7003 in tandem with a MCU can implement automatic turnoff.
```

---
## \#36 Posted by: Kug3lis Posted at: 2019-02-04T19:04:42.041Z Reads: 156

```
Well specialist :D You know better and u have design and replaced design n times :) sot block mosfets burn which are rated 4kA impulse currents :smiley:

Mosfets in linear mode at low voltage with high resistance burn like popcorns do even 200, 1000ms Mosfet is not a resistor :D
```

---
## \#37 Posted by: Gamer43 Posted at: 2019-02-04T19:21:21.238Z Reads: 155

```
I have not worked with such high power circuits before, but I have destroyed my fair share of power MOSFETs (mainly from avalanche breakdown), and I have destroyed power MOSFETs in a low side switch which did not implement precharge. 

I currently have two switches designed with the LTC7004 working in an electric mountainboard and electric scooter for a few months now, they switch 40V with a load capacitance of 1,200uF - 2,000uF.
I have tested them up to 42V at a load capacitance of up to 6,000uF.
They have a rise-time of 100ms (might be longer because I didn't size my capacitors correctly) and use two IPB014N06NATMA1.

If they fail next week, then you have proven your point. 
There is a load capacitance at which the switches will fail, but that's why designs have to keep things like those in mind, *what is the highest load capacitance and system voltage this device will encounter and can it survive in those conditions?*

In this case, longer rise-times will be required to handle large load capacitances and supply voltages.
```

---
## \#38 Posted by: AlexBE Posted at: 2019-02-04T23:44:08.175Z Reads: 151

```
[quote="Gamer43, post:35, topic:82154"]
There should be formulas for calculating inrush current, if not, assuming you know the rise time, the inrush current will be (Load Capacitance * System Voltage ) / Rise-Time.
For example, system voltage of 40V, load capacitance of 3,000uF, Rise-Time of 100ms, inrush current will be
3,000uF * 40V / 100ms = 1.2A.
[/quote]

This doesn't work, MOSFETs don't turn on like that, they turn on suddenly at the threshold voltage. Similarly the gate doesn't rise linearly.

Are you guys discussing a LTC7004 because you need a high side driver? Why not put the FET on the low side?
```

---
## \#39 Posted by: Gamer43 Posted at: 2019-02-04T23:46:36.216Z Reads: 158

```
[quote="AlexBE, post:38, topic:82154"]
> There should be formulas for calculating inrush current, if not, assuming you know the rise time, the inrush current will be (Load Capacitance * System Voltage ) / Rise-Time.
> For example, system voltage of 40V, load capacitance of 3,000uF, Rise-Time of 100ms, inrush current will be
> 3,000uF * 40V / 100ms = 1.2A.

This doesn’t work, MOSFETs don’t turn on like that, they turn on suddenly at the threshold voltage. Similarly the gate doesn’t rise linearly.

Are you guys discussing a LTC7004 because you need a high side driver? Why not put the FET on the low side?
[/quote]

The RC timing circuit as described in the LTC7004 datasheet FORCES the gate voltage (referenced to ground of the system!) of the MOSFETs to rise linearly, and the source voltage trails by 2-4V (voltage at which miller region is encountered). The MOSFET is driven in the miller (linear) region, it passes the necessary current through it to have the source voltage rise at the same rate the RC timing network charges.

Because of the way capacitors work, in order for the voltage across them to rise linearly, a constant current must be passed through them.

Basically the MOSFET is being driven to act as a constant current source until the load capacitance is charged to supply voltage, and because of the way the miller region works, the rate of voltage rise ends up being linear.

This is exactly what happened in Blasto's LTSpice simulation.
Constant current through MOSFET (at non-constant drain-source voltage) and linearly decreasing drain-source voltage.

The issue with low side switching is since everything is referenced to ground, it runs the risk of accidentally shorting something to ground, the device being switched ends up floating at some significant voltage above ground.
```

---
## \#40 Posted by: AlexBE Posted at: 2019-02-05T00:04:16.722Z Reads: 145

```
Ahh ok, sorry didn't realise it was a fancy driver.
```

---
## \#41 Posted by: Pedrodemio Posted at: 2019-02-05T00:13:01.512Z Reads: 155

```
That's all starting to make more sense, thanks for the great discussion so far guys

The MOSFET has to be capable of operating like a resistor, otherwise it wouldn't be possible to build any current source with them
```

---
## \#42 Posted by: Pedrodemio Posted at: 2019-02-05T12:37:19.451Z Reads: 150

```
Thanks for the simulations Blasto

Could you do them with the original vedder circuit please?

![Schematic|690x216](upload://iLJQuk0FhqjdrAGUhxpgmHDNpEO.png)
```

---
## \#43 Posted by: Vanarian Posted at: 2019-02-05T14:28:26.697Z Reads: 139

```
Nice job, I can't wait to see what you guys come up with !
```

---
## \#44 Posted by: Gamer43 Posted at: 2019-02-07T00:21:12.909Z Reads: 140

```
@Pedrodemio
![image|690x255](upload://tmhqkKhAiRxsx5hwCaEXzIk0l1B.png) 
Hey guys, I drew up a schematic that I think should work for an antispark switch to implement push-to-start and automatic turn off (not sure how accurate the embedded current sense amp in the ltc7003 is, so not sure if auto turn off is viable with the ltc7003, if not, would have to leave the current sense feature unused and add an ina240 current sense amp, Push-to-start may not work with extremely high kv motors or high speed gearing, in this design, it relies on the BEMF generated and rectified through the motor controllers).


It would be used with a momentary push button such as this https://www.adafruit.com/product/481.
Let me know what you guys think, if this looks viable I'll see if I have time to build and test a few prototypes.

Drawing up a BOM, using parts from Digikey, and using JLPCB's quoting tool, for a prototype run of 10 of these, 2layer 2oz copper, the price would be $20 each to produce.
Would be slightly cheaper (~$17 per unit) if ordering from Arrow.com.
```

---
## \#45 Posted by: Gamer43 Posted at: 2019-04-03T09:26:37.987Z Reads: 142

```
Actually, while I figure out the details of a push-to-start antispark, here's a relatively simple lowside antispark switch that implements pre-charge. I have a prototype of it at home, but won't be able to post a picture of it until this weekend.
I actually used said prototype in my mountainboard before I moved on to the LTC7004 switch.

If anyone wants to mass produce this and sell it for a low cost feel free.

![image|690x279](upload://A9s9k9L9mbFfUQDi5NDbJpOLBF.png) 
![image|462x370](upload://wIp2QT6N38qOdcLCJvHeRxEARyC.png) 

https://easyeda.com/RuBisCO/LowsideSwitch

@Pedrodemio
This design shouldn't cost more than $10 to make per unit. Maybe $40 for three due to the shipping cost on the PCBs, but protoboard can get around that :P.
```

---
## \#46 Posted by: moon Posted at: 2019-04-03T09:27:18.700Z Reads: 134

```
@shaman maybe this is a project for you.
```

---
## \#47 Posted by: shaman Posted at: 2019-04-03T12:02:31.246Z Reads: 131

```
Yeah might be decent gadget to lump in with my FOCers
```

---
## \#48 Posted by: Pedrodemio Posted at: 2019-04-03T12:43:54.648Z Reads: 128

```
Thanks a lot

If @shaman does it I will probably get one if it can handle a good amount of current

My design still as it was since I’m having little time to work on it
```

---
## \#49 Posted by: shaman Posted at: 2019-04-03T13:09:46.852Z Reads: 125

```
How much current is considered a good amount?
```

---
## \#50 Posted by: Pedrodemio Posted at: 2019-04-03T13:11:33.430Z Reads: 124

```
I’m aiming for 100A peak I.e, for at least 30s, probably that’s already considered continuous
```

---
## \#51 Posted by: shaman Posted at: 2019-04-03T13:13:24.368Z Reads: 120

```
Sort of a tall order but not impossible. Just more FETs in parallel and maybe a small heatsink
```

---
## \#52 Posted by: Gamer43 Posted at: 2019-04-03T20:32:35.919Z Reads: 124

```
Actually, I speced the wrong MOSFET, the price on the ipb014n06n went up. Better would be to use three TPW1R306PL,L1Q in parallel. I'll redo the schematic and design to incorporate those mosfets instead.
```

---
## \#53 Posted by: Gamer43 Posted at: 2019-04-03T21:42:16.572Z Reads: 130

```
ok, how does this look?
![image|690x252](upload://hH8QsjfgguMINN58nJtRa2gn7AY.png) 
![image|642x500](upload://2puOM61J2arfO376zumWtpYIcoQ.png)
```

---
## \#54 Posted by: shaman Posted at: 2019-04-03T22:47:35.159Z Reads: 125

```
I see you are using "thermals" for connecting the FETs and OUT/BATT pads to the planes. While this makes soldering easier, you constrict current flow during operation. Maybe consider have direct connections with these pads for improved current flow and less heating during operation.

Also consider utilizing the bottom layer for helping carry the high current portions as well. You can via stitch the 2 layers together.
```

---
## \#55 Posted by: AlexBE Posted at: 2019-04-04T02:01:46.661Z Reads: 115

```
@shaman is exactly correct. Don't use any thermals and use both sides of the PCB to carry current AND wick heat away from the FETs. I would also space the FETs as far from each other as possible to allow the centre one to get more heat out. I would also ditch through hole components.
```

---
## \#57 Posted by: shaman Posted at: 2019-04-04T12:15:55.064Z Reads: 113

```
I'd say the choice of through hole vs smd would be whether or not you want this to be easy to assemble by a DIYer. SMD would better for Design For Manufacturing (DFM) since pick-and-place is low-cost compared to manual soldering. Pros and cons to each choice here
```

---
## \#58 Posted by: AlexBE Posted at: 2019-04-05T01:17:49.897Z Reads: 113

```
I agree with the general point about diy, however I think for this application it doesn't make sense for 3 reasons.

* There are three large surface mount FETs that cannot be hand soldered, so a diy'er will have to reflow them anyway.
* 10 years ago someone might have been able to save money by hand assembling this kind of board. However these days with small run contract assembly so cheap in China, I guarantee it will be cheaper to buy an assembled version of this board than by making your own.
* An antispark switch is a critical safety component. If one fails the rider could be seriously injured. For that reason I would suggest that people should only buy assembled boards that have been tested to give some level of confidence that they aren't going to fail. If a diy'er is put off by the idea of surface mount assembly (given that they have to do the FETs anyway) they should reconsider just buying a tested switch.
```

---
## \#59 Posted by: AlexBE Posted at: 2019-04-05T01:31:43.598Z Reads: 112

```
Hi @Gamer43, along with my other comments. I would make all the traces on this board much thicker. This board is safety critical and will be in a high vibration environment. Last thing you want is a trace breaking.
```

---
## \#60 Posted by: Gamer43 Posted at: 2019-04-05T01:45:49.204Z Reads: 114

```
The MOSFETs have leads on them, they can easily be hand soldered.
I know because I did it on a flipsky 4.20 xD.

(yes aside from the faults common to all pre-fix 4.20's, it works just as it should :P)
```

---
## \#61 Posted by: AlexBE Posted at: 2019-04-05T01:51:06.490Z Reads: 121

```
If the plane thermals are removed, those mosfets will not be easy to solder. Easy for me, easy for you sure. However if someone is in the situation where they think that 0805 ish surface mount is too hard, they are going to struggle with mosfets attached to large copper planes. 

To me it makes no sense to have a board where you are saying that surface mount resistors are too hard, need to go through hole. However soldering a large mosfet to a solid copper plane with a center thermal pad is easy.
```

---
## \#62 Posted by: Gamer43 Posted at: 2019-04-05T01:52:13.951Z Reads: 129

```
It is when you use the TS80 soldering iron :PPPPP

Seriously, that iron rocks at heat delivery. Dave from EEVblog soldered a TO-220's tab to a huge copper ground plane with it.

Edit: here's a picture of the prototype.
![1554429392641964496387157663201|375x500](upload://gaMLJa3Unf2sNn8m6yWuYBOFEC1.jpeg) 
![15544294329032940100491727801535|375x500](upload://ctNlAsdLgo40YYaLjYhQbaFSEia.jpeg)

MOSFETs used are the IPP029N06N
```

---
## \#63 Posted by: AlexBE Posted at: 2019-04-05T02:09:27.176Z Reads: 120

```
I think you are deliberately ignoring my point.
```

---
## \#64 Posted by: Gamer43 Posted at: 2019-04-05T02:30:48.159Z Reads: 121

```
I'll spin two PCB designs, one with SMD and no thermal reliefs, and a second one with all through hole and thermal reliefs and possibly with a different kind of MOSFET.

This way, someone can mass produce the SMD PCB and have it work perfect, and anyone who's up for DiY can spin the through-hole PCB for themselves.

Also, small run assembly can still run up $5-10 dollars per board in 10 quantity Dx.
```

---
## \#65 Posted by: Gamer43 Posted at: 2019-04-12T06:06:44.435Z Reads: 125

```
Okay, I finally got around to redoing the PCB, how does this look?
@shaman
@AlexBE  

Dimensions are ~55mm x 39mm.

![image|690x451](upload://rS63xZ9AJVO7lxftIKZQwyUH2qm.png)  
![image|690x460](upload://jPQZfcblXEUYzh4U1t33KC52nhq.png) 

This is some A+ via stitching xD.

Any traces I should make thicker or clearances I should increase beyond 10mils?

Schematic for reference 
![image|690x271](upload://ukPSQhL06sIirZp9mpJum9so0lN.png)
```

---
## \#66 Posted by: AlexBE Posted at: 2019-04-12T07:07:13.340Z Reads: 117

```
I would
* make the main 4 solder pads much larger
* Reroute Batt- -> NO to not cut the top copper in half
* Not sure what the P1 connector is, but if it's simple header pins, I would change to a locking RA connector.
* Similarly I would move H1 and P1 down to level with R6 to take them out of the high current path
* Then because I'm being picky - The entire board can be made much smaller and thinner (RA connectors)
* LED connector should be locking also, so much vibration in this environment. I suppose most people would solder those connections though.
```

---
## \#67 Posted by: Gamer43 Posted at: 2019-04-12T07:13:19.628Z Reads: 122

```
The headers are intended to be soldered with JST XH connectors, which I believe are locking (at least to some extent).

I thought the pads were large enough to solder 10 AWG, if not, I'll make them 250x250mils.

Not sure how practical this would be, but I was also intending that the two BATT+ pads be bypassed with external wires, as that is what I have done on all my prototype antisparks, or better yet, don't run the positive current path through the antispark at all (i.e. only use one of the BATT+ pads).

Just realized I had the silkscreen mixed up on the headers xD, fixed that.

EDIT:
@AlexBE, okay I fixed a few things that were dumb
![image|690x461](upload://3sUx8857hINOkjnbL3m4Scvisz1.png)  
![image|690x446](upload://cgZ6ko1J1OnvOWCrspQV0igSJhA.png)
```

---
## \#68 Posted by: AlexBE Posted at: 2019-04-12T07:48:25.129Z Reads: 115

```
[quote="Gamer43, post:67, topic:82154"]
The headers are intended to be soldered with JST XH connectors
[/quote]
Did you have the silkscreen box correct for those connectors? I don't think they look big enough. You also have different size holes for the two connectors. I believe a JST-XH connector will interfere with R4, it will at least be close. Not sure what software you are using, but I always find it is useful to import all the 3d models.

[quote="Gamer43, post:67, topic:82154"]
I thought the pads were large enough to solder 10 AWG, if not, I’ll make them 250x250mils.
[/quote]
They are large enough, but why not extend them double the length towards the centre of the board?

[quote="Gamer43, post:67, topic:82154"]
Not sure how practical this would be, but I was also intending that the two BATT+ pads be bypassed with external wires, as that is what I have done on all my prototype antisparks, or better yet, don’t run the positive current path through the antispark at all (i.e. only use one of the BATT+ pads).
[/quote]
Yes this is a good way of doing it, depending how neat you are. I don't use anti-spark, but if I did I would connect to both batt+ pads for neatness.
```

---
## \#69 Posted by: Gamer43 Posted at: 2019-04-12T08:17:39.725Z Reads: 119

```
Oh, you're right about the silkscreen, my bad. 

I'm using EasyEDA, not the best, but works for getting something up quickly.

I don't want to make the pads too big, because I don't want to put vias in them; from my experience, soldering on vias can sometimes get the solder to drip and pool down on the other side.

![image|690x449](upload://t3GYM0ckZy8CJea5MhmPRL5CGUM.png)  
![image|690x451](upload://A3hEg2kZrJsLgsXfnSA9YzrLPIW.png)
```

---
## \#70 Posted by: AlexBE Posted at: 2019-04-12T08:24:07.308Z Reads: 110

```
Ok so now I'm nickpicking, because that's my job.
* You will get pinged for silkscreen on copper on the connectors (manufacturer might fix it for you)
* Would be much better to be single sided if you can squeeze it in. 
* Ideally the NO NC C etc labels would be visible with the connector mounted.
```

---
## \#71 Posted by: Gamer43 Posted at: 2019-04-12T08:52:23.739Z Reads: 124

```
How does this look? Can't fix the silk screen, manufacturer will most likely do that.

If this design works, it should be bulletproof. If anything fails, it'll be the zener diodes, which are cheap and easy to replace. And if they fail, it won't be catastrophic.
![image|678x500](upload://gGbrRYgfP9DO3vbDpjAHKKqN2Qh.png)  
![image|686x500](upload://rdJ3KKwek4YiLVfKBMvwI2uZbdv.png)
```

---
## \#72 Posted by: Pedrodemio Posted at: 2019-04-12T10:58:54.737Z Reads: 111

```
Looking good, I would make the output pads a bit wider so two wires cans be soldered, onde for each vesc directly from the switch
```

---
## \#73 Posted by: shaman Posted at: 2019-04-12T12:24:14.663Z Reads: 110

```
@Gamer43

Your doing good here. This board is looking nice  👍
```

---
## \#74 Posted by: Gamer43 Posted at: 2019-04-12T21:20:27.583Z Reads: 111

```
Who wants to be the guinea pigs for a prototype run? :p

By my estimates, in 200+ quantity, this shouldn't cost more than $10 per switch to make through a turnkey PCB assembly service. (with 3oz. copper and ENIG :O)

Is the $20 100A 60V antispark (that doesn't die) finally here?
Better question, can we get 200 people to buy this? X_X.
```

---
## \#75 Posted by: Schtekarsten Posted at: 2019-04-12T22:27:40.147Z Reads: 107

```
:heart_eyes:is it possible to go for smaller batches?
```

---
## \#76 Posted by: Gamer43 Posted at: 2019-04-12T22:53:08.157Z Reads: 108

```
It would cost more, like twice as much unfortunately :(.
```

---
## \#77 Posted by: SeanHacker Posted at: 2019-04-12T22:59:11.550Z Reads: 107

```
[quote="Gamer43, post:74, topic:82154"]
can we get 200 people to buy this?
[/quote]

199 left to go. ;)
```

---
## \#78 Posted by: Gamer43 Posted at: 2019-04-13T06:01:24.645Z Reads: 108

```
I have enough MOSFETs to make three prototypes, I think I'll order the PCBs sometime next week, who wants to be the first ones to try out the new antispark?
```

---
## \#79 Posted by: b264 Posted at: 2019-04-16T20:01:07.022Z Reads: 106

```
Why isn't there a precharge circuit on that?
```

---
## \#80 Posted by: Gamer43 Posted at: 2019-04-16T20:03:28.896Z Reads: 109

```
The switch controls the precharge circuit, MOSFETs turn on when the voltage difference is below 4V.

By connecting Common and Normally Open, the resistors bypass the MOSFETs, charging up the load capacitance. Once the voltage difference between the input and output is less than 12 - (7.5 + 0.7)V, Q3 turns on and activates the primary MOSFETs.

Connecting Common and Normally Closed disconnects the pre-charge resistors and shorts MOSFET gate to ground, turning it off.
```

---
## \#81 Posted by: b264 Posted at: 2019-04-16T20:06:55.999Z Reads: 106

```
Which resistor is the precharge happening through?
```

---
## \#82 Posted by: Gamer43 Posted at: 2019-04-16T20:07:39.811Z Reads: 110

```
R4 and R6, I'll repost the schematic down here for reference.

![image|690x271](upload://ukPSQhL06sIirZp9mpJum9so0lN.png)
```

---
## \#83 Posted by: b264 Posted at: 2019-04-16T20:09:02.375Z Reads: 109

```
Ohhhhh this doesn't use a momentary switch and precharges through the switch itself.  Interesting design! :smiley:
```

---
## \#84 Posted by: Gamer43 Posted at: 2019-04-16T20:11:19.880Z Reads: 109

```
Something like this would be a perfect toggle switch :).
Contacts are rated for 3A 250VDC.
https://www.adafruit.com/product/482

My first iteration didn't have precharge, the pair of IPP029N06N blew up immediately XD. 
![image|375x500](upload://o4BfcQAnUPuCsmcGD7l8GyZfEw1.jpeg) 
![image|375x500](upload://vjL3lNayHH4kHS02Edp6zRzXo3L.jpeg) 

Prototype employing roughly the same schematic. Worked in my mountainboard until I moved over to the LTC7004. Switch was soldered directly to the terminals on the board.
```

---
## \#85 Posted by: Jamie42 Posted at: 2019-04-16T20:19:09.322Z Reads: 106

```
Can we possibly get this with push to start? Would be so damn cool!
```

---
## \#86 Posted by: Gamer43 Posted at: 2019-04-16T20:49:06.582Z Reads: 107

```
Impossible with this design.

Roll-to-start and auto-turn-off design is coming in May.
May not even need a pushbutton hehe.
```

---
## \#87 Posted by: b264 Posted at: 2019-04-16T20:54:50.480Z Reads: 102

```
I would strongly suggest referring to that as "roll-to-start".  "Push" is what you do when you operate the switch.
```

---
## \#88 Posted by: Gamer43 Posted at: 2019-04-16T21:28:12.404Z Reads: 106

```
My mistake, did not realize that, thanks.
```

---
## \#89 Posted by: Vanarian Posted at: 2019-04-16T21:28:50.624Z Reads: 104

```
Any chance to make it with a momentary soft latch switch circuit ? Nice work.
```

---
## \#90 Posted by: Gamer43 Posted at: 2019-04-16T21:30:55.029Z Reads: 104

```
It would need a 555 timer as toggle latch. This would add many more components and make the switch more expensive and potentially less reliable.
```

---
## \#91 Posted by: b264 Posted at: 2019-04-16T23:43:17.593Z Reads: 100

```
You'd really need an MCU for that.  It might be able to be done with a single latch, but an MCU would work much better.  I like this current design, it's innovative :slight_smile:

4.0V delta I think is a tad too high but I am curious to see how it works :smiley:
```

---
## \#92 Posted by: Gamer43 Posted at: 2019-04-16T23:44:53.290Z Reads: 100

```
Worked for 20+ cycles, I'll experiment with larger sized zener diodes once I spin out more prototypes in the next week or two. On the first prototype, using larger zeners, I ran into problems with the main MOSFETs not turning on.
4V delta (probably lower honestly) with 6,000uF of load capacitance results in 100mJ of energy dissipated, well below the avalanche energy rating of the MOSFETs
```

---
## \#93 Posted by: Deodand Posted at: 2019-04-17T00:24:24.975Z Reads: 106

```
My 2 cents here that everyone needs to keep in mind is that power dissipation is Volts*Amps. With the linear ramping of the gate we must keep in mind that at the beginning the voltage drop accross the FET is the full battery voltage. The total energy of the turn on event remains constant since you are charging a fixed capacitance to a fixed voltage. So at the very beginning of the turn on event say you are 10s full charge that's

     42V * (charging amps + passive system amps)

The turn on energy is 

     0.5*42V*(charging amps +  passive system amps)*turn on time

Every fet (even within the same batch) has a different voltage knee where the resistance plummets at a given gate voltage, because of this the parallel fet with the lowest Vgs knee due to variance handles the lionshare of the power dissipation. So your single fet must be powerful enough to handle both the instantaneous power as well as the total energy dumped from the turn on event.

The passive current draw can also become relevant for longer turn on times due to the high voltage drop. Say you had something drawing a few hundred milliamp, it ends up being 10s of watts dissipation. For instance, the buck will turn on the MCU and other peripherals when it charges above 5V, these will pull significantly more current then normal operation because the buck is stepping down from such a low voltage. So moral of the story is find a sweet spot with a slow enough turn on time to reduce peak power dissipation, but not so slow that you start dumping a lot of joules into the FET.
```

---
## \#94 Posted by: Gamer43 Posted at: 2019-04-17T02:25:48.120Z Reads: 99

```
I guess it's safe the say that the Unity power switch is bulletproof :).
```

---
## \#95 Posted by: Deodand Posted at: 2019-04-17T03:26:32.595Z Reads: 95

```
@Blasto and I spent so many hours getting that damn thing to work properly :slight_smile:
```

---
## \#97 Posted by: b264 Posted at: 2019-04-17T03:38:19.907Z Reads: 93

```
Is the Unity power switch on the other side of the filter capacitors and so does not have this large turn-on inrush?
```

---
## \#98 Posted by: Deodand Posted at: 2019-04-17T03:48:51.787Z Reads: 100

```
Nope it's an anti-spark, just carefully designed with a known capacitance which means you can make it reliable.
```

---
## \#99 Posted by: Gamer43 Posted at: 2019-04-17T04:06:53.774Z Reads: 101

```
Just curious, have you considered a power on-off solution purely by pulling the DRV8301 enable pins low and putting the MCU into stop mode? Power can supplied to the MCU in this state using a high voltage LDO.

@Deodand Also, did you see my post in the FOC switching frequency thread, you didn't reply, so not sure if you saw it. Or was my post so dumb you ignored it xD.
```

---
## \#100 Posted by: b264 Posted at: 2019-04-17T04:34:27.557Z Reads: 101

```
I think that would subject the main battery to the filter capacitors' leakage current.
```

---
## \#101 Posted by: Gamer43 Posted at: 2019-04-17T04:36:57.309Z Reads: 100

```
Aren't electrolytic capacitor leakage currents on the orders of uA though?
```

---
## \#102 Posted by: Deodand Posted at: 2019-04-17T04:58:17.083Z Reads: 104

```
Yeah it comes down to leakage we did the math and it was a bit too high. Kind of on the edge like 100s of uA where it'd drain your battery in a month or so. Think I did a hardware test and got something similar.
```

---
## \#103 Posted by: Gamer43 Posted at: 2019-04-17T07:35:39.919Z Reads: 105

```
Have you considered hybrid polymer caps? :P.

https://www.digikey.com/product-detail/en/united-chemi-con/HHXC630ARA820MJA0G/565-4791-1-ND/7556762

Ten of these in parallel would only have a maximum leakage of 500uA. It would take three years to drain a 12Ah battery, so if said battery were at storage charge, it would take a full year to drain. Low ESR, impassible to transients, heck why aren't we using ten of these in parallel xD.
```

---
## \#104 Posted by: Blasto Posted at: 2019-04-17T15:04:32.843Z Reads: 99

```
even 500uA is too high of a leakage (well in our book), those smd cap if not properly glued down, will break off in a high vibration environment.

Really like your circuit, very clever.

Little tip while qualifying your switch for inrush, only mount a single fet. If that single fet is able to handle the entire inrush of the circuit, you're on your way to bullet proof.
```

---
## \#105 Posted by: Deodand Posted at: 2019-04-17T16:08:25.888Z Reads: 100

```
Yeah for the passive drain I like to look at worst case, someone rides their 10s2p battery to dead with no discharge protection and leaves it plugged in. Those things are like 5Ah capacity, assuming lower cutoff is like 3.1V then you have about 10% of battery left (0.5Ah)  so 1000 hrs or 40 days until you start doing some damage to the pack.
```

---
## \#106 Posted by: Gamer43 Posted at: 2019-04-18T04:10:59.845Z Reads: 109

```
This is what the design looks like right now, any other thoughts before I order up the PCBs and start making prototypes? @Pedrodemio @AlexBE @shaman @Deodand @Blasto  

![image|690x233](upload://6pKU2dXdW8qHNi631oZeki8B8ov.png) 

![image|690x494](upload://3X8qmn3ZAgHvHvdCYz7nnh7GPLX.png) 

![image|690x497](upload://r0m84Xu9JcAZUEniCeOd1nXikdi.png)
```

---
## \#107 Posted by: b264 Posted at: 2019-04-18T04:13:07.681Z Reads: 103

```
You need to put a bunch of vias under where the heavy gauge wires solder to the PCB.  It keeps the wires from ripping the pads off.

Inside the actual places you're soldering to.
```

---
## \#108 Posted by: b264 Posted at: 2019-04-18T04:16:17.330Z Reads: 97

```
On the surface mount pads that aren't high-current, if you put a ring of no copper around them, with only a little piece connected, it makes the heat flow much better while soldering because the giant plane doesn't try to suck heat from the tiny pad.  For the high-current pads, you can't do that.
```

---
## \#109 Posted by: Deodand Posted at: 2019-04-18T04:18:25.378Z Reads: 102

```
I'd add independent gate resistors. Like a 10 ohm between them to damp parasitic oscillation. I didn't think they would matter with the slow turn on of our linear charge circuit but experimentally it seemed to drastically reduce failure rate.
```

---
## \#110 Posted by: b264 Posted at: 2019-04-18T04:19:52.408Z Reads: 102

```
Your schematic is clever.  I like how you solved this.
```

---
## \#111 Posted by: Pedrodemio Posted at: 2019-04-18T13:54:49.457Z Reads: 106

```
Looks nice

If it’s not too much work I would mãe it even smaller, in my eyes there is plenty of room to shrink it width wise

Q3, R1, R7 and D1 could go down just a little bit and then move the battery pads closer to the center of the board

Same thing with the output pads, once you put vias in the pads itself you can bring it closer to P2
```

---
## \#112 Posted by: Gamer43 Posted at: 2019-04-19T10:18:09.013Z Reads: 109

```
Okay, so a few things:

Easyeda does not allow me to selectively choose which pads to attach thermal reliefs to :(, so I'll have to bite the bullet and solder tiny pads to huge ground planes. Shouldn't be a problem with the TS80, might be a problem during reflow??

I just realized that when the primary MOSFETs are turning on, Q3 is driven into forward active mode (similar to the linear region of a MOSFET). I think this is why I didn't see problems with failures during testing of the initial prototype, and also why I couldn't get it to turn on with larger sized zener diodes. This occurs because as the collector current through Q3 increases, R1 drops more voltage, thus causing the emitter voltage of Q3 to fall, restricting base current.

I can't really move the components around much more, unless I want to redesign the PCB, should I go for that instead? I don't think I'll be able to shrink the PCB much more either.

Current Dimensions are 54mm x 39mm.

![image|682x500](upload://5Hiu8poNIlZUAJ3lt9mjXB8q62U.png) 

![image|669x500](upload://1ownFcgNgLSRWWRpQ18krWHpfDF.png)
```

---
## \#113 Posted by: b264 Posted at: 2019-04-19T18:38:48.198Z Reads: 96

```
I think you should make a small number of those as-is for proof-of-concept.

If it works as planned, then redesign the PCB to make it smaller.  Only after that would I add roll-to-start and auto-shut-off.
```

---
## \#114 Posted by: b264 Posted at: 2019-04-19T18:39:38.906Z Reads: 93

```
On the left, "BATT+" should say "OUT+", right?  Unless you did that on purpose, I can see why.
```

---
## \#115 Posted by: Gamer43 Posted at: 2019-04-21T00:54:58.434Z Reads: 91

```
I will rename the pad and order up the PCBs tomorrow. I have enough parts for three prototypes. Will let you guys know when those are ready. I will be keeping one for myself to test and will see if I can get the other two shipped to you guys for testing.
```

---
## \#116 Posted by: Gamer43 Posted at: 2019-04-21T23:19:50.105Z Reads: 87

```
PCBs ordered!

Will order necessary SMD parts sometime this week, and hopefully prototypes assembled this weekend!
I will be assembling three prototypes for now.
```

---
## \#117 Posted by: Gamer43 Posted at: 2019-04-24T12:18:38.256Z Reads: 85

```
Ordered all the parts

Total cost comes out to about $70 X_X. (Not counting the transistors, I already have those)
Also ordered three adafruit push buttons. They're green.
```

---
## \#118 Posted by: M.Hboards Posted at: 2019-04-24T14:29:56.383Z Reads: 84

```
Will you be selling these/ beta testing this? if yes how much and can i possibly get in?
```

---
## \#119 Posted by: Gamer43 Posted at: 2019-04-24T22:45:02.011Z Reads: 84

```
I am making three prototypes. I am keeping one for me to do my own testing with, the other two I can send to other people for testing.
```

---
## \#120 Posted by: M.Hboards Posted at: 2019-04-24T22:53:22.434Z Reads: 87

```
Can i get 1 of those 2? i have a build it could go in immediately.
```

---
## \#121 Posted by: Gamer43 Posted at: 2019-04-24T22:58:10.824Z Reads: 96

```
I can send one to you. I might have screwed up and not have the connectors until next week. And I leave for a two week vacation then -_-.
I might be able to ship it to you next week, but it may not have the connectors. Would that be alright? It needs a two pin and three pin connector, the spacing is 2.54mm. I intended for it to use right angle connectors, not sure if there is enough clearance between components for vertical connectors.

It is a prototype, so I can't guarantee it won't explode. I would highly recommend inlining a fuse.
```

---
## \#122 Posted by: M.Hboards Posted at: 2019-04-24T23:00:56.826Z Reads: 90

```
What are the 2 and 3 pin connectors for? The push botton to the switch?
```

---
## \#123 Posted by: Gamer43 Posted at: 2019-04-24T23:01:26.303Z Reads: 88

```
The LED and the Pushbutton.
```

---
## \#124 Posted by: M.Hboards Posted at: 2019-04-24T23:04:19.086Z Reads: 84

```
It's it a jst connector? You have a pic of what the connector looks like? I do have basic soldering skills so maybe i could solder directly on
```

---
## \#125 Posted by: Gamer43 Posted at: 2019-04-24T23:26:42.112Z Reads: 92

```
JST, or just standard 2.54mm pin headers if you really want. I might able to supply those. Just need to be careful and make sure they are connected the right way. (Silkscreen is labelled).

Actually, if the JST connectors don't arrive in time, I'll just solder female pin headers and supply male pin headers.
```

---
## \#126 Posted by: M.Hboards Posted at: 2019-04-24T23:34:51.997Z Reads: 94

```
[quote="Gamer43, post:125, topic:82154"]
Actually, if the JST connectors don’t arrive in time, I’ll just solder female pin headers and supply male pin headers.
[/quote]

Sounds good. I basically just need to solder on xt60s right? Are you sending the prototypes out for free? 
Also you have a link to a fuse you would recommend to solder in line? The fuse is soldered onto the positive lead right? The only prob i might have is that it might Be a tad too big I'll open my enclosure to make sure it will fit before your ready to send it out. what's the approximate height of it?
```

---
## \#127 Posted by: Gamer43 Posted at: 2019-04-25T00:26:26.271Z Reads: 92

```
Dimensions are 55 x 39mm

You will need to solder wires to the pads (and xt connectors to those wires)

By inlining a fuse, there are some inline fuse holders for ATC blade fuses you could use, or what I did is I got some auto-link fuses and using ring terminals, bolt the fuse inline.

I'll send them out for free. They are prototypes after all. All I ask in return is feedback and test information.
```

---
## \#128 Posted by: M.Hboards Posted at: 2019-04-25T00:30:24.694Z Reads: 89

```
You have a link to a recommended fuse? Does the fuse go on the positive or negative leave? And before or after the switch?
```

---
## \#129 Posted by: Gamer43 Posted at: 2019-04-25T00:33:43.133Z Reads: 87

```
Before the switch, doesn't matter positive or negative, but I would recommend positive side.

https://www.arrow.com/en/products/142.5631.5702/littelfuse

These are the ones I'm using (I think)
There are different amperage ratings. The bolt holes are slightly too small for 1/4" 20 bolts, so either #14 will  work, or you could do what I did and drill it out.

Derp, the bolt holes are M5
```

---
## \#130 Posted by: Gamer43 Posted at: 2019-04-27T05:54:06.623Z Reads: 87

```
Okay, so I soldered together the first prototype.

Not sure what happened, but when I tried to spin up a motor, there was a loud POP and one of the drain pads was blown clean off.

The MOSFET was also arch-welded to the PCB.

The MOSFET also failed open-circuit, which is REALLY weird.

The ESC I was testing with is also dead, it's a short circuit.

Did the switch kill the ESC or did the ESC kill the switch? The 70A fuse on the 10s lipos I was using is still intact. (It's a slow blow automotive fuse)

The ESC was having problems prior, maybe the ESC died short-circuit, and then the switch saw a few hundred amperes and the single MOSFET I soldered on was like NOPE, K BAIIIYEEEEEEE.

:thinking:


EDIT: okay I think the short on the ESC killed the MOSFET. The exposed source pad on the MOSFET is a short with the drain pins, BUT the source PINS are open circuit. 
The ESC failed short, the few hundred amperes caused the MOSFET to fail short, but the MOSFET's internal bond wires to the source pins to burn.
Now the question is, was the ESC going to die on its own or did the switch do something to bring about its death?

I'm guessing it was the ESC, the ESC was having problems with having one or more phases being undriven. I'm guessing the gate on one of the MOSFETs ended up floating after being driven high, and shoot-through occurred.
```

---
## \#131 Posted by: b264 Posted at: 2019-04-27T07:28:48.222Z Reads: 80

```
What if you try with a heating element as a load instead of an ESC?  To eliminate any uncertainty.

Like, a straight capacitor, nothing else; then a straight heater/resistor, then both.
```

---
## \#132 Posted by: Gamer43 Posted at: 2019-04-27T07:32:10.800Z Reads: 85

```
I'll try a 10 ohm resistor once the primary MOSFET turns on.
```

---
## \#133 Posted by: Gamer43 Posted at: 2019-04-27T09:56:37.767Z Reads: 92

```
Good news, I tested with the 10 ohm resistor and a throw-away VESC.

Resistor got super hot.

throw-away vesc had no problems with FOC detection and keyboard input. I used modest current settings, +-20A everything, 6S lipo test pack.

Pretty sure the first ESC was on its last lengths, I heatguned the crap out of it xD. It's too bad it took a nice MOSFET with it.

I'll assemble the other two prototypes later this weekend and hopefully ship them out on Tuesday.
```

---
## \#134 Posted by: Gamer43 Posted at: 2019-04-28T00:40:08.060Z Reads: 94

```
![20190427_173700|375x500](upload://5jPaJHfdpuIdLiqLOSErr8q1UO4.jpeg) 

![20190427_173713|375x500](upload://pCI6ytIqlLdKwOTHgwjaztrPBhq.jpeg) 

*I love smd soldering*

*Don't ask about Q3*
```

---
## \#135 Posted by: moon Posted at: 2019-04-28T01:01:30.887Z Reads: 90

```
What happened to q3
```

---
## \#136 Posted by: Gamer43 Posted at: 2019-04-28T01:19:08.314Z Reads: 90

```
![image|254x216](upload://oPL1zZWr7szzD5UuzR3d2Xzg3HG.png)
```

---
## \#137 Posted by: Blasto Posted at: 2019-04-28T01:23:43.654Z Reads: 89

```
Good work on the proto & debugging

On your next pcb, get a seringe of paste and hot air the whole thing, it will make it so much easier
```

---
## \#138 Posted by: Gamer43 Posted at: 2019-04-28T01:24:22.886Z Reads: 89

```
Thanks, but

I don't have a hot air station reeeeeeee.
```

---
## \#139 Posted by: AlexBE Posted at: 2019-04-28T01:40:28.372Z Reads: 90

```
SMD reflow is incredibly easy. You can use anything, oven,skillet. Give it a try and you will never go back. Order paste stencils with your boards.
```

---
## \#140 Posted by: b264 Posted at: 2019-04-28T01:43:02.848Z Reads: 90

```
In some circles, if you mention "skillet reflow" you'll get an ass-kicking.
```

---
## \#141 Posted by: AlexBE Posted at: 2019-04-28T01:48:53.675Z Reads: 93

```
If you don't have hot air or a $50 mini oven, a skillet will work fine. An electric skillet at 100C helps with large rework as a preheater also. People can complain about it if they want, doesn't mean it won't work. Also,use leaded paste.
```

---
## \#142 Posted by: Blasto Posted at: 2019-04-28T02:06:16.641Z Reads: 89

```
Next tool on your wish list then. Even before an oven
```

---
## \#143 Posted by: Gamer43 Posted at: 2019-05-03T03:49:26.048Z Reads: 87

```
So, anyone still interested in testing out the two prototypes?

Also, I just checked the dead ESC, Phase B is a short between power rail and ground xD. Must've messed up a solder joint on one of the gate pins when I was reflowing with a heatgun.
```

---
## \#144 Posted by: M.Hboards Posted at: 2019-05-03T04:03:20.631Z Reads: 85

```
Although i am no not able to test it out as it won't fit in my enclosure i do have a friend who would like to test it out on his board he understands how these switches work and has actually made a working prototype before so he could provide you with suggestions on how to improv it if needed for future irritations if your interested.
```

---
## \#145 Posted by: Gamer43 Posted at: 2019-05-03T05:45:24.877Z Reads: 86

```
Is he on this forum? If he's interested in testing the prototype could you ask him to PM me?

If not, I could give you my email.

Also, on the next iteration, I think I only going to use two MOSFETs, three really is overkill. I can't make the design any smaller without removing one of the MOSFETs. I am going to move the connectors to the sides.

EDIT: replaced the MOSFETs on phase B and ESC works again >:).
```

---
## \#146 Posted by: M.Hboards Posted at: 2019-05-03T11:17:03.861Z Reads: 87

```
He is but he's really inactive here. I'll tell him to pm you.
```

---
## \#147 Posted by: Gamer43 Posted at: 2019-05-27T04:37:29.422Z Reads: 84

```
![20190526_213737|243x500](upload://3bR29f09pjXkdrWSSP0P2toevdC.jpeg) 

Properly assembled prototypes.

Testing them tomorrow before shipping them out later this week.
```

---
## \#148 Posted by: Gamer43 Posted at: 2019-05-27T20:36:50.988Z Reads: 82

```
https://youtu.be/L4EUQNVU0-Y

No explosions yay.

3.3mF load capacitance.
```

---
## \#149 Posted by: Gamer43 Posted at: 2019-05-28T01:53:27.521Z Reads: 81

```
Okay, so interesting thing happened.

_The 47 ohm resistors blew up_ (failed open circuit).

Replaced them and works fine again.

Not sure how TWO resistors both fail open circuit.
```

---
## \#150 Posted by: Blasto Posted at: 2019-05-28T04:46:04.166Z Reads: 79

```
What’s their package? 0805 1/4W?
```

---
## \#151 Posted by: Gamer43 Posted at: 2019-05-28T04:46:32.131Z Reads: 83

```
1206, they're big.

Maybe I should go for 2W 2512 resistors?
```

---
## \#152 Posted by: Blasto Posted at: 2019-05-28T04:47:38.080Z Reads: 84

```
Honestly they should be able to take the impulse, check the impulse rating of that specific part
```

---
## \#153 Posted by: Gamer43 Posted at: 2019-05-28T04:48:15.413Z Reads: 87

```
42V with a 3.3mF load capacitance, I'll check the part's specs and the redo the math to see what kind of power dissipation they're seeing.
```

---
## \#154 Posted by: Gamer43 Posted at: 2019-05-28T05:10:11.308Z Reads: 86

```
So the part number is: RMCF1206JT47R0

So, the resistors see 2.2J of energy split between the two of them over a period of 200ms.

They are indeed 1/4W. I don't think I'm reading the datasheet correctly though, can't seem to find an overload power rating, but from what I can see, it should be able to handle overload power for a couple of seconds. Says it can handle 2.5x working voltage for 5s, which means it should certainly survive the turn-on event. 

I cycled the new resistors many more times than the old ones and didn't have a problem.
```

---
## \#155 Posted by: AlexBE Posted at: 2019-05-28T23:37:55.897Z Reads: 78

```
Have you built a rig to power and then drain the caps? I would definitely set something up to test the switch a few thousand times at least. My approach to this kind of testing is always to try and make it fail.
```

---
## \#156 Posted by: Gamer43 Posted at: 2019-06-02T03:51:20.357Z Reads: 69

```
Okay, I have no goddamn clue why this is happening, but after leaving the switch to sit in my garage for a few days, UNPLUGGED from the battery, the 47 ohm resistors again BOTH became high impedance.

Is there something wrong with my design or did I receive defective resistors?!
```

---
## \#157 Posted by: deltazeta Posted at: 2019-06-02T07:51:52.757Z Reads: 70

```
Honestly lgtm, I'm reaching the same conclusion as you on the resistor's power ratings, should be fine. Maybe you need to cover that sucker in probes and see what's happening. Then again, maybe it was a bad batch of resistors?
```

---
## \#158 Posted by: Gamer43 Posted at: 2019-06-02T08:11:40.073Z Reads: 75

```
I give up.

Design now calls for high power through-hole resistors. Initial prototype never had a problem with them, even though those resistors were not specifically high power.

This design was meant to be easy to DiY on protoboard or on a cheap PCB. It is not suited to be put into production.

Heck, I used the IPP029N06N on the initial prototype.

On my existing prototypes, I'm going to put in 100ohm through hole resistors. Test them a bit, and if they don't have problems, ship them out the the person who agreed to field test them for me. 

After that. I'm going to be done with the design. Others are free to redesign the PCB or do fab runs of them if they like. I can't figure out how to make it smaller without my OCD bugging the hell out of me.
```

---
## \#159 Posted by: Elitejarcool Posted at: 2019-06-02T15:19:42.036Z Reads: 74

```
hey sorry very new to this thread have a lot to learn, 
- why dont you have any by pass capacitors in the circuit or are they not required?
- why are you using 2x 47ohm resistor for NO cucorit from what  l just mathed that will still allow 1.75a of current at 42v
- why didnt you just take a very good current desgin and rework the pcb desgin to make an antispark and do a copy or are there issue with that.
- also would love to get my hand on one of the e switches for testing and help out with this desgin and developemnt proccess, l have a rework station (hot air and solder)

and lam currently in the thought of want to sell anti sparks online an thought current pricing is crazy so lam either going to from a good free desgin or just 1 for 1 coyp a good one ucrrently on the market and get it made
```

---
## \#160 Posted by: Gamer43 Posted at: 2019-06-02T20:06:50.397Z Reads: 69

```
Doesn't need bypass capacitors, in fact bypass capacitors may actually introduce ringing into the circuit.

The two 47ohm resistors were arbitrary, they are now going to be two 100 ohm through-hole (power) resistors.

No current design works in this way and the ones that work are expensive.
```

---
## \#161 Posted by: AlexBE Posted at: 2019-06-02T23:02:40.531Z Reads: 64

```
Hmm yep certainly in my simulation, those resistors take a huge current spike (120W) which will certainly kill them.
```

---
## \#162 Posted by: Gamer43 Posted at: 2019-06-03T01:43:48.913Z Reads: 64

```
You'd think they die during turn-on, but no, they died when the switch wasn't plugged into anything,
```

---
## \#163 Posted by: deltazeta Posted at: 2019-06-03T02:17:29.239Z Reads: 64

```
Thick film resistors can take a decent impulse especially with the relatively low time period.
```

---
## \#164 Posted by: AlexBE Posted at: 2019-06-03T07:08:44.570Z Reads: 64

```
I strongly disagree. @Gamer43, I don't have data for your specific part, but to compare. You have 2 x 1206 1/4W resistors. In my simulation (4000uF cap) there is a pulse above 100W for >10ms. Vishay's datasheet for their 1206 1/4W resistor has a maximum pulse time at 100W of 1us. So I think you are a factor of ~10000 outside the spec of a similar resistor.

As to when they died, if you pulse a resistor like that, yes it's most likely to crack immediately, but I'm not surprised that it died at some later time. Ie from impact or thermal cracking as it cooled down.
```

---
## \#165 Posted by: Gamer43 Posted at: 2019-06-03T07:21:41.446Z Reads: 63

```
Whelp, lets see if a pair of 5W wirewound through-hole 100ohm resistors can fair any better. At fully charged 12s they see an instantaneous power of 25W each. Metal should be less susceptible to thermal cracking as it is flexible and the cermaic core might be able to absorb some of the energy. The datasheet says they can handle 12.5W for 5 seconds with 2% resistance deviation, and a surge voltage of 8kV for 50uS.

This is the part number: EP5WS100RJ

The initial prototype used standard 1/2W 100 ohm through-hole resistors and never had a problem. It was cycled several times with 6mF capacitance. It still works now.
```

---
## \#166 Posted by: AlexBE Posted at: 2019-06-03T07:37:11.677Z Reads: 66

```
Unfortunately I think you have to rethink this approach. The energy in the caps is very large, maybe you need to add an inductor in series with the resistors to limit that peak current. I haven't seen a datasheet for a power cap that I would be confident in using in this safety critical circuit.
```

---
## \#167 Posted by: b264 Posted at: 2019-06-03T07:38:42.127Z Reads: 63

```
Now it's really not hard to imagine why all the inrush limiters are dying when all that power is being dissipated in the FET junction itself instead of a separate resistor :rofl:
```

---
## \#168 Posted by: Gamer43 Posted at: 2019-06-03T07:44:25.004Z Reads: 65

```
AC05000002000JAC00

Maybe four of these may work better instead? Or will resistors ultimately fail if repeatedly subject to short time overload?
```

---
## \#169 Posted by: b264 Posted at: 2019-06-03T07:45:57.921Z Reads: 65

```
I wonder how a wirewound inductor would fare?
```

---
## \#170 Posted by: Gamer43 Posted at: 2019-06-03T07:49:19.269Z Reads: 67

```
Bad idea, it would form an LRC circuit with the load capacitance and ring really bad. If the load capacitance were known and fixed, the inductance and resistance could be selected to create a critically damped transient response. But for this kind of switch, the capacitance is highly variable and there's no way to design around it.

Underdamping would cause ringing and wreak havoc with the ESC, overdamping would cause the primary MOSFETs to never turn on (or take a really long time to turn on)
```

---
## \#171 Posted by: deltazeta Posted at: 2019-06-03T08:11:04.919Z Reads: 67

```
That's good info, all I have going for me is stack overflow. How do you interpret overload ratings then? A random 1206 47ohm on mouser had a 1.5x voltage overload for several seconds or so. With the nominal rating at 200V, I can't imagine the rating assumes there's a voltage across the resistor with no current.
```

---
## \#172 Posted by: AlexBE Posted at: 2019-06-03T08:34:23.572Z Reads: 68

```
Have a look for the vishay resistor datasheets on Digikey, look at the power vs time graphs.
```

---
## \#173 Posted by: deucesdown Posted at: 2019-06-03T16:10:49.628Z Reads: 64

```
Is this relevant?

https://endless-sphere.com/forums/viewtopic.php?f=14&t=54138&start=25#p951858

TL;DR is experiments with XT90S and AS150 and some other antispark connector with an NTC resistor, at 100v and 4000uF.

Hm maybe all my XT90S loopkeys are burned out lol.
```

---
## \#174 Posted by: deltazeta Posted at: 2019-06-03T16:28:00.543Z Reads: 65

```
yeah that's really strange, not sure how to reconcile those two ratings. Maybe the Panasonic one is just better than the Vishay one :thinking:
```

---
## \#175 Posted by: AlexBE Posted at: 2019-06-05T01:19:01.942Z Reads: 61

```
You are misunderstanding the voltage ratings. Obviously a 47 ohm resistor cannot handle 200V across it as that would be 800W. My guess is that you are looking at the datasheet for the entire resistor series, ie the datasheet for all resistor values in that series. It might even be a datasheet for multiple package sizes. I have never seen a detailed datasheet for a single resistor value/size.
```

---
## \#176 Posted by: deltazeta Posted at: 2019-06-05T03:25:33.136Z Reads: 59

```
Ah I see what you're saying, found the fine text in the spec sheet about that. Continuous working voltage ends up at 3.5V lmao.
```

---
## \#177 Posted by: Gamer43 Posted at: 2019-06-09T18:50:03.773Z Reads: 55

```
![15601062600582403300588342419289|243x500](upload://nokAJTaIOWhgYVbeEVb8m2SpALN.jpeg) 

When you're too big to fail...
```

---
## \#178 Posted by: AlexBE Posted at: 2019-06-20T05:31:24.982Z Reads: 51

```
In reference to this and your previous post about TH resistors previously working flawlessly -> My guess is that the inductance of these wirewound resistors is what is limiting their peak power and allowing them to survive.
```

---
## \#179 Posted by: Gamer43 Posted at: 2019-06-20T06:20:57.584Z Reads: 52

```
I would think that their parasitic inductance would only be on orders of a few hundred nanohenries, which wouldn't have much of an effect on these timescales.

The currents involved are actually not that much, about 1A or even less, so I'm thinking that the construction of wirewound through-hole resistors just makes them inherently more rugged to repeated short-term overload conditions.

But, it works regardless, and that's all that matters :). So this design will call for through-hole resistors, preferably power resistors, as a requirement.
```

---
## \#180 Posted by: AlexBE Posted at: 2019-06-21T05:20:19.308Z Reads: 46

```
I can't remember which resistors you initially tried , I have a similar inrush limiting problem in my current work. I have a 2612 resistor from Bourns CRM2512 that can handle 200W for 1ms. It does the job in my application controlling inrush to large capacitor banks. I might also add a NTC or PTC to further soften the blow.
```

---
