# Help building 6S2P balanced Li-Ion battery pack

### Replies: 31 Views: 775

## \#1 Posted by: mikyb Posted at: 2019-03-19T13:39:13.187Z Reads: 115

```
Hi,
I've been redirected here from quadcopterforum.com , I'd like to build a battery pack with these specs:
- 22.2V
- at least 5000mAh capacity
- at least 30A constant discharge current
- XT60 plug for charge/discharge
- JST plug for balance
- lightweight

LG 18650 HG2 in 6S2P configuration should meet them:
- 22.2V
- 6000mAh capacity
- 40A constant discharge current (safer)
- about 600g weight

the battery pack is for a quadcopter, my question are:
- 1 ) do you know better quality/price Li-Ion cells in 18650 or other standards? 
- 2 ) I found cheap HG2 cells on AliExpress which suppliers told me they are not genuine but with same specs, can I trust them or where do you advice me to buy them?
- 3 ) can you show me how to wire the 6S2P pack with XT60 and JST plugs for charge/discharge/balance?
Thanks
```

---
## \#2 Posted by: ninTHIENdo Posted at: 2019-03-19T13:46:46.927Z Reads: 111

```
1) Samsung 30qs

2) do not trust them.  use nkon, imrbatteries or other reputable companies.

3) I’m not the one to look for help on that, but there has been lots posted about it. The search button can help with that though
```

---
## \#3 Posted by: yelnats8j Posted at: 2019-03-19T13:46:48.825Z Reads: 106

```
The batterys you want to get are probably not good if there fakes.

Get something like samsung 30q from Nkon
https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html
```

---
## \#4 Posted by: mikyb Posted at: 2019-03-19T13:59:10.135Z Reads: 100

```
do you mean Samsung 30Q?

I know it but is only 15A and I'd be a bit on the edge.

I can't find datasheet for Samsung 30QS.

the reason because I was looking on AliExpress is because I need cells with presoldered nickel strips, because I don't have a spot welder.

I didn't find wiring diagram for 6S2P, I'm not sure how to connect balance leads

what about 21700 cells?
```

---
## \#5 Posted by: Bataleon Posted at: 2019-03-19T14:30:26.542Z Reads: 93

```
Out of interest, is there any reason why you're going for cylindrical cells instead of lipo pouch cells? Lipos are usually a lot more power dense (higher discharge rate for a given capacity) and therefore better suited for weight critical applications like RC aircraft.
```

---
## \#6 Posted by: mikyb Posted at: 2019-03-19T15:06:18.616Z Reads: 87

```
LiIons are lighter so I can build a 6S2P pack with 30% more capacity than a 6S1P Lipo with about the same weight, also they should have a wider workable voltage range. the cons is that they have lower C rating, but in low amperage consumption endurance quadcopters like mine 18650 cells are widely used.
```

---
## \#7 Posted by: thisguyhere Posted at: 2019-03-19T17:21:23.330Z Reads: 80

```
[quote="mikyb, post:1, topic:87629"]
HG2 cells on AliExpress which suppliers told me they are not genuine but with same specs
[/quote]

They dont have the same specs, avoid

[quote="mikyb, post:4, topic:87629"]
only 15A
[/quote]

30Q rated safe at 20a continous, look up mooch's test on them

[quote="mikyb, post:4, topic:87629"]
can’t find datasheet for Samsung 30QS.
[/quote]

Google "30q spec sheet"

[quote="mikyb, post:4, topic:87629"]
I’m not sure how to connect balance leads
[/quote]

It'll depend on bms u choose, but shouldn't be a problem, come back here once u decide on a bms
```

---
## \#8 Posted by: Davide Posted at: 2019-03-19T17:37:12.291Z Reads: 70

```
Nkon.nl or Nkon.ru are amazing, you can get the cells there, if you don’t have any spot welder you can have a look at N.E.S.E modules, they are hella easy to assemble and to check your battery health, BMS would be a good choice bestech
```

---
## \#9 Posted by: b264 Posted at: 2019-03-19T17:42:12.174Z Reads: 71

```
[quote="mikyb, post:4, topic:87629"]
I was looking on AliExpress
[/quote]

Don't buy any skateboard battery from the 'baba
```

---
## \#10 Posted by: mikyb Posted at: 2019-03-19T18:50:15.231Z Reads: 71

```
[quote="thisguyhere, post:7, topic:87629"]
30Q rated safe at 20a continous, look up mooch’s test on them
[/quote]
good to know , I read here https://www.18650batterystore.com/Samsung-18650-p/samsung-30q.htm they were rated 15A.

[quote="ninTHIENdo, post:2, topic:87629"]
* Samsung 30qs
[/quote]

[quote="mikyb, post:4, topic:87629"]
I can’t find datasheet for Samsung 30QS.
[/quote]
[quote="thisguyhere, post:7, topic:87629"]
Google “30q spec sheet”
[/quote]
he wrote 30Q**S**

[quote="thisguyhere, post:7, topic:87629"]
It’ll depend on bms u choose, but shouldn’t be a problem, come back here once u decide on a bms
[/quote]
I wont use a BMS, I'd like to connect a JST plug for balance charging using my iMAX B6 Mini, but I don't know how.

[quote="Davide, post:8, topic:87629"]
Nkon.nl or [Nkon.ru](http://Nkon.ru) are amazing, you can get the cells there, if you don’t have any spot welder you can have a look at N.E.S.E modules, they are hella easy to assemble and to check your battery health, BMS would be a good choice bestech
[/quote]

@Davide are you italian? I don't like these kits like N.E.S.E, VRUZEND etc because are espensive and heavier

I'd rather buy cells with presoldered nickel terminals

![1|200x200](upload://nJHmxCUyiOM4SrqrrK88nqIbiFL.jpeg) 

and insert 3 of them in each arm like in this video

https://www.youtube.com/watch?v=I4IMu__vvhk

otherwise what about combining 4 of these case holders?
![2|500x500](upload://mIte7ngm9K8hzsWWdj2wUaXhu5b.jpeg) 

regarding chinese cells (since I dind't find cells with presoldered nickel terminals elsewhere) I'd ask to sellers and if they guarantee me the specs, I'd give it a chance, in worst case I'd ask to refund.

even for genuine LiPo batteries they recommend to never leave them in charge unattended
```

---
## \#11 Posted by: ninTHIENdo Posted at: 2019-03-19T18:51:20.068Z Reads: 58

```
Sorry, I was meaning multiple and forgot the apostrophe. 30q’s
```

---
## \#12 Posted by: mikyb Posted at: 2019-03-19T18:52:33.345Z Reads: 57

```
np I had imagined it but in doubt I asked ;)
```

---
## \#13 Posted by: thisguyhere Posted at: 2019-03-19T19:07:48.447Z Reads: 58

```
[quote="mikyb, post:10, topic:87629"]
he wrote 30Q **S**
[/quote]

Thats plural, S, no such thing as 30qs
```

---
## \#14 Posted by: Davide Posted at: 2019-03-19T20:19:56.941Z Reads: 60

```
Yeah mate I am, no one is perfect🤣🤣 don’t know anything about those cell olders, NESE modules are pretty much plug and play and very strong, anyway when I bought the cells from Nkon I saw they can add solder tags if needed
```

---
## \#15 Posted by: mikyb Posted at: 2019-03-20T00:25:41.694Z Reads: 58

```
even on nkon 30Q cells are 15A rated, anyway according to this video (imho trustable) Liito-Kala chinese cells should be good enough, so for half price I'll give them a chance.

https://www.youtube.com/watch?v=q2o3Wc-0fVk

anyone can show me a diagram of how the wiring should be in a 6S2P with XT60 charge/discharge and JST balance plugs? if you can, for semplicity, draw it on this image:

![Senza-titolo-1|499x500](upload://jLYXyzdDXzqlKViYmHmhU7hN7g6.jpeg) 

on soldered tags, soldering iron and 16AWG silicone wire are ok ? any advice on how to do it?
```

---
## \#16 Posted by: wafflejock Posted at: 2019-03-20T07:36:47.648Z Reads: 54

```
![6S2P_layout|690x330](upload://h2iYdOPu1w4V9gz2uOYnQYwkRdB.png) 

Others can check me but pretty sure this is correct.  Basically putting 2 cells in parallel 6 times then wire those groups of 2P into series to make the 6S, each balance lead goes between the groups of cells (measuring from ground through each balance lead you should see the voltages shown if the cells are all fully charged)  Simply check a known good LiPo you have with a balance lead on it for which side is 0V and to see the step by step of voltage from each pin in the plug just keep black of multimeter on first pin and go one pin to the next with red probe (in DC voltage measuring mode).

In the arrangement you've shown I suppose you could pair up the ones in the center of the quad to make 2P groups so would have 2 of those between the 4 cells that meet at center then put the two "extra" ones in the arms as a p-group but having them lined up end to end is putting them in series they have to be side by side or have wires run to effectively have negative to negative and positive to positive (parallel)

Also to note the lines going to the balance port (imagine bottom lines going out of page go to balance connector), those balance lines look like they are connected to battery negative but really anywhere between the cells in series is effectively the same voltage.  So far right most thick red line is same voltage as the black line to it's left (they are just connected with a wire/nickel strip).  Regarding gauge of wire with short runs from what I gather it shouldn't make a large difference but again multimeter is the best way to know for sure measure ohms and can calculate voltage drop given some assumed load/current (search for voltage drop calculators quite a few out there just want DC voltage).
```

---
## \#17 Posted by: mikyb Posted at: 2019-03-20T14:39:10.181Z Reads: 45

```
wouldn't be simpler to make 4 3S packs (one for each arm), then pair them in 2 6S, and finally in a 6S2P ?<br>
or is it not possible beacause of balance leads?<br>
looks like they did that in this video (first image at 0:05)<br>
[quote="mikyb, post:10, topic:87629"]
[Project Hopes and Dreams 6s long flight time quadcopter part 1 Flown with...](https://www.youtube.com/watch?v=I4IMu__vvhk)
[/quote]


is there an order in which to proceed when soldering to avoid damages?
```

---
## \#18 Posted by: wafflejock Posted at: 2019-03-20T22:25:33.995Z Reads: 41

```
You could do that the problem would be extra long connections between the cells in parallel means the resistance on that connection will be higher and less even (shorter the material between two things lower the resistance so closer they are together and closer the discharge connection is to the middle of the wire between two cells in parallel, that said the actual connection points between the metal tabs and cells will probably effect resistance more than being a bit off on lengths of anything).

Regarding avoiding damage to things, the main things are to not get the cells too hot while connecting things and to be sure the voltage of all the cells is matching (within .1V but closer they are the better, when you hook two cells in parallel the voltage will drain from the higher charged one to the lower charged one, the rate of charge/current will depend on how far the voltage is off from one cell to the next, when hooked in series no current will flow until the circuit is completed but you still want the voltage of all the cells in series to be roughly the same (balanced) for the sake of not overdischarging or overcharging any of the cells.
```

---
## \#19 Posted by: mikyb Posted at: 2019-03-20T22:37:55.031Z Reads: 37

```
you are right, in the meantime I understood, now I'm preparing the final schema for confirm<br>
I'll buy all the cells at once and I think sellers charge them before shipping but because of long delivery time they could be different in charge when they arrive, so maybe I'd better buy a 18650 charger too but I think they can only charge to max voltage right?<br>
can I solder balance leads on any of the to the 2P cells?<br>
another question, should I isolate the cells from the frame (aluminium) and each other? and how?
```

---
## \#20 Posted by: wafflejock Posted at: 2019-03-20T23:27:09.276Z Reads: 30

```
Yah if I were to attempt this would probably just center all the batteries having the weight further out is just going to make it harder to pitch/roll and for the quad to balance itself I'd guess and not sure what benefit you'd get spreading the cells out.
```

---
## \#21 Posted by: mikyb Posted at: 2019-03-20T23:42:13.095Z Reads: 28

```
I'll probably place the cells as close to the center as possible to shorten wiring and to have a better weight balance, with screws to keep them in position.

to have them inside the frame allows me to protect them from damage and to save space and weight of battery support.
```

---
## \#22 Posted by: mikyb Posted at: 2019-03-22T14:15:36.559Z Reads: 27

```
I'm a bit confusd regarding AWG and ampacity, because motors are 25A rated and arrived with 18AWG wire, but according to wikipedia 18AWG has 16A ampacity, am I reading wrong the table?<br>
https://en.wikipedia.org/wiki/American_wire_gauge<br>
considering the quadcopter maximum draw of 30A, which AWG should I use for wiring the battery?<br>
```

---
## \#23 Posted by: Fiori Posted at: 2019-03-22T15:36:10.067Z Reads: 28

```
Even the official data sheet says it's safe to run them at 20A. You will be fine.
```

---
## \#24 Posted by: mikyb Posted at: 2019-03-22T15:53:10.160Z Reads: 31

```
[quote="Fiori, post:23, topic:87629, full:true"]
Even the official data sheet says it’s safe to run them at 20A. You will be fine.
[/quote]

which data sheet? but shouldn't it have an ampacity greater than 30A to be safe?
```

---
## \#25 Posted by: Sn4pz Posted at: 2019-03-22T16:41:09.411Z Reads: 28

```
![baba%20batery|375x500](upload://dFv7MAhKmcW0ffqAnEB4Fl5TJST.jpeg) 

First thing I thought of when you said battery and Baba :P 

thats a LHB 30q pack, grandma is packing heat :joy:
```

---
## \#26 Posted by: mikyb Posted at: 2019-03-26T17:32:08.642Z Reads: 22

```
Finally here is the diagram (i divided the 2 arms to simplify reading), is it right?
![6S2P|500x500](upload://qdxqR3tL8jWMl3KBMJ31eSo9JfQ.jpeg) <br>
could someone clarify me about AWG ? on the internet I find discordant tables of AWG and ampacity of wires, maybe it depends on temperature? which wires do you recommend for this battery pack (40A maximum constant discharge current)?
[quote="mikyb, post:22, topic:87629, full:true"]
I’m a bit confusd regarding AWG and ampacity, because motors are 25A rated and arrived with 18AWG wire, but according to wikipedia 18AWG has 16A ampacity, am I reading wrong the table?
https://en.wikipedia.org/wiki/American_wire_gauge
considering the quadcopter maximum draw of 30A, which AWG should I use for wiring the battery?
[/quote]
```

---
## \#27 Posted by: Sn4pz Posted at: 2019-03-26T17:36:14.132Z Reads: 21

```
I've never seen a more confusing battery diagram 🤔 

Maybe it's just my inexperience

Also I think you're drastically misunderstanding how weak a 6s2p of liion cells are
```

---
## \#28 Posted by: mikyb Posted at: 2019-03-26T19:37:30.873Z Reads: 20

```
[quote="Sn4pz, post:27, topic:87629"]
I’ve never seen a more confusing battery diagram :thinking:

Maybe it’s just my inexperience

Also I think you’re drastically misunderstanding how weak a 6s2p of liion cells are
[/quote]
I think this is because of the shape required, what do you mean with weak?
```

---
## \#29 Posted by: Sn4pz Posted at: 2019-03-26T19:41:53.783Z Reads: 21

```
The amount of amperage it can *realistically* supply is low, in addition to mAh

Most packs are larger than this, but I wouldn't know your list of necessities/wants :)
```

---
## \#30 Posted by: mikyb Posted at: 2019-03-26T20:25:28.351Z Reads: 20

```
[quote="Sn4pz, post:29, topic:87629"]
The amount of amperage it can *realistically* supply is low, in addition to mAh

Most packs are larger than this, but I wouldn’t know your list of necessities/wants :slight_smile:
[/quote]

using HG2 cells it will have 40A of constant discharge current and 6000mAh of capacity, my quadcopter will draw a maximum of 30A and higher capacity would be too much heavy.<br>
regarding the diagram, how would you do it?
```

---
## \#31 Posted by: cero10 Posted at: 2019-11-05T21:58:52.243Z Reads: 4

```
So when one has batteries in parallel the constant discharge is added? like the capacity?
```

---
