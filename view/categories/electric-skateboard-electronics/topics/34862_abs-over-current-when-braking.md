# ABS_OVER_CURRENT when braking

### Replies: 23 Views: 912

## \#1 Posted by: Ishayc Posted at: 2017-10-05T18:50:31.604Z Reads: 91

```
Hi,

Got this weird issue that started today. 
After a few minutes of ride when trying to brake, most of the time it’s not working though the acceleration works but has the lack of power, like it does not deliver enough current.
I switched between a working esk8 battery to the one with issue and it’s still happens so probably not the battery.
Got home and the vesc terminal threw a lot of abs_over_current errors becuse it exceeded 130A.


My gear:
TB vesc, BLDC mode
Tacon 160 245kv
10s6p 26f 18650 lion pack
16/36 pulleys
97mm wheels.

The Faults i'm getting:
<img src="/uploads/db1493/original/3X/5/7/57aaae64deda551cc2d441129fa0a0c9cc8b8d03.JPG" width="480" height="500"><img src="/uploads/db1493/original/3X/7/c/7c11a797532ee160042f21c1485903deefebcccf.JPG" width="480" height="500">



Thanks
Ishay
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-10-05T18:52:22.189Z Reads: 81

```
Why are you using 245kv with 10s?
```

---
## \#3 Posted by: Ishayc Posted at: 2017-10-05T19:02:02.771Z Reads: 74

```
It was intended to a 6s build but got a good price on a battery..
I tried it with a 6s and it has the same issue
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-10-05T19:03:06.684Z Reads: 71

```
Not sure why, but I have the feeling that @Jinra can help...

Check if any connections are loose and check for bad solder joints
```

---
## \#5 Posted by: Jinra Posted at: 2017-10-05T19:04:06.239Z Reads: 72

```
Post faults, VESC settings, and the f/w version you're using.
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-10-05T19:09:31.959Z Reads: 71

```
+1 to that
```

---
## \#7 Posted by: darkkevind Posted at: 2017-10-05T19:13:59.570Z Reads: 68

```
I bet your motor min is too high for your motor's max current rating....?
```

---
## \#8 Posted by: Ishayc Posted at: 2017-10-05T19:26:53.528Z Reads: 73

```
@darkkevind Motor's max current rating is 75A so I'm good there.
@Jinra i need to recreate the fault, will do once i'll be home in the meanwhile here are the vesc's settings - 
<img src="/uploads/db1493/original/3X/4/7/4796dfe72b3898454f620cca5fb2a419175dcacb.JPG" width="690" height="70"><img src="/uploads/db1493/original/3X/f/4/f40c7c1714644d012ff55b59a2f7b584532f5d80.JPG" width="690" height="207"><img src="/uploads/db1493/original/3X/1/c/1c45dd555d77b975cd9f31fe008b65f4bee3294e.JPG" width="690" height="277"><img src="/uploads/db1493/original/3X/6/6/66669960a5c6c3b1b8dfd352b2419ea825fcd04b.JPG" width="690" height="159"><img src="/uploads/db1493/original/3X/d/2/d23b56439535336f68fc88d3d050aab78fd25853.JPG" width="690" height="292"><img src="/uploads/db1493/original/3X/a/7/a7147d2a692039c64cf1b1e3fa6ea53089560b9e.JPG" width="690" height="176">
```

---
## \#9 Posted by: Jinra Posted at: 2017-10-05T19:30:52.321Z Reads: 62

```
what about f/w version?
```

---
## \#10 Posted by: Ishayc Posted at: 2017-10-05T19:32:50.680Z Reads: 62

```
@Jinra forgot to mention. It's 3.28
```

---
## \#11 Posted by: Ishayc Posted at: 2017-10-07T08:11:52.364Z Reads: 56

```
Uploaded the faults.
can someone help?
thanks
```

---
## \#12 Posted by: scepterr Posted at: 2017-10-07T08:19:13.028Z Reads: 55

```
This isn't from breaking on full battery(if there's a bms)? 
Breaking @ 41.46v and 41.65v could easily spike over 42v and trigger BMS overvoltage cut
```

---
## \#13 Posted by: Ishayc Posted at: 2017-10-07T08:50:01.700Z Reads: 51

```
Hmm, I thought of that after it happened so I skipped the bms for discharge and it didn’t help. Maybe the battery has an internal cutoff feature if overcharged? 🤔
```

---
## \#14 Posted by: scepterr Posted at: 2017-10-07T08:51:16.717Z Reads: 53

```
No the battery itself doesn't have any protection
```

---
## \#15 Posted by: Ishayc Posted at: 2017-10-07T09:14:52.987Z Reads: 51

```
Then I’m clueless. 
Any other suggestions/ideas?
```

---
## \#16 Posted by: Ishayc Posted at: 2017-10-07T16:11:21.423Z Reads: 49

```
New revelations- after I switched to Ackmaniac’s fw and turned off Soft slow max the issue with the braking is gone, however I still loose power on stiff hills due to heat which means it goes above 80 degrees celcius.
My question now - is it normal? 
I’m not having this issue on my first build which has a 6s Lipo battery with the same exact motor and gear.
```

---
## \#17 Posted by: Jinra Posted at: 2017-10-07T16:13:41.846Z Reads: 47

```
how do you know it's thermal shutoff, did you get a fault for that?
```

---
## \#18 Posted by: Ishayc Posted at: 2017-10-07T16:20:27.231Z Reads: 46

```
No faults at all..
```

---
## \#19 Posted by: Jinra Posted at: 2017-10-07T16:22:38.764Z Reads: 44

```
so 80 degrees is when it starts throttling current and you'll feel it becoming weaker. 100c is when it shuts off. If it shuts off without becoming weaker sounds like something else is wrong.
```

---
## \#20 Posted by: Ishayc Posted at: 2017-10-07T16:36:41.240Z Reads: 42

```
After I switched fw it just gets weaker and does not shuts off at all.. is it normal for a vesc to go that high?
```

---
## \#21 Posted by: Ishayc Posted at: 2017-10-08T18:00:44.951Z Reads: 40

```
So i've added a heat sink to 3/6 MOSFETs, turned off Slow absolute max and installed @Ackmaniac's fw and the ride was a bit better, though im still getting the ABS_OVER_CURRENT error and the heat sink and the motor are painfully to touch hot.
The errors i'm getting now are the same besides the current is too high on the Current line and not on the Current filtered:
<img src="/uploads/db1493/original/3X/6/1/61d8e8229c337040b907c977da2bc66427de4e3d.JPG" width="690" height="425">
```

---
## \#22 Posted by: Ishayc Posted at: 2017-10-09T12:24:01.416Z Reads: 37

```
It seems like some of the spikes I’m having are between 130 and 140.
Can I raise the absolute max to 140A?
```

---
## \#23 Posted by: Ishayc Posted at: 2017-10-10T19:40:29.491Z Reads: 32

```
Ok, issue fixed after I changed the wheel pulley to 44t instead of the 36t I had. 
Probably a 245kv motor, 10s battery and 1:3 gear ratio is not a good combination.
```

---
