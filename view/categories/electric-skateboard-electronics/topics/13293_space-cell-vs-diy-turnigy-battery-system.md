# SPACE Cell vs. DIY Turnigy Battery System

### Replies: 13 Views: 1232

## \#1 Posted by: Esrapp21 Posted at: 2016-11-18T23:56:09.131Z Reads: 197

```
I have recently been considering different Battery system, and was drawn away from the SPACE cell Battery from enertion due to the price. But once I saw everything needed for a Diy system, I realized the prices were actually pretty close. Now I think I'm going to go with the SPACE cell. I made a chart to help me and anyone else in this situation. On the DIY side, I used 2 of this Battery: https://hobbyking.com/en_us/turnigy-nano-tech-6000mah-6s-25-50c-lipo-pack.html and the extra price is BMS, switch, charger, voltage meter, series connector, and about 10% extra to account for maintenance that may have to do with BMS malfunctions, battery damage, etc. The reason I didn't add this to the SPACE Cell was because it all is built into the Battery and comes from one place, so a return/refund/maintence will not take as long or be as expensive as pieces from hobbyking, which can have parts from around the world. Also, the calculations are just estimates from calculators and I have not done any physical testing of it. The mph and range are 85% to account for drag and other obstacles. The motor is the CarvON v2.5 single 85kV hub motor, and the range is probably way off, as it doesn't account for a lot more variables, even though it is still at 85% efficiency.
<img src="/uploads/db1493/original/3X/4/a/4adb8a744a8a243a310d0d8325f73f28aa77c00b.PNG" width="677" height="500">
```

---
## \#2 Posted by: laurnts Posted at: 2016-11-19T00:02:40.876Z Reads: 192

```
If you count bms, meter, charger, switch into consideration, then the spacecell is a good price. Since I dont use meter, bms and switch, I saved alot of money by giving away ease of use. Btw 50c is too much. I found that 25c 5000 compared to 30c 8000 have alot of difference. But more than 30c 8000 your paying too much for slightly better performance.
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-19T00:37:15.361Z Reads: 182

```
where did you get those range estimates? the SCP3 has more watt hours and less range? You also won't get anywhere near 30 miles with 270wh, especially on hubs.
```

---
## \#4 Posted by: Esrapp21 Posted at: 2016-11-19T01:35:17.782Z Reads: 168

```
http://217.118.128.188/tests/ev_calc.html But I agree, as I said before, that the range is probably way off.
```

---
## \#5 Posted by: Esrapp21 Posted at: 2016-11-19T01:48:01.300Z Reads: 163

```
Yeah, in my mind I would sacrifice a little bit of extra money for a bit more convenience. But I can see where you are coming from. The only reason why I liked the batteries that I chose was because in series they are 12s, a good voltage source, and 6 ah. I didn't really pay attention to the C rating. The SPACE Cell Battery only has 8C and I think even that is sufficient.
```

---
## \#7 Posted by: saul Posted at: 2016-11-19T04:21:02.251Z Reads: 147

```
those nano tech are overkill

10c multistar at 12s 5200mah gives me 10-14 miles..... on a single v2 carvon
space cell is nice because its just about plug and play...but @barajabali can do that with custom style.
```

---
## \#8 Posted by: Esrapp21 Posted at: 2016-11-19T14:52:15.140Z Reads: 125

```
[quote="Jinra, post:6, topic:13293, full:true"]
(post withdrawn by author, will be automatically deleted in 24 hours unless flagged)
[/quote]


Actually, if you do the calculations, with a peak output of 60A and a capacity of 7.5A, 60/7.5 is 8, so it is 8C.
```

---
## \#9 Posted by: Esrapp21 Posted at: 2016-11-19T14:56:45.297Z Reads: 117

```
Like I said before, I couldn't care less about c. I wanted 6Ah for decent battery life and 6s so I could have a 12s high voltage source.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-11-19T17:00:39.958Z Reads: 112

```
[quote="laurnts, post:2, topic:13293"]
Btw 50c is too much. I found that 25c 5000 compared to 30c 8000 have alot of difference. But more than 30c 8000 your paying too much for slightly better performance.
[/quote]
I'll have to disagree with you on this. 
I have compared 5000/25c with 5000/60c
The higher C rating means less voltage sag under load which not only improves performance but also increases range and durability of the batteries. 
After experiencing this first hand, I will have to say that no C ratting is too high when it comes to Lipos and E-boards. 
That said, the battery listed in this post is not a 50C battery, it's a 25C constant with 50c peak. 
The batteries I tested and am currently running are 60C constant and 120C peak. 
They also have a higher charge rate of 5C or 25a so they can handle regen braking better as well. 
https://hobbyking.com/en_us/turnigy-5000mah-2s-7-4v-60c-hardcase-pack.html
```

---
## \#11 Posted by: Kaden56 Posted at: 2016-11-20T09:44:41.878Z Reads: 91

```
I went with diy electric skateboards 10s4p for all of these same reasons. 360wh with a plug and play convenience is SO worth $400. Didn't have to even see a battery cell and it's ready to go :) the funny thing is that when I decided I would build a board I told my wife $400 total and she barely agreed. There has been some slow and steady convincing to get to $900 in parts (so far) hahaha
```

---
## \#12 Posted by: Namasaki Posted at: 2016-11-20T22:06:47.706Z Reads: 81

```
I noticed that you rated the Space cell at 8C discharge.
C ratings are mostly pertaining to Lipo battery packs.
With 18650 Li-ion packs, the cells used have a discharge rating in amps.
 I'm not sure but I think some are 20a and some are 25a constant discharge depending on brand.
So you need to know exactly what cells are being used in the pack your buying so you can find the discharge/charge specs on them. Multiply by the number of cells in parallel to get the packs max cont discharge and charge rate.
```

---
## \#13 Posted by: powerhungry Posted at: 2016-11-26T17:21:16.815Z Reads: 62

```
I was going to build out of 18650 myself, then was going to buy lipo packs then was going to just do a simple few rc batteries then thought maybe a car battery u know the electric car lipo packs, so frustrated with mah,and c rating haven't done nothing , I'm looking for power range and speed. I'm thinking running 3 batteries at 5000 mah 30c ..3 in series and then 3 in p. now that should take me places lol
```

---
## \#15 Posted by: laurnts Posted at: 2016-11-26T22:30:58.797Z Reads: 45

```
I compared 25c 5000mah with 30c of 8000mah. On discharges at 125A and one discharges at 240A. Ofc there are major differences here. 50C 5000mah also discharges at 250A which is relatively same as 30c 8000mah. Thats why we are both right on this.

However Ives tested higher discharge by having more 30c 8000mah in parallel which in the end give me 500A capable discharge with 1000A burst. Almost no differenece at all. But again depending on what drive system you have, your weight and motor.

190kv belt and or dual 110kv hub motor I say minimum 240A discharge rating. Will output nice maximum torque at start up. In my build I also add giant capacitor to further pushes the discharge power of the battery for the startup.
```

---
