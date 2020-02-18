# Diy Modular Battery Pack

### Replies: 20 Views: 3053

## \#1 Posted by: Namasaki Posted at: 2016-09-14T03:50:52.582Z Reads: 433

```
https://youtu.be/nkytMCKiPjI
```

---
## \#2 Posted by: FlashNova Posted at: 2016-09-14T04:46:20.717Z Reads: 416

```
I don't think it's a modular battery pack, it's a car battery jump starter:

http://www.suaoki.com/product-g_2.html

How come nobody told me I can do this? lol

It's 18000mah, I wonder what voltage it is.
```

---
## \#3 Posted by: Mobutusan Posted at: 2016-09-14T04:46:25.325Z Reads: 388

```
Pretty crafty. Only 12v and he gets up to 30kph?
```

---
## \#4 Posted by: Namasaki Posted at: 2016-09-14T04:52:53.111Z Reads: 372

```
It looked like a cool idea, I didn't realize it was only 12v. I just assumed it was at least 24v
```

---
## \#5 Posted by: cryzies Posted at: 2016-09-14T05:24:16.328Z Reads: 355

```
Clean! 12V 18000mah so 3s5p. Companies like to bloat their mahs as well so it could be really a 3s4p. 3D print a abs/nylon enclosure, get the mount, bam, cold swappable batteries.
```

---
## \#6 Posted by: HTownBomber Posted at: 2016-09-14T12:40:37.233Z Reads: 330

```
Curious about the potential of this as I have flirted with the idea of a modular BMS setup with 2 to 4 packs each with their own BMS in series. I know @JTAG is working on his own amazing (2)x6S BMS design. 

This battery pack is a bit cost-prohibitive if you want to run higher voltages, but there are similar high-current battery jumpstart packs at a $60 price point on Amazon. They have protective cases and LEDs to indicate charge levels. They come with on/off switches, input & output ports, USB ports & lights all pre-wired. These are all things I want on my battery pack. 

These packs claim very high (300-500A) peak output but aren't designed for continuous 12V discharge. So the question is what batteries they are using and how they would hold up to the demands of a typical esk8. If you wired 3 packs in series you'd have a 9s4p (~350 Wh) battery that could push some serious amps, and amp/voltage limits could be set on the VESC side. But would it overheat after a few minutes?  Would the BMS cut off after a few seconds of discharge, as one might want for protection in a jump-start application? Can current be pushed back into the pack safely? 

I might buy a couple of the cheaper packs and experiment.
```

---
## \#7 Posted by: Stevemk14ebr Posted at: 2016-09-14T14:07:38.812Z Reads: 272

```
It's only 2.1A continuous. Not even close to what you need. 600A is just the short term peak.
```

---
## \#8 Posted by: HTownBomber Posted at: 2016-09-14T23:29:04.172Z Reads: 260

```
2.1A is just the 5v discharge rating, as limited by the usb port standard. In jumpstart mode these things output 12V via 5mm bullets (EC5 port). Some of them claim they can supply hundreds of cranking amps, and cranking amps are a measurement of highest current the battery can supply for 18 seconds without a voltage drop. Wondering how they are delivering that kinda power.

I think the answer is that they are fudging their capacity ratings. So when they say 18000 mAh, that's only the capacity when they step down to 3.7v.
```

---
## \#9 Posted by: paragon Posted at: 2016-09-15T00:16:18.966Z Reads: 238

```
There was an rcgroups thread where a similar product was on clearance at walmart for $5, and the advertised 15ah battery within the device turned out to be a 3s 5ah lipo with a bms.
```

---
## \#10 Posted by: ajaynagra Posted at: 2016-09-15T00:22:46.002Z Reads: 218

```
Great video mate i couldnt find the link to the esc enclosure do you mind giving me the link And also how did you mount the battery pack to the board
```

---
## \#11 Posted by: Namasaki Posted at: 2016-09-15T00:45:54.232Z Reads: 204

```
That's not me in the video. I just happened to find the video on YouTube
```

---
## \#12 Posted by: Okami Posted at: 2016-09-15T06:44:09.234Z Reads: 196

```
I also thought that it's perhaps you in the video.. some reference for those who have not seen you in the real life might be helpful there ;)
```

---
## \#13 Posted by: CRABOLSKY Posted at: 2016-09-15T09:17:41.775Z Reads: 178

```
There is also this guy 20000mAh and 3 LED lights! http://www.suaoki.com/product-g_49.html
```

---
## \#14 Posted by: Namasaki Posted at: 2016-09-15T11:25:50.344Z Reads: 176

```
Sorry bout the confusion.
```

---
## \#15 Posted by: JLabs Posted at: 2016-09-15T11:55:44.258Z Reads: 177

```
Only 3s.. not sure how he runs on that. Cool idea tho.
```

---
## \#16 Posted by: HTownBomber Posted at: 2016-09-15T12:24:36.197Z Reads: 191

```
I mean, I guess it makes sense. Power banks are normally a few cells wired in parallel, rated on their total capacity at 3.7v because you're using them to charge your cell phone. With a power bank that can jump a car, those cells are arranged in series to output 12V, but the effective capacity at 3.7v is the same. The voltage is just stepped down with a buck converter. So a 3S 5Ah Lipo pack in the hobby world is a 15,000mAh battery backup for electronics consumers. Whatever, blame it on the people who decided to label batteries in amp-hours instead of watt-hours. 

If I ever see any of these Lipo jumpstart packs on sale for $5 at Walmart, I'll scoop em up and see if I can't make myself a nice Frankenstein battery.
```

---
## \#17 Posted by: cryzies Posted at: 2016-09-16T20:52:21.881Z Reads: 181

```
<img src="/uploads/db1493/original/3X/6/f/6f92c9fc1665778f8d60c2ca5dbd9e7158504a56.png" width="281" height="500">

So these are lipos. 18000 mAh most likely be 3p so ~6000 mAh (exaggerated) per parallel or 4p, ~4500 mAh per parallel. 6000*20C*3packs=360A discharge continuous 6000*30C*3packs=540A discharge burst. Seems close enough. Probably is a 3S with a max voltage of around 12.6 volts. So a 3s3p? Did I calculate everything correctly? 9lipos for $60 doesn't seem that bad!

By the way, something has been bothering me, I can't wrap around the thought of him getting around on just 12V. He must be drawing a lot of amps.
```

---
## \#18 Posted by: jtkharatmal Posted at: 2017-03-10T14:32:33.223Z Reads: 121

```
Guys I m also trying to figure out if this can be a replacement to the traditional Lipo pack. I know I m late by a few months but i stumbled upon this video today and I m just at the assembling stage of my board. So m trying to figure out if the jump starter is a good option to use? here I m getting a jumpstarter with a 50,000mAh capacity and a 60,000mAh capacity  - how many cells would that be? 
Link to the jump starters given below.
http://uae.souq.com/ae-en/50000mah-multi-functional-auto-car-jump-starter-emergency-power-bank-charger-7722435/i/

http://uae.souq.com/ae-en/howin-compact-compressor-and-jump-starter-power-bank-88000mah-k50-8928625/i/

which one should i go for considering I have a 120A 1/8th Scale Sensored Brushless 2S-6S ESC and an Brushless Outrunner Motor N5065 270KV 1665W. 

kindly help.

regards,
JT
```

---
## \#19 Posted by: jtkharatmal Posted at: 2017-03-10T14:33:21.154Z Reads: 117

```
I cant import Lipos here - and the existing ones are way too expensive
```

---
## \#20 Posted by: s00cl0se Posted at: 2019-06-10T07:47:01.798Z Reads: 31

```
I imported my lipos  a while back, but 2 of my cells oin my lipos are weak. tried to import them but they are not shipping through fedex dangerous goods anymore. 

I am parting out my skateboard, if you are intrested in it , I live in UAE
```

---
