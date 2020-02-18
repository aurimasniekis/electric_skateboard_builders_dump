# Just finished setting up vesc tool, wheels are spinning in opposite directions?

### Replies: 14 Views: 354

## \#1 Posted by: Taliesin Posted at: 2018-08-24T03:08:59.030Z Reads: 74

```
Wtf? I thought I was at last finished and then boom, wheels spinning in opposite directions.

Help? Why?
```

---
## \#2 Posted by: ArgentumHeart Posted at: 2018-08-24T03:11:36.532Z Reads: 74

```
Turn off the board, swap 2 phase wires on the motor spinning in the wrong direction.
```

---
## \#3 Posted by: Taliesin Posted at: 2018-08-24T03:14:17.000Z Reads: 71

```
There’s 3 wires; a, b, and c. Which 2?
```

---
## \#4 Posted by: Scoo_B_SK8 Posted at: 2018-08-24T03:18:26.512Z Reads: 68

```
any 2 

10char
```

---
## \#5 Posted by: ArgentumHeart Posted at: 2018-08-24T03:21:20.311Z Reads: 64

```
any 2 of them
```

---
## \#6 Posted by: goldrabe Posted at: 2018-08-24T03:25:50.886Z Reads: 63

```
After swapping two of the wires didn´t you need to do a motor detection again if running FOC?

@ArgentumHeart
```

---
## \#7 Posted by: Taliesin Posted at: 2018-08-24T03:27:00.353Z Reads: 61

```
Yup wheels not spinning, guess I’ll run vesc tool again
```

---
## \#8 Posted by: ArgentumHeart Posted at: 2018-08-24T03:30:38.183Z Reads: 59

```
[quote="Taliesin, post:7, topic:65908, full:true"]
Yup wheels not spinning, guess I’ll run vesc tool again
[/quote]
sensored? I guess yes. 

[quote="goldrabe, post:6, topic:65908"]
After swapping two of the wires didn´t you need to do a motor detection again if running FOC?
[/quote]

Thats weird
```

---
## \#9 Posted by: goldrabe Posted at: 2018-08-24T03:37:16.832Z Reads: 58

```
Yes i rcalled it correctly, if running BLDC you just can swap wires around in Foc you need to recalibrate.

https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/283
```

---
## \#10 Posted by: treenutter Posted at: 2018-08-24T03:46:31.700Z Reads: 56

```
Yes- run motor detection again after swapping the wires. Be sure to secure the tightly w tape or heat shrink.  You don’t want them disconnecting during a ride!
```

---
## \#11 Posted by: Taliesin Posted at: 2018-08-24T04:03:23.524Z Reads: 46

```
I swapped, ran motor detection, and still spinning wrong direction.... ?
```

---
## \#12 Posted by: Taliesin Posted at: 2018-08-24T04:06:31.321Z Reads: 44

```
Ugh...

So it’s spinning the right direction during the motor setup test phase, but as soon as I finish with the remote ppm input setup wizard it spins the wrong direction..



Any ideas?
```

---
## \#13 Posted by: Taliesin Posted at: 2018-08-24T04:13:43.080Z Reads: 44

```
EDIT: found it. GREAT SUCCESS!!!!

Ok I found “invert motor direction” under the general tab in motor settings but I don’t see an “apply” button anywhere.

Anyone know where the “write motor configuration” button would be?
```

---
## \#14 Posted by: goldrabe Posted at: 2018-08-24T04:25:15.862Z Reads: 41

```
On the right hand side of the vesc tool it´s the M with arrow down.
Just hover over it and the symbol will say what it does.
```

---
