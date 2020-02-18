# Modular battery idea multiple BMS 5x 10s1p

### Replies: 11 Views: 369

## \#1 Posted by: Darkie02 Posted at: 2018-11-12T10:02:02.877Z Reads: 109

```
so I'm almost finished my first Esk8 and all ready thinking of my second and what I want to improve upon. first issue that I'm wanting to improve upon is the cable lay out and the battery.

* i'm thinking along the lines of a chamfered edge to minimise wasted space and leave a aesthetically pleasing case tapered edge (my current one is a rectangle box that just looks ugly)

* odd sized BMS and BMS restrictions (my 80a Alien Power system one just docent fit in neatly around other components (and that are unable to provide a spec sheet for it after weeks of asking its not the standard Best Teck one pictured on there website I thought I would be sent)

* keeping the battery with some flex and making the P groups spear and modular. also means I can add more P over time for range or reduce for weight reduction (my first design uses foam double sided tape to space the P packs to allow it to flex joined with silicon cable to the next S so as the deck flexes the pac isn't under strain.

* Low profile (who wants a big pack sticking out the bottom of the long board)

* even weight distrabution 

after reading throu the forms for weeks I've never seen any one use separate BMS in parallel before am I been stupid and this won't work for some reason iv not thought of yet

my idea pictured below
its a 10S 1P then add more packs in parallel to allow board flex

Green 18650
Black is a 16850 spacer 60p of eBay 
![08|565x500](upload://5R9D1lLIxdkCQPHm8h1zMzYYH2E.jpeg) 
Yello XT 30 will also run cables down hear for other batterpacks 
Red BMS 10s rated to 10S 20A continues 30A Peak Discharge with heat sensor (can't fined the dimensions so iv drawn it oversized)

![31|528x500](upload://kicB7rgBiXUg9MeVPrP44jXYkat.jpeg) 

![47|690x493](upload://vWuOEexh9xpbbwFy1lNpWhVMeQW.jpeg)

im thinking this modular design would have better protection for each 18650
and if you had a bad sell only part of you battery would shut down letting the other packs take over to get back home at full voltage. higher current draw and higher charge curret and more accurate over heating protection of batteries  (no restrictions from BMS/more localised heat sensors) reduced cost.

is there any think iv over looked can you put BMS in parallel like this or is there some big obvious issue I'm missing?
```

---
## \#2 Posted by: brenternet Posted at: 2018-11-12T10:19:13.991Z Reads: 95

```
While I don't know for sure I'd assume hoyt are doing this in their swappable/extendable batteries?

![SmartSelect_20181112-101808_Chrome|335x500](upload://49RynS7Viy863q4d3YDGwNNlhto.jpeg)
```

---
## \#3 Posted by: anders Posted at: 2018-11-12T10:44:32.846Z Reads: 87

```
Hi there,
I have run two 10s2p batteries with individual bms for each pack in parallel for 1000km's in the last 9 months.

These are cheap samsung 22p cell packs and the pack each has a individual bms, I split the charge port in two and charge them together.

I made sure that the voltage was the same in each pack when I hooked them together in parallel and have monitored the voltage in each pack after separating them after charging.

Positives are more range and less voltage sag, only negative is more weight.

Good luck
Anders
```

---
## \#4 Posted by: Darkie02 Posted at: 2018-11-12T10:54:20.158Z Reads: 80

```
in theory you shouldn't even need to balance the packs or cells the BMS will take care of that as long as the charger can trickle charge when the current drops from some cells been full.

thanks for the real world knolage/experience of it working. puts my mined at rest that I'm not doing some thing crazy.

I could end up with a cascade effect of BMS cutting out when max current is exceeded but I presuming thats no different from 1 BMS cutting out.
```

---
## \#5 Posted by: baxter Posted at: 2018-11-12T11:23:33.934Z Reads: 75

```
FYI.  Pretty sure each pack has 25R cells, and is 90wh (flightsafe). 

https://eflowboards.com/collections/parts-accessories/products/battery-x2
```

---
## \#6 Posted by: J0ker3366 Posted at: 2018-11-12T11:26:38.647Z Reads: 71

```
What kind of range do you get out of those? About to no weld a 10s6 with those cells.
```

---
## \#7 Posted by: anders Posted at: 2018-11-12T11:32:15.208Z Reads: 67

```
22km with good speed then usable up to 30km but slow, with single pack 7km with good speed  then lots of sag.
```

---
## \#8 Posted by: venom121212 Posted at: 2018-11-12T12:41:44.793Z Reads: 66

```
The only issue that has been laid out to me when I asked this question was what if one bms fails. Your charger will continue to float/trickle charge both of them when the good pack starts dropping and you'll get one pack trying to charge the other. I know a few people who have done it with no issues but I'm honestly too scared to try it because I love my legs and house and board.
```

---
## \#9 Posted by: Darkie02 Posted at: 2018-11-12T13:13:37.741Z Reads: 62

```
if 1 pack tryed to charge the other (if the voltage difference was high enough) wouldn't the bms kick in at min voltage and cut the pack out stoping any damage?

do you have a link to your post would like to read through it
```

---
## \#10 Posted by: venom121212 Posted at: 2018-11-12T13:37:37.055Z Reads: 57

```
The real issue is overcharging the one that had a failed bms. An empty battery won't catch fire, an overcharged one will.

[https://endless-sphere.com/forums/viewtopic.php?t=45720](https://endless-sphere.com/forums/viewtopic.php?t=45720)

Really I guess it comes down to how much you  know about the specific BMS. I'd exercise caution with an unknown.

Shameless plug for @hyperIon1 and @hyperIon2 here : talk to them about getting them rebuilt into one pack with a new BMS. Very knowledgeable guys state side.
```

---
## \#11 Posted by: Darkie02 Posted at: 2018-11-13T17:44:40.214Z Reads: 33

```
So if I understand right the issue is a bms possibly failing and overcharging?

I can see your point of more parts to fail but there’s a lot of people using cheep bms as charge only.

Reading thro that post I see a diode recommended to stop any possible current flowing the rong way if you battery’s have difrent voltages. But my understanding is If discharging together then the higher voltage pack will drag down the lower one as soon as the potenchal difrence appears. just as you get in cells in parallel

Still not found any reason to why it’s bad to have BMS in parallel on separate cells. Starting to believe this could be a urban mith. Surly a regen under braking of 50A that is ofteren used is way worse on a 4p most 18650 rated to 1.5a charge so a 4p is 6a charge current. over 8 times the recommendation. The highest I’ve seen max charge on cells at 4.5a even then we talking over double the max. Is this not way more dangerous for fires?
```

---
