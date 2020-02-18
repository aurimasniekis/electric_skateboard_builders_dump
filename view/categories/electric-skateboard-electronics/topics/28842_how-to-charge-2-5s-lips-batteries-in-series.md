# How to charge 2 5s lips batteries in series

### Replies: 15 Views: 2134

## \#1 Posted by: dg798 Posted at: 2017-07-28T02:27:49.879Z Reads: 112

```
How to charge 2 5S Lipo batteries in series.
Can I use maybe the 2x3s adapter from hobbyking or is that specifically made for 2x3s
```

---
## \#2 Posted by: mmaner Posted at: 2017-07-28T02:33:34.780Z Reads: 113

```
Nope you would need to charge each one idividually with a hobby charger or use a BMS.
```

---
## \#3 Posted by: rojitor Posted at: 2017-07-28T11:46:11.042Z Reads: 106

```
If you charge in series you must use a 10s bulk charger (not rc) 42v dc output. Since that is very risky people usually charges cells to 4.10 instead so you better manipulate the charger to reduce the output. This method can not be used intensely because the lipo has to be balanced. You must balance it once every 5-10 charges if you bulk charge.
If you are not a RESPONSIBLE person do not do this. Bulk charging May result in a lipo fire. You can burn your house down to ashes if you are a procrastinator. 
The safest method is making a harness cable so you switch from series to parallel just by swapping one section. You can use your rc charger and  balance it everytime. If you don't know how to make a harness I can teach you
```

---
## \#4 Posted by: dg798 Posted at: 2017-07-28T11:55:30.002Z Reads: 100

```
I don't know how to make a harness
```

---
## \#5 Posted by: SpeedSloth Posted at: 2017-07-28T12:43:11.885Z Reads: 92

```
You have to charge at 10s in series or charge them in parallel. In my board I have a connector so I can wire them together, when its disconnected I use a Y cable to charge in parallel.

By using male and female connectors in the right places you can idiot proof it ;)

<img src="/uploads/db1493/original/3X/c/1/c18beb10a55021a51dd6195e731b6b80bab2463a.png" width="564" height="500">
```

---
## \#6 Posted by: dg798 Posted at: 2017-07-28T13:13:39.751Z Reads: 91

```
I want to charge them in series.
I saw connectors on hobbyking but it's for 2x3s. Can it also be used for 2x5s?
```

---
## \#7 Posted by: jammin Posted at: 2017-07-28T15:37:41.833Z Reads: 86

```
I have a build which is two 5s batteries in series. The charging harness is just a parallel 5s balance lead connector, and I just bought mine:
https://hobbyking.com/en_us/jst-xh-parallel-balance-lead-5s-250mm-2xjst-xh-1.html
You can find these on other websites but this is what I'm talking about.

You have to use 5s balance leads for 5s batteries. If you want to charge in series, you have to buy a BMS.
```

---
## \#8 Posted by: dg798 Posted at: 2017-07-28T15:56:04.335Z Reads: 81

```
Can you put a link to a 5s Bms link on
```

---
## \#9 Posted by: dg798 Posted at: 2017-07-28T16:24:55.453Z Reads: 74

```
Well 5s in series Bms
```

---
## \#10 Posted by: rojitor Posted at: 2017-07-28T17:24:53.472Z Reads: 74

```
For just two lipo bricks the best is using just a series cable<img src="/uploads/db1493/original/3X/0/4/045c45c0e884251771e875c2fe035ddb1140c30a.jpg" width="565" height="414">
and swap to a parallel cable for charging<img src="/uploads/db1493/original/3X/4/3/431ae12ce8c75d23aa0aeb68c60ea4ed13dec5bc.jpg" width="565" height="414">
for the balance a parallel lead (do not plug this while in series, they will burn)<img src="/uploads/db1493/original/3X/c/6/c6d68a0b4af048e616d8b003ed275b166f228718.jpg" width="690" height="388">

If you have 3+ bricks a harness becomes useful. You must add an extension from every connection from the lipo to an anderson powerpole connector, They can stick together in modules like this,
<img src="/uploads/db1493/original/3X/6/1/614c17d06cef69c87eeef4b58bf1103479621c24.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/4/a/4a5c8cbed51594314418b9377824638a597385b3.jpg" width="690" height="388">
so you have all the connectors together, then you have to solder two cables one for the series like this
<img src="/uploads/db1493/original/3X/d/c/dc0c5afecb2551d1f8a4d7260417240887adf5de.jpg" width="640" height="360">
add as many series connectors as needed
<img src="/uploads/db1493/original/3X/2/3/23656c62394b94c8218dc16cbf589e6aed6ef967.jpg" width="690" height="388">
you use that cable for discharge and you need to do another parallel for charge like this
<img src="/uploads/db1493/original/3X/0/4/04fc5a63f304b39e62472a9d624aa93d6f48a569.jpg" width="690" height="388">
so you can change from series to parallel just swapping one section.
this is a parallel balance cable for more than two bricks
<img src="/uploads/db1493/original/3X/b/9/b9b955cfff92aab9ae18bb550f40dd2a15371256.jpg" width="690" height="388">
That´s the best way. It's fast and safe. If you do bulk charge you just make an adaptor from a common charger to the series discharge cable you have. As i said earlier is very dangerous if you do not do it right. You must lower the voltage from 42v to at least 41 in order to leave a reasonable margin for disbalance issues. Or use a buck converter to  set the voltage and amps you need.
[https://www.amazon.com/KNACRO-10-120V-charging-voltage-adjustable/dp/B01FGZ8HJE/ref=sr_1_1?s=electronics&ie=UTF8&qid=1501262232&sr=1-1&keywords=dc+converter+900w](https://www.amazon.com/KNACRO-10-120V-charging-voltage-adjustable/dp/B01FGZ8HJE/ref=sr_1_1?s=electronics&ie=UTF8&qid=1501262232&sr=1-1&keywords=dc+converter+900w)
Do not bulk charge more than 5-10 times in a row. Balance must be done often.
I recommend the bulk charge only for responsible people. Do it at your own risk.
Or just use bms like other dudes recommend. I'd never trust the most dangerous chemistry available to a bms by any means, But that's just my opinion. I don't usually trust bms at all.
regards
```

---
## \#11 Posted by: jammin Posted at: 2017-07-28T17:54:45.327Z Reads: 72

```
just google a 10s bms (two 5s batteries in series -> 10s total) from either Supower or bestech. Keep in mind it's a relatively involved process, what @rojitor is recommending is probably the best solution for you, although I'm just charging mine in parallel with a imax b6.

I'm also running a 10s setup (with two 5s batteries in series) and it's too not bad to set up. lmk if you have more questions
```

---
## \#12 Posted by: dg798 Posted at: 2017-07-28T19:02:44.038Z Reads: 70

```
So I can charge them in parallel but use them in series?
```

---
## \#13 Posted by: dg798 Posted at: 2017-07-28T19:04:07.525Z Reads: 67

```
I have an xt60 cable at the end of my batteries to put them in series can I just connect that to the charger
```

---
## \#14 Posted by: jammin Posted at: 2017-07-28T19:08:25.614Z Reads: 67

```
yup, just use one cable for discharge and another cable for charging.

https://www.electric-skateboard.builders/t/vanguard-orange-10s-sk3-i-vesc/1337/73?u=jammin

This build should clear things up for you
```

---
## \#15 Posted by: SpeedSloth Posted at: 2017-08-07T12:11:34.870Z Reads: 61

```
Correct, that's what the diagram I posted earlier shows you how to do (just ignore the 2/3s packs and treat them as one 5s)
```

---
