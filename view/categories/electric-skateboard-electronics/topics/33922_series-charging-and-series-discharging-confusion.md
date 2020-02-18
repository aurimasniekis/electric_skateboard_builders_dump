# Series charging AND series discharging confusion

### Replies: 16 Views: 788

## \#1 Posted by: fraannk Posted at: 2017-09-25T12:03:34.807Z Reads: 71

```
Hi. So I have a 8s charger and would like to charge my board with a vga port and a xt90 or xt60 port. 
I drew this diagram:
<img src="/uploads/db1493/original/3X/9/e/9eca4f15eb27e4f2faf52d14ac6572041007533f.jpeg" width="690" height="186">
I’m confused about two things. A lot of guides on the internet says that it is recommended to connect the leads as shown in the green circle. However others also state that the black wire is not needed. What should I do and why? 

The other thing is that something tells me, that when I then discharge, the current could go from one battery to the other as it should in the blue circle (black wire). But could it also go through the balance connector since these now are connected in series? 

Thanks, I hope you understand, 
Lmk if you have any questions.
```

---
## \#2 Posted by: fraannk Posted at: 2017-09-25T12:40:36.677Z Reads: 62

```
For example:
This guide shows to connect all of them: http://www.tjinguytech.com/charging-how-tos/serial-charging
This guide shows that you should remove the red wire: http://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122 (further down @Namasaki says to remove the black wires and not the red :sweat_smile:) 
And @jmasta told me to remove the black wire. http://www.electric-skateboard.builders/t/10s-balance-connector-series-harness/33051/4

Thanks, just trying to make sure I do this right.
```

---
## \#3 Posted by: raven Posted at: 2017-09-25T12:46:41.817Z Reads: 55

```
Make sure the battery is not overcharged. Lipos are sensitive babies
```

---
## \#4 Posted by: fraannk Posted at: 2017-09-25T12:48:16.681Z Reads: 53

```
I use a up-to-10s balance charger, so that should take care of that for me. I just want to know the correct/optimal way of wiring the balance connectors :)
```

---
## \#5 Posted by: SilentException Posted at: 2017-09-25T13:05:13.417Z Reads: 52

```
I hope you aren't planning to connect like in your diagram. 
If the red wire on the balance leads means V+ you will create a short. You connect main leads from upper pack over V- to lower pack V+ and connect balance other way around. Ouch, big bang and melted wire.
```

---
## \#6 Posted by: fraannk Posted at: 2017-09-25T13:07:15.092Z Reads: 49

```
So to avoid this I should do what? Switch the balance connectors? Or should I disconnect any wires? Might try re-drawing the battery-part of the diagram..
```

---
## \#7 Posted by: fraannk Posted at: 2017-09-25T13:16:12.981Z Reads: 46

```
@SilentException Is this any better? 
<img src="/uploads/db1493/original/3X/1/e/1e449dfa8f7f7662a525638958aa61aafb930854.jpeg" width="690" height="430">
```

---
## \#8 Posted by: SilentException Posted at: 2017-09-25T13:19:20.744Z Reads: 45

```
Much better indeed. You don't need one of the middle balance wires because they are already connected over main leads. Doesn't hurt to have though.
```

---
## \#9 Posted by: fraannk Posted at: 2017-09-25T13:23:21.901Z Reads: 45

```
So I would be able to cut one of those two wires in the blue circle? And it would still balance perfectly? <img src="/uploads/db1493/original/3X/9/1/913bd2f8a8b1bb427b324caab8db7d1d25690108.jpeg" width="690" height="472">
And would it be possible in any way for the current to go through the balance connectors if I do not remove any of the wires? They surely won’t be able to handle that kind of current if possible. 
Thanks, appreciate it!
```

---
## \#10 Posted by: SilentException Posted at: 2017-09-25T13:27:19.127Z Reads: 40

```
Yes, it would balance over main black lead going from top - to bottom +. If you planning on disconnecting that one when balancing, leave both wires in the blue circle as is. It doesn't hurt to have them either way.

Current to go over what to where and when? I mean, try to think about it first. You will perhaps see that the question doesn't make much sense, at least in this form :)
```

---
## \#11 Posted by: fraannk Posted at: 2017-09-25T13:34:47.861Z Reads: 36

```
Forget the current thing, I think i figured that out. :) 
So removing either one of the wires in the blue circle, just removes one of the points where it's connected in series? It would still charge and balance normally as long as the XT90's is connected? 

Thanks again...
```

---
## \#12 Posted by: SilentException Posted at: 2017-09-25T13:41:37.539Z Reads: 33

```
Alright, I thought you might figure that one out yourself :slight_smile:
 
Yes, double connection, once over balance leads, once over the XT90 series plugs.
```

---
## \#13 Posted by: fraannk Posted at: 2017-09-25T13:42:14.794Z Reads: 34

```
Nice, thanks! Problem solved then. Let's see if I fry some connectors ;)
```

---
## \#14 Posted by: Emerson Posted at: 2017-09-25T13:54:30.534Z Reads: 30

```
Out of curiosity, wouldn't connecting these wires together put them in parallel?  As such the voltage wouldn't be altered so it would technically still work as intended I believe.  If it was me though I would remove one of them just because both aren't needed.  They both hold the same value for balancing charging so removing one makes things easier.
```

---
## \#15 Posted by: jmasta Posted at: 2017-09-25T14:07:31.424Z Reads: 34

```
[quote="SilentException, post:8, topic:33922, full:true"]
You don't need one of the middle balance wires because they are already connected over main leads. Doesn't hurt to have though.
[/quote]

That's the thing though.  It actually can "hurt to have" the redundant middle balance wire

I can't tell you how many fried lipo balance wires I have seen on here because of this very issue

If you hook everything up correctly, it doesn't matter. However if you hook up the mains as A+B, and then plug in the balance plugs unknowingly as B+A, you will instantly short out a battery.  Boom. Charred connector in your hand.  Cutting the middle balance wire removes this possibility.  Then the worst thing that happens is your balance charger gives you an error
```

---
## \#16 Posted by: SilentException Posted at: 2017-09-25T14:08:50.506Z Reads: 31

```
Yes, well aware of that. But in this case it's a static connection to the VGA plug, that's why I didn't complicate with explanation for that "use case".
```

---
