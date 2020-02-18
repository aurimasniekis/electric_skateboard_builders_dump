# VESC cap board questions

### Replies: 19 Views: 1259

## \#1 Posted by: evoheyax Posted at: 2016-09-05T22:08:23.010Z Reads: 88

```
So two questions maybe someone more knowledgeable could answer?

How many capacitors do I need for 4 vescs?

Do the caps need to within a certain distance to the vescs?

@chaka @JTAG @onloop
```

---
## \#2 Posted by: torqueboards Posted at: 2016-09-05T22:12:05.117Z Reads: 87

```
You can have the 3x total for all 4. It just adds to the amount of space it takes up. More is better and having more isn't a bad thing besides the space issue. The distance from your ESC to your batteries you want as short as possible but within our setups it's usually not that long.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-09-05T22:19:24.401Z Reads: 80

```
@torqueboards Coulda bad cap blow a power switch? I blew 2 of your power switches before and one of @JdogAwesome's just now  in the same setup. Everything was cleanly soldered and heat shrink. No sound of shorting can be heard. It just turns on some time after soldering it up and doesn't want to turn off.
```

---
## \#4 Posted by: JdogAwesome Posted at: 2016-09-05T22:31:59.190Z Reads: 78

```
@evoheyax I think the problem could potentially be that with your 4 VESC's they have a total capacitance of 6720uF if you are using the standard VESC cap setup with 3x 560uF. And that large of a capacitor array on initial startup could draw a LOT of current, potentially more than the peak current in the switch. Now im not 100% sure about this though I think it might be the only viable possibility of the problem. Im going to do some more research and try to figure out the exactish current draw on startup and see if that could be causing the problem. Cause if it was a short it just wouldn't work in the first place, though I also dont know why it would work a couple times then die out.
```

---
## \#5 Posted by: torqueboards Posted at: 2016-09-05T22:37:40.178Z Reads: 72

```
You just have to connect it properly. Any voltage dump on anything can easily fry an ESC, RC Receiver, UBEC, Power Switch.

I'd connect the power switch to the ESC, make sure the power switch is off and plug into the battery. If your turning the power switch on and off. I'd wait 2-4 secs to turn it on again. I wouldn't keep turning it on/off fast.

You should be fine. I've used these switches forever. Occasionally, one will pop or so but that's a very unlikely occurrence. I've had the same switch on boards for years without any issues.
```

---
## \#6 Posted by: evoheyax Posted at: 2016-09-05T22:44:16.234Z Reads: 67

```
Thank you, I think something weird is happening. I've traced wire, looking for any cuts. Everything's clean. I used to suck a soldering, but I have learned to solder very quick, good joints. And I heat shrink everything, sometime I even double up If i feel like the heat shrink wasn't enough insulation with electrical tape.

It's weird cause it does this turn it self on and never turn off by itself. I don't turn it on and it gets stuck. It turns it self on, when I'm moving wires around and tucking it in.

I tried it with a 12v regulated power supply and it's fried... no doubt about it.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-09-05T22:48:25.727Z Reads: 58

```
@torqueboards How could I be connecting it wrong? It works fine for a few minutes before they randomly decide to turn themselves on and never turn off again... I don't turn it off and on real quick, I do give it a few seconds in between. The fets inside the switch look fine, there's no a mark or anything out of place looking...
```

---
## \#8 Posted by: torqueboards Posted at: 2016-09-05T22:54:12.136Z Reads: 61

```
@evoheyax - Yeah, not too sure. Sounds quite odd. Considering I have some switches I use for testing that have been turned on/off well over 800+ times on a 10S (2x5S) setup. I'm working on a better on/off switch though that will be better with higher quality parts. Will keep you in mind once I get those tested.
```

---
## \#9 Posted by: JdogAwesome Posted at: 2016-09-05T23:12:10.083Z Reads: 58

```
[s]@torqueboards have you ever had anybody use your switch in a 4 wheel drive setup before? Or at least used one in a board that has had more than 2 VESC's? Because right now using [THIS](http://planetcalc.com/1980/) calculator at 42V and a resistor value of 0.01Ohms (Using 0.01 to simulate internal resistance of a newish LiPo) and a capacitor value of 6720uF and a charging time of 5 milliseconds (Charging time doesn't matter in this case) the initial current is 4,200 Amps which is FAR above the peak current of the 2 IRFB7530 FET's. I do believe this is whats causing the drain-source short in the MOSFET's. I could be wrong though its seems like this is most likely it.[/s]

I was about to post this but then I thought I may as well try these calculations out at a lower capacitance, like if you had two VESC's, and im getting the same peak current, 4200 Amps. Only variable chat changes the peak current is the resistance value. I do still think that the large capacitance is causing the problem due to the higher initial amperage for a longer duration because there are more capacitors, though im not sure of the proper equation to calculate this yet. Im going to do some more research on this and ill get back to you all when I find something.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-09-05T23:20:56.621Z Reads: 54

```
Thank you. Something weird is defiantly happening here. I've gone over everything multiple times, checked every cable. I hear no noise when it turns itself on, and I see no possible place for a short circuit to occur I even checked every pin on every port on every vesc).

The other thing to keep in mind is the distance between vescs is about a foot and a half.

If I use 5mm bullets, I have no issues. I have ridden the board almost 200 miles and there's no issues. The only time an issue pops up is when trying to use a power switch...
```

---
## \#11 Posted by: racidon Posted at: 2016-09-05T23:25:14.592Z Reads: 45

```
[quote="JdogAwesome, post:4, topic:9004, full:true"]
@evoheyax I think the problem could potentially be that with your 4 VESC's they have a total capacitance of 6720uF if you are using the standard VESC cap setup with 3x 560uF. And that large of a capacitor array on initial startup could draw a LOT of current, potentially more than the peak current in the switch. Now im not 100% sure about this though I think it might be the only viable possibility of the problem. Im going to do some more research and try to figure out the exactish current draw on startup and see if that could be causing the problem. Cause if it was a short it just wouldn't work in the first place, though I also dont know why it would work a couple times then die out.
[/quote]

@evoheyax I would go with what Jdog said mate. Try using 2 switches. 1 for 2 VESCs each 
<img src="/uploads/db1493/original/2X/f/ff5ec8124ea5e37445e53e8f4d588dc195f5ad99.png" width="485" height="320">
```

---
## \#12 Posted by: JdogAwesome Posted at: 2016-09-05T23:28:23.475Z Reads: 44

```
Yeah you wouldnt hear or see anything when the MOSFET's die if its a transient drain to source short because it peaks current so fast that theres no time for anything to heat up. Im still doing some research though I believe thats the problem. I would recommend that you remove half the capacitors from your system and im guessing that would fix your problem. If you have the VESC's in two separate "bundles" then I would remove all 3 from one VESC and all three from the other "bundle" of VESC and just having them share the 3 caps.

@racidon yeah you could use two switches though I think it would make more sense to just remove half the caps like I stated above,
```

---
## \#13 Posted by: JdogAwesome Posted at: 2016-09-06T00:32:33.723Z Reads: 38

```
Alright so I believe figured out the proper equation for figuring out the inrush current for charging the capacitors. Equation is as follows, **I=Vb/R e− t/RC** "Where Vb is the source voltage, R is resistance, t is time and RC is the time constant (product of resistance and capacitance)." Got this off of Stack Exchange [HERE](http://electronics.stackexchange.com/questions/80561/how-much-current-does-a-capacitor-draw-when-charging). For my calculation I did [C = 42/0.015 e−0/0.01411](https://www.wolframalpha.com/input/?i=C+%3D+42%2F0.015+e%E2%88%920%2F0.01411) where 42 is the voltage, 0.015 is the internal resistance of the LiPo, e is Euler’s constant ( ≈ 2.718281828) and 0.01411 is the time constant. Anyways in that equation **C = 7611.19 Amps** which is crazy high lol. And it will take (5⋅0.01411=0.07055s) 0.07055 seconds to charge the capacitors fully. So yeah im pretty sure that its the large capacitance thats causing the problem because it draws a ton of current for almost a tenth of a second. If you were to have only 2 VESC's and have a total capacitance of 3360uF you would be drawing the same amount of current, but for only 0.0353 seconds. Now im pretty sure my calculations are correct, but dont quote me on this. [Wolfram](https://www.wolframalpha.com) helped a lot with the main calculation and is a really cool site, I highly recommend you check them out. [Time Constant Calculator](http://www.digikey.com/en/resources/conversion-calculators/conversion-calculator-time-constant)

EDIT: Im again kinda confused because in the equation **C = 42/0.015 e−0/0.01411**, 0.015 is the internal resitance (IR) of the LiPo and this changes a LOT with the usage of the battery as well as how many cells you have. For example in @evoheyax build he has a 10S LiPo and if they've been fairly used then they may have an IR of around ~7 Miliohms. 7x10S=70 which means that IR then equals 0.070 instead of 0.015 in the equation. Though if I run the equation now, C = 1630.97 Amps. Now 1630 Amps is still a lot of amperage and could still cause this to happen, so it could still be the case. [HERE](http://www.helifreak.com/showthread.php?t=233111) is a forum post about battery IR ratings where I got my numbers from.
```

---
## \#14 Posted by: evoheyax Posted at: 2016-09-06T00:42:00.596Z Reads: 34

```
So what's the solution? I need a switch ASAP that will work, as I need to be ridding by wenesday again. I'll probably put my plugs ok the outside, as I'm tired of opening it every day I get to class.
```

---
## \#15 Posted by: JdogAwesome Posted at: 2016-09-06T00:54:04.789Z Reads: 34

```
Well I believe the solution is to remove half your capacitors like I stated and try again. Now I dont know if this will fix the problem, it should though. I was reading that large inrush current over time will damage MOSFET's so that may be why it works a couple times and then drain-to-source shorts. Another option would be to have a circuit kind of like a XT60 loop key but the ones with a resistor to charge the caps first then power the MOSFET's to let the bulk current flow through. I really have no idea how exactly you would go about doing this except for having an extra momentary push button to charge the capacitors then the main push button for the MOSFET's. You could in theory have a circuit that when triggered lets current flow through a resistor for a certain amount of time and then turns on the MOSFET's though I think it would be much simpler to reduce your capacitance or use a momentary push button with a resistor.
```

---
## \#16 Posted by: evoheyax Posted at: 2016-09-06T00:59:18.679Z Reads: 33

```
What kind of effect would it have to run with half the caps?
```

---
## \#17 Posted by: JdogAwesome Posted at: 2016-09-06T01:02:10.490Z Reads: 34

```
Well it shouldn't have any "affect" on performance per say except for not kiling MOSFET's lol.

EDIT: It definitely shouldn't have any effect on performance because you said that your battery's are only a foot and a half away from your VESC's and the caps are there for longer runs of cable mainly.
```

---
## \#18 Posted by: evoheyax Posted at: 2016-09-06T01:06:49.412Z Reads: 31

```
Do you min if I fix it myself? I might just blow some more out and I can't afford to keep waiting with shipping back and forth. I wouldn't mind buying parts. I just don't know what I need to replace. This board looks incredibly simple to me. So replacing parts won't be a problem, I just need to know what to replcae
```

---
## \#19 Posted by: JdogAwesome Posted at: 2016-09-06T01:12:29.220Z Reads: 33

```
[quote="evoheyax, post:18, topic:9004"]
This board looks incredibly simple to me.
[/quote]

OHH IT DOES NOW HUH

Lol, anyways yeah you can fix it yourself, all you need to do is replace the two MOSFET's on the board by removing the solder on the bolts on the back and unscrewing them. Then desoldering the legs of the MOSFET's and removing them. Then just putting new ones in and and re soldering and bolting them in place. I ordered my FET's off of Mouser though it makes a lot more sens to order them in bulk like I did instead of just buying one or two. I could send them to you cause they weigh like nothing so shipping would be pretty cheap.
```

---
