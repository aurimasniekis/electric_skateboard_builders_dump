# Wiring battery indicator to esc

### Replies: 22 Views: 1476

## \#1 Posted by: Brycehoosiers Posted at: 2017-10-08T18:50:11.906Z Reads: 132

```
So I’m using this Chinese esc for a while until I get a vesc but I’m trying to figure out how to wire the battery indicator so it turns off when I turn the board off. Currently I have it directly wired to the negative and positive leads but it always stays on unless I manually turn it off.
```

---
## \#2 Posted by: Brycehoosiers Posted at: 2017-10-08T18:51:03.884Z Reads: 133

```
<img src="/uploads/db1493/original/3X/f/7/f7029a2ed5f202c162bcff68afb4689be9dc9a98.jpg" width="375" height="500">
```

---
## \#3 Posted by: MontPierre Posted at: 2017-10-08T19:09:30.481Z Reads: 120

```
It should be wired after bms ( if you have one )  and before ESC. So when you flip the switch and your ESC starts up then so will the Voltage meter ;)
```

---
## \#4 Posted by: MontPierre Posted at: 2017-10-08T19:10:35.579Z Reads: 118

```
Btw - does your ESC have switch built in? I’m Not familiar with this model.
```

---
## \#6 Posted by: Brycehoosiers Posted at: 2017-10-08T19:15:52.573Z Reads: 114

```
Yea it has a power button with yellow, black and red wires I 
know normally it would go between the power button but this button has 4 wires
```

---
## \#7 Posted by: MontPierre Posted at: 2017-10-08T19:21:08.165Z Reads: 108

```
Well I don’t think this button is under full battery voltage, if it was the case then cables comming of it would have been much thicker, but I’m not sure myself. Have you got any manual ? I know, it’s a rear thing with Chinese products.
```

---
## \#9 Posted by: Brycehoosiers Posted at: 2017-10-08T19:28:45.054Z Reads: 101

```
Didnt come with a manual , that’s why this is so difficult
```

---
## \#10 Posted by: Namasaki Posted at: 2017-10-08T19:43:04.065Z Reads: 96

```
In order to accomplish what you want,  I recommend that you get an external E-switch or loop key between the battery and the esc.

Unless your are able to find and tap into the full battery voltage on the PCB downstream from the switch. Good luck with that idea.
```

---
## \#11 Posted by: Brycehoosiers Posted at: 2017-10-08T19:44:03.464Z Reads: 87

```
Ok I will probably just use an anti spark key then
```

---
## \#12 Posted by: Namasaki Posted at: 2017-10-08T19:44:40.550Z Reads: 88

```
your gonna need it or an E-switch anyway after you get a Vesc
```

---
## \#13 Posted by: Brycehoosiers Posted at: 2017-10-08T19:45:22.350Z Reads: 86

```
Ok I have some laying around anyways
```

---
## \#14 Posted by: Blacksheep Posted at: 2017-10-08T19:47:24.991Z Reads: 83

```
I have the same esc do you desconect ir when you charge the battery?
```

---
## \#15 Posted by: Brycehoosiers Posted at: 2017-10-08T19:50:22.500Z Reads: 80

```
Yea because I have to plug discharge cables into my balance charger
```

---
## \#16 Posted by: Blacksheep Posted at: 2017-10-08T20:06:55.002Z Reads: 78

```
I don’t have to unplug the cables to charge it but I do because I don’t know
```

---
## \#17 Posted by: Brycehoosiers Posted at: 2017-10-08T20:07:33.598Z Reads: 81

```
What do you mean?
```

---
## \#18 Posted by: Blacksheep Posted at: 2017-10-08T20:13:05.232Z Reads: 82

```
<img src="/uploads/db1493/original/3X/4/5/45acb66d68d34b9d6819a95b97141b60f7336179.jpeg" width="281" height="500">
I have one of this but I don’t know if I can charge it without disconnecting it ?
```

---
## \#20 Posted by: Brycehoosiers Posted at: 2017-10-08T20:16:26.567Z Reads: 78

```
Yea you can do it without disconnecting if you connect everything coreectly
```

---
## \#21 Posted by: Blacksheep Posted at: 2017-10-08T20:17:29.055Z Reads: 74

```
It won’t burn the esc
```

---
## \#22 Posted by: Brycehoosiers Posted at: 2017-10-08T20:17:51.169Z Reads: 72

```
It shouldnt if it’s powered off
```

---
## \#23 Posted by: Brycehoosiers Posted at: 2017-10-08T20:18:08.303Z Reads: 72

```
If you want to be safe you can disconnect it
```

---
## \#24 Posted by: Blacksheep Posted at: 2017-10-08T20:18:13.461Z Reads: 72

```
Ok thanks hehe
```

---
## \#25 Posted by: darkkevind Posted at: 2017-10-08T20:31:35.294Z Reads: 73

```
You could always wire up a little momentary switch on one of the wires for the battery indicator so that it only shows when you press it, even if your board is on like mine?
That way it won't be draining the battery all the time you're using your board either....

<img src="/uploads/db1493/original/3X/a/4/a4a10d48a2778b1dfd57acc4aedf266989522593.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/3/0/30c3a87e90c827dd0a2a7d4de48d85457074160d.jpg" width="690" height="388">
```

---
