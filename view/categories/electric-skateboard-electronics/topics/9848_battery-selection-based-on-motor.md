# Battery Selection based on Motor

### Replies: 33 Views: 2288

## \#1 Posted by: roamin Posted at: 2016-09-19T20:04:59.388Z Reads: 153

```
Hey everyone,
I've gone ahead and purchased enertion's mono drive kit & VESC, along with a turnigy 6364 245 kV motor. I'm trying to figure out the best budget battery configuration: I'd ride a maximum of an hour, and I'm unsure if two 3S batteries in series would be the best bang for buck. (~180 lb. Rider). What's the most effective? Links are welcomed!
```

---
## \#2 Posted by: mason Posted at: 2016-09-19T20:47:53.422Z Reads: 143

```
Max you could go on that is 6s. It would work great
```

---
## \#3 Posted by: roamin Posted at: 2016-09-19T20:52:27.518Z Reads: 137

```
@mason So two Zippy 3S 5000 mAh Lipo's are a good call? Thanks for the help!
```

---
## \#4 Posted by: sl33py Posted at: 2016-09-19T20:57:48.817Z Reads: 138

```
[quote="mason, post:2, topic:9848, full:true"]
Max you could go on that is 6s. It would work great
[/quote]


Um... he can do more than 6s on VESC.  Not sure what's confusing here, but VESC can go 8 or 9s on 245kv motor and stay below the 60k ERPM limit.

I personally - especially for a 180lb rider, would go 8s.  Dual 4s in series.  Boom.  I ride 8s frequently and it works great and i have this rider by 80-90 lbs.  (on the flats no biggie)

Just realize that at 83mm - 245kv - 9s - 15/36 (enertion's usual) - it'll give you a top speed of 31mph.  I might set some rpm limits in the BLDC to avoid that much speed.  or 8s gives you 27mph.
```

---
## \#5 Posted by: chinzw Posted at: 2016-09-19T21:19:06.887Z Reads: 124

```
That motor is MAX 10s
```

---
## \#6 Posted by: roamin Posted at: 2016-09-19T21:43:25.550Z Reads: 110

```
@sl33py I'll give the 8S a try - for charging, would I disconnect its series connection and get a parallel board from hobbyking?
```

---
## \#7 Posted by: mason Posted at: 2016-09-19T21:47:10.339Z Reads: 105

```
My bad, didn't see VESC.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-09-19T21:54:35.389Z Reads: 104

```
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#9 Posted by: roamin Posted at: 2016-09-19T21:55:55.721Z Reads: 98

```
@sl33py I had been looking at the Turnigy 5000 mAh 4S Lipo's, which would you reccomend along with how to charge properly? :sweat_smile:
```

---
## \#10 Posted by: roamin Posted at: 2016-09-19T21:57:57.205Z Reads: 94

```
@Namasaki with 245 kV, based on the chart, the 8S looks fine then(?)
```

---
## \#11 Posted by: Namasaki Posted at: 2016-09-19T22:11:06.257Z Reads: 94

```
245kv X  33.6v X 7=57624 ERPM
So yes, 8s is well under the 60k ERPM limit. 

9s would put you over the limit and your Vesc would be at risk. 
37.8×245×7 = 64827
```

---
## \#12 Posted by: Namasaki Posted at: 2016-09-19T22:16:37.620Z Reads: 88

```
I recomend this charger. It will simultaneously charge 2 5000mah packs in 1 hr or less
Always charge Lipos at 1C or less
That's 5amps for a 5000mah battery

https://www.amazon.com/dp/B00VOYR6MQ/ref=cm_sw_r_cp_api_ulg4xb2QK2JA0
```

---
## \#13 Posted by: roamin Posted at: 2016-09-19T22:22:30.167Z Reads: 88

```
@Namasaki I'm aware that 5000 mA is 5A. I'm looking at getting a charger on a budget unfortunately - anything within the $50 to $60 range(?) That you'd recommend, of course.
```

---
## \#14 Posted by: michaeld33 Posted at: 2016-09-19T22:23:57.768Z Reads: 91

```
https://www.amazon.com/Genuine-SKYRC-Power-6Amps-50Watts/dp/B00ND7J38C

This is pretty similar (mine's a different color and has a different logo) it's 6S 5A, and it's AC powered.
```

---
## \#15 Posted by: Lsalt Posted at: 2016-09-19T23:13:26.781Z Reads: 82

```
Don't use this charger. Michael is wrong lol. Just kidding he offers good advice. :wink:
```

---
## \#16 Posted by: sl33py Posted at: 2016-09-19T23:33:22.237Z Reads: 83

```
Agree w/ Michaeld33 a great starter charger - iMax B6ACv2.  You can go with a higher power one, that requires a dedicated AC->DC power supply like w/ an iCharger, but unless you have a lot of packs charging at the same time, or really big packs - you don't need it.

The B6ACv2 will be slow w/ only 5a output, but they also have some of the better functions like IR (measure internal resistance).
```

---
## \#17 Posted by: sl33py Posted at: 2016-09-19T23:38:55.054Z Reads: 85

```
[quote="roamin, post:6, topic:9848"]
I'll give the 8S a try - for charging, would I disconnect its series connection and get a parallel board from hobbyking?
[/quote]

[quote="roamin, post:9, topic:9848"]
I had been looking at the Turnigy 5000 mAh 4S Lipo's, which would you reccomend along with how to charge properly?
[/quote]


I think 8s will work well for you if you are geared correctly.

Yes disconnect to charge.  most chargers will max out at 6s, so dual 4s is easiest.  Yes you can get a 12s charger if you'd like, but i'd just disconnect, or get BMS.  Issue w/ BMS is i inspect my batteries before charging, so tucked away in board i can't inspect.

I've had good luck with Turnigy, Zippy, and others from HK.  Also a few duds... but that's part of the game for cheap(ish) lipos.  I would look at any of the lipos they sell, check their sizes ( i like "thin" batteries using their C measurement on HK to find thinner packs vs skinny tall packs that stick down lower under board), and target at least 20c (shooting for 100a capability so 5000mAh 20c (20c * 5Ah = 100a)).  More won't hurt, but you spend a premium for 45c+ packs and you likely aren't using the output capability.

GL!
```

---
## \#18 Posted by: Namasaki Posted at: 2016-09-19T23:39:59.398Z Reads: 77

```
On batteries, 
5000mah X 8s = apx 8 mile range. 
I recommend getting Lipos with the highest C rating that you can. 30c ~
You want your batteries to be able to deliver much more current than you need to avoid voltage sag.
```

---
## \#19 Posted by: sl33py Posted at: 2016-09-19T23:41:23.865Z Reads: 78

```
[quote="Namasaki, post:11, topic:9848, full:true"]
245kv X  33.6v X 7=57624 ERPMSo yes, 8s is well under the 60k ERPM limit. 

9s would put you over the limit and your Vesc would be at risk. 37.8×245×7 = 64827
[/quote]

Thanks for this Namasaki!  I usually just plug it into my speed calc spreadsheet to figure speed and ERPM.  This is simple though, so i'll double check.
```

---
## \#20 Posted by: roamin Posted at: 2016-09-20T00:21:50.497Z Reads: 76

```
@Namasaki Awesome!!! Thank you for the advise - I'll purchase the 4S batteries. When it comes to charging, will they need to be balanced? How would I go about solving that with the B6ACv2 charger if I can only do a single battery at a time?
```

---
## \#21 Posted by: Namasaki Posted at: 2016-09-20T00:31:28.226Z Reads: 72

```
[quote="roamin, post:20, topic:9848"]
When it comes to charging, will they need to be balanced? How would I go about solving that with the B6ACv2 charger if I can only do a single battery at a time?
[/quote]

You should always balance charge every time. You will have to charge your packs one at a time with that charger.
Parallel charging is possible but requires extra care and is not optimal. And I would not recommend parallel charging Lipos.
```

---
## \#22 Posted by: roamin Posted at: 2016-09-20T00:42:44.888Z Reads: 71

```
@Namasaki will do - I'll charge one at a time, and then check the charge on each to make sure they're at the approximately the same level? Very new to everything, thank you for bearing with me :slight_smile:
```

---
## \#23 Posted by: Namasaki Posted at: 2016-09-20T00:59:33.204Z Reads: 71

```
read charger instructions thoroughly. You will need to set balance charge limits. 
End Voltage: no more than 4.2v for full charge. 4.0v is recommended by some for battery longevity.
(another key to Lipo longevity is never discharge them below 3.4v per cel)
Mah cut off should be set to match your battery's capacity i.e.: 5000mah
Then the charger will automatically balance charge your battery to full and stop.
Still, when charging Lipos, always monitor them. Never put them on charge and go to bed or leave the house.
Best to get a Lipo fire safe bag to put them in when charging and when storing them.
https://www.amazon.com/Teenitor-Fireproof-Explosionproof-Battery-Storage/dp/B00Z8WG11W/ref=sr_1_7?ie=UTF8&qid=1474333079&sr=8-7&keywords=lipo+fireproof+bag
```

---
## \#24 Posted by: roamin Posted at: 2016-09-20T01:35:34.470Z Reads: 66

```
@Namasaki thank you!!! it looks like hobby king is out of the 5000 mAh 4S Lipo's, but I'll check in a couple days and buy them - thank you so much for the help!!! Also getting some XT-90 anti spark plugs for the positive line. Should be a fantastic build! Love this community's support.
```

---
## \#25 Posted by: popopopop Posted at: 2016-09-20T01:49:44.596Z Reads: 59

```
Which one are you looking at? I see a few 5A 4S in stock.
```

---
## \#26 Posted by: roamin Posted at: 2016-09-20T01:51:56.266Z Reads: 59

```
It looked like they had been on back order @popopopop Do you have a link?
```

---
## \#27 Posted by: popopopop Posted at: 2016-09-20T02:03:10.086Z Reads: 59

```
I think you were looking at the 30c batteries which are on backorder. 

http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=58983
http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=58763
```

---
## \#28 Posted by: michaeld33 Posted at: 2016-09-20T02:17:46.219Z Reads: 53

```
:stuck_out_tongue:
1010100101
```

---
## \#29 Posted by: Namasaki Posted at: 2016-09-20T02:45:07.266Z Reads: 57

```
You have to try different warehouses.
Also very important:
Don't go to their site and buy right off. Sit there and look at the battery you want until they pop up a window offering you an extra discount.
They almost always do.
Tip 2: Set up your login account with them before ordering anything and always log in before ordering.
I tried to order as a guest one time and it was a mess! I couldn't track my order and they couldn't track it either!!!
Also, 25C is good, 125a continuous discharge. But if you can afford to get batteries with higher discharge, higher is better.
Higher C rated batteries will suffer less voltage sag and will tend to have lower internal resistance making them more efficient and less prone to heating up.
```

---
## \#30 Posted by: treenutter Posted at: 2016-09-20T03:16:20.742Z Reads: 55

```
@roamin 8S with that motor and VESC works perfectly. I use this exact config.
```

---
## \#31 Posted by: roamin Posted at: 2016-09-20T05:53:35.345Z Reads: 49

```
@treenutter What's your config like for the BLDC Tool?
```

---
## \#32 Posted by: TarzanHBK Posted at: 2016-09-20T08:00:56.938Z Reads: 47

```
also it takes the same time charging both batterys with a parallel board or just one at a time.
so much better to charge one and monitor your battery with correct balance charging :slight_smile: 
8s on 245kv with vesc will put you some crazy smiles on your face, also it will run really efficiant.
have fun bro :monkey:
```

---
## \#33 Posted by: Pablo_702 Posted at: 2016-09-21T00:11:01.581Z Reads: 44

```
Check out miami boards hes got a really nice 18650 battery pack for a really good price
```

---
