# First build/ dual FSESC 6.6 Plus7/ APS 6355S/INR18650-E35/

### Replies: 33 Views: 834

## \#1 Posted by: tex Posted at: 2019-02-25T21:57:33.836Z Reads: 220

```
Hi everybody, i'm Tex, and i really love skateboard and longboard, in this forum i found many interesting things, from electronics, to mechanics, and many many ideas.

I found out eskate, last year in may, i was walking on the street near a beach and i saw an ekate DIY, i was totaly in love, but i didn't know where to start, cause i wasn't an expert about esc, battery, voltage, wheels.

So i discovered this beautiful forum last year, and i bought an used evolve bamboo for start, i was thinking it's better to learn a lot on the forum, before fry many esc and components.

But now guys, i can't sleep in the night, and i'm thinking every day to build a skate by my self

i'm so excited, i think i'm ready to stard, but consider me like a beginner.

For start at home now i have:

-Dual flipsky fsesc 6.6 plus

-Flipsky nano remote controller

-100mm rough stuff wheels and 90mm wheels

- One long island longboard

-40 cells INR18650-35E  samsung

I really don't know if i want to do a 10S2P conf or a 10S4P,  :persevere: i'm thinking about it.
For the motors i will buy two alien power system sensored

https://alienpowersystem.com/shop/brushless-motors/aps-6355s-sensored-outrunner-brushless-motor-190kv-2200w/
gear 15/36 with 15mm belt

my goal is to ride at a cruise speed of 25-30 km/h with, but with also power below the deck.
What do you think about this motor?

The motor mount and the trucks, will be always self made, by cnc milling machine in 6060 t6.

My doubt is about the BMS, i really don't know how is the good one for me, on the 6355S spec i saw MAX Amp 55 per motor, so with two the max will be 105 A, do i need a BMS with more than 100A.

With this two motors with 10S2P or 10S4P with 90mm wheels, which could be the range riding like in eco mode?

The last question is, when you see a motor on the website, like Alien power system, where you have a huge of possibility, and you loose your mind, how can you distinguish a sucker battery motor, from a less sucker motor?

I hope i wrote everything you need to help me, this is the first step, after that i have other many questions about VESC tool, but this is another chapter :grinning:
```

---
## \#2 Posted by: Fraserrazor Posted at: 2019-02-25T22:01:21.701Z Reads: 205

```
This is your max theoretical speed using 100mm wheels

http://calc.esk8.it/#{%22batt-type-lipo%22:0,%22batt-cells%22:10,%22motor-kv%22:190,%22system-efficiency%22:85,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:36,%22wheel-size%22:100}|

Use this calculator to get a good estimate on range although depends on your location, hills etc.

https://calc.3dservisas.eu/
```

---
## \#3 Posted by: Grozniy Posted at: 2019-02-25T22:03:48.611Z Reads: 189

```
I wouldn't get aps motor, get Maytech ;)
```

---
## \#4 Posted by: Fraserrazor Posted at: 2019-02-25T22:08:59.528Z Reads: 189

```
The alien motor you've chosen is not bad but if you want more torque and power try going up to 6374 or 6364 motor which should also give you more power. I am only suggesting this if you're are building your own trucks you have the ability to change axle length to fit these motors in dual drive.

Alternatively try Torqueboards 6355 as thats rated at 2500w
https:///products/electric-skateboard-motor-6355-190kv
```

---
## \#5 Posted by: tex Posted at: 2019-02-25T22:10:31.948Z Reads: 178

```
[quote="Fraserrazor, post:2, topic:85404"]
This is your max theoretical speed using 100mm wheels

[http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":100}|](http://calc.esk8.it/#%7B%22batt-type-lipo%22:0,%22batt-cells%22:10,%22motor-kv%22:190,%22system-efficiency%22:85,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:36,%22wheel-size%22:100%7D%7C)

Use this calculator to get a good estimate on range although depends on your location, hills etc.

[https://calc.3dservisas.eu/ ](https://calc.3dservisas.eu/)
[/quote]

Yes i already used both, but i don't understa a few value:

-How can i choose the Avg. Power Consumption
-How can i choose the efficiency

i have to configure with 7 poles am i right?
```

---
## \#6 Posted by: Fraserrazor Posted at: 2019-02-25T22:13:55.185Z Reads: 157

```
Set efficiency to around 85 percent, I would leave poles as they are (I think its 14 if I am right). Motors don't tend to come with an uneven number of poles. I'd keep the calculator at 12whr as i dont know what route you'd take.
```

---
## \#7 Posted by: tex Posted at: 2019-02-25T22:17:10.507Z Reads: 152

```
ok this is a good starting point
```

---
## \#8 Posted by: Fraserrazor Posted at: 2019-02-25T22:17:11.483Z Reads: 151

```
A safe range for power consumption would be be 7 to 15 whr/km but it doesnt matter too much as its only for one motor.
```

---
## \#9 Posted by: goldrabe Posted at: 2019-02-25T22:40:26.091Z Reads: 149

```
With E35 do you mean Samsung 35E cells?
If so, they are a bit low on the max. discharge the datasheet says 8A continuous and 13A peak maybe you can go a bit higher than that. With those cells I would suggest going 10S4P in this configuration you can draw around 40A. And you would purchase a BMS accordingly to what the max safe discharge of your battery is, in your case max. 40A.

https://lygte-info.dk/review/batteries2012/Samsung%20INR18650-35E%203500mAh%20%28Pink%29%20UK.html

This site has a lot of useful information on batteries. 
Enjoy building.
```

---
## \#10 Posted by: tex Posted at: 2019-02-25T22:48:27.379Z Reads: 143

```
Yes you are right, i have these at home
https://www.orbtronic.com/content/samsung-35e-datasheet-inr18650-35e.pdf

but wait, how do you calculate 40A? sorry i'm a beginner
```

---
## \#11 Posted by: tex Posted at: 2019-02-25T22:48:55.667Z Reads: 131

```
[quote="goldrabe, post:9, topic:85404"]
[https://lygte-info.dk/review/batteries2012/Samsung%20INR18650-35E%203500mAh%20(Pink)%20UK.html](https://lygte-info.dk/review/batteries2012/Samsung%20INR18650-35E%203500mAh%20%28Pink%29%20UK.html)

This site has a lot of useful information on batteries.
Enjoy building.
[/quote]

Yes it has :smiley:
```

---
## \#12 Posted by: goldrabe Posted at: 2019-02-26T11:46:14.819Z Reads: 125

```
When you put your batteries in series you will double the Voltage, if your batteries have a nominal Voltage of 3.6V then you will have 36V with 10 cells in series eg. 10S.
![connecting_series|367x95](upload://eZZYir27hsWEwtC0gh5BNZTCbdh.gif) 
Putting batteries in parallel will double the Capacity. Now you have four 10S packs which have a max discharge rate of around 10A, combine them and your max discharge is 40A.
![connecting_parallel|367x95](upload://dGGB6YMh0wgQMILcjPWnFTFIOe2.gif) 
Search google for batteries in Series and Parallel to find a more comprehensive answer then I gave, the parallel groups not only double the max discharge they also double the the whole capacity of your pack. Your cells have a capacity of 3500mAh or 3.5Ah multiply this by four to get the total capacity of 14Ah.
```

---
## \#13 Posted by: tex Posted at: 2019-03-11T18:50:02.126Z Reads: 109

```
Motors at home :grinning: ![IMG_20190311_194221|375x500](upload://7H06Atq3Yrb99i5idWodC1VHtSm.jpeg) 

![IMG_20190311_194250|375x500](upload://5lCIFYQFyb9q52fbuUcYWDaD9tS.jpeg) 

Really happy :grinning:
```

---
## \#14 Posted by: tex Posted at: 2019-03-11T19:03:24.004Z Reads: 106

```
So i decided for a 10S4P configuration, but two days ago a friend asked me, if i want to sell my INR18650-35, i was thinking why not, cause he already has these cells in other builds.

So if i sell the cells, i want to by the INR18650 30Q 15A, what do you think?
New for new, please if you have any advice, tell me what's the best cells you think, my goal is the quality, not interested in save money on the battery pack
```

---
## \#15 Posted by: goldrabe Posted at: 2019-03-11T21:22:56.591Z Reads: 102

```
Hi,
the 40A is the highest discharge capacity what the 35E cells chemistry is able to provide.
One cell is rated 3.6V 3500mAh @ 8A discharge. Four cells in parallel will multiply your capacity and discharge current by four, 4x3500mAh=14000mAh, 4x8A=36A.
That means you can discharge a 36V(10S)14000mAh(4P)@36A maximum.
here is a graph from mooch where he tested the 35E cell under different loads.

https://www.e-cigarette-forum.com/threads/samsung-35e-3500mah-18650-bench-test-results-a-so-so-8a-battery.773473/

EDIT*
Sorry that was meant as the answer of your PM. 
And go with the Samsung 30Q best bang for the buck.
```

---
## \#16 Posted by: tex Posted at: 2019-03-11T21:43:04.101Z Reads: 92

```
so if i want to change my cells with INR18650-30Q always in 10S4P, i would have:

4x3000 mAh= 12000 mAh  and 4x15A=60A

in this case the maximum discharge will be 60A

thanks again
```

---
## \#17 Posted by: goldrabe Posted at: 2019-03-11T21:50:12.378Z Reads: 94

```
Yes, correct! Plus you can discharge the 30Q´s up to 20A safely. So your pack can deliver up to 80A.

https://www.facebook.com/batterymooch/posts/samsung-30q-3000mah-18650a-great-15a20-batterybottom-line-this-is-a-retest-of-th/2018668968422679/
```

---
## \#18 Posted by: tex Posted at: 2019-03-11T21:57:36.361Z Reads: 94

```
wow amazing cells, ok tomorow i will definitly sell my cells, and buy the 30Q :slight_smile:
```

---
## \#19 Posted by: tex Posted at: 2019-06-18T19:28:08.638Z Reads: 75

```
Hey guys, I was out my country for a long period, now im at home again :slight_smile: , so I sold my old cells, and now a friend of mine, give me 3 amazing battery packs, alls made with sony vtc6.
I don t know for what they are used , but it told me are standard packs in the facrory where he works, like medical products, but I really don t undestand.
In any case now I have two battery packs with 10s2p conf and one 10s4p with a huge and strage connector, he told me the lastone battery pack is capable to discharge all the power in 9 continuos minutes.

So what you think? Now can I try to use the vesc tool just for see my motors running? :slight_smile: 
And can I modify the 10s4p pack to fix on an xt90  connector?![IMG_20190614_160244|375x500](upload://vgz78LMnNQI4PslRMaLmH8o3xdn.jpeg) ![IMG_20190614_160255|375x500](upload://fSDpstPVGXG7jyCNlR0bgTldlIc.jpeg) ![IMG_20190614_160332|375x500](upload://nGJh5cRfzG6UeHO2rwUVPNKb1rY.jpeg) ![IMG_20190614_160337|375x500](upload://6gqH1PrtwqHebkWfYbuqzspP0s0.jpeg) ![IMG_20190614_160345|375x500](upload://i0Hpia52hGw2sqRBJqmIqiGQbg8.jpeg) ![IMG_20190614_160355|666x500](upload://oo4vG7T52R2FZ6xnyUbzpgV48uq.jpeg) 
The 10s2p is on one layer configuration only, the 10s4p is two layer of 20 cells
```

---
## \#20 Posted by: Chase Posted at: 2019-06-19T04:47:59.878Z Reads: 62

```
The wires on the 4p look super thick. You may have some trouble fitting those into a XT90. You could check your motors out but you’ll probably want to mount them and get a switch or loop key of sorts.
```

---
## \#21 Posted by: tex Posted at: 2019-06-19T07:47:02.034Z Reads: 63

```
Im thinking to use the switch button on my flipsky
```

---
## \#22 Posted by: tex Posted at: 2019-12-10T13:05:18.938Z Reads: 44

```
Hi mates, im here again, I was out my country for work, now im come back home and want to finish my skate.

This week I will connect everything to try running the motors, but I have a doubt.

On the Fsesc there are the phase cables marked a1 b1 c1,  and on my alienpower motor I have 3 cable with one red one yellow and one blue.
How I need to conncet everything?
Is it the position indifferent? 
![IMG_20191210_075752|375x500](upload://dAnySrcdZN36mxRCPUCRNLQiIAV.jpeg) 
![IMG_20191210_075730|666x500](upload://cW0foZIgArAWMuN8vW9Cl3QF8zw.jpeg) 
![IMG_20191210_075724|666x500](upload://o099HmnYqNXImyJMJRdBVMxzZ8w.jpeg) 
Im asking this because I will use mt60 connectors, so when the will soldered on I can t change the cable position
```

---
## \#23 Posted by: Komamtb Posted at: 2019-12-10T16:55:40.940Z Reads: 42

```
No difference on the cables, and you can change the motor direction in the vesc toll if you will need to.
```

---
## \#24 Posted by: tex Posted at: 2019-12-10T18:15:37.264Z Reads: 34

```
Ok, but if is indiferent, why there are the different colors?
```

---
## \#25 Posted by: Haze-Gray Posted at: 2019-12-10T19:24:13.501Z Reads: 36

```
 notice vesc wires have no color? i think the different colors indicate where inside the motor the wire is connected but the esc, doesn't care.
```

---
## \#26 Posted by: tex Posted at: 2019-12-10T21:53:37.284Z Reads: 35

```
Yes esc doen't have colors, but it has letters, like a-b-c but if you tell me dosen't care, better, it will be more easy

Thanks Haze
```

---
## \#27 Posted by: tex Posted at: 2019-12-15T12:02:50.725Z Reads: 33

```
Ok guys, im sorry if im making a stupid question, but I looked on the forum, and I understand that I need an adapter connector from the alien motor sensor to connect it to the flip sky single 6.6

Am I right and if yes, wich connector adapter do I need?

![IMG_20191215_125141|375x500](upload://4xIvWAZdHPJGT5uclC1KojDD5wc.jpeg) 
![IMG_20191215_121826|375x500](upload://MqQP2ObjMzxLGMnEeO9m1PLaU2.jpeg) 
This is the sensor from my motor, and where I must connect it on the 6.6?

![IMG_20191215_125121|375x500](upload://hj7yiUYop2cVTpjn9jCFFTkc5bC.jpeg)

For start I will try to programm one motor with a single 6.6 when I will be sure how to work I will put the second motor with the dual 6.6
```

---
## \#28 Posted by: tex Posted at: 2019-12-15T12:41:10.040Z Reads: 33

```
i'm thinking to swap the alien connector, and use the female connector from the flipsky kit, but i don't know what the alien colors mean.

i need to know
V+ color
TEMP MOTOR color
HALL 1
HALL 2
HALL 3
GND
But on the alien power website, there is no info about that
```

---
## \#29 Posted by: tex Posted at: 2019-12-15T18:53:41.914Z Reads: 32

```
ok guys, i think i found the solution.
https://alienpowersystem.com/shop/rc-ev-accessories/wires/aps-sensored-motors-to-ev-esc-compatible-with-vesc-sensor-lead/
This is the cable that i need i don't know way didn't see it before on the website
```

---
## \#30 Posted by: tex Posted at: 2020-01-02T15:03:09.361Z Reads: 28

```
Today im very happy, I tryed one motor on the table with one esc, and everything is going well.
I know it s nothing special, but it was my first time that I do all by my self, and for me it s a big result. :) happy to share this 
![IMG_20200101_180715|375x500](upload://wcZCdfc8gLaX9mvpyqD5W6tejnb.jpeg) 
I saw there are a lot of tutorials for the vesc tool, wich is the best one that you advice me to learn not only the simple fuction, but where I can learn the advance functions too?
```

---
## \#31 Posted by: Fosterqc Posted at: 2020-01-05T03:37:09.252Z Reads: 27

```
Fantastic! I remember my excitement at my first motor spin up. 

Hope to see your completed first built this year on the forum not owned by a coward.
```

---
## \#32 Posted by: Braniac Posted at: 2020-01-24T19:40:06.902Z Reads: 15

```
What do you mean "owned by a coward"?
```

---
## \#33 Posted by: Fosterqc Posted at: 2020-01-25T04:23:58.805Z Reads: 12

```
@onloop is the owner of this forum. He is Jason Potter the Owner of Enertion. Seen all the enertion ads on this forum?

He only talks to a few people but has tens of thousands of dollars in outstanding orders. He couldn't be bothered to say anything, just sit in his house in Gold Coast Australia.
```

---
