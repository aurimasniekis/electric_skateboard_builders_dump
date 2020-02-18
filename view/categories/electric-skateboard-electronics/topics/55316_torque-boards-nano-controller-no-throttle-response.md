# Torque Boards Nano Controller No Throttle Response

### Replies: 11 Views: 417

## \#1 Posted by: Makkaman Posted at: 2018-05-13T18:36:00.087Z Reads: 41

```
Hello all. I'm having an issue with my TorqueBoards 2.4Ghz Nano remote showing a constant, flickering throttle response around 1.54ms. The controller seems to sync properly. I am throttling fully forward and backwards when powering on, as I have read elsewhere that this controller must be calibrated at each boot. But I still see no response in VESC Tool when throttling the controller. When I switch to "Current No Reverse With Brake" and try to control the motor with my keyboard arrow keys, I hear a crackling sound and the motor doesnt spin. When the controller type is changed to "Off" the keyboard arrows can control the motor.

Attached are a few screenshots and a snapshot of the wiring. Please advise if you think that my controller is defective or if I am missing a step.

TorqueBoards Controller: collections/remote-controller/products/torqueboards-2-4ghz-nano-remote-controller


![Capture|690x442](upload://6ZnEBviChMnKUdUOvAKkIsSZJZI.PNG)![Capture 2|690x441](upload://dxFJ5q6T9cxJKzDtdwBaGAJSlGY.PNG)![20180513_112820|690x388](upload://7sB2ySvrMCR6xHIfvrrZDhE74Pz.jpg)
```

---
## \#2 Posted by: Jinra Posted at: 2018-05-13T18:45:48.352Z Reads: 35

```
Did you switch the mode to PPM and write config in the "App settings > General" tab?
```

---
## \#3 Posted by: Makkaman Posted at: 2018-05-13T18:54:43.037Z Reads: 33

```
I don't see the option to set the mode to PPM. From the left column, I am in the PPM settings and on the "General" tab. I have set the Control Type to "Current No Reverse With Brake"

Through the Input Setup Wizard, I did select PPM controller upon initial.
```

---
## \#4 Posted by: Jinra Posted at: 2018-05-13T18:56:42.084Z Reads: 31

```
See here
![image|676x390](upload://eFaCUy1i0TygsPG6e4OdgMFo4Mk.png)

Make sure to write the config too before you try.
```

---
## \#5 Posted by: Makkaman Posted at: 2018-05-13T18:59:19.185Z Reads: 27

```
I had not...but now set to PPM and written to the VESC. Still not responding.

It was set to PPM and UART. Should I concern over the settings below this such as Send CAN Status and Can rate? I assume this is for a dual VESC build which mine is not.

![Capture 3|690x329](upload://okm8IYMCX40YFpkYwMpeJWlte49.PNG)
```

---
## \#6 Posted by: Jinra Posted at: 2018-05-13T19:00:45.171Z Reads: 26

```
You shouldn't be sending CAN status if you're using the PPM app, it should be false.
```

---
## \#7 Posted by: Makkaman Posted at: 2018-05-13T19:02:10.272Z Reads: 27

```
I just made an observation. When the controller is off, I am still receiving that flickering signal around 1.54ms in VESC Tool. Shouldnt it be static at this point?
```

---
## \#8 Posted by: Jinra Posted at: 2018-05-13T19:02:37.725Z Reads: 25

```
No, it's receiving the neutral PPM signal from the receiver
```

---
## \#9 Posted by: Makkaman Posted at: 2018-05-13T19:03:54.609Z Reads: 23

```
That makes sense. Is there a way to troubleshoot the throttle on my controller? Sounds like this may be the root of my problem.
```

---
## \#10 Posted by: Jinra Posted at: 2018-05-13T19:04:19.980Z Reads: 25

```
Well did you try it again with send can status off?
```

---
## \#13 Posted by: Makkaman Posted at: 2018-05-13T19:40:32.434Z Reads: 23

```
[quote="Makkaman, post:11, topic:55316, full:true"]
I did. Same results.
[/quote]

I did. Same results.
```

---
