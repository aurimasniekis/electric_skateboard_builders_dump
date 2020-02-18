# Crazy range, Does this sound right?

### Replies: 24 Views: 599

## \#1 Posted by: Battosaii Posted at: 2019-01-16T19:55:28.363Z Reads: 266

```
So I have not fully drained my battery yet but I built a 12s8p for my 4wd, right now Ive been running 2wd cause I blew 2 Focboxes (my mistake).

I've run it twice on 2wd one at South Beach I got 12.7 miles distance with 97% battery left and Sunday I went to key Biscayne and did 13 miles but this area had 2 steep hills and I finished with 94% battery. 

Does this mean I could potentially have 100mile range?
```

---
## \#2 Posted by: brenternet Posted at: 2019-01-16T19:57:15.338Z Reads: 259

```
https://calc.3dservisas.eu/ :man_shrugging:
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-01-16T20:10:15.511Z Reads: 254

```
How are you calculating your battery percentage? It's possible your meter/calculations are off. That range number does sound a little high.
```

---
## \#4 Posted by: rsalmon Posted at: 2019-01-16T20:17:43.275Z Reads: 246

```
If this percentage is based on voltage, keep in mind most of the energy density will be between 3.6v - 4.1v (43v - 49v in a 12s pack). Below that, the voltage starts dropping much faster. 

Thats why a percentage based on voltage can be very misleading.
```

---
## \#5 Posted by: thisguyhere Posted at: 2019-01-16T20:19:29.176Z Reads: 239

```
best would be run vesc monitoring of some kind, it gives you a per mile watt-hour reading.  then take total watt hour of your battery, divide by watt-hour / mile, that should be rough total range of your 12s8p pack.
```

---
## \#6 Posted by: Battosaii Posted at: 2019-01-16T20:25:25.047Z Reads: 229

```
Well I calculated it I was at 48.8v after the first trip and 47.2v after the second trip
```

---
## \#7 Posted by: Battosaii Posted at: 2019-01-16T20:26:15.779Z Reads: 220

```
Hmm maybe 100miles is pushing it but I feel like 50-60miles is very doable.
```

---
## \#8 Posted by: danggilmore Posted at: 2019-01-16T20:27:20.720Z Reads: 209

```
You prolly have your lcd set to the wrong “series” and it’s giving a wierd reading
```

---
## \#9 Posted by: Battosaii Posted at: 2019-01-16T20:28:32.956Z Reads: 204

```
Nope it shows voltage and its the same value on my phone as my lcd voltage checker
```

---
## \#10 Posted by: evoheyax Posted at: 2019-01-16T20:43:31.388Z Reads: 196

```
Well assuming these are 30Q cells, your talking 12s @ 36ah. That's almost 1600 wh. If you have a super efficient drive train and motor setup, you'd do around 14 wh per mile (riding 15 mph, flat, no wind, constant throttle). Which at that, means you'd be able to do 114 miles. I find myself with 4wd pulling more like 40 wh per mile, which would yield me 40 miles. I just built a 12s 25ah which is 1100 wh, and by my math, that's 27.5 mile. I'm curious to see how it is in the real world.

Bigger batteries are defiantly trendy right now!
```

---
## \#11 Posted by: Andy87 Posted at: 2019-01-16T20:56:28.524Z Reads: 181

```
[quote="evoheyax, post:10, topic:81096"]
Bigger batteries are defiantly trendy right now!
[/quote]

Seems like i‘m swimming against this trend 😅
I‘m currently try to get the lightest battery possible but still have the performance I need.
```

---
## \#12 Posted by: evoheyax Posted at: 2019-01-17T00:34:01.263Z Reads: 152

```
Well if you want real performance with li-ion, it has to be big. And if you use lipos in bulk, you can eliminate voltage sag by going big.
```

---
## \#13 Posted by: Battosaii Posted at: 2019-01-17T01:00:30.064Z Reads: 142

```
It is a 30q 12s8p but how did you get 1600wh? Just curious cause 12s4p 30q is 532wh I assumed by doubing the battery I'd have double the wh so 1064wh is that correct or is my math wrong?
```

---
## \#14 Posted by: yelnats8j Posted at: 2019-01-17T04:01:46.639Z Reads: 129

```
Your correct, It should be 1036.8 according to the calculator 1600 is way off
```

---
## \#15 Posted by: filmerskier97 Posted at: 2019-01-17T06:38:40.402Z Reads: 120

```
my 12s7p gets me about 35miles in the "real world"
```

---
## \#16 Posted by: b264 Posted at: 2019-01-17T08:28:19.762Z Reads: 112

```
[quote="evoheyax, post:10, topic:81096"]
Bigger batteries are defiantly trendy right now!
[/quote]

They're defiant because they're resistant to carrying around
```

---
## \#17 Posted by: Battosaii Posted at: 2019-01-17T08:32:06.020Z Reads: 110

```
It's because they are soposed to carry you lol. Imo the 4wd is more of a hassle than the weight.
```

---
## \#18 Posted by: meesie Posted at: 2019-01-17T08:48:13.210Z Reads: 110

```
12S8P with average usage of 8Wh/km (yes, km, i'm sorry) should get you about 130 Km's far. which is about 80 miles.

i calculated this as such: 44.4V (12s) / 24Ah (8p when using samsung q30) =  1065 Wh
1065 Wh / [your average usage per mile] = max range
```

---
## \#19 Posted by: LEE Posted at: 2019-01-17T08:55:54.694Z Reads: 112

```
 I am also interested in big batteries.
4motor is heavy.
I prefer 2WD with more batteries.
I am planning 12s 10p of SANYO 18650GA (3.5 Ah).

https://electricbike.com/forum/forum/batteries/18650/52414-3500mah-league-sanyo-ncr18650ga-panasonic-ncr18650ga-lg-mj1-samsung-inr18650-35e
```

---
## \#20 Posted by: evoheyax Posted at: 2019-01-17T16:01:57.184Z Reads: 99

```
oh sorry, I messed up the ah haha, 36ah would be a 12s12p, 24ah is a 12s8p, as 3ah x 8 = 24.

Still, anything over 1 kwh is pretty good and I would still expect at least 30 miles on it without a doubt and probably much more if your efficient.
```

---
## \#21 Posted by: Blitz Posted at: 2019-01-17T23:17:15.450Z Reads: 84

```
[quote="evoheyax, post:10, topic:81096"]
That’s almost 1600 wh.
[/quote]

Are you sure Because you get less WH running higher currents.

Edit: Just checked yea you were way off.
```

---
## \#22 Posted by: evoheyax Posted at: 2019-01-17T23:28:33.437Z Reads: 84

```
I already said I made a mistake with calculating wh
```

---
## \#23 Posted by: Battosaii Posted at: 2019-01-18T00:03:36.185Z Reads: 77

```
We did 21.4 miles last night and I had to pull a 230lb dude on an old space cell build a few miles and up all the bridges I finished with 45.3v 

Last night's ride had a few hiccups. Like my belt snapping cause it was too tight, I also have an issue with my right rear motor, I believe it's a sensor issue cause it randomly stutters at very low speeds or from a.stop or even upside down with no load, but once it's moving it works fine. I had this issue with the regular Focbox but I thought it was an issue with the Focbox but I still have the same issue with the unity. I may try swapping out the sensor wire from left to right and seeing of the problem jumps to the other motor.
```

---
## \#24 Posted by: hyperIon1 Posted at: 2019-01-18T03:00:57.794Z Reads: 63

```
By the calculator and using Samsung 30q
![image|690x288](upload://RbOw4XXgkihA6PVx4w1vmUj4TA.png)
```

---
