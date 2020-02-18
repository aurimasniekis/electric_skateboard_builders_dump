# Gearing ratio for torque!

### Replies: 23 Views: 2252

## \#1 Posted by: 12meterkuk Posted at: 2017-09-30T03:56:15.943Z Reads: 262

```
Hi guys, I was wondering if a 16/48T gearing ratio with a 270kv 5055 motor (Dual 1400 watt total 2800), 83mm wheels, and 10s setup would get me the torque I need?

I come from an evolve so I am more inclined towards having power than speed. Is this enough torque or should i change it?

Edit: A little vague on amount of torque I need. What i meant was if this setup would carry me (85-90 kg) up 20%+ hills? And how would it compare to other production boards
```

---
## \#2 Posted by: Namasaki Posted at: 2017-09-30T04:14:36.831Z Reads: 258

```
Your about the same weight as me.
I have a build with 
dual 190kv 6355's 4800 watts total
10s 60C Lipos
15/40 gears
90mm wheels
I can go up 20% grade but it's a strain.

270kv 5055's are not gonna cut it for you climbing steeps hills.

And if your using Vesc's, 270kv is way over the erpm limit with 10s

If your wanting more power than speed, get larger motors with lower kv

6355 190kv or 6374 190kv

The larger motors yield more torque.

Higher KV = more speed
Lower KV = more torque
```

---
## \#3 Posted by: 12meterkuk Posted at: 2017-09-30T04:17:59.047Z Reads: 238

```
The motor mounts I am using can only handle 50xx motors. How do i gear the current set up for more torque? I am using a custom esc not vesc. Might upgrade to vescs in the future though

Edit: I don't think I will be getting new motors as everything came in a kit. Kind of a waste to swap out everything :(
```

---
## \#4 Posted by: Namasaki Posted at: 2017-09-30T05:09:29.667Z Reads: 224

```
These are 40T pulleys on 90mm wheels. As you can see there is not a lot of clearance between the ground and the belts.

83mm wheels are gonna be 1/4" smaller dia than these. So take off 1/8" all around and then put a bigger 48T pulley on.
I think that with 83mm wheels and 48T pulleys, your belts will be hitting every little rock on the road.
So that is probably not an option.


<img src="/uploads/db1493/original/3X/3/1/31cafebc656303247c3e03bf1bca16e924cf4608.jpeg" width="375" height="500">
```

---
## \#5 Posted by: Namasaki Posted at: 2017-09-30T05:16:39.704Z Reads: 210

```
[quote="12meterkuk, post:3, topic:34348"]
I don't think I will be getting new motors as everything came in a kit. Kind of a waste to swap out everything
[/quote]

The problem is that your trying to build a board that can take a 90kg rider up 20% grades and that is a tall order!
If you where 60kg riding on flat ground only then I think you could make it work.

Is there any way that you could return the parts you already purchased?
```

---
## \#6 Posted by: 12meterkuk Posted at: 2017-09-30T05:58:47.995Z Reads: 204

```
[quote="Namasaki, post:5, topic:34348"]
Is there any way that you could return the parts you already purchased?
[/quote]

I don't think so... 
[quote="Namasaki, post:5, topic:34348"]
The problem is that your trying to build a board that can take a 90kg rider up 20% grades and that is a tall order!
[/quote]

I don't really need that kind of power as i live in a city with little to no hills, I am only trying to estimate the amount of torque I would have (compared to my gt) as I haven't finished the build yet. I am just addicted to torque =P 

I could always upgrade the gearing and motors in the future though. Best part about DIY
```

---
## \#7 Posted by: 12meterkuk Posted at: 2017-09-30T06:00:55.129Z Reads: 192

```
[quote="Namasaki, post:4, topic:34348"]
I think that with 83mm wheels and 48T pulleys, your belts will be hitting every little rock on the road.
[/quote]

<img src="/uploads/db1493/original/3X/d/e/ded1738e2d3e94247f4a29862a6a3bf05a0b7a11.png" width="500" height="500">

This is the motor and motor mount i got. I think its using 3m belts (Looks like yours is 5m) Maybe thats the difference? The clearance looks to be about the same

Edit: Saw the belts not are not 3m my bad, The specs in the store was 3m though.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-09-30T06:26:22.985Z Reads: 180

```
those are not 48t pulleys. Maybe 32T or 36T
```

---
## \#9 Posted by: Namasaki Posted at: 2017-09-30T06:27:19.447Z Reads: 181

```
[quote="12meterkuk, post:1, topic:34348"]
What i meant was if this setup would carry me (85-90 kg) up 20%+ hills?
[/quote]


This is your statement that my advice was based on.
```

---
## \#10 Posted by: 12meterkuk Posted at: 2017-09-30T06:35:43.024Z Reads: 177

```
[quote="Namasaki, post:9, topic:34348"]
This is your statement that I was basing my advice on.
[/quote]

Yeah, I just wanted to get some form of estimate of torque 

[quote="Namasaki, post:8, topic:34348, full:true"]
those are not 48t pulleys. Maybe 32T or 36T
[/quote]

Are you sure? The site stated 16:48 gear ratio. I'll have to confirm with the owner
```

---
## \#11 Posted by: cwazy1 Posted at: 2017-09-30T06:41:18.326Z Reads: 172

```
Those are 100% not 48t on the wheel. From looking at the wheels and comparing the pulley size, I'd say 32T
```

---
## \#12 Posted by: 12meterkuk Posted at: 2017-09-30T07:01:38.642Z Reads: 169

```
You guys are right. CS confirmed its 12:36 gear
```

---
## \#13 Posted by: Ulfberht Posted at: 2017-09-30T07:04:32.142Z Reads: 169

```
Get a 14t motor pulley or two from collections/motor-pulleys
```

---
## \#14 Posted by: 12meterkuk Posted at: 2017-09-30T07:06:07.058Z Reads: 166

```
[quote="Ulfberht, post:13, topic:34348"]
Get a 14t motor pulley or two from
[/quote]
Wouldn't that decrease torque?
```

---
## \#15 Posted by: Ulfberht Posted at: 2017-09-30T07:25:58.109Z Reads: 165

```
Nope...Reducing the motor pulley size will reduce your top speed, but give you more torque. Do you have a good ESK8 calculator in your bookmarks yet? Here's a good one. :)
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":0,"wheel-pulley-teeth":36,"wheel-size":90}|
```

---
## \#16 Posted by: 12meterkuk Posted at: 2017-09-30T07:27:42.794Z Reads: 159

```
My motor pulley size is 12, not 16 (Just confirmed with the store). So 14 would be an increase?
```

---
## \#17 Posted by: cwazy1 Posted at: 2017-09-30T07:48:18.509Z Reads: 159

```
Don't go 14 unless you want to reduce your torque. I don't think @Ulfberht read your latest post. 

I'd honestly leave your ratios where they are. Going to a 40T on your wheel is only going to have negative impact. You will gain a bit of torque, but what will start to happen is (1) you'll run a higher risk of stuff hitting your belts and (2) you'll start having potential belt slippage unless you want to use an idler or run extremely tight belt, which has its own downsides.
```

---
## \#18 Posted by: Ulfberht Posted at: 2017-09-30T08:46:12.004Z Reads: 150

```
Oops! :nerd:
```

---
## \#19 Posted by: pat.speed Posted at: 2017-09-30T11:59:46.818Z Reads: 144

```
I think it should have enough torque. I run a single motor (190kv) with a 2:1 gear ratio and I can go up very steep hills. I can go up my driveway from a stop and my drive way is pretty steep
```

---
## \#20 Posted by: nomeus Posted at: 2017-10-21T11:40:19.353Z Reads: 121

```
Hey,

Do you think 2.32:1 gear ratio with larger 190kv motor and 83mm wheels can still have a boostedboard'ish torque (75kg no hills)? I dont need to go faster than 35km/h, but I want a decent punch!
```

---
## \#21 Posted by: Namasaki Posted at: 2017-10-21T18:34:28.696Z Reads: 113

```
83mm wheels with 36T wheel pulley and 15T motor pulley with dual 190kv motors is what I used to run. 
Good torque and decent speed with motor max set at 80a
```

---
## \#23 Posted by: nomeus Posted at: 2017-10-21T20:25:50.978Z Reads: 107

```
What battery did you use? Do you remember what range you did get out of it?
```

---
## \#24 Posted by: Namasaki Posted at: 2017-10-21T20:48:29.159Z Reads: 103

```
10s1p  60C Lipo pack.
max range 14 miles on flats
Rider weight 195 lbs

Currently running 90mm wheels with 40/15 pulleys.
Smoother ride with 90s
```

---
