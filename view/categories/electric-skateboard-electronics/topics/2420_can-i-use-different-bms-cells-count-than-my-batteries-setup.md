# Can I Use Different BMS Cells Count Than My Batteries Setup?

### Replies: 11 Views: 2472

## \#1 Posted by: laurnts Posted at: 2016-04-17T23:40:03.540Z Reads: 139

```
Exactly like the tittle, I would like to know if I could charge my 6s batteries (lipo / li-ion cells) with higher BMS cells number. I've never seen this being discussed yet, so I would like to see if it does work.
```

---
## \#2 Posted by: lowGuido Posted at: 2016-04-18T00:17:14.320Z Reads: 135

```
no. you can't

----------
```

---
## \#3 Posted by: laurnts Posted at: 2016-04-18T00:34:35.983Z Reads: 137

```
Well thats very sad news. This is might be something for you too @longhairedboy. Apparently not applicable. It does makes sense why BMS'es are being sold per cells basis as they can't be used for different cells.

Btw @lowGuido do you know if BMS actually monitor per cell under-voltage discharge? its clear to me that if it drops below certain voltage that it will cut it off, but what happens if only one of the cells drops at lets say 2.8v while the rest are still 3.4v does the bms protects this as well?
```

---
## \#4 Posted by: lowGuido Posted at: 2016-04-18T00:53:50.055Z Reads: 129

```
there are different BMS' but the most popular ones that I think everyone here uses are resistor BMS'.
first and foremost if the over all pack voltage drops to a pre determined level it will just switch off. thats why you would not be able to use a 6S pack on a 10S BMS. the full charged 6S voltage is lower than the fully discharged 10S voltage. the BMS would simply never turn on because it would believe your pack is over discharged.
secondly, it would be pretty much impossible to have one cell drop to 2.8 and have the others at 3.4 because again the nature of the BMS is that all the cells are joined up and they will always remain at the same voltage. in the case of a resistor BMS if one cell is weak it will simply drag down all the other cells to its voltage, at which point your pack would become kinda crap. It wouldn't last as long as it used to.
at that time you would have to find the damaged cell and replace it so that It doesn't ruin the performance of the other cells..

however in a perfect world this shouldn't happen because all the cells being linked via BMS they should all charge and discharge the same and therefore weaken at the same rate.

..in a perfect world..
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-04-18T12:40:47.281Z Reads: 100

```
Yep, resistors. The guys i follow that build ebike packs have told me that most BMSs are great as long as they have the balance resistors. That kind of stuck with me because i thought they were all built that way, but i guess they aren't.
```

---
## \#6 Posted by: killaton Posted at: 2018-11-03T16:50:14.108Z Reads: 47

```
Would that be an issue though if you bypass the BMS during discharge?
```

---
## \#7 Posted by: kuphjr Posted at: 2018-11-03T18:12:06.426Z Reads: 44

```
That’s actually a good question. Could someone with more experience weigh in?
```

---
## \#8 Posted by: lowGuido Posted at: 2018-11-03T23:31:08.832Z Reads: 41

```
If you bypass the pack for discharge then you wilk not have one weak cell affecting your whole pack, but you can't discount the possibility of one cell going bad. The long story short is:
MONITOR YOUR CELLS REGULARLY.  if you have BMS or not doesn't even matter. you should regularly check your cells so that you can see if one is starting to go bad and replace it.
You wouldn't buy a car and then drive it around without ever servicing it. The same tuing applies to batteries.
```

---
## \#9 Posted by: pat.speed Posted at: 2018-11-03T23:56:10.759Z Reads: 36

```
I think @killaton meant can he bypass the bms and use a higher cell bms. For that question, Yes, you can do that. I do for my 12s pack as a 13s bms is cheaper than a 12s and many other people do this too.

The way to do it is you connect it exactly as normal just leaving the last wires of the bms not connected to anything. I think @scepterr said that it works because since the voltage is exactly 0v the bms doesn’t think a cell is connected and continues working as it normally would. But if the last wires had even a slight voltage then it would go to over discharge state. 

But overall Yes it is possible to do this
```

---
## \#10 Posted by: killaton Posted at: 2018-11-05T13:29:28.166Z Reads: 28

```
Yes pat, that was my question. Thanks for the tip. However a loose wire would have a floating voltage, NOT 0. Its likely that this setup works DESPITE the bms being permanently in over discharge protection, precisely because we bypass it during discharge. No?
```

---
## \#11 Posted by: pat.speed Posted at: 2018-11-05T21:35:56.420Z Reads: 25

```
I would have thought the bms pin would read 0v as no voltage is being applied across it.

 I thought about what you said as I wrote the last reply and that is definitely a possible reason and is probably how it works
```

---
