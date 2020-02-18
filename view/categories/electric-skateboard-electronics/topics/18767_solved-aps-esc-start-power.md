# \[SOLVED\] APS ESC start power

### Replies: 10 Views: 1061

## \#1 Posted by: Davey Posted at: 2017-03-08T19:37:56.064Z Reads: 87

```
Hello there, 
I programmed my ESC (http://alienpowersystem.com/shop/esc/alien-120a-2-7s-ev-mini-esc-bec/) for my budget board and wondered what the "start power - CAR" setting means. I had it at 5% and the motor wobbled a bit at the start, but it was fine whilst driving. The thing that made me change the setting was the motor for taking too long to start. It needed about 3 minutes before I got any response from it. After I set the setting to "Auto" or "50%" the motor responded after no time (5 seconds), but accelerated harder, which is not good for me.
Does anyone know what this setting really does? Thanks
```

---
## \#2 Posted by: Sander Posted at: 2017-03-08T21:32:44.480Z Reads: 72

```
The setting let you choose how "strong" the minimum speed is.
Like how fast it shall go when you give it a little power.

It says itself. Start Power. How much power you want the ESC to give the motor on the first value of going foward
```

---
## \#3 Posted by: Davey Posted at: 2017-03-09T17:15:30.296Z Reads: 58

```
Yeah I got that. But why does the motor need longer to respond on lower start power? As I said if I pulled the trigger on my remote nothing happened, only after like 3mins the motor spun. On Auto/100% start power the motor spun directly after I pulled the trigger for the first time.
```

---
## \#4 Posted by: Sander Posted at: 2017-03-09T18:56:24.816Z Reads: 47

```
Maybe it is so low that the motor doesnt spin?
```

---
## \#5 Posted by: Davey Posted at: 2017-03-09T21:23:57.477Z Reads: 43

```
The motor spins fine after the 3mins of nothing...
```

---
## \#6 Posted by: Davey Posted at: 2017-03-11T17:40:32.681Z Reads: 40

```
UPDATE: I can't tell why the motor hasn't spun, but now I put the start power on "Auto" and it works fine. Acceleration is smooth and so on.
```

---
## \#7 Posted by: Tijmen Posted at: 2017-07-03T09:46:39.237Z Reads: 31

```
I have this problem of having to wait before the ESC does anything. How have you fixed this and what settings are you using?
```

---
## \#8 Posted by: Tijmen Posted at: 2017-07-03T13:59:42.076Z Reads: 24

```
@Davey What firmware are you running? I am now completely lost with this esc...
```

---
## \#9 Posted by: Davey Posted at: 2017-07-05T15:52:45.237Z Reads: 24

```
Hey @Tijmen, I use the SkLv_UV47 or CARLV_UV45, I don't know exactly wich one. But i guess the SkLv one. What problems are you having? Have you flashed your esc already? Which ESC are you using? 
And yes I also have to wait sometimes for the ESC to get started when turning my board on. Like 30-60s but then everything works.
```

---
## \#10 Posted by: Tijmen Posted at: 2017-07-05T16:26:12.254Z Reads: 21

```
Managed to get it to work. Installed some car firmware to it. The brakes are kinda weird though now. When I accelerate, then release throttle to neutral, and then accelerate hard again, the motor tries to stop for a millisecond because it turns the brakes on. When I turn braking to 0% this doesn't happen...
```

---
