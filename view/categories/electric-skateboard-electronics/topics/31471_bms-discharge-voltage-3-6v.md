# Bms Discharge voltage 3.6V?

### Replies: 11 Views: 831

## \#1 Posted by: karosass1 Posted at: 2017-08-25T15:31:16.582Z Reads: 89

```
So I burned my BMS (which might be the cause of problem in the title) by plugging balance connectors with reversed voltages. I have a spare BMS, but to check if I got balance wires correct now, I'm still using the burned BMS (only the resistor by lowest voltage balance wire port got burned. I changed the balance wires and plugged everything again into BMS, nothing else is burning thankfully, but voltage meter doesnt light up and when I checked discharge port with multimeter it showed 3.6V which should be 10x bigger (10s battery)

Is this due to that BMS is burned or I wired something wrong?

My diagram:

http://i.imgur.com/HyQ68qv.png

Diagram by bestech:

http://i.imgur.com/CBCDo5d.png

One thing to note, I just assume those wires are e-switch and I just wired them together.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-08-25T15:45:51.478Z Reads: 79

```
[quote="karosass1, post:1, topic:31471"]
Is this due to that BMS is burned
[/quote]

Most likely yes. 
The balance circuit is damaged.
 The bms is not going to output
```

---
## \#3 Posted by: karosass1 Posted at: 2017-08-25T16:14:34.446Z Reads: 72

```
Connected new bms in same way, nothing smoked in its part. But it's still outputs 3.7V

Connecting what I think is eswitch doesn't change it
```

---
## \#4 Posted by: karosass1 Posted at: 2017-08-25T16:27:17.122Z Reads: 67

```
Idk why, but disconnecting and reconnecting voltage meter fixed it
```

---
## \#5 Posted by: Jinra Posted at: 2017-08-25T16:42:03.420Z Reads: 60

```
Does that BMS even provide an adequate discharge current?
```

---
## \#6 Posted by: karosass1 Posted at: 2017-08-25T16:44:59.642Z Reads: 55

```
60A, yes, but as i said , disconnecting and reconnecting voltage meter at discharge port fixed the problem completely
```

---
## \#7 Posted by: Jinra Posted at: 2017-08-25T16:47:45.396Z Reads: 52

```
Hm, not a bad size for a 70A continuous BMS
```

---
## \#8 Posted by: MontPierre Posted at: 2017-08-26T14:04:07.942Z Reads: 42

```
How can you check if a resistor got burned ? I have also plugged in balance wires in wrong order and now during acceleration my bms shuts off. Shall I probe resistors with multimeter and check if they are same resistance ? Shall I have motor running during this process ? If it is a small resistor I would be tempted to replace it myself.
```

---
## \#9 Posted by: karosass1 Posted at: 2017-08-26T14:22:19.738Z Reads: 36

```
Try to find the burnt ones :smile:
<img src="/uploads/db1493/original/3X/a/a/aa3a45e1fb865d99a96993b5dab6eefdc5622d6a.jpg" width="375" height="500">
```

---
## \#10 Posted by: MontPierre Posted at: 2017-08-26T14:27:31.824Z Reads: 33

```
Hahah! Mine look good :/ so I have tougher problem
;)
```

---
## \#11 Posted by: Deckoz Posted at: 2017-08-26T21:16:38.520Z Reads: 30

```
Multimeter probe in diode test/continuity test mode...
```

---
