# Motor cutting at low speed hard acceleration (Help! VESC now dead)

### Replies: 13 Views: 843

## \#1 Posted by: amazingdave Posted at: 2018-04-21T06:39:05.014Z Reads: 129

```
12s Lipo, 4.12 VESC, 190kv dark matter running unsensored (detection wont work in sensored mode) latest Vedder firmware.
On steep hills at sub 10kmh when I pull the throttle hard the motor cuts out... any ideas? The VESC is not showing a fault on metr but the graph shows the duty shooting up to 95% at the moment of cutout and the amps die away.. at higher speed there’s no problem with tons of power.  ![image|281x500](upload://ykq0xWcUKE5AKYswTThywzr4MsJ.jpg)![image|281x500](upload://m2SzPhfiHje9EEvJoEFDuxHSFIU.jpg)![image|281x500](upload://ntCGNN53Glh7AIXDNi3LsbvFL66.jpg)![image|281x500](upload://oWNVEvEiaLku1jTUyY4BJiXMKtP.jpg)
```

---
## \#2 Posted by: Scoo_B_SK8 Posted at: 2018-04-21T08:19:45.621Z Reads: 113

```
should screen shot bldc/vesctool settings
```

---
## \#3 Posted by: onepunchboard Posted at: 2018-04-21T13:33:39.671Z Reads: 107

```
1. u said the detection won't work with sensor but use sensor may be this?
2. vesc has over current protection check this
3. voltage sag? 
4. bms problem?
 thats all i can think of now
```

---
## \#4 Posted by: Deckoz Posted at: 2018-04-21T14:15:44.922Z Reads: 102

```
Are you using old 4.12 hardware? Ie not an L-shaped PCB?

If you are there's a few things that could cause this
- hardware design, mixed with low motor amp settings. Non direct fets are slower. In my old vanguard I had a motor max of 45 and batt max of 30a. If I accelerated hard, pulling max motor amp or batt amp, when it reaches the max, the fets are slower to close the gates for the drains, so the next current read would be past the max, and the ESC would cut power. I haven't experienced this on ANY direct fet endowed hardware (focbox, hand made ESCape)

I solved this by increasing motor max. And by using sensors, and switching to direct fet ESCs
```

---
## \#5 Posted by: amazingdave Posted at: 2018-04-22T08:03:06.178Z Reads: 86

```
Thanks for the replies, 

@onepunchboard  there is no voltage sag, I don’t use bms, I’ve tried everything to get the motor detection to work in VESCtools but it just comes back with a 255 hall error. I’ve tested the halls with a multimeter and they work. 

@Scoo_B_SK8 @Deckoz I’ll upload images of my settings tomorrow, been at the beach for the weekend.
```

---
## \#6 Posted by: amazingdave Posted at: 2018-04-23T08:37:58.596Z Reads: 76

```
Below are the settings I was using... I say was because I tested the board again last night on a slight gradient, pulled the throttle and it cut out and reset, tried one more time and the VESC died! The VESC still connects to my pc through TCP bridge so I’ve screen shot the settings....

Ordered a new direct fet VESC from esk8.de so I really want to find out what went wrong, I don’t want to cook the new one! ![image|666x500](upload://jT8XXCWyGxQCtoqRy9jwK7VP6oA.jpeg)![image|666x500](upload://9SN9Ky2r9ZQcH8p0zY52wsmahlN.jpeg)![image|666x500](upload://1rLJEHXWOFAdniOQgYJFaLx9BjE.jpeg)![image|666x500](upload://1KrjgVr8no354s0E0OUce5PAZ8M.jpeg)![image|666x500](upload://kzoCerbNd1RVAPRIYcTUy9p79ml.jpeg)![image|666x500](upload://sFXc9YcOJUuYdYr6AQMSeYVs7rd.jpeg)![image|666x500](upload://o38q79ZXpyiVOqZRBntcwtfAhtR.jpeg)![image|666x500](upload://QswfnGH2UzCpYMho1KmK0fHaHi.jpeg)![image|666x500](upload://oQH5TK96wBggMWyW7jmCDun96mg.jpeg)
```

---
## \#7 Posted by: bigben Posted at: 2018-04-23T19:43:37.691Z Reads: 56

```
Hopefully someone can help you with this. To my eyes the settings look ok but I'm beginner level when it comes to vector setup..
Surely someone has some idea?
```

---
## \#8 Posted by: onepunchboard Posted at: 2018-04-24T21:23:48.752Z Reads: 49

```
isn't default switching value 20khz instead of 40?
```

---
## \#9 Posted by: RedEagle Posted at: 2018-04-24T21:44:12.361Z Reads: 48

```
Try these settings:

Motor Max 50
Motor Min -50
Batt Max 30
Batt Min -14

DON'T go up a hill from a standstill. It seems your vesc can't handle it. Push starting might also be a good idea.
```

---
## \#10 Posted by: b264 Posted at: 2018-04-24T22:08:42.699Z Reads: 45

```
What brand HW4.12 is this?
```

---
## \#11 Posted by: RedEagle Posted at: 2018-04-24T22:15:27.769Z Reads: 46

```
scram board
```

---
## \#12 Posted by: amazingdave Posted at: 2018-04-25T06:13:00.676Z Reads: 41

```
As @RedEagle said, it’s a scramboards VESC...

The faults happen even when the board is rolling after a push start.... 

I think the problem started when I went from a 12t motor pinion to a 15t to stop my belts snapping. The board accelerated up any hill with the 12t but the 15t really put the strain on.

I thought that because the recorded currents in metr were nowhere near my max values I was in the clear but it would seem not! 

I’ve got a direct fet VESC on the way and have changed my gearing from 15:36 to 15:44 so that should help drop the current demands a ton. 

I’ll try the values you suggested @RedEagle. 

Thanks for the advice.
```

---
## \#13 Posted by: amazingdave Posted at: 2018-04-25T10:20:33.021Z Reads: 36

```
@onepunchboard I have no idea what the default usually is but that is the figure that came up in the latest VESCtools...
```

---
