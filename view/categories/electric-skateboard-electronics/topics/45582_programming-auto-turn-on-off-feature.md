# Programming Auto Turn On &amp; Off Feature

### Replies: 9 Views: 784

## \#1 Posted by: Jc06505n Posted at: 2018-02-05T00:06:22.032Z Reads: 142

```
I like the features that the DIYEBoard ESC has where one can auto turn on the board via pushing and after a while of inactivity, the board turns off. How can one program that into a Focbox/VESC?
```

---
## \#2 Posted by: SOICDIP Posted at: 2018-02-05T00:35:27.478Z Reads: 138

```
An Arduino that controls a FET anti spark switch with an accelerometer? 

It would need a separate buck converter though.
```

---
## \#3 Posted by: b264 Posted at: 2018-02-05T01:08:41.190Z Reads: 126

```
You could probably do without the arduino and just use a FET antispark with accelerometer and a couple other discrete pieces if you didn't need to be able to reprogram the delays, or maybe just an ATtiny85 / ADXL354

Powering the circuit would probably be a challenge too though like @SOICDIP noted.  10S and 12S are beyond the max input voltage for most 5 volt regulators
```

---
## \#4 Posted by: Pedrodemio Posted at: 2018-02-05T01:22:37.148Z Reads: 116

```
If you use an anti spark switch and add a soft latch using an micro controller it doesn’t even need to be implemented 

On the soft latch you hold the button until the micro controller turns on and the first task on the routine is to activate the FET of the switch

If you push the board, the back EMF of the motors would power the VESC on which in turns turn the micro controller and latch’s the board at ON state

Actually would be harder to do the opposite of that since the button itself would need to be wired to the micro controller, it would only power on if it detects the button pressed
```

---
## \#5 Posted by: b264 Posted at: 2018-02-05T01:23:19.098Z Reads: 103

```
What kind of interest is there around here for this stuff

[poll type=regular public=true]
* I don't want auto turn-ON
* I might want auto turn-ON
* I definitely want auto turn-ON
[/poll]
[poll name=poll2 type=regular public=true]
* I don't want auto turn-OFF
* I might want auto turn-OFF
* I definitely want auto turn-OFF
[/poll]
```

---
## \#6 Posted by: lock Posted at: 2018-02-05T01:24:26.872Z Reads: 94

```
The [DieBieMS](https://github.com/DieBieEngineering/DieBieMS) BMS will turn off automatically after 30min or so if you don't exceed a current threshold in that period (eg; 0.5a). I should probably keep that in mind if I ever plan on rolling down a long hill 😂.

It might be worth having a look through the power management schematic about how it uses a momentary switch and keeps itself turned on. Admittedly it all makes little sense to me...
```

---
## \#7 Posted by: Martinsp Posted at: 2018-02-05T01:27:26.708Z Reads: 91

```
It could be as simple as the VESC powers on the micro controller which as you said powers it on and turns a mosfet on and that mosfet would be on only if the arduino or other micro controller would be on so the pushbutton would disconnect the power to the controller which would turn of and turn the mosfet off which would turn the vesc off. 
But I might be missing something it is 3am here :D
```

---
## \#8 Posted by: Pedrodemio Posted at: 2018-02-05T02:25:03.096Z Reads: 80

```
I think that’s right, the two possibilities would be

- turns on with the board rolling
   Micro controller turns on and latch the mosfet


- don’t turn on

   Micro controller turns on, checks of the power button is pressed and then turn on the mosfet, in this case the switch must be 2 poles, one for the initial current flow and another hooked up to an input
```

---
## \#9 Posted by: chuttney1 Posted at: 2018-02-05T03:14:08.714Z Reads: 69

```
This can only work if the BMS is in control.
```

---
