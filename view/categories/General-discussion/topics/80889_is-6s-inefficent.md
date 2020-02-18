# Is 6s inefficent?

### Replies: 13 Views: 297

## \#1 Posted by: AdamE3399 Posted at: 2019-01-14T22:16:38.727Z Reads: 152

```
Is it just me or is 6s inefficient? So far I have built three boards, two of which were 10s and the other 12s, all relatively powerful boards though they don't get any amazing range due to their 5 amp hour batteries. Though I never though that using a voltage as low as 6s was ever possible until I recently saw builds using it and achieving the same top speeds as some 12s boards and it is now my belief that if you pair 6s with a high kv motor, you loose torque but can achieve similar top speeds? (correct me if I am wrong). So with this in mind I wanted to create a board for range, something like dual 6355 using 6s with graphene lipos to achieve a long cycle life and use 12 ah cells so that I could travel long distances but the esk8 calculator I have used shows that using 6s with a 320kv which reaches 54kmh top speed only has an estimated range of 11km! which is nothing compared to my 5ah packs on 12s which get nearly 20km. So why is this?
```

---
## \#2 Posted by: AlexBE Posted at: 2019-01-14T22:22:59.146Z Reads: 148

```
Don't compare batteries using Ah, you have to use Wh for range calculations.
```

---
## \#3 Posted by: linsus Posted at: 2019-01-14T22:35:55.910Z Reads: 143

```
You dont gain range by dropping voltage. Dropping voltage would mean you'd have to draw more current to achive the same amount of active power. Current has a square relation to losses meaning drawing more current produces more heat. While a higher voltage system runs cooler. Sure theorethically you could run at 1S. But the current draw and losses would be huge.

As @AlexBE said Wh is a better estimate
```

---
## \#4 Posted by: wafflejock Posted at: 2019-01-14T22:37:23.037Z Reads: 135

```
Exactly as AlexBE says, Ah is one half of the equation when it comes to "power" with electricity.  Really power is measured in Watts and is voltage multiplied by amperage, if you reduce cell count in series you reduce voltage so you need more amps to get the same watts (power, which translates into torque/acceleration).  The amount of Watts you use over a given time (amps times volts, times time) is Watt hours and is a measure of power used for a given duration and will give you a better idea of actual range (use 1 Watt for 1 Hour is 1Wh if you use 2W for 1 hr it is 2Wh).

If two systems both require say 400W to power a motor and you have a 40V battery then you need 10A current to be flowing to deliver the 400W, with a 20V battery you would need 20A to deliver the same 400W and since heat loss is related to the square of amperage the increased amperage means more power lost as heat and overall a less "efficient" system (less power going into the end goal of move you forward more going into heat).  That said you can have a system using higher amperage but with so much larger Watt-hour capacity that it can still run for longer.
```

---
## \#5 Posted by: AdamE3399 Posted at: 2019-01-14T22:40:28.156Z Reads: 113

```
Ok I understand thanks for the responses, do you think it would be better than to run 8s or just stick with 10s?
```

---
## \#6 Posted by: linsus Posted at: 2019-01-14T22:41:42.320Z Reads: 107

```
10s all day
```

---
## \#7 Posted by: wafflejock Posted at: 2019-01-14T22:42:31.469Z Reads: 105

```
I'd say stick with 10S if it's not a space constraint or you don't just want to reduce max top speed (really you can just do that and amp adjustment in VESC/FocBox assuming you're using that type of speed controller)
```

---
## \#8 Posted by: AdamE3399 Posted at: 2019-01-14T22:42:54.695Z Reads: 103

```
[quote="wafflejock, post:7, topic:80889"]
t’s not a space constraint or you don’t just want to reduce max top speed (really you can just do that and amp adjustment in VESC/FocB
[/quote]

ok I will cheers
```

---
## \#9 Posted by: Riako Posted at: 2019-01-14T23:29:16.346Z Reads: 85

```
6s are killer !! Its all about the rider !
We saw that this summer in France, at Monségur, for WheelGames.
E-Ride Earth Team are mainly (most of them) on 6s, and they was the leader team of the off road race.
Also they ride hardly in team every time they can.

A lot of DIY and I,  on ESK8FR was inspressed by the capacity of the 6s board, in fact during the ride, there just a rider on his board, and you couldn't say witch is 10s, 6s, 12s, 8s ... (except by the esc/vesc noize ^^).

https://monlongboardelectrique.files.wordpress.com/2018/08/img-20180613-wa0053.jpg
```

---
## \#10 Posted by: monsterbuilder Posted at: 2019-01-14T23:30:27.030Z Reads: 81

```
I was able to hit 25mph very consistently with a single 260kv motor on a 6s lipo.  Was able to get about 18 miles of range (full throttle the whole time) on 13,000 mAh battery.  Was a solid setup other than not being able to go up steep hills and a hot motor if I road in temps above 90'.

That said, I'm switching over to a 190kv motor and 10s this winter.  I want a tad more speed and cooler motor operating temp.

PS I weigh ~150 lbs (without gear)
```

---
## \#11 Posted by: AdamE3399 Posted at: 2019-01-15T02:04:20.345Z Reads: 66

```
Oh that's reassuring to hear but I think I might just go with 8s as a middle ground for my high range board
```

---
## \#12 Posted by: AlexBE Posted at: 2019-01-15T05:51:11.585Z Reads: 54

```
Not sure what you mean by a middle ground. It's worse in every way than a higher voltage. The only time it makes sense is if you are stuck with a high kv motor or high gearing.
```

---
## \#13 Posted by: MoeStooge Posted at: 2019-01-15T13:28:42.475Z Reads: 46

```
Even after all the current improvements to the vesc, I haven't found any power or performance advantages other than dead stop take-off.  Inrunner motors are inherently more efficient by design. Still waiting for a vesc that can handle the e-rpm limits and amp capabilities of the smaller more powerful high kv Inrunner motors. Till it all comes together I will take 8s as it offers the most powerful reliable and heat free drive system per dollar for what I enjoy, going fast without drive system failures.
```

---
