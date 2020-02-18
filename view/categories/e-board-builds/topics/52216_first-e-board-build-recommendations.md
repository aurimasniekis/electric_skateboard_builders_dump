# First E-board Build - Recommendations?

### Replies: 22 Views: 1417

## \#1 Posted by: Matt_54 Posted at: 2018-04-14T03:30:27.346Z Reads: 152

```
I have always been interested in portable motorized vehicles. It started with gas scooters then I found the electric side of things. Initially, I was going to build a skateboard, but I found the builds to be expensive for there results; consequently, I opted for an electric bike. The bike was very cheap and goes +35mph and has 30 mile range, the only problem with it is that it is pretty heavy for a bike. I will be starting my first year of university and my plan was to use the bike, but I have found it might not be the best for shorter trips as it is kind of clunky. Prior to my bike build I bought a complete e-board as I had no prior experience of riding a skateboard, I wanted to see if I even liked it. That being said I have started making purchases for my first eboard build. I would like to have a lightweight set up for portability but would like to stick to a 7 mile or > range. I found a very econmical hub kit: [banshee-2-0-upgrade-kit](https://ridepredator.com/shop/usa-banshee-2-0-upgrade-kit/) which is a reason why I will be made the desicion of a diy board. I am not sure if I have made a mistake going diy with the meepo and verreal board very competitively priced. It seems like a very cheap all put together kit.The seller recommends a 10s battery which ruins my pre existing charger set up at 12s. I was just about to place an order for [ 5 2s lipos](https://hobbyking.com/en_us/turnigy-5000mah-2s-7-4v-60c-hardcase-pack.html), but thought I would post here first. I will put those into series and bulk charge them in an enclosure. I am just not sure how to go about finding or making an enclosure. It looks like i can make a mold and bake one in my oven with KYDEX. I am also not sure what deck to use as I would like stay lightweight as possible, as great as long boards are they are pretty big. What power switch seems to work well and what is used as a voltage meter? Does anyone have any insight that may help? I do not plan on spending more than $400. I may be able to reuse my yuneec ego.
```

---
## \#2 Posted by: goldrabe Posted at: 2018-04-14T12:58:39.627Z Reads: 125

```
The Banshees kit's ESC comes with a switch and the remote has a battery indicator which only shows roughly whats left in percentage. You could make a antispark XT90 loop key and put that between your Lipos and the ESC and solder a proper voltage display between the XT90 antispark loop key and the ESC. In this case you would plug the antispark and see the voltage of your battery and after that you need to turn on the ESC with the supplied switch.
This display would work.
https://www.amazon.com/XCSOURCE-Waterproof-Lead-acid-Backlight-BI728/dp/B071GMVXFD/ref=pd_sbs_469_13?_encoding=UTF8&pd_rd_i=B071GMVXFD&pd_rd_r=MGNJAK9PB791ZD7H26CS&pd_rd_w=9H8Jc&pd_rd_wg=JMBNV&psc=1&refRID=MGNJAK9PB791ZD7H26CS

Antispark loop key.
https://www.electric-skateboard.builders/t/xt90-s-antispark-connector/32646

Antispark switch supplier.
https://www.electric-skateboard.builders/t/launch-of-antisparkheaven-com-bulletproof-antispark-switches-nice-prices/31872

And for the deck, my choice would be a nice cruiser or freeride deck with kicktail around the 36 inch mark. For me 36 inch is the sweet spot between good stance an portability. But this may vary i am a rather tall guy, so your sweet spot might be something different.
```

---
## \#3 Posted by: Matt_54 Posted at: 2018-04-14T13:52:10.399Z Reads: 99

```
Thank you for the reply! I will include a loop key but it doesn't seem very convenient plugging and unplugging the key all the time. I could solder a new switch onto the esc and re route it onto the enclosure, but would that be safe because the battery will still be giving power to the esc. Ideally I would have a switch prior esc, l guess the loop key may work if i used it like an actual key but I imagine losing that little connector to be an issue. I will also use a cruiser I just have to figure out what size works best. Thank you for the help.
```

---
## \#4 Posted by: goldrabe Posted at: 2018-04-14T14:25:58.812Z Reads: 91

```
You don't need the loop key, you could plug your Lipos directly in to the esc and use the switch already supplied with the esc. But in this case you can not monitor the Voltage properly, which is important if you use the Lipos without BMS. The voltage diaplay which i linked in my reply has an on and off switch so you could solder that between battery and esc. In this case you need to switch the diaplay on and off before and after you are using the board.
And if i recall correctly this kind of esc gives a nasty spark when connecting your Lipos after charging.
```

---
## \#5 Posted by: aigenic Posted at: 2018-04-14T15:38:52.236Z Reads: 81

```
Not if ou use XT90S connectors ;) 

I think it might be good idea to browse some of the kids from [diyeboard.com](https://1drv.ms/p/s!AlblNnR-rH_6jl8zsFdRpMYHo7iQ)
It is chineese vendor, but many ppl on this forum are using thier kits, especially those who go low cost way :) 

I was once in a similar position as you are...I bough many cheap parts and I replaced most of them with better and more expensive parts :) But back then the market with cehap components was much smaller :) 
But if I should build cheap board again, I would use second hand parts...IMO it is much better to buy used but proven and working parts than spend your money on cheap crappy parts that end up dead in few weeks or months :/
```

---
## \#6 Posted by: E1Allen Posted at: 2018-04-14T15:50:40.015Z Reads: 73

```
I use xt90s loop key.  My nano X remote has a lanyard so I just loop the loopkey to the lanyard when I'm done.
```

---
## \#7 Posted by: Matt_54 Posted at: 2018-04-14T21:45:00.922Z Reads: 66

```
Yeah I think I will do something similar.
```

---
## \#8 Posted by: b264 Posted at: 2018-04-14T21:46:45.689Z Reads: 63

```
DIY does not make "cheaper" boards, it makes "better" boards.  If you want a toy, get a Meepo, if you want a tool get a Metroboard Shortboard
```

---
## \#9 Posted by: Matt_54 Posted at: 2018-04-14T21:48:36.442Z Reads: 65

```
Should I buy this battery? http://www.electric-skateboard.builders/t/10s2p-meepo-1-5-battery-and-case-price-drop-now-80/45487/34 I am not sure of the quality and it is only 4ah however that is proabaly all I would need. Plus it is outfitted with all the bells and whistles, I assume it has a BMS so all you would have to do is plug it in and not worry about it?
```

---
## \#10 Posted by: Matt_54 Posted at: 2018-04-14T21:54:36.738Z Reads: 62

```
Yes I realize, otherwise this forum would not exist. I will be making a board comparative to expensive pre made ones for a fraction of the cost. Or a higher quality board compared to a complete for the same price.
```

---
## \#12 Posted by: b264 Posted at: 2018-04-14T22:06:44.693Z Reads: 55

```
[quote="Matt_54, post:10, topic:52216"]
I will be making a board comparative to expensive pre made ones for a fraction of the cost.
[/quote]

:rofl:  No, you won't :rofl:
```

---
## \#13 Posted by: Matt_54 Posted at: 2018-04-14T22:42:04.167Z Reads: 52

```
What do you recommend? Is this https://ridepredator.com/shop/usa-banshee-2-0-upgrade-kit/ not a good choice?
```

---
## \#14 Posted by: goldrabe Posted at: 2018-04-14T22:44:12.958Z Reads: 53

```
Yes this battery is just plug and play, the only thing you need is charging port and charger for it.
But this battery has a lot of voltage sag i would not really recommend it. I read that they offer 5,2 Ah and 6,4Ah batteries now which have better cells means less voltage sag.
And @b264 is right, you can't do cheaper then the chinese companys.

Edit*
i just saw that the case is included with the battery, so you only need a charger in this case.
```

---
## \#15 Posted by: b264 Posted at: 2018-04-14T22:44:31.837Z Reads: 54

```
I can't recommend anything that doesn't use 4 longboard wheels, for a start.  And, if you want cheap, then DIY is not for you.
```

---
## \#16 Posted by: goldrabe Posted at: 2018-04-14T22:54:01.995Z Reads: 55

```
This kit is the best out of the cheap generic chinese stuff. I started out with something very similar and upgrade my way to a decent board now. But i bought a very good 10S5P Samsung 30q batterypack in the beginnng and use that as the heart for a build with better components.
```

---
## \#17 Posted by: Matt_54 Posted at: 2018-04-14T22:58:38.423Z Reads: 51

```
I plan on using a cruiser and that is a longboard. You guys may be right in the whole diy/cheap chinese boards. Just buying a meepo could be alot easier and not much of a price difference. For the same thing, since I am trying to spend the minimum.
```

---
## \#18 Posted by: Matt_54 Posted at: 2018-04-14T23:03:24.142Z Reads: 52

```
Yeah I have also seen their voltage sag problem but I thought the battery the user was selling on here is there 1.5 version with better cells to correct for the voltage sag. Does it still have voltage sag? Thank you very much for the help, I don't know all too much about eskate.
```

---
## \#19 Posted by: Matt_54 Posted at: 2018-04-14T23:05:49.596Z Reads: 46

```
What is your current set up? That is definitely a battery to keep! It's huge.
```

---
## \#20 Posted by: goldrabe Posted at: 2018-04-14T23:11:01.145Z Reads: 50

```
Sorry man, i can not answer your question with 100% certainty, but my understanding was that the 4,4Ah packs cells where not changed. Only the bigger options had cells with less voltage sag.
The best thing is to ask the seller directly.
```

---
## \#21 Posted by: Matt_54 Posted at: 2018-04-15T03:12:33.780Z Reads: 41

```
I don't understand.  The meepo board claims 11 mile range but I used http://esk8.today/2016/12/28/how-far-can-i-ride/#rc And the result is wayy less than 11 miles.
```

---
## \#22 Posted by: goldrabe Posted at: 2018-04-15T04:01:08.669Z Reads: 39

```
Range depends on many things. Your weight, the pavement, if they are hills, wind etc.
The meepo 4.4Ah battery is sad to be sagging after you reach around 50% of the capacity.
In this regard are the Lipos you linked to better. But you have to take care of them maybe more than Li-Ion batteries.
My advice would be to get a decent battery and from there on you can replace and upgrade your parts surrounding your pack.
Edit*
I saw that the app you were using calculates the range with 25Wh per mile, this is very conservative. 
But I think, if you take the sagging in account, this is what you get in range with a decent performance of your board, after that it will likely start creeping.
```

---
## \#23 Posted by: Matt_54 Posted at: 2018-04-15T06:58:22.808Z Reads: 35

```
So I think I mind as well purchase a Li-Ion pack. Did you make your pack? I am not sure on the size pack I would like, I am thinking 3p or 4p. Do you have a recommendation, it seems all I need is 3p, 3p should be enough. But a 4p pack is only $50 more. Let me know what you think. What is the range difference?
```

---
