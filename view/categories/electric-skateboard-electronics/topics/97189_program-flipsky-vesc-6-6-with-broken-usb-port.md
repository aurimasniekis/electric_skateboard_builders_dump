# Program Flipsky VESC 6.6 with broken USB port

### Replies: 5 Views: 162

## \#1 Posted by: timheterjag Posted at: 2019-06-23T20:55:58.247Z Reads: 58

```
Hi, 

Got the FESC 6.6 from Flipsky a couple of months ago and finaly got it installed. Went and did the motor setup and noticed that the USB port was very loose, only to have it fail completely the next time i went to plug it in. Contacted Flipsky support but the want me too send it to them in China before replacing it, which isnt really an option since i want to ride this summer.

So, i still need to configure the VESC further. Am i completely screwed or do i have any other options ? Thanks :)
```

---
## \#2 Posted by: Pimousse Posted at: 2019-06-23T21:45:48.208Z Reads: 55

```
Hi,

2 options :
1. Buy a Bluetooth dongle and connect VESC Tool through Bluetooth
2. Connect it to another VESC via CANbus and use CAN Forward communication.
```

---
## \#3 Posted by: Gamer43 Posted at: 2019-06-23T23:15:12.529Z Reads: 47

```
If you are comfortable with a soldering iron (and voiding a warranty), you could either bodge wire a USB connector or solder on a new one. I had to do this for one of mine, was a pain in the ass to get all the solder out of the ground through-hole.
```

---
## \#4 Posted by: timheterjag Posted at: 2019-06-24T22:32:41.760Z Reads: 27

```
I thought id give this a go, but the whole board is pretty much glued in to the case. Some friends are also building a board with the same VESC so i might try can forwarding If all else fails.
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-06-24T22:45:23.058Z Reads: 24

```
Yeah, I had to pry off all the glue, was not fun xD.

Good luck with the CAN forwarding.
```

---
