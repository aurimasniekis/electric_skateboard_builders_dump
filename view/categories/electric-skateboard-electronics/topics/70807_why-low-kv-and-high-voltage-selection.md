# Why low KV and high voltage selection?

### Replies: 57 Views: 1514

## \#1 Posted by: olestra Posted at: 2018-10-10T19:36:24.505Z Reads: 260

```
Since my thinking is so far away from what everyone is doing -- I'd rather ask and be wrong rather than spend a grand before finding out that I was...
I've been poking around and it seems that all the boards use quite low KV motors <300 and quite high voltages, 8-12S.
What's the logic behind this -- in particular- since electric motors have a fairly flat torque curve (particularly compared to IC engine) wouldn't a  1000-1500KV motor running at 2-4S voltages allow for a much wider selection of motors and ESCs?
I know you would draw more amps from the inescapable P=IV, but unless you're dealing with really crap batteries 30-40C will give all the amps needed -- unless my math is wrong (40C * 10amp * 14.8volts gets around 6kw to play with)

so TLDR; why not use higher KV motors with lower voltage systems to achieve performance with more selection of parts?
```

---
## \#2 Posted by: 12meterkuk Posted at: 2018-10-10T19:39:54.873Z Reads: 250

```
It’s simple, more amps = more heat
```

---
## \#3 Posted by: Pedrodemio Posted at: 2018-10-10T19:49:43.612Z Reads: 248

```
The problem of the current is not only on the batteries, every part of the system is subject to I^2R loses, só going lower voltage increases the heat produced to the square to keep the same power, also to handle more current you would need more MOSFET’s in parallel, that will add cost and also more heat dissipated inside the enclosure
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-10T19:56:53.475Z Reads: 241

```
Most of the vescs on the market can handle around 50a before they start heating up.
Sure you can create a heatsink housing like the one from @Kug3lis which would allow you to get more amps out but even than I think with 90amps you on the limit.
90*14,8=1332w ... far away from the 6k😉
```

---
## \#5 Posted by: olestra Posted at: 2018-10-10T20:09:20.536Z Reads: 228

```
I'm seeing 160a 4s ESC for around 60$ --- seems like I could get 2 of those for less than the cost of vesc and spend the leftovers on an aluminum enclosure for the motor controller to handle the heat.

that was an additional question, I suppose - why the fixation on vesc? - I get that it's a nice bldc esc, I'll probably pick some up for a couple of robotics projects come spring.
Is the vesc considered so far superior for e-skateboard applications that little else gets considered?

not arguing or trolling-- I'd like to understand the cause of common design decisions that I've been seeing.

so far, heat.
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-10-10T20:12:39.183Z Reads: 212

```
One thing you missing is that current = torque. Those high kv motors don't have that much torque and just spins fast, to achieve same torque you would need to spin in its effective voltages and the apply aggressive 1:100 gear ratios to decrease RPM to suitable for esk8. Then you also need ESC which would be able to spin motor at these kinda high ERPMs I am talking >300-500k

So in the end its not worth it. Plus you cant use those high kv motors with low voltage they will not even start spinning.

![image|690x300](upload://qTlnStvLyTVQqp7eD3HN284HTQ7.jpeg) 


Any other ESC not made for esk8 will have brakes so hard that every time you just push it sligtly you will fly forward also it misses all goodies and etc ;)
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-10T20:17:31.307Z Reads: 198

```
No for sure you not fixed on a vesc.
But at the moment I think there is no other esc which gives you all this oportunitys to fine tune all the settings you want to get in place for a nice smooth ride. You can adjust your brake forces, you amp limits your throttle curves etc. etc.
I‘m not into all this car esc so i can’t say anything about it. The hobbywing max6 seems to be a good one thou.
```

---
## \#8 Posted by: olestra Posted at: 2018-10-10T20:22:03.320Z Reads: 191

```
Interesting -- one reply I'm getting RC ESCs have too strong of brakes, and the other is saying way too weak.

I totally get that the vesc is _really_ configurable. most RC ESCs give about 5 settings for brake strength.
```

---
## \#9 Posted by: PatRocks Posted at: 2018-10-10T20:22:23.956Z Reads: 194

```
It's important to think about wattage when thinking about "horsepower". @Kug3lis couldn't have said it better, rpms are a limitation as well as amp throughput. But don't be discouraged, @MoeStooge runs high kv motors, and he slays like it's his job.
```

---
## \#10 Posted by: Hummie Posted at: 2018-10-10T20:22:42.277Z Reads: 186

```

1s battery, 2200kv motor, esc that can do 1200 amps, a voltage potential across the motor enough to supply the needed amps for the equivalent torque as 12s n 200kv n 100amps from a capable esc (can u get that current across the motor ...will you have the voltage potential and is it just ohms law at the motor or is the rest of the system needed to be incorporated)

Such a setup would be a huge esc. Huge battery. But regular motor n gearing.
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-10-10T20:25:19.110Z Reads: 170

```
Well I think @MoeStooge runs something in 800kv at 30V range so it is not bad compared to 2000kv :D
```

---
## \#12 Posted by: olestra Posted at: 2018-10-10T20:32:28.472Z Reads: 166

```
So far:
It's looking like heat is a common concern with higher amp/lower voltage.

braking may or may not be a concern.

RPMs could be problematic.

any other reasons? 
and thank you all for the information so far!
```

---
## \#13 Posted by: Pedrodemio Posted at: 2018-10-10T20:34:15.841Z Reads: 166

```
Another thing, try loading these 60 usd 160a esc for more than a few seconds and see what happens, or they will heat up a lot and shutdown or you have a nice firework at your feet

In the beginning when vesc was just starting a lot of people used car/boat esc’s and there was a resistance to switching, but look now, only a few people go for them

What is better? It’s smooth, it’s predictable, all that because it’s made for what we are using it for, others esc was never made to propel a 100kg piece of meat uphill 

I really recommend you to read the VESC thread at endles sphere

(Keep in mind that the video is just an example, the esc used is not a cheap one)

https://youtu.be/JwDwEHQCk5g
```

---
## \#14 Posted by: Hummie Posted at: 2018-10-10T20:39:44.804Z Reads: 153

```
1s battery, 2200kv motor, and an esc that can do 1200 amps,?

 can u get that current across the motor …will you have the voltage potential and is it just ohms law at the motor or is the rest of the system needed to be incorporated). If so could get same performance I think 

Such a setup would be a huge esc. Huge battery. But regular motor n gearing.
```

---
## \#15 Posted by: olestra Posted at: 2018-10-10T20:41:17.597Z Reads: 148

```
nice @Pedrodemio!
I suspect leaving the cooling fan open to debris when kicking up gravel had more to do with that failure than anything else -- but I'll start my reading!
Makes one consider the water cooled motors and ESCs for boats (easy to water-proof:grinning:)
```

---
## \#16 Posted by: olestra Posted at: 2018-10-10T20:43:49.816Z Reads: 140

```
the battery would be exactly the same size 12s vs 12p, btw
```

---
## \#17 Posted by: Hummie Posted at: 2018-10-10T20:44:42.223Z Reads: 134

```
True. Yea.
```

---
## \#18 Posted by: Pedrodemio Posted at: 2018-10-10T20:47:05.801Z Reads: 133

```
Yeah, that could have part, I don't remenver if @Nowind said anything

I think that any losses are energy that could make you ride farther, it's the same think with electric cars that some manufactures didn't realize yet, the cheapest way to increase the range is to lower the drag and rolling loses, not increase battery capacity
```

---
## \#19 Posted by: b264 Posted at: 2018-10-10T22:05:35.026Z Reads: 135

```
[quote="Kug3lis, post:6, topic:70807"]
Any other ESC not made for esk8 will have brakes so hard that every time you just push it sligtly you will fly forward
[/quote]

This :arrow_up:.  Don't use an ESC not specifically designed for esk8.  You can use an esk8 ESC on anything else, though...

Most of the value of VESC comes from the free and open-source software and not so much the hardware...
```

---
## \#20 Posted by: MoeStooge Posted at: 2018-10-10T22:25:41.345Z Reads: 136

```
Amps does not build heat. Resistance builds heat.
```

---
## \#21 Posted by: Namasaki Posted at: 2018-10-10T22:51:18.735Z Reads: 132

```
[quote="olestra, post:8, topic:70807, full:true"]
Interesting – one reply I’m getting RC ESCs have too strong of brakes, and the other is saying way too weak.

I totally get that the vesc is *really* configurable. most RC ESCs give about 5 settings for brake strength.
[/quote]


I started with 120a car ESC's. Vesc's where just starting to hit the scene then.
I had a program card and tried various settings. The problem is that no matter what setting I chose for the brakes, they where still rough and unpredictable.
If I was coasting down a steep hill and tried to apply the brakes, I would push the trigger 1/2-3/4 out before the brakes would respond and then they would grab hard.
The only way to make them work right was to first accelerate and then apply the brakes.  I was already going too fast and the last thing I wanted to do was accelerate!
Acceleration is also not very smooth but jerky and hard to control.
When the Vesc came out, it changed everything. Smooth predictable acceleration and braking.
```

---
## \#22 Posted by: Trillium Posted at: 2018-10-11T00:07:39.002Z Reads: 118

```
I've been working on a 1S skateboard drivetrain. The intent is to get the heat generation outside of the motor where it is easier to cool things. Also would eliminate need for BMS other than temp sensing on the battery and simplify things to a single pouch or prismatic cell. There are some efficiency gains as well but it's a bit tricky to actually make those gains feasible. It's really hard to get a lot of copper in a motor of smaller diameter as the one I'm making. The continuous current is much higher around 30A RMS on 1S if doing around 125W per motor. If your wires aren't pretty big, you've got some problems.

If anyone is interested in learning about my motor, I was thinking of doing a little reveal. I have been working on it a long time and need the support of a forum I think. Preorders would be nice if enough people become passionate, but it's been hard for 1 person to handle so you'd have to respect my time trying to get stuff to you.
```

---
## \#23 Posted by: Jmding Posted at: 2018-10-11T00:14:49.250Z Reads: 108

```
1) We all want power
2) Power = voltage * current
3) Current is limited to a max of 75 amps per motor for 6374 200 Kv motors, the most powerful motors that are commonly used.  Other motors have lower current capabilities, often significantly lower.  Sure you can pick a higher current ESC than the 60A VESC that is popular, but it wont really matter because you'll start melting your motor
4) So the only way to get more power is to increase the voltage

QED
```

---
## \#24 Posted by: Trillium Posted at: 2018-10-11T00:30:15.791Z Reads: 101

```
I'm designing for about 200ARMS battery current per motor. or about 700W input power. Hopefully around 400W peak output power per motor.
```

---
## \#25 Posted by: Jmding Posted at: 2018-10-11T00:53:39.281Z Reads: 100

```
200 amps sounds HUGE, but it sounds plausible given you are using unconventionally low number of turns with crazy thick magnet-wire.  I'm really curious what you're up to from an academic standpoint, but as of yet it doesnt sound too compelling vs conventional designs, given that you're targetting 400W peak output which is frankly pretty low (except when compared to hub motors).  Sure the BMS simplicity has some value, but I figure that's pretty much irrelevant in the face of the fact that I've never seen a 50 A*h 1s battery for sale.  I'm skeptical, but eager to be proven wrong I guess.
```

---
## \#26 Posted by: Trillium Posted at: 2018-10-11T01:08:41.724Z Reads: 100

```
It's about in line with boosted boards output power if I'm not mistaken... certainly a good benchmark to meet.

I have a sheet I made that compares 7S to my 1S I should share. I never made a 1S motor, but I have most of the materials. I only made a 7S motor before using conventional magnet wire.

If you do the math, you'll find that it is possible to get higher efficiency in the motor iteself from a low voltage system simply because it becomes easier to fit more copper in the motor when going to a 1 turn design. However, to get overall better efficiency, the resistance in the phase leads also needs to be scaled up as well, which is the most annoying part.
```

---
## \#27 Posted by: lrdesigns Posted at: 2018-10-11T01:08:42.625Z Reads: 93

```
Gearing is the main reason I use low kv motors. 

If you use belts, and wheels 97mm or smaller you have a limit on the smallest motor pulley and largest wheel pulley you can use.  On the motor side you cant go below 15t or they wear out too fast and skip more. With a low kv motor you can run a 20t motor pulley, because more teeth engagement they never slip, the pulley and belts last much longer.  If the wheel pulley is too larger the belt is close too the ground and gets munched by rocks.

Im on 12s dual and my vesc battery amps only 15amps (30 total) and I still get good performance. Everything stays cool. I personally wouldn't want to subject my batteries to more than 50 amps. 

My motor amps are at 65a which gives good low speed acceleration / hill climbing. It is only lacking a little mid speed acceleration but its enough for my needs.
```

---
## \#28 Posted by: Jmding Posted at: 2018-10-11T01:31:39.982Z Reads: 84

```
[quote="Trillium, post:26, topic:70807"]
that compares 7S to my 1S I should share. I never made a 1S motor, but I have most of the materials. I only made a 7S motor before using conventional magnet wire.

If you do the math, you’ll find that it is possible to get higher efficiency in the motor iteself from a low voltage system simply because it becomes easier to fit more copper in the motor when going to a 1 turn design. However, to get overall better efficiency, the resistance in the phase leads also needs to be scaled up as well, which is the most annoying part.
[/quote]

hah! That's awesome and hilarious!  Are you saying if you do a single, rectangular wire, you can basically fill 100% of the available volume with copper, but with conventional designs you are subject to hexagonal close-packing issues?  I get that, but I dont think you can actually pull off a rectangular wire...  Also yes, the phase wire is going to look RIDICULOUS.  I just dont see how this will work lol

I agree with the idea of using the Boosted as a benchmark.  Their batteries are capable of 50 amps according to the A123 specsheets, so the max power is 50 amps * 12 * 3.3V = 2 kW.  Unless you go 4WD with your system, its just not there.
```

---
## \#29 Posted by: Hummie Posted at: 2018-10-11T01:39:49.162Z Reads: 84

```
wouldn't the esc be huge?


the motor amps would need to be huge for equivalent performance against something more typical with a lower kv.  1000 amps ...I think you should do it direct drvie not a hub motor so you can make the motor leads stationary.   and also might as well make it a heatsink as if you hadn't thought of such an idea.  that would be pretty awesome if the trucks were both completely mechanical and giant functional wires.  with a bit of insulation between them.   how many teeth and magnets?
```

---
## \#30 Posted by: 12meterkuk Posted at: 2018-10-11T01:58:05.094Z Reads: 86

```
It’s given that there is a set amount of resistance, so naturally more amps = more heat produced. But Of course resistance is the cause of the heat.
```

---
## \#31 Posted by: MoeStooge Posted at: 2018-10-11T02:00:07.365Z Reads: 88

```
Any kv any volt as long as you have the watt capability to handle the load-and an adequate delivery system with proper mechanical setup. Low pole motors are more efficient due to copper/iron ratio and make more watts per cc, so naturally more power smaller package.  Bargain esc's are a mistake and you would be better off burning your hard earned cash.  Get a high end esc with the expectation to run it at 60% of it's capability. High end esc's have powerful fully tunable brakes you can customize progressive rates, bomb down hills at 40+mph with confidence and not worry about hitting E-rpm limits.  Figure out what you want your skate to do, overbuild it and de-tune it.  Overloaded conductors and mechanical loss builds heat. Heat is the enemy of all electronics.
```

---
## \#32 Posted by: MoeStooge Posted at: 2018-10-11T02:03:32.366Z Reads: 81

```
[quote="12meterkuk, post:30, topic:70807"]
It’s given that there is a set amount of resistance, s
[/quote]

I guess I missed the part where there is a set amount of resistance, please explain.
```

---
## \#33 Posted by: 12meterkuk Posted at: 2018-10-11T02:14:00.918Z Reads: 80

```
There’s x amount of resistance in every build no? Of course it’s different with every board but I’m just trying to explain it simply to him.

Amp flow is variable in an esk8 system while er is normally not(maybe when temps get too high). So it’s not untrue that more amps create more heat with the same resistance. Also not untrue that more resistance creates more heat with same amp flow. 

Not trying to start a discussion here, just trying to make it as simple as possible for him to understand.
```

---
## \#34 Posted by: Pedrodemio Posted at: 2018-10-11T02:29:43.733Z Reads: 79

```
I suggest reading these for everyone interested in the discussion 

http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
## \#35 Posted by: Trillium Posted at: 2018-10-11T04:52:11.878Z Reads: 74

```
Yeah, this is a good idea to try to use mechanical components as current carriers, but the issue is keeping them isolated. So the next best thing is to run copper along the aluminum truck hangar, which is what I was intending on trying.
```

---
## \#36 Posted by: MoeStooge Posted at: 2018-10-11T12:22:09.591Z Reads: 69

```
The only time you should be worried about heat is if your build dosent have a system properly capable of delivering the demand. Resistance is not a "given" it's a choice you make when you buy and build.
```

---
## \#37 Posted by: professor_shartsis Posted at: 2018-10-11T15:54:33.342Z Reads: 60

```
[quote="olestra, post:1, topic:70807"]
why not use higher KV motors with lower voltage systems to achieve performance with more selection of parts?
[/quote]

here is a comparison of a set of dual hummie V4 hubs w/ 12S (46v) & 100a/60a motor/battery limits **vs** a dual 1500kv 4S (16v) system that obtains similar top speed, acceleration & heating...

https://image.ibb.co/jo4M9U/1500kv_vs_hummie_v4.gif

findings:

in order for the 1500kv 4S system to obtain similar performance to a set of hummie v4 hubs, the system requires:

- 0.007 ohm windings (1/10th as much electrical resistance)
- 6.4:1 gear ratio (64 wheel teeth & 10 motor teeth)
- 320a motor current limit
- 172.5a battery current limit per motor (345a total system peak battery current)
- 84mm tires (same size)
- 24000 peak motor rpm (vs 3358rpm hummie v4)
```

---
## \#38 Posted by: olestra Posted at: 2018-10-11T16:52:30.939Z Reads: 58

```
I'm quite impressed with the amount of discussion my little question has started, thank y'all for being significantly less full of jerks than most of the fora I frequent.

My take-away so far:
High voltage and low kv seems to be a sweet spot for the standard size wheels(83->90mm), motors(<=65MM dia) and gearing used, allowing for a wide range of speeds without hitting a frequency limit for switching fields.
_My focus is larger wheels(120->200MM and a max speed of 25mph. I'd like it to be able to lift a 280# fellow up a wall if needed. Seems like the the 1/8th scale rc motors would satisfy what I'm thinking about_

The reasoning for the VESC vs RC ESCs is laggy response to input and inadquate brake tuning (too strong or too weak) 
_Has anyone considered that the laggy response could have been upsteam in the system (transmitter/receiver) rather than ESC?_
```

---
## \#39 Posted by: olestra Posted at: 2018-10-11T16:53:53.730Z Reads: 56

```
can you punch the numbers for 120mm wheels on those charts? It would be much appreciated!
```

---
## \#40 Posted by: professor_shartsis Posted at: 2018-10-11T17:19:24.743Z Reads: 55

```
120mm / 84mm = 1.42

1.42 * 6.4 ratio = 9.08:1 ratio
```

---
## \#41 Posted by: Hummie Posted at: 2018-10-11T17:34:29.897Z Reads: 51

```
@olestra. In USA olestra is a fat substitute that causes “anal leakage”!!  I remember back when they were doing tv ads For chips with it and have to say “may cause anal leakage”. Really fast.
```

---
## \#42 Posted by: olestra Posted at: 2018-10-11T17:49:44.589Z Reads: 49

```
@Hummie  bingo! I picked out the name 15 years ago for an undead warlock in WoW as I thought it was appropriately gross, having experienced the phenomena myself from a bag of chips, cooked in olestra. Disturbingly nasty, lasted for 3 days.
```

---
## \#43 Posted by: professor_shartsis Posted at: 2018-10-11T17:50:34.034Z Reads: 50

```
what esc do you plan to use to supply the 320a motor current? battery pack & wires rated to 345a?
```

---
## \#44 Posted by: Hummie Posted at: 2018-10-11T17:53:54.661Z Reads: 49

```
320a for a one cell vehicle 
 I’d thought more like 900a motor current needed w high kv motor needed to be similar n get to similar speed n torque as typical
```

---
## \#45 Posted by: professor_shartsis Posted at: 2018-10-11T17:54:41.310Z Reads: 50

```
[quote="Hummie, post:44, topic:70807"]
320a for a one cell vehicle
[/quote]

the 320a motor current was for 4 cells in series (16v)
```

---
## \#46 Posted by: professor_shartsis Posted at: 2018-10-11T18:09:53.987Z Reads: 52

```
one cell dual hub motor:

one cell 4v battery, dual 900kv hubs w/ 0.0005ohm & 84mm tires, 1250a motor current limit, 690a battery current limit per motor (1380a battery combined):

https://image.ibb.co/m4OvKU/1cell.jpg

https://www.batteryspace.com/productimages/lifepo/5907.jpg

https://www.batteryspace.com/lifepo4-prismatic-module-3-2v-100ah-10c-rate-320wh-un38-3-passed-dgr.aspx?gclid=eaiaiqobchmiuvo_ood_3qivgksnch3yfay-eakyasabegklfvd_bwe
```

---
## \#47 Posted by: olestra Posted at: 2018-10-11T18:12:37.884Z Reads: 52

```
very preliminary, I'm considering 4x https://hobbyking.com/en_us/turnigy-1-8th-scale-4-pole-brushless-motor-1900kv.html
yielding an approximate max wattage of 8kw @4s battery

As for wires,esc and battery:
There's a quite a few ESCs -- I'll be looking into the lag of responsiveness and braking levels of what's out there. I'm feeling like the transmitter/receiver stack might be a significant factor -- it blows my mind how cheap some of these are -- quality has to be suffering there -- the rock-crawler RC guys might have some good data.

My batteries are going to be lipoly packs (one per 2 motors) taken from a city bus 4s2p should work.

Wiring seems like 8ga will be sufficient, I'll look up some charts as I get further along
```

---
## \#48 Posted by: Jmding Posted at: 2018-10-11T18:49:50.462Z Reads: 49

```
the body of knowledge on RC ESCs around here is probably starting to dwindle as VESC has come to dominate so much.  It wouldnt be all too surprisng to me if lag is not a significant issue in most cases, a few people just had some bad experiences and those stories are being parroted.  My own experience with an FVT ESC several years ago was that there was no lag at all.

That said, RC ESCs still have a major disadvantage in that they have no current limiting, so be careful, they will easily burn themselves or your motors up in high-torque situations.  That's what happened to my FVT ESC years ago, it burned up, and so I decided to give up on the whole DIY ESK8 thing until better ESCs became available.

Really curious, and really confused about this 4s build.  Those motors are only 70A @5s, whereas 6374's are about 70A @12s, so they're about half as powerful.  With 4s2p, you could easily reconfigure that to 8s1p and run a more conventional setup.  The only big advantage that I can think of is that it allows you to use $40 RC ESCs that are limited to <6s instead of VESC, but you need to go 4WD to get the same power as a 2WD 6374 setup, which means you need 4 ESCs, which puts the price of the electronics very much in line with going with VESCs anyway.  Are you going this direction because in-runners = protection from the elements?
```

---
## \#49 Posted by: olestra Posted at: 2018-10-11T19:02:32.136Z Reads: 50

```
@Jmding crap, misread spec. thought I was looking at 120amp nominal. **time to look for different ones**
I'm thinking 4wd because loose sand and gravel has ruined my day on many different vehicles. I'm not looking to be completely cheap, just the cost of 4x vesc makes me shudder a little.
I currently have a monster with go-cart wheels -- got it off craigslist for 200$, it had lead-acid batteries(fixed that!) and currently has some unknown receiver and _brushed_ esc and motor.
I like it's size and feel, but think I can do it better/right.
 ![00u0u_5HrN3KcrBJ2_600x450|600x450](upload://zuPVXb9nktvMPxHHH5doVQIT723.jpeg) ![20180902_104808|666x500](upload://2WByUc3zTr01CF5iE83bPA5LQ8Z.jpeg)
```

---
## \#50 Posted by: professor_shartsis Posted at: 2018-10-11T19:09:09.767Z Reads: 50

```
[quote="olestra, post:47, topic:70807"]
very preliminary, I’m considering 4x [https://hobbyking.com/en_us/turnigy-1-8th-scale-4-pole-brushless-motor-1900kv.html ](https://hobbyking.com/en_us/turnigy-1-8th-scale-4-pole-brushless-motor-1900kv.html)
yielding an approximate max wattage of 8kw @4s battery
[/quote]

doesn't look too bad with the 4x 1900kv, 0.0074ohm, 16v (4S) & 120mm tires geared for 25mph top speed w/ 100a motor/battery limits... plenty of torque for 31.5% grade... only 100a motor current per motor required for nearly 120lbs thrust... 15:1 gearing sounds like a challenge. nearly 400a battery amps required for accelerating up 31.5% slope while passing through 25mph w/ 120lbs thrust. ~80w ohmic heating per motor seems fairly low for 120lbs total thrust.

https://image.ibb.co/fhnpw9/1900kv-4s.jpg
```

---
## \#51 Posted by: olestra Posted at: 2018-10-11T19:40:59.371Z Reads: 45

```
@professor_shartsis thank you much, sir!

that gearing is problematic... and larger tires don't help that at all
```

---
## \#52 Posted by: Jmding Posted at: 2018-10-11T19:53:32.858Z Reads: 49

```
You can get inexpensive Chinese VESCs on TaoBao for <$60, which even x4 is probably only a $50 upgrade vs the dirt cheap RC ESCs.

https://item.taobao.com/item.htm?id=573731236190&ns=1&abbucket=9#detail

400a battery current!!! Even with these insane 65C "Graphene" lipos, you'd need two in parallel to get that output...  XT90's desolder at 300A!

https://www.youtube.com/watch?v=4rcCdCVBXAI
```

---
## \#53 Posted by: Jmding Posted at: 2018-10-11T19:55:11.395Z Reads: 49

```
Hell, 10 AWG wire starts smoking at 270A...  This is getting nuts!

https://www.youtube.com/watch?v=IDnPX6QPbu4
```

---
## \#54 Posted by: olestra Posted at: 2018-10-11T20:22:23.665Z Reads: 52

```
@Jmding good points, I'll need to watch the limits since I'm looking at a max of 240amp per battery pack
```

---
## \#55 Posted by: thiswasandy Posted at: 2018-10-11T22:14:30.047Z Reads: 53

```
This thing looks amazing, lol.

I think there’s a thread where someone was looking into making their own Onewheel using go kart tires and they stumbled across some hubmotors that work with them.  Not sure what kind of speed you’d be able to achieve and the thermals would probably be insane.

Edit: https://www.electric-skateboard.builders/t/onewheel-skateboard/15901

At the end of the thread they’re discussing the motors.
```

---
## \#56 Posted by: thiswasandy Posted at: 2018-10-11T22:21:00.382Z Reads: 53

```
Lots of fun motors here too, lol.

https://www.peipeiscooter.com/dc-hub-motor.html?p=2&product_list_dir=desc&product_list_order=price
```

---
## \#57 Posted by: olestra Posted at: 2018-10-11T22:36:47.797Z Reads: 50

```
@thiswasandy looks very cool -- for this application, I'm planning on staying away from hubmotors. though.
When I inevitably catch a stop sign or park bench and go superman... I'd rather deal with only a bent axle on a truck than a bent axle on a motor. well, that and whatever bones I brake :bone:
```

---
