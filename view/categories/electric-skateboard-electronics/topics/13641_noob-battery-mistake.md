# Noob Battery Mistake!

### Replies: 21 Views: 1540

## \#1 Posted by: darkkevind Posted at: 2016-11-25T13:25:13.312Z Reads: 131

```
Hi Guys,
I'm running two 3s 11.1v 5000mah batteries in serial, and for the first part I was charging each one individually, because I don't yet have a 2 x 3s > 6s balance lead adapter, then I got lazy and just started charging it in series with no balance leads! Now both my middle sells are at 0.00v and they won't charge up! Is there anything I can do or are they a gonner?

Thanks for your help. I think I've learnt a valuable lesson here :disappointed:
```

---
## \#2 Posted by: Maxid Posted at: 2016-11-25T13:48:44.133Z Reads: 127

```
0.00V seems not right. You are sure your measurements are correct? How did you measure them?
```

---
## \#3 Posted by: darkkevind Posted at: 2016-11-25T13:50:49.638Z Reads: 125

```
<img src="/uploads/db1493/original/3X/a/9/a95ccdfb87bddba9f2e77cd3c8cf91455f967846.jpg" width="690" height="388">

:frowning:
```

---
## \#4 Posted by: Maxid Posted at: 2016-11-25T13:59:47.105Z Reads: 117

```
can you measure with a multimeter? When you charged them was your total voltage correct? I mean if you charged a 6S battery to 25.2V and now the cells are 2.91 0 and 3.67 there must be something weird going on.
```

---
## \#5 Posted by: darkkevind Posted at: 2016-11-25T14:02:26.278Z Reads: 115

```
Not without dismantling the battery, which at this early stage I don't really want to do. I may do though because I may dismantle both my packs and salvage what I do have left with some others and make a bigger pack.

Oh, did I mention that BOTH 3s 11.1v packs that I'm using are like this? Both middle cells are at 0v :frowning:

>  I mean if you charged a 6S battery to 25.2V and now the cells are 2.91 0 and 3.67 there must be something weird going on.

You're right, I'm sure when I took them off charge before they were at the correct voltage! Something fishy's going on here. Do you think maybe (and it would be a massive coincidence) that both middle cell balance leads have become unsoldered?
```

---
## \#6 Posted by: Maxid Posted at: 2016-11-25T14:04:07.110Z Reads: 102

```
how can you hook them up but not measure with a multimeter? You just need to measure the pins of the balance wires.
```

---
## \#7 Posted by: darkkevind Posted at: 2016-11-25T14:05:13.192Z Reads: 98

```
Oh! I see, sorry, I misunderstood. I'll give that a go...
```

---
## \#8 Posted by: TarzanHBK Posted at: 2016-11-25T14:06:26.173Z Reads: 97

```
there´s definitely something wrong with this. Both cells at the same lvl is like winning a lottery (i mean by chances - don´t get me wrong here :D ) hope you didn´t won the lottery :D
```

---
## \#9 Posted by: Maxid Posted at: 2016-11-25T14:07:18.336Z Reads: 100

```
[quote="darkkevind, post:5, topic:13641, full:true"]
You're right, I'm sure when I took them off charge before they were at the correct voltage! Something fishy's going on here. Do you think maybe (and it would be a massive coincidence) that both middle cell balance leads have become unsoldered?
[/quote]

I also wonder how the third cell can be detected as 3.67 when its ground level (the second cell) is desoldered.
You should measure total pack voltage with a multimeter and the single cell voltages. If they add up to the total then your second cell is probably toast - otherwise there is something wrong with your balance wires.
```

---
## \#10 Posted by: darkkevind Posted at: 2016-11-25T14:08:17.940Z Reads: 93

```
OK, this is weird, I just checked with a multi-meter, and all three cells are showing 4.08v (as I just fully charged one pack)!

You think my iMAX is playing up?
```

---
## \#11 Posted by: Maxid Posted at: 2016-11-25T14:09:28.523Z Reads: 88

```
Check if your balance cable is inserted correctly and fully in the charger. You might just have had a loose connection.
```

---
## \#12 Posted by: TarzanHBK Posted at: 2016-11-25T14:10:29.975Z Reads: 86

```
these numbers sounds more realistic to me.
yep check you balance cables and the connection to your imax
```

---
## \#13 Posted by: darkkevind Posted at: 2016-11-25T14:11:13.445Z Reads: 85

```
Yep, all fully in there...  I just checked the pack at the XT60 connector and it's coming up at 12.22v which is right...right?
```

---
## \#14 Posted by: Maxid Posted at: 2016-11-25T14:12:07.999Z Reads: 84

```
As long as they are 4.08V they should be perfectly fine. 12.2V for a 3S pack is also fine. I am just not sure why your charger is showing those weird values. maybe check the charger's balancer pins for corrosion or dust or something.
```

---
## \#15 Posted by: darkkevind Posted at: 2016-11-25T14:12:44.267Z Reads: 85

```
I think my iMAX might be up the swanney as it's getting VERY hot! Which it didn't do when I first got it...

Does anyone else's get hot when charging 3s?
```

---
## \#16 Posted by: Maxid Posted at: 2016-11-25T14:14:41.395Z Reads: 80

```
Temperature should depend on charge current. at something moderate (like 2A) it should not get too hot. You might have shorted something.
--> I'd get a new (quality) charger. Hobbyking's Reaktor series is supposed to be good for example.
```

---
## \#17 Posted by: darkkevind Posted at: 2016-11-25T14:18:20.501Z Reads: 80

```
OK it's definitely that my charger (iMAX B6AC) is faulty, the other pack just came off charge and that too is at 12.4v, even though the balance display was as above! I just checked each cell via the balance lead and they're all around 4.08v.

OK, so It looks like I can still used the charger, if I don't mind it getting a little hot, and don't rely on the display!! :disappointed:

Not good, it's not very old at all. Less than a month!
```

---
## \#18 Posted by: darkkevind Posted at: 2016-11-25T14:19:32.213Z Reads: 72

```
Thanks all for your help, at least it's not my batteries! Phew!!! :flushed:
```

---
## \#19 Posted by: Maxid Posted at: 2016-11-25T14:27:55.235Z Reads: 75

```
Be careful with a broken charger. We don't know what else it will do wrong (overvoltage for example).
Lipos are dangerous and can burn your house down.
```

---
## \#20 Posted by: darkkevind Posted at: 2016-11-25T14:29:57.765Z Reads: 76

```
Good point. I won't ever leave it charging unattended. If I can get more life out of it before blowing up one or more of the batteries, then all's good. However, come payday I'll order another charger. Maybe that HobbyKing one...:+1:
```

---
## \#21 Posted by: B4Me Posted at: 2016-11-26T00:50:21.564Z Reads: 47

```
Try opening the charger up.. and check if one of the pins for balancing leads, are loose, maybe just a bad solder joint
```

---
