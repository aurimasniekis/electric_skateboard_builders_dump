# VESC clocking on slow acceleration

### Replies: 9 Views: 1252

## \#1 Posted by: devilpiggy38 Posted at: 2016-08-14T10:06:19.901Z Reads: 117

```
Continuing the discussion from [Finishing my build (VESCs arrived after 2 months wait)](http://www.electric-skateboard.builders/t/finishing-my-build-vescs-arrived-after-2-months-wait/7593/7):

VESC clocking on slow acceleration (https://www.youtube.com/watch?v=s2pibu1YK00)

can anyone help?
```

---
## \#2 Posted by: chaka Posted at: 2016-08-14T16:13:55.338Z Reads: 94

```
Haha, thats normal. You have the throttle so low that the signal is flickering. The VESC operates on current control so you really should only judge the performance underfoot. Bench testing will almost always result in the motors winding up to max rpm without any load.
```

---
## \#3 Posted by: devilpiggy38 Posted at: 2016-08-15T15:49:42.449Z Reads: 79

```
Thanks Chaka. 

The thing is when i stand on the board with my body load, there are still some minor clocking of the motor moving off from standstill. Is this consider normal?
```

---
## \#4 Posted by: chaka Posted at: 2016-08-15T16:07:06.762Z Reads: 70

```
If running without sensors it is completely normal. I naturally give one kick to start, any amount of forward movement helps get things going.  The vesc takes measurements in order to establish a pole position, a slight foward motion is all that is needed to get things going. 

Quick question, what is your "max current ramp step" set at? You will find it on the advanced tab within motor configuration.
```

---
## \#5 Posted by: devilpiggy38 Posted at: 2016-08-15T16:21:16.746Z Reads: 59

```
Hi chaka, I had done a step up test from 0.03 all the way up to 0.09. it is now staying at 0.09 with not much improvement on the clocking.
```

---
## \#6 Posted by: chaka Posted at: 2016-08-15T16:48:16.256Z Reads: 57

```
Once it is rolling it runs fine right? It could be that you are just being too light on the throttle. If it bugs you too much and you need to start from a dead stop then you may want to think about getting a sensored motor.
```

---
## \#7 Posted by: devilpiggy38 Posted at: 2016-08-15T17:30:35.494Z Reads: 57

```
Thanks chaka， you are absolutely right once it start to roll, , it's fine and performance was awesome. Just asking the forum members is this clocking normal ? and btw, I can live with this minor clocking issue, no big deal.

Thanks for all the answers.
```

---
## \#8 Posted by: chaka Posted at: 2016-08-15T17:34:19.104Z Reads: 57

```
I have noticed less "cogging" if I lower the "max current ramp step" to .004 but you end up with a little less performance, softer response, I don't recommend it..

 Doing a little jig to get the wheels going as you apply throttle is all that is really needed and will become instinct overtime. ;)
```

---
## \#9 Posted by: sl33py Posted at: 2016-08-15T17:35:17.812Z Reads: 55

```
we usually call this "cogging" or "stuttering" on start.  It's an issue for almost all non-sensored setups as the motor can't detect rotation until it gets started.  VESC has some of the best/smoothest starts IMO - even unsensored.  Most Hobby/RC ESC's are really bad in comparison.  Most give a good kick start and it's little/no-issue.

There may be some adjustments in the VESC you can try - or just kick once and then go.
```

---
