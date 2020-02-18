# First Build / Dual 6355 190KV / 12s3p / Vesc

### Replies: 8 Views: 987

## \#1 Posted by: Ashleyp Posted at: 2017-12-03T20:37:48.497Z Reads: 159

```
Hi this is my first time building an electric skateboard. I'm aiming for 25+mph top speed with a decent ride range of 10+ miles. I weigh just over 100kg hence using dual motors for more torque.
I would like to know if the set up I have gone for would work:
-Deck: 38 inch drop through deck
-Motors: Dual 6355 190KV torque boards motors ()
-Battery: 12s3p, should i build my own so that I can choose the arrangement and what Lipos i can use or buy it pre built as it's my first time?
-Remote: 2.4Ghz nano remote controller
-Receiver: 2.4Ghz mini receiver
-Motor mounts/pulleys: Dual motor mechanical kit () with 83mm wheels, 63mm motor mounts, 36T wheel pulley, 16T motor pulley and 265mm High torque timing belt (Do I need wider rear trucks?) and I'm aiming for a 65mm center distance
-BMS: 36V 100A LiFePo4 Battery BMS LFP PCM SMT System 12S 12x 3.2V eBike Battery 12x3V (Does it need to be 100A rated or would 80A do?)
-Charger: 36V 43.8V 5A LiFePo4 Battery Charger 12S 12 x 3.2V LiFe Charger High Performance
-Vesc x2: I am planning to make my own Vesc by taking a PCB design and having it custom made, i will then solder on the components myself and load the program needed. Something along these lines http://vedder.se/2015/01/vesc-open-source-esc/ any notes or things to account for would be much appreciated :) 
-Battery display: 2016 Battery Capacity Tester Indicator for 12V 24v 36v 48v CAR Lead-acid lithium
- I also plan to have an external power switch and potentially put in a fuse (Not too sure on what amp rating and where it would need to go)
Thanks Ashley (Sorry if I've posted in the wrong section)
```

---
## \#2 Posted by: willpark16 Posted at: 2017-12-03T21:44:02.464Z Reads: 137

```
Curious, what is the purpose of the college project
```

---
## \#3 Posted by: Ashleyp Posted at: 2017-12-03T21:51:41.284Z Reads: 135

```
It's long winded but effectively design and make an improved version of a product available on the current market but we got to choose what we wanted to do and it had to be related to electronics.
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-12-03T21:52:15.114Z Reads: 135

```
That charger is designed for 3.2v lithium iron phosphate cells, and is not compatible with 3.7v lithium-ion or lithium-polymer cells. I'd recommend going with a prebuilt pack, or lipos, rather than trying to make a custom pack out of 18650 cells. 

You'll also need a BMS unless you plan to use a balance charger.
```

---
## \#5 Posted by: willpark16 Posted at: 2017-12-03T22:09:16.092Z Reads: 127

```
Sweet, to make the vesc u will need smd soldering if recommended a hot bed, and a battery that is done with lipos may be easier
```

---
## \#6 Posted by: Ashleyp Posted at: 2017-12-03T22:30:01.109Z Reads: 117

```
Okay I'm thinking of:
- battery: 44.4V 9Ah 18650 battery pack 12s3p (https://www.alibaba.com/product-detail/Powerful-electric-skateboard-battery-44-4V_60677725899.html?spm=a2700.7724857.main07.21.213dd662061D0i)
-BMS: 45V 44.4V 12S 90A Lithium ion Li-ion LiPo NMC Battery BMS PCB System Ebike (https://www.ebay.co.uk/itm/45V-44-4V-12S-90A-Lithium-ion-Li-ion-LiPo-NMC-Battery-BMS-PCB-System-Ebike-RARE-/122773818395)
and I can't seem to find a good charger at the moment but i'm going to go with a 4A fast charge one
```

---
## \#7 Posted by: Ashleyp Posted at: 2017-12-03T22:44:05.007Z Reads: 106

```
That's a good shout cheers :)
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-12-03T23:02:40.473Z Reads: 103

```
I don't know if you noticed this, but the minimum order for that battery is 10 packs. Be careful with alibaba/aliexpress packs, they often come with cheap/no name cells with low discharge current.
```

---
