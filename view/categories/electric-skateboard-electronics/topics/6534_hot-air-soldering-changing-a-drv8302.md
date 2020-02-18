# Hot Air Soldering - changing a DRV8302

### Replies: 18 Views: 1934

## \#1 Posted by: whitepony Posted at: 2016-07-23T18:57:22.785Z Reads: 195

```
hey guys,

seems one of the new enertion vescs arrived with a DRV8302 fault and Im not sure how jason will be able to support me here in germany, so I was thinking: why not buy a cheap hot air soldering station and try to fix it yourself (assuming that its back in order with replacing or resoldering the drv8302 chip)? seems you get the cheap ones for just 50€ and a drv8302 swap from a german vesc support guy http://www.lp-electronic.com/vesc/ costs already about 60€, so might actually be the cheapest solution which also enables me to do resolve some PCB issues on my own.

now question to the pros: hot air soldering stations for 50€ - do you think Ill be able to actually swap a drv8302 with that? example: https://www.amazon.de/dp/B007H1U1YK/ref=cm_sw_em_r_mt_dp_z07KxbKZ5E802
```

---
## \#2 Posted by: MasterCho Posted at: 2016-07-23T19:09:32.679Z Reads: 210

```
I saw your post earlier that concerns me little since I placed an order of 4  from Enertion 3weeks ago. 

This is going to help me a lot if I get faulty one.
```

---
## \#3 Posted by: treenutter Posted at: 2016-07-23T22:48:03.399Z Reads: 192

```
@whitepony I had the same issue and also chose to buy q reflow station instead of paying someone else to do it. About midway through the thread below is a lot of advice from folks here on the forum. 

 http://www.electric-skateboard.builders/t/vesc-drv8302-failures-and-repair-options/4201
```

---
## \#4 Posted by: KMeyerson Posted at: 2016-07-24T07:28:44.224Z Reads: 168

```
I finally hooked mine up and found that one of them was DOA (Order #333X)

One worked fine, but the other one in parallel did not. I tried it on a 12V PSU pin just to see if I could power up the LEDs, but still nothing.  When I plugged it directly into my battery, it sparked (Yay for continuity!) but no power. Looks like I'll have to sit on my hands a little longer.
```

---
## \#5 Posted by: whitepony Posted at: 2016-07-24T07:35:03.791Z Reads: 160

```
@treenutter thx for the link! 

@KMeyerson awh, that sucks, but hard to explain a fully dead vesc - from what I know they flash the latest firmware and some rspec settings - so it probably shouldve worked that far.

my vesc powers up, I can connect with the gui, but dev8302 errors prevents any motor commutation - thought that this could actually slip quality control if they dont actually test the vescs with motors attached ... cause everything else works fine.
```

---
## \#6 Posted by: KMeyerson Posted at: 2016-07-24T07:38:49.239Z Reads: 150

```
They certainly do that at the factory and it's odd. They were plugged in parallel, so user error should have killed both but only one ever had lit LEDs.  Bullets had heat shrink and were connected to motors, so they didn't short either. I'm not going to take matters into my own hands at this point - I can wait for an RMA.

VESCs made in AUS at the Enertion HQ get tested, I'm not sure if they test them in the USA factory/Warehouse.
```

---
## \#7 Posted by: lox897 Posted at: 2016-07-24T07:48:29.564Z Reads: 138

```
All the Enertion VESCs are made in USA.
```

---
## \#8 Posted by: KMeyerson Posted at: 2016-07-24T07:49:27.662Z Reads: 136

```
But do they get shipped to AUS for programming and testing (as seen in videos) or do they go directly from programming to shipping?
```

---
## \#9 Posted by: lox897 Posted at: 2016-07-24T07:50:53.136Z Reads: 134

```
They all got shipped to Aus and then some back to US dealer (longhairedboy) they all get programmed in Aus AFAIK
```

---
## \#10 Posted by: KMeyerson Posted at: 2016-07-24T07:59:01.027Z Reads: 133

```
Ahha - you learn something new every day. I feel like I remember someone discussing in-factory flashing, but that could just as easily be from one of a dozen other things I've been working on.

With the exception of serious burn outs, most damaged VESCs probably don't require significant repairs.  The combined time spent on diagnostics and repair is considerable though unless its a common issue (like DRV8302).
```

---
## \#11 Posted by: Jinra Posted at: 2016-07-24T08:03:35.960Z Reads: 125

```
US orders get VESCs straight from the Texas factory. They don't go to AUS first.
```

---
## \#12 Posted by: KMeyerson Posted at: 2016-07-24T08:15:19.530Z Reads: 124

```
Figured that was the case, import/export would be expensive and messy.
```

---
## \#13 Posted by: lox897 Posted at: 2016-07-24T08:19:12.079Z Reads: 119

```
From now on, but the last batch came to Aus and then back. Not 100% sure but maybe @onloop can confirm for us.
```

---
## \#14 Posted by: Jinra Posted at: 2016-07-24T08:30:59.889Z Reads: 120

```
He confirmed it in another thread when we were talking about why some VESCs got 50v caps. You're right though, earlier batches had the VESCs shipped from US -> AUS -> US. Going forward it seems all US orders have it shipped straight from Texas.
```

---
## \#15 Posted by: KMeyerson Posted at: 2016-07-24T08:32:31.749Z Reads: 118

```
So USA ones might not be getting the full testing treatment.  They're still ironing out the kinks, so lets see what happens.
```

---
## \#16 Posted by: Nordle Posted at: 2016-07-24T10:02:39.322Z Reads: 114

```
but whitepony is in germany
```

---
## \#17 Posted by: whitepony Posted at: 2016-07-24T15:30:14.731Z Reads: 104

```
[quote="KMeyerson, post:6, topic:6534"]
VESCs made in AUS at the Enertion HQ get tested, I'm not sure if they test them in the USA factory/Warehouse.
[/quote]

what does "tested" mean though? the german repair guy also send me a "repaired & tested" vesc once, that actually had instant DRV8302 error on my bench. he just resoldered the DRV8302 chip (didnt swap it) and everything was fine from there!

p.s.: and yea, got mine directly from australia.
```

---
## \#18 Posted by: KMeyerson Posted at: 2016-07-24T15:52:23.730Z Reads: 102

```
In AUS, they're flashed and then used to spin up a motor to prove they're functioning.  See the Enertion Vlog about their new automated mass flasher.
```

---
