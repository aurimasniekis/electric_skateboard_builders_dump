# Help, my motor gets hot very quick

### Replies: 15 Views: 319

## \#1 Posted by: Devilmycry Posted at: 2018-10-08T21:56:26.308Z Reads: 111

```
Hi 
My motor get heat really quickly like if I ride like around 35mph 40 for like 10min my motor go to 86c easy I can still touch them but is very hot and the board slow down I have the temperature cutoff start at 90c but when I it 85 86 I have no speed no torque 

And if I ride more easily the motor still go to 80c
Belt are not to tie correct in place the screw for the motor don’t touche anything 
My set up is 12s7p motor sk3 192 sensored 
Gear 62t 15t wheel 7inch 
Motor 60 -60A 
Battery 50A -15 
Erpm 100000 
W 15000 
Vec6
I have another board almost the them except the sk3 are not sensored the wheel are 8inch the gear are 66 15 and the motor don’t get to worm
I’m going to look at it tomorrow 
Any advice 
Thank you
```

---
## \#2 Posted by: professor_shartsis Posted at: 2018-10-08T22:00:18.158Z Reads: 104

```
if you want exactly the same performance but less heat, get motors with the same kv but lower electrical resistance (generally larger physical size)

if you’re willing to sacrifice acceleration for less heat try lowering your battery limit from 50a -> 40a and/or motor limit to 60a -> 50a (or lessen the current limits by some other amount.)

another way to get less heat for the same acceleration is increase your gear reduction ratio, but this will lessen your top speed proportionately.
```

---
## \#3 Posted by: Devilmycry Posted at: 2018-10-08T22:03:30.328Z Reads: 101

```
Yes it what I was thinking go down to 50 for the motor I hope I don’t lose to much torque 
But do you think I have some problem or is just the way it is the motor get hot
```

---
## \#4 Posted by: professor_shartsis Posted at: 2018-10-08T22:06:16.721Z Reads: 96

```
one last way to get the same thrust/acceleration with less heat is use smaller wheel diameter, but again this will lower your top speed like changing the gear ratio.
```

---
## \#5 Posted by: Devilmycry Posted at: 2018-10-08T22:09:53.076Z Reads: 87

```
Yes is the problem bc I have 8inch and go down to 7inch love the torque but don’t like the top speed I was thinking go to 16t motor but bc my motor heat I think is a bad idea
```

---
## \#6 Posted by: Devilmycry Posted at: 2018-10-08T22:16:48.485Z Reads: 79

```
But the think I want to know is if I have a problem or is just the way is it 
Bc lot of people I know use 62t 16t
And the set up is 60 -60 
Battery 30 I know is almost half as my -10 
And 60000erpm and is look like they do heat to much 
And my second board also have the same set up at th one heat up and I have not problem 
I was thinking I have some problem
```

---
## \#7 Posted by: professor_shartsis Posted at: 2018-10-08T22:28:34.374Z Reads: 72

```
here is some related info from another thread (relating to changing the battery current limit)

[quote="professor_shartsis, post:1, topic:70464"]
I wondered how different battery current limit settings affect hill climbing ability-- so I did a comparison of 30a vs 60a battery current limits per motor (both 100a motor current limit) with (2) 73kv hub motors at 46v with 84mm tires…
[/quote]

https://image.ibb.co/e1RAdp/climbing_30a_vs_60a_battery.gif

take a look at the green line, bottom middle chart (ohmic heating watts).. this is for changing only the 60a battery limit to 30a battery limit.

notice the effect the change has on your thrust in pounds (red line, bottom left chart -- vehicle thrust in pounds, 2 motors) -- in this scenario the rider can still reach the same top speed on a 10% slope (yellow line, bottom left chart), but the acceleration is less with 30a battery vs 60a battery.

[quote="Devilmycry, post:6, topic:70603"]
And my second board also have the same set up at th one heat up and I have not problem
I was thinking I have some problem
[/quote]

that's more of an indication of a problem, but i'm not sure exactly what's causing the problem....
```

---
## \#8 Posted by: Devilmycry Posted at: 2018-10-08T22:56:53.276Z Reads: 60

```
Ok thank you 
But is look like the problem is more how I set it up my vesc to a mechanical problem I can fix and stay with the same set up
```

---
## \#9 Posted by: Devilmycry Posted at: 2018-10-08T23:01:53.010Z Reads: 62

```
What problem do you think it will be give me some exemple 
Thank you
```

---
## \#10 Posted by: professor_shartsis Posted at: 2018-10-08T23:36:26.600Z Reads: 56

```
if one motor was getting much hotter than the other on the same board i’d suspect maybe a short in the motor windings...

 but if both motors on the same board are getting equally warm, and you have another board with the same setup and those motors stay cooler, i’d suspect the motors on the board that’s getting warmer have higher electrical resistance due to the way they’re constructed... such as would be the case if the windings were a thinner gauge wire but with the same # of turns to keep the kv the same. less copper in the motor makes things get warmer for the same performance.
```

---
## \#11 Posted by: Devilmycry Posted at: 2018-10-08T23:49:46.543Z Reads: 51

```
Ok thank you so much
The only thing I can do is go down for my battery or my motor 
😭😭😭 or charge motor and go hight kv
```

---
## \#12 Posted by: professor_shartsis Posted at: 2018-10-08T23:59:48.607Z Reads: 48

```
[quote="Devilmycry, post:11, topic:70603"]
or charge motor and go hight kv
[/quote]

you wouldn't need higher kv... you'd want the same kv for same performance... but lower electrical resistance (generally larger physical size motor same kv with more copper) for less heat but the same torque.
```

---
## \#13 Posted by: rich Posted at: 2018-10-09T04:56:37.640Z Reads: 41

```
[quote="Devilmycry, post:1, topic:70603"]
And if I ride more easily the motor still go to 80c
[/quote]

Do you mean it still gets hot when riding slow/normal from start without hills or racing?

I would say it's a short in the windings or cables inside the motor like @professor_shartsis mentioned.
I don't think it's your gearing or settings. 

Remove the belt and spin the motor by hand, do you feel any resistance?

I had the same happening with 2 motors. They reached 80 °C within 4 minutes easy cruising.  I realized there is some resistance when spinning, but not comparable to the resistance when holding 2 phase wires together. 

When I moved the phase wires the resistance was sometimes gone. So there was some kind of short inside the motors. Got them replaced.

Your motor is not sealed so it should never get hot. I can ride 2-3 hours non stop (Urban Carver, dual 6355) and the motors are not even warm.

But on the MTB with sealed motors it's different.
```

---
## \#14 Posted by: Devilmycry Posted at: 2018-10-09T05:02:59.025Z Reads: 36

```
When I ride relax and carving everything look ok 
And I test to spin the motor is look like is normal
```

---
## \#15 Posted by: rich Posted at: 2018-10-09T05:08:31.330Z Reads: 35

```
Ok so no short :grin:

35-40 mph is damn fast :crazy_face:, ride slower or decrease max motor amps
```

---
