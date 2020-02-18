# Feather &#124; Agacê Cruiser &#124; Kegels &#124; 5055 DD &#124; 11S1P

### Replies: 31 Views: 796

## \#1 Posted by: Pedrodemio Posted at: 2019-02-15T01:50:41.275Z Reads: 216

```
Well, as the name says the goal here is extreme lightweight and portable. Since my last build I realized that even if it's a dream to ride, it's a pain when you are not riding

This build at first will be just a resurrection of my old board with what I have laying around, but eventually it will be as the parts list bellow

https://www.electric-skateboard.builders/t/agace-cruiser-33-dual-5055-dual-vesc-6-paris-195mm-10s3p-ncr-ga-kegels-lots-of-3d-print/64307 

Parts:

* Agace Cruiser - 1800g
* Paris 195mm - 860g
* Kegels - 1008g
* 5055 DD - 860g
* 11S1P INR21700-40T - 737g
* Dual VESC 4.12 + misc eletronics ~ 150g
* 3D printed enclosure - 200g
* fasteners, bearings, etc - 100g

Total of 5.7 kg, would like to keep it under 5 kg but it doesn't seen possible

For now what I'm doing is evaluating if it's viable to convert the 5055 motors to direct drive performance and heat wise, first step was to model them as it is, and them play with the windings, this is it wound as 190Kv runing at 40A

We can easily see why they overheated in my build, at 40A we are looking at 100w of heat loss

![image|690x466](upload://wBXSzot6cwSA87OChIXd2erJiUl.png) 

![image|690x464](upload://lGlcY6RJPbe5ScNrFzddGoAqHo6.jpeg) 

Take all this data with caution, I'm merely using it as comparison tool, not absolute performance

Checking if it will fit, I may change to 180mm Paris if it do

![image|690x402](upload://z4tAycmaq7UYu4ijjAFz1n2jyMk.jpeg)
```

---
## \#2 Posted by: bevilacqua Posted at: 2019-02-15T11:08:50.446Z Reads: 189

```
why DD? Wouldn't it be better to go 42XX route with low gearing in order to make the most out of your battery?

I only would consider Hubs/DD if I had enough amps.

I recon that the deck weight quite a bit too, I would try shaving some grams there.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2019-02-15T17:02:09.568Z Reads: 174

```
Probably, but I want to test a DD before going forward with the large DD design for my big board

I'm still on the fence if the 5055 will be enough

The main misconception with hubs/DD is that the Kv matter, it doesn't, it only affect the current needed from the ESC and battery, that's why people overheat their hubs, Raptor being the main example, pushing more current in a low Kv motor will only make it heat more and more

Example of the 5055's, if I take it as it is, 190Kv and just bolt to my wheel I will have the same torque for the same loses, now if I want more torque to overcome the lack of gearing them I will push more current and it will heat up a lot

The truth is that there is no replacement for bigger motor/more cooper

Just as an experiment I scaled the 5055 up to the size of 6355, keeping same Kv, now I can produce the same torque at half the losses
```

---
## \#4 Posted by: bevilacqua Posted at: 2019-02-15T17:16:20.404Z Reads: 159

```
![image|212x152](upload://laetOYVhbkqO2bLflmj6VejXeku.png) 

:wink:
```

---
## \#5 Posted by: Pedrodemio Posted at: 2019-02-15T17:22:24.896Z Reads: 148

```
Could you go a little further? each time I think I got how everything comes togheter there is something that throws me off, we got flux and current that generates torque, whats p? the radius of the airgap?
```

---
## \#6 Posted by: bevilacqua Posted at: 2019-02-15T17:34:28.508Z Reads: 147

```
p = pole pairs.
my only point is that by having a 1:1 gear ratio yo need so much more startup current than a geared system. Therefore you generate I^2 more ohmic losses

compared to a 1:3 gear ratio 3^2=9 times more losses =! heat + poor consumption
```

---
## \#7 Posted by: Pedrodemio Posted at: 2019-02-15T17:44:56.143Z Reads: 138

```
Thanks

Yeah, that's the problem, the only way to overcome that is keeping the same ampere-turn relation, my 190Kv motor could do 40A, rewound to 60Kv it can do 12.6A for the same heat loss
But as you said the problem stats when you expect the same torque for the same motor ungeared, the loses go through the roof fast
```

---
## \#8 Posted by: Pedrodemio Posted at: 2019-02-17T22:14:06.824Z Reads: 134

```
As a test I did some calculations and adjusted my board to have the same torque as the DD would have at 2 N.m per wheel, to be honest it's not great obviously, but it gets the job done, the low speed performance sucks a lot, probably due to the low efficiency of the motors at that range, but once you get to higher speeds is handles well

I refined the simulations a bit and it seen I can get 2.5 N.m for each wheel while keeping heat loss reasonable, I may even at first go without rewinding the motors, it will put more strain on the VESC for sure

Another goal of this build is investigate the effect of Statorade (https://www.ebikes.ca/product-info/statorade.html) on a DD setup, Justin from Ebikes.ca did some tests with Jacob and Inboard hubs, but the effect is not that great because we have the polyurethane in the way

For my big DD in the works I plan to go that way, it makes way more sense to extract heat from the stator that way instead of trying to get it through the hanger, the surface area that could be available from the bell is way bigger

1300 rpm = 20 km/h
2000 rpm = 30 km/h

For 190Kv@37V@40A:

![image|690x463](upload://5yiRQnmWPu7uQJcuHrf60LSm7OC.jpeg)   

![image|690x464](upload://hv0LaCBugleMv48t641pFXMGYfW.png) 

For 50Kv@37V@10.5A:

![image|690x462](upload://kRXxQ1QehIN32j0q4LwZ2TlbKaV.png) 

![image|690x463](upload://DyVAstSIVMfdJVZ6drOura86ts.png) 

If rewind happen, the Kv will have to be increased a bit to have peak efficiency at 25 km/h, which is the speed I plan to limite this build
```

---
## \#9 Posted by: Pedrodemio Posted at: 2019-02-20T03:33:58.580Z Reads: 116

```
DD design done, pretty simple to keep costs down if this should go wrong, also Dexter confirmed that the magnets are N42SH, so I will be able to to run them hotter = more torque

Also I did some thermal simulations, running them at 20A the core will get up to 100°C while the magnets should not go ove 80°C, all this considering the loading they are subject in a typical ride for me, also the software allows me to use oil on the air gap simulating the Statorade, them the everything stay bellow 90°C even at higher currents, with a total of 9 N.m at the wheels

Another concern is that I am almost sure the hanger will bend, but it's cheaper than making one from scratch for testing
![image|690x377](upload://x2HyMNcU24RZebTajwB4KRvDF1G.jpeg) 

![image|690x463](upload://kRdVG4iIsGd66bLhlOnzNW9U81Z.jpeg)

![image|690x426](upload://zQb6S9qqujSJCoYTDS8kL4Euwat.jpeg)
```

---
## \#10 Posted by: Pedrodemio Posted at: 2019-02-21T01:50:13.529Z Reads: 111

```
Test fit, still have to find a suitable capacitor, fit the arduino and an NRF module and if possible a charge only BMS, I may skip it if I can find a 13 pin circular connector that's not huge

![image|690x336](upload://tQgS8mmqQgqbs6RriN2yEUJjpFq.jpeg) 

![image|690x373](upload://sTSGHw565krfohYGkXL05Mb0TXr.jpeg) 

![image|690x297](upload://iJW8CuZJqkFeP7zodFLIHJgkmF8.jpeg)
```

---
## \#11 Posted by: janpom Posted at: 2019-02-21T09:36:19.582Z Reads: 99

```
Why 13 pin? Wouldn't 12 pin suffice for 11s?
```

---
## \#12 Posted by: Pedrodemio Posted at: 2019-02-21T13:16:32.163Z Reads: 93

```
Actually, ideally it should be 14 pins (or 13,depending on them BMS), 12 for the balance wires and positive and negative, if you use b1- and b11+ to actually send current into the battery there is a considerable voltage drop in them, so the BMS/balance charge would first balance considering this voltage drop and then has to balance again as the current drops

My first board was like this, two 5S balance connectors to charge, the current would flow by the same wires the battery voltage is measured

There are some nice and cheap connector from the GX20 series that have up to 15 pins
```

---
## \#13 Posted by: janpom Posted at: 2019-02-21T13:26:18.014Z Reads: 92

```
[quote="Pedrodemio, post:12, topic:84260"]
if you use b1- and b11+ to actually send current into the battery there is a considerable voltage drop in them, so the BMS/balance charge would first balance considering this voltage drop and then has to balance again as the current drops
[/quote]

True. I have exactly that problem in my setup. I have the balancing disabled on the BMS and use it only to monitor the cell voltages and to cut the charger once any cell reaches 4.25V. The first cells to reach that reading are always the first or the last cell because of the voltage drop. In reality they are around 4.15V, which is where I want to stop charging anyway. The 4.25V is still a safe threshold should cells get out of balance.

I agree it's not ideal though. I would prefer extra pins for charging. I currently use a 12 pin connector for 10S battery pack so I'm missing one pin.

Also with 11S1P you probably can't really afford not to charge to full.
```

---
## \#14 Posted by: Pedrodemio Posted at: 2019-02-21T13:32:07.816Z Reads: 88

```
You described it perfectly

I’m still thinking about 11S, it’s harder to find chargers and BMS, buyout gives me more range, 12S in the flipsky is risky, even more since in 11S the spike during regen is greater

I may even got 7S2P of 30Q, it would weight 672g vs 737g for the 40T, be cheaper while keeping the same energy but with probably bigger interl resistance
```

---
## \#15 Posted by: janpom Posted at: 2019-02-21T13:47:20.079Z Reads: 81

```
Maybe 8S2P would be better? 8S balance chargers can still be had for cheap.
```

---
## \#16 Posted by: Pedrodemio Posted at: 2019-02-21T14:19:46.552Z Reads: 84

```
Could it be, most times I will bulk charge

And thinking about, the 12 pins you suggested can work, I don’t need to balance it, just have access to each cell to measure and if out of balance, charge each P group individually
```

---
## \#17 Posted by: janpom Posted at: 2019-02-21T14:29:07.339Z Reads: 86

```
[quote="Pedrodemio, post:16, topic:84260"]
And thinking about, the 12 pins you suggested can work, I don’t need to balance it, just have access to each cell to measure and if out of balance, charge each P group individually
[/quote]

If you go that route, you might find my [external BMS charger](https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words/2992/9748?u=janpom) handy. It's based on the LLT Power Smart BMS. I described above how I use it. No balancing. Just monitor and stop charging at the right time. I added a little display, which I control with ~~Arduino~~ NodeMCU. The ~~Arduino~~ NodeMCU gets cell voltage readings from the BMS and adjusts the first and last cell since it knows how much voltage drop there is on the charge wires, so it always shows the correct voltage on the display even while charging.
```

---
## \#18 Posted by: Pedrodemio Posted at: 2019-02-21T15:10:38.687Z Reads: 77

```
Thanks, will take a look
```

---
## \#19 Posted by: Pedrodemio Posted at: 2019-02-22T02:07:45.562Z Reads: 86

```
Doing a little comparison between 11S1P of INR21700-40T and 7S2P of INR18650-30Q

Main advantage of 30Q is that I can source them locally and for a really good price 

                                    11S1P/40T                      7S2P/30Q
Weight                             737 g                              642 g
Max power@Vnom:        1424 W                           777 W
Pack IR:                           0.22 Ω                            0.14 Ω
P. Loss @300 W:              12 W                             19 W
Energy:                            157 Wh                         150 Wh
Cost (BRL):                    R$496,00                      R$378,00

(EDIT: apparently I don't know how to make a table here)

40T wins easily while not being a lot more expensive, just have to find someone that ships it here
If the 30Q would be capable of a bit more power they would really be great, I will be able to get approximately 500~600W from the motors, maybe running them at 20A like a lot of people do

![image|690x277](upload://kLYgNNtDep8jvVGL5xzyGZGy2Ca.jpeg)
```

---
## \#20 Posted by: Friskies Posted at: 2019-02-23T19:53:11.807Z Reads: 76

```
I don't know where you get your pricing from but even at 1/3 better stats the price of the 40T costs more than 33% more. Meaning the only reason you would pick it over the 30q is if your enclosure for some reason fits 21700 better than 18650.
```

---
## \#21 Posted by: Pedrodemio Posted at: 2019-02-23T20:13:14.322Z Reads: 71

```
That's true, I need to do few more tests with my current board, but I think the power of the 30Q may be to low and loose too much speed in hills

The pricing I got from IMR and with guy that that import them here
```

---
## \#22 Posted by: Lionpuncher Posted at: 2019-02-23T21:51:09.259Z Reads: 65

```
Have you considered the hg6 batteries? Their 20650’s with 30a discharge (actual). Good option for a smaller battery. I have them in 10s2p, really like the end result. Not saggy even at around 3.5v. Usually not too expensive. Something to consider...
```

---
## \#23 Posted by: b264 Posted at: 2019-02-23T21:57:53.871Z Reads: 62

```
If lightweight is your goal, have you considered single drive?  Single drive is probably lighter, even if the one motor you need is bigger.
```

---
## \#24 Posted by: Pedrodemio Posted at: 2019-02-23T22:01:12.648Z Reads: 64

```
@Lionpuncher thanks for the suggestion, will take a look at them

@b264 really bad streets around here, some hills I couldn’t climb fast enough to keep up with traffic due to losing traction on the drive wheel

But the first iteration of this build will be with a single drive 6355, I will just put together some old parts I have, zero money to invest at the moment unfortunately
```

---
## \#25 Posted by: b264 Posted at: 2019-02-24T00:03:09.639Z Reads: 61

```
Single wheel drive sounds bad but it's not really that bad.  For real.  Overkill is the game around here, but often folks forget about the simple stuff that works fine and is lightweight.
```

---
## \#26 Posted by: Lionpuncher Posted at: 2019-02-24T02:45:36.226Z Reads: 63

```
Gotta agree. A mono 6374 will be lighter, consume less energy and still rip up hills given enough amperage. But as @Pedrodemio has said, he’s using what he has.
```

---
## \#27 Posted by: Pedrodemio Posted at: 2019-02-24T04:36:33.218Z Reads: 65

```
For most places I have to ride a single 6355 goes great without getting to hot from the experience with my first board, would love to have smooth roads
```

---
## \#28 Posted by: mishrasubhransu Posted at: 2019-03-20T22:13:02.718Z Reads: 53

```
What software/tool are you using to do the calculations?
```

---
## \#29 Posted by: Pedrodemio Posted at: 2019-03-20T23:10:30.284Z Reads: 50

```
MotorSolve, 15 days trial, them just make another email :grin:

https://www.mentor.com/products/mechanical/motorsolve/bldc/
```

---
## \#30 Posted by: Bor.inc Posted at: 2019-03-21T08:03:01.743Z Reads: 48

```
Do you have any progress or updates? its prety interesting that you make your own dd with also smaller motors
```

---
## \#31 Posted by: Pedrodemio Posted at: 2019-03-21T14:21:06.093Z Reads: 42

```
Thanks Bor, nothing more for now, this will be a pretty long term project, still a lot of things I have do to in my main board and also some other projects I’ve got to finish before focusing on this
```

---
