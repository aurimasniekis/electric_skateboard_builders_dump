# Battery Not Charging Full

### Replies: 7 Views: 507

## \#1 Posted by: jimbosays Posted at: 2017-05-24T17:16:23.857Z Reads: 85

```
I have a 12S3P pack of LG HG2's with a battery supports BMS. Normally it charges to 50.4V full, but recently it's been charging to ~49.6V before spiking to 50.4V and the charger thinks it is done. But when I unplug it, it goes back to 49.6V. That was last week and I've been able to actually get it to charge to 50.4V without dropping. However, today, it charges to 48.6V before spiking to 50.4V and cutting the charger off. I can't seem to get it back up to 50.4V normally. 

I saw a similar post for an 8S6P battery, but my situation is slightly different as sometimes it returns to charging to 50.4V. Anyone know what might be going on? Is it the BMS or a faulty charger?
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-05-24T17:32:09.115Z Reads: 83

```
check your welds. then check your balance leads for broken solder joints that might be intermittently connecting and disconnecting.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-05-24T18:39:43.701Z Reads: 70

```
And while your checking weld and solder joints, might as well check individual cells voltages.
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-05-24T19:09:40.255Z Reads: 70

```
The potential for a dead P group is also pretty good here.
```

---
## \#5 Posted by: JohnA Posted at: 2017-05-24T22:58:04.670Z Reads: 57

```
This happens on my 10s 5p battery with battery supports BMS. From what I've read it seems normal with these BMS's with their low balancing current. It is cutting out so it can do a balance cycle because one or more parallel groups at at 4.2v. Mine charges to 41.2v and then jumps to 42.5v (my chargers voltage), But If I leave it over night and plug it back in it charges up a little more (4.16v). When I checked my parallel groups there is one that is 4.2v while the others are 4.12-4.14. if you manually discharge or charged the outlier value it should charge up to the full 50.4v.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-24T23:23:57.258Z Reads: 54

```
I experienced the same situation with my Bestech bms using a brick charger. My 10s pack would charge to 41.9 and then the charger would shut off.
Now I use a CC/CV Lab power supply and it  doesn't shut off but keeps sending a low current charge to fill the low cells while the bms trims down the high cells.
The balance current of the Bestech is 126ma so when the power supply in CV mode drops to below 126ma it works like a hobby balance charger.
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-24T23:38:00.328Z Reads: 51

```
Oh man this is my exact issue. I thought it was a faulty BMS. What's the best way to discharge the outlier group?
```

---
