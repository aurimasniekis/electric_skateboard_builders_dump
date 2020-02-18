# 13s? 14s? On the vesc

### Replies: 23 Views: 3499

## \#1 Posted by: Hummie Posted at: 2016-05-27T22:38:55.463Z Reads: 261

```
FFrom Vedder's site:
have discovered that a good trade-off is at around 60V (quite safe for 10s or 12s lipos), where the efficiency is good and the voltage is not too problematic to handle.

 on his chat site I read that there are voltage spikes when braking so you can start with 10s or 12s but bump it up when braking.  I got the impression this is battery related and is similar to voltage sag and maybe with a big pack it would keep the voltsge more stable and 13 or 14s would be possible?
Anyone tried it?  The one guy on Vedder's site blew a chip doing 14s. 13s  would give just that smidgen more max speed I'd like while keeping the low kv for torque.

There's a guy over there on vedders chat site that says using his method he can get it up to 15s.  He hasnt done it but says u just have to add capacitors I think. He's looking for people to try it
```

---
## \#2 Posted by: KMeyerson Posted at: 2016-05-28T01:50:28.773Z Reads: 235

```
Electrically speaking, the more sensitive components on the VESC are manufacturer rated with maximum voltages at 60V. Exceeding this for more than a moment under certain conditions will cause components to fail.

The causes of voltage spikes at 10s and 12s are known as you described and can be protected against with a bit of electrical modification - a challenge if you do not have your own PCB mill/flow oven/solder skills.

In F1 Hybrid Racing, the goal has always been to keep the voltage as high as possible and current as low as possible.  Wire weight gets cut, battery discharge/recharge benefits, and of course cause the car has to break some kind of speed limit on the track and in the lab. 

If boosted pushes 5-12 miles from their 12s1p (2.5 Ah) battery and claims they've doubled that range with their double capacity battery (12s1p, 5Ah), then clearly the rest of us should do the next most practical thing is to go 14s, 5Ah at home.  

But wait! Theres more! As a biomedical engineering student, I am informing you that 50V is enough to start creeping through your skin and that a current as low as 10 miliamps can disrupt your heart rhythm.  So be careful, always insulate, and watch your operating temps.
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-05-28T04:33:12.128Z Reads: 207

```
Gees I'm up grading to 50v ... I guess I need to be extra careful
```

---
## \#4 Posted by: KMeyerson Posted at: 2016-05-28T04:45:38.545Z Reads: 199

```
Eh?  It's still a matter of resistance and path length.  Running a current between your fingers might go to your heart, but there's a lot of other things that are in between that can absorb or burn.
```

---
## \#5 Posted by: Hummie Posted at: 2016-05-28T05:00:08.945Z Reads: 196

```
U can get zapped through the skin with as low as 30 volts or less...maybe you had a sweaty day.  Ac will go through you more easily at lower voltages.  Encouragingly most people who get hit by lightning survive.  You're better getting blasted hard which will clench your heart as apposed to something less that will put your heart into arrythmia.  Just need a fraction of an amp going through the heart specifically to lay you out permanently.  

But how bout 14s?!  Anyone know what mods need to be done? I'm overwhelmed by vedder's site and need micro spoon feeding or a good link to how these things work
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-05-28T05:07:00.647Z Reads: 184

```
Lol you freaked me out with the heart disruption lol

Better safe than sorry!
```

---
## \#7 Posted by: KMeyerson Posted at: 2016-05-28T05:23:40.139Z Reads: 180

```
Remember what happened in Edison's public lab tests?

He shocked animals with low doses of DC current (low voltage can't travel far, but current caused pain in targeted areas) to prove it was "safe".  His demo of AC instantly kfilled the anims because voltage travels a great distance and can kill even at a marginal, minimal low current.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-05-28T05:26:27.480Z Reads: 179

```
Well i guess I won't be making that a/c powered board
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-05-28T05:28:23.494Z Reads: 178

```
What's the advantage of moving up past 12s...aside from crazy top speed?
```

---
## \#10 Posted by: Hummie Posted at: 2016-05-28T06:35:17.393Z Reads: 170

```
Edison showed to be sadistic and got a bad rep

Benefits of 12s?  Gives a broader spectrum as you can keep a low kv for torque and have speed
```

---
## \#11 Posted by: KMeyerson Posted at: 2016-05-28T16:24:10.118Z Reads: 152

```
WHat hummie says translates to the ability to have super thin wires (low voltage × high current = thick wires vs high voltage × low current = thin wires)  In a motor, this means you can get more inductive force from more turns of wire rather than a fewer, thicker coils that gave a higher electrical resistance.
```

---
## \#12 Posted by: Hummie Posted at: 2016-05-28T16:45:23.089Z Reads: 146

```
Being nitpicky you get more electrical resistance with the thin wires but more inductance per amp. 

 U could run one volt with a really high kv motor and get practically the same performance in speed and torque and heat generated as with 50 volts and a super low kv motor.  Lots of amps through the windings necessary with the high kv but the windings would be thicker and shorter and have less resistance and ultimately it all ends up equal in terms of torque and heat and speed.  Why no one does one volt??? The other wires would need to be bigger and it could be rough on the esc but I don't think necessarily and depends on the esc
The battery draw would be the same in watt hours with either system
The benefit of high voltage is thinner battery wires so lighter.  In practice, for me, it means keeping the low speed torque and having speed. But really there's no magic and with the higher voltage I will be trading battery space that could be amps so going up steep hills I'll still suck as many amps with the low kv but the battery won't have as many because it's in series and now volts
So the real benefit..now that I put it down in writing...I'm not sure and I'd likely be better off with a higher kv motor and the same voltage if I want to go faster. The differences in efficiency are minimal.  The differences in performance can be adjusted through changing the kv.  The big difference..u can blast more amps through and blow up the motor with the higher voltage due to ohms law where the higher the voltage overcomes resistance easier so more amps. And if you don't blow it up it runs great
```

---
## \#13 Posted by: KMeyerson Posted at: 2016-05-28T16:58:33.134Z Reads: 131

```
True, but if you use many parallel strands the losses are marginal. We use a YASA AC motor on our car - the main loss is having to cool with an electrolytic solution.  

Thumbs up.
```

---
## \#14 Posted by: Hummie Posted at: 2016-05-28T17:01:53.321Z Reads: 132

```
Parallel motor windings?  Only time I hear of them being used is to make winding easier on the hands and manufacturers don't have to get different wire awg for different motors and also with really high frequency switching/commutation due to skin effect but our motors don't do near those speeds of commutation. 
Why do u use the parallel strands?
```

---
## \#15 Posted by: Hummie Posted at: 2016-05-28T17:07:26.888Z Reads: 128

```
Parallel strands in a motor other than to avoid skin effect...I can't think of a good reason other than to allow the coolant to flow through and take the heat away better. Otherwise parallel strands take from the max possible copper fill.  If the coolant were pumped through single strand as apposed to parallel strands it might be better at taking the heat (which would be less) as the copper conducts to its surface so well.  I'm curious.  I'm sure they know what they're doing when they make that motor
```

---
## \#16 Posted by: KMeyerson Posted at: 2016-05-28T17:10:24.911Z Reads: 127

```
Yep, we're not operating at that frequency. Again, we entered the hypothetical with a "one volt" world.

If our motors were operating at that frequency, a lot of things would change for us.

I've used parallel for moving the field. As you mentioned, thinner wires have more inductive power but do get toastier. I experimented for a while with thicker inner strands an thinner outer strands. Why? Because I predicted that the path of least resistance would be closer to the center and because the thinner wires would cool more effectively on the outside. In practice, the design worked, but did require water cooling approaching 75% duty cycle.
```

---
## \#17 Posted by: KMeyerson Posted at: 2016-05-28T17:11:54.242Z Reads: 124

```
Hummie, I can't hit a moving text target when I write responses.

Yasa sponsored us, I did not have the opportunity to open its motor.  I do not think they use parallel strands, but I hope to experiment more with it in the future.
```

---
## \#18 Posted by: Michaelinvegas Posted at: 2016-05-28T18:55:23.989Z Reads: 122

```
Good info guys...thanks for taking the time👍🏻
```

---
## \#19 Posted by: KMeyerson Posted at: 2016-05-28T19:06:45.465Z Reads: 122

```
Np, just manually rewound a Yuneec Motor.  Ditched the bad sensor board.
```

---
## \#20 Posted by: Michaelinvegas Posted at: 2016-05-28T19:17:36.731Z Reads: 122

```
Ok....wait so is there a magic voltage per se where things get more "perfect" or rather more "optimal" for running motors??

Is there such a thing?
```

---
## \#21 Posted by: KMeyerson Posted at: 2016-05-28T19:33:44.880Z Reads: 117

```
Ideal volt/current depends on the motor design (Stator length, diameter, material [thickness if frequencies are used], magnets, air gap, wire diameter/resistance, etc.

Its hard to line everything up for a "perfect" or "magic" setup.
```

---
## \#22 Posted by: Hummie Posted at: 2016-05-28T22:12:09.506Z Reads: 113

```
Depending what you read.

It's said motors are most efficient running at a very high percent of their no-load rpm.  ((The no-load speed is the max speed they spin with no resistance)).   This no-load is adjustable with either more or less voltage and more or less turns of wire around the tooth.  This is the most important reason to adjust voltage.   Other than this purpose where you are designing the system to run within the optimal rpm range using greater voltage enables you to simply have thinner battery wires.  But..another important variable is the esc and what voltage and amperage it runs most efficiently at and I believe, but don't know for sure, escs like to pass as few amps as possible.    So...ultimately...the higher the voltage the more efficient system as long as the motors use puts you at ...let's say 75% of the no-load speed

And that's what they say but...who here rides around at one speed!  If you really want to find what voltage you would be most efficient at you could ride your normal route AT THE SPEED YOU DESIRE, see how many amps were spent, try it again with more or less voltage, and see how many amps you spend.  Doing that you'll find the real variable is how fast you want to go. 
   you can go up a steep hill using a high kv mixed with high voltage but it will suck a huge amount of amps.   in practice, likely because of ohm's law, the greater the voltage the easier it is to push the current, and you will get up that steep hill much faster with a low kv and also save your amps.  I've ridden 80,90,100kv up the same hill, all with almost the same other variables, and the 80s go up faster.  

every other aspect of the motor...size,magnets, length, whatever, can be accounted for looking at the Kv and you can forget about them As long as the motor is big enough for the job though.  In fact having too small a motor for the job is the number one reason to sink into inefficiency.  There are other more powerful motor designs for their size  out there other  than the radial "outrunner" motor.  Axial flux "pancake" motors and the new confusing transverse flux motor. 
Haven't read this and am surprises..it looks readable:
http://www.mht.bme.hu/~bilicz/compumag2013/files/pa3-11.pdf
```

---
## \#23 Posted by: KMeyerson Posted at: 2016-05-31T06:28:13.863Z Reads: 96

```
YASA was axial.

All good stuff, Hummie. Thumbs up.
```

---
