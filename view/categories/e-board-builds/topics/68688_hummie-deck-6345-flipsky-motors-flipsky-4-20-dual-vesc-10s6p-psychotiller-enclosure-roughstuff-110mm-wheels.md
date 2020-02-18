# Hummie deck &#124; 6345 Flipsky motors &#124; Flipsky 4.20 Dual VESC &#124; 10s6p &#124; Psychotiller enclosure &#124; Roughstuff 110mm wheels

### Replies: 21 Views: 1088

## \#1 Posted by: Flashgod224 Posted at: 2018-09-20T22:59:54.804Z Reads: 325

```
Hey guys, just finished up on my new build but still waiting for my hummie deck. I was trying out my board for a bit and noticed something really annoying in throttling.

When full blasting the throttle, my board refuses to accelerate or decelerate. Anyone know what the issue might be? I am runnign BLDC unsensored.
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-09-20T23:00:52.572Z Reads: 319

```
more info please
```

---
## \#3 Posted by: Flashgod224 Posted at: 2018-09-20T23:01:48.230Z Reads: 311

```
Sorry misclicked to begin with, had to re-edit it all. Let me know if u need to know more... I think I should open it up and check the logs maybe :confused:
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-09-20T23:04:13.920Z Reads: 306

```
could have a sticky transmitter pot...? check in bldc tool to see the green bar. is the throttle staying up when you floor and let go it or does it come down when you let go and the motor keeps spinning?
```

---
## \#5 Posted by: Flashgod224 Posted at: 2018-09-20T23:13:36.490Z Reads: 289

```
Ill have to check... also my BMS is always warm/hot sometimes even when my board is off, I am running this set up bypassing discharge as well. Really not sure what's going on with it
```

---
## \#6 Posted by: mynamesmatt Posted at: 2018-09-20T23:15:27.151Z Reads: 286

```
can you upload some pics of the wiring
```

---
## \#7 Posted by: Flashgod224 Posted at: 2018-09-20T23:16:35.858Z Reads: 282

```
![image|612x500](upload://9jUhk8Vwz6M4FZxRhf4Shrocxc6.jpeg) For the BMS
```

---
## \#8 Posted by: Flashgod224 Posted at: 2018-09-20T23:18:14.254Z Reads: 263

```
Minus that last black balance wire.
```

---
## \#9 Posted by: Flashgod224 Posted at: 2018-09-21T00:19:07.722Z Reads: 255

```
So on bldc tool, the green bar stays at zero and as soon as I do the 0-100 there is a flash fault of ABS-over-current... Forgot how to fix this one...
```

---
## \#10 Posted by: mynamesmatt Posted at: 2018-09-21T01:35:49.863Z Reads: 244

```
try lowering the erpm?
```

---
## \#11 Posted by: dareno Posted at: 2018-09-21T01:40:17.722Z Reads: 247

```
If your bms is hot when not riding and switched off then disconnect your battery immediately and check your wiring.  Somethings wrong and could lead to thermal runway.  

[quote="Flashgod224, post:5, topic:68688"]
also my BMS is always warm/hot sometimes even when my board is off,
[/quote]
```

---
## \#12 Posted by: lrdesigns Posted at: 2018-09-21T01:45:45.930Z Reads: 245

```
[quote="Flashgod224, post:9, topic:68688"]
soon as I do the 0-100 there is a flash fault of ABS-over-current…
[/quote]

Sounds similar to others issue on the flipsky 4.2 dual. But they had this issue on 12s, no one reported in on 10s yet. 

So you can get this over current error just on the bench, or is that a log from ridding it under real load?

by "I do the 0-100"  you mean mashing the throttle from zero to full?
```

---
## \#13 Posted by: Flashgod224 Posted at: 2018-09-21T03:25:51.031Z Reads: 224

```
Yes from 0 to full within an instant, working on a fix and I will check if it's just a small programming issue or something else. Will def update on it.

@dareno My balance leads were wired the wrong way. Have to redo the crimped pins on my balance lead housing. Simple fix!
```

---
## \#14 Posted by: Flashgod224 Posted at: 2018-09-21T16:24:28.169Z Reads: 206

```
The over current error happens only if I 0-100 (punching the gas) and it then doesn’t accelerate, but makes it idle until I’ve reset the throttle to the centre.

It flashes for a second on the faults when reading real time data but doesn’t fall under the actual faults log
```

---
## \#15 Posted by: luv2sk8te17 Posted at: 2018-09-26T17:25:52.407Z Reads: 178

```
What are your bldc settings?
```

---
## \#16 Posted by: Benjamin899 Posted at: 2018-09-26T17:57:39.131Z Reads: 179

```
@Flashgod224 the negative to your load should come from p-.
edit: nvm just saw its bypass.
```

---
## \#17 Posted by: Flashgod224 Posted at: 2018-10-02T09:37:23.441Z Reads: 169

```
My bldc settings are 
45
-40
30
-18
```

---
## \#18 Posted by: dougpage Posted at: 2018-11-13T06:24:29.753Z Reads: 136

```
Can you send some pics of the build?
```

---
## \#19 Posted by: Flashgod224 Posted at: 2018-11-13T19:31:43.017Z Reads: 142

```
@dougpage I dyed my flywheels black now, Also I am upgrading to a FocBox Unity and going to make my firefly remote ![image|375x500](upload://dXrp9Z5ctvGcfHsFFJUnuzluUmB.jpeg)  ![image|500x500](upload://qVBvxjY81SqnGqxnFNTm6y8tTt4.jpeg)  ![image|642x480](upload://tkMg8ePx5se9So0mh9sTUmLqgq4.jpeg)  ![image|375x500](upload://lm9k9oKlfcVpy9hr2ah2jB2aZVL.jpeg) ![image|666x500](upload://gy2FsGIxII5QNhvNRTPTat5BoFY.jpeg) ![image|666x500](upload://7LTg8D1iIYwMSjDuY3KeVs4pd4i.jpeg)
```

---
## \#20 Posted by: Skyart15 Posted at: 2019-09-13T04:00:10.210Z Reads: 39

```
Hey how are those flipsky motors treating you, looking to get some, but not sure if they are good or not
```

---
## \#21 Posted by: rangedu Posted at: 2019-09-13T05:01:58.234Z Reads: 35

```
they shitted on him after going in the rain, he got maytech one now.
```

---
