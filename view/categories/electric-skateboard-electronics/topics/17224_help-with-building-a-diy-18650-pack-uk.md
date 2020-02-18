# Help with building a DIY 18650 pack UK

### Replies: 50 Views: 3915

## \#1 Posted by: Freddiecook Posted at: 2017-02-05T00:27:15.820Z Reads: 294

```
So I need to get a BMS for my first build, I am really not sure what maximum discharge I need, I am going dual drive with these motors
http://alienpowersystem.com/shop/brushless-motors/alien-6355-sensored-outrunner-brushless-motor-190kv-2200w/
And using two VESCs as the ESCs, my pack which I'm building is 10s2p 
Can someone please help me
```

---
## \#2 Posted by: rpn314 Posted at: 2017-02-05T00:50:04.966Z Reads: 285

```
The BMS is meant to protect the batteries, and so I'd base the BMS rating on what batteries you're looking at. For example, if you were going to use Samsung 25R 18650 cells (I used them, they can do 20A max discharge) in your 10s2p pack, I'd probably look for a 20-30 amp BMS. Those cells are happiest at 10-15A discharge. You could get a 40 amp BMS if you want to push the cells (get more power out of them but decrease their life). Then on your VESC I'd match or go a little lower than that amp rating (divided by 2 in your case).

You could also get a 40A BMS and then set your VESCs to 30A (15A each since you have 2) so you have a little headroom all the way around.


TLDR: Base it on the batteries. For an 10s2p 18650, I'd say 40A BMS at most (depending on the cell chosen)
```

---
## \#3 Posted by: Freddiecook Posted at: 2017-02-05T13:45:36.879Z Reads: 245

```
So I'm using the Samsung ICR cells and on the spec sheet I found it said they can do 5600mA max discharge, I'm not the best at electronics so which bms would I need for that? Also when you say that it could shorten the life span of the cells, how much of a decrease are we roughly talking here?
```

---
## \#4 Posted by: smurf Posted at: 2017-02-05T14:26:10.148Z Reads: 239

```
When I drive my batteries hardcore 18 amps continuous I get like 300 cycles and then the battery life noticeably reduced to the point where I want to get new ones. If you're running 10A or less on a 20A battery you should get more like 600 charges with only %20 loss in capacity.
I'm no expert on Samsung batteries but I think you want Samsung INR18650-25R not ICR's
```

---
## \#5 Posted by: Freddiecook Posted at: 2017-02-05T14:44:13.676Z Reads: 233

```
Oh so it is quite significant then, do you have any recommendation on what bms to go for?
```

---
## \#6 Posted by: smurf Posted at: 2017-02-05T14:48:26.003Z Reads: 237

```
http://ebay.com/itm/36V-37V-42V-10S-30A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System-/321751870012

http://ebay.com/itm/Lithium-Ion-Battery-Charger-Li-ion-LiPo-10S-42V-2A-for-36V-37V-Wall-Socket-AC-DC-/321555510511
```

---
## \#7 Posted by: rpn314 Posted at: 2017-02-05T14:50:48.930Z Reads: 230

```
Well to be frank you should probably choose different cells. In my opinion 5.6 amps isn't going to be enough. Here's why:
If we don't care about lifespan and you run them at their max, with 2 in parallel you'll get 11.2 amps max. With that I'd be shocked if you got up any hills and you're acceleration and start from stops are going to be pretty lame. I don't have a good gauge for how much you'd be able to do, but your board will feel very limited.

You really want to shoot for at least a 20A available discharge rate. If you put 4 in parallel (a 10s4p in your case) then you could get 22.4 amps, which is a lot better (and enjoyable).

So considering cell life, @smurf is correct. You'll probably see double the cycle count for only going to half the battery's rated max discharge. There's other things as well, but we'll just consider discharge rate vs rated discharge for now.

If you're bent on using the INR cells and you don't care about cell life too much, I'd recommend at least a 4p setup. If you're bent on a 2p setup, you need a different cell.
```

---
## \#8 Posted by: Freddiecook Posted at: 2017-02-05T15:50:27.148Z Reads: 211

```
Okay, this makes sense, when I bought the cells I had a very limited knowledge in cells and wasn't sure which ones to get, the reason I bought these were because they were brand new and cheap on ebay (not fake either) I'm of course trying to keep this pack as cheap as I can but still getting good performance, When I get home I'll see if I can buy any more for a reasonable price but if not, what cells could you recommend which aren't too on the pricy side?
I'm flexible on changing the set up as well, I just don't want it to bankrupt me
```

---
## \#9 Posted by: smurf Posted at: 2017-02-05T17:25:23.605Z Reads: 214

```
https://liionwholesale.com/collections/batteries/products/lg-he2-18650-battery-genuine-tested-20a-2500mah-flat-top-wholesale-lot?variant=1038173256

https://liionwholesale.com/collections/batteries/products/samsung-inr18650-25r-battery-genuine-tested-20a-2500mah-flat-top-wholesale-lot?variant=1038201992

https://liionwholesale.com/collections/batteries/products/sony-18650-vtc4-battery-genuine-tested-30a-2100mah-flat-top-wholesale?variant=1038136780

The Sony's would be good for 2P

PS someone around here might have a discount code or something
```

---
## \#10 Posted by: Freddiecook Posted at: 2017-02-05T19:23:19.374Z Reads: 194

```
thanks man, I'm going to be really difficult here and mention that I'm in the UK so if you know any UK dealers then that would help and which do you think would give me the best bang for my buck taking into account the pack setup, really appreciate this
```

---
## \#11 Posted by: lox897 Posted at: 2017-02-05T20:01:30.257Z Reads: 184

```
Nkon.nl is in Europe
```

---
## \#12 Posted by: smurf Posted at: 2017-02-05T21:12:31.430Z Reads: 179

```
As one answer naturally segues into the next question maybe start a build thread or just rename this one.
```

---
## \#13 Posted by: Freddiecook Posted at: 2017-02-05T22:02:25.868Z Reads: 174

```
Good point, I'll do that now 
The main thing which is currently confusing me is how do I determine what battery I need? How do I determine what my system is drawing and match that with a suitable set of cells? I mean I'm looking at pages of these 18650s and after a while they all look the same lol, what makes one more expensive than the other?
```

---
## \#14 Posted by: smurf Posted at: 2017-02-05T22:33:52.500Z Reads: 161

```
1 motor or 2?  hills or flat land ? How much do you weigh? How many kilometers range? What's the budget?
```

---
## \#15 Posted by: Freddiecook Posted at: 2017-02-05T22:58:57.600Z Reads: 155

```
2 motors, mostly flat, 72kg, I am willing to spend about £120 on the cells, with regards to range, the more the better at this point, it wont be used for commuting so I don't need a huge range
```

---
## \#16 Posted by: smurf Posted at: 2017-02-05T23:06:34.792Z Reads: 151

```
How about 10S3P Samsung 25Rs (30@€3.2 each
https://eu.nkon.nl/samsung-18650-inr18650-25r.html
```

---
## \#17 Posted by: Freddiecook Posted at: 2017-02-05T23:36:47.738Z Reads: 151

```
What makes them a good cell? Sorry for my lack of knowledge, I just want to know what makes them better than others?
```

---
## \#18 Posted by: smurf Posted at: 2017-02-06T01:26:33.365Z Reads: 151

```
http://www.electric-skateboard.builders/t/choosing-18650-cells/6240?u=smurf
```

---
## \#19 Posted by: Namasaki Posted at: 2017-02-06T04:27:11.861Z Reads: 151

```
[quote="Freddiecook, post:3, topic:17224"]
So I'm using the Samsung ICR cells and on the spec sheet I found it said they can do 5600mA max discharge,
[/quote]

That's only 5.6 amps. That's not gonna cut it for an E-board.
The minimum usable 18650's would be 20a discharge and you would need 30 of those for a 10s3p
Imo, a battery with 60a discharge is the bare minimum and even with that your probably gonna have plenty of voltage sag.
```

---
## \#20 Posted by: Freddiecook Posted at: 2017-02-06T12:35:00.960Z Reads: 149

```
Okay so should I aim for a little higher than 60A just to give it some headroom to counter the voltage sag? Maybe 10s4p? Or go for a higher discharge cell I guess
```

---
## \#21 Posted by: Tuomalar Posted at: 2017-02-06T12:56:37.774Z Reads: 142

```
Most common batteries in esk8s are 10s3p, 10s4p and 12s3p and maybe 12s4p with lower kv motors.
```

---
## \#22 Posted by: Namasaki Posted at: 2017-02-06T16:11:57.353Z Reads: 138

```
Higher is always better. 
I use a 10s pack that consists of 5.0ah/60-120c Lipos 
And it supposedly can handle 300a cont to 600a peak. 
Running dual 190kv motors with Vescs set at 60a motor max and 50a battery max each. 15/36 gears and 83mm wheels. 
And I still get some voltage sag when driving hard up a 10% grade. But it's only 1v from total pack voltage.
```

---
## \#23 Posted by: Freddiecook Posted at: 2017-02-20T17:23:42.199Z Reads: 120

```
So I've done a bit more research in my spare time and found what I think look like good cells, I found that I should find my idea voltage by doing 8600/170 (my motor KV) and found that I should be packing about 50V which points towards me upgrading to 12S (if I'm correct), I am now wondering if it is worth going for a higher discharge cell (about 30A) and sacrificing some capacity (having 500mah less) or is it worth going for a lower discharge (20A) and keeping capacity higher (3000mah)
```

---
## \#24 Posted by: Maxid Posted at: 2017-02-20T17:40:27.096Z Reads: 116

```
Where does the 8600 come from?
```

---
## \#25 Posted by: Namasaki Posted at: 2017-02-20T18:42:38.303Z Reads: 118

```
What you need is at least 5000mah and 30c. 
That should give you abt 12 mile range with 12s
5000 mah and 60c would be better.
```

---
## \#26 Posted by: Freddiecook Posted at: 2017-02-20T18:44:47.958Z Reads: 122

```
http://www.electric-skateboard.builders/t/10s-12s-custom-battery-pack-options/1789/19?u=freddiecook
```

---
## \#27 Posted by: Freddiecook Posted at: 2017-02-20T18:52:19.440Z Reads: 120

```
How are you working out the C rating for the cells, these are the two main cells I'm looking at at the moment
1. http://www.gearbest.com/batteries/pp_399870.html 
2. http://www.gearbest.com/batteries/pp_399862.html
```

---
## \#28 Posted by: Namasaki Posted at: 2017-02-20T19:07:23.998Z Reads: 113

```
Thought you wher talking about Lipos
```

---
## \#29 Posted by: Freddiecook Posted at: 2017-02-20T19:37:32.124Z Reads: 108

```
oh sorry no I'm on about making an 18650 battery pack
```

---
## \#30 Posted by: Namasaki Posted at: 2017-02-20T20:07:10.093Z Reads: 108

```
I think Samsung or LG are the go to cells. 
Not sure I would trust imr
```

---
## \#31 Posted by: Maxid Posted at: 2017-02-20T20:18:11.752Z Reads: 106

```
This should be taken with a grain of salt though: it only applies to motors with 14 poles. There are hub motors out there with 28 poles for example. Also 10S is the sweet spot for the VESC - higher is pushing it and only recommended if you absolutely need the added speed.
```

---
## \#32 Posted by: Freddiecook Posted at: 2017-02-20T21:06:49.505Z Reads: 100

```
Okay I'll stick to the 10s then I'm just not sure how many of the cells to put in parallel and of which cell
```

---
## \#33 Posted by: Freddiecook Posted at: 2017-02-20T21:07:31.072Z Reads: 92

```
what's your opinion on what cell to go for in this instant then?
```

---
## \#34 Posted by: Namasaki Posted at: 2017-02-20T21:10:23.506Z Reads: 95

```
Well, the imr is claiming 30a but I find that hard to believe. I would search for reviews before buying that one. They could easily be over rating it. Or they might mean 30a peak.
```

---
## \#35 Posted by: Maxid Posted at: 2017-02-20T21:27:05.112Z Reads: 89

```
If I had to build a pack again I'd go for samsung 30Q cells. Preferably in a 10S4P configuration.
```

---
## \#36 Posted by: fedestanco Posted at: 2017-02-20T21:41:37.058Z Reads: 94

```
@Maxid 
Is there any reason, apart from the price, why Samsung 30q became the preferred cells in this forum? Don't the LG hg2 cells offer the same (or better) performance?
```

---
## \#37 Posted by: Maxid Posted at: 2017-02-20T22:57:33.725Z Reads: 94

```
They perform almost as good as hg2 but at a lower price. High capacity and high current capabilities combined with very little voltage sag compared to for example 25Rs. (I am using 25Rs and regret not getting the 30Q because of voltage sag)
Just compare 25Rs or HG2s with the 30Q on this site: http://lygte-info.dk/review/batteries2012/Common18650comparator.php
```

---
## \#38 Posted by: Freddiecook Posted at: 2017-02-20T23:47:26.504Z Reads: 92

```
I have found that the 30Q cells are only £1.50 cheaper than the hg2 cells (as the hg2 are on sale) I'm leaning more towards the hg2 at this point but have never used them before, are they worth it do you know?
```

---
## \#39 Posted by: Maxid Posted at: 2017-02-20T23:48:00.543Z Reads: 92

```
If you don't care about the money go for HG2. But 1.5 at 40cells is 60pounds
```

---
## \#40 Posted by: Freddiecook Posted at: 2017-02-20T23:51:15.995Z Reads: 92

```
sorry I meant for a pack of 8 as in a pack of 8 hg2 is £1.50 more than a pack of 8x 30q
```

---
## \#41 Posted by: Maxid Posted at: 2017-02-21T00:01:44.394Z Reads: 91

```
I see a 44€ difference with 40 cells
<img src="/uploads/db1493/original/3X/b/0/b0bf1fd2cbffd20cf7150012f0dfe3895f12d351.png" width="281" height="500">
```

---
## \#42 Posted by: Freddiecook Posted at: 2017-02-21T00:21:25.686Z Reads: 90

```
Oh I'm looking on a different website 
http://www.gearbest.com/batteries/pp_399870.html
http://www.gearbest.com/batteries/pp_399866.html?wid=21
```

---
## \#43 Posted by: Maxid Posted at: 2017-02-21T00:23:37.664Z Reads: 88

```
Get them from a trusted source like nkon and not gearbest.
```

---
## \#44 Posted by: Freddiecook Posted at: 2017-02-21T00:27:39.826Z Reads: 88

```
I'll have a little shop around, are gearbest not a good supplier then?
```

---
## \#45 Posted by: Maxid Posted at: 2017-02-21T00:29:53.493Z Reads: 91

```
They'll send from china so you will have to pay VAT on arrival - poof there goes your saving. Plus the added time and unknown sources. Nkon is THE source for european stock batteries. You will not find a cheaper source.
```

---
## \#46 Posted by: Freddiecook Posted at: 2017-02-21T00:45:18.471Z Reads: 88

```
okay nkon it is, thanks
```

---
## \#47 Posted by: AJesk8 Posted at: 2017-12-24T17:28:03.559Z Reads: 62

```
What is voltage sag? Thanks
```

---
## \#48 Posted by: Namasaki Posted at: 2017-12-24T20:07:28.024Z Reads: 62

```
When you pull current from the battery, it's output voltage drops. This is called voltage sag.
The closer the current you pull is to the max discharge rate of the battery, the more it will sag.
This is why we say build more battery than you think you need. The bigger the better.

If you think your gonna need 40a then build a battery than can handle 80a or better yet, 120a

Excessive voltage sag will rob you of power and range.
```

---
## \#49 Posted by: AJesk8 Posted at: 2017-12-24T21:36:29.928Z Reads: 66

```
i only weigh 63kg so should a 10s3p 25r pack be good enough for me even if i put on a bit of weight or what about a 10s2p https://eu.nkon.nl/rechargeable/18650-size/sony-us18650vtc6.html            - vtc6 ?
```

---
## \#50 Posted by: Namasaki Posted at: 2017-12-24T21:59:10.202Z Reads: 65

```
I have never used 25R's but have heard of them sagging.
Seems like everyone is using Samsung's 30Q's these days and they are gaining good reputation.
```

---
