# How connect mini fan for MTB

### Replies: 19 Views: 1159

## \#1 Posted by: Devilmycry Posted at: 2017-11-27T02:17:06.121Z Reads: 123

```
Hi everyone 
It is my thirst building 
I building MTB 
12s7p
But I need some fan for my VESC the fan I have is 12v 0.4A 
What I have to do for connect it 
Use UBEC but which one 
Thank you
```

---
## \#2 Posted by: ThermalM16 Posted at: 2017-11-27T04:48:38.450Z Reads: 117

```
I did some math. You need a 95 Ohm resistor on your fan. Just make sure its large enough so it doesn't let its magic smoke out right away. Hopefully I did that right haha. Here's a pic of how I set it up <img src="/uploads/db1493/original/3X/a/d/adb57b0162ea32439db951ba68683f08cff0a799.jpg" width="374" height="500">
```

---
## \#3 Posted by: ugothakd Posted at: 2017-11-27T04:52:23.108Z Reads: 98

```
Vesc has a built in 5v 1amp for running external devices
```

---
## \#4 Posted by: Devilmycry Posted at: 2017-11-27T05:45:54.775Z Reads: 93

```
I have the VESC from trampa 
And my fan is 12v 0.4A
```

---
## \#5 Posted by: Devilmycry Posted at: 2017-11-27T05:46:05.105Z Reads: 91

```
Ok thank you man
```

---
## \#6 Posted by: Devilmycry Posted at: 2017-11-27T05:51:20.838Z Reads: 87

```
Thank you do you have a link for buy it 
Thank you resistor
```

---
## \#7 Posted by: ThermalM16 Posted at: 2017-11-27T06:17:51.874Z Reads: 87

```
@Devilmycry One thing I forgot to mention is your fan is about 5 watts so you’ll want a resistor that can handle that. 95 Ohm is going to be impossible to find unless you attach multiple in series, but for simplicities sake let’s round up to 100 ohm. Here’s a link for a 5w and 20w variant. 5w is sufficient, 20w is overkill. 

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F282435019995

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F391680061558
```

---
## \#8 Posted by: JdogAwesome Posted at: 2017-11-27T06:53:49.396Z Reads: 78

```
Idk why your using a giant resistor that's going to create a ton of heat to then try and cool your VESC lol, quite counterintuitive.  Id recommended just getting a proper UBEC or buck converter that can handle your input voltage and buck down to 12V to power the fan and anything else you need at 12V i.e. lights, more fans... more lights?
```

---
## \#9 Posted by: Nowind Posted at: 2017-11-27T08:11:57.453Z Reads: 71

```
Get[quote="Devilmycry, post:4, topic:39411"]
And my fan is 12v 0.4A
[/quote]


Get a Fan for 5V , "Yeah Racing" make some really nice ones...
Or use a step down converter, but dont use a resistor IMO

BTW
Try it with some passive cooling like an Aluminium Plate, all i need in my MTB builds...

Regards
```

---
## \#10 Posted by: jmasta Posted at: 2017-11-27T08:29:43.903Z Reads: 68

```
Your math is right, but you only did half of the calculations 

R = (50-12)V / 0.4A = 95 ohm resistor needed 

But...

P = (95 ohm)*(.40A)^2 = 15.2 Watts power dissipated 

Dissipating that much power is going to generate a ton of heat. 15W is a lot.  As others have mentioned, either get a 12V BEC capable of 50V input, or buy a 5V fan and use the VESC to power it through a spare port on your receiver.  Personally I use a 12V BEC for my fan but it also powers my lights. Go with a 5V fan if you don't have any other accessories
```

---
## \#11 Posted by: scepterr Posted at: 2017-11-27T08:33:03.778Z Reads: 62

```
https://www.electric-skateboard.builders/t/eskate-lights-thread/199/467
```

---
## \#12 Posted by: Erniechan Posted at: 2017-11-27T10:44:06.650Z Reads: 48

```
I'd buy a 5v fan. They are dirt cheap.
```

---
## \#13 Posted by: ThermalM16 Posted at: 2017-11-27T13:26:16.210Z Reads: 45

```
Thanks for that correction. That’s what I get for trying to do math before bed
```

---
## \#14 Posted by: ThermalM16 Posted at: 2017-11-27T13:27:55.403Z Reads: 46

```
Everyone here has a good point, 5v fans are super cheap. If I recall you can get 10 packs from eBay for $15 or less.
```

---
## \#15 Posted by: Acido Posted at: 2017-11-27T14:01:00.440Z Reads: 42

```
just buy a 5v fan and solve the problems
```

---
## \#16 Posted by: JdogAwesome Posted at: 2017-11-27T15:23:55.548Z Reads: 42

```
Hey and instead of doing all the math on paper there's a bunch of free calculators online that make it quite simple. I use two apps especially, Electronics Calculator and ElectroDroid both are apps on my phone. Oh and your math for the 95ohm resistor is wrong, so is @jmasta the value should actually be 125Ohm's. 
EDIT: Oh and the actual wattage is 20W not 15.2 (125)*(0.4)^2 = 20
<img src="/uploads/db1493/original/3X/0/0/00216ba16b1301addcaf00f1d7a4e75c00bc4a5a.png" width="395" height="500">
```

---
## \#17 Posted by: jmasta Posted at: 2017-11-27T15:36:27.548Z Reads: 38

```
That's not correct. You don't need an app to calculate Ohm's law. Blindly applying equations leads to incorrect results. I literally typed that from my phone in bed

All your app is doing is:  50/0.4 = 125, which is wrong here

The voltage drop across the resistor should be 50-12= 38V. Not 50V

The point is moot anyway. Don't use a resistor to drop so much voltage
```

---
## \#18 Posted by: ThermalM16 Posted at: 2017-11-27T15:41:33.127Z Reads: 37

```
@jmasta is correct. I use them to drop 8v to 5v for fans, the heat coming from it is going to cause problems in a confined space. Switching to a 5v fan and using a BEC is not the cheapest idea, but it’s the smartest, most practical, and probably cheapest long term.
```

---
## \#19 Posted by: JdogAwesome Posted at: 2017-11-27T19:04:46.021Z Reads: 31

```
God I'm an idiot lol, I guess that's what I also get for trying to do this right before bed lol. Sorry I was thinking of using the resistor as current limiting like in an LED not for the voltage drop, my bad. Anyways  I also mentioned the two apps I use not for ohms laws calculations but for more advanced stuff like, heat dissapation, SMD Codes, voltage dividers, V drop calcs, ect.
```

---
