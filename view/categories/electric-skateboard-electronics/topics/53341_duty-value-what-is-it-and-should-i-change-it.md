# Duty value?&hellip; what is it and should i change it?

### Replies: 50 Views: 1294

## \#1 Posted by: Juvaknin Posted at: 2018-04-24T14:01:58.995Z Reads: 188

```
Hi guys,
This monitor values are from riding up hill.. and didnt had enogh power to make it. even with this values (focbox)
Battery max 20
Motor max 45
What is this Duty 40% only... i should change it somehow?.. its safe to change it?.. it will give more power?.. need your opinions...
Thanks..
![image|325x500](upload://kmKwlAH5Hv5K2zoBS7mQPUvF4WR.jpeg)
```

---
## \#2 Posted by: DeathCookies Posted at: 2018-04-24T14:11:32.455Z Reads: 174

```
I think in simple words: your throttle. So you cannot Change it like a normal vesc Setting (e.g. max Motor amp).

You can only Change that value by giving or releasing throttle ;)
```

---
## \#3 Posted by: Juvaknin Posted at: 2018-04-24T14:17:16.172Z Reads: 170

```
But i was at full throttle.. and on my app in vesc show 100% throttle when i press all the way.
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2018-04-24T14:18:54.696Z Reads: 165

```
Someone correct me if I'm wrong but I believe duty is what percent of your max erpm your motor is currently spinning at. I believe the only thing about it you can adjust is your max duty, which should be 95% or so. Were you full throttle at that point in your image posted? It looks like motor current is being limited to 37 amps for some reason.
```

---
## \#5 Posted by: TehAtheist Posted at: 2018-04-24T14:23:39.782Z Reads: 153

```
It's not your throttle, although it is related.

You have a brushless DC motor, when you apply a constant maximum DC voltage, it'll spin at it's maximum speed. As you can see with metr.at your voltage always stays the same (after a while it drops due to battery voltage drop when it's being depleted, but that's only a few volts over a large amount of time).

So if we were to just apply the voltage to the DC motor with a switch, it would snap to it's max speed (if it was able to draw an unlimited amount of current). Which is not what you want. So how do we control the speed of the motor? Via duty cycle. This means that for example for a duty cycle of 40%, 40% of the time, you apply voltage to the motor and 60% of the time, you don't. This way, the mean voltage over the motor drops and it'll spin slower.

The thing is, your motor cannot accelerate to max speed with you on the board in just an instant. It takes time as otherwise the current needs to be very high. You are however controlling the current by remote, that is your throttle. So the vesc will try to speed up the motor with the duty cycle, as long as the current that the motor needs in order to do so, is allowed to flow to it. Either limited by you or simply the vesc's maximum current.

When you are riding up hill, the motor draws more current as it's putting in more work to get over that steep hill, if the maximum throttle value is reached and your motor is drawing it's maximum from the batteries (accoridng to your set limits) it won't increase in speed.


Edit: So in short, if you want to accelerate on that hill. Your batteries must allow more current to the motor or your motor must allow more current to flow. This is limited by either your batteries, vesc or motor. 

I believe currently your battery current is set to 15A. IF THEY CAN supply more current, you could raise this value and you will speed up when going on that hill.In general you wil also have a more powerful board.
```

---
## \#6 Posted by: Juvaknin Posted at: 2018-04-24T14:37:24.708Z Reads: 116

```
But as you can see it didnt get to my max settings..
My settings are
Batt max 20A
Motor max 45A
Its didnt go up to this values.. why?
```

---
## \#7 Posted by: TehAtheist Posted at: 2018-04-24T14:38:34.724Z Reads: 113

```
I cannot figure that one out either :upside_down_face:
```

---
## \#8 Posted by: Juvaknin Posted at: 2018-04-24T14:41:49.503Z Reads: 108

```
Its must be some vesc setting.. cant find what it is...
```

---
## \#9 Posted by: pat.speed Posted at: 2018-04-24T14:49:44.446Z Reads: 103

```
Can we see your Vesc settings?
```

---
## \#10 Posted by: Juvaknin Posted at: 2018-04-24T15:09:53.757Z Reads: 106

```
Here it is. 
![image|666x500](upload://lnsTCslY5L6VSb7cTpMxWLwvhNm.jpeg)![image|666x500](upload://iprGa677UXe8epwTavnLnwScCWh.jpeg)![image|666x500](upload://pqnMoDmuGN3PKQ2hcn9e23GUstj.jpeg)![image|666x500](upload://noaOhKJ756hJItVaVP3BPtT9wgT.jpeg)
```

---
## \#11 Posted by: Deckoz Posted at: 2018-04-24T15:24:30.566Z Reads: 89

```
Duty cycle is speed dependent..

Duty cycle = motor voltage. Motor voltage and kv= rpm...


So no you cannot change it.
```

---
## \#12 Posted by: Mathias Posted at: 2018-04-24T15:24:38.130Z Reads: 91

```
In general I think 20 A is very low. You might want to increase that to 40 A, which should be safe, according to the info in your other thread.
But regardless, it's definitely strange that your max values are not reached. Do you have motor temperature sensors? Something your telemetry doesn't show is the motor temperature. I don't know that motor, but is you run a small, single motor uphill, then it's efficiency is extremely low, and this will heat it up very quickly.
```

---
## \#13 Posted by: Juvaknin Posted at: 2018-04-24T15:31:18.012Z Reads: 89

```
Nop. The motor cold right after the test. I checked it. 
Again, just dont know why the system
Not getting to max settings.. it can get to y max settings. Its not high values.. cant find why its not getting to 20A or higher motor Amps...
```

---
## \#14 Posted by: Juvaknin Posted at: 2018-04-24T15:33:29.302Z Reads: 81

```
So i dont need to touch the duty cycle?...its not it?..
```

---
## \#15 Posted by: Deckoz Posted at: 2018-04-24T15:33:40.934Z Reads: 77

```
[quote="Juvaknin, post:13, topic:53341"]
not getting to 20A or higher motor Amps…
[/quote]

It is... Your motor amps in that picture are 36.9
```

---
## \#16 Posted by: TehAtheist Posted at: 2018-04-24T15:33:59.436Z Reads: 78

```
No, you don't need to change duty cycle, that values is good :)
```

---
## \#17 Posted by: Juvaknin Posted at: 2018-04-24T15:35:47.387Z Reads: 77

```
No.. the max battery is set to 20A
Motor max is 45A. Its not getting even 40 on my test.
```

---
## \#18 Posted by: Deckoz Posted at: 2018-04-24T15:37:34.442Z Reads: 80

```
If your not getting the full motor max. Then your ppm endpoints are setup wrong. Or your remote is in beginner mode with 80% throw

Make sure you calibrate your PPM Min(pull throttle full brake and set the value on the green bar, while real time data is enabled)

Do the same for ppm max,and then center point.
```

---
## \#19 Posted by: Juvaknin Posted at: 2018-04-24T15:41:55.634Z Reads: 79

```
Yes. Done that. The line on the vesc software going all the way min/full 😕 also used the wizard auto settings for that. Same thing..
```

---
## \#20 Posted by: Jinra Posted at: 2018-04-24T16:01:23.631Z Reads: 77

```
battery max is too low you need to up it.
```

---
## \#21 Posted by: Mathias Posted at: 2018-04-24T16:02:24.165Z Reads: 74

```
I just noticed: your motor is set to "Sensored mode" that's not correct. What you want is hybrid! That means sensored for low RPM and switching to sensorless at higher. Sensored mode does not work well at high RPM. This might be at least part of the problem. 

And I second increasing battery amp to ~40 A. But this is not the issue here.
```

---
## \#22 Posted by: Juvaknin Posted at: 2018-04-24T16:02:34.881Z Reads: 70

```
Its two vesc... its 20 and 20
```

---
## \#23 Posted by: Jinra Posted at: 2018-04-24T16:03:46.887Z Reads: 70

```
Same thing, up the battery max to the the highest the pack supports with a 50A limit per vesc.
```

---
## \#24 Posted by: Juvaknin Posted at: 2018-04-24T16:12:04.996Z Reads: 68

```
Will give it a try. Thanks
```

---
## \#25 Posted by: Mathias Posted at: 2018-04-24T16:12:15.839Z Reads: 66

```
I think he's got 50 A BMS if I remember correctly.
```

---
## \#26 Posted by: Jinra Posted at: 2018-04-24T16:24:57.191Z Reads: 66

```
Sensored mode, while not efficient at high speed, still works. It should not be limiting his duty to 40%. As he's having issues on hills, I am leaning toward it being an insufficient current problem.
```

---
## \#27 Posted by: Juvaknin Posted at: 2018-04-24T16:40:42.972Z Reads: 63

```
Yes. But yet.. cant get max values.. its not high values.
```

---
## \#28 Posted by: Mathias Posted at: 2018-04-24T17:01:32.106Z Reads: 62

```
[quote="Jinra, post:26, topic:53341, full:true"]
Sensored mode, while not efficient at high speed, still works. It should not be limiting his duty to 40%. As he’s having issues on hills, I am leaning toward it being an insufficient current problem.
[/quote]
I'm not so sure about that. When you look at the telemetry it is really the motor amps that run into a plateau. It's not the battery amps. 

And I missed that he's got **2 x** 20 A, which is not that bad. 

Let's see what switching to hybrid mode does. I don't know that much about it, but sensored mode is much louder and less efficient because it doesn't get the current and motor phase aligned. Meaning switching happens at the wrong moment. If that leads to spikes and noisy readout, I could imagine that it triggers the 45 A current limit prematurely, and that's what's becoming the bottle neck here.
```

---
## \#29 Posted by: Mathias Posted at: 2018-04-24T17:04:55.529Z Reads: 58

```
PS: On top of that going to hybrid will give the same output power at much lower battery current, so this issue might go away altogether. But I'm also curious what will happen. I only played with sensored mode on the bench, never took it for a ride.
```

---
## \#30 Posted by: Jinra Posted at: 2018-04-24T17:12:35.837Z Reads: 59

```
I've run full sensored mode before, it doesn't limit DC. Motor amps plateau because duty goes up. You'll never hit motor max at higher duties.
```

---
## \#31 Posted by: Mathias Posted at: 2018-04-24T17:16:15.328Z Reads: 61

```
Sure it can limit DC indirectly. Unceasing DC here would mean increasing current, which is prohibited by another limit, in this case everything points to motor current being the bottle neck.
```

---
## \#32 Posted by: professor_shartsis Posted at: 2018-04-24T17:17:34.070Z Reads: 62

```
the duty cycle lowers the effective voltage of your battery to the voltage necessary to achieve the desired motor current considering the present back emf voltage caused by the spinning magnets. 

50v pack * 50% duty = 25v effective to the motor

at 0rpm:

((50v pack * 50% duty) - 0v bemf) / 0.1 ohm motor = 250a motor amps

25v effective * 250a motor current = 6250w electrical watts
```

---
## \#33 Posted by: Mathias Posted at: 2018-04-24T17:20:55.904Z Reads: 62

```
@devin, is that you?:joy: 
Sorry, I couldn't resist. But that's not how it works.
https://www.electric-skateboard.builders/t/hummie-vs-devin-volts-conversion-to-amps/6910
```

---
## \#34 Posted by: professor_shartsis Posted at: 2018-04-24T17:25:11.101Z Reads: 58

```
http://engineeronadisk.com/V2/notes_labs/engineeronadisk-335.gif

http://engineeronadisk.com/V2/notes_labs/engineeronadisk-91.html

https://upload.wikimedia.org/wikipedia/commons/thumb/5/52/Buck_operating.svg/600px-Buck_operating.svg.png

https://upload.wikimedia.org/wikipedia/commons/6/63/Buck_chronogram.png

https://en.wikipedia.org/wiki/Buck_converter
```

---
## \#35 Posted by: Mathias Posted at: 2018-04-24T17:53:08.293Z Reads: 54

```
Oh, yeah you're right. I just got some major deja vu from my discussions with @devin and didn't read your post properly, sorry :joy:. I already saw him explaining me that the current here is "bucked up" from 36.9 A to several kA and that the power is several 10 kW...

Anyway, you're right and I was trying to say the same thing more or less. Duty DC is here limited indirectly by the current...
```

---
## \#36 Posted by: Juvaknin Posted at: 2018-04-24T18:14:51.007Z Reads: 51

```
Yessss thanks guys!
It was the hybrid!... when i change to hybrid its fly on hill like crazy...!
Now i get the 20A limit all the way. That was it :slight_smile: thanks!
```

---
## \#37 Posted by: Mathias Posted at: 2018-04-24T19:13:06.518Z Reads: 48

```
Awesome! F**k hills. That's how it shoud be!
```

---
## \#38 Posted by: Hummie Posted at: 2018-04-24T20:07:13.010Z Reads: 45

```
[quote="professor_shartsis, post:34, topic:53341"]
en.wikipedia.org

Buck converter

A buck converter (step-down converter) is a DC-to-DC power converter which steps down voltage (while stepping up current) from its input (supply) to its output (load). It is a class of switched-mode power supply (SMPS) typically containing at least two semiconductors (a diode and a transistor, although modern buck converters frequently replace the diode with a second transistor used for synchronous rectification) and at least one energy storage element, a capacitor, inductor, or the two in combin...
[/quote]

hummm sure sounds like converting volts to amp as its the same total wattage at the end.  give me my ten back!

any outside judges who can put in their cents?  the bet was that the esc converts voltage to amps or not.
```

---
## \#39 Posted by: professor_shartsis Posted at: 2018-04-24T21:54:28.535Z Reads: 40

```
[quote="Mathias, post:35, topic:53341"]
I already saw him explaining me that the current here is “bucked up” from 36.9 A to several kA and that the power is several 10 kW…
[/quote]

It might be possible for a few milliseconds at very low speed with a low resistance motor and 100% duty... though a vesc is fail-safe programmed within the firmware to limit motor current below 120a.

((50v battery * 100% duty) - 0v bemf) / 0.025 ohm motor winding = 2000a motor current

2000a motor current * (50v battery * 100% duty) = 100000w (100kw)
```

---
## \#40 Posted by: Mathias Posted at: 2018-04-25T02:12:42.787Z Reads: 41

```
[quote="Hummie, post:38, topic:53341"]
the bet was that the esc converts voltage to amps or not.
[/quote]
We're picking this up again :joy:. So be it...
Yeah, voltage is converted to amps but nowhere near the way @devin imagined. It's the story of having the current in a loop with an inductance (aka the motor) and the current basically going "in a circle" without going up against the battery voltage. This is the reason why motor voltage can be much higher than battery voltage.

[quote="Hummie, post:38, topic:53341"]
as its the same total wattage at the end
[/quote]
Nope, that's exactly the point of duty cycle: to NOT have the same power at the end, but less. 
[quote="professor_shartsis, post:39, topic:53341"]
It might be possible for a few milliseconds at very low speed with a low resistance motor and 100% duty… though a vesc is fail-safe programmed within the firmware to limit motor current below 120a.

((50v battery * 100% duty) - 0v bemf) / 0.025 ohm motor winding = 2000a motor current

2000a motor current * (50v battery * 100% duty) = 100000w (100kw)
[/quote]

Nah, that's not what @devin was talking about. I don't recall completely but I think  his "theory" was something like at 1 ohm and short you get 42 A at 42 V = 1762 W, and 100% DC, so at 10% DC current gets "bucked up" to 1/10% *42 A = 420 A motor current and therefore 420 A * 42/10 V = 1764 W or something. It was complete nonsense. The idea was that there is always the same power leaving the system, which makes no sense whatsoever.
```

---
## \#41 Posted by: lrdesigns Posted at: 2018-04-25T05:01:21.427Z Reads: 36

```
Please un-check this box. If you happen to hit 60k ermp while ridding it will apply the breaks, then your face will meet the road.

![image|482x500](upload://mivDP3Rr2RpaVmIXpo5Df7MjqTs.jpg) 

In regards to the duty cycle, hit full throttle with the wheels in the air and check the telemetry. Then do the same going half speed or going up a hill.  See the results.
```

---
## \#42 Posted by: professor_shartsis Posted at: 2018-04-25T05:27:10.670Z Reads: 37

```
https://image.ibb.co/esRHUH/40duty.jpg

[quote="Mathias, post:40, topic:53341"]
It was complete nonsense. The idea was that there is always the same power leaving the system, which makes no sense whatsoever.
[/quote]

looking at the original poster's data:

39.1v pack voltage * 15.1a battery current = **590.41w** electrical

(39.1v pack voltage * 40% duty) * 36.9a motor current = **577.11w** electrical

(15.64v effective voltage) * 36.9a motor current = **577.11w** electrical

the difference is likely caused by either a combination of iron & esc losses, or possibly decimal rounding inaccuracy of the duty cycle value in the logging app.
```

---
## \#43 Posted by: Juvaknin Posted at: 2018-04-25T07:08:47.761Z Reads: 32

```
Yes. Thanks :slight_smile:
```

---
## \#44 Posted by: Mathias Posted at: 2018-04-25T07:08:49.204Z Reads: 32

```
Yeah, I know. You're totally right. Devin's math was more like:
40 V , 1 ohm = 40 A = 1600 W
10% duty cycle = 4 V * 400 A = 1600 W  BUCKED DOWN! LOGIC! WHY CAN'T YOU EXPLAIN WHERE I'M WRONG! I WILL WRITE 4 ANSWERS TO MY OWN POST!

There are probably 3 topics with 300+ post each by devin about this, and I really really really do not want to revive him. He tends to return as @devin2, @devin4... I'm almost scared of speaking it out.  Like saying "Candyman" 3 times...:joy:
```

---
## \#45 Posted by: professor_shartsis Posted at: 2018-04-25T14:17:28.243Z Reads: 28

```
[quote="Mathias, post:44, topic:53341"]
Yeah, I know. You’re totally right. Devin’s math was more like:

40 V , 1 ohm = 40 A = 1600 W

10% duty cycle = 4 V * 400 A = 1600 W  BUCKED DOWN! LOGIC! WHY CAN’T YOU EXPLAIN WHERE I’M WRONG! I WILL WRITE 4 ANSWERS TO MY OWN POST!
[/quote]

if the winding resistance in this example is in fact 0.01ohm then it seems correct.

((40v battery * 10% duty) - 0v bemf) / 0.01ohm winding = 400a motor current

(40v battery * 10% duty) * 400a motor current = 1600w electrical

(4v effective) * 400a motor current = 1600w electrical

you can calculate the instant back emf voltage to use in this equation by dividing the instant rpm by the kv... for example 1000rpm / 100kv = 10v back emf voltage

so if we assume the motor is 100kv and presently turning 1000rpm, then:

((40v battery * 35% duty) - 10v bemf) / 0.01ohm winding = 400a motor current

(40v battery * 35% duty) * 400a motor current = 5600w electrical

(14v effective) * 400a motor current = 5600w electrical

5600w electrical / 40v battery = 140a battery current

though again, vescs are fail-safe programmed within the firmware to limit motor current below 120a despite any user settings.
```

---
## \#46 Posted by: Mathias Posted at: 2018-04-25T15:14:45.222Z Reads: 19

```
DC of 10% doesn't push 10 times more current than 100%.
```

---
## \#47 Posted by: professor_shartsis Posted at: 2018-04-25T15:18:04.913Z Reads: 21

```
[quote="professor_shartsis, post:45, topic:53341"]
((40v battery * 10% duty) - 0v bemf) / 0.01ohm winding = 400a motor current
[/quote]

[quote="professor_shartsis, post:45, topic:53341"]
(4v effective) * 400a motor current = 1600w electrical
[/quote]

[quote="Mathias, post:46, topic:53341, full:true"]
DC of 10% doesn’t push 10 times more current than 100%.
[/quote]

https://image.ibb.co/djfOKH/1600w.jpg

https://image.ibb.co/fWDkGx/160kw.jpg
```

---
## \#48 Posted by: Mathias Posted at: 2018-04-25T15:24:58.043Z Reads: 18

```
Now you're trolling, @devin :joy: . The motor had 1 ohm at 100%. At 10% DC the motor windings still have one ohm.
```

---
## \#49 Posted by: professor_shartsis Posted at: 2018-04-25T15:34:51.677Z Reads: 18

```
https://image.ibb.co/iyeswx/IMG_4666.jpg

^you can estimate the resistance of your motor + vesc by using your throttle with the motor stalled

in this case we have 20a battery current, 78a motor current, 49.7v battery voltage

49.7v battery voltage * 20a battery current = 994w

994w & 78a motor current into the ohm's law calc (0v bemf - stalled)

https://image.ibb.co/fmoGpH/994w.jpg

this gives roughly 0.163ohm for the motor winding + vesc.

effective voltage for 20a battery current with the motor stalled in this case is ~12.74v effective. (49.7v battery)

the largest source of error in this method is the battery voltage was actually a bit lower than 49.7v while the 20a battery amps were drawn due to voltage sag -- so the electrical wattage in this case was in fact a bit lower than 994w while the 20a battery amps were drawn.
```

---
## \#50 Posted by: Mathias Posted at: 2018-04-25T15:42:27.853Z Reads: 18

```
Dude, yes. I know. 

Last try, then I'm out. I know that you know that the meaning of DC is not that DC of 10% pushes 10 times more current than DC 100%. And that the power at DC 10% is lower than at DC 100%. That's all I was saying. 

I'm too scared of summoning Devin5 to continue.
```

---
