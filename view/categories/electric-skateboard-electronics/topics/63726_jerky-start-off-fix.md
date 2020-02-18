# Jerky start off fix?

### Replies: 14 Views: 686

## \#1 Posted by: Danny414 Posted at: 2018-08-03T16:21:17.523Z Reads: 161

```
Any one know what I have to tweet in BLDC to get the take off to be smooth and not jerky from a stand still

https://streamable.com/sc0bl

Thanks!
```

---
## \#2 Posted by: Static Posted at: 2018-08-03T16:55:27.630Z Reads: 150

```
Are those sensored motors? If you don't have a vesc that can safely run FOC give sensored BLDC a try and will remove the start up jerk. The VESC motor wizard makes this easy to setup. Otherwise just give a single push before you apply throttle in BLDC mode.
```

---
## \#3 Posted by: Acido Posted at: 2018-08-03T17:03:47.980Z Reads: 140

```
Push lightly before presding throttle / get sensored motors / buy a sensor kit
```

---
## \#4 Posted by: Danny414 Posted at: 2018-08-03T17:13:29.108Z Reads: 137

```
Yeah I have sensored motors and using focbox mode.. I do give a push off currently but id like to be able to have a smooth take off from stand still if possible
```

---
## \#5 Posted by: Danny414 Posted at: 2018-08-03T17:13:59.636Z Reads: 130

```
Thanks! they are sensored and am using focbox mode
```

---
## \#6 Posted by: accrobrandon Posted at: 2018-08-03T17:16:32.762Z Reads: 126

```
Did u run hall sensor detection during set up? Could be real jerky like that cuz the vesc doesnt actually know which hall sensor is where... Once u push it understands but a stand still it doesnt. After sensor detection it should be smooth.
```

---
## \#7 Posted by: Danny414 Posted at: 2018-08-03T17:25:59.878Z Reads: 113

```
Yup ran all that stuff.. it’s fine after I give it a kick push.. was just hoping to be able to take off from stand still smooth too
```

---
## \#8 Posted by: accrobrandon Posted at: 2018-08-03T17:36:28.014Z Reads: 114

```
Weird then... I have the same sealed 6355s from maytech and I get a smooth start fpr a stop ... although I rarely ever start standing at a stop after accidentally busting my ass... Maybe theres something off in ppm settings

.... Or maybe double check the halls sensors values got written to the vesc just in case...
```

---
## \#9 Posted by: Fiori Posted at: 2018-08-03T17:56:13.220Z Reads: 107

```
Your sensors are not configured right. Either detection failed or they are disabled. I run sensor less and that's exactly what it looks like.
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-08-03T18:43:31.816Z Reads: 101

```
first, it's not focbox mode, it's just FOC mode

anyway

1. in foc tab, make sure it's in hall mode, and go ahead do motor detect and calculate, etc
2. do hall sensor detection
3. apply
4. write back to esc

![image|690x371](upload://dWmSk0XJVIjz1Fmwy1bzndOKj6c.png)

if that doesn't work your motor sensors may be shot
```

---
## \#11 Posted by: dareno Posted at: 2018-08-04T01:35:48.425Z Reads: 79

```
I know its simple but did you write config/apply settings after the motor detection? If you have a sensor down it will tell you.
```

---
## \#12 Posted by: Danny414 Posted at: 2018-08-04T04:01:43.491Z Reads: 69

```
Oh I did the calibration before but I had sensorless ticked I THINK
```

---
## \#13 Posted by: GenghisConman Posted at: 2019-08-28T16:19:14.487Z Reads: 30

```
Having the same problem with my unity. Solution?
```

---
## \#14 Posted by: Ixf Posted at: 2019-08-28T17:45:01.395Z Reads: 22

```
Make sure its in FOC mode.
Make sure you have it in sensored mode
Make sure the sensor detection actually worked
Make sure you saved your setting
```

---
