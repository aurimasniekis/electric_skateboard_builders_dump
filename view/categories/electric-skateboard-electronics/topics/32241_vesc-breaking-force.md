# Vesc breaking force

### Replies: 18 Views: 1017

## \#1 Posted by: Bloop Posted at: 2017-09-04T15:43:38.092Z Reads: 132

```
Sorry to ask this again .. i guess many asked this before but how could i increase my breaking force ?

Right now i can slow down but i cant fully stop when going down a hill .. I have a 190KV 2400W motor. Also should i change anything else on my settings ?
 <img src="/uploads/db1493/original/3X/4/9/49913c99164f17100f83c68733d1bcf24bdeb4e2.png" width="466" height="268">

Im using watt mode with both breaking and reverse (is working good but is not fully stoping me)
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-04T16:24:10.756Z Reads: 121

```
Is your PPM calibrated?
```

---
## \#3 Posted by: Bloop Posted at: 2017-09-04T16:38:14.504Z Reads: 112

```
the remote yes all min max and mid point
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-04T16:39:45.523Z Reads: 106

```
Is it able to fully stop at any speed ?
```

---
## \#5 Posted by: Bloop Posted at: 2017-09-04T16:43:37.760Z Reads: 104

```
i can slow down and stop eventually when on straight line but if i go down a hill i cannot stop and it will still roll ... if i have speed is even worse.. is slowing but i have to jump off so i dont hit a car or smething at the light stop
```

---
## \#6 Posted by: scepterr Posted at: 2017-09-04T16:52:22.278Z Reads: 100

```
Try increasing max erpm at full break?
```

---
## \#7 Posted by: Nix Posted at: 2017-09-04T16:57:31.078Z Reads: 98

```
What is the ppm
```

---
## \#8 Posted by: scepterr Posted at: 2017-09-04T17:11:06.249Z Reads: 97

```
Ppm is the remote signal, available under the app tab in bldc tool
```

---
## \#9 Posted by: Nix Posted at: 2017-09-04T17:13:23.412Z Reads: 93

```
So it's just like checking the remote signal
```

---
## \#10 Posted by: Bloop Posted at: 2017-09-04T17:21:33.774Z Reads: 90

```
yes when you go in the app you can set to show live what are the values and you have to set min max
```

---
## \#11 Posted by: Bloop Posted at: 2017-09-04T17:22:27.086Z Reads: 84

```
how do i do that and what value should i set it .. i know the erpm are both set max min at + - 60k ?? or you talking about something else?
```

---
## \#12 Posted by: scepterr Posted at: 2017-09-04T17:23:38.187Z Reads: 83

```
It's right under the max erpm option
<img src="/uploads/db1493/original/3X/3/2/321166945d378f1fbf21cc6b4cf1585bcd60c5bb.jpg" width="333" height="250">
```

---
## \#13 Posted by: Bloop Posted at: 2017-09-04T19:56:22.595Z Reads: 66

```
What would be a safe value for max ERPM at full break ?? mine is currently at 300.00 and the full break in current control mode is at 1500.00 

How much should i increase it ??
```

---
## \#14 Posted by: Deakbannok Posted at: 2017-09-04T20:14:35.522Z Reads: 62

```
No you cannot do full complete stop on a down hill.
But you can slow it down enough to do a foot break.

A full stop is more on a flat surface or slightly declined road
```

---
## \#15 Posted by: scepterr Posted at: 2017-09-04T20:24:45.401Z Reads: 56

```
Try 50 at a time

@Deakbannok I stop at the end of a hill going faster than I can accelerate on a straight atleast twice a day, 5 days a week, so I know it's possible
```

---
## \#16 Posted by: Bloop Posted at: 2017-09-04T20:34:09.220Z Reads: 54

```
any idea what should i expect ? Will it just break harder when i go full stop or will increase the breaking all around ? even at high speeds ?
```

---
## \#17 Posted by: scepterr Posted at: 2017-09-04T20:36:04.865Z Reads: 54

```
It should give higher stopping torque at max break
(Assuming I'm remembering my own tweaking correctly :wink: )
```

---
## \#18 Posted by: Bloop Posted at: 2017-09-04T20:38:23.515Z Reads: 51

```
really apreciate it i will test tomorrow and keep you posted :smile: hopefully will be ok. I played a bit with throttle curves with ackmaniac's firmware and is so smooth right now im in love with it.
```

---
