# \[Investigation\] VESC DRV8302 failures

### Replies: 28 Views: 2209

## \#1 Posted by: Mike_Lemon Posted at: 2017-08-26T21:41:24.744Z Reads: 231

```
Hello and welcome,

I'd like to investigate why the VESC keeps failing sins it's a very expensive problem and very dangerous.

the most common failures of most VESCs I've seen accrue from the DRV8302 just being fried up after or during a ride not even maxing out the current or voltage setting of the VESC.
this mostly happens when people use FOC settings(but was kinda "FIXED" after adding a capacitor) but also happens of the other setting.

Does anybody know why this happens and what can you do to prevent it?

This will just help improve our only option of motor controller and prevent further dead VESCs for the graveyard.

Thanks for the contributers.
```

---
## \#2 Posted by: BenTheBarre Posted at: 2017-08-26T21:44:27.457Z Reads: 221

```
I am also very curious on this topic. It would be awesome to have a data base of all the possible ways the DVR can fail, in order for VESC users to diagnose/trouble shoot.
```

---
## \#3 Posted by: JdogAwesome Posted at: 2017-08-26T21:44:53.343Z Reads: 217

```
From what I can tell and what makes sense is that the DRV dies because of high voltage inductive spikes from the motor. Adding more capacitance to C18 like what Ollin VESC's do helps smooth those voltage spikes.
```

---
## \#4 Posted by: jmasta Posted at: 2017-08-26T21:51:56.529Z Reads: 209

```
Always install new firmware on any new VESC.  My VESC is fried from a DRV8302 failure because Torqueboards/DIY sent me a VESC with bugged firmware.  Pretty disappointing when I purchased it months after the current ramp bug had been reported.  Unfortunately there is no way to tell if you have the bad firmware or not, because Benjamin Vedder did not change it to 2.19.  They are both 2.18
```

---
## \#5 Posted by: Mike_Lemon Posted at: 2017-08-26T22:19:56.146Z Reads: 197

```
I know inductive spiking in speakers and DC motors can be solved bu adding a shotkky diode parallel to the load in reverse. couldn't that be the solution for the VESC as well?
```

---
## \#6 Posted by: Mike_Lemon Posted at: 2017-08-26T22:20:35.585Z Reads: 195

```
How can you be sure it is the firmware? the VESC needs to be protected hardware wise as well...
```

---
## \#7 Posted by: jmasta Posted at: 2017-08-26T22:28:24.437Z Reads: 192

```
There are multiple failure modes which can lead to a DRV error.  Bugged firmware is one of them. Unknowingly running a maxed out current ramp step of 50, instead of the default 0.04, is a surefire way of destroying your VESC.  It's a precaution, not an end-all solution...
```

---
## \#8 Posted by: JdogAwesome Posted at: 2017-08-26T22:29:30.206Z Reads: 190

```
The VESC already has a Shottky Diode in it, its D4 Shottky 60V 2A. the diode does help with reverse voltage spikes but clearly not enough. @jmasta was just saying its one thing that can lead to a dead VESC or DRV.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-08-27T00:16:20.466Z Reads: 184

```
Another scenario that can kill a vesc is coasting downhill too fast and then applying the brakes.
Seems that you can exceed the erpm limit with negative as well as positive torque.
```

---
## \#10 Posted by: BenTheBarre Posted at: 2017-08-27T00:46:38.544Z Reads: 181

```
 inductive voltage spikes can occur because of lengthy power wires between the VESC and the battery, correct? In my build, I have a split enclosure in which there is some space(about 10 inches) between the batteries and the VESC, and I just experienced a fried DRV. I also, by accindent, had the ERPM limits set to - and + 100k. Could the long wires could have been the culprit of the ruined VESC?  Or was it the ERPM setting It happened after braking for the first time after going 15 ish mph. (This was all with a torque boards VESC)

Thanks:)

Also, what would be considered the safe length of power wires from the battery to VESC?
```

---
## \#11 Posted by: Mike_Lemon Posted at: 2017-08-27T02:36:16.705Z Reads: 168

```
If doesn't help enough why not add another one in parallel?
```

---
## \#12 Posted by: Mike_Lemon Posted at: 2017-08-27T02:36:50.205Z Reads: 169

```
I don'y think it has anything to do with the length of your wires.
```

---
## \#13 Posted by: chuttney1 Posted at: 2017-08-27T05:50:41.513Z Reads: 171

```
Some of the errors that caused for failure are if you soldered it by hand and the ground pad wasn't connected, it happens. Aside from that, most DRV errors are a result of wrong settings or running on 12S and some spike in current or voltage. Obviously, the VESC wasn't designed to take extra current and burn it off. The brake function wasn't designed to work as a real brake on long down hill stretches.
```

---
## \#14 Posted by: Mike_Lemon Posted at: 2017-08-27T07:49:56.928Z Reads: 159

```
Do you have an example for bad settings besides FOC?

Also the design of the VESC needed to assume the brake would always work as hard as it can without damaging it....
```

---
## \#15 Posted by: Namasaki Posted at: 2017-08-27T13:25:13.479Z Reads: 145

```
[quote="chuttney1, post:13, topic:31545"]
The brake function wasn't designed to work as a real brake on long down hill stretches.
[/quote]

I run my brakes continuously down steep hills and sometimes on a full battery and have had no issues. 
I do use moderate settings for motor and battery min. 
And I'm running dual setup so the load is divided. 
Motor min -40a
Battery min -10a
```

---
## \#16 Posted by: Deckoz Posted at: 2017-08-27T14:17:46.456Z Reads: 144

```
I think my first one originated from this vreg which blew pin 29 on the DRV 
<img src="/uploads/db1493/original/3X/d/0/d0b20cbac5b149305e43a32835b600e55f45368c.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/0/3/031085dd73cfe9207adfddf2b1f2fa293fa068e2.jpg" width="374" height="499">

My second one is from freewheeling downhill and then braking while at a higher then max erpm(39mph, on my setup would be about 67k erpm). No fancy pictures for this one(no burns) just DRV fault.

Downhilling and holding the brake and staying at a speed that is under the erpm limit to your gearing is fine. But freewheeling faster and braking popped my DRV in half a millisecond. As the above poster said running brakes down a hill all the way on a full battery is fine as well. Its just braking while higher then 60k erpm ie I would be at 60kerpm at 35.4mph but I was going 39 when I braked...poof :) 

The good thing is if you built your board right you should never even be close to max erpm of the 4.12 while motors are under power(throttle) within your geared speed - unless your running 12s
```

---
## \#17 Posted by: onepunchboard Posted at: 2017-08-27T14:21:03.754Z Reads: 143

```
mine is longer than 10 inch.
```

---
## \#18 Posted by: Deckoz Posted at: 2017-08-27T14:29:40.383Z Reads: 144

```
Hahaha I read this wrong and forgot the thread topic...lollll

Anyway mine is longer then 10" as well. You see with brushless motors and speed controllers the length of wire from power source to ESC doesn't matter so much, just the ESC to motor. The longer the motor to ESC wires the easier for the back emf to dissipate Down the wire and cause desyncs

My power to ESC wires are about 34 inches total
Vesc power leads are about 10" and my liion packs about 14 inches from the first pack to the terminals
<img src="/uploads/db1493/original/3X/f/1/f19a075e6f7581b7bdabdea3d68e953829c8054d.jpeg" width="295" height="500">

And then 20.5 inches up top 
<img src="/uploads/db1493/original/3X/b/7/b784092ade2a33a2fc65157f2bd677d5abfb3303.jpeg" width="295" height="500">

Power to vescs doesn't matter to much in length. Just motor to escs.
```

---
## \#19 Posted by: Minim Posted at: 2017-08-27T22:22:09.295Z Reads: 137

```
I'm not into how the vesc is designed but on RC groups there is a long thread about too long battery wires will kill your escs. I did some scope measurements to this with running a ESC completely without CAPs, then with stock caps and then at last one with 6xlow ESR capacitors wired in parallele to catch the spikes. It's not the capacitance that matters here hence why I did use many small instead of one big. Without caps I think spikes hit 35volt on a 6S system (25,2V charged). In comparison that would mean 70volt spikes on a 12S system. Could this be related to failed VESCs? It's quite common in big custom quad copters with remote installed ESC to add capacitor banks out close to the ESC to prevent failures caused by this.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-08-27T23:09:29.474Z Reads: 134

```
On my builds, the negative main is fairly short but the positive main is about a foot long 12ga silicone wire.
That has not caused any problems with over a year of operation.
Running dual Vescs 4.12
```

---
## \#21 Posted by: Minim Posted at: 2017-08-28T06:11:54.161Z Reads: 125

```
The therm "too long" is relative tho. Every centimeter will add to the spike effect since it's caused by the wires combined with the off switching/cut of high current. No clue if it applies to this but anyone with a decent oscilloscope can measure this effect with putting some load to the motors and hammering the throttle and set the trigger to for example 55-60V on a 12S system. I would be surprised if we don't see this effect on Esk8 also as the multirotors is using much of the same gear. If the caps are big enough there won't be any speak but if they are to small it will show.
```

---
## \#22 Posted by: Crossfire Posted at: 2017-08-28T08:47:58.076Z Reads: 115

```
Using the Maytech VESC on 8S/245kV setup I was happy for like 1 month of operation. Suddenly on saturday on a casual cruise it all started to act weird and left me hanging in the middle of the way returning home. 
DRV fault as usual.

After reading through the topics and opinions it's still a bit covered in mystery of why it happens so many times...even when everything is correctly setup in BLCD etc. I do think that after we build our VESC enclosures, stack them with antispark switches with DROK's, make them full and even watertight...what we do forget a bit is the airflow...I do think some kind of "ram air" like natural flow would help a lot...I mean, we can mount those little 40mm vents to blow hot air out too...I'm really starting to think all these chips are just capitulating because of lack of cooling...we can mount some passive aluminium radiators which do help but general cooling must be improved too. I'll look into it more, I'll try to monitor enclosure temp with & without decent airflow...maybe I'll run an arduino pro mini with DS18B20 to understand the correlation a bit more...

EDIT: or BT module with online data of FET temps on the phone/watch.
```

---
## \#23 Posted by: onepunchboard Posted at: 2017-08-28T16:28:17.909Z Reads: 107

```
plausible, heat increase resistance of electronics
```

---
## \#24 Posted by: scepterr Posted at: 2017-08-28T16:37:51.608Z Reads: 111

```
On the topic of cooling I've got a bunch of these coming in for testing :wink:
<img src="/uploads/db1493/original/3X/7/e/7e96bba9c3343e2ad17ef81e5507e2b587e9ef68.jpg" width="140" height="250">
<img src="/uploads/db1493/original/3X/1/f/1f63024cd6756a3d35ff71c568110ed156c7c573.jpg" width=140" height="250">
```

---
## \#25 Posted by: JdogAwesome Posted at: 2017-08-28T19:17:33.917Z Reads: 104

```
@Minim  the problem with hooking up an oscilloscope to your board is that you usually only see the voltage spikes when your actually riding your board and have some serious resistance on the wheels, like going down a hill or trying to stop a 150lbs person going 20mph. 

@Crossfire I personally have heatsinks on both sides of my VESC on the MOSFET's but adding one to the DRV is a good idea. I also have a fan inside my enclosure blowing directly on it which helped quite a bit but that's off topic.  

@scepterr those Peltier units might sounds good in theory, though the problem is that there so ridiculously inefficient there just going to create far more heat than it's worth trying to cool one side of it. They also draw a ton of power so thats another consideration.
```

---
## \#26 Posted by: scepterr Posted at: 2017-08-28T20:26:08.339Z Reads: 98

```
@JdogAwesome #forscience
Battery warm up for winter time :yum:
```

---
## \#27 Posted by: Silverline Posted at: 2017-08-28T20:27:10.013Z Reads: 98

```
Do people know / think that with the new upcoming vesc tool , we are going to have a better working fw for 4,12 hardware ?
```

---
## \#28 Posted by: goldenHusky Posted at: 2017-08-28T20:54:40.592Z Reads: 93

```
[quote="scepterr, post:26, topic:31545"]
Battery warm up for winter time :yum:
[/quote]


Sorry offtopic, but that's kinda funny, I was once involved in a project to build a remote controlled snowplower, because of the budget and weight (friction) we went with leaded batteries, like 12x 12V/15Ah and if you used some of the batteries energy to heat themselves up, you gain capacity in total because lead batteries have a ridiculous bad performance at low temperatures :joy:
```

---
