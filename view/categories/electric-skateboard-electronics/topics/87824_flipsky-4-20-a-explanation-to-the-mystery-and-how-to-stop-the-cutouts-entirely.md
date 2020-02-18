# FLIPSKY 4.20, A Explanation to the mystery, and how to stop the cutouts entirely!

### Replies: 239 Views: 7538

## \#1 Posted by: Schtekarsten Posted at: 2019-03-21T09:04:06.084Z Reads: 699

```
Hello good folks of this forum, first post here. kinda nervous :smiley: 
Moi and my good friend Gamer43 #thebrain have an explanation to the cutouts and how to fix it. 
Long long long story short, swap the gate resistors and you wont have the cutout issues anymore.

The reason behind the cutouts of the 4.20 based vesc controllers are something called slew rate (Gamer43 will do a better explanation of that then I ever can, so wait for that if interested), basically when you you pull a shit ton of Amps and do so fast the DRV ship says see ya and cuts out. Sounds familiar... well that Is probable why you threw it in the fuck it bucket at the first place. hopefully you are to lazy to empty the fuck it bucket in the garbage and can still bring it back to life. because it is really quit f***** good when the cutouts are gone, and it can handle continues load surprisingly well, like really well!!!
And to combat that you can change the gate resistor or the mosfets used. The cheapest and simplest solution for us garage folks is to change the gate resistors. Change all the 4.7 ohms resistors of the 4.20 plus to 22ohms and on the other 4.20 based versions to 47ohm. (again we will do a video and explain that better down in. y later on...) The 4.20 plus uses "better" mosfets that's why you need a lower value.
Basically we have done maybe 50 hours trying to disprove our theory by messing around with settings and different hardware but yeah cutouts that wont happened even if you decide to strap the vesc to a truck and turn it's wheels. (well I lied, we have not tried that but you get the point)
Well as far as we got before i ran to mamma crying. Was with a 12s4p setup, dual 6374, sensored/hybrid foc, 80a motor max, 60a battery max on each side. doing so at the steepest hill I could find in the area and started from a standstill. And the only rule was: hit the throttle to max as fast as you could possibly could until you went flying up the hill, or the board cutout, or you went tree hugging.  

Apart from that we have done, y anything imaginable to have the vesc cut out but nop, not a single cutout as long as you don't lower the resistor value, and if you do so just a tiny bit it will cut out instantly with just slightly aggressive settings and throttle movement. Yes even the plus version cuts out real easy. (the 6.6 Vesc's actually has the same issue with cutout but that is at like 80A (alot higher), so you kind of need to strap that to a truck to have it cutout, and very few people do that and we believe that's why people are not posting and crying about flying into a bush on the 6.6 vescs because of cutouts.)

Oh and I would go as far as to say, stay away from the plus versions their anti-sparks are not the most reliable in the world...

Damn I wanted to keep this short but I guess I messed up... :smiley:
Oh and Gamer43 is really the one you should applaud for this. he is the brain and beauty behind all this. :v:


Flipsky are now shipping all their 4.20 based Vesc's with the newer resistors. They just have not had time to update their website as they are in the middle of moving their entire factory.
Have seen and gotten a few questions regarding it so I thought I might post it here. 

If you want to go ahead and make the resistor swap yourself, I have 2-3 posts below and a video covering everything you need to know.
```

---
## \#2 Posted by: Gamer43 Posted at: 2019-03-21T09:12:35.594Z Reads: 616

```
Here is a photo of the resistors in question:
![image|375x500](upload://9vvZmFCYar9GToqkpieoPMy7kIx.jpeg) 

TL:DR, the resistors circled in red need to be replaced with 47 ohm resistors (22 ohm on the plus versions). The result is no more cutouts, even on the settings Schtekarsten mentioned above.
The resistors' original value is 4.7ohm, no other resistors on the VESC 4 has that value.

Basically what was happening was that since the NTMFS5C628NL MOSFET has about 6.5 nC of Miller (gate-drain) charge, this resulted in very high frequency ringing on the switch nodes. Long story short, it caused the DRV8302 to glitch and throw a fault. This would occur when current would change very quickly, so the ringing most likely triggered the VDS monitor on the DRV8302.

I first suspected this was the case when I was lurking on the TI forums, someone reported spurious fault reporting by the DRV8302, and the solutions were about proper routing of PCB gate drive and ground traces.

Will this negatively affect switching losses? Yes. But by my calculations, when switching losses are equal to 2W, conduction losses are equal to 18W, so the effect is negligible, (meaning at the point where temperature becomes a problem, the size of resistors doesn't really matter).
In Fact, the switching losses are still BETTER than 4.12 hardware versions.
(The 4.12 uses the IRFS7530, which has an onerous 70nC of Miller charge)

Also, I really only gave Schtekarsten some ideas, his rework and testing is what allowed us to find a solution to this issue.
```

---
## \#3 Posted by: DeathCookies Posted at: 2019-03-21T09:15:53.794Z Reads: 577

```
Great work of you two! I am excited to see the feedback of the users :)
```

---
## \#4 Posted by: Schtekarsten Posted at: 2019-03-21T09:19:17.625Z Reads: 575

```
Hey thanks, we plan on getting some videos going on how to do the resistor swap your selves.
```

---
## \#5 Posted by: ervinelin Posted at: 2019-03-21T09:24:45.974Z Reads: 572

```
Wow.. just wow... much respect!!

Now if only my hands were steady enough to fix this....

By the way why is it that different firmwares seem to suffer these cutouts differently if it's a hardware issue? Vesctool 0.94 and the latest 1.05 were good for me, 0.95 (which was what came with my dual 4.2 non-pro) would spaz out above 30A.
```

---
## \#6 Posted by: Gamer43 Posted at: 2019-03-21T09:26:29.127Z Reads: 547

```
[quote="ervinelin, post:5, topic:87824"]
By the way why is it that different firmwares seem to suffer these cutouts differently if it’s a hardware issue? Vesctool 0.94 and the latest 1.05 were good for me, 0.95 (which was what came with my dual 4.2 non-pro) would spaz out above 30A.
[/quote]

I think Vedder changed the way the current filter works between those firmwares, and it's the rapid change in currents that would trigger the faults.
```

---
## \#7 Posted by: ervinelin Posted at: 2019-03-21T09:55:40.783Z Reads: 510

```
Sorry if it's a wee bit off topic.. but do you also know why the voltage readout for the flipskys are not stable? I run telemetry to see my decks voltage but for flipsky escs they have so much jitter in the readout.
```

---
## \#8 Posted by: pat.speed Posted at: 2019-03-21T10:03:10.957Z Reads: 496

```
Definitely following this thread, I've been wanting one of these for a while but the cut-outs put me off. Now you are making me spend money...damn it
```

---
## \#9 Posted by: Schtekarsten Posted at: 2019-03-21T10:51:21.411Z Reads: 505

```
For those eager to get going with the resistor swap, i'l just put together a short writeup before i do a more in-depth video thingy:
For the dual 4.20 PLUS vesc's get the 22 ohms resistors in a 603 package
For all the regular dual 4.20 and the 4.20 single vesc's get the 47ohms resistors in the 603 package
Get that stuff from arrow FREE WORLDWIDE shipping ( like 1-2 days to Sweden, click around on the shipping options when at check-out Fedex is the quickest for me)
For the dual 4.20 plus get the: https://www.arrow.com/en/products/rc0603fr-0722rl/yageo
For all the dual 4.20 and the 4.20 single get the: https://www.arrow.com/en/products/rc0603fr-0747rl/yageo

You need 12 of them for a dual and 6 for a single, but F it get like 50 of them they are not even pennies... and you will most likely lose half of them. :smiley:

You need a ton of flux, get the no clean stuff or have fun cleaning afterwards, some normal lead solder, a good iron with a small tip and preferably a large one too. ((and no if the tip is black and crusty toss it!) I happen to like the "ts100" with the TS-D24 and TS-C4 tips with a Mean Well LRS-100-24 power supply and 20awg cable, might get more into that if interested.) Some solder wick, a pokeee thing or some fine tweezers.

Start by desoldering every resistor with the 4R7ohms mark you can find (se Gamers43 picture above). Use the fat tip and a big blood off solder on the iron. The ones in a tight spots use the small tip to desolder. A big goop of flux on the resistors might help.
Use solder wick to get rid of the disgusting lead-free solder on the pads.
Squirt out a big glob of flux on the pads and tin the pads with solder. (I have had better luck with tinning both pads before adding the resistors)
Carve off some of the plastic on some of the JST connectors to make room for the iron. (you will know what I mean when you get into it)
Flux on, heat up the easiest of the two pads and push the resistor into the iron and the iron will kind of move about the resistor. When positioned correctly, stab the resistor with the pokee thing to hold it down on the pad and remove the iron.
Try to lightly poke on the resistor to se if it stuck down well enough.
place the iron on the other pad and reflow the solder.
Important! in order to make sure the resistor has positive contact with the pad try heat up one of the sides/pads with the iron and push it off and then do the same with the other side. If it is still stuck down then that's all good! Celebrate with a beer or two and jump to the next resistor.
When done with all the resistors double check that they are all on correctly by poking each resistor with a iron on each end of the resistors. 
Remember flux is king! if the joints are grey and dull more, flux my friend get them joints shiny!
Clean off the flux with some alcohol if you want to make it look a bit nicer.

ugh shit that got long... a video will be coming in a day or so, grab the resistors from arrow in the meantime and the video will hopefully up by then. (btw I am by no means an expert on this and there are probably better ways to do this with hot air and all that, but I have swapped about a hundred of these little buggers and done so successfully.)
```

---
## \#10 Posted by: Schtekarsten Posted at: 2019-03-21T10:57:19.288Z Reads: 430

```
No worries, both my BT-modules have gotten a sip of the Swedish salty roads so I have not been able able to se if it has to do with this or not, got some new ones on the way though so I will let you know if that is the case or not.
but if I remember correctly I don't think I have ever had that issue. idk
```

---
## \#11 Posted by: pat.speed Posted at: 2019-03-21T11:08:36.537Z Reads: 437

```
[quote="Schtekarsten, post:9, topic:87824"]
Celebrate with a beer or two and jump to the next 
[/quote]

Well, by the time we get to the 12th one the solder job is gonna be pretty darn sloppy lol
```

---
## \#12 Posted by: riverside.rider Posted at: 2019-03-21T11:33:24.665Z Reads: 433

```
yes, same here, would love to know why the voltage seems to be rather unstable with the Flippies....any ideas @Schtekarsten? great work on the write up :slight_smile:
```

---
## \#13 Posted by: Rzkyyy Posted at: 2019-03-21T11:43:06.961Z Reads: 421

```
Would you guys just please sell me the modified version of dual fsesc 4.20. I'm more than happy to be your guinea pig 🤘
```

---
## \#14 Posted by: High-roller Posted at: 2019-03-21T12:21:56.347Z Reads: 412

```
Thanks again for posting this! I'm not confident enough in my own soldering skills- or my budget- to try this so hats off to you for taking the risk and experimenting and sharing the knowledge.
You might want to get a bunch of these to modify and sell before flipsky finds out. :wink:

[quote="Schtekarsten, post:1, topic:87824"]
threw it in the fuck it bucket
[/quote]

Well, that's a new one to add to the lexicon.
```

---
## \#15 Posted by: Riako Posted at: 2019-03-21T13:51:31.405Z Reads: 395

```
Thanks a lot to both of you :D :+1: !!
```

---
## \#16 Posted by: Hummie Posted at: 2019-03-21T15:52:40.631Z Reads: 400

```
Did u tell flipsky? Assuming it stops the cutouts the info is golden.   I’ll link @BarbaraZ and email here
Wow. Nice job!   Just moved the world two steps closer to cheapness and reliability. Probably saved like ten peoples’ face
```

---
## \#17 Posted by: Fiori Posted at: 2019-03-21T16:02:52.986Z Reads: 399

```
Thanks for all the hard work and research fellas. This is awesome. This is why i love this place.
```

---
## \#18 Posted by: 808Chopz Posted at: 2019-03-21T16:49:29.536Z Reads: 397

```
Wow! that's Awesome news! Can't wait video tutorial how to? I want to save my ugly face :joy::joy:
```

---
## \#19 Posted by: Gamer43 Posted at: 2019-03-21T17:56:19.338Z Reads: 392

```
We've contacted Flipsky, they haven't given us a timeline on making the change though :-/.

I also would like to add that the "proper" solution would've been RC snubbers on the switch nodes, but idk why, no one making these things seems to give a damn about transient suppression >:(.
```

---
## \#20 Posted by: Schtekarsten Posted at: 2019-03-21T18:50:52.295Z Reads: 397

```
You people are to kind :heart_eyes:
To be honest I have no idea why the voltage is jittery and unstable on the 4.20 units. Im too dumb to figure that out, but I did just receive three bt-modules from ray8801 so can do some testing and see if it is still there or not. I also plan on doing the soldering thingee sometime tomorrow and them post the video, just need to figure out how to edit first though :D 
I have been successful on both the dual 4.20 and the dual 4.20 plus version with the resistor swap and I have been running the modified plus version for like two weeks without any issues. (and no I dont ride like a granny, the non-modified 4.20 plus cuts out every single time I go from a standstill more or less :v::dancer:)
Even though I dont like the anti-spark design on the 4.20 plus, and moi and my friend would not recommend it, I am running It anyways cus im lazy and like to not get my fingers dirty pushing the on/off button, and it was the last vesc I did my testing on and I could not be bothered swapping back.

Back to my point: The 4.20 plus uses a different set of mosfets that are more efficient and in theory would increase the continues amps from something like a 45A per side (on the old NTMFS5C628NL mosfets) to 55-60A (for the new NTMFS5C612N mosfets). For Flipsky it would result in a cost increase of like 8 dollars per dual vesc by using the "better" 612 mosfets.
What do you guys think would it be worth the cost increase to get some better mosfets going, should we kindly ask flipsky as a community to use the more expensive mosfets?
I for one is just gobsmacked about the performance of the modified 4.20 plus vesc, the board goes like a hot damn and the Swedish winter does not want to let the vesc temperature throttle (well I have ridden it without telemetry up until now, so who the fuck knows really). But I guess the anti-spark might take that away from me sooner or later :smile::rofl:

We do have a solution for the damn anti-spark to though, but we are not too sure if we want to give them that yet I mean, they are not open source and we have not even heard from them for like a week or so when gave them the answer to the cutouts. And fuck me, now we are basically promoting their products. :joy::crazy_face::sleeping:
```

---
## \#21 Posted by: Schtekarsten Posted at: 2019-03-21T18:53:18.979Z Reads: 347

```
Sorry it is too time consuming I am about to go to my brother and try out 31 pairs of climbing shoes :kissing_heart:
```

---
## \#22 Posted by: Okami Posted at: 2019-03-21T19:52:13.948Z Reads: 357

```
This does sound like really good news, as I was recently disapppointed about how they released plus version when i didnt even got the chance to use regular flipsky 4.2 dual (due to winter and board in rebuild process)

Anyways, i hope to get my hands on hot air station, seems like it will make the job a lot easier as these resistors are really tiny..

So yeh, thumbs up for figuring this out.
 Really nice to know now that it is possible to have flipsky vesc 4.2 without errors over 30A.
```

---
## \#23 Posted by: Schtekarsten Posted at: 2019-03-21T19:59:58.199Z Reads: 348

```
Idk if a hot air station would be easier to use to be honest, all the components are so clustered together and there are lots of plastic an shit that you would have to cover up in in order not burn or blow all away.
```

---
## \#24 Posted by: Okami Posted at: 2019-03-21T20:10:25.212Z Reads: 342

```
Yeh good point. I know they have rather small tips but havent really worked that much with hot air.

 I guess will see once i take a look at pcb on my own
```

---
## \#25 Posted by: rey8801 Posted at: 2019-03-21T20:42:50.062Z Reads: 335

```
Finally man! The work you both made is remarkable. I hope a lot of folks will benefit from it.
```

---
## \#26 Posted by: High-roller Posted at: 2019-03-21T21:23:16.405Z Reads: 337

```
[quote="Schtekarsten, post:20, topic:87824"]
For Flipsky it would result in a cost increase of like 8 dollars per dual vesc by using the “better” 612 mosfets. What do you guys think would it be worth the cost increase to get some better mosfets going, should we kindly ask flipsky as a community to use the more expensive mosfets?
[/quote]

Considering that the 4.20 is currently their cheapest vesc by about 10 dollars (standard one is $85) I don't know why we wouldn't want this if it it improves the reliability this much. As long as they don't raise it by an unreasonable amount and maybe add an explanation of the improvement in the description like they already do there doesn't seem to be much of a downside. Isn't this a perfect example of consumer-driven improvement?
```

---
## \#27 Posted by: Schtekarsten Posted at: 2019-03-21T21:56:21.837Z Reads: 336

```
Y no I certainly don’t hope so, and I mean they only raised the price on the plus version by a tiny bit and that also included a anti-spark module.
Well it won’t help the reliability but it will be running cooler/ be able to run higher powered boards. Well you know what I mean. 
The question though is how where does the line goes how hard can you push it? Will it be sufficient for a street setup, kinda fat dude on a 12s dual 6374 or is it higher or lower? Well it will always be hard to kinda compare real world tests and “this VESC is sufficient for 12s or whatever. There are soo many factors involved. What I think we should do though is apart from the general real world test and get a feeling for what works and how it performs we should create a generalised test where preferably the same person does a continues load testing on a testbench as well as some burst/interval testing. 
Well ideally we would start something like that on motors and maybe even batteries as well.
```

---
## \#28 Posted by: High-roller Posted at: 2019-03-21T22:28:44.470Z Reads: 319

```
Have you tried 10s FOC yet? I think that would be the next logical test. If that works then you can scale it up to 12s.
```

---
## \#29 Posted by: Schtekarsten Posted at: 2019-03-21T22:48:57.647Z Reads: 330

```
Well 12s foc works and should not cutout what so ever no matter how many amps you pull through it.

The next question is how well does it handle continious load/heat before it starts to temperature throttle. We know it should be somewhere between 40-45A for the 628 MOSFETs and 55-60A for the 612. But that is not necessarily the case in the real world with all its factors.

What would be interesting is to test all the Vesc, motors, and battery setups to see how they compare to each other. So we can get a feel for “how” much better or worse they perform. 

I’m I am planing on setting up a basic setup so I can start testing contious load but that will have to wait until like may or so.
```

---
## \#30 Posted by: Schtekarsten Posted at: 2019-03-22T08:26:08.694Z Reads: 313

```
Good new people! 
We just got confirmation that they have implemented the changes on some test samples and will send out to one of their local testers in China.
✌️👌
```

---
## \#31 Posted by: rey8801 Posted at: 2019-03-22T08:32:04.019Z Reads: 313

```
That is great! At least they should send some 4.20 to you, as appreciation for the work you and @Gamer43 did.
```

---
## \#32 Posted by: banjaxxed Posted at: 2019-03-22T08:48:03.982Z Reads: 311

```
They should but China
```

---
## \#33 Posted by: Schtekarsten Posted at: 2019-03-22T09:13:49.913Z Reads: 306

```
Y I know, but moi et my friend don't se any possible issue that will be caused by swapping out the resistors in production, the ideal thing would be if they could sent out some test units first but hey... im not Flipsky. The good thing is that they have started to work on it and hopefully soon be available for the market.
```

---
## \#34 Posted by: Schtekarsten Posted at: 2019-03-22T09:16:58.697Z Reads: 303

```
Thanks a lot. that makes me happy!
Well yeah we will see if they will send out some test units before they change out the whole production or not, but I have already done the swap myself on multiple units and as far as my knowledge and testing goes it should be fine :dancer:
```

---
## \#35 Posted by: BillGordon Posted at: 2019-03-22T10:43:09.196Z Reads: 299

```
This is just too fucking cool. I have a pair of these in my Fuckit Bucket (great phrase), and until I found this thread, did not know what the hell to do with them. I will proceed as you have suggested, and I cannot thank you enough for this insight.

Well done!
```

---
## \#36 Posted by: Schtekarsten Posted at: 2019-03-22T10:53:05.528Z Reads: 292

```
Hey thanks that means alot!
Moi et my friend just received some new insight from Flipsky and that they are in the middle of moving their factory to Dongguan, but implementing and testing the out the changes are high on their priority list. So I think we should give them some slack, but hopefully fairly soon they should come out with the new changes made to their Vesc's
```

---
## \#37 Posted by: Schtekarsten Posted at: 2019-03-22T21:52:42.203Z Reads: 296

```
Ohhhkay people so here is the video regarding the resistor swap.
I don't not know how to edit so it is basically all in one take and it is incredibly crusty so I would advise you to fast forward and all that good stuff in order to get through it whitout falling asleep. 
For sure there are a better ways to do it but this is what has worked for me.
I would recommend to do some research before getting into it: Louis Rossmann on YouTube is a good place to start. Then I would mess around on a dead pcb before jumping on the Vesc itself. 
And please do this at your own risk, but again the Vesc is pretty useless without the resistor swap so🤷🏼‍♀️
Anyways here are the is a link to the video.
https://www.youtube.com/channel/UCCcmmGIrmqg701hivscj4NQ?view_as=subscriber

Might do a cleaner write-up in the future but...
```

---
## \#38 Posted by: Riako Posted at: 2019-03-23T01:20:53.938Z Reads: 293

```
Once again, thanks for sharing! It's awesome, I'm sure your tutorial will help a lot of us !! And surprisingly I wasn't absolutely bored, looking the 17min of video, because learning a lot :stuck_out_tongue_winking_eye: :+1:

Big Up Guys !!!
```

---
## \#39 Posted by: Bobby Posted at: 2019-03-23T01:27:45.152Z Reads: 292

```
Hey @JohnnyMeduse, is this a service you may be able to offer in the future? Upgrading all these flipsky for us rookie solder guys
```

---
## \#40 Posted by: 808Chopz Posted at: 2019-03-23T01:47:11.984Z Reads: 301

```
Thank you for posting the video. Hmm.. looks really hard :joy:  I hope flipsky offer service replacing resistor for a small price. I need a magnifying glass... damn those resistor too small :joy:
```

---
## \#41 Posted by: Schtekarsten Posted at: 2019-03-23T01:49:19.690Z Reads: 287

```
meh you will get the hang of it with some practice. If an idiot like me can do it and anyone could :smiley:
```

---
## \#42 Posted by: 808Chopz Posted at: 2019-03-23T02:19:55.536Z Reads: 287

```
oki you convinced me :grin:  just freaking order 100pcs for 0.16 cents too expensive! :rofl: I thought already retired doing soldering and fixing a circuit board. :grinning:
```

---
## \#43 Posted by: Schtekarsten Posted at: 2019-03-23T02:22:13.906Z Reads: 283

```
y it won't really brake the bank :joy:
```

---
## \#44 Posted by: Gamer43 Posted at: 2019-03-25T03:24:55.511Z Reads: 271

```
So Flipsky has informed us that they have sent the proposed changes to their test engineer, and hope to test them in the coming weeks. 
They want to make sure that the proposed solution works with problems and will take the necessary steps to ensure thorough testing. 
Not sure how long it will take, but they have something is in the works.
```

---
## \#45 Posted by: district9prawn Posted at: 2019-03-25T04:18:21.875Z Reads: 264

```
Don't Flipsky use that same mosfet on all their vesc boards?  

And by cutout do you mean over current fault? Or drv uvlo?
```

---
## \#46 Posted by: Gamer43 Posted at: 2019-03-25T05:04:37.344Z Reads: 262

```
no, some versions use the NTMFS5C612NL instead of the NTMFS5C628NL.

The former has a 1.5 mohm rdson and 25 nC switching charge; the latter has a 2.4mohm rdson and 10nC of switching charge. The latter has a better figure of merit and is thus better suited for parallelism.

The cutouts we are referring to is what the VESC sees as a "DRV Fault".
```

---
## \#47 Posted by: Novice Posted at: 2019-03-25T06:29:01.130Z Reads: 257

```
Thanks for this! Awesome work guys, hopefully 10s  of vescs will come back to life! :smile: 
#swedpower :D
```

---
## \#48 Posted by: ervinelin Posted at: 2019-03-25T09:22:33.600Z Reads: 252

```
And I have to do this for not just 1 resistor but 6?? I am 99.99% sure I will screw this up and end up with a dead VESC.... :sweat_smile:
```

---
## \#49 Posted by: Schtekarsten Posted at: 2019-03-25T09:56:04.743Z Reads: 249

```
Well you probably need to do so for 12 of them if you have a dual unit :joy:
Honestly, sure it is fiddly and they resistors are very tiny, but grab a scrap pcb that you dont care about and mess around with it, you will very quickly get the hang of it. Do some research on the side and you are good to go. never said it was super easy but very much possible to do and you need to mess up pretty bad in order to kill the thing. you need to use fairly good tools though, a soldering iron that is oxidized and skipping the flux and things like that is just never going to work. :v:
```

---
## \#50 Posted by: TimothyVaissi Posted at: 2019-03-26T16:14:43.449Z Reads: 248

```
I have two of these VESCs and will try this asap! Been having the same problem so lets hope this fixes it :D
```

---
## \#51 Posted by: Gamer43 Posted at: 2019-03-26T20:48:29.471Z Reads: 252

```
So Flipsky got back to us and said their initial tests were successful, and that they will be moving forward with implementing the change on all of their 4.20 FSESC hardware versions.

They say they have been very busy recently, but Schtekarsten and I will see if we can negotiate with them to offer to replace the resistors on existing 4.20 hardware versions.
```

---
## \#52 Posted by: J0ker3366 Posted at: 2019-03-26T20:49:54.606Z Reads: 254

```
[quote="Gamer43, post:51, topic:87824"]
say they have been very busy recently, but Schtekarsten and I will see if we can negotiate with them to offer to replace the resistors on existing 4.20 hardware versions
[/quote]

This is clutch
```

---
## \#53 Posted by: BillGordon Posted at: 2019-03-26T20:53:40.229Z Reads: 249

```
Yup, and it's such a classic "everyone wins" scenario. Love this aspect of the forum, and guys like @Schtekarsten and @Gamer43 who offer this kind of help.
```

---
## \#54 Posted by: Schtekarsten Posted at: 2019-03-26T20:54:36.474Z Reads: 251

```
Just to add on gamers post. 
They said that they have successfully tested out the resistor modification and that they will from tomorrow and onwards ship the new 4.20 based vescs with the modified resistors. They are just mega busy moving their factory to another location that they have not yet "officially" released the changes.
```

---
## \#55 Posted by: High-roller Posted at: 2019-03-26T20:56:36.584Z Reads: 245

```
Just to be clear, does this mean that the new 4.20 will be able to handle 12s without issues or should we still be cautious?
```

---
## \#56 Posted by: Schtekarsten Posted at: 2019-03-26T21:00:47.182Z Reads: 247

```
Yes!
By all means go wild!
Foc works too without any issues.

Well the cutouts have never been about the voltage to be honest!
```

---
## \#57 Posted by: Gamer43 Posted at: 2019-03-26T23:30:45.437Z Reads: 247

```
I guess we can say that after the resistor change, the FSESC 4.20 is probably one of the best VESC4 hardware variants available, especially at its price point, heatsink, and form factor.

12S FOC 60A, full throttle no problems. Hard to beat.
```

---
## \#58 Posted by: nickw1881 Posted at: 2019-03-27T22:43:07.760Z Reads: 243

```
Does the deadtime requirement not change with the higher gate resistance? Shouldnt we change the DT setting from 360ns or whatever to 400 something? Does the 4.2 drv have auto deadtime control?
```

---
## \#59 Posted by: Schtekarsten Posted at: 2019-03-27T23:03:01.715Z Reads: 250

```
Interesting!
I am not sure if the firmware automatically calculates that or not. Unfortunately im away for a few days so I can't test that right now. I have not noticed anything wired regarding the startup though so who knows. Maybe someone with more knowledge regarding the software or electronics in general can answer that question. :woman_shrugging::dancer:
```

---
## \#60 Posted by: Gamer43 Posted at: 2019-03-28T00:40:56.370Z Reads: 252

```
No, you cannot modify the dead time insertion on the VESC. It is more than sufficient (360nS). The dead time compensation in VESC tool is for the FOC algorithm, but for whatever reason, using the correct values actually introduces bugs.
```

---
## \#61 Posted by: nickw1881 Posted at: 2019-03-28T01:04:28.477Z Reads: 247

```
Not foc DT compensation. That reduces dt at low rpm in foc mode. I mean the deadtime number in the hw ifdefs. Transistor gate capacitance and gate resistance is an RC circuit. It has to charge up to 3.5V to start turning on, then it needs the miller charge, then it is on. If you use gate resistor that is 4x or 10x as large, it makes sense that it would take slightly longer to turn the transistors on. Its obviously not noticeable, so it is probably not a problem, but if it was my VESC i would flip my board over and take 5 min to look at the gate waveforms on the scope to double check.
```

---
## \#62 Posted by: Gamer43 Posted at: 2019-03-28T01:30:36.547Z Reads: 242

```
The default is 60 timer counts (at 168mhz, this is about 357nS.) 

The ntmfs5c628nl has a gate charge of 54nC, and an input capacitance pf 3.6nF. With 47 ohm gate resisfors this results in a rise/fall time of ~300nS. It cuts it close, but if there were problems with shoot-through, we wouldve encountered thermal problems during testing fairly quickly.
```

---
## \#63 Posted by: nickw1881 Posted at: 2019-03-28T03:00:37.951Z Reads: 238

```
You definitely would have noticed a problem by now. Sorry to be a negative nancy today :)
```

---
## \#64 Posted by: Gamer43 Posted at: 2019-03-28T03:07:47.256Z Reads: 241

```
No problem, I actually forgot about dead time insertion with respect to the gate resistors, thanks for bringing it up. Always good to indicate all possible problems with changes.
```

---
## \#65 Posted by: boramiNYC Posted at: 2019-03-28T03:27:10.007Z Reads: 231

```
I need this also, but it's a bit daunting when I don't even have a work bench. Can anyone provide this service?
```

---
## \#66 Posted by: Schtekarsten Posted at: 2019-03-28T08:13:28.074Z Reads: 230

```
well I dont have the equipment/ experience nor the time to make it worth while. Idk be creative contact people that knows their ways around electronics and supply them with the resistors and the vesc and a few beers. Or go to a computer repair store and se if they can do it after hours or something.
```

---
## \#67 Posted by: MiniChopper4Me Posted at: 2019-03-28T14:14:28.247Z Reads: 228

```
@boramiNYC I searched for all kinds of service providers in order to find someone capable of doing this repair down here in Miami.  I haven't gone to see him yet, nor do I know how much he will charge for this repair, but its a Computer Motherboard repair shop.  You might be able to find someone in NY doing this type of work.  Someone who "really repairs" phones might be able to do it as well, but def not a shop that just replaces broken screens mostly.
```

---
## \#68 Posted by: Mich21050 Posted at: 2019-03-28T14:18:22.411Z Reads: 223

```
@boramiNYC just an idea. Just look up Loius Rossmann(https://www.youtube.com/user/rossmanngroup) on youtube. He does board level repair. Maybe he can help you. :slight_smile:
```

---
## \#69 Posted by: TimothyVaissi Posted at: 2019-03-28T20:49:08.519Z Reads: 223

```
It took a couple of hours but I maneged to change the resistors and oh boy did it work! No more cut-offs!
```

---
## \#70 Posted by: Schtekarsten Posted at: 2019-03-28T21:55:31.623Z Reads: 223

```
Hey thats awesome to hear! glad we could help!
```

---
## \#71 Posted by: Okami Posted at: 2019-03-29T08:58:58.059Z Reads: 227

```
Where u ordered them? I guess 602 size is all thats needed and 1% tolerance, right? 

Not sure I will order from Arrow, so should find alternative locally
```

---
## \#72 Posted by: TimothyVaissi Posted at: 2019-03-29T12:54:19.046Z Reads: 223

```
I got them from a local shop here in Sweden. But I think as long the size, tolerance and of course the resistance is correct it should work. It took me a few tries to get the motor to spin correctly due to one or two resistors not soldered correctly. So no worries when it comes to burning the vesc :D
```

---
## \#73 Posted by: ervinelin Posted at: 2019-03-31T04:08:43.789Z Reads: 214

```
Actually I need to do 24 of them! I have 2 dual vescs... Groan...
```

---
## \#74 Posted by: Bobby Posted at: 2019-03-31T04:11:37.046Z Reads: 216

```
I talked to drv wizard himself and he seems willing to do them at his vesc repair price but offers no guarantee or warranty on this flipsky fix. Ive sent my focboxes and vescs to him many times and he returns them flawless. I am absolutely getting this done!!
```

---
## \#75 Posted by: 808Chopz Posted at: 2019-04-01T06:15:29.145Z Reads: 214

```
Successfully!!! installed the 603 resistors for dual 4.20 took couple of hours :joy: and the freaking flipsky anti spark explode! :triumph::triumph::triumph: ruined my discharge port and lucky not dangerous. I'm sticking x90 loop key from now on.
```

---
## \#77 Posted by: 808Chopz Posted at: 2019-04-01T06:33:45.863Z Reads: 218

```
Any update from flipsky about the new resistor modification for 4.20 fvesc? I'm planning buy another one for my second eboard.
```

---
## \#78 Posted by: Andy87 Posted at: 2019-04-01T07:21:50.664Z Reads: 222

```
look more up in the thread.
there is a statement from flipsky and what they going to do.
```

---
## \#79 Posted by: Schtekarsten Posted at: 2019-04-01T15:36:54.084Z Reads: 224

```
Flipsky are now shipping all their 4.20 based Vesc's with the newer resistors. They just have not had time to update their website as they are in the middle of moving their entire factory.
Have seen and gotten a few questions regarding it so I thought I might post it here.
```

---
## \#80 Posted by: briman05 Posted at: 2019-04-01T16:00:58.114Z Reads: 223

```
So who is going to be the one to order one for science?  Thank you to @Schtekarsten and @Gamer43 for going out of your way to figure out their mistake.
```

---
## \#81 Posted by: BillGordon Posted at: 2019-04-01T16:32:42.112Z Reads: 221

```
Thank you for volunteering,@briman05. Please let us know when your new 4.20 arrives.
```

---
## \#82 Posted by: Djens Posted at: 2019-04-01T17:33:08.448Z Reads: 211

```
I have been a long time lurker and finally created an account. If it wasn't for you guys my scooter would never be functional so thanks! I need to upgrade from my current 6s setup and since I'm a poor guy this ESC looks really nice. If they  changed the resistors I'll let you know. Just ordered a 4.20 mini.
```

---
## \#83 Posted by: Benjamin899 Posted at: 2019-04-01T17:35:11.626Z Reads: 204

```
check out the cheap Focer from @shaman
https://www.electric-skateboard.builders/t/cheap-focer-vesc-compatible-4-12-redesign/81344/307
```

---
## \#84 Posted by: Djens Posted at: 2019-04-01T17:54:47.858Z Reads: 202

```

Awesome initiative! If it was for sale, I'd snatch one in an instant.
```

---
## \#85 Posted by: briman05 Posted at: 2019-04-01T18:22:44.691Z Reads: 208

```
I didn't say I was going to do it haha.I just said that someone has to do it because then it will open up more stable options.
```

---
## \#86 Posted by: BillGordon Posted at: 2019-04-01T18:25:31.443Z Reads: 207

```
Thank you for confirming that you are going to be the guinea pig, @briman05. We all appreciate you raising your hand for science and for promising a review of your new 4.20.

Excited!
```

---
## \#87 Posted by: Bobby Posted at: 2019-04-01T18:34:22.864Z Reads: 205

```
@briman05. A class act! Cant wait for your review
```

---
## \#88 Posted by: briman05 Posted at: 2019-04-01T18:41:01.808Z Reads: 206

```
@Bobby

https://thumbs.gfycat.com/TatteredGenuineAardwolf-size_restricted.gif
```

---
## \#89 Posted by: BillGordon Posted at: 2019-04-01T18:48:40.081Z Reads: 207

```
![image|498x498](upload://3u6j3a9ITIuGz9acAAI1nQmgnJg.jpeg)
```

---
## \#90 Posted by: BillGordon Posted at: 2019-04-01T18:49:32.466Z Reads: 202

```
(I'll stop fucking up the thread now. Apologies.)
```

---
## \#91 Posted by: chrischo1996 Posted at: 2019-04-01T18:56:34.022Z Reads: 205

```
Can someone confirm that if I order a new 4.20 dual it will come with the above fixes in place? One side of my Flipsky Dual 6.6 died on me (fried STM chip I believe) so looking for a replacement while I get it fixed. I'll be running 12s FOC with 20 battery amps, so not pushing it too hard.
```

---
## \#92 Posted by: Schtekarsten Posted at: 2019-04-01T19:00:10.961Z Reads: 204

```
yah it should be
```

---
## \#93 Posted by: direct_drive Posted at: 2019-04-01T21:21:00.408Z Reads: 206

```
Sorry to tag you and ask you, but do we have any hope of support from Flipsky/@BarbaraZ for those of us who bought a pre fix 4.20?
```

---
## \#94 Posted by: Schtekarsten Posted at: 2019-04-01T21:42:38.831Z Reads: 204

```
to be honest I doubt it... I have no idea though.
Me and @Gamer43 are looking for ways to have them swapped, but sending them to china to have them replaced. Y I have a hard time seeing that happening.
I think either replacing them yourself or going to someone repairing pcbs or has the knowledge/equipment is the way to go in the end.
```

---
## \#95 Posted by: Gamer43 Posted at: 2019-04-03T09:52:27.551Z Reads: 209

```
Okay, so flipsky told us that they implemented the change at the end of March (March 27), and this applies to the mini and dual (non-plus versions, so ones that DO NOT integrate the antispark switch).

They are currently redesigning the plus version, which is why it has been out of stock.

ALSO, please let us know if you have ANY issues with heat, even at lower currents, or possibly over-current faults, as what @nickw1881 mentioned before with the dead-time insertion, could potentially be a problem on certain batches of MOSFETs that may have higher gate charge than normal. The risk is a potential for shoot-through.
If this does become an issue, the fix is simple, change one line (the dead time insertion #define) in the VESC firmware and recompile it and upload it. I will post binaries for that if that is necessary.
```

---
## \#96 Posted by: Vanarian Posted at: 2019-04-03T17:33:04.582Z Reads: 206

```
"Awesome" refers to people like you. I'll treat you a drink if we ever meet :beers:
```

---
## \#97 Posted by: chrischo1996 Posted at: 2019-04-03T19:41:35.777Z Reads: 211

```
I will be ordering the new 4.20 dual soon and testing it in 12s FOC with 20 battery amps and 65 motor amps. If I like it enough, I'll be keeping it instead of my Dual Flipsky 6.6.
```

---
## \#98 Posted by: banjaxxed Posted at: 2019-04-03T23:07:27.835Z Reads: 211

```
So you get a reward or only in heaven? 😆
```

---
## \#99 Posted by: chrischo1996 Posted at: 2019-04-08T16:10:48.441Z Reads: 216

```
Looks like the new 4.20 with pro switch just got released.
https://flipsky.net/collections/electronic-products/products/dual-fsesc4-20-100a-plus-based-on-vesc-with-anodized-aluminum-heatsink
@Gamer43, any idea if these are good to go?
```

---
## \#100 Posted by: Gamer43 Posted at: 2019-04-09T00:15:54.108Z Reads: 212

```
Flipsky told us they changed the resistors on the 4.20 plus and that is uses two NTMFS5C628NL MOSFETs in parallel for each channel (so the resistors are 22 ohm); they told us they would send us a sample for testing, we will get back to you guys on its performance once they send us one for testing.

Since it uses two MOSFETs in parallel it should in theory be able to handle 40% more current.
```

---
## \#101 Posted by: mtuan293 Posted at: 2019-04-13T01:46:26.690Z Reads: 216

```
Omg thanks a lot. I put a lot of hope to this 4.20 due to its form factor. But the cutouts are so irritating. Thanks for this finding. Now I can enjoy riding my board again!
```

---
## \#102 Posted by: mtuan293 Posted at: 2019-04-17T05:01:38.154Z Reads: 206

```
[quote="Gamer43, post:2, topic:87824"]
need to be replaced with **47** ohm resistors. The resistors’ original value is **4.7** ohm
[/quote]

🤔🤔Hmm... I have a feeling there’s a decimal place error. It’s likely that the engineers at Flipsky originally wanted 47 but then somehow 4.7 is passed along to manufacturing 🤔🤔
```

---
## \#103 Posted by: Arzamenable Posted at: 2019-04-17T05:19:46.337Z Reads: 200

```
Thanks for the work on this. I was getting ready to add another set to the fuckit bucket. 🤙
```

---
## \#104 Posted by: pookybear Posted at: 2019-04-17T05:20:32.962Z Reads: 199

```
Will there be an indicator on the units that it's the newer version? Going to build one for a friend and I'm looking to get these vescs.
```

---
## \#105 Posted by: Gamer43 Posted at: 2019-04-17T07:32:17.919Z Reads: 209

```
[quote="pookybear, post:104, topic:87824, full:true"]
Will there be an indicator on the units that it’s the newer version? Going to build one for a friend and I’m looking to get these vescs.
[/quote]

Flipsky told us they made the change on March 27.

[quote="mtuan293, post:102, topic:87824"]
> need to be replaced with **47** ohm resistors. The resistors’ original value is **4.7** ohm

:thinking::thinking:Hmm… I have a feeling there’s a decimal place error. It’s likely that the engineers at Flipsky originally wanted 47 but then somehow 4.7 is passed along to manufacturing :thinking::thinking:
[/quote]

Original VESC 4 schematic called for 4.7 ohm resistors, so I think they copied the schematic and didn't realize the slew rate on new MOSFETs would cause such a problem.

Just want to reiterate
@nickw1881 has a valid point about dead-time insertion, please do some bench testing before use and let us know if there are any heat issues.
```

---
## \#106 Posted by: chrischo1996 Posted at: 2019-04-17T16:05:04.327Z Reads: 203

```
Just installed the Dual Flipsky 4.20.
[Metr.pro record](https://metr.at/r/1JVHz) from a nighttime golf course ride yesterday.
Running 12s2p, 65 motor amps 20 battery amps to each 6354 motor.
Temperature readings show that the vesc remains cool, it was around 65F/18C outside.
Everything seems great so far!
```

---
## \#107 Posted by: pookybear Posted at: 2019-04-17T16:45:45.209Z Reads: 200

```
Any visual indicator that it is the new version vs the old. 

It's somewhat very hard to believe that they would replace the components on all remaining Vesc that are in stock to the newer hardware.
```

---
## \#108 Posted by: chrischo1996 Posted at: 2019-04-17T17:08:16.961Z Reads: 198

```
Couldn't see any visual indicators but it's running fine at 12s FOC with 65 motor amps, something that wasn't possible before the fix
```

---
## \#109 Posted by: briman05 Posted at: 2019-04-17T17:45:16.162Z Reads: 197

```
That is very encouraging considering it couldnt handle above 30 amps in foc before.
```

---
## \#110 Posted by: mtuan293 Posted at: 2019-04-17T21:24:22.428Z Reads: 194

```
Did you try hard accelerating and braking? Like jam full throttle then full brake
```

---
## \#111 Posted by: chrischo1996 Posted at: 2019-04-18T01:09:26.071Z Reads: 189

```
Yep, I ride hard. Again, I'm only pushing 20 battery amps to each vesc, higher Amos may have different results but so far so good, and vescs are staying exceptionally cool as well.
```

---
## \#112 Posted by: Hummie Posted at: 2019-04-18T02:48:18.732Z Reads: 186

```
How many motor amps can they do reliably? I like me motor amps
```

---
## \#113 Posted by: chrischo1996 Posted at: 2019-04-18T02:55:58.142Z Reads: 190

```
65 in my experience as mentioned above with my dual 6354
```

---
## \#114 Posted by: mtuan293 Posted at: 2019-04-18T03:42:21.431Z Reads: 187

```
My current un-fixed 4.20 (from your group buy a while ago) can peak at 80A
```

---
## \#115 Posted by: landonkun Posted at: 2019-04-18T04:00:36.544Z Reads: 191

```
I have mine at 30/-30 and it cuts out instantly, unless I accelerate REEEEEALLY slowly. Gonna have to do this fix, but damn, it's gonna be a pain.
```

---
## \#116 Posted by: mtuan293 Posted at: 2019-04-18T04:11:02.475Z Reads: 191

```
I have no cutouts whatsoever in BLDC. Only cutout in FOC. Diyeboard 270kv motor.
```

---
## \#117 Posted by: MiniChopper4Me Posted at: 2019-04-18T21:18:23.877Z Reads: 193

```
@Schtekarsten @Gamer43

I completed replacing the resistors on my 4.20 dual (not plus), but I'm not as skilled as some with micro-soldering.  If I didn't solder the resistors right, will the ESC still work? Are there some tests to ensure you soldered the pads well enough? After completion, my ESC works again, but at least on the bench I was still able to get it to shut down by giving it severe inputs.

Any advice would be much appreciated, I need a few beers after doing that job :stuck_out_tongue:
```

---
## \#118 Posted by: Gamer43 Posted at: 2019-04-18T21:19:59.080Z Reads: 198

```
if the motors spin up, you did it right. Visual inspection of the solder joint is normally enough to see if it is a cold joint or something like that.

Under what conditions are you getting it to fault?
```

---
## \#119 Posted by: MiniChopper4Me Posted at: 2019-04-18T21:21:04.282Z Reads: 198

```
If I go from full accel to full brake, the ESC shuts off, and won't turn back on until I power off/on (with a loop key)
```

---
## \#120 Posted by: Gamer43 Posted at: 2019-04-18T21:21:30.847Z Reads: 200

```
Wait, that's different, so the lights go out completely?
```

---
## \#121 Posted by: MiniChopper4Me Posted at: 2019-04-18T21:21:52.655Z Reads: 198

```
Yup, that's the behavior mine has always demonstrated
```

---
## \#122 Posted by: Gamer43 Posted at: 2019-04-18T21:23:41.748Z Reads: 194

```
Hmm, there might be something else wrong with the ESC then. Is this with a battery with a BMS connected?
```

---
## \#123 Posted by: MiniChopper4Me Posted at: 2019-04-18T21:25:41.130Z Reads: 193

```
I didn't make the battery, but I asked for it to have discharge bypassed.  I guess it does sound like the battery is cutting out...I might need to cut it open and inspect.

Well, at least I completed the repair successfully it appears!
```

---
## \#124 Posted by: Gamer43 Posted at: 2019-04-18T21:28:57.275Z Reads: 190

```
When the lights go out, check if anything gets warm, if not, probe across the positive and negative terminals with a multimeter to see if battery voltage is still present.
```

---
## \#125 Posted by: MiniChopper4Me Posted at: 2019-04-18T21:42:40.547Z Reads: 191

```
Thanks for helping me finally figure out what was going on :P Turns out its the battery.  My battery meter is connected to power before the ESC, and when the problem happens, its turning off as well.  I thought the ESC was faulting!

I'll bet the battery has the discharge wired through the BMS as you suggested.  I'll need to hack open the shrink wrap and confirm/repair.
```

---
## \#126 Posted by: Gamer43 Posted at: 2019-04-18T21:49:44.281Z Reads: 196

```
Glad I could help :).
```

---
## \#127 Posted by: Mazda_bater Posted at: 2019-04-24T00:26:07.036Z Reads: 194

```
I had a go at this yesterday and think I've ballsed it up somewhere motors and remote were set up previously on this 
Vesc. I removed all the resistors fairly quickly and took a bit over an hour to re solder the new resistors in. The slave vesc (2) seems to make a knock when spinning the motor up if I switch the motor to the other vesc it spins up fine
```

---
## \#128 Posted by: Gamer43 Posted at: 2019-04-24T02:04:00.642Z Reads: 193

```
Did you try running the detection again after the resistor swap? Does the motor spin up at all?
```

---
## \#129 Posted by: Mazda_bater Posted at: 2019-04-24T03:17:28.736Z Reads: 196

```
Yeah both motors are spinning I pulled the vesc back out and rechecked all the solder joints I can't pick the fault I'll try reconfiguring them and see what it does
```

---
## \#130 Posted by: Mazda_bater Posted at: 2019-04-24T05:30:09.916Z Reads: 194

```
Redetrcting the motors had them configure fine. Although neither side would complete the hall sensor detection. I set the motor amps to something that would have caused a full shutdown of the fsesc 50A and took it out for a test run. There was a notorious rise in the footpath that this exact fsesc, motor and remote combo just wouldn't climb it would have been a rise over 50m going up 5m in total. The fsesc at 30A wouldn't make it up and any higher setting would cause a reset here every time. She lost a bit of speed but hauled my fat ass up there no worries
```

---
## \#131 Posted by: Mazda_bater Posted at: 2019-04-24T05:30:49.992Z Reads: 188

```
I forgot to say THANK YOU
```

---
## \#132 Posted by: landonkun Posted at: 2019-04-25T06:16:36.303Z Reads: 185

```
Welp. Despite feeling like I did a decent enough job with the new resistors, I connected to the bldc tool, ran motor configuration and poof! Smoke came out and vesc will no longer turn on. That's a real bummer. There are no bridges, that's for sure. I guess I must've missed a connection somewhere, but I was under the impression that nothing would happen. Oh well.

Who wants a dead vesc?
```

---
## \#133 Posted by: BillGordon Posted at: 2019-04-25T06:21:46.270Z Reads: 188

```
I feel your pain, brother. I might suggest that before you write it off completely, check in with the Wizard @JohnnyMeduse to see if it can be saved.
```

---
## \#134 Posted by: landonkun Posted at: 2019-04-25T06:24:39.278Z Reads: 189

```
Good call. Thank you. I shot him a message for now.

The worst part is I was quite proud of myself when I put my soldering iron down.. thought I did a pretty good job.
```

---
## \#135 Posted by: BillGordon Posted at: 2019-04-25T06:29:50.362Z Reads: 188

```
Yes, I have felt this particular emotional rollercoaster more than once, and on far less ambitious undertakings.
```

---
## \#136 Posted by: Mich21050 Posted at: 2019-04-25T07:44:06.393Z Reads: 185

```
[quote="landonkun, post:132, topic:87824"]
Who wants a dead vesc?
[/quote]

If you don't send it to @JohnnyMeduse I would highly recommend to do so) just send me a pm... :slight_smile:
```

---
## \#137 Posted by: b264 Posted at: 2019-04-25T08:42:23.681Z Reads: 183

```
Resistors come mainly in standard sizes, like

1, 2.2, 3.3, 4.7, 6.8

then multiply those all by ten or divide by ten any number of times, those are the standard sizes you can choose from.  So it probably wasn't a decimal error, it was probably just a less good design, but intentional.

As @Gamer43 [said](https://www.electric-skateboard.builders/t/flipsky-4-20-a-explanation-to-the-mystery-and-how-to-stop-the-cutouts-entirely/87824/105?u=b264), it's directly from the original VESC 4 design
```

---
## \#138 Posted by: legend27 Posted at: 2019-04-25T10:39:47.237Z Reads: 186

```
Awesome work!

Before my question, I just want to admit, I haven’t read all the posts... Sry..

Would this work for 4.12 hardware and prevent the mosfet from getting crazy hot (75 degrees Celsius even at low speed with 20A motor and 10A battery)?
```

---
## \#139 Posted by: Schtekarsten Posted at: 2019-04-25T11:23:37.495Z Reads: 184

```
noop sorry!
```

---
## \#140 Posted by: Gamer43 Posted at: 2019-04-25T15:27:32.733Z Reads: 184

```
It would actually make it utterly unusable. 

Thats why you dont use international rectifier mosfets.

But everyone seems to love using them :man_shrugging:
```

---
## \#141 Posted by: 1337 Posted at: 2019-04-30T16:58:33.775Z Reads: 188

```
Just got my Vesc 4.20 today, all the resisters say 47o in all the right places, so glad I found this thread before I ordered, I was gonna get a 4.12 version due to reading about cutouts. Thanks a ton guys.
```

---
## \#142 Posted by: chrischo1996 Posted at: 2019-04-30T18:00:08.770Z Reads: 185

```
Ok help me out here folks... I'm getting cutouts in two separate occasions with my (edit: supposedly from the new stock with the correct resistors) Flipsky Dual 4.20.

First, I get cutouts when I'm in a congested intersections with lots of traffic lights. I've tried re-positioning the receiver in several locations in the enclosure, no improvement. I know people say the remote cutting out feels like the board is braking because of belt friction, but I think it's actively lightly braking for a split second, just to jolt me a little bit. I never had these random cutouts with the Flipsky Dual 6.6.

Second, I get cutouts during hard acceleration, i.e. drag racing my friends. The board will cutout every time I go full throttle hard.

Vesc settings are 12s FOC, 20A battery amps, -10A battery regen, 60A motor, 30A motor brake. Any help would be appreciated!
```

---
## \#143 Posted by: Benjamin899 Posted at: 2019-04-30T18:35:23.507Z Reads: 170

```
did you even read this thread?
```

---
## \#144 Posted by: chrischo1996 Posted at: 2019-04-30T18:50:59.269Z Reads: 172

```
Yikes, my bad didn't mention that these are the new ones I ordered after they replaced their stock.
```

---
## \#145 Posted by: Benjamin899 Posted at: 2019-04-30T19:10:47.319Z Reads: 175

```
to me this sounds like you got the old one. Just because they say they will send the new ones, doesnt mean they will. Can you confirm through visual inspection what type of resistors are used?
```

---
## \#146 Posted by: chrischo1996 Posted at: 2019-04-30T19:18:46.417Z Reads: 178

```
Maybe that's the case, I'll take a look when I get the chance once I'm done with finals
```

---
## \#147 Posted by: pat.speed Posted at: 2019-04-30T20:35:01.075Z Reads: 178

```
The first part has nothing to do with the vesc, that is all about your receiver.

The second bit, if it is the new one it’s possible it’s actually the battery cutting out. Is your bms bypassed?
```

---
## \#148 Posted by: chrischo1996 Posted at: 2019-04-30T20:43:51.713Z Reads: 176

```
Yes, it's a charge only BMS. I apologize for not being very knowledgeable about BMS's, how would bypassing discharge create cutouts if the max battery current is properly being limited by the VESC? I should also mention that there are never any fault codes thrown according to my metr.pro.
```

---
## \#149 Posted by: pat.speed Posted at: 2019-04-30T20:49:49.399Z Reads: 176

```
That is good, I was checking to make sure it wasn’t the bms cutting out but you already have it bypasses. What sort of battery are you running? If it is small the high current drawn may cause it to sag below cut off voltages
```

---
## \#150 Posted by: chrischo1996 Posted at: 2019-04-30T20:54:46.301Z Reads: 171

```
Darn I missed out on a lot of details, braindead from pulling an all nighter for finals...
Anyways, I have a 12s2p with Samsung 30Q made by Cory from Hyperion. I'm a little skeptical it's the battery because I didn't have these issues with the 6.6. Regardless, I'll update once I get a chance to peek inside the enclosure and make sure I have the updated 4.20 dual and also check all the wiring again. Thanks!
```

---
## \#151 Posted by: Niak Posted at: 2019-05-01T16:14:23.666Z Reads: 173

```
How do you know if you’re ordering the updated fixed version? Is it only direct from flipsky or also from AliExpress etc?

Has the plus been confirmed as fixed yet? TLDR
```

---
## \#152 Posted by: Schtekarsten Posted at: 2019-05-01T21:38:47.395Z Reads: 174

```
What they told me and @Gamer43 is that from the 27th of mars all 4.20 based VESC's will be shipped with the the updated resistors (so cutouts should not be a problem) as for resellers and so on I have no idea.
I have had a bit of problems receiving the new dual 4.20 plus version from DHL. But hopefully it should be here in a day or two and then it will probably take a few days until I have tested the unit and gone through it properly. 
The integrated anti-spark unit does not have pre charge so that will be a bit of Russian roulette I guess.
```

---
## \#153 Posted by: Niak Posted at: 2019-05-02T00:23:13.722Z Reads: 176

```
I was mostly looking at the plus because on the site it says 10s recommended.

But if 12s is ok on 4.20 then I might just get that
```

---
## \#154 Posted by: nirurin Posted at: 2019-05-03T00:46:06.236Z Reads: 176

```
So I'm currently needing to purchase a dual-VESC for two 170kv motors, running a 10s4p 30Q battery. But I'm on a bit of a budget...

So my main plan was to get the Flipsky Dual 4.20, the 'new' plus version that's on their website, direct from Flipsky. Is this likely to be a problem? Is it generally recommended that the 6.6 is the only one to go for?
```

---
## \#155 Posted by: chrischo1996 Posted at: 2019-05-03T03:27:11.716Z Reads: 180

```
So I opened up the board today, and as far as I can see, all the resistors are correct. Any other ideas what might be causing cutouts?
![Screenshot_Photos_20190502-202030|256x500](upload://mqMDrG1xdZOeYAwUqFUWede62lm.jpeg)
```

---
## \#156 Posted by: BillGordon Posted at: 2019-05-03T04:41:29.652Z Reads: 176

```
Well, with @Schtekarsten posting his review of the updated 4.20 soon, I would wait a bit. I have a 6.6 dual, but it is overkill for my "born to be mild" nature.
```

---
## \#157 Posted by: Schtekarsten Posted at: 2019-05-03T08:26:55.673Z Reads: 180

```
Sorry to hear that!
You should be getting a “over current” fault thrown if it is the regular cutouts.
So that gets me thinking.
I have fooled myself by having too low of a battery voltage thinking it was the cutouts but in fact it was the Vesc cutting it off. As well as accidentally putting in higher voltage cutoff values than normal. 
But y idk it all seems wired.
Do all the easy/obvious stuff first.
Go through the battery battery and check it’s voltage as well as if it is balanced or not.
Reset the Vesc settings and program it again. 
Charge the remote. 
Check all the wiring.
Idk can’t think of much else right now but to me that seems like a voltage cutout that is based on the Vesc.
Trouble shooting through the web is monkey science. 
But y try to go through all the logical stuff.😂💃🏼🤷🏼‍♀️

Oh DHL f***** up twice ✌️
```

---
## \#158 Posted by: nirurin Posted at: 2019-05-04T00:41:26.004Z Reads: 174

```
[quote="BillGordon, post:156, topic:87824"]
Well, with @Schtekarsten posting his review of the updated 4.20 soon, I would wait a bit.
[/quote]

Do we know how soon? Seems he's having some problems with the couriers lol
```

---
## \#159 Posted by: BillGordon Posted at: 2019-05-04T01:05:21.337Z Reads: 176

```
Apparently, not soon enough FOR SOME PEOPLE. 😊

To have it tested by one of the guys who engineered the fix is a pretty unique opportunity. If it gets the thumbs up, I'll be getting one with all the trimmings.
```

---
## \#160 Posted by: nirurin Posted at: 2019-05-10T21:37:05.411Z Reads: 172

```
Has there been any update on this? I assumed someone would mention it on this thread if it happened, but you never know
```

---
## \#161 Posted by: Schtekarsten Posted at: 2019-05-10T22:01:46.377Z Reads: 176

```
that someone should be me...
i have received it but have not had the time to test it yet, sometime life gets in the way... 

What I can say though just by looking at it is that it is a stepup from the last dual 4.20 versions. It uses double the amount of mosfets making it able to handle higher continues current. It does use a shit ton of mosfets on the antispark aswell making it more robust than I previously thought, it might actually last a while before it goes kaboom. whoo knows. the good thing though is that when/if it goes Kabooom it will just render the anti-spark unit useless and you should be able to just bypass the whole anti-spark part of the VESC and use a xt90s or an external antispark instead.

On a side note it does use 22ohm resistors which we tested out and recommended them to use in conjunction with the "better 612 mosfets" which they used on the pervious version of the dual 4.20 plus  esc. but now they have reverted to the "cheeper 628 mosfets" that they always have used on the regular dual 4.20 vesc. but they have instead opted to double up on the 628 mosfets an put them in parallel.

in my tests the 47ohms where the resistors to use with the "cheeper 628 mosfets" and anything below that would make the vesc cut out. and what the F happens when you put the mosfets in parallel is beyond me (im too dumb for that). Maybe @Gamer43 could jump in and answer that.

Either way i will hopefully have some time over tomorrow to test that out. My belt drives are on the healing bench at the moment and so it will have to be on some Chinese hubs until they get back on track. However if I yank up the settings it should not make a difference though.

sorry for being a slow shit. I will continue to post on this thread when I find out some more cool shit regarding the Vesc's. who knows if it will be fire or love.
```

---
## \#162 Posted by: nirurin Posted at: 2019-05-10T22:10:49.204Z Reads: 168

```
[quote="Schtekarsten, post:161, topic:87824"]
sorry for being a slow shit.
[/quote]

Haha, no need to be sorry, I know I appreciate that you took the time to actually do these tests, and I'd expect a lot of other people appreciate it as well! The only reason I asked was because the VESC is the last component I need to order, and I was eager to find out if this one is actually good enough for my purposes. It sounds like it's more than good enough! 

As for the anti-spark (I'm new to these things), but is that what's built in to the 'smart switch' LED button that the dual comes with? I also have a switch built in to my bestech BMS, so I'm not too sure which of these switches I should be using and which is better to bypass. I guess I could always wire up both..
```

---
## \#163 Posted by: Schtekarsten Posted at: 2019-05-10T22:21:38.155Z Reads: 166

```
I would start of by bypassing the besttech bms and use the integrated one on the Dual 4.2 plus vesc if you go for that unit. because the antispark on the 4.20 plus also got room to start auto off and all that stuff which is nice, and when/if that thing blows up you could always bypass the unit and use the Besttech unit instead. (that would require some soldering work though, will update when I have a little video on how to to that in the future, need some help from the smarter man on how to do so exactly so I don't mess stuff up) 
I would maybe wait before I have tested out the cutout thing tomorrow or until @Gamer43 has confirmed that the 22ohms resistors are the correct ones to use.
```

---
## \#164 Posted by: Gamer43 Posted at: 2019-05-11T13:26:28.291Z Reads: 169

```
@Schtekarsten 22 ohm should be the working value. The actual value would be 23.5 or 24 ohm, but if two ohms really makes that much of a difference I'm going to reeeeee out of this forum (If that's the case, hopefully flipsky won't be too annoyed they have to change the resistor value a second time).
Putting MOSFETs in parallel slightly alters the parasitic characteristics, but for all intents and purposes it can be treated as a single MOSFET with corresponding electrical characteristics.
We are actually cutting it real close with the dead time insertion, I'm still worried some units with higher gate charge might have issues with shoot-through. I need to figure out how to pull request the vesc firmware and push a version with 600nS of dead time instead of the default 360nS.

@chrischo1996 any chance you could provide more details on when the cutouts are occurring? Things like current and other parameters would be very helpful in determining the cause. Also what app settings are you using (positive ramping time).
I believe on a previous ride, you said you encountered no cutouts, what changed between that ride and the one you began to experience cutouts with?
```

---
## \#165 Posted by: chrischo1996 Posted at: 2019-05-11T13:31:15.379Z Reads: 174

```
I'm not with my board at the moment so this is all off the top of my head, I'm fairly certain they're accurate though.

Battery Max: 20A.
Battery Min: -10A.
Motor Max: 65A.
Motor min: -30A.

App settings:
Throttle curve: -10% for both accel and braking.
Positive ramping time: 0.30s

Cutouts happened only when I slammed on the throttle to drag race my friends. I went through everything and rechecked all the connections and found a slightly loose bullet connector between the VESC and the motor, it was pulled out less than 1/4" inch. I plugged that back in and taped it up and haven't had cutouts since, so that may have been the problem. I'd like to do more testing before I reach a confident conclusion though.
```

---
## \#166 Posted by: Gamer43 Posted at: 2019-05-12T06:57:32.331Z Reads: 165

```
I've had similar problems with loose connectors. Let us know how your tests go, thanks! If you still get cutouts under hard throttle or braking, try a positive ramping time of 0.5s or 0.8s and see if that helps.
```

---
## \#167 Posted by: chrischo1996 Posted at: 2019-05-12T15:48:48.686Z Reads: 166

```
Won't be back in the states for a week but will update when I get back.
```

---
## \#168 Posted by: nirurin Posted at: 2019-05-13T00:39:39.516Z Reads: 177

```
Question for you - I'm looking to make a 3D printed enclosure for the VESC (which I don't have yet, so I'm having to make the draft using photos and online spec sheets). The problem I have is that I need screw mounting holes in order to bolt the vesc to the enclosure bottom, as I do not want to use glue or sticky tape.

However it seems that the heatsink isn't using bolt-through standoffs but instead some other kind of standoff with a threaded bottom half. I was wondering if it would be possible to remove these standoffs, and replace them with bolt-through ones like these? - [LINK](https://uk.rs-online.com/web/p/standoffs/2808862/)

Figured as you have the vesc to hand it would be easy enough to find out for me (if you don't mind?). Means I can keep making my plans and drafting my 3D model.

Edit: If you could also tell me the height of the standoff (the gap between the pcb and the heatsink), as well as the bolt size they're using? I'm guessing it's M2 or M3.
```

---
## \#169 Posted by: direct_drive Posted at: 2019-05-14T09:34:40.918Z Reads: 166

```
It is worth mentioning i think.... 

I bought my 4.20 dual back in August, and after the cut out fix was announced spoke to Flipsky and they were happy to swap it for me 👍🏻

Im just waiting on the replacement revised unit to land.

I had to pay shipping both ways, which for me in the UK was a total of around £25, which i was happy to pay for a working unit as id most certainly make a balls up of trying to solder the fix 😂
```

---
## \#170 Posted by: Gamer43 Posted at: 2019-05-14T12:26:58.405Z Reads: 161

```
Hey man, that's awesome!

Let us know how it performs after the fix!
```

---
## \#171 Posted by: Gamer43 Posted at: 2019-05-14T12:34:09.635Z Reads: 158

```
@landonkun

I think I know whats wrong with your ESC and it is salvagable. If you still have it could you probe across all three motor phases and see if any of them are a short to the positive rail or ground?

If my hunch is right, a pair of MOSFETs need to be replaced. If not, then it would probably be the drv8302.
```

---
## \#172 Posted by: landonkun Posted at: 2019-05-14T18:34:05.165Z Reads: 157

```
The DRV wizard has already repaired it for me :) but thank you!
```

---
## \#173 Posted by: b264 Posted at: 2019-05-14T23:20:38.235Z Reads: 158

```
I can verify the Flipsky MiniFSESC4.20 that are *currently shipping* have arrived, and they do have the new 47Ω gate resistors.

(In case anyone wanted confirmation. :slight_smile: )
```

---
## \#174 Posted by: DAddYE Posted at: 2019-05-15T02:50:15.891Z Reads: 160

```
They shipped my dual 4.20 plus this morning. :crossed_fingers:
```

---
## \#175 Posted by: lrdesigns Posted at: 2019-05-15T03:02:01.745Z Reads: 160

```
Pics? This thread needs more pics.
```

---
## \#176 Posted by: humanisticnick Posted at: 2019-05-15T04:33:23.995Z Reads: 160

```
Did you just use your 4.20 to upgrade a full DIYEBOARD kit?
```

---
## \#177 Posted by: mtuan293 Posted at: 2019-05-15T06:39:08.309Z Reads: 173

```
Yes. I replaced their ESC with the flipsky 4.20.
```

---
## \#178 Posted by: b264 Posted at: 2019-05-16T00:04:01.900Z Reads: 180

```
[quote="lrdesigns, post:175, topic:87824, full:true"]
Pics? This thread needs more pics.
[/quote]

Sure

[Mini FSESC4.20](https://flipsky.net/collections/electronic-products/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike)

![20190515_185802_HDR|690x388](upload://36tvpYk6qPt9ByEAQLfzsDVE6G7.jpeg) 

![20190515_185810|690x388](upload://zgZaq7MeOlxjFglNQUPQOm5Ur7t.jpeg) 

![20190515_185817_Burst01|690x388](upload://6OwCbMOeIb8ZxUWqDKMXTajWfBh.jpeg) 

![20190515_185823_HDR|690x388](upload://pCT6GjzoAsBiTAhMkRHyNB60BI5.jpeg) 

![20190515_185849_HDR|690x388](upload://mv1w9uh8R0GoOk92BT7cZ71lDPa.jpeg) 

![20190515_185753|690x388](upload://9D88AZ6VJh1i3CoIQjoQkSOAF4r.jpeg)

The wires are 12AWG (motor), 12AWG (battery), and 26AWG (PWM) silicone-insulated stranded wires
```

---
## \#179 Posted by: b264 Posted at: 2019-05-16T00:05:50.043Z Reads: 173

```
Also came with these wires

![20190515_190505|690x388](upload://o0PSR2dHCj6Hc0LLmgaAhnPfEbG.jpeg)
```

---
## \#180 Posted by: goldrabe Posted at: 2019-05-16T03:36:38.345Z Reads: 172

```
What you ordered a dual unit?:exploding_head:
```

---
## \#181 Posted by: pookybear Posted at: 2019-05-16T04:28:25.124Z Reads: 168

```
Can't wait for your test results.
```

---
## \#182 Posted by: lrdesigns Posted at: 2019-05-16T04:38:25.329Z Reads: 171

```
Thanks for the photos. 

@b264 what is your reason for getting one of these? 

I thought you were firmly in the camp of only using stuff proven to be 100% reliable. 

These seem more on the experimental side for your style?

I am just surprised as the esc is one of the most critical items in terms of safety.
```

---
## \#183 Posted by: b264 Posted at: 2019-05-16T06:27:07.877Z Reads: 170

```
[quote="goldrabe, post:180, topic:87824, full:true"]
What you ordered a dual unit?
[/quote]

No way :rofl:

It's two singles.
```

---
## \#184 Posted by: b264 Posted at: 2019-05-16T06:27:53.195Z Reads: 168

```
[quote="lrdesigns, post:182, topic:87824"]
@b264 what is your reason for getting one of these?
[/quote]

Trying to find a goto single ESC now that @onloop canceled FOCBOX production.

Also the small size of this specific unit allows me to decide whether to convert some single drive 6374 skates to dual drive 5065 which is more reliable.

Maybe.  Just testing things out.  I got two to try.

If either fails, I won't be getting any more and will try something else, maybe something based on VESC 6.
```

---
## \#185 Posted by: Gamer43 Posted at: 2019-05-16T06:46:41.747Z Reads: 171

```
[quote="b264, post:184, topic:87824"]
If either fails, I won’t be getting any more and will try something else, maybe something based on VESC 6.
[/quote]


_That moment when @b264 gets the one batch of MOSFETs that results in shootthrough_ :rofl:

Fix for that is easy though, I just need to get an ubuntu box so I can compile the VESC source code :rage:.
```

---
## \#187 Posted by: nirurin Posted at: 2019-05-17T02:51:34.164Z Reads: 159

```
[quote="nirurin, post:168, topic:87824"]
Question for you - I’m looking to make a 3D printed enclosure for the VESC (which I don’t have yet, so I’m having to make the draft using photos and online spec sheets). The problem I have is that I need screw mounting holes in order to bolt the vesc to the enclosure bottom, as I do not want to use glue or sticky tape.

However it seems that the heatsink isn’t using bolt-through standoffs but instead some other kind of standoff with a threaded bottom half. I was wondering if it would be possible to remove these standoffs, and replace them with bolt-through ones like these? - [LINK ](https://uk.rs-online.com/web/p/standoffs/2808862/)

Figured as you have the vesc to hand it would be easy enough to find out for me (if you don’t mind?). Means I can keep making my plans and drafting my 3D model.

Edit: If you could also tell me the height of the standoff (the gap between the pcb and the heatsink), as well as the bolt size they’re using? I’m guessing it’s M2 or M3.
[/quote]

Bumping this question, just because I'm still interested in the answer as it means I can look for the correct standoffs (if the built-in ones are removable, that is).
```

---
## \#188 Posted by: Schtekarsten Posted at: 2019-05-17T20:07:17.822Z Reads: 156

```
sorry for the late reply, yeah you should be able to swap them out and print a case for them. not sure what design you are going for but I guess either a full nut spacer and a long screw going through with a regular nut on the bottom side would be an option, or if height is an issue you could use the printed case itself as the nut spacer in order to not have a nut sticking out on the bottom side. just keep in mind that there are components real close to some of the the screw holes in the pcb.

they are using m3's btw and I pm'd a boatload of pictures as I did not want to clog up the thread.
```

---
## \#189 Posted by: nirurin Posted at: 2019-05-17T22:01:04.454Z Reads: 156

```
[quote="Schtekarsten, post:188, topic:87824"]
I pm’d a boatload of pictures as I did not want to clog up the thread
[/quote]
 Haha yeh I got them, was a little worried when I saw all the notifications! Thanks those pictures will be great! 

I plan to keep the heatsink etc as it is now, but I want to mount the entire VESC to a case using the current bolt holes, so I would just change the current spacers for ones the same height, but which are hollow so that I can screw a short bolt up from the bottom of the case and up into the bottom of the vesc and into the standoff. 

Once I make it I'll post it up here so you can see what I end up with :) 

Thanks again for the pics, they're going to be a lot of help :)
```

---
## \#190 Posted by: 1337 Posted at: 2019-05-18T22:14:52.569Z Reads: 147

```
 Got mine connected and bench tested today, waiting on a motor pulley to go test ride! 

Has anyone run this on sensor less FOC?
```

---
## \#191 Posted by: Schtekarsten Posted at: 2019-05-18T22:18:53.160Z Reads: 143

```
y it's fine
```

---
## \#192 Posted by: jun1208 Posted at: 2019-05-26T06:40:21.174Z Reads: 139

```
Just got my new 4.20 plus yesterday, do you guys reckon that it will run fine with with foosted built? I'm planning to use 40a max/min for motor and 20a for battery max..

6354 190kv
10s3p 30Q
```

---
## \#193 Posted by: Gamer43 Posted at: 2019-05-26T06:49:01.868Z Reads: 140

```
Schtekarsten was using more aggressive settings with his, so it should be fine. I would still be wary and note any possible problems.
```

---
## \#194 Posted by: jun1208 Posted at: 2019-05-26T07:40:58.813Z Reads: 143

```
That's great to hear, was thinking to push it at 45a at some time but was thinking if the 10s3p can cope with it or not .
```

---
## \#195 Posted by: pat.speed Posted at: 2019-05-26T22:10:54.648Z Reads: 138

```
You can up motor max to whatever you want as long as the motors and vesc can handle it. The battery max is what you need to be careful about, it shouldn’t be more than 30a per esc
```

---
## \#196 Posted by: ADrum707 Posted at: 2019-05-27T20:22:54.361Z Reads: 134

```
It looks as if one can only order a minimum of five thousand of those resistors, and there's an 8 week lead time on them. Maybe I'm missing something, but there's got to be a better way to get the resistors I need?
```

---
## \#197 Posted by: Gamer43 Posted at: 2019-05-27T20:30:48.266Z Reads: 138

```
@ADrum707

https://www.arrow.com/en/products/cr0603-jw-470elf/bourns

My apologies, I forgot to reply to you last night X_X.

Free overnight shipping :yum:

_5000 of them is only $12 anyway xDDD_
```

---
## \#198 Posted by: ADrum707 Posted at: 2019-05-27T20:37:36.963Z Reads: 138

```
@Gamer43 

Thanks man, got them ordered! You guys are wizards!  :)
```

---
## \#199 Posted by: ADrum707 Posted at: 2019-05-27T21:06:24.676Z Reads: 141

```
@Gamer43 @Schtekarsten  

Additionally - I noted in the YouTube video (https://www.youtube.com/watch?v=0A8nzc24Mzw) that the person doing the work, mentioned the soldering iron wasn't very hot - "about 340 or so" is it safe to assume that's C and not F? My soldering station is adjustable up to almost 900 degrees F and I don't want to accidentally damage other components if my iron is too hot...
```

---
## \#200 Posted by: Schtekarsten Posted at: 2019-05-27T21:07:42.879Z Reads: 142

```
regular celsius not the Frankenstein units
```

---
## \#201 Posted by: ADrum707 Posted at: 2019-05-27T21:08:14.141Z Reads: 142

```
:rofl::rofl::rofl: maybe someday America will switch it's standard to C
```

---
## \#202 Posted by: AlanZhou Posted at: 2019-05-27T21:08:34.809Z Reads: 144

```
[quote="ADrum707, post:201, topic:87824"]
C
[/quote]

gotta account for old people.
```

---
## \#203 Posted by: Randy_bobandy Posted at: 2019-05-28T17:23:49.270Z Reads: 144

```
Did Flipsky do any revisions for the 6.6 or 6.6 plus?
```

---
## \#204 Posted by: Riako Posted at: 2019-05-29T16:27:26.344Z Reads: 140

```
... don't if I can do this change one day, if someone want a dual FS 4.20 PM me ;)
```

---
## \#205 Posted by: Pimousse Posted at: 2019-05-31T06:53:28.873Z Reads: 138

```
I'll try with those you sent to me and keep you posted.
If ok, I'll do it on your dual.
```

---
## \#206 Posted by: 1337 Posted at: 2019-05-31T23:19:03.324Z Reads: 135

```
Test run today, in foc, I had a drv error in my living room trying to move slowly on the tile from a standstill, had to unplug and plug the loop key back in. Then I rode it outside around the block a few times and all seemed ok, maybe I’ll give it a kick before I get on the throttle from now on. I like how quiet it is now, I’ve never ridden it in bldc to be fair though.

Edit sensor-less keda 190kv motors
```

---
## \#207 Posted by: 1337 Posted at: 2019-06-02T14:32:42.346Z Reads: 126

```
Ok, DO NOT FOC this 4.20 Bad advice above, it is not fine. I had the drv error the other night I unplugged and plugged back in and it worked, today I pushed off the head to the store before work and got the drv error, It’s not going away this time.
```

---
## \#208 Posted by: chrischo1996 Posted at: 2019-06-07T19:08:38.476Z Reads: 122

```
I've been running the revised 4.20 dual in 12S FOC mode no problems for hundreds of miles now. What are your settings?
```

---
## \#209 Posted by: 1337 Posted at: 2019-06-07T19:48:39.674Z Reads: 122

```
Motor 60,-60
Battery 30,-10
```

---
## \#210 Posted by: Mazda_bater Posted at: 2019-06-07T22:20:12.876Z Reads: 130

```
I mustn’t have done the best soldering job, my test ride came back with one side not functioning properly and when I try to motor detect, it fails
```

---
## \#211 Posted by: chrischo1996 Posted at: 2019-06-07T22:22:16.974Z Reads: 130

```
Those settings seek reasonable, make sure your phase wires between motor and vesc are 100% in and insulated, I had similar cutouts due to this before.
```

---
## \#212 Posted by: Gamer43 Posted at: 2019-06-09T03:49:22.338Z Reads: 129

```
Most likely a cold joint, a lot of flux and lightly tapping with a tinned iron should do the trick.
```

---
## \#213 Posted by: trakais Posted at: 2019-06-13T06:17:24.664Z Reads: 128

```
After some contemplation I got 2x FSESC 4.12 Mini's for my small build while I was in china. Got it for TaoBao prices so cannot complain. So far it's been good. Running them on a Chinese iFasun KIT with 10S2P Samsung battery pack and unknown KV motors. I run them in FOC and had no issues with CANbus either. Got them together with VX1 remote and their BLE module, both plugged in on UART ports and work seamlessly together. This is a rather small board with small battery so the amps on the VESCs are quite small but the board still gives very impressive performance. I think I have my motors at 40A each but with 40A max output on the battery, but not 100% sure.
![IMG_20190611_130658|666x500](upload://uKl9HJn0QsVpXNxyH8i6yHYU35F.jpeg)
```

---
## \#214 Posted by: Kaloqn4o Posted at: 2019-06-13T17:04:55.566Z Reads: 126

```
Im looking ebuy and there is 47.5k and 47.5R is there any difference ![mobile|250x500](upload://fjHjnE6XPIwb8S7PHfPhUfyXyg8.png)
```

---
## \#215 Posted by: Gamer43 Posted at: 2019-06-13T19:10:51.007Z Reads: 119

```
Yes there's a huge difference, 47.5K is 47 THOUSAND five Hundred ohms. 

I would highly recommend purchasing from an electronics distributor such as digikey, mouser, or Arrow.
```

---
## \#216 Posted by: Benjamin899 Posted at: 2019-06-15T10:42:49.720Z Reads: 113

```
what do you think about lcsc? good or bad distributor?
```

---
## \#217 Posted by: Gamer43 Posted at: 2019-06-15T16:56:45.036Z Reads: 115

```
Should work, I just recommend digikey, mouser, arrow since they will most likely be able to deliver sooner and for cheaper. (Arrow offers free shipping).
```

---
## \#218 Posted by: Kaloqn4o Posted at: 2019-06-22T18:15:40.315Z Reads: 111

```
Well ive ordered 5k units from arrow and got them last night. Spent about 3-4 hours and dont get me wrong i like soldering stuff like wires, joints, motors but this tiny shit that moves in any direction i hated it. I think ive dont it double and triple checked it looks ok. I tested it on the vesc tool works. So i set it for the parameters that for sure can't handle.
Motors 55A
Brake - 45A
Batt.   30A
Regen  - 20
And left the battery on 37.5v so if they die i dont leave the battery on full
So today i went for a ride and it fricking works lol
Keda 6364 190kv are flying from start in BLDC
I feal a bit the mid to high acceleration is lower than before but that can be the battery. So im charging it to full for a test. Battery is 10s6p Samsung 35E ![IMG_20190620_185151|666x500](upload://SAWELplLDKdyGJcqgEY4OC8WaM.jpeg)
```

---
## \#219 Posted by: Kaloqn4o Posted at: 2019-07-04T06:22:10.432Z Reads: 106

```
So everything is fine until i hard ride it for 20 min then when i hard accelerate one of the motors cuts out and comes back on in 10-20sec then i can ride it again for some time like 2-5 min before doing the same. What can be the problem, overheating?
```

---
## \#220 Posted by: Schtekarsten Posted at: 2019-07-04T15:12:30.254Z Reads: 109

```
hard to say!
it could be your battery sagging/getting low or the VESC itself overheating.
Are you running street wheels or phnumatics? and what version of the vesc are you on?
If you have a bt-module you will easily be able to determine what it is.

as a reference I can fairly easily get the dual 4.20 base module up to 80+ degrees on street wheels. but then I am pretty much flooring it all the time doing 55-60 km/h every time I get a chance to. and it is the constant acceleration and braking that is causing it for me not cruising at high speeds. running 12s and 40 battery 60 motor on each side btw.
phnumatics and hard riding and you really need move up in the esc ladder. but again there are just a gazillion factors coming to play
```

---
## \#221 Posted by: Davewesh Posted at: 2019-07-08T05:04:46.659Z Reads: 105

```
So i did this and got a snap crackle and pop (no big deal cause learning) but im curious if there's a good sanity check to make sure everything is soldered correctly. 

I note that on my dual - Vesc #0 motor phase wires were reading something insanely low, like 30-40Ohms. Where as on Vesc #1 i read out 80+ (not sure what the actual value was). With that being said, what is the expected Ohm resistance on the VESC after the mod is finished - i suspect that i can use this to determine if at least one side of the VESC was correctly done or not. 

As well as look into seeing if anything was damaged and fix that along with the likely incorrectly soldered resistors.
```

---
## \#222 Posted by: Gamer43 Posted at: 2019-07-08T22:59:18.581Z Reads: 105

```
Sounds like one or more of the resistors were not soldered on completely. Make sure to use lots of flux and a well tinned iron with lead solder, I recommend tacky flux from chip quik or MG chemicals.

Visual inspection of the joint is usually enough. The resistor should be well aligned with the pads and the joint be very shiny. 

Cold or faulty joints can result in shootthrough and subsequent shortcircuit, causing serious problems. I had this happen to myself.
```

---
## \#223 Posted by: Kaloqn4o Posted at: 2019-07-12T11:45:57.080Z Reads: 97

```
Something happened with the vesc that was cutting off now shorts out when i touch it to the battery, i resoldered half of the resistors that looked bad but still shorts out. Can i remove all the resistors and see if it still shorts out without resistors so i can see if the problem is somewhere else
```

---
## \#224 Posted by: Gamer43 Posted at: 2019-07-13T00:33:28.539Z Reads: 95

```
MOSFETs failed.

Continuity test each phase with vcc and ground.
```

---
## \#225 Posted by: Kaloqn4o Posted at: 2019-07-13T07:05:14.911Z Reads: 93

```
Any chance you have a picture of the mosfets
```

---
## \#226 Posted by: Komamtb Posted at: 2019-07-18T11:52:02.198Z Reads: 90

```
what amps can it still do safely without the resistor swap?
```

---
## \#228 Posted by: Komamtb Posted at: 2019-07-18T12:35:45.913Z Reads: 90

```
well in my case I will use it on a regular hub cruiser, maybe 15amps per motor max, not sure if I should go threw all the hasle of finding someone to change them.
```

---
## \#229 Posted by: Schtekarsten Posted at: 2019-07-18T12:37:34.409Z Reads: 94

```
when did you get the vesc btw? and from where? what model is it? and what is you battery and motor setup?
```

---
## \#230 Posted by: Komamtb Posted at: 2019-07-18T12:43:17.855Z Reads: 93

```
![IMG_20190718_154140|375x500](upload://hL2WbernkNedYvLEDGKp7MQYx4V.jpeg) 

I bought it new, but from a user, no idea of the exact model. It will be used with 10s3p 30q pack on meepo 1.5 hubs.
```

---
## \#231 Posted by: Schtekarsten Posted at: 2019-07-18T13:11:02.093Z Reads: 93

```
yeah looks like it is and old dual 4.20 with 4R7 (4.7 ohms = old shit) resistors, the pictures zoomed out so I can't see properly . Cutouts will be there my friend I have riden a 10s4p 30q with china hubs for like 4-5months with the cutouts so you should be fine and you will learn after a while when they occur and what the limit will be at. 
and depending on temperatures and so on the hubs are real easy to cook. as a reference 24 battery and 40 ish motor. and a ride longer than 7-8 km going full throttle everywhere 83kg and you will have the motors heat up to the point where the urethane sleeve goes lose from the heat 20c° outside temp. I'm rocking a infra temp sensor for like 20 dollars. and you want to stay below 65c° really or the urethane goes soggy and lose, which creates more drag and heats up the motor even more.

up to you but the resistor swap is not that hard to do tbh. watch my video regarding the swap. and a few others regarding soldering and get your hands on some decent tools and you are golden. 
unfortunately arrow doesn't have free worldwide shipping anymore. 

but it is fine on that setup really. the hubs are a pretty close second bottleneck in terms of continues. sure the cutouts are more geared towards the acceleration and from slower speeds so two different kinds of bottlenecks. I guess. but it will get you from point a to b and do 37+ km/h. 12s is more nice on these hubs if you like some more speed. but then again you will consume the selves alot quicker through heat

I would go for something like 20A battery max 35-40 motor. hybrid/sensored or senseless FOC, change the switching frequency to 25-30kHz (FOC --> advanced tab), and positive ramping time to 0.4-0.5sec. And then play around with the settings from there. be mindful of the hub temps. if you can't hold onto the outside aluminum plate of the hubmotor with your palm pressed to it for more then like 5 sec you know you are pushing it. and they will be crusty from water ingress and other shit aswell and are quite cheap to replace so for it. but you wont have a rocketpoweredmurdermachine under your feet either way, but pretty dope non the less.
```

---
## \#232 Posted by: Schtekarsten Posted at: 2019-07-18T13:23:08.271Z Reads: 91

```
there is also a massive difference in the heat capabilities between the 4.20 versions. de regular dual and single 4.20 being at the bottom the old 4.20 plus in between and new dual 4.20 being quite fucking amazing. main differences being the mosfets used: 628 --> 612 --> dual rows 628. For reference I'm rocking 12s4p 30q, dual 6355, 40 battery, 60 motor on my prototype boards and I'm going at least 55km/h everywhere possible and probably at places where I shouldn't... I'm quite the wind resistance at 192cm strait always strait legging it at 83 kgs. and I'm normally sitting between 60-65 C°. and it is summer here in Sweden so not freezing anymore 20-25c and sitting siliconed into and airtight enclosure.
Btw i will have some pretty dope boards coming out of my parents garage in a few months just saying :v:
```

---
## \#234 Posted by: Schtekarsten Posted at: 2019-07-18T13:37:23.157Z Reads: 90

```
idk should we start a thread regarding this stuff on the forum.esk8.new site as well as it seems that place is way more active now?
```

---
## \#235 Posted by: jun1208 Posted at: 2019-07-18T16:02:52.885Z Reads: 92

```
I think you guys should go for it man :+1:
It's much active there compared to here..
```

---
## \#236 Posted by: Waiboard Posted at: 2019-08-08T22:24:34.572Z Reads: 80

```
Hello @Schtekarsten @Gamer43 @chrischo1996
I am configuring my VESC 4.20 plus but I still have cuts. I bought it in May, so you already have the update of the resistors and capacitors of March.
I read all this thread (also others in the forum about this), but I can't keep my board from working properly.

My board has two Flipsky 6054 190KV / VESC Flipsky dual 4.20 plus / 10s4p 25r engines with BMS 100A for loading and unloading.

I start walking a few meters at low speed, increase the speed a bit and get a cut. I turn it on again, I do a few more meters and it almost does not matter if it is at low or high speed since it is cut again.

I tried the settings that Flipsky recommends:

    Current Max Motor: 30A
    Current Max Brake Motor: -25A
    Absolute Maximum Current: 130A
    Slow ABS Current Limit: True
    Battery Current Max: 30A
    Battery Current Max Regen: -25A
    Current Limit
    16

I also tried:

    Current Max Motor: 50A
    Current Max Brake Motor: -50A
    Absolute Maximum Current: 130A
    Slow ABS Current Limit: True
    Battery Current Max: 60A
    Battery Current Max Regen: -55A
    Current Limit
    16

I would like to know if I am doing something wrong? I don't understand why I get cuts?
```

---
## \#237 Posted by: Gamer43 Posted at: 2019-08-10T02:56:24.457Z Reads: 72

```
Were you able to see what the faults were exactly?

What advanced VESC settings are you running?

FOC?
```

---
## \#238 Posted by: Waiboard Posted at: 2019-08-10T03:40:59.411Z Reads: 72

```
@Gamer43
I am testing the configuration:

    BLDC
    60A (Flipsky 6354 engines can receive 65A maximum current.)
    -50A (I feel comfortable with a -50A brake for how little I can walk before the cuts begin.)

    25A
    -4A

I was reading a lot and analyzing each option and according to what I understood, my battery can deliver 60A (maybe 80A) of direct current. And be regenerated in a 4A peak.

Then I should give a maximum of 30A to each VESC, but it would be better to put a value below so that it has margin. That's why I chose 25A.

Just tomorrow I will be able to go out to test if everything is going well. But according to your point of view, am I correct with this configuration?
```

---
## \#239 Posted by: Gamer43 Posted at: 2019-08-12T03:02:21.491Z Reads: 65

```
Hey, sorry for the delays in replies.

Yes, those current settings should be fine. If you are still getting cutouts, please let us know. If so, try to provide additional detail on the cutouts, such as exactly which fault the VESC is throwing and conditions the fault is thrown.
```

---
## \#240 Posted by: MiniChopper4Me Posted at: 2019-08-14T12:41:27.457Z Reads: 65

```
Waiboard,

If when the cutout happens, you need to turn off and back on again in order to get it working, I would suggest checking your battery.  I had this issue and this is what was going on for me.  My battery had been made with the BMS protecting discharge, even though I had asked for it to be bypassed.  Whenever the VESC would pull more than 20A, it would shut off and I would have to power off/on (in my case with a loop key, and I’m sure I killed a few anti-spark switches with this problem) in order to run again.  Also, I could readily reproduce the problem by hard accelerating/brake to draw alot of amps.

Edit: Nevermind, I see you built your battery.  I’d suggest checking the output voltage when the shutdown occurs.  If your VESC shows no input voltage, your BMS may be no good.

Unless you made the battery yourself, I suggest cutting the battery shrink a little so that you can see where the wires are connected to the BMS, and you can always seal it back up with tape when you’re done provided you are careful while cutting the wrap.
```

---
## \#241 Posted by: Waiboard Posted at: 2019-08-16T02:51:17.639Z Reads: 62

```
I have already been able to solve my problem of cuts. The subject was in my battery. The company where I sent to build my battery did it without having previously measured the cells. My BMS has the bluethoot connection option to verify all values, that's when I see that two cells were unbalanced. At that time I did not give so much importance because I considered that the BMS could balance it automatically (thinking without experience in BMS). One of them marked approximately 3500mv while the other 3300mv. So when charging my battery, the BMS made a voltage detection by firing the protection by individual high voltage cell when reaching the value 4250mv for that cell. While the others were just at 3700mv. At the same time the app has a strange way of responding, because at the time that alarm / protection was triggered the total value went to 100% but in reality the battery had just over 35%. That made when the speed and braking tests went out, the motors consumed the current set in the VESCs but the battery did not have that current stored. By triggering another alarm / protection and turning off the VESCs.

Conclusion: all these errors made me know much more about my battery, my VESC, my BMS and its app. So I do not see what happened so badly, beyond time and the frustration of the moment.
```

---
## \#242 Posted by: Randy_bobandy Posted at: 2019-08-16T07:50:57.435Z Reads: 60

```
So do the new 4.20 duel plus fsesc have any cut out issues? I got mine in early july and have been riding it plenty hard with absolutely 0 issues. I am running 10s5p 30q cells on 6.5" pnumatic with duel 6355 flipsky motors. It's actually my girlfriend's board as I'm still waiting for my parts(I'm running 12s5p 30q with the duel fsesc 6.6 plus). According to the vesc app I have gotten the motors up to 110amps and around 2300w going up hill with no problems. I'm very happy with this vesc so far. My only issue is the voltage display in the vesc app is sporadic and jumps around + or - 8% or so. I think it's something to do with flipsky vescs because my old board did the samething and it had the older large fsesc 6.6. I expect my new 6.6 will do it as well. I know the voltage is stable and just the way it reads on the app since it looks fine with my multi meter.
```

---
## \#243 Posted by: ADrum707 Posted at: 2019-09-18T17:48:51.227Z Reads: 40

```
After sitting for a few months (3-4), my board doesn't perform the same. The battery stayed charged, however, I've got inconsistent performance from the controller and motors. Should I just re-program? Or could there be a different issue going on?
```

---
