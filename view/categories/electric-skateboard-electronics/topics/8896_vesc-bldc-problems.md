# VESC BLDC problems

### Replies: 5 Views: 636

## \#1 Posted by: boardthebuilder Posted at: 2016-09-04T14:46:18.662Z Reads: 118

```
I have seen similar posts to what I am currently going through. but nothing really exactly the same.

My setup is:
x2 Torqueboards 230kv
x2 VESC 4.12
x2 zippy 8000 3s 1P 30C (series)
quantum 2.4ghz transmitter reciever

I recently just got both my VESCs connected to BLDC tool 2.17-2.18. I read the configuration and tested to see if the motors would spin. the arrow keys worked perfectly but for only one of the VESCs. I tried the other one and the motor was all jumpy, stuttery and didn't spin properly. So I went back to the working VESC.
I had already watched @jacobbloy 's videos, so i started to change the battery voltage limits.
When I clicked 'write configuration' the VESC started flashing pink LED. I tried again with the other VESC and the same thing happened. I read some more forums and many people said to re-flash the firmware. I reflashed 2.18. This stopped the original working VESC from flashing pink but not the other VESC.

Next was to see if the motor detection test would work... NOPE. 'Bad Detection Result Received'. There are "No faults registered since startup" and i dont know what else to do.

As for the VESC that is still flashing pink. It connects but I cannot reflash the 2.18 firmware it says "buffer erase timeout". 

it was all going so well about 30 minutes ago. And then it all turned to S#!T. I'm open to ideas!
```

---
## \#2 Posted by: elkick Posted at: 2016-09-04T15:09:25.720Z Reads: 114

```
Is this a VESC from  scramboards (Maytech)? There are several people reporting exactly those problems lately.
```

---
## \#3 Posted by: mason Posted at: 2016-09-04T15:15:27.144Z Reads: 110

```
Scramboards isn't selling Maytech VESCS.
```

---
## \#4 Posted by: elkick Posted at: 2016-09-04T15:25:41.554Z Reads: 102

```
Got that info from a scramboards customer who received his VESCs directly from China. But that's not important anyway.

It seems that there are some more VESCs having exactly the same problem, might be that uploading bootloader with STlink is required.
```

---
## \#5 Posted by: boardthebuilder Posted at: 2016-09-04T16:08:42.724Z Reads: 91

```
I bought it from
```

---
