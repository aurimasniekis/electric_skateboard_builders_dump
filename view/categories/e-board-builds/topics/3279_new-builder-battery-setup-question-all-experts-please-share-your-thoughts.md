# New builder - battery setup question - all experts please share your thoughts!

### Replies: 13 Views: 1869

## \#1 Posted by: listgaus Posted at: 2016-05-14T18:56:20.057Z Reads: 249

```
Hi guys,
I've discovered recently the esk8ts and for at least a month im finding myself developing an addiction serching reading trying to learn and ive decided for an easy start ill go with this setup

The enertion mono rspec pro+ with all the mech incl 12mm pully sys and the bigboy motor
Vesc - i'll have to figure out how to program this fine piece by myself and with help hoping from you guys here
For the remote i've choosen a simple remote like most begginers do
The board will be a bamboo series sektor 9 37.5" with the truck rises supplied in the enertion kit

and my final self debate is on the batteries and charger
I was thinking the best would be either combining 3-4 ZIPPY Flightmax 5000mAh 3S1P 30C in series or use two packs of this batteries 2 in series and switch between them once i run out of juice 
That, or buying 3 ZIPPY Flightmax 5000mAh 4S1P 30C with XT90 and using all togather in a series

My biggest concern is the charger i will need (dont want to spend too much on a pricey charger) 

Im 82kg and my aim is mostly flat with small 15 degree climbs with top speed of 20mph

what you guys think?! 

for now i've ordered the remote. im a moment away from ordering the enertion kit, vest and extra belt just in case
```

---
## \#2 Posted by: lox897 Posted at: 2016-05-14T20:54:22.322Z Reads: 226

```
I would get an IMAX B6AC charger. A lot of people from this forum use it. 3 4s in series would probably be better. Less wires to worry about.
```

---
## \#3 Posted by: listgaus Posted at: 2016-05-14T20:59:51.386Z Reads: 216

```
thx for replying lox897. could i mod the 3 batteries and charge them togather somehow?
```

---
## \#4 Posted by: lox897 Posted at: 2016-05-14T21:01:33.520Z Reads: 207

```
Yes. Using a parallel charging board. Make sure to get the one with your battery connectors. These ones have XT60s.
http://www.hobbyking.com/hobbyking/store/__14856__HobbyKing_Parallel_charging_Board_for_6_packs_2_6S_XT_60_.html
```

---
## \#5 Posted by: listgaus Posted at: 2016-05-14T21:08:32.748Z Reads: 190

```
great! thx! 
should 3 of these batteries do the job?
http://www.hobbyking.com/hobbyking/store/uh_showCart.asp?idproduct=56840&lasturl=
```

---
## \#6 Posted by: lox897 Posted at: 2016-05-14T21:09:46.854Z Reads: 174

```
I can't see your cart. Please give me the link to the exact battery.
```

---
## \#7 Posted by: listgaus Posted at: 2016-05-14T21:12:05.192Z Reads: 176

```
sorry
http://www.hobbyking.com/hobbyking/store/__56840__Multistar_High_Capacity_4S_5200mAh_Multi_Rotor_Lipo_Pack.html

also can you specify what else should i get to make the series connection?
```

---
## \#8 Posted by: lox897 Posted at: 2016-05-14T21:21:08.278Z Reads: 170

```
Do you have a soldering station? I would just make your own harness. I don't think you can buy a harness for three packs in series. Or pay someone on the forum to make you one. http://www.hobbyking.com/hobbyking/store/__29840__ZIPPY_Compact_5800mAh_4S_25C_Lipo_Pack_US_Warehouse_.html
```

---
## \#9 Posted by: listgaus Posted at: 2016-05-15T11:16:25.986Z Reads: 163

```
No but i was thinking about it and to me it seems the best solution that i can do is to build this:

what you guys think about this setup for 4x3S setup?
i was thinking to plug each two batteries with a 3S to 6S charging adapter and to cross a series between them with an arming plug that way when im done riding i could charge each 6s as one battery but when i plus the arming plus i can ride the board via 12S in series. 

is that a good idea? waiting for replies on your thoughts!<img src="/uploads/db1493/original/2X/5/524ea72dd31077309611e2ade1fa00decc14ef5e.jpg" width="612" height="500">
```

---
## \#10 Posted by: AbrownMN Posted at: 2016-05-16T17:56:08.818Z Reads: 143

```
Just my two cents from reading around on here and looking at a lot of reviews, but you may want to consider going with the nano-tech packs or even the Zippy's over Multistar. I have heard nothing but good things about the nano tech packs. They seem to be incredibly reliable and put out consistent power. I have also heard a lot of good about the zippy packs as sort of a standard, well produced pack. I know a lot of the R/C guys use them all the time. The Multistars however have very mixed reviews. While many say they are fine for a cheaper battery, a lot of people seem to think they are rated much higher than they should be. Of course this is all anecdotal evidence from reading, but I believe there have been some tests floating around on the reliability/power of these different packs. If I run across them again I'll post them here for you to take a look at. Hopefully this helps a little bit in your decision-making.

As far as the setup, I think that looks good. Make sure you have an enclosure that fits it all and enough board space with your deck though. When I was considering Lipo packs I would have went with 4 3S Nano Tech packs and done something similar to what you have sketched out there. I wanted to keep it really sleek and easy as possible to charge/setup. Those were the only packs that put out great power and were slim enough for me. At the end of the day, it was about the same cost and more messing around than just buying a prebuilt pack with a display and charge port all built in. Perhaps you want to consider doing the same. It may save you a lot of headache in the long run and probably wouldn't cost that much more. Gotta figure in the value of your time always.
```

---
## \#11 Posted by: listgaus Posted at: 2016-05-16T20:51:55.834Z Reads: 121

```
AbrownMN thanks for the tips! i appriciate your reply.

i'm aiming on a lockNlock enclosure to begin with altough im thinking of making a polyester enclosure since i have plenty that material in handy.
regarding the batteries after giving it some thought i think i will purchase two 5000mah 6S 30C and plug those in parralel hoping to get a good range and a decent speed. charging it will be some headeck in the begining but i'll progress from there gradually. 1st i want to get all the parts and then start the assembly :slight_smile:
Already purchased today my enertion kit and vesc.
this soldering station http://www.aliexpress.com/item/Free-Shipping-9in1-60W-DIY-Electric-Solder-Soldering-Iron-Starter-Tool-Kit-Set-Irons-Stand-Station/32377052521.html?spm=2114.13010208.99999999.261.aKKnXz
3.5mm and 4mm bullet connetor pairs, tx60 connectors and shrinking tubes
now it's a matter of waiting and ordering the batteries and charger :blush:
```

---
## \#12 Posted by: AndyL Posted at: 2017-12-24T17:38:53.801Z Reads: 44

```
Sorry to revive this topic. I've read through many reviews about the Nano Tech batteries, and they are pretty much mixed. I saw this deal on Hobbyking and would like to ask if this would be a good battery to use? 5 in series to make 10s, or 3 to make 6s. Am thinking of purchasing around 10 of them if they are any good, potential to make a 10s2p 12000mAh pack haha. 
Battery in question: https://hobbyking.com/en_us/turnigy-battery-nano-tech-6000mah-2s-25-50c-lipo-pack-xt-90.html
```

---
## \#13 Posted by: AbrownMN Posted at: 2017-12-24T18:49:28.539Z Reads: 40

```
I think the best that can be said about them at this point is that they put out pretty solid power but are inconsistent when it comes to reliability. Some people have issues with them right away, others over time. Usually something seems to occur given enough time, but there are people who claim to love them and never have any problems. They likely just have sub par manufacturing quality control if I had to guess.
```

---
