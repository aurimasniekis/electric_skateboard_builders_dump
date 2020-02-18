# Extending VESC power switch wire?

### Replies: 9 Views: 181

## \#1 Posted by: Lumaci Posted at: 2019-06-05T07:31:42.034Z Reads: 61

```
Ive got a Flipsky Vesc 4.20 and i want to mount the power button at the top, after seing it done on the Unity i headed out to find the parts.

But before i pull the trigger from hobbyking, this should work right? Or do i need to add anything to the wires to help it?

Never done it before, i need to extend it around 80cm.
```

---
## \#2 Posted by: linsus Posted at: 2019-06-05T07:48:06.249Z Reads: 57

```
pictures help
```

---
## \#3 Posted by: Lumaci Posted at: 2019-06-05T07:49:38.843Z Reads: 52

```
Its just a normal power button like this

![image|387x295](upload://isaPacE0zKBOelqyeoXVHbXkOXU.jpeg)
```

---
## \#4 Posted by: linsus Posted at: 2019-06-05T07:53:53.385Z Reads: 51

```
80 cm extra cable? Holy shit. how even..
Will probably work but the shorter cables the better
```

---
## \#5 Posted by: Lumaci Posted at: 2019-06-05T07:55:34.586Z Reads: 53

```
Pretty long yeah, i need it to go from here to here.

Its around 60 - 65cm then some room for the wire to go into the vesc and enclosure at top.

![image|375x500](upload://p7Lmr2UxsmKVzqfdNLQV0kKIOgE.jpeg)
```

---
## \#6 Posted by: LEE Posted at: 2019-06-05T08:18:06.888Z Reads: 45

```
That Flipsky switch is like an alternate switch.
Firmly coat the cable so that it is not cut.
Should the cable be broken, the VESC will also be powered off.

Unity is a momentary switch.
Momentary power turns on by momentary energization, and turns off again by momentary energization.
In the case of Unity, it seems that the power will not turn off even if the cable is broken while driving.
Of course I have not tried it.
The cable has never been broken.

In the case of the alternate switch, make a particularly robust connection.
The shorter the cable, the more robust it is.
```

---
## \#7 Posted by: Lumaci Posted at: 2019-06-05T08:23:40.559Z Reads: 46

```
Using very thick insolated cables and kapton tape over each line with a rubber coat on the deck where everywire is so that should prevent any damage or cuts.

But yeah its a bit long, i know when you do power wires you add something but on these you dont add like a res or cap?
```

---
## \#8 Posted by: LEE Posted at: 2019-06-05T08:47:02.338Z Reads: 43

```
It is important to be able to keep the power on.
A cable extension of about 60 cm seems to have no electrical problems.
Physical problems such as broken cables due to vibration etc. are more scary.
Alternate switches are a bit scary.

The momentary switch can extend the cable more safely.
In the case of momentary switches, the only problem is when turning the power on / off.
It is not necessary for the VESC to turn off, even if the cable is broken while riding.
```

---
## \#9 Posted by: LEE Posted at: 2019-06-05T09:05:38.299Z Reads: 41

```
![image|690x443](upload://1CIdRq8pgHU1m0VyG8TxNMWBSJ9.jpeg) 

The FSESC holds the power supply by a latch.
Unity recognizes each as an ON / OFF signal when the button is pressed.
```

---
