# Throttle and braking issues. Been fine for a week, now I have a problem

### Replies: 30 Views: 1126

## \#1 Posted by: JuniorPotato93 Posted at: 2016-10-17T18:26:13.725Z Reads: 101

```
So, hopped on today and it felt different.  Could feel a notice in acceleration and braking they were both much slower.  Came home and saw this was happening https://youtu.be/vo11NvobB4o 

I just checked and there was one connection that was loose. I since then fixed it. But the issue persists.  Any ideas?

Just checked the connection to the receiver and it seems okay. What do i check next?
```

---
## \#2 Posted by: JuniorPotato93 Posted at: 2016-10-17T18:32:33.247Z Reads: 99

```
When I go to brake, the VESCS that consistently does not brake, the left wheel in the video, it has an LED that blinks red between the blue and the green LED
```

---
## \#3 Posted by: Blasto Posted at: 2016-10-17T18:41:19.742Z Reads: 98

```
huh, post your settings, seems to be something is off
```

---
## \#4 Posted by: JuniorPotato93 Posted at: 2016-10-17T18:43:28.371Z Reads: 96

```
I will post them as soon as I get home. I'm in the middle of class now.
```

---
## \#5 Posted by: Blasto Posted at: 2016-10-17T18:44:12.124Z Reads: 88

```
[quote="JuniorPotato93, post:4, topic:11306, full:true"]
I will post them as soon as I get home. I'm in the middle of class now.
[/quote]
great place to edit a video haha
```

---
## \#6 Posted by: chaka Posted at: 2016-10-17T18:51:15.748Z Reads: 82

```
Looks like an ABS overcurrent situation sending the vesc into fault. Get eyes on the VESC and see if it flashes 3 times when this happens. May be a settings issue or you could need some service. Have you used FOC in the past? No worries if you did, we will still provide service even though we do not recommend using that function of the VESC.
```

---
## \#7 Posted by: JuniorPotato93 Posted at: 2016-10-17T18:59:36.973Z Reads: 74

```
I took that video when I got home just before I left for class, just posted the url  when I got here.
```

---
## \#8 Posted by: JuniorPotato93 Posted at: 2016-10-17T19:03:40.360Z Reads: 72

```
I'll have to check when I get home again, I can't recall how many times it blinked. And no I don't use FOC, both VESCs are exact same settings. I've really been riding it every day around campus for a week straight. Maybe like 7 miles a day.
```

---
## \#9 Posted by: JuniorPotato93 Posted at: 2016-10-17T19:11:59.246Z Reads: 71

```
Blasto, @chaka 

These are the settings I posted in the original post and haven't changed it since. I grabbed this off the original post I made about the build so I don't have access to the rest of it until I get back. 

Just thought about something. My BMS supports charging up to 20amps so should my regen braking be 10 or less per VESC?

<img src="/uploads/db1493/original/3X/f/3/f3c411db74e0ac9e1afecdf28a8f02a5f0464bf3.JPG" width="690" height="353">
```

---
## \#10 Posted by: Blasto Posted at: 2016-10-17T19:15:00.577Z Reads: 64

```
set your maximum input back to 57V

when braking, your are hitting your upper limit, the vesc thinks it needs to protect itself and "shutsdown"
```

---
## \#11 Posted by: JuniorPotato93 Posted at: 2016-10-17T19:19:49.305Z Reads: 64

```
Okay, i will adjust this when I get home. But if this is the case how come I have 2 VESCs with the exact same settings gs but only one just started acting up?
```

---
## \#12 Posted by: Blasto Posted at: 2016-10-17T19:22:54.398Z Reads: 61

```
in the video both of them seem to have this weird behaviour, just not at the same time
```

---
## \#13 Posted by: JuniorPotato93 Posted at: 2016-10-17T19:30:49.642Z Reads: 59

```
That's a good point though it seems to be one more than the other. Let me try this when I get home in 2 hours and I'll update you on if this resolved the issue. So just follow up question, what would have triggeted this? Could one loose bullet connector have caused this while trying to brake? Just trying to understand the root cause so I can prevent it from happening again going forward.
```

---
## \#14 Posted by: Blasto Posted at: 2016-10-17T19:41:56.600Z Reads: 52

```
[quote="JuniorPotato93, post:13, topic:11306"]
what would have triggeted this?
[/quote]

it is just a bad setting, should not touch this setting, it won't damage anything, just give false errors
```

---
## \#15 Posted by: JuniorPotato93 Posted at: 2016-10-17T19:44:38.212Z Reads: 51

```
But my confusion is why did it take a week for this bad setting to manifest itself?  That's kinda what I'm confused about. @chaka can you provide some clarification on this? I'll be changing the max input voltage back up to 57V, but I'm just trying to understand why this wasn't an issue from the get go?
```

---
## \#16 Posted by: Blasto Posted at: 2016-10-17T19:45:19.185Z Reads: 49

```
did you freshly charge your batteries?
```

---
## \#17 Posted by: JuniorPotato93 Posted at: 2016-10-17T19:50:46.559Z Reads: 49

```
Yes. Charged it last night to full.  Just hopped on this morning to head to a meeting and that's when I noticed. But there were issues with acceleration as well, which was probably due to the loose bullet connector. But then I noticed the braking which I knew could be due to just being charged but again. This whole week I haven't had any issues with breaking with a full battery so that's what made me think there was something wrong. Them I went home and made that video
```

---
## \#18 Posted by: chaka Posted at: 2016-10-17T19:50:56.134Z Reads: 49

```
Your cells could be responding to use. If it is a small pack and you have been driving too much regen current they could have degraded enough to rise in voltage much faster than when new. Repeated faults could have also corrupted the firmware. A fresh upload using the bootloader can fix it if that is the case.
```

---
## \#19 Posted by: JuniorPotato93 Posted at: 2016-10-17T19:55:14.322Z Reads: 47

```
It's a 8S6P pack using Samsung 25R 18650 cells.   So when I get back, if raising the input voltage back to 57V doesn't solve the issue I'd have to reset the firmware?  Is that the same as flashing the firmware? Because I heard you can mess that up and render the VESCs useless sof I'm hesitant to do that.

Not sure if it makes a difference @Blasto but the pack is fully charged at 33.6, charged up 33.4 last night.  After my trip to the meeting goes and back its currently sitting at 32.6 so it's not at full.
```

---
## \#20 Posted by: chaka Posted at: 2016-10-17T20:00:07.399Z Reads: 46

```
You should also lower you regen to -7 to -10 per vesc. when you snap the brakes like you were in the video you are probably peaking around 80 amps of regen. The limits on the vesc take a few milliseconds to respond since everything is relying on the processing speed of the stm chip.
```

---
## \#21 Posted by: JuniorPotato93 Posted at: 2016-10-17T20:07:48.119Z Reads: 44

```
Okay, I'll changed that along with the max voltage input. See what that does.
```

---
## \#22 Posted by: JuniorPotato93 Posted at: 2016-10-17T22:06:47.878Z Reads: 41

```
@chaka @Blasto

This look okay? I ran a motor detection and got no fault codes. Dont actually know I'm supposed to check for fault codes but I figure that would be the place.

<img src="/uploads/db1493/original/3X/2/4/24ab6c3e2aa601bca2235e8f52fdec460f9f44e3.png" width="690" height="357"> 

<img src="/uploads/db1493/original/3X/b/4/b47e37ba859c6ccf0f46e3a5bb2a4bff672bdb5a.png" width="690" height="367">

<img src="/uploads/db1493/original/3X/e/1/e18d9b49b07f36aa912a848d8c84bb6c45dcaa4e.png" width="690" height="367">
```

---
## \#23 Posted by: chaka Posted at: 2016-10-17T22:12:38.421Z Reads: 36

```
If you enable active sampling on the realtime data it will show fault codes on the bottom left hand side of the screen.
```

---
## \#24 Posted by: JuniorPotato93 Posted at: 2016-10-17T22:22:59.030Z Reads: 37

```
No Faults found @chaka 

<img src="/uploads/db1493/original/3X/b/8/b896e4055b80a2daa8ab23f4ad6626b32117b79f.png" width="690" height="367">
```

---
## \#25 Posted by: chaka Posted at: 2016-10-17T22:32:05.261Z Reads: 35

```
That will only show them in real time if you want to see if any have logged go to "terminal" and type faults. It will show you if any have logged while connected through the usb port.
```

---
## \#26 Posted by: JuniorPotato93 Posted at: 2016-10-17T23:09:56.118Z Reads: 35

```
Mmmm. Okay. Well, I had upped the max in,  and reduced the regen brake and tried it out real time with no load and I got no issues like I had been before. I will check that again once I get back from class but I put the case back on and tried it out just now and no issues. Full acceleration and braking. I'm also not flicking the remote as hard I was in the video, that was just to demonstrate the issue in worst case scenario.

But as of right now it looks like that resolved the issues. I will post what error I had gotten before.
```

---
## \#27 Posted by: saul Posted at: 2016-10-17T23:18:49.437Z Reads: 35

```
if the input voltage didn't fix it i'm thinking it could be a ppm issue. 
are you using split pwm? make sure the two are calibrated and consistent.
```

---
## \#28 Posted by: JuniorPotato93 Posted at: 2016-10-17T23:36:19.301Z Reads: 33

```
Hey @saul  yeah it is split but it's been working without a problem for a week now so I doubt it was that. I calibrated that over a week ago. And rechecked the calibration today. I did make sure to make sure all the connections are tight and a piece of electrical tape to prevent them coming loose from vibrations. 

The input voltage back up to 57V and reducing the regen braking from each VESC to 7amps seemed to have fixed the issue.
```

---
## \#29 Posted by: saul Posted at: 2016-10-17T23:57:14.801Z Reads: 33

```
ok good to know.
 makes sense since when you brake your input voltage goes a bit higher than a full charge.

57v is safe for 12s which is about 51v full.
so anything above 40 should be fine for 8s. but seem like there is no real reason to lower it....
```

---
## \#30 Posted by: JuniorPotato93 Posted at: 2016-10-18T00:04:10.003Z Reads: 32

```
Yeah I guess there's no real issue with leaving it at the default 57v
```

---
