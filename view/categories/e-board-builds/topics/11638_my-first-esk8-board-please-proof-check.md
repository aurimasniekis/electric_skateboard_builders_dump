# My first esk8-board - please proof check!

### Replies: 11 Views: 1392

## \#1 Posted by: StraightThrough Posted at: 2016-10-21T19:31:13.118Z Reads: 110

```
**hey fellas!**
im new to this sport and want to build an electronic skateboard for daily commute myself.
Please have a fast look over my listed componentes and tell me what doesnt work, im open for any kind of critic!
I want to build a Dual Rear Motor Longboard:

[This is the VESC (2x)](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)

[This ist the battery (1x)](diy-electric-skateboard-kits-parts/electric-skateboard-battery-epower-pack-6s2p/?attribute_type=EPOWER+PACK+6S2P+w%2F+2A+Charger)

- 6S2P
- Length 225mm (w/ 80amp fuse = 280mm)
- Width 150mm
- Height 22mm

[UPDATED: This is the motor (2x), i want them both between the wheels -> under the deck](https://eu.electric-skateboard.market/product/190kv-sensored-motor-6354-6374/)

- 6354 190KV
- Max Power: 2500 Watts
- Max Amps: 80 Amps
- Max Volts: 12S

[This is the motor kit i'd use](diy-electric-skateboard-kits-parts/torqueboards-dual-motor-mechanical-kit/?attribute_motor-mount-size=63mm+Motors&attribute_wheel-color=83mm+Orange&attribute_motor-pulley=13T+HTD5+12mm+Motor+Pulley)

[This is the Can Bus to connect the VESC's](diy-electric-skateboard-kits-parts/vesc-canbus-connector/)

[This is the XT90 connector to connect the VESC's with the battery](diy-electric-skateboard-kits-parts/dual-vesc-xt90-parallel-connector/)

I will buy additionally a Wii Nunchuck Nyko Kama from one guy here in the forum :slight_smile: , prepared for esk8ing!

[Additionally i will buy this mini USB cable to connect my VESC's with my PC](diy-electric-skateboard-kits-parts/mini-usb-cable/)

I'd fix the stuff under my deck with big hook&loop stickers and tape!

Im not sure yet which deck i should use:
[**Olsen&Hekmati d97**](https://www.skatedeluxe.com/de/olson-hekmati-d97-composite-38-19-97cm-longboard-deck_p51659?sort=relevance&count=240&cPath=150)

- construction: laminated birch core, fiberglass, carbon

- length: 97 cm  

- width: 23 cm 

- wheelbase: 70 cm

- concave: medium (12 mm)

- flex: medium -> i am 73kg

- truck mounting: topmount  

OR

[**Loaded Vanguard Flex 3**](https://www.skatedeluxe.com/de/loaded-vanguard-38-42-98-107cm-longboard-deck_p14985?keywords=vanguard)

- construction: Epoxy and Tri-axle fiberglass sandwich a vert-lam bamboo core

- length: 98cm

- width: 21.5cm

- wheelbase: 94cm

- flex: 3 (68-90kg) -> i am 73kg

- truck mounting: topmount  

Im COMPLETE noob on electronics, i just have figured how to connect everything.
_Do you know which deck i shall use?_
_Can you tell me weaknesses of my setup?_
```

---
## \#2 Posted by: ajaynagra Posted at: 2016-10-21T19:43:05.142Z Reads: 96

```
The deck that your using is great but you will need to think about your enclosure design.

European Motors
https://eu.electric-skateboard.market/product/190kv-sensored-motor-6354-6374/
```

---
## \#3 Posted by: Spek Posted at: 2016-10-21T19:55:35.238Z Reads: 91

```
I have those motors and their 10s4p  pack and highly reccomendation both. Excellent customer service as well. For your first build I'd get some vesc insurance they sell just incase.
```

---
## \#4 Posted by: StraightThrough Posted at: 2016-10-21T20:05:55.525Z Reads: 84

```
yea i have to build something around it later  for enclosure

are you using these motors you've linked?
they are cheap! how is the quality?
```

---
## \#5 Posted by: StraightThrough Posted at: 2016-10-21T20:07:09.072Z Reads: 81

```
what could go wrong to crash them? overpowering or overheating or smth?
```

---
## \#6 Posted by: ajaynagra Posted at: 2016-10-21T20:12:49.282Z Reads: 81

```
They are great quality. They're very similar to DIYS

there was a group buy for them 

@JLabs

http://www.electric-skateboard.builders/t/6354-6374-stealth-motor-group-buy-part-2-rotating-light-rocket/8828
```

---
## \#7 Posted by: Spek Posted at: 2016-10-21T20:36:16.440Z Reads: 70

```
More than anything new user error seems to be an issue, from what I've read. As a total noob myself, I had no issues setting up my ollin vescs. After reading some how-to threads it was very easy. But it is possible to mess up your own vesc if you input the settings wrong. I've also read they're unstable in FOC mode so I've never bothered to try it. 

However, a balanced build with correct settings shouldn't have any problems. I went with a 10s4p battery because it was the most recommended setup for a vesc and 190kv motors. BTW, I'm not an expert on this subject. I actually sent Dexter my shopping cart from his site and asked for his input before I purchased which helped clear up some of my beginner confusion. I recommend reading as much on the forum as you can.
```

---
## \#8 Posted by: StraightThrough Posted at: 2016-10-21T20:44:11.730Z Reads: 64

```
ok thanks for the feedback

i will try without insurance, i've some clear guide how to set up VESC

but if i fail and have burned my first VESC ill tell you ^^
```

---
## \#9 Posted by: Namasaki Posted at: 2016-10-23T17:55:28.188Z Reads: 58

```
190kv is low for 6v
Better to go 10s with 190kv. 
It's a good combo that will get you 25mph
And good range. 
6s 2p will prob only get around 5 miles
10s 3p would likely go 15 miles
It's well worth the extra cost if you can swing it.
```

---
## \#10 Posted by: StraightThrough Posted at: 2016-10-23T21:59:33.138Z Reads: 57

```
do you know a specific battery?
do you mean like 10s3p or just 10s ?

[could i build this (2x) in parallel?](http://www.gensace.de/find-batteries-by-voltage/lipo-6s/gens-ace-6000mah-22-2v-35c-6s1p-lipo-battery.html)

- Product Type: lipo battery pack

- Capacity: 6000mAh

- Voltage: 22.2V

- Max Continuous Discharge: 35C (210A)

- Max Burst Discharge: 70C (420A)

- Weight: 874.60g

- Dimensions: 145*45*59mm 

- Balance Plug: JST-XHR

- Discharge Plug: EC5 

- Charge Rate: 1-3C Recommended, 5C Max
```

---
## \#11 Posted by: Namasaki Posted at: 2016-10-23T22:31:47.027Z Reads: 50

```
2 of those would be 12s which is too high for 190kv motor with Vesc. 
You could get a 10s3p battery pack from Diyelectricskateboads.com
Or you could use 2 5s Lipos. 
But if you use Lipos, you'll need a balance charger and you should stay with a known brand like Turnigy
```

---
