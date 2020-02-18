# Power failure after 30 to 90 seconds

### Replies: 8 Views: 758

## \#1 Posted by: Aggdaddy Posted at: 2016-11-11T06:04:43.308Z Reads: 67

```
I have a prebuilt mountain board by a UK builder.  I just installed two new vescs and configured them and the wheels run ok and smoothly, but after 30 seconds to one minute and a half of running them on a box to test, the power shuts down.  if I turn of the power, then back on, the power drops out quicker, like 5 to 10 seconds when I am running the wheels.  The LED volt meter doesn't come back on unless I power cycle it.  

Its wired up to a LED volt meter and a switch and something that looks like a amp shunt.  If I unplug the battery from the power switch, LED VM wires and plug directly into the VESCs using XT60 splitter, it works fine.  No shut down.

I'd like to keep the power switch and LED VM and charging port wiring for convenience, but I am not sure where the problem is to fix it.

Any ideas?



10s battery
2 x 4.12 VESCS with heatsinks
2 x 300KV motors
Winning receiver
power switch
charging port

**SHUNT PIC** 
<img src="/uploads/db1493/original/3X/2/f/2fcf6b8597cf0a86db5fedff0c8ef090ed781934.jpg" width="281" height="500">

**Power switch and charge port PIC**
<img src="/uploads/db1493/original/3X/9/7/97ab6c200f8fa187b1d87a7e9f5761291dace59c.jpg" width="281" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2016-11-11T06:08:11.745Z Reads: 62

```
You should post full details of your VESC settings, screenshots work best.
```

---
## \#3 Posted by: Aggdaddy Posted at: 2016-11-11T06:18:14.488Z Reads: 61

```
Which parts?  Lots of different screens with the tool.  I only did a motor detection and changed to PPM mode with current and braking.  tweaked the min and max pulse for to 1.05 and 2.05  for both VESCs.  Nothing else was changed.  I also made sure to use only one red wire of the servo Y-splitter cable.  No canbus cable being used.

using BLDC, no FOC.

It runs fine with just battery to ESC's.

" tweaked the min and max pulse for to 1.05 and 2.05"  - I was trying to utilize the full throw of my transmitter.  It gets to max speed before I get to 60% throttle.  Not sure how to adjust for that.  I'll make another thread for that.
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-11T06:37:18.055Z Reads: 48

```
what you should do is run it again while your computer is plugged into it until it shuts off and figure what error code you're getting. You can find it on the real-time data tab, just activate "active monitoring".

As far as your motor reaching max speed early, that's just how the current control on the vesc works. Once supplied current overcomes load you go full speed, which is why you go max speed with minimal throttle while bench testing.
```

---
## \#5 Posted by: Aggdaddy Posted at: 2016-11-11T07:04:56.547Z Reads: 44

```
ok, I'll try it in the morning. Doesn't seem like its the vescs though.   It seems like power is being stopped somewhere between the battery and the vescs.  Because the vesc's couldn't make the LED VM turn off, which is what is happening when I lose power.
```

---
## \#6 Posted by: Aggdaddy Posted at: 2016-11-11T07:16:43.699Z Reads: 44

```
Also, I forgot to mention that I am comparing the throttle response to my bamboo GT.  It only gets to max throttle on the bench when I am much closer to full throw of the trigger.   When I am at half throttle, it doesn't ramp up like these VESC's are doing.

I get what you are saying though.  With such a configurable device, I figure there must be a way to fine tune the throttle. 


Probably not a fair comparison, since I'm not sure what kind of techno wizardry is in the bamboo GT but the throttle response is very predictable through out the entire range.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-11-13T05:18:54.476Z Reads: 26

```
300kv motors and 10s voltage is way over the Vesc 60k erpm limit. 
It's a wonder you haven't fried your vescs yet. 
300 x 42 x 7= 88200 erpm
```

---
## \#8 Posted by: Aggdaddy Posted at: 2016-11-13T05:38:26.978Z Reads: 23

```
Thanks.   My power failure problem has been resolved.  The 300kv motors were not my first choice as this was a complete board from the builder.  I didn't know about the ideal motor combos for vescs before I purchased the board.  So I am using what I have. 

So far the motor/vesc combo is working for me.  I've put two hours of riding through the combo since i have installed the vescs and configured them.  They have heat sinks attached and seem to be working ok atm.
```

---
