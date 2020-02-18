# Charging 10S pack made of Samsung 25r cells

### Replies: 21 Views: 1735

## \#1 Posted by: thisguyhere Posted at: 2016-11-29T22:23:08.721Z Reads: 152

```
i'm in the process of building a 10s4p pack and had a question about charging.

i plan to NOT use a bms initially, and just use a balance charger ([iCharger 1010b+](http://www.icharger.co.nz/Products/1010B-.aspx)).

using this charger i plan to balance charge maybe 1 out of 4 times, but just do a normal charge for the remainder.

the charger has different battery type parameters for "normal" charging, but which would i use for a pack consisting of the Samsung 25r cells?

<img src="/uploads/db1493/original/3X/5/d/5d8ef7ee2d4c242bb3df4a2006a3d872b6b124f3.png" width="690" height="180">
```

---
## \#2 Posted by: Eboostin Posted at: 2016-11-29T22:30:22.709Z Reads: 147

```
You would use the "LiIo" for a Samsung 25R pack. 

"LiIo" = Lithium Ion

Hope that helps. 

You could technically charge them with Lipo setting but by charging to 4.1 instead of 4.2 volts per pack, you will extend the life of the battery.
```

---
## \#3 Posted by: thisguyhere Posted at: 2016-11-29T22:31:12.153Z Reads: 140

```
omg, in the table i read that as LILO, thinking it was some type i wasn't familiar with.

awesome, thanks for the quick response!
```

---
## \#4 Posted by: Eboostin Posted at: 2016-11-29T22:45:18.182Z Reads: 130

```
No problem, the capital "i" threw me for a loop too. haha. Also, the 4.1 max charge voltage is off for the 25Rs. 

You can safely charge them to 4.2v/cell.
```

---
## \#5 Posted by: thisguyhere Posted at: 2016-11-29T23:02:33.220Z Reads: 125

```
then would i just be able to use the LIPO setting?
```

---
## \#6 Posted by: Eboostin Posted at: 2016-11-29T23:29:41.135Z Reads: 117

```
Yes, the Lipo settings are fine
```

---
## \#7 Posted by: thisguyhere Posted at: 2016-11-29T23:47:20.805Z Reads: 114

```
sweet, thank you
```

---
## \#8 Posted by: Namasaki Posted at: 2016-12-01T06:22:59.226Z Reads: 106

```
I would recommend balance charging every cycle not just 1 out of 4.
You could ruin a cell if it gets too out of balance. The risk is not worth the time saved when charging.
Even with balance function, the charge time is quick with a good charger like the one your looking at.
```

---
## \#9 Posted by: Tuomalar Posted at: 2016-12-01T06:46:00.419Z Reads: 102

```
Few guys here tried packs without bms and I will try too, because it should not be problem with quality cells.
```

---
## \#10 Posted by: Maxid Posted at: 2016-12-01T07:01:49.463Z Reads: 98

```
There is basically no risk when using quality cells. You can safely charge without a balancer.
```

---
## \#11 Posted by: Maxid Posted at: 2016-12-01T07:04:14.812Z Reads: 94

```
Charging to 4.2 will ALWAYS result in less life cycles no matter the cell you are using. 4.1 seems like a good tradeoff between life and capacity. This is also valid for Lipos.
```

---
## \#12 Posted by: thisguyhere Posted at: 2016-12-01T07:32:12.936Z Reads: 88

```
[quote="Namasaki, post:8, topic:13924"]
I would recommend balance charging every cycle not just 1 out of 4.
[/quote]

that "1 in 4" charges is something i just pulled out my butt...

plan is to use a balance charger ([iCharge 1010b+](https://www.amazon.com/ProgressiveRC-na-iCharger-1010B/dp/B005X0470G)) so doing a balance charge won't be a problem.

[quote="Maxid, post:11, topic:13924, full:true"]
Charging to 4.2 will ALWAYS result in less life cycles no matter the cell you are using. 4.1 seems like a good tradeoff between life and capacity. This is also valid for Lipos.
[/quote]

good point, go safe to extend the life of the pack.  i'm ok with that even with a bit of a capacity sacrifice.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-12-01T14:48:31.824Z Reads: 76

```
I have seen Lipo cells go out of balance after just one discharge. I prefer to balance my cells on every charge for maximum performance and peace of mind.
```

---
## \#14 Posted by: Eboostin Posted at: 2016-12-01T16:13:40.000Z Reads: 70

```
Yes, I wrote that in the second post in this thread. 

Good practice if the pack is large enough that the user doesn't need thr additional range from the extra .1 or whatever they set their cutoff to.

My cutoff on my 10S6P is 40V and my 10S4P is 41V.
```

---
## \#15 Posted by: Maxid Posted at: 2016-12-01T16:41:13.993Z Reads: 71

```
Lipos are not quality cells.
```

---
## \#16 Posted by: Namasaki Posted at: 2016-12-01T16:45:24.841Z Reads: 69

```
I've tried both Lipo then Li-ion. 
I went back to Lipo because pound for pound 
I got more power and less voltage sag with Lipos. 
60/120C Lipos that is.
```

---
## \#17 Posted by: Maxid Posted at: 2016-12-01T16:50:25.984Z Reads: 69

```
while sacrificing safety and the luxury of not having to use a balancer. There is always a tradeoff. 
Also just because you decided to use Lipos you can't tell people that they need to balance charge when they ask you abut Liion charging.
```

---
## \#18 Posted by: Namasaki Posted at: 2016-12-01T18:48:39.974Z Reads: 62

```
[quote="Maxid, post:17, topic:13924"]
Also just because you decided to use Lipos you can't tell people that they need to balance charge when they ask you abut Liion charging.
[/quote]
I can and will always recommend what I feel is the best option for safety and performance. 
And I feel that any type of lithium battery that is used for esk8 should be balanced.
```

---
## \#19 Posted by: SageTX Posted at: 2016-12-01T19:05:10.738Z Reads: 64

```
Lemme ask something somewhat related...  

If using 3 4s lipos in parallel hooked together on the balance leads too, then these 2 "packs" in series, does this help mitigate the out of balance problem?
```

---
## \#20 Posted by: Eboostin Posted at: 2016-12-01T19:33:23.035Z Reads: 62

```
That is not sound advice. Li-ion should still be balance charged especially by an average to intermediate user. 

You can get away without a BMS as @whitepony has done but I would not go around advocating to skip a BMS if a build has room for one.
```

---
## \#21 Posted by: Namasaki Posted at: 2016-12-02T00:18:52.111Z Reads: 49

```
Sounds like you have an 8s 3p battery pack. 
I don't think putting them in parallel will help them balance. 
I believe that lithium cells discharge and charge unevenly because they are not perfectly matched and their internal resistance varies from one cell to the next
```

---
