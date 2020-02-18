# Charging a 9s3p battery HELP

### Replies: 27 Views: 1298

## \#1 Posted by: Acido Posted at: 2017-09-12T19:08:45.708Z Reads: 97

```
This is the battery [link](https://hobbyking.com/en_us/zippy-4000mah-3s1p-30c-hardcase-pack.html)

How can i charge this without having to disassemble everything

I want to make a plug in and charge solution for my future board

Also how much would an bms cost for this kind of a battery since i do not want to balance everything out i do not have the time for it

any help is highly appriciated
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-09-12T19:09:40.747Z Reads: 96

```
You mean for two of those in series?
```

---
## \#3 Posted by: Acido Posted at: 2017-09-12T19:14:24.607Z Reads: 93

```
I mean 3, sorry for the wrong title, also the motor is 10s [link](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html) should it work?

So the correct title will be 9s3p
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-09-12T19:15:34.937Z Reads: 87

```
The motor won’t be a problem, my guess would be that a BMS would be about $60 and toooooootaly worth it
```

---
## \#5 Posted by: Acido Posted at: 2017-09-12T19:19:55.749Z Reads: 79

```
Could you please link some model to me i can not find anything more than 6s on hobbyking

Also how much would an charger cost approx
```

---
## \#6 Posted by: Emerson Posted at: 2017-09-12T19:21:20.864Z Reads: 78

```
I'm sure there's a wiring diagram on the forum somewhere for wiring your batteries in series for use and parallel for easy charging.  I'd definitely recommend going the route of a BMS if you feel capable.
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-09-12T19:21:53.595Z Reads: 77

```
http://www.bestechpower.com/333v9spcmbmspcbforli-ionli-polymerbatterypack/PCM-D266.html
Boom.  Charger is probably about $10-$20
```

---
## \#8 Posted by: Acido Posted at: 2017-09-12T19:28:13.339Z Reads: 70

```
Thanks a lot man i found some bms for about 20ish$ aliexpress one (i guess i can trust it) and my friend has got just the right charger :smiley:
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-09-12T19:58:09.452Z Reads: 68

```
What’s the discharge rate on the aliexpress BMS
```

---
## \#10 Posted by: JdogAwesome Posted at: 2017-09-12T20:41:10.817Z Reads: 59

```
Yeah I found a cheap one for about $10 on AliExpress, discharge is only 20A though I recommend bypassing it anyways. I also found a 9S LiPo charger on eBay for $20 as well, though you could also build your own PSU which would charge faster as well.
```

---
## \#11 Posted by: Acido Posted at: 2017-09-13T06:00:33.137Z Reads: 41

```
How complicated is it to do that
```

---
## \#12 Posted by: Acido Posted at: 2017-09-13T06:01:53.632Z Reads: 40

```
also is it safe to charge more than one cells Ah rating, I red somewhere here that it is not
```

---
## \#13 Posted by: JdogAwesome Posted at: 2017-09-13T06:16:47.243Z Reads: 40

```
How complicated is it to do which? Bypass BMS or build a charger. If it's the former than it's quite easy and plenty of people have shown how to do it. 

The later is a little bit harder though it depends on what kind of experience you have with electronics as well as CC/CV converters. If you know what your doing its quite easy like it was for  me though if your new to this, it may be pretty hard to wire everything together.
```

---
## \#14 Posted by: scepterr Posted at: 2017-09-13T06:28:54.344Z Reads: 43

```
42v charger + dctodc buck CCCV, charge any voltage you want up to 42V<img src="/uploads/db1493/original/3X/a/5/a5da4a69269f675e356d310d8d91b2d58261f686.jpg" width="333" height="250">
```

---
## \#15 Posted by: Acido Posted at: 2017-09-13T07:33:44.945Z Reads: 42

```
None so i guess i will have to read a bit also whats a ladder?
```

---
## \#16 Posted by: JdogAwesome Posted at: 2017-09-13T14:01:54.524Z Reads: 39

```
Oh lol the later(not ladder, woops) is a term for the second option, the former is the first option. So when I said "Bypass BMS or build a charger." and I said the later it meant build a charger. Anyways yeah you could do what @scepterr said with a DPS5005 or DPS5015 module depending on how fast you want to charge it, though that will be the more expensive option rather than doing something like a [R33 Mod](https://endless-sphere.com/forums/viewtopic.php?f=2&t=42793) with a PSU and that way all you need is the PSU and a current and voltage meter. @VladPomogaev has a good tutorial on how to do this [HERE](https://www.instructables.com/id/Fast-Electric-Skateboard-LiPo-Charging-System-BMS-/).
```

---
## \#17 Posted by: Acido Posted at: 2017-09-13T15:38:41.480Z Reads: 33

```
I just read this article and im not sure if i understand it well 
[this](http://www.bestechpower.com/333v9spcmbmspcbforli-ionli-polymerbatterypack/BMS-D270.html) bms can do only 25A but the motor is 60A max is that a problem, im not sure will it catch fire or something lol
```

---
## \#18 Posted by: MysticalDork Posted at: 2017-09-13T15:50:02.218Z Reads: 33

```
There are two ways to use a BMS, either discharging through the BMS or bypassing the BMS  for discharge. Discharging through the BMS is safer because then you have an extra layer of cutoffs to protect the battery, but you're limited to the discharge current of the BMS, so to do this you generally have to buy a more expensive one to get a decent rating. If you bypass the discharge, then you don't have the safety features, but you can use a smaller, cheaper BMS.
```

---
## \#19 Posted by: Acido Posted at: 2017-09-13T15:54:17.357Z Reads: 31

```
I want a bms to charge the batteries for me balance them out etc and for the battery voltages when riding, wouldnt voltage of the batteries be the esc job to monitor when riding?
```

---
## \#20 Posted by: JdogAwesome Posted at: 2017-09-13T16:03:53.485Z Reads: 26

```
The BMS will manage your batteries it will balance them and whatever, though it will not have the low voltage cutoff protection or short protection if you bypass it. However yes with the VESC you can set low voltage cutoff so that you can't drain your battery to much that way though your board will still be on and it will remain on until the battery's are completely dead and ruined. So you have to make sure your turn the board off which is isn't to hard anyways lol.
```

---
## \#21 Posted by: Acido Posted at: 2017-09-13T17:01:01.126Z Reads: 23

```
Yea, i will also have a master switch to disconnect the batteries from the engine so i can push the board without problems (i think there could be some will do some research)
```

---
## \#22 Posted by: JdogAwesome Posted at: 2017-09-13T17:04:37.870Z Reads: 20

```
Unless you completely disconnect the motor from the VESC you could have problems, I'd recommend having your board on when your pushing it.
```

---
## \#23 Posted by: Acido Posted at: 2017-09-13T17:05:47.322Z Reads: 20

```
Isn't it when a motor runs like manually like when you spin it with your hand it creates electricity, is that electricity a problem here
```

---
## \#24 Posted by: MysticalDork Posted at: 2017-09-13T17:08:28.501Z Reads: 19

```
Yes. The back-emf (the generated power) will power the vesc enough to turn it on, and then the vesc will try to brake. It's hard on the electronics.
```

---
## \#25 Posted by: Acido Posted at: 2017-09-13T17:09:46.961Z Reads: 20

```
You seem like an experienced guy, how could i solve this problem
```

---
## \#26 Posted by: MysticalDork Posted at: 2017-09-13T17:20:59.078Z Reads: 19

```
The simplest way is to just physically disconnect the motor from the vesc if you're going to push it manually. I personally don't push, so my experience is limited in that respect.
```

---
## \#27 Posted by: Acido Posted at: 2017-09-13T17:24:17.291Z Reads: 22

```
I will just make one switch between motor and the esc and one between battery and the esc, also i did some calculations last night and the range would be 25km minimum if that's the minimum range i wont even do it since its enough for a day
```

---
