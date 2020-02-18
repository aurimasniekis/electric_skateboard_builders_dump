# Need help understanding battery discharged/current

### Replies: 19 Views: 183

## \#1 Posted by: CrimzonGryphon Posted at: 2018-11-04T17:48:32.957Z Reads: 57

```
To give you a bit more context, here's what I'm trying to decide between:

So I'm deciding now between building a 8s2p battery with Samsung 30Q cells:

[Cells]( https://ru.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html)

[BMS](https://www.aliexpress.com/item/8S-18A-25A-45A-60A-18650-BMS-PCB-for-24V-Li-ion-LiFePO4-battery-pack-for/32845939599.html?spm=2114.search0104.3.8.70737227tE3Zll&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10547_319_317_10548_10696_10192_10190_10084_10083_10618_10307_10820_10821_10301_10303_328_10059_10884_10887_100031_321_322_10103,searchweb201603_55,ppcSwitch_0&algo_expid=acf32f64-ac84-4a3c-b260-316efe16eaef-1&algo_pvid=acf32f64-ac84-4a3c-b260-316efe16eaef) (they provide 3.6v BMS too)

Or just buying a couple of Hobby King Lipos (series of parallel) and saving myself some time. From what I see they cost roughly the same.

The main difference I see between the two is the c-rate or the max currents. The Samsung cells offer 15A output which intuitively would double in parallel while most lipos offer (5AH*25c) 125A! Ok so a huge difference, I'd need a number of parallel cells to keep up. But maybe 125A is overkill, I'm really only interested in finding the minimum output current required for my use case.

Also, "Burst" output is often mentioned. Is this the output while I'm going at full throttle or is it usually only achieved when going up hills or accelerating from a standstill? There is no mention of "burst" or anything like that on the samsung cells so I don't really know how they'll handle on an eSkate.

And finally: If I made it well, and without mistakes, is £75 a good deal for the BMS/Cell combo? 6000Mah + long lasting cells, only downside seems to be that it's limited to 30A possibly.

If you need to ask me a question (about my build plan) before you can answer mine feel free. I've only taken an interest in eSkates this weekend so I'm a bit of a noob and my mind is numb from research.

Thank you to Peter Griffin and the Aku Aku mask guy and everyone else who's in  pretty much in every thread.

PS I searched already

Maybe won't be able to reply to everything tonight.
```

---
## \#2 Posted by: linsus Posted at: 2018-11-04T17:59:10.499Z Reads: 49

```
Current depends on your load. You havnt specified what you want to see from your batteries so far. So its really hard for us to guess. Any single motor setup with some gearing would be alright with 40 or 50A contineuous drain. Top Peak current is refered to when the motor is hungry and wants current to do something. Applicable scenarios in esk8 would be start from stand stil, uphill climbing (moderate distance), and probably the most demanding, start from stand stil uphill.

With that said, we have no Clue what your setup is, what you expect from it, if you can weld cells or what your budget are. Gives us those and we can help further
```

---
## \#3 Posted by: CrimzonGryphon Posted at: 2018-11-04T18:31:06.637Z Reads: 45

```
[Motor](https://www.aliexpress.com/item/free-shipping-RCMOY-5065-50-65-270KV-Heavy-duty-brushless-Sensored-motor-2-6KG-3-8S/32822281393.html?spm=2114.search0104.3.167.11585dc4disNAN&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10547_319_317_10548_10696_10192_10190_10084_10083_10618_10307_10820_10821_10301_10303_328_10059_10884_10887_100031_321_322_10103,searchweb201603_55,ppcSwitch_0&algo_expid=060e5da9-e614-4026-84e3-a5c67bfa194e-24&algo_pvid=060e5da9-e614-4026-84e3-a5c67bfa194e) Single, belt.

Gear ratio is 3:1
 
Wheels are 190mm

I weigh 160lbs

Have yet to find a VESC.

I live in a relatively flat area although I'd like to use it in other places that may be hillier. It's mostly for getting around the city.

I need the batteries to have at least a range of around 8 miles which should be fairly achievable. Top speed should be at the very least 10mph.
```

---
## \#4 Posted by: deucesdown Posted at: 2018-11-04T18:36:54.981Z Reads: 45

```
10s4p (40 cells) has pretty much become the minimum standard for any kind of performance. This is more for power output (voltage x amperes) rather than range. Anything less than this, you're giving up something. Lipos can get you to the minimum power level for cheaper but there are many tradeoffs.

Chinese hubs like meepo can get a lot out of less power. Not anything like the usual 10s4p or greater builds, but if you're not ready for the commitment :) maybe pick up one of the chinese prebuilts instead? And when you get bored or it breaks, expand the budget and come back?
```

---
## \#5 Posted by: psychotiller Posted at: 2018-11-04T18:39:05.254Z Reads: 38

```
I would say, if you're not going to at lease use 30 cells, don't waste your time or money.
```

---
## \#6 Posted by: deucesdown Posted at: 2018-11-04T18:42:09.644Z Reads: 37

```
Btw you're doing good looking at the battery pack first.
```

---
## \#7 Posted by: PXSS Posted at: 2018-11-04T18:42:45.091Z Reads: 36

```
What they said. 
You are trying to put a tiny battery on a tiny motor to push 7"+ sized wheels? Good luck. 

I would get either smaller wheels, way smaller (83mm)

Or beef up everything else. 

It might be a really good commuter compact board but you have to match components appropriately
```

---
## \#8 Posted by: b264 Posted at: 2018-11-04T18:45:43.807Z Reads: 34

```
Use Lipo.  Also check the prices on LiFePO4 bricks.  Don't use 18650

LiFePO4 will be heavy but will last a long time.  But I can't remember if it's cheaper or more expensive.
```

---
## \#9 Posted by: Sebike Posted at: 2018-11-04T18:46:56.337Z Reads: 31

```
The "burst" isn't really a helpful spec in any way other than giving you an idea of what the cell is capable of delivering for a very short amount of time. It does not mean that the cell is intended to feed that current even for a short amount of time and it does not mean that the cell won't take damage when delivering that current. It most probably will affect cell life/damage the cell aso. 
(There isn't a standard for the sc burst or pulse, so you have no idea what the manufacter even means by this rating, ie how it is measured /if it is measured.)

The rated constant discharge current is the maximum of what you should pull from the cell (given that you keep working temperatute within ok limits) if you want to have a somewhat ok cell performance for (a given) x amount of cycles.
```

---
## \#10 Posted by: CrimzonGryphon Posted at: 2018-11-04T18:52:29.673Z Reads: 31

```
[quote="Sebike, post:9, topic:73410"]
he “burst” isn’t really a helpful spec in any way other than giving you an idea of what the cell is capable of delivering for a very short amount of time. It does not mean that the cell is intended to feed that current even for a short amount of time and it does not mean tha
[/quote]

By bigger motor do you mean I need the dimensions to be bigger or do I need more torque and power or both? Should I be looking at a >170Kv motor maybe?
```

---
## \#11 Posted by: deucesdown Posted at: 2018-11-04T18:54:20.275Z Reads: 30

```
The cheapest pack that won't self destruct in a handfull of rides or cause other big headaches is probably 3 of these 

https://hobbyking.com/en_us/turnigy-battery-5000mah-3s-40c-lipo-pack-xt-90.html

The 30c versions might work but might puff up in a fewsrides.

This is 9s at $120. I would consider this bottom of the barrel.

The pack is the heart of the system. If you start with a good pack you always have a chance to make things work.

Bad packs can be money down the drain or a bad fire.

It's not worth talking about the other components until you get the pack in the right ballpark.
```

---
## \#12 Posted by: Sebike Posted at: 2018-11-04T18:56:57.196Z Reads: 35

```
I guess this question was aimed at someone else.. I never mentioned motors 🙂
```

---
## \#13 Posted by: b264 Posted at: 2018-11-04T18:58:05.337Z Reads: 34

```
This would last a LOT longer on a tight budget.  It will be heavier though

https://www.alibaba.com/product-detail/36v-ebike-battery-Lifepo4-battery-pack_60780315682.html

edit: *Nevermind, it's 1C discharge.*

There is a pack that looks like that that is 12S (43.8V) and 5Ah (also 10Ah version) that works great but I can't find it right now.
```

---
## \#14 Posted by: deucesdown Posted at: 2018-11-04T19:40:32.834Z Reads: 28

```
lifepo4, except for A123, usually I see lots of voltage sag? Even those crazy output rated headways.
```

---
## \#15 Posted by: b264 Posted at: 2018-11-04T19:41:11.291Z Reads: 27

```
Mine has little sag at all but it's on a single drive 6374
```

---
## \#16 Posted by: CrimzonGryphon Posted at: 2018-11-04T19:41:31.441Z Reads: 30

```
Yeah I misclicked. it was at pxss
```

---
## \#17 Posted by: CrimzonGryphon Posted at: 2018-11-04T22:16:59.173Z Reads: 25

```
Does[this](https://www.aliexpress.com/item/6374-170KV-Brushless-Motor-With-Hall-Sensor-3000W-Electric-Off-Road-Skateboard-Engine-M10-Motor-Shaft/32920671561.html?spm=2114.search0104.3.23.58f72635p4KYlZ&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10547_319_317_10548_10696_10192_10190_10084_10083_10618_10307_10820_10821_10301_10303_328_10059_10884_10887_100031_321_322_10103,searchweb201603_55,ppcSwitch_0&algo_expid=d31d2649-a0c2-4b6d-870b-7f92d6fc3f2f-3&algo_pvid=d31d2649-a0c2-4b6d-870b-7f92d6fc3f2f) seem decent.

Not quite sure what the thing it's attached to is, could be a VESC but it doesn't look like it has anything on it to dissipate heat.
```

---
## \#18 Posted by: CrimzonGryphon Posted at: 2018-11-04T22:20:52.983Z Reads: 23

```
I'm gonna ask my Uni's lab technician if they have any batteries I can buy off them before I search anymore. Also does[this motor](https://www.aliexpress.com/item/6374-170KV-Brushless-Motor-With-Hall-Sensor-3000W-Electric-Off-Road-Skateboard-Engine-M10-Motor-Shaft/32920671561.html?spm=2114.search0104.3.23.58f72635p4KYlZ&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10130_10068_10547_319_317_10548_10696_10192_10190_10084_10083_10618_10307_10820_10821_10301_10303_328_10059_10884_10887_100031_321_322_10103,searchweb201603_55,ppcSwitch_0&algo_expid=d31d2649-a0c2-4b6d-870b-7f92d6fc3f2f-3&algo_pvid=d31d2649-a0c2-4b6d-870b-7f92d6fc3f2f) seem any good.

I'm probably not going to get the controller or whatever that comes with it.
```

---
## \#19 Posted by: b264 Posted at: 2018-11-04T22:30:14.211Z Reads: 23

```
That is the correct type of motor, but the kv you need will depend on the battery.  Also, I don't know if that vendor is good.  If you get low-quality stuff, you might have little customer service unless you live inside China with that vendor.

So get the battery sorted-out first.
```

---
