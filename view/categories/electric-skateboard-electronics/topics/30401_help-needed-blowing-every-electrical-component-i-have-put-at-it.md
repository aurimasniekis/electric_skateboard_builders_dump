# Help needed &#124; Blowing every electrical component I have put at it

### Replies: 19 Views: 720

## \#1 Posted by: Trdolan03 Posted at: 2017-08-12T04:39:09.139Z Reads: 96

```
 Here is my dilemma,  
 I am currently running a dual 6374 motor setup with a 12s 10.4amp LIPO battery and the dual APS ESC. 
I started with the 120a DIY switch and blew that after 5 minutes. Then switched to a key loop as suggested as it is the most rugged option and blew the ESC. I got it fixed and then put in a 150a breaker after which 5 minutes that blew. I am using 10 guage wire throughout and xt90 connectors. Any ideas? 
Thanks,
Thomas
@okp @Okami @psychotiller @onloop @Idea
```

---
## \#2 Posted by: JLabs Posted at: 2017-08-12T04:43:55.445Z Reads: 91

```
How are your solder connections? 10awg wire can not handle 150a so I'm guessing you had some cold solder joints. Can you post some pics of your setup?
```

---
## \#3 Posted by: Trdolan03 Posted at: 2017-08-12T04:46:28.592Z Reads: 90

```
<img src="/uploads/db1493/original/3X/6/f/6f98b429d25b48db66ddf03bc2ce44af5eca4302.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/d/ed2bb1dfb0dd702e41f117d5dc725cfae8000bc7.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/7/9/795363a8e63498cb9fe08ac310d621274fe8d76f.JPG" width="375" height="500">
```

---
## \#4 Posted by: Trdolan03 Posted at: 2017-08-12T04:47:25.250Z Reads: 86

```
I don't have a whole lot of pictures of all the electronics and stuff as this has all happened in about a two week span.
```

---
## \#5 Posted by: psychotiller Posted at: 2017-08-12T04:49:23.893Z Reads: 83

```
I was going to say cold solder joints as well.
```

---
## \#6 Posted by: Trdolan03 Posted at: 2017-08-12T04:49:50.507Z Reads: 84

```
So what would the fix be for that?
```

---
## \#7 Posted by: wafflejock Posted at: 2017-08-12T04:50:33.648Z Reads: 84

```
These all seem like different issues to me really.  The wire gauge is fine for short runs you aren't going to lose that much power in the line with DC voltages it can handle more than with AC as well:

http://www.calculator.net/voltage-drop-calculator.html?material=copper&wiresize=3.277&voltage=50&phase=dc&noofconductor=1&distance=1&distanceunit=feet&amperes=150&x=88&y=24

For the switch to blow too much power has to go through it and it overheats and blows the FETs I imagine (switches dying seem to be common).

For the ESC would need more info about the conditions it blew under but given it's 12S setup maybe too much voltage which exact ESC is it (link)?
```

---
## \#8 Posted by: Trdolan03 Posted at: 2017-08-12T04:52:43.651Z Reads: 70

```
This is the esc I am using. http://alienpowersystem.com/shop/esc/alien-150a-2-12s-evolution-3-car-esc-hv-twin-sensored/
```

---
## \#9 Posted by: wafflejock Posted at: 2017-08-12T04:56:40.395Z Reads: 72

```
So that got replaced for the same thing and the new one worked? did they tell you anything from the exchange by chance or have you test anything out before sending back?

---
Seems like you were all within spec and whatnot.
```

---
## \#10 Posted by: Trdolan03 Posted at: 2017-08-12T04:57:24.164Z Reads: 71

```
@psychotiller  @JLabs
What would you recommend replacing solder joints with?
```

---
## \#11 Posted by: Trdolan03 Posted at: 2017-08-12T04:58:16.363Z Reads: 69

```
No, Bruno was nice enough to repair it all for me. After I got it back, the switch blew.
```

---
## \#12 Posted by: psychotiller Posted at: 2017-08-12T04:58:17.315Z Reads: 62

```
Just go through your system and make sure every soldered spot is solid.
```

---
## \#13 Posted by: Trdolan03 Posted at: 2017-08-12T05:06:39.341Z Reads: 63

```
That is what is confusing me...any ideas?
```

---
## \#14 Posted by: Jacob1 Posted at: 2017-08-12T05:09:07.646Z Reads: 66

```
Hi, im jacob
Im working with thomas on this project, the breaker seems to be the thing that saved us this time even though it blew. Would it be possible that the batteries are sending too much power that it just blew the breaker (breaker is 48volt). And right now switched to an 8s2p configuration.
```

---
## \#15 Posted by: wafflejock Posted at: 2017-08-12T05:12:16.889Z Reads: 61

```
No sorry no idea really I've only blown a VESC and a few wires from shorting things before by accident but was just probing to see if there was more info that might lead to pulling apart each individual problem.

The ESC "decides" based on the receiver input how much power to let through from the batteries the motor coils and the FETs (gates/valves controlling the flow of power to the coils) on there will fry if they are attempting to deliver more power than they are meant for but having more amps available from the battery (power source) side doesn't mean that power gets pushed through, only higher voltage on the battery side can be a problem really.  If you have too high a voltage for a given component then the current through it will be too high and it will not be able to dissipate the heat quickly enough (amperage squared times resistance is power loss as heat).

---

My blown VESC was from probing around while things were live and shorting something with a probe like a dummy, so can't really learn too much from that, it smoked the DRV chip that drives the MOSFETs so I did learn how those things work together to a degree but doesn't help much with diagnosing the APS ESC.
```

---
## \#16 Posted by: Trdolan03 Posted at: 2017-08-12T05:15:14.458Z Reads: 59

```
That is what is confusing me. We were originally told by Bruno that it was because we didn't have the sensor wires hooked up. We skipped that step so we could get them running as both the motor and esc had male ends. It seems that that was not the problem seeing that we have blown the breaker since connecting them.
```

---
## \#17 Posted by: Trdolan03 Posted at: 2017-08-12T05:15:42.131Z Reads: 58

```
And it actually fried the breaker not just tripped  it.
```

---
## \#18 Posted by: Jacob1 Posted at: 2017-08-12T15:08:13.938Z Reads: 36

```
The new one worked but this time we didnt plug it directly imto the batteries. I had a breaker to interupt it. Luckily i had that there otherwise i would most likely have blown the esc again
```

---
## \#19 Posted by: Namasaki Posted at: 2017-08-12T15:24:20.261Z Reads: 32

```
[quote="Jacob1, post:14, topic:30401"]
Would it be possible that the batteries are sending too much power
[/quote]

Batteries don't send power. 
Power is drawn from them by the esc 
You said the breaker is tripping. 
First thing you need to do check all your wiring and make sure you don't have any shorts or crossed wires.
```

---
