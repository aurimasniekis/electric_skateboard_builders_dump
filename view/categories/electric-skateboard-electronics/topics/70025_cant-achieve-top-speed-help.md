# Can&rsquo;t achieve top speed&hellip; help!

### Replies: 14 Views: 223

## \#1 Posted by: William_Trojel Posted at: 2018-10-03T17:07:48.134Z Reads: 91

```
The last bit of acceleration range on my remote won't respond (if that makes sense).
When i reach a certain point in turning the wheel on my remote from esk8.de, the board just stops accelerating?:worried: 
It haven't always been like this, it happend on my way to school one morning, at that time i just thought it was the low voltage starting.
I have already calibrated my remote on the bldc tool and i get 100%
Do anyone have any tips or solutions, it would be greatly appreciated :smile:
```

---
## \#2 Posted by: Vanarian Posted at: 2018-10-03T17:09:10.584Z Reads: 89

```
Can you rephrase? What do you mean it stops, you don't have anymore power to accelerate more or you suddenly get a power cut?
```

---
## \#3 Posted by: rey8801 Posted at: 2018-10-03T17:16:50.121Z Reads: 84

```
Which is your remote. Post the link.
To me:
-It's the actual max ERPM of your motor.
-wrong calibration in the VESC tool. 
-in case you have two modes on the remote you did the calibration in the slow mode.
-you hit some limits that you set at the vesc level.
```

---
## \#4 Posted by: Itsmedant Posted at: 2018-10-03T18:10:21.258Z Reads: 63

```
Yea we gotta know a few more things before answers will start coming in!

First thing, what type of remote do you have? Maybe briefly run down your build.

And the question that @Vanarian asked was my first thought. Are you talking about something like a governor kicking on and you can't go faster, or are you loosing acceleration when you push the stick further?
```

---
## \#5 Posted by: William_Trojel Posted at: 2018-10-03T18:29:18.260Z Reads: 53

```
Yeah okay.
When i reach the point on the wheel it just stays at the same speed, so it dosen't increase the speed when i turn it even more. This is the remote i have http://www.hellray.de/shop/#!/eSk8-de-Micro-Remote-2-4GHz/p/68315132/category=15842017

My build
sk3 6364 213 Kv
2x 4s 8000mAh lipos in series
Torque Boards VESC
```

---
## \#6 Posted by: William_Trojel Posted at: 2018-10-03T18:35:22.824Z Reads: 48

```
Here are my settings
![53|690x431](upload://a7hqq8Qy5zm7kModRUYoWk7vCrG.png) ![59|690x431](upload://H5pIVdSVjs9vurKGjXJW8KUV8q.png) ![12|690x431](upload://kSf5qyagwmc6NgNFSHGGaregQhc.png)
```

---
## \#7 Posted by: rey8801 Posted at: 2018-10-03T18:35:37.727Z Reads: 39

```
yeh it is a winning remote. It should have double speed setting on the side. to me as I said either you hit a limit on your setting. You simple reach the max speed is a 8s build. Or you did the signal mapping with the slow mode selected. Try to sort these hypothesis first.
```

---
## \#8 Posted by: William_Trojel Posted at: 2018-10-03T18:38:01.754Z Reads: 39

```
Ah i maybe think you are right about the two settings on the remote, will try that tomorrow :+1:
Thanks mate
```

---
## \#9 Posted by: Itsmedant Posted at: 2018-10-03T18:38:13.503Z Reads: 40

```
About how fast are you going when you run into this issue?
```

---
## \#10 Posted by: William_Trojel Posted at: 2018-10-03T18:56:48.340Z Reads: 38

```
26-28 km/h 
But i have easily achieved 34km/h and that wasn't full speed.
```

---
## \#11 Posted by: Itsmedant Posted at: 2018-10-03T18:57:51.165Z Reads: 31

```
So you hit 34km/h on this same board? Has anything changed since you did that? Something had to have been different if there is almost a 10km/h drop off.
```

---
## \#12 Posted by: William_Trojel Posted at: 2018-10-03T19:00:11.458Z Reads: 31

```
That is the weird thing, i just happen'd when i was riding to school.
But i did replace the vesc with another one, but i am back to the old one again.
Can you see anything wrong with my settings?
```

---
## \#13 Posted by: Itsmedant Posted at: 2018-10-03T19:02:09.520Z Reads: 26

```
I'm still trying to learn the VESC settings/troubleshooting stuff right now. Someone else will have to give you some more accurate info.

From what I see, it doesn't seem bad.

Was it a TB to TB VESC direct swap?
```

---
## \#14 Posted by: William_Trojel Posted at: 2018-10-03T19:45:05.105Z Reads: 21

```
no it was TB to esk8.de
```

---
