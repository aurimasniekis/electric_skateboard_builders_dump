# Benefits of higher switching frequency for vesc?

### Replies: 17 Views: 627

## \#1 Posted by: 12meterkuk Posted at: 2018-10-17T09:08:15.808Z Reads: 132

```
I’ve been reading some posts but it’s not clear to me as to how the higher frequency affects motor driver and motor. 

From my understanding it stresses the driver more but is more efficient?
```

---
## \#2 Posted by: Pedrodemio Posted at: 2018-10-17T14:04:56.896Z Reads: 119

```
A bit more since the MOSFET’s switch faster, so they heat up a few degrees more

But it’s definitely worth, using the default 20KHz you can clearly hear the motor, bumping to 30KHz the motor is almost silent, for me there was almost no difference between BLDC and FOC@20KHz

Wish I could bump a little further since I can still hear just a bit at 30KHz, probably a 15KHz harmonic
```

---
## \#3 Posted by: bevilacqua Posted at: 2018-10-17T16:03:59.620Z Reads: 105

```
Hi Pedro, since you are using V6s: I think I remember BV said that even 40khz worked fine for him. Maybe you can try 31khz and go up on small steps.
```

---
## \#4 Posted by: Pedrodemio Posted at: 2018-10-17T16:07:22.968Z Reads: 98

```
Thanks, I searched in his forum a few times but never found anything, I may try and see what happens

Will probably also use my measuring microphone to see if there is a difference in the spectrum
```

---
## \#5 Posted by: 12meterkuk Posted at: 2018-10-17T16:29:06.265Z Reads: 96

```
Does higher switching frequency kill vescs? I bumped mine from 20 to 25khz and man it was such an improvement. I’m really itching to push it up to 30 but worried about something breaking
```

---
## \#6 Posted by: bevilacqua Posted at: 2018-10-17T16:41:32.831Z Reads: 93

```
you might want to cool the drv chip as it might get hotter than at 20khz. Just a small copper heatsink with some silicone pad.

![Self-adhesive Pure Copper Heatsink For Raspberry Pi - Maker - Raspberry Pi - The Pi Hut - 1](https://cdn.shopify.com/s/files/1/0176/3274/products/IMG_0979e-900x600_1024x1024.jpg?v=1539021491)
```

---
## \#7 Posted by: 12meterkuk Posted at: 2018-10-17T16:44:00.355Z Reads: 92

```
Not sure if there’s space for it in a focbox, I’ll try to. 

I’ve read that the max switching frequency is around 40k before the vesc goes poof?
```

---
## \#8 Posted by: bevilacqua Posted at: 2018-10-17T16:46:23.315Z Reads: 90

```
im not sure either.... I'd do it on a V6, but rather not on 4.12 HW
```

---
## \#9 Posted by: 12meterkuk Posted at: 2018-10-17T16:47:58.299Z Reads: 89

```
Alright... I’ll test mine out @ 25khz for a few days... it feels plenty fine but if the benefits outweigh the cons of going up im definitely going with 30khz.
```

---
## \#10 Posted by: bevilacqua Posted at: 2018-10-17T16:53:52.336Z Reads: 84

```
30khz worked fine even on my maytech 4.12 vesc (C18 modded). Should a cake for the focboxes. Above that is untested territory. Better ask deodand or someone with more experience on esc hardware :smile:
```

---
## \#11 Posted by: 12meterkuk Posted at: 2018-10-17T16:55:39.009Z Reads: 82

```
@Deodand hey man would be great if you could chime in on this, thanks
```

---
## \#12 Posted by: Surfer Posted at: 2018-10-17T17:00:48.655Z Reads: 80

```
That's interesting, I can't feel any differences upping to 30khz on Raptor2
```

---
## \#13 Posted by: Pedrodemio Posted at: 2018-10-17T17:06:00.010Z Reads: 82

```
Maybe due to the hub construction the urethane dampen the higher frequency vibrations
```

---
## \#14 Posted by: Hummie Posted at: 2018-10-17T18:05:39.369Z Reads: 77

```
I think the feel would be super subtle and more so the benefit is noise reduction 


It's an on and off event as apposed to a switching of polarity.  30khz seems to silence everything and can’t imagine why youd want to go higher unless u had a very high kv motor that had low inductance and it was hard to get the pulse train to become smooth and consistent  and I think that’s its main purpose. So if u can feel the subtle switching frequency pulses maybe ud be more efficient w it higher as otherwise you’d be experiencing torque ripple.  Maybe

Raptor has very low kv n wouldn’t feel torque ripple even w a low switching frequency as the high inductance smoothens the pulse train
```

---
## \#15 Posted by: Deodand Posted at: 2018-10-17T20:17:05.188Z Reads: 76

```
Edit: TLDR; 30 kHz is fine on most nice hardware, your efficiency may either go down or up. It depends on the motor (winding resistance, inductance) , and the vesc (switching losses). The math is extremely complex to calculate since there are about 5 phenomena that contribute. If it sounds better and works fine its probably fine. I wouldn't advise above 30kHz. 

Don't have a ton of time today here is a non-comprehensive list of things that can limit max switching frequency:

There's a few factors playing into the switching frequency limitations. The first is that the VESC FW runs the control loop at 1/2 the switching frequency. If the switching frequency gets to fast the control loop doesn't finish in time before the start of the next cycle. On a standard vesc this happens around 35-60 kHz, depending on if you sample low and high side or just low-side. Your vesc will freeze up whenever the motor is spun up and become non-responsive but the idle (no motor current loop) executes faster so you can revert it after you turn it up too high usually. 

The second factor is switching losses, dead time, and sample window time. These are more complicated electrical phenomena that will be different on every set of hardware. Gate capacitance, Gate turn on voltage (the knee) and gate drive current/gate resistors all play into how quickly the FETs can be switched on and off (among other things). More powerful fets generally have a higher gate capacitance and thus either take more time to turn on or take more drive current. The DRV8301 has a maximum 1.7 amp drive current which is always used so for most Vescs the drive current will be 1.7 amps. This means depending on the FETs used there will be different turn on times for the FETs. These turn on times cause losses in the FETs everytime they are switched on and off since they pass continuously from a very high resistance (open circuit nearly) to a very low resistance (Rds on, usually a few milliohm). Besides the losses the switching times also mean you need to leave a small dead time between switching to make sure you don't short power and ground through the FETs, in general the larger the switching time the larger the dead time needed. More dead time will reduce the maximum applied voltage the motor driver can apply, usually knocking off a few percentage off the source voltage. The final thing I mentioned is sample time. You'll notice the vesc has a maximum duty cycle of 0.95, it uses the last 0.05 duty cycle for sampling with ADC, if you increase the switchting frequency this last 0.05 window becomes shorter as well, making a tighter sampling window. It may mean you need to decrease the maximum PWM duty cycle if the sampling doesn't have enough time to get an accurtate sample. You'd notice this as really poor performance at the maximum duty cycle. 

A final point here would be to look at the R-L characteristics of your motor. Your motor windings [have a time constant](https://www.electronics-tutorials.ws/inductor/lr-circuits.html) (Just divide motor winding inductance by motor resistance) so at a certain switching frequency (about (10x time constant)^-1) it doesn't much matter if you switch any faster because the motor winding current can't physically change  any quicker.
```

---
## \#17 Posted by: bigdog Posted at: 2018-11-09T09:48:58.775Z Reads: 51

```
[quote="Deodand, post:15, topic:71510"]
I wouldn’t advise above 30kHz.
[/quote]

would it die if i change it to 40kHz ?:joy:
```

---
## \#18 Posted by: 12meterkuk Posted at: 2018-11-11T13:07:30.327Z Reads: 36

```
Anyone know what happens when turn up minimum switching frequency for Bldc from 3khz to something like 15khz other than being less audible? Any potential to damage the vesc ?
```

---
