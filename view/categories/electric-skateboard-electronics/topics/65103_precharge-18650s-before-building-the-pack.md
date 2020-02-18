# Precharge 18650s before building the pack?

### Replies: 10 Views: 270

## \#1 Posted by: Itsmedant Posted at: 2018-08-16T19:07:37.538Z Reads: 132

```
So I've looked through multiple battery build threads as well as read through the entire N.E.S.E. thread (which is what I'm using) but I still can't seem to find the answer to my question.

Do you guys precharge your 18650s before putting them together in your configurations (12s4p for me) or do you put your pack together, and then charge it with the BMS?

I'm going to be putting all of my cells together over the weekend and want to make sure I'm doing it right!
```

---
## \#2 Posted by: Battosaii Posted at: 2018-08-16T19:28:06.397Z Reads: 128

```
I don't thing the amount of charge matters but what matters is that every cell is the same voltage. If they are different then the battery will be unbalanced and it's hard to balance ancomplete battery like that.
```

---
## \#3 Posted by: DougM Posted at: 2018-08-16T19:39:45.190Z Reads: 122

```
If you're buying them just build the pack with the charge they had when shipped.  If you are using disparate sources than @Battosaii is correct.  I'd actually discharge them all to minimum and then build the pack.
```

---
## \#4 Posted by: wafflejock Posted at: 2018-08-16T19:41:22.640Z Reads: 111

```
Cells put in parallel with one another will 'self balance' that is the higher voltage battery will discharge into the lower voltage one so this is key to pay attention to.  Basically all cells that you put into a given P group need to have roughly the same voltage or you will end up with a high current discharge from the higher voltage one to the lower one which would be bad for both but worse for the one quickly charging.
```

---
## \#5 Posted by: Itsmedant Posted at: 2018-08-16T20:16:05.058Z Reads: 92

```
Makes sense now!! Thanks everyone! Wish me luck in my pack building!!!

Also, My wife has a boosted board, I noticed that their charger is rated for 54.4v....can I use this to charge my board since I'm doing 12s?
```

---
## \#6 Posted by: pat.speed Posted at: 2018-08-16T21:31:10.242Z Reads: 79

```
Nope! Unless your battery is the same chemistry you cannot, boosted uses lifepo4 we mostly use lithium-ion, they have different voltage ranges
```

---
## \#7 Posted by: Brdchris Posted at: 2018-08-16T23:20:09.383Z Reads: 66

```
Luna cycle makes a good charger and have different options. I got mine from total battery solution but shipping from China cost as much as the charger. Would have done Luna if I realized.
```

---
## \#8 Posted by: strattos Posted at: 2018-08-17T00:03:49.271Z Reads: 59

```
The only reason to precharge cells is to do a capacity test on them to try and have your p groups as close to each other in total capacity. This takes way to much work typically and you can kinda cheat it by testing internal resistance and making p groups based off that.

As for the charger, it'd probably work in a pinch but it could also overcharge your batteries if you have a cheap BMS, so Imo not worth it. The finishing voltage is 4.0 volts higher than it should be where as my Chinese charger reads at 52V and charges to 50.4 (I had to turn it up from 51v as it wasn't fully charging.
```

---
## \#9 Posted by: Itsmedant Posted at: 2018-08-17T13:13:49.018Z Reads: 32

```
Yea i saw that they use the lifepo4, but everytime I searched for the differences in chargers it never really was clear if you could use them back and forth.

Thanks for the quick reply! Time to buy a charger!
```

---
## \#10 Posted by: Marsen Posted at: 2018-08-18T01:35:30.573Z Reads: 19

```
My choice is to charge them before building. The reason for this is that a balancing circuit in a standard BMS only  balances at about 100mA some are as low as 20mA. If you have cells that are at different charge states then it can take weeks of discharging and charging to fully balance the pack. The balancing circuit only comes on at charge. Cheaper circuits will only work at the full charge voltage. ie when a cell reaches 4.2 volts the extra charge is dissipated through the balancing circuit. Which can only cope with 100mA's. the voltage will continue to rise till the overvolt level is reached and the charging process stops till the the voltage drops to safe levels. The other issue for Lithium cells is that they do not conduct current when fully charged so the cells in series after the charged cell don't get charged, which is why without a balancing circuit or voltage protection the voltage will continue to rise and damage the cell. More expensive BMS's will start balancing at a lower level of about 4V's as they have active control circuits rather than just a purely passive system.
Anyway if you want a balanced battery pack from the start then fully charge each cell at the beginning. A good charger is also important otherwise you may still get different levels of charge state. The BMS will always protect the cells from overvolt so with a BMS you are safe so an unbalanced pack will mean you are not utilising the full capacity of your battery.
```

---
