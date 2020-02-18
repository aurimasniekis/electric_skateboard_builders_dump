# Reasonable Price VESC

### Replies: 15 Views: 526

## \#1 Posted by: freddyfred01 Posted at: 2019-03-27T13:24:20.451Z Reads: 181

```
Hey guys,
Just wondering if anyone has any links or suggestions for reasonably priced VESCs that I can purchase in Australia. I’ve never used a Vesc before. 
Also what C rating is suggested for the batteries if I use either 6s or 8s batteries with the VESC.
Thanks heaps
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-27T13:27:35.606Z Reads: 182

```
All depends on you, your situation and which kind of board you want to build and where you want to drive.
Sounds complicated, but it’s not 😅
Just to give a good advice we need more info about you and your plans (board related plans ☝️😂)
```

---
## \#3 Posted by: meesie Posted at: 2019-03-27T15:39:18.272Z Reads: 155

```
there's a flipsky vesc on aliexpress for 45 Euro. i've got  2 of them running 12S in FOC and it works wonders.

also, battery C rating is basically: **battery capacity * C (number) = max discharge.**
so a 5000mAh 10c battery would technically be able to draw 50 amps. however, companies are known to exaggerate the C-rating.  so stay a little bit under that number.

street board on flat roads, aim at between 20 and 50 amps.

street board on hilly roads, aim at between 30 and 60 amps

mountainboard flat roads, aim at between 30 and 60 amps

mountainboard hilly roads, aim ar vetween 40 and 80 amps

PS: idk how to space on this site, and if you're planning an MTB get focboxes or a unity. flipsky and maytech 4.12 vescs can't handle higher than 50A per vesc
```

---
## \#4 Posted by: olestra Posted at: 2019-03-27T15:59:09.307Z Reads: 128

```
I'm curious about your guidelines for amps, is this figure independent of voltage (i.e. 6s, 10s) and is it total per board or per motor?
I get that it's ballpark number, not a rigorous spec...
```

---
## \#5 Posted by: meesie Posted at: 2019-03-27T16:38:12.803Z Reads: 108

```
oh right. yeah it was more of a ballpark number indeed. it was meant for the guy to guesstimate what lipo's he should get regarding the C-rating.
```

---
## \#6 Posted by: Gamer43 Posted at: 2019-03-27T21:51:58.651Z Reads: 82

```
Flipsky is implementing a change that will solve cutout problems entirely on their 4.20 hardware versions.

Once the change is implemented (in the coming days and weeks) it can handle 12S 60A FOC without a problem.
```

---
## \#7 Posted by: freddyfred01 Posted at: 2019-03-28T05:55:25.037Z Reads: 65

```
I found a relatively cheap Turnigy battery with 4S 4000mah and 12C. Im planning to put two of those in series. Would that be enough of a discharge rating? or is it too close
```

---
## \#8 Posted by: pat.speed Posted at: 2019-03-28T06:01:44.809Z Reads: 62

```
That’s too low, you need at the very least 20c even with this the batteries will sag a lot under load. You want to aim for 40c as a minimum and 60c or higher as the goal. The problem then is by the time you’ve spent the money for those new shiny 60c batteries it would have been cheaper to just get a lithium ion battery. Trust me they are work the money, you can get a lot more Ah of battery into smaller spaces than lipos.
```

---
## \#9 Posted by: b264 Posted at: 2019-03-28T06:38:28.568Z Reads: 56

```
No, you want 40C or higher
```

---
## \#10 Posted by: b264 Posted at: 2019-03-28T06:39:21.450Z Reads: 56

```
See https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/1344?u=b264

Not a VESC, but it helps
```

---
## \#11 Posted by: meesie Posted at: 2019-03-28T06:40:58.718Z Reads: 56

```
It _should_ technically be enough. But as you only have two smaller lipo’s you’ll experiance a lot of voltage sag (voltage drops when drawing amps,) and you’ll be limited in acceleration. i’d recommend going for a 10s 2/3p liion battery.

I’ve started with lipo’s myself too and sooner or later you’re going to want an upgrade.

If you’re reeeaallly on a budget you should look at high capacity lipo’s for some decent range. Multistar 10.000mAh 10c for example, which would be 100A max.
```

---
## \#12 Posted by: Andy87 Posted at: 2019-03-28T07:02:31.684Z Reads: 43

```
[quote="meesie, post:11, topic:88468"]
If you’re reeeaallly on a budget you should look at high capacity lipo’s for some decent range. Multistar 10.000mAh 10c for example, which would be 100A max.
[/quote]

No, just please no!
Those are not high drain Lipos.
They made to charge your packs on the field.
Those are not 10C as stated, they tested to 3-4C max.
Ok you still can run them on a chinese hub build, but for everything  that gets a bit more seriouse, better get the HK Graphene 8Ah or 12Ah. They as minimum close to there stated specs regarding discharge.

[quote="meesie, post:11, topic:88468"]
I’ve started with lipo’s myself too and sooner or later you’re going to want an upgrade
[/quote]
That´s personal preference.
I upgraded my LiIon pack to a Lipo pack... :sweat_smile: just sayin...
```

---
## \#13 Posted by: meesie Posted at: 2019-03-28T07:30:40.959Z Reads: 33

```
Whuuuut? Alright then, didn’t know that multistar overstated it thát much. I’ll take back my words on that one. @freddyfred01

As for your build wit lipo’s, do you have em in a mountainboard? Because then i’d definetely understand why you switched to lipo’s :joy: what lipo’s do you have in there?
```

---
## \#14 Posted by: Andy87 Posted at: 2019-03-28T07:36:13.056Z Reads: 33

```
yeah mountainboard. to be fair, it´s also the only kind of boards i would call them an upgrade :sweat_smile:
I just get more power out of a lighter set up.
the down sides like, storage charge when not used and low range are just not practicable for usual all terrain or street boards.
```

---
## \#15 Posted by: meesie Posted at: 2019-03-28T08:05:09.837Z Reads: 31

```
Haha exactly! The power output is unparalelled though :muscle:
```

---
