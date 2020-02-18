# Best 18650 battery charging options

### Replies: 24 Views: 1627

## \#1 Posted by: webst Posted at: 2018-03-21T12:01:29.409Z Reads: 240

```
Nobody told me making my own eboard will be easy but this battery thing is pretty complicated. I've read Micah Toll book about batteries, most of your posts here and I came to conclusion that I'd like to make 10s4p on samsung 30Q (big thanks to @Vanarian). I am also a little confused on best charging option I should choose. 

1. Small footprint internal BMS that I bypass while riding knowing that I have limits set directly in vesc. It would be used only for charging. 
https://www.aliexpress.com/item/10S-15A-BMS-for-36V-li-ion-battery/1195130789.html
**Pros:** small, cheap
**Cons:** cannot set lower voltage like 4.1V as upper charging limit, need of additional on/off switch

2. 10S 80A Bestech with eswitch
**Pros:** once set works, no need for additional on/off switch, 
**Cons:** large, expensive, cannot change parameters afterwards unless you double the price, need to charge while power is on

3. 10S 80A RJXZS
https://www.aliexpress.com/item/10S-80A-active-bms-2017-new-Li-ion-smart-bms-pcm-with-android-Bluetooth-app-UART/32839468266.html
**Pros:** Bestech price, adjustable parameters
**Cons:** as large as Bestech, lesser known brand, no built in on/off switch

4. Option 2 (without eswitch) or 3 externalized for occasional use
https://www.electric-skateboard.builders/t/li-ion-battery-pack-without-bms/47818/40?u=webst
Under link above @SkaterBoy58 used RJXZS to make external charging station
**Pros:** less electronics onboard, no problem with not working brakes while downhill on charged board, can use one power brick for direct and balanced charge
**Cons:** need of additional on/off switch, large connector, for safety need to direct use of this kind of charger http://www.groetech.de/index.php?main_page=product_info&products_id=837

People mostly tend to choose option number 2 but I'd like something smaller with adjustable parameters. External option is tempting mainly due to space restrictions but then I'd need to use two eswitches which raises the costs, takes enclosure space and fails sometimes. Aren't there any all-in-one solution, small, with eswitch and high discharge at the same time?
```

---
## \#2 Posted by: Vanarian Posted at: 2018-03-21T14:26:43.206Z Reads: 203

```
You're welcome, glad I was able to help. 

There are safest choices (just like the number 2#) but it comes to what you do prefer / which compromise you may make.

There is FlexiBMS and Battman options too which might be interesting to give a go too. 

As an example (not the best) on my build I don't have enough room (or barely maybe) for a decent on-board BMS. So one solution is to get a on-charger external BMS, with JST extra ports to link your cells to the BMS unit.

It is flawed because you don't have any BMS features while riding and your ESC better be well set in order not to damage anything. But it is the lightest setup and no limits whatsoever on discharges. That's the bare minimum I'd say. 

If you can spare some room for a quality  BMS with built-in switch just go for it, you won't regret!
```

---
## \#3 Posted by: webst Posted at: 2018-03-21T15:21:26.622Z Reads: 181

```
On the other hand overcharge protection on built in BMS might cut your brakes on long downhill run. I think I'd feel better with prospect of broken battery rather than leg. What kind of switch and charger do you use? Is 42V charger like [this](https://www.aliexpress.com/item/13S-48V-4-5A-5A-5-5A-6A-6-5A-7A-7-5A-8A-Lithium-Li/32803016273.html) connected to external Bestech BMS allright?
```

---
## \#4 Posted by: webst Posted at: 2018-03-22T01:50:08.923Z Reads: 166

```
Anyone can help?
```

---
## \#5 Posted by: E1Allen Posted at: 2018-03-22T02:40:42.362Z Reads: 155

```
You forgot to mention hobby chargers.  If you setup your battery in 5s or 6s then series two together you can use any hobby charger.  Plus every time you charge you can check to see if any are straying.  Check IR as well.  I have my 12s6p setup as 3s6p.  I have a dual charger 20a each channel.  Doesn't take long to charge.
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-03-22T03:13:13.906Z Reads: 153

```
[quote="webst, post:1, topic:49719"]
cannot set lower voltage like 4.1V
[/quote]

item 1, that's not true. when I order bms from bestech the upper cutoff is modified for 4.15v, and you can customize it further so one could request a 4.1v or even lower cutoff.
```

---
## \#7 Posted by: webst Posted at: 2018-03-22T03:21:18.907Z Reads: 147

```
I was refering to small no name bms there. Bestech is one point lower on the list.
```

---
## \#8 Posted by: MicahT Posted at: 2018-03-22T07:25:42.234Z Reads: 140

```
Glad to hear you found my book helpful!

Might be a stupid question, but do you absolutely require an on/off switch on the BMS? I just leave my battery connected to my dual ESC and use the ESC's on/off switch. If there is any drain when the controller is off, its too low to measure on my meter. I've never gone more than a week without riding, but if I did, I'd simply unplug the battery, like if I was traveling or something.
```

---
## \#9 Posted by: webst Posted at: 2018-03-22T07:54:44.954Z Reads: 135

```
Lots of great info for someone who charged nimh AA batteries for most of his life :slight_smile: 

I’m really glad you showed up because after reading your book I had this idea I’ve never shared here in BMS church HQ, afraid of lynching, that is an extension of your idea from comment above, that is lack of power button. I wanted to use XT90 connectors in place of serial connections, that way I could change battery topology from 10s4p to 10x4p and parallel charge it with 40A 4.1-4.15V power supply while autobalancing at the same time. It looks quite inconvenient in a way (11 XT90 to reconnect when you consider not using power switch) in it’s basic form, but incorporating mosfets in later time would automate the switching process. Is this idea viable from your point of view? Is it really new idea or long-forgotten one?
```

---
## \#10 Posted by: MicahT Posted at: 2018-03-22T08:13:37.672Z Reads: 129

```
Viable? Definitely.
Practical? Depends on you. 

Like you said, you're playing around with a dozen or so connectors every time you charge. At least with XT90s you don't have to worry about reverse polarity, so that removes one common danger with this approach, but its still a fairly cumbersome method to charge. If you don't mind doing all the reconnections then it can work. But that's also a lot of bulk from wire and connectors, which could practically double the volume of your pack. On the other hand, it will automatically balance by being a single 1s40p pack during charging, so that's an advantage.

I'm still a fan of a BMS, and I actually don't agree with the many people that bypass a BMS during discharge, since it removes the individual cell LVC protection of the BMS. Yea, you can set a LVC in your VESC, but if you have one cell group drop down too low first, the VESC won't know about it like the BMS would.

But now I'm rambling. Anyways, your method theoretically can work just fine. The question is how annoying will it become over time to do it manually?
```

---
## \#11 Posted by: E1Allen Posted at: 2018-03-22T08:24:46.526Z Reads: 121

```
[quote="MicahT, post:10, topic:49719"]
since it removes the individual cell LVC protection of the BMS.
[/quote]

So does this cut voltage to the whole pack? If so I'd rather burn up an entire battery than Street face.
```

---
## \#12 Posted by: MicahT Posted at: 2018-03-22T08:28:30.301Z Reads: 120

```
Haha yea, most BMSs will cut output if a cell group drops dangerously low. 

The behavior on your board will then depend on your controller. Mine just freewheels when power is lost, doesn't lock the wheels.
```

---
## \#13 Posted by: E1Allen Posted at: 2018-03-22T08:40:00.575Z Reads: 113

```
[quote="MicahT, post:12, topic:49719"]
Mine just freewheels when power is lost, doesn’t lock the wheels.
[/quote]
Sounds great for cruising, not so great during high amp draw while accelerating.
```

---
## \#14 Posted by: webst Posted at: 2018-03-22T09:08:20.655Z Reads: 106

```
Even worse when decelerating while going high speed downhill and over voltage control kicks in. This is something I fear the most. Only solution seems to be going downhill with battery half empty.
```

---
## \#15 Posted by: Vanarian Posted at: 2018-03-22T09:54:46.201Z Reads: 105

```
The XT90 modular solution is similar to what I do but I use smaller XT60 (I run 4x 8S1P for charging, bundled together in P groups for riding) ; you simply need to get some "quick swap type" to make it easy on daily basis.

So Yea it works. About the HVC you fear, you need to make a DIY dump module so any excessive voltage / current get burned through it and you never trigger the HVC or burn batteries during your ride. 

Have seen it made by a Danish youtuber on his mono wheel, works like a charm but I don't understand the schematics. He replaced shunts by halogen and LED bulbs for fun, which means it doesn't have to be a bulb. Anyway this thing needs a separate heatsink too. 

Maybe somebody here could help doing this if I post the video and schematic?

Edit : BTW I think this guy runs 64v battery if I remember well.
```

---
## \#16 Posted by: webst Posted at: 2018-03-22T10:37:41.324Z Reads: 99

```
[quote="Vanarian, post:15, topic:49719"]
DIY dump module
[/quote]
This sounds like really good temporary solution, post links please. Ideally I imagine that some VESC 7.0 would do that by dumping excessive energy above set voltage treshold into secondary circuit containing power resistors and loud acoustic signal to let you know that you have certain amount of time to stop. I don't know how much time you'll get from small resistor like below but I guess few of them connected to radiator will suffice to dump 1kW(?) of breaking power for few seconds. 

![_SX342_|342x342](upload://viLcc5PpW6V59xUmY9o3wPYy3e6.jpg)

Edit: regular bulbs would be useless after first bump in the road and led ones draw too small current
Edit 2: Now it occured to me that transistors are voltage controlled switches (discovery of the year) which makes this not more complicated than antispark switch.
```

---
## \#17 Posted by: Vanarian Posted at: 2018-03-22T11:44:10.902Z Reads: 98

```
Well the original maker might give you more accurate infos than me, I randomly discovered he has a full thread (only knew his YT videos) here : 

http://forum.electricunicycle.org/topic/6508-brake-chopper-to-avoid-over-voltage-condition/

Might as well open a separate topic here so people can give it a try :wink:

Edit : you'll see that he doesn't ride on perfect road (more like forest track) and it holds good !
```

---
## \#18 Posted by: ihatetopush Posted at: 2018-03-24T05:30:30.134Z Reads: 89

```
1) Battery charger   900W DC-DC Boost Converter 8-60V to 10-120V 15A Step Up Power Supply Module

https://www.youtube.com/watch?v=0Z5QWzSSvdI

https://www.youtube.com/watch?v=4HAQhN6_cnM&t=3s
```

---
## \#19 Posted by: ihatetopush Posted at: 2018-03-27T23:02:27.193Z Reads: 81

```
i use a 12volt pc power sup  charges my battery in 30 mins 36volt 20 cell
```

---
## \#20 Posted by: webst Posted at: 2018-03-28T06:35:41.788Z Reads: 74

```
By reconnecting them parallel?
```

---
## \#21 Posted by: ihatetopush Posted at: 2018-03-29T10:43:14.500Z Reads: 66

```
https://www.youtube.com/watch?time_continue=7&v=0Z5QWzSSvdI in the video this guy charges his ebike with a server power supply and Battery charger 900W DC-DC Boost Converter.  you set the charger to 41 or 42 volts my pack is 36volt 20 cell total 10 cells in series and 10 cell in series both of the sets of 10 in parallel the max charge per cell is 4.2 volt    x 10 cell 42 volt   if you wanted to charge 1 cell set charger to 4.2 volts    4 cells to 16.8 the key is you need a charger that cuts of the voltage at your max battery pack voltage mine is 42 so you dont have a early 4 of july in this side your home.  Jehu Garcia video help me out https://www.youtube.com/watch?v=ZBf_qXEYUoM Check out his electric Samba bus. His boy sell batteries on ebay he is the real deal http://stores.ebay.com/tomhasgooddeals i bought 5 sets 36v 18650 20 cell battery pacts for $125 with bms and t60 samsung all new love them! ![16 AM|300x228](upload://hxtnG0w0Rn5zHwgD4iAbpbY1VTy.png)
```

---
## \#22 Posted by: ihatetopush Posted at: 2018-03-29T10:45:59.801Z Reads: 64

```
hope this helps
```

---
## \#23 Posted by: webst Posted at: 2018-03-29T11:29:35.044Z Reads: 63

```
This buck converter idea seems interesting. I’ll have to make sure that there are safety mechanisms in case of bms failure.
```

---
## \#24 Posted by: ihatetopush Posted at: 2018-03-30T00:07:31.458Z Reads: 52

```
you set the max voltage and it will cut off for you.  Dont trust BMS. I love the buck it does not come with a case  and  you can use and old pc power supply  or better would be old serve supply used what you have on hand bro. I can charge  my battery in 30 mins. The buck cost me less than $30
```

---
