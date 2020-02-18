# Modular Battery System

### Replies: 22 Views: 1112

## \#1 Posted by: niuva Posted at: 2018-07-13T20:38:00.056Z Reads: 253

```
Hi!
I've been thinking of building myself an eSkate now for some time and finally decided to sit down and see if I can figure out the wiring for the battery, since I have zero experience in electronics before. Any feedback is appreciated.

I really wanted to design something that allowed me to easily remove the battery packs for traveling (flying), keep the price low and at the same time keep everything as close to "plug and play" as possible. As the batteries are one of the most expensive part of an electric skateboard, I decided that I'd build one set of 10s2p first and then expand it by building a battery pack nr.2 later on, in hopes of ending up with 10s4p, or more.

So today, I'm here in the hopes of getting some feedback and to double check my wiring diagrams, just in case so I don't end up with a major screwup and burning my house down. 
Each battery pack will have a cheapo 10s BMS in it and each pack will be a 10s2p with Samsung 30Q cells. I will end up adding these packs to eachother in parallel. ( 10s2p -> 10s4p -> 10s6p -> so on).
I'll end up 3D printing a small enclosure that's equipped with two XT60 connectors, forming a battery pack. And as for charging, I'll go with a generic 42v 2A charger.

https://i.imgur.com/HLvLhpO.jpg

Flat 10s2p Battery wiring (Blue numbers are balance wires)
https://i.imgur.com/qyceMKx.jpg
I will be using 18650 cell holders instead of spotwelding the battery packs into 10s2p.
https://www.amazon.de/gp/product/B075V1DYQK/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1

I look forward to hearing your thoughts.
Thanks!
```

---
## \#2 Posted by: Hummie Posted at: 2018-07-13T20:43:38.545Z Reads: 221

```
If u solder or spot weld cells together not legal on a plane
I'm on the same quest and integrating into the deck
```

---
## \#3 Posted by: niuva Posted at: 2018-07-13T20:45:21.887Z Reads: 227

```
I'm using cell holders. Cells will not be soldered and can be removed from the battery packs and stored in their own containers they came with. The cell holders will have a 3D printed enclosure that can be slid open and then emptied of cells. Will fit into rest of the deck enclosure with two XT60's.
https://www.amazon.de/gp/product/B075V1DYQK/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1

Original cell container they came with:
https://img.fasttechcdn.com/463/4637000/4637000-4.jpg
```

---
## \#4 Posted by: JonathanLau1983 Posted at: 2018-07-13T20:51:29.697Z Reads: 214

```
I don't think those snap in holders will handle the currents esk8 requires. 
Check out this video using similar for a power wall
https://youtu.be/9YwErplHps8
```

---
## \#5 Posted by: Hummie Posted at: 2018-07-13T20:58:47.146Z Reads: 210

```
I think most of them won't handle decent current. U could add compression foam and better connectors, but at that point might as well do the plastic holder as u want to match too
```

---
## \#6 Posted by: niuva Posted at: 2018-07-13T21:25:35.050Z Reads: 196

```
How about reinforcing the contact points with copper braid / de-soldering wire. 🤔
I really like the idea of these 18650 cell holders and don't mind the extra hours spent reinforcing them to be able to take the extra amps.
```

---
## \#7 Posted by: Acido Posted at: 2018-07-13T21:35:37.385Z Reads: 188

```
You will need to beef up the connections real good
```

---
## \#8 Posted by: chuttney1 Posted at: 2018-07-13T21:45:03.176Z Reads: 181

```
I believe those cell holders are good for at least 10 amps on each terminal. I can understand if someone wants to use these and not spend money on a spot welder.
```

---
## \#9 Posted by: niuva Posted at: 2018-07-13T21:50:55.775Z Reads: 183

```
Spot welder did cross my mind, but I'd probably use it a couple of times and that would be the end of the story - another expensive large paper weight collecting dust in the corner.

Like buying a large bread maker and using it once to make yourself a loaf. It's not really an every day item. 
Vruzend DIY Battery kit was another option, but that also felt like too much of a permanent solution. I'm really aiming for something super modular / plug and play that I can take apart or repair on the spot.
```

---
## \#10 Posted by: boardman Posted at: 2018-07-13T21:51:27.399Z Reads: 183

```
[quote="niuva, post:1, topic:61793"]
Each battery pack will have a cheapo 10s BMS in it and each pack will be a 10s2p with Samsung 30Q cells. I will end up adding these packs to eachother in parallel. ( 10s2p -&gt; 10s4p -&gt; 10s6p -&gt; so on).
[/quote]

Just a heads up that a 10s2p samsung 30q will be in the ~220 WH range which you won't be able to fly with
```

---
## \#11 Posted by: niuva Posted at: 2018-07-13T21:55:12.518Z Reads: 172

```
Even if they're not spotwelded/soldered together, but as individual cells? For transport/flying I'd remove the individual cells from the battery holder. Each cell is aprox 10.6WH on their own.

Edit: 
US: https://www.faa.gov/about/initiatives/hazmat_safety/more_info/?hazmat=7
EU: https://www.easa.europa.eu/sites/default/files/dfu/Background%20Information%20Lithium%20Batteries_update%20Sept%202017.pdf
```

---
## \#12 Posted by: boardman Posted at: 2018-07-13T22:09:59.269Z Reads: 158

```
Sorry I misunderstood the battery pack. You're 100% correct
```

---
## \#13 Posted by: Okami Posted at: 2018-07-14T11:01:57.897Z Reads: 139

```
Check @agniusm / [www.18650.lt](http://www.18650.lt)
```

---
## \#14 Posted by: niuva Posted at: 2018-07-14T12:18:49.937Z Reads: 132

```
Thanks for the hint Okami, these look like a solid alternative. As I’m 3D printing and designing my enclosures myself, I might as well print out a set of those.


How about my wiring diagrams, do they hold up in general?🤔
```

---
## \#15 Posted by: Hummie Posted at: 2018-07-14T17:32:37.756Z Reads: 117

```
i cant really tell what's up with your wiring plan but its better to have all the paralleled cells together and effectively make one cell out of them and they all balance each other.  maybe you did that it's hard to tell
```

---
## \#16 Posted by: wafflejock Posted at: 2018-07-14T17:38:44.501Z Reads: 112

```
Appears from schematic it's 2p per box/battery and 10S then putting the two in parallel so effectively 10S4P but only self balancing between pairs of cells and then between the main leads of each 2P pack
```

---
## \#17 Posted by: niuva Posted at: 2018-07-14T23:15:09.492Z Reads: 104

```
I'm hoping that it wouldn't be an issue having each pack of 10s2p balanced on their own. So effectively 2 BMS's, one for each pack of 10s2p.

Is it ok? 🤔
```

---
## \#18 Posted by: agniusm Posted at: 2018-07-15T06:39:18.630Z Reads: 99

```
If you have 2 10s2p, then you need one bms. You need to do parallel wiring. Bms balance out will have 2 wires for each sense pin. Its like y splitter
```

---
## \#19 Posted by: niuva Posted at: 2018-07-15T15:48:36.381Z Reads: 81

```
Like so?

https://i.imgur.com/TL8BO0k.png

My bms is a cheap 36v 30-40A one, so I'm skipping it on discharge and only planning on using it for charging. And if I understand this right, that's also what I've done in the wiring diagram? 
I have practically no clue about the electronics. :stuck_out_tongue:
```

---
## \#20 Posted by: agniusm Posted at: 2018-07-15T16:04:58.309Z Reads: 75

```
Yes. 10 or 11(on 10s pcm) goes to one battery, same to another. Need to make sure that both packs are equally charged, otherwise lots of current might pass through those thin pcm wires melting them
```

---
## \#21 Posted by: Eboostin Posted at: 2018-07-15T17:02:42.606Z Reads: 69

```
You can charge two separate packs with one bms?? Never heard this before but would be great if it works
```

---
## \#22 Posted by: agniusm Posted at: 2018-07-16T06:29:49.164Z Reads: 63

```
2 exact packs. Your pcm/bms sense wires acts like series link between parallel cells. As currents are low. Just need to remember to do this on new cells.
```

---
