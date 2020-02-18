# 12S Series Discharge/ 6S Parallel Charge Power Switch

### Replies: 33 Views: 5259

## \#1 Posted by: dstnceswmer Posted at: 2016-09-01T16:26:18.119Z Reads: 307

```
Hey, so I drew up this design for a power switch for my board running a 12S setup (2x 6s in series). If switch is in one position the packs go to a XT-60 Parallel adapter, but if flipped the other way they are in series and hooked up to the VESC/Battery monitors through a series adapter. I'd like a few second opinions on this design before I go out and implement it. Thanks :)

<img src="/uploads/db1493/original/2X/d/decae847e00f85d5157c28b7e60073a24050785e.png" width="676" height="499">

@JdogAwesome
```

---
## \#2 Posted by: saul Posted at: 2016-09-01T17:27:52.909Z Reads: 271

```
seems really complicated, and really bad if something goes wrong...
why not just get a 12s bms and charge/discharge all on 12s?
```

---
## \#3 Posted by: dstnceswmer Posted at: 2016-09-01T17:35:27.248Z Reads: 263

```
For a few reasons:
1.I'd like to avoid having to unplug the VESC for charging
2. I've Heard that Parallel Charging is preferable over series charging
3. Would like to have a On/Off switch instead of plugging/unplugging wires

It should follow the same basic idea used in @JdogAwesome 's power switch
```

---
## \#4 Posted by: Namasaki Posted at: 2016-09-01T17:35:51.789Z Reads: 252

```
Why do you have a diode between pos and neg?
```

---
## \#5 Posted by: dstnceswmer Posted at: 2016-09-01T17:48:18.721Z Reads: 249

```
It was in @JdogAwesome 's switch, below was his explanation.

http://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738/14?u=dstnceswmer
```

---
## \#6 Posted by: saul Posted at: 2016-09-01T18:06:23.171Z Reads: 230

```
the power switch alone would take care of 1 and 3, and for 2 thats mostly just because cheap rc lipo chargers mostly come in 6s max, so charging in parallel at 6s, is easier than finding a 8s+ charger...
but a bms would take of that.

the thing is, you took something very simple, and solid. and make it it a recipe for shorting lipo/lion packs for rocket powered boards i guess? :joy::head_bandage:

mostly i'm just saying there are easier more reliable ways of getting what you want
```

---
## \#7 Posted by: dstnceswmer Posted at: 2016-09-01T18:22:25.899Z Reads: 223

```
hmm, ok. Could someone please explain to me what a BMS is and how it works? Or point me to some good reading on them?
```

---
## \#8 Posted by: dstnceswmer Posted at: 2016-09-01T19:14:17.155Z Reads: 216

```
Been looking around a bit, so I already have this charger, https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=58285 
If I were to go the BMS route would this be sufficient
 http://www.ebay.com/itm/44V-48V-50-4V-12S-30A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System-/221274094989?_trksid=p2352135.m2548.l4275

Are there any cheaper alternatives? or is this pretty much par for the course?
```

---
## \#9 Posted by: JdogAwesome Posted at: 2016-09-02T04:27:54.327Z Reads: 205

```
Hey @dstnceswmer thanks for tagging me. Your design for a series/parallel adapter is accurate and it would work, though like @saul said, it just kinda over-complicates things. First off you would need to have 2 separate switches on the outside of your board for parallel and series as well as a balance port, and a port for the main charging leads. This would mean that you would have more holes to make, more connections that could break, more areas for water to get into, and just generally more things to go wrong and on EBoards you want it to be as simplistic as possible, I learned this the hard way lol. Im not trying to bash on you or anything im just kinda pointing out some possible flaws with your system. Also where did you hear that parallel charging is better than series? Ive only ever heard that series is better than parallel charging because you need less amperage, but higher voltage, to charge in the same amount of time. I would recommend just using a 12S BMS and having a simple DC jack on the outside to charge the board, I seriously wish I had done that with my board. Having to plug my balancer into the board every time I need to charge it has been INSANELY annoying and has caused many many problems. Having a closed system would be preferable. 

For a BMS you can find them on a ton of different websites, but you may want to contact @longhairedboy about BMS's because he works with them a lot. Also have a look [HERE](http://www.aliexpress.com/wholesale?catId=0&initiative_id=SB_20160901201816&SearchText=12S+BMS) for a ton of different options of BMS's. If you want to use the built in over current protection, which is what the amperage rating is on the listings, you would need to have one of probably at least 30A or more. Though in one of @VladPomogaev videos he just bypassed the over current protection entirely by hooking his switch up directly to the batteries instead of using the two separate terminals on the BMS. Also a lot of times the traces on the BMS are far to small and will melt far before the over current protection kicks in lol. Link to Vlads video about BMS's [HERE](https://www.youtube.com/watch?v=jxHQjlHv1y4)
```

---
## \#10 Posted by: dstnceswmer Posted at: 2016-09-02T04:53:34.402Z Reads: 171

```
Thanks for the great feedback @JdogAwesome! I'm definitely convinced of going the BMS route and just using 1 mosfet and a switch for the Main's power. I'll upload a sketch in the morning. For now though I was thinking of ordering the 
http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html
as it has the 60A max that the VESC will be set at and is rated for 12s since I am running 2x 6s in series. Does this look like it will get the job done? The only issue is long delivery times :( 

 As for the question of parallel charging being better, I'm sorry I don't remember where I read that, my guess is it was referring to an easier way to charge 2 6s packs vs two chargers or something.
```

---
## \#11 Posted by: JdogAwesome Posted at: 2016-09-02T05:17:54.610Z Reads: 163

```
That BMS looks awesome! A little pricey but it definitely looks of good quality and the max over charge is 4.2 instead of 4.35 or whatever some have lol. Also what kind of setup are you planning on running, single drive or dual? And im still selling my MOSFET switches if your interested :wink:
```

---
## \#12 Posted by: JdogAwesome Posted at: 2016-09-02T06:27:07.264Z Reads: 164

```
FYI in your oignal schematic you have a diode also going across the series adapter leads, but you only need one near the MOSFET itself.
```

---
## \#13 Posted by: dstnceswmer Posted at: 2016-09-02T16:16:59.223Z Reads: 172

```
Thanks for the offer on the switches, I wil probably make my own though as all I'd need to buy is the fet (have most of the other supplies I can scavenge from work). Curious though what price are you selling them at?

I am using a single motor setup with https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=36657
Already have it mounted to my truck via an aluminum mount welded. Also just ordered some nice large 97mm wheels to give plenty of ground clearance. I'll prob start a build progress thread where I'll post some pics.

Also I was looking a bit at setups that only uses the BMS for charge, since I can use the VESC for discharge protection. This would hopefully allow me to get a bit cheaper BMS.

Anyways, here is the (hopefully) final schematic (doesn't show the balance leads to the BMS) for a system with a high current (60A) BMS. 
<img src="/uploads/db1493/original/2X/e/ea627668e375ea8ec6020c8cd336c9878fefd1aa.png" width="690" height="485">


And her's one for a lower current BMS used only for charging, with a second Mosfet to bypass the BMS during charging.
<img src="/uploads/db1493/original/2X/1/12860a1a3dc9fdad9adf10ed72e12b06c2ff4751.png" width="690" height="485">
```

---
## \#14 Posted by: saul Posted at: 2016-09-02T19:14:14.416Z Reads: 142

```
Glad you found some better options. 

I have the same motor on 12s and 97mm flywheels.
14t/36t has really good torque. And still hits 24+mph.
```

---
## \#15 Posted by: dstnceswmer Posted at: 2016-09-02T19:24:42.546Z Reads: 140

```
Sweet! I'm looking forward to getting it up and running!
```

---
## \#16 Posted by: saul Posted at: 2016-09-02T19:30:46.048Z Reads: 149

```
Take your time and double check, I rushed a bit oncw I had all the parts, then had to rebuild and fix all the tings I over looked.

Still had fun tho! Till I had to walk it home.. Lol
```

---
## \#17 Posted by: jmasta Posted at: 2016-09-02T21:02:00.084Z Reads: 150

```
Hey, I have been working on something very similar but took a different approach.  I am planning to use a DPDT switch to alternate between 6S charging and 12S discharging.  However, I'm a mechanical engineer... not an electrical engineer.  

I tested the following configuration with AA batteries and a voltmeter to make sure it was hooked up correctly.  I have not yet tried it with Lipos.  I feel like I definitely need to add a flyback diode and perhaps some pull-down resistors?  Can anyone give some insight or suggestions for my design?


<img src="/uploads/db1493/original/2X/0/0b96165343466699e9082c6be309d293d000608b.png" width="690" height="427">

Note:  VESC -> Motor was simplified in this diagram as simply [M].  Balance leads are not shown
```

---
## \#18 Posted by: dstnceswmer Posted at: 2016-09-02T21:18:42.165Z Reads: 131

```
Intuitively that is what I was originally trying to accomplish. However I doubt you'll find a DPDT switch that can handle the High current and voltage of the LiPOs. That is ewhy I tried having my DPDT switch controlling high  power FET's in my first drawing.
```

---
## \#19 Posted by: jmasta Posted at: 2016-09-02T21:29:14.989Z Reads: 143

```
I found a DPDT switch rated to ~2.5 - 2.7 kW, but keep in mind there is an embedded safety factor in this number.  At max load:   44V @ 60A equates to 2.9 kW.  The switch is at least going to have a safety factor of 1.3, so really it should be able to handle 3.3+ kW
```

---
## \#20 Posted by: jmasta Posted at: 2016-09-02T21:32:46.781Z Reads: 143

```
Can you explain your DPDT switch notation?  I don't fully understand your diagram. Thanks!
```

---
## \#21 Posted by: dstnceswmer Posted at: 2016-09-02T21:49:44.043Z Reads: 147

```
Not much of an  official notation on my switch, it's essentially the same as you have drawn, Your pins 2/5 correspond to my poles that I have located on the + connection of each 6s battery. It then toggles between which FET it wants to turn on. Are you familiar with the concept of how a FET works?

Also do you have a link to that switch you were considering?
```

---
## \#22 Posted by: JdogAwesome Posted at: 2016-09-03T06:55:48.267Z Reads: 155

```
@dstnceswmer I was looking at the shcematic you made with the 60A BMS and that one looked pretty good, except for the battery positive lead. Though the one below it is again, over complicating things and could cause some problems. First of all a lot BMS's need an input charge to "turn them on" beofore they will start doing anything, so when you bypass the BMS for charging you effectively disconnect the BMS and that would make it shut down. Also a very small amount of current leaks through the MOSFET, enogh to power maybe an LED but thats it,  though this small leakage ive had measure at different voltages sometimes upto 3V which could cause some undesired affects on the BMS side. It could make the BMS thing that the LiPos are SEVERELY over discharged and it could freak the F out or god knows what lol. Now this is unlikely, obviously, though it could cause problems and as I said over complicates, and creates more possibility for problems. What would be best is to do what @VladPomogaev did and use a low amperage cheap BMS and just hook the battery straight upto the main switch for the board, bypassing the OC protection on the BMS. Below is an example of what I mean: 

<img src="/uploads/db1493/original/2X/7/7b433806fec3ab476347299df15375636774fab8.jpg" width="690" height="413">

Also heres the pricing for my switches:
[quote="JdogAwesome, post:1, topic:5738"]
Prices:
IRFB7530 ~40A Single FET Switch ~$25
IRFB7530 ~80A Dual FET Switch ~$35
IRFB7530-7P ~100A Dual FET Switch ~$40
IRFB7530-7P ~50A Single FET Switch ~$30
FYI I custom make every PCB so if you need it to fit a certain size requirement just ask and ill try to accommodate it to your needs.
[/quote]

P.S. Why are you using 33K Ohm resistors? Just curious if you had a reason, they'll work fine, you can use anything from pretty much ~1K-100K lol.
```

---
## \#23 Posted by: JdogAwesome Posted at: 2016-09-03T07:07:59.167Z Reads: 138

```
Hey @jmasta I kinda understand what you mean in your schematic you drew though the actual image is very confusing sorry. If you could possibly try to highlight certain parts of the schematic and try to make them more obvious and labeled better then I may get a better understanding of what your trying to do. Im not trying to be to harsh or anything just its a little confusing, though you have amazing hand writing lol, if I did something like that it would look like some 5 year old drew it. Also the DPDT switch you said you found that is rated at 2.5-2.7kW but could probably handle around 3.3kW would work kind of,  I wouldn't recommend using it at all. First of all im sure the thing is fricken beafy and would be an eye sore as well as a hassle for fitting in your board. Also when you first start up your board you have to charge the ESC caps and that draws a TON of instantaneous current, which causes that dreaded spark everyone talks about, and your switch might not be able to hand that and could fuse together. Also ever time you start the board the contacts would become oxidized more and more from the spark and would eventually need to be cleaned, which may be very hard in a closed switch. In conclusion I would HIGHLY recommend using either a loop key or a MOSFET switch in order to turn your board on and off. I originally used a PIECE OF CRAP fuse as a switch and it worked at first but over time It just created SOO  many problems for me and I wish I had never used it.
```

---
## \#24 Posted by: saul Posted at: 2016-09-04T00:36:12.300Z Reads: 118

```
that must be a monster switch, doubt it was made to survive the vibration of an esk8.
```

---
## \#25 Posted by: dstnceswmer Posted at: 2016-09-06T17:13:37.275Z Reads: 123

```
So I am going with the 60A BMS, already ordered it. From what I have seen the positive lead from the battery does not get hooked up to the BMS at all, only the negative lead and the balance wires. Below are a couple examples of wiring guides I am referring to. In My 60A BMS schematic I don't see how the FET would leak any current when the switch is off, as the positive battery lead is physically disconnected from the gate of the FET? And the reason I have a 33k res in my switch circuit is to divide the 12s voltage down to around 11V to be appropriate for the Vth of the FET's gate.

<img src="/uploads/db1493/original/3X/2/9/29589a28660c356fdfb266999afa6a332f4ececb.jpg" width="648" height="500">
<img src="/uploads/db1493/original/3X/3/c/3c019ac4f3be984b1688fcb9ae2e6860a001a157.jpg" width="690" height="431">
```

---
## \#26 Posted by: SteveS Posted at: 2016-09-06T18:21:36.288Z Reads: 111

```
For a simple, cheap way to do this, have a look at [url=https://endless-sphere.com/forums/viewtopic.php?f=35&t=75945]what I did[/url].
```

---
## \#27 Posted by: chinzw Posted at: 2016-09-07T16:44:39.017Z Reads: 110

```
I was thinking of having a splitter on the discharge leads, one goes to the VESC and the other to a B6 charger, im guessing the balance charger will act like a bms (minus the discharge protections), that way i can leave everything connected inside the enclosure and just 1 plug to charge. Will add a drawing in a few min

<img src="/uploads/db1493/original/3X/8/8/8899cdb9cec88491327afe2877cbd1e8446cf747.jpg" width="666" height="500">
```

---
## \#28 Posted by: dstnceswmer Posted at: 2016-09-07T19:44:39.234Z Reads: 98

```
So you're just putting the entire charger inside the board's casing? seems kinda like a bulky/heavy solution to 1 port charging. Why not just use a BMS and then a standard bulk charger for charging?
```

---
## \#29 Posted by: chinzw Posted at: 2016-09-07T20:40:00.238Z Reads: 98

```
Not the brick, just the lightweight B6
<img src="/uploads/db1493/original/3X/2/9/2909a080d3b11a3b02cbe9ae8ca77c3742ff0b69.jpg" width="565" height="414">
```

---
## \#30 Posted by: Michaelinvegas Posted at: 2016-09-07T20:50:20.474Z Reads: 100

```
I got this one... Works well...slow ito charge but it's stupid proof...no buttons...seem to charge battery to 25v only but that's perfect for long life
```

---
## \#31 Posted by: chinzw Posted at: 2016-09-07T21:10:38.085Z Reads: 97

```
I wonder if it will be safe to have it connected all the time to the battery and if it will drain some charge over time.
```

---
## \#32 Posted by: dstnceswmer Posted at: 2016-09-07T21:12:05.519Z Reads: 97

```
I was actually wondering the same thing.
```

---
## \#33 Posted by: daym10 Posted at: 2018-06-27T17:25:55.877Z Reads: 27

```
I have an additional question in relation to wiring the power switch at higher voltages as i am looking to do a 12 S or higher on a dual motor setup. I know its totally unnecessary but i was wanting to see if it could be done. Could 2 power swtiches be wired together in either of the following ways:

1: Have two entirely separate systems(independent batteries, power switches, vescs, and motors) and connect them at the power on buttion by combining the two ribbon cables into one button. And Pair the Vescs the normal way.( My thought is that becuase the power to the systems is seperate and the only way that the systems are combined is by the VESCs talking to eachother and the on/off being combined thus preventing overpowering anything and still allowing for a single remote.

2. Can a power switch be wired to act in parallel with another switch and then combine the on/off button, so that although the power coming into the group of switches in larger than 1 of the switches capabilities, the 2 split the power so that it is below the maximum capabilities of the switch.

I hope that i was descriptive enough for the idea to make sense.

Thanks for the help!![Dual%20Motor%20Dual%20VESC%20High%20Voltage|690x137](upload://5RBPQctLkcGHY5NitphDEyoWStN.jpg)
```

---
