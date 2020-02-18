# How to increase speed on ranger x2?

### Replies: 9 Views: 260

## \#1 Posted by: Pambalos Posted at: 2019-09-22T17:18:29.376Z Reads: 64

```
Hey guys,

I was wondering if anyone here had some concrete advice on how to increase the top speed on my backfire ranger x2. I've heard that adding voltage works, but with a prebuilt battery pack, that isn't very easy unless I just connect a whole second battery in series, but that would double the voltage heading to the ESCs. Would that break those components? If so, how else can I look to increase my range? Thanks!

Ranger x2 specs:
|**Weight of Board**|**10.8KG**|
| --- | --- | --- |
|**Dimensions**|110*33*16.5cm|
|**Range**|16- 22 miles or 26-35km|
|**Top Speed**|35km/h|
|**Hill Climbing**|Up to 30%|
|**Remote**|R2 Wireless Remote with OLED Display|
|**Battery**|12S 50.4V 454Wh|
|**Tire**|Thickening Honeycomb Structure Airless|
|**Hub Motor**|1200W*2 Hub Motors|
```

---
## \#2 Posted by: Chaki Posted at: 2019-09-22T17:39:50.916Z Reads: 59

```
Well it's a nightmare to be honest. the simplest way is to sell it ang get a beltdrive board. 

1200W @ 50v = 24 A
At 50v (12s) ur motor can handle 24A. not sure even vesc can help with those hub motors. u need to change out the motors and wheels and get pulleys and belt and motormount and maybe vesc's. 
but hopfully i'm wrong and someone will give u more posetive help.

Just loosen up ur trucks and master carving at 35km/h.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-09-22T17:49:14.609Z Reads: 53

```
[quote="Chaki, post:2, topic:102088"]
1200W @ 50v = 24 A At 50v (12s) ur motor can handle 24A
[/quote]

thats actually what the esc can handle (24A) the motors can definitely do more.
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-09-22T17:50:08.130Z Reads: 52

```
[quote="Pambalos, post:1, topic:102088"]
that would double the voltage heading to the ESCs. Would that break those components?
[/quote]

double the voltage would fry your esc instantly.
```

---
## \#6 Posted by: Pambalos Posted at: 2019-09-22T18:28:39.475Z Reads: 43

```
Exactly. Do you know what I could do instead?
```

---
## \#7 Posted by: Pambalos Posted at: 2019-09-22T18:30:09.827Z Reads: 42

```
Would the move be to switch out the esc?
```

---
## \#8 Posted by: Pambalos Posted at: 2019-09-24T07:55:38.848Z Reads: 21

```
Apparently the speed limit is in place because of drain speed on the batteries. Apparently they don't have enough amperage to supply the motors, so the esc limits the speed
```

---
## \#9 Posted by: Ben.Nexus Posted at: 2019-09-24T08:05:32.963Z Reads: 21

```
You may be able to lift any limits by using either a 30A Hobbywing ESC (Although they're super rare in 12S, I don't think you'll be able to find one) Or a dual VESC.
```

---
## \#10 Posted by: Pambalos Posted at: 2019-09-24T08:21:51.511Z Reads: 21

```
I think I could remove the hard coded limit from the esc, I think it's the batteries which are the issue, according to backfire themselves
```

---
