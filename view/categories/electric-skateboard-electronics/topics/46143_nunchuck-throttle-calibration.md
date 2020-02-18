# Nunchuck Throttle calibration?

### Replies: 11 Views: 471

## \#1 Posted by: von_p Posted at: 2018-02-11T21:41:14.354Z Reads: 84

```
Hey all, just built a remote based off of this: https://github.com/RollingGecko/ArduBoardControler and FocBox.
Everything seems to be working fairly well except for the throttle input. In BLDC->App Configuration->Nunchuck display on and joystick at resting position it is at 32% and at full throttle it is at 66%, so there is always resistance on the motor in the "home" position. I have tried playing with the ERPM limit start, ERPM limit start and deadband but does not seem to change anything. How do I adjust this?
```

---
## \#2 Posted by: b264 Posted at: 2018-02-12T02:06:05.145Z Reads: 66

```
Are you using the BLDC_Tool or the VESC_Tool
```

---
## \#3 Posted by: von_p Posted at: 2018-02-12T03:03:11.112Z Reads: 51

```
I am using the BLDC Tool, I did not know there was a VESC Tool. I will try it out, thanks!
```

---
## \#4 Posted by: Pedrodemio Posted at: 2018-02-12T03:42:18.408Z Reads: 50

```
You have to send the data the right way, 0 is full brake and 254 is full throttle 

If you are reading from a analog potentiometer jus use rempack.YJoy = map(analogRead(Pin), 0, 1023, 0, 254) and you are good
```

---
## \#5 Posted by: von_p Posted at: 2018-02-12T06:42:59.812Z Reads: 40

```
Thanks @Pedrodemio , I did have the analog read set to rempack.YJoy = map(analogRead(Pin), 0, 1023, 0, 254), but I think the analog input from my joystick is a little off. I had to massage the 1023 down to about 720 and seems to be working well. Not sure if this is the correct way of adjusting this but it seems to do the trick.
```

---
## \#6 Posted by: Pedrodemio Posted at: 2018-02-12T11:30:25.162Z Reads: 31

```
That’s ok too, mine goes to 98% but I didn’t bother
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2018-02-12T11:40:40.840Z Reads: 31

```
Just a heads up: when using VESC tool you will probably upgrade to the new 3.xx Vesc firmware, however we found out that the whole Nunchuck aspect doesn't work with that right now (problem of the library I guess). So if you're not using FOC I'd suggest staying with firmware 2.xx or modifying ArduBoardControl to use PPM.
```

---
## \#8 Posted by: Pedrodemio Posted at: 2018-02-12T11:44:35.490Z Reads: 29

```
It’s working on 3.33 and 3.34 but not with the library on rolling gecko github, @Pimousse made a modified version that’s work, I think he submitted the changes
```

---
## \#9 Posted by: Der6FingerJo Posted at: 2018-02-12T11:45:05.035Z Reads: 27

```
Ooh alright I wasn't completely up to date on that, thanks!
```

---
## \#10 Posted by: Pimousse Posted at: 2018-02-12T13:14:17.592Z Reads: 26

```
Actually, I took the old library (working with FW2.18) and adjusted the command and values structures and deserialization to match 3.xx firmware.
I didn't change anything else.
So basically, that means that there were no differences on the nunchuck side.

If you're interested, I plan to add COMM_GET_MCCONF in order to set the min scale of the battery gauge exactly to the cutoff set on the VESC.
```

---
## \#11 Posted by: von_p Posted at: 2018-02-12T13:56:32.607Z Reads: 25

```
Thanks for the heads up, I am using the FocBox at 2.18, I was hesitant because I read that there may be some problems with updating the FocBox to the newest firmware and using the VESC Tool. I am new to the forum, are there some threads I should be keeping an eye on for the nunchuck changes?
```

---
