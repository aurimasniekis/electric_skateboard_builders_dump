# Adding a power switch and finding a better charging method to my board

### Replies: 18 Views: 1985

## \#1 Posted by: fredrikinn Posted at: 2018-04-25T14:34:35.476Z Reads: 162

```
Hi im trying to add an power switch to my e-board. Is this ok? 
https://www.ebay.com/itm/Anti-Spark-Power-On-Off-Switch-for-VESC-or-ESC-electric-skateboard-longboard-LED/162991392682?hash=item25f30b47aa:m:mPZxk2QL2i4EVYIUAZWBOyg

or should i look a bit more? wasnt planning on using that much money.

And if i add it, how can i improv the charging setup? 

this is the set up i plan 
![setuo|690x388](upload://kmNTzGtsaHxHFCR0tNJRZMRZXkn.png)

i disconnect the battery and connect it to my battery balance charger every time. is it possible to charge it without disconnecting it every time? (Still want to use the balance charger, but also open for other solutions)

Thanks for any help 

Sorry for my bad english
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-04-25T16:09:41.964Z Reads: 131

```
It seems legit. Just know that it is over 5 weeks for shipping. I would get 2 Incase 1 is DOA
```

---
## \#3 Posted by: Orin635 Posted at: 2018-04-25T16:21:32.195Z Reads: 126

```
watch this video
https://www.youtube.com/watch?v=O5gi35AtPSw
```

---
## \#4 Posted by: fredrikinn Posted at: 2018-04-25T17:10:30.532Z Reads: 119

```
But how would i do it inside the board?
```

---
## \#5 Posted by: Orin635 Posted at: 2018-04-25T17:11:20.740Z Reads: 120

```
what im doing is leaving the balance leads outside the board then you make his special cable then all you need to use to charge are the balance leads
```

---
## \#6 Posted by: fredrikinn Posted at: 2018-04-25T17:13:48.104Z Reads: 113

```
Chargeing with only the balance leads? is that possilbe? 

if so, is it any slower?
```

---
## \#7 Posted by: Orin635 Posted at: 2018-04-25T17:15:46.680Z Reads: 109

```
@lowGuido can answer those questions better than me he's the one who's made it. (I havent done it yet waiting on parts)

but I don't think its slower and it's definitely possible
```

---
## \#8 Posted by: Trdolan03 Posted at: 2018-04-25T17:27:07.551Z Reads: 107

```
You are limited by the 22awg wire that balance leads have.
```

---
## \#9 Posted by: b264 Posted at: 2018-04-25T17:29:10.057Z Reads: 108

```
[quote="fredrikinn, post:1, topic:53466"]
i disconnect the battery and connect it to my battery balance charger every time. is it possible to charge it without disconnecting it every time?
[/quote]

Put a BMS on the battery.

[quote="fredrikinn, post:1, topic:53466"]
Still want to use the balance charger
[/quote]

You can still use it, just without the balance leads.  With a 2 wire plug, like a normal charger
```

---
## \#10 Posted by: Orin635 Posted at: 2018-04-25T18:24:00.231Z Reads: 99

```
for me, my charger only charges at 2.3a for 6s and only allows discharge at 1a so its fine for me
```

---
## \#11 Posted by: SirDiff Posted at: 2018-04-25T18:41:36.372Z Reads: 95

```
Why don't you just get a BMS with an integrated eswitch?
```

---
## \#12 Posted by: fredrikinn Posted at: 2018-04-25T18:45:09.309Z Reads: 96

```
sounds like that may be the best idea. have any good links to where i can buy?

i have 2x
https://hobbyking.com/en_us/zippy-compact-5000mah-3s-25c-lipo-pack.html
```

---
## \#13 Posted by: lowGuido Posted at: 2018-04-26T01:43:44.392Z Reads: 82

```
[quote="fredrikinn, post:6, topic:53466, full:true"]
Chargeing with only the balance leads? is that possilbe?

if so, is it any slower?
[/quote]

22AWG balance leads should be good for 7A charge current. given that most B6 chargers max out at 2.4A this shouldnt be a problem.
```

---
## \#14 Posted by: fredrikinn Posted at: 2018-04-26T07:50:11.212Z Reads: 70

```
Well that didnt work at all. @Orin635 @lowGuido.

Followed the video and after trying to charge my batteries for 5 sec smoke came from my imax b6.
```

---
## \#15 Posted by: lowGuido Posted at: 2018-04-26T08:12:24.010Z Reads: 68

```
you did something wrong then. most likely got the balance leads the wrong way round.
would have burnt out the resistors if you did.

fortunately that's not too hard to fix.
https://static.rcgroups.net/forums/attachments/6/4/9/2/6/3/a8738175-193-1469e1%20IMAX%20SkyRC%20Schematic.jpg
120 ohm surface mount resistors X 6  replace them and you should be good to go again.

it'll be BAL2 or BAL3
```

---
## \#16 Posted by: fredrikinn Posted at: 2018-04-26T19:19:22.799Z Reads: 55

```
This is how i did it.
![setup|690x388](upload://8HZ8V0ycWJCuCbX0Kq2LURZAGrO.png)

Can you see where i faild?
```

---
## \#17 Posted by: lowGuido Posted at: 2018-04-27T10:10:46.318Z Reads: 46

```
yeah, I reckon you put the 2 plugs in the middle the wrong way around. 

your drawing looks correct. I reckon you got them wrong IRL though.
```

---
## \#18 Posted by: fredrikinn Posted at: 2018-04-27T11:52:28.332Z Reads: 39

```
I have it like the picture. Maybe somthing wrong at the other side of the battery? at the XT 90 connector
```

---
