# General question BMS balance charging

### Replies: 13 Views: 1858

## \#1 Posted by: thisguyhere Posted at: 2016-11-10T18:16:22.990Z Reads: 164

```
I had a general question on how a BMS balance charges individual cells.

Given a 10s battery pack, a 10s BMS would have 10 balancing wires.

So the installation would entail connecting the first position balance wire on the first cell, then the second wire to the second cell, etc, all the way down to the end of the pack.

Once connected, how does the BMS know which cell to balance?  Would it not see the entire pack as a single circuit?

I may have a fundamental lack of understanding in electronic circuits in general here so I apologize in advance if this question is making you angry... :grimacing:
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-10T18:30:15.730Z Reads: 157

```
The BMS gets connections to every single cell in your pack, and through resistors is bleeds current to ground. There's a "channel" for each cell.
```

---
## \#3 Posted by: JuniorPotato93 Posted at: 2016-11-10T18:31:15.615Z Reads: 155

```
[quote="thisguyhere, post:1, topic:12825"]
So the installation would entail connecting the first position balance wire on the first cell, then the second wire to the second cell, etc, all the way down to the end of the pack.
[/quote]

These ten wires in a 10S set up, or N wires in a NS, create N secondary circuits. The BMS will pump voltage through the entire pack and these N connections simply drain out some voltage from cells that are higher than the rest until you get a balanced pack.
```

---
## \#4 Posted by: thisguyhere Posted at: 2016-11-11T00:39:49.910Z Reads: 137

```
[quote="JuniorPotato93, post:3, topic:12825"]
These ten wires in a 10S set up, or N wires in a NS, create N secondary circuits. The BMS will pump voltage through the entire pack and these N connections simply drain out some voltage from cells that are higher than the rest until you get a balanced pack.
[/quote]

https://cdn.meme.am/instances/250x250/63733466.jpg

so in this below diagram, wouldn't lead wire 10 see the same voltage as lead wire 1?

<img src="/uploads/db1493/original/3X/8/9/89e045efaca6eb40bce91ac79a4b08c1cad2c8b0.jpg" width="457" height="343">

i guess i'm just confused as how the lead wire targets a specific cell since it's all on the same circuit.
```

---
## \#5 Posted by: chinzw Posted at: 2016-11-11T00:44:19.522Z Reads: 126

```
Wish i was home so i could show you a pic of how i wired my new arduino battery monitor.

Basically, if you test - and 10 you get 36v, but if you test - and 1 you get 3.7v, now if you test 1 and 2 you get 3.7v as well, and the same goes for each pair of adjacent pins.

EDIT:
As an example application, if you connect an opto-isolator (led and light sensor) between pins 1 and 2 and another between pins 2 and 3, both opto-isolators will output 3.7v
```

---
## \#6 Posted by: JuniorPotato93 Posted at: 2016-11-11T01:28:00.234Z Reads: 117

```
No,  this is not the case because each cell increases the voltage from cell to cell. The diagram you show has some of the voltages shown on it.  Each subsequent cell increased the potential by 3.7V nominal value as you add cells,  that is why the 10th cell is(should be 37)  labeled at 36V.   The rest of the circuit after the tenth cell and terminal P is the same potential.  This is why you need to get a BMS specific to the number of cells you are using.  It knows the expected potential at each cell.
```

---
## \#7 Posted by: chinzw Posted at: 2016-11-11T01:44:10.330Z Reads: 112

```
[quote="JuniorPotato93, post:6, topic:12825"]
This is why you need to get a BMS specific to the number of cells you are using.  It knows the expected potential at each cell.
[/quote]

And also why if you reverse or mess the wiring order you will fry the bms.
```

---
## \#8 Posted by: jmasta Posted at: 2016-11-11T01:51:11.043Z Reads: 112

```
[quote="thisguyhere, post:4, topic:12825, full:true"]

so in this below diagram, wouldn't lead wire 10 see the same voltage as lead wire 1?

<img src="/uploads/db1493/original/3X/8/9/89e045efaca6eb40bce91ac79a4b08c1cad2c8b0.jpg" width="457" height="343">

i guess i'm just confused as how the lead wire targets a specific cell since it's all on the same circuit.
[/quote]

No, the voltage difference between wire #10 and #1 in that diagram would be: 36 - 3.7 = ~ 32.3 V

With respect to B-, the voltage at #10 would be 36V
```

---
## \#9 Posted by: thisguyhere Posted at: 2016-11-11T16:28:46.914Z Reads: 95

```
ok, this is coming together for me.

thanks guys.

like i said before, my misunderstanding just stems from my general lack of knowledge in electronics.  doing research though, gettin' better.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-11-11T16:49:52.925Z Reads: 88

```
[quote="thisguyhere, post:4, topic:12825"]
i guess i'm just confused as how the lead wire targets a specific cell since it's all on the same circuit.
[/quote]
Yes, all cells are one the same circuit 
However, because DC current flows only in one direction, the BMS with its balance leads connected to the positive side of each cell or parallel cell group adds up the voltage in sequence and monitors for correct voltage at each sequential cell or cell group isolating from the cells down stream. 
i.e.

Cell1 4.2
Cell2 8.4
Cell3 12.6
And so on.
```

---
## \#11 Posted by: thisguyhere Posted at: 2016-11-11T17:44:30.753Z Reads: 82

```
[quote="Namasaki, post:10, topic:12825"]
Yes, all cells are one the same circuit However, because DC current flows only in one direction, the BMS with its balance leads connected to the positive side of each cell or parallel cell group adds up the voltage in sequence and monitors for correct voltage at each sequential cell or cell group isolating from the cells down stream. i.e.
[/quote]

ok, this solidifies it for me.  the current can be measured at different points in the circuit.  makes total sense.
```

---
## \#12 Posted by: jmasta Posted at: 2016-11-11T21:33:23.273Z Reads: 79

```
[quote="thisguyhere, post:11, topic:12825, full:true"]
[quote="Namasaki, post:10, topic:12825"]
Yes, all cells are one the same circuit However, because DC current flows only in one direction, the BMS with its balance leads connected to the positive side of each cell or parallel cell group adds up the voltage in sequence and monitors for correct voltage at each sequential cell or cell group isolating from the cells down stream. i.e.
[/quote]

ok, this solidifies it for me.  the current can be measured at different points in the circuit.  makes total sense.
[/quote]

The current along a closed loop is the same (look up Kirchoff's laws for more info).  To measure currently directly, your ammeter must be wired inline with your circuit (series).  

Voltage is measured in parallel (your voltmeter and source have same voltage, but different current).  This is why you can measure the voltage potential of each cells simply touching the leads of your voltmeter to the (+) and (-) battery terminals
```

---
## \#13 Posted by: Namasaki Posted at: 2016-11-11T22:00:28.058Z Reads: 72

```
His comment was miss-worded. We were talking about the BMS monitoring the voltage of each cell or cell group not the current.
```

---
