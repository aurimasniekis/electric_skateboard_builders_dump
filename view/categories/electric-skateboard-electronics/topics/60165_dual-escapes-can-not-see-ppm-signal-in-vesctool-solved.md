# Dual ESCapes, Can not see PPM signal in VESCtool *SOLVED*

### Replies: 10 Views: 341

## \#1 Posted by: goldrabe Posted at: 2018-06-27T00:52:29.116Z Reads: 100

```
Hi, I have set up my dual ESCapes to the point to map my signal from the Enertion Nano X. For some reason, no matter what I set, the signal is not visible. The reciever and the remote are binding fine, both have solid led's. I also tried another remote to no success. I will attach a picture of the wiring. Hope someone can help me out!
![20180627_094338|690x388](upload://aRdPP8KEkWs9DPb5BhIKxTofS7A.jpg)
```

---
## \#2 Posted by: strattos Posted at: 2018-06-27T00:55:26.880Z Reads: 91

```
Hmmm I know I had this same issue try to map the ppm signals but I have no idea what I did to fix it. I feel like you probably don't have any input methods activated in the Vesc tool and that's the issue. Honestly I can't remember
```

---
## \#3 Posted by: goldrabe Posted at: 2018-06-27T00:58:16.239Z Reads: 88

```
I have current no reverse with brakes selected, but still no signal.
```

---
## \#4 Posted by: DAddYE Posted at: 2018-06-27T00:59:17.245Z Reads: 85

```
I had issues too but with the TB Vesc. As well I’ve no idea how I fixed it. Try to pair the remote again on a different channel
```

---
## \#5 Posted by: goldrabe Posted at: 2018-06-27T01:01:26.992Z Reads: 83

```
Yeah, the Nano X comes binded already, will try to bind it again, hopefully that fixes it!
```

---
## \#6 Posted by: Blasto Posted at: 2018-06-27T01:03:22.895Z Reads: 80

```
Connect the nano-x in channel 1.

Use the app wizzard to setup the ppm
```

---
## \#7 Posted by: strattos Posted at: 2018-06-27T01:10:41.768Z Reads: 79

```
Do you have ppm+UART enabled as the control mode or just ppm either should work
```

---
## \#8 Posted by: goldrabe Posted at: 2018-06-27T01:11:15.392Z Reads: 78

```
I did that, but no signal.
```

---
## \#9 Posted by: goldrabe Posted at: 2018-06-27T01:14:24.678Z Reads: 79

```
Yes, PPM + UART. On which pin is the signal at the Nano X reciever?
```

---
## \#10 Posted by: goldrabe Posted at: 2018-06-27T09:24:51.722Z Reads: 63

```
Yeahhhh!!
Solved it. The Signal wire had a bent clip inside the JST connector, soldered a new one and everything works perfect.
Thanks for all suggestions!!
```

---
