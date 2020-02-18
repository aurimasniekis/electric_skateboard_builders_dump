# Skateboard Deck Build &#124; $250 &#124; 6s 10000mAh &#124; Big Foot 245kv &#124; DIYEBOARD V1.1 ESC

### Replies: 11 Views: 1381

## \#1 Posted by: loco_motive Posted at: 2018-07-14T12:19:02.202Z Reads: 126

```
Hey everyone,
After doing some more research, I've settled on the following parts for my first build.  I already have 2x 6s 5000mAh Zippy Compact, a Tacon Big Foot 160 245kv motor, and a charger so that saves some money.  I wanted something a little cheaper/shorter/more unique than your typical eboard to use at college.  I found comsa42's Instructable and was inspired:
http://www.instructables.com/id/Electric-Skateboard-v20/

**ESC + Remote ($68 shipped):** 

http://www.diyeboard.com/v11-single-belt-motor-sine-wave-foc-esc-speed-controller-p-523.html

**8" Skateboard Deck ($18 + shipping):** 

https://www.skateshred.com/blank-skateboard-decks-pro.html

**Caliber II Trucks ($40 shipped):** 

https://www.amazon.com/Caliber-Trucks-Cal-50%C2%B0-Longboard/dp/B00NY3Q5Q8/ref=cm_cr_arp_d_product_top?ie=UTF8&th=1&psc=1

**97mm Flywheels ($30 shipped):** 

https://www.ebay.com/itm/Cal-7-97mm-78A-Longboard-Flywheel-Skateboard-White-Wheels-Free-Bearings/362084301124?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D2%26asc%3D52935%26meid%3D4bf0bf5be87048f78a2a0a2c053844f8%26pid%3D100623%26rk%3D4%26rkt%3D6%26sd%3D362084294452%26itm%3D362084301124&_trksid=p2047675.c100623.m-1

**Extras:**
- Griptape, 1/2" risers, hardware, and shipping for deck for $32 from skateshred.com
- 2x HTD 5M 10mm belts for $8 shipped from ebay.com
- Battery Level LCD and stickers for sticker bomb for $10 shipped from aliexpress.com
- Motor mount, pulleys, and electronics enclosure will be 3D printed

Drew it up on Solidworks.  Everything is to scale. (I only modeled the electronics box, the motor, and a quick mount for concept.  The rest I found on grabcad.com to save time):

![post1low|640x360](upload://4brvTR6cq20oCYuckbMcMO9cRZa.JPG)

![post2low|640x360](upload://qvk6Jz6yI6Ww0CYqLXxVC23E0x5.JPG)

![post3low|640x360](upload://dEKY7UQbWbJAIhjvI8Hn8qW2Khs.JPG)

Might have to cut the board like this if there's wheel bite:
![post4low|640x360](upload://3PbXH0W63bLH9N5Hog1feJjb0h.JPG)

Will be updating with progress.  Thanks for looking!
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-07-14T12:34:32.946Z Reads: 107

```
looks great! look forward to seeing some updates on this!
```

---
## \#3 Posted by: marsrover001 Posted at: 2018-07-14T12:52:22.723Z Reads: 98

```
Make sure you have a loud lipo beeper. The diyeboard esc can take 12s, but won't have the low voltage cutoff or accurate remote battery readings.
```

---
## \#4 Posted by: loco_motive Posted at: 2018-07-14T12:53:56.104Z Reads: 96

```
Didn't think about that.  I'll definitely add that to the list, thank you!
```

---
## \#5 Posted by: Grozniy Posted at: 2018-07-14T13:05:58.825Z Reads: 85

```
That esc is rated at 10s max. Did someone test it with 12s? If you go 10 or 12s, that motor will hit erpm limit and ESC might bip always and not work. I would recommend going 6s or getting a <200kv motor.
Edit: also u might not have enough torque with high kv
```

---
## \#6 Posted by: marsrover001 Posted at: 2018-07-14T13:07:46.167Z Reads: 81

```
I have run a v1 esc on 12s. Tourque improvement, but hardly any top end boost. I think it's properly limited. Just give it good cooling as it gets slightly warmer than 10s.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-07-14T13:13:26.130Z Reads: 75

```
Yep, I can say that 12s worked fine for me. The top speed won’t increase though due to the rpm limit set at 6400
```

---
## \#8 Posted by: Grozniy Posted at: 2018-07-14T13:20:29.655Z Reads: 74

```
So what's the best I've for that esc on 12s?
```

---
## \#9 Posted by: pat.speed Posted at: 2018-07-14T13:22:49.270Z Reads: 74

```
6400/ (12x4.2) = roughly a good kv
```

---
## \#10 Posted by: loco_motive Posted at: 2018-07-14T13:41:12.190Z Reads: 73

```
I’ll be using 6s so I can use the motor and batteries I already have (my dad used to fly rc planes and had them sitting around).  If I like it enough I’ll upgrade.  Also, you have to choose between 6s, 8s, or 10s when you order.  Are the boards actually different from each other?  I’d like to be able to upgrade to 10s later down the road
```

---
## \#11 Posted by: Grozniy Posted at: 2018-07-14T13:59:26.572Z Reads: 72

```
It's the same board but with 2 wires soldered in different places. You can just resolder to change voltage.
Ask @dickyho for more info
```

---
