# Just asking for someone to give his blessing

### Replies: 30 Views: 949

## \#1 Posted by: MartyMcFly88 Posted at: 2017-11-14T23:27:45.706Z Reads: 155

```
Hey,

this is my first project like this and although i have read a LOT :) about this topic (thanks for all the details in your amazing builds btw.) I still have some questions. I am planing on a single motor build 
-SK3 6364 190KV,  
-3D printed motor mount with printed gearing as well (15-36) 15mm belt 
-90mm flywheel clones, 
-10S4P Battery from 30Q cells 
and a Vesc to keep everything in control. Now my first Question:  
would it work like this:  

 <img src="/uploads/db1493/original/3X/6/d/6d975ee22bab83340e4029651c53c841fce82247.jpg" width="375" height="500">
	
 
I think the wiring is ok like this(?) but in about 90% of the builds i have seen on this forum the batteries are arranged crosswise, is there any advantage to that? 
And which thickness of cable is recommendable for this kind of setup?  
I'd love any input you can offer me,
Cheers and have a good night.
```

---
## \#2 Posted by: michaelcpg Posted at: 2017-11-14T23:30:36.603Z Reads: 122

```
Looks pretty good to me, but maybe check with someone else just in case. I did a similar setup with a split battery and used 10AWG silicone wire. One thing to think about is including a balance/charge circuit.
```

---
## \#3 Posted by: MartyMcFly88 Posted at: 2017-11-14T23:35:57.245Z Reads: 115

```
I thought i would use the place where the anti spark plug is to charge the batteries? Or is this unwise because of sparks? Could I simply install a splitter the way I plan for the Voltmeter? 
Concerning balance, I was just going check the packs every few month.
```

---
## \#4 Posted by: scepterr Posted at: 2017-11-14T23:36:54.596Z Reads: 105

```
It looks like the antispark is between 2 batt packs? It should in front of all the batteries before the vesc

The way it is now the antispark joins the 2nd bank to the first
```

---
## \#5 Posted by: MartyMcFly88 Posted at: 2017-11-14T23:38:05.593Z Reads: 96

```
Does that matter? as long as the circuit is not closed nothing can happen, right?
```

---
## \#6 Posted by: scepterr Posted at: 2017-11-14T23:39:02.467Z Reads: 94

```
It's wierd, I haven't seen anybody put an antispark in between series connections

How would charge through it? It's positive only

Also I don't get how it could antispark the vesc when the first bank is plugged directly into vesc
```

---
## \#7 Posted by: MartyMcFly88 Posted at: 2017-11-14T23:40:18.070Z Reads: 86

```
no the batterypack on top is actually two packs, the are not connected.
```

---
## \#8 Posted by: scepterr Posted at: 2017-11-14T23:40:47.908Z Reads: 85

```
Antispark needs to be between battery and vesc
```

---
## \#9 Posted by: b264 Posted at: 2017-11-14T23:41:57.918Z Reads: 84

```
This would work fine with no BMS and never charging it.  I don't think you'll be able to hook up a BMS and/or charge it unless you intend to charge it only with the loop key installed.  And even then, I think the balace wires would present a big problem.  I would move the loop key as others suggested
```

---
## \#10 Posted by: scepterr Posted at: 2017-11-14T23:42:35.151Z Reads: 81

```
@b264 and not through the loopkey
```

---
## \#11 Posted by: MartyMcFly88 Posted at: 2017-11-14T23:49:16.192Z Reads: 78

```
I don't undestand why i would have to change the position of the loop key, sorry I don't mean to question your judgement, I would just like to understand :) 
If I installed a double XT60 switch at the top, could I charge the batteries through that? of course with the antispark plugged in!
Sorry for the hassle ..
```

---
## \#12 Posted by: scepterr Posted at: 2017-11-14T23:51:51.024Z Reads: 65

```
For the antispark to antispark it needs to between the vesc and battery, otherwise you'll get current inrush as soon as you plug in xt90s in the middle of the pack, it needs be at the start

It will not perform antispark function otherwise, it'll just be a connector

Loopkey is not just for power on/off
```

---
## \#13 Posted by: MartyMcFly88 Posted at: 2017-11-14T23:53:18.329Z Reads: 62

```
Shouldn't it work if it is the last thing i plug in?
```

---
## \#14 Posted by: scepterr Posted at: 2017-11-14T23:53:42.417Z Reads: 58

```
No 
10 char
```

---
## \#15 Posted by: michaelcpg Posted at: 2017-11-14T23:58:42.327Z Reads: 54

```
Pretty sure the antispark is fine where it is tbh if you're not planning on including a BMS for balancing
```

---
## \#16 Posted by: ARetardedPillow Posted at: 2017-11-15T00:00:30.177Z Reads: 53

```
Should put the antispark between the battery and the vesc and the volt meter between the antispark and the vesc, 3d printed motor mount might break tho
```

---
## \#17 Posted by: michaelcpg Posted at: 2017-11-15T00:03:47.841Z Reads: 53

```
Can you explain why this would be the case? 

The antispark just works by temporarily adding a resistor into the circuit before the loopkey is fully inserted which prevents the sudden rush of current when the loopkey first makes contact with the rest of the circuit. 

Fairly sure that it shouldn't make a difference where in the circuit the resistor goes as long as it creates a point in the circuit that limits the current
```

---
## \#18 Posted by: scepterr Posted at: 2017-11-15T00:05:07.651Z Reads: 49

```
Try it let us know how it goes
```

---
## \#19 Posted by: michaelcpg Posted at: 2017-11-15T00:06:07.218Z Reads: 49

```
So you're just making assumptions and stating them as true then?
```

---
## \#20 Posted by: michaelcpg Posted at: 2017-11-15T00:07:28.604Z Reads: 54

```
> 3d printed motor mount might break tho

This is a good point, not sure how much luck others have had with 3D printing these sorts of parts but I personally wouldn't trust a 3D printed motor mount long term. Will depend a lot on the material you're using though
```

---
## \#21 Posted by: scepterr Posted at: 2017-11-15T00:07:29.704Z Reads: 43

```
Sure why not
```

---
## \#22 Posted by: MartyMcFly88 Posted at: 2017-11-15T00:07:54.697Z Reads: 46

```
From my very little understanding I am with michaelcpg on this one.. the way I understand it, the antispark plug is used if the circuit holds a lot of voltage when closed. The way it works is there is a resistor inside for the first part of the connection, so not all of the current flows at once, if i break the circuit and the antispark is the first to deconnect and the last one i connect it should work as intended.
```

---
## \#23 Posted by: scepterr Posted at: 2017-11-15T00:08:50.187Z Reads: 45

```
I'm happy to be wrong, means I learned something new, I just can't give my blessing as-is
```

---
## \#24 Posted by: korryh Posted at: 2017-11-15T00:09:20.389Z Reads: 49

```
Speaking from experience - do not print your motor mount or little motor gear - unless you are printing in some sort of metal composite.  

I printed my first mount and it gave out while I was going down a hill - turns out I can run really fast.

There are lots of metal motor mounts from sellers on this forum.
```

---
## \#25 Posted by: MartyMcFly88 Posted at: 2017-11-15T00:09:31.824Z Reads: 49

```
I thought I'd give it a hot :P the design looks promising it has metal inlays: 

https://www.thingiverse.com/thing:2429445

Oh yea i plan on only printing the big gear.
```

---
## \#26 Posted by: michaelcpg Posted at: 2017-11-15T00:11:26.419Z Reads: 45

```
Try it if you like I guess. If you're planning on riding at high speed, be prepared to bail at any moment if it suddenly decides to fail though, which won't be fun....
```

---
## \#27 Posted by: krloz Posted at: 2017-11-15T10:31:13.638Z Reads: 36

```
The antispark is fine where it is but only for antisparking  and as always only if it is the last thing pluged in because it is effectively breaking the cycle of power bat- vesc- battery.
You Will not be able to add a bms however. And for charging you will have to input power in parallel to the vmeter and the antispark HAS to be on to charge.  Wich is not good because the vesc  will be on.  Unless you turn it of some other way in which case if you then turn it on back again without pulling the antispark first BOOM sparks
```

---
## \#28 Posted by: MartyMcFly88 Posted at: 2017-11-15T17:29:06.903Z Reads: 23

```
ah okay, that makes sense, yes the antispark should always be the first one to break the circuit and the last one to complete it. 
I didn't know that the vesc shouldn't be connected while charging, thanks for that, now the position of the antispark between battery and vesc would make sense, althoug i could use the xt60 connector at the top to charge. Unplug vesc, plug into charger, then reconnect antispark .. might be too much of a hassle :P I will think about it some more.

any thoughts on why nearly everyone arranges their batteries crosswise and not lengthwise?
```

---
## \#29 Posted by: Hummie Posted at: 2017-11-15T17:41:04.777Z Reads: 21

```
people arrange their batteries for no good reason other than to fit.

and you cant charge through the esc I believe so your antispark, if thats what you also plan to charge through, would need to be at the end of the battery right people?
```

---
## \#30 Posted by: MartyMcFly88 Posted at: 2017-11-15T17:47:37.132Z Reads: 22

```
No i said unplug the vesc and plug the charger into that xt60 switch, then the vesc would be disconnected. Then plug in antispark to close the circuit.Theoretically this should work .. its just a question on wheather I want to do that much plugging everytime i charge...
```

---
