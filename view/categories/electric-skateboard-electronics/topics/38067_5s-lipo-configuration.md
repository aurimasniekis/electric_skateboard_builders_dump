# 5s lipo configuration

### Replies: 2 Views: 349

## \#1 Posted by: Boardnamics Posted at: 2017-11-12T05:46:46.521Z Reads: 52

```
I currently have two 5000mah 5s lipos from hobbyking and was wondering if its worth getting two more. 200wh is decent but I am wanting more. One of the 5s lipos is significantly older than the other one and it's showing. It drains faster than the other. Weird cause u would think it has a higher IR and thus naturally gets drawn from less.

Anyways, how would I go about setting these up without a bms? And by that I mean charging them. Making a harness is easy. What sort of chargers are recommended for this sort of thing? Is it better to charge them as one huge parallel pack or series?
P.S. this could probably be done with a BMS.
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-12T05:57:14.200Z Reads: 50

```
I'm assuming they're in series right now to make a 10s1p pack. If that's the case, each cell in series will have the exact same current drawn from it regardless of internal resistance. You only have uneven sharing caused by IR differences with cells in parallel. 

A BMS will go a long way to solving cell mismatch, as well as preventing you from damaging cells by discharging them too far.

It's still not recommended to mix old and new batteries, especially ones that have already been deeply discharged and/or pushed hard.

A 10s balance charger isn't out of the question, but they're rarer and more expensive than the usual 6s ones, If it were up to me, I'd spend the extra money on a BMS and a 10s non-balance charger, rather than a 10s balancer.
```

---
