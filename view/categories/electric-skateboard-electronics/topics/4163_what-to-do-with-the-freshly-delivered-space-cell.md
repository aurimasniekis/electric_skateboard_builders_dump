# What to do with the freshly delivered Space Cell?

### Replies: 13 Views: 968

## \#1 Posted by: Djupex Posted at: 2016-06-02T21:16:38.174Z Reads: 140

```
Hello everyone!
Short question.
I just got my battery for the raptor but have no board for the upcoming weeks.
Do you think its a good idea to just let it sit around (32% currently) or should I charge it up?
Thanks
```

---
## \#2 Posted by: Jinra Posted at: 2016-06-02T21:23:11.021Z Reads: 138

```
40% is about the best state to leave lithium based batteries at for storage. 32% is good too. Keep it in a cool/dry place and it should be ready to go when you have your raptor!
```

---
## \#3 Posted by: Djupex Posted at: 2016-06-02T21:36:00.216Z Reads: 137

```
Thanks! Ill charge it up for a bit and then its going to see the inside of a cold dark place in my apartment ;-)
```

---
## \#4 Posted by: Randyc1 Posted at: 2016-06-03T01:04:47.590Z Reads: 114

```
40% of 42v ??
```

---
## \#5 Posted by: CSN Posted at: 2016-06-03T01:15:36.741Z Reads: 112

```
For 18650's I think the recommendation is 3.7 volts per cell for longterm storage

https://batterybro.com/blogs/18650-wholesale-battery-reviews/77975750-how-to-store-18650-batteries-safely
```

---
## \#6 Posted by: Jinra Posted at: 2016-06-03T01:24:58.984Z Reads: 106

```
42v is full charge so yes. Unless I'm misunderstanding your question.
```

---
## \#7 Posted by: treenutter Posted at: 2016-06-03T01:47:28.044Z Reads: 105

```
@csn All the new 18650 cells I've receive ship at 3.6-3.65V. That would, presumably, be the ideal storage voltage from the factory. That's for Samsung 25R.
```

---
## \#8 Posted by: chaka Posted at: 2016-06-03T01:51:03.845Z Reads: 102

```
Edited:

You are not accounting for voltage settling after the charger shuts off. Charge to 3.7 and the voltage settles to 3.65v after a bit of time.
```

---
## \#9 Posted by: Djupex Posted at: 2016-06-03T05:58:02.327Z Reads: 82

```
Haha guys! Im a total noob when it comes to these electronics.
My space cell (enertion) is currently 32% charged and my question was, whether to charge it or not until the raptor arrives in a few weeks

And id love someone to explain these 3.65 or 3.7V per something :smile:
```

---
## \#10 Posted by: philipp Posted at: 2016-06-03T08:11:30.117Z Reads: 72

```
Your charging-display monitors the voltage over your batteries.

I don't know the settings of the voltage meter that enertion uses, but normally 4.1V per Cell means full and 3.3V per cell means emtpy.

4.1V(full) - 3.3V(empty) = 0.8 Volts.
0.8V / 100 * 32(your percentage) = 0.256 V left.
3.3V + 0.256V = 3.556

Your cells seem to be around 3.556V wich is slighty below optimum storage voltage.
If you want, you can charge your battery to 40%, this should also balance out all the cells.



If I'm wrong, I'd be glad to be informed :slight_smile:
```

---
## \#11 Posted by: Djupex Posted at: 2016-06-03T08:38:02.044Z Reads: 66

```
Alright! Thanks, seems legit!
```

---
## \#12 Posted by: treenutter Posted at: 2016-06-03T13:31:17.079Z Reads: 51

```
Thanks @chaka. Does voltage sag occur without an electrical load? I'm testing all of these cells individually with a multimeter. They aren't connected to anything yet, just fresh out of the box.
```

---
## \#13 Posted by: chaka Posted at: 2016-06-03T14:19:24.093Z Reads: 48

```
I edited my previous post since using the term "sag" was grossly incorrect and should only be used when describing a circuit under load. 

I don't suspect a factory to trickle charge to a storage state so the voltage will settle quite a bit after charging at 1 amp. If you charge at a much lower amperage the cells will settle much less after removing the charge.
```

---
