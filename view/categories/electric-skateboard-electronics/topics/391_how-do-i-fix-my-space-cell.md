# How do I fix my Space Cell

### Replies: 41 Views: 5136

## \#1 Posted by: Moja Posted at: 2015-11-02T02:46:18.313Z Reads: 176

```
Whilst setting up my board I soldered my XT60 connector on my VESC with the polarity the wrong way round, when I connected my space cell something happened and my space cell is no longer responsive. The VESC and everything else work fine with another battery but I cant get any voltage out of the output wires on the Space Cell. I have opened up the unit for an inspection and I cant find any burnt out connections, I used my multimeter to test for voltage to find the problem and I am reading 37v up until the PCB, after that the voltage reading are between 2-8v, I assume the PCB needs replacing? 

Any idea what he easiest fix will be? 

ps. Separate question but why is there a 30A fuse fitted to the space cell when the VESC draws far more? I have blown out lots of 30A fuses on my other FIIK batteries trying to ride the board, the biggest I can find at Jaycar is 40A. I have used BLDC motor tool to limit the power draw but Im a bit confused with this, specially as I am running a dual VESC setup. What size fuse should I be using on my battery? 

Cheers, 
Moja. 

  <img src="/uploads/db1493/original/1X/914972a8953e378c2b513e20c99128295389620f.JPG" width="666" height="500">
```

---
## \#2 Posted by: cmatson Posted at: 2015-11-02T03:22:06.899Z Reads: 165

```
space cell maxes at 60amps, and 30amp fuses can burst 60amps for 5-10 seconds. Putting a 60amp fuse would allow for it to burst higher than the space cell can handle, ruining the point of the fuse even being there.

one question though:
is the display coming on? 

**if it isn't, then try this:**
When my space cell seemingly died (reading 2 point something volts after the bms, 40 before it) it was actually just a balancing wire... it somehow wiggled out. The weird thing is, it didn't happen on a ride: it happened on my workbench. I'd unplug your 11pin plug (at the top of the BMS) and just look to see if any of the pins/wires seem out of place. If not, just throw it back on there and make sure it is in **all** **the way...**

@onloop and I tried to fix mine for close to 2 weeks with no luck. then, because of a guy on ES who was very adamant about helping me, I was miraculously able to fix it after finding a loose balancing wire. 

just because of your situation, I doubt that is the problem, but mine just stopped working while sitting on my workbench, so it's worth a shot just looking into what I mentioned...

Good luck! I think you'll be able to fix it because the BMS isn't blown up, and like you said, there aren't any fried connections
```

---
## \#3 Posted by: Moja Posted at: 2015-11-02T03:45:27.264Z Reads: 156

```
I am getting nothing on the display. The 11 pin plug is seated perfectly and all the pins are fine, I've done a pretty thorough visual inspection and everything seems to look fine, no loose pins.

What is a BMS? 

Thanks for the support.
```

---
## \#4 Posted by: cmatson Posted at: 2015-11-02T03:49:30.988Z Reads: 153

```
BMS is the brains of the operation- it's the board that the cells, screen, and button are all wired into.

**I think I've found something though!**

It looks like your charging port isn't plugged into the positive lead heading to the battery (that red wire just hanging out in the open)
see my pic where the charging port has two wires:<img src="/uploads/db1493/original/1X/434da9a1e7e7d7b4135aba89a97fee57558be49e.jpg" width="690" height="388">
```

---
## \#5 Posted by: Moja Posted at: 2015-11-02T04:12:24.924Z Reads: 147

```
That fixed it, you rock mate. 

Just going back to the query about the fuses, if your statement is true, why would I be blowing out 30a fuses? surely running 2 VESC's draws twice the current?
```

---
## \#6 Posted by: cmatson Posted at: 2015-11-02T04:51:18.508Z Reads: 149

```
**Awesome!**

I'd refer to @onloop for dual VESC amp draw questions. I know he uses dual VESCs and a space cell on all his pre-made builds; I on the other hand, have always gone with a single.

glad you got the battery all sorted out though!
```

---
## \#7 Posted by: Moja Posted at: 2015-11-02T05:00:29.440Z Reads: 145

```
Its odd how the cause of my problem had nothing to do with how I fixed it :p  Who cares, its fixed!
```

---
## \#8 Posted by: longhairedboy Posted at: 2015-11-02T14:28:51.779Z Reads: 140

```
i'm about to build a DR setup with a space cell, dual R-SPECs and a 12S Torqueboards ESC. I'm not going to be blowing fuses all the time, right? I know about throttling those ESCs down to 80%, but other than that I'm good, right? I keep seeing stuff like this and it makes me wonder. 

This battery porn got my blood flowing this morning.
```

---
## \#9 Posted by: chaka Posted at: 2015-11-02T15:54:17.995Z Reads: 136

```
You could switch it out for a fast blow fuse with a higher rating. They are a little expensive, around $7-$10. I get mine from mouser under automotive fuses, they have some specifically for electric vehicle battery systems.
```

---
## \#10 Posted by: cmatson Posted at: 2015-11-02T17:50:34.689Z Reads: 133

```
[quote="longhairedboy, post:8, topic:391"]
I'm not going to be blowing fuses all the time, right?
[/quote]

I think you honestly would... it's just not a good match up: you have to turn timing all the way down to very low, acceleration on low, and forward force to 80%. It made it slowed than my 245kv 6s build, even with the R-SPEC geared up higher (15/36 vs 14/36). 

and all that is on a single setup with a 140 pound rider; when my 200 pound dad tries to ride it, the fuse blows on the very first acceleration...

I think it would only get worse with two torqueboard's escs- Not to mention VESC's are cheaper, and don't require a separate BMS.
```

---
## \#11 Posted by: longhairedboy Posted at: 2015-11-02T18:20:42.154Z Reads: 127

```
guess i'll save those for a lipo build  and order a pair of VESCs for this space cell. Hopefully I'll get them this year. I need to finish this build soon and sell it. its always something.
```

---
## \#12 Posted by: longhairedboy Posted at: 2015-11-02T18:29:43.977Z Reads: 124

```
on second thought, i think i will convert my current 6S beater board into a 12S and tell myself merry christmas.
```

---
## \#13 Posted by: kai Posted at: 2015-11-02T18:33:10.952Z Reads: 123

```
It just feels so much better when you are building for you and not someone else. The satisfaction is way higher.
```

---
## \#14 Posted by: Moja Posted at: 2015-11-02T22:05:26.942Z Reads: 138

```

I switched out the 30A fuse for a 40A one and Its no longer blowing out. I got catapulted off the board whilst accelerating with full power when the 30A fuse blew and that was extremely dangerous. I have the motor max and battery max set to 60 in BLDC tool. Is having a 40A fuse on the battery doing it any damage? I want to completely avoid any blow outs by having things balanced properly, its far too dangerous to have the system shut down whist you are anticipating power during acceleration.
```

---
## \#15 Posted by: onloop Posted at: 2015-11-02T22:13:04.034Z Reads: 137

```
The correct setting for dual vesc would be 15A  each MAX battery current draw. 

Note: You can also adjust max regen current to prevent accidentally blowing fuse when regen-braking really hard

http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353

2x 15A is 30A Max. You will never blow a fuse unless you accidentally reverse polarity or there is a short somewhere after the battery.

You could probably push this to 20A each VESC and still not blow any fuses. Depends on weight / terrain / drive train config.

The motor current limits can actually be set higher, maybe 80A each. This allows high motor current whilst similtaniously having low battery current without blowing the fuse.

Quote from BV; For the VESC you can configure different current limits for the motor and battery. You can for example set the motor current limit to 80A and battery current to 30A, which should work nicely with dual motors on a space cell. The motor current in each motor will then be able to reach 80A until you have reached 3/8 of the full speed. After that, the motor current will be more and more limited the faster you go. End quote.


I suggest testing different settings and slowly increasing from low to high amps until a fuse pops. Then notch it down.

With these advanced settings in the VESC you could completely bypass the BMS for discharge. You could also remove the fuse. The current controll function in the vesc is very advanced and can manage output & input currents at the battery very effectivly 

I have had the vesc set at 20A each max battery current since day one... never blown a fuse. (With r-spec)

However when I started testing hub motors I blew the fuse everytime I tried to start. They obviously need much more power to start. I had to set max amp draw at 15A on each vesc to prevent fuses blowing.

In the long run I think I am going to have to start advertising the space cell as being "not compatible" with Torque Boards & ALIEN ESC... as they don't have current control.
```

---
## \#16 Posted by: Moja Posted at: 2015-11-02T22:42:01.658Z Reads: 122

```
Good facts to keep in mind. Where in the BLDC tool do I specify the max ampage?
```

---
## \#17 Posted by: onloop Posted at: 2015-11-02T22:44:09.591Z Reads: 128

```
Open that link above about "regen braking" all the settings are in the same page/tab/section.
```

---
## \#18 Posted by: Blasto Posted at: 2015-11-03T01:24:34.046Z Reads: 131

```
What is the BMS that the space cell uses?
```

---
## \#19 Posted by: Moja Posted at: 2015-11-03T01:38:29.933Z Reads: 132

```
Im getting 32kph top speed with those settings, what do I need to be doing to get up to 45?
```

---
## \#20 Posted by: longhairedboy Posted at: 2015-11-03T12:23:49.778Z Reads: 128

```
> In the long run I think I am going to have to start advertising the space cell as being "not compatible" with Torque Boards & ALIEN ESC... as they don't have current control.

Yes. Please make that clear somewhere prominent. In fact, lets just clear all of that up right now. 

While the Space Cell doesn't play nice with LiPo ESCs, it's a great match for VESC after you do a lot of tuning that you can't do in most if any of the other ESCs available. 

And VESC is great for LiPos too, correct? So if you want a space cell, you have to get a VESC, and if you want LiPos, you can have VESC or any number of other car ESCs with good reputation and adequate specs. 

I really wish somebody would build an adequate up-to-12S BMS for lipo packs.
```

---
## \#21 Posted by: chaka Posted at: 2015-11-03T15:37:23.956Z Reads: 124

```
The VESC works great with lipo! The VESC loads with a default setting of 60 amps and to be honest it is a pig with the current limit this low but it is perfect for getting the VESC started. 80 amps seems to be more of a sweet spot for good acceleration.
```

---
## \#22 Posted by: torqueboards Posted at: 2015-11-03T16:09:48.976Z Reads: 114

```
What issues are you guys having with Torqueboards 12S ESC + SpaceCell? I know, about 3-5 people using them together exclusively on a daily basis for commuting to work. No issues or complaints from them.
```

---
## \#23 Posted by: cmatson Posted at: 2015-11-03T17:53:22.919Z Reads: 110

```
it's not a problem per-say, but just a nuisance- you can't get the full performance out of the space cell with your esc.

If you had a currently limiting setting so it didn't try to burst more than the space cell can handle, I'd take it over the VESC any day because it is just a simple, easy to use esc. 

Right now, in order to not blow a fuse I have to use the following settings (I'm only 140ish pounds). When my dad tried to ride my board with these settings (he's about 190ish) the fuse blew after about 3 seconds:
max forward force: 80%
motor timing: low
acceleration: low

braking and most of the other settings (besides raising the lipo cutoff because the space cell will do that for me) are left stock.
```

---
## \#24 Posted by: longhairedboy Posted at: 2015-11-03T19:10:11.534Z Reads: 107

```
The SPACE Cell should be able to work with ANY ESC at all that is rated for 10S or above using all of the maxed out settings on the ESC and not blow a fuse. The idea that I can only reliably use one ESC with it, one that is not plug and play and doesn't even come in a durable package, is irritating. 

Any LiPo ESC is behaving correctly in asking for whatever power it can get when that trigger is pulled, so the BMS in that pack should limit the current output in a way that results in not having to replace fuses. Hopefully in future versions this can be addressed.

The Space Cell showed up to a LiPo party and is eating all the chips but not passing the blunt. Puff puff pass homie, don't just stand and try to hide it. 

/rant
```

---
## \#25 Posted by: onloop Posted at: 2015-11-03T23:04:43.901Z Reads: 113

```
Firstly. Current limiting is a good thing. You should value it. Without it all of your electronics can be destroyed within seconds. This Is why it is built into the vesc.

Also... the fuse is something that I have come to really appreciate. It saves people from an expensive mistake.

Also with Vesc You can achieve higher motors currents whilst limiting the battery current... 
You could have 80A in the motor during start up whilst only drawing 30A from the battery... the vesc is so feature rich! It's truley an awesome piece of gear so if you buy one so your space cell can work optimally its a good investment.

Anyway...

Now Ask yourself on average how long does your lipo batteries last, if used without limits, before puffy the dragon pays them a visit. Some much shorter then others, especially under high Peak amp draws... eventually under high amp draws most things fail prematurely.

From my experience using lipo's (especially the cheap ones from hobbyking aka. Zippy flight max) they can't handle the discharge rates of unlimited-current ESC's. They swell from being over discharged.

Using a BMS with lipo is not a common practise (alien power system does offer it though- go figure), nor recommended. LIPO is notorious for getting out of balance. They also have a naturally short life span... a BMS won't really play a role in changing that fact. Also they shouldn't be charged unattended.... 

Let me move on,

So, If you want to run your system hot and not limit the current that's fine by me... but at least buy some very good quality lipo that are rated to handle it.... the quality lipos will last through the punishment.... but now sit back and wait for the ESC or motors to fail... the electronics tend not to like heat. The weakest link will fail! 

Speaking from a vendors perspective I need my products to last a very long time... So there needs to be saftey limits. Just like in you car... you can never reach max speed or rpm... there are limits. Otherwise without limits I keep needing to replace parts under warranty and eventually go broke. 

It also worth noting that flier can make esc with current limiting but they don't... they also have lots of failures, can you guess why?... Before vesc I had some current limited flier made. They actually worked well. Alien should consider it. As much as I hate to say it customers need to be protected from destroying their products.

Just so you all know the S.P.A.C.E Cell v2.0 will be 10S4P with 50A constant current - this is 30% additional capacity... & It will be ONLY 20mm longer than the existing model. Of course much more expensive too.

One of the main reasons i am doing this  (increasing cont current) is due to the increasing popularity of hub motors, higher current draw is required, especially on start.. Otherwise 30A continuous is actually ample for most systems.... 

Rant over.
```

---
## \#26 Posted by: Moja Posted at: 2015-11-04T06:12:16.474Z Reads: 101

```
[quote="onloop, post:25, topic:391"]
You could have 80A in the motor during start up whilst only drawing 30A from the battery
[/quote]
Will the config XML file you have on your google drive for the R-SPEC 2.0 motors give me this?
```

---
## \#27 Posted by: longhairedboy Posted at: 2015-11-04T12:41:35.696Z Reads: 95

```
Stop making so much sense when I'm angry!
```

---
## \#28 Posted by: chaka Posted at: 2015-11-04T12:55:10.782Z Reads: 92

```
I think this only works for startup boost. I dont think it gives you 80 amps while flying down the road, I could be wrong.
```

---
## \#29 Posted by: onloop Posted at: 2015-11-05T00:21:01.022Z Reads: 92

```
I wrote an article discussing this stuff.

http://www.electric-skateboard.builders/t/vesc-faq-optimized-s-p-a-c-e-cell-settings/414
```

---
## \#30 Posted by: Moja Posted at: 2016-01-05T01:21:00.251Z Reads: 84

```
I didn't have an enclosure on my space cell, after taking it on and off my board a good 50 times its stopped working. I assumed an air gap on a connection due to movement in the cell but can't find any. I'm getting 40v up to the BMS but no voltage coming through the earth on the other side of the BMS. To me it suggests that that the BMS has failed but that's hard to believe as it stopped working overnight on my work bench, no shortage or anything unusual caused it to fail as far as I know. 
 The voltmeter won't show anything, if I charge the unit the voltmeter flashes for a short moment then nothing. 
 The cells seem fine, vtage readings are fine up to the BMS.
Any troubleshooting suggestions?
```

---
## \#31 Posted by: cmatson Posted at: 2016-01-05T01:38:18.155Z Reads: 82

```
same exact thing happened to me: It stumped me for a good couple days (this was a couple weeks ago)

Look at ***ALL*** of your connections to the battery pack's cells- one of mine looked like it was perfectly attached, but it was just like 1/2mm away from the contact points. Soldered that back in there and I was up and running again!

Didn't stop me from taking out all the connections going to the BMS and peripherals to resolder them though... 

I wish I caught it earlier before spending 3+ hours resoldering every dang connection.

I want to get some shrink wrap to re-seal it (and hold everything together) but I don't know where to find shrink wrap that big; I might just see if I can buy some from @onloop
```

---
## \#32 Posted by: Moja Posted at: 2016-01-05T01:41:26.435Z Reads: 83

```
If I'm getting 40v all the way up to the BMS doesn't that suggest that all the connections are sweet?
```

---
## \#33 Posted by: longhairedboy Posted at: 2016-01-05T01:42:04.353Z Reads: 83

```
I would also like some of that giant heat shrink wrappy stuff. My cell is taped up at the moment and i'd rather have it sealed up in that stuff.
```

---
## \#34 Posted by: cmatson Posted at: 2016-01-05T01:44:56.994Z Reads: 86

```
[quote="longhairedboy, post:33, topic:391"]
I would also like some of that giant heat shrink wrappy stuff.
[/quote]

I'll just get some extra and send it down your way- as long as you pay the shipping though since we live so far away :wink:
```

---
## \#35 Posted by: longhairedboy Posted at: 2016-01-05T01:47:05.368Z Reads: 84

```
i drive a tiny truck. it might be cheaper just to drive up there and get it. lol
```

---
## \#36 Posted by: lox897 Posted at: 2016-01-05T01:47:06.916Z Reads: 83

```
I think it's kind of like this one: http://m.ebay.com.au/itm/321494943091?_mwBanner=1

I remember when Whitepony said he used 195mm. Someone correct me if I'm wrong.
```

---
## \#37 Posted by: cmatson Posted at: 2016-01-05T01:47:14.580Z Reads: 84

```
Check each of the balancing connections: that's where my connection went wrong. They all seemed fine (and I had 40v in the end) but one of them was spotty. 

when checking the balancing connections (if you leave it plugged into the pcb, and just measure it by the pins going into the BMS) make sure not to short any connections by touching two pins with your volt meter.. I don't think that'd be too good.
```

---
## \#38 Posted by: cmatson Posted at: 2016-01-05T01:50:04.382Z Reads: 89

```
@lox897 might be onto something here with that ebay shrink wrap.. Maybe I could just find some on there. 

haha @longhairedboy I was only joking about the shipping :stuck_out_tongue_closed_eyes:

You can still drive your tiny truck up here if you want, or I can just pay a couple 'merican dollars and shoot some your way.
```

---
## \#39 Posted by: torqueboards Posted at: 2016-02-01T19:45:43.138Z Reads: 77

```
It's fine.. I have a user who uses the Enertion pack with a single motor and climbs hills.
```

---
## \#40 Posted by: Nasty Posted at: 2016-03-24T23:34:29.872Z Reads: 68

```
When the space cell is switched off, how much volts am I supposed to see at the power leads? I guessing ZERO. But in my case, I'm getting 4 volts.... That's odd right?
```

---
## \#41 Posted by: cmatson Posted at: 2016-03-25T02:48:42.470Z Reads: 66

```
I was getting 2v nominal with both of my space cell's.
```

---
