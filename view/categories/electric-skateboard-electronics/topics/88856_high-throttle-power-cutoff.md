# High Throttle Power Cutoff

### Replies: 13 Views: 279

## \#1 Posted by: VECTOR.xyz Posted at: 2019-03-31T04:26:46.227Z Reads: 107

```
I am using a VESC 4.12 from torque boards and a SK3 6374 192kv with 10s (10s4p 30q w/ 60a BMS). My max motor current is 80a and my max battery current is 40a, and I am using the GT2B remote with PWM and no sensors. Braking current is 15a.

When I push the throttle all the way to full when I'm not already going at a high speed, the board starts accelerating for about half a second, but then the power from the motor completely cuts, and I have to return back to 0 throttle before I can accelerate again (luckily I can still brake). Seems like if I'm asking for the board to accelerate at a high rate with a high amperage, the motor cuts off completely.

This has not been very problematic for me, but it has been somewhat dangerous, especially when I'm at higher speeds because I'm leaning forward and the sudden cutoff throws me forward. It's not a huge issue, but I do really want to get it fixed.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-31T04:35:18.852Z Reads: 103

```
Do you use the vesc Tool or the bldc Tool to programm your settings? 
In bldc you could select, limit erpm with negativ torque, which means as soon as you reach your max erpm your esc break down.
If you use vesc tool that shouldn’t be the case.
```

---
## \#3 Posted by: Eboosted Posted at: 2019-03-31T04:37:47.637Z Reads: 97

```
Does it happens only when your battery is 100% charged?
```

---
## \#4 Posted by: mmaner Posted at: 2019-03-31T05:01:19.222Z Reads: 95

```
Drop it to 50 motor amps and see if you still have the problem, if not bump it to 70a and so on until you find where the limit is.
```

---
## \#5 Posted by: VECTOR.xyz Posted at: 2019-03-31T17:14:54.094Z Reads: 67

```
I'm using the vesc tool. Is the bldc tool better?
```

---
## \#6 Posted by: VECTOR.xyz Posted at: 2019-03-31T17:15:57.253Z Reads: 65

```
I'll try it out.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-03-31T17:24:15.804Z Reads: 61

```
No, the bldc tool is the old version of the vesc tool
```

---
## \#8 Posted by: Z4MSupreme Posted at: 2019-04-12T11:49:43.602Z Reads: 39

```
were you able to sort out this issue? im having the exact same problem. thanks
```

---
## \#9 Posted by: Andy87 Posted at: 2019-04-12T12:00:29.952Z Reads: 38

```
did you try the suggestions in the thread?
```

---
## \#10 Posted by: Z4MSupreme Posted at: 2019-04-12T12:01:31.676Z Reads: 36

```
im a bit worried about increasing the current. was curious to see how you sorted it out...
```

---
## \#11 Posted by: Andy87 Posted at: 2019-04-12T12:03:40.378Z Reads: 36

```
let´s move to your thread... just have seen.
```

---
## \#12 Posted by: VECTOR.xyz Posted at: 2019-04-13T03:44:49.340Z Reads: 28

```
@Z4MSupreme @Andy87 Yeah I lowered the motor amps to 50A and increased battery amps to 50A. Seems to have fixed it, but my acceleration is a little slower.
```

---
## \#13 Posted by: Z4MSupreme Posted at: 2019-04-13T08:11:43.730Z Reads: 24

```
Will give that a try. Thanks 👍
```

---
