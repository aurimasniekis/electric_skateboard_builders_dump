# 3 state power switch

### Replies: 3 Views: 69

## \#1 Posted by: Yarden Posted at: 2020-02-09T23:31:27.059Z Reads: 32

```
So, unrelated to my previous post, here's my idea for an alternative (hopefully cheaper) anti spark power switch..

So the problem is that the VESC's capacitors at t=0 are empty which means zero resistance, and when just plugging in the power, the current goes to infinity..

So those ugly anti-spark key loop XT90 solutions, have a 5ohm resistor inside so when half pluging it, you close loop with 5ohm resistor in series which leads to normal current flow (around 5A), and few moments later, when fully connecting the plug, you switch to non resistor circuit but at this time, the capacitors are pretty full so the current is stable (it takes few milisecond to pass the risky park of super high current).

Its a briliant idea, but the performance is ugly to my opinion.. having a "key" to power on your board by plugging a XT90... 

So I thought about this idea:
![image|666x500](upload://bT0ymiu78IPsLZPRjRmTJgbmkWP.jpeg) 

having a 3 state power switch, which can be mounted to the case and having, a neat, (perhaps water proof if you seal it all), enclosing.

which, when you want to turn on the board you simply rotate from state 1 (off) to state 3 (on).
but since you go through state 2, which has a resistor, you get a few moments of closed loop with resistor in series, which leads to a partial charging of the capacitors with a limited current flow (and fuse for protection).

It will feel similar to ignition a car but without the last part. you just cross two sections on the turn..

I think this solution is more elegant than the key loop one.

The question is now, are there any high current 3 state cheap switches for this fix.

the wires on 2 doesn't need to be that thich, since the current flow there is limited.
the switch also doesn't need to support high current on all switch states, just on one of them.

what do you guys think?
did I miss something in my theory?
are there some cheap switches which can fit this?
```

---
## \#2 Posted by: Yarden Posted at: 2020-02-09T23:37:13.941Z Reads: 25

```
this can also be performed using two normal switches, but thats less user friendly (you will need to push one button to insert a resistor in series, then flip the master switch, then release the push button to remove the resistor in series and leave the circuit zero resistancy closed, it is also a bit more tricky to wire up)

![image|666x500](upload://cDk84ABruXfOOiRdDC3SBBzvo8F.jpeg) 

it takes two high current switches, one state keep, and the other push button..
need to be more careful here not to rotate the power without holding the push button..

Also I'm not sure if it saves bucks that way..
```

---
## \#3 Posted by: PixelatedPolyeurthan Posted at: 2020-02-10T07:36:25.651Z Reads: 17

```
try posting this here.

forum. esk8 .news

It is the new forum. this one is dead due to a long sad story
```

---
