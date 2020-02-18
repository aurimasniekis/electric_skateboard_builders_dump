# Help Charging - Keep getting sparks - 6S2P Lipos Parallel Charging Board

### Replies: 8 Views: 242

## \#1 Posted by: HillRipper21 Posted at: 2018-09-08T16:01:28.384Z Reads: 56

```
Hey guys, I have a problem with my charging setup which I don't understand. I have 4 3s Zippys running 6S2P and am trying to charge them using a parallel charging board and an iMax B6 as so:

![Battery%20Wiring%20Diagram|666x500](upload://l083Cd8zQ7iVHPH8MssFUNXzhq8.jpg)
![Balance%20Wire%20Diagram|666x500](upload://paeddigRXJXC9YJlkq1BpvS7w6c.jpg)

Both of the main power leads plug in fine to the board, I plugged in one balance cable but whenever I try to plug in the second balance cable it sparks a lot and burns up. I don't understand why this is happening, the voltages seem correct on the balance pins, I can measure across and it goes 3.7, 7.4, 11.1, 14.8, 18.5, 22.2. The other balance cable is setup exactly the same and works. I don't think the parallel board is faulty because I've got it to work in the past and I tried multiple ports on it with the same result. I check the continuity on all the pins and they seemed okay too. Here's the parallel board (without the balance cables plugged in) 
 ![parallel_board|374x499](upload://hLy2yJZgWf63j1gJE0jvIFQotQL.jpg)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-08T16:12:01.465Z Reads: 43

```
Did you check that you plug in the balance wires in the right order on the parallel board?
Maybe you mixed there + and -?
```

---
## \#3 Posted by: L3chef Posted at: 2018-09-08T16:13:11.328Z Reads: 42

```
Don't you have your ground balance wire comming from you positive terminal?
Nvm  I'm wrong here...
```

---
## \#4 Posted by: HillRipper21 Posted at: 2018-09-08T16:13:36.294Z Reads: 42

```
There's only 1 way to plug in the plastic piece because it has those 2 little legs on it. I plugged it in the exact same way as the first one.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-09-08T16:17:42.558Z Reads: 43

```
So if you charge only one 6s all is good, with 2 6s it spark right?
Why one balance plug burned on the board? 
Did you check there is no short now?
```

---
## \#6 Posted by: akhlut Posted at: 2018-09-08T16:18:23.221Z Reads: 41

```
my guess:

your cells are out of balance, probably a low cell.

never, ever parallel charge without checking that the cells are within 0.1V of one another.

/edit
grab a dmm and check each cell
```

---
## \#7 Posted by: HillRipper21 Posted at: 2018-09-08T16:21:17.869Z Reads: 36

```
Thats where it burned previously so I'm not using that port anymore. And ya I checked the continuity from each pin on the balance ports to the output pins on the balance port... not sure what else to check

Edit: Ya charging just 1 worked, but I have actually been able to successfully charge both at the same time before using this board in the past.
```

---
## \#8 Posted by: HillRipper21 Posted at: 2018-09-08T16:22:04.407Z Reads: 37

```
I will double check again, but they were all very close together, I checked them individually and they are all 3.8 or 3.81
```

---
