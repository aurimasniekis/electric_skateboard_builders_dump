# Connect bluetooth LE UART dongle and nunchuck receiver at the same time?

### Replies: 11 Views: 646

## \#1 Posted by: Moja Posted at: 2017-03-01T20:10:58.723Z Reads: 89

```
I am running 2x VESC 4.10 and i have a Nunchuck receiver plugged into the P3 port. I have ordered a bluetooth dongle to interface with the Android app and it states in the instructions that it should also plug into the P3 port.

 Can I use the P2 port? Or can I use the UART P3 port on the slave VESC and CAN FWD the bluetooth configuration commands to the master VESC? Any other ideas would be great.
```

---
## \#2 Posted by: Moja Posted at: 2017-03-02T21:59:33.120Z Reads: 62

```
<img src="/uploads/db1493/original/3X/3/0/308f19a5ecfa0cce03d09ffb5e97d912cb6be913.jpg" width="666" height="500">
```

---
## \#3 Posted by: lowGuido Posted at: 2017-03-02T22:41:22.328Z Reads: 58

```
if you have 2 VESC you can put the nunchuck on one and the bluetooth on the other.
```

---
## \#4 Posted by: rpn314 Posted at: 2017-03-03T01:34:49.037Z Reads: 53

```
Accurate. I don't know if many of the apps out there forward configurations onto the master VESC, but unless you're changing major settings, I don't think it'll be much of a problem.
```

---
## \#5 Posted by: Moja Posted at: 2017-03-03T14:44:03.919Z Reads: 43

```
I intend to have as much control over settings as possible. It would be ashame if all I can do is monitor, that's not much use
```

---
## \#6 Posted by: rpn314 Posted at: 2017-03-03T18:28:48.127Z Reads: 39

```
You could change max ERPM configuration on one VESC and it will essentially keep the other in line, but changing things like motor parameters on one and not the other is going to cause you problems.

On the app side of things, it is possible to have the app send the configuration to both VESCs, I just don't know of any app that has implemented it.
```

---
## \#7 Posted by: Moja Posted at: 2017-03-03T20:52:11.242Z Reads: 36

```

So using bluetooth to configure the vesc is only useful for single motor setups?
```

---
## \#8 Posted by: Moja Posted at: 2017-03-03T20:53:02.940Z Reads: 36

```
Phone apps via Bluetooth I mean
```

---
## \#9 Posted by: lowGuido Posted at: 2017-03-03T21:06:54.264Z Reads: 33

```
you should be able initially setup VESC ID's and then select each one and configure separately. you might be limited by the software though.. it should be possible.
```

---
## \#10 Posted by: Maxid Posted at: 2017-03-03T21:09:43.461Z Reads: 31

```
AFAIK @Ackmaniac's firmware can do this
```

---
## \#11 Posted by: rpn314 Posted at: 2017-03-04T13:32:07.709Z Reads: 30

```
[quote="lowGuido, post:9, topic:18421, full:true"]
you should be able initially setup VESC ID's and then select each one and configure separately. you might be limited by the software though.. it should be possible.
[/quote]

You should do all the initial confirmation in BLDC Tool (where you can set the can-bus IDs). And it is _possible_ for an app to configure both VESCs over Bluetooth using the UART of one of them, I'm just not aware of any app that has implemented it. 

[quote="Maxid, post:10, topic:18421, full:true"]
AFAIK @Ackmaniac's firmware can do this
[/quote]

REALLY?! I've been following his work. He's done an amazing job, but I haven't implemented it because of  the android only app right now so I wasn't aware of that.
```

---
