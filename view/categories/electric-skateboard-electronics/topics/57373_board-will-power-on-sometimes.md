# Board will Power On sometimes

### Replies: 16 Views: 331

## \#1 Posted by: achatham Posted at: 2018-05-31T17:49:57.123Z Reads: 85

```
I've run into the situation over the last few days where when I turn on the board sometimes it comes on sometimes it doesnt. Im thinking its a loose wire or something similar. How would you guys troubleshoot this? Run a voltage meter or what to eliminate what is causing the issue. 

First time troubleshooting an electric issue....can you tell.
```

---
## \#2 Posted by: JLabs Posted at: 2018-05-31T17:50:45.432Z Reads: 86

```
What’s your setup like? Got any pictures?
```

---
## \#3 Posted by: achatham Posted at: 2018-05-31T18:06:37.907Z Reads: 82

```
So I'm running 2 lipos in series with a bms (bypassing discharge) connected to the powerswitch then VESC. Its really a basic setup. The only thing I can think is I just replaced my old china bms with a new one. Could that cause a power issue? 

Bought so 14 awg to connect from the battery to the powerswitch. @Emerson mentioned 20 awg is not big enough for the discharge bypass. 

Heres a couple recent pics...
![IMG_3610|375x500](upload://6MKetmxQSDVOMRDgmrwIm6APc3g.jpg)![IMG_3611|374x499](upload://tWaHXNATtqLmd3EKTgWbIMBJwZu.jpg)
```

---
## \#4 Posted by: Martinsp Posted at: 2018-05-31T19:03:07.967Z Reads: 58

```
Since you are bypassing the BMS when discharging it should not be an issue. Try plugging the VESC directly to your battery ideally with an antispark connector but without it will do the job too just expect a spark.
If it turns on without problems try wiggling the wires at the connectors, maybe there is a loose wire somewhere. Try to do it carefully so that if the wire that may be loose, does come loose completely it wont short somewhere so try moving one wire at a time. You can disconnect the BMS for that completely so that it is not in the way, if it is hard soldered in then leave it as is since it does not really matter for discharge.
If the loose wires are not your problem and the setup is just fine without the switch, then it may be the switch that is causing the problem.
```

---
## \#5 Posted by: achatham Posted at: 2018-05-31T19:12:49.042Z Reads: 55

```
Im having a weird suspicion that its dealing with the power switch. Thanks for the 2 cents!
```

---
## \#6 Posted by: b264 Posted at: 2018-05-31T19:15:55.814Z Reads: 52

```
Where is your power switch?  I don't see it in the photos

Is it rated for 60VDC  60A
```

---
## \#7 Posted by: Martinsp Posted at: 2018-05-31T19:23:40.437Z Reads: 50

```
It is the thing in black heatshrink with eskating.eu sticker top center of the photo
```

---
## \#8 Posted by: achatham Posted at: 2018-05-31T20:21:52.728Z Reads: 44

```
Its 60A. This is it @b264

https://eskating.eu/product/anti-spark-power-switch/
```

---
## \#9 Posted by: b264 Posted at: 2018-05-31T20:27:13.280Z Reads: 38

```
If I had to guess, I would suspect,

1) the connection of the wires between the switch (thing your finger touches to turn on board) and the solid-state relay (the thing with the sticker) is not good or one has come loose

or

2) the solid-state-relay from eu has gone bad due to the inrush currents to the ESC capacitors

3) switch is bad


It could be many other things but I'd check those first

Also see if wiggling anything can cause it to fail.  See if you can get it to fail on-demand
```

---
## \#10 Posted by: mccloed Posted at: 2018-05-31T20:29:46.076Z Reads: 37

```
Not pertaining to the switch, but I have had those white BMS's, even bypassed, kill cells in my batteries. Try to keep an eye on the individual cell voltages. :neutral_face:
```

---
## \#11 Posted by: achatham Posted at: 2018-05-31T20:30:08.939Z Reads: 37

```
So yesterday after unplugging and plugging in the power switch got it to come on. I then proceeded to wiggle wires with nothing happening. No flickering or anything. I turned it off and attempted to power on without moving it and it would come on! What the heck!
```

---
## \#12 Posted by: b264 Posted at: 2018-05-31T20:34:44.919Z Reads: 33

```
It's amazing what heavy vibrations will manage to break....  essentially everything

eventually
```

---
## \#13 Posted by: achatham Posted at: 2018-06-03T01:37:55.416Z Reads: 15

```
[quote="b264, post:9, topic:57373"]
the solid-state-relay from eu has gone bad due to the inrush currents to the ESC capacitors
[/quote]

@b264 is there a way to check if this occurred?
```

---
## \#14 Posted by: b264 Posted at: 2018-06-03T01:39:53.441Z Reads: 16

```
I'd ask the seller
```

---
## \#15 Posted by: achatham Posted at: 2018-06-03T01:55:42.998Z Reads: 14

```
I did and haven’t got a response. I know it’s the power switch bc my anti spark loop works fine when I remove it.
```

---
## \#16 Posted by: achatham Posted at: 2018-06-03T02:10:34.830Z Reads: 14

```
Here’s the power switch 
![image|375x500](upload://uzEIxNglD9Y9BPyvsNbFVhnIfSZ.jpeg)

Power switch runs 100A
VESC busrt at 240A with continuous 50A

Could that have caused an issue?
```

---
