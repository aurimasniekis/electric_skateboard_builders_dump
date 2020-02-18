# Throttle issue with GT2B

### Replies: 12 Views: 1204

## \#1 Posted by: FlashNova Posted at: 2016-09-04T19:33:41.410Z Reads: 164

```
I'm having an issue where it starts braking when I let go of the trigger, which prevents me from being able to kick push my board. Is this normal? Or can it be fixed by adjusting the throttle response in BLDC? I was under the impression you could kick push these boards when you wanted to.
```

---
## \#2 Posted by: Titoxd10001 Posted at: 2016-09-04T19:37:39.906Z Reads: 160

```
You need to adjust throttle on your remote and double check on bldc tool that it's at 50%. Then reset your failsafe.
```

---
## \#3 Posted by: FlashNova Posted at: 2016-09-04T19:55:44.613Z Reads: 155

```
How do you reset the failsafe?
```

---
## \#4 Posted by: Titoxd10001 Posted at: 2016-09-04T20:11:19.529Z Reads: 147

```
@FlashNova The failsafe is on the receiver it's a little button that you press and hold. Before you do that you want to set the neutral by adjusting the throttle trim so it reads 50% in bldc tool.
```

---
## \#5 Posted by: Titoxd10001 Posted at: 2016-09-04T20:16:06.434Z Reads: 142

```
You can also check that failsafe is set properly by turning off your remote while on bldc tool it should stay at or close to 50%. If it goes to anything much higher or much lower that's were runaway boards and sudden breaks happen.
```

---
## \#6 Posted by: FlashNova Posted at: 2016-09-04T20:40:29.924Z Reads: 132

```
Okay got it. What do I put for "Brake current to use when a timeout occurs?". Do i just set it to whatever number the throttle reads at 50%?

<img src="/uploads/db1493/original/2X/e/e46f508a26b28f266ae422a156a998686552722a.jpg" width="605" height="500">
```

---
## \#7 Posted by: Titoxd10001 Posted at: 2016-09-04T20:50:57.066Z Reads: 120

```
I think its at zero stock meaning no brakes so it stays at neutral when signal is lost
```

---
## \#8 Posted by: FlashNova Posted at: 2016-09-04T20:53:59.705Z Reads: 120

```
So then leave it at zero?
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2016-09-04T21:00:40.568Z Reads: 121

```
Yeah I left it stock because it's asking for current and not pulsewidth. You would change value if you want brakes to be applied when signal is lost

Double-check when you turn off remote that the pulsewidth stays at 50%
```

---
## \#10 Posted by: FlashNova Posted at: 2016-09-04T21:06:04.657Z Reads: 121

```
Got it! Thank you sir!
```

---
## \#11 Posted by: Titoxd10001 Posted at: 2016-09-04T21:09:29.396Z Reads: 121

```
No problem
```

---
## \#12 Posted by: Namasaki Posted at: 2016-09-06T04:03:03.179Z Reads: 87

```
Here is a great tutorial on how to properly setup your remote with Vesc.
If your remote has trim knobs, set them to middle position before performing this calibration.
Leave time out current at zero or you could be thrown off  the board if your remote looses connection with the receiver.

https://youtu.be/OtuofrQr3F8
```

---
