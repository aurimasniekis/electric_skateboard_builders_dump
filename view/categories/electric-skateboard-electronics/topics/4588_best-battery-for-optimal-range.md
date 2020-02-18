# Best battery for optimal range

### Replies: 15 Views: 4976

## \#1 Posted by: Sk8M8 Posted at: 2016-06-12T06:29:36.926Z Reads: 416

```
What are some commonly used batteries that perform well and have huge capacities?
```

---
## \#2 Posted by: zk8_builder Posted at: 2016-06-12T07:04:14.929Z Reads: 424

```
18650 are most common
```

---
## \#3 Posted by: lowGuido Posted at: 2016-06-12T07:57:22.161Z Reads: 426

```
18650's in large series/parallel combinations, or big mAh Lipos.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-06-12T09:42:24.281Z Reads: 414

```
Especially Low C rated Multistar lipos! Because of the low C they have less acceleration but  bit more range
```

---
## \#5 Posted by: whitepony Posted at: 2016-06-12T09:55:12.689Z Reads: 412

```
there is no "best" cell, it really depends on the size of your battery and the power you plan to drain from it. if you have a superlarge battery with 60+ cells, you can go for max capacity low drain cells. if you however  run intermediate battery sizes like 40 or even less, it becomes much less of a no brainer, since you also need a certain power off the battery. usually you'd have to change to higher drain cells which typically come with less capacity.

currently, on the 18650 market, the very best cells by discipline have:

* 30A continuous current with 2500mAh (VTC5)
* 20A continuous current with 3000mAh (LG HG2)
* 10A continuous current with 3500mAh (Samsung 35E, Sanyo GA, LG MJ1)
```

---
## \#6 Posted by: lox897 Posted at: 2016-06-12T10:01:40.406Z Reads: 390

```
I thought Samsung 25Rs were 20A or 22A continuous? According to this datasheet: https://www.powerstream.com/p/INR18650-25R-datasheet.pdf
```

---
## \#7 Posted by: whitepony Posted at: 2016-06-12T10:15:48.074Z Reads: 380

```
hm, you are right - I seem to remember that the 25Rs had one of the lowest internal resistance of all contenders, but maybe not. removed it from the list! :confused:
```

---
## \#8 Posted by: Nordle Posted at: 2016-06-12T10:29:52.820Z Reads: 379

```
[quote="DeathCookies, post:4, topic:4588, full:true"]
Especially Low C rated Multistar lipos! Because of the low C they have less acceleration but  bit more range
[/quote]
no :hand_splayed: :poop:
```

---
## \#9 Posted by: Sk8M8 Posted at: 2016-06-12T17:34:56.978Z Reads: 353

```
I worded the question poorly. I was thinking more in terms of prebuilt lipo packs.
```

---
## \#10 Posted by: AbrownMN Posted at: 2016-06-12T23:20:48.019Z Reads: 332

```
Same idea applies. Depends how much power to plan to drain from it consistently, it's output, the MAH rating and how you wire them up. Connecting them in series will increase the voltage ( power output), connecting them in parallel will increase your MAH rating (range).
```

---
## \#11 Posted by: DeathCookies Posted at: 2016-06-13T11:37:05.352Z Reads: 307

```
Why not? Can You explain it in more detail? 
That was said by personel experiences with a 8 Ah 6S Multi Star and the same setup with a 8 Ah 6S Zippy
```

---
## \#12 Posted by: Nordle Posted at: 2016-06-13T16:28:48.227Z Reads: 296

```
I can't but you can read it all over the web, the multistars just will blow up earlier if you draw to much amps from them. Your Zippys are probally not true 8000mah or older than your other pack.
```

---
## \#13 Posted by: Hummie Posted at: 2016-06-13T16:46:08.506Z Reads: 288

```
I've read good things about the multistar on rcgroups by a guy who does legitimate testing.  On es on the other hand they're said to be actually 4c.  But if u make a big pack and don't over draw from them they're the cheapest thing out there it seems and as good a cycle life as any other lipo. I got 16ah 12s for 150$. 
The best energy density by weight for lipos are these multistar I think but they still don't come close to the 3500 li-ion cells, either 3000 or 3500mah in that challenge
```

---
## \#14 Posted by: Nordle Posted at: 2016-06-13T17:26:19.200Z Reads: 278

```
I don't say in anyway that that multistars are bad. I think to buy some cause they are so cheap:)
```

---
## \#15 Posted by: evoheyax Posted at: 2016-06-13T19:00:27.018Z Reads: 266

```
The question you asked leads me to believe you don't fully understand how to get optimal range. It's ok, thats what we are here for :slight_smile:

Optimal range infers efficiency, but if you want efficiency, the place to look is not the battery, but the motors and mechanical system together.  What kv motor you use, along with the reduction ratio of your gearing will make the most impact on efficiency. On the space cell and 1:1 gearing ratio with 149 kv motors (essentially a non-efficient system), I can get about 6 miles tops. With 190 kv motor, and a 3:1 ratio, I've seen people get 10 miles, maybe more. 16000 mah at 6s and a 3:1 gearing ratio on a single drive r-spec got me about 18 miles. The same on the 149kv 1:1 gearing, got me 8 miles. So it really comes down to the efficiency of your drive system and motor, more than the particular battery. The energy your system needs is the energy you need. You can reduce the energy you need not in your battery, but in your drive system and motor combo.

For me, 6s zippy 8000 mah have been amazing. Had them in parallel for 16000 mah and got great range. Then put em in series, less range, but more torque. The reason I choose them is the high mah, and the fact you can switch between 6s and 12s so easily.
```

---
