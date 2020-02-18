# Need help building 12s6p Battery!

### Replies: 26 Views: 2618

## \#1 Posted by: Nerdclot Posted at: 2017-07-06T08:58:04.267Z Reads: 308

```
I just need to make sure I have all the parts first before I move onto phase 2:
So far i have this:
MultiMeter 
pulse spot welder
Soldering iron
glue gun 
multi tool wire
heat gun
shrink wrap
nickle tabs
heat shrink
Samsung 30Q batteries

Not sure on what type of Solder. Lead or Lead free
not sure on wire's
or battery life reader

-Need a solid BMS
a good charger?
Led Power switch for board and battery?
Anything I am missing.
Finally a solid link to how to build the battery correctly. It's my first time.
```

---
## \#2 Posted by: darkkevind Posted at: 2017-07-06T10:10:03.957Z Reads: 307

```
Sounds like you have everything except for battery tip protectors: http://www.ebay.co.uk/itm/2X20pcs-Cardboard-18650-battery-Electrical-Insulators-Insulating-Adhesive-Paper/222531849206?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649
```

---
## \#3 Posted by: thisguyhere Posted at: 2017-07-06T16:35:40.396Z Reads: 285

```
this bms seems to be the preferred choice at the moment, they're kind of a pain in the ass to get a hold of.  2 minimum purchase, shipping from china:

http://www.electric-skateboard.builders/t/bestech-10s-bms-usa/22803/73

look at the modifications made to the bms in the group buy.  also, since your pack will have a massive continuous discharge, may want to ask for a bms with at least 100 (or 120) amp continuous discharge rating.

at 12s you'll need a 50.4v charger, either a laptop brick charger at 2amp or 4amp charger for like $60.  shipping from china also.

my 12s4p pack:

<img src="http://www.electric-skateboard.builders/uploads/db1493/original/3X/f/5/f5684d835bd899d78039fcee89ab1883479d245b.jpg" />

<img src="http://www.electric-skateboard.builders/uploads/db1493/original/3X/f/3/f3fe7066ff905c7118fa18f60d977a33cd30ddf2.jpg" />
```

---
## \#4 Posted by: smurf Posted at: 2017-07-06T16:53:04.813Z Reads: 255

```
https://www.amazon.com/gp/product/B004X4KOWS/ref=ox_sc_sfl_title_37?ie=UTF8&psc=1&smid=AJ3PYHDIZANTK

https://www.amazon.com/gp/product/B00068IJOU/ref=ox_sc_sfl_title_36?ie=UTF8&psc=1&smid=AJ3PYHDIZANTK

https://www.amazon.com/dp/B015QHVJR4/ref=twister_B015QHVJOM?_encoding=UTF8&psc=1
```

---
## \#5 Posted by: Nerdclot Posted at: 2017-07-07T07:44:15.159Z Reads: 227

```
you guys are off the Chain!!!! Thank you! Will I need to tune the batteries if they are new?
```

---
## \#6 Posted by: smurf Posted at: 2017-07-07T08:45:59.307Z Reads: 227

```

I tested the internal resistance of 80 cells. it ended up being a total waste of time. There were all the same. New batteries from a reputable company should be good to go.
```

---
## \#7 Posted by: Nerdclot Posted at: 2017-07-07T17:44:52.887Z Reads: 222

```
To be honest I am not quite sure why I would need to have up to 120A? Wouldn't I want to keep it around 60-80 for longer distance. Pleases explain: I know the BMS keeps regulates the current and protects from serges but I thought Ah and or Amps is like the juice to the motors. And I am correct 120A is the max juice that can come out at a time?
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-07-07T18:33:05.782Z Reads: 217

```
ok, your 30q batteries individually are rated at 15amp continuous discharge (many are saying this is understated, they can safely discharge 20amp continuous).

and then you're building a 6p pack, so your pack's continuous discharge will be 90amp, with a much higher burst rate.

generally speaking the bms should have enough "head space" to handle whatever your battery pack can output and then some.

the thinking is, if your battery pack continuous discharge is greater than what your bms can handle, you're just handicapping your battery pack's true performance.  why get a car with 500hp then limit the top speed to 80mph?

your motors will draw a ton of current if accelerating or going up hill or both.  in these instances you want as much current available to your motors (provided the vesc is set correctly).

hope that made sense.
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-07-07T18:35:28.777Z Reads: 203

```
for me, i'm building a 4p pack with lg hg2, which have 20amp continous, so my bms is rated at 80amp continuous with like 250amp burst.
```

---
## \#10 Posted by: smurf Posted at: 2017-07-07T18:41:55.904Z Reads: 200

```
The 120A BMS is designed for a 6 parallel pack . So it's going to have enough discharge capability to keep a 6p pack balanced. But 100A bms is big enough.
Just to throw a curve ball you can skip the BMS and get a balance charger.

http://www.hobbypartz.com/75p-1220-charger.html
```

---
## \#12 Posted by: Nerdclot Posted at: 2017-07-07T19:52:10.714Z Reads: 185

```
Yeah I see a lot of guys using these to regulate their build. But I was hoping to go with a portable charger later on which then I could run into surge problems. Which brings me back to another question Smurf. Why not just go with a portable charger from the start instead of the tekpower? I most likely will have two chargers than? I plan to make a back up battery because of my long commutes but being able to charge the battery while at a location is nice. Is it because of the speed of the tekpower?
```

---
## \#13 Posted by: Nerdclot Posted at: 2017-07-07T19:53:06.470Z Reads: 180

```
Yes perfect! I get it now thank you
```

---
## \#14 Posted by: Nerdclot Posted at: 2017-07-08T05:03:53.258Z Reads: 173

```
also guys what kinda of wire's and connections will I need?
```

---
## \#15 Posted by: thisguyhere Posted at: 2017-07-08T05:45:16.473Z Reads: 177

```
10awg silicone wire

5.5mm bullet connectors

xt90 connectors

https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/82
```

---
## \#16 Posted by: Nerdclot Posted at: 2017-07-08T08:09:51.752Z Reads: 168

```
is that wire going the handle the Amperage?  says max 90amps
```

---
## \#17 Posted by: smurf Posted at: 2017-07-08T08:22:58.043Z Reads: 168

```
10 gauge is big enough 8 gauge will be harder to solder up. Needing a powerful iron.
Your basic portable charger puts out 2 amps.
Now a standard charge for a 6P pack is 6 amps which should take like 3-4 hours.
Now that small charger will take like 9-12 hours to charge and some people have reported that the smaller chargers stop charging about a half a volt to early so the BMS doesn't have a chance to get it's balancing done. That's where a lab quality power supply really starts to shine as it's probably more accurate than your volt meter.
```

---
## \#18 Posted by: smurf Posted at: 2017-07-08T18:48:50.216Z Reads: 152

```
And don't forget the tape

https://www.amazon.com/Foxnovo-Temperature-Resistant-Polyimide-Adhesive/dp/B00N1RHE2Q/ref=pd_sbs_229_1?_encoding=UTF8&pd_rd_i=B00N1RHE2Q&pd_rd_r=G2E727QD8T5TSVT8SZ3Y&pd_rd_w=klsce&pd_rd_wg=aivix&psc=1&refRID=G2E727QD8T5TSVT8SZ3Y
```

---
## \#19 Posted by: Nerdclot Posted at: 2017-07-10T08:31:53.845Z Reads: 142

```
where does this go?
```

---
## \#20 Posted by: smurf Posted at: 2017-07-10T09:12:14.451Z Reads: 142

```
https://m.youtube.com/watch?v=u-4mKh1WaLo
```

---
## \#22 Posted by: Nerdclot Posted at: 2017-07-11T04:22:35.822Z Reads: 136

```
Can someone confirm this? <img src="/uploads/db1493/original/3X/6/8/68ec27decf9c0c69f828a14f32e384309aea687a.jpg" width="690" height="294">
```

---
## \#24 Posted by: Nerdclot Posted at: 2017-07-11T05:30:10.308Z Reads: 121

```
wait bro did you put those heat sinks on the bms?
```

---
## \#25 Posted by: smurf Posted at: 2017-07-11T05:33:26.136Z Reads: 123

```
If that is too long you can fold it over and stack it Two cells high.

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/f/5/f5684d835bd899d78039fcee89ab1883479d245b_1_690x388.jpg
```

---
## \#26 Posted by: thisguyhere Posted at: 2017-07-11T05:38:23.195Z Reads: 126

```
No it comes that way, that's why the bestech stuff is supposed to be pretty legit. U can tell they're well built. 

About your three wide battery pack, not sure what deck or enclosure will fit something that wide.
```

---
## \#27 Posted by: Nerdclot Posted at: 2017-07-11T10:41:55.653Z Reads: 126

```
Its only 8" wide which most decks are 8.6-10. Also i am making a custom Carbon Fiber Deck using a type of pvc foam and carbon molding. Also anyone know a cheap source for Samsung 30q's?
```

---
## \#28 Posted by: Nerdclot Posted at: 2017-07-19T07:48:56.488Z Reads: 123

```
Hey Smurf, How do i use the Tekpower with dc power connector?  5.5*2.1? or is there a better connector out there?
http://www.ebay.com/itm/5-PCs-DC-Power-Socket-Panel-Mounting-Connector-W-Waterproof-Cap-Plug-5-5-2-1mm-/162378537136?hash=item25ce83d8b0:g:BZ8AAOSwImRYWbh3
```

---
## \#29 Posted by: smurf Posted at: 2017-07-19T17:56:55.077Z Reads: 110

```
There are lots of options available but I got a heavy duty waterproof connector

http://www.ebay.com/itm/122288396312
```

---
