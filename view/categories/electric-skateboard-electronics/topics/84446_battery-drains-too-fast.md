# Battery drains too fast?

### Replies: 13 Views: 271

## \#1 Posted by: StefanMe Posted at: 2019-02-17T13:10:03.593Z Reads: 113

```
Hey guys, I started a run for about 15km and drained my battery to 35V (10S4P). That sounds a lot to bad for me... I run some 18650 30Q from nkon... new. 

I measured the p groups on my charge only bus unplugged:
3,54
3,55
3,54
3,54
3,54
3,55
3,54
3,55
3,54
3,54

I run 25A battery and 50A motor (never reach the 50A...)... running the HUGE 105mm all terrain rubber wheels with 15/40 ration on 6374 Motor. Does this drain the battery that much? My weight is around 85kg...

Thanks for your help guys
```

---
## \#2 Posted by: mutantbass Posted at: 2019-02-17T13:20:23.339Z Reads: 103

```
sounds about right. you used about 200wh for 15km and depending on your riding style at your weight seems fine :slight_smile:
```

---
## \#3 Posted by: Benjamin899 Posted at: 2019-02-17T14:19:25.461Z Reads: 95

```
depends on terrain. could be a bit more.
```

---
## \#4 Posted by: Petermartin9 Posted at: 2019-02-18T14:32:53.130Z Reads: 66

```
What was the air temperature you were riding through?
```

---
## \#5 Posted by: StefanMe Posted at: 2019-02-18T15:35:14.891Z Reads: 61

```
Maybe 12 degrees celsius...

I ll make a run with METR. the next days.
```

---
## \#6 Posted by: Narnash Posted at: 2019-02-18T16:01:11.353Z Reads: 57

```
Sounds about right for a dual drive, a bit on the high side but nothing unheard of. 

13,33 Wh/km isn't to bad, I usually run about 11 Wh/km with 23km/h average (more or less flat terrain).
```

---
## \#7 Posted by: StefanMe Posted at: 2019-02-18T20:46:56.443Z Reads: 43

```
https://metr.at/r/U2AsH

I did a test ride after work. 160Wh in 9.53km... not that great. 

Startet by 41V and endet at 35V. That’s just the half of the expected capacity. 

**12Ah*36V=432Wh**

**157Wh/9,53km=16.5Wh per Km**

I am close to the end by 35V... what do i missing?
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-02-18T20:53:18.857Z Reads: 40

```
Is efficiency affected when the ESC is very hot? because that would be something to take care of.... consistently 80C is oof :thinking:
```

---
## \#9 Posted by: StefanMe Posted at: 2019-02-18T21:12:17.852Z Reads: 38

```
That’s definitely a problem! 30A battery is maybe to much for the small focbox without additional cooling. I go for 25A for now. Maybe it helps.
```

---
## \#10 Posted by: pat.speed Posted at: 2019-02-18T21:14:33.851Z Reads: 38

```
3.5v for li-ion is not close to the end. More like just below half way. Those cells can go down to 2.8v safely however 3v is better for life cycles

You were also riding reasonable fast which uses lots of power and those rubber wheels have more frictional losses than urethane
```

---
## \#11 Posted by: StefanMe Posted at: 2019-02-19T12:23:48.143Z Reads: 31

```
I ll go for 32V cutoff start - 29V cutoff end.... 

I think its still a very bad result. I ordered some "normal" ABEC11 97mm wheels and new bearings. Lets see if it decreases the usage
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-02-19T13:11:32.843Z Reads: 24

```
Make sure your drive train is properly assembled and tensioned, that can decrease efficiency alot as well
```

---
## \#13 Posted by: Flashgod224 Posted at: 2019-02-19T13:14:23.131Z Reads: 25

```
Indeed, I had a bad belt length that caused one tooth to always not fit on my pulley causing it to drag/resist my drive from rolling smoothly. Which in the end causes my motors and battery to work much harder due to the handicap. Also tighter tension means more resistance, if you balance it out you can get enough free roll to give you some extra range without getting to many skips.
```

---
