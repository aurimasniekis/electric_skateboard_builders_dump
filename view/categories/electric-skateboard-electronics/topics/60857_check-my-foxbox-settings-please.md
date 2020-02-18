# Check my foxbox settings please!

### Replies: 10 Views: 284

## \#1 Posted by: rexpepper651 Posted at: 2018-07-04T05:11:25.053Z Reads: 88

```
so after flashing my focboxes and starting over from a weird issue  another has reared its frustrating head. ive lost range. i was getting 17-20 miles on a single charge now im getting 12-14 miles. can you check over my settings please? im still pretty new to all this only have had my board complete for about 2 months almost

Battery - 12s5p
dual 6374 

![4|690x351](upload://w91T2Aw06hrjaqPA9pNlreZJHmF.PNG)![2|690x357](upload://3bDhQDwCkqxIDcjR83YxYfQFpxp.PNG)![11|690x354](upload://sQUBNFiG3SYT9jQyehEGEFdDoVR.PNG)![3|690x355](upload://nRx9NQa8cMwpwcKW46SE6FAC5U6.PNG)
```

---
## \#2 Posted by: rexpepper651 Posted at: 2018-07-07T00:42:23.780Z Reads: 51

```
I just checked my battery at full charge and I'm only getting a reading of 50.4 volts. Shouldn't I be closer to 57v at full charge?
```

---
## \#3 Posted by: BoostedBuilder Posted at: 2018-07-07T00:58:45.742Z Reads: 49

```
Please explain your logic behind 57V!?
```

---
## \#4 Posted by: rexpepper651 Posted at: 2018-07-07T01:05:06.914Z Reads: 48

```
I am not sure actually now that I think about it lol. What should my pack read? I'm not sure what it should be at this point.
```

---
## \#5 Posted by: Benjamin899 Posted at: 2018-07-07T01:12:04.158Z Reads: 46

```
looks ok, maybe shitty batteries.
```

---
## \#6 Posted by: rexpepper651 Posted at: 2018-07-07T01:25:35.513Z Reads: 46

```
How can I check if they are crap? They're Samsung 30q. I bought the pack from psychotiller 2 months ago.
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-07-07T01:30:56.837Z Reads: 46

```
no his packs are good, same route same conditions?
```

---
## \#8 Posted by: rexpepper651 Posted at: 2018-07-07T03:03:33.288Z Reads: 42

```
Diff routes. I'll have to see going the same route. It was pretty windy the last time I was out. Am I getting worse range from hettingbused to the speed possibly? I know these maybe dumb questions but I'm still really new to all this and thank you for healing i really appreciate it alot.
```

---
## \#9 Posted by: E1Allen Posted at: 2018-07-07T06:54:18.296Z Reads: 38

```
Motor Config, motor tab. Uncheck limit erpm with negative torque.

Battery min -10 each vesc

Max battery voltage 50.4 with 12s so you're good there.
That's 4.2v x 12s. So not 57v

Battery cutoff start 38.4
Battery cutoff end 36 (recommendations)

You have your battery cutoff end at the absolute minimum for that battery, according to myself and others that's not healthy for battery's.  Sacrifice some range for battery longevity. 

That aside, 12-14mi is garbage range for that pack.  
What are your riding conditions and wheel size type and gearing?

I recommend some sort of Bluetooth module to better track your information.  I have metr pro, it's great.
```

---
## \#10 Posted by: rexpepper651 Posted at: 2018-07-07T13:33:44.999Z Reads: 33

```
I will get those settings changed today after work. im running the evolve 7in AT wheels, 15t motor pulley and 62t i believe for the wheel. we have some hills where i ride but nothing too steep or real long. im not a real heavy guy im about 170lbs with gear on. i mostly ride in the street and on bike paths not much off road riding.
```

---
