# FOC mode throttle problems

### Replies: 11 Views: 1146

## \#1 Posted by: zepton Posted at: 2017-11-10T22:36:54.113Z Reads: 104

```
Okay so I just started using FOC mode on my Vesc and I noticed something odd. My motor RPM spins faster when I am at a lower throttle than when I am at a higher throttle according to the real time data graph. I am in current control mode. 

I tested it using a different remote so it isn't a remote issue.

I also tried using @Ackmaniac firmware, same issue. 

Here are the images of the RPM graph below, the first one is when I am at full throttle and the second one is when I am at around 20% throttle.
<img src="/uploads/db1493/original/3X/d/6/d6e8850cba308af5b14e01cee34ac5f0970e751c.png" width="690" height="385"><img src="/uploads/db1493/original/3X/0/b/0b8c9374165c851783a5fd3e2de0a59b25da26c1.png" width="690" height="385">
```

---
## \#2 Posted by: zepton Posted at: 2017-11-10T22:38:15.403Z Reads: 93

```
Here are some other screenshots for those interested. <img src="/uploads/db1493/original/3X/5/b/5b0051f35982c7a2ae75cf46c64c68b8272a70b7.png" width="690" height="385"><img src="/uploads/db1493/original/3X/1/3/131ac163515ca71ce72b09526f37ae59e6dc1d9f.png" width="690" height="385"><img src="/uploads/db1493/original/3X/c/2/c2c0287947bb8ac3fe02be58fd1cf3ebc51ee1b7.png" width="690" height="385">
```

---
## \#3 Posted by: Surfer Posted at: 2017-11-10T22:39:58.442Z Reads: 89

```
Same here, which vesc are you using?
```

---
## \#4 Posted by: zepton Posted at: 2017-11-10T22:45:52.763Z Reads: 85

```
I'm using the 4.12 Vesc with 2.18 firmware from
```

---
## \#5 Posted by: mccloed Posted at: 2017-11-10T22:46:02.675Z Reads: 87

```
I assume this is on the bench since your motor current is under 3A? May have something to do with your Battery amps being higher than your Motor amps, but I am not the expert on this. @Ackmaniac?
```

---
## \#6 Posted by: Surfer Posted at: 2017-11-10T22:51:18.379Z Reads: 85

```
i'm using a focbox, actually i did never feel that when ridding....weird!!
in another setup i have this doesn't happend in bldc, did you have this issue in bldc?
```

---
## \#7 Posted by: Colson003 Posted at: 2017-11-10T22:56:18.735Z Reads: 82

```
My TB VESC had quirks running FOC on 2.18. I'm now on 3.31 or 3.30 using the VESC tool and it seems to run much better than before.
```

---
## \#8 Posted by: zepton Posted at: 2017-11-10T23:34:09.985Z Reads: 76

```
Never had the issue in BLDC. Maybe it is a bug?
```

---
## \#9 Posted by: Jinra Posted at: 2017-11-11T00:46:12.754Z Reads: 74

```
Both pics are at 95% duty. Throttle in current control doesnt work like most other esk8 brands. Throttle in current control controls acceleration NOT speed. So without a load even a tiny bit of throttle will ramp the motor up to full speed. The two pictures are essentially the same.

HOWEVER, there is a bit of weirdness with FOC on 2.xx software where sending more current at max duty will cause the motor to change in tone (and in this case lose ~1000erpm). I'm not exactly sure what causes it but the problem doesn't exist in f/w 3.xx.

I'd recommend anyone using foc to use f/w 3.xx
```

---
## \#10 Posted by: zepton Posted at: 2017-11-11T01:05:12.921Z Reads: 68

```
Could you reply with a link to where I could find the 3.xx firmware?
```

---
## \#11 Posted by: Jinra Posted at: 2017-11-11T01:06:09.955Z Reads: 64

```
Official: http://vesc-project.com/

Modified Ackmaniac: http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
