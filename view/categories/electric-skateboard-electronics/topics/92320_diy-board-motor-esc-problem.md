# DIY board Motor / ESC Problem

### Replies: 4 Views: 221

## \#1 Posted by: xluckynumber7x Posted at: 2019-04-30T14:17:45.920Z Reads: 60

```
Need some help diagnosing a problem on my DIY board. Everything ran great up until I nailed a big crack in the road recently, even snapped the front off of my deck.

So I have a Torqueboards VESC 4.12 running a Torqueboards 6374 motor on 10s (2 x 5s lipos) and I cannot get it to run as Hall Sensors instead of sensorless. I reflashed the firmware (3.55) and ran through motor setup again. It does all of that though it took a couple of tries as I was getting error -11 a couple of times when running detection.

So it gets through detection and comes back as sensorless, Now in order to get going I have to push first and then it will work fine, braking and all. Is this a symptom of the motor or esc? I cleaned the motor and there doesn't appear to be any physical damage to it or the esc.

I checked for faults in the VESC Tool terminal and all it says is error code drv.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-30T14:21:49.723Z Reads: 63

```
You don’t have a second motor to swap and look from where the issue come?
You probably have an adapter cable from the motor to the vesc, make sure the connection is proper there. Also, did you try motor detection in FOC and bldc?

[quote="xluckynumber7x, post:1, topic:92320"]
error code drv
[/quote]

And this is usually a not so good sign. You might have fried your drv which means you need a replacement or new vesc if the fault is present all the time.
```

---
## \#3 Posted by: danieloath Posted at: 2019-04-30T14:55:26.143Z Reads: 52

```
Having to push before the motors start working is a common trait of running BLDC which is most likely what the VESC tool has decided run your setup in. As @Andy87 has pointed out, if you have a second vesc or motor to begin troubleshooting, that would obviously be optimal in order to narrow down on the issue. DRV error is never a good sign.

Try using VESC tool 0.95 and updating to firmware 3.4 and rerunning setup. You might get lucky.
```

---
## \#4 Posted by: xluckynumber7x Posted at: 2019-04-30T16:24:23.753Z Reads: 35

```
No extra motor or esc yet, and no one close by in the hobby either that might have a spare. Though looks like I'll be ordering some more stuff now, or just ran it as is. 

As far as FOC or BLDC I just ran the FOC motor wizard after reflashing the firmware like I did when I initially set it up after building. Then it came back as Hall Sensors and I could start from a dead stop no problem. Now it won't start from a stop, still FOC, but comes back as sensorless after detection. Manually changing it to Hall Sensors makes it so the motor will not run. 





![06|690x388](upload://k50ZMzwsTp4FsgH7aP6MOKcxceo.png) ![58%20(1)|690x388](upload://xjGLn3XHFxTBtciycUgSkY3jzkm.png)
```

---
