# What to look out for when upgrading battery to a higher mAH?

### Replies: 11 Views: 961

## \#1 Posted by: naytreeee Posted at: 2017-06-03T16:25:49.376Z Reads: 117

```
My current board has a 10s 2200 mAH battery. I am trying to upgrade it to a LG Chem 18650 MJ1 (3500mAH) 10s . What kind of things should I be worried about? 

Only thing i'm worried about is that the board has an xt30 connector, and 16 awg wiring. Will those parts burn out if I upgrade the battery to 3500mAH?

Thanks!
```

---
## \#2 Posted by: Tuomalar Posted at: 2017-06-03T17:47:39.987Z Reads: 99

```
What board you have? That battery is very small.

I don't recommend those cells. Discharge is only 10A
```

---
## \#3 Posted by: naytreeee Posted at: 2017-06-03T17:57:11.437Z Reads: 99

```
Just a Blink S. It uses 18650 batteries, so I just want to put a higher capacity 10s battery in there. 10A is fine. The current one only has 10A batteries in them (https://batterybro.com/products/samsung-22p-icr1865022p-2150mah-10a)
```

---
## \#4 Posted by: Achmed20 Posted at: 2017-06-03T22:27:53.515Z Reads: 88

```
what you want to do is adding additional batteries in paralel, which should be 2200mah as well or otherwhise you will have  a hard time charging them
```

---
## \#5 Posted by: naytreeee Posted at: 2017-06-04T02:42:05.901Z Reads: 69

```
Well, I can't put them in parallel because there's not enough space. I just want to up the capacity of the batteries. I just don't know if I'll need thicker wires since i'll be throwing in a 3400 mah battery at 10C. The current wire that connects from the board to battery is only 16 awg.

I just wanted to remove the 2200mah 10s battery and replace it with a 10s 3400 mah battery.
```

---
## \#6 Posted by: Iceni Posted at: 2017-06-04T07:57:12.247Z Reads: 53

```
If the discharge rating on the new batteries is the same as your old ones there shouldn't be any problems just switching them out.

Even if the new ones are higher discharge it shouldn't matter, since the rest of the system is based on the old cells and most propably won't draw more than it did previously.
```

---
## \#7 Posted by: naytreeee Posted at: 2017-06-04T17:09:13.487Z Reads: 42

```
Thanks for the reply man! Yes, I wasn't sure if I needed to replace the 16 to 12 awg. Didn't want to put the new batteries and have the wires melt. I guess I'll go give it a try.
```

---
## \#8 Posted by: Aeroquiv Posted at: 2017-06-06T05:56:10.561Z Reads: 33

```
If the board didn't burn down with 16 awg, it won't burn down if you change to the same type of batteries. The ESC controls how much current to pull from the battery, so if Acton specced the board correctly, it shouldn't pull any more current than when it came stock. The problem with MJ1's is that their max continuous current is only 10A. They're only good if you build huge parallel packs, since it will share the load. If you know for sure the board pulls less than 10A, then yea it'll be fine. Otherwise, I'd recommend the LG HG2 or Samsung 30Q. They're only 3000 mah, but they'll handle double the current.
```

---
## \#10 Posted by: naytreeee Posted at: 2017-06-06T06:18:26.022Z Reads: 35

```
@Aeroquiv 

Thanks so much for answering in detail!

But yea, I'm sure! These are the current batteries in the board (https://batterybro.com/products/samsung-22p-icr1865022p-2150mah-10a) in a 10S configuration.
```

---
## \#11 Posted by: Aeroquiv Posted at: 2017-06-06T06:43:35.492Z Reads: 34

```
I would also look into the Sanyo NCR18650GA. It handles high current better than the MJ1 and stays cooler as well, but the data sheet states that the GA will retain only about 65% of its nominal charge within 300 cycles at 6A discharge, while the MJ1 will retain 80% of its nominal charge within 400 cycles at 4A discharge. It's not apples to apples, but perhaps the MJ1 will fair worse at higher current levels. Without data to back it up, I couldn't say. Something to think about.

Either way, by 500 charges, you'll still have more than the 22P's that came with the board.
```

---
## \#12 Posted by: naytreeee Posted at: 2017-06-07T01:42:50.829Z Reads: 28

```
@Aeroquiv thanks a lot man! I will go ahead and go with the  NCR18650GA. that sounds good. I just want to extend the range just a little bit more and that battery will be perfect.
```

---
