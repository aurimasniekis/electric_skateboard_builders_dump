# Smoking Motor! Any help appreciated

### Replies: 18 Views: 1517

## \#1 Posted by: darkkevind Posted at: 2016-11-03T20:12:06.267Z Reads: 125

```
Hi everyone,
I'm hoping you guys can help me find out why my motor is fried and smoking after a few test rides...

Here is my video to demonstrate my issue: http://www.youtube.com/watch?v=13hamBiqeLQ

Test riding I used 1 3S 11.1v 5000mah LiPo, and two different types of ESC, one initially 45A, then an 80A. All was good, but then after a while something would cut out and then I'd intermittently get power to the motor, at this point the motor and ESC were quite hot.
I thought the issue was the ESC and not enough AMPS, so I got a 120A ESC, added another battery in serial and now, on the bench, my motor fried! Like, smoking fried!

Why did this happen? Any help is very much appreciated :slight_smile:
```

---
## \#2 Posted by: ArmandR Posted at: 2016-11-03T20:15:04.342Z Reads: 116

```
what kv?

10
```

---
## \#3 Posted by: Blasto Posted at: 2016-11-03T20:18:06.473Z Reads: 112

```
[quote="ArmandR, post:2, topic:12409"]
what kv?
[/quote]

from the video 580Kv

You're running a very low voltage and very high currents, I would suggest going at least 6S with a lower KV motor (it's toast anyways)
```

---
## \#4 Posted by: ArmandR Posted at: 2016-11-03T20:18:57.842Z Reads: 106

```
yeah 580 kv with 3s is very bad.
```

---
## \#5 Posted by: Hummie Posted at: 2016-11-03T20:27:19.900Z Reads: 100

```
did it smoke when you throttled or without throttle?  if with throttle I bet the motor is shorted, if without throttle, that would be weird and mean the esc is probably the problem.
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-11-03T20:29:30.504Z Reads: 95

```
Hoooooly dude ....it was kinda awesome.
```

---
## \#7 Posted by: darkkevind Posted at: 2016-11-03T20:30:44.312Z Reads: 93

```
With throttle only. How can I test if the motor is shorted? Does that basically mean it's beyond salvaging?
```

---
## \#8 Posted by: darkkevind Posted at: 2016-11-03T20:32:26.209Z Reads: 90

```
Initially when I was using only one battery (3s) it was fine, it only started doing this when I added a second battery to make it 6s (in serial).
```

---
## \#9 Posted by: chinzw Posted at: 2016-11-03T21:32:25.180Z Reads: 85

```
That smoke is probably the phase wire insulation. Open up the motor and check it out, you will see "charcoal" around the wires. Once you're done, throw that away and get a decent motor with kv < 230, and since you're using single motor go for a 63mm one not 50
```

---
## \#10 Posted by: darkkevind Posted at: 2016-11-03T21:36:56.748Z Reads: 81

```
[quote="chinzw, post:9, topic:12409, full:true"]
throw that away and get a decent motor with kv < 230, and since you're using single motor go for a 63mm one not 50
[/quote]

Is that really a thing? Does it need to be such a beefy motor? Admittedly I'm around 83kg (185lbs), but I'm sure a 50mm is powerful enough isn't it?

I'm quite the novice as you can tell, why is the low KV so important? I realise the lower the KV the more torque it has...
```

---
## \#11 Posted by: darkkevind Posted at: 2016-11-03T21:38:28.081Z Reads: 74

```
What's wrong with this motor?
http://alienpowersystem.com/shop/brushless-motors/alien-5065-sensored-outrunner-brushless-motor-270kv-2200w-2/
```

---
## \#12 Posted by: chinzw Posted at: 2016-11-03T21:47:05.482Z Reads: 70

```
this is totally wrong, but take it as an example.
a 50cc motor will struggle to move you around, but an 80cc motor will do just fine.
Same goes for 50mm vs 63mm
```

---
## \#13 Posted by: darkkevind Posted at: 2016-11-03T21:55:38.921Z Reads: 69

```
Hmmm I take your point. Just thought 50mm would be sufficient (as per your 80cc example). Thanks for the feedback. I'll probably swap it out for a Turnigy SK3 192kv 63mm.
```

---
## \#14 Posted by: Hummie Posted at: 2016-11-03T22:15:52.402Z Reads: 68

```
the kv shouldn't matter enough to send it smoking.  if it's a higher kv it just means it needs more amps to get that torque, but not any more heat...you'll get the same torque to heat ratio regardless of the kv.  I bet it's shorted somewhere.  Using the vesc it's easy to test but without...a multimeter likely wont do it.   you could use an inductance meter.
```

---
## \#16 Posted by: darkkevind Posted at: 2016-11-03T22:27:03.295Z Reads: 60

```
[quote="Hummie, post:14, topic:12409, full:true"]
...a multimeter likely wont do it.   you could use an inductance meter.
[/quote]

Is this one OK? http://www.ebay.co.uk/itm/like/221756531542?lpid=122&chn=ps&adgroupid=35959456040&rlsatarget=pla-260812202149&adtype=pla&poi=&googleloc=9045031&device=c&campaignid=661151662&crdt=0

How would I test it? Sorry, I'm pretty handy but I'm no electronics guru (as you can tell!).
```

---
## \#17 Posted by: darkkevind Posted at: 2016-11-03T22:30:23.252Z Reads: 56

```
What I don't understand is that when using one battery, I've been on several test rides since I built it, and only had something overheat after a few miles...
This has only happened since adding the second battery and the new ESC. Before that I clocked the speed with the GPS on my phone (some kind of GPS HUD app), and it topped out at 20mph. I did have to kick the board of manually though otherwise it didn't really like starting off with me on it by itself, but I did that every time.
```

---
## \#18 Posted by: Hummie Posted at: 2016-11-04T02:36:59.616Z Reads: 48

```
Did u try going back to the old esc? 

 Or maybe you should check the motor first.  That multimeter might probably is good
```

---
## \#19 Posted by: TheRedPanda Posted at: 2016-11-04T04:12:13.586Z Reads: 39

```
The low voltage 3S (11.1V) was causing your motor to have very little power, to achieve the max wattage of a motor you must have a certain voltage. It's similar to how a combustion engine has a power curve, where you produce the most power(torque x RPM) at a certain RPM, say at 6500RPM you might be able to generate 400HP but at 3000RPM you might only generate 350HP. That's why when you have a gasoline engine in it's upper rev limits the engine tends to be more responsive or jumpy, it's the extra torque that's making it do that. 

If you look when buying a brushless motor a common specification is"X" Watts at "X"S (ex:8S). 

On a related note, neodymium magnets are sensitive to heat in that over time heat demagnetizes them, and if you surpass their temperature rating they will demagnetize below their rated strength and never return back to full strength. As the magnets become less magnetic that makes your motor less efficient because your stator has to put out more power to result in the same force on the magnets thereby causing the stator to run hotter than it usually would. This sort of cycles back and forth, one overheating leading to the other until usually the enamel on the windings start melting which is likely what is causing the smoke in this situation. Your motor may still be operational if you use a higher voltage but the motor is permanently running at a decreased power. I would recommend purchasing a new motor and atleast a 6S battery pack.
```

---
