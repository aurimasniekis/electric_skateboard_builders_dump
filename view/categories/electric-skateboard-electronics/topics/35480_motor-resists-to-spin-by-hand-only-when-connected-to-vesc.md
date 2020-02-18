# Motor resists to spin by hand, only when connected to Vesc

### Replies: 5 Views: 301

## \#1 Posted by: Idobartal Posted at: 2017-10-14T00:03:23.270Z Reads: 54

```
Hi guys, im building a dual motor and im having problems with one of the motors, the motor spins freely while not connected to power (so the phase wires aren’t shorting one another), but when im powering the system, the motor resists to spinning by hand (just to be clear, although its resisting to spin by hand, its spinning fine while pulling the rc triger, but seems to struggle and stops quickly after releasing the trigger)
What is the problem??? 
 i want to know if i fried the basterd or just a minor glitch that i can fix and continue with the complex bldc tool setup (which is not so easy for dual mode over canbus... lots of hiccups in the process)
Thanks !
```

---
## \#2 Posted by: Namasaki Posted at: 2017-10-14T00:18:03.811Z Reads: 51

```
you need to calibrate your controller in the bldc tool
```

---
## \#3 Posted by: notepad Posted at: 2017-10-14T00:18:42.044Z Reads: 52

```
Make sure the settings are in order. I remember somewhere that controller calibration can lead to the motor bastically breaking when the throttle is set to 0.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-10-14T00:19:15.421Z Reads: 51

```
https://www.youtube.com/watch?v=OtuofrQr3F8&t=12s
```

---
## \#5 Posted by: Idobartal Posted at: 2017-10-14T00:35:48.915Z Reads: 47

```
Checking it asap and updating you!  i didn’t  think about it so thx!!!
```

---
