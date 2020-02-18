# 10s3p or 6s5p&hellip;what&rsquo;s better?

### Replies: 25 Views: 1445

## \#1 Posted by: VerticalMedia Posted at: 2017-05-29T18:21:06.030Z Reads: 233

```
Hey guys. Trying to decide which Li-ion configuration to go with. 10s3p or 6s5p? What would the performance differences be? Which setup would help get the most out of what I plan to build? Dual non-hub motors, 80-90mm wheels, Dual Vescs, Would like 20+ mph, and as much range as possible. Limited to one of those two battery choices do to physical size.
```

---
## \#2 Posted by: SirDiff Posted at: 2017-05-29T18:26:38.717Z Reads: 229

```
10s is more efficient, go for that with 190kv motor and 15/36 gear ratio. That's a common standard, possibly get samsung 30Q. It would give you about 30km of range
```

---
## \#3 Posted by: VerticalMedia Posted at: 2017-05-29T18:36:24.361Z Reads: 224

```
Ok great. I was leaning towards the 10s. What is the difference between Samsung 25R and 30Q? I won't be building my own pack, so I am kind of limited to what I can find pre assembled. Chi Boards sells a 10s3p 37v 7.5 AH Samsung 25R with BMS. How does that sound?
```

---
## \#4 Posted by: SirDiff Posted at: 2017-05-29T19:13:15.020Z Reads: 199

```
That sounds good, but 30Qs are slightly better and have more capacity. They are rated for lower current, but people tested them and the community is leaning towards those instead of the 25rs (still good, I have a 10s3p pack myself). Up to you, with 30Qs you have more range and less sag though
```

---
## \#5 Posted by: VerticalMedia Posted at: 2017-05-29T19:26:25.212Z Reads: 178

```
Know any place I could check out/buy a 10s3p 30Q pack with BMS?
```

---
## \#6 Posted by: SirDiff Posted at: 2017-05-29T19:26:57.805Z Reads: 171

```
Where are you from?
```

---
## \#7 Posted by: VerticalMedia Posted at: 2017-05-29T19:28:24.332Z Reads: 163

```
New York City
```

---
## \#8 Posted by: lowGuido Posted at: 2017-05-29T19:36:56.364Z Reads: 158

```
if you are using <strike>VESC's</strike> DRV cookers, then you might as well go 10S. you paid the big bux for a high voltage ESC you'd wanna use it.
```

---
## \#9 Posted by: VerticalMedia Posted at: 2017-05-29T19:39:14.884Z Reads: 152

```
DRV cookers?
```

---
## \#10 Posted by: IsTalo Posted at: 2017-05-29T19:39:56.861Z Reads: 152

```
A lot of people have troubles with the DRV chip, he is just joking
```

---
## \#11 Posted by: VerticalMedia Posted at: 2017-05-29T19:41:57.510Z Reads: 148

```
@lowGuido lol very comforting. I actually haven't bought anything yet. Should I be looking at a different controller?
```

---
## \#12 Posted by: IsTalo Posted at: 2017-05-29T19:44:48.738Z Reads: 144

```
Nope, Vesc was made specifically for Esk8s, it is a Dream if you buy from the right person
```

---
## \#13 Posted by: SirDiff Posted at: 2017-05-29T19:44:55.602Z Reads: 146

```
No, it's still the best but you need to take care of it. 10s won't stress it too much, keep it cool and set the right parameters and it should be good
```

---
## \#14 Posted by: lowGuido Posted at: 2017-05-29T19:46:13.439Z Reads: 144

```
the DRV cookers are a good ESC we just arent allowed to call them VESC anymore because someone trademarked the name.
```

---
## \#15 Posted by: tueboard Posted at: 2017-05-29T19:55:45.774Z Reads: 141

```
sorry for the offtopic.. 10s3p it's ok for running in FOC with maytech VESC?
```

---
## \#16 Posted by: SirDiff Posted at: 2017-05-29T20:02:48.181Z Reads: 141

```
Foc and maytech vesc together aren't good.
```

---
## \#17 Posted by: VerticalMedia Posted at: 2017-05-29T21:44:07.434Z Reads: 124

```
Suggestions for pre made 10s3p li-ion packs with built in BMS?
```

---
## \#18 Posted by: Jinra Posted at: 2017-05-29T23:05:42.015Z Reads: 118

```
We can still call them VESC, you just can't sell them as such. I'm always gonna call it the VESC.
```

---
## \#19 Posted by: mmaner Posted at: 2017-05-30T00:43:01.299Z Reads: 111

```
Check out the enertion space cell 3, they were on sale but not sure if the still are.
```

---
## \#20 Posted by: Jinra Posted at: 2017-05-30T00:44:31.946Z Reads: 112

```
Pretty sure they're discontinued which was the reason for the fire sale. More of a warehouse clearance.
```

---
## \#21 Posted by: VerticalMedia Posted at: 2017-05-30T00:59:30.474Z Reads: 102

```
yea...discontinued now
```

---
## \#22 Posted by: mmaner Posted at: 2017-05-30T01:08:00.399Z Reads: 102

```
That sucks, it was a great buy.  Talk to @oriol360 at Miami Electric Boards, @torqueboards at DIY or @barajabali at ChiBoards.  They all make quality battery packs.
```

---
## \#23 Posted by: will_manners Posted at: 2017-05-30T11:50:25.221Z Reads: 85

```
Yeah wouldn't recommend FOC on maytech drv cooker. 

Just buy from one of the forum vendors ;) Ollin, enertion, torqueboard, diy etc.
```

---
## \#24 Posted by: lowGuido Posted at: 2017-05-30T12:16:35.344Z Reads: 83

```
[quote="Jinra, post:18, topic:24137, full:true"]
We can still call them VESC, you just can't sell them as such. I'm always gonna call it the VESC.
[/quote]

I know. Im just kidding. but I really do like the name "DRV cookers"
```

---
## \#25 Posted by: longhairedboy Posted at: 2017-05-30T14:07:44.969Z Reads: 68

```
maytech vescs stink for anything over 10S and 40 amps. Theyr'e rated at fifty, but who knows. 

We were told they could handle 12S and were tested at 14S. My guess is they tested at 14S LiFePo (roughly 12S li-ion equivilent) and only did a spin up.

we cooked the samples they sent us inside of 5 days with our "nomal" riding. 

Basically they suck. 

get an AXLE or Ollin if you're in the states.
```

---
