# Ownboard esc help

### Replies: 8 Views: 185

## \#1 Posted by: Bobby Posted at: 2018-11-03T20:06:22.966Z Reads: 51

```
So i have an ownboard esc and my power button got lost from the enclosure through vibrations. Seems like there are three wires.... i have another power button but it has four wires... can this work somehow or do i need to find a three pin power button
```

---
## \#2 Posted by: pat.speed Posted at: 2018-11-03T20:43:27.339Z Reads: 42

```
Can work, the esc has 3 wires correct? One should be gnd, one vcc(pos) and one the switch point. I can’t guarantee but my guess would be that the ground and positive go to the + & -  of the switch so that it lights up. Now the 3rd wire for the switching on part goes to either of the left over pins, and the last pin that’s still there should go to either ground or positive. 

If you can read the switch or check the polarity of the wires that would be great so you know which wire to connect, the pos or neg. someone like @Kug3lis or another ee can probs tell you if it’s pos or neg. my guess is pos but I’m not 100% sure and wouldn’t like to be responsible for cooking someone else’s stuff  


The way it works is when you switch it on the positive (just example could also be ground) goes to the esc and basically tells it the switch is being pressed and to turn on. The 4 pin switch’s are exactly the same just you have one wire going there twice pretty much.
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-11-03T21:08:50.464Z Reads: 36

```
It's probably switch input, ground and LED+
```

---
## \#4 Posted by: pat.speed Posted at: 2018-11-03T21:11:43.433Z Reads: 32

```
Yeah that’s what I thought but is the switch input going to be the gnd or pos?
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-11-03T21:12:42.998Z Reads: 30

```
it can be ground too ;) Our button shorts to ground and LED is plus
```

---
## \#6 Posted by: pat.speed Posted at: 2018-11-03T21:16:19.224Z Reads: 28

```
Ahh so it can be either pos or neg that gets sent to esc switch output pin. If he was to connect the wrong one would it fry?
```

---
## \#7 Posted by: Kug3lis Posted at: 2018-11-03T21:18:22.251Z Reads: 24

```
Don't know :) depends on circuit :)
```

---
## \#8 Posted by: pat.speed Posted at: 2018-11-03T21:19:41.740Z Reads: 23

```
Lol, hehe now he has to play Russian roulette
```

---
