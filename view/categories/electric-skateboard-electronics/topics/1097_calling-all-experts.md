# Calling All Experts

### Replies: 34 Views: 3163

## \#1 Posted by: mcoyle Posted at: 2016-01-24T21:34:33.553Z Reads: 279

```
Hey guys,
After an all-nighter and a lot of determination, I've planned the motors, ESC, controller, and battery. Before I make my purchases I would appreciate some expert advice, as I'm new to the e-board world - but I plan to stay. I plan on running a dual motor setup on the rear trucks of my longboard. 

To avoid the cutting, welding, and precise calibrations for the gears and belts, I decided to use the pre-welded motor mounts found here by diyelectricskateboard 

Since I live in hilly Binghamton, I wanted a motor with sufficient power to climb hills, without sacrificing too much max speed. I planned on buying 2 of these motors. 
produc 

To support the two motors, each of which can have 80A max amps, I planned on using a 180A Rotorstar ESC because it could support more batteries if I cared to push my max speed.
produc
-Regarding the ESC though, I want to be sure that it has regenerative breaking. If this one doesn't, I'd appreciate it if someone could direct me to one that does.
-Also, this particular ESC mentioned a LED status display - if anyone has owned one of these, what does it tell the status of..?
(I am now realizing that since I have two motors I may need two ESCs? Maybe smaller max amps? Or instead do I just need to split the wires in the ESC to both motors?)

For a controller, I plan on using a simple 2.4GHz transmitter. I plan on 3D printing a smaller case for it.

For batteries I plan on wiring 2 x 5000mAh 3S1P 30C LiPo in series to create a 6S battery without the worry of too little clearance. I can also wire another 2 of these in series, as the ESC above supports 4~14S battery power. This should double my Voltage and push my max speed...right?

Since LiPo batteries can be harmed if drained too low, I also planned on including 2 LED Rx Voltage Battery Checker 6.6~7.4V LiPoly/LiFe.
But do I need two of these? Or should I rewire the batteries together using a converter before plugging into the battery checker.

The only thing I'm missing as far as I know is the battery chargers, something to safely house the components, and the card required to program the ESC (which I would appreciate help on).

Please send me your input, as I'm ready to invest and get started. Thanks!
```

---
## \#2 Posted by: cmatson Posted at: 2016-01-24T21:50:54.416Z Reads: 256

```
Welcome!

you will need two esc's for two motors- the two best choices (with upgradability in mind) are the VESC and torqueboard's 12s esc. 

Also, you may want to go with more than just 5,000mah. It's a good starting point, but with dual motors and hill climbing it's only going to give you 5-7 miles. 

Have you considered the space cell from enertion? It's a battery with a laptop style charger, percent display, and simple on/off switch. You could pair it with dual VESC's, and have a build that would fly up hills and be able to go 15+ miles on a charge. Higher voltage also means a lower amp draw, so your components don't heat up as much as they would on 6s. 

Finally, what is your desired top speed? 

 - a space cell + 190kv will yield around 20-30mph depending on gearing. 

 - A 6s + 230-270kv will yield around 20-30mph depending on gearing. 

Good luck on your build!
```

---
## \#3 Posted by: mcoyle Posted at: 2016-01-24T22:25:39.273Z Reads: 235

```
What's all the buzz about these VESCs? They only support 50A continuous, which is far below the max motor output. They are also only in beta, so that just makes me worry a bit. And the torqueboard 12S ESC is sensorless - how would that effect the performance of a sensored motor? ( product/electric-skateboard-motor-6355-230kv-2650w/ this is the one I have in mind)

And I've seen many recommendations for 5,000mAh batteries, as I can add more or swap em out when they're dead. Although the space cell is EXTREMELY tempting to double my distance, that alone doesn't justify the vast difference in price. Also, the board I plan on using (Kahuna Creations Magma) has enough of a concave that I would worry about the Space Cell battery not being secured well enough.

Last question: Should everything be wired in series? I know that the motors each must be plugged directly into its ESC, but then how do both ESCs get connected to the receiver?

Price has a bit of a hold on me so I can't make it crazy, but I want a board that's practical on campus for sure. So I still like the idea of the 6S + 230kV. Max speed isn't really my main concern, since there are always hills for that, and I could just throw on a couple more 3S batteries to push my max on occasion, granted I end up getting an esc that can support 12S. It's just these ESCs that worry me. 

Thank you for all your help. You have shown me that I'm a little more fluent in my knowledge of motors than I was yesterday.
```

---
## \#4 Posted by: massy Posted at: 2016-01-24T22:38:27.615Z Reads: 195

```
The VESC is one of the best ESCs for the purpose out there, end of story really. It's a pretty custom PCB with its dedicated STM32F4 chip and is able to deliver 50A continuous, do you even know how much that is? At 12s that's over 2000 Watt CONTINOUS. You'd burn through a 5 Ah battery in SIX minutes, you think you'll ever do that or rather *want to do that*? People tend to go way over on amperage rating with the RC-car ESC's because they are more cheaply made and it's safer to go for a way above rating. For me cruise control is a selling point on the VESC as well, it means the motor breaks if you go downhill or accelerate when going uphill to keep the same speed. 

*"Last question: Should everything be wired in series? I know that the motors each must be plugged directly into its ESC, but then how do both ESCs get connected to the receiver?"*

The VESC at least has support to connect multiple together via CANBUS. You bridge two pins to the same two pins on the other VESC and you're good to go.

Regarding price of SPACE cell, you get more than the extra range really. You get a BMS so you do not need a balance charger (i.e you get a small charger easy to carry and plug in). You get a power button that cost probably at least 30-50 USD to make/get yourself so it's not only about the range but I'm gonna use LiPo's as well so not gonna sweet talk the SPACE cell too much.
```

---
## \#5 Posted by: mcoyle Posted at: 2016-01-24T22:44:32.872Z Reads: 181

```
Wow. Thank you. Really put things in perspective. Looks like I'm waiting until mid february for the VESC to put out their latest model. I just want to confirm that you mean the VESC probably can support 2x 230kV motors at 6s. And maybe even 12S on occasion? Thanks, you offered a very detailed and clearly unbiased answer. I really appreciate this, now I cant wait for my board to come to life in front of me.
```

---
## \#6 Posted by: mcoyle Posted at: 2016-01-24T22:46:03.793Z Reads: 173

```
Whoops one last thing, what's a BMS?
Thanks again!
```

---
## \#7 Posted by: massy Posted at: 2016-01-24T22:50:58.735Z Reads: 169

```
A BMS is a battery management system that's used to keep all cells of the battery balanced. What it means effectively for you is that you can use a laptop style charger instead of having a balance charger that's a bit more work to

1. Connect for charging.
2. Carry, it's a lot heavier and usually needs a power supply (if it doesn't have one built in). 

As far as I know people have run 2x motors at 12s with the VESC (or rather VESCs). Remember that 50 A at 6s (22 V) is 1100 Watts but 50 A at 12s is around 2100 Watts (and using two VESCs provided the batteries can handle that, it's 4,4 KW which is more than you'll ever need). Also, someone correct me here if I'm wrong.
```

---
## \#8 Posted by: mcoyle Posted at: 2016-01-24T23:08:43.843Z Reads: 169

```
Thanks again!
However now I have more questions haha.
Below is a link to 3 LiPo 6S BMSs, the only difference between the three is the differences in Amp.
http://www.batterysupports.com/lion-lipo-nbsp-22v-nbsp-6s-c-32_67.html

They come in 30A, 45A, and 60A. Should the values be matched to the motor? the VESC? 
Looks like after I figure out which BMS and laptop style charger to get, I'll have a complete plan so thank you so much for all your help! and not to mention how much money you're helping me save on the space cell :smiley:
```

---
## \#9 Posted by: massy Posted at: 2016-01-25T00:24:56.632Z Reads: 165

```
Maybe someone else can chime in here, since I am not that sure about these things. Some people advise against using a BMS and LiPo, some against using LiPo at all and so on. My personal plan is to use LiPo's with a BMS but then again LiPo has some pros and cons compared to the 18650 cells in for example the SPACE cell.
```

---
## \#10 Posted by: cmatson Posted at: 2016-01-25T00:59:16.873Z Reads: 160

```
I just want to add that the VESC will not work on 12s with motors over 200kv.. it'd be way to fast anyways if it did support it; I think you'd be looking at over 50mph...

Also, it's not recommended that you run a BMS with lipo cells as @massy said. 

The 18650 style cells in the space cell are simply more durable and less likely to suffer from voltage variations from cell to cell. Not to mention they can last 3x longer than standard lipos.

BMS systems have been used with lipo's in the past, but I honestly wouldn't go that route..

Either just balance charge your lipos, or get a space cell.

it's about $150 vs $300, but the space cell will last longer, have more than double the range, give you more speed with less heat, have a simple on/off switch, LCD percent display, and a simple laptop style charger...

I totally get it if you are on a budget, but if you are thinking about getting a BMS and a laptop charger, then you might as well just go with a space cell.
```

---
## \#11 Posted by: torqueboards Posted at: 2016-01-25T01:21:12.302Z Reads: 148

```
That 180A Rotorstar is a Heli ESC which won't work properly. I would recommend the VESC from Ollin or Enertion and/or the TorqueBoards 12S ESC if you want something easier.

You'll need (2) ESCs for (2) Motors. One for each.

Voltage checker's are OK. Just be careful not to leave them plugged in when not riding. They will pull power from one cell and ruin your pack.

@Mcoyle - The startup on the VESC is great. You practically don't need a sensored motor.

Sensorless setup just requires you to kick push to get going. It eases your motors on the start-up and will not be as "hurtful" for your motors.

The ESC's have a 3pin wire for signal to the RC receiver.

6S on a 230KV should be pretty fast and enough power. If you wanted more power you'd go up to 10S/12S.

IMO - I prefer LiPo's. I'm working and testing 18650's but LiPo's are nice and simple once you learn how to charge. Easy to swap packs. Yearly HobbyKing will have rock bottom deals and I stock up for the year. If a lipo pack fails.. it's a measly $20-40 bucks.. maybe $60 bucks at max for a set.

If your Space Cell breaks and/or you end up wanting two or three DIY boards. You have to purchase another Space Cell $300+. You can fix it but it's a bit more difficult for most.

Don't get me wrong though. Space cell by far is nice and sleek.

But LiPo's are great and flexible.
```

---
## \#12 Posted by: mcoyle Posted at: 2016-01-25T01:30:47.510Z Reads: 132

```
I like the idea of LiPos more as well, mainly because i fear the committment of spending that kind of money on a single battery that may break. I'd rather have a few cheaper batteries that can easily be replaced. I'm just a little overwhelmed with the BMS and struggling to find a good charger. Would you recommend any particular BMS or laptop style charger? thanks!
```

---
## \#13 Posted by: mcoyle Posted at: 2016-01-25T01:33:00.006Z Reads: 131

```
And also would I need one voltage checker per LiPo battery or is there a better way of connecting them? Thanks for all the help!
```

---
## \#14 Posted by: torqueboards Posted at: 2016-01-25T01:40:55.773Z Reads: 131

```
If you go lipo. I prefer iCharger 208B and a HobbyKing 350W Power Supply. No BMS. Makes things too complicated and much harder to swap packs. I charge 6 packs in parallel. 3 sets of 2x packs in series.

You would use a voltage checker per each Lipo pack. You'll eventually know how far your packs will go and I ocassionally jsut check the packs when on a long route. I charge to 4.15v and swap at 3.6v.

The iCharger and HK 350W are expensive at first about $160 for both. But they are both high quality and last a long time. You can also charge up to 20amps. Although for 6x packs I charge at about 15 amps.
```

---
## \#15 Posted by: mcoyle Posted at: 2016-01-25T01:43:08.915Z Reads: 126

```
Thanks for all the help! I like having options to look into. I really appreciate all the advice.
```

---
## \#16 Posted by: RunPlayBack Posted at: 2016-01-25T02:17:57.913Z Reads: 137

```
Agreed with @cmatson on the Space Cell. Before my build, my only experience with Lipos was with Mini Quadcopters and it was never as smooth as I had hoped for. I took great care of them, always used a balance charger, never over discharged, always used a voltage alarm on both the battery and through telemetry on my radio but the voltage variations always seemed off and I ended up buying a lot more batteries than I initially planned. After I sold all of my Mini Quad gear and moved into eskate, I knew it was either Lipos again or Space Cell. I'm satisfied that I went for the Space Cell especially since I've put a few miles into my build. It's a big battery and getting the right enclosure is tricky but the range is insane and the built in BMS, voltage display and fuse makes it almost foolproof. Also having a laptop style charger in my bag means I can charge it anywhere and not have to whip out a lipo charger in the office. I totally get the allure of having a system that you can subtract or add cells at will which is why I'm hoping someone makes a modular li-ion system soon, especially so I can take this thing on a plane :smile:
```

---
## \#17 Posted by: torqueboards Posted at: 2016-01-25T02:43:28.501Z Reads: 134

```
[quote="RunPlayBack, post:16, topic:1097"]
I'm hoping someone makes a modular li-ion system soon :smile:
[/quote]

That would be awesome :smile: Would totally solve the 99wH issue also..
```

---
## \#18 Posted by: Sharkface Posted at: 2016-01-25T04:23:58.669Z Reads: 139

```
[quote="torqueboards, post:17, topic:1097"]
That would be awesome :smile: Would totally solve the 99wH issue also..
[/quote]

Could we reliably get 18650/26650s fixed together into different P cells using bolts? I know there is a lot of vibration so i would hate for cells to jiggle, but if we could bolt them into place rather than spot weld them, not only would we get around that age old argument of "o you shouldnt apply heat to an xx650 battery" but we would also be able to replace individual parts of each parallel cell. If we are going to make a modular battery, we would want to take advantage of modular repairs am i right?
```

---
## \#19 Posted by: chaka Posted at: 2016-01-25T05:03:05.748Z Reads: 135

```
There is a loophole for non-removable batteries with BMS and short circuit protection.
```

---
## \#20 Posted by: onloop Posted at: 2016-01-25T07:39:36.231Z Reads: 142

```
[quote="RunPlayBack, post:16, topic:1097"]
especially so I can take this thing on a plane :smile:
[/quote]

I took several flights from Hawaii back to Australia carrying 2 separate space cells.. Must take them as carry-on luggage, no one asked a single question - not once, three separate custom checks, three different airlines.... 

I placed each battery (inside its cardboard box) into the plastic trays directly in front of the TSA agent, they didn't care, did not ask a single question..

If you are super worried make up a new label that says 20v 4.5Ah and stick it on the pack.
```

---
## \#21 Posted by: RunPlayBack Posted at: 2016-01-25T14:37:55.340Z Reads: 148

```
Excellent idea. I've definitely gotten away with bringing a few heavy duty V-Mount batteries in my camera bag with no problems.
```

---
## \#22 Posted by: barajabali Posted at: 2016-01-25T15:55:09.101Z Reads: 148

```
i vouch for Lipo use, and i'm not bias because i use both types of batteries (18650 and lipo) in a few of my boards. Ive never had a problem, as long as you don't buy a cheap balance charger you should be fine. And Lipos are more "dense", more compact.  18650's are cylinders so there is naturally gaps between cells.

Edit: Lion or Lifepo all the way
```

---
## \#24 Posted by: Acido Posted at: 2018-01-25T21:16:03.233Z Reads: 68

```
Dont go 12s with tourqeboards vesc, it will blow up, VESCs are so popular because of its ability to be programmed like basically anything you wish you can change so much you wont understand more than a half of it
```

---
## \#25 Posted by: mmaner Posted at: 2018-01-25T21:27:28.972Z Reads: 67

```
You realize this thread is from 2 years ago right :slight_smile:
```

---
## \#26 Posted by: barajabali Posted at: 2018-01-25T21:31:21.372Z Reads: 68

```
Back when I used to vouch for Lipos.
```

---
## \#27 Posted by: mmaner Posted at: 2018-01-25T21:33:05.148Z Reads: 71

```
I still use both.  For cheap boards they are still a viable alternative.  I prefer my 30Q packs though, much easier to maintain, vastly increased charge cycles and lots of capacity.
```

---
## \#28 Posted by: Acido Posted at: 2018-01-26T05:53:57.146Z Reads: 58

```
Why do these threads come up and I always reply and then someone says this to me...
```

---
## \#29 Posted by: pennyboard Posted at: 2018-01-26T06:35:29.826Z Reads: 60

```
I still use Lipos. There still isn't a Lion out there that can meet my discharge needs at an acceptable weight
```

---
## \#30 Posted by: ZackoryCramer Posted at: 2018-01-27T05:28:39.167Z Reads: 49

```
HA! I am using 13s on Maytech VESC. Never had problems. Nice try. 
And you know TB sales their skateboards with 12s battery packs right?
```

---
## \#31 Posted by: scepterr Posted at: 2018-01-27T05:36:43.299Z Reads: 48

```
Have you pulled more than 500-600 watts?
If youre not running at its full potential or beyond that of 10s or 12s, just having a 13s battery isnt a good indicator of reliability
I could run 14s all day long at 500watt....doesn't mean anything
If you're pulling 4-5kw between 2 vescs then we can talk 😉
```

---
## \#32 Posted by: ZackoryCramer Posted at: 2018-01-27T05:40:14.242Z Reads: 46

```
I don't think I have enough traction to pull more than 900 watts const., but gas flooring never killed it.
Was just trying to disprove @pennyboard
```

---
## \#33 Posted by: Acido Posted at: 2018-01-27T08:08:17.663Z Reads: 39

```
Probably max a is 30 

Too many stories of fried vesc here from now on im with focbox and vesc6
```

---
## \#34 Posted by: pennyboard Posted at: 2018-01-27T16:36:59.225Z Reads: 30

```
I’ve pulled about 1200 watts on 12s between 2 VESCs during acceleration on flat ground. I’ve never looked at the data for when I accelerate up hill. 
(1200 watts per VESC so 2400 watts total.)
I’d guess I’m pulling somewhere between 4000 and 5000 watts accelerating up hill.
```

---
## \#35 Posted by: ZackoryCramer Posted at: 2018-01-27T18:44:17.078Z Reads: 27

```
If you think about 4~5kw is a lot of frickin Power for a skateboard
```

---
