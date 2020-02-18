# Motor Braking at high speed

### Replies: 12 Views: 1494

## \#1 Posted by: stuxtruth Posted at: 2016-07-29T16:27:49.975Z Reads: 170

```
So I got my board together. Im using a 120A 6S ESC. When I get to around 14mph and try to punch it... the motor locks up. Its hard to describe. My last board did the same thing. But instead this happens intermittently and is just momentary. Any ideas? Could it be that im 230lbs and overloading the motor/esc?

Here's a video of my last board doing it. Different ESC. Different motor. 

https://www.youtube.com/watch?v=r3SGvUxRGtQ
```

---
## \#2 Posted by: TheRedPanda Posted at: 2016-07-29T16:34:45.175Z Reads: 162

```
What battery are you using?

Also this sounds like either the ESC is overheating and stopping the motor or the motor is drawing too much power and tripping an over current protection. 

For a 230lb rider I would highly recommend stepping up your voltage to atleast 8S, 10S would be even better. This will help take you up to higher speed and not put as much heat into your motors/ESC. Dual motors are also always good to have if you're going up hills.
```

---
## \#3 Posted by: Hummie Posted at: 2016-07-29T16:39:12.266Z Reads: 155

```
not true with the higher voltage leading to less heat in the motor but possibly less heat in the esc
```

---
## \#4 Posted by: stuxtruth Posted at: 2016-07-29T16:56:04.678Z Reads: 153

```
I'm running two motors. I think it must be over current protection. I only had one motor hooked up because I haven't received my other esc yet. But 120 amps?? Seems awfully high. 

<img src="/uploads/db1493/original/2X/3/3391b5cae31d5a5eed1e6a8cf1a31490f5192314.jpeg" width="666" height="500">
```

---
## \#5 Posted by: stuxtruth Posted at: 2016-07-29T16:56:39.396Z Reads: 144

```
Also I'm running 6s4p lg he2
```

---
## \#6 Posted by: TheRedPanda Posted at: 2016-07-29T17:00:57.763Z Reads: 142

```
Yeah it definitely shouldn't be tripping the 120A ESC. For your 6S4P are you using a BMS? LG He2s are rated for 20A constant if i remember correctly(can burst higher). I'm not sure if this happens all the time or only after the battery is depleted but if the He2s are depleted passed around 70% full then they might not be outputting the current you need when punching the throttle. This is definitely strange though as the ESC seems to be very unhappy and is making the motor chime and not want to move.
```

---
## \#7 Posted by: stuxtruth Posted at: 2016-08-11T01:43:11.699Z Reads: 109

```
Here is a video of what's going on. 

https://youtu.be/hwQG5sriTAY
```

---
## \#8 Posted by: anon33082420 Posted at: 2016-08-11T04:46:38.399Z Reads: 101

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#9 Posted by: barajabali Posted at: 2016-08-11T05:05:54.040Z Reads: 96

```
Sounds like your motors are pulling more current than your cells can supply at 6s. 

I'd say.
Add more p cells (6p maybe)
Or jump voltage 
Or use different cells with high discharge
```

---
## \#10 Posted by: stuxtruth Posted at: 2016-08-11T22:40:41.563Z Reads: 87

```
My cells should be supplying 80a continuous no? Something's wrong. I think it my be the remote. My last setup used 2 3S lipo batteries with a xerun esc and a single tacon 160. It hauled ass.
```

---
## \#11 Posted by: maxchilton Posted at: 2016-08-11T23:36:14.619Z Reads: 81

```
what is your esc low voltage cutoff setting?
```

---
## \#12 Posted by: stuxtruth Posted at: 2016-08-12T20:11:41.071Z Reads: 74

```
3.4 just to be safe. battery is fully charged right now. I fixed it though. I changed motor timing to "very high" and acceleration to "very high" and it works great now.
```

---
