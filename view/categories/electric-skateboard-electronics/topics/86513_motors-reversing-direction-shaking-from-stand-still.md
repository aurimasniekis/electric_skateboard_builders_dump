# Motors reversing direction/shaking from stand still

### Replies: 14 Views: 269

## \#1 Posted by: Celt Posted at: 2019-03-08T02:29:11.742Z Reads: 102

```
Hey guys,

I have a FOCBOX Unity with dual Torque Boards 6355's and I'm running BLDC. I just finished my build with the Unity and I'm having some issues. When I'm at a stand still I have this problem where my motors will shake and then slowly start running backwards at a set speed regardless of throttle. If I let off and push off it will go forward alright. I know shaking is normal if you don't push off with BLDC but yeah this seems not normal. I had two TB VESC's before this and they needed slightly less of a push off and didn't do this weird reverse thing. Any help would be great!
I included a YouTube link, please let me know what you think.

https://youtu.be/exZvpbcG2co
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-03-08T02:32:16.141Z Reads: 99

```


Are you running them in sensored mode?
```

---
## \#3 Posted by: Celt Posted at: 2019-03-08T02:46:55.715Z Reads: 98

```
Hey, I don't know.  I set them up via BT on the Unity app.  In the guided set up it never mentioned which mode it was set up in.
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-03-08T03:01:20.969Z Reads: 94

```
[quote="Celt, post:3, topic:86513"]
BT
[/quote]

are you sure you saved the settings....
```

---
## \#5 Posted by: Celt Posted at: 2019-03-08T03:05:13.877Z Reads: 92

```
I mean yeah i did. I applied the settings during the setup.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-03-08T03:06:06.744Z Reads: 90

```
Definitely something to do with the settings. more info, screenshots?
```

---
## \#7 Posted by: Celt Posted at: 2019-03-08T03:15:14.166Z Reads: 84

```
Ok i can do that. Should i hook it up manually and use desktop program or do you want some a android app screen shots?
```

---
## \#8 Posted by: ShutterShock Posted at: 2019-03-08T04:42:43.944Z Reads: 79

```
I haven't used the app yet, but I feel like the desktop is easier no matter what, the app is probably better in the end for quick adjustments rather than first time setup.

You can view all of your settings in the desktop app, as long as you remember to click the read settings from VESC button
```

---
## \#9 Posted by: Celt Posted at: 2019-03-10T16:35:48.992Z Reads: 59

```
Hey so the desktop app is the same as the android app. At this point I set it up correctly with one of the Enertion staff and it still does it. I think the only thing to do at this point is to get sensor wires so I can run sensored FOC I think that'd fix it.
```

---
## \#10 Posted by: Blasto Posted at: 2019-03-10T16:45:36.744Z Reads: 55

```
If you are running unsensored, just give it a push start
```

---
## \#11 Posted by: jun1208 Posted at: 2019-03-10T16:53:06.303Z Reads: 50

```
I experienced the name thing when I run my sensorless motor last time, push start and accelerate will solve the issue :+1:
```

---
## \#12 Posted by: ShutterShock Posted at: 2019-03-10T17:13:14.215Z Reads: 41

```
Yeah or like other pastor are saying just push start it, sometimes that's easier
```

---
## \#13 Posted by: maxchilton Posted at: 2019-03-10T17:55:28.157Z Reads: 37

```
[quote="Celt, post:9, topic:86513"]
I think the only thing to do at this point is to get sensor wires so I can run sensored FOC I think that’d fix it.
[/quote]

that "cogging" from a standstill is completely normal if you're running sensorless.  Running sensored will fix it.
```

---
## \#14 Posted by: TommyCnc Posted at: 2019-07-09T08:13:18.760Z Reads: 16

```
I had this exact issue running sensored. Only fix for me  so far was to run sensorless.
```

---
