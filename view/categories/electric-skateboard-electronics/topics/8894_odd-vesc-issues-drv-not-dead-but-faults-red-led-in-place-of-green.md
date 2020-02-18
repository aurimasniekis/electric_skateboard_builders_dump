# Odd Vesc Issues (Drv not dead but faults, red LED in place of green)

### Replies: 1 Views: 442

## \#1 Posted by: bigpianist Posted at: 2016-09-04T14:03:27.524Z Reads: 64

```
I recently got a couple of enertion Vescs, tried setting one up in FOC and after spinup got DRV 8302 error. Thought for sure I blew the chip, bit confused why because I followed all the steps in the many tutorials out there, however I think I narrowed it down to the firmware bug, which really sucks. But heres where it gets weird, because I can run the Vesc on 3s (normal setup is 6s) only occasionally getting the DRV error code, but on 6s it mever spins the motor anymore. I hvae tried almost everything, from flashing the firmware to changing various values for voltage amperage etc. 

The other Vesc I have is even weirder, because the first time I powered up I immediately noticed something strange, as there is a red LED in place of the green one and the blue one is normal. So instead of having a green, red and blue LED like normal, it has 2 red and one blue. No DRV faults on this one, configured it in BLDC mode and the motor spins up fine. However, I cannot control this Vesc from anything other than the Keyboard. It doesnt give power to the receiver, whereas my other one does. Tried controlling it over canbus with my friends Vesc, still didn't work. Bit stumped here.    

I finally tested my friend's Vesc to make sure I wasn't going crazy, and his worked fine! We ordered around the same time (mid August) so it's a pretty odd situation. Little bit frustrated but things happen. Want to get back riding ASAP


Motor is Turnigy SK3 5045-450 2x
Batteries are Turnigy 5000mah 3s 2x (Series)

Thanks for any help :)
```

---
