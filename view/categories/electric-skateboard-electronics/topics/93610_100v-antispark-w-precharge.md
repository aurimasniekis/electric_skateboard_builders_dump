# 100V Antispark w/ Precharge

### Replies: 109 Views: 1801

## \#1 Posted by: deltazeta Posted at: 2019-05-12T22:26:53.394Z Reads: 269

```
After 3 iterations and far too many dud pcbs, here's a new antispark i hope the community will appreciate.

This started with @b264 and his excellent explanation on why the vedder switch blows. 

https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967?u=deltazeta

In designing this, I had a couple goals:

1. overbuilt current and voltage ratings for eskate
2. as small as possible
3. momentary button

To satisfy goal 1:

* this design uses 175A midi fuse blocks I saw on the DieBieMS.
  * The midi fuse standard allows for much higher currents than the old blade fuses.
* The mosfets chosen are rated for 100V and 260A, doubled up for a theoretical 520A continuous.
  * You'll never be able to get that much current through this design but this removes the mosfets from being a bottleneck in either voltage or current.
* Traces are beefed up with solder to improved current capability across them.
* The 5v regulator is rated for 150V.
* To handle the issue of precharge, the design uses a 10ohm resistor and a small 10A continuous mosfet.
  * This combo is enough for precharging even at 100V.

https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639?u=deltazeta

For goal 2:
* the pcb is shrunk down to a 23mm by 40mm size, restricted by the size of the midi fuse
  * If you don't mind forgoing the fuse, the design can be even thinner. 
* The 2 power mosfets are mounted on opposite sides of the pcb to further minimize the size of the pcb.

With goal 3, I personally couldn't come up with a solution that didn't require a microcontroller, so I ended up with an attiny85 running the show. Honestly could've gone even smaller, but this works great. But as many people have found out, these momentary button designs incur a cost of power drain while off. Luckily @Blasto made a post with an excellent design to disable the 5v regulator while off to minimize power. The 5v regulator used sips 1uA while disabled, which results in less battery degradation than the battery would see just sitting on its own. I didn't have equipment sensitive enough to measure that little of current draw, but I imagine its effectively 0.

https://www.electric-skateboard.builders/t/fatboy-antispark-0-5w-draw/85036/49?u=deltazeta

@Winfly gonna be testing this on the road, so we'll see if anything funny happens

![20190512_142744%5B1%5D|375x500](upload://6J2qKza9lgOAF1Z0J8pekv3JtDS.jpeg) 
![20190512_141722%5B1%5D|375x500](upload://sHpiWmWSsMsa8MtMY3CLToIGUW0.jpeg)
![20190512_141727%5B1%5D|375x500](upload://cKq9IQlSF9ANHhzZOT4a8KNzBY3.jpeg)
![20190512_142702%5B1%5D|375x500](upload://nmmbDmN7fzSrbbavCXN5C3CrDMQ.jpeg)

Thumb for scale
![60024839_2352610271662657_1081237615673344000_n|243x500](upload://vJWBhDhVnGuSszf0HvNUt2D6l6A.jpeg) 

Designs can be found at:
https://easyeda.com/ninetailfox97/fused2

Attiny85 source code:
https://github.com/dzhang97/Antispark

Name suggestions are welcome
```

---
## \#2 Posted by: Vanarian Posted at: 2019-05-12T22:30:47.344Z Reads: 215

```
What a wonderful piece of engineering, I need exactly this. Can you please confirm that it can use a momentary push button and is auto reset to off position when you plug the batteries ?

Edit : Is it press ON / hold OFF?
```

---
## \#3 Posted by: Grozniy Posted at: 2019-05-12T22:31:55.169Z Reads: 211

```
Eagerly awaiting @Winfly review. What will be the price?
```

---
## \#4 Posted by: moon Posted at: 2019-05-12T22:35:14.325Z Reads: 208

```
Thumb switch
```

---
## \#5 Posted by: deltazeta Posted at: 2019-05-12T22:37:45.067Z Reads: 203

```
Yup, uses a momentary push button, no latch required. The switch remains off with or without a battery, until you hold the push button for a set amount of time. I personally selected a 1 second on, and a 1.5 second off, but technically it could be personalized.
```

---
## \#6 Posted by: venom121212 Posted at: 2019-05-12T22:38:22.161Z Reads: 194

```
Name suggestion:
(warning, I have been drinking) 

**ANTI-McSparky**
```

---
## \#7 Posted by: deltazeta Posted at: 2019-05-12T22:41:32.640Z Reads: 195

```
Honestly don't know if I'll sell much of these, which is why the design is released. Its a bit of a pain in the ass to put together due to the smallness. But the bom cost is around $18 without fuse, and $25 with fuse related parts.
```

---
## \#8 Posted by: Winfly Posted at: 2019-05-12T22:41:36.029Z Reads: 189

```
I too am excited to test it. if it works I can ditch my loopkey finally lol. wouldn't mind to help solder a bunch when new PCB comes.
```

---
## \#9 Posted by: sofu Posted at: 2019-05-12T22:43:26.238Z Reads: 189

```
Awesome work David!  Can I suggest:

* D-Switch

* The David Antispark Switch

* The Dwitch

* The Ditch

* The D

man that D looks pretty great 👍
```

---
## \#10 Posted by: brenternet Posted at: 2019-05-12T22:46:05.397Z Reads: 181

```
Call it the Vinegar Stroke
```

---
## \#11 Posted by: bigben Posted at: 2019-05-12T22:49:33.954Z Reads: 178

```
SparkyMcSparkFace?
```

---
## \#12 Posted by: landonkun Posted at: 2019-05-12T22:50:36.340Z Reads: 176

```
Damn, came here to make that joke in reply to @venom121212, but you beat me by a minute.
```

---
## \#13 Posted by: brenternet Posted at: 2019-05-12T22:50:54.200Z Reads: 178

```
Call it Dave.

I mean.. why not?
```

---
## \#14 Posted by: bigben Posted at: 2019-05-12T22:51:48.441Z Reads: 174

```
Simon perhaps?
```

---
## \#15 Posted by: brenternet Posted at: 2019-05-12T22:53:56.583Z Reads: 172

```
YESSS. Call it Simon, or Trevor. Both good.
```

---
## \#16 Posted by: Dirt_Bag Posted at: 2019-05-12T22:54:12.472Z Reads: 168

```
Call it "sparky"


Also, how much for one shipped in usa?
```

---
## \#17 Posted by: landonkun Posted at: 2019-05-12T22:56:32.048Z Reads: 169

```
Then it needs a last name: Belmont.
```

---
## \#18 Posted by: AgressivStreetLamp Posted at: 2019-05-12T22:56:41.566Z Reads: 167

```
Happy to help with manufacture and selling them. Glad to see an alternative to the Vedder. 

As far as the name. 
DZ switch.
```

---
## \#19 Posted by: J_Dizzle Posted at: 2019-05-12T22:57:07.128Z Reads: 171

```
+1 for “Simon”
:yum:
```

---
## \#20 Posted by: brenternet Posted at: 2019-05-12T22:58:26.287Z Reads: 178

```
**Should it be called Simon?**

[poll type=regular results=always public=true]
* Yes
* No (I lick frogs)
[/poll]
```

---
## \#21 Posted by: moon Posted at: 2019-05-12T23:01:13.031Z Reads: 172

```
Don't knock it until you try it
```

---
## \#22 Posted by: AgressivStreetLamp Posted at: 2019-05-12T23:03:21.889Z Reads: 169

```
How are you handling programming the attiny?
```

---
## \#23 Posted by: deltazeta Posted at: 2019-05-12T23:03:47.506Z Reads: 166

```
avrdude on a raspi3
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-05-12T23:03:51.436Z Reads: 163

```
@ARetardedPillow
```

---
## \#25 Posted by: AgressivStreetLamp Posted at: 2019-05-12T23:08:13.834Z Reads: 161

```
Awesome. I have yet to program one but looks like its just SPI and can therefore be done with a number of Interfaces. 
Are you ordering the PCBs in bulk? I'd love to try my hand at assembly and distribution of you need help.
```

---
## \#26 Posted by: deltazeta Posted at: 2019-05-12T23:12:03.569Z Reads: 158

```
So far its just been (ab)using jlc's cheap services to get far more pcbs than i need to test. I'll probably go through them again once the design is finalized.
```

---
## \#27 Posted by: mmaner Posted at: 2019-05-13T00:19:07.031Z Reads: 163

```
I'm gonna go with ASS-S (Anti-Spark Switch Solution) 😀

BTW, great work @deltazeta.
```

---
## \#28 Posted by: M.Hboards Posted at: 2019-05-13T00:35:29.641Z Reads: 164

```
@deltazeta when this switch releases the power to the esc/vesc does is it a soft power release or it is a hard on off like a loopkey?

Reason for my question-

https://www.electric-skateboard.builders/t/remote-reciver-wont-turn-on-when-vesc-turns-on-due-to-anti-spark-switch-please-help/92564
```

---
## \#29 Posted by: deltazeta Posted at: 2019-05-13T00:41:49.491Z Reads: 159

```
The power release will be similar to a loopkey. The precharge circuit is just a 10ohm resistor, like the xt90s' 5ohm resistor. The release will be "hard" compared to mosfet-based methods that ramp the power up, but slightly less hard compared to a loopkey.

Whether or not it will be sufficient to solve your problem is anyone's guess though.
```

---
## \#30 Posted by: M.Hboards Posted at: 2019-05-13T00:43:54.148Z Reads: 153

```
Do you have any other prototypes i could buy/test?
```

---
## \#31 Posted by: deltazeta Posted at: 2019-05-13T00:47:33.414Z Reads: 156

```
Not currently, but soon™
```

---
## \#32 Posted by: M.Hboards Posted at: 2019-05-13T00:48:40.458Z Reads: 155

```
Please put me on the list for when they are availible!
```

---
## \#33 Posted by: Gamer43 Posted at: 2019-05-13T01:14:01.572Z Reads: 155

```
Oh dam i have sum competition. XD good work.
```

---
## \#34 Posted by: pixelsilva Posted at: 2019-05-13T01:51:55.296Z Reads: 148

```
**Dee-Zee Anti-Spark**
```

---
## \#35 Posted by: b264 Posted at: 2019-05-13T03:13:49.042Z Reads: 148

```
[quote="deltazeta, post:1, topic:93610"]
With goal 3, I personally couldn’t come up with a solution that didn’t require a microcontroller
[/quote]

I have also attempted this, and also failed to succeed in a way to design this without an MCU.  I feel like a certain combination of flip-flops and comparators should be able to do this, but I never came up with a way, especially after you add 50ms (on) and 2700ms (off) debouncing.  (the latter in case debris hits the power switch)
```

---
## \#36 Posted by: b264 Posted at: 2019-05-13T03:18:08.280Z Reads: 142

```
[quote="deltazeta, post:5, topic:93610"]
I personally selected a 1 second on, and a 1.5 second off
[/quote]

I'd recommend 50ms / 2700ms
```

---
## \#37 Posted by: AlanZhou Posted at: 2019-05-13T03:18:32.929Z Reads: 140

```
Can you at least offer a normal person translation pls 😂
```

---
## \#38 Posted by: b264 Posted at: 2019-05-13T03:19:12.620Z Reads: 146

```
[quote="AlanZhou, post:37, topic:93610"]
Can you at least offer a normal person translation
[/quote]

https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967/4?u=b264
```

---
## \#39 Posted by: AlanZhou Posted at: 2019-05-13T03:20:04.124Z Reads: 145

```
Well I understand that part lol 🤣
```

---
## \#40 Posted by: deucesdown Posted at: 2019-05-13T04:46:19.494Z Reads: 147

```
[quote="deltazeta, post:1, topic:93610"]
The mosfets chosen are rated for 100V and 260A, doubled up for a theoretical 520A continuous.
[/quote]

[quote="deltazeta, post:7, topic:93610"]
bom cost is around $18 without fuse, and $25 with fuse related parts.
[/quote]

Could use just one MOSFET for some savings?

The Wurth screw terminal for fuse are from DieBieMS BOM? They're awesome but $4 per piece, and I think they have to be press fit into pcb using special equipment? I wonder if there's a cheaper and easier for DIY screw terminal.

Very nice, thanks for posting!
```

---
## \#41 Posted by: deltazeta Posted at: 2019-05-13T04:55:52.040Z Reads: 144

```
Almost 3s seems like a long button press just to turn off the switch.... 
The firmware handles debouncing but I wouldn't know how well it performs without randomly throwing rocks at the switch.
```

---
## \#42 Posted by: deltazeta Posted at: 2019-05-13T04:56:35.428Z Reads: 141

```
More options is more better :muscle:
```

---
## \#43 Posted by: b264 Posted at: 2019-05-13T04:57:18.293Z Reads: 144

```
Then make it a little less, the point is hold-to-turn-off so if debris hits the switch it's very, very unlikely to be misinterpreted as a powerdown instruction.

My bicycle lights feel like they are about 50ms/2500ms

You could always try 50ms/1500ms
```

---
## \#44 Posted by: b264 Posted at: 2019-05-13T05:00:36.673Z Reads: 141

```
You could name it skaltch
```

---
## \#45 Posted by: deltazeta Posted at: 2019-05-13T05:01:45.387Z Reads: 143

```
I specced the terminal holes according to the spec sheet and it fit no problem. I haven't looked into other options, but I'm sure there are some likely at lower current ratings. A single MOSFET is probably sufficient, many ways to strip down the bom cost. You could even just ignore the fuse entirely and just solder wire across :stuck_out_tongue:
```

---
## \#46 Posted by: b264 Posted at: 2019-05-13T05:02:59.516Z Reads: 140

```
I agree with you @deucesdown but I think getting a version that works well should be the first priority, then slimming down a lesser version for college budgets should be the second priority.  A "toy" and a "tool" model :rofl:
```

---
## \#47 Posted by: deltazeta Posted at: 2019-05-13T05:06:35.312Z Reads: 141

```
It's 1000ms/1500ms now, but only because I have the precharge time tied to the on timer. Can be easily modified for user preference. To be honest I'd be very surprised debris is going to hold the button down continuously for more than 1.5s.
```

---
## \#48 Posted by: linsus Posted at: 2019-05-13T08:01:28.248Z Reads: 140

```
Can't find Ron anywhere.. feels pretty important
```

---
## \#49 Posted by: Gamer43 Posted at: 2019-05-13T08:15:10.579Z Reads: 139

```
Oh, have you had a chance to look at my design? It automatically turns on the primary MOSFETs onces the capacitors are adequately charged.

I really like how you fit everything in such a small size, I have yet to do that xD.
```

---
## \#50 Posted by: b264 Posted at: 2019-05-13T08:37:49.624Z Reads: 137

```
[quote="Gamer43, post:49, topic:93610"]
automatically turns on the primary MOSFETs onces the capacitors are adequately charged
[/quote]

I really like that.
```

---
## \#51 Posted by: Acido Posted at: 2019-05-13T10:35:25.350Z Reads: 134

```
At that prices you will, even if they fail lol

Definetley interested :D
```

---
## \#52 Posted by: janpom Posted at: 2019-05-13T15:15:08.111Z Reads: 129

```
[quote="brenternet, post:13, topic:93610"]
Call it Dave
[/quote]

:face_with_monocle:
```

---
## \#53 Posted by: brenternet Posted at: 2019-05-13T15:17:08.632Z Reads: 127

```
Oh here he comes to patent troll. Typical
```

---
## \#54 Posted by: janpom Posted at: 2019-05-13T15:21:28.881Z Reads: 128

```
[quote="mmaner, post:27, topic:93610"]
I’m gonna go with ASS-S (Anti-Spark Switch Solution)
[/quote]

Brilliant idea. Since the BOM is not too expensive, it could just as well be Cheap ASS-S. I think it would work great with the Cheap FOCer, making a Cheap ASS-S FOCer combo.
```

---
## \#55 Posted by: banjaxxed Posted at: 2019-05-13T15:21:46.730Z Reads: 131

```
Do it to it Brent 😂
![image|240x135](upload://3TtGx6ExdBUfHKXyuCuQuqeVsha.gif)
```

---
## \#56 Posted by: Battosaii Posted at: 2019-05-13T15:28:29.810Z Reads: 131

```
Introducing the Anti-Dave
```

---
## \#57 Posted by: sofu Posted at: 2019-05-13T15:35:20.731Z Reads: 128

```
What about Sparklet or Sparkler?
```

---
## \#58 Posted by: Vanarian Posted at: 2019-05-13T15:50:26.662Z Reads: 128

```
Why not call it Negan or Lucille ?
One badass name for one badass thing.


https://giphy.com/gifs/rick-springfield-FOJJ7faKeAafS
```

---
## \#59 Posted by: AgressivStreetLamp Posted at: 2019-05-13T15:53:13.185Z Reads: 127

```
For the momentary function, my Logic Design class taught me something very simple, given any logical function, it the the question is "can we do it?" The answer is always: "Yes but how?"

Found this simple little guy. The term "Soft latch switch" brings up a number of.possibilites. I however do not see a switch in the current design and have not yet modeled it or found time to mess with the original design. So I am unsure where and how to implement a switch, of any kind, in your design

http://www.mosaic-industries.com/embedded-systems/microcontroller-projects/electronic-circuits/push-button-switch-turn-on/latching-toggle-power-switch

![Screenshot_20190513-084857|236x500](upload://8q7IHqzp8U94GKfCdLhKgrif0bQ.jpeg)
```

---
## \#60 Posted by: linsus Posted at: 2019-05-13T16:13:05.135Z Reads: 121

```
Problem with that design in your picture is that its not meant for high power applications. Last figure in the link looks most promising but its alot of components..
```

---
## \#61 Posted by: AgressivStreetLamp Posted at: 2019-05-13T16:14:46.204Z Reads: 117

```
This would just be to turn the FETs on and off. Shouldn't really need to be high power specific?
```

---
## \#62 Posted by: linsus Posted at: 2019-05-13T16:25:54.587Z Reads: 115

```
I thought you wanted to use that circuit to supply the ESC. driving gates makes more sense.
```

---
## \#63 Posted by: AgressivStreetLamp Posted at: 2019-05-13T16:28:53.373Z Reads: 117

```
At lunch, I will see with what I can come up with for integrating this logic into the DZ switch.
```

---
## \#64 Posted by: Vanarian Posted at: 2019-05-13T17:39:09.559Z Reads: 117

```
Whatever you come up with, just make it work and keep two spares for me guys :beers: 

Let's spread that thing. It's been missing from DIY scene for waaaaaaay too long.
```

---
## \#65 Posted by: b264 Posted at: 2019-05-13T19:01:20.248Z Reads: 117

```
The other problem is you will need two bits of memory, not just one bit like that circuit has.

* device on or off?
* precharging or discharging?

So at a minimum you'd need two of those wired up in a convoluted way.  Likely with a couple comparators and a couple voltage dividers to get the signals under 5 volts.
```

---
## \#66 Posted by: deltazeta Posted at: 2019-05-13T19:41:26.990Z Reads: 111

```
Yeah! I did see your design, it was really quite an ingenious way to leverage analog logic like that. I considered how to borrow your techniques for a momentary switch based design but never quite figured it out.

This is the 3rd iteration of the pcb, used to be a bit bigger :stuck_out_tongue:. Needed to make it small to fit the eboosted vanguard enclosure, everything felt a bit too cramped.
```

---
## \#67 Posted by: deltazeta Posted at: 2019-05-13T19:45:09.260Z Reads: 109

```
I was on that page for so long when I was initially brainstorming :dizzy_face:. But as @b264 mentioned, it's a bit weird trying to get a precharge circuit in there, but more of my lack of expertise than anything. I also give up due to the sheer number of components needed.
```

---
## \#68 Posted by: Acido Posted at: 2019-05-13T19:57:55.179Z Reads: 103

```
The guy from 3d servisas made it with i think less then 10 parts or something maybe take a look at his
```

---
## \#69 Posted by: AgressivStreetLamp Posted at: 2019-05-13T20:15:38.302Z Reads: 105

```
So what exactly is the drawback to having the microcontroller? It doesn't have to be icp, except on debug boards. Once everything is tried and tested, there's no reason not to omit the header. Sounds to be like attiny is the simplest solution. Maybe I misunderstood, I'm working under the assumption that you are trying to replace the microcontroller.
```

---
## \#70 Posted by: deltazeta Posted at: 2019-05-13T20:17:18.884Z Reads: 105

```
nah, an mcu works for me. replacing it is more of a brain teaser at this point.
```

---
## \#71 Posted by: AgressivStreetLamp Posted at: 2019-05-13T20:22:02.628Z Reads: 104

```
Gotcha, I spent lunch thinking this over and the controller actually adds a ton of flexibility. Integration with other microcontrollers, choice of pretty much every type of switch. Temp sensor etc. All of it just a firmware patch away.
The reason I'm so interested is I'd like to use a teensy controller to control various components via nfc. This makes it more interesting.

Thenet me ask this, any reason **not** to order a set of PCBs and components as per your design, right now?
```

---
## \#72 Posted by: deltazeta Posted at: 2019-05-13T20:31:55.814Z Reads: 107

```
haha, yeah possibly adding roll to start in the future (maybe @Gamer43 could help), and idle time out would be easy with the mcu. I'm mainly holding off on "production" to really make sure it works. With the vedder/fechter antispark known to last for anywhere from 1 min to several months before randomly dying, really want to be thorough. I've been overconfident with my design before :stuck_out_tongue:
```

---
## \#73 Posted by: Gamer43 Posted at: 2019-05-14T02:48:45.163Z Reads: 105

```
_555 Timer_


Also, roll-to-start and auto turn off will require high side switching. This can be done using a photovoltaic optocoupler or the LTC700x series of MOSFET drivers. I use the LTC7004. The LTC7000 is a 150V version if you want higher voltage ratings. This solution will opt for dV/dt inrush current limiting instead of precharge, only two passive components as opposed to multiple active components and a dozen passive components. There are many datasheets and application notes from multiple big semiconductor manufacturers that recommend the dV/dt limiting method.

What really sucks though, is the STM32L0 has a maximum supply voltage of 3.6V, while the LTC700x VCC UVLO kicks in at ~3.5V D:<. Have to go with a crappy attiny85 or an expensive 5v low power MCU, or bite the bullet and add a 3.3V LDO (and another three components reeee).

The LTC700x is better to use than a photovoltaic optocoupler, more stock available and easier to design around.
```

---
## \#74 Posted by: deltazeta Posted at: 2019-05-14T07:35:43.439Z Reads: 104

```
so a mosfet driver allows an n-channel fet to switch high-side?
```

---
## \#75 Posted by: Gamer43 Posted at: 2019-05-14T07:48:41.675Z Reads: 104

```
Yes, it has an integrated charge pump to support 100% duty cycle.

The downside is that the chip is $4 in single quantity.
```

---
## \#76 Posted by: deltazeta Posted at: 2019-05-14T07:50:00.616Z Reads: 105

```
well shit that changes everything...:star_struck:
```

---
## \#77 Posted by: deltazeta Posted at: 2019-05-14T07:50:37.986Z Reads: 100

```
but can't i just have the fet driver go full on or off and keep the precharge circuit? Seems more reliable imo
```

---
## \#78 Posted by: Gamer43 Posted at: 2019-05-14T07:51:44.036Z Reads: 101

```
Precharge has to move to high side along with the primary MOSFETs. It requires two transistors, a zener diode, and a bunch of passive components.

If an RC circuit works good enough, screw precharge. Details of the method can be found in the LTC7004 datasheet, page 9, no I lied, page 11.
```

---
## \#79 Posted by: deltazeta Posted at: 2019-05-14T07:54:45.073Z Reads: 103

```
hmm, I'll see what I can do...

I'm not too familiar with using fets as resistors, but the better the Rdson is, the worse the soa region.
```

---
## \#80 Posted by: Gamer43 Posted at: 2019-05-14T07:58:01.766Z Reads: 107

```
If you really want precharge, use an appropriately sized P-channel MOSFET. It can be driven by an MCU using a level shifting N-channel MOSFET. Add zener diode and appropriate pullup and current limiting resistors accordingly.

The RC circuit controls the dV/dt slew rate and limits the inrush current to a constant value. The power dissipated in the MOSFETs is limited accordingly and decreases as the capacitors charge. Now the design consideration is to ensure power dissipation does not exceed the maximum rating of the MOSFET, i.e. SOA.

Rise time is now fixed and can be calculated (or user determined) easily.
```

---
## \#81 Posted by: deltazeta Posted at: 2019-05-14T08:08:22.162Z Reads: 99

```
Yeah I've looked into that one before, but as you said, its a bit of a hodgepodge of components just for a precharge.

If the RC circuit is based on dV/dt, wouldn't a significant change in capacitance or inductance adversely effect the current? Isn't this what vedder/fechter did in the original design, albeit with only passive components?
```

---
## \#82 Posted by: Gamer43 Posted at: 2019-05-14T08:09:38.037Z Reads: 99

```
Yes, you're right. It means there is a certain capacitance that will make it fail, so we'd have to design for worst case, i.e. maximum capacitance the switch would encounter, smaller capacitances will not be a problem.

And no, the original Vedder switch did not do this, or at least, not properly.

I have already tested this on a switch of my own. A pair of IPB014N06N have survived several cycles charging up to 6mF capacitances.
```

---
## \#83 Posted by: deltazeta Posted at: 2019-05-14T08:16:29.390Z Reads: 92

```
https://endless-sphere.com/forums/viewtopic.php?t=40142&amp;start=100

According to fechter's original design, I'd say they were using this technique, and with properly selected components it would work.
```

---
## \#84 Posted by: deltazeta Posted at: 2019-05-14T08:18:06.584Z Reads: 97

```
hmm, sounds good, what values are you using?

also does the slew rate maintain a constant dV/dt? that fet is restricted to fairly low current initially at full voltage difference
```

---
## \#85 Posted by: Gamer43 Posted at: 2019-05-14T08:21:19.595Z Reads: 101

```
Hmm, looks like it does actually, not sure why those explode and mine haven't yet :man_shrugging:

I used 20k and 1uf, really should be 200k and 100nf. The rise time is actually significantly longer on mine because the bootstrap capacitor is only 2.2uf, maybe that's why mine haven't exploded yet? I have two, one in a mountainboard and another in a scooter.

Yes the dV/dt is constant, this also means the inrush current is constant during the charging process.
```

---
## \#86 Posted by: deltazeta Posted at: 2019-05-14T08:25:56.878Z Reads: 105

```
ok, I guess as long as the rise time is significantly long enough, there's minimal risk to the mosfet. At 60V across the fet, looks like you're limited to .1A, so under that constant current should be 100% safe. You'll probably have a bit more headroom at 50ish volts anyways.

It would be cool to see a rise time graph if you can manage one, real world data is always better than simulations.

I'll think about these ideas for a v2 probably, if the current design works for what it is, no reason to scrap it.
```

---
## \#87 Posted by: M.Hboards Posted at: 2019-05-24T00:56:46.042Z Reads: 99

```
@deltazeta of possible do you mined linking me to a 18mm push button that would work for your switch thanks.
```

---
## \#88 Posted by: deltazeta Posted at: 2019-05-24T01:05:43.945Z Reads: 97

```
A bit bulky but cheap af:
https://www.aliexpress.com/item/32676085681.html?spm=2114.search0604.3.9.2dc35d5cHHFllv&amp;ws_ab_test=searchweb0_0%2Csearchweb201602_4_10065_10130_10068_10890_10547_319_10546_317_10548_10545_10696_453_10084_454_10083_10618_10307_537_536_10059_10884_10887_321_322_10103%2Csearchweb201603_53%2CppcSwitch_0&amp;algo_expid=89f31226-47b6-411e-9171-5db0043a523f-1&amp;algo_pvid=89f31226-47b6-411e-9171-5db0043a523f
a lot more expensive, but probably as small as this switch design goes:
https://www.digikey.com/products/en/switches/pushbutton-switches/199?k=pv6
```

---
## \#89 Posted by: M.Hboards Posted at: 2019-05-24T01:13:26.156Z Reads: 95

```
The digikey link had a vic bunchof different switches would any of those work?
```

---
## \#90 Posted by: deltazeta Posted at: 2019-05-24T01:15:03.811Z Reads: 93

```
yup <del><del>
```

---
## \#91 Posted by: M.Hboards Posted at: 2019-05-24T01:16:58.956Z Reads: 96

```
Also where are the Gerber files? In the easy eda link? This Is my first time doing anything like this so I'm just trying to understand as much as i can before i attempt to make one.
```

---
## \#92 Posted by: deltazeta Posted at: 2019-05-24T01:20:09.674Z Reads: 100

```
For now they'll be in the easyeda link. You'll have to open the design in the online editor and export the gerber files. I can provide the gerbers separately later, once I know I won't need to change the design again.
```

---
## \#93 Posted by: oiitsjamesmate Posted at: 2019-05-26T04:08:14.030Z Reads: 97

```
Keen to make one of these as soon as its finalized. Excellent design.
```

---
## \#94 Posted by: Hanok Posted at: 2019-05-27T02:49:03.740Z Reads: 93

```
The circuit looks good.
Can the circuit be used personally?
![image|690x388](upload://3oW34DLUNHQkZL7B1KoPSQsfQly.png)
    ![image|690x388](upload://8SITtKDW9STiyzTjRmbhGayEPmy.png)
```

---
## \#95 Posted by: deltazeta Posted at: 2019-05-27T02:52:05.898Z Reads: 91

```
Wow looks great! Did you integrate it onto a dual vesc?
```

---
## \#96 Posted by: Hanok Posted at: 2019-05-27T02:54:05.722Z Reads: 92

```
Yeah, I'm trying to make vesc 6 plus dual.
```

---
## \#97 Posted by: deltazeta Posted at: 2019-05-27T02:58:43.225Z Reads: 94

```
Nice, that would be awesome! I'll be working on a roll to start version, so maybe you can make a vesc 6 unity competitor
```

---
## \#98 Posted by: Hanok Posted at: 2019-06-01T15:37:36.616Z Reads: 82

```
What is the part of the Q3?
I don't think it's 2N7000.
```

---
## \#99 Posted by: deltazeta Posted at: 2019-06-02T07:17:36.571Z Reads: 79

```
You are completely right, let me fix some of the mis-label components...
```

---
## \#100 Posted by: dareno Posted at: 2019-06-02T07:44:02.458Z Reads: 75

```
You on the news yet my friend?  Theres a discussion going about this very thing.  Love your input.
You join you retain regular status.
```

---
## \#101 Posted by: deltazeta Posted at: 2019-06-02T07:54:40.115Z Reads: 76

```
I'll make an update there once something major happens, stuck in limbo while I deal with moving, etc.
```

---
## \#102 Posted by: dareno Posted at: 2019-06-02T08:21:16.722Z Reads: 77

```
We need you!  As far as I'm aware you have the only real solution because every other clever bugger is concentrating on bigger things but this is something that has gone overlooked for too long.  Safe switching.  Pretty fundamental.  Good luck with the move brother its a bitch.
```

---
## \#103 Posted by: ARetardedPillow Posted at: 2019-06-02T08:30:04.295Z Reads: 79

```
I'm pretty sure there's a whole army lurking on this thread, me included. 
Been lurking for months now, ever since that thread in December

Waiting for this to become a reality :wink:
```

---
## \#104 Posted by: Hanok Posted at: 2019-06-02T11:53:25.914Z Reads: 73

```
Can you give me the name of the part?
```

---
## \#105 Posted by: deltazeta Posted at: 2019-06-02T16:15:17.123Z Reads: 69

```
https://www.mouser.com/ProductDetail/771-BUK9875-100A-CUX
```

---
## \#106 Posted by: Fungineers Posted at: 2019-10-29T07:22:25.558Z Reads: 48

```
so what happened here. Did anyone test the original DZ? Does it work? Can we build it (final BOM, Gerber)? Can we buy it?
```

---
## \#107 Posted by: deltazeta Posted at: 2019-10-31T01:34:01.147Z Reads: 39

```
Sorry for the late response, but I don't really check this forum anymore, almost always on 

@Winfly took my switch and hasn't done anything with I think :upside_down_face: so honestly i can't say it's been heavily tested. I am planning on making a batch once I get it back from him tho.
```

---
## \#108 Posted by: ZackoryCramer Posted at: 2019-10-31T04:31:46.920Z Reads: 34

```
[quote="deltazeta, post:105, topic:93610, full:true"]
https://www.mouser.com/ProductDetail/771-BUK9875-100A-CUX
[/quote]

I don't think you should use that. Especially if not in parallel. The fet has an Rds resistance of 72mohms. That's way too high. Imaging pushing only 30amps through it. 30^2*0.072=64.8W You are not gonna get away without a huge heatsink.
```

---
## \#109 Posted by: deltazeta Posted at: 2019-11-03T08:30:39.358Z Reads: 26

```
Ah but that's only for the precharge, which has a 10ohm resistor to limit current. The main fets have an on resistance of 1.5mohms, and with two in parallel you get .75 mohms of resistance.
```

---
