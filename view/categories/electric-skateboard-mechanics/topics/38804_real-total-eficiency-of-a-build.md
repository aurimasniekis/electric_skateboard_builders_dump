# Real total eficiency of a build?

### Replies: 7 Views: 777

## \#1 Posted by: josep Posted at: 2017-11-20T10:06:47.440Z Reads: 104

```

Has anyone tested the real eficiency of any motor?

Lets see this theoretical example:

According to physics, if you want to climb a slope 5 km long 500 m of height in 15 min (which means at 20 km/h) you need a constant power of 500 W. That's considering no energy losses at all by air or ground friction, heat production and drive train efficiency. That's calculated for a total weight of 90 kg.

If you add a theoretical total efeciency of 75% the power needed for that would increase to 667 W (0.89 hp).

But does anyone have any experimental data about the real total eficiency of his build?
```

---
## \#2 Posted by: Youssless Posted at: 2017-11-20T10:11:09.649Z Reads: 101

```
I'd imagine we could get enough data from the telemetry apps and work out efficiency but we'd need coefficient of friction, rider mass and air resistance if we want to get to a good enough estimate I believe.
```

---
## \#3 Posted by: josep Posted at: 2017-11-20T10:49:11.746Z Reads: 91

```
Sorry, I did the calculations for 90 kg of total mass. I have just added it to the original post. And that leads to my other question: if I only need 667 watts to climb that hill at 20 km/h (which is a 10% climb ratio), why do we use such overkill 3000W motors? With this example, if we required such power to achieve the same results that would mean the real total eficiency of the build is 17%.
```

---
## \#4 Posted by: Youssless Posted at: 2017-11-20T10:59:04.141Z Reads: 86

```
3kW is the maximum capacity of the motor's output, no? 

During rides you won't usually see that high of a W output. I think for efficiency we need to calculate the power delivered to the motor by the ESC and the real world power output and calculate the efficiency from there?

You'd end up calculating efficiency as Average Real World Power *100 / Average ESC Power. The ESC power is relatively easy to acquire from a run whilst the the ARWP would be more difficult unless you're working in a closed system, i.e. indoors.
```

---
## \#5 Posted by: josep Posted at: 2017-11-20T11:48:47.098Z Reads: 75

```
Yes, I think you are right.

So, why I have read many times that for my weight (85 kg) a single 63 mm motor will NOT be enough to climb hills at 20 km/h? Theoretically, with a 2000W motor there should be more than enough. I don't understand it?
```

---
## \#6 Posted by: Youssless Posted at: 2017-11-20T12:30:18.115Z Reads: 61

```
I believe here they're referring to torque. For reference, I uses a6374 192KV motor with 15/36T gearing. At 90kg load I climb moderate hills decently and hit 30mph.

Here is some reading material you might want to check out (though they don't directly answer your question I think you can find resolve in them):

https://www.electric-skateboard.builders/t/how-does-the-torque-curve-change-with-voltage/25760/6

https://www.electric-skateboard.builders/t/does-lower-kv-really-mean-more-torque/4529/3
```

---
## \#7 Posted by: pat.speed Posted at: 2017-11-20T12:31:53.173Z Reads: 56

```
Yes I don't understand why people say this. In most cases a single motor board is more than enough power to get you going at a good speed and climb moderate hills with ease
```

---
