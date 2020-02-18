# Sk3 6364 190kv vesc configuration

### Replies: 13 Views: 474

## \#1 Posted by: kataklysm Posted at: 2018-06-19T07:29:15.184Z Reads: 112

```
Hi. I finishing my first board. I have vesc 4.12 with last firmware and motor Sk3 6364 190kv. What parameters i must set for safe using?
```

---
## \#2 Posted by: rey8801 Posted at: 2018-06-19T08:24:47.986Z Reads: 108

```
IT depedns on battery setup...you should give a complete description. Then we can tell you. For the moment you can calculate the predicted range and speed using http://calc.esk8.today/.
```

---
## \#3 Posted by: kataklysm Posted at: 2018-06-19T10:02:05.318Z Reads: 95

```
Ok, my setup:
Sk3 6364 190kv 
Lipo battery 10s (37v) 16ah 
Vesc 4.12 lastest firmware 
Wheels orangatang 
Gears 16-36
```

---
## \#4 Posted by: rey8801 Posted at: 2018-06-19T10:21:12.982Z Reads: 89

```
Ok so I don't know which is your battery  but since is Lipo you will have plenty of discharge current. With 16Ah the range is limitless basically. If you have a standard Maytech, TB I would start keep battery max within 30A. Battery min depends on the battery and the charging rate. You porbably have 10s2p battery so I would say start with -8A. Motor max to stay safe can be the max Amp for the motor, in your case I think 65A. Motor min start with -65A. Then adjust the min values based on how the brakes feel. Don't run in FOC, only BLDC.
```

---
## \#5 Posted by: kataklysm Posted at: 2018-06-19T13:58:38.000Z Reads: 71

```
Thanks for help. If it's not a problem, can you show it to me in screenshot from vesc tool?

My battery is lipo turnigy multistar one is 4s 10c second 6s 10c both 16ah
```

---
## \#6 Posted by: squishy654 Posted at: 2018-06-19T14:12:27.461Z Reads: 67

```
The diameter of the wheels is important too
```

---
## \#7 Posted by: kataklysm Posted at: 2018-06-19T14:24:30.658Z Reads: 66

```
Its 80mm - 56mm contact - 80a
```

---
## \#8 Posted by: rey8801 Posted at: 2018-06-19T14:26:06.796Z Reads: 67

```
I think is more important that you understand the passages. I would suggest to watch thish video https://www.youtube.com/watch?v=v1glLDO-EjA&t=1128s. it does show all the passage and you only need to adjust with your parameter. In the movie is a dual set up. Meaning you have to skip the slave part and only do the  procedure once.
```

---
## \#9 Posted by: rey8801 Posted at: 2018-06-19T14:27:17.833Z Reads: 65

```
Do you have enough ground clearance with the big battery you are gonna use and only 80mm wheels?
```

---
## \#10 Posted by: kataklysm Posted at: 2018-06-19T21:18:55.641Z Reads: 54

```
Ground clearance is ok, but i have another (big) problem. http://www.electric-skateboard.builders/t/vesc-motor-detection-faild/59395
```

---
## \#11 Posted by: rey8801 Posted at: 2018-06-19T21:23:36.881Z Reads: 48

```
Yeh DRV failure is never good. IF you buy it from HK just give it back. The nice think is that they have 1 year warranty so you should get a new one. Based on what I read that HK vesc is able to run in FOC too. I think it;s a good VESC for the price.
```

---
## \#12 Posted by: kataklysm Posted at: 2018-06-23T11:59:32.823Z Reads: 29

```
Ok, i solved this problem my vesc is alive now. What maximum A i can set?
```

---
## \#13 Posted by: rey8801 Posted at: 2018-06-23T12:10:53.120Z Reads: 27

```
If you mean Batt max, then for a normal 4.12 hardware VESC I would say 30A max. Since you had problem in the past start with 20A and increase later if everything is fine.
```

---
