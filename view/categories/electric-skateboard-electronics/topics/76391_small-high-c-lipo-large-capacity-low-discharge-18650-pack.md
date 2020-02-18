# Small High-C LiPo + Large Capacity/Low Discharge 18650 pack

### Replies: 22 Views: 548

## \#1 Posted by: skatardude10 Posted at: 2018-11-28T18:37:49.186Z Reads: 152

```
I'll transform this into a build thread if I get to it next year.

I've had this idea floating around in my head for some time now, and I want to post about it to get some thoughts, maybe. 

I am thinking of a relatively slim, 12-13S lipo pack with a high C rating, attached to a large capacity relatively low discharge 18650 pack. The lipo portion will be something up to 300wh to keep it small, but high enough C rated to deliver 240A or so. The 18650 pack will be connected to 1-3 boost converters in parallel to deliver a fairly high charge current of 10-15A to the lipo pack. 

The idea is to have a very powerful quad drive with much higher amp output than 18650s can provide, to avoid a 10+P pack, but maintain the capacity per size advantage of an 18650 pack. This way I can push 240+ amps on demand, but while cruising be able to charge the lipo from the 18650s/boost converter to go much further than the 300wh lipo would provide on its own. 

My proof of concept is my current board, using a low discharge 400wh 18650 pack to charge my main 360wh 18650 pack- it works great and goes really far (further than I've been willing to go to drain it, I love not having *any* range axiety and stopping at mid-voltage perfect for storage if I decide to not ride in a while)... I just currently have half to a quarter of my dream amp output and want to swap to lipos for the main, and do it all up clean this time 😎

Does anyone else do this currently, lipo main pack charging on the go to get extreme amp output with crazy good range charging from a separate 18650 pack? Seems to me like this would be bulky, but the best of both worlds on the road.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-11-28T19:36:34.141Z Reads: 137

```
The question is which advantage you want to get out of it?
That the pack is more light? More cheap?

Which size of pack you want to make the 18650 pack? 
If you make a 12s10p pack out of vtc5a cells you will get a pack with a discharge of 250a with a total weight around 6kg.

If you use the high c rated lipos how you plan you will need what? 2x 6000mAh with 75c?
That would be already 1.8kg or so.
Than a 12s5p pack for charging. That would be another 3kg of cells, plus the boost converter and we in total already at 5kg. 
That’s not that big difference, or?

Why not just get 2 of this
https://www.gensace.de/tattu-14000mah-22-2v-25c-6s1p-lipo-battery-pack.html
That‘s 3,6kg and you get the discharge you need.
```

---
## \#3 Posted by: Jmding Posted at: 2018-11-28T21:37:07.857Z Reads: 123

```
Yeah, I think thats the idea, small improvement in weight. Probably impractical for street riders, but still a cool idea.

I'm not sure how the racing scene works, but I imagine they either need to eventually implement, or already have board weight classes. Otherwise all competitors will just get into an arms race of giant 13s10p 200A battery packs, huge heat-sinks to manage the current through the ESCs, and motors the size of melons. If there were, say, a 14 lb class, it would drive all sorts of creative innovations in all subsystems, including finding ways to make low weight batterys both high power and high capacity as suggested by OP, to super-light trucks and decks, possibly even firmware changes to implement short-term "turbo mode" for motors based on temperature feedback, allowing us to use smaller, lighter motors reliably without being afraid of burning them out.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-11-29T03:25:39.955Z Reads: 108

```
If it would be for racing than it wouldn’t make sense at all. The 1,8miles I can drive with the high c lipos only. No need for extra range.
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-11-29T03:37:07.167Z Reads: 108

```
The idea would be to have a slim pack relative to a 13S10P+ lioon pack on the bottom that packs a big punch, range not being a priority... Just high C. 

Then, like I do now but cleaner, be able to clip on a large pack in the middle on top. 

This way, have all the power output you need. The board stays lightweight until you decide you need to go farther... Maybe 20-50 miles of range... Just clip on a pelican case full of liion batteries and boost converters and plug it in- Either a pelican case or something cleaner, sleeker, printed out of nylon... Not sure yet. Power tool batteries work great for this, but I need to swap 3 or 4 times on longer rides. I'd rather just one big pack... But for lipos. 

Another idea was to combine high capacity liions into a pack with lipos all together in one big pack. It would need to be somewhat modular for when the lipos start to die, but I'll be thinking about this for a while... This might just be dumb. The boost converter is pretty big though... That'd be hmm..


I mainly want the flexibility of not having to lug around literally hundreds of batteries permanently attached to a quad drive.
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-11-29T03:38:04.914Z Reads: 91

```
Not primarily racing. I just need more power!!!!!!! Really. I'll race it, but I want to have a ton of power, and go faaaaar.
```

---
## \#7 Posted by: MoeStooge Posted at: 2018-11-29T03:48:30.787Z Reads: 93

```
I run a low capacity high c lipo close to my esc and large capacity  low c lipo further away in parallel.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-11-29T03:50:56.086Z Reads: 90

```
The idea is good.
I just don’t understand why to make it more complicated than it is.
Just buy 4 of the tattu lipos I linked.
That will give you 40-50km range and you need to swap it out only once and it’s still light.
Your solution could be a bit more cheap thou 😅
Depending on which sells you plan to use.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-11-29T03:52:31.884Z Reads: 87

```
How that works?
Parallel is parallel. They always share the full discharge current over all packs. Doesn’t matter if closer or more far away from your esc.
No?
```

---
## \#10 Posted by: Jmding Posted at: 2018-11-29T03:53:04.665Z Reads: 84

```
Bam! That's exactly the same concept basically, just with all lipos. Moe, you doing that to get as much energy density as possible while still achieving your power output requirements?
```

---
## \#11 Posted by: MoeStooge Posted at: 2018-11-29T04:02:33.064Z Reads: 78

```
The low c lipo hits an amp wall around 100a. The high c never sees it's wall. The amp and volts are held up over short high Amp draw bursts. When the Amp draw settles below the low c lipo limit the voltage eqalizes like water finding it's own level spilling back into the low capacity high c Battery. It allows you to have a high discharge high amp hr pack without spending a fortune on batteries.
```

---
## \#12 Posted by: Jmding Posted at: 2018-11-29T04:11:13.644Z Reads: 71

```
Any reason you went with lipos for the low-c pack? I ran some numbers earlier and found 18650s to be generally more energy dense and cheaper per unit energy as well, but may have missed some lipos
```

---
## \#13 Posted by: MoeStooge Posted at: 2018-11-29T04:15:38.747Z Reads: 71

```
1000wh 260.00 hard 2 beat that.
```

---
## \#14 Posted by: Andy87 Posted at: 2018-11-29T04:55:02.495Z Reads: 68

```
Can you help me to understand that?
I totally don’t get it.
Which lipos you use for the high c and which for the low c and what’s your max discharge current and for how long you draw it from your packs (just in case you have telemetry data 😅)
```

---
## \#15 Posted by: MoeStooge Posted at: 2018-11-29T05:37:42.051Z Reads: 66

```
10000mah 10c lipo.   100a.   
6000mah 90c.              500a
Esc/motor amp.          300a
Will pull equal amp from each battery untill the low c battery gets near it's amp limit. When the low c battery hits it's amp limit voltage begins to drop. The smaller high c battery then begins picking up the demand. It's like water being fed from two different size hoses connected to a bigger hose being pushed by the same pressure. The bigger hose will flow more volume without pressure loss.   Pressure=Volts hose size = amps
```

---
## \#16 Posted by: Andy87 Posted at: 2018-11-29T05:50:16.803Z Reads: 62

```
ok but that doesn´t mean the the request from the low discharge lipo isn´t still there.
even if it´s more easy availaible from the high c pack.
the low c pack doesn´t cut off after 100a.
so it´s still  not good for the low c-rated pack to pull more than 100a.

to come back to your hose example.
I would look from the other side.
You don´t push out the water, you suck it from the esc.
And you suck that water out with the same pressure in both pipes.
in the one with bigger diameter water flows more easy and slowly (so lipo run cooler).
in the one with smaller diameter the water flows faster to supply the same amount of water in the same time (the lipo gets more warm).
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-11-29T05:57:14.393Z Reads: 65

```
I would love to see some real time data on your setup to imagine how it works in real world :D Like some current/voltage sensors to see how load is distributed. Because I think its not only pressure/volume works in this case because higher C rated pack has lower resistance so it will always supposedly be main source of energy as energy flows from lowest resistance source first. that's why low ESR capacitors sits on the ESC to provide that burst of energy
```

---
## \#18 Posted by: Andy87 Posted at: 2018-11-29T06:03:00.920Z Reads: 64

```
with this explenation it makes now more sense for me :sweat_smile:
I´m not that into the water boy stuff...
```

---
## \#19 Posted by: Andy87 Posted at: 2018-11-29T06:06:22.825Z Reads: 64

```
@MoeStooge how you manage to not discharge one lipo too much?
add a lipo alarm to all packs?
what would be the end range in your case.
just like 2x6Ah packs in parallel, or you will than also get more out of it, like 2x 8Ah parallel?
```

---
## \#20 Posted by: MoeStooge Posted at: 2018-11-29T13:47:43.022Z Reads: 62

```
[quote="Andy87, post:18, topic:76391"]
I´m not that into the water boy stuff…
[/quote]

Understanding how electrical theory works for some people is hard to explain. Transmission of electrons across a conductor is most easily explained by using the mechanics of water pushed through a pipe, not "sucked", pushed.  Volts= Water Pressure.  Amps or Current = Flow or size of the hose.   Try and follow. 

[quote="Andy87, post:19, topic:76391"]
how you manage to not discharge one lipo too much?
add a lipo alarm to all packs?
[/quote]

When the small pack high c pack is under high demand for a long period of time there will be a small voltage difference between the high mah low c and low mAh high c packs. When demand dropps to nominal levels for both packs, the higher mAh pack is pushing electrons into the paralleled low mAh pack until voltage is level or "paralled" on both packs.   So back to the water, if you have a large glass and a small glass with a hose between. Water will find a way to seek it's own level as you add or remove water from one side or the other.  Paralleled packs of different mAh behave in this manner.
```

---
## \#21 Posted by: ElectricCoast Posted at: 2018-11-29T14:49:21.575Z Reads: 50

```
Very interesting concept
```

---
## \#22 Posted by: longhairedboy Posted at: 2018-11-29T14:54:51.542Z Reads: 53

```
something like this could be used to manage braking voltage spikes.
```

---
