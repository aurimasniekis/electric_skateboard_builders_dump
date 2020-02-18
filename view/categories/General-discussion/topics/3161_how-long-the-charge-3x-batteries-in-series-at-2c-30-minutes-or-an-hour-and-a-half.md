# How long the charge 3x batteries in series at 2C? 30 minutes, or an hour and a half?

### Replies: 10 Views: 1438

## \#1 Posted by: itsmikeholland Posted at: 2016-05-12T06:40:30.249Z Reads: 99

```
I'm planning on having 3 batteries on my vacation board with a 2C max charge rate. When charging in series, could I triple the chargers output since its being split between 3 batteries? thanks in advance!
```

---
## \#2 Posted by: Tarzan Posted at: 2016-05-12T06:58:23.879Z Reads: 95

```
If I'm correct you have to charge them parallel and then the time doubles.
But wait for someone with more experience with lipos.
Use the search function.
I'm sure you can find thins information in the forum.
```

---
## \#3 Posted by: seanpain4 Posted at: 2016-05-12T07:28:37.480Z Reads: 90

```
When in series each pack will get the exact same current. It is in parallel where the  current is divided. 

In series the voltage will be divided though, so keep that in mind.
```

---
## \#4 Posted by: mohammedex Posted at: 2016-05-12T11:26:50.506Z Reads: 82

```
If your batteries are in series then you need to charge them with a higher voltage..
Lets say we have a 3s 5000 mah battery. Charge with 11.1 volts at 2c (10ah) and charge time will be 30 min.

now if we have 3 of those 5000 mah batteries in series you would need to charge with 33.3 volts t 2c (still 10ah) and the charge time will be half an hour.

when you charge with 2c then you are charging with 2 times the batteries capacity. So it doesn't matter how big the battery pack is it will always take around 30 minutes to charge.

2c means 2x the batteries capacity so 2c on a 5000 mah is 10ah while 2c on a 15000 mah battery is 30ah

basically
charging batteries in series = use higher voltage
charging batteries in parallel = use more amps
```

---
## \#5 Posted by: seanpain4 Posted at: 2016-05-12T12:07:14.887Z Reads: 74

```
You would usually charge at the cells max voltage, or close to it, so a 3S would be charged at 12.6v.

2C on a 5000mAh is a current rate of 10A. Not Ah as its not measuring capacity
```

---
## \#6 Posted by: Namasaki Posted at: 2016-05-12T18:01:06.927Z Reads: 68

```
 First of all, let's assume that you have a balance charger designed for charging Lipos. Because there is no other way to charge them that is safe and correct. 
You neglected to mention what size of batteries your charging in series. I.e.: 2s, 3s, 4s, 5s or 6s. 
Most balance chargers are limited to 6s. 
So if your charging 3 - 2s packs in series, you'll need a series adapter for the balance leads. And then just set the charger to 6s and it will provide the correct voltage. Charge them at 1C. Or 1x ah rating
5000mah = 5amp charge rate and set the charge limit for the capacity of the battery. If the b packs are different capacities then don't charge them in series.  
Always balance charge at 1C and you won't have to worry about your batteries exploding into a fire ball.
```

---
## \#7 Posted by: itsmikeholland Posted at: 2016-05-13T06:09:27.222Z Reads: 53

```
I have 3x 4s 6600mah batteries, I'm planning on getting a 12s balance charger since I can't stand to wait an hour to charge while I'm on the go, but if it's not feasible to get all 3 charged at 2C when I'm outI might just bight the bullet and buy a weaker charger, or two of them if one goes on sale before my vesc ships out.

So ideally for 2C, i'd need a 12s >19A balance charger... is there something I should look for regarding the wattage?
```

---
## \#8 Posted by: seanpain4 Posted at: 2016-05-13T07:03:55.936Z Reads: 50

```
You could use a BMS. Otherwise, i am sure there are some high powered 12S balance chargers out there
```

---
## \#9 Posted by: Iceni Posted at: 2016-05-13T08:17:22.315Z Reads: 49

```
12s 6600mah would need 13A-ish chargecurrent for 2c.
That's almost 600 watts.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-05-13T15:41:31.875Z Reads: 47

```
I imagine that a 12s balance charger would be expensive. 
Another option is a multi bank charger. 
You can use bullet connectors to connect your batteries in series and disconnect them for charging. 
Here is a 4 bank charger. It won't quite do 2c but it does 10 amps and could probably charge your packs in 30 min. 
The best option is always charging your batteries separately. 
https://www.amazon.com/dp/B00NKO9NEW/ref=cm_sw_r_sms_api_nrFnxb6YD4J7Q
<img src="/uploads/db1493/original/2X/6/66abf21070ce260ced396eb34cf4a54611474385.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/2X/9/90c7e764c159054d359f3f5b93981f9a28d23bcd.jpeg" width="372" height="500">
```

---
