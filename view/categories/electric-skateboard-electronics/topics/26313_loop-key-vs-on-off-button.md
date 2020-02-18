# Loop key vs on off button

### Replies: 45 Views: 2899

## \#1 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T04:11:27.164Z Reads: 449

```
<img src="/uploads/db1493/original/3X/1/3/139b49e342275e269cf48dbe905b097e8e58d00a.JPG" width="241" height="499">What would be the difference between getting an XT loop key vs a torqueboards on off button? Also if you did go with xt, how do you know if to go with 60 or 90... where would you wire either on in this diagram?
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-28T04:49:53.769Z Reads: 429

```
You can basically put a loop key anywhere on the leads connected to the batteries (could be on the +,- or in between the batteries) all you're doing with the loop key is making a part of the circuit you can take out to open up the circuit so it's basically just a big removable "switch" of sorts.  I imagine the same holds true with antispark switches since same concept holds, if it's not a closed loop (circuit) then no current flows.  Regarding XT-90 vs 60, pretty sure the 60 is 60A and 90 is 90A either one will probably work but safer bet to just go with the 90s but in most cases you won't really be drawing that much amperage.

---

With the 12S you're going to be at a relatively high voltage so the amperage to drive the motor at it's peak wattage (or whatever it's pulling due to the throttle input) so you won't have super high amperage.  In a basic load situation (which this isn't but go with me a bit on this) if you have 2000W and the battery is at 50.4V then it would be 2000/50.4 = 40A of current to deliver that power.

That said I'm pretty sure I rarely ever actually have more than 400W draw for any substantial amount of time while accelerating though I haven't measured with instruments that can give instantaneous values on the go.  I need to get a bluetooth module for the VESC to get those details, basic volt/ammeter tells me it's about 400W-600W though while accelerating and about 4A*40V or 160W when up to speed and just cruising.

My battery is 2 5S 5Ah in series so 10S 5Ah effective or about 190Wh which makes sense with around 160W of draw (maybe a bit less) I can ride a bit over an hour and a half (probably actually closer to two but regen braking probably helps a small bit too)
```

---
## \#3 Posted by: lowGuido Posted at: 2017-06-28T07:04:15.589Z Reads: 382

```
This is my personal opinion. 
Loop key is best for a few reasons. 
If there is any problem with the electronics you can pull it out and you are more or less safe. Unless you have a short inside your battery pack. 
With a soft switch/FET switch/antispark switch your circuit is never really off as such. Like never physically disconnected.
You have to rely on potentially faulty electronics to protect you from potentially faulty electronics.
Ans when said that way it seems like a pretty stupid idea.

However. Antispark/FET switches look sexy and have blue LEDs so they are obviously the more popular choice.
```

---
## \#4 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T12:01:09.547Z Reads: 349

```
<img src="/uploads/db1493/original/3X/d/5/d53864397828585cdb6b35d5665e2cac629c4cf5.JPG" width="241" height="499">
If I put a loop key where the blue is, wouldn't electricity still be flowing through where the red is? Also, dexter from diy told me that on/ off is safer, and wouldn't ware out each time I use it...
```

---
## \#5 Posted by: lowGuido Posted at: 2017-06-28T12:39:25.267Z Reads: 324

```
sorry, where is the blue?[quote="NewbieBoardBuilder, post:4, topic:26313"]
on/ off is safer
[/quote]
lies.
And an XT-90s will never wear out.
```

---
## \#6 Posted by: L3chef Posted at: 2017-06-28T12:48:37.307Z Reads: 314

```
Click on the pic. Circle in middle.
Between possitive and negativ of 2 battery packs..
```

---
## \#7 Posted by: lowGuido Posted at: 2017-06-28T12:50:24.016Z Reads: 310

```
LOL whoops.. I didn't click on it.
yeah that's all good. you can loop key there, the current can't flow through the red because you have broken the circuit.
```

---
## \#8 Posted by: JLabs Posted at: 2017-06-28T12:51:10.148Z Reads: 302

```
[quote="NewbieBoardBuilder, post:4, topic:26313"]
on/ off is safer
[/quote]
Look up DIY switch and see how many people have problems with it failing. Then lookup XT90 And see how many people had one fail. I can only think of one off of the top of my head. 

I couldn't agree more with @lowGuido
```

---
## \#9 Posted by: lowGuido Posted at: 2017-06-28T12:54:52.891Z Reads: 286

```
the only time I have heard of an XT-90s fail is when it wasn't pushed in fully and the resistor burnt up.

for what its worth who you gonna believe? Me an electronic engineer who have been making e sk8 for years and is giving you advice out of his own time with nothing to gain, 
Or
someone who is trying to sell you a product? 
just sayin.
```

---
## \#10 Posted by: oldguy Posted at: 2017-06-28T13:02:03.292Z Reads: 283

```
I went with both. I put a loop key on the + lead and a manual switch on the - lead. I typically just use the switch, but I have the loop key there for emergencies when I may want to airgap my batteries and motor.
```

---
## \#11 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T19:15:45.513Z Reads: 270

```
<img src="/uploads/db1493/original/3X/d/d/dda783cff8095b5bcf01c82cbca1cd4be71e19e8.jpg" width="375" height="500">
I think I added the xt-90 loop key right... where would I add a voltage meter that could tell me my battery percentage. I know the negative and positive termenals, but of what!?!?
```

---
## \#12 Posted by: wafflejock Posted at: 2017-06-28T19:38:48.103Z Reads: 260

```
You can hook up the voltmeter to the + and - where it connects to the VESC, I just tapped the lines for voltage reading off of there.  If it is the type with a built in shunt and ammeter then it needs to just be inline with those battery lines before they go to the VESC.  If it's just voltage though then should just be black on - and red on +.  You're basically just reading the voltage of the battery bank by putting them where the battery lines go into the VESC.

---

Also the loop key will work fine where you have it, that's the same way I have it setup right now... trying to work on a slightly better box so I can swap out the batteries more easily myself (and for safety since the most recent fire post reminded me that's still an issue).
```

---
## \#13 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T20:05:34.174Z Reads: 239

```
[quote="wafflejock, post:12, topic:26313"]
and for safety since the most recent fire post reminded me that's still an issue
[/quote]

How'd yours catch fire?
Also, where do you buy your voltage meter? What would you look up to find them?
```

---
## \#14 Posted by: wafflejock Posted at: 2017-06-28T20:15:07.468Z Reads: 237

```
Oh sorry wasn't clear, mine didn't catch fire but just saw the post from another thread here where someone posted the video of their board ablaze.  Just something I've been paranoid about and figure it'd be nice to be able to bring an extra set of batteries with me for long days cruising around.  I got the volt/ammeter on Amazon I just searched for ammeters I'm pretty sure but they make them for measuring boat battery voltage.  The ammeter is probably not worth it just tells you instantaneous amperage but either need a shunt for the current to go through for it to measure the voltage drop and work out the current or you need a loop that goes around the wire, either way lots of trouble for little pay off, the voltage is good to know for a general idea of "fuel gauge".

---

Staring point for product searches of similar stuff:
https://www.amazon.com/gp/product/B00GLKQOKI/ref=oh_aui_search_detailpage?ie=UTF8&psc=1

Make sure if you get one similar to this it can deal with the voltage you're going to supply also good to be sure they don't need a separate power source (built in voltage regulator for it's ICs).
```

---
## \#15 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T20:20:07.321Z Reads: 224

```
Is there an easier way?
I just need to plug in a meter to see my percentage or voltage...
```

---
## \#16 Posted by: wafflejock Posted at: 2017-06-28T20:21:06.444Z Reads: 226

```
mmm not sure what you mean really only need two wires with the ones that just do voltage, one I linked has the ammeter part too so that complicates things. there are straight up voltage ones should be a few bucks cheaper

Only easier thing I can think you can do is temporarily using any old voltmeter to check the - and + on the battery leads, but for a permanent solution two wires is as easy as it can get.
```

---
## \#17 Posted by: wafflejock Posted at: 2017-06-28T20:25:09.195Z Reads: 224

```
I actually have one closer to this now
https://www.amazon.com/dp/B01DDQM6Z4?psc=1 

The loop that measures amperage pooped out so I just get the voltage reading from it now anyhow, I'm sure you can find the same thing without the amp reading in the first place should be like $10 probably on amazon (probably cheaper on ebay or the like if you have more patience than $)

---
Picture of mine in the board (I do like it :) but probably not for everyone )

https://raw.githubusercontent.com/shusain/eskatecontroller/master/Images/IMG_20170420_181015.jpg
```

---
## \#18 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T20:28:10.239Z Reads: 212

```
Do you have to program it to how many cells you have? Also, don't they have a max voltage they can withstand?
```

---
## \#19 Posted by: wafflejock Posted at: 2017-06-28T20:30:44.754Z Reads: 205

```
Yeah last one I linked has it in the title 5-120V above 120V you'd fry it I use it for 10S it works fine (it's not perfect but gives you the gist of how much voltage is left).  You don't have to program anything there is one button on it you can hold down to get it to recalibrate but otherwise so long as there is power going through the lines it will show you the voltage.
```

---
## \#20 Posted by: wafflejock Posted at: 2017-06-28T20:32:34.492Z Reads: 207

```
Actually another probably better option is to check out the metr app and maybe throw a bluetooth module on the VESC for getting the live data streamed to your phone or however that works but someone would need to fill in the details, with that you wouldn't have anything extra to put on the board really just a little circuit board on the VESC I believe (haven't used it).
```

---
## \#21 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T20:37:29.089Z Reads: 193

```
Okay...how many volts are 10s and 12s?
```

---
## \#22 Posted by: wafflejock Posted at: 2017-06-28T20:39:40.053Z Reads: 193

```
The voltage varies as the battery discharges.  So fully charged it's 4.2V per cell and the 10S is series so 10*4.2 = 42V, when fully drained would be 3.6ish V (I'm assuming we're talking about LiPo chemistry, other cells have different voltage per cell) usually 3.8V is considered "Nominal" or basically the mid point but you don't want to drain them to 0% (about 3.3ish V any lower and you will damage the cell) for max life too from what I gather.

VESC has configuration for low battery cut off to reduce power then cut it off completely to avoid draining your cells be sure to set those values to reasonable numbers.
```

---
## \#23 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T20:45:47.061Z Reads: 188

```
Okay, how long is battery life if you take care of it?
```

---
## \#24 Posted by: wafflejock Posted at: 2017-06-28T20:55:43.857Z Reads: 184

```
It varies from cell manufacturer to cell manufacturer and particular runs and exact conditions but I've heard basically 400 cycles (charge discharge) is reasonable if you take care of them well and they don't ever get too stressed from overheating or anything like that.  So far I haven't had any noticeable degradation for about a year and I recharge every few days basically.
```

---
## \#25 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T20:57:14.200Z Reads: 182

```
https://www.amazon.com/EDEALLINE-Meter-7-Digital-Capacity-Controller/dp/B00AKR8V9K
Thoughts?
```

---
## \#26 Posted by: wafflejock Posted at: 2017-06-28T20:58:41.677Z Reads: 165

```
These things are handy to have for sure just depends on if you want something permanent or not, that one you just plug the balance lead into and tells you overall voltage and individual cell so it's good for diagnostics but not good for mounting really since you'd need one for each battery.
```

---
## \#27 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T20:59:18.894Z Reads: 166

```
https://www.amazon.com/gp/aw/d/B00SCJOITA/ref=mp_s_a_1_3?ie=UTF8&qid=1498683471&sr=8-3&pi=AC_SX236_SY340_QL65&keywords=lipo+voltage&dpPl=1&dpID=513QVi2ujFL&ref=plSrch Maybe this simple thing instead?
```

---
## \#28 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T20:59:46.951Z Reads: 156

```
Shouldn't you combine your balance cables into one so charging becomes easier?
```

---
## \#29 Posted by: wafflejock Posted at: 2017-06-28T21:03:05.102Z Reads: 169

```
That is an option but it means you're charging pairs of cells so between the two in a pair things could become imbalanced.  I thought about doing it but probably better to either go BMS then or use a parallel charging board.   In either case my charging is already limited because of the Wattage of my charger so I'd really be better off just doing the two chargers thing... that's another motivation for the swappable battery pack type thing.  I'm trying to make it based on a NAS enclosure that has hot swap drive bays but for wrapping 5S 5Ah LiPos, could probably be adjusted for other sizes pretty easy too, doing it with OnShape.

Regarding the last listing from Amazon I use those for my quad copter their good but same deal made for reading the values off the balance leads, the one I linked you just have two wires to connect the +/- but you don't get individual cell info... the ones you linked there cycle through each cell then show the total battery voltage but you'd need two on the board one for each battery... so trade offs.
```

---
## \#30 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T21:09:11.118Z Reads: 158

```
So should I just stop worrying about BMS and balance cables, and just charge the two batteries separately? What if one is charged and one isn't?
```

---
## \#31 Posted by: wafflejock Posted at: 2017-06-28T21:17:34.929Z Reads: 158

```
Yeah I just balance charge them separately back to back.  You could go with BMS my reason for avoiding them when I did the build was there were a lot of threads saying it could cause problems because of the BMS "overactively" trying to balance the cells when the board wasn't being charged and other things that made it seem not worth the effort.

So far I haven't had any problems I believe if the cells were not balanced between the two batteries you wouldn't want to ride because you could end up putting more stress on the higher voltage battery and drain the already more empty battery below the safe per cell limit, but aside from that it shouldn't cause immediate problems if you accidentally connected the loop key with one charged and one not (I never tested this fyi, if they were hooked up in parallel one battery would dump into the other but otherwise you're just making a 10S or 12S imbalanced battery basically, by itself being imbalanced cells in series isn't dangerous just in use it's a problem since you can over drain some cells).

I've definitely had times I only added like +1V to each but I try to make sure they both end up within .01 or .02V of each other and redo the balance charge next time I get back.
```

---
## \#32 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T22:54:12.474Z Reads: 153

```
https://www.amazon.com/gp/aw/d/B00NZV7K3G/ref=mp_s_a_1_fkmr3_2?ie=UTF8&qid=1498690224&sr=8-2-fkmr3&pi=AC_SX236_SY340_QL65&keywords=lipo+voltage+battery+monitor+50v
I'm doing that...
```

---
## \#33 Posted by: NewbieBoardBuilder Posted at: 2017-06-28T22:55:24.748Z Reads: 160

```
https://www.amazon.com/EDEALLINE-Meter-7-Digital-Capacity-Controller/dp/B00AKR8V9K
Then this to make sure the batteries are functioning and even...
```

---
## \#34 Posted by: lowGuido Posted at: 2017-06-28T23:03:36.311Z Reads: 162

```
Here i made a video on how to attach a voltage meter.
https://youtu.be/rJweMkj0aOE
```

---
## \#35 Posted by: wafflejock Posted at: 2017-06-29T00:04:39.189Z Reads: 160

```
Nice cut out, I ended up using a drill to make a few holes then used a dremel to connect the dots and smooth things out and a file to get it big enough for the display to sink in.  The DROK type I used didn't have the cell selection with the nice battery percent but can generally work it out.  I just soldered the wires on top of the already big solder blobs on the battery cables going into the capacitor board attached to the VESC (no need to cut the silicon that way, although I ended up cutting it for other wires)
```

---
## \#36 Posted by: lowGuido Posted at: 2017-06-29T01:54:22.700Z Reads: 152

```
lol yeah I just used a blade from a stanley knife drew the shape and cut it (its in the other video) box is only plastic so its pretty easyto cut through.

oh wait you are talking about the board cut out... yeah I used a dremel multi tool.. so handy. but it was hard to get the corners because of the angles and blade width etc.
```

---
## \#37 Posted by: NewbieBoardBuilder Posted at: 2017-06-29T02:19:23.963Z Reads: 155

```
<img src="/uploads/db1493/original/3X/e/e/ee052773c5f37462e0a0710164cc34053101a92b.JPG" width="277" height="500">
Connect negative and positive here? Purple circles?
```

---
## \#38 Posted by: wafflejock Posted at: 2017-06-29T02:34:36.737Z Reads: 151

```
Yup diagram circles are good.  There are usually big blobs of solder on the fat wires going into the VESC that @lowGuido showed where he put his into the cables I just tacked mine on the top of that board, but if you want the display closer to the batteries then can do as he did and slice the silicon to patch them in there.
```

---
## \#39 Posted by: lowGuido Posted at: 2017-06-29T02:36:29.073Z Reads: 149

```
yeah the only reason I had to cut into the silicon on mine was because I had already hot glued the shit outa everything in there LOL
```

---
## \#40 Posted by: Hummie Posted at: 2017-06-29T02:38:14.181Z Reads: 156

```
i have one of those and rarely use it, but instead use one of the many similar that also discharge balances the cells.
```

---
## \#41 Posted by: NewbieBoardBuilder Posted at: 2017-06-29T02:43:12.697Z Reads: 151

```
https://youtu.be/2vfSURczARA
Everything you need to know of a BMS
```

---
## \#42 Posted by: wafflejock Posted at: 2017-06-29T03:14:56.220Z Reads: 150

```
Nice simple walk through but he didn't cover a few things brought up in the comments

"that power supply is weak! :)﻿"
"Yeah, but at $10 who cares :D It takes about 2.5 hours to charge, but for all I care it could take 6 hours. I only ride once a day.﻿"

---

"Hey I am deluxe, great video! But I have one question: Do you fully charge your batteries with this methode? Because I saw a video (https://www.youtube.com/watch?v=KYnxmXvkMYE) where someone tested this methode and saw that the batteries only charged to 60%. A lipo charger charges the battery to 100% because he first begins with a certain mAh (1100mAh) and voltage and steps up the voltage everytime until he reaches 4,2v then he steps up the mAh to 2200mAh.

So is that true?﻿"

"+SheepIsGaming a little bit true. My Lipo charger got my cells to 4.2V and my BMS gets my cells to 4.1V. so I would say more like 90% charged, not 60%. I don't notice a difference in range though, my board still goes over 10 miles, more than I can continuously handle.﻿"

---

If you just have 2 batteries it's not that big of a hassle and if you buy two chargers you can get both of them charged in less than half the time that BMS will take, plus I wouldn't trust hooking cheap stuff up to my relatively expensive cells... why risk it so I can have extra junk on the board that can get broken by vibrations.  I get it's convenient but I still see it as a lot of trade offs.

---

Edit also personally had a charger from quadcopter lipos so wasn't an extra cost.  If you go with a BMS would just say make sure you get one that isn't going to damage your cells or create more loose connections, if you do it do your research too.
```

---
## \#43 Posted by: NewbieBoardBuilder Posted at: 2017-06-29T12:07:04.304Z Reads: 129

```
I'm not gonna get one.. just two chargers simple
```

---
## \#44 Posted by: treenutter Posted at: 2017-07-03T15:12:26.194Z Reads: 117

```
[quote="NewbieBoardBuilder, post:21, topic:26313, full:true"]
Okay...how many volts are 10s and 12s?
[/quote]


These kinds of facts are easily found with a search. Please respect everyone's time and find the basic info on your own.
```

---
## \#45 Posted by: NewbieBoardBuilder Posted at: 2017-07-03T16:22:43.215Z Reads: 114

```
I'll try harder to figure things out
```

---
