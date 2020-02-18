# Charger states that the battery is full but it isn&rsquo;t

### Replies: 4 Views: 139

## \#1 Posted by: lambievu0916 Posted at: 2019-04-05T16:18:21.124Z Reads: 50

```
I currently run with a 12sp2 battery with li-ion samsung 30q 3000mah. 
I recently upgraded my vesc firmware and went with foc mode. I pluged in the charger but it charges until 46 volts but really it should be at 50.2 volts. so my "full is 64 percent" Does anyone know whats wrong with this? in my vesc set up i used 6ah and 12 in series, and my voltage/battery reader is set to 12 in series.
```

---
## \#2 Posted by: thisguyhere Posted at: 2019-04-05T16:23:20.387Z Reads: 50

```
i bet one of the cells in your pack is dead.

50.2 - 46 is exactly 4.2 which is voltage of a single cell in your pack.

measure each P group in your pack, i bet you'll find one that's dead.

https://www.electric-skateboard.builders/t/checking-and-correcting-voltage-drift-in-a-battery-pack/87250
```

---
## \#3 Posted by: lambievu0916 Posted at: 2019-04-05T16:32:04.099Z Reads: 44

```
That makes sense, the bms has been hot a bit lately
```

---
## \#4 Posted by: meesie Posted at: 2019-04-05T17:09:52.429Z Reads: 29

```
had the same problem. it was a dead cell. after replacing the cell it charges to 100% again :+1:
```

---
