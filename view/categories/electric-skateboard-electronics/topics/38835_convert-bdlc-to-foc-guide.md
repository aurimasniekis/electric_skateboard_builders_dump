# Convert BDLC to FOC guide?

### Replies: 20 Views: 1497

## \#1 Posted by: trigger4point7 Posted at: 2017-11-20T18:27:09.987Z Reads: 206

```
I've looked around a bit, and haven't found anything, but do y'all know a good guide of converting BLDC settings to FOC?
```

---
## \#2 Posted by: FredrikHems Posted at: 2017-11-20T18:45:39.107Z Reads: 206

```
Well then you havent looked good enought. There is 10's of threads Where it is described with both text and photos
```

---
## \#3 Posted by: trigger4point7 Posted at: 2017-11-20T19:44:38.164Z Reads: 207

```
Alright dude, if you going to be smart about it just don't answer the question.
```

---
## \#4 Posted by: lasplaner Posted at: 2017-11-21T10:06:19.693Z Reads: 190

```
I'm no expert, but the conversion is relatively simple. This guide may serve as a general guide for FOC converters.

A few things to note: 

- Make sure your **ERPM limit is less than 60,000**, or you will likely fry your DRV chip, as many VESC users have (including me, but not because of this reason). Set this in the **PPM tab** of your **App Configuration**, if you use PPM. If you aren't, then I don't know how to set it. (Ignore other settings with 0, focus in the red box)
<img src="/uploads/db1493/original/3X/7/7/774e0d1d4446f8537df9099639da691afa861fbb.png" width="690" height="250">
- If you're running 12S, and using FOC, don't. The chances of DRV failure will be much higher. As I am light, and don't require much power, 6S suffices for me, and FOC runs flawlessly (so far, don't quote me). I wouldn't even use FOC on 10S to be honest.
- The loud motor noise in the FOC detection is completly normal. Don't panic like I did, when it made that sound!

Assuming that all settings work with BLDC, and that you have set:

(Click _Read Configuration_ on the Bottom Left of BLDC Tool before continuing)

1. **Motor Amps** in **Motor Configuration -> Motor -> Current Limits** (Motor Max and Motor Min). You should test this, but start from around **30A in 6S**, or **25A in 8-10S**, and work your way up 5A at a time to a suitable number. A higher number is fine. You can observe the amps this in the "_Realtime Data_" tab. You should have already done this. Also, Motor Max should equal Motor Min (regen). Ignore my "0" Values.
2. **Voltage Limits**. Get your voltage "Cell" number, and multiply by 3.4 to get **Battery Cutoff Start**, and by 3.2 to get **Battery Cutoff End**. So if you are on 6S, then BCS = 6X3.4 = 20.4, and BCE is 6X3.2 = 19.2. You can set values slightly higher, and get better battery cycles (amount of functional discharge and charges), but at the expense of lowering your range. Leave the **Minimum/Maximum Input Voltage** at **6V** and **54V** respectively. Again, ignore my "0" Values.
3. Don't set your ERPM Limits in the Motor tab.
<img src="/uploads/db1493/original/3X/4/2/42f5ad7cb8dc347a021e79285de4f83facc293a0.png" width="690" height="231">

(Click _Write Configuration_ after done. Make sure it says "Write Successful")

One last time: Make sure you can operate using BLDC before trying FOC. There are many guides out there, just search on this website / Torque Boards youtube channel.

You can now set up FOC mode, finally!

1. In the box that says _"Motor Type"_, select **FOC**.
<img src="/uploads/db1493/original/3X/b/8/b8de3eb84f4d7e15e3aa21b6241b433b482ed7a3.png" width="172" height="49">
2. Go to **Motor Configuration -> FOC**, and detect and apply the following parameters in order, making sure to wait until something happens:
 - Measure R and L
 - Measure λ
 - Apply, on the same row as Measure R and L
 - Calc CC
 - Apply, on the same row as Calc CC.
3. Select "Sensorless" in the yellow box, if you don't have a sensored motors. If you have Hall Sensors, select "Hall" and click "measure" in the blue box. Then hit the "apply" in the blue box. Also, if you are running Sensored motors, set the Sensorless ERPM to 3000, as you won't need the sensors after that speed. Also, it wastes power, reduces speed, and increases noise, if you don't set it to 3000. 
<img src="/uploads/db1493/original/3X/c/a/caa360e2a3f97964cf3b5001e25d0ea8f339dcb8.png" width="690" height="473">
4. Click Write Configuration here | , and test the motor(s) on bench (without you standing on it). Then run a test. Don't push the board too hard at first. If there are no issues, feel free to push the board harder, and to increase Motor Min/Max values (but not above your motor specification).

Assuming you got the settings right, **you now have a FOC-enabled board!** 

P.S. In response to that d*ckhead who is being a smartass, I am sick (not annoyed, but I feel bad) of seeing people disorientated, like I was, while setting up their board (esp. VESC, a $100+ piece of equipment). **I belive it is our responsibility as an esk8 community, to help others** who spend huge amounts of money on their boards and parts, and do not want to risk breaking goods/injuring themselves. Sometimes looking at other posts doesn't answer your question, and may misguide or mislead you. If you don't have something to say, **don't say it.**

Extra info on FOC. Great resource, maybe could have linked to it?
http://www.electric-skateboard.builders/t/the-difference-between-motors-commutation-bldc-vs-foc-trapeziodal-sinosuidal/3002

-lasplaner
```

---
## \#5 Posted by: trigger4point7 Posted at: 2017-11-21T18:43:25.277Z Reads: 142

```
Um... Damn dude. Not an expert huh?? Thanks for all this info, super helpful!
```

---
## \#6 Posted by: trigger4point7 Posted at: 2017-12-03T18:46:53.199Z Reads: 137

```
[quote="lasplaner, post:4, topic:38835"]
Get your voltage "Cell" number, and multiply by 3.4
[/quote]

Is this the nominal battery voltage? So this may differ based on the cell?
```

---
## \#7 Posted by: yaca Posted at: 2017-12-03T20:13:33.632Z Reads: 121

```
No, nominal voltage of Lipo is 3.7V and Li-Ion has 3.6V (I'm not sure but maybe some have higher nominal voltages)

[quote="lasplaner, post:4, topic:38835"]
Get your voltage "Cell" number, and multiply by 3.4 to get Battery Cutoff Start, and by 3.2 to get Battery Cutoff End
[/quote]

I wouldn't go with this low values for Lipo batteries. For Lipo I have for Cutoff Start 3.6V and for Cutoff End 3.4V. This is recommended by @ackmaniac. For Li-Ion battery he set 3.0 and 2.8 in his ESC Tool, but I have no experience with Li-Ions.
```

---
## \#8 Posted by: XIII Posted at: 2017-12-03T20:47:17.985Z Reads: 104

```
flashing new firmware before switching is also a must (maybe somoene said it before me)

and I have had 3 drv error's because of vesc running FOC and all while doing a sharp turn....
Since I unchecked the traction controll, I have never had a drv fail on 10s ( now i'm good for between 500-800 km I would guess)
```

---
## \#9 Posted by: yaca Posted at: 2017-12-03T20:59:33.063Z Reads: 101

```
[quote="XIII, post:8, topic:38835"]
flashing new firmware before switching is also a must (maybe somoene said it before me)
[/quote]

 ... and some say it's a myth. :slight_smile:
```

---
## \#10 Posted by: XIII Posted at: 2017-12-03T21:19:54.831Z Reads: 98

```
well it could be, but it's 2 min work and you start from a nice new platform which is always a win
```

---
## \#11 Posted by: b264 Posted at: 2017-12-03T21:30:05.064Z Reads: 96

```
[quote="XIII, post:8, topic:38835"]
flashing new firmware
[/quote]

Perhaps it'd be a good idea to link to more information about where to get this
```

---
## \#12 Posted by: trigger4point7 Posted at: 2017-12-03T21:34:19.516Z Reads: 95

```
FOC honestly sounds like more trouble than it's worth. Every conversation about it references drv errors and blown up hardware.
```

---
## \#13 Posted by: XIII Posted at: 2017-12-03T22:22:46.221Z Reads: 88

```
depends, how high you value silence. I love it that people can't hear me coming at all and are like wtf is that.
```

---
## \#14 Posted by: mmaner Posted at: 2017-12-03T22:24:43.971Z Reads: 87

```
I typically don't run FOC, I have used it and really enjoy the silence but it scares me a little bit. I run hybrid mode on pretty much everything at this point.
```

---
## \#15 Posted by: trigger4point7 Posted at: 2017-12-03T23:04:19.272Z Reads: 82

```
I live in SF I hope to think it helps fewer people walk out in front of me. Haha
```

---
## \#16 Posted by: willpark16 Posted at: 2017-12-03T23:11:50.871Z Reads: 83

```
You simply haven't used the search button everything you need is already posted on other threads
```

---
## \#17 Posted by: danielz Posted at: 2017-12-04T00:25:26.574Z Reads: 77

```
I quite like the motor whine in bldc
```

---
## \#18 Posted by: briman05 Posted at: 2017-12-04T01:21:01.332Z Reads: 68

```
Maybe we should link to the threads instead of criticize him for asking a question. I had thought about running the board I will be doing in foc but am unsure because of drv fails
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2017-12-04T02:33:53.588Z Reads: 60

```
<img src="/uploads/db1493/original/3X/d/c/dc4f39d6676726650aae6fcc326d42f92469cc3d.png" width="690" height="365">
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2017-12-04T02:40:55.974Z Reads: 58

```
[quote="lasplaner, post:4, topic:38835"]
Make sure your ERPM limit is less than 60,000
[/quote]

Erpm limit only applies to BLDC. :confused:
```

---
