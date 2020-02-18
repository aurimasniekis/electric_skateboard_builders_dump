# Dual motor setup

### Replies: 9 Views: 1563

## \#1 Posted by: willpark16 Posted at: 2016-02-13T23:06:43.736Z Reads: 147

```
How do you calculate the speed of a dual motor setup?
```

---
## \#2 Posted by: delta_19 Posted at: 2016-02-13T23:22:11.803Z Reads: 147

```
pretty sure top speed is all the same you just have more torque to get you there and up hills.

speed calculator here: http://toddy616.blogspot.ca/2013/07/electric-skateboard-calculator.html?m=1
```

---
## \#3 Posted by: willpark16 Posted at: 2016-02-13T23:43:41.021Z Reads: 141

```
thanks!!!!!!!! hahaha
```

---
## \#4 Posted by: Namasaki Posted at: 2016-02-14T17:10:55.523Z Reads: 124

```
bench speed= Rpm x wheel circumference 
Real speed = bench speed - load factor
Dual motor cuts load factor in half
How to figure load factor? 
Good question!
```

---
## \#5 Posted by: lowGuido Posted at: 2016-02-14T17:23:00.492Z Reads: 115

```
good question indeed.

I have always found that even though theoretically the top speed should be the same, the dual motors will have a slightly higher top speed than single just because they are able to push that load just a little bit better than the single.
```

---
## \#6 Posted by: laurnts Posted at: 2016-02-14T20:52:37.246Z Reads: 106

```
Dyno test could provide load factor! Theoritically there should not be load factor at all in my pov. Thats because the motor should just draw more current to maintain the speed (something like motor timing / govenor mode value could effect this). Load factor it's self also a non-static value, it also depends on the rpm / effective motor load.

My suspicion lies in motor timing and esc processing speed. Because weight could shift the timing of esc to determine which winding to be energized (also involved by the frequency rate of the esc). So instead of giving the "right constant energy to the motor", the esc kept on giving correction value to the motor, as a result the motor always run slower than the respond. That slowness also gets affected by BEMF as sensorless depends on back emf value, so esc always provide "late" value to the motor.

I suppose load factor could be diminished by knowing how much load / constant avg load and inpu them into esc. So the esc will always supply more power instead of waiting to know if it requires more power to operate the motor. I believe if we make our brushless motor 10x bigger, there won't be so much load factor as the motor won't even notice the load we put.

Anyway this is just my speculation, maybe someone else with engineering background could explain this better / more accurate! :D (Sometimes the topic in this forum made me wonder if I studied the correct subject, I should have gone engineering!)
```

---
## \#7 Posted by: Risten135 Posted at: 2016-08-20T03:53:01.855Z Reads: 69

```
Does anyone have a diagram of how to wire a dual motor setup? If so, hmu cause I'm really liking forward to it 👍😁
```

---
## \#8 Posted by: lox897 Posted at: 2016-08-20T08:50:38.122Z Reads: 59

```
Check out the beautiful diagrams thread. You might find what you want there.
```

---
## \#9 Posted by: Risten135 Posted at: 2016-08-20T12:54:45.487Z Reads: 56

```
Thank you very much! 👍🏻
```

---
