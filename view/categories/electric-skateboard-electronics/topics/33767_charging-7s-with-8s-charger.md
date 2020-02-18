# Charging 7S with 8S Charger

### Replies: 23 Views: 1244

## \#1 Posted by: florensvb Posted at: 2017-09-23T09:43:47.916Z Reads: 60

```
Hey guys,

I have just recently removed a dead cell from my 8S pack, as described in [this thread.](http://www.electric-skateboard.builders/t/lipo-cell-dead/33569/9).

New problem is that I need to trick my 8S charger into charging my 7S pack. I have made my own charging port using a D-Sub15 pin plug (essentially a big VGA plug) and now I just cant figure out how to re-wire it to make it work.

This here is my charger: 

https://tomtop_shop.guphotos.com/i/w?u=/images/R/RM3758EU/RM3758EU-4-dd67.jpg

If someone could draw me a quick sketch, basically explaining how a 8S to 7S JST adapter would look like, id be forever greatful :) 

Thanks guys!
```

---
## \#2 Posted by: Cobber Posted at: 2017-09-23T09:48:37.552Z Reads: 55

```
um is the busted cell still wired in series?
if it is not, you just need to make a 7s balance plug...
```

---
## \#3 Posted by: florensvb Posted at: 2017-09-23T09:55:02.608Z Reads: 53

```
Hey @Cobber, no I cut it out and re-wired it to be a 3S pack. So I have a 7S battery that is made of a 4S and a 3S Lipo. 

 [quote="Cobber, post:2, topic:33767"]
if it is not, you just need to make a 7s balance plug...
[/quote]

Thats exactly what I dont know how to do :)
```

---
## \#4 Posted by: SilentException Posted at: 2017-09-23T10:00:38.383Z Reads: 50

```
You have 9 pin connector and 9 cables. Remove first or last cable. Use 8 pin connectors. Done. Seriously, not sure what's bugging you, it's the simplest thing :)
```

---
## \#5 Posted by: Cobber Posted at: 2017-09-23T10:01:45.323Z Reads: 47

```
putting un-balanced cells together in a single battery aside...
the cells would all need to be in series with the 7 balance wires in a single balance lead... be careful. you will need to watch charge and discharge voltage constantly. you don't want a fire
```

---
## \#6 Posted by: florensvb Posted at: 2017-09-23T10:03:49.137Z Reads: 44

```
[quote="Cobber, post:5, topic:33767"]
putting un-balanced cells together in a single battery aside...
[/quote]

The cells were all balanced to +-0.02 difference in voltage :) 

For sake of simplicity, lets just assume i had a 7S battery with a single 7S balance lead. How do I connect that to my 8S balance lead on the charger? Thats ultimately my question
```

---
## \#7 Posted by: Cobber Posted at: 2017-09-23T10:05:21.560Z Reads: 35

```
plug the 7s plug in to the 1-7 cells on your chargers balance port?
```

---
## \#8 Posted by: scepterr Posted at: 2017-09-23T10:05:36.707Z Reads: 32

```
Remove the extra wire that's not connected to any cells..
```

---
## \#9 Posted by: SilentException Posted at: 2017-09-23T10:05:54.396Z Reads: 30

```
Does your charger have setting for charging 7s pack, is it configurable in any way?
```

---
## \#10 Posted by: florensvb Posted at: 2017-09-23T10:06:38.500Z Reads: 29

```
Well on the manual it says its capable of charging 2-8S batteries and it also originally came with a balance board (its long gone), so i am assuming it can
```

---
## \#11 Posted by: SilentException Posted at: 2017-09-23T10:07:38.978Z Reads: 28

```
And do you have 9pin JST coming out of your pack?
```

---
## \#12 Posted by: Cobber Posted at: 2017-09-23T10:08:55.679Z Reads: 27

```
along the lines of what sceppy said, what does your balance lead look like? 7 cell balance wires?
```

---
## \#13 Posted by: florensvb Posted at: 2017-09-23T10:09:26.246Z Reads: 28

```
No i am hooking up the balance leads into my vga port, so that i have a plug'n'play solution without bms, so i am not actually using the jst plugs on my lipo
```

---
## \#14 Posted by: SilentException Posted at: 2017-09-23T10:10:56.716Z Reads: 28

```
Alright, but you do have pin 0 (gnd) - pin 8 (v+) and getting around 29,4V across them?
```

---
## \#15 Posted by: florensvb Posted at: 2017-09-23T10:12:49.052Z Reads: 29

```
I have 8 balance leads:

1st pack is 3S:
- and + first cell,
+ second cell,
+ third cell
= 4 balance wires

2nd pack is 4S:
+ first cell (leaving - disconnected as its redundant),
+ second cell,
+ third cell,
+ fourth cell,
= 4 balance wires

= 8 balance wires in total
```

---
## \#16 Posted by: florensvb Posted at: 2017-09-23T10:14:23.918Z Reads: 29

```
yeah i do, voltages seem ok
```

---
## \#17 Posted by: SilentException Posted at: 2017-09-23T10:16:25.706Z Reads: 25

```
Alright, yo need to make a cable that will connect (-) from the charger to the pin 0 on the VGA, following through pin 1 (4,2V), 2 (8,4V)... up to 8 (29,4V). Pin 8 will finish at marking 7 on the charger. 8 on the charger will be free.
```

---
## \#18 Posted by: florensvb Posted at: 2017-09-23T10:17:37.760Z Reads: 25

```
Thank you, i think i got it, i will try in a few hours when i am at home!! :)
```

---
## \#19 Posted by: SilentException Posted at: 2017-09-23T10:47:52.011Z Reads: 24

```
No problem. If your charger doesn't have auto detection and selection of number of cells, make sure you switch to the 7S mode.
BTW, where did you get the charger? :)
```

---
## \#20 Posted by: florensvb Posted at: 2017-09-23T10:59:31.320Z Reads: 22

```
I got it from tomtop.com but now its also available on amazon
```

---
## \#21 Posted by: TehAtheist Posted at: 2017-09-23T11:33:37.481Z Reads: 17

```
I have the exact same charger ;), also with VGA port! I love it, just the fan that makes a lot of noise is a bit annoying.
I indeed also think it's possible to use the balance board to charge your 7S battery.
```

---
## \#22 Posted by: florensvb Posted at: 2017-09-23T11:44:34.445Z Reads: 17

```
haha nice!! i dont have the balance board anymore :D
```

---
## \#23 Posted by: florensvb Posted at: 2017-09-23T12:13:30.734Z Reads: 16

```
Thank you @SilentException and @Cobber for your help!

<img src="/uploads/db1493/original/3X/9/3/93a0228650ee14548c8e3d2cf449e82903bb748b.jpg" width="375" height="500">
```

---
