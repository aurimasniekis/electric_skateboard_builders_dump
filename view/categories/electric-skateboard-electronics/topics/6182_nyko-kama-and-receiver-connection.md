# Nyko Kama and Receiver Connection

### Replies: 10 Views: 922

## \#1 Posted by: arpitdave Posted at: 2016-07-16T03:57:35.264Z Reads: 83

```
Hello, 
I soldered the nyko kama to a JST and connected it to the VESC. When i turn my battery on the there is no light turning on from the receiver? Any ideas as to why that may be? I have triple checked my connection. Maybe i messed up the soldering?
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-16T04:14:56.275Z Reads: 81

```
Picture of soldering please.
```

---
## \#3 Posted by: arpitdave Posted at: 2016-07-16T04:47:48.545Z Reads: 77

```
<img src="/uploads/db1493/original/2X/f/f0a218c6223fac0e565b990ac81c3b0f2bd622ba.png" width="640" height="480">
```

---
## \#4 Posted by: treenutter Posted at: 2016-07-16T06:01:29.088Z Reads: 67

```
@arpitdave are any of the wires shorting? You should heat-shrink those connections after you make them.
```

---
## \#5 Posted by: lox897 Posted at: 2016-07-16T06:45:37.136Z Reads: 60

```
Closer to the solder joints please.
```

---
## \#6 Posted by: trbt555 Posted at: 2016-07-19T08:46:52.860Z Reads: 42

```
If you're using a VESC with a HW version higher than 4.10 it will have a 7-pin header.
You're using a 6-pin plug, so you need to plug it in to one side of the header an leave the 7th pin (closest to the MOSFETS) open.
Are you 100% certain you're plugging it in to the correct side of the header ?
```

---
## \#7 Posted by: arpitdave Posted at: 2016-07-19T21:37:33.740Z Reads: 36

```
So I attached a few more pictures here. I put electrical tape around all the connections after taking these pictures. I plugged the JST in so that the green wire is closest to vesc side that connects to the motor. I am not sure where I could have errored. I am still not getting a light coming from this small pcb when i plug it in and turn the battery on :/
<img src="/uploads/db1493/original/2X/3/323aa21fa0567f456f3848075f033ce377e2ed68.JPG" width="375" height="500"><img src="/uploads/db1493/original/2X/e/e0792acb23dfebd6d1ed6cace46e32be9ca370a7.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/c/c8e03c5770fc6562ee8a34135e8fe3a82f71f3cc.JPG" width="375" height="500">[Uploading...]()
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-07-19T21:46:03.792Z Reads: 33

```
Get some shrink tubing next time...looks neater ...
```

---
## \#9 Posted by: Maxid Posted at: 2016-07-19T22:01:19.137Z Reads: 34

```
In this case it is not even about looks: with wires exposed like this, it will simply never work.
```

---
## \#10 Posted by: banjaxxed Posted at: 2017-09-23T23:20:25.630Z Reads: 11

```
I'd say you shorted it.

I'm in the know as I've just done the same thing, RIP Nyko
```

---
