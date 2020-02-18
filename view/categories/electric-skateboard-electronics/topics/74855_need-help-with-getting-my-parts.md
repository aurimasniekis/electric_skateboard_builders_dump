# Need help with getting my parts!

### Replies: 68 Views: 474

## \#1 Posted by: JosephShubin Posted at: 2018-11-15T21:05:22.707Z Reads: 141

```
Hello builders, I'm "new" to E-Boards. I mean there isn't much to understand once you know electronics well enough, but I'm no pro when it comes to Electronic Systems, so I wanted to ask for help and recommendations. Note: The board will have 6 wheels, yeah 6. It will have a Tandem Axle setup in the nose. Pic:![image|666x500](upload://mgb85Rtf0RbT1J8htxCQHdlwAwp.jpeg) 
These are my following 'Specs':
- 42" DIY Deck (3 x 3/16" Plywood W/ Fiberglass and Resin in between Layers)
- Caliber II RKP Trucks, Front, and Rear
- Cal 97mm Wheels, 6x
- Flipsky Dual FSEC 4.20, 100A
- 2x Hobbysky 6374 190KV BLDC
- DIY, 12S2-4P Li-Po Battery Pack using 10000Mah Cells from Alibaba (many to choose from, but they are ALL dirt cheap)
- Tx/Rx, just a cheap one
- Gearing ~2.5-3.5:1 Ratio
- BMS 12S 30A(?) 48V
So the only real part I need help with is the BMS, at least for now. I understand how to wire up the BMS to the cells (not hard), but what I can't seem to understand is the Amp rating for the BMS. The eBay seller I will buy the BMS from sells multiple variants, ranging from 30-60A. Is the Amp rating the max the system can take before its toast? Idk, kinda lost, so I decided to ask you pros. I think it has to do with the C rating of the entire Battery Pack than I will need to get the BMS according to the Battery Specs...?

Thank you guys, 

Regards, 

Joseph, a noob builder :grinning:
```

---
## \#2 Posted by: RedEagle Posted at: 2018-11-15T21:13:38.397Z Reads: 122

```
So let's say you have a 60a bms. If you pull more than 60a your bms will cut the power because it's designed to deliver 60a and not more than that. You'd be better off with a 80a bms because if you overbuild then you can ride knowing you're not pushing your system. Most of us run 60a bms's.
You can also bypass a low amp bms and use it for charging only.
```

---
## \#3 Posted by: dg798 Posted at: 2018-11-15T21:14:25.760Z Reads: 116

```
If u are doing dual setup you should take a look into the dual flipsky vesc 6. I’ve heard pretty good things about it. Also you will want a 12s4p if running dual drive. If u are using bms for discharge as well spend the extra money on a 12s bestech bms so u get a high discharge amperage rating. If ur doing charge only get whatever amperage u want for discharge because u won’t be discharging for it. I have used theb12s bestech d140 for charge only and it works fine.
Good luck
```

---
## \#4 Posted by: dg798 Posted at: 2018-11-15T21:15:34.247Z Reads: 102

```
Also buy real cells like Samsung 30q or 25r. I would trust Chinese cells because they are so cheap, it’s probaly too good to be true
```

---
## \#5 Posted by: Grozniy Posted at: 2018-11-15T21:17:17.168Z Reads: 92

```
Choose dual 6.6 instead of 4.2 if going flipsky. If not, get Focbox.
```

---
## \#6 Posted by: dg798 Posted at: 2018-11-15T21:17:58.817Z Reads: 87

```
Also if u want a cheap and reliable remote get the 2.4 ghz rc mini remote
```

---
## \#7 Posted by: JosephShubin Posted at: 2018-11-15T21:22:11.695Z Reads: 86

```
WOW, response in just 2 mins. Thank you! Yeah, I'll go with 12S4P. And, ill spend an extra buck on a high discharge BMS, probably. Also, about the 18650 cells. To build what i want, and the budget I got, it would be over ~$200 for just a battery (good cells cost ~$5-8/Ea). I cant afford that. So I will probably just buy 4 x 3S Li-Po's and dissect them to fit my requirements.

-Joseph
```

---
## \#8 Posted by: JosephShubin Posted at: 2018-11-15T21:23:41.473Z Reads: 81

```
I would if I had the cash. :frowning_face:
```

---
## \#9 Posted by: dg798 Posted at: 2018-11-15T21:25:15.780Z Reads: 80

```
Lipos are also good. Make sure u get a high c rating lipo
```

---
## \#12 Posted by: dg798 Posted at: 2018-11-15T22:56:11.630Z Reads: 67

```
Just remember it’s only 60 amps.
```

---
## \#13 Posted by: JosephShubin Posted at: 2018-11-15T23:33:15.995Z Reads: 68

```
Yeah, I'll go up to an 80Amp instead. Better safe than sorry.
~$70....:face_with_raised_eyebrow::open_mouth:
https://www.ebay.com/itm/44V-48V-50-4V-12S-80A-12x-3-6V-3-7V-4-2V-Lithium-Li-ion-Li-Po-Battery-PCB-BMS/173543196319?hash=item2867fb069f:g:a1QAAOSwNaNbTWU7:rk:3:pf:1&frcectupt=true
```

---
## \#14 Posted by: JosephShubin Posted at: 2018-11-15T23:37:00.669Z Reads: 70

```
Update: I forgot I had found these cells earlier.
- 8Ah (8000Mah)
- 25C
https://www.ebay.com/itm/183036786061
They telling me they're monsters of cells, so maybe them. Idk just yet.
```

---
## \#15 Posted by: dareno Posted at: 2018-11-15T23:41:35.730Z Reads: 68

```
This guy used those cells in a pretty average build but it might be helpful.
https://www.youtube.com/watch?v=5Q0m8n-b8cY&t=31s


Also if you are running 12s then don't use the 4.20 vesc.  Go for a 6 or a focbox.

Also don't go cheap on the bms.  Use a decent one or you will have drama.  Go for a bestech with a minimum of 80 amps or a low amp wired for charge only.
```

---
## \#16 Posted by: JosephShubin Posted at: 2018-11-15T23:45:51.480Z Reads: 63

```
Well, yes, but he is only running 6S. Mine would be 12S4P, so range and overall power output would more than double,in theory. Well and, it would be ~$160 for 16 of these, and needing all the other parts, that is sadly MAYBE just too much for my budget, but we'll see.
```

---
## \#18 Posted by: dareno Posted at: 2018-11-15T23:49:45.995Z Reads: 60

```
Theres a big sale coming up too.  You can not go better than a focbox unless you can afford a proper vesc6.  I use them on all my builds and they are rock solid on 12s.
```

---
## \#19 Posted by: dg798 Posted at: 2018-11-15T23:49:57.716Z Reads: 58

```
I say but a charge only bms for cheap like from @JLabs and then use the extra money for other things.
```

---
## \#20 Posted by: dg798 Posted at: 2018-11-15T23:51:19.843Z Reads: 55

```
If u din want a focbox or vesc 6 @torqueboards vescs are indestructible even at 12s. I have used them with 12s before.
```

---
## \#21 Posted by: JosephShubin Posted at: 2018-11-15T23:53:31.151Z Reads: 51

```
Yeah, Ill consider all the options.
```

---
## \#22 Posted by: dareno Posted at: 2018-11-15T23:53:48.853Z Reads: 51

```
Yeah i would be a bit careful with a standard 4.12 vesc.  If you are going to run them then you definitely need to heatsink the shit out of them.  My tb and hk vescs got extremely hot running 12s.
```

---
## \#23 Posted by: dg798 Posted at: 2018-11-15T23:54:28.070Z Reads: 53

```
I don’t heatsink mine and they are perfectly fine.
```

---
## \#24 Posted by: JosephShubin Posted at: 2018-11-15T23:54:39.339Z Reads: 56

```
I would need two since i'm running dual. Would I need a custom wiring system so they would work synchronous?
```

---
## \#25 Posted by: dg798 Posted at: 2018-11-15T23:57:25.642Z Reads: 54

```
Canbus or split ppm. I think split ppm is safer. Also go onto @torqueboards website. He has a guide for setting up dual drive setups with 2 vescs
```

---
## \#26 Posted by: Skunk Posted at: 2018-11-16T00:02:39.783Z Reads: 57

```
New focboxes no longer have canbus issues
```

---
## \#27 Posted by: dareno Posted at: 2018-11-16T00:03:55.335Z Reads: 56

```
If you are going to run foc with all the bells and whistles ie traction control or a bluetooth module then you need a canbus connector.  If you want simple bldc then a split ppm cable for the receiver will do.  
https://www.youtube.com/watch?v=qpovd2XRKqc&t=890s

this vid goes through the wiring and set up for both  

@dg798  do you run them constantly on 12s or was it just for a while.  Do you have a 12s set up running tb vescs?
```

---
## \#28 Posted by: dg798 Posted at: 2018-11-16T00:05:01.958Z Reads: 48

```
I have only used 12s with Tb vesc
```

---
## \#29 Posted by: dareno Posted at: 2018-11-16T00:08:24.263Z Reads: 51

```
For me the heat was an issue.  Bearing in mind I do live in Australia where an average winter is still 26'c so that may have played a part but I also don't like how close you come to the erpm limit on 4.12 either.  It just makes things much easier for a noob to pop something with incorrect kv etc.  
Hey don't go blaming me if I have put the kiss of death on your set up and something blows lol
```

---
## \#30 Posted by: dg798 Posted at: 2018-11-16T00:09:04.041Z Reads: 47

```
I limit the erpm to 60000
```

---
## \#31 Posted by: dg798 Posted at: 2018-11-16T00:10:02.086Z Reads: 48

```
Winters in New York can get below 32f
```

---
## \#32 Posted by: dareno Posted at: 2018-11-16T00:13:48.582Z Reads: 48

```
Without confusing the guy too much. I use tb vescs and hk vescs but I'm sure that no one can argue that the focbox is the best 4 variant on the market for control and reliability.  It just is.
```

---
## \#33 Posted by: JosephShubin Posted at: 2018-11-16T00:15:43.463Z Reads: 47

```
I'll run twin Focbox, why not lol. They get good reviews.
```

---
## \#34 Posted by: Skunk Posted at: 2018-11-16T00:17:24.739Z Reads: 48

```
[quote="dg798, post:31, topic:74855"]
New York can get below 32f
[/quote]

He was taking about how hot Australia can get.
Note the c after 26.
We're not taking about cold focbox issues.
```

---
## \#35 Posted by: dareno Posted at: 2018-11-16T00:19:55.060Z Reads: 44

```
They are the most widely used motor controller and for a good reason.  They work very well
```

---
## \#36 Posted by: JosephShubin Posted at: 2018-11-16T00:22:24.840Z Reads: 44

```
About the BMS. I'll be running 12S4P. Every cell (16) needs to be hooked up to the BMS if I'm using it for charging. So if i run the BMS bypassed when not charging, it does not really matter how high the Amp rating is, right?
```

---
## \#37 Posted by: moone Posted at: 2018-11-16T00:25:21.757Z Reads: 44

```
It's 35'C or 95'F here today and it's not even summer yet. 🔥

Focbox unity is something else to look into as well if you don't mind the wait.
```

---
## \#38 Posted by: J0ker3366 Posted at: 2018-11-16T00:27:40.012Z Reads: 44

```
[quote="JosephShubin, post:36, topic:74855"]
Every cell (16)
[/quote]

Do you have this 12s4 you speek of?
```

---
## \#39 Posted by: JosephShubin Posted at: 2018-11-16T00:28:19.291Z Reads: 40

```
Lol, nope. It'll take time.
```

---
## \#40 Posted by: J0ker3366 Posted at: 2018-11-16T00:28:37.126Z Reads: 40

```
I'd really like to see a 12s4 that only has 16 cells.
```

---
## \#41 Posted by: JosephShubin Posted at: 2018-11-16T00:29:01.060Z Reads: 36

```
Whoops, lol my mistake.
```

---
## \#42 Posted by: dareno Posted at: 2018-11-16T00:30:33.870Z Reads: 38

```
We're in the thirties and its spring lol.  
@JosephShubin
If you're not discharging through it then the amp rating can be low.  Nice little tiny one.  The bestech 80 amp is a beast of a thing.  If I was using a charge only I could have got another 10 cells in my evo.
```

---
## \#43 Posted by: J0ker3366 Posted at: 2018-11-16T00:31:54.875Z Reads: 35

```
Should of would of could of 😛😈
```

---
## \#44 Posted by: JosephShubin Posted at: 2018-11-16T00:40:02.077Z Reads: 37

```
4.20V/Cell x 12 Cells, in Series gives me a max voltage of 50.4 Volts. Add 2-4 Cells in Parallel will increase Ah. I'm getting this right?
Note: Lipo Cells are slim/flat, so I might be able to fit all this in a large pack. :thinking:
```

---
## \#45 Posted by: dg798 Posted at: 2018-11-16T01:02:56.835Z Reads: 37

```
I can help you with ur bms once ur ready to wire it. Shoot me a PM and I can walk u through the process
```

---
## \#46 Posted by: dg798 Posted at: 2018-11-16T01:03:44.379Z Reads: 37

```
I know I’m just saying why I don’t necessarily need a heatsink on my board.
But let’s stay on topic
```

---
## \#47 Posted by: JosephShubin Posted at: 2018-11-16T01:38:52.412Z Reads: 36

```
Thank, I defenitly will when time comes.
```

---
## \#48 Posted by: dg798 Posted at: 2018-11-16T01:39:24.849Z Reads: 37

```
Ok take ur time and learn. This can be a very tedious process. Good luck
```

---
## \#49 Posted by: JosephShubin Posted at: 2018-11-17T07:16:28.349Z Reads: 36

```
Uhm, just found this. Idk what to say. Should I buy one? Test it?

https://www.alibaba.com/product-detail/22-2v-60C-120C-6s-24000mAh_60194025070.html?spm=a2700.7724838.2017115.52.62bd51dbL2CyKY
```

---
## \#50 Posted by: Grozniy Posted at: 2018-11-17T07:40:51.362Z Reads: 33

```
For science, yes
```

---
## \#51 Posted by: JosephShubin Posted at: 2018-11-17T07:42:18.604Z Reads: 35

```
What do you mean science? Buy, test, post here?
```

---
## \#52 Posted by: JosephShubin Posted at: 2018-11-20T01:06:04.486Z Reads: 25

```
Update: So after some more research and thought, I have further refined and zeroed in on how I want my E-Board to look like and perform. Here is my updated parts list and explanations:

Note: The board will be built around my weight, height, budget, and personal preference. I'll take any constructive criticism happily.

I weigh ~145-150Ibs (66-68Kgs), 5'11" tall, male, currently 17.

Mechanical, non Electric:
- Deck will be made of 3 x 3/16" Plywood w/ Fiberglass tape in-between layers. Bonded with Bondo Fiberglass Resin. The deck will be 10" wide and 42" long. I want stability.
- The Trucks will be 2 x Caliber II (44 Deg.) and will be drop through. Nothing special. They got good reviews, are very common, and very cheap. They're 10" wide axles, so overall width w/ wheels will be over 1'. This will also increase stability.
- Wheels will be 4 x Cal 97mm wheels. They're cheap, got good reviews, and large. I want higher speeds than acceleration. 
- The pulley setup is a bit iffy. I will go for a ratio of ~2-3. I don't got any hills to go over around me, at least significant, so I'll prefer speed. The motor gear, or input will be a 20T, 10mm bore. I can't seem to find any reasonable priced and 'good' quality gear for the motors. They are expensive (~$100 for two sets) and that would be ~40-42T. Recommendations? 10mm belt(s).

Electrical:
- I'll be running a dual drive system. The motors a will be 2 x 6374's. I was going to go with "Hobbysky" motors, but they are $80/Ea. Too much. I know going with unbranded Chinese motors is iffy, but spending ~$180 is too much.
- I'll go with two Focbox systems. They seem to be popular and good. Not to cheap, but reasonable. 
- A cheap, ~$30 Tx/Rx. Nothing special.
- I've updated my battery system as well. I want to go with Zop 5200mah 50C 3S Li-Po's. They get good reviews on eBay and Bangood. I'll buy them from eBay. The seller is selling 4 of them for only $100! That's awesome! I will be running 12S4P, so 11.1V (3S) x 4 cells = 44V. Than i'll add 3-4 more in Parallel to increase capacity. 
- I'll bypass BMS, but will charge w/ BMS.
- The charger will be a Power Supply rated for 60V @ 5A.

So, that's about it for now. Any corrections, recommendations, etc are welcome. Here is the parts list with links on Google Sheets. Total price right now is around ~$800.

https://docs.google.com/spreadsheets/d/1KfCwrqg6k5E3N9IFZmhBAoCHk1Cx_zV-6Z9xUjNmEa4/edit#gid=0
```

---
## \#53 Posted by: briman05 Posted at: 2018-11-20T01:14:27.574Z Reads: 20

```
You need a remote
```

---
## \#54 Posted by: JosephShubin Posted at: 2018-11-20T01:16:15.212Z Reads: 20

```
" A cheap Tx/Rx..."  Tx= Remote. Rx= Receiver.
```

---
## \#55 Posted by: dg798 Posted at: 2018-11-20T01:30:59.993Z Reads: 19

```
power supply for 12s should be 50.4v
```

---
## \#56 Posted by: JosephShubin Posted at: 2018-11-20T01:33:53.436Z Reads: 19

```
Forgot to mention, you can change the Voltage and Amperage. 60V is max.
```

---
## \#57 Posted by: dg798 Posted at: 2018-11-20T01:35:06.463Z Reads: 18

```
can you post a link where u are getting it from
```

---
## \#58 Posted by: JosephShubin Posted at: 2018-11-20T01:36:09.895Z Reads: 18

```
It is in the parts list Google Sheet slink, but her it is: 

https://www.ebay.com/itm/0-5A-0-60V-10A-30V-Lab-Adjustable-DC-Power-Supply-Line-Variable-Digital-Voltage/382416128861?hash=item5909c70b5d:m:mgIKEaOtfMiqHfGGR_y_4rw:rk:6:pf:1&frcectupt=true
```

---
## \#59 Posted by: dg798 Posted at: 2018-11-20T01:37:53.467Z Reads: 18

```
im just gonna check and make sure its cc-cv charging
```

---
## \#60 Posted by: dg798 Posted at: 2018-11-20T01:39:34.107Z Reads: 16

```
you cant get this one because it doesnt have cc-cv charging and your battery will be all out of wack if theres not cc-cv charging
```

---
## \#61 Posted by: JosephShubin Posted at: 2018-11-20T01:41:04.681Z Reads: 16

```
I didn't even know that. Thank you. I have a charger that i charge my lipos with but it would just take to long to charge each battery individually. Any recommendations on chargers?
```

---
## \#62 Posted by: dg798 Posted at: 2018-11-20T01:41:37.113Z Reads: 16

```
look at diyelectricskateboards.com chargers for 12s.
it should be there
```

---
## \#63 Posted by: dg798 Posted at: 2018-11-20T01:42:35.452Z Reads: 16

```
collections/battery-chargers/products/12s-2a-battery-charger
```

---
## \#64 Posted by: dg798 Posted at: 2018-11-20T01:43:26.479Z Reads: 14

```
collections/battery-chargers/products/12s-4a-battery-charger
```

---
## \#65 Posted by: JosephShubin Posted at: 2018-11-20T01:43:39.882Z Reads: 15

```
Wow, only $30. I just hope it charges fast.
```

---
## \#66 Posted by: dg798 Posted at: 2018-11-20T01:44:18.760Z Reads: 15

```
2 amps will be a little on the slower side but the 4 amp one will be fast
```

---
## \#67 Posted by: JosephShubin Posted at: 2018-11-20T01:44:51.970Z Reads: 15

```
Yeah, ill go with 4amp. A bit more, not a problem.
```

---
## \#68 Posted by: dg798 Posted at: 2018-11-20T01:45:12.406Z Reads: 15

```
good idea
10 charc
```

---
## \#69 Posted by: JosephShubin Posted at: 2018-11-20T01:45:55.663Z Reads: 16

```
10 charc? what does that mean?
```

---
## \#70 Posted by: dg798 Posted at: 2018-11-20T01:46:38.517Z Reads: 17

```
you have to type 10 characters in a post so if you dont ppl. just type 10 charc
```

---
## \#71 Posted by: JosephShubin Posted at: 2018-11-20T01:47:53.367Z Reads: 17

```
Thank you
10 charc
```

---
