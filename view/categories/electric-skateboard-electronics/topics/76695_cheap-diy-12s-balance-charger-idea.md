# Cheap DIY 12S balance charger idea

### Replies: 86 Views: 1835

## \#1 Posted by: janpom Posted at: 2018-12-01T15:06:15.709Z Reads: 256

```
Most people seem to be using bypassed BMS-es for their battery pack since it's a simple and cheap solution. I don't like it for the following reasons:

- BMS takes up space in the enclosure.
- No feedback. You have to trust the BMS to do the right thing. You don't get the individual cell voltage reading (unless you use a smart BMS).
- If you charge fast, the cell balancing may be insufficient as pointed out by @chaka [here](https://www.electric-skateboard.builders/t/float-charging-why-you-shouldnt-bypass-the-bms/39879?u=janpom).

I would much rather use a balance charger than a BMS. The problem is that 12S balance chargers are rare and expensive.

Here's how I think one could make one with low cost. The idea is inspired by the ["frankenstein charger"](https://www.electric-skateboard.builders/t/first-build-mono-6374-vesc-10s3p-bms-90mm-flywheel/37257/14?u=janpom) by @Luuke, which basically uses ten 1S chargers at the same time to charge individual battery cells. While I do like that it seems a bit too bulky and complicated. An alternative would be to use:

- 13 "small" relays to create a connection to each individual cell out of the 12
- only one 1S charger
- 1 "fat" relay for the whole 12S pack
- 12S "brick" charger
- MCU (Arduino)
- small/cheap OLED or TFT display for monitoring

The idea is that the MCU would first activate the "fat relay" for the brick charger to charge the full pack without balancing. While it's charging, individual cell voltages would be monitored using the small relays. This would be done by connecting one cell to the MCU at the time and use an ADC enabled pin for reading the voltage. This doesn't need to be done too often (limited number of relay operations would not be a problem).

Once one of the cells reaches the full charge, the MCU would cut off the brick charger and would use the 1S charger to finish charging one cell at the time. Again, the "small" relays would be used for this phase.

Charging individual cells this way would be slow, but as long as good cells are used, they shouldn't get too much out of balance, so this balancing phase should be short.

The nice thing about this is that it should work for any number of cells. For 13S or 14S, just add one or two more "small" relays. Also, having a custom FW for the MCU would allow full customization of the charge process, such as the max cell voltage, charging current, etc.

Would this work or is there an obvious problem I'm overlooking? I'm tempted to build this for science. :smiley:
```

---
## \#2 Posted by: Mich21050 Posted at: 2018-12-01T15:08:07.317Z Reads: 225

```
Wouldn't it be better to use mosfets? They are smaller and cheaper :smile:
```

---
## \#3 Posted by: janpom Posted at: 2018-12-01T15:13:35.776Z Reads: 221

```
Yes, maybe. It's actually beyond my limited electronics background whether it would be better. I have a pretty good idea about how to do it with relays. With mosfets, there's always some voltage drop across the mosfet that you would need to account for. I like to keep things simple.
```

---
## \#4 Posted by: Mich21050 Posted at: 2018-12-01T15:15:11.579Z Reads: 216

```
Sure. They are better for prototyping and easier.. maybe I can help you once you get everything up and running with the relais
```

---
## \#5 Posted by: deltazeta Posted at: 2018-12-01T23:49:59.274Z Reads: 195

```
maybe you could use a buck to get rid of the 1s charger
```

---
## \#6 Posted by: pat.speed Posted at: 2018-12-01T23:54:04.096Z Reads: 191

```
Another solution is to have a double balance lead, one goes to the bms and one goes to a plug on your enclosure. That way you can check all cells as they balance
```

---
## \#7 Posted by: Friskies Posted at: 2018-12-02T01:15:39.447Z Reads: 177

```
Just get a diebiems and use the OLED or integration with the metr app I know it's not the cheapest option or the smallest but it will do everything and more than what you require.
```

---
## \#8 Posted by: b264 Posted at: 2018-12-02T01:21:13.545Z Reads: 176

```
[quote="janpom, post:1, topic:76695"]
The problem is that 12S balance chargers are rare and expensive.
[/quote]

The other problem is waterproofing a 13-wire connection instead of a 2-wire connection.  Also, how quickly it wears out with plug/unplug cycles.
```

---
## \#9 Posted by: b264 Posted at: 2018-12-02T01:23:30.363Z Reads: 172

```
[quote="janpom, post:3, topic:76695"]
With mosfets, there’s always some voltage drop across the mosfet that you would need to account for.
[/quote]

That's the old-school bipolar transistors.  MOSFETs you can view more closely as like a 50mΩ resistor instead of a diode with a voltage drop.
```

---
## \#10 Posted by: mynamesmatt Posted at: 2018-12-02T03:27:08.322Z Reads: 164

```
I've wired my balance leads in parallel. This way I can balance my batteries (which are each 5s) with my BMS while also monitoring eat cells voltage through a maximum 6s battery checker from Hobbyking. I have the main negative from each balance lead on a switch so I can turn the voltage checkers on and off to see how balanced my cells are
![MSGR_PHOTO_FOR_UPLOAD_1531658522803|257x500](upload://madPWuXuTEAD3PcvHag1CXDfOGU.jpeg) ![20180622_140311|375x500](upload://iFSUxrje46YbDeJKL2zeD2d8CQV.jpeg) ![20180715_224021|666x500](upload://6Bb8EzC54Fg4F7bBv1ofKhUKxG2.jpeg)
```

---
## \#11 Posted by: janpom Posted at: 2018-12-02T07:17:24.175Z Reads: 156

```
[quote="b264, post:8, topic:76695"]
The other problem is waterproofing a 13-wire connection instead of a 2-wire connection.
[/quote]

There's [this 12 pin waterproof connector](https://www.amazon.com/Waterproof-Connector-Aviation-Plug-female-Socket-male/dp/B07BK3MYXV?th=1). Yeah, one pin short for 12S.

[quote="Friskies, post:7, topic:76695"]
Just get a diebiems
[/quote]

I like DieBieMS a lot, even more now with the Metr Pro integration. It would be a go to solution for me if it wasn't so bulky. I wish there was a charge only DieBieMS lite. You could then use it both inside the enclosure or outside (basically use it as a balance charger). I mean, you could use it as a balance charger even now. It would still be cheaper than getting a regular 12S balance charger. It would just be a complete waste of the nice features (e-switch, discharge protection) that you wouldn't use at all.

[quote="mynamesmatt, post:10, topic:76695"]
I can balance my batteries (which are each 5s) with my BMS while also monitoring eat cells voltage through a maximum 6s battery checker
[/quote]

I like that. I thought about doing something along those lines as well.

[quote="mynamesmatt, post:10, topic:76695"]
I have the main negative from each balance lead on a switch so I can turn the voltage checkers on and off to see how balanced my cells are
[/quote]

These cheap checkers use voltage dividers to get the individual cell voltage readings. If your switch is only on the negative lead and the other balance leads remain connected to the checker, I believe it will still discharge the cells a little bit. There will be a small current going across the resistors of the voltage dividers. Probably not a big problem, but still something to keep in mind.
```

---
## \#12 Posted by: janpom Posted at: 2018-12-02T07:29:34.829Z Reads: 143

```
After a little more thinking about this, I can't see a good way of making it work with 13 relays/MOSFETs (switches) for 12 cells. I think I would need 24 switches, 12 of which would go to the negative of each cell and 12 to each positive. That's still not a showstopper since both relays and MOSFETs can be found for very cheap.

What I see is a more serious problem, though, is that it would be pretty dangerous to wire things up in that way. If more than 1 switch in any of the 12-switch group got closed, that would create a short over the battery cells and destroy the battery. A bug in the controller would then be a disaster.  I think I know how to make a hardware protection for this, but with that it's already drifting away from the intended "simple solution". I may still build this for science. :smiley:  At least for 3S to start with.
```

---
## \#13 Posted by: mynamesmatt Posted at: 2018-12-02T08:25:51.341Z Reads: 128

```
[quote="janpom, post:11, topic:76695"]
I believe it will still discharge the cells a little bit
[/quote]

nah once the negative rail is disconnected it can't measure across the cells (pretty sure)
```

---
## \#14 Posted by: pat.speed Posted at: 2018-12-02T08:30:42.777Z Reads: 127

```
Not sure about that, I have a batterymedic from HK and I had to have a switch on the first 3 wires to cut the power, even then it was probably still drawing power
```

---
## \#15 Posted by: janpom Posted at: 2018-12-02T08:42:36.196Z Reads: 131

```
I didn't say it would "measure" across the cell, but you would still have resistors between cells and small current would flow there, which would only be turned into heat.

With the negative connected you have something like [this](https://www.falstad.com/circuit/circuitjs.html?cct=$+1+0.000005+10.20027730826997+50+5+43%0Av+64+80+96+80+0+0+40+4.2+0+0+0.5%0Av+112+80+144+80+0+0+40+4.2+0+0+0.5%0Av+160+80+192+80+0+0+40+4.2+0+0+0.5%0Av+208+80+240+80+0+0+40+4.2+0+0+0.5%0Av+256+80+288+80+0+0+40+4.2+0+0+0.5%0Av+304+80+336+80+0+0+40+4.2+0+0+0.5%0Av+352+80+384+80+0+0+40+4.2+0+0+0.5%0Av+400+80+432+80+0+0+40+4.2+0+0+0.5%0Av+448+80+480+80+0+0+40+4.2+0+0+0.5%0Av+496+80+528+80+0+0+40+4.2+0+0+0.5%0Av+544+80+576+80+0+0+40+4.2+0+0+0.5%0Av+592+80+624+80+0+0+40+4.2+0+0+0.5%0Aw+160+80+160+112+0%0Aw+208+80+208+112+0%0Ar+160+112+160+160+0+20000%0Ar+160+160+160+208+0+2200%0Aw+160+160+144+160+0%0Aw+144+160+144+272+0%0Aw+64+80+64+208+0%0Aw+112+208+160+208+0%0Aw+160+208+208+208+0%0Ar+208+160+208+208+0+2200%0Aw+96+80+112+80+0%0Aw+144+80+160+80+0%0Aw+192+80+208+80+0%0Aw+240+80+256+80+0%0Aw+288+80+304+80+0%0Aw+336+80+352+80+0%0Aw+384+80+400+80+0%0Aw+432+80+448+80+0%0Aw+480+80+496+80+0%0Aw+528+80+544+80+0%0Aw+576+80+592+80+0%0Aw+208+160+192+160+0%0Aw+192+160+192+272+0%0Aw+240+160+240+272+0%0Aw+256+160+240+160+0%0Ar+208+112+208+160+0+30000%0Ar+256+160+256+208+0+2200%0Aw+208+208+256+208+0%0Aw+256+80+256+112+0%0Aw+288+160+288+272+0%0Aw+304+160+288+160+0%0Ar+256+112+256+160+0+43000%0Aw+256+208+304+208+0%0Aw+304+80+304+112+0%0Aw+336+160+336+272+0%0Aw+352+160+336+160+0%0Ar+304+112+304+160+0+47000%0Aw+304+208+352+208+0%0Aw+352+80+352+112+0%0Aw+384+160+384+272+0%0Aw+400+160+384+160+0%0Ar+352+112+352+160+0+51000%0Aw+352+208+400+208+0%0Aw+400+80+400+112+0%0Aw+432+160+432+272+0%0Aw+448+160+432+160+0%0Ar+400+112+400+160+0+62000%0Aw+400+208+448+208+0%0Aw+448+80+448+112+0%0Aw+480+160+480+272+0%0Aw+496+160+480+160+0%0Ar+448+112+448+160+0+75000%0Aw+448+208+496+208+0%0Aw+496+80+496+112+0%0Aw+528+160+528+272+0%0Aw+544+160+528+160+0%0Ar+496+112+496+160+0+82000%0Aw+496+208+544+208+0%0Aw+544+80+544+112+0%0Aw+576+160+576+272+0%0Aw+592+160+576+160+0%0Ar+544+112+544+160+0+91000%0Aw+544+208+592+208+0%0Aw+592+80+592+112+0%0Aw+624+160+624+272+0%0Aw+640+160+624+160+0%0Ar+592+112+592+160+0+100000%0Aw+592+208+640+208+0%0Aw+640+80+640+112+0%0Aw+624+80+640+80+0%0Ar+112+160+112+208+0+2200%0Aw+112+208+64+208+0%0Aw+112+160+96+160+0%0Aw+96+160+96+272+0%0Ar+112+112+112+160+0+10000%0Aw+112+80+112+112+0%0Ar+304+160+304+208+0+2200%0Ar+352+160+352+208+0+2000%0Ar+400+160+400+208+0+2000%0Ar+448+160+448+208+0+2000%0Ar+496+160+496+208+0+2000%0Ar+544+160+544+208+0+2000%0Ar+592+160+592+208+0+2000%0Ar+640+160+640+208+0+2000%0Ar+640+112+640+160+0+110000%0A). Without it, you have [this](http://tinyurl.com/yc5goe5f).
```

---
## \#16 Posted by: janpom Posted at: 2018-12-02T08:48:36.011Z Reads: 130

```
Maybe something like this would work for toggling between individual cells. Good old binary tree. :) For 8S, it would require 14 two-state relays, organized into three rows. Each row would be controlled with the same signal.

This would be pretty safe. It can never create a short across a battery cell, even if the relays in the same row don't switch exactly at the same time. It could create a short across the charger, but that can certainly be dealt with.

![IMG_1544|666x500](upload://xBWl6NiwMkBvd98MrFe3npeAXMq.jpeg) 

12S would then require 22 relays organized into 4 rows.
```

---
## \#17 Posted by: Andy87 Posted at: 2018-12-02T08:53:01.791Z Reads: 125

```
Why not just using a smart bms and use it as „balance“ adapter on your charger.
Just route the balance leads out of your enclosure on the waterproof plug.
Than make an adapter plug from the bms to the enclosure and you good to go.
Brick charger - smart bms - battery
The smart charger is about 25€ and you can use it than on all 12s batteries you have.

I hope that’s working 😅
As min it was my plan when the smart bms finally arrive.

I don‘t like to don’t monitor the individual cell voltage with a usual bms.
I don’t need the e-switch function of a discharge bms. 
And a fuse in line is way much smaller.


Edit: i‘m not 100% sure yet, but I think with the smart bms you even can set the balance voltage to 4.1v per cell (or any other value you want).
This way you even can adjust the charge level and don’t need to worry that you hit your cells when „fully“ charged you need to hit the breaks
```

---
## \#18 Posted by: janpom Posted at: 2018-12-02T08:57:34.655Z Reads: 119

```
[quote="Andy87, post:17, topic:76695"]
Why not just using a smart bms and use it as „balance“ adapter on your charger.
[/quote]

Yes, I thought about that too. Is there a smart BMS that you can interface with, though? Ideally one with a clearly documented communication protocol? I don't want one that only sends data to my cell phone with a proprietary protocol. Plus, installing some Chinese app from an untrusted source on my phone would make me feel queasy.
```

---
## \#19 Posted by: pat.speed Posted at: 2018-12-02T09:04:31.250Z Reads: 114

```
You can buy bms modules from AliExpress that allow you to change all of the parameters from your phone or computer. I wanted to use one but it’s a little too big for my integrated deck
```

---
## \#20 Posted by: Andy87 Posted at: 2018-12-02T09:07:57.969Z Reads: 117

```
I‘ll get this one
https://s.click.aliexpress.com/e/cHKIZBXy
Unfortunately it is not so much documtation about it and you will need an app which is luckily not only in Chinese. (iOS user so not sure how it is with apps you can get in the playstore and if you can trust them)

I know some guys here already use this bms and on endless sphere they also speak a lot about it and it seems to work pretty good.

As mine just on the way, so all I say is all I read here. Hope it will arrive next week. 
I can hold you up to date how it’s working if you want.
```

---
## \#21 Posted by: deucesdown Posted at: 2018-12-02T09:10:41.117Z Reads: 104

```
https://github.com/simat/BatteryMonitor/wiki/Generic-Chinese-Bluetooth-BMS-communication-protocol
```

---
## \#22 Posted by: Friskies Posted at: 2018-12-02T09:30:29.011Z Reads: 94

```
[quote="janpom, post:18, topic:76695"]
Is there a smart BMS that you can interface with, though? Ideally one with a clearly documented communication protocol
[/quote]

[quote="Friskies, post:7, topic:76695"]
Just get a diebiems
[/quote]

Maybe look it up. It's literally what you are looking for and more.
```

---
## \#23 Posted by: janpom Posted at: 2018-12-02T09:43:25.374Z Reads: 96

```
@Friskies I'm aware of DieBieMS and I have commented on it above. I like it but it just seems a complete waste to use it as a balance charger only.
```

---
## \#24 Posted by: Friskies Posted at: 2018-12-02T09:50:12.560Z Reads: 94

```
Why charge only? It can handle more than most will be able to throw it it in regards to discharge too... You're talking about bulk etc buy how many relays were you going to wire together??
```

---
## \#25 Posted by: janpom Posted at: 2018-12-02T11:00:19.613Z Reads: 92

```
@Friskies Bulky is only an issue if you were to put the thing inside the enclosure. That was never the intention.

The issue with DieBieMS is that either you put it inside the enclosure, in which case you have to make a lot of space for it, or you use it outside of the enclosure as a balance charger, in which case you're wasting a nice product.
```

---
## \#26 Posted by: Luuke Posted at: 2018-12-02T11:19:05.937Z Reads: 88

```
Meanwhile i use a 80A bestech BMS for daily use. it is so easy to use and trustable.
every 2 month I use my "frankenstein charger" to charge the cells independent from the bms.
therefor I have to open enclosure, unplug the BMS and plug the charger instead.
Not a big deal to do so...
```

---
## \#27 Posted by: Friskies Posted at: 2018-12-02T11:28:28.099Z Reads: 84

```
It just seems a little counter intuitive. If you are that worried about unbalanced P groups then you are probably just better off finding a way to incorporate a discharge BMS. There are still some really compact 60a discharge units around.
LHB recommended one from batterysupports which seems to be pretty tiny..

http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html
```

---
## \#28 Posted by: janpom Posted at: 2018-12-02T12:48:52.149Z Reads: 81

```
[quote="Andy87, post:20, topic:76695"]
I‘ll get this one
https://s.click.aliexpress.com/e/cHKIZBXy
[/quote]

This looks like a good option, especially with the link that @deucesdown has shared. I will get one too for experimenting. Which one are you getting? The cheapest one to bypass or the 60A one?
```

---
## \#29 Posted by: Andy87 Posted at: 2018-12-02T12:55:18.136Z Reads: 77

```
Sure the cheapest one.
I anyhow use it only in time of charging and I think I will not charge with more than 20a 😜
I ordered a pc module too, but not sure if it’s really needed.
```

---
## \#30 Posted by: janpom Posted at: 2018-12-02T13:24:34.151Z Reads: 72

```
Sounds good. I just ordered the same. If it works, that's an easy way to implement a 12S balance charger. If it doesn't, I'll just have to build my binary relay tree. :smiley:
```

---
## \#31 Posted by: Acido Posted at: 2018-12-02T13:39:44.797Z Reads: 72

```
that bms is great, in the pc software you can edit more things you can even imagine!
```

---
## \#32 Posted by: Andy87 Posted at: 2018-12-02T13:41:23.475Z Reads: 74

```
Did you notice that you get one for LiIon?
The one I linked is for lifepo4 cells.
I was speaking with the shop and they said they will set it up for lipo/LiIon.
If you didn’t, better write them a message too.
```

---
## \#33 Posted by: janpom Posted at: 2018-12-02T14:11:12.643Z Reads: 71

```
Ah, I didn't notice there were multiple versions. I ordered from [this link](https://www.aliexpress.com/item/48V-Smart-bluetooth-BMS-system-with-30A-discharge-current-for-54-6V-Battery-system-E-Bike/32733414980.html?spm=a2g0s.9042311.0.0.21904c4dQqEorQ), so I should be good. Thanks for the warning though.

Now I have to figure out how do I install their Windows app on my Mac. :slight_smile:
```

---
## \#34 Posted by: janpom Posted at: 2018-12-02T14:14:52.383Z Reads: 75

```
Could anyone help me choose an appropriate relay for that [binary relay tree](https://www.electric-skateboard.builders/t/cheap-diy-12s-balance-charger-idea/76695/16?u=janpom)? Ideally it would possible to switch it with 5V and it would be rated at least 5A at 5V DC. I guess some solid state relay would be best? Oh, and it has to be 2 pole. Does that even exist?
```

---
## \#35 Posted by: Andy87 Posted at: 2018-12-02T14:26:00.399Z Reads: 77

```
The one you linked is for 13s.
That’s ok for you?
```

---
## \#36 Posted by: janpom Posted at: 2018-12-02T14:28:52.648Z Reads: 73

```
Uh, good point. Do you think it won't work with 12S only?
```

---
## \#37 Posted by: Andy87 Posted at: 2018-12-02T14:32:46.286Z Reads: 74

```
Not sure. Normal bms usually work if you just don’t wire the last pin.
Maybe @Acido know if it would work.
```

---
## \#38 Posted by: janpom Posted at: 2018-12-02T14:36:28.125Z Reads: 71

```
I messaged the seller. They actually don't offer a 12S for li-ion. Only the lifepo4. Weird.
```

---
## \#39 Posted by: Andy87 Posted at: 2018-12-02T14:38:40.205Z Reads: 71

```
Strange, than let’s see what i‘ll get 😬😅
```

---
## \#40 Posted by: Acido Posted at: 2018-12-02T14:40:32.465Z Reads: 77

```
i didn't read the full thread but with what i read i understand that he doesn't trust the bms to do the balancing and that he want to be able to check on the voltages

this bms has an app and you can see the exact voltages in it and its not that big either so i see no point of making the "charger" when the bms has all he needs
```

---
## \#41 Posted by: Acido Posted at: 2018-12-02T14:41:06.860Z Reads: 73

```
There is an option for li ion, i built a pack with it recently
```

---
## \#42 Posted by: Andy87 Posted at: 2018-12-02T14:43:30.366Z Reads: 70

```
The question is just if the 13s he ordered would work with 12s too
```

---
## \#43 Posted by: Acido Posted at: 2018-12-02T14:44:07.369Z Reads: 74

```
ohhh, that i have no idea
```

---
## \#44 Posted by: totalgeek9224 Posted at: 2018-12-02T14:55:43.687Z Reads: 71

```
https://www.aliexpress.com/item/Bluetooth-smart-BMS-with-100A-constant-current-suitable-for-10S-36V-11S-12S-13S-48V-14S/32849172235.html?spm=2114.10010108.1000023.6.5fb179512IXJSI

Would this be suitable?
```

---
## \#45 Posted by: deucesdown Posted at: 2018-12-02T15:07:59.028Z Reads: 71

```
https://www.lithiumbatterypcb.com/product-instructionev-battery-pcb-boardev-battery-pcb-board/ev-battery-pcb-board/smart-bms-of-power-battery/

I believe this is the oem. They can supposedly be reconfigured for number of cells in series by jumping some solder pads and changing software settings. I tried this on one and no luck for me.

There's also an external display..
```

---
## \#46 Posted by: janpom Posted at: 2018-12-02T15:25:43.037Z Reads: 75

```
I checked both links and both offer the 12s only for lifepo4. @Andy87, sounds like each of us will have his challenge. You make yours work with li-ion. I make mine work with 12s. Seems like a lot of fun to be had for 40 bucks. :smiley:
```

---
## \#47 Posted by: Andy87 Posted at: 2018-12-02T15:36:05.700Z Reads: 77

```
I asked the producer before I ordered and they said I just need to write them when I placed the order and they will sent it for LiIon set up.
I asked after they sent and they said they sent the right type.
Let’s hope it is like this 😅 but AliExpress... you never know what you get 😂
```

---
## \#48 Posted by: janpom Posted at: 2019-01-03T23:40:58.164Z Reads: 74

```
@Andy87 Have you used your smart BMS yet? Does it work for you? I received mine about a week ago. Of course it's 13S, even though the seller told me they would send 12S. :roll_eyes: Fortunately, I figured it can be easily configured for 12S. It's a matter of shorting the BC3 and BC4 pins and configuring 12 cells using the PC app they provide. The seller even responded to my email and confirmed this is the right way to do it.

I'm still having some issues though. First, when I connect it to the computer and read the cell voltages in the PC app, the first cell is very flaky. It's exactly the same problem as what's shown in [this video](https://youtu.be/ClGmMY0kXvQ?t=315), so I assume it's a bug.

I also tried connecting the BMS to my Android tablet using the Bluetooth module and that worked fine. However, I'm getting completely wrong cell voltages there. The first two cells appear as dead (around 0.5V) and the third cell voltage is flaky in the same way as the first cell in the PC app. The remaining 9 voltages look OK.

So the software seems buggy. I wonder if the MCU reads correct voltages and it only incorrectly communicates them to the computer/phone or if it has wrong voltages as well -- that wouldn't be good for cell balancing.
```

---
## \#49 Posted by: deucesdown Posted at: 2019-01-04T01:21:49.640Z Reads: 68

```
I had a similar experience with one there I reconfigured the series count. :(  

But I have multiple other units, unmodified, that work as expected.
```

---
## \#50 Posted by: Andy87 Posted at: 2019-01-04T07:07:00.035Z Reads: 68

```
Unfortunately I didn’t have had a time before Christmas. Broken motors etc. took more time than expected. As soon as I have the bms installed i‘ll give you a Feedback
```

---
## \#51 Posted by: janpom Posted at: 2019-01-04T07:50:00.491Z Reads: 71

```
@deucesdown Thanks for the info. Have you played with the UART connection to the BMS? I wasn't able to get it working with Arduino.
```

---
## \#52 Posted by: deucesdown Posted at: 2019-01-04T15:45:12.241Z Reads: 71

```
I've not had a go yet, as the janky apps work well enough for me (barely). 

But hey I've been thinking about that link you sent to Luuke's stuff, with the isolated ac-dc 5v buck converters and TP4056 modules. I ordered up a bunch of stuff. I'm thinking, per channel, put in a voltmeter, TP4056 and a 5v dc-dc converter.

voltmeter something like this (There are 2 wire and 3 wire versions, and versions with a calibration pot. Gotta find one that has the required voltage range and has 2 digits precision):

https://www.ebay.com/itm/DC-0-30V-Wires-LED-3-Digital-Mini-Voltmeter-Meter-Display-Voltage-Panel-Tester/173216068573

This scary isolated buck converter running off mains voltage

https://www.banggood.com/10pcs-AC-DC-5V-2A-10W-Switching-Power-Bare-Board-Stabilivolt-Power-Module-AC-100-240V-To-DC-5V-p-1196264.html

And TP4056 modules. There are 3amp versions, also scary! I think 3 TP4056 in parallel, how is termination handled? (shoutout to @Hummie I think you found these first) 

https://www.ebay.com/itm/1PCS-TP4056-4-2V-3A-High-Current-Lithium-Battery-Charging-Board-Charger-Module/201743594219

Hm or this, TP5000, 2A, includes heat sink. More likely to work than the 3A one.

https://www.ebay.com/itm/TP5000-3-6v-4-2v-2A-Charger-Board-3-7v-Lithium-3-2v-LiFePO4-Battery-Charging/152987945653
```

---
## \#53 Posted by: Hummie Posted at: 2019-01-04T17:34:19.225Z Reads: 66

```
https://www.ebay.com/itm/1PCS-TP4056-4-2V-3A-High-Current-Lithium-Battery-Charging-Board-Charger-Module/201743594219

Oo three amps. Nice find. Unfortunately someone said hooking 12 of these up to the battery to charge and balance at the same time would cause a short.  Damn I want to do that.  Who can tell me that’s a bad idea again @Blasto. Who else knows electronics?  Maybe could add something extra?
```

---
## \#54 Posted by: Blasto Posted at: 2019-01-04T17:45:35.696Z Reads: 63

```
If all the cells are inside a pack, you'll need an isolated power supply for each.

you made me go through my old shit, this is what i found lol

https://www.electric-skateboard.builders/t/why-not-make-a-balance-charger-with-these/38934/4?u=blasto
```

---
## \#55 Posted by: deucesdown Posted at: 2019-01-04T17:52:36.074Z Reads: 62

```
I linked the isolated power supplies, under $2 per piece.
```

---
## \#56 Posted by: Hummie Posted at: 2019-01-04T17:59:17.997Z Reads: 66

```
[quote="Kug3lis, post:48, topic:38934, full:true"]
Just remembered if you going to charge a battery pack through balancer leads with multiple chargers connected you will have a problem, because between cells its not real ground, its + of cell before and those small chargers have B- connected to ground so if you have multiple chargers your going to shorten the circuit
[/quote] 
Im getting conflicting answers. Maybe linear supply vs switching?
```

---
## \#57 Posted by: deucesdown Posted at: 2019-01-04T18:03:15.440Z Reads: 64

```
You've seen this?

https://www.electric-skateboard.builders/t/first-build-mono-6374-vesc-10s3p-bms-90mm-flywheel/37257/14

Isolated ac-dc 5v supplies, one per TP4056 charger.

It's been done. It's just crazy :) I want one too.
```

---
## \#58 Posted by: Hummie Posted at: 2019-01-04T18:10:29.664Z Reads: 65

```
This guy used a separate supply for each module.  Hoping @Blasto explains how his buddy uses one supply for multiple.  Smaller cheaper.
```

---
## \#59 Posted by: Blasto Posted at: 2019-01-04T18:12:03.421Z Reads: 65

```
The cells are individual, not in a “pack”
```

---
## \#60 Posted by: Hummie Posted at: 2019-01-04T18:27:21.096Z Reads: 64

```
Aha. Of course. Bummer.  So need a supply for each cell.  As said
```

---
## \#61 Posted by: janpom Posted at: 2019-01-05T00:49:54.973Z Reads: 61

```
I turned out the problems I had were due to the B- not being connected. I thought it's the same rail as the BC0, but apparently not. Now it works like a charm. I started to work on intercepting the communication between the PC module and the BMS. It turns out the data sent by the PC module is exactly as documented [here](https://github.com/simat/BatteryMonitor/wiki/Generic-Chinese-Bluetooth-BMS-communication-protocol) and that's exactly what I used in my last attempt to connect an Arduino. I must have done something wrong. Will try again.

BTW, when I connect the charger, the voltage on the first and the last cell increases quite a bit. Without the charger connected, I have all cells pretty much in balance, say around 4.10V. When I connect the charger, all voltages go up a little bit, maybe to 4.15V, but the first and the last cell go much higher, like 4.25V. Measured by both the BMS and multimeter. Is that normal?
```

---
## \#62 Posted by: deucesdown Posted at: 2019-01-05T01:12:14.003Z Reads: 65

```
If you hook up the charger without bms, does it have the same behavior?
```

---
## \#63 Posted by: janpom Posted at: 2019-01-05T08:31:21.701Z Reads: 70

```
yes
10char
```

---
## \#64 Posted by: janpom Posted at: 2019-01-05T11:12:49.868Z Reads: 72

```
Woohoo, looks like I'm getting somewhere. :slight_smile:

![image|432x500](upload://4DsHoGDNNX42wQ8noJq87xZLRZ0.jpeg)

![image|375x500](upload://7usbcf6P2KDUVMcwfWy6PoxpKkR.jpeg)
```

---
## \#65 Posted by: deucesdown Posted at: 2019-01-05T15:05:38.033Z Reads: 67

```
[quote="janpom, post:63, topic:76695"]
yes
[/quote]

Sounds like a problem with the pack? Not the bms. As if the resistance of the series connetions varies (a lot?). Or weak cells in the first and last groups but that seems unlikely.

[quote="janpom, post:64, topic:76695"]
Woohoo, looks like I’m getting somewhere
[/quote]

Ooh so exciting. 2 input vega coming soon?
```

---
## \#66 Posted by: janpom Posted at: 2019-01-05T15:31:22.324Z Reads: 66

```
[quote="deucesdown, post:65, topic:76695"]
Sounds like a problem with the pack? Not the bms. As if the resistance of the series connetions varies (a lot?).
[/quote]

That was my first thought, too. However, if that was the case, wouldn't the cells get out of balance when charging/discharging? I do not balance the cells. I merely monitor the voltages. I only have the battery pack shortly, but there were at least 3 discharge/charge cycles and the cells apparently discharge/charge evenly. The first cell is slightly (~0.02V) higher than the other cells, but it has been like that from the beginning and isn't drifting away. All other cells are within 0.005V difference.

[quote="deucesdown, post:65, topic:76695"]
Ooh so exciting. 2 input vega coming soon?
[/quote]

I just needed something with display and UART and realized I have a fair amount of such devices on hand. :smiley: There have already been requests for displaying individual cell voltages on Davega. I said no to that, but I'm rethinking now. The problem is that there's only one UART on ATMEGA328 and also not many people use the LLT smart bms. Instead, I'm thinking of making a simple I2C cell voltage monitoring module that I could hook up with the Davega I2C pins, which are still unoccupied. The module could be just a voltage divider and three ADS1115 on the same I2C bus. These are 4-channel 16bit ADC modules, so by using three, up to 12S would be supported. The resolution would be more than enough with 16bit ADC. I'm not sure how accurate these ADS1115 are though. I'll probably buy some and do some testing.
```

---
## \#67 Posted by: deucesdown Posted at: 2019-01-06T17:40:04.620Z Reads: 60

```
I've been wanting per cell monitoring pretty bad, bad enough to at least attempt to put smartbms in every board.

From ignorantly googling around, voltage divider for something like 12s will have stacking error, and resistors have quite a bit of variability?

ASD1115, looks like it has 4 16bit ADC, but that's in single ended mode (common ground). In differential mode there are only ADC.

I think a BMS chip (maybe from TI, maybe same family as smartbms or diebms?) will have all the voltmeters in one easy to use package, and probably cost less than rigging a bunch of ADC and voltage dividers?
```

---
## \#68 Posted by: janpom Posted at: 2019-01-06T19:09:12.659Z Reads: 61

```
[quote="deucesdown, post:67, topic:76695"]
From ignorantly googling around, voltage divider for something like 12s will have stacking error, and resistors have quite a bit of variability?
[/quote]

I have actually played with it a few months back. Here's what I have done on a perfboard with two ATTINY84 chips (I had to use two to get enough ADC pins) and a bunch of resistors.

![IMG_1603|608x500](upload://xeIi4EWL9PiVuO4tsq1vFtgLldP.jpeg)
![IMG_1604|578x500](upload://smXFsrUf5E1yUFlbvh1YWdYBZdU.jpeg) 
![IMG_1605|652x500](upload://sFkAmzK5w1rlUoteg3WWNEE2aGA.jpeg)

It kinda works, but the ADC pins on ATTINY84 are only 10bit and they are not very accurate, so especially the voltage reading on the last cell is +-0.1V, which is pretty bad.

There's not really a stacking error. You measure the voltage on the last cell by measuring the 11S voltage and the 12S voltage and substract the values. The problem is that the resolution decreases with each cell. You get a usable resolution on the first cell, but the resolution on the last cell is 12 times worse (on 12S battery) and that's unusable if measured with 10bit ADC. However, with a 16bit ADC, you would still get a pretty good resolution even on the last cell.

The variability in the resistors is not a problem. You don't need exactly 1/2, 1/3, 1/4, etc dividers as long as you know the exact ratios of the dividers, which is a matter of simply measuring the exact resistance of the used resistors. You then adjust the measured voltage correctly in software.

[quote="deucesdown, post:67, topic:76695"]
ASD1115, looks like it has 4 16bit ADC, but that’s in single ended mode (common ground).
[/quote]

Sure, that's why you need the voltage divider. You don't measure individual cells. Rather, you measure the first cell, first two, first three, etc. [Like this](https://www.falstad.com/circuit/circuitjs.html?cct=$+1+0.000005+10.20027730826997+50+5+43%0Av+64+80+96+80+0+0+40+4.2+0+0+0.5%0Av+112+80+144+80+0+0+40+4.2+0+0+0.5%0Av+160+80+192+80+0+0+40+4.2+0+0+0.5%0Av+208+80+240+80+0+0+40+4.2+0+0+0.5%0Av+256+80+288+80+0+0+40+4.2+0+0+0.5%0Av+304+80+336+80+0+0+40+4.2+0+0+0.5%0Av+352+80+384+80+0+0+40+4.2+0+0+0.5%0Av+400+80+432+80+0+0+40+4.2+0+0+0.5%0Av+448+80+480+80+0+0+40+4.2+0+0+0.5%0Av+496+80+528+80+0+0+40+4.2+0+0+0.5%0Av+544+80+576+80+0+0+40+4.2+0+0+0.5%0Av+592+80+624+80+0+0+40+4.2+0+0+0.5%0Aw+160+80+160+112+0%0Aw+208+80+208+112+0%0Ar+160+112+160+160+0+20000%0Ar+160+160+160+208+0+2200%0Aw+160+160+144+160+0%0Aw+144+160+144+272+0%0Aw+64+80+64+208+0%0Aw+112+208+160+208+0%0Aw+160+208+208+208+0%0Ar+208+160+208+208+0+2200%0Aw+96+80+112+80+0%0Aw+144+80+160+80+0%0Aw+192+80+208+80+0%0Aw+240+80+256+80+0%0Aw+288+80+304+80+0%0Aw+336+80+352+80+0%0Aw+384+80+400+80+0%0Aw+432+80+448+80+0%0Aw+480+80+496+80+0%0Aw+528+80+544+80+0%0Aw+576+80+592+80+0%0Aw+208+160+192+160+0%0Aw+192+160+192+272+0%0Aw+240+160+240+272+0%0Aw+256+160+240+160+0%0Ar+208+112+208+160+0+30000%0Ar+256+160+256+208+0+2200%0Aw+208+208+256+208+0%0Aw+256+80+256+112+0%0Aw+288+160+288+272+0%0Aw+304+160+288+160+0%0Ar+256+112+256+160+0+43000%0Aw+256+208+304+208+0%0Aw+304+80+304+112+0%0Aw+336+160+336+272+0%0Aw+352+160+336+160+0%0Ar+304+112+304+160+0+47000%0Aw+304+208+352+208+0%0Aw+352+80+352+112+0%0Aw+384+160+384+272+0%0Aw+400+160+384+160+0%0Ar+352+112+352+160+0+51000%0Aw+352+208+400+208+0%0Aw+400+80+400+112+0%0Aw+432+160+432+272+0%0Aw+448+160+432+160+0%0Ar+400+112+400+160+0+62000%0Aw+400+208+448+208+0%0Aw+448+80+448+112+0%0Aw+480+160+480+272+0%0Aw+496+160+480+160+0%0Ar+448+112+448+160+0+75000%0Aw+448+208+496+208+0%0Aw+496+80+496+112+0%0Aw+528+160+528+272+0%0Aw+544+160+528+160+0%0Ar+496+112+496+160+0+82000%0Aw+496+208+544+208+0%0Aw+544+80+544+112+0%0Aw+576+160+576+272+0%0Aw+592+160+576+160+0%0Ar+544+112+544+160+0+91000%0Aw+544+208+592+208+0%0Aw+592+80+592+112+0%0Aw+624+160+624+272+0%0Aw+640+160+624+160+0%0Ar+592+112+592+160+0+100000%0Aw+592+208+640+208+0%0Aw+640+80+640+112+0%0Aw+624+80+640+80+0%0Ar+112+160+112+208+0+2200%0Aw+112+208+64+208+0%0Aw+112+160+96+160+0%0Aw+96+160+96+272+0%0Ar+112+112+112+160+0+10000%0Aw+112+80+112+112+0%0Ar+304+160+304+208+0+2200%0Ar+352+160+352+208+0+2000%0Ar+400+160+400+208+0+2000%0Ar+448+160+448+208+0+2000%0Ar+496+160+496+208+0+2000%0Ar+544+160+544+208+0+2000%0Ar+592+160+592+208+0+2000%0Ar+640+160+640+208+0+2000%0Ar+640+112+640+160+0+110000%0A).

The main problem I see with the voltage divider is that the cells get constantly discharged over the resistors. Even worse, the discharge is uneven. The first cell gets discharged most while the last gets discharged least. Even though the current flow can be kept low by using high enough resistors, this would get the cells out of balance eventually, especially should the measuring module be connected to the battery all the time. There's no easy way to turn it off.

[quote="deucesdown, post:67, topic:76695"]
I think a BMS chip (maybe from TI, maybe same family as smartbms or diebms?) will have all the voltmeters in one easy to use package, and probably cost less than rigging a bunch of ADC and voltage dividers?
[/quote]

I don't think it would cost less. Three ASD1115 would be around $5 and resistors cost almost nothing. I agree that a BMS chip would be a more elegant and generally better solution though. It just seems terribly complicated. I read through the [datasheet of the TI bq76940](http://www.ti.com/lit/ds/slusbk2g/slusbk2g.pdf) that the LLT Smart BMS uses and there were too many things I didn't understand at all. Plus, it doesn't seem you can use the chip alone. The datasheet contains a schematics of circuits to be used with the BMS chip and there's a bunch of other components. You can probably exclude many if you only want to measure the cell voltage. Still, it didn't seem at all easy to figure out, at least for a hobbyist like myself. A voltage divider, on the other hand, is simple and straightforward.
```

---
## \#69 Posted by: Giga Posted at: 2019-01-06T20:01:53.594Z Reads: 55

```
Very nice!

I have a similar BMS and don't understand the power routing. 
So I know left side is B- and right side is C-/P-. In the App I can activate and deactivate charging and discharging which both works like set in the app (when I power down the discharge mosfet, the ESC doesnt work anymore, when I power down the charge mosfet the charger doenst charge anymore, when I power down the discharge and charge is still on: I can still charge but not discharge, never tried discharge:on charge:off and charge then). 

So now I am thinking about how this works, I got a clue but that makes no sense: since the B- is on the left side, does that mean the current is flowing from B- through the little shunts/fueses to and through the first row of mosfets to the middle and then through second row of mosfets to right?

And how does charging from the C-/P- work if the discharge fet is powered off? 

Since you have your BMS opened, did you check for this? Mine is currently in use in a batterypack 150km away from me... :confused:
```

---
## \#70 Posted by: janpom Posted at: 2019-01-06T20:47:04.207Z Reads: 55

```
I believe that if the charge MOSFET is enabled, it connects the B- and C-. If the discharge MOSFET is enabled, it connects the B- and P-. That is, the MOSFETs simply close the charge/discharge circuits.
```

---
## \#71 Posted by: Giga Posted at: 2019-01-06T21:36:30.984Z Reads: 58

```
But my BMS has C- and P- on same connector. I charge through discharge wires/pad...
also this would mean the battery pad is the middle one and there are same number of discharge mosfets as charge mosfets...
```

---
## \#72 Posted by: janpom Posted at: 2019-01-07T06:01:00.071Z Reads: 57

```
From how you describe the BMS behaves, I don't believe the C- and P- are actually the same pad. I would check continuity between them with a multimeter.
```

---
## \#73 Posted by: janpom Posted at: 2019-01-07T12:11:41.093Z Reads: 56

```
[quote="Giga, post:71, topic:76695"]
I charge through discharge wires
[/quote]

Oh, I missed this bit. Then that must really be one pad. I don't know how that works then, sorry.
```

---
## \#74 Posted by: Giga Posted at: 2019-01-07T12:37:39.858Z Reads: 54

```
Are you able to follow the path of the main current via the multimeter in your testsetup? Mine is currently not open...
```

---
## \#75 Posted by: janpom Posted at: 2019-01-07T16:42:03.784Z Reads: 55

```
Not sure what you mean. After more thinking about your BMS though, I believe it could allow the current to only pass in one direction. When discharge is disabled, only current from P/C- to B- is allowed and vice versa for charge being disabled. I believe that could be achieved with two MOSFETs and two diodes. That's just an uneducated guess though. I don't really know much about BMSes.
```

---
## \#76 Posted by: Hummie Posted at: 2019-01-07T17:01:58.657Z Reads: 55

```
Could you use diodes or mosfets with the 12 separate lipo chargers and the earlier mentioned charging/balancing scheme using one power supply and not short? Still trying
```

---
## \#77 Posted by: deucesdown Posted at: 2019-01-07T19:31:03.974Z Reads: 55

```
The short happens because all the negatives of each charger, on both the supply and output end, are electrically wired together (common ground). So if you hook all the chargers up, shorts everywhere.

I believe the only reasonable way to isolate power circuits is transformers. So if you put a transformer between the single power supply and the 1s chargers, as long as nothing else is completing the circuit to ground, you have floating power supplies, which is safe. It can even be a 1-to-1 transformer (5 volts in, 5 volts out).

And transformers work via alternating current (doh), so practically, 120vac -> splitter -> transformer -> 5vac -> 5vdc -> 1s charger seems the simplest to do. dc-dc I guess is possible but you have to convert to ac and back somewhere.

I hope I'm not completely wrong again lol.
```

---
## \#78 Posted by: Hummie Posted at: 2019-01-07T19:44:32.920Z Reads: 59

```
Could maybe do a single to multiple transformer at least.  Simplify a bit.
```

---
## \#79 Posted by: Giga Posted at: 2019-01-09T15:14:47.680Z Reads: 53

```
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/8892
Please tell me you made this work with the Serialoutput of the ChinaBMS :pray:
```

---
## \#80 Posted by: janpom Posted at: 2019-01-09T15:17:54.626Z Reads: 53

```
Depends on what you mean by "ChinaBMS". If the LLT Power Smart BMS then yes.
```

---
## \#81 Posted by: Giga Posted at: 2019-01-09T15:22:46.498Z Reads: 53

```
All china bms working with xiaoxiang app (yellow elephant)
I guess there are only 2 different smart bms on the market, the one with yellow elephant app and the one with big SPI screen and the app is called vmax or something...
```

---
## \#82 Posted by: janpom Posted at: 2019-01-09T15:24:01.928Z Reads: 50

```
That's the one then. I mean one that works with the xiaoxiang app.
```

---
## \#83 Posted by: Giga Posted at: 2019-01-09T15:25:52.101Z Reads: 50

```
Any chance you are posting the code? 
Which display driver you you have? ili9341?
Did you figure out the bms lock/unlock function?
Would like to attach a display + button....
```

---
## \#84 Posted by: janpom Posted at: 2019-01-09T15:30:33.329Z Reads: 49

```
Yes, I'll make the code available, but I want to do some polishing first. Probably some time next week. It uses this display driver: https://github.com/Nkawu/TFT_22_ILI9225

Currently I can only read data from the BMS. I can't control it or change settings. That part of the protocol is not documented so I would have to reverse engineer it.
```

---
## \#85 Posted by: Giga Posted at: 2019-01-09T15:44:18.915Z Reads: 51

```
[quote="janpom, post:84, topic:76695"]
Yes, I’ll make the code available, but I want to do some polishing first. Probably some time next week.
[/quote]

:heart: thanks!

[quote="janpom, post:84, topic:76695"]
It uses this display driver: [https://github.com/Nkawu/TFT_22_ILI9225 ](https://github.com/Nkawu/TFT_22_ILI9225)
[/quote]

Damn, that is the version/driver for 176x220 TFT screens...I got (and used so far) Ili9341 based displays since they got 240x320px and are available from 2.2" to 2.4" till 2.8".

[quote="janpom, post:84, topic:76695"]
Currently I can only read data from the BMS. I can’t control it or change settings.
[/quote]
Still one step ahead of me^^ 

[quote="janpom, post:84, topic:76695"]
That part of the protocol is not documented so I would have to reverse engineer it.
[/quote]
There is a documentation? Some time ago I found a threat on ES forum where someone logged the protocol, but I couldn't find it right now.

This guy already managed it https://github.com/smagicld/xiaoxiangBMS#Xiaoxiang-BMS
But no dokumentation or real sourcecode...
```

---
## \#86 Posted by: janpom Posted at: 2019-01-09T15:50:12.587Z Reads: 47

```
You can download a zipped Excel file from this page: https://www.lithiumbatterypcb.com/smart-bms-software-download/

[quote="Giga, post:85, topic:76695"]
his guy already managed it https://github.com/smagicld/xiaoxiangBMS#Xiaoxiang-BMS
[/quote]

Yeah, I know. We can try getting in touch with him and ask about the secret formula for writing into the BMS. :smile:
```

---
