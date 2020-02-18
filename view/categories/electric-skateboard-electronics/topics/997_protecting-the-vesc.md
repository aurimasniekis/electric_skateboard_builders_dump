# Protecting the VESC

### Replies: 18 Views: 4157

## \#1 Posted by: NNGG Posted at: 2016-01-14T02:35:52.620Z Reads: 246

```
Really busy right now and wanted to know how to keep my vesc safe from any extra voltage and amps form my motor and batteries. I was browsing nospark connectors and came across these. 
 http://www.amazon.com/No-Spark-Current-Battery-Arming-Connectors/dp/B0092U6940

Any thoughts about how they can protect the VESC and what they should do?
```

---
## \#2 Posted by: lowGuido Posted at: 2016-01-14T03:04:47.102Z Reads: 245

```
read here on how to make your own.

http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
```

---
## \#3 Posted by: psychotiller Posted at: 2016-01-14T03:24:07.740Z Reads: 231

```
You could get the same effect with an xt90 antispark plug. Then just make a loop key out of it. Half the price.

@lowGuido beat me to it...
```

---
## \#4 Posted by: BigAl Posted at: 2016-01-14T03:33:49.437Z Reads: 227

```
so whats the deal with the spark that occurs when you pull the plug?  can it ruin the VESC?  I was thinking of making a dead man kill switch and was wondering if it would be a problem.  Is the problem on unplugging or plugging in?  or both?

Thanks
Al...
```

---
## \#5 Posted by: psychotiller Posted at: 2016-01-14T03:53:38.383Z Reads: 213

```
If you use an antispark loop key there will be no sparks ever.
```

---
## \#6 Posted by: lowGuido Posted at: 2016-01-14T04:04:06.901Z Reads: 210

```
the spark is actually caused by the VESC so to speak.
the spark is caused by the Caps causing a large inrush of current on connection. in fact if you connect and get a spark, then disconnect and re connect you will notice there is no spark the 2nd time.

if you charge the caps before connecting then there is no inrush (because caps are already full) and result: no spark.
and basically that's what these devices do. they allow the caps to charge slowly through a resistor first before connecting fully.
 I don't believe that you could actually damage the VESC with (this) spark.
the connectors on the other hand.. they get damaged and can erode away

edit on another note: if you DON'T get a spark when you connect that is a sign of weak Caps and caps should therefore be replaced (as I have mentioned in another thread) having sick caps CAN certainly cause damage to your ESC
there is a whole different school of thought here as well. some people refuse to use anti spark because it doesn't continue to give a good gauge of cap health, preferring to replace their connectors every now and then rather than not knowing if their caps are dead. Castle creations actually quote "the spark is your friend"
> The spark is your friend. If ever you plug your pack into your controller and you don’t see the spark, contact tech support at support@castlecreations.com or (913) 390-6939 and send the controller in for repair. Your capacitors will need to be changed. NEVER fly if you do not see the spark, especially with high voltage applications! The higher the voltage, the bigger the spark should be. Remember, the spark is your friend!!!
```

---
## \#7 Posted by: NNGG Posted at: 2016-01-14T05:06:23.445Z Reads: 183

```
Im confused, what is the pro and con of an antispark plug? Will my vesc be damaged form continual sparks? Is it worth the $10-20?
```

---
## \#8 Posted by: lowGuido Posted at: 2016-01-14T05:21:47.284Z Reads: 178

```
Pro: you wont erode the contacts of your plug

Con: you wont know if your caps are dead.
```

---
## \#9 Posted by: NNGG Posted at: 2016-01-14T06:58:58.998Z Reads: 173

```
Guess I'll just replace my deans connectors
```

---
## \#10 Posted by: Hummie Posted at: 2016-01-15T18:12:26.824Z Reads: 169

```
The xt90s plugs are a great simple solution.  

big. Easy to solder.  No shrink wrap required. I don't bother making a loop just use them as the main battery connection. Make sure you push them all the way together. 

I also installed one on my bulk charger and I only  charge through one plug. Simple.  I also use a 10$ balancer/discharger and want to convert a standard 12 volt laptop charger to charge 3s packs through the balance leads. I like to only have to take one plug apart and it's at least a big one<img src="/uploads/db1493/original/2X/3/3e53b8ad4614e65a8d537750e6205e84d7497b40.jpg" width="375" height="500">

I bring the bulk charger up because  it's simplifies things.<img src="/uploads/db1493/original/2X/6/6f8facdc39d262458b404b5335f666e9a55a8e61.jpg" width="666" height="500">
Protecting the vesc from physical damage is something else though and I want to pot these I rubber soon.
```

---
## \#11 Posted by: lowGuido Posted at: 2016-01-15T22:10:21.934Z Reads: 149

```
@Hummie is that velcro holding your lipos on there?
```

---
## \#12 Posted by: lowGuido Posted at: 2016-01-15T22:12:07.131Z Reads: 147

```
@NNGG or you could use an XT90 loop key and then every now any then short it to check for spark, that way you have the best of both worlds. (so long as you remember)

I gotta admit. I don't like the spark. i have loop keys on one of my builds, and a circuit breaker on another, i have a manual charge resistor on another, and one I have nothing. 
out of all I prefer the breaker.
```

---
## \#13 Posted by: NNGG Posted at: 2016-01-15T22:17:59.715Z Reads: 144

```
Well I don't really care and just want the least amount of trouble for this exact area, and If it doesn't hurt the batteries or the VESC, then Im happpy.
```

---
## \#14 Posted by: NNGG Posted at: 2016-01-15T22:19:07.447Z Reads: 142

```
Do you have 12S going into both your hub motors?
```

---
## \#15 Posted by: lowGuido Posted at: 2016-01-15T22:19:09.945Z Reads: 142

```
yeah its certainly the cheapest and easiest option. i mean deans connectors are like $1 a bag anyway.
```

---
## \#16 Posted by: NNGG Posted at: 2016-01-15T22:19:50.963Z Reads: 143

```
same I spent $20 and now have at least 100+ deans connector pairs
```

---
## \#17 Posted by: Hummie Posted at: 2016-01-16T01:46:29.709Z Reads: 145

```
I thought the spark was bad for the esc, or maybe it kills the capacitors and then the esc?  

12s in series to 2 vesc in parallel. 12s to both.  I wonder if anyone does esc in series.  

Just Velcro.  It's temporary but those work with packs up to 3s for me.   I want to pot 24 18650 li-ion cells stuck to the board in clear 70 duro polyurethane. And 

Buuuuuyyyy.  Mmmmmmyyyyy motoooorss!  Come on guys these things rock and I'm selling them for less than anything available.  I won't screw you on rubber cost later. 
And I'm charged and back out! 
Really loving the board. My old board I almost never rode it was so loud and awkward. The vesc and these motors have potential.
```

---
## \#18 Posted by: lowGuido Posted at: 2016-01-16T11:57:38.511Z Reads: 125

```
7 posts were merged into an existing topic: [The nicest hub motors! For sale cheaper than anywhere!](/t/the-nicest-hub-motors-for-sale-cheaper-than-anywhere/1002)
```

---
