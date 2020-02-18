# VESC BLDC motor detection failed and not showing a fault code. Please Help

### Replies: 15 Views: 1569

## \#1 Posted by: nick.schweng Posted at: 2016-08-26T15:57:23.639Z Reads: 172

```
I'm trying to program my VESC and it's not working. I currently have a 10,000mAh 14.8V 4S battery connected to a VESC that is connected to an Enertion R-Spec motor. 

I tried programming it a couple weeks ago and I and I had no problem 
with the motor detection. But now whenever I try to do a motor 
detection, the motor shakes and jerks and the motor detection fails. I 
went into the Realtime Data tab and it didn't give me an error message 
of any sort. It said No Fault. What's going on with my board?
```

---
## \#2 Posted by: Blasto Posted at: 2016-08-26T16:17:06.360Z Reads: 165

```
Make sure your batteries are charged, your phase connectors are well isolated.
```

---
## \#3 Posted by: nick.schweng Posted at: 2016-08-26T16:27:24.039Z Reads: 164

```
Okay I checked and  the battery is fully charged and the phase connectors are isolated
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-26T16:30:28.852Z Reads: 159

```
What are your battery voltage cutoffs?
```

---
## \#5 Posted by: nick.schweng Posted at: 2016-08-26T16:35:03.486Z Reads: 152

```
My minimum voltage is 8.0 Volts and the maximum voltage is 57 Volts
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-26T16:35:37.775Z Reads: 147

```
Not those, your battery cut off start/end. It's right below those fields.
```

---
## \#7 Posted by: nick.schweng Posted at: 2016-08-26T16:40:22.178Z Reads: 141

```
Start is 30.00 Volts and End is 33.00 Volts
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-26T16:42:20.054Z Reads: 142

```
Change it to 13v start and 12v end and retry detection.

EDIT: make sure you write config before detection.
```

---
## \#9 Posted by: nick.schweng Posted at: 2016-08-26T16:46:26.549Z Reads: 139

```
IT WORKED THANK YOU SO MUCH. 

Would you mind explaining what exactly it was that I changed?
```

---
## \#10 Posted by: Jinra Posted at: 2016-08-26T16:48:41.446Z Reads: 138

```
Since you're detecting on 4s your VESC was already hitting low voltage cut off. You always want cutoffs to be lower than your nominal working voltage. I set mine to start at 3.3v per cell and end at 3.0v per cell, though I would stop riding once the cut off starts.
```

---
## \#11 Posted by: nick.schweng Posted at: 2016-08-26T17:40:40.896Z Reads: 125

```
I'm also having trouble with my VESCs. I'm running a dual motor set up with the two VESCs and the USB port isn't working on one of them. I've tried every port on my laptop. It just doesn't work with the other VESC. Is there anything I can do to fix this?
```

---
## \#12 Posted by: elkick Posted at: 2016-08-26T18:03:42.012Z Reads: 114

```
How did you connect the two VESCs together? If you're using CAN bus, do you only connect the two cables out of four?
```

---
## \#13 Posted by: nick.schweng Posted at: 2016-08-26T18:06:57.317Z Reads: 107

```
Yes. The middle two
```

---
## \#14 Posted by: elkick Posted at: 2016-08-26T18:29:25.916Z Reads: 104

```
That's good, because it only needs one try with 4 cables connected on the CAN bus to create ground loops and it will short the can transceiver causing the 3.3V rail to fail. Result is a non working USB port. 

But the power indication led (blue one) is lit? Did you try other USB cables as well?
```

---
## \#15 Posted by: nick.schweng Posted at: 2016-08-26T18:45:03.437Z Reads: 96

```
The power indication light does come on. And the usb cable I'm using is working with my other VESC. And it's worked with this one before, it just isn't right now.
```

---
