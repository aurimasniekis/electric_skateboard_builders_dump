# Feasibility Study - Alki Cruiser

### Replies: 14 Views: 271

## \#1 Posted by: DougM Posted at: 2019-01-24T02:09:19.677Z Reads: 116

```
So I know I'm supposed to be working on a different project (the eFoil) but in preparation for spring I've decided to do one more sk8 project - my first one that will actually be based on a skateboard deck - the Alki Cruiser - I'm hoping to mimic old-school.

But I want to skate by all the difficult work (see what I did there) and only make a few changes.

I got this deck:
![image|690x334](upload://bRyFQR85iN32lzpi3htDEhTx0tH.jpeg) 

and want to route 2 channels down the center and put in 10S2P of [these](https://liionwholesale.com/collections/batteries/products/molicel-npe-inr-21700-p42a-45a-4200mah-flat-top-21700-battery-authorized-distributor?variant=15913210675294) cells giving me 8400 MaH, just enough, I calculate, to get from one end of Alki beach to the other and back (about 16 miles going the long way).  These cells are larger than the 18650's, so a custom channel, probably with a stylish bamboo cover to hide it all away.

But here's the tricky part.  I want to buy a Backfire G2T and cannibalize the motors, the remote, the driver and the BMS and install in this build.  The G2T uses Samsung 30Q's so they're just 18650's.  I don't think the BMS would even notice that I swapped in higher capacity so long as I wired them up properly.

So the question is has anyone else done a transplant like this successfully?  Should I go for it or am I going down a path that will lead to a lot of money wasted?

Thanks for any input.
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-01-24T02:19:32.972Z Reads: 95

```
bms work with any cells as long as they have the same nominal voltage and max voltage.. for example a bms for 18650's can be used with 20700 and 21700 cells (even though when bms are designed the designer dont make it cell specific they just state lithium ion and lithium polymer)

[quote="DougM, post:1, topic:81883"]
So the question is has anyone else done a transplant like this successfully? Should I go for it or am I going down a path that will lead to a lot of money wasted?
[/quote]

and everything sound work in thoery. and why swap out the 30q's? the backfire esc needs atleast 24a to work, any cell with a capacity higer than 3000mah has 10a discharge basically...
```

---
## \#3 Posted by: DougM Posted at: 2019-01-24T02:24:13.237Z Reads: 79

```
[quote="AlanZhou, post:2, topic:81883"]
and why swap out the 30q’s
[/quote]


The 30Q's are only a 6Ah pack, so don't have enough range.  The Molicel's are 45A discharge cells, so more than enough to cover the 30A max of the G2T driver.

Plus I want to go as subtle as possible so I don't want that giant black battery box, preferring to integrate into 2 long channels covered with Bamboo.  I realize there'll still be the driver box.

Thanks for your input,
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-01-24T02:24:58.182Z Reads: 72

```
[quote="DougM, post:1, topic:81883"]
8400
[/quote]

Plus 8400mah isdnt even enough for 16 miles...

10s 8400mah is around 302wh and on the avarge of 25wh per mile youll only get 12 miles

im 115 pounds i draw around 20wh per mile and even than youll only get 15.1 miles...
```

---
## \#5 Posted by: DougM Posted at: 2019-01-24T02:27:35.564Z Reads: 61

```
On dual hub motors and flat terrain?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-01-24T02:29:51.109Z Reads: 55

```
Yeah..... thats why youll see wowgo users complaning that they get 6 miles on a 6.4ah pack.
```

---
## \#7 Posted by: DougM Posted at: 2019-01-24T02:59:21.600Z Reads: 52

```
Darn it, the other requirement that I didn't mention was keeping it as light as possible but it sounds like I'm going to 3P 18650's.  But maybe that's not so bad since I get 2P for free when I buy the G2T I just need to buy 10 more cells.  

Cheaper actually, though I had those cells earmarked for an older esk8 with a dead battery pack.

Thanks again for your input.

Do you think the fuel gauge on the remote is calibrated only for the original pack, or will it show true for any pack?
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-01-24T02:59:57.829Z Reads: 50

```
15 miles on a 10s3p pack sounds way more reasonable. (30q) cells produce less mah when there being pushed to their limits
```

---
## \#9 Posted by: DougM Posted at: 2019-01-24T04:54:16.658Z Reads: 42

```
I'll have to think about this.  All my boards to date have been stupidly heavy (because they are all dual motor 10S5P's amongst other things) I might be willing to sacrifice range for weight in this case.
```

---
## \#10 Posted by: pat.speed Posted at: 2019-01-24T05:05:38.404Z Reads: 40

```
I would add 10 cells to the pack you already have, much cheaper and you will end up with more range. 

However an even better option would be to buy some hubs and the rest of the parts separately then you can have whatever battery you want and no big cases, however this could cost more depending on what you want
```

---
## \#11 Posted by: DougM Posted at: 2019-01-24T05:17:48.750Z Reads: 39

```
I was trying to keep the whole project under $1,000.  I spent $40 on the deck so I've only got $960 left :slight_smile:
```

---
## \#12 Posted by: pat.speed Posted at: 2019-01-24T05:20:38.876Z Reads: 40

```
Lol, IMO that is plenty of money for a very nice build. It’s all about the parts you buy, not just buying the best parts but the cheapest with good quality
```

---
## \#13 Posted by: DougM Posted at: 2019-01-24T05:24:23.019Z Reads: 33

```
The sacrifical G2T is $600, add in another $200 for cells and I've got $160 left.  Which isn't bad.  But a major goal was to make this a quick and dirty transplant job rather than a ground up build.

On a side note I really got spoiled by single motor.  My first board went 26 miles on a 15Ah pack.  Then I put dual motors and pneumies on it and I can barely get 12 miles out of the thing.
```

---
## \#14 Posted by: pat.speed Posted at: 2019-01-24T05:28:38.173Z Reads: 34

```
Yeah nummies suck your battery down a lot.
```

---
