# Asking for a detail personal opinion on quality of the parts

### Replies: 28 Views: 1051

## \#1 Posted by: Itz Posted at: 2017-10-18T19:39:31.527Z Reads: 136

```
I've been researching for almost a month so what I'm asking is a second opinion from anyone. Why's that? It's beacuse not all of us have a same point of view on things. I hope that you will be able to leave any kind of comment on this tread and It's worth nothing that I strongly welcome the negative opionions.
 
Here is the link of a product:

http://www.diyeboard.com/10s5p-360wh-battery-esc-dual-motor-belt-drive-power-truck-kit-p-590.html?zenid=jd1grt45k7cogivb9hnm75ibk5

So what my real question is what can I expect from this build's specifications? How does it compare to Raptor 2 or Boosted Board?

Thank you in advance and as noted above, every opinion is welcome!
```

---
## \#2 Posted by: Jedi Posted at: 2017-10-18T19:45:24.181Z Reads: 129

```
This discharge on that pack is lower than the battery packs in a raptor or boosted. Meaning voltage sag is likely. Also, that pack weighs a lot.
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-10-18T19:45:46.728Z Reads: 125

```
i wonder what cells are in that 10S5P. That's not a small pack. 

drive system is likely reliable but not high performance. 

more boosted than raptor. Not even in the same class as the raptor drive system.
```

---
## \#4 Posted by: Itz Posted at: 2017-10-18T19:47:17.120Z Reads: 117

```
The cells are LG mf1
Why it doesn't provide high perfomance?
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-10-18T19:59:13.945Z Reads: 106

```
They're small, inexpensive motors designed to work well but not shove out loads of power. 

That cell looks kind of weak. Can't immediately find a discharge curve on that but the specs seem mediocre at best. low current and low-ish capacity.

This would make a good beginner set up.
```

---
## \#6 Posted by: Itz Posted at: 2017-10-18T20:13:17.443Z Reads: 95

```
So how could I improve my board then? Which products should I buy later on?
```

---
## \#7 Posted by: evoheyax Posted at: 2017-10-18T20:24:05.798Z Reads: 94

```
I would not recommend this if you looking for more than a toy. Yes, it'll probably work for a bit. How long, no one knows. But those cells can't kick out enough amps and those motors won't produce enough torque or handle the amps you need to get good torque.

As @longhairedboy said, it's a good beginner board. But theres not a great path of upgrade for you...

You need to replace the esc, replace the battery, and replace the motors. Now, you'll need a bigger enclosure for the battery and vescs, and those motor mounts probably can't take bigger motors, so you'd have to replace EVERYTHING to improve the boards performance.

Better to buy better parts to begin with, so you don't waste money.

If you can't afford everything at once, start with good vescs (like the focbox) and buy cheaper motors, and upgrade those later. Or buy a smaller battery now and upgrade it later. This has no path to upgrade though.
```

---
## \#8 Posted by: Itz Posted at: 2017-10-18T20:30:52.160Z Reads: 87

```
Can you reccomend me parts that would cost me not more than 450$ and that I'm able to buy and get shipped to Croatia(EU)?
```

---
## \#9 Posted by: telnoi Posted at: 2017-10-18T20:46:10.681Z Reads: 90

```
Would save up more money. It will be worth it in the end. Otherwise, you will buy semi-crappy components only to upgrade them a few months later...and as mentioned before, an upgrade path will be next to impossible without replacing almost all parts.
*Esc goes up to 50a, thus a better battery would not even make a difference
*Replacing the esc? You are still stuck with a voltage sagging battery pack with poor braking performance due to low charge rate
*Replace motor? Only a few options due to fixed bolting patterns
*Belt tension incorrect? No way to alter thar

2x focbox (300 euro)
2x 5000mah 5s 60c Lipo (around 140 euro)
Get a board plus trucks for which people here already created and are selling motor brackets
Then you have your pulleys, belts, motors...

Alternative is a 6s build with car ESCs. Will be cheaper. Do a search for reliable car ESCs.

If you insist on getting the components you mentioned you might as well just get a meepo board.
```

---
## \#10 Posted by: Fatos Posted at: 2017-10-18T21:00:15.154Z Reads: 86

```
They are either LGmf1 or Samsung 22p. Both have around 2ah for cell and can discharge at 10A but the sag that you will get from them is out of any proportion. 
<img src="/uploads/db1493/original/3X/4/4/44ecc1fbf728b955cf6e2342099312721bbdd2fd.png" width="690" height="462">.
Maby 5p would help a bit with sag but still he would end up with  2.3 kg of batteries,
```

---
## \#11 Posted by: Itz Posted at: 2017-10-18T21:03:11.238Z Reads: 75

```
So basically the more I empty the battery's capacity the less perfomace I would get?
```

---
## \#12 Posted by: evoheyax Posted at: 2017-10-18T21:07:32.504Z Reads: 72

```
This is true with every battery. I have issues with 12s4p sag with 20a rates cells. Those cells will sag like no tomorrow.

The reality is, you can't build a decent board for under $1000 USD.

Seems everyone has good things to say about Meepo so that would probably be a better bet for you.
```

---
## \#13 Posted by: scepterr Posted at: 2017-10-18T21:08:57.569Z Reads: 75

```
Yeah with mf1 or 22p you need about double the P count you normally would need to keep discharge low per cell and limit sag 
I use them in 10s6p and 10s8p packs where size/weight doesn't matter
I don't categorize these as "power cells" I consider them really good laptop cells..
```

---
## \#14 Posted by: Itz Posted at: 2017-10-18T21:11:51.748Z Reads: 69

```
Could you please explain what is the "P" count? Would really appreciate it
```

---
## \#15 Posted by: scepterr Posted at: 2017-10-18T21:13:32.120Z Reads: 70

```
P= parallel
10s5p, means 5 parallel cells connected in 10s
Discharge A is divided by P to get you discharge per cell
I prefer to run these cells at 5-7A max
Even pulling 5A for a while will heat them up
```

---
## \#16 Posted by: Fatos Posted at: 2017-10-18T21:17:09.494Z Reads: 68

```
@Itz
http://www.electric-skateboard.builders/t/my-centaur-longboard-half-boosted-half-meepo/34971

I had a Meepo board for some days just to try it . They have the samme battery cells. I sold it some days after. If you read from the link you can get more info. There I try to explain the batteries and behavior.. Meepo has only 20cells though .
```

---
## \#17 Posted by: Itz Posted at: 2017-10-18T21:17:15.936Z Reads: 64

```
Could I "mod" this battery to make it less saggy? Talking about changing the p count and s count(connecting batteries in different ways). Sorry if I sound dumb i didn't quite understand things about the battery
```

---
## \#18 Posted by: scepterr Posted at: 2017-10-18T21:18:02.992Z Reads: 62

```
Not really,  if youre able to do that, just build your own pack
```

---
## \#19 Posted by: Fatos Posted at: 2017-10-18T21:18:46.053Z Reads: 63

```
@Itz
  No. You cant . Thats the reason why these batteries are cheap. If you want good batteries they will cost more.

Samsung 30Q are the most prefered , here in this forum
LG HG2

And I myself use  Sony VTC6 and A123 25660(sony cells are harder to find i hear and A123 are expensive and heavier)
```

---
## \#20 Posted by: b264 Posted at: 2017-10-18T21:23:34.854Z Reads: 63

```
[quote="Itz, post:1, topic:35897"]
How does it compare to Raptor 2 or Boosted Board?
[/quote]

It doesn't compare to the Raptor2, because the Raptor2 uses hub motors.  That's comparing two completely different things.  This kit has real longboard wheels and the gear ratio can be tweaked and motors changed.  As far as how it compares to a board from Boosted, I don't know.  Don't have one LoLz

It also appears to be the same kit the Riptide R1 is using
```

---
## \#21 Posted by: pat.speed Posted at: 2017-10-18T21:27:34.242Z Reads: 58

```
How about a single 6374 motor, a Vesc and a lipo pack. That should stay under 450 and give you plenty of performance
```

---
## \#22 Posted by: Itz Posted at: 2017-10-18T21:28:08.848Z Reads: 56

```
So basically my biggest setback is the battery?
```

---
## \#23 Posted by: scepterr Posted at: 2017-10-18T21:36:10.368Z Reads: 52

```
That and the ESC has no customization, what it does is all it will do
```

---
## \#24 Posted by: Fatos Posted at: 2017-10-18T21:38:36.365Z Reads: 49

```
Depends on what you want.  As stated before, if you want to take the kit as it is,then I guess it would work for a beginner that does not want to make hands dirty :). If you think to upgrade in the future it this is not the way to go since every part has its weaknes. And in that case you have to change everything. 
Depends a lot on your weight, hills that you want to climb and the speed you want to climb at?
```

---
## \#25 Posted by: lukeyluke Posted at: 2017-10-18T22:15:30.726Z Reads: 50

```
I ordered their esc/remote/esc case from them last week. Got an email it was shipped today. 

They test check their product before they ship which I thought was nice. 

If your not going crazy for top speed I say go for it. It’s looks like a good kit if your not going for huge speed. Two motors with 50A constant battery will get your hills behind you. I’m still yet to even complete an esk8 build but just with all the reading and numbers checking it looks like a good commuter kit. And like a boosted board for sure. Little less voltage, and more cells in parallel. Not sure boosted’s batteries current rating though. It’s good see the belts are HTD5. I know they also sell HTD3 kits too so good to get the 5 depth. 

Grab a deck you like off eBay. There’s complete boards under $50shipped. Or go to skateshred.com and pick a blank for $20-$50 plus shipping. Or one of their decks. 

My final thought. Despite the cells being lower end. It’ll have 5 sets of 10s in parallel. You got 15mile range looks like give or take. You have a solid fun commuter for under $550 with deck. They sell the same batt pack separate for $98 you could grab later and keep in a backpack to have a longer day of riding. Has an easy on off switch and charge display. Nice feature to have. Little things add up when you wish you had it and don’t. If you want more top end speed just get 90’s or 97’s wheels unless it’s really steep hills where your at. 

Again. Haven’t even gotten my board finished yet but I read a lot when at work with nothing to do hehe. 

If you’re not a performance junkie like a lot of these guys here. Try it.
```

---
## \#26 Posted by: b264 Posted at: 2017-10-18T22:26:32.107Z Reads: 48

```
This kit would make a great backup/travel board, like the Riptide R1, but being a primary rider is unlikely
```

---
## \#27 Posted by: telnoi Posted at: 2017-10-19T04:53:27.298Z Reads: 42

```
The meepo also contains the exact same ESC.
Basically, it has the components listed by the OP.
```

---
## \#28 Posted by: b264 Posted at: 2017-10-19T05:51:20.934Z Reads: 36

```
[quote="telnoi, post:27, topic:35897, full:true"]
The meepo also contains the exact same ESC.
Basically, it has the components listed by the OP.
[/quote]

No way, Meepo is missing wheels.  (hub motors) The components listed by OP have all 4 wheels
```

---
