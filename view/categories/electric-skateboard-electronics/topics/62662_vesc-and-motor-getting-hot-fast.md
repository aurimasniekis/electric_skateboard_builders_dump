# Vesc and motor getting hot&hellip;fast

### Replies: 10 Views: 479

## \#1 Posted by: Andy87 Posted at: 2018-07-23T19:19:18.266Z Reads: 164

```
after one of my vescs give up to work i now run only single drive.
i just made a 30min test ride incl. recording.
my vesc run once into temp restriction and lowered the output.
max temp. was about 87 degrees.
when i came home the motor was also around 70 degrees.
what can cause such a fast rising of temp.?

my vesc has a heatsink but is mounted under the deck in the battery tray (trampa tray).
I looked through the log files and the average motor current was about 14A.
for me everything looks a bit strange.
can't explain myself how such a current can produce such a temperature.
```

---
## \#2 Posted by: AutoItKing Posted at: 2018-07-23T20:27:51.805Z Reads: 154

```
Did you do any reprogramming when you went to single drive? BLDC or FOC? What are your current/voltage settings?
You were splitting the load before, now the whole load is on one motor/VESC. It does seem a bit odd though.
Post your settings and if possible your log.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-07-23T20:55:21.435Z Reads: 139

```
my vescs already became hot in time i was driving dual.
not so fast as it was split to two vescs and motors but with about 65degrees after normal driving
with two vesc it shouldn't be so much. as minimum i thought so.
run bldc on ackmanick 3.102.
motor max 60a
motor min -60a
battery max 60a
battery min -30a
battery max is a bit high...that's a mistake, should change to 40a...
during my ride i never came over 44A battery
here a picture of the ride
![IMG_5081|636x500](upload://gRnszzE0tJVrY4yPl0BJbFIPnJw.jpg)
```

---
## \#4 Posted by: AutoItKing Posted at: 2018-07-23T21:33:32.944Z Reads: 123

```
Can you show temp on the same plot? I'd expect it to spike at or slightly after high current.
Are you sure your heat sink is actually heat sinking and not insulating?
```

---
## \#5 Posted by: Andy87 Posted at: 2018-07-24T05:01:19.762Z Reads: 101

```
There is no temp log over time, or as min I didn’t found yet.
I can only say max and min values.
The down site of my enclosure becomes warm and the temp. is falling down relatively fast if I just stop.
I made some tests while driving yesterday. 
5min constant driving than stop and check temp, again 5min driving and than check temp...
For sure the temp rise up in time of driving.
If I drive in short streets where I need to stop and accelerate ever 100m the temp is up to 65 degrees after 2min.
The vesc temp I could somehow maybe understand, but is it normal that the motor heat up to 70degree after 30min ride?
```

---
## \#6 Posted by: AutoItKing Posted at: 2018-07-24T05:12:02.028Z Reads: 93

```
If the motor is small it could explain the heat. My 6355 is usually just warm to the touch after a long-ish ride.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-07-24T05:27:40.969Z Reads: 90

```
it´s a 6374 190kV
```

---
## \#8 Posted by: ctincristy Posted at: 2018-09-10T05:05:04.780Z Reads: 46

```
Have you solved this temperature issue? Seems strange (I dug a bit in your past after reading the 6374 comment on my topic lmao) My guess is bad BMS/vesc connection?
```

---
## \#9 Posted by: Andy87 Posted at: 2018-09-10T05:08:54.712Z Reads: 43

```
No not yet...my board started to flame up...
Just get my things together, rebuilt the motors and hope next week I can finally get them to go again.
The problem with the heating up vesc I guess I found. Why the motor in single heated up to I still can’t explain. Maybe it was too much breaking and accelerating on only one motor which also was sealed...we will see soon I hope
```

---
## \#10 Posted by: Andy87 Posted at: 2018-09-10T05:10:55.009Z Reads: 44

```
Ah and I added a bit more to your discussion.
If you just look on the wattage I guess a single 6384 would be the best choice as it fit perfectly the 4K watt.
```

---
