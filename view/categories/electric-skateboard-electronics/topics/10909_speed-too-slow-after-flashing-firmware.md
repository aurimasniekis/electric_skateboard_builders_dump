# Speed too SLOW after flashing firmware

### Replies: 7 Views: 751

## \#1 Posted by: Thanhnd Posted at: 2016-10-10T11:18:09.235Z Reads: 91

```
Hi Builders.

I've flashing my VESC v2.18 PBC v4.1.0 but when jump on the board it too slowly (about 5km/h I guess).

Before It was work great 30-40 km/h. Please help me take a look. 


<img src="/uploads/db1493/original/3X/5/4/54cfb897f717661dbe4ba8635c4541862a1bc01f.png" width="690" height="396">

<img src="/uploads/db1493/original/3X/2/6/26bcd3b7db6345cb4c6cfffa404c529734950f87.png" width="690" height="387">

<img src="/uploads/db1493/original/3X/6/7/678a58a3c61003461313dbc43207eed0f6cfdaaf.png" width="690" height="387">

<img src="/uploads/db1493/original/3X/2/d/2d6cde5ec7e704206a1cc520a93bdf42d659bb64.png" width="690" height="391">

<img src="/uploads/db1493/original/3X/b/4/b401d4d353bd767db4b558d96b6017af35e9bdda.png" width="690" height="392">
```

---
## \#2 Posted by: Maxid Posted at: 2016-10-10T12:50:11.958Z Reads: 78

```
your battery cutoff is at 28V - what kind of battery are you using?
```

---
## \#3 Posted by: Thanhnd Posted at: 2016-10-10T13:01:01.924Z Reads: 78

```
I'm using 8s
```

---
## \#4 Posted by: Maxid Posted at: 2016-10-10T13:04:45.957Z Reads: 77

```
Lipo or Lifepo? Whats the voltage?
```

---
## \#5 Posted by: Thanhnd Posted at: 2016-10-10T13:07:57.520Z Reads: 76

```
Lipo 4.2v max
```

---
## \#6 Posted by: Namasaki Posted at: 2016-10-11T03:20:19.576Z Reads: 49

```
You should be able to go higher on your battery max amps setting with Lipos.
What are the specs on your 8s Lipo?
mah?
C rating?
Oh, just noticed your running FOC.
Could be your FOC settings.
Still 25a seems low for batt max amps
```

---
## \#7 Posted by: guyguy Posted at: 2016-10-11T14:20:49.066Z Reads: 32

```
Check your nunchuck settings under app config too - make sure your band is calibrated correctly. 

25A seems low (half of what it should be) on batt max unless you're running dual. I didn't see multiple esc over CAN ticked off so I'm assuming you're on single.
```

---
