# Is pushing w/ a motor bad?

### Replies: 6 Views: 1112

## \#1 Posted by: JT_Clemente Posted at: 2016-04-03T20:27:41.654Z Reads: 109

```
I remember reading about this on the forum somewhere, but I can't seem to find any info again.
Is pushing on a brushless motor bad for it? If I were to spin the motor manually (pushing, riding downhill, etc.) would it ruin it in any way? A friend of mine was under the impression it isn't good and could mess the motor up.
```

---
## \#2 Posted by: JLabs Posted at: 2016-04-03T20:31:00.561Z Reads: 109

```
It can blow the esc because it is charging the board (creating electricity) when u push.. but I wouldn't worry about it, it should be fine in my experience
```

---
## \#3 Posted by: JLabs Posted at: 2016-04-03T20:31:55.080Z Reads: 110

```
Its basically the same as going down a hill
```

---
## \#4 Posted by: thisrealhuman Posted at: 2016-04-03T21:01:30.630Z Reads: 106

```
It's not the motor you need to worry about, if you are using a BEC or step down converter you could overload the caps. I've burned two 50v BECs because my loop key fell out while going approx 15mph. If there is a path for the power to flow, the motor will still spin. If you try to push with the ESC disconnected from the battery and there is nowhere for the power to flow then the power will build up in the motor (or loop back into it?) and cause it to halt. I try to keep my downhill speed around 80% of my flat ground top speed and I never brake for more than 5 seconds. I don't know how much damage can be done by going faster. I've noticed that if my battery dies (3.3v cutoff) and i push (while everything is still powered on) for about a block i can keep riding for another block or so, BUT my cells were off balance afterward (+0.05v difference in less than a mile of pushing) so I don't do that anymore.
```

---
## \#5 Posted by: Hummie Posted at: 2016-04-04T04:18:03.441Z Reads: 85

```
The vesc lights up when u push the board unpowered. I assumed it was fine to do.  Are u saying it's not safe on the vesc or just at high speeds?
```

---
## \#6 Posted by: thisrealhuman Posted at: 2016-04-05T20:03:43.663Z Reads: 59

```
I've never used a VESC, so I don't know. Maybe connect a watt meter and see if any power is leaving the vesc toward the batteries while pushing? If the vesc has a way to utilize the generated power without overcharging cells or locking the motor then it has another selling point that I haven't seen mentioned. Someone needs to make the financial sacrifice and test the max amperage the vesc can handle while pushing powered off. I would certainly like to know that there's a safety cutoff of some type.
```

---
