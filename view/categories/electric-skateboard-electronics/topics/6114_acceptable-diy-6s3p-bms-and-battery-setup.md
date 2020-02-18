# Acceptable DIY 6S3P BMS and battery setup?

### Replies: 17 Views: 3320

## \#1 Posted by: theviith Posted at: 2016-07-14T20:52:57.376Z Reads: 179

```
Hey guys, so I am planning to make a 6S3P battery and BMS pack but was wondering if any battery wiz out there could verify the setup with me so that I don't blow myself up trying to make the pack, or much less ruin expensive electronic equipment. I have attached the diagram in this post. Any help would be very much appreciated!
<img src="/uploads/db1493/original/2X/1/190c03d8cc2d64b85cf002205c9d553b463a0bf4.jpg" width="690" height="388">
```

---
## \#2 Posted by: rubz Posted at: 2016-07-14T21:53:18.358Z Reads: 162

```
I'm assuming this is the BMS schema:

<img src="/uploads/db1493/original/2X/d/d70dd99eb8f254c17b0ca160bdba9b8890831028.jpeg" width="690" height="406">

Your drawing is perfect. B- connects to the BMS via mains and the other wires via balance wires. Make sure you get a 6-pin JST-XH connector (those are meant for 5S) and not one made for 6S batteries.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-07-15T02:21:09.637Z Reads: 144

```
Seem Legit :sunglasses: But don't forget to put a fuses before your switch, so in case of a problem you won't burn your esc.
```

---
## \#4 Posted by: theviith Posted at: 2016-07-15T05:00:13.996Z Reads: 140

```
@rubz yeah I basically followed that diagram but just added the cells in parallel

@JohnnyMeduse thanks for the heads up. Do you know if it matters where I put the fuse? as in which polarity to put the in-line fuse on? 

Also, does it matter what polarity I put the 2-12S toggle switch on? I've heard that it is best to put it on the positive side of the circuit but there hasn't been any proof why that is.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-07-15T05:07:00.174Z Reads: 141

```
I think this is better on your positive side, because the battery is directly connect to all your electronics, on the negative side de BMS should act as a buffer for the current (good BMS are suppose to protect your circuit). And for the switch it really depend on the BMS you use.
```

---
## \#6 Posted by: theviith Posted at: 2016-07-23T23:24:20.059Z Reads: 126

```
so I've finished making the battery pack and wired the 2-14S toggle switch from Dexter, as shown in the picture. But now I run into a bit of a problem when trying to connect the voltmeter. When the voltmeter is wired (pos to pos; neg. to neg.), the reading shows a constant 100% no matter the battery state...even when it is drawing amps out of the pack. Does anyone know what I am doing wrong? Does it need be wired directly to the BMS instead of from the toggle switch?

thanks in advance<img src="/uploads/db1493/original/2X/a/aa22850f5a1b758b410810decab5487dec288df9.jpg" width="690" height="388">
```

---
## \#7 Posted by: lox897 Posted at: 2016-07-23T23:39:37.877Z Reads: 119

```
You would wire it between the switch and the ESC.
```

---
## \#8 Posted by: theviith Posted at: 2016-07-23T23:52:50.318Z Reads: 116

```
hm I tried that but the reading just stayed at a constant 100%. I measured the pack's voltage and its at 21.8 which is nowhere near its capacity for 6S if I'm not mistaken
```

---
## \#9 Posted by: lox897 Posted at: 2016-07-24T00:05:54.247Z Reads: 111

```
That is near 6S. Did you have the power switch on when it was %100?
```

---
## \#10 Posted by: lox897 Posted at: 2016-07-24T00:06:20.983Z Reads: 107

```
Can you show me a picture of the voltage meter itself?
```

---
## \#11 Posted by: Jinra Posted at: 2016-07-24T00:10:57.241Z Reads: 102

```
I bet the voltmeter is configured on the wrong S count
```

---
## \#12 Posted by: theviith Posted at: 2016-07-24T00:21:51.007Z Reads: 102

```
<img src="/uploads/db1493/original/2X/c/c082e101bf4d7a3e8ca2478369f4f3a474a80a47.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/d/d3dc8de157b9e06a279561d135992364d9315abc.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/4/414603a3b93d5444c099ccafa8395be6ef6ebf48.jpg" width="690" height="388">
```

---
## \#13 Posted by: theviith Posted at: 2016-07-24T00:26:57.356Z Reads: 97

```
pressing that little button on the back of the voltmeter also did nothing...soo not sure what the problem is here
```

---
## \#14 Posted by: Jinra Posted at: 2016-07-24T01:28:20.928Z Reads: 93

```
Have you ever configured the voltmeter? You should be able to scroll through the S count with the button. Check the instructions that came with it, or try holding or double tapping the button. It might be on a default 3s setting or something.
```

---
## \#15 Posted by: theviith Posted at: 2016-07-24T03:36:58.004Z Reads: 92

```
it never came with any instructions..bought it somewhat cheap from ebay lol. but yea I tried pressing the buttons a couple times but I haven't tried holding or double tapping it so i'll give that a try.
```

---
## \#16 Posted by: mason Posted at: 2016-07-24T04:06:24.927Z Reads: 90

```
press it and hold, then turn on the meter. press the button again to switch types
```

---
## \#17 Posted by: theviith Posted at: 2016-07-24T04:30:16.978Z Reads: 88

```
it worked! Thanks so much @link5505!!!
```

---
