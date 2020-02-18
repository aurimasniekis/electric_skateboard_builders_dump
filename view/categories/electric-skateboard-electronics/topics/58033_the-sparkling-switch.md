# The Sparkling switch

### Replies: 30 Views: 834

## \#1 Posted by: fedestanco Posted at: 2018-06-06T16:44:58.335Z Reads: 206

```
Yesterday I introduced the[Escalate in this thread](https://www.electric-skateboard.builders/t/escalate-a-vesc-6-derivative/57947?u=fedestanco) and among the upgrades I want to introduce there is a reliable anti-spark switch. 
This thing is well know to have a high failure rate so I though it was better to overkill the design.

These are features that I want in it. All of them are all already implemented in the schematics.
1) short press for turn on, longer press for turn off
2) reverse polarity protection :you plug black on red and nothing happens to the switch 
3) overvoltage transitiens protection: if voltage reaches high spikes, for example 100v spikes on a 60v preset maximum, then the switch will clamp the voltage to 60v dissipating excessive energy within the mosfets
4)overcurrent protection/ efuse: if the preset current limit is exceeded for more than a preset time, then the gate closes. This feature can be used as a fuse if the preset time is very short (<1ms)
5) inrush limiting (this was already done within the vedder switch): the charge pump will slowly turn the mosfets, safely charging capacitive loads (vesc caps)
6) superlow shutdown compsumpion: the ic draws 7uA (0.000007 amps)
7) high current capability

8) Cost very close to Vedder antispark: the ic I choose costs 2eu at quantity 1.

I will draw the pcbs hopefully this summer, but given the simplicity of the schematics anyone can do it on his own.
![sparkling2|690x333](upload://dnDoXTDqqtDcJxCLmYHH0SuQ9ZH.PNG)
![sparkling1|690x431](upload://6yaLu4eztQx0AizO86LePE314Gu.PNG)
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-06-06T16:49:44.931Z Reads: 168

```
I think feature number 1 is really good. When I made the switch myself it shuts off the board due to vibration trigers the switch.

but number 2 feature, does it not affect the regen feature?
```

---
## \#3 Posted by: fedestanco Posted at: 2018-06-06T16:51:03.630Z Reads: 165

```
I explained mysef wrong: the SWITCH circuits does not get damaged when reverse polarity is applied.
Reverse polarity is when VCC<VOUT (see schematics)
```

---
## \#4 Posted by: onepunchboard Posted at: 2018-06-06T16:53:10.937Z Reads: 164

```
ah ha! got it. sounds very robust.
I really like feature 3 as well. voltage spike seems to break many switches.
```

---
## \#5 Posted by: b264 Posted at: 2018-06-06T18:21:18.177Z Reads: 147

```
What happens if you put a 22mF load on it at 42V?  What part will be stressed the most?
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-06-06T18:29:42.428Z Reads: 135

```
Nice design, just one problem lt4356-1 will shutdown every time you will plug in VESC it will trigger overcurrent as high capacitive loads from capacitors inside will surge current ~100-500A That's where you get that spark. I tried similar chip in my design research it was constantly turning off because of overcurrent :)
```

---
## \#7 Posted by: fedestanco Posted at: 2018-06-06T18:43:27.421Z Reads: 122

```
The absence of C1 would certainly determine a huge inrush current; this is because the gate capacitance of mosfets is very low (nC) and the charging current high quite high (mA).

With the presence of C1, mosfets gates get charged slower (as slow as you want), thus they have very high resistance for a longer time, thus inrush current does not reach critical value.

The datasheet provides a formula to calculate how much capacitance is needed to avoid high inrush currents:
![lt4356|352x193](upload://vZw2O8lFSoUCS4LddvGPURVlXcu.PNG)![2%20lt4356|357x410](upload://nx48HcA3eIy7y0IfUQLqRQ2vmOZ.PNG)

BTW I have just started learning electronics so what I say may not be 100% correct. Appreciate any hint @Kug3lis
```

---
## \#8 Posted by: fedestanco Posted at: 2018-06-06T18:47:09.758Z Reads: 109

```
See my answer above: if you have 22mF (20 vescs) and want a max of (example) 2A inrush current, you put this value in the formula and find the best C1 for your needs.

Edit 2 vescs (2*680uf) --> 20 vescs
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-06-06T18:53:51.845Z Reads: 106

```
This type of circuit generates a ramp for the gate voltage which causes the output voltage to ramp. This limits inrush current due to capacitive loads. But there is a down side, while the voltage is ramping the MOSFET is operating in linear mode and subjected to stress of V*I. So half through the ramp for e.g. limited to 20A ramp up current in that time MOSFET will be dissipating 25V * 20A = 500W of energy. So it can really easily exceed SOA (Safe operating area) in MOSFET at that Vds which specifies how much current and how long it can withstand at specific Vds. So it will blow through the MOSFET :) For e.g. some MOSFET's cant handle 20A at 30V for more than 50ms

This is theories I learned myself while designing and working on my Anti-Spark switch :)
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-06-06T18:58:00.948Z Reads: 99

```
The best design would be similar to @jtag BMS with pre-charge circuit which pre-loads circuit with low current and then opens main gates :)
```

---
## \#11 Posted by: b264 Posted at: 2018-06-06T19:05:36.604Z Reads: 98

```
[quote="fedestanco, post:8, topic:58033, full:true"]
See my answer above: if you have 22mF (2 vescs) and want a max of (example) 2A inrush current, you put this value in the formula and find the best C1 for your needs.
[/quote]

Two HW4.12 ESCs is more like 4mF. (680μF x 3 x 2)

I mean a huge capacitive load like 22mF
```

---
## \#12 Posted by: fedestanco Posted at: 2018-06-06T19:11:50.785Z Reads: 95

```
Fixed it.
I haven't made one yet. But it would be interesting to see.

As @Kug3lis says, any quantity of energy required to charge capacitive loads needs to pass through the mosfets. So generally speaking you would need to see how much avalanche energy a single mosfet is capable of handling; then you would calculate how much avalanche energy your capacitive load generates; this way you'd know how many mosfets are needed to cope with your particular inrush current.
```

---
## \#13 Posted by: Maxid Posted at: 2018-06-07T13:47:18.628Z Reads: 77

```
Why not go for a similar FET as the fatboy one? Looks like the single but powerful fet works quite well.
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-06-07T13:49:00.419Z Reads: 81

```
Yes its possible as its SOA is pretty big ;) But don't forget for high **constant** (>50A) currents you need cooling. It has higher internal resistance compared to smaller friends :)
```

---
## \#15 Posted by: fedestanco Posted at: 2018-06-07T14:06:44.760Z Reads: 75

```
The thing is IF this layout is capable of coping with the inrush currents, then the big boy mosfet is not needed. 

Since the chip that I selected is specifically designed to manage inrush currents, I believe that the effect @Kug3lis is predicting will not happen as long as  you follow the manufacturer reccomendations (which is adding the ramping up cap C1). 
Real world testing will have the final word on this. If the six mos I choose fail, then an industrial mos should be choosen OR a buck converter must be added to replicate the precharge circuit of diebiems.

Now the comparison in terms of cost and heat generated:
SOA mosfet: I believe is around 15eu, not sure though
6 NTMFS5C628NLT1G are about 6 eu at quantity 1000

6 NTMFS5C628NLT1G have 0.4mohm rdson (combined) so when 100amps are travelling through them, only 4 watts are dissipated
```

---
## \#16 Posted by: Kug3lis Posted at: 2018-06-07T14:23:40.673Z Reads: 72

```
[quote="fedestanco, post:15, topic:58033"]
6 NTMFS5C628NLT1G have 0.4mohm rdson (combined) so when 100amps are travelling through them, only 4 watts are dissipated
[/quote]

Then it's fully opened. When it's partially (charging gate capacitance it works in linear mode V*I) so 50V * 100A = 50000W) check

As this works as a high side switch gate voltage is Vds + Vgate so around 60-65V depends on IC Vg voltage.

So while Cgate chargers resistance will be huge inside mosfet. Look at the graph (those voltages are Vds + as its working in high side switch) so at 52V (Vds 50V) its resistance is 9mΩ so at like Vgate 10-20V it will be like 20-50mΩ

![00%20PM|338x301](upload://tP4f0yZp4zNAXTqa6p3s58CcHI3.png)

Even our big mosfets was blowing with long rising time so we have to find golden spot for enough current to not kill mosfet and enough time to not burnt it.
```

---
## \#17 Posted by: fedestanco Posted at: 2018-06-07T14:28:58.439Z Reads: 62

```
[quote="Kug3lis, post:16, topic:58033"]
Then it’s fully opened
[/quote]

I believe @Maxid wanted a comparison at normal operating condition (gate at 12v)

[quote="Kug3lis, post:16, topic:58033"]
Even our big mosfets was blowing with long rising time so we have to find golden spot for enough current to not kill mosfet and enough time to not burnt it.
[/quote]

Definitely agree. Real world testing is a must to understand if the design is capable or not to handle specs.
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-06-07T14:31:42.908Z Reads: 66

```
[quote="fedestanco, post:17, topic:58033"]
(gate at 12v)
[/quote]

62V :D

10char
```

---
## \#19 Posted by: fedestanco Posted at: 2018-06-07T14:33:56.522Z Reads: 62

```
lt4356 controls n-side mosfets and uses 12v charge pump at the gate.
Edit: 12v respect to vcc.
```

---
## \#20 Posted by: Kug3lis Posted at: 2018-06-07T14:35:50.172Z Reads: 70

```
High side switching mosfet gate voltage reference is Vds not 0V in case of low side that's why you need charge pump to lift up your source voltage to Vds + Vgate voltage ;)

http://tahmidmc.blogspot.com/2013/02/n-channel-mosfet-high-side-drive-when.html

> Now let’s go back to the high-side drive. Let’s say you apply a voltage of 12V (with reference to ground) to the MOSFET gate. However, when the MOSFET is on, voltage at source is equal to +V. Let’s assume +V is +15V. Now the problem is +12V gate drive (with reference to ground) will not keep the MOSFET on. When the MOSFET is on, the MOSFET source will be at a potential of +15V. To be on, the MOSFET must have +8V VGS minimum. So, if source is at +15V, the voltage at the gate with respect to ground must be at least +23V. If source was at +300V, for example, gate drive would require a minimum of +308V with respect to ground. This is if the gate drive is referenced to ground. If you have a separate isolated power supply whose ground and the ground of the MOSFET-based circuit are isolated, then  you can use that to drive the MOSFET as well.
```

---
## \#21 Posted by: fedestanco Posted at: 2018-06-07T14:39:20.528Z Reads: 62

```
Thanks for explaining. Do you know if there are reliability differences between low side and high side switching?
```

---
## \#22 Posted by: Kug3lis Posted at: 2018-06-07T14:44:10.692Z Reads: 65

```
Don't really remember much difference, just as I have worked with auto/moto industry high side is preferred way because of ground loops/cases and etc. Low-side is the easiest to make as it doesn't need charge pumps and etc. But if you have somewhere ground available is bit pain in the ass because you have to make sure your electronics will not get ground from anywhere else not through communications ports like CAN and etc ;)

Good discusion happening here:
https://electronics.stackexchange.com/questions/188072/difference-between-high-and-low-side-switching-of-power

> For an isolated circuit, no there is no great difference between high and low-side switching. For higher load currents, low side semiconductor switches (for example NPN transistors and N-channel MOSFETs) are often less lossy than their high-side equivalents, and so are preferred.

>However, if the circuit is connected to external devices with their own power connections, this becomes blurred. If these external devices provide a connection to the same ground reference as the power supply to the circuit and you switch this in and out then the external devices will provide an alternate route to ground, your switching will be ineffective and you may end up damaging something not rated for the appropriate current along the way.

> Similarly, if the external devices provide a V+ supply which is referenced to the same ground as the supply that you are switching, you can end up back-powering the positive voltage rail via the externally powered devices, again with undesirable results.
```

---
## \#23 Posted by: fedestanco Posted at: 2018-06-07T14:50:48.489Z Reads: 58

```
Getting back to the precharge discussion, I was thinking that integrating this switch directly on the vesc would have this advantage: we could use the soft-swicth to also enable the drv (and put some delay to enable lt4356). This way we could use drv buck converter to do the precharge of the caps, eliminating the inrush problem when lt4356 wakes up. What do you think?
```

---
## \#24 Posted by: Maxid Posted at: 2018-06-07T15:19:46.651Z Reads: 60

```
I was more concerned with the total footprint than anything else.
6 FETs will need much more space than a single fatboy one. It's also the reason why I don't like the Vedder ones - they are just so huge for what they do. Until @kuglis nobody used the vertical space available (I am obviously talking about use cases where you would not need the aluminium block (in for example low power commuter boards))
```

---
## \#25 Posted by: fedestanco Posted at: 2018-06-07T15:30:01.172Z Reads: 69

```
They are 5 by 6 mm. So 3cm long  when they are placed in line. (max 3.5cm if you space them properly)
```

---
## \#26 Posted by: fedestanco Posted at: 2018-09-09T18:27:32.380Z Reads: 57

```
Update. I have added the precharge function with a cheap and reliable 555 timer. I also made a first pcb draft; the soft switch function has been left out temporarely to achieve a compact design and a single side smt assembly. The whole thing will be open source after testing prototypes. I may also incorporate it into the escalate pcb.

@Maxid I layed out the design in a way that allows the user to cut off one or more mosfets without altering the functionality, like you would do with an LED strip.

![SPARKLING%20SWITCH%20DRAFT|690x427](upload://5C69IRaratvMtbBgxv188cP9lwU.PNG)
![new%20schematic|690x456](upload://2AnoGYMslkmaBybT0ZxuW5fEqc1.PNG)
```

---
## \#27 Posted by: Deodand Posted at: 2018-09-10T16:27:08.723Z Reads: 46

```
I would reccomend independent 10-20 ohm gate resistors for each parallel FET.
```

---
## \#28 Posted by: fedestanco Posted at: 2018-09-10T19:01:48.524Z Reads: 40

```
I assumed that few fets with low gate charge would be equivalent to having a big fet; thus I only placed one resistor. A quick research revealed that I was wrong since the resistor also suppresses the gate oscillation if you have high inductance in the gate trace. Thanks for the tip.
```

---
## \#29 Posted by: Kug3lis Posted at: 2018-09-10T20:28:53.193Z Reads: 37

```
Well its all good if you have switching load, here we have a constant on/off so there will be not much oscillation as it will be always on
```

---
## \#30 Posted by: Deodand Posted at: 2018-09-10T20:51:54.295Z Reads: 30

```
I thought the same, especially with the slow-ish turn on of the gate. But I had some really strange behavior going on with my switch which seemed to disappear when I added individual gate resistors close to each FET and things quit exploding. It isn't much cost or real-estate anyway.
```

---
