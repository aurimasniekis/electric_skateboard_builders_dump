# Still Unnamed &#124; Loaded Vanguard &#124; Caliber trucks&#124; Torqueboards 230KV &#124; 150A X-Car Beast &#124; 6S Li-Po

### Replies: 18 Views: 859

## \#1 Posted by: phrancini Posted at: 2018-05-08T13:30:37.836Z Reads: 172

```
Hi! 

After a full year of thinking I finally decided to get myself a board. 

I wanted to start fresh but after looking around the used market I came across a setup for a ridiculously low price and I decided to go for it.

This is what I got:


* Loaded Vanguard deck

* Caliber trucks,

* 83mm wheels

* Torqueboards 6355 230kv (sensored but running sensorless because the JST connector doesn't fit on the ESC)

* TB mount

* Xcar beast 150A esc

* Random big fat transmitter

* 6S Zippy Flightmax 5800 mAh 30C


![20180422_175617|690x301](upload://7aFZoTFKZ9aMDOdQp1u5wdi2NbG.jpg)

Before it was held togheter by this ugly plastic case


But now that I completed some of my upgrades the board looks like this. 


![photo5445016438604671482|283x500](upload://19vcZcHGuNgnAIkg2COzor3xvHe.jpg)
I'm still waiting for the battery meter to arrive, hence the white tape :smiley: 

I found on thingiverse a BoostedBoards style VESC case and modified it to house that big ESC I got and then I 3d printed it, after that i modeled and again printed a case for the batteries to match the aesthetics of the ESC case, added an XT90s as an antispark switch and a battery meter. 

To be honest I don't know how i could better route the cables because for me this is the most disappointing part of the board right now. (I'm open to suggestions!)

![photo5445016438604671481|375x500](upload://t2wtjxGv369n4pNfPuRTiTN8JxG.jpg)![photo5445016438604671482|283x500](upload://19vcZcHGuNgnAIkg2COzor3xvHe.jpg)

I also replaced the transmitter with a mini remote that I have rehoused modifing another project found on thingiverse, and swapping the potentiometer for an Hall sensor following some advice found here on the forum. In the near future the remote will be completely scratch built using two arduinos maybe adding a voltage indicator on the transmitter. 

![photo5443076242963277974|375x500](upload://rafB0zHoywkmHBIsjPSBvMxKfLq.jpg)!

I can show you some more photos of the interior, if you are interested :slight_smile: 



The board Works fine, but I have to say that the range is a bit disappointing.

Have you got any Idea how I could make the board better w/o spending too much?

Hope you like it and looking forward to hear some suggestion from you guys!

Bye
```

---
## \#2 Posted by: rey8801 Posted at: 2018-05-08T13:50:06.672Z Reads: 136

```
[quote="phrancini, post:1, topic:54801"]
6S Zippy Flightmax 5800 mAh 30C
[/quote]

Nice! Let me know how it rides. Curious about the performance of the ESC, I guess hobbyking one. For the range 5800mAh is a bit low for esk8, moreover with Lipo at high discarge rate. You can lower the performance at the ESC level, if you have the programmable card or buy anothe rbattery and wire them in parallel 2p. If you won't like the ESC for almost the same price you could get a VESC 4.12 from Hobbyking, fully oppen source https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html. It's a good deal.

EDIT: For a good estimation of performance and range. Use http://calc.esk8.today/
```

---
## \#3 Posted by: AndyL Posted at: 2018-05-08T13:58:49.605Z Reads: 116

```
How ridiculously low did the setup cost?
```

---
## \#4 Posted by: phrancini Posted at: 2018-05-08T14:21:55.394Z Reads: 111

```
I spent 270eur for the board altogether + balance charger that I won't use since I have an IMAX B6

15 eur for the mini remote + another 10 for the hall sensor, charging board and step down for the remote mod.

another 10 in spares

3d prints were made at work, i'm estimating 5/6 eur in filament
```

---
## \#5 Posted by: Scoo_B_SK8 Posted at: 2018-05-08T14:32:02.885Z Reads: 100

```
Nice transformation, much improved ascetics.
```

---
## \#6 Posted by: phrancini Posted at: 2018-05-08T14:35:07.823Z Reads: 101

```
The board rides pretty well for what I can tell. It's my first board (and first time riding a longboard, but I've been riding snowboards for the last 20 yrs and this led me to buy one) so I don't really know what is good or bad (YET)

I'm still playing with the programming card to find the best settings for the ESC, but for now I set the maximum power to 70% because I'm still noob. :slight_smile: 

the ESC is pretty noisy and big, so VESC may be an option at least dimensionwise. Is there really a big difference from a Turnigy VESC an a Maytech one?

For now I'll stick with 2x3S batteries because they're pretty big and adding 2 more packs to get 2P woud require another battery case, maybe in the future I'll swap them for a 18650 pack, but I don't want to spend 200 eur at least ATM.
```

---
## \#7 Posted by: rey8801 Posted at: 2018-05-08T14:37:48.948Z Reads: 98

```
The VESC in general doesn't make any noisy. For what you spent it's a great build. Well done. I also moved to es8 from snowboarding :smile:
```

---
## \#8 Posted by: Wilsonliang777 Posted at: 2018-05-08T15:00:57.451Z Reads: 92

```
I like the remote case.  Do you have more pictures of it and can you send me the file so I can print one myself.   Thank you.
```

---
## \#9 Posted by: phrancini Posted at: 2018-05-08T15:20:29.557Z Reads: 89

```
Sure. the remote is based off this one. https://www.thingiverse.com/thing:2454391 but i scrapped the spring part and added 2 more magnets to make the thumbwheel go back to neutral. I also capped the hole for the screen, since I'm not using it.

EDIT: more picture will come as soon as I get home
```

---
## \#10 Posted by: phrancini Posted at: 2018-05-08T17:05:08.706Z Reads: 89

```
Here are the photos..

As you can see there is a dead man trigger that I already tested, yet not implemented since I'm waiting for the right switch to arrive.

![photo_2018-05-08_19-04-25 (2)|375x500](upload://itDO8jkOSYZPFpn0eLLdf3PRVv5.jpg)![photo_2018-05-08_19-04-24 (2)|375x500](upload://sFpMDWJG2CQEGLdXcm4kSoSQbQy.jpg)![photo_2018-05-08_19-04-25|375x500](upload://yW8MhGKBsD4rh8LbZA2BWy7spnS.jpg)![photo_2018-05-08_19-04-23|666x500](upload://fOubVTdm09JbQcvETuv8GkRJ5bR.jpg)![photo_2018-05-08_19-04-24|375x500](upload://5hpXb9qwuBLKNJYKyWPtPCXP92H.jpg)
```

---
## \#11 Posted by: Gabriel Posted at: 2018-05-08T18:44:18.304Z Reads: 81

```
Hey,

Really like your battery and ESC enclosure. Would you mind uploading them to thingiverse? :smiley:
```

---
## \#12 Posted by: phrancini Posted at: 2018-05-08T18:48:07.634Z Reads: 76

```
yeah! sure, i'll be doing that tomorrow morning once i get back to work! mind that are designed to be mounted only on a vanguard board! 

anyway, if you don't hear me back in a day just send me a PM!
```

---
## \#13 Posted by: phrancini Posted at: 2018-05-09T09:49:29.088Z Reads: 64

```
Here you are https://www.thingiverse.com/thing:2901270
```

---
## \#14 Posted by: Gabriel Posted at: 2018-05-09T15:05:01.691Z Reads: 57

```
Thanks a lot! I have just purchased a vanguard board so it's perfect!
```

---
## \#15 Posted by: Gabriel Posted at: 2018-05-09T15:15:00.461Z Reads: 52

```
Do you have the dimentions for your batteries? Just want to make sure that [these](https://hobbyking.com/en_us/zippy-compact-6200mah-6s-40c-lipo-pack-xt90-1.html) will fit before i start i 2 day print :D
```

---
## \#16 Posted by: phrancini Posted at: 2018-05-09T16:11:58.189Z Reads: 50

```
[these](https://hobbyking.com/en_us/zippy-flightmax-5800mah-3s1p-30c.html?___store=en_us) are the one i'm using. i'm using them side by side, like this

![batte|690x358](upload://kKIOU6nCmsGYtRmuGi9ZUS8hAoG.jpg)

i'm not sure you'll be able to fit that big battery, i suggest you (if you can) to switch for the one i'm using
```

---
## \#17 Posted by: Gabriel Posted at: 2018-05-09T19:09:01.455Z Reads: 43

```
Hmm would like to make my board 12s :D What program do you use to edit the 3d files?
```

---
## \#18 Posted by: phrancini Posted at: 2018-05-10T09:10:55.249Z Reads: 32

```
I designed it using rhinoceros
```

---
