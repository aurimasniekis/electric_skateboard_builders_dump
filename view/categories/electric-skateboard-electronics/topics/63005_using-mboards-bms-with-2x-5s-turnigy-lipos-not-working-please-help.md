# Using Mboards bms with 2x 5s turnigy lipos, not working please help

### Replies: 17 Views: 375

## \#1 Posted by: Jake2k17 Posted at: 2018-07-27T01:16:18.432Z Reads: 87

```
I was using the IMAX b6 charger but they was really inconvenient so I used the bms from Mboards site and it doesn’t seem to be charging. The green light on the charger is on, which either means charge full or disconnect, but the batteries are each at 18.8 volts. Everything seems to wired right from the different tutorials I have seen and there are no burn marks on the bms at all. If anybody could give me some insight on this that would be really helpful. Thanks.
```

---
## \#2 Posted by: nuttyjeff Posted at: 2018-07-27T02:09:35.753Z Reads: 75

```
Pictures of your connections would help,
```

---
## \#3 Posted by: Jake2k17 Posted at: 2018-07-27T02:52:43.094Z Reads: 72

```
U![image|375x500](upload://pE17tBPfFx5zCDIAXzcD61FL1yU.jpeg)![image|375x500](upload://wrZ9fZUH2GftblP6m66VG6vZg87.jpeg) 

The main video that i used for the wiring was from kvboards and he said that I could connect the balance wires from the bms to the lipos using hot glue so that’s what I did. Will that work or should I solder the wires?
```

---
## \#4 Posted by: nuttyjeff Posted at: 2018-07-27T03:35:21.352Z Reads: 62

```
I’m going to assume you wired the balance leads right, probably need more pictures to determine that.

What are the 2 cables entering your bms’s C- and B - ports?
```

---
## \#5 Posted by: Jake2k17 Posted at: 2018-07-27T04:05:50.381Z Reads: 58

```
There is only one in the c- port and that is the negative charge port wire. For the b- there is a wire connected to the negative lead and then the negative balance wire from one of my lipos
```

---
## \#6 Posted by: DeathByBacon Posted at: 2018-07-27T04:20:11.744Z Reads: 58

```
Your balance leads, I assume, are wired correctly since it's not on fire.

I have the exact same BMS and I wired it as you did except for B-. I only connected the main negative but not the balance wire negative. It's been working so far. 

By the way, what charger are you using?
```

---
## \#7 Posted by: nuttyjeff Posted at: 2018-07-27T04:37:12.726Z Reads: 54

```
Can you check if you reversed the polarity of your charging connector?
```

---
## \#8 Posted by: Jake2k17 Posted at: 2018-07-27T04:42:52.878Z Reads: 49

```
Not sure what the polarity is but I’m using a 42v laptop brick from mboards
```

---
## \#9 Posted by: Jake2k17 Posted at: 2018-07-27T04:47:00.947Z Reads: 52

```
Also what do you do with the negative balance cable? I have all 6 balance cables on the first battery wired in as 10-5 on the bms, and then the first balance on the second battery is not connected to anything, while the next four are wired in as 4-1. The last negative cable is connected to the b-
```

---
## \#10 Posted by: nuttyjeff Posted at: 2018-07-27T04:47:37.442Z Reads: 50

```
![image|666x500](upload://thEIAZraBYOV5lYPvfCMO5bN4zO.png)
```

---
## \#11 Posted by: Jake2k17 Posted at: 2018-07-27T05:03:01.439Z Reads: 44

```
thank you so much bro you saved me.
```

---
## \#12 Posted by: nuttyjeff Posted at: 2018-07-27T05:08:17.583Z Reads: 43

```
Did you manage to fix it?
```

---
## \#13 Posted by: Jake2k17 Posted at: 2018-07-27T05:29:46.172Z Reads: 43

```
Not yet I will in the morning (US) and tomorrow my battery meter will be arriving. Will post pictures when done.
```

---
## \#14 Posted by: Jake2k17 Posted at: 2018-07-27T17:41:16.303Z Reads: 34

```
I did what you said, but it still doesn’t seem to be working, I guess it’s not solved lol. The battery meter still hasnt come, but there is green light on the charge brick, and green either means charge full or disconnect, but i know that it isn’t close to charge full yet. Any thoughts on this?
@nuttyjeff
```

---
## \#15 Posted by: nuttyjeff Posted at: 2018-07-28T04:35:27.900Z Reads: 27

```
Can you check to see what charger you have. If youre plugging an 8S charger to a 10S BMS its alwayw going to read that it's full.
```

---
## \#16 Posted by: Jake2k17 Posted at: 2018-07-28T05:51:09.013Z Reads: 24

```
No I’m using the 42 volt charger from Mboards
```

---
## \#17 Posted by: Jake2k17 Posted at: 2018-07-28T05:54:03.211Z Reads: 26

```
My only thoughts are that
1) the cells are in the wrong order and the bms recognizes and won’t charge? 

2) there are 3 pins on the charger, positive, negative, and a bottom pin which tells the board not to ride away while charging. If the bottom pin is not connected maybe it isn’t charting?Or at least that’s what I understand. This is a little bit far fetched but maybe?
```

---
