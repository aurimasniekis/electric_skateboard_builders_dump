# My motor controller dev thread

### Replies: 75 Views: 3524

## \#1 Posted by: SimosMCmuffin Posted at: 2016-09-09T09:45:05.362Z Reads: 209

```
I am currently writing my bachelor's degree for "BLDC motor and controller" and I'm just bringing out couple of theories and hypothesis' to see if they make sense to you guys.

**1st topic/theory: "Effective" voltage and torque**

_What is effective voltage?_
Effective voltage is the "voltage doing work" in the motor's windings and is the difference between the PWM cycled battery voltage and the motor's BEMF voltage. If the PWM battery voltage is the same as the BEMF voltage, no current flows and no torque is generated.

> Example with arbitrary values:
> 12 V battery voltage and 50 % PWM duty cycle -> 6 V
> Motor's BEMF voltage -> 4 V
> "Effective voltage" = 6 V - 4 V = 2 V

_Question: Does the effective voltage linearly effect the current/torque?_
AKA using the example values above. The 2 V "effective voltage" would cause current **X**, to flow through the winding. Now, if the motor's BEMF is just 2 Volts, the "effective voltage" would now be 4 Volts, would the resulting current now be **2X**?

**2nd topic/theory: Offset of "Effective" voltage and behavior**

How does the current behave when we offset the "effective voltage" and BEMF voltage?
> Example with arbitrary values:
> Our "effective voltage" -> 2 V
> 1st case voltages -> PWM 4 V, BEMF 2 V
> 2nd case voltages -> PWM 12 V, BEMF 10 V

_Question: Is the same current flowing the same in both cases?_
Both cases have the same "effective voltage", but is the current the same too? Or is the current effected something else also that is derived from those 2 voltages (Test conditions are theoretical and therefore ideal, no friction losses or hysteresis losses etc...)?

_Please stay on topic and avoid digressing. Or at least point out that you're going off-topic like below_

**Offtopic**. I have gathered a bunch of student candidates from my local university who we're interested in my electric longboard project. I am in the process of interviewing them. I made a presentation in which I showed the board, it's specs and how it was developed and presented three bachelor's degree eligible works for the group of 14 students. Out of the 14 students I got five interested students who wanted to join in. I have 3 areas available (BMS, Remote and smartphone app), so I'll have to interview the five and pick one to each area. We'll see how it progresses from here.
```

---
## \#2 Posted by: devin Posted at: 2016-09-09T10:30:50.366Z Reads: 178

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2016-09-09T10:47:27.722Z Reads: 160

```
_I'm going to post all future questions in the original post, so people don't have to go hunting for them in the case this thread gets larger._

[quote="devin, post:2, topic:9255"]
My Theory: My opinion with PWM BLDC Motors (commonly used by this community - ie "VESC"), similar performance will only be seen if batt max and motor max limits are entered in a specific ratio depending on DC voltage, winding resistance & desired available wattage at 0rpm, full throttle.
[/quote]

I have changed the way I think/look about the VESC's motor max setting. Rather then thinking it's effects on PWM cycles or so on, I think it's easier to think about it as the maximum "effective voltage" that the controller can use. Of course the effective voltage will be different for different motors as their attributes are different AKA. how much current will X amount of effective voltage cause.

> Example with arbitrary values:
> Motor amp limit: 25 A
> with a particular motor, this current would be delivered with 5 V of effective voltage

So as long as difference between battery supply voltage and BEMF voltage is larger than 5 V, it's possible to  hold the effective voltage at 5V and the motor will be supplied 25 Amps or in another words, constant torque.
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2016-09-09T11:08:29.500Z Reads: 153

```
That chart is also a bit hard to apply as the X-axis RPM is relative to the Battery PWM cycle and it also causes the current line to behave a bit weirdly once taken into account.
```

---
## \#5 Posted by: devin Posted at: 2016-09-09T11:09:36.369Z Reads: 157

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2016-09-09T11:31:27.486Z Reads: 131

```
_I updated the original post with a 2nd question_

<img src="/uploads/db1493/original/3X/6/6/66fb5875a0cd710f261783eeeccedd6e38d266f6.JPG" width="690" height="325">

So is this how the VESC would behave in your example? It would keep the effective voltage at ~11.2 V -> current at ~89 Amps and the board would accelerate (I know the graph is not linear due to kinetic energy having velocity squared) until the BEMF hits ~38.8 V at point Z (the upper horizontal marked voltage point should be 38.8, not 48.8) at which point the VESC would then just keep the PWM at 100 % and while the motor would still keep accelerating the current would start decreasing along with "effective voltage" and therefore torque.

I'm personally interested in this from point of my own motor controller and it's control schemes.
```

---
## \#7 Posted by: devin Posted at: 2016-09-09T11:40:25.836Z Reads: 122

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2016-09-09T11:51:09.383Z Reads: 120

```
[quote="SimosMCmuffin, post:1, topic:9255"]
If the PWM battery voltage is the same as the BEMF voltage, no current flows and no torque is generated.
[/quote]

The point is that the AC voltage needs to 11.2 Volts higher than the BEMF voltage for the 89 Amps to flow. Using your AC/DC terms, the difference between AC voltage and BEMF voltage is the "effective voltage", and the "PWM BAT" line in the graph is the AC voltage.
```

---
## \#9 Posted by: Svenska Posted at: 2016-09-09T11:51:15.858Z Reads: 114

```
@SimosMCmuffin 

You are much better off asking these questions in Benjamins forum: http://vedder.se/forums/

And here is the code you want to look at for the controlling bit: https://github.com/vedderb/bldc/blob/cb2a205cb8f99f9dd5a75d7a1606394b6c2cf58f/mcpwm.c

Re your questions.
Assumptions I made: Ideal motor model, identical motor in all cases, no voltage sag, losses...

1. No, the effective voltage does not relate linear to current torque. If you're interested I can see if I still got the lecture slides floating around that explain it. If you want to make any predictions about current you need to know the applied torque.

2. That voltage gap gives you the rpm your motor desires. Therefore it wants to accelerate in this case. 
Same as the first case. Current relates to torque. Remember your  ideal motor model!

**Offish Topic**

What do you study?
```

---
## \#10 Posted by: devin Posted at: 2016-09-09T11:54:29.159Z Reads: 105

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#11 Posted by: SimosMCmuffin Posted at: 2016-09-09T12:20:28.196Z Reads: 100

```
[quote="Svenska, post:9, topic:9255"]
And here is the code you want to look at for the controlling bit: https://github.com/vedderb/bldc/blob/cb2a205cb8f99f9dd5a75d7a1606394b6c2cf58f/mcpwm.c
[/quote]

I'm the kind of guy who likes to study the theory and then apply it with my understanding to the problem, so in problem cases, if I understand that my theory understanding is wrong, I need to figure out what part I don't understand or I misunderstood.

[quote="Svenska, post:9, topic:9255"]
No, the effective voltage does not relate linear to current torque. If you're interested I can see if I still got the lecture slides floating around that explain it. If you want to make any predictions about current you need to know the applied torque.
[/quote]

It would be greatly appreciated if you could find those lecture slides.

[quote="Svenska, post:9, topic:9255"]
That voltage gap gives you the rpm your motor desires. Therefore it wants to accelerate in this case. Same as the first case. Current relates to torque. Remember your  ideal motor model!
[/quote]

I know it wants to accelerate. I know current is directly related to torque. What I want to know how the voltage gap and current relate to one another at different motor RPMs (BEMF). 

[quote="Svenska, post:9, topic:9255"]
What do you study?
[/quote]

I study embedded systems in Finland at Tampere's polytechnic university. I have a strong electronics background and mechanical design from hobby time.
```

---
## \#12 Posted by: devin Posted at: 2016-09-09T12:33:39.901Z Reads: 83

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#13 Posted by: SimosMCmuffin Posted at: 2016-09-09T12:50:56.159Z Reads: 89

```
[quote="devin, post:12, topic:9255, full:true"]
Let's think about where the energy to power the Back EMF comes from. I think it comes from the momentum of the magnets. Does potential energy increase linearly with momentum?
[/quote]

[quote="SimosMCmuffin, post:6, topic:9255"]
(I know the graph is not linear due to kinetic energy having velocity squared)
[/quote]
I already pointed out that the nice linearity is not real. The point was that the AC voltage was maintained 11.2 V over the BEMF.


BEMF is generated from the change in the magnetic field over electric field, which changes linearly with speed. If you have a coil and you move a magnet through it at X speed the voltage it produces in the coil would be Y, now if the speed is 2X then the voltage is 2Y.


Electric field and magnetic field theory on pages 5 and 6 (note how not any function has anything squared):
https://www.monolithicpower.com/Portals/0/Documents/Products/Documents/appnotes/Brushless%20DC%20Motor%20Fundamentals.pdf
```

---
## \#14 Posted by: devin Posted at: 2016-09-09T12:57:33.867Z Reads: 88

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#15 Posted by: SimosMCmuffin Posted at: 2016-09-09T13:05:48.533Z Reads: 93

```
[quote="devin, post:14, topic:9255"]
the only speed 11.2 motor AC volts should exist would be exceedingly close to 0rpm.
[/quote]

That's why when the motor starts turning and generating BEMF, we need to increase our PWM duty cycle to raise the AC voltage so it stays 11.2 volts higher than the BEMF voltage. 


<img src="/uploads/db1493/original/3X/6/6/66fb5875a0cd710f261783eeeccedd6e38d266f6.JPG" width="690" height="325">

As pictured in the graph. when BEMF is 0 V (meaning motor is NOT turning, 0 RPM), our duty cycle with the 50V battery would be 22.4 %. But later at the vertical voltage gap mark (effective voltage) our BEMF is ~17 V, and we change the duty cycle to 56.4 % so that the AC voltage is now 28.2 V and the voltage gap is still 11.2 Volts.

[quote="devin, post:14, topic:9255"]
Though I still believe when the duty cycle reaches 100% at full throttle, you will have 50V AC which matches the 50V DC, before accounting for the BEMF at that particular RPM. But I have no idea what the "effective" ac voltage would be at that RPM, after you account for the BEMF.
[/quote]

That's why the PWM BAT plateaus at 50 V meaning 100% duty
```

---
## \#16 Posted by: devin Posted at: 2016-09-09T13:10:26.766Z Reads: 79

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#17 Posted by: SimosMCmuffin Posted at: 2016-09-09T13:12:04.316Z Reads: 76

```
That's exactly what my theory is trying to solve, how the system behaves dynamically at different motor BEMF/RPMs. I'm sorry if I didn't point out that BEMF is only generated when the motor is turning, so all my examples have the motor rotating at different speeds, but the BEMF can be used without knowing the motors real kV and RPM values, because it's always relative.

It's a bit like Ohm's Law, R = U / I  -> BEMF = RPM / kV
```

---
## \#18 Posted by: devin Posted at: 2016-09-09T13:16:12.495Z Reads: 71

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#19 Posted by: devin Posted at: 2016-09-09T13:20:41.725Z Reads: 70

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#20 Posted by: SimosMCmuffin Posted at: 2016-09-09T13:21:05.710Z Reads: 71

```
The reason why I'm asking this question to test my theory is because I want to make a constant torque algorithm for the controller, which means I need to have a constant current going through the motor. X current = X torque. Sure the acceleration is not linear, but the change in kinetic energy is.

That's why I wondered if I know what speed the motor is turning (BEMF) then I would know what duty cycle to keep the "effective voltage" constant to produce a constant torque, IF my theory is correct.
```

---
## \#21 Posted by: SimosMCmuffin Posted at: 2016-09-09T13:22:18.012Z Reads: 60

```
It's AC of course. It's on the motor side (AC side)
```

---
## \#22 Posted by: devin Posted at: 2016-09-09T13:22:57.773Z Reads: 62

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#23 Posted by: devin Posted at: 2016-09-09T13:23:58.109Z Reads: 65

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#24 Posted by: SimosMCmuffin Posted at: 2016-09-09T13:28:46.352Z Reads: 67

```
[quote="devin, post:23, topic:9255"]
So BEMF voltage is in AC terms, but it effects amps linearly in DC terms on the DC side with a typical PMDC motor?
[/quote]

BEMF affects the ratio between DC / AC side. It's bit hard to describe clearly... I can try to give an example if you're interested.
```

---
## \#25 Posted by: devin Posted at: 2016-09-09T13:30:29.063Z Reads: 68

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#26 Posted by: SimosMCmuffin Posted at: 2016-09-09T13:35:39.107Z Reads: 57

```
I need to say that the BEMF does not necessarily stay close to the AC voltage.
```

---
## \#27 Posted by: devin Posted at: 2016-09-09T13:42:50.695Z Reads: 59

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#28 Posted by: devin Posted at: 2016-09-09T13:54:58.512Z Reads: 60

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#29 Posted by: SimosMCmuffin Posted at: 2016-09-09T14:02:33.456Z Reads: 53

```
Okay, so we are calculating electrical power here, right?
But, should we also mention the current =  torque, so in all these three examples, shouldn't we still get roughly the same torque?

You got skype or voice comms where we could ramble?
```

---
## \#30 Posted by: devin Posted at: 2016-09-09T14:02:43.098Z Reads: 55

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#31 Posted by: Svenska Posted at: 2016-09-09T14:08:28.070Z Reads: 50

```
Where are you located @SimosMCmuffin

I'm happy to have a Skype ramble with you about that stuff. 

Did I understand that right that you want to make your own ESC?
```

---
## \#32 Posted by: SimosMCmuffin Posted at: 2016-09-09T14:16:15.076Z Reads: 56

```
[quote="SimosMCmuffin, post:11, topic:9255"]
I study embedded systems in Finland at Tampere's polytechnic university. I have a strong electronics background and mechanical design from hobby time.
[/quote]

http://imgur.com/a/Mjodj

I have already designed and run one, but I'm working on the next iteration.
```

---
## \#33 Posted by: devin Posted at: 2016-09-09T14:21:44.249Z Reads: 55

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#34 Posted by: SimosMCmuffin Posted at: 2016-09-09T14:26:00.497Z Reads: 57

```
I'm interested now in the analogue of horsepower and torque in cars.

Because we know that current = torque, but how does the power factor in...

https://www.youtube.com/watch?v=iXAbCpqizok
```

---
## \#35 Posted by: devin Posted at: 2016-09-09T14:27:37.245Z Reads: 59

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#36 Posted by: SimosMCmuffin Posted at: 2016-09-09T14:30:05.248Z Reads: 57

```
Okay, now I start to see my theory go wrong
```

---
## \#37 Posted by: devin Posted at: 2016-09-09T15:45:18.884Z Reads: 55

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#38 Posted by: SimosMCmuffin Posted at: 2016-09-10T07:12:33.312Z Reads: 50

```
After a good night's sleep and allowing my head to process stuff during the night. I have a new model to explain things, but it's not good enough yet that I would know how to draw any graphs of it.

But I'll try to set up the basis here.

> So as we have now concluded: **Power = Torque x RPM**  -> **Power = Current x BEMF**

> So to have a steady acceleration we need constant power and not torque.

> In the beginning when our motor is not turning we need more torque (current) to make up for the lack of RPM.

> But as our motor starts to spin up and our RPM rises, our torque needs to lower in order to keep the power constant.

> But to get torque (current), our AC voltage needs to be higher than the BEMF, or no current flows.

_Seems like a good basis?_

**Off-topic** I have noticed how during the day I usually in the university suck up as much information as I can, but sometimes I don't understand the principles behind them. After a good night's sleep though, things start to fall in place.
```

---
## \#39 Posted by: Svenska Posted at: 2016-09-10T07:36:43.582Z Reads: 47

```
[quote="SimosMCmuffin, post:38, topic:9255"]
Power = Torque x RPM  -&gt; Power = Current x BEMF
[/quote]

Power = Torque x RPM That is right. 

But I'm not sure about your second statement. 
Power = Current x BEMF

Shouldn't it rather be: Power = Current x Effective Voltage?

But that seems to simple too. I think you should try and derive it from first principles.
```

---
## \#40 Posted by: SimosMCmuffin Posted at: 2016-09-10T07:42:09.140Z Reads: 44

```
[quote="Svenska, post:39, topic:9255"]
Shouldn't it rather be: Power = Current x Effective Voltage?
[/quote]

That was my first theory, but as we discussed it with Devin it turned out not to work. Because the effective voltage is indirectly affected by the BEMF/RPM , so it doesn't work with the Power = Torque x RPM.

It is apparent in the Vedder's video logs, as the Power he logs is much higher at higher speeds, even though the motor current is the same and that is the RPM giving higher overall power.

[quote="devin, post:33, topic:9255"]
even more revealing...

20.31 motor amps @ 37.6 km/hr = 614.71 watts

23.49 motor amps @ 0.5 km/hr = 37.29 watts
[/quote]



And BEMF is directly related to RPM.
```

---
## \#41 Posted by: SimosMCmuffin Posted at: 2016-09-10T07:51:28.677Z Reads: 38

```
Now the real question still is, how is current affected by the "effective voltage" when the BEMF/RPM changes, is it still linear?
```

---
## \#42 Posted by: Svenska Posted at: 2016-09-10T07:51:34.512Z Reads: 40

```
The power has to be higher at higher speeds. The current being the same is due to having to overcome all the resistances, losses...

And your right, Power = Current x Effective Voltage is wrong. It needs to be Power = (Current x Effective Voltage) + initial power.
Or Power needed to be added to reach desired RPM = Current x Effective Voltage
```

---
## \#43 Posted by: SimosMCmuffin Posted at: 2016-09-10T07:55:45.861Z Reads: 40

```
The "effective voltage" can be handled as the speed difference that the motor wants to achieve and it therefore pulls current to try to achieve that speed, If there is no "effective voltage", then the motor is already at the speed it wants to spin and it won't pull any current and therefore power = 0.
```

---
## \#44 Posted by: Svenska Posted at: 2016-09-10T08:13:31.304Z Reads: 40

```
[quote="SimosMCmuffin, post:43, topic:9255"]
at the speed it wants to spin and it won't pull any current and therefore power = 0.
[/quote]

That is true if you want to neglect ALL losses. But then you can't compare it to the videos of a skateboard...
```

---
## \#45 Posted by: SimosMCmuffin Posted at: 2016-09-10T08:16:46.469Z Reads: 40

```
Yes the statement is correct, but factoring the real life losses, it will never spin at the speed it wants to spin (as you said), so there is always a little bit of "effective voltage" giving current to combat the losses and it then settles somewhere below the "desired speed" where the used power counteracts the losses.
```

---
## \#46 Posted by: Svenska Posted at: 2016-09-10T08:49:07.773Z Reads: 41

```
I'm glad we agree. You might want to think about what that means for your implementation of current/torque control. 
That is the whole point of the thread, isn't it?
```

---
## \#47 Posted by: SimosMCmuffin Posted at: 2016-09-10T09:02:53.726Z Reads: 44

```
I still need to know how the current relates to the "effective voltage" and BEMF. Is it linear to "effective voltage" no matter what the BEMF/RPM is or does it change with it. AKA 2nd question.

[quote="SimosMCmuffin, post:1, topic:9255"]
2nd topic/theory: Offset of "Effective" voltage and behavior

How does the current behave when we offset the "effective voltage" and BEMF voltage?

Example with arbitrary values:
Our "effective voltage" -&gt; 2 V
1st case voltages -&gt; PWM 4 V, BEMF 2 V
2nd case voltages -&gt; PWM 12 V, BEMF 10 V

Question: Is the same current flowing the same in both cases?
Both cases have the same "effective voltage", but is the current the same too? Or is the current effected something else also that is derived from those 2 voltages (Test conditions are theoretical and therefore ideal, no friction losses or hysteresis losses etc...)?
[/quote]
```

---
## \#48 Posted by: devin Posted at: 2016-09-10T15:46:46.660Z Reads: 41

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#49 Posted by: devin Posted at: 2016-09-10T15:58:51.567Z Reads: 38

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#50 Posted by: devin Posted at: 2016-09-10T16:10:34.892Z Reads: 41

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#51 Posted by: Hummie Posted at: 2016-09-10T16:20:23.147Z Reads: 53

```
`The back emf limiting the torque though...you only need a very small voltage across the motor, the difference between the battery voltage and back emf, to have potential for a huge amp flow.    lets take this motor as an example because it's similar in size to what we've been working in equations  just with a 5x higher kv<img src="/uploads/db1493/original/3X/8/2/8249d10e41cd23da85e9285826ff09225ba9ff4f.png" width="281" height="499">
http://www.rapidtables.com/calc/electric/watt-volt-amp-calculator.htm
With only two volt potential and using my motors first in the equation with its resistance ,  I can draw 17 amps per motor.  Simos



And with this 5x higher kv motor run it through ohm's law and with the 2 volt potential <img src="/uploads/db1493/original/3X/8/e/8e6a17d0351b66bae4f9f662eff416d0523c8864.png" width="281" height="499">  I can get 80 amps!

And here's my question:  the wattage number above is dismal at 166 watts even though 80amps. Of course u can point to the low voltage...but what good is voltage anyway!?  I still can't figure out the basic of how voltage is power if a motor only runs on amps 


On another note about speed and power, this is how I see speed in the power equation:   say I'm coasting at 20mph down a hill without a motor it would be fair to say I have power.  I have power to get from a to b as I finally slow but it's not power in the typical sense I think about it. Torque is power to me.  Without torque there will be no speed. Speed is just torque's dregs
Simosmcmuffin I'm probably far from ur project talking about this but it's a fundamental that I still can't get my mind around after years
```

---
## \#52 Posted by: SimosMCmuffin Posted at: 2016-09-10T17:57:47.917Z Reads: 47

```
The effective voltage values I have been using are not based on any real values, as I have not measured it ever, yet. So they are just there to say: "So we have some voltage that is doing work, and let's say X amount of voltage causes Y amount of current." point being, that they might not be close to actual values we get from motors we use.

The calculator you use is just a static power calculator, but as it doesn't have the RPM/BEMF element to it, is this what the motor would see at 0 RPM? What about if the motor is spinning, as an example: the BEMF is 10 Volts and then we supply 12 Volts to the motor, giving the effective voltage of 2 V. Will the motor still pull 83.3 Amps? And then our power would be 12 V * 83 A = ~1000 Watts. This makes sense with the Power = Torque x RPM.

Also, if your assumption that current increases linearly with voltage across the motor winding resistance. Than that would answer the 1st question:
[quote="SimosMCmuffin, post:1, topic:9255"]
1st topic/theory: "Effective" voltage and torque

What is effective voltage?
Effective voltage is the "voltage doing work" in the motor's windings and is the difference between the PWM cycled battery voltage and the motor's BEMF voltage. If the PWM battery voltage is the same as the BEMF voltage, no current flows and no torque is generated.

Example with arbitrary values:
12 V battery voltage and 50 % PWM duty cycle -&gt; 6 V
Motor's BEMF voltage -&gt; 4 V
"Effective voltage" = 6 V - 4 V = 2 V

Question: Does the effective voltage linearly effect the current/torque?
AKA using the example values above. The 2 V "effective voltage" would cause current X, to flow through the winding. Now, if the motor's BEMF is just 2 Volts, the "effective voltage" would now be 4 Volts, would the resulting current now be 2X?
[/quote]
```

---
## \#53 Posted by: SimosMCmuffin Posted at: 2016-09-10T19:50:37.809Z Reads: 44

```
I would like add a point a couple of things about about the performance graph.

The RPM, as depicted in the graph in percentage, is a relative measurement.

[quote="devin, post:48, topic:9255"]
% Electrical to Mechanical Conversion Efficiency value is generally highest at constant ~85% No Load RPM Full Throttle (shown as green line below) with PMDC (commutator based) electric motors.
[/quote]

Not necessarily at full throttle, but at 85 % BEMF voltage of the constant voltage.
> as an example:
> Motor has 100 kV, we have a lab power supply and a controller which runs constantly at 100% duty.
> If our power supply voltage is 10 V, the peak efficiency is at 850 RPM
> supply voltage 15 V, peak efficiency at 1275 RPM
> supply voltage 20 V, peak efficiency at 1700 RPM

This supply voltage can be also directly controlled with a battery voltage and the duty cycle:
> Motor 100 kV, 20 V battery voltage
> Duty cycle 50 % -> voltage 10 V, peak efficiency at 850 RPM
> Duty cycle 75 % -> voltage 15 V, peak efficiency at 1275 RPM
> Duty cycle 100 % -> voltage 20 V, peak efficiency at 1700 RPM

Point being that the RPM axis is always 100% given the voltage applied to the motors kV value. And you're running at peak efficiency when the BEMF is 85 % of the supplied voltage.
```

---
## \#54 Posted by: SimosMCmuffin Posted at: 2016-09-10T20:07:14.625Z Reads: 45

```
"The DC Motor block represents the electrical and torque characteristics of a DC motor using the following equivalent circuit model:"

http://www.mathworks.com/help/physmod/elec/ref/dc_motor_diag.png
Source: http://www.mathworks.com/help/physmod/elec/ref/dcmotor.html

As seen in the model, BEMF (Vb) is just a counter voltage against the applied voltage. And the BEMF is a function of the motor's kV and RPM.
```

---
## \#55 Posted by: devin Posted at: 2016-09-10T21:42:06.595Z Reads: 46

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#56 Posted by: Photorph Posted at: 2016-09-11T01:07:24.908Z Reads: 41

```
Not really contributing here...but this thread is total mind F@#&
```

---
## \#57 Posted by: saul Posted at: 2016-09-11T04:33:50.713Z Reads: 44

```
No time to read all this because it reminds me of physics class too much, but where are you going to school? my eboard would have been a cool senior design project....at least till the advisors suck all the fun out of it....
```

---
## \#58 Posted by: SimosMCmuffin Posted at: 2016-09-11T07:18:36.591Z Reads: 43

```
I'm Finnish and I go to the Tampere's Polytechnic University. 24 Years old, studying in the embedded systems department (microcontrollers). I plan on keeping the project under my own wing as much as I can. I'll of course let other people give their opinions on things, but how far they go depend on me. AKA we will do as we see fit.

I'm interviewing the last 2 guys on Monday and then assembling the team of 3 out of the 5 interested volunteers.
```

---
## \#59 Posted by: SimosMCmuffin Posted at: 2016-09-11T07:59:23.426Z Reads: 46

```
You don't have to have full throttle (100% duty) to get peak performance.

[quote="devin, post:55, topic:9255"]
if the battery voltage is 50V, and the motor is 100kv, with full throttle, 100% rpm on the graph would be 5,000rpm also known as no load rpm.
[/quote]
Yes, but then we can use the duty % to change the no load 100% speed.
On my controller this is possible, for example I can use a 50 V battery, but limit my duty cycle at full throttle to 50 %, then my "constant voltage" would be just 25 V and my no load is 2500 RPM, then the peak efficiency is at ~2100 RPM.

Then when you factor in the dynamics of accelerating from standstill. It causes the graph to sort of stretch on X axis (power and efficiency) as the duty cycle increases, while the torque & amps curve doesn't get stretched, it gets offset horizontally.
```

---
## \#60 Posted by: saul Posted at: 2016-09-11T08:23:54.526Z Reads: 45

```
that sounds about right, good luck on this project, hopefully you can get all this theory into something we can see in the real world, like more torque and/or efficiency.
```

---
## \#61 Posted by: Svenska Posted at: 2016-09-11T12:20:45.900Z Reads: 41

```
@SimosMCmuffin

You got the wrong Matlab model there. Try this one:

http://au.mathworks.com/help/physmod/elec/ref/inductionmotor.html
```

---
## \#62 Posted by: SimosMCmuffin Posted at: 2016-09-11T12:23:48.873Z Reads: 45

```
Are you sure? I mean a permanent magnet motor surely is not an induction motor. Induction motor needs to create magnetic rotor flux in order to create torque, while a permanent magnet motor already has the magnets providing a constant flux.

Actually, I correct myself that this: http://www.mathworks.com/help/physmod/elec/ref/femparameterizedpmsm.html Would be the correct model for 3-phase BLDC motor.
```

---
## \#63 Posted by: Svenska Posted at: 2016-09-11T12:33:25.484Z Reads: 45

```
That ones close too. But its defined in terms of flux linkage.
Induction and BLDC motors are pretty much equivalent.
```

---
## \#64 Posted by: SimosMCmuffin Posted at: 2016-09-14T10:26:57.837Z Reads: 44

```
Okay, so. Discussed my motor theories with my electronics lab teacher and he agreed with all the hypothesis and also confirmed the 1st and 2nd hold true. I also figured out how to model the regen braking.

The whole point of my theory is to mathematically figure out the AC/DC currents and power, when we know the characteristics of the motor (kV, pole count and internal winding resistance), it's RPM, battery voltage and duty cycle. This means my controller has to only be able to measure the battery voltage and motor RPM. And everything else is configured as a constant value.
```

---
## \#65 Posted by: Svenska Posted at: 2016-09-14T10:34:07.582Z Reads: 46

```
I'm looking forward to seeing that implementation!
```

---
## \#66 Posted by: SimosMCmuffin Posted at: 2016-09-14T10:46:37.478Z Reads: 46

```
I have already ordered the PCBs for the next iteration of my controller. Currently waiting for the boards to arrive, but I'm having a delay with Digi-Key until 28th, because unfortunately they have a backorder on one of the components for the board.
<img src="/uploads/db1493/original/3X/7/8/78683c19903ff0b1e4e868322336ba23ba1b0640.png" width="689" height="354">

It's also going to take time to learn the ARM-platform. Lots of testing, debugging and blinking LEDS with registers, but I believe it will be worth it in the end (because otherwise I would have stayed with the familiar AVR-family).

Also development team news.  I have interviewed the 5 interested students and 3 has been selected into the team. I held an orientation with them on Monday. Basically going a bit deeper with what we're trying to achieve and looked at different executions of products available on market today. I have established comms with the group (telegram) and we meet on Mondays for face-to-face time. I'll update things as we start the progress.

Control scheme wise, I also brought it up with the teacher and we agreed that speed control would most likely feel the most natural to control the board. So I'll use the algorithm to figure out the AC/DC currents and make sure they stay within safe limits, so we don't burnout our motor or battery.
```

---
## \#67 Posted by: Svenska Posted at: 2016-09-14T11:01:39.918Z Reads: 45

```
Speed control as in RPM control? 
Torque control is the one that feels more natural to me and as far as I'm aware to most people here.
```

---
## \#68 Posted by: SimosMCmuffin Posted at: 2016-09-14T11:11:27.107Z Reads: 47

```
Yes.

I know that constant torque = true constant acceleration, but RPM control has a bit easier time to truly control the speed at which you want to move.

I don't actually know exactly how it works on the VESC, but I hope you could elaborate on that. How do you control speed with VESC? Because as far as I know, the throttle position is linearly linked to the motor amps and motor amp limit.
AKA 100 Amp motor limit, 50% throttle = VESC will try to maintain 50 Amps of motor current.

Because the problem I see with torque control is that it's controlling the rate at which speed changes, at least in principle. But as an example. if your board tops out, let's say 40 km/h, at what position do you have to hold the throttle to go 20 km/h? because it's not 50%. With speed control it would be 50% This is what I'm interested in when controlling torque and speed control.
```

---
## \#69 Posted by: elkick Posted at: 2016-09-14T11:58:26.328Z Reads: 43

```
Have you seen Benjamin's comments about the different control modes at http://vedder.se/2015/01/vesc-open-source-esc/?
```

---
## \#70 Posted by: devin Posted at: 2016-09-14T14:10:18.467Z Reads: 45

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#71 Posted by: SimosMCmuffin Posted at: 2016-09-14T14:11:15.972Z Reads: 54

```
Funny, I have that webpage bookmarked, but don't remember reading or seeing that "control mode" section before :D

I guess I'll implement at least the torque and speed modes and then add a configuration menu to the smartphone app, where people can decide which they want to use, along with max speed and max torque settings.


Also PCBs arrived today!
<img src="/uploads/db1493/original/3X/2/a/2a1c8120114e389bcf4353ab917a805e752ca42e.jpg" width="282" height="500">
```

---
## \#72 Posted by: SimosMCmuffin Posted at: 2016-09-30T10:50:59.539Z Reads: 41

```
Rage.... **RAGE!!!!**.... _*Sigh, disappointment in myself_...

Finally, parts arrived for the new motor controller and I was going to keep myself busy with it the whole weekend... Or so I hoped.

**See if you guys can locate the problem in the picture attached below...**

<img src="/uploads/db1493/original/3X/a/f/af89c77e1313843af818d8a134ecd963943cb3c3.jpg" width="690" height="389">

Turns out  TQFP packages can have different lead pitches... The PCB has a 0.8 mm lead pitch and the ARM MCU meant to be used has 0.5 mm pitch... dangit!
```

---
## \#73 Posted by: SimosMCmuffin Posted at: 2016-10-13T15:52:25.647Z Reads: 45

```
Got the new boards today and immediately got to work assembling it and I'm happy to say it's ALIVE!
I'm finally able to start messing around in the ARM architecture and start learning it :grin:

<img src="/uploads/db1493/original/3X/6/2/62eb3b2038fd3c4639691ead4210e08f21ac5368.jpg" width="689" height="390">

Plan is first to learn how to use the ARM's peripherals and then copy the functions over from the older controller and start driving some light loads.

Will update as things progress!
```

---
## \#74 Posted by: SimosMCmuffin Posted at: 2016-10-19T18:07:17.959Z Reads: 40

```
Update time!

<img src="/uploads/db1493/original/3X/7/d/7d1e08536d33af346598865f2e42c13b06e08ae5.jpg" width="690" height="389">

Motor is spinning, timers are running, LCD-display is outputting, AD-conversions are converging, Bluetooth communication works and interrupts are being serviced!

Still some work to do before going for a test ride, but I'm aiming to do it this week!

I also met up with our dev team's smartphone guy and we did some test transmits between his WIP phone app and the motor controller and we had working comms! We then discussed a bit about the packet framework for actual use case and developed a first draft of the protocol. **Bluetooth will only be used for non-critical communication!** If you wanna check out some concept mock-up pictures for the smartphone app, check here https://drive.google.com/file/d/0B45b0uNJKZ0eQ3VQMUFFRXN1RDA/view?usp=sharing

Our remote controller developer is prototyping with the Nordic nRF24-modules (**2.4 GHz RF**), for more stable and reliable remote connection.
```

---
## \#75 Posted by: Okami Posted at: 2017-05-19T16:13:08.304Z Reads: 17

```
Nice thread, once again! You should have written more precisely it is DIY controller or something :D I think not that many people develop their own controllers :)
```

---
