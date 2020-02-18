# Balance cable shorted when charging 2x3s lipos in series

### Replies: 11 Views: 1033

## \#1 Posted by: Armitage Posted at: 2017-10-03T15:20:23.135Z Reads: 78

```
Hey, I have a little problem. I was connecting my two 3s 5800mAh Zippy batteries in series to charge them on 6s charger. 

I connected the Balance leads wrongly together, leaving the positive side on the negative side and the positive on the negative side of battery. When I connected power leads, the balance cables shorted out for a 0.5 second. Could this cause any damage? I used someones schematic and showed what i plugged wrong. Credits to whos schematic this is

<img src="/uploads/db1493/original/3X/9/9/99a1e568a644757aa6316c6241a331117245fad0.png" width="690" height="489">
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-10-03T15:25:34.376Z Reads: 70

```
yeah u have to disconnect one of the black wire in balance, I vaporized entire connector before, but works fine. it sort of acted like a fuse so.

a lot of smoke too but yeah. It will still work no worries.
```

---
## \#3 Posted by: Armitage Posted at: 2017-10-03T15:29:44.547Z Reads: 67

```
Yes, but later I tried the way on the original schematic and it didn't short out. What exactly do i need to disconnect? Thanks
```

---
## \#4 Posted by: SilentException Posted at: 2017-10-03T15:34:41.025Z Reads: 65

```
You don't need to disconnect anything. You had it wrong, it shorted, now you have it correct. If your balance wires are okay and not destroyed due to short, everything's good. The cells might have suffered some internal damage but they'll survive :)

onepunchboard is probably talking about not needing to have both middle balance wires connected to the main balance plug. You can have one or the other, it'll work just as well as long as the mains leads are connected in series.
```

---
## \#5 Posted by: Armitage Posted at: 2017-10-03T15:40:42.773Z Reads: 59

```
Okay, thanks for help :slight_smile:
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-10-03T16:25:49.243Z Reads: 53

```
oh srry i thought it as for parallel charging. should've read through haha, it sould be fine,
but if u connect the balance like that and do parallel, it will have very big flash :slight_smile:
```

---
## \#7 Posted by: Armitage Posted at: 2017-10-03T16:46:05.547Z Reads: 47

```
No no, I am charging it in series on the board without taking it out from it.
```

---
## \#8 Posted by: linkedtim Posted at: 2018-02-05T18:42:43.866Z Reads: 36

```
When the balance leads are spliced like this, is it essentially configuring the batteries in series even if the 10-awg black and red cables aren't connected? I noticed that I can plug in the 10-awg red & black cable into the VESC without plugging in the final red&black cable (image w/ arrow pointing to batt1+2) to configure them in series and the boards becomes operational.  To be clear, the connections between battery 1+2 illustrated by the black cable in the original image is NOT connected, but the board is working?

  ![Series|690x489](upload://wsD6AV0uFJX9mRptNvOr0iqt3Bv.png)
```

---
## \#9 Posted by: lowGuido Posted at: 2018-02-05T20:45:27.390Z Reads: 29

```
It IS connected. 
Through the balance leads. 
Look at it this way. If you conect 2 wires from point A to point B and then you cut one of the wires.
Point A and B are still connected by the other wire.

Its probably not a good idea to leave it like that  though. The balance lead might not be able to handle all the operational current.

This is why I always recomend to cut one of the balance leads in the middle. While physically it makes no difference. It sure does confuse A LOT of people.
```

---
## \#10 Posted by: linkedtim Posted at: 2018-02-05T21:49:17.480Z Reads: 26

```
@lowGuido, your content is :fire:! I still get a spark when I connect the 10-awg wires, which I found odd b/c if they were connected prior via the balance wires I wouldn't have anticipated a spark on that additional 10-awg cable connection but I'll defer to your expertise, just caught a newb off-guard. This all started when I made an anti-spark key using a 330ohm resistor; the anti-spark was going to connect where I had highlighted in my previous image where there was a disconnect. When I went to test the anti-spark, I plugged everything in EXCEPT where referenced as 'disconnected' in my image and got that spark. Sucks because I spliced it this way in hoping I could leave that and charge two lipos at once v having to plug in additional connectors and then charge it all up
  ![IMG_4604|375x500](upload://wmhgNuk11M43faJohwx8knOyBhU.JPG)
-In your Youtube video, you cut a 6s 7-wire balance lead connector in half, plugged one half into the JST from 1 lipo and the other into the secondary lipo? do you connect/disconnect that manually before/after every charge? Lesson learned I guess, appreciate your help. Thanks for your awesome content in this community.
```

---
## \#11 Posted by: lowGuido Posted at: 2018-02-05T23:23:20.887Z Reads: 25

```
How i do it in the video is how it stays always. I don't  disconnect anything for charge.

Just make sure that your positive wire from the battery lines up with the most positive of the 2 balance leads. This is critical.
As long as all wires are lined up correctly the new lead is no different from a standard 6S lead.
```

---
