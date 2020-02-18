# Battery work + other related quetsions

### Replies: 27 Views: 2128

## \#1 Posted by: seantjaeger Posted at: 2017-01-31T20:49:21.584Z Reads: 133

```
Hey guys, id like to get some thoughts on a few things:

First off, I just popped open my old hover board and took out the battery. Do you think this could be any help towards a build? Or perhaps combining this with a Lipo/other batteries?

<img src="/uploads/db1493/original/3X/3/e/3ef9b285e563fdb38f24873396487714031de191.jpg" width="375" height="500">

I'm hoping it will, because this will save me some money.Any input on that would help a ton.

If that would not work, as of right now I'm thinking of doing a 9s build (3 11.1v lipos) with 55000 mAh and 35c discharge. Would this be overkill being that it would give around 190A? Unless I did the math wrong, which is a big possibility :joy:. Would I be ok with going for 20c lipos instead?

Just in case you haven't read my other post, I only weigh about 115 and I'm planning on using a 190kV motor to achieve relatively high speeds.

Thanks
-Sean
```

---
## \#2 Posted by: Okami Posted at: 2017-02-01T20:53:48.660Z Reads: 91

```
From volts and capacity looks good! Though- you should check what cells are inside!

This would determine how hard you could push your board.. or how powerful it would be..
```

---
## \#3 Posted by: seantjaeger Posted at: 2017-02-01T21:01:12.325Z Reads: 89

```
Well that's music to my ears!

If I were to open it to check the cells, how should I repackage it back into one piece? Also, what should the cells look like/say? I know of 18650s and some small things about them but not how much power and all that.

Thanks
-Sean
```

---
## \#4 Posted by: Okami Posted at: 2017-02-01T21:09:19.320Z Reads: 85

```
You should probably carefully cut a ''line'' into the packaging.. but before you cut it.. you should check in what formation the cells are layed out... there's probably 2 rows of them, tip to tip..

Then (if you are lucky) on the side there should be some markings to figure this out..

---

2nd method - try to search on the net what batterys hover boards have.. perhaps there are others who have the same battery as you and who have torn it open before you! Would avoid the manual work and cutting the plastic (heatshrink) cover!

---

3rd method.. dont cut it or.. check what cells.. just hook it up to a motor or a load.. and try to figure how many amps it can give out..
```

---
## \#5 Posted by: seantjaeger Posted at: 2017-02-01T21:10:01.924Z Reads: 84

```
Alright - went for it, opened it off of a video:
They don't look bad, that's a start

<img src="/uploads/db1493/original/3X/3/9/39f030e346a82fef1dd520b65efcdb28409313de.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/e/7/e7fd2a5578e9d07350bad12da634e69b9f359005.jpg" width="375" height="500">

Any thoughts? I looked them up and it does seem like people actually use them so they could be okay.

Please let me know ASAP as this will be the green or red light for ordering parts!

Thanks
```

---
## \#6 Posted by: seantjaeger Posted at: 2017-02-01T21:11:09.946Z Reads: 83

```
Wow you responded as I did, haha. I hope I can re cover it if needed!

**EDIT**

<img src="/uploads/db1493/original/3X/2/1/216f50a627957f4019ec2b4210712462a3fca9a8.jpg" width="375" height="500">

This is also on it. Looks like a BMS of some sort. I'm new so not positive, but you tell me.
```

---
## \#7 Posted by: seantjaeger Posted at: 2017-02-01T21:29:46.040Z Reads: 85

```
Alright I'm sorry for the spam, but I just keep finding things out.

Apparently they may have around 2100-2200mAh and around 10A discharge, would this be ok? Or maybe could I use these along with a lipo or something similar to reach the power levels id need?
```

---
## \#8 Posted by: Okami Posted at: 2017-02-01T21:58:52.749Z Reads: 81

```
[quote="Okami, post:4, topic:16993"]
you
[/quote]

oh yeah.. the bms might be a problem.. sorry for the 30min off reply.. had things to do..

Well, for ''light cruising'' 20A might be enough.. usually ppl here advertise / suggest sticking to 60A capable cells.. but so far, it seems it should be okay for not very heavy use.. typically longboard might need max 500-800watts of power anyways.. if you multiply rougly your 36v pack x 20A = 720w.. Should suffice for the startup / acceleration..

If you board would lack power.. u could always ''downgrade'' a gearing a bit.. make it easier for the batteries / motor / controller.. so it reaches less speed.. but perhaps takes less load on the batteries..

--

As of this far.. i hope i have not written crap haha.. if so.. some other ppl should step in.. built only one board so far and reads tons of info.. so i might still be wrong from practical side of things..

---

As for the cells - if they are genuine LG cells.. I think you should be ok :) would be perhaps a bit bad.. if they were some knock-off / no brand cells.. where you couldnt get any info.. wouldnt be any datasheets.. or their performance would have been dubious..

--

Again about Bms part - there should be some way on how to test / figure out what its max amperage (power) rating is.. there might be a thing / possibility, that the bms wont allow full power from the cells and thus will limit the power available.. or perhaps even shut down a bit.. have not dealt with bms a lot..so not gonna be the best expert in this field.. 

Though if bms turns out to be a problem at later stage.. you could disconnect it / cut it off.. and ride without it.. or install a different bms..(though then you would work out the charging thing from zero, I assume)..

---

As for other notes.. I think if you can get decent power (at least you should get some).. then your other problem might only be to fit the battery with its size onto the deck.. check out how big it is and what deck would be suitable.. u will also need some sort of enclosure for it probably

--

Ending here.. some others to step in are welcome.. just thought to give my ''quick'' reply to not make you wait haha.. hope it helps.

--

**About mixing / adding more cells in ''parallel''**

In general.. ppl dont advise doing so.. the best scenario (if you pack is not used much also).. would be to perhaps find similar cells (in terms of max discharge and capacity).. then add those in parallel..

This would boost your capacity (range) and also the discharge capability (power)

---

It might not be that great to mix lipo and li-ion (the ones you have).. because they have a bit ''different'' parameters between each other.. for example - lipos shouldnt be discharged as low / as much as li-ions can.. so if you would do it all.. u would have to monitor the cells / voltages, so that they dont get depleted too much!.. Plus, there is also this unknown factor on how your bms would act if there was another battery connected to your existing one..

I've ridden 2x 3s lipo's at 2.2ah capacity and 20c discharge I believe.. in theory, they should have given me about 40A discharge.. as far as I remember I could ride my board just fine.. perhaps it was a bit more ''smoother'', not so quick.. but I still could maintain decent speed.. Plus, I got a mountainboard (heavy + big tires).. which usually consumes about 5-20A on flats (24v) and about 40-55A peak.. which might as well be for a few seconds or even less..

So with you and a longboard.. and not much hills.. for the sake of using what you already have I think you should try it.. if you run into some sort of problems.. like cells draining too fast or anything.. u could always consider other options later, once you would have built your system.. just plan ahead and decide how to make it ''adaptable'' so that you can switch out a battery or add some more.. if you later need it..
```

---
## \#9 Posted by: seantjaeger Posted at: 2017-02-01T22:16:02.379Z Reads: 66

```
Thanks for telling me all that. I'm not very into the whole battery part, so I still don't know too much, but I understand what you mean.

So basically what you are saying is: give it a shot and see how things go?

Is there any way I could tet them and see if they truly are legit and not just look legit but are labeled fake? Or is it just trusting the gut here?

Also, if this were not to work well and I decide to switch to lipos, do you know if I could use lipos with different discharge rates but the same mAh and still get good results? Because that was my alternative choice.

Oh and don't worry about the wait, my mind is just racing so I'm being impatient :joy:

Thanks
-Sean
```

---
## \#10 Posted by: Okami Posted at: 2017-02-01T22:21:45.089Z Reads: 68

```
emm from what I believe.. if you get the same ''efficiency'' as others have.. **then you should be able to ride about 15km or about 11miles I believe**.. This is taken from '**'WH''** rating of your batteries..

Generally, it is said / believed, that 10 WH is consumed per km. (10wh/km).. so I ''downgraded'' a bit your battery.. and you should be able to travel the said distance.. 

But **that is only if you dont push the batteries at max**.. there should be this ''discharge chart'' on the internet.. which shows what capacity you get out of your batteries, at what discharge rate (amperes)..

---

_Wont be able to tell about the ''legit-ness'' part.. should probably look on the net.._ - have others tried to test it or not.. I believe, if the cells (batteries) perform as advertised.. then they should be ''legit'' / original..

--

**Testing**

To really test them - **should find a load / ''source'' of power/device, that needs a lot of ampers..**

im not entirely sure can you easly get 10A load for 36v.. that would be already 360W..

**The easiest ppl have done / are doing..** to discharge their batteries:

Buy a dozen / couple of **12V car headlight lamps (bulbs)**. 

String them together (12v x 3).. then add in parallel about 4 bulbs.. though, you would make a very powerful ''lantern'' / stadium light out of this haha.. but this setup should draw about ~50w x 12 = 600w

You will also need to have an **''amp meter'' or just a regular ''multi-meter''..** these are cheap.. some cost around 10usd more or less.. Though, the multi meters are usually rater for only 10A.. So you would have difficulty measuring over 300W.. otherwise they get blown.. have not happened to me, but there's usually a warning that there is no fuse for 10A setting..

--

I hope my ''headlight bulb'' math is correct.. I still need to check, whenever each bulb adds to the total ''watts'' or only the parallel ones.. otherwise you would need not 12bulbs but perhaps even 36x.. which would be a bit crazy and hard to wire all of them together haha..

Try to find some cheap bulbs.. where im living in some packages there are bulbs for about 2.50 usd a piece.., so if you had to get 12bulbs.. that would still cost you like 25usd or so.. just to ''test'' your batteries..

--

U can try to search on net.. perhaps.. ''500w load for 36v batteries'' or something like that.. if your dad is crafty.. perhaps ask him does he have any ideas.. for devices which consume 36v and a lot of watts / amps..

--

Last idea - you could try to test just one cell or a group of them, if you can ''connect to the wiring of just a few cells''.. Im not sure how your bms would like this.. but you would later need to charge up your batteries (the ones you drained) individually.. from the rest of the pack..

This way you wouldnt need so many bulbs.. but you would need to check that the wires you attach the bulbs to.. are fat enough (so they dont get hot/start to melt or something..)

--

**If you got money - might as well go with lipos straight away.**. will have more power / less ''drag'' (strain - pressure) on the batteries.. as lipos perform a lot better in terms of watts/amps/power they can deliver, compared to li-ions.

Though.. they seem to be a bit less ''stable'' will require seperate charger or bms circuit to charge them.. 

Also ppl report that they get ''worn out'' faster.. though some still discuss whenever this is true or not.. as that also depends on how hard / often do you use them and other factors..

----

If you go the ''lipo'' route.. you could always connect (if you have space) this Li-ion battery pack as ''reserve'' battery.. to just get home or something.. or.. make it a ''portable battery charger'' and just carry it with you to charge a bit of your batteries, when you run down your main pack / main batteries on the board..
```

---
## \#11 Posted by: sl33py Posted at: 2017-02-01T22:38:16.520Z Reads: 61

```
Some great info and suggestions from @Okami.

I would definitely try the battery out, but i would not mix this pack and others.

A claimed 10A per cell = 20A in 2p.  That's pretty small even for 115lbs.  You will get less range the more you overdraw the cells and besides short runtime - you can damage the cells themselves.

Do you have the charging circuit out of the hoverboard to charge this pack?  It's important to balance charge so you don't over charge a cell if it's out of balance and have a bigger issue (like fire).

Not to be doom/gloom here, but just be careful if you are set on using this pack.  Don't mix would be my biggest suggestion.

I would still suggest getting a set of Lipos for 6/8/9/10s however you want to configure it.

GL!
```

---
## \#12 Posted by: Okami Posted at: 2017-02-01T23:01:00.849Z Reads: 58

```
Actually I just found out it is written on the pack'' 22p-001H..

Im not sure though, why on the cells there are the marking for LG..

Even though, 22P stands for samsng 22p cells usually..

Anyways.. I hope you still can ''tape back'' the plastic sheet/cover your batteries had.. and at least now we know what is written on the cells.. and not what the label says.. 

--

I tried to look up how to find counterfeits.. it seems it might be really hard in some cases, here it is for a different cell:

https://batterybro.com/blogs/18650-wholesale-battery-reviews/104619270-can-you-identify-the-fake-lg-hg2-18650-battery

I've heard that ppl have tried to weight the cells etc.. but this will be really hard and unneeded in your case, I think, as you cannot really remove the cells.. plus you wont probably have much to compare them to..

Non the less, if they are really samsung 22p ''analogue'' cells. it looks quite promising:

http://lygte-info.dk/review/batteries2012/Samsung%20ICR18650-22P%202200mAh%20(Blue)%20UK.html

For these even at 10A they keep up about 2050 mah or so.. so over 2ah..

So you shouldnt loose much capacity.. and should expect these 11miles/15km probably (36vx4 =144wh)

So about 10miles/14km.. (theoretical)
```

---
## \#13 Posted by: seantjaeger Posted at: 2017-02-01T23:06:07.197Z Reads: 59

```
Yeah that was my biggest worry. I know that the batteries could be fake, and if they are then that will be bad.

I guess I'm gonna go back to the lipos just in case. I don't wanna finish it all and then have my whole build blow up in my face (literally).

I'm gonna look at some more lipos tonight, hopefully order all parts and get building. 

Sorry if I wasted your time with all the other battery stuff, I'm just trying to find some ways to save money :joy:. If spending some more will be worth it then I don't mind doing it, though.

Thanks for all your help, I think I'm starting to understand this whole battery thing now.
-Sean
```

---
## \#14 Posted by: Okami Posted at: 2017-02-01T23:08:46.553Z Reads: 56

```
I can lastly give you some battery info sources..

http://www.rchelicopterfun.com/rc-lipo-batteries.html

This was a good one!

Then there''s also:

www.batteryuniversity.com

--

I believe you are familiar with C rates / capacity / parallel / series thing.. but non the less.. these sites i gave have some background info about all of that..

--

No worries.. at least I somewhat ''compiled'' a lot of battery info.. perhaps some other users will benefit from it later.. it's still sad nobody has really tried (or it's not widely popularized) low discharge batteries.. With the recent info about not having problems discharging batteries at high rate.. it seems someone should give this a green light..

One u get your setup complete / running.. would be nice, if you had XT60 plug/connector for your esc (or vesc).. so that you could still try how this hoverboard battery works!... Or just connect an adapter/converter cable, if the esc will have a different connector!

Ok wish you luck with building then! I hope this was somewhat educative / informative for you to read haha.. been using li-ions for awhile.. had low capacity lipos for short while but they did not fulfill my needs as an backup battery as I could only do 1-2km with them.. were pretty useless to keep them on board :)
```

---
## \#15 Posted by: seantjaeger Posted at: 2017-02-01T23:11:48.733Z Reads: 49

```
I think I'm gonna stick with your original suggestions and go the lipo route, just for safety reasons.

So the setup I listed before, would it be okay?
(Right below this)

2x 35c 3s 5500mAh
1x 20c 3s 5500mAh

Or, would this way be better/the same? If it is worse, is it really worth spending the extra for the 1st setup? (Noticable difference or small)

2x 20c 3s 5500mAh
1x 35c 3s 5500mAh

Once you tell me which is really worth it than I think it's about time to start emptying my wallet!

Really excited to do this now, thank you. 
-Sean
```

---
## \#16 Posted by: seantjaeger Posted at: 2017-02-01T23:15:16.595Z Reads: 46

```
Welp, that pretty much might clear up most of the questions I've asked @sl33py like as you sent that post through lol.

That looks like a good resource, I'll read through it.

And yeah you're right, that would be a huge benefit for everyone. Also I know it'll definitely help people in my situation by looking at this, seems like most of the battery posts are more skilled builds/builders.

I will try the hover board battery once I learn more, and I'll let you know!

Thanks for the help
-Sean
```

---
## \#17 Posted by: Okami Posted at: 2017-02-01T23:19:23.136Z Reads: 44

```
Ok, quick feedback - is it possible for you not to mix ''C ratings''?

I think it is generally not recommended.. as the cells still could discharge at different rates.. u would have to monitor them an extra more.. or use some sort of extra bms / cut-off protection not to over-discharge then,, (or just regularly check whenever they stay at the same level / balance in general..)

Generally ppl suggest to stick with 25c or so.. but I think you might be okay with 20C and 5.5ah..

at 10c it should give you 55amps.. which is close to the recommended.. some will probably argue again.. etc but then they can tell their experience, if they have some facts / statements to make..

Also - usually it is suggested to ''de-rate'' the c rate.. as u have probably read already.. so 10c should be a somewhat safe measure.. perhaps 12-14c is the max expected.. that you should be able to pull from these..

It has been stated that these C rates.. are what manufacturers have deemed ''safe'' to discharge.. but it does not mean that it is not close to the max.. or that it might get a bit bad
```

---
## \#18 Posted by: seantjaeger Posted at: 2017-02-01T23:29:42.675Z Reads: 39

```
Hmm, I could try but only with lower discharge rates (20-25) only because they start to get kinda pricey over that. Like I said if I really need to I'll do it, but if it's possible than using the seperate rates would just be easier in my case. Reason being I have a 5500 35c from an airsoft gun I built a few months back. So I'd think 3x 35c would be kinda high. 

20-25c on the other hand I can find for relatively cheap, so that would be easier to get 3 of.

Hey I mean you're the experienced one so you tell me and I'll try and go for that route.

Thanks for the considerations.
-Sean
```

---
## \#19 Posted by: Okami Posted at: 2017-02-01T23:32:58.898Z Reads: 43

```
mh it is still info what ive read from others.. so Im a bit unsure on approving anything here haha.. (especially LiPos when used on eboards).. just can give you some last tips.. such as that it does not seem to make much difference in the ''punch'' / acceleration / power if you go over 45c..

And as you probably already know.. then for bigger capacity battery's the discharge rate (c rate) can be lower.. as the total amps given will increase anyways.. (Ah x C)

--

You could mix them.. but it really depends.. might be a bit worse / especially bad, if yo dont have the same make / model / brand battery as the ones you plan to order.. there might be some tweaks/differences and as said - this would lead to some sort of inbalance.. especially, cuz you would run in serial.. in parallel cells might balance each other out, if they get out of balance.. but in series they wont (at least as far as I know :D )

So stick with 20-25c if you can.. perhaps these 25c does not make that much different..

+ get all the right connectors and charger.. 50W charger might take you about 3hours 20mins (at max charge rate, deeply depleted pack) to charge them +.. you will have to seperate the cells... standard balance chargers take p only 6cells in serial.. you would need to charge 6first.. then 3 after that.. (unless you make ''parallel''charging connection..so that you can charge all of them at once.. as 3s 5.5ah x 3 pack.. (3s 16.5ah pack )

--

This might be the ''other side of the coin'' - if you go with your already owned hover board pack.. no seperate / extra charger might be needed.. 

If you go with lipo, you will need either a bms (soldered by yourself) or a smart charger (balance charger), which does the balancing for you..

--

if you are really brave, u could hook up some bms .. it might help with not running the cells down.. but this will be extra cost again.. i think you would be better off just getting 3x exactly same batteries.. rather than to fiddle with 1 different one and a monitoring circuit to not overdischarge the 2 other ones .. [complicated stuff]

Ok im somewhat over here.. **try to look up whenever ppl ran different c rate batteries.. got no experience here.. and neither have lipos at such high capacity / amps / configuration to tell how all of this works in practice..**
```

---
## \#20 Posted by: seantjaeger Posted at: 2017-02-01T23:50:07.731Z Reads: 36

```
Ah ok thank you. Maybe I will look into a bms at some point for all that. As for the lipos themselves, I'll look for 3 20-25c ones. Thank you for clearing that up.

I'll go do some more research now.

Thanks
-Sean
```

---
## \#21 Posted by: Okami Posted at: 2017-02-01T23:53:47.889Z Reads: 30

```
If it does not change much for you (in terms of tax or shipping cost..) just might as well try that hoverboard battery! if it works decently.. and doesnt give out only 10A.. you might be able to still ride it quite okay... just my little opinion :D sorry for not trying a low discharge battery..

 some ppl like @Ackmaniac **should be able to tell how it is to ride on only 20A of power (at 10s li ion)..**
```

---
## \#22 Posted by: seantjaeger Posted at: 2017-02-02T00:07:29.012Z Reads: 33

```
I would love to try, but I'm just too afraid to after all the fires and such with them, and that was even when drawing less of a current. when I figure out if they are legitimate or not then that will be the 1st thing i'll do!

I found a few lipos, could you give me your opinion?

https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html

https://hobbyking.com/en_us/turnigy-5000mah-3s-25c-lipo-pack.html

Or I found another with the same, but 25c discharge. Would you say those would all be basically the same?

Thanks
-Sean
```

---
## \#23 Posted by: Okami Posted at: 2017-02-02T00:16:52.533Z Reads: 35

```
Looks good to me for ''starter'' setup..

Im not sure whenever there is a big difference between turnigy and zippy.. both seem adequate.. and somewhat respected in the rc hobby community.. 

if youre in doubt check on google what RC hobby ppl say about turnigy and what abot zippy's..

Turnigy's seem to be quite a bit cheaper.. will probably save about 15usd in the end. if you choose turnigy's it seems..

--

Sorry about forgetting about the hoverboard fires! That has really fallen out of my head haha.. I think it usally happened with non-genuine cells.. with these I believe all sorts of things can go wrong lol.. especially if the circuit / protection on the board itself is not the greatest.. should look it up one day.. what really has caused all of these fires for them!

--

I think just get 3 of them the same.. dont cheap out with 20usd extra usd.. at least you will know that all of these have come from about the same time/specs.. and shouldnt differ that much between each other
```

---
## \#24 Posted by: seantjaeger Posted at: 2017-02-02T00:22:32.906Z Reads: 34

```
Alright, perfect thanks. I'll probably go with the Turnigy ones, just because I have also heard good things about them.

As for the fires, I believe it was due to the way they were put together. Some were soldered wrong and others literally had broken cells just in the packs!

Either way- just glad mine didn't go on fire.

Thanks
-Sean
```

---
## \#25 Posted by: Okami Posted at: 2017-02-02T00:25:33.213Z Reads: 32

```
yep, stick with turnigy's.. at that price it is quite a good deal.. should get enough range anyways.. have you decided on what esc / motor speed controller to get?

I think with 9s.. you dont have that many options now ha
```

---
## \#26 Posted by: seantjaeger Posted at: 2017-02-02T17:58:34.394Z Reads: 27

```
Sorry for the late response, been busy with school and such.

I'm gonna go with a VESC and a 190kv motor from DIYeSkate. Seems like decent prices, and I've heard good things.
```

---
## \#27 Posted by: ramon Posted at: 2018-01-07T16:56:05.879Z Reads: 17

```
That BMS is 10S right? I'm gonna buy a 30$ broken hoverboard in order to salvage its parts and that one of the main components I'm looking for.
```

---
