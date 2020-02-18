# Single motor on 6s with VESC, no go?

### Replies: 15 Views: 1195

## \#1 Posted by: B4Me Posted at: 2016-11-07T17:31:49.664Z Reads: 178

```
Hi 
Just a quick question, as I havnt found a solid YES or NO..
I weigh around 100kg, and I have a single 2kw motor on my board..

If I run my VESC using my excisting 6s setup, will everything work okay ?
Or should I wait for my extra battery for 9s setup ?
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-07T19:20:26.761Z Reads: 160

```
I'm using 6s, works perfect
```

---
## \#3 Posted by: SORRENTINO Posted at: 2016-11-07T19:25:49.999Z Reads: 160

```
I wouldn't recommend it!
```

---
## \#4 Posted by: B4Me Posted at: 2016-11-07T19:27:09.767Z Reads: 160

```
Your weight ?
```

---
## \#5 Posted by: B4Me Posted at: 2016-11-07T19:27:26.606Z Reads: 158

```
So you say 6s is to low ?
```

---
## \#6 Posted by: SORRENTINO Posted at: 2016-11-07T19:29:35.388Z Reads: 157

```
I think you run the risk of pulling to many amps with 6s vs 9s. Its up to you, you might be fine but I personally would wait for my other battery to come in. Just my opinion.
```

---
## \#7 Posted by: DougM Posted at: 2016-11-07T19:31:22.889Z Reads: 156

```
It depends on if you want to climb hills.  My 6s boards are fine (I'm 200 pounds) on the flat, but pretty useless on hills.
```

---
## \#8 Posted by: B4Me Posted at: 2016-11-07T19:31:52.810Z Reads: 156

```
I was thinking the same.. just wanted to hear other peoples thoughts
```

---
## \#9 Posted by: B4Me Posted at: 2016-11-07T19:32:20.847Z Reads: 152

```
Does it fry the chips, or just power down the speed ?
```

---
## \#10 Posted by: Hummie Posted at: 2016-11-07T19:43:00.218Z Reads: 146

```
Too many amps through vesc is necessary to achieve the same power as if the voltage were zincreased and you'll likely hit a temp shutdown.  
So must run Not as much power. Lowered speed.  But if ur esc can do more amps and u run more amps the motor can perform as wel...with as much power
```

---
## \#11 Posted by: DougM Posted at: 2016-11-07T19:49:11.103Z Reads: 143

```
You should limit the current in the configuration utility.  @Hummie's nailed it.
```

---
## \#12 Posted by: B4Me Posted at: 2016-11-07T19:53:35.952Z Reads: 143

```
what settings :) ?
```

---
## \#13 Posted by: Hummie Posted at: 2016-11-07T19:59:41.511Z Reads: 138

```
Ur "battery amp" limit is what determines the heat in the vesc
Still don't know what the max amp limit setting really does. 
In theory the vesc will shut down if it gets too hot as set in max temp setting so u could experiment with maybe running higher amps an see how it does.  Maybe decrease the temp cutoff if u feel safer.  I like 70amps battery and also have motor amps set to 70 and have never had a temp shutdown on 12s. but it's seeming u can up the Motor amps to its 200 max.  That'll get u faster accelerations and With the pmw(way the esc works) it would be 200 for fractions of a second, at slower speeds, and still average the 70 battery max setting if that's what it's set to.  How bout do 90 and 200 and tell us how it goes on 6s!?  Add a big heatsink
```

---
## \#14 Posted by: B4Me Posted at: 2016-11-07T23:07:42.702Z Reads: 121

```
[quote="Hummie, post:13, topic:12658"]
How bout do 90 and 200 and tell us how it goes on 6s!?  Add a big heatsink
[/quote]
I will try it when I have the VESC's ready then :)
But you cant really do much with a heatsink on a VESC 4.12.. the FETs used are dissipating heat into the PCB, and its trapped there due to the bad thermal design of the VESC :stuck_out_tongue:
 I thought about changing the layout before ordering my pcb's, so the FETs were on the same side, and then add heat-sink, but time wasn't there to it :(
```

---
## \#15 Posted by: TarzanHBK Posted at: 2016-11-08T11:08:19.077Z Reads: 93

```
on 6s, a normal 120 or 150A esc will deliver much more power than the vesc is capable of.

Also lot´s of people on single drive having problem going uphill with 6s + vesc (depending on weight)
```

---
