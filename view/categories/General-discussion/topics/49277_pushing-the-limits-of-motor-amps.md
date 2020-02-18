# Pushing The Limits of Motor Amps

### Replies: 89 Views: 4249

## \#1 Posted by: Eboosted Posted at: 2018-03-15T06:36:49.086Z Reads: 525

```
I'm pushing 40Amax battery and 100A max motor amps on 12s4p with Samsung 30Q

The 6384s feel really torquey
```

---
## \#2 Posted by: E1Allen Posted at: 2018-03-15T07:02:49.259Z Reads: 511

```
[quote="Eboosted, post:29, topic:49103"]
100A max motor amps 
[/quote]
Do you have BT module to see how many amps your motor is pulling?  Do they get that high?
```

---
## \#3 Posted by: Deckoz Posted at: 2018-03-15T13:53:56.958Z Reads: 486

```
I also have 100 amp motor max on my 13s setup...

100a Motor Max
-40a motor min
50a batt max
-15a bat min

I only hit the motor max from a stop..lol
```

---
## \#4 Posted by: Eboosted Posted at: 2018-03-15T22:04:52.617Z Reads: 457

```
[quote="E1Allen, post:30, topic:49103"]
Do you have BT module to see how many amps your motor is pulling?  Do they get that high?
[/quote]

This was on a flat surface no incline, that means almost 70A per motor. On an incline full throttle it might reach 90A per motor, battery max didn't ever exceeded 40A per VESC

[img]http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/9/f/9fb4708de4b1b00b6f6aef935ea209b926edf65a_1_520x500.png[/img]
```

---
## \#5 Posted by: E1Allen Posted at: 2018-03-15T23:35:06.284Z Reads: 422

```
Very interesting.  I just didn't think it would be able to spread that far between battery and motor amps.  Like if you set it to a hypothetical 10a battery and 120a motor it seems like it wouldn't be able to reach those motor amps because there wasn't enough battery amps coming in to support it.  I just don't understand the limits associated with it other than you get higher motor amps at lower motor rpm
```

---
## \#6 Posted by: Eboosted Posted at: 2018-03-15T23:46:24.484Z Reads: 425

```
It's pretty confusing, it seems the current is accumulated between the motor and battery, like a power container, this creates immediate power/torque response whenever it's needed by the VESC.

I wonder if I''d have more power or torque if I increase the motor max to 120A even though I'm limiting the battery draw to 40A per VESC
```

---
## \#7 Posted by: E1Allen Posted at: 2018-03-15T23:54:37.455Z Reads: 410

```
Exactly.  I don't know.  The Caps may be transferring some of that peak power as well. But I dunno how much
```

---
## \#8 Posted by: Cobber Posted at: 2018-03-16T00:01:54.252Z Reads: 410

```
doesn't the speed controller for a brush less motor "pulse" the power to the motor? certain poles at certain times, at a particular frequency?

I might be wrong I'm not a EE

edit:

Jenso has his set up 130/100/175 here

http://www.electric-skateboard.builders/t/e-toxx-directdrive-vs-trampa-vesc6-vs-leopard-8072-170kv-vs-nowind/30822/129?u=cobber
```

---
## \#9 Posted by: Deckoz Posted at: 2018-03-16T00:27:07.245Z Reads: 394

```
It's very simple

Battery max of 50amps on a 50v system is 2500 watts

That means at 100% duty cycle you can have a max of 50 battery amps. 

50v * 50a = 2500w

This means that above 50% duty cycle you can no longer create 100 motor amps

2500w/100a = 25v

50v * 50% duty cycle = 25v

50v * 75% duty * 100a = 3750w. But battery max is 2500w(50a on 50v)
Meaning motor max will really be

50v* 75% duty = 37.5v
2500w/37.5v = 66.6a or 2500w on 37.5v...


All of this also means that below 50% duty if the fets could do it you could theoretically set upto 250 motor amps what the fets are spec'd for... But as duty cycle increases motor amp output will drop to meet the battery max requirements

2500w / 250a = 10v. Or 20% duty. Above 20% duty 250a would not be capable. Motor amps fall as duty increases to not exceed battery max
```

---
## \#10 Posted by: Cobber Posted at: 2018-03-16T01:32:51.426Z Reads: 355

```
[quote="Deckoz, post:37, topic:49103"]
Motor amps fall as duty increases to not exceed battery max
[/quote]

if within the limits of the controller...
what happens in reverse? (If battery is set higher than motor, but AC is higher than both)
```

---
## \#11 Posted by: Deckoz Posted at: 2018-03-16T01:40:20.524Z Reads: 365

```
If battery is set higher then motor...

The motor just isn't provided more amps then max motor . There are some instances where AC is hit because of a improper motor config which causes the magnetic flux to stall and the AC is hit... But that shouldn't happen with a good motor that's been detected properly

Also... Another example from a PM

>  It will shift downward with each % of duty
> 
> 30a bat max
> 
> 36v * 30a = 1080w
> 
> 36v * 25% duty = 9v * 60 motor amp = 540w
> 36v * 50% duty = 18v * 60 motor amp = 1080w
> 36v * 51% duty = 18.36v 1080w max/ 18.36v = 58.82 motor amps
> 36v * 52% duty = 18.72v 1080w max/ 18.72v = 57.56motor amps
> 
> Etc etc…
```

---
## \#12 Posted by: Deckoz Posted at: 2018-03-16T02:01:10.207Z Reads: 347

```
One more example because I see this alot...

Battery and motor amps set to be the same

36v system 30 battery max.. 30a motor max

As nominal is 36v but charged is 42v and discharged is in the range of 30-33.5 depending how safely you treat your li-ions.

42v * 30a = 1260w
40v * 30a = 1200w
38v * 30a = 1140w
36v * 30a = 1080w
34v * 30a = 1020w

Basically this configuration makes it feel like your board is slowly dying...vs feeling like the same!e performance across the charge as the maximum wattage slowly decreases..

With a motor amp lower then battery it will feel the same across the charge, top speed and acceleration

With a motor amp higher then battery it will accelerate the same across the pack  with a lower top speed as the pack voltage drop
```

---
## \#13 Posted by: Cobber Posted at: 2018-03-16T02:21:24.306Z Reads: 333

```
@Deckoz so with 49.8v full charge (4.15v * 12) and a 44.4v soft cutoff (3.7v * 12) running 80 battery amps and 72 motor amps...

49.8v * 72a = 3,585.6w
&
44.4v * 80a = 3,552w

I would have a linear power delivery and top speed across my usable battery voltage as set above (4.15v to 3.7v a cell).

Did I get that right or did I miss something?
```

---
## \#14 Posted by: Deckoz Posted at: 2018-03-16T02:32:25.792Z Reads: 326

```
For the most part yes...

Battery can output
49.8v * 80a = 3984W
Motor can receive
49.8v * 72a = 3585W

At 44.4v
Battery can output 
44.4v * 80A = 3552W
Motor can only receive
44.4v * 72A = 3196W

This is probably about as close as you can get to linear without specifying watts in a firmware like ackmaniacs. Ie set a 80a batt max and 80 motor max with a 3552w limit to limit output only the max power that I can output at cuttoff voltage across the entire pack.
```

---
## \#15 Posted by: Eboosted Posted at: 2018-03-16T04:46:22.364Z Reads: 313

```
Well now I understand a little bit more thanks @deckoz

I always thought the VESC adjusted the motor amps, now I know it adjusts voltage output through duty cycle. So the higher the DC the higher the voltage and more power is generated according to the preset motor current limit. 

That means increasing the motor amps won't help with more power output. However I'd like to kmow why my board feels say more powerful on full charge on 100A motor than at 80A
```

---
## \#16 Posted by: E1Allen Posted at: 2018-03-16T05:03:18.355Z Reads: 305

```
[quote="Eboosted, post:43, topic:49103"]
However I’d like to kmow why my board feels say more powerful on full charge on 100A motor than at 80A
[/quote]

Placebo effect.  🤔
```

---
## \#17 Posted by: Cobber Posted at: 2018-03-16T06:08:51.644Z Reads: 293

```
Maybe we should split this topic?
some of this may be useful to someone else one day :thinking:

kind of de-railed this build thread

@Namasaki
```

---
## \#18 Posted by: Deckoz Posted at: 2018-03-16T11:53:01.574Z Reads: 263

```
Agreed sorry for clutter
```

---
## \#19 Posted by: Namasaki Posted at: 2018-03-16T11:57:33.914Z Reads: 263

```
Agreed, very good info in this discussion. 
Don’t know if you guys knew it but @Hummie was one of the first if not the first to push the limits of motor amps when Vesc 4 was still relatively new. 
He convinced me to try it and I found a substantial increase in power just going from 60a to 80a.
```

---
## \#20 Posted by: professor_shartsis Posted at: 2018-03-16T12:19:24.572Z Reads: 263

```
an esc works by a similar principle to a dc to dc buck converter in continuous mode which can also lower the effective voltage while increasing the amps. the battery is periodically connected and then disconnected from the winding at a frequency on the order of 25khz. During the times the winding is disconnected from the battery, the winding is shorted to itself which allows the current generated during the brief on times to continue circulating during the off times. since the current continues to flow in the winding during the off times, the “motor amps” are numerically higher than the “battery amps.” the battery may see 10a @ 50v, 10% of the time which averages to 1a, while the motor effectively sees 10a @ 5v the entire time. In reality the current rises in the motor from, say, 9.5a to 10.5a during the 10% on times, then decays from 10.5a to 9.5a during the off times.

as the back emf voltage produced by the motor increases with increasing speed, it is necessary to increase the on time (duty cycle) of the circuit to maintain the same number of motor amps, which draws more and more battery amps.

Pack V * duty cycle % = V effective

(V effective - V bemf)/Resistance=Motor Current
```

---
## \#21 Posted by: Deckoz Posted at: 2018-03-16T12:24:19.603Z Reads: 245

```
[quote="Eboosted, post:15, topic:49277"]
always thought the VESC adjusted the motor amps, now I know it adjusts voltage output through duty cycle. So the higher the DC the higher the voltage and more power is generated according to the preset motor current limit
[/quote]

The vesc does adjust motor amps... Most of us use current control, which the primary function is amp adjustment, Just it is adjusting amps and rampung duty cycle to change motor voltage to generate more wattage 
If it tried to throw as many amps at the motor as it can..say 80 amps motor max

If you hit 80a motor max at 10% duty
50v * 10% duty = 5v * 80a = 400w

We can only produce 400w on 10% duty of 50v at 80 amps, but the load(your weight + demand of acceleration or speed) is requiring more wattage.

The 80 motor amps will stay 80 motor amps and increase duty cycle to output more wattage, until 

- The load decreases(stopped acceleration)
- motor gets into it's efficiency torque rpms where it generates torque with very little amps above x rpm
- The combination of motor amps, and duty cycle makes a wattage/current higher then max battery
```

---
## \#22 Posted by: professor_shartsis Posted at: 2018-03-16T12:38:24.884Z Reads: 238

```
[quote="Deckoz, post:21, topic:49277"]
50v * 10% duty = 5v * 80a = 400w
[/quote]

50v battery * 10% duty = 5v effective volts
(5v effective - 0v bemf) / 0.0625ohm winding = 80a motor amps
5v * 80a motor amps = 400w electrical watts
80a motor * 80a motor * 0.0625ohm = 400w copper loss
400w / 50v battery = 8a battery amps
```

---
## \#23 Posted by: Deckoz Posted at: 2018-03-16T12:49:54.022Z Reads: 223

```
Exactly

I was just trying to keep the maths simple for everyone. As we could bring in BEMF, and load and heat saturation...but...yea :)
```

---
## \#24 Posted by: professor_shartsis Posted at: 2018-03-16T12:53:06.784Z Reads: 218

```
(1/KV)*RPM=BEMF V

(1/100kv)*100RPM=1V BEMF
```

---
## \#25 Posted by: Pedrodemio Posted at: 2018-03-16T13:02:41.324Z Reads: 217

```
[quote="Eboosted, post:15, topic:49277"]
I’d like to kmow why my board feels say more powerful on full charge on 100A motor than at 80A
[/quote]

Because it is more “powerful”, what we fell is is not power, but acceleration, and it’s directly proportional to torque and that’s proportional to current

So if the duty cycle is low enough that you are not hitting the battery limit, that’s means low speed since duty cycle and speed generally have a linear relation, you are getting more torque if you motor off the line until the battery current limit is hit comparing the 80A to 100A

The more you increase the motor current the more torque you get until a given speed, but if you maintain the same battery limit, this speed that you can use max torque gets lower as you keep increasing motor max

This if of course ignoring motor saturation or it breaking itself apart 

As example, my board can theoretically climb a 27% incline, but only at a max of 16 km/h since that’s the speed that the motors can keep the max current of 80A without hitting the 30A battery limit
```

---
## \#26 Posted by: SimosMCmuffin Posted at: 2018-03-16T13:04:35.551Z Reads: 212

```
[quote="Deckoz, post:21, topic:49277"]
The 80 motor amps will stay 80 motor amps and increase duty cycle to output more wattage, until

- The load decreases(stopped acceleration)
- **motor gets into it’s efficiency torque rpms where it generates torque with very little amps above x rpm**
- The combination of motor amps, and duty cycle makes a wattage/current higher then max battery
[/quote]
Can you clarify/explain what you mean with the boldened text?
```

---
## \#27 Posted by: Deckoz Posted at: 2018-03-16T13:08:19.913Z Reads: 216

```
Most motors have a torque curve that could likely be provided by manufacturer. Example

![torque-speed-393|690x480](upload://as7sD6XP8WpJfDamR098p7sXj82.jpg)

Let me know if this doesn't make sense...

As side note this is pronounced on single drives. Struggle along til say 16mph then out of no where it feels like turbo boost because the motor has gotten into it's efficiency range... So 0-16 is moderate acceleration, but 16-24 feels like a rocket..
```

---
## \#28 Posted by: professor_shartsis Posted at: 2018-03-16T13:21:39.674Z Reads: 203

```
KT (torque per amp) can be calculated directly from KV:

KT (newton meters torque per motor amp) = 60/(2 * pi * kv)

0.0954nm/a = 60/(2 * pi * 100kv)

therefore 80a motor current * 0.0954nm/a = 7.632 newton meters torque @ 100kv

7.632 newton meters torque * angular speed of the motor in radians per second = mechanical watts

(1000rpm * 2 * pi)/60 = 104.719 rad/sec

7.632 newton meters torque * 104.719 radians per sec angular speed= 799.22w mechanical power

799.22w mechanical power / 1000w electrical power = 79.92% electrical to mechanical efficiency

the difference between the electrical power and mechanical power appears as ohmic heating in the motor windings.
```

---
## \#29 Posted by: SimosMCmuffin Posted at: 2018-03-16T13:22:18.168Z Reads: 201

```
[quote="Deckoz, post:21, topic:49277"]
it generates torque with very little amps above x rpm
[/quote]
This part is the one I have issue with.
What exactly do you mean by with this? Does it generate more torque with little amps @ high rpm?
Isn't torque theoretically (not counting losses or other un-ideal effects) directly related to motor current?

Am I to understand that the motor generated more torque with lower motor current at higher RPM?

EDIT: I also looked up that same graph as you linked, before asking the question, because I still couldn't understand what you meant by this specific part of the sentence.

EDIT2: Or do you mean "it generates **very little** torque with very little amps above x rpm"
```

---
## \#30 Posted by: Deckoz Posted at: 2018-03-16T13:27:51.915Z Reads: 193

```
If volts is speed and current is throughput, and load is equivalent to watts

If the load stays the same, the voltage goes up(duty cycle) and amps goes down. 

Typically you won't hold max motor amps up until the max duty cycle equal to max battery amps... As the motor is "unloading" in a sense as voltage increases...  as the load is staying the same(board + your weight @ throttle %)

Higher amperage is affected by resistance more then voltage. So at low voltage, high amps. More watts are wasted as heat. where at higher voltage lower amperage, less watts are wasted as heat and translate into mechanical power

@professor_shartsis has a good example above to calculate efficiency.
```

---
## \#31 Posted by: SimosMCmuffin Posted at: 2018-03-16T13:34:26.578Z Reads: 191

```
So you meant that in the scenario of the motor current being restricted by battery current?

AKA, if you have hit the battery max and continue speeding up, then motor amps will start to decrease to keep the same power?
```

---
## \#32 Posted by: Cobber Posted at: 2018-03-16T14:06:43.567Z Reads: 179

```
i'm sorry DeckyBro you stood up and now you have to endure...
props mate
```

---
## \#33 Posted by: Pedrodemio Posted at: 2018-03-16T14:08:50.315Z Reads: 180

```
What’s VESC are you using? If it’s 4.12 or any variant with just two shunts the boost is because noise in the current measurement that makes the duty cycle jump to 95%
```

---
## \#34 Posted by: Deckoz Posted at: 2018-03-16T14:09:06.591Z Reads: 186

```
Ah no I mean more so efficiency in combination with duty as efficiency and torque curves change with duty(motor voltage)

![tokai-u-motor-efficiency-graph|300x290](upload://7P7XG7n8JlvXEzIJShZ8pFcCySs.jpg)![Silicon Labs - AMC Figure 1|348x218](upload://gUUMnzAfjzUP0eIqbGdlRSgPn5M.jpg)

What ends up really happening is you have many voltages and many curves, if you were to plot a graphs with the various curves on many voltages(duty) you would end up some something that looks similar to surge graph for turbochargers...but for bldc

Basically same electrical power over varying voltages results in different efficiency
![500px-Torque_at_different_voltages|500x220](upload://xoifMXblvleqChuOWwgtGGgcYTY.png)

Anyway I cannot find any images where people have overlaid the graphs at different voltages(duty) from the same bldc. but it would looks similar to pump/compressor graphs
![H-3|439x500](upload://9dpEHTFzuozLUZzIPdqbGEF7hJm.JPG)
```

---
## \#35 Posted by: Sebike Posted at: 2018-03-16T14:28:07.564Z Reads: 172

```
Thank you @deckoz for enlightening and educating us 😊
```

---
## \#36 Posted by: b264 Posted at: 2018-03-16T14:32:56.329Z Reads: 175

```
[quote="Eboosted, post:6, topic:49277"]
it seems the current is accumulated between the motor and battery, like a power container, this creates immediate power/torque response whenever it’s needed by the VESC
[/quote]

Yeah, it's accumulated in those 2 or 3 big capacitors on the VESC input and the reason you need an anti-spark switch.
```

---
## \#37 Posted by: SimosMCmuffin Posted at: 2018-03-16T19:20:00.304Z Reads: 175

```
You mean a map of the motor efficiency like this one? 
![image|690x409](upload://r2SOyucKTHJZAx36VqFYbcnGMKp.jpg)
https://www.eleceng.adelaide.edu.au/students/wiki/projects/index.php/Projects:2015s1-61_Computer_Aided_Measurement_and_Analysis_of_Equal_Efficiency_Characteristics_of_Electrical_Machines

Or
![image|690x406](upload://4nvMQFjolrHaEHLk9OXVSj8Hext.png)
https://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2017/apg67_kss223_ejy25/kss223_apg67_ejy25/kss223_apg67_ejy25/index.html

So Y-axis is motor current(torque) and X-axis would be motor speed(BEMF)?
```

---
## \#38 Posted by: Deckoz Posted at: 2018-03-16T19:22:57.667Z Reads: 172

```
Yes exactly like that.

And yep you got it right with amps and BEMF. 

Good find, i dug for a while and couldn't find and overlay like that
```

---
## \#39 Posted by: Cobber Posted at: 2018-03-16T19:23:26.904Z Reads: 174

```
Adelaide represent! :grinning:
```

---
## \#40 Posted by: SimosMCmuffin Posted at: 2018-03-19T12:49:56.125Z Reads: 183

```
@Deckoz @professor_shartsis
Been letting this thing brew in the back of my mind and I think I have a pretty good understanding of the parameters and their effects now, but then I started to think why does the efficiency go down with different torque/current at some specific speed?

For example in the linked graph @ 2400 RPM, if we're running the motor with low torque/current or high torque/current it's efficiency is worse than at around 30 Nm?
![image|690x406](upload://cSANB75FzqxtY5tMRFjAZI5IjA.png)

Well I found another research paper with the following graphs for IM (induction motor), IPM (interior permanent magnet motor) and SPM(surface permanent magnet motor), which they generated with a similarly spec'd motors of the different types.
![image|356x500](upload://bIKNnCVskYeCkQBIsLbySnI8O9c.jpg)

So, if I apply my understanding. At low torque/current the motor is essentially operating closer to the no-load state, which is effectively a speed dependent static drag on the motor, which uses in relation a bigger portion of the power with low torque/current for the output power (aka, just to spin the motor). 

And then at the higher torque/current we're getting exponentially increasing copper losses, which then limit the efficiency at high torque/current?

Referenced research paper:
http://porto.polito.it/2627142/1/effciency_mapping_ecce_rv2.4.pdf
```

---
## \#41 Posted by: Deckoz Posted at: 2018-03-19T13:27:08.823Z Reads: 163

```
Yep copper losses, and the magnetic flux linkage. The iron in the bell's magnets go through demagnetization and have losses as well depending on the magnet type (n42h n42sh n52sh etc)
```

---
## \#42 Posted by: Hummie Posted at: 2018-03-23T18:24:38.556Z Reads: 161

```
[quote="Deckoz, post:41, topic:49277"]
copper losses, and the magnetic flux linkage. The iron in the bell’s magnets go through demagnetization and have losses as well depending on the magnet type (n42h n42sh n52sh etc)
[/quote]

The magnets don't go through demag. If they do they are done. The only losses in mags are Eddy currents. Regardless of type
```

---
## \#43 Posted by: Deckoz Posted at: 2018-03-23T19:00:23.954Z Reads: 157

```
Demagnetization of the permanent magnets occurs to some extent whenever a current flows in the motor winding. 

As well most of the magnets we use start to.demagnetize around 160-170F and are fine once cooled.
```

---
## \#44 Posted by: Hummie Posted at: 2018-03-23T19:11:27.338Z Reads: 155

```
Yea mags will decrease their magnetism at high heat a bit n come back but its not a loss. It's heat related. Not current related.
```

---
## \#45 Posted by: RedEagle Posted at: 2018-03-23T20:16:27.504Z Reads: 159

```
I always thought that once they're demagnetized they will be unusable?(no magnetization afterwards)
You learn something everyday around here..
```

---
## \#46 Posted by: Hummie Posted at: 2018-03-23T21:15:06.133Z Reads: 156

```
But I think it right in that at higher temps when the mags are decreasig. Their strength then in compensationitscopper losses as the mag field is needed to be built theretoxontume same torque
```

---
## \#47 Posted by: Pedrodemio Posted at: 2018-03-23T21:35:01.021Z Reads: 156

```
But, and a big but, if the motor is badly designed the hysterisis loop that makes the magnet work can dive into the demagnetization region, even at ambient temperature.

 I still didn't get that part well enough to be certain, but from what i understood with a high enough flux, or with high flux concentration due to stator design you can make this happen, so each phase activation would demagnetize the motor a little

That being said I guess the flux intensity and materials that are used for our application don't let this happen, but again, not sure yet
```

---
## \#48 Posted by: Hummie Posted at: 2018-03-23T23:43:37.486Z Reads: 153

```
I thought the mags would demanitize not ever a little but an instantly reverse polarity.  with a bad hysteresis loop would that be an overlapping of polarity or something where the motor produced a strong enough field to reverse polarity?
```

---
## \#49 Posted by: RedEagle Posted at: 2018-03-23T23:49:17.020Z Reads: 148

```
Devin is that you?
```

---
## \#50 Posted by: Deckoz Posted at: 2018-03-24T00:08:10.776Z Reads: 147

```
Devin? Not sure what your trying to imply..
```

---
## \#51 Posted by: RedEagle Posted at: 2018-03-24T12:20:52.266Z Reads: 141

```
To someone who doesn't know a thing about motors he sounds just like him, no?
(not to be rude, it was just a thought)
```

---
## \#52 Posted by: Pedrodemio Posted at: 2018-03-24T12:48:17.240Z Reads: 140

```
Not to be rude too, but the discussion is better if everybody try to add something. I’m expert in motors? No way, I know very little at the moment, but I’ve studying a lot in the past few months to manage to build my own and only now everything is starting to click

Cheers
```

---
## \#53 Posted by: RedEagle Posted at: 2018-03-24T12:53:46.752Z Reads: 140

```
I know. I wasn't trying to be insultive(is that a word?). I just thought he reminded me of devin with all the technical stuff. @Hummie has definitely more knowledge than anybody else in my opinion. I could only dream to know as much as him about the subject.
```

---
## \#54 Posted by: Deckoz Posted at: 2018-03-24T14:35:59.407Z Reads: 139

```
I'm not Devin, and no offense, but hummie doesn't know everything.

Do a search, hummies been in alot of convos. There's some surprising ones around that show how little hummie knows about these motors in a system, and yet he builds them..

http://vedder.se/forums/viewtopic.php?f=6&t=276

So hate on me all you want, but I don't trust half the stuff he says..

Move along with that Devin nonsense.
```

---
## \#55 Posted by: Cobber Posted at: 2018-03-24T15:11:25.159Z Reads: 137

```
[quote="Deckoz, post:54, topic:49277"]
Move along with that Devin nonsense.
[/quote]

:grimacing:
```

---
## \#56 Posted by: Deckoz Posted at: 2018-03-24T15:20:32.823Z Reads: 136

```
No use comparing me to someone I clearly am not... So just making that as clear as possible. Lol not trying to start anything, just don't want to be compared to someone who has clearly been banned from theforums 5+ times.

I only share what I know, I'm not forcing my views in y'all or demeaning anyone when I share what I know. If x person doesn't agree with what I've said, don't agree and move along. Just because some dude(me or anyone else) in the internet said something doesn't make it right, so take what you want, leave what you don't. But I'm anything but this Devin character.
```

---
## \#57 Posted by: Cobber Posted at: 2018-03-24T15:24:09.145Z Reads: 135

```
100% with you DeckyBro!

struggling to believe that was a comment.
```

---
## \#58 Posted by: RedEagle Posted at: 2018-03-24T15:27:14.878Z Reads: 138

```
Sure no problem but I'm not sure what happened. I thought I replied to @Hummie not you lol
```

---
## \#59 Posted by: Pedrodemio Posted at: 2018-03-24T16:04:40.214Z Reads: 145

```
![image|690x388](upload://dURAeuYKtUGfJsYJouopA8NCZqZ.jpeg)

![image|690x388](upload://95sbzsPSzBwE5OnaKOSUEAPzQH1.jpeg)

From the first picture you can see the hysteresis loop in normal operation, as the external field (generated by the coils) gets more intense the loop goes down and two the left, if it goes down to cross the x axis you enter in the demagnetization region

The second picture show the influence of temperature, since the intrinsic field intensity goes down as it gets hotter, the external field intensity to cross the x axis gets smaller

The knee on the diagonal lines represent the non-linearity that is often discarded during design, so you can demagnetize sooner than expected


About the who knows what’s discussion, there’s two approaches to most things, practical and theoretical, @Hummie aproach is most practical and iterative, there’s nothing wrong with that

What’s better? Who knows, of course by an engineering stand point you should predict, design, simulate and etc before making something, but for a low volume market such as hub motors it may not be worth, a state of the art multi physics FEA software would set you back 30K or more, and if you have no knowledge of what’s happening on the background it’s worthless
```

---
## \#60 Posted by: Hummie Posted at: 2018-03-24T16:28:19.381Z Reads: 139

```
@Deckoz sorry I wasn't meaning to insinuate you were anyone, I was saying someone else here sounds a lot like Devin.  Devin is a good friend of mine for like nine years so regardless it's not an insult. 

@RedEagle thanks for the compliment but I don't know a lot of stuff that for many people is easy.  Coming with endless repeated questions till I figure it out is probably how I do it.    

that link thought @Deckoz,...I still didn't get my question answered.  its a basics electronics questions probably: how can the vesc make a complete circuit with the motor where there is created a high voltage,  ..so a circuit with a high voltage but not a high current.  why?  in my basic understanding if you have a high voltage in a circuit ...current will go.  unless there is some other circuitry bit which would just reduce it.  if you know....
I like to be in discussions above my head...like the present....   In practice demagnetizing the motor's magnets I still understand from either a high temp or an extremely strong field, and I'm guessing that what's produced in the "hysteresis loop" above is an extreme field produced by the coils and iron.  I'm guessing the stator would need both a very high current and also so much speed so as to have the peaks and valleys of the hysteresis loop overlap in a way to build the field strong enough....no?
```

---
## \#61 Posted by: Pedrodemio Posted at: 2018-03-24T17:55:02.099Z Reads: 133

```
I can't answer that since i'm still a little lost, but i highly recommend this book, "Brushless Permanent Magnet Motor Design" by Dueane Hanselman, the good think is that it doesn't assume you know anything like most books about motor design, it starts in the beginning and explains all the theory behind
```

---
## \#62 Posted by: SimosMCmuffin Posted at: 2018-03-25T09:41:58.916Z Reads: 136

```
[quote="Hummie, post:60, topic:49277"]
that link thought @Deckoz,…I still didn’t get my question answered.  its a basics electronics questions probably: how can the vesc make a complete circuit with the motor where there is created a high voltage,  …so a circuit with a high voltage but not a high current.  why?  in my basic understanding if you have a high voltage in a circuit …current will go.  unless there is some other circuitry bit which would just reduce
[/quote]

So why can the motor current be low if the applied motor voltage is high? Is this the right way to interpret your question?

The short answer is: because of the "Effective voltage", created by the VESC's duty cycle and battery voltage is only somewhat higher than the motor's "BEMF voltage", which is kV and RPM dependent. "Drive voltage" is the actual potential difference between the "Effective voltage" and "BEMF voltage" and is the actual potential/voltage difference that is pushing electrons through the motor winding.

"Drive voltage" = "Effective voltage" - "BEMF voltage"
"Motor current" = "Drive voltage" / "Motor winding resistance"

---

Example calculation with 100kV motor, with 100mOhm winding resistance. 40 V battery voltage. 25 Amps of motor current @ 0 RPM and 1000 RPM.

**0 RPM, BEMF = 0V:**
"Effective voltage" = "BEMF voltage" + "motor current" * "winding resistance" = 0V + 25 A * 0.1 Ohm = 2.5V
"Drive voltage" = "Effective voltage" - "BEMF voltage" = 2.5V - 0V = 2.5V
Vesc duty cycle = "Effective voltage" / "Battery voltage" * 100 = 2.5V / 40V * 100 = 6.25%
Electric power = "Effective voltage" * "motor current" = 2.5V * 25A = 62.5W

**1000 RPM, BEMF = 10V:**
"Effective voltage" = "BEMF voltage" + "motor current" * "winding resistance" = 10V + 25 A * 0.1 Ohm = 12.5V
"Drive voltage" = "Effective voltage" - "BEMF voltage" = 12.5V - 10V = 2.5V
Vesc duty cycle = "Effective voltage" / "Battery voltage" * 100 = 12.5V / 40V * 100 = 31.25%
Electric power = "Effective voltage" * "motor current" = 12.5V * 25A = 312.5W

---

Now, provided I didn't screw up the calculations. You can see that we're pushing in both example RPMs 25 Amps of motor current, but why? The VESC effective voltage is completely different in the examples, so why is the motor current the same?

Because BEMF voltage.

As the motor spins up, it's BEMF voltage opposes the effective voltage. What we should look in the examples is the difference between the BEMF voltage and effective voltage, which I would call the Drive voltage, because it's the actual electron moving potential difference. And as can be seen above, it's 2.5V at both RPMs, which explains the 25 Amps of motor current.

Thoughts on this model, questions?
```

---
## \#63 Posted by: Hummie Posted at: 2018-03-25T16:10:16.237Z Reads: 126

```
I’m saying how can the esc light up when pushing it with no batteries, so a circuit there, but not enough current to blow it unless the brakes go on. (Without batteries talking about). That’s what my question was on the vedder site
```

---
## \#64 Posted by: Deckoz Posted at: 2018-03-25T16:59:42.859Z Reads: 127

```
Current doesn't flow without the load.

vESc by itself only demands x load. Which equals to milliamps. How hard is that to understand?

Hook up a 12v led with a resistor, the led load is only a few mA, but the battery can power it for years. Does the led explode? No because the led only demanded x current. Aka load. Same thing.

Without a battery hooked up to the vesc, when the motor spins, the load is the components of the vesc.  Spin the motor components demand a small load. Eventually if you spin the motor fast enough the voltage is to high for the system and the components burn because of voltage, not because of current.
```

---
## \#65 Posted by: Hummie Posted at: 2018-03-25T17:03:04.843Z Reads: 124

```
Im imagining a generator spinning hooked up to an led and the generator is varying it’s output voltage.  How does the led not blow.  What limits the output from the generator.
```

---
## \#66 Posted by: Hummie Posted at: 2018-03-25T17:04:11.650Z Reads: 125

```
So it will blow if spun fast. Without brakes?
```

---
## \#67 Posted by: Deckoz Posted at: 2018-03-25T17:05:37.538Z Reads: 124

```
Back to what I just said.

[quote="Deckoz, post:64, topic:49277"]
Without a battery hooked up to the vesc, when the motor spins, the load is the components of the vesc.  Spin the motor components demand a small load. Eventually if you spin the motor fast enough the voltage is to high for the system and the components burn because of voltage, not because of current.
[/quote]

The components are rated for x voltage. The buck circuits limit voltage on the each for the different components. So the MCU stmf4 gets it's 3.3 and 5.5v, the low sides still exist. When the motor spins fast enough to over volt the DRV(63v) then the 5v buck burns the TVS diode(d5) and you have 8v gong to the MCU and they blow in order..

So yes a fast enough motor will over volt and blow the circuit. But within the limits of the circuit they only demand x current because they only equate to x load.
```

---
## \#68 Posted by: Sender Posted at: 2018-03-25T18:06:49.730Z Reads: 120

```
I figured it was something like this is the reason behind  the ole "dont ride your board switched off."

This makes perfect sense.
```

---
## \#69 Posted by: SimosMCmuffin Posted at: 2018-03-25T19:13:16.028Z Reads: 131

```
[quote="Sender, post:68, topic:49277"]
“dont ride your board switched off.”
[/quote]

[quote="Hummie, post:63, topic:49277, full:true"]
I’m saying how can the esc light up when pushing it with no batteries, so a circuit there,  but not enough current to blow it unless the brakes go on. (Without batteries talking about). That’s what my question was on the vedder site
[/quote]

Well, the same dangers are present even if your board is on. The real question should be, "is your battery connected?".

Below is an illustration of the "battery - motor controller - motor" connections.

![image|521x224](upload://6wMHbG8YZ17flVgOYo8DpasLXpp.png)

[quote="Hummie, post:63, topic:49277"]
I’m saying how can the esc light up when pushing it with no batteries
[/quote]
Even if the battery is disconnected from the motor controller, the motor can power it up. Why? BEMF voltage. as the motor turns it generates a voltage on it's phase wires. Now this voltage is relative to the motor's kV value and it's rpm. Let's say we have a 100kV motor turning at 1000 rpm (going downhill maybe), so it generates 10 V from it's phase wires. This current will be able to flow back into the DC bus, through the mosfet body diodes and charge up the capacitors, as illustrated below. 
The actual DC bus voltage will be the BEMF - 2 * "body diode forward voltage", so maybe realistically around 8.6 V. 
![image|521x224](upload://cpzijcHosKLFx5hEU7c7mGNoIVD.png)

This is enough for the DRV8302 buck regulator to create it's 5V output and then the 3V3 with the linear regulator and the MCU will power up. That's the short answer for how the motor alone can power up the motor controller.


[quote="Hummie, post:63, topic:49277"]
so a circuit there, but not enough current to blow it unless the brakes go on. (Without batteries talking about).
[/quote]
The voltage on the DC bus can become high in two cases when powered by the motor. 

Either the motor is spinning very fast and therefore generating high BEMF voltage, which is enough to exceed the voltage ratings on the components, making stuff blow up.

Or because the motor is spinning and keeping the motor controller powered up and you don't realize it, you decide to apply the brake with the remote control. When the motor controller is regen braking, it's actually acting like a boost regulator for the BEMF and thereby increasing the DC bus voltage. 
Remember that the **motor controller is acting like a buck controller when it's driving a motor** to lower the battery voltage to a more suitable level for the motor.
Well **in regen braking, it's behaving like a boost controller.** Using the motor BEMF voltage as a source and boosting it above the battery voltage, so the current will start to flow to the battery.

Now why does the motor controller blow up when it doesn't have the battery connected to it? Because we are boosting the motor's BEMF voltage, but there is nowhere for the energy to go, except to the DC bus capacitors, but the problem is that they can't store a lot of energy, so their voltage will keep climbing and climbing very quickly, until the voltage gets so high again that stuff starts exploding.

Did this explain it?
```

---
## \#70 Posted by: Deckoz Posted at: 2018-03-25T19:20:41.622Z Reads: 114

```
@SimosMCmuffin you are a master with words. 🤗🤗🤗
```

---
## \#71 Posted by: SimosMCmuffin Posted at: 2018-03-25T19:33:40.630Z Reads: 119

```
Thanks, I actually had a good conversation about this particular phenomenon with a customer at work, who develop and manufacture BMS' for industrial use. We're developing a product for them.

The scenario we were talking about was, what happens if you're regen braking and your battery pack gets disconnected for a reason or another. 

Two things can happen, if your motor controller is fast enough it can detect the dangerously high DC bus voltage (VESC high voltage cut-off) and stop the regen braking, at which point you can't slow down anymore, because you can't dumb the energy anywhere, but at least you didn't blow up your motor controller.
Or your controller isn't fast enough, it will boost the DC bus voltage too high and blow itself up, at which point 
again, you can't slow down anymore and you blew up your motor controller :smile:

The bleed resistor could prevent this, as talked in the http://www.electric-skateboard.builders/t/diy-break-chopper-protection-against-overvoltage-no-cutoff/49823/34 thread, but depending on it's location (battery, BMS, motor controller) and the electronic/mechanical fault that happens, it might still not be able to save the day. The best place for it would be at the motor controller, because then even if the battery and the BMS get disconnected, you can dump the energy right at the motor controller.
```

---
## \#72 Posted by: Sender Posted at: 2018-03-25T23:49:51.246Z Reads: 114

```
Dude, I had to read that like 4 times but I definitely gained some insight there; thank you for the knowledge bomb.

So, I got the bulk of this, but to some up (well I am in no place to sum up the eloquence)... the biggest risk is not having the battery connected more than merely the board not being on as there is nowhere to dump the excess BEMF voltage?   If the motor controllers are switched off but the battery is connected, will the BEMF voltage still dump the excess into the battery or can it only do that function if it is switched on?
```

---
## \#73 Posted by: Deckoz Posted at: 2018-03-26T01:55:41.483Z Reads: 113

```
Depends on if your using an antispark with fets or a loop key style... As one can be back powered one cannot.
```

---
## \#74 Posted by: Sender Posted at: 2018-03-26T03:05:15.019Z Reads: 112

```
Of course, I get it.....Still took me too long to figure out why it mattered.. duh and lol. Gracias.
```

---
## \#75 Posted by: SimosMCmuffin Posted at: 2018-03-26T05:35:56.550Z Reads: 115

```
[quote="Deckoz, post:73, topic:49277, full:true"]
Depends on if your using an antispark with fets or a loop key style… As one can be back powered one cannot.
[/quote]

Even the anti-spark/BMS might allow current to flow back to the battery from the "load side", if it's not a fully blocking FET setup. Loop key is indifferent to the direction of current, as one could guess.

The Vedder anti-spark would not stop this, as the current is able to go through the mosfet's body diode in the anti-spark itself + through the body diodes in the inverter bridge, in the case that it's just the purely the motor generating a high BEMF voltage. Not 100% sure what's the conduction path during regen braking in the mosfets, but regardless vedder anti-spark would still allow the regen braking to happen.
![image|690x224](upload://kL7hxPYB3Sa83dBGnEByn7ITDXZ.png)

A fully blocking switch setup usually has 2 N-channel mosfets with their Drains connected together, as shown below from the BQ76200's datasheet. The current would be able to go through the first mosfet's body diode, but then would be blocked by the second one. The second mosfet would need to be in conducting mode, for the current to go to the battery.
![image|690x263](upload://cveiuE4zvpVSjZcXDrJarQ03IFJ.png)
```

---
## \#76 Posted by: Deckoz Posted at: 2018-04-08T00:48:46.873Z Reads: 105

```
I'm revisiting this, as I made a mistake in some of my wordings in regards to top speed.

I've been gearing for the top speeds I want to achieve at dead battery. So as the battery dies I won't really ever notice as it is outside of my normal riding range.
```

---
## \#77 Posted by: Hummie Posted at: 2018-04-08T08:03:33.100Z Reads: 102

```
@SimosMCmuffin
what is it that makes the motor less efficient when it is producing torque while further from it's no-load speed? 


when further from the no-load speed the back emf will be less but why would that make the motor less efficient? 

similarly why would a 100kv motor doing 20mph be more efficient than a 200kv motor doing 20mph?  Are motor amps more inefficient than battery amps for some reason?
```

---
## \#78 Posted by: SimosMCmuffin Posted at: 2018-04-08T09:55:07.565Z Reads: 100

```
[quote="Hummie, post:77, topic:49277"]
what is it that makes the motor less efficient when it is producing torque while further from it’s no-load speed?
[/quote]
Well, the further the motor is being run from it's no-load speed, the more amps you have to give it (hence it's further from it's no-load speed), which directly equate to more losses just in the windings due to their resistance. That is a pretty simple fact that should always be true. I think there are then more dynamic losses which are speed dependent.

Then there is the mechanical efficiency perspective, with the electric power IN and mechanical power OUT. for example if we are not driving any load, but we are spinning the motor, then our mechanical efficiency is 0%, because there is no useful mechanical work being done, but we are still using electrical power to just spin the motor.

[quote="SimosMCmuffin, post:40, topic:49277"]
So, if I apply my understanding. At low torque/current the motor is essentially operating closer to the no-load state, which is effectively a speed dependent static drag on the motor, which uses in relation a bigger portion of the power with low torque/current for the output power (aka, just to spin the motor).

And then at the higher torque/current we’re getting exponentially increasing copper losses, which then limit the efficiency at high torque/current?
[/quote]
---

[quote="Hummie, post:77, topic:49277"]
similarly why would a 100kv motor doing 20mph be more efficient than a 200kv motor doing 20mph?  Are motor amps more inefficient than battery amps for some reason?
[/quote]
It's mainly because of the higher currents with the higher Kv motors. Not so much in the motor itself, but everywhere else. I mean all things being equal in the motor, same stator size, same amount of copper with only the amount of winding turns changing, hence the different Kv values. They should still be able to run identically at different battery voltages, but with the higher Kv motor, the current everywhere else in the electrical system will be higher, so more resistive losses in the wiring and in the transistor stage.

Or so my understanding goes.

EDIT: wiring wise the difference between high and low Kv systems, is the wire insulation breakdown voltage and wire resistance. This goes for the whole electrical system overall. With very high voltages we wouldn't need as much copper to carry the same power, because low current, but we would need more insulation strength/thickness to stop the insulation from breaking down due to the higher voltage. Opposite of that with low voltages we would need more copper with less insulation to be able to carry the higher current.

I think this makes sense, if you look at something like an electric car with the battery voltages in the multiple hundreds of Volts. They still have pretty thick wires with thick insulation on them, but imagine how much copper (which is expensive) they would need if their system was a low voltage one. I think it's more economical to have higher voltage, use less expensive copper and more cheap insulation on wires, because the electronics can handle the higher voltages these days.
```

---
## \#79 Posted by: pakue Posted at: 2018-04-08T11:01:46.192Z Reads: 87

```
Copper losses should be relatively linear when ignoring skin effect of the windings. However the core losses increase exponentially with higher switching frequencies and flux densities. The magnetic field of any electromagnet tries to resist change thereby introducing a hysteresis in the system and causing losses. At even higher frequencies eddy currents induced in the stator taken an even stronger effect.
```

---
## \#80 Posted by: SimosMCmuffin Posted at: 2018-04-08T13:18:05.859Z Reads: 83

```
[quote="pakue, post:79, topic:49277"]
Copper losses should be relatively linear when ignoring skin effect of the windings.
[/quote]

Shouldn't copper losses be on an exponential curve in relation to current? P = I^2 * R ?
```

---
## \#81 Posted by: pakue Posted at: 2018-04-08T13:57:31.387Z Reads: 85

```
Yeah true, but different Kv motors the same size should also have the same amount of copper. So the one with the lower Kv should have a higher resistance and vice versa. Therefore the copper loss shouldn't be responsible for a large difference in efficiency.
```

---
## \#82 Posted by: professor_shartsis Posted at: 2018-04-08T14:38:02.855Z Reads: 86

```
[quote="Hummie, post:77, topic:49277"]
**what is it that makes the motor less efficient** when it is producing torque while **further from it’s no-load speed**?

when further from the no-load speed the back emf will be less but why would that make the motor less efficient?
[/quote]


assume the motor amp limit is constant... therefore copper losses and torque are constant. torque in newton meters multiplied by the angular speed of the motor in radians per second is the mechanical power produced. as the motor spins faster (closer to no load), more and more mechanical power is produced for the same constant copper losses (constant motor amp limit), and more mechanical power for the same losses means greater efficiency.

[quote="Hummie, post:77, topic:49277"]
similarly why would a 100kv motor doing 20mph be more efficient than a 200kv motor doing 20mph?  Are motor amps more inefficient than battery amps for some reason?
[/quote]

with the same km, pack voltage, battery amps and motor amps, the 100kv motor is less efficient, even when assuming the 200kv motor has double the Io & iron loss.

suppose these 2 motors are geared such that for both the present ground speed is 20mph.... both are the same KM... which is greater efficiency?

calculator source: http://www.bavaria-direct.co.za/constants/

https://image.ibb.co/cHRQHH/100kv_01rm.jpg

https://image.ibb.co/eSOi4x/200kv_025rm.jpg

^even with double the assumed iron losses & Io with the higher kv motor (io input doubled in this example) & the same km, **the higher kv motor has greater efficiency**, not less... 98% motor efficiency & 97.1% system efficiency for the 200kv compared to 95.5% motor efficiency & 94.6% system efficiency for the 100kv.

-------------

[quote="professor_shartsis, post:136, topic:7246, full:true"]
**km is the same:**

**100kv - 10 turns - 1 cross section - 0.1ohm**
60/(2 * pi * 100kv)=0.09549296585513720146133 newton meters torque per motor amp
(4v battery - 0v bemf) / 0.1ohm = 40a motor & battery current at 0rpm
4v * 40a = 160w electrical
40a * 0.09549296585513720146133nm/a = 3.819718634205488058453nm
3.819718634205488058453nm / sqrt(160w electrical) = **0.3019752726269222102173km**


**200kv - 5 turns - 2 cross section - 0.025ohm**
60/(2 * pi * 200kv)=0.04774648292756860073067 newton meters torque per motor amp
(4v battery - 0v bemf) / 0.025 ohm = 160a motor & battery current at 0rpm
4v * 160a = 640w electrical
160a * 0.04774648292756860073067nm/a = 7.639437268410976116907nm
7.639437268410976116907nm / sqrt(640w electrical) = **0.3019752726269222102173km**

**^km (torque per square root of watt) is the same**

-----------------------

**1:1 gearing - 10mph ground speed**
**100kv - 10 turns - 1 cross section - 0.1ohm**
1000rpm = 104.719755 radians per second
(11v battery - 10v bemf) / 0.1ohm = 10a motor/battery current
torque per amp: 60/(2 * pi * KV) = 0.095492nm/a
10a * 0.095492nm/a = 0.95492newton meters torque
11v battery * 10a current = 110w electrical
0.95492newton meters torque * 104.719755 radians per second = 99.99w mechanical
copper loss: 10a * 10a * 0.1ohm = 10w
wheel torque at 10mph @ 110w electrical = 0.95492nm * 1 gear reduction = 0.95 newton meters
**summary: 10mph ground speed, 0.95nm wheel torque, 99.99w mechanical, 110w electrical, 10w copper loss**

**2.150:1 gearing - 10mph ground speed**
**200kv - 5 turns - 2 cross section - 0.025ohm**
2150rpm = 225.14747 radians per second
(11v battery - 10.75v bemf) / 0.025ohm = 10a motor/battery current
torque per amp: 60/(2 * pi * KV) = 0.047746nm/a
10a * 0.047746nm/a = 0.47746 newton meters torque
11v battery * 10a current = 110w electrical
0.47746 newton meters torque * 225.14747 radians per second = 107.49w mechanical
copper loss: 10a * 10a * 0.025ohm = 2.5w
wheel torque at 10mph @ 110w electrical = 0.47746nm * 2.15 gear reduction = 1.02 newton meters
**summary: 10mph ground speed, 1.02nm wheel torque, 107.5w mechanical, 110w electrical, 2.5w copper loss**

^same ground speed, same voltage battery, same battery current and motor current, different gearing & **the higher kv appears more efficient**… it would seem if the 100kv is at constant speed @ 10mph from the load, with the same ground speed & load the 200kv is still accelerating because there is more torque at the wheel…
[/quote]

^in this example, for the same km but higher kv motor to draw the same current at the same effective voltage at the same ground speed, the higher kv motor must spin at more than double the angular speed of the lower kv motor (thanks to gearing), but the higher kv motor at same current has exactly half the torque as the lower kv motor, but half the torque & more than double the angular speed means the higher kv motor (same km) is actually generating more mechanical power with lower losses for the same input power, and therefore the higher kv motor is more efficient for the same km, when properly geared for the mechanical load.
```

---
## \#83 Posted by: Hummie Posted at: 2018-04-08T15:39:41.067Z Reads: 77

```
@professor_shartsis (professor of ...)


the values you plugged in you have the winding resistance as a fourth of the value of the other not half which I think would make sense...double the turns double the resistance.   and the Io should be the same I believe if it's taken at the same rpm

http://powerditto.de/indexditto.html

https://translate.google.com/translate?sl=auto&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fpowerditto.de%2Findexditto.html&edit-text=&act=url

heres a page I recently got that has a lot of links.  pages and pages.  it does explain how a higher kv motor will have more power similar to your explanation somewhere in one of the links.  speed is a cheap addition to the motor with less losses even if the same copper volume in the motor.
```

---
## \#84 Posted by: Hummie Posted at: 2018-04-08T15:45:27.443Z Reads: 74

```
don't think we have to worry about skin effect at our frequencies though right?




@SimosMCmuffin 
[quote="SimosMCmuffin, post:78, topic:49277"]
Well, the further the motor is being run from it’s no-load speed, the more amps you have to give it (hence it’s further from it’s no-load speed), which directly equate to more losses just in the windings due to their resistance
[/quote]

this makes sense as a reason why greater torque is more inefficient following I2r
```

---
## \#85 Posted by: professor_shartsis Posted at: 2018-04-08T16:22:53.046Z Reads: 74

```
[quote="Hummie, post:83, topic:49277"]
**the values you plugged in you have the winding resistance as a fourth of the value of the other not half which I think would make sense…** double the turns double the resistance.   and the Io should be the same I believe if it’s taken at the same rpm
[/quote]


yes, half the turns half the resistance... double the cross section area of the wire (for same copper volume) and half the resistance again for the same km. 1/2 * 1/2 = 0.25

Io is measured at the maximum unloaded angular speed of the motor.
```

---
## \#86 Posted by: Hummie Posted at: 2018-04-08T16:26:23.893Z Reads: 72

```
makes sense with the 1/4 resistance and halving twice thanks

 ive seen the Io taken at different speeds but if it's at the maximum speed of the motor it will be more than double for the double kv as the motor would be going double the speed and the eddy current being exponential based on speed
```

---
## \#87 Posted by: Bjork3n Posted at: 2018-04-08T18:48:08.625Z Reads: 73

```
I currently run motormax 60A and battery 30A. 
While there be any benefit raising motormax to 80A?
It's a dual 6355 190kv setup (torque motors)
```

---
## \#88 Posted by: professor_shartsis Posted at: 2018-04-08T18:55:23.487Z Reads: 73

```
[quote="Bjork3n, post:87, topic:49277"]
While there be any benefit raising motormax to 80A?
[/quote]


~%33.3 greater torque until you reach the 30a battery amps limit at higher rpms.
```

---
## \#89 Posted by: Deckoz Posted at: 2018-04-08T19:01:22.543Z Reads: 72

```
As @professor_shartsis said more 🚀🚀🚀 sauce in low rpms until you reach your battery amp limit. Basically better low end acceleration.
```

---
