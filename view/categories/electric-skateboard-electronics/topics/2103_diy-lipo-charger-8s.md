# DIY LiPo charger 8s

### Replies: 13 Views: 3203

## \#1 Posted by: makepeace Posted at: 2016-04-01T07:57:07.904Z Reads: 210

```
Hey guys,

Just wondering if anyone has any design resources or advice on a circuit or a direction to go in in terms of designing one to balance charge an 8s LiPo pack at high current (say 10A or so)? I've looked on the internet and there don't seem to be any obvious answers.

Any ideas would be appreciated.

Thanks!

P.S. I'm not looking for alternative suggestions or for any discouragement on this idea. I know that it's probably cheaper/easier to buy an off the shelf solution. That's not the point here.

Edited to change a ridiculous calc error.
```

---
## \#2 Posted by: lox897 Posted at: 2016-04-01T09:18:19.610Z Reads: 205

```
Charging lipos at 60 amp? What lipos do you have? That's crazy!
```

---
## \#3 Posted by: makepeace Posted at: 2016-04-01T09:33:15.832Z Reads: 204

```
Oh, wait. Sorry, my mistake. I am charging my pack in parallel at the moment, so that was what I was going for if I was charging at 4.2 V.

Call it 10 A, for an 8s pack balance charge. That makes more sense. :)
```

---
## \#4 Posted by: Namasaki Posted at: 2016-04-01T17:19:11.151Z Reads: 195

```
Your description is not totally clear but if your running 2 4s packs in parallel, there 4s not 8s. 
If your running them in series, there 8s. 
Either way, it's best to charge them separately with a dual bank charger. 
Parallel charging is possible but not recommended. 
And you should not charge at 10a unless your packs have a capacity of 10,000 mah each. 
It's safest to charge at 1c
```

---
## \#5 Posted by: makepeace Posted at: 2016-04-01T18:00:36.300Z Reads: 195

```
Thanks for your comment.

My pack is an 8s pack made from single 5.8 Ah cells. I am going for 10 Ah next time around, but 1.66C is fine for charging my current pack.

Being on a tight budget, I am currently charging all 8 cells in parallel at 6 A 4.2 V with an iMax B6, and have made seperate connector plugs out of perspex for the battery, charger and esc. Despite it being a lot more convenient than most solutions I've seen so far, it's still not easy enough for my tastes. Unplugging a 16 point 5.5 mm bullet connector plug is no mean feat.

My design aim for this charger is to build an all in 1 no fuss charger specifically for my cell count and charge current that I can just plug into my board and that is that.
```

---
## \#6 Posted by: psychotiller Posted at: 2016-04-01T20:10:37.315Z Reads: 180

```
Just buy one of these:
http://www.ebay.com/itm/321471399664?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

And one of these:
http://www.amazon.com/5-5mm-2-1mm-Female-Connector-Camera/dp/B005CMP434?ie=UTF8&psc=1&redirect=true&ref_=oh_aui_detailpage_o01_s00
 
I'm using this setup on my 10s4p Li-ion Build (with a 10s version) and on a new build with 8s lipo. Working great so far. I will check cells periodically, and replace if needed.
```

---
## \#7 Posted by: makepeace Posted at: 2016-04-02T07:20:32.621Z Reads: 153

```
Thanks for the tip. Could you explain how this balance charges the pack? Not entirely sure what the intention is in terms of how to implement this setup.
```

---
## \#8 Posted by: willpark16 Posted at: 2016-04-15T00:22:50.529Z Reads: 141

```
if u still are looking for a charger i have an 8s capable 7a charger that can do basically any chemistry
```

---
## \#9 Posted by: claudiofiore88 Posted at: 2016-04-15T02:35:31.434Z Reads: 136

```
Just out of curiosity, what charger do you have.?The only ones I've seen only do up to 6s.
```

---
## \#10 Posted by: willpark16 Posted at: 2016-04-15T03:48:05.945Z Reads: 131

```
the turnigy accucell 8 7a charger
```

---
## \#11 Posted by: claudiofiore88 Posted at: 2016-04-15T03:53:34.660Z Reads: 130

```
Oh, nice.  I've had my iMAX B6AC V2 for a couple weeks now.  The quality is quite good.  It has a lot of features that my Onxy 235 charger doesn't have like being able to discharge and goes up to 6s vs 4s on the 235 at half the cost, so I'm quite happy with my purchase.
```

---
## \#12 Posted by: willpark16 Posted at: 2016-04-15T03:55:46.580Z Reads: 127

```
heard a lot of good things about that charger especially its features however the one i have came as a steal.
```

---
## \#13 Posted by: makepeace Posted at: 2016-04-15T20:29:10.188Z Reads: 121

```
Thanks for the heads up. I'm going to buy an 8s BMS 10 A (charge) and a power supply and box those to use as a charger. Seems the best (cheapest, fastest, easiest) option to me. Case closed, from my side. :wink:
```

---
