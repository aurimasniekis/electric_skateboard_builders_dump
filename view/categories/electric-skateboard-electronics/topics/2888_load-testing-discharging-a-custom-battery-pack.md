# Load testing/discharging a custom battery pack

### Replies: 37 Views: 3140

## \#1 Posted by: longhairedboy Posted at: 2016-05-04T18:38:04.468Z Reads: 193

```
years and years ago in what seems like a whole other lifetime, i worked for a tech firm that made some of the most reliable and awesome remote power and data management equipment for data centers. They made these smart power switches that you could telnet into or make serial connections to and tell them to turn outlets on and off and read power draw from servers and other cool shit like that.

They had what they called HiPots to test them with (that's a brand name for other test equipment too, so they were treating it like a generic term), and they were basically just giant aluminum racks of resistors hanging over the workstations. They would use them to load test the power strips we built. 

I want something like that or maybe something better or more appropriate for discharging and load testing these packs i build. Running them down with motors on the bench is going to take forever and i'd like to have a way of testing them before i put them in a board and ride with them. 

Is there something i could make myself out of a clever arrangement of resistors that wouldn't burn my house down but would adequately drain the pack within a reasonable amount of time and let me test things like the BMS's low voltage cutoff and shit like that?
```

---
## \#2 Posted by: Karmannghiagirl Posted at: 2016-05-04T18:43:45.029Z Reads: 191

```
use some lightbulbs? or get some massive capacitors, use the batteries to charge them, and then use them to charge the batteries?
```

---
## \#3 Posted by: makepeace Posted at: 2016-05-04T18:49:40.315Z Reads: 189

```
R = V / I, my friend. And P = I^2 R. Choose your pack voltage and your discharge current (based on your limits there, and also the time you want to discharge over), calculate your resistor value, calculate the power rating for it, stick a voltmeter across your battery and away you go. You can parallel resistors to increase their power rating, but just make sure you work out the values you need to get your required series resistance.

To elaborate, say you have a 10s 10Ah pack thst does 20 C continuous. I = 200 A, V(max) = 42 V. Therefore R = 0.21 ohms. Power rating is P = 8.4 kW. Get 1000 10 W 220 Ohm resistors and stick them in parallel and you'll have a 10 kW  0.22 Ohm resistor. Oh, and your battery will drain in 10 / 200 x 1hr = 3 minutes. That is fast. 

Probably too fast, so maybe go with something more.conservative. I'd use half of the max continuous discharge rating as your guide, and make sure the resistor setup is very safe so that you don't burn anything down/get electrocuted.

This is also bound to be expensive.
```

---
## \#4 Posted by: Blasto Posted at: 2016-05-04T18:54:13.206Z Reads: 159

```
You want an electronic load, but they aren't cheap (N3300). You can make shift jig with a bunch of power resistors.

http://www.ebay.com/itm/2pc-8ohm-8R-500W-Watt-Power-Metal-resistor-for-tube-amp-test-dummy-Load-/191572833675?hash=item2c9aa1758b:g:MjkAAOSwPhdVR3kP

slap these bad boys in parallel, it's a safe way of draining 10Amps

2pcs in parallel is: 8//8 = 4 ohm

42V (worst case)/4ohm = 10.2Amps

10.2Amps * 42V = 441W

you will safely operate under the 1000W of capacity of this jig.

or 

get 2 of these

http://www.ebay.com/itm/500W-4-Ohm-Solder-Lug-Terminals-Aluminium-Housing-Braking-Resistor-Resistance-/322067356979?hash=item4afcb5dd33:g:WHAAAOSwGYVXB53t

you will drain 20A if you put them in parallel
10A if you use just one
5A if you put them in series.
and you would be running in all cases under the max 1000W
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-05-04T18:54:15.164Z Reads: 148

```
electrical math like this is an area i'm not strong in, so thanks for the formula. Can you define R, V, P and I just so i'm 100% clear on what those vars actually are? I'm assuming resistance, voltage, power, and I don't know what I would be. 

but if i build something i will definitely share of course.
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-05-04T18:55:34.028Z Reads: 145

```
Those look just like the things in the aluminum rails that they were calling HiPots at my old job. I'm checking them out now.

also i just saw a $3000 price tag on an n3300 load tester... yeah. not happening lol. That's 2 X-Carves or half a steel hydraulic deck press.
```

---
## \#8 Posted by: makepeace Posted at: 2016-05-04T19:00:53.616Z Reads: 131

```
See edits above. Oh yeah and V is voltage in Volts (V), P is power in Watts (W), I is current in Amperes (A), R is resistance in Ohms.
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-05-04T19:07:14.582Z Reads: 129

```
[quote="makepeace, post:3, topic:2888"]
This is also bound to be expensive.
[/quote]

yes... it seems so. But i think it will be worth it in the long run. It may be something i have to wait a bit to build, but its definitely happening.
```

---
## \#10 Posted by: makepeace Posted at: 2016-05-04T19:19:39.332Z Reads: 124

```
I'd almost think it might be better to build a test setup similar to @onloop's but with a "dyno" so to speak. Strap the board down with the wheel driving a drag wheel and then you can load test batteries, motors and ESCs all at the same time, probably for a lot cheaper. You'll have more variables there though, so it might be hard to figure out what's failing. The VESCs will provide pretty good diagnostics though. If you load some of these motors close to their max power draw, you'll get these battery drained in no time.
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-05-04T19:23:15.786Z Reads: 115

```
It was actually @onloop 's dyno that gave me the idea, so i may just go this route if i can find a way to do it without consuming more garage space. It would be a purely mechanical solution at first, of course, and i'm not quite sure how i would put resistance on the wheel yet but i could maybe figure something out.
```

---
## \#12 Posted by: Mobutusan Posted at: 2016-05-04T19:36:44.887Z Reads: 113

```
@longhairedboy 
Maybe you could rig up some drive system from the wheels to something like a small outboard boat motor & prop that's mounted in a big bucket of water to provide resistance. It would be a consistent source of resistance if you could pull it off. Just a thought.
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-05-04T19:40:42.284Z Reads: 111

```
that sort of thing s along the lines of my thinking... i thought about a big wheel with a thick belt on it that would just drag on the wheel but that would make a lot of heat and wear out and probably make dust or grime as well. water as the force resister... hmmmmm
```

---
## \#14 Posted by: Mobutusan Posted at: 2016-05-04T19:43:47.354Z Reads: 107

```
Water is great for heat absorption too (as if you didn't know)! You could get all crazy and route a water cooling loop to the battery pack and motor to try and simulate the cooling effect from riding, or just keep temps down in general during testing.
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-05-04T19:45:24.590Z Reads: 103

```
don't tempt me. I ran a water cooled pentium 4 dual core for a couple of years as a gaming rig. I still have the heat exchangers and pumps. next thing you know we've got water cooled battery packs, soft switches, and VESCs.
```

---
## \#16 Posted by: Mobutusan Posted at: 2016-05-04T19:56:04.172Z Reads: 111

```
Oh, I would NEVER try to tempt you. Besides, I don't think you've got the skills or cajones to make it work anyway. :wink: :laughing: jk

And how cool would that be to run a water cooled system through some visible vein/tube system in the deck or enclosure and fill it with water dyed a crimson red color? Scarlet would have her own working circulatory system. And illuminate the whole system so it looks super sweet, while your at it.
```

---
## \#17 Posted by: Karmannghiagirl Posted at: 2016-05-04T19:57:28.347Z Reads: 119

```
If you want to replicate cooling from riding, why not have a fan be the load? Just get a RC prop (which will obviously fit on a brushless motor) and have that be the load.
```

---
## \#18 Posted by: chaka Posted at: 2016-05-04T20:05:36.118Z Reads: 140

```
Build a bench test rig using a prop and a coulometer on a large motor. Cheapest way to get it done. Be careful though, you can easily pull enough wattage to ruin some gear.

This guy rigged up a thrust gauge but it isn't needed for our use.

Oh yeah, almost forgot. This is very dangerous, it can kill you!

https://www.youtube.com/watch?v=q80Zl1Ca0Hc
```

---
## \#19 Posted by: lock Posted at: 2018-01-16T11:01:09.177Z Reads: 92

```
Used a [simple online circuit design tool](http://www.falstad.com/circuit/circuitjs.html) to come up with this.

![IMG_1999|640x480](upload://xhzZc80Qsqm7USnJvSIxDcxjtv8.jpg)

It's 2s2p 25ohm 100w resistors. Based on the calculations total drain should be 1.8a, and each resistor should be burning off a little under 20w or so; well under the 100w they are rated for. Interestingly at this low wattage they are still too hot to touch.

Running them in a 1s4p configuration would result in about an 8a current, and each resistor would be pushed to 80w. Given how hot they are now I'm not too keen on testing this. Might look around to see what else offers a suitable resistance for higher currents (and is able to sustain them) without costing too much.

I use the watt meter for charging, but it's handy here. Looking to see if the capacity just before it (hopefully) gets shut down by the BMS matches what it should be. Speaking of which, the DieBieMS spits out everything the watt meter does but also includes individual cell voltages so it's kind of a little redundant in this case.
```

---
## \#20 Posted by: pat.speed Posted at: 2018-01-16T11:34:40.000Z Reads: 82

```
You could put your cup off coffee on there so it doesn't go cold or you might as well just boil the water for your coffee with it
```

---
## \#21 Posted by: lock Posted at: 2018-01-16T11:53:47.779Z Reads: 84

```
Hmmm, might just get the multimeter out to probe the resistance of the kettle🤔. 

We use electric kettles for boiling water round these parts; recently I was lead to believe this is quite the novelty in the US.
```

---
## \#22 Posted by: Okami Posted at: 2018-01-16T13:30:32.292Z Reads: 80

```
Not sure whats the situation where u live but u could try to find decent power tool li ion packs. 

These should have high drain batteries inside of them, usually already spotwelded.
```

---
## \#23 Posted by: SimosMCmuffin Posted at: 2018-01-16T13:37:04.295Z Reads: 85

```
Those high power resistors are meant to be mounted to a larger metal heatsink for cooling. Your carbon cellulose slab is not an ideal heatsinking material :D (You probably just wanted to attach them to something, fair enough)

But for reference, something like this. Might not even need anything huge size wise, if you add some fans for forced convection cooling.
http://diyaudioprojects.com/Technical/DIY-Speaker-Dummy-Load/DIY-Speaker-Dummy-Load-u.jpg
```

---
## \#24 Posted by: longhairedboy Posted at: 2018-01-16T15:16:17.213Z Reads: 76

```
That's basically a HiPOT, which is something i need. They're used for load testing and discharging. Most people use lightbulbs now because they're cheaper than these huge resistors that also require some kind of framing and have to be kept away from everything. 

maybe there's a fancy way to make a hipot out of lightbulbs. Maybe some kind of hilarious sign full of bulbs.
```

---
## \#25 Posted by: pat.speed Posted at: 2018-01-16T22:22:35.117Z Reads: 75

```
Just hang a bunch of em up all around your work shop. When it goes dark plug em into your skateboard and poof your shed is lit. Oh and make sure to get multi coloured ones 😝
```

---
## \#26 Posted by: SkaterBoy58 Posted at: 2018-01-16T23:09:32.431Z Reads: 73

```
LHB -Best bet is to get an 8 ohm 100W wirewound resistor (Got mine from Aliexpress) and do a full discharge test from 42V to 30V (for 10S) with regular voltage readings of each cell pack. This will show up any dud cells.See my blog at https://evolveforums.com/threads/bamboo-gt-at-50km-range-project.1169/page-7
for how I did it .Check voltage and AH against cell specs -use exel for graphing and ah calculation -I can send file to you if you want.
Note fan for cooling of resistor . 8 ohm at 40V will give 5 amp and 200W -but with a fan 100W resistor will be fine ![image|666x500](upload://bAlCuNYn1bVAz0nux8ae4ilrYrV.jpeg)![image|281x499](upload://myp6DBzsWVpX7j1sGNzhKBxfIkD.jpeg)
```

---
## \#27 Posted by: lock Posted at: 2018-01-17T13:54:48.210Z Reads: 60

```
Liked your idea so much @SkaterBoy58 I, errrr, stole it  :grimacing:

Wrote some python code to periodically poll the DieBieMS and write the data out to a CSV file I could create a chart from fairly easy. I'll give a few more details on this over in the [other thread](http://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/251).

a123 LiFePO3 based pack, so if the voltages seem a little odd...

![2018-01-17-21-09-09_cells|663x482](upload://6XwqZz248XYMvuHPxRn9aLMtMrc.png)

Discharge was no more than 1.6a, so I really wasn't expecting to see much drift across the cells. Having a less well balanced pack probably would have made for a more interesting chart though.

![2018-01-17-21-09-09_status|671x485](upload://iO9OEtr9YEziBtCuutwXxqRIMSr.png)

One of the nice things about the DieBieMS is how it tracks state of charge, and doesn't just base percentage remaining off the current pack voltage. It'd be tough to get a reliable charge % based on the voltage change shown above. Red line seems right as the pack was drained using a constant resistance.

Will be interesting to run the same tests after the pack has been used for a while.
```

---
## \#28 Posted by: Acido Posted at: 2018-01-17T14:00:13.446Z Reads: 50

```
Maybe use an engine starter?
But it probably draws way more amps than batteries for eksate
```

---
## \#29 Posted by: lock Posted at: 2018-01-17T14:15:58.687Z Reads: 54

```
[quote="SimosMCmuffin, post:23, topic:2888"]
Your carbon cellulose slab is not an ideal heatsinking material :smiley: (You probably just wanted to attach them to something, fair enough)
[/quote]

I just noticed the wood under the resistors is singed :open_mouth: .
```

---
## \#30 Posted by: SimosMCmuffin Posted at: 2018-01-18T06:22:31.662Z Reads: 52

```
Do you have any spare fans hanging around? Just some forced airflow over them would greatly increase their heat dissipation
```

---
## \#31 Posted by: SkaterBoy58 Posted at: 2018-01-18T08:27:31.697Z Reads: 55

```
no worries -ideas are for sharing here
My DIY pack is 10S8P with MJ1 cells so about 1000wh in total-explains the long time for my discharge test!

.I used a 200W load to simulate average riding conditions .
That is at 20km/hr and 10wh/km =average of 200W .

Cheers
```

---
## \#32 Posted by: pat.speed Posted at: 2018-01-18T11:13:03.946Z Reads: 53

```
Just letting you know but the 10wh/km is for distance referencing not speed. Although it may work for speed too but I don't think it does
```

---
## \#33 Posted by: SkaterBoy58 Posted at: 2018-01-18T13:43:01.381Z Reads: 50

```
Nah 
10wh/km is typical board energy consumption going at 20km/hr
Cheers
```

---
## \#34 Posted by: longhairedboy Posted at: 2018-01-18T15:16:35.475Z Reads: 48

```
it takes about 440 watt hours to take ~150 pound man ~25 miles at ~20 mph on a calm day on terrain that is on average mostly flat. 

That metric is based on the 12S4P 25R pack, which is what i used to build. 

i base all of my gut calculations on that and have been getting adequately close results to what i suspect will happen.
```

---
## \#35 Posted by: pat.speed Posted at: 2018-01-18T21:45:03.417Z Reads: 41

```
Actually it is the typical consumption of power from your battery pack. That can vary greatly depending on hills, rider weight and quality of the cells

Other people have come up with results showing that around 4000 watts is required to reach 40mph (64km/h). According to what you have said it would only take about 650 watts.
```

---
## \#36 Posted by: lock Posted at: 2018-01-20T07:28:36.358Z Reads: 42

```
Load test setup v2. Added some bullet connectors so I can switch between 2s2p and 1s4p. 4p drops the resistance and ups the amps to about 6, power works out to be approx 250w.

It was fairly obvious something was going to catch fire if I didn't change anything, so here's the new setup. As suggested I dug the fan out, but also g-clamped a meter long strip of aluminium I had lying around across the top of the resistors.
![IMG_2005|625x500](upload://6CA73U702ICHI4zlLzVpDOqa48s.png)

Kept an eye on temps throughout the test, and it was cooler than when I was testing at 1.6a. Nothing too surprising about the discharge curves, which is a good thing. Kept recording data after the BMS shut down discharge to see how the cell voltage bounced back.
![chart|663x482](upload://ra5F9TWYiivDXylwTiNmg3KV8wc.png)

And here's the charge cycle after this test. The DieBieMS cell mismatch is set to 0.01v, which makes  sense when you look at the chart.
![chart (2)|663x482](upload://deaaAOoK8cwzDlbc69DD01CfMGP.png)
```

---
## \#37 Posted by: SkaterBoy58 Posted at: 2018-01-20T08:18:44.652Z Reads: 37

```
LHB 
Ater doing US/Aust conversins  this equates to about 10.9 Wh/km which is about what I get on streets on flat ground on a good day.

Good to know that the laws of physics work world wide?

Cheers
```

---
## \#38 Posted by: SkaterBoy58 Posted at: 2018-01-20T08:22:35.085Z Reads: 38

```
Pat
Think you getting mixed up with instantaneous power required for a particular speed and friction overcomming requirement with energy (with a time element) over a range of riding conditions 

Cheers
```

---
