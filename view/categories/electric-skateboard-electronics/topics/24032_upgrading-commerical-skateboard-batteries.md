# Upgrading Commerical Skateboard Batteries

### Replies: 19 Views: 1402

## \#1 Posted by: Steamboat_Rock Posted at: 2017-05-28T01:40:49.024Z Reads: 212

```
Hello, in advance I really appreciate any assistance I receive! Over the past month I have been researching building my own electric skateboard from scratch and have been quite intimidated haha. As a side project to help build my confidence, I've decided to do some upgrades on my two existing store-bought electric skateboards first before I take on building one from scratch. 

At the moment I am working on my MotoTec 1600W skateboard (http://www.bigtoysusa.com/mototec1600welectricskateboard.aspx). When originally purchased I could make a 10mile+ trip without recharge, while now I am barely getting 3 miles. The batteries this thing came with are MASSIVE and heavy. Here is a photo of the batteries and the available space (about a foot) 
<img src="/uploads/db1493/original/3X/c/1/c14e2ec441625ff2ff78e119f82d71be116c623e.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/6/1/6149127fc86a886501ed548411c9eb7ab46b8365.jpg" width="690" height="388">

The batteries themselves have basically zero labeling. I have narrowed them down to Kijo batteries, so from china (http://kijobattery.manufacturer.globalsources.com/si/6008848464288/Showroom/3000000149681/ALL/16.htm). Although exact voltage and amperage are unknown. According to website of purchase (which could be incorrect) the batteries in series total 36V 14AH.  

I am looking to replace the batteries with some smaller, lighter, and possibly more powerful (good idea?) to get additional speed. 

I am looking at a couple of different options, please let me know if these will work:
https://hobbyking.com/en_us/zippy-compact-4000mah-10s-25c-lipo-pack.html 
or two of the below run in parallel
https://hobbyking.com/en_us/turnigy-nano-tech-4500mah-4s-35-70c-lipo-pack.html 
or these run in parallel
https://hobbyking.com/en_us/turnigy-nano-tech-4500mah-4s-25-50c-lipo-pack.html

Would these different batteries work? 
Is there a way to estimate the miles between charge these new batteries could make compared to existing batteries? Lastly, would I be able to use the existing charger to charge these?

Thank you!
```

---
## \#2 Posted by: Lambjr088 Posted at: 2017-05-28T02:40:06.915Z Reads: 176

```
Are you looking to have the same amps as before or are you willing to have less? If so i would recommend 3 of the 10s packs or 4 connected in parallel. If you get the 4s packs you would have more volts but less amps and that would probably shorter distance unless you mod the belts and pulley which would cost more. Of course i see you have a lot of space. I would use 18650 batteries but they are more expensive, still they are the best in my opinion
```

---
## \#3 Posted by: Lambjr088 Posted at: 2017-05-28T02:43:55.669Z Reads: 171

```
Actually measure the size of the compartment where the batteries go? That will help make a best decision for what you can fit in it.
```

---
## \#4 Posted by: Steamboat_Rock Posted at: 2017-05-28T02:57:21.743Z Reads: 164

```
The dimensions of the battery compartment are 4"(H) x 7" (W) x 12.5" (L) .  

As far as having the same amps etc., the honest answer is I do not know. I'd like to board to travel at least 15 miles between charge. The board reaches 20mph now, so I would like to at least reach this speed, but if possible with just a battery change I'd like to get 25mph to 30mph...

Are the 18650 batteries the one that I cannot leave on the charger once fully charged or they set on fire and cannot be run completely dry? I'd like to avoid these types as I'd probably burn my house down or break the batteries...
```

---
## \#5 Posted by: BigBoyToys Posted at: 2017-05-28T08:14:36.077Z Reads: 127

```
Your current battery apppears to be a combination of three 12v lead acid 14AH batterys connected in series totaling 36V. If you arent planning on changing your charger and speed controller(s) you would need to stay at 36V which means you will have the same top speed.

If you want similar range to the original batteries (14Ah), You'd need to run 3-4 of the 10S zippy lipos you asked about in parallel. If you wanted to use 18650 cells you'd need a 10S5P-10S6P setup depending on which cells you use. 

Sidenote: I can tell from the picture that your board doesnt use a Battery Management System (BMS). Using lipos without one will seriously shorten their life and could be dangerous.

@barajabali might be willing to build a 18650 pack with a built-in BMS for you that would suit your application but Im guessing that battery would run you $600 dollars or so.
```

---
## \#6 Posted by: Steamboat_Rock Posted at: 2017-05-28T09:01:18.764Z Reads: 109

```
I really appreciate the response. My main question at this point is the pro's and con's of zippy vs lead acid batteries. 
The cost of 3-4 x 10S zippy lipos is ~$210 to $280. 
The cost of 3 x 12V 14AH batteries is ~$75.

What are the pro's of spending the extra money and getting the zippy lipos? 


Also, I could not tell from your post, will I need a Battery Management System for the zippy lipos or does this only apply to the 18650 cells?
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-05-28T09:23:01.300Z Reads: 100

```
Lead acid batteies are just too heavy for skateboards and there lifespan is shorter too.

Lipos are inexpensive compared to Li ion cells but definitely needs a BMS.

Li ion cells are the most expensive but have the longest lifespan.
```

---
## \#8 Posted by: Steamboat_Rock Posted at: 2017-05-28T19:13:47.373Z Reads: 97

```
Ok, well if I am going to get into this hobby I better dive in and learn how to do this stuff from scratch! After doing a lot more research I THINK I am getting a little bit of a grasp on what needs to be done...

So if I buy two packs of  10 x 3.7V 10000mAh 18650 Li-ion Rechargeable Battery and run in parallel, that will give me 36V 20Ah. Looking at: 
http://www.ebay.com/itm/10-x-3-7V-10000mAh-18650-Li-ion-Rechargeable-Battery-Charger-for-LED-Flashlight-/152203085686?hash=item237002c776:g:bNoAAOSwfVpYrteB

Then I'll need two BMS to monitor each series, so two 
http://www.batteryspace.com/pcbforli-ion18650batterypack-36v37v27a-1alimit.aspx. 

Then I'll need a specific battery charger, something like:
http://www.batteryjunction.com/tenergy-90263-tb6b-chgr.html?gclid=CjsKDwjw6qnJBRDpoonDwLSeZhIkAIpTR8JHbdBSNIGCCJJYtb_WYmN1OR465NqWWgTuBWUsym9TGgJRTvD_BwE 

Am I on the right track? Anything I am missing?
```

---
## \#9 Posted by: Achmed20 Posted at: 2017-05-28T19:35:09.104Z Reads: 89

```
pretty sure those batteries are scam.
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-05-28T20:11:11.961Z Reads: 84

```
Reading up on the current rating for the various 18650 cells available would be a great idea. The most commonly used cell is the Samsung 25R. The cells you posted supply very little current and are not suitable for the high current demands of an electric skateboard.

Building battey packs also takes a decent amount if knowledge and some tools. Many use spot welders and nickle strips to connect the cells, some solder them together.  If you search battery builds on the forums you'll find some great info.

Also, you can use 1 BMS for the 10S2P pack you have in mind if you connect two cells in parallel and then connect each of the 10 pairs in series.
```

---
## \#11 Posted by: Steamboat_Rock Posted at: 2017-05-28T20:21:03.218Z Reads: 77

```
Quick question, the Samsung 25R are 2500mAh. To get to the 14 Ah the lead acid batteries were providing I'd have to run like 6 in parallel?
```

---
## \#12 Posted by: BigBoyToys Posted at: 2017-05-28T21:32:05.800Z Reads: 76

```
Correct that would give you 15Ah
```

---
## \#13 Posted by: Steamboat_Rock Posted at: 2017-06-10T20:08:51.149Z Reads: 63

```
What do you think about this 10s3p setup?

30x 18650 batteries
https://www.imrbatteries.com/lg-he2-18650-2500mah-20a-flat-top-battery/

BMS:
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html
or 
http://www.batterysupports.com/36v-37v-42v-10s-80a-10x-36v-lithium-ion-lipolymer-battery-bms-p-389.html

Charger:
http://www.ebay.com/itm/Lithium-Ion-Battery-Charger-Li-ion-LiPo-10S-42V-2A-for-36V-37V-Wall-Socket-AC-DC-/321555510511
or 
http://www.batterysupports.com/36v-42v-5a-lithium-ion-battery-charger-10s-10x-36v-lion-lipo-p-166.html


Thank you!
```

---
## \#14 Posted by: BigBoyToys Posted at: 2017-06-16T17:25:10.547Z Reads: 55

```
Those look good to me
```

---
## \#15 Posted by: Psyborg Posted at: 2018-04-24T04:00:03.073Z Reads: 38

```
Did you ever Successfully upgrade your battery? I am looking to do the Same thing
```

---
## \#16 Posted by: tsunami982 Posted at: 2019-03-06T20:01:49.843Z Reads: 29

```
I did something similar but used 5 LG hoverboard batteries wired in parallel (36v 4.4ah each totalling 22ah).  They don't sell the exact ones I used anymore but they are similar ones on eBay for around $35 each.  To wire them up, you can either create your own XT90 to 5x XT60 connector or buy a XT90 to XT60 adapter and 5 XT60 splitters (all easily found on Amazon). 

Hope this helps.
```

---
## \#17 Posted by: Paolosk8 Posted at: 2019-11-07T03:37:03.202Z Reads: 16

```
Hi mate, how did you end up charging these 5 batteries in parallel? I want to do something similar (only 2 batteries in parallel connected via a XT60 to 2 XT60 parallel connector) but not sure how to wire them so that I can charge them in parallel. Thanks!
```

---
## \#18 Posted by: tsunami982 Posted at: 2020-01-07T21:06:18.283Z Reads: 10

```
Long story short, yes you can charge them in parallel but (since you didn't state exactly which batteries you are using) make sure you consider your BMS discharge rating since you are using fewer packs.  The LG hoverboard packs I used were rated to discharge at 15a each (30a max) before the BMS overcurrent protection disables the battery.  At full throttle and at the lower end of the voltage range you could theoretically be pulling ~53a (1600w/30v) so to be safe I'd make sure your combined BMS output can handle at **least** 60a or you risk having a battery shutting down (or worse if it doesn't shut down and your batteries overheat).

I've since upgraded to 4x 36v 7.8ah packs.  I'm not an expert but my quick and dirty estimate gives me about ~445% range vs stock. Shoot me a message if you have any questions.

Calc: 7.8ah x 4 = 31.2ah.  Since Li depth of discharge is about 2x compared to SLA, that would be the equivalent of 62.4ah of SLA batteries.  Stock SLA batteries are 14ah so 62.4/14*100 = ~445%. Even if my calcs are way off (which they very well might be), I've gotten ~40 miles with capacity left to spare.
```

---
## \#19 Posted by: Paolosk8 Posted at: 2020-01-08T00:27:15.302Z Reads: 8

```
Thanks mate, 
Very clear.

I got some LiitoKala from AliExpress, the picture attached has all the details.
I've unpacked one and seems a good built pack.
The label says:
Max discharge: 30A
Max continuous discharge rate: 20A
Discharge rate: 15A

I'm going to try to run 2 of these in parallel and see how they run.
I don't envision for now going at full throttle, I may need to upgrade the battery in the future if thay becomes a must.

I'll keep you posted!
Paolo

![Screenshot_20200108-082157_AliExpress|243x500](upload://g5IuNV1Js2A4bo6TZfRJHKGAaFy.jpeg)
```

---
