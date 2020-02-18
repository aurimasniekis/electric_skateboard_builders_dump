# VESC 4.12 Motor Detection Not Working

### Replies: 12 Views: 594

## \#1 Posted by: Alanhunt123 Posted at: 2017-07-19T01:34:12.521Z Reads: 50

```
Hi All,

I recently picked up a VESC 4.12 from a friend who purchased it from DIY Electric Skateboard. I just tried doing a motor detection with it, which isn't going very well. When I hit the "start detection" button nothing seems to happen. No stuttering, no spinning. When I open up the realtime data, I can see that the VESC can see the current spikes when I spin the motor, and accurately tracks the ERPM. I'm sure there are no shorts on the motor wires.

Any ideas?
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-19T01:35:55.704Z Reads: 50

```
could be battery cutoff values, make sure they're both lower than your power source voltage
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2017-07-19T01:38:18.614Z Reads: 48

```
It was set to 34v and 33v, using a 10S battery here. I tried setting both to 10V, no change.
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-19T01:39:18.967Z Reads: 48

```
could you post vesc settings, or try writing defaults (and adjusting cutoffs again) and redoing detection
```

---
## \#5 Posted by: Alanhunt123 Posted at: 2017-07-19T01:41:14.578Z Reads: 47

```
<img src="/uploads/db1493/original/3X/7/0/70170b279c8699e2050eb9e232378bbf1a8f3b37.JPG" width="690" height="407">

<img src="/uploads/db1493/original/3X/c/c/cc78cd24a7392cdfb7d58e350f28bd2704556c27.JPG" width="690" height="407">
```

---
## \#6 Posted by: torqueboards Posted at: 2017-07-19T01:46:43.934Z Reads: 41

```
I'd try the battery cut off settings again and make sure they match with the battery pack your testing with. That's typically the #1 reason you wouldn't be able to "motor detect".
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-19T01:47:07.100Z Reads: 41

```
try upping min eRPM (to up to about 1000) or low duty (up to .15)
```

---
## \#8 Posted by: Alanhunt123 Posted at: 2017-07-19T01:50:41.339Z Reads: 40

```
Tried all above suggestions. Nothing. Just checked the battery voltage on my multimeter, it reads 40.4V
```

---
## \#9 Posted by: Alanhunt123 Posted at: 2017-07-19T01:51:22.716Z Reads: 38

```
By the way, the VESC is flashing its red light 5 times, continuously.
```

---
## \#10 Posted by: Jinra Posted at: 2017-07-19T01:53:14.791Z Reads: 39

```
Go to the "terminal" tab and type "faults" after you try to run detection
```

---
## \#11 Posted by: Alanhunt123 Posted at: 2017-07-19T01:53:46.103Z Reads: 38

```
"No faults registered since startup."
```

---
## \#12 Posted by: Blasto Posted at: 2017-07-19T03:57:41.297Z Reads: 33

```
[quote="Alanhunt123, post:9, topic:27992, full:true"]
By the way, the VESC is flashing its red light 5 times, continuously.
[/quote]

Whats the input voltage and temperature reading in the real time data tab?
```

---
