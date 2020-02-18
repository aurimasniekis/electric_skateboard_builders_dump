# FOC Negative Power?

### Replies: 12 Views: 381

## \#1 Posted by: twan Posted at: 2017-09-17T02:40:25.221Z Reads: 78

```
<img src="/uploads/db1493/original/3X/8/4/84bdf5afa61aab829f718c46febe6be8045d2496.png" width="690" height="405">

Anyone seen this before? If i push my throttle to about 20% the motor spins at max, but if i press it down some more the motor then sounds like it has a load on it and the graph shows negative wattage and the mosfet temps increase really fast.
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-17T02:45:34.638Z Reads: 73

```
Calibrate ppm/ your remote
```

---
## \#3 Posted by: twan Posted at: 2017-09-17T02:48:40.710Z Reads: 72

```
It is calibrated though :O <img src="/uploads/db1493/original/3X/8/3/83c5af9a786076eb1416565c8ebebd9759f76ae5.png" width="690" height="407">
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-17T02:50:45.448Z Reads: 70

```
Rerun motor detection? Any faults showing up?
You're running 2 vescs? Does this happen on both or just one?
```

---
## \#5 Posted by: twan Posted at: 2017-09-17T02:51:56.264Z Reads: 67

```
Wow thats weird so I switched the ppm from 1.92 to 1.93 and it fixed it, thank so much ! So weird. Any clue why it does that?
```

---
## \#6 Posted by: scepterr Posted at: 2017-09-17T02:52:30.739Z Reads: 67

```
The remote itself could've lost calibration. I would suggest the extended firmware by @Ackmaniac, the wizard there might give you more reliable values
```

---
## \#7 Posted by: twan Posted at: 2017-09-17T04:58:21.059Z Reads: 50

```
ahh i flashed his firmware and how the problem is back. max throttle gives me -150 watts no load.. this is gonna make the motor heat up reall quick...
```

---
## \#8 Posted by: Bloop Posted at: 2017-09-17T05:06:00.659Z Reads: 46

```
What remote are you using also make a screenshot of the application tab
```

---
## \#9 Posted by: scepterr Posted at: 2017-09-17T05:09:26.973Z Reads: 46

```
@twan did you run wizard after you flashed firmware? And write settings
```

---
## \#10 Posted by: twan Posted at: 2017-09-17T05:15:13.585Z Reads: 46

```
@scepterr yess i ran the wizard and got the controller all set up to get the correct range but still dont understand why the motor is getting -150 watts at max throttle. when it was set at no app and i use my keyboard and maxed it, it showed 50wats but when i changed over to my mini remote it gets fked up. '

@Bloop im using the mini remote 
<img src="/uploads/db1493/original/3X/7/e/7e81750de0a270c274b0db4c3ca0d54acac482f0.png" width="690" height="412">
```

---
## \#11 Posted by: scepterr Posted at: 2017-09-17T05:17:40.777Z Reads: 39

```
I'm not personally familiar with that remote
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-09-17T08:09:03.802Z Reads: 34

```
Just don't torture the Vesc on the bench. 
Via remote you tell it to use much power which it can't use because it spins already at full speed. With the keyboard you tell it to use little amps which are enough to reach max speed. 

Its like you at work. Keyboard is when your Boss told you to do something and lets you do it quietly. Via remote is like he stands beside you with a megaphone and shouts at you to work faster the entire time.
```

---
