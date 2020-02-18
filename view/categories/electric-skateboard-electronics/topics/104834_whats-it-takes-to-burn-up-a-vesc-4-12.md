# Whats it takes to burn up a vesc 4.12?

### Replies: 42 Views: 575

## \#1 Posted by: cskarke Posted at: 2019-12-19T18:01:34.723Z Reads: 123

```
Hey there, new to the esk8 world and I have some uncertainties on how exactly I should set up my current/amperage parameters for my specific build. Building a mountain board on a slimmer budget so the last thing I want to do is burn something up when I could have easily prevented it. 
Build components:

-FS vesc 4.12 50a cont. 240a peak

-7s4p li-ion 8ah (2 hoverboard battery packs in parallel, not ideal but dirt cheap with a built in bms and will be upgrading later)

-180kv 6354 1920w 80a max sensrd unbranded Chinese  (figured I could get away with running way under the max amps to greatly reduce risk of burning up my cheap motor) 

-16t pinion pulley

-72t drive pulley

200mm (7.9 inch) off road pneumatics

I know its not the greatest set up and definitely not a performance set up but its all that budget will allow for the time being. I do have a second identical vesc and motor in the mail on its way so will be doing a dual drive set up mainly for off road traction purposes. But the main thing I want to know is how many amps can the vesc safely handle? Im just unsure because the advertised 240a peak really throws me off. Im more familiar with the RC world that has advertises esc's with burst current ratings for a set amount of second of burst at that current that the escs can handle but they are never 5 times the max continuous like with the 4.12. I dont want to limit my vesc to 50a if it can handle way more than that. Aslo, is that 50a rating referring to the battery in current or the motor out current? 

Ive done some flat ground testing with what I think is a conservative set up but I want to know very clearly what the line is so that I never cross it. 
Here is the setting for my initial tests with only 1 motor and vesc:

Motor max 50a

brake max 30a

absolute max 130a

battery max 35a

regen max 15a

I just left temp settings at default, I think 80c start 100c off for mosfet

*recommended settings for all would be greatly appreciated.

I was surprise at the performance considering my settings so I believe with another motor and vesc and also with turning up the power to what it can really handle, I wont need much more performance for a long time to come other than a different battery. I got up to 18 mph, which I dont think I'll want much more speed with an off road board anyways, brakes were slow but I know I can turn up a bit, just didnt want to go flying for the first ride. And nothing got even remotely hot.

Last question for this thread, Has anybody played with installing heat sinks to their mosfets and could that greatly improve performance and lower the risk of burning something up? If you have heat sinks can you over amp your vesc a bit more as long as the temperature settings are correctly set and catch it before anything gets hot? Just thought it was crazy that nearly every RC esc comes with a heat sink and fan but these 4.12 vescs dont initially need them and they are moving much heavier objects. 

Thanks in advanced. I hope this is not too much information on one post at one time.

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/b/3/b3a3a593dd2148493917341cadef80deca3854a8.jpeg)
```

---
## \#2 Posted by: Anubis Posted at: 2019-12-19T18:21:39.226Z Reads: 107

```
On 7S you should be pretty safe with a 4.12. I wouldn't bother bursting to 130, just leave it at 50 and if it feels underwhelming then slowly move it up. Your regen max is way, way too high if thats per side then -30 amps into a 4P battery will destroy it. 
You want about -6A per side or if you only have 1WD then -12. 

Again if you're using hoverboard batteries they'll be a massive bottleneck, you can only use about 20 battery amps per side.

Given that a 4.12 ESC is only about $40, its not worth trying to overclock them for better performance, it just creates a potentially unsafe scenario and will cost enough that you should have just gotten a better one. RC ESCs run at about 4S, 150 amps, and its amps that causes the heating. At 50 amps its not as much of an issue
```

---
## \#3 Posted by: cskarke Posted at: 2019-12-19T19:04:37.464Z Reads: 103

```
@Anubis No I currently have the 2 hover board batteries with a parallel connector going to 1 vesc. So it was only feeding -15 amps to both, -7.5 each. I'll bump it down to 12 though, thanks for letting me know that. I didnt ride hard so I doubt I hurt anything. And if I understood correctly, I can pull 20 amps off each 2p battery pack? So 40a total since I have 2 2p in parallel? Or just 20amps off a 4p pack? 

And yeah Im going to upgrade batteries as soon as possible, I purchased the entire hoverboards for 25 dollars each "needing new batteries", I knew they were just over discharged from sitting unused too long so I just by passed bms to just high enough voltage so that the bms would take back over and do the rest of the balancing.

Btw, Is that 40$ usd for a 4.12? if so whats your source?? I spent 60 usd on mine from china!
```

---
## \#4 Posted by: Anubis Posted at: 2019-12-19T22:42:45.365Z Reads: 90

```
In the UK we get super cheap 4.12s, they're as low as £36 on ebay which depending on the status of brexit fluctuates between 42-46$, and that's shipped from the UK and taxed :smiley: 
20 amps per pack so if you're only using single drive then yea 40 amps max, some of those hoverboards use a 12 amp bms though so better to check maybe. 
And yea, max 2~3 amps regen per p group, so no more than 12 amps back into a 4p pack. Remember, max regen doesn't effect how hard you can brake, only the energy the vesc will recover.
```

---
## \#5 Posted by: cskarke Posted at: 2019-12-19T22:47:27.010Z Reads: 81

```
Ok cool! thanks for the help man. I just discovered batteryhookup.com and will probably be making a battery purchase from them pretty soon. Stupid cheap resale fully tested cells and packs! And yeah Ill check on that bms
```

---
## \#6 Posted by: Fosterqc Posted at: 2019-12-19T22:50:39.772Z Reads: 81

```
NICE!

I have a $260 order halfway here pending delivery estimate. I also got a KWeld to begin serious battery construction. 

Also I burnt my VESC 4.12 PCB on 6S due to a high KV+A motor, so watch out for that. It was perfectly fine with the same motor on 12S, lower V = more A = not good.
```

---
## \#7 Posted by: cskarke Posted at: 2019-12-19T23:00:50.871Z Reads: 74

```
@Fosterqc Oh sweet! What will the specs be on your battery?
```

---
## \#8 Posted by: cskarke Posted at: 2019-12-19T23:11:17.916Z Reads: 72

```
Do you by chance know the best way to figure out how many amps my bms is rated for on these packs? No specs online have said a thing about that. Its a jettech 25.2v
```

---
## \#9 Posted by: JohnA Posted at: 2019-12-19T23:15:11.242Z Reads: 71

```
Beware on the battery hookups 9s ATL packs. I got 21 of them and 14 arrived completely DOA with no good cells. (Of the good cells I’ve tested all are 2850-3050mah). They are replacing 6 of them though, and the cases and BMS’s are legit.

I have been stress testing them and they are very high quality cells. 10 amp charge, 20 amp discharge, 5 cycles Without puffing and only get warm on the discharge. Under 10 amp load 0.1v voltage drop observed and no noticeable warmth generated. Tried charging to 4.5v then draining completely and it and they puffed to 160% of the original size but no warmth or signs of failure. Did a capacity test and still at 1800 mah. Then when fully charged I punctured with a BB gun and they didn’t even smoke with a gaping hole in the pouch. And still was able to output 10amps shorted through my damn and held voltage at 3.85v for hours. So I think they are way safer then LiPo pouches and pretty cheap for a nice pack if you go that rout instead of 18650’s. 

(Making a 12s 9p ebike battery with them. 1.2 kWh for under 250 all in). 

Battery hookups is a good company, fast email reply’s and good shipping times.
```

---
## \#10 Posted by: cskarke Posted at: 2019-12-19T23:25:13.508Z Reads: 66

```
@JohnA Man I just found those flat packs and was blown away at the price of them! On sale for 4.99 each! I couldn't find the discharge rate anywhere and that was the only thing worrying me so thanks for answering that for me! Is the bms rated for 20a dischage or just the cells? 

If the shipping wasn't as high I would have bought 6 of them already! I think a 9s4p would suit me quite nice for the time being.

Dude 12s9p!? What kind of range you think you'll get with a 25+ah battery??
```

---
## \#11 Posted by: JohnA Posted at: 2019-12-19T23:31:24.038Z Reads: 63

```
The BMS is only rated for 10 amps discharge. (And assume the cells are too, i did 20 amps to test the limits). It also uses a TI chipset in the bms that works for 6-9s packs do you could wire two in series for a 12s battery. 

I’m hoping for a 40-50 mile range on my ebike without pedaling. But we will see. If you go this route too, look into closed cell polyurethane foam. Pouch batteries work best under some compression force and also can “breathe” 5-10% in normal charging and discharging use. so you wanna make sure your pack has room for this, and when the batteries eventually puff.

Pretty easy to disassembly cleanly, can give tips if you end up buying them. 
![image|666x500](upload://e3xXv3EyCUBHJmrsdcbHfWEFboD.jpeg)
```

---
## \#12 Posted by: cskarke Posted at: 2019-12-19T23:42:31.150Z Reads: 61

```
Ok gotchya! Well thanks a bunch for the tips already! If I end up getting them I will defiantly holler at you if I have any questions! Seems that you've done your homework and know your stuff quite well!

That would be incredible to get that kind of range with no more than your battery cost you. Unbeatable dollar per mile. I hope to build a bike one day, I have the great palo duro canyon basically in my back yard and have always dreamed of rippin down the trails on a e-mountain bike.

Are you using the Included bms's that the packs came with and doing a 6s in series +9p type set up or different bms all together?

Also, how thick is a single cell?
```

---
## \#13 Posted by: JohnA Posted at: 2019-12-19T23:54:25.049Z Reads: 58

```
No problem, I wasn’t able to find any info on them myself so I wanna do a full write up after i finish my pack with all of the tips and tricks I’ve discovered. Most of the research I’ve done has been on this forum or the other new one. 

I’m currently planning on making two 6s9p batteries, each wired to one of the BMS’s. And then those packs in series. Im also thinking about modding two 24v chargers to be together in one case with one output so that I have a 4 prong cord that can charge each pack separately but at the same time. I also wanna have an extra balance plug wired in so I can connect my hobby charger to if I need to active balance the packs ever. Most bms’s on the market have like a 50-100mah balance current that barely does anything for high capacity packs, I just want it for the over charge cell protection.
```

---
## \#14 Posted by: JohnA Posted at: 2019-12-20T00:56:26.387Z Reads: 52

```
Single cells about 4.3-4.4mm thick from the ones I measured. Out of 10 cells the mean was 4.34mm thick. 

The WxH dimensions are roughly 64mm by 89mm
Or  2.5 by 3.5 inches.
```

---
## \#15 Posted by: cskarke Posted at: 2019-12-20T01:42:16.978Z Reads: 49

```
Appreciate it!
```

---
## \#16 Posted by: Fosterqc Posted at: 2019-12-20T03:14:53.955Z Reads: 49

```
Shame they had a lot of dead cells. I got two I was hoping to use as portable charger.
```

---
## \#17 Posted by: JohnA Posted at: 2019-12-21T00:44:09.553Z Reads: 48

```
@Fosterqc I told them about the dead cells and they were happy to replace a couple. They said they weren’t aware some were completely dead, and that they have multiple pallets of them so it’s too many to go through. I had good luck “waking up” the dead cells, with low current from my lab supply. (I’ll run a capacity test on a few of the dead ones and reply back). I’m not sure how they will hold up long term, or how many cycles they can do before they puff though, being they say dead for so long.
```

---
## \#18 Posted by: cskarke Posted at: 2019-12-21T02:18:23.606Z Reads: 46

```
@JohnA Well I think it's worth the risk since they're so cheap. Glad they were willing to replace a few if them for ya!

When I revived my hover board packs they were about .3v per cell (i know, scary) and now I'm getting about 7 miles per charge on an inefficient mountain board. Original rated total ah would be 8ah but I have no idea how many amp hours I'm actually getting out of them since my hobby charger/discharger only goes to 6s. But I was surprised they are doing as well as they are with no dead cells so far! 

I have a question for you though, have you experimented or ever heard of deep freezing over charged lipos to revive their capacities? I've watched a few YouTube videos but nobody that I can find has done a detailed experiment by physically measuring amp hours so idk if it's legit or not. Definatly makes me want to do my own experiment.
```

---
## \#19 Posted by: Fosterqc Posted at: 2019-12-21T06:14:40.801Z Reads: 46

```
![Snapchat-582313043|281x500](upload://zwg6yxxvQ33279MKBATeEBbqO4.jpeg) 
The ATL packs look well built. 

I'm going to use them as CNR for my Onewheel. I wonder how much of a hit they could take
```

---
## \#20 Posted by: JohnA Posted at: 2019-12-21T07:19:06.598Z Reads: 44

```
@cskarke I haven’t really experimented with freezing the packs for capacity gain. But I did try freezing a puffed cell that I overcharged to 4.5v. Before the freeze the aluminum bag was fully inflated and after 24 hours it lost about 30% of its thickness. After the tests it went from 2879 mah to 1800 mah. I would be interested to see if it could help revive the capacity though. 

If you plan to disassemble or remake a pack, keep in mind one of the electrodes is aluminum so you either need aluminum solder or to spot weld nickel strips to the battery to solder to. This solder from amazon works very well on soldering wires to the cells. Aluminum Solder Wire 96.5 Sn/3.5Ag .062 Flux Core https://www.amazon.com/dp/B00DC3102Y/ref=cm_sw_r_cp_api_i_pDC.DbYEEH6MY
```

---
## \#21 Posted by: Schulerbible Posted at: 2019-12-21T09:06:40.487Z Reads: 40

```
12s and FOC
```

---
## \#22 Posted by: cskarke Posted at: 2019-12-21T13:45:37.543Z Reads: 41

```
@Schulerbible 12s FOC burns up vescs? I keep getting told that high voltage has less chance of burning stuff because of the lower amps.
```

---
## \#23 Posted by: cskarke Posted at: 2019-12-21T13:47:37.559Z Reads: 38

```
@JohnA You just saved me some serious time trying to figure out how to solder to aluminum :joy:
```

---
## \#24 Posted by: cskarke Posted at: 2020-01-07T00:33:08.291Z Reads: 37

```
@JohnA  Just got 10 ATL flat packs delivered from Battery Hookup. About to do some testing to see if what they sent me is any good! I think I'm going to build a 10s pack out of them and buy a separate 10s BMS for it and bypass the bms for discharge. Probably will do 5 or 6p depending on how much space I end up with. You know if cheap Chinese bms's are worth it? I thought about doing the 6s in series with the included bms's but 12s would put me at 34 mph at my current gear ratio and I don't want to go anywhere near that on my mountain board yet. Also didn't know if I was more likely to burn up a 4.12 with higher voltage, Ive had some mixed feed back on that.

I would love to hear how your flat pack project is going or if you've made any progress on it yet!
```

---
## \#26 Posted by: cskarke Posted at: 2020-01-07T02:11:47.004Z Reads: 36

```
@JohnA Any tips for disassembling packs? I got one cell off a pack so far but it was a fight. I just cut the foam separations with a razor knife and cut the cell terminals with a razor but I feel like there should be a safer way that's less risky of shorting something.
```

---
## \#27 Posted by: JohnA Posted at: 2020-01-07T06:34:15.923Z Reads: 40

```
@cskarke I personally wouldn’t trust the cheap BMS’s, if they do something wrong it can be a fire hazard so I think it’s worth buying something from a good brand like supower or bestech. I’ve tried 7 or so of the BMS’s included with the ATL packs and I can’t get one to work with my 6s pack. Not sure if the BMS’s are mostly bad or I was doing something wrong...

Basically what I did was put the packs in my lab oven for a few hours and heat them to 100F, then take them out and use a heat gun to remove the metal sides to minimize the lifting of the aluminum cell pouch. I then took a old gift card and sanded it down making Into a sharp knife and used that to cut the foam and help split the clear adhesive. I would be worried with a razor blade about puncturing the cells. Beyond that I take some edge cutters and pry and roll the top plates one by one and the cells drop out the bottom. Once they are removed one by one it’s hard to short. It’s hard to describe the last part so I’ll try and post a video tomorrow. Also check your voltages, possible most are 0v asleep so don’t worry much about shorting 

Here’s half of my ebike battery, and some of the assembly pictures. Using foam to apply a constant pressure to the cells and also allow for expansion during charging. I noticed that most of the cells expand .1-.15mm or so when cycling 3-4.2v. 
![image|666x500](upload://x8VOobzK25xJFsRno8QO5Ey519m.jpeg) ![image|375x500](upload://ha8EFtQB0lKIRKEun4MjN7E7xVs.jpeg)
```

---
## \#28 Posted by: cskarke Posted at: 2020-01-07T15:33:02.263Z Reads: 35

```
That's lookin awesome man! And gift cards are a good idea! The razor was making me nervous, I was super cautious but got a few of them out. Out of the 18 cells I've tested so far, 16 of them have been at 3.5-3.6v and 2 have been at 0v. That makes me pretty optimistic for the rest, but we'll see.
```

---
## \#29 Posted by: JohnA Posted at: 2020-01-07T16:50:07.271Z Reads: 36

```
@cskarke thanks brother. Yeah the card sounds like a safer bet. Sounds like you got some good packs though, only 14 of the 26 I ordered had voltage, the rest were 1v or less for the whole pack. But some are able to wake up and have a decent capacity still.
```

---
## \#30 Posted by: cskarke Posted at: 2020-01-07T17:31:42.611Z Reads: 35

```
So that's what I thought as well. I checked all my pack voltage out of the xt60 and only had 2 packs above 5v, the rest were <1v. I thought they were all toast..Then I opened the pack that had the lowest voltage and tested each cell and I was getting 3.5v on all but 1 cell. Seems like the BMS was shutting down the whole pack output due to 1 bad cell. You may want to check all of them again if you havent checked voltage directly off the power distribution board. That may be why you cant get the bms to work for your 6s packs, it might think you have dead cells.
```

---
## \#31 Posted by: JohnA Posted at: 2020-01-07T18:04:38.840Z Reads: 31

```
@cskarke nah, I fully disassembled all of my packs and already measured each individual cells voltage. I musta just got a little unlucky with the packs they sent. My last order I ordered 5 more and all were dead, no cells over .5v. And two were totally puffed. CS wouldn’t do anything about it either, they just replied they are salvage packs

And for the BMS not working, I looked up the TI controller on it and it’s supposed to work from 6s-10s, wired it all up correctly and no dice: they just got warm after being connected to the battery.
```

---
## \#32 Posted by: cskarke Posted at: 2020-01-07T18:40:56.019Z Reads: 32

```
Dang man you got screwed. So you have enough good ones to make it work or you gunna have to roll the dice and order some more? Now I'm anxious to test the rest of mine.
```

---
## \#33 Posted by: JohnA Posted at: 2020-01-07T20:03:46.158Z Reads: 34

```
@cskarke I was able to make the 6s9p I shared earlier with all good cells, and I have 3s of the second battery. But now I’m forced to go through each cell and cycle them to determine capacity. I’m seeing some are good and test 2900mah or higher but some test lower then 2400. All of my good cells that came with voltage have been testing 2900-3100 mah. But the long term stability has yet to be seen. The most I’ve cycled any is 10 times. I’ll prolly end up picking one bad cell by mistake that destroys my whole pack.

I will say, do a really good physical inspection of them. Any looseness in the internal laminations or any gas inside the cell alludes to them not being stable. And I’ve had ones that look perfect externally but test kinda low
```

---
## \#34 Posted by: cskarke Posted at: 2020-01-14T23:58:04.687Z Reads: 27

```
@JohnA ![20200114_175147|375x500](upload://fIctEW1eegVKyg1w9WV8UL7r0DG.jpeg)  I really really didnt want to spend 35 bucks on aluminum solder and I'm not extremely confident in soldering unfamiliar materials so I quickly whipped up this spot welder from my motorcycle battery and a relay. I have 10ft of nickel strips laying around anyways. The spot welds are legit and hopefully the relay will hold up through all 60 cells that I plan on tying together.
```

---
## \#35 Posted by: JohnA Posted at: 2020-01-15T01:07:55.365Z Reads: 27

```
How many amps are you gonna try to pull per cell? And what’s your plan for connecting balance or end wires to the batteries? I would be weary of that spot welding setup... But if you are confident them go for it... (maybe add some capacitors for extra performance). That relay shouldn’t last too long.  35 bucks for some extra secure connections might be worth it in the long run, and one roll is plenty to make my 108 cell pack. Are you going to use a good BMS?
```

---
## \#36 Posted by: cskarke Posted at: 2020-01-15T02:11:52.552Z Reads: 25

```
I not 100% on the amps yet but I wont go over 10a per cell (10a per parallel). Will most likely have a 6p pack so I wont ever need 10amps per cell. Right now I'm pulling 30a total from my current pack and already have great acceleration and hill climbing ability so Im sure I'll never even go over 50a total draw. And I realized I have some old 4 wheeler starter solenoids laying around so I will use one in place of my relay. I plan on spot welding nickel strips directly from one positive of a cell to the negative of another cell and then flipping the cells 180° on top of one another. (I'll post a pic once I get started) and I'll just solder the balance leads directly to the nickel strips. And yes, with all this work going into this, I'll find a good bms.
```

---
## \#37 Posted by: cskarke Posted at: 2020-01-17T23:10:33.885Z Reads: 24

```
@JohnA Out of 90 cells, I miraculously only had 7 cells below 3v. Most were at 3.2-3.5v. Idk if I got really lucky or if you got really unlucky.

Quick question, are the blue and white wires coming from the bms supposed to be charging leads or is that some kind of battery cut off? I ask because I had multiple packs with all good cells but none of my pack gave me full voltage out of the xt60 so the bms was cutting off power for some reason..
```

---
## \#38 Posted by: JohnA Posted at: 2020-01-18T01:12:50.448Z Reads: 24

```
@cskarke Hah, good for you, I must have just been very unlucky. I think the blue and white are the charge wires, but haven’t been able to test it. That’s why earlier I was saying that I think the BMS’s are broken, I haven’t been able to get one to work.. like my guess is these packs were scrapped for a faulty bms batch or something.
```

---
## \#39 Posted by: cskarke Posted at: 2020-01-18T20:18:43.752Z Reads: 21

```
@JohnA Yeah I tried shorting the white and blue on a complete and good pack and nothing happened.. I have 2 spare packs I was planning on just using as a remote charge bank but if the bms's are trash then I'd have to build my own pack from scratch with another 10s bms and a dc-dc converter to throttle the amps. 

So are the bms's that you reffered me to able to balance a 6p pack ok? Or will I need more than one to get the job done?
```

---
## \#40 Posted by: cskarke Posted at: 2020-01-27T18:49:39.733Z Reads: 13

```
@JohnA Whats the best way to group together cells based on their capacities? Im making 10 individual 1s6p sub packs and I'll be joining them in series for my 10s6p. So should I group each 6p pack all with similar capacity cells or should I make the total capacity for each 6s pack as similar as possible to all the others. In other words, average out the capacities of each 6p pack so that the bms dosent have to work so hard to balance. 

If all 6 in a pack on the low end were 2700mah and all 6 on the high end were 2900mah then the totals would be 16,200mah on the low and 17,400mah on the high. Seems like a lot of work for a bms. 

I hope that all makes sense, kinda hard for me to communicate what Im trying to say.

Btw, I ordered a bluetooth smart bms that I can set custom parameters on and monitor everything. Its not a high dollar one but ill be able to monitor everything and that gives me a bit more peace of mind while not breaking the bank.
```

---
## \#41 Posted by: JohnA Posted at: 2020-01-27T22:07:46.143Z Reads: 12

```
You'll probably have to look it up to be certain (I've looked and struggled to find solid info).  I personally would group the like MAH with Like MAH. Your idea of making the P groups the same total sounds like it would work on paper. but I can't find anything online to verify it.. I would just be worried about one lower capacity battery being a strain on the higher capacity cells.. your guess is as good as mine though :). if you can check the Internal resistance it might be worth trying to group by that also, that determines more so how the cells will act under load. I probably measured 1/4 of my cells, only the ones that I had to "wake up" and some other randoms to test. I'm interested to see how hard it'll be to keep my 9p pack balanced. 

Cool about the BMS! I ended up ordering one of the XiaoXiang smart bms's for my ebike too. I feel like it'll be a good way to monitor the balance of the pack and also set it up to only charge too V4.0 each cell to preserve longevity.
```

---
## \#42 Posted by: cskarke Posted at: 2020-01-27T22:30:28.318Z Reads: 12

```
@JohnA I'll do some more research then. It just make more sense in my mind to average the capacities but maybe I'm looking at it all wrong. 

What are you charging/discharging with durring testing? All I have are 2 imax b6 hobby chargers and it takes FOREVER at 5amp charge and 1 amp discharge to test all 60+ of my cells. I'm only discharging, charging, and then storage-dischaging. Its takes me a long time and idk how I'd get more than one capacity test in every cell before going insane. 

yea I believe I'll have more capacity than I'd ever want so I was planning on setting my charge and discharge end voltage pretty conservatively to preserve this battery for as long as possible. From what I understand, it dramatically lengthens the life.
```

---
## \#43 Posted by: JohnA Posted at: 2020-01-28T16:29:11.265Z Reads: 8

```
Doing all of your testing on 2 max b6's would suck... I got one of these : https://www.amazon.com/gp/product/B07428G1G2/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1
I soldered some alligator leads on the battery terminals, and then I do the fast test profile. It takes a while because it discharges them at 0.5 Amps to 2.8v (I think thats the cutoff) and then it charges at .5 amps and records capacity. It seems to work really well as far as the cycling and capacity readout, but the internal resistance measurement doesn't seem good enough to be useful (not repeatable). Then after they are charged, I run another fast test, interrupt them an hour and a half in and see if any of the cells dropped weirdly fast or anything. (have had a few that test over 3000mah but some reason most of their capacity is in the 3.2-3.6v range instead of the 3.6-4v range). Lastly I just unplug and group the cells up. 

I would be weary about the 5 amp charge on your Imax. I was doing 5amp to test some cells, and they handled it fine (no warmth or anything), but the lower the current the better. I think its best to charge lithium batteries at 1C so roughly 2.9 amps or so. I believe their original charger was just 1.5-2 amps. It is nice to know though that we can have regen be 5A per cell and they can easily handle it. 

Thats how Tesla is able to get their million mile battery, they only charge up to 80% unless the driver explicitly changes the setting to fully charge for a trip. These cells seem pretty durable though (as far as fire safety), i've destroyed over 10 by now. My last test was over charge to 4.4v and then puncture with a screw. It puffed and smoked but no fire. One of my other cells I fully charged, put between 2 aluminum blocks for cooling and discharged to 2v. after 12 cycles it was down to 1200 mah, but still wasn't puffed over 1.5mm. Hopefully in real world use they last.
```

---
