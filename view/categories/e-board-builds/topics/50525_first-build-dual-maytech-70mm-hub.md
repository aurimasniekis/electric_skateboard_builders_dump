# First build - dual maytech 70mm hub

### Replies: 7 Views: 529

## \#1 Posted by: Harley164 Posted at: 2018-03-29T03:26:09.990Z Reads: 102

```
Hi All,

About to embark on my first build.   The idea is to build a putting around board that I can carry on to an airplane.  I'm also trying not to break the bank and from what i understand the maytech stuff isn't that bad as long as you get your settings right and don't do anything stupid.

Thinking of a kicktail board similar to this one - want to keep length <33"
https://www.ebay.com/itm/Natural-Pool-deck-9-25-x-31-75-7ply-Canadian-skateboard-blank-9-25-X-31-75-C9-/172466114028

For the guts i'm going to go with dual maytech 70mm hubs - I think the 90's will be too big for the shorter board.

Going to use two Maytech VESC's v3.3 and attempt to operate in FOC/Hybrid mode.

I also plan on using a charge only BMS with a 10s setup.  All wiring/connectors will be 90XT/10 AWG except for the motor wires - 12 AWG

for the batteries I plan on using two Turnigy 5s 5000mah batts for a 10s setup.  I see a lot of boards with 4 or more Turnigy's on the bottom, but I think for shorter ranges i can get away with just 2.

Not sure on enclosures - for the time being i'm going to go with some sandwich boxes temporarily, then go with something more permanent.

about to pull the trigger on all the parts.
```

---
## \#2 Posted by: Namasaki Posted at: 2018-03-29T21:37:23.204Z Reads: 62

```
[quote="Harley164, post:1, topic:50525"]
Turnigy 5s 5000mah batts for a 10s setup.
[/quote]


If you go with Lipo packs, it is advisable to get packs with a high C rating Like 50C or higher.
I run Lipos in a 10s configuration with five 2s 5000mah 60C packs. It works pretty well with minimum voltage sag but I wouldn't mind having packs that are 90C-100C for even better range and performance.
When building a board to take aboard airplanes, You must keep the capacity to a minimum.
I'm not sure what the limit is currently. 
But with minimum capacity, it helps to have the highest C rating possible.
```

---
## \#3 Posted by: Harley164 Posted at: 2018-03-29T21:49:50.795Z Reads: 55

```
Thanks - i was looking to just use 2 of them.

Will look for two of them with a 50C rating or higher.

thanks man,
dave
```

---
## \#4 Posted by: Harley164 Posted at: 2018-03-29T21:52:10.202Z Reads: 55

```
Not many options with high C ratings

https://hobbyking.com/en_us/turnigy-graphene-5000mah-5s1p-65c.html
```

---
## \#5 Posted by: pat.speed Posted at: 2018-03-29T21:53:16.075Z Reads: 48

```
I would advise against a maytech vesc, ecspecially in foc mode.

The limit for sir travel is 99wh
```

---
## \#6 Posted by: Namasaki Posted at: 2018-03-29T22:04:59.239Z Reads: 46

```
I haven't personally tried the Graphene's but have heard they are good.

The nice thing about Lipos is you can get high current output in a compact low watt-hour battery.
It's gonna hard to stay within a 99wh limit though

A 10s 5ah is gonna put you way over at 185wh

You'll have to go with 2500mah at 10s
```

---
## \#7 Posted by: Harley164 Posted at: 2018-03-29T22:11:37.746Z Reads: 47

```
I plan on making the batteries easily removable.  

As long as you can show they are separate it will be fine - at least in my experience.  I travel with lots of lithium since I'm in television.

I've heard lots of mixed reviews on the Maytech Vesc's . . .. the latest is that since they're at v3.3, they work great.  worse case i'll run it BLDC.

thanks for the advice.

it might be worth it to go with a lower mah just for a smaller profile on the battery
```

---
