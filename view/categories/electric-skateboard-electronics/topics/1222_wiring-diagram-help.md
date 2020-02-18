# Wiring Diagram Help?

### Replies: 15 Views: 4971

## \#1 Posted by: gamma2 Posted at: 2016-02-04T08:24:25.913Z Reads: 215

```
So, I'm fairly new to working with anything about 3s and creating my own wiring harnesses. I was hoping someone would be able to sketch a quick drawing of how I need to wire my board, if its even possible at all. My goals are as follows:

 1. 2x 6s LiPos in series to make a 12s.
 2. Antispark killswitch made with an XT90s plug on the positive line.
 3. Add a [battery life display][1].
 4. Charge the batteries as if they are wired in parallel. (Is this possible??)
 5. Power VESC and GT2B Rx.

Any pointers at all would be a great help! Thanks guys!


  [1]: http://www.ebay.com/itm/LCD-Capacity-Tester-Indicator-for-12V-48V-Lead-acid-Lithium-Cell-LiPo-Battery-US/331424151150?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D35218%26meid%3D1c393d62cfa34ce3846e86018088055d%26pid%3D100005%26rk%3D4%26rkt%3D6%26sd%3D111482414278
```

---
## \#2 Posted by: lowGuido Posted at: 2016-02-04T09:09:17.044Z Reads: 210

```
I think rather than trying to charge in parallel you would be better off using 2 chargers or a double charger and charging the 2 6S simultaneously.
```

---
## \#3 Posted by: gamma2 Posted at: 2016-02-04T09:25:46.498Z Reads: 204

```
I was hoping there would be some solution for this where I wouldn't have to reinvest in another charger. I'm even willing to charge each battery separately, I'm just not sure how to wire things in such a way that I can disconnect them from eachother for charging while keeping the rest of the harness in tact.
```

---
## \#4 Posted by: lowGuido Posted at: 2016-02-04T09:31:46.860Z Reads: 198

```
Imax B6 is cheap. 
I own 4 of them I think there were about $18 each
I leave one at work and a few at home
```

---
## \#5 Posted by: gamma2 Posted at: 2016-02-04T10:00:09.575Z Reads: 200

```
Yeah I use the Imax as well, I was just trying to avoid the extra cost. I don't need a super fast charging solution. So after some more research, this is what I have come up with. Does this look like it is okay to use?<img src="/uploads/db1493/original/2X/2/26415d5d41e61104b5ae9cd8b297a3387d60dfdd.jpg" width="555" height="500">
```

---
## \#6 Posted by: lowGuido Posted at: 2016-02-04T10:32:08.234Z Reads: 197

```
you can certainly do it that way it will work.
```

---
## \#7 Posted by: Riako Posted at: 2016-02-04T12:58:49.304Z Reads: 194

```
But I read its gonna take the same time than if you charge 1 by 1 ...
Thx Gamma2 for your diagram !
I look for charge my 2 x 5s 8ah, it will be the same so (imax b6 too) ? Cause actually I charge one by one
<img src='/uploads/db1493/original/2X/5/513e6dc1efafc8d17d13a39e35180c8b51c8778b.jpg'>
https://monlongboardelectrique.wordpress.com/2016/01/15/schema-de-cablage-electrique-e-skate/
```

---
## \#8 Posted by: lowGuido Posted at: 2016-02-04T13:33:14.001Z Reads: 177

```
if you charge 1 by 1 or parallel or series it will take around the same time. (assuming you are fast with the swap)

the only way you can charge faster is to use a bigger charger with more amps.
```

---
## \#9 Posted by: trbt555 Posted at: 2016-02-04T13:48:43.529Z Reads: 175

```
Get XT60 connectors for the batteries, XT90's are HUGE.
XT90 only for loop key.

What's the use of the bullet in the middle ?
```

---
## \#10 Posted by: gamma2 Posted at: 2016-02-04T22:50:16.219Z Reads: 162

```
I read that XT90 is more suited for anything over 4 or 5s. Honestly I don't mind the size. The XT60's on my 3s LiPos are too tiny to get a good grab on them for disconnecting. The bullet is just a way of connecting them in series in a way that's easy to undo if I ever want to modify the wiring harness. The antispark loop and other connections will probably be bullets too.
```

---
## \#11 Posted by: gamma2 Posted at: 2016-02-04T22:53:14.922Z Reads: 160

```
I like the way that diagram  is laid out! It looks like they're using some kind of circuit breaker style for their on/off switch. I personally think just adding a loop key on the positive line is easier. If you wire the batteries in parallel or use a parallel balance board the B6 will charge them at the same rate as doing them one by one.
```

---
## \#12 Posted by: NNGG Posted at: 2016-02-05T04:18:02.784Z Reads: 146

```
Do you have a original IMAX or a OEM clone?
```

---
## \#13 Posted by: lowGuido Posted at: 2016-02-05T07:39:56.188Z Reads: 145

```
i have 3 original and 1 clone.
```

---
## \#14 Posted by: NNGG Posted at: 2016-02-05T07:45:18.190Z Reads: 139

```
any differences between them?
```

---
## \#15 Posted by: lowGuido Posted at: 2016-02-07T10:17:01.940Z Reads: 137

```
Hardly. The clone has silver terminals and the genuine has gold. The genuine came with better cables. Haven’t noticed any difference in charging.
```

---
