# Budget 6s Build: E-Bike BMS and Complete 6S Wiring Diagram

### Replies: 7 Views: 2625

## \#1 Posted by: johnny_261 Posted at: 2016-08-30T06:19:19.979Z Reads: 176

```
Hi Guys,

I'm planning on doing a 10S build with hub motors soon, but since I've never used li-ion cells or a BMS, I thought I would start small to get some practice before I do my 10S build.  I have a left over motor and 6s esc so wanted to do a small single drive 6s setup with a BMS.

I was initially going to buy a cheap 6S BMS and bypass the discharging, but then found this [6s E-bike BMS rated for 60A](http://www.ebay.com/itm/6s-24v-Li-ion-Lithium-Cell-60A-18650-Battery-Protection-BMS-PCM-Board-w-Balance/172310664402?_trksid=p2047675.c100010.m2109&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D38828%26meid%3De3dd16f3c51747f2bf64e784ca11ddb2%26pid%3D100010%26rk%3D3%26rkt%3D9%26sd%3D222233315789) which I think should be enough amps.

Any reason why you guys think it won't work? Aside from being what appears to be on the big side.

The other things I will need are a charger.  Will something like this [charger](http://www.batterysupports.com/liion-lipo-252v-222v-2a-6s-wall-socket-battery-charger-ac-dc-p-135.html) work?

A QUESTION that's been bothering me is where do you find the female end for the charge plug that would go on the board.  How do you know which ones will fit? The chargers don't appear to give any specs on the male end of the plugs.  Are they standard or something? This is probably a noob question, but I couldn't find anything on this...

Was also going to wire in a [battery indicator](http://www.ebay.com/itm/2016-Battery-Capacity-Tester-Indicator-for-12V-24v-36v-48v-CAR-Lead-acid-lithium/172143986261?_trksid=p2141725.c100338.m3726&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D20150313114020%26meid%3Dc15551bc7aaa4c58b0d860a219d62251%26pid%3D100338%26rk%3D3%26rkt%3D18%26sd%3D331508332778) and probably use a 100amp circuit breaker as the on off switch just to keep costs down and make things easy for this build.

I'm going to be using Basen's for my 10s build and copying @Namasaki basically, so for this was thinking a 6s2p with Basen 26650's.

Also will be buying a [Sunnko 709A spot welder](http://www.ebay.com/itm/272216171968?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT) - most people seem to have good things to say about this one
```

---
## \#2 Posted by: Namasaki Posted at: 2016-08-30T06:42:09.636Z Reads: 165

```
The spot welder is good. It's what I use. 
The charger is fine but I wouldn't buy it from Supower. There shipping is very slow. You can get 2a chargers on eBay US sellers cheap and they work just as good. 
Be careful about that BMS. They are not specifying 60a continuous or 60a peak. My guess at that price it's 60a peak and maybe 15-20a continuous.
```

---
## \#3 Posted by: johnny_261 Posted at: 2016-08-30T06:47:04.836Z Reads: 153

```
Thanks for the heads up on Supower.   Yeah, I wasn't sure if it was 60a continuous or not, but since it is suppose to be for a bike that why I thought it might be.  It does say Typ 60A Max 70A, which I would interpret to mean 60 amp continuous 70 amp peak...but who can say for sure...

Where you did you get the female side of the jack?  I just want to make sure I get the right size that matches the charger.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-08-30T07:15:57.153Z Reads: 148

```
Ok, I didn't see that part. I bought a 5a 42v charger from Supower through EBay and paid $50 for expedited shipping and they didn't ship it for over 10days. I started emailing them and complaining and then they finally got on the ball and shipped it. 
The only reason I bought it from then was because I couldn't find one anywhere else. 
I had a worse experience with them when I was building my battery. I ordered a BMS and charger from them again through eBay and it never got past Chinese customs. I ended up getting a refund and buying from Bestech.
```

---
## \#5 Posted by: johnny_261 Posted at: 2016-08-30T18:30:23.906Z Reads: 124

```
<img src="/uploads/db1493/original/2X/2/20ca6e523e92861320cf17d3c032f52e7ac84013.jpg" width="333" height="500">

I've made a wiring diagram for this now.  I think I got it right, but was hoping someone could take a look.  I wanted the battery gauge to only be on when the board is on (to act as an on/off light sort of), I think I put it in the right place, but someone let me know if I didn't!
```

---
## \#6 Posted by: johnny_261 Posted at: 2016-08-30T18:35:35.268Z Reads: 110

```
This is the BMS diagram from the seller.<img src="/uploads/db1493/original/2X/a/a0daa9323203fe01487bee955e5a857ff3f47e32.jpg" width="500" height="500">
```

---
## \#7 Posted by: johnny_261 Posted at: 2016-08-31T16:32:15.279Z Reads: 88

```
I've now pulled the trigger and have bought the E-Bike BMS.  I will give it a shot and report back.

I know there aren't a lot of 6s guys out there anymore, but this might be a good and cheap way to get a electric skate together for people who are new to the hobby.

So far my budget is looking as follows:
$16 BMS
$55 for 12 Basen 4500 26650 cells
$50 for 190KV sensorless motor
$55 for 6s car esc
$4 for voltage meter
$16 for 25.2V charger
$10 for breaker switch
$30 for pulleys
$10 for belts
$30 for other random wires and connectors
$40 for trucks
$25 for wheels
$40 for remote 
Will make a homemade motor mount
Going to use an old board

So this build is looking like it will cost me under $400.  If you had to buy a board and motor mount I guess you would be closer to $550 perhaps.
```

---
