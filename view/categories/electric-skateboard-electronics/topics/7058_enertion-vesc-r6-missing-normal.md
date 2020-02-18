# Enertion VESC R6 missing - normal!

### Replies: 4 Views: 884

## \#1 Posted by: Maxid Posted at: 2016-08-03T07:49:53.286Z Reads: 104

```
After reading http://www.electric-skateboard.builders/t/identify-part-on-my-vesc/7016 I checked my two VESCs that i got from Enertion in July. 
I noticed that R6 is missing on both of them - is that normal? Can't remember to have read about that issue somewhere already so wanted to ask you guys.
<img src="/uploads/db1493/original/2X/6/60e28ec58d8db67f111becd35c391b4ecdb23c28.jpg" width="375" height="500">

Edit: Looking at images online of other VESCs this seems to be indeed normal. Anyone knows why the R6 is omitted but the PCB not changed?
```

---
## \#2 Posted by: furryfrog Posted at: 2016-08-03T08:09:58.646Z Reads: 98

```
If used it is a 0 ohm resistor anyway, schematic notes that its used for USB host. The BOM has it listed but 0 quantity and Do not place.
```

---
## \#3 Posted by: furryfrog Posted at: 2016-08-03T08:12:12.563Z Reads: 96

```
Should note, I Have not seen a VESC in person yet, Waiting for my Raptor, But I did download the schematic and BOM from Vedders website.

R6 just applys 5v to pin 1 of the USB, I assume all connected devices have there own power supply, so not needed.
```

---
## \#4 Posted by: elkick Posted at: 2016-08-03T09:13:04.893Z Reads: 83

```
R6 needs to be omitted, thats correct that way.
```

---
