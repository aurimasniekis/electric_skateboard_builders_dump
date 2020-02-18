# What do you guys think of my build?

### Replies: 28 Views: 1778

## \#1 Posted by: Snowi Posted at: 2017-07-14T22:27:18.698Z Reads: 185

```
Hey guys. I am making my own electric skateboard, but instead, there are going to be modifications. Mostly, this is for college, but check it out anyways. Tell me if any parts should be changed. I would love feedback.

Motor:  Turnigy Aerodrive SK3 260kv
Battery: 2x Turnigy 5000mAh 5S 20C Lipo Pack
ESC: VESC Torque Boards
Controller: Torque Boards Nano
Motor Gear: 16T
Wheel Gear: 36T

I will be 3d Printing the motor mount, the gears, and the enclosure.

Do you guys think this setup will fail or not?
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-14T22:31:45.610Z Reads: 180

```
All the parts look pretty good. 2 things:

1. The nano remote is notorious for drop outs. I recommend a mini remote or GT2B.

2. I have not seen a successful 3d printed motor mount. They just don't have enough strength. Aluminum is your best bet. 

Other than that your good!

You can also check out my store here: www.buildkitboards.com/collections/all. I have some of the parts available that your looking for.
```

---
## \#3 Posted by: WARMAN Posted at: 2017-07-14T23:24:53.290Z Reads: 164

```
Looks good I agree with @JLabs though you want a strong mount for something that's going to propell you at speed.
Also i have some gt2b's in stock with the lead to connect to esc/vesc  
Never had a dropout with it,very solid connection.
http://www.electric-skateboard.builders/t/battery-enclosure-35-gt2b-18-with-free-cable-free-uk-shipping/26067?u=warman
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-15T00:50:38.476Z Reads: 137

```
[quote="JLabs, post:2, topic:27655"]
The nano remote is notorious for drop outs. I recommend a mini remote or GT2B.
[/quote]

DIYES doesn't sell the v1 anymore. I found the v2 to be very reliable but not without it's cons (auto-bind)
```

---
## \#5 Posted by: JLabs Posted at: 2017-07-15T00:53:02.437Z Reads: 127

```
Well then yes, that one is more reliable. I thought he was referring to the V1
```

---
## \#6 Posted by: Snowi Posted at: 2017-07-15T01:41:37.236Z Reads: 110

```
Do you guys think I will burn out the motor or esc? I feel like 260kv is too much
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-15T01:45:13.674Z Reads: 100

```
It will if you put them in series, go for <= 210kv
```

---
## \#8 Posted by: Snowi Posted at: 2017-07-15T02:09:37.579Z Reads: 101

```
How can I avoid this without changing the motor? Can I put a throttle on the motor or something?
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-15T02:20:25.231Z Reads: 100

```
Couple options:

1. Get 2x 4s batteries for 8s instead
2. Put your 5s batteries in parallel (not recommended)
3. Limit your eRPM on the VESC (inefficient)

Best option is to get a more compatible motor though.
```

---
## \#10 Posted by: Snowi Posted at: 2017-07-15T04:32:56.344Z Reads: 88

```
So should I get a more compatible motor and 2x 4s batteries? Also, what is another hobby online store besides HobbyKing.
```

---
## \#11 Posted by: Snowi Posted at: 2017-07-15T04:34:02.952Z Reads: 86

```
Nvm, how is a 213kv motor with my current setup?
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-15T04:48:12.113Z Reads: 81

```
Yea should run fine
```

---
## \#13 Posted by: Snowi Posted at: 2017-07-16T15:43:17.851Z Reads: 64

```
Do you think a 2x 3000 mAh 30C battery would do better or worse in terms of range?
```

---
## \#14 Posted by: gliz5714 Posted at: 2017-07-16T16:16:21.119Z Reads: 59

```
To the best of my knowledge, mAh more or less the range.  So if you downsize to 3000mAh (what 'S'?), you will cut your range by about 40% off of the 5000mAh - Probably something close to 5 miles.

[quote="sl33py, post:8, topic:21776"]
to calculate your distance - determine your Wh of your pack (V x Ah = Wh), and 10Wh = 1km (typical).  Good ballpark to see what size pack (mAh and voltage) you need for your goal of 10-15miles (you want 160-240Wh pack - easy math helps).
[/quote]
```

---
## \#15 Posted by: Snowi Posted at: 2017-07-16T16:33:49.040Z Reads: 57

```
My batteries are 5S, 10S in total with two batteries in series. Does the calculation include the C rating as well? For example, my battery is 3 Ah, but with the 20C rating, it would go to 60 Ah. Should I calculate the 60Ah or 3Ah.
```

---
## \#16 Posted by: Jinra Posted at: 2017-07-16T16:34:57.519Z Reads: 56

```
Just watt hours, nominal voltage x mah. The more you have the more range (approximately 10wh = 1km)
```

---
## \#17 Posted by: Snowi Posted at: 2017-07-16T16:37:53.842Z Reads: 50

```
Do you mean mah or ah? I don't belive mah is right
```

---
## \#18 Posted by: Jinra Posted at: 2017-07-16T16:40:07.700Z Reads: 46

```
right ah, though they're the same just a lower unit of measurement.
```

---
## \#19 Posted by: Snowi Posted at: 2017-07-16T16:41:47.299Z Reads: 46

```
cool. One more question: Should I calculate the ah with the 20C rating or not? For example, my battery is 3 Ah, but with the 20C rating, it would go to 60 Ah. 3Ah or 60 Ah?
```

---
## \#20 Posted by: Jinra Posted at: 2017-07-16T16:43:52.000Z Reads: 54

```
C rating signifies discharge potential. While the rate of discharge plays into the time to depletion, it has no bearing on the watt hours of the pack.
```

---
## \#21 Posted by: Snowi Posted at: 2017-07-16T16:45:02.282Z Reads: 48

```
Oh I thought it does. I guess I misread this Battery guide: http://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/36?source_topic_id=215
```

---
## \#22 Posted by: Snowi Posted at: 2017-07-16T16:48:46.027Z Reads: 47

```
Is putting 2 batteries in series will make it go further in distance or faster? I am confused whether to put my two batteries in series or parallel.
```

---
## \#23 Posted by: Jinra Posted at: 2017-07-16T16:50:05.258Z Reads: 49

```
I'd aim for 10s. putting in series directly increases the watt hours of the pack and increases range
```

---
## \#24 Posted by: wafflejock Posted at: 2017-07-16T16:56:18.234Z Reads: 51

```
Series increases voltage but doesn't add the capacity (you get power at higher voltage but the electrons flow through all cells in series at the same rate Amps, one bucket pouring into another pouring into a pipe).  If you put batteries in parallel with the same voltage their voltage doesn't add but the capacity is increased ( you have twice the buckets at the same height pouring into the same pipe... Twice capacity no change in voltage potential)

---

C rating has to do with max amperage due to internal resistance and heat build up in the batteries, higher amperage through a fixed resistance creates power loss I^2*R higher c rating means higher max amps and less voltage sag under load (when pulling high amps to drive the motor).  Power to the ESC and motor is a product of voltage and amperage so 20V at 20A is 400W if you have a 40V battery only need 10A to deliver the 400W. C rating is used in conjunction with the Ah of the pack to determine max amperage so a 5Ah battery with 10C rating can discharge at 5*10=50A whereas a 20C with same Ah would be 5*20=100A
```

---
## \#25 Posted by: Snowi Posted at: 2017-07-16T22:53:04.148Z Reads: 31

```
So what would be better? 20C or 30C?
```

---
## \#26 Posted by: Jinra Posted at: 2017-07-16T23:03:51.350Z Reads: 35

```
The more the better
```

---
## \#27 Posted by: Snowi Posted at: 2017-07-17T02:45:32.676Z Reads: 31

```
Is it better to have a shorter or longer belt? Or does it not matter?
```

---
## \#28 Posted by: wafflejock Posted at: 2017-07-17T02:50:10.102Z Reads: 36

```
You want a belt that fits tight and ideally wider is typically better in terms of power transfer (length shouldn't make much of a difference there).  Another thing to consider is a slightly longer belt will be wrapping around the pulley more which gives you more surface area contact between the belt and the pulley teeth which is always a good thing (see posts on idler bearing usage to improve this further if you're interested as well).

---

http://www.electric-skateboard.builders/t/does-the-location-of-an-idler-pulley-bearing-affect-the-usable-life-of-a-belt/13036/22
```

---
