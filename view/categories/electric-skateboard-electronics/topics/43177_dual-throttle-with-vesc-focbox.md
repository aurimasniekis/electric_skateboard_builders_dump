# Dual throttle with VESC/FOCBOX?

### Replies: 3 Views: 609

## \#1 Posted by: SOICDIP Posted at: 2018-01-08T11:40:50.373Z Reads: 99

```
I'm planning to have two throttles for my kick scooter, one for accelerating and another for breaking, as shown in this video:

https://youtu.be/PPyHvkypKjo?t=12m34s

Tom is using a VESC6 but I'm not sure how to wire two analog throttles into a VESC. I think both the VESC4 and 6 have a single input for PPM or an analog throttle.

Maybe he's using an Arduino to combine the two and send it as a PWM servo signal to the VESC? I wonder where this "second input" in the speed controller is, which he mentions at 12:48.
```

---
## \#2 Posted by: Blasto Posted at: 2018-01-08T15:57:16.133Z Reads: 71

```
Didn’t look at the video, but there’s two ADC inputs on hw 4.12 and hw 6.xx. If he is using a twist throttle he is using the ADC inputs and not ppm
```

---
## \#3 Posted by: SOICDIP Posted at: 2018-01-08T18:22:44.372Z Reads: 54

```
Ah, found the second ADC header. Thanks.
<img src="/uploads/db1493/original/3X/e/7/e7c2aad4ffa8048c65ce66e0c40bfe4b87c0d22d.PNG" width="477" height="500">
```

---
