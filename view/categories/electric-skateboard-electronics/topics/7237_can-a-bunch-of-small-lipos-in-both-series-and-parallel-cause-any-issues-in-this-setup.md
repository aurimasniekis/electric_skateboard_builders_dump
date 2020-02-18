# Can a bunch of small lipos in both series and parallel cause any issues in this setup?

### Replies: 27 Views: 2074

## \#1 Posted by: evoheyax Posted at: 2016-08-06T23:20:50.026Z Reads: 100

```
So I was planning to use the multistar 16 Ah cells in my new build, but I'm realizing, that I don't have space for the vescs unless I put them inside, and the multistars literally take up every square inch, so they will not work for this build.

I'm looking at these small batteries. They are a 3s 2.2 Ah's. Dimensions are exactly what I'm looking for (with a little extra room for cabling).

So my plan... 24 of these packs in total, putting them in sets of 4 in series to create 6 set is parallel, to get a 12s6p battery. 13.2 Ah in total. They are 25c batteries, which I know is probably exaggerated. If there are 25c, we would have 330 amps max. If I stay conservative at 10c, they can do 132 constant, which Is close to what I would like to run this board at.

Now, I will desolder the wires so I can use 8 gauge wire (they come with 12 gauge I believe).

Could one see any issues with this battery pack?
Are the tabs of the cells limited to a certain amps?

Thank you for any advise. Total cost for this battery would be $266 USD plus shipping, and I would have some play room for wires, and space for 4 vescs so I can do the quad motor still.
```

---
## \#2 Posted by: zk8_builder Posted at: 2016-08-06T23:26:21.996Z Reads: 98

```
You could do the flat pack strategy to the 16ah multistar
```

---
## \#3 Posted by: evoheyax Posted at: 2016-08-06T23:32:53.390Z Reads: 96

```
I did that. I have them soldered up as 2 6s packs right now and they are 23mm thick, each one is a 2s2p.

Basically, I have 2 long square slots to put batteries. Each hollow slot for electronics is 792mm long, 84mm wide, and 23mm deep. 3 of the 2s2p multistars fit in each slot with very little space for anything else. I have done the geometric math and determined I can fit 4 vescs and 24 of these small cells into these cutouts with extra space for power switch, and maybe even for a bms. But I need to know if I'm over looking something with putting a bunch of small cells together like this.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-08-07T00:06:00.190Z Reads: 89

```
The alternative also is that I could fit a 12s5p (60 cells total) of the LG HG2. This would be 15 Ah total and 100 amps continuous max, which I think will be enough. The only problem is I don't have a spot welder, so putting this guy together might be hard.

Any thoughts?
```

---
## \#5 Posted by: lowGuido Posted at: 2016-08-07T00:18:29.612Z Reads: 82

```
this thread needs diagrams...

or photos


..or both
```

---
## \#6 Posted by: evoheyax Posted at: 2016-08-07T00:30:05.385Z Reads: 81

```
Ok, here's a diagram of what I'm working with.

<img src="/uploads/db1493/original/2X/f/fc1ddb41c7b78c41841586548b0be434bc937ca4.jpg" width="690" height="381">

And an extra one to show it's sexy curves :slight_smile:

<img src="/uploads/db1493/original/2X/d/dcec4d2f00aa4912fb06c7e376fb17c4376fa7f6.JPG" width="375" height="500">

It's no polished yet (you can see some glue stains still), but the idea is there :)

All of those little screws btw are for the lid :)
```

---
## \#7 Posted by: zk8_builder Posted at: 2016-08-07T01:22:07.061Z Reads: 74

```
4 motors

powerful
```

---
## \#8 Posted by: evoheyax Posted at: 2016-08-07T01:29:58.314Z Reads: 73

```
As you can tell, this board is being built for high speed and distance. I should be able by my calculations get to around 34 mph on flats with hummies hubs, and with a 13.2 Ah battery, I'm expecting around 15-20 miles range. with the 15 Ah battery, 20-25 miles range. The 16 Ah, I expect could be around 28 mile range. But I also have a lot of hills, so my real numbers may end up being far less.

The multi star are out... They simply take up too much space.

so...

LG HG2 3 Ah lion cells (12s5p, 60 cells total, 100 amp max con, 15 Ah)
or
Zippy Compact 2.2 Ah lipo cells (12s6p, 24 packs total, 150+ amp max con, 13.2 Ah)
or
any other options that fit these dimensions and give some room for power switch, wiring, and other miscellaneous things???
```

---
## \#9 Posted by: evoheyax Posted at: 2016-08-07T01:37:01.593Z Reads: 72

```
Since I'm at it, might as well post some other pictures.

Here's the multistar 16 Ah 12s battery. As you can see, no room for anything but batteries.

<img src="/uploads/db1493/original/2X/1/17a0e495b22b06eb4e9b38f5a15a005f3ba13999.JPG" width="666" height="500">

And a tease with motors attached.

<img src="/uploads/db1493/original/2X/7/7fe94ff50d975c1faf4922d7aec8a02048d7c790.JPG" width="666" height="500">
```

---
## \#10 Posted by: lowGuido Posted at: 2016-08-07T01:56:11.699Z Reads: 69

```
im struggling to follow your maths..  24 cells.. per slot..
 so thats 4S6P per slot..
the cells are 2.2Ah so by 6 thats  13.2Ah

and I suppose you put them both in series to give you 8S6P 13.2Ah?

but then you talk about an option of 12S5P 60 cells.. so 5p would be 11Ah but you say 15Ah? Im not sure where that came from..

and then you are talking about 12S from 24 cells? so thats only 2P? 4.4Ah? 
im really confused.
```

---
## \#11 Posted by: lowGuido Posted at: 2016-08-07T01:57:33.983Z Reads: 66

```
wait.. at first you said 2.2 Ah and then later you said 3Ah per cell now I see where I was confused..
```

---
## \#12 Posted by: evoheyax Posted at: 2016-08-07T01:58:29.341Z Reads: 67

```
2.2 is the zippy lipos, 3 is the LG HG3 lion
```

---
## \#13 Posted by: lowGuido Posted at: 2016-08-07T01:59:14.591Z Reads: 70

```
yeah I got it now..
go with the 12S5P 15Ah option if you can fit it.
```

---
## \#14 Posted by: lowGuido Posted at: 2016-08-07T02:00:24.996Z Reads: 70

```
or make a small enclousre for the VESC's on top of the truck  mounts.
```

---
## \#16 Posted by: evoheyax Posted at: 2016-08-07T02:06:15.510Z Reads: 70

```
And I just realized my math is way off...

I miss measured the big spaces...

I really have about 535mm total in length in each one. take off 219mm for a vesc on each side, and that leaves about 317mm for battery space.

I updated the image to reflect this. I only have space for 17 cells per slot, or 34 total (I can squeeze 2 more in on the side to get 36). Way too few. But a 12s3p is too small, would only be 60 amps max.

If I do it sideways, I can fit 20 per slot, which is only 40 total. Not enough as far as I'm concerned, I might be able to fit 8 more in next to the vescs, but that still leaves me at 12s4p, 80 amps max, which I don't think will be enough.
```

---
## \#17 Posted by: lowGuido Posted at: 2016-08-07T05:26:49.998Z Reads: 60

```
I thought something wasn't right...  
make the VESCs little enclosures on top of the truck mounts.
```

---
## \#18 Posted by: evoheyax Posted at: 2016-08-07T05:33:21.524Z Reads: 58

```
I was originally planning on tucking them up close to the trucks under the board, as that's what hummie does and it works great. But I forgot that he doesn't have the heatsinks I have, which add bulkiness. Maybe I could do without the heatsinks, since I'm running 4? I wanted to keep the entire board very clean looking. I had put a layer of fiber glass on the bottom, but I don't really like it and am going to rip it off and put another layer of wood to cover the screw insert that hold the lid down. I wan to keep it all wood.

Thanks for the idea about putting them on top, didn't think about that, since your feet are never going to stand there anyways. The only thing is it kills the looks :( But then I could keep my 16 Ah multistars :stuck_out_tongue:
```

---
## \#19 Posted by: lowGuido Posted at: 2016-08-07T05:39:14.464Z Reads: 54

```
yeah it kinda sucks to have put all the effort into making it all internal and the have to mount them on top. but you have done a pretty nice job so far so Im sure you can make a couple of nice little boxes to go on top that will not spoil the looks too much.
```

---
## \#20 Posted by: evoheyax Posted at: 2016-08-07T05:50:27.053Z Reads: 55

```
I'm trying to see if theres a way I can fit more in. One option would be to add a few more layers.

Right now, I have 17 layers (3 base + 14 hollow). If I can stack the 18650 cells in eachothers grooves and do 2 layers, this would work. But I need to calculate how many more layers I would need. The good thing is, Its acctuall 22.225 mm's deep, and the 18650's are 18.35mm diameter. So I need to figure out what hieght I would need to stack a second row in the grooves to see if that's an option.

I could also do 20 of those zippy compact 2.2 Ah batteries instead of 24, which would know 1 p off and make it a 12s5p, with 11 Ah instead of 13.2 Ah, and then they would all be inside. But again, I don't know if I'm overlooking anything.

I have so many options:

- Mount underneath without heatsinks, maybe move the caps up to reduce footprint
- Mount on top with enclosure.
- Get these zippy compact 2.2 Ah lipos
- Get 18650s (either smaller count or maybe 2 rows)
```

---
## \#21 Posted by: lowGuido Posted at: 2016-08-07T05:59:12.040Z Reads: 56

```
I got the solution!
VESC INSIDE the wheels!
http://www.electric-skateboard.builders/uploads/db1493/original/2X/f/fb16e017cbc2b52153e3dd18152fef6e26de75bf.png
Boom :punch::microphone: (Mic drop)
```

---
## \#22 Posted by: evoheyax Posted at: 2016-08-07T06:01:17.478Z Reads: 52

```
I thought about this way back when I first noticed this problem, but he's not selling them yet as far as I know...

haha, I like the mic drop.
```

---
## \#23 Posted by: lowGuido Posted at: 2016-08-07T06:13:59.504Z Reads: 53

```
yeah true. cool idea though..
i'd go with the small enclosure on top. there is too many compromises with the other options.
```

---
## \#24 Posted by: Michaelinvegas Posted at: 2016-08-07T06:17:06.721Z Reads: 53

```
https://youtu.be/c1kC1EZoPaE

Multi star motors with ESCs built in
```

---
## \#25 Posted by: SimosMCmuffin Posted at: 2016-08-07T06:33:34.327Z Reads: 50

```
I'm not entirely sure if you just linked the motors to show that motors with built-in ESCs exist, or you proposed using them.

But I don't think multistar offers motors with the built-in esc in large enough can/power sizes to use in an E-board and the motors aren't built for hub motor use (axle and can not supported well enough) + the polyurethane attachment is another challenge.
```

---
## \#26 Posted by: Michaelinvegas Posted at: 2016-08-07T06:45:46.391Z Reads: 45

```
If I was a leprechaun 🍀I might consider using them...

Just saying that in motor ESC technology is herein the beginning stages
```

---
## \#27 Posted by: jrpwit Posted at: 2016-08-07T08:10:03.278Z Reads: 47

```
What are u from the future or something?!?! :laughing:
```

---
## \#28 Posted by: lowGuido Posted at: 2016-08-07T08:14:02.009Z Reads: 48

```
well I did design this chair with a flux capacitor..

http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/17
```

---
