# VESC not responding to input

### Replies: 8 Views: 852

## \#1 Posted by: richardx Posted at: 2017-08-08T22:47:53.585Z Reads: 83

```
I'm using a Torqueboards VESC with their Nano remote. When I connect the board to the BLDC tool, I can move the motor with the arrow keys, and I can see my pulsewidth changing. However, the display for pulsewidth doesn't move at all, and the remote doesn't move the motor. The LED for ESC activity also doesn't light up when I move the remote (it does when I use arrow keys). Does anybody know what my problem is and how to fix it?
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-08T22:49:00.671Z Reads: 83

```
Did you choose "PPM" from App config > General?

Also, did you choose a control mode in App config > PPM?
```

---
## \#3 Posted by: richardx Posted at: 2017-08-08T23:53:04.083Z Reads: 76

```
Yes, my app is currently set to PPM and my control mode is set to "Current no reverse with brake".
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-08T23:54:15.658Z Reads: 72

```
Pic on how it's hooked up from receiver to VESC?
```

---
## \#5 Posted by: MontPierre Posted at: 2017-08-09T00:00:50.500Z Reads: 67

```
I think when you change from ppm to no app and vice Versa you have to reboot vesc to take effect . Had the same problem an hour ago.
```

---
## \#6 Posted by: richardx Posted at: 2017-08-09T17:21:24.919Z Reads: 58

```
The VESC was already set to that as default/factory settings, but I also rebooted it.
```

---
## \#7 Posted by: Martinsp Posted at: 2017-08-09T17:49:56.210Z Reads: 55

```
If there is no mechanical ptoblem I would save the config to save time to XML file and flash the firmware because this seems like a rare issue which is most probably something like an unfortunate software bug that happened when flashing in factory. Check the mechanical connection etc before you do anything else. Maybe try a different remote if you can because it may as well be a remote/receiver problem.

is the remote and receiver binded correctly?
```

---
## \#8 Posted by: Mainsedora Posted at: 2019-04-18T22:26:53.344Z Reads: 17

```
Solution for this. Set it to no App, then it'll work right away with arrow keys
```

---
