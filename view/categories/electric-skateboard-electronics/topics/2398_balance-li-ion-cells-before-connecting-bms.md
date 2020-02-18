# Balance Li-ion Cells Before Connecting BMS?

### Replies: 12 Views: 1533

## \#1 Posted by: paragon Posted at: 2016-04-16T16:49:32.835Z Reads: 111

```
@chaka  
@torqueboards
Does anyone know if it's beneficial to balance your cells before building the pack and connecting the BMS? Or will the bms take care of that during the first charge?
```

---
## \#2 Posted by: Blasto Posted at: 2016-04-16T17:37:31.331Z Reads: 106

```
[quote="paragon, post:1, topic:2398"]
Also, for a 10s 4p pack, would it be better to use 4 bms (each connected to 10s1p) so that each cell is individually monitored?
[/quote]

Can't do that, the cells are already in parallel, you would be taking the same measurement 4 times.
```

---
## \#3 Posted by: paragon Posted at: 2016-04-16T19:09:33.445Z Reads: 102

```
Wow, good point, brain fart.
```

---
## \#4 Posted by: chaka Posted at: 2016-04-16T20:13:11.660Z Reads: 100

```
Just make sure they are all about the same in voltage before making the parallel connections.
```

---
## \#5 Posted by: lowGuido Posted at: 2016-04-17T00:19:24.871Z Reads: 95

```
It wont hurt to balance them first. I probably would.
that way you know they are all around about the same voltage when you start. saves you from measuring each individual cell.
```

---
## \#6 Posted by: Namasaki Posted at: 2016-04-17T06:46:43.345Z Reads: 89

```
Doesn't the BMS balance all the cells the first time you charge it up?
Doesn't the BMS balance every cell every time you charge the pack?
Doesn't it also discharge all cells equally?
I thought that was the whole point of the BMS.
```

---
## \#7 Posted by: lowGuido Posted at: 2016-04-17T07:48:02.358Z Reads: 81

```
if you are assembling a battery you would probably be connecting the parallel cells and spot welding them in place well before you have hooked up the BMS. un balanced cells being connected together in parallel will equalize themselves rapidly, causing large current and possibly cell damage. its best to bring all the cells to the same potential before connecting them.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-06-21T23:45:46.676Z Reads: 67

```
do you recommend charging each cell full or storage charge before building the pack.
```

---
## \#9 Posted by: paragon Posted at: 2016-06-24T02:42:34.811Z Reads: 59

```
I don't think it matters too much if all the cells are balanced.
I'd prefer storage voltage before building a pack because it may be slightly safer.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-06-24T02:53:51.638Z Reads: 56

```
According to lowguido, it does matter when building parallel packs.
```

---
## \#11 Posted by: lox897 Posted at: 2016-06-24T05:55:47.400Z Reads: 47

```
I think storage voltage would be better too. As long as they are all the same voltage of course.
```

---
## \#12 Posted by: Nordle Posted at: 2016-06-24T06:05:21.496Z Reads: 47

```
And what needs to be connected first? Power wires or balance wires? Always forget this.
```

---
