# Battery recommendation? (Slightly compact AT board. UK/EU)

### Replies: 21 Views: 306

## \#1 Posted by: nirurin Posted at: 2019-03-23T02:36:14.433Z Reads: 92

```
Hey everyone, some of you may know me from my build thread, where I've been learning a lot about what's good and what's bad and what is feasible within my rather tight budget and niche-ish needs lol. 

Current basics for my board/needs:

- Haggy drive setup, with dual-190kv or 170kv motors, and bergmeister 6" wheels (usually). 
- Hopefully a 36" board like a switchblade but I haven't sourced a board yet.

- Trying to keep it relatively light/compact (for what it is) as it'll need to be transported in a fairly small boot and/or carried occasionally.
- Mostly normal use (roads et al), but I may sometimes be going onto a beach or something similar (with different 8" wheels instead), and so I've been told I need a decent amount of Amps to keep me moving even on the firm-packed sand where I live.
- On the bright side, where I live only has a few hills, however the ones we have are pretty steep and so decent/reliable braking is definitely a requirement. Something else I was told I need a decent rating for.
- Top speed is completely bottom of my list of needs. As long as it moves decently I'll be happy. 
- Range / time is more important than speed. I'd rather cruise around for an hour, than blast around for 10 minutes haha. 

So I have a few options:

Liion

10s5p (something i've been offered) - overkill for speed but should fill my needs. Pretty big and heavy though, and probably won't fit on a 36" board (it was designed for a 40" setup). 

8s5p - probably the best configuration for my uses, that I can come up with. Still pretty big and heavy though. ~£300 and 2.4kg. 

LiPo

Turnigy 4s 60C 5000mah - 8s2p setup. Way more discharge (overkill? not sure). Similar weight at 2.3kg, but will fit on the board more easily. Also only £140. Same speed but less range compared to Liion. (Could change to 8s3p setup for £210, but then it's over 3.5kg)

Turnigy 5s 30C 5000mah - 10s2p setup. Still more discharge rate than liion I think. Same weight etc. £200. More speed than I'd need, but almost the range of the liion. Might be the best option? 

New edit: Zippy flightmax 4s 30C 8000mah - 12s1p setup. Actually seems to work out better than the 10s2p setup. Similar price and weight, but a flatter package. 


So yeh this is where I am. Playing around with lipo configs to see what I can come up with. I think 6s is a little too low, 8s or 10s seems to be about right, but getting to 3p is suddenly much heavier than i would like. 

And after spending a couple of days reading up on batteries and prices and dimensions and voltages and amperages... I needed a sanity check from people on here. It's very likely I'm missing something obvious, or that my calculations are totally wrong (I've been using [calc.3dservisas.eu](https://calc.3dservisas.eu/)). Where I'm confused is that I'd been recommended LiPo as it was meant to be the better option when it came to size/weight/price/performance... but in order to match the LiIon for range I seem to end up much much heavier, or wasting a bunch of performance on speed I don't want/need (though I'm not sure if this excess can be used in my favour?) 

So yeh, long story short, if anyone has some advice on the most efficient setup for my needs, please do let me know. I'm sure most of this made no sense! Like I said, I needed some guidance and a sanity check, as there's just so much information to go through and so much of it is out of date or doesn't apply to my situation. 

Thanks to anyone who helps, everyone has already been really helpful on here, it's been a great community :)

EDIT - Turns out these packs are all too deep really. Need to stick to 3s or 2s lipo packs. Back to the drawing board!
```

---
## \#2 Posted by: moon Posted at: 2019-03-23T02:44:46.362Z Reads: 76

```
[quote="nirurin, post:1, topic:87999"]
* Hopefully a 36" board like a switchblade but I haven’t sourced a board yet.
[/quote]

I think @bigben is selling an evo falcon (36"?) with an enclosure for a good price
```

---
## \#3 Posted by: nirurin Posted at: 2019-03-23T02:54:42.835Z Reads: 77

```
Haha, he's selling the batteries (which is from an Evo Falcon 40) but he doesn't have the board anymore. That's where the 10s5p is from :slight_smile:

Which is probably the cheapest setup (from a reliable source) I could go for, and it's definitely tempting. But it's going to be heavy and (unless I can figure something out) it'll require a 40" board which may not fit where it needs to go for transport.
```

---
## \#4 Posted by: moon Posted at: 2019-03-23T02:55:52.471Z Reads: 75

```
10s5p what cells?
```

---
## \#5 Posted by: nirurin Posted at: 2019-03-23T03:02:12.969Z Reads: 74

```
30Q. So I mean they're great, if I was going for a commuting board and 40" would definitely work for me I'd snap them up. I may still snap them up haha. They're just a bit overkill for my needs (I think?) and it'll mean I'd have to compromise on size and weight. 

My plan for tomorrow is to take a tape measure to my boot to see if I can make it fit. I think it'll be very close though, especially taking the motors/wheels into account.
```

---
## \#6 Posted by: moon Posted at: 2019-03-23T03:03:25.068Z Reads: 69

```
if your lightweight and don't encounter many hills and want max range you can probably go single 6374
```

---
## \#7 Posted by: nirurin Posted at: 2019-03-23T03:24:23.299Z Reads: 63

```
oh, wow. All of my calculations I did, and I never tried changing from 2wd to 1wd. I'd played around with top speeds and torque and kv, but not actually dropping an entire motor. 

Dropping to a single motor will halve my torque, but double my range. (According to the calculator, though people on here seem to say it's more like 30%). Still pretty significant though. Really don't know why I didn't think of it earlier. 

It would have other compromises obviously, but it's worth keeping in mind.
```

---
## \#8 Posted by: nirurin Posted at: 2019-03-23T04:02:33.784Z Reads: 59

```
Hmm, randomly came across another battery I didn't know existed. 
https://hobbyking.com/en_us/zippy-flightmax-8000mah-4s1p-30c-xt90.html

A 12s1p gets me more range than the 8s2p 5000mah, and more speed, and it's roughly the same price and weight, and it's even a flatter package so it'll fit better under the board. Going to add it to the OP.

Edit:
Turns out these packs are all too deep really. Need to stick to 3s or 2s lipo packs. Back to the drawing board!
```

---
## \#9 Posted by: nirurin Posted at: 2019-03-28T06:19:56.551Z Reads: 44

```
Hi again :) I'm back with another question (though I'd like to think I'm much more knowledgable now than I used to be haha). 

Basically, I've now sourced two complete drive kits, largely using Dicky as a good source of various bits and pieces. However it's gotten to the point where I need to make a decision, and I'm not sure which way to lean with it. Thought maybe you could give me some thoughts?

I can now get either:

Full drive system (15/60T) with 6" pneumatics on 8mm axle trucks. 

or Full drive system (15/72T) with 8" pneumatics (different hubs) on 10mm axle trucks. 

I also have to choose between 170kv and 190kv motors, but I've mostly been erring on the 170kv side so I don't think that'll be a problem. 

The 8" wheels will be good for wherever I go, but I'm not sure if they'll be too much of a hindrance on road/path use. Though we do have fairly crummy road-edges in this country, so maybe the bigger tyres could be the way forward. Without having them in front of me it's difficult to visualise. 

Any thoughts? I would consider getting both sizes for different uses, but the axle sizes are different and I don't think there's an easy solution to that.
```

---
## \#10 Posted by: Andy87 Posted at: 2019-03-28T06:48:41.875Z Reads: 43

```
You can just get different bearing to make the hubs fit 8mm or 10mm trucks. shouldn´t be a big problem.
if nobody else will do it, i could take a picture from 6" compared to 8" after work... probably you more fast to look through the picture thread. I think @Riako posted once a picture with all kind of wheel sizes laying next to each other.

If you just want to go over grass and uneven street parts i would prefer the smaller wheels.
Idk how 8" and 8mm trucks would work out. seems a bit slim for me :sweat_smile: so if 8" than definitly the 10mm trucks. But that´s just my opinion.
```

---
## \#11 Posted by: nirurin Posted at: 2019-03-28T06:51:55.129Z Reads: 38

```
I've looked for bearings before, but seems that there isn't a bearing that bridges that gap. Making mtb wheels fit either 12mm or 10mm has bearing options, but I struggled to find a jump from 10 to 8.

It may depend on what the internal diameter of the wheels are though. I shall ask and find out. But Yeh using the big wheels on the thin axles does feel a little odd haha, and the width may cause issues on the smaller axles too.
```

---
## \#12 Posted by: Andy87 Posted at: 2019-03-28T06:57:19.749Z Reads: 40

```
Trampa sell adapter to make there superstar hubs fit 8mm trucks.
Inbetween of which trucks you need to decide?
```

---
## \#13 Posted by: nirurin Posted at: 2019-03-28T07:00:00.942Z Reads: 39

```
Both sets of trucks right now are parts of the drive kits that dickyho sells. I looked into getting other (brand name) trucks, but I hit problems with compatibility with motor mounts and pulleys.
```

---
## \#14 Posted by: nirurin Posted at: 2019-03-28T07:04:58.242Z Reads: 39

```
![s-l1600|690x451](upload://aqlaq6NYPOR6HN8WO2MIgbGaZSM.jpeg)

Thats the 8" kit. The trucks for the 6" are the ones in his shop (Paris style)
```

---
## \#15 Posted by: Andy87 Posted at: 2019-03-28T07:05:25.891Z Reads: 39

```
Ah ok! I don´t have any experience with those.
Just get the option which gives you most opportunities later to swap to different set ups with minimal changes.
It´s hard anyway to get the perfect set up ever. If it´s the first it´s even more hard. you will most likely anyhow want to change out some parts after you found your way of driving.
```

---
## \#16 Posted by: Riako Posted at: 2019-03-28T11:32:18.421Z Reads: 33

```
Don't know if it still could help ... 

8", 7", 6", 9"
https://amadridefr.files.wordpress.com/2018/11/img_201131_1601.jpg

9", 8", 7", 5"
https://monlongboardelectrique.files.wordpress.com/2017/10/img_20171027_231202l.jpg
;)
```

---
## \#17 Posted by: nirurin Posted at: 2019-03-28T16:34:18.761Z Reads: 26

```
Is that 7" tyre on the same size hub as the 8" tyre? I hadnt thought about that as an option.. Get the bigger wheels and have smaller tyres as a change option (two sets of tyres instead of two sets of wheels.)
```

---
## \#18 Posted by: Riako Posted at: 2019-03-28T17:18:27.934Z Reads: 25

```
YEs ;) 5" (Gummies), 6.5", 7" and 8" same hub with Trampa for exemple.

Also, 6.5", 7", 8" and 9" same hub with Fivestar hub for example.
```

---
## \#19 Posted by: nirurin Posted at: 2019-03-28T21:59:50.299Z Reads: 21

```
Unfortunately I think all those wheels will only work with 10mm/12mm axles, and I'm struggling to find a motor mount for a decent set of trucks in that size (without spending more than my budget allows). 

At the moment the DickyHo kit with the 8mm paris-style trucks is looking like my best option. Though it may be possible to fit larger wheels onto it in the future with a bearing spacer.
```

---
## \#20 Posted by: Riako Posted at: 2019-03-28T22:51:16.793Z Reads: 19

```
[quote="Riako, post:18, topic:87999"]
YEs :wink: 5" (Gummies), 6.5", 7" and 8" same hub with Trampa for exemple.
[/quote]

15, 14, 12, 10, 8mm axle truck ... the Trampa fits all of them :v: (sure they cost way more than the trucks you choose or than MBS Rockstar or Fivestar, but they fit all type).

Just add this : 
http://www.trampaboards.com/superstar--megastar-spoke-support-8mm-bearing-converter--off-set-p-26206.html

or get a 28x8mm bearing ..!
```

---
## \#21 Posted by: nirurin Posted at: 2019-03-28T22:59:59.836Z Reads: 20

```
I tried to find decent 28x8 mm skate bearings the other day but I couldn't really see any. I found a couple but the widths were way off and I wasn't sure they could be made to work. The only ones I noticed were similar didn't have any seals so they'd wear out pretty fast. 

I may well have been looking in the wrong places though. Certainly none of the skate shops had them, but there are other places I tried too. 

I DID try trampa because I knew they had some kind of converter, but I didn't notice they did one specifically for their wheels. Might be something to keep in mind for the future (if I'm unable to find a 28x8mm bearing!)

Someone did send me a picture of a 10mm bearing with some kind of spacer inside it that made it fit to 8mm, but I couldn't find where to buy those kinds of adapters. (It was just a metal sleeve, not the trampa one)
```

---
