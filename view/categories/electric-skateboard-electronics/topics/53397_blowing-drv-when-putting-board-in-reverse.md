# Blowing DRV when putting board in reverse

### Replies: 10 Views: 347

## \#1 Posted by: Squidprorow Posted at: 2018-04-24T21:45:31.393Z Reads: 76

```
I've gotten two DRV errors both caused by putting the board in reverse when at a stand still. Before the chip goes I heard a pop sound both times. Why is this happening?!?!?

Notes about setup:
VESC from TorqueBoards
set to current control
10s4p Li Ion battery
BLDC motor control
6374 motors with motor max set to 80a
All other VESC settings left at TorqueBoards default

Please help me, i'm so lost.
```

---
## \#2 Posted by: RedEagle Posted at: 2018-04-24T21:54:56.133Z Reads: 72

```
You need to post screenshots of your vesc settings.
```

---
## \#3 Posted by: Squidprorow Posted at: 2018-04-24T23:44:06.172Z Reads: 62

```
![03 PM|689x384](upload://ohnWlPEry8a5KVUpyM9723l6oMe.png)![51 PM|690x385](upload://37TRlP6i7pkhyd5oecG8tsvAcmX.png)![25 PM|689x380](upload://zvyIuVOXj6p8Md0pXQaICRQ4Yf0.png)![35 PM|690x381](upload://a1hCdpqR7n1EkwNN4cKzWHqQpMJ.png)
```

---
## \#4 Posted by: RedEagle Posted at: 2018-04-24T23:59:03.248Z Reads: 50

```
Slave vesc should have send status over can enabled. 
Did you do a successful detection?
```

---
## \#5 Posted by: E1Allen Posted at: 2018-04-25T01:26:34.531Z Reads: 42

```
What do you mean erpm limit should be checked?
```

---
## \#6 Posted by: RedEagle Posted at: 2018-04-25T01:29:06.382Z Reads: 43

```
Whoops... Nevermind. It was a typo. 
Limit erpm should always be unchecked. Lol.
```

---
## \#7 Posted by: E1Allen Posted at: 2018-04-25T01:40:36.777Z Reads: 41

```
Was making sure we were on the same page
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2018-04-25T01:49:21.533Z Reads: 38

```
Motor detection failed?
```

---
## \#9 Posted by: Squidprorow Posted at: 2018-04-25T02:22:53.386Z Reads: 36

```
Motor detection did not fail either of the VESCs that were on the board when the DRV chip blew. Both seemed to be working fine. The screen shots I shared have the same settings, only I was trying to set up another VESC that was having problems with motor detection when I took the screenshots.
```

---
## \#10 Posted by: seanray007 Posted at: 2018-04-25T02:36:13.019Z Reads: 33

```
I had same popping sound  and it stopped working I tried replacing the capacitors with no luck
```

---
