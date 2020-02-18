# First ride! (yayyy) Loop key problems! (noooo)

### Replies: 19 Views: 914

## \#1 Posted by: High-roller Posted at: 2018-01-09T11:00:53.973Z Reads: 209

```
Finally took my board out for a test spin- worked like a charm! Everything seemed to be just fine, I spent about an hour just riding around the parking lot. Once or twice I thought I smelled burning plastic, but I couldn't see any damage when I looked so I figured it was something other than my board.
When I was done I tried to pull the loop key only to find it stuck, and my first attempts to remove it did nothing. 
Getting it home and carefully opening the enclosure and disconnecting the battery, I got a better look at the underside of the key:
<img src="/uploads/db1493/original/3X/9/6/969fb66b838ed9f466a1d1bb8fa750f0b326bd32.jpg" width="375" height="499">

That wouldn't be a burned resistor would it? At the moment the key is still lodged in there, I think it must have fused with the melting plastic.
There doesn't appear to be any other damage, so I'm hoping I can just replace that part:
<img src="/uploads/db1493/original/3X/d/4/d42605c15554e15d3a981ee6511bf6c4465696ec.jpg" width="375" height="499">
Could my wiring have anything to do with it? I'm using what I think is about 16awg, but it's unmarked:
<img src="/uploads/db1493/original/3X/7/5/756d7da3142cad6d7e858ae9148293acb3c27487.jpg" width="375" height="499">
I'm planning to do a full build log soon but I want to get this straightened out first. Thanks!
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2018-01-09T11:05:24.986Z Reads: 204

```
The only time I've seen a loopkey/ antispark connector get hot is when it's not fully seated.  Is there a chance that the 3D printed cover is preventing it from being fully inserted?
```

---
## \#3 Posted by: High-roller Posted at: 2018-01-09T11:12:34.171Z Reads: 203

```
Possibly... there's a 1mm lip around the opening to prevent plug housing from coming out when I pull the key. I can't tell without taking it apart if that was too much. If so I guess I'll remove the lip and glue it down next time.
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2018-01-09T11:18:55.785Z Reads: 194

```
1mm doesn't seem like enough to cause that, but it might. Glad you're board is up and running. Hope the loop key is an easy fix for you.
```

---
## \#5 Posted by: High-roller Posted at: 2018-01-09T11:23:54.732Z Reads: 186

```
Thanks! I wouldn't have thought so either, but apparently not. It just goes to show that even the smallest details matter.
```

---
## \#6 Posted by: JonathanLau1983 Posted at: 2018-01-09T11:50:20.931Z Reads: 171

```
If I'm not mistaken the anti spark connector has a built in resistor, it sounds like this could be getting really hot because the connectors not seated correctly so all current is going through it.
```

---
## \#7 Posted by: laurnts Posted at: 2018-01-09T12:21:37.252Z Reads: 163

```
Theres definitely a gap between the xt90 female and male. The resistor can be quite hot if there is no cable attached and would definitely be untouchable. I think the vibrations of your board makes those antiloop not perfectly inserted. If the resistor broke, you will always get the huge spark.
```

---
## \#8 Posted by: High-roller Posted at: 2018-01-09T13:54:20.941Z Reads: 141

```
Thanks, that's good to know. So I think I've gotten lucky and not had any sparks, mainly because I couldn't even disconnect it. I disconnected the battery from the loop key circuit and I'll fix that before I hook everything back up again.
```

---
## \#9 Posted by: rojitor Posted at: 2018-01-09T14:09:16.346Z Reads: 142

```
Small gaps between contacts create arcs and therefore heat and burning. 
I bet that was the issue
```

---
## \#10 Posted by: GrecoMan Posted at: 2018-01-09T14:10:19.064Z Reads: 138

```
yea, plastic probably melted together nicely, take an xacto knife and cut the connectors apart (batteries UNPLUGGED)
```

---
## \#11 Posted by: Nordle Posted at: 2018-01-09T14:45:42.506Z Reads: 120

```
Is this 12awg wire or better? Cause this looks like speaker wire to me.. you probably build a portable radiator
```

---
## \#12 Posted by: High-roller Posted at: 2018-01-09T15:14:45.771Z Reads: 111

```
I think it's 16awg, as it's just slightly thinner than the vesc wires, and those are marked as being 14awg. You think I should go for 12? Thicker?
The loop key itself is the only part that seems to have heated up.
```

---
## \#13 Posted by: Nordle Posted at: 2018-01-09T17:53:57.812Z Reads: 94

```
Depends on voltage, but you say vesc so max 12S for that i would recommend 10awg wire, for 6S builds maybe even thicker.
```

---
## \#14 Posted by: anorak234 Posted at: 2018-01-10T00:17:53.173Z Reads: 88

```
Here's another thought: the wire you ran through your XT90 might be too long. That creates extra resistance, and therefore more heat which will definitely melt on 16awg wire after a little while. Make the bridge as short as possible...
```

---
## \#15 Posted by: scepterr Posted at: 2018-01-10T00:50:46.789Z Reads: 77

```
You need high strand wire, that doesn't look like it, I can't really tell from the pics
```

---
## \#16 Posted by: lowGuido Posted at: 2018-01-10T01:57:06.711Z Reads: 72

```
You can clearly see in the picture that you didnt insert it properly.  That is why the resistor fryed.
```

---
## \#17 Posted by: High-roller Posted at: 2018-01-10T06:00:14.945Z Reads: 57

```
Okay, so with my battery being 10s (36v) is 12awg enough or should I go straight to 10awg? 
Definitely agree about keeping the wires short though.
```

---
## \#18 Posted by: i2oadsweepei2 Posted at: 2018-01-10T15:05:34.479Z Reads: 44

```
I would say 12 is enough. 10 allows for a lot of headroom and is bulkier too. when I built my battery I used 10g for discharge and 12g for charging because I like headroom.
```

---
## \#19 Posted by: GrecoMan Posted at: 2018-01-10T15:07:45.400Z Reads: 46

```
i honestly don’t think it was the wire.  yes 16awg is too small.  but I used long ass 16awg on my first loopkey without issues. the key wasn’t plugged all the way in, all current went through the resistor, resistor heated up, melted they connectors together
```

---
