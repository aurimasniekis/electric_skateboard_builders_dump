# What should be the BLDC tool values for this setup?

### Replies: 11 Views: 1493

## \#1 Posted by: orkunturkey Posted at: 2017-09-26T08:32:47.574Z Reads: 87

```
I have a dual hub motor, VESC 2.54 and 8S3P lithium battery setup. Here are the spec sheets I got from the manufacturers. Not so much other info regarding the parts since I was getting them from a chinese supplier. What do you suggest for my BLDC tool values for this setup?

<img src="/uploads/db1493/original/3X/1/e/1eab5e9453bee428f8ba5be68031ca26544afb4b.JPG" width="358" height="496">

<img src="/uploads/db1493/original/3X/b/0/b0dc0c4a0fd6de0ec26c52fb2f2a8f0b7fcc340f.jpg" width="600" height="331">
```

---
## \#2 Posted by: orkunturkey Posted at: 2017-09-29T09:14:06.985Z Reads: 68

```
Still looking for those values, anyone?
```

---
## \#3 Posted by: scepterr Posted at: 2017-09-29T09:20:02.773Z Reads: 72

```
You "setup" the vesc to get those values
Run motor detection, etc
https://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500
```

---
## \#4 Posted by: DeathCookies Posted at: 2017-09-29T09:21:46.081Z Reads: 72

```
P = U * I
Watt = Volt * Ampere

600 Watt Motor = 36 Volt Motor * Battery amp     | :36V
600 / 36 = A

A = 16

You should set battery max to 16A
Am i wrong?
```

---
## \#5 Posted by: scepterr Posted at: 2017-09-29T09:22:49.822Z Reads: 63

```
battery current is not motor current
```

---
## \#6 Posted by: DeathCookies Posted at: 2017-09-29T09:27:10.402Z Reads: 66

```
Then he would Need to set?

Motor max: 16
battery max: 16

That way he would not exceed the Power of the hubs.
```

---
## \#7 Posted by: scepterr Posted at: 2017-09-29T09:31:35.539Z Reads: 63

```
Don't know what batteries he has so nothing to base batt max on and again battery current and motor current are separate
https://www.electric-skateboard.builders/t/focing-around-weak-brakes-and-cutout/33203/66?u=scepterr
https://www.electric-skateboard.builders/t/what-does-motor-max-actually-means/8292/
```

---
## \#8 Posted by: DeathCookies Posted at: 2017-09-29T09:37:54.544Z Reads: 59

```
[quote="scepterr, post:7, topic:33983"]
so nothing to base batt max on
[/quote]

Well, his Motor can only run up to 600W
His Motor max can only be 16A.
Therefor his battery max should be at max at 16A. It does not make sense if he set up battery max to 50A because Motor max will constraint it.... 

it is not necessary to use the same battery max as Motor max but it is another safety Feature you can add
```

---
## \#9 Posted by: scepterr Posted at: 2017-09-29T09:38:57.986Z Reads: 50

```
Read this please
https://www.electric-skateboard.builders/t/focing-around-weak-brakes-and-cutout/33203/66?u=scepterr
```

---
## \#10 Posted by: DeathCookies Posted at: 2017-09-29T10:31:02.782Z Reads: 46

```
90% duty cycle
Battery 40V  36A
Motor   36V  40A


10% duty cycle
Battery 40V   4A
Motor    4V  40A


Result: the battery max does not exceed the Motor max. it cannot because the duty cycle will never be 100%. there is always some loss.
So i would set Motor max to 16A (when using 10S) and battery max to 16A or lower.
```

---
## \#11 Posted by: orkunturkey Posted at: 2017-11-14T10:55:20.070Z Reads: 32

```
Sorry for the late reply. What would you suggest for a 7s3p battery?
```

---
