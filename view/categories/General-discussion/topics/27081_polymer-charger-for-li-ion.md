# Polymer charger for Li-Ion

### Replies: 5 Views: 497

## \#1 Posted by: TehAtheist Posted at: 2017-07-08T18:48:25.022Z Reads: 61

```
Hi guys, I've encountered a problem. The charger I've bought to charge my Li-ion batteries is only capable of charging Li-Polymer or LiFe batteries. Now the issue is that polymer batteries are charged to 4.2V and Li-ion to 4.1V, so the charging would work just fine but to a to high voltage.

Although I'm an electronics student, I'm not familiar with Li-ion or Lipo's and balance charging, so my question is if I monitor the voltage of the battery, will I be able to charge them without damaging, to 4.1V's? Or will one cell reach 4.2V quicker than other ones?

**The question really comes down to, how much do the cells differ in voltage, during charging? Are they being balanced as soon as they're starting to charge or are they balanced towards the end of the charging?**

Thanks in advance.

Edit with some more information:
Charger: SkyRC E8
    Cell Terminate Voltage : LiPo: 4.2V ± 0.02V / LiFe: 3.6V ± 0.02V
    Circuit Power : 100W
    Current Drain for Balancing : 200mA
https://www.mcmracing.com/nl/home/85462-skyrc-sky100096-disc-e8-ac-charger-lipo-life-2-8s-up-to-6a-100w-SK-100096-03
Battery: Turnigy 5000mAh 4S x 2 (in series for 8S, will be charged in 8S)
https://hobbyking.com/en_us/turnigy-5000mah-4s-25c-lipo-pack.html?___store=en_us

Edit3: Alright, turns out I was completely oblivious to the fact that my charger is compatible with my batteries... Which makes sense as I double checked everything when I bought it. I do not know where I got the idea that my battery is Li-ion afterwards, sorry ;) and thanks for the fast replies!
```

---
## \#2 Posted by: smurf Posted at: 2017-07-08T18:53:21.866Z Reads: 55

```
How about a little more details. What model charger do you have and what kind of battery pack are you going to use?
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-07-08T18:59:00.670Z Reads: 53

```
From what I've heard balance chargers do the balancing at the very end of the charge cycle. Also I've heard that charging liions past 4.1 can be quite bad for them.
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-08T19:00:26.286Z Reads: 51

```
Typical Lipos and cylinder cell li-ions charge to 4.2v. You can check the datasheet for any li-ion cell, and it should say 4.2v is the max  charging voltage, not sure where you saw 4.1v. However, if you do charge to 4.1v it'll double the cycle life of the cell.
```

---
## \#5 Posted by: TehAtheist Posted at: 2017-07-08T19:33:18.999Z Reads: 44

```
I'm confused now, I've updated the topic with info about my batteries and charger.
But I looked to the voltage and it says 14.8V, but that's 3.7V for each cell?
I know the fact that you need a higher voltage than the cell to charge it, but is it really that high?

Well fuck me, I've got a lipo pack?! Jesus Christ, how couldn't I have noticed!
```

---
