# Help me understand how amperage works with acceleration

### Replies: 21 Views: 1231

## \#1 Posted by: TheFluffiest Posted at: 2018-04-11T22:24:49.011Z Reads: 218

```
So, I understand that more amps=more acceleration. But, once the motor reaches its max rpm, will the amperage go down again? I've seen people say they cruise around 5 amps, which seems really low to me. 

I use 8s1p 5000mah lipo batteries, and can ride for roughly 30-45 minutes before the battery dies. So, 5Ah/.5 hours=10amps on average. Is this an accurate way to do it? 

If this is the case, could I theoretically put my motor amps really high (70-80 amps?) because it will only be that way while accelerating? With that amount of torque, I can't imagine accelerating for more than a couple seconds. Will this hurt the vesc?
```

---
## \#2 Posted by: E1Allen Posted at: 2018-04-11T22:35:15.310Z Reads: 211

```
Yes the amperage will decrease. Extra Force (amps) are required to increase speed.  Once speed is constant Force is reduced so less amps.

So without Bluetooth telemetry I would use any app on your phone or whatever to get an accurate distance traveled.  Then use the mAh going back into the battery to determine average.  Your motor has a amp limit.  What motor are you using.  In general you can increase motor amps so long as it's within limits of the motors.  The concern is operating the motor for long periods above it's rated wattage.

What vesc are you using?
```

---
## \#3 Posted by: ShutterShock Posted at: 2018-04-11T22:36:25.249Z Reads: 200

```
Your assumptions seem to be mostly correct.  And I suppose your amp hour calculation is slightly accurate, but you would be assuming a constant drain in that scenario, in reality, it will be stop and go, which will probably result in a longer overall ride time.

That cruise is probably about right, but also depends on hills, rider weight, wheels, and a number of other variables.  But for the most part, my dual drive board runs about 10-12WH/mile

And your final statement is correct.  However, it is likely you will never reach that high of a number. You should also know that the VESC is rated for 50 battery amps throughput, which is very different from motor amps.  My VESCS pull a max of about 60 amps, together, on max acceleration.
```

---
## \#4 Posted by: TheFluffiest Posted at: 2018-04-11T22:49:38.508Z Reads: 182

```
@E1Allen The motor I use is a KEDA 6364 190kv motor. Hobby King rates it at 90amps, 2000 watts so I'm not concerned about putting too much through the motor. The vesc I have is the older enertion 4.12 vesc. Not the VESCX or FOCBOX, just an older VESC. I bought it off a guy on the forum that never ended up using it. 

@ShutterShock That was just assuming cruising at 22-25mph. That is what I am USUALLY at (according to strava) so I would say it is accurate enough for the purpose of discussion. Vedder's website says it can take up to 240A for a few seconds, so i was thinking it would be ok to run it at high amps for a bit.
```

---
## \#5 Posted by: E1Allen Posted at: 2018-04-11T22:53:39.381Z Reads: 164

```
Probably safe to up the motor amps.  You can take the Max wattage then divide by your volts to get the Max number of amps required to reach the Max wattage of the motor.  For you around 66 motor amps
```

---
## \#6 Posted by: ShutterShock Posted at: 2018-04-11T22:55:22.057Z Reads: 151

```
Yeah you're fine, nothing to worry about.
```

---
## \#7 Posted by: TheFluffiest Posted at: 2018-04-11T23:00:26.694Z Reads: 147

```
@E1Allen I had it at 60, I will push it up to 66. Thanks!

What are you guys running it at @ShutterShock @E1Allen?
```

---
## \#8 Posted by: E1Allen Posted at: 2018-04-12T00:13:30.264Z Reads: 141

```
80 in bursts probably won't hurt.  I think mine are 75 but it doesn't reach it in dual setup.  You may or may not notice a difference. You can try going up in increments of 5a to find a good number that works.
```

---
## \#9 Posted by: ShutterShock Posted at: 2018-04-12T00:54:26.466Z Reads: 137

```
I run my motor values  and +80 and -80, respectively.
```

---
## \#10 Posted by: Cobber Posted at: 2018-04-12T01:42:43.021Z Reads: 129

```
[quote="TheFluffiest, post:4, topic:51983"]
The motor I use is a KEDA 6364 190kv motor. Hobby King rates it at 90amps, 2000 watts
[/quote]

that has to be a peak amp rating, not cont. the 2000w though is likely cont.

watts divided by volts will equal amps
ie.
2000w/37v = 54a
2000w/44.4v = 45a
the only real question is what voltage are the motors rated at as that will tell you through duduction  what the cont. amp rating is

edit: did a quick search your motor has been rated at 10s or 37 nominal volts, so 54a cont. rating :)
i'd set your AC to 90 and your MC to 54 if you want to run on specification
```

---
## \#11 Posted by: TheFluffiest Posted at: 2018-04-12T02:39:09.568Z Reads: 118

```
For some reason my brain isn't working and I'm not at my computer so I can't check, but what does AC stand for in this case? I'm guessing MC is motor current...
```

---
## \#12 Posted by: Cobber Posted at: 2018-04-12T02:40:09.442Z Reads: 115

```
Absolute Current
```

---
## \#13 Posted by: SimosMCmuffin Posted at: 2018-04-12T10:12:08.945Z Reads: 108

```
[quote="Cobber, post:12, topic:51983, full:true"]
Absolute Current
[/quote]

This is a terrible acronym for AC, which in any electronics or electric context means "Alternating Current". I would suggest it might just be better to use the terms "battery current" and "motor current", just to avoid confusion with any real AC systems.
```

---
## \#14 Posted by: professor_shartsis Posted at: 2018-04-12T12:48:08.551Z Reads: 99

```
[quote="TheFluffiest, post:1, topic:51983"]
But, once the motor reaches its max rpm, will the amperage go down again?
[/quote]

[quote="TheFluffiest, post:1, topic:51983"]
If this is the case, could I theoretically put my motor amps really high (70-80 amps?) because it will only be that way while accelerating?
[/quote]

If you take a look at this chart from a different thread (representing 30a battery limit & 90a motor limit), it may visually give you some idea of the factors limiting the motor current at higher rpms (blue and black lines, top left chart)...

[quote="professor_shartsis, post:652, topic:25251"]
based on 78kv, 83mm tire, 1:1 gearing (hub), 0.057ohm, 46v pack, 30a battery limit per motor, 90a motor limit per motor:
[/quote]

https://image.ibb.co/bKsnn7/54151d6e32a232b6687333983d5e443b9c1422ed.jpg

^notice at 0rpm, the battery amps are limited below 30a by the 90a motor amp limit setting, and at higher rpms, the motor amps are limited below 90a by the 30a battery amp limit setting (blue and black lines, top left chart).

at higher and higher rpms, the same number of battery amps (software setting limited) results in less and less motor amps... or you could say the same number of motor amps results in more and more battery amps as rpms increase... & this is a result of the increasing back emf voltage as the rpm increases. (the bemf voltage works in opposition to the battery pack voltage & is produced in the motor windings as a result of the spinning magnets on the rotor.)

battery current and motor current drop to 0a at the no load rpm because the back emf voltage surpasses the battery pack & esc’s maximum effective voltage above this speed (red & yellow lines, top left chart). In reality when forcing the motor above no load speed, the current reverses direction leading to a braking sensation & charging of the battery pack, even at full throttle.
```

---
## \#15 Posted by: Cobber Posted at: 2018-04-12T12:55:28.372Z Reads: 77

```
The number of references on this forum alone discussing VESC settings (in this context: BC, MC & AC and are all in use at the same time) where "AC" is described as Absolute (max/maximum) Current, where by it acts as a over current protection are too numerous for me to count for you MC'y... :no_mouth:
```

---
## \#16 Posted by: MaxMalouf Posted at: 2018-10-25T03:41:17.992Z Reads: 56

```
@Cobber I need some help understanding this, 
say if you have a board that uses a 4S setup and is capable of 80a(1,184watts). Is the acceleration faster than a 10s capable of  32a (1,184watts)? 
the wattage is the same so is the acceleration the same or is the 4s way better acceleration wise?
```

---
## \#17 Posted by: professor_shartsis Posted at: 2018-10-25T05:37:01.897Z Reads: 54

```
[quote="MaxMalouf, post:16, topic:51983"]
if you have a board that uses a 4S setup and is capable of 80a(1,184watts). Is the acceleration faster than a 10s capable of 32a (1,184watts)?
the wattage is the same so is the acceleration the same or is the 4s way better acceleration wise?
[/quote]

@MaxMalouf with 4S vs 10S, the acceleration is the same (assuming the motor current limit setting is the same), and more battery current is drawn from the 4S battery than the 10S battery to achieve the same motor current and thrust at the same speed. the 4S also has much lower top speed...

notice the thrust is the same at 5mph (purple line, bottom left chart, vehicle thrust pounds, 2 motors), but far more amps are drawn from the 4S battery at 5mph to achieve the identical thrust (red line, bottom right chart, battery amps 1 motor). also the motor current for both systems is the same at 5mph (blue line, top left chart, motor current).
https://image.ibb.co/ea9bmV/4s-vs-10s.gif
```

---
## \#18 Posted by: MaxMalouf Posted at: 2018-10-25T07:33:59.776Z Reads: 52

```
@professor_shartsis Wow that's really cool. What program did you use to do this?

basically, I had a thought that you could have some sort of system like the Jaykay e trucks have: https://www.electric-skateboard.builders/t/jaykay-e-truck-statement/25698

they switch from 2s2p (for acceleration) to 4s1p (for top speed)
they somehow use some sort of switch in the circuit board to do this, I have no clue.
but I was thinking, what if someone made a system like this but on a much larger scale with 42 cells instead of 4. It could switch from a 6s7p pack at low speeds to provide easy acceleration without straining the battery and then for higher speeds, it switches to a 14s3p. 

I have very very little knowledge on electronics but something like this would be a cool thing to do. 
Does it even work? or is this just completely pointless??
```

---
## \#19 Posted by: nuttyjeff Posted at: 2018-10-25T08:03:46.237Z Reads: 49

```
If it could run at 14s to begin with, i would just set it at 14S (for a higher efficiency) and limit my speed via ERPM.
```

---
## \#20 Posted by: professor_shartsis Posted at: 2018-10-25T15:35:32.446Z Reads: 43

```
@MaxMalouf lowering the voltage of the battery while adding cells in parallel by itself won't improve acceleration. you'd have to make other changes like lowering the kv of the motors, increasing the motor current limit, increasing the gear ratio, or decreasing the wheel diameter to increase the acceleration.
```

---
## \#21 Posted by: MaxMalouf Posted at: 2018-10-25T23:35:16.732Z Reads: 36

```
@professor_shartsis alrighty, what was the program you used to graph all that information i would love to test that stuff out
```

---
