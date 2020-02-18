# Nuff Longboard Experiences and Repairs

### Replies: 31 Views: 1179

## \#1 Posted by: bluegreen Posted at: 2019-04-08T01:49:26.729Z Reads: 157

```
So I got this for $229 but it went up to $249 has anyone else had experience with these?

https://www.ebay.com/itm/Nuff-1000-Watt-Electric-Skateboard-Long-Board-Blue-Teal-TOROID-L2-BRAND-NEW/163567498037?hash=item261561f335:g:AFgAAOSwS3NcdZfw

The best info for me so far has been this thread:

https://www.electric-skateboard.builders/t/onan-x2-hack-jet-spud-swappable-10s2p-2x-vesc-hummie-hubs/14965 

Before anyone says anything I bought this mostly out of curiosity of how much board you could actually get for $229, fully expecting there to be problems and things to break.
![55498131_10103786744874908_7930326962222923776_n|690x388](upload://uLn7oUmvFvIX2JOsigPayGLzj81.jpeg) 

This is based on the Onan X1, so first off I was most worried about the battery falling out, as this was the most common problem I had read about online but It hasn't been an issue yet. I was surprised the power the board delivers does seem to be as advertised, the low setting is about 13mph and the high setting is about 18. The battery gets between 6 and 8 miles depending on how hard you push it. 

I was also surprised, but realized later that it is normal, you have to kick off first it won't move from a dead stop.

The remote is probably the biggest problem most people would have with it, that it has disconnection problems really bad if you ride it anywhere in the city with a lot of interference. If you are somewhere you ever have problems with your bluetooth headphones, you're going to be in trouble because the remote won't work and you will be embarrassed looking confused why you are coming to a stop getting passed by lots of bicycles tell you the bike lane is for bikes only :frowning:  ... have some hope to fix that more on that later...
![55759870_10103794885391248_2574936449908473856_n|666x500](upload://q0Rls7iTFPAJKV1RCSzjR68XqS1.jpeg) 

The main reason I'm writing this post other than I'm curious if anyone else has one of these boards is that actually it was making a grinding noise sometimes. When I did some testing I found one of the motors stalled out much easier when gripping it by hand with a glove. I figured that it had blown a winding in the motor, but when I took apart the case a surface mount capacitor fell out!
![55869278_10103795161667588_5269281370126942208_n|666x500](upload://62pob5TXC5l51UWfyduCygC8N1k.jpeg) 

I was able to identify where it came from and did a very terrible job soldering it back in (I didn't have a good iron, and it's a tight space). I traced the circuit and this capacitor was on the boot up line of one of the fets, so yeah.. one of the motors was only running on 2 phases, it rides sooo much better now! Curious if this happened while I was riding it due to vibration, or perhaps this is why it was on sale.... The built the board and individually all of the components passed through QC, then when they went to test ride it there was a problem so they took that batch and sold it to a liquidator?

A lot of speculation..

Anyways I have a plan to replace the antennas on the remote and receiver with higher gain antennas. 5db for the receiver and 3.5 for the remote. Fingers crossed.

If the remote problem can be fixed, I'll be pretty pleased with my purchase actually. Just so you know I've already got a bunch of other parts for a DIY build... caught the bug so fast! This is a cool forum I love the pictures only thread! :slight_smile:
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-04-08T02:05:16.287Z Reads: 128

```
Well, the forum also has a search feature thats pretty useful

I searched Nuff and this is the first thing that came up
https://www.electric-skateboard.builders/t/nuff-replacement-hub/85694

A thread in which a user of a Nuff board had a hub issue, and Nuff tried to charge his 200+usd to send him a new motor. 

When dealing with Nuff you'll be dealing with shady flippers who likely buy B grade rejects from a factory and upcharge you significantly

Nuff? more like Nutt(z)

Safe your money though, seriously. Its not worth it.
```

---
## \#3 Posted by: J0ker3366 Posted at: 2019-04-08T02:19:40.150Z Reads: 115

```
Nuff said.
```

---
## \#4 Posted by: bluegreen Posted at: 2019-04-08T02:20:25.057Z Reads: 114

```
Yeah I had seen that post too, but I suppose based on his experiences it could theoretically have just been a capacitor issue like mine. I design hardware electronics for a living so it's kind of like an investigation into manufacturing cost cutting. I'm curious what will blow up, don't worry I wear a lot of safety gear when I ride ;)

And as I mentioned, I'm already in the process of building my own board now. When the parts show up I'll start a build log. I'll have to warn you that build is kind of similar, I'm going to start by using some cheap parts expecting to have to repair and replace them along the way, as this is primarily a learning experience for me.

So I guess I kind of meant to make this post so that more people googling Nuff will know the real truth, because it actually took me a while to figure it out. But because of the price I was actually expecting it to show up DOA, so the fact that it even worked at all out of the box was a pleasant surprise for me :laughing:

[quote="J0ker3366, post:3, topic:89756, full:true"]
Nuff said.
[/quote]

I should have taken a picture but that was actually on their box it said something like "The best electric skateboard. Nuff said." :joy:
```

---
## \#5 Posted by: bluegreen Posted at: 2019-04-09T07:41:35.323Z Reads: 86

```
Opened it back up:
![20190408_170535|666x500](upload://mtKWcWkLX3JYl20vpV0eyc7yzfu.jpeg) 

The antenna is buried under phase cables and is bent 90 degrees against the case, this is not optimal placement.

![20190408_171815|666x500](upload://mTU9zZIjqQg6Ai5wpx3hMCRjLjZ.jpeg) 

This reciever has the common 27mm whip antenna, which isn't as good as 31.5mm. I'm not an RF engineer, but from what I do understand combined with speculation is that the series capacitor balances the difference and also keeps the DBi intentionally low so it is easier to pass FCC emission tests. I am guessing. Also there is no RF can, which is just an insane level of cost cutting.

![20190408_170552|666x500](upload://8vUbYH0CO2snBCGzu9PcNSoyhfD.jpeg) 

This is the antenna, there is actually a chance it might fit in this remote after all... but this one is going on the receiver.

![20190408_173214|666x500](upload://sYEtJq0OgglZvv1yAiDMyLAVcgf.jpeg) 

I stripped off the UFL connector and scraped off some soldermask on the ground plane to attach the shielding to.

![20190408_173641|666x500](upload://mG9Pdj0Gpo8lVyHIyeLSz7OSohv.jpeg) 

Completed.

So, I put it all back in like normal and was getting no connection at all. I was pretty upset. Then I poked the receiver and it flicked to life for a second. I was getting all sorts of different behaviors depending on when I wiggled the connections, so this was obvious there was a cold solder joint on the bottom side of the pin header. So the receiver was soldered to the pins, but the pins were not properly connected to the motherboard.

![20190408_203234|375x500](upload://waMHciLsM8RNBgqU2PoPGn0ZBsM.jpeg) 

After putting it all together, the reciever worked, but it was unable to sense the battery. The entire pad had gone dead, I must have damaged the trace on the bottom side with all the soldering, so I found another switched 42v source and wired that in.

I think the bad solder joints might have actually been the disconnection problem, not the wireless potentially. It's for sure possible.
![20190408_204812|375x500](upload://pj8dByc5z0UtbHb9HyL15XjwHRE.jpeg) 

It is raining, so I cannot test it outside but I do still maintain a connection if I leave my apartment, shut the door and start to drop after 2 doors down. I got too excited when I got the antenna to remember to do a before test, but... at least it works.

Bonus pics: I didn't wait long enough for the capacitors to discharge and was careless on which wires I was snipping together...

![20190408_230102|666x500](upload://plLN6MM8rE49P1wicBZ817L9YOa.jpeg) 

And now my angle cutters are wire strippers! :zap:
```

---
## \#6 Posted by: bluegreen Posted at: 2019-04-09T23:20:41.082Z Reads: 69

```
Happy to report the antenna upgrade on the Nuff board completely solved the connection problems.

Only problem I've got with the board now is that sometimes the battery goes what I'm guessing is overcurrent protection on the BMS. If the battery is fully charged the ESC can draw enough current in some strange conditions. It's pretty obvious the ESC is programmed very poorly, and this is the real true downside of these boards is that even if you win the lottery and nothing breaks on it, it still struggles.

I'll come back to this board at a later date and try to extract the hex file and decompile the code to see if there is anything obvious or easy that could be changed. I'm hopeful to understand the code as these ATmega chips are cousins of the 328p that are used in the Arduino uno, meaning there is a wealth of knowledge about working with these chips.
```

---
## \#7 Posted by: JohnyEvil Posted at: 2019-04-10T14:51:16.219Z Reads: 66

```
It is my beater board. I have a Halo 2 Edition as well as an Ownboard and a Chinease dual belt that goes 32mph. Custom Ownboard picture attached.![20190406_092903|666x500](upload://ndhzlCSOQg8UywPE2RPQaajcefh.jpeg) ![20190406_092903|666x500](upload://ndhzlCSOQg8UywPE2RPQaajcefh.jpeg)
```

---
## \#8 Posted by: bluegreen Posted at: 2019-05-14T00:30:07.198Z Reads: 55

```
Opened up the battery.

Samsung 24R cells, not too shabby! Unfortunately I think one is bad because the pack voltage won't charge more than 40.2 volts.

How do I go about testing the packs? Just measure positive to negative between each pack? Like I was testing just 1 normally? Does it make any sense to try and do it through the balance connector or should I do it from the end of the battery. Either way looks like I need to do some disassembly to get at all of them.

![20190513_172504|666x500](upload://2oMCoUcyM9C9NcgronJ389VWSQm.jpeg) 
![20190513_172453|666x500](upload://jMrmEseYuG89K5HIh8rYpwgWwZ1.jpeg)

Yo @City-Blade-101
```

---
## \#9 Posted by: City-Blade-101 Posted at: 2019-05-14T00:47:40.430Z Reads: 54

```
Yeah, got an bursted battery pack at hand, too and disassembled it.
In there are 22P cells not like in yours 24R but anyways.
I read a thread about measuring the packs and i am pretty sure you have to measure without the bms in between to get the right result.
```

---
## \#10 Posted by: bluegreen Posted at: 2019-05-14T00:55:45.474Z Reads: 54

```
Oh really? Ok I'll try to do some more reading. I measured all the P groups with the BMS still attached and they all came back the same. The pack is discharged right now at 3.68v so I will try charging it back up and see if the cells are still even. Maybe the BMS is bad.

I think the other pack I got came with LG cells so I don't think I could easily combine them to a 10s4p but that would be sweet if I could.
```

---
## \#11 Posted by: City-Blade-101 Posted at: 2019-05-14T00:57:18.236Z Reads: 53

```
Yeah, not an expert at battery builds, but i think i have read it these days in here somewhere My pack bursted because of I don't really know if water was in or if a nickelstrip broke, but 80% i think of condensation was the cause.
Edit: I think its not a good idea to combine differnt cells to one pack, though.
```

---
## \#12 Posted by: City-Blade-101 Posted at: 2019-05-14T01:03:08.442Z Reads: 55

```
![20190221_101058|281x500](upload://3NAxNjXlT468UuOryCSMulSuhQA.jpeg) ![20190221_101104|690x388](upload://4Yhhyide87eiixJoWOn0bmxiH3.jpeg) ![20190225_125945|281x500](upload://eo1XCgBZC45DynGoBq2xeOyuXsx.jpeg)
```

---
## \#13 Posted by: City-Blade-101 Posted at: 2019-05-14T01:30:14.378Z Reads: 50

```
The new models dont have any antenna and work perfect.
```

---
## \#14 Posted by: bluegreen Posted at: 2019-05-14T04:06:04.714Z Reads: 49

```
Just leaving it on the charger after the green light says its "done" has so far got it up to 41 volts, so maybe the charger is just weak and has difficult pushing amps into the last 90% of the battery.

EDIT: Nah it wont go over 41 volts, The P cells look fine. Either the BMS is detecting some other condition, like too much resistance maybe? So just maybe a shitty BMS? It looks smaller than the one you've got.

DOUBLE EDIT: There is for sure a bad cell in there, it's just only kind of bad. Voltage has dropped down to 40.8 in the last few minutes. I'll have to take the whole pack apart and capacity test all of them to find the culprit. :expressionless:
```

---
## \#15 Posted by: City-Blade-101 Posted at: 2019-05-14T12:54:39.186Z Reads: 39

```
yeah its a good thing to leave the packs charging for a few hours more when they fully charged because cell balancing starts then.
```

---
## \#16 Posted by: bluegreen Posted at: 2019-05-15T00:46:52.433Z Reads: 34

```
Ok so I what is happening is if I disconnect the balance wires, and the reconnect them it seems like I can fully charge to 42v however as soon as the charger stops whichever dead cell is there absorbs the balance charge until the pack voltage drops down to 40.7~40.8ish. It would seem like the BMS is remembering this and it is a protection to stop charging at that voltage the next time it is charged.

So disconnecting the balance wires seems to reset the BMS logic.

Right now I just charged it up to as close as I could get 41.7 and then disconnected the balance wires. I'll let the cells alone for a couple days hopefully one of P cells will be at the lower voltage and the rest of them will still be at 41.7.
```

---
## \#17 Posted by: City-Blade-101 Posted at: 2019-05-15T01:01:44.653Z Reads: 34

```
Mhh..good idea so far. hopefully it works like you want it to.
Is there no chance for you to locate the maybe dead cell without disassembling the whole pack?
```

---
## \#18 Posted by: bluegreen Posted at: 2019-05-15T01:06:15.053Z Reads: 32

```
If one of the parallel packs self discharges on it's own at least I'll be able to narrow it down to 2 cells. That will help immensely because then, yeah, I won't have to rip the whole thing apart.
```

---
## \#19 Posted by: City-Blade-101 Posted at: 2019-05-15T01:08:38.033Z Reads: 34

```
sounds good, 15 dollars and some hours of work and you are good to go.
```

---
## \#20 Posted by: bluegreen Posted at: 2019-05-15T01:10:42.362Z Reads: 34

```
Yep, also looking at 20 30q cells on ebay also ;)

I think maybe I will try making a pack. No spot welder though would just be with solder, but from the research I've done as long as you are careful to not overheat the cell this is just fine.
```

---
## \#21 Posted by: City-Blade-101 Posted at: 2019-05-15T01:12:19.362Z Reads: 32

```
ouuuu, every professional battery freak in here warns about that.
I wouldn't do it this way.
```

---
## \#22 Posted by: bluegreen Posted at: 2019-05-15T01:31:16.518Z Reads: 30

```
I don't think anyone selling their pack should do it, but I also don't think it is worth $100+ if you already have a good soldering iron and know what you are doing.

I'd ruin a bunch of cells just trying to figure out how to use the arc welder...

I guess lots of people in the forum are in SF have a spot welder maybe I can get their help..
```

---
## \#23 Posted by: City-Blade-101 Posted at: 2019-05-15T01:36:21.807Z Reads: 31

```
Original onan battery pack is 89 dollars hahahaha, but anyways, its your decision. But let me give you the only advice i can give you: if you need 20 cells order a bit more, but it is always possible to get a dead cell right out of the box.
I read it many times in here:wink:
OH, you're from San francisco?:wink: thought you were an australian but maybe i confound you with someone else.
```

---
## \#24 Posted by: bluegreen Posted at: 2019-05-15T01:54:11.978Z Reads: 33

```
This was an original onan pack! from ebay anyways.

Weird after a few hours these are the results. It kind of looks like maybe the first two cells are lower capacity than the rest, so they get fully charged before the others... stopping the charge and then it balances out to 40.8?

1. 4.22
2. 4.22
3. 4.18
4. 4.16
5. 4.16
6. 4.17
7. 4.19
8. 4.19
9. 4.19
10. 4.17

Doesn't seem right, is the BMS just fucked?
```

---
## \#25 Posted by: bluegreen Posted at: 2019-05-15T05:15:46.289Z Reads: 34

```
Reset the bms again and charged it for about another hour...

|cell|before|difference from max|after|difference from max|change|change in difference from max|
|---|---|---|---|---|---|---|
|1|4.22|0|4.26|0|0.04|0|
|2|4.22|0|4.26|0|0.04|0|
|3|4.18|0.04|4.2|0.06|0.02|0.02|
|4|4.16|0.06|4.18|0.08|0.02|0.02|
|5|4.16|0.06|4.18|0.08|0.02|0.02|
|6|4.17|0.05|4.2|0.06|0.03|0.01|
|7|4.19|0.03|4.22|0.04|0.03|0.01|
|8|4.19|0.03|4.22|0.04|0.03|0.01|
|9|4.19|0.03|4.21|0.05|0.02|0.02|
|10|4.17|0.05|4.21|0.05|0.04|0|

It kinda just looks like a poorly matched pack. Cells 1 and 2 appear to be a lower capacity than the rest causing them to get charged first and continue to accept more charge. Or the BMS is broken or just plain sucks.


Is less than .1 volt even something to worry about between packs?
```

---
## \#26 Posted by: City-Blade-101 Posted at: 2019-05-15T10:44:14.168Z Reads: 33

```
don't really know if its to worry about, but what could happen in a worst case scenario? It will not blow up anything on the esc or something i guess, the pack just is not as good as it should be.
```

---
## \#27 Posted by: bluegreen Posted at: 2019-05-15T23:27:12.633Z Reads: 30

```
![20190515_161528|666x500](upload://yVGNlbwLmb7EMqfz6gZti8iYQHj.jpeg) 

Manually balancing cells with a taken apart usb flashlight.

The protection board from the lipo is taken out to prevent over or undervolting. The light turned on discharges the cell (very slowly .5A red 1A white) and then plugging a usb in will charge the cell (very slowly .5A).

Going to get all the cells the same and go through a power cycle and see what happens. I think this BMS doesn't actually "balance charge" to match cells, it just "balances the charge" while it is charging as best as it can and if one cell hits 4.2 then it stops. But if the cells are out of balance then the pack won't ever hit 100%
```

---
## \#28 Posted by: City-Blade-101 Posted at: 2019-05-16T00:45:22.549Z Reads: 27

```
yeah this is crazy, hopefully you get the right result you are looking for.
isn't it possible to skip the bms, like you did, and just use a better balance charger instead to get them cells all the same voltage?
```

---
## \#29 Posted by: bluegreen Posted at: 2019-05-16T06:36:42.470Z Reads: 26

```
![20190515_205121|666x500](upload://cVDwBU88ITHaCbwJ9esCvY4CXbL.jpeg) 

Hopefully I got it! I manually balanced all the cells to 4.15~4.16 and then charged it up the rest of the way with the 42v through the BMS. I taped it back together and heatshrink put it back together for testing as soon as it stops raining!

So yeah, I think the bms is just a "balance charger", but not an "active balance" meaning it will try to distribute the charge between the cells but once any one pack reaches 4.2 it stops instead of topping the rest off.

Oh yeah I also cut some of the fiberglass between the cells to make space for the wires, they were getting pinched.
```

---
## \#30 Posted by: City-Blade-101 Posted at: 2019-05-16T11:44:34.979Z Reads: 21

```
looks good man, maybe you did it...another option is to get just another bms instead to avoid the problems you got with the chinese one.
```

---
## \#31 Posted by: City-Blade-101 Posted at: 2019-05-19T12:08:06.797Z Reads: 19

```
Did some experiments and mock ups with parts i have and a totallly diassembled x3...still forced from inside to follow my plans...i want a board with cheap hubs i can treat hard( so wasting and changing them dont needs a bank robbery at all...My first goal is to match it with the onan battery packs( which will be hacked later on).
second i want an integrated charger, so i just have to carry a dc conector in my pockets😀
Anyways...this is not a build thread and i think i run out of topic a bit but maybe im in with that, who knows.
![20190517_192313|281x500](upload://3k5eVuCyZ7M86IkvlOyjns8yf2J.jpeg) 
![20190517_192402|281x500](upload://fHARrIFNdFVOYHug58C4iqCDzro.jpeg)....
Edit: these are X2 hubs  ( will hack them next, and show up in here, still waiting on parts)😀
```

---
