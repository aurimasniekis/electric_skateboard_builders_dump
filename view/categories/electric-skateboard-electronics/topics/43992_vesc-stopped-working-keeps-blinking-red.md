# VESC stopped working, keeps blinking red!

### Replies: 13 Views: 919

## \#1 Posted by: SkateYS Posted at: 2018-01-18T04:20:45.785Z Reads: 106

```
Hi everyone, I got a new VESC yesterday, set it up with a 10s2p battery. It worked great yesterday but today after a couple of miles it slowed down as if i braked. i stopped and realized that the VESC has that solid blue light and a blinking red. I disconnected the battery and the wheel still can't spin freely! VESC is generating a sort of brake even without no power source connected. I carried that heavy board home and hooked it up to BLDC tool! here are pictures: 
![20180117_223908|666x500](upload://hTB9kM4GHbyuRDPw7PHGduGKQay.jpg)![20180117_223729|666x500](upload://66NA7yJWVoOZcG2KkRJU59jai8P.jpg)![20180117_223807|666x500](upload://h5SGyXv2aHeIm00tLlULJZk1qA9.jpg)

The realtime data give a Fault code:
![realtime data|690x420](upload://sFUDt21UVw4CdcCgLNjmtikro4z.png)

Now i don't know if the VESC is broken or if there is a way to fix this problem. If it's broken, then : WHAT!!! 100 BUCKS??? Any help would be appreciated!
```

---
## \#2 Posted by: ShutterShock Posted at: 2018-01-18T04:23:39.632Z Reads: 96

```
It looks like your DRV chip got fried (DRV8302 fault code).  Could you look into your motor and check all your connections and possibly see if any of the leads have shorted out against each other? 

When you said you felt resistance even with no power, the only thing I could think of is that two motor leads are touching one another.  That will kill your DRV for sure.
```

---
## \#3 Posted by: SkateYS Posted at: 2018-01-18T04:28:13.260Z Reads: 92

```
Not sure if those wires touched one other! because they re pretty well wrapped up! Do you think there is a fix for that, or do i need a new VESC?
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2018-01-18T04:29:59.795Z Reads: 89

```
Try to unplug your vesc and then spin the motor, if you feel resistance then your motor is shorted, and as of now you probably have 2 choices, get your DRV repaired or get a new vesc. Your DRV is pretty much toast, but find out the problem so if you plug in it vesc again it doesn't blow a 2nd time.
```

---
## \#5 Posted by: ARetardedPillow Posted at: 2018-01-18T04:31:08.662Z Reads: 85

```
Also what type of motor are you running? Those phase wires look really really thin
```

---
## \#6 Posted by: SkateYS Posted at: 2018-01-18T04:32:26.037Z Reads: 78

```
the resistance stops right away when i unplug the VESC tree wires! Where can i get a DRV fixed?
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2018-01-18T04:33:49.027Z Reads: 75

```
Hmm, take it to @scepterr to get it checked out, sounds like a weird problem.
```

---
## \#8 Posted by: SkateYS Posted at: 2018-01-18T04:33:56.694Z Reads: 75

```
Yeah, it's the motor of the yuneec E-GO, low top motor! but handles my 10s so!!!
```

---
## \#9 Posted by: scepterr Posted at: 2018-01-18T04:38:41.617Z Reads: 72

```
Should get you a frequent visitor pass :laughing:
```

---
## \#10 Posted by: SkateYS Posted at: 2018-01-18T04:39:52.574Z Reads: 72

```
:rofl: Clearly!
```

---
## \#11 Posted by: SkateYS Posted at: 2018-01-18T04:48:19.469Z Reads: 66

```
Are you available sundays?
```

---
## \#12 Posted by: scepterr Posted at: 2018-01-18T04:51:25.447Z Reads: 64

```
Yeah 12-6.
```

---
## \#13 Posted by: SkateYS Posted at: 2018-01-18T04:54:23.798Z Reads: 62

```
Okay, cool! I wish i could come sooner, i can't deal with the fact that i can't ride it! See you !
```

---
