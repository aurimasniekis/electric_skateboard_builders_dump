# Vesc DRV Pins Misaligned - Causing Faults?

### Replies: 23 Views: 1907

## \#1 Posted by: Pantologist Posted at: 2016-09-22T21:44:38.273Z Reads: 130

```
<img src="/uploads/db1493/original/3X/c/8/c8bf57fca223cca90b1267792f694f46fc6a1279.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/9/7/9751367e0c9e4b692171abd43c3a7e2a9874b3c4.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/5/1/51be5f3313aa3f33403c416e810ff097b678da94.jpg" width="281" height="500">
The DRV chip on this Vesc seems to be misaligned a bit and it seems to cause the FAULT_CODE_DRV8302 and ABS OVER CURRENT error codes. Also, if my eyes aren't playing tricks on me, it appears that some pins are bridged.

Would this internally damage the drv chip? Should I just replaced it or realign the pins? I've got the proper equipment(rework station, flux).
```

---
## \#2 Posted by: chinzw Posted at: 2016-09-22T22:21:02.696Z Reads: 117

```
Realign it, the 2 bridges i think its normal (i've seen it on other VESCS). Then just try it again.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-09-22T22:39:50.257Z Reads: 116

```
Before trying to realign it, I highly suggest to look under it to see if the Ground pad is correctly solder, because the soldering job look pretty weak.
```

---
## \#4 Posted by: Pantologist Posted at: 2016-09-22T23:20:40.922Z Reads: 110

```
Yeah I was thinking about that too. The pad looks to be making contact, might be a little higher than usual since the pins are not fully flat on the pcb trace.
```

---
## \#5 Posted by: Pantologist Posted at: 2016-09-22T23:33:14.106Z Reads: 106

```
Can anyone confirm this? I find that hard to believe. 

@chaka
@torqueboards
```

---
## \#6 Posted by: chinzw Posted at: 2016-09-22T23:38:27.939Z Reads: 101

```
I think you're right, this is from benjamin's website:

http://vedder.se/wp-content/uploads/2015/01/PCB_Front.png
```

---
## \#7 Posted by: Pantologist Posted at: 2016-09-22T23:39:53.104Z Reads: 95

```
Yeah no bridges. This board almost looks as if the solder joints were not hot enough when soldered. They are all dull.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-09-22T23:43:47.797Z Reads: 91

```
The two bridge are normal... at pad 53-54 and 51-50
```

---
## \#9 Posted by: Pantologist Posted at: 2016-09-22T23:45:04.465Z Reads: 91

```
Any idea why Vedder's picture doesn't have em?
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-09-22T23:52:50.957Z Reads: 91

```
It depend on the mask of the PCB.
```

---
## \#11 Posted by: Carvin_Ginger Posted at: 2016-09-22T23:53:58.673Z Reads: 91

```
This is a stock @torqueboards No Warranty VESC.  Buyers beware.
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2016-09-22T23:55:59.966Z Reads: 89

```
You can clearly see them on this blank PCB

<img src="/uploads/db1493/original/3X/1/a/1a75b9c74129ef56d996aa301b14b118fbe1ec14.jpg" width="375" height="500">
```

---
## \#13 Posted by: Pantologist Posted at: 2016-09-22T23:57:16.131Z Reads: 85

```
Ah okay. Gotcha.
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2016-09-22T23:57:23.234Z Reads: 86

```
Please don't make bad publicity on other Topic, because you didn't read the term and condition before buying something...

It is not nice to do something like that for someone who try to do is best... @torqueboards
```

---
## \#15 Posted by: chaka Posted at: 2016-09-23T00:29:06.359Z Reads: 86

```
What voltage have you supplied to the vesc? If you reflow  the DRV chip it could still be operational. Takes a steady hand.
```

---
## \#16 Posted by: Pantologist Posted at: 2016-09-23T00:34:07.262Z Reads: 85

```
It was tested using 8S Lipos(30v). 

Depending on @torqueboards response, I'll reflow the chip and test again.
```

---
## \#17 Posted by: zmoney Posted at: 2016-09-23T01:15:07.283Z Reads: 80

```
Use a heat gun to nudge the DRV a bit.
```

---
## \#18 Posted by: Pantologist Posted at: 2016-09-23T01:19:00.852Z Reads: 80

```
I've got the reflow equipment. I'll do just that. I just don't want to modify anything in case TB does a replacement.
```

---
## \#19 Posted by: zmoney Posted at: 2016-09-23T01:19:31.958Z Reads: 80

```
I hear you. Best to talk with your vendor first.
```

---
## \#20 Posted by: torqueboards Posted at: 2016-09-23T02:46:38.838Z Reads: 79

```
Yeah, sure. Send it in.
```

---
## \#23 Posted by: treenutter Posted at: 2016-09-26T17:05:08.023Z Reads: 52

```
@Pantologist Dexter is @torqueboards so he's giving you a replacement it sounds like :thumbsup:
```

---
## \#25 Posted by: chinzw Posted at: 2016-09-27T01:35:27.005Z Reads: 45

```
You can talk to him through the chat on diyes website, he's always online.
```

---
## \#26 Posted by: torqueboards Posted at: 2016-09-27T02:56:03.688Z Reads: 45

```
Hey @Pantologist. PM'ed you.
```

---
