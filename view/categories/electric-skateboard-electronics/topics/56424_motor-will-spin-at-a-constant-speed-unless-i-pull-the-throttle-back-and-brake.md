# Motor will spin at a constant speed unless i pull the throttle back and brake

### Replies: 6 Views: 227

## \#1 Posted by: EverBlade21 Posted at: 2018-05-23T00:35:39.838Z Reads: 58

```
When I connect my esc to my RX and turn it on, the throttle input is in the middle but the motor will spin at a constant speed unless i pull the throttle back(braking)
```

---
## \#2 Posted by: b264 Posted at: 2018-05-23T00:46:01.144Z Reads: 54

```
You need to adjust your PPM settings to set the center point and deadband in the vesc settings
```

---
## \#3 Posted by: EverBlade21 Posted at: 2018-05-23T01:00:03.366Z Reads: 49

```
Is there a way to adjust that on an esc that only has PWM, @ power inputs and 3 motor outputs? I'm aware this esc isn't specifically for esk8s
```

---
## \#4 Posted by: b264 Posted at: 2018-05-23T01:13:55.289Z Reads: 43

```
If you use the mini remote there is an adjustment on the remote itself, yes.  I don't know if any other remote has that.
```

---
## \#5 Posted by: Deckoz Posted at: 2018-05-23T01:26:27.811Z Reads: 34

```
If it is a car ESC or the like it is probably running some iteration of BLHELI or SimonK.

Just boot up with your throttle in full power, it should make the motors beep. After the calibration beeps end(holding full throttle the whole time), pull throttle to full reverse.

If your motors spin instead of do calibration beeps. You will need to have a remote like @b264 said that can adjust the ppm pulse width....
```

---
## \#6 Posted by: EverBlade21 Posted at: 2018-05-23T01:31:51.596Z Reads: 33

```
OMG thank you so much i totally forgot I could calibrate the esc during start up thank you :laughing:
```

---
