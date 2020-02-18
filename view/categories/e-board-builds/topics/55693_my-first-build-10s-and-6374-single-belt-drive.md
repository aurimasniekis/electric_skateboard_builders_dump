# My First Build - 10S and 6374 Single Belt Drive

### Replies: 50 Views: 2655

## \#1 Posted by: blaccIX Posted at: 2018-05-16T19:50:14.455Z Reads: 390

```
Hello everyone, I already intended to build my first board last year, but the summer ended so I dropped it in the hope of building it this year. I haven't completely decided about what parts to use yet, but I kind of know what I'm aiming for. So I would try to build a board with a **single 6374 motor**, **10S battery**, and **VESC**. Also, I'm located in Europe.

**VESC**: Probably going to use the **Focbox** (or is there another viable option that isn't overly expensive)
**Motor**: Bought the APS 6374 HEV 170kv - http://alienpowersystem.com/shop/brushless-motors/aps-6374hev-outrunner-brushless-motor-170kv-3300w/
**Remote**: GT2B with a custom case looks like the most reliable way to go.
**Battery**: I have decided that I'll get a 10s4p Li-ion pack from a local battery builder, I currently don't which cells he uses, but I'm sure I can have it built with samsung 30q or some other cells that are good for esk8.

Mechanical Parts :
**Wheels**: 97mm flywheel clones 73A -https://eskating.eu/product/new-73a-duro-electric-skateboard-wheels-90-97mm-black/
**Trucks**: 50° Caliber II from @e.board_solutions 

Drive system :
I think I'll use 15/40 gearing (15mm wide)
**Motor pulley**:15mm wide, 10mm bore, 15t steel pulley - https://eskating.eu/product/custom-htd-5m-12-to-20-teeth-steel-motor-pulley-in-9121520-width/
**Wheel pulley**:15mm wide 40t flywheel pulley - https://eskating.eu/product/htd-5m-363840-teeth-nylon-carbon-abec-11-flywheels-wheel-pulley/
**Belt**: Haven't calculated the length yet, but I'll buy it from eskating.eu

Other parts :
**Motor mount**: Caliber V2 mount from @e.board_solutions
**Enclosure**: Not sure yet, might try diy fiberglass 
**Deck** : I'm going to use the deck from my [Brunotti Boxter](https://www.brunotti.com/nl/boards/longboards/boxter-22517.html), maybe I'll later upgrade to a loaded vanguard.

Thanks,
BlaccIX
```

---
## \#2 Posted by: moon Posted at: 2018-05-16T19:56:40.137Z Reads: 349

```
For the trucks you don't have many options - just because of what motor mounts are available

You could use 

* Caliber trucks
* Caliber clones
* The ones used by evolve
* TB 218mm trucks


Similar things for the wheels

* ABEC 11 Flywheels (or clones)
* Orangatang Kegels

(or any wheel with the same core)

Motor and VESC sounds good

Does your deck flex?
```

---
## \#3 Posted by: blaccIX Posted at: 2018-05-16T20:11:24.438Z Reads: 325

```
I was going to use 44-degree Caliber II trucks and 97mm flywheel clones, my deck is a bamboo-fiberglass sandwich, it flexes, but since I'm pretty lightweight I don't think it'll be a much of a problem.
```

---
## \#4 Posted by: moon Posted at: 2018-05-16T20:12:55.931Z Reads: 313

```
You should think about how you mount your electronics then

Like how the boosted v1 does
```

---
## \#5 Posted by: Jones_Blake Posted at: 2018-05-17T08:30:46.233Z Reads: 284

```
My skateboard GS01 with hub drive motor, 500W, 36V, whose speed can reach to 12mph.
```

---
## \#6 Posted by: Peter90 Posted at: 2018-05-17T08:46:36.036Z Reads: 283

```
I have almost the same setup what you planning but on a mountainboard trampa:

single
FocBox
motor sk3 6374 192kv 
nano-x remote
4 x 5s 5000mah = 10s10000mah
gears 15/72

This setup is realy good. I can reach 55km/h without any problem but i have big tires 8". Range is around 15/18 km its depend on your ride style. I can go up the hill and still speedup.
```

---
## \#7 Posted by: rey8801 Posted at: 2018-05-17T09:07:23.044Z Reads: 266

```
Hi!
The Vesc and motor you picked are good for a 10S battery. For the deck you have to pay attention to the flex. If it flex then either you make it stiff by adding carbon fiber or fabirglass or you split your enclosure in two part, front and back. For the trucks few are compatible with the motor mount available (as moon said). THe last thing the battery. I build mine recently for the first time. It is not that difficult but you nned a spot welder. I made my custom one for the occasion from a microwave trasformer and an arduino I had at home. My suggestion is ho for it if you have the time to spend in learning and the money for a spot welder, otherwise you could either ask to one of the guy of the forum to build the Liion pack for you. I would suggest stick with Liion if possible, othersie LiPo it's also fine, then the soldering skill needed are really basic and yes connecting a BMS will allow you to simple recharge them with a normal charger.
Good luck!
```

---
## \#8 Posted by: blaccIX Posted at: 2018-05-17T09:16:40.440Z Reads: 247

```
Thanks! I think I'll try to use a boosted style enclosure
```

---
## \#9 Posted by: blaccIX Posted at: 2018-05-17T09:17:30.970Z Reads: 237

```
Do you use a BMS for the LiPo-s?
```

---
## \#10 Posted by: Peter90 Posted at: 2018-05-17T09:30:18.078Z Reads: 236

```
No, I have a imax b6 charger and I have to charge every battery separately.
I considering to buy a charging board to connect all 4 batteries and charging them in one time.
```

---
## \#11 Posted by: mixedcreation Posted at: 2018-05-17T09:37:26.803Z Reads: 230

```
There are plenty of lipo folks that run bms. Just do a quick search and you will find good information for those that run with bms.
```

---
## \#12 Posted by: blaccIX Posted at: 2018-05-30T17:06:50.829Z Reads: 211

```
**Update**:

I have updated and completed the parts list, added
 some links and bought motor, motor mount and trucks.
```

---
## \#13 Posted by: blaccIX Posted at: 2018-05-30T17:09:11.937Z Reads: 202

```
Does anyone know what's the size of the bullet connectors the APS 6374 motor has?
```

---
## \#14 Posted by: Benjamin899 Posted at: 2018-05-30T17:27:03.217Z Reads: 212

```
just write him an email. he response quite fast, but it probably won't be 4mm connector.
Btw just a tip, since this build will go fast, try to do a split between the axles. Like 50° front and 44° rear, i did it on my board and stabilized my board at high speeds.
I recommend reading up on this thread, loads of good info about bushings ect.
https://www.electric-skateboard.builders/t/bushing-set-up-help/42036
```

---
## \#15 Posted by: blaccIX Posted at: 2018-05-30T17:47:56.481Z Reads: 200

```
thanks for the suggestions, I look into it
```

---
## \#16 Posted by: blaccIX Posted at: 2018-06-05T16:08:22.513Z Reads: 202

```
Does anyone have some suggestions or ideas for a 10s4p 18650 Li-ion split enclosure? Would be great if it was made for the Vanguard. So far I've considered diy fiberglass, 3d printing and @Eboosted Vanguard enclosure.
```

---
## \#17 Posted by: Eboosted Posted at: 2018-06-06T02:54:12.620Z Reads: 202

```
I have the Vanguard set in stock waiting to be bought :blush: , let me know
```

---
## \#18 Posted by: blaccIX Posted at: 2018-06-09T14:12:31.249Z Reads: 204

```
Just recieved the APS motor, looks like it's decent quality. Still trying to figure out how to save costs on the enclosure.
![20180608_225216|374x500](upload://pOc7RbXyuN9kt45X5CFeUaA8UDb.jpg)
```

---
## \#19 Posted by: Benjamin899 Posted at: 2018-06-09T14:29:59.043Z Reads: 198

```
if you go DIY fiberglass don't forget you have to calculate the costs for the molds.
```

---
## \#20 Posted by: blaccIX Posted at: 2018-06-09T15:58:03.814Z Reads: 190

```
Kinda torn towards kydex atm. Should be cheap and reliable?
```

---
## \#21 Posted by: Benjamin899 Posted at: 2018-06-09T16:39:17.514Z Reads: 173

```
Kydex is reliable or ABS but it is expensive compared to fiberglass
```

---
## \#22 Posted by: blaccIX Posted at: 2018-06-11T22:44:03.794Z Reads: 172

```
Just ordered the Focbox from enertion's own website during the sale. I'm hoping the support guy was right when he told me that it'll take approx 2-3 weeks to ship it to EU.
```

---
## \#23 Posted by: blaccIX Posted at: 2018-06-12T10:42:20.833Z Reads: 167

```
Should I make the enclosure's mold out of wood or is there anything easier to use?
```

---
## \#24 Posted by: Sn4pz Posted at: 2018-06-12T13:52:57.060Z Reads: 173

```
sort of off topic but have you seen the enertion sale for the focboxes? :D 

This would be a great time to pick one up!

(i also picked this up: http://www.electric-skateboard.builders/t/dual-focbox-fully-enclosed-cnc-machined-case/42321 aparpently it helps temperatures significantly)\

edit: lol woops... jumped the gun :laughing:
```

---
## \#25 Posted by: rey8801 Posted at: 2018-06-12T14:05:41.797Z Reads: 167

```
I made my mold with a 3D printer. Otherwise, wood, cardboard will all work. IT depends, how complicate is your design. Keep in mind that is not that true that kydex and ABS are more expensive. If you can make a vaccum pump (there are tutorial online, it's pretty easy) than the total cost would be more with fiberglass. I went for fiber glass and I paid 30 euro for the material without any gel coat or fancy stuff. I found ABS, Kydex sheets on ALi, Ebay for less than 20 euro. To me depends of what you would like as final result.
```

---
## \#27 Posted by: rey8801 Posted at: 2018-06-12T17:22:34.727Z Reads: 157

```
I have found some kydexs at good price in EU, if you need it I can have a look if I find them
```

---
## \#28 Posted by: brenternet Posted at: 2018-06-12T18:45:21.073Z Reads: 153

```
You can make it out of dense foam and wrap it in duct tape for kydex, really easy to hype angles to attract ladies.
```

---
## \#29 Posted by: blaccIX Posted at: 2018-06-27T10:05:34.667Z Reads: 144

```
Got some kydex from amazon, recieved the FOCBOX.  Also I got refunded on the GT2B I ordered from amazon (it got stuck in the customs somewhere) and because enertion's having this huge sale now for the Nano-X I'm going to use it instead of a custom gt2b.
```

---
## \#30 Posted by: carwyn987 Posted at: 2018-06-29T23:30:10.310Z Reads: 147

```
[quote="Peter90, post:6, topic:55693"]
10000mah
[/quote]

I have a very similar setup...
single motor 190kv 6374
4 x 3s 5000mah = 12s5000mah
gears 16/40
controller is phone to created bluetooth application that runs on rfduino.

Tires are only 90mm tho lmao

I really hope my range(without damaging batteries) is at least 10 miles because I have to commute 5 miles to work and back and I don't have enough money to buy 4 more lipo 3s batteries
```

---
## \#31 Posted by: Exigent Posted at: 2018-06-30T22:28:58.948Z Reads: 141

```
I've used kydex with decent results in a number of different projects (battery enclosures, accessory holsters, splash shields, etc). If this is your first time with kydex, experiment with a scrap piece first to get a feel for the material.
```

---
## \#32 Posted by: blaccIX Posted at: 2018-07-04T20:53:41.048Z Reads: 129

```
Recieved a lot of stuff today, including 97mm wheels. Sadly I'm getting pretty strong wheelbite with those, I'm currently using 1/8 inch risers.
I think I'll change them to 1/2 inch risers. Does anyone have some other suggestions?

Thanks
```

---
## \#33 Posted by: ashe Posted at: 2018-07-04T21:48:46.970Z Reads: 121

```
risers are a good option, ive seen some people stick some course sandpaper to their wheels and actually carve out bigger wheel wells from the board. you can also stiffen up the bushings of your trucks, but that will make the board less carvy
```

---
## \#34 Posted by: Sender Posted at: 2018-07-05T08:45:14.089Z Reads: 113

```
Also bushing setup can help a lot with wheel bite.  Some harder board side bushings would help
```

---
## \#35 Posted by: blaccIX Posted at: 2018-07-06T14:34:57.810Z Reads: 109

```
Went to a local battery guy today. He showed me the elements he wants to use. They were Samsung 29E. As far as I know they're not the best for eboards? I'm planning to use 10s4p, I have a single 6374 motor.
```

---
## \#36 Posted by: moon Posted at: 2018-07-06T14:41:25.986Z Reads: 108

```
30q is the best
```

---
## \#37 Posted by: blaccIX Posted at: 2018-07-06T15:05:55.990Z Reads: 117

```
How much will the lower discharge rate of 29E actually influence me when using 10s4p?
```

---
## \#38 Posted by: blaccIX Posted at: 2018-07-09T14:49:30.274Z Reads: 112

```
Can anyone link me the Bestech BMS with an e-switch? Do I have to contact them to order it?
I'm going to order 40 30Q sells and have my local battery guy build the battery for 50€.
```

---
## \#39 Posted by: moon Posted at: 2018-07-09T14:52:37.013Z Reads: 109

```
You have to email them and order at least 2 BMS
```

---
## \#41 Posted by: blaccIX Posted at: 2018-07-09T15:04:42.843Z Reads: 108

```
Okay, thanks for the quick reply
```

---
## \#42 Posted by: mixedcreation Posted at: 2018-07-09T16:04:43.153Z Reads: 105

```
@JLabs sells them.  

[BMS](https://buildkitboards.com/)

Wait, you need 12s... I think the highest series he sells is 10s.  But you can always ask.
```

---
## \#43 Posted by: JLabs Posted at: 2018-07-09T16:18:20.827Z Reads: 99

```
I have the 12s but am out of stock. When I get them in stock I will put them back up on the website

Thanks for the shout @mixedcreation
```

---
## \#44 Posted by: blaccIX Posted at: 2018-07-09T16:35:48.468Z Reads: 89

```
I need 10S tho, but I'm in europe.
```

---
## \#45 Posted by: moon Posted at: 2018-07-09T16:48:12.178Z Reads: 90

```
10S 80a or 10S 60a?
```

---
## \#46 Posted by: blaccIX Posted at: 2018-07-09T17:27:40.421Z Reads: 87

```
Well I think I can handle with 60A, but I'd really love to have an e-switch.
```

---
## \#47 Posted by: TdeBeer Posted at: 2018-07-09T17:55:47.233Z Reads: 89

```
Hey there guys, I pretty much have the same setup except the batteries which is a single 10s3p pack. It is currently a street setup but I would like to set it up like a Trampa electric Mountainboard, single drive, 6374 170KV motor, ESC, Nano-X remote etc. 

Any suggestions as to how I could do this and where would be a good place to get the parts needed to make it like a trampa EMTB
```

---
## \#48 Posted by: mixedcreation Posted at: 2018-07-09T19:05:34.080Z Reads: 81

```
Doesn't hurt to ask how much..just saying.  Still be cheaper than buying two from Bestech.  Jlabs sells one.  Just saying.
```

---
## \#49 Posted by: moon Posted at: 2018-07-09T19:14:52.103Z Reads: 82

```
I have a unused one. Want to PM?
```

---
## \#50 Posted by: blaccIX Posted at: 2018-07-09T19:25:37.839Z Reads: 82

```
If it's 10s, 60+a and has e-switch then yes, sure.
```

---
## \#51 Posted by: moon Posted at: 2018-07-09T19:35:22.615Z Reads: 82

```
Yeah its a bestech one, I am not sure if I can sell it yet. I will have to see if I can get get a replacement one
```

---
## \#52 Posted by: blaccIX Posted at: 2018-08-28T00:38:04.251Z Reads: 64

```
I've recieved all the parts, assembled the board and got it up and running. I still have to make the kydex case, but I guess it can't be that hard. Something that I noticed on my test rided (I mounted everything with duct tape lol)
is that my acceleration was way too agressive and braking was really slow, even if I pushed the throttle fully down.
Im currently using 10s4p made of 30Q cells, focboc, single 6374(36/15 gearing) and a nano-x remote
battery max is 60a and min is -16a
```

---
