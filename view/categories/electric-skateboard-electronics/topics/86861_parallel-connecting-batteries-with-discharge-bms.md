# Parallel connecting batteries with discharge BMS

### Replies: 8 Views: 237

## \#1 Posted by: humanisticnick Posted at: 2019-03-11T15:04:52.501Z Reads: 61

```
If I were to take two of these:

http://www.diyeboard.com/10s5p-18650-lithium-battery-pack-36v-10ah-360wh-p-460.html

and connect them in parallel does that mean that since each one has a discharge BMS of 50amps that the new max discharge would be 100amps or does it not work like that?

Also in this scenario would they need to be charged individually or could I splice the charging ports together and it would just charge slower.

Not a battery/electric pro, any help would be appreciated.
```

---
## \#2 Posted by: akhlut Posted at: 2019-03-11T15:15:53.049Z Reads: 60

```
You effectively have a 10S10P battery.   Why charge them as a single unit?  Two chargers means half the time on charge - this is a good thing.  Faster to charge, faster to balance. 

And yeah, series boosts voltage, parallel boosts current.  Together they should be able to deliver 100A.
```

---
## \#3 Posted by: Fraserrazor Posted at: 2019-03-11T15:59:47.338Z Reads: 53

```
Do take into consideration that this battery does use cheap cells which will be liable to outputting reduced continuous current than stated. These batteries also have terrible voltage sag so do not expect nearly as much range as a 10s6p of quality cells using samsung 30Qs wiring these two packs in parallel. It would be a lot easier rebuilding the pack and using only one BMS as splicing charge ports will pose the problem of delivering insufficient current and a very long wait till full charge as the current output of the charger will halve at the parallel junction of the splice so you would need at least a 4A charger (2A to both packs).
```

---
## \#4 Posted by: humanisticnick Posted at: 2019-03-11T16:51:25.339Z Reads: 42

```
I understand I'm just having a hard time finding anyone willing to sell a 30Q battery pre-built at a competitive cost. I bought a TB 12s4P 30Q and it arrived non-functioning for $480 ( I am going to have to pay return shipping as well). I already have one of these el' cheapo batteries and it has worked well (besides the sag) for a while. Two of these are ~$350 shipped, 3 for $500. The weight will suck, but at $500 I could have 10s15p even with the cheap cells that will be a tremendous amount of range/power. It's just an idea at this point.
```

---
## \#5 Posted by: Fraserrazor Posted at: 2019-03-11T17:24:06.900Z Reads: 38

```
True I'm only speaking as I have the same pack in my build. One thing I will say though is a charger supplying beyond 4A can be expensive and  become very hot whilst charging. The 15p would be sweet as but if you want 2A charging current per pack you'll need a 6A charger like this one from aliexpress https://www.aliexpress.com/item/42V-6A-charger-for-10S-Li-ion-battery-pack-4-2V-10-42V-battery-smart-charger/32812089700.html

Where are you based? Sometimes filling in your bio information can really help source battery builders locally.

Lastly, from experience these batteries do weigh a lot but they are also quite tall so this would be a monster to fit under most builds assuming two or more packs. This would also need a custom enclosure to match the stack as the packs would need to be close to one another to splice the charging ports. The output connector is an XT-60 just for your information so you would need an XT-60 parallel harness to wire the packs in parallel without solder.
```

---
## \#6 Posted by: humanisticnick Posted at: 2019-03-11T17:56:28.128Z Reads: 33

```
I'm located in Pittsburgh PA USA. I'm planning on 3D printing the enclosures as individual ~cells~ one enclosure for each 10s5p and either cutting a channel in the top of the board to route the cables under the grip tape (like many cheapo boards) or even running the wires between the cells in a thin rubber hose (to avoid drilling into my deck). I'm thinking running all the xt60's to the 4th enclosure with my vesc and then manually soldering the 3 xt60s to 1 xt90, then anti spark, then VESC. Like I said it's just an idea now but I'm warming up to it myself. I just need to mock up an enclosure and make sure everything will fit under the board.
```

---
## \#7 Posted by: Fraserrazor Posted at: 2019-03-11T18:36:53.463Z Reads: 32

```
Be careful of how long you battery wire is to the vesc as if it is too long you can get induced voltage spikes that can fry the vesc. Just a heads up as I know many new builders have not come across this information so it may be worth reading up on it. If your board has flex then having a third battery slap bang in the middle may have grounding issues when riding. What vesc are you using? Most VESCs are rated at 50A continuous. Just asking so you don't go on a buy rampage and make a mistake :+1:
```

---
## \#8 Posted by: humanisticnick Posted at: 2019-03-11T18:40:47.020Z Reads: 31

```
I already have a FSESC dual 6.6 and everything else lol. Deck, trucks, mounts, remote, 2 6374s. I  was all ready to go but my battery kept giving me issues that's why I'm entertaining alternatives.
```

---
