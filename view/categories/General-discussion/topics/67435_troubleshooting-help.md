# Troubleshooting Help

### Replies: 10 Views: 340

## \#1 Posted by: ElBandido Posted at: 2018-09-08T18:02:05.311Z Reads: 45

```
![image|690x451](upload://7qzLQANiYlmMIaH8p6OflDWV8ER.jpeg)

Hey all

I’m so close to the finish line I can taste it.

I’ve been unsuccessful getting the motors to turn tho.  I’ve got everything hooked up, bms correctly installed, and power to the vescs and to the receiver.  What else am I not thinking about?

Y’alls help is greatly appreciated.
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-09-08T18:12:44.255Z Reads: 40

```
Did you do a detection for the motors?
```

---
## \#3 Posted by: ElBandido Posted at: 2018-09-08T18:33:10.168Z Reads: 39

```
Nope.  I guess I wasn't aware of that step.  Is that in the vesc tool?
```

---
## \#4 Posted by: J0ker3366 Posted at: 2018-09-08T18:46:12.654Z Reads: 34

```
https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#5 Posted by: Andy87 Posted at: 2018-09-08T19:01:52.248Z Reads: 27

```
How is it going?
Hope you will fix your batteries in the tray and planed to cover the nickel strips as min with some battery tape. Like this it’s big risk that you short your balance wires sooner or later.

If you not sure with your vesc settings, upload some screenshots and we can have a look if everything is how it should be.
```

---
## \#6 Posted by: L3chef Posted at: 2018-09-08T19:08:59.879Z Reads: 26

```
Are your motor sensored or sensorless? If ther have no sensors you have to spinn them before they will move
```

---
## \#7 Posted by: ElBandido Posted at: 2018-09-11T00:19:25.278Z Reads: 15

```
I've run motor detection, and the motor runs when I run the FOC sensorless test, but I get no response after with the transmitter.
```

---
## \#8 Posted by: goldrabe Posted at: 2018-09-11T00:24:06.640Z Reads: 16

```
Are you using the wizards for setup?
You have to setup your PPM signal with the APP wizard after motor detection.
```

---
## \#9 Posted by: goldrabe Posted at: 2018-09-11T00:27:55.407Z Reads: 14

```
https://www.electric-skateboard.builders/t/how-to-program-canbus-properly-video-tutorial/52606

Thid video is helpful.
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-09-11T22:25:59.334Z Reads: 11

```
i always run detection multiple times on same values to be sure it wasnt a fluke that the detection was successful. How much amps did you set for motor and battery?
```

---
