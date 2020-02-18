# I am a newbee and I kinda need some help :)

### Replies: 50 Views: 2405

## \#1 Posted by: DexterEsk8 Posted at: 2017-10-31T19:09:56.345Z Reads: 180

```
Hello everyone, I am Dexter from the Netherlands. When I first saw a boosted board I thought I want that to so got to there site and it is right now 1.934,79 (Dual+) that was a bit expensive for me, thats why i decided to make one myself so this is what i am planning to use:
https://hobbyking.com/en_us/zippy-flightmax-3000mah-6s-20c-lipo-pack-w-xt60u-connector.html
two 6s battery's

https://hobbyking.com/en_us/turnigy-sk8-esc-for-electric-skateboard-conversion.html
 2 Esc's with Bec

http://www.diyeboard.com/dual-belt-drive-1400w2-n5055-motor-power-truckfront-truck-kit-p-422.html
A dual belt driven motor with 7.8 torque

https://www.ebay.com/itm/221644780045 
12s BMS 

http://www.diyeboard.com/new-thumb-24ghz-remote-controller-and-receiver-rc3-p-538.html
Remote

But i am not sure what i need to use for connection between this esc and battery and to make it a dual vesc

Can someone help my out?
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2017-10-31T19:31:14.950Z Reads: 159

```
To be honest, i wouln't use the Hobbyking VESC as its an old hardware revision, the cheapest VESC you could find an, well, it's from hobbyking. Of course it would probably work at first but it might give some problems in the long run.

Also, are you planning on running the board on 12S? This would exceed the eRPM limit of a 4.10 (and also 4.12) VESC with 270kv motors. And secondly, it would be about 60 km/h top speed, you sure you want to try this for your first board? :smile:

Here's a handy calculator with you values already put in: http://esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":270,"system-efficiency":85,"motor-pulley-teeth":12,"wheel-pulley-teeth":36,"wheel-size":83}|

I'd suggest a 6S System at first since you already plan to use 2 6S Batteries, you could just put them in parallel.

Personally i wouldn't use a BMS for LiPo applications instead of a regular charger, but that depends on you.

As for connections, you would need a serial or parallel XT60 wiring harness for you battery, depending on wether you go for 6S or 12S, as well as XT 60 Connectors on the VESC end. And some wires for the Receiver, either you split the PWM Signal or you set the VESC to be Master and Slave over CAN bus.


Otherwise that would be a complete build list minus the deck :blush:
```

---
## \#3 Posted by: DexterEsk8 Posted at: 2017-10-31T20:12:41.058Z Reads: 136

```
thank you so much for your reply really helped my out, what is the best and cheapest vesc you suggest
And what is the range with the 6s battery and speed?
```

---
## \#4 Posted by: DexterEsk8 Posted at: 2017-10-31T20:18:21.690Z Reads: 129

```
Can i also use this?
https://hobbyking.com/en_us/zippy-flightmax-2200mah-5s1p-40c.html

and that 2 times
```

---
## \#5 Posted by: Brycehoosiers Posted at: 2017-10-31T20:21:55.456Z Reads: 123

```
if your going to run them in parallel then go with two 6s batteries not 5s, and go with the torque boards VESC
```

---
## \#6 Posted by: FredrikHems Posted at: 2017-10-31T20:24:46.815Z Reads: 119

```
You will wanna either some higher C rating batteries, or some high capacity. With that 6s you will only be able to output 60a MAX!
```

---
## \#7 Posted by: DexterEsk8 Posted at: 2017-10-31T20:28:09.647Z Reads: 111

```
can the torque board vesc run 2 motors or 1
```

---
## \#8 Posted by: Der6FingerJo Posted at: 2017-10-31T20:30:40.355Z Reads: 110

```
Each VESC can only run 1 Motor. 
Now, depending on what your roads look like and how much you weigh, I'd suggest a single drive 6374 Setup on 10S or so. It's cheap and with the right gearing you could get a lot of power.
```

---
## \#9 Posted by: Michael319 Posted at: 2017-10-31T20:33:35.708Z Reads: 107

```
That's wrong. Lipos have very high discharge and 2 of those 6s batteries in parallel will be totally fine.
```

---
## \#10 Posted by: DexterEsk8 Posted at: 2017-10-31T20:35:15.856Z Reads: 103

```
what is the good kv rating for me i weight 45kg and the roads are decent but no hills
```

---
## \#11 Posted by: DexterEsk8 Posted at: 2017-10-31T20:36:56.111Z Reads: 101

```
http://alienpowersystem.com/shop/brushless-motors/aps-6374-outrunner-brushless-motor-240kv-3200w/
```

---
## \#12 Posted by: Michael319 Posted at: 2017-10-31T20:37:10.633Z Reads: 98

```
Honestly, if you are looking to save a buck, you could definitely go with a single drive board, you can save money from that and you will only need one esc. You could also use that money for a better battery
```

---
## \#13 Posted by: Michael319 Posted at: 2017-10-31T20:41:02.306Z Reads: 97

```
If you know about kv then ignore this.

In simple terms: 
Lower KV will give you better torque. (Better low speed performance)
Higher KV will give you less torque, but a higher top speed. (Better high speed performance)

Torque can always be altered by changing your gearing ratio.
```

---
## \#14 Posted by: FredrikHems Posted at: 2017-10-31T20:53:29.927Z Reads: 95

```
In parallel it would work, yes. But unless he will only ride on flat terrian, the voltage sag will be pretty extreme. He also said He would Go 12s. Also, you should take in concederstion that almost every lipos are overrated. They usually will be destroyed very fast If you run them om their limits all the time
```

---
## \#15 Posted by: Michael319 Posted at: 2017-10-31T20:53:46.283Z Reads: 91

```
You could use 2 of https://hobbyking.com/en_us/zippy-compact-6200mah-4s-40c-lipo-pack.html

But you would have to solder a xt60. I personally think 8s is the best option for your build. That motor kit you linked is actually a great deal if you pair it up with the right battery
```

---
## \#16 Posted by: Der6FingerJo Posted at: 2017-10-31T21:04:55.432Z Reads: 87

```
With 45kg you have a lot of options, I'd go for kv on the lower side and readily available parts for gearing, no need to do custom work for a tall transmission.
```

---
## \#17 Posted by: ShutterShock Posted at: 2017-10-31T21:08:42.382Z Reads: 86

```
No you are still incorrect.  Those batteries are more than enough.  You're not doing your calculations right, they will be able to provide way more than 60A, especially with a 40C discharge.  My Zippy Compact batteries only have a 25C discharge and my voltage sag even on hills with a dual drive board is very minimal.  Zippy makes good batteries, and Turnigy is pretty good too.  Stay away from the Amazon ones, some are kinda sketchy.  +1 to what @Michael319 said. 

@DexterEsk8  You could run the 5S ones as well, especially with the great discharge rate, however, the 2200mAh is very very small.  I would personally look for something that is 5000mAh or above.

Edit:  If I were to rebuild I would probably go with a 30C pack or above.
```

---
## \#18 Posted by: DexterEsk8 Posted at: 2017-10-31T21:16:06.870Z Reads: 86

```
after al those tips i think i am going with a 2 of.         https://hobbyking.com/en_us/zippy-compact-3300mah-6s-35c-lipo-pack.html
Is this a good idea?

I am still not sure About taking a dual motor or a single motor
```

---
## \#19 Posted by: ShutterShock Posted at: 2017-10-31T21:19:13.573Z Reads: 80

```
That is a decent decision, however if money permits I would still go for a higher mAh rating to get some more range.  Also if the budget permits, dual drive puts a lot less stress on one motor and provides (in my opinion) a nicer riding experience, however, it is quite a bit more expensive.
```

---
## \#20 Posted by: bigben Posted at: 2017-10-31T21:27:20.909Z Reads: 81

```
I agree with @ShutterShock go for 5000mah batteries. 30c and above.
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-10-31T23:06:15.609Z Reads: 75

```
bro...

my pack only has 25a cont. and I go up massive hills all the time without an issue.  what are you smoking?
```

---
## \#22 Posted by: Michael319 Posted at: 2017-11-01T02:09:51.690Z Reads: 72

```
@DexterEsk8 I'm gonna lay it all out for ya.

If you go with that battery (**x2**) You have **2** choices

**Choice One** 
You set up the battery in a **parallel** configuration. Therefore you have a **6s** config. Okay. That's all fine. Only issue is, you have a **theoretical** max speed of **~19.5mph**. Realistically you're looking @ around **16mph**. Not so great.

**Choice Two**
You set up the battery in a **series** configuration. Therefore will have a **12s** config. That's not so great. While it will give you high enough speeds to keep up with cars on a freeway, your **VESC** will **fry** before that. VESC's have an ERPM limit of 60K, and that would go way over.

**Then there is my solution**

You get **two 4s batteries**, creating an **8s** series config. 8s is the perfect solution because it **won't** exceed the VESC's **ERPM** **limit** and you still get a realistic top speed of about 25 I think, I don't remember.....

This only makes sense if you go with your original motor choice. Which I think will save in the long run, you don't have to buy wheels, trucks, motor mounts, any of it. An 8s battery with that is the optimal solution.


hope i helped
```

---
## \#23 Posted by: FredrikHems Posted at: 2017-11-01T06:24:14.824Z Reads: 70

```
Wtf , 25 a continious? Well i dont know How thats work for you, but thats way to little for me. I didnt say it woldnt work for him, but I said the voltage sag will be veery much If plan to do lots of hill clims. Its also not good for the batteries, to be used at their limits all the time
```

---
## \#24 Posted by: DexterEsk8 Posted at: 2017-11-01T06:48:16.286Z Reads: 70

```
when i use 2 4s battery i hit a top speed pf 19 mph weighted, i think i should go with 2 5s battery with a top speed of 25 mph but i got know idea it can handle those amps


https://hobbyking.com/en_us/turnigy-nano-tech-4000mah-4s-45-90c-lipo-pack-xt-60.html

or i could use 

https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-40c.html
```

---
## \#25 Posted by: DexterEsk8 Posted at: 2017-11-01T06:49:14.958Z Reads: 68

```
and how do you calculate the amps
```

---
## \#26 Posted by: ShutterShock Posted at: 2017-11-01T07:32:03.449Z Reads: 70

```
We must keep in mind that @GrecoMan is very light :joy: 

His point is still completely valid.  I barely pull 60A cont from my battery on maximum acceleration, but that is with two motors.  I'm also fairly certain that I am probably heavier than him as well.
```

---
## \#27 Posted by: ShutterShock Posted at: 2017-11-01T07:35:59.413Z Reads: 69

```
You could use this website to calculate the battery amps using the mAh rating and C rating.

https://www.kritikalmass.net/battery-calculator/

But the manual calculation is multiplying the mAh rating by the C rating and then dividing by 1000.

For example, a 12S1P 5000mAh pack with a discharge rating of 30C would be 5000*30/1000 = 150A max

Keep in mind this is optimal conditions but those are the calculations behind it
```

---
## \#28 Posted by: kptheinventor Posted at: 2017-11-01T08:32:49.497Z Reads: 63

```
If you want to save a little bit of money you could go for 6364 (has plenty of power) but then again it's only like $10 or something.
```

---
## \#29 Posted by: GrecoMan Posted at: 2017-11-01T10:47:40.402Z Reads: 62

```
sorry but @GrecoMan weighs about 160lbs... not super light
```

---
## \#30 Posted by: DexterEsk8 Posted at: 2017-11-01T12:06:47.290Z Reads: 59

```
I am like 99 lbs
```

---
## \#31 Posted by: DexterEsk8 Posted at: 2017-11-01T13:01:26.093Z Reads: 57

```
This is what i am thinking to do
2 5s battery's
https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-40c.html

Dual motor
http://www.diyeboard.com/dual-belt-drive-1400w2-n5055-motor-power-truckfront-truck-kit-p-422.html
 and 2 vescs
products/torque-esc-vesc-bldc-electronic-speed-controller
```

---
## \#32 Posted by: GrecoMan Posted at: 2017-11-01T13:02:36.869Z Reads: 58

```
using it as 10s I assume?
```

---
## \#33 Posted by: DexterEsk8 Posted at: 2017-11-01T13:03:40.811Z Reads: 56

```
yes connect in series
```

---
## \#34 Posted by: DexterEsk8 Posted at: 2017-11-01T13:04:09.939Z Reads: 57

```
but wich connecter do you need to connect the 2 vescs
```

---
## \#35 Posted by: GrecoMan Posted at: 2017-11-01T13:07:02.969Z Reads: 59

```
you need different motors. 270kv on 10s will destroy the vesc
```

---
## \#36 Posted by: DexterEsk8 Posted at: 2017-11-01T13:11:03.270Z Reads: 58

```
http://www.diyeboard.com/180kv-n6354-outrunner-motor-2000w-for-diy-electric-skateboard-p-540.html

or
http://alienpowersystem.com/shop/brushless-motors/aps-6384s-sensored-outrunner-brushless-motor-170kv-4000w/?doing_wp_cron=1509541817.4173750877380371093750
```

---
## \#37 Posted by: DexterEsk8 Posted at: 2017-11-01T13:13:29.195Z Reads: 56

```
with the one from diyeboard.com i can make a dual motor setup with
http://www.diyeboard.com/dual-motor-beltdrive-mechanical-kit-for-5055-6354-motors-p-543.html
```

---
## \#38 Posted by: GrecoMan Posted at: 2017-11-01T13:15:57.122Z Reads: 56

```
no, don’t use the one from diyeboard.  much lower quality than the APS one

the APS one in a single drive will probably give you more power anyways
```

---
## \#39 Posted by: DexterEsk8 Posted at: 2017-11-01T13:22:04.745Z Reads: 56

```
Should i do a single or dual motor setup
```

---
## \#40 Posted by: electricjim79 Posted at: 2017-11-01T13:29:22.920Z Reads: 57

```
singles is cheaper, you could always upgrade later on
```

---
## \#41 Posted by: leonsc Posted at: 2017-11-01T14:20:07.449Z Reads: 62

```
Single is alot cheaper and just fine for a first board j used a 213kv for ages no worries  amp ar worked out take the mah add a destimal point so 5000 mah would be 5 ah then x that by c rating so a battery with 5000 would be.      5 ah x 20c = 100a continuous
```

---
## \#42 Posted by: DexterEsk8 Posted at: 2017-11-01T19:28:36.975Z Reads: 62

```
I sure i am going with a single motor, but wat is the best battery S to make it fast with 80 mm kegels and diys vesc
This is the motor i gonna use, i would think about 12S because i am now going for a single setup with 80 mm kegels 
and with 12 i could make a higher top speed. but i am not sure diys vesc can handle this much amps

collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv 

or
http://alienpowersystem.com/shop/brushless-motors/aps-6384s-sensored-outrunner-brushless-motor-170kv-4000w/

battery 2 6s together 12s
https://hobbyking.com/en_us/multistar-high-capacity-6s-5200mah-multi-rotor-lipo-pack.html

collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller

or
collections/esc-speed-controller/products/torqueboards-12s-120a-car-esc-opto-hv
```

---
## \#43 Posted by: DexterEsk8 Posted at: 2017-11-01T19:42:19.007Z Reads: 55

```
than the battery should handle 200a but the vesc could go up to 240A for a few seconds or 50A continous. My question is would the ves burn out out by this much amps?
```

---
## \#44 Posted by: Michael319 Posted at: 2017-11-01T20:55:10.366Z Reads: 56

```
You will set a max amps in the vesc settings, so don't worry about too much amps.
```

---
## \#45 Posted by: Acido Posted at: 2017-11-01T21:01:54.459Z Reads: 52

```
Heres a better calc

Calc.esk8.today
```

---
## \#46 Posted by: FredrikHems Posted at: 2017-11-01T21:06:30.414Z Reads: 53

```
The batteries you linked to can only output 52a in a 12s connection theoretically. Many people have found out that these pack only can provide arond 5c. Thats just 26a. The motor you are linking to want 80a at full power, so you will only be able to use 1/3 of the motor power. Just a reminder
```

---
## \#47 Posted by: Michael319 Posted at: 2017-11-01T21:11:53.405Z Reads: 50

```
Because you are running @ a higher voltage, you won't actually need as many amps to get the same power. I think that 170 kv would do very nicely
```

---
## \#48 Posted by: Michael319 Posted at: 2017-11-01T21:12:48.491Z Reads: 52

```
Definitely get the vesc. It's worth it especially if you're only doing single drive.
```

---
## \#49 Posted by: Michael319 Posted at: 2017-11-01T21:24:01.942Z Reads: 52

```
I recommend you choose one of these, or anything similar.  I recommend the first one.
https://hobbyking.com/en_us/turnigy-5000mah-6s-20c-lipo-pack-w-xt-90.html

https://hobbyking.com/en_us/zippy-compact-5000mah-6s-40c-lipo-pack-xt90.html
https://hobbyking.com/en_us/turnigy-battery-4500mah-6s-30c-lipo-pack-xt-90.html
```

---
## \#50 Posted by: DexterEsk8 Posted at: 2017-11-04T14:54:13.224Z Reads: 47

```
Does anyone know how to wire the charging port to the bms
```

---
