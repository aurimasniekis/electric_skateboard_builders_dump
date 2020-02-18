# 12s battery charger?

### Replies: 20 Views: 7339

## \#1 Posted by: Sharkface Posted at: 2015-12-09T23:11:10.241Z Reads: 530

```
Whaddup yaaaallllll

Alrighty so I am taking a look at getting a space cell, and it brought something up that I hadn't fully considered. Assuming that I got the space cell it would only make sense to pick up the charger as well. However I already have a very large power supply and a quatro charger that tops out at 6s. Are there any chargers that take in DC input and throw out up to 12s levels of voltage for charging? 

Assuming i made my own 18650/26650 battery pack that ran at 12s.... how would I properly ensure that I can charge my custom pack? I would need charge leads that could throw out that 12s.... hmmmmmm
```

---
## \#2 Posted by: chaka Posted at: 2015-12-09T23:37:47.033Z Reads: 524

```
We use custom made chargers  on all of our packs. You can have them made to charge almost any voltage.
```

---
## \#3 Posted by: cmatson Posted at: 2015-12-10T00:30:21.587Z Reads: 523

```
When you refer to "pick up the charger aswell" what charger exactly are you referring to? The space cell comes with one, and I think you are talking about that, but it seems like you're assuming it's an extra item sold seperately-

That said, all you need is to wire your cells to a BMS, and then it can take DC input. The hard part is finding a BMS for the amount of cells, desired amp rating, etc. <img src="/uploads/db1493/original/2X/f/f3d346164730c5b6df5996e7b474bbaea4979533.jpg" width="690" height="388"> this is a space cell BMS for example (I tore mine apart.. don't recommend it)
```

---
## \#4 Posted by: Sharkface Posted at: 2015-12-10T05:19:22.264Z Reads: 504

```
[quote="cmatson, post:3, topic:695"]
this is a space cell BMS for example (I tore mine apart.. don't recommend it)
[/quote]

Are you sure its not a good idea to take it all apart?!?!? (he asks drunkenly)

And yeah I am totally on board on how the BMS works. However I wasn't entirely sure about the whole charger on top of the space cell as the space cell charger was listed as an add on item... I suppose @onloop could throw in his two cents here on that... but hes also super  duper busy delivering a lot of VESCs.

I was more concerned about getting that 48v 10amp(?) going into the charge/main leads of the battery pack itself. For example, when I am charging my current lipo setup (4 x 6s 5000mah) I have a power supply that provides 12 volts and can rock out up to 1200 watts. I would like to just use that guy to charge a life4 12s setup.... but I am unclear on how I would get that 12v (3s) from the power supply ramped up to 48v (12s)?? For those 4 6s batteries just using a hobbyking quatro charger makes it easy as cake. Obviously this is where the space cell has that custom power supply/charger, but I am an avid off-roader so the possibility of using my jeep battery to charge the future me life4 battery pack is most appealing.
```

---
## \#5 Posted by: longhairedboy Posted at: 2015-12-10T12:10:38.354Z Reads: 472

```
This beast looks like it could balance charge anything all the way up to 14S.

http://www.amainhobbies.com/rc-cars-trucks/thunder-power-dc-tp1430c-dc-114-cell-lipo-charger-w-balancer-14s-30a-1000w-thp1430c/p218950?gclid=CNyOnoWh0ckCFc4XHwodFKEErQ

I should definitely get myself a bigger balance charger one of these days.
```

---
## \#6 Posted by: Sharkface Posted at: 2015-12-10T15:37:22.393Z Reads: 453

```
[quote="longhairedboy, post:5, topic:695"]
This beast looks like it could balance charge anything all the way up to 14S
[/quote]

aaaannnnndddddd my search is over.... it just ended hella expensive lol
```

---
## \#7 Posted by: MonsterCoatings Posted at: 2015-12-10T16:42:50.800Z Reads: 434

```
[quote="Sharkface, post:6, topic:695"]
http://www.amainhobbies.com/rc-cars-trucks/thunder-power-dc-tp1430c-dc-114-cell-lipo-charger-w-balancer-14s-30a-1000w-thp1430c/p218950?gclid=CNyOnoWh0ckCFc4XHwodFKEErQ
[/quote]


Guess all the savings of building my own packs just went out the window. LOL
```

---
## \#8 Posted by: chaka Posted at: 2015-12-10T16:45:18.304Z Reads: 414

```
A custom charger will only set you back about $70.
```

---
## \#9 Posted by: Sharkface Posted at: 2015-12-10T16:45:50.566Z Reads: 407

```
[quote="MonsterCoatings, post:7, topic:695"]
Guess all the savings of building my own packs just went out the window. LOL
[/quote]

yeah kinda/sorta though. at the very least it makes it so you have to budget it out over a few months and not just as a one off type thing. If you are making a battery pack without a BMS, then yeah youll need this, but after building a handful of packs without BMS youll start saving cuz you dont have to purchase the BMS every time. If you are only going to make that one pack, then you mise well get a BMS on that pack, and then find that custom charger that @chaka just mentioned.
```

---
## \#10 Posted by: chaka Posted at: 2015-12-10T16:49:21.338Z Reads: 374

```
I imagine you could retrofit a bms to balance charge all your packs. You could even Install it into an enclosure and plug your balance lead into it when you need to balance your packs.

I could draw a schematic of how it would work if you like.
```

---
## \#11 Posted by: Sharkface Posted at: 2015-12-10T16:57:03.786Z Reads: 365

```
[quote="chaka, post:10, topic:695, full:true"]
I imagine you could retrofit a bms to balance charge all your packs. You could even Install it into an enclosure and plug you balance lead into it when you need to balance your packs.

I could draw a schematic of how it would work if you like.
[/quote]

actually this makes a lot of sense, building off that idea you could almost do a battery style like cell phones had in place back when you could still get their battery out. I am guessing it wouldnt be exactly like that cuz of vibrations, but its inspiring none the less. 

@chaka thanks for the offer of a schematic but I am good on that guy. Just building out a few ideas for now ;)  er wait actually... if you could draw a schematic for converting 12v into 48v so i can just rely on the BMS for balanceing then yeah draw it up buddy lololololol (being sarcastic here as that would be a bit of work)

EDIT: added in a bit to that last sentence to @chaka
```

---
## \#12 Posted by: longhairedboy Posted at: 2015-12-10T17:13:41.462Z Reads: 343

```
onboard BMS is still the best option if you have the space for it i would think. Even the big ones which are long and sort of wide still aren't very tall and could be packed in either on top of or under the battery pack inside the battery compartment of your box.
```

---
## \#13 Posted by: itsmikeholland Posted at: 2016-06-12T19:50:46.140Z Reads: 320

```
Can you go into more details about a custom charger? I'm trying to charge a 12s 6.6ah rig in an hour, but I'm having trouble finding anything to charge 12s within a reasonable price, and from what I'm reading it seems like series is the best way to charge since you can balance cells individually. I have 3x 4s batteries
```

---
## \#14 Posted by: Hummie Posted at: 2016-06-13T05:02:37.738Z Reads: 318

```
They've been out of stock forever.  I've yet to find a balance charger that will do 12s but even if another becomes available for sale again someday I won't bother as it'll likely cost a fortune and bulk charging is easier. 

  Charging 50 volts or 12s. (Someone mentioned lifepo4 which is different) can be done without a bms by using a bulk charger and little balancer/dischargers like the battery medic.  That's what I do.  I use the Meanwell 48volt power supply and it's adjustable but it's an awkward machine and finicky and ur better off finding another "bulk charger" that Is more user friendly.  They're out there.  Electric bikes use them. 

U can charge with a 15 dollar bulk charger intended for a computer that will do 48 volts and get u to 4 volts a cell. It will only do many 3 amps but works.

Space cell is limited to 30 amps. That sucks.  Low power
```

---
## \#15 Posted by: hotwire Posted at: 2016-07-03T20:21:28.154Z Reads: 286

```
I have a similar question I'm just about to finish up my 12s 4p pack just waiting on the BMS I'm using LG HE4 and 60amp bms my question is I just received my 48v charger and it puts out 56.3v. My understanding is I couldn't go over 50.4 V I know the BMS will protect it from overcharging but I rather not rely on the BMS so I need some opinions should I or can I use this charger.
```

---
## \#16 Posted by: Nordle Posted at: 2016-07-03T20:31:25.954Z Reads: 280

```
Most (aluminium cased) chargers have pots inside to adjust voltage and current.
```

---
## \#17 Posted by: lowGuido Posted at: 2016-07-03T20:51:44.457Z Reads: 280

```
I like to think of charging batteries like filling buckets of water with a syphon. 
if you want to fill one bucket from another, it needs to be a higher potential than the other.

such that if you want to charge a 48V battery (13S @ 4.2V =  54.6V)  then you will need a charger of a higher voltage.

so to charge a 48V battery you need a 55+V charger.
```

---
## \#18 Posted by: hotwire Posted at: 2016-07-03T21:24:31.896Z Reads: 279

```
No it doesn't have a pot inside it's a bulk charger and it's 12s pack not 13s so 44.4v and max 50.4 can anyone recommend a better charger that's not from Supowerbattery cause I'm still waiting on the BMS from them or will that 13s bulk charger I have will work on 12s with bms until I order the right charger
```

---
## \#19 Posted by: dmtdan Posted at: 2017-08-06T11:35:35.714Z Reads: 158

```
how would i go about making a charger sounds cost effective :slight_smile:
```

---
## \#20 Posted by: Highwon Posted at: 2017-09-29T04:38:32.056Z Reads: 133

```
What BMS did you get?
```

---
