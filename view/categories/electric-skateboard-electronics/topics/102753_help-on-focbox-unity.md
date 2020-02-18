# Help on focbox unity

### Replies: 29 Views: 437

## \#1 Posted by: Shawnl55 Posted at: 2019-10-09T15:42:58.170Z Reads: 88

```
Hi, i just wanted to make sure, are there any things i need to change in the focbox to use hub motors with it? And i assume max brake current can be the same amps as max motor current? Im not sure what to put for max braking regen current.
```

---
## \#2 Posted by: deucesdown Posted at: 2019-10-09T21:22:24.581Z Reads: 74

```
These are pretty basic questions. You should probably read a LOT more before hooking up, there's some basic knowledge that's hard to impart by answering a few questions. This basic knowledge may prevent blowing your stuff up.

But, basically, battery max amps and regen should be matched to the capabilities of your battery pack, and motor max and -max should be matched to the capabilities of your motors. If it's too strong, all can be lowered to meet your skill level.
```

---
## \#3 Posted by: Shawnl55 Posted at: 2019-10-11T01:36:25.423Z Reads: 64

```
No, i know what my motors and battery can handle, but for regen, im not sure if u put it same as battery current or if u supposed to put it at a lower current/certain percent of the battery current. And for everything else im just making sure so i actually dont blow stuff up lol.
```

---
## \#4 Posted by: Shawnl55 Posted at: 2019-10-11T01:38:34.318Z Reads: 56

```
Actually im kinda confused on my max amps for my metroboard battery cuz on the website it say 30 amps Continuous and so i email metroboard to see what the max amps r and he said 30 amps. I asked on the forums but seems like no one knows. (or no one responds to me lol)
```

---
## \#5 Posted by: pundahh Posted at: 2019-10-11T02:02:14.136Z Reads: 55

```
[quote="deucesdown, post:2, topic:102753"]
But, basically, battery max amps and regen should be matched to the capabilities of your battery pack, and motor max and -max should be matched to the capabilities of your motors. If it’s too strong, all can be lowered to meet your skill level.
[/quote]

he already answered this for you
```

---
## \#6 Posted by: Shawnl55 Posted at: 2019-10-11T02:19:54.353Z Reads: 52

```
What i meant was im not 100% sure what my rated max amps r for my battery so i will just set it at 30 amps just to be safe.
```

---
## \#7 Posted by: pundahh Posted at: 2019-10-11T02:30:17.308Z Reads: 50

```
[quote="Shawnl55, post:4, topic:102753"]
i email metroboard to see what the max amps r and he said **30 amps**
[/quote]

didn't they give you the answer?
```

---
## \#8 Posted by: Shawnl55 Posted at: 2019-10-11T02:50:33.942Z Reads: 46

```
Yea, they said 30 amps max before the bms shuts down, but on the metroboard website it say 30 amps Continuous. So that was a little confusing for me because its 30 amps Continuous and max. Unless they meant it can output 30 amps Continuous but is also max which wouldnt make sense y they would do that.
```

---
## \#9 Posted by: pundahh Posted at: 2019-10-11T02:54:58.882Z Reads: 44

```
go with 30a :slight_smile:
```

---
## \#10 Posted by: Shawnl55 Posted at: 2019-10-11T02:57:34.338Z Reads: 44

```
Yea lol. Thx
```

---
## \#11 Posted by: deucesdown Posted at: 2019-10-11T05:04:25.899Z Reads: 43

```
Hey. :) Generally you'll get more help if you post specifics, like a link to the battery pack. Otherwise you get vague stuff like my first post. Looks like this one?

https://metro-board.com/e-skate-shop/battery-metroboard/

* **10 mile Battery THIN** (10S2P, 36V 4.4AH) rated for 30 Amps Continuous Discharge, 14AWG Silicone Wires and XT60 Female Connector,  Electronic Switch to enable/disable discharge of Battery, 216 mm long x 160 mm wide x 21 mm high, 2.2 lbs.  [CHARGER](https://metro-board.com/e-skate-shop/charger-slim-2amp/)

Unity battery amps is total for both sides, so 30A is a reasonable choice here. BUT! if metroboards told you bms is max 30A, maybe give it a bit of headroom, as you _do not_ want the bms to trip. 25-28A perhaps.

For regen, you need to suss out what cells the pack has, and check the spec sheet on the cell. You can use 2x the max/fast charge rate safely. 2x because 2p. For example if the cell were Samsung 25R, [the spec sheet](https://www.powerstream.com/p/INR18650-25R-datasheet.pdf) says 1.25A standard, 4A max. So you can safely set regen to -8A. Note this is just an example -- don't use -8A.

The cell is NOT 25R though. The webpage for the packs proudly states LG MH1 for the bigger packs but conspicuously doesn't state for the smaller packs, which probably means generic chinese cells. I couldn't google it up. You'll have to ask metro what cells are in there, and what the max charge rate for that pack is.
```

---
## \#12 Posted by: Shawnl55 Posted at: 2019-10-11T05:19:30.475Z Reads: 38

```
The battery i have is the 55 mile one that uses LG MH1 like u stated in a 10s8p system.  This is actually very helpful, thanks.
```

---
## \#13 Posted by: deucesdown Posted at: 2019-10-11T05:25:08.681Z Reads: 39

```
Nice! spec sheet:

https://produktinfo.conrad.com/datenblaetter/1500000-1599999/001558879-da-01-en-LG_LIION_AKKU_INR18650MH1__3200MAH.pdf

standard charge 1.55A, max charge 3.1A, so your battery regen should be -(3.1A x p_size). You can tweak it a bit higher if it's not enough (within bms limits).

Did you say you have the 8p pack? MH1 max discharge is 10A on the spec sheet, so you're really hamstrung by that 30A bms.

If you're 8p, the cells can take -24.8, and chances are the bms can do -30, but check with metro, as that's unusually high regen current. Maybe start at -8 to -12 and see how it feels.
```

---
## \#14 Posted by: Shawnl55 Posted at: 2019-10-11T12:00:25.622Z Reads: 35

```
Ok thanks.
```

---
## \#15 Posted by: Shawnl55 Posted at: 2019-10-13T20:27:48.731Z Reads: 27

```
I was just wondering, do motors have limits on how much current can go through for battery regen?
```

---
## \#16 Posted by: deucesdown Posted at: 2019-10-13T20:30:44.580Z Reads: 29

```
Theroetically, yes. In practice you can if you wish to set it very high.
```

---
## \#17 Posted by: Shawnl55 Posted at: 2019-10-13T20:51:00.843Z Reads: 29

```
So should my motors affect what i put in max regen current?
```

---
## \#18 Posted by: drone001 Posted at: 2019-10-18T02:27:30.859Z Reads: 23

```
I'm thinking about getting that same battery in the interim. how do you like it so far, i wondered about that 30a BMS.
```

---
## \#19 Posted by: Shawnl55 Posted at: 2019-10-18T03:22:38.769Z Reads: 18

```
I haven't tested it yet cuz the remote is taking a while to ship. If u wait a little ill definitely tell u how it goes. If u are going to use belt motors, then i cant give an accurate say on how it is for belt motors cuz i am using hubs from a chinese company. But i do plan on switching to belt motors soon, i dont think u would want to wait that long just to get my opinion of the 55 mile battery tho.
```

---
## \#20 Posted by: Shawnl55 Posted at: 2019-10-18T03:35:05.995Z Reads: 18

```
If u worry the 30 amp limit of the bms is a bit low (i personally think so), u can get two 27 mile and connect them in parallel, u can get a total of 60 amps max. Theoretically, u will get the same range as the 55 mile battery cuz the 27 mile is a 10s4p with 12.8 AH and 55 mile is 10s8p with 25.6 AH(the 55 mile battery enclosure will fit two 27 mile cuz the 27 mile is exactly half the Height of the 55mile.) If u do that, it might cost a little more and u will have to do a bit of tweaking and soldering, mainly the charge cables and power on/off switch for the battery cuz u have 2 batteries (2 charge cable and 2 power on/off cable) and u only have 1 enclosure (1 charge port and 1 on/off switch.) Last time i checked they ran out of the 27 mile battery pack, so u could wait for more of those packs or just get the 55 mile to save u all that work, but with the cost of lower amps.
```

---
## \#21 Posted by: Shawnl55 Posted at: 2019-10-18T03:41:58.794Z Reads: 14

```
Btw if u get metroboard enclosure with 55 mile battery, the space for the esc is pretty limited. Im using a focbox unity and it perfectly fits. The unity seems like a very compact dual esc compared to other dual motor esc, so just watch out for that.
```

---
## \#22 Posted by: drone001 Posted at: 2019-10-18T03:56:23.183Z Reads: 14

```
thx, i'm also using a Unity. I don't see an option for the enclosure.
```

---
## \#23 Posted by: Shawnl55 Posted at: 2019-10-18T04:15:23.441Z Reads: 14

```
U have to email metro for the enclosure. Tell them the battery enclosure u want. for example, 55 mile battery u need 55mile battery enclosure.
```

---
## \#24 Posted by: drone001 Posted at: 2019-10-18T04:24:03.689Z Reads: 13

```
got it... thx i think i'll order this weekend
```

---
## \#25 Posted by: Shawnl55 Posted at: 2019-10-18T04:48:35.054Z Reads: 13

```
Nice. Just wondering, what set up for ur motors r u using? Gear ratio, motor kv, size, motor mounts, etc
```

---
## \#26 Posted by: drone001 Posted at: 2019-10-18T04:54:02.422Z Reads: 13

```
6374s 190Kv, 60/16t, 152mm sixshooters long Jaunx mounts with pressfits from @lrdesigns, SR RKPs, RedEmber the 44 deck 10 ply, 12s6p (waiting on battery repair...reason for the 10s from MB interim battery)
```

---
## \#27 Posted by: Shawnl55 Posted at: 2019-10-18T05:12:47.424Z Reads: 13

```
What range u get with that 12s6p?
```

---
## \#28 Posted by: drone001 Posted at: 2019-10-18T05:15:40.296Z Reads: 13

```
never lasted long enough for a good test. this will be the 3rd repair. this time doing a total rebuild.
```

---
## \#29 Posted by: Shawnl55 Posted at: 2019-10-21T11:36:43.401Z Reads: 9

```
If i use the vx1 with vesc 4 receiver and the focbox unity, what baud would i choose for uart mode?
```

---
