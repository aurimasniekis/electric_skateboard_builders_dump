# VESC Stopped Working.. I think.. Please Help

### Replies: 19 Views: 1838

## \#1 Posted by: deke997 Posted at: 2016-10-21T23:29:54.433Z Reads: 154

```
So I finally got all the parts together that I needed to bench test my board, and everything was working great. My motor was reacting as was expected, until everything stopped working all of a sudden. To give a little context, I have a vesc, a bldc motor, and a DC power supply that I used for testing because I don't have a battery yet. The power supply can output any voltage from 0-31.5V up to 1 Amp (could this be the root of the problem?). My motor is rated for 8-10s so I figured this would be perfect. I cranked the voltage all the way to 31.5, and I mounted the motor on the board, plugged the power supply into the vesc, and plugged the vesc into my computer and the motor. 

Everything was working good. I switched from the default setting for BLDC to FOC (my motor is unsensored). Then, I followed [this](https://www.youtube.com/watch?v=bYYNbxPXNEU) tutorial to configure the FOC settings. It was working great on FOC, and it made much less noise, which was even better. I wanted to show my friend the difference in noise between to two configurations, so I saved my configuration, and I switched back and forth between the default configuration and my new configuration a couple of times. All of a sudden, I heard a loud "click" noise, and my motor stopped turning. The vesc still had a blue light, and the yellowish-greenish light still comes on when I hit the arrow keys on my computer, but the motor doesn't turn.

I can't imagine that the problem is in the motor, although I am definitely not an expert, so please correct me if you think otherwise. The motor still turns fine when I turn it with my hand. Running "faults" in the terminal window returns nothing. On the "Realtime Data" tab, when I turn the motor with my hand, I get the expected results on the Current/Duty and RPM tabs, and the Tacho and Tacho ABS values respond as expected. 

However, when I hit the up arrow on my keyboard while using the default configuration, the ERPM maxes at about 210 and does a weird pattern (see picture). Before, it would go up to around 14,000 and do a kind of jagged line that stayed between 13,000 and 15,000. The motor doesn't even twitch.<img src="/uploads/db1493/original/3X/3/e/3ef8bef4cfdeb92b6003b879a979eeb9f9ba4308.png" width="690" height="387">

When I hit the up arrow on my keyboard while using my saved FOC configuration from when my motor/vesc was working, I get a flat line at about 10,000 ERPM. Before, it was a flat line at 13,000 RPM. The motor doesn't even twitch.<img src="/uploads/db1493/original/3X/6/1/61282c6e17b2d80190c20b8600b52e4bac1aa9b7.png" width="690" height="387">

Also, the Tacho and Tacho ABS values go up when I hit the arrow key, even though the motor is not moving.

Here is a screenshot of the ERPM values when I turn the motor back and forth quickly by hand:
<img src="/uploads/db1493/original/3X/b/0/b096d1f09d1502fdcc53132e5b57e73fef991c40.png" width="690" height="387">

Please help me out here. Is the problem my VESC? Is it my motor? Is it my power supply? Let me know what you think!

BTW, I got my VESC from
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-10-22T00:12:39.063Z Reads: 129

```
have you try to reprogram the VESC...
```

---
## \#3 Posted by: deke997 Posted at: 2016-10-22T00:17:19.074Z Reads: 128

```
I have not. Can you point me in the right direction to figure out how to do that? Do you have nay ideas what may have caused the issue in the first place?
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-10-22T00:22:28.985Z Reads: 124

```
Well, it is not recommend by anyone to switch from FOC to bldc, also there a missing capacitor (witch has been place on version 4.12 for helping with FOC use) on Torqueboards VESC. 

Just go in the Tab Firmware... Then choose the default.bin inside the firmware for 4.10-4.12 folder.... then upload.
```

---
## \#5 Posted by: deke997 Posted at: 2016-10-22T00:29:12.214Z Reads: 121

```
That didn't help at all. It behaves exactly the same. The motor does not respond. Motor detection fails.

Edit: I'm not sure what you mean by the part about the missing capacitor. I have version 4.12.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-10-22T00:30:22.799Z Reads: 116

```
when you does your motor detection does the red led flash

c26 is missing... it a capacitor that had been add for FOC stability and reliability
```

---
## \#7 Posted by: deke997 Posted at: 2016-10-22T00:32:21.784Z Reads: 110

```
No. The greenish-yellowish led comes on for a second, and then the software says "bad detection result received."

Are you saying that my VESC is missing a capacitor? It is the latest VESC.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-10-22T00:34:03.203Z Reads: 109

```
well, it might be the latest pcb, but from the few one I have repair from torqueboard it seem he still use the BOM from 4.10 version.

edit.. can you go in terminal tab and write  FAULTS
```

---
## \#9 Posted by: deke997 Posted at: 2016-10-22T00:37:28.725Z Reads: 106

```
I already did that. I mentioned it in my first post. It returns no errors. How do I tell if this is truly a problem with my VESC and not a problem with my motor? Is it likely that the problem is my motor?
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-10-22T00:39:54.010Z Reads: 103

```
can you try to mesure the resistance in foc, and spin up for Lamda
```

---
## \#11 Posted by: deke997 Posted at: 2016-10-22T00:44:42.192Z Reads: 102

```
Resistance: green led comes on. Then, the software says "port disconnected", and the VESC disconnects from my computer. The motor does nothing.

Lambda: green led comes on. The software says "detection result received". The motor does nothing.
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2016-10-22T00:46:26.433Z Reads: 98

```
hummmm... this look like a VESC problem...
```

---
## \#13 Posted by: deke997 Posted at: 2016-10-22T00:47:09.381Z Reads: 95

```
Should I try to get a replacement from http://?
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2016-10-22T00:50:24.192Z Reads: 94

```
you can always try to contact them about your issue... Are your motor also from DIY
```

---
## \#16 Posted by: deke997 Posted at: 2016-10-22T00:52:55.400Z Reads: 95

```
I will try that. My motor is not from DIY
```

---
## \#17 Posted by: Bender Posted at: 2016-10-22T10:21:52.272Z Reads: 89

```
Easy way to find out if it is the VESC do a reboot and see if you see the red led flash 3 times

I'm having the same issue and am going to replace the Drv chip
I'll let you know if that fixes it
```

---
## \#18 Posted by: deke997 Posted at: 2016-10-25T01:35:41.705Z Reads: 74

```
The red LED does not flash. 

I think 2 of my motor leads may have touched. I don't know for sure though. What would the symptoms of this be on the esc?
```

---
## \#19 Posted by: Jameshagerty Posted at: 2017-01-14T22:24:42.923Z Reads: 51

```
Hey there community! This is my first post! I have an issue with my electric skateboard and wondered if someone could help! I oringally bought a magneto board, I have been using it a couple of months but the breaking has been unreliable! So I bought a brand new VESC (see link below for the one I bought) I wired it all up! Worked perfectly, configured it on my computer and then went out and tested it! After a while I was going along and suddenly bam!! It stopped the wheels stopped, I flew off the board! I'm fine a few cuts and bruises, but I'm just wondering what went wrong!? Any suggestions I would be greatly appreciative! Thanks guys! 

http://r.ebay.com/1xz4R4
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2017-01-15T02:02:38.637Z Reads: 43

```
It's kind of hard to tell, because these VESC as been highly modify by the manufacturer, and there hundred of reason that can explain this kind of failure.... Maybe if you can post some picture of your connection and a bit more detail about your setup it could be easier to help you.
```

---
