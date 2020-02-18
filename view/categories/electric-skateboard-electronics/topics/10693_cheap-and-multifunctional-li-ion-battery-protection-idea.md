# Cheap and multifunctional Li-Ion battery protection idea

### Replies: 30 Views: 2509

## \#1 Posted by: IDVert3X Posted at: 2016-10-05T20:02:54.751Z Reads: 192

```
This project was discontinued.
The idea was to use relay for switching the power instead of transistors to get rid of heat.
Also, I wanted it to be more than just a BMS, like main power board & monitoring board.

Latest schematic:

[img]http://www.electric-skateboard.builders/uploads/db1493/original/3X/8/0/8076325a25d6f212fafed7945c1a5904085ac31e.jpg[/img]

---

Original message:

> Hi, I was thinging how could I improve the way people protect their batteries.
> Currently, most of us use some kind of **BMS**, but not all the functionality is acctualy needed.
> If we use 25R cells for example, they are so good quality that they don't have to be balanced.
> So the only thing we need then is **overcharge**, **over-discharge** and **short circuit** protection.
> Then I thought... What is the most effective way? Like something that won't produce any heat.
> Do you remember those old mechanical switches called **relays**? Yes, they're still used.
> They can switch hundreds of ams without producing any heat!
> Well, they produce some heat, but negligibly amount. Compared to mosfets it's amazing!
> This can be used as anti-spark switch as well, but about this later.
> So, the next thing I need to do is to measure the actual voltage of the pack.
> Yeah, I could use some parts made for this.. BUT: why not to use **microcontroller**?
> ATTiny are great for that. They have built-in **ADC**, so you can measure the voltage.
> All we need is a voltage divider ( 2 resistors ) and one ceramic capacitor ( 330nF should be fine ).
> And because the microcontroller itself is controlling the relay, we can connect switch to the microcontroller and voala: we have **anti-spark switch** as well!
> Nice! What's next?
> Well, you can connect a display to the microcontroller ( those 0.97" OLED displays you can buy on ebay are great for that ) and **display the voltage** or the **percents left** based on the voltage to percent chart from datasheet.
> And because we all love to short circuit our stuff, the protection is very important. So let's add a fuse as well.

> So, what this solves?
> * Over-charge protection
> * Over-discharge protection
> * Over-current protection
> * Anti-spark switch
> * Voltage / percentage monitor

> Are there any disadvantages?
> Well, yes - idle current would be higher than on the most of BMSs.

> So.. how much would it cost?
> Shouldn't be expensive, as I can't product SMD at home, I'm working with THT components, main components:
> * cuprextit ( material used to produce PCBs ): up to 0.20 eur
> * input filter cap: 0.05e
> * linear voltage regulator ( should be fine for ~10mA of power ): up to 0.15 eur
> * microcontroller: 1.00 - 1.50 eur
> * relay: 7 eur
> * fuse & fuse socket: 2 eur
> * resistors ( for voltage divider ) : 0.06 eur
> * headers - 0.02 euros
> * display - 3 euros
> If you do the math, you will find out that it will cost at max 10 euros.

> Not that bad as it's small, does a lot and produces virtually no heat.
> I don't have a prototype yet, I'm going to draw a scheme tomorrow and share it with you guys.
> I'm not going to say it's the best way to do it, it just an idea that I'm going to prototype once I have my pack.

> What do you think?
```

---
## \#2 Posted by: oneafrikan Posted at: 2016-10-05T20:06:32.131Z Reads: 167

```
Do it ;-)

10 char
```

---
## \#3 Posted by: IDVert3X Posted at: 2016-10-05T20:13:47.742Z Reads: 170

```
I'm going to do it once I have my battery pack ( planning on 10S4P ) but that's probably going to be next year.
That's why I wanted to share this idea. This design can be improved even more tho.
If you really wanted to, you could program it to communicate with VESC and get more data, for example current.
I will draw the schematic tomorrow ( no promises! ), probably with a few more components that are not neccesery, but it's better to have them ( like diode and pullup on reset pin of the microcontroller and so on ).
Will update you once I have somthing.
```

---
## \#4 Posted by: H3rose Posted at: 2016-10-05T20:21:11.558Z Reads: 154

```
This sounds like an awesome concept. Ive been researching li ion batteries and while im still not that well versed on the technology I know some things. Like how li ion batteries like 18650s dont require balance charging like lipos do. However, i havent been able to find any other solutions that were cost effective. So you my friend are amazing. 😉
```

---
## \#5 Posted by: IDVert3X Posted at: 2016-10-06T06:28:56.259Z Reads: 127

```
While designing the circuit, I came up with multiple issues I need to solve, but it's definitely possible, just need few more components. Working on it now!
```

---
## \#6 Posted by: TarzanHBK Posted at: 2016-10-06T08:20:19.397Z Reads: 118

```
sounds good! i like when people go creative and overthink something again to maybe produce something better :slight_smile:
```

---
## \#7 Posted by: IDVert3X Posted at: 2016-10-06T16:42:03.855Z Reads: 109

```
Hi, good news!
Today I drown most of the schematic. I havn't had enough time to calculate all the resistor and capacitor values tho.
But at least something to show, hopefuly I will be able to finish the schematic tomorrow with all the values and details.

Basic explanation:
Top left: battery input, it's fused for 80A continous, 150A pulse.
Top right: 5V buck converter for microcontroller, display, relay control etc.
Left: relay itself controlled by microcontroller
Bottom left: voltage divider ( so I can measure high voltage using ADC in MCU ), accuracy ~0.05V
Absolute bottom left: output for ESC / other cool stuff & input for charger
Center: microcontroller and AVR ISP header ( for uploading newest firmware )
Right: connector for OLED display, button to switch between displaying voltage/perctentage, antispark switch and status LED ( for example it can blink when you try switch power on but the battery is too low ).

Finally, the schematic: <img src="/uploads/db1493/original/3X/4/7/473df3c2df7d5b5fbbc7515ccd509e07e1763151.jpg" width="666" height="500">
```

---
## \#8 Posted by: fuelre Posted at: 2016-10-06T19:32:53.431Z Reads: 99

```
thats not bad input, just a few thougths that hopefully helps you:

a relais is nothing else than a simple XT60 Plug - it generates a spark inside the case. -> huge inrush currents to the ESC
please show me a relais that is capable of 50A (burst, but contious would be better) -> are you capable to drive such a relais with a attiny pin? (dont forget the flyback diode)
heat in the LM2576?
cap. for µC VCC

for the development - a reset button and some outputLEDs for debuging!

AND last, but not least - I realy like your paper style work!
```

---
## \#9 Posted by: smurf Posted at: 2016-10-06T19:42:11.137Z Reads: 95

```
Mechanical relays don't handle vibration as well as solid state relays
```

---
## \#10 Posted by: IDVert3X Posted at: 2016-10-06T19:45:35.754Z Reads: 99

```
@fuelre 
Good quality relay won't spark much on DC current ( will be different on AC inductive load of course ).
There are few ones made especially as "non-spark" ones which are capable of handling 100A ( crazy )!
Show you 50A relay? Google it or take a look at some catalogues, for example: http://tme.eu/
Relay needs only about 10mA-15mA of power, you can drive it with digital pin of attiny ( capable of 20mA ).
In the worst case, I can still add mosfet to drive the relay, but I don't think it's really necessary.
Heat in LM2576? Dude, it's buck converter, not linear regulator!
About the cap, you are right. I'm thinking of adding 300nF ceramic cap on the VCC of the attiny.

About the paper style - thanks :D I prefer it over Eagle because I can just draw and I don't have to think about all the libraries for all the components and so on... Once I'm done, I usally redraw it to the Eagle so I can design the PCB.

@smurf
Good point. I havn't though of this, will look more deepely into it.
```

---
## \#11 Posted by: SORRENTINO Posted at: 2016-10-06T19:50:26.763Z Reads: 93

```
Wouldn't Internal resistance in the cells change over time and hence why you would need to always balance. All it takes is a couple cells to be worse then the others and you end up over charging the rest and undercharging the bad ones. then when you're riding those under charged cells would go well under the normal discharge voltage. Ive seen this in happen to lipos. People end up catching there house on fire this way :) Maybe im wrong when it comes yo Li-Ion but I think its foolish not to balance charge imo.
```

---
## \#12 Posted by: IDVert3X Posted at: 2016-10-06T19:52:34.775Z Reads: 88

```
Only LiPos have this problem...
Quality Li-ion cells don't have to be balanced at all.
```

---
## \#13 Posted by: SORRENTINO Posted at: 2016-10-06T19:57:10.297Z Reads: 85

```
Quality Li-ion cells have uniform capacity and low self-discharge when new. Adding cell balancing is beneficial especially as the pack ages and the performance of each cell decreases at its own pace. A problem arises when a cell in a string loses capacity or develops elevated self-discharge. This can be attributed to high-temperature spots in a large battery. Low-quality cells may also be prone to unequal aging. Li-phosphate has higher self-discharge that other Li-ion, and this complicates cell balancing. (See BU-802b: What does Elevated Self-discharge do?)

A battery expert once said: “I have not seen a cell balancing circuit that works.” For multi-cell packs, he suggested using quality Li-ion cells that have been factory-sorted on capacity and voltage. This works well for Li-ion packs up to 24V; **packs above 24V should have balancing**. Most balancing is passive; active balancing is complex and is only used in very large systems.

http://batteryuniversity.com/learn/article/bu_803a_cell_mismatch_balancing
```

---
## \#14 Posted by: Jinra Posted at: 2016-10-06T19:59:02.770Z Reads: 79

```
don't be misinformed. 18650's should be balanced as well as lipos
```

---
## \#15 Posted by: Hummie Posted at: 2016-10-06T20:01:21.547Z Reads: 87

```
thats all i want is balancing.  the vesc has the low cut off and a max amp limit already and I use an xt90s.  how hard would it be to make a simple 12s balancer?  not a charger but more of a battery medic that did 12s instead of 6s and did it quicker.  I imagine it'd be a pretty simple circuit.  need not have a screen just a light maybe when all the cells hit the lowest.  how bout that @IDVert3X ?
```

---
## \#16 Posted by: IDVert3X Posted at: 2016-10-06T20:14:43.640Z Reads: 88

```
Yes, I could do that. But the actual reasons why I'm making this:
- something needs to stop the charging when the pack is fully charged
- fuses! Because there are only two types of people: those, who use them and those, who will.
- I want a small display that will show me the voltage / percentage ( it's like 3 euros so why not? )

I don't need over discharge protection, like you said, VESC handles this nicely, but... It's just a thing of adding few more lines of code to the firmware, the same goes for the display.

I'm making this just because all those 80A BMSs are really expensive and have functionality I don't need.

Also, I'm not going to make balance charger, it's not worth it for me. And it's not that simple as well tbh.

Btw, I just disassembled my old project where I use 8S DIY Li-Ion pack. 
I has been recharged every day for almost a year now without any balancing.
I have measured the voltages on the cells: 3.974, 3.969. 3.971, 3.979, 3.975, 3.968, 3.969, 3.976

BTW, you are not fully balancing your packs either. For example: 10S4P. Do you think it really balances all those 40 cells individually? No, it does not. It balances them as groups of 4 in parallel.

I'm not going to say balance charing is bad. It's great and necessary for the LiPos, but for quality Li-Ion pack I can live without it.
```

---
## \#17 Posted by: fuelre Posted at: 2016-10-06T20:17:33.819Z Reads: 84

```
there is a reason why the LM2576 has this package, but yes, maybe its my fault
Yes - there are relais for high currents - but they are big, and than they need way more current/voltage for switching
the current isnt the problem - the voltage is the problem!
tme is a nice example -> i searched only by max DC Current/ DC Voltage (at least 48V and 50Amps)
<img src="/uploads/db1493/original/3X/a/1/a104c8947c6d58c8092a4a4f41232a00b69d67b1.png" width="164" height="195">
only 17 relais are left, and they are at least 77€.

please show me a link from your 7€ relais, that would be realy nice!
```

---
## \#18 Posted by: Hummie Posted at: 2016-10-06T20:26:37.687Z Reads: 77

```
yea I know when balancing it wont do the cells that are in parallel but I think them being in parallel keeps them balanced.  if you can make a 12s balancer, or show a schematic of how to do it, I'd do it.  

all the bulk chargers I've had, even the cheapest, have a high cut-off.  It seems unneeded.
```

---
## \#19 Posted by: IDVert3X Posted at: 2016-10-06T20:33:25.913Z Reads: 80

```
@fuelre 
Car relays are good for that, you will definitely be able to find some for 7 euros.
I can't send you a link as I was asking in my local store few days ago and they offered me 100A 60V relay, but it was quite huge so I havn't aksed anything more, just said no, thanks thinking I can find something better.
But like you mentioned, most of them are more than 5V ( 7-15V ).
Current & voltage for the relay could be fixed using a mosfet like I already said, not ideal tho.

@Hummie
That fact that they are beign parallel doesn't means they will balance equally.
About the shcematic: I'm sorry, but I don't have any already created and I don't have time to design it.
You should be able to find something on Google.
I don't use "chargers", I use power supplies and they don't have cutoff so I PERSONALLY need it, it can be different for you of course if you use charger that has this function built-in.

Anyway, thanks to everyone for the feedback and recommendations. Really appreciate it!
```

---
## \#20 Posted by: Hummie Posted at: 2016-10-06T20:36:01.181Z Reads: 78

```
all my bulk power supplies charge to a specified voltage and then cut off.

i thought the parallel cells have to balance because they were parallel.  all cells in parallel will be the same voltage.
```

---
## \#21 Posted by: fuelre Posted at: 2016-10-06T20:38:45.991Z Reads: 70

```
too bad - would be realy nice to have such a relais.
car relais are just for 12V systems - not 48V systems (i dont like it to use stuff outside there tolerances)

but hey - plese finish your project and give us some feedback!
```

---
## \#22 Posted by: IDVert3X Posted at: 2016-10-06T20:41:00.988Z Reads: 76

```
@Hummie 

You probably don't use something like this:

<img src="/uploads/db1493/original/3X/0/6/06ec4ecdeb972b72cadb7b5c7172de666a30bdff.png" width="500" height="500">

Even the cells in parallel can have slighly different capacity so they may not discharge/charge equally.
But the truth is that they will - because they are all almost the same capacity.

@fuelre

In the datasheet for the car relay: Switched voltage	max 75V DC 
Doesn't that means it's capable of switching 75V?
```

---
## \#23 Posted by: fuelre Posted at: 2016-10-06T20:42:45.954Z Reads: 69

```
nice - i didnt know that
```

---
## \#24 Posted by: IDVert3X Posted at: 2016-10-06T20:46:43.611Z Reads: 67

```
Yeah, but it's still made for 12V even it can handle 75V. The question is lifespan.

Off topic: it's late there in central Europe ( 22:45 ). I'm going to sleep, I have to wake up early, will reply tomorrow.
```

---
## \#25 Posted by: Hummie Posted at: 2016-10-06T20:49:00.945Z Reads: 65

```
i have a charger just like that from meanwell.  the little screwdriver slot is the same in the picture and it adjusts the voltage.
i think parallel cells may not have the same capacity but a low capacity cell in parallel will hit the high voltage faster ..the whole paralllel pack will have less capacity but no cell will individually go above or below the pack as a whole and it's safe that wasy
```

---
## \#26 Posted by: H3rose Posted at: 2016-10-07T02:24:30.258Z Reads: 54

```
[quote="IDVert3X, post:16, topic:10693"]
I don't need over discharge protection, like you said, VESC handles this nicely, but... It's just a thing of adding few more lines of code to the firmware, the same goes for the display
[/quote]

Please add this. I dont plan on using a vesc.
```

---
## \#27 Posted by: IDVert3X Posted at: 2016-10-07T05:29:51.244Z Reads: 47

```
I definitely will :)
```

---
## \#28 Posted by: IDVert3X Posted at: 2016-10-08T12:42:39.398Z Reads: 43

```
I have improved the design ( thanks to everyone for your feedback ), noticable changes:
* added 12V rail, used for switching the relay, but can also be used as a power supply for your LED strips or other lights / devices that require 12V to operate ( max. 3A ).
* added MOSFET which will handle switching the relay ( 5V pin of the uC goes to the gate ).
* added MOSFET which will switch the 12V rail ON or OFF ( only need 5V for uC when device is off )
* added flyback diode ( thanks @fuelre ).

Will draw the new schematic for you once I have enough time to do so.
Believe it or not, hand-drawing the schematic can take quite a long time if you want it to look nice.
```

---
## \#29 Posted by: IDVert3X Posted at: 2016-10-09T12:28:17.427Z Reads: 40

```
Hi, bad news.
As I have changed my mind and I will go with LiPo for my project, this project is now discontinued.
But for you, who were interested, I drew the last schematic:

<img src="/uploads/db1493/original/3X/8/0/8076325a25d6f212fafed7945c1a5904085ac31e.jpg" width="499" height="500">

Current design is capable of handling up to 50V ( 12S ). Actually, the regulators can handle up to 60V as well as relay can, but the voltage divider is 10:1, so that would result into 6V on the ADC pin of the ATTiny and that's not good. However, if you want, you can use different ratio on the voltage divider and increse the limit to 60V max. 

Also, there is an 12V 2.5A output which is only active only when the output is switched on, you can use this for your lights or anything that requires 12V.

5V rail is always active as it powers the microcontroller which is in standby mode until it receives the signal from the power switch which will wake it up, it will switch on the display ( in SW ), enable 12V rail and switch on the relay.

There is also a small push button that can be used to switch between different modes  ( voltage / percentage ).
Small 3mm led ( D6 ) can be used as an indicator of something ( errors and so on ).

Firmware can be easily updated using the AVR ISP programming header.

There are probably quite a few things you can do better than I did, so feel free to make any changes to the current design, would be nice if you share it with us, but you don't have to ( MIT license ).
```

---
## \#30 Posted by: anorak234 Posted at: 2019-04-24T00:29:37.405Z Reads: 1

```

```

---
