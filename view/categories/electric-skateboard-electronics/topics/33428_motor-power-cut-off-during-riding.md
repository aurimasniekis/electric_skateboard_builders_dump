# Motor power cut off during riding

### Replies: 8 Views: 488

## \#1 Posted by: wald.adrien Posted at: 2017-09-18T18:21:45.015Z Reads: 71

```
Hello all,

I have a problem with my motor losing power whilst I'm accelerating. Once I let go of the trigger and press it down again to accelerate it works again immediately. This happened relatively frequently to me yesterday. Going uphill did not significantly increase these cut offs as far as I can tell, but I was also going slower and not throttling as hard. I think the problem is due to my VESC settings, in particular the hard limits I set. Could someone with expertise in the subject please look over my VESC settings? My setup is: 10s4p pack with 18650 cells, one 6374 190kv sensored BLDC motor with a gear ratio of 15:36, Maytech VESC50A. If you want more information about the problem or have any other ideas as to what may be causing this let me know.

Thanks so much for your help!

<img src="/uploads/db1493/original/3X/4/7/47159096f080ee681b3e711540b37b6b8f38f74c.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/1/c1a08c145cd6128359bd383b75415fb99a3fb5f9.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/9/c92ac140168e321443972f4cd9223b982053828e.png" width="690" height="431"><img src="/uploads/db1493/original/3X/b/6/b6e242b8143b2fd467c735090ec7b4e8baf68510.png" width="689" height="431">
```

---
## \#2 Posted by: Bloop Posted at: 2017-09-18T20:17:10.093Z Reads: 54

```
Not an expert but i see you have in App configuration tab -> PPM  the RPM limit . And my guess is that you rich 30k ERPM when you are accelerating hard so the vesc is cutting you off.

Also i saw you have the battery cutoff start and end really low.. i would set it up 33V 30V or 30V 27V would be some better values.
```

---
## \#3 Posted by: Bloop Posted at: 2017-09-18T20:20:03.194Z Reads: 53

```
Also in Motor Configuration -> Motor in the right part set the RPM Limits to + - 60 000 more than that and you will fry your vesc.
```

---
## \#4 Posted by: wald.adrien Posted at: 2017-09-19T12:15:06.717Z Reads: 42

```
So I changed some settings. Motor max and min are +-40 now. Bat max to 45 so I don't fry the VESC. Battery cutoff at 34-33 now so I get longer battery life. Now I realised yesterday that I was running in sensorless mode when I was supposed to be or rather wanted to be in sensored. Applied all these settings. Still the problem persists. I will check my wire connections again but they were all good. I also don't think it's the ERPM limit because that just sets a top speed and doesn't actually cut the motors power when the limit is reached. It's just so I don't go too fast in the beginning.
```

---
## \#5 Posted by: pat.speed Posted at: 2017-09-19T12:24:24.076Z Reads: 35

```
Well it could be the erpm limit becuse it might be cutting your power to stop you from going over the limit. Try setting it to 50,000 or 60,000 but NO higher
```

---
## \#6 Posted by: wald.adrien Posted at: 2017-09-19T12:36:28.762Z Reads: 32

```
Ok I will give that a shot and report back. Unfortunately raining right now so I can't ride :(
```

---
## \#7 Posted by: Bloop Posted at: 2017-09-19T12:45:17.725Z Reads: 30

```
but can you reproduce it on bench ? flip the board and easily push the throttle you should hit the erpm without a problem. Also check the live graph on bldc tool and see there what is the erpm the motor is getting too. 

If you have the erpm set to 30k and your motor spins faster than that and not stoping well :-?? idk then .
```

---
## \#8 Posted by: wald.adrien Posted at: 2017-09-19T14:30:34.849Z Reads: 27

```
No that's also a noteworthy thing. I can't reproduce it on the bench. When there's no pressure on the wheel, it just spins until it reaches the ERPM limit and keeps spinning without fault. It's only when I'm accelerating and I haven't even reached the ERPM limit (because it's still accelerating) that it cuts off the power. Probably might cut off when I am at max speed too, but I haven't dared to reach it because I'm afraid I will lose my balance if the motor loses power.
```

---
