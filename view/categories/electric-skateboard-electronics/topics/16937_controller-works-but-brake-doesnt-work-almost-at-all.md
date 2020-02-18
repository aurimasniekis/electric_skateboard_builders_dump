# Controller works but brake doesnt work almost at all

### Replies: 5 Views: 797

## \#1 Posted by: Ryanliu Posted at: 2017-01-31T04:04:25.925Z Reads: 61

```

Setup
149kv turnigy sk3 motor
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
Vesc, No more link but it has firmware 2.18
Controller that has been tested to work:
http://www.ebay.com/itm/172388976080?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
Battery: 10s 4p lithium battery that has been tested on my 500w ebike and it works

my controller is good because i can see the pulsewidth changing consistently and smoothly with the controller
When my motor is over the 300rpm (the minimum rpm for max brake) the brake just doesnt work. 
How do i fix this? 
These are screenshots of my BLDC configuration
<img src="/uploads/db1493/original/3X/6/0/6096d8e4909ea306fa203463db9e9ef8e844eb2c.png" width="690" height="388"><img src="/uploads/db1493/original/3X/a/f/af79c8ed4ab27ce432b8b6026baaabb984c711db.png" width="690" height="388"><img src="/uploads/db1493/original/3X/4/1/41d258c813bfaa87f255e70fd60106ebd7d7a476.png" width="690" height="388"><img src="/uploads/db1493/original/3X/d/0/d0fd6458a280464af690144b7874b7edcf1db395.png" width="690" height="388">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-01-31T04:17:41.523Z Reads: 49

```
did you input the max and min pulse width according to the readings in the box next to the green bar display?
and write to the vesc?
```

---
## \#3 Posted by: Ryanliu Posted at: 2017-01-31T06:04:53.049Z Reads: 46

```
Yes i put the throttle to max and put that value in. And also the throttle low
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2017-01-31T06:43:55.204Z Reads: 44

```
Does this remote have a mode feature? Beginner and regular?
```

---
## \#5 Posted by: Ryanliu Posted at: 2017-01-31T19:51:17.057Z Reads: 28

```
No it can only change channes with a switch. There is no more change button
```

---
