# Second motor inverted

### Replies: 9 Views: 526

## \#1 Posted by: Dook Posted at: 2018-07-07T17:02:46.022Z Reads: 139

```
Hey Eskate community

I've set up my Dual motors with  VESC6 on Vesc Tool. Set up each motor individually, before linking remote BT UART etc and setting up master and slave VESC. I've obviously effed somenthing up as the motor on the slave VESC is running in reverse. double checked and cables are connected correctly. Help very much appreciated. What have I missed?

Cheers fellas
```

---
## \#2 Posted by: strattos Posted at: 2018-07-07T17:13:23.453Z Reads: 138

```
Swap any 2 phase wires or invert motor direction in vesc tool should change that
```

---
## \#3 Posted by: Sender Posted at: 2018-07-07T17:34:42.795Z Reads: 126

```
What firmware are you running? There is a setting to change motor direction in 3.0 and up. Or like @strattos said, swap two phase wires, then redo detection
```

---
## \#4 Posted by: Dook Posted at: 2018-07-08T09:48:48.409Z Reads: 85

```
Hi I am running firmware 3.38. Were do I find the change motor direction? cheers
```

---
## \#5 Posted by: Moros Posted at: 2018-07-08T10:41:38.291Z Reads: 79

```
This is from the latest version of [Ackmaniacs esc tool.](https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116?u=moros)

![invert%20motor%20direction|690x399](upload://AkcpsfWc3MumGC6AqsQmA0Esnfx.png)

On the General option then under the General tab, you can invert the motor direction. change it to true to make the motor spin the opposite direction.
```

---
## \#6 Posted by: Dook Posted at: 2018-07-08T14:19:44.660Z Reads: 50

```
ok so plugged  into master vesc this is what happens

On false setting, the master VESC motor runs forward, slave VESC motor runs in reverse
On True setting, Both motors run in reverse. Confused.com?
```

---
## \#7 Posted by: Sender Posted at: 2018-07-08T14:28:41.581Z Reads: 46

```
[quote="Dook, post:1, topic:61158"]
the motor on the slave VESC is running in reverse
[/quote]

Set the master back to false.  Write setting. Disconnect.

Plug into slave, Read setting, set to True. Write. Disconnect. Reboot.
```

---
## \#8 Posted by: wafflejock Posted at: 2018-07-08T14:30:56.134Z Reads: 43

```
Hah funny situation there but what @Sender said will likely fix it.  The master likely applies the Boolean to both throttle values the slave one should just effect the slave... If it's still wrong after reversing the slave they should at least both be going the same direction then reverse the master again.  Ah the fun of negation.
```

---
## \#9 Posted by: Dook Posted at: 2018-07-08T14:36:52.798Z Reads: 40

```
Worked, Fixed, thank you so much dude. And this is why this is an awesome community.
```

---
