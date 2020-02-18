# Using a BMS on a 8s1p 8000mah Lipo

### Replies: 17 Views: 3749

## \#1 Posted by: gaetjen Posted at: 2016-06-12T11:34:21.554Z Reads: 271

```
Hey there,
I bought two Zippy 4s with 8000mah and I want to connect them in series, so that I have a 8s battery with 8000mah. The problem is that chargers for 8s are really expensive, so for convenience and money reasons I'm planing on using a BMS with 60A. I was thinking about this one 
http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html
Is 60A enough? Because I've read mixture opinions about it.
In addtion I want to then get a charger like this
http://www.ebay.com/itm/321471399664?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
Any ideas if this setup would work? 
I have a VESC from a enertion and a SK3 - 6364-245kv Brushless Motor.
I also found this 8s charger on ebay. 
http://www.ebay.de/itm/HK-ECO8-150W-7A-8S-Bal-Dis-Cyc-Charger-Ladegeraet-w-acc-/151728079796?_trksid=p2141725.m3641.l6368
Would this be an easier solution than having to build in a BMS into the board?
I'm thankful for any help :slight_smile:
```

---
## \#2 Posted by: Nordle Posted at: 2016-06-12T11:57:46.488Z Reads: 261

```
BMS solution is more elegant, but with the hobbycharger you can charge other batterys too.
Both works , the decision is yours.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-06-12T12:41:53.444Z Reads: 240

```
You could get a dual bank charger for about $120
Then you can charge both batteries at the same time separately. They'll charge a lot faster and you won't have the current limitation of a BMS. 

UP120AC Duo Dual 2 Port (2x 12Amps, 2x 120Watts, 240Watts Total): LiPo, LiHV, LiIon, LiFe, NiCd, NiMh, Pb AC/DC Balancing Battery Multi-Chemistry Multicharger with 300Watt Power Supply https://www.amazon.com/dp/B00SZ1CBVC/ref=cm_sw_r_cp_api_YHvxxbK57G9W1
```

---
## \#5 Posted by: ArmandR Posted at: 2016-06-12T12:43:20.598Z Reads: 228

```
How does the charger hold up? Is it resistant? Or should I go for Icharger 208b?
```

---
## \#6 Posted by: Namasaki Posted at: 2016-06-12T12:45:50.647Z Reads: 216

```
I've been using mine for 6 months with no problems. 
It fully charges my 5000mah packs in 1hr at 5amps
```

---
## \#7 Posted by: gaetjen Posted at: 2016-06-12T12:51:00.167Z Reads: 199

```
Is the current limitation of a BMS a Problem. Should I go then with a 80A BMS?
```

---
## \#8 Posted by: ArmandR Posted at: 2016-06-12T13:12:44.538Z Reads: 192

```
Go with what your esc can do because then getting an expensive esc doesn't make sense. If the BMS is 60 amps and you buy a 120 amp esc you can only use those 60 amps.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-06-12T14:19:11.459Z Reads: 186

```
Usually a BMS rated at 60amps is 60amp peak and only 30amp continuous. 
An 80amp BMS should handle 40 amp continuous. 
I would recommend getting a 100 amp BMS or at least 80amp. 
And at least a 4 amp charger. 
A 2 amp charger will likely take 4 hours to fully charge your batteries. 
Normally a BMS is not used with Lipos. 
Only with lithium-ion batteries
```

---
## \#10 Posted by: jrpwit Posted at: 2016-06-12T14:56:41.006Z Reads: 175

```
I use a bms on my lipos and it works great! I wanted it to be this way because it would solve the problem of me having to remove the batteries every time I want to charge them on a balance charger. I also use one of those really expensive chargers cause it charges the batteries a lot faster but I am considering getting a 5 amp laptop charger to charge my board on the go (which is another benefit to having a bms). Anyways when I first started doing my build with the bms someon on the forum gave me this very helpful diagram of how the lipos from hobby stores are assembled. The battery in the diagram is a 3s battery.<img src="/uploads/db1493/original/2X/c/c3440a1c26fd938d955190679f9d7990f12026f8.jpg" width="640" height="480">
Anyways hope this helps you out. Also here is the links to my bms I used and charger.
bms: http://www.batterysupports.com/44v-48v-504v-12s-100a-12x36v-lithium-ion-lipolymer-battery-bms-p-393.html
charger: http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html
```

---
## \#11 Posted by: gaetjen Posted at: 2016-06-12T14:57:25.722Z Reads: 159

```
@Namasaki  Would you then suggest to just the balance charger from HK or why is it no so common?
```

---
## \#12 Posted by: gaetjen Posted at: 2016-06-12T15:04:00.161Z Reads: 153

```
@jrpwit  You are using a 30A. Do you have any Problems going uphill because it seems a bit low?
```

---
## \#13 Posted by: jrpwit Posted at: 2016-06-12T15:19:34.417Z Reads: 156

```
Oops sorry that was the wrong bms. Here is the correct link to the bms: http://www.batterysupports.com/44v-48v-504v-12s-100a-12x36v-lithium-ion-lipolymer-battery-bms-p-393.html (I will also change the incorrect link)
 
Anyways Im using four 3s 5000 mah zippy lipos from hobbyking (but I recommend turnigy lipo batteries) in series for a 12s battery. So that is 100 amp max if my calculations are correct. Usually on any board you will not go over 60 amp no matter what hill you are going up. Also I have a 50 amp blade fuse between my vesc and batteries so there is no chance I will go over 50 amps. I have yet to blow the fuse so I not going over 50 amps. Also I should mention that I live in a very flat area so I dont pull to many amps anyways. It is also important to always to over spec your components you use on your board improving how long them last. 

In conclusion, go for the 100 amp bms.
```

---
## \#14 Posted by: Namasaki Posted at: 2016-06-12T15:31:17.085Z Reads: 146

```
It's just not necessary to use a BMS with Lipo packs. 
You'd be adding extra circuitry for the current to go through. Creating more potential for failure under heavy load situations. And extending your charge time from 1 hour to 4 hours.
```

---
## \#15 Posted by: Bender Posted at: 2016-06-12T16:31:33.540Z Reads: 140

```
I'd love to not have a BMS, but I too am sick of constantly having to deal with removing and charging 4 lipo packs. (3s x 4 for 12s)
Do you have any other suggestions for simple ways to charge them without having to constantly remove and charge 4 packs?

I'm thinking of at least making them into 2 6s so I'll only have 2 to deal with
Or even 1 12s but do they make a charger that accepts a 12s (13 pin jxt) lead?
```

---
## \#16 Posted by: Namasaki Posted at: 2016-06-12T17:49:11.106Z Reads: 131

```
Any balance charger that charges over 6s is gonna be pricey. 
You could use a 4 bank charger. 
The thing with Lipos is that there just not the most convenient option. But they deliver the most power and charging is very fast.
```

---
## \#17 Posted by: Namasaki Posted at: 2016-06-12T18:15:46.592Z Reads: 128

```
 If you're already using a BMS  and it's working for you,  why change it?
```

---
## \#18 Posted by: Namasaki Posted at: 2016-06-12T18:20:30.339Z Reads: 127

```
[quote="Bender, post:15, topic:4593"]
Do you have any other suggestions for simple ways to charge them without having to constantly remove and charge 4 packs?
[/quote]
Using a BMS is probably the best option if your priority is to make charging simple and convenient
```

---
