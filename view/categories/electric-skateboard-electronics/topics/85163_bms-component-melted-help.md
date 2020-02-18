# BMS - Component Melted Help

### Replies: 32 Views: 266

## \#1 Posted by: AlanZhou Posted at: 2019-02-23T20:20:14.350Z Reads: 60

```
Hey so i was swapping out my "cheap Chinese bms" that caused my cells to go -/+ 0.20v out of balance, and this happened, one of the components looked like a melted Hershey wasn't that bad, this happened when I was doing a test when I connected my negative lead to b- , was it user error? :sweat_smile: i have another one on hand

bms in question bestech d124
![IMG_20190223_151445|375x500](upload://rIliZAhR4EgRh0NRFQbjOeoENjl.jpeg) ![InkedIMG_20190223_151430_LI|375x500](upload://mZJEa2jsamOmJJ7xWnXfXNAPh2d.jpeg)

Any idea what might of caused it?
```

---
## \#2 Posted by: DerelictRobot Posted at: 2019-02-23T21:02:38.501Z Reads: 41

```
Heat and user error. :smiley:

I just fatfingered a 12S D127 and did the same damn thing last week.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-02-23T21:03:28.467Z Reads: 39

```
:rofl::rofl: rly.. but but its brand new :joy::sob:
```

---
## \#4 Posted by: EstTerminus Posted at: 2019-02-23T21:04:05.939Z Reads: 40

```
That doesn't look like burned, but some glue or etc, this is a chip which balances a cell, next to it is transistor and resistor which gets hot while balancing but that chip shouldn't get warm.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-02-23T21:04:44.897Z Reads: 38

```
smoke came out.... it was a mock so i only touch the negative to b- for a split second

mabye i put the balances wires in the wrong order?
```

---
## \#6 Posted by: DerelictRobot Posted at: 2019-02-23T21:04:59.090Z Reads: 38

```
That's a small mosfet. They burn like that if you short a balance lead to the wrong thing wiring em up hot
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-02-23T21:05:20.116Z Reads: 36

```
my issue is the bms did not have a clear indication.
```

---
## \#8 Posted by: DerelictRobot Posted at: 2019-02-23T21:05:35.061Z Reads: 36

```
[quote="AlanZhou, post:5, topic:85163"]
mabye i put the balances wires in the wrong order?
[/quote]

Have a drawing or pic of your schematic?

Yep, every BMS ever.
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-02-23T21:06:20.554Z Reads: 34

```
...
![IMG_20190223_160547|666x500](upload://yFe3Eu6566L47w2MSlCqQuOp7XF.jpeg)

both sides frekin says b10

how hard would it be to write b1 b2 b3 b4 b5 b6 b7 b8 b9 b10

heck the Chinese bms was even easyier to hook up
```

---
## \#10 Posted by: DerelictRobot Posted at: 2019-02-23T21:12:06.725Z Reads: 28

```
So on the left I see B-. Think of that as the bottom of your stack of series. You likely have a B- cable separate from the balance, no B- on the balance connector as I only count 10 pins. 

From there balance connector left to right should go
B1 = 1S, B2 = 2S, B3 = 3S.... B10 = 10S. 

Make sense?

Are you bypassing?
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-02-23T21:14:04.977Z Reads: 29

```
Yep, the only thing i hooked up was the balance leads and when i tryied to connect the b- smoke came up.

pretty sure i started off at b-
```

---
## \#12 Posted by: DerelictRobot Posted at: 2019-02-23T21:17:01.238Z Reads: 30

```
You might have one of your balance connections miswired then.

If you visualize your 10S as a stack of 10 batteries like a totem, just walk through and double check your connections starting from the 'ground':  B-

Then 1S, 2S, 3S, so on up to 10S. Check your voltage going to the p group stack

Wire your balance cable to each P group, and then wire B- to B-, triple check all your connections, plug in and hope for the best.
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-02-23T21:18:00.985Z Reads: 28

```
i did.... i wires the balance wires first than wired the b- , didnt have any issues on the chinese bms
```

---
## \#14 Posted by: DerelictRobot Posted at: 2019-02-23T21:24:30.492Z Reads: 29

```
Did you have the balance cable harness plugged into the BMS prior to soldering ground?

Dunno. To be fair I've also just had a BMS die like this for no reason at all on first current draw test. cut it out and swapped in an identical and it worked fine. 

QA can be shifty on some of these. I don't think it's just Bestech making Bestech BMS if you know what I mean
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-02-23T21:26:00.597Z Reads: 28

```
[quote="DerelictRobot, post:14, topic:85163"]
Did you have the balance cable harness plugged into the BMS prior to soldering ground?
[/quote]

yeah.... mabye
```

---
## \#16 Posted by: DerelictRobot Posted at: 2019-02-23T21:26:29.549Z Reads: 23

```
Hahaha. Round 2, fight!

Good luck.
```

---
## \#17 Posted by: AlanZhou Posted at: 2019-02-23T21:28:35.298Z Reads: 21

```
so wait waht...
```

---
## \#18 Posted by: DerelictRobot Posted at: 2019-02-23T21:32:25.212Z Reads: 24

```
[quote="AlanZhou, post:17, topic:85163, full:true"]
so wait waht…
[/quote]

Fly strong lil bird I believe in you!
```

---
## \#19 Posted by: AlanZhou Posted at: 2019-02-23T21:32:43.885Z Reads: 23

```
so that was the issue?
```

---
## \#20 Posted by: DerelictRobot Posted at: 2019-02-23T21:34:34.646Z Reads: 23

```
Honestly without being able to touch it with my Fluke I'm just doing educated best guesses here. If you wire it correctly and it's not a DOA/defective unit, it theoretically should not catch fire.

I'm just filling you with confidence aren't I?

Let me see if I can find an example schematic for you to verify a known good against.
```

---
## \#21 Posted by: DerelictRobot Posted at: 2019-02-23T21:36:26.752Z Reads: 23

```
Hold the phone. 

Are you sure this is a 10S BMS? Pic of the other spare you have? Top/bottom?
```

---
## \#22 Posted by: AlanZhou Posted at: 2019-02-23T21:37:06.835Z Reads: 23

```
![IMG_20190223_163646|666x500](upload://wEfSRjaWNG5tzuNqXGfDcJS3iZv.jpeg)
```

---
## \#23 Posted by: DerelictRobot Posted at: 2019-02-23T21:40:24.447Z Reads: 21

```
Do me a favor, take a picture of your BMS and point out to me your C- and B- connection points on the PCB that you used
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-02-23T21:41:50.774Z Reads: 21

```
![Inkedqe32_LI|375x500](upload://VmkCejmiYvVWmDE3flzh1UTaVg.jpeg)

i didnt even get a chance to hook up c- :sob:
```

---
## \#25 Posted by: DerelictRobot Posted at: 2019-02-23T21:54:31.129Z Reads: 20

```
You don't need C- for now. Make sure your battery output is all there and double check your discharge voltage too to make sure they match.

This diagram is still probably the most concise I've seen, even though it's for 12S, same deal. It does not include an extra B- connection on the balance cable, just like yours:

https://www.electric-skateboard.builders/t/12s5p-30qs-charge-rate/78259/76?u=derelictrobot

Connect B-. Then balance cable.
```

---
## \#26 Posted by: AlanZhou Posted at: 2019-02-23T21:56:45.666Z Reads: 20

```
eh would of been burned anyways..... b10 was at b1, that diagram was for d124? (not exactly)

and i thought the negative wire of the charger goes to c- not p

i hooked up the bms at 31v and it blew... hehe
```

---
## \#27 Posted by: DerelictRobot Posted at: 2019-02-23T22:13:24.018Z Reads: 20

```
The diagram I linked isn't specific to a BMS, just a general bypass diagram without the extra B- negative. 

Charge port goes C-. Some BMS have output and input on the same channel, yours doesn't. You don't need to hook to P- at all.
```

---
## \#28 Posted by: AlanZhou Posted at: 2019-02-23T22:13:47.046Z Reads: 18

```
i know how to hook up a bms....

i just dont know which side is b1 or b10
```

---
## \#29 Posted by: DerelictRobot Posted at: 2019-02-23T22:14:58.029Z Reads: 18

```
Left is B1 on your picture
```

---
## \#30 Posted by: AlanZhou Posted at: 2019-02-23T22:16:08.581Z Reads: 17

```
k thx i hope so :sob::joy::joy:
```

---
## \#31 Posted by: DerelictRobot Posted at: 2019-02-23T22:17:02.219Z Reads: 18

```
Is almost always on the same side as B-. I am 98% positive this is correct on yours. I just can't be 100% without it in hand.

Or just do the opposite of your burny way. :smiley:
```

---
## \#32 Posted by: Jaydawg56 Posted at: 2019-02-24T01:20:02.743Z Reads: 15

```
@AlanZhou here you go, should answer any doubt in your mind. I’m hooked up this way and works with no issues. Of course, charge only. 

![20190208_142130|375x500](upload://dg3AdE6Ff2y6up3TgK2qmy8IB5n.jpeg)
```

---
