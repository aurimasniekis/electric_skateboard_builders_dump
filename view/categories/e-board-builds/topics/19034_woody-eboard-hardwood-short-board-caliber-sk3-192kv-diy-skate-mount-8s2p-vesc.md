# &ldquo;Woody&rdquo; eBoard &#124; Hardwood Short Board &#124; Caliber &#124; SK3 192Kv &#124; DIY Skate Mount &#124; 8s2p &#124; VESC

### Replies: 20 Views: 2211

## \#1 Posted by: PL4 Posted at: 2017-03-13T23:42:07.224Z Reads: 239

```
I've started planning and ordering my first build and could use some advice from all of you.
I've built a few quadcopters so I'm familiar with the tech, but I'm having a hard time trying to decide what motor to pull the trigger on.  I'm looking to start with a single motor setup to keep costs in check at first.

Build Plans:

* Custom Hardwood Deck 32" x 9.5"
* 90mm Flywheel Clones
* Caliber 10" 50 deg,. Trucks
* DIY Electric Skate Mount
* VESC - Any suggestions on the best source?
* Enertion Nano Controller
* 2-4x 5200Mah 10c 4s Lipo in series for 8s (already have them from my quadcopter). Plan to build my enclosure for 8s2p. 

Having never ridden an e-board I have no frame of reference to judge what motor to go with or the gear ratio.

Im 190lbs (86kg) and live in an area with some moderate hills. Right now I'm leaning towards the SK3 6473 192kv motor with 16t/36T gearing. I have access to a 3D printer so I should be able to play with the ratio if needed, but was really wondering if that motor was the way to go or if I should consider a higher kv option?

Putting the deck together:
<img src="/uploads/db1493/original/3X/b/3/b34f9fb0d5fc93681a6b96a0ca6ae8b4fe9b0d29.JPG" width="640" height="480">

Threw some old trucks/wheels on it to test out. 
<img src="/uploads/db1493/original/3X/a/d/ad648a9e0215f0385d8c4853cc5e774b2eb1b829.JPG" width="640" height="480">
```

---
## \#2 Posted by: IsTalo Posted at: 2017-03-14T00:06:00.935Z Reads: 219

```
Nice Build, but your battery just offers 52A, isn't it low for a Esk8? About Vescs, everybody says that @chaka ones is good, but they are normally similar one to each other. I think a 190kv motor is ok for you, and some pieces that try to don't forgive. You will need a Power Switch or a Switch key, or plug and displug every time and also nerd a 8s charger, I recommend buying a Bms, It is more conventional, just plug and charge. Always put photos, we all want to see
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-03-14T00:19:35.275Z Reads: 210

```
If you're looking to save money I'd get the remote and VESC from  however just get a VESC-X from Enertion if you've got the cash to spare.

[quote="IsTalo, post:2, topic:19034"]
52A, isn't it low for a Esk8?
[/quote]

Generally 52A isn't too low, especially for a single motor, however, lipo manufacturers are known to overrate their batteries so a lot of people cut the C rating in half to be safe. 26A would be too low so it might be wise to find a higher discharge battery.

Also, with higher voltage you get higher power, and the VESC can take 10S so I'd go with 10S. The 192kV 6374 SK3 will be good for a single motor build, and work well with the VESC and a 10S or 8S battery.
```

---
## \#4 Posted by: PL4 Posted at: 2017-03-14T01:05:41.464Z Reads: 202

```
Thanks for the replies!

I have a lipo charger already, so adding a BMS is probably down the road a bit.

As for the amp rating, please correct me if I'm wrong, but if I run 8sp2, I'd have up to 104A, right?
I was working under the assumption that the additional 2 packs in parallel would double the amperage. 

I'll definitely keep in mind moving to 10s when building my enclosure. 
I'll check out the VESC-X as well.

Is it worth looking at a sensored motor?

Thanks again!
```

---
## \#5 Posted by: IsTalo Posted at: 2017-03-14T01:17:56.686Z Reads: 191

```
Which calculations have you done to find 104A? It depends on the C-Rating...
Vesc-X looks pretty solid, but Everyweek someone have troubles with it...
About the sensored motors, It is better, but a lot of people say that it don't worth the money, I think it is good on lower speeds
```

---
## \#6 Posted by: PL4 Posted at: 2017-03-14T01:28:52.227Z Reads: 181

```
I was calculating, 
5200 Mah x 2 in parallel = 10400mah = 10.4 Ah x 10 C = 104A
```

---
## \#7 Posted by: IsTalo Posted at: 2017-03-14T01:39:24.350Z Reads: 176

```
Oh, right, so you want to use a 4s battery on a Esk8? It will have less power than a 8s... even less than a 6s that everybody says is the minimum (but it is not, I saw guys with 4s that runs cool). Or you use your batteries in series and make a 8s 52A that I think would work if you configure your vesc in a nice way or you use them in parallel that will give you more discharge, but less power. What do I recommend: Batteries are the part of the skate that if you try save money maybe you will mess up all your work, continue using this 4s batteries in your drone and buy a Finished Battery like Space Cell, it already have The switch and the Bms, so it is awesome. If you want to save a bit of money, buy the battery (6s or more) and the Bms and make your own.

In Brazil (Where I live) is 22:40pm so I'll sleep because tomorrow I have class (English Class too). Any questions, ask me, I would love to answer
```

---
## \#8 Posted by: PL4 Posted at: 2017-03-14T01:53:54.243Z Reads: 161

```
Thanks for all the info, I do plan on 2 packs in series and then another 2 packs to march in parallel. So 8s with 10400mah.
```

---
## \#9 Posted by: NickTheDude Posted at: 2017-03-14T02:11:18.049Z Reads: 174

```
Yeah that would work fine, however lipos are known for their high discharge rates so I would suggest finding a different one with a higher c rating as to save space. 20-30C is not uncommon.

https://hobbyking.com/en_us/zippy-flightmax-5000mah-4s1p-20c.html
```

---
## \#10 Posted by: PL4 Posted at: 2017-03-19T20:49:46.082Z Reads: 163

```
A few more components have arrived!

Caliber II Trucks
1/4" risers
90mm flywheel clones
XT60 to XT90 adapters
Battery display
10AWG wire

Motor and various Hobby King parts arrive tomorrow!
<img src="/uploads/db1493/original/3X/5/c/5c2f8503a3a2de20972a882981dbc91ac4b0119e.JPG" width="666" height="500">
```

---
## \#11 Posted by: PL4 Posted at: 2017-03-20T19:11:33.771Z Reads: 158

```
HK order is in. Received a few more odds and ends.

XT90 Series connectors.
XT90 Parallel connectors.
5.5mm bullet connectors.

And most importantly my Sk3 motor.
<img src="/uploads/db1493/original/3X/2/1/2109e75c110581fc1432ba71ee079701dda48b47.JPG" width="326" height="500">

Now the wait on DIY to ship their mount and VESC intensifies.
```

---
## \#12 Posted by: PL4 Posted at: 2017-03-22T16:18:05.535Z Reads: 152

```
<img src="/uploads/db1493/original/3X/1/2/125dcc4e9e98aaa0d8ad1f84e7df726df93ee28c.JPG" width="375" height="500">

Another pic while we wait on the VESC and mount. 

I also picked up a couple Kydex sheets for the enclosure and will 3D print a controller for the GT2B that should arrive shortly. 

I'm going to need to step up to 1/2" spacers, too much wheel bite when turning with the 1/4" spacers.
```

---
## \#13 Posted by: rok Posted at: 2017-03-23T18:15:44.723Z Reads: 136

```
Do you mind sharing the price of everything together?
```

---
## \#14 Posted by: PL4 Posted at: 2017-03-24T10:24:18.161Z Reads: 135

```
All said and done a little under $600. 

Largest Expenses being:
Motor Mount + Pulleys: $110
VESC: $100
Motor: $80
Batteries (2 x 4s as I already had 2 on hand for 8S2P): $80
Trucks & Wheels: $70

I also already had a Lipo charger, so that was a savings there over getting into it first time.
```

---
## \#15 Posted by: PL4 Posted at: 2017-03-24T11:24:23.424Z Reads: 141

```
Started laying out my electronics and building a mold for my enclosure. Still a work in progress. 

Motor mount and VESC should be here tomorrow! 

Tight fit, hope the VESC fits. 
<img src="/uploads/db1493/original/3X/6/a/6a817bffde1909161e5834fc661ee684e7796beb.JPG" width="375" height="500">

1/2" insulation panel, hot glue and some sanding...

<img src="/uploads/db1493/original/3X/4/7/471ce426b94c0fecae0886feb22fd851cbd82d0b.JPG" width="666" height="500">

Not bad, needs a bit more shape before I mold the Kydex.

<img src="/uploads/db1493/original/3X/6/a/6af65f194869a2c4a1deeb2dd390bf59203d00cf.JPG" width="666" height="500">`
```

---
## \#16 Posted by: PL4 Posted at: 2017-03-26T22:03:13.463Z Reads: 126

```
The Kydex mold didn't form as welll as I hoped, so on to plan B with that.

Otherwise the electronics are good to go. VESC, anti spark loop key, motor, and controller are all setup. VESC needs more tuning, I'm sure. Flat spot has been ground into the Sk3. 

<img src="/uploads/db1493/original/3X/2/1/2153a567c42e18c79e051845ec506bdf07b61779.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/f/f/fff08b080b593b7ad0d299192b836e17538f726d.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/1/1/1181cccb685096169edb69e1ecb1b0a742b6112f.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/2/5/257988b363a9115064950b0a47fedc30bbb4456e.JPG" width="666" height="500">
```

---
## \#17 Posted by: saul Posted at: 2017-03-27T00:23:55.529Z Reads: 118

```
looks good. i have the same cells but the 10ah 2x 4s. you should get about 22ish but If your ok will a bit less speed I think 16/40 would be better for that size wheels. 
should be fine if the hills aren't too long. 

should be around 16 miles range... 18 if you are cruising...
```

---
## \#18 Posted by: PL4 Posted at: 2017-03-30T14:50:35.834Z Reads: 109

```
I'm still working out my enclosure, and hope to have something built by the end of the week, but in the mean time, I've got my VESC all tuned up and in FOC mode. I was able to take the board out or a brief test ride last night. 

   <blockquote class="instagram-media" data-instgrm-version="7" style=" background:#FFF; border:0; border-radius:3px; box-shadow:0 0 1px 0 rgba(0,0,0,0.5),0 1px 10px 0 rgba(0,0,0,0.15); margin: 1px; max-width:658px; padding:0; width:99.375%; width:-webkit-calc(100% - 2px); width:calc(100% - 2px);"><div style="padding:8px;"> <div style=" background:#F8F8F8; line-height:0; margin-top:40px; padding:50.0% 0; text-align:center; width:100%;"> <div style=" background:url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACwAAAAsCAMAAAApWqozAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAAAMUExURczMzPf399fX1+bm5mzY9AMAAADiSURBVDjLvZXbEsMgCES5/P8/t9FuRVCRmU73JWlzosgSIIZURCjo/ad+EQJJB4Hv8BFt+IDpQoCx1wjOSBFhh2XssxEIYn3ulI/6MNReE07UIWJEv8UEOWDS88LY97kqyTliJKKtuYBbruAyVh5wOHiXmpi5we58Ek028czwyuQdLKPG1Bkb4NnM+VeAnfHqn1k4+GPT6uGQcvu2h2OVuIf/gWUFyy8OWEpdyZSa3aVCqpVoVvzZZ2VTnn2wU8qzVjDDetO90GSy9mVLqtgYSy231MxrY6I2gGqjrTY0L8fxCxfCBbhWrsYYAAAAAElFTkSuQmCC); display:block; height:44px; margin:0 auto -44px; position:relative; top:-22px; width:44px;"></div></div><p style=" color:#c9c8cd; font-family:Arial,sans-serif; font-size:14px; line-height:17px; margin-bottom:0; margin-top:8px; overflow:hidden; padding:8px 0 7px; text-align:center; text-overflow:ellipsis; white-space:nowrap;"><a href="https://www.instagram.com/p/BSPikksg18b/" style=" color:#c9c8cd; font-family:Arial,sans-serif; font-size:14px; font-style:normal; font-weight:normal; line-height:17px; text-decoration:none;" target="_blank">A post shared by (@plfour)</a> on <time style=" font-family:Arial,sans-serif; font-size:14px; line-height:17px;" datetime="2017-03-30T00:52:02+00:00">Mar 29, 2017 at 5:52pm PDT</time></p></div></blockquote>
<script async defer src="//platform.instagram.com/en_US/embeds.js"></script>

Once I get my enclosure sorted I'll double check everything and get into final assembly mode.
```

---
## \#19 Posted by: PL4 Posted at: 2017-04-08T21:19:33.591Z Reads: 93

```
Tried to mold more Kydex and still didn't have the best results. Decided to go another route....

Picked up two 11"x7x1.5" baking pans, cutting the pans to make a 14" long enclosure.

<img src="/uploads/db1493/original/3X/8/7/8713c4c9c3e23f6e4df30f0a9be012926b7a61c4.JPG" width="666" height="500">

Cut out holes for the battery level display and epoxy'd in the loop key switch.
<img src="/uploads/db1493/original/3X/9/c/9c9866d5f5f1df8eac67de6282f48ff5dcd1f143.JPG" width="375" height="500">

I lined the inside of the pans with 2"wide electrical tape to prevent shorts. Used a bit of hot glue to keep stuff from moving too much.
<img src="/uploads/db1493/original/3X/9/b/9bf503e8f72f8f3db6a069e5bd8476f97de7fa26.JPG" width="375" height="500">

Some primer, paint and screw inserts for the deck later....
<img src="/uploads/db1493/original/3X/0/d/0d0b6a900ac20c285e48231e0d251247b138009e.JPG" width="375" height="500">

I left a small gap so the vesc could cool.
<img src="/uploads/db1493/original/3X/1/7/17af1fe41c9d122ed76b96ae6954b2d1e187c640.JPG" width="666" height="499">

Took a 3 mile ride today, tons of torque and more speed than I need.
It's been a fun build, still needs some tuning and refinement. 

Next up 3D printing a new case for the GT2B remote.
```

---
## \#20 Posted by: PL4 Posted at: 2017-05-03T22:30:56.178Z Reads: 66

```
Quick update, the original deck cracked, which is too bad, but I've got a very similar, yet thicker one to try out next.

Today I had my first eskate wipe out, the VESC cut out while accelerating hard, the board slowed and I then was slowed by the pavement. 
I found my absolute max amps was too low, causing the cut out. I bumped it to 160a and it's all good now!
```

---
