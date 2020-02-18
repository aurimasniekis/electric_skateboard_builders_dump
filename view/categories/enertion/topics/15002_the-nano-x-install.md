# The nano-x install

### Replies: 7 Views: 1738

## \#1 Posted by: ripnrider Posted at: 2016-12-21T01:26:39.292Z Reads: 235

```
Received the nano-x yesterday & today I paired it with the receiver; both motors ran, and I took it out for maiden trip, about a mile. shut off receiver & tried turning on again and there was no reception.  the lights are solid on receiver but no control to the motors. Ran up both motors from BLDC.   Any recommendations on troubleshooting this issue.  thanks.
```

---
## \#2 Posted by: Jebe Posted at: 2016-12-21T03:30:12.866Z Reads: 213

```
any errors on the vesc's?
I had some trouble pairing but nothing during my test ride.
```

---
## \#3 Posted by: Schulerbible Posted at: 2016-12-21T08:53:42.152Z Reads: 195

```
Off topic question: Did you change your ppm settings to get more control over the remote?
```

---
## \#4 Posted by: SeanHacker Posted at: 2016-12-21T09:06:34.497Z Reads: 189

```
You would definitely want to set the min and max pulse width in order for the remote to use its full potential.
```

---
## \#5 Posted by: ripnrider Posted at: 2016-12-21T10:55:33.259Z Reads: 171

```
PID max ERPM  is 15000.00
deadband           is .015
min. pulsewidth  is  1.00
max. pulsewidth is  2.00
<img src="/uploads/db1493/original/3X/d/b/dbc34c23616e0e4fb1d4d98165f277df3345ce98.png" width="689" height="75">
```

---
## \#6 Posted by: ripnrider Posted at: 2016-12-21T11:29:00.432Z Reads: 161

```
<img src="/uploads/db1493/original/3X/d/7/d77839f42438a4ed08aa268fbd5920c90c1d042e.JPG" width="690" height="132">



screen shot from nunchuck tab
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-12-21T13:43:39.460Z Reads: 145

```
you need to be in ppm.... not nunchuck

Maybe use this topic to help you configure it : 
http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244
```

---
