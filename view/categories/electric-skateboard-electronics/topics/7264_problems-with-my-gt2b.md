# Problems with my GT2B

### Replies: 12 Views: 1094

## \#1 Posted by: Monte Posted at: 2016-08-07T16:29:39.645Z Reads: 137

```
So i have the problem that when i try to connect my gt2b reciever to my vesc, the light on it go on and it look like its connected to my transmitter. But BLDC tool gets no signal. PPM is on, the other stuff i need to run it is on too.
sry for my bad english
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-07T16:33:52.929Z Reads: 140

```
check the display box in bldc tool and see if it's receiving a pulse width signal
```

---
## \#3 Posted by: chaka Posted at: 2016-08-07T16:47:09.982Z Reads: 137

```
Be sure to reboot the bldc-tool after enabling PPM.
```

---
## \#4 Posted by: racidon Posted at: 2016-08-07T16:47:57.280Z Reads: 128

```
You may not have bound it to the controller.

First plug in your receiver using the VCC pins (top lot) and put the bind plug into CH3/BIND
Turn on your VESC (supply power to the Receiver)
Hold on to the Bind button on the GT2B controller and turn it on. It will flash the green light. 
Turn of both your receiver and controller
Charge the plug in your receiver to CH2 and remove the bind plug
Turn on your controller (before the VESC)
Now turn on your VESC
```

---
## \#5 Posted by: Monte Posted at: 2016-08-07T17:04:27.744Z Reads: 112

```
No there is only a pulse when i connect it like @racidon said. But then the reciever is slowly flashing red. And its not working.
Pulse is 0.030
```

---
## \#6 Posted by: Monte Posted at: 2016-08-07T17:05:25.231Z Reads: 106

```
i did but it didnt helped me
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-07T17:11:33.401Z Reads: 102

```
did you make sure you plugged the receiver the correct direction? Maybe a pic would help.
```

---
## \#8 Posted by: Monte Posted at: 2016-08-07T17:15:00.592Z Reads: 98

```
Sry my phone is broken so i cant make a pic at the moment :/ 
The receiver is plugget in the right way. If the red light flashing slowly, bldc gets a signal but i have no idea what slowly blinking mean...
```

---
## \#9 Posted by: Monte Posted at: 2016-08-07T17:18:39.628Z Reads: 98

```
I do it exacly like the guy in this Vid: https://www.youtube.com/watch?v=W-1CZ5wXC4g
But when i switch it back on like him, i get that slow blinking.... 
I checked the cables and everything but there is nothing wrong with it :(
```

---
## \#10 Posted by: chaka Posted at: 2016-08-07T18:04:20.342Z Reads: 91

```
Do you have a multimeter/continuity tester? You may have a bad crimp connection on the signal wire. You should be getting a bright green led on the VESC when you apply throttle or brake.
```

---
## \#11 Posted by: Monte Posted at: 2016-08-07T18:08:25.802Z Reads: 86

```
Yes the vesc and motor is okay, like i said, everythink works exept of the remote
I got a Multimeter somewhere i go to search for it
```

---
## \#12 Posted by: Monte Posted at: 2016-08-07T18:55:32.703Z Reads: 79

```
Okay i got the problem now. It was a litte short on my board from the antenna. :D
```

---
