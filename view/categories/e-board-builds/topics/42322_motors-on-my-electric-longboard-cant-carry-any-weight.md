# Motors on my electric longboard cant carry any weight

### Replies: 34 Views: 1190

## \#1 Posted by: tonystark Posted at: 2017-12-30T19:33:06.920Z Reads: 159

```
So I have completed my electric longboard and everything work fine (when board is upside down), wheels turn fine. When I put board on its wheels motors cant turn. When board is upside down and wheels turn i can stop it with my hand. I tried to stand on it and ride but same problem. If motors cant carry weight of the board leave alone  carrying me. I have dual motor set up. Motors are from Alien Power Systems 5065 Sensored Outrunner brushless motor 220KV 2200W. It runs from 8S4P battery.  I am using dual VESC as well
Anyone have any idea what can be wrong? Link to the video is attached
https://youtu.be/mjm5lD6RGW8<img src="/uploads/db1493/original/3X/e/6/e672a11e894397d70f6815f754853fa85f6ed65a.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/0/3/035f4b562236039b97d8df85149a7528ae445dd0.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/a/3/a3f7a30677a998eaeeb2902de6a6709fc269d7ef.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/f/6/f641e1078669ae23f2e4a78e0ee1b1323309eaab.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/b/9/b982e43f02bda031f1dd83098dffce06c8941adf.png" width="689" height="435">
<img src="/uploads/db1493/original/3X/2/8/2822eb0d187fdaf3ad1b25a8fe0c3b5ee703b434.png" width="690" height="489">
<img src="/uploads/db1493/original/3X/b/f/bffa2e9321ca67f0c29802ade81f7e3588e3ff82.png" width="690" height="436"><img src="/uploads/db1493/original/3X/0/9/099b49d6830441675d07614130236151de0068d5.png" width="690" height="434"><img src="/uploads/db1493/original/3X/1/6/1671a8a43162c3576360f711d4a67cd7748215b2.png" width="690" height="432">
```

---
## \#2 Posted by: thisguyhere Posted at: 2017-12-30T19:36:06.947Z Reads: 147

```
are you using a vesc?  if so, please post screenshots (not smartphone photos of your screen) of your motor, bldc, ppm tabs
```

---
## \#3 Posted by: tonystark Posted at: 2017-12-30T19:41:33.938Z Reads: 141

```
Yes, I am using dual VESC. I will post pictures and video. As soon as i will find out how to attach it
```

---
## \#4 Posted by: Colson003 Posted at: 2017-12-30T20:27:00.794Z Reads: 131

```
your trucks are backwards but that's a different problem.
```

---
## \#5 Posted by: tonystark Posted at: 2017-12-30T20:31:23.766Z Reads: 127

```
Yeah, i know they are backwards. i just put them on without thinking which way to put them on. Just wanted to see if it works
```

---
## \#6 Posted by: scepterr Posted at: 2017-12-30T20:36:38.326Z Reads: 121

```
Your battery cutoff is set for 10S config
Your start is set at 33v
Your full charge is 33.6

If you want the start to be at 3.4 per cell it's 27.2v
```

---
## \#7 Posted by: tonystark Posted at: 2017-12-30T20:43:34.060Z Reads: 114

```
whait, did you see it on screen shots of bldc tool?
```

---
## \#8 Posted by: L3chef Posted at: 2017-12-30T20:47:07.905Z Reads: 114

```
7th picture bottom right
```

---
## \#9 Posted by: Sk8Board Posted at: 2017-12-30T20:47:31.907Z Reads: 114

```
Try pushing the board manually then push the throttle. Maybe that would work. Looks like you didn't plug in sensor wires. Are you running sensored or sensorless
```

---
## \#10 Posted by: tonystark Posted at: 2017-12-30T20:49:45.615Z Reads: 113

```
I see. the voltage limits settings. so what should i type in there? for max input voltage is voltage of my 8S battery. how about min input voltage?and battery cut oof start and end, wtf is that?
```

---
## \#11 Posted by: tonystark Posted at: 2017-12-30T20:50:12.615Z Reads: 112

```
i did. it moves really slowly but cant carry my weight
```

---
## \#12 Posted by: kyletrainy Posted at: 2017-12-30T20:52:24.934Z Reads: 107

```
Try 24v on battery cutoff start and 22.4v for battery cutoff end. Don’t need to change voltage limits
```

---
## \#13 Posted by: tonystark Posted at: 2017-12-30T20:59:47.970Z Reads: 108

```
Ok, looks like it works now. it can carry my weight. Thanks for help everyone
```

---
## \#14 Posted by: GrecoMan Posted at: 2017-12-30T21:12:15.065Z Reads: 101

```
did you do motor detection?
```

---
## \#15 Posted by: laurnts Posted at: 2017-12-30T21:17:18.084Z Reads: 97

```
I also suspect the same thing, the battery cut off was set too high for 8s.
So when throttle is being slammed, the voltage dropped. That voltage dropped being knocked off completely by the battery cut off, hence no power distribution.
```

---
## \#16 Posted by: scepterr Posted at: 2017-12-30T22:02:16.177Z Reads: 90

```
That's too low ,3.3-3.4 per cell is normal cut start
3.1-3.2 cut end

3.3 is 26.4
3.4 is 27.2

At 24-22v it's likely the BMS shut-off will kick in before vesc shuts off and no bueno
```

---
## \#17 Posted by: kyletrainy Posted at: 2017-12-30T22:14:37.463Z Reads: 83

```
Yea this seems healthier for the batteries, but how much would it affect his range?
```

---
## \#18 Posted by: scepterr Posted at: 2017-12-30T22:25:32.898Z Reads: 79

```
Yes it healthier, range will not be affected at all, there's no usable capacity at that voltage range, like a couple of feet
```

---
## \#19 Posted by: kyletrainy Posted at: 2017-12-30T22:31:10.557Z Reads: 72

```
I was agreeing with your cut off values but ok
```

---
## \#20 Posted by: scepterr Posted at: 2017-12-30T22:35:31.071Z Reads: 72

```
Hmm? A little confusion it seems

There will be no loss in range using 3.3-3.4v as the cut start vs 3v
```

---
## \#21 Posted by: kyletrainy Posted at: 2017-12-30T22:38:32.928Z Reads: 70

```
My bad man I should have been more clear. Anyway if there isn’t any difference in range op should definitely change his values
```

---
## \#22 Posted by: tonystark Posted at: 2017-12-30T23:04:10.689Z Reads: 64

```
So everything worked fine when i had when i had 24 v cut off start and 22.4 v cut off end. Now as you suggested i changed it to 26.4 and 27.2 and one of the motors turn fine and i can't stop it with my hand but the other one can be stopped by hand. some weird shit going on
```

---
## \#23 Posted by: rich Posted at: 2017-12-30T23:13:55.931Z Reads: 63

```
[quote="tonystark, post:22, topic:42322"]
i changed it to 26.4 and 27.2 and one of the motors turn fine and i can't stop it with my hand but the other one can be stopped by hand. some weird shit going on
[/quote]


Did you change the cut off settings on both vescs?
```

---
## \#24 Posted by: Deckoz Posted at: 2017-12-30T23:32:31.908Z Reads: 54

```
Is it just me or do y'all only see a 10s1p 😂
```

---
## \#25 Posted by: scepterr Posted at: 2017-12-30T23:37:36.868Z Reads: 52

```
Lol it's multiple layers, hard to see
```

---
## \#26 Posted by: pat.speed Posted at: 2017-12-30T23:38:12.762Z Reads: 52

```
What I thought it was an 8s2p
```

---
## \#27 Posted by: Sebike Posted at: 2017-12-30T23:40:17.958Z Reads: 53

```
8 x 2 cells per layer, but no telling how many layers.. might as well be 8s30p
```

---
## \#28 Posted by: tonystark Posted at: 2017-12-30T23:57:36.289Z Reads: 52

```
I did not know i had to change it on both vesc bc one vesc is like a master so i thought it will apply to both of them. besides, when i changed settings first time to 24 and 22.4 i also did it only once and both motors were turning strong and i was not able to stop any of them by hand. now i can stop one of them. how do i change it on both vesc anyway?
```

---
## \#29 Posted by: tonystark Posted at: 2017-12-30T23:58:42.832Z Reads: 50

```
what are you talking about?
```

---
## \#30 Posted by: tonystark Posted at: 2017-12-31T00:02:10.118Z Reads: 51

```
I think i know what  you are talking about. is it in controller ID? i have to choose 1 and 2 and change settings?
```

---
## \#31 Posted by: rich Posted at: 2017-12-31T00:11:23.038Z Reads: 50

```
[quote="tonystark, post:28, topic:42322"]
one vesc is like a master so i thought it will apply to both of them
[/quote]

Everything has to be changed on both vescs. You can plug the usb cable to the slave vesc or connect via master to ID 1 (usually the master is 0). Just to get sure, you did motor detection and settings on both vescs before use?
```

---
## \#33 Posted by: tonystark Posted at: 2017-12-31T00:14:44.199Z Reads: 43

```
yes, i did motor detection and everything before use. i did it a while ago but it was done. ok, cool, so i will see what happens if i change settings on both vesc. thanks again!!!
```

---
## \#34 Posted by: rich Posted at: 2017-12-31T00:16:46.128Z Reads: 45

```
You are welcome :grin:
As long as you have the same settings on both vescs everything should run flawlessly
```

---
## \#35 Posted by: pat.speed Posted at: 2017-12-31T04:22:11.777Z Reads: 34

```
The key word here is SHOULD 😂
```

---
