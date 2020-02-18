# Ollin Motor Clicking

### Replies: 30 Views: 1550

## \#1 Posted by: Jcullinan09 Posted at: 2017-08-29T04:41:18.473Z Reads: 202

```
Hi All,

In as few words as possible, I am having problems with motors clicking when they spin up.

I find this problem peculiar because when I begin to spin up the motors SLOWLY there is no problem. However when the throttle (on the 2.4ghz controller) is pushed QUICKLY, the motors begin to throw a temper tantrum, and click.

I am using:

2 Ollin 5065 200kv motors
2 Ollin 4.12 VESC's - Using vesc firmware (2.18)
1 Enertion SPACE Cell 10s3p
---

<img src="/uploads/db1493/original/3X/d/c/dc4cf1c02b103cd9e99235a1b7f16d04d8dc847c.png" width="690" height="446">

---

https://www.youtube.com/watch?v=iOgCbGaeN3s

--- 
If anyone has any ideas why this is happenning, I would love to know why.

Thanks,
Have a nice day,

John
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-29T04:48:47.359Z Reads: 182

```
try tightening down your pulley to the shaft.
```

---
## \#3 Posted by: Jebe Posted at: 2017-08-29T04:57:21.969Z Reads: 177

```
Is it happening with the drive gear removed ?
I had one that was clicking as well, removed drive gear tried again still there. Ended up just running it and it seems fine now.
Ollin 200kv motor
```

---
## \#4 Posted by: guyguy Posted at: 2017-08-29T17:53:07.981Z Reads: 157

```
Does this happen on load (when you're riding) or only when full throttle it on the bench?
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-08-29T18:11:46.735Z Reads: 152

```
@chaka
Maybe he can help?
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-29T18:15:13.694Z Reads: 143

```
The starting up issue is normal. You need to use sensors if you want smooth start up. You'll have to kick the board to get it going. 

As for the clicking, now that I got to review the video, it could be that your belts are too tight, but you should still check the pulley like I mentioned before.
```

---
## \#7 Posted by: chinzw Posted at: 2017-08-29T18:24:10.352Z Reads: 138

```
That looks like the tracker is stalling, its quite normal when going full throttle from a stop in sensorless mode. You could try increase or reduce the startup boost see if it works better, or you could just go easy on the throttle.
```

---
## \#8 Posted by: Jcullinan09 Posted at: 2017-08-29T20:42:43.757Z Reads: 130

```
First of all thanks everybody for responding, I was at school this afternoon. 

@Jinra Hi thanks for the feedback. Not sure what you mean by tightening the pulley to the shaft. Also, I don't think it has to do with the belts being too tight, in just a moment I'll try to post a video of the motors still clicking even without the wheels on (Standalone motor).

@Jebe What did you end up doing to help stop the motor from clicking?   

@guyguy Yes, The motors click when in full throttle and when there is load present. In fact the only time they do not click is when spinning up slowly, or without any load like in the video. :confused: . 

@GrecoMan Thanks for tagging @chaka He has always been a very reliable member in this community, and I hope he has some time to help with this hiccup.

@chinzw Thanks for some feedback. I'm not sure what the tracker is? Secondly, could you show me where I can adjust the startup boost (in BLDC i'm assuming)?  And I thought I could just go easy on the throttle too, however with even the slightest load on the motors they begin to stall and do what happened on the bench :pensive:
```

---
## \#9 Posted by: Jcullinan09 Posted at: 2017-08-29T20:52:51.118Z Reads: 120

```
Ok. So I took the wheels off, and in as soon as I tried to spin the motors they jammed and smoke began to come out... I believe this is probably from the copper windings melting?:cry: 

I don't even think I should take a video to show this happening as I am afraid of further causing damage. Has this happened to anybody else ever?
```

---
## \#10 Posted by: darkkevind Posted at: 2017-08-29T21:14:07.414Z Reads: 114

```
Is this what happened?

https://youtu.be/13hamBiqeLQ?t=49
```

---
## \#11 Posted by: Jcullinan09 Posted at: 2017-08-29T21:17:39.302Z Reads: 114

```
I had no where near that much smoke, probably 1/20th of that much. But essentially yes there was smoke coming out.
```

---
## \#12 Posted by: darkkevind Posted at: 2017-08-29T21:18:51.839Z Reads: 112

```
Probably your motor wires are shorting. Mine did, and then it got worse and worse.

You can only rewind after that, nothing more....
```

---
## \#13 Posted by: Jcullinan09 Posted at: 2017-08-29T21:18:58.572Z Reads: 105

```
Did this happen to you? Or was it a video you found online? If it happened to you, what did you do, was the motor totally fried thereafter?
```

---
## \#14 Posted by: darkkevind Posted at: 2017-08-29T21:19:35.068Z Reads: 102

```
Yes this is my video from my first motor i bought. It was totally the wrong motor, 580kv!! lol
```

---
## \#15 Posted by: Jcullinan09 Posted at: 2017-08-29T21:20:51.172Z Reads: 102

```
Holy crap.. mine is only a 200kv.
```

---
## \#16 Posted by: darkkevind Posted at: 2017-08-29T21:22:27.056Z Reads: 102

```
Well I'm not saying it's the kv that's at fault, it was just the wrong motor and it ended up burning up lol
```

---
## \#17 Posted by: Jcullinan09 Posted at: 2017-08-29T21:28:45.673Z Reads: 103

```
I know, but I don't think 200kv is a wrong motor. Maybe @chaka might have an idea on this issue?
```

---
## \#18 Posted by: darkkevind Posted at: 2017-08-29T21:34:42.121Z Reads: 105

```
No, 200kv is fine.
```

---
## \#19 Posted by: Jebe Posted at: 2017-08-29T22:01:02.041Z Reads: 104

```
What voltage did you have on it ? What are your vesc settings ?
```

---
## \#20 Posted by: Jcullinan09 Posted at: 2017-08-29T22:16:51.924Z Reads: 99

```
I posted a screenshot up top. If there is a different one. I'll go grab a screenshot and put it up.
```

---
## \#21 Posted by: chaka Posted at: 2017-08-30T12:58:43.718Z Reads: 89

```
Wish I had seen this sooner. Looks like a bearing or spacer failure, seems like the whole stack lost proper spacing and the outrunner was rubbing. I will follow up with you later today and get a replacement out to you.
```

---
## \#22 Posted by: Jcullinan09 Posted at: 2017-08-30T22:33:09.419Z Reads: 88

```
Thanks for the response! Yesterday I played with mixing some of the motors and VESC's to one another, and am confident only one motor is acting up. 
The other motor (on the right) is running smoothly, and I'm just going to run the board with a single motor for now.

What are your thoughts? I think only one motor is failing.

-John
Jcullinan09@Gmail.com
```

---
## \#23 Posted by: chaka Posted at: 2017-08-31T12:56:19.255Z Reads: 82

```
We will take care of it! Have another motor posted to you today. Do me a favor and send the bad one back, I want to know how it failed. Plus, I need some extra stators for a side project. ;)
```

---
## \#24 Posted by: Jcullinan09 Posted at: 2017-09-02T18:46:12.487Z Reads: 71

```
This sounds great! The motors here were for a board for my little brother.
So If it is OK with you I would like to send both of the motors back as I am begging to think the other one is following in the steps of the already shot motor. I can help pay for shipping or some repairs that need to be done when they get to you. 
Would you be OK if I sent both back to you?
@chaka
```

---
## \#25 Posted by: chaka Posted at: 2017-09-02T19:01:04.812Z Reads: 68

```
Yes, please do!
```

---
## \#26 Posted by: Jcullinan09 Posted at: 2017-09-02T19:26:27.970Z Reads: 66

```
Okay, will do!
```

---
## \#27 Posted by: Jcullinan09 Posted at: 2017-09-02T19:31:59.490Z Reads: 68

```
Gahh! Could you provide me with your address on where to ship to again? I can't seem to find where I wrote it down earlier.
```

---
## \#28 Posted by: chaka Posted at: 2017-09-02T22:41:14.829Z Reads: 69

```
You can find it all here. http://www.ollinboardcompany.com/support
```

---
## \#29 Posted by: jkrider Posted at: 2017-09-10T18:19:02.744Z Reads: 55

```
I may have the same problem. Not sure if it's the same "clicking" noise.  https://youtu.be/33J9zMgiZ0k
@chaka Any ideas what happened to my motor?
```

---
## \#30 Posted by: Jcullinan09 Posted at: 2017-09-12T01:03:56.411Z Reads: 47

```
I don't think that you had the same problem as mine. The motors I had would not even spin up, however in my very scientific answer... your clicking did not sound the same as mine.
```

---
