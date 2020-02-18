# Battery: 26650 LiitoKala Lii - 50A 5000mAh

### Replies: 18 Views: 1659

## \#1 Posted by: webst Posted at: 2018-03-19T06:44:16.884Z Reads: 199

```
I found this battery, looks promising but I don’t know the brand etc. Has any of you had any experience with this company? What do you think about it? Previous model has very good opinions and was maesured very good on lygte-info.dk

https://m.gearbest.com/batteries/pp_663615.html?lkid=10956872
```

---
## \#2 Posted by: Maxid Posted at: 2018-03-19T06:51:18.107Z Reads: 194

```
Isn't that the same model than on lygyte? He tested a cyan and a black version.
```

---
## \#3 Posted by: webst Posted at: 2018-03-19T06:52:49.787Z Reads: 188

```
I found only cyan one. I’ll check it but I’m more interested on how it performs in time if anyone uses it. What do you think about it? Would you choose this over Samsung 30q for your build?

Found it:
http://lygte-info.dk/review/batteries2012/LiitoKala%20INR26650-50A%205000mAh%20(Black)%20UK.html
```

---
## \#4 Posted by: Vanarian Posted at: 2018-03-19T10:05:09.759Z Reads: 170

```
Nah just look at the discharge & temp graphs, then compare weight and size with an actual 30Q. Compare price too.

Any cell adversiting specs it can't pack *is* a bad cell by definition, and this is no exception. 

Next!
```

---
## \#5 Posted by: pat.speed Posted at: 2018-03-19T10:22:38.774Z Reads: 158

```
What if a 18650 advertises 24000mah and 80a discharge, but it only has 8000mah and 60a discharge. Does that make it a bad cell?  🤔
```

---
## \#6 Posted by: Maxid Posted at: 2018-03-19T11:06:58.001Z Reads: 150

```
Hm? Lygyte tested this cell as actually quite good. With your definition basically all cells are bad.
```

---
## \#7 Posted by: webst Posted at: 2018-03-19T12:32:56.438Z Reads: 136

```
What @Maxid said, also it packs almost twice as much power in not that much bigger package at comparable price. For me it's a good deal and at 30A discharge 2p seems viable option.

![02|690x394](upload://fZBICMfSytGJi2zkwkkaeNokCSL.png)

Both cost the same on gearbest.

https://lygte-info.dk/pic/Batteries2012/Samsung%20INR18650-30Q%203000mAh%20(Pink)/Samsung%20INR18650-30Q%203000mAh%20(Pink)-info.png

https://lygte-info.dk/pic/Batteries2012/LiitoKala%20INR26650-50A%205000mAh%20(Black)/LiitoKala%20INR26650-50A%205000mAh%20(Black)-info.png
All data from lygte-info.dk.
```

---
## \#8 Posted by: Vanarian Posted at: 2018-03-19T14:13:04.847Z Reads: 110

```
Nope. A cell supposed to advertise **50A** continuous and being reviewed by Lygte as **way to hot at 30A, it can't be used continuously at 30A** means that it is good up to maybe **20A** max. The discharge graph posted above shows the same.

That's my definition of a bad cell, when you can't trust the manufacturer's rating because you put your life at danger if you do so. You can give it a try at factory specs and test if your board won't **fire up** in the bad way. Go ahead.

@pat.speed find me a cell able to make this magic without the magic smoke and even my stubborn forehead will forgive the over specs. 

@webst So you're basically ready to more than double the weight of your battery (46gr /cell vs 96gr / cell), and limit cell numbers (because you won't be able to stuff as many as 18650) to make a 2p config for low amp setup of 30A for 2Ah more per cell?

The LiitoKala is almost 27mm wide vs close 18mm wide of the 30Q. Seems huge if you care for low profile thicnkess.

Guys I've been a believer of the 26650 and went back. The new shit will be the 20700 and 21700 when price drops, but as it is now, stay within 18650 and Lipo grasp.

If you want more 26650 surprises from Gearbest, check UltraFire LI-HP and Li-Mn 26550 cells (purple wrap). Very good at what they do within their Wh despite overspecd. Yet expensive and do not go above 20/30A either.

Heck even LifePo4 M1-B cells with their virtually unkillable cycle and 70A high discharge lose interest when faced against LTO cells in smaller package.

There's no perfect setup yet for your compact battery to stuff under your board. 

You can't have 5 minute charge, 500+Wh, 100A+ discharge, full fireproof and dumb proof, +1000 cycles all combined in a Scrabble box format. Not yet.

Factor in weight, size, shape, ampacity and total range, cost... spend months or more fiddling through cell models, reviews, prices, different sites, go look for **the cell you need** and you'll end up doing the same thing I did : come back to the classics.
```

---
## \#9 Posted by: webst Posted at: 2018-03-19T15:59:33.256Z Reads: 90

```
I understood that you wouldn't go with 1kg more mass and 8mm lower battery pack for the cell that has basically 50% more juice at the same price. Temperature is the same as 30Q at 20A but really how frequently will you use 40 or 60 Amps(2-3p) for such long time for battery to get to 50degrees? In test it took 12minutes for Samsung to get there while LiitoKala took 27 minutes. 

I still don't think it's bad battery per se. For it's price it looks like ideal for someone who needs long range on budget. The only unknown is if measured parameters last in time. I also started to wonder if I need such a range in a first place (12s2p would last roughly for 40km assuming 10Wh/km). I can always charge it to 4.1V and get some more cycles though.
```

---
## \#10 Posted by: Vanarian Posted at: 2018-03-19T16:54:21.789Z Reads: 88

```
I get your point and wish you the best with these cells. But IMHO I'd rather overbuild a bit & double the P counts to lessen the stress put on the cells. 

The load cells continuously take during a ride (discharge, regenerative charge, etc) with quick interruptions in a closed non actively cooled tight space and lots of vibrations + potential frictions makes for a very bad environment. 

You won't achieve the optimal results shown on the graphs *per cell*, though you can definitely achieve good results (else no one here would be running monster boards). As for the cycles, I can't speak as you will be the first using them on a skateboard.

BTW a triangle stack of 18650 cells (if a snug fit) makes 27mm thickness for the pack. Ok let's be fair and add at least 1mm between cells for a quality pack with bit of air circulating. 29mm wide ? Versus a single 27mm cell.

Sooo my point was to compare 1x 26650 against 2x 30Q 18650. No matter the layout, results are the following : 
- Range and ampacity got doubled with 30Q = 6Ah and 40A continuous no sweat. The LiitoKala at 5Ah and 20A is beaten.

- Strain has been halved on cells, makes for a potential longer cycle life for sure cause 2P vs 1P. Might be $ wise in the long run to get the best out of it.

- Search well and you can safely manage 3.25$/cell for 30Q, that's 6.5$ for 2x 30Q ; versus (24/4) = 6$ for 1x LiitoKala. You might manage better prices with bulk order on Gearbest and get 5$/cell. 
Make your call, you can pay 1.5$ less per cell for 1Ah less per P count and a shorter life pack. But if you plan to use your battery pack for years or want to re-use the pack, the 30Q might still be the winner.

- 2x 30Q = 2x 45.9 = 91.8gr. 1x LiitoKala = 95.7gr. Oh well, still end up with a *lighter* 2p pack with the 30Q.

- 29mm thickness for 2x 30Q vs 27mm thickness for 1x LiitoKala. Make your choice based on the listed features, size is a close call again *but* triangle layout means you can get flat faces at the edges of the batterie where with one big round 27mm circle you're asking for a flat rectancle enclosure period.

No offense meant with my different posts, it is just my 2 cents at the end of the day and I really hope your pack will deliver what you want, cause that's your board and your wallet too.
```

---
## \#11 Posted by: Maxid Posted at: 2018-03-19T16:58:35.226Z Reads: 73

```
[quote="Vanarian, post:8, topic:49495, full:true"]
Nope. A cell supposed to advertise **50A** continuous and being reviewed by Lygte as **way to hot at 30A, it can't be used continuously at 30A** means that it is good up to maybe **20A** max. The discharge graph posted above shows the same.

That's my definition of a bad cell, when you can't trust the manufacturer's rating because you put your life at danger if you do so. You can give it a try at factory specs and test if your board won't **fire up** in the bad way. Go ahead.
[/quote]

That is true for basically all cells:
HG2 rated for 20A and gets too hot at 20A continuous
25R rated for 20A and is basically unusable at 20A due to voltage sag
VTC6 rated for 30A and gets too hot
30Q rated for 15A and gets too hot at 15A continuous

Whats the problem again?

I get your point and would also prefer 30Q over these - but bashing them this hard seems a bit off. There are truly bad cells out there that we have to keep people from using but this seems to not be one of them if somebody chooses to go for it.
```

---
## \#12 Posted by: Vanarian Posted at: 2018-03-19T17:05:22.806Z Reads: 69

```
[quote="Maxid, post:11, topic:49495"]
That is true for basically all cells:

HG2 rated for 20A and gets too hot at 20A continuous
25R rated for 20A and is basically unusable at 20A due to voltage sag
VTC6 rated for 30A and gets too hot
**30Q rated for 15A and gets too hot at 15A continuous**

Whats the problem again?
[/quote]

Dude my safety limit for "too hot" is at 80 degrees per cell. That's what **Mooch** use as his safety line as it doesn't show accelerated degradation of the cell under that, namely CDR rating from him (and he's as independant as Lygte). 

VTC6 *is* a bad choice for cell if you plan to really draw more than 18A from it IMHO, it doesn't live up AT ALL to its specs. Apart from packed Wh it should never be used unless in big P counts. Same goes for VTC5, same for VTC5A. 

Sony cells pack a punch with solid voltage and you pay it dirty when you abuse this punch despite the specs written.

HG2 is *decent* and not running as hot as you say, 30Q runs **cooler** than HG2. 25R have dirty voltage sag but acceptable temps. 30Q runs **cooler** than 25R and blows it in every department. All these cells are around or under the 80 degrees limit.

What's your point ? 

Summary : only 30A 18650 cells without bad temp are HB2 and HB6 period. 1500mAh and voltag saggy too. Only 30A 18650 cell with solid voltage and shitty temps is SOny VTC5A period. Best all around performer for 20A 18650 cell is the 30Q period.
```

---
## \#13 Posted by: Maxid Posted at: 2018-03-19T17:08:32.993Z Reads: 66

```
[quote="Vanarian, post:12, topic:49495, full:true"]
What's your point ?
[/quote]

See my edit. You were the one starting to generalize that all cells that don't live up to their ratings are bad cells. I am just saying that this is too drastic of a view.
Also for the temps I considered Henrik's values when he had to stop his discharge tests.
```

---
## \#14 Posted by: Vanarian Posted at: 2018-03-19T17:08:55.606Z Reads: 63

```
Ok my bad, saw your edit after writing. Need some tea to cool down a bit.
```

---
## \#15 Posted by: webst Posted at: 2018-03-19T19:18:37.510Z Reads: 60

```
I think you guys convinced me to go the known/proven road for slightly more money. 10s4p 30Q it is. I'm afraid this way we'll never find new good cells, but not finding bad ones might be worth it as well. 

T.Hanks
```

---
## \#16 Posted by: b264 Posted at: 2018-03-19T19:25:26.845Z Reads: 62

```
We will find new good ones, with discussions just like this.  Just not this time....
```

---
## \#17 Posted by: pat.speed Posted at: 2018-03-19T20:57:32.635Z Reads: 54

```
Lol that was just an example, a very exaggerated one
```

---
## \#18 Posted by: Ronaldinho Posted at: 2018-11-21T03:34:58.025Z Reads: 25

```
they are fake....  we have bought them...  they are 1600mah
```

---
