# Focbox DRV fault ? Please help

### Replies: 23 Views: 362

## \#1 Posted by: PickSix24 Posted at: 2018-12-15T20:21:28.464Z Reads: 100

```
Noticed during my ride today these faults popped up while checking my Xmatic app. I believe I know when they happened as I felt a slight jerking while at speed both times. If I recall it happened right after I let off the throttle when I was applying throttle again. Happened once on each 3mi ride. Rode fine afterwards. 
I have the screenshots from Xmatic and I’ll try to plug my Focboxes into my computer later. Can anyone shed some light on this ? Thanks !!!![image|281x500](upload://sThg5JhjPtuRFRVlliHGyI4wk1l.jpeg) ![image|281x500](upload://kjudLTio4pFAK3GPWwtfiUtEOJz.jpeg)
```

---
## \#2 Posted by: PickSix24 Posted at: 2018-12-15T20:47:45.616Z Reads: 82

```
Update: I hooked both Focboxes to my computer using the Vesc tool. Went into terminal and typed “fault” and “faults”  both came back with no faults. So.. this is a good sign I guess but now I’m wondering why Xmatic is generating a drv fault and what that stutter/jerking  I felt while riding.
```

---
## \#3 Posted by: PickSix24 Posted at: 2018-12-16T15:34:37.902Z Reads: 67

```
So if Vesc Tool is reporting no faults does that mean the Xmatic app is incorrect ? Could this be the DRV chip going bad ?
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-16T16:17:37.097Z Reads: 63

```
I had similar thing, my terminal didn’t showed a fault even when there was a know drv fault on the focbox.
The fault was shown via davega display, but nothing in the terminal.
If you power up your focbox, does a res light blinking?
Did you try to do a motor detection?
Sometimes faults just displayed after you started a motor detection.

If everything is working now fine but you had a drv fault while driving, I would highly recommend you to check all connections and wires.
Could be you have a short somewhere or something similar which can fry you drv totally on the next ride.
```

---
## \#5 Posted by: PickSix24 Posted at: 2018-12-16T19:04:56.856Z Reads: 55

```
No blinking lights , I haven’t tried a motor detection yet. I can ride the board fine right now but whatever is going on causes a stutter in the motors then rides fine
```

---
## \#6 Posted by: Blasto Posted at: 2018-12-16T19:06:36.647Z Reads: 56

```
[quote="PickSix24, post:5, topic:78107"]
I haven’t tried a motor detection yet.
[/quote]

Well..... there’s your problem
```

---
## \#7 Posted by: PickSix24 Posted at: 2018-12-16T19:09:04.991Z Reads: 55

```
So am I better off leaving it alone til it stops working completely or run a motor detection and then have a non working board ?
```

---
## \#8 Posted by: Blasto Posted at: 2018-12-16T19:09:56.558Z Reads: 51

```
Your getting faults because you didnt run a motor detection, the focbox needs to know your motor parameters to run properly
```

---
## \#9 Posted by: PickSix24 Posted at: 2018-12-16T19:32:50.191Z Reads: 51

```
Motor detection was done on the initial board setup. I thought the post above was saying that in order to read the fault I should run the motor detection again.
```

---
## \#10 Posted by: b264 Posted at: 2018-12-16T19:36:29.041Z Reads: 52

```
Did you turn the board off between typing on the terminal and seeing the message on the "app"?
```

---
## \#11 Posted by: PickSix24 Posted at: 2018-12-16T19:41:48.842Z Reads: 48

```
Yes , I thought the fault codes would be saved but I’m guessing that’s not the case
```

---
## \#12 Posted by: mtuan293 Posted at: 2018-12-16T19:42:45.565Z Reads: 47

```
I think the VESC won’t store the faults. It just reports in real time. If you were able to hook up VESC tool while riding then you would see the fault just like the Xmatic app reported.
```

---
## \#13 Posted by: b264 Posted at: 2018-12-16T19:44:32.102Z Reads: 49

```
This is 12S, right?

Also what is your motor kv and gearing ratio and wheel diameter
```

---
## \#14 Posted by: PickSix24 Posted at: 2018-12-16T19:46:45.867Z Reads: 49

```
10s , 15t / 66t on 8” AT ,  200kv
```

---
## \#15 Posted by: Andy87 Posted at: 2018-12-16T19:48:31.519Z Reads: 46

```
Yes it’s not the case.
You need to look up the faults after motor detection, without to switch off inbetween.
```

---
## \#16 Posted by: PickSix24 Posted at: 2018-12-16T20:03:50.350Z Reads: 38

```
Ok so if there is an actual fault happening , running another motor detection should pick it up ?
```

---
## \#17 Posted by: Andy87 Posted at: 2018-12-16T20:06:28.641Z Reads: 39

```
Probably yes. In my case it wasn’t listed under faults even after I tried to run a motor detection.
Still nobody could answer me why.
```

---
## \#18 Posted by: PickSix24 Posted at: 2018-12-16T22:10:42.949Z Reads: 36

```
Just ran motor detection on both motors , no faults. I’m gonna wait until it happens again and then hope I can get it plugged in to my computer before shutting off the board.
```

---
## \#19 Posted by: Thelifelonglearner Posted at: 2019-08-10T17:29:07.058Z Reads: 16

```
Did you ever find out what was the issue with the DRV fault ? I had the same issue and I lost my connection for 3 secs and now my board is working fine however, I am afraid if it happens again while am riding ?
```

---
## \#20 Posted by: PickSix24 Posted at: 2019-08-10T18:12:10.844Z Reads: 16

```
Never did get it to repeat after I reran the motor detection again.
```

---
## \#21 Posted by: Thelifelonglearner Posted at: 2019-08-11T06:29:41.029Z Reads: 12

```
Mine is working fine now and connection is solid. Do you reckon running a motor detection will be a safe move or not necessary ?
```

---
## \#22 Posted by: PickSix24 Posted at: 2019-08-11T15:18:12.288Z Reads: 10

```
If your good now I’d leave it. Don’t fix what isn’t broke ;)
```

---
## \#23 Posted by: Thelifelonglearner Posted at: 2019-08-11T16:53:07.439Z Reads: 7

```
I still want to know why I lost that connection for 3secs where I could neither brake or accelerate because that could happen again. 
I am not sure if it was a DRV fault because my other motor should still be able to accelerate as it can’t affect both motors.
Thoughts would be appreciated.
Thanks
```

---
