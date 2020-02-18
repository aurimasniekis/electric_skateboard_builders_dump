# VESC Power questions

### Replies: 9 Views: 849

## \#1 Posted by: rasmukri Posted at: 2016-12-22T13:08:45.092Z Reads: 102

```
I am finishing up on my new case for the vesc. I hear that I shouldn't make it entirely enclosed, so I was thinking about installing a 20mm computer fan to the side of the case. Now it will draw 5 vdc can I plug that into the receiver for the g2xb or where should I plug that into for power that wont fry anything.
Also I am looking for a monitor for my batteries that will tell me single cell volts for a 12 cell. Also I have a drop through deck and has anyone ever installed something like that into the drop through hole right above the trucks?
```

---
## \#2 Posted by: chaka Posted at: 2016-12-22T14:38:48.455Z Reads: 93

```
It really depends on how large of a motor your are driving and gear ratio. you may not need any active or passive airflow.

Driving a fan can be done since the drv83xx has an integrated buck converter. Word of caution, drawing too much current can cause problems. The buck converter is really only meant for driving IC's or other small circuits will very low power draw. In my opinion it is better to buy a buck converter off ebay and power accessories with that instead.
```

---
## \#3 Posted by: benwong Posted at: 2016-12-22T14:43:01.097Z Reads: 88

```
Giving airflow to vesc casing will cause alot dust. Maybe i living in asia country have this kind of problem. So i seal up my vesc casing.
```

---
## \#4 Posted by: saul Posted at: 2016-12-22T16:03:10.317Z Reads: 71

```
I don't think you need cooling unless you are pushing really high power. 30mph+.

@benwong is right, theres alot of dust out on the road, sealed case is better for most applications.
```

---
## \#5 Posted by: rasmukri Posted at: 2016-12-22T16:25:02.422Z Reads: 70

```
I was thinking of having a fan blow outwards. or maybe just a hole with a filter element.

I have a 12s4p battery with dual 195kv motors. so I have gotten up to 33mph and usually cruise at about 20mph.
```

---
## \#6 Posted by: Randyc1 Posted at: 2016-12-22T20:17:21.751Z Reads: 60

```
<img src="/uploads/db1493/original/2X/1/18ef007ea900607e13a719f82570dfc9f61ada3c.jpg" width="690" height="388">
```

---
## \#7 Posted by: rasmukri Posted at: 2016-12-22T21:20:56.688Z Reads: 56

```
That looks cool, where can I get something like that battery monitor?
```

---
## \#8 Posted by: Randyc1 Posted at: 2016-12-22T21:26:24.199Z Reads: 55

```
Its called "Drok" voltage meter
```

---
## \#9 Posted by: Namasaki Posted at: 2016-12-23T19:24:03.740Z Reads: 39

```
I have dual Vesc's from Chaka with heatsinks inside an air tight enclosure and have had no issues with overheating
Running 10s with 190kv motors
```

---
