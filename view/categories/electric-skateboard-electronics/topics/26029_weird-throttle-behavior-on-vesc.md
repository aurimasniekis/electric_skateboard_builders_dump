# Weird throttle behavior on VESC

### Replies: 10 Views: 1603

## \#1 Posted by: Silverline Posted at: 2017-06-24T00:18:20.892Z Reads: 139

```
Hallo

Just upgraded this E-board to a VESC 4.12 https://www.elxskate.com/collections/all/products/x1-electric-skateboard

I´m new to VESC and BLDC tool. But i have a weird throttle behavior. From about 70-100% throttle, the motor just spins up maximum rpms, without any difference between 70-100 % throttle.

When i check my ppm output, it`s looks fine, when i not touching the remote it is 50%, and full throttle 100% 

Ohh and sometimes when i give fast throttle indput from 0, i can make the motor "stutter a little. Something i can do about that ??

Please help a newbee 
thanks :slight_smile: 
<img src="/uploads/db1493/original/3X/d/6/d63b692203cdd60d418f20efef64416d286b92d0.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/b/d/bde3e80cc9748e4e9dc85d4f6316f2c1f2c1edd8.jpg" width="690" height="388">
```

---
## \#2 Posted by: Stef Posted at: 2017-06-24T00:40:08.350Z Reads: 123

```
Max revs at any throttle is normal with current control if you lift up the wheels, for me it goes to max revs even at 10% if I lift up the wheels. Do you notice a difference between 70 and 100 when riding normally?

Your remote is acting normally

A little motor stuttering from startup is normal if you run unsensored. You can prevent this by pushing your board once at startup, or using sensored motors
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2017-06-24T00:43:32.742Z Reads: 120

```
If your on a bench it is normal, to see a difference you need to put some load on your motor... Like when you ridding it...
```

---
## \#4 Posted by: Silverline Posted at: 2017-06-24T00:44:26.023Z Reads: 118

```
Hallo Stef and JohnnyMeduse
And thanks for answering :slight_smile:

I have only tested on the bench, with no load on the motor. But with my old normal esc, i could change rpm`s on the bench. But maybe the VESC is doing something different ? 

I will try riding tomorrow, im a newbee, so full throttle behavior on the bench makes me a little nervous
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-06-24T00:48:42.434Z Reads: 113

```
the Vesc is a current control esc, so if don't have any current rushing trough it won't give you more power.
```

---
## \#6 Posted by: Silverline Posted at: 2017-06-24T00:54:43.050Z Reads: 110

```
I try riding my board tomorrow then...
Fingers crossed :-)

Btw. What about my Erpms limits. Wich i think is default numbers. They are okay ?
```

---
## \#7 Posted by: rpn314 Posted at: 2017-06-24T02:23:25.628Z Reads: 106

```
You could set the ERPM to -60,000 and 60,000 to be safe, but it looks like you're running a 6s system, so as long as you have a motor kv under 300ish, I doubt it would really change anything.
```

---
## \#8 Posted by: Silverline Posted at: 2017-06-24T15:29:28.601Z Reads: 97

```
Thanks

Yes exactly a 6s Lipo setup
I wil set the Erpm to 60.000 just in case :slight_smile:

Btw.  Battery cutoff start and end. What is that exactly ? And what numbers with 6s lipo setup ?

And one more.
When im building racing drones, can i in the software GUI change my throttle curve. Is this possible in the BLDC tool as well ? I`m a newbee, so i don`t want to fast acceleration from 0 mph / kmph to lets say 50 % throttle.
If i dont want 100 % top speed when going full throttle on my remote, is it just a matter of changing the PPM max number, so instead of 100 % when full throttle i have eg. 70 %
```

---
## \#9 Posted by: rpn314 Posted at: 2017-06-24T15:40:30.901Z Reads: 93

```
I'll let you search around for 6s cutoff settings. I'm sure you'll find them ;)

That's awesome! Drones may be my next tinkering project.
I completely understand what you're saying. The BLDC tool that Vedder built does not have throttle curves. However @Ackmaniac's firmware and modifed BLDC tool do, so I'd check that out :slight_smile:
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#10 Posted by: Silverline Posted at: 2017-06-24T17:09:17.876Z Reads: 74

```
Cool thanks........

OMG..... Back from my first riding, with my new VESC..... this esc is sooooooo much better than stock esc, like crazy better. I dont think i need different throttle curve, because the throttle curve and throttle response on the vesc vs. stock esc is soooo much better.

Damn, this is the best thing to do with a chineese E-board.....

Btw. Flying fpv  with racing drones, is something everybody should try.
```

---
