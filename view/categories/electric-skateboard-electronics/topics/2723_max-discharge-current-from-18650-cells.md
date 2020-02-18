# Max discharge current from 18650 cells

### Replies: 10 Views: 36855

## \#1 Posted by: Ferret99 Posted at: 2016-04-29T20:18:09.681Z Reads: 312

```
Hello,

I am building my first electric longboard and I have alot of 18650 cells from old laptops.
All the cells are brand (samsung, panasonic, LG, sanyo).
My quation is what the maximum discharge current that I can use for 6s4p (all the batteries is 2000-3000mah and 2c rate)

Thank you,
Ofek
```

---
## \#2 Posted by: brywisco Posted at: 2016-04-29T20:28:00.261Z Reads: 309

```
2C = 2 x Capacity so 2 x 3000mAh => 6A discharge
the 4P then multiplies that by 4 so: 6A x 4p => 24A max that the pack could handle.
In my opinion- not enough for e-boarding...
```

---
## \#3 Posted by: harpie Posted at: 2016-04-29T20:28:08.794Z Reads: 306

```
If every cell had a discharge rate of 2c that would mean that at a capacity of 2500mAh each cell could handle 5000mA through them. With 5A through a cell and 4 cells in parallel the max discharge rate of the battery would be rated at 20A. I would think that these cells have a higher discharge rate than 2c, more like 10c maybe...
```

---
## \#4 Posted by: Ferret99 Posted at: 2016-04-29T20:35:13.127Z Reads: 291

```
OK thank you very much!! I am probably going to use lipo batteries
```

---
## \#5 Posted by: delta_19 Posted at: 2016-04-29T21:33:18.340Z Reads: 266

```
it depends on the cell you have

an lg hb2 has a max discharge of 30A but only a 1500Mah capacity but, the samsung 25R has a max discharge of 20A and a 2500mAh capacity. 

second using pulled batteries is a bad idea, very low discharge and not always the best stock.
```

---
## \#6 Posted by: onloop Posted at: 2016-04-30T01:09:15.794Z Reads: 242

```
I think 18650 cells for eboards should be rated at 8C if you plan to have 3P or less. (LG he2 or Samsung 25R)

If you have 4P or more you might be able to get away with lower C rating.

More cells in Parallel allow each cell to have a lower discharge rating... but I still think 2C is probably a bit low.

A good idea is to build a battery that can output more power than you will ever use. example. 80A max output, but set current limit to 40A. This will result in a happy long life battery.
```

---
## \#7 Posted by: Okami Posted at: 2016-07-11T22:00:07.826Z Reads: 198

```
Not to make a new topic -

Can people who have built 18650 packs, share their max theoretical discharge?
```

---
## \#8 Posted by: fruitgrower Posted at: 2017-06-21T17:40:08.114Z Reads: 134

```
Just my humble opinion here.

We learned in our electronics classes that the current in a series circuit is the same through every component in that circuit.  Not only that, the maximum current in a series of cells would only be as great as the cell-current that is available from the weakest cell in the chain of series components.  Consequently, if a particular cell in a series string is able to deliver 20 to 25  amps and another cell is only able to yield 15 amps maximum then the actual output current from the string will only be 15 amps.

My advice would be to use a parallel arrangement with fewer cells and then build a series-parallel circuit.   E.g.  A series-parallel arrangement of 72 cells to develop 24 volts output.

I welcome your comments. Please.tell me if I'm missing something.
```

---
## \#9 Posted by: smurf Posted at: 2017-06-21T17:59:23.615Z Reads: 118

```
No that would be bad advice. You want to use the least amount of wire to complete a circuit as it has to flow through all the batteries anyway. When you get to the lessons on inductive loads you'll understand why.
```

---
## \#10 Posted by: Maxid Posted at: 2017-06-21T18:18:22.991Z Reads: 115

```
[quote="fruitgrower, post:8, topic:2723, full:true"]
We learned in our electronics classes that the current in a series circuit is the same through every component in that circuit.
[/quote]
That is also not true when you have multiple power sources in your circuit.
In a battery pack a single cell can only have 15A while another outputs 20A.
Also think of this image:
http://www.electric-skateboard.builders/t/the-predator-trampa-street-carver-12s4p-dual-6374-kaly-motormounts-and-enclosure/24597/16?u=maxid

Edit: Ah I think I got your point now. We are talking about a mix of parallel and series connections in one large circuit. Sure If you only connect a couple batteries in series then the current will be limited by the weakest one in that series connection. But you want to have them in parallel so that they can balance each other. I think there was a discussion on endless-sphere about what the beast approach is in terms of connecting batteries in parallel or series first.
```

---
