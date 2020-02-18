# 2nd Build (Dual Drive) COMPLETE

### Replies: 14 Views: 1097

## \#1 Posted by: MannyM0E Posted at: 2018-04-18T03:53:13.698Z Reads: 212

```
So here's my first build if you want to check out. 
Continuing the discussion from [First build (accomplished)](https://www.electric-skateboard.builders/t/first-build-accomplished/45013):


I wanna go for a dual drive this time for this second build. I have everything already to build it. Here's the list that I'll be using 

• Board •
Is a sector 9 I believe. Bought from someone from offerup

•Remote• @thisguyhere
2.4Ghz mini remote  

•Gears• @marcmt88 
40/16 

•Wheels•
100mm MBS All Terrian 

•Trucks• from @torqueboards
218mm DIY Trucks 

•Mounts• @marcmt88

•Motor• @bimmer 
6374 170kv

•VESC• @torqueboards
4.12 vesc  

•Batteries•
Using lipo ATM, waiting on tax money to come so I can try buy some 18650. Never went that route yet but will be soon
![image|375x500](upload://rkVlbQNpauKzzrnr5icEqbzp63h.jpg)

•Belt Cover• @intensivegecko
3D Printed  

•Bearings•
Reds 

•Griptape•
Jessup or however it's spilt

•Enclosure•
I'll be using one that I made. It looks kinda ugly since it was my first time trying it but it'll do the job for now 
![IMG_4053|375x500](upload://ysyArzkaBnI32xgqezekY40ULro.JPG)

Here's a picture of the board half way build. Sorry for bad pictures, it's late right now and will post better pictures tomorrow.
![IMG_4048|666x500](upload://zIue3aZ1EQZdxI3kCJTpDOS3Cnk.JPG)![IMG_4050|666x500](upload://j6DA15uiiim1DlETVnvOhBsNkYe.JPG)![IMG_4047|666x500](upload://7ZzFMr5Zsps8GNNeu8Nk8pmbz2n.JPG)![IMG_4049|666x500](upload://1FVb5uBBEqXPPFnchrlY0dmFWxU.JPG)

Only part I'm worried about is connecting both the VESC. Never tried it before, only that mono drive. I got a PPM Splitter from @JLabs and was told to remove this red wire or I could fry my vesc 
![image|375x500](upload://auydHOm3jTf2iXyO4gp0ApRZboh.jpg) 
 I guess I connect it to both VESC PPM and the other end is connected to the receiver. 
So am I missing anything here ? I read somewhere on here that if using PPM Splitter Ima have to motor detect the motor to whatever VESC it's connected to first. 
Any advice or pointers or help would be very much appreciated


UPDATE: Got it to work only problem is my enclosure isn't gulley bolted due to bolts not long enough on the side because of the boards curve .

SETUP FOR EACH VESC: 
Motor Max 40a
Motor Min 30a
Batt Max 20a
Batt Min .04 

Is this a good setup for the vesc I'm using ?

![IMG_4066|690x387](upload://hksIBLmeUmXsbj6FeJmWXvvVdL9.JPG)
```

---
## \#2 Posted by: mmaner Posted at: 2018-04-18T04:01:28.784Z Reads: 173

```
Remive the +5 volt from the PPM cable left that is going to the 2nd vesc and you are good. Do your motor detections in at a time, just use the primary side of the split PPM cable on the VESC's that you are doing the detection on. 

That being said, can is really the way to go, better control and as long as you do it properly it's better for the VESC's. The problem most people have is doing it properly. 

> 1. With can connected only power both VESC's, never singly. 
> 2. Before can is connected so detections in each motor with the veac connected to the given motor. 

That's all there is to it.
```

---
## \#3 Posted by: MannyM0E Posted at: 2018-04-18T04:06:29.459Z Reads: 160

```
On the motor detection part, can't I just motor detect it first on the first motor on the first VESC then motor detect the second motor onto the second VESC, THEN plug in the PPM Spillter ? Or do I have to motor detect them with the PPM Spillter on ?
```

---
## \#4 Posted by: torqueboards Posted at: 2018-04-18T04:08:52.767Z Reads: 149

```
You can detect without the Canbus on. I'd recommend that as people have fried the canbus. Then connect canbus when you are ready to test the board after programmed.
As for the PPM Splitter, it doesn't matter.
```

---
## \#5 Posted by: mmaner Posted at: 2018-04-18T04:19:41.396Z Reads: 144

```
That is correct, I just didn't do a good job if explaining.
```

---
## \#6 Posted by: MannyM0E Posted at: 2018-04-18T04:22:44.365Z Reads: 146

```
Will this work for connecting both VESC into the batteries? 

![image|375x500](upload://xnjrHTuBLJGuk98HpyxZduzCY2j.jpg)
```

---
## \#8 Posted by: mmaner Posted at: 2018-04-18T11:49:46.652Z Reads: 128

```
Yep, looks good.
```

---
## \#9 Posted by: MannyM0E Posted at: 2018-04-18T12:56:31.091Z Reads: 124

```
I have a gt2e receiver also a mini remote trigger receiver. I seen @Namasaki post somewhere where he used 2 receivers. Will I be able to with these two receivers that I have work ?
```

---
## \#10 Posted by: mmaner Posted at: 2018-04-18T13:05:38.958Z Reads: 128

```
I don't think so, I think you have to use the mini-remote with dual receivers.
```

---
## \#12 Posted by: MannyM0E Posted at: 2018-04-20T04:44:48.972Z Reads: 101

```
@torqueboards @mmaner @Namasaki @JLabs @Mikenopolis  and anyone else that I didn't mention  
Thanks for the inputs it helped out
Are my setting on my VESC okay ?
```

---
## \#13 Posted by: Mikenopolis Posted at: 2018-04-20T05:47:14.544Z Reads: 96

```
I would not listen to me since these numbers are still up in the air until I get my FocBox back after a fault. But this is what I was using on dual 6374. ![image|690x308](upload://83clVVwXuvVVOGCEY9N9fHC1gnb.jpeg)
```

---
## \#14 Posted by: mmaner Posted at: 2018-04-20T10:36:58.984Z Reads: 84

```
That's exactly what I start with, then test and adjust.
```

---
## \#15 Posted by: Mikenopolis Posted at: 2018-04-20T17:56:22.444Z Reads: 73

```
I noticed this XT splitter that Ernesto (KalyNYC) posted. Don’t know why we didn’t think of doing it like this, I’m gonna make these for my board to get rid of the wire clutter I have with Y splitters
![image|569x315](upload://9oFPKdjJurjcbLM7xhhHDnd9MkM.jpeg)
```

---
## \#16 Posted by: MannyM0E Posted at: 2018-04-24T03:26:25.113Z Reads: 57

```
Came home from work today and realized my motors were really hot to a point where I can hold it. My motor max is set at 50a each. Should I go for 45a ?
```

---
