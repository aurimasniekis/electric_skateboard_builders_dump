# Planning a e-mtb build

### Replies: 3 Views: 761

## \#1 Posted by: Kubbur Posted at: 2018-07-19T01:10:52.995Z Reads: 98

```
so im planning a build for a commuting/forest riding rig and have some questions

**Board**
im not quite sure what board(base plate) to pick, im around 197cm and 140kg, i will be carrying some equipment most of the time so it needs to withstand max 160kg
it seems that the trampa boards are the way to go, are there any alternatives ?
and how many layers (ie ply)?
I will be using straps with the option to use heelstraps

**Trucks/Hangers**
Is there any difference between infinity and vertigo trucks and hangers beside weight ?
I know I need to buy a hanger from etoxx to fit with the driver mech

**drive mech**
*pulleys
I'm not sure about them, too many horror stories and don't think that the dirt will treat them well
*chains
Could be a good idea, open chain system are used on all bicycles but they are usually much higher up so dirt isn't really a problem
*direct drive
This is the way I want to go
https://www.e-toxx-shop.com/trampa/direct-drive/aps-80mm-direct-drive/#cc-m-product-9979266070
I've not heard any bad things about the direct drive(other than a bit of a noise)
Helical gears, are they worth it noise Vs price ?


**ESC's**
now i know that this topic is directly related to the motors i pick
*the original VESC 6 that trampa sells are quite expensive, are they worth it ?
*focboxes
Seems to fail quite often
*EScape's
Seem to be solid, would just have to wait for a community order when the time comes
*flipsky
This is probably the way I'll go, if they can handle the motors 
*others
*Alien
https://alienpowersystem.com/shop/esc/alien-sport-ii-450a-4-24s-esc-hv/
Could this work ?


**Motors**
Go big or go home
https://alienpowersystem.com/shop/brushless-motors/aps8072s-sensored-bldc-motor-250kv-6000w/
Now I know that this is a bit of a high kv paired with the 5:1 gear ratio, loaded top speed should be around 50-60km/h

**Batteries:**
i dont really consider lipos an option, used them in my racing and freestyle quads and while they suit that application okay id rather have something that'l last for this as it will probably be my main transport vehicle

*18650 vs 26650?
18650's are great, i know because i use them in my mech mods every day, but the 26650 offer more throughput per cell(ie max amps pulled)
*samsung25r = 205,83 wh/kg (9wh per cell)
*Ijoy4200mah= 166 wh/kg (15,12 wh per cell)

another thing im considering:
i want the battery to be somewhat modular
i was thinking about building a 12s10p (1080wh) battery
options are
*12*1s10p
*12*12s1p
for me its more logical to build a 12*1s10p than the other, when the battery gets older it would be easy to swap out packs

**Other electronics**
*Bluetooth
Can I only use Bluetooth with the vesc an vesc clones?
What apps are there for Android?
Im thinking about building a rpie pipboy style slate for information screen among other things

*Remote
products/torqueboards-2-4ghz-mini-remote-controller

Any input would be greatly appreciated, also, am I forgetting something?
```

---
## \#2 Posted by: E1Allen Posted at: 2018-07-19T11:37:44.949Z Reads: 59

```
[quote="Kubbur, post:1, topic:62251"]
how many layers (ie ply)?
[/quote]

Trampa website covers ply thickness based on weight.

[quote="Kubbur, post:1, topic:62251"]
I’ve not heard any bad things about the direct drive
[/quote]
Nothing bad so far about enclosed gears.  Belts are fine as well though.

[quote="Kubbur, post:1, topic:62251"]
focboxes
Seems to fail quite often
[/quote]
Being the most used vesc I don't think they fail often, you just hear more stories because they are used by many people.

Two of these is plenty to power you and your board. Especially if you get a nice custom heatsink.

[quote="Kubbur, post:1, topic:62251"]
Could this work ?
[/quote]
That's Overkill

[quote="Kubbur, post:1, topic:62251"]
Go big or go home
[/quote]
Possibly more motor than needed.  6374/6380-84 is good.  You unleash a whole new animal with 80xx motors.  But if you get those I'd go with a lower kv as in 140-190

[quote="Kubbur, post:1, topic:62251"]
for me its more logical to build a 12*1s10p than the other, when the battery gets older it would be easy to swap out packs
[/quote]
You will have a significant amount of wire bundled up. 12 connections.  If you go the 12s1p route you will need 12BMS which would suck.  A purpose built 12s10p would last. With a bms
```

---
## \#3 Posted by: telnoi Posted at: 2018-07-19T11:40:22.761Z Reads: 56

```
[quote="Kubbur, post:1, topic:62251"]
**Board**
im not quite sure what board(base plate) to pick, im around 197cm and 140kg, i will be carrying some equipment most of the time so it needs to withstand max 160kg
it seems that the trampa boards are the way to go, are there any alternatives ?
and how many layers (ie ply)?
I will be using straps with the option to use heelstraps

**Trucks/Hangers**
Is there any difference between infinity and vertigo trucks and hangers beside weight ?
I know I need to buy a hanger from etoxx to fit with the driver mech
[/quote]

Board needs to be a 17 ply. I've got 20 kg less and would not go with 16 ply.

Trucks is mainly a weight difference and a slighty different shape, though that doesn't matter for the e-toxx drive. For strength purposes I would go with the cheaper but heavier infinity trucks. The cutouts are a bit of a weak point and I've seen posts where they bend/deform around those areas.

Those motors are amp hungry (thus no focbox, you'll limit the performance of those motors) . For commuting you want good control/definable parameters for braking and your remote (curves).  Escape or vesc 6 is more reliable. KV is a bit over the top. You should be able to get up to 50 km/h with 200 KV. I reach 42 on 10s with 149kv 6374.
```

---
