# Turnigy Reaktor 300W 20A 6s Balance Charger

### Replies: 20 Views: 3659

## \#1 Posted by: Mobutusan Posted at: 2016-02-20T23:17:26.556Z Reads: 181

```
I've been having a hard time trying to figure out what battery charger to get, and after reading all the battery charging posts on this site, I haven't seen this unit even mentioned. Has anyone had any experience with this charger?

https://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=56924

It seems to be quite a bit more powerful than the popular 50W B6AC and 80W Accucel chargers, but is still reasonably affordable. Currently ~$65 on HK (U.S.-West), but can be had for $57 using the buddy code links on rcsearch.info:

http://rcsearch.info/hobbyking/buddy/?strSearch=reaktor+300#catalog

According to this site, it sounds like this is almost identical to the icharger 206b which costs twice as much. 

http://www.rcgroups.com/forums/showthread.php?t=2115921&page=1

In my estimation, charging a 6s 5000mah battery at a 2c rate would take around 30min. on this charger vs. 1.5 - 2.5+ hours on the B6AC & Accucel chargers. 

Thoughts?
```

---
## \#2 Posted by: Mobutusan Posted at: 2016-02-26T08:03:47.917Z Reads: 157

```
If anyone is interested, the 250W 10A Reaktor is on sale for <$25 ($23 if you wait for the pop up deal) on Hobby King (US). That's less than the BA6C or Accucel. The 300W unit was backordered, so I found this 50% off deal instead.

http://www.hobbyking.com/hobbyking/store/__78380__Turnigy_Reaktor_250W_10A_1_6S_Balance_Charger_US_Warehouse_.html
```

---
## \#3 Posted by: Okami Posted at: 2016-06-06T11:53:13.003Z Reads: 129

```
Hey! I'm also in a search for a suitable charger.. So what was your final choice then?

I'm using CalcRc to calculate the approx time it would take to charge the batteries.. and yeah would be willing to charge at 10A, 5A for each 5000mah 3s pack, Because charging 6s (2x 3s serial) packs with 2.5A each, would take something like 2hours.. I would be happy to get that number to 1hour.. so that i could get a  chance to ''quick charge'' if im somewhere out of home with the board and have to recharge the batteries outside of home.

So far I have found the Accucel 6, which is capable of 7a charging.. which is a lot more decent than imax b6 with 5a/50w.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-06-06T12:00:53.215Z Reads: 114

```
Keep in mind that a "fast charge" is not that good for your lipos. You will stress them and they will not last as long as you would have charged them slowly.
Another keypoint of fast charging is that the chargers are more expensive!
```

---
## \#5 Posted by: Maxid Posted at: 2016-06-06T12:04:29.027Z Reads: 112

```
[quote="Okami, post:3, topic:1478, full:true"]
...would be willing to charge at 10A, 5A for each 5000mah 3s pack, Because charging 6s (2x 3s serial) packs with 2.5A each, would take something like 2hours...

So far I have found the Accucel 6, which is capable of 7a charging.. which is a lot more decent than imax b6 with 5a/50w.
[/quote]

Keep in mind the watts the charger can output. At 6S and 1C (so 5A) you already have 126W.
If you charge every battery separately then this will double your charging time again.
Your best bet is to get a 6S charger and charge them in series. At 1C it will take them an hour to be full. But as @DeathCookies has already said: the faster you charge the more it will damage your batteries. That is why I charge at only 0.5C and up to 4.1V instead of 4.2V

Also in series you don't need 10A to charge them at 1C - you still need 5 and only the voltage goes up. In Parallel it would be the other way around
```

---
## \#6 Posted by: Okami Posted at: 2016-06-06T12:07:03.784Z Reads: 101

```
Yeah, Im very well aware of the fact that fast charging may damage the batteries. I would not be doing all the time though, only when I need to.

W
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-06-06T12:12:15.060Z Reads: 98

```
Do it correctly!
I just bought a 1080W power supply and a 400Watt dual output (800Watt) charger.
Then i can charge two 6S batteries with 18A each. So i can charge one of my boards (2x 6S 8Ah) in a half hour. That is fast charging but i nearly never do that. It is much wiser to know when you have to charge and if you are in the hurry you should swap it with a charged battery.
```

---
## \#8 Posted by: Okami Posted at: 2016-06-06T12:20:21.563Z Reads: 93

```
Good point actually.. perhaps I should just invest in bigger or more batteries rather than fast charging.. since the weight should be very similar between carrying extra batteries or carrying a charger + psu around.. 
 
Anyways.. will probably go for accucel 6, as that is able to charge a little bit more faster than the imax b6.. since 1c is 5a, and Im probably going to be charging with 3.5a (0.7c) one 5000 3s pack, which is still quite good
```

---
## \#9 Posted by: Maxid Posted at: 2016-06-06T13:04:49.178Z Reads: 94

```
As I said the accucel 6 ist only rated 80W and thus should not be used to charge 6S at more than 3A.
Also your PSu needs to support more Watts.

Just go with a Reaktor 250 10A charger - they are pretty cheap and clones of the more expensive Junsi iCharger 106B+.
```

---
## \#10 Posted by: DeathCookies Posted at: 2016-06-06T13:39:59.122Z Reads: 90

```
I would not recommend to buy a RC PSU. It is much more expensive than a normal [3d printer PSU](https://www.amazon.de/gp/product/B0191H4VF2/ref=s9_simh_gw_g201_i1_r?pf_rd_m=A3JWKAKR8XB7XF&pf_rd_s=desktop-1&pf_rd_r=Z3M14GTKSWH9CZKN9FQN&pf_rd_t=36701&pf_rd_p=942141227&pf_rd_i=desktop).
```

---
## \#11 Posted by: Maxid Posted at: 2016-06-06T13:48:42.039Z Reads: 87

```
I just use an old Computer PSU - get the 12V cable and ground and you are good to go.
They are super cheap and almost everybody has some spare ones lying around.
With usually at least 250W they are also more than capable of supplying a large enough current.
You can even make your own adapter to hook the charger up to any PC PSU - so no reason to carry the PSU to work for example - just hook it up to your PC under the table.
```

---
## \#13 Posted by: Bobfandango Posted at: 2016-06-06T18:08:06.760Z Reads: 88

```
FWIW, I use two of the Reaktor chargers mentioned by the OP.  It *is* a re-branded Junsi 206b. 

I ride 12S4P, but built my pack as two 6S sticks.  It is certainly not terribly convenient that I have to pull the cover off to get to the balance leads and charge connectors.  I could in theory rewire everything to bring charge and balance leads to the side of the enclosure, but I doubt I will bother. I charge the entire pack at once, each half on its own charger.  I charge at the standard charge rate for LG HG2s, 1.5A/cell or 6A total for the pack (since they are wired 4P).  I run a 3.1V cutoff and 4.1 charge, so it takes about 1.5 hours to charge the pack and maybe another 5 to 10 min to take apart the board and put it back together and what not....   

Anyhow, since I'm not running a BMS, it gives me some piece of mind knowing the pack is fully balanced every charge.   The cells are staying very well balanced at this point.... which you'd expect of (what were) new HG2s.  

I bought a Meanwell, but haven't gotten around to doing a constant current mod to it yet....  I may do that and bring out a charge connector so I can charge it without taking anything apart, and do periodic balance charges as needed...
```

---
## \#14 Posted by: Mobutusan Posted at: 2016-06-07T06:46:06.291Z Reads: 86

```
Here is my "all in one" charging setup. It allows me to charge two 3s 5000mah Lipos in parallel at 8 amps, so full charge takes about 1:15 or so at 0.8c charge rate.
<img src="/uploads/db1493/original/2X/2/20a1df925f3a2ba636eed72dc4d2b7b9a1c3016d.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/1/1c77acfbd5614467f33721618cda882f019f516d.jpg" width="690" height="388">

I'd really like to try one of these, but I haven't been able to find any reviews on them. I may just buy two to try them out and to save on shipping, unless someone in the San Francisco area wants one too?

http://m.ebay.com/itm/Turnigy-Reaktor-12v-75amp-900-watts-R-C-Power-Supply-Protek-RC-/172219379329?nav=SEARCH
```

---
## \#15 Posted by: itsmikeholland Posted at: 2016-06-12T19:11:41.538Z Reads: 73

```
wow that charger is small! From the pics on hobby king they look massive!
```

---
## \#16 Posted by: Okami Posted at: 2016-11-23T13:36:06.525Z Reads: 50

```
[quote="Maxid, post:11, topic:1478"]
You can even make your own adapter to hook the charger up to any PC PSU - so no reason to carry the PSU to work for example - just hook it up to your PC under the table.
[/quote]

Sorry for bringing up old topics.. but:

What do you mean by adapter?

The only way to connect to the pc psu is to get wires which you connect to the disk drive or hard drive.. or have you found another place where to connect more directly?

No problem if it a pc you use often and can make the wiring accesible from outside.. not so useful, if it is not your pc.. and have to ask someone to open up the case and get the cables :D
```

---
## \#17 Posted by: Maxid Posted at: 2016-11-23T13:50:19.283Z Reads: 48

```
something like this
http://www.buildcomputers.net/images/molex-to-sata-power-adapter.jpg
so you can cut of the sata part and solder whatever plug you need on there. With this you just go to any PSU and hook it up to a free molex plug.
```

---
## \#18 Posted by: Okami Posted at: 2016-11-23T16:38:21.845Z Reads: 45

```
Yep that's what I imagined. My idea is to use (borrow) laptop chargers.. they wont be as beefy but their voltage is usually higher. Also there's no need to take the cover off of a pc and search for molex cable.. 

Though it would be required to have multiple female laptop ports available, to be able to get the juice from them..
```

---
## \#19 Posted by: rtasca Posted at: 2016-11-23T16:40:31.954Z Reads: 44

```
I have a Reaktor and is BY FAR the best charger I've ever had.
```

---
## \#20 Posted by: Maxid Posted at: 2016-11-23T16:45:29.872Z Reads: 44

```
Probably because it is actually a Junsi iCharger ;)
```

---
## \#21 Posted by: Okami Posted at: 2016-11-23T16:56:23.980Z Reads: 42

```
Btw there's also a similar charger but just with 10A rating. Ppl said it also has junsi firmware n such. It's called "Antimatter". There was quite a good deal for it on banggood. About 50usd.
```

---
