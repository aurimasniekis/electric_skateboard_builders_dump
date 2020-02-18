# Is any vesc X on/off switch solution

### Replies: 16 Views: 4144

## \#1 Posted by: Hoho0220 Posted at: 2016-12-06T16:02:11.189Z Reads: 353

```
hi everyone 
I bought 2 Vesc-X.
I find this Vesc-X without any switch.
How can I turn off Vesc X( Vedder antispark or Loop key)?
Could I charge the battery when Vesc X turn on?
```

---
## \#2 Posted by: rpn314 Posted at: 2016-12-06T16:08:27.105Z Reads: 352

```
You'd need something before the VESC (An anti-spark switch or anti-spark loop-key) The vesc has never had a built in on/off solution. There's a number of solutions around here.

As for charging while it's on, it won't damage it, but it could create some interesting circumstances like if you accidentally hit the remote and the board takes off across the room and damages something (and/or itself), so I don't recommend it.
```

---
## \#3 Posted by: Hoho0220 Posted at: 2016-12-06T16:34:59.202Z Reads: 333

```
I plan buy  XT60 Connector - 2 in 1 Series

http://www.quadrocopter.com/XT60-Connector--2-in-1-Series_p_172.html

Then diy a XT60 loop key.

Is it OK?

I found in http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204/18

XT 60 loop key is welded with 680 ohm resistor.
Is this resistor necessary?
thank you for your kindly reply.
```

---
## \#4 Posted by: themegak Posted at: 2016-12-06T16:42:51.625Z Reads: 297

```
no offense but there are a bunch of posts about this very thing.  If you search  for this and how to build an eboard, all will be revealed to you.  Also, yes the resistor in necessary for what you are trying to do.
```

---
## \#5 Posted by: rpn314 Posted at: 2016-12-06T16:48:45.977Z Reads: 277

```
Sorry, I tried to be nice about it ("There's a number of solutions around here"), but yes, try searching a bit more. This topic has been addressed a lot.
```

---
## \#6 Posted by: jga Posted at: 2016-12-07T12:54:41.759Z Reads: 235

```
Sorry, I did not find anything similar to "anti-spark loop key for the dummies", maybe my search is not pointing in the right direction. All the threads I have found assumes the basic knowledge is well known by the readers on this topic, and clearly i am not there yet even if I start to understand the principle. :confused:
Can you guide me to an existing post on this if it is somewhere?
Thanks
```

---
## \#7 Posted by: themegak Posted at: 2016-12-07T14:30:31.330Z Reads: 218

```
are you serious ?  [How-To: Anti-Spark XT-90 Loop Key](http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204) .
```

---
## \#8 Posted by: Hoho0220 Posted at: 2016-12-07T14:41:29.098Z Reads: 213

```
I think that you can buy a XT60 Connector - 2 in 1 Series .
then DIY a loop key. finish the project
```

---
## \#9 Posted by: jga Posted at: 2016-12-07T15:03:17.398Z Reads: 205

```
Yes, I have seen this threads, and sorry but the discussion is not clear. There has been much better posts on batteries, VESC, motors,... I cannot see why it is not possible to have the same on this topic.
If you can build something with the schematic proposed on feb 23 then it means you did not need to read the previous messages, as it is anything but clear.
I would like something that starts with the basis in a few words: do you absolutely need it? How does it work? How do you use it (compare to a simple on/off switch? And a clear schematic on how to connect the various elements of the system.
```

---
## \#10 Posted by: themegak Posted at: 2016-12-07T15:14:03.850Z Reads: 185

```
Yes you need some kind of anti spark switch.  Sparks are thrown when you power on the vesc with whatever battery you use and sparks are bad news.  You absolutely need to use an anti spark switch to both protect your investment and to be safe.  You can buy one premade from  or esk8.de or make one out of xt90s connectors, or if you want to get hardcore you can source and make a vedder antispark switch (i think ollin sells these as well), and you can always make a loop switch with xt90s connectors.  Hope that clears it up for you.
```

---
## \#11 Posted by: jga Posted at: 2016-12-07T15:25:06.886Z Reads: 176

```
Thank you. 
Of course at $50 or $60 a piece, I'd rather build my own one! They must make 400% margin on this product!
But these are switches, and I understood from some of the posts that it was not necessarily ideal. Is that correct?
```

---
## \#12 Posted by: rpn314 Posted at: 2016-12-07T15:29:26.852Z Reads: 168

```
Go ahead and build your own! I did (as well as almost everything else in my board) and I can tell you they're definitely not making anywhere near 400%. Most of those around here are selling them close to cost. In the solid-state anti-spark switches (like vedder's and those sold by Ollin and diy), high quality mosfets are not cheap.
```

---
## \#13 Posted by: Hoho0220 Posted at: 2016-12-07T15:53:05.372Z Reads: 169

```
http://www.electric-skateboard.builders/t/project-ai-custom-deck-90mm-wheel-caliber-v2-50-degree-single-motor-sk3-6354-custom-motor-mont-enertion-vesc-2x-4s-5000mah-20c/11731/4
```

---
## \#14 Posted by: jga Posted at: 2016-12-07T16:17:15.823Z Reads: 163

```
Ok, I start to see how it should look like. So on the left it goes back to +/- of the battery, and on the right to the ESC/VESC. And on the top we have the famous loop. What are the two small black and red wires with the white connector? And what is the string at the top used for: is that to cut the circuit?
```

---
## \#15 Posted by: darkkevind Posted at: 2016-12-07T16:32:31.116Z Reads: 167

```
This should serve well for an on/off switch. You can add a momentary switch sending 5v from the receiver to the relay which will latch the relay.

This one is rated for 80A but they do a 100A one as well.

http://www.ebay.co.uk/itm/10A-To-100A-Solid-State-Relay-SSR-DC-DC-3V-32V-DC-5V-220V-DC-High-Quality-/262715391180?var=&hash=item3d2b0ebccc:m:mgkEkzSrMH1ykXQ3_O6pqQw
```

---
## \#16 Posted by: sl33py Posted at: 2016-12-07T18:45:32.533Z Reads: 160

```
[quote="jga, post:11, topic:14268"]
Of course at $50 or $60 a piece, I'd rather build my own one! They must make 400% margin on this product!
[/quote]


HA - wait until you price out the BOM.  As i recall it was around 15-20$ in components alone.  The FETs are around 3-5 ea.  Getting the PCB's the price varies a ton depending where you get them and quantity prices help.

I had a "kit" of all the components and my math had about $7-10 "profit" which i split 50/50 with Vedder.  All gone now, but just so you see there really isn't much $ to be made.  I'd bet even at large quantities discount you *might* get 20-30 profit max.  And hold onto that stock and bill on your credit card for a year waiting for them all to sell.  Definitely not a "get rich quick" scheme...  And for 100-120% profit a pretty poor return.  My 20 extra kits took over a year - not that i pushed them or made much effort to sell them...

AND - perhaps most importantly - _you need to know how to do hot-air rework or SMD soldering._  (skillet, oven, hot-air).  This is not as simple as it may look and i know a few kits went to folks who butchered them.  I intentionally did not sell a few as they said they had no experience and i suggested they buy a pre-made vs waste money on something they can't build.  Super tiny little components and you need more than basic solder skills.  One guy said he did his whole thing w/ an iron, but i'm curious how those FETs have held up - they are temp sensitive and overheating them to get the solder under them to flow likely will damage them.  Also the most $ component to replace if you F it up...

And like @themegak linked - i did a writeup to make your own cheap anti-spark loop key a few years back.  Still the cheapest solution...
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204


HTH - GL!
```

---
