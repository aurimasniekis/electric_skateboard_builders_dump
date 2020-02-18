# Hrb 12s lipo balance issues

### Replies: 11 Views: 197

## \#1 Posted by: pduck911 Posted at: 2019-04-09T02:24:09.149Z Reads: 57

```
I bought a Trampa Orrsom longboard with the 6.5" pneumatic tires and ordered the recommended 12S Lipo from HRB from the link on Trampa's website.  The batteries are 6 2S  10,000mah Lipos in series for 12S. 
 Anyways I have only used the board 3 times and have kept the battery at storage voltage until charging the night before a ride. The last 2 times when I got back home and hooked up the balance charger I got a low voltage error in several cells and had to manually charge the pack at 1 amp for 15 minutes or so before the error would go away and I could then balance charge as normal.  When it happened today (second time) I checked the individual cell voltages and read the following values

1 - 3.593
2 - 3.510
3 - 3.507
4 - 3.584
5 - 3.539
6 - 3.581
7 - 2.984
8 - 3.254
9 - 3.419
10 - 3.006
11 - 2.545
12 - 3.496

I got in touch with HRB  and they said to charge and discharge for 4 cycles and the cells will balance themselves out.  To me this sounds like bullshit, however I am not a lipo expert.  Any ideas would be appreciated. Thanks.
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-04-09T02:32:24.341Z Reads: 54

```
2.5v is basically a dead lipo
```

---
## \#3 Posted by: pduck911 Posted at: 2019-04-09T03:17:58.396Z Reads: 49

```
Thanks for the reply @AlanZhou   Just to clarify that cell is toast and should be replaced correct.  Would you replace the last 3 lipos in the series (cells 7 - 12)?  Is it a safety concern to run this pack through 4 charge and discharge cycles?  I would like to get the cells replaced by the manufacturer however I don't want to burn my house down jumping through hoops for $200 in lipos if the cells are toast.
```

---
## \#4 Posted by: wafflejock Posted at: 2019-04-09T03:27:05.663Z Reads: 47

```
Basically once you've gone through the charger telling you the voltage is too low (typically anything below 3.0V) then the cell is damaged and won't end up balancing with the rest of the pack and will very quickly degrade afterwards.  If you choose to attempt charging/discharging I would certainly put them in a very fire proof place where you can also keep an eye on them and/or have a fire alarm near by (during recharging is most likely time to blow with a damaged cell).

https://www.instructables.com/id/Restoring-over-discharged-LiPo-Lithium-Polymer-bat/

On a side note it seems irresponsible of the mfg to suggest doing this especially if they didn't give you proper guidance/warnings about potential danger.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-09T03:29:12.639Z Reads: 42

```
You may not need to toss it, you can try to cycle the pack a few times to try to see if it balances and always not use balance charge
```

---
## \#6 Posted by: Santino Posted at: 2019-04-09T04:26:26.259Z Reads: 37

```
I have 4 6s from them, I do not know why, but my Lipos do not like to be sleeping for short or long periods. I do abuse them all the time, but I am never squeezed them too much; even I got the same problem a few months ago...They still perform well, but not great. I charge them at 1C...I read if you start them for no more than 5 minutes in Lifepan (very slow charging voltage and Amps), you must have a chance to keep on going...I did that, its being a while since the situation, within 2 charges they got balanced. Also I use a Lipo safe bag for charging, and always around to check on them...Hope it helps...
```

---
## \#7 Posted by: wafflejock Posted at: 2019-04-09T04:38:34.168Z Reads: 34

```
Since this is a bunch of 2S packs strung in series I'd just ditch the last 2S pack replace it at least and see how it goes with the rest.  Personal experience was having multistar 6S packs that had a cell dip too low and attempted the same kind of slow charge with constant current then use regular lipo charging and basically could never get it to balance and after rides the cell was always unpredictably lower than the rest (the IR had changed from the rest of the cells so it was drifting a lot in voltage).

I decided to go down from 12S (which was honestly overkill for my needs/desires) and cut it down to 6S (dropping the extra battery with the dead cell), but that was too slow/weak so now at 10S which is a happy medium for me.
```

---
## \#8 Posted by: Andy87 Posted at: 2019-04-09T04:47:19.967Z Reads: 32

```
If that’s like new cells, check if you have a warranty on them. Usually like 30-60 days should be. As min worth a try.

The other thing I see, what is your storage voltage? According to your numbers it looks like it is something about 3.5-3.6V. If that’s your storage voltage, than how deep you discharge your packs?

Storage voltage should be around 3.8V, just in case it’s different from what you set it up for.
```

---
## \#9 Posted by: pduck911 Posted at: 2019-04-09T10:02:33.199Z Reads: 23

```
Those values were at the end of a ride when the board would not go any further, I usually discharge to 3.2 V per cell and store at 3.7-3.8 V per cell.  I am definitely going to try and get the last 3 packs replaced under warranty, but the manufacturer won't do anything until I go through the charge /Discharge 4 times.  I will let you all know how I make out.  Thanks for all the help
```

---
## \#10 Posted by: Andy87 Posted at: 2019-04-09T10:08:04.106Z Reads: 23

```
[quote="pduck911, post:9, topic:89887"]
3.2 V per cell
[/quote]

if that´s the voltage without load than that might be your issue and the reason why some of your packs are done now. From 3.4V there is not much energy in the cells left. means if you discharge your pack till 3.2V per cell, some of the cells could easy sag down to 2.8-3 V which could cause what you now see.
3.5-3.4V for battery cut off should be the minimum to hold your packs healthy.
```

---
## \#11 Posted by: pduck911 Posted at: 2019-04-09T16:07:19.492Z Reads: 14

```
Thanks for all the advice everyone it is appreciated
```

---
