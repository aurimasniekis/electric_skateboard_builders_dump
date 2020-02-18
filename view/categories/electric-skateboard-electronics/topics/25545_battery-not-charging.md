# Battery not Charging!

### Replies: 41 Views: 3051

## \#1 Posted by: SeanHacker Posted at: 2017-06-17T01:02:11.917Z Reads: 156

```
Hey guys! It's me again. I'm having an issue with my battery only charging to 70-80%. I just changed the BMS (Supower 10s 60a) because I thought that the one prior was going bad. But it seems to be doing the same thing. I noticed my charger (Enertion fast charger) started turning off and on when it's gets to 70-80%. Is this part of the BMS working and it's trying to balance the cells or something? I'm at a loss and really hope I don't need to replace the battery. Too expensive of a fix for me right now. I have a 10s4p Samsung 22r (green ones) from Chiboards. Anyone have a clue?

Here's a video of what happens with the charger now. 
 https://www.youtube.com/watch?v=ilY3KGt7P1c
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-17T01:03:13.159Z Reads: 154

```
My guess are some cells got disconnected or died. Check individual group voltages.
```

---
## \#3 Posted by: SeanHacker Posted at: 2017-06-17T01:05:14.406Z Reads: 150

```
Thanks @Jinra. I'm a total dummy when it comes to batteries. I just bought a multi-meter but I'm not really sure where to to poke them to. Can you maybe help me with that. Here's a pick of my battery. 

<img src="/uploads/db1493/original/3X/c/b/cbec4ff46def048201d618f13a6dff4b3ec2d50a.jpg" width="375" height="500">
```

---
## \#4 Posted by: Jinra Posted at: 2017-06-17T01:15:29.417Z Reads: 139

```
negative to positive for each group of 4 cells. You should be getting 3-4v~ per group. See if you can find one or two not like the others. I can't edit pictures right now so hard to explain.
```

---
## \#5 Posted by: SeanHacker Posted at: 2017-06-17T01:17:30.056Z Reads: 137

```
I really wish I knew where the positive and negative for each cell groups were. Lol. I also wish I knew more about these batteries. FML. Thanks for the input though dude. I really appreciate it!
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-17T01:21:17.950Z Reads: 139

```
prod one probe on the bottom left cell group of that picture and the other one to the corresponding terminals of the cell group (in between the cells), start there. Hopefully you can get it. Just try to get that 3-4~v reading. Make sure your multimeter is setup correctly for reading voltage.

EDIT: it looks like the cell groups are numbered on the cells, that should help as well
```

---
## \#7 Posted by: JLabs Posted at: 2017-06-17T01:22:25.189Z Reads: 134

```
You want to get on Skype quick? It would be a lot easier to explain over video. PM me your Skype username if you want.
```

---
## \#8 Posted by: SeanHacker Posted at: 2017-06-17T01:24:44.730Z Reads: 132

```
I wish I could right now. I actually wrapped up the battery and packed it up in my enclosure (It's a bitch to take apart) already. I have some family from out of town here at the house until tomorrow morning too. Would you be able to Skype with me tomorrow? I will have the board taken apart in the morning. Thanks a lot dude!!!

I really love this board and hope to get it working like it used to. 
<img src="/uploads/db1493/original/3X/8/e/8edc7dc9aedc525c96161eb5280d9eabd9ae6935.jpg" width="375" height="500">
```

---
## \#9 Posted by: JLabs Posted at: 2017-06-17T01:27:34.928Z Reads: 127

```
Yeah no problem, I will be getting lunch or dinner for fathers day tomorrow but before/aftee that is cool with me. I actually have a battery taken apart to use as an example
```

---
## \#10 Posted by: SeanHacker Posted at: 2017-06-17T01:33:46.635Z Reads: 129

```
Sweet!!! Thanks a lot dude. I'll PM you here tomorrow to see if you're around.
```

---
## \#11 Posted by: SeanHacker Posted at: 2017-06-17T01:35:18.738Z Reads: 130

```
Thanks! That helps me get the picture. I'm going to look at some diagrama of 10s4p batteries just to try and get the hang of how these are setup. And @JLabs is going to help through skype (which will be nice to actually see).
```

---
## \#12 Posted by: JdogAwesome Posted at: 2017-06-17T01:55:29.621Z Reads: 127

```
This sounds like it could be a problem with your charger not your BMS or LiPo's. I feel like the BMS would have, and should have, prevented any cells from being over or under charged and balanced them out appropriately.  I do recommend doing what @Jinra said as it should be kinda common practice to make sure there balanced properly but after that if the problem persists maybe try a different power supply.
```

---
## \#13 Posted by: SeanHacker Posted at: 2017-06-17T04:14:17.865Z Reads: 121

```
Do you have any recommendations for a power supply @JdogAwesome?
```

---
## \#14 Posted by: Tobi Posted at: 2017-06-18T06:06:19.561Z Reads: 118

```
take your volt meter turn the bms and put the negative end of your volt meter on b1 and let it stay there. Put the positive wire on b2 then b3 b4 b5 to get the voltage of each cell groups.

easy peasy
```

---
## \#15 Posted by: SeanHacker Posted at: 2017-06-18T16:55:20.021Z Reads: 111

```
Thanks dude. You mean like this right? The voltages differ from each other a bit between a couple series. 

https://youtu.be/lKYm0LmixpE

@JLabs I got way too busy yesterday to get a hold of you and today is fathers day and didn't want to bother you. :slight_smile:
```

---
## \#16 Posted by: JLabs Posted at: 2017-06-18T17:10:51.153Z Reads: 106

```
Yes that's exactly what you want to do! I would he worried about the 3.56v group, it varies a lot from the 3.84v. maybe you could consult @barajabali. My guess it that the BMS is trying to protect the pack, thus not charging it (not my complete expertise).
```

---
## \#17 Posted by: SeanHacker Posted at: 2017-06-18T17:56:50.784Z Reads: 101

```
Nice. I knew I was trying to over complicate how to check voltages in my head. I for some reason thought I was going to have to take a part the battery (which I can't do) in order to check the individual series groups. Do you have any clue as to why this would happen? Is it possible to just charge one group at a time that you know of?
```

---
## \#18 Posted by: JdogAwesome Posted at: 2017-06-18T23:42:18.598Z Reads: 98

```
Hey sorry for the late reply, been on a road trip and haven't had service for a while. It really depends on how the charging system works, if the Enertion fast charger is just a 42V power block then really any 42V PSU will work. I personally use a generic 24V PSU to charge my 6S LiPo pack and I adjust the internal pot up a bit to get 25.2V and you could just turn yours down to 42V. 
[quote="SeanHacker, post:17, topic:25545"]
Is it possible to just charge one group at a time that you know of?
[/quote]
Yeah definitely, just find the cells that you want to charge and connect either a CC/CV PSU to it and just slowly charge it to the same voltage as the other cells or use a LiPo charger like Imax B6 in 1S mode and charge it that way.
```

---
## \#19 Posted by: Tobi Posted at: 2017-06-19T03:56:05.717Z Reads: 93

```
The voltage should increase lets say battery is charged to 36 volt ist should be looking like this

b1 = 3.6 v
b2 = 7.2 v
b3 = 10.8 v
b4 = 14.4 v

thats how it should look like
```

---
## \#20 Posted by: SeanHacker Posted at: 2017-06-20T00:03:43.532Z Reads: 89

```
Thanks @Tobi.  That's about the voltages I got when I did that.
```

---
## \#21 Posted by: SeanHacker Posted at: 2017-06-20T00:05:04.448Z Reads: 85

```
Does anyone here have any recommendations for any chargers on Amazon I can get that will work with my battery?
```

---
## \#22 Posted by: Tobi Posted at: 2017-06-20T03:58:32.415Z Reads: 85

```
you need 42 volt 2 ampere charger

https://www.amazon.com/s/ref=nb_sb_noss?url=search-alias%3Daps&field-keywords=42+v+charger+2a&rh=i%3Aaps%2Ck%3A42+v+charger+2a
```

---
## \#23 Posted by: SeanHacker Posted at: 2017-06-21T00:35:04.208Z Reads: 82

```
I have two 42 volt chargers here at home. One is an enertion fast charger and the other is just the regular one for my old Raptor. I was wondering about a balance charger that would work for my battery so that I can make all the cell equal again.
```

---
## \#24 Posted by: SeanHacker Posted at: 2017-06-21T00:39:39.652Z Reads: 83

```
Hey s guys. I'm searching for lipos on amazon and I think I read somewhere that @Namasaki said that Venom brand batteries are good. Are these batteries decent. And what charger should I get to charge them? How many should I get. I would like to go fast and get some good mileage per charge like my 10s4p would get. Thanks again dudes!

https://www.amazon.com/Venom-5000mAh-Battery-Universal-Traxxas/dp/B004YNQX7S/ref=sr_1_40?ie=UTF8&qid=1498005095&sr=8-40&keywords=venom+lipo+battery

https://www.amazon.com/Venom-5000mAh-Hardcase-Battery-Connector/dp/B01KBRKYPM/ref=sr_1_62?ie=UTF8&qid=1498005439&sr=8-62&keywords=venom+lipo+battery
```

---
## \#25 Posted by: JLabs Posted at: 2017-06-21T00:45:57.577Z Reads: 75

```
I also heard that the Venom batteries for good so I spent quite a bit extra to get them and even paid for the corresponding lipo charger. Lasted only eight months and then the cells got totally imbalanced
<img src="/uploads/db1493/original/3X/c/6/c60d2e500c760c349e2bb34a03374a49ea8430ff.JPG" width="375" height="500">
Also when I built my first board pre-built liion packs weren't really a thing
```

---
## \#26 Posted by: SeanHacker Posted at: 2017-06-21T01:01:21.046Z Reads: 73

```
Bummer about your experience. I can deal with 8 months though. I ride hard around the city so I just want something dependable. I wish I could find a prebuilt liion pack for a lower price than what I've seen. I've spent too much in the last 6 months and my fiance won't have it anymore. lol.
```

---
## \#27 Posted by: Namasaki Posted at: 2017-06-21T01:22:46.979Z Reads: 70

```
I had only one set of Venoms.  6s/2500mah I ran them in series.
They gave me a solid 5 mile range and no swelling.
I didn't have them in service for 8 mo. though.
They where in my safe along with my Basen 4500 battery build when it got stolen during a burglary.
Also mine where the older version, not the "Fly" version.
```

---
## \#28 Posted by: Namasaki Posted at: 2017-06-21T01:27:37.418Z Reads: 71

```
Those Venom batteries from Amazon are just too expensive, I would not recomend paying that much for them.

You would probably do better with Gens Ace. They are said to be good and a lot cheaper than Venom.

**Disclamer**
I have never used Gens Ace, I have just heard that they are good.
https://www.amazon.com/s/ref=nb_sb_noss_2?url=search-alias%3Daps&field-keywords=gens+ace
```

---
## \#29 Posted by: wmj259 Posted at: 2017-06-21T02:21:07.290Z Reads: 68

```
Yeah, those batteries are costing you more then what li-ion cells would cost. I would recommend using the lipo search on Hobbyking.com. You can enter many specifics criterias and it will show you many good options. For $101 I bought me some good lipos from aliepress.
```

---
## \#30 Posted by: Namasaki Posted at: 2017-06-21T02:56:44.162Z Reads: 69

```
I have been using five of these in series with a BMS on both of my builds and they have been rock solid so far.
My build number one has been sporting them for  9 months of recreational riding with lots of hill climbing.
https://hobbyking.com/en_us/turnigy-5000mah-2s-7-4v-60c-hardcase-pack.html
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014?u=namasaki
```

---
## \#31 Posted by: Namasaki Posted at: 2017-06-21T03:22:16.887Z Reads: 66

```
This is my main charger for my boards with onboard bms
My Battery Supports 5a charger is in the closet getting dusty.
https://www.amazon.com/gp/product/B00G0HAY3U/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#32 Posted by: SeanHacker Posted at: 2017-06-21T16:17:59.413Z Reads: 61

```
Looks great. I think I'm going to order this charger today. @Namasaki Would u be able to charge my boards through  the charge port (same as the space cell has)? Would I also be able to charge the groups of cells individually so that if they are u balance I can balance them properly?
```

---
## \#33 Posted by: Namasaki Posted at: 2017-06-21T17:02:30.741Z Reads: 61

```
This power supply makes a very versatile charger. 
You can adjust the voltage anywhere from 0-60v
So you can charge any size pack up to 12s as a whole or charge individual cells or cell groups. 
You just need to make a charge cable for your charge socket and some alligator clips for charging individual cells
```

---
## \#34 Posted by: SeanHacker Posted at: 2017-06-21T17:30:41.192Z Reads: 60

```
That's awesome. Sounds like I need something like this. Do you have any info on how to make a charge cable for the socket? I think I know how to make the alligator clips for charging individual cell groups.
```

---
## \#35 Posted by: Namasaki Posted at: 2017-06-21T17:36:15.461Z Reads: 57

```
Just find a matching connector for the charge socket and  two 4mm male banana connectors and son wire
```

---
## \#36 Posted by: SeanHacker Posted at: 2017-06-22T00:58:09.800Z Reads: 55

```
Thanks @Namasaki for the power supply recommendation. I just ordered the same one you have. It'll be here in a week or so. So now if I switch over to lipos I should be in a better position to charge them and keep them safe and healthy. Hopefully it'll do the same for my liions too!
```

---
## \#37 Posted by: Namasaki Posted at: 2017-06-22T04:41:34.991Z Reads: 51

```
I still use a hobby charger to charge individual multi cell Lipo packs because you can't connect to their individual cells seeing that they are sealed up.
You could use the power supply to balance them by charging their individual cells though the balance leads as long as you use low current.

Anytime you charge multiple cells in series, you either need a balance hobby charger or power supply charging through a bms.
When charging a single cell or cell group which is multiple cells in parallel, you don't need the bms or a balance charger.
```

---
## \#38 Posted by: kitthak123 Posted at: 2019-03-04T20:43:18.735Z Reads: 23

```
Hi I am having a similar problem.  I have a 10s2p homemade battery 36V.  My problem is that it is not charging.  I had a 42v 3A charger but it seems to be broken.  I've borrowed a normal 19V laptop charger and it appears that my battery is in fact losing charge.  Is this supposed to happen?  Any suggestions?
```

---
## \#39 Posted by: TowerCrisis Posted at: 2019-03-04T20:48:53.200Z Reads: 23

```
Oh lord.

Do NOT plug in that 19V charger.

A chargers voltage isn't some kind of "power" spec. The voltage needs to match the battery, hands down, or something could catch fire.

If you have a 10S battery then that means your charger needs to go up to 42V.

How are you try to charge it? Is there a BMS between the charge port and the battery? Are you trying to charge just the pack alone? We need more details.
```

---
## \#40 Posted by: kitthak123 Posted at: 2019-03-04T21:12:25.451Z Reads: 22

```
yes there is  a bms attached but the 42v charger i had broke so I was trying to find a way to charge it for the moment.  Thanks for saving me lol
```

---
## \#41 Posted by: TowerCrisis Posted at: 2019-03-04T21:28:55.422Z Reads: 20

```
If you have a CCCV bench power supply you can set it to 42V 3A you could charge it that way until you get yourself a new charger.
```

---
