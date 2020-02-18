# Battery/Voltage Meter Location on Build

### Replies: 18 Views: 847

## \#1 Posted by: flywithgriff Posted at: 2017-08-05T04:23:00.635Z Reads: 118

```
I have heard and read several different opinions on where to place the meter on my build. I will have two enclosure about 14" apart. One will contain the Batteries, BMS, and Charging port while the other will contain the two FOCBOX. I would like to place the Meter in the Battery box as it will be between my feet and easier to see but I would like to know what be best. I have already had one of these burn out and would like to avoid this issue on this build.
```

---
## \#2 Posted by: mmaner Posted at: 2017-08-05T04:27:38.769Z Reads: 117

```
I've started putting them between my feet, it's the easiest place to see.  Get the drok dc8 and you won't have any doa's.
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-08-05T04:31:54.549Z Reads: 112

```
Cool deal! I like this idea because I can pull the loop key so they FOCBOX are not powered while charging but still see the voltage percentage on the meter.
```

---
## \#4 Posted by: mmaner Posted at: 2017-08-05T04:47:35.789Z Reads: 107

```
Good engineering.
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-08-05T04:49:04.659Z Reads: 102

```
I have put quite a bit of thought into this build and so far it is coming out well. Pm me the pics of your 10x 2s lipo build.
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-05T05:08:43.696Z Reads: 99

```
when you solder the leads, make sure they're as close as possible (electrically, not physically). I burned 2 Drok's because my leads were too far apart.
```

---
## \#7 Posted by: Jammeslu Posted at: 2017-08-06T13:20:54.578Z Reads: 72

```
What do you mean?
```

---
## \#8 Posted by: Jinra Posted at: 2017-08-06T18:55:55.383Z Reads: 66

```
Solder them so there is the least electrical distance for current to travel from pos to neg. I had my negative on the XT60 after my switch and the positive on my battery positive. It worked, but under heavy load, it burnt out my meter. I now have both on my XT60 and everything's been great.
```

---
## \#9 Posted by: Jammeslu Posted at: 2017-08-07T12:02:29.098Z Reads: 52

```
[Uploading...]() 

Could you take a look and maybe give suggestions then Where to put it, Sry for bad pic
```

---
## \#10 Posted by: Jammeslu Posted at: 2017-08-07T13:00:26.244Z Reads: 50

```
<img src="/uploads/db1493/original/3X/b/0/b06067fa1db364b2a0249a28056d6e1fffe2a8a5.jpg" width="281" height="499">
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-07T14:56:50.025Z Reads: 45

```
Sorry i cant really tell from the pic, do you have a diagram?
```

---
## \#12 Posted by: Jammeslu Posted at: 2017-08-07T15:30:22.568Z Reads: 42

```
Pos is just after xt60 loop key and neg is between Vesc and bms
```

---
## \#13 Posted by: Jinra Posted at: 2017-08-07T15:33:53.885Z Reads: 40

```
I still can't really tell, but I would just put it on the +/- where the VESC connects to the battery.
```

---
## \#14 Posted by: Bloop Posted at: 2017-08-07T15:39:04.072Z Reads: 38

```
@Jinra i have it connected negative wire the goes into vesc and on positive from keyloop again just before the vesc . should be fine right ?
```

---
## \#15 Posted by: Jinra Posted at: 2017-08-07T15:40:47.397Z Reads: 37

```
Probably. I think a lot of people have it hooked up like that. I don't know how much distance will cause it to burn up exactly. Mine was about 20 cm apart, electrically.
```

---
## \#16 Posted by: SilentException Posted at: 2017-08-07T15:42:56.453Z Reads: 36

```
Is there any explanation on why does it burn? Is it the same wire inductance problem as too long wires from battery to ESC? Put a cap on the meter then, should help a bit :)
```

---
## \#17 Posted by: Bloop Posted at: 2017-08-07T15:43:17.443Z Reads: 39

```
Well if anything i will report back. so far is working just fine for me
```

---
## \#18 Posted by: Jinra Posted at: 2017-08-07T15:44:32.634Z Reads: 36

```
Easier to just hook it up correctly. I think it may be something with inductance though. When it burned, my meter shared the same 12 awg line as main power from battery to ESC.
```

---
