# MTB Lipo or Li-ion

### Replies: 15 Views: 442

## \#1 Posted by: JensSjogren Posted at: 2018-10-01T12:49:57.189Z Reads: 132

```
So i'm just about to do my first build and it's a Trampa mountainboard with 2x 3500 watt motors. I am going to use the board for heavy off road riding in MTB tracks etc. The only part(s) that i have not ordered yet is the battery. Can't decide on what would be the best choice. I've heard that Li-ion batteries sags more during heavy load and it would be great to get some perspective. I'm currently looking at two options, either 4x 6s 6200 mah lipos (https://hobbyking.com/en_us/zippy-compact-6200mah-6s-40c-lipo-pack-xt90-1.html) these are the ones that trampa recomend. The other option is a 12s5p li-ion from eskating.eu (https://eskating.eu/product/square-12s5p-eskating-electric-mountainboard-battery-samsung-30q/). I have no experiance with lipo balance charging and feel like finding a good charger for the lipos is a bit confusing aswell as it seems more time consuming to deal with lipo batteries. 

Anyone has any good input regarding this that could make my choice easier? 

Best regards//Jens
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-01T12:55:42.260Z Reads: 126

```
you can always use a bms for lipos also that shouldn´t be an issue.

to find a blance chager also not so difficult.
just depends how much money you ready to spend for it and how fast it should charge your cells.

for you lipo solution you plan to connect them 12s2p, just to be sure I don´t get anything wrong?
I also assume you will mount the batteries on top of the deck, right?
```

---
## \#3 Posted by: JensSjogren Posted at: 2018-10-01T12:59:39.398Z Reads: 123

```
If i connect a bms to the lipos does that mean that i have to open the pack up to connect wires? Charging time doesnt really matter that much to me. Yes it would be a 12s2p.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-01T13:08:37.752Z Reads: 115

```
no, you don´t need to open the packs.
Just search here for "lipo bms wiring" you will find a lot of examples how to make it.

if you go with lipos in parallel make sure they match each other (should have close the same voltage and IR)

balance charger you can find for cheap "imax b06 ac", expensive I charger.
There even balance charger with which you can charge 4 packs in one (without parallel plug).
```

---
## \#5 Posted by: JensSjogren Posted at: 2018-10-01T18:48:40.089Z Reads: 91

```
Hmm i see, think that this charger would be fine for charging 4 6s lipos at the same time? 

https://hobbyking.com/en_us/turnigy-4x6s-lithium-polymer-battery-pack-charger.html
```

---
## \#6 Posted by: b264 Posted at: 2018-10-01T18:51:47.946Z Reads: 85

```
Just use a BMS and a [regular 12S two wire charger](https://www.banggood.com/50_4V-2A-Power-Adapter-For-Self-Balanced-Vehicle12S-Li-ion-Battery-Charger-p-1201167.html?), not a hobby charger
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-01T19:05:55.056Z Reads: 77

```
Keep in mind that for this you always need a separate DC power supply also. It’s not working with AC. 
Like @b264 said, the most easy and probably also more cheap way is just to get a regular 12s charger and a bms. The advantage of it is also that you don’t always need to open your enclosure for charging.
```

---
## \#8 Posted by: b264 Posted at: 2018-10-01T19:10:35.116Z Reads: 75

```
[quote="Andy87, post:7, topic:69734"]
The advantage of it is also that you don’t always need to open your enclosure for charging.
[/quote]

Yes, it's cheaper, it's better, you can't accidentally destroy your cells just by charging it the wrong way, and you don't have to take your skateboard apart to charge it and destroy waterproofing.  Of course it's slightly slower to charge... but you'll find that may not matter as much as you think it matters
```

---
## \#9 Posted by: wafflejock Posted at: 2018-10-01T19:12:28.909Z Reads: 71

```
Some other downsides to BMS you are carrying your charge circuitry with you, small additional weight and now it's subject to all the vibration and other things you encounter out on the road.  1 more thing to break attached to a thing that breaks things :slight_smile:

That said there are as stated plus sides as well so up to you to weigh them.
```

---
## \#10 Posted by: b264 Posted at: 2018-10-01T19:15:21.555Z Reads: 71

```
Fact: if you have to take your skateboard apart to charge it, you will end up charging it less and riding it less and enjoying it less.

Don't forget to weigh that one in the mix :stuck_out_tongue:
```

---
## \#11 Posted by: JensSjogren Posted at: 2018-10-01T19:21:33.587Z Reads: 67

```
Good point about the bms guys, so what i need to look for in a bms should be that it is rated for 12s packs and can discharge 80 amps in order for my motors to get the power that they crave?
```

---
## \#12 Posted by: b264 Posted at: 2018-10-01T19:38:38.351Z Reads: 67

```
Yes; if you want to discharge through the BMS.

You don't have to.  You can use the BMS only for charging if you want, just like if you were using a hobby charger for charging, you would have no BMS on the main battery output
```

---
## \#13 Posted by: JensSjogren Posted at: 2018-10-02T04:22:21.357Z Reads: 57

```
Aha, so what's the advantage of using the bms for discharge aswell? I suppose it controls the outcoming current. I'm going to use Torqueboard Vesc. Maybe the vesc also has some kind of current control? 🤔
```

---
## \#14 Posted by: b264 Posted at: 2018-10-02T04:59:51.190Z Reads: 58

```
[quote="JensSjogren, post:13, topic:69734"]
what’s the advantage of using the bms for discharge
[/quote]

"For esk8" I would say "there isn't; it's actually worse" but for most things it's better.  Also some folks may disagree with me.  So don't take that as fact.

If stuff starts going wrong, I would *personally* prefer to destroy the battery trying to save my face, as opposed to destroying my face trying to save the battery.
```

---
## \#15 Posted by: Andy87 Posted at: 2018-10-02T05:58:20.563Z Reads: 53

```
if you discharge throu your bms, your bms keeps your battery from overdischarge (what will do your vesc too if setup right)
the bms will restrict the output current to the max current your bms can handle.
if you buy a 80a bms it will cut off if you exceed that (like a fuse) just that you can switch on the bms after again.
it also will protect your battery from overcharge, which can be an issue if you start to break with fully charged battery, it can happen that your bms will cut off the battery and you can´t break anymore.
the last thing which you will get when discharge throug the bms, 
you can use the e-switch which usually build in the bms. This means less space and money to spend for an antispark or vedder switch.
```

---
