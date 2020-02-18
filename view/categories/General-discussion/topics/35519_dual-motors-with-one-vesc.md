# Dual Motors&hellip; With one VESC?

### Replies: 18 Views: 2715

## \#1 Posted by: GrecoMan Posted at: 2017-10-14T18:10:03.295Z Reads: 226

```
I'm just wondering why someone hasn't tried something of the sort, for science.  I was thinking of soldering 2 phase wire leads to each of the vesc terminals, in the end, giving you six phase wires with one vesc.  I feel like erpm is probably the stopping block but I don't know how.  Probably wont try this since I don't have any extra parts but...

Does someone else see a reason why this cant be done?  Am I missing something?
```

---
## \#2 Posted by: wafflejock Posted at: 2017-10-14T18:12:17.303Z Reads: 222

```
The back emf and integrator limit values you get (during motor detection) are per motor I'm pretty sure and vary a bit so I think it would have problems with the rate of firing also you're pushing all the power for two motors through one speed controller (more amps to deal with).
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-10-14T18:13:40.669Z Reads: 221

```
seems like if you were running conservative settings on the vesc those things wouldn't matter very much.  The slight difference in kV shouldn't really be a problem
```

---
## \#4 Posted by: wafflejock Posted at: 2017-10-14T18:15:42.452Z Reads: 218

```
Yeah not sure if either of those would be show stoppers just saying things I could see as potential issues, would be interested to hear if someone has tried it as well.
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-10-14T18:17:50.613Z Reads: 201

```
yea I bet there are definetly some things that would slow down progress just cant think of anything of the top of my head.  Sounds like something @lowGuido would try...
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-10-14T18:21:59.388Z Reads: 187

```
Im not sure if vesc can do but, boat rc esc can push 2 motor with no apperent problem. u probably need to get something goes over 150a with gooood heatsink
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-10-14T18:22:45.159Z Reads: 178

```
maybe a beefy vesc like focbox with heatsink or @chaka vesc could handle it
```

---
## \#8 Posted by: Martinsp Posted at: 2017-10-14T18:24:22.641Z Reads: 167

```
I tried this and it does work on bench with no load on the motors but as soon as you slow one motor it does not work. Also when I put it on a board it worked with just the board going back and forth but as soon as I stepped on it and tried it it was just jerking like crazy and would not work, even with a little push before accelerating. I was running sensor-less of course because joining the sensor wires and slowing one motor down definitely would not work.
```

---
## \#9 Posted by: darkkevind Posted at: 2017-10-14T18:25:37.376Z Reads: 160

```
If you know anything about electronics and how these AC three phase motors work, you'll know that it's impossible to power two motors off of one ESC because the ESC is an inverter that sends signals to the motor to power the relevant poles depending on where the can is compared to the stator.
In this process the ESC gets signals from the motor telling it where it is in the state of rotation, in order for the ESC to send the correct signals to the correct set of windings...

If you were to put two motors on one inverter, it will either blow up or one motor would spin fine and the other would judder, or that would happen randomly and in turn. So one motor ok for a second then the other judders, then the other one's ok and now the other one' juddering etc etc.

In short, it will either blow your ESC or f*ck stuff up. :thumbsup:
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-10-14T18:26:05.246Z Reads: 135

```
hmm then super beefy 150a+ esc would be needed.  I guarantee it was because both motor were demanding 50a+ but vesc was limiting to like 20a each
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-10-14T18:26:59.801Z Reads: 132

```
lol makes sense.  Knew I was missing something...
```

---
## \#12 Posted by: darkkevind Posted at: 2017-10-14T18:27:15.172Z Reads: 129

```
Yes, as soon as you've got something that stops the no-load rotation, and basically isn't free wheeling, it will come out of sync.
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-10-14T18:27:46.320Z Reads: 122

```
Unless you were able to link both the motors together somehow...
*thinking face emoji*
```

---
## \#14 Posted by: darkkevind Posted at: 2017-10-14T18:29:20.640Z Reads: 119

```
If both motors were running ONE axle it would work if their poles were lined up exactly...
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-10-14T18:30:25.812Z Reads: 110

```
didn't mean with one axle. More like 2 independent axles and then idk maybe sheet metal or something connecting them and forcing them to spin as one
```

---
## \#16 Posted by: darkkevind Posted at: 2017-10-14T18:31:16.002Z Reads: 99

```
But then you might as well just have one axle no?
```

---
## \#17 Posted by: GrecoMan Posted at: 2017-10-14T18:31:47.077Z Reads: 99

```
true.  But then were back to the problem of turning :sweat:
```

---
## \#18 Posted by: onepunchboard Posted at: 2017-10-14T18:32:47.952Z Reads: 97

```
https://youtu.be/O0iMQ9rQNuo
for the science!
```

---
