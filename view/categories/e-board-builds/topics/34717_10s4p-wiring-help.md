# 10s4p wiring help

### Replies: 22 Views: 1481

## \#1 Posted by: 12meterkuk Posted at: 2017-10-04T02:46:50.850Z Reads: 137

```
Hey everyone, I am planning out my 10s4p battery for my bamboo gt upgrade, cells are arriving in 2 days.

I have run into a problem that is the enclosure not being long enough to fit this configuration: <img src="/uploads/db1493/original/3X/8/f/8fec76939c47543bb933db2592aa59a5233324e5.png" width="188" height="500">

I do not have the tools to extend the enclosure or cnc the deck. I also don't want to squeeze the bms on top of the esc as I am afraid the heat would cause problems.

I have looked into another configuration but still not sure exactly how it is supposed to be wired: <img src="/uploads/db1493/original/3X/9/2/926511c335878e761ecfa7f353934ac0e7df6282.png" width="246" height="500">

Can anyone help out with this? I also have no idea where to solder the new balance wires for the 2nd configuration.

Thanks
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-04T03:01:01.086Z Reads: 122

```
Why not just have all cells vertically stacked?
```

---
## \#3 Posted by: 12meterkuk Posted at: 2017-10-04T03:01:36.777Z Reads: 122

```
Because the enclosure has screw holes that are in the way

<img src="/uploads/db1493/original/3X/4/5/4588e56e449860848ffaef48f4c9744b497d5299.png" width="382" height="500">
```

---
## \#4 Posted by: Jinra Posted at: 2017-10-04T03:06:56.140Z Reads: 121

```
If you don't want to downgrade to 10s3p, you can wire it like this... but it's really weird<img src="/uploads/db1493/original/3X/4/b/4b12308f4f292c71ff1087e976cdc91c55b3962a.png" width="242" height="500">
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-10-04T03:14:49.915Z Reads: 116

```
Similar to my idea. Hooray for MSPaint! <img src="/uploads/db1493/original/3X/4/9/49d06d1093aaedcaa6d9028752eca6c6924db517.png" width="246" height="500">

And yes, I did change line widths like 4 times :P
```

---
## \#6 Posted by: Jinra Posted at: 2017-10-04T03:15:26.713Z Reads: 114

```
Yours is much better... lol.

However, make sure you insulate the shit out of that, that diagram can short very easily.
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-10-04T03:16:14.246Z Reads: 116

```
it's pretty close to my current 10s4p pack, just without the rotated banks.

Yeah, mine has four layers of kapton and a layer of neoprene foam between them.

I take battery shorts **very** seriously.
```

---
## \#8 Posted by: 12meterkuk Posted at: 2017-10-04T03:19:02.751Z Reads: 116

```
Thanks for the drawings,

Is this right? <img src="/uploads/db1493/original/3X/3/c/3cfb914147833d97b4a6e666dba40b9bae91e3a6.png" width="283" height="500">

[quote="MysticalDork, post:7, topic:34717"]
Yeah, mine has four layers of kapton and a layer of neoprene foam between them.
[/quote]

Do you tape up each cell group?
```

---
## \#9 Posted by: 12meterkuk Posted at: 2017-10-04T03:21:27.227Z Reads: 109

```
[quote="MysticalDork, post:5, topic:34717"]
926511c335878e761ecfa7f353934ac0e7df6282.png282x572 9.83 KB
[/quote]

Your is like an upside down U shape. Is there any benefit to it?
```

---
## \#10 Posted by: Jinra Posted at: 2017-10-04T03:22:14.476Z Reads: 108

```
Less wire, but more chance of short. Just gotta make sure you insulate well.
```

---
## \#11 Posted by: 12meterkuk Posted at: 2017-10-04T03:22:38.359Z Reads: 105

```
Which one, mine?
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-10-04T03:22:52.123Z Reads: 104

```
That configuration lets you keep the output wires as short as possible, which helps prevent voltage spikes and noise. Yes, I insulated each cell group, then when the pack was all soldered I insulated between them again before heatshirnking it.
```

---
## \#13 Posted by: 12meterkuk Posted at: 2017-10-04T03:24:33.352Z Reads: 102

```
[quote="MysticalDork, post:12, topic:34717"]
That configuration lets you keep the output wires as short as possible
[/quote]

Ah i understand now. I will mock up each configuration with the cells before I spot weld them. Thanks for the advice @Jinra and @MysticalDork
```

---
## \#14 Posted by: Namasaki Posted at: 2017-10-07T23:10:06.670Z Reads: 81

```
@Jinra
I'm worried that this is gonna be another board on fire.
Those cells are so tight in there that the positive nickel strips are gonna be rubbing against the thin insulation of the negative cell housings. and there doesn't appear to be enough room to properly insulate the cell groups.
```

---
## \#15 Posted by: Jinra Posted at: 2017-10-07T23:18:44.791Z Reads: 84

```
Yea I noticed that too, not sure how well it'll hold up to miles and miles of vibrations
```

---
## \#16 Posted by: Namasaki Posted at: 2017-10-07T23:20:55.387Z Reads: 86

```
Like this:

<img src="/uploads/db1493/original/3X/f/f/ff2846ce445faeae63d2d0ac0375c4bc9b7273bb.jpg" width="690" height="387">

@12meterkuk
This is what can happen when your batteries short out.
```

---
## \#17 Posted by: CheerioCoil Posted at: 2017-10-08T04:22:09.495Z Reads: 78

```
Shave off the plastic boundaries at the top and bottom (according to your picture's orientation) and you'll have more space to play around with. I'm going to stack my bms though. I feel that the much greater potential to create a short with your unconventional configuration will cause more problems than a possible overheating issue with the bms stacked on top. Just my 2 cents.
```

---
## \#18 Posted by: 12meterkuk Posted at: 2017-10-08T06:43:03.435Z Reads: 74

```
I just finished the pack, all is well for now. Using the normal configuration. Will update if any explosions occur.
```

---
## \#19 Posted by: CheerioCoil Posted at: 2017-10-08T12:08:59.953Z Reads: 67

```
pics! pics! you must show pics!
```

---
## \#20 Posted by: 12meterkuk Posted at: 2017-10-08T13:16:57.330Z Reads: 64

```
<img src="/uploads/db1493/original/3X/d/d/dd609cd05d76c0c2f459fb5114375cb6a1daead6.jpeg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/a/7ab415b6b9b955c83a3e960d88b3389dea6482e5.jpeg" width="690" height="388"><img src="/uploads/db1493/original/3X/4/7/47d1b13c83a33f379c304d81e7ee24b34ba6b6ec.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/b/db7f551cb2f258d78aeda562efad66bfebfe5d1b.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/3/5/357721d2dd03761ca15daee322884ca1b6748bab.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/0/8/08df4f26875cf6d97fa272e7de8e9f37ab0ba391.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/1/2/12ee02b4853ad6dc12b5162c4f35377b6d758375.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/0/2/021aeb5920c991891ae8551e9feacf3789d96617.jpeg" width="375" height="500">



Still waiting on some insulation and heat shrink to arrive. Will post more pics then. 

A little messy right now but will clean it up in a few days
```

---
## \#21 Posted by: CheerioCoil Posted at: 2017-10-08T13:39:46.360Z Reads: 58

```
Looks nice so far! I'll be doing the same project later this month once all the materials come in. I also have a Bamboo GT :slight_smile:
```

---
## \#22 Posted by: 12meterkuk Posted at: 2017-10-08T16:28:52.379Z Reads: 60

```
So I went out tonight to try and test the full range of the new pack, and here are the results <img src="/uploads/db1493/original/3X/d/d/dd8d11184919e76f0d7b372cfdf46ab8c7e54331.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/7/f7fc96ae29a607fc6e15b84c33439ac923ea3b01.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/3/0/30f82d5edbd25efdc7748aae1e84d708c36e3953.jpeg" width="375" height="500">

I was going pretty slow as the ground was wet. Probably around 20kph average. 

The voltage never sagged below 70% from 80+% even when climbing a pretty steep hill. The last time I tried it it’s added from 85 to 40%. 

Pretty pleased with the results.
```

---
