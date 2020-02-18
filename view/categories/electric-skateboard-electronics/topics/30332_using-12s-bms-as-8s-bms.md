# Using 12s BMS as 8s BMS

### Replies: 6 Views: 999

## \#1 Posted by: vap Posted at: 2017-08-11T12:33:03.702Z Reads: 161

```
I've got a Supower 12s BMS, but my escs don't behave well on 12s, so i'm running 8s now. Is it possible to use just 8 balancing lines instead of all 12?
It seems like the design is repetitive, and the 12s board i'm using has 13 lines, only the 13th is not connected.
http://www.batterysupports.com/images/48V%2012S%2030A%20Lithium%20BMS_02.jpg

//Of course with a corresponding 33.6v charger.
```

---
## \#2 Posted by: krloz Posted at: 2017-08-11T13:01:50.493Z Reads: 154

```
Don't. 
The balancing part of the board may look and be repetitive but there is more than balancing in a bms. And if you wire the positive or negative leads of the battery or the charger you will either put the bms into some kind of protection state (under voltage I assume) or more probably fry or smoke something
```

---
## \#3 Posted by: krloz Posted at: 2017-08-11T13:04:15.085Z Reads: 149

```
There are however some bms designed for a range of cell counts but
1. It is advertised as a big aspect of said bms.
2. You have to configure and program said bms
3. The one you show Isnt the case because 1
```

---
## \#4 Posted by: vap Posted at: 2017-08-11T20:19:15.009Z Reads: 119

```
Thanks,
Hmm, i think ordering a 8s one would be easier for me than reverse engineering the board :)
```

---
## \#5 Posted by: Namasaki Posted at: 2017-08-12T20:04:33.917Z Reads: 104

```
You could replace your esc with a Vesc. 
Problem solved

RC Car ESC's are designed for RC cars. 
Vescs are designed for E-skates
```

---
## \#6 Posted by: vap Posted at: 2017-08-12T21:55:52.866Z Reads: 87

```
Nah, my 2 vescs went up in flames first time i tried 12s, without any load, while i was standing in place. Didn't like them before that either, too weak for offroad, never know when they throw a fault or overcurrent.
I'll get a vesc when it can handle at least 100 amps and doesn't use that cursed DRV8302.
FVT 120a, POWAAAH!
```

---
