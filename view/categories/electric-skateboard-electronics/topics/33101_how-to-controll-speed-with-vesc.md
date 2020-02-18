# How to controll speed with vesc?

### Replies: 9 Views: 1547

## \#1 Posted by: Dariks Posted at: 2017-09-14T01:00:17.169Z Reads: 162

```
Hi so I'm wondering how I can control the speed i go at with the vesc can you guys post pictures of vesc settings on bldc tool like which ones limit speed?
```

---
## \#2 Posted by: Clonkex Posted at: 2017-09-14T01:01:27.938Z Reads: 162

```
Why not just use less throttle?
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-09-14T01:02:24.344Z Reads: 163

```
Current control controls power, not speed.  Duty Cycle will control speed, it’s what Boosted Boards uses
```

---
## \#4 Posted by: Dariks Posted at: 2017-09-14T01:02:57.224Z Reads: 164

```
Oh that kinda works but it really limits the throw of the actually throttle making it jumpy.
```

---
## \#5 Posted by: Dariks Posted at: 2017-09-14T01:03:38.169Z Reads: 159

```
how do i use the duty cycle?
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-09-14T01:03:47.429Z Reads: 156

```
Adjust throttle trim on remote and redo PPM calibration in BLDC Tool
```

---
## \#7 Posted by: Namasaki Posted at: 2017-09-14T04:53:36.220Z Reads: 139

```
I would not recommend switching to duty cycle. One of the main reasons that vesc is better than esc's is current control mode.
Can you post more info about your build and post bldc settings so we can know better how to advise you?
```

---
## \#8 Posted by: racidon Posted at: 2017-09-14T05:54:32.295Z Reads: 132

```
I've not looked at all the settings in VESC6 but I know there's a throttle curve that can be adjusted. If you adjust this and set the ERPM limit you could theoretically set your speed limit that way?
```

---
## \#9 Posted by: ninja Posted at: 2017-09-14T08:49:05.686Z Reads: 111

```
Just use @Ackmaniac bldc tool and firmware+ app with bluetooth module. So in bldc is throttle curve for nice throttle feel. In the app you can make different modes- like for an example: easy, medium, hard and for police😄. There is very helpfull option to limit speed. So for an example: for easy mode can make 15km/h, medium 25km/h, hard maximum allowed for your setup, police mode 4km/h 😃

These are my modes, but i still playing with numbers to get best feel. There is also default mode witch is not in this picture:

<img src="/uploads/db1493/original/3X/e/d/edb7506b7f0c77ae17c775f489e6ac268c319813.png" width="281" height="500">

But also for lower speeds also make lower amps on motor and battery and watts.
```

---
