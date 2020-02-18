# Hall sensor detection failed

### Replies: 8 Views: 2308

## \#1 Posted by: MarioGC Posted at: 2017-03-29T01:03:48.458Z Reads: 243

```
Hey e-board builders

Maybe one of you have had this problem before...

One of the motor stoped working due to Hall Sensor Detection Failed.... 

I have checked:
 1.- The wires  from the plug to the sensor board inside the motor, all the wires are OK. 
 2.- Replace the VESC's position, VESC's OK
 
The wiring order I have is:
 - Red
 - White (Temperature)
 - Orange/Blue
 - Green
 - Black

I'm riding a DualDrive 190KV POLAR motors with TorqueBoards VESC's, 

I managed to open the motor and this is what I found with the multimeter.

<img src="/uploads/db1493/original/3X/5/e/5e2553d366ae9d96791fd090afd94e3b72bdf101.jpg" width="566" height="449">

Let me know what would you guys check.
```

---
## \#2 Posted by: Blasto Posted at: 2017-03-29T01:44:31.383Z Reads: 228

```
Wiring looks good, are the halls sitting on the stator or is there a gap?
```

---
## \#3 Posted by: Blasto Posted at: 2017-03-29T01:45:57.351Z Reads: 233

```
[quote="MarioGC, post:1, topic:19878"]
The wiring order I have is: - Red - White (Temperature) - Orange/Blue - Green - Black
[/quote]

Is your connector 5 or 6 pin?
```

---
## \#4 Posted by: torqueboards Posted at: 2017-03-29T03:35:58.678Z Reads: 225

```
Not sure what mode (BLDC/FOC) your testing in but I've found BLDC Sensored or Hybrid Sensored to be a hit or miss. It also seems that Ben has spent more time making FOC Sensored work better than BLDC Sensored.

I haven't had any issues with FOC Sensored but BLDC/Hybrid Sensored has always been a hit or miss for me. @MarioGC
```

---
## \#5 Posted by: Eboosted Posted at: 2017-03-29T05:22:07.861Z Reads: 217

```
[quote="Blasto, post:3, topic:19878"]
Is your connector 5 or 6 pin?
[/quote]

His connector is JST 2.0 6 pin connector andhe is running BLDC.

Is there anyway to change the bad hall sensor somehow?
```

---
## \#6 Posted by: kovjanos Posted at: 2017-03-29T06:05:47.414Z Reads: 211

```
if wiring is OK, next step is to hook up an 5V on it and grab a magnet to test - one-by-one - if your sensors are working
best would be to put your motor back together and just slowly turn it by hand, that way you can test if sensors are always on the 1-2-3-4-5-6 states (never 0 or 7) with rotation in both direction.


<img src="/uploads/db1493/original/3X/b/1/b157185d4bcd2adf8b21ebe2b8c8c8aa04fdcd69.gif" width="430" height="172">
```

---
## \#7 Posted by: torqueboards Posted at: 2017-03-29T06:34:26.895Z Reads: 199

```
I highly doubt it's a bad hall sensor. @Eboosted OP @MarioGC should try to detect in FOC Sensored vs BLDC/Hybrid Sensored and I'm pretty sure it will detect on FOC sensored but fail on BLDC/Hybrid Sensored.

The easiest would be to run the test above. IMO
```

---
## \#8 Posted by: MarioGC Posted at: 2017-03-29T15:03:44.022Z Reads: 186

```
I'll try FOC today, but I've been running BLDC hybrid for 3 months maybe without a problem. 
One motor does detect the sensors. 
I moved the VESC's postition to check if it was the VESC but the same motor was failing. 

I'll keep you updated.
```

---
