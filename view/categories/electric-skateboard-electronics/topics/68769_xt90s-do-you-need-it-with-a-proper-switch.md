# XT90S - do you need it with a proper switch?

### Replies: 9 Views: 346

## \#1 Posted by: MrDGOrman Posted at: 2018-09-21T16:30:37.422Z Reads: 139

```
Hi everyone,

This is going to be a noob question for sure, but I want to double check.

I'm making the transition from a LiPo battery setup where my XT90S is a "switch" to a Li-Ion battery which I plan to have an inline on/off button like boards such as Boosted and Evolve.

They don't use an XT90S, so I'm guessing you don't need to include this. Is that right?

Can someone give me a nice and detailed wiring diagram, if they've got it, suitable for a single motor setup? The only things I want visible on the outside of the enclosure is the on button, the battery level (%) and the charging port.

Cheers,
Daniel
```

---
## \#2 Posted by: L3chef Posted at: 2018-09-21T17:25:30.064Z Reads: 126

```
You don't need to include a xt90. But it's always good to have the battery fysical disconnected when not in use.
What you are looking for is either a anti spark with a on/off button or a bms.with a e-switch
```

---
## \#3 Posted by: dareno Posted at: 2018-09-21T22:35:13.520Z Reads: 92

```
The only way to physically disconnect your battery when not in use is to incorporate a loop key into your design.  @mmaner does some lovely little panel mount xt90 surrounds and I think some nice battery indicator mounts too.   
Kind of a piece of mind thing though and a lot of guys don't bother if they run either e switch from the bms or a vedder style antispark unit.
```

---
## \#4 Posted by: MrDGOrman Posted at: 2018-09-23T15:57:47.058Z Reads: 66

```
I think I'm going to go with the e-switch option. It's just a pain having to plug in an additional item when in my opinion a simple on off button is all that's needed.

I'm going to order the eskating bestech BMS. Looks like I can use it with my LiPos and then with the Li-ion when I alter the setup completely. Not sure how that works because the cut off for minimal discharge is different for LiPos Vs Li-ion, right?
```

---
## \#5 Posted by: L3chef Posted at: 2018-09-23T16:18:07.172Z Reads: 58

```
If you use a vesc you can setup soft and hard votlage cut off.
```

---
## \#6 Posted by: MrDGOrman Posted at: 2018-09-23T19:08:01.086Z Reads: 45

```
I have a FOCBOX which has a battery minimum setting but my concern is when the battery is being charged. Unless I'm being stupid and the max cell voltage is the same for LiPos and Li-ion?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-09-23T19:34:52.843Z Reads: 41

```
It’s the same. 4.2v max for lipos and LiIon cells
```

---
## \#8 Posted by: MrDGOrman Posted at: 2018-09-23T19:40:18.064Z Reads: 43

```
Oh right okay!

Do you maybe know the answer to a question I posted in another thread? I want to get a BMS that will work with my LiPos and then with the Li-ion batteries when I get them. I also want one with an e-switch as that seems to be the best option.

https://www.electric-skateboard.builders/t/bms-question-noob-alert/68993

Thanks
```

---
## \#9 Posted by: Andy87 Posted at: 2018-09-23T19:47:37.182Z Reads: 37

```
As long as it’s not a smart bms you usually fixed on the cells count the bms is made for.
So if you buy a 10s bms it will not work for a 3s battery. (Ok, there could be a ways to bridge the input wires or so to simulate a 10s, but that’s probably not what you want to do)
```

---
