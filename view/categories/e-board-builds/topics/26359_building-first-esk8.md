# Building first Esk8!

### Replies: 60 Views: 2158

## \#1 Posted by: abctheing Posted at: 2017-06-28T21:12:06.976Z Reads: 168

```
Hey people! I'm going to build my first electric longboard!

I already have the board itself, i also have the vesc-x and a diy 433 controller. What i need is basically a battery, motor, charger, the rest i have/can build myself.

Here are pictures of my board (not finished)

<img src="/uploads/db1493/original/3X/b/9/b9a6eda523652095c9fa29ab20620cb60f46ec7e.JPG" width="374" height="500"> <img src="/uploads/db1493/original/3X/a/0/a011173689c04b1545934146462d90a21fa1c589.JPG" width="374" height="500">

Anway, i wanted to buy the SK3 6374 192kv, but it's sold out, so now i'm thinking about the Torqueboards 6374 190KV, is that any good? I was also thinking of making my own 18650 battery. I was thinking of buying 10 of these, so in total 30 cells: https://www.banggood.com/3PCS-Elfeland-3_7v-4200mAh-18650-Rechargeable-Li-ion-Battery-Blue-p-1152745.html Where can i buy a cheap charger from?

I have a lot of experience with lipos, having built quadcopters and other toys before, and i would like to use 18650 for this project :slight_smile: 

I will wire the batteries so i get around 50 volts/12s and i have a budget at around 240 dollars for the motor/battery.

I weight around 85kg/185pounds but will probably become a little lighter in the next few months :stuck_out_tongue:  I want to build my board for torque, not speed because there are some really insane hills where i live. What kinda gearing would you recommend? Here are some hills where i live, and by the way, these are not the steepest hills around here:

<img src="/uploads/db1493/original/3X/a/c/ac1454e901e44f2a55db83e26316b3e7466e90a2.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/f/a/fa8b9b8dccfb11d553fee0792f9f39947e693886.JPG" width="666" height="500">

I would be fine with a top speed of 20kmh/13mph, i am a skating beginner :)

That's all i can think of for now, thank you very much!
```

---
## \#2 Posted by: Guacamoleface Posted at: 2017-06-28T21:16:40.691Z Reads: 143

```
The torqueboards 6374 is a good motor for sure - I use it myself.


but.. If you wanna build for torque I would probably go for dualdrive, thoose hills(Atleast the first one) look steep but that may just be the pictures.
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2017-06-28T21:20:25.221Z Reads: 144

```
Looks pretty good so far! Ambition to build a pack from scratch on your first go. But there's plenty of resources around here. You really want to stick with name brand 18650's though. Samsung 25r or LG HE2's are popular. Off brands won't be able to output enough current, or won't last as many charge cycles, or claim to have way higher capacities than they do, or any combination of the above. 

Yes, lots of people use motors from DIY, including myself.But there's no point in gearing it to only do 13mph. I've run a single 6355 geared for 30mph and still had PLENTY of torque. You'll want to go faster when you get comfortable anyway. If you're really worried about it, you can limit speed with the vesc software until you're more confident.
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2017-06-28T21:21:44.463Z Reads: 134

```
Yeah I second this. If you're really chasing torque, go dual and you'll have more power than you could ever use.
```

---
## \#5 Posted by: abctheing Posted at: 2017-06-28T21:24:38.811Z Reads: 125

```
Hey, thanks to both of you. I had a small look at buying 2 of these: https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html

But the only way i'll buy them is if my single vesc-x can handle both of them, and i'm not really sure about that.
I have also soldered lipos myself and done a lot of research so i think i know what to do! :slight_smile:
```

---
## \#6 Posted by: abctheing Posted at: 2017-06-28T21:26:18.562Z Reads: 119

```
I could also change the gearing later if i would so want to!
```

---
## \#7 Posted by: t0m_r1dd1e Posted at: 2017-06-28T21:35:28.193Z Reads: 121

```
Yeah I've never heard of being able to run two motors off one controller. And yeah you can definitely change gearing later.
```

---
## \#8 Posted by: Guacamoleface Posted at: 2017-06-28T21:35:45.323Z Reads: 122

```
You will need one vesc per motor, so no a single vesc wont handleboth.

But if you wanna stick to single drive I highly suggest going for a 15mm setup. 
On a 12s Im not sure but I think something like 13/36 gearing would be good. Correct me if Im wrong whomever sees this, but thats my guess. 

The size of wheels also does alot, I feel like my single on 13/36 has alot of torque, but a huge difference if I go 100mm wheels vs 83mm wheels.

Edit, bigger wheels - higher top speed and less torque.
```

---
## \#9 Posted by: t0m_r1dd1e Posted at: 2017-06-28T21:40:11.484Z Reads: 110

```
You can play with different motor KV, gearing ratios, and wheels sizes here: http://calc.esk8.it/
```

---
## \#10 Posted by: abctheing Posted at: 2017-06-28T21:40:14.386Z Reads: 110

```
Thanks :slight_smile: my wheels are 80mm. 
I used the speed calculator and got this, but it's my first time using it:<img src="/uploads/db1493/original/3X/8/d/8d312a276be22cd4d1cfe05669292eb355504836.jpg" width="658" height="500">
```

---
## \#11 Posted by: Guacamoleface Posted at: 2017-06-28T21:42:00.780Z Reads: 97

```
Also, why 12s if you dont wanna go that fast?
```

---
## \#12 Posted by: abctheing Posted at: 2017-06-28T21:43:19.836Z Reads: 101

```
The esc supports 12s so i thought why not use a big 6374 12s motor. It will be powerful and probably have lots of torque.

Edit: I wanna go as fast as possible but still wanna climb those hills, that's why i want to gear a little extra to be sure :slight_smile:
```

---
## \#13 Posted by: Guacamoleface Posted at: 2017-06-28T21:44:58.932Z Reads: 100

```
Well as for what I recall it Volt(serial) will increase your speed,While the amperage(paralells) that your battery can deliver will give you the torque.
```

---
## \#14 Posted by: abctheing Posted at: 2017-06-28T21:49:53.516Z Reads: 98

```
Well i thought if 12S is the max i can give it then i'll do that, to get the most out of the motor.
```

---
## \#15 Posted by: Guacamoleface Posted at: 2017-06-28T21:55:33.501Z Reads: 100

```
Im currently using a 10s myself and I dont use its full potential. And I've been cruising in around 40kmh.

My best suggestion I can give you is go check other peoples build out, different battery setups(6s,8s etc.) and just look how they perform.

As for now I use Ackmaniacs application for my board which means I can set the parameters for what I want my setup to deliver(Aka different modes, limit speed, power etc). May be worth checking if you wanna go for a high power setup but wanna limit it.
```

---
## \#16 Posted by: abctheing Posted at: 2017-06-28T21:59:21.239Z Reads: 96

```
Thanks! This project has been set on hold for a few months and now i want to finish it. I would like to order the parts tomorrow so i don't really want to wait and do the most heavy research in the world but i'll have a look. My vesc-x also has options for everything, so i know i can limit the speed if i want. Anyway, the gearing i found was 4.5:1, where can i buy gears that are as close as possible to that? 

Edit: To stay on the safe side, maybe i'll just solder my batteries to a 10s instead? I hope i won't lose that much power from it thought.
```

---
## \#17 Posted by: Challlsss Posted at: 2017-06-28T22:04:51.145Z Reads: 88

```
Hi @abctheing VESC uses current control rather than voltage. So you are actually best off designing the build around the top speed, rather than trying to program it. That being said. The easiest way to get a **lot** of torque would be to go high voltage and then use a really low gear ratio. (lowet Kv motor posible and pulley ratio) plug it into the esk8 calc and see what you get. If I were you I would aim around 20-25 mph for a first build and if you decide  you want more speed later you can change the pulleys.
```

---
## \#18 Posted by: abctheing Posted at: 2017-06-28T22:16:33.172Z Reads: 93

```
Hey, thanks a lot! I already put it in my calculator and got this, but the speed is a bit slow for you though: <img src="/uploads/db1493/original/3X/8/d/8d312a276be22cd4d1cfe05669292eb355504836.jpg" width="658" height="500">

But you are telling me i should stick to 12S and gear it low, just like i thought about doing from the start?
```

---
## \#19 Posted by: gee Posted at: 2017-06-29T01:48:23.033Z Reads: 84

```
motor pulley : 8
HOPEFULLY the belt doesn't skip when you ride it.
```

---
## \#20 Posted by: Challlsss Posted at: 2017-06-29T01:59:27.430Z Reads: 88

```
yeah the motor pulley teeth # is really low. I'd reccomend getting higher teeth like 13 min. Then focusing on getting a lower kv motor.
```

---
## \#21 Posted by: abctheing Posted at: 2017-06-29T12:36:18.629Z Reads: 83

```
Hey, can you check if the parts i selected will work well? Thanks

diy-electric-skateboard-kits-parts/12t-htd5-20mm-motor-pulley/

diy-electric-skateboard-kits-parts/36t-abec11-drive-wheel-pulley/

diy-electric-skateboard-kits-parts/265mm-htd5-12mm-belt/

Then i have the 6374 motor i talked about on 12S, will that give me enough torque up hills?
```

---
## \#22 Posted by: Alanhunt123 Posted at: 2017-06-29T12:43:34.800Z Reads: 80

```
Only issue with your pulleys is that the motor pulley is 20mm wide. Since the motor pulley is the only pulley that has flanges on both sides, so since your belt is only 12mm wide, it may want to walk off of the other pulley.

I would recommend getting at least a 13t or 14t motor pulley to avoid skipping. I assure you, a 6374 will give you plenty of torque with 13/36 or 14/36!

Good luck!
```

---
## \#23 Posted by: abctheing Posted at: 2017-06-29T12:51:05.120Z Reads: 73

```
Thanks, they only had the 20mm version of the 12T pulley.

I replaced it with this, is it fine? diy-electric-skateboard-kits-parts/13t-htd5-motor-pulley-12mm/
```

---
## \#24 Posted by: abctheing Posted at: 2017-06-29T13:41:02.770Z Reads: 67

```
I also wonder what charger i'm gonna use for the 18650 batteries. I already have a lipo charger but i don't think i can use it
```

---
## \#25 Posted by: Challlsss Posted at: 2017-06-29T13:50:19.722Z Reads: 63

```
Not with 12S Just get a bms
```

---
## \#26 Posted by: Alanhunt123 Posted at: 2017-06-29T13:50:34.758Z Reads: 61

```
That pulley looks fine. Just make sure that you have enough clearance for the set screw. If not, you might have to go to the hardware store to get a smaller one.

I've been using a LiPo balance charger for my Samsung 25r 10S4P pack with no issues. What kind of LiPo charger do you have?
```

---
## \#27 Posted by: abctheing Posted at: 2017-06-29T13:53:12.978Z Reads: 62

```
I also have a budget you know? I wrote it in the beginning, but i am already over it
```

---
## \#28 Posted by: Challlsss Posted at: 2017-06-29T13:54:53.316Z Reads: 62

```
Well then just don't charge your board
;)
JkJk
Seriously though unless you have a 12S Lipo Charger, a BMS is just going to be part of the requirements. Unless you really want to save an extra $30 for a shitload of extra work
```

---
## \#29 Posted by: abctheing Posted at: 2017-06-29T13:56:07.455Z Reads: 63

```
I have a charger i got from my local hobby store, it can only charge up to 6S though. http://www.rc-deler.no/produkt/imaxrc-x80-ac-dc-balance-charger/
```

---
## \#30 Posted by: im-done Posted at: 2017-06-29T13:56:13.372Z Reads: 63

```
i dont know where you are located but here is a 6374 sk3 but its only 149kv but you can get the speed back in the  gear reduction, plus it will have a higher torque. Only 1 left act fast 
https://www.amazon.com/Turnigy-Aerodrive-SK3-6374-149kv-Brushless/dp/B00URCM8RO/ref=sr_1_1?ie=UTF8&qid=1498744470&sr=8-1&keywords=sk3+6374
```

---
## \#31 Posted by: Challlsss Posted at: 2017-06-29T13:57:19.952Z Reads: 64

```
Be careful with this link! Looks like the seller is selling shitty motors
```

---
## \#32 Posted by: abctheing Posted at: 2017-06-29T13:57:24.387Z Reads: 62

```
Haha, i would like a BMS but i haven't read a lot about it, and i don't know what's best to buy. Any recommendations?
```

---
## \#33 Posted by: abctheing Posted at: 2017-06-29T13:58:57.185Z Reads: 64

```
I looked at the SK3's and i would like to buy them from hobbyking themselves but they are all sold out, so i wanna go for something else. Torqueboards doesn't have a lower kv motor.
```

---
## \#34 Posted by: im-done Posted at: 2017-06-29T14:07:40.043Z Reads: 62

```
whats weird is amazon says "sipped and sold by HobbyKing" under the price. but hobbyking also seems to have them 
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
and the 192kv also is in stock its your lucky day!
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
```

---
## \#35 Posted by: Challlsss Posted at: 2017-06-29T14:33:59.416Z Reads: 56

```
@abctheing
1) Go on ebay and get one that can handle  as many amps as you want to charge with. Learn how to wire it so you are "Bypassing BMS"
2) Make a margarita cuz "Treat yo self"
```

---
## \#36 Posted by: abctheing Posted at: 2017-06-29T14:36:13.405Z Reads: 58

```
Thanks, but what should i search for? "electric skateboard bms" or what?
```

---
## \#37 Posted by: abctheing Posted at: 2017-06-29T14:37:16.780Z Reads: 57

```
No, i was supposed to buy the 192kv but even though it says it's in stock it's not. So no way i am ordering a SK3.
```

---
## \#38 Posted by: Challlsss Posted at: 2017-06-29T14:37:39.104Z Reads: 57

```
12S BMS
SK3 are not bad.
```

---
## \#39 Posted by: abctheing Posted at: 2017-06-29T14:41:22.623Z Reads: 60

```
Thanks. SK3's are good i know, but out of stock. 

I found this BMS: http://www.ebay.com/itm/44V-48V-50-4V-12S-30A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System-/221274094989?hash=item3384f6bd8d:g:30UAAOxy-NVSEdSO

It says it can handle 30A, does that mean i can charge with 30A??? That's a lot, no way i'm going to charge that fast.

I also don't know how i can plug it in the wall to get charge power.
Edit: Power supply
```

---
## \#40 Posted by: Challlsss Posted at: 2017-06-29T14:48:32.818Z Reads: 60

```
Looks good to me. You should be able to find info on this forum about how to set up a wall charger with. BMS I am not a good source of info there as I personally have yet to use one.
```

---
## \#41 Posted by: abctheing Posted at: 2017-06-29T14:52:58.769Z Reads: 57

```
Great! Thanks! I just wonder now how many battery cells i should buy? I don't want to spend to much and i can probably upgrade later, but i thought about buying 13 of these: https://www.banggood.com/1pcs-NCR18650B-3400mAH-3_7-V-Unprotected-Rechargeable-Lithium-Battery-p-72906.html?rmmds=cart

I honestly think i need more.
```

---
## \#42 Posted by: Challlsss Posted at: 2017-06-29T14:59:05.936Z Reads: 60

```
The cost is too high
and why 13 that number makes no sense
look at Samsung 18650 25R or 30Q (36 Cells)
and Basen 26650 (24 cells)

https://liionwholesale.com/collections/batteries/products/basen-4500mah-26650?variant=14135870212
```

---
## \#43 Posted by: abctheing Posted at: 2017-06-29T15:00:20.606Z Reads: 57

```
I took 13 because that was the money i was willing to use
```

---
## \#44 Posted by: abctheing Posted at: 2017-06-29T15:02:09.248Z Reads: 54

```
This website won't show to Norway, is there any other trusted places you know about?
```

---
## \#45 Posted by: Challlsss Posted at: 2017-06-29T15:03:26.716Z Reads: 55

```
oookay. So if you are going to do 12S you need factors of 12. 
A good rule of thumb with Liion cells is if you want to draw a certain current for your board you'll need double the max continuous current draw capability. As a result if you do the Samsung cells I listed above a 12S3P (36 cells) would be a great pack size (although pricy) and the Basen cells 12S2P (24 cells) would be a great pack size.
Checkout NKON, they are in Europe i believe
```

---
## \#46 Posted by: abctheing Posted at: 2017-06-29T15:05:33.507Z Reads: 53

```
I found these: https://batterionline.no/samsung-icr18560-26j-li-ion-batteri

I am thinking of buying 24 cells.

But if i buy everything including BMS i will be like twice over my budget, maybe i should just set this project on pause again..
```

---
## \#47 Posted by: Challlsss Posted at: 2017-06-29T15:36:29.639Z Reads: 50

```
if you buy those cells you will need at very least 12S8P pack although 12S10P or 12S12P would be better because they are max discharge 5.2A

So you are looking at 100-150 Cells and a shitload of weight if you decide to buy those. What I'm saying is they wont work.
If you are trying to save money buy Lipo Batteries from HobbyKing.
```

---
## \#48 Posted by: abctheing Posted at: 2017-06-29T16:03:25.888Z Reads: 53

```
Ahh thanks, how about these then: https://ru.nkon.nl/sony-us18650vtc6.html

I think i'll buy 30 since they were cheaper.
```

---
## \#49 Posted by: Challlsss Posted at: 2017-06-29T16:14:50.233Z Reads: 54

```
Holy Shit... Those are an amazing deal. I'm jealous af. I'll just mention again. If you are doing a 12S system you will need 36 cells
```

---
## \#50 Posted by: abctheing Posted at: 2017-06-29T20:45:52.842Z Reads: 54

```
Greeat! I am thinking of ordering this right now, does it seem ok: <img src="/uploads/db1493/original/3X/b/9/b9af82b5518ab1d7ccf7c3981ee07e847c45aa53.jpg" width="690" height="441">

Then i will buy this seperate, today/tomorrow: 

36 of these: https://ru.nkon.nl/sony-us18650vtc6.html

BMS: http://www.ebay.com/itm/44V-48V-50-4V-12S-30A-Lithium-ion-Li-ion-LiPo-Li-Polymer-Battery-BMS-PCB-System-/221274094989?hash=item3384f6bd8d:g:30UAAOxy-NVSEdSO

LCD: http://www.ebay.com/itm/LCD-Indicator-Battery-capacity-Tester-voltmeter-12V-24v-36-48V-Lead-acid-Lithium-/221984681155?hash=item33af516cc3:g:Y6cAAOSwwPhWiPF~#rwid

I also need a charger, i think i normal laptop charger will work but i am unsure about voltage and amps. Any suggestions?
```

---
## \#52 Posted by: abctheing Posted at: 2017-06-30T11:22:24.527Z Reads: 42

```
I read on the forum that i need to connect 4 cells in parallel. With 36 cells i'll get 9 of those "parallels" and i'll wire them in series. But that'l only be 33,3 volts? So do i really have to buy 48 cells to get 50 volts? 3,7 * 9 = 33,3 volts

Edit: I can wire 3 in parallell to get 50 volts with 36 cells, but seems like the "magic" number everyone is talking about is 4?  It will be 9450mah, that will be enough right?
```

---
## \#53 Posted by: Decdog Posted at: 2017-06-30T14:03:53.735Z Reads: 43

```
For the gearing, why don't you just by the kit. It will be cheaper. Also, for the batteries, I would suggest getting 37 batteries. Better safe than sorry if you mess up soldering or if you get a dud battery.
```

---
## \#54 Posted by: Decdog Posted at: 2017-06-30T14:08:05.473Z Reads: 51

```
Those wheels look like kegels, so you will need this kit instead. 

diy-electric-skateboard-kits-parts/36t-kegel-pulley-combo-kit/
```

---
## \#55 Posted by: abctheing Posted at: 2017-06-30T14:08:53.663Z Reads: 44

```
Hahaha thanks, didn't even think of buying a kit! Great, i'll buy these diy-electric-skateboard-kits-parts/36t-kegel-pulley-combo-kit/?attribute_motor-pulley=13T+Motor+Pulley&attribute_belt-size=265mm+12mm+Wide

and 37 batteries. The BMS should also be fine i guess :)
```

---
## \#56 Posted by: Decdog Posted at: 2017-06-30T14:14:09.664Z Reads: 49

```
The battery capacitor meter could take up to two months to ship. This ones a couple bucks more and for me, it says free one day shipping with prime.

https://www.amazon.com/dp/B00UY9PY44/ref=cm_sw_r_cp_api_uWLvzb9ZBBYMT
```

---
## \#57 Posted by: twan Posted at: 2017-06-30T14:48:25.478Z Reads: 49

```
Turnigy Aerodrive SK3 - 6374 vs DYI Torque Boards 6374, can someone tell me which one is better? the turning is  $80 vs $120  . Im trying to build my first single drive long board but cant decide on the motor. Whats the difference?
```

---
## \#58 Posted by: abctheing Posted at: 2017-06-30T15:29:16.138Z Reads: 46

```
I was going to buy SK3 but it's sold out so i'm getting Torqueboards instead, only thing i see is that torqueboards has mor watt
```

---
## \#59 Posted by: twan Posted at: 2017-06-30T16:17:29.347Z Reads: 45

```
looks like its instock on hobbyking website
```

---
## \#60 Posted by: abctheing Posted at: 2017-06-30T16:47:02.920Z Reads: 46

```
Not in the "global" warehouse, it said it was in stock, but as soon as i added it to cart it said it was on backorder.
```

---
## \#61 Posted by: abctheing Posted at: 2017-06-30T17:20:46.137Z Reads: 44

```
Just thank everybody who helped me! I just ordered the parts! I would have ordered the completely wrong parts if it hadn't been for you guys so thanks!
```

---
