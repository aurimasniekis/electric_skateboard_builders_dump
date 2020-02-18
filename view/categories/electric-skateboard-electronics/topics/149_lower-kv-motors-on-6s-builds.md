# Lower kv motors on 6S builds

### Replies: 6 Views: 2312

## \#1 Posted by: longhairedboy Posted at: 2015-08-27T15:02:16.153Z Reads: 138

```
On my daily rampaging 6S build, i've used 245s and 270s. That seems to be the common acceptable pairing for 6S. However I just went to spec parts for a potential customer who only has $400 to spend and found myself with this question:

What kind of results can I expect by using a 170kv on a 6S battery with a 6-8S ESC? Overheating? Weird performance? Will it even matter? Given the unreliability of availability of good motors at low low prices, it can be difficult to always ideally match the kv factor with the S factor when trying to help a brother out. 

Thoughts?
```

---
## \#2 Posted by: torqueboards Posted at: 2015-08-27T15:11:18.003Z Reads: 137

```
6S is perfectly fine to be honest. I think if you are running specifically on flat ground 6S will do up to 20mph maybe climb 10-15% inclines. Granted this is more so someone who is under 200 lbs. Also you can expect to climb a few 10-15% hills but monitoring the heat of the motor is a good indicator if you are overworking your single motor setup.

I've actually been able to scale 20-30% inclines with 6S and dual motors so 12S is literally just for added torque on start-up and more power going uphill and top end. 12S does provide less stress on components since you are using higher voltage immediately. I've had a 230-240lb friend climb a 15-20% incline and he was actually pretty impressed on dual 5055 SK3 on 6S.

Doesn't necessarily mean we have to use the entire 12S voltage like crazy. The added range for the 12S 5ah is double of 6S 5ah for the most part.

To build something for $400 would be a real DIY rig. Your talking about building your own connectors and using a loop plug for your on/off switch, buying the cheapest charger. I'm sure, it's still doable.
```

---
## \#3 Posted by: longhairedboy Posted at: 2015-08-27T15:59:47.883Z Reads: 129

```
A lot of the minor components i actually have on hand. For example, i have about 50 5mm bullet connectors in a bin, tons of screws, excess wire, etc. At any rate, i told the guy $550 was the lowest I could actually go on a build. I'd basically be building it for free at that point, but it might be worth it to get one of my completes out on the street. 

I just wanted to make sure these newer, lower kv motors would do fine with the lower voltages coming from a 6S build because typically you see them paired with 8S, 10S, and 12S, and the 6Ss usually have between 200 and 300 kv motors on them. That may just be my perception of it though because of when i got into this.
```

---
## \#4 Posted by: torqueboards Posted at: 2015-08-27T19:02:59.928Z Reads: 116

```
I would go for a 200KV-280KV type motor for a 6S build. I wouldn't go 200KV or lower usually for a 6S build because of the lower voltage.
```

---
## \#5 Posted by: onloop Posted at: 2015-08-27T23:01:10.641Z Reads: 111

```
I would simply ask the customer what is their desired top speed, then work backwards.

**Novice -** with no skateboard experience but able bodied. 20-25kmh
**Intermediate -** not a veteran skateboarder but has some general "skate/snow/wake boarding" skillz. 25-35kmh
**Experienced skateboarder -** years of riding, very good skillz, understands risk. 45-50km/h


Motor pulley 15
Wheel pulley 36
Battery 6S (22 volt nominal)
Motor kv 170
Wheel diameter 83mm


**TOP SPEED EQUALS 24kmh (15mph)**
So good for a beginner/intermediate.

If they are complete novice go 13T motor pulley = 21kmh top speed.

You can also change power settings in the ESC to further soften the experience.
```

---
## \#6 Posted by: longhairedboy Posted at: 2015-08-28T13:51:25.914Z Reads: 105

```
Thanks guys that was really helpful. I kind of assumed this was the deal with it, but I just wasn't sure.
```

---
