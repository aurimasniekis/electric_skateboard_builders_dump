# Solder joint strength?

### Replies: 17 Views: 929

## \#1 Posted by: Zyb Posted at: 2018-03-27T21:56:33.934Z Reads: 153

```
Im in the process of building my pack for a segmented enclosure and thats going to be my first build. Going to connect serial packs with a silicone cable. Right now experimenting with solder joints and found out if you try to peel the nickel from the opposite direction joint is not really strong but if you pull from each end its virtually impossible to break with brute force. yes, i roughed up the nickel, used flux and tinned both ends before joining them.
a short demostration
https://www.youtube.com/watch?v=SG-PiQGfuW4&feature=youtu.be

another option i found is wrapping the nickel around the cable and soldering it that way, similar to soldering bullet connectors. it seems to be very strong when i pull from left or right side of it. 
am i being too obsessive about this i dont know :stuck_out_tongue_closed_eyes:  open to suggestions.

![image_123923953 (7)|595x500](upload://95n7JCgSwR6UxwHLOxTcshWP0G9.JPG)
![image_6483441|690x458](upload://yBiVpyfx1rmZxmq0AR19OmRgYu5.JPG)
```

---
## \#2 Posted by: b264 Posted at: 2018-03-27T22:01:53.845Z Reads: 137

```
The main cause of failure for a battery pack is chronic vibration and scuffing causing a short circuit.  I would put forth a hypothesis that because the metal cylinder has more sharp edges it might be worse, but that is 100% determined by how you use it and insulate it in a battery.
```

---
## \#3 Posted by: Zyb Posted at: 2018-03-27T22:12:00.921Z Reads: 125

```
im planning to heat shrink the battery pack but i will keep the cables outside of it because i dont want those cables to rub against any kind of metal and causing a short like you said. and may be wrap everything with a thin felt cloth or something.
```

---
## \#4 Posted by: deucesdown Posted at: 2018-03-28T04:29:39.722Z Reads: 98

```
Untested idea, but if worried about adhesion, maybe drill a small hole and solder like through hole pcb?
```

---
## \#5 Posted by: Acidfie Posted at: 2018-03-28T08:27:19.080Z Reads: 71

```
the main reason this is the weak spot is because of physics. this is because of shearing force. tr the same thing with tape or any adhesive like tape.

pulling wont do much since you're only attacking the bond on the whole area. if you're turning it around you just stress the bond on a little area. See:

![|666x500](upload://uHfElnCpd8uCWBpI2AYSimjGd3s.jpg)

i want to reference to my [thread](http://www.electric-skateboard.builders/t/battery-soldering-service-eu/48422/47)

you can for sure drill a hole, but this wont bring so much more adhesion. a good solder will always do its job. also, when soldering dont use nickel, use copper instead and then use Sn60Pb38Cu2 tin.

when using nickel, the copper is not really needed. also use flux cored solder. when soldering batterys, always use at minimum 75W and a very, very broad tip.
```

---
## \#6 Posted by: Zyb Posted at: 2018-03-28T08:38:34.405Z Reads: 65

```
that makes sense now. im spot welding the pack just going to use solder at the ends of nickel plates to connect packs.
```

---
## \#7 Posted by: Acidfie Posted at: 2018-03-28T08:57:38.214Z Reads: 68

```
this should be no problem, just make sure there is no physical force applied on the joints, like pulling.

also, be sure to use thick enough BMS wires when soldering, i am using always 0.5mm^2
```

---
## \#8 Posted by: Zyb Posted at: 2018-03-28T09:13:56.556Z Reads: 64

```
im using 22awg silicone for that. i actually asked supower about their balance cable thickness to match it because i had no idea what size to use and bought my cable accordingly. 
im having somewhat bigger issue tho, spot welding nickel to nickel is so weak and it breaks off easily. did not try different pulse settings but in case if i continue to have adhesion issue im thinking to pre solder those bridge pieces. i ll have to position them between batteries so they dont interfere with spot welding. 
![Untitled|646x458](upload://nTZCt7LpDEr0qomWsJ9WTKnrhni.jpg)
```

---
## \#9 Posted by: Acidfie Posted at: 2018-03-28T09:15:25.941Z Reads: 56

```
sadly, i do not know anything about spotwelding, i think there are more experienced guys here. 

i just know soldering work
```

---
## \#10 Posted by: Zyb Posted at: 2018-03-28T09:17:25.647Z Reads: 58

```
its ok man thanks for the help
```

---
## \#11 Posted by: Zyb Posted at: 2018-03-28T13:45:00.389Z Reads: 46

```
I tried the method I mentioned above and it turned out ok. Just like soldering bullet connectors filled the hole with solder![image|603x500](upload://xORTXBCuKDt9lf89pzD63fIcHmm.jpeg)![image|690x474](upload://hyvNscL3MU6eCx2sG7FQRsL6VJD.jpeg)
```

---
## \#12 Posted by: Acidfie Posted at: 2018-03-28T13:52:32.368Z Reads: 43

```
looking good, this should work. be aware that the weak point of a soldered joint is always short after the joint.
```

---
## \#13 Posted by: Zyb Posted at: 2018-03-28T13:59:12.779Z Reads: 41

```
You mean where solder flows in the cable after the actual joint?
```

---
## \#14 Posted by: Acidfie Posted at: 2018-03-28T14:26:57.310Z Reads: 40

```
between the pure cable and the soldered joint, this is the weakest spot, like from bending all the time.
```

---
## \#15 Posted by: Zyb Posted at: 2018-03-28T14:50:18.616Z Reads: 36

```
Oh ok then it’s destined to fail at some point 😁
```

---
## \#16 Posted by: Acidfie Posted at: 2018-03-28T15:49:40.233Z Reads: 30

```
i dont think you will take your battery out every time or am i wrong? 

also you dont start bending your cables for fun, or are you?

it will be good, just dont stress it too much
```

---
## \#17 Posted by: Zyb Posted at: 2018-03-28T15:55:07.673Z Reads: 28

```
i will use bms so i dont think i ll check them regularly when i heat shrink them they will be in the enclosure to stay :) yea it will be good i hope. i just seen terrible things these are not toys thats why i started to question most of the things when it comes to batteries and their connection but good insulation is the key i ll take necessary measures.
```

---
