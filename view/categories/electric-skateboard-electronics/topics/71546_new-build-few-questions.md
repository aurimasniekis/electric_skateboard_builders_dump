# New build - few questions

### Replies: 5 Views: 434

## \#1 Posted by: paweu54 Posted at: 2018-10-17T16:00:43.954Z Reads: 89

```
Hi everyone,
So I've decited to build my first own electric skateboard. I've chosen all the parts for it, but I have some questions about compatibility and if those are the best I can get for my budget (around 600-700USD), feel free to suggest or share your opinions about my setup!
1. Motor
I have dillema if should i go for double motor, or single one. I live in city, there is no big hills but I don't want to have a problems with riding on them and not overheat my motor. My first thought was to buy two 5055 sk3 motors (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-320kv-brushless-outrunner-motor.html), but I've read that motors with higher KV could fry your VESC/ESC. Here is formula: Numer of cells*voltage*KV*7. If it is under 60k you won't fry your controller. Can you confirm that? After that information I've done some research and many people recomend this 6374 motor (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html). What do you think about it?
2. VESC/ESC
Im still looking for VESC/ESC, what do you think about this Turnigy SK8-ESC (https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html)? Its not cheap, but it looks quality to me. Is it good? Is there one controller for Double motors?
3. Batteries
I've decited to buy 10x18650 Samsung INR18650-35E 3500mah Li-Ion bateries and make 10s from them. Do you know what distance can I travel on those?
4. BMS
Just a regular 10s BMS (https://www.ebay.com/itm/Max-40A-Balance-Battery-Protection-Board-BMS-PCB-For-36V-10S-10Packs-Li-ion-Cell/311862435323?hash=item489c731dfb:g:dUgAAOSwoSFbRdL3:rk:3:pf:0). Is there sense to buy more expensive one?
5. Pulley and motor mount
So here i have another problem, should I buy kit from Ebay or should I depute it to someone to make it. Which option is better? How much gear should big and small have? What size belt should be?
6. Remote controller. 
Just a standard 2.4 Ghz remote controller (https://www.ebay.co.uk/p/2-4g-Electric-Skateboard-Longboard-Wireless-Remote-Controller-Mini-Receiver-W2/2242848397)
7. Charger
i've found this cheap battery charger (https://pl.aliexpress.com/item/42V4A-Charger-10S-36V-li-ion-battery-Charger-Output-DC-42V-With-cooling-fan-Free-Shipping/32760909127.html?spm=a2g17.search0104.3.1.41c1dee9PjKVlL&ws_ab_test=searchweb0_0,searchweb201602_4_10065_10068_318_319_10546_317_10548_10696_450_10084_10083_10618_452_535_534_10304_533_10307_10820_532_204_10843_10059_10884_323_10887_100031_320_10103_448_449,searchweb201603_60,ppcSwitch_0&algo_expid=c6e358b1-8dcd-48d4-9d71-20da8077823a-0&algo_pvid=c6e358b1-8dcd-48d4-9d71-20da8077823a&transAbTest=ae803_4). Do You know, if should I buy like more expensive charger or this one is enough? I don't want my batteries to explode or break.
8. Battery holders
Here are some basic holders (https://www.amazon.com/gp/product/B075N4DLSJ/ref=as_li_ss_tl?ie=UTF8&psc=1&linkCode=sl1&tag=just02b0-20&linkId=ae7716d1c1628ce9d4e6df754b346f8f). I think those are ok, but im open for any suggestions if I should replace them.

Now I'm trying to figure out the mechanical components. Board, Trucks and Board have to wait this problems to be solved. It would be nice to have answers for at least some questions! Thanks for answers! :grinning:
```

---
## \#2 Posted by: linsus Posted at: 2018-10-17T16:11:59.993Z Reads: 74

```
[quote="paweu54, post:1, topic:71546"]
Motor
I have dillema if should i go for double motor, or single one. I live in city, there is no big hills but I don’t want to have a problems with riding on them and not overheat my motor. My first thought was to buy two 5055 sk3 motors (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-320kv-brushless-outrunner-motor.html), but I’ve read that motors with higher KV could fry your VESC/ESC. Here is formula: Numer of cells *voltage* KV*7. If it is under 60k you won’t fry your controller. Can you confirm that? After that information I’ve done some research and many people recomend this 6374 motor (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html). What do you think about it?
[/quote]

Its your first build, you're unexeperienced and on a budget. Do one motor. 6374 packs a hell of a punch anyway.

[quote="paweu54, post:1, topic:71546"]
VESC/ESC
Im still looking for VESC/ESC, what do you think about this Turnigy SK8-ESC (https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html)? Its not cheap, but it looks quality to me. Is it good? Is there one controller for Double motors?
[/quote]
Not sure about the hobbyking ESC. I assembled all of my VESCs by hand and saved money that way instead. 95% of all new builders here facepalm and wonder why things break and learn the hard way that you cant cheap out on the most important hardware. I'd sudgest settling for something midrange like the FOC box or buy a 2nd hand one from someone here, until you figure out whats on the market abit, and what your intended use are (FOC/BLDC, 10s/12s, etc..)

[quote="paweu54, post:1, topic:71546"]
Batteries
I’ve decited to buy 10x18650 Samsung INR18650-35E 3500mah Li-Ion bateries and make 10s from them. Do you know what distance can I travel on those?
[/quote]

Not very far. google esk8 calculator for a decent estimation. Capacity isnt the bottleneck but rather how much current you can draw from your battery, Id recommend a battery capable of atleast minimum 40A continues draw from your pack. on one motor. nothing less.

[quote="paweu54, post:1, topic:71546"]
BMS
Just a regular 10s BMS ([https://www.ebay.com/itm/Max-40A-Balance-Battery-Protection-Board-BMS-PCB-For-36V-10S-10Packs-Li-ion-Cell/311862435323?](https://www.ebay.com/itm/Max-40A-Balance-Battery-Protection-Board-BMS-PCB-For-36V-10S-10Packs-Li-ion-Cell/311862435323?hash=item489c731dfb:g:dUgAAOSwoSFbRdL3:rk:3:pf:0)
[/quote]
try Bestech or Supower, theyre quite popular here.

[quote="paweu54, post:1, topic:71546"]
Pulley and motor mount
So here i have another problem, should I buy kit from Ebay or should I depute it to someone to make it. Which option is better? How much gear should big and small have? What size belt should be?
[/quote]
Look around here on the forum, theres alot of suppliers and sources avaible.

[quote="paweu54, post:1, topic:71546"]
Remote controller.
Just a standard 2.4 Ghz remote controller (https://www.ebay.co.uk/p/2-4g-Electric-Skateboard-Longboard-Wireless-Remote-Controller-Mini-Receiver-W2/2242848397)
[/quote]
Same here, search the forum

[quote="paweu54, post:1, topic:71546"]
Charger
i’ve found this cheap battery charger (https://pl.aliexpress.com/item/42V4A-Charger-10S-36V-li-ion-battery-Charger-Output-DC-42V-With-cooling-fan-Free-Shipping/32760909127.html?spm=a2g17.search0104.3.1.41c1dee9PjKVlL&amp;ws_ab_test=searchweb0_0,searchweb201602_4_10065_10068_318_319_10546_317_10548_10696_450_10084_10083_10618_452_535_534_10304_533_10307_10820_532_204_10843_10059_10884_323_10887_100031_320_10103_448_449,searchweb201603_60,ppcSwitch_0&amp;algo_expid=c6e358b1-8dcd-48d4-9d71-20da8077823a-0&amp;algo_pvid=c6e358b1-8dcd-48d4-9d71-20da8077823a&amp;transAbTest=ae803_4). Do You know, if should I buy like more expensive charger or this one is enough? I don’t want my batteries to explode or break.
[/quote]
Alway match the charger and batteries. Dont assume you're getting what you need by pouring more money into it. More research.

[quote="paweu54, post:1, topic:71546"]
Battery holders
Here are some basic holders (https://www.amazon.com/gp/product/B075N4DLSJ/ref=as_li_ss_tl?ie=UTF8&amp;psc=1&amp;linkCode=sl1&amp;tag=just02b0-20&amp;linkId=ae7716d1c1628ce9d4e6df754b346f8f). I think those are ok, but im open for any suggestions if I should replace them.
[/quote]
I'd look into buying a pre built pack from someone that welds it properly. If your heart is set on having "holders" you can look up the NESE modules. Again, search the forums how people here build batteries.

Conclution, read more, take notes. Save potential stuff you might consider/want in your build. Come back with more questions.
```

---
## \#3 Posted by: dareno Posted at: 2018-10-18T22:25:56.541Z Reads: 44

```
As a side note to all that lovely info you got there.  I currently run four HK 4.12 vesc and apart from a battery short that killed one they are not a bad unit and the back up from hk is second to none.  They replaced the bad one even though it was my fault.  Good luck
```

---
## \#4 Posted by: Jmding Posted at: 2018-10-18T23:05:22.671Z Reads: 39

```
Consider hobby lipos on the battery side of things.  IMO 18650's dont make sense below 4p setups because of the lack of current capability.  A 3x 4s1p, 5000 mah Zippy lipo packs costs about $120 and will allow you to realize much higher torques
```

---
## \#5 Posted by: paweu54 Posted at: 2018-11-07T13:10:45.654Z Reads: 23

```
Hi again,

thanks for suggestions, I've done some research and here are some changes I would like to apply:

Engine : https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html .
I've decited to buy this one, because there is discount on it. 

ESC + Remote controller : https://www.enertionboards.com/raptor-accessories/enertion-nano-x-focbox-sales-bundle/
I have seen many topics about focbox and many people recomend it. Also there is nice bundle with the controller. Btw what do you think about FLIPSKY esc? I've seen some recomendations as cheap esc.

Batteries : 4x https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack-xt90.html
I chose lipos over li-ion, because they are much easier for first build. Four of them will work with engine I chose. What do you think about it?

Bms : https://pl.aliexpress.com/item/SuPower-12S-43-2V-44-4V-50-4V-60A-Li-ion-Lithium-LiPo-Battery-BMS-Management/32800557987.html?spm=a2g17.search0104.3.34.ff3d454eCqWABh&ws_ab_test=searchweb0_0,searchweb201602_4_10065_10068_10890_5730315_319_10546_10548_317_10696_5728811_453_10084_454_10083_10618_5729215_10304_10307_10820_537_536_5733215_5733315_10843_328_10059_10884_5733115_10887_100031_321_5733413_322_5732515_10103_5733613_5733513-10890,searchweb201603_55,ppcSwitch_0&algo_expid=e43e8019-8d09-440a-abe1-e7e3fa12afc9-5&algo_pvid=e43e8019-8d09-440a-abe1-e7e3fa12afc9

Here is SuPower you recomended to me. I think it's good choice.

Charger : https://pl.aliexpress.com/item/50-4-V-2-5A-Li-ion-Bateria-ithium-ion-battery-charger-12-S-44-4/32884605169.html?spm=a2g17.search0104.3.267.2eb07e536DASSt&ws_ab_test=searchweb0_0%2Csearchweb201602_4_10065_10068_10890_5730315_319_10546_10548_317_10696_5728811_453_10084_454_10083_10618_5729215_10304_10307_10820_537_536_5733215_5733315_10843_328_10059_10884_5733115_10887_100031_321_5733413_322_5732515_10103_5733613_5733513%2Csearchweb201603_55%2CppcSwitch_0&algo_pvid=83e37078-2644-4052-96ca-1f5fa08b2d2f&algo_expid=83e37078-2644-4052-96ca-1f5fa08b2d2f-36

I chose it, because it matches my batteries.

I've decited to buy pulley and motor mount from this forum. : https://www.electric-skateboard.builders/t/15-20-boardnamics-caliber-motor-mounts/73643 + https://www.electric-skateboard.builders/t/15mm-wide-pulley-kits-wheel-motor-pulleys-belts-and-hardware/17131

What do you think? Thanks for answers!
```

---
