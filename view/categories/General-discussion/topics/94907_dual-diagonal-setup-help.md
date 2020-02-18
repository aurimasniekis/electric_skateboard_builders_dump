# Dual Diagonal Setup Help

### Replies: 10 Views: 228

## \#1 Posted by: Mar-Key Posted at: 2019-05-25T04:23:07.802Z Reads: 89

```
I'm planning a dual diagonal build with a custom battery. If anyone has built a DD board, which wires did you extend? 

The way I see it there are two options:

1. Use 2 VESC's, one at the front, one at the back. Split and extend the battery wires to power each. Extend a CAN bus cable to connect them together.

2. Use either a dual VESC or 2 at the back. Extend the motor and sensor wires for the further motor.

Please let me know what works best, or if there are other ways to go about it!
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-05-25T05:22:57.928Z Reads: 78

```
I think the best option is to use the battery wires full length as well as the vesc, and make a small extender where needed. The less the better.
```

---
## \#3 Posted by: Mar-Key Posted at: 2019-05-25T05:25:17.571Z Reads: 76

```
Can you explain that a little more?
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-05-25T05:26:31.388Z Reads: 73

```
1 vesc at the front, 1 at the back. Extend battery wires as little as possible.
```

---
## \#5 Posted by: Mar-Key Posted at: 2019-05-25T05:28:19.596Z Reads: 71

```
Okay so more akin to option 1
```

---
## \#6 Posted by: Dirt_Bag Posted at: 2019-05-25T05:30:49.890Z Reads: 71

```
Yes. You will get emf interferance with long battery wires. It might be worth it to install several capacitors right before the vesc on the battery leads. A quick search will show other people doing it and what you need to know. I think the said if the wires are over a 16in, it might be time for some caps
```

---
## \#7 Posted by: Mar-Key Posted at: 2019-05-25T05:40:57.031Z Reads: 68

```
I'll look into it, but my wires would definitely be longer than 16". Out of curiosity, what makes this way better than a dual VESC with extended motor and sensor wires?
```

---
## \#8 Posted by: Dirt_Bag Posted at: 2019-05-25T05:45:58.278Z Reads: 69

```
Extended phase wires have the same issue. For all the extra length, it will affect the smoothness of the motor. You cant add caps to phase wires, but you can to the battery
```

---
## \#9 Posted by: dareno Posted at: 2019-05-25T09:14:47.386Z Reads: 56

```
Don't complicate things that don't need complicating.  You running end to end motors then run end to end vescs.   Simple.   Battery wiring will be fine in the space of a normal longboard.
```

---
## \#10 Posted by: skelstar Posted at: 2019-05-25T18:02:27.022Z Reads: 39

```
Good question though.

I have VESCs at each end and run the battery wires to each... although my board isn't very long (~34").
```

---
