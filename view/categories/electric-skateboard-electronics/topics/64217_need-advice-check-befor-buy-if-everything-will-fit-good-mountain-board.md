# Need advice/check befor buy - if everything will fit good (Mountain Board)

### Replies: 7 Views: 239

## \#1 Posted by: derbe Posted at: 2018-08-08T09:15:18.242Z Reads: 68

```
Hey guys,

I plan to build a 2x  Mountain Board. One for me one for a friend (But I will do all the work here)

Here are my planed parts:

- Trampa Board Vertigo  with Superstar wheels
- Direct Drive (from E-troxx)
- 190 KV Sesored (https://de.aliexpress.com/item/6368-BLDC-outrunner-brushless-motor-190KV-280KV-620KV-sensored-sensorless-22-48V-for-electric-balancing-scooter/32844026701.html?spm=a2g0s.9042311.0.0.68654c4dUaYaCj) does this one fit on the direct drive?
- Maytech Vesc 50a (I already own one which work well for now)
- Batterie 4x 5000mAh from Hobbyking (put 2x 6S) as 12S (https://hobbyking.com/de_de/turnigy-battery-heavy-duty-5000mah-6s-60c-lipo-pack-xt-90.html)
- I already have Quantum controller (I build one normal e board which work fine for now)
- Search for package for Vesc and Batterie (should stay on the board between legs)

Question is if I use 12S (44.4V) @ full load it is like 50V and the motor can handle 2340W for me its like should be at 44,4 V @ 52A (2A too low but okay for me) for max Watt or at 50V 49A looks like vest fit well right? Or do I lose a lot power here cause of the 50A vesc?

Other question is do I need to send trampa trucks to etoxx? Or does the driect drive already fit there? Or do I get trucks with that motor mount?

I also serch for cheap box for vesc and batterie any ideas?

Mabye you have some ideas for improvements for me ?

Thanks!
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-08T11:41:17.317Z Reads: 43

```
As far as I know the trucks need to be modified.
You can order them directly to etoxx or sent them after you received by trampa there.
Did you already get in contact with jens?
If no just write him.
```

---
## \#3 Posted by: derbe Posted at: 2018-08-08T11:52:13.014Z Reads: 40

```
I aready did, waiting for anwser.
```

---
## \#4 Posted by: rich Posted at: 2018-08-08T16:47:16.237Z Reads: 38

```
All 63mm motors fit the drivetrain but I would go with sensored 6374 between 130-150kv (max. 170) dependent on your desired top speed, weight, terrain and if you want to climb hills.

I'm not sure if Maytech V4.12 can do FOC (the new version), last year they didn't. IMO sensored FOC is a must in combination with vesc on MTB.
```

---
## \#5 Posted by: derbe Posted at: 2018-08-08T17:14:30.316Z Reads: 35

```
I think they can, but it not recommanded for what ever reason. I dont have the XP with FOC but is that really worth? I thought sensored Motor should be good enough. And I took 190kv because would like to have speed arround 50km/h.
```

---
## \#6 Posted by: rich Posted at: 2018-08-08T19:22:32.427Z Reads: 27

```
[quote="derbe, post:5, topic:64217"]
I thought sensored Motor should be good enough
[/quote]


Exactly what I thought last year but look here

https://youtu.be/ptlHqK7kqCA

The performance  was really annoying and ridiculous in hybrid or sensored BLDC. FOC for the win.

With 190kv you'll get about 60km/h top speed
```

---
## \#7 Posted by: derbe Posted at: 2018-08-08T20:17:55.168Z Reads: 19

```
Wow, thats  a very big difference. You got me, hm okay I need to check if my maytech can handle FOC I will test the next days otherwise I need another VESC for FOC which can do it without killing my bank account? :smiley:
```

---
