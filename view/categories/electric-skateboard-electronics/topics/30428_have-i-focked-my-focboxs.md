# Have I focked my FOCBOXs?

### Replies: 26 Views: 2381

## \#1 Posted by: DanSkates Posted at: 2017-08-12T12:15:21.856Z Reads: 286

```
Hi folks,

I hate to post another 'why do my VESCs not work' post, but I was really just after some confirmation and maybe a clue as to wether or not they are toast or can be fixed.  I've read posts extensively but can't find anything to match.

**Scenario:**
I finally got my eMTB spinning yesterday (see post [here](https://www.electric-skateboard.builders/t/e-mtb-build-would-this-trampa-foundation-work-and-the-future-of-e-mtb/21343/56)) and couldn't wait to take it for a ride today.  In my haste I took it out pretty much just with the batteries and wires held down with tape and only intended to take it round the block but got carried away and hit a few speed bumps, pulled a few spins, etc!  Anyways, on the way back I only had half power and when I got home I realised that only wheel was spinning.  On inspection I noticed that one of the XT60 connectors into the FOCBOX had come out so without thinking I just plugged it back in.  This created a small spark (more of a subtle pop) and then I realised that I hadn't unplugged the loop key to make the connection.  I tried the remote and had no power.  Unplugged the loop key, plugged it back in but the FOCBOXes didn't light up :fearful:

Since then I've tried all the tests I can think of; plugging one of the FBs into my esk8 setup, wiring up a smaller battery, plugging into BLDC with different power supplies (6s, 12s) and trying to detect.  Both FBs seem to be completely dead.  I've taken their clothes off and there is no obvious damage I can see:

<img src="/uploads/db1493/original/3X/8/7/87fcf8b5fb6de1f1b96acf9613fa6aa34d4ea5d2.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/f/5/f59a2c8339cee5862e9281ee701b1d5614d664db.JPG" width="666" height="500">

Did I create a short and kill them?  Is there a way to fix them or anyone I can send them to?  I'm in Oz btw.

Any help would be gratefully received as I finally got to ride it today and it was absolutely bloody magical!

Thanks,

Dan
```

---
## \#2 Posted by: Blasto Posted at: 2017-08-12T13:39:58.484Z Reads: 266

```
You blew the CAN tranceiver on both of them. This happens when one of them is not grounded anymore and still connected via CAN.

The fix here is replacing U401 on both units.
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-08-12T13:42:26.744Z Reads: 262

```
Could he simply pair them with a servo Y cable to bypass the canbus?
```

---
## \#4 Posted by: L3chef Posted at: 2017-08-12T13:47:09.154Z Reads: 257

```
That's what I did on my dual 4.12 vesc. Removed can transciever and split y servo. 
Best would be to send them in for repair
```

---
## \#5 Posted by: DanSkates Posted at: 2017-08-12T13:49:51.802Z Reads: 253

```
Thanks for the info @Blasto - so would this prevent them from turning on at all?  I'm currently getting nothing from them - no LEDs or anything and BLDC can't detect them?

@L3chef any ideas who might be able to repair them?  I'm in Oz but happy to post...
```

---
## \#6 Posted by: lowGuido Posted at: 2017-08-12T13:50:49.389Z Reads: 253

```
[quote="DanSkates, post:1, topic:30428"]
couldn't wait to take it for a ride today.  In my haste I took it out pretty much just with the batteries and wires held down with tape
[/quote]

Im pretty sure 80% of eskate failures stem from this excitement to get going prematurely.

on the flipside, this seems like a pretty fragile flaw, especially when most people are running dual..
[quote="Blasto, post:2, topic:30428"]
This happens when one of them is not grounded anymore and still connected via CAN.
[/quote]
 there should be like a failsafe ground connection between the two or something if this is a known thing..

all the more reason to:
solder all the things!
https://www.electric-skateboard.builders/uploads/db1493/original/2X/7/7c2b8b63aea0ccd4bb8a7d03af06eb487aab32f6.jpg
```

---
## \#7 Posted by: DanSkates Posted at: 2017-08-12T13:54:15.722Z Reads: 233

```
[quote="lowGuido, post:6, topic:30428"]
Im pretty sure 80% of eskate failures stem from this excitement to get going prematurely.
[/quote]

Yeah I reckon you'd be spot on there.  I knew I shouldn't be going out too with things not properly secured but I just couldn't help myself!!  And I was literally gonna go up the road and turn around but one thing led to another... :blush:  Ha...now I'm paying the price!!  :confounded:
```

---
## \#8 Posted by: Blasto Posted at: 2017-08-12T13:55:31.252Z Reads: 226

```
[quote="lowGuido, post:6, topic:30428"]
there should be like a failsafe ground connection between the two or something if this is a known thing.
[/quote]

That would create a ground loop having a third wire as gnd... never tried tbh

If it's any consolation, this would have happened w any vesc. 

Talk to @JohnnyMeduse for repair
```

---
## \#9 Posted by: DanSkates Posted at: 2017-08-12T13:58:30.635Z Reads: 219

```
[quote="Blasto, post:8, topic:30428"]
Talk to @JohnnyMeduse for repair
[/quote]

Ok - cheers @Blasto

@JohnnyMeduse does this sound like something you'd be able to fix?  

Appreciate all the help guys - I feel like such a dick!
```

---
## \#11 Posted by: L3chef Posted at: 2017-08-12T14:02:09.953Z Reads: 208

```
The wizard who already is mentioned in this thread. Second option is to buy the parts yourself and solder them.
```

---
## \#12 Posted by: DanSkates Posted at: 2017-08-12T14:05:48.146Z Reads: 210

```
Lol, I'd love to say I'd give this a go but with my track record of things going bang I might leave this to a pro :wink: plus - I can hardly see half the chips on the board!


.......out of morbid curiosity which chip is the U401?  Scanned the boards but I'm guessing it's not labelled as such?
```

---
## \#13 Posted by: Blasto Posted at: 2017-08-12T14:11:18.172Z Reads: 205

```
<img src="/uploads/db1493/original/3X/4/5/450c1d4d34ae5fe9a30ebbf676e9578245b51609.PNG" width="640" height="480">

The guy that is circled
```

---
## \#14 Posted by: DanSkates Posted at: 2017-08-12T14:13:21.258Z Reads: 204

```
Aha...interesting.  He's actually one of the bigger dudes there.  Are these chips easy to source?
```

---
## \#15 Posted by: Blasto Posted at: 2017-08-12T14:22:16.056Z Reads: 202

```
Yes fairly easy, the hard part is removing and installing the new one properly

Part number SN65HVD232DR
```

---
## \#16 Posted by: DanSkates Posted at: 2017-08-12T14:27:03.426Z Reads: 201

```
Thanks buddy - I'll look into it for sure - what's the worst that could happen?!!

<img src="/uploads/db1493/original/3X/3/3/33c660cd3255af874ee2e0a0dca00fec5d0d45fb.jpg" width="300" height="225">
```

---
## \#17 Posted by: CamBo Posted at: 2017-08-14T03:23:11.053Z Reads: 171

```
Is the ground you are talking about one of the CAN wires or something else?  I'm sorry for the stupid question, but this seems like something I could screw up.  Thanks Blasto.
```

---
## \#18 Posted by: Blasto Posted at: 2017-08-14T03:27:13.080Z Reads: 172

```
Yes the CAN bus connector has 4 pins, 5V, CAN H, CAN L and gnd. But we are only using CAN H and CAN L at the moment.

I haven't tried connecting the gnd wire also, so i don't recommend doing it at the moment before it is properly tested
```

---
## \#19 Posted by: DanSkates Posted at: 2017-08-18T13:10:42.596Z Reads: 155

```
[quote="Blasto, post:15, topic:30428"]
Part number SN65HVD232DR
[/quote]

So I'm really toying with the idea of trying to unsolder/solder these chips myself.  @JohnnyMeduse offers a fair price for repairing VESCs but the postage to the US and back is a killer so I want to at least explore the idea.  After all - this is a DIY forum! :wink:

I've had a look for the chips and I can find stacks of VP232 (keyword searching: SN65HVD232DR) but the chips themselves all seem to have different numbers/characters on the chip.  Can anyone tell me what the '62M' AHEC on the chip refers to?  Do I need to match this or just ensure the 'M' is within a similar range?

This is the closest I can find [here](https://www.aliexpress.com/item/1pcs-SN65HVD232DR-SN65HVD232D-VP232-SOP8/32824890626.html?spm=2114.search0104.3.66.BtZdw2&ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10130_10068_10309_5400013_10307_10137_10060_10131_10155_10132_10133_10154_10056_10055_10054_5370013_10059_100031_10099_5380013_10103_10102_5410013_5430013_10052_10053_10107_10050_10142_10051_10326_10084_10083_10080_10082_10081_10110_5390013_10175_10111_10112_10113_10114_10312_10313_10314_10315_10078_10079_10073_5420013,searchweb201603_18,ppcSwitch_4&btsid=62a1158e-c93d-4698-b1a6-888bf523ce0b&algo_expid=93d1cdfe-badd-4688-bfa3-d0d9b785f22e-9&algo_pvid=93d1cdfe-badd-4688-bfa3-d0d9b785f22e) at 66M 

Or this which has a more apt description:
http://www.ebay.com.au/itm/2pcs-SN65HVD232DR-Texas-Instruments-CAN-Interface-IC-3-3-V-CAN-TRANSCEIVER-/262440960393?hash=item3d1ab34189:g:n64AAOSwVcFXOoC6

Or is all of this a red herring and will any SN65HVD232DR or VP232 work? 

Thank you 

Dan
```

---
## \#20 Posted by: DanSkates Posted at: 2017-08-21T13:03:05.232Z Reads: 140

```
Thank you to all the guys who contributed on this thread - I've managed to remove the fried can bus chips and the FOCBOXs have sprung back to life!!  Gonna use a split ppm cable now rather than can bus so I'll be back on the road!!  Still not sure if vescs are right for my build but I'll secure them properly this time and do some proper testing.

<img src="/uploads/db1493/original/3X/8/d/8dd330774fc4ae8e025a06cd34f628e40a26cbb0.jpg" width="322" height="500">
```

---
## \#21 Posted by: trancejunkiexxl Posted at: 2017-08-21T14:31:02.974Z Reads: 131

```
tat is sick brohan, good job on the mcguyver!
```

---
## \#22 Posted by: pakue Posted at: 2017-08-21T14:32:03.701Z Reads: 127

```
As far as I can tell SN65HVD232 CAN bus chip isn't an isolated version meaning it needs the same ground reference between the VESCs (even trough in theory a differential transmission protocol should handle that). The thing I'm not sure about is what happens once a ground shift occurs (e.g. due to higher current draw on one VESC) If it still fries something on the board.
```

---
## \#23 Posted by: longhairedboy Posted at: 2017-08-21T16:49:45.377Z Reads: 119

```
if i understand something i heard recently correctly.. and somebody please correct me if i'm wrong... 

yeah you can fry it that way. 

if somebody else would like to confirm that it would make me happy.
```

---
## \#24 Posted by: Alanhunt123 Posted at: 2017-08-24T04:11:42.468Z Reads: 111

```
Oh no! I just did the same thing with my Esk8 with FOCBOXs...

Looks like I'll be doing some repair work. Shouldn't be too hard, since I'm pretty good with soldering, and have a nice small chisel tip to use for the pins.

Argh, can't believe after getting my first dual working that I fried both of my new boards! Looks like I'm going with split ppm from now on... CANBUS serves me no benefits.
```

---
## \#25 Posted by: DanSkates Posted at: 2017-08-24T04:17:56.976Z Reads: 114

```
Ah crap - sorry to hear that welcome to the castrated CAN bus chip club!!  

Yeah I have fairly rubbish soldering skills and no chisle tip and still managed an ok job so you should be fine!!  :wink:  That said I butchered the chips by chopping the legs off first (as they were dead anyway) and then tidied up the pcb after.

Good luck!
```

---
## \#26 Posted by: Alanhunt123 Posted at: 2017-08-24T04:20:23.038Z Reads: 113

```
Thanks,

The board needs an overhaul anyways. It's my 8 wheel setup, which needs a new deck so the motors don't rub. Guess this will keep me off of it so I can actually focus on building it right!

That said, I do wish there was a warning on the device that says not to plug in canbus if only one ESC is plugged in...
```

---
## \#27 Posted by: Alanhunt123 Posted at: 2017-08-30T20:43:53.704Z Reads: 96

```
Just finished soldering on the new CANBUS chips. Big success! The FBs are back in action!

It wasn't a terrifically difficult job, but I do recommend using as small an iron tip as possible, and using a magnifying glass. Even better if you have a set of binocular magnifiers.

Cheers!
```

---
