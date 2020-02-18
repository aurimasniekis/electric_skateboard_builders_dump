# Small wheel hub motors

### Replies: 115 Views: 6833

## \#1 Posted by: brams Posted at: 2016-07-25T13:29:45.532Z Reads: 260

```
I would like to consider the option of hub motors for my tiny board 24" with small wheels.
I think I can fit a 5030 or 5035 motor into the 59mm urethane wheel. With a dual drive system, a 6S battery and 25kmh max, I would need 100kv motors. Is it technically possible with the copper inside a 5030/5035 to get such a low kv?
```

---
## \#2 Posted by: devin Posted at: 2016-07-25T13:50:51.882Z Reads: 245

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#3 Posted by: brams Posted at: 2016-07-25T14:01:20.685Z Reads: 229

```
I'm planning to build a custom hub motor. But before that, I need to be sure that's technically possible...
```

---
## \#4 Posted by: devin Posted at: 2016-07-25T15:19:32.457Z Reads: 214

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#5 Posted by: brams Posted at: 2016-07-25T15:35:46.320Z Reads: 202

```
The fact that I'm considering a dual drive and a 25kmh max speed couldn't cool down the motors?

Also boosted boars seems to use small motors in dual without heat issues...
```

---
## \#6 Posted by: devin Posted at: 2016-07-25T15:48:08.526Z Reads: 201

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#7 Posted by: KMeyerson Posted at: 2016-07-25T16:58:38.997Z Reads: 176

```
I've got some CAD files from a 40 and 50mm hub motor that was once in design if you're interested. 

The idea was scrapped because it simply wasn't powerful enough in practice. If the stator is lengthened, it would probably work, but them its not truly a hub motor so much as a motor that has some thane attached to it.
```

---
## \#8 Posted by: brams Posted at: 2016-07-25T17:08:39.797Z Reads: 176

```
Yeah would love to see these CAD!

Were you considering dual drive at the time ?
```

---
## \#9 Posted by: KMeyerson Posted at: 2016-07-25T17:34:28.934Z Reads: 173

```
Yeah. You'd need 4x drive with these wheels.  If you lengthen the stator (1.5-2x) you might be OK.
```

---
## \#10 Posted by: Hummie Posted at: 2016-07-25T17:51:40.593Z Reads: 179

```
http://shop.subsonicplanes.com/category.sc?categoryId=48

I've never seen these before!! And I looked a lot. Good stuff. Bit expensive.  
Im selling the smallest hub motors I've seen for sale.  Steelhubs.com.  help me make these!  It's still experimental and progressing.  I use a rare 4725 stator soon to be 4727.
```

---
## \#11 Posted by: KMeyerson Posted at: 2016-07-25T21:18:20.971Z Reads: 179

```
@Hummie I dunno, I know people like the 60-80mm wheel sizes, but I feel like big wheels are better for eBoards because the inertia will carry you further than a smaller diameter wheel will (plus smooth ride).  Heat buildup is an issue you'll have with making things smaller.

@brams Boosted can get away with small motors because of two features hub motors do not have:
1. Gearing (meaning that the work to turn the wheel is distributed over several rotations, whereas a Hub Motor is a 1:1 direct drive).
2. Cooling (Boosted Motors are exposed to the air without insulation. Hub Motors are heavily insulated by the wheels around them and warmer due to the amount of power needed to generate sufficient torque).

**My opinion on the current state of community hub motors:**
Before I bring out the haters and criticisms, they all bring different things to the table and are all pretty incredible. These notes compare Size/Heat/Shock + Sliding Durability based on what I've seen and what I would predict from the designs I've seen.

A) Hummie Hubs are small and dense but get a little on the warm side (still safe and good, and not really an issue unless considering thermal waste and the potential for a shorter life due to thermal wear-down on the windings/magnets).  The bell + cap design should hold up against most sliding and shock damage.

B) Jacob's Hubs are large in diameter and stay cool thanks to their decent ventilation (perform as well as Hummie's for practical purposes. They generate less thermal waste but are probably more susceptible to mechanical wear [as in they're tough, but I doubt they'd hold up against serious sliding]).

C) Carvon Hubs are essentially normal motors that are inline with the wheel and probably get as warm as a same size motor geared 1:1. They're a different breed of hub motor from A or B.  I have not read a recent comparison, but I would assume they stay relatively cool since they're exposed and imagine that they're mechanically susceptible to both sliding and shock by design, but I've heard nothing to support my imaginings.).
```

---
## \#12 Posted by: evoheyax Posted at: 2016-07-25T22:30:12.094Z Reads: 157

```
Right now, of the three you listed, I would say the carvons are the least problematic. I say that cause I can't do my normal route with hummies motors without having to stop multiple times to cool them down. 

Because of the design on carvons, you can have the gear inside slip, and eat up the inside grooves design to hold the plastic gear ring in place. This only seems to be a problem if the board is jointed hard, and you don't notice the ring slightly popped out and kep riding, as happened to me. I also had the hanger bend on the carvon, which is scary.

With hummies, mechanically, they are sound motors. Ridden many miles, with both the aluminum and now the steel. Temps are slightly better on the steel, but still too hot. My test is an 8 block test, which involves a 2 blocks of flat, 1 block of steep hill, followed by 1 block of flat, a block of slight up, 2 blocks down, 1 block flat, and 1 block up a slight hill again. on the aluminium, I was at 245 F, way too hot. The steel got to 198 F, which is still too hot. Part of my problem could be the difference between 10s and 12s. The other part is likely the low amp limits, due to the limits of the space cell. I did do a test climbing a hill with my laptop connected to the vesc. It shows me hitting do a constant 26-27 amps on one motor (the limit is set to 25). What this says to me is, I need a 12s that can pull more amps. Maybe 50 pounds is the difference, but hummie has very little heating issues, and generally doesn't take breaks, while I find my self always taking breaks to let them cool.

Bottom line, I think a 4wd hub settup using hummies motors is the best option. Will get lots of torque, and will keep the motors much cooler (at least, that's the hope). This is what I'm building right now, and am almost done with.
```

---
## \#13 Posted by: KMeyerson Posted at: 2016-07-25T22:52:40.518Z Reads: 147

```
Bottom line for me is that hub motors shouldn't be too small. If you're really keen on this, get in touch.

I predict that the smaller the hub motor, the thinner the wire gets. Therefore you'll need more voltage  and fewer amps (to keep cool for the same performance).  The VESC can't do 12s or more reliably and Jaanb's motors are wound with 0.19mm wire.

You'll need a higher voltage ESC and a higher voltage battery.  The development costs for a hub motor hovers in the $2,000-$5,000 range right now so all things considered, it's not economically worth it unless you're selling it to offset the investment.
```

---
## \#14 Posted by: evoheyax Posted at: 2016-07-26T02:50:08.579Z Reads: 141

```
[quote="KMeyerson, post:13, topic:6590"]
I predict that the smaller the hub motor, the thinner the wire gets.
[/quote]

Not necessarily. Hummie showed me his motor vs a tacon 160 today. His stator is much smaller than the tacon but the wire is much much thicker.
```

---
## \#15 Posted by: Hummie Posted at: 2016-07-26T05:57:44.460Z Reads: 139

```
no cooler motors from higher voltage.  the classic amps and volts equal watts equation ...the volts get converted to amps in the motor or something like that.  Vedders site has a better explanation.  

the motors are small.  stators small.  more power out of this little size though is definitely possible.  nothing magic but theres room for more copper for sure and a bit longer stator.  stronger magnets.  Yea it could get longer too and that would be another way to go instead of wider.

it all depends on what you expect though.  I can blast from one side of the city to the other at 25mphplus all day long.  evohyax is a big guy and travels some long steep blocks but for me the same blocks arent a question and I do much steeper.  I have a trigger finger and go everywhere fast and I'm happy on the terrain in san francisco.  I've ridden the boosted and the evolve gt and these two motors blow them away.
```

---
## \#16 Posted by: brams Posted at: 2016-07-26T09:51:19.608Z Reads: 136

```
Still, I just found out that carvon is selling these Chinese EMC boards
http://www.carvonskates.com/store/p32/CARVON_Emc_--_Electric_Mini_Cruiser_with_Single_Hub_Motor.html
which are no more than these https://wholesaler.alibaba.com/product-detail/Sport-electric-skateboard-with-remote-control_60493394037.html?spm=a2700.7782932.0.0.syld9Q

It's 6S 2500mah powered by Samsung 18650 with a 400w carvon/hub motor in 70mm wheels.
400/(6*3.7) = 18 amps per hub. It's not very powerful but I'm still talking about a 22-24" deck.

Maybe I can reverse engineer these hubs to stuff them in 59mm wheels. I'm curious what KV these are and what stator size they use.

EDIT : Just found the complete tear apart here! https://www.flickr.com/photos/kasparsdambis/albums/72157667661928215
```

---
## \#17 Posted by: devin Posted at: 2016-07-26T13:12:32.904Z Reads: 134

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#18 Posted by: brams Posted at: 2016-07-26T13:47:44.245Z Reads: 126

```
+1 to the fact that volts DOES NOT convert to amps. Still seeing this all over the board.
```

---
## \#19 Posted by: Hummie Posted at: 2016-07-26T15:51:47.737Z Reads: 126

```
http://vedder.se/forums/viewtopic.php?f=6&t=6&start=60
```

---
## \#20 Posted by: devin Posted at: 2016-07-26T15:55:50.431Z Reads: 125

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#21 Posted by: Hummie Posted at: 2016-07-26T15:59:36.201Z Reads: 119

```
my analysis tells me to listen to what these people say.

http://vedder.se/forums/viewtopic.php?f=6&t=6&start=10
```

---
## \#22 Posted by: devin Posted at: 2016-07-26T16:03:34.735Z Reads: 117

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#23 Posted by: Hummie Posted at: 2016-07-26T16:05:08.800Z Reads: 111

```
I'm saying yes they get converted to amps or something like that.  sign up on vedders thing and ask those guys how it works or read the whole thread.

you do not get a cooler motor from more voltage that much is true, the details I cant explain
```

---
## \#24 Posted by: devin Posted at: 2016-07-26T16:06:57.634Z Reads: 110

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#25 Posted by: Hummie Posted at: 2016-07-26T16:07:33.790Z Reads: 106

```
you dont have to sign up for anything and just read it.  then maybe you can explain.  the fact remains no cooler motors with more volts.  INfact more likely the opposite as the no-load speed is now further away and more inefficient unless going faster
```

---
## \#26 Posted by: devin Posted at: 2016-07-26T16:08:56.984Z Reads: 104

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#27 Posted by: Hummie Posted at: 2016-07-26T16:09:33.940Z Reads: 99

```
go tell vedder.   this is a repeat conversation i've had a couple times.  sometimes people freak out and tell me I'm an idiot.  best you go to the source and shoot them not  me
```

---
## \#28 Posted by: devin Posted at: 2016-07-26T16:11:20.833Z Reads: 95

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#29 Posted by: brams Posted at: 2016-07-26T16:20:31.049Z Reads: 98

```
@devin  
I think that @Hummie just misread the Vedder explanation.

Vedder simply illustrate the Amps * Volts = Watts equation, at the same Power (Watts) the heat is the same regarding if you add more Volts or Amps.
Example : 10A * 3.7V = 37W and 1A * 37V = 37W. The heat is the same, the balance is different.
You have to keep in mind that heat is generated by the losses in the motor, and this heat is calculated in Watts.

Now, Vedder never stated that amps convert to volts, that simply basic knowledge of electricity.
```

---
## \#30 Posted by: PB1 Posted at: 2016-07-26T16:22:44.971Z Reads: 98

```
@Hummie and @devin just to confuse you and very much oversimplified: it's the VESC that converts volts into amps, not the motor.
```

---
## \#31 Posted by: devin Posted at: 2016-07-26T16:26:01.453Z Reads: 98

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#32 Posted by: brams Posted at: 2016-07-26T16:26:24.578Z Reads: 92

```
Seriously stop saying confusing stuff like that. VESC does not convert volts into amps. It controls (like any ESC) the 3 phases of the motor. The VESC just warms up at higher current.

Seriously it's not magic, again it's just electricity.
```

---
## \#33 Posted by: Nordle Posted at: 2016-07-26T16:28:03.075Z Reads: 92

```
and it's the esc wich stays cooler as the voltage becomes higher, not the motors
```

---
## \#34 Posted by: devin Posted at: 2016-07-26T16:30:18.404Z Reads: 94

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#35 Posted by: brams Posted at: 2016-07-26T16:35:06.214Z Reads: 100

```
[quote="devin, post:6, topic:6590, full:true"]
heat could be addressed by limiting amps, running motors as close as possible to %85 of no load rpm at full throttle on the flats (this would set your optimal kv based on mechanical load / wind resistance on the flats), air vents, active cooling such as forced air, choice of motor materials (this option affords about %60 of max potential power, but at about the theoretical max [%85] electrical to mechanical conversion efficiency).

to get the most power (and most heat without sacrificing power) from your motors on the flats, you would target kv so you are running at %50 of no load rpm at full throttle on the flats (because of wind drag, etc). (%100 of max potential power, about %50 electrical-to-mechanical conversion efficiency vs %85 max)

running at about %70 no load rpm at full throttle on the flats strikes somewhat of a balance between max power and max electrical-to-mechanical conversion efficiency at full throttle (about %90 of max power vs %100, and about %70 electrical-to-mechanical conversion efficiency vs max %85)
[/quote]

How do you calculate those numbers? Also why 50% of no load rpm would produce 100% of max power?
```

---
## \#36 Posted by: devin Posted at: 2016-07-26T16:39:13.586Z Reads: 96

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#37 Posted by: brams Posted at: 2016-07-26T16:44:26.231Z Reads: 94

```
Have PMDC and BLDC the same performance curve?
```

---
## \#38 Posted by: devin Posted at: 2016-07-26T16:45:27.877Z Reads: 94

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#39 Posted by: devin Posted at: 2016-07-26T16:46:57.270Z Reads: 96

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#40 Posted by: PB1 Posted at: 2016-07-26T16:56:15.648Z Reads: 95

```
@brams of course it does,  in an oversimplified way.  

Input of an ESC is DC voltage and current. Output is AC voltage and current.  And they do not to be the same.  So this is a conversion.  
I can write more later,  in the train commuting right now...
```

---
## \#41 Posted by: devin Posted at: 2016-07-26T16:57:07.750Z Reads: 81

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#42 Posted by: brams Posted at: 2016-07-26T16:57:31.365Z Reads: 84

```
https://evmc2.wordpress.com/2014/12/04/basic-motor-types-pmdc-bldc-ac-induction-and-synchronous-and-series-dc/

PMDC seems to be the word for brushed motors...
```

---
## \#43 Posted by: devin Posted at: 2016-07-26T16:59:10.470Z Reads: 80

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#44 Posted by: brams Posted at: 2016-07-26T17:00:32.794Z Reads: 82

```
True, I do remember now that BL"DC" motors are driven by AC. In that point of view, yes the ESC does "convert" volts to amps.
```

---
## \#45 Posted by: Hummie Posted at: 2016-07-26T17:00:34.495Z Reads: 84

```
The main point of contention: motors will stay cooler with more voltage.  Not true.  I'm sticking with this belief as it's been told by experts and shown in testing by a member on esk8

It's not basic electricity with simply adding cool voltage to get the same wattage
```

---
## \#46 Posted by: brams Posted at: 2016-07-26T17:02:53.815Z Reads: 83

```
True, you don't add "cool" volts since watts are the same.
I think that **what's should be retained** is that **Watts = Heat** and not _Volts = Cool and Amps = Heat_
```

---
## \#47 Posted by: devin Posted at: 2016-07-26T17:04:09.369Z Reads: 84

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#48 Posted by: devin Posted at: 2016-07-26T17:05:42.912Z Reads: 81

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#49 Posted by: Hummie Posted at: 2016-07-26T17:08:37.788Z Reads: 75

```
The motor will get just as hot running on 6s vs 12s for a given load.   If u want to research why and tell me id like to know the details but the fact is there
```

---
## \#50 Posted by: devin Posted at: 2016-07-26T17:12:38.313Z Reads: 80

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#51 Posted by: Hummie Posted at: 2016-07-26T17:22:07.074Z Reads: 81

```
Motors are not high power cables.
```

---
## \#52 Posted by: devin Posted at: 2016-07-26T17:23:53.010Z Reads: 82

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#53 Posted by: Hummie Posted at: 2016-07-26T17:27:31.161Z Reads: 78

```
you're the second person who has told me that this month.  a motor will perform the same with a battery that's 1s or 100s if the kv is adjusted.
```

---
## \#54 Posted by: devin Posted at: 2016-07-26T17:31:09.621Z Reads: 77

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#55 Posted by: Hummie Posted at: 2016-07-26T17:36:59.960Z Reads: 69

```
 Whatever u want to relate it to but the analogy isn't appropriate as motor will get just as hot regardless of what voltage it's run at
```

---
## \#56 Posted by: devin Posted at: 2016-07-26T17:39:25.385Z Reads: 73

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#57 Posted by: Hummie Posted at: 2016-07-26T17:45:04.319Z Reads: 82

```
Did you read the links?  At some point u can't call a motor a high power cable and a higher voltage battery will not a cooler motor make.  Keep the wires going to the vesc cooler and the vesc cooler but that's it.  I don't have an answer how it works but will repeat that statement endlessly.
```

---
## \#58 Posted by: devin Posted at: 2016-07-26T17:47:28.095Z Reads: 83

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#59 Posted by: brams Posted at: 2016-07-26T18:16:27.637Z Reads: 83

```
This thread has been widely hijacked.

Can we move the Current/Heat conversation into another?
```

---
## \#60 Posted by: eblade Posted at: 2016-07-26T18:58:05.991Z Reads: 85

```
Volts are like balls of rocks (that stores energy) in a pipe/tube. Amps are like water that pushes the balls of rocks flowing through the pipe. Higher voltage means more balls of rocks in the same tube means slower/lower/blocked water flow (amps). Lower voltage means less balls of rocks in the same tube means higher/freer/faster water flow (amps). 10 balls at speed x1 = 10W. 20 balls at speed x2 = 20W. 20 balls at speed x1 = 20W. As the balls went through the pipe they release their stored energy (magnetic field). As the balls went through the pipe they collide onto each other and the walls of pipe thus creating friction (heat). Theoratically "Dense/high enough" voltage would have less collision (heat) as the balls would have less space to collide and instead will be forced through the pipe by the amps, with most but not more friction by the walls of the pipe ONLY (reason bold below). They would have less friction as the higher water pressure will cause the velocity among the balls (and not particle) to be equal and small (slower/lower/blocked water) with smaller+equal gaps and higher pressure, moving in one direction. **Pressure along the pipe from one end to another are all equal**. Conclusion; Imagine 100 balls moving along a long pipe with fast, lower pressure water (more prone to collision among balls and walls as the balls move very fast and free with lower pressure and 1 collision will easily cause a chain effect when there is an altered direction) and compare it to **2000 balls with EQUAL GAPS** (due to higher pressure of water, resulting in a more similar density, the faster particles pushing rocks in all direction, as if they are one with the water) **that are moving very slowly and less free to move, in 1 direction along the pipe** (balls don't usually collide with walls if there is no altered direction). **If the balls got stuck** in the pipe (usually smaller pipes/wires or exceeding balls/volts) it will cause the balls to be dragged along the pipe walls thus creating friction (heat). More volts/less amps = tendency for the balls to be stuck. Less volts/more amps = tendency for balls to collide.
**Less heat only applies when you have "dense enough" or "scientifically determined " voltage per given pipe size, striking balance with amps. Over voltage(lower amp) will only cause similar amount of heat as under voltage(higher amp) in the same size of pipe** as per @Hummie  mentioned. **Striking the balance of balls (volts), water (amps) and pipe (wire) is the key**. Higher/lower voltage and amps and wire **only alters the level of heat, and it does not specifically determine that higher volts means lower heat.** So play with the variables.

That's from my understanding guys, please correct me if there's any mistake. Trying to help here.
```

---
## \#61 Posted by: eblade Posted at: 2016-07-26T19:05:09.596Z Reads: 78

```
That is why some people played with thinner/thicker wires or higher/lower voltage etc.
Btw, bigger cable has more space/pipesize to store the balls, thus can have more volts to reach its "dense enough" capacity. Thats why they dont run 100 amps at 1 volts nor 1 amp at 100 volts but at 5 amps at 15 volts assuming that it's efficiency point are at 15 volts per given capacity. (It's just an example).
```

---
## \#62 Posted by: brams Posted at: 2016-07-26T21:19:09.418Z Reads: 76

```
Can we use N52 or 50M to get more torque on the permanent magnets side?

Here is a magnet chart https://www.amazingmagnets.com/magnetgrades.aspx
```

---
## \#63 Posted by: Hummie Posted at: 2016-07-26T21:51:20.145Z Reads: 80

```
stronger magnets will drop the kv with everything else being equal so to bring it back to the same kv you can use less turns of wire around the tooth, so therefore thicker wire with less resistance,  better.  but scorpion motors as an example use low strength magnets with very high heat ability and they have great claims of improved wattage produced.  I wonder how this would go really and utilizing high heat magnets and then being able to have a higher continuous operating temp before the magnets suffer requires having the resistance of the copper go up forty percent from 20c to 120c.  On a small motor, hub motor, copper losses are the biggest lose.  if you want to strike the perfect size motor for the job, no size or weight considerations involved, you eventually have enough copper so that the iron losses will equal or surpass.   So copper losses are everything in a hub motor....except...except..the dreaded magnetic saturation of the stator as it's small and forced to produce huge magnetism.  as it saturates it suffers greater hysterisis, meaning the polarity is slower to flip back and forth as is wanted.  How much copper losses vs iron losses are in a small wheel hub motor I don t  know

I dont know what youre saying exactly eblade and there's lots of different situations but inside the motor alone you can get the same performance, meaning same torque to heat ratio, regardless of what voltage is plugged to the esc.  so i read.
```

---
## \#64 Posted by: devin Posted at: 2016-07-26T22:12:00.641Z Reads: 81

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#65 Posted by: Hummie Posted at: 2016-07-26T22:13:35.231Z Reads: 81

```
to explain it In my own words I'd say you plug it in and then that's when the magic happens.:grinning:

theres a lot in that thread i posted and i cant find the exact words i'd like to pull out.  i'm just leaving it here till someone comes and tells it better.
```

---
## \#66 Posted by: brams Posted at: 2016-07-27T00:54:33.512Z Reads: 80

```
Please stop hijacking this thread about this matter. It's really annoying.
```

---
## \#67 Posted by: PB1 Posted at: 2016-07-27T06:39:02.149Z Reads: 77

```
Sorry @brams for posting again.  I will open a new thread trying to explain why hub motors produce more heat than satellite motors,  so no more hijacking from my side. 

@devin and @Hummie,  is a motor like a power line? Yes and no.  Fact is that the same motor sometimes acts like high voltage / low current power line,  sometimes like a low voltage / high current power line.  
And this is not dependent on the thickness of the wire inside the motor.
```

---
## \#68 Posted by: brams Posted at: 2016-07-27T17:30:16.142Z Reads: 79

```
@Hummie Is a thicker magnet than another with the same grade like N50M is more powerful and then will permet more thicker copper? Like if I double thickness of actual magnets
```

---
## \#69 Posted by: Hummie Posted at: 2016-07-27T17:46:06.443Z Reads: 85

```
add stronger magnets lowers kv so you can then use thicker wire to get it back to the higher kv.  details of how much of this equals that I dont know.  or add a thicker back iron/flux ring.  or hallbach array
```

---
## \#70 Posted by: KMeyerson Posted at: 2016-07-27T18:28:10.291Z Reads: 83

```
I'm gonna hit the pause button right here.

**Thread Subjects:**
*  Smaller Hub Motor Designs and Complications
*  Heat and Wattage (as it pertains to motor design)
*  Magnets and Rotors (as it pertains to motor design)

**Thread Summary:**
Smaller Hub Motors need to be designed to compensate for heat and efficiency problems. Either longer stator for increased torque or windings need to change to reduce current flow for less heat.

A wire has resistance. Passing current through it incurs a force similar to friction, thus generating heat.  By increasing the current while maintaining wire resistance will increase heat. By decreasing the current while maintaining the wire resistance will decrease the heat. The relationship of Watts to volts and amps is key here (but also not everything as theory and reality in design rarely are the same).  You can have two designs where the wattage applied is the same. Theory would suggest that the magnetic field would be operate under reasonably similar conditions to similar results. Theory would also suggest that a motor designed with a stronger volt:amp ratio under no load would operate more cooly as the lower current would encounter less resistance thereby reducing heat.  Logistically, we have to consider motor load which will cause heat to build up in both designs. Based on theory, we should expect less heat from a system running at a higher voltage with a capped current (to match a motor with similarly capped wattage) which also decreased wasted watts.

My personal opinion is that Hummie's motors are constantly at the limits of their design - his thermally tolerant magnets and wires will give you the performance but are be losing precious watts to heat. This is neither optimal or practical for endurance runs where heat buildup is inadvisable (aka 100*F weather).

Before anything is further said on this subject, we need practical evidence and data. I would like @Hummie to hand wire two stators for his motors (for equivalent copper content but with different gauges). Moving his own weight using only one powered wheel test the practical performance of ONE motor under load. Configure the VESC for this motor which we will cap at 1000watts. One system at 6s and the other with 12s both capped amperage for 1000W.  As described above, theoretically the high voltage (12s) system should be cooler when consuming the same amperage when compared to the high current (6s) system. Please report these findings to the appropriate thread (and link results to this thread too).

Finally, Magnets. Flux ring and magnets are important. At a certain point, increasing magnetic fields with stators this size will decrease top speed and increase torque.  Practically it will only increase expense (not by much, btw).  In a hub motor, this might be desired but remains to be tested (see above).
```

---
## \#71 Posted by: Hummie Posted at: 2016-07-27T18:55:28.994Z Reads: 77

```
I can't spell his name but someone here has done this test and posted the results here.  Abit worse efficiency running on 6s instead of 12s.  Running at 12s, if ur going the same speed as 6s, u are forced to be at further from the no-load speed and therefore a bit more inefficient.  He measured amp or watt hours. 

Voltage won't make the motor cooler but increasing the flux in the gap with stronger magnets, smaller airgap, and bigger stator, will allow you to use a thicker wire with less resistance as less turns on the tooth are needed to get required flux.

I do 90kv and if I did 50kv I'm sure they would run cooler but who wants to go 18mph.   
You can design a moto to run a motor efficiently and it will have a high max continuous power and if I did 50kv itd be more efficient but who wants to go 18mph?  it may be more electrically more inefficient but mechanically more efficient.  The difference in watt hours expended I don't know at different speeds and I hope to test and compare with ginra and his gt
```

---
## \#72 Posted by: brams Posted at: 2016-07-27T19:41:49.882Z Reads: 76

```
[quote="Hummie, post:71, topic:6590"]
who wants to go 18mph?
[/quote]

I want ! :grin:

Since it's actually a 22" board, I would like to go between 15mph and 18mph, as it would wobble at higher speed.
I have a 6S battery at 40A continuous made of 18650. The max power W that I can get with these constants PER motor in a dual drive setup is Power = Amps * Volts / 2 = 40 * 3.7 * 6 / 2 = 444W.

With 400W dual drive motors stuffed into 59mm wheels, will it be that much heat?
Active cooling with forced air could also be considered.
```

---
## \#73 Posted by: Hummie Posted at: 2016-07-27T20:14:21.669Z Reads: 75

```
the forced-air cooling designs i had done, three of them,  did little.   Not that it necessarily not be that effective just what I made had minimal sized blades and I've heard of forced-air cooling being effective for hub motors when done right.  

You can have more amps put to the motor than come form the battery.  the sidetrack above is about that.  I dont know much but know on the vesc theres a max amp limit from the battery, and a max amp limit going to the motor.  they are not the same and depending on your speed I believe the voltage is converted to amps in the motor. ...infact maybe it's the only way to make an amps x volts equals watts equation work because a motor, which is an inductor, only responds to amps not watts,  inductance formula is a combo of turns of wire times amps.   I've been on the hunt for what volts do in a motor for a long time.  PB1 is hopefully going to give an understandable breakdown of the magic. 

59mm wheel? what's the motor size?  

Ill get off my ass today, away from the polyurethane fumes, and get the wattmeter out and finally do some wattage to heat outputs.  18mph for me on the 4725 stator I'm riding I could do all day I'm sure.  I do also have good stuff in the motor  but then again there isn't nearly as much copper in the 90kv I have as could be and that's important and the magnets are only n45sh and not n48s as I'll do in the future..

((the temp ability of the magnets and therefore the max temp the motor can get to seems to increase the max continuous wattage producible .  how that plays out I'd like to know exactly as well))
I'll find what wattage it is at those speeds and the temps.
kmeyerson that's a tall order, maybe you'd like to rewind the two I shorted.  it's an awkward rewind with the steel wall close by.  I want to say namasaki is his name..or haimindo, he did a test without the rewind to match the voltage so ran 6s on the same motors and get better efficiency..a little because of being further from the now load while on 12s. not the test as you want.  it's been done though.
```

---
## \#74 Posted by: devin Posted at: 2016-07-27T21:24:35.574Z Reads: 72

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#75 Posted by: PB1 Posted at: 2016-07-28T07:55:36.629Z Reads: 78

```
[quote="devin, post:74, topic:6590"]
_Hummie: You can have more amps put to the motor than come form the battery._

based on my understanding of electricity i disagree that averaged over a whole second you can have more amps into the motor than come from the battery. (because the vesc does not feature a dc to dc transformer to my knowledge).

will someone knowledgeable post an equation or evidence showing whether or not this is possible?
[/quote]

Yes of course it's possible to put more amps into a motor than amps are coming from the battery. 
What needs to stay the same is the power P=U*I, 

Let's say on the battery side we have 37V*20A=740W

Now the voltage on the VESC output side is also 37V, but only in very short bursts, so we have to think average voltage. 
Average voltage will be lower depending on how fast the motor turns. Let's say its 20V.
Then 740W / 20V = 37A will flow through the motor producing torque and a power of 740W. 
All simplified because I'm negeglecting losses here. In real life it would be even more amps due to losses. 

Yes @hummie, I've started writing an article about all of this. I've finished the stuff about the workings of a BLDC motor, now I'm concentrating on the figures and hub motors. It will be a while. 

Now let's hand over this thread to the OP. 

Oh, and @devin, you can't transform DC, you can only transform AC.
```

---
## \#76 Posted by: Maxid Posted at: 2016-07-28T08:09:52.963Z Reads: 72

```
[quote="PB1, post:75, topic:6590, full:true"]
Oh, and @devin, you can't transform DC, you can only transform AC.
[/quote]

What? https://en.wikipedia.org/wiki/Boost_converter
```

---
## \#77 Posted by: PB1 Posted at: 2016-07-28T08:13:47.718Z Reads: 71

```
That's CONVERT and not TRANSFORM!!!

You can convert DC. Never said anything against that. 

But you can only **transform** AC. 

While the end result might be similar, the technique of converting and transforming is very very very different!!!
```

---
## \#78 Posted by: Maxid Posted at: 2016-07-28T08:14:37.892Z Reads: 69

```
that is what he meant and you knew it all along. If he did not use the scientifically correct terminology you could have pointed that out nicely.
```

---
## \#79 Posted by: PB1 Posted at: 2016-07-28T08:18:38.133Z Reads: 71

```
Yes, fully agreeing with you. I knew what he meant. 

I mentioned it because:
1) I wanted to be a smartass :grin:
2) when talking about all of this stuff here we need to be precise. So when I see a mistake like that => see 1)
```

---
## \#80 Posted by: Maxid Posted at: 2016-07-28T08:19:40.872Z Reads: 72

```
instead of going to 1) you should have gone to 
3) tell the correct way and teach your fellow eboarders
```

---
## \#81 Posted by: PB1 Posted at: 2016-07-28T08:27:30.732Z Reads: 72

```
Look, now we have a second smartass. :innocent:

That's why I pointed it out. 
And look here: 
http://www.electric-skateboard.builders/t/how-a-bldc-motor-works-and-why-a-hub-motor-gets-hotter/6753/1
```

---
## \#82 Posted by: brams Posted at: 2016-07-28T12:35:53.159Z Reads: 70

```
@Hummie What are your motors specs with your 4725, max watts, max amps, KV, AWG, Turns, magnets rating and Poles? (You can PM me if you don't want to make that public...)
And then what is the max temperature that you encountered?
It would be so nice to get those informations as I would like to be able to predict what max temp my small hub would be relative to yours at 16-18mph, and also be able to choose the right magnet with the right Curie temp.
```

---
## \#83 Posted by: KMeyerson Posted at: 2016-07-28T15:27:11.673Z Reads: 68

```
Just heads up, you should be careful about using fin powered air cooling.  That is a features claimed and protected by US20140262574A1.  Its pretty ineffective and will just end up breaking or getting caught on something (Rock between the fins and truck could result in a serious accident).

If you send me the shorted stators, I'll rewind them for you for testing (@hummie, PM me). I should be able to do it in my free time in the next few weeks, but I am getting lost in my Oculus Rift every night (I have poor eyesight so Solidworks is better on a virtual 20 foot screen than on my 34" 4K monitor).
```

---
## \#84 Posted by: Hummie Posted at: 2016-07-28T16:00:37.138Z Reads: 70

```
Brams I didn't do the testing yet.  Went to sleep.  I do want o get it done though.  Hopefully today.  Devin above has the wattmeter I want to use and he lives 4 3 blocks away and I like to ride so should be soon. 

I don't have any continuous or peak power numbers but do know the kv, turns, all dimensions.  I forget
What wire size and turns these in using now are but .13ohms resistance I think.  I'll get it all later after I get the results

I think adding a heat sink wouldn't be a bad idea.  I'm not going to do it but the patent can't be simply for a heatsink. I think heat sinks are pretty effective thought
```

---
## \#85 Posted by: KMeyerson Posted at: 2016-07-28T20:23:50.215Z Reads: 71

```
Heat sinks are different enough, yes.  But are they necessary?
```

---
## \#86 Posted by: TheRedPanda Posted at: 2016-07-29T16:15:30.791Z Reads: 71

```
I'd love to see a small eBoard with 4wd with all small motors. It's definitely doable, I'm not sure how much free time you have but I'd absolutely be willing to help design a small motor setup with you if you'd like!

Things to keep in mind:

* Small motors require a small stator, if you want a low kV you'll need it to have as much copper as you can get in there and usually in this case that means you'll be accomplishing that with fairly thin wire. Thin wire doesn't handle high voltage super well so I think your idea of using 6S could definitely work, but I think 8S would end up running them a bit cooler because you don't need to throw as much current at the motor as you would need to with a 6S setup to achieve the same performance.

* The longboard axle is already 8mm, so fitting a stator over that and still accommodating room for the mounting screw will take up a lot of room so you're going to likely need to make the motor fairly wide to make up for what it's lacking in diameter. I don't think it would be too ridiculous though with 4WD because the load is so well distributed. This could potentially be solved by using a permanent mounting solution or making a hard modification to the trucks for mounting with less space needed.

* This 4WD setup will likely more of a cruiser/light commuter setup and not a hill climbing monster.

* To meet the minimum order quantity of custom motors this size will cost somewhere between $2-5k depending on the manufacturer and material selection.


On a side note to chime in on the whole voltage vs current affecting brushless motors it boils down to 
kV * voltage=max rpm. The motor will run most efficiently near it's top rpm, unfortunately this means at the lower end of it's RPM range it's efficiency is pretty low and that turns into heat. The reason why increasing your voltage allows you to run motors cooler is that you can achieve higher rpm using the same current. This is great because you can run motors at a higher voltage and actually decrease the necessary current to have the same performance you would have if you were running lower voltage and higher current. I used to spec out by eBoard to around 70A when I ran 6S(belt driven), and over time found like many others here that increasing my voltage gave me better startup torque and top speed and I could now spec my eBoard to 40A.  

The heat generated from running at higher currents in hub motors is particularly noticeable because there is no gearing(generally) so the motor that usually runs happily at 6S at say 1000rpm is now only running at half or a third the speed it usually would run at in a belt driven setup. So as you accelerate from a stop on a hub motor you are spending significantly more time in the motors "inefficient" low rpm range, because at any given time on a belt system the motor is running 2-3x faster than on a hub so it gets up to it "happy" rpm much quicker. This is aside from the fact that the gearing in a belt system also minimizes the necessary current to get the motor spinning but is also a factor. **edit**: in addition this effect is another reason why unsensored belt driven systems tend to have pretty great braking, when the motor is running at a pretty high rpm even when you're going slow the regen braking is more powerful, you run into an issue with unsensored hub motors that when you are coasting at a low speed and want to brake the motor is essentially reading a zero state with the ESC and can no longer be regen'd, this is why sensors in hubs are really great, you can apply active braking effectively with the addition of sensors and come to a complete stop instead of only having brakes down to 5 or so mph.
```

---
## \#87 Posted by: Hummie Posted at: 2016-07-29T16:28:39.322Z Reads: 62

```
Ive yet to see evidence of higher voltage systems keeping a motor cooler.  someone here did just such a test and the higher voltage system performed worse: at the same speed a higher voltage set-up is further from the no-load speed when at the same speed as the lower voltage system, as you describe as being inefficient.

i can brake down to 2mph without sensors
```

---
## \#88 Posted by: TheRedPanda Posted at: 2016-07-29T16:49:34.538Z Reads: 64

```
Higher voltage isn't always the answer, the best solution is one suited for the particular motor set up. With small motors they tend to not be able to handle higher voltage of 10-12s but also can't handle a lot of current so there's a sweet spot of 6-8S. I forget what the exact size of your motors are but I'd imagine 8-10S is probably ideal. This is where kV is pretty important. The higher your voltage goes the lower your kV needs to be so that the motor doesn't heat up too fast as it's accelerating and taking in massive amounts of power. The main problem you run into when you increase voltage is that heat can build up heat very quickly if the motor can't keep up with the power your putting in. Because Watts = volts x amps, say you are running 40V at 40A = 1600 watts but you then compare that to a system that's 24V at 40A = 960 watts. While technically there is more power available in the higher voltage setup that 1600W means there is a lot more heat that can be generated if the motor isn't running efficiently because watts in the system essentially dictates how much heat can be generated in the system. So if your motor is struggling a bit at startup running the 24V setup at 40A might give it enough time to get spinning before it overheats, 640W less of power makes a huge difference when the bulk of the power is going into heat when you start unsensored. Personally I like 10S for hubs right now as with my setup i haven't had any overheating issues, the 40V 40A figure was purely as an example figure.
```

---
## \#89 Posted by: Hummie Posted at: 2016-07-29T16:56:24.156Z Reads: 62

```
 The voltage a motor can take is only dictated by the magnet wire enamel and the rpm limit of the bearings

Energy in a battery isn't necessarily power in a motor

I read that higher voltage wont increase anything necessarily other than the no-load speed.   You can burn up your stuff just as quickly on 2s system.  Voltage is the force pushing the amps but u can get just as many amps to the motor and just as much performance with any voltage

After lots of looking into this and coming at it assuming more volts equals more power... there is no reason to go to higher voltage unless u want more speed or to keep the esc cooler.  Amps can get there just as fast.  Just as fast acceleration possible with low voltage. More volts is more energy in practice.
```

---
## \#90 Posted by: devin Posted at: 2016-07-29T17:00:07.962Z Reads: 67

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#91 Posted by: TheRedPanda Posted at: 2016-07-29T17:12:10.609Z Reads: 66

```
The magnet wire enamel is insulating the wire from whatever voltage it's rated for but if the magnet wire is heating up quickly this directly affects the efficiency of the whole motor so wire gauge can be really important, while thicker gauge wire technically has a lower resistance than thin gauge wire, there is something called the skin effect which says that the electricity primarily flows on the outside or "skin" of the wire so the inside of the thick wire isn't really doing much. So to a point thin wires actually increase your surface area because you can fit more turns in and pack the stator much tighter. 

My thoughts on the whole higher voltage vs higher current is that it all depends on how you're planning to use the board and what ESC motor and batteries you can get your hands on. Voltage is really just one small part of the whole problem and having a properly setup system is really the goal instead of aiming for a set voltage or current. I agree that if your system is running well at a lower voltage and you're not having any heat problems and you're content with the top speed then you have a great setup for yourself and no need to change that. My points above mainly pertain to increasing the voltage as a means of fixing some part of the system that you're not happy with, usually that is top speed for a lot of folks. This is all aside from the limits of the ESC and how higher voltage can cause significantly higher heat in the esc if not spec'd appropriately.
```

---
## \#92 Posted by: Hummie Posted at: 2016-07-29T17:21:31.210Z Reads: 61

```
Skin effect isn't relevant at these frequencies.

From what I read heat in the esc, at least the vesc, and probably all of them, goes down with voltage not up
```

---
## \#93 Posted by: TheRedPanda Posted at: 2016-07-29T17:43:10.665Z Reads: 63

```
So this is starting to reach the limit of my understanding of motor control but the Miller Effect increases the input capacitance in the gate driver(DRV8302) as the voltage goes up, so even though the current can remain basically the same to flip the gate there is a small increase in the current coming from the driver that when left constantly running like in an eBoard ends up turning into increased heat in the driver. Unfortunately I'm not an expert(not even close) in embedded systems or in circuit design so my knowledge on this is minimal. I think Vedder could probably give a much better answer to the question of increased heat due to higher voltage in the VESC but from what I've read the miller effect seems to be the main cause.

edit: I believe in the Vesc 6.0 vedder switched to the DRV8301(mainly due to the 8302 being phased out), and I think he separated the gate driver to be switching the mosfets indirectly so less power should run through it and make the DRV not so prone to failure.
```

---
## \#94 Posted by: Hummie Posted at: 2016-07-29T18:05:55.989Z Reads: 62

```
from what I remember vedder said the higher the voltage the cooler the vesc will run.   until you get too high of course and then SNAP!
```

---
## \#95 Posted by: Hummie Posted at: 2016-07-30T01:07:15.808Z Reads: 61

```
All these side tracks are fun but small wheel hub motors is the topic.
  I really am excited to get one done long! Same diameter.  Yes!!!  A single.  Only need one and one vesc.   A roller that goes on 10mm axle!  I'm on it if u guys want it.  I'll get it done and charge u all cost plus very small cost for time.   include motor (singular😀)  and 2 tires that are made of epdm high heat rubber.  

If ur into it. 

I am. 

I like the idea of the single sticking out the side asymmetrical.  Fuck symmetry.  Cheaper.  Simpler.  I can imagine not a single reason not to..other than maybe even a 10mm axle would bend or the glue won't hold.  Can easily be tested!! What's the strongest way to connect. 

I've always wanted the simplest cheapest thing.  Maybe I'll change my mind but I really like this idea now.  Not (2) 4725 stators,  but single 4760 or maybe even 4777. Hehe. Hoho.


Chhheeeeeeeep!!  est build possible.
```

---
## \#96 Posted by: brams Posted at: 2016-08-01T18:43:00.558Z Reads: 60

```
Do someone know what the number of teeth of a stator does to a motor specs?
Is more teeth car bring more torque with same number of turns? What about heat?
```

---
## \#97 Posted by: Hummie Posted at: 2016-08-01T18:49:00.849Z Reads: 61

```
I think if I remember it correctly more teeth will allow a smoother very slow movement but u can still only get a certain amount of copper and iron into the same volume regardless if u do a standard 12 tooth vs something else so similar power performance in that regard.  I think the 12x14 that is pretty standard is one of the best combos for power but if u do a multiple of that, say 24x28 it's the same power possible.  12x 14 is not the most efficient but most powerful.  Power is what we all want...to be efficient.

What do u guys think of the motor I'm going to get prototypes made of?  I'm still calling it a small wheel. Small and long. If any of u are interested in getting prototypes of it I'll get them for u at cost.  Get the price in a day or two.   The redundancy of needing two hub motors if they're small is silly.  2x as wide 3x the power and run one motor and esc.
```

---
## \#98 Posted by: bbq870 Posted at: 2016-08-02T15:06:16.415Z Reads: 56

```
I would take 2 motors if you make them.
```

---
## \#99 Posted by: Nordle Posted at: 2016-08-02T15:27:14.875Z Reads: 64

```
Do you know maybe what stator size sk3 6374 is? would like immagine a comparisation with mine.
I hate the tube sticking out on mine^^ but helps cooling and diy options are limited sometimes.
```

---
## \#100 Posted by: devin Posted at: 2016-08-02T15:37:27.378Z Reads: 66

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#101 Posted by: Nordle Posted at: 2016-08-02T15:38:57.027Z Reads: 62

```
Thats the bell not the stator
actually the bell is 59mm diameter even if the motors are named 63xx
```

---
## \#102 Posted by: Hummie Posted at: 2016-08-02T15:40:16.779Z Reads: 62

```
I'm not sure if sk3 does it the same as most but that should have a 74mm long.  But if I remember right it isn't. Can u measure.  It'd be interesting to know how u do with a single. It might be comprable.  Maybe some math with ur bigger diameter wheel and bigger motor matching up with my smaller diameter wheel and smaller diameter motor at 47 instead of your 53

"6374" motor probably has ~5045 stator (-it is 86mm long overall)". And they're 60mm overall as said so the actual stator...I think it's almost always a cm less so a 50mm stator diameter 

So I read

Rather have more motor than fan
```

---
## \#103 Posted by: Nordle Posted at: 2016-08-02T15:48:14.892Z Reads: 57

```
I can measure them the next days, have them in my workshop.
```

---
## \#104 Posted by: brams Posted at: 2016-08-02T23:31:43.749Z Reads: 56

```
To custom motors makers, do you know good magnets suppliers?

Also how do you fix them to the rotor, glue?
```

---
## \#105 Posted by: KMeyerson Posted at: 2016-08-03T01:03:35.901Z Reads: 60

```
For that, I suggest you contact a company that produces rotors.  I know of several Chinese companies, but you're better off NEVER SPEAKING TO THEM UNTIL YOU HAVE A PATENT. Also probably after because they'll ignore your IP rights because they can.

If you find a good one USA side that doesn't charge several thousand, I'd appreciate the info.
```

---
## \#106 Posted by: brams Posted at: 2016-08-03T22:14:38.878Z Reads: 53

```
Thanks for the tips.
I think I will go with [supermagnetman](https://supermagnetman.com) for the prototyping phase. And manufacture different parts in different Chinese companies for full production.
```

---
## \#107 Posted by: brams Posted at: 2016-08-03T22:21:38.584Z Reads: 51

```
@jacobbloy Sorry to bring you to this thread, but seeing your motors makes me wonder what are the advantages of a 21 or 24 slots stator over a standard 12 one?
Also considering the fact that I'm aiming for a 3620 stator for this small hub, to minimise heat, maximise efficiency, get about 400W max P and get 18 mph max (59mm wheels), what are your advices?
```

---
## \#108 Posted by: jacobbloy Posted at: 2016-08-03T22:49:05.633Z Reads: 53

```
I would recommend you will only get a 18slot stator that small and in that size a stator with more slots is going to lower your strand count so increase heat.

It is a fine line before you go big. Smallest stator I would recommend would be 40.6mm

I can help you get a 36mm 18slot 0.2mm lamination or a 39mm 18slot 0.2mm lamination or a 40.6mm 24slot 0.2mm lamination
```

---
## \#109 Posted by: Hummie Posted at: 2016-08-03T22:57:37.365Z Reads: 58

```
are you going to wind them yourself?  getting stators is harder and more costly than getting motors made.  
do you have any pics? 
3620 is tiny.  with one motor you will burst into smoke.  You could do the 59mm wheel if you make it really long. 

i think a 24 slot vs a 12 is almost the same power as its the same amount of copper and iron but i think it is less prone to cogging at really slow speed.  12x14 or a multiple is a pretty magical number for power I think.  not necessarily efficiency but power.  I vaguely remember something about it.  

for such a small wheel you could do an inrunner for the skate hanger.  it would spin the axle and have one wheel fixed and the other on bearings and floating on the spinning axle.  there's a lot more potential motor room in a fat hanger than in a 3620.  you could have your small wheel and with some decent power.  one motor no redundancy.  swappable wheels.  similar to the lagrange drive system with it's floating axle. always wanted to make that.   the torque out of an inrunner isn't as good as outrunner but if you make it long enough you could get there.  definately better than that little stator.  and then your tires will run cool!  not complications there.  real regular wheels.
```

---
## \#110 Posted by: KMeyerson Posted at: 2016-08-04T04:19:23.076Z Reads: 55

```
I don't advise inrunners. Not enough torque. Look at Stary - they struggle to climb intense hills and you can REALLY hear that gear set churning.

@brams Does supermagnetman also make rotors?
```

---
## \#111 Posted by: brams Posted at: 2016-08-04T12:22:10.582Z Reads: 52

```
@Hummie Yes, for me I don't think inrunner is a good option, I can't have a long stator.

@KMeyerson I don't think supermagnetman is selling any rotors, it's really a magnet specialist.

Also, what should be used for fixing magnets to the rotors? Epoxy?
```

---
## \#112 Posted by: Nordle Posted at: 2016-08-04T12:27:36.283Z Reads: 54

```
i want have [this gearing](https://www.youtube.com/watch?v=EAELukfr2oY)!
```

---
## \#113 Posted by: KMeyerson Posted at: 2016-08-04T13:18:59.750Z Reads: 55

```
Def epoxy.  You can design a clip mechanism that locks the magnets in position around the rotor, but it won't replace epoxy.
```

---
## \#114 Posted by: Hummie Posted at: 2016-08-04T15:21:39.488Z Reads: 53

```
stary dont use an inrunner it's a little outrunner with a planetary gear.

brams if you try to use the little stator you mentioned it will be super under-powered.  U will not have a max speed on a flat of more than maybe 5 mph and that's if you were to push it to speed.  Thats a guess but...way under powered and all the problems associated with that.
```

---
## \#115 Posted by: KMeyerson Posted at: 2016-08-04T16:49:17.672Z Reads: 50

```
Oh good catch. The rotor is actually not connected the way I thought it was.
```

---
