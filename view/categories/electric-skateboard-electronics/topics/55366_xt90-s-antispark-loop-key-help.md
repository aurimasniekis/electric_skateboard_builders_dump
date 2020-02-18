# XT90-S Antispark Loop key help

### Replies: 28 Views: 1050

## \#1 Posted by: TSThunder Posted at: 2018-05-14T02:21:23.881Z Reads: 227

```
Hey guys, so I have become tired of plugging the batteries directly into my VESC, so I have committed to creating an anti spark loop key, but I have a few questions. I made a picture for reference.
-Is there any problems I would encounter if I were to do it this way?
-Do I buy the XT90, or the XT90-S?
-Any links to find some cheap XT90-S or XT90 connectors

appreciate any help!

![layout|690x388](upload://54zWxzwlSBx4y972tGvBVqf3jiL.png)

Also, check out this video by Big Kids and share it for a chance of winning some cool wheels --> https://www.google.com/url?q=https://www.youtube.com/watch?v%3D2M3J8B5H3Go&sa=D&ust=1526267839300000&usg=AFQjCNGwWuFRXSHJLa9g_aMDXSXb1jKyHQ
```

---
## \#2 Posted by: RedEagle Posted at: 2018-05-14T02:28:56.094Z Reads: 210

```
Diagram looks good. You need a xt90-s. I've got some.
```

---
## \#3 Posted by: TSThunder Posted at: 2018-05-14T02:30:12.650Z Reads: 206

```
Got a link? Also, will the length of my wiring effect anything?
```

---
## \#4 Posted by: RedEagle Posted at: 2018-05-14T02:32:13.183Z Reads: 202

```
If your wires are longer than 30cm you'll risk failures due to ripple current. 

https://www.electric-skateboard.builders/t/new-vescs-remotes-bmss-chargers-and-more-for-sale-eu-only/31643/
```

---
## \#5 Posted by: TSThunder Posted at: 2018-05-14T02:37:26.344Z Reads: 191

```
And putting the antispark on the negative side is safe?
```

---
## \#6 Posted by: RedEagle Posted at: 2018-05-14T02:39:17.184Z Reads: 185

```
Yes. It doesn't matter which side it is but many of us put it on the positive side.
```

---
## \#7 Posted by: TSThunder Posted at: 2018-05-14T02:40:34.786Z Reads: 180

```
Ok. Do you have a ling for some cheap xt90-s connectors? I am looking to make my own.
```

---
## \#8 Posted by: RedEagle Posted at: 2018-05-14T02:41:55.893Z Reads: 177

```
You can try hobbyking. They should have some.
```

---
## \#9 Posted by: TSThunder Posted at: 2018-05-14T02:46:38.971Z Reads: 173

```
You can make it with these right? https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html
```

---
## \#10 Posted by: MysticalDork Posted at: 2018-05-14T02:48:08.830Z Reads: 167

```
Yes, it's literally just one of those with the terminals bridged.
```

---
## \#11 Posted by: RedEagle Posted at: 2018-05-14T02:48:50.809Z Reads: 168

```
[quote="MysticalDork, post:10, topic:55366, full:true"]
Yes, it’s literally just one of those with the terminals bridged
[/quote]

What he said.
```

---
## \#12 Posted by: TSThunder Posted at: 2018-05-14T02:50:28.634Z Reads: 158

```
Sorry for being such a noob. One last question. Does it matter whether which sides the wires are soldered on?
```

---
## \#13 Posted by: TSThunder Posted at: 2018-05-14T02:52:21.099Z Reads: 160

```
(male/female)
```

---
## \#14 Posted by: RedEagle Posted at: 2018-05-14T02:52:37.045Z Reads: 157

```
No, but it's advisable to have the connector with the green mark soldered on the board. That's the one with the resistor. If you lose it it's game over and hello sparks.
```

---
## \#15 Posted by: MysticalDork Posted at: 2018-05-14T02:56:13.571Z Reads: 159

```
I beg to differ with @RedEagle, since the anti-spark part can fail on rare occasions, it's better for it to be in the "key" rather than in the board, that way if it ever fails, you can just replace it.
```

---
## \#16 Posted by: mmaner Posted at: 2018-05-14T02:57:57.535Z Reads: 159

```
@MysticalDork is right, use the resistor side as the key. Also, it's better to do it in the positive leg.
```

---
## \#17 Posted by: MysticalDork Posted at: 2018-05-14T02:58:58.845Z Reads: 155

```
And you can get them on Amazon too, if you don't want to wait for hobbyking shipping. https://smile.amazon.com/XT90-S-Connector-housing-Li-poly-Battery/dp/B06XW63S87/
```

---
## \#18 Posted by: TSThunder Posted at: 2018-05-14T03:23:40.795Z Reads: 148

```
Ok. Great tips. I ordered some wire and the xt90-S'  thank you all
```

---
## \#19 Posted by: Lionpuncher Posted at: 2018-05-14T03:40:50.642Z Reads: 143

```
Hey bro, why is it better on the positive side?
```

---
## \#20 Posted by: mmaner Posted at: 2018-05-14T04:02:36.203Z Reads: 143

```
If it's in the negative side and you get a short without the loop key the negative side could still active as a ground and them the amps flownon the positive.
```

---
## \#21 Posted by: Lionpuncher Posted at: 2018-05-14T15:17:24.114Z Reads: 120

```
 Ahhh that totally makes sense. So cut off from the source and prevent ALL issues as opposed to just MOST issues. Thank you.
```

---
## \#22 Posted by: amazingdave Posted at: 2018-05-14T17:40:41.823Z Reads: 109

```
I’m of the opinion that accidental shorting the connection is far more likely if you use the resistor side for the key... 

may well not cause any issues but I went the other way round to be safe...
```

---
## \#23 Posted by: mmaner Posted at: 2018-05-14T19:15:10.631Z Reads: 104

```
I don't see how, but it's all good. We are all just trying to figure out how to make mountains out of hills around here 😀
```

---
## \#24 Posted by: amazingdave Posted at: 2018-05-14T19:50:21.440Z Reads: 99

```
Just because you end up with the male pins as live rather than the female sockets... I know if they short it’s only connecting the power to the VESC but the little arc when the caps charge bothered me! 

But as you say we’re all just rolling along!
```

---
## \#25 Posted by: TSThunder Posted at: 2018-05-14T21:27:27.513Z Reads: 93

```
I am confused now. Should I use the resistor side for the "key" or but it on the board?
```

---
## \#26 Posted by: mmaner Posted at: 2018-05-14T21:57:53.505Z Reads: 91

```
I use the resistor side for the key.  If you use on the board side and it fails, you have to tear into the board and rework the soldering.  If you use it as the key, the worst that can happen is you lose it, but I keep spares.

Some people are worried about shorting the pins if you use the male board side, but I'e never seen it happen and cant see how it would.  

Do whatever you want though, whatever makes you feel safest.
```

---
## \#27 Posted by: Slak Posted at: 2018-05-15T10:11:15.256Z Reads: 82

```
Diagram does not look good because there is no fuse in this setup ! :frowning:

For the rest, I use the resistor side as key and my Anti-Spark is on negative wire and my fuse is on positive wire.
```

---
## \#28 Posted by: TSThunder Posted at: 2018-05-15T22:06:29.329Z Reads: 70

```
What is this "fuse" you talk about?
```

---
