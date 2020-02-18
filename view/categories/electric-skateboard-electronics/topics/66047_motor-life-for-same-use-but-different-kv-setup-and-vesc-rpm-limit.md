# Motor life for same use but different kv setup and VESC RPM Limit

### Replies: 28 Views: 465

## \#1 Posted by: thetechtrader Posted at: 2018-08-25T17:09:45.746Z Reads: 94

```
I can't seem to figure this out no matter how much I read and was hoping someone can help?

Assume two motors are the same factory, same size, only KV is different, which motor would last longer and be under less stress using a high powered VESC setup V200S ESC handles up to 18S.

I'm wondering which KV motor will handle running at constant higher amps without damage/overheat of coils?

Setup #1
56114 inrunner, **300kv**, operation volts from 54v drawing 120A - 75v drawing 97A, RPM limit set at 14,500 RPM

Setup #2 
56114 inrunner, **600kv**, operation volts from 54v drawing 120A - 75v drawing 97A, RPM limit set at 14,500 RPM
```

---
## \#2 Posted by: Hummie Posted at: 2018-08-26T02:17:01.434Z Reads: 77

```

but youre just looking for motor "life".  motors should last a very long time as long as they dont get too hot to ruin the magnets.  magnets lose their magnetism very slowly over time.  you can replace bearings and the insulation on the magnet wire is rated to probably thousands of hours at whatever temp you would put them to. 
your gearing will likely have a much shorter lifespan than the motor.  maybe get steel pulleys and belts
```

---
## \#3 Posted by: thetechtrader Posted at: 2018-08-26T02:23:09.850Z Reads: 72

```
Thank you, this is for a jet surfboard, full throttle would be 14,500 RPM then cruising around 10,000 RPM.
Its direct drive so we cannot use gears. So I was wondering if higher KV would have thicker copper wires and handle the current better than a low kv with thinner wires?
```

---
## \#4 Posted by: Hummie Posted at: 2018-08-26T02:24:31.472Z Reads: 65

```
it takes double the amps to get the torque with the kv being double and ultimately a motor with 200kv and 10amps vs a motor with 100kv and 50amps will pretty much have the same heat and same performance
```

---
## \#5 Posted by: thetechtrader Posted at: 2018-08-26T02:27:40.172Z Reads: 67

```
You mean 100kv and 20A I take it?
So it would really come down to the lower KV having a better/slower/smoother throttle response vs higher kv that would jump to full speek fast then, and heat/performance is about the same no matter kv?
```

---
## \#6 Posted by: Hummie Posted at: 2018-08-26T02:30:57.205Z Reads: 63

```
you should plug some options into the grin motor simulator. you can search for it.   the efficiency will go down if youre not riding close to the max speed of the motor based on the voltage and kv.  so you could go with a super high kv motor and limit the rpm but it will be inefficient.  get the kv and voltage that will get you to just the top speed you want to go but no further.

and when you compare the results on there and it shows maybe 90 percent eff with one motor vs another at maybe 92 percent, that seems small but its a 20percent increase and that's a lot
```

---
## \#7 Posted by: thetechtrader Posted at: 2018-08-26T02:33:25.365Z Reads: 58

```
yes, this is what im trying to figure out, but I dont know how or where to learn/figure it out.
```

---
## \#8 Posted by: Hummie Posted at: 2018-08-26T02:36:17.081Z Reads: 56

```
the speed you will want to spin the motor you mean and what would be ideal?  i guess you'd just have to try it and hard to guess at that with a prop and water and all.   maybe its a very different situation with that vehicle as youre not really NEEDING the torque as you do on a board and it could spin up slowly or something.   i have no idea.
```

---
## \#9 Posted by: Hummie Posted at: 2018-08-26T02:38:11.947Z Reads: 56

```
and ud want to pick a prop for certain rpm too i think
```

---
## \#10 Posted by: thetechtrader Posted at: 2018-08-26T02:38:22.441Z Reads: 55

```
Well, I have a RPM sensor, so I would just need to know the most used RPM for cruising then we would run some numbers in that simulator to find the best motor kv for our volt setup?
```

---
## \#11 Posted by: thetechtrader Posted at: 2018-08-26T02:39:25.825Z Reads: 56

```
We do have the impeller, now we just need to get the most efficient motor for these RPMs
```

---
## \#12 Posted by: Hummie Posted at: 2018-08-26T02:43:16.029Z Reads: 51

```
figure what you can and then write it up here and maybe i could be of help.  i think the best help i could be would be to run you through the grin motor simulator so you can visualize what im saying.  what im saying is pretty one dimensional and your vehicle is multifaceted in terms of what it would maybe need to take into consideration.  but if you pm me and get on the grin simulator. . or call me while youre on it id help you with that.
you'd have to explain more the loads and speeds and stuff.
```

---
## \#13 Posted by: thetechtrader Posted at: 2018-08-26T02:45:43.221Z Reads: 48

```
Re-reading this, I think I get it, and knowing my running RPMS with sensor This give me a good idea of the KV motor to use I think.

I will take you up on that offer once we do more testing over the next week and your walking me through it would be amazing and greatly appreciated Hummie! Thanks for the offer, ill circle back after more testing with new parts that arrive Monday and we can attack this in a 1-2 weeks. Cheers!

Chris V.
```

---
## \#14 Posted by: Jmding Posted at: 2018-08-26T06:53:40.020Z Reads: 46

```
If you gear both motors to the same top speed (they will also produce the same torque), the higher kv motor will have lower internal resistance and generate less heat, and probably more durable. However, due to the higher motor rpm, it may wear out motor bearings faster (maybe...), it may exceed VESC erpm limits, and you may have difficulty fitting the gearing without hitting the ground
```

---
## \#15 Posted by: Hummie Posted at: 2018-08-26T07:27:52.304Z Reads: 45

```
I agree the higher kv will have less electrical resistance and with gearing it would produce less heat in the windings but at some point spinning faster wont be a benefit as the faster the motor spins the more lost energy and heat is produced in the iron or other conductive materials through eddy currents and hysteresis.  since he's doing a direct drive on a jet surfboard he will be able to spin the motor much faster than us as he doesnt have the physical constraints of gearing so he can spin at an optimum speed that finds the balance between the copper losses and the iron losses, unlike what we do, and that will be the most efficient speed the motor can run at and therefore that will be the most powerful speed.  but you cant always be at that speed on whatever vehicle and  there's loads at different speeds that need to be thought of.   for example if he does a super high kv and optimized for efficiency at some high speed...it might take huge current to get up to that speed and overall not ideal.   
its hard to figure the iron losses and probably best to just do unloaded testing at high speeds to see what the temp increase is.  but if youre on the water and will have water cooling it doesnt matter how inefficient you are if you can rid the motor of the heat.  and maybe youd just have a slightly decreased range as the drawback
```

---
## \#16 Posted by: professor_shartsis Posted at: 2018-08-26T13:47:15.181Z Reads: 41

```
[quote="thetechtrader, post:1, topic:66047"]
Assume two motors are the same factory, same size, only KV is different, which motor would last longer and be under less stress using a high powered VESC setup V200S ESC handles up to 18S.

**I’m wondering which KV motor will handle running at constant higher amps without damage/overheat of coils**?

Setup #1
56114 inrunner, **300kv** , operation volts from 54v drawing 120A - 75v drawing 97A, RPM limit set at 14,500 RPM

Setup #2
56114 inrunner, **600kv** , operation volts from 54v drawing 120A - 75v drawing 97A, RPM limit set at 14,500 RPM
[/quote]

since you are using a propeller with no gearing at 14,500rpm, you will need the same amount of torque out of both motors to sustain this rpm...

if they are the same KM or size constant, the 600kv has 1/4th as much electrical resistance as the 300kv, because the 600kv winding wires are half the length but twice the cross section area.

to solve this let's assume we want to reach & sustain 14,780 motor rpm on 2 electric skateboards (300kv vs 600kv), both with the same 2.05:1 gear ratio & 83mm tires... this is 70mph in the graphs below.

the 600kv has half the torque per amp compared to the 300kv motor, so the 600kv needs twice as much motor current to produce the same torque, but since the 600kv motor has 1/4th the electrical resistance of the 300kv motor, it turns out that both motors produce exactly the same amount of ohmic heating (blue line, bottom middle chart -- ohmic heating watts, 1 motor).

since both motors are generating the same amount of heat, both motors should last equally as long. and in fact, both motors draw the same amount of amps from the battery to produce the necessary torque to sustain 14,780 motor rpm (red line, bottom right chart -- battery amps).

but in the controller it's a different story... take a look at the motor current (blue line, top left chart, motor amps). it takes 290a motor current to sustain 14,780rpm with the 600kv motor vs 145a motor current to sustain 14,780rpm with the 300kv motor.

even though the 600kv motor has 1/4th the electrical resistance compared to the 300kv motor and therefore produces the same motor heating for the same torque at the same rpm, **the motor controller's electrical resistance will be the same regardless of which motor you choose. you have to send twice as much motor current through the controller to sustain 14,780rpm with the 600kv motor, and twice as much current through the 600kv controller will heat the 600kv controller 4 times faster according to the copper loss equation I^2R=W**.

So in summary while both 300kv and 600kv **motors** should last equally as long at 14,780rpm, **you'll be heating up the controller 4 times more quickly with the 600kv motor**.

75v battery, 2.05:1 gear ratio, 83mm tire, (300kv, 0.004ohm, 145a motor current limit) vs (600kv, 0.001ohm, 290a motor current limit)

https://image.ibb.co/e7kDyU/300kv_vs_600kv.gif
```

---
## \#17 Posted by: thetechtrader Posted at: 2018-08-26T14:04:35.923Z Reads: 30

```
Fantastic! Thank you!
Yes, the controller heat is something that must be managed and knowing the higher kv setup jacks up the heat more for this setup is one of the golden nuggets I was hoping to learn/figure out.
```

---
## \#18 Posted by: professor_shartsis Posted at: 2018-08-26T15:28:43.698Z Reads: 32

```
[quote="Jmding, post:14, topic:66047, full:true"]
If you gear both motors to the same top speed (they will also produce the same torque), the higher kv motor will have lower internal resistance and generate less heat, and probably more durable. However, due to the higher motor rpm, it may wear out motor bearings faster (maybe…), it may exceed VESC erpm limits, and you may have difficulty fitting the gearing without hitting the ground
[/quote]

@thetechtrader-- but as @Jmding pointed out if you double the gear reduction ratio on the higher kv motor, and let the 600kv spin twice as fast -- 29,560rpm with the 600kv instead of 14,780rpm with the 300kv, and use the same 145a motor current on both... then the controller generates the same heat for both options, the 600kv motor generates 1/4th as much heat, and consumes less amps from the battery for the same final propeller power and rpm. in this case the 600kv motor's bearings might wear out more quickly, while less heat is produced in the 600kv windings.

https://image.ibb.co/g5XDhp/300_vs_600_2_1.gif
```

---
## \#19 Posted by: thetechtrader Posted at: 2018-08-26T15:36:00.618Z Reads: 27

```
Interesting, thank again. Our focus is a on a direct drive system to avoid the added weight, reduction gears, cost etc..  the reduction gears for our situation are about $400 USD. There is trade off, lower cost, less to breakdown, less weight, shorter length, but we will lose some efficiency. I just want to be sure we select the best motor option for durability, ESC and wire heat.
```

---
## \#20 Posted by: TowerCrisis Posted at: 2018-08-26T15:55:00.700Z Reads: 30

```
I'm guessing the 14500 number came from the max prop speed before cavitation occurs?

I'm sure you understand what's your best option, but to summarize the solution to anyone reading all this technical stuff:

You want the lowest KV motor you can achieve while still reaching your calculated max RPM target. KV will not affect motor heat given the same torque requirements, but it will affect motor controller heating. Lower KV is good for sustaining higher power draw for longer periods because it requires less motor amps, which will heat up the esc less. This only applies to a situation where both motors have the same gearing / direct drive.
```

---
## \#21 Posted by: Hummie Posted at: 2018-08-26T17:32:16.722Z Reads: 26

```
![Capture|690x372](upload://tmrn47aMbRjk2mL87gBulwctzib.JPG)

this graph shows two systems which are the same except one has a motor with double the kv and that system is showing to have almost double the losses at this speed and output.  the losses accounted for with the simulation are esc and motor.  what percent of the losses do you think are in the esc and what are in the motor?
```

---
## \#22 Posted by: professor_shartsis Posted at: 2018-08-26T22:04:12.023Z Reads: 18

```
[quote="Hummie, post:21, topic:66047"]
what percent of the losses do you think are in the esc and what are in the motor?
[/quote]

both motors have the same copper losses if the km (mass constant), torque and rpm are the same, so in the higher kv system, 100% of the “extra/additional losses” would be in the ESC... in other words the circuitry in the esc of the doubled kv motor is producing 4 times as many watts of heating as the other esc, since it’s using twice as much motor current to produce the same torque with the doubled kv motor.

also @Hummie  it isn’t clear in your simulation whether the doubled kv motor has 1/4th the electrical resistance of the other motor as would be the case if the km of both motors is the same.
```

---
## \#23 Posted by: Hummie Posted at: 2018-08-26T22:47:35.214Z Reads: 16

```
So it seems and the" motor amps" are about double w the x2 kv.   but "total wattage " shows higher.  Don't remember seeing that term on there defined.  That's a lot of heating the esc no?
```

---
## \#24 Posted by: Jmding Posted at: 2018-08-27T03:51:49.812Z Reads: 15

```
If you're married to the specific impeller, which implies a specific range of rpms, and you dont have the option of gearing, then you will want to pick a motor such that Kv * battery_voltage = max rpm.  Furthermore, you practically always want to run as high a battery_voltage as possible (given your ESC, space, and weight constraints) as this will mean lower current draw, and less ohmic heating.

If you aren't married to the chosen impeller, I'd say you should really talk to the quad-copter / airplane / boat guys, as they will know a lot more about picking a motor+impeller combo.  You say you dont have gearing, but I get the feeling that impeller diameter is very similar to gearing: higher diameter = more water pushed per rpm = high torque, low speed motor.

Edit: on second thought I think you're going to need to do the math. This problem is enough outside our typical domain, that I dont trust my intuition.  The big difference is that in our application, the amount of torque it actually takes to sustain top speed on flats is pretty low.  We're not moving fast enough for aerodynamic drag to overpower our motors.  But in your application, you have to overcome hydrodynamic drag of the board AND the torque it takes to just spin an impeller in water, in addition to aerodynamics.  Frankly, 14500 rpm sounds like a LOT in water, I'm guessing its going to take a LOT of torque to hold speed, and I'm not sure our motors will be able to sustain that power output without going above the typical 10-12s voltages.  Out of curiosity, do you know what the torque required to spin that impeller is, and how it varies as a function of rpm?  On the electromechanical side, motor torque = Kt * Current, and Kt = 1/Kv.  So higher Kv motors also produce less torque per Amp.  If you pick a motor with a relatively high (for eskate anyway) ~325 Kv (which should hit 14500 rpm @ 12s under no-load conditions), the Kt might be so low that to get enough torque to actually hit that rpm figure in water, you'll draw so many amps that you'll definitely fry the ESC if not the motor.  You want to pick a high Kv motor to spin the impeller at efficient speeds, but if you go too high you wont get enough torque to actually spin the impeller at the desired speed.  Its a maximization problem that doesnt exist in our skateboard applications, so I doubt any of us have done the homework yet.

Also in answering your original question about Kv and max amps, yes, you are right that low Kv motors have thinner, longer wire and more internal resistance.  Roughly speaking, motor wire resistance should scale with Kv^2.  Since max current is mostly a function wire heating, which is a function of internal resistance, max current should scale with 1/Kv^2.  Most of our motor manufacturers dont reflect this in their technical specs, but I think those specs are probably pretty made up anyway.  A higher Kv motor will be able to handle more current.
```

---
## \#25 Posted by: Jmding Posted at: 2018-08-27T04:00:55.759Z Reads: 11

```
@Hummie do you have a good way to estimate the losses at the ESC?  For comparison, a 10s board with dual 6354 motors, geared to 50 km/h max speed, climbing a 10% hill (steady speed, not accelerating ) will draw *ballpark* 40A total (20A per motor), and have motor internal resistance 0.039 ohm.  That comes out to 20A^2 * 0.039 ohm = 15.6 Watts of ohmic heating.  My guess is that ESC inefficiencies will be negligible in comparison, but frankly I have no idea.
```

---
## \#26 Posted by: Hummie Posted at: 2018-08-27T05:00:00.722Z Reads: 12

```
i assume the vesc wattage measurement is just what is coming from the battery before its losses.  maybe not.  but if so then maybe possible to add a wattmeter on each phase?  i dont know how people isolate esc and motor losses and thats a guess.  
i'm curious how your motor will show on the grin simulator!  you can adjust the wheel diameter, and go into the motor selection and at the bottom there is "custom" and plug in resistance and a bunch of iron loss stuff and other things you can get off the vesc tests or running in real time, even a gearing option.   wish i had a motor running to see.  also can even adjust frontal area to incorporate aerodynamics somewhere on there.  this tool is pretty awesome for boards too it seems.  **super excited to see if i can beat its predictions at 30mph with my best aero tuck**  and see how we stack up verse bikes at speed in a tuck.  going for lowest wattage used at 30mph on a flat.   and then you have to lay down and go for the record.

http://www.ebikes.ca/tools/simulator.html
```

---
## \#27 Posted by: Jmding Posted at: 2018-08-27T05:02:30.652Z Reads: 12

```
That's a really cool simulator, but I haven't educated myself on iron losses to configure custom motors correctly yet. Next in line I guess
```

---
## \#28 Posted by: Hummie Posted at: 2018-08-27T05:06:27.026Z Reads: 13

```
resistance (i think phase to phase, if not then double it) is on the vesc foc test, as well as the inductance, and the others you can get in the real time screen going full speed doing the no load speed, and get the current you see then, and some other slower speed see what current is happening then.![image|690x405](upload://8U8mC2hBvxQViUG565oZ99ZJvkg.png)
```

---
