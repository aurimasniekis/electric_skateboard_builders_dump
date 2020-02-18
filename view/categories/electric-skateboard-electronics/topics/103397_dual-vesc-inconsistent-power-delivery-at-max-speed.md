# Dual VESC inconsistent power delivery at max speed

### Replies: 16 Views: 274

## \#1 Posted by: Joe1 Posted at: 2019-10-28T21:27:43.628Z Reads: 75

```
I have 2 builds with the same issue. 

At max speed (limited by KV and battery voltage) the torque output from each motor varies and feels unstable. 

I can feel one side pulling more than the other but each side will switch to which is putting down more power and the other side feels to drag or freewheel. It feels like the board is pulling in one direction or the other when this occurs. 

I understand that the max RPM at the given battery voltage is being reached. If I reduce the throttle just a little bit I can feel the power delivery being consistent again across both motors. 

Same motors, same VESC setting on each, using CAN bus for dual config, ppm remote. 

Anyone else experience this?
```

---
## \#2 Posted by: BillGordon Posted at: 2019-10-28T21:38:38.834Z Reads: 72

```
Motors are?
```

---
## \#3 Posted by: Joe1 Posted at: 2019-10-28T21:51:44.719Z Reads: 69

```
Dual Flipsky 6355 on one build, dual FS 6374 on the other. 190kv

Doubt it’s the motors. I can feel the issue at different speeds as the battery voltage starts to drop as the battery is used
```

---
## \#4 Posted by: Stan8 Posted at: 2019-10-28T22:27:07.348Z Reads: 64

```
How do you notice the difference? Do you feel it, and is it that noticable?
```

---
## \#5 Posted by: Joe1 Posted at: 2019-10-28T22:52:50.392Z Reads: 61

```
Yes it’s very noticeable. At first I thought it was an issue with the front trucks. 

The boards starts actively veering to a side and I need to actively compensate. However it’s scary/difficult at speed (28-30mph). Laying off the throttle even the slightest bit recovers to even power. 

I’m using the latest Ackmaniac build, 15T/66T, 175mm AT wheels, FS6.6, 10S6P

I haven’t ridden other dual VESC boards at max speed limited by KV so I don’t have a reference. 

Is this typical?
```

---
## \#6 Posted by: esk8snith Posted at: 2019-10-28T23:49:31.076Z Reads: 60

```
After programming the motors, are you setting the batt max of each of the VESC's separately? 

If you are using the FOC setup tool, it will set your batt max on each side to 99A by default, if you're not changing that manually on both sides of the VESC, one side will more current when you accelerate.
```

---
## \#7 Posted by: Joe1 Posted at: 2019-10-29T00:28:17.130Z Reads: 55

```
Battery amps are the same on both VESCs. I’m leaving it to 99A each and not drawing max current at max speed. Testing on flat. 
Motor amps are 60A ea on one board and 80a on the other. Also not maxing motor amps at max speed.
```

---
## \#8 Posted by: esk8snith Posted at: 2019-10-29T01:09:05.984Z Reads: 52

```
why would you set different motor amps on each side. That's why you're experiencing the pull. It's not about max draw. If you have different values, obviously one side will pull harder than the other.
```

---
## \#9 Posted by: Joe1 Posted at: 2019-10-29T01:24:30.348Z Reads: 49

```
Same on both sides. I have 2 boards with 60a each motor on one and 80a each motor on the other.
```

---
## \#10 Posted by: itsrow Posted at: 2019-10-29T02:04:26.045Z Reads: 48

```
Ideally I would set them the same, because even though you may not be drawing 60A or 80A at any time or even a split second, I believe FOC and BLDC still uses the value when calculating acceleration curves and other settings.  I would change it for now just to rule it out as a problem because every VESC works differently and their a finnicky bitch until their not.
```

---
## \#11 Posted by: gijoe28 Posted at: 2019-10-29T02:20:28.837Z Reads: 45

```
They ARE the same - we have TWO builds - one build both motors run at 60a, and the other build both motors run at 80a.

I'm the guy with the 80a motors build - @Joe1 has the 60a, but we're both experiencing the same exact symptoms.

We actually have two distinct issues but they may be co-related.

1) what Joe1 said earlier, at max speed the board starts to veer out in a direction (random which direction never the same)

2) when you let off the throttle after max'ing the board briefly jerks in a direction and then corrects itself.
```

---
## \#12 Posted by: itsrow Posted at: 2019-10-30T17:46:50.077Z Reads: 30

```
Are you using traction control?  It sounds like its kicking in too early, try  increasing the difference value of when it enables (default 3000rpm) and if that doesnt help try disabling it and if that doesnt work try split PPM instead of canbus for the connection.  Any DRV failures or fault messages when it happens?  I can't imagine any reason for them to do it.
```

---
## \#13 Posted by: Skyart15 Posted at: 2019-10-30T22:00:11.620Z Reads: 24

```
Are you using the Fsesc dual 6.6? I have the same problem and it gets worse when my battery is under 30%
```

---
## \#14 Posted by: Joe1 Posted at: 2019-10-30T22:39:44.880Z Reads: 25

```
Yes,

FlipSky Dual 6.6 on one board and 2x FlipSky Single 6.6 connect via CAN on the other board. 

So you feel it when you hit top speed?
Can you explain it.
```

---
## \#15 Posted by: itsrow Posted at: 2019-10-31T01:00:33.800Z Reads: 26

```
For your safety I would genuinely replace those VESCs if possible.
```

---
## \#16 Posted by: Joe1 Posted at: 2019-10-31T05:49:16.212Z Reads: 24

```
TC is off. Unfortunately it’s raining all week and can’t test.
```

---
