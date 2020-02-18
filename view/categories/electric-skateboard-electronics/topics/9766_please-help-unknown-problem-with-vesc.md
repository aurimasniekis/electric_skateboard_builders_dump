# Please help, unknown problem with VESC

### Replies: 16 Views: 1242

## \#1 Posted by: theviith Posted at: 2016-09-17T22:28:22.503Z Reads: 115

```
Hey guys, so there seems to be a problem with the VESC I got from Ollin. When powered on and spinning freely, everything seemed normal. However, once I put my weight on the board, it started acting weird. It would suddenly accelerate really fast and then stop, throwing me off the board. Other times, I would loose complete control over the board, including braking. I've swapped out the receiver with another one and it still does the same thing so the problem can't be in the r/c. Could this be a DRV fault? But I've checked the realtime sampling and it doesn't seem like it (unless I am missing something?). So now I'm thinking it might be my VESC settings. I've attached a few screenshot below, please let me know if these settings are correct. I am running 2x VESC on 2x sk3 260kv motors, 10S Space cell GT2B Rx/Tx, Abec 11 83 mm, 16/36. 

Also, does anyone know the sign and symptoms to a DRV fault/failure/overheating? Now that I think about it, it could be a DRV issue after all since I did run it pretty hot on a hot night one time..

Thanks in advance

Pictures 1-4 are settings for the Master VESC
Pictures 5-8 are settings for the Slave
1. <img src="/uploads/db1493/original/3X/0/6/06eade9c1afc299941188cf3d2645a1229e849aa.jpg" width="690" height="388">
2. <img src="/uploads/db1493/original/3X/c/5/c54aedd33baff8854c60819b491159800b8da09a.jpg" width="690" height="388">
3. <img src="/uploads/db1493/original/3X/4/c/4cdae9e063416cd7ac893912b5f4c8df44e4c5b1.jpg" width="690" height="388">
4.<img src="/uploads/db1493/original/3X/d/1/d15d2070c363bc7fd81347d99b40b599dfdf812b.jpg" width="690" height="388">
Motor settings for the Slave is the same as the Master shown in pictures 1 and 2.
7. <img src="/uploads/db1493/original/3X/0/9/09044d79f7a5845de7d560e1fb69e288f116bcc3.jpg" width="690" height="388">
8. <img src="/uploads/db1493/original/3X/4/5/451950c4be0f2411378fbbf6b7a11eddf6888367.jpg" width="690" height="388">
```

---
## \#2 Posted by: Lsalt Posted at: 2016-09-17T22:51:32.578Z Reads: 92

```
Did you hook it up to bldc tool and run realtime data? Drv would pop up there if that's at fault. But maybe not if only acting up under load....when mine Drv faulted it was just dead. But tool revealed code
```

---
## \#3 Posted by: Jinra Posted at: 2016-09-18T00:19:11.712Z Reads: 91

```
Might be loose, unsecure CAN cable
```

---
## \#4 Posted by: elkick Posted at: 2016-09-18T00:28:50.696Z Reads: 87

```
You need to correct your slave settings: disable app entirely (you enabled "multiple ESC over can", this will cause problems, it should only be enabled for the master).

The rest seems to be ok.
```

---
## \#5 Posted by: theviith Posted at: 2016-09-18T04:43:22.727Z Reads: 77

```
yup I did. but all the data appears to be normal upon free spinning. I could only record it while free spinning since I can't really do the same with load. And the problem seem to only appear when under load.
```

---
## \#6 Posted by: theviith Posted at: 2016-09-18T04:57:03.019Z Reads: 77

```
@Jinra I've checked the cable and it's secure. 

@elkick I just corrected those values and went for a test run, but still have the same problem.

Additionally, due to the limited space of my enclosure, I have the GT2B receiver sandwiched between the two VESCs surrounded by wires. Could this be a possible cause for radio interference? If so, would installing a ferric ring solve the problem?
```

---
## \#7 Posted by: Jinra Posted at: 2016-09-18T05:00:43.974Z Reads: 74

```
If any metal bits or the phase wires are touching the receiver, it can cause the receiver to freak out. I've personally experienced this. A ferrite ring won't help with this, but can help against other noise. Also, try wiggling the can cable around and seeing if it's working properly, sometimes it looks secure, but doesn't work in certain positions.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-09-18T06:25:51.769Z Reads: 76

```
First of all 260kv is much too high for Vesc at 10s 
You should be running 190kv at 10s
You could easily burn up your Vescs with that combination.
I'm running dual vescs without canbus. I'm using both Vescs as masters and each has a signal harness going to a Y-connector with the red wire clipped on one of them.
Works great that way.
```

---
## \#9 Posted by: devin Posted at: 2016-09-18T09:01:10.931Z Reads: 70

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#10 Posted by: theviith Posted at: 2016-09-18T19:47:21.929Z Reads: 62

```
@Jinra I've repositioned the receiver and away from the phase wires, it still does the same thing.

@Namasaki Yeah, I know 260kv might be a bit high but I haven't been running it at max throttle so theoretically it shouldn't burn up my VESC if I keep to low/mid throttle right? Or unless it doesn't matter?

Also, would you mind sharing a pic/drawing of what you mean by the Y-connector in using both VESCs as masters?

@devin I'm not sure where to get that value. I'm not using FOC so everything in the BLDC sensorless settings has been posted in my first post.
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2016-09-18T20:35:35.199Z Reads: 60

```
Put the ERPM down to 70000
```

---
## \#12 Posted by: Namasaki Posted at: 2016-09-18T21:24:59.970Z Reads: 59

```
[quote="theviith, post:10, topic:9766"]
Yeah, I know 260kv might be a bit high but I haven't been running it at max throttle so theoretically it shouldn't burn up my VESC if I keep to low/mid throttle right? Or unless it doesn't matter?
[/quote]
Check with @chaka about that. 
190kv is recommended for the Vesc at 10s. 
260kv is really high.
```

---
## \#13 Posted by: theviith Posted at: 2016-09-18T22:43:34.603Z Reads: 59

```
hm so upon more testing, I found out the problem is definitely with the VESC...but I just don't know what exactly. Also it appears that it is the Master vesc that is having issues as the pink light appears to be blinking whenever it starts acting up.

@Namasaki yeah I'll shoot him a message. Thanks for the help
```

---
## \#14 Posted by: chaka Posted at: 2016-09-18T23:00:40.749Z Reads: 58

```
Few things, the difference between your motor max and battery max are way too high. Bring the motor max down to 35 to 40 amps. This may have contributed to the funky behavior.

You also need to use a lower kv motor. It seems like you already fried one. Even a 245kv tacon will fry a vesc at 10s.

Why did you fit 260kv motors at 10s?

You will need to contact us through our website and send in the vesc with the drv fualt. We will get you back up and running but you wil continue to have problems if you dont being your system onto check.

One other issue is the very tall gear ratio paired with the high kv motors.  Have you checked to see what you theretical top speed is? Your motors are likely loading up and wanting to pull a huge amount of current.
```

---
## \#15 Posted by: theviith Posted at: 2016-09-18T23:26:58.902Z Reads: 54

```
@chaka Thanks for the detailed response. I fit the 260kv at 10S primarily for the range rather than the top speed. I was thinking that by using these motors at low throttle for normal cruising, I would get a much larger range while still enjoying the benefit of dual motor configuration. But now that I think about it, I think what you said about the large current pull (esp. on a hot summer day) is most likely what caused the vesc to fault.

Thanks, will do. Can I send both of them in? Just to make sure that the other vesc wasn't affected.

Regarding kv and gear ratio, would 213kv at 16/36 work? If not, I guess I'll need to invest in some 190kv
```

---
## \#16 Posted by: chaka Posted at: 2016-09-18T23:44:26.524Z Reads: 50

```
Sure, you can send them both. If you are looking for max range an maximum efficiency then you want your board to top out at roughly 20mph at max throttle. This gives you good startup and acceleration without pulling a large amount of amperage.
```

---
