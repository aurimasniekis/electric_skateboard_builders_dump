# BLDC Tool changes for increasing battery size

### Replies: 15 Views: 1085

## \#1 Posted by: maker7 Posted at: 2016-12-10T18:03:48.488Z Reads: 108

```
I went from 6S to 9S on a 245kv, Enertion Vesc setup and have a question -

 I weigh 167lbs - and on 6S, I was getting a 20mph top speed, on 9s, it seems about the same, maybe 22mph.  I think maybe I missed a VESC setting - all I changed was cutoff start and end, did I miss something???
```

---
## \#2 Posted by: Blasto Posted at: 2016-12-10T18:53:14.144Z Reads: 99

```
post your configurations of the motor tab
```

---
## \#3 Posted by: maker7 Posted at: 2016-12-10T19:00:22.599Z Reads: 98

```
<img src="/uploads/db1493/original/3X/8/a/8a90a1b41fb9f850ce5b17ebe2920b776a453ea3.jpg" width="690" height="232">
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-12-10T19:05:52.675Z Reads: 90

```
Go higher with your motor max if the motors can handle it. 60 or 80 for example. Then go higher with your battery max if the batteries can handle it. Maybe 40 for example. And then set the maximum input voltage to 57.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-12-10T19:06:45.705Z Reads: 90

```
Please also post the bldc and application settings to be sure that you did the right thing.
```

---
## \#6 Posted by: maker7 Posted at: 2016-12-10T19:09:50.346Z Reads: 82

```
<img src="/uploads/db1493/original/3X/2/0/20fbfb29d311b43bd47c0b2bec97251804096d7b.png" width="690" height="424">
```

---
## \#7 Posted by: maker7 Posted at: 2016-12-10T19:18:38.699Z Reads: 66

```
Application or Advanced setting?
```

---
## \#9 Posted by: Ackmaniac Posted at: 2016-12-10T19:49:00.670Z Reads: 61

```
For the motor detection you should take the values which will be entered by the apply button. These are a bit lower than the detected values.  And just post all Screenshots you have.
```

---
## \#10 Posted by: maker7 Posted at: 2016-12-10T20:12:52.627Z Reads: 59

```
Ok here is the Motor Config - BLDC tab after detection and config write....

<img src="/uploads/db1493/original/3X/5/b/5b4b6993b81243f289231a73db813311fa2c1306.jpg" width="690" height="232">
```

---
## \#11 Posted by: maker7 Posted at: 2016-12-10T20:13:56.475Z Reads: 55

```
Also, my motor has a 70A max, should i set motor max to 70 and motor min to -70?
```

---
## \#12 Posted by: Ackmaniac Posted at: 2016-12-10T20:25:30.742Z Reads: 52

```
Correct. If it is too strong then you can lower it again. Seems that you had the wrong motor detection values before.
```

---
## \#13 Posted by: maker7 Posted at: 2016-12-10T20:27:52.170Z Reads: 54

```
Think I did not hit apply before.  Would you happen to know wht the avg distance range for a 6s setup would be?  I initially decided to upgrade to 9s to increase my range - was only getting 8 miles from 6s - could be because i had the motor settings wrong?
```

---
## \#14 Posted by: Ackmaniac Posted at: 2016-12-10T21:00:14.960Z Reads: 52

```
That depends on the ah the battery has.
6S * 3,7V * 5ah = 111Wh. And in average you need about 10 wh per km.  So a 6S 5ah battery would be good for roughly 11 km.
```

---
## \#15 Posted by: maker7 Posted at: 2016-12-10T21:35:02.551Z Reads: 45

```
I hate to be such a pain in the arse - I really do appreciate all of the help, BTW.  If I am using 3 Zippy 5000mAh 3S1P 20C battery - what should my Batt max setting be?
```

---
## \#16 Posted by: Ackmaniac Posted at: 2016-12-10T22:09:53.127Z Reads: 43

```
It would be capable of 5000mAh = 5Ah * 20C = 100A

But 100A would be too much for one VESC. If you have a single and want alot of power the try 50A and if you have 2 motors than use 40A on each. If it is too much then lower it.
```

---
