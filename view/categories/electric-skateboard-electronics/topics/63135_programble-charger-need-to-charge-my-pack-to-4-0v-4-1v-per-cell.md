# Programble charger? need to charge my pack to 4.0v-4.1v per cell

### Replies: 16 Views: 395

## \#1 Posted by: Leav Posted at: 2018-07-28T07:22:22.872Z Reads: 113

```
Hi,

So I start off my commute with a pretty long downhill portion (~500m?), and after first testing out my build yesterday, The option I was afraid of happened: braking was disabled after ~50m (over voltage protection kicked in).

I knew this was an option but was hoping maybe the charger would leave enough space in the batteries for the energy from the hill.

Right now I think the simplest option is charging to ~4.0v-4.1v per cell (I have a 6s5p pack), and maybe topping off at work if I need it.

Is there a charger I can program to select a voltage? I have a imax b6 (clone and original on loan from a friend), but they seem to only allow you to go down to 4.18v?

Any other chargers you can recommend?
Any other options?
```

---
## \#2 Posted by: Winfly Posted at: 2018-07-28T07:31:36.805Z Reads: 104

```
can get a watt meter for your outlet to limit how much goes into your battery.
```

---
## \#3 Posted by: cryo Posted at: 2018-07-28T07:33:35.975Z Reads: 103

```
I've seen people with diy chargers like this https://www.aliexpress.com/item/DPS5015-15A-Constant-Voltage-current-Step-down-Programmable-digital-Power-Supply-buck-Voltage-converter-color-LCD/32797129142.html?spm=2114.search0104.3.15.464b6c1fSXjbhk&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10151_10065_10344_10130_10068_10324_10547_10342_10325_10546_10343_10340_10548_10341_10545_10696_10084_10083_10618_10307_10869_10868_10059_100031_10103_10624_10623_10622_10621_10620,searchweb201603_6,ppcSwitch_4&algo_expid=63d92204-06d0-4619-b0ac-21f33dde1c9c-2&algo_pvid=63d92204-06d0-4619-b0ac-21f33dde1c9c&priceBeautifyAB=0

find one that matches your batteries specs and maybe that could work? Alternatively I have the same problem and I usually just go up 1 hill and that shaves off enough voltage to brake the rest of the way since regen is 20% efficiency at most..
```

---
## \#4 Posted by: Leav Posted at: 2018-07-28T08:29:51.840Z Reads: 92

```
So If I find a 24v CCCV power supply that's adjustable to 24.6 I could use that as a Li-Ion charger? are there no special functions that make a Li-ion charger "smarter" than a CCCV power supply?
```

---
## \#5 Posted by: cryo Posted at: 2018-07-28T09:26:36.375Z Reads: 87

```
sure I've brought undervolted lipos back with cccv chargers, a power supplys a power supply. I'm not sure what you mean by Li-ion charger but those benchtop cccv chargers are as smart as it gets although not very portable
```

---
## \#6 Posted by: Leav Posted at: 2018-07-28T11:00:41.570Z Reads: 76

```
Found [this MeanWell CLG-60-24](https://www.aliexpress.com/item/MEANWELL-24V-60W-UL-Certificated-CLG-series-IP67-Waterproof-Power-Supply-90-295VAC-to-24V-DC/32246773073.html?spm=2114.search0104.3.19.33885e24ix3FZx&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10065_10151_10344_10068_10869_10342_10868_10343_10340_10059_10341_10696_100031_10084_10083_10103_10618_10624_10307_10623_10622_10621_10620,searchweb201603_12,ppcSwitch_5&algo_expid=7f27d0c2-ec32-4539-bc90-93437be5e1c8-3&algo_pvid=7f27d0c2-ec32-4539-bc90-93437be5e1c8&priceBeautifyAB=0), but i'm bummed out about spending ~$80 for a charger :-\

Any other suggestions would be highly appreciated.
```

---
## \#7 Posted by: PXSS Posted at: 2018-07-28T11:23:50.889Z Reads: 67

```
Get any rc charger that is decent. Isdt chargers are great for the money
```

---
## \#8 Posted by: Leav Posted at: 2018-07-28T12:29:24.880Z Reads: 67

```
Thanks for the suggestion, never heard of them.

Looking a bit online, couldn't find definitive proof you could change the end-of-charge voltage (looked at their manuals and some videos online) are you sure you can change that?

For example, on the imax you can only dial it down to 4.18....

Edit: looks like the [isdt chargers only go down to 4.15v](https://youtu.be/xclAF6KxQUI?t=360)
```

---
## \#9 Posted by: MonkeyM Posted at: 2018-07-28T15:54:53.396Z Reads: 59

```
I'm charging 6S lipo with a cc cv step up (boost) voltage converter which is powered from a 19v laptop power supply.

I've not had any problems. I don't believe there is any special charging intelligence in the chargers you mention other than the balancing, which can be done by your bms, and some other features (discharging for example) 

With cv cc converter set the voltage to the max you want to reach (24v?), plug it into the bms. The voltage will drop to that of your battery pack and the amps will shoot up to your max (ensure your supply can supply enough power [power = volts x amps] and your batteries can be charged at that rate otherwise turn the current down). As the batteries approach the max voltage you dialed into the converter the amps will reduce progressively until 0amps.

I think they should be called "adjustable max voltage, adjustable max amperage" instead of cc cv, but maybe that doesn't roll off the tongue quite so well! 

I got the boost converter from ebay or aliexpress. Give me a shout if you want more details.

(I used a non cc version first time round, it kept pulling too much power from the laptop charger causing it to cut out through protection mode. Don't make the same mistake!)
```

---
## \#10 Posted by: PXSS Posted at: 2018-07-28T18:18:17.656Z Reads: 52

```
Check out iChargers. They're abit more money but they can definitely adjust lower than 4.1v. My hitec x2 ac also goes lower than 4.1v. 

Look up in rcgroups for good deals in their classified section. 

I'm not home right now but I'll let you know which chargers can do what. 

Skyrc. Hitec. iChargers. Powerlabs. All good chargers to look into for RC stuff.

E. Check this out

https://www.progressiverc.com/skyrc-s60.html

![image|690x180](upload://pgIjzseYV5PQBQSaddjxaqDGEpl.jpeg)

So you can go down to 4.08v. Lipo and liion are essentially the same
```

---
## \#11 Posted by: deucesdown Posted at: 2018-07-28T19:12:40.523Z Reads: 49

```
https://www.amazon.com/Tekpower-TP3005N-Regulated-Variable-Supply/dp/B078MY5RGQ/

Many uses for such a thing. The 60v versions are more useful if you go above 6s.

Might want a outlet timer to go with it, as you won't have end of charge termination.

And what @PXSS says. Note, my powerlab won't charge 6s without balance leads connected.

Oh and most of the nicer hobby chargers need a separate source of DC power. The ones that don't are usually limited to 50w
```

---
## \#12 Posted by: PXSS Posted at: 2018-07-28T19:44:34.606Z Reads: 47

```
The skyrc that i linked has ac in and also allows unbalanced charging. Most chargers do. I'm surprised your powerlab doesn't support it.
```

---
## \#13 Posted by: Jake2k17 Posted at: 2018-07-28T22:41:08.136Z Reads: 45

```
why don't you just watch your batteries voltage and when it gets to 4v just unplug it?
```

---
## \#14 Posted by: pat.speed Posted at: 2018-07-28T22:54:46.519Z Reads: 46

```
I’m doing the same as @MonkeyM I bought a cc/cv charger on eBay and a 60v watt meter to connect inline with it. I can now charge all my packs to any voltage I would like. 

One problem that will occur though is the lack of balancing, if you don’t use a bms they will become unbalanced and even with the bms they only balance the cells at 4.18v at the lowest. So I’m not sure what you will do there, maybe just fully charge the board every second or third ride, or fully charge at work to rebalance the cells
```

---
## \#15 Posted by: Okami Posted at: 2018-07-29T07:31:57.214Z Reads: 42

```
Concerning 'hobby' / rc chargers, i can confirm Turnigy reaktor can be set to any voltage u like.

A cheaper version is Charlsoon (o or similar name) which can be found on banggood for 40-50usd (at least a while ago)

---

Didnt know isdt alllows only down to 4.15, thats a shame but u can always charge in li-ion mode, i think, turnigy chargers usually charge to 4.1v in this case (or i think they did)
```

---
## \#16 Posted by: Acido Posted at: 2018-07-29T20:34:40.040Z Reads: 28

```
Did you check out those chargers that are used for vaping I guess?
They sell on nkon
```

---
