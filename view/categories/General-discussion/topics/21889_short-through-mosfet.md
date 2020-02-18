# Short through mosfet?

### Replies: 4 Views: 443

## \#1 Posted by: Zoomic Posted at: 2017-04-27T09:08:54.497Z Reads: 56

```
Hello.

Is it possible to short a mosfet when hooking it up with a power switch? I did that yesterday and the fuse blew. Then I desoldered the output pins and checked the power switch board for any shorts, however there were no shorts. Then I checked between the input terminals on the motor controller and it turned out that there were a short. The only thing I did on the VESC motor controller board was to desolder the 3 wires from the motor and solder them back onto the board. One of the MOSFETS now have a short through it.

How is that possible and what do I do to fix it? I have checked that the outer pin does not connect with the rest, but it still
seems that they somehow are connected.
```

---
## \#2 Posted by: Zoomic Posted at: 2017-04-27T09:09:26.211Z Reads: 55

```
<img src="/uploads/db1493/original/3X/7/1/71a845c4935c4ed1481adb9ba71ac1fab62f50a4.jpg" width="375" height="500">
```

---
## \#3 Posted by: Pantologist Posted at: 2017-04-27T21:29:35.703Z Reads: 38

```
A mosfet is just a switch, so if there was a short it is probably worth your battery somehow or motor.
```

---
## \#4 Posted by: JTAG Posted at: 2017-04-28T20:04:18.578Z Reads: 25

```
You also seem to mis R28, that is a seriously important part :fearful:.
```

---
