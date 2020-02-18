# Dual Vesc y-cable configuration?

### Replies: 11 Views: 1225

## \#1 Posted by: marcmt88 Posted at: 2017-10-01T15:43:57.099Z Reads: 138

```
Hi,
Need your advise on how to configure dual vesc using y-cable.  Do I configure each vesc individually then connect the 2 vesc's together with the y-cable?  Trying to look for a similar thread regarding this but to no avail.  
Thanks for your help.
```

---
## \#2 Posted by: bigben Posted at: 2017-10-01T15:46:02.836Z Reads: 137

```
http://www.electric-skateboard.builders/t/y-piece-or-canbus/26461
```

---
## \#3 Posted by: PartyPoison Posted at: 2017-10-01T15:46:12.772Z Reads: 135

```
Yup, you will configure it individually
```

---
## \#4 Posted by: Namasaki Posted at: 2017-10-01T18:15:01.646Z Reads: 125

```
Configure each vesc as a master.
Be sure to clip the 5v wire from one of the vesc
If you try to supply 5v from both vescs, you will damage them

<img src="/uploads/db1493/original/3X/4/9/49e97d871a6c8eaae5e00cd59cd5320d7774ab0c.jpeg" width="375" height="500">
```

---
## \#5 Posted by: marcmt88 Posted at: 2017-10-01T20:01:29.815Z Reads: 113

```
Greatly appreciated everybody.  What I gathered from all those great contributors/discussion to this forum, here is my schema to my first built.  Did I miss anything?  Is it necessary to up 12 AWG (battery/BMS) to 10 AWG ? 

<img src="/uploads/db1493/original/3X/6/3/63476facd35ae696698c00e8372c961ec4832702.gif" width="690" height="388">
```

---
## \#6 Posted by: karma Posted at: 2017-10-01T20:28:26.238Z Reads: 103

```
Denepds on how many amps you will draw, you can check the cable needed here. https://www.powerstream.com/Wire_Size.htm
```

---
## \#7 Posted by: Namasaki Posted at: 2017-10-01T20:52:09.949Z Reads: 97

```
Current ratings for silicone wire.
Always use silicone wire because it has higher current rating and it's insulation can withstand higher temps.
12 awg is enough for most street boards. If your building an electric mountain board or similar then you might want to go 10awg for extra safety. 

<img src="/uploads/db1493/original/3X/1/3/1391f424e39f07fe8ef8ff5854b7d7f4f3fcefd6.png" width="295" height="223">
```

---
## \#8 Posted by: Tampaesk8er Posted at: 2018-10-06T10:52:09.069Z Reads: 37

```
What is a good motor setting for each motor dual (6374) sk3 149kv 10s setup in vesc tool, amps to motor, breaking, ect.?
```

---
## \#9 Posted by: Namasaki Posted at: 2018-10-06T12:29:28.839Z Reads: 36

```
What type of battery/bms are you using?
```

---
## \#10 Posted by: Tampaesk8er Posted at: 2018-10-06T14:19:14.491Z Reads: 33

```
Samsung 10s2p 36v with a standard 45a bms, 4.4ah.
```

---
## \#11 Posted by: Namasaki Posted at: 2018-10-06T17:02:22.872Z Reads: 28

```
You need to.get the cell specs to determine max output current and charge current for the Vesc settings. 

I think a 10s2p is going to be a bit overwhelmed. 
You really need more battery. At least a 10s4p
Or Lipos with a C rating of 60 or more.
```

---
