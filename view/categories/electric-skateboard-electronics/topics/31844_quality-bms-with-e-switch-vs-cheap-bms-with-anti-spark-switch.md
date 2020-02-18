# Quality BMS with E-switch vs. Cheap BMS with Anti-Spark Switch

### Replies: 10 Views: 2141

## \#1 Posted by: Tomer Posted at: 2017-08-30T10:24:20.530Z Reads: 598

```
For my next build I'm going to ditch the traditional XT90 key and finally move on to an ON/OFF switch.

I can't decide which integration should I use. It's either going with a BesTech Power BMS that includes e-switch, although it's pretty pricey for a BMS. The second option is to go for a cheap BMS from Aliexpress,
using it only for charging, and add to it an anti-spark switch.

I would like to hear your ideas about those two options, what's your favorite one and how come?

For me personally I don't really like the idea of turning ON the system every time I wan't to charge it with BesTech BMS. I also don't like the high prices of it. :cry:
```

---
## \#2 Posted by: darkkevind Posted at: 2017-08-30T10:37:27.646Z Reads: 592

```
How much is the Bestech one?
```

---
## \#3 Posted by: Tomer Posted at: 2017-08-30T10:40:00.626Z Reads: 588

```
There's a MOQ of x2 per order, each BMS costs 40.00$. So it's 80.00$ for two BMS + 24.00$ shipping to me.
I'm going to split the order with someone so I don't care much about the MOQ.
```

---
## \#4 Posted by: darkkevind Posted at: 2017-08-30T10:45:17.316Z Reads: 574

```
OK. Well I got a slightly more expensive BMS for mine, partly because it's 8s but also because the discharge is 60A, it's £35 and doesn't even come with a switch!...

In hindsight I wish I'd have gotten a much cheaper lower discharge one because I'm just bypassing discharge anyway, I let the VESC deal with that... I've got my own anti-spark on/off switch solution in the form of a 120A latching relay hooked up to a momentary rocker switch. The relay was £5, switch £3.
```

---
## \#5 Posted by: MontPierre Posted at: 2017-08-30T14:08:22.397Z Reads: 535

```
I had both options. Now I have Bestech BMS with e switch and I'm vey happy, the vedder antispark took additional space inside of my enclosure which was annoying. The switch itself costed me £25 plus shipping to UK. That's half the cost of Bestech BMS...
```

---
## \#6 Posted by: tueboard Posted at: 2017-08-31T10:35:41.054Z Reads: 491

```
to charge the battery with the bestech bms, do you have to turn on the battery ?

with the bestech bms the anti-spark its not necessary ?
```

---
## \#7 Posted by: Tomer Posted at: 2017-08-31T10:36:57.857Z Reads: 488

```
Yes for both.
```

---
## \#8 Posted by: rusins Posted at: 2018-07-01T16:08:43.817Z Reads: 262

```
Do you still have a loop key or something to disconnect the battery from the VESC while charging, or are you using a quality charger you can trust to not do anything stupid like spark?
```

---
## \#10 Posted by: grrsona Posted at: 2019-04-09T01:48:47.260Z Reads: 87

```
hey there, this is super old, but could you explain the concept of bypassing the bms? Its to not burn it out right? What does that meant for build?
```

---
## \#11 Posted by: darkkevind Posted at: 2019-04-12T17:58:19.620Z Reads: 76

```
Bypassing the BMS, is where your power comes directly from the positive and the negative of the battery, but the BMS is still connected to the cells in order to charge them.
```

---
