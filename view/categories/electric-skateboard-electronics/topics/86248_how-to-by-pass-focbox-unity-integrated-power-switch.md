# How to by pass FocBox Unity integrated Power switch

### Replies: 6 Views: 384

## \#1 Posted by: Celt Posted at: 2019-03-05T23:53:35.500Z Reads: 133

```
Hey guys,

I have a Torque Boards 12S4P battery (The TB battery has everything integrated) and dual 6355 motors and I need a way to by pass the integrated power switch in the FocBox Unity. Is there a way? Besides doing a push to start.

Thanks!
```

---
## \#2 Posted by: brenternet Posted at: 2019-03-05T23:56:38.453Z Reads: 133

```
Unplug it and turn auto shutdown off in the software?
```

---
## \#3 Posted by: Indiangummy Posted at: 2019-03-05T23:58:07.226Z Reads: 131

```
You have to short the pins on the unity so it is in always on mode. Then you can add your loop key.
 If you have nothing pluged in to the switch port of the unity it will always be off no matter what you do. You have to make a cable and short the pins.
```

---
## \#4 Posted by: nuttyjeff Posted at: 2019-03-06T00:01:34.272Z Reads: 127

```
![f875eab383a1c81171c2faa6ce0cd8bd01fc2935_2_1332x1000|666x500](upload://9y0XKiQRkBubl8PaJkFkgAmCySB.jpeg) 

Make the jst cable on the right and plug that into the switch plug to connect the pins.
```

---
## \#6 Posted by: Celt Posted at: 2019-03-06T00:06:24.919Z Reads: 124

```
[2m](https://www.electric-skateboard.builders/t/how-to-by-pass-focbox-unity-integrated-power-switch/86248/5?u=celt)

Hey thanks! I don’t know how to make that!
What do I need?
```

---
## \#7 Posted by: nuttyjeff Posted at: 2019-03-06T00:24:01.316Z Reads: 115

```
A jst 2 pin connector with wires, then solder the 2 wires together.
```

---
