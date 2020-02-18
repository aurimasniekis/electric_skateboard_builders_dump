# Fliess - to BMS, or not to BMS?

### Replies: 23 Views: 577

## \#1 Posted by: fliess Posted at: 2019-02-17T18:17:31.941Z Reads: 173

```
hey guys.
Want to share my **battery** experience with you to:
- help (read confuse) others, who cannot decide on BMS usage
- collect opinions about what actually happened to my battery over last 2 years

Trying to be short. This is how it was in chronological order:
1. ~ end of 2016 I bought **40x Samsung 25r** from reliable [source](http://nkon.nl) for my [Fliess1](https://www.electric-skateboard.builders/t/fliess-65kmh/22413). Each was perfectly 3.53V. Of course :wink: I opted for BMS-free solution and made 10s4p out of them
2. happy riding maybe 500-700km. 70A battery limit
3. ~  mid of 2017 I bought another **10x Samsung 25r** from the same source. To mix 'em with existing 10s4p battery and make 10s5p for my [Fliess3](https://www.electric-skateboard.builders/t/fliess-3-einmal-directdrive-immer-directdrive/32279), [Fliess3FL](https://www.electric-skateboard.builders/t/fliess-3-facelift/33271), [Fliess3Bulletproof](https://www.electric-skateboard.builders/t/fliess-bulletproof-directdrive/47379). Of course :wink: I made sure to distribute them equally and even the voltage up in parallels as well as in series
4. happy riding another 1000km+. 80A battery limit
5. ~ end of 2018 while riding I felt a sudden loss of power, and after another several km got "disconnected". Since it was already Nov I decided to put Fliess3 on a shelve and investigate the battery later. Although I knew it could be fatal for the battery, but I convinced myself that it was just a broken/bad connection
6. Feb 2019 I fetched the battery and got surprised to see 1 bank (#2 on the picture) totally dead (infinite resistance) and #10 almost dead (see pic). However the voltage distribution right after opening was almost perfect :thinking:

https://4.bp.blogspot.com/-geu-NHGMKB8/XGmBMOB-mVI/AAAAAAAAMAQ/OFPBuTgO8DItP2KJDdV_AAVdS6fWx8aVwCLcBGAs/s1600/IMG_20190120_121936.jpg

https://2.bp.blogspot.com/-_1jpZNbi_P8/XGmBMpMEAJI/AAAAAAAAMAY/am8yZd_y6fk-2a7qTErmhyJ5a9fz5lVVgCLcBGAs/s1600/IMG_20190127_132926.jpg

https://3.bp.blogspot.com/--oBDt28pgr8/XGmBMad9JKI/AAAAAAAAMAU/a8DxGRWrp5MpaWvUU_HmKyLDNBV50uLtACLcBGAs/s1600/IMG_20190217_125036.jpg

https://2.bp.blogspot.com/-fn5GxObWpMU/XGmBNoQi2eI/AAAAAAAAMAc/2l8uR-VOwlIOcmAtDMd4SGguCUrONHaHQCLcBGAs/s1600/IMG_20190217_155058.jpg

I find it strange that despite on gradual and very predictable degradation over ~2 years, I suddenly got a battery in such poor condition. Yet before the last ride, I managed to achieve expected 22-25km of ride.

Any ideas guys what has actually happened and in which order?
```

---
## \#2 Posted by: Bor.inc Posted at: 2019-02-17T20:17:14.308Z Reads: 147

```
FLIESS HAS A NEW THREAD?? 
Sorry back on topic :slightly_smiling_face:
```

---
## \#3 Posted by: fliess Posted at: 2019-02-17T20:25:25.993Z Reads: 142

```
@Bor.inc this time it's very prosaic :smile: Still...I really wish to understand what exactly happened to the battery to avoid such things happening again in the future. Would BMS prevent this shit?! I doubt.. But would definitely be safer.
```

---
## \#4 Posted by: Jumpman Posted at: 2019-02-17T20:29:38.276Z Reads: 139

```
Perhaps you reached the end of life cycle of some of your original cells?  I think you are supposed to get 300 to 500 cycles, or about 2 years depending on how you use them.
```

---
## \#5 Posted by: Bor.inc Posted at: 2019-02-17T20:30:38.564Z Reads: 131

```
Well the BMS balances the cells ofcourse and maybe (I have like no clue on this topic btw) the 10 new cells you bought have a different internal resistance compared to the other pack which could result in something like this?

Edit: if this was the case, a bms could have helped stopping certain cells overdischarging or something
```

---
## \#6 Posted by: pat.speed Posted at: 2019-02-17T21:19:20.596Z Reads: 116

```
I would think the cells happened to come out of balance on this last ride. Some of the cells got over discharged (that’s what the power dropped) and then the vesc cut off as they reached very low levels (1v or so). 

That same think happened to me a few weeks ago with a Lipo pack. It is now not usable for esk8 so I’m building a 12s3p 30q pack. This will hopefully stay in balance better and I’ll also be adding a plug for individual cell monitoring instead of just the whole pack
```

---
## \#7 Posted by: fliess Posted at: 2019-02-17T22:58:50.094Z Reads: 106

```
[quote="Jumpman, post:4, topic:84467"]
Perhaps you reached the end of life cycle of some of your original cells?
[/quote]
should not be the case. Let's quickly and very roughly estimate - given I was always able to do at least 20km per charge and that I've done let's say 3000km altogether, we get only 150 charges/discharges. For branded cells it must definitely not be a limit.

[quote="Bor.inc, post:5, topic:84467"]
different internal resistance compared to the other pack which could result in something like this?
[/quote]
I can imagine this to harm only if I made the whole bank from the new cells while keeping the other banks from the old cells. But I didn't. I have added 1 extra cell to each of already existing banks.

[quote="pat.speed, post:6, topic:84467"]
I would think the cells happened to come out of balance on this last ride. Some of the cells got over discharged (that’s what the power dropped) and then the vesc cut off as they reached very low levels (1v or so).
[/quote]
even if 1 cell in #2 bank got damaged on the last ride, which caused the whole bank to get unbalanced, it should not have caused its total death. Until 25r behaves very different than 30q when got fully discharged. Once I tested 30q very-very hard, i.e. short circuit (total 0) over multiple days, overcharge, freezing/heating, and I could not get it broken. Without even losing a capacity. Even A123 shown worse than 30q in my hard test. Eventually I managed to kill both by overcharging to 4.7-4.8V :crazy_face: (do not remember exactly).
```

---
## \#8 Posted by: Jumpman Posted at: 2019-02-17T23:42:48.324Z Reads: 91

```
I guessed that the cells were probably not too old when I noticed that pack #4 seems to have “better than new” capacity!


This looks like interesting information:  [Battery study](http://web.mit.edu/bazant/www/papers/pdf/Gogoana_2013_J_Power_Sources.pdf)
```

---
## \#9 Posted by: pat.speed Posted at: 2019-02-18T05:04:38.761Z Reads: 87

```
I was meaning the whole p group was damaged. So all 5 cells. 

Is every p group damaged now or only some?

Letting it sit for a long time while discharged is also not a good idea
```

---
## \#10 Posted by: fliess Posted at: 2019-02-18T09:04:26.289Z Reads: 80

```
[quote="Jumpman, post:8, topic:84467"]
pack #4 seems to have “better than new” capacity!
[/quote]
haha, well, it depends very much on high and low end cut-offs you setup when make capacity measurement. I tested discharging 4.2 -> 2.9V.

[quote="Jumpman, post:8, topic:84467"]
This looks like interesting information: [Battery study](http://web.mit.edu/bazant/www/papers/pdf/Gogoana_2013_J_Power_Sources.pdf)
[/quote]
indeed interesting. Was surprised about "At 4.5C charge and discharge, 20% resistance mismatch reduces lifetime by 40%". Still my conditions were much softer (only 1 new cell mixed with 4 older) and far from declared lifecycle limits.

[quote="pat.speed, post:9, topic:84467"]
Is every p group damaged now or only some?
[/quote]
as seen from photos, only #2 P group was totally damaged, i.e. each cell in this group has infinite resistance and doesn't react on applied voltage (even relatively high 42V).

[quote="pat.speed, post:9, topic:84467"]
Letting it sit for a long time while discharged is also not a good idea
[/quote]
again, as I mentioned, when I pulled the battery out and measured each group, they were not discharged (3.8V).
```

---
## \#11 Posted by: pat.speed Posted at: 2019-02-18T11:18:38.483Z Reads: 66

```
I would think then that the p group came unbalanced and drained too low (below about 2.5v). That is due to not have a bms to balance when charging. Cells come unbalanced during discharge quite often, but it’s usually ok due to being balanced again when charging. Since it wasn’t balance charged the cells just got out of hand and some maybe even overcharging making the ir even worse and more likely to unbalanced in discharge
```

---
## \#12 Posted by: Jumpman Posted at: 2019-02-18T12:09:15.933Z Reads: 63

```
I agree.  I think that over time what starts as a small mismatch will escalate.  Some packs may eventually overcharge, leading to faster degradation, while others will be well under their threshold which could explain why some packs are in nearly new condition.

Perhaps packs #1,2,9 and 10 also aged faster due to heat?
```

---
## \#13 Posted by: fliess Posted at: 2019-02-18T18:11:25.188Z Reads: 57

```
@pat.speed, @Jumpman I am almost sure my next experiment will be to take 2 brand new cells, one let's say 3.5V and another 3.8V, connect them serially and run through multiple charges/discharges. After several cycles I will see the tendency. I like a theory and usually trust it, but still prefer to double check on practice :wink:

[quote="Jumpman, post:12, topic:84467"]
Perhaps packs #1,2,9 and 10 also aged faster due to heat?
[/quote]

this is what called thinking out of the box! Dude, nice notice, indeed #1, #2, #9 and #10 are those living next to controllers. I barely believe it could have had such big effect but damn...there is correlation :slightly_smiling_face:
```

---
## \#14 Posted by: Hummie Posted at: 2019-02-18T18:16:09.467Z Reads: 53

```
Thinking in the box.  Everyone’s got there cells airtight/watertight in a box with thin nickel that gets hot. we probably are killing cells all over
```

---
## \#15 Posted by: fliess Posted at: 2019-02-19T06:07:36.880Z Reads: 51

```
[quote="Hummie, post:14, topic:84467"]
with thin nickel that gets hot
[/quote]

agree, also not without sense.

Still..when I get equal cells and kill them equally, I expect that even without balancing they would show good at least first 150-200 cycles. I am however below that and honestly surprised. If I didn't make my own hard tests on 30q (in the comments above), I would just believe that Li-ions are indeed very sensitive to over-charge/discharge/heat. But I honestly had a hard time to kill it :hushed:
```

---
## \#16 Posted by: fliess Posted at: 2019-02-19T21:19:01.497Z Reads: 44

```
@Bor.inc
@Jumpman
@pat.speed
@Hummie

guys, I really appreciate your opinions and willingness to help me personally or to make community knowledge base better! Dope!

BUT, honestly I never believed in all this BULLSHIT about BMS for branded (read good) li-ion cells. And good that I didn't give up just blindly accepting another theory. For myself I decided - **NO BMS** in my future builds.

I am sure my problem is not new and if more people just open this boring BMS thread, then someone would definitely know the answer and help. Although I played a lot with individual cells, I never used unbalanced packs for a long time. That's why for me it was new. If anybody still interested what happened to battery, then I will happily explain.
```

---
## \#17 Posted by: Bor.inc Posted at: 2019-02-19T22:09:35.123Z Reads: 39

```
Im certainly interested in what caused all the problems, I before this asumed a BMS is necessairy for a pack to balance but that isnt the case apparently (learned something new! :slight_smile:)
```

---
## \#18 Posted by: Jumpman Posted at: 2019-02-19T23:43:56.004Z Reads: 42

```
No BMS should be fine, provided that the pack is made from similar cells, and in use they are kept at similar temperatures relative to each other.  

On top of that it is important not to charge fully, so you could charge to 41V instead of 42V, for 10s.  This allows small imbalances not to have such a detrimental effect, for example if a cell is overcharged it may go to 4.15V instead of 4.25V.  Likewise raise your low voltage cut off so weaker cells don’t dip too low.  

One thing to watch out for is that even batteries from the same batch can have a 15% variance in their impedance.  Unless you measure your cells, it can be down to chance how quickly your packs get unbalanced.
```

---
## \#19 Posted by: fliess Posted at: 2019-02-20T06:25:47.148Z Reads: 38

```
@Bor.inc all cells in #2 appeared to be just good and even perfectly balanced with the rest.

https://2.bp.blogspot.com/-tz30ArozimA/XGzwILqlBPI/AAAAAAAAMDo/M3V_Nrvez_oezNpQib9VpB-lB7gjk3TEQCLcBGAs/s1600/IMG_20190219_213254.jpg

https://4.bp.blogspot.com/-X8Yp1KWDG4Y/XGzwIC3k8pI/AAAAAAAAMDk/ngx0EiJgRmMiTDMI0wbm-vvkE5nH55NPwCLcBGAs/s1600/IMG_20190219_213330.jpg

https://1.bp.blogspot.com/-tqtGONSGi0Q/XGzwH85e0CI/AAAAAAAAMDg/o7zEYus9OsYJEhhI1pCJeVZ90evIQQvZgCLcBGAs/s1600/IMG_20190219_214623.jpg

https://1.bp.blogspot.com/-sNS4WAWY8L4/XGzwJXkOzwI/AAAAAAAAMDs/MVnSk1FYR4Ul0knZ_wCir4w39JhvR-KVQCLcBGAs/s1600/IMG_20190219_214729.jpg

Protective plate popped up on one of the cells and then (my assumption) on the rest of the group, because overcurrent? I will test.
The same for group #10, but not to the end. Almost sure all cells are good there as well.

In other words, the whole pack (despite being partially mixed) stayed very well balanced during ~2 years (2000km+) and no BMS.
```

---
## \#20 Posted by: Jumpman Posted at: 2019-02-20T09:19:39.271Z Reads: 27

```
Nice find!  So, you think it was just mechanical failure due to vibrations?  Are you sure that it wasn’t the CID tripping?
```

---
## \#21 Posted by: fliess Posted at: 2019-02-20T17:18:37.296Z Reads: 29

```
@Jumpman I've never heard that pressure valve can open because of vibrations, and it's hard to believe considering its construction..
What is remaining excessive pressure.
Still not clear if overcurrent triggered it or Samsung 25r are just prone to such failure, or it has something to do with ageing as well.

My "killing" tests on 30q never revealed such a weakness...
```

---
## \#22 Posted by: Hummie Posted at: 2019-02-20T18:38:21.961Z Reads: 28

```
Great mystery. 
The gov vib test for airlines I’m guessing isn’t going to well represent what happens on a board but tells of different directions tested and the details of testing.  what do these numbers of amplitude and frequency equate to or what would be on a typical board? 
 
“(1) Vibration test. The battery must be rigidly clamped to the platform of a vi- bration machine, and a simple har- monic motion having an amplitude of 0.8 mm (0.03 inches) with a 1.6 mm (0.063 inches) maximum total excursion must be applied. The frequency must be varied at the rate of 1 Hz/min be- tween the limits of 10 Hz to 55 Hz. The entire range of frequencies and return must be traversed in 95 ± 5 minutes for each mounting position (direction of vibrator) of the battery. The battery must be tested in three mutually per- pendicular positions (to include testing with fill openings and vents, if any, in an inverted position) for equal time pe- riods.”
-https://www.govinfo.gov/content/pkg/CFR-2010-title49-vol2/pdf/CFR-2010-title49-vol2-sec173-159.pdf

Im too cheap to ever know beyond the headlines but vibration could be a possible cause of failure   But to have multiple p groups fail...and these https://www.sciencedirect.com/science/article/abs/pii/S0378775315007648?via%3Dihub
“ Post mortem analyses and μCT revealed a loose mandrel for the tested 18650 cells.

•

Depending on the direction of motion, the loose mandrel caused serious damage.”

I’m confused about the pressure relief value; are you saying it once was an open circuit and now showing a voltage again?  I thought when they popped I’d see open circuit permanently and no going back unless u maybe too off the device. I have no idea and don’t recommend doing that just wondering about how they work
```

---
## \#23 Posted by: fliess Posted at: 2019-02-20T19:22:41.277Z Reads: 27

```
@Hummie you always manage to find some interesting articles :smile: But actually there is a nice point about orientation, since indeed I would expect more damage if cells are in vertical position. Which is not the case for boards btw.

[quote="Hummie, post:22, topic:84467"]
are you saying it once was an open circuit and now showing a voltage again? I thought when they popped I’d see open circuit permanently and no going back
[/quote]
you understand correctly - valve is not going back until you press on it (see picture above). Pity that with nickel strips welded there is no enough room to reach the valve, so I needed to tear strips off :expressionless:
```

---
