# No PPM signal on Vesc 4.12

### Replies: 3 Views: 168

## \#1 Posted by: AgressivStreetLamp Posted at: 2019-05-15T04:49:35.656Z Reads: 46

```
Alright, so I broke it. Hardeeharhar, now please help me fix it.

I hooked up my torque (sue me) Vesc 4.12 to an 8s batter without any sort of anti spark
I've done this with 12s a few times without much issue and didn't think it would be this time either.
However, this time something went puff. Specifically one of the drains on one of the FETS.

I resoldered the connection and this is where the mystery begins. When I have my vesc connected to the PC, I can use the keyboard to control the motor, but I get no PPM signal. I'm using a cheap remote but I've also tried a PPM servo controller that I know works so the issue isn't the remote. 

Is the PPM read by the DRV? could I have melted that? I'm currently not sure what caused the surge in the first place

.![vescfired|375x500](upload://eSK8PIZsSKSoSMbPWV246YQNEUX.jpeg)
```

---
## \#2 Posted by: linsus Posted at: 2019-05-15T11:51:32.773Z Reads: 31

```
No, the PPM is connected to the MCU. Should be a resistor called R5 in series into pin 57(PB5) on the MCU. Check if you have connection all the way
```

---
## \#3 Posted by: AgressivStreetLamp Posted at: 2019-05-23T05:22:49.612Z Reads: 12

```
Just putting this here for Reference.

Hooked it up as follows:
Bench PSU 12V@ 80 mA or so. remote control connected and output confirmed with Oscope.
Checked the Servo pin on the MCU, no signal.

Noticed the MCU was getting toasty. (hot to touch) under no load besides quiescent current. almost 1 Watt seemed like a lot for the device to just be on... 
Time for some SMD soldering...  Going to replace the MCU.
```

---
