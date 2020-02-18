# Dual FOCBoxes using remote Splitter

### Replies: 12 Views: 669

## \#1 Posted by: GJHS Posted at: 2018-02-19T05:19:30.648Z Reads: 151

```
Hey Guys.  I have my FOCBoxes connected using a remote (Nano-X) splitter.  When I configure each using BLDC, do I configure them the same?  Does Master or Slave apply?
```

---
## \#2 Posted by: High-roller Posted at: 2018-02-19T05:25:16.288Z Reads: 151

```
If you're using a splitter, that is, a Y-cable to connect them via the reciever, you don't need to designate master/slave, they're both masters. You configure them both exactly the same.
What you're talking about only applies if you're using a canbus cable.
In any case, test each motor separately. Don't just copy and paste!
```

---
## \#3 Posted by: GJHS Posted at: 2018-02-19T05:26:34.818Z Reads: 147

```
Thanks @High-roller, I thought so.  Only difference would be the one with the Bluetooth module or is that the same as well?
```

---
## \#4 Posted by: High-roller Posted at: 2018-02-19T05:28:09.214Z Reads: 143

```
I'm not sure, I've never used Bluetooth modules. This is for telemetry, right?
```

---
## \#5 Posted by: GJHS Posted at: 2018-02-19T05:32:50.326Z Reads: 131

```
Yes, I have read on the FOCBox with the Bluetooth make sure ppm+uart is enabled and set baud rate to 9600
```

---
## \#6 Posted by: pennyboard Posted at: 2018-02-19T06:24:29.531Z Reads: 126

```
Make sure you only have the red wire (5 volt supply) connected to one of the VESC’s or you risk killing one of your VESC’s. 

So all 3 wires into 1 VESC and only white and Black into the other.
```

---
## \#7 Posted by: High-roller Posted at: 2018-02-19T06:35:19.016Z Reads: 113

```
Woah, thanks for catching that, I completely forgot to mention it!
```

---
## \#8 Posted by: Jammeslu Posted at: 2018-02-19T09:02:35.224Z Reads: 103

```
Is ground still neccesery for the other focbox with a cut 5v?
```

---
## \#9 Posted by: pennyboard Posted at: 2018-02-19T09:58:00.807Z Reads: 95

```
Yes. The FOCbox will need something, a reference point, to compare the signal coming through the white wire to. That is what the ground is.
```

---
## \#10 Posted by: rojitor Posted at: 2018-02-19T23:06:25.756Z Reads: 70

```
[https://youtu.be/F70Kr9w4sj0](https://youtu.be/F70Kr9w4sj0)
```

---
## \#11 Posted by: GJHS Posted at: 2018-02-20T02:43:02.885Z Reads: 60

```
Is anyone using 2 receivers vs a Y splitter?
```

---
## \#12 Posted by: bigben Posted at: 2018-02-20T06:39:31.831Z Reads: 51

```
Yes.  Works like a charm. Bigboystoys ran his 4x4 boards like this. 
Just pair the remote with both receivers separately.
```

---
