# What is the best way to power SSR?

### Replies: 3 Views: 209

## \#1 Posted by: null Posted at: 2018-04-20T08:36:02.295Z Reads: 38

```
Yo! I have Solid State Relay and have a question about how to power it again after surcuit shutdown. Is there any smart way to use properly capacitors or smth so I have small charge when I break 12v circuit and connect it again, so it can power up SSR, which handle 50v, which convert in 12 to power my laptop, SSR and 5v transformer for Arduino and phone.![15242132088121464108041|281x500](upload://m8PSMlcDgZWZdSH5ZzbHrKChinT.jpg)
Thanks!
```

---
## \#2 Posted by: TowerCrisis Posted at: 2018-04-20T08:42:21.180Z Reads: 30

```
Ideally, the SSR can operate on your battery voltage. If it's spec'd for that, you can hook a switch between the positive battery lead and the SSR switch positive, and ground the SSR switch negative. That way when your switch is off, it consumes no power. When switched on, it power's the SSR and the SSR powers the VESC.
```

---
## \#3 Posted by: null Posted at: 2018-04-20T09:09:35.512Z Reads: 26

```
Hey. My SSR requires 5V to operate. It would require 2 additional li-ions. I don't actually have much space, so I thought that I can use 12v of 5v circuit for that. I had that idea but I saved it for later if I don't get how to make circuit with capacitors, that save charge during the usage and store it until the next eboard's "boot" :slight_smile:
```

---
