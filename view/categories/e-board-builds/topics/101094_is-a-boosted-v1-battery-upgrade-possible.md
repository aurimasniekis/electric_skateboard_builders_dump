# Is a Boosted V1 battery upgrade possible

### Replies: 14 Views: 230

## \#1 Posted by: Dog Posted at: 2019-08-30T12:26:20.675Z Reads: 73

```
So I bought a few cheap v1 project boards with dead batteries and was wondering, do I have to use the boosted board battery pack and their respective bms in order to use their vesc or I can install a completely different battery pack without the original boosted bms, as long as the voltage is as it should be? Does the vesc communicate with that specific bms or it doesn’t care?

Also on a side note, is it possible to solder connectors to the boosted board v1 battery wires to make it detachable, removable and swappable?
```

---
## \#2 Posted by: Superflim Posted at: 2019-08-30T13:34:37.496Z Reads: 65

```
Yeah you need the boosted battery Bms in order for it to work with the esc. You'd be better off getting a new Vesc.
```

---
## \#3 Posted by: Andy87 Posted at: 2019-08-30T17:48:16.129Z Reads: 59

```
Boosted dont use vescs 😉 
But yes the bms communicates with the esc, so you can’t just swap the original pack to a diy pack. What you could do is an extended pack which you add in parallel to the original battery pack. 
Search a bit here. You should be able to find some information about it. It was done before by others
```

---
## \#4 Posted by: Dog Posted at: 2019-09-01T04:26:07.797Z Reads: 46

```
Does the parallel pack have to be of a certain capacity or it could be substantially bigger in capacity than the v1, even if it’s the same voltage? I’m thinking about building bigger parallel packs than the ones that were build here. 

Also, could I upgrade the v1 pack with more cells or the bms is configured for that certain amount of cells?

Also, could the v1 battery pack be made detachable by soldering connectors to wires for easy install/uninstall?

Lastly, could the motors be replaced/upgraded to more powerful ones but still use the or b1 esc and bms?

Thanks for the answers.
```

---
## \#5 Posted by: Andy87 Posted at: 2019-09-01T09:06:12.258Z Reads: 39

```
[quote="Dog, post:4, topic:101094"]
Does the parallel pack have to be of a certain capacity or it could be substantially bigger in capacity than the v1
[/quote]

Capacity doesn’t matter, just make sure the voltage match up and don’t forget the bms from the original pack will not balance the additional pack

[quote="Dog, post:4, topic:101094"]
upgrade the v1 pack with more cells or the bms is configured for that certain amount of cells?
[/quote]
A bms just balance the parallel groups which attached to the balance leads. If you add a complete pack in parallel than the bms will not balance that pack


[quote="Dog, post:4, topic:101094"]
could the v1 battery pack be made detachable by soldering connectors to wires for easy install/uninstall?
[/quote]

I would make the self made pack attachable with separate charge port and charge only bms.


[quote="Dog, post:4, topic:101094"]
Lastly, could the motors be replaced/upgraded to more powerful ones but still use the or b1 esc
[/quote]
Don’t think so.


All in all i would just use the deck and trucks, wheels etc and switch the whole electronics to diy components. Get two vesc or a dual vesc and you can run what ever you want.
```

---
## \#6 Posted by: Dog Posted at: 2019-09-01T09:11:35.475Z Reads: 32

```
M[quote="Andy87, post:5, topic:101094"]
> could the v1 battery pack be made detachable by soldering connectors to wires for easy install/uninstall?

I would make the self made pack attachable with separate charge port and charge only bms.

![|20x20](https://www.electric-skateboard.builders/letter_avatar_proxy/v4/letter/d/13edae/40.png) Dog:
[/quote]

Thank you for the opinion on what you would do, but I want to have the option to remove the main pack too.

Can it be done, even considering that you won’t do it for your own boosted board?
```

---
## \#7 Posted by: Dog Posted at: 2019-09-01T09:13:04.833Z Reads: 29

```
Ты по русски лучше пишешь, да? Непонятно иногда.
```

---
## \#8 Posted by: Dog Posted at: 2019-09-01T09:21:28.753Z Reads: 29

```
So from what you’re saying, the boosted v1 bms is made only for that 12s1p and it’s impossible to connect a 12s2p pack to that bms?
```

---
## \#9 Posted by: Sn4pz Posted at: 2019-09-01T11:09:09.315Z Reads: 28

```
Hi Dog, I'm in a sort of similar predicament regarding v1 boosteds and getting it back up and running. 

I'm getting rid of the of pack that was in there and replacing it with a 10s3p of Samsung 30ts, replacing the speed controller with a focbox Unity and including a Metr module and Flipsky VX1, keeping the drive train and just upgrading to fresh wheel pulleys and 85mm purple cags. 

To extend the packs to a 12s2p(or more)  you would have to first remove the bad / dead cells in the first p pack, then add only the exact same cell in the same configuration for your second, third or even fourth p group. The BMS only works with that wonky voltage, so using the same A123 cells boosted does is unfortunately required

Imo, you would be better off just ditching the internals and instead, buy a new liion battery and spend time programming a smooth throttle curve. 

It's what I'm going to do at least 🤷
```

---
## \#10 Posted by: Andy87 Posted at: 2019-09-01T12:06:13.788Z Reads: 27

```
I have a boosted v2 and there you can remove the main pack buy just disconnect one plug, but the esc will not work without signal from the original pack.

мой русский не достаточно хорош, чтобы объяснить
```

---
## \#11 Posted by: Dog Posted at: 2019-09-01T18:22:30.944Z Reads: 19

```
So I’m other words, I can use the same bb v1 bms to extend the og pack from 12s1p to 12s2p or 3p but only if I use the same cells?
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-09-01T18:25:21.298Z Reads: 21

```
Yes. A bms doesn't care about parallel packs unless it's wired for discharge, which means there is a limit to what the BMS can push towards the ESC and motors. 

If the BMS is skipped / bypassed for discharge then you're golden. 

It's easy to switch a normal bms from charge and discharge to bypass, I don't know about the boosted bms... Only one way to find out ;)
```

---
## \#13 Posted by: Dog Posted at: 2019-09-02T23:35:05.022Z Reads: 13

```
Can I solder connectors to the positive and negative wires and a 2pin connector to the gray wire on the BOOSTED BOARD VERSION ONE BATTERY PACK and make it detachable/unplugable/removable without the need to cut the wires?
```

---
## \#14 Posted by: Andy87 Posted at: 2019-09-03T05:36:28.556Z Reads: 13

```
I don´t have a boosted V1, so I unfortunately can´t say how it should be.
```

---
