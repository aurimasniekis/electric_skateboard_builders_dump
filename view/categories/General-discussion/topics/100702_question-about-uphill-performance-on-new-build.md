# Question about uphill performance on new build

### Replies: 19 Views: 304

## \#1 Posted by: ODBounty Posted at: 2019-08-22T05:56:06.559Z Reads: 109

```
Hey all, I recently finished my build and I love it. Im just having a little problem with it. When building it I wanted to make sure it could go uphill relatively easily. The build has a 10s3p li-ion battery, vesc from mboards, and a single 6374 180kv motor from mboards. The wheels are all terrain 100mm from amazon. The problem is it can't go up the hill to my house. Did i misunderstand what it takes to go uphill or is there a technical problem? Thank you!
```

---
## \#2 Posted by: Hummie Posted at: 2019-08-22T06:01:14.483Z Reads: 107

```
you should have no trouble   maybe your settings on the vesc is too low or your gearing too low
```

---
## \#3 Posted by: ODBounty Posted at: 2019-08-22T06:12:22.698Z Reads: 102

```
I dont reall know what that means can u elaborate?
```

---
## \#4 Posted by: Skunk Posted at: 2019-08-22T06:29:25.654Z Reads: 101

```
What part?
Vesc settings or gearing? 

I thought people generally went dual drive when needing hill climbing abilities.
```

---
## \#5 Posted by: ODBounty Posted at: 2019-08-22T06:40:30.147Z Reads: 94

```
lmao both xD
```

---
## \#6 Posted by: Skunk Posted at: 2019-08-22T06:44:53.636Z Reads: 90

```
Well vesc setting really kinda determine the way your board behaves. Power, brakes, it's the brains. 

Maybe post your vesc settings? 

Gearing affects speed and acceleration. 
What pulleys are you running? Motor/ wheel
```

---
## \#7 Posted by: ODBounty Posted at: 2019-08-22T06:59:40.461Z Reads: 84

```
Where do I go in vesc tool to see settings?

Gearing: 36t wheel pulley, 16t motor pulley
```

---
## \#8 Posted by: wwohl602 Posted at: 2019-08-22T07:49:50.906Z Reads: 82

```
That’s gearing. Especially with wheels that big. Check out the eskate calculator. Probably a 15 or 14T motor pulley would help.

Your top speed is 30 mph according to it. A 14T would get your top down to 25 weighted but you’d get low end torque back 

I haven’t even finished my build, this is just educated input from me. Hopefully someone will verify soon. 

You could change the wheel pulleys but that’s more $
```

---
## \#9 Posted by: pundahh Posted at: 2019-08-22T08:24:53.928Z Reads: 79

```
I’d bump to like 40+ teeth on your wheel pulley if you want more torque.

And yeah, go under motor in your vesc tool and pull up your max/mins.
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-08-22T08:55:14.437Z Reads: 79

```
Bigger wheel pulley, and/or smaller motor pulley will increase your torque but reduce your top speed.

Increase your motor and battery current up to the limit of your vesc and battery if you haven't already: I'd say 50-60 battery amps and 80 motor amps. (Assuming your 10s3p is made of 30Q cells)

If you do all that and it's still not enough, then you need a bigger battery, and dual motors.
```

---
## \#11 Posted by: MysticalDork Posted at: 2019-08-22T09:00:12.046Z Reads: 77

```
It's also entirely possible that your issue is thermal: You're using a stock 4.12 vesc with a 6374 motor, which is like trying to run a v8 engine with the carburetor from a honda civic - no matter how big your motor is, you're limited by the ESC. That vesc, having lower current capability, no heatsink or significant thermal mass compared to something like a vesc6 or a focbox, will heat up much quicker and begin limiting its output to protect itself.
```

---
## \#12 Posted by: ODBounty Posted at: 2019-08-22T19:48:18.456Z Reads: 52

```
Ok so I have found that Im using UART which replaces PPM so i cant really change the settings. So does that mean that i for sure need to upgrade my vesc from 4 to 6?
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-08-22T20:03:33.230Z Reads: 50

```
Are you sure your vesc is using Uart and not ppm? It's in the settings and won't automatically change when you plug one in vs the other
```

---
## \#14 Posted by: ODBounty Posted at: 2019-08-22T20:16:56.815Z Reads: 48

```
Everyone in this post said its UART (https://www.electric-skateboard.builders/t/question-about-ppm/100716)
```

---
## \#15 Posted by: wwohl602 Posted at: 2019-08-22T20:42:53.955Z Reads: 45

```
I don’t believe this to be the case. Does it run well from a rolling start and at speed?

He said above he’s loving it. Assuming the board is running well and he’s not severely under powered in the VESC settings, i keep coming back to gearing first. 
It’s a single motor board that’s geared to do over 30 mph - either change the motor pulley or try some smaller wheels and see if it makes a difference
```

---
## \#16 Posted by: ODBounty Posted at: 2019-08-22T21:24:21.016Z Reads: 42

```
yeah its my board. it doesnt start on a rolling start but i am using the specific wiring meant for vesc 4 as shown on the flipsky website. and im unable to see PPM
```

---
## \#17 Posted by: MysticalDork Posted at: 2019-08-23T01:25:32.762Z Reads: 35

```
whether you're using uart or PPM has no bearing on your battery/motor current settings.

My previous statements still stand: Change your gearing, and/or change your battery/motor current settings, and if both of those aren't enough, then upgrade your vesc and/or go dual and/or upgrade your battery.
```

---
## \#18 Posted by: Skunk Posted at: 2019-08-23T01:30:59.799Z Reads: 35

```
[quote="MysticalDork, post:17, topic:100702"]
whether you’re using uart or PPM has no bearing on your battery/motor current settings.
[/quote]

This. 

I was super confused by this statement. 

[quote="ODBounty, post:12, topic:100702"]
so i cant really change the settings.
[/quote]

if you're using a vesc you can change settings. 

Unless you're using a diyeboard esc or a old rc car controller.
```

---
## \#19 Posted by: leroy Posted at: 2019-08-23T04:37:31.392Z Reads: 28

```
I would be asking mboards these questions, 
they may have seen this before, or at least know how to diagnose their hardware quickly.
```

---
