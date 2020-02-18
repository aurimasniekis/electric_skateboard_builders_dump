# What BMS to use for a 6s4p setup of 18650 Samsung 25r5s?

### Replies: 43 Views: 2731

## \#1 Posted by: FrozenFury Posted at: 2016-08-11T04:58:50.039Z Reads: 150

```
What BMS to use for a 6s4p setup of 18650 Samsung 25r5s?

Looking for something cheap, < 50 hopefully
```

---
## \#2 Posted by: barajabali Posted at: 2016-08-11T05:06:59.025Z Reads: 151

```
Just find a cheap bms (underrated) 20amp cont and bypass it. 

But you can use batterysupports bms they're mostly all pretty low cost
```

---
## \#3 Posted by: FrozenFury Posted at: 2016-08-11T05:07:25.092Z Reads: 148

```
I only need 20 amp?
```

---
## \#4 Posted by: barajabali Posted at: 2016-08-11T05:08:47.567Z Reads: 144

```
Hell no at 6s you need like 80 or more amp cont lol. 

But trust me that's not in your budget. So just get a 20amp bms and bypass it (only use the charge function) and let the cells deplete via the main terminals
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-08-11T05:15:55.912Z Reads: 135

```
If you don't bypass the bms at 20amps when you discharge you will fry the bms....

@barajabali is trying to save you money by getting a cheaper one and just bypassing it ... Since it's only a 6s
```

---
## \#6 Posted by: FrozenFury Posted at: 2016-08-11T05:17:17.625Z Reads: 125

```
Oh okay. how do i bypass it? does it require any soldering or anything?
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-08-11T05:17:41.707Z Reads: 123

```
It will all require soldering lol
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-08-11T05:18:45.347Z Reads: 124

```
[quote="FrozenFury, post:6, topic:7461, full:true"]
Oh okay. how do i bypass it? does it require any soldering or anything?
[/quote]

@barajabali care to draw a quick pic on a napkin for @FrozenFury?
```

---
## \#9 Posted by: FrozenFury Posted at: 2016-08-11T05:18:57.464Z Reads: 119

```
Right, but anything different? do i solder it the same way or is there a specific way with bypassing?
```

---
## \#10 Posted by: FrozenFury Posted at: 2016-08-11T05:19:14.163Z Reads: 115

```
Pls do @barajabali , thx!
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-08-11T05:20:22.640Z Reads: 113

```
Yeah... When you red and the black from the battery....it goes into the esc...instead of the BMS then ESC......basically
```

---
## \#12 Posted by: FrozenFury Posted at: 2016-08-11T05:23:12.530Z Reads: 111

```
Oh okay. So you put it into the ESC and then the BMS?

Battery -> ESC -> BMS

Like this?

Sorry for the dumb question - I know close to nothing about soldering
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-08-11T05:24:46.349Z Reads: 113

```
AC Charger to BMS to Batteries

Then a separate +/- from the battery to the ESC


If you notice ... When you use the power...you bypass the BMS completely
```

---
## \#14 Posted by: FrozenFury Posted at: 2016-08-11T05:26:55.983Z Reads: 110

```
ohhhh I see. So the BMS and ESC aren't directly connected which means the BMS doesnt have to pass the full power. That's what bypassing is, and what you mean right?
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-08-11T05:29:08.054Z Reads: 108

```
If you had say a 80amp bms or higher ...and used it


It would be AC - BMS - Battery

Then


Battery -BMS - ESC-MOTOR
```

---
## \#16 Posted by: FrozenFury Posted at: 2016-08-11T05:30:31.245Z Reads: 111

```
But instead what I need to do is

AC -> BMS -> Battery

Battery -> ESC -> Motor

Right?

Also is there any downsides to this?
```

---
## \#17 Posted by: Michaelinvegas Posted at: 2016-08-11T05:33:57.107Z Reads: 106

```
Correct 

.... That..question is best left for the pros .....

I think one issue is that you can't have the bms cut your power to protect your against over discharge ...but you can resolve that with sometypenof monitor
```

---
## \#18 Posted by: barajabali Posted at: 2016-08-11T05:37:29.844Z Reads: 107

```
All you need to do is ignore the instructions on how to connect the esc to the battery instead of following directions on that part just connect the esc directly to the main battery leads. (Bypass)

But you have to still follow the charging directions
```

---
## \#19 Posted by: barajabali Posted at: 2016-08-11T05:37:56.932Z Reads: 104

```
If you buy a supower bms I'll help you set it up
```

---
## \#20 Posted by: FrozenFury Posted at: 2016-08-11T05:38:34.697Z Reads: 104

```
Awesome! I'll buy one of those then. Where would I get it?

Also is there any downside to bypassing?
```

---
## \#21 Posted by: barajabali Posted at: 2016-08-11T05:40:07.734Z Reads: 98

```
Yes there are downsides. 
No over discharge protection. 
And no max amp pull 

But you'll be fine just stop riding when your battery says empty. 

You can get it from batterysupports.com
```

---
## \#22 Posted by: FrozenFury Posted at: 2016-08-11T05:41:40.682Z Reads: 95

```
Should I get this one?
http://www.batterysupports.com/22v-24v-6s-30a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-475.html
```

---
## \#23 Posted by: barajabali Posted at: 2016-08-11T05:44:47.857Z Reads: 92

```
yes and get this charger http://www.batterysupports.com/liion-lipo-252v-222v-2a-6s-wall-socket-battery-charger-ac-dc-p-135.html
```

---
## \#24 Posted by: FrozenFury Posted at: 2016-08-11T05:50:08.050Z Reads: 91

```
Should I buy it off of Ebay in order to avoid the $15 shipping charge?
```

---
## \#25 Posted by: barajabali Posted at: 2016-08-11T05:51:36.549Z Reads: 92

```
I order off ebay but it takes a long time... could be up to a month off ebay.

I order in bulk-ish so i dont mind it
```

---
## \#26 Posted by: FrozenFury Posted at: 2016-08-11T06:14:49.232Z Reads: 90

```
okay cool. I ordered the charger, but I couldn't find the BMS so I got a 7S BMS. This is the one: http://www.ebay.com/itm/221740200297

Will this work?
```

---
## \#27 Posted by: barajabali Posted at: 2016-08-11T06:16:35.979Z Reads: 89

```
no a 6s charger wont work with a 7s bms. 

it can but its gets even more complicated. id just order the 6s bms from them
```

---
## \#28 Posted by: barajabali Posted at: 2016-08-11T06:16:58.512Z Reads: 90

```
where did you order the charger from?
```

---
## \#29 Posted by: FrozenFury Posted at: 2016-08-11T06:32:45.455Z Reads: 91

```
Okay I changed my order. This is what I ordered:

http://www.ebay.com/itm/321751878865?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
http://www.ebay.com/itm/321823419482?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
## \#30 Posted by: FrozenFury Posted at: 2016-08-11T06:44:02.029Z Reads: 86

```
By the way I was thinking of getting a VESC. Should I get that? If yes, Should I get it from Enertion?
```

---
## \#31 Posted by: lox897 Posted at: 2016-08-11T07:12:00.798Z Reads: 84

```
Ollin = Highest Quality IMO 2 week lead time  (bit more expensive
Enertion = Ok quality (not sure of lead time)
DIY = heard good things about it
```

---
## \#32 Posted by: jrpwit Posted at: 2016-08-11T07:16:13.494Z Reads: 83

```
Wait... why not just get the 6s 60A BMS? It's only 6 buxs more than the 30A one... That way you can keep it connected all the time and not just for charging. This way when you are discharging your battery the BMS will not let the cells get out of balance, ultimately making your battery last longer.. Even with 6s I doubt you will be hitting 60A from your battery. I don't understand why everyone is telling you to save the money by getting a lower continuous BMS when a proper BMS is only 6 bux more. You still will have to deal with the terrible shipping either way.
```

---
## \#33 Posted by: Michaelinvegas Posted at: 2016-08-11T07:18:03.997Z Reads: 80

```
He could do anything he wants including paying a tiny bit extra ... We are just giving him choices ... He knows he can run the pack through the bms if he wanted with the right amp rating
```

---
## \#34 Posted by: jrpwit Posted at: 2016-08-11T07:18:40.182Z Reads: 80

```
OBC undoubtedly makes the best vescs and with a great 12 month warranty!
```

---
## \#35 Posted by: jrpwit Posted at: 2016-08-11T07:20:05.637Z Reads: 76

```
Oh okay. I just would think that the 6 bux would go a long way by making his battery last longer.
```

---
## \#36 Posted by: Michaelinvegas Posted at: 2016-08-11T07:21:04.482Z Reads: 74

```
Yeah are arguments for and against using a BMS....

Not sure which side he's on lol
```

---
## \#37 Posted by: FrozenFury Posted at: 2016-08-12T05:05:51.669Z Reads: 68

```
I just opted for the 60A BMS so that I don't have to bypass. Will that be enough amps to go uphill and sustain cruising for long periods of time do you think?
```

---
## \#38 Posted by: Michaelinvegas Posted at: 2016-08-12T05:30:40.344Z Reads: 70

```
Should be mate
```

---
## \#39 Posted by: Bibzz Posted at: 2017-11-09T16:16:05.699Z Reads: 26

```
Does this bms work for 10s1p 18650 25r setup? 
 <img src="/uploads/db1493/original/3X/7/c/7c215bf850cec87b283e628275fa1c9e0f10d18f.jpeg" width="298" height="500">

http://www.batterysupports.com/36v-37v-42v-10s-30a-10x-36v-lithium-ion-lipolymer-battery-bms-p-265.html

This help will be highly appreciated thanks!
```

---
## \#40 Posted by: barajabali Posted at: 2017-11-09T17:08:19.815Z Reads: 25

```
Yes just get the 60amp model
```

---
## \#41 Posted by: Bibzz Posted at: 2017-11-09T19:26:35.503Z Reads: 24

```
Not the 30 amp? Even though I'm using the lithium 18650 25r ?
```

---
## \#42 Posted by: barajabali Posted at: 2017-11-09T19:54:50.656Z Reads: 22

```
yes you'll be pulling more than 30 amps with a 6s setup. You can use the 30amp if you decide to bypass it
```

---
## \#43 Posted by: Bibzz Posted at: 2017-11-09T22:48:46.305Z Reads: 20

```
But I'm just doing the 10 in series (10s 1p) not 6s ?
```

---
