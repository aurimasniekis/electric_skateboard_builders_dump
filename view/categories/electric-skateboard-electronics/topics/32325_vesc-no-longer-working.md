# VESC No Longer Working

### Replies: 20 Views: 941

## \#1 Posted by: kuphjr Posted at: 2017-09-05T12:49:41.795Z Reads: 167

```
So I just got my board working and I have ridden over 30 miles, but when I plugged in my VESC to the battery this morning, the blue power LED would not turn on.  I tested the batteries with my volt meter and they are at full charge (42 volts for my 10s x2 Zippy Flightmax 5s 8000mah setup).  I tried different batteries and I tried only using one battery, but still no luck.

The RC transmitter starts and connects just fine, but the VESC won't turn on and nothing happens when I hit he throttle.

I have checked all the solder connections and they all appear to be fine.  This would make sense since the light on the RC transmitter turns on without a problem.

I tried plugging the VESC into my computer, but I get a "No Firmware Read Response" error.

Did I short something out? Is there any recommendations anyone can give me for how to fix this?

Thanks!
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-09-05T13:17:11.617Z Reads: 157

```
Can you provide pics of your setup. Is there a switch or anti spark in between the vesc and battery? Is the receiver powered by the vesc or separate bec?
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-09-05T13:52:55.954Z Reads: 148

```
Make sure your switch did not go bad. This has happened to me a few times.
```

---
## \#4 Posted by: kuphjr Posted at: 2017-09-05T15:29:24.510Z Reads: 130

```
I will send pictures as soon as I get home. There is no switch or anti spark. I plugged it directly into the battery. The receiver is power by the BEC.
```

---
## \#5 Posted by: kuphjr Posted at: 2017-09-05T15:30:27.717Z Reads: 127

```
Are you referring to a power switch for the board itself? I do not have a switch. I plug directly into the VESC from the battery. Is that bad?
```

---
## \#6 Posted by: kuphjr Posted at: 2017-09-05T15:32:14.994Z Reads: 121

```
I'm really worried I somehow fried the VESC. Is that possible? How could this have happened? All the original shrink tubing is on the VESC.
```

---
## \#7 Posted by: i2oadsweepei2 Posted at: 2017-09-05T15:45:52.016Z Reads: 113

```
Just to be clear, you are using a separate bec? and you have disconnected the 5v red wire from vesc to receiver? Or the vesc is powering the receiver? I ask because if you are using the vesc to power the receiver then power is definitely getting from the battery to the vesc and it may be fried. If not and you are using a separate bec then the connector or solder joint for the connector may be faulty.

edit: Also is it an anti spark connector?
```

---
## \#8 Posted by: kuphjr Posted at: 2017-09-05T16:19:20.788Z Reads: 100

```
I am using the power from the BEC on the VESC to power the receiver. The receiver appears to be working just fine and is getting power from the VESC. The issue is the VESC itself will not turn on and the blue LED on the VESC is not turning on.

I am not using any anti spark connector. I just connect directly to the battery.
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-09-05T17:16:31.694Z Reads: 94

```
I was afraid to hear that. Ok pics of your setup when you can. Clear close ups of the vesc on both sides. I can't help you troubleshoot any further, but there are many who can. This is beyond my knowledge now. Best of luck to you.
```

---
## \#10 Posted by: kuphjr Posted at: 2017-09-05T18:36:16.143Z Reads: 93

```
<img src="/uploads/db1493/original/3X/2/f/2f73d2acb45270762d3e3e593c71957a0849cb60.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/4/04b508f6316ebdcec6da70f434be71f46c8be4ee.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/f/6/f6d6d66ce92ad87a5055a4daa1d2cdf4d1b023fa.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/f/f/ff1f28e15ad631a6d7714c235be681a85dcaf1a5.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/d/1d09a7afc27e77c2ecd7399067872172e7df434c.JPG" width="375" height="500">
```

---
## \#11 Posted by: kuphjr Posted at: 2017-09-05T18:41:08.633Z Reads: 89

```
<img src="/uploads/db1493/original/3X/0/7/0717e8c1c85b660914d29d02808dce16ea76a08c.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/5/d/5d39aa918799de42516b86bf92e851ec7e0dca57.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/a/4/a4baf560f973abb1af48bf93077900d983cd68e0.JPG" width="375" height="500">I took off the heatshrink and I can't see any damage on the VESC itself.
```

---
## \#12 Posted by: qq404041481 Posted at: 2017-09-05T20:49:12.562Z Reads: 82

```
hey I am a EE engineer in college. If you have devices. I can help you through this or you can send me the board I can fix it for you.
```

---
## \#13 Posted by: kuphjr Posted at: 2017-09-05T21:15:27.178Z Reads: 81

```
Really? I'd definitely do that if you want. How do you want me to get in contact with you so I can get your shipping address?  I don't really have much for tools at my apartment right now (I am also in college) and I am pretty bad at soldering. :confused: 

Is this an issue you have seen before or know something about?
```

---
## \#14 Posted by: i2oadsweepei2 Posted at: 2017-09-05T22:41:00.449Z Reads: 78

```
I don't mean any disrespect but I would not hand over my vesc to someone I don't know that just joined the forum 20 hours ago. There is a repair guy here in Montreal Canada that might be able to help you out. He may even know what's wrong by seeing your post and pics @JohnnyMeduse. Where did you buy your vesc from?
```

---
## \#15 Posted by: kuphjr Posted at: 2017-09-05T23:55:02.724Z Reads: 75

```
Lol probably a good call. I'm feeling pretty desperate at the moment and honestly. I don't have any cash left in the budget for a new VESC and a broken VESC is worth about as much to me as no VESC at all.  Unless I can maybe sell it for parts or repair and use the money to buy a new one.
```

---
## \#16 Posted by: kuphjr Posted at: 2017-09-05T23:56:09.128Z Reads: 74

```
I got my VESC from DIYelectricSkateboards.com.
```

---
## \#17 Posted by: i2oadsweepei2 Posted at: 2017-09-06T01:34:42.141Z Reads: 67

```
Try and get ahold of DIY's support via the online chat. Dexter has been pretty helpful to me. However things in Texas are harsh and that may have had an impact on our good friend too and I hope all is well with @torqueboards and another storm is on the way. If it's not a warranty issue that DIY can resolve then contact Johnnymeduse via pm about a repair. He is very reasonable and trustworthy.

All the best to you.
```

---
## \#18 Posted by: kuphjr Posted at: 2017-09-06T15:49:48.092Z Reads: 54

```
[quote="i2oadsweepei2, post:17, topic:32325"]
@torqueboards
[/quote]

Thank you for all your help! I'll see what I can do.  Not sure exactly how this forum works (this is my first thread), but if it needs to be closed someone can close it now.  I have all the information I think I need.
```

---
## \#19 Posted by: i2oadsweepei2 Posted at: 2017-09-06T15:52:27.945Z Reads: 52

```
Its all good. It will disappear into nothingness eventually. You can also update us on how things turn out as well.
```

---
## \#20 Posted by: qq404041481 Posted at: 2017-09-06T18:10:15.646Z Reads: 43

```
I mean I know it's kind of hard to trust people but I am just a college student trying to help. If you have right equipments. I can diagnose it for you pretty fast. Just measure if you have 5V and 3.3V (you can do it at the bottom connectors) and if you have 5v but not 3.3v, it's probably your LDO is not working, that's an easy fix. Is anything getting hot? can you measure the current going to the board?
```

---
