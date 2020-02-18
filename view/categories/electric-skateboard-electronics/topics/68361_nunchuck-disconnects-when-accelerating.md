# Nunchuck disconnects when accelerating

### Replies: 2 Views: 153

## \#1 Posted by: sch_ch1 Posted at: 2018-09-17T23:16:22.502Z Reads: 35

```
hello there! :)

this summer I upgraded my battery from 6S to 10S and since then I got disconnects when accelerating, using my nyko kama.

when I move the stick slightly, everything works fine. when I push the stick more than like half way at once it comes to a disconnect (no matter how fast I already ride), I see my nunchuck blinking and the board just continues accelerating due to timeout setting set to 1000ms.


I tried different settings of timeout, to make this incident seem a little less scary while riding, but there must be some kind of interference with the wiiceiver and the amps that get to the motor.


I recently used my nunchuck with an arduino + wiiceiver, but as the arduino broke, I just connected the nyko receiver directly to the vesc, that changed nothing. 
Then I tried with 2.4ghz ppm, worked just fine, no disconnects. :thinking:

Tried to put the receiver in different positions and places in my enclosure, even out of it, but nothing changed. 
I hope that the problem may be to solve by using the vesc tool and lower some parameters, but I’m not quite sure what to change honestly.

hoping for your help, thanks!
```

---
## \#2 Posted by: sch_ch1 Posted at: 2018-09-18T12:59:19.808Z Reads: 20

```
I made a few screens from the vesc’s realtime data, maybe helpful to fix the problem.

first 3 screens are with the nunchuck from 0 to half/full throttle, for so long till the nunchuck reconnects and I was able to stop. 
The last one is in ppm mode with a 2.4ghz remote where it seems to work just fine. (I went to full throttle, then released to see if the vesc stops accelerating, then went full throttle again - thats why there are 2 peaking curves in that screen)

![vesc%20throttle|690x387](upload://kheuPMbUzinLrLmP6P4J23AUMWQ.jpeg) 
![vesc%20throttle1|690x387](upload://kHY6MZ6ZtSGvYhwrYCyheukMDEb.jpeg) 
![vesc%20throttle2|690x387](upload://jcOdpJ6JDpDoRIqPDgGBUfYRvBp.jpeg) 
![vesc%20ppm|690x387](upload://qjHCXVy7jPIrJBitNUME5CxTP4U.jpeg)
```

---
