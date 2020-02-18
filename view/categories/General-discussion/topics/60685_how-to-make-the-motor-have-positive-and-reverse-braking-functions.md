# How to make the motor have positive and reverse braking functions?

### Replies: 14 Views: 858

## \#1 Posted by: Wentworth Posted at: 2018-07-02T09:07:02.474Z Reads: 165

```
I see a lot of remote controls that have the function of turning and braking, and can also make a reversal function through key buttons. I'm curious about how he uses a receiver to control the function. The premise of doing this is PPM control instead of NRF control mode. Can anyone tell me how to realize this function?
```

---
## \#2 Posted by: Wentworth Posted at: 2018-07-02T09:48:27.498Z Reads: 156

```
It seems to be controlled by serial port. What data is written to the serial port? I think they all use the serial port, as long as there are positive and reverse functions.
```

---
## \#3 Posted by: Wentworth Posted at: 2018-07-02T11:39:38.541Z Reads: 142

```
Can anyone tell me how to do it?I just need a little hint.
```

---
## \#4 Posted by: Holyman92 Posted at: 2018-07-02T12:25:35.433Z Reads: 134

```
u mean you want to know how to gain the reverse ability with a PPM remote?
```

---
## \#5 Posted by: Holyman92 Posted at: 2018-07-02T12:28:03.611Z Reads: 130

```
if so... all u need is ACKMANIACS firmware and boom presto change-o u have reverse
```

---
## \#6 Posted by: Wentworth Posted at: 2018-07-03T01:15:10.204Z Reads: 106

```
I use VESC, as if you know very well, but I can't understand you. Can you provide more information? I haven't been in contact with this thing before.
```

---
## \#7 Posted by: Wentworth Posted at: 2018-07-03T01:33:00.794Z Reads: 102

```
Just checked it on GitHub. Is ACKMANIACS firmware the firmware of Benjamin?

Well, this Benjamin's vesc I bought should have this, but boom Presto change-o I still don't know what this is
```

---
## \#8 Posted by: abenny Posted at: 2018-07-03T02:41:25.806Z Reads: 95

```
start reading :grin:
https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---
## \#9 Posted by: Wentworth Posted at: 2018-07-04T02:31:50.884Z Reads: 75

```
After reading it, I still don't know how to do it, so that I can design a remote controller with buttons to realize forward and reverse and brakes. Am I too stupid?
```

---
## \#10 Posted by: abenny Posted at: 2018-07-04T02:37:36.527Z Reads: 67

```
download ackmaniac esc tool, update ypur firmware with it, and in input setup there should be some setting that allows your to set up reverse...thats as far as i can guide you since i haven't done this myself
```

---
## \#11 Posted by: wafflejock Posted at: 2018-07-04T02:43:06.863Z Reads: 64

```
The regular firmware has a reverse option as well but no safety built in on that really so it might be better to use ackmaniac firmware and verision of the vesc tool.  In the ppm config you can choose "current control no reverse with brake" or just "current control" if you want reverse.  This doesn't work through a switch or button though it just uses the bottom half of the the ppm range to count as reverse once the motor has come to a stop (ackmaniac added some bits so you have to hit brake after coming to a stop basically to kick it into reverse so you don't accidentally reverse the board out from under yourself when trying to just brake).  To have the reverse only active through a button or switch believe you'd need to tap into the serial/uart from the receiver which basically means making a custom receiver.
```

---
## \#13 Posted by: Wentworth Posted at: 2018-07-04T03:35:21.393Z Reads: 54

```
I didn't try it, because I wanted to write the data to the serial port to realize the function of positive rotation and inversion. If it can not be realized, I will consider this method again.
```

---
## \#14 Posted by: Wentworth Posted at: 2018-07-04T03:36:56.462Z Reads: 53

```
Yes, I just want to customize it myself, but I don't have any information about it. I would like to write data to the serial port to achieve positive and reverse, but there is no specific way. Do you have the relevant information?
Thank you for your reply
```

---
## \#15 Posted by: wafflejock Posted at: 2018-07-04T03:37:25.607Z Reads: 49

```
http://vedder.se/2015/10/communicating-with-the-vesc-using-uart/

Vedder provides code and some explanation there but will still require you to know how to make your own receiver can also Google for VESC UART github to find some repos.
```

---
