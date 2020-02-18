# Thinking of building my first Eboard, how does this look

### Replies: 48 Views: 2146

## \#1 Posted by: MrMidJiT Posted at: 2018-01-15T20:51:19.290Z Reads: 214

```
<table><tr><td><b>Parts for electric skateboard</b></td><td><b></b></td><td><b>Price</b></td><td><b></b></td><td><b>Link</b></td></tr>
<tr><td><b></b></td><td></td><td></td><td></td><td></td></tr>
<tr><td><b>Motor</b></td><td></td><td>£68.55</td><td></td><td>products/electric-skateboard-motor-6355-190kv</td></tr>
<tr><td><b>ESC</b></td><td></td><td>£76.16</td><td></td><td>products/torque-esc-vesc-bldc-electronic-speed-controller</td></tr>
<tr><td><b>ESC enclosure</b></td><td></td><td>£26.65</td><td></td><td>products/esc-enclosure</td></tr>
<tr><td><b>ESC USB port</b></td><td></td><td>£11.81</td><td></td><td>products/vesc-usb-programmer-stlinkv2</td></tr>
<tr><td><b>Controller/Remote</b></td><td></td><td>£45.70</td><td></td><td>products/torqueboards-2-4ghz-nano-remote-controller</td></tr>
<tr><td><b>Mechanical kit</b></td><td></td><td>£152.33</td><td></td><td>collections/featured-items/products/single-motor-mechanical-kit</td></tr>
<tr><td><b>Deck</b></td><td></td><td>tbc</td><td></td><td>tbc</td></tr>
<tr><td><b>Battery</b></td><td></td><td>£37.14</td><td></td><td>https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack-xt90.html</td></tr>
<tr><td><b>BMS</b></td><td></td><td>£9.52</td><td></td><td>https://hobbyking.com/en_us/6s-li-ion-10a-pcm.html</td></tr>
<tr><td><b>Charging port/power button</b></td><td></td><td>£4.94</td><td></td><td>https://www.amazon.co.uk/Wingsmoto-Charging-Repalcement-Self-balancing-Hoverboard/dp/B074TC551D/ref=sr_1_1?s=sports&ie=UTF8&qid=1516046379&sr=1-1&keywords=hoverboard+charging+port</td></tr>
<tr><td><b>Charger</b></td><td></td><td>£10.95</td><td></td><td>https://www.amazon.co.uk/Electric-Universal-Swagtron-Hoverboard-Connector/dp/B06XP5PJHR/ref=sr_1_4?s=sports&ie=UTF8&qid=1516046379&sr=1-4&keywords=hoverboard+charging+port</td></tr>
<tr><td><b>Battery enclosure</b></td><td></td><td>£26.65</td><td></td><td>collections/battery-enclosures/products/2x3s-rc-lipo-battery-enclosure</td></tr>
<tr><td><b>Battery bag</b></td><td></td><td>£2.13</td><td></td><td>https://hobbyking.com/en_us/fire-retardant-lipo-battery-bag-190x60x82mm.html</td></tr></table>

As the title says, this would be my first build. Me and a friend, who has built a board, have quickly put together a list of the parts I plan on using. The main focuses of this board would be:
* Decent range
* Decent speed
* An easily upgradeable platform for the future

Again, this is my first board so I'm probably making some mistakes as even my friend who helped me barely got his working. All I ask is that you help me. Thanks in advance. 

Also I really hope the html table worked
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-01-15T21:12:35.562Z Reads: 193

```
How many of these 3s 8000mah batteries are you planning to buy? 1 won't be enough
```

---
## \#3 Posted by: Martinsp Posted at: 2018-01-15T21:15:33.893Z Reads: 192

```
Isnt it more econimical for you to order from www.alienpowersystem.com? They are based in UK and have similar motors to DIY in my opinion and a good reputation. They also have a lot of other esk8 stuff you might want to check them out if you have not already. Because if your package gets stopped by customs you will have to pay a lot, VAT+import fees.
```

---
## \#4 Posted by: Grolletje Posted at: 2018-01-15T21:18:58.929Z Reads: 177

```
I think that you won't need the st-link programmer. the VESC will probably have a bootloader on it already.

If the Vesc has a bootloader then you can just connect the VESC to your pc via mini usb.
```

---
## \#5 Posted by: Grolletje Posted at: 2018-01-15T21:24:21.661Z Reads: 167

```
It depents a bit on the amount of batteries you are going to put in series, but if you have 2 in series (22,2 V nominal) you would have a kind of low top speed with your 190 KV (rpm/v) motor. 22,2*190= 4200 rpm. 

http://calc.esk8.it/ is a very useful site to see what your board will be capable of!
```

---
## \#6 Posted by: MrMidJiT Posted at: 2018-01-15T21:56:56.828Z Reads: 153

```
Didn’t realise that a 3s would be so bad for speed, I’d probably be better going for a 6 cell 18650 li ion then. Is there anyone on here that is UK based that could provide?
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-01-15T22:04:06.122Z Reads: 143

```
@darkkevind might do it
```

---
## \#8 Posted by: FredrikHems Posted at: 2018-01-15T22:04:53.150Z Reads: 139

```
Just buy 2 and connect them in series- and voila, a 6S battery :slight_smile: However it would be better for the Vesc to buy 3 to make it a 9s.
```

---
## \#9 Posted by: atenner Posted at: 2018-01-15T22:07:38.057Z Reads: 139

```
Also 

Www.street-wing.com 

@DavidBanner 

Where abouts in the UK are you ?
```

---
## \#10 Posted by: DavidBanner Posted at: 2018-01-15T22:09:40.768Z Reads: 139

```
I am based in London
```

---
## \#11 Posted by: mmaner Posted at: 2018-01-15T22:10:47.227Z Reads: 137

```
To be clear, higher voltage is more efficient...nit necessarily better for a vesc as there is less voltage delivery. Regardless if the "studies" I've been running a vesc in 6s for iber a year and it's stood up at lease as well as my 10s boards. Though the lack of speed sucks ☺️.
```

---
## \#12 Posted by: DavidBanner Posted at: 2018-01-15T22:11:53.770Z Reads: 127

```
[quote="MrMidJiT, post:6, topic:43807"]
I’d probably be better going for a 6 cell 18650 li ion then. Is there anyone on here that is UK based that could provide?
[/quote]

I make custom packs.

Do you have any idea of the configuration of the pack you want? 10S4P is a popular choice, or maybe 8S?
```

---
## \#13 Posted by: atenner Posted at: 2018-01-15T22:12:32.569Z Reads: 125

```
I think I need to do some PR work, we need more esk8’s in the Midlands 😡
```

---
## \#14 Posted by: DavidBanner Posted at: 2018-01-15T22:14:38.290Z Reads: 122

```
[quote="atenner, post:13, topic:43807"]
we need more esk8’s in the Midlands
[/quote]

I can usually get packages in people's hands anywhere in the UK within 2-3 days or ordering. Even the midlands :slight_smile:
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-01-15T22:17:28.055Z Reads: 115

```
IMO its better for the Vesc to run 9s compared to 6s.. At 33v you Aren't really pushing the voltage "limit". As the standard Vesc's only can take 27? Amps (Which is little) countinous. And with 6s you will (in theory) pull 50% more current,- compared to 9s.
```

---
## \#16 Posted by: darkkevind Posted at: 2018-01-15T22:39:14.078Z Reads: 110

```
Yeah I could do you a nice 18650 pack :+1:
```

---
## \#17 Posted by: westonbe Posted at: 2018-01-16T01:00:19.750Z Reads: 105

```
Yea looks good except for the battery situation. Make sure to do your research with the BLDC online.
These videos will help when you come to that situation:
https://www.youtube.com/watch?v=5HLZaMcYRuY
https://www.youtube.com/watch?v=XfC4QOcDcvE
```

---
## \#18 Posted by: MrMidJiT Posted at: 2018-01-16T10:28:41.319Z Reads: 94

```
TBH whatever is cheapest and wont be terrible on speed. I’m still just a student with limited funds trying to make my commute less terrible
```

---
## \#19 Posted by: DavidBanner Posted at: 2018-01-16T10:49:14.285Z Reads: 86

```
Lipos are probably going to be the cheapest option, but won't have the same sort of lifespan an 18650 would do.
```

---
## \#20 Posted by: MrMidJiT Posted at: 2018-01-16T11:03:33.893Z Reads: 86

```
I’m willing to splurge a little bit if it means they’ll last longer. I’m also a little paranoid about lipos catching fire / blowing up
```

---
## \#21 Posted by: DavidBanner Posted at: 2018-01-16T11:21:19.941Z Reads: 79

```
it's the never ending conundrum, save money now and pay more later, or take the pain up front and save some cash down the line. It's always hard to make that call :slight_smile:

Another factor just to add to your confusion - most 18650 packs are not going to be allowed on a plane, but lipo packs can be pulled out of the board and taken hand luggage.
```

---
## \#22 Posted by: MrMidJiT Posted at: 2018-01-16T12:06:34.408Z Reads: 80

```
I’m fine with it not being allowed on a plane, don’t travel too often. I’m 99% sure I want 18650s as long as they’re <= £50
```

---
## \#23 Posted by: DavidBanner Posted at: 2018-01-16T12:09:46.571Z Reads: 80

```
a pack is going to be a lot more than £50. A BMS and charger alone will run you close to that figure...
```

---
## \#24 Posted by: GrecoMan Posted at: 2018-01-16T12:21:21.475Z Reads: 70

```
most people charge about $400-600 for a 10s4p pack. use that as a reference
```

---
## \#25 Posted by: MrMidJiT Posted at: 2018-01-16T12:21:54.592Z Reads: 69

```
Even if I’m only getting a 6 cell pack? I know the BMS/Charger will run me about that but I’m leaving them out the price. I can find 6 18650s online for less than £40
```

---
## \#26 Posted by: DavidBanner Posted at: 2018-01-16T12:36:51.241Z Reads: 70

```
6S1P is not going to do you much good
```

---
## \#27 Posted by: riva_00 Posted at: 2018-01-16T13:30:15.997Z Reads: 72

```
@DavidBanner So can you make custom packs? I'm in the UK and considering a spot welder but would prefer someone to make them instead.

MrMidJit, i'd recommend a 18650 battery pack over LiPo, it's technically safer and can be built to spec. Unless you want the absolute maximum capacity for the space, or superior discharge capability.....or ease of purchase and implementation.

Also check here for a FOCBOX instead of a Vesc, i don't yet have one but according to posts here it's better. And these are already in the UK, so no customs

http://www.electric-skateboard.builders/t/focbox-110-nano-x-40-uk-europe-eu-buy-new-price-reduced-16-16-3-3-available-next-day-uk-delivery-d/43705
```

---
## \#28 Posted by: TheLastEnting Posted at: 2018-01-16T13:33:32.731Z Reads: 68

```
[quote="atenner, post:13, topic:43807"]
we need more esk8’s in the Midlands
[/quote]

True that man, I think I've only ever seen one other eSk8 around here, and the guy wasn't hanging around to strike up a conversation.

What part of the Midlands are you from?
```

---
## \#29 Posted by: riva_00 Posted at: 2018-01-16T13:40:34.234Z Reads: 66

```
@TheLastEnting @atenner
I'm also in midlands (Nottinghamshire), but my legs healing after a bad fall shaved the skin off my knee and scratched a tendon, hoping to be boarding again by march.
```

---
## \#30 Posted by: MrMidJiT Posted at: 2018-01-16T13:46:31.734Z Reads: 65

```
Would it work until I have the funds to upgrade? As long as it works and can be upgraded to a 6s2p or 6s4p in the future I’m fine with that for now
```

---
## \#31 Posted by: TheLastEnting Posted at: 2018-01-16T13:49:16.332Z Reads: 66

```
Sorry to hear that man, hope you make a full recovery and everything. As long as your boarding again by the time the weather brightens up though.
```

---
## \#32 Posted by: DavidBanner Posted at: 2018-01-16T13:54:56.695Z Reads: 69

```
[quote="MrMidJiT, post:30, topic:43807"]
Would it work until I have the funds to upgrade?
[/quote]

it would work, but it's probably not worth recycling the cells from the first pack, too much work.
```

---
## \#33 Posted by: DavidBanner Posted at: 2018-01-16T13:55:26.663Z Reads: 64

```
[quote="riva_00, post:27, topic:43807"]
So can you make custom packs? I’m in the UK and considering a spot welder but would prefer someone to make them instead.
[/quote]

@riva_00 I sure do.

What spec do you have in mind?
```

---
## \#34 Posted by: SimosMCmuffin Posted at: 2018-01-16T14:05:09.323Z Reads: 61

```
Just going to point out that the linked BMS is only for 6S packs and is only 10 A discharge max, which IMO is nowhere near enough. You're either going to cook your BMS or it's going to constantly keep cutting-off, because you're going over the current limit.

I would have also pointed out that the single 3S Zippy battery is not not compatible with the BMS in question, but seems you have other inquiries in that area already.
```

---
## \#35 Posted by: riva_00 Posted at: 2018-01-16T14:07:31.022Z Reads: 63

```
@DavidBanner awesome, I'm looking for a 10s6p or 4p, however I'm looking at 3d printing 2~3 individual battery boxes, and having everything kind of modular.
I don't want to hijack this thread though, so I'll PM you regarding this.
```

---
## \#36 Posted by: GrecoMan Posted at: 2018-01-16T14:07:33.836Z Reads: 65

```
you can bypass the bms for discharge.  I use a 10a bms with 60a max draw
```

---
## \#37 Posted by: SimosMCmuffin Posted at: 2018-01-16T14:09:41.441Z Reads: 64

```
Yes you can, but OP nowhere stated that he would bypass the BMS for discharge, and as OP is a newbie it might be plausible that he would try to use it for discharge
```

---
## \#38 Posted by: atenner Posted at: 2018-01-16T14:22:15.600Z Reads: 65

```
I’m living in Derby. From leicester originally. I guess we’ll see more people soon enough. Would be nice to get a local group ride on the go 👍🏻

@riva_00 shame to hear that. But good you’ll be back up and riding soon. I’ve (touch wood) not come off yet, and wont. 

Well, now up to 5 or 6 riders. That’ll totally count as a ‘group’ ride 😂

Also are you on the Facebook page ? ‘UK e-sk8t’
```

---
## \#39 Posted by: Kug3lis Posted at: 2018-01-16T14:30:31.449Z Reads: 64

```
With 1P and max current of 20A from cell he will catch it on fire faster than BMS will cut off
```

---
## \#40 Posted by: MrMidJiT Posted at: 2018-01-16T15:49:40.288Z Reads: 60

```
Yeah, haven’t mentioned it but I do plan on bypassing the bms for discharge. Been advised to elsewhere
```

---
## \#41 Posted by: riva_00 Posted at: 2018-01-16T16:57:13.152Z Reads: 60

```
@MrMidJiT, this is the inspiration you need for your board: -

http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/

He seems to do everything the right way, not cutting any corners. I don't expect you to go this far, but have a read of his battery setup and management.
```

---
## \#42 Posted by: MrMidJiT Posted at: 2018-01-16T20:52:27.689Z Reads: 55

```
Taken your guys suggestions for an updated parts list, Changed some of the parts to come from a UK supplier, made sure the stuff that is coming from a non-UK supplier can be delivered and decided to go for a 6s LiPo battery (for now) and upgrade to a Li-Ion in the future. I plan on bypassing the BMS for discharge. Is there anything else obvious that I am missing or something obvious i'm overlooking?
Updated table of parts
<table><tr><td><b>Parts for electric skateboard</b></td><td><b></b></td><td><b>Price</b></td><td><b></b></td><td><b>Link</b></td></tr>
<tr><td><b></b></td><td></td><td></td><td></td><td></td></tr>
<tr><td><b>Motor</b></td><td></td><td>£69.00</td><td></td><td>http://alienpowersystem.com/shop/brushless-motors/aps-6355hev-outrunner-brushless-motor-230kv-2400w/</td></tr>
<tr><td><b>ESC</b></td><td></td><td>£89.00</td><td></td><td>http://alienpowersystem.com/shop/esc/ev-esc/vesc/</td></tr>
<tr><td><b>ESC enclosure</b></td><td></td><td>£26.65</td><td></td><td>products/esc-enclosure</td></tr>
<tr><td><b>Controller/Remote</b></td><td></td><td>£45.70</td><td></td><td>products/torqueboards-2-4ghz-nano-remote-controller</td></tr>
<tr><td><b>Mechanical kit</b></td><td></td><td>£152.33</td><td></td><td>collections/featured-items/products/single-motor-mechanical-kit</td></tr>
<tr><td><b>Deck</b></td><td></td><td>£30.00</td><td></td><td>https://vandemlongboardshop.co.uk/collections/longboard-decks/products/lush-longboards-freebyrd-classic-deck-only-blemished</td></tr>
<tr><td><b>Battery</b></td><td></td><td>£36.26</td><td></td><td>https://hobbyking.com/en_us/zippy-compact-4500mah-6s-40c-lipo-pack.html</td></tr>
<tr><td><b>Battery enclosure</b></td><td></td><td>£26.65</td><td></td><td>collections/battery-enclosures/products/2x6s-rc-lipo-battery-enclosure</td></tr>
<tr><td><b>BMS</b></td><td></td><td>£9.52</td><td></td><td>https://hobbyking.com/en_us/6s-li-ion-10a-pcm.html</td></tr>
<tr><td><b>Charging port/power button</b></td><td></td><td>£4.94</td><td></td><td>https://www.amazon.co.uk/Wingsmoto-Charging-Repalcement-Self-balancing-Hoverboard/dp/B074TC551D/ref=sr_1_1?s=sports&ie=UTF8&qid=1516046379&sr=1-1&keywords=hoverboard+charging+port</td></tr>
<tr><td><b>Charger</b></td><td></td><td>£10.95</td><td></td><td>https://www.amazon.co.uk/Electric-Universal-Swagtron-Hoverboard-Connector/dp/B06XP5PJHR/ref=sr_1_4?s=sports&ie=UTF8&qid=1516046379&sr=1-4&keywords=hoverboard+charging+port</td></tr>
<tr><td><b></b></td><td></td><td></td><td></td><td></td></tr>
<tr><td><b>Total price</b></td><td></td><td>£501.00</td></tr></table>
```

---
## \#43 Posted by: atenner Posted at: 2018-01-16T21:23:36.890Z Reads: 53

```
I still think you can tweak it a little and instead of paying customs on the stuff from DIY you can put that money towards making your board a bit more upgradable/better maybe . . . I might end up with a shitlist

Working . . .
```

---
## \#44 Posted by: atenner Posted at: 2018-01-16T22:03:07.016Z Reads: 57

```
Motor £64.45

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

Esc £110

Foc box (pick one up off the forum)

Elcosure £50 + ish maybe

@bigben will make you a beautiful one. I don’t know how much they are. I would say buy a long enclosure. Plenty of room and you shouldn’t need to buy a new enclosure if you upgrade to 18650’s PS you will ;)

OR

Post a wanted thread for someone to 3d print you a 2 part enclosure

Nano-x off the forum £40

Motor mount £49 (options on forum as well)

https://street-wing.com/product/street-wing-motor-mount/

Pulley kit £43 including shipping

http://www.electric-skateboard.builders/t/15mm-wide-pulley-kits-and-individual-parts-wheel-pulley-motor-pulley-belts-and-hardware/27184

Wheels - clones are annoying hard to find cheap in UK. I have a 5 sets coming to have a sample of. You can have a set £27.50. Aliexpress £40. OR SAVE UP A BIT AND BUY ABEC11 90mm’s !!!!!!!!!!!!!!!!!!!!!!! 

Trucks (taking a risk with these but meh) £21 free shipping

Look what I found on AliExpress
http://s.aliexpress.com/FFNRjIZb

Charge port gx-16 3pin £3.50

10s charger £32 (mail him and ask for uk plug and gx-16 before purchase)

Look what I found on AliExpress
http://s.aliexpress.com/iiaeEfy6

Lipo Batteries 2x5s YOU CAN HAVE MINE FOR FREE IF YOU COLLECT FROM DERBY

10s bms (bypass) £10 ebay I CAN GIVE YOU ONE FOR FREE 

Power whatyamcallit xt-90-s loop key £peanuts 

Deck - I dunno, the one you chose £30

Notes - this would be a budget build that will be easily upgradable to 18650’s (thats all you would HAVE to replace. + £0 customs
```

---
## \#45 Posted by: atenner Posted at: 2018-01-16T22:07:46.434Z Reads: 52

```
£470.45 not including some shipping or if you can’t get free stuff from me or the peanuts

OR 

£442.95 not including some shipping or if you can’t get free stuff from me or the peanuts. AND NOT INCLUDING YOUR ££ FOR YOUR SHINNY ABEC11 90mm 

🤪

Edit : someone will surely point out if I have missed something
```

---
## \#46 Posted by: Acido Posted at: 2018-01-16T22:14:10.168Z Reads: 50

```
Thats expensive, buy your cells at nkon they have reasonable prices
```

---
## \#47 Posted by: TheLastEnting Posted at: 2018-01-17T14:35:05.078Z Reads: 43

```
Well "local" might be a bit of a stretch if the Midlands are what we are using as a local area, but a group ride would be cool at some point.

Didn't know about the facebook page though, have you got a link or something for it?
```

---
## \#48 Posted by: atenner Posted at: 2018-01-17T14:55:08.692Z Reads: 34

```
Yes I suppose it’s not very local. I don’t mind traveling a bit, I just don’t really have time to go down to London where all the rides happen. If you search ‘uk e-sk8t’ on FB it’ll come up 👍🏻
```

---
