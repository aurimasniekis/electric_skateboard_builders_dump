# Looking for 100W buck converter

### Replies: 25 Views: 231

## \#1 Posted by: ZachTetra Posted at: 2019-04-04T20:21:55.529Z Reads: 66

```
Gonna make an aux power bus for my longboard, need 5v to run Arduino/addressable underglow/LED headlamps/phone charger.  Estimate is 20A (15A for lights and 5A for electronics).  Battery is 12s li-ion

Where can I get one/how can I make one?  ~$30 limit

The best I found would be 2 of these for $34, anyone know anything better or can validate this one?
https://www.amazon.com/uxcell-Converter-Regulator-Waterproof-Transformer/dp/B01ENT1KCU/ref=mp_s_a_1_8?keywords=5v%2B10a%2Bdc-dc&qid=1554409472&s=gateway&sr=8-8&th=1&psc=1
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2019-04-04T20:36:54.394Z Reads: 59

```
https://www.aliexpress.com/item/Free-Shipping-High-Quality-Step-Down-DC-DC-Converter-Regulator-24V-Buck-TO-12V-20A-240W/32518020047.html?spm=2114.search0104.3.1.2d4616c8LBctWD&amp;ws_ab_test=searchweb0_0,searchweb201602_9_10065_10068_10130_10547_319_10059_10884_317_10548_10887_10696_321_322_10084_453_10083_454_10103_10618_10307_537_536,searchweb201603_51,ppcSwitch_0&amp;algo_expid=ca2a9522-4979-4c3e-b41a-a0898bb7a417-0&amp;algo_pvid=ca2a9522-4979-4c3e-b41a-a0898bb7a417&amp;transAbTest=ae803_5
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2019-04-04T20:41:29.149Z Reads: 53

```
Just be aware that those thing are F.... huge 

That is a 10A

![image|375x500](upload://gMSkqXYNHdZsGPOjSflViA0qVSv.jpeg) ![image|666x500](upload://1tO6BGEUW3p513uKYe3cXYdCPXl.jpeg)
```

---
## \#4 Posted by: Mich21050 Posted at: 2019-04-04T21:05:34.783Z Reads: 45

```
[quote="ZachTetra, post:1, topic:89374"]
15A for lights
[/quote]

What kind of lights are you going to use? \
To me, 15A (75W) for lights seem a bit excessive.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-04T21:06:48.410Z Reads: 43

```
[quote="Mich21050, post:4, topic:89374"]
15A for lights seem a bit excessive.
[/quote]

not..... lights a super important, the brighter your lights are, the better, just to show drivers not to mess with you
```

---
## \#6 Posted by: Mich21050 Posted at: 2019-04-04T21:09:05.764Z Reads: 41

```
Your right about that. But I'm using ws2811b led`s and they are really bright and they draw minimal current (need to find my notes). :slight_smile:
```

---
## \#7 Posted by: wafflejock Posted at: 2019-04-04T21:09:06.801Z Reads: 40

```
I have a 75W panel of 256 individually addressable RGB LEDs here that is bright as the sun when on full power, agree this sounds like a bit overkill for a board.
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-04-04T21:10:14.318Z Reads: 38

```
[quote="wafflejock, post:7, topic:89374"]
overkill
[/quote]

lights are never overkill, i would put 5000 lumen lights on my 13s10p when i finish it just to show drivers who's boss :grinning:
```

---
## \#9 Posted by: ZachTetra Posted at: 2019-04-04T21:12:15.951Z Reads: 36

```
It's 144 neopixels as underglow (full perimeter) and a a light crash bar with 5 high power led arrays (2 headlights and 3 highbeams)

My time of choice for riding is 2am on backroads
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-04-04T21:12:37.417Z Reads: 35

```
[quote="ZachTetra, post:9, topic:89374"]
2am on backroads
[/quote]

hehe i went all the way to 5am
```

---
## \#11 Posted by: ZachTetra Posted at: 2019-04-04T21:14:45.385Z Reads: 37

```
I'm limited to only an hour on the road before the battery is dead...10s 5ah is not enough

All my torque is gone after 30 minutes and it's just a crawl after that
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-04-04T21:15:30.712Z Reads: 33

```
[quote="ZachTetra, post:11, topic:89374"]
5ah
[/quote]

thats nothing, i went though a raptor 2 battery in about 9 miles and im only 115 lbs\
^10s4p = 12ah
```

---
## \#13 Posted by: Mich21050 Posted at: 2019-04-04T21:16:26.520Z Reads: 33

```
Shoot me a pm. I might be able to help you. :slight_smile:
```

---
## \#14 Posted by: AlanZhou Posted at: 2019-04-04T21:16:43.891Z Reads: 34

```
huh? im confused

the raptor hubs is the issue, they drain power like a mofo
```

---
## \#15 Posted by: ZachTetra Posted at: 2019-04-04T21:17:07.142Z Reads: 32

```
I'm using dual 350W hubs otherwise it'd be over in 20 minutes
```

---
## \#16 Posted by: Mich21050 Posted at: 2019-04-04T21:17:39.833Z Reads: 32

```
I just looked up a bunch of ic's and I might be able to design one for him.
```

---
## \#17 Posted by: AlanZhou Posted at: 2019-04-04T21:18:06.772Z Reads: 32

```
[quote="Mich21050, post:16, topic:89374"]
I just looked up a bunch of ic’s and I might be able to des
[/quote]

i might need one too lolz
```

---
## \#18 Posted by: deucesdown Posted at: 2019-04-04T21:58:46.559Z Reads: 28

```
My advice is to use lights that can take 60v. Or at least 24v. Dropping 40v to 5v at 15a is gonna be big hot and prone to failure.
```

---
## \#19 Posted by: ZachTetra Posted at: 2019-04-04T22:11:25.709Z Reads: 28

```
But phone charger and Arduino are 5v anyways and addressable LEDs are 12v or 5v only
```

---
## \#20 Posted by: ZachTetra Posted at: 2019-04-04T22:13:14.057Z Reads: 30

```
Highest I found is 24v
```

---
## \#21 Posted by: deucesdown Posted at: 2019-04-04T22:15:29.806Z Reads: 27

```
those other 5v things are like 1a or less...
```

---
## \#22 Posted by: Mich21050 Posted at: 2019-04-04T22:16:42.208Z Reads: 24

```
It might help if you send a link with regarding the lights you are going to use.
```

---
## \#23 Posted by: Pedrodemio Posted at: 2019-04-04T22:20:38.213Z Reads: 26

```
There are a few high voltage UBEC at Hobbyking, apart form that you could get several LM2556HVS DC-DC converters and use them in parallel (not sure if it's a good idea) or make multiple circuits to not exceed the current
```

---
## \#24 Posted by: ZachTetra Posted at: 2019-04-04T23:27:29.943Z Reads: 21

```
These LEDs as underglow, 50cm down each side with voltage insertin at each end

https://www.amazon.com/BTF-LIGHTING-WS2812B-Individual-Addressable-Waterproof/dp/B01CDTE6Y6/ref=mp_s_a_1_3?keywords=144%2Bpixel%2Baddressable%2Bled%2Bstrip%2B1m&qid=1554419212&s=gateway&sr=8-3&th=1&psc=1

These are the flashlights I'm gonna gut for the headlights, maybe different ones but still similar power
https://www.amazon.com/MODOAO-Zoomable-Handheld-Tactical-Flashlight/dp/B01LW6E1B3/ref=mp_s_a_1_4?crid=1QCHHR48X6AY0&keywords=t6%2Bflashlight&qid=1554420649&s=gateway&sprefix=t6%2Bflashl&sr=8-4&th=1&psc=1
```

---
## \#25 Posted by: wafflejock Posted at: 2019-04-04T23:39:24.833Z Reads: 23

```
I'd check with a multimeter or bench power supply like you can see here to see how many amps you're actually pulling given the brightness and color settings or sequence you plan to use it can change how many amps are needed quite a bit:

https://photos.app.goo.gl/bfiEbdph6U7s98Vt6

https://photos.app.goo.gl/vPCFuTxPFaoXBdzU7

Using this panel: https://www.amazon.com/gp/product/B01DC0IPVU/ref=oh_aui_search_asin_title?ie=UTF8&amp;psc=1

Think I was going for low power but decent brightness in the first photo but at a few amps they are too bright to look at (this is an array of 256, but since I'm only lighting some of them and at I think 25% power here the power consumption is low)  Bottom photo it was I think at 50% and powered off a 5V 4A adapter.
```

---
