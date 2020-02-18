# Broken Boosted Board

### Replies: 89 Views: 5708

## \#1 Posted by: Sebious Posted at: 2017-07-11T07:54:15.361Z Reads: 507

```
Hi,

I have a Boosted Board that had an issue with the battery, someone suggest me to tear down the board and put a new battery I success to dissassembly the board but it seems that the BMS not working anymore (Not sure) I can try to put new cells 12s1p for around 350 euros but I don't want to take the risk if the BMS is broken. So I don't know if someone can help me out or give me advice.
There is a possibility to know if my BMS still working ?
Or if it is possible to keep the original remote original charger and put an VESC with new battery pack ?
I apologize if my English is not good I live in Europe.
```

---
## \#2 Posted by: willpark16 Posted at: 2017-07-11T08:27:18.973Z Reads: 468

```
I think it will be hard unless u don't mind voiding your warranty but rn I recommend sending it back to boosted for repair
```

---
## \#3 Posted by: Sebious Posted at: 2017-07-11T08:42:46.642Z Reads: 452

```
I already voiding my warranty because the board is dissamble right now, if you want to know the full story I did ask boosted board for a repair but they told me that the board was not suppose to Europe market so it will cost me 600 dollars for battery plus shipping.
```

---
## \#4 Posted by: aigenic Posted at: 2017-07-11T09:45:29.110Z Reads: 436

```
Ok, tell us the whole story how did the battery died., can you charge it? 
where are you from?
Do you have multi meter to measure the voltage of the battery?
```

---
## \#5 Posted by: aigenic Posted at: 2017-07-11T09:46:29.513Z Reads: 414

```
You might keep the ESC if it is OK...
```

---
## \#6 Posted by: Sebious Posted at: 2017-07-11T10:13:14.669Z Reads: 398

```
I'm from France the whole story is that the board was working before but can do only 2 kilometers after that the board was stock for month and then when I try to use it again the battery did not work anymore but the led from the BMS was still working,someone suggest me to dissassemble the battery but boosted put a lot of glue and it was really hard to do if you don't want to break the original cover.
But after pull out the battery from the board the BMS did not working maybe because the cells are disconnect and when I put a charger on the bms there is not lights so don't really know if the BMS still working.
But I think the ESC is working the board is pretty new that's why I want to keep it.
I have a multi meter.
I will post some photo of the board maybe it help
```

---
## \#7 Posted by: aigenic Posted at: 2017-07-11T10:14:38.808Z Reads: 369

```
Ok, if you have acess to the batteries, try mesuring each cell and post the voltage of them...yeah photos would be nice :slight_smile:
```

---
## \#8 Posted by: aigenic Posted at: 2017-07-11T10:19:21.706Z Reads: 352

```
It sound like over discharged batteries...
```

---
## \#9 Posted by: Sebious Posted at: 2017-07-11T10:48:30.752Z Reads: 360

```
<img src="/uploads/db1493/original/3X/e/d/edcf2f1e29b85821966b3bc84fee8234edd71d84.png" width="375" height="500"><img src="/uploads/db1493/original/3X/f/2/f20ff02e5aad016f62759273f22cb8ac41a59b2c.png" width="375" height="500">

I already did a mesuring and if I remember correctly only half of the battery have 2.7V the other one was 0V
```

---
## \#10 Posted by: aigenic Posted at: 2017-07-11T11:10:48.405Z Reads: 352

```
What do you mean by the half? that half of the cells (6) are 0V and 6 are 2.7V?
```

---
## \#11 Posted by: Sebious Posted at: 2017-07-11T11:19:57.500Z Reads: 341

```
Exactly the left side or right side 6 cells was 0v and the other half 6 cells was 2.7v
```

---
## \#12 Posted by: aigenic Posted at: 2017-07-11T12:08:15.256Z Reads: 341

```
Measure it once more to make sure, if it is same it looks like you have 6 dead cells...its kinda weird that they are all on the same side, my personal opinion is, that you will have to replace whole battery pack...but I am not experienced with BMS and batteries, maybe somone more experienced will help you :)
```

---
## \#13 Posted by: Sebious Posted at: 2017-07-11T12:18:54.198Z Reads: 328

```
Replace the whole battery is not a problem for me but how I can be sure that the BMS is still working. I don't really want to put hundred bucks if my BMS is dead
```

---
## \#14 Posted by: Sebious Posted at: 2017-07-11T12:22:02.079Z Reads: 320

```
Also if the BMS is dead do you think I can still use the same remote and ESC - Motor and take another BMS.
I have many electric boards (not DIY)  but if I can make an DIY Boosted board it will be great
```

---
## \#15 Posted by: aigenic Posted at: 2017-07-11T12:58:05.125Z Reads: 309

```
Yes, you can for sure keep your ESC if you will use the same voltage...
10S LiPo or LiIon should be ok (used for external battery packs)...

I would swap the BMS, new BMS costs like 30$ if you buy small one just for charging :)
```

---
## \#16 Posted by: aigenic Posted at: 2017-07-11T12:58:31.208Z Reads: 300

```
But befor you do anything, w8 for somone more experienced to give you advice...
```

---
## \#17 Posted by: Jammeslu Posted at: 2017-07-11T15:09:53.586Z Reads: 292

```
Some others with board on yt har the same problem and they made it work på ”jumpstarting” just drive the board without elektricity and it Will charge up
```

---
## \#18 Posted by: NAF Posted at: 2017-07-11T15:17:54.251Z Reads: 291

```
Just send your orignal battery to @barajabali and I am sure he will make you proper pack  :slight_smile:
```

---
## \#19 Posted by: Pantologist Posted at: 2017-07-11T15:29:44.577Z Reads: 296

```
[quote="Sebious, post:1, topic:27318"]
There is a possibility to know if my BMS still working ?
[/quote]

Even without working batteries, connecting the charger should produce a warning light of some sort

[quote="Sebious, post:1, topic:27318"]
Or if it is possible to keep the original remote original charger and put an VESC with new battery pack?
I apologize if my English is not good I live in Europe.
[/quote]

Original remote will require a bit of work considering it is a properties Bluetooth remote. Might be easier to put in a Bluetooth Arduino setup to communicate

You are definitely checking the voltage incorrectly unless something shorted between cells, which I highly doubt. Check voltage across B+ and B- on the BMS.
```

---
## \#20 Posted by: Sebious Posted at: 2017-07-11T18:06:47.718Z Reads: 280

```
I don't have any warning I think my BMS is fucked up

Also I did check the voltage across B+ and B- and it show 0 volt.

Actually I don't really know what to do with the board hope I will find a way to fix it and keep the original ESC

But it's good to know that there is more than one solution
```

---
## \#21 Posted by: Sebious Posted at: 2017-07-11T18:07:28.105Z Reads: 240

```
I will PM barajabali but I live in Europe hope he can help me
```

---
## \#22 Posted by: Pantologist Posted at: 2017-07-11T18:11:49.023Z Reads: 239

```
If the BMS does not work, the ESC will not either. They have to have a communication between them for the ESC to function. 

0V is not normal. There should be some voltage between those two points. Try measuring each individual cell by putting one probe on ground B- and then on each cell + pad(C1, C2 etc)
```

---
## \#23 Posted by: IsTalo Posted at: 2017-07-11T18:23:18.557Z Reads: 238

```
[quote="NAF, post:18, topic:27318"]
Just send your orignal battery to @barajabali
[/quote]

He can't ship overseas, just US
```

---
## \#24 Posted by: IsTalo Posted at: 2017-07-11T18:26:17.306Z Reads: 236

```
Hi, I saw your post and had an Idea, maybe you can buy a Extended Battery Pack from Boosted, if you can't, buy a battery pack from a local (EU) esk8 shop, I now that Alien sells packs with Bms, but do not know if their pack have a good BMS.
```

---
## \#25 Posted by: Sebious Posted at: 2017-07-11T18:34:08.644Z Reads: 235

```
So if I can't make my BMS working the esc will be also fucked up, and if barajabali can't do overseas I have no choice to do it myself or find battery pack with bms + 2 vesc ?

I will try to measuring each cell again don't have my multi meter right now but I will do it ASAP.

Also I see that @raphaelchang have done an internship in Boosted Board and have done is own ESC and BMS do you think he can help me ?
```

---
## \#26 Posted by: aigenic Posted at: 2017-07-11T19:42:46.785Z Reads: 228

```
@Pantologist  Are you sure that you cant use ESC with different BMS? SOme guys use the external battery packs on BB without any BMS without problem...

I am not a pro, it just doesnt make sense to me...explain it pls :)
```

---
## \#27 Posted by: Lawndart Posted at: 2017-07-11T19:46:34.210Z Reads: 219

```
You must be getting some of that world class customer service boost is known for?  What I always hear is to that Boost boards have a short range, crap top speed, but the best customer service...
```

---
## \#28 Posted by: Pantologist Posted at: 2017-07-11T19:49:05.040Z Reads: 220

```
I'm sure there is nothing really he can directly help with. It is proprietary software/hardware that communicates with each other.
```

---
## \#29 Posted by: Sebious Posted at: 2017-07-12T10:39:46.110Z Reads: 213

```
As I said even if Boosted board have the best customer service they do not help european customer because they do not sell boosted board v1 overseas

Also someone know if the BMS of the v2 battery pack is the same as the v1 because if it is the same I can try to put an v2 battery that can be sell seperatly ???
```

---
## \#30 Posted by: pat.speed Posted at: 2017-07-12T11:40:51.331Z Reads: 196

```
Hey mate. I have a idea I saw this same thing happen to Casey. What he did was get his mate to drive is car around with a rope and him on the board for about half an hour. I think it used the regen braking to recharge the cells and it seemed to work again. You could try this but no guarantee. Worth a try tho🙂
```

---
## \#31 Posted by: Sebious Posted at: 2017-07-12T12:03:32.049Z Reads: 194

```
There is a lot of people who telling me that but I have two boosted board and I did it to my other one who have a battery problem before and now it work like a charm but when I had try with this one it did not work also you may need to have a BMS working ?
```

---
## \#32 Posted by: pat.speed Posted at: 2017-07-12T12:04:49.127Z Reads: 189

```
I am not sure I'm not very experienced with the boosted board
```

---
## \#33 Posted by: Pantologist Posted at: 2017-07-12T17:38:16.784Z Reads: 195

```
[quote="Sebious, post:29, topic:27318"]
Also someone know if the BMS of the v2 battery pack is the same as the v1 because if it is the same I can try to put an v2 battery that can be sell seperatly ???
[/quote]

Nope, you cannot connect a V2 battery to a V1 ESC. They are not compatible.
```

---
## \#35 Posted by: Sebious Posted at: 2017-07-18T20:58:00.932Z Reads: 187

```
So I check the voltage between B+ and B- and I got 8,46 Volt as I said 6 cells are 0 volt and the other 6 cells have 1.1V.
```

---
## \#36 Posted by: Martinsp Posted at: 2017-07-18T21:15:16.199Z Reads: 194

```
Well as far as i know boosted board has the BMS and ESC as separate units... meaning that they dont "talk" to each other so you should be fine changing the batteries with another BMS... BMS is not expensive at all copared to batteries..

BTW are you masuring at the batteries directly or on some cable coming from them? because if on cable it might have just disconnected somewhere due to vibrations and so on
```

---
## \#37 Posted by: Pantologist Posted at: 2017-07-18T21:20:12.392Z Reads: 192

```
There is communication between the two. There are both power connections and data connections between the two. Check out a tear down video. Fairly easy to spot. I should have a tear down video coming soon as well.
```

---
## \#38 Posted by: Martinsp Posted at: 2017-07-18T21:21:38.182Z Reads: 192

```
Oh sorry my bad.. didn know for sure. I thought that there are only like 4 wires for power
```

---
## \#39 Posted by: Pantologist Posted at: 2017-07-18T21:31:38.754Z Reads: 195

```
Definitely 4 wires. A positive, negative and some kind of communication line with an additional two wires.
```

---
## \#40 Posted by: Sebious Posted at: 2017-07-18T21:55:26.167Z Reads: 190

```
Do you have an idea if I have only half cells that working the bms should power on right ?
```

---
## \#41 Posted by: Pantologist Posted at: 2017-07-18T22:24:51.920Z Reads: 189

```
When you plug in a working charger, the BMS should turn on. Sounds like a damaged BMS. I currently have a board with an apparently damaged BMS. I will open it up in to check it out but I am pretty sure that is the easiest way to check if the BMS still functions.

I am planning on just removing the electronics and maybe replace the motor and just put DIY components in mine. You might be able to do the same. You will need a new battery pack either way.
```

---
## \#42 Posted by: Sebious Posted at: 2017-07-19T06:34:23.890Z Reads: 170

```
Also I forget to tell that I have two cable that have been cut off when I was trying to remove the battery this is the two cable going to the esc I think (a small red and black wire) maybe the BMS can not work without these two cable ?
```

---
## \#43 Posted by: aigenic Posted at: 2017-07-19T12:09:27.367Z Reads: 171

```
Try soldering them together again :) and the isolate them so they wont short :) 
If you measure 8.46V, how can 6 cells be 1.1V?! It would be 6.6V together...Something is wrong :/ Try again :)
```

---
## \#44 Posted by: Sebious Posted at: 2017-07-19T16:22:27.042Z Reads: 167

```
Yes you right maybe I missed 1 cell I will measure my cells again this week and try to soldering the two cable
```

---
## \#45 Posted by: Pantologist Posted at: 2017-07-19T16:55:56.071Z Reads: 168

```
No matter. The voltage is way too low. The cells were damaged one way or another.
```

---
## \#46 Posted by: Pantologist Posted at: 2017-07-20T03:43:47.467Z Reads: 158

```
Is there a special way to open the battery pack up. I am trying to open mine but the glue is mad strong. @Sebious
```

---
## \#47 Posted by: Sebious Posted at: 2017-07-20T06:37:14.334Z Reads: 154

```
You need to use an heat gun and put some strengh but be careful or you will broke the BMS
```

---
## \#48 Posted by: Pantologist Posted at: 2017-07-21T01:09:23.356Z Reads: 150

```
Heat around the bottom lid that holds the batteries?

I've been prying for and hour now. This stuff is sticky af.

EDIT: A Hammer worked.
```

---
## \#49 Posted by: Sebious Posted at: 2017-07-21T06:41:19.769Z Reads: 142

```
You need to be patient if you heat the bottom lid it take me an hour to do it but I don't know how you did it with an hammer lol
```

---
## \#50 Posted by: Pantologist Posted at: 2017-07-21T12:47:07.794Z Reads: 143

```
I used heat to pry the bottom lid enough to get my multimeter probes in to make sure the cells were dead. Literally 0V. That's when I got the hammer out. 

Prying from the top pointed edge with my hammer gave me enough leverage to just get the entire battery out.
```

---
## \#51 Posted by: deucesdown Posted at: 2017-07-21T16:19:47.514Z Reads: 151

```
didn't read everything, but these A123 are very tough. I have a 12s2p pack, that I managed to drain to about 1.5v (for the whole 12s). Hobby chargers wouldn't touch it. :( but I read multiple accounts of people reviving these cells. My pack is built so I can split into 6s1p subpacks.

I connected a 6s1p section to a lab PSU, about 18v current limited at 0.5a. 18v/12 = 3v. Kept an eye on the voltage and temperature, let it come up to 18v, took a few hours. repeated for all 4 subpacks. They more or less held near 18v after taking them off. Put them on the hobby charger, and voila, back in business, maybe lost 10-15% of their capacity but they're running great.

sooo, if the cells have not been previously badly abused and have not vented or anything like that, I think if you get about 2.5v at each cell, the BMS may decide it's safe to charge again.

You could maybe get a psu and put about 30v at 0.5a at b+ and b-, perhaps desoldering the BMS connection first. it'll take many hours to come up to 30v. If you're worried the cells have been damaged, it'll be good to check voltage at each cell fairly often at first. Unbalanced series charging with some toasted cells mixed in can be dangerous even with A123.

If the BMS is broken and draining the cells down, you still have a shot at salvaging the cells.
```

---
## \#52 Posted by: Sebious Posted at: 2017-07-21T19:54:34.293Z Reads: 138

```
It look complicated I think I will try to replace all my A123 and if it don't work I will take these cells to do an DIY project
```

---
## \#53 Posted by: pat.speed Posted at: 2017-07-21T21:46:00.522Z Reads: 138

```
Dude just give it a go it could save you heaps of money. All you need to do is connect a 30v-32v power supply to the battery leads and your done maybe just cut off or desolder the negative lead going the the bms. That's it you could possibly save these cells
```

---
## \#54 Posted by: deucesdown Posted at: 2017-07-28T22:04:57.379Z Reads: 147

```
It's not complicated. Get something like this:

http://www.ebay.com/itm/Lab-DC-Variable-Power-Supply-Precision-Digital-5A-30V-DC-Adjustable-PSU-110V-/282430250339?epid=899576533&hash=item41c2279d63:g:PuYAAOSww3tY7aYl

follow instructions to make sure you're in current limiting mode at around 30v (usually this involves turning knobs to minimum, shorting the leads, then raising the knobs slowly). set the current limit low, like 0.5A. This is for safety, so nothing happens too quickly.

Hook it up to the pack where you can watch it. When you hook it up the voltage will drop to close to zero, and current will be at what you set. Voltage will come up very slowly over many hours. If you have the case ripped off, check cell voltages from time to time to make sure they're not too far apart. A small spread should be fixable by the BMS. A large spread, like 1v, stop and come up with a new plan. Also make sure things are not getting hot.

Once the voltage hits whatever you had set it to (the current should start dropping at this point), remove PSU, hook up bms and see if it'll charge.

One of the good things about A123, it's very unlikely to actually shoot flames. Maybe just some poison gas. :slight_smile:
```

---
## \#55 Posted by: wafflejock Posted at: 2017-07-29T01:57:13.007Z Reads: 143

```
mmm poison gas

https://i.ytimg.com/vi/V59gAU6XhzY/hqdefault.jpg

I've got a similar one of those power supplies wasn't sure if I really needed it when I got it but has been really helpful with getting random voltage for little ICs I play with.
```

---
## \#56 Posted by: JTAG Posted at: 2017-07-29T02:19:34.790Z Reads: 134

```
This all sounds like the BMS killed the battery pack :sweat_smile:.
```

---
## \#57 Posted by: deucesdown Posted at: 2017-07-30T16:27:24.142Z Reads: 133

```
It's like UPS, eh? I get more outages from running small UPSes than from power going out.
```

---
## \#58 Posted by: barajabali Posted at: 2017-08-03T22:22:14.673Z Reads: 134

```
I'd buy it from you. Would you be interested in that?
@Sebious
```

---
## \#59 Posted by: Detonatedfrost Posted at: 2017-11-24T19:34:36.874Z Reads: 127

```
I have a boosted v1 with dead battery on its way from Ebay seller...  Just seeing here that its not 18650’s.😒..  Has anyone successfully replaced the a123 cells using original BMS..  seems like the cells are readily available.  Any tips?
```

---
## \#60 Posted by: aigenic Posted at: 2017-11-24T20:16:41.430Z Reads: 123

```
1. you will have to change BMS, remote, reciever and ESC, because the boosted bms and esc are connected somehow...
2. You can use 18650 cells, if the 26650 A123 cookies are not working...
3. How much did you pay for it?
```

---
## \#61 Posted by: pat.speed Posted at: 2017-11-24T21:14:57.928Z Reads: 119

```
You can get the same cells from nkon. Then just put them into the same configuration and your all set. I would possibly add some more in parallel to give you some more range
```

---
## \#62 Posted by: Detonatedfrost Posted at: 2017-11-25T01:44:56.363Z Reads: 114

```
I got it for $305 no remote no charger.  Just ordered both from boosted.

I want the boosted control system above all its the biggest mostest reason for acuiring the board so..  I plan to replace with same cells.
```

---
## \#63 Posted by: Detonatedfrost Posted at: 2017-11-25T01:53:44.883Z Reads: 117

```
Nkon..  thanks..👍
```

---
## \#64 Posted by: aigenic Posted at: 2017-11-25T07:47:06.791Z Reads: 115

```
If the battery is dead, then you try to revieve it, if you wont be sucessful, then you will have to change the cells and hope, that the BMS and ESC works...

This BB was probably stolen from somone...
```

---
## \#65 Posted by: Detonatedfrost Posted at: 2017-11-25T12:53:59.908Z Reads: 116

```
The ebay seller has good history but claims the board came out of a storage locker sale.  Seems a bit suspicious but I have no reason not to believe its the truth.  
  Is there a password to connect with the app?  Once I connect I’ll get some info and so will boosted.  IDK if they do but they could track stolen boards through the app when any one connects to it.
```

---
## \#66 Posted by: aigenic Posted at: 2017-11-25T13:04:51.078Z Reads: 113

```
IDK if boosted does so, IDK the app...as far as I know the only board with anti theft protection is Marble...but who would want to steal board like this one :D :D
```

---
## \#67 Posted by: Detonatedfrost Posted at: 2017-11-28T19:49:34.622Z Reads: 118

```
I got the ebay board.  Serial# checked out ok and the battery seems to be good.  I’ll have charger and remote Thursday.  Hopefully I get lucky and have a working board.  
Funny thing is its an early v1 with orange light instead of green.  I was concerned untill I figured out that was a thing...
```

---
## \#68 Posted by: Pantologist Posted at: 2017-11-30T19:45:23.524Z Reads: 113

```
If you bought the whole board you can replace the cells by assembling and spot welding a new pack. If the bms was not damaged you won't have an issue. Make sure to replace with the exact cells. Should be the B variant of the 26mm A123 cells.
```

---
## \#69 Posted by: Acido Posted at: 2017-11-30T19:53:53.648Z Reads: 112

```
What cells are you buying dude 350$ for 12cells is way too much you are getting ripped off 12cells is 60$ tops
```

---
## \#70 Posted by: Pantologist Posted at: 2017-11-30T21:05:21.803Z Reads: 107

```
He said he got the broken board for $305...
```

---
## \#71 Posted by: BoostedBuilder Posted at: 2017-11-30T21:14:14.048Z Reads: 107

```
[quote="Acido, post:69, topic:27318"]
12cells is 60$ tops
[/quote]

So you are able to find 12 genuine 20700A cells for under $60?
```

---
## \#72 Posted by: Pantologist Posted at: 2017-11-30T22:32:00.770Z Reads: 109

```
@Detonatedfrost

To get some replacement cells will cost about $120.

Not a bad deal at all over on [eBay](https://www.ebay.com/itm/A123-Systems-ANR26650M1B-High-Power-Lithium-Ion-Cells-New-With-specs-12ea/222711588863?epid=2255354793&hash=item33daa527ff:g:EVYAAOSwHHFY93PC)
```

---
## \#73 Posted by: Detonatedfrost Posted at: 2017-12-01T02:17:36.610Z Reads: 109

```
Board $305
Remote $100
Charger $79
Shipping $50
Total $534
Board works great. Put a few miles on it tonight.   I lucked out and batteries are fine..  Its an early V1 with an orange light instead of green..  They changed to green early on because it was confusing people.
```

---
## \#74 Posted by: Martinscce Posted at: 2018-03-17T08:53:31.145Z Reads: 104

```
Guys i destroyed my boosted board v1BMS... now i want to change the bms the esc and the remote with custom hardware. Is it possible to connect the remote from boosted with a custom vesc?
```

---
## \#75 Posted by: Martinsp Posted at: 2018-03-17T10:29:31.623Z Reads: 106

```
You definitely can replace the hardware but the remote may be a bit too difficult for what it is worth, maybe a clone with standard receiver would be a better option. Anyway, here is a thread you might want to check out 
http://www.electric-skateboard.builders/t/possible-to-mod-boosted-board-remote-to-use-for-diy-build/4680
```

---
## \#76 Posted by: baxter Posted at: 2018-03-17T10:52:07.027Z Reads: 103

```
You could get/build a firefly remote

https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543
```

---
## \#77 Posted by: aigenic Posted at: 2018-03-17T13:03:25.581Z Reads: 102

```
Just out of interest...do you have link to BB remote clone ? :) It is quite nice remote, I would consider it for my 2nd board :)
```

---
## \#78 Posted by: Martinsp Posted at: 2018-03-17T13:11:05.197Z Reads: 103

```
The link that baxter posted above is a clone. 
https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543 

It uses arduino so it may involve some tinkering to setup but it has a display which could maybe be adjusted to display whatever you want which is pretty cool... :D
```

---
## \#79 Posted by: aigenic Posted at: 2018-03-17T13:29:30.310Z Reads: 102

```
Yea, i know :) I just meant if you know about chineese clones, since there are some chineese boards with similar remote :) I dont have anything against the arduino based :) I might try that just as a challenge :)
```

---
## \#80 Posted by: Martinsp Posted at: 2018-03-17T13:31:33.326Z Reads: 103

```
Maybe this? [Winning remote](https://www.aliexpress.com/item/Wholesale-New-arrival-2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32678995218.html?spm=2114.search0104.3.64.43f166a5CMcZ75&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10151_10065_10344_10068_10342_10343_10340_10341_10696_10084_10083_10618_10307_10303_5711215_10313_10059_10534_100031_10103_10624_10623_443_10622_5711315_10621_10620_5722415,searchweb201603_25,ppcSwitch_5&algo_expid=fc9273f8-31f5-4fdf-b7a3-fee17d66e9ed-9&algo_pvid=fc9273f8-31f5-4fdf-b7a3-fee17d66e9ed&priceBeautifyAB=0)
```

---
## \#81 Posted by: aigenic Posted at: 2018-03-17T13:32:03.180Z Reads: 104

```
Nah, I know that, unreliable :D Unless you mod it a little bit :)
```

---
## \#82 Posted by: aigenic Posted at: 2018-03-17T13:34:21.276Z Reads: 108

```
Predator uses the same one :) Maybe @PredatorBoards could tell us where to get it :D But its probably secret, am I right? :D  
![image|500x500](upload://mDJ1m9fXfhp7TbxmTSxerjzW0Oe.jpg)

EDIT: They are bought from Winboard :) Still I am interested if it were possbile to buy just a piece somewhere :)
```

---
## \#83 Posted by: GrecoMan Posted at: 2018-03-17T14:11:50.438Z Reads: 100

```
they don’t have independent receivers. the receivers are soldered on to the custom escs.
```

---
## \#84 Posted by: PredatorBoards Posted at: 2018-03-17T18:32:00.803Z Reads: 94

```
Unfortunately this is the sad case. It's all proprietary stuff.
```

---
## \#85 Posted by: Martinscce Posted at: 2018-03-18T16:12:09.174Z Reads: 94

```
![image|375x500](upload://r30JWqv4ztygFMjzuVhBw8KRhs3.jpeg)can anyone tell me what this little cable are doing if i connect the baterie to te big cables the esc is working and i can connect the remote to the boosted board v1 but i cant start the motor. I think the old bms has send an singnal on a lower voltage. 

Thanks for help
```

---
## \#86 Posted by: Martinscce Posted at: 2018-03-18T16:20:02.750Z Reads: 93

```
![image|281x500](upload://d1q84FbPrQFb4yPyWQmClH1zP3x.jpg)here was the connection
```

---
## \#87 Posted by: aigenic Posted at: 2018-03-18T16:32:31.569Z Reads: 93

```
They make connection between ESC and BMS...this way they communicate together, which is also the reason, why you cant use ESC separably...

IDK why, boosted probably ensure that it cant by moded, it might have some advantages :)
```

---
## \#88 Posted by: TeckniX Posted at: 2018-05-17T14:54:17.317Z Reads: 83

```
@Martinscce did you figure out how to replicate the CAN h/l data for your board to work again?

For others, is there a range of voltage accepted by the esc? I’m guessing yes, since they take on the extended packs without issues.
```

---
## \#89 Posted by: Vin Posted at: 2019-04-15T11:26:11.051Z Reads: 34

```
Hi do you still have your BB V1 ESC if so would you be willing to sell it?
```

---
## \#90 Posted by: ryanza Posted at: 2019-04-27T19:16:12.299Z Reads: 26

```
I got the same problem 
iv tryd connecting diff voltages to those 2 small cables 
3v,12v even the full 40v from the batteries
.remote connects to the board but it indicated low battery 
and does not start the motors
```

---
