# Help needed with Lipo Balance Cable

### Replies: 21 Views: 1019

## \#1 Posted by: r_chung Posted at: 2018-02-03T17:02:05.672Z Reads: 90

```
Hey,
I am planing to charge my 6S battery in a way so I don't need to take out the battery to charge and just plug the charger into the board. 
Similar to this: http://www.electric-skateboard.builders/t/guide-how-to-charge-lipo-batteries-without-removing-them-from-the-board/34254/3

I also wanted a voltage readout like this: https://hobbyking.com/en_us/hobbykingtm-lipo-voltage-checker-2s-8s.html, so I can read the battery levels when I'm riding.

But from what I've read. It's best to connect the balance cable from the battery into the charger. And since there's only one balance cable from the battery, is there a way I can just plug in the balance charger into the battery as well as having a voltage monitor with needing to take out any electronics. 
Thanks
```

---
## \#2 Posted by: LAVAMAN Posted at: 2018-02-03T17:08:37.062Z Reads: 79

```
I have a 6S battery (3 x 2S LIPO) and I charge it without removing from the enclosure. Please see wiring diagram and photo attached.![BALANCE_PORT_WIRING_REVISED|644x485](upload://Ao9p5zT2zs4SGMFrrpGcRwDSDgr.jpg)![FIRST BUILD BOTTOM|690x414](upload://kYAEj7005doe79Y7DzbZSDRg8JE.jpg)
```

---
## \#3 Posted by: r_chung Posted at: 2018-02-03T17:11:19.477Z Reads: 72

```
Hi, 
Thanks for the reply.
Does your board have a voltage monitor? Because I'm unsure how to plug in the balance cable into both the charger and the voltage monitor at the same time when I charge it.
```

---
## \#4 Posted by: LAVAMAN Posted at: 2018-02-03T17:25:55.379Z Reads: 67

```
I do not use one currently, but it is not hard to wire into your setup. Do a search and you should find how to integrate into your wiring diagram. I am not an electronics person and so the experienced guys on this forum helped me with my wiring and sent me the diagram I attached. Works great.
```

---
## \#5 Posted by: r_chung Posted at: 2018-02-03T17:26:56.634Z Reads: 69

```
Alright, thanks I'll see what I can do.
```

---
## \#6 Posted by: krloz Posted at: 2018-02-03T17:47:57.885Z Reads: 62

```
 Maybe a parallel balance cable but with 1 male connector and 2 female. 
But you can do this simply with the battery cable.  Plug the balance charger when charging and the voltage monitor when discharging.  And nothing when neither. 
That way your voltage monitor won't empty your battery
```

---
## \#7 Posted by: r_chung Posted at: 2018-02-03T20:26:36.430Z Reads: 53

```
Oh something like this: http://www.nexusmodels.co.uk/jst-xh-parallel-adapter-6s.html
That would make sense actually. Thanks a lot
```

---
## \#8 Posted by: krloz Posted at: 2018-02-03T21:18:18.195Z Reads: 52

```
Actually no
The opposite.  That one has two males one female, to connect two batteries in parallel to a same charger.  You need one with two females and one male. Which is harder to find and probably easier to make if you know your soldering
```

---
## \#9 Posted by: r_chung Posted at: 2018-02-03T22:36:27.109Z Reads: 49

```
I'm only using a single 6S lipo battery though so it should be OK right.
```

---
## \#10 Posted by: krloz Posted at: 2018-02-03T22:42:01.489Z Reads: 42

```
I didn't explain my self properly. 
The one you post links 2 batteries to one bms or cell monitor. 
You want one that links a single battery to two bms or cell monitor.
That is 2 input one out. You want 1 input 2 outputs
```

---
## \#11 Posted by: pat.speed Posted at: 2018-02-03T23:02:46.407Z Reads: 38

```
He needs one female to a double male connector
```

---
## \#12 Posted by: r_chung Posted at: 2018-02-03T23:19:14.381Z Reads: 38

```
Yh I just realised my bad. Does anyone sell them or do I need to make my own.
```

---
## \#13 Posted by: krloz Posted at: 2018-02-03T23:35:26.645Z Reads: 33

```
Nope. Male is the one that connects to battery.  Female is the one that connects to bms or monitor.  So wanting to connect a single battery to a bms and a monitor he needs one male and two females
```

---
## \#14 Posted by: krloz Posted at: 2018-02-03T23:36:31.173Z Reads: 34

```
@r_chung
 [quote="krloz, post:8, topic:45468"]
Which is harder to find and probably easier to make if you know your soldering
[/quote]

Make one or get somebody to make one.  Or search, like, a lot
```

---
## \#15 Posted by: r_chung Posted at: 2018-02-04T00:34:42.493Z Reads: 31

```
Yh alright. I mean I can solder but if its just easier buying one and would probably look better. But thanks a lot anyway.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-02-04T06:47:47.467Z Reads: 31

```
Um no, your wrong... this is a male connector ![image|375x500](upload://rp9F4v82IDxBA1Z1xEfSZZhwm5a.jpg)

And the battery already has a male connector so he will need a female that connects to the battery. Read brother, read, read, read
```

---
## \#17 Posted by: Ishayc Posted at: 2018-02-04T07:03:13.424Z Reads: 28

```
This is a female connector.
From what I've seen so far, all balance chargers have male connectors which means that the batteries have female ones.
```

---
## \#18 Posted by: krloz Posted at: 2018-02-04T10:39:50.725Z Reads: 23

```
I have read man, lots.  And go have look at some primary school biology dude. Male is the one with the pipi hanging out and female is the one with the hole you put the pipi in, as long as she totally agrees. "Brother"
```

---
## \#19 Posted by: pat.speed Posted at: 2018-02-04T11:15:20.752Z Reads: 20

```
Sorry I was meaning as in the plug shape. (The plastic bit) didn't realise you were talking about the pins and sockets
```

---
## \#20 Posted by: krloz Posted at: 2018-02-04T11:18:55.465Z Reads: 18

```
Actually I have been trying to find a photo with a single jstxh connector That clearly states its gender and from a trusty source.  And I haven't been able, so it seems understandable people are getting them mixed up as they are more referred to as battery side...
Anyway as I understand connectors are always referred to considering whether the connection part (metal, not housing) resembles what I explained.  
Oh and sorry if it sounded childish, or mockery...i kind of learned it that way, way long ago.
```

---
## \#21 Posted by: pat.speed Posted at: 2018-02-04T11:30:33.531Z Reads: 19

```
As reliable as it gets. Lol

![IMG_1149|384x384](upload://1kT932Sizw2JpAnFKRet9VtBAiW.JPG)


I'll put this in the just pics thread too, to clarify if anyone else though like I was
```

---
