# Connecting 2 vescs (XT90 female plugs) to one anti-spark (M&amp;F bullet connectors)

### Replies: 15 Views: 712

## \#1 Posted by: jalapeno_ninja Posted at: 2017-09-30T09:08:48.099Z Reads: 111

```
Hi All,

I've almost got all the parts for my build, and once putting it all together realising it's not all as plug & play as I thought!

Any advice on connecting my 2 vescs (female XT90s) to the anti-spark switch (diyelectricskate), which is 5.5mm bullet connectors. 

Cheers,

Andrew
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-09-30T12:17:32.245Z Reads: 104

```
Any chance you could post a photo of those three items. The inputs on the diy antispark are 5.5?
```

---
## \#3 Posted by: jalapeno_ninja Posted at: 2017-09-30T12:26:54.728Z Reads: 102

```
<img src="/uploads/db1493/original/3X/e/b/ebc97c9a15f30977e00459befca71457cfccef11.jpg" width="590" height="393"> x2 (female XT90)

+

<img src="/uploads/db1493/original/3X/7/2/7210888cd6b6dbb8e68ca28be26f848489e2b7b8.jpg" width="690" height="460"> (Male & Female 5.5 bullets on the anti-spark)

You can make/buy a XT90 parallell connector, then a XT90 to 5.5 bullets connector, just wondering if I can get it done in one, or there's a better solution (putting a different end connection on the vesc or antispark)
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2017-09-30T12:43:28.183Z Reads: 95

```
Ya I see what you mean. you could make something like [this](https://youtu.be/aCtiN1KR9iE) XT-90s are a bit bulky. Or you could switch everything over to 5.5's and be done with it. I use xt-60's personally. They carry enough current for me. I just use the xt-90 antis part for a loop key too. For me the least amount of bulk is best as long as it can carry the current safely with some headroom.
```

---
## \#5 Posted by: jalapeno_ninja Posted at: 2017-09-30T13:01:12.706Z Reads: 90

```
Lol, just watched that! :) Thanks for the link though. But then you'd still have to go from the one XT90 to bullets?

Yeh I agree, these XT90s seem quite chunky and real estate inside the enclosure is at a premium.

Wondering if I make the Connections off the VESC into bullets and make a 4 into 2 for the 2 vescs into the anti-spark. Wondering what the community normally does at both these items are 'off the shelf' (from diy)
```

---
## \#6 Posted by: jalapeno_ninja Posted at: 2017-09-30T13:05:16.509Z Reads: 87

```
Better question (I think) going back to the drawing board... best way to get 2 (-) 12AWG wires and 2 (+) 12AWG wires into 1 (-) 12AWg and 1 (+) AWG...

10s6P battery, 2x5065 140kV motors.. (if that helps to know max V pulled through)
```

---
## \#7 Posted by: i2oadsweepei2 Posted at: 2017-09-30T13:18:06.154Z Reads: 76

```
Yup you are correct. When I ordered my stuff from diy last year it really was plug and play. I ended up doing a bunch of soldering myself for the same reason. Real estate is at a premium. I like a clean setup too. Much less to go wrong. What you propose would be perfect and take up less space.
```

---
## \#8 Posted by: jalapeno_ninja Posted at: 2017-09-30T13:22:06.889Z Reads: 74

```
How would you practically go about getting 2 12AWGs into 1, x2? Trying to find a how-to/youtube on how to make these: https://i.ebayimg.com/thumbs/images/g/FzkAAOSwB-1YtESS/s-l225.jpg (sorry, I'm really new to electronics etc.. but not skating or engineering stuff
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-09-30T13:27:07.066Z Reads: 74

```
Are you using a bms for discharge? The max continuous for your bms divided by two. The 5.5's should handle at least 80 amps. I doubt your bms is capable of 160 amps. Even if it was 100 amps divided by two its only 50 amps per side. You would control this through the vesc.

I have a photo of the splitter that diy sent me. I'll post it in a sec here. Its easy enough to make. Being custom you can have the wires only as long as you need. brb
```

---
## \#10 Posted by: jalapeno_ninja Posted at: 2017-09-30T13:31:42.548Z Reads: 69

```
Was just discussing with our diy eSkate guru we skate with about discharging via the vescs and not using the BMS for discharge. My concern though is the vescs handle the overall pack discharge, if one cell (of the 10) plays up, the BMS would pick that up. I think my BMS is only a 60A / 30A max per motor, will double check.
```

---
## \#11 Posted by: i2oadsweepei2 Posted at: 2017-09-30T13:39:10.204Z Reads: 69

```
[quote="jalapeno_ninja, post:8, topic:34360"]
https://i.ebayimg.com/thumbs/images/g/FzkAAOSwB-1YtESS/s-l225.jpg (sorry, I'm really new to electronics etc.. but not skating or engineering stuff
[/quote]


I like those. My photo won't help you then. I'm not going to strip it off for you to see. This photo is not mine. You will need some soldering skills to get this done or a buddy with skills to help you.

<img src="/uploads/db1493/original/3X/c/b/cb7b5f395e4a91e700e421b67a50ea1e1ae27e44.jpeg" width="666" height="500">
```

---
## \#12 Posted by: jalapeno_ninja Posted at: 2017-09-30T13:43:21.266Z Reads: 64

```
Lol ws going to post this link: https://forums.offshoreelectrics.com/showthread.php?30639-*PYRO*-Parallel-bullet-connectors

I'm A-ok w/ soldering though, replaced an old BMS last night. I'm kind of always surprised at how.. 'obvious' (?) these solutions are... literally just soldering the bullets you need together, shrink wrapping them to finish..

2 of these will do the trick :) Thanks for your help eh, much appreciated.

Thought just ironing out the battery schematic was the had bit, the wiring etc for the rest of the component is a bigger pain in the backside!
```

---
## \#13 Posted by: i2oadsweepei2 Posted at: 2017-09-30T13:44:00.353Z Reads: 61

```
Or if your 5.5's have the notches you will need some kind of jig to hold them together otherwise you will go insane with them rolling around. Something that won't steal heat from the connectors like a popsicle stick or similar.

<img src="/uploads/db1493/original/3X/9/5/95df8bf770b7123e2fb1e47fa59a110a36625531.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/1/e12e30d5b45fc81cef7ed7551e17d34fcbe312dd.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/3/13287f4be1b76bf02171c215e38b44a974535946.JPG" width="375" height="500">
```

---
## \#14 Posted by: i2oadsweepei2 Posted at: 2017-09-30T13:45:13.453Z Reads: 55

```
oops guess you didn't need the last barrage of pics :stuck_out_tongue_winking_eye:
```

---
## \#15 Posted by: jalapeno_ninja Posted at: 2017-09-30T13:48:23.581Z Reads: 55

```
ha nah it's all good, just thinking now how to make them sit together, will get the dremel out and notch slots in each so they're locked in.

Lol, each 'answered' question on this diy eSkate just leads me to "ok cool, now onto solving the next bit!" .. bleh
```

---
