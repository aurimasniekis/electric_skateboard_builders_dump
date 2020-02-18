# Evolve Carbon GT Battery/BMS/ESC Upgrade

### Replies: 35 Views: 1256

## \#1 Posted by: asuras Posted at: 2019-04-16T13:25:27.921Z Reads: 172

```
I've bought an aftermarket LG HG2 10s5p battery to upgrade my CGT, foolishly thinking this would be a straightforward modification. During the install I accidentally plugged the Batt SW cable into the PSEN socket of the stock BMS, and now it seems the BMS is cooked; a BMS that is all but impossible to replace with the same one it turns out :roll_eyes:

So I investigated my options here and there seems to be a few opinions that plugging a 10s5p Li-Ion into the stock BMS is not advisable anyway and could result in a fire hazard. Apparently this is why Evolve themselves refuse to install a replacement BMS if you have an aftermarket Li-Ion battery. I heard that from a few different sources. One of these guys also told me that even if you do decide to go with the stock BMS, quite often the ESC will fail shortly thereafter, something to do with the way a Li-Ion battery discharges compared to the stock battery. This particular guy runs a business building and selling Li-Ion packs and has done dozens of upgrades on Evolve boards and this was his experience, so I tend to trust his point of view. And thus I don't really care to get another Evolve BMS into this rig...

Currently I have the 10s5p LG HG2 battery pack in perfect working order, all cells are balanced perfectly and I just want to get this board working again with some decent components; so I'm looking to swap out the BMS and ESC with something higher quality that will fit into the CGT enclosure. The battery pack came with a spacer to lower the heatsink in the ESC cavity, thus allowing me to mount the BMS on top of the ESC, so even though the new pack doesn't incorporate the BMS I have a little wiggle room space-wise. I'm running MBS A/T tyres on stock evolve hubs.

I assume I'm not the first person to do this upgrade, so can anyone recommend a good BMS/ESC/Remote combo that will do the job? I don't mind throwing extra $ at the problem if it will give me a reliable solution that won't overheat or disconnect - this is especially important as I sometimes tow a cargo trailer and the stock BMS (no heatsink) struggled a bit with overheating issues, especially on steep inclines.

One caveat is that I don't want to go with a FOCBox; and I've heard good things about Flipsky & Alien Power BMS's so if there's anything in those ranges you'd recommend that would be a great help. Eventually I'd also be looking to slightly upgrade the motors to help deal with the extra load of towing a trailer, although I don't think that factors into the purchase of these particular components. I'm doing my own research on these components currently as well, but I figure there'd be a few noggins in here that are waaay ahead of me? :face_with_raised_eyebrow:

Edit: Also does anyone know if I can fit dual 6374s onto the stock motor mounts (or get modified mounts that will)? Seems like the only way to get high torque & low kv motors is 6374/6384
```

---
## \#2 Posted by: M.Hboards Posted at: 2019-04-16T15:27:25.847Z Reads: 138

```
[quote="asuras, post:1, topic:90742"]
One caveat is that I don’t want to go with a FOCBox
[/quote]

Why not ? A focbox unity with a remote and charge only bms would be perfect your case.
```

---
## \#3 Posted by: asuras Posted at: 2019-04-16T15:36:39.240Z Reads: 138

```
[quote="M.Hboards, post:2, topic:90742"]
Why not ? A focbox unity with a remote and charge only bms would be perfect your case.
[/quote]

merrr, lets just say my help for doing this build has a gripe with the Enertion guy, something about him stealing the VESC stuff from the creator and apparently not paying him for stealing his tech. I dunno, just what I was told. :man_shrugging:

Looking at it, it would be suitable except that I'm going to run into clearance problems with the 19mm height, but same goes for my other top choice which is a [Dual FSESC6.6 Based upon VESC6 with Aluminum Heatsink](https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink)

Even with the ESC lowered with the spacer by my measurements there's about 13mm clearance left on top, and I have a feeling the only way around this is to get a new, thicker, spacer printed. (Any leads on that would be helpful!), or alternatively go with some super-thin ESC that probably won't allow me to run > 50A motors...
```

---
## \#4 Posted by: M.Hboards Posted at: 2019-04-16T15:44:29.158Z Reads: 122

```
Just something to keep in mind -The unity has a built in power switch and the flipsky doesn't.

[quote="asuras, post:3, topic:90742"]
stealing the VESC stuff from the creator and apparently not paying him for stealing his tech
[/quote]
Just so you know the vesc is an open source project meaning anyone can use the "vesc tech" for free. flipsky and enertion both take advantage of it. (Not in a bad way like abusing it but that they both use the "vesc tech" without paying for it.)
```

---
## \#5 Posted by: asuras Posted at: 2019-04-16T15:52:30.237Z Reads: 114

```
[quote="M.Hboards, post:4, topic:90742"]
(Not in a bad way like abusing it but that they both use the “vesc tech” without paying for it.)
[/quote]

Well his view is that Flipsky kicks back some margin to the creator but Enertion doesn't, I assume there's some sort of internet bitch fight that this all stems from.

Does the built-in power switch really help me though? I mean my board already has one I guess it just needs to be plugged in or soldered on to any other ESC. I should also add, the total height clearance currently available for the ESC/BMS stack is 24mm total which isn't a lot. I'm probably going to have to get that thicker spacer...
```

---
## \#6 Posted by: M.Hboards Posted at: 2019-04-16T15:58:00.067Z Reads: 109

```
The regular switch on your evolve won't work as it ties into your esc which has a anti spark circuit built-in like the unity if you just solder In the switch the switch you have now it will burn up.
```

---
## \#7 Posted by: KaramQ Posted at: 2019-04-16T16:03:18.710Z Reads: 100

```
I have a freind who has a replacement bms as well as a replacement gen 3 evolve esc
```

---
## \#8 Posted by: asuras Posted at: 2019-04-16T16:05:52.059Z Reads: 99

```
Definitely interested in the BMS! If he can post to me in Australia that would at least get me up and running while I shop around for the upgraded parts, send me a PM if he's interested in getting rid of it and he knows it's in good working order.
```

---
## \#9 Posted by: asuras Posted at: 2019-04-16T16:10:43.755Z Reads: 100

```
[quote="M.Hboards, post:6, topic:90742, full:true"]
The regular switch on your evolve won’t work as it ties into your esc which has a anti spark circuit built-in like the unity if you just solder In the switch the switch you have now it will burn up.
[/quote]

Ah ok, thanks for the tip, duly noted. I also just found this https://www.thingiverse.com/thing:2883308 
but looks like it's not designed for a Unity, so I'll still have to do something to create more clearance in that cavity. I think I'll need around 45mm total once a new BMS is in there too...
```

---
## \#10 Posted by: asuras Posted at: 2019-04-17T07:17:06.464Z Reads: 87

```
@M.Hboards With the ESC's, do you know if the Flipsky and FOCBox Unity come in a standard size heatsink that will just "fit" on my evolve? So their heatsinks are the same size and same threading as the evolve ESC? 
I can't even find dimensions for the Flipsky Dual FSESC 6.6 on their website...

EDIT: Nevermind I just found them, and the Flipsky is too big to fit into the Carbon enclosure without making some sort of weird 3D-printed drop-through cavity, but the FOCBOX will fit easily
```

---
## \#11 Posted by: asuras Posted at: 2019-04-17T11:57:02.948Z Reads: 83

```
So far I've narrowed down my shopping to:
1. [FOCBOX UNITY ESC](https://www.enertionboards.com/focbox-speed-controller/focbox-unity-dual-motor-foc-controller-esc/)

2. Dual [Turnigy Aerodrive SK3 - 6374-149KV Brushless Outrunner Motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html)

   Or  
Dual  [Turnigy Aerodrive SK3 - 6374-168KV Brushless Outrunner Motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-168kv-brushless-outrunner-motor.html)

Now I'm just trying to pick a suitable BMS, but I'm not sure how to figure out what Amp rating I need to target?

I would like charge and discharge protection, I have about 135x115x~20mm space to play with. 
The batt pack is a 10s5p LG HG2, the motors only say they have a 70A max loading. Does that mean I need a BMS that can handle the smaller of the battery draw vs. the combined peak draw of the two motors?  And I'm pretty clueless how to figure out what a typical cruise draw would be. If it helps I'm pretty light at around 65kg, and run A/T tyres, there is plenty of hilly action where I live, I hope to have a board that can pull me at around 40-45 km/hr on the flat. However, I also tow a trailer with this board which is why I'm angling more towards a torquey rig rather than a top-speed rig. 

Any advice here on specs I should shoot for would be appreciated, there's definitely a lot of BMS's that I know would do the job but generally they're all too long to fit in the enclosure. Really hard to find a smart, high amp BMS that has a small footprint.
```

---
## \#12 Posted by: Vero Posted at: 2019-04-17T12:14:39.012Z Reads: 74

```
you're discharge protection is your vesc? No point limiting yourself by using a bms imo
```

---
## \#13 Posted by: never4getf150forums Posted at: 2019-04-17T15:00:32.265Z Reads: 73

```
oof, so you burned out your bms.

bummer.

dibs on that bms :rofl:


i'd suggest lookin for a new bms, doing the bms install correctly and voila, you have a sick modded evolve board.

i know a lot of guys who have done it with no issues, the discharge isn't true, because it will only discharge what it uses, and it uses the same amount of power available on the original pack the only caveat being it has no voltage sag.. trust me, the bms isn't an issue, you just had to install it right and prove that guy wrong.

the single biggest reason these packs fail over time is because the pack itself is built wrong, either spot welded or soldered terribly which fails over time.
```

---
## \#14 Posted by: asuras Posted at: 2019-04-17T15:59:20.457Z Reads: 69

```
Yeah I didn't realise I don't need discharge protection on the BMS if its in the vesc already, so that opens up a ton of options for a low-profile BMS. One guy has suggested a [D140](http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/BMS-D140.html) which is a charge only BMS, does that sounds like a good option for this combo?
```

---
## \#15 Posted by: asuras Posted at: 2019-04-17T16:02:20.716Z Reads: 70

```
Yeah you might be right, as that guy builds and sells his own batt packs and he might be making crappy ones for all I know. However another guy helping me with this thought that it's possible that Li-Ion cells could produce intermittent voltage spikes (or something of that nature) that the stock BMS isn't handling and thus could damage the ESC over time, but that's just a theory...
```

---
## \#16 Posted by: Jaydawg56 Posted at: 2019-04-19T00:48:40.167Z Reads: 65

```
Similar build on my GT. 

Maytech sealed 6374 @170kv
10S5P Sony VTC6
Unity
Charge only BMS (HCX-D124 I think**) looking 4 receipt
Hm-10 BL

I used a spacer to give me some breathing room in the enclosure.  Doesn’t add much IMO and it provided some space for an already snug enclosure. 

Good luck! 

![image|375x500](upload://8DEbA6soYihgIJGDjDk1Uskvk5H.jpeg)
```

---
## \#17 Posted by: Jaydawg56 Posted at: 2019-04-19T00:49:20.965Z Reads: 63

```
![image|375x500](upload://m33BtgBgEYy9tTUoBDVWQLaPcK9.jpeg)
```

---
## \#18 Posted by: esk8jpn Posted at: 2019-04-19T04:14:36.089Z Reads: 62

```
Nice Carbon build! @Jaydawg56
```

---
## \#19 Posted by: asuras Posted at: 2019-04-19T06:00:44.814Z Reads: 63

```
Nice! Very similar to what I'm doing except I'm going for a full BMS, I know it'll be more expensive and a tighter squeeze but I don't like the thought of my board bursting into flames due to an unbalanced discharge, however remote that risk might be... Where'd you get the spacer? Looks sexy as. I have made up an STL of one that will give me and extra 20mm, but have since found an awesome tiny full BMS that might not require that much headspace. [Tiny BMS s516 - 150A/750A](https://www.energusps.com/shop/product/tiny-bms-s516-150a-750a-36?category=4)

What's your opinion of going to 170kv? Whats your top speed on that rig? I am sticking with pneumatics (8" = 200mm) and not sure if gearing 15/66 would give this thing too much top end to be comfortable, I don't really like going over 42ish km/hr, things get a bit sketchy haha
```

---
## \#20 Posted by: Kingdom421 Posted at: 2019-04-19T06:07:05.613Z Reads: 63

```
@Jackaltruckin here's one
```

---
## \#21 Posted by: Wizeartz Posted at: 2019-07-11T20:15:24.505Z Reads: 53

```
Slick Carbon Jaydawg! I've just bought an old CGT on AT's that I'll jam an 18650 into, probably 10S5P, with stock electronics until something blows up.
```

---
## \#22 Posted by: Jaydawg56 Posted at: 2019-07-11T20:57:09.763Z Reads: 55

```
Thanks.  No room for pcb, let me know if you take another approach. Otherwise, the butterfly approach is about the only config you can do.

A little wolf in sheep’s clothing. To confuse the masses, haha

![image|375x500](upload://fWaOYZuDE4V09E86yLo674VRIGx.jpeg)
```

---
## \#23 Posted by: Wizeartz Posted at: 2019-07-11T20:57:57.653Z Reads: 54

```
Ah, good to know! Thanks mate
```

---
## \#24 Posted by: Jaydawg56 Posted at: 2019-08-22T19:23:26.344Z Reads: 47

```
Hey bro, think I want to order some 4P groups.  Can you send me the info on the PCBs? I am paying $1.20 USD plus shipping and I think I might as well go bulk order. Thanks

Jason
```

---
## \#25 Posted by: Wizeartz Posted at: 2019-08-22T21:27:54.310Z Reads: 44

```
I think I still have 10 of them in my kit, as I’m going 10s5p on my next pack so won’t need them. Can send you the gerber files too though.
```

---
## \#26 Posted by: Wizeartz Posted at: 2019-08-22T22:21:01.949Z Reads: 44

```
Hit me up via wizeartz@gmail.com and I'll email you the gerber file set mate.
```

---
## \#27 Posted by: Jaydawg56 Posted at: 2019-08-22T22:30:07.098Z Reads: 44

```
Ah cool. But I think shipping over the pond might make it a moot point.   How about that batt spacer? Did you end up perfecting it?
```

---
## \#28 Posted by: Wizeartz Posted at: 2019-08-22T22:50:09.579Z Reads: 43

```
Yep, the last recipient was very happy with the fit. I'll be doing the controller spacer for CGT soon with my upgrade too.
```

---
## \#29 Posted by: Wizeartz Posted at: 2019-09-11T10:09:22.479Z Reads: 35

```
![image|375x500](upload://gqzf3o1Pozx12NTtpFU8lDT5s10.jpeg) ![image|666x500](upload://fMIIRrwhW5KqFkW4yzuIRVHkG8c.jpeg) ![image|375x500](upload://7cCJ4wq7IrAIQZ3CWN87dBXw1vv.jpeg)
```

---
## \#30 Posted by: Jaydawg56 Posted at: 2019-09-11T11:01:58.223Z Reads: 34

```
Ooooh interesting.   You went braid to wire. How did you mate those two up? Soldered it?
```

---
## \#31 Posted by: Wizeartz Posted at: 2019-09-11T19:35:39.540Z Reads: 33

```
Yeah, I drowned the braid in solder and it bonded nicely to the nickel strip. No fat 12AWG to contend with until the end of the pack where the braid runs off the end. Went 35E's on this one too, see if I get any more range out of her. Will put 8" MBS as well, for commuting to work. Love the stiffness of the carbon.
Did you get your PCB's?
```

---
## \#32 Posted by: Wizeartz Posted at: 2019-09-11T20:03:24.767Z Reads: 33

```
Going to make my own badge too... reworking the original kit to perform like it should've out of the box, Revolve, whaddya think?:grin:
![RevolveBadge|180x195](upload://clOXntnICDVbpjuuomLpXL8tiWL.jpeg)
```

---
## \#33 Posted by: Wizeartz Posted at: 2019-09-13T09:00:11.308Z Reads: 33

```
Just finished my 10S5P pack for the CGT, but I’ve encountered a problem! I plug the battery in and it turns on, even when the power button is set to off. I then unplug the switch from the controller board, and it still turns on as soon as I plug the battery in! Any thoughts?  ![image|375x500](upload://6R30noWmePHfPJqai5FQum3Gquc.jpeg) ![image|375x500](upload://wl7YtwZ5s4V2LwcTStJSF0F9HdU.jpeg)
```

---
## \#34 Posted by: Kram720 Posted at: 2019-11-04T13:02:44.681Z Reads: 26

```
Hard to see in the pic but your neg battery and neg power out to esc might be around the wrong way on the bms.
Bat neg go’s to the corner. Neg bms to escfrom the middle of the bms
How did the range go with 35e
With a 31v cut of there is still a lot of energy in the cells
```

---
## \#35 Posted by: Wizeartz Posted at: 2019-11-04T19:10:05.296Z Reads: 23

```
Thanks very much, you were dead right! I swapped them around and now it works fine. It cuts out in GT mode though, even though I've moved the heat sensor away from electronics etc. FAST is fine though, I'm getting up to 42 km/h and at least 20Km range on 8" AT tyres, 55psi, with all up weight of 180lbs.
```

---
