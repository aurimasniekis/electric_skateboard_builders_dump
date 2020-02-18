# Arduino board project

### Replies: 2 Views: 414

## \#1 Posted by: pengy Posted at: 2017-04-18T08:30:36.828Z Reads: 86

```
Hey everyone, I am intending to connect a VESC to an Arduino board,  however since the VESC was previously fried.. (not my fault apparantly) and repaired, I'm a little nervous about the connections. I have VESC version 4.12 and trying to connect to the arduino via the PPM pins, I can see the ground pin but don't know which is the one for the signal and which for the 5V.. For testing purposes I'd like to connect a 4s battery and maybe should limit the current draw on the bldc tool.

Thanks for any help
```

---
## \#2 Posted by: rpn314 Posted at: 2017-04-19T03:15:38.896Z Reads: 46

```
Outside: GND
Middle: 5V
Inside: Signal
```

---
