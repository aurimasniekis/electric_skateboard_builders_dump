# Battery questions

### Replies: 38 Views: 2706

## \#1 Posted by: KTMinni Posted at: 2017-03-07T22:31:14.633Z Reads: 236

```
Hi so I'm planning on making a battery out of LG HG2 18650 cells.  These particular cells are 3000mAh and rated at 20A and if I wired 15 of them in a 5S3P would it be correct in saying each pseudo "cell" would effectively be 9000mAh? Furthermore would that make this pack, 9000mAh @ 18V nominal?
```

---
## \#2 Posted by: mccloed Posted at: 2017-03-07T22:39:37.644Z Reads: 236

```
Correct. Each cell would be 9000mah at 3.6v nominal. Your max continuous would be 60a. Are you going to run two in series? 5S is not much for an ESK8.
```

---
## \#3 Posted by: spaso Posted at: 2017-03-07T22:44:23.968Z Reads: 231

```
I agree, 5s is very little.  If you can, I would recommend buying 5 more cells and making a 10s2p battery.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-07T23:06:10.782Z Reads: 221

```
Just to confer. 5s is not enough for eskate. 
6s is the minimum and doesn't provide much torque.
```

---
## \#5 Posted by: michaelcpg Posted at: 2017-03-07T23:06:58.975Z Reads: 209

```
Also something worth mentioning is that even though the cells are rated at 20A continuous, don't plan around a battery design that relies on drawing even close to a cells rated discharge current for long periods of time regularly as you'll end up generating a lot of heat, get less range out of your battery per cycle and degrade the cell life more quickly. 

I think a lot of people here use batteries that generally draw closer to half theirs cells rated current or less most of the time. Obviously if you live somewhere very flat then its not as much of an issue as if you riding up hills regularly. 

If cost is a limiting factor, have a look at Samsung 25R or LG HE4 cells, they're usually a reasonable amount cheaper so you should be able to get a few more cells for the same price and would likely give you very similar per cell range to the larger capacity of the HG2 cells when setup in such a small pack anyway.
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2017-03-08T02:13:35.622Z Reads: 188

```
hey....I've tried 4s before...feels like yuneec-ego

so...5s will work....just ride flats and small inclines and you'll be fine
```

---
## \#7 Posted by: KTMinni Posted at: 2017-03-08T04:14:48.431Z Reads: 180

```
Yeah, the 15 cells was an example, I was thinking maybe 16 and do 8S2P or like what michaelcpg said, get the 25R or HE2 and get more for the same price.
```

---
## \#8 Posted by: benwong Posted at: 2017-03-08T04:24:25.479Z Reads: 180

```
how to determine how many pack i need for my setup? 
base on motor AMP or ?
```

---
## \#9 Posted by: Hummie Posted at: 2017-03-08T04:25:08.471Z Reads: 180

```
or you could just up the amp limits on the esc if you can.  compensate for less voltage with amperage
```

---
## \#10 Posted by: PXSS Posted at: 2017-03-08T04:30:54.919Z Reads: 174

```
Do not get 25Rs or HE2. 
Go with 30Q from nkon, they're just as good as hg2s but way cheaper
```

---
## \#11 Posted by: michaelcpg Posted at: 2017-03-08T06:43:01.871Z Reads: 167

```
30Q have an even lower discharge rating than the other cells which could be an issue with such a small pack. In saying that, I haven't personally seen any data comparing their discharge curves to other cells. 

They're still more expensive than 25Rs by a reasonable amount as well. They certainly look like great cells for larger packs though.
```

---
## \#12 Posted by: jrpwit Posted at: 2017-03-08T10:01:05.437Z Reads: 161

```
Umm no... Don't go with 30Q cells. Only 15 amp continuous and quite a bit more expensive then 25r. 25r is the best cell for the money 20 amp and cheapest compared to other similar cells. Lg hg2 are a bit more expensive but have 500 mAh more capacity. Lg hg2 cells the same price as 30Q so there is no point in getting 30Q.
```

---
## \#13 Posted by: Maxid Posted at: 2017-03-08T10:55:46.009Z Reads: 165

```
ratings mean shit - look at actual discharge curves.
30Q can withstand far more than 15A and have less voltage sag.
They might heat up more than the 25R but you are not going to use the full 15A per cell for extended periods of time.

See:
http://lygte-info.dk/review/batteries2012/Common18650comparator.php
```

---
## \#15 Posted by: KTMinni Posted at: 2017-03-08T12:42:22.666Z Reads: 159

```
I went ahead and bought 20 LG HE2 18650s and will configure them in a 10S2P config
```

---
## \#16 Posted by: PXSS Posted at: 2017-03-08T17:31:52.297Z Reads: 155

```
@Okami, @radium
Back me up here... I'm tired of repeating myself...

Do some research. If you just want to be spoon fed answers and follow what people say blindly, you're going to end up with a mediocre board. 

Both @michaelcpg and @jrpwit are wrong, no offense to you two. But it's my daytime job to know battery technology like the back of my hand. I've posted in several threads why the 30Qs are much better than 25Rs, backed up with actual test data and not just numbers from a table I saw somewhere. Have you guys even looked at the actual data sheets??? Do you know where the 15A limit on the Samsung 30Q comes from? It's got nothing to do with power and more to do with number of cycles you get out of the cell if you push 20+A CONTINUOUSLY through them. Samsung actually tests these up to 25A. Look up the spec sheet, inform yourselves...
```

---
## \#17 Posted by: michaelcpg Posted at: 2017-03-08T21:01:25.444Z Reads: 142

```
No need to get worked up about it man. 

I specifically said in my previous comment that I hadn't looked at any data comparing the discharge curves and was purely basing what I said off the manufacturer provided ratings which I know don't give the full story.

If the 30Q's are comparable to 25R's then that's awesome.
```

---
## \#18 Posted by: michaelcpg Posted at: 2017-03-08T21:04:53.095Z Reads: 139

```
Cheers for the link :)
```

---
## \#19 Posted by: PXSS Posted at: 2017-03-08T22:12:25.668Z Reads: 140

```
Not comparable... Better, much better
```

---
## \#20 Posted by: radium Posted at: 2017-03-09T05:02:22.364Z Reads: 140

```
I'll back you up. The 25r is an ok battery, but it's going to sag more than the 30q and have less capacity overall. If you look on ecig forum you can find information directly comparing the two at a 20A continuous discharge.
```

---
## \#21 Posted by: Gromok Posted at: 2017-03-09T08:21:58.106Z Reads: 134

```
I have been looking at the VTC6 and thinking about buying 65 of them soon for a 10s6p pack. The extra 5 is in case there is a couple sub par batteries in the box.

Since you say it is your day job to know about batteries, are the VTC6 better then the 30Q's? From what I read, VTC6 is the best li-ion 18650 at the moment.
```

---
## \#22 Posted by: smurf Posted at: 2017-03-09T09:25:05.708Z Reads: 130

```
How are you going to find out which 5 are sub par?
```

---
## \#23 Posted by: Gromok Posted at: 2017-03-09T09:45:03.518Z Reads: 132

```
No idea, but I do not have an ABN (Australian business number) so the company that is willing make the packs cannot purchase the batteries for me. Just wanted a few extra's in case there is issues with one or two instead of being stuck at not being able to have the pack done.

Also if that is not necessary, then I will just use the five of them as spare rechargeable batteries for whatever!

Was going to wait till VESC 6 and JTAG's BMS goes gold, but I'm already fed up with Evolve's voltage sagging on hills and short range, so gonna bite the bullet and do my DIY by the end of the month, hence asking about VTC6.
```

---
## \#24 Posted by: smurf Posted at: 2017-03-09T10:08:00.107Z Reads: 127

```
I'm doing about the same thing. After doing way too much battery research I ended up going with the cheapest 20 amp battery I could get he2 and getting enough for a 10S8P
```

---
## \#25 Posted by: PXSS Posted at: 2017-03-09T12:38:34.204Z Reads: 124

```
VTC6 is the best power cell out there. There's about 5-10% improvement over 30Q. If you have an rc charger that can measure internal resistance then that would be the way to match them. You want the spread to be as little as possible and on the lower side. The low spread will determine how balanced your cells remain over their life, and the low ir will make them sag less.

If you want to spend less then buy 30Q from nkon. I bought 70 for $230 including shipping ($3.30 per cell). It's significantly cheaper than VTC6 which cost $5-6 per cell (in the us at least). 

I only use VTC6 when cost is a non issue and I want the absolute best power output. Otherwise I use 30Q for marginally worse power output but a lot less $$$. 
If you want a high range pack then Sanyo GA is the cell you want, again a little pricey $5-6 a cell but it has 16% more capacity than 30Q and VTC6 and has a power output that's just as good as 25R cells. Which is about half as much as VTC6 and 30Q unless you let it sag significantly. 

I currently have 2 battery packs, one out of 30Qs and one out of GA cells. My gf usually rides the GA pack as she wants long range and doesn't really do high speeds or crazy hills on her way to school, while I like to ride the 30Q because of the sheer power it can output.
```

---
## \#26 Posted by: Gromok Posted at: 2017-03-09T13:12:46.434Z Reads: 123

```
Thanks for your reply. 

Pretty much what I thought, although it is the first that I have heard of Sanyo GA. ( Is that the Tesla battery? )

Sag is what I want to kill off. Range should be acceptable in six parallel.
```

---
## \#27 Posted by: Gromok Posted at: 2017-03-09T13:14:27.277Z Reads: 123

```
80 cells? What board are you using? I'm thinking you are going AT, right?
```

---
## \#28 Posted by: PXSS Posted at: 2017-03-09T14:32:50.793Z Reads: 124

```
@Gromok, Yep, it is the updated version of the Panasonic B cell which is the Tesla cell.
@smurf, what was the purpose of your large pack? Sorry to be a party pooper but I'm afraid you could have gotten 66 30Q cells for the same range and more power output than HE2 cells.

<img src="/uploads/db1493/original/3X/0/6/060f3b7501b32eb44a1312b05f939a8843fbede9.png" width="690" height="383">
Voltage sag for 30Q vs HE2.
outputting 15A per cell, the 30Q sags as much as the HE2 outputting 7A past the 1Ah mark. Outputting 7A with the 30Q has slightly more voltage sag than the HE2 at 0.2A...
A 10S8P HE2 would have a total of 720Wh, while a 11S6P would have 712Wh, when you adjust for sag, the HE2 has 641Wh when outputting 7A/cell and the 30Q has 617Wh at 15A/cell.

Also you can buy 30Qs for $2.75ea + shipping from Nkon
```

---
## \#29 Posted by: TheImmortalJew Posted at: 2017-03-09T14:47:43.580Z Reads: 114

```
@PXSS Are you in the US or Europe? I'm looking at ordering some 30Q from Nkon and wondering what the shipping time is like to the US. They say at least 2 weeks.
```

---
## \#30 Posted by: PXSS Posted at: 2017-03-09T15:07:46.761Z Reads: 114

```
@TheImmortalJew I'm in the US. I gotta check my email for how long they took, but I want to say it was 2 weeks from ordering to my doorstep, maybe 3.
```

---
## \#31 Posted by: smurf Posted at: 2017-03-09T19:11:29.412Z Reads: 113

```
Rough asphalt and big hills. This is where crazy people go to build crazy electric skateboards right.
@PXSS at the time Samsung anything was substantially higher in price. Black Friday sale
```

---
## \#32 Posted by: PXSS Posted at: 2017-03-09T19:22:49.350Z Reads: 112

```
I'm guessing Liion wholesale? I wish I had bought more stuff on their Black Friday sale. :P
```

---
## \#33 Posted by: smurf Posted at: 2017-03-09T19:31:19.905Z Reads: 112

```
https://www.instagram.com/p/BNsF7f-jUHH/

I got a great deal on a handful of protected cells for flashlights and I almost went nuts and got the Sony's with the special sauce but there so expensive. I wish money wasn't a factor but in the real world it is.

The real question is still Unanswered. so you get a few extra battery's how do you sort out the good from the less than ideal batteries?
```

---
## \#34 Posted by: longhairedboy Posted at: 2017-03-09T19:39:07.384Z Reads: 106

```
i'm still using Samsung INR18650-25R cells. 20amp continuous, 2500mAh, 100amp burst. They're older tech, but they take a fair amount of abuse. I've even been able to tear off tabs  and re-weld them without an issue. We just repacked 60 of them from two different older series space cells into a 12S5P triangular cell layout for shits and giggles and it is behaving as expected. Better, actually, as we sort of thought those original packs were nearing cycle life.
```

---
## \#35 Posted by: PXSS Posted at: 2017-03-09T20:08:42.426Z Reads: 105

```
@smurf I answered that above. 
[quote="PXSS, post:25, topic:18712"]
If you have an rc charger that can measure internal resistance then that would be the way to match them. You want the spread to be as little as possible and on the lower side. The low spread will determine how balanced your cells remain over their life, and the low ir will make them sag less.
[/quote]
```

---
## \#36 Posted by: longhairedboy Posted at: 2017-03-09T20:23:23.164Z Reads: 101

```
@smurf also, there's this:
http://www.all-battery.com/TenergyIntelligentCellMeter-01444.aspx?utm_source=GoogleShopping&utm_medium=GDF&gdffi=fb520bc42d4e46cbab702234d35f7d38&gdfms=CC42B2303B634D3A8A6391EA98B28E6E&gclid=CNXQ_IygytICFUZEhgodAG0Ojw 

and i'm sure several other products that are similar.
```

---
## \#37 Posted by: smurf Posted at: 2017-03-09T20:41:35.944Z Reads: 97

```
Do you test every cell or do you just trust them?
```

---
## \#38 Posted by: PXSS Posted at: 2017-03-09T21:53:14.356Z Reads: 100

```
I test them,
I have 4 icharger 308 duos, which have 2 channels with up to 8S balance port.
http://www.progressiverc.com/icharger-308duo.html

I wired 2 of these in series to form 8S battery holders:
https://www.amazon.com/Battery-Case-Holder-4x3-7V-18650/dp/B01FSDKXRI/ref=sr_1_2?ie=UTF8&qid=1489095715&sr=8-2&keywords=18650+battery+holder+4

So I can test up to 16 cells per charger at a time.
The charger has a test internal resistance feature that runs in about 10 seconds and tells me the internal resistance of each individual cell. I then group the cells from lowest to highest IR, and try to choose the ones that are closest to each other. I rather choose cells that are in the middle of the IR range but that have a smaller spread as this means I have to worry less about them going out of balance. Eventually, we get enough cells in inventory to do a pack with a low spread and low internal resistance. These packs are usually reserved for high profile projects while the high internal resistance packs I usually only use for bench testing.

---
That said I've never had any cells that were out of spec according to the manufacturers datasheet
```

---
## \#39 Posted by: jrpwit Posted at: 2017-03-10T02:40:48.277Z Reads: 90

```
Huh I have never looked into the actual data. Thanks for the link really appreciate it. Wish I had known this before I build my pack.
```

---
