# Discharge 2x 6S liPo packs in parallel, charge them individually

### Replies: 10 Views: 494

## \#1 Posted by: TipsyTrex Posted at: 2018-03-06T13:25:24.513Z Reads: 102

```
Hello,

I have not found anything like this, so here is my problem.
I have 2 6S 3700mAh zippy lipo packs. I want to discharge them in parallel. For the charging i want a simple solution to charge them individually. I don't want to parallel charge the packs as it is not really recommended. (BMS is not a option, as i don't have the space)
So now i either have to open up the enclosure and get them out of it, or i try something like [this](https://imgur.com/a/vHMXZ).
The idea is that i can control wich pack i'm charging with the switches. It wont arc because there is no power running when the loop key is removed. I know that i need big siwtches but thats okay. i got some.

Anyone got any idea's? I still have to make my enclosure. I want to keep it stealthy so no food storage container for me ;)
If i make an enclosure that is easy to open, the problem is solved as well. Still have not found anything useful.
I do have access to a 3d printer (ultimaker 2 and 3) so if anyone has a enclosure that i cant print and is easy to open, please let me know.

If it is save to parallel charge, why and how does it work exactly? i'm really skeptic about it because the charger has to balance 2 packs at the same time.

Thanks in advance :smiley:

-TT


UPDATE:

I found some motivation and dedicated my entire day to designing an enclosure that is printable on most printers.
Here are some screen caps as a proof of concept. [Screencaps](https://imgur.com/a/rlm80)

If this is fully designed and tested i will upload the files and make a new thread in the mechanical sub.

For the mounting of the 2 shell parts i will just use glue or epoxy. For the baseplate i will mount an aluminium plate to the bottom. This prevents the plastic getting damaged by the little rocks that smash against it while riding. I'm not sure how i will mount it, but i will come up with something.

The baseplate is removable from the shell using M5 Thumbscrews on 6 location along the structure. inside the shell are hexagon holes big enough to press fit a m5 Lock Nut in. this will ensure that the thumbscrews won't come lose while riding.
i left the front flat so if anyone that wants to add a screen is able to do so.

rough dimensions : Height 55mm , length 370, width 170. Everything is at least 5mm thick to ensure stiffness,

let me know what you think or how this may be improved!
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-03-06T13:39:16.510Z Reads: 91

```
In theory this would work out, but i would be skeptical about the switches. They need to be really beefy and well isolated.

Also i'd prefer taking lipos out of the enclosure to visually inspect them once in a while. I never had Lipo go puffy while being properly use, but still...

Parallel charging isn't so bad really. I'm charging my 6S12Ah Graphene packs in parallel while discharging them in series.

The moment you hook the batteries up in parallel they start to equalize their voltage. This isn't inherently bad as long as their original voltage difference is less than 0.1V. 
So if you connect both main and balancer plug in parallel they will essentially both be on the same voltage level all the time and can be charged as one big battery. The same thing also happens when discharging, as long as they are connected the voltage of the packs will be the same.

As always with lithium, if you take care and check the voltages each time before plugging them in in parallel everything will be good.
```

---
## \#3 Posted by: TipsyTrex Posted at: 2018-03-06T13:49:11.181Z Reads: 76

```
So it would be like [this](https://imgur.com/a/LTb54) when it comes to parallel charging?
Sounds good then. I will look more into it i guess. 
What kind of enclosure do you have? you said that you take them out once in a while. If i get an easy to open enclosure i can inspect and charge the packs individually.

Thanks for the fast reply! :smiley:
```

---
## \#4 Posted by: Acido Posted at: 2018-03-06T14:15:43.768Z Reads: 69

```
You can buy a charge only bms, take the cables for balancing and put them on the enclosure, then connect your charger to bms that's outside of the skate, in some kind of a printed enclosure and get another cable that fits the balance wires to the bms
Not the simplest way but much better than taking out the batteries and charging
```

---
## \#5 Posted by: Der6FingerJo Posted at: 2018-03-06T18:33:09.907Z Reads: 54

```
Yes that looks like it would work. Since it's all in parallel all the time it's basically one battery. 

Sorry to disappoint you, I just used a planter tray with 4 screws through the deck. So not that time consuming but also not that easy to open up.
```

---
## \#6 Posted by: FabianOdermatt Posted at: 2018-03-06T19:03:13.058Z Reads: 48

```
I have 2 5S 5000mAh Lipos and I charge them in parallel. No issues.
```

---
## \#7 Posted by: TipsyTrex Posted at: 2018-03-07T07:54:42.261Z Reads: 43

```
Thanks for helping me out. I'm into the process of designing a easy to open enclosure wich easy to print. (It's harder then it sounds...)
If that doesn't work out i will just settle with parallel charging the packs. If i succeed in designing one i will post the files somewhere on here. if someone is interested i can tag you in it. (not saying it will succeed though)

It will be designed to hold the vesc, receiver and 2 removable 6s packs with some spare space for cables etc. I want to make it in a way that it is easy to print, easy to remove the packs and at last make the vesc and receiver reachable without to much effort.
```

---
## \#8 Posted by: Der6FingerJo Posted at: 2018-03-07T08:05:08.773Z Reads: 44

```
I know what you are talking about. I also played around with printing enclosures but never put enough design into it to actually test it. The hard part is to find a material that will hold up and is easy enough to print in large.
```

---
## \#9 Posted by: gbutcher Posted at: 2018-03-07T08:38:19.154Z Reads: 39

```
I have been charging LiPo's in parallel for years with no issues.  As mentioned above, so long as they are close in voltage then it is safe and reliable.  It would keep your setup simple.

If you want to do some extra reading check out these links -

https://oscarliang.com/parallel-charging-multiple-lipo/

https://www.rchelicopterfun.com/parallel-lipo-charging.html
```

---
## \#11 Posted by: TipsyTrex Posted at: 2018-03-07T10:10:03.876Z Reads: 34

```
Thanks for the info! will read trough it as soon as i can.
```

---
