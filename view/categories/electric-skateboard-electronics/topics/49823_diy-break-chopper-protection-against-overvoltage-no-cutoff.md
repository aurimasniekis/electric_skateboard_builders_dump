# DIY break chopper - protection against overvoltage - no cutoff

### Replies: 57 Views: 2854

## \#1 Posted by: Vanarian Posted at: 2018-03-22T11:54:21.820Z Reads: 297

```
Folks I've found back the break chopper circuit made by Sawyer !! @Sawyer93 is it you by chance ?

Short word it is **the end of HVC cut-off** (like if you coast downhill and want to regen brake while battery is full, well you can still go at it). 

We'd need to replace the halogen bulbs he uses to dry the excessive power by something more discrete IMHO. A big shunt or something similar ? A rack of high power LEDs to give it post-apocalyptic look?

Anybody is able to decipher it better than I do ? @b264 @Deckoz  what do you guys say ? 

http://forum.electricunicycle.org/topic/6508-brake-chopper-to-avoid-over-voltage-condition/

And a video of how it works / what it does (see the gauges in left corner) : 

https://youtu.be/zoTT0M_YPJo
```

---
## \#2 Posted by: ducktaperules Posted at: 2018-03-22T13:14:29.248Z Reads: 269

```
maybe you could wire this to a big break light :)
```

---
## \#3 Posted by: Vanarian Posted at: 2018-03-22T13:25:13.904Z Reads: 262

```
Would be a killer look if the light is mounted on the rear truck for example :smile:
```

---
## \#4 Posted by: Deckoz Posted at: 2018-03-22T14:31:39.463Z Reads: 258

```
![brake-chopper-circuit-300x300|300x300](upload://iHVuVmsxRu6ydagk2mJES3hCmtX.png)

Here's the brake chopper circuit in full simplicity

Just replace the Brake resistor with another resistive load...


And actually they made a microcircuits which is at the end of that video... With the schematic to be able to customize the clamping voltage
![OZ8khhz|690x431](upload://DHudhHvqwbd9yhF7CWfcQjCTyv.jpg)
```

---
## \#5 Posted by: akhlut Posted at: 2018-03-22T14:39:35.598Z Reads: 236

```
[This](https://www.digikey.com/product-detail/en/te-connectivity-passive-product/HSC1001R0J/A102106-ND/2055297) is probably overkill.

![4-1625999-8|500x500](upload://7t74Xqk0gXXEeYuApcbLnsWv8Lk.JPG)
```

---
## \#6 Posted by: webst Posted at: 2018-03-22T20:50:18.115Z Reads: 216

```
Probably not, you might be dumping 1-2kW into this thing. Also look at this:
http://www.electric-skateboard.builders/t/best-18650-battery-charging-options/49719/16?u=webst
;)
```

---
## \#7 Posted by: akhlut Posted at: 2018-03-22T21:08:00.620Z Reads: 200

```
I dunno - were not talking about instantaneously dumping all the kinetic energy of the traveler.  This guy uses a 225W array of bulbs to dump the excess current, and i doubt he's shedding the maximum load that array can emit.
```

---
## \#8 Posted by: webst Posted at: 2018-03-22T21:30:01.070Z Reads: 194

```
You're saying that 100W resistor will be overkill. 
From the link in first post:
> Braking 100 kg from 30km/h within 30m should need ~1900W ( time to brake = v/2 / s, E=mv²/2, P=Delta E/Delta t )
```

---
## \#9 Posted by: b264 Posted at: 2018-03-22T21:31:39.643Z Reads: 187

```
It's my opinion that this should be handled by the BMS and not an add-on circuit.  The balancing circuitry in the BMS would be best suited for this, maybe have a place for a large resistor or energy sink to hook up.  @SimosMCmuffin
```

---
## \#10 Posted by: Vanarian Posted at: 2018-03-22T22:08:36.783Z Reads: 182

```
Thank s for the replies guys. Yep à BMS managing this would be killer (was thinking of the FLEXIBMS) ; still would be nice to get a spare pcb to simply hook up to your battery?
```

---
## \#11 Posted by: lock Posted at: 2018-03-22T23:14:27.101Z Reads: 185

```
[quote="webst, post:8, topic:49823, full:true"]
You’re saying that 100W resistor will be overkill.

From the link in first post:

Braking 100 kg from 30km/h within 30m should need ~1900W ( time to brake = v/2 / s, E=mv²/2, P=Delta E/Delta t )
[/quote]

[Even at only 20w, those 100w resistors get burning hot in seconds](http://www.electric-skateboard.builders/t/load-testing-discharging-a-custom-battery-pack/2888/19). So hot they burnt the piece of wood they were mounted too. You'll need a lot more than just one, hook them up to a large heatsink, and probably still need a fan (a big fan).

Generally think the issue with this idea is finding something that can absorb the load. 225w is only like an extra 6a of breaking power...
```

---
## \#12 Posted by: Deckoz Posted at: 2018-03-23T00:45:23.390Z Reads: 156

```
Mellow has this in a 1000w resistor...inside a tube of aluminum...
```

---
## \#13 Posted by: b264 Posted at: 2018-03-23T00:59:46.477Z Reads: 161

```
[quote="lock, post:11, topic:49823"]
225w is only like an extra 6a of breaking power…
[/quote]

If it's built right, it's only braking power.  If it's built wrong, it might be breaking power.
```

---
## \#14 Posted by: lock Posted at: 2018-03-23T01:05:55.542Z Reads: 164

```
Heh, I just googled this and ended up [right back here](http://www.electric-skateboard.builders/t/anyone-want-to-know-how-mellow-does-their-braking-systems/8507). There's also some info on their website.

I'd be interested to see this, all the big resistors (1000w range) I came across were huge, as in the size of my forearm. Anyone pulled apart a Mellow board?

edit... Nevermind they have a rundown on their site too.
![image|664x353](upload://o3NMPE73YnPExuC2yuCRMGCXB8l.jpg)
```

---
## \#15 Posted by: akhlut Posted at: 2018-03-23T02:33:39.636Z Reads: 154

```
I'm not suggesting that a 100w resistor could effectively bring you to a dead stop.  I watched the video, and based on that use case (light, short braking) a 100w resistor would be fine.  

I know how hot they can get.  We used to use them to make heated beds for repraps back in the day.
```

---
## \#16 Posted by: webst Posted at: 2018-03-23T06:28:15.491Z Reads: 151

```
Well, that should do!
![image|300x225](upload://1XqbJkHhrPxZKEuUf0478AH5KOB.jpeg)
```

---
## \#17 Posted by: SimosMCmuffin Posted at: 2018-03-23T06:28:36.551Z Reads: 150

```
I suppose it could be done on the Switch-module. I don't see any real reason it couldn't. Might be actually possible to just use the BQ76200's Charge FET output to directly control a N-channel FET going to a brake resistor. Heat dissipation might be the real problem, as you need to dissipate all that extra power somewhere else than the battery.
```

---
## \#18 Posted by: b264 Posted at: 2018-03-23T06:29:38.689Z Reads: 147

```
[quote="SimosMCmuffin, post:17, topic:49823"]
Heat dissipation might be the real problem, as you need to dissipate all that extra power somewhere else than the battery.
[/quote]

Heat dissipation wouldn't be the BMS's problem :stuck_out_tongue:

If you want to hook up an external dissipator though, it'd be interesting if the BMS had a spot for it.  Maybe even a power resistor bolted to the truck hanger or something, dissipate heat on that...
```

---
## \#19 Posted by: SimosMCmuffin Posted at: 2018-03-23T06:32:40.984Z Reads: 141

```
I was about to ask about the type of resistor you're thinking to use. My first thought was something located on the switch PCBs itself, but you seem to be thinking of a completely external resistor. I suppose the easiest could be to just leave wire hookup points available on the board.
```

---
## \#20 Posted by: b264 Posted at: 2018-03-23T06:36:16.594Z Reads: 142

```
As we can see above, it may not even be a resistor.  I wouldn't assume what it is at all.  Just somewhere to dump energy, if it's hooked up...
```

---
## \#21 Posted by: webst Posted at: 2018-03-23T06:40:33.087Z Reads: 131

```
It’s always kind of resistor
```

---
## \#22 Posted by: SimosMCmuffin Posted at: 2018-03-23T06:45:25.713Z Reads: 133

```
About the discussion above between 100-1000W rated resistors, those are the continuous rated power under sufficient cooling conditions. A 100W resistor will burn itself out from the inside if it's subjected to for example 200W for long enough time, because it simply can't move the heat from the resistive element inside to the heat mass outside efficienctly enough.

But the resistor itself doesn't need to be that huge, but rather have good heat transferring capability to a heat mass, which is preferably cooled. I believe Mellow is using their whole drive unit as a heatsink.

[quote="webst, post:21, topic:49823, full:true"]
It’s always kind of resistor
[/quote]
Could be a MOSFET run in the ohmic region as well. Behaves like a adjustable resistor, so the braking power can be controlled.
```

---
## \#23 Posted by: b264 Posted at: 2018-03-23T06:48:52.003Z Reads: 129

```
[quote="webst, post:21, topic:49823, full:true"]
It’s always kind of resistor
[/quote]

Could be a resistor, a diode, a light, a heating element, another battery, a supercapacitor, a motor & propeller

Never assume ;-)
```

---
## \#24 Posted by: webst Posted at: 2018-03-23T06:51:41.995Z Reads: 121

```
Actualy you just assumed those components have no resistance :slight_smile:
```

---
## \#25 Posted by: webst Posted at: 2018-03-23T06:55:17.997Z Reads: 123

```
But talking about supercaps, yesterday I bought mini screwdriver that has 4.6V 320F cap inside. It’s roughly 400mAh if my calculations are correct but pretty large charger that’s in a set charges it within 60 seconds. Also I don’t know how much of this energy can be used but I suppose that it might be more than in battery where you have to care about not destroying internal chemistry.
```

---
## \#26 Posted by: SimosMCmuffin Posted at: 2018-03-23T07:00:18.848Z Reads: 122

```
[quote="webst, post:25, topic:49823"]
It’s roughly 400mAh
[/quote]
At what nominal voltage?

Capacitor stored energy:
E = 0.5 * C * U^2 = 3240 Ws or J, if charged to 4.5V
3240 Ws = 0.9 Wh
Li-ion equivalent capacity, using nominal 3.6 V  -> 0.9 Wh / 3.6V = 250 mAh
```

---
## \#27 Posted by: webst Posted at: 2018-03-23T07:09:40.331Z Reads: 125

```
I used formula I found on arduino forum: 320F 4.6V capacitor can store Q=CV=1472 Coulombs of charge, 1mAh is 0.001 Columbs per second (0.001A) multiplied by 3600 seconds or 3.6 Coulombs.  So the capacitor should be equivalent to 1472/3.6 = 409mAh
```

---
## \#28 Posted by: SimosMCmuffin Posted at: 2018-03-23T07:17:14.456Z Reads: 129

```
I'm talking about the stored energy inside the cap, which we can then compare to a li-ion cells nominal voltage capacity.

http://hyperphysics.phy-astr.gsu.edu/hbase/electric/capeng.html
![image|690x424](upload://kLFgyKeJx6z9THruI32qaLRZ4e.png)

Anyhow, how does the driver feel? How much can you do before the voltage drops too low?
```

---
## \#29 Posted by: b264 Posted at: 2018-03-23T07:35:49.496Z Reads: 124

```
[quote="webst, post:25, topic:49823"]
4.6V 320F cap
[/quote]

That's a shit-ton of capacitance.  Can't believe that says `F` and not `μF`
```

---
## \#30 Posted by: SimosMCmuffin Posted at: 2018-03-23T07:39:16.575Z Reads: 122

```
3000F 2.7V
https://www.digikey.fi/product-detail/en/maxwell-technologies-inc/BCAP3000-P270-K04/1182-1021-ND/3079285
```

---
## \#31 Posted by: webst Posted at: 2018-03-23T09:00:19.117Z Reads: 122

```
[quote="SimosMCmuffin, post:28, topic:49823"]
Anyhow, how does the driver feel? How much can you do before the voltage drops too low?
[/quote]

I have no rig to test it but feels good, no difference between regular battery operated one  except capacity and charging time. I can compare it with regular battery powered one of similar power later. But the only test i can think of is putting screws into pine board until battery dies.
```

---
## \#32 Posted by: webst Posted at: 2018-03-23T09:23:54.585Z Reads: 117

```
Going back on tracks I think that easiest method would be relatively short wire heater (the one you see on top in your oven) on some kind of ceramic insulator in a cage. It can get extremely hot and can eat 2000W easily. This is also method used to stop small wind turbines.
```

---
## \#33 Posted by: Vanarian Posted at: 2018-03-25T17:37:46.113Z Reads: 111

```
Well **WOW** I wasn't expecting such a strong feedback on this thing :sweat_smile: 

@lock Mellow is ahead in the future ! That's how every damn skate should be setup (I mean safety and quality wise). I got a bunch of their battery connectors, RoPD connectors 40A, these things are nice ! Waterproof and magnetic at the same time, easy to mount and impossible to mismatch. 

Supposedly a 500W break chopper might be enough to burn away excessive loads, given you can also aerodynamically slow down with your body. Spread arms, stand higher a bit, it will eat away them watts. 

@webst which kind of ceramic cage were you talking about ? Which length of heat wire ? With a good placement on air pathway can do, I guess it should be put away from the ESC too as much as possible.

What about a string of smaller resistors or wires mounted on a heatsink with thermal compound ?
```

---
## \#34 Posted by: Kug3lis Posted at: 2018-03-25T18:34:47.448Z Reads: 108

```
I was thinking about this for a moment and then had a thought that when breaking the voltage rise on the bus voltage not in the batteries itself. I think cutoff should be operated on cell level using BMS which can sense each cell voltage than the whole bus. Because then you brake you generate a voltage which is not instantly consumed by battery, it is like charging a battery with higher voltage when it is. So for voltage cut off, I think cell voltage would be more appropriate.

For e.g. you brake for 10s with 30A power u battery pack is 42V 10Ah so you generate 42V * 30A = 1,2kW for 10s which is 3.33Wh.

So if I understand correctly in those 10s you generate less than 1% of battery capacity which is also not all energy going into battery considered all the loses and other consumptions on the circuit. So even when you apply a higher voltage with current I don't think it would overcharge the battery but just rise the bus voltage which is kinda ok. But it's just my 6-year-old physics thoughts on this problem.

P.S. I can be really wrong on this. It's just my assumptions :D

tl;dr Don't make cut off based on bus voltage but on summed cell voltage.
```

---
## \#35 Posted by: Pedrodemio Posted at: 2018-03-25T18:48:44.658Z Reads: 102

```
The big problem is that the cells don’t like fast charging, even more at a high state of charge

Mellow use the braking resistor not only when the battery full, but every time the current going back into the battery is greater than a set level for a given state of charge
```

---
## \#36 Posted by: Deckoz Posted at: 2018-03-25T19:00:34.789Z Reads: 103

```
Cells don't like fast Charging because of IR. Cells will absorb current as quickly as they can, when the current cannot be absorbed it turns into voltage spikes. Lower IR cells absorb more amps, just like lower IR cells give off more current easily vs higher IR...

As I stated in another post..but it was about antispark. More capacitance would solve this. But it would make the spark larger if you don't have an antispark...
```

---
## \#37 Posted by: webst Posted at: 2018-03-25T22:25:10.883Z Reads: 101

```
http://solarhomestead.com/dump-loads-for-solar-wind-and-microhydro/

I also found solution little closer to what we need, I'm unable to evaluate if there's everything fine with this rather uncomplicated circuit:

http://vedder.se/forums/viewtopic.php?f=15&t=586&start=10#p3635

Edit: update on my last link "This energy dump is intended for running a motor on the lab bench, from a lab power supply that cannot absorb regenerated energy. It would also allow you to do regenerative braking even though your batteries were fully charged if used on a vehicle (and if it was carefully dimensioned for the load), of course."
```

---
## \#38 Posted by: webst Posted at: 2018-05-08T12:16:41.948Z Reads: 89

```
I thought about it for some time and come to following conclusion. All this heating element idea is a little low tech. It would be much more elegant to redirect excess power to electromagnets surrounding copper discs connected directly to front wheels. That should induce eddy currents stopping the board. This would unfortunately need new esc construction with additional circuit dedicated to this task but I like the idea of frictionless brake.
```

---
## \#39 Posted by: Vanarian Posted at: 2018-05-08T18:09:18.296Z Reads: 87

```
Would actually be some next Gen braking safety, but required circuitry seems a bit complicated and steep price. First let's get the brake chopper as reliable and as affordable as possible.

If it is well done and quick enough to trigger the protection, it could even lead to safely play closer to the DRV absolute max (if even transient voltages spikes can never cross the protection, you're good to play with 13-14S worry free).
```

---
## \#40 Posted by: webst Posted at: 2018-05-08T22:16:45.034Z Reads: 85

```
I like brake chopper idea but DRV problem lies in compromises taken during vesc design and making that kind of prostetics would not be worth it. Imo the only proper way to deal with it is getting 6th gen that has much higher limits. Nevertheless I don’t think that any of solutions provided can be added with simple switch, well actually there is one: when the voltage goes above 4.2 per cell you’d open this brake chopper circuit assuming it can work as dump load. This should be theoretically done with some minimum effort. Other solutions involving going directly with power into some load would involve esc that can handle this as something has to redirect this power to another place while you remain control over the board.
```

---
## \#41 Posted by: Nordle Posted at: 2018-06-14T08:15:45.827Z Reads: 87

```
I‘m really interested in this. I hit that overvoltage so often... almost dislocated my shoulder the first time it happened, and 5 times in 2 yrs was really enough..

I found this simple circuit:
![image|281x499](upload://pHbKaiuDksdlox8z3m4imNv9s6v.png)
[source](https://www.roboteq.com/index.php/support/setup-troubleshooting-faq/113-support/supportfaq/377-q-protecting-against-reneration)
I think i can build one, but i can‘t program digital outputs on my vesc. Could someone teach me that or head me to a guide, or simply do it 4 me?:)
```

---
## \#42 Posted by: Vanarian Posted at: 2018-06-14T12:11:46.430Z Reads: 80

```
I still need one too, overvoltage and battery cut off in general is scary. I'd rather not experiment that at all, you getting thrown by it 5x times is too much already. 

Please report how it goes if you build it, on my side I'll ask an engineer what he'd do/advise/correct based on both this circuitry and the ones shown previously.
```

---
## \#43 Posted by: Nordle Posted at: 2018-06-14T16:24:15.900Z Reads: 77

```
Was thrown off once, jumped off and run it out the other times. The 5 shoulder dislocations were from snowboarding:/

The circuit seems dead simple to me, but i‘m a software noob and would need to change vesc settings, so it would give me 5V somewhere instead of going overvoltage cutoff.
```

---
## \#44 Posted by: Vanarian Posted at: 2018-06-14T21:01:33.050Z Reads: 80

```
Damn, didn't know snowboarding could hurt this much (actually I may have been very lucky till now with snow sports : never broke / hurt anything despite many falls) !

I checked the full page you linked,  yea it does sound pretty simple and hopefully reliable. Which resistor and which MOSFET would you use for this method ? Can it trigger upon overvoltage detection *before* the VESC issues a cut-off, it it relies on the digital output ?
```

---
## \#45 Posted by: Nordle Posted at: 2018-06-15T05:03:50.849Z Reads: 77

```
Didn‘t plan anything so far. But any mosfet (as long as it can handle the loads) should do the trick. 
For the resistor, one of the big ones linked previously. Or maybe can find something gimmicky like the heater wire but with some arcs like in star wars pot racers maybe... probably not:D

I don‘t get the last part, but this would instead of going overvoltage cutoff rise a voltage on any chosen pin wich would then open the mosfet. That puts the resistor in parallel with the battery and the Voltage in the bus wire that would normally exceed battery voltage is droped by the resistor.
There is no overvoltage cutoff anymore, the digital output and this circuit instead.

Sadly i can‘t program:(
```

---
## \#46 Posted by: Nordle Posted at: 2018-06-20T09:06:50.368Z Reads: 67

```
Tried to make one a bit more simple:
edit: look below for new schematic
```

---
## \#47 Posted by: Vanarian Posted at: 2018-06-21T21:01:29.537Z Reads: 59

```
Basically you only need a programmer to be able to test it ?
```

---
## \#48 Posted by: Nordle Posted at: 2018-06-21T21:27:33.661Z Reads: 59

```
No this one does not require a signal fom esc.

You set a voltage with the potentiometer and it **should** work.
i got help [here](https://forum.allaboutcircuits.com/threads/braking-chopper-overvoltage-dumb-load.149820/) recently, will make one soon i think
```

---
## \#49 Posted by: Vanarian Posted at: 2018-06-21T21:49:50.543Z Reads: 55

```
If you can lay it on a PCB under 50x50, I'm up to participate as test guinea pig haha! I might as well keep it in the fam' instead of going freelance route. I'll try it up to 13S voltage. I can relocate the resistor if it is big, "a la Mellow" with an aluminum cylinder.

I'll need many brake choppers units in the long run, and push it to the DIY scene along the way if it works as a good standard !
```

---
## \#50 Posted by: Nordle Posted at: 2018-06-22T06:23:42.181Z Reads: 61

```
How big should the difference between trip voltages be?
lets assume a 10S 42V battery:
trip on voltage is set to 42V, now we break but battery is already full and we would exceed 42V. instead of getting an overvoltage cutoff the break chopper turns on. Voltage suddenly drops (how much is dependent by the size of the dump load and battery capacity), and the chopper would instantly turn off again and may beginn to oscilate. Against this we create a second trip point.
How much lower should that trip off voltage be?

i doubt 1V lower should be fine?
```

---
## \#51 Posted by: Vanarian Posted at: 2018-06-22T13:47:57.703Z Reads: 61

```
Depends in the load itself IMHO but looking at the unicycle project shown in video, a 0.5v max trip might be way enough.

Supposed behavior I see is : when he brakes is : it does actually exceeds the first trip voltage shortly and comes back under the value. But it still is fed with a lot of power from the regen braking, so voltage kinda "fights" to rise back to a higher level.

Edit : OK reading again what I wrote, had to correct it.

Given how the Zener opens gradually till full open (and vice versa) can't you use 41.5v to 42v? I was guessing 41.7v trigger earlier cause it brings a safe margin too.
```

---
## \#52 Posted by: Nordle Posted at: 2018-06-23T17:04:50.698Z Reads: 56

```
![circuit%20(1)|690x411](upload://owVuJ05aRPQI7gDXjOhp0mqbyKW.png)
this should be the final circuit

the zener D1 just creates a 7V reference voltage, D2 is 12V supply for the op amp.

the first (high) trip point is set by adjusting the pot R4
the second (lower) trip point is created by adding a hysteresis resistor (R8)

if i set 41.5v as first point and use 2MOhm for R8 the second trip point becomes 40.9v. (1MOhm resistor and the second trip point becomes 40.4v)
```

---
## \#53 Posted by: Vanarian Posted at: 2018-07-20T19:58:04.746Z Reads: 46

```
Hey, how is the circuit going? Did you get your testing units done? I wanna try this too!
```

---
## \#54 Posted by: Brdchris Posted at: 2018-07-20T21:09:18.029Z Reads: 43

```
This is fairly common in high inertia industrial drives. I’ve installed a few of these to shed dc buss voltage.
```

---
## \#55 Posted by: Vanarian Posted at: 2018-07-20T22:08:45.734Z Reads: 42

```
Dude we absolutely need this into our DIY. What are you waiting for? :wink:

Edit : On my side, I'm taking some time for myself, will press the throttle again in September. And I got a shlongboard FWD to figure out for August !
```

---
## \#56 Posted by: Nordle Posted at: 2018-07-21T07:59:55.008Z Reads: 41

```
Take a look here:
[http://vedder.se/forums/viewtopic.php?f=15&t=586#p3515](http://vedder.se/forums/viewtopic.php?f=15&t=586#p3515)
[http://vedder.se/forums/viewtopic.php?f=15&t=1723&p=9047#p9047](http://vedder.se/forums/viewtopic.php?f=15&t=1723&p=9047#p9047)
i also opened a topic on this forum, but the only response was that i rather just shouldn't charge my battery full and that guy claimed to be an electrical engineer-.-
```

---
## \#57 Posted by: Vanarian Posted at: 2018-07-21T18:43:33.318Z Reads: 34

```
Lol that sounds like somebody I've met here too. Still we got good tracks with your topics and what has been posted here :sunglasses:
```

---
