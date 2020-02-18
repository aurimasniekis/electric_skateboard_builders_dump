# What happens if: 2 motors different kv&rsquo;s

### Replies: 15 Views: 1308

## \#1 Posted by: accrobrandon Posted at: 2018-05-12T04:15:09.128Z Reads: 252

```
Let's say I have a 6355 190kv and the other is same brand..same size and 170kv and u run that on a dual setup... How does this change board performance..

I assume since one has a lower kv thats less rpms and that the one motor tops out sooner than the other in the high end? And if this is correct then is there any major issues in the low end performance?
```

---
## \#2 Posted by: Cobber Posted at: 2018-05-12T04:18:02.363Z Reads: 252

```
http://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113

:no_mouth:
```

---
## \#3 Posted by: b264 Posted at: 2018-05-12T05:18:56.043Z Reads: 239

```
Is totally fine.  Both drives will operate as they normally do -- one will be better at low-end torque and the other will be better at top speed.  Make sure the higher kv motor doesn't exceed its ESC's max erpm.
```

---
## \#4 Posted by: E1Allen Posted at: 2018-05-12T05:36:07.382Z Reads: 235

```
![IMG_5133|474x313](upload://29aeFyobDmfmRViw4Nuebif4WmA.JPG)
```

---
## \#5 Posted by: professor_shartsis Posted at: 2018-05-12T12:38:38.471Z Reads: 208

```
[quote="accrobrandon, post:1, topic:55179, full:true"]
Let’s say I have a 6355 190kv and the other is same brand…same size and 170kv and u run that on a dual setup… How does this change board performance…

I assume since one has a lower kv thats less rpms and that the one motor tops out sooner than the other in the high end? And if this is correct then is there any major issues in the low end performance?
[/quote]

when the lower kv motor is above its no load speed, it will create drag for the other motor because it will be charging the battery (the back emf voltage produced is higher than pack voltage above no load speed). this has the potential to quickly overheat the attached vesc because, while the mosfets on a vesc are designed to cool ~50a motor current and ~3.7w continuously (P = I^2 * R = 50A * 50A * .0015ohm = 3.7W), the reverse current path is through the parasitic diodes in the mosfets which have a forward voltage drop of ~0.6v... you’ll hit ~3.7w at about ~6a of motor/battery reverse current, and after that the diodes will begin overheating. this will occur even without using the throttle on the lower kv motor. for reference, the mosfet drops about ~0.075V but the diode drops ~0.6V which means ~8 times less current through the diode generates the same heating on the vesc as ~50a motor current.

long story short, to protect your esc and for efficiency it isn’t recommended using 2 different kvs on your board.
```

---
## \#6 Posted by: telnoi Posted at: 2018-05-12T12:55:47.247Z Reads: 184

```
Or you limit the max erpm to the lowest KV motor. I guess that should be possible?
```

---
## \#7 Posted by: chocol4te Posted at: 2018-05-12T13:21:54.358Z Reads: 177

```
It really wouldn't be great. One of the main benefits of dual drives is even power on both sides to reduce turning when accelerating or braking and you would lose that. You also get the worst of both worlds by having one of each motor. The 190KV won't be able to reach it's top speed and the 170KV's torque will be imbalanced.
```

---
## \#8 Posted by: MoeStooge Posted at: 2018-05-12T13:34:48.545Z Reads: 165

```
Dual kv is a bad idea. Even if you gear so the motors run close to the same wheel speed you will never get the torque to balance between them.. You will get away with cruising, you may even find a sweet spot where torque will sync up and work at a certain speed.  When you need max torque one motor will be dominant. If your gearing is identical it will put the demand on the higher kv motor and smoke it. Your rigging for problems by splitting kv. Increasing Watts and proper gearing is the only way to get the best of both world's, Torque and Speed..🏁
```

---
## \#9 Posted by: accrobrandon Posted at: 2018-05-12T22:37:04.691Z Reads: 127

```
I ask cuz I have a sealed Maytech at 190 and having a hard time finding a second "sealed" online... Did see a recent post with someone who had the 170s for sale which is why I posed the question... Or I run one sealed and one not =\
```

---
## \#10 Posted by: Namasaki Posted at: 2018-05-13T02:21:48.326Z Reads: 112

```
I’m an doubtful that a 20kv difference would even be noticeable when riding.
Also, be aware that many motors have an actual kv that is different than their claimed KV. 
For example, I have 200kv and 190kv motors that are both actually 170-175 kv
```

---
## \#11 Posted by: b264 Posted at: 2018-05-13T02:32:11.787Z Reads: 108

```
[quote="Namasaki, post:10, topic:55179"]
I’m an doubtful that a 20kv difference would even be noticeable when riding.
[/quote]

When I change my Evolve from dual 150kv to split 140kv/150kv it is surprisingly noticable
```

---
## \#12 Posted by: onepunchboard Posted at: 2018-05-13T03:11:42.506Z Reads: 104

```
Im bit extreme im using 260 and 190 together with different each gearing. I use diagonal. real value when I measured was 280 and 200. 

That being said,  there is definitely torque steering when accelerating hard. but once I got used to it, wasn't a problem. I always use side walk which is very hard on board but so far I see no problem.

I hit 30mph with them and I didn't notice any difference in focbox or motor temperature. neither too hot on hot sunny day.
```

---
## \#13 Posted by: ATLesk8 Posted at: 2018-05-13T03:15:11.596Z Reads: 100

```
So I kinda asked this in a separate thread, but I'd like to use my carvon v2 single as the front drive motor on a dual diagonal, however I don't know how to figure out which rear drive train to use kv/gearing wise
```

---
## \#14 Posted by: onepunchboard Posted at: 2018-05-13T03:17:29.354Z Reads: 99

```
I used lower kv at back and high kv at front. because it accelerate better that way since ur body weight will press backwards.
```

---
## \#15 Posted by: accrobrandon Posted at: 2018-05-20T22:59:46.066Z Reads: 70

```
Re bump before I start another thread... Since i currently can't find a matching sealed can what should I do? But one that's unsealed but matching specs but visual symmetry will be off... Or buy another pair unsealed so they match??
```

---
