# Couldn&rsquo;t an esc do?

### Replies: 9 Views: 799

## \#1 Posted by: Nix Posted at: 2017-09-01T20:17:57.200Z Reads: 132

```
If I monitor the discharge, and have the exact right specs for using a motor, couldn't I just use an esc?
```

---
## \#2 Posted by: dg798 Posted at: 2017-09-01T20:22:27.596Z Reads: 134

```
an esc is not configured for an eboard. It's meant for an rc car or boat.
it could blow up or fry up because of the weight, batteries or motor.
if i were you i would spend the money on a vesc and configure it for your motor and batteries.
i wouldn't go with an esc.
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-09-02T03:06:54.183Z Reads: 113

```
biggest issue with esc is weak brake. cuz it is made for 20lb rc where as human is like 150lb. when I was using esc before it dies from my mistake, I had to use reverse for my brake.
both has pro and con but to get esc performs same as vesc, it probably cost same if not more.

beside it is loud coggy and accelerate crazy
```

---
## \#4 Posted by: Cobber Posted at: 2017-09-02T03:42:24.599Z Reads: 99

```
& vesc 4.xx is know for cooking it's DRV chip...
all speed control solutions have pro/con
could get a vesc 6 but $$$
could get a hobbywing  max5/6... bullet/water proof but 8s...

One thing I wouldn't do is buy cheap or without research. The most expensive thing you buy is the thing you buy twice :wink:
```

---
## \#5 Posted by: Nix Posted at: 2017-09-02T13:27:25.260Z Reads: 69

```
@cobber You say the vesc 4.xx could fry... Meaning the 4.12... right... And what the difference between firmware and hardware? The torque boards vesc is hardware 4.12 so does that mean it'll probably fry?
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-09-02T13:38:44.296Z Reads: 68

```
Doesn't mean it'll probably fry.  I use the torqueboards vesc for 100 miles or so now with not a single issue.  My only warning is DO NOT use FOC with the torqueboards vesc.  I only recommend trying FOC with a FocBox or the @chaka vesc
```

---
## \#7 Posted by: Cobber Posted at: 2017-09-02T14:03:33.384Z Reads: 62

```
I'm not saying it will, but it could. A search of the forum yields the breadth of the communities experience. There is a reason [this](http://www.electric-skateboard.builders/t/vesc-drv8302-failures-and-repair-options/4201) thread is on the front page... 
The vesc 4.xx is very adjustable be careful how you set it up or it might destroy it self, running 12s & or FOC will narrow the range of usable settings.
But most people want to up their volts and reduce their amps... 
& they want to run FOC... 

[quote="Nix, post:5, topic:32042"]
And what the difference between firmware and hardware?
[/quote]

I say 4.xx because some have upgraded some physical parts of the hardware to compensate for past failures. These units generally cost more with slight advantage. But then you are well on your way to the price of a vesc6 which will run 12s and other advanced settings with no trouble.

It is a conundrum, there is no answer with it all.
```

---
## \#8 Posted by: Nix Posted at: 2017-09-02T15:40:11.951Z Reads: 53

```
With a 245 kv brushless out runner motor which has a max loading of 70Amps (but says max power is 2700w- {2700/24 = 112 amps - does this mean It can pull 70 amps or 112 safely?}) 24 v coming out of 6s battery... Either way it is so much more than 50amps of the vesc... Is this dangerous?
```

---
## \#9 Posted by: psychotiller Posted at: 2017-09-02T16:05:50.279Z Reads: 47

```
You can! Thing is, you sacrifice smooth acceleration, smooth braking, silence of operation, and in alot of cases safety. Remember, your board isn't a a toy. It's a vehicle. Acceleration and braking control shouldn't be overlooked unless you'd look better with scars. Most of us do!
```

---
