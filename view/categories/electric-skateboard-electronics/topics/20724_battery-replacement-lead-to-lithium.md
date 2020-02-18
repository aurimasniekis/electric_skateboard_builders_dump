# Battery Replacement, Lead to Lithium?

### Replies: 30 Views: 2649

## \#1 Posted by: ExtraSour Posted at: 2017-04-10T13:43:27.691Z Reads: 173

```
I have recently purchased a moto tec off road E-board however i didnt realize the battery was a lead acid until it arrived. (should have read more into i guess) Anyways i was curious if it was possible to switch it from a lead acid to a lithium. The lead battery has an output of 36v with 14ah and the motors are both 800w requiring 36v and a rated current of 28.5A (there are 2 of them) Basically what i am asking is if anyone knows a lithium battery that will work with this set up? Heres a link to the motors/speed controller

http://www.bigtoysusa.com/mototec-skateboard-800w-36v-motor.aspx
http://www.bigtoysusa.com/MT-SKT-1600-electronic-controller.aspx
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-04-10T13:47:03.587Z Reads: 165

```
36V equals 10s lithium batt.
So get for example 2x 5s Lipos. Connect them in series and you´re good to go.
You could also take 5x 2s Lipos
```

---
## \#3 Posted by: ExtraSour Posted at: 2017-04-10T13:59:59.195Z Reads: 158

```
Im kind of new to this if you cant already tell, would i just go higher in the number of cells to make the range of the board longer or would i have to just stay with 10s and go higher in the mah? as of now this board only has a range of 10 miles.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-04-10T14:06:26.998Z Reads: 150

```
this is an inrunner motor, so not really efficient for an eskate and if you start replacing parts, you end up better getting rid of that thing and building your own ;)
If thats and 36V ESC you have to stay with 10s and put more cells in parallel to add mah, just do a bit research here
```

---
## \#5 Posted by: Namasaki Posted at: 2017-04-10T15:37:38.713Z Reads: 122

```
@TarzanHBK
10s Li-ion or Lipo is not 36v
It's 42v at full charge. 
Lifepo4 cells would probably work since they are 3.65v at full charge.
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-04-10T15:49:17.715Z Reads: 109

```
The lead battery is 36V nominal too, so no problem in using a 10s lipo here
```

---
## \#7 Posted by: ExtraSour Posted at: 2017-04-10T18:41:39.526Z Reads: 106

```
the lipo's weigh substantially less then the lead acid correct? Thats my main concern with this is to get the weight and charge time down. Right now it takes a good 6 hours to charge this battery.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-04-10T20:03:23.919Z Reads: 97

```
Fully charge your Lead Acid battery with its designated charger and check its voltage just to be on the safe side. If it charges up to at least 42v then your good to go with Lipos.
```

---
## \#9 Posted by: ExtraSour Posted at: 2017-04-10T21:03:23.869Z Reads: 94

```
I would have to run to the store and grab a voltage meter. However for the time being i did find out its not 1 battery but 3 in series. <img src="/uploads/db1493/original/3X/8/a/8a3640b6bbb12227c7c07c62523dcbf5166c2653.jpg" width="374" height="500">
```

---
## \#10 Posted by: Namasaki Posted at: 2017-04-10T21:47:36.429Z Reads: 85

```
3 12v batteries in series. 
You might be able to find out by the charger. 
If it has input and output info printed on it. 
the output voltage will be your battery's full charge voltage.
```

---
## \#11 Posted by: ExtraSour Posted at: 2017-04-10T21:59:33.056Z Reads: 83

```
Input:100-240VAC,50/60Hz 1.5A
Output: DC+36V/2A
```

---
## \#12 Posted by: Namasaki Posted at: 2017-04-10T22:10:26.522Z Reads: 83

```
This is what I suspected, your battery is only going to be 36v at full charge. So your system is designed for 36v. 
If you go higher i.e.: 10s Lipo or Li-ion, 42v,
there is a possibility that you could damage the system and then it won't work at all.
You could put a couple 4s Lipos in series which would give you 33.6v at full. You will have some performance loss and you would need a balance hobby charger to charge them. And this might not work either if there is a battery management system built in to the electronics because it would be designed for the 36v lead acid batteries.
```

---
## \#13 Posted by: IsTalo Posted at: 2017-04-10T22:20:25.345Z Reads: 81

```
He could go with less voltage, lose a bit of speed but increase the range compared to the Lead acid batteries
```

---
## \#14 Posted by: Namasaki Posted at: 2017-04-10T22:29:38.952Z Reads: 77

```
The range with the lead acid battery is 10 miles. 
Not bad really. 
The total weight of the board is 71 lbs
Which is really heavy.
Looking at the batteries, I don't see any type of wiring for a management system so that is probably not an issue.
```

---
## \#15 Posted by: IsTalo Posted at: 2017-04-10T22:31:58.901Z Reads: 74

```
So a 8s battery would give more range, less speed (But the board will be lighter, so maybe, more speed).
 But it, maybe, don't work well, because the potentiometer is for 36v (I mean, it maybe uses Duty Cycle, so the voltage is relevant), so 8s or 10s will get it crazy, right?
```

---
## \#16 Posted by: Namasaki Posted at: 2017-04-10T22:36:12.223Z Reads: 73

```
10s 42v might burn the circuits out. No way to be sure. 
He could try 8s 33.6. 
Like you said, the lighter weight might make up for the loss of voltage.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-04-10T22:45:45.578Z Reads: 68

```
Two of these might do it. 
https://hobbyking.com/en_us/zippy-flightmax-8000mah-4s1p-30c.html
```

---
## \#18 Posted by: ExtraSour Posted at: 2017-04-10T22:52:17.905Z Reads: 70

```
Is there some sort of management system i could get to run the 10s lipos but run it through a resistor of some sort to get it back to 36v?
```

---
## \#19 Posted by: IsTalo Posted at: 2017-04-10T23:05:16.706Z Reads: 74

```
I think some mosfets could do it, but go with 8s, is cheaper and the chargers are cheaper
```

---
## \#20 Posted by: Namasaki Posted at: 2017-04-10T23:05:23.306Z Reads: 78

```
No but you could get a 10s battery pack made of lifepo4 cells that would be 36.5v at full charge together with a BMS and then you could use a simple charger like the one you already have. 
@barajabali is a lithium battery maker who could probably help you with that. 
The Lifepo4, also known as A123 cells are also high amp output so they work well with e-boards.
```

---
## \#21 Posted by: JonasHoNobleHouse Posted at: 2017-04-11T03:54:01.289Z Reads: 66

```
Greetings Guys. Would an eBay 36v 30ah lithium battery (e-bike, scooter), work for this MotoTec 1800watt off-road skateboard. I have the same question. Thanks.
```

---
## \#22 Posted by: JonasHoNobleHouse Posted at: 2017-04-11T03:55:28.832Z Reads: 72

```
https://www.ebay.com/itm/201864169307
```

---
## \#23 Posted by: Namasaki Posted at: 2017-04-11T04:27:40.363Z Reads: 73

```

The listing description says 10 30ah cells
42v charging voltage 36v operating. 30ah cells?
@barajabali Have you ever seen anything like this? 
<img src="/uploads/db1493/original/3X/c/1/c1f0a3d2777c0d3d1351db282d9ac959cebf5bc9.jpg" width="500" height="490">
<img src="/uploads/db1493/original/3X/f/f/ff95d5a67d9e74f65645a9af2999d387ee8fe413.jpg" width="376" height="500">
<img src="/uploads/db1493/original/3X/0/7/07ca69e15658fb9b0e6139216549ea1814535ba8.png" width="658" height="500">
```

---
## \#24 Posted by: ExtraSour Posted at: 2017-04-11T05:06:35.778Z Reads: 66

```
If the battery wasnt 480$ i could probably justify getting it xD however seeing as how i could build a single motor e board for the price of say 500-600 i would probably go that route instead of paying that much for a battery.
```

---
## \#25 Posted by: JonasHoNobleHouse Posted at: 2017-04-11T12:50:13.685Z Reads: 66

```
My goal is to increase range and decrease weight on my MotoTec 1600w electric skateboard. I am currently using 3 -12v 15ah sealed lead acid battery and was wondering if I can swap these out. I understand it will be an expensive gamble, but was wondering if this will work or a better recommendation.  Thanks for all of y'all times.
```

---
## \#27 Posted by: longhairedboy Posted at: 2017-04-11T13:13:21.634Z Reads: 62

```
Specs usually refer to nominal voltages though. 36v for 10S is 50% charge. Nominals for liion can be 3.6v or 3.7v occasionally, lipos are almost always 3.7v and lifepo4 is 3.2v or 3.3v ish.
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-04-11T13:15:54.022Z Reads: 62

```
that's one fat pack!
```

---
## \#29 Posted by: Namasaki Posted at: 2017-04-11T13:51:12.620Z Reads: 58

```
The thing I don't get is they advertise it as lifepo4 
10s which should be 36.5v full but it comes with a 43.8v charger.
```

---
## \#30 Posted by: Psyborg Posted at: 2018-04-24T03:58:58.527Z Reads: 40

```
Did you Ever Successfully upgrade your battery? Im looking to do the Same
```

---
## \#31 Posted by: riley25 Posted at: 2018-08-02T13:52:06.352Z Reads: 25

```
Did anyone ever do this battery upgrade? Curious to see how this worked out. I am in the same situation
```

---
