# Battery charger 10s, &ldquo;36v output 42v?&rdquo;

### Replies: 7 Views: 2990

## \#1 Posted by: Hannes Posted at: 2018-06-25T18:08:38.127Z Reads: 177

```
Hi, i'm about to buy a charger for a 10s4p (30q) li-ion battery pack but i'm a little bit confused,

I'm looking at 42v 2a chargers but when i do a [ebay search](https://www.ebay.com/sch/i.html?_from=R40&_nkw=42v+2a+li-ion+battery+charger&_sacat=0&LH_PrefLoc=5) i'll get these kind of results "36v 2a Battery Charger Output 42v 2a Charger Input 100-240 Vac Lithium Li-ion Li".

Whats with the 36v vs output 42v?

Also, if i choose a higher amperage 2-4 does that affect anything else other than just charging faster?
```

---
## \#2 Posted by: wafflejock Posted at: 2018-06-25T18:15:07.666Z Reads: 166

```
You'd need to plug that charger into some kind of balance circuitry for it to balance all the cells or parallel groups individually.  The 36V vs 42V is just the 'nominal voltage' vs the fully charged voltage.  Most cells are 'nominal' voltage of 3.6 or 3.7V per cell so 10 in series is 36V (or 37V depending on the specifics of the cell might be +/- a volt or two from here), this is where they are at 50% basically or what voltage you can expect out of them for most of the discharge.

Regarding amperage it is the limit on how quickly you can charge this is also typically capped by the 1C (or 1 times the Ah rating on the battery for charge rate, say you have 2.5Ah battery you should only charge at 2.5A at most, if you put two in parallel you can double the rate since it gets split between the parallel packs.

---

Most people using lipos I think use the imax b6, I've used a few chargers from keenstone that I like (they have a 500W one but only has DC input so need to have some kind of AC->DC transformer still before the charger).  For li-ion I think the tendency is to go with a BMS (bestech is a good brand from what I hear) but you can search for 10S balance chargers as well.  Advantage with balance charger vs BMS is less crap on the board to potentially fail, advantage of BMS is easier to charge once you've set everything up.
```

---
## \#3 Posted by: Benjamin899 Posted at: 2018-06-25T18:17:24.007Z Reads: 149

```
you know the seller even put that info into the description, just scroll down mate
```

---
## \#4 Posted by: Hannes Posted at: 2018-06-25T18:17:38.073Z Reads: 141

```
okey then i get it, thanks for the explanation :slight_smile:
```

---
## \#5 Posted by: Hannes Posted at: 2018-06-25T18:19:09.354Z Reads: 136

```
Yes, I see your point, my lazy side showing. "42V actual output. Please note: it is often confused between 36V battery and 42V charger output. It means that when a battery is fully charged, its voltage is 42V. The charger would only start to charge your battery when the battery power has been used up below 36V."

Thanks for the heads up :)
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-06-25T18:40:11.944Z Reads: 121

```
np happens to everyone
```

---
## \#7 Posted by: karma Posted at: 2018-06-25T20:55:17.811Z Reads: 109

```
Extra note, a 36V charger can also be LiFePO4 charger since those cells have a nominal voltage of 3.2-3.3V and max of 3.6V. Which means a 10S LiFePO4 is max 36V. Such a charger is not conpatible with lithium ion. Just make sure the title says Li-Ion and not LiFePO4 and you will not make that misstake.
```

---
