# Make my remote rechargeable!

### Replies: 24 Views: 537

## \#1 Posted by: robthebuilder Posted at: 2019-04-12T12:11:32.838Z Reads: 182

```
Good day!

I have this remote:
https:///collections/remote-controller/products/torqueboards-2-4ghz-mini-remote-controller

It runs on two AA-batteries in series (1.5V *2 = 3V). I want to make this rechargeable via a usb-port so I wanna stuff a lipo battery inside it :sunglasses:
 
I have a 1S 500mah lipo with a built in bms that I wanna use for this. The maximum voltage is as you all know 4.2V so i guess I'll have to step it down to 3 or 3.3V in order to use it with the remote. I then have to add a USB-port and step down the 5V from that to 4.2V to charge the battery. I also need to limit the current here to 500mah to charge the battery at 1C.

Can anyone help me with where I can find the step-down converters? :) I know some electronics but I'm far from an expert! If you know of any parts that can help me with this or if you have a better idea or solution, please let me know!


Thank you! :)
```

---
## \#2 Posted by: yelnats8j Posted at: 2019-04-12T12:25:55.174Z Reads: 172

```
https://www.electric-skateboard.builders/t/the-avio-mini-remote-mod/72074?u=yelnats8j

Check this thread out 

He mods the battery to be rechargeable and Im sure it can be adapted to fit in the normal case.
```

---
## \#3 Posted by: venom121212 Posted at: 2019-04-12T12:27:36.120Z Reads: 166

```
What @yelnats8j said :arrow_up:

Here's mine I just took a picture of oddly enough right before clicking this thread. 

![20190412_082537|281x500](upload://bjaVk9J6Vf3ri900QlU5PZI53KY.jpeg)
```

---
## \#4 Posted by: robthebuilder Posted at: 2019-04-12T12:35:45.804Z Reads: 152

```
Awesome! Thank you! :)
```

---
## \#5 Posted by: robthebuilder Posted at: 2019-04-12T12:51:07.329Z Reads: 148

```
Damn, that's a sweet controller :D
```

---
## \#6 Posted by: mmaner Posted at: 2019-04-12T13:26:04.047Z Reads: 142

```
calling @b264, aisle 2.
```

---
## \#7 Posted by: b264 Posted at: 2019-04-12T16:28:23.916Z Reads: 114

```
I've done this, and while it's cool and all, I don't really know if I recommend it.  The AA batteries last so long and in 1.5 years of daily use, I've only had to charge the lithium-ion battery twice, and the second time was yesterday.  I guess that means the microUSB jack won't wear-out, huh?

![20171227_015215|249x499](upload://iocUPJYDlr49I6zRcmJsZOYjQSJ.jpeg) 

![20171227_024410|249x499](upload://hU7q0Sn8g83QkmpxuUgELVutQxE.jpeg)

![20171227_031414|249x499](upload://8ozAF3hFWHW9qMxvrSaTcIMBxIl.jpeg) 

![20171227_031414%20(another%20copy)|690x345](upload://xthO8N98q91xTGY2oMGJaVGzEL6.jpeg) 

![20171227_033012|690x345](upload://8alVEAu3KGQkofoCMOaLezafsM7.jpeg) 

![20171227_033105|249x499](upload://6qT5MpjlikhVY4okhZClAa6mBjT.jpeg) 

![20171227_033124|690x345](upload://7upOlYAa46tq9TMuTv4ta9FPs0u.jpeg) 

![20171227_033152|249x499](upload://h6NCz6BIHk00fUGS3qPuVKhgr1w.jpeg) 

![20171227_033157|249x499](upload://x0b2uyC5UeMJqrnCGLFRCpFClCF.jpeg) 

![20171227_033216|249x499](upload://1jB1RGWrn55Q2LuyPwI7DjmkZCG.jpeg)
```

---
## \#8 Posted by: robthebuilder Posted at: 2019-04-12T16:40:53.982Z Reads: 100

```
Oh I see! Thanks for the info, that's interesting! Really nice with all the pictures :) I'll think a bit more about it before I do anything :)
```

---
## \#9 Posted by: b264 Posted at: 2019-04-12T16:43:34.760Z Reads: 101

```
FYI: 18650 will NOT fit in there.  A 14650 or an 18500 will fit.  To fit an 18650, you'd have to cut out a support piece that needs to be left there.

That's a Panasonic NCR18500A 2000mAh cell
```

---
## \#10 Posted by: robthebuilder Posted at: 2019-04-12T16:46:45.056Z Reads: 99

```
Ok, great! I was thinking of using a LiPo but maybe a 18500 is a better choice :)
```

---
## \#11 Posted by: b264 Posted at: 2019-04-12T16:48:34.425Z Reads: 98

```
The internal circuitry seems to run just fine on 4.2V.  I didn't need any kind of regulator.  It's just running on the 1S lithium voltage, straight.
```

---
## \#12 Posted by: b264 Posted at: 2019-04-12T16:56:43.257Z Reads: 91

```
I have about 8 Mini Remotes and I only modded this one.  I really fail to justify the effort to mod any more.  The AA batteries last so long, especially if you get the really good ones.  Now I use "Energizer Ultimate Lithium" AA batteries (not rechargeable)
```

---
## \#13 Posted by: deucesdown Posted at: 2019-04-12T17:06:26.962Z Reads: 90

```
https://www.electric-skateboard.builders/t/mini-remote-upgrade/51991?u=deucesdown
```

---
## \#14 Posted by: Dmaxx Posted at: 2019-04-12T17:07:43.063Z Reads: 88

```
![15550885455447753901589883684195|690x388](upload://An173L5kBUSJVU8KMnO1WIS1pFH.jpeg) ![15550885915067017196592320074477|690x388](upload://zES5GZvn0MV3zBvVlAG1v8XQ0Yp.jpeg) 
I modded all 3 of my mini remotes with lithium ion cells,1s bms for charge only, voltage display, and a decent rocker switch for power. Never bothered with the step down voltage and have not had a single issue. Like @b264 said, the cell must be smaller than 18650.
```

---
## \#15 Posted by: deucesdown Posted at: 2019-04-12T17:12:34.778Z Reads: 81

```
The thing is, with primary cells it's guaranteed to run out at some point on the road. So you have to carry spare batteries and a phillips #1 screwdriver. Or be ready to walk. Which sucks balls. So any kind of rechargeable is preferable so you can reasonably control the state of charge.

I had to change batteries on the road 2 days ago.

But, the remote likes 1.5v not 1.2v like common nimh AA (eneloop)😭

So imo it's worth the trouble to mod.
```

---
## \#16 Posted by: b264 Posted at: 2019-04-12T17:16:23.709Z Reads: 81

```
True that, but using Mini Remotes daily for years I've only had to "change batteries or kickpush" once and I did actually have a tiny screwdriver and two batteries in my bag.

But you do have a point.

If you modded it to have a ***battery gauge*** instead of be fully rechargeable I think it'd be fine also.
```

---
## \#17 Posted by: robthebuilder Posted at: 2019-04-12T17:43:40.710Z Reads: 78

```
Thank you guys! All very interesting information.

I will either do some kind of mod on the mini receiver or build a firefly remote instead :grin: 

At the moment I always carry spare batteries and a screwdriver. I also always carry spare belts and all the tools needed to change them so i'd say I'm quite prepared :sunglasses:
```

---
## \#18 Posted by: robthebuilder Posted at: 2019-04-12T17:44:08.014Z Reads: 79

```
Very nice mods! :grinning:
```

---
## \#19 Posted by: deucesdown Posted at: 2019-06-05T03:27:09.139Z Reads: 59

```
[quote="b264, post:16, topic:90250"]
If you modded it to have a ***battery gauge*** instead of be fully rechargeable I think it’d be fine also.
[/quote]

This made sense, took a crack at it.

![IMG_20190604_232134|666x500](upload://IZLG8f4MR4ToOhQj9KfyMIOEy3.jpeg) 

![IMG_20190604_232148|666x500](upload://mh5EHrqepkh0b0y9sGPDaXEgJpD.jpeg) 

The voltmeter is one of these. There are a lot of different ones. This one is 0-100v, but shows single digit volts as "3.41" not " 3.4". Has the adjustment pot. It's the 3 wire version -- just connect the blue and red together. Minimum voltage is about 2.5v or so. Unfortunately this makes things not great with eneloop, but as you said, getting a voltage indication is 99% of the battle. I can use duracells here (those fucking things leak in every device I put them in).

https://id.aliexpress.com/item/DC-0-V-100-V-0-28-Inci-LED-Digital-Voltmeter-Tegangan-Meter-Auto-Mobil-Ponsel/32974251122.html

To make the cavity I traced the meter with magic marker, used a brad point bit to drill 2 holes, then diagonal cutters and utility knife to creep up on the fit. hotglued everything in.

Tactile switch, I think a 6x6x7 will be perfect. Will report when I test one. The hole for the switch was made with a 5/32 brad point bit.

I made a AVIO remote, but unfortunately I can't get a good grip with gloves that lets me have full range of the trigger. Maybe just need practice.
```

---
## \#20 Posted by: deucesdown Posted at: 2019-07-09T16:02:26.900Z Reads: 39

```
![IMG_20190709_115814|666x499](upload://plkYsnsVvz8fJrqJlPM52QHzkmw.jpeg) 

Very happy with the mod. 6x6x6 button will be flush with surface, need some nails to press. 6x6x7 will protrude just a bit, also very workable.

I'm gonna need some colored tape or paint soon...
```

---
## \#21 Posted by: thisguyhere Posted at: 2019-07-09T17:23:22.840Z Reads: 36

```
you sellin' these or what?

i tried and hated it.

![0322191953|690x388](upload://iVourfLasHSZ7EIDMASUYpBeSQq.jpeg)

![0322192002b|690x388](upload://wNtrkOuGovO5E0jmqAPomVQcPgK.jpeg)
```

---
## \#22 Posted by: deucesdown Posted at: 2019-07-11T04:13:57.459Z Reads: 29

```
[quote="thisguyhere, post:21, topic:90250"]
i tried and hated it.
[/quote]

Hated making the mods, or hated the results?

[quote="thisguyhere, post:21, topic:90250"]
you sellin’ these or what?
[/quote]

It's very tedious cutting out the hole for the voltmeter. Not fun. But hmm maybe I'll try to do a few as a give-back to the community...
```

---
## \#23 Posted by: thisguyhere Posted at: 2019-07-11T04:40:23.396Z Reads: 28

```
[quote="deucesdown, post:22, topic:90250"]
Hated making the mods, or hated the results?
[/quote]

hated doing the mod, like cutting stuff out, gluing the usb charging board, etc.

got a single 30q in there, i suspect it'll take years for the thing to deplete.
```

---
## \#24 Posted by: robthebuilder Posted at: 2019-07-11T07:56:20.469Z Reads: 23

```
Yeah probably. The AA batteries has about the same Ah and those lasts for years :)
```

---
