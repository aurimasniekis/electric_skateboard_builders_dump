# XT90-S loop key short circuit

### Replies: 30 Views: 6089

## \#1 Posted by: DeathCookies Posted at: 2016-04-15T20:57:52.103Z Reads: 454

```
Today i attached my new motor (12S) and resoldered my setup from 6S2P to 12S1P. I did it like the following wiring from @trbt555. Thanks for this.
http://www.electric-skateboard.builders/uploads/db1493/original/2X/2/2677600ddb451bf7ea5cb112584e83df8ee9e82a.PNG
I used a XT90-S for the loop key. I plugged it in and it instantly short the circuit. My VESC is alright but the XT90-S key is burned... Now when i plug it in it will always spark....
<img src="/uploads/db1493/original/2X/c/c886484467108237b7c6874f8b42910f5ca690e5.jpg" width="375" height="500">
Did anybody get the same problem?
Faulty XT90-S?? 
Did i plug it in too fast?
```

---
## \#2 Posted by: lowGuido Posted at: 2016-04-15T21:58:12.602Z Reads: 419

```
you have made a mistake in the wiring.. I would guess you have the balance leads the wrong way around.

...if I had a dollar....
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-04-15T21:59:46.443Z Reads: 421

```
The balance leads are not connected. It did not happen while charging.
It happened as i wanted to power my system for a test drive.

But why should be the wiring of the balance leads wrong? That way i can discharge them in series and charge them simultaniously with my dual charger.
```

---
## \#4 Posted by: psychotiller Posted at: 2016-04-15T22:32:00.724Z Reads: 407

```
The loop key only needs to be spliced into either the ground wire or the positive wire. Not both. If you didn't use an xt90 anti spark plug then you will get a spark.
```

---
## \#5 Posted by: paragon Posted at: 2016-04-15T22:36:04.271Z Reads: 406

```
What did you expect, you connected the positive straight to the negative with that loop key :open_mouth:
It is supposed to connect/disconnect either the positive OR the ground, but positive is more often used, because there can be multiple grounds.
Best of luck with the build!


Edit: Nevermind, the chart looks correct. What is the anti-spark connector rated for? Are the batteries in series the exact same model? Are they both charged to the same voltage?
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-04-15T22:51:11.055Z Reads: 393

```
[quote="paragon, post:5, topic:2383"]
What did you expect, you connected the positive straight to the negative with that loop key :open_mouth:
[/quote]

<img src="/uploads/db1493/original/2X/9/98b5e85a8bab1f886c49ec62324c7f2255d98779.png" width="690" height="407">
(red connectors = XT90-S / black connector = XT90)
Do these wirings make a difference?
I believe the  following but i can be proofed wrong ;) 

There will be no difference 
--> i dont create a circuit if i dont attach an esc. If i attach a esc there will be a circuit and the current will always  flow through the XT90-S plug.
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-04-15T22:57:01.296Z Reads: 366

```
[quote="psychotiller, post:4, topic:2383, full:true"]
The loop key only needs to be spliced into either the ground wire or the positive wire. Not both. If you didn't use an xt90 anti spark plug then you will get a spark.
[/quote]

I want to learn something so i just wrote down my questions. I hope i get them answered ;)

1. So i dont have a chance to charge it seperate and discharge parallel? 
2. Only way would be to change the XT90-S with a normal XT90 and splice a new XT90-S into ground or positive?
3. Which one is preferred? And why? positive or negative?
```

---
## \#8 Posted by: laurnts Posted at: 2016-04-15T23:24:24.431Z Reads: 352

```
To be simple, consider anti spark loop key as a switch. You only instal it on the positive side / negative side.
So both wires that goes in and out of the anti spark should be the same color (only red or only black).

ohh I see you use the antiloop for the series connector. Then @lowGuido is correct, you have missed something within your balance plug.

---

If it still shorts, my suggestion is now to swap your balance plug around.  6s and 6s into 12s.
Left 6s balance plug to the right side and the right 6s balance plug to the left side. Seems weird at beginning (they are still end up as 12s anyway) but it does change the polarity of the balance plug removing your shorts.
```

---
## \#9 Posted by: lowGuido Posted at: 2016-04-15T23:39:55.928Z Reads: 332

```
the connection of the loop key is correct that's not in question. 
something else happened to pop the resistor in the anti spark, and that's why you are now getting a spark.. I don't know what happened to cause it, I can only assume some sort of short..
```

---
## \#10 Posted by: laurnts Posted at: 2016-04-15T23:46:04.502Z Reads: 325

```
Well if it gets shorted out earlier, that resistor is dead for sure. It's a small 100ohm'sih resistor can't handle the heat and current that large from lipo packs.
```

---
## \#11 Posted by: lowGuido Posted at: 2016-04-15T23:49:22.804Z Reads: 326

```
yeah once its gone its anti spark capability is no more.

does the VESC still power up? I cant think of how you could have shorted it unless it was the balance leads?can you take photos of the actual setup? the diagram is fine, but i'd like to see the real life picture.
```

---
## \#12 Posted by: laurnts Posted at: 2016-04-16T00:02:03.336Z Reads: 321

```
[quote="DeathCookies, post:7, topic:2383"]
Which one is preferred? And why? positive or negative?
[/quote]

I prefer negative side, because thats were the electrons (the current) is flowing from. Also BMS'es seems to alternate the negative side for either charging or power switching, so I believe negative side is better.

[quote="DeathCookies, post:7, topic:2383"]
So i dont have a chance to charge it seperate and discharge parallel?
[/quote]

Your diagram is correct. Your diagram shows you are discharging in series. You can charge separate and discharge parallel.

[quote="DeathCookies, post:7, topic:2383"]
Only way would be to change the XT90-S with a normal XT90 and splice a new XT90-S into ground or positive?
[/quote]

I dont quite understand the question. XT90s and XT90 have no difference at all, one provide anti spark function and the other doesnt. You can use all XT90s or XT90 or combination doesnt even matter.
```

---
## \#13 Posted by: lowGuido Posted at: 2016-04-16T00:12:41.272Z Reads: 272

```

nah there is nothing wrong with the way you have it set up @psychotiller and @paragon just didn't understand what you were doing. the diagram is correct, but I want to see real world photos.
```

---
## \#14 Posted by: psychotiller Posted at: 2016-04-16T00:21:11.721Z Reads: 267

```
Yeah I had to stare at it for a while..it looks like a nice way way to run series and charge parallel. If the balance leads weren't plugged into the charger why the spark then?
```

---
## \#15 Posted by: lowGuido Posted at: 2016-04-16T00:22:00.944Z Reads: 273

```
well thats the $500 question isnt it?

I recognised the circuit right away because it is mine.
```

---
## \#16 Posted by: laurnts Posted at: 2016-04-16T00:39:25.671Z Reads: 273

```
Just get a voltmeter and test each connection before making the plug. If theres voltage reading, that means its a short! Do not plug it in.
```

---
## \#17 Posted by: trbt555 Posted at: 2016-04-16T08:05:47.496Z Reads: 270

```
Show us a clear picture of your wiring please.
```

---
## \#18 Posted by: DeathCookies Posted at: 2016-04-16T10:54:36.408Z Reads: 289

```
The resistor of the xt90-s was directly shorten after i plugged it in the first time. Since that i always get a spark... Obviously. I still can Run my system with no Problem. I just always get a spark. 
If i still plug it in and it will spark does it make serious damage in long terms?

Here are some photos. I hope that they are not too Bad otherwise i have to take it apart. <img src="/uploads/db1493/original/2X/2/22a61bb55f46eb781ae2748f23270c033f66dccd.jpg" width="666" height="500">that are the Batteries and the charging cables. 
<img src="/uploads/db1493/original/2X/d/d9964288564236a48fb924fe1c681a54cddb33e1.jpg" width="375" height="500">that is the series Adapter with loop key. The cable to the legt upper and right upper are for the batteries and the only one going down is for the vesc
```

---
## \#19 Posted by: lowGuido Posted at: 2016-04-16T10:59:38.425Z Reads: 282

```
what are the balance plugs connected to in that photo?

the spark wont damage anything. its just the inrush to the caps. it tells you your caps are good.
the thing I want to know is why it blew the resistors in the first place
```

---
## \#20 Posted by: DeathCookies Posted at: 2016-04-16T11:02:05.944Z Reads: 283

```
It did not happen while charging. It happened when i Run the System. 
<img src="/uploads/db1493/original/2X/e/eccdab2783bd155fe900b0f360e3fac2053289b2.jpg" width="666" height="500">
That is the charging cables of one battery. The outside is for the charger. The right upper cable is for the battery and the right cable below is for the vesc or the series adapter
```

---
## \#21 Posted by: lowGuido Posted at: 2016-04-16T11:03:24.753Z Reads: 273

```
ahh k.
have you tried another anti spark plug for the loop?
```

---
## \#22 Posted by: trbt555 Posted at: 2016-04-16T11:16:28.641Z Reads: 265

```
The spark won't damage other components, it will just wear out  your loop key over time.
If all your wiring is correct then it could be a dodgy loop key.
```

---
## \#23 Posted by: DeathCookies Posted at: 2016-04-16T15:03:58.917Z Reads: 263

```
[quote="trbt555, post:22, topic:2383"]
If all your wiring is correct then it could be a dodgy loop key.[/quote]

I thought this wiring was a good idea. I will replace the xt90-s with a new one and retest it. Back to my questions:
1. Do you have a better wiring i could test? (maybe i change the XT90-S with a normal XT90 and splice a new XT90-S into negative ?
2. Faulty XT90-S?? 
3. Did i plug it in too fast?
```

---
## \#24 Posted by: trbt555 Posted at: 2016-04-16T16:05:27.860Z Reads: 250

```
If the xt90s resistor blew, there was obviously an overcurrent.
There must be a short somewhere in your system.
You cannot have anything plugged into the charge or balance connections when you insert the loop key.
You need to re-check if your wiring corrsponds to the schematic.
Perhaps you can draw up a schematic of precisely how you've rigged it together.
```

---
## \#25 Posted by: lowGuido Posted at: 2016-04-16T21:50:31.967Z Reads: 261

```
[quote="DeathCookies, post:23, topic:2383"]
1. Do you have a better wiring i could test? (maybe i change the XT90-S with a normal XT90 and splice a new XT90-S into negative ?2. Faulty XT90-S?? 3. Did i plug it in too fast?
[/quote]

1.) This is as far as I can see the best or only wiring for this situation. (adding more loop keys would be pointless)
2.) It is now.
3.) No.
```

---
## \#26 Posted by: Hummie Posted at: 2016-04-17T05:29:39.275Z Reads: 257

```
All that complicated wiring.  Why not just use the xt90s plug as a plug?  <img src="/uploads/db1493/original/2X/3/36a14241832c4eede321630062c14507627c672d.jpeg" width="375" height="500">
Charging or turning on or of
```

---
## \#27 Posted by: lowGuido Posted at: 2016-04-17T06:34:50.534Z Reads: 252

```
@hummie I think you missed the point. its so that you can charge as 6S and discharge as 12S
and its not really that complicated.
```

---
## \#28 Posted by: Hummie Posted at: 2016-04-17T13:56:35.360Z Reads: 252

```
Ok that's the point.  

I have the same problem since I also have a vesc and want to use 12s.  12s chargers are pretty much non-existent but the set-up I use now Im really happy with as it seems the simplest, least amount of plugging and unplugging, and the cheapest.  I use a Meanwell bulk charger and wire in a wattmeter and use a couple 15$ balancers at the same time.  I hate plugging and unplugging balance plugs into chargers.  They always get stuck and require a lot of force. These little balancers are really easy to put plugs in or out of, or even just lay them just touching. [Uploading...]() 

I can charge at 400watts.  

If anyone is nyerested in my Icharger that does 8s I'm getting rid of it cheap. Make me an offer
```

---
## \#29 Posted by: DeathCookies Posted at: 2016-04-20T21:29:40.698Z Reads: 249

```
Today I rechecked my wiring and did find the mistake... I just soldered it like the wiring you have Seen before. Exactly like the wiring diagramm and that was my mistake. <img src="/uploads/db1493/original/2X/7/7e282727778eecae40ff5fbf95f60c1f66e747b0.PNG" width="479" height="500">
In that wiring the polarity of the xt90-s loop key will be wrong! In the diagramm there is a Red positive cable to the left and the black negative on the right. But when we Look at the Battery cables they go the other way to the Esc... So i changed the polarity and blow my xt90-s. 
Thanks for the Input! I really appreciate this forum ;)
```

---
## \#30 Posted by: lowGuido Posted at: 2016-04-20T23:33:31.633Z Reads: 236

```
to be fair, the diagram doesn't really show polarity of the XT connectors but just a box which represents them.

having said that I'm also surprised that it matters. if you were connecting a battery to a load then the polarity is important, but a loop key shouldn't really matter about polarity.

either way its good that you have sorted out the problem.
```

---
