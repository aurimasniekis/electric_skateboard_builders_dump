# Board not responding (Over Voltage)

### Replies: 16 Views: 1064

## \#1 Posted by: rasmukri Posted at: 2017-01-14T14:35:50.167Z Reads: 77

```
I was out riding last night and was cruizing along at like 15mph and the brakes were non responsive so i bailed onto a lawn and ran it off.
I have encountered this same problem several times since but only while riding. I cant get it to do anything while on the bench.
When i do active sampling no faults present themselves.
in terminal i type faults and get the following:
The following faults were registered since start:

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -4.5
Current filtered : -6.2
Voltage          : 57.38
Duty             : 0.47
RPM              : 38324.7
Tacho            : 446045
Cycles running   : 5593
TIM duty         : 3871
TIM val samp     : 1934
TIM current samp : 6059
TIM top          : 8250
Comm step        : 4
Temperature      : 45.40

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -7.4
Current filtered : -6.2
Voltage          : 57.38
Duty             : 0.35
RPM              : 29668.7
Tacho            : 456350
Cycles running   : 318
TIM duty         : 3687
TIM val samp     : 1837
TIM current samp : 7095
TIM top          : 10515
Comm step        : 1
Temperature      : 44.51

Fault            : FAULT_CODE_OVER_VOLTAGE
Current          : -24.7
Current filtered : -21.9
Voltage          : 58.48
Duty             : 0.21
RPM              : 22319.5
Tacho            : 464672
Cycles running   : 814
TIM duty         : 3270
TIM val samp     : 1630
TIM current samp : 9462
TIM top          : 15664
Comm step        : 1
Temperature      : 43.55

So over voltage cool, easy enough, but i still dont know how to fix this. my settings for both vesc are set at 57v max, I am running a 12s4p battery from brand new samsung 18650. 2x VESC and 2x enertion 190KV motors also i am getting this when i do the detect parameters:
Detection results:
Integrator limit: 104.95
BEMF Coupling: 728.46
Hall sensor detection failed:
-1, -1, -1, -1, -1, -1, -1, 5

<img src="/uploads/db1493/original/3X/4/a/4aca80c7a90c1ab9085cb7fb241eabab9455e5c2.jpg" width="690" height="404"><img src="/uploads/db1493/original/3X/3/0/300cf9fc4efcd4e68d19cfcad2c0f8a5659d6c3b.jpg" width="690" height="179">
```

---
## \#2 Posted by: Mrmoonlight Posted at: 2017-01-14T15:13:32.436Z Reads: 61

```
Was your battery full? I had a similar issue a while back.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2017-01-14T15:16:04.101Z Reads: 62

```
Are you using a BMS ?
```

---
## \#4 Posted by: rasmukri Posted at: 2017-01-14T15:25:28.310Z Reads: 61

```
No BMS, and the battery was full once and about 2/3 full another time.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-01-14T15:37:15.502Z Reads: 62

```
can you check the voltage show in the tabs realtime, don't forget to clicl on activate sampling ?
```

---
## \#6 Posted by: rasmukri Posted at: 2017-01-14T15:59:01.809Z Reads: 60

```
first one is full throttle
second one is about half

<img src="/uploads/db1493/original/3X/0/0/0043550d9023504c66ae36a6dafd1bfb13a193ee.jpg" width="690" height="406"><img src="/uploads/db1493/original/3X/5/f/5f643b6bd69b88ceeaa32f30599ac88edb1063d0.jpg" width="690" height="407">
```

---
## \#7 Posted by: rasmukri Posted at: 2017-01-14T16:03:35.419Z Reads: 55

```
Also all the info is being pulled off the Master VESC.
When i look at the slave it has no errors, but i was briefly able to get it to only spin one motor and the one that was not spinning was the salve VESC. When the slave was not spinning the master seemed to try and slow from traction control it went to like half power, until the other one came back online.
also ALL the settings are identical for both VESC with the exception of the master is #1 and the slave is #2 also send status over CAN is only selected on the slave with the rate set at 500
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-01-14T16:04:53.896Z Reads: 53

```
and without any throttle ? :wink:

also if you can post sone picture of your vesc, and they are from witch  vendor
```

---
## \#9 Posted by: Keenan Posted at: 2017-01-14T16:06:50.732Z Reads: 55

```
Bailed into a lawn?!?! It boggles my mind how you'd guys can do so much research into the technical side of things while apparently totally ignoring basic safety maxims widey accepted in longboarding. 

Learn how to footbrake, for chrissake!
```

---
## \#10 Posted by: rasmukri Posted at: 2017-01-14T16:14:37.706Z Reads: 53

```
While yes jumping and running in the air till i was running on the ground is not considered the best idea.
I have foot braked before when i had a belt snap so i was without brakes, and it didn't end well. I applied a bit too much downward force twisted my toe inward and tripped ran over my foot and ate shit. So I decided to say fuck it and just jumped off.
```

---
## \#11 Posted by: chaka Posted at: 2017-01-14T16:23:47.240Z Reads: 49

```
What type of samsung cells are you using? You may need to adjust your regen values or add more cells in parralel if they are not designed high charge rates.
```

---
## \#12 Posted by: rasmukri Posted at: 2017-01-14T16:27:07.284Z Reads: 51

```
[quote="JohnnyMeduse, post:8, topic:16088, full:true"]
and without any throttle ? :wink:

also if you can post sone picture of your vesc, and they are from witch  vendor
[/quote]

Both of the VESC are from enertion
here is the no throttle pic.
[quote="chaka, post:11, topic:16088, full:true"]
What type of samsung cells are you using? You may need to adjust your regen values or add more cells in parralel if they are not designed high charge rates.
[/quote]

the batteries are Samsung 25R not sure on the charge rates for these. but if so what should i change and by how much?


<img src="/uploads/db1493/original/3X/7/5/75065afd4d9f14039fa7c0bd7d3927cee538ef8a.jpg" width="690" height="404">

master VESC
<img src="/uploads/db1493/original/3X/4/b/4b2796919b14ffd7b681acfabe8bccba1d3dbcdd.jpg" width="445" height="500">

slave VESC
<img src="/uploads/db1493/original/3X/d/b/db2a6e5e139d81de688e195ed8dc290224a0a931.jpg" width="491" height="500">
```

---
## \#13 Posted by: Blasto Posted at: 2017-01-14T17:25:57.186Z Reads: 42

```
Little perplexed on whats going on here... could try to swap your master to become the slave and your slave to become your master... 

not entirely sure what would that achieve but it's a harmless action to take meanwhile thinking of whats going on here

The other thing i can think of is one of your 2 vesc has a bad batt max setting and so one of them would throw a fault and that the traction control would stop your board all together

So double check your batt max setting on both vesc's first
```

---
## \#14 Posted by: rasmukri Posted at: 2017-01-14T19:07:45.421Z Reads: 37

```
[quote="Blasto, post:13, topic:16088, full:true"]
Little perplexed on whats going on here... could try to swap your master to become the slave and your slave to become your master... 

not entirely sure what would that achieve but it's a harmless action to take meanwhile thinking of whats going on here

The other thing i can think of is one of your 2 vesc has a bad batt max setting and so one of them would throw a fault and that the traction control would stop your board all together

So double check your batt max setting on both vesc's first
[/quote]

I tried switching the master and slave just for sheer why the hell not. no change to my problem.

both of the VESC have the same settings for batteries 100% identical on that page of BLDC tool

I have contacted enertion support about this issue and am waiting for them to get back with me as far as what to do.
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2017-01-14T19:17:54.302Z Reads: 35

```
Are you using some kind of switch
```

---
## \#16 Posted by: rasmukri Posted at: 2017-01-14T19:29:58.163Z Reads: 35

```
[quote="JohnnyMeduse, post:15, topic:16088, full:true"]
Are you using some kind of switch
[/quote]

I made a loop key out of a XT90s
 and i have an inline fuse 50A solid connections and all before the wires split to go to the 2x VESC
```

---
