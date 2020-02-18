# Designing My First eSk8

### Replies: 32 Views: 1243

## \#1 Posted by: adrienfeve Posted at: 2018-08-02T21:57:39.001Z Reads: 252

```
Hi, my name is Adrien. 

I just started learning longboard a few weeks ago and discovered the DIY eskate community at the same time. I start to really enjoy the sport/hobby and as I live in a really hilly area in Bristol in the UK I thought going electric could be a good step forward. 

I’m however not yet willing to pay the price for a £1000+ board knowing the battery could die in a few years with me not being able to replace it. A DIY build is therefore a good solution for me I believe. I’m also an Engineer so I kind of enjoy that sort of design project. 

Before pulling the trigger, I am willing to get some advice from experienced builder about the build I designed. 

My requirements are:
-	A skate that will be easy top ride – I am not an experienced rider
-	Good torque to climb hills
-	Good breaking power and regen
-	Speed does not matter too much for me – Not planning on dying on a skateboard :), let’s say at least 15-20 mph
-	Around 10 miles range from a charge
-	Safe and convenient charge of the battery
-	As water-resistant as possible to withstand the UK weather
-	Cost less than £500 

I did some initial calculation and created a little script in Matlab to start designing my build. I still need to make some assumptions on the motor curve to calculate how fast I could climb some hills in my area:
![35|407x500](upload://x8efC9nlKPpTUQkJ9u5RSP8xb1r.png)
 
Those calculations and my research lead me to the following components for now:

* Deck – Already bought a 40in one
https://www.ebay.co.uk/itm/40-X-9-5-INCH-NO-FEAR-RED-STRIPE-LONGBOARD-DECK-GOOD-SOLID-STIFF-GRIPTAPED-DECK/132725049211?hash=item1ee707877b:g:V~YAAOSwqfpZ2ic6

* Trucks – I think I’ll take the caliber II because of the profile with flat face which could be nice to secure the motor mount
https://www.amazon.com/gp/product/B0719BXH7G/ref=oh_aui_detailpage_o00_s00?ie=UTF8&th=1&psc=1

* Wheels – 83mm wheels, hesitating with 90mm
https://fr.aliexpress.com/store/product/78A-Skateboard-Wheels-87-52mm-Long-Board-Cross-country-83-52mm-Wheels-6mm-Riserpad-35mm-Bolts/2943263_32829115461.html?spm=a2g0w.12010108.1000016.1.3c116253FVfTr1&isOrigTitle=true

* Motor – Two options there:
1) 6354 190KV 2450W cheaper but not waterproof
https://www.banggood.com/HGLRC-Flipsky-6354-190KV-2450W-Brushless-Sensored-Motor-Shaft-8mm-for-Electric-Skateboard-Rc-Models-p-1323575.html?rmmds=search&cur_warehouse=CN

2) 6365 190Kv 3550W (Water Resistant, Sealed and Sensored) more expensive, waterproof but maybe too powerful? (Might be a non issue if I can limit it with the VESC)
https://eskating.eu/product/eskating-pro-motors-6365-190kv-water-resistant-sealed-and-sensored/

* Motor mount – Cheap but apparently good quality and only requires some tweaking to fit calibre II
https://hobbyking.com/en_us/motor-mount-5.html?wrh_pdp=3&___store=en_us

* Gearing – Not found a suitable solution yet – hesitating between chain or belt and will tweak the gear ratio based on my calculation for torque required to climb some hills in my area at a decent speed.

* VESC + remote kit – Maytech
https://fr.aliexpress.com/store/product/Maytech-logboard-skateboard-remote-controller-with-receiver-and-VESC-ESC-50A-at-12lipos/1630416_32709724719.html?spm=a2g0w.12010108.1000016.1.519716c79AfuMJ&isOrigTitle=true

* BMS – 12S 80A Bestech
https://eskating.eu/product-category/bestech-bmss/

* Power switch – Probably going for a cheap loop key

* Charger – Depends if I go for BMS option or not. It will be 42V charger or balance charger if no BMS

* Battery – Not sure about what brand to buy but I think about going with 3*4S 5000mAh 25C cells to get a 12S pack and keep the thickness below 35mm
https://hobbyking.com/en_us/turnigy-battery-5000mah-4s-25c-lipo-pack-xt-90.html?___store=en_us
https://hobbyking.com/en_us/zippy-compact-5000mah-4s-25c-lipo-pack.html

* Electronics casing: Tupperware style solution to keep cost down and be as water resistant as possible

If I could get some feedback that would be awesome. The build as I created it should end up around £400-£500.
Thanks.

Adrien
```

---
## \#2 Posted by: b264 Posted at: 2018-08-02T22:03:48.977Z Reads: 208

```
[quote="adrienfeve, post:1, topic:63649"]
sport/hobby
[/quote]

Some folks use this as a primary method of transportation.  It also is more convenient for some folks than an automobile and it's pollution-free.  It's better for all of us to just call it "esk8ing" or electric skateboarding.
```

---
## \#3 Posted by: adrienfeve Posted at: 2018-08-02T22:06:31.989Z Reads: 206

```
Oh yes agree no offence. I'll actually use it for part of my commute.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-08-02T22:08:23.996Z Reads: 205

```
Some tips, 

1. the mount only fits the trucks they sell

2. HobbyKing has some 195kv and 190kv Keda motors for cheap

3. If you are using 12s you need a 50.4v charger. 42v is for a 10s pack
```

---
## \#5 Posted by: Vampiresquid64 Posted at: 2018-08-02T22:29:58.608Z Reads: 195

```
If you don't wanna go very fast, you're probably better off with a 10s pack that's bigger. With a 12s much of that top end voltage is likely to be wasted. Unless you have weird gear ratios
```

---
## \#6 Posted by: Grozniy Posted at: 2018-08-03T00:01:16.387Z Reads: 188

```
[Wheels](Big 80mm 87mm 83mm 90mm 97mm Longboard wheel SHR78A Red Color PU Wheels High Level Soft Wheels Resistant PU Skateboard Wheels  http://s.aliexpress.com/7fIJz6NR?fromSns=Copiar para a área de transferência), go with 90mm.
40/44T wheel pulley, 15T motor pulley, 15mm belt
Avoid maytech if you can. Get Hobbyking ESC or even flipsky.
Get the KEDA 6364 AS @pat.speed said. .
You'll probably be spend 15/20Wh/km. Means 240/320wh battery.
@marcmt88 or @fottaz mount
  Cheap mini remote from eBay.
The rest of money you save, invest in custom li-ion battery with charge only bms and charger. 30Q or 20700b.
```

---
## \#7 Posted by: adrienfeve Posted at: 2018-08-03T05:57:29.625Z Reads: 174

```
https://www.electric-skateboard.builders/t/designing-my-first-esk8/63649/5?u=adrienfeve

Thanks, this confirms what i was also thinking with the 10s instead of the 12s.
Another reason to do that is that I read that if you go over the max ERPM of the VESC it is possible to fry it and my 12s build theoretically goes over with no load on the wheels.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-08-03T06:07:21.203Z Reads: 164

```
Look for the hobbyking sk8 series.
Sealed motors and relatively cheap.
Would look for 150-170kV motor which should rise up your torque.
Get a higher c rated lipo. 60-65c min. They more expensive, but if you climp mountains often, you also need higher currents more often.
With higher c rated lipos the voltage sag will keep minimal and the batteries run cooler which results in longer lifespan. For the long it will safe you some money.
```

---
## \#9 Posted by: adrienfeve Posted at: 2018-08-03T06:12:34.043Z Reads: 156

```
https://www.electric-skateboard.builders/t/designing-my-first-esk8/63649/8?u=adrienfeve

When you talk about voltage sag, do you mean the voltage drop of the cell during discharges? If I understand you correctly this drop goes up with current but can be minimised by buying better C rate cells.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-08-03T06:31:55.801Z Reads: 151

```
Every cell has a internal resistance.
The higher the resistance, the higher the voltage drop under high loads.
The higher the c-rating, the lower should be the resistance. It’s not 100% like this but manufacturers usually don’t give information about the internal resistance.
The c-Rating shows you how much current the battery can handle constantly.
You can calculate it like this
Pack size(ah)*c rating = max constant current 
That’s the theory...but as there is a marketing in everything which is sold now adays you can take from this value about the half. That should be your max constant current.
So 5000mah*25c=125a /2 =62.5a
As you said you climp a lot of mountains I guess you can go up to 80a quite often.
This would result in getting your batteries run hotter and your voltage under load will drop for example from 3.9-3.5 in time of the load.
After you reached the top the voltage will swap back. So as long as your batteries fully charged it’s not a problem.
But when you already around the 3.7v for example you can come under 3.5 and your vesc will cut off your battery.
So on your way home you will need to walk up the mountains with low c rated batteries, with high c rated batteries you still can drive.
🤔hope that was somehow clear and not confusing 😅
```

---
## \#11 Posted by: adrienfeve Posted at: 2018-08-03T10:34:50.957Z Reads: 138

```
https://www.electric-skateboard.builders/t/designing-my-first-esk8/63649/10?u=adrienfeve

It's all clear thanks a lot! 
I'll go for above 50C rate cells and probably a 10S pack.
```

---
## \#12 Posted by: dareno Posted at: 2018-08-04T19:46:56.990Z Reads: 126

```
Leave that hk motor mount alone its pretty cheapo. 
Hk sk8 motors are good as are the vescs
and I would consider the graphene lipos from hk too they are in a different league, bit more money but if you are going to spend, spend on the battery.

@b264 soccer mum!
```

---
## \#13 Posted by: dareno Posted at: 2018-08-04T19:55:42.083Z Reads: 125

```
One more thing, Unless uk pavements and roads have changed dramatically in the last 4 years then go for the bigger wheel option.
```

---
## \#14 Posted by: adrienfeve Posted at: 2018-08-05T00:16:07.038Z Reads: 121

```
I'm sure they did not change... :)
I'll need to check the clearance with my deck for the 90mm wheels but will consider, maybe with raiser pads. 
For the battery I'll also have a look at the graphene option. I've also spotted an 8000mah 5s option at 30C. What would you advise between more capacity or a better chemistry cell?
```

---
## \#15 Posted by: dareno Posted at: 2018-08-05T00:32:27.038Z Reads: 121

```
Discharge rate is what you want so the higher the c rating the better and the less sag you'll get.  I think the graphenes are all fairly high and unfortunately so is the cost but its the heart of your board so its money very well spent. Cheap batteries are false economy as you will upgrade them later trust me.

Wheels make a world of difference to riding comfort and if you are going to go on the pavements then bigger the better with some nice soft risers to help cushion. I run 97mm but am upgrading to 107mm for that reason and here in oz we have pretty good sidewalks and roads but the concrete beach tracks with expansion joints every 10m really work on your calves after a while.  Anyway hope this helps and keep the build here with pics!  good luck
```

---
## \#16 Posted by: BigZu Posted at: 2018-08-06T15:44:45.626Z Reads: 106

```
Hello,
I am planning on building a similar board and trying to decide on the battery.  is there a big difference between 3000 MAH https://hobbyking.com/en_us/turnigy-graphine-3000mah-5s1p-45c.html  and 5000 MAH https://hobbyking.com/en_us/turnigy-graphine-5000mah-5s1p-45c.html

Thank you
```

---
## \#17 Posted by: adrienfeve Posted at: 2018-08-06T18:02:06.291Z Reads: 103

```
https://www.electric-skateboard.builders/t/designing-my-first-esk8/63649/16?u=adrienfeve

Your capacity will reflect the range. So 5000/3000 more range with the 5000 mAh roughly for the same rated voltage pack. Based on my build and calculations, I would get around 14km per charge.
```

---
## \#18 Posted by: BigZu Posted at: 2018-08-06T18:23:00.595Z Reads: 99

```
Great.  Thank you.  I guess I will spend more money and get 2 of the 5000MAH 5S1P 45C.
```

---
## \#19 Posted by: adrienfeve Posted at: 2018-08-08T20:36:53.797Z Reads: 101

```
Just an update on my build. I have now ordered most of the parts (except the batteries):
![57|622x500](upload://7HccjrPqlejOJ9OGNH1vONfm3sn.png)

I am still studying the battery as I am still unsure whether I go 2*5s or 5*2s 5000mAh batteries.
As I am also over my budget already and will probably finish around £550, I try to find a good solution without compromising too much on C rate.

I am tempted by the graphene range from Turnigy expecting that those cells will last longer.
```

---
## \#20 Posted by: adrienfeve Posted at: 2018-08-14T19:59:26.725Z Reads: 97

```
![37|601x500](upload://nuy3hRKweR9G841jTke4y1Ued8K.png)

Final update of the parts on my build. I went with 5S Graphene Lipo 5000mAh 45C.
A bit more expensive than planned initially but worth it hopefully.
```

---
## \#22 Posted by: Superflim Posted at: 2018-08-14T21:40:43.556Z Reads: 82

```
Looking good man.

Will be a pain in the ass to charge these tho hahah
```

---
## \#23 Posted by: adrienfeve Posted at: 2018-08-15T08:44:41.012Z Reads: 81

```
I plan to parallel charge at 0.5C on a balance charger. The case I chose is easy to open so I hope this won't be too much hassle.

I also should have enough range for 2 to 3 days of commute.
```

---
## \#24 Posted by: Socalscare Posted at: 2018-08-15T16:49:47.159Z Reads: 77

```
I'm looking forward to seeing how this works out, I just started looking at building an e skate after commuting on a Segway for the past few months but I'm tired of the Slow 10.9mph top speed and lack of easily being able to carry it.
```

---
## \#25 Posted by: adrienfeve Posted at: 2018-08-15T19:09:00.674Z Reads: 79

```
My plan is to update as I build. I don't have all the parts yet but will continue to post pictures and feedback on that thread.
```

---
## \#26 Posted by: adrienfeve Posted at: 2018-08-20T23:10:56.911Z Reads: 81

```
Finally starting to receive parts. I have assembled the deck, trucks, wheels and bearings to give the board a test drive: 
![20180820_235214|666x500](upload://waMZqYkdekBcYe63KOukaDzUZeH.jpg)

I used DIY 6mm rubber pads to hopefully dampen vibration and raise the deck from the wheels:
![20180820_235157|666x500](upload://pYDRc1cer8ovtAEhmIRPnZYSF4R.jpg)

Bearings are venom brand and have a nice red and black touch that suits the board well. Wheels are 90mm ones:
![20180820_235121|666x500](upload://qgkfA3B67GhXu5PFbVfzAHSZERH.jpg)

I have nearly everything except the motor and pulley which is stuck on backorder in Hobbyking HK. I'll setup a Bluetooth module to communicate with the VESC and lights in the meantime. 

Batteries turnigy graphene look very premium. Hope they serve me well!
```

---
## \#27 Posted by: adrienfeve Posted at: 2018-08-22T19:51:57.652Z Reads: 70

```
https://www.electric-skateboard.builders/t/designing-my-first-esk8/63649/18?u=adrienfeve

This is what I bought in the end. Graphene 45C 5000mah.
```

---
## \#28 Posted by: Toughook Posted at: 2018-08-22T20:18:04.318Z Reads: 71

```
"I also should have enough range for 2 to 3 days of commute"

Probably not. 

What will happen is that you'll enjoy the ride so much that you go the long way, just because you can. Certainly for the first few months you'll be charging after every ride :)
```

---
## \#29 Posted by: adrienfeve Posted at: 2018-08-22T20:40:20.985Z Reads: 69

```
That's exactly the plan 😁
```

---
## \#30 Posted by: adrienfeve Posted at: 2018-09-26T17:12:42.115Z Reads: 63

```
![20180926_180318|375x500](upload://jhkmrFHrvRR5SFRg2N6QwqEWlp0.jpeg)
Nearly finished with the electronics. I have planned for lighting from the battery and a Bluetooth module to connect to the vesc app. 

I mounted the vesc on a module with a heatsink connected on the FETs both sides. 

![20180926_180518|666x500](upload://hV80YozuI7xJn59iUDEz3sQ71Bs.jpeg)
```

---
## \#31 Posted by: UKRider Posted at: 2018-09-26T19:05:07.399Z Reads: 59

```
A bit late but I would of suggested that you went for a decent motor mount as this is where many problems come about. Also if your doing hills you need good brakes so a dual motor setup is what you want. Again with hills you will have belt slippage with single motor.  What will happen you will end up paying for more in a short space of time for upgrades.

By the way loving the Tupperware but I suggest you make another as they don't last long.

I understand your on a budget but you may have to spend another £200-300 for a board that will last a little longer.
```

---
## \#32 Posted by: adrienfeve Posted at: 2018-11-03T19:01:09.247Z Reads: 39

```
![20181103_132116|666x500](upload://pkdJvOb4xEM7A77KDlqZkjdUK0S.jpeg)

Motor mounted. The hobbyking mount works on caliber trucks with just a little bit of sand down rework.
The belt is in tension and everything seems in correct alignment and clearances. 

![20181103_132052|666x500](upload://9ZzbM5VWNTRMYhjX3xyZJT4Y3V9.jpeg)

I installed headlights as well which will be powered by the battery via a 12v buck converter.
```

---
## \#33 Posted by: adrienfeve Posted at: 2018-11-13T12:09:44.307Z Reads: 26

```
Well this is working very well and it is amazing. Thanks for the help guys
![20181105_222951|666x500](upload://6pAE8Rxuoyk65wPLVAWarBz4BVE.jpeg) 

![20181110_094447|666x500](upload://4q9bqEEk4jbsDRQPT4CmAuWoE8P.jpeg)
```

---
