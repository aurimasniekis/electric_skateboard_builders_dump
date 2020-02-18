# 12S8P 30q cells experiencing voltage sag?\[solved\] (fake cells)

### Replies: 73 Views: 1144

## \#1 Posted by: J95hicks Posted at: 2018-12-02T22:29:37.591Z Reads: 314

```
Recently made my 1st Mnt board, first ride was yesterday. Thought maybe board wasnt fully charged or i missed something, so I re-assembled and fixed some battery pack V drifting. Took it for a ride today, after maybe 2 miles on my way home(so while riding) my V meter on the board![20181201_144602|374x500](upload://kwGOfQFv2YlR1MCjLzqxUpkjxCQ.jpeg) 
 dropped to below 40 V and i could feel it losing "power" so i rode it easy home. After i got off the board i just let it sit and it came up from ~44v to ~47.5v. Am I experiencing Voltage sag on a 12s8p ??? i read about the concept of volatge sag on 12s which is why i made an 8p pack... to avoid sag. Is it my BLDC tool settings or what? Im a big guy, weigh like 270lbs, but still...what gives? ![Screenshot%20(7)|690x387](upload://167N6DInH2L0fp6f1L5cUc8MM3a.png) 


So i bought 100 cells, i found some i hadnt opened.. here are some pics. Ill let yall decide what you think ![20181203_120511|375x500](upload://sovEe2hqTGoiu1ndxQHKHyxlCCH.jpeg)![20181203_120527|375x500](upload://fVK4dpm2KQvHx8VEduqsNGTXWwc.jpeg) ![20181203_120723|375x500](upload://bOP1qQEDiwrOi2L5t6a0G7bO6k7.jpeg)  ![20181203_120744|375x500](upload://3uvuRlleTM5rLXS5id1Pnm94qYj.jpeg)
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2018-12-02T22:32:40.924Z Reads: 278

```
What cells are you using
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-12-02T22:39:34.648Z Reads: 278

```
I have massive voltage sag on my 8p but it is made of 25r cells which are nutritious for sag. As much as 30% while accelerating
```

---
## \#5 Posted by: J95hicks Posted at: 2018-12-02T22:41:48.804Z Reads: 277

```
are there any Vesc setting adjustments to combat the sag then?
```

---
## \#6 Posted by: b264 Posted at: 2018-12-02T22:52:14.804Z Reads: 275

```
[quote="J95hicks, post:5, topic:76843, full:true"]
are there any Vesc setting adjustments to combat the sag then?
[/quote]

"Maximum battery amps"
```

---
## \#7 Posted by: totalgeek9224 Posted at: 2018-12-02T22:55:40.668Z Reads: 275

```
Did you build the battery yourself? Perhaps something went wrong? (Bad p group, impure nickel/ not enough layers, poor connection) 
From what I understand you shouldn't be experiencing any sag at all with that battery.
There no chance of fake cells, is there?
```

---
## \#8 Posted by: psychotiller Posted at: 2018-12-02T22:56:44.261Z Reads: 271

```
Sounds like a bad p group.
```

---
## \#9 Posted by: J95hicks Posted at: 2018-12-02T23:01:38.089Z Reads: 264

```
Built it myself using nese modules, so  connections should be okay. There could be fake cells,, doubt it though. No dead cells, some drifting issues yesterday that i fixed https://www.electric-skateboard.builders/t/batteries-out-of-balance/76556
```

---
## \#10 Posted by: Trdolan03 Posted at: 2018-12-02T23:05:03.726Z Reads: 259

```
I also use NESE modules.
```

---
## \#11 Posted by: J95hicks Posted at: 2018-12-02T23:05:27.472Z Reads: 254

```
should i just keep decreasing maximum battery amps till the sag lessens enough that im happy? This will effect the riding behavior of the board as well im assuming, will it effect my acc or top speed though?
```

---
## \#12 Posted by: Trdolan03 Posted at: 2018-12-02T23:07:30.919Z Reads: 246

```
Acc yes. Max speed no but any sort of hills it would.
```

---
## \#13 Posted by: b264 Posted at: 2018-12-02T23:08:27.551Z Reads: 239

```
I think watching the voltage while you ride and learning how to operate the machine with less sag is better than doing that, but doing that can give you a good idea of how it feels when you're riding more efficiently, so after you turn it back up, you try to make it feel the same way most of the time .. and know when it doesn't feel that way that you're causing sag.
```

---
## \#14 Posted by: J95hicks Posted at: 2018-12-02T23:11:12.087Z Reads: 234

```
shucks, but I like going faast quickly lol... thats a good place for me to start.
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-12-02T23:15:05.187Z Reads: 230

```
Where did you buy your cells? Batt max of 25 is really low on an emtb tbh.
```

---
## \#16 Posted by: J95hicks Posted at: 2018-12-02T23:19:42.188Z Reads: 231

```
Shit, it was 30, just bumped it down to 25...but i still thought that 30 was norm for mtb. I bought from dhgate website.. forgot who specifically. researched the seller though.
```

---
## \#17 Posted by: Trdolan03 Posted at: 2018-12-02T23:21:08.214Z Reads: 221

```
I like 60 battery amps but still that is <10a per cell
```

---
## \#18 Posted by: Battosaii Posted at: 2018-12-02T23:21:18.713Z Reads: 220

```
Strange I get almost no sag, infact I rode about 5 miles on grass and I went from 50.4v to 48.8v
```

---
## \#19 Posted by: J95hicks Posted at: 2018-12-02T23:24:45.052Z Reads: 217

```
Im running unsensored sk3 149kv motors...are yall running sensored?? would that maybe be effecting things?
```

---
## \#20 Posted by: Trdolan03 Posted at: 2018-12-02T23:25:17.552Z Reads: 218

```
I currently run sk8 with one sensored and one unsenssored.
```

---
## \#21 Posted by: J95hicks Posted at: 2018-12-02T23:27:53.597Z Reads: 211

```
i was just thinking of buying one sensored motor just for startup purposes... both of your motors the same? just added a sensor? or 2 dif motors
```

---
## \#22 Posted by: Trdolan03 Posted at: 2018-12-02T23:33:43.996Z Reads: 201

```
Same motors. One of the sensors was DOA so I am one sensored and one not.
```

---
## \#23 Posted by: Benjamin899 Posted at: 2018-12-02T23:40:34.503Z Reads: 197

```
never buy batteries from sources you don't know.
```

---
## \#24 Posted by: FredrikHems Posted at: 2018-12-02T23:42:19.683Z Reads: 195

```
60a batt max is still low on a dual emtb. Guys here are running like 120a. I either think there is something wrong in the connections of the pack, or you have got some bad cells..
```

---
## \#25 Posted by: b264 Posted at: 2018-12-02T23:43:28.772Z Reads: 193

```
[quote="FredrikHems, post:15, topic:76843"]
Where did you buy your cells?
[/quote]

@J95hicks :arrow_up: :arrow_down:  

[quote="psychotiller, post:8, topic:76843, full:true"]
Sounds like a bad p group.
[/quote]
```

---
## \#26 Posted by: Trdolan03 Posted at: 2018-12-02T23:48:05.863Z Reads: 181

```
I got mine from liionwholesale.com who certify their cells. Checked all the voltages when I assembled the pack.
```

---
## \#27 Posted by: J95hicks Posted at: 2018-12-02T23:56:06.760Z Reads: 181

```
i checked all 100 cells upon arrival, they were all within .03v at the correct storage voltage. So idk, they looked good. but idk
```

---
## \#28 Posted by: Benjamin899 Posted at: 2018-12-03T00:16:23.476Z Reads: 177

```
that doesnt say much, there are enough batteries with similar capacity but way lower discharge Amps.
```

---
## \#29 Posted by: Trdolan03 Posted at: 2018-12-03T00:26:55.602Z Reads: 180

```
[quote="Benjamin899, post:28, topic:76843, full:true"]
that doesnt say much, there are enough batteries with similar capacity but way lower discharge Amps.
[/quote]
Care to explain. They are supposedly genuine 25r cells which are rated at 20a per. And at <10 they have extreme voltage sag.
```

---
## \#30 Posted by: Benjamin899 Posted at: 2018-12-03T00:37:04.369Z Reads: 176

```
that was supposed to be for @J95hicks, dunno about yours.
```

---
## \#31 Posted by: Benjamin899 Posted at: 2018-12-03T00:42:41.330Z Reads: 172

```
sorry to hear that. still hard to believe a 8p pack has extreme sag.
```

---
## \#32 Posted by: totalgeek9224 Posted at: 2018-12-03T08:33:21.610Z Reads: 161

```
What temperatures were you riding in? Perhaps the VESC throttled due to high temps?
```

---
## \#33 Posted by: totalgeek9224 Posted at: 2018-12-03T08:36:07.121Z Reads: 163

```
Yeah unfortunately this isnt how to check for fake cells. 
both capacity and discharge capabilities are what must be tested, not max v.

Maybe link us to the site/seller? perhaps we can let you know?
if not, how much did you pay per cell? sometimes (not always) that can be an indication 

Furthermore, if possible, you should try and see the temp of the cells as they are heavily discharged. If theyre 30q's and producing heavy heat at only 8-10amps- bad news for you
```

---
## \#34 Posted by: visnu777 Posted at: 2018-12-03T09:25:53.907Z Reads: 159

```
Since you are using NESE modules you can (and should) check every single cell and identify the bad ones or the bad P-packs. I had a similar problem with my tiny 10s3p and found a P pack completely dead and cells different in voltage from the others shortly after charge. I suspect it happens sometimes that the plastic cover of the cells get cut and stuck between cell and plate, causing some cells to not discharge properly. My solution for now is checking everything, chargin every single cell and when reassembling rotating them after insertion. the P pack internal resistance and overall Voltage will also be checked :)
```

---
## \#35 Posted by: rich Posted at: 2018-12-03T10:15:47.265Z Reads: 150

```
No idea what's wrong with your battery but the max battery amps are way too low. Increase it to 50-60A each vesc. Which vescs do you use?

Don't change the ABSOLUTE MAX setting! You changed it to 100A. I think the default is 130A if I remember right.

Also I would increase the batt cut off settings a bit.
```

---
## \#36 Posted by: J95hicks Posted at: 2018-12-03T16:33:47.167Z Reads: 132

```
Im in Texas, but its was like 65F yesterday when i rode. Im using dual Focbox and dual recievers. Nothing felt even warm to the touch... as the pic indicates i cant really feel or tell actually battery temp...and how would you actually test for fakes?.. it was last year i bought them, i xant remember where, i think they were $3.50 plus per cell.
```

---
## \#37 Posted by: FredrikHems Posted at: 2018-12-03T16:39:37.862Z Reads: 128

```
Am I the only one thinking that $3.5 per cell sounds a bit low? Might be wrong though.
```

---
## \#38 Posted by: Kug3lis Posted at: 2018-12-03T16:46:35.717Z Reads: 126

```
That much sag is definitely fake cells... 8P 30Q is like 120A on nominal current and 30Q are known to go up to 20A which makes it even up to 160A.
```

---
## \#39 Posted by: J95hicks Posted at: 2018-12-03T16:48:46.333Z Reads: 130

```
Yeppers, sounds like fake cells, well great lol. Guess ill just use these for awhile till theyre dead.. unless anyone wants to buy 100 who know what rating cells lol
```

---
## \#40 Posted by: Kug3lis Posted at: 2018-12-03T16:49:39.252Z Reads: 127

```
Also what about range? Because I don't think you measured each cells capacity?
```

---
## \#41 Posted by: evoheyax Posted at: 2018-12-03T16:52:55.350Z Reads: 131

```
This is why I stick to lipos personally.

If you stick to zippys from hobbyking, you won't get fakes. And voltage sag is much less than li-ion in general.

Only annoying part can be puffy cells.
```

---
## \#42 Posted by: b264 Posted at: 2018-12-03T17:11:10.728Z Reads: 130

```
You should investigate if you have a P-group not working properly before you 100% write this off as fake cells
```

---
## \#43 Posted by: J95hicks Posted at: 2018-12-03T17:20:28.495Z Reads: 130

```
Already did that, there is a tag in one of my post...  1 p group was lower by .3 v. Checked each cell in that group and none dead. Just let it balance charge for awhile now its less than .1v low from the highest p group
```

---
## \#44 Posted by: J95hicks Posted at: 2018-12-03T17:23:15.235Z Reads: 130

```
I think the range is okay. Granted ive only been on 2 rides, combined maybe 5 miles and indicator still says 100%. But i need to ride more first
```

---
## \#45 Posted by: longhairedboy Posted at: 2018-12-03T17:30:00.031Z Reads: 130

```
How exactly is the pack built? you may not have fake cells. You may just have bad connections between cells in the same p group.

If the pack is welded, check for broken welds. If you're using compression modules or somethign else, make sure everything is snug. Its possible for a shitty connection to carry charge current just fine then totally shit out on discharge. I've even seen this with bad welds.
```

---
## \#46 Posted by: Trdolan03 Posted at: 2018-12-03T17:31:40.759Z Reads: 127

```
It uses nese modules so not a bad connection
```

---
## \#47 Posted by: longhairedboy Posted at: 2018-12-03T17:39:22.217Z Reads: 125

```
i'm familiar with those, they'e compression modules. While unlikely that it is a bad connection, i would still recommend removing the cells and cleaning the contacts with a solvent like alcohol.
```

---
## \#48 Posted by: J95hicks Posted at: 2018-12-03T17:55:37.773Z Reads: 124

```
im using the nese modules. They are connected with 3/8 in thick copper flat stock and bolts, i bought new hardware to make sure i had several threads on the bolts and everything is snug
```

---
## \#49 Posted by: J95hicks Posted at: 2018-12-03T17:59:14.759Z Reads: 128

```
If i have time i suppose i could do this sometime... all 96 lol...i inspected every cell and tab before i put it all together. i highly doubt there is any contact issue
```

---
## \#50 Posted by: legend27 Posted at: 2018-12-03T18:22:57.619Z Reads: 125

```
Here is a few suggestions:
- like a lot of people said: bad p-group
- "absolute max in vesc settings" change it back to 130
- don't know if you're using bms for discharging but you should really change the battery cut off voltage end to minimum 37,2V. For the longest life span I suggest 40,8V
```

---
## \#51 Posted by: J95hicks Posted at: 2018-12-03T18:24:32.804Z Reads: 124

```
also i added picks of the cells im using at the top
```

---
## \#52 Posted by: deucesdown Posted at: 2018-12-03T18:27:59.215Z Reads: 125

```
If it's sagging crazy it should also be getting hot. If bad contact, the connetors and bus bars and cell top/bottom would get hot first. If weak cells maybe the cell bodies get hot first.
```

---
## \#53 Posted by: Andy87 Posted at: 2018-12-03T18:35:29.258Z Reads: 128

```
Read a bit in here
https://www.electric-skateboard.builders/t/samsung-30q-fake-vs-real/70695?u=andy87

There you can find some examples how to find out from the optic if it’s real or fake cells.

I can’t see it proper on the pictures you uploaded, but it looks like the second ring is missing and also the inprint on the top.
But you can check it better by your own.
```

---
## \#54 Posted by: J95hicks Posted at: 2018-12-03T18:51:35.098Z Reads: 123

```
![20181203_125009|375x500](upload://A1tRNcxgGffoLzKmMsWjbWfytTU.jpeg) ![20181203_125005|375x500](upload://94JksNXDm7m4Ec53Gq34QXhgd3W.jpeg)
  slightly better pics, but i do see what you mean by missing a ring.. i hadnt caught that.. damn
```

---
## \#55 Posted by: Benjamin899 Posted at: 2018-12-03T18:55:10.110Z Reads: 119

```
if you can, remove the wrapping, there should be markings from the plant where they are made. Fake's usually don't have them.
```

---
## \#56 Posted by: J95hicks Posted at: 2018-12-03T18:57:40.960Z Reads: 120

```
No markings......i think i got fakes guys. Well damn 
![20181203_125814|375x500](upload://2sne3Roj06Q7JTIeoKl0LHjYe8j.jpeg) 
![20181203_125800|374x500](upload://moFxgaPvlSYR4Yy8qyKEKZ9mPBo.jpeg)
```

---
## \#57 Posted by: Pedrodemio Posted at: 2018-12-03T19:05:34.405Z Reads: 118

```
Definitely fakes, can't you send them back? or do a charge back or your card?
```

---
## \#58 Posted by: Benjamin899 Posted at: 2018-12-03T19:05:59.154Z Reads: 119

```
damn brother
https://www.youtube.com/watch?v=cIAKNhPGzXw
```

---
## \#59 Posted by: J95hicks Posted at: 2018-12-03T19:06:42.616Z Reads: 121

```
i bought them like a year ago.... i highly doubt a return is possible. ill look into though
Actually got them in June, and i just tried to contact the seller
```

---
## \#60 Posted by: longhairedboy Posted at: 2018-12-03T20:56:49.946Z Reads: 119

```
i've been using liionwholesale.com and imrbatteries.com for the past 3 years with zero issues. If you end up replacing your cells, i would suggest using one of those two, but compare prices. Often one has batter prices than the other, and on any given day it could be either.
```

---
## \#61 Posted by: J95hicks Posted at: 2018-12-03T21:03:32.911Z Reads: 120

```
Was just about to buy some from thisguyhere his website esk8life.com has a sale going on. Thoughts?
```

---
## \#62 Posted by: longhairedboy Posted at: 2018-12-03T21:06:24.500Z Reads: 118

```
he likely wouldn't have a good rep here if he was going to rip you off or sell you junk.
```

---
## \#63 Posted by: J95hicks Posted at: 2018-12-03T21:07:22.273Z Reads: 114

```
Agreed lol. Just triple checking haha. Sounds good
```

---
## \#64 Posted by: thisguyhere Posted at: 2018-12-03T21:20:32.855Z Reads: 112

```
The cells i have now i got from liion wholesale, had to beg jon (owner) directly to let me get a bunch.

he probably wouldn't be too happy to find out i'm undercutting his prices so don't say nothing.
```

---
## \#65 Posted by: thisguyhere Posted at: 2018-12-03T21:23:51.148Z Reads: 112

```
i see your order, it'll be in the mail tonight.

thanks.
```

---
## \#66 Posted by: longhairedboy Posted at: 2018-12-03T21:27:12.731Z Reads: 111

```
[quote="thisguyhere, post:64, topic:76843"]
he probably wouldn’t be too happy to find out i’m undercutting his prices so don’t say nothing.
[/quote]

You mean like... for example... posting about it on a public forum? lol

you must have gotten quite a bunch. I've never ordered more than 300 cells at a time.
```

---
## \#67 Posted by: Trdolan03 Posted at: 2018-12-03T22:57:35.570Z Reads: 104

```
You could just not sell individual cells and you wouldn’t have issues.
```

---
## \#68 Posted by: Eboosted Posted at: 2018-12-04T05:47:28.368Z Reads: 102

```
It sounds like if you were hitting minimum voltage before completely shut down.

How much volts are you charging your battery to? What charger did you get?
```

---
## \#69 Posted by: linsus Posted at: 2018-12-04T11:37:06.505Z Reads: 85

```
Just do a load and capacity test to tell if theyre legit. I skimmed thru the thread, couldnt find where you bought them. Care to tell us?
```

---
## \#70 Posted by: Skunk Posted at: 2018-12-04T11:50:49.701Z Reads: 88

```
Added to the title of the thread so people wouldn't keep trying to solve the issue
```

---
## \#71 Posted by: Andy87 Posted at: 2018-12-04T12:08:12.319Z Reads: 87

```
why not only added [solved] ?
```

---
## \#72 Posted by: Skunk Posted at: 2018-12-04T12:24:26.258Z Reads: 80

```
Idk. Didn't think of it.  Really tired
```

---
## \#73 Posted by: J95hicks Posted at: 2018-12-04T19:03:49.333Z Reads: 61

```
Thx, sorry ive been busy and didnt think to do that.... but it does seem that no one ever reads the thread and just comments without looking lol
```

---
## \#74 Posted by: Andy87 Posted at: 2018-12-04T19:13:08.425Z Reads: 58

```
It’s just a lot of words already 😅 no worries thou 😜
```

---
