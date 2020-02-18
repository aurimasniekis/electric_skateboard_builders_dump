# An idea for a simple and cheap battery balancer. could this work?

### Replies: 18 Views: 1722

## \#1 Posted by: Hillso Posted at: 2016-11-10T15:51:39.518Z Reads: 146

```
each cell is connected to a capacitor. one cell at a time. using transistors and some kind of an ic, or even a microprocessor. the device is connected to the balance wires only.

second 1: cell 1 connected to the capacitor
second 2: cell 2 connected to the capacitor
second 3: cell 3 connected to the capacitor
second 4: cell 1 connected to the capacitor
second 5: cell 2 connected to the capacitor
second 6: cell 3 connected to the capacitor
second 7: cell 1 connected to the capacitor


This is roughly the idea, not a real diagram:
<img src="/uploads/db1493/original/3X/b/f/bfbe8ad7e28daf6c8076c1052dd4909e98f3f814.png" width="571" height="345">

I'm not very good at explaining things in English.
what do you think?
```

---
## \#2 Posted by: Hummie Posted at: 2016-11-10T16:02:19.499Z Reads: 139

```
Can u explain how the circuit works in detail for idiots?
```

---
## \#3 Posted by: evoheyax Posted at: 2016-11-10T16:03:53.834Z Reads: 138

```
I'm not sure if this will work but what I will add to this topic is that you can always manually balance them... This is how I have been riding for the last few months. I manually balance once every few weeks by measuring all the voltages of the cells, and using a regulated power supply, tuned to 4.2 volts, to charge up cell by cell until they are all within .01 of each other.
```

---
## \#4 Posted by: jmasta Posted at: 2016-11-10T16:41:53.507Z Reads: 122

```
One question... why?

I'm not trying to discourage innovation.  I just don't see how the added time, complexity, and risk justifies saving a few dollars to reinvent the wheel.  I sure don't trust my electrical skills enough to design something like this, but maybe you do! Good luck!
```

---
## \#5 Posted by: Hummie Posted at: 2016-11-10T16:49:42.161Z Reads: 113

```
https://hobbyking.com/en_us/turnigy-dlux-lipo-battery-cell-display-and-balancer-2s-6s.html

this is what I use.  two of them.  very simple and cheap.  but I'd like to know how what you show would work
```

---
## \#6 Posted by: chinzw Posted at: 2016-11-10T17:50:07.910Z Reads: 95

```
A capacitor? I don't see this working. Are you trying to charge the capacitor to discharge one of the cells? I don't think that would work.
This wont be simple, or cheap. You will need differential op-amps to measure the cell voltages, you will need an arduino/attiny or some other form of controller.
A BMS costs 20-50$ depending on number of cells and amp rating, an arduino/attiny alone costs that, add the opamps, resistors, pcb, connectors, mosfets and you'll be throwing your money away.
Unless you want to do this to learn, you should should stick to tried and tested bms from the usual brands.
```

---
## \#7 Posted by: Hillso Posted at: 2016-11-10T17:58:00.022Z Reads: 86

```
the Idea is to cycle between the cells one at a time, no need for measuring the cells.
the idea of balancing cells with a capacitor is not new, it's called charge shuttle (or something like that. you can google balance cells with capacitors).


@Hummie
The idea is to simulate a parallel connection between the cells, but without really connecting the cells in parallel (because then there will be a short).

@jmasta
This is not an invention of mine, what is new here is that I think this method doesn't require to measure the cells at all, it is stupid balancing.  

@chinzw
I already have a BMS, I'm thinking about it for fun :slight_smile:  
and it doesn't require measuring the cells.

I think this have some advantages, for example, it will not balance the cells at the end of charge, so you can charge the battery less than 100% for example (I'm not sure, but I think BMS balance the cells at end of charge). It should be plug and play. no protection of any kind though.
and it should be pretty cheap.
```

---
## \#8 Posted by: Hummie Posted at: 2016-11-10T18:04:00.641Z Reads: 71

```
i was looking into breaking the series connections and making them all parallel to balance but the voltage difference between cells would create a huge transfer of power quickly and not be good for cells.  would this do that but slow the transfer of power?  I imagine simply some resistors between the cells in parallel would work 

this similar:
http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.842.9011&rep=rep1&type=pdf
```

---
## \#9 Posted by: Hillso Posted at: 2016-11-10T18:14:40.363Z Reads: 67

```
I ask the same question, I hoped people here could know if this idea is good. I'm really a beginner in electronics.
I think the current can be limited, with resistors?
it might not be a problem if the balancing is happening all the time passively because there would be very small differences between the cells.
the url doesn't work for me:
 "We are sorry !
The URL does not match any resource in our repository."
```

---
## \#10 Posted by: Hummie Posted at: 2016-11-10T18:16:30.228Z Reads: 70

```
that would be good!  if you could balance autonomously all the time.  so you'd have a short as they'd be in series for the main power leads and  parallel connections constantly with huge resistors between the parallel connections to constantly balance.  sounds good to me but I dont know much either.  sounds so simple and minimalist I really like the idea.  too good to be true i fear but I'm open to more complexity if it does the job autonomously and i can keep whatever would do it constantly on the job of balancing.

hum the link works for me.  i havent read it yet but looks readable and a similar intention.
```

---
## \#11 Posted by: chinzw Posted at: 2016-11-10T18:24:28.306Z Reads: 59

```
That whitepaper even has a PCB layout.
```

---
## \#12 Posted by: Hummie Posted at: 2016-11-10T18:29:45.089Z Reads: 54

```
@chinzw
how about doing as we're both saying and have the main leads all in series permanently and also parallel connections permanently but with the parallel with large resistors between to limit the current to something super small?
```

---
## \#13 Posted by: chinzw Posted at: 2016-11-10T18:31:58.011Z Reads: 51

```
Im not sure what you mean, care to draw a quick sketch of what you have in mind?
```

---
## \#14 Posted by: Hummie Posted at: 2016-11-10T18:34:10.943Z Reads: 52

```
cant draw on here.  dont know how.  just imagine 12s all in series.  and then each cell also put in parallel with all the others but with large resistors between all the parallel connections.  maybe the resistors would have to all be a different stronger resistance as they moved further along..as the voltage would increase throughout the series chain.
```

---
## \#15 Posted by: chinzw Posted at: 2016-11-10T18:36:24.488Z Reads: 55

```
But why would you want to do that?
```

---
## \#16 Posted by: Hillso Posted at: 2016-11-10T18:46:32.259Z Reads: 56

```
@Hummie that would short the cells, every cell positive will be connected to it's negative. my idea would not short the cells, because the positive is not connected to the negative, but the positive of one cell would virtually be connected to the positive and the negative would be connected to the negative of another cell.
I think your suggestion is:
<img src="/uploads/db1493/original/3X/8/1/819ad87aa761ba8249df175800a9ed3d9dd800f2.png" width="182" height="101">

this is a normal battery:
<img src="/uploads/db1493/original/3X/7/d/7d5f1582f103aa4adab46de8babe1d08ace06144.png" width="200" height="102">
```

---
## \#17 Posted by: Multi Posted at: 2017-10-03T20:14:05.551Z Reads: 31

```
Possible blut expensive and complicated.

Active balancing

Active cell balancing methods remove charge from one or more high cells and deliver the charge to one or more low cells. Since it is impractical to provide independent charging for all the individual cells simultaneously, the balancing charge must be applied sequentially. Taking into account the charging times for each cell, the equalisation process is also very time consuming with charging times measured in hours. Some active cell balancing schemes are designed to halt the charging of the fully charged cells and continue charging the weaker cells till they reach full charge thus maximising the battery's charge capacity.

    Charge Shuttle (Flying Capacitor) Charge Distribution

    With this method a capacitor is switched sequentially across each cell in the series chain. The capacitor averages the charge level on the cells by picking up charge from the cells with higher than average voltage and dumping the charge into cells with lower than average voltage. Alternatively the process can be speeded up by programming the capacitor to repeatedly transfer charge from the highest voltage cell to the lowest voltage cell. Efficiency is reduced as the cell voltage differences are reduced. The method is fairly complex with expensive electronics.
```

---
## \#18 Posted by: Martinsp Posted at: 2017-10-03T20:17:53.800Z Reads: 29

```
There are balancers like this, you can find them on HobbyKing for under 10 bucks... But you have to realize that the balancing current is very very very low... say 10mA Which for a regular battery, say 10 000 is not even worth trying... And also you are adding one more thing to the system that is connected directly to the battery which can fail at any time and short cells together and blow your whole battery up... Id say that there are cheaper ways to destroy a battery than this :D :D
```

---
