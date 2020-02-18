# Vesc drv8302 fault + Failed detection

### Replies: 9 Views: 2395

## \#1 Posted by: sk8ace Posted at: 2015-12-19T19:06:39.371Z Reads: 113

```
I didn't want to hijack the other thread so I'm making this one. 

I had everything set up and running last night. Went out for 2 test rides and both went well. After the second test ride I wanted to adjust the sensitivity of the nunchuck stick for smoother acceleration. I loaded up bldc tool and was browsing around the tabs and realized that in App Config/PPM tab, Control mode was checkmarked Current instead of Disabled. I had it set for the Nunchuck so I disabled PPM and rebooted. When it turned back on, the motor spun up by itself for a few seconds and stopped. After that, the motor would not respond to the nunchuck input. I went to the nunchuck tab and can watch the Display move when I move the stick so the vesc is seeing my inputs but nothing is happening. Next I went to the Realtime Data tab and saw the Fault drv8302 when I would hit any button on the nunchuck. 

I just loaded up the latest firmware to see if would be fixed but I am still getting the same drv8302 fault and Detection fails every time now. The motor isn't moving at all. 

Pictures: 
<img src="/uploads/db1493/original/2X/0/06096f45603da8949b69008a3a552f932eac8eff.jpg" width="690" height="482">
<img src="/uploads/db1493/original/2X/7/79a738e7a66321b9e160392f4d369c135fe776ae.jpg" width="690" height="440">

At this point, it seems I have a dead drv8302 chip. Any ideas?
```

---
## \#2 Posted by: NIK Posted at: 2015-12-19T20:34:55.254Z Reads: 109

```
I got the same result. Do u have any plan to replace with new DRV8302?
```

---
## \#3 Posted by: sk8ace Posted at: 2015-12-19T21:09:23.117Z Reads: 111

```
Probably going to order both a new chip and another vesc. I've never soldered something that small so if I mess up.. I'll still be able to ride. And if I do it and it works, I'll be ready for dual motors lol. 

I just want to be sure that's what it is. This is going to set me back at least another 2 weeks :-(
```

---
## \#4 Posted by: kai Posted at: 2015-12-19T22:10:23.174Z Reads: 108

```
That sucks bro. At least you can still ride though!
```

---
## \#5 Posted by: sk8ace Posted at: 2015-12-20T00:03:15.781Z Reads: 106

```
New vesc ordered. Still going to try to get this working while I wait for it to get here. At least I got to ride for a few minutes last night lol.
```

---
## \#6 Posted by: NIK Posted at: 2015-12-22T19:29:22.211Z Reads: 97

```
Hi guys, I replaced new DRV8302 and tested, works like a charm now. Good for dual drive. yeah :smile:
```

---
## \#7 Posted by: sk8ace Posted at: 2015-12-22T20:10:39.988Z Reads: 97

```
Woohoo! Glad you got it working. My chip has been ordered should be in this weekend. How was it soldering all those tiny pins?
```

---
## \#8 Posted by: NIK Posted at: 2015-12-23T09:15:22.207Z Reads: 94

```
I bought 2 chip in case anything happens and hell it did. I have no experience in surface mount soldering. Via prof. youtube, I tried to solder it and very poor soldering. Removed it again and went to Portsmouth Uni lab, asked for a technician to do it for me. hahaha I must say its quite hard to do it myself for the first time. Removing the chip is easy if you use hot gas and I think that's what Vedder's using in his tutorial vid.
```

---
## \#9 Posted by: Patate Posted at: 2016-11-28T23:49:24.204Z Reads: 35

```
I have had the error DRV8302 after passing to FOC mode, the autoconfig had been done with the gears and was not precise, each time i accelerated the error jumped in, and I couldn't get the board moving when standing on it, after removing the Belt I did the config properly and voila every thing is working as a charm, FOC does make a huge difference compared to BLDC.
Hope this helps
```

---
