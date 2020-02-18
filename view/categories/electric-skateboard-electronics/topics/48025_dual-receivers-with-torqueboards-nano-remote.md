# Dual receivers with torqueboards nano remote

### Replies: 29 Views: 1170

## \#1 Posted by: Da_gree Posted at: 2018-03-03T13:53:57.062Z Reads: 161

```
I somehow fried my last two 4.12 VESC's while setting up CANBUS connection. I spent hours reading the threads about CANBUS vs. split ppm, and it would appear the issue is still unresolved. I just received my repaired VESCs and am still trying to put together a dual build. I happen to have an extra receiver for my nano remote. I know it's possible to run to receivers with the mini remote and the GT2b. Does anyone know if that will work with the Nano?
```

---
## \#2 Posted by: Tuomalar Posted at: 2018-03-03T14:15:15.165Z Reads: 157

```
But why you just don’t use canbus or ppm? You definitely wired something wrong if neither of those doesn’t work.
```

---
## \#3 Posted by: Bjork3n Posted at: 2018-03-03T14:21:25.995Z Reads: 155

```
i also fried one of my vesc from torqueboards, did everything to the letter as diyelectricskateboard manual suggested.
Torqueboard vesc fried and maytech vesc still going strong. 
Will contact diyelectricskateboard on monday... 

I get that vesc fries using FOC or user error but i swear i did nothing wrong and it still fried, cheap components? Manufacture fault?
```

---
## \#4 Posted by: Da_gree Posted at: 2018-03-03T15:31:51.071Z Reads: 139

```
I fried both VESCs through the CANBUS - diyelectric informed me that there is an occasional recurring problem with their CANBUS connections on 4.12 VESC and replaced both VESC for a lower price. I don't want to connect via the CANBUS again with these boards. I was going to do split ppm, but apparently there is a lot of resistance to that idea from Vedder himself.
Using two receivers seems like a great solution to me for redundancy and simplicity.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-03-03T16:06:15.403Z Reads: 121

```
Split ppm is perfectly safe on Vesc 4
Just be sure to cut the red wire from one of the Vescs and power the receiver by one Vesc. 
And set them both up as masters. 
I have been running this setup since day 1 with never an issue.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-03-03T17:26:39.152Z Reads: 113

```
Hey guys, it’s ok to talk publicly  about problems with hardware but publicly complaining about vendors is not ok
Please keep this in mind when posting here.
```

---
## \#9 Posted by: Namasaki Posted at: 2018-03-03T17:56:50.176Z Reads: 104

```
Using canbus is risky. If the 2 Vescs don’t power up at the same instant, poof. 
If the canbus connection isnt 100% solid, poof. 
If you don’t get the settings just right, poof. 
This is why I don’t use canbus and why I recommend using split ppm or dual receiver instead
```

---
## \#10 Posted by: Namasaki Posted at: 2018-03-03T18:01:07.745Z Reads: 100

```
[quote="Bjork3n, post:3, topic:48025"]
Torqueboard vesc fried and maytech vesc still going strong.
[/quote]

When you have a canbus issue, it may fry only one Vesc.
```

---
## \#11 Posted by: Bjork3n Posted at: 2018-03-03T18:04:31.411Z Reads: 99

```
Thats correct, it was the slave vesc (torqueboards) that got the DRV fault.
All settings was correct and wires was properly seated.

I want all the features canbus gives... Ability to use the METR app and switch modes and such.
```

---
## \#12 Posted by: abenny Posted at: 2018-03-03T18:05:00.487Z Reads: 97

```
I agree with @Namasaki . Just like you @Da_gree , the first time i tried to set up my dual motors i connected by canbus and ended up blowing a drv chip  (because i didnt set it up correctly)... after my repair i ended up using a split ppm connector with no problem
```

---
## \#13 Posted by: Bjork3n Posted at: 2018-03-03T18:34:56.407Z Reads: 91

```
Didnt know this was a issue... so i have to sacrifice all the canbus features, live data , mode switch to get reliability?
```

---
## \#14 Posted by: Da_gree Posted at: 2018-03-03T18:39:44.806Z Reads: 91

```
Apologies if that was directed at me. The vendor treated me very well, and I'm perfectly happy with the outcome.
```

---
## \#15 Posted by: Namasaki Posted at: 2018-03-03T18:43:12.606Z Reads: 86

```
[quote="Da_gree, post:14, topic:48025"]
Apologies if that was directed at me.
[/quote]

It was not directed at you.
```

---
## \#16 Posted by: Namasaki Posted at: 2018-03-03T18:57:49.863Z Reads: 87

```
[quote="Bjork3n, post:13, topic:48025, full:true"]
Didnt know this was a issue… so i have to sacrifice all the canbus features, live data , mode switch to get reliability?
[/quote]

You can still get live data from one Vesc 
Which is what I do and it’s good enough for me. 
As for adjustments and modes , you could stil do that by having 2 modules, one for each Vesc and just connect to each one separately to make adjustments. 
I know it’s somewhat redundant but it would be dependable.
```

---
## \#17 Posted by: Bjork3n Posted at: 2018-03-03T19:36:12.142Z Reads: 83

```
But it still seems that most people use canbus with no issues, I have no idea what caused mine to blow. 
It must be manufacture fault, I mean what settings would cause it to blow?
```

---
## \#18 Posted by: Namasaki Posted at: 2018-03-03T19:43:38.370Z Reads: 82

```
Your not the first to have issues with canbus. There are other threads with accounts of this.
Canbus is just risky in an esk8 application where vibration and bumps are a problem.
The connector can work loose and cause a failure.
It may not happen in all cases but it is always a possibility.
```

---
## \#19 Posted by: Bjork3n Posted at: 2018-03-03T19:47:18.892Z Reads: 77

```
I can guarantee all connectors was seated so what setting can cause the issue? Just can't be random?
```

---
## \#20 Posted by: Namasaki Posted at: 2018-03-03T19:59:12.159Z Reads: 78

```
Just because they are fully seated doesn't guarantee that the little male pins are fitting tightly in the little female receptacles 
Also if both Vescs don't boot up at exactly the same time it can cause a canbus failure.
And the settings:
You have to assign a a  controller id to each vesc
Only one of them has multiple esc's over can checked
And only one of them has send status over can checked
And it matters which one has each though I can't remember which.
```

---
## \#21 Posted by: torqueboards Posted at: 2018-03-04T08:46:43.166Z Reads: 67

```
@Namasaki - I do not sell maytech VESCs. Just FYI :)
```

---
## \#22 Posted by: Bjork3n Posted at: 2018-03-04T11:05:05.729Z Reads: 63

```
Everything was correct, promise you.

If you use ppm split then you have to set up the controller on each vesc with the exact same settings (values input min and max etc) right? 
Except that one can have ppm + uart.
```

---
## \#23 Posted by: Namasaki Posted at: 2018-03-04T14:39:18.780Z Reads: 53

```
My mistake, sorry for that.
I have edited my post.
```

---
## \#24 Posted by: Da_gree Posted at: 2018-03-05T21:01:39.626Z Reads: 48

```
just to come full circle, I wound up doing split-ppm. I soldered just an extra signal wire for the second VESC, and it seems to be working fine. I don't think I'll be trying to make another CANBUS connection until I'm more comfortable with the software.
```

---
## \#25 Posted by: Bjork3n Posted at: 2018-03-05T21:02:24.499Z Reads: 51

```
I'm also going to ppm route, seems most reliable.
```

---
## \#26 Posted by: Bjork3n Posted at: 2018-04-23T11:08:11.931Z Reads: 48

```
Hey man!
Just a question regarding the split ppm .
You had one remote connected to 2 receivers right? 

Mini-remote and 2 receivers? 
This must be to absolute safest way to get a realiable board.

I use split ppm but yesterday my remote disconnected during rapid acceleration and i flew off.... 
Seems like its getting worse and worse so im guessing my reciver is going bad... Using maytech (eskating v2) remote.

Thinking of going the mini-remote with 2 recivers route.


Lucky me i was wearing full protection. ![crash remote|375x500](upload://yyPJjqmmwCFOfeC27V7KD49Tp4b.jpg)
```

---
## \#27 Posted by: banjaxxed Posted at: 2018-04-23T11:27:03.258Z Reads: 47

```
the pins may not be keeping a good connection with the receiver when vibration happens. it's a good idea to hardwire or hot glue them. you also should ensure that the vesc setting for disconnected state is to power down

http://www.electric-skateboard.builders/t/vesc-goes-full-throttle-when-remote-disconnects/30756

http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116

see section 'Timeout Behavior'
```

---
## \#28 Posted by: Namasaki Posted at: 2018-04-23T11:51:37.763Z Reads: 38

```
[quote="Bjork3n, post:26, topic:48025"]
Mini-remote and 2 receivers?
[/quote]
Yes, I bound the remote to one receiver then pulled the binding plug and turned that receiver off then turned the remote off. 
Then repeated those steps with the 2nd receiver. 
Then power up both receivers and then turn on the remote.
```

---
## \#29 Posted by: Bjork3n Posted at: 2018-04-23T12:10:37.639Z Reads: 37

```
Great!
Think i will go this route, then nothing should fail! Im going to be unstoppable! :joy:
```

---
## \#30 Posted by: Namasaki Posted at: 2018-04-23T15:03:03.697Z Reads: 31

```
@zelectric is running dual receivers with one Mini remote and as far as I know he has had no issues.
```

---
## \#31 Posted by: zelectric Posted at: 2018-04-23T16:27:15.744Z Reads: 29

```
Works great since day 1!  Thanks for hooking me up...litterally.
```

---
