# Focbox cogging in start up Help!

### Replies: 26 Views: 521

## \#1 Posted by: Davide Posted at: 2018-10-14T17:10:53.963Z Reads: 115

```
Hey there! I'm coming here to y'all for advices.
I got this APS mountain board (chinese stuff I reckon) and that's where I fell in love with this hobby and I get addicted to it.
So last weel I decided to switch to focboxes as I heard very good things, and the stock escs where just terrible, and they are actually working fine! But I got a problem, for some reason the motors cog on startup and afterwards they are just fine, no problems at all. And weird thing, is if on the bench I pull the trigger the focboxes seems to me that aren't really working together on low A ( see video attached).
My setup is 
10s5p 10Ah 10C battery
2×1650 watt stock motors ( which I'm gonna change for 2 Overion or Unikboards  sensored motors)
The setup of Focbox is
FOC unsensored
40A motors 40A battery
Ackmaniac Firmware
[https://youtu.be/8l2-nhr9yA8](https://youtu.be/8l2-nhr9yA8)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-14T17:15:25.292Z Reads: 110

```
You run unsensored motors.
Give your board a kick when start up and you good to go.
There are lots of threads about it.
The same about the phenomenon that the motors not start spinning at the same time.
The search function is your friend 😉
```

---
## \#3 Posted by: threebysix Posted at: 2018-10-14T17:40:56.320Z Reads: 104

```
nothing wrong with your focbox  because you are running unsensored motors. Either push start or go extra on the throttle when starting.
```

---
## \#4 Posted by: Davide Posted at: 2018-10-14T18:00:22.197Z Reads: 95

```
I actually read heaps of em, but I missed out that!! But why the vesc is having troubles with unsensored and the crappy esc was working fine? Do they work in such a different way?
```

---
## \#5 Posted by: Andy87 Posted at: 2018-10-14T19:20:17.404Z Reads: 84

```
I never had one of the cheap Chinese esc, so I can’t say what’s different with them. Maybe they have a stronger start up current or something like this.
Just can say from my experience with a vesc it was always like this if I ran unsensored. More in bldc than in FOC. Your motors need to rotate a bit and after it runs very smooth.
```

---
## \#6 Posted by: Davide Posted at: 2018-10-14T19:25:04.173Z Reads: 79

```
Thanks man, I really love this community, there's lots of stuff to learn!! Do you have any raccomandations for sensored motors for an emtb build? I think I'll go with low kv, something like 130 and 3kw, do you have any suggestions for good choices? I read something about wiring of the motors but I'm still confused about it, I saw some APS motors that are pretty good to me...
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-14T19:26:59.424Z Reads: 78

```
Where you from, us or eu?
```

---
## \#8 Posted by: Davide Posted at: 2018-10-14T19:28:04.239Z Reads: 78

```
I'm from EU
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-14T19:38:12.975Z Reads: 75

```
I would go with this ones
https://www.unikboards.com/fr/boutique/moteur-skateboard-electrique-6374/

They sealed and sensored so no issues with shorted sensors or dirt inside the motor.
They sell them in 130 and 150kV and if you need support or have problems you can always ask @okp . He is the owner and also here 😉
```

---
## \#10 Posted by: Davide Posted at: 2018-10-14T19:41:17.551Z Reads: 71

```
Thanks a lot!!
```

---
## \#11 Posted by: telnoi Posted at: 2018-10-14T20:04:49.260Z Reads: 64

```
There is a very realistic chance that the motor bolt pattern is different compared to the motors you currently have. You most likely also have a 10 mm shaft where the Polaris have a 8 mm shaft.
```

---
## \#12 Posted by: Andy87 Posted at: 2018-10-14T20:15:38.742Z Reads: 62

```
Like @telnoi said it’s likely that your old motormounts will not fit the 6374 motors.
1650watt sound like 50xx motor size or something like this. If it is it’s definitely not fit and you need new mounts too.
Check also the diameter of your shaft.
The unik ones are 8mm and you know it’s shitty if you get all your stuff and than realize that you can’t drive because the motor pulley doesn’t fit 😅 the right size of pulleys you can find on the Unik side too.
```

---
## \#13 Posted by: telnoi Posted at: 2018-10-14T20:24:05.305Z Reads: 59

```
That board is almost identical to this, slightly newer motor mount. It took a fair bit of work to get it up to somewhat acceptable standards.

https://www.electric-skateboard.builders/t/ninestep-diyeboard-l-faster-8-mountainboard-trucks-electronics-review/46955
```

---
## \#14 Posted by: Andy87 Posted at: 2018-10-14T20:24:36.916Z Reads: 56

```
The link not working
```

---
## \#15 Posted by: telnoi Posted at: 2018-10-14T20:25:05.315Z Reads: 56

```
Fixed 10 chars
```

---
## \#16 Posted by: dareno Posted at: 2018-10-14T21:00:06.060Z Reads: 53

```
Did you do a detection on both motors?
```

---
## \#17 Posted by: mynamesmatt Posted at: 2018-10-15T00:12:45.631Z Reads: 52

```
i'd personally go for the SK8 motors from hobbyking. they have multiple versions of the 6374, have a look at em
```

---
## \#18 Posted by: Davide Posted at: 2018-10-15T04:43:57.060Z Reads: 46

```
It's a 6355, so I thought I should be fine but I gotta check🤔🤔
```

---
## \#19 Posted by: Davide Posted at: 2018-10-15T05:00:55.146Z Reads: 42

```
Yep, I've seen it! They are pretty much the same except for different ESC battery and motors..  and I know there'll be lots of work involved, but I like this challenge😉
```

---
## \#20 Posted by: Davide Posted at: 2018-10-15T05:02:06.086Z Reads: 41

```
If motors are 6355 the bolts on the motor mount shold be the same, aren't they?
```

---
## \#21 Posted by: Davide Posted at: 2018-10-15T05:02:42.116Z Reads: 41

```
Yep I did!
```

---
## \#22 Posted by: Andy87 Posted at: 2018-10-15T05:04:50.851Z Reads: 41

```
Usually yes, if they standard pattern.
If you want I can measure it out in the evening when i‘m back from work.
```

---
## \#23 Posted by: Andy87 Posted at: 2018-10-15T21:22:33.630Z Reads: 35

```
A bit late but here you go, the standard pattern for 63xx motor size 
![image|375x500](upload://chuZcojSqonflR5nvsv8Q3SFRr8.jpeg) ![image|375x500](upload://vQn6nTIEWGAYHFLGZVc9RnSQZmg.jpeg)
```

---
## \#24 Posted by: Davide Posted at: 2018-10-16T04:56:05.412Z Reads: 29

```
Thanks mate, I'm gonna check out these days!!
```

---
## \#25 Posted by: lrdesigns Posted at: 2018-10-16T05:15:05.688Z Reads: 29

```
You can increase the minimum amps from the default 0.1 amp to 1-3 amps it can help smooth out start up without sensors. Still wont be perfect but can make it hesitate less. 

![image|690x198](upload://bgz6KEBVUn56aVKoPyHLa2V60bt.png)
```

---
## \#26 Posted by: Davide Posted at: 2018-10-16T18:30:22.414Z Reads: 24

```
Ok, it ain't a solution, but I can start from standstill uphill!! Thanks for the advice, it's waaay better... at least I can enjoy my ride till I won't get motors!
```

---
