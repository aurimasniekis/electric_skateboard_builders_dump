# Would extra capacitor on esc help with voltage sag?

### Replies: 31 Views: 3224

## \#1 Posted by: leven Posted at: 2017-08-15T12:04:21.219Z Reads: 256

```
Hi,

Is 'upgrading' the capacitors something that could help with voltage sag?

Been reading about capacitors and inductance and the capacitors role, and thinking about changing my current ESC's 63v 470uF single capacitor to two quality 63v 1000uF in parallel (like the vesc).

I have a 10s2p 18650 battery and I think in seeing voltage-sag sometimes, mainly uphill.
```

---
## \#2 Posted by: Cobber Posted at: 2017-08-15T12:25:47.949Z Reads: 252

```
Caps on your ESC leads help with battery wire induced inductance spikes...  they will help with smoothing out spikes, you going WOT, your motors drawing peak and it taking time for the current to hit your motors from your batteries and you adjusting...

As I understand it

SAG on the other hand comes from the "c" rating of you batteries not being able to provide the amps your motors want.
```

---
## \#3 Posted by: sl33py Posted at: 2017-08-15T12:34:41.011Z Reads: 239

```
Agree with @Cobber.  The smoothing ability of caps is not going to help with voltage sag.

You will see sag if your setup current capacity (delivery of amps) in C is insufficient.  

I guess theoretically you could do a huge cap bank, but not very feasible or practical.  Caps are good at delivery power in milliseconds - not seconds long delivery under heavy load...  As I recall with my limited understanding (not an EE).

I would instead work on a better battery solution - add more in parallel to reduce sag.

HTH - GL!
```

---
## \#4 Posted by: leven Posted at: 2017-08-15T13:14:43.916Z Reads: 213

```
Ok thanks!

Panning a bigger battery as well, but that will take time.

Deciding between LG HG2 (3000nah) or Sayno (3500 mah) to make a 10s3p, but that probably won't happen until vinter.
```

---
## \#5 Posted by: DeathCookies Posted at: 2017-08-15T13:19:22.209Z Reads: 191

```
[quote="leven, post:4, topic:30702"]
Sayno (3500 mah)
[/quote]

Seems like the 10A continous discharge Version? If so it is much too less for eboard ing a 10S3P configuration. Then i would recommend the HG2!
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-08-15T13:23:27.444Z Reads: 177

```
something that might help with sag is a smaller 1P pack in parallel and in front (as in closer to the ESC, not in series) of the main pack, using cells with a more explosive discharge curve. 

it would have the advantage of providing the immediate current for acceleration when needed and just sitting there generally contributing when cruising, ideally...

wired parrallel with the main side's balance leads may also keep it balanced with the main packs's voltages. 

just a crazy idea.
```

---
## \#7 Posted by: ugothakd Posted at: 2017-08-15T17:15:52.651Z Reads: 147

```
A crazier idea is supercapacitors. Would take too much space at the moment, though..
```

---
## \#8 Posted by: leven Posted at: 2017-08-15T17:31:59.251Z Reads: 143

```
yeah that is a crazy idea ;)

So do you mean a extra pair of wires back to the battery or do you mean a 10s1p pack at the front with positive to mainpack-positive and negative to mainpacck-negative?

what cells would be good for that?
```

---
## \#9 Posted by: treenutter Posted at: 2017-08-15T17:52:57.727Z Reads: 140

```
@longhairedboy have you tried this?
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-08-15T17:55:28.519Z Reads: 139

```
no i have not. It just came to me in a blur of delerium. 

@leven i don't know.. something that can handle tons of abuse and has a high discharge rate.
```

---
## \#11 Posted by: sl33py Posted at: 2017-08-15T18:46:22.005Z Reads: 132

```
Unless you need monster range - i'd instead recommend a higher C cell (more current/amp delivery capacity), with smaller mAh capacity.

I'd recommend the 2600mAh VTC5a (25A capacity tested), or 30q (20A tested iirc).  

7.8Ah * 42v = 327Wh = ~32km/20mi
9Ah * 42v = 378Wh = ~37km/23mi

Rought estimate of 10Wh=1km.
```

---
## \#12 Posted by: longhairedboy Posted at: 2017-08-15T18:57:23.908Z Reads: 133

```
30Q is 15, you want the 25R for the 20 amp rated. 

The 25R is a great cell for mid-large, high discharge packs. ITs basically perfect for a 4P at 20amps continuous and 100amp pulse. I went with 30Qs on my 5P because more cells means each one can do less for longer and the range dramatically increases because of it.
```

---
## \#13 Posted by: leven Posted at: 2017-08-15T22:47:13.445Z Reads: 116

```
Ok, thanks, but isnt LG HG2 a high discharge cell as well? It has 20amp maximum and 3000mah.

VTC5a is interesting, i have been looking att Sonys VTC6 3000mah but they are a bit expensive.
```

---
## \#14 Posted by: sl33py Posted at: 2017-08-16T10:13:27.482Z Reads: 107

```
Hey LHB - i thought it was "rated" at 15, but actually ran much higher output?

[img]https://farm2.staticflickr.com/1602/24717095646_0db75f906d_o.jpg[/img]
```

---
## \#15 Posted by: longhairedboy Posted at: 2017-08-17T11:14:33.979Z Reads: 92

```
Its true. I feel like all the samsungs perform higher than specced in a lot of cases.
```

---
## \#16 Posted by: darkkevind Posted at: 2017-08-17T12:25:43.529Z Reads: 89

```
Technically you could use a super capacitor between the battery and the ESC that has the ability to expel a much higher current than your batteries, in much the same way as the lipo/li-ion based spot welder does.

The super cap will need time (not that much) to reach full capacity, then when you need a burst of power it can supply it, all while getting topped back up by the slower, less current providing cells. This could even out the voltage/current supply from your battery and ultimately stop voltage sag. But it could only be sustained for short bursts.
```

---
## \#17 Posted by: longhairedboy Posted at: 2017-08-17T12:47:07.128Z Reads: 85

```
This is something we've been thinking about doing actually. It could potentially eliminate the effects of sag completely. Finding the right form factor has been difficult though.
```

---
## \#18 Posted by: darkkevind Posted at: 2017-08-17T13:04:37.636Z Reads: 87

```
Well, we'd need flat and long and at the moment they're all round and very fat! :/
```

---
## \#19 Posted by: longhairedboy Posted at: 2017-08-17T13:19:33.252Z Reads: 89

```
that is correct. We need one in the form factor of either an 18650, a 26650, a prismatic, or one of those new 207xx cells and i don't think materials science is quite there yet, and if it is, the demand hasn't been recognized. I have about 4-6 cubic inches of space for it, so they need to get on it.
```

---
## \#20 Posted by: toma Posted at: 2017-08-17T13:31:53.868Z Reads: 87

```
I've tried the big capacitor thing... it helps, but only slightly. 


<img src="/uploads/db1493/original/3X/e/6/e64a757b0f7963d9862423bf8b67304666ac89db.jpg" width="666" height="500">

Those were the two biggest capacitors I could find at my local hackspace.
```

---
## \#21 Posted by: Cobber Posted at: 2017-08-17T14:49:25.360Z Reads: 84

```
How would a _super capacitor_ effect your esc...
I know from reading the rc forums multiple small high voltage/ low resistance caps are best for taming inductance induced spikes?
```

---
## \#22 Posted by: TehAtheist Posted at: 2017-08-17T15:44:18.949Z Reads: 80

```
People saying the so called "super capacitors" would help, are **not** correct.

- **Voltage sag:** Voltage drop at battery connector due to drawing high current, occurs at every voltage, increases when battery depleted.

When adding a capacitor, you're practically adding a battery with a high C rating, but with such small capacity that it won't matter. In less than 250ms the capacitor would be at a to low voltage and battery current will rise just as if there was no capacitor. So unless you plan on accelerating for times less than 250ms, this idea is not viable.
```

---
## \#23 Posted by: darkkevind Posted at: 2017-08-17T15:58:53.258Z Reads: 79

```
There are super capaciters that deplete their capacitance much slower than that...

You're going to ask me for evidence but for the life of me I can't find it! :frowning: :confused:

Trust me, there is.....
```

---
## \#24 Posted by: darkkevind Posted at: 2017-08-17T16:09:34.064Z Reads: 77

```
Although this article is about Ultra-capacitors (which could still be used), they talk about using in EVs for sudden short bursts of current, such as this use case...

https://gigaom.com/2011/07/12/how-ultracapacitors-work-and-why-they-fall-short/
```

---
## \#25 Posted by: TehAtheist Posted at: 2017-08-17T16:36:23.496Z Reads: 77

```
Hmm, nice find.

Let's say you get your hands on a 500F capacitor for 8S battery though. (Probably would cost you around €1000). Calculating this fast, would let me guess this would give you 1 minute 15 seconds of acceleration power, until the capacitor is depleted to a voltage level insufficient to let the motor spin at a decent speed. (As the motor's speed is in direct relation to its voltage, unless it's current is limited). If we calculate generously, we may say minute and a half. (This calculation is made for a current draw of 30A, which is what my board draws when acceleration full throttle.)

You would also need this time to charge it back to full voltage with a 30A current, although to prevent the voltage sag I suppose you want this lower than the amps you're using the capacitors for, right? So let's say 15A, which would require 3 minutes to charge the capacitor again.

No matter what scenario you write down, the time to charge the capacitor will always be higher than the time you accelerate, don't you think? In the case the capacitor is depleted, the battery would be providing current to charge the capacitor + power the motors and would be limited by the charge resistor for the capacitor to the previously selected 15A. I suppose the motor would receive half of that (not quite sure).

Anyway, I don't know enough about this to give a definite answer, but I can pretty much conclude for myself that this is a bad idea. For the price, you'd be better of buying good batteries with low voltage sag ;).
```

---
## \#26 Posted by: darkkevind Posted at: 2017-08-17T16:43:26.691Z Reads: 72

```
You could always buy several smaller capacitors and parallel them...

Caps get charged very quickly, I think you're underestimating the speed in which they charge back up. Also, if someone were to create a 'smart' battery, electronics could turn on and off the capacitor as and when it's needed. You're not going to hard accelerate for more than a few seconds at a time, when the draw goes over a threshold, in kicks the super cap, when it eases, switch back to the cells, all the while the cells are charging the caps up at the highest rate they can cope with without sagging... I'M A GENIUS!!! Someone needs to make these 'smart, super-cap-ion' battery packs!! lol
:D
```

---
## \#27 Posted by: TehAtheist Posted at: 2017-08-18T12:19:25.940Z Reads: 68

```
It'll still be around the same price then, cause that's the only option as far as I've seen. (And you'll have to put them in series instead of parallel, as the voltage they're built for is the issue. So your capacity will stay the same but possible voltage will be higher.)

And yes they do, but only in figure of speech (Well, they're faster than batteries, but if it's not faster than discharging then I'm not going to call it fast.). They charge as fast as they discharge, and because regular capacitors only have low capacity, they appear to charge very fast. In practice it's 4-5 times the RC (Resistor 
 to limit charge current X capacity) coefficient. Where after 1 x RC coefficient, it already reached 63% of it's maximum voltage. But after 2 x RC it reached 86% then 95% and then 98%. This means that because the raise in voltage, the voltage difference between the battery and the capacitor decreases, resulting in a drop in charge current and slower charging the higher the capacitor voltage will be.

That's why the calculated times in my previous post are so low - and probably still estimated to good -.

But to be honest, it simply won't matter. The voltage drop on your battery will be significant once it's nearly depleted. Look at this graph, at the start your voltage will drop quite significantly, then it'll remain quite constant for some time and it'll appear as if you're barely losing charge. (For those with a % meter on their longboards, you'll be finding yourself in the 80%-40% range, but suddenly, after dropping below 40% it seems like your batteries break :p and they suddenly get to 10% really quick! But it's normal and putting capacitors in their won't benefit this, it won't matter.
<img src="/uploads/db1493/original/3X/1/b/1b449d7cbedc813892e28fb6fb183f4999c3c084.png" width="666" height="500">

But yeah, it'll prevent that a sudden acceleration makes the battery drop a few % for a few seconds. But I do not see this as an issue as long as your cutoff voltage is set conservative and this issue decreases if the C rating of your battery is higher.
```

---
## \#28 Posted by: darkkevind Posted at: 2017-08-18T12:25:00.717Z Reads: 59

```
But that's the point. Most voltage sage issues happen under hard acceleration, perhaps on some kind of incline. A lot of them result in a cut out in power. This can be potentially dangerous for the rider as they get catapulted forwards (it's happened to me!). This solution will effectively eradicate that issue.

The cap deals with the sudden draw of high current, then it peters out after a second or two where the normal battery resumes and has less current draw/load.
```

---
## \#29 Posted by: TehAtheist Posted at: 2017-08-18T12:40:04.307Z Reads: 57

```
If that issue is so significant, then you should limit the current, your batteries are simply not up for the task.
I don't see any gains for developing a capacitor system if you could just spend less money, for a battery setup that works just as great. A battery should be chosen with a C rating, offering a current minimal double of the current you'll maximum draw. My battery setup can deliver 125A and I've never had issues like this.

You'll perhaps also want to measure the resistance between your battery and VESC if you had issues. Perhaps a bad soldering causes a high resistance connection. If the total resistance of the cable, connections would be lets say 0.05Ohm, it would cause another 1.5V voltage drop at full acceleration in my case.

But if you were to develop something like this, I do want to check it out ;)
```

---
## \#30 Posted by: darkkevind Posted at: 2017-08-18T14:06:39.383Z Reads: 54

```
The difference between more cells in parallel could be as much as €100 depending on what cells you have. Some li-ion cells put out 42A but they're mega expensive.

I believe smaller less expensive caps in parallel will make this a cost effective solution.
```

---
## \#32 Posted by: Deckoz Posted at: 2017-09-05T21:43:33.844Z Reads: 41

```
If your gonna do anything. Figure out a cap+TVS solution for going downhill  and preventing over voltage during braking. Forget the cap for acceleration, get bigger/more batteries.
```

---
