# First time BMSer, Is this wiring diagram correct?

### Replies: 27 Views: 816

## \#1 Posted by: notepad Posted at: 2018-09-23T16:21:11.568Z Reads: 137

```
 Hello all,  I have been trying to figure out how to correctly wire up 4, 6s lipos into a 12s2p pack with a BMS

The [Bms that Im using](http://www.batterysupports.com/44v-48v-504v-12s-150a-12x36v-lithium-ion-lipolymer-battery-bms-p-394.html) has instructions, albiet in chinglish so I am hesitant to just solder things up without getting advice first.
Ontop of that each lipo has 7 balance connectors instead of 6 - 6 black cables, one red (turnigy graphene 6s 8Ah)

Any help you guys can give would be amazing!!

![bms%20drawing|690x332](upload://4HkjQKarjhedtu4dT62my1wIfxt.png) 
p.s I did ask this twice on noob questions thread, but to no avail as I dont like cluttering up main chat with basic questions.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-23T17:55:50.887Z Reads: 116

```
Look up this thread everything should be explained there.
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/24

I‘m not lipo expert but I know that if you balance charge cells in parallel every single cell need to have nearly the same voltage and internal resistance. If not you can mess them up or in the worst case fire them up.
```

---
## \#3 Posted by: notepad Posted at: 2018-09-23T18:00:52.161Z Reads: 108

```
[quote="Andy87, post:2, topic:68975"]
I‘m not lipo expert but I know that if you balance charge cells in parallel every single cell need to have nearly the same voltage and internal resistance. If not you can mess them up or in the worst case fire them up.
[/quote]

I was under the impression that those internal cells should auto balance within the 6s2p. if this isnt the case, how would I get all the cells auto balancing.  ?merging the balance connectors together so when they are charging they balance?
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-09-23T18:18:00.731Z Reads: 85

```
not much help but you've made an awesome purchase with those graphenes, they're amazing batteries
```

---
## \#5 Posted by: Andy87 Posted at: 2018-09-23T18:18:29.304Z Reads: 80

```
Don’t want to say you something wrong, so better to call people with more experience.
@PatRocks @deucesdown @Kug3lis @Namasaki maybe you can explain what to take care about if balance charge lipos?
```

---
## \#6 Posted by: notepad Posted at: 2018-09-23T18:19:03.884Z Reads: 77

```
Thankyou, I was able to get them on sale for £45ea. I couldnt say no. even if it means stepping down from the 16Ah multistars
```

---
## \#7 Posted by: mynamesmatt Posted at: 2018-09-23T18:19:51.177Z Reads: 76

```
oh they will be so so so much better than multistars
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-09-23T18:23:50.727Z Reads: 74

```
P group balance connectors connect in parallel and series connect together there first negative side group last connects together with first positive side group first balance pin
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-09-23T18:27:18.354Z Reads: 71

```
Like this:

![58%20PM|535x500](upload://6hQCzu1pMjBAIrCgZfdJ1t1bjmt.png)
```

---
## \#10 Posted by: deucesdown Posted at: 2018-09-23T18:28:03.502Z Reads: 67

```
[quote="notepad, post:3, topic:68975"]
I was under the impression that those internal cells should auto balance within the 6s2p. if this isnt the case, how would I get all the cells auto balancing. ?merging the balance connectors together so when they are charging they balance?
[/quote]

I think this is an overly complicated way to think about this. The phenomenon you're talking about is explained by this:

If you connect 2 cells together in parallel, with slightly different voltages, the act of connecting them together will force them to be at the same voltage. Energy will flow from the "more full" cell to the "less full cell". If you leave the cells connect together, this will happen all the time.

This activity happens at the cell level, not the pack level. It's not automatic nor magical. You must connect each cell in parallel to get this action. For you, this means, you must:
- splice each wire in the balance connector for 2 packs. This gives you a pair of 6s2p packs. Note, this is a 3 way splice, as you need a wire coming out to connect to the bms.
- Then join the 6s2p packs in series to get 12s2p. The power leads will have to be joined in series. The balance leads, kug3lis diagram is perfect.
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-09-23T18:31:14.944Z Reads: 64

```
Ahh I see your BMS has 12 pins and first of balance connector goes to battery GND just double check if first pin on your lipo is negative

![18%20PM|475x486](upload://2tin2OGuWtEkcBjHlI218O4jdgO.png)
```

---
## \#12 Posted by: notepad Posted at: 2018-09-23T18:32:45.173Z Reads: 58

```
Ahh I see.  that diagram is amazingly helpful!!
```

---
## \#13 Posted by: notepad Posted at: 2018-09-23T18:45:12.141Z Reads: 53

```
> * splice each wire in the balance connector for 2 packs. This gives you a pair of 6s2p packs. Note, this is a 3 way splice, as you need a wire coming out to connect to the bms.
>* Then join the 6s2p packs in series to get 12s2p. The power leads will have to be joined in series. The balance leads, kug3lis diagram is perfect.

So the act of  splicing the balance connectors together is what lets the cells self balance just by sitting / auto balance during charging.  Then just wire up the two packs like normal for 12S and it should be good??
```

---
## \#14 Posted by: deucesdown Posted at: 2018-09-23T18:49:29.373Z Reads: 51

```
One further clarification. With respect to self balanceing -- the only cells affected are the ones connected in parallel. Series guys have to be balanced (if needed) actively by a balance charger or the balancing circuits in a bms.
```

---
## \#15 Posted by: notepad Posted at: 2018-09-23T18:50:34.532Z Reads: 51

```
SO as long as All charging is done through the bms everything should be fine?
```

---
## \#16 Posted by: deucesdown Posted at: 2018-09-23T18:54:00.107Z Reads: 45

```
The answer to this type of question must be earned through reading research and testing. :)
```

---
## \#17 Posted by: notepad Posted at: 2018-09-23T18:58:36.975Z Reads: 43

```
Fair enough, I do thank you for your amazing assistance! both you and @Kug3lis - I can finally finish the build! 

The only other thing was the charging port location and polarity. but since no one has mentioned it Im guessing I got it correct!.

And Again, Thank you!
```

---
## \#18 Posted by: deucesdown Posted at: 2018-09-23T19:05:42.918Z Reads: 44

```
Hey one more thing in your diagram on the bms you have "P+". I think it's really "P-"?

Okay I lied, another thing. You want a fuse (important), loop key and/or /switch?
```

---
## \#19 Posted by: notepad Posted at: 2018-09-23T19:12:05.189Z Reads: 46

```
Your absolutely right, It should be P-  My mistake!!

I Am definitely going to have a xt90-s loop key to interrupt the circuit. but also to isolate the Vesc's while charging. However I didn't consider a fuse.  would soldering 5, 30A car fuses together in parallel do the trick, or should I look for a specific fuse of the correct rating?

Edit. Is a fuse even needed? as I see lots of people forgo one in favour of a decent bms and loopkey
```

---
## \#20 Posted by: Andy87 Posted at: 2018-09-23T19:15:53.215Z Reads: 45

```
If you go with a fuse and 12s look for 58v fuses not the 32v ones
```

---
## \#21 Posted by: deucesdown Posted at: 2018-09-23T19:17:19.524Z Reads: 40

```
[quote="notepad, post:19, topic:68975"]
. Is a fuse even needed
[/quote]

Everyone must decide for themselves what acceptable risk is.

But the safe approach is to have many layers of protection. Everything can fail. What would happen when this or that part fails? If the answer is "fire" you need to do better.

The fuse will be the last line of defense for your pack. Don't go cheap, get the right type, and size it perfectly. :)
```

---
## \#22 Posted by: notepad Posted at: 2018-09-23T19:20:30.388Z Reads: 39

```
> The fuse will be the last line of defense for your pack

That definitely sold it to me, Ive already killed 3 multistar ones (never figured out how since they would just suddenly drop to 0V) so I really dont want to ahve to buy more 

@Andy87 58V, Ill make sure not to get the wrong ones,  thanks for the heads up!

Strangely enough its really hard to find a decent fuse. I think [THIS](https://www.amazon.co.uk/Holder-Inline-100amp-Yellow-Marine/dp/B07DY1BDZ9/ref=sr_1_2?ie=UTF8&qid=1537730937&sr=8-2&keywords=100+amp+inline+fuse) is good enough but if not I can just get the fuses on their own and manually solder them inline!
```

---
## \#23 Posted by: notepad Posted at: 2018-09-24T00:28:10.103Z Reads: 34

```
Well BMS is on order.  now comes the scary part of actually wiring it up.

For someone with a mild phobia of electricity, I sometimes wonder why I do this to myself - but if it works its going to be worth it!
```

---
## \#24 Posted by: Pmac Posted at: 2018-09-24T06:34:13.474Z Reads: 33

```
If you have a hobby charger I would storage charge the batteries first which means they are all balanced at 3.7 or 3.8 volts.  That way when you connect the batteries in parallel they are all either the same or 0.01v out.

With lipos if the voltage of the parallel cells you are connecting are too far out you can not only ruin the cells you are connecting but cause a fire due to the inrush of current.  Please be very careful.
```

---
## \#25 Posted by: notepad Posted at: 2018-09-24T18:27:02.173Z Reads: 31

```
Would that also work if I just balance charge them to 4.2V  as discharging each battery on my charger will take days each.
```

---
## \#26 Posted by: Pmac Posted at: 2018-09-25T01:33:43.851Z Reads: 32

```
Yes it would.

They all just need to be the same voltage.

But you do not want to leave the batteries fully charged if you aren't going to use them for days as Lipo's start to wear quicker if always left fully charged.  Which is why I suggested balancing them to 3.7/3.8 volts.  Just from how I work as i only get weekends to work on my boards (if that) so it is better for the batteries to keep them at the storage charge while working on them.
```

---
## \#27 Posted by: AreaKruzer Posted at: 2018-09-25T02:06:34.690Z Reads: 31

```
lipo tend to bloat up too if they are left at full charge for prolong periods.
```

---
