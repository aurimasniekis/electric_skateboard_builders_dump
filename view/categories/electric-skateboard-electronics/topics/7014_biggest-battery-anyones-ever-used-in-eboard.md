# Biggest battery anyones ever used in eboard?

### Replies: 48 Views: 3470

## \#1 Posted by: evoheyax Posted at: 2016-08-02T16:02:31.612Z Reads: 367

```
Just curious as to how big of a battery some of you are using? I'm building a pack right now which is a 12s 16000 mah, which is massive 710 Wh. Never heard of anyone using a battery this large,

So whats the biggest anyone's used before?
```

---
## \#2 Posted by: sl33py Posted at: 2016-08-02T16:06:12.552Z Reads: 371

```
probably biggest i know about being used is probably @chaka's.  6-700 Wh iirc.

I'm a fan of smaller lighter setups - ideally swappable if i want to go further distance.  A spare battery in my bag or pocket is easier to carry than more weight under my board IMO.  Different strokes for different folks!
```

---
## \#3 Posted by: barajabali Posted at: 2016-08-02T16:09:29.277Z Reads: 365

```
I use a 10s8p on my mountain board. 720 WH
```

---
## \#4 Posted by: XIII Posted at: 2016-08-02T16:10:23.231Z Reads: 359

```
What about the guy who build a 13p battery out of laptop cells? 

Never saw a picture though
```

---
## \#5 Posted by: barajabali Posted at: 2016-08-02T16:11:09.928Z Reads: 352

```
How is your pack 806? if youre using liion your nominal is 3.6 volts/cell. so 3.6 * 12= 43.2   and 43.2 * 16= 691.

and lipo is still only 710.   From what i know i have the biggest pack lol   even the 13P pack is smaller due to old cells.  I remember calculating it.
```

---
## \#6 Posted by: evoheyax Posted at: 2016-08-02T16:13:06.404Z Reads: 348

```
ok, maybe I did it wrong. I did the calculation at 4.2 volts per cell, since that's a full charge.

You do the calculation at the lowest voltage per cell?
```

---
## \#7 Posted by: barajabali Posted at: 2016-08-02T16:14:04.534Z Reads: 341

```
 you do it at nominal so 3.6 for liion and 3.7 for lipo.  3.2 for lifepo
```

---
## \#8 Posted by: evoheyax Posted at: 2016-08-02T16:15:54.291Z Reads: 339

```
ok, I'll edit that than, thanks for the heads up. It's a lipo 12s2p. multistar pack, aka, the weaksauce filled packs, but they won't be weak at this size.
```

---
## \#9 Posted by: barajabali Posted at: 2016-08-02T16:17:14.270Z Reads: 333

```
Yea if you run them at 2p then theyre fine.  ive done a 10s2p with multistar before and it was totally fine :)
```

---
## \#10 Posted by: evoheyax Posted at: 2016-08-02T16:26:48.489Z Reads: 326

```
Do you know how many amps you've pulled from them at once? I might be building an over kill, but I'm build a 4wd with these and I want to pull 100 amps (25 per vesc/motor). They advertise 10c discharge, but on ES, some guys said 4c or 5c was really their limit.

How many miles do you get with that massive pack?
```

---
## \#11 Posted by: barajabali Posted at: 2016-08-02T16:33:25.879Z Reads: 307

```
oh man you shouldnt be using multistar for a 4wd board...  mine was find with 2p on a single drive.  your acceleration is gonna tank! I don't know the amp pull sorry!

and its on a dual rear chain drive on 8 in pneumatics I havent measured range yet! but i think itll get me like 30 miles.  on a single drive street board it would get around 55miles
```

---
## \#12 Posted by: evoheyax Posted at: 2016-08-02T16:38:35.488Z Reads: 295

```
Why do you think the acceleration will tank? It's a question of how many amps I can draw.  If I pull 100 amps to one motor or across 4, whats the difference? It's just spreading the work out across the four motors instead of one or two doing it all.
```

---
## \#13 Posted by: barajabali Posted at: 2016-08-02T16:46:32.271Z Reads: 292

```
2 motors pulls about 30% more amps than 1 motor with the same load. 

I'm not sure how that math works out with 3 or 4 wheels but I'm sure it just pulls more amps. 

There is less amp pull PER esc 
But more amp pull from the battery since all the esc's share the same battery
The question is-can that battery give you 100amps.  I don't think it can
```

---
## \#14 Posted by: whitepony Posted at: 2016-08-02T16:52:39.173Z Reads: 277

```
I built a few evolve carbon replacements with 756Wh each. 10S6P with 3500mAh cells :slight_smile:
```

---
## \#15 Posted by: barajabali Posted at: 2016-08-02T16:55:07.345Z Reads: 277

```
I'm honored to be bested by you! Lol my downfall is using 2500 mah cells
```

---
## \#16 Posted by: Nordle Posted at: 2016-08-02T16:56:45.299Z Reads: 274

```
i built the same, but it won't get empty! xD 
_tumnich 4 president!_
```

---
## \#17 Posted by: evoheyax Posted at: 2016-08-02T17:02:14.773Z Reads: 268

```
If there are 10c discharge at 16ah, that's 160 amp discharge. If I pull 100 amps, that's like 6-7c. I guess only time will tell
```

---
## \#18 Posted by: Nordle Posted at: 2016-08-02T17:06:32.515Z Reads: 268

```
But they are actually 4-5C in reality. If you can afford 4 wheel setup, don't save at the wrong place.
```

---
## \#19 Posted by: barajabali Posted at: 2016-08-02T17:09:59.471Z Reads: 267

```
Yea I know that's what the label says but time will tell
```

---
## \#20 Posted by: Mobutusan Posted at: 2016-08-02T17:20:39.231Z Reads: 271

```
Wouldn't the total amps pulled be similar on 2wd vs. 4wd? That same 50 amps would just be split 4 ways instead of 2, right? You're still moving the same load. I'm also going to try a 4wd hub board, and I'm planning on running off a 12s 5200mah multistar, so I hope you should be ok, cause I hope I'm gonna be ok. Lol
I'll hook up my watt meter when I do it and see what's really going on.
```

---
## \#21 Posted by: evoheyax Posted at: 2016-08-02T17:20:43.248Z Reads: 242

```
It's not about money. It's about space. They have the highest density of mAh for the size. If it doesn't work out, I will use another battery. The next best option I could find was half the mAh and only slightly smaller, but a 20c rating.

What would happen if I try drawing more than they can sustained? Will the blow up and catch fire? Or just die early?
```

---
## \#22 Posted by: Nordle Posted at: 2016-08-02T17:22:56.893Z Reads: 243

```
If you draw more amps than it candle handle, you already listed your options:
-blow up
-catch fire
-die early
combinations of these effects also are possible
```

---
## \#23 Posted by: evoheyax Posted at: 2016-08-02T17:55:31.418Z Reads: 236

```
So if accept take them to be 5c, I'm still at 80 amps, or 20 per motor. Right now, I'm running 10s and max amps to 50 total in a dual drive, and only issue I have is heat in motor. With 80 amps at 12s, I assume I should have much more power than 50 amps at 10s, which is hill climbing and acceleration wise fine with me.
```

---
## \#24 Posted by: Nordle Posted at: 2016-08-02T18:05:08.595Z Reads: 226

```
It's possible this will work.
But i would get some 18650's instead. :sunglasses:
```

---
## \#25 Posted by: Kaly Posted at: 2016-08-02T18:06:07.593Z Reads: 231

```
I previously use a 12S 15Ah 30C Lipo on my eMTB.  On this post http://www.electric-skateboard.builders/t/emtb-and-vanguard-built/995?u=kaly

In my experience a 10C Lipo will work but the performance for your application will be average at least you'll be better serve if you go with a higher C rating if you want to get the best of that 4wd setup.
```

---
## \#26 Posted by: Randyc1 Posted at: 2016-08-02T18:09:26.302Z Reads: 242

```
Do you know what the current GT Battery is ??  ?S?P
```

---
## \#27 Posted by: lox897 Posted at: 2016-08-02T22:12:14.007Z Reads: 232

```
10s4P probably about 10-12ah
```

---
## \#28 Posted by: GhettoFab.rictation Posted at: 2017-12-16T08:30:14.633Z Reads: 167

```
What about someone using these 5500 shockli cells or 4200mah ijoy cells to make a crazy long ride? If the 5500 work and someone made a single drive emtb you could make 12s8p with 88000mah hahah!
Shockli: https://www.e-cigarette-forum.com/threads/bench-test-results-shockli-20a-5500mah-26650-accurately-rated-great-choice-for-under-65w.824465/ 
Ijoy: https://www.e-cigarette-forum.com/threads/ijoy-40a-4200mah-26650-bench-test-results-overrated-but-a-great-30a-battery.764411/
```

---
## \#29 Posted by: FredrikHems Posted at: 2017-12-16T10:53:18.093Z Reads: 158

```
No, your math is wrong
In a 12s 8p it would be; 5500mAh* 8= 44000mAh 43.2v* 44Ah= 1900.8wh
```

---
## \#30 Posted by: Youssless Posted at: 2017-12-16T10:57:38.819Z Reads: 156

```
Doesn't V*Ah =Wh? :wink:
```

---
## \#31 Posted by: FredrikHems Posted at: 2017-12-16T14:31:27.333Z Reads: 144

```
You are totally right, that was a typo
```

---
## \#32 Posted by: Acido Posted at: 2017-12-16T14:33:44.295Z Reads: 147

```
My new battery will be 12s6p 30q If everything goes as planned, and that Christmas bonus comes
```

---
## \#33 Posted by: GhettoFab.rictation Posted at: 2017-12-16T21:01:12.835Z Reads: 137

```
This is all hypothetical, but thank you for the correction! Still way better than 10000mah
```

---
## \#34 Posted by: barajabali Posted at: 2017-12-16T21:06:26.280Z Reads: 132

```
12s7p with an additional 12s9p in my backpack. 12s16p total 

Do I hold the record yet? Does it even count? I’d say yes
```

---
## \#35 Posted by: Acido Posted at: 2017-12-16T22:23:24.143Z Reads: 133

```
What cells?
```

---
## \#36 Posted by: Kug3lis Posted at: 2017-12-16T22:33:58.833Z Reads: 137

```
My pack will be around ~1.1kWh at 3.7V
```

---
## \#37 Posted by: notger Posted at: 2017-12-16T22:40:05.815Z Reads: 140

```
With my 5AH Makitas i have 720WH now. 8X18VX5Ah
After finishing my 8X 18V 7,5 Packs it will be 1,1kWh

And to be honest i could really use that. with the altitude i have here in the Austrian Alps a big Battery is not a fault at all for a Daytrip.

http://www.electric-skateboard.builders/t/tramakitoxx-wtf-trampa-makita-e-toxx/30815/14?u=notger
http://www.electric-skateboard.builders/uploads/db1493/original/3X/2/8/2883679892cd92987811b7d1f05d19bcb693323d.JPG
```

---
## \#38 Posted by: E1Allen Posted at: 2017-12-16T23:00:24.152Z Reads: 131

```
I plan on doing 12s8p on my 48" deck.  Probably 3s4p combined to get 12s8p
```

---
## \#39 Posted by: Colson003 Posted at: 2017-12-16T23:23:58.690Z Reads: 127

```
@squishy654 is using 15 of those 10s2p packs from eBay 
10s30p :astonished:
```

---
## \#40 Posted by: barajabali Posted at: 2017-12-17T00:10:08.137Z Reads: 122

```
25Rs so it would be nearly 1.8 kwh at 3.7v 

Legitimate cells.
```

---
## \#41 Posted by: Acido Posted at: 2017-12-17T09:37:57.421Z Reads: 116

```
Woah thats huge whats the charger for that
```

---
## \#42 Posted by: PXSS Posted at: 2017-12-17T13:28:51.026Z Reads: 104

```
8S13P. 1310Wh. @3.6v
I'm missing escs to finish this board...
```

---
## \#43 Posted by: barajabali Posted at: 2017-12-17T15:22:54.462Z Reads: 100

```
I could use an ebike charger and pump 10 amps into it but I’m gonna go with my 4amp since I have it already
```

---
## \#44 Posted by: FredrikHems Posted at: 2017-12-17T15:25:04.437Z Reads: 99

```
Thats like 10 hour charge time, haha :joy:
```

---
## \#45 Posted by: barajabali Posted at: 2017-12-17T15:30:20.777Z Reads: 101

```
Yea but it’s also got like 80 mile range with my mono sooo I don’t mind
```

---
## \#46 Posted by: FredrikHems Posted at: 2017-12-17T15:35:33.811Z Reads: 102

```
Mono Street or terrian?
```

---
## \#47 Posted by: barajabali Posted at: 2017-12-17T16:55:35.255Z Reads: 100

```
This pack is gonna be used for my mono street and my 4wd off-road trampa
```

---
## \#48 Posted by: BigBoyToys Posted at: 2017-12-17T23:08:46.375Z Reads: 90

```
My battery is 12S 4P lipo 36AH 1600 whr.

@squishy654 is building a 2400 whr battery.

Yours will be the biggest!
```

---
