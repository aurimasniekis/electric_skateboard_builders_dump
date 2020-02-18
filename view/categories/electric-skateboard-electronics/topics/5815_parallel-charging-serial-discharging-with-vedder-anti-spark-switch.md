# Parallel charging, serial discharging with Vedder Anti-Spark Switch?

### Replies: 4 Views: 1029

## \#1 Posted by: fraannk Posted at: 2016-07-09T17:08:52.295Z Reads: 123

```
Hi guys. 

I'm trying to figure out how to do parallel charging with the Vedder switch in the circuit. I would like it to be as simple as possible, without having to plug/unplug connectors (other than the balance and charge connector of course)

How can I achieve this?
My gear: 
2x 5S batteries connected in serial to one VESC.
Vedder Switch not currently connected to the system
6S charger. 

I know there's a lot of threads about parallel charging, but I couldn't find a circuit with the vedder switch! Thanks
```

---
## \#2 Posted by: ArmandR Posted at: 2016-07-09T18:25:12.157Z Reads: 111

```
Anti-spart?
```

---
## \#3 Posted by: fraannk Posted at: 2016-07-09T18:43:22.217Z Reads: 106

```
Anti-Spark dammit autocorrect
```

---
## \#4 Posted by: Bender Posted at: 2016-07-09T18:45:36.007Z Reads: 105

```
I just did asimilar thing but 2x 6s charging 12s discharge, you do need a loop-key.
[Read this thread](http://www.electric-skateboard.builders/t/how-to-discharge-in-series-and-charge-in-parallel-solved/1589/24) I used the diagram
But added TB's anti-spark switch just before the VESC 
<img src="/uploads/db1493/original/2X/6/6905cb1bed9222024e54218f24475739580e3e6a.png" width="479" height="500">
```

---
