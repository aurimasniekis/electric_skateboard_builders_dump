# Why is there a extra balance wire?

### Replies: 17 Views: 363

## \#1 Posted by: Gabegds2001 Posted at: 2018-11-03T18:45:39.569Z Reads: 139

```
Why is there an extra balance wire? I'm a little confused because the bms diagram only shows 12 of the 13 wires used. ![IMG_20181103_133910|374x500](upload://sGjwHKg9cSzEhVsmtnzPEd6rjoi.jpeg)
```

---
## \#2 Posted by: Fiori Posted at: 2018-11-03T18:55:47.108Z Reads: 132

```
12s BMS will have 13 wires. The extra is usually for the power or ground. Need a better photos of that diagram.
```

---
## \#3 Posted by: Trdolan03 Posted at: 2018-11-03T19:04:16.739Z Reads: 125

```
Look at the bottom where the wires come out. It will likely say b- b1 b2 .... the b- goes to the battery neg or vice versa
```

---
## \#4 Posted by: Gabegds2001 Posted at: 2018-11-03T19:06:36.686Z Reads: 121

```
It does say b- thanks
```

---
## \#5 Posted by: Andy87 Posted at: 2018-11-03T20:35:20.439Z Reads: 107

```
You see on the diagram that the first pin is left open, right?
If yes, check with a multimeter if the first pin is connected with the B- Termin on the pcb (should be 0ohm)
If yes, just forget about the first lead of the white cables. Isolation it and you good to go.
```

---
## \#6 Posted by: Gabegds2001 Posted at: 2018-11-03T21:54:28.128Z Reads: 89

```
![15412819755611257198557|375x500](upload://sa1BlSZ3OkvBhM4ID2rfrS651Km.jpeg) If I don't want to use this e-switch on the bms(the two wires on the right) do I just wire them together? I want to just use a loop key on the batteries.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-11-03T22:02:37.494Z Reads: 78

```
How come that’s usually the opposite of what people want to do
```

---
## \#8 Posted by: Gabegds2001 Posted at: 2018-11-03T22:05:22.908Z Reads: 78

```
I mean I can use it... I have a generic on/off switch but I was afraid bumps on the road would switch it off.
```

---
## \#9 Posted by: pat.speed Posted at: 2018-11-03T23:28:23.633Z Reads: 72

```
Nope, very unlikely bumps will switch it off. If you don’t want to you it you can wire it together and the bms will always be open, although I’m not sure if that will add some power draw and may drain the battery over time.

Personally I would just use the button
```

---
## \#10 Posted by: Gabegds2001 Posted at: 2018-11-04T00:54:22.424Z Reads: 56

```
It's more of a light switch with a huge lever rather than a button
```

---
## \#11 Posted by: pat.speed Posted at: 2018-11-04T01:03:05.751Z Reads: 55

```
oh, I thought the bms came with a switch already attached. I would buy a new button switch like most people here use. They cost about $3 on ebay
```

---
## \#12 Posted by: Gabegds2001 Posted at: 2018-11-04T01:04:44.520Z Reads: 53

```
No it just had two wires haha.. I guess you don't get any goodies when you pay 50 dollars for a bms
```

---
## \#13 Posted by: longboardshort Posted at: 2018-11-04T02:17:35.368Z Reads: 50

```
What was the conclusion? The extra wire is indeed b-, verified w/ multimeter too. So is the correct thing to omit the first b- wire in the harness and only connect the b- pad on top to the battery negative, or (I think this is the case) it doesn't matter if that first wire harness b- connection connects to the first batterys gnd balance wire?
```

---
## \#14 Posted by: Friskies Posted at: 2018-11-04T02:37:08.236Z Reads: 46

```
I have the same BMS and contacted the manufacturer about the extra wire. It's not needed, don't wire it - this is the first wire before B1. As for the switch wires I would use them as your switch. Just keep in mind when charging with this BMS that you need to have it turned on to charge.
```

---
## \#15 Posted by: Gabegds2001 Posted at: 2018-11-04T03:13:42.494Z Reads: 39

```
Ok thanks guys
```

---
## \#16 Posted by: pat.speed Posted at: 2018-11-04T04:08:28.755Z Reads: 39

```
you can always wire it if you want, its probably easier than cutting it off and insulating the connection
```

---
## \#17 Posted by: Friskies Posted at: 2018-11-04T10:11:46.783Z Reads: 25

```
You could even pull the pin out completely without much hassle. In saying that I just insulated mine and let it live its life.
```

---
