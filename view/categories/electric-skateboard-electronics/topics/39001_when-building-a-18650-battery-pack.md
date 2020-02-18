# When building a 18650 battery pack&hellip;?

### Replies: 46 Views: 3224

## \#1 Posted by: Wolphe Posted at: 2017-11-22T14:23:00.039Z Reads: 260

```
Hi, all
I'm currently using four 6s 6200mah lipos with 2 series connectors to make two 12s batteries running twin motors. 

I recently saw that 18650's are more efficient and safer to handle than lipos.

So if I set six 18650 6000mah Li-ion batteries in series, that would make them a 6s? With 6000mah?

I will be setting it up with a balance connector instead of a bms.
```

---
## \#2 Posted by: gee Posted at: 2017-11-22T14:53:46.818Z Reads: 252

```
18650 with 60000 mah? Like two 18650 in parallel? or ONE 18650 with 6000 mah because that's unheard of.
```

---
## \#3 Posted by: Wolphe Posted at: 2017-11-22T15:01:18.946Z Reads: 245

```
I've seen it on Alibaba, but is the 3000mah easier to get?

If I get the 3000mah batteries, I would need to have 12 of them to make a 6s 6000mah?
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2017-11-22T15:03:23.906Z Reads: 235

```
6000mah is non existant. Chemistries simply aren't there yet. Samsung 30Q cells are one of the best on the market right now and are 3000mAh which is a good capacity for a 18650
```

---
## \#5 Posted by: Wolphe Posted at: 2017-11-22T15:04:02.699Z Reads: 224

```
So this isn't real?

https://m.alibaba.com/product/60339405074/18650-li-ion-battery-3-7v.html?s=p&spm=a2706.7843299.1998817009.4.sGffRM
```

---
## \#6 Posted by: BoostedBuilder Posted at: 2017-11-22T15:04:36.681Z Reads: 211

```
nope. where are you located?
```

---
## \#7 Posted by: gee Posted at: 2017-11-22T15:05:29.443Z Reads: 214

```
Parallel : add mAh.
Series : add voltage
so you want 12s, 12 in series, 2p, 2 parallel. Let's say 18650 is 3000 mah. You want 12 of those in series to make it 12s but it only has 3000 mah. So you need another 12s in PARALLEL to make it 3000 mah + 3000 mah = 6000.

So to your question, yes you would need 12 of them to make it 6s with 6000 mah.
```

---
## \#8 Posted by: Acido Posted at: 2017-11-22T15:06:09.624Z Reads: 208

```
you mean 24 for 12s2p
```

---
## \#9 Posted by: Wolphe Posted at: 2017-11-22T15:08:58.189Z Reads: 211

```
Thanks boostedbuilder. Km located in Florida (U.S.)

Gee: thanks! 

Where is a good source in buying good 18650's at a good price?
```

---
## \#10 Posted by: BoostedBuilder Posted at: 2017-11-22T15:10:44.599Z Reads: 210

```
https://liionwholesale.com
https://batterybro.com/collections/18650-battery
These are US vendors.

https://eu.nkon.nl
This one is in the eu but they ship to the US
```

---
## \#11 Posted by: darkkevind Posted at: 2017-11-22T15:14:00.535Z Reads: 194

```
The highest mah of any 18650 at the moment is 3500. Those ones you linked to are fake.

You should use either of the following cells in at least 2 parallel;
Samsung 30q 3000mah 15A cont. discharge (6000mah 30A)
LG HG2 3000mah 20A cont. discharge (6000mah 40A)
Sony Konion VT6 3120mah 30A cont. discharge (6240mah 60A)

You should get your cells from a reputable source, I suggest nkon.nl
```

---
## \#12 Posted by: Wolphe Posted at: 2017-11-22T16:24:07.439Z Reads: 183

```
So $7 is the average price for one 18650 3000mah battery?
```

---
## \#13 Posted by: FredrikHems Posted at: 2017-11-22T16:30:27.604Z Reads: 182

```
Something around there, unless you buy in very high quantities
```

---
## \#14 Posted by: Wolphe Posted at: 2017-11-22T16:40:42.610Z Reads: 173

```
Last question for the day, lol. Will 20a do the job, or should I go higher?
```

---
## \#15 Posted by: MysticalDork Posted at: 2017-11-22T16:52:46.829Z Reads: 168

```
It depends on the battery. If you get 30q cells, they're about $4.00 a piece in quantity. You definitely need more than 2p with them, I wouldn't go below 3p, and 4p would be even better. If you go with the absolute top of the line vtc6 cells, yes they're a lot more expensive. You still need at least 2p to get a decent amount of current and range.

Also keep in mind that you're running 4 6s packs, each 6000mah. To have a similar range with 18650s, you'll need 12000mah and 12s, which is 12s4p.
```

---
## \#16 Posted by: Wolphe Posted at: 2017-11-22T17:18:05.087Z Reads: 156

```
That makes sense. It seems like even though 18650's are safer and more efficient than lipos, I will be sacrificing weight and space management for the same amount of power I'm getting for lipos.
```

---
## \#17 Posted by: NickTheDude Posted at: 2017-11-22T17:21:07.771Z Reads: 157

```
[quote="darkkevind, post:11, topic:39001"]
Sony Konion VT6 3120mah 30A cont. discharge
[/quote]

3120mAh with 30A discharge?! Where can I find these things? The only VT6s I've seen are 3000mAh and 15A discharge.
```

---
## \#18 Posted by: wafflejock Posted at: 2017-11-22T17:45:35.575Z Reads: 159

```
Far as I know the chemistry is very similar the package is just different with some safety benefit on the side of 18650s in terms of controlled failure (place on the cell designed to blow out, that said I've seen plenty of 18650 boards on fire to let me know it's not entirely safe).  I see this much how I see virus protection on computers, it gives people a false sense of security and safety, these things are dangerous no matter what kind of shell you put the chemicals in.

---

### 18650 Volume
(18/2)^2*65 * 3.14 = 16,532 mm^3 = 16.5cm^3

### 18650 Power Density (power per cm^3)
(3.7V*3Ah) / 16.5 mm^3 = 0.67 Wh/cm^3

---

Compare with Lipo 5S pack

### LiPo Volume
145*50*41 = 300,000 mm^3 = 300cm^3

### Lipo Power
5S*3.7V*5Ah = 92.5Wh

### LiPo Density
92.5Wh/300 = 0.30Wh/cm^3

---

So in terms of energy density for volume you're actually better off with 18650s, one thing to keep in mind here though is the packing space lost when stacking cells next to each other, if we assumed the 18650 is a rectangular cube instead it is:
18*18*65 = 21,060 mm^3 or 21 cm^3 which brings the energy density down to .52Wh/cm^3 but still slightly better than a regular 30C LiPo pack.

Personally I use LiPo packs because they are cheaper and I have the equipment (a soldering iron) to remake the connections to wire them together without potentially damaging cells.  Also started off with quadcopters before I got into the esk8 hobby so had the charger and knowledge/experience with the batteries.
```

---
## \#19 Posted by: darkkevind Posted at: 2017-11-22T18:18:29.599Z Reads: 143

```
https://eu.nkon.nl/rechargeable/18650-size/sony-us18650vtc6.html
```

---
## \#20 Posted by: Wolphe Posted at: 2017-11-22T18:37:09.980Z Reads: 144

```
 I've been in Drone Racing for 4 years. I'm use to lipos as well and all the tools to build one.

Just thought I'd look into 18650's as they are another option.
```

---
## \#21 Posted by: wafflejock Posted at: 2017-11-22T18:39:57.652Z Reads: 141

```
Nice I'm sure you would wreck me on the drones I just tinker around with mine at the park nothing too serious, been flying on and off over a couple of years but not really regularly ever and still getting used to FPV.  You can go either way with it, if you have the cash and want the slimmer profile and want to wire up a BMS and switch then would go 18650.  If you want to go more minimal (I have a web/software engineering background so in my mind less things = less things breaking) then LiPos, a loop-key, and a decent charger and you're all set.

---

Some quad abuse :slight_smile:
https://www.youtube.com/watch?v=2jHwfi7Tfng&t=192s
```

---
## \#22 Posted by: psychotiller Posted at: 2017-11-22T18:58:59.154Z Reads: 139

```
Nope! But this is:
<img src="/uploads/db1493/original/3X/9/0/90ac39803984e269ae76354d436d3341ab5f23fd.png" width="225" height="225">
```

---
## \#23 Posted by: Wolphe Posted at: 2017-11-22T19:31:56.031Z Reads: 134

```
So far I have the minimum setup, but gonna add a battery meter and a Lipo buzzer. Maybe a switch. It's an easy setup and it's all gonna be in a hard box sitting on top of my trampa mtb.

I like tinkering and building electronics.

As far as drone racing, I'm still a noob pilot. I mostly host drone racing events through MultiGP.
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-11-22T19:35:58.850Z Reads: 134

```
your mom's a random unicorn fart.
```

---
## \#25 Posted by: michaelcpg Posted at: 2017-11-22T21:27:28.752Z Reads: 124

```
https://ru.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html

Pretty sure you're better off buying from Nkon's non eu site if you're outside the EU. That's where I got my last lot of cells from. The 30Q's work out to be about $3.30USD per cell plus shipping
```

---
## \#26 Posted by: michaelcpg Posted at: 2017-11-22T21:53:20.669Z Reads: 123

```
As some others have mentioned, you probably want a minimum of 3P with 18650s although 4P would be preferable, particularly if you live in a hilly area
```

---
## \#27 Posted by: Wolphe Posted at: 2017-11-22T22:14:55.093Z Reads: 131

```
Thanks Michaelcpg! 

Though I know lipos pretty well, this will be my first time handling any battery in "parallel/series"

So 4p would be 4 series running in parallel?  
(12s4p would be twelve 18650's in seriesx4 in parallel?)
Ex. One"18650 3000mah" x 12 into a series x 4 in parallel?

I'm just writing that down as a visual.
```

---
## \#28 Posted by: Wolphe Posted at: 2017-11-22T22:18:13.227Z Reads: 127

```
Also, that link describes that battery amp rating at 15a. Is that enough or too low of an amperage?
```

---
## \#29 Posted by: wafflejock Posted at: 2017-11-22T22:21:17.944Z Reads: 127

```
Believe most people actually do it as packs of cells in parallel with each other because easier to spot weld (or solder) the tabs across a set of positives with a block of cells and negatives on the other side and they are effectively in parallel, then wire those blocks of cells that are in parallel, in series to get the 12S.  Regarding amperage you multiply the amps supplied by number in parallel (15A flow from each set of cells in parallel, each one of the cells in parallel is feeding into the positive and negative it isn't flowing through all the cells as is the case when connecting in series).

http://www.electric-skateboard.builders/t/battery-wiring-diagram-help/39011/4

When you hook up cells in parallel they are effectively going to charge/discharge each other until they are level so be sure the cells are close to the same charge before connecting them, once connected they will self balance but if too much charge is quickly dumped into a cell it will overheat it.

---

Regarding 15A per cell if you have 4 in parallel you have 60A max discharge without causing a problem, and at around 45-50V you could be drawing 3000W which I think is pretty unlikely (unless you're racing up a hill perhaps and have huge motors).  That said in the case of max discharge and current in general leaving some buffer is always a good thing.

---

If you don't plan on buying or making a spot welder though your options are limited on how to get this done safely.  There are these packs http://vruzend.com/ believe they've posted on some threads here too but would have to search around and find those to see how that turned out.

Lots of places to get them premade as well, miami electric, diy, believe psychotiller, and longhairdboy may do them too.
```

---
## \#30 Posted by: MysticalDork Posted at: 2017-11-22T22:53:41.185Z Reads: 110

```
When thinking about batteries in series and parallel, like your earlier "4p" example, if there isn't a separate "S" number with it, you can assume it's 1s, or one cell in series. So a "4p" pack would be four cells, connected so that all their positive terminals are together, and all their negative terminals are together. 

If you run across "12S" with no parallel number with it, you can assume it's 1p, or 12 cells end to end, the positive of the first going to the negative of the next, and so on.

"12s4p" means you take 4 batteries and put them in parallel, then take 12 sets like that and put them all in series.

Batteries in series add voltage, but not capacity. So a 12s1p pack of 3000mah cells will still be 3000mah.

Batteries in parallel add capacity, but not voltage. So a 1s4p pack will have the same voltage as a single cell, but 4 times the capacity (and 4 times the current too).

Add them together, and you have 12 times the voltage and 4 times the capacity.
```

---
## \#31 Posted by: michaelcpg Posted at: 2017-11-22T23:39:55.160Z Reads: 107

```
Yup you got it so if you made a 12S4P pack out of those Samsung 30Q cells which are 3.6V and 3Ah, you'd end up with an overall battery pack rating of 43.2V and 12Ah which works out to 518Wh. 

And because the pack is 4P, you'd have a total discharge rating of 4*15A = 60A, which as long as you're not building a mountainboard etc, is fine.

Keep in mind thought that just because each cell might be rated at 15A discharge, ideally you don't want to be pushing that much current very often if you want to get the most out of them as they'll generate less heat and be less stressed. 

In general, the less current you're regularly drawing from your battery, the longer the cells are gonna last and the more charge cycles you'll get out them, so if you're on a budget, keep in mind that if you spend a bit extra now, they'll last you longer.

Also, when comparing cells, don't just go by their manufacturer rating as these values aren't particularly reliable. Try and find discharge curve charts that people having created from testing, such as this one:

<img src="/uploads/db1493/original/3X/a/2/a292c73b544bcef74595ed12c7910b7363301c43.jpeg" width="690" height="341">

As you can see, you could draw 20-25A from these cells if you really wanted but they're going to get a lot hotter and not last anywhere near as long.
```

---
## \#32 Posted by: Wolphe Posted at: 2017-11-23T02:11:21.304Z Reads: 104

```
Wow. This is a wealth of information! I really thank you all for taking the time to share and educate me on this.

I would rather purchase a spot welder than to solder, even though I am very good at soldering, it just seem a bit too risky to solder these kinds of batteries.

Michaelcpg: I'm curious as to why you said this:
"And because the pack is 4P, you'd have a total discharge rating of 4*15A = 60A, which as long as you're not building a mountainboard etc, is fine"

Is that too much power? I have a trampa mtb running 2 low kv motors for good torque. Would 60a be too much draw of power? I'm in Florida going over fields and pavement. Flat lands.

WaffleJock: I'm using these lipos:
https://hobbyking.com/en_us/zippy-compact-6200mah-6s-40c-lipo-pack-xt90-1.html
On 60xx 118kv motors. Reason I chose low kv is because I'm a big guy. 6'2" and about 230lbs built with a Lil belly, lol. So I need some torque to carry this big body.
```

---
## \#33 Posted by: wafflejock Posted at: 2017-11-23T02:28:23.492Z Reads: 109

```
Hah all good.  Think you're mixed up in a common way though.  The max discharge isn't how much will go through the circuit you apply the voltage to it's the maximum you should ever draw (really you should never draw that much ideally).  How much gets drawn is dependent on how much on time (duty cycle) the speed controller is opening the gates to let power flow to the coils of the motor.  Basically the ESC ramps up the power it lets flow through the coils until there is enough current (amperage) flowing in the coils to turn the motor then when it detects the motor is turning it fires the next set of gates (MOSFETs) to let the current flow through the next set of coils.  It's a little more complicated than this but that's a general picture.

So the amps we're talking about with the battery supply you want to be much higher than what the system will ever actually use.  It's not as though the battery is "pushing x amps" the battery is just charged with y voltage potential and the circuit has z resistance in ohms then the x amps you need the battery to supply (calculated as y voltage over z ohms y/z = x, or more commonly V/R = I)  should be under the "max amps" the cells can safely supply.  So increasing the number in parallel increases the buckets you have to draw the total current from and you want the current from any given bucket to be below the max rating for that bucket.

Think this visual series is helpful in getting a picture in your head of how things work if you don't have a lot of background in electrical circuits or batteries:

https://www.youtube.com/watch?v=u4FpbaMW5sk&t=2s

The batteries all have "internal resistance" just resistance like any other component but in the battery itself so if that is too high the battery cooks itself inside out.  Max amperage ratings are in a round about way telling you the internal resistance of the cells and the heat dissipation capability of the cells.

---

The discharge current (amperage) through a circuit is always equal to the voltage divided by the resistance so say you hook your battery up to a high resistance load (say a bunch of light bulbs) if their resistance is high enough the current will stay low but if they have very low resistance then the current is high.  In our case the load is more complicated since we have chips that open and close gates/switches at a high speed the current flow to be regulated but the same basic rules apply.

https://socratic.org/questions/how-does-voltage-affect-a-magnetic-field

https://www.khanacademy.org/science/physics/circuits-topic/circuits-resistance/v/electric-power
```

---
## \#34 Posted by: wafflejock Posted at: 2017-11-23T05:25:31.601Z Reads: 96

```
I'm the opposite body type wise (and Chicagoland area so flat ground mostly), but here's some actual data recorded from my bluetooth module using the metr.at app for logging data

https://metr.at/r/rKZvg

I run 10S 5Ah or 185Wh (2x5S 5Ah) battery and  149kv 6374 Turnigy SK3 motor

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":149,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":90}|

The chart @michaelcpg linked is showing that if you have higher discharge rated (lower internal resistance) cells then you get more mAh out of them if you draw the power at a lower current, basically less you are stressing the cell with heat the more power you actually get out of them and the less you'll damage them in the long run.  The long story short is more in parallel can't really be bad aside from weight/volume issues more in series and you can end up with voltage potential that is higher than the components you're using are rated to handle

Amperage causes loss as heat (I^2*R = power loss, so delivering power [Watts=Amps*Volts] at as high a voltage your components can support and doesn't kill you is ideal).
```

---
## \#35 Posted by: Wolphe Posted at: 2017-11-23T17:02:03.468Z Reads: 83

```
That almost got a little confusing on the last 2 post, not gonna lie, lol. But I get the gist of it. 

Best way I can compare it as a Drone Racing guy, is pretty much the same. Not one number is good. There are variables that need to be considered.

Foe example; a 
500g racing drone, 
with 2207 2600kv motors 
with 30a esc for each motor 
on 5 inch 50 pitch propellers 
= a  power house, powered by a 4s 1300mah 100c. 
Too much power for a light drone. The 30a esc's are basically overkill. I would be fine with a 20a with my skill level, but with a pro, 30a isn't enough, they would need a 35a otherwise risk of burning out the esc's.

If I change it up with a 4s 1500mah 90c instead of 1400mah 100c

And 

5 inch 40 pitch propellers 
I would lessened the aggressiveness of the power by adding weight from the Lipo and toning down on the propeller pitch. Much easier to tame for me. 

The heavier the drone, the more mAh I need, less c rating, bigger propellers and lower kv motors to keep it efficient. Maybe get a higher esc amps,  like a 40.

This is more my language, but it is the same concept. Everything is accounted for based on weight. Does that make any sense? Lol. I'm rambling now....
```

---
## \#36 Posted by: GrecoMan Posted at: 2017-11-23T17:24:04.198Z Reads: 80

```
not sure I understood that but I think it might be wrong :joy:

Max discharge is the amperage a battery CAN discharge continuosly, the vesc (or esc) will determine how many amps it needs to draw from the batteries. At most times on street boards that is only about 40a on hard accelerations, once you get up to speed and start cruising the motor will need less amps since the load on the motor is decreased because it is already spinning (normally 1-2a). For mountainboard I recommend you get batteries with a bit more discharge rating (not sure if you posted your weight but that plays a big role too). Mountainboards require more amps to turn the motor becuase the pulleys on the wheels are much bigger and the wheels are also much bigger, which leads to bigger rolling resistance. Hope this helped :)
```

---
## \#37 Posted by: Acido Posted at: 2017-11-23T17:28:33.249Z Reads: 76

```
where are you buying your getting ripped off lol
```

---
## \#38 Posted by: FredrikHems Posted at: 2017-11-23T18:03:49.669Z Reads: 77

```
I am not using li-ion packs. IMO I think lipos are better unless you go with a large pack like 6p or higher. Also, I live in Europe so shipping and stuff is hella expensive
```

---
## \#39 Posted by: Wolphe Posted at: 2017-11-23T18:33:09.546Z Reads: 77

```
Acido, where do you get yours?
```

---
## \#40 Posted by: Acido Posted at: 2017-11-23T18:49:24.983Z Reads: 79

```
Samsung 30q 143euro 40pieces shipped to Croatia, that was 2 months ago or so now they are a bit more expensive but still a good price, check out the prices for hg2

EDIT: Nkon.nl
```

---
## \#41 Posted by: Acido Posted at: 2017-11-23T18:49:54.615Z Reads: 74

```
someone said 7$ per cell so I assumed 18650 li ion batteries
```

---
## \#42 Posted by: GrecoMan Posted at: 2017-11-23T18:50:18.328Z Reads: 73

```
you didn’t say where you got them from...
```

---
## \#43 Posted by: Acido Posted at: 2017-11-23T18:51:46.804Z Reads: 76

```
whoops was thinking about how can i control lights for my skate with vesc and ackmaniacs app and an hm10 module
sorry

anyways its nkon
```

---
## \#44 Posted by: wafflejock Posted at: 2017-11-23T18:52:48.235Z Reads: 82

```
Yeah I was compiling code so was in highly academic mode :)  Really if you grok Ohm's law though and get that voltage is the electrical potential/electromotive force that gives rise to a current based on the resistance in the circuit that's all that matters.  So amperage isn't anything but that flow and isn't something you really "apply" rather something that falls out of the resistance and the voltage being used.  Also extra bits basically saying power loss in components is related by the square of the amperage so 5amps adds a 25x factor (5^2) in that equation whereas 10amps adds a 100x factor (10^2) in the power loss equation so you ideally want to deliver power at higher voltage.  The final part was trying to give some links that explain how the voltage that gets to the coils ultimately drives the amperage in them and the strength of that amperage also relates to the strength of the magnetic field.

Anyhow just figured I'd drop some of my favorite academic sources here, glad you got something out of it.

Good thing is with the background in quadcopters we're using almost the same exact setup with regard to controlling the flow of power to the motors and controlling the rate of firing of the coils to keep the motor spinning or get it spinning faster/slower.

To get away from the academic stuff and physics fundamentals ultimately more strength in the magnetic field means it will have more force to drive the motor/wheel around and push you forward.

To try and relate to your example in esk8 terms:
90kg rider+10kg skateboard
6374 149kv (190kv seems a sweet spot really for most riders/applications)
50A continuous 240A burst VESC 4.x or above is a good option for controlling the motor and delivering power from battery
83-90mm wheels with a 16T:36T pulley ratio is typical
= a board that will go somewhere in the 20mph-30mph range and gets about 1km for every 10Wh of battery (higher voltage higher efficiency)

You can limit the actual amperage used in the VESC configuration.  Last night I compiled the new VESC tool on my computer (didn't want to sign up to download the prebuilt and like to build stuff myself) and got the new metr.at app where I can select "modes" to limit amperage to 10A or 30A or 60A depending on rider ability or if I'm just cruising vs testing top speed/acceleration.  Without modes I was just on 60A all the time which was sketchy especially if letting someone else try my board, I never actually would draw 60A most I've seen was around 20A at 40ish Volts but I'm also only about 55kg (120lbs)

http://calc.esk8.it

http://calc.esk8.today/

search for esk8 calculator quite a few out there to help you try and calculate actual values for different rider size, grade, gear ratio, wheel size, motor, battery, but lots of variables just like quads so it's hard to just give a direct answer without a very clearly defined set of parameters (even then calculation never completely matches reality).
```

---
## \#45 Posted by: Wolphe Posted at: 2017-11-23T20:02:08.843Z Reads: 76

```
The calculator seems more geared to street wheels averaging around 80mm sized wheels. I'm not getting a good reading with 8 inch wheels, plus not to mention my weight plays a big roll. Like you said, calculated number vs real life number don't ever really matchup. 

As soon as my board comes in this week, I will be documenting and testing different scenarios.
```

---
## \#46 Posted by: wafflejock Posted at: 2017-11-23T20:05:36.136Z Reads: 74

```
Yup best we can do is guess and check and post more data about real world conditions.  It's both the plus and the minus to doing things yourself and working with relatively new components.
```

---
