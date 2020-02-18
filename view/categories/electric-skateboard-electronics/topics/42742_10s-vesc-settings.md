# 10s VESC Settings

### Replies: 13 Views: 2372

## \#1 Posted by: pengy Posted at: 2018-01-04T12:28:03.467Z Reads: 267

```
Hey I was wondering if there is a way to see a screenshot of a 10s configuration for the VESC
Or a step through guide.

Thanks.
```

---
## \#2 Posted by: PartyPoison Posted at: 2018-01-04T12:46:05.385Z Reads: 266

```
http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#3 Posted by: pengy Posted at: 2018-01-04T12:51:40.254Z Reads: 257

```
Thanks, there is a really nice YouTube video, and it all makes since.
Was just thinking perhaps there is a ready made configurations but I on the other hand after watching this video, I came to realize it might be a user preference as well. As some prefer to push it more or less to the limit and also tweaking the regen breaking etc. So I'll give it a go. Super nervous about assembling it all.
```

---
## \#4 Posted by: mmaner Posted at: 2018-01-04T14:17:14.004Z Reads: 254

```
Here are the setting from VESC #1 of my Evo dual setup.  This should give you an idea of what to look for, but make sure you do motor detection in BLDC and FOC (if you are going to run FOC or Hybrid mode).

<img src="/uploads/db1493/original/3X/0/4/0472c8eb94c3f5de2619de955a752cb89f6b3d1a.PNG" width="690" height="412">
<img src="/uploads/db1493/original/3X/8/4/844429113b80da6b99c60144044768bdca521596.PNG" width="690" height="412">
<img src="/uploads/db1493/original/3X/e/d/ed71ac9cc514e670b5e572e0ae825a7ad4e231a4.PNG" width="690" height="412">
<img src="/uploads/db1493/original/3X/6/7/67eb910b9254b9df3f3fb8781b0fa24c06f7ba4e.PNG" width="690" height="412">
<img src="/uploads/db1493/original/3X/b/b/bbac4d591304961ae8abaa60a3aca1dba7564b39.PNG" width="690" height="412">
```

---
## \#5 Posted by: Deckoz Posted at: 2018-01-04T15:46:54.242Z Reads: 220

```
What MManner said however

I would start yourself off with 30-40 motor amps if you have duals and it's your first board

And the cut off start and end I don't agree with

Liion drop off after 3.35/cell
Lipo drop off at 3.65/cell

Liion
Cuttoff start 34.5
Cutoff end 33.0

Lipo cutoff start
36.75
36.00

These will allow for some sag - while allowing your rested voltage to be right at the point where the batteries drop off in discharge current and keep your packs healthy.

If you have a large parallel group(ie 5p+) you can likely get away with discharging LIION packs to a lower voltage without damaging the cells by not having a high current draws at the cell level. 

Ie
1p 36v end
2p 34.75v end
3p 33.5v end
4p 32.25v
5p 30.75v
6p+ down to 29v~

That's just relative to about how much current your pulling to keep the packs cool, and not over discharged relative to the current required at any given riding point.

Also if it's below 30F, I wouldn't advise discharging past 3.35/cell as the cold increases internal resistance which makes the cells heat quickly during high amp discharge and give off less amps over time.. slowly damaging the packs
```

---
## \#6 Posted by: pengy Posted at: 2018-01-05T11:08:23.967Z Reads: 201

```
This is a very useful information. 
I have a single motor which is kinda huge 6470 I think..
So to do both motor checks BLDC and FOC right?
I'm going to run 10S 2P of high quality 18650s so the recommendation of 2p 34.75v battery cutoff meaning 3.47 for each cell sounds good.
```

---
## \#7 Posted by: michaelcpg Posted at: 2018-01-05T11:37:04.411Z Reads: 192

```
You should probably looking at using a larger battery. You're really going to be pushing a 10S2P pack to it's limits with a motor that size.
```

---
## \#8 Posted by: pengy Posted at: 2018-01-05T11:44:47.969Z Reads: 182

```
Yeah but at that point I prefer that on going 6s 3p and pretty sure I'm going to not push that motor to its limits, just a comfortable cruiser..
```

---
## \#9 Posted by: michaelcpg Posted at: 2018-01-05T11:54:29.752Z Reads: 179

```
Cells are cheap, if you're building an 18650 pack, save a bit more money and go 3P, if not 4P. You'll get a lot more charge cycles out of your battery, have more power available and be less likely to have issues with your board due to sag etc. Just my opinion

https://ru.nkon.nl/samsung-inr-18650-30q-3000mah.html
```

---
## \#10 Posted by: pengy Posted at: 2018-01-05T12:14:24.367Z Reads: 179

```
That's a good recommendation and price for a great cell, gonna keep that link for future projects. My LG cost almost double than that.. with the same mah.. I think the discharge is higher a bit on my LG but that doesn't really differ..

For me it's more about shipping time, with an order like that i'm expected to wait a long long time for it to arrive to my country..

I get the sense of why reducing the cycle improves the longevity of the cells but confused as why a 3p for example would be better than 2p since the same wattage is drawn anyways.
```

---
## \#11 Posted by: michaelcpg Posted at: 2018-01-05T12:26:16.368Z Reads: 173

```
Drawing higher current from a cell increases the temperature (the difference can be quite dramatic with smaller batteries) which has a big impact on the life of the cells. Also keep in mind that that its not a great idea to just go off the manufacturer's current rating each cell as these values are usual pretty generalized.

I'm assuming you're using LG HG2 cells so here's a comparison of the LG to the Samsung cell :slight_smile:

<img src="/uploads/db1493/original/3X/7/7/77446892c093dff0c70308beb50ec007850d5661.jpg" width="690" height="341"><img src="/uploads/db1493/original/3X/a/2/a292c73b544bcef74595ed12c7910b7363301c43.jpeg" width="690" height="341">

The LG HG2 are still nice cells but as you can see, they get hotter than the 30Q when being discharged around 15-20A even though they have a higher manufacturer current rating.

From what I've seen, you don't really want your cells getting much hotter than 70C unless you're willing to give up a fair bit of cycle life for the cells which is why (depending on how you use your board) going 3P or even 4P could help to reduce the temperature of your cells and increase the life/power of the battery in general
```

---
## \#12 Posted by: pengy Posted at: 2018-01-05T12:38:30.062Z Reads: 154

```
Nice! So I have no realistic idea yet of how many watts I should aim to draw considering the speed acceleration and my weight..
But I think 800watts meaning 19amps drawn from 42 volts sounds good considering? Or you think it's better to reduce it.
```

---
## \#13 Posted by: michaelcpg Posted at: 2018-01-06T04:14:01.451Z Reads: 143

```
You should calculate using the nominal voltage (36V) to get a more realistic value. 

How much current you can expect to draw can vary a lot but you probably don't want to set your battery max to the equivalent of any more than 10-15A per cell, so 20 - 30A at most for 2P with those cells. 

As a comparison, I have mine set to 54A battery max (27A per VESC) on my board which is using a pair of smaller 5060 motors with a 6P pack. I don't do much crazy acceleration but I live in a fairly hilly city which requires more power. 
I also used to have a board with a single 6374 motor and a 10S4P pack and I had my battery max set to 40A.
```

---
