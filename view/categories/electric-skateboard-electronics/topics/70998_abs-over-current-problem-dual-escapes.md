# Abs-over-current problem (Dual Escapes)

### Replies: 13 Views: 193

## \#1 Posted by: Silverline Posted at: 2018-10-12T17:17:17.388Z Reads: 75

```
Hallo

I have this annoying problem with my Trampa MTB, i`m getting "ABS-over-current" failure, and the Escapes just brakes down the motors, wich is pretty scary and dangerous.

**Its always happen when i`m not going very fast, and NOT braking, so i`m not hitting any max values at all.**

I use two Escapes in dual mode via can-bus... and 2 x Sk8 149kv motors (had the same problem, when i was running flipsky motors)

Both the escapes showing the "ABS over current" in the terminal....

My Vesc settings is pretty normal, and not very agressiv at all
Motor max : 70A
Battery Max : 60 A
Motor Min : -40A
Battery min : -12A

Where to start ?

**I have used the wizzard for both setting up the vesc`s in dual mode, and for indput mode. It is working perfect, one thing i have noticed though, is my Slave vesc under "control mode" is set to OFF. Is this normal in a dual slave/master setup ? It does work and brake without problem. But i find it stange, that only my master vesc is set to "current no reverse with brake" ????**

![Screenshot_20181012-175308|281x500](upload://9dM8YM3FM94nQt2ibvQIUo56JGc.png) ![Screenshot_20181012-175415|281x500](upload://cCxoKgjVsDEAfYROZHqFgaMhuj0.png) ![Screenshot_20181012-175314|281x500](upload://sjZJuW2rqMaO9OjhgmI7o5zSMVO.png)
```

---
## \#2 Posted by: strattos Posted at: 2018-10-12T17:23:11.893Z Reads: 64

```
Check your cap legs and connections.
```

---
## \#3 Posted by: Silverline Posted at: 2018-10-12T17:27:11.924Z Reads: 66

```
Yeah i am familiar with that problem. I think they look okay. And i have glued the caps to the pcb, to take the stress. But i will have a second look again, thanks.....
```

---
## \#4 Posted by: strattos Posted at: 2018-10-12T17:29:11.683Z Reads: 64

```
Give em a wiggle I initially missed it as well.
```

---
## \#5 Posted by: Silverline Posted at: 2018-10-12T17:30:51.095Z Reads: 61

```
So you had the same problem ?
I just find it funny, it always happen when they are NOT under heavy load.
```

---
## \#6 Posted by: pjotr47 Posted at: 2018-10-12T17:38:30.945Z Reads: 57

```
On how much do you set your ABS over current setting?
```

---
## \#7 Posted by: Silverline Posted at: 2018-10-12T17:47:26.706Z Reads: 54

```
Huh..   where do you find that setting ? Default i guess....
```

---
## \#8 Posted by: pjotr47 Posted at: 2018-10-12T17:49:15.044Z Reads: 52

```
On the esc tool when you connect your vesc with the pc. Place your ABS over current on 130A and your problem will normally go away :slight_smile:
```

---
## \#9 Posted by: Silverline Posted at: 2018-10-12T18:27:43.964Z Reads: 45

```
Are you talking about "absolut max" setting ?
![IMG_20181012_202345|281x500](upload://a57bh9IEZU0enl0dO4ndAbTkWIk.jpeg)
```

---
## \#10 Posted by: Silverline Posted at: 2018-10-12T18:29:26.146Z Reads: 46

```
This is my control settings for my slave vesc
![IMG_20181012_202504|281x500](upload://rkL7Gh2iA5rQWGbo1Vz5fmPju1a.jpeg)
```

---
## \#11 Posted by: pjotr47 Posted at: 2018-10-12T18:40:30.663Z Reads: 41

```
Yes the 150A setting. But if it is so it looks good. If you Still have that check those capacitor are connected good. Do you have a long wire?
```

---
## \#12 Posted by: Andy87 Posted at: 2018-10-12T18:43:50.108Z Reads: 42

```
I had that issue once coming from the sensor wires... didn’t understood why but after I disconnected the sensors the faults where gone.
But my vesc didn’t cut out like your. Just got the fault message from time to time.
```

---
## \#13 Posted by: Silverline Posted at: 2018-10-12T18:45:29.608Z Reads: 41

```
No, i think the wires is pretty normal for a MTB, i even use 8awg wires. Looks like my caps is the best bet. I'v just find it strange, that it seems to be both of them.

Do my control settings for the slave vesc, looks normal to you ?
```

---
