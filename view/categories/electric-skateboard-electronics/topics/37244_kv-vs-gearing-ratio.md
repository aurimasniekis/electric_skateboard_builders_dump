# kV vs Gearing ratio

### Replies: 35 Views: 2171

## \#1 Posted by: 12meterkuk Posted at: 2017-11-03T12:44:44.417Z Reads: 278

```
Hi there, I have spent the better part of the last 2 months reading up on the forums, and I have found that information regarding this topic is pretty spread out and scattered, making it hard for new users to fully understand it. 

What is the difference between 2 setups, with the same voltage and amp output, but one with a high kV motor with high gearing ratio, and one with a Low kV motor and Low gearing ratio? Both are geared for the same top speed

So far what I understand is that the difference is in efficiency, and torque/responsiveness at higher speeds

I hope the veterans and experienced Builders can chime in and contribute their knowledge to this thread and help out some newbies to understand kv vs gearing ratio better.
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-11-03T12:56:35.602Z Reads: 274

```
Good question. Hopefully somebody with a braoder spectrum of trial and error can speak up here, but here's my experience:

i used to run 270KV 50mm motors at 6S on a 15/36 ratio on 83mm wheels. The motors got hot. The torque wasn't really present so much, and the top speed was south of 30mph. 

I have also run 190KV 63mm motors at 10S on a 15/36 ratio on 83mm wheels. The motors stay cooler, the torque is defeinitely more present, and top speed is around 30mph ish

I now run 190kv 63mm motors at 12S on a 16/32ratio on  90mm wheels. The motors are significant;y cooler at all times, the torque is very very present, and the top speed is well over 30mph, would say 36 or 37 for me. I've been clocked at 36 but i feel i've been faster on that board. 

So what i haven't done here is run a motor on a higher KV at 12S because i'm already bumping the limit. 

I just finished modding an Evolve for which the customer upgraded his motors to 200KV race stars. Same ratio but noticeably faster on the top end then a stock bamboo. 

None of this answers your question directly, and i'm sorry for that, but i really feel like the lower KV on a lower ratio is the better option, and higher voltage while doing so is icing on the cake. 

10S is likely the best place to experiment with this since at 12S you're already bumping the KV limit for most VESC based ESCs out there at the moment.
```

---
## \#3 Posted by: 12meterkuk Posted at: 2017-11-03T14:09:09.476Z Reads: 256

```
Thanks for chiming in

[quote="longhairedboy, post:2, topic:37244"]
I now run 190kv 63mm motors at 12S on a 16/32ratio on  90mm wheels. The motors are significant;y cooler at all times, the torque is very very present, and the top speed is well over 30mph, would say 36 or 37 for me. I've been clocked at 36 but i feel i've been faster on that board.
[/quote]

Have you ever burned a vesc with this setup? That should be cutting it close for the erpm limit no? I have a build planned for 12s and 190kv 63 motors too. Holding off until i have more experience and cash :joy:
```

---
## \#4 Posted by: MoeStooge Posted at: 2017-11-03T14:12:36.386Z Reads: 251

```
1250 kv 4200w single on 8s 72/9 on 90mm wheel.   Inrunner 4 pole 40mmx100mm can. Very small profile light weight. 34mph on a single motor decent accel and will out pull most  dual hub or direct drives and uphill. Inrunner motors work above 90% efficiency and the gear drive is the path of least resistance for a ratioed setup with a 100% mechanical connection.<img src="/uploads/db1493/original/3X/a/2/a21f13ee64374a1a0773e8f782b2a097131b0960.jpg" width="281" height="499">
```

---
## \#5 Posted by: 12meterkuk Posted at: 2017-11-03T14:28:02.427Z Reads: 235

```
[quote="MoeStooge, post:4, topic:37244"]
1250 kv 4200w single on 8s 72/9 on 90mm wheel.   Inrunner 4 pole 40mmx100mm can
[/quote]

thats quite a unique setup, what esc are you using?
```

---
## \#6 Posted by: MoeStooge Posted at: 2017-11-03T14:35:43.037Z Reads: 230

```
200a toro beast.
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-11-03T14:36:05.952Z Reads: 227

```
pics or it didn’t happen 😉
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-11-03T14:58:34.579Z Reads: 226

```
The ERPM limit becomes a false idol when the KV on the motors is wrong anyway. The reaosn i use 190KV motors instead of 200KV motors is because a 200KV motor might actually be a 190KV motor while a 190KV motor is never really quite 190KV.
```

---
## \#9 Posted by: egzplicit Posted at: 2017-11-03T17:32:01.518Z Reads: 216

```
[quote="longhairedboy, post:2, topic:37244"]
I just finished modding an Evolve for which the customer upgraded his motors to 200KV race stars. Same ratio but noticeably faster on the top end then a stock bamboo.
[/quote]

Hey @longhairedboy , do you happen to know how much torque was lost when switching to the 200KV motors? I have just finished a build using racer stars 140kv dual and while I'm happy with the top speed, I wonder how much torque is lost when you go with the 200kv version of these motors.
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-11-03T17:53:08.234Z Reads: 210

```
didn't seem too much different on the Evolve. Still had close to the usual start up feel to it so i'm not sure how much of a difference their tuning makes here as well. On a fully DIY board you could adjust the settings in the ESC and probably eliminate a lot of the difference in just settings.
```

---
## \#11 Posted by: Vanarian Posted at: 2017-11-03T19:41:54.903Z Reads: 201

```
What size is that motor ? It is a mystery to me ! Sick trucks.
```

---
## \#12 Posted by: pixelsilva Posted at: 2017-11-04T08:12:33.425Z Reads: 182

```
I'm trying to know the KV on this motor.... 

Here the specs: rated as **6033** motor (between the 50XX and 63XX class sizes); Amp: < **50A**; Rpm: **5100** (-+)5%; Volt: **36 VDC**; Power: > 1600 W.

Anybody?
```

---
## \#13 Posted by: MonkeyFist Posted at: 2018-03-02T21:07:41.050Z Reads: 150

```
Does anyone have more info on this topic? Is it best to go for low kv and low gearing or high kv and high gearing. :thinking:
I feel like we didnt get any clear advice here. or am i wrong... :roll_eyes:
For example on 6S: 200kv low gearing bigger wheels, or 270kv high gearing smaller wheels.
```

---
## \#14 Posted by: MoeStooge Posted at: 2018-03-02T21:38:57.032Z Reads: 145

```
Important thing is how fast do you want to go and how many watts do you need to achieve that goal the rest is balancing your volts, gearing, wheel size and motor kv. Use this tool. http://calc.esk8.it/
```

---
## \#15 Posted by: MonkeyFist Posted at: 2018-03-02T21:44:36.843Z Reads: 143

```
If you have the same speed on both setups. What would be the best. Or is it just a preference thing? 
What about climbing ability? Heat/amp draw.
```

---
## \#16 Posted by: b264 Posted at: 2018-03-02T21:58:54.643Z Reads: 138

```
Pick a real-world top speed you want to have, like 25mph.  Don't be greedy here, or you won't have as much torque or braking.  Pick a voltage, I recommend 10S (32V - 42V) if you're using a VESC4.  Pick a wheel size, I recommend 97mm - 110mm.

Use an [esk8 calculator](https://www.electric-skateboard.builders/search?q=calculator) to find a pulley ratio and motor kv that works for you.  You want to maximise the motor kv while staying under 50,000 erpm and matching the loaded top speed you picked.

Try not to use pulleys smaller than 15 teeth for belt longevity.
```

---
## \#17 Posted by: Hummie Posted at: 2018-03-02T22:07:02.684Z Reads: 135

```
@MoeStooge spins inrunners a million rpm and maybe gets more efficiency (in the motor) than others. Generally the faster u can zpin the motor the greater efficiency
```

---
## \#18 Posted by: MoeStooge Posted at: 2018-03-02T22:16:04.909Z Reads: 126

```
Think of watts as horsepower. 2000w=2.7hp. If your setup requires 3hp to haul a 170lb load up a 20% grade at 25mph and your setup makes 2.7hp it's going to heat up.  Now gear it for 20mph and your in the zip code and heat  is ok.  More Watts makes more HP = less Heat. When working with watt limits your gearing is most important for keeping your build from making magic smoke.
```

---
## \#19 Posted by: MoeStooge Posted at: 2018-03-02T22:20:04.457Z Reads: 122

```
I like the low pole count renders a more efficient iron to copper ratio theory. They do spin up the kv quite high
```

---
## \#20 Posted by: MonkeyFist Posted at: 2018-03-02T23:13:27.541Z Reads: 114

```
Okay. I think i get it. So it would be better on 6s with 270kv and keep the gearing higher.
```

---
## \#21 Posted by: pat.speed Posted at: 2018-03-02T23:21:07.163Z Reads: 106

```
No, that might reach the same top speed as a lower kV motor and higher voltage but it will have significantly less torque. The best setup in terms of torque and speed is 10-12s and 170-190kV. Then you just have to adjust your gear ratio depending on your wheel size
```

---
## \#22 Posted by: MonkeyFist Posted at: 2018-03-02T23:32:01.119Z Reads: 107

```
Okai. I'm sorry, but the reason i keep mentioning 6s all the time is that i plan to build my first board on 6s. I understand that i can calculate the speed with gearing and wheels size, i just wonder if a 280 or a 200kv motor would be best. :thinking:
```

---
## \#23 Posted by: Pedrodemio Posted at: 2018-03-02T23:43:47.549Z Reads: 107

```
Generally higher motor speed is better

Cooper loss on the motor is proportional to the current, if you run the motor at higher rpm and use a more aggressive gearing you can keep the motor torque lower, thus lower current and lower copper loss, so better efficiency
```

---
## \#24 Posted by: b264 Posted at: 2018-03-02T23:52:26.349Z Reads: 102

```
Did you see my response?

I gave you a fishing pole, and you're still asking for a fish.
```

---
## \#25 Posted by: MonkeyFist Posted at: 2018-03-02T23:56:36.738Z Reads: 102

```
Yes i did. According to it i should choose the 280kv motor on 6s. Am i right? It will be closer to the erpm limit. Sorry, maybe im a little slow. I'm not an expert...
```

---
## \#26 Posted by: b264 Posted at: 2018-03-03T00:00:48.451Z Reads: 98

```
voltage - 6S
max erpm - 50000
efficiency - 85%
wheel size ?
top speed ?
```

---
## \#27 Posted by: MonkeyFist Posted at: 2018-03-03T00:03:55.838Z Reads: 97

```
Wheel size 83mm, top speed maybe 20-22mph. I'm a beginner.
```

---
## \#28 Posted by: b264 Posted at: 2018-03-03T00:14:13.095Z Reads: 95

```
Around about 300kv would be a good match for a 22mph top speed on 15/36 ratio with 83mm wheels and 6S voltage

http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":6,"motor-kv":300,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":83}|
```

---
## \#29 Posted by: GrecoMan Posted at: 2018-03-03T00:14:36.403Z Reads: 96

```
don’t use 300kv lol 🤣

use 270kv. I don’t recommend 6s on the vesc either. it’s not really the sweet spot. if it’s possible, go for atleast 8s and bump it down to 245kv. as a beginner, 15mph feels really damn fast, if you get bored, just change up the gearing a little bit.
```

---
## \#30 Posted by: MonkeyFist Posted at: 2018-03-03T00:23:11.777Z Reads: 89

```
Okay. Thank you for the feedback. :slight_smile: i think i know what to buy now. :thinking:
```

---
## \#31 Posted by: GrecoMan Posted at: 2018-03-03T00:24:34.213Z Reads: 88

```
I highly recommend 10s and 190kv, as it is considered the sweet spot. but if you’re dealing with space constraints or other issues 8s is a bare minimum IMO.
```

---
## \#32 Posted by: b264 Posted at: 2018-03-03T00:25:22.175Z Reads: 92

```
14mph is about where I consider it to be "fast" when you're on an esk8.  25mph is fucking flying and 35mph is "I'm ready to die today"

5-8mph is a normal speed for beginners
```

---
## \#33 Posted by: b264 Posted at: 2018-03-03T00:27:05.761Z Reads: 91

```
[quote="GrecoMan, post:31, topic:37244, full:true"]
I highly recommend 10s and 190kv, as it is considered the sweet spot. but if you’re dealing with space constraints or other issues 8s is a bare minimum IMO.
[/quote]

I'd recommend 10S and [170kv](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":170,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":38,"wheel-size":107}|) or [150kv](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":150,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":38,"wheel-size":107}|) but that's just me.  I like more power/torque/braking instead of top speed personally
```

---
## \#34 Posted by: GrecoMan Posted at: 2018-03-03T00:27:37.888Z Reads: 90

```
[quote="b264, post:32, topic:37244"]
35mph is “I’m ready to die today”
[/quote]
[quote="b264, post:32, topic:37244"]
I’m ready to die today
[/quote]

i think that’s a typo, most of us would call that “fun” 😜
```

---
## \#35 Posted by: MonkeyFist Posted at: 2018-03-03T00:28:26.447Z Reads: 90

```
:laughing:
I think i would be ready to die.
```

---
