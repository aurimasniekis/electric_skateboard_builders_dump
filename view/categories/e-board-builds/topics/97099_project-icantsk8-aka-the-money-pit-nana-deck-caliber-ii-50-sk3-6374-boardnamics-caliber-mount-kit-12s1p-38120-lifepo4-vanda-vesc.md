# Project iCantSk8, aka The Money Pit &#124; Nana Deck &#124; Caliber II 50 &#124; SK3 6374 &#124; Boardnamics Caliber Mount Kit &#124; 12S1P 38120 LiFePO4 &#124; Vanda VESC

### Replies: 23 Views: 534

## \#1 Posted by: iSteeb Posted at: 2019-06-22T06:54:43.016Z Reads: 169

```
This isn't just my first DIY electronic skateboard - this is probably the first major DIY project I've undertaken and I honestly thought I'd bitten off more than I could chew for a while there.  I mean, in the end I probably could have bought a Boosted board for not that much more, but I'm pretty fucking stoked with the result anyway.  Pictures, specs and settings at the end.

I'm an Aussie which is generally a pretty dope thing to be, but it turns out the DIY scene here sucks.  I was really limited in what parts were affordably available here, so the parts chosen are actually less my choice and more "that's what you can get."  My main concern was the VESC: I was worried about it being under-spec'd (not many reviews on the Vanda on here), and I definitely wanted to avoid Chinese manufactured ones (too many bad reviews) so the Vanda looked like the best of a budget bunch.  So far, it's working great!

Most of the build came together pretty simply.  The batteries have a couple of layers of electrical tape for insulation, and are then held together with duct tape.  They're mounted onto the board with heavy duty Velcro and an aluminium bar - Velcro keeps it from sliding and does most of the holding work, and the bar just makes sure the Velcro maintains contact.  I couldn't find a good cheap enclosure and don't have the tools to make one, so I'm just using a 3mm rubber sheet.  With plenty of ground clearance, this seems like a good enough option for my purposes and it doesn't look too bad.

Originally I was planning on using the the board's stock trucks, but there were no available mounting options due to it's shitty design, so that is the only reason I got Caliber II's and the Boardnamics mount.  Both are great.  Some Chinese pulley kit fit the MBS wheels perfectly.

I couldn't be arsed to have a switch.  They're expensive.  The XT90's that came with the VESC were pretty stiff so I fucked them off and went with Anderson plugs.  They work so well.  That pretty much wraps it up, although I do have a couple of little tweaks I need to do (better clips to hold the wires to the board, some heatshrink and/or braided wrap for aesthetics on the wires, and a layer of Velcro between the rubber and the aluminium to hold it together).

**Pictures**
![IMG_0831|666x500](upload://a6J6WHfm5UPAVMjOb1iKCUBhMx4.jpeg) 
![IMG_0825|666x500](upload://eV0Lkoj4RVnahg7tpGaIXF80W1U.jpeg)
![IMG_0830|666x500](upload://npQuwuZ4IMyfFrZ3kJnwRXlWKD4.jpeg) 
![IMG_0826|666x500](upload://iO6W6KExTE5DuRsB8Cma5xiwe4k.jpeg)
![IMG_0828|666x500](upload://q3JNVyHfzjTlDhhh0ScHhkwAvcj.jpeg)
![IMG_0829|666x500](upload://oVJiTF8SEPoT18s41LAeNa10WqV.jpeg)

**Parts List**
* Board: https://www.nanaskateboards.com/shop/42-night-forest/ (upgraded to 50 degree Caliber II trucks, and MBS 100mm all terrain wheels)
* Motor: Turnigy Aerodrive SK3 - 6374 - 192KV
* ESC: Vanda VESC https://vandaelectronics.myshopify.com/
* Batteries: 12S1P Headway 38120S (30A continuous, 10Ah, these were a rare score at $20.15AUD each; I decided on these over 18650 cells because they were more cost efficient than accessing a spot welder, and the built in screw heads made building the pack simple)
* Charging: A BMS honestly seemed like a bit of a waste of money, so I just bought an IMAX B6 and plan on charging the cells individually to keep them balanced.
* Mount: Boardnamics Caliber II Kit
* Remote: Cheapest small form factor remote I could find on eBay that was stocked locally https://www.ebay.com.au/itm/Ultra-Mini-2-4Ghz-CH2-Wireless-Remote-Control-Receiver-For-Electric-Skateboard/202074456495

**Specs**
* Max Speed: calculators put it at around 40-45km/h when loaded, and so far I've hit about 35km/h comfortably and it feels like there's more in the tank.  When I max it out, I'll update the thread (might be a while, it's scary at those speeds)!
* Range: again, calculators estimate approx 40km of range.  Once I've actually fully charged and fully run down the board, I'll update this post.  I'd be pretty happy with 30km I think.
* Charging: apparently 60 minutes at 10A.  This sounds pretty fucking quick, so we'll see.

**VESC Settings - Ackmaniac ESC Tool**
* BLDC Sensorless Motor
* Motor Current Max: 70A (motor is rated to 80A, so staying below this for safety)
* Motor Current Max Brake: -30A (I think I'd rather have this at -40A, but, given my teething issues, I'm playing it safe for now and -30A still feels reasonably strong for me)
* Absolute Maximum Current: 130A (VESC default and saw no reason to change)
* Battery Current Max: 30A (the maximum continuous current my Headways are rated at and this seems reasonably safe to maxout)
* Battery Current Max Regen: -10A (1C is recommended for charging, and it seems like having this higher is both outside of the battery's specs and contributing to the braking issues I originally experienced)
* Battery Voltage Cutoff Start/End: 35.00V/34.00V (I've only charged these batteries once, to almost-but-not-quite-full, and haven't run them down to these cutoff voltages yet; as such, these numbers are currently set to conservatively safe levels based on the information I could find online, but if someone has a better suggestion, I'd be happy to hear it)
* Max ERPM/Max ERPM Reverse: 55000/-55000 ( 🤷, really not sure how important this is, but it's close enough I feel)
* Control Type: Current (with Ackmaniac's tool, this allows forward, braking, AND reverse, which so far has worked flawlessly)
```

---
## \#2 Posted by: nuttyjeff Posted at: 2019-06-22T16:43:29.670Z Reads: 115

```
I like how you went with an unconventional battery, but please don't ride it until those exposed battery connections are sealed away..
```

---
## \#3 Posted by: Voxu Posted at: 2019-06-22T20:05:34.638Z Reads: 105

```
40km on a 12s1p?
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-06-22T20:30:24.419Z Reads: 106

```
Those are 10AH 30A cells.

So its a 38.4V nominal (Lipofe4), 10AH capacity and 30A pack, alough 40km is possible it would be extremly hard to achive.

you would have to average 15.5WH/mile to achieve 40km
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-06-22T20:35:24.636Z Reads: 101

```
[quote="iSteeb, post:1, topic:97099"]
Max ERPM/Max ERPM Reverse: 55000/-55000 ( 🤷, really not sure how important this is, but it’s close enough I feel)
[/quote]

if you exceed 60k erpm your vesc will go boom  (limited by 4xx hardware.)
```

---
## \#6 Posted by: Skunk Posted at: 2019-06-22T20:54:22.693Z Reads: 95

```
[quote="iSteeb, post:1, topic:97099"]
the built in screw heads
[/quote]

I was sitting here thinking "did this m*********** really put screws and his batteries?"

It's cool seeing something different.
But yes please do cover those terminals with something.
```

---
## \#7 Posted by: tardyparty7 Posted at: 2019-06-22T21:08:59.342Z Reads: 89

```
please close up that enclosure. That looks extremely dangerous
```

---
## \#8 Posted by: iSteeb Posted at: 2019-06-22T22:13:16.722Z Reads: 82

```
hey man, thanks for this. all i’ve seen is don’t set it more than 60k cos of this. is 55k low enough or should i drop it a bit?
```

---
## \#9 Posted by: iSteeb Posted at: 2019-06-22T22:19:16.258Z Reads: 77

```
yeah that’s about the figure i used in the calculators to get the 40km. i did a cursory search of this forum and it seemed like that figure was a fairly common ballpark for some people’s average use. will have to see where mine lies.
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-06-22T22:25:03.950Z Reads: 71

```
dont mess with those settings.
```

---
## \#11 Posted by: iSteeb Posted at: 2019-06-22T22:27:09.240Z Reads: 67

```
thanks man :) there’s not many builds with them out there which is understandable. i think their regular price is at least 50% higher than what i paid for them plus their energy density is kind of low, so they’re not really a go-to product.  but i got lucky with price and the specs fit my build well enough!  hopefully this post throws a few more people in the direction of the 38120s because not having to spot weld is a bloody saviour.

i really dont think it’s unsafe at all without a proper enclosure though. i mean, whats gonna jump up in there and short the batteries?
```

---
## \#12 Posted by: DEEIF Posted at: 2019-06-23T01:05:21.787Z Reads: 58

```
Rocks, stick, etc...
```

---
## \#13 Posted by: iSteeb Posted at: 2019-06-23T01:19:15.416Z Reads: 56

```
i’m not riding cross country and i don’t think there’s much of a chance of something coming at the board from the side. acceptable risk, imo.
```

---
## \#14 Posted by: nuttyjeff Posted at: 2019-06-23T01:29:02.684Z Reads: 55

```
Wheels kick up a nail, nail shorts the batteries, or punctures them.

You drop an allen key, it shorts them.

Being exposed also makes them alot more susceptible to corrosion and water damage.

I can go on and on, but the bottom line is: protect them batteries.
```

---
## \#15 Posted by: dareno Posted at: 2019-06-23T02:24:26.544Z Reads: 51

```
I like what you have done there my friend.  Something different.  Interesting.  
Working with liion and lipo has us all a bit battery paranoid but even though lifepo is inherently safer it would not hurt to get some protection on them.  
What part of Aus are you in?
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-06-23T03:43:58.919Z Reads: 51

```
[quote="dareno, post:15, topic:97099"]
Working with liion and lipo has us all a bit battery paranoid but even though lifepo is inherently safer it would not hurt to get some protection on them.
[/quote]

anything related with lithium/batteries  is inherently dangerous, especially cause of the power densities of the vehicles we build. :upside_down_face:
```

---
## \#17 Posted by: dareno Posted at: 2019-06-23T04:19:45.967Z Reads: 52

```
Hey bro, are you building a 13s10p? :sunglasses: 

Lifepo are much less volatile and if it wasn't for the size and weight would be a much better choice for esk8.  Isn't that right Brian? @b264
```

---
## \#18 Posted by: AlanZhou Posted at: 2019-06-23T04:35:42.727Z Reads: 53

```
[quote="dareno, post:17, topic:97099"]
Lifepo are much less volatile and if it wasn’t for the size and weight
[/quote]

Energy density is also not as good. 😛

[quote="dareno, post:17, topic:97099"]
Hey bro, are you building a 13s10p? :sunglasses:
[/quote]

😤🤦‍♂️
```

---
## \#20 Posted by: tardyparty7 Posted at: 2019-06-23T05:22:28.463Z Reads: 47

```
the occasional puddle, starts to rain when ur out there. 

[quote="iSteeb, post:13, topic:97099"]
acceptable risk, imo.
[/quote]
lol, not the right mindset when you're racing down a street on a longboard. If there is something you can fix that will cut down on the risk of u getting hurt, you should do it, no matter the amount of pads you wear.
```

---
## \#21 Posted by: iSteeb Posted at: 2019-06-23T05:37:31.392Z Reads: 49

```
i’m in canberra unfortunately haha
```

---
## \#22 Posted by: iSteeb Posted at: 2019-06-23T05:38:46.707Z Reads: 45

```
well it’s really gonna rile you up that i don’t have any protective gear and usually ride in a tank top and shorts lol

and anyway, a little splash isn’t gonna short them out the terminals are too far apart
```

---
## \#23 Posted by: tardyparty7 Posted at: 2019-06-24T19:55:51.592Z Reads: 42

```
[quote="iSteeb, post:22, topic:97099"]
i don’t have any protective gear and usually ride in a tank top and shorts lol
[/quote]

@b264 will have something to say about this. 😂
```

---
## \#24 Posted by: b264 Posted at: 2019-06-25T04:01:01.188Z Reads: 33

```
Not in the censored place I won't.  Come to where it's freedom
```

---
