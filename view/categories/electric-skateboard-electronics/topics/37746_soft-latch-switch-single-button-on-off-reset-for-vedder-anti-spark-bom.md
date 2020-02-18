# Soft-latch switch single button ON/OFF &amp; reset for Vedder anti spark : BOM?

### Replies: 37 Views: 3490

## \#1 Posted by: Vanarian Posted at: 2017-11-08T15:55:50.073Z Reads: 271

```
_EDIT² : I updated the BOM at bottom of this post._

The title says it all guys :smile: Btw I realize this is my first thread ! It's time I started moving my lazy ass. 

I need a reliable yet very flat & compact switch button for my skates so most mechanical buttons can't work for me. _I simply don't have the space for the cylindrical body and toggle switch is out of question !_ And I'd like to make a custom button shape and material with RGB LED for a sexy finish. Momentary push-type is sleek.

I already got a vedder-type anti-spark module from @goldenHusky, what I only miss is really the switch itself to command the module.

So... I've been itching to build a soft-latching single button switch instead. If you look around, you'll find tutorials with different methods to achieve that - first example : 

https://www.youtube.com/watch?v=tjrSdET6NFc&t=19s

Please note that this example have the drawback of starting in "ON" position and not "OFF" yet we **do** want the switch to always start disconnected. So we'd need an auto-reset function included to guarantee that.

Edit : we also want a delay function (push ON / hold 2-3seconds OFF) !

Well there are good news : @s28400  has done the hard work to make an auto-reset soft-latching switch interface with Vedder's anti-spark module ! There is no update on the matter since September 2016 and no BOM posted but as shown below **it was already working back then with all wanted features** : 

https://www.youtube.com/watch?v=UR5QIhaAFDc&feature=youtu.be

Posted from his page "radical-creation" : 

> The best solution I have found is a soft latching switch circuit. This utilizes a momentary switch to latch a logic signal high or low. A slightly modified version of this circuit will yield a push on and hold off configuration. This is ideal because it is the most reliable and most robust of all the options. 

> I put together a quick circuit on a breadboard and interfaced it with a mosfet. I will post a full schematic once I finish it. Anyway here is a video of the working circuit.

> It seems to work perfectly and I will next look to reduce the size of the circuit by making it on perforated board and possibly a custom pcb.  
 
So what we lack is a PCB with a BOM. Can you help me source proper parts to try this out ? We can make a great low-profile custom switch to plug on our anti-park modules thanks to Joshua's work. 

**Here is the schematic :** 

[img]https://www.radicalcreation.com/forums/download/file.php?id=328&mode=view[/img]


**Proposed BOM (work in progress) :** 

- 1x Linear regulator : LM317HVT (60v max input, programmable output to 5v - need a pair of resistors or potentiometer to fix 5v output - good up to 12s/13s) 
or
1x LM7805 linear regulator (40V max input, fixed 5v output - no resistor needed - good up to 8S)
- 2x 100kOhm resistors
- 1x 5mOhm resistor
- 2x 1uF capacitor (from the bucket)
- 1x 1mOhm resistor
- 1x heatsink for the regulator
- 1x NAND gate (5v) - I went for CD4011 chips, cheap 4x NAND available on eBay
- 1x MT3608 boost converter or 1x LM2596S step-up converter for excitation of "C" pin
- 1x 12v zener diode
- 1x irf510 mosfet
- 1x momentary push button (you can either get a mechanical one or recycle one from a TV remote)

**Optional (for some custom) :**

- 1x simple LED
or the combo
- 1x ws2812/sk6812 RGB LED or more
- 1x arduino (Nano or else)
- 1x 470ohm resistor
- 1x 1000uF capacitor

**Next step (work incoming) :**

- The wiring !
```

---
## \#2 Posted by: Kug3lis Posted at: 2017-11-08T15:58:32.928Z Reads: 215

```
u will need pretty sick voltage regulator if u have 10S :D
```

---
## \#3 Posted by: Vanarian Posted at: 2017-11-08T16:01:33.502Z Reads: 211

```
I'm not sure because the switch itself may not see as much voltage! 

[quote="goldenHusky, post:77, topic:31872"]
You basically need to set the "C" pin to high or low. High should be at least around 20V (equals 6s input voltage) to make it work because there's a 12V zener diode on it. You could use a small N-channel logic level mosfet and a resistor with a high value to make it work.
[/quote]
```

---
## \#4 Posted by: Kug3lis Posted at: 2017-11-08T16:03:52.361Z Reads: 193

```
U connect ur 5V regulator to + of battery
```

---
## \#5 Posted by: b264 Posted at: 2017-11-08T16:11:35.416Z Reads: 184

```
"Push On / Hold Off" would also be way safer, if a stick or debris bumped your switch, your board would not shut down.  Or heavy vibrations would not shut your board down either...  me like
```

---
## \#6 Posted by: Vanarian Posted at: 2017-11-08T16:11:57.703Z Reads: 180

```
How are the mechanical push-lock or toggle switch usually plugged to the anti-spark ? I was thinking we could feed power to the soft-latch from same source at least to limit current. Then we could look for a big regulator as you pointed out (thanks btw!). 

a 60v regulator would give some margin... but maybe selecting different modules for lower voltage would allow less wasted heat on the regulator ?
```

---
## \#7 Posted by: Vanarian Posted at: 2017-11-08T16:13:53.444Z Reads: 169

```
Edit : sorry I misread your post. Yea, push ON / Hold OFF !
```

---
## \#8 Posted by: SORRENTINO Posted at: 2017-11-08T16:19:42.068Z Reads: 166

```
If boosted can do it so can this community :grinning:
```

---
## \#9 Posted by: b264 Posted at: 2017-11-08T16:23:15.212Z Reads: 170

```
I actually traced down all my "Evolve remote disconnects" to a problem where the (mechanically-latched) power switch disconnects for a few milliseconds under vibration and shuts the board down...

So improvements like this "hold for off" soft power button can actually have really important safety implications under the right conditions
```

---
## \#10 Posted by: Vanarian Posted at: 2017-11-08T17:59:10.483Z Reads: 164

```
@b264 that's pretty scary. All the more a reason to sort this circuit out.

I narrowed a first choice for the regulator : LM317HVT chip in TO-220 package ! 

https://compelectronic.fr/pdf/lm317hvt.pdf

Pretty cheap and seems reliable. Would need a heatsink to manage heat. It has programmable voltage though, how do we manage that ?
```

---
## \#11 Posted by: b264 Posted at: 2017-11-08T18:44:31.973Z Reads: 142

```
You can do that by selecting the values for the resistor R2 or using a potentiometer.  What voltage do you need?
```

---
## \#12 Posted by: Vanarian Posted at: 2017-11-08T18:48:25.655Z Reads: 148

```
Ideally I need 5v fixed output voltage from the regulator.

Edit : what about the NAND gate, is this one a good choice ? 

https://www.ebay.fr/itm/MC14093BCP-4093-Quad-NAND-2-Entrees-Schmitt-Trigger-DIP14-Motorola-Neuf/272576117513?hash=item3f76cd7b09:g:8sIAAOSwOgdYuYOK
```

---
## \#13 Posted by: b264 Posted at: 2017-11-08T18:49:53.703Z Reads: 137

```
If you need 750mA or less (3.75 watts) use an LM7805 instead of the LM317HVT
```

---
## \#14 Posted by: Vanarian Posted at: 2017-11-08T18:52:31.245Z Reads: 140

```
I got some spare LM7805 in hand but I think max voltage input is 40v ? It would be good for max 8S (which is enough for my build though) no?
```

---
## \#15 Posted by: b264 Posted at: 2017-11-08T18:53:49.370Z Reads: 133

```
Oh, good point
```

---
## \#16 Posted by: b264 Posted at: 2017-11-08T18:55:24.393Z Reads: 130

```
What about this, it's smaller and cheaper https://www.digikey.com/product-detail/en/toshiba-semiconductor-and-storage/TC7WZ00FKLJ-CT/TC7WZ00FKLJ-CTCT-ND/6198841  
  
Plus you get to demonstrate your soldering prowess ha ha ha
```

---
## \#17 Posted by: Vanarian Posted at: 2017-11-08T19:05:15.119Z Reads: 145

```
Haha well my soldering skills are at lvl 5 - trainee but I fear not ! Though I realize that I got a handful of these in a box 

http://www.ebay.fr/itm/Texas-Instruments-SN74-30-N-8-Input-Positif-NAND-Gate-Porte-DIP-14-IC-5V-13ns/272110272584?hash=item3f5b094048:g:cOIAAOSw8lBTrVwK

So I'll experiment with these ! And it is cheap too (and bit bigger pins so hopefully I won't fry them while soldering)  !

Edit : Ok we're almost complete for the BOM ! What's left is a MOSFET and a momentary button (but I'll salvage the inner button from a TV remote I think). Maybe we need a boost converter for excitation of the "C" pin ?

I received 2x MT3608 modules which could do the job, still very compact and flat modules. Just plug it after the MOSFET and voilà !
```

---
## \#18 Posted by: b264 Posted at: 2017-11-08T19:11:48.059Z Reads: 138

```
Actually the LM2596S are a great part for this but they are $5 each  (10S max)
```

---
## \#19 Posted by: Vanarian Posted at: 2017-11-08T21:17:17.297Z Reads: 137

```
Ok I added it to the BOM. I just ordered irf510 mosfets to complete the circuit, pretty cheap too!
```

---
## \#20 Posted by: b264 Posted at: 2017-11-08T21:28:47.511Z Reads: 137

```
It'd be awesome if we could find something just like LM2596S except that works on 14S ... also the DC-DC converters already built are cheaper than the chip itself
```

---
## \#21 Posted by: Vanarian Posted at: 2017-11-08T21:33:54.702Z Reads: 121

```
How do you want to use the LM2596S?

If as boost voltage for the "C" pin, 20/25V should be enough from what @goldenHusky said.
```

---
## \#22 Posted by: b264 Posted at: 2017-11-08T21:40:42.640Z Reads: 122

```

As a DC-DC converter with a little 100mH inductor
```

---
## \#23 Posted by: goldenHusky Posted at: 2017-11-09T06:32:38.348Z Reads: 118

```
@Vanarian Also use a 1MOhm resistor in series with the "C" pin to limit the current. So it's basicially a voltage divider with R1 = 1MOhm and the 12V Zener as R2 and as supply voltage the 20/25V. Have a look at the schematic on vedders github. Also some kind of latching relay between the 1NO and C pin works.
```

---
## \#24 Posted by: Vanarian Posted at: 2017-11-09T13:36:54.327Z Reads: 111

```
Thanks for the tip :smile: I updated the BOM again ! Btw just realized that we also need only one SN74 NAND chip because it is built with at least 4 NAND gates inside (we only need 2). 

I still need to determine the correct pins and we'll get something good !
```

---
## \#25 Posted by: Vanarian Posted at: 2017-12-02T12:16:57.953Z Reads: 101

```
Bit of update on the BOM, I still require a NAND (my chips at home are octo buffer drivers not NAND gates so ordered a batch) and we'll be starting assembly and tests !
```

---
## \#26 Posted by: Vanarian Posted at: 2017-12-10T20:35:00.941Z Reads: 107

```
Up ! I need some insight from more competent people than me :sweat_smile:

I tried a first version of the soft-latch itself trying to comprehend how to plug everything from regulator output pin till mosfet.  

I replaced regulator with direct 5v source to "simulate" it. Mosfet outputs are 1x to ground, other to a LED diode. Goal is : if the LED diode follows press = ON, hold = OFF, it works.

I use cd4011be NAND and irf510 mosfet. 

http://www.allaboutsensors.com/image/cache/data/4011-500x500.JPG

http://www.geocities.ws/radio107mhz/mosfet1.gif

Here is my actual plugs, which doesn't work yet. Can you guys point me out where I went wrong ?

<img src="/uploads/db1493/original/3X/a/1/a1b0a34c5f7de77378cb7b9863e89ba34857d6f5.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/8/a/8a767e01e332803cff095e17ebbc3574db0805aa.jpg" width="690" height="388">
```

---
## \#27 Posted by: Pimousse Posted at: 2018-01-10T10:04:15.835Z Reads: 91

```
Do you power red LED directly with 5V ? (I can see its resistor)
Anyway, it's hard to tell just looking at theses pictures :grin:
Do you have the schematics ?
And dumb question : are your wires reliable ? (no false contact)
```

---
## \#28 Posted by: Vanarian Posted at: 2018-01-11T10:28:22.554Z Reads: 90

```
True it looks like a mess, I'll split the whole schematic into separate schematics and post according breadboard pics, should be easier to troubleshoot. I also had 2x hazardous wires in the lot, which doesn't help !
```

---
## \#29 Posted by: Vanarian Posted at: 2018-01-20T21:22:53.196Z Reads: 98

```
I'm back :smile:  I've split everything in five smaller sections to check all the wiring. I temporarily replaced the anti-spark module pins by a simple LED so it is easier to read.

So first, the BOM used for schematic (simplified to minimum) : 

- 1x L7805CV linear regulator (5V 1.5A fixed output, max 8S input -
 can be replaced by LM317HVT + couple resistors for higher voltage)
- 2x 100kOhm resistors
- 1x 5mOhm resistor
- 2x 1uF capacitor
- 2x NAND gates (5v) in 1x combo CD4011be chip (up to 4x gates inside)
- 1x irf510 mosfet
- 1x momentary switch

Next, the overall schematic : 

![soft latch general schematic|690x388](upload://dzMTsvmZEUyqNXsc8gsOYZ4nOyF.jpg)

Part 1 & 2  : 

![Soft latch schematic pt1&2|690x388](upload://oGdk3eSY3D0tGK7KY8cP67rEpsp.jpg)

![Soft latch pt1|346x500](upload://4SYPaPzXV5s5zQAb34ARpWEC3nQ.jpg)

![Soft latch pt2|366x500](upload://yKvewDB1714edULLv94BIHkkwVO.jpg)

Part 3 : 

![Soft latch schematic pt3|690x387](upload://5M2E9HIanUM4ggOcKTKwh93zZ6T.jpg)

![Soft latch pt3a|345x500](upload://6xstxzOrE0xbtjBblsLocUeniGj.jpg)

![Soft latch pt3b|365x500](upload://iKqdbgaVSrK4iVsIv8v1Z0tCkLR.jpg)

Part 4 & 5 : 

![Soft latch schematic pt4&5|690x388](upload://xIShVZ9VMGw5QWEeJ00gxxXou3M.jpg)

![Soft latch pt4|377x499](upload://tS4MzSU0FONAoX4gaeS547vL1X3.jpg)

![Soft latch pt5|404x500](upload://i5lO9sT6a1tPV5QLzJ9oRA3FOyD.jpg)

Do you see anything wrong within the small sections ? Or does everything match correctly ? Another question that occured to me is : does placing the 1uF caps in one direction or other changes anything in the circuit ? Cause this was not precised in radical-creation's schematics. 

@Holyman92 @b264 @goldenHusky Guys I tag you so we can brainstorm that thing :beers:
```

---
## \#30 Posted by: b264 Posted at: 2018-01-21T04:26:29.098Z Reads: 78

```
The first thing right away is the FET isn't driving the LED so if it is or isn't working you won't even know without a 'scope

see my changes to the LED current path below

![5f27ec4f712c813b23fec15adf15325ceefe2a15|690x388](upload://tXGEePq6izWw0I9SKTMWHHXWsVd.jpg)

So if you do that and connect gate to +5V it should come on, right?  If you connect gate to ground it should go off, right?

Also I'm assuming
[quote]
1x 5mOhm resistor
[/quote]
means `1x 5MOhm resistor`
and if so, then I'd have to question why so big - I'd increase a capacitor before I used a resistor that high because that can lead to stray noise
```

---
## \#31 Posted by: Vanarian Posted at: 2018-01-21T13:45:17.665Z Reads: 81

```
I'm not sure about the MOSFET not driving the LED : maybe I'm wrong but when (G) goes HIGH, it feeds current from (S) to (D) and it doesn't allow to flow from (D) to (S) no? When (G) is LOW, it should be a closed loop. The LED I use does only let current flow one way too.

If that's the case plugging the LED this way wouldn't short the circuit?

I assumed that current flows kinda this way through the circuit (red is "permanent current", yellow is "excited current", pink is virtual "closed loop") : 

![soft latch current path|690x388](upload://sh6lDJjp6NtdkgMIsDPtK6H8fWB.jpg)

Edit : BTW I'm not aware of the use of the 5Mohm resistor, I supposed it is to limit current sent on NAND gates (when the switch connects it bypass the resistor and raise current to excitation level)? What would you advise to improve this / get rid of the resistor?
```

---
## \#32 Posted by: b264 Posted at: 2018-01-21T21:29:46.828Z Reads: 74

```
[quote="Vanarian, post:31, topic:37746"]
feeds current from (S) to (D)
[/quote]

current flows from positive to negative
electrons flow from negative to positive

Think of the mosfet leads as "source of electrons", "drain where they go out" and "gate controller", so if you steal electrons from the gate controller it dumps more into the drain, all from the source.

No current can flow through the LED because it's being driven from ground, into ground.  It's like connecting the two leads together with a wire.  Did you try what I suggested?

I suggested not to use a 5MΩ resistor because values that high start to approach the resistance of insulators -- like human fingers, plastic cases, PCB, and humid air.  Inside a skateboard, if moisture gets inside, you want the strength of the signals to be stronger than noise caused by moist air
```

---
## \#33 Posted by: Vanarian Posted at: 2018-01-22T14:50:19.811Z Reads: 68

```
Thank you for the explanation, I need to try this out and report :beer: gonna correct the schematic too

How about replacing the 5Mohm by 1Mohm ?
```

---
## \#34 Posted by: Vanarian Posted at: 2018-01-24T15:53:29.886Z Reads: 75

```
Bump, I got fun with a simulator with the NAND gates logic and schematic is working in simulator :man_factory_worker:t5: See here : https://academo.org/demos/logic-gate-simulator/

And the results (I emulated NAND "A" output Low/High to NAND "B" by adding a third input) are following !

![Interrupteur OFF 1|690x420](upload://v4SNroemvBTOKsj8XMZ9KaMoQLC.png)

![Interrupteur OFF 2|690x420](upload://2OovlHgzHUIrjppaYcJm0DLYjc4.png)

![Interrupteur ON|690x420](upload://q40D0HxLtWd7hcnpKSTlJbxpmaR.png)

So what's left to determine is capacitor and resistor values (the ones closest to the momentary push button) to charge HIGH and drain LOW the NAND B.
```

---
## \#35 Posted by: s28400 Posted at: 2018-02-04T00:37:51.949Z Reads: 77

```
Hello everyone,
I just saw this thread for the first time. I have recently been working on implementing a similar system into a dual custom VESC design but I could look into doing a standalone anti-spark PCB. I threw that original breadboard circuit together with some electronic scraps in the lab I work at so I don't remember exactly what parts I used. If you guys are interested in pursuing this more, I can whip together a PCB design and start on some prototypes.
Cheers,
Josh
```

---
## \#36 Posted by: Vanarian Posted at: 2018-02-04T03:23:38.357Z Reads: 76

```
Hi Josh, nice to see you here ! Actually this project has progressed thanks to your work :wink: 

I'm slowly troubleshooting on the breadboard & learnt a lot along the way. Would really appreciate your input to finish checking the wiring about the NAND and the MOSFET, and same for a PCB design to get the soft-latch plug and play.

I have a question : why use specifically a 2xNAND loop instead of a single AND gate ? 

Btw I replaced the original 5M resistor with a 2M instead to shorten the duration of "Hold" toward 2 seconds. 

Best
Chris
```

---
## \#37 Posted by: scepterr Posted at: 2018-02-04T05:10:20.840Z Reads: 76

```
Hey, curious to hear more about the custom dual vesc 😊
```

---
