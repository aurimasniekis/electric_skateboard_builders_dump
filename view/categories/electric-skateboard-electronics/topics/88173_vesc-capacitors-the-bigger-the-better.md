# Vesc Capacitors: The Bigger the Better?

### Replies: 15 Views: 452

## \#1 Posted by: ATMorris Posted at: 2019-03-24T22:32:23.298Z Reads: 139

```
Hello Everyone,

So we all know that the purpose of capacitors in a VESC circuit is to smooth out rapid transitions in current flow, either during acceleration or braking. That said, the known constraints of having undersized capacitors range from motor jitters during acceleration, to limited regenerative properties in braking. Appropriately sized caps appear to mitigate these issues, but would a larger-than-stock capacitor bank yield any benefits in high current draw situations? I've got a 10,000 microfarad 100v capacitor lying around from a previous project, and I am curious to see if swapping that into my VESC circuit would give my board more boost. Perhaps tighter braking and nippier acceleration? I'd like to get your folk's opinion before whipping out the soldering iron. Cheers guys!

![0324191529_HDR|690x388](upload://z8rWmE4yjg8Ta3Ur5mBF8DgSXZQ.jpeg)
```

---
## \#2 Posted by: danielz Posted at: 2019-03-24T23:12:12.697Z Reads: 134

```
From my understanding 10,000uf is still way too small to make any difference in acceleration.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-03-24T23:28:55.695Z Reads: 128

```
Standard 4.12 use around 1800-2200uf caps
```

---
## \#4 Posted by: danielz Posted at: 2019-03-24T23:53:03.903Z Reads: 127

```
They are decoupling caps.
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-03-25T02:33:44.809Z Reads: 113

```
VESC hardware already uses capacitors that are 2x bigger than they have to be.

If you want to add extra weight, go for it :).

The size of the capacitor determines how much energy it can store, i.e. how long of a current pulse it can sustain at x voltage drop and y current draw. 

ESR determines the flat voltage drop that results from a current pulse, and is generally what causes "jitter" on the power rail from current ripple.

Assuming 20khz switching, and a max current pulse of 100A the existing capacitance on 4.12 hardware results in a voltage drop of less than 1V on the power rail.
I'm guessing the ESR of those capacitors is somewhere in range of ~30mohm, that means the capacitors are supplying a ripple current of +-50A in worst case (50% duty cycle), the result is a 3V swing in the worst case every PWM cycle. Most battery setups of 10S and 12S, this is 10% or less of the battery's voltage. 

I've personally never ran into problems during acceleration and braking (+-80A motor current, +- 40A battery current) and I would think increasing the capacitance would only provide very marginal improvement when max battery current is significantly lower than motor current (since lower voltage drop means a lower duty cycle needed).
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-03-25T02:51:19.713Z Reads: 105

```
@b264 hehe
```

---
## \#7 Posted by: b264 Posted at: 2019-03-25T08:01:28.148Z Reads: 85

```
Yes, what @Gamer43 said and also it would help you more adding a few smaller caps in parallel -- then adding this monster in there.  Like a 10pF and a 10nF and a 10μF in parallel with the 680μF/2.2mF caps.  But really the caps it has are very adequate.  Adding more capacitance will absolutely kill your antispark switch if you don't use a loopkey.

If you really want to help your ESC do all it can do, forget about the capacitors and then add heatsink to the output FETs and use large gauge wire on the battery inputs and motor phase outputs.
```

---
## \#8 Posted by: Gamer43 Posted at: 2019-03-25T08:18:31.737Z Reads: 81

```
[quote="b264, post:7, topic:88173"]
Adding more capacitance will absolutely kill your antispark switch if you don’t use a loopkey.
[/quote]

That's right, completely forgot about that xD. 
Some anti-sparks come with pre-charge functionality, but those are usually the more expensive ones. 
Thanks for pointing that out.
(I'm hoping to design a $20 anti-spark in May, though. It'll have pre-charge, push to start, and auto turn-off, hopefully).


[quote="b264, post:7, topic:88173"]
If you really want to help your ESC do all it can do, forget about the capacitors and then add heatsink to the output FETs and use large gauge wire on the battery inputs and motor phase outputs.
[/quote]

Tinning the traces will help as well, I did that with a TB ESC and it got slightly less warm xD.
```

---
## \#9 Posted by: b264 Posted at: 2019-03-25T08:25:59.097Z Reads: 73

```
[quote="Gamer43, post:8, topic:88173"]
Tinning the traces will help as well
[/quote]

Ah yes, I forgot about that one ;-)
```

---
## \#10 Posted by: b264 Posted at: 2019-03-25T08:27:26.011Z Reads: 72

```
[quote="Gamer43, post:8, topic:88173"]
(I’m hoping to design a $20 anti-spark in May, though. It’ll have pre-charge, push to start, and auto turn-off, hopefully)
[/quote]

Please PM me when the time comes :smiley:
```

---
## \#11 Posted by: Andy87 Posted at: 2019-03-25T08:50:37.162Z Reads: 65

```
@Gamer43 pm me as well when you had the time to get that done :grin:
```

---
## \#12 Posted by: ervinelin Posted at: 2019-03-25T09:25:13.871Z Reads: 60

```
Can I understand why adding more capacitance will kill an AS? Just out of curiosity...
```

---
## \#13 Posted by: b264 Posted at: 2019-03-25T09:29:27.126Z Reads: 60

```
It makes [this problem](https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967/4?u=b264) worse.
```

---
## \#14 Posted by: ATMorris Posted at: 2019-03-25T18:17:16.563Z Reads: 38

```
A fully discharged capacitor starts with virtually zero resistance, and will accept a sizable spike in current (this is the spark you see when connecting your Vesc). As the capacitor charges, it's resistance goes up, causing current draw to go down (Ohm's law). How angry that current spike gets is dependent on the output voltage of your pack and the size of the capacitors, so raising one or the other too much can push more current through your AS than it is rated for.
```

---
## \#15 Posted by: ATMorris Posted at: 2019-03-25T18:24:41.203Z Reads: 34

```
Thanks @Gamer43, I really appreciate the depth of your answer. I suppose I'll have to find other ways to increase my efficiency :slight_smile: . Keep us posted on that AS you're working on! Using a loopkey at the moment but definitely looking for a more elegant solution.
```

---
