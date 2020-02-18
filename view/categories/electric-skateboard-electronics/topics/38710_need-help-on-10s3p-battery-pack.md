# Need help on 10s3p battery pack

### Replies: 4 Views: 371

## \#1 Posted by: mnelson3690 Posted at: 2017-11-18T21:53:48.437Z Reads: 83

```
My battery pack will only charge up to 80% and then the charger begins to pulse and won’t charge anymore. Can anybody help me out? I’m not sure what is going on
```

---
## \#2 Posted by: surprisebirthday Posted at: 2017-11-18T22:08:47.431Z Reads: 77

```
I have this problem with my own 10s3p.  My problem seems to be caused by a pack that has a lower voltage than the others, about 0.7 volts lower.  The BMS stops charging when the other cells hit 4.2.  My pack dies early when the gimpy cell hits my cutoff at 3.2 volts.  

I'm in the process of trying to rebalance my cells using just the BMS, but I'm not having much luck.

Try using a mutlimeter to check the voltages of the cells.
```

---
## \#3 Posted by: Battosaii Posted at: 2017-11-18T22:19:55.585Z Reads: 68

```
this happened to my space cell i took it apart and found 4 cells that the spot weld had failed and come off so i soldered the nickel strip back in place since i dont have a spot welder and its been fine ever since.
```

---
## \#4 Posted by: treenutter Posted at: 2017-11-18T23:39:20.768Z Reads: 51

```
@mnelson3690 post some pics of your pack and tell us which BMS you're using. @surprisebirthday is right, and the alternative is that some BMSs will stop charging as soon as any single pack reaches 4.2V. So, if any of them have drifted you'll need to charge them up individually to get all packs at the same level. AND: the battery indicators we use don't always show a useful number. i.e. 80% doesn't necessarily mean you're getting only 80% of your ride time, it means that the V is at 80% of the max; but since the discharge curve at the top of the charge is very steep, you might not get a lot of usable discharge in that top 10-15%.
```

---
