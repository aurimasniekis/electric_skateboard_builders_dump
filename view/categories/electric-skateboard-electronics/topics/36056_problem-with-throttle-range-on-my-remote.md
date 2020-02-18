# Problem with throttle range on my remote

### Replies: 4 Views: 663

## \#1 Posted by: zepton Posted at: 2017-10-20T16:21:04.006Z Reads: 100

```
I’ve had a problem recently that causes my 2.4ghz remote to not get the full throttle range out of the controller. If I push my throttle stick to around 80% my longboard hits its top speed which can be quite frustrating. The controller is already quite small, and having only 80% of the throttle range means that I can’t control my speed as precisely as I would like.

I have calibrated the throttle range so that the maximum and minimum throttle positions appear as maximum and minimum on the pulsewidth display in BLDC tool. My Vesc is set to current control mode. When I tried using duty cycle mode, the problem went away; Duty cycle mode allowed for my top speed to be reached when I hit 100% on my throttle, which is what I would like to happen in current control mode.

I also tested this with my rc car controller and I had the same problem, meaning that it is not an issue with the controller.

My setup: Single drive, 6S setup
2.4gHz nano remote from 
4.12 Vesc from  with firmware 2.18
192kv motor from hobbyking.com
2 5000mAh 3S lipo batteries in series

Here are some pictures that I made that describe my problem:<img src="/uploads/db1493/original/3X/d/e/de19773531f0a185eadfe0e883e729b3f2f6ee22.jpg" width="608" height="160"><img src="/uploads/db1493/original/3X/7/7/775f033e0c7dfb56ab6fec56ff8d9a62e1b971ce.JPG" width="670" height="422">
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-20T16:25:37.556Z Reads: 91

```
That's how current control works on the VESC. It controls acceleration not speed. You can use PID speed control or duty cycle, but they're worse solutions since you can't coast with them.

Throttle modulates current and once the given current can overcome load, it'll spin at full duty cycle.

@Ackmaniac's f/w uses watt control which is similar to current control but gives you superior throttle control at speed, so you can try that as well.
```

---
## \#3 Posted by: Titoxd10001 Posted at: 2017-10-20T16:47:48.229Z Reads: 88

```
Yes unfortunately that's how vesc with current control works. I probably only use 25% if that with ackmaniacs firmware and still reach high speed. Only use close to full throttle to start up. It's unfortunate we can't use duty cycle mode which would be perfect. Would give you more torque down low and more control in the upper rpms.
```

---
## \#4 Posted by: vishal_tejwani Posted at: 2017-10-21T08:40:36.927Z Reads: 65

```
I am selling custom made remote , wii nunchuck check out my page under used items for sale
```

---
