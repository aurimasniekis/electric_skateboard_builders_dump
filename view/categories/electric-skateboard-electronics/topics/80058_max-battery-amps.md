# Max Battery Amps?!

### Replies: 27 Views: 1024

## \#1 Posted by: 701Superjet Posted at: 2019-01-06T01:38:47.256Z Reads: 257

```
Just curious. What are the max Amps you have pulled from your battery? Could be any Chemistry, Motors, Drive type, or Vesc.
Whats the most you have seen??
```

---
## \#2 Posted by: Saturn_Corp Posted at: 2019-01-06T01:58:23.783Z Reads: 252

```
I haven't kept very good record, but the most I've recorded is 33 amps.
```

---
## \#3 Posted by: mynamesmatt Posted at: 2019-01-06T03:10:42.376Z Reads: 246

```
considering i run an 80a bms i would say no more than 80a?
```

---
## \#4 Posted by: ShutterShock Posted at: 2019-01-06T03:18:21.811Z Reads: 245

```
I run  a 60A BMS most I have seen is 55A

Same as saturn tho I haven't paid much attention
```

---
## \#5 Posted by: Andy87 Posted at: 2019-01-06T07:45:04.625Z Reads: 238

```
I recommend to watch this videos with live data.
https://www.electric-skateboard.builders/t/4wd-heavy-duty-offroad-monster-board-vesc-c6364-sensored-12s30ah-10kw/20783?u=andy87
Probably one of the highest current drawn on an esk8
```

---
## \#6 Posted by: PatRocks Posted at: 2019-01-06T08:41:20.985Z Reads: 223

```
On my hill-climb tests, which I perform on Hill St. In San Diego (21-22% grade), i have recorded as much as 85 battery amps. But my motors breath easy on a 15/44t drive ratio. However, this is almost never at WOT, because it's _REALLY_ scary. As my lipos are aging, im seeing a voltage drop of 3.7v at that current on a 12s pack (about 0.31 v/c).
```

---
## \#7 Posted by: Bjork3n Posted at: 2019-01-06T09:04:51.382Z Reads: 220

```
On full acceleration from standstill I've seen 76A on battery amps 👹
```

---
## \#8 Posted by: sayekim Posted at: 2019-01-06T09:05:07.999Z Reads: 219

```
Some testing with too many amps. 

Motor 
120
-60
 
Battery
60
-30

Dual 6374 on escapes fw3.38. 12s6p 30q. 

https://metr.at/r/L2FVo

I have since dialed it down to 80 motor amps. I can’t trust 120 and even 100 because it gives me drv faults at random.
```

---
## \#9 Posted by: Friskies Posted at: 2019-01-06T09:29:10.130Z Reads: 198

```
120 motor amps...... Why?
Do you see the 10V sag in your voltage when hits 240A. All you are doing is forcing drv faults and overheating your motors.
```

---
## \#10 Posted by: sayekim Posted at: 2019-01-06T09:47:38.578Z Reads: 194

```
![image|320x213](upload://iEH2luUeiZlPo9VxdCL2WcSyTj6.gif)
```

---
## \#11 Posted by: Narnash Posted at: 2019-01-06T13:52:17.018Z Reads: 180

```
My max. was 108A on the battery for a brief second with my  2WD EMTB packing a 10S8P 30Q. On a short but stong incline with very low tire preasure, on dirt in the woods.

Usually I don't see more than 60A on regular rides.
```

---
## \#12 Posted by: sayekim Posted at: 2019-01-06T18:17:32.592Z Reads: 166

```
Here is the ride from today on 70 motor amp max. 

https://metr.at/r/mhfp4
```

---
## \#13 Posted by: 701Superjet Posted at: 2019-01-08T16:48:47.902Z Reads: 146

```
When you get a drv fault does it cut power?
```

---
## \#14 Posted by: Bjork3n Posted at: 2019-01-08T16:53:25.271Z Reads: 143

```
It will reset yes.
```

---
## \#15 Posted by: sayekim Posted at: 2019-01-08T17:44:04.165Z Reads: 140

```
Like they said. It will cut off and reset.
```

---
## \#16 Posted by: 701Superjet Posted at: 2019-01-09T13:49:11.031Z Reads: 125

```
I can see your running 12s. How many Ah is your pack and what chemistry?
```

---
## \#17 Posted by: sayekim Posted at: 2019-01-09T13:56:57.154Z Reads: 123

```
Samsung 30q. 

3x12x6x3,6 = 777,6 

or

3x12x6x4.2 = 907,2
```

---
## \#18 Posted by: Sn4pz Posted at: 2019-01-09T14:27:44.179Z Reads: 119

```
Whats your average range?

Im thinking of going either 12s5p or 12s6p but I cant decide, its gonna be a dual 170kv 1:6.25 165mm+ pneumie build
```

---
## \#19 Posted by: sayekim Posted at: 2019-01-09T15:14:47.345Z Reads: 119

```
Too soon to tell. 

With the cold temps on multiple days I got a max of 39km. I had to call a taxi (aka wife) to get home for the last few km. 

I do ride pretty fast. Mostly above 40-45 kph when possible. 

This one was in the rain on a full charge. Didn’t make it home either since both belts snapped. 

https://metr.at/r/GJmQv
```

---
## \#20 Posted by: Sebike Posted at: 2019-01-09T20:51:12.567Z Reads: 110

```
You asked for Ah right, so a 6p pack of 30q should be

6 x 3000mAh = 18Ah

Chemistry is NCA
```

---
## \#21 Posted by: 701Superjet Posted at: 2019-01-09T22:43:51.743Z Reads: 97

```
I wouldn't think a 12s6p 30q pack would sag that much.
```

---
## \#22 Posted by: sayekim Posted at: 2019-01-09T23:14:34.702Z Reads: 98

```
Well it wouldn’t if you’d went for lower amp settings which apparently most people ride with. I just really like my punch nice and spicy.

Don’t forget I’m also riding in cold 5C weather which really makes a big difference.
```

---
## \#23 Posted by: 701Superjet Posted at: 2019-01-09T23:42:28.356Z Reads: 97

```
Ah ya the cold will do it. I ride at 100 motor amps on my unity. I love the punch as well and would take more if I could get it.
```

---
## \#24 Posted by: Sn4pz Posted at: 2019-01-10T01:32:38.367Z Reads: 93

```
[quote="sayekim, post:22, topic:80058"]
really makes a big difference.
[/quote]


Any Metr data that shows you doing some high speed pulls on a warm day? 

I cant decide between 30q or 30t or 40t

I would pay out the wazoo for 40t or even 30t but its about building my final (LOL, ok) build, and I want it to be perfect*

*very minimal voltage sag, at least 20mi range on pneumies at 75% throttle, and a top speed of 25mph(limited by the esc, I dont want to kill myself)
```

---
## \#25 Posted by: hyperIon1 Posted at: 2019-01-10T05:15:59.399Z Reads: 88

```
new kid on the bock
samsung 50E 21700
![35%20PM|660x500](upload://nVXOhqsYP6SyvqdTN2THTHv6ZH5.png)
```

---
## \#26 Posted by: hyperIon1 Posted at: 2019-01-10T05:18:19.463Z Reads: 87

```
![IMG_1114|388x499](upload://rUPVU6MFsKEW7MiuJrxqhyj7c1m.jpeg) ![IMG_1113|383x500](upload://4Q9vpr209EXaBXQU2bh7SJbHpdu.jpeg)
```

---
## \#27 Posted by: sayekim Posted at: 2019-01-10T06:41:44.758Z Reads: 79

```
Unfortunately not. My first and second rides on this build it was around 1C outside. 

https://metr.at/r/INxWh

https://metr.at/r/PTuRT

It’s my understanding lipo will give you minimal sag but until I have tried them out I won’t trust that. More p on li ion should give you less sag too but since I also use a lot more power with more it ends up being more sag than on a 2 p setup or equivalent.
```

---
