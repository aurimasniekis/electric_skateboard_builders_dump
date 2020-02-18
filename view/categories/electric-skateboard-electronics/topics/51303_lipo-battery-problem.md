# Lipo battery problem

### Replies: 17 Views: 871

## \#1 Posted by: DullElysium Posted at: 2018-04-05T14:17:16.473Z Reads: 142

```
Hi,

I just got all my parts for my first build and I ran into this problem..

I tested the battery cells with a multimeter to see that I connect everything the right way. But I noticed that when I connect the multimeter to the battery negative and the start going through the cells, the 2nd and 3rd cells give me the exact same reading, no voltage increase.

If I put one head of the multimeter to the 2nd cell and the other one to the 3rd cell I get a reading of 0.0V. Every other combination seems to give me some results.

Might it be just an empty cell, or is my lipo faulty? I've not charged them yet, but I don't want to plug the bms in if it's something is wrong with the battery.
```

---
## \#2 Posted by: uncosk8r Posted at: 2018-04-05T14:32:35.363Z Reads: 132

```
What voltage do you get when you measure from the very first positive and the very last negative, and how many cells are in the pack?




More likely there is a bad connection, than a dead cell........either way it sounds like you might have a faulty (but maybe fixable) pack...
```

---
## \#3 Posted by: onepunchboard Posted at: 2018-04-05T18:39:02.963Z Reads: 111

```
sometimes the lipo connection inside cell gets torn apart. u just need to reconnect it with aluminum solder or spot welder.( i think u can also use acid flux with lead to solder but didnt try it before...)
```

---
## \#4 Posted by: DullElysium Posted at: 2018-04-05T18:48:40.967Z Reads: 107

```
5 cells. From first to last it shows 14.2V. I have another battery too and it is 21.5V, so there's definitely something wrong here.

I think I'll contact the seller, even though it's been quite a long time since I ordered, but due to Enertions delays, I didn't start building until now.

*fixed typo
```

---
## \#5 Posted by: wafflejock Posted at: 2018-04-05T18:56:07.786Z Reads: 96

```
Even if 1 cell is dead at 13.3V for the entire pack if we assume 4 are working that's still 13.3/4 = 3.325V which is getting pretty close to the voltage cliff.  Wondering how long ago you go the pack and if it was checked beforehand and what voltage the cells were at before sitting.  In general lithium based batteries can sit on the shelf for a pretty long time and barely lose charge typically but they aren't supposed to be stored for long periods at full charge or anywhere near empty (want to be around 3.7-3.8V per cell to have them around the middle area for storage to avoid falling off the low voltage cliff or stressing the cell storing it full)
```

---
## \#6 Posted by: DullElysium Posted at: 2018-04-05T19:02:14.797Z Reads: 81

```
Sorry i got a typo there. 14.2V seems to be the full battery voltage at the moment.

It's one of those Zippy lipos from Hobbyking. Just checked my order and it was placed on the 3rd of december and the batteries have been sitting on my shelf ever since they arrived.

Wish I checked the cells as soon as the order arrived, but I'm still a big time newbie when it comes to these things.
```

---
## \#7 Posted by: Acido Posted at: 2018-04-05T19:07:01.342Z Reads: 68

```
Check every battery alone, if its reads out good then you just connected something wrong
```

---
## \#8 Posted by: DullElysium Posted at: 2018-04-05T19:14:15.491Z Reads: 68

```
ok so here's what my multimeter shows now if I contact the negative straight to the battery negative and start going through the cells:

cell 1: 2.0V, 
cell 2: 6.5V,
cell 3: 6.5V,
cell 4: 11.1V,
cell 5: 13.8V

I'm currently talking to customer support too. Let's see what they say.
```

---
## \#9 Posted by: wafflejock Posted at: 2018-04-05T19:34:43.755Z Reads: 61

```
Yeah not sure what to tell ya but something definitely screwy going on there, would see what customer support says but no cell should be below 3.0 and no cell should be above 4.2 so something funky happening.  Measuring from the negative going up you should basically see the voltage of one cell added at each spot definitely not the case here let us know what they say.
```

---
## \#10 Posted by: Okami Posted at: 2018-04-05T21:13:52.852Z Reads: 55

```
Balance lead might be broken. I also had this sort of problem a while ago
```

---
## \#11 Posted by: ZackoryCramer Posted at: 2018-04-06T04:19:27.780Z Reads: 52

```
[quote="DullElysium, post:8, topic:51303"]
cell 1: 2.0V,
[/quote]

You need to get rid of that pack rn.
```

---
## \#12 Posted by: DullElysium Posted at: 2018-04-06T07:36:38.003Z Reads: 51

```
So here's where I'm at at the moment. I contacted the customer support and they told me to file a warranty claim and hold on to the faulty pack until I get a replacement and then dispose the faulty one according to my country's laws.

I did one claim and it came back rejected with no explanation so I contacted their support again. Found out that they wanted a picture of me measuring every cell (guess they wanted to make sure it's actually faulty). So I filled out the warranty claim with the pictures and it's currently  pending.

I'm surprised they didn't tell me that I should've contacted them sooner. We'll see how this new claim goes.
```

---
## \#13 Posted by: DullElysium Posted at: 2018-04-07T07:32:34.602Z Reads: 40

```
Ok so they finally got to the 30 days warranty and no matter how I tried to put it, they wouldn't nudge. So the lesson here is that if you go and order from hobbyking, you are the quality control so test everything asap and don't just assume that the product was tested before sent to you.
```

---
## \#14 Posted by: pat.speed Posted at: 2018-04-07T09:27:34.972Z Reads: 33

```
I have to say HobbyKing is normally great in terms of lipos. I have ordered over 10 packs from them, 4x 3s 5000mah, 2 x 3s 2200mah and 5x 2s 5000mah. Every cell cane balanced within 0.02v of the others. I personally think turnigy blue or graphenes are the most reliable. I’ve heard a few bad things about zippys (although mine are fine) and nano techs
```

---
## \#15 Posted by: Namasaki Posted at: 2018-04-07T13:28:18.978Z Reads: 29

```
Anytime you buy Lipo packs from anywhere, you need to check them upon arrival. 
I had to return 2 packs to hobby king once and it was a no hassle experience and the replacements came quickly. 
The problem with your situation is that you had the battery too long and they can't tell if you used and abused them or not. 
Also besides testing new batteries, you need to storage charge them and check them periodically if your not going to put them into service for a while.
```

---
## \#16 Posted by: DullElysium Posted at: 2018-04-07T16:48:52.743Z Reads: 20

```
Live and learn. Well that was 50€ worth of a lesson for me.
```

---
## \#17 Posted by: DullElysium Posted at: 2018-04-07T20:50:22.895Z Reads: 18

```
Quick question. So now I have to order a battery to replace the faulty one. Ideally I'd order the exact same one, but it's not available to order from EU and 40€ shipping is a bit steep for me. But there's another battery with similiar specs, but higher discharge burst value.

So could I safely pair

ZIPPY Flightmax 8000mAh 5S1P 30C (40C burst)
with
ZIPPY Flightmax 8000mAh 5S1P 30C With XT90 (60C burst)

Thanks again for your help guys!
```

---
