# DRV-Fault, connection lost for 3 seconds. Maybe BMS?

### Replies: 7 Views: 321

## \#1 Posted by: Goofycat Posted at: 2018-04-18T14:33:50.946Z Reads: 68

```
Hey, 
I have a problem with a board. The board consists of the following components:
Enertion Space Cell Pro 3 (10s3p, fuse, XT60, charger, BMS, display)
DIYElectric VESC 4.12 v.218 ( at the moment firmware 2.54 with the ackermaniac BLDC Tool)
Torque Boards 6355 Engine, 230 kV

The board went really well and had no problems. 

At some point I noticed, however, that the connection occasionally breaks off and one can neither accelerate nor brake. after about 3 seconds of waiting, the board can be controlled normally again. 
When reading out with the BLDC tool, the same error occurred and the error code FAULT_CODE_DRV8302 is displayed. (When this failure happens, the red LED Blinks 2x3Times )

Motor detection works (Hall sensors are not detected (tested on 2 motors)), but when trying to accelerate the motor with the arrow keys the error FAULT_CODE_DRV8302 appears immediately. 

Furthermore, I noticed that the Space Cell3 only shows 100% as charging display (if you change to display=battery voltage, the correct voltage is displayed). 

Has anyone ever had such a mistake or does anyone know of a solution? You can ride the board, but with the interruptions it's too dangerous! 
I am grateful for any help! 


Greetings Andre
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-04-18T14:52:20.277Z Reads: 59

```
buy a new vesc.
```

---
## \#3 Posted by: Goofycat Posted at: 2018-04-18T14:54:55.165Z Reads: 58

```
hmm would be the easiest option. But wich one?
```

---
## \#4 Posted by: FabianOdermatt Posted at: 2018-04-18T19:10:22.733Z Reads: 44

```
Go for a FOCBox, or even a ESCape. :slight_smile:
```

---
## \#5 Posted by: Chewie Posted at: 2018-04-18T20:24:51.236Z Reads: 36

```
DIYelectric VESC's suck, they're known to be garbage and they keep selling them. (mine died doing 5mph in a parking lot)
F*** DIYelectric with a fork
```

---
## \#6 Posted by: Chewie Posted at: 2018-04-18T20:25:10.938Z Reads: 36

```
Pretty happy with my FOCbox
```

---
## \#7 Posted by: Thelifelonglearner Posted at: 2019-08-11T13:50:41.896Z Reads: 7

```
Did you figure out what was the issue ?
```

---
