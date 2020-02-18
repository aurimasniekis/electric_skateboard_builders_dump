# Ollin sensored motor to VESC connection?

### Replies: 11 Views: 945

## \#1 Posted by: theviith Posted at: 2017-05-06T18:20:58.209Z Reads: 135

```
Hey guys, does anyone know how to connect the hall sensors for ollin 170kv sensored motors to VESC? The ollin motors has a 5 pin hall sensor which is different than the traditional 6 pin hall sensor. Can someone show me which wire is which and where it should go on the VESC? Thanks in advance
```

---
## \#2 Posted by: laurnts Posted at: 2017-05-06T18:33:26.386Z Reads: 131

```
I think the missing pin is the thermometer sensor pin. As long as the pin matches, although one of the pin is not being used thats fine.
```

---
## \#3 Posted by: Jinra Posted at: 2017-05-06T18:43:39.836Z Reads: 129

```
@laurnts is correct,

Black = GND
Red = +5v

The rest are the 3 sensors.
```

---
## \#4 Posted by: theviith Posted at: 2017-05-06T18:57:45.285Z Reads: 122

```
I see, does it matter which order the 3 sensor wires are in? the wire colors for my motor is red, blue, white, yellow, black in that order. 

So is it safe to assume:
red = +5v
blue = H3
white = H2
yellow = H1
black = GND
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-06T19:06:21.933Z Reads: 117

```
Sensor order doesn't matter on the VESC, just make sure you do motor detection so it knows the position of each sensor.
```

---
## \#6 Posted by: theviith Posted at: 2017-05-06T21:00:26.204Z Reads: 116

```
gotcha, thanks for the help guys!
```

---
## \#7 Posted by: laurnts Posted at: 2017-05-06T23:08:50.516Z Reads: 110

```
Just becareful not to mistake the 3 pins of hall sensors with the temperature pin. The outer edges are the positive and negative.
```

---
## \#8 Posted by: theviith Posted at: 2017-05-12T01:29:57.799Z Reads: 88

```
So after everything is hooked up and starting the motor detection on BLDC, the results came back with "failed to detect hall sensor" I've triple checked my wire connections and everything checks out. When I tested the VESC-X with another 6-pin sensored motor, it was able to detect the hall sensors on that motor. So I'm a little confused as to what might be the problem. The only thing that seem to be different from the two motors is that the Ollin motor has a 5-pin that is missing the Temperature cable. Does anyone know if I need to change some settings in BLDC tool for motor detection to work? This problem did not occur with other 6-pin motors but only with the Ollin motor. Please help, thanks!
```

---
## \#9 Posted by: Jinra Posted at: 2017-05-12T04:40:04.058Z Reads: 82

```
TEMP wire does not need to be plugged for it to detect. Got pics?
```

---
## \#10 Posted by: theviith Posted at: 2017-05-14T05:08:22.316Z Reads: 75

```
nevermind, I got it working. Apparently, it says "failed to detect hall sensor" but the sensor values are already detected. I just need to physically input all the values and they'll work. Not sure why it says that though..
```

---
## \#11 Posted by: Jinra Posted at: 2017-05-14T05:09:58.326Z Reads: 74

```
yea that's weird, mine does not say that when i do detection.
```

---
