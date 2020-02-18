# Advanced Remote, BMS and battery concerns / 2WD switchable to 4WD setup

### Replies: 2 Views: 371

## \#1 Posted by: Froggy Posted at: 2017-11-06T16:07:51.877Z Reads: 100

```
Hi guys
I'm new here and currently planning to build up a switchable 4WD to 2WD board. (Still in the engineering process though.) The board should be around 96 cm long (Around 38 inches, pintail shape)
Two main reasons for this:
- 4WD will increase its torque and max speed (traction under a given weight)
- Lighter weight on each motor will prevent them from overheating on starts and braking. (Smaller hubs seems to be known for this, and I'd like to prevent it)
Here are in brief the parts that i plan to use:
- 4 hub motors (Maytech, 70 mm hubs, 450W, 22A max current, 100kv each)
- 2 dual ESCs (Maytech, 2X30A continuous each)
- A total amount of 40 li-ion cells rated at 20A to 35A max discharge current each. I didn't chose the brand and capacity yet but it will be one of the big 3 brand, Samsung 25R, LG HG2 or Sony VTC5-5A or VTC6, depending on my budget. So the capacity should be from 10A/h up to 12A/h.
**Now here are my main concerns:**
**- The board should be switchable from 2WD to 4WD to preserve the total amount of available watts from the batt, and use 4WD only at starts, climbing and braking (Seems that it would be possible with a radio commanded ON/OFF switch, set between the front dual ESC and a single radio receiver splitted in two with a T wire  (one branch to each dual ESC, and paired to a dual channel remote) I definitely need more informations on this point. Some help would really be appreciated!**
I was initially planning to build a single 36V 10S4P battery to run the full setting. Then, the  smallest 80A max discharge BMS that would match with this set up, but may already limit the hubs a bit, as they need 22A max current each, definitely won't match the board's dimensions (I mean it may fit, but would jeopardize the deck's strenght, and destroy the nice "all buit in" design I'm currently engineering...)
SOOOO...
**Here is eventualy my (tough) question:**
**- Is it possible to set 2*10S2P in parallel, each of them managed by a 45A max BMS, but to link them to a single charging port?..  As 2 of them: https://fr.aliexpress.com/store/product/SuPower-10S-36V-37V-42V-45A-Li-ion-Lithium-LiPo-Battery-BMS-Management-System-Balance-PCB/605190_32800545892.html?spm=a2g0w.12010612.0.0.12a94e50Lip7ov would perfectly fit my design and wouldn't limit the hubs anyhow...**
I would gladly avoid the use of a big BMS or two smaller ones for discharge and use it (them) for balancing the cells when they charge only, sticking to a cheaper Ebay crap and bypassing discharge, but the dual ESCs being rated at 2*2*30A max discharge current (120A total) makes it a bit frightening for the battery life...( Even if i eventually use the Sony VTC5A rated at 35A discharge current, but closer to 25A in facts, and ridiculously expensive...)
So guys, if any of you feels comfortable and knowing enough on those topics, PLEASE, feel free to help (diagrams, technical drawings would be fairly appreciated!)
Here are a few screenshots from my 3D software. Work in progress... And yes... There are 40*18650 cells, 2 dual ESCs, and two 45A BMS in it... :grin:<img src="/uploads/db1493/original/3X/c/2/c2a31441db873fa1d01aca76c37cd7e0d9219f6f.jpg" width="689" height="401"><img src="/uploads/db1493/original/3X/3/c/3c1bbe3f81d53f20d426519555687071d15a7381.jpg" width="689" height="401">
<img src="/uploads/db1493/original/3X/5/2/52d38912220d9e2762b914add8c1c6a7d4d5e985.jpg" width="689" height="401">
Cheers!!!
```

---
## \#2 Posted by: scepterr Posted at: 2017-11-06T17:19:15.560Z Reads: 77

```
This kind of thing has been discussed before, search for the other topics. There are a lot of hurdles to doing this
```

---
