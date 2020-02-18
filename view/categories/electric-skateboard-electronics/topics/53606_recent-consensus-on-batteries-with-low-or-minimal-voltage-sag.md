# Recent Consensus on Batteries with low or minimal voltage sag

### Replies: 15 Views: 1083

## \#1 Posted by: sydeskater Posted at: 2018-04-26T22:04:58.460Z Reads: 186

```
I searched voltage sag and there hasn't been a lot of new data on this, but is there a good consensus among the more experienced builders on which are the better batteries out for the build market today?  Maybe I was looking at the wrong place, but there doesn't seem to be any up-to-date information on this topic.  Looking to spend about $1500 USD on a good quality build.  I realize the motor demands that can cause voltage sags, but mainly looking at the battery quality side (as it is discharging, you don't get a big dip in voltage).  Thank you in advance for any who can help.
```

---
## \#2 Posted by: b264 Posted at: 2018-04-26T22:58:14.076Z Reads: 177

```
10S4P made from forty Samsung INR18650-30Q cells is your best bet
```

---
## \#3 Posted by: Namasaki Posted at: 2018-04-26T22:59:49.043Z Reads: 174

```
If your using Li-ions: Samsung 30Q cells  10s4p or above.
If your using Lipos: Get High C packs between 50C and 100C
http://www.electric-skateboard.builders/t/lets-talk-about-voltage-sag-poll/12085
```

---
## \#4 Posted by: evoheyax Posted at: 2018-04-26T23:29:07.328Z Reads: 154

```
I personally run a 12s4p 30q pack. About the best option in cells today.
```

---
## \#5 Posted by: deucesdown Posted at: 2018-04-26T23:48:51.620Z Reads: 157

```
I know you were riding lipos and you're 4wd. How does the 30 q pack compare?
```

---
## \#6 Posted by: Jebe Posted at: 2018-04-26T23:55:42.677Z Reads: 152

```
about to trial 12 pack of Headway 38120 10Ah cell LiFePO4 Cell 3.2V 10Ah
```

---
## \#7 Posted by: evoheyax Posted at: 2018-04-27T00:04:35.474Z Reads: 146

```
Weaker for sure. But not that much at full charge, the issue is that 18650s sag more and go to a lower voltage. So with current control which is what I’m riding now, I get 20a per motor at whatever voltage the pack is at. At full charge it sags from 4.2 down to 3.8 off the bat. Then quickly drops to 3.3 where I cut them off. Lipos sag from 4.2 down to 3.9 but then stay above 3.6 basically the rest of the ride. So you notice the difference most later in the ride. But I am running 12s4p, so at 12ah, there’s a lot of wh in this pack. So I’m getting much better range. More like 10 miles now (doing 27 mph in the middle of the block then braking, and so on, very wasteful riding. But quicker than a car still). Based on the range hummie gets, easily could do 25 miles or more. But for my weight, riding style, and hills, 10. Better than the 6 I used to get with the 8ah Lipo.
```

---
## \#8 Posted by: Eboosted Posted at: 2018-04-27T06:42:44.437Z Reads: 118

```
All my high power boards are 12s4p more than enough before increasing the weight unnecessarily
```

---
## \#9 Posted by: strattos Posted at: 2018-04-27T07:04:58.926Z Reads: 113

```
Isn't 3.3 a little high for the cutoff the official spec sheet for the cells has it listed as 2.5 while I personally wouldn't run them that low I feel like 3.3 is really high.
```

---
## \#10 Posted by: b264 Posted at: 2018-04-27T07:10:19.371Z Reads: 111

```
3.3V is a bit high but there are 2 complications here -- firstly, even with a 3.3V cutoff it could momentarily be dropping lower than that depending on how it's being measured and secondly, the amount of range you will get out of the last 0.5V is essentially zero because the capacity falls off a cliff.  But you could set it at 3.0V.  I wouldn't go any lower than that.  You'll probably get an extra 10 meters of range.  LoLz
```

---
## \#11 Posted by: Surfer Posted at: 2018-04-27T07:17:35.099Z Reads: 107

```
How about the vtc6 from Sony? It pulls more amps but actually don't know about voltage sag, someone can throw some light from real testing on skate?
```

---
## \#12 Posted by: TarzanHBK Posted at: 2018-04-27T08:20:57.891Z Reads: 95

```
30Q is cheaper and better after a few cycles than the VTC6.

http://www.electric-skateboard.builders/t/li-ion-18650-battery-comparison/11015/22?u=tarzanhbk
```

---
## \#13 Posted by: sydeskater Posted at: 2018-04-27T15:14:55.754Z Reads: 78

```
Thanks guys for the initial feedback.  In general, Li-Ion has more sag than Lipo.  It is also lighter, and I know Lipo's are less stable and much less cycle life.  Has Lipo's improved or is the tradeoff still favoring the use of Li-Ions despite more sag?  Thanks again in advance.
```

---
## \#14 Posted by: sydeskater Posted at: 2018-04-27T15:15:37.050Z Reads: 78

```
I mean Lipo's are lighter, not Li-Ion.
```

---
## \#15 Posted by: evoheyax Posted at: 2018-04-27T15:20:27.182Z Reads: 78

```
You will sag at least .4v at any part of the spectrum while pulling 20a per cell. At 3.3, it's down to 2.6. So this is why. I am not running a bms either and that's an easy way to unbalance your cells. It's not that big of a deal because of my battery voltage display, I can always see what's happening, but it's still a pain to open up, and bring cells up one by one.
```

---
