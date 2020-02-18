# Torque HUBS with 130KV and 12S (50V)

### Replies: 13 Views: 900

## \#1 Posted by: nordlicht Posted at: 2018-03-28T09:29:58.186Z Reads: 176

```
Hi,
I'm confused by the diyelectricskateboard page.

Info 1:
>TORQUE Hub 130KV is recommended for 6S battery setups and under. 8S should be ok.

Info 2:
>130KV for 6S is 20mph. 130KV for 12S is 30mph.

Ralph from the support said they recommend only 6S on 130KV motors and gave this reason:

>Only 6S.
Our VESCs can't sustain higher voltage. 

Which is weird because the VESCs do sustain the voltage on other motors?
And even tho they say "8S should be ok." Ralph said "**Only** 6s", which looks odd to me aswell.


Do you guys have experience with running 130KV motors on more than 6s? Maybe even the torque ones? Could you speculate what the reason for this recommendation would be? Do they get too hot or something similar?

Cheers
```

---
## \#2 Posted by: PXSS Posted at: 2018-03-28T11:53:14.272Z Reads: 150

```
Erpm is most likely the issue. Depends on the motor poles...
```

---
## \#3 Posted by: Sn4pz Posted at: 2018-03-28T12:19:56.226Z Reads: 138

```
hey, ive had the 130kv motors on my space cell pro 4 before it bit the dust, and i know the motors werent the issue, i was just careless. Seems possible but maybe lower the power of the motors themselves in the BLDC tool, I think thats what I did.
```

---
## \#4 Posted by: Acido Posted at: 2018-03-28T12:54:52.116Z Reads: 131

```
Hub motors are around 70kv, as i know, not the expert on hubs
```

---
## \#5 Posted by: Sn4pz Posted at: 2018-03-28T13:32:29.139Z Reads: 123

```
They can be wound for either. Toruqeboards does both, and I think evoHax(cant rememer his user) has some hubs with hummie that can be customized to whatever you want :)
```

---
## \#6 Posted by: TarzanHBK Posted at: 2018-03-28T13:38:20.194Z Reads: 117

```
Torqueboards hubs have 14 pole pairs so:

eRPM = (voltage)x(kv rating)x( pole pairs)

= 6s x 3,6V x 130kv x 14pole pairs = 39312 erpm

= 8s x 3,6V x 130kv x 14pole pairs = 52416 erpm

= 10s x 3,6V x 130kv x 14pole pairs = 65520 erpm - so already a bit over the 60000 limit of the vesc.
```

---
## \#7 Posted by: TarzanHBK Posted at: 2018-03-28T13:40:06.494Z Reads: 110

```
= 12s x 3,6V x 130kv x 14pole pairs = 78624 erpm - too much for the 4.12 hardware

Doable if you limit erpm to 60000 or use a 6.x hardware, where you can go way more up, before blowing something
```

---
## \#8 Posted by: Namasaki Posted at: 2018-03-28T21:26:35.614Z Reads: 93

```
[quote="TarzanHBK, post:6, topic:50420"]
Torqueboards hubs have 14 pole pairs so:
[/quote]

So they have a total of 28 magnets ?
Must be some small magnets.
```

---
## \#9 Posted by: nordlicht Posted at: 2018-03-29T08:07:48.458Z Reads: 77

```
Thanks! Really helpful. I'll go with 8s6p than, because I originally bought 50 cells for 12s4p.
```

---
## \#10 Posted by: torqueboards Posted at: 2018-03-29T08:17:13.504Z Reads: 77

```
@nordlicht These are out of stock. We're working on finishing a design up for a new one.

It's gonna be.... :night_with_stars: VS :sun_behind_small_cloud:

:fire: :+1::muscle::zap:
```

---
## \#11 Posted by: TarzanHBK Posted at: 2018-03-29T11:02:13.274Z Reads: 71

```
But the 130kv were 14 poles pairs and how many magnets?
```

---
## \#12 Posted by: torqueboards Posted at: 2018-03-29T22:35:15.077Z Reads: 59

```
@TarzanHBK 14/12 for the 130KV Hub Motors.
```

---
## \#13 Posted by: nordlicht Posted at: 2018-04-02T20:35:05.204Z Reads: 43

```
@torqueboards Thanks, but I already have em liing here. One of which has no working hall sensor (got full refund from , so I'm not too mad, even tho it was a fight..) and I think about opening the motor to check if there is just a bad soldering on the sensor or something.
I'm 100% sure that its the sensor, I checked the cables with an oszi (can even provide video of the wiring and the oszisignal) and the HUBs never touched the ground.

Got a few question

1) Is it likely that I can repair them on my own? I'm almost done studiing mechatronics, so knowlegde is there. Do you think its likely that its just a bad soldering?

2) Can I open the motor without breaking it? Can you give me some advise, without garuantee or anything? Searched for videos of ppl opening them and couldn't find :confused: 

Would appreciate help a lot!

Nordlicht
```

---
