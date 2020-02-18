# BMS and ESC protection

### Replies: 13 Views: 629

## \#1 Posted by: D_Sk8 Posted at: 2018-06-13T21:37:39.362Z Reads: 137

```
I am looking to build a dual 6374 build with 100a worth of power (more on that in a bit) and am worried about burning the ESC's out after a few forum posts (given, I don't recall why users ESC's failed, or what type they were using or whether it's actually an issue to be too concerned about).

My concern is burning up the ESC. I'm thinking TORQUE ESC's, which max out at 50a continuous/240a peak.

I am going to run a 12s2p A123 26550 pack. Continous run 100a total, with a peak of 240a. 

At what point should one worry about how much power the ESC's can handle? Should I make 2 separate 12s packs and throw 50a BMS's on them, or would that be overkill. 

I will certainly have a BMS on the pack(s) for balance charging, but not certain whether I should wire directly to the ESC, or do my best to protect the ESCs.

Would Focbox, with the extra 10a of support be a better idea if I am my max continuous is 50a?

VESC6 is out of my price range.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-06-13T22:04:45.147Z Reads: 117

```
The esc will only draw as much current as it needs, so you could set it to 45amps and you won’t draw anymore than that. I would also recommend getting a bms slightly higher amperage than what you will draw otherwise it might cutout during a hill climb
```

---
## \#3 Posted by: Kuchi Posted at: 2018-06-14T00:06:05.228Z Reads: 105

```
Route the bms only for charging and you won’t need to worry about that amp being an issue, the vesc can program low voltage cutoff so over discharge will not be an issue. I would recommend torque boards esc for their motors as they were made simultaneously to work with each other
```

---
## \#4 Posted by: D_Sk8 Posted at: 2018-06-14T00:59:41.795Z Reads: 97

```
Ok, cool. Thank you. I'm getting the impression the VESC should be fine without a BMS. Saves me as a 20a BMS is cheaper anyway :)
```

---
## \#5 Posted by: Zac13 Posted at: 2018-06-14T04:15:55.190Z Reads: 79

```
Don't get a torqueboards vesc.

They have a high failure rate.

Do a bit of research around and you'll see that.  Instead get an ollin or a focbox
```

---
## \#6 Posted by: D_Sk8 Posted at: 2018-06-14T05:01:57.725Z Reads: 70

```
Yeah, that is my concern. Not certain why they are failing though, I just assumed because of high amps?

Ollin VESC don't seem to be available any longer, @chaka are you still making them?  

I swear Focbox was listed at under $140 earlier today, but now it's listed at closer to $180. Not sure if I am trippen or if the price actually went up. I'll need two of them. I'd be willing to risk buying two from Torqueboards if the only other alternative is $180 each.
```

---
## \#7 Posted by: Zac13 Posted at: 2018-06-14T05:16:07.200Z Reads: 64

```
Price went up and they're out of stock :/
```

---
## \#8 Posted by: pat.speed Posted at: 2018-06-14T06:22:50.140Z Reads: 62

```
You just missed enertion’s sale on focboxs, if you need different escs get HK ones, they have a 1 year warranty
```

---
## \#9 Posted by: Zac13 Posted at: 2018-06-14T15:03:21.881Z Reads: 47

```
On the plus side, the focbox unity likely will come out soon and the current model of focbox price is likely to drop /  be on sale all the time
```

---
## \#10 Posted by: D_Sk8 Posted at: 2018-06-14T15:35:38.959Z Reads: 49

```
That would be cool. I'm really hoping to pay no more than $300 for 2 ESC's shipped, if at all possible. 

There's been mention that most VESC failures are due to user error. Since we're dealing with electronics, I imagine heat is a major factor and part of the user error could be that the configuration doesn't keep heat in mind. I'm also guessing attempting to increase cooling might help that, but I'm also guessing that might be difficult while retaining water resistance.
```

---
## \#11 Posted by: DAddYE Posted at: 2018-06-14T16:10:22.711Z Reads: 44

```
Get 2 vesc 6 from flipsky they’re 159$ on rcmoments
```

---
## \#12 Posted by: D_Sk8 Posted at: 2018-06-14T17:14:51.036Z Reads: 40

```
[quote="DAddYE, post:11, topic:58792"]
flipsky
[/quote]

Ohh wow! That looks like a great plan. Is FlipSky a good product overall?
```

---
## \#13 Posted by: DAddYE Posted at: 2018-06-14T19:47:36.809Z Reads: 35

```
It seems so, search here IIRC there are few topics about it
```

---
