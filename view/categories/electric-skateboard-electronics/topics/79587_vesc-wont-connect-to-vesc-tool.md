# VESC wont connect to VESC tool

### Replies: 19 Views: 896

## \#1 Posted by: wolfgangcole Posted at: 2019-01-02T02:13:08.877Z Reads: 137

```
I have a Ollin Vesc that I have used before without issue, but when I went to reconfigure the settings, it wont stay connected and then wont connect at all after it disconnects. I got this:
![vescoof|690x103](upload://2cvPvGncDYBin3ELrCshlzChhoI.png) 
I updated my VESC tool with no luck. I am on a windows computer. What could be causing this, and how do I fix it?
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-02T05:17:41.375Z Reads: 123

```
Change the cable, check if everything is plugged in correctly and the port is not damaged.
```

---
## \#3 Posted by: wolfgangcole Posted at: 2019-01-02T15:52:42.626Z Reads: 109

```
I tried multiple cables, and there is no visible damage to the port,
```

---
## \#4 Posted by: Andy87 Posted at: 2019-01-02T15:56:31.273Z Reads: 105

```
I know you said you checked the drivers, but maybe non the less give this a try
https://www.electric-skateboard.builders/t/driver-issues-with-vesc6-chibios-rt-virtual-com-port-driver-fixed/61769?u=andy87
```

---
## \#5 Posted by: wolfgangcole Posted at: 2019-01-10T22:13:34.945Z Reads: 89

```
tried this on two separate VESCs having this issue with no luck.
```

---
## \#6 Posted by: Andy87 Posted at: 2019-01-11T03:44:22.740Z Reads: 81

```
Did you try a different computer?
```

---
## \#7 Posted by: wolfgangcole Posted at: 2019-01-11T04:12:53.123Z Reads: 79

```
tried three different computers with multiple cables and made sure everything was up to date. No luck with an Ollin or a Tb vesc
```

---
## \#8 Posted by: briman05 Posted at: 2019-01-11T04:16:58.713Z Reads: 74

```
Maybe contact ollin about it just to see if they have any idea why.
```

---
## \#9 Posted by: Gamer43 Posted at: 2019-01-11T04:30:17.509Z Reads: 74

```
Does the blue led light up?

If so, maybe the firmware is corrupted or bricked by some other means. 

Do the computers recognize the VESCs are USB devices?
```

---
## \#10 Posted by: wolfgangcole Posted at: 2019-01-11T04:39:55.865Z Reads: 73

```
not from what I can’t tell; I just updated the firmware. yea it lights up and the computer does not make a sound when t is piggies in or taken out, so ig not
```

---
## \#11 Posted by: Gamer43 Posted at: 2019-01-11T04:44:19.575Z Reads: 71

```
Does the green or red led light up as well?

Have you tried wiggling the connector around in the mini-usb port? On some of mine, the contacts have worn 
out and I have to shift the connector around a bit for the connections to make contact.
```

---
## \#12 Posted by: Andy87 Posted at: 2019-01-11T04:44:32.114Z Reads: 69

```
Wait you updated the fw?
Which file you choose? Could it be you uploaded the wrong fw?
```

---
## \#13 Posted by: wolfgangcole Posted at: 2019-01-11T04:48:06.622Z Reads: 68

```
@Gamer43 I’ll check on those lights later or tomorrow and yea I’ve tried wiggling it around
@Andy87 I update through the vesc tool and ik I chose the proper fw
```

---
## \#14 Posted by: Andy87 Posted at: 2019-01-11T04:49:40.234Z Reads: 65

```
But how you updated firmware if you can’t connect?
Does it mean before the update you could connect?
```

---
## \#15 Posted by: Gamer43 Posted at: 2019-01-11T04:51:58.829Z Reads: 63

```
VESC tool doesn't actually update firmware sometimes.

To ensure the correct firmware is on the VESC, you need an St-link and the appropriate connector. 
There should be videos online on how to do it. St-link clone is 6 dollars off ebay, or a proper one is $10 from Digikey or Arrow if you buy a nucleo board (st-link is embedded in the nucleo board, needs to be a nucleo-64 or nucleo-144 board)
```

---
## \#16 Posted by: wolfgangcole Posted at: 2019-01-11T12:44:25.408Z Reads: 61

```
the vesc would connect and disconnect if I tried to program it
```

---
## \#17 Posted by: Andy87 Posted at: 2019-01-11T12:47:08.089Z Reads: 60

```
still don´t get it.
so you had a solid connection first.
than you updated the vesc and now you can´t connect anymore?
or 
you had a bad connection and with that bad connection you made a fw update?
```

---
## \#18 Posted by: briman05 Posted at: 2019-01-11T13:49:11.397Z Reads: 55

```
Have you written to it and set up the board to ride? That is how I took it was that you had set it up first then were going back to make adjustments.  What firmware did you load from which hardware bin
```

---
## \#19 Posted by: wolfgangcole Posted at: 2019-01-11T17:23:27.246Z Reads: 48

```
@Andy87 The connection was shotty, but it would reliably connect to the vesc tool. It would get kicked if I tried to do a motor detection. I only updated one of the vescs, as the other was up to date. Both vescs had this same level of connection.
@briman05 I hadnt been using one of them and the other I got with about 20 miles on it, and was using it for a small single build im working on. Not sure about the firmware, its just the newest version from the vesc tool from vescproject.
```

---
