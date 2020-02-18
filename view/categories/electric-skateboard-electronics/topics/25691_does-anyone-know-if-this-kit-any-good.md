# Does anyone know if this kit any good?

### Replies: 12 Views: 1045

## \#1 Posted by: Tomer Posted at: 2017-06-19T13:27:58.916Z Reads: 178

```
Hi folks,

I am looking for upgrading my system to dual drive one. I was looking on Aliexpress and found out [this kit](https://www.aliexpress.com/item/Electric-Longboard-skateboard-Conversion-Kit-Rear-Truck-With-Two-Motor-front-truck-Belt-Drive-dual-motor/32801299931.html?trace=msiteDetail2pcDetail).

My idea is to buy only the motor pulley, motor mount, belts and use 2x Maytech 5065 220kv motors instead. 
I weigh about 75kg (165 pounds) and would like to reach top speed of 40-50 km/h (25-30 mp/h). The biggest hill in my city has hill grade of 4.5%.

I will also replace the wheels from 80mm to 83mm. I will use [195mm 50º BLK/BLK](https://shop.paristruckco.com/collections/reverse-kingpin-trucks/products/195mm-black-black) trucks. 

EDIT: Forgot to mention, I use 10s1p battery pack @ 42v.

I would like to hear your opinions about this idea, maybe you even had a chance to test this kit.

Thanks.
```

---
## \#2 Posted by: aigenic Posted at: 2017-06-19T21:02:01.676Z Reads: 147

```
I havent seen anyone on DIY scene usinge them, but from what I know they are also used by some eskate company (benchwheel maybe?)...if you want to use them then make sure, that hey fits your hanger nicely...you will prbably have to modify the hanger a little (making small flat surfaces or holes for the screws from the motor mount)...The wheels are not same as flywheels so the pulley wont fit in them...

I wouldnt buy this...you can get a set for similar prices if you buy some parts from members of this forum...
```

---
## \#3 Posted by: sl33py Posted at: 2017-06-19T22:44:18.712Z Reads: 131

```
Welcome!

You don't really need dual motors for such small hills and relatively light weight.  

I'd suggest legit Caliber II's and @korryh's motor mounts instead.  More substantial and less frustration than the round Paris 195 trucks (i had a set and a PITA to keep it from spinning and grinding motor on ground).

Some spacers and dual 6355 motors are pretty simple to add - even without spacers the 6355 dual works, or go single 6374 if you want a single w/ more power.

Battery - assuming some sort of li-ion using 18650 cells?  1p is not going to work well or work at all.  I'd stick to Lipo if on a budget, or at least 3p w/ 18650's (20a capable each cell = 60a in 3p).  Or 4p - more equals better performance and less sag.  Or get some 5000mAh 30c+ Lipos for a lot less (claimed 150A = realistically maybe half?  5Ah * 30c = 150A).

HTH - GL!
```

---
## \#4 Posted by: Tomer Posted at: 2017-06-20T09:17:23.500Z Reads: 96

```
Benchwheel use hexagonal cross-section truck, while the kit I showed here use regular trucks. 
The seller mentioned that the kit comes with Paris trucks, however if I want to switch to 83mm wheels, it won't fit to this kit (no room will be left for the dual motors). So I looked up and found wider Paris trucks.
I do hope he really use Paris trucks and not a clone Paris, because otherwise I will need to modify the genuine Paris truck to fit the kit.

As for the wheel pulley, I will use a different one that will fit the 83mm wheels. 

Can you please share with me names of pepole who sells kit like this?
```

---
## \#5 Posted by: Tomer Posted at: 2017-06-20T09:42:30.499Z Reads: 89

```
I am going to gain more weight so I will need more power in the future.

I will think about korryh's motor mount. Thanks for that. 

I really love the idea of having dual motor drive, seems to have better braking and good torque.

I use ACTON's battery pack that I used with my ACTON Blink board. Right now it's working great with the motor that I have from ACTON as well (it's a sh*tty motor). My next project is to build a battery pack by myself. How do you think that 10s1p will handle x2 5055 motors until then?
```

---
## \#6 Posted by: sl33py Posted at: 2017-06-20T15:38:42.497Z Reads: 83

```
[quote="Tomer, post:5, topic:25691, full:true"]
I am going to gain more weight so I will need more power in the future.
[/quote]
Ha!  Yeah - that happens...  I'm about 120kg/265lbs (2m/6'8" helps) and ride frequently single motor.  Just so you know it's very doable.  But prefer dual motors for hills.

[quote="Tomer, post:5, topic:25691, full:true"]
I will think about korryh's motor mount. Thanks for that. 

I really love the idea of having dual motor drive, seems to have better braking and good torque.

I use ACTON's battery pack that I used with my ACTON Blink board. Right now it's working great with the motor that I have from ACTON as well (it's a sh*tty motor). My next project is to build a battery pack by myself. How do you think that 10s1p will handle x2 5055 motors until then?
[/quote]

You can do a dual 6355 setup on Caliber II trucks w/o problem.  I have a dual 6355 w/ 12mm belts and it might fit 15mm (i have some speed rings to move the wheels out to give as much room as possible - with low profile axle nuts and the nylock just flush w/ axle end).

I would steer this way and avoid round trucks (Paris or other).  If you are willing to sacrifice speed for torque i'd also look at the 40t options from DIYes (12mm), or @Titoxd10001 (15mm).  They both have flywheel gear setups in 40t.  I would then measure axle to axle (CtC) distance and use the bbman belt length calculator to make sure you get the right belt length to fit your gears.

Battery -  1p was concerning, so i did a bit of digging...  I don't think this is an 18650 pack, but rather a Lipo pack.  That's much better for amp capacity / delivery.

Just to confirm if you've looked - check out @Mikenopolis' thread:
http://www.electric-skateboard.builders/t/half-ass-diy-with-off-the-shelf-acton-blink-board-and-enertion-motor/4403

There also should be some good info if this matches your setup.  Learn from his process and hopefully it'll help.

Any time we get the battery questions... "will this be enough" - my answer is *maybe*.

Will it run - likely if it was already setup for a single motor and sticking with single.  Or dual to dual.  Where you run into issues is C Rating of batteries and amp delivery.  Ability to keep up with demand - it'll either sag heavily and reduce range (and pack life, and a lot of heat), or be gutless up hills and hard acceleration - but fine on flats.  ETC.  Hard to say without testing in person.  

Regardless - frankenstein it and just be careful if it gets too hot - STOP.  Nobody likes to see an esk8 in flames on the news...
```

---
## \#7 Posted by: Tomer Posted at: 2017-06-25T07:02:31.844Z Reads: 55

```
I made a mistake when choosing 5065 dual motors as an option. Bad news is that I already purchased from Banggood [this 50xx motor mount kit](https://www.banggood.com/Electric-Skateboard-Belt-Motor-Mount-Bracket-Pulley-Screws-For-839097MM-Wheel-p-1105929.html?utm_campaign=ios-share&utm_medium=cussku&utm_design=0&utm_source=youtube&ios_share=1&_branch_match_id=406175731559677642), but the good news is that at least I didn't ordered x2 5065 motors.

So x2 6355 is going to be my choice of motors with Caliber II 50 trucks. In regards of the kit itself, I think I'll get x2 [DIYelectric Caliber II V4 motor mount](diy-electric-skateboard-kits-parts/v4-63mm-motor-mount/?attribute_motor-size=63mm+Motor+Mount). [I'll use x2 Maytech wheel pulley](https://www.aliexpress.com/item/Maytech-cheap-hoverboard-1x17mm-wide-wheel-Pulley-and-belt-Combo-for-overboard-electric-skateboard/32742223448.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_10172_10084_10083_10080_10082_10081_10110_10136_10137_519_10111_10060_10112_10113_10155_10062_10114_437_10154_10056_10055_10054_10182_10059_303_100031_10099_10078_10079_10103_10073_10102_10096_10123_10189_10052_10053_10142_10107_142_10050_10051,searchweb201603_9,ppcSwitch_5&btsid=0b9c7dd6-886d-438e-bd00-32c69c6b0733&algo_expid=08326b78-2c81-433d-8491-324c45d3403d-0&algo_pvid=08326b78-2c81-433d-8491-324c45d3403d). I wonder if they will work well together? What are you thoughts about it?

As for the battery, soon I'll start to put all my effort on building the battery package.
```

---
## \#8 Posted by: sl33py Posted at: 2017-06-25T17:57:50.896Z Reads: 56

```
[quote="Tomer, post:7, topic:25691"]
I wonder if they will work well together? What are you thoughts about it?
[/quote]


DON'T get that maytech wheel "kit".  It's a nylon wheel gear not aluminum, and not injected molded i don't think like Enertion's - i bet it's a print or other poor quality... and for the price i'd just get DIYes motor mount kit with gears - likely save you a few $ and much more durable being all metal.
```

---
## \#9 Posted by: Tomer Posted at: 2017-06-26T09:49:49.018Z Reads: 50

```
How bad is it to use nylon wheel pulley? Currently my ACTON board has nylon pulley and I haven't experienced any issues with it whatsoever. Is it not good to use it performance wise or in terms of durability?

Nylon wheel pulley will be **much** cheaper for me to get as all the aluminum pulleys that I found - shipment is very expensive to my country.
```

---
## \#10 Posted by: sl33py Posted at: 2017-06-26T14:56:27.763Z Reads: 46

```
It's a personal bias.  If it's a quality injected molded gear like Enertion sells - they are really durable.  If it's a poorer quality mold, or 3d printed - it can be an issue.  

I setup a nylon gear for my GF's DIY esk8 i built so she could ride w/ me.  It worked OK.  First it was 9mm and a single - so not great anyway, but since she only goes about 8mph it was workable for her.  Anytime i rode it skipped the entire time.

If i were to use another printed gear, i'd make sure it was 15mm or possibly 20mm depending on your weight.

A recent issue with heat and printed gears highlights a temperature based concern.  A printed gear at 5-10mph setup correctly should not get too hot (and you should double check a few times before going faster).  If you have any misalignment in your setup, where something will rub and cause heat - now you can have an issue!  One guy here melted his wheel gears at speed!

Last - they are expensive for what you are getting.  So if you are already getting the motor mount from DIYes - look at the price of his full kit and shipping will be the same.  Delay to get to your location also should be the same unless he's out of one and has to split shipments.  the Maytech gear kit was ~$40 iirc - so if it really is just a few $ more, i strongly suggest you get his.

I would say that your Acton board likely has a quality nylon gear, and doesn't go super fast.  If your new build DIY board is going to go a lot faster - just make sure to ride a slower speed a few times and check for heat, then increase speed again and re-test.  Before you go bomb a full speed run.

HTH - GL!
```

---
## \#11 Posted by: Tomer Posted at: 2017-06-29T20:23:08.904Z Reads: 29

```
Hey there! So I thought about making a 3D print of the wheel pulley. 
I found a local printer who gave me a real nice pricing for printing, however it was for 25% fill printing.
I've asked him how much will it be for 50%, 75% and 100%. Will wait for an update and hope the prices will be still reasonable (something makes me feel it won't).
So I guess PETG will be the material of choice for the print, however I am not sure on which pulley size to go with. Options are 9mm, 12mm and 15mm (I got the STL files here on the forum). So I guess you'll probably advise me to go with 15mm, and I can ask the printer of he can make the 3D print modified and print a bigger pulley.

Any thoughts?
```

---
## \#12 Posted by: Jinra Posted at: 2017-06-29T20:25:29.348Z Reads: 28

```
The kit in OP is definitely a Benchwheel power kit
```

---
