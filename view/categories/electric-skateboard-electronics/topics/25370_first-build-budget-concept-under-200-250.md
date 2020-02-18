# First build - Budget concept under £200 ($250)?

### Replies: 9 Views: 1660

## \#1 Posted by: MattC Posted at: 2017-06-14T15:05:04.304Z Reads: 135

```
This is a design I have been working on for a while now to try and reduce the price down as much as possible to create a board which is no Boosted Board but no toy either. 

I am looking for advice on any errors in the design (specifically in the electronics) and improvements which are not too expensive.

This project does not need to meet a specification for a specific use (apart from a low price) but is more of a project.

The current planned parts are:
ESC - FVT 120A - £40
Battery - ZIPPY Flightmax 5000mAh 3S1P 20C - £40
Motor - Brushless Sensored Motor 5065 50 65 270KV 1820W £35
Motor mount and drive system - Electric Skateboard Accessories Belt Motor Bracket Pulley For 72MM Wheel from BangGood - £20
Controller - 2.4GHz Radio Remote Controller from BangGood - £10
Board - Osprey longboard 38" - £40
Connectors - 1 HXT to T and 1 ESC extension lead to connect cells together - £7.50
Total = £192.50

Calculations:
Approx. top speed = 26 km/h without weight
Appox. range = 9 km

Any help would be appreciated.

Thanks

Links:
https://www.banggood.com/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-Skateboard-ESC-p-985970.html
https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html
http://www.ebay.co.uk/itm/Brushless-Sensored-Motor-5065-50-65-270KV-1820W-For-Electric-Skate-Scooter-3-8s-/201945011419?hash=item2f04dc54db:g:JNUAAOSwuMZZMjCx
https://www.banggood.com/Electric-Skateboard-Accessories-Belt-Motor-Bracket-Pulley-For-7270MM-Wheel-p-1104585.html?rmmds=search
https://www.banggood.com/2_4GHz-Radio-Remote-Controller-Receiver-Transmitter-For-Electric-Skateboard-p-1125575.html?rmmds=search
http://www.ebay.co.uk/itm/Osprey-38-Complete-Skateboard-Twin-Tip-Longboard-Cruiser-Text-Blue-White-/332089899067?hash=item4d5219b83b:g:u20AAOSwZ4dZJXdb
```

---
## \#2 Posted by: Smorto Posted at: 2017-06-14T16:45:20.772Z Reads: 102

```
What trucks and wheels do you plan on using? Finding a trucks and wheels to fit that mount/pulleys may be tricky. I am also not sure if that motor and hat mount would work together. I would recommend caliber trucks and DIYES motor mount along with some 3d printed pulleys if you can print them or just finding some HTD 5 pulleys online. You can also find belts from Vbelt supply for pretty cheap.
```

---
## \#3 Posted by: MattC Posted at: 2017-06-14T17:21:08.558Z Reads: 93

```
I have already checked if the motor fits to the hat mount and it does so that should be fine. I am still doing research to try and find a complete board which will fit well with the mount from BangGood just because that mount system is so much cheaper than any alternative. Thank you for the information about the Caliber trucks, they look like they may be useful. Thank you for the help with this.
```

---
## \#4 Posted by: Rrosmo Posted at: 2017-06-14T17:43:30.153Z Reads: 86

```
I have made pretty similar setup with cheap ebay parts and they do actually work (Overall cost about 150€ since I had a longboard already). I have the same remote (15€), motor mount & pulley kit (17€) and similar motor (35€). 

-Remote works fine, never had problems with it. 
-Motor mount is suitable for pretty much all trucks with round profile, BUT it is a bit sketchy if you dont tighten it HARD and use loctite.
-I would recommend to get a motor mount & pulley kit with 15mm wide belt or then buy them from some place else. I had the 9mm belt and it started skipping in every uphill. On ebay there are kits with the same parts but with wider belt and pulleys for the same price.

I have 4 x 11,1V 2200mah lipos wired 2s2p and get about 7-8 km of range depending highly on driving style.

Also something weird happened in my build because it was meant to have top speed around 28km/h or so but it is actually 37km/h on flat surface, so the kv number of those china-motors might not be the most accurate. And yes, the motor is powerful since I weight 95kg and it moves me like a child.
```

---
## \#5 Posted by: MattC Posted at: 2017-06-14T17:52:38.654Z Reads: 71

```
Thank you for all that useful information, that is seriously helpful. 
Can I ask what sized wheels you are using and how you attached the motor mount and pulley kit to your wheels?
Thanks.
```

---
## \#6 Posted by: Rrosmo Posted at: 2017-06-14T18:03:44.039Z Reads: 69

```
Im using a Madrid deck with drop-through trucks and 70mm wheels. I drilled through my wheels and put a spacer between the wheel and the pulley. The 36T pulley had a hole of 20mm which is the diameter of the wheel bearing. Put a bearing in the pulley and place the wheel and the pulley (with bearing) on 8mm pole or your truck and attach them together with tape. Then just use upright drill to drill holes through the wheel and the pulley. Also recommended to use a big washer on the opposite side of the pulley.
Cheers.
```

---
## \#7 Posted by: MattC Posted at: 2017-06-14T18:28:44.163Z Reads: 65

```
Thank you for that advice. I am now trying to find a board with trucks that will fit onto the mount nicely. Do you believe that most rounded trucks will fit this mount then?
Also, does it need to be rounded most of the way down from the center or can there be a reasonable amount of support metal but still a good amount of rounded truck?
Thanks
Edit: I was considering the below board due to its 70mm wheels and very rounded trucks.
http://www.ebay.co.uk/itm/Longboard-Complete-Skateboard-Cruiser-Kicktail-9-Bamboo-Maple-ABEC-11-PU-Wheels/112219490166?_trksid=p2045573.c100506.m3226&_trkparms=aid%3D555014%26algo%3DPL.DEFAULT%26ao%3D1%26asc%3D43782%26meid%3D70338c8a3b5a4143aa88f5c4ed67f380%26pid%3D100506%26rk%3D1%26rkt%3D1%26
Edit 2: I have now changed this board back to a classic longboard as it will be larger and a better ride with electric power in my opinion.
```

---
## \#8 Posted by: Rrosmo Posted at: 2017-06-14T19:10:45.112Z Reads: 59

```
I believe that you can use that board with your build even though board that cheap can be a bit risky. It really doesnt matter how long the "straight" part of the truck is since you can use a metal field (the tool) to shape the reinforced part of the truck. I had to shape my truck just a bit, maybe 0,5m from one spot to get the truck into the mount plates hole. How long the "straight" part should be depends on the width of the wheel and the width of the pulley but by looking the pictures of that board Im guessing you would need to flatten the reinforcement part of the truck for 1-2cm. That will of course make it more likely to bend but this is a budget build after all :smiley:
```

---
## \#9 Posted by: MattC Posted at: 2017-06-14T19:14:30.312Z Reads: 55

```
Thank you again for the great advice on that. Cutting the truck does sound like a good solution.
```

---
