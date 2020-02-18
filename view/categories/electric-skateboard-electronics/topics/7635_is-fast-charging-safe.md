# Is fast charging safe?

### Replies: 10 Views: 1472

## \#1 Posted by: Tijmen Posted at: 2016-08-14T18:23:53.567Z Reads: 135

```
I use an iMax b6 6A 80W charger to charge my two 8000mAh 30C 3s batteries in parallel using a parallel charging board. I was wondering about the fast charge option on the charger.
Normally I charge at 6A but I think that takes 8 hours to charge...

My question is if fast charging is putting my batteries at a risk. I understand that fast charging doesn't balance charge them, but I could use one of those balancer things to balance them after I think, and balance charger when I don't need fast charging.
Also, how much faster would fast charging be. Would it even be worth it?
```

---
## \#2 Posted by: maxchilton Posted at: 2016-08-14T18:45:39.820Z Reads: 128

```
[quote="Tijmen, post:1, topic:7635, full:true"]
I use an iMax b6 6A 80W charger to charge my two 8000mAh 30C 3s batteries in parallel using a parallel charging board. I was wondering about the fast charge option on the charger.Normally I charge at 6A but I think that takes 8 hours to charge...

[/quote]

your charger is capable is 6s charging so charge in series, not parallel. Charging at 8ah 6s pack at 6a  will take about 1 hr and 20 minutes, not 8 hours.   It's simple math. 


[quote="Tijmen, post:1, topic:7635, full:true"]
My question is if fast charging is putting my batteries at a risk. I understand that fast charging doesn't balance charge them, but I could use one of those balancer things to balance them after I think, and balance charger when I don't need fast charging.Also, how much faster would fast charging be. Would it even be worth it?
[/quote]

Anything below 1c charging is perfectly fine.
```

---
## \#3 Posted by: Tijmen Posted at: 2016-08-14T18:59:12.107Z Reads: 125

```
[quote="maxchilton, post:2, topic:7635"]
your charger is capable is 6s charging so charge in series, not parallel.
[/quote]

I'm assuming I'd have to solder up a little harness to do that then but that's ok. If I were to do that though, then how would it work out for the balance cables? 
And just to double check, you're saying that I could balance charge much quicker if I were to charge in series and at 6S right?
```

---
## \#4 Posted by: Jeefberky Posted at: 2016-08-14T19:29:55.989Z Reads: 120

```
The charger is 80W. 
Max charging amps will be something like 3A @6S (series charging).
@3S max charging amps will be something like 6A (parallel charging).

I also charge 2x 3S in series and it takes about a hour to complete the charge (5000mAh balance charging).
The charger will only stop sooner with charging if fast charging is selected because the charger does not top off the cells to their max capacity level.
```

---
## \#5 Posted by: Tijmen Posted at: 2016-08-14T20:14:49.625Z Reads: 106

```
How do you do your balance cables when wired in series? Mind showing me a picture?
```

---
## \#6 Posted by: Jeefberky Posted at: 2016-08-15T07:10:38.213Z Reads: 85

```
A verry crude drawing. Notice that one of the wires from the balance plug from one of your batteries is not connected (green wire in drawing).

<img src="/uploads/db1493/original/2X/1/12a551747b97121c7da08d77cf2f8ebb8141a3cf.jpg" width="660" height="258">

Maybe this site also helps:
http://scriptasylum.com/rc_speed/lipo.html
```

---
## \#7 Posted by: Tijmen Posted at: 2016-08-15T07:12:11.684Z Reads: 80

```
I'll have to do some more research on this before I wire everything up, but could you explain as to why the green wire isn't connected? Wouldn't that be unsafe?
```

---
## \#8 Posted by: Jeefberky Posted at: 2016-08-15T07:15:44.845Z Reads: 77

```
The green wire is doing the same as the first black wire from the right 3S LIPO pack. A 6S LIPO has 7 wires comming from the balance plug. A 3S LIPO has 4 wires. Combining two 3S LIPO batteries in series wil not give you a balance plug with 8 wires.

Be carefull when doing this. You could fry your chargers balance plug when wiring like the picture below.
<img src="/uploads/db1493/original/2X/9/90e18468d7209331980ada13465e9b4be7483d0c.jpg" width="660" height="258">
 
To be safe I have measured the voltages on the balance plug. You keep one probe of your multimeter on most left or right balance pin. With the other probe you check if each pin adds up 3,7 volt (voltage is depending on how full the lipo is) starting on the pin adjacent to the pin of your first probe.

If the voltage does not add up like it should then your wiring is not good and you might blow up your chargers balance port.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-08-15T07:24:59.724Z Reads: 64

```
Nice diagram imo
```

---
## \#10 Posted by: Jeefberky Posted at: 2016-08-15T07:40:34.575Z Reads: 59

```
Thanks :grin:
```

---
