# Brakes way too sensitive

### Replies: 10 Views: 1244

## \#1 Posted by: Ryanliu Posted at: 2017-01-30T23:24:07.151Z Reads: 141

```
I checked everything on my esk8.
Battery: 36v 4p 10s tested, can handle 45a continuous 
Motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
ESC: link no longer available but it is a vesc firmware 2.16 version 4.12
Controller: http://www.ebay.com/itm/172388976080?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

My esk8 braking is way too sensitive and i was wondering how to change brake sensitivity. I am using current no reverse with brake and the displayed pulsewidth shows my throttle moving responsively and accurately to my inputs so my controller is good. 
Settings: IDK how to screen shot but let me know if u need more info
motor max: 40A
motor min (regen) -30A
Battery max 40A
Battery min (regen) -30A
MAX Erpm at full brake: 100,000
MAX Erpm at full brake in current control mode: 100,000
Min Erpm: -100,000
Max Erpm: 100,000
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-01-30T23:27:49.093Z Reads: 137

```
The is actually a little bit funny and easy to fix. You max Erpm at full brake in current control mode is way too high. It stands for below this Erpm the VESC should do a full brake. Just check which value it is when you read the default settings and use that.
```

---
## \#3 Posted by: Ryanliu Posted at: 2017-01-31T00:54:08.473Z Reads: 119

```
i changed it to 500Erpm for the full brake in both full brake and current control and now it works if it is going under 500rpm but anymore than that it just doesnt work. is there a value i might have changed unknowingly? i made the limits and ppm under app config. 
PID Max Erpm is 15000.00
deadband: .15
minimum pulsewidth: 1.12
maximum pulsewidth: 2.19
safestart is checked off
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-01-31T01:11:32.863Z Reads: 110

```
What do you mean by it doesn't work? No brake at all or does it brake too soft? Maybe post Screenshots of you settings or start again with the default settings.
```

---
## \#5 Posted by: Ryanliu Posted at: 2017-01-31T01:50:59.951Z Reads: 103

```
<img src="/uploads/db1493/original/3X/d/7/d7c64863726dc05088ab540d1e36cad090649b62.png" width="690" height="388"><img src="/uploads/db1493/original/3X/7/3/7302cd356ac1c686492b08a5bc6af6f0e4493d02.png" width="690" height="388">

these are my personalized settings
```

---
## \#6 Posted by: Ryanliu Posted at: 2017-01-31T01:51:32.836Z Reads: 90

```
i get no brakes at all after 500rpm
i also tried resetting everything to default config and nothing changed
```

---
## \#7 Posted by: Ryanliu Posted at: 2017-01-31T01:55:43.624Z Reads: 95

```
My ppm was the same as default but these r my default limits<img src="/uploads/db1493/original/3X/2/2/222b93f29ae5ac3ac6c8adb288da2e005a609646.png" width="690" height="388">
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-01-31T04:12:53.715Z Reads: 87

```
try these parameter... and it should work just fine..

<img src="/uploads/db1493/original/3X/1/6/167a3673c9618143da30f50fbd29ca44b03c0eaf.jpg" width="690" height="366">
```

---
## \#9 Posted by: lrdesigns Posted at: 2017-03-14T01:49:02.918Z Reads: 67

```
[quote="Ryanliu, post:1, topic:16930"]
Battery min (regen) -30A
[/quote]

I would change this to -5A which will probably be too soft, then go up 5amps at a time until it feels good. I thinks somewhere between -10 and -20 will be good. 

Also just keep the max ERPM at full brake and max ERPM at full brake under CC mode as per defaults, these seems to work for everyone. 300 and 1500 respectively.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-03-14T07:17:49.298Z Reads: 56

```
His problem was the maximum input voltage of 42V. With a fully charged 10S battery it shut down each time the regenerative braking raised the voltage.
```

---
