# 8s 4p battery help

### Replies: 4 Views: 854

## \#1 Posted by: david11 Posted at: 2017-06-10T22:02:16.723Z Reads: 88

```
Hi guys im new to building e scateboards and i find the battery stuff very confusing. i have 32 18650 cells that im trying to turn into a 8s 4p battery. the cells must be flat and not layered as i want the scateboard to be thin. i know theres another thread on this but i dont understand the diagram that was made. will this work if i use a bms.

The grey lines represent the nickle plates. 
<img src="/uploads/db1493/original/3X/0/a/0a1644ca08b2f75fd85030f958097e056f8ef836.png" width="690" height="388">
```

---
## \#2 Posted by: oyta Posted at: 2017-06-10T22:23:30.035Z Reads: 82

```
<img src="/uploads/db1493/original/3X/6/4/645bbd4888f5c430d9c5111c449144993f6b1532.png" width="623" height="500">
This is an example of how you can connect your batteries in a 8s4p configuration. At the top you see the concepts.

And yes - there are 8s BMSes out there. The balance wires will connect between each parallell pack.
```

---
## \#3 Posted by: david11 Posted at: 2017-06-12T11:52:17.181Z Reads: 52

```
ok thanks alot this really helps. does anybody know the range i will get on this 10,000 mah battery back. i weight 130 pounds and will use a single motor
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2017-06-12T19:23:01.650Z Reads: 40

```
The number that matters more than that 10k mah number is watt-hour (Wh), which is parallel group capacity (10 amp-hour) times nominal pack voltage (3.7 volts per cell * 8 groups in series). So you'll have a 296 Wh battery. 

The rule of thumb is that you'll use about 16 Wh per mile so you're looking at around 18.5 miles of range (though you don't really want to drain the battery all the way).
```

---
