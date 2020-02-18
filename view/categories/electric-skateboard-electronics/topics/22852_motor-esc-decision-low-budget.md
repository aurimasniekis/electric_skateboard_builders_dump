# Motor &amp; ESC decision &#124; low budget

### Replies: 18 Views: 2223

## \#1 Posted by: Vaney Posted at: 2017-05-11T21:27:06.042Z Reads: 183

```
Hi guys,

I need some help choosing a motor and an ESC for my first build.
Some numbers to work with
top speed I want: 30-35km/h (~20mph)
normal speed (most time): 20kmh (~12mph)
my weight: 60kg (~130lbs)
wheels: 70mm
My build will run with 2x3S Lipos in series -> 6S
I don't need much torque, as I'm living in a flat area and don't need starts from standing still.

Most people say you should buy a motor with low kV, but others have done some builds with pretty high kV motors.  [380kv](https://www.electric-skateboard.builders/t/budget-electric-skateboard-krown-exotic-krown-trucks-380kv-prop-drive-custom-motor-mount-6s-5000-mah-hobbyking-x-car/4325) or even [430kv](https://www.electric-skateboard.builders/t/the-proof-that-you-can-electrify-your-longboard-for-350/19499).

I will use this [mount](https://www.banggood.com/Electric-Skateboard-Accessories-Belt-Motor-Bracket-Pulley-For-7270MM-Wheel-p-1104585.html) which fits for 5065 and 5055 motors. (the motor pulley, I will buy on my own, depending on the needed gearing ratio to gain my wanted top speed (which depends on the kV of the motor xD). I know how to use the eSk8-calc:slight_smile: ).

So found some motors, which I may use for my own build, but I can't decide, cause I don't know I will benefit from low kV. However, here are some:
[Turnigy SK3 5055-280kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html?___store=en_us)
[Turnigy SK3 5065-320kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html?___store=en_us) (example [calculation](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":320,"system-efficiency":80,"motor-pulley-teeth":22,"wheel-pulley-teeth":48,"wheel-size":70}|) for this motor)
[PROPDRIVE **v2** 5060 270KV](https://hobbyking.com/en_us/ntm-prop-drive-50-60-270kv-2400w-1.html?___store=en_us) (I don't even know, they would fit, but 5060 is between 5055 and 5065 so I thought...) (I've seen nobody testing them (the VERSION2), but I've seen the NTM 5060 270kV in many builds (not V2))

which motor fits my use case the most or are there any proposals for a different motor in about the same price-range?

I also found some ESCs, which should get the job done, but don't know, which one to pick
[FVT 120A](https://www.banggood.com/de/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-Skateboard-ESC-p-985970.html) (Primary choice, cause It's recommended in some threads and the Skateboard Programming)
[HobbyKing X-Car Beast 120A](https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html?___store=en_us)
[Hobbywing 150A](http://www.ebay.de/itm/Hobbywing-QUICRUN-WP-8BL-Wasserdicht-Brushless-150A-ESC-Regler-1-8-RC-Car-Buggy/321520445669?_trksid=p2047675.c100623.m-1&_trkparms=aid=222007&algo=SIC.MBE&ao=2&asc=43785&meid=8412e7d137d3430497fbc80776fa0666&pid=100623&rk=2&rkt=6&mehot=ag&sd=291777557740) (seen much people recommend this, but its price is a little higher (~75€ -> ~80$) (the FVT costs 15€ less, including taxes))

I've also read about people running their motor with this [90A Boat ESC](https://hobbyking.com/de_de/hobbyking-90a-boat-esc-4a-sbec.html?___store=de_de) who said 'it never ran hot'. It has a really attractive price, but I'm not quite sure about it.

So which ESC would you guys recommend? Is the FVT alright?


Kind regards


PS: The recommendation of the wheel pulley says, that it only fits 72mm wheels. But I will just drill holes in my wheels. So it should work with this pulley, shouldn't it?

btw, I'm from Germany so hobbyking parts should be in EU-warehouse for me :slight_smile: 

PPS: sry for the long text and sorry for shitty grammar, etc xD
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-11T22:13:25.898Z Reads: 155

```
You should use larger wheels. 
With 70mm, your pulley and belt will not have enough ground clearance. 
And with larger wheels, you'll have higher top speed and a smoother ride. 
At least 83mm or 90mm

6s
90mm wheels
260kv motor
15/36 gears
20 mph
```

---
## \#3 Posted by: Namasaki Posted at: 2017-05-12T01:26:28.078Z Reads: 143

```
[quote="Vaney, post:1, topic:22852"]
FVT 120A (Primary choice, cause It's recommended in some threads and the Skateboard Programming)
[/quote]

I've never personally tried an FVT ESC but the word on the street is that they work but they don't last.
If this is true, then after you buy the 2nd one, you'll have spent enough money for a Vesc.
```

---
## \#4 Posted by: Alan_Smithee Posted at: 2017-05-12T03:24:51.750Z Reads: 131

```
if you want to go hardcore cheap, there are super basic ESC like this one:
https://hobbyking.com/de_de/hobbyking-100a-esc-4a-ubec.html 
or even this one:
https://hobbyking.com/de_de/hobbykingtm-ss-series-90-100a-esc-opto-only.html

I'm using the first one on my 6s test board together with a keda 240kv motor (it goes to 30km/h with larger wheels, a bit more kv would be preferable I think) and it works no problem. but you will not have a break with these cheap ESCs.

as namasaki said.. use an FTV 120A ESC which gives you more features or even a VESC for maximum configurability. A VESC (very nice breaks!) however only offers 50A constant current draw (with 130A max for a short time).
Since you are on 6S, you will need more amps than a higher voltage setup for the same power . That might be dangerous for the VESC. The FVT is 120A constant iirc. 

and yes.. larger wheels.. 70mm is simply not enough for good ground clearance and high enough top speed. get some 90 or 97mm flywheels clones. If you're in europe, they might be hard to get.. I think, I'll make a EU group buy for these in the next few weeks
```

---
## \#5 Posted by: aigenic Posted at: 2017-05-12T08:00:26.822Z Reads: 109

```
I wouldn't use any of these ESCs because they are not CAR ESCs, which means they will break when you have your throttle in neutral...
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-05-12T08:36:33.981Z Reads: 105

```
They are ESC not VESCs!
```

---
## \#7 Posted by: aigenic Posted at: 2017-05-12T09:21:03.236Z Reads: 107

```
Yeah I know, i somehow mischanged the worlds :D sorry
```

---
## \#8 Posted by: Jebe Posted at: 2017-05-12T10:01:15.559Z Reads: 108

```
<img src="/uploads/db1493/original/3X/6/9/696dd33dbf99bf720166ac78b0147098abf2b3e8.jpg" width="690" height="388">
Here's what happened to my FVT at 6s, small incline, thermal cut out kicked in a moment before it let all the magic black smoke out
My advice, if you are on a budget DIY is not for you. Buy an evolve. DIY is constant $$$$. especially if you have a limited budget as you will always experience failures while you learn.
Most reliable ESC - hobbywing max 6, but it's more than a vesc, - the lower the voltage, the higher the current so you will put pressure on your components.
Seriously, DIY costs me more than buying a ready made board, and still, isn't as reliable.
I only do it because I love to build shit.
```

---
## \#9 Posted by: Jebe Posted at: 2017-05-12T10:02:18.533Z Reads: 105

```
Oh, and I have more money than sense !
```

---
## \#10 Posted by: bartroosen12 Posted at: 2017-05-12T11:24:21.175Z Reads: 99

```
I have had the 120A boat esc and the sk3-320kv
Don't buy the boat esc, it's good for cruising without brakes because they are so bad!
The good thing about it, it's the build quality.
Not just a plastic housing but a aluminum one, so it feels like a well solid piece.
I've not had any problems with the 320Kv motor.

Right now I have the FVT 120A and the sk3-236kv and they run very good in my opinion.
Good brakes, smooth startup and I'm running it without a fan (just because that looked like a crappy fan)

If you're using that kit, ground clearance will be fine with 70mm wheels but if you wanne get a speed between 30-35km/h, you will need the 320kv motor and 83mm wheels to go 34km/h.
The gear ratio (48/16="3") is so high that you need a high kv and big wheels to get a decent speed...

Aren't there other cheap kits with lower gear ratio (gear ratio around "2") ?
```

---
## \#11 Posted by: Jebe Posted at: 2017-05-12T11:29:15.812Z Reads: 88

```
how do you find hill climbing?
```

---
## \#12 Posted by: bartroosen12 Posted at: 2017-05-12T11:54:49.276Z Reads: 89

```
We have no big hills so most flat, but the steepest we have are bridges (10%) and never had problems with them.
```

---
## \#13 Posted by: Vaney Posted at: 2017-05-12T12:31:55.878Z Reads: 82

```
Thanks for all the answers!

[quote=bartroosen12]If you're using that kit, ground clearance will be fine with 70mm wheels but if you wanna get a speed between 30-35km/h, you will need the 320kv motor and 83mm wheels to go 34km/h.
The gear ratio (48/16="3") is so high that you need a high kV and big wheels to get a decent speed...[/quote]

I will buy a pulley with more teeth to fit my top-speed. So for example, if I'd get the SK3 with 320kv, I will use a pulley with 22t (bought separately in a store). [Calcuation](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":320,"system-efficiency":80,"motor-pulley-teeth":22,"wheel-pulley-teeth":48,"wheel-size":70}|)
Or if I'd go with the 270kV motor, I will use a [24t or 26t](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":270,"system-efficiency":80,"motor-pulley-teeth":26,"wheel-pulley-teeth":48,"wheel-size":70}|) pulley for the motor.
But I don't know, which would be better in terms of performance, heat and efficiency. 

btw I prefer to save money by using my wheels instead of buying new.
```

---
## \#14 Posted by: Alan_Smithee Posted at: 2017-05-12T14:36:59.879Z Reads: 73

```
[quote="aigenic, post:5, topic:22852, full:true"]
I wouldn't use any of these ESCs because they are not CAR ESCs, which means they will break when you have your throttle in neutral...
[/quote]

no they won't. you can turn the break feature on or off. I have it switched off on my test board and it rides just fine. you have to break like on a regular board. with your feet. I wouldn't recommend it for city traffic obviously but out of the city its very ridable.
```

---
## \#15 Posted by: Vaney Posted at: 2017-05-13T22:31:06.755Z Reads: 65

```

I noticed, that i didn't replied the right way, so:
[quote=bartroosen12]If you're using that kit, ground clearance will be fine with 70mm wheels but if you wanna get a speed between 30-35km/h, you will need the 320kv motor and 83mm wheels to go 34km/h.
The gear ratio (48/16="3") is so high that you need a high kV and big wheels to get a decent speed...[/quote]

I will buy a pulley with more teeth to fit my top-speed. So for example, if I'd get the SK3 with 320kv, I will use a pulley with 22t (bought separately in a store). Calcuation1
Or if I'd go with the 270kV motor, I will use a 24t or 26t pulley for the motor.
But I don't know, which would be better in terms of performance, heat and efficiency.

btw I prefer to save money by using my wheels instead of buying new.

Anyway, is the PROPDRIVE v2 5060 270KV the best option, cause it has the highest max current of 90A?
And it should fit the motor mount, shouldn't it? (Motor mount is recommended for 5055 and 5065 motors)
```

---
## \#16 Posted by: bartroosen12 Posted at: 2017-05-14T15:29:43.639Z Reads: 57

```
Oh yeah that's perfect if you find some other motorpulleys. There won't be a big difference between the SK3 and NTM, maybe the sk3 build quality will be a bit better but the ntm has a bit more power but both very good motors.
```

---
## \#17 Posted by: Surfer Posted at: 2017-05-14T15:36:34.474Z Reads: 52

```
This one is not tested yet, I hope soon. It looks pretty and I'm not in love with vesc.
Price wise is amazing!!

www.electric-skateboard.builders/t/fvt-dual-motor-esc/23016
```

---
## \#18 Posted by: Davey Posted at: 2017-05-14T16:28:15.354Z Reads: 54

```
Sure you can be as dumb as me and use 430kv but that's not a good choice. :smile: Even with full protection I don't dare to go full speed, because of unexpected cogging and the small torque of the 5055 motor.
```

---
