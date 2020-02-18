# 6s setup to 12s

### Replies: 16 Views: 2896

## \#1 Posted by: saabsaviorlee Posted at: 2016-02-04T23:33:05.721Z Reads: 154

```
Hey all, sure enough I've outgrown my 6s single motor setup. My question is, as I jump up to 12s and a VESC what other pieces do I need?

I have a DIYElectricskateboard power switch
series cable
DIYElectric 2.4 ghz rx tx

My plans is to get 2 6s batteries and run em in series using the existing series cable that is connected to the  power switch.

Does the VESC need a UBEC? 
Do I just solder the power wires from power switch onto VESC and plug rx and I'm done?

Is it really that easy or am I missing something?
```

---
## \#2 Posted by: saabsaviorlee Posted at: 2016-02-04T23:40:00.249Z Reads: 154

```
<img src="/uploads/db1493/original/2X/2/29a88594c8e07b4e42140d0ab98deb0e7d364023.jpg" width="374" height="500">
```

---
## \#3 Posted by: torqueboards Posted at: 2016-02-05T02:12:25.875Z Reads: 143

```
You can just swap with the VESC and replace it for your current ESC. It's an easy swap. We plan on having VESCs in stock shortly.

Ollin and Enertion both have VESCs available.
```

---
## \#4 Posted by: saabsaviorlee Posted at: 2016-02-05T02:26:50.845Z Reads: 139

```
Awesome thanks, Torque! Your 6s kit will make switching to 12s so easy then!  I'm maxing out at around 12mph on the 6s setup. (hefty rider) what kind of speeds would you estimate I'll reach with 12s?
```

---
## \#5 Posted by: Namasaki Posted at: 2016-02-05T03:07:22.594Z Reads: 139

```
<img src="/uploads/db1493/original/2X/5/59f2a7a7a25520e4325fe0825519eed5280df0da.png" width="281" height="500">
```

---
## \#6 Posted by: Namasaki Posted at: 2016-02-05T03:07:41.795Z Reads: 138

```
<img src="/uploads/db1493/original/2X/a/a8e116dad5731d40724cc42857aef9036f82477f.png" width="281" height="500">
```

---
## \#7 Posted by: Namasaki Posted at: 2016-02-05T03:13:04.647Z Reads: 137

```
I used the trans ratio to factor in rider weight. 
So if your getting 12mph with 6s, you should see 24mph with 12s using same motor, gears and wheels. With 12s you should see a lot more torque as well and you will be pulling less amps so you should see better range unless I'm mistaken.
```

---
## \#8 Posted by: saabsaviorlee Posted at: 2016-02-05T03:27:18.582Z Reads: 134

```
That's awesome @namasaki thanks! I'm pretty stoked for more speed!
```

---
## \#9 Posted by: Namasaki Posted at: 2016-02-05T03:33:50.919Z Reads: 134

```
Btw, the app i used is called gear speed. its an iphone app
Another really cool iphone app is SpeedTracker. ( a gps speedometer that records your avg and max speed in a given run.
Oh and, you will be stoked!
Jumping form 12 to 20+mph is huge! At least it was for me...
```

---
## \#10 Posted by: saabsaviorlee Posted at: 2016-02-05T03:51:39.653Z Reads: 128

```
I have android but I'll look into android equivalents. I am looking forward to the speed jump, helluva lot easier than dropping 50lbs! I might actually have to tune my trucks. Haven't gone fast enough to get the wobbles yet!
```

---
## \#11 Posted by: Namasaki Posted at: 2016-02-05T04:33:44.303Z Reads: 123

```
double barrel bushings something around 90A. I'm using orangatang nipples 89A, works good for my weight 185lbs
very stable at 20mph
I'm pretty sure there are similar apps for android.
```

---
## \#12 Posted by: massy Posted at: 2016-02-05T14:09:36.502Z Reads: 112

```
Just to comment at the range thing. Yes, you pull less amps but cost wise etc 6s 10000 mAh is usually as expensive as 12s 5000 mAh which should correspond to the same amount of energy. Guess the biggest perk is higher voltage.

Upgrading a 5000 mAh 6s setup to 5000 mAh 12s though should give roughly double the range.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-02-05T16:30:43.882Z Reads: 106

```
6s to 12s
Double speed
Double range
Although I don't think you get both at the same time. 
I believe it's double range at 12 mph
or same range at 24 mph, but I can't really say for sure. It's just theory. 
And less amp pull means less heat in the motor and Esc if I'm not mistaken.
```

---
## \#14 Posted by: saabsaviorlee Posted at: 2016-02-05T19:21:52.528Z Reads: 102

```
I'm pretty excited for double the speed. I haven't hit my voltage cutout so the range at 6s seems to fit my needs for now. With more power I might find myself going farther though. I've only gone a few miles at a time so far.
```

---
## \#15 Posted by: massy Posted at: 2016-02-05T22:21:20.009Z Reads: 97

```
That's absolutely correct. You have P=U*I where P is watt, U is voltage and I is amps. 

So 2000 watts at 6s drains I = 2000 W /22 V  => I= 91 amps...

..while 2000 watts at 12s drains I = 2000 W/44 V => I= 45.5 amps.

This roughly translates to "a 12s battery of the same capacity(mAh) as a 6s battery gives AROUND the double range at the SAME SPEED"
```

---
## \#16 Posted by: onloop Posted at: 2016-02-06T04:24:34.237Z Reads: 93

```
That app looks nice!
```

---
