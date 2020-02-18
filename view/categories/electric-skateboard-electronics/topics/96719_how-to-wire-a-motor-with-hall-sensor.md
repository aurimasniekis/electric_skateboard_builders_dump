# How to wire a motor with hall sensor?

### Replies: 6 Views: 320

## \#1 Posted by: ebuilder Posted at: 2019-06-16T12:23:10.116Z Reads: 48

```
I didn’t find any wiring diagram about how to wire the hall sensor of an electric longboard motor. Where the hall sensor wires should be connected?

1) To the esc as the esc needs to know the position and the speed of the motor? 

2) To the receiver as the receiver might need to know the position and the speed of the motor in order to adjust the signal command that will send to the esc?

3) To both the esc and the receiver as both need to know informations about the motor?
```

---
## \#2 Posted by: McErono Posted at: 2019-06-16T12:50:46.103Z Reads: 44

```
You just plug the motor sensor wires into the esc, done.

You may need sensor adapter cables though.
https:///products/vesc-sensor-wires
```

---
## \#3 Posted by: ebuilder Posted at: 2019-06-16T12:55:32.439Z Reads: 39

```
And if there is an ESP that powers 2 motors, will that ESP have two special inputs for 2 hall sensors from the two motors?
```

---
## \#4 Posted by: McErono Posted at: 2019-06-16T12:57:13.610Z Reads: 39

```
Yes on dual vesc there are two sensor inputs.
```

---
## \#5 Posted by: ebuilder Posted at: 2019-06-16T13:07:13.282Z Reads: 37

```
Thank you for your answer. I looked at the picture from your link. The connector from the right side of the picture has 6 pins and 6 wires and I think that is the hall motor to esc connector. 
Why it needs 6 wires? Does it transmits to the ESC 6 different motor positions of the hall motor or it transmits 3 different positions by using 2 wires for each position?
```

---
## \#6 Posted by: McErono Posted at: 2019-06-16T13:11:11.282Z Reads: 32

```
No there are 3 phase wires on your motor so 3 wires of the sensor cables are the phases. One is negative, one positive and the sixth wire is the temperature reading if the motor has a temp sensor.

![teaserbox_2460885724|690x489](upload://azgtrQXrLHkpkA1yOmwCtkVYKrT.png)
```

---
