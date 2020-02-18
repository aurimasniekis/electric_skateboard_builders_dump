# VESC usb port not working

### Replies: 15 Views: 2048

## \#1 Posted by: nick.schweng Posted at: 2016-08-28T23:20:26.230Z Reads: 190

```
I'm doing a dual motor setup and one of my VESCs won't connect to my computer. I'm trying to connect them via canbus and while the first VESC connects to my computer fine, this one won't register when I try to connect it to my computer. What should I do?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-08-28T23:29:23.022Z Reads: 189

```
wich VESC does you have ? Also, do you any picture of the one who is not working properly, and does the blue light go on  when you apply tension to the board
```

---
## \#3 Posted by: nick.schweng Posted at: 2016-08-28T23:37:16.510Z Reads: 187

```
It's from Enertion. It's version 4.12. I'm not sure what you mean by tension, but the blue light does come on when the battery is attached to it. 

https://imgur.com/a/UAkyt
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-08-28T23:43:42.500Z Reads: 175

```
I mean the battery, Also is the red light blinking 3 time (not more), when you put the battery?
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-08-28T23:47:13.900Z Reads: 172

```
Can you also, look under the red wire, near the connector to see if there puncture Hole.
```

---
## \#6 Posted by: nick.schweng Posted at: 2016-08-28T23:53:24.470Z Reads: 169

```
The light just goes solid blue when its plugged in. 
I didn't see any puncture, but I'll upload a photo and you can let me see if you see one. 

https://imgur.com/a/lBBRB
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-08-29T00:12:30.384Z Reads: 163

```
You are suppose to see A red led blinking, if don't see one you are probably missing the bootloader... And won't be able to connect the vesc with the usb
```

---
## \#8 Posted by: nick.schweng Posted at: 2016-08-29T00:13:41.750Z Reads: 156

```
Is there any other way that I can connect my VESC or do I need to order a new one?
```

---
## \#9 Posted by: nick.schweng Posted at: 2016-08-29T00:31:06.823Z Reads: 155

```
This Vesc has connected to my computer before. It just isn't connecting anymore.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-08-29T01:14:25.295Z Reads: 153

```
Theres 2 lights on the vesc, one which turns blue, which means the vesc has enough power to turn on. The other light should blink red three times when you turn it on and turn green. This signifies the vesc has no error codes and is ready to go. If it continues blinking red, you have an error code.
```

---
## \#11 Posted by: onloop Posted at: 2016-08-29T01:40:51.809Z Reads: 146

```
a few things,

1. you can load images directly onto this forum
2. you are likely to short your vesc out if you don't have it insulated, specifically those pins that are pointing to the capacitor board.


also check this out: 

http://www.electric-skateboard.builders/t/vesc-faq-my-vesc-doesnt-work-help-qiqo/672
```

---
## \#12 Posted by: nick.schweng Posted at: 2016-08-29T02:46:33.444Z Reads: 130

```
Is there any way that I can tell which error code it is?
```

---
## \#13 Posted by: evoheyax Posted at: 2016-08-29T02:49:45.922Z Reads: 129

```
Id you can connect the usb to the bldc program, yes. Once connected, go to the data tab and click activate sampling, and the line fault code will say none is there's no fault code or the fault code.
```

---
## \#14 Posted by: Dredoggz Posted at: 2018-03-25T14:10:01.258Z Reads: 67

```
I have the same problem. It connected the first time. Now its just a solid blue light when powered up. Is it fried?
```

---
## \#15 Posted by: Dredoggz Posted at: 2018-03-25T16:05:02.063Z Reads: 61

```
I have the same problem. I just examined my vesc more thoroughly. This is what i found. ![20180325_113808|666x500](upload://pKQAeQ1oYZc5pZbyNft4juKg6lV.jpg)
It shorted out from the pins peircing the positive wire. Lesson learned.
```

---
