# Lots of Battery Questions

### Replies: 3 Views: 504

## \#1 Posted by: paullj Posted at: 2017-03-09T13:06:53.849Z Reads: 99

```
Hi I am thinking of building an Electric Longboard and have lots of questions regarding batteries.

I know LiPoly batteries are very common but having used some for a DIY drone I'm not confident with them. So, what are the main advantages and disadvantages of the different battery types?

For symplicity sake I would like to just connect the board to mains to charge it, is this possible? or would I have to use a balance charger? I've heard of BMSs but what do they actually do? are they like on board balance chargers?

On to battery specific, is it beneficial to get 2 or more batteries in series? and if so how would you charge them? I assume you would have a 3 way switch with on/off/charge. Where charge would put them in parallel?

Sorry for all the questions, I am in the process of resding loads of content on here to learn. Thank you very much.
```

---
## \#2 Posted by: rpn314 Posted at: 2017-03-11T02:20:08.185Z Reads: 67

```
I will assume you're just asking about other lithium based batteries and not something like nickel or lead based batteries.

By my counts LiPo (Lithium-Polymer) and Li-Ion (Lithium-Ion) are by far the most popular, with LiFePO4 (Lithium-Iron Phosphate) coming in 3rd. Each has some advantages and disadvantages. Here's some _generalizations._

- Current per cell (higher is better): LiPo > Li-Ion > LiFePO4
- Stability (Higher = less likely to explode): LiFePO4 > Li-Ion > LiPo
- Longevity: LiFePO4 > Li-Ion > LiPo
- Cost per Wh (My best guesses, but feel free to correct): LiPo < Li-Ion < LiFePO4

And though it's not necessarily better either way, this is good information to know

- Nominal Voltage (no benefit higher or lower): Li-Ion > LiPo > LiFePO4

If you're looking to have a "one plug" charging solution (just a brick with a barrel plug, like on a laptop) then you'd need a BMS onboard. The BMS (usually stands for Battery Management System) does what it sounds like: it manages the batteries individually to make sure they don't go too far over or under their voltage ratings. So yeah, they're sort of like onboard balance chargers. I'd say hit up youtube for a better (more precise and in depth) explanation than that.

More batteries in series means a higher voltage (series adds the voltage) Charging them in series means you'd need a different charger (higher voltage) and BMS (if you're considering one). More batteries in series means same voltage, but you can pull more current (ie. parallel adds current).

Most of us just have an on-off switch (and some BMS's have them built in, just so you know), but it depends on how the wiring is set up.
```

---
## \#3 Posted by: paullj Posted at: 2017-03-11T22:08:37.756Z Reads: 34

```
Thank you very much for the detailed reply, this is really useful. I'm sure it will be very useful for me but also for others on here :smiley:
```

---
