# Abrupt control, possible remote issue?

### Replies: 6 Views: 186

## \#1 Posted by: chickengun Posted at: 2019-04-22T17:12:33.961Z Reads: 60

```
So I was test riding my first build (10s4p, Bestech [HCX-D223V1](http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html), 2x Vanda Vesc 4.21, [Dual HUB Motor](http://www.diyeboard.com/dual-hub-motor-9052mm-1000w75kv-power-truck-front-truck-kit-p-558.html)) and the control is anything else than smooth. Both motors are connected over CAN bus and I am using the firefly receiver and remote, both working without connection issues. My min value at the firefly remote is 355, center 515 and max 655.

In the vesc tool's input setup I noticed that my pulselength min is 0.15, center 0.7 and max 0.95. Do you think the difference between center and max should be the same as center and min? When I only accelerate a tiny bit on the firefly remote (~10%) it goes quite fast to 100% motor speed. For that reason I adjusted the throttle curve to -30% for braking and acceleration:

![image|690x428](upload://2r2qsMMoIw7YJjnvDJHUNNUNqQp.png) 

It helps to have a smooth start but as I am riding it is still very difficult to control the speed, not smooth at all.

I have tried in the past to use the recent firmware 3.52 but I failed because I didn't manage to let both motors spin for some unknown reason, [here is the thread about this issue](https://www.electric-skateboard.builders/t/setup-two-vanda-vescs/91234/9). So for now I am sticking with FW 3.40

What do you think is the problem? Thanks!
```

---
## \#2 Posted by: olestra Posted at: 2019-04-22T17:29:51.588Z Reads: 48

```
did you run the 'setup input wizard' found under "welcome and wizards"?
```

---
## \#3 Posted by: chickengun Posted at: 2019-04-22T17:31:53.799Z Reads: 47

```
Yes that is what I did
```

---
## \#4 Posted by: chickengun Posted at: 2019-04-23T19:43:45.217Z Reads: 26

```
so first thing I noticed is that I didn't place the hall sensor on my firefly remote directly below the magnets. Now I get values from 0 to 1023. Anyways, the problem is not the remote, it is the receiver. Haven't solved it yet.
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-04-23T19:53:15.346Z Reads: 21

```
Now that you've changed the magnet placement in the remote, you may need to re-pair it with the receiver and redo your input setup.
```

---
## \#6 Posted by: chickengun Posted at: 2019-04-23T21:05:00.969Z Reads: 18

```
I did. I even inverted the magnets, same issue. The remote is sending values between 0 and 1023 to the receiver which is good. It is a receiver issue I guess.
```

---
