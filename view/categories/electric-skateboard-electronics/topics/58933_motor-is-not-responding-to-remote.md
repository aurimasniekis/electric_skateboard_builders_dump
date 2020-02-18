# Motor is not responding to Remote

### Replies: 10 Views: 197

## \#1 Posted by: SyrusB Posted at: 2018-06-15T00:57:19.910Z Reads: 56

```
Here is how my connections are, I thought that everything was correct, can y'all tell me what you think I did wrong.
![IMG_20180614_204618|666x500](upload://3scJ66rrxfB7OQaQ4eSvTsT7P8n.jpg)
```

---
## \#2 Posted by: RedEagle Posted at: 2018-06-15T01:11:03.964Z Reads: 46

```
Diagram would be nice.
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2018-06-15T01:13:10.551Z Reads: 46

```
Make sure your connector going in to your receiver is the right way around and connected to channel 2
```

---
## \#4 Posted by: SyrusB Posted at: 2018-06-15T01:16:07.381Z Reads: 46

```
It is connected to channel 2 now and the right way would be the white wire to the left correct.
```

---
## \#5 Posted by: SyrusB Posted at: 2018-06-15T01:22:54.510Z Reads: 45

```
![IMG_20180614_212019|690x337](upload://nWF63HKzYOTueRsCcN0IGI1RaSX.jpg)
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2018-06-15T01:51:45.363Z Reads: 41

```
did you bind your receiver to your remote?
```

---
## \#7 Posted by: SyrusB Posted at: 2018-06-15T01:56:08.245Z Reads: 40

```
I thought that I did I might reset it and try again
```

---
## \#8 Posted by: SyrusB Posted at: 2018-06-15T02:20:04.340Z Reads: 37

```
Ok I tested it with a different Vesc and it worked, so I think the vesc is broken I bought it from @wolfgangcole
```

---
## \#9 Posted by: wolfgangcole Posted at: 2018-06-15T03:08:12.742Z Reads: 35

```
Had it working just before I sent it out so don’t blame this on me mate.
```

---
## \#10 Posted by: Mathias Posted at: 2018-06-15T06:03:32.894Z Reads: 24

```
Go into your VESC tool. It's not too hard to find out whete the problem is. 

If the VESC is broken or your motor settings are wrong then you'll get a red blinking light when you try to accelerate. If that's the case you should read out the fault from VESC tool. This will tell you what's wrong.

If you don't get a fault/red blinking light it's either your remote or app settings. Check what PPM signal the VESC gets. If it's nothing then it is your receiver. If it is stuck on neutral (1.5 ms I think) even if you pull your throttle then it's the pairing or your remote.
```

---
