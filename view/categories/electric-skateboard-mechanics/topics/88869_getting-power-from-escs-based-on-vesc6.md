# Getting power from ESCs based on VESC6

### Replies: 17 Views: 524

## \#1 Posted by: DavidC Posted at: 2019-03-31T09:35:56.920Z Reads: 125

```
I've got two dual 12S mountainboard builds : 

1) ROXXY 9120-12 Opto + Turnigy Aerodrive SK3 - 6374-192KV + Turnigy Graphene 6000mAh 6S 65C (all dual) + gear ratio 5 (gears 12/60)

2) Dual FSESC6.6 + Turnigy SK8 6374-192KV Sensored +  Turnigy Graphene 6000mAh 6S 65C (all dual) + gear ratio 5 (chains 8/40)

The Dual FSESC6.6 build really feels underpowered. Motors have quite same specs. Lipo are the same. Gear ratio is the same. So I think this ESC based on VESC6 is guilty.

VESC-Tool 2019 1.06 says I can put 67A into the Turnigy SK8 6374-192KV motors. I tried Motor/Battery max 67A, 70A, 80A and 90A. I get strator saturation with 90A so I set below. 

I did not manage to get more than 51A from the Lipo (Battery max current). There's a lack of power, and delay when pulling the trigger before getting it. I set Positive Ramping Time to 0,10 but it's not enough.

When looking at Jens (E-TOXX) videos relating to VESC6, I can not believe he uses the same kind of ESC, even though I know he uses bigger motors from Leopard or APS.

So, is it possible that this VESC6 based ESC from Flipsky is not as good as original VESC6 from Trampa?

Other question, should I increase Absolute Maximum Current? to 200 or 250 with Battery/Motor Current Max 80A?
```

---
## \#2 Posted by: deucesdown Posted at: 2019-04-05T12:34:25.381Z Reads: 98

```
https://www.electric-skateboard.builders/t/e-toxx-directdrive-vs-trampa-vesc6-vs-leopard-8072-170kv-vs-nowind/30822/87

I remember nowind complaining about vesc being lame until he installed the unlimited firmware and changed some settings. Maybe dig around in his threads? And post here what you find :)
```

---
## \#3 Posted by: Pedrodemio Posted at: 2019-04-05T12:57:04.784Z Reads: 90

```
Check your ramping time for acceleration and braking, set both to zero for maximum punch
```

---
## \#4 Posted by: deucesdown Posted at: 2019-04-05T12:58:15.895Z Reads: 89

```
[quote="Pedrodemio, post:3, topic:88869"]
ramping time
[/quote]

ramping is only for bldc mode, right?
```

---
## \#5 Posted by: Pedrodemio Posted at: 2019-04-05T13:00:49.218Z Reads: 87

```
No, works for all, the one I’m saying inside the ppm or nunchuck settings 

Just be careful that it can throw you off, I never tried 0, but even going from the default to 0.2 I almost kissed the road
```

---
## \#6 Posted by: taz Posted at: 2019-04-05T13:26:36.808Z Reads: 87

```
The motors may have the same specs but I am not sure this also applies to their performance.
I am still on the fence about the SK8 motors as they don't feel as strong as the Maytech 6374
```

---
## \#7 Posted by: rich Posted at: 2019-04-05T16:29:28.137Z Reads: 83

```
[quote="Pedrodemio, post:3, topic:88869, full:true"]
Check your ramping time for acceleration and braking, set both to zero for maximum punch
[/quote]


Did you try zero? My minimum was 0.1 but would like to try 0.01 for positive ramping time. I'm afraid this could be bad for the Vesc because the tutorial says changements between 0.1 and 0.9. That's why I never tried it, do you think it's safe?
```

---
## \#8 Posted by: Pedrodemio Posted at: 2019-04-05T17:12:00.532Z Reads: 74

```
@trampa can confirm, I remember a discussion on the Vesc project forum

I lowered it to make the throttle more responsive when going to full acceleration to full brake, I actually prefer it a bit smoother
```

---
## \#9 Posted by: taz Posted at: 2019-04-05T17:16:49.229Z Reads: 76

```
From this post it seems you are using an older version of the vesc tool that activated temperature compensation by default and caused various problems. I had that happen too.
https://www.electric-skateboard.builders/t/vesc-motor-detection-database/88020/13?u=taz

https://www.electric-skateboard.builders/t/all-new-2019-vesc-tool-release/83619/423?u=taz

Update your firmware and it will most likely solve your problem
```

---
## \#10 Posted by: pookybear Posted at: 2019-04-12T17:51:08.629Z Reads: 67

```
@DavidC 

I'm experiencing the same. Have you gotten this resolved?
```

---
## \#11 Posted by: DavidC Posted at: 2019-04-12T22:46:30.579Z Reads: 63

```
I tried what @deucesdown said but I got no clues from @nowind's thread about getting more power.

I don't need it smooth, I have footstraps. I just need punch in the face :rofl:

Tomorrow I'll try almost vertical throttle curve.

@taz I use @ackmaniac latest firmware. I feel it overperforms official firmware imho.

About (as if) lost current I wonder if vedder's antispark switch could steal current. It's the only thing between the Lipos and the FSESCDUAL. If it does then it would change current into heat. The antispark is inside a box but I don't think it gets hot. Maybe I'm wrong…
```

---
## \#12 Posted by: Nowind Posted at: 2019-04-13T12:42:13.714Z Reads: 57

```
[quote="DavidC, post:11, topic:88869"]
I don’t need it smooth, I have footstraps. I just need punch in the face :rofl:
[/quote]


Thats my brother :sunglasses: :heart_eyes:
```

---
## \#13 Posted by: DavidC Posted at: 2019-04-13T21:22:45.704Z Reads: 50

```
Thanks Jens!

Got the feeling to have more power this way : 

- Motor Current Max : 100,00 A
- Motor Current Max Brake : -60,00 A
- Battery Current Max : 100,00 A
- Battery Current Max Regen : -60,00 A

- Max ERPM : 100000,00

- Positive Ramping Time : 0,10

- Throttle Expo : 25%
- Throttle Expo Brake : 10%
- Throttle Expo Mode : Exponential

Way more fun!!
  
Anyway, this FSESCDUAL6 didn't want to pull more than 66 A (I'd prefer 666).

While riding with the ROXXYs Lipos are warm at the end. With the FSESCDUAL6, the Lipos stay cool… Why that thing doesn't want to pull the resquested amps… :hear_no_evil:
```

---
## \#14 Posted by: pookybear Posted at: 2019-04-13T22:52:49.689Z Reads: 45

```
Damn. I'm no way near those settings. Looks like I need to bump up mine way more.
```

---
## \#15 Posted by: taz Posted at: 2019-04-14T18:22:39.475Z Reads: 43

```
Don't your motors overheat with these settings?
```

---
## \#16 Posted by: DavidC Posted at: 2019-04-14T21:14:52.948Z Reads: 38

```
A bit… but with heavy abuse only. No big deal.

What's weird is the temperature of the same Lipos after the same ride : 
- w/ ROXXYs : 40°C
- w/ FSESCDUAL6 : 28°C.
```

---
## \#17 Posted by: pookybear Posted at: 2019-04-15T04:00:38.136Z Reads: 37

```
FYI. 

POS ramping to 0.1 helps a ton!
```

---
