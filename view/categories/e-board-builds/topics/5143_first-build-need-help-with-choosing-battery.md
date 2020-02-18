# First build! Need help with choosing battery

### Replies: 28 Views: 5229

## \#1 Posted by: ouch_fiyah Posted at: 2016-06-25T21:15:18.938Z Reads: 283

```
1. Reusing longboard deck
2. Caliber 2 Trucks
3. Shock/Raiser pads
4. Ebay flywheel clones
5. DIY's Mount/drive kit
6. VESC
7. DIY's 230kv Motor (was looking at sk3 motor but it always seems out of stock)
8. Either 6s or 10s battery
9. DIY's Torqueboard nano remote

I want to build a good/decent board and be able to upgrade later one if I need to. One thing I'm having trouble with is what battery to choose. What would be good battery specs (or spec range) for my build? (thinking of 10s battery).

For example: I'm looking at a battery on aliexpress, [Battery link](https://www.alibaba.com/product-detail/good-quality-and-high-power-36v_60398470947.html?spm=a2700.7724857.0.0.End5Df&s=p) they have a whole spec sheet and so if I were looking around for batteries, I wanted to know what specs I could use.

Also, if anyone had other suggestions for better/more bang for your buck parts, i'd be happy to know them!
```

---
## \#2 Posted by: mattdig Posted at: 2016-06-25T21:34:06.938Z Reads: 269

```
Figure out how much you want to spend on a balance charger. If you want to start with 6s then upgrade to 10s you'll want to get a 10s charger from the start. That's the mistake I made.
```

---
## \#3 Posted by: Luke Posted at: 2016-06-25T21:46:35.344Z Reads: 257

```
A 230kv motor may hit the erpm limit using a 10s battery, if you were to use a 10s battery a lower kv motor may be beneficial. If you get a 10s battery are you considering the diy  pre-made li ion battery which comes with a charger and BMS, or would you prefer to use lipo batteries?
```

---
## \#4 Posted by: Pablo_702 Posted at: 2016-06-25T22:17:30.671Z Reads: 242

```
Check @oriol360 at miami electric boards hes taking orders for 12S 18650 with bms and charger for cheap, about the same as if you go the lipo batteries, and have to buy a charger and all thatcrap
```

---
## \#5 Posted by: Jinra Posted at: 2016-06-25T22:29:01.858Z Reads: 248

```
230 should be okay as it only hits the 60k limit at full charge. Li-ions wont' stay at 4.2v for very long and will quickly drop to under the limit. He may encounter problems if he tries to go full speed at max voltage, though chaka said we have some wiggle room there. There have also been reports of DIY's motor actually being 190kv, so it might just work out for him/her.
```

---
## \#6 Posted by: Jinra Posted at: 2016-06-25T22:31:34.440Z Reads: 238

```
I'd be careful buying batteries from alibaba/aliexpress. That pack has a pretty low continuous current rating and having 4.4AH from a 3P pack sounds strange. My money is on them using low quality cells which may not last long or be able to handle DIY's larger, more power hungry, motor.
```

---
## \#7 Posted by: Pablo_702 Posted at: 2016-06-25T23:28:27.058Z Reads: 232

```
it sounds like you have the numbers down, i still dont get it would you help me figure out what my erpm are going to be on a full 12s 8000mah 30/40 C (6374 149kv) 16/36 gearing
```

---
## \#8 Posted by: Jinra Posted at: 2016-06-25T23:32:28.194Z Reads: 227

```
about 52500 max. you'll be fine!
```

---
## \#9 Posted by: Pablo_702 Posted at: 2016-06-25T23:50:13.975Z Reads: 223

```
would you mine breaking it down for me so i dont have to ask you every time i change pulleys or wheels size
```

---
## \#10 Posted by: ouch_fiyah Posted at: 2016-06-26T00:12:26.727Z Reads: 223

```
Thanks for the reply guys! 

@Pablo_702 I would choose a premade DIY battery pack for the convenience since I'm still new at this. I can solder but I'm not sure about where to buy legit 18650 batteries and what BMS chip, and how to put it all together (though i'm sure there are plenty of tutorials out there).

How is erpm calculated? But with the erpm in mind, I suppose I could go with a 6s and be just fine. I don't plan to commute with it (just joy riding). If I opt for a DIY battery pack (with the built in BMS), do I still need a balance charger? 

As an alternative, if I go for a 6s Lipo setup, what would be a good setup? (Which batterties/BMS/Charger/ and anything else i missed, would I need to buy?). I would probably opt for lipo's if it was (a lot) more cost effective.


Thanks for the help guys. Can't wait to get parts orderedd
```

---
## \#11 Posted by: Jinra Posted at: 2016-06-26T00:31:53.280Z Reads: 196

```
eRPM = (voltage)x(kv rating)x(7 pole pairs, for most 50-63mm motors)
```

---
## \#12 Posted by: Pablo_702 Posted at: 2016-06-26T00:47:13.625Z Reads: 186

```
so gearing dont play a role in erpm?
```

---
## \#13 Posted by: Jinra Posted at: 2016-06-26T00:49:26.037Z Reads: 187

```
nope. you calculate erpm without load.
```

---
## \#14 Posted by: ouch_fiyah Posted at: 2016-06-26T01:57:38.322Z Reads: 179

```
If I purchase a pre-made battery pack with a BMS (from DIY for example), do I still need a balance charger?
```

---
## \#15 Posted by: Jinra Posted at: 2016-06-26T02:14:21.968Z Reads: 176

```
BMS balance charges for you. so no
```

---
## \#16 Posted by: rpn314 Posted at: 2016-06-26T02:16:02.150Z Reads: 171

```
There's a few places to buy in here in the states that are good. [LiIon Wholesale](http://liionwholesale.com/) is the cheapest I've found..
```

---
## \#17 Posted by: jrpwit Posted at: 2016-06-26T04:06:22.611Z Reads: 163

```
I have a quick question. So I have a tacon 160 245kv and have it with a 12s battery. Could I just limit the erpm to 60k and it will be safe right? I haven't tried it yet cause I'm waiting on my enertion vesc.
```

---
## \#18 Posted by: Jinra Posted at: 2016-06-26T04:08:37.867Z Reads: 162

```
You could, just not ideal
```

---
## \#19 Posted by: jrpwit Posted at: 2016-06-26T04:09:55.431Z Reads: 164

```
So no damage to the vesc even if I go full throttle?
```

---
## \#20 Posted by: Jinra Posted at: 2016-06-26T04:11:14.977Z Reads: 166

```
nah, hitting erpm limit shouldn't damage the VESC anyway, just causes errors. The hard limit is 100k.
```

---
## \#21 Posted by: jrpwit Posted at: 2016-06-26T04:14:17.757Z Reads: 149

```
Oh seriously? Huh I must have misunderstood that kv thread. Thank for the help :)
```

---
## \#23 Posted by: chaka Posted at: 2016-07-12T13:57:35.092Z Reads: 132

```
> nah, hitting erpm limit shouldn't damage the VESC anyway, just causes errors. The hard limit is 100k.

The errors at high ERPM will actually blow the DRV8302. A good/bad analogy would be a misfire while redlining an internal combustion engine.
```

---
## \#24 Posted by: Jinra Posted at: 2016-07-12T14:04:35.115Z Reads: 126

```
my mistake!
```

---
## \#25 Posted by: chaka Posted at: 2016-07-12T14:22:04.725Z Reads: 129

```
No worries! There is a lot of information out there, it can be a challenge to digest.
```

---
## \#26 Posted by: Randyc1 Posted at: 2016-07-12T16:04:26.086Z Reads: 125

```
Just to be very clear ?,...when a ERPM of 60.000
Is Set ....and Hit at full throttle, what happens ??

- Damage to chip?
- just limiting rpm
- cutoffs ?
```

---
## \#27 Posted by: jrpwit Posted at: 2016-07-12T19:29:23.856Z Reads: 112

```
You can set the vesc to have a limited erpm below 60k so you cant exceed 60k erpm while riding (Im doing this). Yes going over 60k will damage the vesc and cause errors.
```

---
## \#28 Posted by: Randyc1 Posted at: 2016-07-12T22:22:48.798Z Reads: 117

```
My question is what happens when you hit the Set erpm limit ??

Does the motor just continue to run at that limit, or does the motor cut off ??... dont wanna be thrown off board if motor just cutts off when limit is hit ??
```

---
## \#29 Posted by: Jinra Posted at: 2016-07-12T22:36:45.025Z Reads: 109

```
From what I understand, it'll stop accelerating after hitting the set limit. If you check "limit erpm with negative torque" it'll slow down your board if it goes past the limit. Please correct me if I'm wrong.
```

---
