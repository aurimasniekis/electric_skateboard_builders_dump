# Modding my focbox

### Replies: 24 Views: 1346

## \#1 Posted by: Sirshaunsta Posted at: 2018-01-27T20:05:04.930Z Reads: 225

```
I have used 10awg and xt90s for my whole battery and motor setup to allow the best current for high amps to get the most of this board, but I have a bottleneck in my power, the vesc x(focbox) uses 12 awg wire and xt60s. So I'm going to re solder on 10awg wire with an xt90adaptor for less resistance and higher capacity, and lower heat.
```

---
## \#2 Posted by: Sirshaunsta Posted at: 2018-01-27T20:09:11.775Z Reads: 225

```
Does anyone know where I can get new connectors to attach the focbox to my motors? The motor has a thicker wire and plug
```

---
## \#3 Posted by: Lukas Posted at: 2018-01-27T20:29:53.053Z Reads: 215

```
Try to search "bullet connectors" on hobbyking, amazon, ebay
You can get them in different diamenters
```

---
## \#4 Posted by: ShutterShock Posted at: 2018-01-27T20:37:17.350Z Reads: 207

```
I usually buy bullet connectors from Amazon, 5.5mm.  Usually, motors come soldered with 5.5mm unless they're hubs.
```

---
## \#5 Posted by: Surfer Posted at: 2018-01-27T20:40:01.387Z Reads: 201

```
Actually is not need it to do that, the cables from the focbox are enough for the amps you going to use, also xt60 is enough no need it xt90, bigger not means more efficiency
```

---
## \#6 Posted by: Blitz Posted at: 2018-01-27T20:53:14.754Z Reads: 193

```
Just put xt90 on the Vesc-x if needed but there is no need to mod the wire because!
The 12awg cable is not the bottle-neck rather the Internal electronics that handle all the current,
The guys at enertion would not Cheap out on 12awg instead of 10awg,
everything for a reason.
```

---
## \#7 Posted by: Sirshaunsta Posted at: 2018-01-27T21:02:36.876Z Reads: 184

```
I agree they are anal about quality but also weight reduction which the lighter wire and plug also reduce a fair bit @Blitz I wonder if maybe it was seen as a just sacrifice or a tolerable tradoff
```

---
## \#8 Posted by: ShutterShock Posted at: 2018-01-27T21:05:37.857Z Reads: 178

```
It was probably a tradeoff for performance that the raptor will not use, also the 12AWG is probably cheaper
```

---
## \#9 Posted by: Blitz Posted at: 2018-01-27T21:54:00.322Z Reads: 162

```
what I can say is that, If your not very good at opening things and soldering big wires on smaller ports
It's just not worth the risk, also if your Vesc fails well you kinda tampered so Be aware! 
If you still decide to do so then Please test performance before the mod and after
If you find anything interesting share with us.
```

---
## \#10 Posted by: Sirshaunsta Posted at: 2018-01-27T22:09:51.156Z Reads: 154

```
Will do, I'll only adjust 1 to make sure I don't waste more than 1 vesc @Blitz
```

---
## \#11 Posted by: Blitz Posted at: 2018-01-27T22:12:09.878Z Reads: 148

```
Good Luck measure twice cut once :)
```

---
## \#12 Posted by: Sirshaunsta Posted at: 2018-02-12T10:16:18.407Z Reads: 105

```
So I've decided against modding the focbox wires, I'm going to re order my battery adaptors in xt60 links. It will save weight size and a headache
```

---
## \#13 Posted by: Blitz Posted at: 2018-02-12T10:18:00.950Z Reads: 103

```
Wait what? You can put on a xt90 IT makes no difference!

there is an amp draw limit better connector wont change that.
```

---
## \#14 Posted by: Sirshaunsta Posted at: 2018-02-12T10:19:51.140Z Reads: 102

```
How do I put an xt90 on a xt60 unless I get more adaptors and re solder them together?
```

---
## \#15 Posted by: Blitz Posted at: 2018-02-12T10:20:10.100Z Reads: 104

```
IF you have xt90s use them.

You cut the wire and solder it to a new connector.

https://www.youtube.com/watch?v=mH32jwFc8Js
```

---
## \#16 Posted by: Blitz Posted at: 2018-02-12T10:35:33.637Z Reads: 101

```
OK lets be productive!

from what iv'e read your battery setup uses xt-90 does that include a series wire harness? 
https://hobbyking.com/media/catalog/product/cache/1/image/565x414/9df78eab33525d08d6e5fb8d27136e95/2/5/25661_1.jpg

Now Why get xt60 instead of xt90 does the size really matter to you? 
you should not use adapters they could just be another point of error or just take up more space. So now your thinking should i go for xt60 or xt90 connectors on all my stuff?

xt90 Pros: you batteries already have it, Soldering 10awg is a lot easier with xt90.
It's a bit more reliable, cons: it costs a bit more and its bigger.
And when you said adapters did you mean connectors because all the confusion is  from that.
```

---
## \#17 Posted by: Sirshaunsta Posted at: 2018-02-12T10:58:39.749Z Reads: 90

```
My batteries are 5s, they were made with xt60s. Your video showed me I can put the 90s on my battery and then continue using my xt90 harness (yes series and parallel) and I could easily do the same to the focbox. No the size doesn't bother me at all but I wonder if I'm actually going to see any benefit to using the heavier gauge wire and connectors when my battery and speed controllers are limited to 12 awg wire, while my harness wires are all 10 awg @Blitz
```

---
## \#18 Posted by: Blitz Posted at: 2018-02-12T11:08:37.855Z Reads: 84

```
If you use XT90 you can take advantage of "120A Peak Current Limit " "60A Continuous Current"
(as specified on enertions website) Do you really want to be near the edge from the connectors side?

The wires can heat up but the peak is only like 2-4 sec? (for acceleration and uphill I guess) 
good wires should be pure silicon so The heat won't melt nothin.

I recommend go with xt90 and don't worry about no 12awg wire
Just play in the safe limits set by professionals.
```

---
## \#19 Posted by: Sirshaunsta Posted at: 2018-02-12T11:38:58.833Z Reads: 76

```
I like your thinking, I'm gonna order male to female xt90  and re solder them to my batteries and speed controllers as suggested and leave the existing 12awg wires. @Blitz
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2018-02-12T13:52:44.865Z Reads: 66

```
[quote="Blitz, post:18, topic:44816"]
If you use XT90 you can take advantage of "120A Peak Current Limit " “60A Continuous Current”

(as specified on enertions website)
[/quote]

Those specs are with the XT60, which is built for 60A continuous. And 120A peak is the rating For the Focbox max peak Amp.

So there no bottle neck with those connector.
```

---
## \#21 Posted by: Blitz Posted at: 2018-02-12T13:53:22.988Z Reads: 62

```
Does this void my recommendation of useing xt90?
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2018-02-12T13:54:03.261Z Reads: 61

```
Yes it does... there is no need for a XT90 connector.
```

---
## \#23 Posted by: Blitz Posted at: 2018-02-12T13:54:51.632Z Reads: 59

```
OK but he has a xt90 harness i tough that xt90 would be a drop more solid true?
and for upgrade to vesc6 Good investment no

Thanks for calling me out @JohnnyMeduse !
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2018-02-12T13:58:04.632Z Reads: 59

```
I'm not calling you out :wink: 

I just think their some part of this thread that is a bit misleading.
```

---
