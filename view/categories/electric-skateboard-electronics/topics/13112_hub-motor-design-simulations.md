# Hub Motor Design Simulations

### Replies: 134 Views: 8292

## \#1 Posted by: KMeyerson Posted at: 2016-11-15T19:22:50.280Z Reads: 378

```
Hello All,

I'm here to bring forward some simulation data on the available hub motors.  These simulations assume that the VESC is a Sinusoidal, Space Vector Modulation @ 6 Khz or 20Khz.  I am going to present the information available for @Hummie  and @jacobbloy's  hub motor designs. Because of the limitations of the software I am using, I cannot simulate their temperatures.  That said, the temperatures I do simulate do not account for passive air cooling through vents or shaft/hangar heat sinks (@EnertionSupport).

Target RMS Current is 30Amps for these simulations. I do account for the voltage difference between Jacobs (10s) and Hummie's (12s).  I ask that everyone STOP TALKING ABOUT KV.  Focus on Temperature and Torque because those are the variables we need to be more careful about - not speed! Scaling can happen later. If you can respect that, then please add your commentary.

I'll update this as I get around to it. If people want me to produce more accurate results, I do not have any version of Hummie's motors so please tell me the specs.

## Jacob's V2 Motors (24 Pole, Wye)

[quote="jacobbloy, post:757, topic:4762, full:true"]
0.19mm (36 gage) wire... strand count should be between 18 and 23... 8 turns... 0.480ohms per phase.
[/quote]

6Khz SVM Freq.
<img src="/uploads/db1493/original/3X/7/e/7e3e03c573f64c5f0d25544fe666971a7584e6a4.png" width="584" height="500">
20Khz SVM Freq.
<img src="/uploads/db1493/original/3X/4/4/44fb316888237c33b36aa7773efda199e7bd8daf.png" width="581" height="500">

Winding Specs.
<img src="/uploads/db1493/original/3X/3/6/36d29553b779ec508a3cf58b3b79e8744570dc89.png" width="563" height="500">
<img src="/uploads/db1493/original/3X/8/6/86101fe11a174f532f5e829cc54fa662aa4a7839.png" width="527" height="500">

## Hummie's V2 Motors (12 Pole, _Wye????_, 80 kv)

[quote="Hummie, post:229, topic:1002"]
80kv have 33 turn and the 90kv have 30 turns.  Single strand.
[/quote]
I interpert this to mean that his 80 kv model is 24.25 Awg, 1 Strand, 33 Turns.

6Khz SVM Freq.
<img src="/uploads/db1493/original/3X/a/7/a732a7bd4a92c422f62e731849073874a2ecd473.png" width="583" height="500">

20Khz SVM Freq.
<img src="/uploads/db1493/original/3X/c/2/c23b4603cce8d177af24abad538f286cb4dacd5d.png" width="583" height="500">

Winding Specs.
<img src="/uploads/db1493/original/3X/0/1/01c91954b2b2d4243bfa292a7b6bb55fe6826933.png" width="555" height="500">
<img src="/uploads/db1493/original/3X/7/4/748ac5b6f1ecd8536f606c8692b1090c9de0f045.png" width="638" height="500">

## Hummie's V2 Motors (12 Pole, _Wye????_, 90 kv)

[quote="Hummie, post:229, topic:1002"]
80kv have 33 turn and the 90kv have 30 turns.  Single strand.
[/quote]
I interpert this to mean that his 90 kv model is 24.75 Awg, 1 Strand, 30 Turns.

6Khz SVM Freq.
<img src="/uploads/db1493/original/3X/0/c/0c83d7ea44ef7ca9340ba5ae8785291c60603ee5.png" width="582" height="500">

20Khz SVM Freq.
<img src="/uploads/db1493/original/3X/4/6/4603abd2a4fb48622e84779e6ca2de9c3104a86f.png" width="582" height="500">

Winding Specs.
<img src="/uploads/db1493/original/3X/c/e/ce3504189bc1c09d1fdc1f3ea377f813ffc62565.png" width="565" height="500">
<img src="/uploads/db1493/original/3X/5/3/539c3a06cb7e47026e37d4af8ee15d6b7ffb3e38.png" width="637" height="500">

## Hummie's V2 Motors (12 Pole, _Wye????_, 100 kv)

[quote="Hummie, post:363, topic:1002"]
27 turns and 100kv.
[/quote]
I interpert this to mean that his 100 kv model is  Awg, 1 Strand, 27 Turns.

6Khz SVM Freq.
<img src="/uploads/db1493/original/3X/3/e/3e7dc1cf3a4da66bb68cabf48735c65a8ae0d4e4.png" width="585" height="500">

20Khz SVM Freq.
<img src="/uploads/db1493/original/3X/b/5/b5deaa82b0a23e8bd24a2f5e1945f93c729cf96c.png" width="584" height="500">

Winding Specs.
<img src="/uploads/db1493/original/3X/9/7/975202b2b0ddd2edb4469a2f514e1a18a7ecd3fe.png" width="565" height="500">
<img src="/uploads/db1493/original/3X/e/9/e9be35d5fb6ed8a785bb1b4c5d977da7b2d73a2b.png" width="638" height="500">

## Reference:

VESC:
Sinusiosal SVM
20,000hz switching

Torque for 80mm Wheel to stall/equal to gravity with a 100kg load:
05% - 3.9Nm total (or 3.9/2 Nm per motor)
10% - 7.8Nm total
15% - 12Nm total
20% - 15Nm total
25% - 19Nm total

RPM/Speed for 80mm Wheel:
0560 - 05 mph / 8.1 kmh
1100 - 10 mph / 16 kmh
1600 - 15 mph / 24 kmh
2100 - 20 mph / 32 kmh
2700 - 25 mph / 40 kmh

For the same max current, Jacob's Hubs are superior.  That does not mean that they are without fault. The losses are significantly lower however.
-KM
```

---
## \#2 Posted by: Pedrodemio Posted at: 2016-11-15T19:51:01.404Z Reads: 287

```
Amazing data, the program you use is specifically made for simulating motors or just a FEA with your own modeling? 

i read in another thread that you are developing your own hub's that are simulation optimized, any more info on that? any idea when they will become available?
```

---
## \#3 Posted by: johnny_261 Posted at: 2016-11-15T19:58:25.610Z Reads: 282

```
I have no idea what any of this means, but looks cool!  Maybe at some point, you can give the "for dummies" run down at some point of your findings!
```

---
## \#5 Posted by: KMeyerson Posted at: 2016-11-15T20:06:23.014Z Reads: 277

```
This is MotorSolve by Infolytica. Its designed to simulate BLDC motors, a real handy program but its hard to get a hold of. University IT people might help get an EDU discount, but its about $500-700 a copy. Very useful tool though if you're planning to build motors.

I am building my own motors and also an ESC specifically for them. If and when they get to market, they would be released as a set because the drive signal would not be SVM but Current Hysteresis.  This allows me to have better control over the motors temperature and torque.
```

---
## \#6 Posted by: KMeyerson Posted at: 2016-11-15T20:08:19.779Z Reads: 259

```
Compare the Torque of each model's graph to the RPM,
Compare the Current of each model's graph to the RPM,
Compare the Efficiency too.

Thats the simplest way to compare them.

Changed by 10 char to make this a reply
```

---
## \#7 Posted by: Hummie Posted at: 2016-11-15T20:18:42.822Z Reads: 242

```
This is a simulation based on assumed resistance and inductance numbers and the simulation doesn't take into account magnet strength, air gap, and permeability of the back iron which will affect the inductance of the whole motor beyond the winding 
What size stators are they in the simulation?
I can give u real inductance and resistance numbers when I plug back in the vescs as I forget the numbers but there are other variables
```

---
## \#8 Posted by: KMeyerson Posted at: 2016-11-15T20:25:26.496Z Reads: 259

```
False, it does take all of that into account. These are finite element simulations. I have been working from the specs I have found online and have been shared by you.

Here is an example from your 80 kv design, I only changed the winding between these simulations.  I have done my best to recreate your designs. I have Jacobs and can verify the accuracy of these simulations. I cannot accurately represent yours without a sample.

## Full Hummie Motor Specs

<img src="/uploads/db1493/original/3X/d/a/da114804508053d553a18c3fe0a414ae756e0252.png" width="690" height="345">
<img src="/uploads/db1493/original/3X/5/2/522b0a8689704b6da326b572068cdcbfafab1c0a.png" width="690" height="299">
<img src="/uploads/db1493/original/3X/4/6/46949740a5f3527b5db32ef70f42a887920b953a.png" width="690" height="372">
<img src="/uploads/db1493/original/3X/5/c/5c98df74d280ffb8313f3320d83b00e28b1577fb.png" width="549" height="500">
<img src="/uploads/db1493/original/3X/4/e/4e925e393beecb34160252138ab968277d2c7e8c.png" width="690" height="479">
<img src="/uploads/db1493/original/3X/a/4/a4df90593dd27f706f0137093f0d41006c44e36a.png" width="690" height="480">
<img src="/uploads/db1493/original/3X/6/0/603a9d7e0d9d47472f97de8345d7dcc3e875d6bc.png" width="690" height="399">
<img src="/uploads/db1493/original/3X/e/1/e1990752a5021b915909f5a508762733cfa40d1f.png" width="690" height="406">
```

---
## \#9 Posted by: Hummie Posted at: 2016-11-15T20:29:00.483Z Reads: 223

```
You can't know the inductance in the airgap without knowing the airgap width, magnet strength and the permability of the back iron. The winding inductance is just one side of the gap and the other will affect it hugely. No?  It might as well be iron less in this simulation. You could compare iron less to a huge back iron and get the same numbers here but have drastically different performance in the motors
```

---
## \#10 Posted by: KMeyerson Posted at: 2016-11-15T20:38:11.960Z Reads: 241

```
It's specified in the above specifications. Jacobs was 0.1mm. Yours was somewhere between 0.5 and 0.1mm as I recall. I specified the magnet materials as Neodymium Iron Boron 38/15 which translates to N35 (Remember, there is no N52 magnet that is rated to survive 200*C. N35s have that rating.). Iron losses can also be calculated from the 0.2mm laminations of M-19 29Ga silicone steel. I did not include simulations with losses because it would distort the graph in an attempt to display the kW losses (apparently the rubber-melting heat can be identified my friend).

I am not here to attack you, but I need you to help me out here. I can help Jacob patch up his motors to some degree with the CAD and numbers I already have from him. I have none of yours so I've had to speculate based off an old schematic you released (and have continued to use, just with varying winding):

<img src="/uploads/db1493/original/3X/8/7/876918b1908b6c10d61b6c4db7bd3a6753b5b820.png" width="666" height="500">

I have reached out to you before to get official specs so I could crunch numbers. As you told me, the majority of your electromagnetic work is being done by a company and not by you (determining the windings, for example) which is why you can't tell me details like how many turns of what gauge with how many strands.  If I have those numbers, I can make some sense of it. But this is what I have gleaned.

**Also, this is based of a max current of 30Amps. I know you push yours much higher, but I'm looking for an efficient board.**

I do my best to represent the science here. Can we work together and move past the blame game and criticisms? We all just want something we can reliably ride and not have to wear insulating gloves (flesh meltingly hot hangars? I've been there using Jacob's Hubs with a Seismic G5 truck as a heat sink. It hurts. @EnertionSupport #raptor2)
```

---
## \#11 Posted by: Hummie Posted at: 2016-11-15T20:49:56.500Z Reads: 233

```
No one has a .1mm airgap.  You'll be lucky to find .4mm. 
There are now N52 that can do much higher than in the link here that scorpion motors use.  I've been using n45sh. Check here for common high heat stuff
https://www.kjmagnetics.com/specs.asp

Iron losses will be much smaller than copper with small hub motors

As far as "electromagnetic work" it came down o the manufacturer trying to see what was the fatest single strand they could fit for the amount of turns. 30 for 90kv. Really they used the fatest they could do for 33 turns and used the same wire so the 33 turn 80kv 
has greater copper fill and less resistance

Not feeling attacked but making sure if you're doing a sumulation with results it's accurate

I think there is not much that can be done to optimize other than getting as much copper in and as strong a magnetic field as can be built with strong magnets, powerful back iron, and thin gap.  The stator shape and size is staying.  
I was interested in looking into different magnet shapes and sizes and strengths and temp ability but it's a toss up and bigger isn't always most efficient and seeming pretty insignificant

At the end of testing or simulations those motors I was selling were decided as too small and I don't sell them anymore.  I feel like simulations might tell finer details, possibly innacurately, and real world testing is easier and really the simple solution is just to get a bigger motor if you want greater power or efficiency. Until the iron losses balance with the copper the motor is smaller than it should be for efficiency. Likely every little motor we are using.  Bigger solves all problems
But I'm interested in what u can come up with and will get u real resistance and L numbers tonight
```

---
## \#12 Posted by: KMeyerson Posted at: 2016-11-15T21:14:23.542Z Reads: 235

```
Jacobs are designed with a 0.1mm airgap. The result is that the 51.8mm diameter stator is surrounded by magnets with an ID of 52mm.  I've measured mine with mistsuboyo calipers and they're basically spot on with the drawings.

Yeah, but you're cooking them. Jacob tried N42SH for the anti-corrosives. I cooked half of my magnets. Have you seen the scorpion factory in china? They hand wind all of their motors. They run them at insane temperatures and I don't know if I would trust their numbers consistently. "Patent Pending" is always written on their sales pages, but I have yet to see any submitted applications.

You can use TWO wires to accomplish the same task as one.  They should know that too. 12 Gauge wire is basically impossible to use in a stator because of how thick it is. I used 6 strands of 20 gauge wire to get 14 gauge equivalent. I would have used fewer strands with 18, but the 20 was cheaper!

Copper fill doesn't always directly influence the motors performance is the iron is already saturated.  Jacobs have less than a 10% fill and half the resistance of the designs of your motors that I simulated (the winding factor was basically the same though.

The results are accurate for Jacobs. Thats why I want your gauge, turns, and strand count. I got them for the most part. Again, I used a 30 Amp current because I know both motors can sustain that for 120 minutes max torque at max rpm. 

Using two magnets per pole, for example, is a great way to increase torque without working too hard. I've done it with great success for small BLDC motors in the past.

Real world is great, but spending thousands on motor development for each production run seems like a bad idea. Better to do the math a bunch, build it a few times, then release it (Boosted really does win in the product design and testing department. Using PIC controllers for their motors is brilliant, professional, and cheap. We all need to learn from them to a degree.

Get me the Phase Resistance, Strand Diameter/Awg, Strand Count, and Turns and I'll run it for you.  If you could also send me a 2D cad of the stator just so that I can clean up the tooth thickness and what not that would improve the windings as well. Magnet widths/lengths help too (I know they're 2.65mm thick, but idk how wide they are/the gaps between the magnets are.
```

---
## \#13 Posted by: Hummie Posted at: 2016-11-15T21:21:03.159Z Reads: 214

```
I can do that but it would be a simulation between two motors that aren't available anymore. More interesting would be simulations of the the motors I'll be getting with 4770 stators and enertions hub motors which are said to be the "most powerful" and I believe the same stator as the 6372 motor they sell. 
I've never seen a motor with a .1mm airgap for sale anywhere and scorpion and hacker will do at most a .4mm
```

---
## \#14 Posted by: KMeyerson Posted at: 2016-11-15T21:33:05.844Z Reads: 205

```
Sure.

If you send me details on the new one I can tell you what to expect.
```

---
## \#15 Posted by: Pedrodemio Posted at: 2016-11-15T22:05:05.011Z Reads: 203

```
For anyone wanting to jump on the boat, here is trial version 

http://www.infolytica.com/en/products/trial/motorsolve.aspx
```

---
## \#16 Posted by: KMeyerson Posted at: 2016-11-15T22:08:33.925Z Reads: 202

```
I would instead suggest people use the online trial if they're not willing to wait for simulation results. Their servers are faster than most peoples computers.
```

---
## \#17 Posted by: Pedrodemio Posted at: 2016-11-24T19:29:59.091Z Reads: 205

```
Just started my trial so i can play with it on the weekend, fantastic tool, but too expensive, i will start an academic study on research around hub motors and will try to contact then to see if i can get a good discount or something like that, with the current political and financial situation here no way i will get my university to pay for the license

@KMeyerson , can you give some guide lines on how to achieve a relative flat torque curve? i tried lots of combinations and none seen to be going on the direction o flatness, i saw some torque graphs from @Mellow updates on kickstarter and they have an almost flat curve until max rpm

Edit:
After a lot of tests I accidentally discovered that using hysteresis current control the torque goes up significantly and becomes flat, so thats one of the secrets of a good permanece hub motor
Based o what I read this is somewhat similar to FOC but no quite, so using VESC on the actual stage there's no way to get the best performance out of a hub?
```

---
## \#18 Posted by: Trillium Posted at: 2016-12-11T08:20:25.011Z Reads: 191

```
Hi all, I'm never on here but I think I might be doing some beta tests through this forum in near future. I simmed the Trillium motor and its a bit of a lower performer torque-wise than hummie (30A limit, however) but it is in a 75mm wheel and has better thermal management. Glad to see people doing new stuff but at the same time frustrated! Would be nice to see some of my other competition before I waste any more effort with my motor development! ;)
```

---
## \#19 Posted by: evoheyax Posted at: 2016-12-11T09:04:32.097Z Reads: 191

```
[quote="Trillium, post:18, topic:13112"]
Would be nice to see some of my other competition before I waste any more effort with my motor development!
[/quote]

I felt the same way when I was a building my VESC iphone app. But hummies have been around since February or so of this year. Idk if I would say he's that new...
```

---
## \#20 Posted by: Trillium Posted at: 2016-12-11T09:20:12.220Z Reads: 186

```
I was talking about kmeyerson
```

---
## \#21 Posted by: KMeyerson Posted at: 2016-12-11T09:50:53.352Z Reads: 183

```
If you plan to use a VESC or similar ESC, or motors aren't comparable.

I am using DTC,  not SVM so my windings are different and yield different results.  For the record, the transition from DTC to DTC-SVM is not easy. Simulink hasn't been great help here.
```

---
## \#22 Posted by: KMeyerson Posted at: 2016-12-11T09:53:04.479Z Reads: 177

```
Yeah, sorry I didn't see your reply.

Boosted and Mellow probably use DTC, not SVM.  That's the secret tbh.  The VESC can be programmed for DTC, but it would be a significant firmware rewrite. Plus it works great for external motors so I think we just need a hub centric ESC
```

---
## \#23 Posted by: Mellow Posted at: 2016-12-11T10:05:15.084Z Reads: 178

```
Nice stuff. Sorry to be coy. We'd love to be able to contribute, but want to hit the market first before spilling (too much) of our guts.
```

---
## \#24 Posted by: Trillium Posted at: 2016-12-11T10:10:02.517Z Reads: 173

```
Isn't Svm a variant of dtc...? Don't you mean dsc? Why is it so much better? Are you winding the motor to use more of the winding >66% all the time?
```

---
## \#25 Posted by: Trillium Posted at: 2016-12-11T10:10:42.807Z Reads: 164

```
You guys already hit the market what are you talking about lol
```

---
## \#26 Posted by: trampa Posted at: 2016-12-11T13:24:33.498Z Reads: 171

```
Nice Job @KMeyerson. I Think before going that deep into detail, you should assume a perfect motor and a perfect electrical system. When you do that, you dig down to the physics behind BLDC motors. And you can stop to debate different motor designs. The "my design is better than yours" discussions don't help to understand the matter. 

We just assume the designer did everything right, he managed to build a nearly perfect motor for the size of a 90-100mm Skate wheel.

Benjamin Vedder did some nice explanations on that issue:
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/

So that this size motor wants to run at about 60K ERPM to be at peak efficiency for matters you can't influence. **You can't cheat the Physics behind BLDC outrunners.**
Dividing 60K ERPM by 7 is 8570 RPM. Using a 83mm wheel, wanting to hit roughly 35 km/h you would need to run a 1:4 gearing. Using 5M belts you can achieve roughly 1:2.5, so your system is already a bit less efficient, running the motor slower than it should.
Anyway, such a geared system could still be up to 85% efficient. Losses in the belt system are only 1-2%, so nothing that needs to be addressed. 
Now we look at 1:1 gearing and drastically reduce the RPM. We will end up with a motor that runs most of the time in a region of the efficiency curve that you don't want the motor to run in. At best you are 50-60% efficient, since the  efficiency curve usually has a steep drop! 

What happens: A huge amount of your stored energy (inside the battery) will dissipate into heat, reducing range and causing problems for the motor (overheating)

What do you do: Lets use the hanger as a heat sink (works at least to cool the stator, not the magnets)

What does that tell you: You ride a super inefficient system. Heat = Losses

If your electrical system is staying cool, you are running a efficient system - If you face heat problem, something is funny. 

I do understand that hub motors are interesting and everyone wants them. Please understand that they are at this stage a lot more inefficient and do have disadvantages. Its O.K. if you live in a rather flat and cool environment and if you can live with a lot less efficiency for the benefits of the stealthy look. If your tarmac is 70°C in summer + you face some hills, or want max. range, or you are going quite slow (20-30 km/h) or you need more urethane on the Hub (bad roads) it might be problematic to ride hubs. Understanding the Pros and Cons is important.
I am curious if the simulations will go hand in hand with the measured results. 

Frank
```

---
## \#27 Posted by: Hummie Posted at: 2016-12-11T16:56:03.336Z Reads: 166

```
I think the variable load and speed people do while riding negates a lot of
the value of doing much optimizing.  There's compromises made.  we all know that the most efficient way to run the motor is 80% of the no-load but no one ever stays at that speed for long, and if you also want a high top speed you're forced to have a large
Rpm range and greater inefficiency.

  With the way the vesc is getting more efficient and able To take more amps it seems more practical to make a high kv motor and then if someone wants to run it more efficiently they can lower the voltage.

I'll get you number and shapes Ken when the motors come in soon though.  I'm interested in what you come up with and have been looking to do simulations but know that a lot of the variables are set in stone for me (stator and back iron shape and magnet thickness) and all that I have adjustable is the magnet strength and temp ability and kv. And in my experience the biggest factor has been what the manufacturer decided they can wind with.  All I'm left to do now...all I feel is worthwhile doing now..is repeated asking the manufacturer to jam as much wire in as they can. Even maybe multi strand would be
better if they can get more copper in.  It's largely copper losses with these slow turning hub motors...more copper less
Resistance and a better motor. From the little I've found magnetic saturation and the increased hysteresis that comes with it is at flux densities way high and not as much of a loss as I'd thought maybe possible.  But I'd like to see and can get you what steel the stator I'm using is made of.  Known as Kawasaki steel.

What I really think would be an improvement which no one is doing is halbach arrays for the magnets!!  I hope to do that as soon as I can
I think losses in the belt-pulley system are much more than just a couple percent @Trillium.  Pushing the board I can feel a lot more resistance. If a hub motor and pulley set-up are compared with both operating at 80% of the no-load I bet the hub will by far be more efficient.  Not getting up to speed but once there. And there's other benefits in a hub motor of course which I'd say out-value possible losses in efficiency.
```

---
## \#28 Posted by: KMeyerson Posted at: 2016-12-11T17:14:05.698Z Reads: 160

```
I don't disagree with you about efficiency and losses. I agree that hub motors in their current setup dont work all that well.  Essentially I am moving from SVM motor control to DTC to have better information about the thermodynamics before I wind a motor.

A motor used in SVM based on the simulations with no load tends to have a sharp torque curve. The strandcount/total wire gauge is low and the number of turns is high.  You don't need 100% fill to get peak efficiency with SVM.  Essentially, Jacob and I scratch our heads at the SVM simulation data cause it doesn't always make logical sense.

Using DTC control, a motor is wound to maximum capacity with the thickest gauge and maximum number of turns.  The thickness of the gauge does correlate to the speed you'll get and the number of turns are also related to the toque.  If you assume 30% grade, 100kg, 100mm wheel you'll want to be on the safe side and make at least 10-15Nm of torque per wheel.  Not only does DTC follows all rules of motor logic making it easier to fiddle with the numbers, but the simulated thermal profiles with and without load are promising.

The way the simulation data churns out, SVM driven motors are just harder to get thermal calculations before manufacturing. DTC can be calculated thermally and with a load.  The goal is to keep the temperatures under 200*C for up to three hours at max.  At this point, a 63*52mm wheel goes from 23*C to 200*C under max torque and max rpm  in a about 60 minutes (For normal riding varied flats and 30% grades, you can go 2.5 hours without needing to cool down, and on a total flat you won't pass 80*C). That's not bad, it's not great though for people who put pedal to the metal. I figure a thermistor can tell people who do ride crazy hills all day that they need a few minutes to cool. I am using Seismic trucks (the G1 spring truck) because of the light aluminum and structural stregeic cutouts. Way better heat sink than any solid truck, even if it squeaks like there's no tomorrow.

On manufacturing I just want to be clear - you can wind a stator with 12 AWG wire or 12 AWG worth of 36 AWG.  The thermal properties are barely different in simulations, but it's a ton more wire to buy and if you're winding by hand it is an unfortunate business.

Hub motors are different from the ground up in what were asking from the BLDC.  We should approach them not by adapting them to existing tech, by developing around its needs. What does it need to have both torque and speed? The answer is not SVM at this point.  The VESC 6.0  schematic includes more current sense resistors so you'll have a higher accuracy with FOC. Additionally it overall design is promising for the SVM driven hub motors. What is left is the firmware to take advantage of these hardware improvements. Benjamin believes that the 6.0s FOC will be as coordinated and powerful as DTC, but well see. It's worth building anyway.
```

---
## \#29 Posted by: Trillium Posted at: 2016-12-11T19:07:32.527Z Reads: 131

```
I read a paper that seemed to indicate Svm was generally superior to DTC now that processors are so fast and cheap. I don't understand how you would get much gains from DTC that could've just be easily offset by stator geometry / cooling optimization in the first place. I think the only real gains with control are going to 6 phase or greater system. I would run a 6 phase in a heart beat if there were proven controllers (and small, like half size of vesc) available for it. I think 6 phase will be a later version of Trillium once the mechanicals are proven.
```

---
## \#30 Posted by: KMeyerson Posted at: 2016-12-11T19:19:22.664Z Reads: 126

```
Depends on the paper you read and the specific application studied.  DTC can be used with a lot of different motors, BLDC is one of them and put runner design is different from inrunner.

The reality is that the motors are going to have to get a bit bigger if we want efficiency as Frank said earlier. By how much? Depends really. The question for size is determining what sacrifice I can live with.

On my to do list is to build a dynamometer and get a steady test bench setup (@jacobbloy).  It'll make development a lot easier.
```

---
## \#31 Posted by: Trillium Posted at: 2016-12-11T19:21:34.549Z Reads: 132

```
I have built one and it was not cheap. Let me know if I can help I'm in LA.
```

---
## \#32 Posted by: KMeyerson Posted at: 2016-12-11T19:29:42.788Z Reads: 131

```
Medford Massachusetts.

How much did it cost and what kind of scale are we talking? car/motorcycle/bike?
```

---
## \#33 Posted by: Trillium Posted at: 2016-12-11T19:37:22.732Z Reads: 140

```
I spent around $3k. half machining half instrumentation. I have it set up for up to 50Nm. Use a huge motorcycle hub for varying load. It was mostly intended for simulating rides with a truck and two motors, so currently it is only set up to measure one motor at a time. I could make it do both motors but just seems wasteful
```

---
## \#34 Posted by: Trillium Posted at: 2016-12-11T19:41:33.430Z Reads: 138

```
Why do people want 200N of thrust _per wheel?_ That's insane. I don't even think boosted is doing that with their geared system. Is there documentation somewhere on that? I was thinking of buying one just to benchmark, but they are having issues lately
```

---
## \#35 Posted by: trampa Posted at: 2016-12-11T19:46:31.912Z Reads: 139

```
A lot of customers want MTB being 50+km fast and able to climb massive hills and they should have a super good range. I tell them they should balance the system, using these tiny motors. It's still a one gear system.
If you aim at an efficient system, you need to find the right balance. Average Speed should match 80% of no load RPM.
With Hubs that's difficult because they start to feel well at 60+km/h. Average speed is realistically 18-22km/h. The gap between average speed and top performance speed is to big.

Belt systems are 98% efficient. The reason why you can't push that good is simple. You push against a efficiently setup generator. The motor spins faster when you push (2.5x), creating more resistance. In many cases people do also over tighten the belt. 
Freewheeling pulleys would be nice....

I don't think controllers will do the magic. Its really a motor problem. Maybe thinking outside the box will bring something up.

Frank
```

---
## \#36 Posted by: KMeyerson Posted at: 2016-12-11T19:52:44.968Z Reads: 135

```
Consider 200N of thust as the max and that we want the ESC to keep the user around the 50-75% mark.  The ability to push 200N should only be unlocked when the speed is not maxed at 25mph and the current draw is high (aka, accelerating up a terrible hill).

I'd rather over design this than underdesign it.  We are all using off the shelf parts (the VESC 4.12 and VESC-X both are essentially off the shelf at this point).  

Measure twice, cut once.

And yeah, currebt hubs aren't there yet.  But that doesn't mean we can't bring it there.  It will take a ground up approach and it will take time.

Edit, Tampa beat me to the point about why 200N. 80% target.
```

---
## \#37 Posted by: Hummie Posted at: 2016-12-11T19:56:52.157Z Reads: 130

```
I'll definately finally do some comparitive testing of pulley vs hub and energy needed.  You make exceptions for why such resistance and say it's only a 2% loss at the belt but somehow in practice a coasting hubmotor will go over twice as far in my experience. Same electrical cogging issues with both set-ups but none the less much further. So much assuming and guessing and speculation related to efficiency, a lot of it from me, and the real world will tell us soon and I'll get out there and report back. Maybe I can get @Jinra to come out again and we can do it this time. I'll be rolling in a couple days.
```

---
## \#38 Posted by: trampa Posted at: 2016-12-11T20:00:54.803Z Reads: 124

```
Belts are efficient. 98%. You just spin the motor faster when pushing a geard system.
Its a more efficient generator in that case.

Frank
```

---
## \#39 Posted by: Hummie Posted at: 2016-12-11T20:04:13.364Z Reads: 122

```
Assuming 98 percent efficiency, maybe it's not taking into account the gear ratio and extra rotation necessary.  With a 3:1 maybe it's 3x that 2% loss.  Maybe. None the less it feels a lot more and I want to compare real numbers
```

---
## \#40 Posted by: KMeyerson Posted at: 2016-12-11T20:13:44.972Z Reads: 127

```
Personally, when I ride my Boosted, I get to top speed and then I coast it out till I'm at 13mph and then go back up and repeat. I get about 9 miles on the V1 Dual now at Pro mode instead of the 6 I used to get riding at full throttle the whole time.  Commuting time is a little longer than driving when you're not at 22mph the whole time, but the range is worth it.

I just saw an article that I can't find about a guy who put his Tesla into neutral all the time to ride/coast and he gets a crazy high range per charge.

Hubs can be great for riders with patience who are commuting.  If you want to gun it all the time, then gears might be best for now.  Hopefully the tables will turn and we can get the best of both worlds.
```

---
## \#41 Posted by: Pedrodemio Posted at: 2016-12-11T20:14:25.297Z Reads: 134

```
Main problem with belts are damage, that's my reason to start developing a hub, what's worth to have a better efficiency if I have to change belts every few rides? 

This is my particular situation, "good" roads but full of little rocks 

For those interested, there's a software called Emetor, free and online, nowhere as good as motorsolve but it's free
```

---
## \#42 Posted by: KMeyerson Posted at: 2016-12-11T20:18:36.180Z Reads: 132

```
Amen.  My boosted is constantly scraping the ground (the motor mount is silver now, not black) and I've busted a handful of Kevlar reinforced belts.  Maybe V2 solves this entirely.

I would like to cut down on the appearance.  Belted speeds and efficiency is nice, but the motor assembly can look and feel like a car hitch ball sack thats dragging in the street. Certainly wrinkly and scabbed enough.  It get caught in stuff all the time as well that the front truck doesn't snag.
```

---
## \#43 Posted by: Pedrodemio Posted at: 2016-12-11T20:24:08.041Z Reads: 129

```
Exactly, the only solution would be reduce the gearing to have a smaller wheel pulley or reduce the pitch, tried both and them you go to a new set of problems, maybe getting a crazy low kV motor until I get this hub project going

One thing is great with HTD 3M, less belt drag, a lot less, the first time I tried the 5M it felt like something was wrong and braking the board
```

---
## \#44 Posted by: Trillium Posted at: 2016-12-11T20:25:14.562Z Reads: 117

```
Seems wasteful to shoot that high and will result in a very heavy motor.
```

---
## \#45 Posted by: Pedrodemio Posted at: 2016-12-11T20:31:28.938Z Reads: 121

```
@KMeyerson did you manage to get the motorsolve interface, such as matlab working? If I manage to get my hands on a license my plan is to program a evolutive algorithm to optimize everything on the motor automatically, not needed to spend hours of worked trying to get better results when you can tell your pc to do that

The hard part on this aproach is to define the parameters and maximum and minimum boundaries to be optimized
```

---
## \#46 Posted by: KMeyerson Posted at: 2016-12-11T20:38:54.042Z Reads: 113

```
We're dealing with two separate things.

1. Design a kickass motor that stays cool under stress. Use MotorSolve (MotorSolve online is just as good tbh probably).

2. Design a kickass ESC to power said motor. Use Matlab simulink to get this going (considering ditching sinusoidal waveforms because sin is better for AC I'm finding. Trapezoid is gonna be a little louder but it'll have minimal torque ripples).

I haven't connected them and wouldn't want to. There are so many variables and it's just not worth it.  MotorSolve takes 3-5 minute per simulation on my server/desktop and 4-7 minutes of my top of the line MacBook Pro Retina.  Don't try to merge them, you've been warned. It'll suck.
```

---
## \#47 Posted by: Hummie Posted at: 2016-12-11T20:47:41.235Z Reads: 115

```
But through simulations will you find magic in another design different than what's being used? You might get a bit here or there but the general rules of efficiency will apply and the size and weight of the motor will largely determine its output ability and efficiency is right around the corner
```

---
## \#48 Posted by: Trillium Posted at: 2016-12-11T20:47:42.582Z Reads: 112

```
Let me know if you get that working, I've been wanting something like that for a while.
```

---
## \#49 Posted by: Trillium Posted at: 2016-12-11T20:48:30.872Z Reads: 109

```
What kind of mesh settings are you using to get 3-7 min run times?
```

---
## \#50 Posted by: Pedrodemio Posted at: 2016-12-11T20:49:52.260Z Reads: 110

```
Thanks for the warning, I still believe that optimization for at least the bulk of the design is worth, I found this article to be enlightening http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.625.4767&rep=rep1&type=pdf
```

---
## \#51 Posted by: KMeyerson Posted at: 2016-12-11T20:50:30.276Z Reads: 111

```
These finite element analysis take a lot into account. More than is really necessary to get into the ballpark.

Just plotting a Speed vs Torque graph takes 3 minutes to calculate every phase angle for each of the speeds (in increments of 100rpm from [1,3000])

Field Oriented Control and Direct Torque Control have historically been too close to prove superiority.  However I would rather be able to simulate the heat before I wind it.

The VESC 6.0 will be a game changer with the best FOC setup we can get our hands on for small ESCs and vehicles.

http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.193.6219&rep=rep1&type=pdf
```

---
## \#52 Posted by: Pedrodemio Posted at: 2016-12-11T20:51:23.325Z Reads: 105

```
Yes, the gains could be minimal, but a lot of small gains could be significative in the final design, I still have to analyze the cost/benefit of this aproach
```

---
## \#53 Posted by: Pedrodemio Posted at: 2016-12-11T20:54:12.487Z Reads: 111

```
With motor not yet, by I've done simple problems just as proof of concept in one my courses, if you are interested search for Yang nature book, it has a lot of types of evolutive algorithms that mimics the behavior of groups of animals, crazy ideias, but work beautifully to get a maximum point in problem of non linear behavior and multiple dimensions, and the computational cost in relatively low
```

---
## \#54 Posted by: Pedrodemio Posted at: 2016-12-11T20:58:39.588Z Reads: 107

```
Back on topic, did you manage to understand in simple terms what exactly is this hysteresis control? I've a few more papers but could not understand in what way it is better than FOC or even BLDC, I talked a lot to the teacher that's guinding me and we could not wrap out yet heads arround it
```

---
## \#55 Posted by: Hummie Posted at: 2016-12-11T20:59:23.788Z Reads: 113

```
In looking for most efficiency include the manufacturing and cost limitation.
what can the air gap be, what cost for tiny laminations of ideal steel you're willing to spend, and if you really want the most efficient maybe add the cost of multiple small segment magnets to cut eddy currents, or the cost of going further with a halbach array or laminations in the flux ring, or skip using wire and instead formed copper sheets.

My point is there are a lot of known ways to get better efficiency but a lot easier and cheaper and more reliable direction might be to just go bigger.  Not efficient per se but makes it a non-issue to a large degree

but id love to be more efficient and if I thought I could do much better using simulations I'd be all up and in it.  I do respect it and know an efficient motor is effectively a more powerful motor, if only it were more easily achieved and it just needed some adjusting of number but Ido t see it and just follow the tried and true methods within limitations of practicality and expense
```

---
## \#56 Posted by: KMeyerson Posted at: 2016-12-11T21:11:10.358Z Reads: 120

```
It's direct torque control (DTC).  Look at the wave forms and then also look at a DTC algorithm and compare it to an FOC algorithm.  It'll click.

For your consumption about the breakdown of motor control types we can use. The gold would be DTC-SVM.

I've put something like 100 hours in Novemeber/December in research for ESCs.  The best thing you can do is study up.  Google Scholar if you don't have access to JStor or a comparable academic database collection.


<img src="/uploads/db1493/original/3X/e/6/e67659d7196b69947b062cdb4d295d4dc0366df3.png" width="690" height="388">
```

---
## \#57 Posted by: trampa Posted at: 2016-12-11T21:16:16.489Z Reads: 125

```
Best mileage is achieved when going slow all the time. Wind resistance is the mileage killer No1.
I built a 12S4P (Samsung 3000mAh 18650 cells) Longboard, using our Trampa 118kV Motor, 37/14 gearing. Set the VESC to max. ERPM to match 20km/h. Range was 60 Km. Its impossible to empty the pack in one go - feet start burning after one hour....Belts do wear but you could 3D print a cover for the belt to solve that issue. My belts (Strongbelt premium) last for more than a year. 

Current Hub motor issues are in my eyes (compared to a 1 : 2.5 gearing):

- very low efficiency (only 50-60%)
- therefore heat issues (losses =heat)
- therefore a lot less mileage
- low torque (ca.2,5x less)
- therefore the need for a twin setup (Two VESCs, two motors)
- magnets are nearly impossible to cool (insulated by urethane and resting on bearings).
- Thin urethane on a stiff core and therefore more problems with vibrations and less damping.
- Thin Urethane will put more strain on the hub motor itself + your feet
- servicing the wheel bearings is more complicated (customers will struggle to disassemble the motor)
- not good for a hot summer environment and hills or heavy riders.
- braking is less strong (no gearing)

Advantages of hubs:
- better coasting (due to inefficient motor gearing)
- stealthy look
- cheap to make 

Belt Systems advantages:

- much much better efficiency (ca. 85%)
- much more torque (2,5x)
- ability to change gearing and find out best setup for your ride
- Wheel bearings are easy to change and maintain
- you can use different motors and experiment
- motor is under less strain from vibrations
- motor sits in the airflow and cools down easily
- thick urethane tires prevent vibrations (ride comfort)
- braking is much better (geared brakes)
- A single, geared motor setup can perform just as good as a dual hub setup (cheaper to build and maintain, 1 VESC only)

Disadvantages:

- less stealthy and less slick appearance
- Belts and gears need a service once a while (hub motors will also want some attention btw.)
- A transmission is more expensive to make (less profit if we compare a twin setup to a twin setup)
- coasting is less good (I simply use the cruise control button to keep the speed) 


Frank
```

---
## \#58 Posted by: Pedrodemio Posted at: 2016-12-11T21:25:43.553Z Reads: 123

```
This max 60% I don't think it's true, this picture I got from the Mellow engineer, its bad to look but its way more that than we have on the belted sistems, we all talk that belt is great efficiency but I've never seen anyone put a board in a dynamometer and run lots of speed and torque combinations to get this kind of data, thinks is something that has to be done, maybe you guys could do it, it will improve your product and make more scientifically to determine the optimum gear ratio 

<img src="/uploads/db1493/original/3X/8/9/89458c2caa94b525acb8e22312c320e4aaf9cd19.PNG" width="281" height="500">
```

---
## \#59 Posted by: onloop Posted at: 2016-12-11T21:46:19.496Z Reads: 119

```
https://cdn.meme.am/cache/instances/folder120/500x/73840120.jpg
```

---
## \#60 Posted by: trampa Posted at: 2016-12-11T22:02:42.804Z Reads: 123

```
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/

"Now we know that copper losses are proportional to the square of the 
torque produced by the motor, and at low RPM and high load they are 
dominant. As RPM increases, other losses start to add up exponentially. 
In my experience, these losses start to get significant around 60k 
electrical RPM, which for a 14-pole motor is about 8570 mechanical rpm 
(most 50mm+ outrunners have 14 poles, some unusual ones have 18). 
Because of the square relation, it is desirable to run at as high speed 
and low torque as possible as long as we stay below 8.6k RPM. To express
 the square relation in some numbers, having double the RPM and half the
 torque at a certain power output will cause four times less losses. The
 lesson from this is that: make sure the top speed you design the 
skateboard for is at around 8.6k rpm on the motor if you are using an 
50mm-60mm outrunner." quote Benjamin Vedder

Don't get me wrong, I love the idea of hubs - but you have to face the reality of physics.  
Hope someone will come up with a clever idea one day. 

Frank
```

---
## \#61 Posted by: Trillium Posted at: 2016-12-11T22:16:39.690Z Reads: 118

```
I'm pretty sure that the first Trillium hub is going to be the most cosmetically controversial hub so far. In fact if everyone on here doesn't like the cosmetics I'm probably not going to take it into full production. Per motor it will probably peak at 100N to ground (on 7S/30A with no load around 23mph) so certainly not for those people who are looking for that extra dose of adrenaline and don't mind getting injured. Going for power density, better urethane mechanics, and better thermal performance than what is currently on the market.
```

---
## \#62 Posted by: trampa Posted at: 2016-12-11T22:54:09.078Z Reads: 120

```
@Hummie, you would need two boards, one using the same motor as a hub drive and the other (wound to a proportional higher KV) within a geared system. You could simply do a comparison, riding parallel @ same speed. You don't want to compare apples to oranges....So you use the same motor. A thermistor inside the motors would tell you a lot about losses. A range test will also tell a lot. This would be the ultimate comparison in a real world environment. 

Frank
```

---
## \#63 Posted by: Pedrodemio Posted at: 2016-12-11T23:27:31.808Z Reads: 122

```
Yeah, i agree on that, its a compromise, the only solution on that case is to go to a geared hub like Stary, or implement a geared transmission like @Nowind did on their builds

I think the main goal we have to achieve is reliability, without that our boards are just toys, mine right now is pretty efficient running on a 230kV 10S with 3:1 gear ratio, i get 8Wh/Km on my commute, full throttle for 90% of the time and with two big hills, i'm weight something like 80Kg + backpack, bit i literally can't afford($$$) the amount of belts i've been using
```

---
## \#64 Posted by: Pedrodemio Posted at: 2016-12-11T23:29:59.946Z Reads: 116

```
Yeah, i have access to something of that type, will look into it, thanks, for now i will focus my effort on using VESC, my codding abilities is only on basic to intermediate level, maybe in the future or with one of yours ESC's
```

---
## \#65 Posted by: KMeyerson Posted at: 2016-12-11T23:41:33.418Z Reads: 117

```
It's a lot of work but it'll be worth it.  In the end, stary has the best in wheel motor. Even if it's not a real hub and is super loud
```

---
## \#66 Posted by: Pedrodemio Posted at: 2016-12-11T23:53:57.302Z Reads: 126

```
I hope so. The noise in the Stary is the major drawback, but with a few tricks such changing the gear profile and making it work partially submerged in oil would do the trick to quiet it down

I am starting to take a look on geared setup that i said, it will be necessary a dumb gear in the middle so the motor does not colide with the truck and i have to test if it can fit a dual motor

Also, i'm diggin a little deeper in Emetor but getting really weird results and its a lot of work to test a new design, you have to run each speed separated

Edit: just a test to see what a geared setup would look like, this is with a 190Kv 50mm motor and geared to 35Km/h

<img src="/uploads/db1493/original/3X/a/9/a911dac0223a38f8043306ce4fa360904900465d.JPG" width="690" height="392">
```

---
## \#67 Posted by: Trillium Posted at: 2016-12-12T00:53:54.960Z Reads: 114

```
Is there any real data on their motor? Anyone dyno it? Maybe someone can send me one to dyno
```

---
## \#68 Posted by: KMeyerson Posted at: 2016-12-12T01:06:06.452Z Reads: 111

```
I wish. But inrunner are more efficient than inrunners and gears are also a win.

If you do, i would be impressed. They have a one wheel drive.
```

---
## \#69 Posted by: Hummie Posted at: 2016-12-12T02:00:50.475Z Reads: 112

```
Inrunners being more efficient I guess you mean iron less. Core less. I think most efficient would be coreless.  Id like to see how much torque u can get out of a coreless motor. Or skip torque and use its speed and a gear to get the power could you?  A high speed inrunner coreless (or not coreless) geared hanger.   180mm or so of motor space
```

---
## \#70 Posted by: KMeyerson Posted at: 2016-12-12T02:20:55.587Z Reads: 115

```
Coreless is a pain in the ass cause it's totally submersed or immersed in epoxy. A lot of heat buildup. I toyed with the idea.
```

---
## \#71 Posted by: trampa Posted at: 2016-12-12T09:32:27.922Z Reads: 116

```
I would say, gears are badly needed and a good planetary gear box is well expensive. These gears will always be noisy unless they run in oil and have curved teeth. It gets a bit complicated and expensive in my eyes. 
Belts are simple, efficient, quiet and for the $$$ of a good planetary gearbox you can buy a lot of replacement belts and pulleys. A good belt cover would sort out most problems.

But its also really fun to think of new solutions. Otherwise we would still be in stone age.
My feeling is: The Outrunner motor is pretty much at its peak now and and still we see to much inefficiency and problems. A major design tweak would need to be implemented.
Most customers don't understand the Hub motor issues and will buy 1:1 hubs anyway, especially if they are cheap. 
It's o.K. when they are taught that hubs go hand in hand with compromises. Basically a matrix would help to make the decision "geared or hub". This way advantages and disadvantages of both systems would get known and you can make your decision on facts rather than hype. The simulations @KMeyerson does are really helpful.
@KMeyerson: Could you simulate the same motor (with proportional different KV) for 1:1 Hub and a 1:2.5 geared setups? Maybe that would shine some light on the issue and will help to develop better hubs.

Frank
```

---
## \#72 Posted by: Pedrodemio Posted at: 2016-12-12T11:33:00.732Z Reads: 114

```
Frank, of your motors, they are made to custom parameters? Like stator format, etc?

One think that I imagine happens is most of the motors uses readily made stators and geometry to lower costs, maybe the outrunners that use are no that efficient, but the gating mask the drawbacks of that

One step would be teardown a bunch of motors and simulate them, or assembly a dynamometer and test, them we can compare, I think this quest to a usable hub can lead to even beter geared system, optimizing the motors to our specific use to have peak efficiency where we need and a custom torque curve, something on the shape that of the Mellow hub
```

---
## \#73 Posted by: trampa Posted at: 2016-12-12T14:10:05.965Z Reads: 109

```
Hi Pedrodemio, our motors use an existing Stator, but that's about it. Everything else has been reworked and optimized. We tested the motor on dynamos at different voltages and loads. 12S setups are at peak performance close to 90% efficient, so you won't be able to optimize that. The efficiency curve is very flat already. Torque is linear to input power. These motors are already very very efficient.

Anyway, design a hub, rewind it to higher KVs and use it within a geared system. You will see that there is a square relation between copper losses and torque@RPM As Benjamin said: double the torque, decrease the RPM by half and your losses will get 4xhigher. There is nothing you an do about hat except building a bigger motor.
You can optimize things up to a certain point, sure. Magic won't happen unless you come up with a radical new motor design that will spin the Magnets at 14x lower ERPM rate. That's gearing again.

Frank
```

---
## \#74 Posted by: Pedrodemio Posted at: 2016-12-12T14:14:23.894Z Reads: 106

```
Good work, do you have a picture or something about the dynamometer used?
If it's not something confiditial could you share the results for one of your motor? 

Thanks
```

---
## \#75 Posted by: Hummie Posted at: 2016-12-12T15:54:53.478Z Reads: 104

```
  When you say the motor is 90% efficient on 12s how would the voltage effect the motor efficiency?
Frank I guess you meant a design that will spin magnets at a faster rate at the end of what you wrote
When you say you can make torque more linear..how is this possible other than through the esc?  The motor as I understood will have a torque to speed and efficiency graph that's pretty set in stone with these motors and it's more so what speed you're at that decides where you on on the graph, as your vedder quote/law states.
```

---
## \#76 Posted by: Hummie Posted at: 2016-12-12T16:03:01.949Z Reads: 104

```
[quote="KMeyerson, post:70, topic:13112, full:true"]
Coreless is a pain in the ass cause it's totally submersed or immersed in epoxy. A lot of heat buildup. I toyed with the idea.
[/quote]

Tesla car motors are potted. It need not add heat.  

http://www.evtechexpo.com/media/news/2015/02/26/how-proper-applications-of-thermally-conductive-materials-will-improve-motor-power-density/
A coreless motor need not be potted anyway
```

---
## \#77 Posted by: KMeyerson Posted at: 2016-12-12T16:15:44.318Z Reads: 100

```
Cost per 100mm wheel?
```

---
## \#78 Posted by: KMeyerson Posted at: 2016-12-12T16:16:33.519Z Reads: 99

```
You can make the torque linear in both ESC and Motor.  You just need to know how the ESC behaves and tailor the motors performance to that.
```

---
## \#79 Posted by: NickTheDude Posted at: 2016-12-12T16:19:06.262Z Reads: 104

```
I don't know what most of this means... But I hope to at some point in the future, so, from my future self, thank you!
```

---
## \#80 Posted by: Hummie Posted at: 2016-12-12T16:46:36.587Z Reads: 109

```
300$ for two pints of the best stuff I could find. Buy larger go cheaper

http://www.lord.com/products-and-solutions/electronic-materials/thermoset-sc-320-THK-thermally-conductive-silicone

I have never see a motor that inherently had a more linear torque curve.  What would make a motor design have such a thing?
```

---
## \#81 Posted by: KMeyerson Posted at: 2016-12-12T17:00:38.003Z Reads: 110

```
Huh, not bad price wise. Could try doing it at home.  Might be great as an alternative to Starys inrunner as a mod.

Well consider it from a calculus perspective.  If the motors peak torque is something like 50Nm at 0.000001RPM, then the curve drops steeply and plateaus before approaching zero then that segment of the curve is spot on.

The window/frame of reference were concerned with is 0-4000 RPM with hub motors.

Plotting a DTC curve is a lot easier than an SVM.
```

---
## \#82 Posted by: Hummie Posted at: 2016-12-12T17:17:45.316Z Reads: 107

```
But how would you design a motor with a more linear torque curve?  If u did it would therefore have a more linear efficiency curve no?  I've never heard of such a thing in motor design.  Gaining more torque through motor design, sure, but it will still follow the same slopped performance curve when graphed.  Can u please show me two graphs with one having a more linear torque curve and explain why
```

---
## \#83 Posted by: trampa Posted at: 2016-12-12T17:26:52.109Z Reads: 112

```
We tested different voltages and they did have an effect on efficiency. Low KV seams to like less Amps and higher voltages. Technocratically it should not have a huge impact within a certain range, agreed.
Anyway, we always wanted to go for 12S, so most test were done at 45V and therefore I state the results we got together with the voltage we used. Roughly 88% efficiency at peak. When you read 95% efficiency somewhere, be sceptic! 75-85% is realistic for hobby size BLDC Outrunners.
Torque is linear and nothing special - did I say we made torque linear? I said Torque is linear. 
Anyway, I don't want to debate our Motor or any other motor. I stated that before: **We simply assume the perfect motor to debate that issue.** The "my motor is better than your motor debate" is not helpful in that case.
All I want to say: Most of these Motors are quite good already and if you wind them accordingly to application they are performing quite good. There is an optimum RPM you should run them at in order to stay efficient. That is what Benjamin stated in his article. You can't increase torque and lower RPM beyond a certain point without getting huge losses (square relation). If that was possible we would not see gearboxes in electromechanical machines. 

More torque needed @ low RPM @ high efficiency: Bigger motor required, or gearbox. End of the Benjamin Story.

Basically my point is: Physics set limits and it has nothing to do with the design of the motor if you stay in the same size class. Some motors are better, other worse, magic won't happen unless someone finds a major design tweak allowing sort of magnetic motor gearing or whatever. People spend their lives on motor improvements. Its not that easy.

Don't get me wrong, the idea of Hubs is fascinating and you can ride them somehow if you can accept the facts above.
Hubs are not yet what customers believe they are. They will find out.
But: There is a market and someone will serve that. I really respect Jacob Bloy's and your work on Hubs! Good job, go on, never give up. 

Frank
```

---
## \#84 Posted by: KMeyerson Posted at: 2016-12-12T17:32:14.255Z Reads: 101

```
The trouble is people want to hit sales and make products more than pioneer a science.
```

---
## \#85 Posted by: KMeyerson Posted at: 2016-12-12T17:35:17.476Z Reads: 114

```
Here are two example virtual motors I toyed with.  If these motors were being used under 1000rpm. Torque would be linear.  At this point to make the torque flatter at higher RPMs, then the motor does have to be bigger. 

<img src="/uploads/db1493/original/3X/8/9/8929f56daa396bc47f9a6191e564c182c155200f.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/d/a/daaeadee9c2d6726b35872236352a42380683a82.jpg" width="375" height="500">
```

---
## \#86 Posted by: Hummie Posted at: 2016-12-12T18:09:38.571Z Reads: 103

```
I don't understand how you can have a linear torque as speed is increasing. They are said to be inversely proportional as with increased speed the bemf increases and limits the current that can be put to the motor.  It seems like those examples of a motor are stifled in some way and they should have greater torque at the slowest speeds on the graph. 
What characteristics of a motor would equate to a linear torque curve, meaning level? I still am not a believer yet.  Convince me please!

I'm also not a believer in higher voltage making a more efficient motor if it's wound appropriately for the voltage and load.  @trampa. I'm sure I'm just sounding like a contrarian but I've seen too much evidence saying otherwise.
```

---
## \#87 Posted by: KMeyerson Posted at: 2016-12-12T18:23:04.137Z Reads: 102

```
If the torque at 1rpm is below 0Nm, the graphs tend to be upwards sloping.

It's annoying to get it right. Also level for a given frame of reference.
```

---
## \#88 Posted by: Hummie Posted at: 2016-12-12T18:30:20.056Z Reads: 102

```
Don't understand what ur saying 
How can a motor have a linear torque curve inherent to the motor?  Never seen that other than through the controller limitation. I'd heard, as I just wrote above and makes sense, the back emf will reduce current at increased rpm. This is universal as far as I understand
```

---
## \#89 Posted by: KMeyerson Posted at: 2016-12-12T19:34:42.737Z Reads: 102

```
I've stressed this a few times.

It's a frame of reference issue.  If I graph the height of a falling object, but zoom in to 0-100Ns, the change in high will look insignificant.  It's not representative of the whole picture.

If I take the tangent of a curve. It's representative of the curves behavior at and around that point but not necessarily of the whole curve.  If you build a motor that is efficient a a billion rpm, and you sample 0-4000 RPM, the massive slope over a billion could be virtually flat during the sampled range.

These graphs visualize data and performance. I set the window to 1-4000 because it's the range I am most concerned with. If I set it to 1-10,000 the torque will become negative which is useless and not helpful for our purposes.  I am including the relevant data here. Not the extraneous points.
```

---
## \#90 Posted by: Hummie Posted at: 2016-12-12T20:51:54.433Z Reads: 100

```
 
Maybe you're talking about a different graph or seeing it differently.  Looking at the second graph you posted the most efficient speed would be roughly 15000 rpm, and assuming maybe 85mm wheel roughly about 15 mph and a possible top speed for a hub motor.  In fact it doesn't seem a small window on the bigger picture, this graph shows the motor spinning up to 3500, way beyond practical, without an increase in voltage somehow. 
This as it shows here would be a dream motor where torque doesn't decrease with speed but instead is continuous all the way from 0 till the most efficient rpm 80%.  There isn't a power graphing but would like to see.  Full torque at full speed I've never seen.
```

---
## \#91 Posted by: KMeyerson Posted at: 2016-12-12T21:44:07.471Z Reads: 99

```
Hummie, you haven't simulated nearly as many motors as I have. When you spend three months fiddling with the numbers to get SVM and DTC results. You'll see a lot. I've kept the results I care about. The results I dint care about I didn't bother to render as a PDF.

I have a life and I would appreciate it if you accepted my word that these graphs are a SMALL picture of a HUGE number of simulated results.

If you feel so compelled, I will generate a shitty graph for a motor with a peak torque at 8000 rpm that would have a flat torque at 0-4000rpm that's below 0 Nm.
```

---
## \#92 Posted by: Hummie Posted at: 2016-12-12T23:18:09.263Z Reads: 98

```
I'm just trying to talk about motors.  I'm questionng how you can design a motor to have a linear torque curve as in the graph you posted
These guys half way down the page lay claim to it and show a graph:
https://www.kickstarter.com/projects/1800147378/mellow-the-electric-drive-that-fits-under-every-sk/posts/1352482?lang=de

and they give the impression it's due to the motor.  I still have it unanswered for
sure though as what they say is ambiguous and i think it would be the esc doing it and that's what makes sense to me. I don't think you can design a motor to have linear torque.
```

---
## \#93 Posted by: KMeyerson Posted at: 2016-12-12T23:45:27.116Z Reads: 96

```
Oh I see. Yeah I think it's nonsense.  They're ESC and motor are probably very well tuned to each other

Just claiming their motor is doing everything is probably advertising
```

---
## \#94 Posted by: Hummie Posted at: 2016-12-13T00:15:33.934Z Reads: 101

```
And here I can page him with a snap @Mellow. Pretty awesome.  
How's the torque stay level as in your ad?

https://www.kickstarter.com/projects/1800147378/mellow-the-electric-drive-that-fits-under-every-sk/posts/1352482?lang=de
```

---
## \#95 Posted by: trampa Posted at: 2016-12-13T01:06:31.082Z Reads: 109

```
Hi, I put something together for you guys:

This would be a typical Dyno result: The 120 and 140 KV are real data from prototype motors we made in 2015, the 70KV Motor is a guess. I think a very friendly one, putting out 3Nm @ 30A @ 62.5%efficiency

Basically when you go for lower KV/RPM, the efficiency curve drops steeper. You can't push as many amps at a given voltage + we deal with this issue: Copper losses are proportional to the square of the 
torque produced by the motor, and at low RPM and high load they are dominant.

<img src="/uploads/db1493/original/3X/4/4/44a4a0e0a18da3ac5ba162be6ebc34ae0f82b1b1.jpg" width="584" height="500">

If I now gear down our 140 KV Motor, putting out 3,5 Nm @ 50A @ 45V, using a 1:2.85 gearing, I will have roughly 10Nm at the wheel on a single motor setup. A twin drive could output nearly 20Nm! I would still be close to 80% efficient in that case. The Board is a beast taking any hill without even getting really warm.
We managed to push 200Kg up a 12% hill with a single motor using a VESC4.12., 118 KV motor and 14/37 transmission.

Now we look at the Hub: 3Nm at 30A, only 62.5% efficient. A Twin would only output 6Nm under a lot of sweat.
I would say 2Nm is more realistic if you don't want to cook your coils and magnets.

Now some say: But the 15mm belt can't handle that >> It can. 
If its rated 3.0 Nm for a given transmission, the 3.0 Nm applies to the smallest pulley within the system (weakest part of the chain). Assuming a 1:2.85 Gearing: 3 Nm x 2,85=8,55 Nm at the wheel. This is the safe side and usually the belts can handle 1.5x that. Otherwise you could not push 200Kg up a 12% incline on a single. 

I still like the idea of hubs, I'm just very realistic. Its a motor problem that can be solved using a much bigger motor.

Frank
```

---
## \#96 Posted by: monkey32 Posted at: 2016-12-13T08:29:06.876Z Reads: 103

```
Hey Frank,
When you talk about much bigger motors what size do you think would be adequate?
```

---
## \#97 Posted by: trampa Posted at: 2016-12-13T09:49:12.914Z Reads: 103

```
To big to fit inside a 100mm wheel. 

I would love to see the dynos of some Hubmotors, so we are out of the guess range.
Maybe 4-6Nm is achievable when accepting **the massive low RPM high torque losses** and managing to cool the system.
Anyway, this is sort of funny because you don't want to operate in that 50-60% efficiency range. lets assume you drop in temp and hall sensors. @105°C plus hall sensors will suffer and give up soon. Many parts of the motor don't like the heat above 100°C over time. Heat is your enemy No1.
Electric motors are so efficient, why wasting all that efficiency + get heat issues? Technically its the wrong approach to try to squees a competitive torque out of a 1:1 transmission without scaling the motor. Problems will occur!   
When I understood Benjamins Videos correctly, VESC Tool will be able to calculate efficiency because all the relevant data is being gathered. So its just a matter of generating an output file.
That would really help to understand the matter and everyone running Vest Tool would be able to see the performance of the system under strain.

@Hummie: Do you have some data to fill in? Torque, efficiency etc.

With regards to size: I'm not an expert but assume its a lot bigger in diameter and weighs like double to triple (sorry, square relation again).

I'm not against hubs! I like the idea, but currently I see to many issues to get really thrilled. Scaling would be needed.
I could probably ride small hubs over here in Berlin. The town is flat like a pancake and my weight is low.
I could go slower and my way to work is only 7Km. In Summer at 35°C, in combination with 70° hot tarmac + knowing my ride style I would pretty soon hit the limits. If you know the compromise, its fine. 
If the motor gets to hot, you should work towards a cooler system and not try to dissipate the heat (losses).
A cure is always better than fighting the symptoms. But: Sometimes you have to accept a compromise.

In my eyes the compromise is the belt drive. Others see the compromise in the acceptance of losses.

In Germany we would say: Egg-laying-wool-milk-pigs don't exist. 

http://www.tse.de/Extras/Bilder/WOLLSAU.jpg

Frank
```

---
## \#98 Posted by: Pedrodemio Posted at: 2016-12-13T14:21:17.099Z Reads: 101

```
VESC with a few additional data could do that, the problem is that we have to measure mechanical output, if we knew precisely the drag coefficient, grade, wind speed, rolling resistance (including loss in bearings and belts) then we could do it, otherwise the value would be to far from reality

One way to do is to use a dynamometer to map the efficiency surface of a motor, like the picture from mellow i posted a while back, and store that on VESC or some microcontroller connected to it, them knowing the current on the motor and speed would could go on that data base and see what efficiency we are getting, would be a cool information to display on the remote to ride as efficiently as possible

@Mellow  could you guys share what software suite have been used to develop your motor? i'm trying to find a cheaper alternative to MotorSolve, even though i think it does not exist
```

---
## \#99 Posted by: Hummie Posted at: 2016-12-13T17:37:57.402Z Reads: 103

```
It's not new turf and electric bikes are still using hubs and mid-drives, as their pulley setup is termed.  Hubs are going strong still. Some have developed internal gearing but a lot haven't and as this article states the gearing just got in the way of where there could've been more motor. 
 https://www.electricbike.com/large-hot-rod-hubmotors/

Motor simulations may reveal a lot but I've read of too many incidences of them not being accurate and they don't take into account the losses of the gear system (I've read that the pulley and belt is maybe 3% but simply spinning a hub motor vs pulleyed wheel I have suspicion it's much more). The real revealer is on the road and how many watthours spent to reach a distance at a certain speed and I haven't seen a test yet!   Next week I will make it happen.  At least I can definately do the hub motor numbers and hopefully can find a pulley setup with a vesc to compare to. Anyone in San Francisco capable of doing the pulley board numbers? @Jinra

One mile at 15mph seems a good test but the variation in kv and gearing will make it unbalanced and have to see.  I guess I could just lower voltage to get to 80% no load at that speed...although very rarely someone @trampa states different voltages will change efficiency performance  

We could use the results to see if the computer simulations are accurate
```

---
## \#100 Posted by: KMeyerson Posted at: 2016-12-13T17:50:49.753Z Reads: 100

```
I'm glad you also bring up hall sensor temp maxes. I sent Enertion a PM about this, but they didn't seem too concerned. Only time will tell.
```

---
## \#101 Posted by: KMeyerson Posted at: 2016-12-13T17:51:58.835Z Reads: 99

```
What seems like a really important thing to build and design as a community is a universal dynamometer we can all compare things on.

There are a few different projects going on to make this happen, but a community effort might be a great thing.
```

---
## \#102 Posted by: Hummie Posted at: 2016-12-13T18:08:33.955Z Reads: 90

```
A dyno can't be everywhere though and requires everything come to it, but with the vesc and if we came up with a standard test it'd be just as good maybe - Distance to watthours consumed at different speeds. At higher speeds air resistance and the rider profile becomes important but with similar sized riders in the same position should be pretty good
```

---
## \#103 Posted by: KMeyerson Posted at: 2016-12-14T00:56:12.412Z Reads: 91

```
I mean we build a dynamo that can be 3D printed or laser cute for a nominal price AND supply a motor with known constants so we can ALL study motors with something of a standard.
```

---
## \#104 Posted by: Pedrodemio Posted at: 2016-12-14T01:19:05.311Z Reads: 93

```
That would be great and not so hard, my plan for now is to build a inertia dynamometer, the downside is that we can only obtain the torque curve, but not test at a fixed rpm/torque for long time, but hey, its cheap
```

---
## \#105 Posted by: KMeyerson Posted at: 2016-12-14T02:29:59.809Z Reads: 94

```
It would be a start.

With some work, we could repurpose old VESCs to create a variable load for standard testing.  Plenty of programming memory!
```

---
## \#106 Posted by: Jinra Posted at: 2016-12-14T03:19:01.918Z Reads: 94

```
What are you proposing?
```

---
## \#107 Posted by: KMeyerson Posted at: 2016-12-14T04:10:46.558Z Reads: 93

```
The Action Blink 4WD will be interesting. I look forward to mine in March.  It'll give me hope and something to improve on.  It's a pro version of what we already have developed as a community.
```

---
## \#108 Posted by: Trillium Posted at: 2016-12-14T05:50:07.395Z Reads: 96

```
Like I said, I have a dyno and the software is on trial but if/when I buy it it's $500. Highly discourage 3D printed dynos. Fast spinning objects + heat + plastic + inconsistency of 3D print asking for injuries and frustration.

I'm totally willing to setup others motors. There is some cost in adapting others  motors to my setup.. easiest would be to have a complete wheel with urethane ready to go. I can load up to at least 2kW for short periods. Resolution is 0.00263 Nm at 2.5Hz or 0.036 Nm at 200Hz, up to 50Nm. I'm in LA, just ship me your shit.

I might have a christmas surprise for you all if parts arrive on time, however I will probably be thermally loading it with field weakening until my urethane is made properly.

I would like to see a sub 700 gram hub motor that is still useful and doesn't get too hot. I hope my design fulfills that goal, although to get to that point I think I will need some thermal FEA software.
```

---
## \#109 Posted by: Trillium Posted at: 2016-12-14T06:07:34.055Z Reads: 94

```
There lacks innovation in winding / copper fill optimization, largely because there hasn't been a need for high powered micro motors because most people just make it bigger and accept the huge weight and size and bulkiness difference. If you can get 90% slot fill with most of these hubs, you're in happy place. I think 3D printed motors are the future... Where you have the machine sintering copper and silicon steel in one operation, adding gaps between winds to create your insulation.
```

---
## \#110 Posted by: Mellow Posted at: 2016-12-14T08:14:43.689Z Reads: 106

```
Thanks, @Hummie. Yes, our torque curve remains flat at 7Nm until around 28 kph - dropping to 5 Nm at 40 kmh. This is **total** torque so divide by 2 for one motor.  We're at 70% implementation of the full capability (don't want to cook any more motors than we have; our last two months will be used wisely). Feedback from assembled testers (of different riding levels) is a mix of shock, awe and....fear. So we have come acceleration shaping and smoothing to do.

@Pedrodemio The instagram shot has a misspelling on the Excel tab; the efficiency graph was for a Boosted Dual+, not the Mellow. Our analyses with our dyno showed max torque of 9.8 Nm (total) and then a rather steep descent to 0Nm at 35 kmh making it hard to see where field weakening starts. Max mechanical power _output_ was 820W.  The cells are capable of 70A continuous, but the system of course never goes that high. 

BTW, anyone else playing with dynamic field weakening?
```

---
## \#111 Posted by: trampa Posted at: 2016-12-14T08:14:49.674Z Reads: 107

```
The Action Blink 4WD looks like having the ready made Chinese motors on. They just look 100% the same.
Urethane is just a bit different....
I thought: Well, they just made some futuristic looking board, based on the Chinese stuff available, and cashed in. There is a lot of stuff like that going on on KS and Indiegogo. You just make your crowd believe..... It works.  http://winboardskateboard.en.ec21.com/

Frank
```

---
## \#112 Posted by: Trillium Posted at: 2016-12-14T09:28:26.816Z Reads: 108

```
Just building the market up for us. lol
```

---
## \#113 Posted by: Trillium Posted at: 2016-12-14T09:31:52.091Z Reads: 111

```
80mm wheel or? I wouldn't expect many complaints.
```

---
## \#114 Posted by: Pedrodemio Posted at: 2016-12-14T10:21:47.311Z Reads: 115

```
I saw that something was not adding up, the graph was too different than the previous one, if in the future after the release of Mellow you could release your hub efficiency graph, that would be great

Mellow should not be left behind a lot according to this data, maybe even pass when speed catches up
```

---
## \#115 Posted by: Mellow Posted at: 2016-12-14T16:48:27.770Z Reads: 115

```
@Trillium 80mm wheel.  

We've used the dyno to do for pre-builts what @KMeyerson is doing with you all here. We've done a full workup on efficiency, torque, power, etc for Carbon GT, Boosted Dual+, Onan X-1, Stary and an Evolve Pintail, and are *very* happy where we stand. @Pedrodemio As you have surmised: we do catch up to the Dual+ eventually. Our torque curves cross each other at 13 km/h. Hubs can and will compete with the belt drives performance-wise. We'll release the charts in the near future.
```

---
## \#116 Posted by: KMeyerson Posted at: 2016-12-14T17:59:12.070Z Reads: 119

```
@Mellow Thank you for the support.  In a product oriented community, its not often that we get support in development/pioneering a project, since its easier for people to criticize and throw money at problems.

So guys, its clear that we need a half decent bench testing solution we can all reference.  Laser Cut aluminum or CNCed aluminum frame dynamometer.  We need a community effort to build one for BLDC testing.

**Boosted's in house Dynamometer from their early days:**
<img src=https://phaven-prod.s3.amazonaws.com/files/image_part/asset/986136/UMC3xrLKAMBeJZH1Qkg-IVb6VlI/medium_Boosted-Dyno2Sml.jpg>

**Preliminary VESC Based Dynamometer (DATED, but useful):**
http://i.imgur.com/poDt1gP.jpg

With the VESC 6.0, we can have higher resolution data from the motors we use in testing.  While we wait, lets consider the best way to test motors by considering how to BUILD a rig for hub motors.  We could build a custom can/rotor that connects to the shaft, but thats additional milling for every motor. A Wheel-to-Wheel test might work, but we have mechanical losses.  I'm pretty good at AutoCAD and Solidworks, but I need someone to do the mechanical engineering here to reduce losses. Anyone with me? If so, PM me. Otherwise, I'll create a new thread about a community driven Dynamometer.
```

---
## \#117 Posted by: Pedrodemio Posted at: 2016-12-14T18:59:17.610Z Reads: 108

```
I'm in but let's keep all open, and I can help on the mechanical part

In my opinion the better aproach to be cheap and easy and to make is to use friction, a bike disc brake and caliper, a load cell taken out os a cheap scale or bought, an arduino and we are done
The vesc send info to the arduino, same for the load cell, with that info we can make a simple mechanism to apply brake, that can be manual or servo driven, on the latter we can make a routine to automatically generate a torque/current/efficiency curve
```

---
## \#118 Posted by: KMeyerson Posted at: 2016-12-14T19:11:22.495Z Reads: 106

```
That's a great start.  I like the idea of using a disk break instead of another BLDC.

I'm going to get some basic information together and start a thread tonight.
```

---
## \#119 Posted by: Pedrodemio Posted at: 2016-12-14T19:13:33.221Z Reads: 106

```
Nice, we continue the discussion there to not go off topic
```

---
## \#120 Posted by: trampa Posted at: 2016-12-14T19:35:17.119Z Reads: 108

```
I think a generator would be better. It will be hard to use a disc brake as sort of standard.
You want a well defined and measurable resistance. You need to know the output power to measure the efficiency. If you know your generator it's easy to straights out the numbers.  Define a cheap generator everyone has access to and standard is set.
Mechanics should be easy to sort out. Some alloy and wood...


Frank
```

---
## \#121 Posted by: Pedrodemio Posted at: 2016-12-14T19:36:07.385Z Reads: 114

```
The programming will be quite simple, seen in the image bellow, we just have to test how stable is the torque using the brake

The test will be completely automatic and will generate in one run torque vs speed vs efficiency

I'm just a bit worried if the brake disc will end the test on a acceptable temperature, I think a big fan pointed at it will be needed and incorporate cooling time and stabilization time, or in another aproach, make each measurement so quick that it don't have time to heat up, Just have to check if the data is stable in short periods or if we will have to round and filter it over a period of time 

<img src="/uploads/db1493/original/3X/0/e/0e4e10a666d2be851b21081ad9f6e4dd0a9ae528.jpg" width="375" height="500">
```

---
## \#122 Posted by: Pedrodemio Posted at: 2016-12-14T19:46:50.654Z Reads: 107

```
The disc brake doesn't matter, what we need is the torque that it generates, so the load cell matters, but that can be easily calibrated using a portable dynamometer, the ones used to tighten bolts
```

---
## \#123 Posted by: Trillium Posted at: 2016-12-14T20:18:11.829Z Reads: 107

```
Would you mind to share the excel data for the competitors to you and not yours? It's not critical to my development but would be nice to have.
```

---
## \#124 Posted by: KMeyerson Posted at: 2016-12-14T20:40:12.649Z Reads: 109

```
This is a community driven process. We'll have some form of database I think.
```

---
## \#125 Posted by: KMeyerson Posted at: 2016-12-14T22:56:15.052Z Reads: 106

```
Heads up, I have created the thread regarding Dynamometer to properly split the topic. Look for it under innovations.
```

---
## \#126 Posted by: Trillium Posted at: 2016-12-15T05:39:29.144Z Reads: 104

```
Is the stator on your website the same one that's in your motor or is that just a dummy stator with unrealistic pole count and such you used to camouflage your design?
```

---
## \#127 Posted by: Mellow Posted at: 2016-12-15T06:46:20.769Z Reads: 103

```
We'll share studies on all we tested, including ours, in the near future. 

The stator is our actual one. Check out the Mellow subforum here, or the MellowBoards subreddit on Reddit for more.
```

---
## \#128 Posted by: Trillium Posted at: 2016-12-15T08:24:32.943Z Reads: 98

```
What is the steady state temp of your motor cover / hanger?
```

---
## \#129 Posted by: PB1 Posted at: 2016-12-16T20:57:25.068Z Reads: 100

```
guys, kudos for this thread

In my opinion this is one of the most informative, valuable and civilized discussions on this forum. 

Respect
```

---
## \#130 Posted by: KMeyerson Posted at: 2016-12-16T21:26:01.076Z Reads: 95

```
It's a study of science by engineers and design practitioners.  With any luck, we can pioneer something great.
```

---
## \#131 Posted by: KMeyerson Posted at: 2016-12-19T05:45:54.371Z Reads: 102

```
**Progress Update**

This is how a hub motor should behave.  It's only taken a few months of simulation to get here. With a 4WD setup, less heat is generated per motor when starting so the temperatures tend to stay pretty cool. Practically, the thermal results indicate you wouldn't want to push more than 1.5 hours of riding time and definitely half that if you're going up hills constantly. Two motors aren't strong enough and wouldn't stay cool under those conditions with 100kg of human..  Looking at the data, I wonder how close these results are to the specs from the Action Blink Quatro.

Easy to replace stators/inexpensive recycling or rewinding would be a victory.

<img src="/uploads/db1493/original/3X/0/c/0cecd09f69810a13840a59c951b68bf0d1f4dc52.png" width="690" height="335">
<img src="/uploads/db1493/original/3X/0/8/08b7577eac08356834833f66fd8bc6fd4e738f0a.png" width="690" height="253">
<img src="/uploads/db1493/original/3X/2/c/2cba24de791fd7d04075353987d27eace473e55a.png" width="690" height="479">
```

---
## \#132 Posted by: Pedrodemio Posted at: 2016-12-19T09:33:13.009Z Reads: 100

```
And what about a forced air cooling? I think going 4wd is a major drawback that most people, incluindo me, would not do
But sure that flat torque curve is pleasing

The loses are linear with torque? Maybe you could could run the simulation with 1/2 and 1/4 of the current just tô see what we get, in the average course you would never be using full torque constantly

I noticed that the torque versus grade that you are using are significantly higher than what I calculated(80mm wheels 90kg person and taking in account aerodynamic drag)

<img src="/uploads/db1493/original/3X/2/f/2f174ca1bdecb2552a26eddf33d64f569fb2e285.JPG" width="690" height="339">

Edit: did you used the diameter of the wheel on your spreadsheet? It should be the radius, if I divide your results by 2 they agree with what I found
```

---
## \#133 Posted by: Ackmaniac Posted at: 2016-12-19T10:15:15.351Z Reads: 96

```
Isn't it that the cooling effect get's stronger the higher the temperatur difference is between the motor and the air. Because it seems that this isn't taken into account in your graph.
```

---
## \#134 Posted by: KMeyerson Posted at: 2016-12-19T17:37:26.831Z Reads: 100

```
@Pedrodemio, I want the motor to achieve kick ass at 75%, not 100%.  This is going to make the motor survive for longer and perform better. More head room.


 @Ackmaniac, It is, but I can't calculate forced air Coolings efficiency for something this small.  It would have to be measured, not calculated then included in the simulation.  I do not know how well ventilated my rotor will be since I am still playing with cap designs.  I am limited by the 5Axis CNC mills I can use. An impeller seems like the best idea, but idk if it would survive 100kg hitting a crack at 30mph.  Solidworks syas it would, but it assumes perfect quality aluminum.  Titanium is too expensive and hard to mill right now, so I'll look into that later.
```

---
## \#135 Posted by: Pedrodemio Posted at: 2019-02-15T01:25:13.657Z Reads: 26

```
Digging this old thread

@KMeyerson it's been a while since you logged here, but what end become your hub?

For anyone wanting to play. Infolytica was bought by Siemens recently and now the MotorSolve online trial is much more powerfull, with the thermal module included and lasts for 15 days

https://www.mentor.com/products/product-eval/motosolve-cloud-base-trial?sfm=free_form
```

---
