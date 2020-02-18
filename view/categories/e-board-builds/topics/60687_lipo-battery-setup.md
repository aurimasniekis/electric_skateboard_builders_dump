# LiPo battery setup

### Replies: 43 Views: 3727

## \#1 Posted by: MrDGOrman Posted at: 2018-07-02T09:29:14.164Z Reads: 353

```
Hi everyone,

I'm building my own electric skateboard and the last bits I need are the enclosure and battery. I've got everything else. The battery seems to be the most expensive part of the build and I want to get out on the board now. The weather in the UK is incredible and I want to be out enjoying it!

I'm thinking of throwing in some LiPo batteries in so that I can get out and about. I know I'm not going to have the distance or speed of a Li-ion setup, but it's better than nothing.

Any advice on the batteries I should buy along with a suitable charger? I've got a single Eskating.eu 6374 motor with FOCBOX (awaiting delivery).

Thanks,
Daniel
```

---
## \#2 Posted by: telnoi Posted at: 2018-07-02T09:34:59.320Z Reads: 338

```
Personally happy with 4x 8000mah flight Max (30c). Would not get turnigy nano-tech or multistar or super cheap ebay brands. Anything above 30c should be fine. Anything around or above 8000mah should be fine (even 2x) if you are not going for distance.

If cash isn't an issue, the turnigy Graphenes offer good value when comparing it to other high c lipos.
```

---
## \#3 Posted by: MrDGOrman Posted at: 2018-07-02T09:43:56.327Z Reads: 323

```
Do you have a link to the ones you're using? I'd prefer to go off of a recommendation based on experience.

Thanks,
Daniel
```

---
## \#4 Posted by: MrDGOrman Posted at: 2018-07-02T09:56:48.312Z Reads: 298

```
Found them :slight_smile:
```

---
## \#5 Posted by: Acido Posted at: 2018-07-02T11:13:02.727Z Reads: 286

```
compare how much would you spend on lipos and see what you can get for the same money with a custom made li ion pack
```

---
## \#6 Posted by: telnoi Posted at: 2018-07-02T13:40:16.946Z Reads: 276

```
They are rather expensive now. I bought them for 55 euro via their European warehouse about a year ago with JST-XH connectors. The xt-90 version was 20 euro more expensive. 

They are listed cheaper via the Hobbyking eBay stores as opposed to their official website.
```

---
## \#7 Posted by: MrDGOrman Posted at: 2018-07-02T15:01:02.407Z Reads: 266

```
@acido It's definitely cheaper to buy some run of the mill LiPo batteries than a custom made pack. I've already got a balance charger so all I would need is some newer batteries. I've got some old 1600mAh RC car batteries but I don't want to link loads of them together.

@telnoi According to the HobbyKing website they're £27.61 a pack which seems like a good price. I'll get 2 of them and will use them on a budget board which I can lend to friends when I no longer need the batteries.
https://hobbyking.com/en_us/zippy-flightmax-8000mah-2s1p-30c.html
```

---
## \#8 Posted by: wafflejock Posted at: 2018-07-02T15:13:13.871Z Reads: 252

```
You'll want somewhere in the 8-12S range so will need to link these in series to boost the voltage.   When you link in parallel you add the capacity (mah) but the voltage stays the same (can't connect say 3S to 4S in parallel cause it will dump charge from the 4S into the 3S until all the cells are over voltage, can hook them in series though effectively a 7S).  I use 2 5Ah 5S 20C (turnigy) and don't have any issue but I don't draw a ton of amps either being a small dude on flat land:

https://metr.at/r/GLCvO

For two 5Ah 5S turnigy 20-30C batteries the price of the batteries is around $40-50 a piece so about $100 for 185Wh, compare with a li-ion you'll typically get twice the Wh for three times the price.
```

---
## \#9 Posted by: MrDGOrman Posted at: 2018-07-02T15:42:37.112Z Reads: 236

```
So I think I'll now get 3 of these as they seem cheap and will be perfect(?) for a temporary build:
https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html

Any recommendations on a balance charger where I can plug all 3 batteries in at once and charge together rather than charging them individually? My current LiPo charger requires me to charge individually which is a little bit of a faff.

Thanks,
Daniel
```

---
## \#10 Posted by: telnoi Posted at: 2018-07-02T15:46:13.065Z Reads: 224

```
Balance board should solve that.
```

---
## \#11 Posted by: MrDGOrman Posted at: 2018-07-02T15:58:45.824Z Reads: 224

```
Can't seem to find any bullet connector versions but I presume it's something like this?:
https://hobbyking.com/en_us/hobbyking-parallel-charging-board-for-6-packs-2-6s-xt-60.html
```

---
## \#12 Posted by: telnoi Posted at: 2018-07-02T17:22:13.209Z Reads: 216

```
Yah, you'd just have to solder your own connectors or replace the lipo connectors.

Most balance boards are xt60. I personally soldered xt60 to 90 connectors.
```

---
## \#13 Posted by: CougarKiller Posted at: 2018-07-02T17:35:40.117Z Reads: 219

```
I get 37+ Volts out of my old 3 X 3S set up .. it's comparable speed wise to a 10S li- ion pack.. would go 2 X 6S tho  ![15305528037378739365336611779992|374x499](upload://1o47ZWBFvrCuzMQN9dINylakI8b.jpg)
```

---
## \#14 Posted by: wafflejock Posted at: 2018-07-02T17:54:49.369Z Reads: 215

```
Regarding the parallel charging board might be worth getting the kind with built in fuses to avoid accidentally dumping charge too quickly from one battery to another.  Typically you want the batteries total voltage to be within 1 or 2 **tenths** of a volt when hooking up to the parallel board.  This is the one I use for my quadcopters but only works for 3S or 4S batteries https://www.amazon.com/gp/product/B077N41KJ7/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1 nice side is it has the voltage display built in so just plug in the main lead and I can check voltage on each of them before plugging in multiple batteries.  Personally just using 2 chargers for my 5S (was charging in sequence before getting a second charger, but between the quad and skateboard I need to charge a lot of things).

https://www.youtube.com/watch?v=mRlsaD5tf_8
```

---
## \#15 Posted by: MrDGOrman Posted at: 2018-07-02T19:12:26.159Z Reads: 208

```
@telnoi I thought that would be the easiest solution. I'll do whatever I need to get it working.

@CougarKiller It's good to know what sort of power I'll be getting from this cheaper solution. I'm not massively worried about power levels right now because I just want to get out and play!

@wafflejock I've decided to go with the below option because of the exact reason that the previous didn't have fuses. A small system error could cause a big problem. I feel this HobbyKing option is suitable for the job:
https://hobbyking.com/en_us/hobbyking-safe-40a-parallel-charge-board-for-4-packs-2-6s-xt60.html 

Could someone recommend an anti-spark switch I could use? I don't really want to have a makeshift key. I'd like the setup to be fused in order to prevent damage on the FOCBOX. I'll be ordering all these parts from HobbyKing as it's easier, so if they've got an option then that would be fantastic.

Thanks,
Daniel
```

---
## \#16 Posted by: wafflejock Posted at: 2018-07-02T19:26:42.510Z Reads: 188

```
Cool looks good on the parallel board, still good to check the voltage before you hook them up to avoid blowing the fuses.  Regarding antispark I think the homemade loop key is sort of the only option.  There are a few variations using 3d printed parts and bullet connectors or 3d prints around the anti-spark xt-90 but don't think you can buy ones premade (luckily they're easy to make).  You'll want to have XT-90 male/female connectors anyhow for hooking the batteries in series etc. so probably worth it to just get a box of those some silicone 12 gauge or 10 gauge wire the loop key is just a matter of hooking one wire in a loop onto the XT-90 antispark (buy one of these separate from the 'extra' xt-90s) and putting some heatshrink on there.  If you have to replace battery connectors at all just make sure you cut and tape up each lead separately easy to forget and cut across both leads shorting the battery through your tool (possibly welding it to the leads causing bigger problems).
```

---
## \#17 Posted by: MrDGOrman Posted at: 2018-07-02T20:35:15.718Z Reads: 178

```
I'll go with the anti-spark option then providing that doesn't cause any damage to the speed controller. I'll place my order tomorrow.

Out of interest - which charger would you recommend for £30-£40 on the HobbyKing website? Got an extra £6 to spend for free delivery and can't figure out what to get!
```

---
## \#18 Posted by: wafflejock Posted at: 2018-07-02T20:56:40.733Z Reads: 177

```
Yah insofar as I know you don't actually need the antispark either it's just nice to have to avoid burning up the connectors when there is a spark from the initial inrush current into the capacitors on the ESC.  I used my first VESC for a while without one and it worked fine but I had to replace my xt-90s after a while because the sparking charred the connectors over time (also just unnerving to hear and sometimes see the spark when hooking things up).  Another plus with the anti-spark is you can just remove it if the board is going haywire assuming you have it in a place that is easy to grab and you have your wits about you when you need to pull it, other nice things are no one can just jump on your board and hit a button and go and unlike the switches/buttons there's very little room for failure with an anti-spark (switches/buttons can fail closed/on or open/off)

Regarding chargers the imax b6 is widely used and pretty much trusted option https://hobbyking.com/en_us/imax-b6-50w-5a-charger-discharger-1-6-cells-genuine.html

Personally I use a couple of keenstone chargers, one is basically a clone of the b6 but lets you do 80W instead of 50W, newest one I got goes up to 500W.  With the 80W one with 5S*4.2V ~= 20V, 80W/20V = 4A I can really charge at 3.6A or so before it starts to overheat itself.  The 500W one I've brought up to 5A (1C) with no problems (it has a fan inside, only downside with that one is it needs DC input no AC->DC transformer inside).
```

---
## \#19 Posted by: telnoi Posted at: 2018-07-02T21:11:27.141Z Reads: 165

```
Hmm, xt90-s has been working fine for over a year with constant unplugging for charging. I got rid of the anti-spark switch, cause it's just another component that can blow up if the amp draw is too high. Not gonna happen with a single drive, but personally a big fan of simplicity. Up to you. If you're in the EU I can send you a working anti-spark switch for 15 Euro. 

As for a chargers, ISDT is brilliant. They are a bit more expensive, but less so than equivalent charger offering similar amp ratings. Charging my lipos at 14a with a q6 plus.
```

---
## \#20 Posted by: wafflejock Posted at: 2018-07-02T21:22:30.451Z Reads: 162

```
Yah I should mention it was really bad with 12S I was initially running but at 10S the spark was less of an issue really.
```

---
## \#21 Posted by: MrDGOrman Posted at: 2018-07-02T21:28:38.262Z Reads: 151

```
I'm not on my laptop at the moment but I'll post my shopping list tomorrow. I have the IMAX B6 already in my shopping bag.

I like the idea of having a switch of some sort to turn it on and off easily. I don't want to unplug the battery cables each time.
```

---
## \#22 Posted by: wafflejock Posted at: 2018-07-02T21:38:08.830Z Reads: 156

```
Seems like a good enough reason to add the anti-spark but just keep in mind you'll still need to disconnect batteries when charging unless you get a charger that can deal with all the cells in series (high voltage chargers tend to get expensive since they are pretty niche).  People tend to go with a BMS in part for that reason but I personally think it's not worth having extra components on the board to shake free or start acting up while I'm out on the road... think everyone becomes a minimalist once you are relying on the board and something fails.
```

---
## \#23 Posted by: MrDGOrman Posted at: 2018-07-04T09:48:56.054Z Reads: 144

```
So I need some advice for the charger. I don't want to be ordering from different warehouses on HobbyKing. I'd like to place an order for UK based products and then have them sent on a premium delivery service.

I currently have the IMAX B6 selected which as we know is a good charger but it's an EU product. I'm wondering if one of these products would work:
https://hobbyking.com/en_us/accuell-s60-ac-charger-uk-plug.html
https://hobbyking.com/en_us/pd606-charger-uk-plug.html

They're UK based and both have a UK charging plug which is perfect for me.

Note that I will be using the following products in conjunction with it. Will they all work together? I want to be able to charge the 3 batteries at once.
https://hobbyking.com/en_us/hobbyking-safe-40a-parallel-charge-board-for-4-packs-2-6s-xt60.html
https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html

HobbyKing livechat couldn't help because they didn't have a product specialist available so hopefully you guys can help!

Cheers,
Daniel
```

---
## \#24 Posted by: wafflejock Posted at: 2018-07-04T17:08:18.503Z Reads: 133

```
First one won't work only does 2-4S the second one might be okay.  I'm a bit suspicious of the auto charge when balance leads are connected, usually you want to set the charge rate to 1C maximum or up to the wattage limit of the charger.

Take charger wattage 50W for second one, divide by battery max voltage, for 5S it's 21V (4.2x5) so 50W/21V = 2.something amps.  So to charge 5Ah you divide 5Ah by the 2A charge rate and you get basically 2.5hrs.  Also have to multiply the time by 2 so it's really 5hrs if they are totally drained.  Bad side with that is then it's tempting to charge overnight which is risky at best.  With my 80W one I was limited to about 3.6A before it would start overheating and cut off while charging (this means 5Ah/3.6 = less than 2 hrs per battery).

With my 500W (keenstone ar1) one I'm just limited with how fast I want to put charge into the batteries I go with 1C or 5A charge rate and each battery is done in an hour, if I parallel charge could kick the charge rate up to 10A and have them both done in an hour, haven't tried that though it may max out my bench power supply feeding the charger the DC input it needs.  Usually with my batteries partially drained it's more like 45-50m per battery but I don't like to completely discharge them really.

---

Feel a bit like I'm writing an ad for the keenstone I have no relationship but have used a couple of their chargers and been good so far.  Just wanted to add the AR1 one I have will also show the internal resistance on each cell which is nice so you can see how healthy they are or compare between mfgs C ratings with measured IR during charging.

https://photos.app.goo.gl/SVneJtU2vwfaBUG2A
[Chargers](https://photos.app.goo.gl/SVneJtU2vwfaBUG2A)

Long story short I think it's worth thinking about this and shopping around a bit for a good charger that will handle 5S and supports enough wattage to charge at a rate that's acceptable to you.
```

---
## \#25 Posted by: telnoi Posted at: 2018-07-05T09:49:44.286Z Reads: 120

```
[quote="wafflejock, post:24, topic:60687"]
First one won’t work only does 2-4S the second one might be okay
[/quote]

? he has 3S lipos...a balance board does not change the cell count.
Those chargers will work...if you are willing to wait for a few hours to charge 3x 5000.
Already gave my advice above. If you want to charge lipos fast, the cheapest solution is ISDT. You can connect all three and be done within the hour.

2-5A max chargers have been awfully frustrating in the past. Just takes way too long. They are typically also crap at balance charging, thus near the end of the cycle charging takes ages.
```

---
## \#26 Posted by: MrDGOrman Posted at: 2018-07-05T10:53:11.613Z Reads: 112

```
@wafflejock I'm not going to need a massive setup like you've got, nor am I looking for something that will charge the batteries extra fast. I'm looking for something mid range that's "cheap" because this is a temporary solution. Give it a few months and I'll be ordering my more permanent battery setup.

@telnoi so with them Zippy batteries and the balance board you would suggest the iSDT? I think I've found the right one on the Hobby King website (below) but would like to make sure. £40 seems to be a reasonable price to me. It looks like I'd have to re-wire an XT90/60 plug onto the balance board and then it's good to go? Any ideas how long it would take to charge the 3 batteries using this?
https://hobbyking.com/en_us/isdt-q6-lite-200w-battery-charger.html

Thanks,
Daniel
```

---
## \#27 Posted by: MrDGOrman Posted at: 2018-07-05T11:00:36.320Z Reads: 100

```
Also, will that charger cut off automatically once the cells have reached a "full" capacity? That would be a nice little feature to have!
```

---
## \#28 Posted by: wafflejock Posted at: 2018-07-05T13:06:42.151Z Reads: 98

```
Ah right saw the 5Ah and was thinking 5S.

Regarding my "massive" setup it's just a bench power supply being used to give ac-> DC transformer cause I didn't realize when I ordered the balance charger it didn't have a built in transformer and I had the bench power supply for testing other projects... Was just showing the AR1 and some features it has.

---

Anyhow I gave you all the information I can do whatever makes sense to you at this point.

Good luck
```

---
## \#29 Posted by: telnoi Posted at: 2018-07-05T13:08:09.638Z Reads: 98

```
[quote="MrDGOrman, post:26, topic:60687"]
XT90/60 plug onto the balance board and then it’s good to go? Any ideas how long it would take to charge the 3 batteries using this?
[/quote]

The ISDT Q6 light is 8A MAX, where the plus goes up to 14A. I personally own the Q6 plus. 
Typically, lipos are charged at 1c (for 3x 5000mah, that means 15A). 
Lipos are typically discharged until 30%, thus you will have to charge a total of 10,500 after each ride.

You can calculate here how long that is roughly going to take.
http://www.csgnetwork.com/batterychg2calc.html

You'll have to decide yourself if 8A is going to be fast enough.
P.S. They both require a separate power supply. The Plus requires a 24V 15-20A power supply to be able to deliver 14A. The lite should be good with a 12V 10A power supply.

The charger cuts off at a certain voltage, which is considered full capacity. This is determined by the cell count.
```

---
## \#30 Posted by: MrDGOrman Posted at: 2018-07-05T14:25:27.249Z Reads: 89

```
@wafflejock Thank you so much for your help. I want a stand alone unit which I can plug into the wall and leave to charge and then shuts off once it's finished. I don't think I need anything fancy or fast, just something portable.

@telnoi I honestly don't have a clue what any of that means. I just want something that will take no longer than a few hours to charge the batteries fully.

Side question: 10 AWG to AMPS? I'm from the UK and all our wiring is in AMPS. Just trying to figure out what cabling I need to create the additional bits like loop key etc.
```

---
## \#31 Posted by: telnoi Posted at: 2018-07-05T15:42:00.717Z Reads: 88

```
[quote="MrDGOrman, post:30, topic:60687"]
I honestly don’t have a clue what any of that means. I just want something that will take no longer than a few hours to charge the batteries fully.
[/quote]

in that case the Q6 lite will do. Worst case, less than 3 hours. Q6 plus, less than an hour.
```

---
## \#32 Posted by: MrDGOrman Posted at: 2018-07-05T15:55:29.747Z Reads: 84

```
I think the normal Q6 will be fine for the time being. As for the power port - what have you done with that? Looks like it uses an XT90/60 input. Did you make your own?
```

---
## \#33 Posted by: wafflejock Posted at: 2018-07-05T16:12:04.371Z Reads: 88

```
Chart on this page is useful for seeing what gauge wire you can use.  Personal experience has been 12AWG is good enough on my setup but can go 10AWG if it's a concern and should be in the safe zone: https://www.bluesea.com/resources/1437

Nice calc [here too](https://www.calculator.net/voltage-drop-calculator.html?material=copper&wiresize=3.277&voltage=42&phase=dc&noofconductor=1&distance=.1&distanceunit=feet&amperes=100&x=0&y=0) if you can calculate voltage drop on a segment of wire can multiply by the amperage to get the heat dissipated by a wire/component but I can't seem to find info on what a safe wattage is given a particular insulation type (suppose again it depends on the length of the wire as well since it is dissipating that wattage across the length of it).
```

---
## \#34 Posted by: telnoi Posted at: 2018-07-05T16:18:17.136Z Reads: 84

```
![46|690x378](upload://t7OT3U5x2cxlmeFzfY2ZFH9haWE.jpg)

or 

Asus 90XB01QN-MPW000

for example. You'll have to create your own xt-60 adapter.
```

---
## \#35 Posted by: MrDGOrman Posted at: 2018-07-05T16:51:16.170Z Reads: 82

```
@wafflejock That link is really good. Thank you. I can now go to the shop and get the correct wire!

@telnoi I wanted something a little less bulky. I'll look on the internet for something that does the job. Either way, I'll be getting the Q6 Lite.

Thank you both so much for the help. You've been amazing. I'm very grateful!!
```

---
## \#36 Posted by: telnoi Posted at: 2018-07-05T16:54:46.992Z Reads: 80

```
Just make sure it's roughly 200w/delivers 10a or more to ensure that the charger reaches 8a output. 8a or less input will lead to issues (power supply operating at its limits/heating up/burning your house down. Not kidding). I think the Toshiba notebook supply will be the smallest format capable of pushing out high enough amps.
```

---
## \#37 Posted by: MrDGOrman Posted at: 2018-07-06T13:24:47.165Z Reads: 81

```
Change of plans with the iSDT - I'm going to go with the IMAX B6 v2:
https://hobbyking.com/en_us/imax-b6ac-v2-professional-balance-charger-discharger.html

The main reason for this is because it comes with a wall plug. It's one entire unit. I don't want to be buying multiple charging stations.

After going through all this hassle I see why Li-Ion Is better. This was meant to be a cheap solution so I can get out and ride - it's turned into half the price of the battery and twice the faff. :frowning:
```

---
## \#38 Posted by: telnoi Posted at: 2018-07-06T13:44:01.787Z Reads: 79

```
Understandable. I've got a power supply at work and one at home. The small ISDT goes into my backpack. All I need, but demands are very personal.
```

---
## \#39 Posted by: MrDGOrman Posted at: 2018-07-06T14:06:16.971Z Reads: 76

```
If it's your main setup and you don't plan to move away from that setup then what you've got is ideal, but as I'm only having this for a few months I don't see the point in investing loads of money. Once I've got the proper setup I'll probably use these bits for a slower board and give it to my girlfriend. Might even make her a scooter, I'm not sure!

Either way. Thank you so much for the help. You too @wafflejock, you've been a massive help aswell!
```

---
## \#40 Posted by: MrDGOrman Posted at: 2018-07-14T09:22:55.075Z Reads: 76

```
I'm back! And naturally I'm stuck in a predicament :smile:

I was going to order the IMAX B6 V2 along with a wall plug converter (US to UK, or something) and a lipo safe bag to charge the batteries.

However, I would need to buy these from the EU warehouse on HobbyKing which means shipping charges, wait times, etc.

However, I remember someone (@telnoi or @wafflejock maybe?) mentioning the keenstone charger. This only works out about £5 more expensive to buy and it already had a UK AC lead with it (I assume I don't need to have a power converter of any sorts for this?). It is. 100w charger compared to a 50w charger aswell. Not sure if that's good or not, but would it be worth while getting that instead? I've found it on Amazon and it's included in the Prime service so I'll get it next day (winner!)

https://www.amazon.co.uk/dp/B072WRGV6M/ref=cm_sw_r_cp_apa_KjisBb81VH4ZB

Thoughts? I know it doesn't have a lipo bag but I'll order that at the same time on Amazon which is next day delivery again.

Side question with lipo safe bags - I've found one that will fit the 3 zippy batteries in but it'll be a "tight fit". Do the batteries heat up while charging, and if so - does that mean you shouldn't place them close to eachother?

Cheers,
Daniel
```

---
## \#41 Posted by: wafflejock Posted at: 2018-07-14T14:59:44.126Z Reads: 65

```
Looks like a good deal to me, they throw in a lipo tester too those are usually a couple of bucks and convenient (especially if you want to parallel charge can quickly check all the batteries voltage through the balance lead).  Regarding heat build up I wouldn't worry about it while charging really, if the batteries are getting hot you're probably charging them too fast (with 100W charger pretty sure you'll still be limited to less than 1C charge rate).  With my quad lipos that I charge more often and have my hands on directly I've never noticed heat on them after charging but after flying and big discharges they're always cooking hot.  Alternatively or along with lipo safe bags can get an ammo box from army surplus (not sure if that's just an American thing) for about $20 it's basically just a metal box with a lid but should safely contain any fire (I've not had a problem in over 2 years of flying and riding my esk8, started flying a few months before building my esk8, but better safe than sorry).
```

---
## \#42 Posted by: MrDGOrman Posted at: 2018-07-14T16:22:29.557Z Reads: 61

```
Sweet! I'll order the keenstone charger then. I've already got a battery tester because I ordered that at the same time as ordering the batteries which is annoying but not to worry.

I'm fairly sure I've got an old ammo box somewhere from my long range shooting competition days. Will be more than enough to contain a fire! I'll go on the hunt.

Thanks for all the help. I'm getting very excited now!
```

---
## \#43 Posted by: wafflejock Posted at: 2018-07-14T16:40:46.843Z Reads: 62

```
No problem.  If you take the charger wattage and divide by charged voltage of your batteries can work out max amperage the charger can handle before it starts to overheat (usually in reality will be like 10% lower than that).  The keenstone one's I have will shut themselves off if they get too hot, for the 50W one on 5S I'm limited to about 3.4A (if I point some fans at it can go up to 3.6A).  Take battery capacity in Ah and that's your max charge rate to keep the batteries healthy and will charge in 1hr if you can maintain that charge rate.  So for my 5Ah it's 5A max charge rate, with two in parallel can do 10A charge rate (my 500W one can do this has built in fans)
```

---
