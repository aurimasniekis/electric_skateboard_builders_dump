# Vesc 4.12 bldc restricted

### Replies: 7 Views: 237

## \#1 Posted by: Moza Posted at: 2018-08-24T16:36:53.156Z Reads: 85

```
Hi guys.

I have a razor e300 scooter running esk8 vesc 4.12. Running with a keda 190kv outrunner, 10s6p battery. (Gear ratio has been increased for acceleration)

I've been running on foc for first dozen rides and its fast! Anyhow, I've recently tried out bldc.

For some reason bldc is really down on power compared to foc.

All settings are the same, ie 
motor max is 80a
Battery max is 45a
Power max is 2000w
![Screenshot_20180824-172729|281x500](upload://qogPWfr1wgqqZ6U6e2uJhUIDDik.png)
There's no restrictions according to the graph but  the motor is not pulling enough amps.

Below are the same settings but in foc mode

![Screenshot_20180824-174004|281x500](upload://88o7RRMcZCQXNPyrrT8W9sUKqro.png)

Anyone have any ideas ?

Thanks in advance. 
Steve
```

---
## \#2 Posted by: mccloed Posted at: 2018-08-24T17:30:56.838Z Reads: 58

```
Idea: Leave it in FOC! :grin: I just recently changed my board back to BLDC to see if it resolved an issue I was having. I ended up going back to FOC. It's just more powerful. You loose a little top end speed but its worht the loss, in my opinion.
```

---
## \#3 Posted by: Moza Posted at: 2018-08-24T17:41:05.682Z Reads: 61

```
Not helpfull 😁! 

I changed it to bldc because I was having problems with foc. 

When I'm free wheeling sometimes I struggle to re-engage throttle. Occasionally I have to roll to a stop and gently feather throttle until it comes back. (Nothing to do with overheating, etc and no faults logged).

There must be a reason why the motor is not pulling many amps in bldc.

I've restricted my top speed because its silly fast so not bothered about top end anyway. It's the acceleration that's fun.
```

---
## \#4 Posted by: mccloed Posted at: 2018-08-24T17:43:50.672Z Reads: 54

```
Have you tried to do another motor detection in FOC? That's where I would start.
```

---
## \#5 Posted by: Moza Posted at: 2018-08-24T17:52:00.667Z Reads: 49

```
Yes I tried. Its a strange problem but I suppose I could live with it.

Problem is when friends have a go they dont know how to deal with it when throttle locks out.

It hasn't done it yet in bldc but I can't cope with the lack of power.

Oh, btw it is back in foc. Lol.
```

---
## \#6 Posted by: xilw3r Posted at: 2018-08-25T10:10:13.523Z Reads: 33

```
You are using the vesc from hobby king? Anny issues besides the magical ones here?

I actually had the same issue with regular 4.12 vesc that was hand soldered. I only used bldc, foc detection did not work at all, not even for R and L parameters.

But in bldc i never saw motor current rise to the top limit that was set.
```

---
## \#7 Posted by: Moza Posted at: 2018-08-25T11:57:10.497Z Reads: 26

```
Yeah, hobby king one is good so far.

I killed the drv on one but that may have been down to user error as I was new to the vesc then.

Only other problem is the throttle issues mentioned above.
```

---
