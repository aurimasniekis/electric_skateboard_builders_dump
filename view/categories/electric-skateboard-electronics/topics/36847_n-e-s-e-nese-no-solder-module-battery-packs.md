# N.E.S.E / NESE - No solder module battery packs

### Replies: 1104 Views: 33317

## \#1 Posted by: NAF Posted at: 2017-10-30T06:28:54.181Z Reads: 1543

```
Guys has anyone tried these ? Seems like finally someone got the solder less packs sorted out the right way.
I am super tempted to try these with 12s4p setup. 

https://www.youtube.com/watch?v=04lDZh19k64

Link to the store:
http://18650.lt/index.php/product/n-e-s-e-module/
```

---
## \#2 Posted by: NAF Posted at: 2017-10-30T06:34:30.332Z Reads: 1373

```
Vibration test:
https://www.youtube.com/watch?v=93JBo87LJiU
```

---
## \#3 Posted by: banjaxxed Posted at: 2017-10-30T06:41:47.251Z Reads: 1335

```
Saw those on electric sphere, they look pretty cool I was planning a build based on them
```

---
## \#4 Posted by: NAF Posted at: 2017-10-30T06:44:26.766Z Reads: 1337

```
Long term this saves shit load of money. The idea that you just pop in new cells every now and then is so cool. 
There is also VRUZEND very similar project but somehow i like this NESE pack design better. 

http://vruzend.com/
```

---
## \#5 Posted by: scepterr Posted at: 2017-10-30T07:23:27.681Z Reads: 1310

```
Space is the only issue I see
```

---
## \#6 Posted by: NAF Posted at: 2017-10-30T07:25:35.711Z Reads: 1293

```
why ? It says on their website it's 22mm in height.
```

---
## \#7 Posted by: willpark16 Posted at: 2017-10-30T07:25:59.368Z Reads: 1263

```
Agreed but the design is good, I could probably skim it down if justbnees to source the nickel strip that he's using
```

---
## \#8 Posted by: scepterr Posted at: 2017-10-30T07:26:08.067Z Reads: 1242

```
Right it's just bigger all around compared to bare cells
```

---
## \#9 Posted by: NAF Posted at: 2017-10-30T07:27:50.821Z Reads: 1212

```
To be more specific here are the exact dimensions : Size – 22x74x123mm 
To me it's super compact :slight_smile:
```

---
## \#10 Posted by: willpark16 Posted at: 2017-10-30T07:30:03.244Z Reads: 1195

```
It's designed to be stacked height wise though so it would have to be redesigned for esk8 also with nickel that can carry 20-80a
```

---
## \#11 Posted by: NAF Posted at: 2017-10-30T07:31:54.262Z Reads: 1179

```
We should invite this dude here on the forum.
```

---
## \#12 Posted by: rojitor Posted at: 2017-10-30T07:44:51.358Z Reads: 1168

```
The nice thing about those is that you can buy just the hardware and print the molds yourself. Cheaper and faster shipping and no customs.
The only downside is that you need a little more room. I tested vruzend and I found it an excellent solution. I am sure nese is awesome as well. Replacing cells looks easier to do with nese.
```

---
## \#13 Posted by: agniusm Posted at: 2017-10-30T08:17:43.222Z Reads: 1144

```
Hi guys. I was registered on this forum for some time now but i think i was confused a bit how this forum works :)
Anyhow, i appreciate you guys taking interest in my design.
Just as a note, modules could be stacked sideways as well which is what you want on the deck.
Also, my tabs are tin plated 0.6mm copper, not nickel. I had to abandon nickel plating as it was making copper brittle but tin is fine as i have tested these modules at 200+ amps in 6P configuration and at the moment there are no cells to push out that much current without getting damaged.
Any, questions, dont hesitate to ask, here to answer all of them.
```

---
## \#14 Posted by: NAF Posted at: 2017-10-30T08:30:43.182Z Reads: 1106

```
Hi @agniusm thanks for visiting us. You did an awesome job. Do sell those nice BALANCING CABLES as well ? I can't find them anywhere in the store. It would useful to buy them as well .
```

---
## \#15 Posted by: agniusm Posted at: 2017-10-30T08:38:44.437Z Reads: 1084

```
I was intending to have them made but nature of DIY stopped me cause different lengths are needed so if longer supplied someone who need short ones would not be happy overpaying for stuff they dont need. I could do some on personal request though ;)
```

---
## \#16 Posted by: pennyboard Posted at: 2017-10-30T09:23:50.576Z Reads: 1086

```
Have you considered a similar design but doing series packs instead of parallel? As in, instead of buying 4p or 6p modules, you buy 10s or 12s modules, and stack them in parallel to build the battery you want. 

The reasoning behind this would be adjustable battery size. That way you can run 10s3p for picking up groceries, riding to class, etc. but if you did a long 30+ mile ride, you could stick in 3 more packs in parallel for extended range. 

The idea is to only carry as many batteries as you need for the type of ride you're doing, and only deal with the heavy weight of extra batteries when necessary.
```

---
## \#18 Posted by: scepterr Posted at: 2017-10-30T09:25:45.536Z Reads: 1041

```
That would be complicated by a bms, either having to split one between all somehow or have a bms per module
```

---
## \#19 Posted by: pennyboard Posted at: 2017-10-30T09:27:55.170Z Reads: 1039

```
Yeah, true, I didn't really consider a BMS. I actually don't use a BMS, 9 months in and no problems so far.
```

---
## \#20 Posted by: agniusm Posted at: 2017-10-30T09:31:19.586Z Reads: 1026

```
If you would look at the batteries the rule is you parallel your cells and then series them. Imagine the web of wires doing the proposed way. 3P of 12 series stacks would equate to 39 wires for balancing and that webbing you have to incorporate in the design. It is a bad practice which was discussed extensively on endless sphere.
```

---
## \#21 Posted by: scepterr Posted at: 2017-10-30T09:33:21.120Z Reads: 1016

```
You could make the current design into series by just cutting and staggering the copper if you don't want to use bms
It's actually not a terrible idea considering you could take the cells out to charge in a balance charger
Having multiple xS1P modules precharged would eliminate downtime
```

---
## \#22 Posted by: pennyboard Posted at: 2017-10-30T09:33:23.144Z Reads: 937

```
Yeah, true, although that is assuming you balance charge your cells. Probably better for the batteries, but I wouldn't say it's absolutely necessary.
```

---
## \#23 Posted by: agniusm Posted at: 2017-10-30T09:37:26.829Z Reads: 916

```
These modules are designed to be used by masses and used properly meaning bms.... but, you can hack away and make it suitable for your applications and needs.
Balance charging is a pain in the ass
```

---
## \#24 Posted by: scepterr Posted at: 2017-10-30T09:38:23.496Z Reads: 907

```
Lol hacking away is the specialty around here
```

---
## \#25 Posted by: agniusm Posted at: 2017-10-30T11:17:07.632Z Reads: 903

```
Depending on size of the board there is little to no hacking required from my point of view. Depending on size of the battery modules could be stuck to underside with some quality double sided tape and stainless steel strap used to secure ir further. I probably could do a rendering of that if someone could point me to the right cad file of the board.
```

---
## \#26 Posted by: agniusm Posted at: 2017-10-30T11:28:27.237Z Reads: 885

```
BTW if these are tested to be suitable for your application, and there is significant demand  i could design and produce vacuum formed covers depending on size
```

---
## \#27 Posted by: briman05 Posted at: 2017-10-30T12:04:52.060Z Reads: 878

```
I would be interested in these if they could be connected long ways and flat. That way it would be like one custom built packs and would be the slimmest possible.
```

---
## \#28 Posted by: AgileCow Posted at: 2017-10-30T12:14:11.886Z Reads: 865

```
@agniusm do you have a picture with dimensions of the different sizes listed (including connection terminals at the top)?
```

---
## \#29 Posted by: banjaxxed Posted at: 2017-10-30T12:29:13.255Z Reads: 865

```
You can download the cell pack file and measure any dimension you like from his website in post #1
```

---
## \#30 Posted by: AgileCow Posted at: 2017-10-30T12:35:48.373Z Reads: 886

```
Hmm, I haven't looked at the file, but that will only include the casing, not the external connection terminal...?
```

---
## \#31 Posted by: agniusm Posted at: 2017-10-30T12:43:51.244Z Reads: 917

```
Here is a quick 36V 4P mock up on 1000mm longboard:

[img]https://i.imgur.com/FUzOV90.jpg[/img]

[img]https://i.imgur.com/MFcYqs0.jpg[/img]

Bolts ant tab adds 6.5mm so for 6P it would be 123+6.5=129.5mm total. If you need a rubber cap, then add 2mm or so on top
```

---
## \#32 Posted by: agniusm Posted at: 2017-10-30T12:56:48.773Z Reads: 887

```
Bolt dimensions could be found here: http://in.misumi-ec.com/asia/ItemDetail/10300240650.html

All fixings are quality stainless steel. Bolts are comming from Japan, plastic screws and square nuts  from Germany and the rest is made in Lithiania.

I will get series tab technical drawing made and upload to my website
```

---
## \#33 Posted by: agniusm Posted at: 2017-10-30T15:18:33.953Z Reads: 887

```
Series bus bar drawings added. See reference area on the website.
You can download stl models for assembled module with series bus bar and bolt and with series bus bar, bolt and protective cap here:
https://drive.google.com/open?id=0B56NVZIdTBFOd2RGNktnZE5QSE0
I understand that space on the board is tight and each .5mm counts. Take a look and do allow for printer tolerances.
```

---
## \#34 Posted by: briman05 Posted at: 2017-10-30T18:02:22.621Z Reads: 849

```
How would you make it a 10s build with 3p or 4p with only one module high.
```

---
## \#35 Posted by: agniusm Posted at: 2017-10-30T18:38:36.613Z Reads: 842

```
Have you seen my renderings? That one is 12S. Take off 2 modules and you have 10S
```

---
## \#36 Posted by: korryh Posted at: 2017-10-30T18:41:08.056Z Reads: 830

```
I saw the rendering as well, still dont know how they attach with connectors in that configuration.
```

---
## \#37 Posted by: agniusm Posted at: 2017-10-30T18:45:04.185Z Reads: 839

```
I am stuck at home with my kid being sick but i have parts here and i will make a small video on this. Words mean little so i hope i will make it clearer. Stay tuned
```

---
## \#38 Posted by: korryh Posted at: 2017-10-30T18:50:27.774Z Reads: 841

```
No worries, take your time.  I have 3 little petri dishes at home as well and they all get me sick at the same time.  I saw this awhile back when I was making my flexible trampa build and thought it would be a good solution - good to see how far you have come.
```

---
## \#39 Posted by: pennyboard Posted at: 2017-10-30T21:06:13.528Z Reads: 829

```
[quote="agniusm, post:23, topic:36847"]
Balance charging is a pain in the ass
[/quote]


Yes I agree, that's why I don't balance charge or use a bms. Much simpler and so far no problems.
```

---
## \#40 Posted by: agniusm Posted at: 2017-10-30T21:18:24.735Z Reads: 826

```
It only takes once to burn you with your skateboard alive while you are a sleep. Too many excamples to put a blind eye not to mention close ones that you are responsible for.
```

---
## \#41 Posted by: briman05 Posted at: 2017-10-30T23:50:58.173Z Reads: 817

```
These are interested but the shipping and customs would kill me
```

---
## \#42 Posted by: agniusm Posted at: 2017-10-31T11:45:00.523Z Reads: 757

```
Never had anyone complaining about customs and most of my customers are from US
```

---
## \#43 Posted by: longhairedboy Posted at: 2017-10-31T12:08:30.191Z Reads: 778

```
This is prefect for lots of things but not boards in my personal opinion. Yeah you could strap on a 12S4P pack that's almost the size of two 12S5P packs but i don't really see the advantage there other than swapping out individual cells or even P Groups when they die out for age which is kind of a bad practice anyway. 

I'd put these on a bike or in a fun cart. Power wheels, electric paddle boards maybe. I'd probably not put them on a skateboard. Anywhere i need cell protection and ease of maintenance but have no concern for space constraints. 

home power storage is also an ideal candidate for these.
```

---
## \#44 Posted by: Ronny_CTS Posted at: 2017-10-31T16:33:19.862Z Reads: 806

```
These seem like a good idea if you travel with your board on planes...just take the cells out in put them in the carry on bag. No welds, just batteries in their stock form. 

My only concerns are the fact that you need almost 1kg of filament to make a 10S4P pack so you are making you board heavier by 1kg. The other is how the connection between the tabs and the cell will hold up over time. Spot welding ensures a solid connection with high amp delivery. Will a pressure connection be able to do the same?
```

---
## \#45 Posted by: agniusm Posted at: 2017-10-31T17:26:46.337Z Reads: 829

```
longhairedboy, it might be larger, than glued pack, but you are missing the point. Not all can or have equipment to spotweld or solder. This allows least literate to still build a usable battery which will beat every spotwelded or soldered battery in power, hands down which equates to most efficient.

 Ronny_CTS,  1kg of filament prints 14 6P modules. 
The spring is made out of low density low compression set foam with certain deflection force. The low set means that after 10 years of compression, when released foam comes back to its thickness loosing about 5% so say 1mm foam after 10 years will become .95mm.
Spot welding will never deliver same amount of power NESE can, and here is why:
 Nickel is of lower conductivity than copper, check iacs table
 Welded nickel strip is usually up to 0.2mm thick where my tabs are 0.6mm.
 Spotwelding means that you have couple 1mm^2 spots of good connection where here precision stamped tabs have ten times that. 
Do a test, spot weld 6p and pull 200A and see what happens:)

Here is promissed video:
https://youtu.be/qCMFbMVe6_4
```

---
## \#46 Posted by: Jammeslu Posted at: 2017-10-31T18:22:09.284Z Reads: 794

```
How much can the buzzbars handle con?
```

---
## \#47 Posted by: agniusm Posted at: 2017-10-31T18:25:25.215Z Reads: 789

```
Not tested beyond 200A
```

---
## \#48 Posted by: smurf Posted at: 2017-10-31T18:53:40.557Z Reads: 793

```
I don't know if it would be too difficult to add a fuse on every cell. But ya that would be the ultimate! 

http://i.ebayimg.com/images/i/201079869468-0-1/s-l1000.jpg
```

---
## \#49 Posted by: longhairedboy Posted at: 2017-10-31T18:57:46.707Z Reads: 769

```
yeah. I get some flavor of that response a lot. I know that $150 is probably a crippling investment for some people for a spot welder but how much are we going to pay for 12 of these? Wil it be more than a $50 soldering station and a couple hours of youtube?
```

---
## \#50 Posted by: Henkow Posted at: 2017-10-31T19:04:41.649Z Reads: 748

```
For a larger battery such as 10s4p it seems cheaper to buy an arduino spot welder.

Ofcourse you don't get the benefit of modularity with a spot welded battery, but if you wan't to get away as cheap as possible it still seems like a better option.
```

---
## \#51 Posted by: longhairedboy Posted at: 2017-10-31T19:10:07.738Z Reads: 753

```
plus i guess you have to figure cost of nickel.. which is cheap on dollars but expensive on wait time. Then i suppose you have to learn how to use a welder without blowing holes in the cells. Or i suppose how to solder cells without destroying their cycle life.

ok maybe I am spoiled on experience.
```

---
## \#52 Posted by: NAF Posted at: 2017-10-31T19:11:12.929Z Reads: 732

```
[quote="longhairedboy, post:51, topic:36847"]
ok maybe I am spoiled on experience.
[/quote]

yes you are :slight_smile:
```

---
## \#53 Posted by: agniusm Posted at: 2017-10-31T19:12:32.968Z Reads: 736

```
It totally depends on you, what you want. I am not pushing my product and i would rather have people who have no appreciation for it leave it be. My point of view is biased, its my baby but then again,  i am in electric bikes for some 10 years and the only thing kept me of 18650 was the hassle. I even build my own spotwelder with dual pulses and pneumatic electrode clamping(have some tests on youtube, my channel).
I went from ordering packs spotwelded to doing it myself, ordering nickel strip, receiving nickel plated steel strip, dialing in pulse duration and power while damaging some good cells with electolite siphoning.
I was working on this design for three years, learning plastic properties, materials that might be suitable or not.
BTW those 150$ welders are a pile of crap. Good welders cost in exess of couple k's.
```

---
## \#54 Posted by: agniusm Posted at: 2017-10-31T19:18:14.427Z Reads: 725

```
Anyway, i am not here to tell the tale or explain my pricing. If it suits and you have questions i will answer them.
If its too big for application, there is no need for discutions, all specs are accessible to size it and see if it fitts the needs, if not, skip along.
There is too much debate going over nothing
```

---
## \#55 Posted by: Henkow Posted at: 2017-10-31T19:20:16.011Z Reads: 727

```
I didn't wan't to come off as negative. I can definitately see this being a viable option. I for instance will most likely move abroad next year for studies and the modularity your solution provides would solve the problem of getting the battery on an airplane.
```

---
## \#56 Posted by: longhairedboy Posted at: 2017-10-31T19:48:02.645Z Reads: 762

```
HA!

You're new here, aren't you? Just to crash course on the culture quickly: We debate nothing here on a regular basis and let me tell you, brother, we get a lot of nothing resolved. Why just the other day somebody posted something and a few of my colleagues and myself had almost nothing to offer, but we offered it anyway and wow was that nothing special. It was quite the spectacle. 

To further my point, i hand you over to Vice President Sharktopus to resume the considerations for your product. 

<img src="/uploads/db1493/original/3X/b/8/b886478816d5c53d9feb0a5a1747b08beaa29b63.png" width="640" height="480">
```

---
## \#57 Posted by: agniusm Posted at: 2017-10-31T19:49:28.824Z Reads: 734

```
Me neither :) Just dont want this to become a debate over size or price:)
Went through that
```

---
## \#58 Posted by: korryh Posted at: 2017-10-31T21:56:12.312Z Reads: 732

```
Thanks for the video.  Are you going to offer a similar compartment for dual/single VESC, BMS and remote receiver.  Would be cool if they all fit together.  Would still need a balance wire cover to have an all in one solution (just thinking out loud).

Nice Job!
```

---
## \#59 Posted by: michichopf Posted at: 2017-10-31T23:21:05.621Z Reads: 718

```
This is golden, haha
```

---
## \#60 Posted by: agniusm Posted at: 2017-11-01T07:24:00.457Z Reads: 718

```
Managing battery stuff alone is quiet some task so at the moment i have no time on full system. With tools available and lrimting services all arorround something could be designed by the community here. I dont have vesc or other hardware to even start.
```

---
## \#61 Posted by: OLnewB Posted at: 2017-11-03T02:16:24.934Z Reads: 709

```
@agniusm Awesome NESE modules! Do you have any recommendations for 18650 cells? Any that fit best and best discharge characteristics? Have you tried LifePO4 18650s?
```

---
## \#62 Posted by: b264 Posted at: 2017-11-03T02:20:27.511Z Reads: 686

```
[quote="agniusm, post:20, topic:36847, full:true"]
If you would look at the batteries the rule is you parallel your cells and then series them. Imagine the web of wires doing the proposed way. 3P of 12 series stacks would equate to 39 wires for balancing and that webbing you have to incorporate in the design. It is a bad practice which was discussed extensively on endless sphere.
[/quote]

How deep?  6P?  8P?  10P?  16P?  At some point, you need to start doing it a different way.  Do you have a link to that endless sphere discussion?  That place is hard to navigate :imp:

The web of 39 wires would allow every cell to be balanced as well... and if they were 30 gauge wires, they'd be as small as hairs... and also act as fuses if there was a short... just sayin'
```

---
## \#63 Posted by: agniusm Posted at: 2017-11-03T07:07:32.135Z Reads: 670

```
B264, 8P is as large as i will go. 8P already is on the limit i would like it to be. There are other solutions if you need something above that.
What you are saying regarding series then parallel has no technical background and will not get into that, if you want to research why, would be good start if you are or considering building batteries. To begin with, think what happens to those hair wires when soc of each series battery is not equal and power goes through that thin wire at full current?
```

---
## \#64 Posted by: agniusm Posted at: 2017-11-03T07:09:48.691Z Reads: 648

```
ALnewB, there are couple couple good cells out there from sony samsung and lg. All depends what you need, capacity, power and how much you want to spend.
```

---
## \#65 Posted by: agniusm Posted at: 2017-11-05T21:34:49.722Z Reads: 656

```
I think i found a BMS that i like. Its 10S 30A which would fit into NESE 6P case (might not be suitable for all as ot will add 123x74x22mm enclosure)
It has blutooth module and android app so you can set cell parameters and view state of the battery wireless.
```

---
## \#66 Posted by: b264 Posted at: 2017-11-05T21:39:13.375Z Reads: 662

```
[quote="agniusm, post:63, topic:36847"]
soc
[/quote]

What is soc?  Series operating current is a guess.  I was talking about using a thin wire for balance charging only, not discharging.  Hence the thinness, any use of it by accident for discharging would burn it up before something worse happened.
```

---
## \#67 Posted by: Acido Posted at: 2017-11-05T21:42:54.600Z Reads: 638

```
10s4p 30q is only 1kg
Also if you have a bms for discharge its not that fast
```

---
## \#68 Posted by: agniusm Posted at: 2017-11-06T05:37:13.163Z Reads: 643

```
Soc - state of charge.
Parallel cells equalize capacity. That means when you connect different s groups with different state of charge, cells in parallel will want to equalize and they will do that through that thin wire and it will go vaporized:)
```

---
## \#69 Posted by: NAF Posted at: 2017-11-06T08:46:32.117Z Reads: 662

```
@agniusm Are you talking about one of these bms's ? They look awesome. There are even 12s 60A options and even more. Are you going to sell these?  In two months I'll be building 12s 4p setup I definitely want to go with your setup. One of the biggest advantages that I like about your packs is that I can freely take them on any flight and noone is going to say anything. 

 <img src="/uploads/db1493/original/3X/2/d/2d0b17a1ae668f11d3d21d044a2fb904993a6a7c.png" width="222" height="142">
```

---
## \#70 Posted by: b264 Posted at: 2017-11-06T09:13:10.584Z Reads: 658

```
Oh no, that's not how I meant to connect them at all.  I mean each 1P group is connected to the bms via 30 gauge wire.  So, 1 cell total.  For example a 10S3P pack would have 27 30gauge wires and two 8gauge wires going to the BMS.  Not all connected to the same pad on the bms.  It'd have to be a bms that could balance charge all of them.  Most likely 3 separate BMSs
```

---
## \#71 Posted by: NAF Posted at: 2017-11-06T09:27:27.076Z Reads: 645

```
@agniusm Also one more question would you be able to adopt your design to 21700 in the future ?? When SAMSUNG will release Samsung 30T - with 40a discharge people will jump onto 21700 format. This will allow to make smaller lighter packs like 12s2p
```

---
## \#72 Posted by: agniusm Posted at: 2017-11-06T10:22:41.832Z Reads: 632

```
@b264.
 In that case i could not name worse solution than yours. Its as bad as it can get and beyond. Sorry, but i will not continue to push some sense into you :smile:  
You just made your system that meny times more unreliable; a lot bulkier and hevier; a lot more expensive;  
If  you think its a cleaver and beneficial approach, its not, its the most stupid one. Sorry, but i had to say it
```

---
## \#73 Posted by: agniusm Posted at: 2017-11-06T10:28:58.315Z Reads: 620

```
@NAF 
Thats not the one i was thinking about. 10s 30a is all i can fit and henze i will adopt it so batteries build with my kits have seamless design. They cost arround 60usd and i have yet not decided if i am going to sell them. Perhaps, just to save people from ordering stuff from multiple places.
I have the 21700 worked out but at the moment i have no intensions of making them. There is no point on small scale applications. It works out as less dence solution when you need only few of them and the price will still be higher. It is wise to use them In Tesla cause of so many of them tips the density scales towadrs it
```

---
## \#74 Posted by: agniusm Posted at: 2017-11-06T11:24:17.601Z Reads: 585

```
@NAF Just looked at that 30T cell and its worse than I thought. Its 3000mah cell at 35A. 2P volume comes out at 0.125l at 21wh and 70A discharge.
Now let's take Sony vtc5 3p which comes out at same 0.120l but at 33wh and 90A discharge. It will not replace 18650, far from it
```

---
## \#75 Posted by: NAF Posted at: 2017-11-06T11:35:08.626Z Reads: 602

```
@agniusm Your point is valid ...but if you look at Mooch tests - he rates these cells at 40a and 3100mah ...similar thing to his rating of 30Q 18650 cells, - samsung rates them at 15A but in real life they just as good as 20A LG HG2. 

https://www.e-cigarette-forum.com/forum/threads/samsung-inr21700-30t-35a-3000mah-21700-bench-test-results-an-incredible-40a-3100mah-battery.798683/
```

---
## \#76 Posted by: agniusm Posted at: 2017-11-06T13:34:16.210Z Reads: 612

```
@NAF Even if so, 6200mah vs 9300mah and power 80 vs 90A by the numbers is just a step back and there are cells at 2000mah with even more power. Sorry, i am not convinced, i see it as not suitable. Maybe some time later they will improove. 18650 is manufactured for so long and in such huge numbers that most bugs are ironed out from manufacturing process. Just dont see the point to switch. OK, if you are spotwelding or soldering makes some point as you do less work, but whats the point when you just shuffle cells in in my design and forget about it?
```

---
## \#77 Posted by: agniusm Posted at: 2017-11-20T08:24:08.923Z Reads: 642

```
Started designing BMS enclosure to fit the NESE design. BMS will be available up to 15S and 30A charge/discharge or unlimited discharge/30A charge with external disconnect (controller logic or contactor hard disconnect).
First i was gonna implement 15pin JST XH 2.5mm connector at the top of the modules (Need 16pin but that does not fit), but it introduced a second wiring loom failure point and i could not utilize full 15S capability, only 14S max. Also this meant a lot more work so more expensive. I started to look for grommets online just realizing that i can print them the way i need. here is what i came up with. The grommet will exit 16 wires to 15 cells or less depending on system voltage. Here are couple of teaser pics:
[img]https://i.imgur.com/nEE52Yw.jpg[/img]

[img]https://i.imgur.com/6tsOkpV.jpg[/img]

[img]https://i.imgur.com/dWeFXzT.jpg[/img]

Minimum enclosure size is 6P or 123mm in length.
```

---
## \#78 Posted by: Sebike Posted at: 2017-11-20T12:59:13.734Z Reads: 607

```
As seen on the Jehu Garcia vlog right?
```

---
## \#79 Posted by: agniusm Posted at: 2017-11-20T19:13:43.760Z Reads: 604

```
I think he mentioned about doing review but still haven't or perhaps i missed it but yes :)
Just checked and there is another mention here: https://youtu.be/Kvlh1mflOCc?t=3120
Probably he is just too busy with so many projects going on. I know those things takes a lot of time, throw in video editing and you are running out of time.
```

---
## \#80 Posted by: banjaxxed Posted at: 2017-11-20T21:19:44.052Z Reads: 592

```
Cell level fusing would be interesting
```

---
## \#81 Posted by: agniusm Posted at: 2017-11-21T09:38:24.996Z Reads: 606

```
  Cell fusing is hyped. If nissan leaf cells can operate unfused, i think we are alright with couple tiny cells.
  Its overrated in small applications and most packs would ignite before the fuse goes off. Note how tesla has air gap arround the fuse. Most diy fised packs dont. You have to sum up failure rate and you will see that properly built 18650 pack does not need complication. Failure rate of 18650 is one in 10000000, do the math
```

---
## \#82 Posted by: Vanarian Posted at: 2017-11-21T10:17:32.372Z Reads: 571

```
Hey my 2 cents opinion disagrees on this point! Any safety feature to prevent hazard, as long as it is well built and do not restrict the ride, should be welcome. Adding air gap between cells and on fuse area should not be so difficult even under a board.
You know better than me random shit happens with lithium batteries. Better be prepared when it comes.
```

---
## \#83 Posted by: agniusm Posted at: 2017-11-21T11:10:04.708Z Reads: 573

```
Random shit happens when people do random stuff with batteries. Use random shit to build batteries.   Look at laptops, tool packs, most of them are unfused. Use propper cells, propper balancing, charger, build packs according to guidelines and you will be fine. Check youtube for overcharged overdischarged and shorted cells. They are not that dramatic. I do reffer this to 18650. 
BTW, adding a fuse is complicated, adding a fuse DIY for it to function is too complicated. Added space arround the fuse will be an issue to most cause it will be that much larger :)
```

---
## \#84 Posted by: Vanarian Posted at: 2017-11-21T13:13:53.309Z Reads: 590

```
I get your point and with proper care everything should be alright, true. But with our hobby we are mainly talking about unsuspended compact vehicle, boards and any "small wheel" stuff deal with lot of vibrations and urban "agressions" (rocks, pebbles, potholes, direct contact with concrete...) 

Let's face it too, most of us don't give a damn about "abusing batteries" when the ride feels sweet, being tempted to pull more current to keep going when suddenly power feels lacking. It's just us being humans, adrenaline can't wait.

When battery packs go thermal runaway for XY reasons it still is ugly. Being able to limit the source of energy to a single defective cell instead of a potential whole pack makes a big difference, be it safety or cost effective - at worst, gaining more time to get off the board ; maybe get enough time to strip battery pack off the board ; maybe the defective parallel cell simply shuts its parallel line down. At best, being able to save undamaged cells and not need buy a whole new battery pack.

This is even more interesting if you use solderless no ? Apart from ease of assembly best part is cells remain standard and never suffered cathode damage due to spot welding.
```

---
## \#85 Posted by: agniusm Posted at: 2017-11-21T13:50:53.045Z Reads: 555

```
Sure, hobby is what makes differnce. I stand by my point cause i dont care about soldered or welded packs. I only care and see the future in solderless and thats why i dedicated some years on this. Put my module on your board and it will not care about the vibration one bit. I have done vibration test at 200A full discharge. Fuse is meant to protect parallel cells not series excluding fire situation. In my case you would need to change 8 cells max, largest module. Making fuses out of copper is nonsense and my busbars are copper. Making busbars from other material is nonsense cause of high r and when you have few cells that limmits your power. Look at vruzend, 3.5A ler cell vs 35A i can pull. Mix of materials? You enter plasma or ultrasonic welders zone and the cost goes up a lot. Plus thin fuses will not sustain compretion and this whole design would not be viable.
```

---
## \#86 Posted by: banjaxxed Posted at: 2017-11-21T18:28:20.064Z Reads: 543

```
The change in tooling is minimal, the change in materials used is a small amount more poron 😉
```

---
## \#87 Posted by: agniusm Posted at: 2017-11-21T19:22:44.743Z Reads: 578

```
The change is dependant on how many you sell ;)
I dont see a point so i wont do it. I would advise to use propper electronics with my system and you will be alright and the rest systems i dont care about. If people want to glue cells with houshold hot glue, fine. If people want to use rc stuff for charging, monitoring, fine but i am not gonna start changing stuff that i have no believe in based on thin air. I have other facts and my math is based on solid propper stuff, not on missuses
```

---
## \#88 Posted by: agniusm Posted at: 2017-11-22T14:20:34.615Z Reads: 588

```
Got some tools and supplies. Will start making test samples for BMS harness

[img]https://i.imgur.com/jjcTuFY.jpg?1[/img]

P.S. Just this once i can offer a pre-built battery containing 10S(3-6)P with bluetooth BMS and chosen cell type from www.nkon.nl with free assembly for EU.
```

---
## \#89 Posted by: themegak Posted at: 2017-11-22T14:33:05.630Z Reads: 548

```
Kudos for innovating on this front.  Wish I knew of your solution a couple of years ago.
```

---
## \#90 Posted by: banjaxxed Posted at: 2017-11-24T18:18:41.006Z Reads: 541

```
Knipex? they make some sweet levers, love mine.
```

---
## \#91 Posted by: agniusm Posted at: 2017-11-25T19:41:12.953Z Reads: 542

```
Yeah, i think they are one of top brands for wire manipulation tools (cutters, strippers, crimpers). I still want a crimper with interchangeable dies but they are 150-250 eur :(
```

---
## \#92 Posted by: banjaxxed Posted at: 2017-11-26T09:40:53.170Z Reads: 528

```
Ouch! Yeah they are top like festool
```

---
## \#93 Posted by: OLnewB Posted at: 2017-11-27T03:01:45.832Z Reads: 531

```
Weird question; can you use 3 cells in a 4p enclosure since the bus bars are continuous? I was thinking I could buy batteries for a 10s3p setup and if not enough power, I could upgrade it to 10s4p without changing enclosures.
```

---
## \#94 Posted by: banjaxxed Posted at: 2017-11-27T19:26:34.347Z Reads: 505

```
Can't see why not
```

---
## \#95 Posted by: agniusm Posted at: 2017-11-28T08:41:01.683Z Reads: 515

```
Sure it will work any way you like it. You could put one cell in 8P add the rest later.
Only thing to watch out is cell age and cycle life. You want cells to be as close to one another with cycle life and age as possible
```

---
## \#96 Posted by: Nowind Posted at: 2017-12-04T09:20:20.860Z Reads: 526

```
[quote="agniusm, post:88, topic:36847"]
P.S. Just this once i can offer a pre-built battery containing 10S(3-6)P with bluetooth BMS and chosen cell type from www.nkon.nl with free assembly for EU.
[/quote]


Hey @agniusm
Really like your work on this modules.
Interrested in 10S-4P
and 12S-6P 
I would prefer the Samsung 30Q
Could you send me a pm with your Pricepoint ?

Cheers from Germany
Jens
```

---
## \#97 Posted by: agniusm Posted at: 2017-12-04T10:02:42.368Z Reads: 512

```
Hi, could you contact me on agniusmk at gmail dot com
```

---
## \#98 Posted by: banjaxxed Posted at: 2017-12-11T13:00:29.316Z Reads: 538

```
Hey @agniusm, any interest in releasing a coupon - to the community for a discount or by pm? I'm on the verge of ordering a 12s4p hardware set after making a test print.

Also going to build a powerbank, how cool! I have the circuit board that you show although had some problems getting it to power up using my graphene 3s lipo, any suggestions or details on getting it together? Ah, methinks it should only get a max of Power input: 5V 1A

Edit wiring is covered on YouTube if not self evident
```

---
## \#99 Posted by: agniusm Posted at: 2017-12-12T05:59:57.914Z Reads: 534

```
I'll se what i can do for Christmas even if its small.
Wiring powerbank is like soldering two wires. Simple
```

---
## \#100 Posted by: agniusm Posted at: 2017-12-12T07:16:42.210Z Reads: 529

```
:santa: Till the end of the year small present, 10% off. Coupon code - christmas :santa:
```

---
## \#101 Posted by: banjaxxed Posted at: 2017-12-12T10:06:08.853Z Reads: 541

```
Thank you I took advantage of this kind offer to the forum, you should see some orders no doubt oncluding mine today.

You do nice work like some of the folks here, I'm pretty much a newbie too but welcome ☘️
```

---
## \#102 Posted by: DEEIF Posted at: 2017-12-21T01:18:17.652Z Reads: 506

```
Hey @agniusm  you have an update for the bms
Also what does the 3-4-5-6p enclosure thing do
```

---
## \#103 Posted by: agniusm Posted at: 2017-12-21T19:01:51.530Z Reads: 510

```
Hi. You lost me here. What do you mean. "What it does"? It encloses 3 to 6 cells.
Bms is being worked on. I have no space to play with so basically push things arround so it fits 6P enclosure. Its really tight fit for 15 balance wires and jst connector. I have soldered different header for the bms so it could be pluged without wires. Need to print another sample to see fitment but my printer is buisy :stuck_out_tongue:
```

---
## \#104 Posted by: DEEIF Posted at: 2017-12-21T23:03:17.452Z Reads: 500

```
Oh ok hit me up when the bms is done
```

---
## \#105 Posted by: deucesdown Posted at: 2017-12-29T02:58:13.077Z Reads: 501

```
The code got me, order placed. thanks also to @banjaxxed for badgering for coupon :)
```

---
## \#106 Posted by: SeanHacker Posted at: 2017-12-29T03:18:48.389Z Reads: 507

```
@agniusm 

Hi! This looks awesome. I'm dumb in the battery department. So bare with me. Just tell me EVERYTHING I need to buy from your website for a 10S5P setup. Nuts, bolts, buss connectors, etc... Thanks!!!
```

---
## \#107 Posted by: deucesdown Posted at: 2017-12-29T04:29:30.876Z Reads: 481

```
1st question is going to be do you have a 3d printer or access to one?
```

---
## \#108 Posted by: SeanHacker Posted at: 2017-12-29T05:04:50.585Z Reads: 479

```
I don't own a 3d printer or anything. I can use 3D hubs if need be. I thought I could just buy everything from the site in the OP of this thread?
```

---
## \#109 Posted by: deucesdown Posted at: 2017-12-29T05:44:02.118Z Reads: 514

```
Yup, but your answer changes what you need to buy.

Just to get things going until the man answers, I think you'll be looking at 10 of these (5p version):

http://18650.lt/index.php/product/n-e-s-e-module/

In the description, 
[quote]
You will need to purchase series tabs to connect modules into battery pack. Optionally you can order twin and single bolt caps to avoid accidental short circuit.  Technical drawings are in Resources area.
[/quote]

You'll need 9 series tabs to hook the units up. If you go for the caps, 9 twin caps and 2 single caps.
```

---
## \#110 Posted by: agniusm Posted at: 2017-12-29T07:01:19.285Z Reads: 499

```
Hi mate. deucesdown answered your question so i will just repeat.
I have printer cases in my shop and they work out at least 3rd cheaper of what you can find on 3d hubs. Shipping goes up but in the end i think its cheaper.
Here is the list what you need:
10 x 5P [http://18650.lt/index.php/product/n-e-s-e-module/](http://18650.lt/index.php/product/n-e-s-e-module/)
9 x [http://18650.lt/index.php/product/n-e-s-e-series-tab/](http://18650.lt/index.php/product/n-e-s-e-series-tab/)
Optionally you want:
9 x [http://18650.lt/index.php/product/twin-bolt-cap/](http://18650.lt/index.php/product/twin-bolt-cap/)
2 x [http://18650.lt/index.php/product/single-bolt-cap/](http://18650.lt/index.php/product/single-bolt-cap/)
Regards
```

---
## \#111 Posted by: banjaxxed Posted at: 2017-12-29T10:53:43.981Z Reads: 486

```
Balls I forgot to order the single cap terminals haha, guess I'll be modding for the small roll of ninja flex soon ☘️

Ps don't think the series connections would be viable for a bottom side series of packs? Can you use them for packs laid flat?
```

---
## \#112 Posted by: agniusm Posted at: 2017-12-29T11:09:58.510Z Reads: 491

```
Yes, you can. center of terminal holes are 11mm from ether side so you can stack them back to back or side by side. Series busbars have oval holes so should allow for minor slack. I can sort you out with caps so you dont need whole roll of filament. I will adjust and refund overpaid shipping after posting. 
Regards
```

---
## \#113 Posted by: banjaxxed Posted at: 2017-12-29T12:11:31.574Z Reads: 474

```
Well that's mighty thanks for the offer sir. I may just put in an order for those caps etc

But I have the roll of ninja already :skull_crossbones: & the extruder part that wil allow me to grab it, if I give up you'll hear from me :)

Cheers, wishing you a happy new year and plenty of esk8 orders
```

---
## \#114 Posted by: deucesdown Posted at: 2017-12-29T14:54:52.274Z Reads: 465

```
Hey wait I thought the caps were abs? I may need to add to my order...

Edit: I need to learn to read. Well I gUess buying a spool of ninjaflex will be better for me in the long run.
```

---
## \#115 Posted by: NAF Posted at: 2017-12-29T15:01:07.314Z Reads: 449

```
Please make a youtube video on you battery pack assembly.
```

---
## \#116 Posted by: banjaxxed Posted at: 2017-12-29T16:29:52.486Z Reads: 490

```
I think @agniusm has pack assembly videos on YouTube already principle is the same, esk8 application on my unfinished build thread

http://www.electric-skateboard.builders/t/magharees-puca-caliber-ii-fifty-2-x-aps-6355s-wsb-v1-0-mounts-johnny-261-pulleys-akhlut-x-bolt-plates-agniusm-n-e-s-e-cell-holders-samsung-25r-12s4p-freebord-s2-bindings/41278/19
```

---
## \#117 Posted by: banjaxxed Posted at: 2018-01-24T11:44:01.834Z Reads: 480

```
@agniusm I tried to print out a couple of caps myself, mostly to try a flex filiment 

But the stl I pulled from the site is smaller and different? Please Ignore the print quality 🙃 ![IMG_8440|666x500](upload://7CP5LKm8n9kc55mWvjVhXWUPb7U.JPG)

http://18650.lt/index.php/resources/single-bolt-cap/
```

---
## \#118 Posted by: agniusm Posted at: 2018-01-24T14:38:40.175Z Reads: 466

```
Hm, good to know. Probably old version mixed up somehow. I will reupload in an hour. Thanks for letting me know
```

---
## \#119 Posted by: agniusm Posted at: 2018-01-24T16:29:07.479Z Reads: 451

```
Re-uploaded files. Please check now
```

---
## \#120 Posted by: deucesdown Posted at: 2018-02-03T19:13:40.799Z Reads: 472

```
Hey, thanks for the idea about connecting and printing 3-4 trays together. Maybe I'll give it a try scaled to 50% or something, to see if the lids still work, and work out the spacing.

In other news, I used up a whole spool of that color change ABS learning how to print with the stuff. Ordered more, so I can try more stuff. Printing with the bed at 115-120 seems make the top contract, so the lids don't fit nicely. I think I'm gonna do something with an enclosure after all. Which would let me try ganged trays (although PETG is probably gonna hurt me less).

I got some HK TPU as well. Tried printing your revised caps, and using Prusa's semiflex settings, which has extrusion multiplier 1.10. Had to scale the parts 117% for fit. 

In flex filament news, HK seems to have revised their TPU spools from 1kg to .8kg. Maybe it's all the same stuff, HK, SainSmart, eSun, Inland... Anway this makes the SainSmart TPU on Amazon with Prime a lot more attractive. I'm having better luck with HK's TPU right now, over the SainSmart. I'm also going to try at some point Polymaker's Polyflex. It's expensive, but if it prints with no headaches it'll be worth it. And it's available on Prime. For some reason white is cheaper.

And I think I discovered something, for the people in USA. If I add one spool of filament to my cart, and hit $50+ for the order, I get free shipping.
```

---
## \#121 Posted by: banjaxxed Posted at: 2018-02-03T19:36:17.481Z Reads: 449

```
Fwiw I used hobbyking abs colour changing filament. Iirc it has a nice melt / print point about 239, the bed I kept at 105, but I also use a glass sheet. The case will want to warp so place a plastic box over the printer for higher ambient temperature.

It helps to use some glue stick especially around the corners
```

---
## \#122 Posted by: deucesdown Posted at: 2018-02-03T19:50:53.775Z Reads: 445

```
Might as well dump out what I've learned so far.

I tried PLA, PETG and the HK color change ABS. PLA doesn't really make sense for this. PETG I think printed the best and felt the strongest. ABS is really a pain to print, and doesn't feel that strong. Haven't tried an enclosure yet. I'm not sure that the temperature advantage over PETG is worth it. But that color change is very compelling.

PETG was not easy to print for me, in general. I believe I had to slow first layer down to 10mm/s, and globally limit to 50mm/s. Lots of stringing and blobbing. Enough blobbing, and the print fails. But I don't remember having the corners lift with such intensity, so if the first layer stuck and blobbing was not too bad, dimensionally the part came out good. And strong. This is Inland's PETG from Microcenter, which is about the cheapest I could find, $19 per 1kg.

For flex for rubber caps, I tried SainSmart TPU and HK TPU. They're both a stringy mess :) I think they're both 95A but the HK is noticeably stiffer. Either will work. They're among the cheapest flex filament. SS was amazon prime about $27 for .8kg. HK is about $29 for .8kg.

Oh and HK color change ABS is about $20 for 1kg.
```

---
## \#123 Posted by: Hariboisawesome Posted at: 2018-02-03T20:07:05.104Z Reads: 455

```
![image|375x500](upload://ifOvcoNFAeBO10GzBttW4s1kgXY.jpg)
I had bought one of these kits from veruzend(spelling?) though I’m not sure if it’s practical
```

---
## \#124 Posted by: deucesdown Posted at: 2018-02-03T20:10:27.189Z Reads: 454

```
They look good but the max current is a fraction of NESE. So depends on your application. I don't think they're great for high power boards.
```

---
## \#125 Posted by: Hariboisawesome Posted at: 2018-02-03T20:18:54.415Z Reads: 456

```
I had bought it for science, 😂(I finally get to say that!) I had the 25r cells and was going to use it for a dual jet Spud with Turnigy 260kv
```

---
## \#126 Posted by: agniusm Posted at: 2018-02-25T19:13:49.447Z Reads: 439

```
Most of the stringing is your orint setting. It is a balance between temperature and retraction. Hk flex is stringy and I dont lower temp just to get layer bond better. Mkst of the stringing is inside and I burn it with blow torch, just a quick pass. Depending on which surface you print, petg sticks to pei like crazy. 
It boils down to how good you knkw your printer and how good it is set up:)
```

---
## \#127 Posted by: agniusm Posted at: 2018-04-19T16:45:25.649Z Reads: 424

```
Now 2P is also in the line up
```

---
## \#128 Posted by: Benjamin899 Posted at: 2018-04-30T21:47:55.019Z Reads: 415

```
nice work. i looked around for 3d print services and they are all way way way more expensive than you are, even with tax and shipping...kinda crazy how cheap you sell those modules.
```

---
## \#129 Posted by: Holyman92 Posted at: 2018-04-30T22:41:38.489Z Reads: 398

```
3d services are only worth it for large batch prototyping... anything else you're better off finding a printer at a local makerspace or buying your own
```

---
## \#130 Posted by: uigiroux Posted at: 2018-04-30T23:10:34.777Z Reads: 395

```
I hadn't planned on using these but thinking about it now they would be kinda perfect and you could easily take the battery apart for flights so regardless of the size you could take it anywhere.  I hope they can make them in 20700 or 21700 size..
```

---
## \#131 Posted by: Benjamin899 Posted at: 2018-05-01T00:01:43.506Z Reads: 382

```
26650 would be awesome
```

---
## \#132 Posted by: agniusm Posted at: 2018-05-01T05:09:59.615Z Reads: 370

```
Yes, even biggest 8P is 103wh with 3500mah cells so you could take it on a plane.
```

---
## \#133 Posted by: agniusm Posted at: 2018-05-01T05:12:01.166Z Reads: 367

```
Yeah. I could not understand why they charge so much. It was the reason i went on printing them myself. I even build my 400x400 diy printer for that.
```

---
## \#134 Posted by: agniusm Posted at: 2018-05-01T05:15:23.081Z Reads: 390

```
Although it would be easy for me to make for different cell size, little demand will not cover tooling cost. I think that there is no reason to choose other format than 18650. They are most dense, have most power.
```

---
## \#135 Posted by: agniusm Posted at: 2018-05-01T08:22:39.343Z Reads: 423

```
BTW, if any of you guys are also into powerbanks(powerwalls). I have a design for that. Its a 5 slot module utilizing same principal for 10 parallel cells. Bolts to the wall and interconnects with each other to form large modules. It is designed so fuses could be used per 2 cells.

[img]https://i.imgur.com/qBp9xzD.jpg[/img]

[img]https://i.imgur.com/HnZPt01.jpg[/img]

Here is a prototype assembly vid:
https://youtu.be/NreICu4gYaE

I have DIY kit on my website if anyone wants to experiment but i am getting pricing to make it cheap for large builds including enclosures.
```

---
## \#136 Posted by: banjaxxed Posted at: 2018-05-01T09:29:36.101Z Reads: 404

```
Pretty cool 
http://18650.lt/index.php/2018/04/16/powerwall/
```

---
## \#137 Posted by: Benjamin899 Posted at: 2018-05-01T10:26:12.126Z Reads: 409

```
how much did you pay for your diy printer? rough estimate
```

---
## \#138 Posted by: agniusm Posted at: 2018-05-01T10:32:55.506Z Reads: 430

```
I think i spent over 2000€

[img]https://i.imgur.com/gXSUfz8.jpg[/img]
```

---
## \#139 Posted by: uigiroux Posted at: 2018-05-01T11:22:02.629Z Reads: 421

```
Well the new cell sizes are like 50-60% + or more, more powerful so it would make sense to use them...  I was going to have to use a 12s6p with 30Q's for my AWD build but instead with these cells I can go 12s4p :smile:
```

---
## \#140 Posted by: Ronny_CTS Posted at: 2018-05-01T11:29:04.389Z Reads: 423

```
@agniusm i've been toying in my mind the following idea and would like to get your opinion on its viability. 

I've been thinking of creating a 16 cell long module and using two 8 cell tabs welded in the middle. Since uncut tabs have holes on both side, by bending the hole tabs inwards and welding them you could create a 16 cell long tab. 

My plan is not to create a 16P battery pack, but a 4S 4P with this design. You think it would work? I would then connect 3 and make a 12S 4P modular pack made from 3 rows of 16 cell modules.

These modules could also have terminals on both ends or not. Depending on the application.
```

---
## \#141 Posted by: agniusm Posted at: 2018-05-01T11:40:54.917Z Reads: 413

```
@uigiroux show me that cell capable of 50-69% more and i will prove you wrong ;)
@Ronny_CTS its possible. You cant bend tabs invard as cells are tight and there is no room. You could cut and weld tabs with tig though if you know someone. Problem is balance wires. No room for them unless you drill out sides and run them externally. You would also need to double wire for bms. Why not just take 4P module and series to 12S ?
A lot better that way.
```

---
## \#142 Posted by: Ronny_CTS Posted at: 2018-05-01T12:34:12.140Z Reads: 390

```
I was thinking of modelling some space between the 8th and 9th cell to to accommodate the bent tabs and also serve as nerving to avoid bowing of the sides. 

The whole reason is space constraint. I was trying to add as much as i could to the smallest package possible. From what I've determined with your packs, the higher the number of cells, the less space is lost.
```

---
## \#143 Posted by: uigiroux Posted at: 2018-05-01T12:39:27.368Z Reads: 385

```
Well I can't say for sure what the exact percentage higher these cells are, but I read multiple times it was up to that amount.  I've been looking at the Samsung 30T, 40T, Sanyo NCR20700C, and a few others, but those are the main ones I'd say..
```

---
## \#144 Posted by: banjaxxed Posted at: 2018-05-01T13:40:07.347Z Reads: 377

```
An inbuilt cell capacity monitoring system would be great
```

---
## \#145 Posted by: agniusm Posted at: 2018-05-01T13:40:15.467Z Reads: 400

```
@Ronny_CTS, yes, you are correct. Space is lost at bolt end where it is allocated for holes and cavities.
If you want you terminals to be on one side you cant go 8P+8P, you need 8P+7P. For terminals to be on one side you need uneven count of cells. If you OK with terminals on opposite ends, that means you add same allowance for screw holes and cavities. Then you add your spacing and some wire routing and you are at the point where space saving is negligible if any. Printing might be hard as well. Mine were designed strait away to be printed without supports if you look at the angles .
Try, and you might come up with something ;)
@uigiroux  Take the last one, NCR20700C (3500mah), volumetric density is 21991.15mm^3 if translated to 18650 volume it would hold 2630mah
Sony US18650VTC6 is 3120mah, 19% more dense than you 20700 at the same power (30A). 
Take 4 20700, cell are is 1242mm^2 bounding rectangle area of these is 1600mm^2
Take 5 18650, cell area is 1258mm^2 bounding rectangle area - 1620mm^2
4 parallel 20700(NCR C) will give you 14AH and 120A peak
5 parallel 18650(VTC6) will give you 15.6ah and 150A peak.
```

---
## \#146 Posted by: agniusm Posted at: 2018-05-01T13:42:54.811Z Reads: 366

```
@banjaxxed thats what bms is for.
```

---
## \#147 Posted by: banjaxxed Posted at: 2018-05-01T13:47:03.753Z Reads: 381

```
true, I'm not au fait with powerwalls but I saw a picture of one which had a led beside each cell.

I think leds are the way to go with so many cells, you can glance at the wall and see where a problem exists.

I like this product branch for nese, I'll try it when I have my own wall and not a rented one where I live now, we get power cuts fairly frequently
```

---
## \#148 Posted by: uigiroux Posted at: 2018-05-01T14:22:00.812Z Reads: 371

```
Well I'm figuring more than just the voltage but the amps as well, there double on many of those cells.
```

---
## \#149 Posted by: agniusm Posted at: 2018-05-01T14:31:35.145Z Reads: 379

```
@uigiroux what do you mean? Volts are the same no matter size. I pointed that soni us18650vtc6 is 19% mkre dense then NCR20700 at the same power or 19% more powerfull at the same  volumetric density.
```

---
## \#150 Posted by: uigiroux Posted at: 2018-05-01T14:34:38.091Z Reads: 373

```
Lol my bad, I meant mAh, not volts :blush:
```

---
## \#151 Posted by: uigiroux Posted at: 2018-05-01T14:35:46.239Z Reads: 371

```
What about with the Samsung 30T and 40T?
```

---
## \#152 Posted by: agniusm Posted at: 2018-05-01T14:42:44.352Z Reads: 372

```
@uigiroux, 30T is worse than ncr, 40T is larger so i would assume same math applies.
@banjaxxed How about investing in BT bms so you get audible notification when cells go out of normal? No need to glance anywhere?
I just dont like the idea LED's draining cells 24/7
```

---
## \#153 Posted by: uigiroux Posted at: 2018-05-01T14:44:35.953Z Reads: 364

```
How are they worse though?  Like your completely ignoring amps, there double to even more than double.  The mAh isn't the only important value with these cells.
```

---
## \#154 Posted by: agniusm Posted at: 2018-05-01T15:03:00.473Z Reads: 402

```
I am not ignoring amps. Here, 2 examples. 
INR21700-30T
Size - 21700
Capacity - 3000mAh
Power - 35A

US18650VTC6
Size - 18650
Capacity - 3120mah
Power - 30A

Even this will be better:
US18650VTC5A
Capacity - 2600mah
Power - 35A

I don't know how can one not see the numbers?
I wrote power levels of the two in P groups:
4 parallel 20700(NCR C) will give you 14AH and 120A peak
5 parallel 18650(VTC6) will give you 15.6ah and 150A peak.
in the same size package (VTC6 being 20mm^2 larger area (not volume))

I can sum up: 20700, 21700 is crap
```

---
## \#155 Posted by: uigiroux Posted at: 2018-05-01T15:17:24.410Z Reads: 381

```
Ok but those aren't the actual values?  The VTC6's are 3000mAh and 15A.  VTC5A is 2500mAh and 25A, Samsung 30Q is 3000mAh and 15A.  So the 40T has 4000mAh and 30A so for most cells its double amp and 33% more mAh. Samsung 30T is 3000mAh and 35A so more than double A then many buy still about the same mAh.  Sanyo NCR20700C is 3500mAh and 30A.  Still better than the 18650's as well..?  I'm not trying to argue or anything, I'm new to this stuff until about a year ago, but as far as I see these are much higher amps than most of the smaller cells and usually about 25-35% more mAh.
```

---
## \#156 Posted by: agniusm Posted at: 2018-05-01T15:42:51.725Z Reads: 368

```
Those are actual manufacturers numbers and I were comparing them on both sides 18650 vs. 20700/21700
Real world values will vary but they will vary on both sides. I have fully discharged six vtc5a at over 200A.
```

---
## \#157 Posted by: uigiroux Posted at: 2018-05-01T15:50:19.402Z Reads: 384

```
Well yeah I mean they can discharge at higher levels, but so can the larger sized ones as well.  The average levels they are putting out though I imagine has to be relative, so even if they can have burst levels that are much higher, I would imagine that the larger cells have burst levels that are even higher since under normal conditions they are rated higher...  Lol I dunno bro, you may very well be right, I just think I'm going to go for the larger ones regardless :smile:
```

---
## \#158 Posted by: agniusm Posted at: 2018-05-01T16:03:47.935Z Reads: 384

```
I think you should go for something you like. I like 18650. Its old standard, manufacturing is well worked out.
Thats why my solution is based on 18650 which use 95% of people :)
```

---
## \#159 Posted by: uigiroux Posted at: 2018-05-01T16:08:15.344Z Reads: 391

```
Right on, that probably is the best business decision.  I thought the larger sized cells would be becoming much more popular by now but it seems the price is off putting for most..
```

---
## \#160 Posted by: agniusm Posted at: 2018-05-01T16:35:31.039Z Reads: 395

```
They make sence in tesla, robots can save a lot of time having less welds to do = money, not so much on small builds like bikes or boards ;)
```

---
## \#161 Posted by: agniusm Posted at: 2018-05-16T06:25:20.958Z Reads: 398

```
**SUMMER IS COMING. 10% OFF FOR THE WHOLE JUNE.**
Code - SUMMER
```

---
## \#162 Posted by: agniusm Posted at: 2018-06-01T05:30:12.652Z Reads: 379

```
Coupon code is active now.
3D models were updated to the new version.
Happy building this summer!
```

---
## \#163 Posted by: uigiroux Posted at: 2018-06-01T05:40:37.575Z Reads: 382

```
What's the new version?

I really think these are such a great product, though if I could make one change, I would like to see terminals on both sides of the pack.  That way regardless of orientation in an enclosure, battery packs could be assembled with your terminal connectors and not require any lengthened wire.
```

---
## \#164 Posted by: agniusm Posted at: 2018-06-01T05:56:36.406Z Reads: 384

```
Thank you. I can make a 3d model for you. If you dont have a means to 3d print, we can arrange a custom order.

Changes are slight:
Added chamfer all round so it feels better and someone eho prints modules and has nozzle too close, to help with "elephant foot"
Added markings for positive/negative near terminals.
After my holydays i will do short vid on tips and tricks.
```

---
## \#165 Posted by: uigiroux Posted at: 2018-06-01T05:58:02.733Z Reads: 371

```
Thank you!  I'll PM you tomorrow :smile:
```

---
## \#166 Posted by: dg798 Posted at: 2018-06-01T14:20:48.110Z Reads: 378

```
Noob question: if I’m doing 12s5p how many series busbars do I need?
```

---
## \#167 Posted by: Benjamin899 Posted at: 2018-06-01T22:30:23.631Z Reads: 364

```
make a drawing, if you need to ask that you shouldn't be building your own battery, no offense
```

---
## \#168 Posted by: dg798 Posted at: 2018-06-01T22:31:41.972Z Reads: 370

```
I don’t plan on building my own I was just curious if I decide to in far future 😉
```

---
## \#169 Posted by: agniusm Posted at: 2018-06-02T10:25:27.313Z Reads: 374

```
Dont be discouraged. No offence Benjamin899 but long time ago I would ask similar questions and this is how you start. I am all hand and encourage people to diy.
To answer your question, you always deduct -1 from your total series pack, 12S 11 series bus bars, 24S 23 series busbars. For BMS/PCM balance/sense wires you always add 1, so for 12S you will have 13 wires for 24s you will have 25 wires in most cases as sometimes some bms/pcm's use main negative power wire as well as sense wire.
If you will decide to go with my system I provide advice and help choosing other hardware in terms of bms and can help guiding you how to wire. Good luck
```

---
## \#170 Posted by: Benjamin899 Posted at: 2018-06-02T11:18:41.434Z Reads: 350

```
np, i just want him to use the search function and educate himself, because there is so much to learn about batteries, because relying on other people can go wrong fast in many ways
```

---
## \#171 Posted by: dg798 Posted at: 2018-06-03T01:21:07.204Z Reads: 355

```
Wow thanks sooo much. Very informative. I appreciate it
```

---
## \#172 Posted by: agniusm Posted at: 2018-06-03T19:06:53.251Z Reads: 382

```
So i have been asked if i can make 2S4P module by @uigiroux. I thought i would post this here for anyone interested. Only downside would be longer series connection if you place them flat on the deck. I have also added 4mm holes to mount them permanent but the lid could be taken off and cells inspected/replaced. Here it goes:
[img]https://i.imgur.com/4PDIgP9.jpg[/img]

[img]https://i.imgur.com/fERrl95.jpg[/img]

Holes are also slotted at the top to accommodate DIN912 hex bolt head so the lid still closes.
```

---
## \#173 Posted by: uigiroux Posted at: 2018-06-03T19:18:54.709Z Reads: 351

```
Looks great!  Just finalized my order :smile:
```

---
## \#174 Posted by: agniusm Posted at: 2018-06-03T19:30:05.813Z Reads: 351

```
Thanks. Sent you an email
```

---
## \#175 Posted by: Benjamin899 Posted at: 2018-06-03T20:51:59.396Z Reads: 351

```
wow this is awesome, i was about to finalize my build but with this 2s4p i could built it the way i wanted.
```

---
## \#176 Posted by: Ronny_CTS Posted at: 2018-06-03T23:51:08.023Z Reads: 354

```
Looks great! Can i get the overall dimension on the 2S4P? Basically length as the rest should be the same.
```

---
## \#177 Posted by: uigiroux Posted at: 2018-06-04T00:57:57.558Z Reads: 350

```
Just add an extra 10mm for each side with a terminal, so 18x8 + 20= total width.  I think it's about 70mm tall, maybe a bit more.
```

---
## \#178 Posted by: Benjamin899 Posted at: 2018-06-04T01:03:22.052Z Reads: 349

```
standart 1s8p is ~160mm so ~170mm+
```

---
## \#179 Posted by: uigiroux Posted at: 2018-06-04T01:37:24.001Z Reads: 344

```
Yeah basically
When I was talking with him about the dimensions, we arrived at 6
164mm, so 6.5in.
```

---
## \#180 Posted by: Benjamin899 Posted at: 2018-06-04T12:33:03.544Z Reads: 339

```
thats cool, i rly like that 2s setup, saves space under the deck.
```

---
## \#181 Posted by: uigiroux Posted at: 2018-06-04T12:40:04.341Z Reads: 344

```
I think so too, and just so much easier to make, and easier to travel with for sure!
```

---
## \#182 Posted by: XTLA Posted at: 2018-06-04T12:56:30.223Z Reads: 317

```
Why i can not see the 2s4p image above :face_with_raised_eyebrow:
```

---
## \#183 Posted by: Benjamin899 Posted at: 2018-06-04T13:00:56.707Z Reads: 319

```
dunno, i can see it normally
```

---
## \#184 Posted by: XTLA Posted at: 2018-06-04T13:04:44.581Z Reads: 318

```
I also interested with nese module, i’ve tried with vruzend kit before, its working but i notice that the nuts keep coming loose. Maybe i should check the image from my laptop not from my phone.
```

---
## \#185 Posted by: Benjamin899 Posted at: 2018-06-04T13:23:54.370Z Reads: 319

```
the v2 kit oder v1.5 and older? mabe try some locktide
```

---
## \#186 Posted by: XTLA Posted at: 2018-06-04T13:24:24.191Z Reads: 321

```
The new v2 kit
```

---
## \#187 Posted by: agniusm Posted at: 2018-06-04T13:48:53.806Z Reads: 330

```
The overal dimensions are 167.1 x 74 x 22mm.
I will get the modules done for uigiroux and will post findings
```

---
## \#188 Posted by: uigiroux Posted at: 2018-06-04T14:06:50.884Z Reads: 334

```
I'll post many pics as well.  This has so many more benefits then being easy to assemble and no soldering required, but this makes it so you can fly with any sized battery you want, plus if you notice a problem with a cell, you can easily swap out cells.  Additionally, I was just thinking how these may be the largest size you can get, so 4p is the largest they make, but you could easily add another p group or more.  Just order 2 of the 6p models, and make it a single 12s series.  You could double this for 2p, or more easily would be to get 3 8p units and just components) combine these with the other pack and you have 12s4p + 12s1p/2p/etc..
```

---
## \#189 Posted by: XTLA Posted at: 2018-06-04T14:11:29.254Z Reads: 341

```
Planning to built 10s3p with nese, but this 2s4p idea also good option to go.
```

---
## \#190 Posted by: uigiroux Posted at: 2018-06-04T14:13:18.634Z Reads: 351

```
I sure you could request a double sided 6p module.  Would be very easy to build :smile:
```

---
## \#191 Posted by: agniusm Posted at: 2018-06-12T08:28:57.571Z Reads: 373

```
So after collaboration with uigiroux, we have 2S4P module. The listing on my shop was created for him to get first batch but someone from here i guess snatched another 2 modules, naughty :slight_smile:
Had one batch failed so it takes more time than anticipated, but we are getting there. mounting holes were changed to M3. 4 x is plenty and they allow for thicker walls. I have assembled first sample without mounting holes and it feels and looks very good. Here are some shots i made yesterday:

[img]https://i.imgur.com/xEXxwOy.jpg[/img]

[img]https://i.imgur.com/hT2uMzN.jpg[/img]

[img]https://i.imgur.com/Wy9GvKz.jpg[/img]

So if someone finds them useful, you can thank uigiroux for kicking me in a butt :smiley:

Another thing we are working is same type of enclosure to fit DieBieMS BMS produced on these forums and i am personally very excited for the brilliant products engineered by DIY folks.

[img]https://i.imgur.com/Jtt0qeI.jpg[/img]

[img]https://i.imgur.com/oRgZ0R5.jpg[/img]
```

---
## \#192 Posted by: agniusm Posted at: 2018-06-12T09:29:43.346Z Reads: 364

```
Some brainstorming needed.There are 5 power connections to the bms and as i was told 2 are linked, common- and pack-. So we have 4 power connections which is good as 2S4P has 4 power outputs. BMS also has USB, CAN, dont know if VESC has another connector or connects through CAN and display.
BMS enclosure will have output for sense wires similar to this:
[img]https://i.imgur.com/6tsOkpV.jpg[/img]
i thought perhaps it would be better to route OLED, VESC as well as sence wires like that as there will be two openings, one at each end?
...and leave USB without access(i think i read that it could be programmed through VESC(even if not its one time job)? i think making a bunch of openings is a bad idea.

BTW I will have some tube ring terminals(for NESE modules) in my shop later this month, 2.5mm²(10AWG), 6mm²(8-7AWG), 10mm²(5-4AWG) and 16mm²(4-3AWG) to be used with this tool:
[img]https://i.imgur.com/7eAou7b.jpg[/img]
or larger:
[img]https://i.imgur.com/6HH169J.jpg[/img]
```

---
## \#193 Posted by: lock Posted at: 2018-06-12T12:10:38.512Z Reads: 354

```
This could all work together quite nicely, it'd be possible to offer pre-wired configurations with multiple NESE modules already strung together to the BMS module itself. Only thing left to do would be to insert the cells and that looks pretty hard to mess up . . . assuming you get polarity correct.

A few thoughts.

There's **5 power connections** you'll need to expose; battery positive, battery negative, load positive, charge positive, and common negative (for charge and load).

There's a connector for the display, another for the power button, and two canbus connectors. It can get annoying having cables running inside an enclosure such as this as you have to open it up to connect/disconnect them. I don't have a good solution for this, ideally these connectors would be on the case surface. The small hole you've shown above could work, these are all small gauge wires.

The other side of the sense wire connector is quite large. Imagine that black connector being 30% wider, with that extra 30% extending off to the RHS. It wont fit in your current design mockup. Then there's the wires themselves, the whole section between the two RHS terminals may need to be removed.

Ideally the canbus would be used for setup and monitoring, but last I heard from jtag the firmware wasn't quite 'there' yet. That leaves USB as the only reliable way to configure it; as you've said it's a one time job. You can also get diagnostic information via USB (cell voltages, current state, etc), it would be a shame not to be able to get at this easily. I'll usually check the cell voltages/balance when I remove my deck enclosure, but this is pretty infrequent.
```

---
## \#194 Posted by: agniusm Posted at: 2018-06-12T12:56:35.734Z Reads: 348

```
Battery negative and common negative are linked internally I was told, so you can use either.
I will not get into building full systems as this takes lots of time, systems varie, and people want different setups. Mockup is with other end connector plugged in so there should be space for balance wires. I tried 15s with lesser space on 6P module. It almost fitted :D
The reason I dont want holes is for water and dirt to have less chance to get in as its delicate electronics inside.
Something like this could be used:
https://www.fasttech.com/product/1329800-micro-usb-to-usb-2-0-right-angled-otg-cable-15cm
```

---
## \#195 Posted by: uigiroux Posted at: 2018-06-12T12:56:40.456Z Reads: 343

```
I love the idea of having a BMS enclosure all wired up only requiring the addition of cells!  Though I would like to mount the LED display on the outside of the main enclosure, not the outside of the NESE module.

Another thing I would really like is a cable professionally made that allows you to connect two VESC's via canbus, but also has the canbus from the BMS connected to that as well.  I know this can be made on one's own rather easily, but I'd prefer a professionally made cable.
```

---
## \#196 Posted by: uigiroux Posted at: 2018-06-12T12:58:47.611Z Reads: 329

```
I've noticed a few people making 13s builds using charge only bms that are very small.  It would be cool if you could make a 2s4p module, where the other half is fitted for a small bms!
```

---
## \#197 Posted by: lock Posted at: 2018-06-12T13:21:16.317Z Reads: 341

```
[quote="agniusm, post:194, topic:36847"]
Battery negative and common negative are linked internally I was told, so you can use either.
...
Mockup is with other end connector plugged in so there should be space for balance wires.
[/quote]

yeah, you're right on both counts, I probably should have looked at the schematics. I still have my doubts on the sense wires though, but I'm sure you'll figure something out.

Guess I'm not as concerned about holes as I can't imagine anyone would use NESE modules without them being inside another larger enclosure anyway. But in principle, fewer the better.
```

---
## \#198 Posted by: agniusm Posted at: 2018-06-12T13:52:07.603Z Reads: 340

```
I can make access for USB no issues and if you say its fine, i'll do it. CAN cables could be routed through the openings i was referring to earlier.
BMS still could be pushed to the left some to allow for more clearance. It will be more space there, i just used standard module enclosure without modifications.
About that momentary switch. Do i need to get that built in(if space allows) or are they mounted on external enclosure?
I have asked to include me on the second run list to get BMS and have physical object to test fit. I think i will get it by the end of the summer if enough people come on board.
@uigiroux, i will concentrate on these two additions. If i will start wander about, none will be done ;)
```

---
## \#199 Posted by: deucesdown Posted at: 2018-06-12T13:54:37.119Z Reads: 330

```
Lovely. No worries about heat from the mosfets softening the enclosure?
```

---
## \#200 Posted by: uigiroux Posted at: 2018-06-12T14:14:52.484Z Reads: 329

```
Perhaps a thin heat sink could be placed at the bottom of a module?
```

---
## \#201 Posted by: TheMachine Posted at: 2018-06-12T15:49:33.231Z Reads: 336

```
Very interested in the 2s4p modules, are they going to be a semi-permanent offering?
```

---
## \#202 Posted by: banjaxxed Posted at: 2018-06-12T16:07:32.131Z Reads: 326

```
You can just thermal glue a piece of aluminium or PC-type heatsinks to the FETs if concerned about heat with high discharge
```

---
## \#203 Posted by: ducktaperules Posted at: 2018-06-12T23:04:00.525Z Reads: 322

```
These packs look awesome :)
```

---
## \#204 Posted by: Benjamin899 Posted at: 2018-06-12T23:18:41.732Z Reads: 316

```
so am i right that this 2s4p module has one 8P tab and two 4P tabs ? or how is it constructed. btw is this now avbailable for everyone? Just to clarify
```

---
## \#205 Posted by: boardman Posted at: 2018-06-12T23:51:12.968Z Reads: 320

```
Is there any way to wire this up into a 4s2p configuration?
```

---
## \#206 Posted by: Benjamin899 Posted at: 2018-06-13T00:30:40.973Z Reads: 321

```
just buy the 2p modules, but to your question. I don't think there is a reasonable solution without changing the design completly.
```

---
## \#207 Posted by: uigiroux Posted at: 2018-06-13T02:17:53.146Z Reads: 313

```
As a single unit by itself it has one 8p and two 4p tabs, but as a whole unit for a 12s4p, it's got twenty two 4p tabs, and one 8p tab.
```

---
## \#208 Posted by: uigiroux Posted at: 2018-06-13T02:24:35.415Z Reads: 316

```
I think that absolutely could be done, so you'd need three modules to make a 12s2p system.  Just draw out three dual sided 8p modules, and you'll see what you would need to make it work :slight_smile:  That's another reason I like this design is you can expand beyond just the 12s4p if you add two 6p (12s1p) modules or three 8p (12s2p) modules.
```

---
## \#209 Posted by: agniusm Posted at: 2018-06-13T04:00:08.206Z Reads: 332

```
@TheMachine Yes, i think they will be permanent.
@Benjamin899 Its on the shop ATM, description and other bits on the website are not filled yet though.
@boardman In theory you could do 4S2P but it will be impossible to nicely route sense wires inside the module. There would be loose bits like 2P tabs to be inserted one by one with cells holding them. As Benjamin899 mentioned, needs heavy alteration of the design or heavy DIY.
So for the design as it meant to be, best we can have is 2S4P. It has full tabs which are not cut and soldered, they are all constrained on one end at least. Even 2S4P needs full tab to be bowed out to be inserted which is fine.
```

---
## \#210 Posted by: boardman Posted at: 2018-06-13T07:32:06.102Z Reads: 325

```
I see. Thanks for the detailed response
```

---
## \#211 Posted by: agniusm Posted at: 2018-06-13T13:32:52.033Z Reads: 353

```
OK. Reworked 2S4P module for the BMS. Added access to USB(not keen on it. The hole must accommodate whole USB connector with casing which makes it big. If i push it to the wall it will still be not enough to reach as enclosure walls are thick and it wont allow for tabs). I think it would be better to use extension cord and route it out along with OLED, switch wires:

[img]https://i.imgur.com/tOuWEsf.jpg[/img]

[img]https://i.imgur.com/bL3bYj7.jpg[/img]

Grey grommets are where the wires would enter. They will be made out of softer TPU material.
I don't know if the angled grommet is needed.
Some good news is that i was offered a BMS from the first batch to advance with this faster so it just might happen sooner than i thought. Great
```

---
## \#212 Posted by: banjaxxed Posted at: 2018-06-13T15:04:43.832Z Reads: 325

```
Nice will you make an STL available when happy on 18650.lt ?
```

---
## \#213 Posted by: agniusm Posted at: 2018-06-13T15:29:53.022Z Reads: 332

```
Sure mate they will be available. Just need to iron out so its 120% ;)
```

---
## \#214 Posted by: OLnewB Posted at: 2018-06-14T02:40:28.694Z Reads: 343

```
@agniusm @uigiroux I don't understand, what is the goal with these 2s4p modules?
```

---
## \#215 Posted by: banjaxxed Posted at: 2018-06-14T04:36:26.402Z Reads: 348

```
![image|341x307](upload://Ae0rSpIVGPsYo94EMCOstRrrLxW.jpeg)
```

---
## \#216 Posted by: agniusm Posted at: 2018-06-14T10:29:07.830Z Reads: 344

```
1. Less modules to mount
2. Smaller overal size
3. Less series connections outside the enclosure.
If you dont need it there are 4P modules still available.
Would you not agree that broader choice is better? You might not need it but the world is bigger than that and some might benefit.
```

---
## \#217 Posted by: uigiroux Posted at: 2018-06-14T12:36:27.739Z Reads: 355

```
They make it so you can use 6 modules rather than 12 since both sides have screw terminals.  So I'm using 22 single sided 4p tabs as the pic illustrates, and then 1  8p tab that doesn't need any screw tabs, as shown in the bottom module in the pic. 

![20180614_073728|387x500](upload://vH7ycib2GrvmMpWkRTNdQTaxK4X.jpg)

Let me know if you have any questions :smile:
```

---
## \#218 Posted by: OLnewB Posted at: 2018-06-14T16:12:11.372Z Reads: 347

```
@agniusm, thanks. I get it now. I went back and looked more closely. Five modules to make a 10s4p battery, and the pack will be 375mm x 167.1mm x 22mm (14.75 inch x 6.57 inch x .86 inch) instead of 10 4p modules at 375mm x 195mm x 22mm (14.75 in x 7.75 in x .86 in). @uigiroux, thanks for the drawing. I've been following the developement of NESE modules all along. I was thinking about doing a 10s3p pack because of the width of the 4p modules. This design saves some space!
```

---
## \#219 Posted by: uigiroux Posted at: 2018-06-14T16:23:31.877Z Reads: 334

```
That was exactly why I wanted a double sided unit, it saves space and cuts the number of modules you need in half.  Only down side is it can only go up to 8p, where as I'd of preferred to make a 12s5p battery, but I guess 8 is a wide as they can go, I was told 10 couldn't be done cause it would maybe start to bow or flex a bit in the center.
```

---
## \#220 Posted by: OLnewB Posted at: 2018-06-14T16:26:34.883Z Reads: 333

```
Yes, I wonder about the flex because my deck has a large amount of concave. With a router one could make a flat spot for the pack if necessary.
```

---
## \#221 Posted by: OLnewB Posted at: 2018-06-14T16:32:58.342Z Reads: 330

```
Are the 4p bus bars as secure in the 8p modules? I was impressed by @agniusm monster shake test videos on his modules with the continuous bus bars (tabs?) I know this is a beta product. Shake test?


 https://www.youtube.com/watch?v=93JBo87LJiU
```

---
## \#222 Posted by: agniusm Posted at: 2018-06-14T18:19:47.029Z Reads: 324

```
@OLnewB, tabs inside are constrained same as on all othe modules. Cell "cradle" does not allow them to move anywhere other than .5mm that is left for error.
BTW, you can call them finished. I have betas sitting on my desk and @uigiroux will get first set of finished product.
```

---
## \#223 Posted by: agniusm Posted at: 2018-06-14T18:33:39.301Z Reads: 333

```
On the flex. The flex uigiroux was reffering to is in modules, lengthwise, not the deck. The more cells, the more bow as there is special foam which adds pressure with each cell, and its a lot of pressure. I would not go beyond 8P for that reason as it will be difficult to close the lid on the enclosure and sides would be too much stressed. I cant afford to have bad product. 1st of July going to be 1 year since i opened webshop and i had 0 returns, 0 negative emails from customers or mentions elswhere which i am proud of.

Just quoting myself from early postings on endless sphere on presure per cell:
"All the data of pressure on tabs is in earlier posts, its in SI units and if you are interested, convert them yourself online to whatever you like. I can repeat it here, 17-20 newtons / 2.54cm² or 1.73-2.03kgf/2.54cm²" if you are interested scientific motives on why no larger than 8P. Actually 8P is a bit of stretch as design was for 6P only.
EDIT: You can translate that as hanging 16 kilograms on one side of the module on 8P unit
```

---
## \#224 Posted by: OLnewB Posted at: 2018-06-14T21:36:51.192Z Reads: 315

```
Yes, I understand we are talking about the flex of the module. My deck is very concave on its width, not like these flat planks. It has almost no flex. If 8p or 2s4p modules are mounted across the deck, can they take a bit of a curve?
```

---
## \#225 Posted by: agniusm Posted at: 2018-06-15T05:40:54.932Z Reads: 307

```
Modules cant take any curve, they are rigid.
```

---
## \#226 Posted by: agniusm Posted at: 2018-06-18T07:09:05.038Z Reads: 300

```
I think i can add 2S3P and 2S2P modules to the line up. Should be fairly similar, only one end of the module will have hookup for sense wire instead of two like on 2S4P module.
```

---
## \#227 Posted by: banjaxxed Posted at: 2018-06-18T11:04:33.678Z Reads: 297

```
I AM going to finish fixing my 3D printer & complete the Puka build with your packs once this is out, thanks dude
```

---
## \#228 Posted by: XTLA Posted at: 2018-06-18T12:07:58.784Z Reads: 294

```
Yes please 😋
```

---
## \#229 Posted by: Benjamin899 Posted at: 2018-06-19T09:16:41.640Z Reads: 301

```
@agniusm can you solder wires directly to your Series Tabs you cell in your shop? Because you are out of Tube Ring lugs atm and i am too lazy to drive to the next store^^
```

---
## \#230 Posted by: agniusm Posted at: 2018-06-19T09:32:25.512Z Reads: 290

```
Yes. Its tin plated copper so very good for soldering. I guess you needed 6mm^2 and supplier was out of stock for them. Have to wait.
```

---
## \#231 Posted by: Benjamin899 Posted at: 2018-06-19T09:33:32.869Z Reads: 289

```
awesome thanks
```

---
## \#232 Posted by: Clanger Posted at: 2018-06-19T12:57:36.371Z Reads: 292

```
This is all going a bit over my head.

How would i make a 10s2p pack with a BMS using this kit?
```

---
## \#233 Posted by: uigiroux Posted at: 2018-06-19T13:00:02.958Z Reads: 299

```
If you just want 2p, then order 5 double sided 4p modules, they would be labeled 2s2p special order and say in the comments you want to use them for a 10s2p battery pack.
```

---
## \#234 Posted by: Clanger Posted at: 2018-06-19T13:08:44.472Z Reads: 300

```
These kits could be huge IMHO.

Simple instructional videos on how to assemble full pack properly and safely would definitely help increase the rate of adoption!
```

---
## \#235 Posted by: Benjamin899 Posted at: 2018-06-19T13:20:51.631Z Reads: 298

```
his first post is an assembly video. Many people who already have a spotwelder won't buy this, some still buy it for other reasons.
You basicly treat a module like you would treat a normal battery, nothing realy changes.
```

---
## \#236 Posted by: uigiroux Posted at: 2018-06-19T13:58:24.006Z Reads: 313

```
I think so too, I've been hoping these will take off.  I sold my spot welder once I ordered these.  Compared to the cost of buying a fully assembled battery, vs using these to be able to make your battery, and once the cells go bad you can simply swap it out, so it will be good forever essentially, lol.  The only thing I think would make these more desirable is if they could do 10, even 12 cells so that 5p and 6p batteries can be made.  Also it'd be cool if they could be adapted to use the new cell sizes 20700 and 21700, which I've been told they can easily be made to fit those, but the series tabs require a mold that costs like 2k or something, so he'd need enough orders to justify the cost of making the new molds for the copper and nickel plated series tabs.  Overall though, now that these can be made double sided, I think that is the biggest benefit to these!  Very convenient!
```

---
## \#237 Posted by: Benjamin899 Posted at: 2018-06-19T14:32:00.698Z Reads: 287

```
well and they are safer imo, there is just less chance of shorts from batteries which lost their wrap from rubbing ect. You want to switch from a commuter to a small fun board no problem with these.
```

---
## \#238 Posted by: uigiroux Posted at: 2018-06-19T14:38:51.848Z Reads: 295

```
Exactly!  Also like I've been saying this allows for unlimited battery sizes to travel on flights with.  Just disconnect the bus bars and have them add individual modules.
```

---
## \#239 Posted by: Benjamin899 Posted at: 2018-06-19T14:41:44.116Z Reads: 299

```
i just bought my 5x 2s4p, can't wait^^
```

---
## \#240 Posted by: Clanger Posted at: 2018-06-19T15:01:11.422Z Reads: 310

```
Once you guys build your batteries, can you post about how you wired the BMS up etc!

These things have me curious.
```

---
## \#241 Posted by: Benjamin899 Posted at: 2018-06-19T15:06:19.707Z Reads: 306

```
well you have positive and negative terminals on the modules and you can either use ringterminals for your balance wires or you solder onto the seriers tabs, as far as i know. Just like a normal pack where you solder between cells so not to dmg the cells.
```

---
## \#242 Posted by: uigiroux Posted at: 2018-06-19T23:03:19.855Z Reads: 281

```
Yeah I should have mine by tomorrow so I'll set it up and take pics.
```

---
## \#243 Posted by: Benjamin899 Posted at: 2018-06-19T23:07:00.460Z Reads: 296

```
do that, mine will come probably next week. every instruction for bms say you have to connect balance wires to the positive of every P group but i see many place them between cells even on series connections. Does it actually rly matter where exactly to place the contact point? I find the lack of specific manuals for bms kinda weird.
```

---
## \#244 Posted by: agniusm Posted at: 2018-06-20T06:24:02.357Z Reads: 322

```
All BMS/PCM wiring is mostly the same and sense wire goes on the series junction meaning on positive of one cell and negative of the other. It does not matter where you place the contact as its a junction. B- would go to first cell negative B1 would go to first cell positive and second cell negative series connection and so forth. Some BMS/PCM will not need first B- negative as its internally routed from main battery negative connection (thick wire).
I have here 2 more additions, 2S2P and 2S3P. That will conclude options i think.

[img]https://i.imgur.com/c0cpiqr.jpg[/img]

[img]https://i.imgur.com/0uCaqmM.jpg[/img]

Note how there is no contact in last photo on one side. Sense wire for BMS would have to be attached from the other side. I am still including nut and bolt to be there as a spare.
Rough dimensions:
2S2P 94x74x22mm
2S3P 131x74x22mm
```

---
## \#245 Posted by: agniusm Posted at: 2018-06-20T07:48:21.496Z Reads: 304

```
Webshop updated with new modules. I will update 3D model section this week, hopefully if i can get some time.
Just a reminder, 10 days left with summer discount which you can spend on BEER for battery builds ;)
```

---
## \#246 Posted by: tsr Posted at: 2018-06-20T08:09:22.146Z Reads: 299

```
I followed the discussion about the BMS, but I am still a little bit confused;) Does the Hardware set for e.g. 10s/3p you have on your site also include a module for the BMS? If not is there a set available that includes "all I need" for a complete battery (apart from the cells and the actual BMS)?
```

---
## \#247 Posted by: agniusm Posted at: 2018-06-20T13:40:50.867Z Reads: 298

```
No. There is no set. Its a mix and match type of shop. Its impossible to have each configuration for everyone, you'd be lost, and I will be doing only that, updating data :slight_smile: 
Hardware sets do not include enclosures. They are made for people who have 3D printers or access to them so they can print locally. 
I dont finished product for BMS yet.
You can drop me pm or email and I will help picking the right stuff for the battery
```

---
## \#248 Posted by: Xurok Posted at: 2018-06-20T14:21:52.838Z Reads: 289

```
I wish you had 10P tabs..
```

---
## \#249 Posted by: agniusm Posted at: 2018-06-20T16:56:00.312Z Reads: 281

```
I have updated my site and all new confirmed models are up. Let me know if you find any errors etc. Was kinda intense :D
```

---
## \#250 Posted by: banjaxxed Posted at: 2018-06-20T18:14:30.340Z Reads: 293

```
Will do muchos gracias
```

---
## \#251 Posted by: banjaxxed Posted at: 2018-06-20T18:19:16.135Z Reads: 308

```
Maybe just the mobile version are we discussing the bms case?, not at a pc  ![image|281x500](upload://rEEkebgYBrhInkj5cGliIKhreB1.png)
```

---
## \#252 Posted by: uigiroux Posted at: 2018-06-20T18:33:51.067Z Reads: 297

```
Like we just discussed in the pm about my order, maybe it would also be good to list 2p+2p, 3p+3p, and in my case 4p+4p.  Then you could explain or have a quick video explaining what they'll need to order if they choose any of the 2sXp, cause they won't need 5 or 6 of the 2s4p to make a 10/12s4p.  They'd need one 2sXp and then 4 or 5 of the Xp+Xp.  So for me making a 12s4p, I should have ordered 1  2s4p and 5  4p+4p.  Showing a drawing like I showed you could help too.  Package should be in today or tomorrow I think.  Can't wait!
```

---
## \#253 Posted by: agniusm Posted at: 2018-06-20T18:36:43.960Z Reads: 293

```
I think i got the grip now and a note will suffice. 
There are no BMS enclosures models yet. Only new modules. i am still waiting on BMS
```

---
## \#254 Posted by: Benjamin899 Posted at: 2018-06-20T18:39:40.123Z Reads: 290

```
i really want to thank you again for your dedication and openess for input, that is rare and i hope you have success now and in the future.
```

---
## \#255 Posted by: agniusm Posted at: 2018-06-20T18:41:10.355Z Reads: 284

```
Thank you. No worries, will try to deliver best to my ability ;)
```

---
## \#256 Posted by: agniusm Posted at: 2018-06-20T18:48:24.535Z Reads: 279

```
I think i will make a vid explaining stuff on a white board regarding these modules. Just need to get some time. Very busy lately with stuff i want to finish designing, website updates and more orders coming in. I even started thinking about SLS machine :D (just not yet i guess :D ), my printers start to lag :)
```

---
## \#257 Posted by: agniusm Posted at: 2018-06-20T18:54:54.911Z Reads: 277

```
@banjaxxed, i can compile stl's for you for the BMS prototype if you want, Have no problem with that if someone wants to experiment ;)
```

---
## \#258 Posted by: karma Posted at: 2018-06-20T19:39:33.231Z Reads: 275

```
Recieved your tabs and tested them out, they work fantastic! Great work! I will the the 2SXP models. What BMS is suppose to be in your BMS prototype?
```

---
## \#259 Posted by: agniusm Posted at: 2018-06-20T19:58:50.195Z Reads: 281

```
Great. How did the enclosures turned out and what material?
Its DieBieMS developed here on the forum. You can follow back up on this thread, i have rendering of it.
```

---
## \#260 Posted by: karma Posted at: 2018-06-20T20:37:53.043Z Reads: 303

```
The enclosure turned out great! I did the 4P version in [DAS FILAMENT orange PETG](https://www.dasfilament.de/filament-spulen/petg-1-75-mm/259/petg-filament-1-75-mm-leuchtorange?c=21) with the 5% infill, 0.2mm layer height and my settings for the material. Printed on a Prusa i3 MK3. The snap fit on this was god tier, really rigid. My printer is well calibrated right now so that also helped.

Also did a unintended crash test at around 30-35km/h onto hard asflat while having the module in my backpack and landing on my side (including the backpack smashing into the ground), the cells survived with out any noticeable damage, only the 3D printed Case broke.

Well fimiliar with the DieBieMS, trying to get hold of one myself :)'

![image|375x500](upload://uTsq5BzBTS24PLarF8D1vBwlwFk.jpeg)![image|375x500](upload://5SZX4DlmlQUDUYqWf1XS2XIv4L9.jpeg)![image|375x500](upload://6ZVCDs7qqRGSuPKpRF7dEwb8EIk.jpeg)
```

---
## \#261 Posted by: agniusm Posted at: 2018-06-20T21:46:10.494Z Reads: 303

```
You can print at 0.01% infill. Makes them a bit lighter and faster to print. Those vented modules are weaker due to the fact that they have lots of openings.
When you will reuse tabs, bend them back and heat up with blow torch, gas solderimg iron or on a gas stove(be careful with the one that has foam, dip it in a water so only heated part remains) It will return copper molecules to relaxed form again. When bending copper multiple times it becomes brittle and will break. This heating process will return it to previous state.
```

---
## \#262 Posted by: agniusm Posted at: 2018-06-20T21:48:23.216Z Reads: 308

```
BTW, hope you are fine. Crash at that speed aint funny at all
I had a crash far slower on my drift trike:
[IMG]https://lh3.googleusercontent.com/-qA_IAgPCpj4/VU-ml28OSEI/AAAAAAAAKcs/LfqJkckvU7o/s1024/20150510_185430.jpg[/IMG]

[IMG]https://lh3.googleusercontent.com/-6I1FWjXs0WA/VT3Uc21n1fI/AAAAAAAAKXQ/63Y00bzkpH4/s912/_DSC4330%25201.JPG[/IMG]
```

---
## \#263 Posted by: Benjamin899 Posted at: 2018-06-20T22:03:25.816Z Reads: 304

```
autsch that looks painfull
```

---
## \#264 Posted by: agniusm Posted at: 2018-06-21T10:21:00.724Z Reads: 306

```
DieBieMS enclosure prototype is up on site if anyone wants to try and print it.
http://18650.lt/index.php/resources/

Here is a video how 2S4P becomes 4P+4P:
https://youtu.be/plCNRt8FboY

@tsr something that will print PETG, ABS or PC. PLA is NO good.

P.S. I have 7 prototype modules i can sell at 10EUR/each, 65EUR for 7. They are same dimensions and only difference is that 4 of them are without mounting holes and 3 have D=4mm mounting holes. Otherwise same as complete ones with same size and function.
```

---
## \#265 Posted by: tsr Posted at: 2018-06-21T10:24:41.453Z Reads: 301

```
maybe a stupid questions, but I am thinking about buying a 3d printer next winter - is there any minimal requirement to print these modules?
```

---
## \#266 Posted by: banjaxxed Posted at: 2018-06-21T14:03:34.743Z Reads: 299

```
I was considering the creality cr10s but leaning towards tevo tornado now, better heating, afaik you can mod with auto level making it really good

Also consider the tevo black widow, very heavy strong frame giving super definition/accuracy

See GearBest.com
```

---
## \#267 Posted by: Benjamin899 Posted at: 2018-06-21T14:13:55.505Z Reads: 303

```
https://www.youtube.com/watch?v=2IE6hSQu4lI
 Check this guy out.
```

---
## \#268 Posted by: banjaxxed Posted at: 2018-06-21T17:14:11.305Z Reads: 303

```
The problem is the heatbed being 12v and the price, the tevo has great heat and you can as he said take care of smoothing fairly easily as well as auto leveling.

For esk8 you will probably at some stage want to look at printing Filiment which needs a very hot bed and full metal extruder (nylon, Pom and abs), the revue was a little biased towards flexible and the tornado has the hot end already for this, the tornado has an even better titan extruder and much larger build space.

My vote would be the tornado with minor mods -

Auto level kit
Maybe stepper driver smoothers (if settings tweaks don’t remove artifacts)

This
https://m.all3dp.com/1/tevo-tornado-upgrades-mods-3d-printer/


I would probably also look at the black widow for ultimate perfection with some mods and an enclosure
```

---
## \#269 Posted by: uigiroux Posted at: 2018-06-21T17:32:32.560Z Reads: 288

```
Got my order today, will post pics later.  Very happy with these, they look professional quality!  Great job!
```

---
## \#270 Posted by: uigiroux Posted at: 2018-06-21T17:33:27.984Z Reads: 286

```
Also is there a BMS module now?  I wasn't sure from the messages a few before this.  Can someone post the link so I can check it out, given it actually exists, lol.  Thanks yes!
```

---
## \#271 Posted by: tsr Posted at: 2018-06-21T19:10:46.172Z Reads: 274

```
Thanks for the tips - will check it out!
```

---
## \#272 Posted by: Benjamin899 Posted at: 2018-06-22T00:37:26.462Z Reads: 271

```
@agniusm how does the PETG react to normal Silicone sealant? I am thinking to use it to dampen vibration.
```

---
## \#273 Posted by: wafflejock Posted at: 2018-06-22T00:39:58.548Z Reads: 271

```
Pretty sure petg is what most coke bottles use so can probably test with that and get a rough idea.
```

---
## \#274 Posted by: agniusm Posted at: 2018-06-22T05:10:10.406Z Reads: 284

```
As said before i have nothing yet. I have uploaded 3D file for people to try if they have 3d printer.
You are first to know when its ready as you have paid for it ;)
```

---
## \#275 Posted by: agniusm Posted at: 2018-06-22T05:11:49.357Z Reads: 279

```
Most bottles are made from PET. Its just modified PET with G (ethylene glycol)  😁
```

---
## \#276 Posted by: agniusm Posted at: 2018-06-22T05:18:45.568Z Reads: 291

```
For example Ceresit does not recommend using silicone on clear plastics including PETG. I have not tested it against chemicals.
http://kmac-plastics.net/data/chemical/petg-chemical.htm#.WyyIOmqEbqA
```

---
## \#277 Posted by: Benjamin899 Posted at: 2018-06-22T13:32:35.085Z Reads: 303

```
yep did some research, gonna go the safe route and use a rubber sheet
ty for the answers
```

---
## \#278 Posted by: rsalmon Posted at: 2018-06-23T01:27:56.544Z Reads: 312

```
Hey @agniusm, check out this cool video using your modules.

https://www.youtube.com/watch?v=1y4zh5mAdzA
```

---
## \#279 Posted by: uigiroux Posted at: 2018-06-23T04:21:35.665Z Reads: 325

```
Got my order in, lacking the batteries, but thought I'd put it together so everyone can see what it looks like.  I love this!  12s4p :smile:![1529727598986923277177|374x500](upload://3m3ci38Li3q6Syc1rnwGEDeyx3G.jpg)

![15297276388541952418221|374x500](upload://8cXYhZdZ9ZgjMoi9GJ1h2eBYzSZ.jpg)
```

---
## \#280 Posted by: agniusm Posted at: 2018-06-23T06:16:53.372Z Reads: 312

```
Thanks. Have not seen this one. Jehu has one on twitch building 12v battery with my 8P modules
```

---
## \#281 Posted by: agniusm Posted at: 2018-06-23T06:20:36.035Z Reads: 320

```
Have you tried cutting tabs to fix them? Good thing is you can mount and wire you battery, then just pop in the cells when you het them :slight_smile:
Did i miss to put one single cap?
```

---
## \#282 Posted by: Westy Posted at: 2018-06-23T06:44:21.422Z Reads: 311

```
Do you have dimensions for the 2s3p packs? I think I'm gonna try to fit a 12s3p into Hummies board.
```

---
## \#283 Posted by: oyta Posted at: 2018-06-23T07:15:01.839Z Reads: 307

```
Nice! What are the dimensions? How do you fix it to your board?
```

---
## \#284 Posted by: Ronny_CTS Posted at: 2018-06-23T11:43:18.957Z Reads: 303

```
From how i see it, the way you connected those series tabs will not give you a 12S4P configuration. It will either give you a 2S12P battery, a 8S6P  battery or a fire. You need to remove some of those series Tabs as you are connecting in series and parallel simultaneously.
```

---
## \#285 Posted by: uigiroux Posted at: 2018-06-23T13:53:24.462Z Reads: 298

```
Yes I know, I just wanted to see what it would look like put together.  Right now it's 6 2s4p module, I'm going to keep one for the bottom, then the top five will be 4p+4p, so believe me, I've got it covered :wink:
```

---
## \#286 Posted by: uigiroux Posted at: 2018-06-23T13:56:08.155Z Reads: 292

```
Didn't cut tabs yet, just put together so far.  Today I'll cut the series tabs in half though.

Yeah I see too be missing a cap lol. Oh well..
```

---
## \#287 Posted by: agniusm Posted at: 2018-06-23T14:25:33.075Z Reads: 292

```
Go to website please. Resource page will give you all information needed.
```

---
## \#288 Posted by: Ronny_CTS Posted at: 2018-06-23T16:12:14.708Z Reads: 308

```
Why are you cutting the tabs? Why not connect the 2S4P packs in series until you reach 12S.
```

---
## \#289 Posted by: agniusm Posted at: 2018-06-23T17:52:12.671Z Reads: 324

```
Cause he would need long bus bars and all will be messy. If you would stick them on the sides, sure, and still, depending on where you want your power output to be, on one side, or opposite ends.

Have not posted these photos i have. It was failed print but it shows how everything works inside:

[img]https://i.imgur.com/EdHhQHu.jpg[/img]

[img]https://i.imgur.com/ZpGEyBm.jpg[/img]

[img]https://i.imgur.com/ZYtgGsP.jpg[/img]
```

---
## \#290 Posted by: uigiroux Posted at: 2018-06-23T18:11:53.490Z Reads: 307

```
Let me make a drawing to show what I'm doing.  One sec.
```

---
## \#291 Posted by: uigiroux Posted at: 2018-06-23T18:31:44.475Z Reads: 319

```
![15297787241456945072458337439741|375x500](upload://2GQprJFuk8EeK3lm9wxLk61ew7c.jpg)

![15297787658586503353117884756780|375x500](upload://6nsYfrdchUATVwL3bSi73ONXlni.jpg)


![15297786496133488424630959312969|375x500](upload://bw6Km9eCj80hobuW9knOdxH4JCq.jpg)
```

---
## \#292 Posted by: uigiroux Posted at: 2018-06-23T18:56:27.571Z Reads: 321

```
Just made my first cut and it looks great! ![1529780071308623363110673728534|375x500](upload://pBTtlzosqgOJ3wL0PjlIk6p9WRP.jpg)![15297801589598846646313746910062|375x500](upload://hrphdBLLBGuSuaOLQ10VYLfYm6U.jpg)
```

---
## \#293 Posted by: XTLA Posted at: 2018-06-24T01:24:04.891Z Reads: 316

```
I’ve made my order for 10S3P also with that configuration

1x2s3p and 4x2s3p(with 3p+3p mode)

👌
```

---
## \#294 Posted by: jens_c Posted at: 2018-06-24T07:38:45.625Z Reads: 313

```
is there any way i can have the cad files of P N.E.S.E?
```

---
## \#295 Posted by: agniusm Posted at: 2018-06-24T08:35:47.868Z Reads: 313

```
Sorry, but those are not available.
```

---
## \#296 Posted by: agniusm Posted at: 2018-06-24T09:56:31.898Z Reads: 320

```
I have received my test sample of PCM i was thinking integrating with NESE earlier. What i like about them is that they are 2 wire units. Also, they are waterproof(i would say splashproof). Not expensive units also. I am talking with the manufacturer to get dimensions for different one, ones could fit NESE enclosures. Perhaps i will have a complete NESE BMS module, plug&play.

[img]https://i.imgur.com/up2O56l.jpg[/img]
```

---
## \#297 Posted by: agniusm Posted at: 2018-06-25T19:48:26.433Z Reads: 314

```
Any one fancies another no solder 18650 from India? Why for F... sake battery needs a hammer or log for assembly? Its like the thing now. Whack it with a hammer or something heahvy.
https://youtu.be/qL2QUgm5gS8
I need to make biased video why Whoosend and the likes are not such a good idea, at least not the market they aim for. 
Another thing they say, its easy to swap a cell? How the f..ck it can be easy? If you have 36v 4s, thats like 80 nuts to undo. Unlucky if the cell is in the middle.
```

---
## \#298 Posted by: Benjamin899 Posted at: 2018-06-25T20:00:54.335Z Reads: 305

```
yeah i wanted to buy vruzend, but decided against it, just too big and unreliable. It is realy just for stationary use at best.
```

---
## \#299 Posted by: banjaxxed Posted at: 2018-06-25T20:11:40.989Z Reads: 296

```
I bought their kit. tried to make it high capacity then just shelved it, I found it too...well crap 💩 

Maybe a powerwall or scooter but it's just not good enough for esk8. There is a version 2 I believe but my hands say no to this forever
```

---
## \#300 Posted by: uigiroux Posted at: 2018-06-25T20:11:48.642Z Reads: 295

```
I thought 'battery blocs' were a good idea, but they didn't offer the size and shape I wanted.  These are the best solution by far IMO.
```

---
## \#301 Posted by: karma Posted at: 2018-06-25T20:48:25.841Z Reads: 305

```
I also bought some Vruzend and tried but damn that felt like 💩. The metal ”spring” which is s bent metal piece didn’t make good contact and assembly was HARDER then spot welding imo.

Trird the NESE and it feels more rigid, super easy to make and good electrical connection.
```

---
## \#302 Posted by: Benjamin899 Posted at: 2018-06-25T20:50:00.083Z Reads: 291

```
it was always odd to me with vruzend and that bend metal contact
```

---
## \#303 Posted by: Blitz Posted at: 2018-06-25T20:58:31.777Z Reads: 290

```
These are a little pricey It kinda makes a spot welder look like a good investment. 
I'm open to mind changers.
```

---
## \#304 Posted by: Benjamin899 Posted at: 2018-06-25T21:03:41.759Z Reads: 296

```
Advantages:
You want to change a single cell, no problem
You want to make a smaller battery, ez reduce the P number or take a module away
You want to reuse the cells somewhere else, ez no spotweld no dmg
You want protection for cell, it is already inklusiv
```

---
## \#305 Posted by: karma Posted at: 2018-06-25T21:05:07.432Z Reads: 295

```
If you are saying the NESE system is expensive I would say the opposite. If you 3D print the enclosure which is the intended you only buy the strips it’s about 50€ + 2€ for nuts and bolts for a 10S4P. Easy assembly and no real learning curve. A spot welder costs around 200€ (+ 40-60€ for a battery) for a decent + nickel + glue and on top of that you got a decent learning curve to make good welds.
```

---
## \#306 Posted by: Blitz Posted at: 2018-06-25T21:09:42.863Z Reads: 297

```
I don't have a 3d printer And I don't know anyone who does.
and a spot welder from china is like 150.
And I get china can have a long shipping time
but for someone who has lipos and is looking to upgrade in a year it's no issue.
```

---
## \#307 Posted by: moon Posted at: 2018-06-25T21:13:30.687Z Reads: 291

```
If your spot welder breaks your screwed, if it comes from China that it is.

If my budget spot welder doesn't work, which it should I would buy these modules as a second best alternative
```

---
## \#308 Posted by: uigiroux Posted at: 2018-06-26T03:21:29.282Z Reads: 287

```
Another advantage, you can fly with any sized battery using these!
```

---
## \#309 Posted by: skatardude10 Posted at: 2018-06-26T04:11:27.010Z Reads: 305

```
You can get some relatively cheap and solid printers these days. You need to start somewhere, and if you plan to print nese cases, this would be a great project to start with. There is a slight learning curve, but it's not difficult to get the hang of. I honestly didn't know what I was going to end up printing when I first got mine a little over a year ago, but hundreds of projects later and it has by far paid for itself in utility alone, not to mention if I sold anything (which people will pay good money for one off custom printed parts, I get requests all the time) I would recoup my investment that much faster.

I had no projects in mind when I got my printer, I just knew it would be useful. I've made computer parts, all sorts of adapters for tools, hangars, decorations, designs to solve leaky wet things, film rollers, spacers, tools themselves, mounts for so many things that would have been inconveniently placed in a drawer or bundled up on the floor, skateboard risers, inserts, washers, fly swatters, toys for the kids, decorations for the wife, parts for firearms, basically anything. As time goes on you will find way too many things that are just too easy to either download or take 5 minutes and a set of calipers to draw up your own solution and hit print. If you really want nese, this would be a great project to get you into printing, as unlike many people, your first project will be an awesome and legit useful project instead of a test cube or something while trying to figure out what you could make instead.
```

---
## \#310 Posted by: agniusm Posted at: 2018-06-26T06:30:25.227Z Reads: 287

```
I hear very good things about creality ender 3 and its 170eur at gearbest with shipping atm. I think 3d printer is so much more than a spotwelder and is a must for the maker not even talking about nese.
3d printer is what allowed me to design and prototype nese. Before i would spend tons of time and money in cnc shops for prototypes. My prusa mk2 cost me as much as 3 prototypes i paid for before so it made sence.
```

---
## \#311 Posted by: uigiroux Posted at: 2018-06-26T10:19:27.588Z Reads: 285

```
I just watched a 3d printer comparison, and they above all recommended the Creality CR-10, or the CR-10S.  They start at like $360 for the CR-10 and $460 for the CR-10S.
```

---
## \#312 Posted by: moon Posted at: 2018-06-26T10:55:24.537Z Reads: 279

```
Wait you can? Thats sick!
```

---
## \#313 Posted by: uigiroux Posted at: 2018-06-26T11:21:04.432Z Reads: 285

```
Which comment are you referring to? Lol :smile:
```

---
## \#314 Posted by: moon Posted at: 2018-06-26T11:21:23.261Z Reads: 279

```
you can fly with any sized battery using these!
```

---
## \#315 Posted by: Benjamin899 Posted at: 2018-06-26T11:25:55.062Z Reads: 286

```
well you just need to seperate them as far as i understand
```

---
## \#316 Posted by: uigiroux Posted at: 2018-06-26T11:37:21.299Z Reads: 293

```
Yeah that's what I meant. :smile:
```

---
## \#317 Posted by: agniusm Posted at: 2018-06-26T12:51:15.775Z Reads: 286

```
I bought cr-10 s4 (400x400). Then i could not get a print out of it. Then i threw some 2k on it and now it prints non stop modules for you :)
Ender 3 is smaller, less chance for bed to warp so i think its cool little one. I might pick one up.
```

---
## \#318 Posted by: karma Posted at: 2018-06-26T18:03:16.355Z Reads: 281

```
At that price I feel like I am robbing them. The parts costs more if I would buy them O.o. I can recomend the Prusa i3 MK3 if you got the money for it. Then you can print some materials with better properties for our applications (heat, toughness, etc). 

@agniusm what printers do you own and what's your fav?
```

---
## \#319 Posted by: agniusm Posted at: 2018-06-26T18:50:20.026Z Reads: 283

```
Yeah, the price is crazy low.
I have prusa mk2 converted to zaribo edition with quick disconnect at the head and the creality cr 10 which is no more creality. Quality linear rails all round, e3d titan aero, duet wifi mobo with touchscreen, precision milled 8mm aluminium bed with keenovo 220v heater. Its a monster and i like it most. I built it and it performs like a dream with 410x420 bed. I could print PEEK or PEI if i needed to :)
```

---
## \#320 Posted by: strattos Posted at: 2018-06-26T19:10:22.910Z Reads: 281

```
You can build a really nice spot welder for pretty cheap honestly. Get a timing board from China for 20 bucks and find an old microwave transformer. I've had 0 issues with my homemade spot welder. (seriously it took me longer practicing welding than it did to build this thing and it costed me under 50 USD.

I'm gonna do a write up here on it sometime but in my opinion it's a better product than a sunkko or any hobby type spot welder, more adjustability. 

And I can do roughly 600 welds before I need to give the machine a rest to cool down a little, I'm sure I could keep going but at that point i wanna clean the pack and stuff.

Sorry for hijacking the thread but I really liked the idea of these but considering I don't own a 3d printer the cost was just to high to justify, especially when you're doing 2 12s4p packs.
```

---
## \#321 Posted by: Benjamin899 Posted at: 2018-06-26T19:13:22.326Z Reads: 267

```
cool, would like to read that. Hope you make a nice guide.
```

---
## \#322 Posted by: strattos Posted at: 2018-06-26T19:16:05.177Z Reads: 263

```
This community is so incredibly helpful I'd like to give back to you guys somehow!
```

---
## \#323 Posted by: Benjamin899 Posted at: 2018-06-26T19:17:20.405Z Reads: 274

```
i have seen some microwave spotwelder, which is the same as a Sunkho, but i dont have a car battery and used ones are also expensive.
```

---
## \#324 Posted by: strattos Posted at: 2018-06-26T19:25:08.964Z Reads: 285

```
Just Pm me if ya have any questions mate I'll try to get that guide up sometimes on but it's probably at least a couple weeks away. More than willing to send ya some photos and get ya started on the right track!
```

---
## \#325 Posted by: agniusm Posted at: 2018-06-26T19:42:28.371Z Reads: 307

```
Spotwelding is a bit like walking on a razorblade. Too little and its not enough, too much and you have electrolire siphoning. I built mine with arduino and just scrapped it.

https://youtu.be/5sSYZJCsT9s

https://youtu.be/f9px9VdmrD0

https://youtu.be/n02m0h_oGho

Maybe you spend more on the kit, but calculate how much time will you spend toying about getting spotwelder, all the supplies and then welding and assembling the pack. OK if its your thing and you like doing that but price your time at 10eur/h and i can tell you, it will look dirt cheap to get NESE and spend the rest of your saved time with family or friends ;)
```

---
## \#326 Posted by: karma Posted at: 2018-06-26T21:53:54.016Z Reads: 295

```
That is really interesting! A pneumatic approach, I have only seen that in professionals spot welders. Have you open sourced it or wrote more about it?
```

---
## \#327 Posted by: agniusm Posted at: 2018-06-26T23:17:40.046Z Reads: 299

```
There is some on endless sphere. I did not pursue that route. Went the other direction i saw more benefit in, for me and diy'ers. Before NESE i had a system developed for A123 20AH pouch cells sold on ES, then Chinese company OSN power copied it and it was cheap, but crap. I have some bikes made, remote lawnmoower with cameras and all that. The design os not out of the blue, i do have a bit of experience here and there :slight_smile:
All the stuff i did is documented on endless sphere. If you put my nickname in search it should bring my threads
```

---
## \#328 Posted by: RazzleDazzle Posted at: 2018-06-27T23:27:16.529Z Reads: 291

```
i liked the 3d printed enclosure, what I dont get about these N.E.S.E's is what the bus bar looks like, does someone have a link where i can get them or what they look like?
```

---
## \#329 Posted by: Benjamin899 Posted at: 2018-06-28T09:18:20.846Z Reads: 285

```
@agniusm Nice my modules came today, everything is there and you even precut and installed the tabs, thanks for that. Surprised how smooth they feel.
```

---
## \#330 Posted by: agniusm Posted at: 2018-06-28T10:00:40.707Z Reads: 294

```
The tabs could be seen at www.18650.lt shop. 
Good news Benjamin. Glad you like them. I sell them assembled like that so its even faster to assemble them :)
```

---
## \#331 Posted by: agniusm Posted at: 2018-06-28T11:15:34.495Z Reads: 302

```
Customer from France ordered some 8P modules for 58ah 12V battery with custom color. I think they look sweet:
[img]https://i.imgur.com/oWaIV33.jpg[/img]
```

---
## \#332 Posted by: agniusm Posted at: 2018-06-28T13:25:09.815Z Reads: 296

```
I bit tje bullet and got myself ender 3. If i can get it to work reliably with 60eur< aditional investment, i might be up for a small farm. Got it for 160eur with faster shipping 


2 DAYS LEFT FOR SUMMER DISCOUNT
```

---
## \#333 Posted by: Benjamin899 Posted at: 2018-06-28T15:43:16.725Z Reads: 296

```
@agniusm what do you think is better for the balance cables of the bms, to squeeze them between the tab and bolt or rather solder them onto the seriers tabs between each module?
```

---
## \#334 Posted by: agniusm Posted at: 2018-06-28T16:15:38.159Z Reads: 293

```
Mostly i avoid soldering if i can and use uninsulated terminals crimping them. I also avoid making pressure contacts :) Sorry but i dont know which is better. Probably if you solder wire in the middle and use some heatshrink? I had some ring terminals in the shop for that. I use them all the time as its easy to take them off.
```

---
## \#335 Posted by: Benjamin899 Posted at: 2018-06-28T16:22:30.531Z Reads: 285

```
ok thanks, just wanted to know what you would prefere
```

---
## \#336 Posted by: sami Posted at: 2018-06-28T20:32:59.865Z Reads: 278

```
I just got the exact same printer and it is printing perfect... Best printer for the price
```

---
## \#337 Posted by: uigiroux Posted at: 2018-06-28T20:48:26.576Z Reads: 285

```
I was considering one of the CR-10S models, but now I think I want to spend a bit more and get a Prussia i3 MK3.  Seems like a step up, though it doesn't have the same print size as the S4...  that is really a nice feature...
```

---
## \#338 Posted by: Benjamin899 Posted at: 2018-06-29T11:39:07.294Z Reads: 280

```
@agniusm hey i have a hard time pushing the printed caps unto the terminals, is that normal for the first time
```

---
## \#339 Posted by: agniusm Posted at: 2018-06-29T12:50:24.989Z Reads: 277

```
They are hard :) They are designed so they act as a secondary protection for screws to stay tightened. If its impossible for you, maybe some hot water will help.
```

---
## \#340 Posted by: Benjamin899 Posted at: 2018-06-29T12:54:28.978Z Reads: 278

```
ok i will start with some semi hot water or a little bit of hot air from the hairdryer
```

---
## \#341 Posted by: skatardude10 Posted at: 2018-06-29T13:27:52.592Z Reads: 284

```
Sometimes what I like to do is (use pliers) hold the offending nut, heat it up a bit with a lighter, then screw it in. It will melt the plastic just a bit and slide right in permanently, basically. Only heat it up a tad bit, just as much as you need to get the plastic around it slightly pliable. Be careful doing this as you can throw off other dimensions easily.
```

---
## \#342 Posted by: uigiroux Posted at: 2018-06-29T14:14:40.058Z Reads: 275

```
Lol yeah my fingers were soar after putting those on!
```

---
## \#343 Posted by: Itsmedant Posted at: 2018-06-29T18:44:53.536Z Reads: 274

```
Thats pretty close to the printer I have (Wanhao Duplicator I3)

From what I've learned so far, the best upgrade I've done is throwing a glass bed on there. I bought a 8x10 inch frame and just took the glass out and used some binder clips. Spray some hairspray on the glass before the print and now everything I'm doing is turning out really great!
```

---
## \#344 Posted by: moon Posted at: 2018-06-29T21:35:53.174Z Reads: 277

```
My wanhao i3 broke the other day.

They use pretty cheap connectors for the mainboard and my hotend connector burnt out and ruined the pcb. So probably need to replace it or buy something else.

Just lucky I was there whilst it was printing since there was smoke coming out of it
```

---
## \#345 Posted by: agniusm Posted at: 2018-06-30T07:27:15.168Z Reads: 271

```
You guys probably have not held a shovel in your hands :smiley:
I will print next batch 101% size.
```

---
## \#346 Posted by: agniusm Posted at: 2018-06-30T07:29:08.038Z Reads: 271

```
I dont like glossy finish when printing on glass. I will use it when I will print my cargo ebike tail lights.
I print on satin finish PEI.
```

---
## \#347 Posted by: uigiroux Posted at: 2018-06-30T08:53:46.745Z Reads: 267

```
Haha, oh that's not true, I've done a LOT of manual labor...  I was able to get them all on, but it was just damn difficult lol :wink:
```

---
## \#348 Posted by: Itsmedant Posted at: 2018-07-02T16:34:57.479Z Reads: 273

```
There is a fix for that, its only 9 bucks! It runs the power through a separate mosfet. If you end up getting the same printer there is a huge facebook group and thats the first mod they recommend before you even start using the printer!
```

---
## \#349 Posted by: moon Posted at: 2018-07-02T16:37:15.966Z Reads: 274

```
Yes but I cant fix if the PCB is burnt
```

---
## \#350 Posted by: Itsmedant Posted at: 2018-07-02T16:45:28.073Z Reads: 277

```
You can buy the PCB from Uncle Chuck

http://www.unclechucks3dprinterstuff.com/di3%20printer%20parts%20oem.htm
```

---
## \#351 Posted by: moon Posted at: 2018-07-02T17:08:55.352Z Reads: 270

```
Yes I am planning on buying that or just buying a new one and keep the wanhao as spares- or just sell as spares
```

---
## \#352 Posted by: Itsmedant Posted at: 2018-07-02T17:13:25.153Z Reads: 269

```
The new IS plus went up to 24v connectors on the hot bed so you don't have to worry about it anymore, its the one I got but I'm still going to do the mosfet upgrade just for piece of mind. I'm building an enclosure for it now for when i print PETG and ABS to keep the ambient temp up. 

Been doing nothing up upgrade prints so far and one N.E.S.E 4p holder, I gotta get it printing perfectly so I can get all of my enclosures good.
```

---
## \#353 Posted by: jens_c Posted at: 2018-07-03T14:44:02.558Z Reads: 267

```
strange i thought the N.E.S.E no solder module's were licenced under https://creativecommons.org/licenses/by-nc-sa/4.0/
```

---
## \#354 Posted by: agniusm Posted at: 2018-07-03T15:25:27.054Z Reads: 273

```
And they are, you can download 3d model files on site. Can i choose what i can opensource and what not? After all its my work and my chosen model of operation.
```

---
## \#355 Posted by: agniusm Posted at: 2018-07-04T07:46:01.290Z Reads: 291

```
Added a bit of improvement to 2S modules. I have designed in a through hole for a lid so 2 modules could be stacked for those mountain boards and bolted through to the deck. They are hidden inside with marks to drill them with 3.2 or 3.3mm drill bit:
[img]https://i.imgur.com/3hW14pL.jpg[/img]
Also added a notch so its easier to open the lid:
[img]https://i.imgur.com/TvVTnJf.jpg[/img]
BMS is paid for and should be shipped soon. Not long now.
```

---
## \#356 Posted by: banjaxxed Posted at: 2018-07-04T09:49:19.849Z Reads: 276

```
Gas! I got some bolts to help hold my packs on. And penny washers to spread the load across two packs.
But this is neater and only requires a drill, nice idea. I can use this on the inside end and use penny washers on the outside.

I bought 35mm M3 bolts for the job, but maybe 30mm would be better.

The notch is welcome, they are a little tricky on a good print
```

---
## \#357 Posted by: L3chef Posted at: 2018-07-04T10:07:30.178Z Reads: 261

```
A bit OT but is that colorfabb xt transparent filament?
```

---
## \#358 Posted by: agniusm Posted at: 2018-07-04T10:21:23.420Z Reads: 263

```
Devil Design transparent. Colorfabb would make enclosures more expensive.
```

---
## \#359 Posted by: L3chef Posted at: 2018-07-04T10:35:54.965Z Reads: 266

```
Okay :+1:Yes colorfabb is very expensive. Might have to pick up some devil design just to compare them both
```

---
## \#360 Posted by: visnu777 Posted at: 2018-07-07T10:20:29.351Z Reads: 278

```
My 10 3P N.E.S.E. arrived today and I already assembled two half of the final pack. 
It really worked like a charm but one thing I noticed: When you push in the cells it happened twice that the edge on the copper band cut open the plastic shell of the battery at the positive side and shortened the cell (incl. sparking) After that I tried to push it in a the positive side first which doesn't work that well but in the end i succeeded. I'm still convinced of this. Actually I have found a reliable battery builder who did my first battery pack but your NESE gives me a even better feeling about this.
```

---
## \#361 Posted by: agniusm Posted at: 2018-07-10T17:19:05.825Z Reads: 273

```
Yes, this might happen. That is why i always recommend using garolite gaskets for the positive no matter what you do, solder, spot weld. The PVC ring and heatshrink are too thin for mechanical protection.
As a side note, you place your cells positive end first at an angle. That way positive will not cut on tab and negative side does not matter.
I actually put cells naked, without any insulation and have just occasional sparks :)
```

---
## \#362 Posted by: agniusm Posted at: 2018-07-10T17:21:54.697Z Reads: 269

```
I have assembled some of the old stock in bulks with 40% discount.
1 set 3 x 2S4P with 2 extra lids
1 set 4 x 2S4P with 3 extra lid
1 set 3 x 8P
1 set 2 x 5P
http://18650.lt/index.php/product-category/discounted/
```

---
## \#363 Posted by: DAddYE Posted at: 2018-07-10T17:24:43.328Z Reads: 267

```
What should I buy to make a 12s2p?
```

---
## \#364 Posted by: visnu777 Posted at: 2018-07-10T17:28:45.953Z Reads: 265

```
Depends on how you want to arrange it, you could buy 6 2s2p cases.
```

---
## \#365 Posted by: agniusm Posted at: 2018-07-10T18:25:02.484Z Reads: 266

```
Or 12 2P cases, better 2S2P though
```

---
## \#366 Posted by: uigiroux Posted at: 2018-07-10T18:34:55.478Z Reads: 269

```
Ahh dude!  I really could have used this 40% off deal... :wink:
```

---
## \#367 Posted by: Benjamin899 Posted at: 2018-07-10T18:35:30.067Z Reads: 265

```
Who doesnt 😁
```

---
## \#368 Posted by: Hummie Posted at: 2018-07-10T18:56:57.917Z Reads: 274

```
[quote="agniusm, post:361, topic:36847"]
Yes, this might happen. That is why i always recommend using garolite gaskets for the positive no matter what you do, solder, spot weld. The PVC ring and heatshrink are too thin for mechanical protection.
As a side note, you place your cells positive end first at an angle. That way positive will not cut on tab and negative side does not matter.
I actually put cells naked, without any insulation and have just occasional sparks :slight_smile:
[/quote]

why not print a protector
```

---
## \#369 Posted by: DAddYE Posted at: 2018-07-10T19:01:26.239Z Reads: 260

```
Does it mean I’m getting 6 pieces to wire together? Wouldn’t it be giant?
```

---
## \#370 Posted by: agniusm Posted at: 2018-07-10T19:04:21.104Z Reads: 262

```
I dont remember all the sizes but it would be 22mm in height, 74x6mm in length and ??? in width (check website for exact sizes.

EDIT: The size would be 22x444x94mm
```

---
## \#371 Posted by: agniusm Posted at: 2018-07-10T19:05:20.776Z Reads: 260

```
They are first protos. No mounting holes of big mounting holes and i have just a set amount of them, no more :slight_smile:
```

---
## \#372 Posted by: agniusm Posted at: 2018-07-10T19:05:47.831Z Reads: 256

```
There still could be a second board for weekends :D
```

---
## \#373 Posted by: deucesdown Posted at: 2018-07-10T19:10:13.915Z Reads: 264

```
[quote="agniusm, post:372, topic:36847"]
second board for weekends
[/quote]

Sometimes it seems like everyone has all the days of the week covered, and need longer weeks ;)
```

---
## \#374 Posted by: ron Posted at: 2018-07-12T14:18:19.028Z Reads: 264

```
Spaß In understand these packs are printable by anyone? I am in the progress of making a Swappable Battery system for my Board which can be transported on plane for travel. These NESE modules go a little bit further by giving the possibility to exchange every cell when needed. So I want to print/modify these modules so that it fits 10S . So where do I get the additional Hardware, especially the nickel inserts?! Does someone have a link to AliExpress or other Chinese site? I searched and I couldn't find them. I only found separate cell caps. 

Thanks in advance...
Ron
```

---
## \#375 Posted by: Benjamin899 Posted at: 2018-07-12T14:21:11.775Z Reads: 254

```
It is in the hardware section.
```

---
## \#376 Posted by: ron Posted at: 2018-07-12T15:14:05.778Z Reads: 252

```
SO the nickel plated tabs are only available over his shop. ? 

Thanks in advance.
```

---
## \#377 Posted by: Benjamin899 Posted at: 2018-07-12T15:17:54.196Z Reads: 250

```
as far as i know yes.
@agniusm made them for his design, so i guess they are unique
```

---
## \#378 Posted by: ron Posted at: 2018-07-12T15:28:10.480Z Reads: 253

```
Thank you very much for the clarification! :)
```

---
## \#379 Posted by: agniusm Posted at: 2018-07-12T16:00:06.600Z Reads: 262

```
Ron, yes, the tabs are only sold by me. They are specific size and thickness for specific low set foam so under compression foam is compressed 50% +/-5%, to get best possible properties. It is tin plated copper, not nickel plated copper. Nickel makes copper brittle and i needed the tabs to be reuseable if the enclosure would get damaged.
Chinese might be pleasing with their pricing but that does not mean that QC and quality in general is better than what you pay for.
Buying from someone like me or other developer, helps us to continue doing our work and make it worth a while.
```

---
## \#380 Posted by: ron Posted at: 2018-07-12T19:03:55.135Z Reads: 272

```
Thanks for the answer. Yeah, I thought they are complete DiY so also the Tabs. Didn't know that you made them by yourself. Thought I could customize and hack it together for my special purpose. That's because I asked for the Hardwarelinks so I can order them in a bigger batch and can experiment with it.
And surely I would support such people which are providing something good for the community. :) .. Again, thanks for the answer.
```

---
## \#381 Posted by: visnu777 Posted at: 2018-07-14T17:57:52.454Z Reads: 280

```
Here is my final battery (10s3p, Sony Konion VTC6)

![newBattery|690x279](upload://4rrAYe00WBAQNfN1h3eRJOBdYv0.jpeg)

The Antispark Plug might be overkill here but I had nothing else at hand :)

I connected the two 5s packs with 16mm² solid copper wire, same goes for the XT90s on the left.
I soldered spare bus connectors to the wire so everything is still modular ;)

Greetings,
Michael
```

---
## \#382 Posted by: Eboostin Posted at: 2018-07-14T18:01:22.249Z Reads: 273

```
This looks so good! Would you mind sharing the overal dimensions of the finished pack?

@visnu777
```

---
## \#383 Posted by: visnu777 Posted at: 2018-07-14T18:02:39.602Z Reads: 270

```
of course, its 15,5x42x2,3cm (including XT90s) :)
```

---
## \#384 Posted by: mutantbass Posted at: 2018-07-14T18:09:16.406Z Reads: 263

```
What are people doing in terms of BMS on these packs?
```

---
## \#385 Posted by: visnu777 Posted at: 2018-07-14T18:12:07.210Z Reads: 264

```
You could put some cable shoes on the balance wires and fix them with the same screw that holds the bus connector. @mutantbass
```

---
## \#386 Posted by: ATLesk8 Posted at: 2018-07-14T18:53:05.644Z Reads: 263

```
How and where can I purchase a kit?
```

---
## \#387 Posted by: uigiroux Posted at: 2018-07-14T18:56:15.457Z Reads: 268

```
18650.it

That's where you can get them. I'd recommend getting one of the two sided modules, makes it a bit easier and you only have to use half as many as you normally would.  I've got a 12s4p worth these, it's great :slight_smile:
```

---
## \#388 Posted by: Benjamin899 Posted at: 2018-07-14T19:00:07.250Z Reads: 262

```
the upside of using the none double sided is for decks with alot of concave. other than that go for the double sided modules.
```

---
## \#389 Posted by: ATLesk8 Posted at: 2018-07-14T22:17:28.529Z Reads: 257

```
What are they called exactly? Im having a hard time here you'll have to forgive me.
```

---
## \#390 Posted by: Benjamin899 Posted at: 2018-07-14T22:30:16.019Z Reads: 262

```
http://18650.lt/index.php/product/n-e-s-e-module/
```

---
## \#391 Posted by: Eboostin Posted at: 2018-07-14T23:01:01.441Z Reads: 267

```
Does anyone have any better ideas for the connecting hardware? The current design is nicely protected but the bolts and plastic caps increase the width a good amount. 

Something like nylon or press together like legos, not sure, just thinking out loud
```

---
## \#392 Posted by: uigiroux Posted at: 2018-07-14T23:37:15.554Z Reads: 265

```
They do increase the width, but it's really only like 5mm combined for both sides so not that big a deal for me.  I was already going to have to modify my deck to use these, so an extra 5mm wasn't really much of a concern.
```

---
## \#393 Posted by: ATLesk8 Posted at: 2018-07-14T23:44:59.927Z Reads: 260

```
So should I go for 6 of the 2s4p packs for a 12s4p? How does this work. Newb battery builder here....also would it be smart to order any additional parts to assemble the pack from this site? Any recommendations are greatly appreciated
```

---
## \#394 Posted by: Benjamin899 Posted at: 2018-07-15T00:17:42.416Z Reads: 264

```
if you scroll up you see a nice diagram of @uigiroux showing how he placed them. And yes if you plan to build a 12s4p battery, you can get either 6x2s4p modules or 12x1s4p packs, depending on your deck.
```

---
## \#395 Posted by: uigiroux Posted at: 2018-07-15T00:46:55.202Z Reads: 263

```
To build a complete battery you need more than just the modules.  They have bus bars, tabs that cover the screws, etc.  In the comments section, you can ask that they confirm that you've gotten all you need to do the build you want.
```

---
## \#396 Posted by: Eboostin Posted at: 2018-07-15T01:03:23.000Z Reads: 260

```
Also, still very interested if you can figure out a 2s6p module. Trying to run 12 cells width wise and the more compact the better

@agniusm
```

---
## \#397 Posted by: Benjamin899 Posted at: 2018-07-15T01:11:11.596Z Reads: 256

```
he mentioned at some point that 8cells per module is the max, because of structural integrity reasons.
```

---
## \#398 Posted by: uigiroux Posted at: 2018-07-15T01:31:21.227Z Reads: 261

```
That's right.  I wanted ten wide for a 5p battery, but I guess at length over 8 cells there is the potential for warping of the modules.
```

---
## \#399 Posted by: Eboostin Posted at: 2018-07-15T02:05:13.958Z Reads: 267

```
I had already reached out to him directly and was told the same unfortunately

Edit: and would also be ok with two 1s6p in one case to save the extra material that two separate 1s6p cases would have
```

---
## \#400 Posted by: DAddYE Posted at: 2018-07-15T02:25:43.928Z Reads: 273

```
Does anyone a a pic of the 2s2p module?
```

---
## \#401 Posted by: Benjamin899 Posted at: 2018-07-15T02:37:30.156Z Reads: 286

```
http://18650.lt/index.php/2s2p-n-e-s-e-module/
explore his page^^
```

---
## \#402 Posted by: uigiroux Posted at: 2018-07-15T03:20:26.107Z Reads: 293

```
These are my 2s4p modules.

![20180711_155609|666x500](upload://9TNUZvbEUUFRPj0A0j76ppm5GrC.jpg)
```

---
## \#403 Posted by: uigiroux Posted at: 2018-07-15T17:32:45.824Z Reads: 289

```
Hey I was just looking at some batteries on NKON and they have two types of the Samsung 30Q's.  One is the normal kind, and the other has a button top for the positive terminal.  Are these made for the normal types like this:

https://ru.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html

Or for the botton tops like these:

https://ru.nkon.nl/samsung-inr-18650-30q-3000mah-button-top.html

The button tops go for a full euro more than the regular ones also.
```

---
## \#404 Posted by: visnu777 Posted at: 2018-07-15T17:36:59.018Z Reads: 278

```
Both are 65mm in length, which should be total length, so I think it will work.
It definitely works with the regular tops.
```

---
## \#405 Posted by: uigiroux Posted at: 2018-07-15T17:37:24.247Z Reads: 273

```
Meaning either of them would work?
```

---
## \#406 Posted by: visnu777 Posted at: 2018-07-15T17:39:21.651Z Reads: 268

```
Should, but lets wait for Agnius :)
```

---
## \#407 Posted by: Benjamin899 Posted at: 2018-07-15T17:44:34.612Z Reads: 269

```
the button top could be a problem, i wouldnt buy them for these modules.
```

---
## \#408 Posted by: uigiroux Posted at: 2018-07-15T17:54:24.120Z Reads: 274

```
Well that's good, that's an extra euro less per cell :smile:  can get them for $3.39 now.  Just hope shipping isn't crazy...
```

---
## \#409 Posted by: agniusm Posted at: 2018-07-16T06:39:44.100Z Reads: 282

```
The button top cells are same cells. They only have that nipple plate which could be removed. You will need to reshrink wrap the cell. If used with nese, garolite gasket could be placed instead and installed taking little extra care.
https://www.lygte-info.dk/info/battery%20protection%20UK.html
```

---
## \#410 Posted by: agniusm Posted at: 2018-07-16T08:47:13.918Z Reads: 287

```
Here are some packs in black:
[img]https://i.imgur.com/3SYQld6.jpg[/img]
```

---
## \#411 Posted by: Falcon87407 Posted at: 2018-07-16T22:42:53.658Z Reads: 280

```
How long does shipping usually take to the USA for just the hardware/tabs/screws etc.
```

---
## \#412 Posted by: trigger4point7 Posted at: 2018-07-17T08:43:28.924Z Reads: 286

```
Curious about this too, I ordered on July 4th. Curious of shipping time. I'm not in a huge hurry just want to know when to expect.
```

---
## \#413 Posted by: visnu777 Posted at: 2018-07-18T12:17:01.142Z Reads: 287

```
Integrated a 50A fuse and a connector for the Antispark-plug :)

![batteryplusfuse|333x500](upload://8oADuB7WTJiwJuR1h8oR3vYYZvj.jpg)
```

---
## \#414 Posted by: oyta Posted at: 2018-07-18T14:00:43.777Z Reads: 279

```
Nice. You should have had caps on the fuse screws as well 🙂 is that 10s4p?
```

---
## \#415 Posted by: Benjamin899 Posted at: 2018-07-18T14:11:36.686Z Reads: 282

```
Looks Like 3p.
```

---
## \#416 Posted by: XTLA Posted at: 2018-07-18T14:34:16.689Z Reads: 285

```
Got mine today 👌
![image|690x387](upload://mTkJCzF4f5yya6MAtUcdmguOAVC.jpeg)
```

---
## \#417 Posted by: visnu777 Posted at: 2018-07-18T16:18:09.802Z Reads: 280

```
It is 3p :) And of course will the fuse screws get a cap.
```

---
## \#418 Posted by: Itsmedant Posted at: 2018-07-18T16:59:41.640Z Reads: 283

```
Has anyone fully completed a build with these and a BMS? I just got all of my hardware and I'm starting to print my enclosures, I just want to see how everyone else is routing their stuff and mounting everything to a deck!
```

---
## \#419 Posted by: Benjamin899 Posted at: 2018-07-18T17:15:15.346Z Reads: 282

```
sadly i am still waiting on some other parts to finish my build.....it is frustuating
```

---
## \#420 Posted by: agniusm Posted at: 2018-07-18T19:24:58.356Z Reads: 285

```
@trigger4point7, @Falcon87407   Shipping across the pond takes just a few days. What i have noticed it gets bounced around in Chicago IL international distribution center. Someone in Chicago area or close by will get it faster. Someone farther away slower. All shipments end up in that sorting center. I provide shipping information through my site and paypal, so anyone who bought from me should have a copy on email. Check your spam if you don't. Check paypal order detais. You must have it
```

---
## \#421 Posted by: Kubbur Posted at: 2018-07-18T23:41:57.409Z Reads: 273

```
@agniusm no way of getting 1s10p single holster?
```

---
## \#422 Posted by: agniusm Posted at: 2018-07-19T09:57:39.453Z Reads: 269

```
Sorry. No way.
EDIT: I can print 10P holders, i can include 8P and 2P tabs, if you can diy them into 10P. But i am not responsible for these modules integrity nor i would like to get bad publicity. I can help if you want. Just tryimg to be a member of community here ;)
```

---
## \#423 Posted by: Eboostin Posted at: 2018-07-19T16:39:03.435Z Reads: 256

```
Can you print 12P holders? I don't need them to flex. 

How much room is saved on your 2S4P modules vs 2 separate 1S4P modules?
```

---
## \#424 Posted by: agniusm Posted at: 2018-07-19T17:19:14.487Z Reads: 261

```
Not much room is saved, couple mill. I can print them to the limits of the machine = 400mm
the tabs are in question. If you can DIY them to whatever P from 8P tabs you are good, on your own though. Not supporting that :D
```

---
## \#425 Posted by: uigiroux Posted at: 2018-07-20T13:53:06.753Z Reads: 268

```
Hey have you gotten a DieBieBMS yet to fashion a module as a case for it, or still working on it?
```

---
## \#426 Posted by: agniusm Posted at: 2018-07-20T14:13:48.865Z Reads: 266

```
Yes, its in the post office now. Have to pay additional 40eur import tax. It will be monday when i have it in my hands
```

---
## \#427 Posted by: uigiroux Posted at: 2018-07-20T14:19:35.910Z Reads: 269

```
Great!  We'll put me down for the first one you make :wink:
```

---
## \#428 Posted by: deucesdown Posted at: 2018-07-20T16:01:53.436Z Reads: 271

```
[quote="agniusm, post:426, topic:36847"]
additional 40eur import tax
[/quote]

omgwtf... :(
```

---
## \#429 Posted by: Benjamin899 Posted at: 2018-07-20T16:57:51.673Z Reads: 269

```
Whaaaaaat 40€? Did you buy 50 or so
```

---
## \#430 Posted by: agniusm Posted at: 2018-07-21T05:22:21.910Z Reads: 271

```
:) Thas how it is here. 120 + 21% tax + customs fees. Its crasy,  my fault, i did not ask to declare it like 25usd, then it would be nothing most likely
```

---
## \#431 Posted by: agniusm Posted at: 2018-07-21T07:26:12.695Z Reads: 278

```
[img]https://i.imgur.com/rjTbd6X.jpg[/img]
```

---
## \#432 Posted by: rojitor Posted at: 2018-07-21T16:45:17.861Z Reads: 275

```
Here is 120+shippings price added to totals+21%+customs fee+VAT of all of that again. It is very easy paying as much as the item or even more than the item. For 22€ shipped items customs are 30€. They usually stop above 30€ because many people refuses to pay.
Ah... If the item price is above 150€ we pay special bigger tax.
```

---
## \#433 Posted by: agniusm Posted at: 2018-07-21T16:48:10.750Z Reads: 272

```
F....ing gov rippoff
```

---
## \#434 Posted by: agniusm Posted at: 2018-07-25T08:55:09.592Z Reads: 278

```
Printed BMS enclosure. All seems good. Need to shift isb port up .5mm
I will be putting 4 2 cell tabs in bms enclosure set and you guys will need to solder or somehow attach wiring to the bms. 

[img]https://i.imgur.com/zyhlLVT.jpg?1[/img]

[img]https://i.imgur.com/nu9jqpq.jpg[/img]
```

---
## \#435 Posted by: damyzster Posted at: 2018-07-25T13:45:36.004Z Reads: 275

```
Hello community I'm planning to  make my first project. I would like to know if I could prepare cases with 4p cells and use just 3 p batteries in every one, leaving one slot for future use? ![20180725_153701|243x500](upload://q99k0GBFzljr9Z9wf2K171DgtW8.jpg)
```

---
## \#436 Posted by: Benjamin899 Posted at: 2018-07-25T13:51:33.304Z Reads: 259

```
sure, i see no problem. thats the big advantahe.
```

---
## \#437 Posted by: uigiroux Posted at: 2018-07-25T14:42:21.572Z Reads: 269

```
Awesome!  Put me down for one :smile:  Are these the same width as the 2s4p modules I got?
```

---
## \#438 Posted by: agniusm Posted at: 2018-07-25T15:52:39.369Z Reads: 271

```
1:1 external dimensions
```

---
## \#439 Posted by: agniusm Posted at: 2018-07-27T11:48:27.407Z Reads: 284

```
Fitted bms. Still want to fit balancing cables if they are OK and have enough room:

[img]https://i.imgur.com/AaxHi2p.jpg[/img]

[img]https://i.imgur.com/fBCbvx4.jpg[/img]

Also trying fillamentum 98A (Shore) tpu filament. So far it prints nocer than HK tpu. Feels more rubbery so debating if i want to switch as it will slightly increase product price
```

---
## \#440 Posted by: ervinelin Posted at: 2018-07-27T11:57:27.855Z Reads: 266

```
If I wanted to make a 10S2P pack, which module should I be buying? 10 pieces of 2P?
```

---
## \#441 Posted by: uigiroux Posted at: 2018-07-27T15:06:54.624Z Reads: 265

```
5 of the 2s2p modules, but in the notes say what your building, cause what you'll actually need is one 2s2p module, and then four 2p+2p modules.  Since the 2p+2p modules aren't listed, just order the five like I said and in the notes ask for the other modules so you can build a 10s2p.

Also, make sure you also buy 8 bus bars, 8 double cap covers, and 4 single cap covers (for the singles, get 3 black and one in another color so you can tell which terminal has the positive and which has the negative.  You may also want some ring terminals, though these aren't necessary as you can buy them at almost any hardware store.
```

---
## \#442 Posted by: uigiroux Posted at: 2018-07-27T15:12:33.224Z Reads: 255

```
Where do the cables from the battery and others go through?
```

---
## \#443 Posted by: agniusm Posted at: 2018-07-27T18:50:38.372Z Reads: 256

```
You wire it internally to and it exits the same way modules does so you would bolt your negative and positive to the bms box same as to another module and then you have 2 more for charging and load. You will need to solder or somehow attach wires from the tabs to bms. Look couple photos up, there is a closeup
```

---
## \#444 Posted by: uigiroux Posted at: 2018-07-27T19:46:25.512Z Reads: 253

```
Ok I get it.  Last question.  Is there access to the micro USB?

When will these be up for sale, and how much?
```

---
## \#445 Posted by: agniusm Posted at: 2018-07-27T19:59:08.567Z Reads: 250

```
Yes, there is access to usb. I still want to design a plug for that so its not that open
```

---
## \#446 Posted by: uigiroux Posted at: 2018-07-27T20:28:26.240Z Reads: 246

```
That'd be cool.  We could always use like a silicon sealant though.  So how long you think till you'll have this up for sale, and cost?
```

---
## \#447 Posted by: agniusm Posted at: 2018-07-28T14:00:36.457Z Reads: 248

```
Give me a week to finalyze it. Price wise, arround 20.
```

---
## \#448 Posted by: ervinelin Posted at: 2018-07-28T14:25:48.052Z Reads: 253

```
What's the diff between 2S2P and 2P+2P module?
```

---
## \#449 Posted by: uigiroux Posted at: 2018-07-28T15:51:02.933Z Reads: 271

```
I made a drawing so you can see how your battery will be made using the NESE Modules with one 2s2p, and four 2p+2p.  Also at the top of the drawing you see what the difference is between the two and hopefully when you see how the battery is assembled this way, you'll see why you need the different types.  Ask me if you have any other questions :slight_smile:

![15327929765677039357035448433186|374x500](upload://c1bOWmBZhkS5cPzJmB3G2Hie1lH.jpg)
```

---
## \#450 Posted by: agniusm Posted at: 2018-07-29T11:42:51.263Z Reads: 276

```
OK. All fits, i have populated all 16 wires including T1, T2 and second GND. My wires are 0.35mm^2 or 22AWG. Its snug and you have to feed couple of wires through grommet but its worth having it all nice and protected.

[img]https://i.imgur.com/78mIMtQ.jpg?1[/img]

[img]https://i.imgur.com/ymHHtzH.jpg?1[/img]

I might have full set later as i have no use for this BMS at the moment as i am working with larger packs (16S-20S)
```

---
## \#451 Posted by: agniusm Posted at: 2018-07-29T11:57:18.060Z Reads: 273

```
USB cover:

[img]https://i.imgur.com/a6bGHDX.jpg[/img]
```

---
## \#452 Posted by: uigiroux Posted at: 2018-07-29T12:46:10.853Z Reads: 265

```
Looks great!  Would the canbus cables go through the same exit as the power and display does?
```

---
## \#453 Posted by: agniusm Posted at: 2018-07-29T13:35:38.642Z Reads: 263

```
One side all the sense wires for the pack + temp if needed, the other - the rest of the cables.
```

---
## \#454 Posted by: karma Posted at: 2018-07-29T16:46:40.157Z Reads: 259

```
@agniusm is that CATIA as CAD software? 
Are the grommets 3D printed in TPU?
```

---
## \#455 Posted by: agniusm Posted at: 2018-07-29T17:01:24.939Z Reads: 258

```
Yes, tpu. Trying out fillamentum tpu
```

---
## \#456 Posted by: uigiroux Posted at: 2018-07-29T18:07:08.433Z Reads: 259

```
One thing I'm concerned about is the sensor wires are 22 gauge. I thought they needed to be about 18 gauge... I could be wrong though.
```

---
## \#457 Posted by: karma Posted at: 2018-07-29T18:17:29.259Z Reads: 257

```
Why would they have to be 18 gauge? The only thing I could see is that if the current is larger than what 22 gauge can handle. But since these are balance wires and shouldn't see alot of current I think it's fine. (Don't know the balance current on DieBieMS though...)
```

---
## \#458 Posted by: karma Posted at: 2018-07-29T18:20:09.300Z Reads: 259

```
22 AWG seems to be 3A and 18 AWG 7A according to [JST](http://www.jst.fr/doc/jst/pdf/current_rating.pdf). How many strands does play a big role though.
```

---
## \#459 Posted by: agniusm Posted at: 2018-07-29T18:32:31.013Z Reads: 254

```
@karma is right. Even 28awg or  ethernet cable would do. 22awg is overkill
```

---
## \#460 Posted by: uigiroux Posted at: 2018-07-29T18:32:34.862Z Reads: 254

```
Ok so if I'm using a 4 amp charger then I'd need thicker than 22 gauge.
```

---
## \#461 Posted by: Jumpman Posted at: 2018-07-29T18:41:12.054Z Reads: 260

```
If you use high strand silicone wire you should be good for up to 7A to 10A, I think, although you might not want to push things too far.
```

---
## \#462 Posted by: karma Posted at: 2018-07-29T18:53:16.933Z Reads: 258

```
Hmm I think you got the charging process wrong. The big leads comming of the charger, into the BMS, and onto the negative and positive terminals on your big battery pack is what is going to deliver the majority of energy for charging the pack. The small leads are for balancing the individual cell groups that is connected in series. The current going through the small wires will only be a small amount to burn of acess charge in order to balance the cell groups to the same voltage.
```

---
## \#463 Posted by: uigiroux Posted at: 2018-07-29T18:54:45.663Z Reads: 260

```
Oh, ok that makes sense, thanks for the explanation :smile:
```

---
## \#464 Posted by: agniusm Posted at: 2018-07-29T20:30:39.638Z Reads: 269

```
To further explain @karma explanation :D 4 big connectors will be used out of 5(you might need to reverse cells in you nese:).  First pack + and pack - will connect with series bus bars, same as you would connect another nese modules. Then you will have load + that you will route to pack - side and charge + that you will route to pack + side. You will connect your controller to load +  and pack - on nese bms. You will connect your charger to pack - and charge + on nese bms. You will connect your sense wires as per diebiems instructions. 
Bms'es that have 100mA of balancing curret would push 0.42A at 4.2V, less at smaller voltage, less if balancing power is smaller. Nissan Leaf i believe has BMS with 60mA balancing current on 60AH cell.
If i am correct, there are 15ohm resistors so if balancing happens at 4.2V the current eould be: ohms law I=V÷R=4.2÷15=0.28A, at 3V 0.2A and so on
```

---
## \#465 Posted by: mishrasubhransu Posted at: 2018-08-01T17:27:10.915Z Reads: 249

```
Hey @agniusm I just ordered several N.E.S.E tab sets but will be printing the case myself with some structural modification to conceal exposed leads completely. I was wondering if you used solidworks and were willing to share the design files. If not, no issues. I'll build on top of the stl files.
```

---
## \#467 Posted by: uigiroux Posted at: 2018-08-01T18:10:15.360Z Reads: 249

```
Can you show a pic of how you set your BMS up with the other NESE Modules and the VESC?  The explanation kinda confused me.  I've watched a bunch of YouTube videos on how to wire a BMS, but not sure if it's different on this BMS...
```

---
## \#468 Posted by: agniusm Posted at: 2018-08-01T18:17:20.737Z Reads: 249

```
I have not done wiring of thos BMS. If you have trouble i would suggest asking on the product thread. I would not want to support a product without inside out knowledge.
```

---
## \#469 Posted by: agniusm Posted at: 2018-08-01T18:29:51.264Z Reads: 256

```
Which one you need?
```

---
## \#471 Posted by: agniusm Posted at: 2018-08-01T18:59:51.554Z Reads: 260

```
? 2S4P? Better us PM for these questions not to clog main thread ;)
```

---
## \#472 Posted by: uigiroux Posted at: 2018-08-01T19:06:38.219Z Reads: 275

```
https://www.electric-skateboard.builders/t/n-e-s-e-no-solder-module-battery-packs/36847/464?u=uigiroux

But this whole explanation is about how to wire it up..?  You mention it by name (DieBieBMS)...  What was that describing if not how to wire it up using one of your new modules for that BMS.
```

---
## \#473 Posted by: mishrasubhransu Posted at: 2018-08-02T16:54:26.082Z Reads: 276

```
@agniusm, have you considered implementing a per cell fuse system into your units? Do you think it could be useful?
 From what I have understood from http://www.electricbike.com/inside-18650-cell, it will only be helpful with huge number of parallel cells. Otherwise it won't be able to support high current draw.

![image|690x478](upload://xQ2SQyRq9GNXC7wdcAIjiWPyzgN.jpg)
```

---
## \#474 Posted by: karma Posted at: 2018-08-03T14:59:02.422Z Reads: 276

```
Those fuses usually blow around 1-10A which would not work on our packs since we can draw 10-20A on each without breaking them. I am sure there are highjer current ones, just hard to find.  Tesla has such low current draw from each battery that they make alot of sense and if one would blow you would not notice it but if your 10S2P (samsung 30Q cells and 25A fuse on the parallel connections) blew 1 cell in a parallell you would have a problem. The VESC would not notice anything was wrong and still try to pull 30A (15A *2 parallell) which would damage the 15A rated cell that is alone. In the Tesla the 77P becomming 76P would only mean a tiny more current from the other 76 cells.
```

---
## \#475 Posted by: Itsmedant Posted at: 2018-08-05T18:25:17.125Z Reads: 274

```
Finally got my 3d printer going!

Here's a timelapse of the print, going to shoot another one from the top!

https://youtu.be/kaOci96JtqY
```

---
## \#476 Posted by: Giga Posted at: 2018-08-06T07:55:26.748Z Reads: 275

```
[quote="karma, post:474, topic:36847"]
The VESC would not notice anything was wrong and still try to pull 30A (15A *2 parallell) which would damage the 15A rated cell that is alone.
[/quote]

No, thats exactly why you have the fuse, then the other fuse will break as well and your battery will consist of one open connection.
So all in all, you only have 1 broken cell instead of all parallel ones, by the expenses of pushing home. 
(e.g. you have 10s4p, and 3rdS2ndP will fail, with cell level fusing the whole 4p of the 3rdS might got their fuse blown (if your battery is designed to only deliver the max. current drawn with ~0 tolerances), but only one damaged cell; if you dont have cell level fusing and 3rdS2ndP fails, then all 4cells of the 3rdS might be damaged (since it happens what you described, the remaining cells will have to share the load and die too) ; same applies for any other S or P count).
```

---
## \#477 Posted by: karma Posted at: 2018-08-07T19:47:42.221Z Reads: 258

```
I was for some reason thinking that since it was only a series connection that no fuse would blow since you usually have big wires for series connection. There is ofc a CLF from the cell to where the series connection is made.
```

---
## \#478 Posted by: agniusm Posted at: 2018-08-08T20:48:43.286Z Reads: 271

```
[quote="Giga, post:476, topic:36847"]
ght got their fuse blown (if your battery is designed to only deliver the max. current drawn with ~0 toler
[/quote]

OK, so you pull 80A from your pack and you have 4P. Each fuse (per cell) will have to be a 20A fuse, 20A x 4=80A.
Don't know about that. It does not make sense. I have not seen a laptop with fused cells, i have not seen tool pack with fused cells, most ebike packs are unfused, even Nissan leaf has no parallel fusing. Whats the fuss about that fusing? Get cells from proper vendor and you will be fine. And what @karma said.
```

---
## \#479 Posted by: agniusm Posted at: 2018-08-08T20:50:21.081Z Reads: 279

```
OK, i will have BMS enclosures these days. Have made couple so i have some initial stock:

[img]https://i.imgur.com/OhzfEyB.jpg[/img]

[img]https://i.imgur.com/fgXVMlN.jpg[/img]
```

---
## \#480 Posted by: uigiroux Posted at: 2018-08-08T20:51:31.056Z Reads: 267

```
Very nice!  As soon as I get a little extra cash I'll be getting one.  Probably in a few days :smile:
```

---
## \#481 Posted by: SixVogaR Posted at: 2018-08-08T21:06:09.157Z Reads: 267

```
Further up on this thread, @agniusm mentioned that PLA is not suitable for printing N.E.S.E modules. Why is that? Also, I plan on building a 10s4p N.E.S.E - would it be better to make 10x 4P or 5x 2S4P N.E.S.E modules? Asking this, because my deck has a bit of a concave, so I was wondering which N.E.S.E setup would fit better. Thanks!
```

---
## \#482 Posted by: Itsmedant Posted at: 2018-08-08T21:10:32.916Z Reads: 268

```
PLA has the potential to become pliable again under heat, so once your cells heat up, you run the risk of the enclosure not withstanding the forces of riding. (My understanding here, correct me if I'm wrong)

Also PETG is much stronger and more pliable. 

I wish it wasn't the case because I'm still sucking at PETG!
```

---
## \#483 Posted by: agniusm Posted at: 2018-08-09T05:41:25.138Z Reads: 261

```
Actually PLA is very strong and i would say, even stronger than PETG but its temperature is quiet low at 50C. It deforms if left in summer on a car. There is 3dxtech pla that is better on this count i believe. You can research their brand and see.
```

---
## \#484 Posted by: agniusm Posted at: 2018-08-09T05:53:39.047Z Reads: 256

```
Just checked, its called ECOMAX HT. They say, after anealing parts they can withstand 120-140C !? 😮
```

---
## \#485 Posted by: Trdolan03 Posted at: 2018-08-09T06:24:57.950Z Reads: 258

```
Has anyone made a 2 layer N.E.S.E pack for higher parallels like 6p or 8p?
```

---
## \#486 Posted by: agniusm Posted at: 2018-08-10T19:05:34.885Z Reads: 255

```
Easy to do if 44mm depth is acceptable. Series tabs are compatible and new 2s modules have through mounting holes on both ends
```

---
## \#487 Posted by: uigiroux Posted at: 2018-08-10T19:41:33.930Z Reads: 262

```
Man that would be a huge pack, lol!  Would be super sweet if along with the BMS module, there was a long flat box or case that would fit these modules in perfectly sized and at the BMS's end there was some extra space so like the BMS's LCD display, the on /off and charger port, etc... could be installed and it would make the modules look like a professionally made battery pack :heart_eyes:  think you could 3d-print something like that?  Even if not one whole piece you could make it several pieces to be assembled like a box, lol.

Sorry for going off topic on this little tangent, haha. :wink:
```

---
## \#488 Posted by: agniusm Posted at: 2018-08-10T20:13:41.807Z Reads: 266

```
Sorry, i am done for the time being :smile: Need to get on my powerwall module project as it is behind my schedule :).
@uigiroux, you can diy vacuum former out of vacuum cleaner, make a mold out of mdf and form a cover. It will be flexible and tougher. Have a demo video on my channel of my diy former made some 8 years ago
```

---
## \#489 Posted by: mishrasubhransu Posted at: 2018-08-10T20:21:20.683Z Reads: 262

```
agniusm kindly provided me with files for 2S4P, I can definitely put in some time in designing it as a single battery pack. We can discuss ideas here.
```

---
## \#490 Posted by: uigiroux Posted at: 2018-08-10T20:23:41.097Z Reads: 269

```
That's awesome!  What's the stats of your power wall going to be?  I really really want to get a set up with a huge power wall and then a couple huge solar panels that are fixed on one of those huge poles that follows the sun so you have like optimal lighting the whole time. Go totally off grid and then be able to sell your excess power.... Yep, that's the dream, haha.

How many days you hoping to get out of your power wall if it's your only source?
```

---
## \#491 Posted by: agniusm Posted at: 2018-08-11T07:12:35.486Z Reads: 276

```
Nah, dont have the money for powerwall yet. Its NESE powerwall module i am working on. Its 10 cell fused module you can lego to whatever capacity and whatever voltage.

[img]https://i.imgur.com/qBp9xzD.jpg[/img]

[img]https://i.imgur.com/HnZPt01.jpg[/img]
```

---
## \#492 Posted by: Wraith Posted at: 2018-08-11T07:35:24.253Z Reads: 273

```
Interested to follow the progress for this. I've been looking for a good alternative to powerwall because those aren't sold in my country :sweat:
```

---
## \#493 Posted by: mishrasubhransu Posted at: 2018-08-12T02:21:44.610Z Reads: 276

```
I'll know what features would be nice to have when I start building the modules, I am yet to receive the tabs. But in the meantime I edited the NESE 2S3P module into a hinged version. I can add mounting points so that they can be mounted to the board. Any special requests? 
All solidworks file available at https://drive.google.com/drive/folders/0B1q9GisJy4tHN1JiSlZubmVpaUk?usp=sharing(go to battery_pack/agniusm folder)

![Untitled|690x354](upload://pU8d71oRB7os03207GNgfZQV80a.JPG)
```

---
## \#494 Posted by: Trdolan03 Posted at: 2018-08-12T05:18:44.663Z Reads: 274

```
Do you use these without another enclosure to protect them?
```

---
## \#495 Posted by: oyta Posted at: 2018-08-12T05:33:52.506Z Reads: 275

```
Are there no mounting holes on the standard design from @agniusm? How do people attach them to the board? How are you gonna do it, @uigiroux?
```

---
## \#496 Posted by: Trdolan03 Posted at: 2018-08-12T05:47:06.900Z Reads: 264

```
@agniusm What is the price for 12, 1s 8p modules including all the hardware for them?
```

---
## \#497 Posted by: agniusm Posted at: 2018-08-12T05:55:52.588Z Reads: 260

```
Only 2S modules have mounting holes. Its possible as there is space for them on both ends. You can mount standard ones with double sided tape and feed som stainless strip through the modules and screw them at the end.
```

---
## \#498 Posted by: agniusm Posted at: 2018-08-12T05:56:21.866Z Reads: 255

```
You can find prices and whats included on the webshop
```

---
## \#499 Posted by: Trdolan03 Posted at: 2018-08-12T06:00:55.361Z Reads: 262

```
Ok, one other question, what is the pros/cons of the vented vs. unvented models?
```

---
## \#500 Posted by: agniusm Posted at: 2018-08-12T06:53:05.176Z Reads: 272

```
Cooling of the cells but its really for extreme currents where you even take off cell pvc jacket to help cooling
```

---
## \#501 Posted by: Trdolan03 Posted at: 2018-08-12T07:19:25.123Z Reads: 285

```
So it isn’t really necessary for esk8 then. I have some cells that I spot welded and then removed the spot welds because they were incredibly shitty. You can see that there are a few marks on each cell where the weld actually stuck. Do you think I could use these with the modules or would I have contact issues?![image|375x500](upload://fdXkztguhhqsElZHtMyriofCQtl.jpeg)![image|375x500](upload://9wkjJllMIBVBOxnCSTxhxPecFmq.jpeg)
```

---
## \#502 Posted by: Wraith Posted at: 2018-08-12T07:46:15.952Z Reads: 278

```
Hi @agniusm sent you a PM about the 2s modules that I’m looking into for an esk8 build. Will likely go with out the vents to make it more water resistant
```

---
## \#503 Posted by: agniusm Posted at: 2018-08-12T08:22:11.229Z Reads: 281

```
I recommend new cells with my modules but you can buff those off with dremel. It wont work like this. Needs cleaning
```

---
## \#504 Posted by: Wraith Posted at: 2018-08-13T07:10:08.084Z Reads: 285

```
Been asking @agniusm for some advice on the modules but seeing as you're also building on the @hummie deck. Wanted to ask if its possible to go 12s4p or 12s5p using the 2s3p  modules?

I would prefer not to have to route the hole any longer and wider than it already is and I measured that the 2s3p can fit across the width of the hole which is at 145mm with the  2s3p measuring at 142.3mm similar to how you set them here:
https://www.electric-skateboard.builders/t/hummie-based-build-respect/60150/34?u=wraith
but with double stacking :smile: 
What modules would I need exactly to get the 12s4p or even 12s5p? is it 1 2s3p and the rest being 3p + 3p? I've been measuring the height of a double stack and it comes in at 44mm so I'll be sending two of the 2sXp modules over to @psychotiller for him to measure it up on the enclosure.
```

---
## \#505 Posted by: Wraith Posted at: 2018-08-13T08:00:38.558Z Reads: 286

```
This actually helped me understand it better. I'll put together a diagram as well and see if my understanding of my build is right? Apologies in advance for my terrible writing :laughing:

![image|375x500](upload://aAbB7uwmVkN7YKBGQqt2BQDDvfE.jpg)
Sorry if I copied your diagram @uigiroux but all credit goes to you for it :wink:  
Is my understanding correct so far? i do plan on double stacking these so it would more or less look the same with the second layer overlapping? How would the 2nd layer be connected via the bus bars?
```

---
## \#506 Posted by: agniusm Posted at: 2018-08-16T17:59:40.667Z Reads: 283

```
Just a notification. I have put diebiems bms module for purchase and 3d stl download.
```

---
## \#507 Posted by: mishrasubhransu Posted at: 2018-08-21T13:53:23.263Z Reads: 286

```
Time to get started :D. @agniusm, the tabs are beautiful. 
![IMG_20180821_094816|666x500](upload://mTOmhVErKYiYq7u9dm2Yegcb7ep.jpg)
```

---
## \#508 Posted by: mishrasubhransu Posted at: 2018-08-22T19:40:04.294Z Reads: 280

```
@agniusm, in the 2S4P pack the middle 2 battery are very close, like the rest, so is it a bit risky given that they are not a part of the parallel pack anymore? I was thinking of putting a fishpaper in between or do you think that's not important.
```

---
## \#509 Posted by: agniusm Posted at: 2018-08-22T20:17:10.848Z Reads: 277

```
Dont think they will move at all to cause a problem. Put it in if it will make you certain
.
```

---
## \#510 Posted by: mishrasubhransu Posted at: 2018-08-25T05:48:56.312Z Reads: 288

```
@agniusm Where did you obtain the CAD for DieBieMS? I wanted to make the following part in sheet metal in CAD so that I print a template to cut and fold the 0.6mm copper sheet in the following manner. 
![MVIMG_20180825_022323|666x500](upload://gDEOpSXzO838nxC2Dh2cEJXtDx8.jpg)
![MVIMG_20180825_022318|666x500](upload://dl3ihG4maLRmFrqlR43rXVMsQMp.jpg)![MVIMG_20180825_021455|690x465](upload://fXYbIDEsorYtalMJfqVGtlqY0ON.jpg)
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/6623?u=mishrasubhransu
```

---
## \#511 Posted by: agniusm Posted at: 2018-08-25T07:13:01.355Z Reads: 264

```
I think its on github. Nice work there 👍
```

---
## \#512 Posted by: mishrasubhransu Posted at: 2018-08-25T07:59:20.331Z Reads: 264

```
https://github.com/DieBieEngineering/DieBieMS doesn't have .step, .igs, .iges ... Do I need to install altium and somehow export it to my CAD software?
```

---
## \#513 Posted by: TowerCrisis Posted at: 2018-08-25T15:19:50.284Z Reads: 263

```
What's your cad software? Afaik a .step file is fairly universal and can be imported directly to most cad softwares as a mesh or solid body.
```

---
## \#514 Posted by: mishrasubhransu Posted at: 2018-08-25T16:35:36.347Z Reads: 261

```
I just talked to jtag. It had gotten removed from the git repo somehow. He fixed it. 

Of course I can open .step file in CAD, haha. It's just that it wasn't there in the latest commit of the repo.
```

---
## \#515 Posted by: JTAG Posted at: 2018-08-25T17:04:10.737Z Reads: 264

```
Sowwy ☺️.

There is a parasolid as well now, I heard that mechanical cad people like that 🤭.
```

---
## \#516 Posted by: mishrasubhransu Posted at: 2018-08-26T08:47:38.699Z Reads: 284

```
Never worked with sheet metal cad before, it's pretty neat. BTW, it is super easy to make if you have sort of a clamp and a sheet cutter. It's pretty easy to make 90/45 degree bends with your finger. for 180 you need a clamp(or pliers?)
![MVIMG_20180826_040334|690x393](upload://r4TIqR6W5k6gDSfYTP6WRzYLoet.jpg)
I just made it yesterday by eyeballing it, today I made the cad. 

![DieBieMS_copper_tabs_render|524x500](upload://gwMZLcZQCsgWKXfkCg555OrzR45.JPG)
There is a long one in the pic above so as to avoid the usb and can port
![dbms_tabs_flat_pattern|690x452](upload://5Oa4c5X7no7hKtctzFX06smTi1e.JPG)
The pic above is available as pdf in the shared folder for you to print, cut, paste on 0.6mm copper and bend. 
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/6633?u=mishrasubhransu
```

---
## \#517 Posted by: uigiroux Posted at: 2018-08-26T16:40:18.168Z Reads: 263

```
Omfg this is amazing! :heart_eyes:
```

---
## \#518 Posted by: Powadangaboards Posted at: 2018-08-26T22:22:56.730Z Reads: 261

```
Need me some of these....
```

---
## \#519 Posted by: agniusm Posted at: 2018-08-26T22:54:19.218Z Reads: 259

```
Probably would be good to shrinkwrap the long one just in case.
```

---
## \#520 Posted by: agniusm Posted at: 2018-08-26T23:04:03.718Z Reads: 256

```
Parasolid? Whats that?
```

---
## \#521 Posted by: JTAG Posted at: 2018-08-27T00:01:36.266Z Reads: 260

```
A 3D file format preferred by the mechanical engineers I work with.
```

---
## \#522 Posted by: mishrasubhransu Posted at: 2018-08-27T06:24:45.976Z Reads: 266

```
I had printed these caps out but it I am using button head screws now, let me know if anyone wants them. You pay shipping.

![MVIMG_20180827_020711|666x500](upload://hNZDbxKxnVkDQXBSHdqAZXF9I2F.jpg)
```

---
## \#523 Posted by: agniusm Posted at: 2018-08-27T06:31:41.352Z Reads: 258

```
So you went with a snowflake theme then :slight_smile:
```

---
## \#524 Posted by: mishrasubhransu Posted at: 2018-08-27T07:18:00.475Z Reads: 261

```
snowflake theme? Because it's all white? Haha, well it look very pretty and clean now. We'll see what happens later.
```

---
## \#525 Posted by: mishrasubhransu Posted at: 2018-08-28T01:01:41.892Z Reads: 269

```
I can't figure out how this module keeps the cells compressed. Shrink fit?
![image|500x500](upload://2okeaHbgzxojePcic9cKrQiwiAa.jpg)
```

---
## \#526 Posted by: Wraith Posted at: 2018-08-28T01:12:38.050Z Reads: 261

```
Where’d you find this? Looks interesting
```

---
## \#527 Posted by: uigiroux Posted at: 2018-08-28T01:31:59.876Z Reads: 263

```
If it had double sided screws like the new NESE Modules it would explain that more.  As it is with one side open that does make me wonder how it will compress them too.  A lid that screws on (both sides), would also provide compression.  This basically looks like a modified NESE design, I like it though :slight_smile:
```

---
## \#528 Posted by: kylem21 Posted at: 2018-08-28T01:35:37.306Z Reads: 257

```
Energus power system
```

---
## \#529 Posted by: mishrasubhransu Posted at: 2018-08-28T01:35:47.240Z Reads: 248

```
https://www.energusps.com/shop/product/li2x4p25rt-li-ion-building-block-with-temp-sensor-3-6v-20ah-18c-325
```

---
## \#530 Posted by: mishrasubhransu Posted at: 2018-08-28T01:37:25.738Z Reads: 253

```
Oh yeah, They use 4 bolts, each about the length of the battery. Each of the 4 bolts sits in the space between 4 cells.

I think I can cad it up and we can make it using agnius's tabs and some sheet metal magic. Haha. But do we see a clear advantage of these over N.E.S.E? The only one I can think of is that connecting balancing wire is very easy which to be honest can be easily put into N.E.S.E too.
```

---
## \#531 Posted by: Powadangaboards Posted at: 2018-08-28T05:39:01.251Z Reads: 242

```
Where did you get this DieBieMS from?
```

---
## \#532 Posted by: Wraith Posted at: 2018-08-28T06:02:02.880Z Reads: 261

```
You can read all about it here:
https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639?u=wraith
```

---
## \#533 Posted by: uigiroux Posted at: 2018-08-30T15:03:22.593Z Reads: 256

```
Hey I was about to order the DieBieBMS module from you, was wondering if you were going to be making those copper strips that @mishrasubhransu posted?  Looks like a fantastic way to avoid having to solder things..

Also, for the balance wires, do we just connect them with a loop terminal to the corresponding screw?
```

---
## \#534 Posted by: mishrasubhransu Posted at: 2018-08-30T16:05:10.827Z Reads: 246

```
That would require steel tooling to stamp out the pieces and then jigs to bend them to the correct angles. I don't think he's going to do all that given minimal DieBieMS modules. Easiest way would be to order sheet from McMaster and cutting it with some sheet cutting shears.
```

---
## \#535 Posted by: agniusm Posted at: 2018-08-30T16:09:58.377Z Reads: 246

```
Not gonna make the strips. Too expensive for the tool, too time intensive doind it manually.
Balance wires connect with ring terminals as you mentioned.
```

---
## \#536 Posted by: mishrasubhransu Posted at: 2018-09-01T03:07:32.484Z Reads: 267

```
So here's a few links to the terminal you can use for making the connection. I had to spend quite a bit of time to find the right size., thought other's might need it too. One needs 2 different sizes.

**If you want to solder:**
* ring terminal for 12-10 awg wire: https://www.amazon.com/gp/product/B00AJSANVE
ring terminal for 22-26 awg wire: https://www.digikey.com/product-detail/en/panduit-corp/P22-10R-M/298-10065-ND/450218

**If you want to crimp:**
* ring terminal for 12-10 AWG wire: https://www.amazon.com/gp/product/B01D8E5JG4
* ringer terminal for 20-22 awg wire: https://www.digikey.com/product-detail/en/te-connectivity-amp-connectors/41582/A100613CT-ND/2233510
* crimper for 10AWG wire: https://www.amazon.com/gp/product/B01IQIALJC

![image|500x321](upload://jBV1HbIFAAswAuPLwS9hGGNuGcF.jpg)
![image|200x200](upload://OEYUd9DwdKAcjXyPgD0Ey1tqcu.jpg)
![image|500x500](upload://dQ9ILlNUR3OsNpctlDbqOlB5Gq0.jpg)
![image|200x200](upload://fnMb4ETW0Ul9SNbQuocUt1msoaT.jpg)
```

---
## \#537 Posted by: uigiroux Posted at: 2018-09-01T03:09:32.194Z Reads: 238

```
Wow thanks for all the info!!
```

---
## \#538 Posted by: Powadangaboards Posted at: 2018-09-01T07:19:07.261Z Reads: 237

```
How far have you got with your pack?
```

---
## \#539 Posted by: mishrasubhransu Posted at: 2018-09-01T07:22:56.940Z Reads: 238

```
If you meant me, then I am waiting for the ring terminal connectors. Just got 10 awg wire that I'll be using for all battey connections. Are you making one as well?
```

---
## \#540 Posted by: Powadangaboards Posted at: 2018-09-01T07:28:28.972Z Reads: 242

```
I am planning on it yes, i have 5 decks that are all partially done. 

2 x Evolve BGT rebuilds 
2 x Hummies V4 Hubs (1 Falcon Evo - 1 Hummie Carbon Deck)
1 Trampa Street Carver

Have everything for all but batteries, seems to be really hard to get them here in the UK.
```

---
## \#541 Posted by: deucesdown Posted at: 2018-09-01T11:42:27.402Z Reads: 240

```
Be careful, the first link is plated steel. You want plated copper for this.

If using the uninsulated terminals Channel Lock 909 are a good cheap crimper. Don't forget to heatshrink.

Be careful, you want high quality connections which can be hard to achieve with cheap crimpers. And probably want high quality connectors from say digikey/mouser if you're passing a lot of current.
```

---
## \#542 Posted by: uigiroux Posted at: 2018-09-01T14:04:14.331Z Reads: 237

```
Wouldn't the ring terminals on @agniusm site work too?
```

---
## \#543 Posted by: mishrasubhransu Posted at: 2018-09-01T17:56:06.771Z Reads: 237

```
Good catch regarding the steel part, it slipped me. 
I actually have copper lugs for soldering from Amazon but they are pretty big if I want to put the modules next to each other. I'll put pics soon. 

Regarding the 12-10 gauge crimps themselves. They are the exact same part (in terms of size and specification) to what is being sold in digikey and also what @Samau18 provided with dbms modules. 

All I can say about the crimper is that no matter how much I pulled by hand it didn't come off, can't say anything for current carrying capacity. If one is worried about current, then soldering copper lugs is the way to go.
```

---
## \#544 Posted by: moon Posted at: 2018-09-01T18:02:51.109Z Reads: 232

```
Fogstar wholesale
```

---
## \#545 Posted by: Chalupa_Batman Posted at: 2018-09-01T19:37:15.141Z Reads: 223

```
Any thoughts on making a 2s6p module? Would be great for a 10s6p build.
```

---
## \#546 Posted by: deucesdown Posted at: 2018-09-01T19:58:11.872Z Reads: 221

```
I'd be surprised if Agnius sold subpar stuff on his site. He's picky as hell. :slight_smile:
```

---
## \#547 Posted by: mishrasubhransu Posted at: 2018-09-01T23:28:22.757Z Reads: 233

```
I think I read somwhere that @agniusm had said that he won't make anything more than 2S4P modules. I forget the reason. Maybe he can explain.

But based on the tabs that he has, up to 2S8P modules  can be made.
```

---
## \#548 Posted by: Wraith Posted at: 2018-09-01T23:33:11.289Z Reads: 247

```
He isn’t going betond 2s4p as it’s way too long and it would be subject to even stress on the case
```

---
## \#549 Posted by: mishrasubhransu Posted at: 2018-09-02T04:26:45.662Z Reads: 262

```
So I tried 3 connection techniques. Left to right
1. vertical crimped 10AWG wire. 
2. Horizontal crimped 10AWG wire
3. bus bar(similar to agniusm's [bus-bar](http://18650.lt/index.php/product/n-e-s-e-series-tab/))

So this is my impression of the connection technique. 
1. The vertical crimps would work well with flex but adds some height to the battery. 
2. Horizontal would work well with flex but adds a lot of gap between modules
3. Bus-bar would be problematic because it would make the joints rigid. If the bus-bar were a bit longer it would allow the modules to bend relative to each other, but at the cost of rotational friction where it comes in contact with the screw.

To make joints flexible, I am thinking of making some copper sheet metal part so that there is some flexibility. Will post a solidworks model soon.

![MVIMG_20180901_235202|666x500](upload://iwQWtmaSoUdTrOsBcGwzBmXB2nT.jpg)
![MVIMG_20180901_235156|666x500](upload://eZ2I2eh4nTSJZGQYzjGe9NDeGiQ.jpg)
```

---
## \#550 Posted by: Wraith Posted at: 2018-09-02T04:54:37.035Z Reads: 257

```
Interesting. I thought @agniusm’s busbars would allow for some play for a deck with some flex as the bar rotate back and forth slightly as the packs would move.

Haven’t seen a complete setup with the busbars yet though
```

---
## \#551 Posted by: J0ker3366 Posted at: 2018-09-02T05:47:43.832Z Reads: 252

```
Honestly, just from looking at the picture, the inverted connection would only be great for flexy decks. The second connection is great no flex to medium flex and the third would be great for no flex decks. I dont see why all three arent viable options. Just my .02

Edit: agree on second connection lol.
```

---
## \#552 Posted by: mishrasubhransu Posted at: 2018-09-02T06:35:44.388Z Reads: 261

```
I edited my post above to structure it better for discussion.

I think 1st and 3rd are both good, but one is for flexy and other one is for rigid decks. 2nd just introduces too much of a gap.
```

---
## \#553 Posted by: Wraith Posted at: 2018-09-02T07:05:39.709Z Reads: 251

```
Would the third be ideal for a Hummie deck? Thats what i plan to use these on. I’ve reaf that there’s a slight flex to it so I figured enough for the busbar option sold at @agniusm’s site
```

---
## \#554 Posted by: J0ker3366 Posted at: 2018-09-02T07:55:08.099Z Reads: 244

```
Is say go for the first connection. Its more suited for flexing.
```

---
## \#555 Posted by: agniusm Posted at: 2018-09-02T09:43:01.546Z Reads: 255

```
Guys, you are overthinking flex. Cut out a piece of wood that is the size of 2 modules, and try to flex it. It wont flex at all and the bus bars i have have oval holes to allow for some movement. The flex ocurs over the length of the board and if you divide that up the joints between modules have minimal flex which are covered by the series bus bars. Sure if you compare 1st module and the last the deformation is significant but nothing to worried about modules next to each other. Just my line of thinking.
```

---
## \#556 Posted by: agniusm Posted at: 2018-09-02T09:46:54.443Z Reads: 247

```
If you are obsesed, one more option would be to use copper braid. Flatten copper pipe of similar size, insert a braid, hit it with a hammer and drill 5.5mm. Do that on both ends and you have flexible link
```

---
## \#557 Posted by: J0ker3366 Posted at: 2018-09-02T09:48:02.991Z Reads: 253

```
I agree but think of a Never Summer Heist deck. Made to flex lol. Now I would never diy my Heist lol. Its just too pretty. But if I did, I would definitely go the first connection. It would allow the room to flex with the board. I'm not trying to argue anything lol. Just see functional applications in all three.
```

---
## \#558 Posted by: mishrasubhransu Posted at: 2018-09-02T10:22:02.045Z Reads: 273

```
I actually really like the idea. Just got this. Might make it simpler by soldering the ends to keep it from unravelling and poking a 5mm hole to let the screw in.

3/8"(9.5mm) wide(when flat) and 1mm thick(when flat) should be plenty as a replacement to the bus bar(I do realize that it's better for DC current to have a solid block than lots of surface area). I got 10ft of it. 
https://www.amazon.com/Tinned-Copper-Metal-Braided-Sleeving/dp/B01MEG9V2R

![image|500x500](upload://tpgchEcYutXVE9WN2cEujPxNKUj.jpg)
```

---
## \#559 Posted by: Wraith Posted at: 2018-09-02T10:24:26.490Z Reads: 270

```
Which size are you going for and length? Looks promising and able to survive heavy flexing :smile:
```

---
## \#560 Posted by: mishrasubhransu Posted at: 2018-09-02T10:30:01.366Z Reads: 269

```
I edited my post above to answer your question :D
```

---
## \#561 Posted by: agniusm Posted at: 2018-09-02T12:32:32.272Z Reads: 275

```
This is what you might be making:

![maxresdefault|636x500](upload://dL0OnOkZ872atmHQRVAyKZ76hPR.jpg)
```

---
## \#562 Posted by: mishrasubhransu Posted at: 2018-09-03T05:10:26.601Z Reads: 275

```
Ok so while waiting for braided sleeve, I decided to figure out how to mount individual modules on the board and this is the prelimnary idea that I came up with. basically this plastic structure is how you easily connect to the deck while providing a bit of play in up-down and left-right direction to absorb shocks and account for any small flex. I think it would be a lot better if I use some elastic material to print this out.  Apart from this mount. I'll have an enclosure for dust and splash protection.

Do you guys have any suggestions to improve this or any different mounting idea? I think the first change that I have to make is to reduce the gap from the deck. 

![MVIMG_20180903_010332|666x500](upload://pWrxYLo88ChnDeWlPypNi3pCf0I.jpg)
![MVIMG_20180903_005914|666x500](upload://nv57VR9hykHrocL08uCjVmBM8fR.jpg)
![MVIMG_20180903_005936|666x500](upload://8quC0hOfxvxDKE4q9AvbwQOBKis.jpg)
![MVIMG_20180903_005929|666x500](upload://v0UX1pALEAlndL8myPpM2mW6g2b.jpg)
```

---
## \#563 Posted by: Benjamin899 Posted at: 2018-09-03T09:41:41.703Z Reads: 264

```
This Looks Epic
```

---
## \#564 Posted by: mishrasubhransu Posted at: 2018-09-05T16:22:38.200Z Reads: 269

```
3 things that work really well together. The crimper, braided cable and the 12-10 awg crimp. The cable is just perfect for bending. It turns out to be equivalent to 10awg wire, maybe a bit better. I have been very impressed with the quality of crimp that that the crimper makes. I haven't been able to pull it off, like at all. Really good value for money. 

Second thing that I finalized is the deck adapter for the nese modules. The circular cross section gives the module a nice springy base which conforms to the shape of the deck. As usual all files shared.

Next up is mounting them on the deck. Have a project deadline. So will work on it after the 15th. 

![MVIMG_20180905_004825|666x500](upload://rJqkRKfuVmae5Anno6s0FF9tVIF.jpg)![MVIMG_20180905_004431|374x500](upload://4k8iEeXJDJSP6Aq9TZZZW1CHlr2.jpg)
```

---
## \#565 Posted by: agniusm Posted at: 2018-09-05T20:42:04.167Z Reads: 260

```
I know you've been working on these mounts, but would it not be simplier to just use silicone spacers as standoffs and use mounting holes to screw modules to the deck? You can get wood inserts to make it reusable.
```

---
## \#566 Posted by: Benjamin899 Posted at: 2018-09-05T20:47:12.807Z Reads: 260

```
thats what i did. but i used normal wood screws. you get a slight bend into the modules, so if you want the premium solution, @mishrasubhransu seems to solve it all, and i must admit, those things look sick^^
```

---
## \#567 Posted by: uigiroux Posted at: 2018-09-05T21:29:27.384Z Reads: 257

```
Dude I NEED that braided cable!  Where do you get yours???
```

---
## \#568 Posted by: Benjamin899 Posted at: 2018-09-05T22:37:51.218Z Reads: 256

```
just search on ebay, took me 3min^^
```

---
## \#569 Posted by: mishrasubhransu Posted at: 2018-09-05T22:56:44.198Z Reads: 267

```
I posted it above. Select 3/8"(9.5mm) and 10Ft should be enough. https://www.amazon.com/Tinned-Copper-Metal-Braided-Sleeving/dp/B01MEG9V2R

![MVIMG_20180905_185024|666x500](upload://wBDwLe22R9pgtNuowcruTFmAJil.jpg)
```

---
## \#570 Posted by: Wraith Posted at: 2018-09-05T23:10:38.801Z Reads: 267

```
So on decks that are flat width-wise you wouldn’t need the mounts as much? My understanding is that’s the main reason for them while the braid allows the flex on the board lengths-wise?
```

---
## \#571 Posted by: mishrasubhransu Posted at: 2018-09-05T23:26:17.166Z Reads: 278

```
Yes, that was precisely my first thought. but the deck that I got is concave, so it is kind of weird mounting them. Also, I felt like the mounting screws would put pressure on the modules when the board is bending along the width. Of course it won't fail instantly but like a long-term fatigue failure. Maybe it's just me overthinking it, but it's definitely a clean way of mounting it and providing relief from vibrations and lateral bending. 

![MVIMG_20180905_192107|666x500](upload://dcVe7KaNw1SkXmn4ZJYNcDmOtXL.jpg)
![MVIMG_20180905_193044|666x500](upload://fS1INmHq3WrqVbKWaVAEQDkPZsR.jpg)
```

---
## \#572 Posted by: mishrasubhransu Posted at: 2018-09-05T23:29:21.536Z Reads: 266

```
I would love to see how you mounted it, maybe I am over-engineering this.
```

---
## \#573 Posted by: mishrasubhransu Posted at: 2018-09-05T23:34:56.925Z Reads: 260

```
The mounts are for mounting the nese modules on lateral curved surface and to provide strain relief when the board bends laterally. For bending along the length, the braided cable do the work.
```

---
## \#574 Posted by: moon Posted at: 2018-09-05T23:35:37.231Z Reads: 258

```
Why not just silicone them in?
```

---
## \#575 Posted by: mishrasubhransu Posted at: 2018-09-05T23:36:12.977Z Reads: 254

```
example? sdfasdfs
```

---
## \#576 Posted by: Wraith Posted at: 2018-09-05T23:37:51.971Z Reads: 254

```
I really like how the braided cables look so i think im going to do it that way as well.

Reason I asked was i plan on mounting on a hummie deck which I believe doesn’t have any concave on the mounting side so i could save abit of space for these as i May likely double stack for 12s8p later on lol
```

---
## \#577 Posted by: moon Posted at: 2018-09-05T23:43:07.179Z Reads: 255

```
Dont have these modules but what I would do is get some NEUTRAL CURE SILICONE, I found some for like £5 ($7)

And you can just try and see if you can apply the silicone on the deck and just press the modules onto the deck (or the other way around) but it provides dampening properties and stick real good and some people like LHB use it to attach their battery packs and other electronics to the deck/electroincs
```

---
## \#578 Posted by: uigiroux Posted at: 2018-09-05T23:46:59.197Z Reads: 258

```
I didn't really understand those mounts until just now seeing them from the side.  That's super cool!  Are you thinking of selling them or can you upload the file?
```

---
## \#579 Posted by: mishrasubhransu Posted at: 2018-09-06T00:39:08.075Z Reads: 273

```
Make sure to print this part vertically so that it is strong along the right direction. 
stl file: https://drive.google.com/file/d/13Kss8qCCWYNcwPeAVUciY7Qvw_sl8GWt/view?usp=sharing 

You need four inserts(M3x3mmx4.3) per module. You can get it from amazon or aliexpress
https://www.amazon.com/dp/B01M28WNQX
```

---
## \#580 Posted by: uigiroux Posted at: 2018-09-06T03:13:48.938Z Reads: 260

```
Sweet, thank you!
```

---
## \#581 Posted by: Trdolan03 Posted at: 2018-09-06T05:53:42.763Z Reads: 265

```
[quote="mishrasubhransu, post:569, topic:36847"]
I posted it above. Select 3/8"(9.5mm) and 10Ft should be enough. [https://www.amazon.com/Tinned-Copper-Metal-Braided-Sleeving/dp/B01MEG9V2R ](https://www.amazon.com/Tinned-Copper-Metal-Braided-Sleeving/dp/B01MEG9V2R)
[/quote]

My only concern is the amp carrying capacity of this. Can you ease my concerns at all?
```

---
## \#582 Posted by: Benjamin899 Posted at: 2018-09-06T06:56:04.235Z Reads: 258

```
these braided connections can carry a lot.
```

---
## \#583 Posted by: Trdolan03 Posted at: 2018-09-06T06:57:07.997Z Reads: 265

```
Like 4wd MTB a lot?
```

---
## \#584 Posted by: Benjamin899 Posted at: 2018-09-06T10:38:16.519Z Reads: 276

```
Not rly. I think you solution IS rly good.
I used some Pads right under the Module.
But i will either not mount them directly to the Deck or find some other solution. But i will probabyl Go your way with these holders. They Just eliminate all concerns. Rly nice Work.
![IMG_20180906_123122|281x499](upload://kJRLxy7SyGsF8TemjeBuQcNgNtw.jpg)
```

---
## \#585 Posted by: mishrasubhransu Posted at: 2018-09-08T07:49:46.146Z Reads: 271

```
What enclosure are you guys thinking of using with these packs? Given it any thought?
```

---
## \#586 Posted by: Wraith Posted at: 2018-09-08T07:54:54.433Z Reads: 278

```
Going for @psychotiller altar wedge. Similar to @Itsmedant though I don’t think I’ll have enough space to double stack on the hummie deck if I try your mounts as I recall making measurements and having it flat between the deck and enclosure already.
```

---
## \#587 Posted by: uigiroux Posted at: 2018-09-08T07:56:42.058Z Reads: 287

```
I am going to make a custom enclosure, but I got two of Hummies decks, so for the other one I'm gonna get one of @bigben enclosures for that board.  It's very nice and thin, so the bottom is barely noticeable, and it's only like €40.

![Screenshot_20180904-203912_Chrome|431x500](upload://5loaeYCQBKgUAiCiuPUaJbiUESt.jpg)
```

---
## \#588 Posted by: bigben Posted at: 2018-09-08T08:36:43.360Z Reads: 276

```
£45... but they’re fibreglass and got a few different styles.
```

---
## \#589 Posted by: mishrasubhransu Posted at: 2018-09-08T09:46:50.017Z Reads: 281

```
I like psychotiller's enclosure and the price point is good too.  I might get that. 

What do you mean double stack? Are you going for 10S8P? :open_mouth: Also are you using hummie's deck?

@Wraith, @uigiroux  since you are going to mount these on flat decks, I'll make different ones which doesn't have any bend in the base. That way the module will just hover 2mm above the board like mine does. Don't use the stl that I provided before. What do you guys think?

BTW this is my [deck](https://www.skateshred.com/wholesale-blank-longboard-decks/41-x-9-5-dark-walnut-drop-down-decks-dw41.html) 
![image|690x265](upload://cDSmSaS59G7NCaEGmid3sDughXQ.jpg)
```

---
## \#590 Posted by: Wraith Posted at: 2018-09-08T09:53:39.851Z Reads: 280

```
[quote="mishrasubhransu, post:589, topic:36847"]
What do you mean double stack? Are you going for 10S8P? :open_mouth: Also are you using hummie’s deck?
[/quote]
Yeah I'm going to go with a Hummie deck, just waiting on the flipskys and Hummie should be sending them over to Tiller for mounting and the enclosure. Figured I'd get that out of the way and ask him to do it so its more or less done before it gets shipped internationally to me.

As for the double stack yeah thats something I do plan on later on but for now I'll go with a 12s4p just to make the most out of the space. Tiller will be widening the hole on the deck as well cause the 2s4p modules wont fit without modifying the recessed area.

yeah having the base flat would work better but I could see myself using the ones with a rounder base if I deck swap to something with a more aggressive concave. Also not sure yet if they will fit or if I'm going to still drill the holes for them. I'm guessing 3m hook velcro won't cut it because of the surface area on the base?
```

---
## \#591 Posted by: mishrasubhransu Posted at: 2018-09-08T10:09:40.950Z Reads: 281

```
[quote="Wraith, post:590, topic:36847"]
Also not sure yet if they will fit or if I’m going to still drill the holes for them. I’m guessing 3m hook velcro won’t cut it because of the surface area on the base?
[/quote]

So the best way would be to use wood screws with a big flat head, because unlike the enclosure you won't be taking these off(unless you change board). Even when you want to take the nese modules off for servicing these will still remain on the board.  I am going to use these [screws](https://www.amazon.com/dp/B01MFAIS08)
![image|200x200](upload://5RjCZrnjN9fwuEk1bkV9JlE0Q4L.jpg)

[quote="Wraith, post:590, topic:36847"]
As for the double stack yeah thats something I do plan on later on but for now I’ll go with a 12s4p just to make the most out of the space. Tiller will be widening the hole on the deck as well cause the 2s4p modules wont fit without modifying the recessed area.
[/quote]

Oh that's actually awesome. The very reason I didn't go for hummie's deck was that it couldn't fit nese 2S4P modules.
```

---
## \#592 Posted by: Wraith Posted at: 2018-09-08T10:25:03.977Z Reads: 260

```
yeah I do like the decks. @uigiroux modified his Hummie deck as well actually

Also just saw your deck and thats a massive drop! 1" or 2"? lol that should really lock you in! looks similar to the Red Ember boards which I would like to get as well haha
```

---
## \#593 Posted by: Benjamin899 Posted at: 2018-09-08T11:00:28.482Z Reads: 261

```
nice seller. i was always looking for a site that a has thicker decks. Do they ship worldwide?
```

---
## \#594 Posted by: SqueekyCBJ Posted at: 2018-09-08T12:52:05.782Z Reads: 259

```
@mishrasubhransu I'm using the olive wood version of the deck in my build.  If you come up with custom battery mounting, etc and want to make some $ and make two I know it will fit my deck.  ;)
```

---
## \#595 Posted by: Trdolan03 Posted at: 2018-09-08T15:11:14.735Z Reads: 256

```
Does anyone have an issue with the screw terminals vibrating loose on their packs? Or do you use loctite on the terminal screws?
```

---
## \#596 Posted by: agniusm Posted at: 2018-09-08T20:15:11.756Z Reads: 266

```
Overlooked this. This is my friends from energusps modules(also from Lithuania). They are spotwelded and sold ready made with cells. They can make whatever cells you want with if the quantity is right. They have temp sensor integrated and each cell is fused. NESE density falls between Energusps and Vruzend although i don't think of Vruzend as a solution at all. Too many well known errors implemented.
These are high end modules used in Formula E.
This is pre-history and the man himself: https://translate.google.com/translate?hl=lt&sl=lt&tl=en&u=http%3A%2F%2Fe-motion.lt%2F2013%2F12%2F12%2Fakumuliatoriaus-blokas-is-18650-cilindriniu-celiu%2F
```

---
## \#597 Posted by: agniusm Posted at: 2018-09-08T20:22:36.726Z Reads: 278

```
There are 2 countermeasures implemented.
1. Supplied screws have a spring washer and they are of very good quality made by Japanese.
2. Printed screw caps have grooves mimicking spanner socket:
![image|450x375](upload://yaRIbIeaM4kQ87Fre6isoOXiHpO.jpg)
 for second stage of unbolting protection: http://18650.lt/index.php/product/twin-bolt-cap/
```

---
## \#598 Posted by: agniusm Posted at: 2018-09-08T20:30:09.104Z Reads: 281

```
I dont have a board. I am more of a 2 wheel person but these are the things i would try:
https://www.racedayquads.com/products/fc-anti-vibration-standoffs-m3x7-4-5-4-piece-set
along with threaded wood inserts:
![image|500x500](upload://6QmaQUe6Rg66HxnvLqMKtLOkU6B.jpg)
fitted with some epoxy
```

---
## \#599 Posted by: uigiroux Posted at: 2018-09-08T22:30:39.555Z Reads: 266

```
I think that's a great idea!  Would definitely work well for me, I made my modifications to the board already and the cutout is a bit wider then the modules now, so I think using those too mount the NESE Modules would be ideal :slight_smile:
```

---
## \#600 Posted by: mishrasubhransu Posted at: 2018-09-08T23:48:57.853Z Reads: 274

```
I had found them on McMaster, but to my disappointment they are rated for compression. Not tension.
```

---
## \#601 Posted by: mishrasubhransu Posted at: 2018-09-08T23:56:43.217Z Reads: 281

```
Cool. I'll put links to flat mounts soon.
```

---
## \#602 Posted by: mishrasubhransu Posted at: 2018-09-09T09:51:14.079Z Reads: 286

```
stl files: https://drive.google.com/open?id=12nsSWwk84cC8EZ4IVN4RpWdnaNB0QHoO
You have to print them vertically, otherwise it might delaminate when stressed too much. Normal loading doesn't affect it though. 
flat deck vs concave deck
![flat_deck_mount|300x270](upload://8W5gfYEOdf26aMx0IH0ESBGyEl7.PNG)![concave_deck_mount|300x284](upload://zjgxxUmvCVzXjSXqbGfe2Kaxpfr.PNG)
![flat_deck_mount2|300x175](upload://uvcpRRuCL2rLdBE0kfyLx9zQcER.jpg)![concave_deck_mount2|300x194](upload://jTPXXk4h71fxUfznRXXilQ7xZEZ.PNG)
```

---
## \#603 Posted by: Benjamin899 Posted at: 2018-09-09T10:00:27.361Z Reads: 279

```
that holder has flex or is it stiff?
```

---
## \#604 Posted by: mishrasubhransu Posted at: 2018-09-09T10:09:02.437Z Reads: 280

```
flex, that's why it has that circular region, otherwise it would have been one straight line(that was my first design, very stiff). I could make the circular portion more wiggly too to increase flex further, but from my tests it's at a sweet-spot.
```

---
## \#605 Posted by: uigiroux Posted at: 2018-09-10T01:11:04.450Z Reads: 281

```
How much length does this add to a module?  Let's say my current modules are 100mm in length.  What would they be with these added on from end to end?
```

---
## \#606 Posted by: Benjamin899 Posted at: 2018-09-23T20:44:37.203Z Reads: 287

```
Hey i just wanted you share the battery i build. 10s4p and works like a charm.

![IMG-20180909-WA0005|281x500](upload://onqzb4bBxCRw2aICwGW7fCyVExn.jpeg) ![IMG-20180909-WA0008|281x500](upload://s0MOkEIkPcL4AsotCJUhgiJX5jz.jpeg) ![IMG-20180909-WA0011|281x500](upload://512PXYHDJLenBLLKO7zV90ASJPT.jpeg) ![IMG-20180910-WA0002|690x388](upload://qNVzgCo847LZFxvWP24G7fcGH8f.jpeg) 

I used Lipo Silicon protector to cushion the battery and then completly put it in heatshrink.

![IMG-20180909-WA0013|690x388](upload://ssc5KVTW9YK7gfqiaPP7sqFMhJs.jpeg) ![IMG-20180909-WA0015|281x500](upload://yUFt3Qxs8xPlbP7xv0T0l5lwYEN.jpeg) ![IMG-20180909-WA0017|281x500](upload://pLqArzkjeZkL0Ui5VLFQl9C3oNU.jpeg) ![IMG-20180910-WA0005|690x388](upload://gyfYmxfveiFjJzi591UrQLcynCg.jpeg)
```

---
## \#607 Posted by: mishrasubhransu Posted at: 2018-09-23T20:48:08.071Z Reads: 275

```
Cool! What does it look like on the board?
```

---
## \#608 Posted by: Benjamin899 Posted at: 2018-09-23T21:15:21.246Z Reads: 280

```
Looked like that last week. I made some mods. Build a tunnelriser in UNIK style and cleaned it up, so no more cables dangling around. 
![IMG_20180911_130923|690x388](upload://3VjBR3WyTvwG0djkuUIcTcMBYjz.jpeg)
```

---
## \#609 Posted by: agniusm Posted at: 2018-09-29T16:04:22.351Z Reads: 269

```
Great. Looks like doublestacking works on street boards as well.
```

---
## \#610 Posted by: Benjamin899 Posted at: 2018-09-29T16:25:07.765Z Reads: 267

```
yep works flawlessly. but this is more like a prototype. once i have my stuff i will get a stiff deck and make a flat pack.
```

---
## \#611 Posted by: mishrasubhransu Posted at: 2018-09-29T21:53:49.536Z Reads: 274

```
Since I am using the NESE copper tabs in this mod, I thought it would be relevant to post it here too:
More details at: https://www.electric-skateboard.builders/t/my-compression-pack-design-gauging-interest/67878/143?u=mishrasubhransu

![IMG_20180929_171130|666x500](upload://3xIdV43Fwi13FLTKOU9YqqafEvq.jpeg)
```

---
## \#612 Posted by: uigiroux Posted at: 2018-09-29T23:32:03.495Z Reads: 273

```
I really like your design.  It's perfect for two rows of cells style, but if your wanting to orient the cells the other way I think that would be quite difficult.
```

---
## \#613 Posted by: mishrasubhransu Posted at: 2018-10-01T06:26:12.179Z Reads: 280

```
It's mostly assembled on my board. I have to flip cells from +ve to -ve to use a short cable from battery to DieBieMS. @agniusm, I was wondering if you realized that was a problem? 

Of course, I still have to crimp the balancing wires, route it nicely and take it to DieBieMS.

![IMG_20180930_032031|666x500](upload://Awo8ej4SirEN0lzafNvhDvgcA7s.jpeg) ![IMG_20180930_031952|666x500](upload://fXkFBH3ebgt9ldy4bzmunpDfWlT.jpeg) ![IMG_20180930_032000|666x500](upload://7pFqW1On7WDRsaR7Iia5mzSoywW.jpeg) ![IMG_20180930_031846|666x500](upload://eOPJo9oWRAiql0axRwS57wn8UgX.jpeg) ![IMG_20180930_031910|666x500](upload://aIVc3EqXCfwjt0ewljKCnBh0rps.jpeg)
```

---
## \#614 Posted by: uigiroux Posted at: 2018-10-01T06:43:44.725Z Reads: 267

```
I love how you secured these to your deck!  I know the designs of them were already shown and discussed, but seeing it actually assembled and mounted on the deck.... Looks pretty great..  They don't add that much extra width as I thought they would, so I think I'm gonna do that too :smile:  What were you saying about having to swap positive and negative wires btw?
```

---
## \#615 Posted by: agniusm Posted at: 2018-10-01T06:55:28.032Z Reads: 260

```
I too have no idea what problem there is
```

---
## \#616 Posted by: mishrasubhransu Posted at: 2018-10-01T07:08:14.855Z Reads: 260

```
@uigiroux, @agniusm maybe I wasn't clear. As per your +ve and -ve marking on the battery and the DieBieMS battery + and battery -ve sign, I would have to use long wires from one side to the other to connect the battery to DieBieMS.
```

---
## \#617 Posted by: mishrasubhransu Posted at: 2018-10-01T07:09:54.954Z Reads: 267

```
Basically, I can't connect them together
![Screenshot_20181001-030909|281x500](upload://iCiPHhHAGKH7bn11HpsMkiKXhxE.jpeg)
```

---
## \#618 Posted by: agniusm Posted at: 2018-10-01T07:57:22.524Z Reads: 263

```
I still don't get it. You have PACK- of the BMS on the photo and what?
I mean the whole problem you have is markings?
Flip the damn cells, take red and black marker and remark you positive and negative. DieBieMS enclosure was adopted to suit NESE modules not the other way round. There are a lot of CAD files that make up my modules and i will certainly not add more for enclosure that i don't sell (or sell 2) just because of marking.
Sorry, but you are being too fussy calling it a problem.
```

---
## \#619 Posted by: agniusm Posted at: 2018-10-01T08:04:12.088Z Reads: 258

```
The pack and board looks great BTW.
```

---
## \#620 Posted by: mmaner Posted at: 2018-10-01T13:25:08.115Z Reads: 257

```
[quote="agniusm, post:618, topic:36847"]
you are being too fussy calling it a problem
[/quote]

good lord, this is the new face of capitalism...
```

---
## \#621 Posted by: agniusm Posted at: 2018-10-01T13:40:45.936Z Reads: 259

```
You just have to go and pick out each fraze 😂
It must have something to do with lord...
Chill
```

---
## \#622 Posted by: mmaner Posted at: 2018-10-01T13:42:21.406Z Reads: 257

```
Don't wanna get called out, don't be so arrogant, I mean all you did was make some boxes FFS.  You can't talk to people like that and expect to not get called on it.
```

---
## \#623 Posted by: agniusm Posted at: 2018-10-01T14:31:19.791Z Reads: 260

```
Looks like you browse the threads looking to pick a fight. 
Relax, not gonna

P.S. There are differences between nations, etiquette, norms of manners and if you think every nation in the world will be painted to your spec., get real. And here is me being rude: buzz off
```

---
## \#624 Posted by: mmaner Posted at: 2018-10-01T14:37:50.412Z Reads: 265

```
there you go again, acting like you have some juice.  have you been to the internet before?

Here's the facts...
1.  Your a dick to anyone who has the audacity to question anything about your ridiculous little boxes
2.  Your level of arrogance is ludicrously high for the elementary achievement of designing and printing a box
3.  Being an asshat is not a geographic issue, its an issue with being an asshat

In closing...Have some respect n00b.
```

---
## \#625 Posted by: agniusm Posted at: 2018-10-01T15:11:09.702Z Reads: 255

```
For another time you started calling someone names and expressing your empty anger., not me.
I just pointed out that problem man had is not a problem at all, and that i called being fussy, as it does not affect electrical integrity.
Thanks for showing your true nature once again caveman.
```

---
## \#626 Posted by: mmaner Posted at: 2018-10-01T15:15:01.528Z Reads: 258

```
[quote="agniusm, post:625, topic:36847"]
caveman
[/quote]

you spent 30 mins replying and that's all you can come up with?  you've been insulting people in here for a week, that's pretty weak with all the practice you've had.

[quote="agniusm, post:625, topic:36847"]
For another time you started calling someone names and expressing your empty anger., not me.
[/quote]

I'm not even sure how to read that.  But in the interest of being clear, you began this by insulting another user...again.  Simply put, I'm tired of it.  I would suggest you be an adult and apologize to the man and try to amend your behaviour.  Or you could just continue to be arrogant and insulting.  Either way, I'm having fun :slight_smile:.
```

---
## \#627 Posted by: agniusm Posted at: 2018-10-01T15:45:29.956Z Reads: 254

```
**Friends, customers fellows,**
_I have decided not to participate here anymore. I think i have done all i can do. I would like to take time to invite you with any inquiries, questions or suggestions directly. My email: agniusmk@gmail.com. If you need verbal conversation, we can arrange that by email._
_I have no time for the sorts of attacks. I am how i am, sometimes blunt, sometimes too straightforward or ignorant but i have no intentions to insult, harm or abuse someone i don't know well enough for no reason._
_So for some of you farewell and to others, see ya later ;)_
Kirk out
```

---
## \#628 Posted by: mishrasubhransu Posted at: 2018-10-01T15:45:57.475Z Reads: 251

```
Thanks for backing me up here @mmaner, but I didn't take it as an insult. Agnius and have talked about multiple things over private chat and public chat and he's a pretty helpful guy, someone that takes suggestion and definitely not a dickhead, like you think. His style might be a bit different than what we are used to but definitely doesn't mean harm.
```

---
## \#629 Posted by: GrecoMan Posted at: 2018-10-01T16:01:23.512Z Reads: 247

```
lmao you’re a disgrace to the forum 🤣
```

---
## \#630 Posted by: mmaner Posted at: 2018-10-01T16:10:46.275Z Reads: 246

```
I appreciate you saying so, just for clarification your not the only one he has insulted.
```

---
## \#631 Posted by: mmaner Posted at: 2018-10-01T16:12:32.060Z Reads: 258

```
[quote="agniusm, post:627, topic:36847"]
I am how i am, sometimes blunt, sometimes too straightforward or ignorant
[/quote]

Meaning, he can say what he wants and its ok, but when he gets called on it he's being attacked...I really don't know how the human race still exists some days.
```

---
## \#632 Posted by: Jc06505n Posted at: 2018-10-01T16:30:52.852Z Reads: 254

```
but why the italics though :thinking:
```

---
## \#633 Posted by: Benjamin899 Posted at: 2018-10-01T17:57:57.917Z Reads: 250

```
jesus guys take a chill pill. don't forget that there goes alot lost in translation and writing.
```

---
## \#634 Posted by: pylotope Posted at: 2018-10-01T18:03:13.930Z Reads: 255

```
[quote="mmaner, post:624, topic:36847"]
Your a dick..
ridiculous little boxes..
elementary achievement..
asshat..
n00b.

I’m having fun :slight_smile:
[/quote]

[quote="GrecoMan, post:629, topic:36847"]
lmao you’re a disgrace to the forum :rofl:
[/quote]

So you're supposed to be the good guys here?
I'm not so convinced the right guy gtfo'ed.
Even went through the logs for the past month or so and only saw people getting offended for nothing.

Wtf.
```

---
## \#635 Posted by: uigiroux Posted at: 2018-10-01T18:12:52.598Z Reads: 240

```
I find this extremely troubling.  @mods need to shut this down since apperantly the ones who should be taking the higher road are behaving the worst.
```

---
## \#636 Posted by: mmaner Posted at: 2018-10-01T18:13:17.362Z Reads: 245

```
he was insulting people, essentially calling them stupid, I had enough and called him on it, he got but hurt and left...end of story.

[quote="pylotope, post:634, topic:36847"]
I’m not so convinced the right guy gtfo’ed.
[/quote]

your welcome to take it up with @treenutter or @onloop  or @anorak234 if you think I acted inappropriately.
```

---
## \#637 Posted by: mmaner Posted at: 2018-10-01T18:13:51.031Z Reads: 255

```
[quote="uigiroux, post:635, topic:36847, full:true"]
I find this extremely troubling. @mods need to shut this down since apperantly the ones who should be taking the higher road are behaving the worst.
[/quote]

ridiculous, as usual.
```

---
## \#638 Posted by: uigiroux Posted at: 2018-10-01T18:15:11.408Z Reads: 248

```
Yep, and now as expected you're going to attack me.  Great leadership btw..
```

---
## \#639 Posted by: mmaner Posted at: 2018-10-01T18:16:20.741Z Reads: 259

```
You need to learn a little logic.  I didn't say anything to you, you came in here and said something silly about me and I rebutted.  That's not an attack, by any definition.
```

---
## \#640 Posted by: anorak234 Posted at: 2018-10-01T18:17:29.458Z Reads: 256

```

```

---
## \#641 Posted by: anorak234 Posted at: 2018-10-01T18:18:53.567Z Reads: 262

```
@uigiroux my apologies for cutting you off, that was not deliberate but I don’t have time to review the situation a present. I’m closing this out of control topic for now and the situation will be reviewed later today.
```

---
## \#642 Posted by: anorak234 Posted at: 2018-10-02T19:17:23.978Z Reads: 255

```

```

---
## \#643 Posted by: anorak234 Posted at: 2018-10-02T19:18:08.404Z Reads: 265

```
Please keep any new posts within the subject of the topic - this is about modules, not who's attacking who.
```

---
## \#644 Posted by: neiru37 Posted at: 2018-11-05T16:19:40.336Z Reads: 255

```
Which hardware set do I buy if I want to 3d print the 2s4p pack myself?
```

---
## \#645 Posted by: Benjamin899 Posted at: 2018-11-05T16:33:27.866Z Reads: 263

```
It is a modified 8p Pack. So the 8p hardware set. Only thing you need to do is a bit of cutting.
```

---
## \#646 Posted by: mishrasubhransu Posted at: 2018-11-05T22:40:40.149Z Reads: 270

```
Buying the fasteners in bulk makes it really cost effective(only if you are 3D printing your own boxes, otherwise, I would say, just get everything from 18650.lt). Agnius uses spring loaded japanese bolts that are really good at preventing unscrewing due to vibration, but I just use locktight to do the same. Just a bit messier and a bit more inconvenient. 

If you are in the US, then you can buy it from:
[M5 Bolt](https://www.mcmaster.com/90909a722)
[M5 square nut](https://www.mcmaster.com/90225a101)
[M2.9 screw](https://www.mcmaster.com/95844a250)

![image|151x122](upload://2oDqoeaZP6qW3Wm2apSlusE2F2I.jpeg) ![image|152x123](upload://klR0U9gHA6h5P44MvKLv9mok8o7.jpeg) ![image|150x77](upload://nNAZ51tVLEm27ZRjx6nIv1F8fqr.jpeg) 

BTW guys, I modified the module to have a support bar in between(thickness can be increased). Now we should be able to do up to 2S8P modules. He appreciated the change but said that since most of his sales come from 8P modules, so doesn't make sense to change the existing design, but if you want to use the NESE hardware and have something more than 2S4P, then let me know, I can provide the stl/solidworks for any size upto 2S8P(for free of course). @agnius do let me know if you think it's alright to do so. 
![image|690x305](upload://gYNqLa9SOfAa3gL4J6hakjiWzRM.jpeg)
```

---
## \#647 Posted by: Benjamin899 Posted at: 2018-11-05T22:43:30.046Z Reads: 255

```
nice work. i am more interest in a 21700 version. we could still use his hardware taps, just need to make an extrusion so they stay centered on the terminals.
```

---
## \#648 Posted by: mishrasubhransu Posted at: 2018-11-05T22:50:46.824Z Reads: 254

```
Yeah, absolutely, everything is parametric, as long as the diameter of cells is same as, or less than, 18650 , I can make a module for you.

Edit: but I just checked and it seems the diameter of those cells is at max 21.22mm, so that's not going to work with the tabs that he has.
```

---
## \#649 Posted by: Benjamin899 Posted at: 2018-11-05T23:17:39.040Z Reads: 263

```
well look at it this way. You make everything a bit bigger to fit 21700 and then you "mill" pockets for the 18650 taps but position them centered over the 21700.
This is a rough idea of what i mean. You basicly make a pocket into the wall for the "old" tabs and just make the rest of the body bigger for bigger batteries.
![Untitled|690x388](upload://2jsctMXjDfmH3pz3bHHDAonkf1r.png)
Edit: This will make them a bit wider than normal.
```

---
## \#650 Posted by: Trdolan03 Posted at: 2018-11-12T17:51:33.321Z Reads: 246

```
@agniusm when I purchase a 10s 3p hardware kit on the website, do I get 1s 3p modules or 2s 3p modules?
```

---
## \#651 Posted by: Trdolan03 Posted at: 2018-11-12T17:53:09.975Z Reads: 244

```
[quote="mishrasubhransu, post:646, topic:36847"]
Now we should be able to do up to 2S8P modules. He
[/quote]
Do you have a rendering of this?
```

---
## \#652 Posted by: mishrasubhransu Posted at: 2018-11-12T18:09:20.890Z Reads: 236

```
You would purchase 5 qty of 2s3p modules
```

---
## \#653 Posted by: mishrasubhransu Posted at: 2018-11-12T18:12:51.572Z Reads: 240

```
It's similar to the module above just has space for more cells. I am travelling until Wednesday. I'll send after that.
```

---
## \#654 Posted by: agniusm Posted at: 2018-11-12T18:16:29.390Z Reads: 241

```
Hardware kits are tabs only. Its for those peeps printing their own enclosures 
@mishrasubhransu You can mod as you want mate. Just a clarification that you cannot make 2S8P module, only 8P+8P so you will need to do external loop at the top of the pack. Applies to everything above 4P.
```

---
## \#655 Posted by: mishrasubhransu Posted at: 2018-11-12T18:18:15.665Z Reads: 243

```
Aah, so that's the nomenclature. 8P+8P is what I meant.
```

---
## \#656 Posted by: agniusm Posted at: 2018-11-12T18:19:31.581Z Reads: 241

```
Enclosures are simple. Its just a matter of scaling exsisting one plus changing holes back. Problem is tabs unless you are thinking of making some diy tabs
```

---
## \#657 Posted by: Benjamin899 Posted at: 2018-11-12T18:50:05.419Z Reads: 246

```
no i thought about using yours. right, like you said, scaling is a non issue, but i thought to make a slot for the tabs into the wall of the module, so that they stay centered on the cells. It will make the module thicker than just scaling up, but first i have to finish my DD.
```

---
## \#658 Posted by: agniusm Posted at: 2018-11-12T19:13:56.448Z Reads: 246

```
You can't. You could use a thinner cell. Imagine that the bump centers are 18mm apart. You cant center a cell when they are 21mm apart unless you will hammer it flat to 18mm. Or you could use each second bump but thats a waste of space
```

---
## \#659 Posted by: Benjamin899 Posted at: 2018-11-12T19:33:08.844Z Reads: 237

```
ah dang totally forgot that part^^ yeah ofc that is not possible.
```

---
## \#660 Posted by: Trdolan03 Posted at: 2018-11-12T20:07:07.564Z Reads: 243

```
@agniusm my question is about the complete hardware sets  http://18650.lt/index.php/product/n-e-s-e-hardware-set-2/
Is this for 10 1s 3p packs or would I get 5 sets for 2s 3p?

Edit: and yes, I have my own printer and plan on printing the cases myself
```

---
## \#661 Posted by: agniusm Posted at: 2018-11-12T20:23:48.330Z Reads: 255

```
Sorry. You mentioned modules which confused me. Yes, just order 10s 3p and leave a note if you need it as 2s3p. I  will make what you need. Cheers
```

---
## \#662 Posted by: XTLA Posted at: 2018-11-19T13:12:28.687Z Reads: 258

```
Just wodering if N.E.S.E will have some good deal for black friday/cyber monday 😋, might get some module.
```

---
## \#663 Posted by: agniusm Posted at: 2018-11-27T13:12:34.128Z Reads: 263

```
[img]https://i.imgur.com/PadhqiM.jpg?1[/img]
```

---
## \#664 Posted by: banjaxxed Posted at: 2018-11-27T13:29:24.483Z Reads: 264

```
Thanks for this design, I have to try it as not completely happy with velco and wire.
I did this to make it easier to print and no supports, printing now not sure if it is an improvement

![image|373x477](upload://oOhvupky6caaX59T0VgYdaRhNYR.jpeg)
```

---
## \#665 Posted by: agniusm Posted at: 2018-11-27T14:59:54.885Z Reads: 248

```
One more thing is to change fillets you have to chamfers. They print a lot better and final print will look much nicer.
```

---
## \#666 Posted by: banjaxxed Posted at: 2018-11-27T15:50:40.172Z Reads: 262

```
It's @mishrasubhransu's design. In fact I made a boo-boo, I am using your original NESE cases so there is only mounting on the outside and nothing for the inside. In any event always good to collaborate

0.6mm nozzle on a volcano, not really suitable for this but 10m print time
![image|666x500](upload://48cPlbPKYOMuIsQLfOWyIXNSH3v.jpeg)
```

---
## \#667 Posted by: mishrasubhransu Posted at: 2018-11-27T21:43:19.095Z Reads: 252

```
Looks good to me. Why do you think you made a boo-boo? Have you tested the springiness?
```

---
## \#668 Posted by: banjaxxed Posted at: 2018-11-27T21:58:02.246Z Reads: 258

```
I’m using the original cases so there is two rows of cases and using this mounting system does not secure the inside of each row

It printed ok and seems just as 💪
```

---
## \#669 Posted by: mishrasubhransu Posted at: 2018-11-27T23:25:20.935Z Reads: 260

```
I am a bit confused. Why do you have 2 rows of cases? Can I see your layout? Is it different from the one below?
![image|333x250](upload://oj7E8pyKsnuK7HWTdpKjQWGjy9x.jpeg)

Edit:
Now I get it. So you'll have to create a new part that just joins the middle part together. Just a flat plate. It will remain suspended in air. You are effectively turning it into 4P+4P module.

![image|333x250](upload://tdf1MPq9ZDFoCvdlZq8KaQmqI9v.jpeg)
```

---
## \#670 Posted by: banjaxxed Posted at: 2018-11-28T09:24:20.729Z Reads: 258

```
Sounds like a plan, thanks bro
```

---
## \#671 Posted by: Benjamin899 Posted at: 2018-11-28T11:57:39.629Z Reads: 254

```
Mine are stacked.
```

---
## \#672 Posted by: CamBo Posted at: 2018-12-01T21:34:23.397Z Reads: 251

```
Hi @agniusm, is the code working?  I can’t get the site to recognize ‘Wintersale’
```

---
## \#673 Posted by: Benjamin899 Posted at: 2018-12-01T21:36:26.928Z Reads: 247

```
did you try capslock?
```

---
## \#674 Posted by: CamBo Posted at: 2018-12-01T21:43:30.253Z Reads: 244

```
Caps or no caps, I get ‘code wintersale does not exist’
```

---
## \#675 Posted by: Benjamin899 Posted at: 2018-12-01T22:05:04.565Z Reads: 238

```
i am sure he will activate it soon.
```

---
## \#676 Posted by: agniusm Posted at: 2018-12-01T22:07:42.910Z Reads: 238

```
Hi. Sorry, tried all caps? Should be working
```

---
## \#677 Posted by: Benjamin899 Posted at: 2018-12-01T22:08:26.183Z Reads: 242

```
yep all caps works.
```

---
## \#678 Posted by: agniusm Posted at: 2018-12-01T22:14:34.708Z Reads: 251

```
BTW, just a heads up, I am expecting shortages of some bits as supplier is late with delivery. I will inform about the delay personally and it will be possible to cancle order with full refund if delay is unacceptable. Mainly concerns hardware not complete modules.
Cheers
```

---
## \#679 Posted by: agniusm Posted at: 2018-12-22T21:03:58.515Z Reads: 246

```
@banjaxxed. I have done a quick mock-up to see what could be done for you. I don't know if it will be stiff enough but here, final dimensions: 167.1x74.2x16.7mm

![slim_line|690x366](upload://36Bm6L3AyBGsXO7ZNT8EvUiNfNb.jpeg) 

![slim_line_2|690x366](upload://1dt555YcoYSQYHPOIz1vl42pM5H.jpeg)

I will run a print tomorrow. BTW your tabs are sent out as promised, today.
Cheers
```

---
## \#680 Posted by: banjaxxed Posted at: 2018-12-22T21:42:01.391Z Reads: 239

```
Thanks @agniusm please don’t expend any effort on my part, I had to butcher one of your stls in order to reach 13s pic incoming. Something like what you have may work in a Hummie deck build tho

Looking closer I probably should have waited nice minimalist design change there. 

In the 2 channels I have available I only have room for terminal ends at the end of 2 really long packs, should not be an issue given their snug solid location
![image|666x500](upload://llZXuj6MrdEa2HvLM9aP45MJVkc.jpeg) 

Sone glue is needed to fuse them, both are in two parts given their size, I may try to cell fuse the anodes hence the markings on the packs by snipping individual ‘buttons’ from the tabs and fusing those to copper strips running parallel there is just enough space

Not sure how crap this charge-only BMS is, it will mean a new charging solution or modding a 12s charger with a potentiometer.

It would be nice to be able to take it to Denver (if I go) and borrow or buy cells stateside, 10 minute job, that maybe something that becomes common in esk8
```

---
## \#681 Posted by: agniusm Posted at: 2018-12-22T22:10:08.029Z Reads: 233

```
I do not expect anything. It was for my own exercise when I saw you try to slim it down. I did skinned it to less than a cell itself and just want to see how tough it will be with all that material scraped off. If it works, well, another option is always good.
```

---
## \#682 Posted by: banjaxxed Posted at: 2018-12-22T22:13:53.287Z Reads: 236

```
For sure that would have worked and this includes a lid too! Really nice. Length was the killer for me.
Someone will definitely use it you should release on your site with proviso that it needs to be supported and in a sealed environment
```

---
## \#683 Posted by: agniusm Posted at: 2018-12-24T19:48:14.353Z Reads: 246

```
![20181223_100944|666x500](upload://uoecv2wG6d0TGW5VL3qpXJ6P37a.jpeg) 

![20181223_100959|666x500](upload://2hMonX5Yl6ojTLTv0WCK3N0YFCx.jpeg) 

Too flimsy for my taste to add to my shop but it works. Needs a vice to get it closed effortless. Good outcome is that it flexes length wise. So its probably thinest module ever :) unless you hammer down a cell to oval 😂
```

---
## \#684 Posted by: banjaxxed Posted at: 2018-12-24T19:51:58.025Z Reads: 236

```
like it, want it maybe enough to reprint, share and care? It is Christmas after all, my guess is 20mm height with lid in which case HAYA can do
```

---
## \#685 Posted by: agniusm Posted at: 2018-12-24T20:02:57.712Z Reads: 236

```
NOOOO! Its 17mm in height 😂 you will need to hamer down your cells to make them that 😂
Cell height is what you get so 18mm
```

---
## \#686 Posted by: agniusm Posted at: 2018-12-24T20:04:46.371Z Reads: 231

```
Sure will share if interested.
```

---
## \#687 Posted by: banjaxxed Posted at: 2018-12-25T09:22:02.677Z Reads: 237

```
Tardis? Wait it’s smaller then the cell radius, oof you clever man
```

---
## \#688 Posted by: agniusm Posted at: 2018-12-25T09:48:56.074Z Reads: 243

```
[2S4P SlimLine STL](https://drive.google.com/drive/folders/1a12YgQL3C1AGESJBbicjNjR83O2MKPnX?usp=sharing)
```

---
## \#689 Posted by: jaatis Posted at: 2018-12-25T10:08:48.588Z Reads: 245

```
Nice way of reducing wasted space! I like it.
Would making the v-slots solid help with rigidity?
![15c5967433d49c1dd665bb9ce84139b76d35b27d|690x366](upload://wwB7BriHZFtwMQ2cFaEN1feAZGp.jpeg)
```

---
## \#690 Posted by: agniusm Posted at: 2018-12-25T10:37:57.814Z Reads: 239

```
No. The cutouts where cells protrude make it flex.
I know it might sound like a waist of space. But i have tested various thicknesses to have as little material as i need to to make it rigid enough for assembly and protection.
```

---
## \#691 Posted by: agniusm Posted at: 2018-12-25T10:42:16.934Z Reads: 235

```
You can make it rigid with exotic materials but those cost 300-500usd per 0.5kg and require special printers to print which are very expensive too. So this is a compromise made so anyone could print them, they are safe and easy to assemble.
```

---
## \#692 Posted by: agniusm Posted at: 2018-12-25T14:00:49.428Z Reads: 236

```
Just a reminder that offer expires in a week so don't miss out ;)
```

---
## \#693 Posted by: mishrasubhransu Posted at: 2018-12-25T14:02:19.264Z Reads: 238

```
What offer?
```

---
## \#694 Posted by: agniusm Posted at: 2018-12-25T14:03:08.959Z Reads: 244

```
[quote="mishrasubhransu, post:693, topic:36847, full:true"]
What offer?
[/quote]

Winter offer with 15% off
```

---
## \#695 Posted by: agniusm Posted at: 2019-01-04T11:37:53.272Z Reads: 245

```
More common way of wiring PCM's balancing port(s), like bestechpower.

![10S8P_assembly2|690x366](upload://fupvYSPjA1vYVlasDHPeWuzCrhY.jpeg) 

![10S8P_assembly|690x366](upload://lBLUUcd5uUx8G9lAIsHO5AhkBoh.jpeg)
```

---
## \#696 Posted by: Benjamin899 Posted at: 2019-01-04T12:25:29.291Z Reads: 240

```
why switch between the negative and postive terminal?
```

---
## \#697 Posted by: xilw3r Posted at: 2019-01-04T13:50:43.050Z Reads: 236

```
it does not matter to which screw you tighten the balance cable, they both are literally the same spot as far as the BMS can tell
```

---
## \#698 Posted by: agniusm Posted at: 2019-01-04T14:10:25.156Z Reads: 244

```
Was quicker to cad and have them inline. I think this is basic stuff electrically and all should know that it is the same where on conductor you place your connection, it will get connected 😋
```

---
## \#699 Posted by: mishrasubhransu Posted at: 2019-01-19T15:13:43.536Z Reads: 246

```
I made a new enclosure for DieBieMS. It is a bit wider(5mm) than the standard NESE box and I have moved a few things around to attach the balance connectors while BMS is already mounted in place. It has more space for routing the balance wires and restricts them in a channel. The copper tabs are very easy to DIY now. Only one 90 degree bend.

Rest of the pics [here](https://www.electric-skateboard.builders/t/basic-nummie-skateshred-41-drop-down-tb-218-fs-6374-tb-63mm-reverse-10s4p-n-e-s-e-with-diebiems-fsesc-6-6-6x2-aliexpress-pneumatic-wheel/67482/37?u=mishrasubhransu). The pic below is a completely assembled working board. 
![IMG_20190119_064319|666x500](upload://zidwqtiz4f3WUI9klEnUmmrVz5r.jpeg)
```

---
## \#700 Posted by: mishrasubhransu Posted at: 2019-01-23T23:39:20.100Z Reads: 254

```
Rear view
![IMG_20190116_233028|666x500](upload://iEgjfdauxvK6a33NAD76NIMDG3m.jpeg)

Front 
![IMG_20190116_232937|690x350](upload://sB5qcY1eyh2CE2AZZl8tf1S0Szx.jpeg)
```

---
## \#701 Posted by: uigiroux Posted at: 2019-01-23T23:44:13.315Z Reads: 248

```
Such a beauty!
:heart_eyes:
```

---
## \#702 Posted by: agniusm Posted at: 2019-01-24T09:42:47.880Z Reads: 259

```
So, i want to be grumpy :) I had flames thrown at me for making some statements. Don't want to tag Winfly here as i don't want to put him off of hes development endeavour.
Will quote hes first post:
_1. Cost_
_  * It’s kind of expensive.  **€103.35**  for a 10s4p module to ship to the US_
_2. Size_
_  * it got that extended part for screws terminals. I don’t see it as a necessity. It adds length to the whole P group and IMO length is pretty important since most battery packs are made laying the 18650s along the length of the deck_

So the cost: 100USD NESE vs 80USD Winfly (and this is early access which most of the time is cheaper than regular)
20USD for stamped proper tab with raised nipple, plated, then proper low set foam for compression added must be worth that?
What got me is that he even does not want to share stl files, not to mention CAD's cause its bad for business.
In the end, the system started taking NESE shape with lower quality components costing marginally less.
Maybe its me but it does not make sense to me, and i was flamed for the things i said that became true in the end.
Am i weird?

On the better note, my system is going to be used in student formula E. Pakistan team will be using it.
![](https://c.ndtvimg.com/7j7u3nu_all-girls-pakistani-team-student-formula-competition_625x300_15_July_18.jpg)
 We were working on implementing temp sensors. Rules require to have one probe per 3 cells max with proximity of <10mm. I have found the sensor and implemented in NESE 8P module. it got wider by 3mm but is still compacts for car:
![](https://i.imgur.com/wmKynGg.png)
(Illustration, middle probe is placed correctly now)
![](https://i.imgur.com/xKnEWKC.png)
![](https://i.imgur.com/fMF73yy.png)
Its not public, but if someone has project requiring this capability, its available on request (stl or cad)
```

---
## \#703 Posted by: mishrasubhransu Posted at: 2019-01-24T11:14:01.764Z Reads: 244

```
The integrated temperature sensor looks fantastic. Congratulations that your system is going to be used by the Formula E Team. 

My next battery pack will be a slightly modified version of your thin profile module with some easy way to pass the balance data from one module to the next in a modular way and finally into the DieBieMS/other BMS along with thermistors per cell pack. 

Don't be grumpy, you have a great tested product.  I love the modularity, the safety, use of big m5 bolts for joining connections ... Even though these modules look good on paper, when it comes to more people adopting it, well, they will need to see several different implementations that has been tested in real world condition for 1000s of miles(collectively). **What would really help is for you(and other existing users) to assemble and showcase their functioning system**. That would instil the confidence required and give users ideas to put together their system. To put that in a different way, understand that a lot of the experienced builders just use welded cells because they can make very compact system and a lot of the newer builders are afraid to try NESE because they don't see a lot of builds based on that here(esk8 forum). You have a huge potential customer base but they need a bit of hand holding.
```

---
## \#704 Posted by: agniusm Posted at: 2019-01-24T11:46:41.288Z Reads: 238

```
Funny is, a lot of these are in the wild. I mean a LOT. But I see one or two builds. Then I gathered if people do not talk about them, that's a good thing, most of the time people start talking and looking for solutions when something does not work or have overall bad experience.
Sadly all the good comments and thanks I get by email so no point in sharing as it might seem fake
```

---
## \#705 Posted by: agniusm Posted at: 2019-01-24T11:55:34.189Z Reads: 250

```
Another thing I wanted to share is I am engineering some stuff for the printer. The major thing is automation. I have two inexpensive ideas to try. One is nearing test phase with conveyor part removal. This allows unlimited parts to me manufactured unattended autonomously. 
Here is most recent photo![20190123_162116|666x500](upload://m5kObEWbSaarO2uJK6F8CwbwsDk.jpeg) 
![20190123_162122|666x500](upload://5lzh1paeQeRSDPRxe9fhcV0dtQZ.jpeg) 
Another approach is using al2o3 porous ceramic plate with vacuum to hold parts while printing and then push them from build surface with lever. I am skeptical about this one as surface at the start of a print is very small for vacuum to work vut you never know. Needs to be tested.
If any of the solution will work, I will be able to cut my prices by further 10%.
```

---
## \#706 Posted by: mishrasubhransu Posted at: 2019-01-24T12:28:18.547Z Reads: 235

```
Well then one idea would be to encourage them(people saying thank you) to share a pic of their setup(on this thread or email them to you) and then you can put those pics here or on your web page, with their permission of course. You should def do that. Make different categories for their application and post pics under them.
```

---
## \#707 Posted by: mishrasubhransu Posted at: 2019-01-24T12:32:07.193Z Reads: 235

```
Conveyor seems to be the easiest to implement. Also i am skeptical about the vacuum because it won't let the bed heat up. Are you going to use tool steel plate for the conveyor, that is fed through certain distance using a servo?
```

---
## \#708 Posted by: agniusm Posted at: 2019-01-24T12:48:43.042Z Reads: 240

```
If vacuum holds, then there is no need for heat, after all heat is used to get prints to stick.
Conveyor will have a belt on top of aluminium heated platform. After print is finished, stepper motor will turn the conveyor and drop the part into collection bin. The another part will start and so on. I have 0.05mm stainless scheet to test as well as 0.25mm single layer carbon.

![20190124_144826|666x500](upload://eKEQxiIvibD3krFGrO9Z4xmC835.jpeg)
```

---
## \#709 Posted by: banjaxxed Posted at: 2019-01-24T14:25:43.457Z Reads: 225

```
Have you seen the endless Y axis design? It uses a rolling bed very innovative
Edit: you have indeed!
```

---
## \#710 Posted by: banjaxxed Posted at: 2019-01-24T14:33:18.052Z Reads: 225

```
Any chance that you would look into cell level fusing at some stage? A mod to the case design and the cutting of tabs is all that is required.

Also/or some balance wire conduit/passage where they are safe from a short. That’s nice work with the Fomula E car, this is useful to the above ^
```

---
## \#711 Posted by: agniusm Posted at: 2019-01-24T14:46:46.814Z Reads: 218

```
Yes, the blackbelt. Its good for long parts but smaller does not look too good when printed. I have not seen such printer producing same quality parts as conventional printers and you are constrained how you orient parts. You get away with some overhangs but there is the other side to it.
```

---
## \#712 Posted by: Benjamin899 Posted at: 2019-01-24T15:58:49.724Z Reads: 219

```
the moment i read conveyor belt i thought "Factorio". Congrats on the cooperation with Formula E. Great stuff, love the new lower profile.
```

---
## \#713 Posted by: mishrasubhransu Posted at: 2019-01-24T16:26:10.198Z Reads: 217

```
@agniusm, can this is printed without support? What settings do you recommend. I realize it varies between different printer setup but it will give me an idea.
```

---
## \#714 Posted by: agniusm Posted at: 2019-01-24T16:30:50.555Z Reads: 214

```
Sorry but what? If you are talking about NESE, they are designed to be printed without supports as is
```

---
## \#715 Posted by: mishrasubhransu Posted at: 2019-01-24T16:32:15.461Z Reads: 208

```
My question was about your slim file.
```

---
## \#716 Posted by: agniusm Posted at: 2019-01-24T16:42:16.427Z Reads: 217

```
Sorry but no. I have not changed my mind on this. Having read formula e rules, there is no requirement and their regulations are strict. Its a complexity over nothing. I see why you would want that on second life cell in your house.
Its possible. You can make the nipple as wide as the cell, add proper fr4 gasket to positive of the cell and drill out the nipple so it sits on cell positive side negative edge. Than just solder or weld your fuse wire.
OK, if you dont mind soldering, can assemble 10k of orders, i can do it, and it will cost same as the usual tab 😁
```

---
## \#717 Posted by: agniusm Posted at: 2019-01-24T16:42:57.269Z Reads: 212

```
No supports on that too
```

---
## \#718 Posted by: banjaxxed Posted at: 2019-01-24T17:21:00.065Z Reads: 215

```
I’ll pass thanks 🤭

But good option for diy so always worthwhile meshing ideas
```

---
## \#719 Posted by: agniusm Posted at: 2019-01-24T17:43:29.950Z Reads: 212

```
You are not determined at all mate 😂
For diy, yes. You can do it even with existing tabs i think. Just need to find a round gasket to cover up positive terminal. Drill a hole on the tab nipple and solder your fuses inside the nipple and to the cell. Inserting it might be tricky
```

---
## \#720 Posted by: mishrasubhransu Posted at: 2019-01-29T12:20:56.054Z Reads: 225

```
Hey @agniusm, I have raised this concern with you before, but still wanted to do it again for a sense of security. Since the new slim pack is specific to electric skateboarding, could you please put a divider in between? That will make sure that under no freak circumstances will the middle 2 cells come in contact with each other. Plus it will provide additional strength. A divider bar like in the pic below. Sure I have the cad and make the modification but this is for rest of the people. 

Edit: this is only for 2S packs. Like 4P+4P
![image|690x305](upload://gYNqLa9SOfAa3gL4J6hakjiWzRM.jpeg)
```

---
## \#721 Posted by: banjaxxed Posted at: 2019-01-29T12:28:07.728Z Reads: 223

```
Do you mean from flexing? I would suppose the packs should not be under stress, I think you designed some holders for the packs with a flexible type design, surely the flex should go into that?

If the pack flexes and the cell wrap disintegrates the only risk I can see if that the negative cans touch each other....which they already do at the negative pole

The cells in the tray are all the same parallel group, not sure how a short occurs in the scenario painted?

**EDIT:** Ah right I get you using the 2p in a single pack, yes that could happen & your suggestion makes sense. You could easily chop and add that before Agnius gets around to it
```

---
## \#722 Posted by: visnu777 Posted at: 2019-01-29T12:31:35.090Z Reads: 210

```
That's what I was thinking too, maybe we should add that it concerns the 2s packs only 😉
```

---
## \#723 Posted by: mishrasubhransu Posted at: 2019-01-29T12:32:16.236Z Reads: 217

```
The middle 2 cells are not from the same parallel group. I fear that say a crash happens and the impact makes the middle 2 cells touch each other momentarily. Then a short would happen producing a lot of heat and then melt the plastic leading to a full blown short.
```

---
## \#724 Posted by: rey8801 Posted at: 2019-01-29T12:37:31.442Z Reads: 228

```
@agniusm great solution for making battery safer and faster. I also found that what @mishrasubhransu suggested is right, a thin wall will make it sfare for internal series connection. One side completely close, while the other with a left space for the tab to go through. Plus I would also add a little cutout or a hole in the lid for the balance wire for the BMS.  This modification are really easy and everyone can do it by himself , but maybe you can make it public too, if you are interested of course.
I am making a deck with integrated enclosure and I will use your modules for the battery. Here same rendering of the prototype. The chambers are made to host your modules :wink:

![image|666x500](upload://zLe3JhYAVJVlADHlQmH2Kt8cGwf.jpeg) 
![image|666x500](upload://4iwncQgxXH750HZ473kegwoEwhG.jpeg) 
![image|690x479](upload://rjLX0jlsA2ocBlAbxFoQiFKhAey.jpeg)
```

---
## \#725 Posted by: agniusm Posted at: 2019-01-29T13:03:24.316Z Reads: 224

```
My initial suggestion was to place a piece of paper, the one use for baking. Its thin, impregnated and can withstand high temps. I did not want to increase the size of the module at all, but if community is addressing this, i am all over. I will make necessary changes and re-upload to my website. I can add this to 2SxP packs too, would be triangle shape, sloping towards 2S tab to get it in but it should cover for cells not to touch. I it will increase module by .9mm as i need 2 extrusion to make up the wall @ 0.45mm to matter.
@rey8801, fantastic work on CAD, love the board. At first glimpse i thought it was real photoshoot in light box.
```

---
## \#726 Posted by: mishrasubhransu Posted at: 2019-01-29T13:22:26.570Z Reads: 219

```
[quote="rey8801, post:724, topic:36847"]
Plus I would also add a little cutout or a hole in the lid for the balance wire for the BMS
[/quote]

Actually that is not desirable on the lid because then you can't open the lid and service the cells(say you are upgrading them or replacing them). Ideal would be to do it underneath and route everything from underneath. Plus his current design has v shape cutouts exactly for that purpose.
```

---
## \#727 Posted by: rey8801 Posted at: 2019-01-29T13:23:54.221Z Reads: 226

```
thanks! yeh rendering is pretty cool. It makes photo realistic reconstructions. Concerning the 2SxP modules I also thought about a piece of paper in between. In that case I would opt for fish paper since it has been made for that. I also like a lot the slim version. If I missed in thread I am sorry, but do you perhaps share the CAD file of the modules? I mean STL is ok but a bit more nasty to work with it.
Thanks for listening the community!
```

---
## \#728 Posted by: rey8801 Posted at: 2019-01-29T13:26:47.069Z Reads: 227

```
True for the hole but the cut out in the lid would be on the side so you can still remove the lid since the balance lead will just slide out. At least in my imagination can still do it :grin:

![IMG_20190129_142550|281x500](upload://93lRYOCLeEjNetgAyXpejVSnYDQ.jpeg)
```

---
## \#729 Posted by: agniusm Posted at: 2019-01-29T13:45:39.429Z Reads: 213

```
You have a terminal exiting at front and back. Why would you want another exit for balance wire and solder directly to the tab when you can use ring terminal and bolt it where it suppose to?
```

---
## \#730 Posted by: rey8801 Posted at: 2019-01-29T13:46:42.436Z Reads: 214

```
I perfectly see your point but in case of the internal S connection in the 2s module you need a balance lead there. No?
```

---
## \#731 Posted by: agniusm Posted at: 2019-01-29T13:55:14.541Z Reads: 225

```
Its not internal. there are 4(2S4P) or 3(2S3,2P) connections at both ends of the module. There is no need to modify for balancing wires. All works as is ;)
You can see it here:
![image|666x500](upload://fVRW5FYw4BdaKOwK6PrfjenFH7e.jpeg) 
I am measuring voltage on 2S but at the bottom you have bolt on both sides to connect your balance wire. On 2S3P and 2S2P there is only one bolt on one side. You can also cut the tabs and have only wire exiting tab opening for balancing and leaving bolts out for compactness.
```

---
## \#732 Posted by: mishrasubhransu Posted at: 2019-01-29T14:03:00.932Z Reads: 224

```
I basically chose not to have the compactness and made the series connection from outside. That's why I was asking for a big divider in between. Haha.
```

---
## \#733 Posted by: rey8801 Posted at: 2019-01-29T14:10:17.115Z Reads: 227

```
I see. So just to be sure I got it 

![image|690x460](upload://2aoQ63r3l5j28hYJmUoXgzxGU2e.jpeg) 

Is it correct?
```

---
## \#734 Posted by: agniusm Posted at: 2019-01-29T14:11:31.651Z Reads: 222

```
Yes. That is correct
```

---
## \#735 Posted by: rey8801 Posted at: 2019-01-29T14:12:03.071Z Reads: 219

```
perfect then no modification needed :wink:
```

---
## \#736 Posted by: Benjamin899 Posted at: 2019-01-29T14:16:39.497Z Reads: 221

```
took me also a moment the first time i build mine, but works like a charm.
```

---
## \#737 Posted by: rey8801 Posted at: 2019-01-29T14:20:28.943Z Reads: 225

```
it indeed looks super clean. I am going to use it for sure
```

---
## \#738 Posted by: agniusm Posted at: 2019-01-31T09:46:03.682Z Reads: 231

```
Made some changes for requested futures. Please chime in to asses before i print samples and waist plastic :slight_smile:
This one is for 2S4P:
![2S4P|690x366](upload://2DENEJ65s0XpCut7eHA8V1M8FxN.jpeg) 
and for 4P+4P:
![4P%204P|690x366](upload://AkZ24Bt8oayekCRKHbkzDsJXnSH.jpeg) 
The barrier is 0.9mm wide so add that to final module length
```

---
## \#739 Posted by: rey8801 Posted at: 2019-01-31T09:51:44.399Z Reads: 218

```
looks good to me :wink: Thx!
```

---
## \#740 Posted by: mishrasubhransu Posted at: 2019-01-31T09:58:39.336Z Reads: 220

```
Why not have a wall with a constant slope from start to end in both cases. Save plastic?

Also in the 1st case you can raise the wall until it just hits the copper tab center. Did I make sense?

Edit: ignore the second thing I said. 

Also, BTW, why .9mm wall? What's your nozzle size?
```

---
## \#741 Posted by: rey8801 Posted at: 2019-01-31T09:59:55.163Z Reads: 214

```
yeh I tought it already passed the tab center. I need to print one and fit a tab to better visualise it
```

---
## \#742 Posted by: sebaszz Posted at: 2019-01-31T11:04:24.166Z Reads: 213

```
very nice design, really like how you developed this product :+1:
have you considered designing double stack module with the batteries nested. 
The hardware remains the same only new module design. 
I would be interested, can work on the design if there is a compatible fusion 360 file.
```

---
## \#743 Posted by: agniusm Posted at: 2019-01-31T14:00:36.247Z Reads: 213

```
[quote="mishrasubhransu, post:740, topic:36847"]
from
[/quote]

No point in wasting time or plastic. i would not had the wall at all but it is good to make these larger module more rigid hence triangulation.
@sebaszz, can you draw up what you mean? On request i can provide CAD files. I believe @mishrasubhransu has some on gdrive as mine are exported and it is extra job i would rather not do :) when there is availability.
```

---
## \#744 Posted by: mishrasubhransu Posted at: 2019-01-31T15:21:23.271Z Reads: 205

```
I'll share the files with him.
```

---
## \#745 Posted by: deucesdown Posted at: 2019-01-31T15:30:27.956Z Reads: 206

```
@mishrasubhransu Cad links for me too! lack of cad stopped me making use of them. tried to reverse engineer the model but slow progress due to being too n00b.
```

---
## \#746 Posted by: mishrasubhransu Posted at: 2019-01-31T15:38:21.241Z Reads: 204

```
I have iges and solidworks files. Hope you both can use them.
```

---
## \#747 Posted by: ZachTetra Posted at: 2019-01-31T15:41:35.167Z Reads: 205

```
Has anyone mentioned using a 2 sided end plate what gets bolted to the deck? Instead of wiring say 3 packs to make a 6s4p, you would put 7 ends and have no wires

Basically a end divider with contacts on both ends to make series more compact
```

---
## \#748 Posted by: mishrasubhransu Posted at: 2019-01-31T15:47:52.296Z Reads: 207

```
A quick sketch maybe?
```

---
## \#749 Posted by: deucesdown Posted at: 2019-01-31T15:50:37.885Z Reads: 217

```
Oooh this is clever if I understand.

Basically, NESE uses copper things with 2 holes to do the series connections. I think Zach is saying to change the tab to have a section that can be bolted to the deck. An L-shaped extension.

So the brackets would serve as mounting tabs, and as series connections.

I'm thinking, since it's bolted, you can just add a piece of L shaped metal to the bolted together stack -- no need to modify the series tab.

This could save me hours of cad work, but worried about vibrations.
```

---
## \#750 Posted by: ZachTetra Posted at: 2019-01-31T15:55:46.935Z Reads: 218

```
![image|375x500](upload://v2kLtnfh7kbwMCaeyIfq6REjLbF.jpeg) 

Ignore the calc

The bus is common to both sides
```

---
## \#751 Posted by: deucesdown Posted at: 2019-01-31T15:57:17.866Z Reads: 206

```
dude plz rotate lol. my neck!
```

---
## \#752 Posted by: mishrasubhransu Posted at: 2019-01-31T15:59:51.970Z Reads: 200

```
I like your idea but it makes the modules rigid. Which is okay for decks that are pretty stiff.
```

---
## \#753 Posted by: mishrasubhransu Posted at: 2019-01-31T16:00:59.386Z Reads: 196

```
Aah, I get it. You are saying to do away with the plastic boxes but just use the copper tabs with support to directly mount on the deck. Could work. You wanna cad it up and show us how it looks?
```

---
## \#754 Posted by: agniusm Posted at: 2019-01-31T16:18:39.639Z Reads: 202

```
Makes no sence. Enclosures are there to restrain cells from flying arround so they are properly seated even with exsessive vibrations. Also mechanical and weather protection, at least first stage. The space you are saving is nothing compering to trouble you are adding. Its better to go and spotweld the pack if you are counting millimeters.
```

---
## \#755 Posted by: agniusm Posted at: 2019-01-31T16:24:07.606Z Reads: 197

```
Have not answered all the questions. Most print with 0.4mm nozzle and extrusion width with it is 0.45mm mostly so 0.9 make two perimeters which is enough for it not to be floppy and matter.
You cant have both cases with the same slope. 2sXp has full tab and the wall would not allow it to be inserted while 4p+4p has 4 tabs and full separator is no problem
```

---
## \#756 Posted by: mishrasubhransu Posted at: 2019-01-31T16:31:35.447Z Reads: 199

```
By the same slope I didn't mean same slope for both of them, but rather a constant slope. But you have explained above why.

Yeah, the cad looks nice. Thank you for listening to us.
```

---
## \#757 Posted by: agniusm Posted at: 2019-01-31T17:05:39.685Z Reads: 202

```
Just to confirm, by the slope you mean trapezoidal cutout i have and rectangular separator in your model?
```

---
## \#758 Posted by: mishrasubhransu Posted at: 2019-01-31T17:13:17.849Z Reads: 203

```
Yes, exactly.
```

---
## \#759 Posted by: Hummie Posted at: 2019-01-31T17:16:07.581Z Reads: 208

```
[quote="agniusm, post:702, topic:36847"]
We were working on implementing temp sensors. Rules require to have one probe per 3 cells max with proximity of &lt;10mm.
[/quote]
How many sensors wires you think you need for a whole pack of 48 cells?  Be nice if could use one long sensor wire for numerous cells.  Looks like that’s what you’re maybe doing in the photo
```

---
## \#760 Posted by: agniusm Posted at: 2019-01-31T17:29:04.392Z Reads: 204

```
Its a 3 wire sensor so you need to parallel required amount of sensors on 3 wires. They work in parasitic 2 wire mode but some data is lost on larger arrays. The SAE rules require one data point per 3 18650 cells but i would not go that crazy myself, one sensor per module would be enough.
```

---
## \#761 Posted by: Hummie Posted at: 2019-01-31T17:36:05.454Z Reads: 201

```
Assuming one sensor per module how much would that roughly cost?  Like the possibility of having it work as a safety feature sending info to the Vesc if it gets too hot n could tell u
```

---
## \#762 Posted by: mishrasubhransu Posted at: 2019-01-31T17:58:33.227Z Reads: 197

```
Diebiems can take cell temperature data and relay it to the VESC. Already.
```

---
## \#763 Posted by: Hummie Posted at: 2019-01-31T18:03:10.264Z Reads: 202

```
It would be adding sensors either way.  Getting the voltages would be nice but the Vesc could accept a temp sensor as is with no more electronics I think
```

---
## \#764 Posted by: agniusm Posted at: 2019-01-31T18:16:22.649Z Reads: 205

```
Its a daizy chainable sensor. You cant just plug it in. Sensors have their own signature like wifi mac address. You need to read that and implement it in your final code. The stuff works on arduino so its simple but you need means of interfacing between sensors and controller or bms. Module sensors >>arduino or similar microcontroller>>lcd output or controller/bms or CAN output.

Edit: DieBieMS has CAN so it might be possible bit you are in open waters as i have no time for that. Soon i will make my pcb to be inserted mid-print and buried under plastic
```

---
## \#765 Posted by: deucesdown Posted at: 2019-01-31T19:23:23.656Z Reads: 218

```
[quote="agniusm, post:764, topic:36847"]
Soon i will make my pcb to be inserted mid-print and buried under plastic
[/quote]

Some kind of daisy chainable balance wire connection points would be awesome. I've been thinking about this, with all the pcb-per-parallel-group battery builds. It's tricky doing the daisy chain in a safe and reliable way.

If power (already is daisychain), temperature, balance wires are all daisy chain, it would make wiring much neater and more modular.

Like this for balance wires:

https://www.electric-skateboard.builders/t/arch-s-build-log-kaly-nyc-build-dual-6374-focbox-12s4p/25995/1
```

---
## \#766 Posted by: agniusm Posted at: 2019-01-31T19:52:30.460Z Reads: 219

```
Its possible to do it the easy way. Question is, are you preapred to pay?
You need distributed BMS. Look at eMus bms system. Then simple pcb design with spacing between NESE terminals for slaves:
![net-resizeimage-35|690x460](upload://50B7C4ExH5Q2WIFq1cBeatj3V50.jpeg) 
and you have powerfull balancing (1.2A) integrated temp probe and 2 wire interface.
```

---
## \#767 Posted by: agniusm Posted at: 2019-01-31T20:02:17.665Z Reads: 223

```
This is the first thought of using ffc cable to mount temp probes:

![20190131_213447|666x500](upload://nOPByZIl2zrPYIDUFRXBigs54ka.jpeg) 
and there is 2 types of the probe, TO-92 and uSOP but later one is so expensive that it does not make sense:
![20190131_213019|375x500](upload://b3qBcNK0dFGVNbhM92YIrCXnZwx.jpeg) 
Soldering that many sensors would be total pain in the ass and uSOP being .5mm pitch does not help. So i scrapped that idea, settled on TO-92 and went pcb route as you can have stencil where to lay probes and they are 1.25mm pitch which is workable.
```

---
## \#768 Posted by: deucesdown Posted at: 2019-01-31T23:41:14.807Z Reads: 218

```
Oh this is good stuff!

https://www.electricmotorsport.com/ev-parts/batteries/battery-management

That module is for lifepo4 but voltage range looks okay. $16/pc. But the control unit is like $400+, and additional for bluetooth (50-100?) or display (200+?). Yow.

This mini bms though...

https://emusbms.com/product/bms-mini
- 6 to 16 cells
- bluetooth!
- only 200ma balance current, but that's more than usual
- $$$$$$ I see below at 250 euros

https://www.faktor.de/bms/emus-bms/

very sexy stuff!

But the more I think about it, the more I think I just need monitoring/alerting. I can balance offline if monitoring says it's warranted.
```

---
## \#769 Posted by: agniusm Posted at: 2019-02-01T07:20:38.803Z Reads: 208

```
I think diebiems is good solution. There is no point overcomplicating and spending a lot of money over couple thin wires :)
```

---
## \#770 Posted by: mikenyc Posted at: 2019-02-01T15:29:36.671Z Reads: 207

```
can you make a 20700 version?!
```

---
## \#771 Posted by: agniusm Posted at: 2019-02-01T17:54:11.989Z Reads: 201

```
Not likely
```

---
## \#772 Posted by: agniusm Posted at: 2019-02-01T18:00:05.474Z Reads: 217

```
Printed 2 samples. Forgot that 2sxp module has long tab and spacer offsets it. Good thing it still fits and the offset is not that big.![20190201_163201|666x500](upload://7L6XT2duWI09DTFOIAt598TSKMy.jpeg) 

![20190201_163752~2|637x500](upload://cBgA6FYobPPjdu4MERBU7L0Vq2i.jpeg)
```

---
## \#773 Posted by: mishrasubhransu Posted at: 2019-02-02T03:53:23.587Z Reads: 216

```
I had made a minimalistic NESE module a while back. Not truly "no solder", because the ends are supposed to be soldered. I guess they are supposed to be velcro-ed to the deck, because I removed the mounting holes. The dimensions are: 83.4mmx74mmx22mm. The height can be reduced further based on the slim design.
![image|690x430](upload://hHOduFm87DLXjfAnPe85TogDu7R.jpeg)   
![image|564x500](upload://kCqjnC4WLVes8HiLo8ae6YVLLKq.png)
![minimalistic_NESE_1|690x439](upload://gtzM9FQGNmfz0tlWqfFlFAaI3Py.png)

I made them after I realized how much of a hassle it was to make and assemble these guys
![image|465x414](upload://3PJjzIrhW5y4GDrCBUGD0Cvhm7p.jpeg)
```

---
## \#774 Posted by: rey8801 Posted at: 2019-02-02T12:07:37.720Z Reads: 209

```
I was thinking in the open module why not use a nut and a bolt instead of two bolts? You don't have to relay on 3d printed threads and it will hold the compression better. So you just play a nut on one side and screw the bolt from the other. The spacer in between can be 3.1mm in diameter and no thread. Screw and bolt place in diagolan layout to even the pulling force.
```

---
## \#775 Posted by: mishrasubhransu Posted at: 2019-02-02T14:17:53.670Z Reads: 210

```
I have 10 of those modules sitting tightened for several months and they are still intact. I just have a hole rather than a 3d printed thread and use a screw with tapping threads. This design works, just that it is a pain to assemble and disassemble compared to box design.
![Screenshot_20190202-091124|690x278](upload://8Sjmq1ItcH7FDb5qhbgR4wWVvve.png) 

What you are suggesting, in my opinion, will be equally difficult to assemble and also produce a twisting force. But give it a shot, maybe you'll make it better.
```

---
## \#776 Posted by: rey8801 Posted at: 2019-02-02T15:09:23.229Z Reads: 205

```
ah didn't know that they were actually tapping screws, I thought they were normal screw.
Definitely the assembly would be equally difficult. Well compare to spot welding would still be 5 times faster. What I like of using bolt and nut is that you do not relay on the 3d print part for keep the compression. I will try like that. Thanks man!
```

---
## \#777 Posted by: Benjamin899 Posted at: 2019-02-02T17:10:09.921Z Reads: 197

```
love that design. Well that little bit of soldering is totally ok. The screw took some valuable space.
```

---
## \#778 Posted by: deucesdown Posted at: 2019-02-02T17:46:34.859Z Reads: 209

```
[quote="rey8801, post:776, topic:36847"]
relay on the 3d print part for keep the compression
[/quote]

While technically you're correct, his design uses structure and leverage very well. It's unlikely that losing compression will be a problem with PETG printed modules. The "flex" part of the compression comes from those Poron cushions.

You should print a module and check it out.
```

---
## \#779 Posted by: rey8801 Posted at: 2019-02-02T17:51:08.596Z Reads: 207

```
I mean I was talking about another module. The one @mishrasubhransucame out with. I think thst also his solution is really good and I am going to use it actually since the original NESE module are too big for the board and configuration I want. I am the first one using 3D printed parts but of with the same design and space needed I can replace plastic support with metal, then I will do it. Probably is over killed but since takes the same effort. I will aslo add a little cleft for a zip tie. Probably not need it but doesn't cost much.
```

---
## \#780 Posted by: mishrasubhransu Posted at: 2019-02-04T07:23:25.450Z Reads: 213

```
So I made the slim version(how Agnius did) of the minimalistic nese module. it works great except that when using compression tabs it is very hard to put the cover on. The compression is pretty solid atleast in the 4p modules because of the short wall distance. The dimensions are 83mm x 19mm x 74mm
![IMG_20190203_172717|500x666](upload://eMpxU0ni3DZLvwFuH0PzAaOEwsc.jpeg) 
![IMG_20190204_020429|500x375](upload://aLRefEBE7WYqSMZsmFuh9s7EGZZ.jpeg)

 Next iteration will use just 2 screws from the side, something like the design below. It will also greatly help with the compression on the top. Might go with the tested 4 screw design if this doesn't work well.
![image|690x360](upload://3ttKpoXDIZzS0A2KhavDDxgluQn.jpeg)
```

---
## \#781 Posted by: mishrasubhransu Posted at: 2019-02-06T13:16:13.767Z Reads: 206

```
@agniusm, in your designs, the box is what keeps the compression right and not the lid? The lid is just there to keep the cells from flying out? I am asking because i was wondering if i should make the lid strong enough to help with the compression or just enough stay in place. 

dim: 77x75(along len of cell)x20
![image|690x399](upload://qCwHvHsvMnPGIKsf7MyvlOZ64b8.jpeg) 
![image|690x209](upload://iPbG4DmigEaX0eKTneEFJqfit8Q.jpeg) 
![image|690x324](upload://ez6It0xFeWjMZS2BctxgMXsDVBM.jpeg)
```

---
## \#782 Posted by: agniusm Posted at: 2019-02-06T13:39:05.982Z Reads: 203

```
No. The lid helps with compression. You can see a thin lip on the bottom enclosure where the lid mates. I get away having them thin as they have support to the inserted tab. The greater P count, the more lid is important.
Dug up old photo of the difference
![DSCN1177|666x500](upload://vGfU7GFIHqNIe3NUCUkNULPx6f4.jpeg)
```

---
## \#783 Posted by: mikenyc Posted at: 2019-02-06T15:08:50.863Z Reads: 198

```
are the STL's for these available? I'm going to buy a 3d printer soon, this will be a great first print

@mishrasubhransu @agniusm
```

---
## \#784 Posted by: deucesdown Posted at: 2019-02-06T15:22:28.314Z Reads: 199

```
originals are here

http://18650.lt/index.php/resources/

If you look around on the site, there are many tips and tricks for printing the modules.

The rest you have to get from the creators directly.
```

---
## \#785 Posted by: rey8801 Posted at: 2019-02-06T15:26:58.312Z Reads: 196

```
I hope you are going for the Cr10s pro. I have the Cr10S and it's amazing but needs to be modified a bit to print really well. Over the year I pimped and I am happy with it, but hte Cr10s pro comes with all the upgrades that you need...for 520-580 Euro is the best you can have...I am so tempted to buy it...:stuck_out_tongue:
Sorry the off topic.
```

---
## \#786 Posted by: mishrasubhransu Posted at: 2019-02-06T16:15:14.499Z Reads: 199

```
Just use the original files. Mine are not tested and everchanging. Haha. 

But if you need anything in particular I'll provide the cad files. Shoot me a pm.
```

---
## \#787 Posted by: Hummie Posted at: 2019-02-06T17:04:07.526Z Reads: 205

```
These are A mm shorter and a mm taller at 74 long n 21mm tall. 
If anyone is interested in this super minimalist design using epdm rubberbands and copper strip pressed on a 3D prints I’ll post it when done tonight 

...![image|375x500](upload://![image|375x500](upload://wibeVe6TUm50DWBOfBCGQnAaybz.jpeg) wibeVe6TUm50DWBOfBCGQnAaybz.jpeg)   write me.  Or if you have any advice on the design 
If I get these bands in bulk especially I think this could be cheap.  
I believe, based on my own thoughts alone, that using bands is more reliable compression than just a print or even with a thin strip of poron.   Don’t know how much you’re compressing the poron but I hear between 20-60% is best for least compression set and staying within the compression zone. 
I just altered the design for a lot of flexibility and an individual band compressing each cell. 
I’ll press the copper and insert it tonight under the guard for you to see.  Between packs I just use a long exposed part of the strip giving a lot of room to twist n flex. Very easy to press and trim w a print and using a guard to protect cells from the sharp edge.  Too impatient to post these when done...I’ll post Them done tonight.
```

---
## \#788 Posted by: mishrasubhransu Posted at: 2019-02-06T18:04:12.319Z Reads: 191

```
Hummie, do you have any plans to make it look more polished? Rubber degrades over time, do you keep replacing them?
```

---
## \#789 Posted by: agniusm Posted at: 2019-02-06T18:27:38.292Z Reads: 195

```
Looks like you have butyl rubber. If its generic stuff compression set resistance could be fair comparing to poron - exelent. I wont post numbers as its irrelevant when there is no definitive data on rubber hummie used. You say it looks better physically but most of the time it is not how it feels or looks but how it performs under the skinn. I saw butyl rubbers get compressed and do not recover in 2 years. Same would apply to stretch or elongation.
```

---
## \#790 Posted by: mikenyc Posted at: 2019-02-06T18:49:31.227Z Reads: 200

```
I was looking at this one

https://shop.prusa3d.com/en/3d-printers/180-original-prusa-i3-mk3-kit.html#

What do you guys recommend?
```

---
## \#791 Posted by: Hummie Posted at: 2019-02-06T18:52:37.037Z Reads: 200

```
Epdm rubber bands which are more durable and heat resistant than nitrile and in terms of material in use its a lot more. True poron is really good compression set but these bands...who knows and never seen comparison.  I would like to compare!  And can easily add more bands if needed. I’ve got two on there now
```

---
## \#792 Posted by: agniusm Posted at: 2019-02-06T18:54:40.465Z Reads: 193

```
Btw, some advice on using poron (urethane blend) came from a person who designed battery for zero motorcycles as i was leaning towards bisco silicone with higher temperature rating and compression force. I just want to clarify for people that my design is not based on poke and pick model, but rather investigation and studie of mechanical, thermal properties and testing of various elastomers and materials. I know its to early to make boldest claims since 2 years have past fom first modules out the door. But i am very confident.
```

---
## \#793 Posted by: Hummie Posted at: 2019-02-06T18:56:52.134Z Reads: 186

```
I know you’ve tested the crunk out of them but...based on no science and just assumptions I think a band with way more material in use (compression/tension) I think it’s a contender.
```

---
## \#794 Posted by: agniusm Posted at: 2019-02-06T18:57:51.345Z Reads: 188

```
I am not saying that its not enough force but rather how long it can keep it. Sure you can swap the bands every 2 years and its viable diy solution but me selling modules have to be 110%.
```

---
## \#795 Posted by: agniusm Posted at: 2019-02-06T19:03:39.463Z Reads: 196

```
You know that size does not matter but the punch? And thats not sex talk :D Cause size matters in bed :smiley:
Take 4130(US) carbon steel and something generic, like CRxxx(eu) steel. You will need far less of the 4130 ( chromium molybden blend)
```

---
## \#796 Posted by: rey8801 Posted at: 2019-02-06T19:11:55.962Z Reads: 192

```
We are off topic here. Ask on the thread about 3D printing. Anyhow believe me save the money and get a cr10s pro.there is no reason to spend on a old prusa compare to a new creality. Even my cr10s is conperable to the prusa.
```

---
## \#797 Posted by: Hummie Posted at: 2019-02-06T19:12:58.089Z Reads: 198

```
As I understand it based on people who sell the stuff, whatever stuff, they all have different compression set but the more material the better. Yea poron is great but if using like a 1mm piece even if compressed within its ideal percent, a higher compression set material may be better in use and keep compression longer.  Wish there was an easy challenge we could do.  Even poron will eventually even compress
```

---
## \#798 Posted by: agniusm Posted at: 2019-02-06T19:21:45.452Z Reads: 198

```
In my case i dont want a lot of material to allow cell to move more than its needed. I spaced inside to allow for 50-60% compression which leaves ~0.8mm of compressed foam. Not much for cell to flap arround, sure not applicable to boards as they are mounted flat on deck and forces are in different direction.
```

---
## \#799 Posted by: deucesdown Posted at: 2019-02-06T21:14:00.907Z Reads: 198

```
[quote="mikenyc, post:790, topic:36847"]
What do you guys recommend?
[/quote]

IMO the one you're looking at is the sweet spot (prusa mk3)
```

---
## \#800 Posted by: Mich21050 Posted at: 2019-02-06T21:14:52.394Z Reads: 195

```
I can recommend the Ender 3. It's a geat printer.. you can add auto leveling later on too.. :slight_smile:
```

---
## \#801 Posted by: mikenyc Posted at: 2019-02-06T21:15:28.476Z Reads: 191

```
i just ordered the creality!
```

---
## \#802 Posted by: Mich21050 Posted at: 2019-02-06T21:15:41.094Z Reads: 189

```
Which one? :smile:
```

---
## \#803 Posted by: mikenyc Posted at: 2019-02-06T21:16:27.778Z Reads: 185

```
the cr10spro
```

---
## \#804 Posted by: deucesdown Posted at: 2019-02-06T21:22:54.507Z Reads: 187

```
should be good, but you have some limitations.

bowden makes printing flex difficult. hotend temperatures limit you to PLA, ABS and PETG (not sure on this one for cr10spro).
```

---
## \#805 Posted by: rey8801 Posted at: 2019-02-06T21:26:51.983Z Reads: 190

```
you say right, but the cr10 pro has capricorn XS tube, better extruder for flex filament ecc... Watch here...towards the end flexlible filament too...https://www.youtube.com/watch?v=d2oD4lktOT4
I have a cr10s and the pro has all the parts I updated along the years.
```

---
## \#806 Posted by: rey8801 Posted at: 2019-02-07T09:59:08.947Z Reads: 193

```
@agniusm I am going to buy the tabs for me and my friend. I will need the 8p with both ends that you have on the website, so no problem, but my friend want ot go for a 3p battery. Do you have the same double ends tabs but 6p instead of 8p? Thanks a lot.

PS: I just realised that your domain is .it. Are you from Italy?
```

---
## \#807 Posted by: mishrasubhransu Posted at: 2019-02-07T10:02:36.244Z Reads: 191

```
LT. Lithuania 

I am pretty sure he just has one size i.e. 8p and then cuts from there accordingly. But maybe he has leftovers from someone ordering 2p.
```

---
## \#808 Posted by: rey8801 Posted at: 2019-02-07T10:05:20.211Z Reads: 196

```
ahahahah my bad. I mean my computer didn't help ![image|598x39](upload://2p7pcZm00hfjfbcS3l6aXqKBuaV.png) 
:rofl:

But then if you have to cut it no possible to do the internal series connections anymore. Only sinlge module for 3p configuration. i mean you have to solder the other end and have left over tabs, which is a pity.
```

---
## \#809 Posted by: visnu777 Posted at: 2019-02-07T10:13:31.474Z Reads: 185

```
In my upcoming battery build I'll use the 2s3p neses for a 12s3p, it'll work when you reverse the poles on the other half of the pack. Then you can use a 6p nese tab at the end to connect both rows in series
Edit: I'll assemble them later and upload pictures
```

---
## \#810 Posted by: agniusm Posted at: 2019-02-07T10:15:48.626Z Reads: 185

```
It is possible. I have mentioned before. You only loose an option to choose where to attach balance wire. With 2s4p you can do that on left or right and with 2s3p and 2p just on one side.
And your computer displays correct for Italy it would be .it and for Lithuania .lt caps would look .IT and .LT :)
```

---
## \#811 Posted by: rey8801 Posted at: 2019-02-07T10:16:22.008Z Reads: 191

```
I see indeed. It's still fine. Only the left over tab is a pity but for the rest you can still do it. I was thinking to use the other end for the balance lead connections that why I said it won't be possible with one end only.
Actually the guy is making the battery for the same deck as you. If you have a special module to better fit the integrated deck would be awesome.
```

---
## \#812 Posted by: rey8801 Posted at: 2019-02-07T10:17:50.359Z Reads: 196

```
Yeh indeed you only loose the double option for the balance lead. Not a big deal. Yes the domain fooled me :laughing:
```

---
## \#813 Posted by: agniusm Posted at: 2019-02-08T13:28:06.597Z Reads: 207

```
So Mr.XXX got a cracked case. Don't jump to conclusions as lots could be happening here. He PM'd me but i would like to stay open and disclose every detail:
![ee69dfb6fb36f20b7ca7f4bcef72d8f320f3a0b4_1_666x500|666x500](upload://zkCqVdpRrJle9tXf0liOyv0wRFW.jpeg) 
My first impression was, it prints like shit :D, for a machine costing tens of thousands, its bad :) And we are talking xxxxxxsys.
Modules are printed in ABS. I sell mine done with PETG so there is interesting data point. Next, i admit that for such mounting and flexible boards the spot where it cracked is week. They were not intended to be used this way but still, its good feedback.
So i have done little changes that should improve that. I don't know if i will change all of the modules or just the ones meant for skateboards. Probably all, just need time to update and reupload for those downloading.
Here are changes i made and test samples are being made atm:
![cc7e046dcde27691828ea515a7d3caa307e1af05_1_690x360|690x360](upload://l4DRKniNHLj9h0LAHmABlbQo5ld.jpeg) 
![cc7354271e5f3061270788f26dfa5f73cd38b270_1_690x360|690x360](upload://s0DwTukOtrbdyhul95VFvHag556.jpeg)
```

---
## \#814 Posted by: rey8801 Posted at: 2019-02-08T13:42:21.572Z Reads: 195

```
Probably in case of slightly flexible deck is better to use the 1s modules since they allow more flexibility compare to the 2s ones. Can be wrong but @mishrasubhransu used the 2s modules and packed them perpendicular to the long deck axis. Then he fixed them to the deck on the side. In my mind in this way the net vector forces are on the side while the modules are pushed downwards when the deck flex a bit. Still better a crack since you can replace the module. In case of spot welded battery you will end up with a disconnected weld and you need to disassemble the whole battery most of the time.
```

---
## \#815 Posted by: mishrasubhransu Posted at: 2019-02-08T16:20:51.677Z Reads: 191

```
[quote="rey8801, post:814, topic:36847"]
Probably in case of slightly flexible deck is better to use the 1s modules since they allow more flexibility compare to the 2s ones.
[/quote]
I didn't quite get what you were trying to say. Could you explain in a different way?

By the way @agniusm, my way of mounting would reduce stresses due to flex. All the flex will be taken by the flexi-stands.  BTW, is that what you meant by "it's not intended to be used this way?"

[quote="rey8801, post:814, topic:36847"]
In case of spot welded battery you will end up with a disconnected weld and you need to disassemble the whole battery most of the time.
[/quote]

Amen!
```

---
## \#816 Posted by: rey8801 Posted at: 2019-02-08T16:26:42.429Z Reads: 182

```
I meant that if I remember correctly you use 2s modules mounted perpendicular to the length of the deck. In my mind if the deck is not super rigid then is better to use 1s module since they have smaller surface where the forces can apply pressure and moreover more external series connections capable of flex. While with a long 2s module you have a rigid structure in the middle and when it is compressed, all the stress goes to the side resulting in more chances of crack in those spots.
```

---
## \#817 Posted by: mishrasubhransu Posted at: 2019-02-08T16:33:12.199Z Reads: 186

```
Precisely. These were the first modules that I printed a long time ago. Now when I redo it, I'll use the one with a divider in between. Also I don't remember what infill density I used. In addition, the new chamfer that Agnius introduced takes away a lot of the stress that that thin walls experienced.
```

---
## \#818 Posted by: agniusm Posted at: 2019-02-08T18:49:18.866Z Reads: 189

```
What i mean is that these were not designed to be used as standalone modules. They were meant to be placed in an enclosure of some sort. I did not had skateboards in mind at that time. Ebikes, mopeds, motorcycles and LEV's was what i was aiming for.
```

---
## \#819 Posted by: agniusm Posted at: 2019-02-08T18:53:24.836Z Reads: 194

```
Btw, i can see underextrusion at the nut openings, overextrusion at the very top. 
Its not the first print i see from the xxxxxxsys and they dont look too good. I will need to print something white and share the quality i am getting
```

---
## \#820 Posted by: mishrasubhransu Posted at: 2019-02-08T19:13:03.802Z Reads: 193

```
The parts are actually pretty good from the printer. Unfortunately I don't remember what infill percentage I used back then, but layer height was .254mm . Also ABS is kinda brittle from my experience. 

Now I just print with clear PETG on an ender 3. Seems to be working great.
```

---
## \#821 Posted by: rey8801 Posted at: 2019-02-08T19:30:06.002Z Reads: 187

```
I print quite a lot and ABS is good if printed well but PETG has just more layer adhesion. At least that what I get. I sue ABS and I am totally fine with it, but the layer adhesion that I get with PETG is on another level.
```

---
## \#822 Posted by: deucesdown Posted at: 2019-02-08T20:03:53.399Z Reads: 191

```
I find PETG to be strong, but when it breaks, it breaks in strange unpredictable ways. I guess what I'm trying to say is, it's not as strong as I expect, and fails in places I don't think are the stress points.
```

---
## \#823 Posted by: mishrasubhransu Posted at: 2019-02-09T06:40:27.582Z Reads: 210

```
Any guesses what I am trying to show here?

![bottom|490x500](upload://hiLCKZCAgRX03iV2JryINucSxac.png) 
Bottom

![top|496x500](upload://1ReGlb0CcVcg6xLkkc6Af4pvOSi.png) 
top

![Capture|690x256](upload://lbhrxK3z0202lHXItFwRJ2OnZCc.png) 
corner
```

---
## \#824 Posted by: agniusm Posted at: 2019-02-10T08:25:27.198Z Reads: 205

```
Files have been updated. I have no time yet to upload to my website but you can access them here:
https://drive.google.com/drive/folders/1PGZ9yq_fR-jCwFaxxJ06rq8rRdNKgKuQ?usp=sharing
```

---
## \#825 Posted by: mishrasubhransu Posted at: 2019-02-11T04:07:17.035Z Reads: 211

```
since so many of you took so much interest, I must tell you more about it. Haha.

Well, i tried to make a compact 4 cell module all of them **swelled up in the middle**. so a load bearing lid was necessary to maintain the compression. The load bearing lid would add to the thickness and also you would have to trust the plastic to hold the compression along with screws. Going Agnius's way made the module a bit longer (83mm vs 77mm)

So final decision was to **free the lid** from having to help in compression. In absence of lid the module would bulge in the middle, but what if you make the **walls gradually curve inward as the height increases**. Basically you come up with the geometry that after bending looks like the things that you wanted in the first place. That's what you see in the previous image. An inward curving wall. It is a straight wall at the bottom but curved at the top. And it worked out great. The poron is uniformly compressed and the box is a rectangle and not a rectangle after a thanksgiving dinner. Also I increased wall thickness a bit to increase wall strength.

Final dimensions are **77x75x21**. Along the length of the cells it measures 75mm. 

The lid now uses a M2 screw to hold the cells in place and it does it's work very well.  The quality of my prints are not that good(PETG sticking to outside of nozzle) but there are some shots.

![Walls curve inside|666x500, 50%](upload://bZD6TQE9eQQCzUqn456rLFAYqID.jpeg) ![IMG_20190210_222614|666x500, 50%](upload://b0KzW6hNhb6Zf3xGdmf28KJvnkb.jpeg) 
![see, no bulge|666x500, 50%](upload://x65U9vXW5mFLoWtYa1cUcrQCrKC.jpeg)![IMG_20190210_223805|666x500, 50%](upload://eKodPYob4Vxl5YUf2h4O27tRNj8.jpeg)  
![IMG_20190210_224516|375x500, 80%](upload://iZux5kZCOpG0fclRtvrAINeZGL9.jpeg) ![looks clean|666x500, 50%](upload://5PjhxKKomDNS2OGKM2wbibSjDN4.jpeg)
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words/2992/9593?u=mishrasubhransu
```

---
## \#826 Posted by: agniusm Posted at: 2019-02-11T15:43:03.213Z Reads: 200

```
Good work. Good to have options.

**I have made very simple survey and if people who purchased parts or kits from me, could spend 1 minute of their time to fill it in i would appreciate it. I would appreciate unbiased, good or bad.**

https://www.surveymonkey.com/r/RJSMM3Y
```

---
## \#827 Posted by: Benjamin899 Posted at: 2019-02-12T12:08:47.247Z Reads: 195

```
that was the first ever survey that actually just took a minute^^
```

---
## \#828 Posted by: JonathanLau1983 Posted at: 2019-02-12T12:39:55.715Z Reads: 199

```
Anyone made a 5S2P pack using N.E.S.E modules yet? I'm looking to make a flight safe pack so will be splitting a 10S2P pack into 2 x 5S2P for cabin baggage.
Space is tight on the board so cells will need to be in two rows of 10 cells, so I was thinking 5S2P configuration of 4-2-4 in terms of N.E.S.E modules. 
Would this work? The bars would need to come out either side of the modules instead of out one end though so I would have to edit the 3D models I assume.
```

---
## \#829 Posted by: Benjamin899 Posted at: 2019-02-12T12:51:55.813Z Reads: 198

```
Sure you can. "Two rows of 10 cells" what is that supposed to mean?
```

---
## \#830 Posted by: JonathanLau1983 Posted at: 2019-02-12T12:57:17.180Z Reads: 197

```
[quote="Benjamin899, post:829, topic:36847"]
“Two rows of 10 cells” what is that supposed to mean?
[/quote]

![image|315x197](upload://j5StB72r4ggfQ4Y2RdKahAEYa7M.png)
```

---
## \#831 Posted by: Benjamin899 Posted at: 2019-02-12T13:09:10.219Z Reads: 195

```
why so complicated. just buy 10x2p modules.
```

---
## \#832 Posted by: JonathanLau1983 Posted at: 2019-02-12T13:33:07.626Z Reads: 195

```
5 x 2P modules will add a lot of length I believe as the embedded nuts add length to each module.
I don't have much space available under the deck.
```

---
## \#833 Posted by: Benjamin899 Posted at: 2019-02-12T13:44:02.899Z Reads: 196

```
I get the feeling you don't understand these modules.
```

---
## \#834 Posted by: JonathanLau1983 Posted at: 2019-02-12T13:49:43.645Z Reads: 202

```
Each module has a captive nut I believe which adds length.
![image|259x292](upload://rou2U20Erq6Ck2FPN9GIORgZjY4.png) 

Here's my board mocked up with the cells side by side, as you can see I don't have much length to use.

![image|690x340](upload://rvHeFaptlLzr5IuAcSBsOtsk1vr.png)
```

---
## \#835 Posted by: Benjamin899 Posted at: 2019-02-12T14:06:31.668Z Reads: 201

```
adding modules increases the length alongside the board. the part you marked changes nothing in the already existing dimensions. Also the 2P modules are even smaller compared to the 2s2p modules, also considering that only even numbers are possible with those.
```

---
## \#836 Posted by: JonathanLau1983 Posted at: 2019-02-12T14:09:01.375Z Reads: 201

```
The section I marked will be added 5 times if I used 5 x 2P modules. Which would take the battery outside the marked purple/blue area in my drawing.

![image|690x438](upload://9erCgQ5U5HUIxTeyMamZY8IIc1s.png)
```

---
## \#837 Posted by: agniusm Posted at: 2019-02-12T14:25:24.207Z Reads: 195

```
Only way out i see is using @mishrasubhransu design he posted recently, if it had exits on both sides. For the compactness, you would need to solder tabs outside or use some other method for series and balance.
```

---
## \#838 Posted by: Benjamin899 Posted at: 2019-02-12T14:31:23.327Z Reads: 191

```
the nuts show outwards, the way you showed is a total waste of space. Since this is a topmount you can just stack them.
```

---
## \#839 Posted by: JonathanLau1983 Posted at: 2019-02-12T14:32:47.983Z Reads: 189

```
It's bottom mount, so space is limited as I mentioned.
```

---
## \#840 Posted by: Benjamin899 Posted at: 2019-02-12T14:38:47.098Z Reads: 184

```
i meant the deck. You have enough space towards the ground. Or you can put them upride, nuts showing down or up, since this is 2p.
```

---
## \#841 Posted by: JonathanLau1983 Posted at: 2019-02-12T15:03:15.568Z Reads: 186

```
Ah, I gotcha. Unfortunately that won't work as I'll need to be able to get the cells out easily so I can take them in the cabin of a plane. Having them in any other orientation would make it a much lengthier process. Stacking them would also have the same effect.

I think I'm going to order some tab sets and make my own design to fit my purpose.
```

---
## \#842 Posted by: Benjamin899 Posted at: 2019-02-12T16:13:35.499Z Reads: 195

```
that wouldnt be a problem having stay upright. You can have two rows with one point of connection to make it 10s.![2P_Closed%20v1|690x419](upload://wWb8KxXusHA1zZeT4g4tqnNhrYX.jpeg)
```

---
## \#843 Posted by: agniusm Posted at: 2019-02-12T16:40:10.473Z Reads: 193

```
I dont think nese is the right solution for you. Taking out cells for travel is nonsense from my viewpoint. Having modules separated would be hassle but taking out cells is on another level.
Easier option would be to get slightly longer deck.
```

---
## \#844 Posted by: ZachTetra Posted at: 2019-02-12T16:45:55.728Z Reads: 194

```
If you use braided copper as all the contacts and are willing to sacrafice an extra 2cm on each side you can have sprung locks so they all pop out the side when you flip the tabs...it's be a paint to print and one end of each cell has to be on the edge of the board but its possible
```

---
## \#845 Posted by: mishrasubhransu Posted at: 2019-02-12T21:30:41.967Z Reads: 199

```
Actually, I beg to differ. NESE modules are perfect for removing and replacing cells. You can't do that with welded cells, super annoyit with vruzend, or the ones using standoffs. 

And also in comparison, removing the entire module is rather difficult when compared to removing the cells.
```

---
## \#846 Posted by: Hummie Posted at: 2019-02-13T00:57:57.481Z Reads: 206

```
What u think is going to happen? 
Never found epdm tension fatigue numbers to compare to poron but at least will be able to see how the bands are holding up periodically. ![image|666x500](upload://p0lqwXRNAVwg4CESNYiqtRLp3qs.jpeg) ![image|666x500](upload://b1xVYU9CeV6xR3fNuL7ukb0SZsc.jpeg) ![image|375x500](upload://wbv49fp4DCiPYiIZ66S4PSo2D7D.jpeg) 
Same weight as 12 awg but still a bit flexible. It’s all flexible.  21x74
```

---
## \#847 Posted by: Benjamin899 Posted at: 2019-02-13T01:02:24.881Z Reads: 199

```
Just i quesiton, when using copperbars, is there a chance of corrosion?
```

---
## \#848 Posted by: Hummie Posted at: 2019-02-13T01:04:12.038Z Reads: 200

```
Maybe for some environments but my stuff sits for years still looks the same.  You can plate it pretty easily. Or maybe even dip it and scratch off the coating on the tab.
```

---
## \#849 Posted by: Benjamin899 Posted at: 2019-02-13T01:06:32.444Z Reads: 191

```
ok, i read that on endless sphere, but i guess they have them outside in the humidity
```

---
## \#850 Posted by: gmurad Posted at: 2019-02-14T11:48:26.183Z Reads: 193

```
How is the CR10S PRO going? I bought one and it's just full of problems (mainly faulty bed leveling sensor, warped bed). I spent too many hours trying to get consistent prints out of it and I finally decided to return it and I got the Prusa MK3S Kit(New version just came out a couple of days ago). Will miss the large printing bed but the consistency is more important. Hope yours is printing good.
```

---
## \#851 Posted by: mikenyc Posted at: 2019-02-14T13:10:46.169Z Reads: 182

```
I haven’t gotten to test print anything yet. This weekend though. NESE seems like a simple enough first print.
```

---
## \#852 Posted by: rey8801 Posted at: 2019-02-14T13:49:01.184Z Reads: 185

```
It is easy but won't tell you too much. If you don't have 3d print experience start with test model for shrinking, cubes for preslcision and under or over extrusion. I would be surprise if the machine comes perfectly set it. Plus for each filament run a temperature tower to find the right temp for printing then start adjust your profile to reach the best results.
```

---
## \#853 Posted by: mishrasubhransu Posted at: 2019-02-14T15:05:51.717Z Reads: 185

```
Yeah, it's a learning experience. In the end you know more about 3d printer than just an end user. As a DIYer, I am glad I had those issues and learned to recognize the problems and fix them.
```

---
## \#854 Posted by: gmurad Posted at: 2019-02-14T16:00:10.133Z Reads: 193

```
This particular model (CR10S Pro) has some inherited issues that can't be tweaked short of buying new parts. e.g.: ABL sensor is inaccurate to 0.7mm, bed is warped. A small percentage of people (e.g.: Youtube reviewers) got non-faulty units but most are facing the same problems on user groups. Definitely learned a lot from it but the Prusa MK3S kit is a lot more geared towards DIYers.

Sorry for the off-topic. I will print these modules for my next build!
```

---
## \#855 Posted by: deucesdown Posted at: 2019-02-14T16:22:45.777Z Reads: 191

```
My first and only printer is a mk3 and I'll say I've spent an unbelievable amount of time troubleshooting things. So Prusa is most likely tons better but still has the feeling of being enslaved by the printer! :)

@mikenyc for initial calibration/troubleshoot, try to use good quality filament.
```

---
## \#856 Posted by: ryansinatra Posted at: 2019-02-16T13:42:09.817Z Reads: 190

```
Quick question. Is there any reason why printing this out of PLA is bad? The one I printed seems plenty sturdy. I'm sure PETG is a better option, just wondered
```

---
## \#857 Posted by: rey8801 Posted at: 2019-02-16T13:44:11.917Z Reads: 187

```
pla is brittle, so when it brakes it just fall apart.  PLus PLA doesn't held temperature as well as PETG and ABS
```

---
## \#858 Posted by: rey8801 Posted at: 2019-02-16T13:45:24.469Z Reads: 188

```
Man, we got batteries and we are gonna test your modules. Could you make a 3p version? maybe also 2s3p if the module with the wall separation is done for the 2s4p. Thanks a lot!
```

---
## \#859 Posted by: deucesdown Posted at: 2019-02-16T14:47:42.337Z Reads: 189

```
Also pla under tension will deform over time.
```

---
## \#860 Posted by: jneumann Posted at: 2019-02-17T00:28:50.195Z Reads: 187

```
hummie how do these modules go for fitting in your deck? would you recommend them of spot welded?
```

---
## \#861 Posted by: ryansinatra Posted at: 2019-02-17T02:52:07.344Z Reads: 181

```
So PETG is the ideal filament for these then?
```

---
## \#862 Posted by: deucesdown Posted at: 2019-02-17T03:29:57.128Z Reads: 188

```
I believe PETG is recommended. ABS is 2nd, but it's a real pain to print and can also be brittle.
```

---
## \#863 Posted by: ryansinatra Posted at: 2019-02-17T03:36:55.241Z Reads: 194

```
Yeah I've printed both and I'd prefer petg for the dimensional accuracy and ease of printing. Thanks yo
```

---
## \#864 Posted by: Hummie Posted at: 2019-02-17T16:56:06.637Z Reads: 202

```
@jneumann They fit well w one or two bands.  Bands are in compression not tension but tension as a back up now I guess. “Or” spotwelding?  ...I like these ![image|375x500](upload://uickYfTkT60jjpHwlNkvL7GaPNm.jpeg) ![image|375x500](upload://y1OSghFxkUNv0wvBUGEBUnNjPG8.jpeg) ![image|375x500](upload://sICjjtQCBJIXxDLiy8YK7AXhPhj.jpeg)
```

---
## \#865 Posted by: sainttjames Posted at: 2019-02-21T11:09:37.353Z Reads: 191

```
If you could please share the cad links of your updated 2s4p and latch files it would be much appreciated!
```

---
## \#866 Posted by: mishrasubhransu Posted at: 2019-02-21T14:02:10.331Z Reads: 193

```
I'll post all the NESE stuff to thingivere today.
```

---
## \#867 Posted by: sainttjames Posted at: 2019-02-21T14:30:59.632Z Reads: 193

```
Many thanks in advance!
```

---
## \#868 Posted by: ryansinatra Posted at: 2019-02-21T15:49:18.139Z Reads: 198

```
I'm making a 10s3p pack. I'll be printing the modules myself but I want to make sure I purchase the correct hardware the first time and have everything right in my mind. Does this diagram look correct?

![IMG_20190221_073845|374x500](upload://shx9YEA35Td7MWqszlV4jdl8hS7.jpeg)
```

---
## \#869 Posted by: mishrasubhransu Posted at: 2019-02-21T15:53:35.680Z Reads: 197

```
Yep, that's correct. Are you ordering the 3D printed parts from Agnius? Make sure they are the updated parts.
```

---
## \#870 Posted by: ryansinatra Posted at: 2019-02-21T16:05:21.800Z Reads: 192

```
I printed the correct modules from the files you linked me to. I would need (4x) 3p+3p modules and then (1x) module on the end with no center wall
```

---
## \#871 Posted by: mishrasubhransu Posted at: 2019-02-22T05:24:33.869Z Reads: 196

```
@sainttjames,  I have several of my 2S4P modules, what style were you thinking? Minimalist one is the one without the standard screw attachment point, where you have to do a bit of soldering. 

If you were going to use latch(stand) files, then that only works with Agnius's designs and the updated ones are [here](https://www.electric-skateboard.builders/t/n-e-s-e-nese-no-solder-module-battery-packs/36847/824?u=mishrasubhransu):
```

---
## \#872 Posted by: mishrasubhransu Posted at: 2019-02-22T05:59:12.589Z Reads: 197

```
@sainttjames, all NESE related files here: https://www.thingiverse.com/thing:3444525
![DieBieMS_nonstandard2|690x353](upload://ktPQYEbHjpjamZyldzoeAZMEJ1L.jpeg) ![DieBieMS_nonstandard|476x500,90%](upload://aEQVxv1Zu0DbSS5Nk7Naxp8f2Ce.jpeg)![IMG_20190119_064319|227x500](upload://ozvJwsY5rhzqtss0MjtdftA7rcy.jpeg)
```

---
## \#873 Posted by: sainttjames Posted at: 2019-02-22T09:56:22.159Z Reads: 184

```
Hey Thanks! Is there a chance you could publish your 2S4P (Lid +Base) as well ?

I built a board in 2017 nearly identical to WhitePony and would like to be able to take the board on vacation. Hence, the NESE modules are very intriguing and what you did regarding the curved wall and freeing the lid, etc. Thanks again~
```

---
## \#874 Posted by: visnu777 Posted at: 2019-02-22T10:02:39.613Z Reads: 185

```
I just had the idea of merging both worlds: Spotwelding the P-Groups but putting them in N.E.S.E. like modules for easy disassembly... :thinking:
```

---
## \#875 Posted by: mishrasubhransu Posted at: 2019-02-22T10:04:07.261Z Reads: 187

```
@sainttjames 
I have a 2S4P but I haven't printed and tested it. I have only tested the 4P module with curved wall design. 

4P can very easily be converted to 4P+4P and will be bit smaller than two 4P side by side. It will work 100%

2S4P on the other hand, you will need to print and test it. I can upload to thingiverse now. So which one do you need?
```

---
## \#876 Posted by: mishrasubhransu Posted at: 2019-02-22T10:07:00.365Z Reads: 189

```
or you solder them directly when assembled something like this
![image|690x380](upload://47lu0r5eSVGFGc2RpYMR73NvWuf.jpeg)
```

---
## \#877 Posted by: sainttjames Posted at: 2019-02-22T10:07:51.191Z Reads: 188

```
Hmmm ...I'm not certain. I just finished printing Agnius's 2s4p - I liked how you mounted them on your board. Are you still rolling with that setup?
```

---
## \#878 Posted by: sainttjames Posted at: 2019-02-22T10:11:21.813Z Reads: 190

```
BTW - I have been using Simplify3D for slicing PETG (gives me slightly better results than Cura) BUT it gave me some weird artifacts as a result of its Gcode. I fixed one of Agniu's bases with Rhino3D, but I'm wondering if anybody else has seen this problem? Doesn't happen in Cura.![2s4p%20strange|690x437](upload://4MetC17pUmEkPaPuezUxC0UAMku.jpeg)
```

---
## \#879 Posted by: visnu777 Posted at: 2019-02-22T10:12:33.587Z Reads: 178

```
hmm, yeah, but with NESE style like nut and screws for easy assembly and protection outside of the enclosure.
```

---
## \#880 Posted by: sainttjames Posted at: 2019-02-22T10:13:56.496Z Reads: 177

```
For me, I like the fact that the individual cells are not welded. If a cell dies you can just pull and replace.
```

---
## \#881 Posted by: mishrasubhransu Posted at: 2019-02-22T10:16:05.456Z Reads: 183

```
Yeah, and that setup works great. I have been riding it daily and have ridden more than 250 km total.

The mounts that I used for mounting on my board are available on the thingiverse link and they are compatible with Agnius's 2S4P design.

EDIT: Hmm, weird. I have printed his files without any issues using Cura on my Ender 3. @agniusm, would you know why his slicer giving him weird artifacts?
```

---
## \#882 Posted by: mishrasubhransu Posted at: 2019-02-22T10:19:30.633Z Reads: 180

```
[quote="visnu777, post:874, topic:36847"]
P-Groups but putting them in N.E.S.E. like modules for easy disassembly… :thinking:
[/quote]

Aah, Okay. You want to do opposite of what I was thinking. I wanted to have removable cells but a welded pack but you want welded cells but removable pack. 

That could be interesting. Give it shot.
```

---
## \#883 Posted by: visnu777 Posted at: 2019-02-22T10:19:31.471Z Reads: 176

```
For me that is also the most important thing apart from modularization, I actually know every cell by name ;) but there might be some that only need the modularity
```

---
## \#884 Posted by: sainttjames Posted at: 2019-02-22T10:25:16.604Z Reads: 179

```
250km! That's great!!! Exactly what I want to hear. :sunglasses:


<CURA>....I didn't get the artifacting in Cura...only Simplify3d.

MeshMixer reported problems with the STL file as well...and it didn't play nice while I tried to repair it. I ended up bringing it into Rhino3D and rebuilding Mesh normals ( i think...can't remember now). After export that weird artifact I posted above went away.

Regardless, MeshMixer reports problems with the original STL.
```

---
## \#885 Posted by: sainttjames Posted at: 2019-02-22T10:28:16.736Z Reads: 171

```
I built a 10S4P just like Whitepony...vacuum formed individual battery trays, etc. I just want to be able to take the damn board with me on summer vacation! :stuck_out_tongue_winking_eye:

With my current setup I can't take anything apart. Board rides like a dream otherwise~
```

---
## \#886 Posted by: agniusm Posted at: 2019-02-22T11:23:28.695Z Reads: 175

```
@mishrasubhransu and @sainttjames,
The files are generated from inventor then brought into s3d, oriented how they should be printed and saved as binary stl. I had no issues with s3d or slic3r. I remember someone from french customers had similar issue on repetier.
```

---
## \#887 Posted by: jneumann Posted at: 2019-02-22T12:19:03.861Z Reads: 180

```
@Hummie are you using a different style of inserts? I notice yours are copper but the near strips seem to be coated copper
```

---
## \#888 Posted by: sainttjames Posted at: 2019-02-22T14:06:42.517Z Reads: 193

```
Hey Agnius, not trying to throw any shade on ya....I'm a big fan of your design!

An analysis in Meshmixer looks like this. It's probably why my first print had some artifacts in S3D.
![Meshmixer%20analysis%202S4P(4P%204P)|644x500](upload://a72HTcIqHWGmqICta0jQKllSNY6.png)

A magenta sphere points out disconnected components with small area relative to the entire mesh.
```

---
## \#889 Posted by: agniusm Posted at: 2019-02-22T14:43:26.543Z Reads: 183

```
Some could be disconnected. There are now 8 half parts that build up module, e.g. base front, base middle and base rear. These are halfs. They are mirrored to form complete section, then those sections are assembled into modulea, say 1 front one rear and 3 middle. The constraint is at one edge. That could pose a problem when the is no uniform solid and errors might appear in translation. I would not be able to easy update or revise modules as it would take ages. Now i just update a section and assemblies get updated automatically. I am printing them 24/7 and if there is meshes that show errors in meshmixer, i dont care as they do not inprint. I will check the ones you are trying just to be certain.
```

---
## \#890 Posted by: StefanMe Posted at: 2019-02-22T14:44:34.362Z Reads: 178

```
Why is ABS just the second choice?! ABS is better in all categories. Just harder to print for some people.
```

---
## \#891 Posted by: agniusm Posted at: 2019-02-22T14:46:37.550Z Reads: 178

```
It is harder to print for larger procentage of people plus ita toxic when printing. For me it is easier with lower error margin so i can keep the prices as low as i can.
```

---
## \#892 Posted by: ryansinatra Posted at: 2019-02-22T15:03:55.164Z Reads: 180

```
Hey @agniusm - I have the printed parts and the hardware, I just need the tabs only for 10s3p 

The tabs on the site look like they are 8 units long. How do I get the tab that goes in my base module that is 6 batteries wide that has a tab on each end?
```

---
## \#893 Posted by: agniusm Posted at: 2019-02-22T15:30:20.344Z Reads: 189

```
You dont. You cut it at 6P and the tab exits on one end but that is sufficient to hook up balance wire.
```

---
## \#894 Posted by: Hummie Posted at: 2019-02-22T15:56:55.390Z Reads: 204

```
![image|666x500](upload://kmCjizY5misMDegevKdeWu7WTQp.jpeg) ![image|666x500](upload://b1xVYU9CeV6xR3fNuL7ukb0SZsc.jpeg) ![image|375x500](upload://ljehecOSBYnbFZxFBNvoX47DCDt.jpeg) ![image|375x500](upload://iWG8hNOW2pGfnHDmR2quVC6F4cl.jpeg) ![image|375x500](upload://uickYfTkT60jjpHwlNkvL7GaPNm.jpeg) [Uploading: A3947D1B-BFF1-4D59-B88A-25E6B8342B68.jpeg...]() [quote="jneumann, post:887, topic:36847, full:true"]
@Hummie are you using a different style of inserts? I notice yours are copper but the near strips seem to be coated copper
[/quote]
They’re bare copper. A different design. I press the strip with an abs press and epdm bands for compressing to contacts.
```

---
## \#895 Posted by: ryansinatra Posted at: 2019-02-22T18:52:10.310Z Reads: 193

```
Perfect! Figured as much.im glad you understood my question. Much appreciated.
```

---
## \#896 Posted by: deucesdown Posted at: 2019-02-22T19:03:30.746Z Reads: 198

```
[quote="StefanMe, post:890, topic:36847"]
Why is ABS just the second choice?!
[/quote]

I was basically trying to summarize 18650.lt for the people reading the thread.

But IMO after attempting to print these in ABS (prusa mk3, 2 spools and a foam enclosure):

- ABS has shrinkage, which means you have to print at 101% or 102% with trial and error.
- ABS shrinkage makes it very challenging to print these NESE modules, lots of trial and error at least for me. Many failed prints, and even the good prints are deformed in the corners at least a bit. Lid fit is hit-and-miss.
- 3d printed ABS seems quite brittle. I understand this can be tuned with temperatures, but again lots of trial and error and competing with other desirable properties.
- have to print hot in a hot space, and it smells when printing (reading a lot, I'm not very concerned about internet chatter on health risks, at my volume of printing)

but,
- ABS is cheap
- ABS is fast to print once dialed
- ABS is somewhat UV resistant
- ABS can be strong and nonbrittle if you get things dialed in

now for PETG:
- PETG is dimensionally more stable
- PETGis less brittle

but,
- PETG is more expensive
- at least for me, I have to print PETG slower


Given all the time and materials spent with trial and error, PETG is actually for me a lot faster and a lot cheaper as well.

Disclaimer: I am not an expert (but boy I sure spent a lot of time with ABS), and I am using hobbyking colorchange ABS, of which I have many spools due to some crazy sale they had.
```

---
## \#897 Posted by: s5300 Posted at: 2019-02-22T19:19:32.918Z Reads: 181

```
@Hummie , my bad if it's been mentioned earlier - but are you open sourcing any of this? Cause it looks dope
```

---
## \#898 Posted by: StefanMe Posted at: 2019-02-22T20:04:22.762Z Reads: 190

```
Sorry man... but then u just can’t print ABS.

ABS hast a Extrusion multiplier by 1.0. 
PET-G 0.85-0.95.
PLA 0.9. 

That are basics in 3D Printing. Of course it needs a lot more to print ABS. If u print ABS in a chamber it is defiantly more stable and a lot more temperature resistant then PETG.

PETG is great because it’s that easy to print. Specially if u don’t have a chamber or full metal hotend ect... print at least with Ooz shield...

Let’s say PETG is definitely easier to print. But ABS is the first Choice of u could handle it. I have a lot experience in printing ABS. 

Sorry! I don’t wanna blame u or any other guy here... but I also don’t want that someone is saying PETG is the best. In mechanical and specialy mechanical resistance under temperature influence... the winner is definitely ABS. :slight_smile: BUT OF COURSE... PETG is just fine for these purposes!


EDIT: 

Maybe I just hate PETG 😂 I hate this stringing... HATE!
```

---
## \#899 Posted by: Hummie Posted at: 2019-02-22T20:12:00.877Z Reads: 186

```
I will as soon as I run it later today!  you'll need to get the right copper sheeting (forget the size now but equates to 12awg weight) and also you'll need to print the press for it too.  you can see it in the pics above.   @agniusm 's stuff has been inspirational for me and I like to think it's like his....but better!   no hard feelings but I feel the use of bands is maybe better and the tension of epdm bands will last better long term then thin strips of Poron compression foam but I can't find evidence and just going off assumptions and hope.   could always add two bands or more or check them periodically.   I do like how the bands perform some protection and no foam is needed.   I also think since this method doesn't rely on the compression set and tension fatigue of 3d printed plastic its safer.   bands are meant to be stretched and keep that tension for long periods of time.  it's their specialty.
```

---
## \#900 Posted by: deucesdown Posted at: 2019-02-22T20:12:20.318Z Reads: 193

```
[quote="StefanMe, post:898, topic:36847"]
Sorry man… but then u just can’t print ABS.
[/quote]

[quote="StefanMe, post:898, topic:36847"]
Maybe I just hate PETG :joy: I hate this stringing… HATE!
[/quote]

Haha maybe you just can't print PETG ;)

No worries my feelings are not hurt. But I did try enclosure and all. I'd argue if that much dicking around still doesn't produce results, it ain't worth it. But I have this huge pile of cheap ABS lol.

And definitely all this information helps me.
```

---
## \#901 Posted by: mishrasubhransu Posted at: 2019-02-22T20:26:57.687Z Reads: 184

```
PETG prints best with direct drive. Making sure the first layer is not too squished. Using a silicone sock. Maybe @agniusm can tell us his tricks in printing it perfectly.
```

---
## \#902 Posted by: agniusm Posted at: 2019-02-22T20:30:50.065Z Reads: 197

```
I have minor stringing. I blow it with heat gun if any. I print strait on pei 60mm/s. Nothing fancy.
@Hummie, nice you have thing moving. Can i ask to make separate thread for your design as this one gets hijacked and might be confusing for new people visitig? Dont meen to be rude or anything but its not NESE or not NESE mod like @mishrasubhransu modding anymore. Appreciate your understanding.
```

---
## \#903 Posted by: StefanMe Posted at: 2019-02-22T20:53:22.587Z Reads: 204

```
I know how to print PETG. I just hate the stringing. ABS is just so clean. It’s more a personal preference :slight_smile:

Of course i use a condom. On my nozzle. In the Printer. 

![image|375x500](upload://torK4O7jiNGyDCjY3tb9WWekHd5.jpeg)
```

---
## \#904 Posted by: agniusm Posted at: 2019-02-24T14:55:07.985Z Reads: 194

```
If its stringing, the teps are too high. Lower by 5C then back up a tad
```

---
## \#905 Posted by: Winfly Posted at: 2019-02-25T01:40:04.567Z Reads: 194

```
Petg is very sticky so it tends to string a lot. I would lower temp by 5 at a time and teak your retraction setting. Also printing 40mm/s is the fastest I would go.
```

---
## \#906 Posted by: JonathanLau1983 Posted at: 2019-02-27T11:08:49.427Z Reads: 185

```
Are you guys using fish paper rings with the N.E.S.E tabs? Would it increase the gap too much to make contact with the positive terminal?
```

---
## \#907 Posted by: visnu777 Posted at: 2019-02-27T11:19:12.155Z Reads: 190

```
it should work (the tabs from Agnius are with pins for the contact that are higher than fish paper) but its not necessary due to the construction of the modules. He even showed them working with removed cell wrapping. (I wouldnt do that though :))
```

---
## \#908 Posted by: StefanMe Posted at: 2019-02-27T12:26:26.099Z Reads: 192

```
That sounds scary. It should work, but still scary 😂😬 if u need more thrill 😏
```

---
## \#909 Posted by: mishrasubhransu Posted at: 2019-02-27T12:29:17.063Z Reads: 189

```
I have put about 300km on the original NESE and also without any fishpaper between the cells or around the positive terminal. I'll soon print the updated box that's has a divider in between for safety of mind. But @JonathanLau1983, the fish paper rings is absolutely not a necessity because of the raised tabs.
```

---
## \#910 Posted by: JonathanLau1983 Posted at: 2019-02-27T15:35:22.944Z Reads: 184

```
Thanks, I was thinking that, however as I will be removing the cells for flights it does mean the cells will be moved in an out more than a normal build. My only concern would be wear on the heat shrink due to this.
I am designing my battery case with this in mind so the positive ends have to be inserted first, and negative end slid down.
```

---
## \#911 Posted by: mishrasubhransu Posted at: 2019-02-27T15:43:13.614Z Reads: 189

```
I have probably removed and installed it 10 times or so. I am wary of that potential problem, so I make sure to push it in vertically and while taking out I make the modules be upside down and gently-slam(hope you understand) the board on the ground. All the cells pop out in a couple of tries and land softly on a towel. 

@agniusm, what's your recommendation for frequent installation and removal of cells? I am guessing your modules are not typically designed for that.
```

---
## \#912 Posted by: agniusm Posted at: 2019-02-27T17:59:33.595Z Reads: 185

```
Its not meant for that. Occasional bad cell replacement is whats it for. You can take 100wh on the plane so better have module release system and have separate <100wh modules.

Just a teaser, summer(mid to late) might bring 21700 (20700 compatible) modules and hardware.
```

---
## \#913 Posted by: DAddYE Posted at: 2019-02-27T18:54:34.243Z Reads: 180

```
21700 please!
```

---
## \#914 Posted by: mishrasubhransu Posted at: 2019-02-27T19:02:12.233Z Reads: 180

```
Nice! If moulds haven't already been made, please do consider  to have a little more gap between the cells so that it's not skin to skin and a wider gap between the 2S groups built into the tabs.  :slight_smile:
```

---
## \#915 Posted by: agniusm Posted at: 2019-02-27T19:20:43.120Z Reads: 191

```
It will be skin to skin as it does not matter in P groups. I have sold too many to fault them there. Having said that, for people who are concerned (like you :) ) 20700 cell will give you that 0.65mm gap peace of mind ;)
For the S modules it will work the same way as with 18650. I think its enough of a gap for isolating groups from shorts.
The key here is to have modules as compact as they can be while retaining the ease of builability with single phillips scredriwer
```

---
## \#916 Posted by: visnu777 Posted at: 2019-02-27T19:24:56.647Z Reads: 196

```
I think he meant specifically the tabs. The divider width makes the tab a bit off on one side, eg for a 2s3P like mine the 6p compression tab you just send me should be a 2 groups of three with a little wider gap in between. its working though, but if its possible to change them its better.![15512956122327544047669622957053|374x499](upload://v3Oeg4mNnMm7aofG3ePFG4FtOMA.jpeg)
```

---
## \#917 Posted by: agniusm Posted at: 2019-02-27T20:15:25.268Z Reads: 185

```
If i make it, i need to make it for all the P groups, that means a bigger gap on 3 cells, after 2P, 3P and 4P. If its 0.9mm that is 2.7mm longer modules. The nipples are smaller that positive end of the cell so there is no electrical or mechanical issue there, just visual if you are not keen on the offset cells.
I think going 20700 is a good compromise if you are concerned.
```

---
## \#918 Posted by: ryansinatra Posted at: 2019-03-01T02:35:31.603Z Reads: 188

```
Quick question on these. When assembling the pack, which order is appropriate to connect everything? Balance leads plugged in to BMS first or battery negative attached first?
```

---
## \#919 Posted by: agniusm Posted at: 2019-03-01T10:19:42.637Z Reads: 199

```
Depends on BMS or PCM. The ones i use was balance connector first. I ,dont think it matters though. Balance connector always has B- as first pin. So balance connector B- (sometimes B1) has continuity with BMS/PCM battery negative power pole.

Here is a comparison between 18650 8P and 21700 8P modules
This summer might bring new modules. 21700 and 20700 has no no solder solution so i am investing in tooling to get this covered. Here are some teaser photos on size comparison between 21700 and 18650:

[img]https://i.imgur.com/A3UO2GH.jpg[/img]

[img]https://i.imgur.com/TAKKly2.jpg[/img]

[img]https://i.imgur.com/oP4oawp.jpg[/img]
```

---
## \#920 Posted by: neiru37 Posted at: 2019-03-04T09:03:05.140Z Reads: 200

```
[quote="StefanMe, post:903, topic:36847"]
I know how to print PETG. I just hate the stringing
[/quote]

![20190303_211631|666x500](upload://xysKxn9UD36INqaWyaSc7QKohZJ.jpeg)

These are both petg but the left one is a result of a few tweaks here and there.
```

---
## \#921 Posted by: StefanMe Posted at: 2019-03-04T09:13:20.258Z Reads: 202

```
hmm yes... the left one is definelty better... but not good. Maybe i just have to high requirements to PET-G. Tried A bit PET on the weekend. Its ok, but for ME the material is not that good printable. The results in ABS are just better. At least for me. 

But if i find some time, i ll give it another try.

My ABS are just perfect at the moment. So its not nesserary to change.

![image|281x500](upload://xPF3rmIQbeI0XLCHx5D2xzKoq9L.jpeg) ![image|375x500](upload://2R8n9H9PzQb4GHX9k0UyIUJdjkK.jpeg)
```

---
## \#922 Posted by: Benjamin899 Posted at: 2019-03-04T13:49:07.483Z Reads: 197

```
looks like a watermelon. love it
```

---
## \#923 Posted by: mishrasubhransu Posted at: 2019-03-04T14:07:50.316Z Reads: 203

```
Use no pigment PETG. Additives make it worse in my experience. Also use a silicone sock and a thin layer of silicone sealant on the exposed nozzle. Bam! No sticking or dragging. Final thing is that the nozzle shouldn't be as close to the build plate as you have with PLA. This results in the molten filament curling up and causing problem when the next layer is being laid.   
This how my prints look. 
![IMG_20190125_110629|666x500](upload://royG3NZnoiXWbJXf448g7gIfnNJ.jpeg)
I have a beautiful  benchy too, that I printed after silicone sock and silicone sealant mod. I'll post it here when I go home.



And look at this abomination printed with black PETG. No matter what I did, I couldn't print well with it.
![image|666x500](upload://mDtmYI2DGDgJhVMCsyXPrsXvo2X.jpeg)
```

---
## \#924 Posted by: deucesdown Posted at: 2019-03-04T15:08:06.112Z Reads: 192

```
I'm' very impressed by the overhang with PETG
```

---
## \#925 Posted by: mishrasubhransu Posted at: 2019-03-04T15:22:36.682Z Reads: 194

```
And this is without any cooling. The layer adhesion is incredible if you print without part cooling.
```

---
## \#926 Posted by: LOSI Posted at: 2019-03-04T15:48:12.525Z Reads: 189

```
I need a holder for my liftboard. ASAP. 

Joey 
Strongislandguy@yahoo.com
```

---
## \#927 Posted by: neiru37 Posted at: 2019-03-04T16:32:39.680Z Reads: 198

```
[quote="StefanMe, post:921, topic:36847"]
My ABS are just perfect at the moment. So its not necessary to change.
[/quote]

I mean, I'll take perfect too if I was in your position. Don't fix what's not broken. I just wanted to show you that it can be done, so don't discount PETG just yet.

[quote="mishrasubhransu, post:923, topic:36847"]
Use no pigment PETG.
[/quote]

Got any recommendations? I have esun petg black at the moment.

[quote="mishrasubhransu, post:923, topic:36847"]
Also use a silicone sock
[/quote]

Thankfully the newest ender 3's have this.

[quote="mishrasubhransu, post:923, topic:36847"]
a thin layer of silicone sealant
[/quote]

Would give this a shot
```

---
## \#928 Posted by: StefanMe Posted at: 2019-03-04T16:35:39.263Z Reads: 193

```
I am using some high quality PETG form some German guys... should be one of the best u can get on the marked. Still not satisfied with hit. But maybe I just did not found the correct settings for this. :rofl:

https://www.material4print.de/de/petg-filamente__106/?fltr4[]=5&
```

---
## \#929 Posted by: mishrasubhransu Posted at: 2019-03-04T17:18:06.766Z Reads: 197

```
I am on my 3rd roll. It prints great. 
https://www.amazon.com/gp/product/B075M68Y19
```

---
## \#930 Posted by: StefanMe Posted at: 2019-03-04T17:29:59.935Z Reads: 198

```
Sunulu is great. I really like the PLA colours they have. The Pearl white is amazing!
```

---
## \#931 Posted by: neiru37 Posted at: 2019-03-04T17:46:47.911Z Reads: 198

```
[quote="mishrasubhransu, post:929, topic:36847"]
I am on my 3rd roll. It prints great.
[/quote]

Surprisingly, they don't ship to my address in the US.
```

---
## \#932 Posted by: mishrasubhransu Posted at: 2019-03-07T06:48:28.945Z Reads: 203

```
As promised my PETG benchy

![IMG_20190307_012553|422x500, 50%](upload://1b8lzI54UYjqWAPK9asFLRtlUWA.jpeg)![IMG_20190307_012426|666x500, 50%](upload://2bqKtKkHIoVBHzVhu4FTDKw1YIG.jpeg) ![IMG_20190307_012539|578x500,50%](upload://3hhBootjNnSFDz1OmIZwJb8eElZ.jpeg)![IMG_20190307_012544|578x500, 50%](upload://gTl34SQU9EvlQConzSFrGi3OBvf.jpeg)
```

---
## \#933 Posted by: rey8801 Posted at: 2019-03-07T07:04:23.434Z Reads: 199

```
I also use SUNLU PETG, 3rd rools, great filament. The benchy is good. With fan or without?
```

---
## \#934 Posted by: StefanMe Posted at: 2019-03-07T09:01:47.029Z Reads: 195

```
PET-G without fan? Sounds not that good...

Maybe i have that much of a problem, because my extruder is running on and old tmc2130 driver in spreadcycle... 

What temps are u printing the SUNULU PETG? The PETG i use form M4P need a quiete hot temperature. ~240 degrees
```

---
## \#935 Posted by: rey8801 Posted at: 2019-03-07T09:05:47.217Z Reads: 193

```
Petg can be printed with, without or middle fan. The higher fan is for details but the lower is for mechanical purpose. All the Pulley I printed in petg was 0% fan. I don't have problem in print it like that. You just need a bit more cleaning afterwards, since it will string more.

Sunlu petg prints well without clear difference from 230 to 240 in my case. I use 230 for details, 235 for layer adhesion with no fan. Petg requires really low retraction, in cura you can not set it so you need S3D to better tune your printer.
```

---
## \#936 Posted by: neiru37 Posted at: 2019-03-07T09:11:11.979Z Reads: 194

```
[quote="rey8801, post:935, topic:36847"]
in cura you can not set it
[/quote]

Err you can

![image|486x237](upload://hoUtJtSQG3cwoNUnA4oqkl9TDnw.png)
```

---
## \#937 Posted by: rey8801 Posted at: 2019-03-07T09:12:14.116Z Reads: 184

```
Ah ok I stopped to use cura 3 years ago. My bad. Then keep it low for petg. I advice 2-3mm max
```

---
## \#938 Posted by: StefanMe Posted at: 2019-03-07T09:32:04.956Z Reads: 190

```
Same for me... i just use S3D. But they are way behind the others at the moment. Its the more technical/profssional programm, but with less features. 

Ah i always have 100mm/s retraction speed. Maybe thats the problem ;) As i said...i am not a big fan of PETG. BUT i ll give it another try... got some really nice rolls of PETG at home.
```

---
## \#939 Posted by: visnu777 Posted at: 2019-03-07T09:41:27.751Z Reads: 191

```
Once you get used to it you don't want to use the stinky ABS anymore :D 
I just found out that printing heat towers with new filament is generally a good idea since it tells you the optimal temp for the specific stuff on your printer. Then you have to increase the distance to the bed compared to PLA, at least two layers of paper instead of one when leveling :) Last but already said: Retraction is important. I recently got a Micro Swiss all metal hotend for my Ender3 and had to learn printing again :D (My values: 3-4mm @ 60mm/s).
```

---
## \#940 Posted by: rey8801 Posted at: 2019-03-07T09:46:28.455Z Reads: 194

```
Also take into account that petg absorbs moisture so put in the oven 2-3 hours at 50-60 degree for better result. Which printer do you have? If it is creality cr10, cr10s and pro I could give you my profile to try it out
```

---
## \#941 Posted by: StefanMe Posted at: 2019-03-07T09:50:28.107Z Reads: 197

```
It’s a selfmade coreXY Printer... Running on KLIPPER.

Its more a precise high speed printer... Klipper and CoreXY kinematic. Runs easy over 300mm/s travel with silent tmc and acc 10.000mm/s²

![image|375x500](upload://ld8qpElkWW4ws9T7jqe3Kom1C93.jpeg)
```

---
## \#942 Posted by: rey8801 Posted at: 2019-03-07T10:07:30.543Z Reads: 201

```
Then no :grin: nice printer. Then PETG is just a matter of settings. You also have to print it slow. To get really good result I stay at 35mm/sec

This one is my benchy out of the bed. You can still see all the stringings that can be easy removed btw

![IMG_20190307_110608|690x388](upload://tvzdOUMpC2Evb1TD7dwk7HpWjda.jpeg)
I don't have here the newer one but now the layer separation is even better.
```

---
## \#943 Posted by: StefanMe Posted at: 2019-03-07T10:18:28.876Z Reads: 197

```
thx man ;)

Ok then i prefer to print ABS with 120mm/s.... :stuck_out_tongue:  But definitly i ll try the PETG again.
```

---
## \#944 Posted by: rey8801 Posted at: 2019-03-07T10:23:27.814Z Reads: 198

```
Ah yeh if you print PETG so fast that will be really tricky.
```

---
## \#945 Posted by: mishrasubhransu Posted at: 2019-03-07T12:34:15.993Z Reads: 204

```
I don't use part cooling fan. I have done strength testing and without part cooling I have the best layer adhesion.  
My retraction is 3mm at 70mm/sec retraction and 40mm/sec prime(putting it back)

Use silicone sock + high temp silicone on rest of the exposed nozzle if possible.

Double the nozzle to bed distance than what you use for pla

Print speed is 40mm/sec. 

Nozzle temp at 245C

I use the clone BGM extruder though($30). The best upgrade I made. 

I also have a drybox with dessicant packets
![IMG_20181220_193331|666x500](upload://jq1PtnTxGEx2FUCwLaJAsn9RXTt.jpeg)
```

---
## \#946 Posted by: rey8801 Posted at: 2019-03-07T12:37:25.714Z Reads: 197

```
got both tabs and battery I will try out your module
```

---
## \#948 Posted by: CarbonV Posted at: 2019-03-07T18:39:58.970Z Reads: 198

```
Does someone have a link to the most recent "Agnus" NESE modules please? Because I heard they are no longer up-to-date on the site. Thanks in advance.
```

---
## \#949 Posted by: mishrasubhransu Posted at: 2019-03-07T18:51:39.031Z Reads: 197

```
Search up on the thread. There is a Google drive Link that agnius posted.
```

---
## \#950 Posted by: CarbonV Posted at: 2019-03-07T21:05:01.859Z Reads: 196

```
That one didn't work for me.
```

---
## \#951 Posted by: ryansinatra Posted at: 2019-03-07T21:16:23.944Z Reads: 200

```
https://drive.google.com/drive/folders/1PGZ9yq_fR-jCwFaxxJ06rq8rRdNKgKuQ?usp=sharing
```

---
## \#952 Posted by: CarbonV Posted at: 2019-03-07T21:27:42.058Z Reads: 202

```
Thank you!
```

---
## \#953 Posted by: StefanMe Posted at: 2019-03-09T14:18:44.298Z Reads: 205

```
Printed now in PETG with success. It was just my extruder running with only 600mA... Thats a b it low for sticky material. Went up to 900 and now its just finde. Also reduced the speed to crappy 50mm/s. Slow but it works.

The martial is really "strong" in case of impacts. Nice. I go for a small riser with lights, charge plug and ON ONFF button. Thx for the idea...

![Riser_Pad_front_2019-Mar-09_02-14-57PM-000_CustomizedView21152626265|690x425](upload://2bqmkO3xbKKmJd2mUf9uvINZok5.jpeg)
```

---
## \#954 Posted by: ryansinatra Posted at: 2019-03-14T06:02:34.714Z Reads: 200

```
![IMG_20190314_020030|666x500](upload://k5JkWywGgBf78Ns6VPrX8SsT56A.jpeg) 

10s3p NESE

Thank you for allowing a noob to still build a great and safe battery 👍
```

---
## \#955 Posted by: twan Posted at: 2019-03-14T18:24:17.237Z Reads: 189

```
wow thats cool! please show the finished product once you make it.
```

---
## \#956 Posted by: mishrasubhransu Posted at: 2019-03-16T16:58:09.077Z Reads: 192

```
Can a mod or @NAF, make this a solution. So that people have the latest files when they scroll from the top.
```

---
## \#957 Posted by: agniusm Posted at: 2019-03-16T17:33:13.046Z Reads: 191

```
I will add a link. I will have archive on the website instead of flashy 3d preview. Maintenance is too demanding when you have so many options. I have just remaking stl files. Found batch tool to rotate and orient models in batches which saves me so 3 hours of manual borring work. 
@ryansinatra looking great so far.
```

---
## \#958 Posted by: visnu777 Posted at: 2019-03-19T11:37:48.888Z Reads: 188

```
@agniusm you are a master at printing these. Thanks for the fast delivery.
```

---
## \#959 Posted by: agniusm Posted at: 2019-03-19T11:56:31.423Z Reads: 188

```
@visnu777 thank you very much for kind words. I do try improve quality constantly. The latest printers yours are printed on are printing better than prusa but i took me since july to get here and i have final upgrades in my mind for even better accuracy.
Hopefully you will pinpoint the issue you have.
```

---
## \#960 Posted by: mishrasubhransu Posted at: 2019-03-19T19:12:11.320Z Reads: 183

```
Now you just teasing us. Show us the pics.
```

---
## \#961 Posted by: visnu777 Posted at: 2019-03-19T19:23:01.968Z Reads: 193

```
I said this because I recently printed the same 2s3p cases I just got which was a pita. I produced a lot of scrap PETG (I will hopefully have access to a filament recyler so its not that bad) in the process. I learned a lot about my Ender 3 though, it is now not comparable to the stock version anymore :D. I printed PETG totally wrong (bed leveled for PLA is way too close for it), now its perfectly calibrated and everything. I was really happy with my results but today when I held the ones @agniusm printed it was like night and day. I needed to clean up my prints, his look and feel just perfect. Anybody who complains about the price needs to try print them by her/himself, actually when you calculate material and time (which is quite expensive in my case, but its a hobby right? :D) its way too cheap imho.

![SAM_2433|690x460](upload://kl09UYoQFySKUVAfMi8IyJe7LS2.jpeg) ![SAM_2431|333x500](upload://eRDXlXDbYW5KFNcRf0OmQnPXI0k.jpeg)

mine are more shiny because it was printed on the backside of the tempered glass cf plate from creality :)
The first green lid in the first pic was printed on the CF side. Which build surface do you use @agniusm? it almost feels like glass but slightly less polished
```

---
## \#962 Posted by: agniusm Posted at: 2019-03-19T19:51:54.172Z Reads: 184

```
I always use PEI but not the chinese ones. Mine are matt finish from prusa or prima 3d. I am not a fan of glossy finish, i would only use it for tail lights :) And it could make scratches more pronounced. I also chose clear for my main color as it is harder to see imperfection that are present using this method of manufacturing. Sneaky :smile:
```

---
## \#963 Posted by: visnu777 Posted at: 2019-03-21T11:53:46.637Z Reads: 191

```
![15531691965371279943708427545950|375x500](upload://hCAbXTxwUuorSxhprRmtnGoPxTm.jpeg)![15531724467072934461873519331142|375x500](upload://mnyYm9jfvxHBmOvWYjtjgCFo3rQ.jpeg) 
I should have gotten the 2s3p modules from the start, much cleaner than twice of 1s3p plus more stability. Btw: used fishpaper rings on the plus pole this time, just to be more sure 😏
```

---
## \#964 Posted by: agniusm Posted at: 2019-03-23T17:56:09.404Z Reads: 187

```
Must be paint in the a.. charging each module separately? Any plans for BMS?
```

---
## \#965 Posted by: visnu777 Posted at: 2019-03-23T18:14:22.103Z Reads: 196

```
No, I don't trust them :D. There is no space for a good BMS but I might build an external BMS charger with a DieBMS like someone here in the forum. Actually I sometimes balance and check every single cell for internal resistance :)
Edit: I have a brick charger too which I normally use. The hobby charger is for balancing manually ;)
```

---
## \#966 Posted by: mishrasubhransu Posted at: 2019-03-24T07:49:37.868Z Reads: 203

```
I'll start working on a new board and this time it will be 10S5P, based on the tested 4P module post that I am replying to. Still wanted to go with the same layout as before(see the last pic) but wasn't possible given the deck and enclosure size, so I'll be using something like in the pics below.
1. It's printed as 2 part and joined with some PETG specific glue(MEK maybe). 
1. The downward "v" is not for vendetta, but actually to better conform to the curve of the deck.  
2. I am going for vibration absorbing standoff which Agnius had suggested at some point. 
3. The series connection between adjacent modules will be made by soldering a u shaped flexible wire.
4. The distance between the 2 end lines is 190mm(7.4").  The space in between the standoffs will be used to mount the enclosure, ensuring max space utilization. Planning to use with a 9.5" wide deck.
5. The only(&major) issue is that these are rated for compression and my use case is tension. lets see. 
![image|690x227](upload://vQ139vmcE2OeY2i5hNFD2D6Q5H7.png) 
![5P5P_1|690x288](upload://g5XvkFmcajL0BWt6zTQWjOqYzQp.jpeg) ![5P5P_2|690x425](upload://pzksqARk9mmN1xvwvo42QiTVZdv.jpeg) ![5P5P_3|690x403](upload://6kVHz9w5sECtubPXiZxaznSEFrv.jpeg) ![5P5P_4|690x357](upload://brjlr09YZtLj7jMdMQsO1ORWSg5.jpeg) 

old setup for reference
![image|690x350](upload://2gizM6EyyxQ1YKQGVx0YGBgETLt.jpeg)

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words/2992/10402?u=mishrasubhransu
```

---
## \#967 Posted by: mishrasubhransu Posted at: 2019-03-24T21:59:13.160Z Reads: 201

```
Turned out pretty well.

![IMG_20190324_155012|666x500](upload://n3pFsiUccBYAFevT6oNCzFoMI8S.jpeg) 
![IMG_20190324_161556|666x500](upload://r2s9O53GeT6VxXVhHXjD1cBeec7.jpeg) 
![IMG_20190324_174045|666x500](upload://576EmJPOq8b7sVS1regICBot6bc.jpeg) 
![IMG_20190324_174052|666x500](upload://9YpxZMb7cpM7J6P2lxIWu3Xin6I.jpeg) 
![IMG_20190324_172900|666x500](upload://qV52nLtUE4EcWNoxlLOuQ9RAM4t.jpeg) 
https://photos.app.goo.gl/17amAr75XXpcp3pq8
```

---
## \#968 Posted by: rey8801 Posted at: 2019-03-24T22:41:31.426Z Reads: 187

```
Looks good man!
```

---
## \#969 Posted by: banjaxxed Posted at: 2019-03-24T22:55:45.824Z Reads: 185

```
Looks good, lid stays closed right through the parts?
```

---
## \#970 Posted by: mishrasubhransu Posted at: 2019-03-24T23:43:44.957Z Reads: 188

```
I didn't get what you were asking, but if it's about the lid placement then it's will be like in the pic below. I haven't printed the lid yet

![image|333x250](upload://acvhxGNTDejCuieQqroJzjeXI2i.jpeg)
```

---
## \#971 Posted by: skatardude10 Posted at: 2019-03-24T23:51:40.845Z Reads: 191

```
You should add a small shock absorbing washer to the top of the screw (screw head, thin hard washer, shock washer, PETG case, bottom shock washer that you have)

That way it's shock absorbing either way and not just one. Just need a slightly longer screw, current design should accommodate just fine.

Fuckin sexy too btw!
```

---
## \#972 Posted by: Benjamin899 Posted at: 2019-03-25T01:38:06.970Z Reads: 185

```
@agniusm are you going to sell 21700 tabs?
```

---
## \#973 Posted by: mishrasubhransu Posted at: 2019-03-25T03:34:23.474Z Reads: 192

```
I get what you are saying, but if you hold these shock standoffs you will realize they won't help. The crew doesn't go all the way through. I have to search for a different kind of shockproof washer to do that.
```

---
## \#974 Posted by: banjaxxed Posted at: 2019-03-25T04:40:28.632Z Reads: 187

```
I’m preparing some cell holders for welding 21700, some great cells coming out in this size
```

---
## \#975 Posted by: mishrasubhransu Posted at: 2019-03-25T05:54:31.900Z Reads: 188

```
I was wondering if anyone in the USA has 3 qty of 5P(or higher) NESE tabs, to sell/exchange. I have lots of new 4P and 3P tabs if you are willing to exchange. Please PM me.
```

---
## \#976 Posted by: Benjamin899 Posted at: 2019-03-25T12:34:48.445Z Reads: 185

```
aliexpress has a sale again, and i rly want to try the liitokal 21700 out. They just brake every metric, based lygte data.
```

---
## \#977 Posted by: goldrabe Posted at: 2019-03-30T03:09:31.946Z Reads: 183

```
@agniusm
The modules arrived today, thanks! Feels much more solid then my impression from the photos. 
![PSX_20190330_120318|690x388](upload://mWaLhmBcnad6isDqCSAZyzBJaV4.jpeg)
```

---
## \#978 Posted by: mishrasubhransu Posted at: 2019-03-30T03:23:12.736Z Reads: 179

```
Wow, so many! How many packs are you building?
```

---
## \#979 Posted by: goldrabe Posted at: 2019-03-30T03:27:13.734Z Reads: 177

```
Two packs, 11S8P Samsung 35E and 10S4P 30Q if only Nkon shipping was faster. :grinning:
```

---
## \#980 Posted by: agniusm Posted at: 2019-03-30T06:43:32.156Z Reads: 172

```
Great that they are with you. More solid, is it a good thing or bad ? :)
```

---
## \#981 Posted by: goldrabe Posted at: 2019-03-30T07:52:10.141Z Reads: 173

```
Good thing!\
Compression is strong the cells are sitting tight, I am stoked! I would have spent the same amount on Spotwelder, Nickel strips, shrink wrap etc. I like the fact that I can reuse your modules once the cells are bad. You developed a unique product and therefore I don't see it as too expensive! 
Looking forward to the 21700 modules :grinning:
```

---
## \#982 Posted by: gmurad Posted at: 2019-03-31T14:48:18.976Z Reads: 173

```
I'm doing a 12s4p pack. I guess I can get to that configuration through 2s4p modules or 1s4p ones. When I buy a 12s4p hardware set from https://18650.lt/index.php/product/n-e-s-e-hardware-set-2/ which module configuration is it compatible with?
```

---
## \#983 Posted by: Benjamin899 Posted at: 2019-03-31T15:59:56.599Z Reads: 168

```
look at the series tabs included. you get the amount needed to build it with 1s Modules.
```

---
## \#984 Posted by: gmurad Posted at: 2019-03-31T16:01:30.680Z Reads: 173

```
Then where is the hardware for the 2s4p modules?
```

---
## \#985 Posted by: Benjamin899 Posted at: 2019-03-31T16:04:01.065Z Reads: 170

```
you buy the parts seperately.
```

---
## \#986 Posted by: beherit Posted at: 2019-04-03T16:49:16.526Z Reads: 167

```
Mine arrived! Bought a single enclosure for scaling my own print and the parts for a 14s5p for my e-bike. Took about a month to arrive to western Canada on flat rate shipping. I'm really impressed by your print quality, it's stunning and could easily make me think it's injection molded. I'm noticing the part that arrived is a different design than my own though. Your part does not have the ledges that separate the batteries, although the version on your site does. It has some ledging, but on the 5P and 3P vented models from your site it's a big difference. ie. OOOOO vs. O^O^O^O^O

EDIT: I suppose a better way to describe it is that the part I was sold has its vents in between the batteries, but the printable parts have them on the battery itself, with the area between the batteries being plastic. Is this intentional?

EDIT 2: Is a heat gun mandatory? I can't seem to fit the cells in the part I was sent without a large bulge in the middle.
```

---
## \#987 Posted by: nirurin Posted at: 2019-04-03T17:42:38.275Z Reads: 165

```
Interesting, I had assumed that all the NESE modules had the ledging gaps. I had originally thought to remove those in my own version, but then I saw a 'how to' video using them that showed the batteries were flush against each other, so I just thought those ledges weren't as big a gap as it seemed from the 3d model. 

Now I'm wondering if the module in the video didn't have those ledges. I need to do a test myself really but I still haven't gotten around to ordering my batteries haha
```

---
## \#988 Posted by: gmurad Posted at: 2019-04-03T19:34:33.082Z Reads: 158

```
Took 1 month to arrive in Canada after ordering? I better place my order soon then.
```

---
## \#989 Posted by: mishrasubhransu Posted at: 2019-04-03T23:09:32.296Z Reads: 170

```
You shouldn't have to use heatgun at all. If you have a calliper measure how wide are your cells. Shouldn't be anymore than 18.3mm. 

[quote="beherit, post:986, topic:36847"]
Your part does not have the ledges that separate the batteries, although the version on your site does. It has some ledging, but on the 5P and 3P vented models from your site it’s a big difference. ie. OOOOO vs. O^O^O^O^O
[/quote]
Pics would be nice when describing an issue.
```

---
## \#990 Posted by: beherit Posted at: 2019-04-03T23:28:35.608Z Reads: 173

```
Admittedly, I was avoiding pics to not show my awful PETG print job. But here's some.

Difference between model on site and sent print:

![IMG_20190403_161531_633|150x100](upload://wzPAAXacqhJQd24yhdfAxQZWwX6.jpeg) 

The tight fit for my Sanyo NCR18650GA cells, roughly 18.5mm. (electrical tape is over minor dings in the wrapping, not thick enough to greatly effect cell width).

![IMG_20190403_161519_108|250x100](upload://sLC1YdxkqkCYnuuI6KoJbGrw2mv.jpeg)

EDIT: With some liberal use of strength I've managed to get them in pretty well, however the sides (pos/neg of cells) bulge making the lid very difficult to put on...
```

---
## \#991 Posted by: mishrasubhransu Posted at: 2019-04-04T01:03:50.211Z Reads: 167

```
By design it's a tight fit to save as much space as possible, so the addition of the black tape on either side makes it not fit. You should remove them and try again.

[quote="beherit, post:990, topic:36847"]
electrical tape is over minor dings in the wrapping, not thick enough to greatly effect cell width
[/quote]
It actually is pretty significant. I had a kapton tape to insulate two parallel groups and even that caused tightness. They are parallel groups so you don't need that extra insulation(black tape)
```

---
## \#992 Posted by: beherit Posted at: 2019-04-04T01:43:27.946Z Reads: 160

```
Wouldn't bare cells touching cause a major issue? Even if they're parallel and wouldn't short. wouldn't the current transfer between the bare-area and not utilize the whole cell?
```

---
## \#993 Posted by: mishrasubhransu Posted at: 2019-04-04T01:46:57.826Z Reads: 161

```
Nope! They are all connected through the same thick metal. Where you connect, doesn't matter. I have seen Agnius remove the entire cover in the parallel groups. 

BTW, where did you get the files from? There are updated files in this thread above. look for google drive link.
```

---
## \#994 Posted by: beherit Posted at: 2019-04-04T01:53:16.989Z Reads: 158

```
I grabbed them from the resources page on 18650.lt, last updated 2018.
```

---
## \#995 Posted by: mishrasubhransu Posted at: 2019-04-04T01:55:31.940Z Reads: 158

```
Those are old files. Search for google drive link above.
```

---
## \#996 Posted by: mishrasubhransu Posted at: 2019-04-05T01:16:23.365Z Reads: 158

```
Good brand 18650 cells available at $2(flash sale) in the usa. Shipping is $6 in USA. 
https://www.electric-skateboard.builders/t/molicel-p26a-2600mah-25a-1-99-cell-imr
```

---
## \#997 Posted by: Benjamin899 Posted at: 2019-04-05T08:07:03.119Z Reads: 158

```
Saw that. Really nice. Sadly I am eu
```

---
## \#998 Posted by: ron Posted at: 2019-04-05T17:37:15.194Z Reads: 155

```
One question, how to you stance the holes and press the molds/buttons or whatever you call them into the Nickel strips?

Would want to experiment with nese modules but more i am planning to do some custom 10s packs and need some tips/hints..

Thanks in advance
Greetings Ron.
```

---
## \#999 Posted by: mishrasubhransu Posted at: 2019-04-05T19:12:00.615Z Reads: 151

```
Well your question is for @agniusm and NESE is his product. I just bought the copper tabs from him and made my own custom boxes.
```

---
## \#1000 Posted by: agniusm Posted at: 2019-04-05T20:44:41.055Z Reads: 159

```
@beherit, most recent models are linked here. They are not on 18650.lt as i run them to be sure they are 100%. If you feel its too tight, just scale  when you slicing uniformly by 1-2% and you should be fine. Most of the time printers dont have 0.01 tolerances so 0.15 or 0.2 would make that difference not fitting well.
.
@mishrasubhransu i have finally sorted customs and yours will ship tomorrow. Sorry for the delay, still adjusting to increased demand.
```

---
## \#1001 Posted by: beherit Posted at: 2019-04-06T00:08:57.082Z Reads: 156

```
Thanks. I find 102% is a nice fit, maybe a little loose. I eventually got the cells and lid to fit on the case you sent, it was just a little difficult. I'm saving on cash so instead of buying ninjaflex for the caps I just scaled the single caps to 118% which fits pretty tight onto the screw.
```

---
## \#1002 Posted by: mishrasubhransu Posted at: 2019-04-06T01:39:30.664Z Reads: 156

```
I am currently printing at 100.5. So give it a couple more tries. What filament are you using?
```

---
## \#1003 Posted by: beherit Posted at: 2019-04-06T01:51:58.255Z Reads: 161

```
I use Econofil PETG, although fighting that first layer to stop blobbing has likely been the root of a lot of my issues. I'll slowly move down from 102 to 101 or 100.5 and see what works best for me.
```

---
## \#1004 Posted by: skatardude10 Posted at: 2019-04-06T01:56:00.194Z Reads: 162

```
Do you use a glass bed? What temp bed? Do you use glue stick?

I have issues with PETG blobbing sometimes when I use gluestick, but PETG on raw clean glass sticks great. Only problem is that one time it took some glass with it but usually it's not an issue. 

How about initial layer Z height? First layer speed? Do you do a nozzle wipe routine prior to printing the part? Clean nozzle? Silicone sock? 

I think any of these will help, slightly higher initial Z height, slower speed, hotter bed, clean nozzle, silicone sock, nozzle wipe to prevent blobbing from starting and getting flow going, print without glue, print on raw glass... 

I'm sure there are other better tips for reducing PETG blobbing but these worked for me for the most part
```

---
## \#1005 Posted by: mishrasubhransu Posted at: 2019-04-06T02:07:55.835Z Reads: 168

```
I used to have blobs but 3 things removed all blobbing. 
1. Putting a silicone sock(I glued it to the heater block using some silicone sealant) 
2. Putting a thin layer of the silicone sealant on the exposed nozzle itself 
3. Raise the nozzle just a little bit from the bed than what you would do for PLA. 

For sticking to the glass bed I use hairspray once in a while, but spray isopropyl alcohol before every print to reactivate the hairspray that is still present on the bed. This prevents a constant build up of hairspray on the bed. Also I print at 245 without any cooling. That greatly improves layer adhesion and hence the strength. Print speed 40mm/sec and nozzle dia 0.4mm
https://photos.app.goo.gl/hiPoPTuzp3ihgFyg6
![image|666x500](upload://cM2fbKpvicHBSRKl5E6tA4R3Xxs.jpeg)
```

---
## \#1006 Posted by: beherit Posted at: 2019-04-06T02:24:37.516Z Reads: 165

```
I actually just got my perfect layer height going today, so way less blobbing! I use a gluestick layer over the PEI sheet on my glass bed at 70c, 245c for the Econofil PETG with no cooling. I found a silicone sock made printing worse, or at least it did when it got caught in the print one day. Moved my retraction up to 4mm too, that helped.

EDIT: My main scaling problem is that the positive/negative sides of the battery bulge the case out slightly, so the lid requires a lot of hand strength to make the slots line up.
```

---
## \#1007 Posted by: mishrasubhransu Posted at: 2019-04-06T06:17:22.335Z Reads: 168

```
[quote="agniusm, post:1000, topic:36847"]
@mishrasubhransu i have finally sorted customs and yours will ship tomorrow. Sorry for the delay, still adjusting to increased demand.
[/quote]

No problem, I am waiting for some cells too. 10S5P boxes are ready though.  
![image|666x500](upload://47ZXSJQlwZC2o40arAPmIL6RcBI.jpeg)
```

---
## \#1008 Posted by: agniusm Posted at: 2019-04-06T18:01:54.410Z Reads: 164

```
DIY'ing tabs would still be a lot more expensive. You need to make a die, then get the tabs cut to shape and punch them. I paid 150€ for my test die plus
30€ for clamps. Then it cost me 70ct per one copper tab to laser cut it. 
Making them from nickel strip reneders little sence, better spotweld battery pack.
They are not too expensive when you start adding things up. You can look up abother project here that was meant to make cheaper versions of what i have. He used copper braid and it ended up being just marginally cheaper.
```

---
## \#1009 Posted by: agniusm Posted at: 2019-04-09T17:41:30.960Z Reads: 154

```
Perhaps someone knows how to insert a reply at the top of the page or even if mods can do it? Would like to get most important stuff there so people wont have to dig through all the chat.
```

---
## \#1010 Posted by: mishrasubhransu Posted at: 2019-04-09T19:04:56.846Z Reads: 156

```
@agniusm You could and should create a new thread--your own thread--with all details, photos, FAQ, designs, user builds, etc and we'll just start posting there. That way we can get rid of a lot of junk post(a lot from me, hehe) and start clean.

You'll also have the editing power of the 1st post for 3 or 6 months. 
 
We can ask a mod to edit to put that as a link on the very top of this thread. So that people know where to go.
```

---
## \#1011 Posted by: Benjamin899 Posted at: 2019-04-09T19:08:04.798Z Reads: 150

```
lol true, i thought this is his thread^^
```

---
## \#1012 Posted by: agniusm Posted at: 2019-04-09T19:17:19.243Z Reads: 151

```
Sounds good.
```

---
## \#1013 Posted by: agniusm Posted at: 2019-04-09T19:18:08.515Z Reads: 154

```
The man in the first post invited me to comment and it all started
```

---
## \#1014 Posted by: beherit Posted at: 2019-04-11T02:35:37.542Z Reads: 152

```
Not even done building and every time my sharp Vruzend kit scratches my hands during assembly, it acts as a reminder of how much better I like this design :slight_smile:
```

---
## \#1015 Posted by: banjaxxed Posted at: 2019-04-11T07:11:10.635Z Reads: 153

```
Beetlejuice Beetlejuice Beetlejuice
```

---
## \#1016 Posted by: gmurad Posted at: 2019-04-20T12:19:59.123Z Reads: 147

```
Hey, I bought N.E.S.E Tabs from the website and planning on using the 2s4p cases for a 12s4p battery that will go in a HAYA deck. Does the layout bellow make sense? Is there a better layout? Thanks.

![image|408x500](upload://mz1KEX2UzhoVXDMApaNmwExNF9o.png)
```

---
## \#1017 Posted by: Benjamin899 Posted at: 2019-04-20T13:22:13.300Z Reads: 144

```
looks good to me.
```

---
## \#1018 Posted by: rey8801 Posted at: 2019-04-20T13:29:33.476Z Reads: 143

```
Looks good. Same I will do but make sure you have space left for vesc ecc... Otherwise you can go with 5 2s4p modules and two 1s4p modules where one side has two 2s4p and one 1s4p modules and the other has three 2s4p and one 1s4p modules. Depends on the space available
```

---
## \#1019 Posted by: mishrasubhransu Posted at: 2019-04-21T04:08:00.232Z Reads: 140

```
@agniusm, any updates on this?
```

---
## \#1020 Posted by: agniusm Posted at: 2019-04-21T05:32:52.839Z Reads: 144

```
On the new thread? Had no time yet to sit and put it all together.
I need to find some time to finish 2 of the ebikes till june. 1 battery build and one more intense build with welding and stuff :slight_smile:
![20180521_184527|666x500](upload://8688NmjDCVpTbrM0UAn6NophBU.jpeg) 
![20180527_163000|375x500](upload://yIY8UgEaUPydCG9pNd6A3tCHTKN.jpeg)
```

---
## \#1021 Posted by: mishrasubhransu Posted at: 2019-04-21T06:09:12.492Z Reads: 145

```
Looking at the pics, I have so many questions.
1. Is the big space between the seat and the rear tire for hauling cargo and/or your kids? Haha
2. Battery capacity and size?
3. Where do you normally post about your projects? Endless-sphere?
4. Is that a huge metal zip tie holding the NESE boxes together? Where to get them?
```

---
## \#1022 Posted by: agniusm Posted at: 2019-04-21T06:23:04.803Z Reads: 144

```
1. Kids and wife
2. 20S 15AH (will be upgraded to 20ah)
3. Usually ES but not for some time, i have none of it 😂
4. Yes, SS from aliexpress
```

---
## \#1023 Posted by: banjaxxed Posted at: 2019-04-21T16:34:32.678Z Reads: 148

```
Cool fabrication mate
```

---
## \#1024 Posted by: agniusm Posted at: 2019-04-26T10:32:15.887Z Reads: 140

```
Listing this here as well:
I have 20S6P kit that was intended for my cargo bike. Driven 200 meters  and crappy BMS drained my cells dry over winter. I am building new one, only larger.
Modules are in bright red color and include everything to build 20S6P battery pack. Very easy to build and even easier to take apart to swap cells. The kit is reusable and can serve for a lifetime of human.
List:
20 6P modules (bright red)
19 series bus bars
19 twin bolt caps (blue)
2 single bolt cap (orange/blue)
[img]http://18650.lt/wp-content/uploads/2017/07/DSCN1262-564x1024.jpg[/img]

**50% off of the retail**

Price, 150EUR includes world wide shipping.

**SOLD**
```

---
## \#1025 Posted by: agniusm Posted at: 2019-04-26T15:58:45.920Z Reads: 133

```
Guys, i had a moment :) Brilliant idea came, tested and its fantastic. I have used M3 threaded rods to slide on the modules. Works great. You only need 2 aluminium angles to mount to the board and its flexible. If you leave a small gap between modules it will flex good both ways. ![20190426_184822_HDR|375x500](upload://p1yFpK7A0agxImEDJtC5zMX8Hqt.jpeg) 

![20190426_184833|666x500](upload://njdAM0oyyyGLW6Cm1J34kRVsd6z.jpeg)

...and you can have more of them for strength. I paid 0.50ct/m
```

---
## \#1026 Posted by: visnu777 Posted at: 2019-04-26T16:03:22.315Z Reads: 127

```
A little reinforcment of the channel might be necessary, maybe test it on your shaking table first :) But the ide itself is great :)
```

---
## \#1027 Posted by: agniusm Posted at: 2019-04-26T16:04:33.827Z Reads: 125

```
You suppose to mount them as per second photo. Should be tons of strength
```

---
## \#1028 Posted by: visnu777 Posted at: 2019-04-26T16:10:15.428Z Reads: 132

```
Don't underestimate the vibrations working on the heavy (when filled with cells) cases. The threads might scrub the petg and finally break it. I just tested the stability of the spot on a broken case with a punch on a flat screwdriver -> broken, so it might need reinforcement and maybe only threads on the ends of the rods.
```

---
## \#1029 Posted by: agniusm Posted at: 2019-04-26T17:23:10.553Z Reads: 130

```
Sure needs road testing. I am going to mount my bike battery like that but vibrations are far milder
```

---
## \#1030 Posted by: mishrasubhransu Posted at: 2019-04-26T18:19:19.976Z Reads: 133

```
Nice!

In my latest iteration, I am using 3mm carbon fiber rod in similar fashion. I say similar, because instead of holding the m3 rods on the edges of the box, it holds in the middle. This allows for max flexibility. There is a piece of 1mm tpu slice in between each module. In addition, each module is mounted to the board using a tpu mount.
```

---
## \#1031 Posted by: ryansinatra Posted at: 2019-04-26T23:37:49.025Z Reads: 131

```
Struggling with my battery right now. Never used. All cells were brand new from @thisguyhere and at the same voltage going in. Each group is at 4.19 to 4.2v except one that is at 4.08 

I am getting a green light on my charger though so I cannot get the single group to go up 

Full pack reads like 41.5v

![IMG_20190426_192530|374x500](upload://cPMjL5eQpNiinUGirSODJUt1nlC.jpeg)
```

---
## \#1032 Posted by: ryansinatra Posted at: 2019-04-26T23:38:09.841Z Reads: 123

```
Do I need to discharge it a bit and re balance charge or?
```

---
## \#1033 Posted by: mishrasubhransu Posted at: 2019-04-26T23:55:55.463Z Reads: 123

```
I have those cheap BMS too and they slow to balance. Just give it time or if you have a hobby charger, charge each parallel groups to full individually and then will be fine.
```

---
## \#1034 Posted by: ryansinatra Posted at: 2019-04-26T23:58:59.612Z Reads: 120

```
Will it still balance and charge even if light on the charger is green?
```

---
## \#1035 Posted by: ryansinatra Posted at: 2019-04-26T23:59:24.877Z Reads: 118

```
I need to buy a hobby charger for sure
```

---
## \#1036 Posted by: mishrasubhransu Posted at: 2019-04-27T00:15:12.147Z Reads: 116

```
You can take a multimeter and see if balancing is happening. Check over 15 minutes duration.
```

---
## \#1037 Posted by: ryansinatra Posted at: 2019-04-27T00:22:05.190Z Reads: 118

```
Yeah I don't think anything is happening :/ just sits at 4.05 while others at 4.18
```

---
## \#1038 Posted by: Winfly Posted at: 2019-04-27T00:43:19.135Z Reads: 120

```
You need to manually balance it. 0.1v is too off.
```

---
## \#1039 Posted by: ryansinatra Posted at: 2019-04-27T00:45:08.306Z Reads: 122

```
Recommendations for hobby chargers are appreciated,I don't have one and I'm sure that's really the only way.
```

---
## \#1040 Posted by: Winfly Posted at: 2019-04-27T00:47:45.277Z Reads: 126

```
If you wanna do it for cheap. You can use these Tp4056 and charge them up slowly


TP4056 Charging Module 5V Micro USB 1A 18650 Lithium Battery Charging Board with Protection Charger Module https://www.amazon.com/dp/B071RG4YWM/ref=cm_sw_r_cp_apa_i_dA6WCbBPQF72X
```

---
## \#1041 Posted by: ryansinatra Posted at: 2019-04-27T00:52:03.263Z Reads: 123

```
Would I just wire the + and - to alligator clips and charge the p group?
```

---
## \#1042 Posted by: Winfly Posted at: 2019-04-27T00:55:32.900Z Reads: 129

```
Yeah. Or use jumper wires and stick them into the balance wire jst connector.
```

---
## \#1043 Posted by: ryansinatra Posted at: 2019-04-27T01:15:21.482Z Reads: 129

```
![IMG_20190426_211448|375x500](upload://qB2GjJ9vcR77QKbHtPrrA4vXQFd.jpeg)
```

---
## \#1044 Posted by: ryansinatra Posted at: 2019-04-27T01:15:41.356Z Reads: 123

```
Surprisingly I had one from a remote build
```

---
## \#1045 Posted by: Winfly Posted at: 2019-04-27T01:15:52.080Z Reads: 122

```
No, wire to the out +-.
```

---
## \#1046 Posted by: ryansinatra Posted at: 2019-04-27T01:16:23.642Z Reads: 124

```
The out + and - only was pushing 4.12v where as these terminals we're pushing 5
```

---
## \#1047 Posted by: Winfly Posted at: 2019-04-27T01:16:52.423Z Reads: 124

```
Because it's 5v from usb it's not gonna know when to stop. That PCB step down 5V from usb to 1s charge voltage.
```

---
## \#1048 Posted by: ryansinatra Posted at: 2019-04-27T01:17:17.067Z Reads: 120

```
I can't just watch it and stop it at 4.18 or so?
```

---
## \#1049 Posted by: Winfly Posted at: 2019-04-27T01:30:33.199Z Reads: 117

```
Then you will have to watch it.
```

---
## \#1050 Posted by: ryansinatra Posted at: 2019-04-27T01:33:40.714Z Reads: 109

```
Checking it every damn minute until it matches the others. Thanks again for the tip on the charger board 👌much appreciated
```

---
## \#1051 Posted by: deucesdown Posted at: 2019-04-27T01:48:20.350Z Reads: 120

```
[quote="ryansinatra, post:1031, topic:36847"]
Each group is at 4.19 to 4.2v except one that is at 4.08
[/quote]

If I were you I'd check the cells in the last group. Decent chance there's a bad cell in that group, no? NESE gives you the option to test each cell.
```

---
## \#1052 Posted by: ryansinatra Posted at: 2019-04-27T02:00:56.660Z Reads: 118

```
The cells are brand new and we're all tested for voltage before putting them in the packs. Literally never used this pack yet. I doubt there is a bad cell. I just think I had a faulty BMS hooked up to it when I first built it, and a resistor drained that group a bit.
```

---
## \#1053 Posted by: ryansinatra Posted at: 2019-04-27T02:01:20.450Z Reads: 117

```
The pack is now balanced. Every group is at 4.17-4.18
```

---
## \#1055 Posted by: ryansinatra Posted at: 2019-04-27T02:26:02.073Z Reads: 117

```
Will bad cells not hold a charge on their own?
```

---
## \#1056 Posted by: deucesdown Posted at: 2019-04-27T02:56:33.094Z Reads: 122

```
I was concerned because .1v drop across 4 parallel cells while doing nothing is quite a lot. Are you hooking up that red BMS again to confirm?

I'm concerned personally because I have 2 of those BMS waiting for builds. :slight_smile:
```

---
## \#1057 Posted by: ryansinatra Posted at: 2019-04-27T03:48:43.578Z Reads: 120

```
It's a 3p pack. Maybe that p group just has a bad cell. Time will tell. I doubt it's the BMS since it was low before I received this BMS
```

---
## \#1058 Posted by: deucesdown Posted at: 2019-04-27T03:57:36.449Z Reads: 124

```
wait so were the cells all at the same voltage when you got them, then on  first charge group charged slower? Hmm. Equal chance on weak cell, dodgy balance wiring, or dodgy bms...
```

---
## \#1059 Posted by: ryansinatra Posted at: 2019-04-27T04:26:37.425Z Reads: 127

```
I had this pack assembled differently before with a different BMS but did not end up using it. I charged it once with that other BMS and then it had been sitting. I recently reassembled the modules to a brick like this for a top mount build and upon checking the voltages, this one p group was low yes.
```

---
## \#1060 Posted by: mishrasubhransu Posted at: 2019-04-27T07:32:21.020Z Reads: 131

```
@agniusm, I upgraded my ender3 to BGM+E3DV6 direct drive setup. Since you have direct drive too and get such clean prints I was wondering what is your
1. Print temperature
2.  Retraction distance
3. Retraction speed
4. Retraction prime speed

For PETG. Thanks so much.
```

---
## \#1061 Posted by: agniusm Posted at: 2019-04-27T07:53:47.838Z Reads: 129

```
Whats your slicer? Mine has linear rails on x and y.
```

---
## \#1062 Posted by: rey8801 Posted at: 2019-04-27T08:08:50.236Z Reads: 127

```
linear rails make a lot of difference. I am looking at it for my CNC, never though on a 3d printer but indeed the principle is the same.
```

---
## \#1063 Posted by: mishrasubhransu Posted at: 2019-04-27T09:08:50.367Z Reads: 140

```
Linear rails would improve the dimensional accuracy for sure, but didn't realize it would have that much effect on visual quality. When you changed over to rails, what was the biggest advantage that you saw?

I am using Cura. I am having a bit of blobbing.  I currently have:
1. print temp 245C
2. Retraction Distance: 0.2mm
3. Retraction speed: 60mm/sec
4. Retraction print speed: 40mm/sec
5. Coasting enabled
```

---
## \#1064 Posted by: agniusm Posted at: 2019-04-27T10:07:23.213Z Reads: 146

```
Use Slic3r PE (prusa edition)
![image|690x373](upload://gOfhuEbq2hURjereAzAURZJkToS.png) 
![image|690x373](upload://v0UQYeUoltok0nJSsjjSNQvhIbY.png) 
![image|690x373](upload://nHDz0hJ8tMENEAtVinfoBnxWKYl.png) 
![image|690x373](upload://yJmYEzzr23PTRXmi7kNjdEpnl3u.png) 
![image|690x373](upload://9svE1eQ4k2BaDRiU3uZ89XA1oNm.png) 
![image|690x373](upload://bpr8oUTQiK5PX8KG6DAMU5kT1wT.png)
```

---
## \#1065 Posted by: gmurad Posted at: 2019-04-27T11:21:13.680Z Reads: 123

```
Hey, do you print out of a Prusa? Thanks for the settings! I'm gonna be printing the cases (was gonna use the CR10s pro, but now will use the PRUSA instead) soon so this will be useful.
```

---
## \#1066 Posted by: agniusm Posted at: 2019-04-27T12:09:39.212Z Reads: 124

```
I print out of many. Prusa mk2 zaribo one of them. Slic3r pe is suited for every printed, its bot specifically tied to their printers
```

---
## \#1067 Posted by: Mikolaj Posted at: 2019-04-27T16:48:33.440Z Reads: 125

```
Hello. I am planning to build a 12s6P pack yo fit a Trampa's Monster box with the internal dimensions usable for the battery  205mm x 190mm x74 mm. Can anyone reccomend best wiring diagram and which moduls I should use. Also recomendations for charge/discharge bms will be much appreciated
```

---
## \#1068 Posted by: agniusm Posted at: 2019-04-27T18:03:58.611Z Reads: 128

```
You wont be able to fit that many in that space. Single 6P module is 22x74.2x123mm.
12 modules are 264mm.
```

---
## \#1069 Posted by: Mikolaj Posted at: 2019-04-27T19:01:14.080Z Reads: 131

```
Would I be able to fit 12S4P pack do you think?
```

---
## \#1070 Posted by: mishrasubhransu Posted at: 2019-04-28T06:20:36.428Z Reads: 126

```
Thanks so much. I'll put them in an see how the print comes out.
```

---
## \#1071 Posted by: agniusm Posted at: 2019-04-28T06:55:33.367Z Reads: 129

```
You can fit up to 18S4P in that space using 2S4P modules. They are 168mm in length so they utilyze space better.
```

---
## \#1072 Posted by: Mikolaj Posted at: 2019-04-28T08:24:13.631Z Reads: 125

```
Thanks. Just checked your website and see that you selling printed 4P modules. How would I need to proceed if I wanted to buy 12 printed moduls and all of the hardware that is required to build the pack. Also would you or enyone else be able to provide a wiring/conecting diagram with bms
```

---
## \#1073 Posted by: agniusm Posted at: 2019-04-28T09:23:11.860Z Reads: 121

```
For wiring see post 692.
For buying component just go on the website and order:

12 4P modules (or 6 2S4P modules)

11 series bus bars (or 10 ↑)

optional:

11 twin bolt caps or (or 8 ↑)

2 single bolt caps or (or 4 ↑)

1 ring terminal set

1 tube ring lugs of chosen wire gauge

Dont forget to check resources area to double check dimensions. Bolt, series bus bar and cap adds 10mm to the module.
```

---
## \#1074 Posted by: agniusm Posted at: 2019-04-28T09:26:37.059Z Reads: 116

```
**2P and 2S2P module prices are reduced by 20%. Permanent.**
```

---
## \#1075 Posted by: Mikolaj Posted at: 2019-04-28T11:09:13.878Z Reads: 114

```
Thanks for all the info I am just bit worried that 12S4P may not give me enough range for mountain board
```

---
## \#1076 Posted by: nirurin Posted at: 2019-04-28T23:18:05.961Z Reads: 114

```
How are you guys mounting your NESE modules to the board? Are you just bolting them straight into the board inserts, or are you using some kind of rubber washers or vibration mountings?
```

---
## \#1077 Posted by: ryansinatra Posted at: 2019-04-28T23:23:07.273Z Reads: 110

```
Same way you would mount any battery for me. Neoprene for anti vibration then gorilla tape
```

---
## \#1078 Posted by: Tadagami Posted at: 2019-04-28T23:26:11.918Z Reads: 117

```
I think I saw printable models of holders for NESE modules. Not sure but it was somewhere on the NESE site. So if you have an access to 3Dprinter you can use them.
```

---
## \#1079 Posted by: ryansinatra Posted at: 2019-04-28T23:35:47.838Z Reads: 117

```
@mishrasubhransu made those yeah! You could use that too
```

---
## \#1080 Posted by: mishrasubhransu Posted at: 2019-04-29T00:02:44.579Z Reads: 132

```
I have successfully used 2 different techniques, one uses 3D printer and the other uses vibration standoffs from aliexpress. Basically it is highly desirable to put everything on/inside mounts/pads/sheets to increase functional life of your parts whether it be electronics or mechanical parts. I have had capacitors fall out after 1000km or so. I have since made sure to mount/surround everything with sponge/flexible plastic/rubber based structures.

# 3D printed mounts
https://www.thingiverse.com/thing:3444525
![image|300x270](upload://k7J67ywSmcgOW7wMNiqEU8ptGxv.png) 
![image|666x500](upload://5wJWP5xggsbWL44v6zkxXHJDxpX.jpeg) 
![image|666x500](upload://7gMRpybJGZGzI4rKJz3mazwaQkP.jpeg) 
I currently have more than 700km on this setup above.

I also discovered recently that TPU makes a good mount too while being pretty compact. Experimenting more on it.  
https://photos.app.goo.gl/Pswa42iWmAmga6j57

# Vibration standoffs
https://www.aliexpress.com/item/8pcs-lot-M3-Male-Female-Anti-Vibration-Rubber-Isolator-Mounts-Set-8-8mm-for-Air-Compressors/32843986528.html
Don't let the size fool you. They are pretty strong in compression and in tension while having a lot of flex. 

![image|375x500](upload://fAESFjkyKNRQjOu6MOI9quZsKwU.jpeg) 
![image|666x500](upload://m9CeYf9Atw12Ch6vQGGjEcp361N.jpeg)
![image|666x500](upload://9yVtfHXIBMu3m6l4TkJBkFnA8iP.jpeg) 
![image|666x500](upload://yMgPQxcgFPjjhvXuerF98OwRK7Z.jpeg) 
This was just a trial setup that I made. Final setup will have all the balance wires tucked away nicely.
```

---
## \#1081 Posted by: nirurin Posted at: 2019-04-29T00:24:02.883Z Reads: 120

```
Those rubber standoffs are pretty much exactly what I had bookmarked, but my only concern was that they would leave a pretty big (about 8mm) gap between the nese and the board. Which might be fine, I'm not sure, that's why I'm asking :slight_smile:
 
However I see you made them offset from the NESE itself, which drops them slightly. Good plan, and should be easy enough to 3D print something that will bolt onto my printed NESE modules and add those end bolt holes to it...
```

---
## \#1082 Posted by: nirurin Posted at: 2019-04-29T00:37:39.044Z Reads: 116

```
Do you prefer the rubber standoffs version, or your own 3D printed spring mounts?
```

---
## \#1083 Posted by: mishrasubhransu Posted at: 2019-04-29T00:52:20.047Z Reads: 117

```
Rubber standoffs because they are super super compact. But mounting them is a tiny bit harder. What I had to do was to drill undersize holes in the deck, then screw in a m3 bolt making sure that I don't destroy the threads that I am creating adn then finally put the standoffs in using a vice-grip like in the images above. Ideally I would take some inserts for wood and put them in first and then mount the rubber standoffs to it using small amount of threadlocker.
```

---
## \#1084 Posted by: nirurin Posted at: 2019-04-29T01:48:01.323Z Reads: 112

```
What size bolts do you use? I'm guessing either M3 or M4?
```

---
## \#1085 Posted by: agniusm Posted at: 2019-04-29T05:37:27.786Z Reads: 113

```
If the deck is thick enough, you could sink those some by drulling larger hole and then smaller through and bolting from the top if you dont mind bolts at top side
```

---
## \#1086 Posted by: nirurin Posted at: 2019-04-29T22:12:14.059Z Reads: 109

```
Yeh I'm trying to avoid having bolts through the top of the deck if I can help it, wouldn't be so bad if it was one or two but it would be.... 28 lol. 

So would M3 bolts be enough (4 per NESE) or should I go up to M4s?
```

---
## \#1087 Posted by: mishrasubhransu Posted at: 2019-04-29T22:16:15.922Z Reads: 119

```
m3 is plenty strong. Plus, NESE has holes for m3 not m4. My [inserts](https://www.amazon.com/gp/product/B0026GSYE0) just arrived.
![IMG_20190429_181544|666x500](upload://a75Y6WzOq7qSdv9nbkRJnVAuBAI.jpeg)
```

---
## \#1088 Posted by: gmurad Posted at: 2019-04-29T22:55:29.587Z Reads: 121

```
damn, I didn't realize how long it will take to print the cases! I think it will take me ~50 hours to do a 12s4p battery.

What are some ways to connect the modules when you are putting them in this orientation? https://www.electric-skateboard.builders/t/n-e-s-e-nese-no-solder-module-battery-packs/36847/1016?u=gmurad
```

---
## \#1089 Posted by: mishrasubhransu Posted at: 2019-04-29T22:58:52.788Z Reads: 129

```
Maybe something like this? But it won't be "no solder" anymore. 
[quote="Winfly, post:219, topic:67878"]
![image|666x500](https://www.electric-skateboard.builders/uploads/db1493/original/3X/b/c/bce9ce8b9973fe32cf920f77e5aa3fae619467a5.jpeg)
![image|375x500](https://www.electric-skateboard.builders/uploads/db1493/original/3X/f/5/f5c814b89b6c6a014bf3245f53e34b753bb80063.jpeg)
[/quote]
```

---
## \#1090 Posted by: gmurad Posted at: 2019-04-29T23:05:03.784Z Reads: 130

```
:+1: I guess I can have a bullet connector on one side, some short wire and a ring connector on the other side that goes on the NESE module case bolt. I think I will try that.
```

---
## \#1091 Posted by: nirurin Posted at: 2019-04-29T23:13:30.560Z Reads: 132

```
[quote="mishrasubhransu, post:1087, topic:36847"]
m3 is plent. Plus, NESE has holes for m3 not m4.
[/quote]

Going from your pictures you didn't use the default NESE holes anyway, you added new ones onto the ends didn't you? So making those M4 instead of M3 seems straightforward. However if M3 is enough then I'll stick with that, means smaller holes in my deck too!
```

---
## \#1092 Posted by: agniusm Posted at: 2019-04-30T13:52:51.148Z Reads: 132

```
Another way of mounting nese would be to have thin sheet of aluminium or CF(~2mm) the size of assembled pack. Bolt nese to that sheet with countersunk bolts and have 4 to 6 holes to bolt that sheet to the board. Would need to check but i think it might be possible to heat insert brass inserts into the modules.
You could even mount it so the sheet faces down for protection and use longer, 23-24mm rubber standoffs like @mishrasubhransu showed
```

---
## \#1093 Posted by: agniusm Posted at: 2019-04-30T16:46:40.059Z Reads: 129

```
I will be offering new service. Anyone ordering at www.18650.lt will be able to order custom parts needed for the builds. I will not offer design service but rather printing service. As an example you might need custom controller enclosure or bracket and you have designed it so to save on shipping and looking at different 3d printing services you could just order everything in one place with your battery kit.
Here is an example. Long channel for balance wires and pcm enclosure on 10S pack with 3 wire pcm so its all nice and tidy and protected:

![20190430_142512|666x500](upload://7rFoxrCbA2nchBuZ579GVfuRAll.jpeg)
```

---
## \#1094 Posted by: IndyPilot Posted at: 2019-04-30T16:49:42.962Z Reads: 127

```
Do you guys have a website for newbs like me to buy or custom order these from you?  I am looking for a 6s2P pack without the hassle of building or having to trash a whole pack if one cell goes bad.

(LOL, I was typing when you posted your website and replied before I saw it).
```

---
## \#1095 Posted by: mishrasubhransu Posted at: 2019-04-30T18:49:26.718Z Reads: 121

```
Great idea! That will be a complete product for esk8. Maybe you should make it for selling.
```

---
## \#1096 Posted by: beherit Posted at: 2019-05-01T21:21:49.901Z Reads: 122

```
What's the record for the biggest NESE battery? Here's my 13S5P. Only outputs 25v for some reason, I likely need more contact on the positive than a single ring terminal.
![obscura1556744080914|400x200](upload://wezZ7gmPZGhPTihPY2z0vJhdFZt.jpeg)
```

---
## \#1097 Posted by: ryansinatra Posted at: 2019-05-01T23:13:44.329Z Reads: 150

```
top mount battery box i designed for my 10s3p NESE battery pack

https://www.thingiverse.com/thing:3601598

![IMG_20190501_162338|375x500](upload://iXd5SiKq6Ql1yfFaYyh3Zvu3Ubg.jpeg)
```

---
## \#1098 Posted by: agniusm Posted at: 2019-05-02T06:58:15.938Z Reads: 152

```
Not here but the biggest battery built with NESE is 20S16P i believe:
![image|547x500](upload://4ck6lkw3MKH0e0B8CmOQTTA39u2.jpeg) 
Here is what he said about the system:
_"NESE hands down. 100% better. The vruzend might have its place but overall not sold on its quality / durability long term. The hardware on them breaks way to easily. I managed to assembled all 40 modules (8 cells each) in less time than the 30 cell 12v battery. Having printed these modules in ABS following the recommended settings on your website I can say that they went together with no issues, (snug but in a good way) I will likely end up changing the 3s 10p battery for a 4s 8p NESE system."_
```

---
## \#1099 Posted by: agniusm Posted at: 2019-05-02T07:29:04.111Z Reads: 146

```
NEW THREAD CREATED, PLEASE CONTINUE THERE:

**[THE NEW NESE THREAD](https://www.electric-skateboard.builders/t/nese-the-no-solder-18650-battery-system/92517)**
```

---
## \#1100 Posted by: agniusm Posted at: 2019-05-02T07:50:48.395Z Reads: 142

```
I have missed your question. If the BMS is connected correctly, you would need to leave it on a charger for 48H to see if something is happening. These PCM's have balancing current of ~30mA so it will take a while. What is happening, the charger lights green when PCM cuts it off. Then PCM slowly(at 30mA) rate discharges all of the cells except low ones to set threshold. When cells reach that threshold, PCM will kick in charger until low cells will catch up with high cells. It will take time.
But if the cells are brand new they should be pretty equal in SOC.

NEW THREAD CREATED, PLEASE CONTINUE THERE:

**[THE NEW NESE THREAD](https://www.electric-skateboard.builders/t/nese-the-no-solder-18650-battery-system/92517)**
```

---
## \#1101 Posted by: mishrasubhransu Posted at: 2019-05-02T07:52:43.888Z Reads: 142

```
@agniusm, please consider creating a FAQ post in the new thread. That will be useful.
```

---
## \#1102 Posted by: nirurin Posted at: 2019-05-17T01:56:54.441Z Reads: 116

```
Quick question - The m5 bolts that the NESE uses for the bus bars : what length are they? 

Going by the sizing of the spacing, 10mm seems a little short, and 16mm seems a little long. I don't yet have all the tab sets though, so I figured I'd ask as it means I can pick up some correct sized bolts.
```

---
## \#1103 Posted by: cubed Posted at: 2019-06-27T04:55:50.705Z Reads: 77

```
Will these packs work with Samsung 30T batteries? Or is there no wiggle room.
```

---
## \#1104 Posted by: Benjamin899 Posted at: 2019-06-27T19:53:38.306Z Reads: 71

```
30t are standard 21700, so what is the question here?
```

---
## \#1105 Posted by: cubed Posted at: 2019-06-27T20:11:38.403Z Reads: 71

```
I couldnt find anyone who can build me a battery pack right now, so I figured Id do it myself. Since Im new to it though I was wondering if the nese packs would work or if there is an alternative for 21700 cells. Sorry for the confusion, thanks!
```

---
## \#1106 Posted by: Benjamin899 Posted at: 2019-06-27T20:20:21.650Z Reads: 74

```
they have not been released yet. He will announce once the 21700 version is available for sale. mainly the tabs are the issue.
```

---
## \#1107 Posted by: cubed Posted at: 2019-06-27T20:31:57.520Z Reads: 73

```
Gotcha thanks for the update :)
```

---
## \#1108 Posted by: Benjamin899 Posted at: 2019-06-27T20:49:42.499Z Reads: 79

```
https://www.electric-skateboard.builders/t/nese-the-no-solder-18650-battery-system/92517/123
 he made a new thread, since this thread is not the one he started.
```

---
## \#1109 Posted by: mishrasubhransu Posted at: 2019-06-27T21:49:13.023Z Reads: 75

```
This one is more active these days. You'll have your questions answered faster.
https://forum./t/nese-the-no-solder-18650-battery-system/1777?u=mishrasubhransu
```

---
