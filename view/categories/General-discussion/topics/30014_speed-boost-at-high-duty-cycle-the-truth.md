# Speed Boost at High Duty Cycle. The Truth

### Replies: 23 Views: 1203

## \#1 Posted by: pshaw Posted at: 2017-08-08T01:54:40.337Z Reads: 161

```
I have been doing a bunch of reading on this topic as it has been plaguing me on my setups and I've been trying to figure out what is going on. I just wanted to post this so we can have a clear and concise answer on why it is happening, what setups it affects, and is there a solution.

Why is it happening? This speed boost you feel is due to noise on the current sensor which creates bad readings inducing a "boost" that can often be really startling if you aren't expecting it. 

What setups? This I'm not sure on. At one time I thought FOC was the only mode that didn't do it but that doesn't make sense because it is simply a basic hardware issue. So I'm thinking it will affect all setups. Can someone confirm or deny this?

Is there a solution? Form what I've gathered you can limit your duty cycle to .85 or so which will completely get rid of the solution, but will I think reduce your top speed as well. The other option is I believe to buy vesc 6, which I believe is the only vesc out there that doesn't have the issue with the current sensors. 

You gurus jump in here and please add on to this so we can have a better understanding.
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-08-08T01:57:37.203Z Reads: 162

```
I bet @Ackmaniac's firmware will help that. Not totally sure but seems like it might help
```

---
## \#3 Posted by: pshaw Posted at: 2017-08-08T02:00:43.437Z Reads: 158

```
[quote="GrecoMan, post:2, topic:30014, full:true"]
I bet @Ackmaniac's firmware will help that. Not totally sure but seems like it might help
[/quote]

It's a hardware issue so his firmware doesn't get rid of the problem unfortunately (I'm running his currently)
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-08-08T02:02:55.436Z Reads: 147

```
Ah, I'm running his too and it hasn't been a problem for me.  There is a very small amount of kick when I hit max efficiency but nothing that you will notice unless your trying to feel it.  Maybe it isn't such a problem on higher kV motors?  I'm using the NTM Propdrive V2 270kV
```

---
## \#5 Posted by: pshaw Posted at: 2017-08-08T02:03:50.608Z Reads: 139

```
I'm on dual 6374 on 12S and when it happens it almost knocks me off at close to 30mph. It's really brutal haha
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-08T02:12:14.430Z Reads: 131

```
This will happen on all vesc 4's. It's an inherent hardware bug, and i believe it's addressed in the vesc 6
```

---
## \#7 Posted by: pshaw Posted at: 2017-08-08T02:16:49.634Z Reads: 132

```
The current default control loop is 2000hz I believe. Do you think we can lower the control loop time so that we can increase the sample rate? This in theory should smooth everything out and reduce the noise on the current sensor and hopefully get rid of the high duty cycle boost everyone is experiencing. 

Thoughts?
```

---
## \#8 Posted by: JdogAwesome Posted at: 2017-08-08T02:18:45.628Z Reads: 125

```
I haven't ever experienced this bug and im running a single Carvon V1 Hub motor that I believe has a Kv of like 100 I think.
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-08T02:19:47.043Z Reads: 129

```
That's interesting, i wonder if this issue is exclusive to higher erpms and not necessarily duty cycle.
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-08-08T02:21:17.687Z Reads: 128

```
Yea because I've got the vesc 4.12 and haven't had anything even come close to throwing me off the board
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-08-08T02:22:03.677Z Reads: 126

```
The highest erpm I've ever gotten with my current setup is only about 45k
```

---
## \#12 Posted by: lrdesigns Posted at: 2017-08-08T03:16:56.177Z Reads: 120

```
I found a slightly lower gear ratio, like a bit larger motor pulley really smoothed out the power delivery. Secondly I think if you reduce the current ramp step from default .04 it will smooth out acceleration.  And thirdly reducing battery amps can help while keeping motor amps high will make it much more manageable while still giving low speed power.
```

---
## \#13 Posted by: racidon Posted at: 2017-08-08T03:26:20.362Z Reads: 112

```
I've never had this issue either on single drive Rspec3
```

---
## \#14 Posted by: SORRENTINO Posted at: 2017-08-08T03:35:43.306Z Reads: 110

```
This happen to me on my single 6374 149kv. Maybe it's a 6374 thing?
```

---
## \#15 Posted by: Jinra Posted at: 2017-08-08T04:02:40.740Z Reads: 104

```
Nope, happens on my 6355's and 5065's as well. Though less, or less noticeable on my 6355
```

---
## \#16 Posted by: longhairedboy Posted at: 2017-08-08T04:08:14.880Z Reads: 98

```
We're talking about when the V-TECH kicks in right? I don't know, i kind of like it. I haven't noticed it too much on the VESC-Xs I've been using though. I'm not calling the FocBoxes because i've had them since before that unholy ruckus.  

I thought it was caused by the motors reaching their peak efficiency and therefore popping a little burst of power to the ground. I didn't realize it was literally just a hardware bug. I haven't had a lot of time to read about this issue, just been living with it for the past three years.
```

---
## \#17 Posted by: lrdesigns Posted at: 2017-08-08T04:14:12.765Z Reads: 97

```
[quote="SORRENTINO, post:14, topic:30014"]
Maybe it's a 6374 thing
[/quote]

I had it real bad on dual 5065 270kv with 4:1 gearing. Now same setup with 2:1 gearing and 140kv motors its completely gone. Though I now run @Ackmaniac watt mode firmware and lower battery amps.  On the original setup I went from 4:1 to 3.2:1 and found the power delivery was much smoother, and also the boost was more manageable.
```

---
## \#18 Posted by: pshaw Posted at: 2017-08-08T15:17:25.107Z Reads: 87

```
[quote="longhairedboy, post:16, topic:30014, full:true"]
We're talking about when the V-TECH kicks in right? I don't know, i kind of like it. I haven't noticed it too much on the VESC-Xs I've been using though. I'm not calling the FocBoxes because i've had them since before that unholy ruckus.  

I thought it was caused by the motors reaching their peak efficiency and therefore popping a little burst of power to the ground. I didn't realize it was literally just a hardware bug. I haven't had a lot of time to read about this issue, just been living with it for the past three years.
[/quote]

Exactly what I'm talking about :) 

Maybe it's my settings or physical board setup but it hits so hard that it seems actually pretty tough to control. Not sure if this kind of jolt you can get used to with time :/

Look at the jump... 89% duty cycle straight to 95%

<img src="/uploads/db1493/original/3X/9/6/96a49a97316d8e474f48fcea3e209495a79edc96.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/f/d/fdda1f6529968415deb52ce447186fb8e8143d44.PNG" width="281" height="500">
```

---
## \#19 Posted by: longhairedboy Posted at: 2017-08-08T16:24:16.892Z Reads: 73

```
oh damn yeah that's enough to throw you back a little for sure. ass on the street time.
```

---
## \#20 Posted by: pshaw Posted at: 2017-08-08T16:42:27.897Z Reads: 71

```
Haha yeah! So are the only two fixes to limit max current ramp or to buy a crazy expensive vesc 6?
```

---
## \#21 Posted by: pshaw Posted at: 2017-08-10T17:32:16.929Z Reads: 61

```
Little update here for you guys. I set my max watts to 1300 per motor and I never got the speed boost. I think it because I never hit the duty cycle jump.
```

---
## \#22 Posted by: Jinra Posted at: 2017-08-10T18:04:38.302Z Reads: 61

```
You should still ramp up to full duty cycle with that limit set. I wonder what actually causes it.. I barely ever feel it on my dual 6355 build.
```

---
## \#23 Posted by: pshaw Posted at: 2017-08-10T19:40:16.914Z Reads: 53

```
82 was the max I saw from 23miles of riding last night.... Would flooring it uphill yield a higher duty cycle than on level ground all things being equal?
```

---
