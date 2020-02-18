# XT90S Anti-spark Loop Key Polarity

### Replies: 22 Views: 2406

## \#1 Posted by: roamin Posted at: 2016-10-24T03:00:03.001Z Reads: 290

```
Hey gang, I'm placing the loop key on the negative line, going from the VESC back to the battery. Does the polarity of the XT90 matter? I'd imagine it's positive terminal is on the VESC side, with the negative terminal running back to the battery - just want to confirm! Thanks
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-24T03:01:43.988Z Reads: 289

```
It doesn't matter. But for cleanliness, put the - side of the connector to the - side of the battery.
```

---
## \#3 Posted by: kyo Posted at: 2016-10-24T03:13:09.639Z Reads: 284

```
one more question? does it matter if the anti-spark loop key is on negative or positive wire of the battery ???
```

---
## \#4 Posted by: chinzw Posted at: 2016-10-24T03:23:47.818Z Reads: 277

```
In theory its the same (think of your wiring as a circle O, current just "flows" around the circle, wherever you cut that circle its the same. In practice, its better to cut the positive side because of common ground. But for this application, where the loop key will be directly connected to the battery either positive or negative is fine.
```

---
## \#5 Posted by: lox897 Posted at: 2016-10-24T04:59:39.315Z Reads: 251

```
If it is an xt90s then yes the polarity can matter. Some have reported melting connectors cause the resistor was on the wrong side.
```

---
## \#6 Posted by: Maxid Posted at: 2016-10-24T05:15:24.411Z Reads: 240

```
That was a myth and I still think they simply made mistakes by for example not inserting the plug correctly. There is just a resistor in there - why should polarity matter?
```

---
## \#7 Posted by: lox897 Posted at: 2016-10-24T05:18:07.839Z Reads: 233

```
Not sure. @sl33py or @barajabali (can't remember who) said that when they did it the other way it worked. I think the resistor is on one side so that the current from the batteries is limited when it comes in, not when it goes out.
```

---
## \#8 Posted by: IDVert3X Posted at: 2016-10-24T06:06:17.260Z Reads: 226

```
Its a loop, doesnt matter where the resistor is, also, resistor has no polarity.
```

---
## \#9 Posted by: lox897 Posted at: 2016-10-24T10:14:16.566Z Reads: 217

```
I know that resistors have no polarity. I'm just confused as to why some people's issues have been fixed when they swapped it around.
```

---
## \#10 Posted by: Maxid Posted at: 2016-10-24T11:47:39.427Z Reads: 210

```
http://www.electric-skateboard.builders/t/melting-loop-key-solved/5241/65

maybe because it was a different issue from the start ;)
```

---
## \#11 Posted by: DeathCookies Posted at: 2016-10-24T12:18:17.194Z Reads: 199

```
[quote="Maxid, post:10, topic:11780"]
maybe because it was a different issue from the start
[/quote]

Well, i have experienced it like @lox897 said

My wiring was correct but my loop key got destroyed when i plugged it in the first time...
I changed the loop key with a new one and plugged it in the other way. Since then it is working.
[My thread to it](http://www.electric-skateboard.builders/t/xt90-s-loop-key-short-circuit/2383)
```

---
## \#12 Posted by: Maxid Posted at: 2016-10-24T12:56:45.126Z Reads: 181

```
exactly - "you destroyed it the first time you plugged it in" perfectly describes how you most probably have not plugged it in correctly and just concluded from there that something bigger must be wrong. After the initial mistake the resistor died and you always got a spark. If you had used your new plug in your old configuration it would have also worked. Also everybody in your thread told you that the polarity does not matter.
```

---
## \#13 Posted by: DeathCookies Posted at: 2016-10-24T13:19:10.883Z Reads: 169

```
**How** can i **not** plug in my XT90-S **correctly?**
Or what was wrong with my wiring when i have not changed **ANYTHING** except a new XT90-S in another orientation?

Would be good to know!
```

---
## \#14 Posted by: Maxid Posted at: 2016-10-24T13:25:27.980Z Reads: 159

```
For example the way I linked directly above: not inserting it all the way. Your wiring was right and it would have worked with a new plug no matter the orientation you had used. You can't conclude it was a polarity issue solely on the fact that you turned it around and it works now. That is not the way to go. You would have to retest after making sure the plug works correctly on its own (like you did now). I am sure that changing the polarity now will not make a difference in your system.
```

---
## \#15 Posted by: DeathCookies Posted at: 2016-10-24T13:33:49.102Z Reads: 163

```
[quote="lox897, post:9, topic:11780"]
I know that resistors have no polarity.
[/quote]

Me too.
[quote="Maxid, post:14, topic:11780"]
You can't conclude it was a polarity issue solely on the fact that you turned it around and it works now. That is not the way to go.
[/quote]
you are right ;)

[quote="Maxid, post:14, topic:11780"]
For example the way I linked directly above: not inserting it all the way.
[/quote]
I disagree!
When i plug it in half way that only the resistor is touching the plug my XT90-S should not be melted! The resistor refuses the energy to flow with high current. But when you just plug it in halfway to turn the board on (**not riding**) there is no high current needed. Why should the resistor blow?
```

---
## \#16 Posted by: IDVert3X Posted at: 2016-10-24T13:56:30.769Z Reads: 153

```
Just accept the fact that it was human error ( or faulty product - less likely ).

[quote="DeathCookies, post:15, topic:11780"]
Why should the resistor blow?
[/quote]

There is a voltage drop voltage drop across the resistor ( depends on the current and resistance ).
If the current flows, heat level increases until it's fucked up.
```

---
## \#17 Posted by: DeathCookies Posted at: 2016-10-24T14:09:26.836Z Reads: 150

```
[quote="IDVert3X, post:16, topic:11780"]
Just accept the fact that it was human error ( or faulty product - less likely ).
[/quote]

That could be a reason... everytime...[quote="IDVert3X, post:16, topic:11780"]
There is a voltage drop voltage drop across the resistor ( depends on the current and resistance ).If the current flows, heat level increases until it's fucked up.
[/quote]

The XT90-S is designed for the current. So why should the resistor of the XT90-S blow?
```

---
## \#18 Posted by: IDVert3X Posted at: 2016-10-24T14:11:00.257Z Reads: 147

```
The resistor is designed to handle the current for very short period of time.
Heat accumulates and small package like this can't handle much heat.
That's why you have to always push it all the way in.

Let's do the math. You have 100R resistor for example.
If using 42V, it will limit the current to 420mA.
420mA @ 42V gives you ~ 17W, and that's A LOT of heat!
It's designed to handle this current for a fraction of a second when pushing the connector in.
```

---
## \#19 Posted by: DeathCookies Posted at: 2016-10-24T14:20:27.230Z Reads: 144

```
Maybe many ppl are to shy to plug it in completly in half a second.
Thanks for the clarification.
```

---
## \#20 Posted by: TarzanHBK Posted at: 2016-10-24T14:25:50.681Z Reads: 148

```
also these are not hightech connections/solderings inside that xt90s, so if you have a weak connection due to a bad production, it could melt down in a few seconds if you don´t push it all the way in directly.
 the next connector might be better and have a more solid connection, so that it handles the heat longer.
```

---
## \#21 Posted by: IDVert3X Posted at: 2016-10-24T14:26:51.974Z Reads: 140

```
That's right.
It doesn't necessary have to be half a second, second or two should be fine.
```

---
## \#23 Posted by: sl33py Posted at: 2016-10-24T17:33:47.525Z Reads: 136

```
[quote="DeathCookies, post:13, topic:11780"]
except a new XT90-S
[/quote]


There are two likely failure points here for the simple XT-90s loop key melting:

1 - not plugged all the way in.  That small resistor doesn't stand a chance of handling the full load.  Poof!  Especially when new these suckers are TIGHT and can be tough to seat fully.  

2 - they fail.  simple.  They are made cheaply and if one misses a good QC and has an issue - it'll still fail if everything else is still correct.  My assumption of your issue @DeathCookies.

Orientation should not matter.  Period.  If you did not fully kill it and swapped orientation and it worked i would then suspect some soldering issue or similar.  But most of the time it will die if it goes - and a new XT-90s that works in the other orientation may seem like the fix, but i'd be willing to bet you a shiny nickel if you swapped it - it would still work.

Still one of the easiest and cheapest ways to suppress the spark.  Definitely worth getting a few spares just in case.
```

---
