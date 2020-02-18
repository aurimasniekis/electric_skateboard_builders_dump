# Motor Comparison Database

### Replies: 18 Views: 1271

## \#1 Posted by: akelly Posted at: 2018-05-26T04:54:53.811Z Reads: 288

```
I'm coming from the ebike world and looking at what motors to buy for a skateboard, and I haven't seen any good empirical comparisons between the different motors available. People say things like "these motors are super powerful" or "I can climb a 100% grade hill no problem," which are horribly inconsistent, so inspired by [this thread comparing Raptor 2 hubs to Hummie hubs](http://www.electric-skateboard.builders/t/raptor-2-hubs-alternatives/56649/17), and [this ebike motor comparison database](https://endless-sphere.com/forums/viewtopic.php?f=30&t=65757), I want to build a spreadsheet of actual scientific numbers for as many motors as possible.

Fortunately, you all have fancy computers attached to our motors that can measure all the necessary parameters called VESCs. So can you guys post screenshots in this thread from the VESC tool for your motors, and I'll add them all to the spreadsheet? What I need is the Motor Resistance from the FOC tab, and the measured kV of the motor. To measure the kV, remove the belt if you use one, then run the motor at full speed, and type `kv` into the terminal several times so we can average the numbers, and it'll return the kV in eRPM/V, and then you divide by the number of motor pole pairs (usually 7) to get the actual kV. A mass number for the motor would be nice to have as well, but not necessary.

With the motor resistance and kV, we can calculate kM, the motor size constant, a measure of how much torque the motor can produce for a certain amount of heat output. Larger motors with more copper have a higher kM, so they will heat up less and have a higher current rating. But unlike current ratings, the kM is a more fair comparison because it doesn't depend on things like airflow or motor kV, and can be measured much more easily. With the mass of the motor, you also know the kM/kg, a measure of how lightweight the motor is built for its power level.

[So here's the spreadsheet!](https://docs.google.com/spreadsheets/d/1MO_MTQGfHK8qPuBR74QlUKQ68MMGChDq6vC7X30unAk/edit?usp=sharing)

I added numbers for all the motors I could find, which unfortunately doesn't include any eskate hub motors. Initial results show that the Turnigy SK3 6374-149kV blows all the other belt drive motors out of the water. Like, the numbers Hobbyking gives are so good I'm suspicious of them. Let's verify those numbers, and measure some hub motors!
```

---
## \#2 Posted by: evoheyax Posted at: 2018-05-26T06:00:41.502Z Reads: 270

```
The numbers of the raptor 2 hubs are interesting when compared to hummies v4 hubs. Not sure if I can legally disclose the numbers, but the raptor 2 does appear to have slightly lower resistance, likely due to the larger diameter stator. Hummies hubs have a longer stator though, but larger diameter yields more space for copper. They both have way more power than most people need if used in high enough wattage board. Can't wait to ship so we can get real world comparisons.
```

---
## \#3 Posted by: akelly Posted at: 2018-05-26T06:24:34.938Z Reads: 250

```
Yeah both of those motors seem to have crossed over the line of "big enough." I do wonder how much better they are than the Chinese hub motors though. And winding resistance varies a ton based on what kV you wind the motor with, which is why I'm using kM instead. It's curious you can't share numbers though, considering the Raptor 2 is shipping now and anyone with one can go measure it.

Also I just realized that the VESC resistance measurement will include the resistance of the FETs and PCB traces, and so will come out higher than a proper measurement of the motor with the right equipment. Perhaps we can do both with the same motor and use that to correct the measurements other people do with that speed controller model.
```

---
## \#4 Posted by: evoheyax Posted at: 2018-05-26T21:42:31.487Z Reads: 203

```
[quote="akelly, post:3, topic:56817"]
I do wonder how much better they are than the Chinese hub motors though.
[/quote]

Well that is a loaded question. My understanding is most are rated from 150 watts up to 1250 watts. I haven’t seen any hubs from China that can do more than that. We’re finding doing double that is not an issue and they barely get warm at 2500 watts per motor on dual drive. Heat will be a big difference. And it’s not double the motor size half the heat. It’s more of an exponential function. I’m seeing less than a 1/4th of the heat from the v1 hummie motors that were half this size.

The other difference is serviceability. My understanding is the only China hubs that don’t have issues with out slipping urathene glue them to the hub. We have a way to easily replace wheels, with no issues of slipping or dirt getting in like the raptor 2 hubs have. Even if you blew out the winding somehow, it’s only $30 in parts for us to fix cause we can reuse everything but the stator and wire in that case. Mess up magnets? Well send you a new bell and you can replace it in 2 minutes  or less with simple tools that cost less than $50. That is another difference between China hubs and ours/raptor 2 hubs.
```

---
## \#5 Posted by: b264 Posted at: 2018-05-26T22:01:36.299Z Reads: 187

```
[quote="akelly, post:1, topic:56817"]
Turnigy SK3 6374-149kV
[/quote]

It is a very popular motor BUT it's not 6374 (63mm x 74mm) and it's not sensored, both of which hurt its practical usage
```

---
## \#6 Posted by: Deodand Posted at: 2018-05-26T22:11:07.271Z Reads: 188

```
Could we potentially add columns to this for rated amps as well? Then we could calculate some stuff like max cont. Torque etc with motor kv.

For hub motor designs it will be pretty important to achieve a certain amount of continuous torque for hill climbing etc. I suppose Km in some ways captures this idea but not completely since thermal dissipation plays a role.

I might also suggest adding the inductance measurement and flux linkage measurement from the vesc. Flux linkage can help us validate the kV measured (math relation to kv). Inductance seems less immediatley useful but when building a database its good to add extra data if it doesn't come at extra cost.

I started compiling a similar database recently. I have found that most listed specs on the website tend to be pretty far from vesc-measured values. We should have a marker for values measured with vesc and use them as a consistent baseline for comparison. 

I'll add some motor data from what I was compiling in a bit.
```

---
## \#7 Posted by: akelly Posted at: 2018-05-28T00:56:52.236Z Reads: 163

```
Yes the max power depends a lot on the thermal dissapation, but I really don't trust manufacturer power and current ratings. I think a lot of them are inflated, or are not continuous numbers. And measuring it ourselves is not that simple. And another factor that the kM doesn't take into account is the maximum motor speed. If two motors have the same kM and heat dissipation abilities, then they have the same torque rating, but if one can be spun faster, that's a higher power rating, and I think that compensates for the poor kM numbers on the inrunner motors. Need to see if I can get the math to work out right and come up with a better figure of merit.

I'm not sure how useful flux linkage and inductance would be, but you're right that we might as well include them. I'm not familiar with the flux linkage, but [according to Vedder it's simply a function of kV and the number of poles](http://vedder.se/forums/viewtopic.php?t=131#p693).

Thanks for offering to contribute the data @Deodand, once I replace the DRV on my VESC I'll be able to do the same. I need to figure out where to buy a second one too. The "Data Source" column is for differentiating between manufacturer numbers and community sourced measurements, including what VESC variant was used. And we can also do 4-wire resistance measurements, to see how far off the VESC measurements are.

You're right @b264, the SK3-6374's high kM numbers are even more suspicious given the fact that it's actually a ~~5961~~ 5986 motor, and it has a ring bearing which further reduces the stator size. I find it hard to believe that they fit more copper in it than the Maytech and Eskating 6374's, but I also find it hard to believe they would fudge the resistance number, given how most people just look at the current rating. I'll try to add actual motor dimensions to the spreadsheet though.
```

---
## \#8 Posted by: b264 Posted at: 2018-05-28T01:10:49.610Z Reads: 139

```
[quote="akelly, post:7, topic:56817"]
SK3-6374’s high kM numbers are even more suspicious given the fact that it’s actually a 5961 motor, and it has a ring bearing which further reduces the stator size. I find it hard to believe that they fit more copper in it than the Maytech and Eskating 6374’s, but I also find it hard to believe they would fudge the resistance number
[/quote]

That's nothing, look at this one.  They claim the [Turnigy SK8 6354-140KV Sensored Brushless Motor (14P)](https://hobbyking.com/en_us/turnigy-sk8-6354-140kv-sensored-brushless-motor-14p.html) has a 98 megaohm resistance, which is the same as air.  So essentially, you can just leave the phase wires laying on the carpet and not hook it up to the ESC and it should still work.  Well, according to their numbers anyway.

More likely they have untruths listed.
```

---
## \#9 Posted by: akelly Posted at: 2018-05-28T01:17:55.463Z Reads: 137

```
Hah, that's just a simple typo. I should add that motor though. But it's like Alien claiming their 6374 has a resistance of 0.66, when they probably meant 0.066 Ohms. Which is still high, I would expect something more like 0.04.

I did find [this thread](https://vesc-project.com/node/267) where Roger Wolff shared his VESC numbers for the SK3-6374-149kV and he got 16 mOhm, compared to the suspiciously low 21 mOhm that Hobbyking says. Which is even weirder because I think the VESC resistance should add on the order of 5 mOhm. And calculating from his flux linkage I'm getting 156 kV, which is pretty reasonable.
```

---
## \#10 Posted by: Naysh Posted at: 2018-05-28T01:49:31.697Z Reads: 131

```
I like where this thread is going, we are finally getting some truth to the claims.  We need to include videos to somewhat validate objectivity because anyone can fabricate numbers up.
```

---
## \#11 Posted by: akelly Posted at: 2018-05-28T03:31:19.282Z Reads: 132

```
Yep, the idea is to introduce some actual science into motor selection. Videos of the VESC motor detection might be a good idea, we'll see.

Messing around with the numbers trying to find an approximation for power, the metric RPM^2 * kM^2 seems to work well. If you put a 2:1 gear reduction on the motor, that metric stays the same, as it should for a measure of power, while the kM doubles, as it is a metric of torque. But the margin between motors is massive, for example it's hard to believe that the SK8 6374 is actually 4x more powerful than the SK8 6354. But if you run the numbers for two identical motors in parallel, using RPM^2 * kM^2 you get 2x the power as you should, but RPM * kM would indicate only 1.41x the power. I think this metric should approximate the efficiency of the motor if you only take into account resistive losses and ignore the iron losses and friction losses, maybe we should try to calculate that from scratch and see if they match up.

Edit: Intuitively you would think that a motor geared down 2:1 would have the same torque and kM as two of that motor connected in parallel, but the two motors in parallel would have 2x the power because the RPM is twice as high. But that's not the case. The kM of the motor geared 2:1 is 2x the motor on its own, but the kM of the two motors is in only 1.41x the single motor. So the power using RPM^2 * kM^2 is the same.
```

---
## \#12 Posted by: akelly Posted at: 2018-05-28T04:37:08.079Z Reads: 118

```
I figured out why the power ratings varied so much between motors. For the different kV versions of a motor, whether it's 110kV or 260kV, Hobbyking lists the same 12S maximum voltage. But the only limit on a brushless motor's voltage are how fast it can spin! Obviously a lower kV motor can take a higher voltage, so I calculated the RPM for the highest kV motor in each family at the rated voltage, and then use that as the max RPM for all the motors in that family. So since the 260kV 6354 is rated to 12S (50V max), the 140kV 6354 is actually a 93V max motor, which brings the power in line with what you would expect, 15% below the 6374. Why does Hobbyking do this...
```

---
## \#13 Posted by: Deckoz Posted at: 2018-05-28T05:12:56.366Z Reads: 109

```
If we wanna make a list. What someone needs to do is contact Ryan at miniquadtestbench. Tell him to throw some 15" props on our motors. And make charts.

Either that or someone replicate what Ryan is doing at miniquadtestbench.
```

---
## \#14 Posted by: Deodand Posted at: 2018-05-28T05:38:17.205Z Reads: 115

```
I definitely agree on the lack of ability to depend on rated amps from the manufacturer and agree that a uniform test would be difficult. Km is a nice theoretical compromise. One other thing to mention, I have been doing some work to gather lots of motor data as mentioned before and then rather than a theoretical function I performed some emperical non-linear function fitting based on parameters to find some interesting trends. One that I found was something similar to this:

Rated motor Amps = C1 * 1/( kV ^ 0.6 * Res ^ 0.6) 

C1 being an arbitrary constant. Since its a fit of imperfect data you could assume those 0.6 exponential might be sqrt functions. Maybe a constant of 1/(sqrt(kV) * sqrt(res)) would give a good idea of max cont. amps based on some empirical observations. Ultimately some tests with a thermistor pressed against the windings plugged into vesc and waiting a preset time for throttling to steady state current would be much more accurate. But that is a lot of work to test each motor unfortunately. 

I would suggest we have a separate column for "VESC measured value" and any other type of manufacturer or otherwise measured value. Standardizing our measurement tool would really improve comparison, and the vescs detection routine helps with this. Also maybe we could start spotting trends in how manufacturers define winding resistance as compared to the VESC definition (I think there is a 2/3rds somehwere in the vesc code). Obviously some variance will still exist vesc to vesc but it seems more consistent than any other method we might use.

edit: I see you have different rows for different data gathering, that works fine I suppose. 

[quote="akelly, post:12, topic:56817, full:false"]
But the only limit on a brushless motor’s voltage are how fast it can spin! 
[/quote]


There is also a voltage limit at which the winding insulation breaks down. Additionally there's about a 100-150k erpm limit depending on the motor controller. I think it might be wise to leave a 12s limit calculation since the majority of motor drivers people use in eskate will blow up beyond that. 

But yes theoretically it makes more sense that the power output stay roughly constant, and agree with what you are saying.
```

---
## \#15 Posted by: OlivierDud Posted at: 2018-06-04T09:42:13.839Z Reads: 87

```
The raptor 2 sleeves aren't slipping anymore and there's has never been dust sneaking it's way in there, it's the motor can just slightly eating some urethane from the inside when the sleeves are new, creating urethane dust.
```

---
## \#16 Posted by: Acido Posted at: 2018-06-04T12:01:55.074Z Reads: 76

```
im 95kg and i pushed my single 6374 super hard and it got like 40celsius hot which is nothing
I would say that our limit is a vesc
but dual 6374 should be enough for everyone
```

---
## \#17 Posted by: evoheyax Posted at: 2018-06-04T13:21:31.277Z Reads: 75

```
[quote="OlivierDud, post:15, topic:56817"]
there’s has never been dust sneaking it’s way in there
[/quote]

Someone posted a pic of a small rock getting in there. Maybe the urathene wore away some and then stuff could get in, but I def saw pics of debris getting in there. Mind you, this is the earlier wheels I'm talking about, not the ones with a core now.
```

---
## \#18 Posted by: professor_shartsis Posted at: 2018-06-04T13:46:35.804Z Reads: 69

```
[quote="akelly, post:11, topic:56817"]
Messing around with the numbers trying to find an approximation for power, the metric RPM^2 * kM^2 seems to work well. If you put a 2:1 gear reduction on the motor, that metric stays the same, as it should for a measure of power, while the kM doubles, as it is a metric of torque.
[/quote]

@akelly Can you explain how you arrived at RPM^2 * kM^2 giving an approximation of power & share the formula you used that shows changing the gear ratio changes the KM?

mechanical power = torque in newton meters * angular velocity in radians per second.

torque in newton meters BLDC = KM * sqrt(copper loss in watts)

torque in newton meters BLDC = KT * motor current

copper loss in watts BLDC = motor current * motor current * lead-to-lead resistance in ohms

KT (torque per motor amp)= 60 / (2 * pi * kv)

angular velocity in radians per second = (rpm * 2 * pi) / 60

&

KM (torque per square root of copper loss in watts)=(30 * sqrt(1 / R)) / (pi * KV)
where:
R=resistance in ohms lead to lead
KV=rpm per volt
```

---
