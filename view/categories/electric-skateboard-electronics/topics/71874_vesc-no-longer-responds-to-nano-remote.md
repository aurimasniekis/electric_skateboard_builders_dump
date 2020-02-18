# VESC no longer responds to nano remote

### Replies: 10 Views: 275

## \#1 Posted by: ravedown Posted at: 2018-10-21T07:16:48.961Z Reads: 75

```
Hi all-

I am a first time builder, and finally received all my parts this weekend.  Here's what I've got:

10S2P battery from DIYesk8
2 6355 190 kV motores from Torqueboards
1 dual FSESC4.20 by Flipsky
1 nano remote and receiver from Torqueboards
1 Trivent 300A anti-spark power switch

I did a dry fit and configured the VESC with the new VESC tool, and it all worked.  I noted that every time I trigger the remote, the green LEDs on the dual VESC both light up.

I disassembled everything and mount everything up on the board and trucks, powered up, and the remote no longer lit up the green LEDs on the VESC.

I reset everything back to defaults and started over, and still didn't work.  I tested the voltage on the receiver and it looked like is was ~200mV at full brake and ~320mV at full forward.  I tested this on the VESC side of the connection as well.

No idea what to troubleshoot next.

Any ideas?

Thanks,

Pej
```

---
## \#2 Posted by: baxtred Posted at: 2018-10-21T08:06:53.096Z Reads: 62

```
Plug in your VESC, open the new VESC tool program, click the connect button, and configure the "app" settings. When you get to the PPM screen where there is a black bar with green, take a picture and post it here.

Uploading pictures isn't working: https://www.vesc-project.com/sites/default/files/Manuals/MSW_03_connect.jpg

In that picture, there is the Input Setup Wizard for app in the bottom right corner. Click that. Go through the first few screens and stop when you get to the black bar as explained above.
```

---
## \#3 Posted by: baxtred Posted at: 2018-10-21T08:15:44.880Z Reads: 55

```
Additionally, PPM recievers run off a pulse frequency and not really a voltage. Higher throttle ranges send more spaces out pulses while low throttle ranges sense out less pulses. For example full brake is normal a pulse every 1 millisecond, while full throttle is 2 milliseconds. Neutral throttle is 1.5 ms. Basically the VESC can figure out how fast your want to go by measuring the time between pulses.
```

---
## \#4 Posted by: ravedown Posted at: 2018-10-21T17:19:17.309Z Reads: 40

```
![ppm%20mapping|690x406](upload://rl2zUeFvSLPpXODh38N3SAo5LEF.png)
```

---
## \#5 Posted by: ravedown Posted at: 2018-10-21T17:23:10.882Z Reads: 38

```
Also, here are a few photos of the setup

![41|374x500](upload://flUQ9qL5NfttEJaEje3UnWMOz8e.jpeg) ![38|374x500](upload://ydcn8ebvChmwc70aOG8tR8yoUye.jpeg) 

The second shows the vesc upon power up.  Note the green and blue LEDs are on.  Use of the nano does not do anything nor does the green LED get brighter.

In the first, I have connected VESC tool and controlling the VESC via the keyboard.  Note that the green LED is bright while receiving input from the VESC tool.

Thanks for your help

Pej
```

---
## \#6 Posted by: baxtred Posted at: 2018-10-21T17:51:19.411Z Reads: 36

```
Here's a couple ideas:

![Screenshot_20181021-114648_Chrome|243x500](upload://mCiudXuiebgHbYbuLr5whkf9Nfs.jpeg)

Ensure the can bus switch is on. 

Go to the PPM, and change Multiple ESCs over CAN to true and write to the ESC using the "A symbol with a down arrow" on the right side of your screen. 

![20181021_115011|666x500](upload://vFcEwL8P3Krq7Tx6k16sY19IdPh.jpeg)
```

---
## \#7 Posted by: baxtred Posted at: 2018-10-21T17:56:17.901Z Reads: 31

```
Once you have flashed the ESCs over CAN = true thing. Go back to the Welcome and Wizards and click input setup wizard. When prompted to load default configuration say "No". See if you can now see the remotes input. If that doesn't work try configuring the slave and see if that recognizes the control.
```

---
## \#8 Posted by: ravedown Posted at: 2018-10-21T18:52:01.530Z Reads: 28

```
Thanks Baxtred.  The switch was already set to ON.  Whats interesting is if I click the CAN icon on the far left of the VESC tool, I can see remote input register in the PPM pulselength settings, but only when plugged into VESC 2.  Weird.  It still doesn't control the motors, though.

Pej
```

---
## \#9 Posted by: ravedown Posted at: 2018-10-22T06:39:34.465Z Reads: 26

```
Ok, I figured it out.  The dual vesc HW config seems to be hardwired, ie only one specific VESC can be master and the other has to be slave.  You can't flip it around.  I only figured this out when I noticed the "1" and "2" on the unit (see pic).  Everything works as expected now.  I was trying to configure "2" as master and "1" as slave.  Once I flipped it around, everything started working.  Thanks for your help Baxtred.

![dualvesc|603x500](upload://dCjvkPPgMPp4zzoqnYxCtBFT9wV.jpeg)
```

---
## \#10 Posted by: baxtred Posted at: 2018-10-22T06:51:24.101Z Reads: 24

```
Glad you figured it out. No problem!
```

---
