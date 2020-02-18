# Brushless motor makes weird &ldquo;puffing&rdquo; noise every few seconds

### Replies: 6 Views: 366

## \#1 Posted by: Jasper Posted at: 2017-11-05T16:28:36.964Z Reads: 65

```
After installing my arduino, esc and motor everything seems to work fine. It arms perfectly and I can make it turn slower and faster with my remote. However once every few seconds the motor makes a weird noise (It seems like it is missing one "step" every few seconds. Anyone got a clue what this might be caused by?
1drv.ms/f/s!AvPQ3WkD_K2yrGfXMwynEvd8PXl4
```

---
## \#2 Posted by: Rinzler Posted at: 2017-11-05T17:05:13.169Z Reads: 55

```
Looks like the esc is revving the motor. Isolate the pwm wires of the vesc from the high voltage battery wires, and try a different remote. Arduino based transmitter and reciever is sketchy as is, more so when going fast on an esk8.
```

---
## \#4 Posted by: Jasper Posted at: 2017-11-05T17:12:19.130Z Reads: 48

```
Im not using a vesc, but 2 arduinos with 2 hc-05 modules and a turnigy sentilon esc, what do you mean with isolating the pwm wires?
```

---
## \#5 Posted by: Rinzler Posted at: 2017-11-05T17:19:04.330Z Reads: 30

```
The three thin wires that feed into your arduido ard the pwn wires of the esc, being a wire the pwn wire can have currents induced by other thicker wire with a flow of electricity. It is likely related to unstable signal or the interference between the two HC-05 modules, or some troublesome arduino code. I would buy a traditional 2.4Ghz remote.
```

---
## \#6 Posted by: Jasper Posted at: 2017-11-05T17:32:32.610Z Reads: 27

```
AAH thanks so much, apparently i can't have a stable pwm output and a stable serial connection at the same time.... well i better look for an alternative i guess..
```

---
## \#7 Posted by: Jasper Posted at: 2017-11-05T17:41:43.626Z Reads: 23

```
And btw for other people, it is possible just DONT combine softwareserial with controlling an ESC, if i use hardware serial the connection is stable
```

---
