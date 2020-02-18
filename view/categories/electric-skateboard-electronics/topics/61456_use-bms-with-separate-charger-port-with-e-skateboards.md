# Use BMS with separate charger port with e-skateboards

### Replies: 12 Views: 1067

## \#1 Posted by: alessandroemm Posted at: 2018-07-10T13:36:51.785Z Reads: 150

```
Hey there

 I thought i was being smart when I bought my BMS(es) with a separate chargeport (there was obviously a combined version as well). It is only now that i realise that a skateboards actually brakes using recuperation. So short story shorter: can a BMS with a separate port be used generally speaking?

Thanks a lot 
Alessandro
```

---
## \#2 Posted by: dino15309 Posted at: 2018-07-10T13:54:55.047Z Reads: 139

```
Post a picture of its diagram or the link to where you bought it. That will make it easier for us to help you.
```

---
## \#3 Posted by: alessandroemm Posted at: 2018-07-10T21:10:20.514Z Reads: 120

```
Hey Dino 

I'm not sure whether it is going to help the informations  on the sellers site are a little sparse.

https://de.aliexpress.com/item/10-s-36-v-Lithium-Batterie-Schutz-Bord-BMS-mit-balance-Wasserdichte-18650-lipo-Li-Ion/32839578059.html?spm=a2g0s.9042311.0.0.27424c4dQcb6cM

Thanks for your feedback
Alessandro
```

---
## \#4 Posted by: dino15309 Posted at: 2018-07-11T00:37:49.682Z Reads: 94

```
That looks normal. If you are referring to the fact that it has the balance lead, you are fine. Every BMS has those exact leads and ports. I was going to get a similar bms, but it has a positive lead, negative lead, and negative charge lead. All BMS's have the balance leads though.

I hope this helps
```

---
## \#5 Posted by: pjotr47 Posted at: 2018-07-11T00:40:32.276Z Reads: 92

```
I think @dino15309 understand it wrong...
Almost every bestechpower BMS have an separate charge port and regeneration just works fine
```

---
## \#6 Posted by: dino15309 Posted at: 2018-07-11T01:40:51.426Z Reads: 86

```
Yea I dont think I did. I've never used bestechpower before so I shouldn't have replied. Sorry about that.
```

---
## \#7 Posted by: alessandroemm Posted at: 2018-07-11T06:33:07.372Z Reads: 75

```
Any clue then why the port is separated? After all thats would be just costlier, wouldn't it? The weird thing with these BMS is that the ones with the separate Port are actually cheaper, which sounds like the were able to make the board simpler with the separation and thus drive cost down.
```

---
## \#8 Posted by: pjotr47 Posted at: 2018-07-11T14:31:50.237Z Reads: 69

```
Haha no prob :p It's nice that you want to help ;)
```

---
## \#9 Posted by: pjotr47 Posted at: 2018-07-11T14:32:19.902Z Reads: 71

```
I have no clue about that. What is some euro's on the total price? Nothing ;)
```

---
## \#10 Posted by: DerelictRobot Posted at: 2018-11-23T21:54:56.843Z Reads: 52

```
I believe you're correct. It's my understanding that there are two methods in which the battery takes in a charge current. The charge port on the BMS charges via the balance connectors, where the regen current comes from the ESC, which comes into the main battery connection (I believe this comes in as an unbalanced "quick charge"). I could be incorrect though, most of my experience in this involves building large lipo packs.

I'd be curious how the combined charge/discharge BMS variants handle the charge current input from a charger vs regen. I can't imagine it tries to balance charge the regen current? And I would think the combined variant would be more complex and therefore be more expensive, but they seem to be about the same price. I'm by no means a DC power systems expert, anyone care to chime in? @chaka ?
```

---
## \#11 Posted by: chaka Posted at: 2018-11-24T03:28:30.345Z Reads: 45

```
Actually no charging takes place via the balance cables, they only bleed of the excess voltage when the battery is being topped off. They keep the high cells in check while the rest catch up. There are exceptions but the common BMS units work this way.

Usually a BMS will only be able to discharge a high cell at a very small rate, about 0.10 Amp per cell. Not much help when you have a full battery and you are pumping in a heavy regen current.
```

---
## \#12 Posted by: DerelictRobot Posted at: 2018-11-24T03:37:25.526Z Reads: 43

```
Wow, TIL. Quite different from the BMS modules we used to build out big lipo packs. That makes sense though, active balancing via regen didn't sound like something these were capable of.

Thanks!
```

---
