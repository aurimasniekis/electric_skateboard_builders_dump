# Mid-range pintail &#124; 1x 260kV &#124; Turnigy VESC &#124; 8s1p &#124; Belt drive &#124; unique wobble suppression

### Replies: 32 Views: 837

## \#1 Posted by: Matrom Posted at: 2018-07-25T04:01:42.353Z Reads: 196

```
Hello :raising_hand_man:
Reading on this forum has been spectacular so far. I'm building my first esk8 which will fit in a half-locker at my university's gym. It'll have a knock-off pennyboard deck that I already own... I'll be fine! 

**Could someone please do a sanity check on my parts list?**

1x Zippy compact 6s 5000mAh
https://hobbyking.com/en_us/zippy-compact-5000mah-6s-25c-lipo-pack-xt90.html


KEDA 195kV outrunner
https://hobbyking.com/en_us/kd-53-20-brushless-outrunner-195kv.html

X-Car Beast 120A
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html

Pulleys
https://www.ebay.ca/itm/DIY-Electric-Skateboard-ABEC-Flywheel-Pulley-Kit-15mm-Wide-Belts/112736539417?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

Charger
https://hobbyking.com/en_us/turnigy-accucel-6-50w-6a-balancer-charger-w-accessories.html

Mount
https://hobbyking.com/en_us/motor-mount-5.html

Trucks and wheels
https://www.ebay.ca/itm/Cal-7-Longboard-Flywheel-180mm-Truck-Bearing-83mm-Black-Skateboard-Wheels/263173290839?hash=item3d4659bb57%3Ag%3APaoAAOSwkthZpH03&_sacat=0&_nkw=83m+longboard+wheels&_from=R40&rt=nc

I don't have much room under the board for parallel batteries; online calculators estimate ~10km. The calculator also spit out a measly 18.5km/h loaded max speed. Max road grade of 70%. My thoughts:

1. I do not want loads of speed anyways on this minimized deck; want to replace kicking and a little bit more
2. This config gives me peace of mind with the medium hills in my area... right?
3. This can get me to my gym back and forth 3x in one charge, that's not bad

The reason I'm using a noisy-braking x-car instead of [this guy](https://www.ebay.ca/itm/Single-Brushless-Motor-Controller-ESC-Replace-for-Electric-Longboard-Skateboard/122838106470?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D2%26asc%3D40971%26meid%3Dd1ef20a1013e4da19ebb0325ab0eaa39%26pid%3D100005%26rk%3D5%26rkt%3D12%26sd%3D142860298598%26itm%3D122838106470&_trksid=p2047675.c100005.m1851) from ebay, is because I want the ability to control my PWM from a microcontroller.

That brings me to the feature which may or may not have been implemented in the past. I will interface an MPU 6050 gyro to measure angular velocity on the roll-axis to characterize, detect, and suppress speed wobble by applying the brakes. I have the general pipeline in mind and I can't wait to start prototyping! 

How concerned should I be about footbite on this small deck?

Thanks a million!!1! :pray:
```

---
## \#2 Posted by: Grozniy Posted at: 2018-07-25T04:16:32.983Z Reads: 165

```
Hi there and welcome.
Get a higher C battery, like 60C at least to minimise sag.
It will be a huge pia to adapt the mount on those trucks. If using that mount, go with their trucks. But with their trucks, you can't use that eBay wheel pulley unless you shave inner diameter by 3mm. Also that 11T motor pulley is complete garbage, it feels light as paper. Get another one.
How about enclosure?
If you want to go for cheap but still rideable, you could buy pretty much everything from @dickyho [Here](https://ebay.com/usr/eboard-shop) & [Here](https://ebay.com/usr/dickyho2015)
```

---
## \#3 Posted by: kalebludlow Posted at: 2018-07-25T04:22:03.854Z Reads: 163

```
One thing I noticed is the mounts. They are designed to have 63xx motors mounted to them, while the motor you have is 5663. You are already buying mounts from Hobbyking, why not also get one of their motors? You could also get a VESC instead of that X-Car ESC and take advantage of customizability as well as using sensored if you were to buy those. 

Of course all of this involves increasing budget and I can understand your reluctance to do so
```

---
## \#4 Posted by: Matrom Posted at: 2018-07-25T04:32:20.903Z Reads: 150

```
Thanks for the response! I will cart a different battery.
Hm, looks like Turnigy's trucks are sold out, do they re-stock if it doesn't say 'back-order'? Any suggestion for a truck variety? Just for my own understanding, what is your concern with the ebay trucks?

Also for my understanding, what do you mean by light as paper? How do you know it's trash? Own one?

Thanks!
```

---
## \#5 Posted by: Matrom Posted at: 2018-07-25T04:35:08.886Z Reads: 148

```
Looks like the KEDA has two sets of face mounting holes, will they not work with the mount? Hard to say without a technical drawing.

Edit: Oh, I see. The outermost holes of the KEDA are not as far out as the mount's. Any objection to this motor as a replacement? 
https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html
```

---
## \#6 Posted by: kalebludlow Posted at: 2018-07-25T04:51:37.180Z Reads: 135

```
That one looks good to me
```

---
## \#7 Posted by: sunnyD Posted at: 2018-07-25T05:25:44.188Z Reads: 140

```
One thing to consider is that even though you may be comfortable on a penny board at your current speeds of push riding, if your purpose of converting the board is to become more efficient in travel, you may have a a problem on your hands. Even at only five mph higher, a really small board (such as a penny) the board is often referred to as a "death stick" for the reason that they often don't handle well and are unstable. Now I am not a shortboard hater, I am constantly trying new trucks, wheels and different deck sizes in order to make a shortboard that suffers less of thee downsides. Until somebody comes up with a better way, the perceivably only way you are able to ride you board is at only slightly higher speeds than the speeds you have already been doing. So my suggestion is to measure your locker and then find the largest possible board you can fit in it as because, sadly, bigger is better. (or hell, maybe even a folding Eboard?) Gl on your build!
```

---
## \#8 Posted by: dareno Posted at: 2018-07-25T07:59:30.160Z Reads: 119

```
My friend stick to the tried and tested vesc please and messing around with a gyro that will correct your braking when leaning is a surefire way of making like superman.  Be careful please.
```

---
## \#9 Posted by: dareno Posted at: 2018-07-25T08:12:49.142Z Reads: 119

```
Also go for a graphene lipo.  As high an ah and c rating as you can get. those turnigy graphenes are in a different league when dealing with sag.  2 years ago I re-purposed an old lead acid fiik board with 2 3s graphenes a 280 kv brushless and a mamba max car esc.  It was very pedestrian compared to current tech but almost zero voltage sag.  braking was either on or off though and accelerating while moving was a snatchy experience.  Use vescs and if you are going to use lipos then graphenes all the way. Really not sure about the gyro though but hey I'm sure people were like mate don't do it to Mr Vedder in the beginning.  Good luck!
```

---
## \#10 Posted by: pat.speed Posted at: 2018-07-25T08:16:43.393Z Reads: 108

```
The previous motor actually is a 6356 motor, HobbyKing have just mislabeled it on their website. I have two of them on my dual board.

Edit: all of the parts will work fine. That is almost the exact same as my first build. 

I have experience with these parts and would reccomend you to get that eBay esc instead or a Vesc. Also like others have said the mount will be hard to fit to the trucks, so either another mount is needed or different trucks. Also that battery will be fine for a low power board like this. Good luck
```

---
## \#11 Posted by: Grozniy Posted at: 2018-07-25T08:43:26.497Z Reads: 100

```
[Here](7.25inch Black Skateboard Trucks Aluminium Longboard Bridge Skateboard Parts Skate Board Trucks  http://s.aliexpress.com/z67n2IVj?fromSns=Copiar para a área de transferência) you go HK trucks. I don't have concerns about durability,  only about which Riptide bushings can you upgrade to, ask Brad @Alphamail. 
I had the kit, motor pulley is trash, no quality at all.
```

---
## \#12 Posted by: Grozniy Posted at: 2018-07-25T08:46:16.445Z Reads: 94

```
I have this motor, I had HK mount. I managed to mount 6364 keda to it but the circlip on the shaft doesn't fit the opening on the mount. So the only solution was to get 17mm bolts I think and at washers between the mount and motor to create space for circlip. Also you'll need to file 2 flat spots on the shaft for knurled point grub screws
```

---
## \#13 Posted by: Skunk Posted at: 2018-07-25T08:55:47.163Z Reads: 98

```
Throwing wide reverse Kingpin trucks on a penny board is going to feel really awkward and probably have a weird turning radius. 
If this is what you want to do I would highly recommend trying to borrow a pair of longboard trucks from a friend and throw them on your penny board and just try rolling around on it for an afternoon.
With something as small as a penny board, Hub Motors would save you a ton of space for mounting under the deck.
```

---
## \#14 Posted by: bartroosen12 Posted at: 2018-07-25T08:55:59.513Z Reads: 93

```
Yeah I should also go for thr ebay esc instead of the car esc. It's smoother and cheaper
```

---
## \#15 Posted by: Skunk Posted at: 2018-07-25T09:17:31.751Z Reads: 105

```
@Matrom are you set on the penny board merely because you have it and it'll fit in your locker or are you really wanting a epenny board ?
Would something the size of one of the oversized penny boards work?
I have a practically brand new arbor pocket deck not getting used.  I'd be willing to hook you up with it for cheap if you thought it would help.
```

---
## \#16 Posted by: Matrom Posted at: 2018-07-25T11:38:13.153Z Reads: 96

```
@Skunk just for the compactness. Here’s an image for reference:
![image|281x499](upload://hkdApyBMV6XJ62RiJy5SU22Oqnc.jpeg)

A folding board would work too and would look super dope and I might just save my neck. That raises more questions like should I saw my pintail in half or go buy some baltic birch wood like others on this forum.
```

---
## \#17 Posted by: Skunk Posted at: 2018-07-25T11:41:56.966Z Reads: 94

```
Damn that's a small locker....
```

---
## \#18 Posted by: pat.speed Posted at: 2018-07-25T11:46:45.112Z Reads: 97

```
That's the same sized lockers I have to use at school :( Anyway may I recommend you a BMS. It will end up being the same price or cheaper than that other charger and will be a lot more convenient. It might be hard to wire at first but then will only require one plug to charge. 

Cheap BMS modules can be bought on eBay or amazon for really cheap ($15). Just make sure that the overcharge feature is at 4.2v and that it balances the cells at 4.2v as well otherwise it may harm the cells. 

Good luck with the build and I want to see how it turns out as I've got a similar build coming soon
```

---
## \#19 Posted by: TarzanHBK Posted at: 2018-07-25T11:59:34.408Z Reads: 95

```
I´m doing the same thing soon with my pennyboard for fun and science!
Get a cheap hub motor with axle from china, use a vesc, use something like a 6s2p out of 30Qs and you have one of the lightest and coolest cruisers around.
```

---
## \#20 Posted by: Matrom Posted at: 2018-07-25T12:12:40.237Z Reads: 93

```
Is [this esc](https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.ca%2Fulk%2Fitm%2F322688416729) not a vesc? I only ask because I need to control using a micro controller, I’ve seen this done on the forum with vesc+arduino+uart 
Thanks!
```

---
## \#21 Posted by: pat.speed Posted at: 2018-07-25T12:20:21.873Z Reads: 90

```
Nope that’s not a Vesc, it’s the esc used in most cheap premade boards from overseas. It’s honestly pretty decent but not nearly as good as a Vesc.

 Why do you need to control it with an arduino? If it’s for the braking feature I would highly recommend not implementing it as it seems like it might make matters worse. If your trucks are starting to wobble and you change the forces from accelerating to braking the truck will be jerked by the motor changing speed/direction most likely resulting in a large wobble before slowing down. It’s not impossible and encourage you to try but I feel as though it may not help. 

On the other hand something that locks the truck in a straight line when wobbles occur might be beneficial
```

---
## \#22 Posted by: Matrom Posted at: 2018-07-25T17:46:00.647Z Reads: 83

```
Updated parts list! If someone has a moment, please look over:

https://hobbyking.com/en_us/turnigy-sk8-6354-260kv-sensored-brushless-motor-14p.html

2 X 
https://hobbyking.com/en_us/turnigy-heavy-duty-5000mah-4s-60c-lipo-pack-w-xt-90.html

https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html

Trucks
http://s.aliexpress.com/z67n2IVj?fromSns=Copiar

Same mount. No penny deck, going to make a foldy boi.
Any suggestions for an affordable BMS?
```

---
## \#23 Posted by: HillRipper21 Posted at: 2018-07-25T18:44:49.086Z Reads: 74

```
Damn, was interested to see how a penny board with those parts would end up, I was thinking of doing something similar in the future.
```

---
## \#24 Posted by: Matrom Posted at: 2018-08-18T04:15:52.926Z Reads: 71

```
Lots of parts arrived! Unfortunately, I’m going to have to do some filing/grinding ![image|374x500](upload://bOP8VeWzQxv97m5O6bqGq2ZymzM.jpeg)
```

---
## \#25 Posted by: Grozniy Posted at: 2018-08-18T04:30:45.529Z Reads: 69

```
What else arrived? Links?
```

---
## \#26 Posted by: Matrom Posted at: 2018-08-18T04:43:46.520Z Reads: 73

```
Everything is linked above :D 
![image|374x500](upload://jttrubFV4sB5c7hyUMkzKzgtazp.jpg)

Trucks and wheels are on, zippys and vesc is mocked up in the photo, the 260kv sensored is mocked up on the Hobbyking mount

I’m going to have to file down this fillet to fit the mount better:
![image|393x500](upload://7sCybpCSoelMWrdj28F2004zmb5.jpeg)

Grozniy, at what point did you find out the pulley is bad? Perhaps I just can’t tell good quality apart from bad, but it looks ok to me so far
```

---
## \#27 Posted by: Matrom Posted at: 2018-08-18T04:47:07.409Z Reads: 71

```
Cheapo 8s BMS is here
![image|374x500](upload://b3eWD2IJ2SSvgDkz7lqluCgudkh.jpg)
but my charger might take a couple more weeks to ship in :( 
![image|281x499](upload://rZNGu6VrTTUarECpO7oFp0WSqLH.jpg)
```

---
## \#28 Posted by: Grozniy Posted at: 2018-08-18T08:19:34.694Z Reads: 60

```
The motor pulley is bad because it's very light meaning the metal is not strong and will skip the belts after some use.
```

---
## \#29 Posted by: pat.speed Posted at: 2018-08-18T13:07:33.771Z Reads: 55

```
I’m sure it will last fine for the time being. Cool build btw
```

---
## \#30 Posted by: Matrom Posted at: 2018-08-18T21:38:42.568Z Reads: 52

```
My dad convinced me to stick with my pintail deck for the time being, also first day of work completed! 

![image|374x500](upload://v29SpDyAAOcs9lAa39KTcalezlW.jpeg)

![image|233x411](upload://s8zJxo3T0RxL0EuWtmW2WIzu5V9.jpeg)
```

---
## \#31 Posted by: Matrom Posted at: 2018-08-28T05:22:14.275Z Reads: 40

```
Hey! Could someone please glance over my electrical diagram before I start soldering? Thanks a million!
![image|666x500](upload://h7BNeCzCpW0pzwAOAbwdnbnHzuv.jpg)
```

---
## \#32 Posted by: Matrom Posted at: 2018-08-28T05:35:23.756Z Reads: 38

```
Added another xt90 after the series adapter
```

---
