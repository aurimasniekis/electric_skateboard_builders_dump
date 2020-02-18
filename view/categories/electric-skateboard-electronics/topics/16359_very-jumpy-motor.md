# Very Jumpy Motor

### Replies: 5 Views: 596

## \#1 Posted by: Zoomy Posted at: 2017-01-20T02:30:28.295Z Reads: 99

```
Hi there, so I got my board up and running for the first time a few days ago. On the first day of riding I got half way through climbing quite a steep hill and all of a sudden all power cut off even though I have all slow cut off settings for temp and voltage... so I thought this was very odd. After jumping off the board I tested it with a bit of throttle and it worked as normal with no more problems. 

On my second day of riding, I noticed that whenever I would climb a hill for more than about 10 seconds or so the board would loose power for a split second maybe once or twice but carry on. 

Later that day I was accelerating very slowly from a stand still and similarly to before, it lost power for a split second, except this time it happened multiple times like it was stuttering. This was the first time it happened at a slow speed.

After checking over my configuration in the bldc tool and finding nothing that jumped out at me I gave it another shot but this time the cutting in and out was severe. It would cut in and out on flat ground even without me on the board! and additionally would accelerate hard or put on brakes randomly, both for a split second which made it impossible to even stand on.  

If I just push off with no throttle it brakes randomly and with the board on the bench, the motor runs completely freely with no stuttering.

My remote doesn't seem to be the cause as through the bldc tool I could see that the throttle signal held very steady.
I've pulled apart the motor but to my knowledge couldn't see any signs of shorting.
While the board was on the bench I shock around each component individually to see if vibration was the cause but the motor still ran smoothly. 
I increased the max input voltage which didn't fix it.

My setup is 

vesc 4.12
gt2b flysky
6s lipo
alien power systems 170kv 3300w 

In the bldc tool the window is cut at the bottom where I would normally be able to see the fault code if there was one. I'm planning on getting a bluetooth module so I can see if there's a fault code and also to look at whats happening when it stutters. 

If anyone has any ideas i'd appreciate it because i'm lost.
```

---
## \#2 Posted by: mmaner Posted at: 2017-01-20T03:32:17.465Z Reads: 78

```
The best way to get help with a VESC is post screen shots of BLDC Tool windows. 

Increase your resolution if you need too.  Go to the terminal window, type fault and post the results.
```

---
## \#3 Posted by: Zoomy Posted at: 2017-01-20T03:46:25.437Z Reads: 76

```
I just hand another fiddle around and think I found the problem :smile: It seems like the white wire coming from the receiver is the culprit!  

Ill post results once I fix or replace it.
```

---
## \#4 Posted by: filipandre95 Posted at: 2017-08-04T20:54:06.611Z Reads: 32

```
Did you fix it? I have the same problem and it started after trying to climb a steep hill and the power cut off. My board now randomly brakes at any time at any surface...
```

---
## \#5 Posted by: Zoomy Posted at: 2017-08-05T00:47:28.759Z Reads: 25

```
Hi, the white wire was half way out of my receiver conector. I pushed it back in and added some hot glue to keep it there and it's been good to me since.
```

---
