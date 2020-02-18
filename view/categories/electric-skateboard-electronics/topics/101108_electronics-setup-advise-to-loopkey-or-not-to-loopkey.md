# Electronics setup advise? To loopkey or not to loopkey

### Replies: 8 Views: 191

## \#1 Posted by: Ultimiant Posted at: 2019-08-30T16:10:20.473Z Reads: 74

```
Alright so I've posted this build before, but I now have my battery that has a charge only BMS with the discharge bypassed. I've been reading up on how to deal with the electronics and I'm a bit confused regarding the function of a loopkey.

I've seen posts about using a loopkey along with a power switch, as well as a loop key as a replacement for a power switch. Is a loopkey's only functional to prevent sparking or does it only serve its function if its removed?

Ideally I'd like to use a power switch for aesthetics but I am unsure if the [**Flipsky pro switch**](https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-plus-based-on-vesc6) would work with a loopkey, and if it did, could I just keep the loopkey within my enclosure and use the power switch to toggle power? My confusion comes from the fact that the pro switch plugs straight into the VESC. What should be my plan of action regarding finishing my setup? Or would my best bet be getting just a regular anti spark power switch like [**this one**](https://flipsky.net/collections/accessories/products/antispark-switch-pro-280a).

My build as it stand is this:
![esk8_setup|690x395](upload://3WoJuN4lziRzRNajtM8ONp10AuU.jpeg) 

Any guidance would be appreciated, trying my best to get riding before winter hits haha.
```

---
## \#2 Posted by: Grozniy Posted at: 2019-08-30T16:22:01.333Z Reads: 62

```
You connect the loop key on negative lead from the battery. XT90S or as150. I prefer as150. Both serve to prevent the big spark, that's all. All anti spark switches will fail and can destroy your board. So XT90S or as150 is the way to go.
```

---
## \#3 Posted by: Ultimiant Posted at: 2019-08-30T16:53:13.091Z Reads: 58

```
So I can use an as150 or an XT90s loopkey and leave that connection in my enclosure, to prevent the spark, and then use the pro switch in the vesc to power on/off?
```

---
## \#4 Posted by: thisguyhere Posted at: 2019-08-30T17:08:39.343Z Reads: 57

```
switches fail.  almost always.  even the ones that come onboard the esc.

consider the loopkey as a master switch.  like a breaker in your house.

so...if the switch on the esc is working, no need to mess with the loopkey.  but if the esc switch fails, you have the loopkey to cut the circuit.

hope that made sense.

so your diagram would look like this

![image|690x395](upload://x6Vf8I58goaJPGhrpB8o9yHsWUN.jpeg)
```

---
## \#5 Posted by: Ultimiant Posted at: 2019-08-30T17:27:40.777Z Reads: 51

```
So just leaving the loopkey as part of the circuit will prevent any sparking, and would function as a sort of *deadman switch*?
```

---
## \#6 Posted by: Grozniy Posted at: 2019-08-30T18:02:39.260Z Reads: 47

```
It will work as on/off switch
```

---
## \#7 Posted by: Skunk Posted at: 2019-08-30T19:40:25.890Z Reads: 42

```
[quote="Ultimiant, post:5, topic:101108"]
So just leaving the loopkey as part of the circuit will prevent any sparking,
[/quote]

No. 
It only prevents spark when its used as your on / off switch. 
Just being in line on your harness won't prevent your on of switch on the esc from failure.
```

---
## \#8 Posted by: Flasher Posted at: 2019-08-30T22:54:23.330Z Reads: 27

```
As @Skunk says, It only prevents sparks when plugged. As compared to using a regular xt90 in the exact same place.
```

---
