# VESC - FOC and nunchuck cruise - Oscillating forward / backward

### Replies: 5 Views: 518

## \#1 Posted by: mt37 Posted at: 2017-03-30T19:26:05.797Z Reads: 65

```
Hello! 

I've been playing with FOC with a sensored motor. It works well, except for the Cruise mode.

If I hit cruise the motor will oscillate forward and backward with gradually faster RPM. 

Has anyone experienced something similar ?
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-03-30T22:07:15.374Z Reads: 57

```
What are your speed controller settings in the Motor Advanced Tab? I mean the KP, KI and KD values?
You can try 
KP=0,00400
KI=0,00400
KD=0,00000
```

---
## \#3 Posted by: mt37 Posted at: 2017-03-30T22:08:58.600Z Reads: 51

```
I'll take a look tonight, I think they are default values (?)

What would be the recommended settings

Edit: Thanks for the recommendation!
I also found this thread that talk about these values [1]

[1] http://vedder.se/forums/viewtopic.php?f=6&t=74&p=586&hilit=cruise+control#p586
```

---
## \#4 Posted by: mt37 Posted at: 2017-03-31T04:15:47.900Z Reads: 39

```
@Ackmaniac Thank you that did it!
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-03-31T06:29:59.770Z Reads: 35

```
Now that you found a good base you can fine tune it. If you want that it adjusts to speed changes quicker you can raise KP and KI. If you want that it adjust slower then you can lower the values. And every time you change the motor max you have to adjust the KP and KI again.
```

---
