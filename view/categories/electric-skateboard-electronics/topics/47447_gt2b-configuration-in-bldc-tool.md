# GT2B Configuration in BLDC Tool

### Replies: 9 Views: 519

## \#1 Posted by: butt_stallion Posted at: 2018-02-25T21:13:49.173Z Reads: 75

```
So, I have been trying to configure my GT2B controller in the BLDC tool.  I set it so that the throttle trim is at 50% and then pulled the trigger and typed in the value and did the same for the brake.  But then when I write the configuration the value on the display jumps to like 65% and the throttle doesn't work, but when I push forwards the motor starts to spins up to full throttle.  I can't figure out what the perfect setting.  

I don't know if the images will help but those are what the pulse width ranges should be.

![ControllerMax|690x459](upload://uIiAitpForOxDGgBvTPP3hPIgMB.PNG)

![ControllerMin|690x440](upload://gLFJvzRDCZmXmdOW4aHvXTa86TY.PNG)
```

---
## \#2 Posted by: mccloed Posted at: 2018-02-25T21:22:44.178Z Reads: 57

```
Two things: 1. On the bench(without load)the VESC will go full throttle with very little trigger. 2. You need to mess with the Max/Min pulse width settings until you are at 50% with no movement of the trigger.
```

---
## \#3 Posted by: butt_stallion Posted at: 2018-02-25T21:32:04.585Z Reads: 57

```
Okay, so that's it?  I thought you had to pull the trigger to set the Max/Min?
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-02-25T21:41:50.336Z Reads: 51

```
there’s a switch on the gt2b called “reverse throttle” or something like that. flip it
```

---
## \#5 Posted by: butt_stallion Posted at: 2018-02-25T21:46:31.423Z Reads: 49

```
It only does that when I set the minimum pulse width below 1 ms though
```

---
## \#6 Posted by: GrecoMan Posted at: 2018-02-25T21:47:56.363Z Reads: 47

```
does what...
```

---
## \#7 Posted by: butt_stallion Posted at: 2018-02-25T21:49:44.223Z Reads: 47

```
The thing I described in my original post.  When I set the min below 1 ms the throttle stops working and when I push it forward (for the brake) it goes full throttle and doesn't stop unless I disconnect the battery.
```

---
## \#8 Posted by: mmaner Posted at: 2018-02-26T03:04:58.760Z Reads: 39

```
[quote="GrecoMan, post:4, topic:47447, full:true"]
there’s a switch on the gt2b called “reverse throttle” or something like that. flip it
[/quote]

Yeah, flip it then remove it. 😀

My very first esk8, a santa Cruz 30in bad hand double kick...I used a gt2b.  I built it, everything tested fine, jumped on it and hit the trigger.  

End result was me on my ass and the board 40 feet behind me.  I started working slower and learned the proper wheel roratiin after that.
```

---
## \#9 Posted by: butt_stallion Posted at: 2018-03-16T23:23:35.198Z Reads: 24

```
I finally got a chance to try this.  I set the max and min limits and flipped the switch, but that didn't fix it.  The motor just starts going full throttle and doesn't stop unless I unplug it.
```

---
