# How many amps do you pull on your setup?

### Replies: 23 Views: 7462

## \#1 Posted by: willpark16 Posted at: 2016-05-11T06:49:29.478Z Reads: 462

```
I thought it was about time to start a thread on the amp draw of different setups. So include specs and how many amps you pull on average continuous and how many u peak.
```

---
## \#2 Posted by: lowGuido Posted at: 2016-05-11T06:54:13.374Z Reads: 466

```
average around 5 Amp draw on my 6S single SK3
```

---
## \#3 Posted by: trbt555 Posted at: 2016-05-11T07:06:00.349Z Reads: 463

```
12S single R-SPEC 6355/190 -> 30A peak
```

---
## \#4 Posted by: makevoid Posted at: 2016-05-11T07:11:48.504Z Reads: 462

```
6S setup, enertion RSpec 6372

From the measurement I did when I had the wattmeter plugged in between the battery and the FVT ESC:
10-20 Ah  when accelerating slowly and cruising (~250/500Wh) and 40Ah (900Wh) at peak (accelerating full throttle uphill)

On the VESC, initially I had configured motor max as 40A and then 50A but I had not enough power to accelerate strongly uphill (I weigh 95kg), after I changed it to 60A I never experienced cut-offs so I guess the max drain will be around 55A.

My question is, if I had a 12S setup then I could set motor max to 30-40A and not experience cut offs in theory isnt it?
```

---
## \#5 Posted by: willpark16 Posted at: 2016-05-11T07:16:48.594Z Reads: 439

```
yes in theory that would be correct it also depends on terrain and gearing too
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-05-11T08:38:16.816Z Reads: 424

```
@willpark16 you're on a tear today ... Go take a nap or something .... Even better .... Go Skate
```

---
## \#7 Posted by: willpark16 Posted at: 2016-05-11T15:15:43.986Z Reads: 396

```
haha just took my nap
```

---
## \#8 Posted by: Karmannghiagirl Posted at: 2016-05-11T15:26:44.463Z Reads: 384

```
So with amperages sounding so low, why does everyone use really high amperage ESCs? couldnt you use a 45-60A car ESC if you barely hit 40A?
```

---
## \#9 Posted by: makevoid Posted at: 2016-05-11T15:33:58.308Z Reads: 375

```
To **keep** the mosfets (a.k.a. FETs) of the ESC **cool**. 
They handle most of the current in the ESC, they switch and modulate the current from battery to motor (electrical side of the things, the main chip instead, the DRV in case of VESCs, sends low voltage pulses to them to control their output current)
```

---
## \#10 Posted by: willpark16 Posted at: 2016-05-11T15:34:20.229Z Reads: 367

```
im assuming everyone is using the vesc. This allows them to run there motor at its optimum
```

---
## \#11 Posted by: Karmannghiagirl Posted at: 2016-05-11T15:45:03.616Z Reads: 363

```
couldn't you just mod one and add a massive heatsink ?

or maybe go crazy and do water cooling or submerged oil cooling :imp:
```

---
## \#12 Posted by: makevoid Posted at: 2016-05-11T15:50:15.315Z Reads: 353

```
yes, people put small heatsinks that have adhesive tape on them (like [these](https://www.amazon.co.uk/s/?field-keywords=raspberry%20heatsink)) or thermal glue to keep them cool, or even a piece of metal so the dissipation surface is increased, also if you add more code to the VESC that does extra calculations is recommended to cool the main chip down as well.
```

---
## \#13 Posted by: Karmannghiagirl Posted at: 2016-05-11T15:56:25.215Z Reads: 348

```
Im talking about a car esc, not the vesc
```

---
## \#14 Posted by: makevoid Posted at: 2016-05-11T16:09:24.081Z Reads: 341

```
Yes, these things apply to any ESC, every ESC has a chip that is the "brain" of the ESC, and does the calculation for draining and outputting the right current based on the receiver's input, battery and motor status, and that chip, like the FETs, has to be kept cool as well.
```

---
## \#15 Posted by: Karmannghiagirl Posted at: 2016-05-11T16:11:38.416Z Reads: 338

```
ah, i see what your saying now.
```

---
## \#16 Posted by: trbt555 Posted at: 2016-05-11T16:22:22.968Z Reads: 332

```
CSI

Chinese Spec Inflation
```

---
## \#17 Posted by: chaka Posted at: 2016-05-11T16:41:46.158Z Reads: 324

```
Average 600 watts and max out at 3500 watts when accelerating on a dual drive.
```

---
## \#18 Posted by: Hummie Posted at: 2016-05-11T16:46:54.437Z Reads: 327

```
I've been planning forever to pot my vescs since then they wouldn't be suffering the physical abuse that they get otherwise and according to Chaka and Vedder the vesc's fets are the only heat source that I'd need to worry about and shouldn't be potted.

  The brain doesn't get that hot?

I have so much potting resin but am still afraid to do it.  Wouldn't need an enclose just glue it to the board with the potting resin. 
How fragile are the fets? I planned to have them exposed and just covered with stick-on heatsinks.
```

---
## \#19 Posted by: claudiofiore88 Posted at: 2016-05-12T00:27:40.117Z Reads: 314

```
[quote="Karmannghiagirl, post:8, topic:3116, full:true"]
So with amperages sounding so low, why does everyone use really high amperage ESCs? couldnt you use a 45-60A car ESC if you barely hit 40A?
[/quote]

Main reason is lower amp car esc's are less than 6s.
```

---
## \#20 Posted by: Okami Posted at: 2016-07-16T07:30:38.096Z Reads: 295

```
Hello everyone! A topic about what is the real amp draw / current needs for a system surfaced on another topic.

So, gladly @DeathCookies made a simple template for everyone to enter their data into 

Although, it is still in beta stage and needs to be improved!
---

---
Any feedback / improvements would be great!

-----

 Poll for entering Amp draw data:
--------

http://gct-hp.de/esk8/index.php
----

<img src="/uploads/db1493/original/2X/8/80b166bf3bc2b048f4577d7bb1101aae4ad215f0.png" width="195" height="195">


---

We don't have a seperate topic for feedback / improvements yet, so you could contact @DeathCookies by messaging him. 

---
I can invite everyone to our conversation, if someone is up to contribute more in creating this tool.
```

---
## \#21 Posted by: Okami Posted at: 2016-07-16T07:32:20.816Z Reads: 282

```
Original disccusion started on this thread:
http://www.electric-skateboard.builders/t/sanyo-ncr-18650ga/6140/24

Here is what @whitepony posted:
[quote="whitepony, post:25, topic:6140"]
someone should start a thread about this and collect data properly. with enough and properly verified data, one could maybe have a hit on quite a few interesting topics: single vs. double motor, 63 vs 50mm, foc vs bldc, vesc vs. other escs, impact of KV values, impact of wheel choices and and and!
[/quote]

Which may give a hint to which direction should we start going, as his suggestion is more detailed than what I suggested.
```

---
## \#22 Posted by: whitepony Posted at: 2016-07-16T07:38:48.301Z Reads: 267

```
nice effort! :slight_smile: not sure if this worked though - had a weird result screen after submit. also I got a lot of suggestions since many things arent clear enough and allow various funky inputs:

gear ratio -> example of input in brackets (16/36, 1:2, ...)
wheel size -> add unit (mm)
board weight -> add unit (kg)
rider weight -> add unit (kg)
battery voltage -> add "nominal"
battery capacity -> add unit (Ah)
C-Rating -> floating number with "," or "."?
imo: add "Continuous Current (A)" and calculate C-Rating and vice versa!

peak draw -> add unit (A) or power (W)
average draw -> add unit (A) or (W)
max speed -> add unit kph, mph or m/s
energy consumed -> add unit (Wh)
watt/hour per mile -> thats wrong, change to Wh/mile (I prefer Wh/km obviously)
Energy consumed -> add unit Wh

Hill Time -> add "in % of total ride"
Average incline -> add "in %"

the lower 4 entries are supposed to be what?

max wattage used -> max power used in units (W)
avg wattage used -> avg power used in units (W)
watt/hour -> not sure what that is supposed to be?
wat/hour per mile -> Wh/mile


imo, to the right of the entries should be an example template completely filled out so that people can at least see if their numbers make ANY sense at all. not everyone is firm with basic physics, units, etc!

also, please no unnecessary input:
from avg speed, distance and energy consumed, the script should calculate avg draw and Wh/mile on its own - no need for the user to calculate all that imo.

personally I would also add ESC & commutation mode (maybe as text like you did for motor), single/dual/quad config and belt/hub (which is probably halfway clear with gearing)!

p.s.: dont have access to that link: http://www.electric-skateboard.builders/t/custom-poll/6171
```

---
## \#23 Posted by: Okami Posted at: 2016-07-16T11:00:32.369Z Reads: 232

```
... (wrong place)
```

---
