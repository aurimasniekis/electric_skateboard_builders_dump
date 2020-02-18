# Board going slow when I&rsquo;m on it

### Replies: 8 Views: 282

## \#1 Posted by: Sapphirinia Posted at: 2019-02-28T23:29:10.545Z Reads: 126

```
My quick search didn't help, so I recently replaced my broken vesc with a focbox and it seemed alright. I got all the kinks out where the belts no longer slipping off, replacement remote actually works (as long as I don't squeeze too hard), and stuff is stable. But again, I just did some adjustments and rode it and it. An barely move me while I'm on it. I'm assuming it's a focbox setting issue. I did the motor detection and kept most default settings. But this same board with a vesc and same battery setup got me easily 24mph. Which settings should I be looking at to fix this.


Quick question version: which settings control power to push the board?
```

---
## \#2 Posted by: b264 Posted at: 2019-02-28T23:31:16.716Z Reads: 120

```
"Motor current max" controls power at low speed and "Battery current max" controls power at high speed but this sounds more like a PWM / PPM problem where your throttle isn't hitting 100%
```

---
## \#3 Posted by: Sapphirinia Posted at: 2019-02-28T23:41:30.954Z Reads: 110

```
You're probably right. Just adjusted that setting. Going to try it out. Thanks
```

---
## \#4 Posted by: lrdesigns Posted at: 2019-03-01T01:21:53.979Z Reads: 91

```
Seen a few people with this symptom, in those case the battery cut off voltage was wrong. So the vesc was in battery protect mode. 

Go to General / voltage, set voltage cut off relative to your cell number.

How many cells is your pack?

Oh man I cant upload images at the moment. Says its full. 

Or also the minium and maximum voltage but leave this defualt 8v and 57v.
```

---
## \#5 Posted by: Sapphirinia Posted at: 2019-03-01T03:09:05.984Z Reads: 74

```
I tried uploading my settings and it wouldn't let me either. But it was the throttle control settings
```

---
## \#6 Posted by: Sender Posted at: 2019-03-01T03:20:57.643Z Reads: 66

```
Yeah, the forum is acting funky right now. 

As soon as you post them up we will get on it. My guess is one of the things already suggested.

Following this thread now for updates and I will help out if I can.

We will get it sorted!
```

---
## \#7 Posted by: Andy87 Posted at: 2019-03-01T04:08:35.032Z Reads: 55

```
Besides the things all others already said, check your battery to focbox connected and loop key, in case you have one.
I once had this issue as the loopkey was plugged in only 80%. With it the vescs worked only in the reduced power mode, like battery cut off mode.
```

---
## \#8 Posted by: buildityourself Posted at: 2019-03-06T23:52:28.044Z Reads: 22

```
So I seem to be having the same issue where yesterday my board was flying and now it barely moves. I may have messed up my vesc settings yesterday but i don't know which. I believe my motor settings are correct. I looked into the settings for the remote and the tests say that I am hitting 100% but yet it is still slow. What does PPM/PWM mean? Can I change something else to fix this?

This is what it looks like ![2019-03-06|690x387](upload://wc5VJLaUaxvElpeM3eDSkzl0jtv.jpeg)
```

---
