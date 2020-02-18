# Hub motors vibrating but not spinning

### Replies: 12 Views: 943

## \#1 Posted by: packable Posted at: 2017-12-30T13:56:15.927Z Reads: 112

```

Hi Guys, 

Eskate newbie here looking for some help.

A friend gifted me a broken, but essentially brand new Chinese board (hub motor). The speed controller board was broken but everything else is in great shape.

I thought I would essentially be able to order any duel hub ESC online, plug it in and be good to go. Probably a stupid assumption I now realise.

I ordered a new ESC from the meepo guys. The original board is not a meepo but the ESC looked pretty much identical.

Below I have added a video of whats happening now that its all plugged in. Once I hit the throttle I get movement but it essentially just vibrates, not spinning.

I know there isn’t a lot to go on but any help would be really appreciated. Is there any way to get this thing going using this new ESC or did I simply order the wrong kind of ESC?

[https://youtu.be/FOPHxs8KFgo](https://youtu.be/FOPHxs8KFgo)
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-12-30T14:09:53.158Z Reads: 108

```
check all phase wires.
```

---
## \#3 Posted by: packable Posted at: 2017-12-31T02:37:15.911Z Reads: 78

```
[quote="GrecoMan, post:2, topic:42300"]
phase wires
[/quote]


phase wires seem fine
```

---
## \#4 Posted by: Namasaki Posted at: 2017-12-31T04:07:40.165Z Reads: 70

```
Check the solder connections of the phase wires. That's where the problem will most likely be.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-12-31T04:09:56.993Z Reads: 66

```
What brand/type of esc is that?
```

---
## \#6 Posted by: packable Posted at: 2017-12-31T04:16:54.309Z Reads: 62

```
Cheers, checking connections again now

The ESC is from meepo boards: https://meepoboard.com/collections/parts-accessories/products/electronic-speed-controller
```

---
## \#7 Posted by: Namasaki Posted at: 2017-12-31T04:19:40.245Z Reads: 61

```
<img src="/uploads/db1493/original/3X/7/c/7c871fa1938c3537222c8be79ced78490818434b.png" width="487" height="120">

Looks like you have to move the motors to turn the esc on ?
I never heard of an esc like that before.
```

---
## \#8 Posted by: packable Posted at: 2017-12-31T04:46:13.640Z Reads: 52

```
The solder connection looks pretty good where they connect to the board. No solder on the connector side just crimp on bullet connectors on both sides. I can add solder also to rule that out but the crimp looks quite solid.

Not sure about the roll so turn on thing. Surely thats just an option, Ill give it a go. Thanks for the help.
```

---
## \#9 Posted by: packable Posted at: 2017-12-31T05:27:58.111Z Reads: 51

```
The spin to power on thing works. Kinda cool. but still no dice with getting the motors to spin.

https://youtu.be/umBeFjwnRwk
```

---
## \#10 Posted by: goldrabe Posted at: 2017-12-31T12:01:09.758Z Reads: 46

```
Did you try to cross swap the hall sensor wires?
Maybe that will get your hubs spinning the right way.
```

---
## \#11 Posted by: packable Posted at: 2017-12-31T15:00:06.488Z Reads: 41

```
Mate that did it! I can't believe I didn't think to try that earlier. Thanks a bunch.

https://youtu.be/m_rLg3mFQSw
```

---
## \#12 Posted by: packable Posted at: 2018-01-01T14:15:03.572Z Reads: 23

```
Update: Things seem to kind of work with the hall sensor wires swapped but it does have an annoying habit of not knowing which way to go when at the start.

When running with the hall sensor wires unplugged however everything seems just perfect. Is there anything wrong with just not using the sensors in a hub motor setup like this?
```

---
