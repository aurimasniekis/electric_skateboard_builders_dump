# CHALLENGE BUILD! Laptop batteries,motor options considering low current

### Replies: 18 Views: 327

## \#1 Posted by: aos64 Posted at: 2019-08-16T19:47:47.429Z Reads: 92

```
we need to establish few things beforehand.

first of all,living in a country which has weak currency against usd.so gotta use dead laptop batteries because they are dirt cheap out here.if not im not gonna be able to afford to build an esk8.

so my first build have to shape around the continious current bottleneck of the storage laptop cells.for better safety and better performance more paralleled cell groups are necessary.considering the number of cells i have and considering the board size i can use, need to go with 8s8p pack.

so not a 10s or 12s build and even with 8 parallel groups my continious current will be limited around 35-40a(i will try to get my hands on legit laptop bateries)

also unfortunately due to currency and shipping limitations wont be able to use a VESC(not available in my country).so i have to work with rc ESC.

and also i have problems with even the simplest stuff,like longboard availability,80/90mm wheel availability etc.literally couldnt find a regular wheel which has bigger diameter then 70mm let alone finding a wheel with pulley attached.so will find biggest wheel and try to modify a pulley into it.also mount bracket needs to be made by me.apparently noone interested in longboards out here...

im currently 75kg and i can say that city im living in has hills here and there.

what kind of motor makes sense for a build like this?diameter,shaft length,kv value?

i can get my hands on a single 6374 170kv motor.considering im an inexperienced rider,with a correct gear ratio and 40a current limit,would this build be suitable?i think 20-25kmh would be plenty for me.

i just cant pick stuff off a shelf...
```

---
## \#2 Posted by: ShutterShock Posted at: 2019-08-16T21:10:59.852Z Reads: 84

```
I think your best option given your strict constraints might be to get hubs.  Weird as it sounds it might be better than the trouble of making a mount and everything.  I have a Landwheel and I have been using it on a modified 8s3p pack that I made from flat lipo cells extracted from a few dead Landwheel packs.  
https://forum./t/frankenwheel-landwheel-l3-x-mod/4305?u=shuttershock 
I am using VESCS but there are a few ESC's / hub motors out there that are good for the price

How accessible is it for you to order from China?

Additionally, it is possible to use something like the ownboard kit, which uses a great hobbywing esc and has a pretty good 8/10 belt drive

https://www.ownboard.net/collections/parts-accessories-for-electric-skateboard/products/ownboard-dual-belt-motor-kit?variant=29227542872106
```

---
## \#3 Posted by: aos64 Posted at: 2019-08-16T22:03:38.505Z Reads: 70

```
thx for your input.

buying 1 strong motor is cheaper then buying 2-4 weak hub ones and also it gives you more freedom for different configurations in the future imo.

it seems like a good kit but pretty expensive and also i have access to raw material and cnc machining.so i would rather get my hands dirty.

another question,since batteries im gonna use have limited discharge current there are 2 options for making it work

1-making more available discharge current by paralleling more cells.

2-but you can also achieve the SAME WATT and lower current by increasing the voltage.

i thought option 1 would be my best bet but im having doubts about that now.what option would generate better outcome?i think motor still has a big role in this answer and i cant decide which one to get.which motor should i choose to squeeze out more performance with less amps?
```

---
## \#4 Posted by: ShutterShock Posted at: 2019-08-16T22:14:42.645Z Reads: 70

```
Fair enough, I also much prefer the belts over hubs, but the hubs can be cheaper in the end, which was my main point, additionally, the hubs pull a lot less current in my experience, and you don't get the loss of traction that you do with one motor.

However, seeing that you want to make your own mount, that's cool for sure.  With less voltage it is going to take more amps to get it going.  I don't know what kind of amps a 6374 is going to want to pull at 8s, I think most people run 10s, so if you were to able to make a 10s one with more cells maybe that would be better
```

---
## \#5 Posted by: Randy_bobandy Posted at: 2019-08-17T01:58:20.344Z Reads: 65

```
Is it possible to find any used 18v drill batteries? The cells are high current cells atleast 10-15amps.
```

---
## \#6 Posted by: Santino Posted at: 2019-08-17T08:16:45.907Z Reads: 60

```
Chain drive it is a reliable solution, also if you have a cnc machine you could make almost everything (motor mount, spurs, etc...). My country have the same problem, 1usd = 60 Pesos...But here they sale cheap fake batteries, and used laptop batts, for almost the same price of original ones...Wheelchair wheels could be a solution if you have shity roads like me, you will win clearance and that is great if you are going to put a lot of cells... 2 x 6374 motors will give you better power and great handling (you will waste less energy, great torque, and equal differential power distribution)...If you can get a low kv (150kv or 130kv for example), the benefit will be more torque with less amp requirements, therefore your battery will work much better for your needs... Hope my thoughts help you
```

---
## \#7 Posted by: Jebe Posted at: 2019-08-17T10:07:23.886Z Reads: 57

```
laptop batteries will not work, sorry, not even an option.
Lipo batteries will be your best bet.
www.hobbyking.com ship worldwide and have good specials
```

---
## \#8 Posted by: Super Posted at: 2019-08-17T14:06:29.069Z Reads: 54

```
Um yes they would. Sure your performance would suck but if you had limited options(weak currency, budget, etc) in building an esk8 and you just want to have fun, this is the way to go.
```

---
## \#9 Posted by: Grozniy Posted at: 2019-08-17T14:55:08.337Z Reads: 54

```
It's possible
https://youtu.be/pI8E2xMcUjo
@aos64 what is the hardest part for you to get?
```

---
## \#10 Posted by: aos64 Posted at: 2019-08-17T16:38:37.346Z Reads: 50

```
yea its possible.

so im gonna modify my board(which is kind of a cheap board for testing anyways) and i would be able to up my battery config to 12s8p-12s9p.but considering i cannot get my hands on a vesc,running with 12s is my biggest problem right now,there is no cheap esc which can run more than 6s.so i would say hardest part for me to get is vesc/esc.

i wonder can i do dual 5065 setup with ***6s8p*** battery for each motor(and also cheap 6s esc for each motor) instead of 12s8p single 6374(which means needing to buy a vesc)? 6s with 15-20amp each would be enough for motors?

if not i wont push my chances and try to get an vesc for 12s single motor setup.

edit:yes i can buy stuff from china,my motors will come from there.and no its not easy to get my hands on to dead drill batteries.people change the dead cells and reuse the pack because they are expensive.even people does that for laptop batteries in my country...but was able to find laptop ones for 1usd per laptop battery.generally 3s2p pack inside and 1 dead cell per battery,so i can salvage 5 cell for a buck,means 12s8p config would cost me like 30bucks.

edit2:oops,meant 6s8p instead of 6s4p.edited the part to bold text type.
```

---
## \#11 Posted by: Grozniy Posted at: 2019-08-17T17:03:27.118Z Reads: 46

```
In your place I would buy a ESC substitute for 50. You'll be able to run dual setup on 10s. It will give around 15/20A per motor
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F173935689034
```

---
## \#12 Posted by: Jebe Posted at: 2019-08-18T09:32:21.074Z Reads: 37

```
Putting together a battery made up of cells with different capacities and discharge rates is a really bad idea. Those ebay bms's will not balance a pack like that. That pack is a flare waiting to happen.
```

---
## \#13 Posted by: aos64 Posted at: 2019-08-18T09:50:03.290Z Reads: 36

```
esc substitute is looking like another option,thanks.

since i havent done any pack bigger then 5-10 cells before,further research is needed on my part.but i think its possible because people doing few kw packs from laptop batteries for solar usage.
```

---
## \#14 Posted by: Jebe Posted at: 2019-08-18T10:07:49.408Z Reads: 35

```
solar storage and eskate power are too completely different uses.
solar storage does not have high current draw consistantly, they are also tending to pay massive parallel packs. they also fuse individual cells so one going down doesn't turn into a short. but what the hell do I know
```

---
## \#15 Posted by: aos64 Posted at: 2019-08-18T12:59:03.216Z Reads: 26

```
Yes you are %100 right.but what i was trying to say is i thought those problems were solvable for esk8 use,at least on the paper.you can build a 10p pack and limit the esc for what your pack can deliver max safely,so it turns into not so different then solar.

Like,12s and 35-40amps battery current limit  is not usable for esk8?it makes like 2kw at peak power(not considering efficiency losts and sag) and im not even experienced rider,not gonna be able to go more then 12miles/h at first probably lol.
```

---
## \#16 Posted by: Komamtb Posted at: 2019-08-18T13:27:26.137Z Reads: 24

```
Where are you?
```

---
## \#17 Posted by: aos64 Posted at: 2019-08-18T13:28:26.537Z Reads: 24

```
living in Turkey.
```

---
## \#18 Posted by: leroy Posted at: 2019-08-23T04:32:27.937Z Reads: 15

```
I've built  several boards following the

>  **"10-12s battery, a vesc, and a low amp motor**" setup.

Finally,

>  **I decided to try a hobbywing 6s 150 amp esc, 80amp 2000w motor and a couple of 24volt drill battery packs,**

and that's the board I've ridden for the last 8 months.

 I weigh 200lbs, and I can start the board from a dead stop.
> 
> Top speed I've seen on it is
> **26 mph, that's a good speed for a motorized skateboard.**

it climbs hills like mad, and has never stalled or even sputtered going uphill.

>  **As long as you keep airflow over the esc, the heat from the high amps is not an issue.**

> Those cheap esc are shit, **don't by a cheap esc.**

**> Batteries are heavy, and a 50lb board is no fun to carry around.**

I say **yes to high amp motors and higher amp escs**, I think a 6s4p is a good size. 
> **Have you considered adding a bank of capacitors to smooth out high amp spikes?**
> **Capacitors are cheap.**

> That's just my opinion.....
```

---
