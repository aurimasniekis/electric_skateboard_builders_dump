# FocBox Detection failed (Solved)

### Replies: 9 Views: 189

## \#1 Posted by: xatonic Posted at: 2019-06-16T07:46:36.546Z Reads: 72

```
Hey guys! so i just set up everything I need on my board to the point where I'm doing the software stuff now and im having an issue. so my issue is that the BLDC firmware (ackmaniack) fails the motor detection and gives me the message "bad detection result received" in the lower right-hand corner. I have upped the duty cycle all the way to .10 and am worried to go past that point, I have also incrementally upped the amperage to 10a and no luck. when I press detect motor (Btw I'm doing this as sensored bldc and have tried sensorless bldc with the same results) the motor spins up then slows down and stutters (I've heard it's supposed to do that) and then gives me that error. I've checked the terminal for faults and there are none, what am I doing wrong?! I am using an enertion FocBox and a DIYes 6380 motor, here are my settings as always thanks a bunch!
 ![image|690x425](upload://srqIWAo7TF1CybHbYOXoVmTFLGj.png) ![image|690x421](upload://4ohidmmqN3JH4T6jG47gtJYi1zc.png) ![image|690x422](upload://3KlRCGu9AUPZx5jHIg5ViIH3SBf.png) ![image|690x421](upload://520q8z0tVeFRTjRZvh0rAL65lx3.png) ![image|690x425](upload://2dj1hpfQfAOPj1vGbdd9511T97Y.png)
```

---
## \#2 Posted by: CarlCollins Posted at: 2019-06-16T10:16:22.565Z Reads: 53

```
Try reverting back to 2.18 firmware and use Enertion's BLDC tool for the motor detection.
let us know if you still face same issue.
```

---
## \#3 Posted by: xatonic Posted at: 2019-06-16T17:21:34.679Z Reads: 36

```
It says I need a programmer and I can't figure it out
```

---
## \#4 Posted by: Blasto Posted at: 2019-06-16T17:47:18.137Z Reads: 36

```
Increase this setting to 10A

![image|690x348](upload://x1qNdStt2dWmgPlsas21XEZPGKG.jpeg)
```

---
## \#5 Posted by: xatonic Posted at: 2019-06-16T17:53:08.448Z Reads: 34

```
Just tried that, still no luck
```

---
## \#6 Posted by: xatonic Posted at: 2019-06-16T23:33:18.949Z Reads: 32

```
@blasto any other suggestions?
```

---
## \#7 Posted by: Blasto Posted at: 2019-06-16T23:38:17.582Z Reads: 32

```
What is your motor doing? A quick video will help
```

---
## \#8 Posted by: ShutterShock Posted at: 2019-06-17T03:43:43.545Z Reads: 26

```
This happened to me every time I tried to use BLDC on my FOCBOX's too, so I ended up just using FOC haha.  I have been running FOC on 12s 190kv for like a year and a half now with no issues but sometimes I wish I had the better braking from BLDC.
```

---
## \#9 Posted by: xatonic Posted at: 2019-06-17T03:54:12.106Z Reads: 26

```
so I figured it out! I had to up the ERPM to 350 because it was such a large motor
```

---
