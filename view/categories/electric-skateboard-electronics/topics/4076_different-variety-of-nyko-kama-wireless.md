# Different variety of Nyko Kama wireless

### Replies: 23 Views: 3476

## \#1 Posted by: hamminitup Posted at: 2016-05-31T21:54:56.051Z Reads: 151

```
Hey guys I just got this nyko Kama wireless that I ordered from eBay, and in the disassembly process I became confused. This version of the kama seems to have a different dongle receiver than the others I have seen. Anyone have experience with these? And if so, how did you wire it to a VESC? I guess Im just wondering what each cable is for.
<img src="/uploads/db1493/original/2X/3/34d7e6f0022a15d84a4e082570abf92710ef1edd.jpg" width="690" height="388">
```

---
## \#2 Posted by: wallaboo Posted at: 2016-05-31T23:59:58.654Z Reads: 132

```
Looks normal to me. I can't see the wires so it's hard to say if they really did change the wire colors... You will just need to get the JST connector and it will connect to the VESC

http://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139
```

---
## \#3 Posted by: hamminitup Posted at: 2016-06-01T00:14:45.370Z Reads: 126

```
Hmm ok. I was confused because the receiver on this one is different than the guide. The wires are also different colors, so I can't tell which wires are for what.
```

---
## \#4 Posted by: lowGuido Posted at: 2016-06-01T01:06:35.300Z Reads: 128

```
[quote="wallaboo, post:2, topic:4076"]
Looks normal to me
[/quote]

its pretty far from normal.


yeah looks like you got one of the odd ones. pre nintendo court case probably. i'm pretty sure the latest ones are the ones that everyone uses. 
there have been a few people on the forum show up with one like yours, but i'm not sure if they worked or not.
```

---
## \#5 Posted by: hamminitup Posted at: 2016-06-01T01:23:17.005Z Reads: 117

```
Thanks for replying @lowGuido. Any idea what the cables represent? That sucks I may have to get a different one
```

---
## \#6 Posted by: lowGuido Posted at: 2016-06-01T01:28:00.278Z Reads: 113

```
you should still be able to use it. just match up the wires.
```

---
## \#7 Posted by: hamminitup Posted at: 2016-06-01T01:29:40.581Z Reads: 113

```
ok. Is there any way to figure out for sure what each wire is for? This version has different colors than the standard. Should I just do trial and error?
```

---
## \#8 Posted by: lowGuido Posted at: 2016-06-01T01:56:57.924Z Reads: 111

```
yeah. there is a diagram. 
props to whoever drew this..
http://www.electric-skateboard.builders/uploads/db1493/original/2X/6/6d09691075d077109f1915f6322bc8b7b6a42605.png
```

---
## \#9 Posted by: hamminitup Posted at: 2016-06-01T01:58:42.224Z Reads: 106

```
OH sweet. thanks so much. lifesaver
```

---
## \#10 Posted by: lowGuido Posted at: 2016-06-01T02:00:04.713Z Reads: 104

```
keep in mind that if you have the latest VESC it has 7 pins, so there will be an unused pin at the bottom as well
```

---
## \#11 Posted by: hamminitup Posted at: 2016-06-01T02:01:42.303Z Reads: 106

```
ok thanks so much @lowGuido
```

---
## \#12 Posted by: sgaana Posted at: 2016-06-01T05:00:51.213Z Reads: 104

```
Some pictures to illustrate:
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/b/be48c58487cc1fc8419d145f2728e69d0d6c2820_1_666x500.jpeg
From @chaka 
<img src="/uploads/db1493/original/2X/e/e949e5c7d72e81d45d716caeb6a73fe1b1cc1f64.png" width="606" height="500">
From @elkick
<img src="/uploads/db1493/original/2X/2/29dfb762425f72df5ef2fa0ccc5ee408733780d4.png" width="589" height="500"> 
Pin 1 Do not use
Pin 2: Green SCL/RX. (closest to motor wires)
Pin 3: Blue SDX/TX
Pin 4: Do not use
Pin 5: Black GND 
Pin 6: Red 3.3v 
Pin 7: Do not use (closest to battery wires)
```

---
## \#13 Posted by: philipp Posted at: 2016-06-01T07:48:00.965Z Reads: 90

```
please tell us if you get this controller to work with the vesc.
This model is way easier and cheaper to get here in switzerland :slight_smile:
```

---
## \#14 Posted by: hamminitup Posted at: 2016-06-01T10:51:52.316Z Reads: 82

```
Ok will do once my VESC comes in. Hopefully a week or so if @torqueboards is still on time
```

---
## \#15 Posted by: trbt555 Posted at: 2016-06-01T15:58:56.036Z Reads: 74

```
[quote="sgaana, post:12, topic:4076"]
Pin 1 Do not usePin 2: Green SCL/RX. (closest to motor wires)Pin 3: Blue SDX/TXPin 4: Do not usePin 5: Black GND Pin 6: Red 3.3v Pin 7: Do not use (closest to battery wires)
[/quote]

I hate that picture. it should be banned.
The pin numbering is exactly the inverse of the numbering in Vedder's diagrams: pin1 (5V) is the farthest from the MOSFETS and pin 7 (ADC2) is closest to the MOSFETS.
```

---
## \#16 Posted by: hamminitup Posted at: 2016-06-01T16:38:03.334Z Reads: 70

```
OK thanks for that info. Glad I didn't screw up anything yet.
```

---
## \#17 Posted by: sgaana Posted at: 2016-06-01T18:30:11.700Z Reads: 70

```
No wonder. I had to insert upside down to work. @trbt555, can you post a correct picture?
```

---
## \#18 Posted by: trbt555 Posted at: 2016-06-01T18:32:42.391Z Reads: 68

```
The connections in the picture are correct. The pin numbers just don't correspond to Vedder's schematics.
```

---
## \#19 Posted by: trbt555 Posted at: 2016-06-01T19:08:06.581Z Reads: 75

```
Here's a quick diagram I made with correct pin numbering:
<img src="/uploads/db1493/original/2X/9/910191d0025582762512bf7de175a8182d795a77.jpeg" width="678" height="500">
```

---
## \#20 Posted by: lowGuido Posted at: 2016-06-01T22:24:28.776Z Reads: 72

```
pin numbers and wire colours aside. all these diagrams assume you have the later model Kama. 
there is 4 (used) wires: power, ground, data and clock. just make sure 

GND goes to GND
3.3v goes to Vcc
Data goes to SDA
Clock goes to SCL

Simples
```

---
## \#21 Posted by: hamminitup Posted at: 2016-06-02T00:33:31.197Z Reads: 65

```
OK thanks. This is what I was looking for lol. The diagrams should help though.
```

---
## \#22 Posted by: boards Posted at: 2016-06-02T05:13:59.283Z Reads: 57

```
AHAHAHHAHA.

Batch 1 still hasn't arrived for anybody (The one supposed to arrive late march), I wouldn't get your hopes up...
```

---
## \#23 Posted by: hamminitup Posted at: 2016-06-02T10:44:16.236Z Reads: 54

```
Oh no. I didn't know this. I just recently talked to @torqueboards and he said that he would be receiving a batch of VESCs in like a week or so.
```

---
