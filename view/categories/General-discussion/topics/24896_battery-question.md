# Battery question

### Replies: 27 Views: 2014

## \#1 Posted by: Perrin21 Posted at: 2017-06-08T16:21:15.374Z Reads: 163

```
I have been going through the posts on the forum and I'm basically lost.  I am trying to build a list of suitable batteries for my first build.

I would like the following from the battery
Slim profile to mount on the underside of the board.
High capacity for long range 14 miles +
High Performance for high speed.

What is the best i can get?  i have read 10s 4p is the way to go but i have been going through alibaba looking for batteries and i can't settle on anything suitable.  I want to build a kick ass board.  What batteries does Enertion and Evolve use?  I will be using dual FOCBOX controllers and dual motors (to be decided which).  All help is appreciated.  Im based in UK.

Thanks
```

---
## \#2 Posted by: thisguyhere Posted at: 2017-06-08T16:33:06.779Z Reads: 158

```
your best bet is to slow down a bit...do some more studying on batteries and how to put them together...and build your own pack using li-ion cells.

some use lipos used for RC applications but i won't touch on that here since i've never used them (and there are  [arguments on why they should be avoided](http://www.electric-skateboard.builders/t/lipo-vs-li-ion-electric-skateboard-battery-chemistry/3023)).

going this route will take longer, but knowing how to build your own pack will be indispensable going forward since you'll be able to fix and extend your power in the future.

to start, the most common li-lion cells used for esk8 are samsung 25r, samsung 30q, and lg hg2.  these cells have a high discharge rate which is necessary since the motors used in esk8 applications draw a lot of current (in amps).

since you're going for a 10s4p pack, you will need 40 of these cells.  once you have them, you'd string them together in particular configuration to make your 10s4p pack.

once that's done, please consider balance charging them through a balance charger or with a bms (battery management system).

there are great posts for each of these steps here on the board, if you have problems finding them i can send you some links.  just try googling first though.
```

---
## \#3 Posted by: Perrin21 Posted at: 2017-06-08T17:18:53.640Z Reads: 126

```
What do you think of this pack?  https://www.alibaba.com/product-detail/electric-skateboard-lithium-ion-battery-36V_60653022656.html?spm=a2700.7724838.0.0.52RIwn
```

---
## \#4 Posted by: lowGuido Posted at: 2017-06-08T17:40:18.265Z Reads: 119

```
that actually looks like a pretty reasonable pack. if you can get it for that price.
```

---
## \#5 Posted by: mccloed Posted at: 2017-06-08T18:10:15.139Z Reads: 113

```
Shipping will probably be another $75 - $100. But it looks like it has decent specs.
```

---
## \#6 Posted by: Perrin21 Posted at: 2017-06-08T18:19:21.253Z Reads: 109

```
i will enquire and let you know.  Thanks for the reassurance its a good pick.  What range and performance should this be capable of on a dual motor board?
```

---
## \#7 Posted by: Tuomalar Posted at: 2017-06-08T18:22:26.074Z Reads: 103

```
Specs say that it can discharge only 40A continuous which isn't enough for dual drive. I don't recommed.
```

---
## \#8 Posted by: Perrin21 Posted at: 2017-06-08T18:25:22.538Z Reads: 97

```
I haven't been able to find an 18650 based pack that outputs more.  any suggestions?
```

---
## \#9 Posted by: Blucas Posted at: 2017-06-08T18:28:20.657Z Reads: 99

```
If you have the money, you can try the LiiNiCoAlO2 (the same batteries that Tesla use in their cars if I remember correctly :stuck_out_tongue:)

 Jokes aside, the pack that you linked above seems like a decent pack.
```

---
## \#10 Posted by: Tuomalar Posted at: 2017-06-08T18:30:36.039Z Reads: 100

```
I think that you can't find any from alixpress or any other cheap places. You have to ask from some battery supplier or some body from here to make a battery pack for you if you don't have equipments.

Most of us use 10s4p made of 25R or 30Q cells which can discharge aprox 80A continuous.
Your range will be terrible due to massive voltage sag.
```

---
## \#11 Posted by: Perrin21 Posted at: 2017-06-08T18:36:41.385Z Reads: 108

```
well that killed my enthusiasm for the day :frowning:  it seems everything i do to get this project off the ground hits a roadblock.
```

---
## \#13 Posted by: Tuomalar Posted at: 2017-06-08T18:43:32.633Z Reads: 106

```
Usually these roadblocks are avoidable with bigger budget, but if you want to go cheap route you have to be creative.

25R can discharge 20A and 10s is 10 in series (10x3.6=36V) and 4p is 4 in parrallel (4x20A=80A)
```

---
## \#14 Posted by: Perrin21 Posted at: 2017-06-08T18:45:39.773Z Reads: 103

```
I'm not trying to go the cheap route.  I'm trying to go the not having to build it myself and burn down the house route
```

---
## \#15 Posted by: Tuomalar Posted at: 2017-06-08T18:46:21.411Z Reads: 101

```
Ok where are u located?
```

---
## \#16 Posted by: Perrin21 Posted at: 2017-06-08T18:48:53.271Z Reads: 100

```
UK, that pack says max 80A discharge.
```

---
## \#17 Posted by: Tuomalar Posted at: 2017-06-08T18:51:48.203Z Reads: 98

```
Max PEAK discharge. Look at continuous. Pack of 25Rs can peak disharge 200A for 5 second if you watch specs.
```

---
## \#19 Posted by: Tuomalar Posted at: 2017-06-08T18:57:43.499Z Reads: 101

```
50A but that doesn't matter. It's about performance. You batteries will drain faster if you stress them at 100% all the time. With higher discharge batteries you don't have to stress them so much which mean for example better range and lifetime.
```

---
## \#20 Posted by: Perrin21 Posted at: 2017-06-08T19:00:10.056Z Reads: 100

```
i have looked at the specs on the site for the pack and the individual cells have 8c discharge the same as the ones you describe.

Cell:
3.7V 2500mAh 18650 8C
```

---
## \#21 Posted by: Tuomalar Posted at: 2017-06-08T19:03:16.549Z Reads: 92

```
You should email them and ask what cells they use. And why they say it's made of 20A capable cells, but specs say it can only disharge 40A.
```

---
## \#22 Posted by: Perrin21 Posted at: 2017-06-08T19:05:37.220Z Reads: 91

```
i have emailed them, I will report back.  They may be able to build the pack with the samsung cells.  I will ask.
```

---
## \#23 Posted by: lowGuido Posted at: 2017-06-08T19:08:40.724Z Reads: 99

```
the 40A discharge will be likely because of the BMS they are using... if im not mistaken, the early SPACE cell that enertion sold had a 40A fuse on it as well.
```

---
## \#24 Posted by: sl33py Posted at: 2017-06-08T19:41:14.226Z Reads: 106

```
[quote="Perrin21, post:20, topic:24896, full:true"]
i have looked at the specs on the site for the pack and the individual cells have 8c discharge the same as the ones you describe.

Cell:
3.7V 2500mAh 18650 8C
[/quote]

I hate to burst your bubble - but if this pack works it will not work well.

As @Tuomalar has mentioned it will sag horribly and affect performance and range (and battery longevity).

Cells are rated with constant and peak (some specify max 10s discharge in amps):
the most frequent are the 25R, 30Q, and other similar 20A continuous cells (some are now higher).  Typically you can get higher capacity 3000mAh+ from cells with less continuous amps capability, or lower capacity 2500mAh and less that can sometimes output more than 20A.

The cells you linked on Alibaba are only 10A max discharge (peak to 20A for 10s):
<img src="/uploads/db1493/original/3X/8/0/80171479f7ed7d5a639e596d8431acd2c6599924.JPG" width="373" height="500">

You don't want to use 100% of the discharge capacity or it will sag.  They sag and heat - heat is bad for long life, and you'll get significant performance and range decrease.

Here's a great example of some great cells at their full 20A discharge:
[img]https://images.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.mountainprophet.de%2Fwp-content%2Fuploads%2F2015%2F06%2FSamsung30q.png&f=1[/img]
Especially note that right from fully charged they sag to 3.65/3.8 depending on cell!  I have my voltage cuttoff warning set to 3.7 (and it'll beep going up a hill as it sags under load - then not beep until i accelerate hard or another hill) (on lipos, but still applies).

Li-ion vs Lipo...  I usually go Lipo because they have a higher discharge rating - especially when you get into the 30C+ batteries (5000mAh = 150A discharge capacity w/ peak to usually 40-45C), and i have some 65C lipos as well (smaller 3s 4500mAh A-Spec nanotech for 9/12s in series).  at 65C *4.5Ah = 292A discharge!  So when you only use 40-60A of almost 300A...  no/minimal sag!  better range and better performance.

I would not trust alibaba or aliexpress to sell legit cells, or to have honest ratings.  I always figure even the lipo C ratings are more marketing than fact - but with so much more discharge capacity - more room for leeway IMO.

I charge and inspect my lipos, so i'm not as worried about them catching fire.  Look for damage/puffed cells - and use a temp probe when charging - any bad batteries will have a heat issue before catastrophic failure.  And charge in pyrex (cheap from goodwill/used).

my .02 - hope it helps.
```

---
## \#25 Posted by: jaykup Posted at: 2017-06-08T20:00:18.859Z Reads: 92

```
I see 4 options:

1.  Make a battery out of 18650 cells.  10s4p / 12s3p.  Samsung 25r, 30Q. Buy from https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html.  Solder or tab weld, a few tutorials on the forums.

2.  Have someone build you an 18650 pack, there are a few builders on the forums.  Maybe @chaka or @longhairedboy can make you one.

3.  Buy an 18650 pack that you know contain high quality cells (Samsung 25R/30Q etc) from @torqueboards at diyelectricskateboard or alien power systems

4.  Buy some lipo packs from Hobby King.

Edit: Highly recommend staying away from chinese no-name 18650 cells.  They are not all created equal, and most 18650 cells will give poor performance, there are only a few good ones out there that have enough discharge ability to work on our skateboards.
```

---
## \#26 Posted by: Hummie Posted at: 2017-06-08T20:44:20.209Z Reads: 91

```
Gare you trying to it all at once or just get going because doing an 18650 pack spot welded with a bms and switch is a lot.   easier is just get some lipos from hobby king and a 10 dollar balance discharger and be done.  the hobby king flightmax 2 or 3 cell packs will out do almost any li-ion pack's power output so you won't have to worry about that and you can just plug them in and same with the balance discharger.
But I want a nice li-ion pack n button badly. Just has so many drawbacks.  Not cheap
```

---
## \#28 Posted by: Tuomalar Posted at: 2017-06-09T11:07:16.244Z Reads: 78

```
Depending how big that bms is. You can try to remove it and set it next to battery if you deck is long enough to make it fit.
But for example i dont't have that much space so i ordered smaller one. I recommed to leave that bms and order better one for example from batterysupports.
```

---
## \#29 Posted by: Hummie Posted at: 2017-06-09T14:07:04.533Z Reads: 70

```
http://www.etotheipiplusone.net/?p=4187

here's the harbor freight chainsaw teardown i was talking about above with the large battery with no bms running by "the power of robot baby jesus" alone
```

---
## \#30 Posted by: billappleton Posted at: 2018-09-11T16:14:54.475Z Reads: 31

```
I have another battery question. In this video he hooks up six of these HRB 7.4V 10000mAh 2S LiPo Battery 25C. 

https://youtu.be/LPoy7YSkd98

Why didn't he route the balance cable harness through the deck for an external charger? When you charge these cells you need the balance cable connected to the BMS right?

https://www.ebay.com/itm/HRB-12S-10000mAh-25C-high-spec-Lipo-battery-assembly-for-electric-skateboards-/113188753322
```

---
