# 10S lipo 40km/h Small Board Build

### Replies: 17 Views: 2906

## \#1 Posted by: Ben Posted at: 2016-01-20T03:43:39.758Z Reads: 237

```
Hello,

Im just a neebie so still learning. I had an electric bike for about a year which was great to commute to uni but a friend gave it away to lifeline so I need a replacement. It was a 1kw hub motor kit and got me to uni in about 10 mins (6km)  So averaging around 36km/h i think. 
I would like to build a skateboard to try and get a similar speed and travel time. From what ive been reading I would probably need a 12S setup. However, I came across this slimmer 10S battery and I would love to try use my cnc to build 2 or 3 of these batteries into the deck.
http://hobbyking.com.au/hobbyking/store/__37299__ZIPPY_Compact_4000mAh_10S_25C_Long_Lipo_Pack_AU_Warehouse_.html

I cant decide whether to go with the 190kv motor from enertion or the much cheaper Turnigy Aerodrive SK3 - 5065-236kv motor. 
http://hobbyking.com.au/hobbyking/store/__37598__Turnigy_Aerodrive_SK3_5065_236kv_Brushless_Outrunner_Motor_AU_Warehouse_.html

I think the best option will be to go with a VESC from enertion too along with the motor pulley and belt. I think the gt2b controller sounds like the way to go however doesn't seem to be easily available in Australia.

I plan on just making my own deck or hacking up a cheap one and using my cnc to make the large pulley and motor bracket. 

My main question is if anyone can share some information on the best way to charge a 10S lipo. I really dont want to buy a crazy expensive charger so I'm guessing building my own would be the cheapest option. I know I could get two 5S lipos and connect them up in series to get 10S and then charge them in parallel with a cheaper charger but I would prefer to minimise wiring and like the idea of using 2 or 3 - 10S slim batteries in parallel.  Could anyone point me in the right direction as to if it is possible to get a charger for such a setup on a budget (sub $100aud)? 

Many thanks :smile:
```

---
## \#2 Posted by: cmatson Posted at: 2016-01-20T04:05:31.311Z Reads: 225

```
The 5065 will be very under powered, and I would never recommend a single motor that small: I think it's something you'd regret down the rode. 

I'd either got with a 63mm turnigy for $80, or bump up to the enertion R-Spec for $100. (I'm referring to prices in usd because that's all I know: sorry if that causes any confusion) 

Also, I know people have CNC'd the wheel pulley, but has anyone done a motor pulley? My one recommendation is to make sure their is a ring around the edge of the motor pulley to keep the belt from becoming off centered. 

For the batteries and charging, you could always just go with two 6s packs in series to get your 12s voltage goal. 6s packs are easy to charge with any standard balance charger, and I'm sure you could find one for less than 100aud. 

Hope this helps :smile:
```

---
## \#3 Posted by: lox897 Posted at: 2016-01-20T04:26:07.522Z Reads: 211

```
GT2B from HobbyWarehouse in Australia and an IMAX B6AC V2 is around $110 AUD I believe. Where are you in Australia?
```

---
## \#4 Posted by: Ben Posted at: 2016-01-20T04:36:35.135Z Reads: 214

```
This is the only thing Ive seen thats similar to a small pulley like would be used on the motor. 
https://www.youtube.com/watch?v=oPJYVJg43dY
Not worth the time to machine as they are so cheap anyway imo. 

I'll stick with the R-Spec motor then. 

I know 2 x 10Ah 6S batteries in series would be the easiest option but Id love to use those skinny 10S batteries. but if its going to cost be $200 for a charger, I would be better off getting a space cell.

Cheers
```

---
## \#5 Posted by: Ben Posted at: 2016-01-20T04:37:09.568Z Reads: 208

```
Im in Brisbane :sunny: and thanks, just wasn't looking hard enough for the gt2b.
```

---
## \#6 Posted by: cmatson Posted at: 2016-01-20T04:56:02.390Z Reads: 205

```
You could always buy an R-Spec and then just add an enertion motor pulley to your cart.

I'd have a keyway, and would definitely be the easiest option. 

Haha I also agree with you on those sweet flat 10s packs, but charging would be a hassle. You could buy four 3s packs, and wire them all in series to give you a flat enclosure (you could charge them in two groups with each group acting as a 6s) but that is a lot of wiring just to get a thinner profile....

In the end it's really up to you, but I am going to recommend the 2x 6s option as the cheapest, easiest, and simplest solution (besides a space cell of cources, but I understand that's out of your budget :wink:)
```

---
## \#7 Posted by: Ben Posted at: 2016-01-20T05:03:44.734Z Reads: 200

```
Yeah ill just buy the motor pulley and belt through enertion.

This seems a little sketchy but an interesting idea. What do you think? <img src="/uploads/db1493/original/2X/d/de149ce26935d159b3928d55074cd04099b67c35.png" width="690" height="127">

https://endless-sphere.com/forums/viewtopic.php?f=35&t=73931
```

---
## \#8 Posted by: chaka Posted at: 2016-01-20T05:20:16.642Z Reads: 184

```
Did someone say sketchy? ;)

I only recommend doing this with a really out of balance pack. Way too tedious to do regularly.
```

---
## \#9 Posted by: Ben Posted at: 2016-01-20T05:35:25.525Z Reads: 186

```
I dont really understand how you found that so quick. What is tedious about about it? Sorry if I ask basic questions, I still know nothing.
```

---
## \#10 Posted by: lox897 Posted at: 2016-01-20T06:08:29.351Z Reads: 176

```
The IMAX B6ACV2 is $110 AUD
```

---
## \#11 Posted by: lox897 Posted at: 2016-01-20T06:08:47.177Z Reads: 172

```
But it can only go up to 6s
```

---
## \#12 Posted by: chaka Posted at: 2016-01-20T06:40:02.185Z Reads: 173

```
I guess I am just spoiled. I use a bms with a dedicated charger. No setting or buttons, just plug it in and walk away.
```

---
## \#13 Posted by: Ben Posted at: 2016-01-21T03:02:21.263Z Reads: 167

```
So is it possible to get a bms and wire it to a couple of those 10S lipos in parallel?
```

---
## \#14 Posted by: torqueboards Posted at: 2016-01-21T03:58:59.787Z Reads: 167

```
You could set that up for 10s lipos but a nice benefit for lipos is the swap of lipos. If you end up using a BMS using 18650’s is a better idea.
```

---
## \#15 Posted by: Ben Posted at: 2016-01-27T22:40:46.340Z Reads: 163

```
I think I might bite the bullet and just get a space cell. 

Is there any reason why I shouldn't get these?

http://m.ebay.com/itm/191282982361?_mwBanner=1

http://m.ebay.com/itm/301432673340?_mwBanner=1
```

---
## \#16 Posted by: psychotiller Posted at: 2016-01-28T00:25:57.435Z Reads: 156

```
You'd just have to make sure you're wheel pulley has the XL profile.
```

---
## \#17 Posted by: lowGuido Posted at: 2016-01-29T02:35:49.905Z Reads: 146

```
the XL belts do not have as much holding torque as the HTD belts, but they will work. especially if you put an idler or 2 in there.
```

---
