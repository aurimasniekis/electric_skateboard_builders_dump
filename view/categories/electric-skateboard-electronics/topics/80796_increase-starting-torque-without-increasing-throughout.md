# Increase starting torque without increasing throughout?

### Replies: 23 Views: 206

## \#1 Posted by: maxbicyclemax Posted at: 2019-01-13T21:07:38.898Z Reads: 86

```
Hey all. Running two Focbox’s on FOC.
Is there any setting you can increase starting torque, without increasing power throughout the rest of the range???
I’m happy with power everywhere else and don’t want more. But I do want more from 0-5% rpm.
Cheers
```

---
## \#2 Posted by: Jc06505n Posted at: 2019-01-13T21:17:01.524Z Reads: 84

```
sounds like referring to acceleration?
```

---
## \#3 Posted by: Andy87 Posted at: 2019-01-13T21:23:24.060Z Reads: 75

```
Adjust your throttle curve via vesc tool.
```

---
## \#4 Posted by: maxbicyclemax Posted at: 2019-01-13T21:23:54.033Z Reads: 74

```
I’ve played with the throttle curve and it gives a little of the effect I’m chasing.
But it’s not exactly what I’m after.
Was wondering if there’s a specific start only setting
```

---
## \#5 Posted by: Andy87 Posted at: 2019-01-13T21:25:18.684Z Reads: 69

```
Which gearing and which motors you rock?
If your start up torque not strong enough and you already adjusted the throttle curve than you probably need to change parameters there.
```

---
## \#6 Posted by: maxbicyclemax Posted at: 2019-01-13T21:26:39.205Z Reads: 69

```
Went upto 15% but back down to 10%
It’s good at 15% for a bit more kick from start, but then it’s uncomfortably aggressive everywhere else for my liking.
```

---
## \#7 Posted by: maxbicyclemax Posted at: 2019-01-13T21:28:52.161Z Reads: 60

```
I’ve got it geared very tall for high speed.
Lacroix deck 18-66t 8’ tyres.
Motors are sealed Maytech 6374 170kv
```

---
## \#8 Posted by: maxbicyclemax Posted at: 2019-01-13T21:29:55.841Z Reads: 55

```
Getting some 17t made up.
But still, that will increase torque everywhere though the range
```

---
## \#9 Posted by: Andy87 Posted at: 2019-01-13T21:30:20.600Z Reads: 55

```
I wouldn’t wonder with it.
Change the motor pulley to 15th that should give you already a good start up torque.
```

---
## \#10 Posted by: maxbicyclemax Posted at: 2019-01-13T21:32:58.774Z Reads: 52

```
Thx, did some maths and 17t is as small as I want to go... love the top end and high cruising speed.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-01-13T21:33:03.145Z Reads: 51

```
17th will not change that much.
With 18th you geared up for 70km/h 😅
💁‍♂️
```

---
## \#12 Posted by: maxbicyclemax Posted at: 2019-01-13T21:34:29.864Z Reads: 50

```
It’s a reduction of about 5%
Currently my board will do only 54kph.
I don’t think the 170kv from Maytech is accurate
```

---
## \#13 Posted by: Andy87 Posted at: 2019-01-13T21:35:27.790Z Reads: 48

```
Yap everybody how he think it’s best fit for riding.
What‘s your max speed you ever reached?
Just curious, 😅 i‘m not a speak freak and interested how long the deck stay stable without speed wobbles
```

---
## \#14 Posted by: Andy87 Posted at: 2019-01-13T21:37:27.966Z Reads: 48

```
https://calc.3dservisas.eu/?Pc8xD8IgEAXg_8JsDBRoqys1ThoSE7srQ00kJelo-t9776Fu3z2O4_ioR5jUUb1fZVY7Ka5S2H0nXsJNbCwZhY4KaNBasxhQGV-NnqbmnGmEBTNaAJ2-3isRaUPFnzjKehJhS_4HPSeeUydRr8k7rjs4h--kzLU7ZnGGHYkf1PdzYIzmNC7cGnE6XxD35IgVsHjCawet1g0=

If it does only 54kph than check the kV via vesc tool.
You should get way higher speed with this gearing.
```

---
## \#15 Posted by: Hummie Posted at: 2019-01-13T21:38:18.505Z Reads: 45

```
Increase motor amps and leave battery amps the same or reduce them
```

---
## \#16 Posted by: maxbicyclemax Posted at: 2019-01-13T21:38:58.532Z Reads: 45

```
I’ve taken it to 51kph.
Just cause I wanted to crack 50😁
But it’s not comfortable at all.
The 17t will top out at 50kph.
I just like how the motors purr at around 70-80 rpm at high cruising speed
```

---
## \#17 Posted by: maxbicyclemax Posted at: 2019-01-13T21:41:38.484Z Reads: 44

```
Yeah that’s what I thought when doing the maths.
I’ll check the Kev next time I open it up.
I was expecting 6000+motor rpm.
Works out to stop at 5500rpm
```

---
## \#18 Posted by: maxbicyclemax Posted at: 2019-01-13T21:42:14.771Z Reads: 44

```
Thx, that makes sense
```

---
## \#19 Posted by: Bjork3n Posted at: 2019-01-13T21:44:42.235Z Reads: 43

```
Raise motor amps as hummie suggested.
Makes a big diffrence IMO.
Recently went from 60 to 70A and it was a big change.
```

---
## \#20 Posted by: maxbicyclemax Posted at: 2019-01-13T21:45:15.619Z Reads: 42

```
Oh, and part reason the maths is different from real life, is.
A 200mm tyre is actually 185mm.
To get a correct reading on Xmatic.
And just measured with a ruler
```

---
## \#21 Posted by: maxbicyclemax Posted at: 2019-01-13T21:46:53.085Z Reads: 41

```
Thx. But I figured that will increase everywhere else too.... but that and reducing battery amps might be the ticket
```

---
## \#22 Posted by: Surfer Posted at: 2019-01-13T22:07:27.378Z Reads: 40

```
Did you try to reduce the positive ramping time?
Default is 0.3, try lowering it.
You will find this in settings of the vesc tool or metr.
Good luck!
```

---
## \#23 Posted by: maxbicyclemax Posted at: 2019-01-13T22:10:38.025Z Reads: 39

```
Yep, cheers, reduced it to 0.1
```

---
