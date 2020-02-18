# THE Overkill - 4WD 36KW 20S13P 100+MPH build from scratch

### Replies: 363 Views: 16648

## \#1 Posted by: FullMetal_Machinist Posted at: 2019-01-19T19:33:25.938Z Reads: 1471

```
Hi everyone.

Got far enough with my build to share it.
Main concept was to build something so ridiculous and poweful that i will never want to build or ride anything else. Figured that some Guiness Records can also be made.
Completely disregarded difficulty and cost (currently estimated at $9k).
_Someone is sure to comment that with such budget one should buy two Bajaboards - my answer is that my board will be faster while PULLING BOTH Bajaboards_ with respective riders than original Bajaboard and will get further on a single charge, while pulling.
After debating for a while decided to go for 20S bencause currents are half of that on 10s and battery pack will fit nicely under entire deck.
Ordered 260 pcs of LG HG2 cells (same as SONY VTC6 only twice as good cycle life).
Arranged at 20S13P. Photos as follows, including that of elastic 8x2,5mm2 joint between sections:
![47|666x500](upload://qC8gR4Tb9eB2B41JmYj1D9iFtjO.jpeg) ![47%5B01%5D|666x500](upload://8dHjjm9qgAYFPgSqstQINmWnUrY.jpeg) ![05|666x500](upload://xYAuA4YvZjqPj2RXuiNbIoQk6al.jpeg) 
Battery is 700mm long, 220mm wide, 50mm thick and weighs 12.5 KG. Can supply 260 Amps continous and about 600 for 10 seconds at 72 volts sagged under load 84 volts nominal. It has 3000 watt hours capacity, several times that of any other build i have seen.
It will go into moulded monocque carbon fiber casing under the deck.
Deck itself is custom made , photos to follow when finished. Now making mould. Similiar in shape to NEXT BLACK CHILI but thicker stronger and 100mm longer, 300 wide in center.
Trucks are modified Trampa Infinity - strongest i could find, did not want to make my own.
Axle was removed to prevent temper loss and bracket welded at the end of the truck, then machined and axle inserted again with glue.
Bracket holds motor stator, rotor is the wheel hub itself. Real Hub Motors.
Photos:
![40|666x500](upload://ypKW7KMzHX7ThjlazVQmBbMUdu9.jpeg) 
Motor stator is taken from these motors:
http://store-en.tmotor.com/goods.php?id=330
3 such motors are taken apart, windings removed and iron core stacked and press-fit onto self-made retaining cup, which connects by screws to the welded flange. Per each wheel. 12 total.
Then winding with copper strands will follow, for targeted 50Kv, at 1 turn per pole, under 8 AWG thickness.
Motor continous current 150 amps, 350 for 10 seconds. 60Nm of torque per motor, 240 total, which at tire radius of 125mm gives 195 kilograms of driving force. Enough to smoke all four gokart supersofts at any speed up to 80 kph (50 mph), when power limit of the battery takes over and torque begins to drop.
And wheel hub:
![30|666x500](upload://tKCnYiBhomA6f1JnQTo2ziI1vdV.jpeg) ![29|666x500](upload://fCFNMoqp3I2q7jMMFBRvc4eU1Yq.jpeg) 
Magnets of N52 power are then glued inside of the hub, photos to follow later when all finished.
Tubeless tire of 9 to 12 inches diameter is mounted by removing outer ring, held by 9 black screws.
Later an ring adaptor to mount tires with 5in internal diameter is planned for the board to use gocart supersoft slicks (crucial to use power at 1,7 friction factor).
With such engines board will do 100 kph (60 mph) in 2,6 seconds with 70kg rider, about as fast as a liter sports bike. For cars only tire smoke will be left.
All that is left is the ESC to handle such abnormal conditions.
Designed based on VESC 4.12, from which an MCU and firmware is taken (i cannot program an MCU myself). Took about 6 months to figure out. Board size 100x92mm.
![VESC10|625x500](upload://ryMqT71ApfWGtcnbCI25jUZCpUW.jpeg) 
Power stage designed from scratch, features 36 power mosfets at 0,6 miliohm equivalent resistance per branch. Currently waiting for the PCB (ordered custom made 4-layered 3Oz copper boards in China and waiting for arrival, should come before january meets its end).
Assembly will be done by me in a proper reflow oven and will take about a day, parts already stocked.
Absolute limits should be 150 motor amps continous without cooling, 300 with good cooling, 600 pulsed. At 20S. Per ESC. There are four of them.

That is all for now, updates to follow whenever i have spare time and money (conjunctive).

FullMetal Machinist
```

---
## \#2 Posted by: okp Posted at: 2019-01-19T19:35:12.288Z Reads: 1323

```
wow. that's gonna be insane.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-01-19T19:39:14.553Z Reads: 1319

```
What deck you gonna use lol!
```

---
## \#4 Posted by: Grozniy Posted at: 2019-01-19T19:40:02.777Z Reads: 1299

```
I love it. Keep it updated
```

---
## \#5 Posted by: Arek Posted at: 2019-01-19T19:40:07.115Z Reads: 1268

```
No positive side paper isolators on this bomb? :open_mouth:
```

---
## \#6 Posted by: Indiangummy Posted at: 2019-01-19T19:41:26.200Z Reads: 1248

```

https://www.electric-skateboard.builders/t/bioboards-thorium-x4-4wd-geared-drive-custom-made-evo-style-board-caliber-2-baseplate-fatboy-230-hanger-12s6p-30q-4x-vesc-6-6-4xfatboy-gear-drive-4x-6374-special-ordered-motors-metro-pro-abec-11-107mm/69348/5?u=indiangummy

Just gonna leave this here
```

---
## \#7 Posted by: Sebike Posted at: 2019-01-19T19:47:21.783Z Reads: 1196

```
This is the most insane esk8 related thing I have ever seen. 
100 mph and a monster truck sized battery. 

Only because you can I guess. :dizzy_face:
```

---
## \#8 Posted by: FullMetal_Machinist Posted at: 2019-01-19T19:52:11.520Z Reads: 1196

```
There is no need for them bencause of the way sections are connected positive of one section goes directly to the negative of next section. Only insulation required is between battery halves and it is present at 3mm of pcb laminate + pvc cable duct in the middle. Battery will go into shrink wrap after it is tested under full 600 amp load and every cell nickel strip welding is verified.
```

---
## \#9 Posted by: Hummie Posted at: 2019-01-19T19:57:13.288Z Reads: 1211

```
![image|666x500](upload://lFmJh4No4v8YulEQivQHINLdYYI.jpeg) https://www.electric-skateboard.builders/uploads/db1493/original/3X/e/e/ee21124ba1138d4e4c01aa1159cf625b6dc96ab9.jpeg
Some of those sharp edges could cut through the insulation to the negative being squeezed in an enclosure. Very easy to do.
```

---
## \#10 Posted by: Jacobee Posted at: 2019-01-19T19:59:41.319Z Reads: 1138

```
This is absolutely insane! What esc are you using?

Edit: I see a 4.12 based are you sure that can handle 20s?
```

---
## \#11 Posted by: Arek Posted at: 2019-01-19T20:00:34.493Z Reads: 1129

```
I know but you can still short positive to negative of the cell itself, because negative wraps around positive and if you pierce top isulation which is very weak, you short it.
Check out some pics of unwrapped 18650s.
```

---
## \#12 Posted by: FullMetal_Machinist Posted at: 2019-01-19T20:05:53.048Z Reads: 1120

```
Fortunately HG2's have thick paper spacer just under the wrap (look closely), unlike VTC6, no need to double it, also when i looked at individual sections i tried to remove edges facing inwards with flat pliers. Unfortunately cell welding was done by external company and required some extra work, including wiring. They only welded nickel for me.
```

---
## \#13 Posted by: legend27 Posted at: 2019-01-19T20:09:31.919Z Reads: 1090

```
THAT'S INSANE! I LOVE IT!!!

10char?
```

---
## \#14 Posted by: FullMetal_Machinist Posted at: 2019-01-19T20:09:38.052Z Reads: 1082

```
The weakest link are the mosfets. If replaced with different model it will handle 24S, but at the expense of increased equivalent serial resistance to about 1 miliohm. Not worth doubling heat output. At 20S i still have 20 volts margin left on weakest component, 40 volts on drivers and other circuitry.
```

---
## \#15 Posted by: epss4 Posted at: 2019-01-19T20:30:10.226Z Reads: 1070

```
Wow incredible
```

---
## \#16 Posted by: topcloud Posted at: 2019-01-19T20:46:25.091Z Reads: 1070

```
@MoeStooge
```

---
## \#17 Posted by: Sebike Posted at: 2019-01-19T20:49:03.065Z Reads: 1091

```
[quote="FullMetal_Machinist, post:1, topic:81410"]
board will do 100 kph (60 mph) in 2,6 seconds with 70kg rider
[/quote]

How are you going to prevent the rider from being thrown off the board at such a crazy acceleration and speed? 

Strapped to the board? Epoxy? :thinking:
```

---
## \#18 Posted by: Andy87 Posted at: 2019-01-19T20:50:31.265Z Reads: 1072

```
Velcron 😜[](http://)
```

---
## \#19 Posted by: FullMetal_Machinist Posted at: 2019-01-19T20:53:21.454Z Reads: 1075

```
Good quality carbon snowboard bindings (= strapped to the board) + very low kneeling position, moved waaay over front of the board + extra hand holder for my left hand at the front of the board. Plus a lot of practice. And one loose screw.
```

---
## \#20 Posted by: Superflim Posted at: 2019-01-19T20:55:14.900Z Reads: 1072

```
[quote="FullMetal_Machinist, post:19, topic:81410"]
And one loose screw.
[/quote]

HAHA :rofl::rofl:
```

---
## \#21 Posted by: Titoxd10001 Posted at: 2019-01-19T20:57:02.571Z Reads: 989

```
Trampa truck? Strapped to the board? 100mph? How fast have you ridden before? Custom trucks would be must imo something like @MoeStooge has proven works
```

---
## \#22 Posted by: Grozniy Posted at: 2019-01-19T20:57:09.693Z Reads: 948

```
It's: 10Jason
:unamused:
```

---
## \#23 Posted by: Sebike Posted at: 2019-01-19T20:59:24.878Z Reads: 949

```
no <nothing></nothing>
```

---
## \#24 Posted by: Adam0311 Posted at: 2019-01-19T21:01:22.536Z Reads: 971

```
[quote="topcloud, post:16, topic:81410, full:true"]
@MoeStooge
[/quote]
What @topcloud said. You seem to know what your about, but it might worth your time to chat with @MoeStooge he builds and rides the craziest speed boards I’ve seen.
```

---
## \#25 Posted by: Andy87 Posted at: 2019-01-19T21:02:30.783Z Reads: 940

```
Anything planed to prevent speed wobbles?
```

---
## \#26 Posted by: FullMetal_Machinist Posted at: 2019-01-19T21:02:36.583Z Reads: 971

```
I have been pulled by a motorbike with 20ft of rope on my regular NEXT Blach Chili at about 70 kph without crashing in the woods. It is a flimsy board for a guy like me. This setup will have much stiffer deck and hydraulic shock absorbers size of 20ml syringes, one per wheel, to reduce speed wobble. When it appears i will do my best to reduce it without decreasing truck angle below 30*, which would make board unrideable in daily conditions.
```

---
## \#27 Posted by: Sebike Posted at: 2019-01-19T21:03:46.059Z Reads: 964

```
fixed hangers? :grin:
```

---
## \#28 Posted by: Andy87 Posted at: 2019-01-19T21:04:37.481Z Reads: 987

```
I have seen green dampas 😱😅
```

---
## \#29 Posted by: Sn4pz Posted at: 2019-01-19T21:10:37.945Z Reads: 1003

```
![wow|320x240](upload://qndS7LwZmx0oW4IEYvQnyOEzBFF.gif)
```

---
## \#30 Posted by: FullMetal_Machinist Posted at: 2019-01-19T21:12:57.192Z Reads: 989

```
Then look again AFTER it is bolted to the deck in few months. They come stock with green ones. I already have other dampers but have not changed them due to risk of damage during motor assembly (aggresive resin coatnig of windings involved). Besides with hydraulic system planned it will have very little effect on wobble itself, which is rapid oscillation of RIDER and board as a pair.
In the worst case scenario truck angle will be decreased _just for topspeed runs_ to a few (2-6) degrees in front and 0 rear. Making angled spacers with a bandsaw is fast enough.
```

---
## \#31 Posted by: totalgeek9224 Posted at: 2019-01-19T21:13:34.090Z Reads: 946

```
Mental
<Idjdh>
```

---
## \#32 Posted by: Allofyoush Posted at: 2019-01-19T21:13:36.105Z Reads: 936

```
Goddamn. You're making a car for your feet. This will be interesting.
```

---
## \#33 Posted by: linsus Posted at: 2019-01-19T21:59:48.012Z Reads: 904

```
Holy shit thats a costly build! 😂
```

---
## \#34 Posted by: linsus Posted at: 2019-01-19T22:03:19.976Z Reads: 896

```
That board is power reserve for a house in a blackout 🤣
```

---
## \#36 Posted by: banjaxxed Posted at: 2019-01-19T23:21:15.987Z Reads: 909

```
This is insane in a good way, but sadly also very demoralizing for anyone mid-build 😢 in terms of what you are able to achieve in comparison, this is awesome keep posting it!

Subbed
```

---
## \#37 Posted by: pjotr47 Posted at: 2019-01-19T23:25:48.423Z Reads: 892

```
You are crazy! That will be a awesome board. You can even pull a car with that power.
```

---
## \#38 Posted by: Toughook Posted at: 2019-01-19T23:27:43.981Z Reads: 918

```
Always love to see people pushing the boundaries 👍
```

---
## \#39 Posted by: rojitor Posted at: 2019-01-19T23:30:34.775Z Reads: 919

```
Amazing project. Just one question...why?
```

---
## \#40 Posted by: Benjamin899 Posted at: 2019-01-19T23:31:25.072Z Reads: 912

```
why not build a offroad buggy^^
```

---
## \#41 Posted by: b264 Posted at: 2019-01-19T23:34:02.399Z Reads: 922

```
[quote="rojitor, post:39, topic:81410"]
Just one question…why?
[/quote]

Why not?&ZeroWidthSpace;
```

---
## \#42 Posted by: ZachTetra Posted at: 2019-01-19T23:34:33.198Z Reads: 851

```
How can you push 600A through the wires?  You could use a solid copper rod and it would still melt
```

---
## \#43 Posted by: b264 Posted at: 2019-01-19T23:34:52.078Z Reads: 843

```
Multiple wires
```

---
## \#44 Posted by: eb1925 Posted at: 2019-01-19T23:38:39.324Z Reads: 856

```
Holy hell

10char
```

---
## \#45 Posted by: dg798 Posted at: 2019-01-19T23:47:52.351Z Reads: 865

```
definitely watching this.
gonna be awesome!!!
```

---
## \#46 Posted by: rojitor Posted at: 2019-01-19T23:49:02.641Z Reads: 878

```
I'd like to know his motivation. Hence my question. I find It the most intriguing.
```

---
## \#47 Posted by: Sebike Posted at: 2019-01-19T23:54:38.517Z Reads: 914

```
That battery is not to mess with. 

Fully charged = 84 VDC!!

 I'm not sure I'd be comfortable assembling and mounting that battery and all the electronics. Would definitely use some kind of insulated electricians gloves. 

http://www.mid-westelectric.com/wp-content/uploads/2015/02/MWE7.jpg
```

---
## \#48 Posted by: FullMetal_Machinist Posted at: 2019-01-20T00:18:59.390Z Reads: 899

```
@rojitor :slightly_smiling_face: 3 years ago (was 27 at the time) my family would not allow me to buy a motorcycle. Told them i would build something 10x worse. They laughed. Rest is engineering.
btw. got a motorcycle last year and continuing with the build.
@sebike You can actually grab main terminals with bare hands and barely feel a tingle, unless you have very sweaty hands at the moment it is not this bad.
However battery is very dangerous bencause it would output over 2.000 amps during short circuit melting everything and blowing up in flames splendidly, and i would rather not see $1500 going up in smoke.
@Pedrodemio
Basically yes.
Torque would be 3x greater since i am "mating" 3 stators together plus then another +50% bencause of the magnets used - original motors have N38 magnet pole inductance of 9kGs, while mine N52 have 14kGs. It allows for a higher torque from same motor at the cost of more heat loss within core itself. For "normal" riding up to lets say 50km/h it wont be a problem and at the speed runs there wont be ebough time to overheat the motor. Eddy losses go with the square of the motor speed - 3x the speed 10x the losses. Especially that motor would spin only at 3.500 RPM at 200 km/h while it spun 8.000 in original application - drone propeller drive. Another benefit is that you need less winding turns for a given KV, which means a thicker wires and less conduction loss.
```

---
## \#49 Posted by: pat.speed Posted at: 2019-01-20T00:22:27.971Z Reads: 847

```
You need to be very careful. If you were to touch main terminals with opposite hands you could get a potentially lethal jolt through the chest/heart
```

---
## \#50 Posted by: Pedrodemio Posted at: 2019-01-20T00:24:02.057Z Reads: 843

```
@FullMetal_Machinist What a crazy build, love it

How did you achieved the figures for the hub motors? based on the original specs of the motors you teared down?
```

---
## \#51 Posted by: colinphotovideo Posted at: 2019-01-20T00:31:46.739Z Reads: 828

```
Damn this is mental but props to you, good luck with it! :smiley:
```

---
## \#52 Posted by: ryansinatra Posted at: 2019-01-20T00:36:07.935Z Reads: 830

```
[quote="banjaxxed, post:36, topic:81410"]
This is insane in a good way, but sadly also very demoralizing for anyone mid-build :cry:
[/quote]

For real 😂 I was so stoked about completing my (very average) drivetrain today. 

This is wild
```

---
## \#53 Posted by: Pedrodemio Posted at: 2019-01-20T00:42:26.780Z Reads: 783

```
Nice, please add temperature sensors to that so we can see how hot the motors got
```

---
## \#54 Posted by: Newbie-1 Posted at: 2019-01-20T00:44:56.124Z Reads: 786

```
R u trying 2 kill yourself?
```

---
## \#55 Posted by: Hummie Posted at: 2019-01-20T01:08:32.733Z Reads: 819

```
winding with 8awg wire sounds really hard but ideal with only having to do one turn:  You could maybe get a cast conductor completely filling the slot as apposed to cylindrical and lots of bare space.   after you wind it you should get some good stator glue to fix everyting against vibrations and shorting.  getting a 8awg wire to be solidly held on the stator sounds hella hard.  i'll wind a motor by pulling on a 17 or 16 awg with the other end fixed tight against a doorknob or something and I pull it on in tension but at 8 awg that's a work out and 3x the diameter.  getting the wire to bend around the teeth, maybe you'll need a tool.

with so many teeth on the stator what erpm would you have to hit to get to those high speeds?
```

---
## \#56 Posted by: banjaxxed Posted at: 2019-01-20T07:31:30.661Z Reads: 859

```
Hope you are looking at controlling the surrounding conditions when testing speed, if you lose it you will most likely be a highsiding & that hurts even without a tree 

I know you will be wearing your liter bike gear but spare a thought for the speed at which a get-off on an esk8 going say 85mph vs a motorbike, with a motorbike you have much more options in terms of laying bike down, sliding out etc.
An esk8 going that speed wil most likely rag-doll you, I would look at those instant inflatable vest over the motorbike jacket with a full back protector and top quality motorbike helmet.

[quote="Sebike, post:7, topic:81410"]
This is the most insane esk8
[/quote]

[quote="Jacobee, post:10, topic:81410"]
This is absolutely insane!
[/quote]

[quote="legend27, post:13, topic:81410"]
THAT’S INSANE!
[/quote]

[quote="totalgeek9224, post:31, topic:81410, full:true"]
Mental
[/quote]

[quote="banjaxxed, post:36, topic:81410"]
This is insane
[/quote]

[quote="pjotr47, post:37, topic:81410"]
You are crazy!
[/quote]

[quote="okp, post:2, topic:81410"]
gonna be insane
[/quote]
```

---
## \#57 Posted by: Chrisjarram Posted at: 2019-01-20T08:25:39.005Z Reads: 756

```
RIP.  Please leave it to me in your will :)
```

---
## \#58 Posted by: TowerCrisis Posted at: 2019-01-20T08:44:56.975Z Reads: 791

```
OFFS

You could not pay me to ride this thing.

Also, I hope you don't sweat under the stress of putting the electronics together 😂 moist hands don't mix well with that kinda voltage
```

---
## \#59 Posted by: evoheyax Posted at: 2019-01-20T08:46:56.532Z Reads: 831

```
Well I thought 200a at 12s was a lot... the one thing I can say from experience is be careful being strapped in to such a heavy board is dangerous. On lighter boards, you can lift it a little like a snowboard. But heavier boards that you strap into are trickery when falling.

The question I have for you is how are you going to get the traction to put that kind of power to the pavement? With that kind of power, I imagine your going to need a large contact patch.
```

---
## \#60 Posted by: sk8l8r Posted at: 2019-01-20T09:07:08.808Z Reads: 807

```
What about breaks?
```

---
## \#61 Posted by: mutantbass Posted at: 2019-01-20T09:19:57.793Z Reads: 800

```
Fuck me. I was one of the smartest kids in school. Now I feel dumb :rofl:

Can’t wait to see the final product
```

---
## \#62 Posted by: Chrisjarram Posted at: 2019-01-20T10:36:52.542Z Reads: 735

```
9 grand...
```

---
## \#63 Posted by: Chrisjarram Posted at: 2019-01-20T10:38:50.865Z Reads: 731

```
Might want to scotch tape a couple to his nipples too...
```

---
## \#64 Posted by: Vanarian Posted at: 2019-01-20T11:08:53.107Z Reads: 764

```
Careful with your n52 magnets, maybe you'd prefer n45h or n45sh to have safe overheating room (even n44h). 

Also, what made you choose LG HG2 over Samsung 30Q or even another format (Turnigy Graphene / Samsung 40T)? 

That's an insane build for sure, are you dead confident these trucks and dampers will be enough to take such speed and torque?
```

---
## \#65 Posted by: banjaxxed Posted at: 2019-01-20T11:25:05.500Z Reads: 763

```
I would strongly consider using...and I bite my knuckles saying it, Freebord bindings

 WHEN you come off, not breaking your legs is a plus

Have a look at @Nowind’s rubber dampers for the trucks to stabilize things

Consider using a motorbike steering damper like others
```

---
## \#66 Posted by: Pantata Posted at: 2019-01-20T11:30:39.408Z Reads: 724

```
Someone cares to explain the purpose of this? I can't think of any other than achieving meaningless records on a track... This is totally useless... Unless you weight 200 kg+
```

---
## \#67 Posted by: totalgeek9224 Posted at: 2019-01-20T11:32:25.551Z Reads: 735

```
[quote="Sebike, post:7, topic:81410"]
Only because you can I guess. :dizzy_face:
[/quote]
<hhdhfhhghgh>
```

---
## \#68 Posted by: Balta_6 Posted at: 2019-01-20T11:42:38.417Z Reads: 713

```
Would love to see some kind of motherboard thing, where other boards can charge with your battery, like some other did
```

---
## \#69 Posted by: banjaxxed Posted at: 2019-01-20T11:57:55.193Z Reads: 730

```
It's fairly obvious it's an engineering excercise, a possible record attempt and because he can from the intro

If it plays out like the first post I could see it winning hill events that aren't too extremely bendy
```

---
## \#70 Posted by: Pantata Posted at: 2019-01-20T12:00:04.569Z Reads: 732

```
Not sure how it makes any difference engineering wise, possible record ttempt doesn't make sense cause it's an overkill for physical reality we live in, unusable power, totally... I am not a hater, just saying this has nothing to do with riding electric boards and all to do with, as you say, "I can"  Doesn't make sense what so ever but I can... I agree with that.  BTW the world record is around 60 mph... And it is almost impossible to go that fast, only in perfect conditions, on a race track and with lots of luck...
```

---
## \#71 Posted by: b264 Posted at: 2019-01-20T12:03:17.990Z Reads: 704

```
This is very clearly a "toy" and not a "tool".  Let the man have some fun! :slight_smile:
```

---
## \#72 Posted by: banjaxxed Posted at: 2019-01-20T12:03:38.651Z Reads: 733

```
[quote="Pantata, post:70, topic:81410"]
possible record ttempt doesn’t make sense cause it’s an overkill for physical reality we live in, unusable power,
[/quote]

That's pretty much the definition of a motorised record breaker
```

---
## \#73 Posted by: Vanarian Posted at: 2019-01-20T12:05:50.704Z Reads: 755

```
https://cdn.discordapp.com/attachments/377558872765759491/536516562643976213/sketch-1547985845053.png

**It Begins**
```

---
## \#74 Posted by: Riako Posted at: 2019-01-20T12:06:35.636Z Reads: 784

```
**Epic build !!!**... I'm still stocked :dizzy_face: ... So I seat here !!

Don't know what to say except maybe  **Happy DIY mate** :muscle: :crazy_face::call_me_hand:

EDIT ! I haven't taken time to notice your pseudo :heart_eyes:

https://media.tenor.com/images/c372875b8e2b989c999f8e6073196ae5/tenor.gif
```

---
## \#75 Posted by: banjaxxed Posted at: 2019-01-20T12:06:45.741Z Reads: 799

```
https://watchyourselves.com/airbag-vests-jackets-motorcycle-equestrian/

Some jackets here ^

@Nowind dampers 
 https://www.e-toxx-shop.com/trampa/elastomere-damper/#cc-m-product-10002752170

Steering damper mount 
https://www.e-toxx-shop.com/trampa/steering-damper/#cc-m-product-9945270570
```

---
## \#76 Posted by: Andy87 Posted at: 2019-01-20T12:20:37.219Z Reads: 778

```
As much as i love the elastomer damper i don’t think they will work with 100km/h +

And I think @FullMetal_Machinist already found a steering solution.
He mentioned how some posts ago.

https://www.electric-skateboard.builders/t/the-overkill-4wd-36kw-20s13p-100-mph-build-from-scratch/81410/30?u=andy87
```

---
## \#77 Posted by: Ackmaniac Posted at: 2019-01-20T12:26:44.543Z Reads: 746

```
The VESC 4.12 Hardware has a limitation of 60V at the DRV (doesn't matter if the mosfets can do more). So 13S is more or less the maximum it can handle with the standard schematics.
```

---
## \#78 Posted by: linsus Posted at: 2019-01-20T12:34:26.886Z Reads: 764

```
Since he spent half a year on it I'm guessing he switched the DRV. 
I was going to sudgest the 75/300 VESC but he has higher voltage then that too...
```

---
## \#79 Posted by: Winfly Posted at: 2019-01-20T12:38:24.053Z Reads: 768

```
I have seen 100v drv chips from Ti.
```

---
## \#80 Posted by: hazza Posted at: 2019-01-20T12:49:42.261Z Reads: 767

```
After an hour ride on my carbon gt my back leg hurts from the acceleration. I wonder how this would accelerate and how well the vesc traction control will handle it.
```

---
## \#81 Posted by: b264 Posted at: 2019-01-20T13:14:55.136Z Reads: 752

```
The DRV8353 is 100V
```

---
## \#82 Posted by: banjaxxed Posted at: 2019-01-20T14:18:40.745Z Reads: 708

```
The ESC is of interest what’s going on there? Hubs design is great for keeping the weight down but why so many P in the pack, surely a 7/8P would prove the point or is it to have long range as well?

A separate smaller P lipo pack for the speed challenge?
```

---
## \#83 Posted by: taz Posted at: 2019-01-20T14:22:30.109Z Reads: 689

```
That's a lot of power for a 7/8P pack. He will have too much voltage sag.
If it was me though I would go with Lipos, you can get a lot more current out of them and if you are not looking for range, going with Lipos will shave a lot of weight.
```

---
## \#84 Posted by: Sebike Posted at: 2019-01-20T14:24:55.051Z Reads: 681

```
If total weight is too little, this monster will lift off the ground or dig a hole in it 😂

Is a kamikaze machine without wings.
```

---
## \#85 Posted by: banjaxxed Posted at: 2019-01-20T14:32:44.210Z Reads: 670

```
Yeah I mean a drop in P and switch to Lipo for speed attempts, but ok the sag needs to be compensated for
```

---
## \#86 Posted by: Indiangummy Posted at: 2019-01-20T15:16:34.942Z Reads: 685

```
[quote="banjaxxed, post:85, topic:81410"]
but ok the sag needs to be compensated for
[/quote]

Wonder if there is anything else he is copensating for? 😂😂
```

---
## \#87 Posted by: banjaxxed Posted at: 2019-01-20T15:24:00.172Z Reads: 691

```
The target is the NXT record. They utilize a number of factors to get that record, pro DH skater, light weight, controlled conditions

This is a different approach & realistically who knows? but I would be concerned that it is akin to trying to get a speed record out of a muscle car, mind yourself!

Ps. Was that record beat by MoeStooge?
```

---
## \#88 Posted by: Battosaii Posted at: 2019-01-20T15:35:36.928Z Reads: 664

```
This is impressive but to me it sounds like your building more of a vehicle that you stand than an esk8.
```

---
## \#89 Posted by: mmaner Posted at: 2019-01-20T15:36:36.278Z Reads: 660

```
For the sake of disclosing all the info...

The board was dead at the end of the run, the end of the run was a crash. I'm not sure the record matters or is valid.
```

---
## \#90 Posted by: DerelictRobot Posted at: 2019-01-20T15:44:17.737Z Reads: 643

```
Which board we talking?
```

---
## \#91 Posted by: mmaner Posted at: 2019-01-20T15:57:29.171Z Reads: 641

```
The NXT board, speed world record.
```

---
## \#92 Posted by: NullReference Posted at: 2019-01-20T16:09:18.148Z Reads: 658

```
Godspeed, you magnificent bastard.

This reminds me of a great quote from George Mallory. When he was asked why he risked his life climbing Everest, he replied “Because it’s there.”

Make sure someone else is there to record your speed run. We need to see that footage.
```

---
## \#93 Posted by: Blitz Posted at: 2019-01-20T16:13:51.225Z Reads: 655

```
I mean dude really?
Is a picasso painting a toy because it's not a tool?

Hearing you call someone's esk8 a toy because it's not as practical as yours sounds hypocritical but then again I guess we should all just relax and enjoy this hobby however we see fit.
```

---
## \#94 Posted by: MoeStooge Posted at: 2019-01-20T16:20:15.514Z Reads: 657

```
If anyone is interested in officially breaking the record, the board and rider are standing by ready.  https://youtu.be/Hsj9guNrlmU
```

---
## \#95 Posted by: b264 Posted at: 2019-01-20T16:26:59.888Z Reads: 651

```
[quote="Blitz, post:93, topic:81410"]
Is a picasso painting a toy because it’s not a tool?
[/quote]

Yes.&ZeroWidthSpace;
```

---
## \#96 Posted by: mikenyc Posted at: 2019-01-20T17:49:07.969Z Reads: 626

```
Are they still around? @ngv-nextboards
```

---
## \#97 Posted by: mmaner Posted at: 2019-01-20T18:52:27.631Z Reads: 622

```
No clue, haven't seen then recently.
```

---
## \#98 Posted by: Hummie Posted at: 2019-01-20T19:05:28.500Z Reads: 657

```
yea if you fall off right after the speed sensor going for the record, or maybe he fell off even at the speed sensor, that seems an invalid result.  Im surprised guiness records accepted it.   


I think moe came off at  like 50mph with a crazy rear truck speed wobble, or maybe he was faster.   there's great video of it somewhere filled by bigboytoys I think
```

---
## \#99 Posted by: FullMetal_Machinist Posted at: 2019-01-20T20:17:40.514Z Reads: 710

```
Considered going for LiPo packs but decided against it.
Going by the maximum current i would need at least 3500mah 50C per motor, more realistic is something like
https://hobbyking.com/en_us/turnigy-nano-tech-4500mah-5s-35-70c-lipo-pack-xt-60.html  with 4 of them wired in series for each motor. It means total of 16, meaning 9 kgs of battery for 18AH capacity.
16 Pcs of 65E each + shitload of connectors costs same as 18650 pack.
Could not go with one pack per board bencause it would not support the current. Packs are terminated with XT90 plugs which is barely acceptable for a single wheel. With my pack i go with XT150 and 6mm2 wires per each ESC.Afer the connector there is a capacitor bank, wiring between capacitor bank and ESC will be 16mm2. Output wiring also 10 or 16mm2 not decided yet.
With LIion i get 40AH at 12,5 kgs. 
If i went hardcore for 2000mah 100c packs it would be lighter but with little usable range, only good for maximum acceleration test at 7 kgs lighter. Cost again same as 18650.
Cycle life is another beast - lipo gets 100 cycles, HG2 gets 600 cycles at 20 amps to 80% capacity.
At the smaller capacity i would go through the cycles twice as fast, meaning hg2 is 10x more durable than lipo.
Charging the packs would be a nightmare, with 16 packs to charge and balance. This is after you get them out of the board. Each frigging time.
So i went with liion 18650, 20700 have smaller energy and power per unit of weight (for now).
13P is the result of battery layout under the deck. If i went with 2 layers of cells it would be 9P which is too small - at max current each cell would get 60 amps, sag would be a problem. 3 layers let me fit 13 cells in pararel, which tops at 40 amps per cell, good enough.
```

---
## \#100 Posted by: FullMetal_Machinist Posted at: 2019-01-20T20:37:50.459Z Reads: 726

```
@MoeStooge
Speakig the truth i am in awe of what you accomplished already. Your creation is faster than existing record and after sorting wobbling it will get even faster. Perhaps even 150 Kph.
You got there utilising conventional, orthodox methods improved steadily over decades. It is based on existing, high quality components. It is the safest approach and will yield good results over time, no discussion about it.
My approach is throwing everything we know out of the window and starting form scratch with little knowledge about downhill speed skating and no experience. There exist no components meeting my criteria so i make my own, based on every bit of knowledge i can piece together to make some sense.
I am 99% certain that my build will get to 100Kph safely. It is sturdier, stiffer and heavier than the board that i took to 70 Kph. After that there is a barren land, waiting for the first explorers to get there.
I am 100% certain that my build will get speed wobble. Question is "at what speed". And how to move this limit forward.
**My project will end big. All i do not know is whether it will be a big crash or a big record.**
```

---
## \#101 Posted by: murdomeek Posted at: 2019-01-20T20:44:09.724Z Reads: 701

```
This is insane! 
I am super impressed at your still at custom winding your own hubmotors
As well as custom designing your own VESC

You an engineer by day? :)
```

---
## \#102 Posted by: FullMetal_Machinist Posted at: 2019-01-20T20:57:18.641Z Reads: 690

```
@hazza
i will not use vesc traction control, it is no good for 4wd with this much power. Reason is that you select 1 wheel as "master" and the rest follows. Front will have less traction than rear which blows it.
Inside the motors there will be additional hall sensors connected to separate TC board, all wheels independent. 
It will allow for much more control than build-in solution and accelerating with rear while braking with front for sharp turns with powerslide. Separate controls for braking and accelerating. 
@b264
Briefly considered using this chip but it has only 1 amp mosfet driving current and is slow as armored turtle. If you read the datasheet and understand it it becomes clear.
Chips i chose offer 6 amps driving current at 120 volts max supply, transients up to 150 volts and they can be connected in pararel to give even more current, which i did.
This will allow me to keep switching times very low, in the 10-15 ns range. Dead time will be something like 20 ns.
Original VESC 4.12 has a dead time setting of 180-220 ns. If i used DRV8353 it would be like 300ns with the amount of mosfets used and their combined gate capacities. Anything less blows the fets to heaven.
After my analysis i deduced that almost half of the heat in old vesc is generated not by conduction but by switching losses. Did not want that.
```

---
## \#103 Posted by: b264 Posted at: 2019-01-20T20:59:14.571Z Reads: 629

```
What chips did you choose with 6A driving current?
```

---
## \#104 Posted by: Hummie Posted at: 2019-01-20T21:09:24.175Z Reads: 626

```
But as said already how will you keep traction with that much power?  You’ll need super soft tires and lots of contact. I can spinout my tires on even my two normal hub motors using typical settings and 78duro
```

---
## \#105 Posted by: FullMetal_Machinist Posted at: 2019-01-20T21:09:29.209Z Reads: 631

```
Check Maxim  dual high side drivers on mouser, you will find them. 
For the rest of the people it is a company secret.
```

---
## \#106 Posted by: b264 Posted at: 2019-01-20T21:13:03.582Z Reads: 627

```
Beyond the actual traction limit of 4 wheels spinning, all the extra power beyond that should just be applied to making loud roaring sounds to make it seem even more powerful.
```

---
## \#107 Posted by: Hummie Posted at: 2019-01-20T21:33:48.413Z Reads: 653

```
It seems better to make it a street luge and then u could at least hold on.  

There’s surely some math revealing how much tire contact and what duro for what wattage at what weight to stay stuck to the road and not just burnout.   I think be worth doing.
```

---
## \#108 Posted by: ripcurldog Posted at: 2019-01-21T06:29:33.422Z Reads: 671

```
All Trampa electric mountain boards have foot straps, just like snowboarding.  That may seem nuts, but after riding my Evolve GT and my Trampa E-Mountainboard(strapped), I much prefer the foot straps.  There is a lot you can do with straps that you can't do without them (though falling truly sucks ass!)!
```

---
## \#109 Posted by: Westy Posted at: 2019-01-21T09:44:39.161Z Reads: 695

```
Holy shit

![oldest-wing-walker-header_tcm25-400245|580x327](upload://cxOm70rrVoLp4INEY3RLJ0w1y4Q.jpeg)
```

---
## \#110 Posted by: SoloSpaceMonkey Posted at: 2019-01-21T10:18:31.415Z Reads: 677

```
This is just insane! And I can't wait to see it when it's done. I will def. be following this build.
```

---
## \#111 Posted by: FullMetal_Machinist Posted at: 2019-01-21T12:25:36.295Z Reads: 677

```
Then get some snowboard bindings and ty it too. Tried both and stayed with snowboards.
Bindings alone give +20 Kph to speed wobble limit, control is much better and sharper. It allows much tighter turns.
I have several friends who do mountainboarding and all of them had injuries of either knee or ankle bencause during crash 1 foot got out of the strap and the other did not, twisting the leg.
With bindings you go visit the ditch together. Done that enough times.
Also the difference is that with bindings you 95% crash on your butt, which is actually better.
The only downside is that you cannot push yourself with your leg, which is of no importance on the electric.
```

---
## \#112 Posted by: banjaxxed Posted at: 2019-01-21T13:40:32.348Z Reads: 621

```
Not at the speed you’re aiming for, the two proper get offs I’ve had were with Trampa bindings with no heel straps, I came out of the bindings, flung really, but that was only 57kph and on sand. If you get into a wobbler there is no adjusting position
```

---
## \#113 Posted by: evoheyax Posted at: 2019-01-21T15:27:20.751Z Reads: 655

```
Since you seem to keep ignoring my and hummies question, I’m guessing you haven’t solve the traction issue. I can tell you with 10k watts 4wd with 78a urathene, I break traction on every full throttle acceleration. To put 8k to each wheel would mean you need almost 4 times as much traction as I have with my 78a duro wise contact patch urathene wheels.

I’m not trying to hate, but considering your building your own hub motors and I’ve yet to see any other eboard you’ve built, I’m trying to give you the inside experienced knowledge from someone whose been trying to push bouderies with his builds. I would be doubful if you can find a pneumatic that can take 4K watts per motor and not lose traction, none the less 8k. It just seems like you’ve picked some crazy specs arbitrarally without any experience of what something even a 4th of that is capable of.

As someone whose skated street for 11 years and eboards for almost 4 years, I can tell you that it is incredibally hard to commit to the acceleration at 10k watts. I’m sure the straps will help.

I guess my point is do the math on traction and figure out what will work. The last thing I want to see is you build these motors and realize you lose traction and need to redo the motors to fit a wheel with a bigger contact patch.
```

---
## \#114 Posted by: mishrasubhransu Posted at: 2019-01-21T15:36:14.672Z Reads: 599

```
He just has to put some lead blocks in the front and the back. Thankfully friction is proportional to normal force. But sure he needs the wheels that can handle that traction.
```

---
## \#115 Posted by: FullMetal_Machinist Posted at: 2019-01-21T15:43:11.779Z Reads: 620

```
I do not ignore, i have simply done my math.
Recalculate using torque instead of watts.
Your build has more torque per watt than mine at the expense of much lower top speed. I will get 240Nm on wheels at 1400 motor amps combined for 4 wheels. Battery being 20S plays a big role in those calculations, increasing top speed at given amps.
At tire radius 125mm it means 195 kgs of driving force.
Gokart supersofts have a friction coefficient of 1,6 which means that if the board + rider weighs more than 121 kgs tires wont spin. Urethane has half of this friction coefficient.  I top at 90 kgs, board will be hair short of 30 kgs. Math fits. If you do not believe use the calc yourself  https://calc.3dservisas.eu/ . Target motor kv 50 motor in wheel so 1:1 gearing ratio motor config 36s42p. Current per motor 350 amps.
```

---
## \#116 Posted by: evoheyax Posted at: 2019-01-21T15:47:06.064Z Reads: 587

```
I'm lost in your lipo math.

I run a 2x 6s5p packs to make a 12s pack from these cells: https://hobbyking.com/en_us/zippy-compact-5000mah-6s-25c-lipo-pack-xt90.html

With 5 in parallel, that's a 125c rating. And with 44.4 nominal as in my case, this is over 5000a. My 12s battery is only 6.5 kg. Now you wouldn't be able to hit 20s with this battery (18 or 24 yes), you can see this battery would be lighter than the li-ion and also far more powerful. It will also sag a lot less.
```

---
## \#117 Posted by: FullMetal_Machinist Posted at: 2019-01-21T15:52:17.170Z Reads: 571

```
Putting the cells in pararel does not increase C rating. Only the capacity.
If i put 4 cells of 5000mah 25C in pararel i get 20000mah still 25C, meaning 500 amps. Good.
Then to get to 20S i need to put 4 packs of 5S in series, which increases voltage but not the current.
4pack series x 4 packs pararel = 16 packs.
```

---
## \#118 Posted by: evoheyax Posted at: 2019-01-21T15:52:45.613Z Reads: 613

```
[quote="FullMetal_Machinist, post:115, topic:81410"]
Gokart supersofts
[/quote]

ok, sorry, missed where you mentioned your using go kart tires.

Still, not sure where you are, but I think you should try a really powerful 4wd before you get too deep. with 10k watts on 84mm urathene with 85kv, I hit 0-20mph in just over 2 seconds. Your going to theoretically do it in a 3rd of that time.
```

---
## \#119 Posted by: Kug3lis Posted at: 2019-01-21T15:52:58.650Z Reads: 631

```
I love how this build ignores physics :smiley:

Keep it up :)
```

---
## \#120 Posted by: barajabali Posted at: 2019-01-21T15:56:54.485Z Reads: 664

```
https://www.electric-skateboard.builders/t/biggest-battery-anyones-ever-used-in-eboard/7014

New Winner if this works out
```

---
## \#121 Posted by: FullMetal_Machinist Posted at: 2019-01-21T15:57:57.419Z Reads: 646

```
84mm 85kv is equal to  250mm 28kv (imagine you applied gearing). Mine is 2x greater at 50kv - 2x less torque per amp, 2x top speed per volt.

You get 20 MPH in 2 secs, i get 60 mph in 3 secs. Acceleration is 2x greater, so is the friction factor of the tires.
```

---
## \#122 Posted by: evoheyax Posted at: 2019-01-21T16:01:29.232Z Reads: 615

```
[quote="FullMetal_Machinist, post:117, topic:81410"]
Putting the cells in pararel does not increase C rating. Only the capacity.
[/quote]

Ah, my mistake. I get confused with c ratings because we don't talk about c ratings in any other chemistry than lipo. 

[quote="FullMetal_Machinist, post:117, topic:81410"]
4pack series x 4 packs pararel = 16 packs.
[/quote]

And 16 x 565g = 9040g, smaller than the 12kg li-ion pack.

But I do think that with lipos, I wouldn't take their ratings a face value.
```

---
## \#123 Posted by: evoheyax Posted at: 2019-01-21T16:07:31.699Z Reads: 616

```
[quote="FullMetal_Machinist, post:121, topic:81410"]
Acceleration is 2x greater, so is the friction factor of the tires.
[/quote]

Hm, interesting... I can't imagine doubling this acceleration though. Crazy stuff. You've clearly thought this all through very thoroughly.

Best of luck.
```

---
## \#124 Posted by: FullMetal_Machinist Posted at: 2019-01-21T16:55:39.374Z Reads: 614

```
Here you have the calc with filled board parameters:
https://calc.3dservisas.eu/?TY7LCsIwEEX_JWuRPJr42KbSVSUg2L12UcHaQJfiv3fujVR3Z07u3Mlb3eKgjur5mF5qI8NZBrfdCc_xImw1MQkaR4xIaF18HX-ZGqGqMEuNYEYJFvPfXk6wFQlLFsQq54mQgbgW3Qe8G008Ce4LXrHPq2P8lo5o91RpgrNEBIPXJQofhPpuhme6b1p8gbrpVsSxQ1CfBQ==
See for yourself!.
```

---
## \#125 Posted by: Battosaii Posted at: 2019-01-21T17:40:00.160Z Reads: 608

```
Also depends on weight I can full throttle my board that has theoretically 12kv of power and I don't get wheel spin under full throttle with 107s

I'm heavier than the average rider so I have more traction.
```

---
## \#126 Posted by: janpom Posted at: 2019-01-21T20:16:51.031Z Reads: 624

```
[quote="barajabali, post:120, topic:81410"]
New Winner if this works out
[/quote]

There's also:

https://www.electric-skateboard.builders/t/atom-camper-emtb-mbs-dual-focbox-10s12p/65314/65?u=janpom
```

---
## \#127 Posted by: Stielz Posted at: 2019-01-22T03:41:05.953Z Reads: 595

```
Awesome project man, you clearly know what you're doing. I'll be hanging out for updates on this!
```

---
## \#128 Posted by: briman05 Posted at: 2019-01-22T04:56:53.040Z Reads: 589

```
I’m super excited to see this board all finished if this thing works and gets to 100 mph it will be the build of the year. I have only gone that fast in a car a handful of times..
```

---
## \#129 Posted by: lrdesigns Posted at: 2019-01-22T05:17:55.833Z Reads: 579

```
@FullMetal_Machinist Will you use an unsymmetrical truck angle setup? I think its the only way to get really good stability at really high speed. 

Or even adjustable steering angle for tunning?
```

---
## \#130 Posted by: Sebike Posted at: 2019-01-22T05:56:28.802Z Reads: 576

```
Going on a rail is the only way of getting good stability at that speed
```

---
## \#131 Posted by: banjaxxed Posted at: 2019-01-22T07:37:41.032Z Reads: 565

```
Who knows if you can keep it locked down on a rail at that kind of speed, 160kph is out there by itself untested
```

---
## \#132 Posted by: Andy87 Posted at: 2019-01-22T07:43:24.898Z Reads: 559

```
@FullMetal_Machinist just to get that clear, you try to push your board to 100km/h or 100mph? Because the title says mph but in your comments you speak about km/h.
```

---
## \#133 Posted by: Sebike Posted at: 2019-01-22T08:22:01.961Z Reads: 578

```
Maglev esk8
```

---
## \#134 Posted by: FullMetal_Machinist Posted at: 2019-01-22T09:18:33.755Z Reads: 601

```
Read carefully. 100 Kph is what i am almost (99%) certain can be done immediately, 100 MPH is the designed limit of drive system - motor, esc and battery. Whether i can actually get to 100 mph depends on speed wobble and how i manage to deal with it. I have no idea how this setup will behave and i wont until i test it. We will all know in a few months, half year tops. There are a lot of components that have yet to be machined and some that have to be designed. I will work throug this gradually, testing everything in the process, maybe redesigning some (especially within traction control section and hydraulic dampers, which are just a product of my mind for now).
```

---
## \#135 Posted by: hazza Posted at: 2019-01-22T11:23:45.934Z Reads: 578

```
if I'm correct you are using go cart slicks for wheels?
```

---
## \#136 Posted by: banjaxxed Posted at: 2019-01-22T11:52:41.495Z Reads: 592

```
yes, you read correctly
```

---
## \#137 Posted by: mikenyc Posted at: 2019-01-22T12:07:05.515Z Reads: 588

```
Is this still a skateboard?
```

---
## \#138 Posted by: pat.speed Posted at: 2019-01-22T12:28:33.155Z Reads: 599

```
Does it have a deck with skate trucks mounted ...
```

---
## \#139 Posted by: rich Posted at: 2019-01-22T12:36:33.662Z Reads: 623

```
I would rather call this build "death wish" instead of "the overkill" :stuck_out_tongue_winking_eye:.
Good luck!
```

---
## \#140 Posted by: hazza Posted at: 2019-01-22T12:56:20.922Z Reads: 615

```
we need more pictures!
```

---
## \#141 Posted by: Nemesis Posted at: 2019-01-23T04:37:31.071Z Reads: 622

```
This is madness but i like madness, i hope you obtain your goals, if you do get in the Guiness book of records that would be probably worth more than 9 grand in advertising for your company could be money well spent me thinks...  
Good luck and godspeed.
```

---
## \#142 Posted by: FullMetal_Machinist Posted at: 2019-01-23T08:27:44.369Z Reads: 589

```
@rich
I certainly do not wish to kill myself, only to have more fun than legally allowed.
Considered "Widowmaker" but i'm not married yet!
Then one of my friends came and after some questions said:
"Dude, this thing could go into Encyclopedia Britannica as very definition of the word "OVERKILL". So it sticked.
@hazza
Pictures due in few days, when progress is done and photographed. 
VESC 10 PCB manufactured and in route from china, also today some machining will be done due to free time.
```

---
## \#143 Posted by: Sebike Posted at: 2019-01-23T09:01:23.963Z Reads: 567

```
There's a thin line between achieving something awesome and standing in line for a Darwin award. 

That thin line is called speed wobble on a high velocity board. :fearful:
```

---
## \#144 Posted by: never4getf150forums Posted at: 2019-01-23T09:04:03.835Z Reads: 569

```
how will you account for the heat the in hub motors will get... i can only assume 20s will absolutely kill the adhesive holding the magnets in place with the heat produced..
```

---
## \#145 Posted by: FullMetal_Machinist Posted at: 2019-01-23T09:11:23.947Z Reads: 601

```
It is not he voltage that heats the motors but the current. And you go high voltage to decrease the current. Another beast is that at 12S i would have to wind 1/2 turn of wire per pole, which is hard to do!
```

---
## \#146 Posted by: FullMetal_Machinist Posted at: 2019-01-23T09:14:22.008Z Reads: 643

```
Wanted some photos here you go.
Rendered design for deck mould, top and bottom. 30cm wide, 110 cm long, 3,5 cm curve.![d%C3%B3%C5%82%20formy|690x454](upload://fObU3vOnsi8aZ60gwsom0xRY4uY.jpeg) ![g%C3%B3ra%20formy|690x454](upload://zNwO23RJKSKA8ok2LO1s3spW0yx.jpeg)
```

---
## \#147 Posted by: lrdesigns Posted at: 2019-01-23T09:14:43.093Z Reads: 624

```
@FullMetal_Machinist maybe I am pointing out the obvious, if so my apologies. 

I just want to make sure that your truck angles front to rear are not symmetrical. This is what creates speed wobbles.  And if you build the deck from scratch you can put in adjustable angles. 

Standard longboard trucks with be like 50 deg front and rear. But for down hill racing people run the rear at a much lower angle. Like 50 front 30 rear. This eliminates the oscillation that causes speed wobble. 

But for crazy fast maybe you can run lower angles like 35 front 15 rear for more stability.
```

---
## \#148 Posted by: FullMetal_Machinist Posted at: 2019-01-23T09:17:17.611Z Reads: 604

```
As i mentioned some posts ago initial setup is 30/30 degrees, if it needs adjusting then angled spacers will be cut using bandsaw and put between truck and deck. All depends on how the board will behave.
```

---
## \#149 Posted by: lrdesigns Posted at: 2019-01-23T09:20:56.446Z Reads: 626

```
ok cool, low angle is good. :grinning: But symmetrical angles front and rear will still be a problem, (it will just happen at a higher speed) its what induces uncontrollable oscillation.
```

---
## \#150 Posted by: FullMetal_Machinist Posted at: 2019-01-23T20:48:19.780Z Reads: 667

```
Today was the metal shavings day. Two more hubs got machined, one to go.![01|666x500](upload://7RrQEXT0X72vnC9LgcFIocTGLaG.jpeg) ![28|666x500](upload://6O3FRwlmHdIMTzzujpDoYhuXA3z.jpeg) 
As you can see hub consists of two parts - inner aluminium part and steel flux ring.
They are connected by a M90x1,5 thread which is machined directly on a lathe - no tap required. Tap of this size would have cost over a 1000$ and is impossible to use bencause of enormous torque required, so i did away with regular pointed blade. Parts will be glued together with special industrial adhesive and final 0,5mm of steel removed afer centering the hub. This is the job for tomorrow.
Test winding of 3 turns per pole was made using colored wires - each color is different 
phase.
![30%5B01%5D|666x500](upload://Tw0aWd3u0COR21AM877DYG1rqu.jpeg) 
 Magnets were glued inside first hub
![31%5B01%5D|666x500](upload://m5rNlTlgpbFzhcYmxcemDJsRrn3.jpeg) 
and then motor can be test assembled
![30|666x500](upload://11TDTt8K4e6TaZAjvp5yn4cNmYr.jpeg) 
Using drill press method exact motor KV will be determined and final winding will commence in a few days.
Did i mention metal shavings? Like a barrel of them?
![02%5B01%5D|666x500](upload://aq6cKOq6mJomtHxsLOJSpO2oPBa.jpeg)
```

---
## \#151 Posted by: Der6FingerJo Posted at: 2019-01-23T20:57:55.106Z Reads: 634

```
Awesome stuff man! I've always had an eye on those big tiger motors but I never expected them to show up in an esk8 build!
```

---
## \#152 Posted by: Hummie Posted at: 2019-01-23T21:10:09.410Z Reads: 635

```
Thinking of obstacles to your goal maybe you’d need two sets of tires, one super low duro for acceleration and one hard pair that could stay on the motors and not be thrown off from centrifugal force.
Higher voltage won’t make motors run cooler. Someone was saying otherwise.

That’s a huge amount of poles in the rotor. Will u be able to stay under the esc erpm limit at such high speeds?
```

---
## \#153 Posted by: FullMetal_Machinist Posted at: 2019-01-23T21:31:36.175Z Reads: 631

```
Use the link to filled calculator data i posted yesterday.
erpm at top speed will be just 88.000, about half of original vesc limit, no idea how higher my improved design will go. No problem here. Higher voltage will make motors cooler only when motors with lower KV are used, here running lower voltage was not an option for 2 reasons:
1) at 20S i will run 500-600 battery amps, if i switched to 12S i would have to run over 1000amps, thicker wires etc. Max motor amps combined 1400 amps, with 12S would be over 2500 amps, wires as thick as a middle finger.
2) At 20S i estimated 50 KV needed, which should be 1 turn per pole. Will know exactly on monday. At 12S i would need 85KV, and i cannot wind motor pole with 0,6 turns of wire.
```

---
## \#154 Posted by: Kug3lis Posted at: 2019-01-23T21:33:45.026Z Reads: 583

```
Are you going to use liquid nitrogen for cooling motors?
```

---
## \#155 Posted by: FullMetal_Machinist Posted at: 2019-01-23T21:45:23.304Z Reads: 586

```
All components of this build are so oversized and overpowered this is no longer a joke, just pure overkill. Textbook overkill.
For "normal" riding everything will operate at under 10% rated capacity and no heat buildup is possible, i consider lukewarm is worst that can happen after long ride in woods at 50 KPH.
For "racing" even 1/4 mile would take like 10 seconds. Can you burn a motor in 10 seconds from heat buildup? i dont think so.
```

---
## \#156 Posted by: Kug3lis Posted at: 2019-01-23T21:50:10.959Z Reads: 605

```
Well, like I mentioned in my first post on this topic this build denies physics :D My 80100 with not even reaching 20km/h heats up so badly with open ends full cooling, aluminium heat exchanging from gear drive and etc :slight_smile:

Your motor is under metal jacket, and aluminium hub with big ass rubber over it without any ventilation. You will be able to fry steaks on it. (P.S. you know that magnets start losing magnetism at around 80ºC)

Also learn about duty cycle your motors will consume your max current at speed zero as the weight and large pole number will make it super hard to spin it now make it 4 of them.

Another thing you know that >60V DC is lethal and you know spark gap requirements for currents over 200A on higher than 60V?

**EDIT:**

> Magnets with the N52 magnetisation have a maximum working temperature of 65°C.
```

---
## \#157 Posted by: sk8l8r Posted at: 2019-01-23T21:59:17.713Z Reads: 573

```
[quote="Kug3lis, post:154, topic:81410"]
liquid nitrogen for cooling motors
[/quote]

.... I love this place, that post just made me smile so much :smile: 

I considered that for hardcore vesc cooling, but just cannot imagine using it outside a bench test
```

---
## \#158 Posted by: Lambjr088 Posted at: 2019-01-23T22:03:46.273Z Reads: 578

```
I thought thats what esk8n is. Denying physics?!
```

---
## \#159 Posted by: FullMetal_Machinist Posted at: 2019-01-23T22:05:56.119Z Reads: 633

```
Motor will be wound with 12mm2 of copper per phase which is thicker than 8awg. It is designed for 350 amps. Casual riding at 20 amps is nothing, Entire motor loss will be like 10 watts. Imagine you drive your board at 5 amps - will it be hot?
A lot depends on steel core quality - it gets no better than tiger motor.
As for 60 volts you do not even make me laugh.
I am certified elctrican for 10 years, got shocked more times than can remember. Once discharged big ass capacitor at 3000 volts through my hand, was missing entire tip of the thumb. Took 6 month to heal. Not my mistake. Another time through-air discharge from high frequency coil caught me from 1,5 meters afar. Took almost a year for the hair to grow back. I still live and have all limbs in proper working order.
Now i own electronic assembly company and make my own vesc.
You are teaching a father how to make a child.
```

---
## \#160 Posted by: Kug3lis Posted at: 2019-01-23T22:07:02.703Z Reads: 616

```
Well professor mechanist you know better :) Good luck
```

---
## \#161 Posted by: Lambjr088 Posted at: 2019-01-23T22:10:07.057Z Reads: 636

```
![popcorn_yes|301x250](upload://93DfkX0uNLhFkfGgqZ5WtpACI3o.gif)
```

---
## \#162 Posted by: Lambjr088 Posted at: 2019-01-23T22:11:25.128Z Reads: 630

```
https://m.imgur.com/gallery/H3cSAwQ
```

---
## \#163 Posted by: Kug3lis Posted at: 2019-01-23T22:19:36.147Z Reads: 626

```
https://media.giphy.com/media/U0T7lv73Zu3C0/giphy.gif
```

---
## \#164 Posted by: Lambjr088 Posted at: 2019-01-23T22:24:34.119Z Reads: 635

```
![giphy|360x360](upload://zMYWPftrDRAyySg0ORAzsUgmasj.gif)
```

---
## \#165 Posted by: dareno Posted at: 2019-01-23T22:43:59.776Z Reads: 624

```
[quote="FullMetal_Machinist, post:100, topic:81410"]
You got there utilising conventional, orthodox methods improved steadily over decades. It is based on existing, high quality components. It is the safest approach and will yield good results over time, no discussion about it.
My approach is throwing everything we know out of the window and starting form scratch with little knowledge about downhill speed skating and no experience
[/quote]

Have you actually seen one of @MoeStooge race boards?  Absolutely nothing conventional about them at all.  That aside good luck
```

---
## \#166 Posted by: Pedrodemio Posted at: 2019-01-23T22:48:47.366Z Reads: 616

```
Max operating temperature is also a function of geometry, not only grade

@FullMetal_Machinist what are the dimensions of the magnets?

But I agree that this will probabaly never overheat, unless you do sustained pulls back to back to top speed

But normal riding, only if you pull a car everywhere you go

It has so much peak power that it never will operate at that peak for more than a few seconds
```

---
## \#167 Posted by: Arzamenable Posted at: 2019-01-23T23:00:33.874Z Reads: 585

```
Please do continue to post updates regardless of well intentioned critiques. This build is ridiculous 👍
```

---
## \#168 Posted by: Jacobee Posted at: 2019-01-24T00:48:33.623Z Reads: 574

```
I know the ultimate goal of this build is to see how fast you can go on an eboard, so do you think once it's done you'll try and race with it at some of the races that are popping up? Cuz this thing would be crazy fast in an uphill race like Barrett.
```

---
## \#169 Posted by: Lambjr088 Posted at: 2019-01-24T02:18:53.450Z Reads: 567

```
I kid u not. This build looks sick it is something I could of only dream up now u r making it a reality cant wait to see the finished product
```

---
## \#170 Posted by: J_Dizzle Posted at: 2019-01-24T02:37:21.346Z Reads: 593

```
Did you take any inspiration from this thread?
https://www.electric-skateboard.builders/t/dream-builds-what-cool-sh-t-do-you-wanna-build/78208?u=j_dizzle
Cause that’s what this board is man, a dream
```

---
## \#171 Posted by: Deckoz Posted at: 2019-01-24T04:07:19.392Z Reads: 563

```
lol the insanity has surpassed me. And yall thought I was crazy with 13s going ~44mph..

This would be better as a luge. 100mph... lol
```

---
## \#172 Posted by: barajabali Posted at: 2019-01-24T05:24:08.309Z Reads: 565

```
Can you even stand on a board going 100mph due to wind resistance? 

Need to practice standing in a wind tunnel lol
```

---
## \#173 Posted by: Indiangummy Posted at: 2019-01-24T05:49:58.262Z Reads: 571

```
LMAO he might actually need a wing for downforce. 😂😂
```

---
## \#174 Posted by: Sebike Posted at: 2019-01-24T05:58:25.600Z Reads: 583

```
[quote="ZackoryCramer, post:9, topic:44745"]
safer sitting. Just my preference.
[/quote]

Where's buttboarding-boy when you need him??
```

---
## \#175 Posted by: FullMetal_Machinist Posted at: 2019-01-24T11:36:37.753Z Reads: 614

```
@Pedrodemio
Worst thing that can happen is that magnets overheat and loose some power. It will cost 350$  (4*42pcs*2.06$/piece) and a day of work. By the time this happens N52SH will be available.
For now i will trust in vesc built-in thermal protection of the motor (NTC sensor planned) and set it to like 80* for the stator which will keep outer rotor under 60*. When i get too cocky with throttle ESC will cut it down for me.
Magnet size is 5mm thick 6mm wide 40mm long. Original motors use 2,4x5x15mm N38SH.
@J_Dizzle
Initial design was complete long before i found this forum.
Started with the stickiest tires i could fit and worked my way up from there to completely use this grip at maximum efficiency and somehow keeping wieght down when possible.
@Jacobee
I live in Europe, so if there are races nearby i would like to participate. Hauling this bad boy overseas to USA is not an option time- and cost- wise.  I looked at https://www.electric-skateboard.builders/t/1-8-mile-up-hill-race/72437 and strongly regretted i could not participate.
@barajabali
I have no idea how much wind force i will experience on a eboard and if simple leaning forward will be enough. Experience to be earned. For now driven at 120mph on a motorcycle and it was a blast. Also done 93 kph on ilnine skates down the Belwederska street in Warsaw and didnt crash - bet a friend i could go over 70. You should see his face.
I think i will slowly increase my speed until something prevents me from doing so, then try to find better solution and ride again.
@Sebike
I believe he is already working on a custom pair of slide pants for his butt, capable of 100MPH.
```

---
## \#176 Posted by: janpom Posted at: 2019-01-24T12:07:59.437Z Reads: 597

```
[quote="FullMetal_Machinist, post:159, topic:81410"]
got shocked more times than can remember
[/quote]

[quote="FullMetal_Machinist, post:159, topic:81410"]
Once discharged big ass capacitor at 3000 volts through my hand, was missing entire tip of the thumb.
[/quote]

[quote="FullMetal_Machinist, post:159, topic:81410"]
Another time through-air discharge from high frequency coil caught me from 1,5 meters afar
[/quote]

[quote="FullMetal_Machinist, post:175, topic:81410"]
driven at 120mph on a motorcycle
[/quote]

[quote="FullMetal_Machinist, post:175, topic:81410"]
done 93 kph on ilnine skates
[/quote]

And yet he's still alive. :smiley:
```

---
## \#177 Posted by: FullMetal_Machinist Posted at: 2019-01-24T12:10:03.865Z Reads: 554

```
And all limbs in a proper working order !
```

---
## \#178 Posted by: will_manners Posted at: 2019-01-24T12:13:21.439Z Reads: 553

```
@FullMetal_Machinist You're out of your damn mind! Love it. Fucking mental 👍
```

---
## \#179 Posted by: sk8l8r Posted at: 2019-01-24T12:38:07.365Z Reads: 595

```
[quote="FullMetal_Machinist, post:175, topic:81410"]
I live in Europe
[/quote]

If your complete by July please take this beast to the Paris meet!  :slight_smile: 

Btw are you going to sell anything when your happy with it?
```

---
## \#180 Posted by: FullMetal_Machinist Posted at: 2019-01-24T13:15:26.922Z Reads: 608

```
ESC will be for sale once fully tested, in 24S and 20S version. I have ordered some extra PCB.
Once i am certain that it works at rated current without blowing i will start another thread with it.
It will be superior to that of Alien power with full vesc compatibility and a lot smaller and lighter.
Motors are too much hassle to manufacture for sale, it would have to cost exorbitant sum of money to compell me to make it for someone else.
Battery and deck everyone makes for himself., nothing new here.
```

---
## \#181 Posted by: hazza Posted at: 2019-01-24T13:19:38.630Z Reads: 585

```
how much is it costing you to develop this vesc?
what drv is it using?
```

---
## \#182 Posted by: sk8l8r Posted at: 2019-01-24T13:36:36.569Z Reads: 549

```
Excellent :smile:
```

---
## \#183 Posted by: FullMetal_Machinist Posted at: 2019-01-24T13:54:56.992Z Reads: 598

```
Just checked component list and it figures at $450-480 for components alone. So ready-made would be like $600, as it takes full day to assemble and test it.
It does not use any chip from DRV family, as those are too weak and slow. Separate drivers for each group of mosfets are used instead.
```

---
## \#184 Posted by: banjaxxed Posted at: 2019-01-24T13:55:12.700Z Reads: 626

```
[quote="barajabali, post:172, topic:81410"]
Can you even stand on a board going 100mph due to wind resistance
[/quote]

I'd say so
https://www.youtube.com/watch?v=CgBRs07fY4A
```

---
## \#185 Posted by: hazza Posted at: 2019-01-24T13:57:30.927Z Reads: 610

```
600 for one or both?
```

---
## \#186 Posted by: banjaxxed Posted at: 2019-01-24T14:00:12.791Z Reads: 612

```
[quote="FullMetal_Machinist, post:159, topic:81410"]
You are teaching a father how to make a child
[/quote]

That's going in the back pocket :joy:
```

---
## \#187 Posted by: FullMetal_Machinist Posted at: 2019-01-24T14:05:27.536Z Reads: 605

```
Unfortunately for one.
If it was for a full set then my budget wouldnt be 9k but far less, now it figures:
4k for motors (trucks, donor motors, magnets, metal billets for machining)
2k for esc
1,5k for battery
500 for minor stuff like wiring, screws, some other electronics
about 1000 yet to be spent on other stuff, eg. deck and covers.

@banjaxxed it is quite common idiom in Poland literally "Nie ucz ojca dzieci robić".
It means that you try to explain basics to someone well versed in the topic.
```

---
## \#188 Posted by: hazza Posted at: 2019-01-24T14:07:18.501Z Reads: 564

```
what battery are you using? 18650s or lipo?
```

---
## \#189 Posted by: FullMetal_Machinist Posted at: 2019-01-24T14:07:50.319Z Reads: 553

```
Read from the top.
```

---
## \#190 Posted by: hazza Posted at: 2019-01-24T14:10:56.696Z Reads: 548

```
ah ok. that's one huge battery.
```

---
## \#191 Posted by: Toughook Posted at: 2019-01-24T14:27:56.324Z Reads: 584

```
[quote="Kug3lis, post:119, topic:81410"]
I love how this build ignores physics :smiley:
[/quote]


where he's going, he don't need physics........... :grin:
```

---
## \#192 Posted by: Pedrodemio Posted at: 2019-01-24T14:51:40.902Z Reads: 639

```
Do you mind sharing where you got your magnets? I will need some for my own DD soon

And for N52 and your geometry I wouldn't let the magnets get hotter than  55°C or you will enter permanent demagnetization temperature

![image|665x500](upload://4r7ej17phsySDBUTxYkZ3OC0ZWS.jpeg) 

But if you change them to N48H you would loose maybe 10% of max torque but could take them to 115°C

![image|664x500](upload://4t5TAUze9X9EQe3ZKvUtFtCkJpC.jpeg) 

The main challenge is measuring how the rotor and magnets temperature relate to each other
```

---
## \#193 Posted by: FullMetal_Machinist Posted at: 2019-01-24T15:15:20.310Z Reads: 596

```
The company i bought the magnets almost 2 years ago is 
http://www.aimmagnet.com/
Checked emails and they assured me that with this shape (5x6x40mm bar) and application (closed magnetic loop) i can take them up to 70C without permanent loss of magnetic force.
Permeance coefficient is 0,8 for a single magnet but 1,2 for array of alternating poles, therefore 70C is possible.
Today some companies already make N52H which is good to 120C. 
If it goes then replacing magnets is easy enough. Those are what i have and will use for now.
```

---
## \#194 Posted by: Pedrodemio Posted at: 2019-01-24T15:43:59.147Z Reads: 548

```
Thanks, will add them to my list

I trust more in them than in me
```

---
## \#195 Posted by: Vanarian Posted at: 2019-01-24T16:30:07.565Z Reads: 572

```
[quote="FullMetal_Machinist, post:175, topic:81410"]
I live in Europe, so if there are races nearby i would like to participate. 

**Also done 93 kph on ilnine skates** down the Belwederska street in Warsaw and didnt crash - bet a friend i could go over 70. You should see his face.
[/quote]

I feel like I'd really appreciate meeting you man. Where are you based in EU? What's the name of your company?
```

---
## \#196 Posted by: Spiritrunner47 Posted at: 2019-01-24T16:30:31.929Z Reads: 576

```
(Sits back takes a deep breath) Broooooo!!!

Legit. That is all. Oh, theoretical now. Big facts later.
```

---
## \#197 Posted by: banjaxxed Posted at: 2019-01-24T17:23:13.584Z Reads: 594

```
This board needs self replacing underwear if it’s overkill
```

---
## \#198 Posted by: Sn4pz Posted at: 2019-01-24T19:25:19.514Z Reads: 623

```
![giphy%20(1)|250x224](upload://tku4nQMPJ4Kx86QNO6T5Dee3Hko.gif)
```

---
## \#199 Posted by: ricardo Posted at: 2019-01-24T22:53:31.428Z Reads: 615

```
Will this be ready for the Paris event in July? Would love to see this in action
```

---
## \#200 Posted by: Steve-81 Posted at: 2019-01-25T08:24:46.446Z Reads: 614

```
I really like this build. I hope you get on with it how you want to. I love it when people are coming up whit stuf like: you can't make it, it's impossible…


We all know (or let me say most of us know) that all big changes are always comming from people out of the field, because they can think different :slight_smile:

Get on with it mate, I want to see the end rásült :)
```

---
## \#201 Posted by: Chrisjarram Posted at: 2019-01-25T08:29:25.327Z Reads: 594

```
 This really isn't going to end well...
```

---
## \#202 Posted by: Steve-81 Posted at: 2019-01-25T08:39:48.929Z Reads: 581

```
This build is brilliant. @FullMetal_Machinist is really trying his best, to come up with good solutions. If you guys read bak, you will see, that he never ever said, he will go full trottle on it… but he said, he will climb up the ladder…


Come on guys, just think on this project on the way: What is possible, what isn't? If you don't try new ideas, you will never know where an esk8 can be in some years from now. I guess when someone built the very first esk8 everybody around were laughing, that it won't work…


I myself really like it, that there are some people, who can think out of the box. I even do understand people have their concerns, but come on guys, be positive, or just let @FullMetal_Machinist do his project... It's his own money he is willing to spend on something he believes can work. Thumbs up man :)
```

---
## \#203 Posted by: FullMetal_Machinist Posted at: 2019-01-25T09:25:40.631Z Reads: 569

```
Finally someone who knows what i feel. 
Truthfully i would love to go to a drag strip with my board and outrun 600cc stock bike but it is not something that can be done immediately. A lot of trials, tweeking and fixing stuff that was not good enough is on the way. And it needs to be done, just like any other good build out there.Peole like Kug3lis https://www.electric-skateboard.builders/t/monster-board-trampa-holypro-35-80100-180kv-8kw-fatboy-ss-gear-drive-12s-3p-18ah-dual-focbox/36560
or Pedrodemio also understand as they had to go this road as well. Those are the people that make all the interesting, technical comments instead of typical lols and rotfl. Also seen several attempts of designing ESC on this forum, albeit none of them succeeded for now. Hope mine goes better.
Cheers!
```

---
## \#204 Posted by: Andy87 Posted at: 2019-01-25T09:36:24.924Z Reads: 575

```
[quote="FullMetal_Machinist, post:203, topic:81410"]
designing ESC on this forum, albeit none of them succeeded for now
[/quote]

I guess you speak about escs with a higher S rating as usual, because if no than you not right with this point. The ESCapes by @stewii have been a great success and still outstanding for a vesc 6 based esc.
Please also keep in mind that there is not only this forum where people work on vesc based escs. I just dump this here for example 
https://vesc-project.com/node/339
```

---
## \#205 Posted by: sk8l8r Posted at: 2019-01-25T09:40:22.492Z Reads: 566

```
@FullMetal_Machinist I love your attitude! 

Skating has always been about pushing boundaries - your pushing so many :slight_smile:

Also I think 'ive built somethingso fast I will have to practice to stay on' is one of the BEST problems to have ever!
```

---
## \#206 Posted by: FullMetal_Machinist Posted at: 2019-01-25T12:04:16.777Z Reads: 587

```
Looked over his design and compared to mine.
Pity it already is copied by chinese. Read his thread carefully.
He used VESC6 as a base so 3 current shunts on high voltage side, i wanted to avoid that at all cost.
His board uses single drivers per group of mosfets so he gets 4a driving current over 45nf of gate capacity, I use double drivers per group and different mosfets with less capacity and faster switching so i get 12a driving over 16nf of gate capacity (numbers combined for both). This leads to my design switching almost 10x faster, lower dead times (his are 330ns, mine TBD but 20-30 ns projected). 
Another beast is that he does not have step-down on his board and it needs separate voltage supply for logic, mine features power section and is perfectly fine with only main voltage. Designs of power stage in both cases look almost identical (component placement, current paths) only difference is  component size and count. My design will have round wires 4mm thick soldered onto PCB as it is much cheaper and does not overheat entire PCB during soldering (he mentioned it takes him 5 mins of heating), as he made water-cut busbar from 3mm copper sheet for 50$. 

My design is slightly cheaper in comparison, i hope to get to 20S voltage - his is 16S, 18 max. 

His design is tested and works after sorting some shenigans, mine is waiting for first PCB to arrive.
We will see in a week or two, depends how much free time i will have.
Thanks for posting the link. Did not know someone got this far.
```

---
## \#207 Posted by: Andy87 Posted at: 2019-01-25T12:09:53.187Z Reads: 573

```
[quote="FullMetal_Machinist, post:206, topic:81410"]
Read his thread carefully.
[/quote]

I was referring to your last post only.
And in this post you was not clear enough formulated.
It’s just not right to say that all this forum totally sucked in designing vescs. That’s definitely not right.

Read my answer please carefully!
I ask you just to specify your statement.
Your idea to create a esc like you doing is outstanding and can’t be compaired with something, somebody tried here before, so you also can’t say we failed in the attempt in doing it!
```

---
## \#208 Posted by: FullMetal_Machinist Posted at: 2019-01-25T12:20:21.363Z Reads: 548

```
Sorry for misspelling.
Not succeding and failing are different and i wouldnt consider changing 1 chip designing, only minor tweak. Will try my best not to badmouth anyone, but english is not my first language.
```

---
## \#209 Posted by: Andy87 Posted at: 2019-01-25T12:31:34.363Z Reads: 544

```
All good 😉 waiting 2019 to be the year of 18-20s escs 🙏 and maybe some Esk8 Guiness Records...
```

---
## \#210 Posted by: marioflatini Posted at: 2019-01-25T14:40:13.237Z Reads: 532

```
Start on a steep downhill :joy:
```

---
## \#211 Posted by: Hummie Posted at: 2019-01-25T19:19:45.791Z Reads: 523

```
Did u do magnetic modeling to decide on those huge 5mm thick magnets?
```

---
## \#212 Posted by: Dornacht Posted at: 2019-01-26T03:23:20.522Z Reads: 524

```
@FullMetal_Machinist, build looks awesome, mad but awesome 

How are you going to passively cool the motors without airflow and with a current draw that large?
```

---
## \#213 Posted by: ZachTetra Posted at: 2019-01-26T03:42:38.334Z Reads: 541

```
@FullMetal_Machinist Have you considered high temperature super conductors for the stater core?  If you add a pressure vent at the ends of the rotor housings and pot the magnets with epoxy (anything to make them smooth all the way around) you can flood the motor with liquid nitrogen and drop the resistance of the motors and pull far more power into them, as long as the magnets don't crack the torque you get is based only on the internal resistance of the battery and the magnets wouldn't demagnetize under load. Also the wheels would 'smoke' as you go faster and that is amazing

You could also use liquid helium since copper should super conduct at 4K but its kinda expensive
```

---
## \#214 Posted by: FullMetal_Machinist Posted at: 2019-01-26T08:21:36.608Z Reads: 551

```
Idea is that motors are so oversized that during normal riding at 50 kph they will be under 10% nominal current and heat will be so small that passive cooling is enough and during high power runs actual working time is 10 seconds and it is not enough time to overheat the motor even at max power, as motor thermal capacity is not small. If the motors start to overheat after all i will be forced to switch the magnets to higher temperature grade, which was yet unavailable when i first bought them. However this is not expensive or time-consuming considering rest of the build at 350$ and 1 day of work.
Tires will smoke with actual design, as design was made to use full grip of the tires (supersofts on tarmac).
If treaded dirt tires are used it will be impossible to apply over 50% of throttle without smoking them, on gravel or grass grip limit is under 25% of the throttle setting.
```

---
## \#215 Posted by: Dornacht Posted at: 2019-01-26T14:49:51.591Z Reads: 523

```
Okay makes a little more sense if your not going to use it on 70 mile treks
```

---
## \#216 Posted by: StickyBlue Posted at: 2019-01-27T01:39:51.396Z Reads: 526

```
Any idea what your quarter mile time will be?
```

---
## \#217 Posted by: Friskies Posted at: 2019-01-27T02:19:27.097Z Reads: 529

```
0.02 seconds or DNF cause he almost died doing mach 5 on an Esk8.
```

---
## \#218 Posted by: mozza Posted at: 2019-01-27T09:04:09.912Z Reads: 524

```
first post< title says it all THE OVER KILL
boldly go where no man has gone before 
theirs  *Klingon*s on the starboard bow
```

---
## \#219 Posted by: Stielz Posted at: 2019-01-27T20:16:14.268Z Reads: 576

```
[quote="FullMetal_Machinist, post:206, topic:81410"]
He used VESC6 as a base so 3 current shunts on high voltage side, i wanted to avoid that at all cost.
His board uses single drivers per group of mosfets so he gets 4a driving current over 45nf of gate capacity, I use double drivers per group and different mosfets with less capacity and faster switching so i get 12a driving over 16nf of gate capacity (numbers combined for both). This leads to my design switching almost 10x faster, lower dead times (his are 330ns, mine TBD but 20-30 ns projected).
[/quote]

Switching those MOSFETs hard. 

Great for minimising power loss across the FETs but man, that's going to create some nasty voltage spike when switching those high currents. 
Are you using 100V rated FETs?
I may suggest that your controllers will need some very low ESR capacitors across the DC bus to soak up those voltage spikes, and very close proximity to the FETs. 
I believe such voltage spikes are probably the reason that other fellow's controllers can only run 18s max even though they are 100V MOSFETs. 
You've probably already considered all this, but just in case, thought I'd mention something.
May I ask why wanted to avoid the 3 shut design?
```

---
## \#220 Posted by: FullMetal_Machinist Posted at: 2019-01-27T21:44:23.947Z Reads: 601

```
I would love to have 3 shunts, but not on high voltage side. This is what causes 50% of spike problems. Someone https://www.electric-skateboard.builders/t/sesc-a-vesc-6-derivative/58106 has done this by modifying VESC6 firmware to use shunts on ground side.
I cannot modify firmware (not my field of work), so i was limited to using 4.12 as a base.
For technical side it would add roughly 20 components to the design, no big deal for me.
Other spike generating issue is power routing by itself.
As described here https://vesc-project.com/node/655 there is problem with ringing at radio frequencies, common to all high-current ESC, however some people do not get to the point of identifying it and vieving spikes on oscilloscope, as most digital oscilloscopes do not "see" frequencies this high - it is over their bandwidth. It is caused by high current path creating a circular "loop" on the PCB itself. It can only be remedied by redesigning with different current paths, ground planes, multiple current layers etc.
Problem is more pronounced with high-speed switching as in my design.
Spikes can be as high as 50% of voltage supply. Decoupling capacitors (my design has over 30) and their proper placement help somehow but do not get rid of the problem source itself, which is the physical size of mosfets. Low-ESR electrolytic or polymer capacitors are too far (physically) to even count. Getting them closer makes the loop get actually bigger. This is the reason for me to use smaller powerSO-8 package instead of D2Pak-7.  Another thing that can be done is isolating external inductance (means motor) by means of RC filters and high-speed diodes, capable of "catching" those frequencies.
Mosfet internal diodes are too slow by an order of magnitude to do the job.
My design can accomodate 100V or 120V fets. I start with 100v ones, as they have lower internal resistance. First tests will be done at lower voltage, so i have room for spikes, then when filters are working i will up voltage to 20s, as supply voltage has no effect on the presence of ringing, only on spike magnitude. What is important is to run tests at high current and with low external inductance (motor with few turns on the stator), as low inductance promotes spikes. I encountered this problem multiple times with other designs and was able to subdue it somehow. In worst case i myself blew 2000 Amp 1200volt IGBT at 460 volt power supply. Ringing was cauced by long motor leads (industrial application, very big DC motor). Testing in-house had no effect bencause problem was at the installation site.  Decoupling had to be applied exactly in the middle of motor leads(sic!).
Other time friend from Warsaw University of Technology called me bencause 100KW 30khz transformer i made for them was getting too hot. When i looked at oscilloscope the top horizontal line of square waveform was of 400volt thickness. They didnt even realize it was continous line of 2Mhz spikes. Ended up swearing fucks to a real colonel who was supervising the project. Then i sent them a bill for on-site consulting.
So in the end i hope that my previous experience will help me somehow to make this a reality.




I
```

---
## \#221 Posted by: Stielz Posted at: 2019-01-27T22:49:59.951Z Reads: 535

```
Excellent,I hope your testing goes well and look forward to hearing about your results when your PCBs arrive shortly :sunglasses:
```

---
## \#222 Posted by: linsus Posted at: 2019-01-27T23:49:12.144Z Reads: 498

```
I've read alot about SiC-FETs throughout the year, how they're s'posed to be superior in HV designs but never seen anyone incorporate them so far. Any thoughts on this?
```

---
## \#223 Posted by: NullReference Posted at: 2019-01-27T23:56:08.420Z Reads: 534

```
I think my favorite part of this build is the sheer insanity of it. If OP’s calculations are correct, this board has a good chance of being limited in its acceleration by traction.

Four go-kart racing slicks won’t provide enough traction. I’m trying to wrap my mind around how utterly ridiculous that is.

My current board has clocked in at 28mph with only one driven wheel. It feels like a rocket ship when I floor it. And my board isn’t really limited by one wheel drive.

This is going to be awe inspiring to watch.
```

---
## \#224 Posted by: FullMetal_Machinist Posted at: 2019-01-28T00:22:31.056Z Reads: 558

```
I have several SiC mosfets, those are either 900 or 1200 volts. You would want GaN,https://pl.mouser.com/ProductDetail/GaN-Systems/GS-010-120-1-P-E01-MR?qs=%252bEew9%252b0nqrB2GFgqM79EvQ%3d%3d but to get low enough resistance 10 of them in pararel is just about right. At $15 per one mosfet it is not economically viable to use them. Switching at 20ns is fast enough, no need to go at 0,1 ns. Finding fast enough drivers is difficult and ringing would go ito GHz range. Done that once in my life and once is enough. Only '80 vaccuum tube oscilloscope could see the spikes.
```

---
## \#225 Posted by: pat.speed Posted at: 2019-01-28T05:54:51.714Z Reads: 541

```
I’d just like to tag @ngv-nextboards, this is your competition I’m sure you’ve seen some of there videos
```

---
## \#226 Posted by: sk8l8r Posted at: 2019-01-28T11:21:37.171Z Reads: 590

```
[quote="pat.speed, post:225, topic:81410"]
this is your competition 
[/quote]

yet to see one on video even do 40mph.... its been years now, screenshot or it didnt happen lol
```

---
## \#227 Posted by: FullMetal_Machinist Posted at: 2019-01-28T21:39:55.481Z Reads: 610

```
PCB's have arrived today. 
![32%5B01%5D|666x500](upload://9t3r312Qn5CiO9tI0631w7HdDeO.jpeg) 
![32%5B03%5D|666x500](upload://7fz9ju76crWGixvb8sYoW27jUg1.jpeg) 
Assembly will follow tomorrow, as it is over 11pm here.
At first only 1 pcb will be populated, as i am not 100% certain everything is ok. Components are pricey after all.
Filtering capacitors will also be ommited to set dead time properly, to be added with soldering iron later when initial setting is complete.
```

---
## \#228 Posted by: Blitz Posted at: 2019-01-28T21:42:51.314Z Reads: 571

```
Nice man looks soo good! 

can't wait to see how this thing turns out.
```

---
## \#229 Posted by: pat.speed Posted at: 2019-01-28T23:03:33.431Z Reads: 565

```
Quick tip, make sure lots of silicon holds he caps in place. Vibrations break the legs off if there isn’t support
```

---
## \#230 Posted by: hazza Posted at: 2019-01-29T03:38:56.824Z Reads: 550

```
this thing is going to be a monster!
```

---
## \#231 Posted by: Stielz Posted at: 2019-01-30T03:49:32.847Z Reads: 547

```
Nice progress! Looks like your routing the battery positive net to the high side FETs on internal layers? I don't know of any other high current controllers doing it this way, hope it works well for you
```

---
## \#232 Posted by: FullMetal_Machinist Posted at: 2019-01-30T10:08:03.323Z Reads: 588

```
Any high current path is routed on total of 3 layers in pararel to improve current distribution.
Bottom layer is one big ground plane, with only small areas not being ground.
Tracks are much wider than open solder areas - those were made to have room for soldering extra copper on top and botom sides respectively.
This pcb is good for about 200 amps as it is, for targeted 350-400 amps motor current additional 4mm dia copper wires will be soldered onto it.
```

---
## \#233 Posted by: FullMetal_Machinist Posted at: 2019-02-01T10:42:10.945Z Reads: 622

```
PCB is now assembled.
First was applying solder paste through dedicated stencil:
![34%5B01%5D|666x500](upload://m0T0KO3ICyBKt9Z3nGH2TiVlTEV.jpeg) 
And the pcb after lifting stencil:
![35%5B01%5D|666x500](upload://4m2WdFW9knet0cgYu8kuaJz1xcf.jpeg) 
All the components were carefully placed with needle-sharp tweezers:
![23%5B02%5D|666x500](upload://pVxMjZDppyq4bZN3hYYYHfkZ5lh.jpeg) 
And after a trip through reflow oven components are soldered in place:
![20|666x500](upload://eSstsowLQloQv43B57KGoK5Gy2W.jpeg) 
Bottom side was done with a soldering iron due to small component count:
![20%5B01%5D|666x500](upload://zbpscY6g7C6oMt3UpuwXRHSS0Tk.jpeg) 

For now PCB is partially tested.
Step-down converters that supply voltage to logic are working fine and deliver proper voltage (12,6v to gate drivers and 5,0v to anthing else) to remaining components.
Op-amp section that feeds signal from current sense resistors also works fine.
One mistake was found, as on a main step-down i put 1 ohm resistor instead of 1uf capacitor which resulted in circuit not starting. After 10 minutes it was fixed and running, nothing blew.

Today a friend of mine is coming with a programming interface and software wil be loaded into MCU.
I hope to test it somehow during weekend, however not on full power as motors are not yet complete.
For now sensitivity of current sense was increased for better debugging, resulting in a limit of -80/+200 amps. After startup is complete it will be reduced to give designed useful range of -200/+600 motor amps, as this involves only changing 2 resistors.
```

---
## \#234 Posted by: Kug3lis Posted at: 2019-02-01T12:54:24.588Z Reads: 557

```
-200/+600 amps on 12bit adc xD you will have resolution of 0.2A/step :D Also you know that you will need to change code configuration for voltage dividers and etc to get those currents correct values?
```

---
## \#235 Posted by: Pedrodemio Posted at: 2019-02-01T13:33:37.147Z Reads: 566

```
Nice progress 

What are the size of the PCB? And how you will mount them? 4 staked or 2 stacked on each side of the battery?
```

---
## \#236 Posted by: FullMetal_Machinist Posted at: 2019-02-01T14:02:14.201Z Reads: 575

```
My friend knows how to change configuration values, he already has compiled code ready.
Resolution is 3x worse than in original VESC, but there is no going around ADC resolution,
0,2A/600A is 0,03%. Fine enough. Going for higher resolution is pointless bencause of noise induced in the circuit anyway.
As for placement ESC will go under deck in front and back, between battery and truck. PCB is 100 mm wide by 92mm long. It wont use any enclosure, instead i will coat with ample amount of urethane resin for complete waterproofing,l i want to be able to swim with it.
Two ESC will be mounted side-by-side to a single heatsink 200mm wide 50mm thick 60mm long. Entire assembly will hide behind tires (looking from the side).
```

---
## \#237 Posted by: LukePL Posted at: 2019-02-01T15:44:57.267Z Reads: 545

```
@FullMetal_Machinist that is amazing and just by looking at PCB a realized that you are crazy fellow countryman  :D
```

---
## \#238 Posted by: evoheyax Posted at: 2019-02-01T21:49:55.680Z Reads: 538

```
Dude, you are like the Jesus of eskate. Holy crap! Love all of the custom work. And can't wait to see the final build.

I will be amazed if you can stay on it under a full acceleration, but if anything, sounds like a new sport. Bull riding, but on an eskate... Who can stay on? lol
```

---
## \#239 Posted by: pat.speed Posted at: 2019-02-01T22:37:48.584Z Reads: 563

```
[quote="evoheyax, post:238, topic:81410"]
Bull riding, but on an eskate
[/quote]

Water bull riding lol

[quote="FullMetal_Machinist, post:236, topic:81410"]
i want to be able to swim with it.
[/quote]

@FullMetal_Machinist what about if something fails and you need to get the the electronics? How do you get the resin off
```

---
## \#240 Posted by: FullMetal_Machinist Posted at: 2019-02-01T23:22:43.248Z Reads: 601

```
When ESC is adjusted and tested there will be no "something failed so i want to change a component". No DRV6302 present. Wiring will be soldered permanently. Everything else than mosfets is with more than sufficient margin, main step-down works fine up to 140 volts. Safety limit in place that cuts it off at 90 volts. Mosfet drivers up to 125 volts. If it goes there will be nothing to salvage, as short circuit current of my monster battery exceeds 2000 amps. Before the fuse manages to do its job there will be a hole in pcb through which you can put a finger. There are several videos of ESC burning with normal lipo battery. Nothing remains. https://www.youtube.com/watch?v=JwDwEHQCk5g Components that are not fried are "uncertain" enough not to use them again for anything important.
Only damage that can be caused to ESC is by electrolysis eating away component leads.
Under such assumption making a solid block of urethane out of it is the only logical solution.
Using plastic casing for ESC means having seriously reduced cooling, heavier overall, bigger by at least 3 cm each direction and sealing all wires going through is a pain in the ass.
As for my choice of resin here is an explanation:
Epoxy is not elastic and tends to crack and tear components out of pcb, ask Jens Kappel for "epoxy roxy". Went through this with one of my customers, who wanted to hide PCB from unwanted sihgt with colored epoxy. Everything had to be redone with urethane. Cause is thermal cycling through resin glass temperature. Polyester resin will also peel off after like 50 thermal cycles, with small chance of not pulling away components. Urethane is much better. Cost the same, doesnt smell nearly as bad. Remains elastic like forever.
I want to be able to ride my board in all conditions, snow, mud, heavy rain etc. Have fun.
I want to grab garden hose and wash dirt away when i get home from the woods, as i do with my regular mountainboard.
Motors (windings) will be coated internally with other type of resin and 100% waterproof.
Battery and other stuff can easily have sealed enclosures, especially when i make custom carbon tray for the battery and remaining electronics (limiters and traction control) is the size of a fist and doesnt have nearly as much thick wires coming in.
```

---
## \#241 Posted by: pat.speed Posted at: 2019-02-02T03:15:17.246Z Reads: 555

```
I thought you were going to epoxy the battery lol
```

---
## \#242 Posted by: Pedrodemio Posted at: 2019-02-02T03:48:32.944Z Reads: 524

```
Be careful off water creeping in via the wires, for example from the motor, burned my RC car ESC that way, took more than a year of use, the esc was completely sealed, but eventually enough water came thorough the phase wires and boom
```

---
## \#243 Posted by: taco Posted at: 2019-02-02T04:00:39.828Z Reads: 534

```
I had cells with a terminal spacer under the wrap and pressure from the side of the enclosure was still enough to break through it. This allowed the nickel tab to cause a short from the negative to positive terminal while I was riding. The board died and I saw a spark. I was scared shitless carrying it home thinking it would turn into a bomb at any second.  luckily the conductor burnt out and broke the connection immediately.
```

---
## \#244 Posted by: goldrabe Posted at: 2019-02-02T14:02:58.682Z Reads: 544

```
That's truly DIY, can't wait to see the finished board.

> Motors (windings) will be coated internally with other type of resin and 100% waterproof.

What kind of resin will you use for this?
```

---
## \#245 Posted by: FullMetal_Machinist Posted at: 2019-02-02T17:32:12.195Z Reads: 568

```
I fortunately was able to grab some 20-year-old leftover military supply that was used for impregnating alternators and starters for T-72 tank. It has no name, long number, stinks like hell for a week and is harder than 6061 aluminium when hardened in oven.
Unfortunately it eats away gloves in like 5 seconds and is pain in the ass to use, as windings need to be over 100C while impregnating. Stuff is flammable if not explosive.
I dare not use it for most of the work i do. Epoxy is enough.
However having indestructible motors is worth a hassle.
No resin or typical alkide coating can even be compared to this.
```

---
## \#246 Posted by: Pedrodemio Posted at: 2019-02-02T21:41:50.883Z Reads: 533

```
Just don’t forget to put a camera filming while you work on that, so we can see the hub motors from hell rise from the flames in case things go wrong
```

---
## \#247 Posted by: pat.speed Posted at: 2019-02-02T21:54:56.805Z Reads: 538

```
@FullMetal_Machinist you do realise that by building this enertion can no longer call there board the most “powerful direct drive skateboard”
```

---
## \#248 Posted by: FullMetal_Machinist Posted at: 2019-02-02T22:48:45.796Z Reads: 545

```
Yea..   for starters my battery alone is more expensive than their entire board
Top speed 49 kph..  i can go faster on level road on inline skates..
```

---
## \#249 Posted by: Sindre Posted at: 2019-02-03T00:59:39.007Z Reads: 532

```
Sick build man!
```

---
## \#250 Posted by: FullMetal_Machinist Posted at: 2019-02-05T19:33:42.712Z Reads: 539

```
ESC is now tested at reduced voltage, servo motor was used as i have not completed hub motors. One small mistake was found as one via did not connect to ground plane, fixed with 0,5mm drop of solder. Value of few resistors was adjusted.
It runs in sensored mode in bldc and foc without problems.
I did not have motor with high enough KV to go above 30k erpm for now.
For sensorless i can say for certain that it wont run with a very small unloaded motor, as noise in current sense is now at 0,4 A (about 5-6 ADC steps). If big enough motor is used, it should run sensorless as well, to be tested.
```

---
## \#251 Posted by: Stielz Posted at: 2019-02-06T21:18:12.854Z Reads: 521

```
Nice job getting the controller working. Sounds like you really need those hub motors finished to properly test it. Hows the progress on the motors?

Way back in your earlier posts you were talking about how this machine is going to be capable of breaking traction on all 4 wheels with go-Kart slicks for tires. I'm thinking you'd be more likely to do wheel stands instead. How low does your center of gravity need to be to not do a wheel stand?
```

---
## \#252 Posted by: FullMetal_Machinist Posted at: 2019-02-06T21:43:54.446Z Reads: 543

```
I am glueing magnets to rotor right now.
Brought home from work two spools of magnet wire 0,15 and 0,2mm diameter and will be doing winding with 450-something stranded Litz wire made from those those on friday/saturday.
Friend of mine lets me borrow very fast 4-ch digital oscilloscope for a week.
Hope to have it fully tested and adjusted in a week or two.
When i am certain voltage spikes are within reasonable values i will switch to 20S, as main battery is ready.
As for center of gravity it needs to stay below line easliest described as 60% incline starting at contact point of back wheels, what translates to 60 cm high over front wheels.
In my opinion 100% doable.
However keeping stable position at 1,6G of acceleration is something that has to be learned by experience. For now tales of the future.
Looked over https://www.electric-skateboard.builders/t/indoor-esk8-event-nl-5feb/80847 and figured that some practice on karting track would be good, luckily in Warsaw several karting tracks are present. Hopefully some of them will let me in during empty hours. It really looks like a good blast.
Back to glueing magnets.
```

---
## \#253 Posted by: Stielz Posted at: 2019-02-07T02:38:44.489Z Reads: 520

```
That will make for easy winding using such fine magnet wire. But do you think that the performance of your motors might suffer from doing it this way?
What I mean is that using 450 strands of fine wire, you pay the price of the enamel insulation thickness 450 times. Whereas if you use less strands of larger diameter wire, you have less insulation cross sectional area 'waste', leaving more cross section area for copper. 
I would have thought that optimising your motors for lower phase resistance would be more beneficial than optimising to lower skin effect?
Of course you will have considered this already, what are your thoughts?
```

---
## \#254 Posted by: FullMetal_Machinist Posted at: 2019-02-07T09:55:04.597Z Reads: 519

```
With thinner wire fill rate is much better, so net amount of copper is greater.
With thick wire it is hard to compact winding inside the triangular slot.
Also depends on which wires you use - if single insulated to 500 volts are used it is better, however if double-indulated to 1000volts were used then insulation would have consumed too much space without giving any benefit.
Especially for ESC with very fast switching times it is good to use litz wires, wew dozen watts at full power  can be saved compared to same awg but single thick wire. On idle or small load difference is so small it is hard to measure.
```

---
## \#255 Posted by: banjaxxed Posted at: 2019-02-07T12:29:50.004Z Reads: 518

```
On the material choice, silver was looked at, it’s expensive but swissboards are going to use it
https://www.electric-skateboard.builders/t/new-hummie-hubs/25251/466?u=banjaxxed
```

---
## \#256 Posted by: FullMetal_Machinist Posted at: 2019-02-07T15:03:52.763Z Reads: 524

```
Not a choice for me as i would have to use at least 8 strands of that in pararel, winding length per phase is about 4 feet, so i would need total of 96 feet per motor, which means $1800 per motor in winding wire alone. And i am not certain everything is ok at the moment so i will pass.
If everything is tested at full capacity and i happen to grab a spool of silver wire then why not?
Winding alone weighs about 10oz per motor, at silver scrap price it would be $160 per motor.

https://www.hopea.eu/drut-srebrny-ag999/druty-srebrne-ag999-okr/srednica-0-40mm-miekki-drut-okragly-ag-999.html
 I could buy silver wire here at close to market price but insulating it myself would be an issue. Proper enamel is not easy to make.
For total of 1,5 kg needed (silver weighs more than copper) i would have to pay about 1000$.
Might look into it when everythin else is done.
```

---
## \#257 Posted by: banjaxxed Posted at: 2019-02-07T15:41:41.850Z Reads: 486

```
Ouch, understandably avoidable
```

---
## \#258 Posted by: Hummie Posted at: 2019-02-07T16:37:31.249Z Reads: 517

```
Every motor rewinding I’ve ever read about has shown an improvement with thicker wire as apposed to thin mutistrand with a reduction in electrical resistance and likely better cooling ability.  
From what I read the skin effect, which litz wire is designed for, occurs at higher frequencies than we use.  https://www.rcgroups.com/forums/showthread.php?2318019-Skin-effect-within-the-windings-of-a-BLDC-motor

I’ll be surprised if they use solid silver wire in their motors.  Crazy expensive and rare.  Ive seen silver coated wire  which is touted as better because of...skin effect. But in motors that didn’t get to a frequency it would occur

I though the motor’s pwm current would be largely smoothened by the inductance anyway and there isn’t an ac frequency in the motor
```

---
## \#259 Posted by: FullMetal_Machinist Posted at: 2019-02-07T16:58:37.515Z Reads: 550

```
Today i have tested how much coppper i can fit using different wires.
Using only 0,2mm 520 wires can be fit, which is over 16mm2. With mixed 0,15 and 0,20 
360 pairs can be fit, which is 17,7 mm2. With 1,2mm wire only 12/13 can be fit reasonably, which is 13,6mm2 per slot. Nothing thicker than 1,2 is possible bencause this is the width of slot opening. Result is clear.
This is result of slot geometry and length of the stator - the longer the harder it is to fill completely, at 40mm it is hardcore.
Litz wires are easy to compact using a piece of wood or bakelite, then slot cover slides in to protect the winding from sticking out, exactly as big industrial motors are wound (done that myself).
At single enamel there is not much difference in slot fill due to only wire diameter.
Mixing two different diameters is what does the trick.
Also look here: http://eprints.whiterose.ac.uk/9077/1/Zhu_Influence.pdf?origin=publication_detail
It is proven that skin loss is greater than extra loss from longer strands in 10KW motor.
In my case, with much faster switching and faster current rise it will be even more pronounced, as they tested at 10kHz and i will run at 40kHz.
```

---
## \#260 Posted by: Pedrodemio Posted at: 2019-02-08T04:04:40.374Z Reads: 559

```
This is a point the I still didn’t understand perfectly

What switching frequency we have to take in account? In my minds is obviously that it’s not the MOSFETS switching frequency since the inductance of the motor smooths it out

Isn’t the electrical rotational frequency we should consider? Them what @Hummie said makes perfect sense, in a book I’m studying about BLDC motor design I remember the author saying the same but the wording was not clear enough to be sure

In this case running at 60k ERPM we would be just at 1 kHz and the skin effect would be much lower
```

---
## \#261 Posted by: Crisco Posted at: 2019-02-08T14:35:31.717Z Reads: 557

```
its not the speed that kills

...its the sudden stop
```

---
## \#262 Posted by: Pedrodemio Posted at: 2019-02-08T15:17:56.271Z Reads: 557

```
![image|500x330](upload://4XEPZNbHRWvh1h76beqktWaHHsl.jpeg) 

Or in our case the board suddenly becoming stationary and we keep going
```

---
## \#263 Posted by: Chrisjarram Posted at: 2019-02-12T21:51:10.231Z Reads: 530

```
Again fine, until we become stationary too
```

---
## \#264 Posted by: xilw3r Posted at: 2019-02-13T21:15:07.252Z Reads: 544

```
while this is a late reply and this is really an extremely dangerous battery, it will *probably* not kill you.

I know from experience unfortunatelly. I designed and built a 96S battery for a motorcycle. I was really careful but the fucking balance wires still managed to jolt me arm to arm at ~330VDC... like 5 times. It is not pleasant and you get some adrenaline, but you will live. Or I am a mutant of some sort.

edited because its late and i suck and the good people pointed it out
```

---
## \#265 Posted by: kalebludlow Posted at: 2019-02-13T21:17:32.848Z Reads: 523

```
What sort of ESCs exist that can handle voltage and current that high?
```

---
## \#266 Posted by: xilw3r Posted at: 2019-02-13T21:22:36.409Z Reads: 526

```
Some extremely expensive one that is custom made I suppose. Our company was just subcontracted for the battery with a bms and a case, so I have no clue :)

Edit: sorry for slight thread hijack, wont happen more
```

---
## \#267 Posted by: briman05 Posted at: 2019-02-13T21:28:50.608Z Reads: 515

```
The arc200 could probably handle it.
```

---
## \#268 Posted by: pat.speed Posted at: 2019-02-13T21:44:55.512Z Reads: 529

```
[quote="xilw3r, post:264, topic:81410"]
it will not kill you, this is DC after all.
[/quote]

That is not correct, a mere 30mA of dc is required to kill a human being. Yes dc is less dangerous than ac but it is still very dangerous. Especially at these high voltages as they ARE able to penetrate the resistance of the skin
```

---
## \#269 Posted by: Mich21050 Posted at: 2019-02-13T21:49:18.648Z Reads: 546

```
[quote="xilw3r, post:264, topic:81410"]
it will not kill you, this is DC after all.
[/quote]
Please don't say stuff like that... DC CAN kill you.. About 120v and 130mA and you could be dead... 
For example: Your heart is controlled using an electric impulse. This impulse could be interrupted or modified.. :slight_smile:
Just one way to die with DC...
```

---
## \#270 Posted by: murloc992 Posted at: 2019-02-13T21:52:09.011Z Reads: 557

```
[quote="Mich21050, post:269, topic:81410"]
This impulse could be interrupted or modified…
[/quote]

https://media.giphy.com/media/RyXVu4ZW454IM/giphy.gif

I am sorry, I just couldn't let this slip. :laughing:
```

---
## \#271 Posted by: xilw3r Posted at: 2019-02-13T21:53:11.467Z Reads: 537

```
ok jesus damn sorry for my wording yes milliamps of dc will kill you but it has to go in the right palce, meaning the heart. 
I dont know how I am still alive then. I will edit my post for the future generations
```

---
## \#272 Posted by: Mich21050 Posted at: 2019-02-13T21:55:38.638Z Reads: 525

```
[quote="xilw3r, post:271, topic:81410"]
meaning the heart.
[/quote]
It certainly will.. Your body resistance is not that big... :slight_smile:
You know there could be someone new to here and read this and be like.. Alright nothing to worry bc it's dc... I just don't want anyone get hurt.. :slight_smile:
```

---
## \#273 Posted by: murloc992 Posted at: 2019-02-13T21:57:48.061Z Reads: 521

```
[quote="Mich21050, post:272, topic:81410"]
I just don’t want anyone get hurt… :slight_smile:
[/quote]

...Or hack through time...

Okay I am out.

:laughing:
```

---
## \#274 Posted by: Mich21050 Posted at: 2019-02-13T22:03:19.673Z Reads: 511

```
Random:
Why does your profile picture remind me of "Donut Operator".. :joy:
```

---
## \#275 Posted by: linsus Posted at: 2019-02-14T13:38:39.178Z Reads: 524

```
[quote="pat.speed, post:268, topic:81410"]
Yes dc is less dangerous than ac but it is still very dangerous.
[/quote]
This is very debatable. DC makes your muscles go into unending cramp, AC penetrates alot more tho but In AC you atleast have a shot to let reflexes loosen the grip of w/e dangeruous you might have grabbed.
```

---
## \#276 Posted by: pat.speed Posted at: 2019-02-14T19:35:50.936Z Reads: 506

```
Really? I read the opposite the other day that ac makes your muscles contract a lot more visciously
```

---
## \#277 Posted by: Hummie Posted at: 2019-02-14T19:58:29.299Z Reads: 534

```
I read the ac, since on and off at maybe 120 per second, gives a bit of time to release.  Ac will get through a lower resistance too I read.  

 ironically you’re better off with a big zap, such as lightening, which will be so strong as to clench the heart as apposed to lower voltage which will put it in defibrillation. Only 1 in 10 people hit by lightening are killed while 1 in 4 noobie eskate enthusiasts get killed trying to put on an xt-90 plug with a blindfold.  Always leave a little peak hole if youre blindfolded
```

---
## \#278 Posted by: venom121212 Posted at: 2019-02-14T20:02:15.304Z Reads: 523

```
AC kills elephants! At least, that's what Edison proved trying to scare people away from Tesla and AC...
```

---
## \#279 Posted by: Hummie Posted at: 2019-02-14T20:05:26.240Z Reads: 527

```
Seems the frequency at 60 on and off per min, which we have in USA, has the most penetrating effect
```

---
## \#280 Posted by: venom121212 Posted at: 2019-02-14T20:07:17.556Z Reads: 535

```
Yeah I don't want to do the math on the piezoelectric numbers for human flesh. I didn't know you were in the US. Where outta may I ask?
```

---
## \#281 Posted by: Hummie Posted at: 2019-02-14T20:13:44.212Z Reads: 556

```
Sunny Francisco ca
```

---
## \#282 Posted by: Hummie Posted at: 2019-02-14T20:15:33.434Z Reads: 557

```
https://en.m.wikipedia.org/wiki/Piezoelectricity

Heard they’ve used it to power lights on the road while the piezoelectric stuff is in the road with cars rolling over
```

---
## \#283 Posted by: venom121212 Posted at: 2019-02-14T20:21:16.817Z Reads: 540

```
Recycling thermal generated energy is tough but key in future tech. I bought a wireless light switch the other day that requires no charge and uses the resistance from toggling the switch manually a few times to keep it charged perpetually. Genius.
```

---
## \#284 Posted by: janpom Posted at: 2019-02-14T20:48:55.700Z Reads: 540

```
[quote="Hummie, post:279, topic:81410"]
60 on and off per min
[/quote]

You mean "per sec", right?
```

---
## \#285 Posted by: murdomeek Posted at: 2019-02-14T20:53:00.320Z Reads: 534

```
yeah, definately 60 per second
(60hz)
```

---
## \#286 Posted by: linsus Posted at: 2019-02-14T21:17:21.034Z Reads: 541

```
Actually about to start developing an ASIC for pacemakers, that harvests piezoelectric energy from the heart... dont tell anyone tho, alot of NDAs etc.
```

---
## \#287 Posted by: venom121212 Posted at: 2019-02-14T21:22:50.443Z Reads: 537

```
Oooh deal. I've got zika in my fridge cooking up something good so we're even :wink:
```

---
## \#288 Posted by: MoeStooge Posted at: 2019-02-14T21:27:29.881Z Reads: 542

```
I'm a HV lineman by trade. For a/c secondary voltage.  120 will make you grab and hang on.  240 is characterized as "safer" because it will blow you off it.  Lol I'm not willing to test this, but that's what they say in the trade.  DC can make an entry wound on your skin at 60v.  It takes 50miliamps (nothing) to stop the human heart at 120v ac.
```

---
## \#289 Posted by: totalgeek9224 Posted at: 2019-02-14T21:31:51.316Z Reads: 535

```
The new meta is bringing a defib wherever we go, havent you heard? 
/s
```

---
## \#290 Posted by: linsus Posted at: 2019-02-14T21:32:40.220Z Reads: 550

```
Nice, have a friend in the same trade. He had a major accident while back. Many risks involved, hat off to you sir. 

I've been hanging under a 10kV transformer changing venting fans...65m up in the air in a windmill. Shit was turned off ofcourse.. but still.. shat my pants few times feeling the wind blowing in my neck..
```

---
## \#291 Posted by: Pedrodemio Posted at: 2019-02-14T21:33:16.495Z Reads: 552

```
Damn guys, everytime I see lots of posts here I'm hoping for a new update but it's just people saying things that don't matter, like someone could die and etc :confused:
```

---
## \#292 Posted by: FullMetal_Machinist Posted at: 2019-02-15T08:13:54.611Z Reads: 590

```
Updates soon.
Was busy with making some money to live on.
Thread hijacked by masochistic shock-lovers for now. Hope they find new thread soon.
I think only way to shoo them away is with updates!
Had some troubles with making ESC work properly but it was finally (1 week of scratching my head) traced to poor choice of op-amp in current sense section, it had large DC offset and lot of noise. After replacing op-amp with different model i hope everything will be ok, as LM358 had offset of 1mv (about 4 amps of current measurement at 0,25 miliohm) and i have ordered OP626 which has 0,012mv.
Voltage and current dividers are fixed in firmware and ok, deadtime reduced, but running sensorless was still a mess.
Also have some problems with motors as gap between stator and rotor is too big and not enough magnetic flux goes into the windings. As a result motor has bigger KV than designed and less torque. Will have to redo the hubs with internal diameter smaller by 0,5mm. Temporary fix will be to glue some 0,25mm thick steel on top of the magnets to take measurements. Magnetically equal to having smaller bell  diameter. Good thing i have ordered more magnets.
```

---
## \#293 Posted by: Pedrodemio Posted at: 2019-02-15T12:14:46.375Z Reads: 566

```
What airgap size are you aiming?
```

---
## \#294 Posted by: FullMetal_Machinist Posted at: 2019-02-15T12:43:00.680Z Reads: 575

```
initially wanted some 0,8mm but it is too much.
Was afraid that due to axle deflecting under weight stator might rub on the rotor.
```

---
## \#296 Posted by: Sn4pz Posted at: 2019-02-18T12:28:44.293Z Reads: 618

```
![tenor%20(3)|400x448](upload://oZMLeJKg5AGSgHDM8pk4gPIjXaB.gif)  

@FullMetal_Machinist can't wait to see it until it's done... Sometimes I like not visiting build threads until they're done.... Might do that with this one so it's a surprise 😂😂
```

---
## \#297 Posted by: B_in_tha_OZ Posted at: 2019-02-21T00:53:25.819Z Reads: 617

```
Your a madman, can’t wait to see the results and how you overcome the traction control problem from all that torque. The power to weight ratio is going to be insane. Keep up the good work and good luck
```

---
## \#298 Posted by: Chrisjarram Posted at: 2019-02-22T08:12:51.131Z Reads: 622

```
Better be wearing leathers!

https://youtu.be/roO4P0cTN48
```

---
## \#299 Posted by: rpasichnyk Posted at: 2019-02-22T22:04:56.560Z Reads: 615

```
Really hope you can finish this project! So exciting! So much overkill!
```

---
## \#300 Posted by: eb1925 Posted at: 2019-02-24T07:20:32.459Z Reads: 605

```
@MoeStooge goes more faster
```

---
## \#301 Posted by: Stielz Posted at: 2019-03-08T00:13:37.889Z Reads: 600

```
All good? How are you getting on with your motor fix?
```

---
## \#302 Posted by: B_in_tha_OZ Posted at: 2019-03-08T06:42:41.737Z Reads: 599

```
This is insane. Wonder what sort of mileage he'd get?
```

---
## \#303 Posted by: harrypzee Posted at: 2019-03-08T19:10:37.369Z Reads: 579

```
@FullMetal_Machinist This is insane and awesome. I love it. Makes me think of the quote from Jurassic Park "Your scientists were so preoccupied with whether or not they could, they didn’t stop to think if they should."
```

---
## \#304 Posted by: FullMetal_Machinist Posted at: 2019-03-09T07:21:20.270Z Reads: 596

```
I am currently sorting out the ESC.
Current measurement is fixed.
After setting dead times and soldering all power bus bypass capacitors mosfet drivers started to give up, loosing gate drive on high side.
Cause was traced to negative transient on gate drive pin during mosfet turn-off.
Drivers i chose initially can withstand up to -0,3v (datasheet), measured -1,0v.
Found another drivers, slightly slower, but up to -2,0v transients.
When it is done i will post results.
Cheers!
```

---
## \#305 Posted by: ricardo Posted at: 2019-03-12T07:31:23.483Z Reads: 600

```
![image|354x500](upload://bIL8t1PW8L7OS6EEf2nheQqA8FR.jpeg)
```

---
## \#306 Posted by: macncheese Posted at: 2019-04-10T00:56:45.150Z Reads: 557

```
My 10S18P is probably not big enough for his remote.
```

---
## \#307 Posted by: AlanZhou Posted at: 2019-04-10T02:00:52.661Z Reads: 544

```
damn you beat me im making a 13s10p :sob:
```

---
## \#308 Posted by: b264 Posted at: 2019-04-10T02:01:55.527Z Reads: 551

```
[quote="Pedrodemio, post:242, topic:81410, full:true"]
Be careful off water creeping in via the wires, for example from the motor, burned my RC car ESC that way, took more than a year of use, the esc was completely sealed, but eventually enough water came thorough the phase wires and boom
[/quote]

This happened at my old house.  The water came in the house through the power cable, inside the insulation, and got all over inside the power box and the wall.
```

---
## \#309 Posted by: evoheyax Posted at: 2019-04-10T02:02:55.337Z Reads: 519

```
Lol he’s. Everyone with their overkill batteries. Though I must say, it’s nice to know you can do 30+ miles of aggressive riding without thinking about charging.
```

---
## \#310 Posted by: AlanZhou Posted at: 2019-04-10T02:07:24.223Z Reads: 524

```
I draw 27 ish wh/ mile and im 115 lbs can't imagine how much I will draw when I grow up :rofl::sob:

I'll get around 53 miles according to the calculations of my 13s10p being around 1.5kwh

^some slow ass guy can prolly get 100 miles outta it
```

---
## \#311 Posted by: yelnats8j Posted at: 2019-04-10T02:10:25.986Z Reads: 516

```
[quote="AlanZhou, post:307, topic:81410"]
im making a 13s10p
[/quote]

😭😭😭😭

Every damn time you gotta compare your size.
```

---
## \#312 Posted by: AlanZhou Posted at: 2019-04-10T02:12:57.040Z Reads: 502

```
yes what size you got a 6s1p? :joy:

jkjk\

@yelnats8j also when you coming to NYC?
```

---
## \#313 Posted by: evoheyax Posted at: 2019-04-10T02:14:35.654Z Reads: 505

```
I get about 40 miles in normal conditions with my 1100wh battery. If I really push it, I eat at least 80wh per miles.
```

---
## \#314 Posted by: AlanZhou Posted at: 2019-04-10T02:16:10.322Z Reads: 496

```
hmmmm? i mean i drained a raptor 2 in 9 miles do i hold a record? :rofl:
```

---
## \#315 Posted by: yelnats8j Posted at: 2019-04-10T02:16:37.202Z Reads: 507

```
Some time this summer

I will be up there next week but sadly only for a day and Ive got no time to ride

Waiting on the redember still 😔
```

---
## \#316 Posted by: AlanZhou Posted at: 2019-04-10T02:17:10.414Z Reads: 496

```
well be happy cause none of my board are working...
```

---
## \#317 Posted by: yelnats8j Posted at: 2019-04-10T02:18:50.187Z Reads: 513

```
Same atm

My OG board finally died and it doesnt look like its gonna be working soon.

Hey and if you dont get your board working by summer you can borrow the Tayto for the day, its no 13s10p but its still a lotta fun.
```

---
## \#319 Posted by: evoheyax Posted at: 2019-04-10T02:28:42.892Z Reads: 512

```
I would kill a 12s4p in 4 miles sorry lol
```

---
## \#320 Posted by: b264 Posted at: 2019-04-10T02:35:32.782Z Reads: 539

```
[quote="AlanZhou, post:314, topic:81410"]
i drained a raptor 2 in 9 miles do i hold a record?
[/quote]

You do indeed hold a record -- 9 miles is the furthest any Raptor 2 has gone without breaking-down
```

---
## \#321 Posted by: yelnats8j Posted at: 2019-04-10T02:36:28.299Z Reads: 531

```
It was probably because his remote got stuck at 100%
```

---
## \#322 Posted by: AlanZhou Posted at: 2019-04-10T02:37:41.619Z Reads: 550

```
[quote="b264, post:320, topic:81410"]
9 miles is the furthest any Raptor 2 has gone without breaking-down
[/quote]

oouf why gotta do it so dirty, it wasnt even my raptor :rofl::joy::joy:
```

---
## \#323 Posted by: Skyart15 Posted at: 2019-04-10T02:54:02.140Z Reads: 547

```
It looks like an eraser
```

---
## \#324 Posted by: Noah Posted at: 2019-04-10T03:07:04.644Z Reads: 556

```
Can I ride it? Ill sign a release form :smile:

 ![dear-baby-jesus-i-wanna-go-fast|475x354](upload://xLY6gm3FxQiIeMqHqopWPE1fRHA.jpeg)
```

---
## \#325 Posted by: DEEIF Posted at: 2019-04-10T03:51:33.166Z Reads: 538

```
Bet I could get around 90-100 with my regular slow speed....(15-20mph avg, 90-95ish pounds, 5ft...) 🙃
```

---
## \#326 Posted by: evoheyax Posted at: 2019-04-10T04:22:36.889Z Reads: 533

```
You know, I just found out someone ate it during the first raptor 2 tour In sf be ause a truck broke haha
```

---
## \#327 Posted by: ElectricHabitatLeaf Posted at: 2019-04-10T04:51:50.182Z Reads: 554

```
To reduce speed wobble:
#1 speed wobbles are caused by the rear end steering. In cars the rear end doesn't steer so they never get wobbles. Solution:
have much stiffer suspension at the rear than at the front, this will force the board to steer with the front more than the rear, hence making it much more stable at speed. Because if you ever tried pushing a grocery cart backwards, you notice how hard it is to steer because when the rear end steers its much more sensitive than when the front end steers. 
I tighten up my rear trucks more than the front and never worry about speed wobbles. 
#2 maybe use longer wheelbase than any regular longboard to help with high speed stability? There's a reason why hyper cars are almost as long as pickup trucks
#3 tight as heck suspension. Why do sports cars have stiffer swaybars? Less bodyroll. Which makes them stable at high speed and at cornering. 

Use the 3 points I mentioned and you could probably get away with going 100kph using a really long deck and regular reverse kingpin trucks that are concrete tight at the rear and almost as tight at the front. 

I'm just a car mechanic, have been building and tuning my own cars. Also I'm into electric skateboards recently. This is just my 2 cents.
```

---
## \#328 Posted by: ricardo Posted at: 2019-04-10T06:52:06.018Z Reads: 516

```
are there any news on this build @FullMetal_Machinist ?
```

---
## \#329 Posted by: FullMetal_Machinist Posted at: 2019-04-10T07:25:13.312Z Reads: 532

```
ESC is sorted out good enough for me, new mosfet drivers helped, nothing blows up.
With my big motors it will run BLDC or FOC sensored.
It wont run unsensored under 10 amps, too much noise in current sense for that.
Got a hold of company that makes wind turbines and has motor simulation software.
I will try to persuade them to simulate my motor and figure optimal magnet-stator spacing, before i waste more magnets. 
Slow progress due to too much IRL problems. 
Cheers!
```

---
## \#330 Posted by: Pedrodemio Posted at: 2019-04-10T12:45:10.410Z Reads: 525

```
If you have time play with this

Has a few days of free trial 

https://www.mentor.com/products/mechanical/motorsolve/bldc/
```

---
## \#331 Posted by: FullMetal_Machinist Posted at: 2019-04-12T18:45:59.412Z Reads: 538

```
I have tested several configurations using this software in trial mode and here is result:
problem was not with rotor-stator spacing but with spacing between magnets.
Too much flux was "taken away" and formed closed loop between magnets without going into the stator.
When magnet count is reduced to 34 and winding scheme is different motor produces designed parameters - 60 nm at 350A, peak stator flux 2,2T - just at steel core saturation point (at peak current). Spacing between magnets is increased form 0,25mm to 2,0mm.
Total motor efficiency chart varies between 82% (at low RPM or low torque) to 96% in central region. Winding 2 turns delta or 1 turn wye.
Now proceeding to manufacturing test piece.

Simulation results of existing configuration (42N36P) were within 3% of measured values from last test piece so i am certain simulation is accurate.

Cheers!
```

---
## \#332 Posted by: Hummie Posted at: 2019-04-12T19:20:05.217Z Reads: 559

```
With saturation starting at 1.6t and 2.2t being maybe the max possible flux strength of electrical steel I guess ur going for the peak possible output regardless of efficiency then. Where will u even find a load big enough to get to such current?  I feel we’d need to strap u down and send u up the steepest thing possible. 

https://en.m.wikipedia.org/wiki/Saturation_(magnetic)
```

---
## \#333 Posted by: Pedrodemio Posted at: 2019-04-12T19:25:46.971Z Reads: 530

```
Nice, and with 42N36P you have a better winding factor of 0.966

How do you arrived at this conclusion? Just looking at the flux lines diagrams? Good find, maybe other hub motors also suffer from this since most have the magnets touching 

And could you post the results of the final design? Mainly the rpmx(torque/efficiency/current/loss) diagram for it?

And a Hummie said, the flux is a bit high, but since you will probably never run at the peak for more than a few seconds its all good
```

---
## \#334 Posted by: FullMetal_Machinist Posted at: 2019-04-12T19:38:44.013Z Reads: 528

```
Flux density reaches 2,2T at max current of 350A.
It is under 1,5T when current does not exceed 250A.
I made simulations for different values of current.
So for normal riding no saturation and very high efficiency, at peak power i am going for highest torque and flux possible, **slightly** disregarding efficiency, however still somewhere above any ready-made motor. Value of 96% efficiency is present at 60% of max rpm and 30-50% of torque (going at 100 kph continous).
I agree that with 42N36P winding factor was slightly better but with 34N36P it is 0,9525 and i get a lot less cogging (0,15 Nm peak 0,07Nm average), which means less noise and smoother ride.
Right now i am just happy to fnally pinpoint the problem and find solution.
All components i have are correct and can be used to get result.
```

---
## \#335 Posted by: FullMetal_Machinist Posted at: 2019-04-12T19:47:26.924Z Reads: 537

```
I got to the solution by simulating over 20 motor configurations with different airgap and magnet count. 38 magnets go with same winding scheme but not nearly as good.
Airgap is about 0,8mm optimal but it is thanks to N52 magnets. With N38 0,4mm is good, which would cause rotor to rub stator under my weight.
With 42 magnets airgap would need to be under 0,2mm, which is not physically possible to make.
Then i tried different magnet counts and found best solution.
I could go with even fewer magnets but then power and torque would suffer too much.
```

---
## \#336 Posted by: FullMetal_Machinist Posted at: 2019-04-12T20:12:15.281Z Reads: 575

```
![1|625x500](upload://gI0T9Gd14apZwmwUiEffgNuZaXt.jpeg) ![2|625x500](upload://nShUP64i8sS0gqVdfJQMHPRjeUp.jpeg) ![3|625x500](upload://3WAydkwLvaaNXbylA6lgzqFf1jS.jpeg)
```

---
## \#337 Posted by: Hummie Posted at: 2019-04-13T06:30:50.994Z Reads: 529

```
to get the motor to bend it will take a lot more than your weight and shouldn’t be a concern with deciding the airgap width.  How much are u going to assume is going to glue?
```

---
## \#338 Posted by: FullMetal_Machinist Posted at: 2019-04-13T06:43:29.157Z Reads: 548

```
i am concerned about truck axle, bencause relative position of rotor depends on axle deflection. Rotor is wheel hub itself. I have not measured how much axle bends under 100kg load, but i am certain that when landing a jump or going up a curb there will be some rubbing.
There was topic about axle deflection somewhere on this forum.
If i ever have to redo the trucks i will make axle 17mm.
As for the glue nothing goes to it bencause magnet squeezes out any glue from under it in split second, as it sticks with about 10kgs of force to the steel hub by itself.

One more thing - **efficiency chart INCLUDES ESC loss** - i had to input ESC parameters to calculate motor efficiency.
```

---
## \#340 Posted by: pat.speed Posted at: 2019-04-13T12:55:44.650Z Reads: 528

```
He must not be using a stator pipe, this means as the axle bends one end of the stator may rub
```

---
## \#341 Posted by: FullMetal_Machinist Posted at: 2019-04-13T13:03:38.374Z Reads: 547

```
Just found another way to mitigate this problem.
I just need to insert 3rd bearing at the end of stator.
This is going to be low-profile bearing, similiar to one supporting bell end in bigger motors. Rotor is sturdy enough, no need to reiforce it further.
This way it will behave like it was stator pipe.
Stator is mounted very sturdily, with at least 6mm of 7075 aluminium anywhere.
As i have to machine 4 new hubs anyway it is a good timing for improvements.
Look at photos i published previously - it will become clear.
```

---
## \#343 Posted by: yelnats8j Posted at: 2019-04-13T15:01:31.223Z Reads: 547

```
[quote="Miniproto, post:342, topic:81410"]
but going 100 mph
[/quote]

May I ask, WHY???
```

---
## \#344 Posted by: Hummie Posted at: 2019-04-13T15:37:43.839Z Reads: 575

```
I don’t know what a stator pipe is and can’t tell by your pics but surely with bearings on both sides of the rotor nothing should be bending.  You should be able to make a .2mm airgap thickness safely.  
Lately I’m thinking the bigger the bearing the better for more durability and less maintenance.  If u can get to each bearing’s seal without having to take the motor apart it makes it much easier. 

Are u pressing the bearings or gluing them?  How tight are your machine tolerances?  I’m hoping to do press fitting parts as supposed to retaining fluid but it’s very expensive.
```

---
## \#345 Posted by: FullMetal_Machinist Posted at: 2019-04-13T16:18:26.047Z Reads: 588

```
![4|641x500](upload://mbDStbYdUO6sOM0HukEFezxy47R.jpeg) 
Cross-section of wheel hub motor.
Here is the difference with 3rd 61808 bearing (52x40x7) added.
As for the tolerances i can easily do 0,01mm or better, it only takes few minutes more on a manual lathe for 1-2 finishing passes with sharp tool.
All bearings are press-fit, tolerance is about 0,005 to 0,01mm too tight.
```

---
## \#346 Posted by: DeepSeaSwan Posted at: 2019-05-03T15:42:13.797Z Reads: 548

```
This is gonna be insane. are you considering a dampening system? maybe coil over? 9-12 in tires seems huge.
```

---
## \#347 Posted by: DeepSeaSwan Posted at: 2019-05-03T15:44:42.088Z Reads: 547

```
1 HELLA FAST mile.
```

---
## \#348 Posted by: trapsends Posted at: 2019-06-21T11:20:52.980Z Reads: 474

```
yo, hows it going, whats the progress?
```

---
## \#349 Posted by: FullMetal_Machinist Posted at: 2019-06-25T16:02:16.980Z Reads: 453

```
Much slower than i would like to due to several jobs i took simultainously, one of them being machining a hybrid rocket motor from stainless steel for students building a rocket.
Currently there is no way for me to finish in time for Paris meeting.

ESC is sorted good enough, motors are in final machining, deck is missing (not moulded yet).
```

---
## \#350 Posted by: drangboards Posted at: 2019-06-27T04:20:13.683Z Reads: 438

```
Hey, Ive been doing decks for a really long time.  I had some input on the kicks of your board, they seem way steeper than you might want them to be once the thing is all done.  Maybe I can help...
```

---
## \#351 Posted by: FullMetal_Machinist Posted at: 2019-06-27T06:38:17.036Z Reads: 429

```
I have a guy here locally who has the press and makes decks.
Mould is not yet finished , few hours are needed for it.
```

---
## \#352 Posted by: Harrisonwms Posted at: 2019-07-03T05:48:04.809Z Reads: 412

```
Please do show show us all the insane monster when it’s complete!!
```

---
## \#353 Posted by: evoheyax Posted at: 2019-07-03T14:21:10.239Z Reads: 414

```
[quote="FullMetal_Machinist, post:335, topic:81410"]
airgap would need to be under 0,2mm, which is not physically possible to make
[/quote]

Hummie hubs are .2mm airgap with n48sh... If you engineer things right, nothing should deflect or bend.
```

---
## \#354 Posted by: Harrisonwms Posted at: 2019-07-05T06:46:46.809Z Reads: 401

```
Any update?
```

---
## \#355 Posted by: FullMetal_Machinist Posted at: 2019-07-07T06:42:57.101Z Reads: 398

```
Not for at least 2 more weeks. Currently i do not have enough time to properly scratch my ass, let alone continue the project. However when storm passes, i will progress ASAP.
```

---
## \#356 Posted by: Harrisonwms Posted at: 2019-07-07T07:02:50.776Z Reads: 391

```
Copy that.
```

---
## \#357 Posted by: Harrisonwms Posted at: 2019-07-24T01:29:23.634Z Reads: 375

```
Any progress?
```

---
## \#358 Posted by: Dirt_Bag Posted at: 2019-07-24T04:41:01.396Z Reads: 380

```
@FullMetal_Machinist i am dying to see more.
```

---
## \#359 Posted by: Harrisonwms Posted at: 2019-07-31T17:54:28.373Z Reads: 364

```
Any update?
```

---
## \#360 Posted by: FullMetal_Machinist Posted at: 2019-08-01T06:52:52.332Z Reads: 356

```
starting monday i will have some time to finish working on motors.
Cheers!
```

---
## \#361 Posted by: Harrisonwms Posted at: 2019-08-01T10:11:56.543Z Reads: 355

```
Goodluck!!
```

---
## \#362 Posted by: Harrisonwms Posted at: 2019-08-12T03:34:46.000Z Reads: 323

```
How’s it going?
```

---
## \#363 Posted by: amms50 Posted at: 2019-10-21T20:35:03.352Z Reads: 232

```
Updatessss????
```

---
## \#364 Posted by: Fosterqc Posted at: 2019-10-21T22:14:40.412Z Reads: 236

```
9 grand in parts sitting there... 

Gotta work to live I guess.
```

---
## \#365 Posted by: murdomeek Posted at: 2019-10-22T21:24:41.781Z Reads: 225

```
@FullMetal_Machinist
```

---
## \#366 Posted by: Benjo Posted at: 2019-11-07T21:35:52.944Z Reads: 188

```
@FullMetal_Machinist did you die during a test ride? 😢 Long time no see
```

---
## \#367 Posted by: PixelatedPolyeurthan Posted at: 2019-11-08T17:51:16.719Z Reads: 176

```
a build requiring so much maths even shart would shit his pants...
```

---
## \#368 Posted by: VIV Posted at: 2019-11-20T17:55:44.698Z Reads: 115

```
Hi! 
Great project! 
From 3 years ago i worked my self in a project identical similar to yours, high powered lightweight outrunner brushless hub electric motor direct drive. 
My research conducted me to a brushless outrunner, helical hallbach array neodymium config, coreless (statorless), helical aluminium coil, and like you, a lot of power, voltage, to give lots of torque, in ultra lightweight performance design.
But with low budget i never ended... 
After seeing all your fantastic work I think a god solution improvement for your project is the implementation of hallbach array config neodymium.
I don't know if it helps.
Maybe it's to late or not applicably.
Amazing project I say! I'm dying to see it working.
Keep on going! ;)
Sorry for my English.
Best regards.
```

---
