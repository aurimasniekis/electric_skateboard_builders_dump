# Needing help with building a circuit

### Replies: 49 Views: 1904

## \#1 Posted by: epster Posted at: 2017-11-12T15:28:41.834Z Reads: 145

```
Hey guys i would like to build a skateboard for my nephew in the Netherlands. I selected some parts and i did some research but i don`t really know how to make the circuit. Could you give me tips what to use to combine for instance the batteries and how i need to do that and if this is a good build or if its is going to overheat in the first 100 metres.

These are the parts 
ELECTRIC SKATEBOARD MOTOR 6355 260KV
products/electric-skateboard-motor-6355-260kv?variant=712632074263 

FOCBOX Motor Controller
http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/#details 

ZIPPY Compact 5000mAh 6S 25C Lipo Pack i will buy those 2 times so 6S2P
https://hobbyking.com/en_us/zippy-compact-5000mah-6s-25c-lipo-pack.html 

Do you guys think this is a descent build or do i need to change some stuff around? I really tried my best but i am just not the best electrian there is.
```

---
## \#2 Posted by: aigenic Posted at: 2017-11-12T15:32:43.378Z Reads: 130

```
It will work together, but if you plan on buying two battereis it will be better to connect them in series to get 12s and use one 170kv 6374 motor...it would give you more power this way and still the same range :) or go 10s (two 5s batteries in series) with 190kv motor...
```

---
## \#3 Posted by: mmaner Posted at: 2017-11-12T15:41:10.673Z Reads: 129

```
There is absolutely nothing wrong with 6S and a 260kv motor.  Hundreds of people have done it.  Ive done it, still doing it.

Take a look at the builds category and you can see the process for dozens of builds.  You still need a wheels pulley, motor pulley, belt, xt90s loop key or vedder switch and enclosure at a minimum...assuming you already have the standard skate gear.

Here's a sample diagram of how it all goes together...
http://www.electric-skateboard.builders/uploads/db1493/original/3X/2/e/2e1dad479b80ea26687a9f4da341b30451c7c4c7.jpg
```

---
## \#4 Posted by: ShutterShock Posted at: 2017-11-12T15:58:41.738Z Reads: 114

```
Actually you're a bit wrong here. Connecting them in parallel will be effectively twice the range, not the same range :stuck_out_tongue:

Like @mmaner said, nothing wrong with 6s!
```

---
## \#5 Posted by: epster Posted at: 2017-11-12T16:12:40.867Z Reads: 108

```
Thanks for the replys guys. So if i want to make full use of my 260kv motor what is a smart battery setup 12s2p? Or do you guys recommend doing something else? And if i upp my battery capacity will my esc still tolarate it or is there a max?
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-11-12T16:14:36.807Z Reads: 103

```
stick with 6s. 12s on 260kv will destroy something
```

---
## \#7 Posted by: epster Posted at: 2017-11-12T16:18:34.476Z Reads: 97

```
I got a kit linked by a friend that fits the motor and recommends 6s or 12s this is the kit collections/single-motor-mechanical-kit/products/single-motor-mechanical-kit 
If i add to this kit the motor a battery a deck controller and a motor computer (vesc if i remember it right). I am good to go right?
```

---
## \#8 Posted by: epster Posted at: 2017-11-12T16:19:37.511Z Reads: 92

```
Ah oke so 6s2p is the best option with my motor and vesc?
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-11-12T16:21:01.056Z Reads: 87

```
6sXp will serve you well with 260kv and VESC
```

---
## \#10 Posted by: epster Posted at: 2017-11-12T16:36:08.558Z Reads: 79

```
Ah thanks man. I couldnt figure out from the forums  how I set everything up and what cables to use could someone make like a pic in paint or some for me what to connect where.
```

---
## \#11 Posted by: epster Posted at: 2017-11-12T16:37:16.621Z Reads: 78

```
Another question is the 25C or the 30C better considering my 260kv motor
```

---
## \#12 Posted by: aigenic Posted at: 2017-11-12T21:48:57.804Z Reads: 78

```
@ShutterShock 

If you use two 6s batteries of the same capacity and connect them in parallel and then use two of the same batteries and connect them in series you will get the same watt hours, which means the same range (almost, the 6S could give a little bit more)

@GrecoMan
yeah, 12s on 260 would destroy everything, tahts why I offered 170kv motor...

6S is ok, but if you can choose motor (meaning you havent bought it yet) I would go for 170kv motor and run it on 12s1p, you would get more power for the same money (50.4*80= about 4000W, limited by motor)
 if you use 260 kv motor on 6s2p, you would get about 25.2*80 = about 2000W, maybe a little bit more and thats what I am talking about...

OFC 260kv motor is completly allright, you just cant use it on 12s...

25C will be enough, even 20C or 15C would work well if you would use 2 of them in paralel (6S2P)
```

---
## \#13 Posted by: epster Posted at: 2017-11-12T22:14:20.867Z Reads: 71

```
Ah oke thanks for explaining. What do you think about a 7s gives 25.4v or 8s or am i risking battery loss then with the 260kv motor ? I would like to put 2 batteries parralel because of the extra range.
```

---
## \#14 Posted by: aigenic Posted at: 2017-11-12T22:22:43.153Z Reads: 70

```
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":260,"system-efficiency":90,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":90}|

Battery loss? No, you are not...you could be risking burned DRV, but it is still under ERPM limit so it should be ok :) 

The motor you linked has the max of 80A, if you use 2 8S 5000Ah 25c batteries in parallel then they can output up to 250A (5Ah x 25c x 2) so the batteries are more than safe :) 

Not completly sure what you mean about the battery loss...Voltage sag?
```

---
## \#15 Posted by: Jinra Posted at: 2017-11-12T22:24:11.076Z Reads: 64

```
doesn't matter if you connect in series or parallel, you still get twice the watt hours
```

---
## \#16 Posted by: aigenic Posted at: 2017-11-12T22:24:37.243Z Reads: 62

```
Thats exactly what I said :) <3
```

---
## \#17 Posted by: Jinra Posted at: 2017-11-12T22:25:30.262Z Reads: 63

```
guess i misunderstood
```

---
## \#18 Posted by: aigenic Posted at: 2017-11-12T22:28:13.297Z Reads: 65

```
Guess I cant speak English properly...I envy all the native English speakers...
```

---
## \#19 Posted by: epster Posted at: 2017-11-12T22:36:04.832Z Reads: 62

```
Yeah i meant voltage sag haha i am kinda new to all the terms.

So i will go with the 260kv motor because i already had it 
8s2p 5000mah batteries
But i am thinking one thing now i saw this vesc which one do you guys recommend? Considering the 80 dollar price diffirence? products/torque-esc-vesc-bldc-electronic-speed-controller
This cheaper one only has a consistent 50A output compared to the 80A. So the cheaper one is not a goos choice right?
```

---
## \#20 Posted by: aigenic Posted at: 2017-11-13T06:51:30.446Z Reads: 58

```
The FOCBOX is the way...better quality...Its worth it :) Do not try to go as cheap as possible....
IF you will use two of them in paralel there will be almost no sag...
```

---
## \#21 Posted by: ShutterShock Posted at: 2017-11-13T07:08:07.293Z Reads: 60

```
Yeah that's what I said lol I don't think it was understood properly lol
```

---
## \#22 Posted by: epster Posted at: 2017-11-13T07:20:37.316Z Reads: 61

```
Oh sorry i didnt understand that properly. English is not my first language haha

So the 260kv motor
products/electric-skateboard-motor-6355-260kv?variant=712632074263

8s2p batteries
https://hobbyking.com/en_us/zippy-compact-5800mah-8s-25c-lipo-pack.html?___store=en_us

And thd focbox is the way to go right
http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/

on off power switch 
http://alienpowersystem.com/shop/rc-ev-accessories/electronics/alien-antispark-power-switch-3-16s-300amp-max/

The remote
```

---
## \#23 Posted by: ShutterShock Posted at: 2017-11-13T07:21:54.312Z Reads: 57

```
That's alright! Good luck with building :)
```

---
## \#24 Posted by: epster Posted at: 2017-11-13T07:23:08.923Z Reads: 55

```
Thanks man does anynone know a good guide or where i can buy covers for my components
```

---
## \#25 Posted by: pat.speed Posted at: 2017-11-13T11:10:52.050Z Reads: 53

```
Your English is perfectly fine I understood what you meant and you are correct series produces the same range as parallel. 

As for the enclosures they can be made or you can buy them at a few places like DIYElectricSkateboard or I think Miami electric boards? And I think @MasterCho  on this forum sells them too
```

---
## \#26 Posted by: aigenic Posted at: 2017-11-13T12:02:01.276Z Reads: 54

```
Also @Eboosted sells some...its not difficlt to find somone to make custom one for you :) just ask in the general chat :)
```

---
## \#27 Posted by: epster Posted at: 2017-11-13T14:07:15.836Z Reads: 50

```
Yo guys i designed the circuit could you guys check for mistakes or improvements i also would like to use a bms wouls that profit my system or isnt it worth it i also alwant to add a battterylife indicator maybe this one https://hobbyking.com/en_us/zippy-compact-5800mah-8s-25c-lipo-pack.html?___store=en_us
Hope i did my homework well haha <img src="/uploads/db1493/original/3X/a/f/af335173bacc701d3081611c76581a85f223b256.jpg" width="690" height="387">

This is the on/off switch products/on-off-power-switch-electric-skateboard
```

---
## \#28 Posted by: pat.speed Posted at: 2017-11-13T19:55:01.039Z Reads: 45

```
Yes that is correct. Instead of getting an on off switch I would suggest a antispark loop key. One because the switchs sometimes break very easily and if you have a s just get a bestech one and it will already have a switch on it
```

---
## \#29 Posted by: epster Posted at: 2017-11-14T22:06:16.041Z Reads: 39

```
Hey guys what do you think of leaving out the BMS because the battery will almost never overheat because of its capacity compared to the motor and instead put a battery power meter in its place like this one, for instance, seems like a good plan?

https://hobbyking.com/en_us/turnigy-180a-watt-meter-and-power-analyzer.html
```

---
## \#30 Posted by: epster Posted at: 2017-11-16T15:12:45.685Z Reads: 35

```
Hey guys I would like to realise my build but idk how I need to connect everything to each other for instance: when i replace the BMS with a power meter how do I make it like it is a full circuit. And can i just plug my motor into the Vesc or isnt that possible?
```

---
## \#31 Posted by: aigenic Posted at: 2017-11-16T21:28:56.366Z Reads: 34

```
Reaad more :) 
Motor is connected by the bullet conenctors to the vesc...
If you dont have BMS you will have to charge it with a hobby charger :) 
Power meter connects red and black wire (plus and minus) and it should be behind the switch...
```

---
## \#32 Posted by: epster Posted at: 2017-11-17T20:27:36.089Z Reads: 32

```
Hey man i did some research and i found out that maybe this would be a good bms what do you think for my 80A motor?

https://bmsbattery.com/ebike-battery/378-24s-lifepo4-bms-battery-management-system-battery.html
```

---
## \#33 Posted by: pat.speed Posted at: 2017-11-17T21:08:47.930Z Reads: 29

```
That won't work it is for lifepo4 cells you have lipo. And you don't need 80a, 60a will be fine
```

---
## \#34 Posted by: aigenic Posted at: 2017-11-17T21:43:12.207Z Reads: 29

```
And it is 24S BMS, you will have 6s batteries of different chemistry...
these two can be used if you would bypass them only for charging (you would have to solder more wires together, cheaper): https://hobbyking.com/en_us/6s-li-ion-10a-pcm.html
 https://hobbyking.com/en_us/6s-li-ion-pcm-charge-4a-discharge-10a.html

Or this one used for both discharging and charging: https://www.ebay.com/itm/6s-24v-Li-ion-Lithium-Cell-60A-18650-Battery-Protection-Board-BMS-PCM-Balance/152483333427?epid=705838451&hash=item2380b70533:g:Y4UAAOSwi0RXyWAW

There are lot of BMSes on ebay and anywhere else...the most favourite are BesTech BMSes and SUPOWER, thy are pricey, but worth the money :) 


For more info and differences about BMSes, read more...search the internet, use google...there is no good article about BMSes here from what I know...
```

---
## \#35 Posted by: b264 Posted at: 2017-11-17T22:26:18.010Z Reads: 28

```
[quote="epster, post:27, topic:38100"]
Yo guys i designed the circuit could you guys check for mistakes
[/quote]

I don't think that's correct.  Are you trying to run 6S + double-range, or 12S?
```

---
## \#36 Posted by: pat.speed Posted at: 2017-11-17T22:54:31.759Z Reads: 24

```
Ahhh I thought it was one of the ones when you just plug in the amount of wires you need and it will charge any number up to 24s
```

---
## \#37 Posted by: aigenic Posted at: 2017-11-18T07:54:31.901Z Reads: 25

```
No thats hobby style charger :)
```

---
## \#38 Posted by: aigenic Posted at: 2017-11-18T07:55:16.889Z Reads: 26

```
He will be running 6s2p
```

---
## \#39 Posted by: pat.speed Posted at: 2017-11-18T08:27:26.510Z Reads: 25

```
Yeah but you can get bms style ones like that I think I saw one at bestech it said something like 8-16s
```

---
## \#40 Posted by: aigenic Posted at: 2017-11-18T10:20:28.751Z Reads: 26

```
Might exist, would not buy, waste of money.
```

---
## \#41 Posted by: epster Posted at: 2017-11-18T14:17:47.868Z Reads: 22

```
so you recommend me just to let the bms out?
```

---
## \#42 Posted by: aigenic Posted at: 2017-11-18T16:05:02.795Z Reads: 21

```
No :D you can use BMS, but you need to buy 6S LIPO BMS, not 24S LiFePO4...you look like you dont know anything about it...

[Read this](http://www.electric-skateboard.builders/t/how-do-you-charge-your-longboard/21561)
[This also might help](http://www.electric-skateboard.builders/t/help-for-bms-wiring-and-bms-cutoff-limits-needed/22263)

ANd just few random links from google, some of them might be usefull :) Some might not, I did not read them, just linked those who look interesting... 
[1](http://www.electric-skateboard.builders/t/you-really-dont-need-a-bms-with-cheap-lipos/17765)
[2](http://www.electric-skateboard.builders/t/balance-charger-vs-bms-for-12s5p-lithium-ion-pack/16050)
[3](https://www.electricbike.com/bmss-what-do-they-do/)
[4](https://endless-sphere.com/forums/viewtopic.php?f=2&t=76386)
[5](https://www.fullspectrumpower.com/blogs/full-spectrum-news/8310438-balance-charger-or-bms-for-lightweight-lithium-battery)

Just read and read, it is not easy to build your skateboard, its not just about getting an answer, it is also about understanding the problem...
```

---
## \#43 Posted by: Hummie Posted at: 2017-11-18T18:09:16.289Z Reads: 21

```
6s 2p u might need to pull more amps than esc can take and over temp shut down. 
U don't need a bms. Especially w lipo its easy to attach a lipo discharge balancer and be careful
```

---
## \#44 Posted by: epster Posted at: 2017-11-18T18:40:24.510Z Reads: 20

```
Read your links and i think i got a good one now

http://www.bestechpower.com/communicationbms/BMSD328.html

 but if i want to upgrade to a dual motor in the future do i make the motor and the vesc parallel to the other vesc and motor becuase if thats how you make a 2 motor system i need to get this one another question that is like never talked about what does the overcharge voltage mean? If i use 3.7v batteries x 8 wont the bms work then? Hope you guys can help me out with that
```

---
## \#45 Posted by: aigenic Posted at: 2017-11-18T19:22:45.869Z Reads: 20

```
This one would work, but i dont get why you prefer these modular BMSes, they will be way more expensive than normal 8s BMS...

Overcharge voltage protection...SEARCH BUTTON PLS...when you are charging your batteries it stops the charge at 4.2 V (or a little bit less), the same thing happends when you are going town the hill with fully charged battery = NO BRAKES...
```

---
## \#46 Posted by: epster Posted at: 2017-11-18T19:40:14.622Z Reads: 21

```
But you just linked me that this was a good site to buy a bms?
```

---
## \#47 Posted by: Hummie Posted at: 2017-11-18T21:03:57.426Z Reads: 20

```
what happens if you have overvoltage protection on your bms?  I'm guessing if you have it it will stop further charging of the cells when youre braking.  so then what happens?  the vesc isn't going to shut down and the energy has to go somewhere when being directed somewhere other than the cell.   I guess something blows up while you lose your brakes?
```

---
## \#48 Posted by: aigenic Posted at: 2017-11-18T21:37:49.187Z Reads: 21

```
Yep, exactly :) More detailed answer :)

@epster
Yep, it is good site, I just think you dont know what BMS is for  and what you can expect from it...
```

---
## \#49 Posted by: epster Posted at: 2017-11-20T18:12:36.552Z Reads: 18

```
Hey guys do you have a good recommendation for a VESC because i think it would be smart to make full use of the motor by changing to a 80A vesc

if i go with a new vesc 80A
i will go with this BMS for my batteries 

http://bestechpower.com/296v8spcmbmspcbforli-ionli-polymerbatterypack/PCM-D131.html 

or this one depending on the vesc

http://bestechpower.com/296v8spcmbmspcbforli-ionli-polymerbatterypack/BMS-D298V1.html
```

---
