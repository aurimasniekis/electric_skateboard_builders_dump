# 6s battery charging cell voltage fluctuation

### Replies: 7 Views: 438

## \#1 Posted by: linkedtim Posted at: 2018-02-24T16:28:50.365Z Reads: 40

```
Hi,
Newb here, please excuse some ignorance...
Two-3s batteries in series that I'm charging; all cells show on the imax B6 charger, cell 3 and 4 are fluctuating as its charging and I'm not sure why? There doesn’t appear to be any consistency; one second all the cells will show similar voltage, the next cell 3 will show zero and cell 4 maxes out. It'll show this real quick and then jump back to all 6 showing similar voltage. In regular charge mode the charger usually stops after a few seconds and I assume its because cell 4 hits ~5v(as in the picture) and the summation of all the cells reaches the cutoff V ceiling. In balance mode it usually makes it a little farther along the charge process, though as in the picture, cell 3 is lagging a bit. Has anyone seen this or anything I can do to try and resolve or are these cells cooked somehow? I typically only charge in 'Balance mode' thinking that's the safer approach given the inconsistency.

Batteries = Zippy Capacity: 5000mAh, Voltage: 3S1P / 3 Cell / 11.1v, Discharge: 20C Constant / 30C Burst

![IMG_4684|666x500](upload://t9lzAmCdRbTHOzggxxYoUmOOp9X.JPG)
![IMG_4683|666x500](upload://rpIr3NJO0PlymHUGp6Q3NnWYfgu.JPG)
```

---
## \#2 Posted by: krloz Posted at: 2018-02-24T16:55:51.172Z Reads: 35

```
It looks more like a charger issue than Battery issue.  I don't care how old or dead a battery is I don't think it could ever go 3.7v to 0v in a split second unless you dropped it in salty water. Is than Ann original imax or a clone?  Do you have any other means of charging too check on the battery
```

---
## \#3 Posted by: Ishayc Posted at: 2018-02-24T17:08:45.503Z Reads: 29

```
I’ve seen it once but it happened immediately after the balance connector was plugged in.
The problem was a bad wiring.
It might be a different issue since it looked ok before you charged it.
```

---
## \#4 Posted by: E1Allen Posted at: 2018-02-24T17:34:27.068Z Reads: 27

```
Do you have a voltmeter so you can check the individual cell voltage from the balance lead.  Can you charge each 3s separate?  Also it is possible you have one bad cell. However the 0 and 5v readings aren't correct either.  I'd check each cell prior to charging then charge each separate.  Then see what happens
```

---
## \#5 Posted by: linkedtim Posted at: 2018-02-24T18:05:00.561Z Reads: 20

```
Little embarrassed but yeah, seemed to be the wiring. I soldered together my balance lead's JST connectors so I could charge the two 3s batteries simultaneously, seems my middle balance lead cable (4th) wasn't a strong connection at all (I gave them all a little tug and that one easily separated.) That would account for the wonkiness on the 3rd and 4th cell I think.
![IMG_4686|666x500](upload://e0UbsDRjZEMrbgESMdKigNB9bt6.JPG)

Seems to be charging correctly now. Thanks so much.

To anyone else that reads these post, might be worth buying a 2x-3s to 6s adapter instead of trying to solder everything yourself.
```

---
## \#6 Posted by: Ishayc Posted at: 2018-02-24T18:50:36.063Z Reads: 15

```
Nothing to be embarrassed about.
Enjoy the ride.
```

---
## \#7 Posted by: Pennguy Posted at: 2019-01-23T22:58:20.425Z Reads: 8

```
Hi, I have a 12s setup with bms and a common scooter 3 prong charging port hooked up to it I am not sure what’s the issue but when I power up the esc it works great but it discharges quick in my opinion then I hook the charger to it and it charges the battery to quickly also. Not sure if only 1 of the 6s battery is working but I don’t know why this is happening. Could it be that I have a defective battery?
```

---
