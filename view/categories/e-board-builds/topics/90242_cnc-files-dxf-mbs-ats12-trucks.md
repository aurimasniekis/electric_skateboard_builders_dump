# Cnc files dxf mbs ats12 trucks

### Replies: 33 Views: 1101

## \#1 Posted by: Toby-Aus Posted at: 2019-04-12T09:25:11.170Z Reads: 202

```
Hi this is my first build. I have access to a cnc router so will be designing and cutting parts for my build. i plan on making pullys, motor mount, and a sealed focbox heatsink enclosure.
I will list all my cut files .dxf if anyone is interested in makng there own. but i would also love any files that people may already have that i could use.
Thanks Toby 

https://www.dropbox.com/sh/to1r10s8xo1ltaq/AADiRlMfGyQ3t6Z5GkHobKNea?dl=0


![PT1|500x500](upload://H3a3brijv8gvqq6whUoHoEkmgy.jpeg) 

MBS mountain board Core 94 

ATS12 trucks 

Fivestar mbs hubs


WINNING 2.4Ghz mini remote

Race star 5065 140kv  may change will see how they perform

5m 9mm 450mm belt

Focbox esc 

Flpsky anti-spark switch (not going to use this now too risky)

6s or 12s not sure on battery setup yet


been prototyping these cogs getting the holes to fit the hubs
![56780988_2178864138873371_3825260253646159872_n|690x388](upload://5rOnqnEUxeFvrokBsLoy93HDDdT.jpeg)

dxf files for pully

https://www.dropbox.com/sh/to1r10s8xo1ltaq/AADiRlMfGyQ3t6Z5GkHobKNea?dl=0

Got the focbox running smoothly with vesc tool. but may have bricked one of them. uploaded the firmware for the wrong hardware need to see if it can be reversed.

Anyone in Newcastle Australia let me know
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-12T10:12:28.161Z Reads: 178

```
this here is a similar project and might help you with some of your thoughts

https://www.electric-skateboard.builders/t/wenzani-mbs-core-16-mbs-matrix-trucks-10sxp-rest-is-still-unknown/82405?u=andy87
```

---
## \#3 Posted by: Andy87 Posted at: 2019-04-12T10:15:07.554Z Reads: 169

```
[quote="Toby-Aus, post:1, topic:90242"]
uploaded the firmware for the wrong hardware need to see if it can be reversed.
[/quote]

yes it can. search for st v2 link (or stl V2), but you will need to solder the header on the pcb of your focbox.
I think with the newest FW you can upload a slave vesc via CAN, so that might be an option as well and you don´t need a STL V2 link and no header soldering. Disclaimer, I never tried the last one by my own.
```

---
## \#4 Posted by: Toby-Aus Posted at: 2019-04-12T12:59:33.283Z Reads: 150

```
i can still connect to it with vesc tool but the firmware for the other hardware is no longer accessible. Tried uploading the firmware version from bldc tool  but it terminates before it finishes.
```

---
## \#5 Posted by: Andy87 Posted at: 2019-04-12T13:02:58.653Z Reads: 144

```
Try to follow this instruction 
https://vesc-project.com/comment/225#comment-225
```

---
## \#6 Posted by: Acido Posted at: 2019-04-12T13:20:23.149Z Reads: 147

```
Flipsky anti spark switches are crap, dont go with one as it wil fail sooner or later

The best switch is one built in the bestech bms or one in the unity vescs
If you do not have any of those parts in your build go with the Fatboy switch as it was smarter than the others
```

---
## \#7 Posted by: Toby-Aus Posted at: 2019-04-12T13:29:15.816Z Reads: 140

```
thanks. Shit just bought one not cheap
```

---
## \#8 Posted by: Toby-Aus Posted at: 2019-04-12T13:31:45.431Z Reads: 136

```
how do they fail do they cut out. not like they will damage anything
```

---
## \#9 Posted by: RedBaron Posted at: 2019-04-12T16:06:38.017Z Reads: 127

```
I've seen a few of the flispky antisparks fail right infront of me. The antispark gets hot and either melts or catches fire. One of the guys was going full speed when his failed and his motors locked up immediately and he ate shit pretty hard. Ontop of that half the stuff inside his case caught fire aswell.
```

---
## \#10 Posted by: Toby-Aus Posted at: 2019-04-13T02:26:32.724Z Reads: 114

```
Oh shit so not even worth trying it out. too risky wow
```

---
## \#11 Posted by: Toby-Aus Posted at: 2019-04-13T02:38:15.854Z Reads: 115

```
Stage two motor mount.
Manadged to profile the axel acuratly by tracing one of the other mounts found from a pic on the net.
![20190413_095531|281x500](upload://b3JUv2HvEFOHw9kvYgnUbHGFDz.jpeg) 

![20190413_095556|690x388](upload://7DCNzjfV50QPQK3PyGkIdHAPD5J.jpeg) 

Continued to design the mount. Yes its acrylic and the mount is a bit thin this is just for prototyping.

![20190413_115505|690x388](upload://bIKFPMEdTnuSnHwl0ioFLSwRruw.jpeg) 

Discovered a prob with the clamp on the axel, because the axel tappers ie not same thickness its harder ro set the clamp square.

![20190413_122447|281x500](upload://mrRqsvrpD9gf0Ws1bdVfydKpnZ9.jpeg) 

Iv seen other designs have lots of cros bars spreading between both motors prob to keep them square to the wheels. But i dont like the looks. Looks very cluttered.

https://www.dropbox.com/sh/to1r10s8xo1ltaq/AADiRlMfGyQ3t6Z5GkHobKNea?dl=0
```

---
## \#12 Posted by: Acido Posted at: 2019-04-13T16:17:42.260Z Reads: 92

```
Mine turned in to a 5x3cm resistor...
And with 2+kw of power thats a serious problem
```

---
## \#13 Posted by: Toby-Aus Posted at: 2019-04-17T06:48:49.696Z Reads: 93

```
Time to cut 

![20190415_190251|690x388](upload://vHTYNOT9bTNgqdlkztKVjCqW6FH.jpeg) 

![20190417_164039|281x500](upload://16O0MqpIIA8Zeyrr6ZdvDfOZoHE.jpeg) 

Got the belts and batteries today. 
The tattu batteries are beasts.
 ![20190417_164019|281x500](upload://4ldsMrLejMJ0YgaPiFpD6Ud8rkW.jpeg) 

![20190417_123310|690x388](upload://9CYS6TXxNMAMSt0Tn1MjTkLCr9.jpeg) 


Still need to 

design focbox heatsink and waterproof box.

Batt box that is small but durable to protect batteries.

Motor mount -fit belts with a baring for tensioning.
```

---
## \#14 Posted by: Toby-Aus Posted at: 2019-04-17T10:41:24.210Z Reads: 91

```
**Focbox**

 iv started on the heatsink. Using these dimensions as well as measuring the focbox
![image|481x407](upload://8k1UJ5vbAPSsJVGN70rdFP4BLnD.png) 

![image|594x500](upload://hF1ChZg7dyHOqofn1GBj0WcQulf.png)

![image|690x375](upload://yeUF6830LxU8uq2PqSJzXQOGTsW.png) 

![44|281x500](upload://o1e0cltBDrbENY9mI9VuYeo6kUX.jpeg) 

![58|690x388](upload://2olSASgG974SIiMRErCzvuNXfHh.jpeg)
```

---
## \#15 Posted by: Toby-Aus Posted at: 2019-04-18T12:55:43.865Z Reads: 84

```
OK

So looked up the esk8 calculator and my max speed was going to be 43kmh. Thats just a bit fast. So recalculated for around 30kmh. so redid puleys using traceparts.com (files need work as they have been modified so they are not complete shapes).

Now using 14tooth pully on motor and 90tooth on 200mm wheel
 
![20190418_163038|690x388](upload://dMNl1mqlVrXN9PHwd1y7iG2BPTu.jpeg) 

http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:12,%22motor-kv%22:140,%22system-efficiency%22:85,%22motor-pulley-teeth%22:14,%22wheel-pulley-teeth%22:90,%22wheel-size%22:200}|


https://www.dropbox.com/sh/to1r10s8xo1ltaq/AADiRlMfGyQ3t6Z5GkHobKNea?dl=0
```

---
## \#16 Posted by: Toby-Aus Posted at: 2019-04-19T04:55:43.192Z Reads: 81

```
Motor mount

![20190419_130634|690x388](upload://j4u0aJDAnC3NEAJAop3evV1USyv.jpeg) 

![20190419_130645|690x388](upload://3oS3Tl54QCHI6erRQlqAFR2Qja0.jpeg) 

![20190419_143652|690x388](upload://yfTGDpeUWzDcgRN3q6JtMt5jLfs.jpeg) 

![20190419_143702|281x500](upload://4aqyd07Yn7GLHV3YV2wfxF0HBL.jpeg) 

![20190419_143728|281x500](upload://epZiYSAMRakkelvyydrxORZIM6j.jpeg) 

Need to get longer belts now but thia will work right :)
```

---
## \#17 Posted by: Toby-Aus Posted at: 2019-04-23T09:26:54.969Z Reads: 73

```
ok got new belts today fitted everything and found issues with the motor and the wheel not being square to each other and so the belt driving off the pulley. Going to try changing the axle clamp to grub screws trying to square them to the flat faces on the trucks.
```

---
## \#18 Posted by: Toby-Aus Posted at: 2019-04-25T11:02:44.443Z Reads: 71

```
Ok slight design change still using the truck frofile but instead of clamping it using grub screws. Iv removed the black spacer that goes before the wheel and replaced it with a spacer that i can screw to so now the motor mount is square to the wheel and is clamped on using the wheel and held from rotating using the profile of the truck. Easier to show than tell.

![image|690x231](upload://2KttQFf2RMfIgMfTBo8dGGANA2I.png) 

![20190425_162809|281x500](upload://6KkorD0Ol0xkf9JQ7P5xHUWhoGC.jpeg) 

![20190425_162710|281x500](upload://uigdlR21cKWL2IRpcT8ySmAMr7m.jpeg) 

![20190425_164538|690x388](upload://futKAT6besheCVKHbc2sdCKi68q.jpeg) 

![20190425_170541|690x388](upload://2tST0RQ9bJHHYGJ4vh4mM1mRukJ.jpeg) 

![20190425_170545|690x388](upload://oko9u6ZCP1W7t3gzC3RJ9LhoSxO.jpeg) 

Im verry happy had it running on and old 6s half of my final build. Anticipating thr power. 

https://youtu.be/WX7iqyJHDLg

Next stop box for electronics.
```

---
## \#19 Posted by: Toby-Aus Posted at: 2019-04-29T12:57:24.075Z Reads: 65

```
Focbox time

Iv been riding around on the single motor and pushing it quite hard (gets very hot) but have found that the esc never gets very hot so instated of doing an elaborate heat-sink with fins and such, im just going to go with this for now.

![58978265_432011897563401_3078121705772679168_n|690x388](upload://qxJKrlRsidrGSLyouRIatgS4Dfp.jpeg) 

![59295822_625335811213566_1822051721124249600_n|690x388](upload://8SBimP7ELlGp6NasrpX4HtXQvNM.jpeg) 

Dont have alot of space but hopefully i can keep it tidy and fit it all in.
```

---
## \#20 Posted by: Toby-Aus Posted at: 2019-05-03T08:33:11.041Z Reads: 63

```
Progress on the battery box. Got the box all wired. Waiting for 2 lcd ballance checkers that ill wire in permanently they have built in balancing will test. Might not need to use my ballance charger then.

Now to wire up the focboxs
![20190503_181337|690x388](upload://5r6hjGwj6gXAX4FF6BEJcQ7iJqz.jpeg) 

![20190503_181409|281x500](upload://wfXqeZ3oBxJkCTrrTipXcMtLHeo.jpeg) 

![20190503_182149|690x388](upload://hxrrJBbPtM548pSeIOgspvd97xq.jpeg) 

![20190503_182152|690x388](upload://oemLYe5LO2pwWKiMb0fqr9mfepM.jpeg)
```

---
## \#21 Posted by: Andy87 Posted at: 2019-05-03T13:43:53.584Z Reads: 57

```
Do you have a link to the Balance checker?
```

---
## \#22 Posted by: Toby-Aus Posted at: 2019-05-03T13:49:33.870Z Reads: 56

```
im really not expecting much out of them as they are the cheapest on the market 

https://www.aliexpress.com/item/IMAX-B6-80W-Li-Po-NiMh-Li-ion-Battery-Balance-Charger-15V-6A-AC-Power-Adapter/32799780534.html?spm=a2g0s.9042311.0.0.1b4b4c4d4i0bF5

these are probebly the better option but a bit more pricy

https://www.aliexpress.com/item/ISDT-BattGo-BG-8S-Smart-Battery-Checker-Balancer-Receiver-Signal-Tester-Quick-Charge-Function/32982486258.html?spm=2114.search0104.3.1.10b73c5bA2umGq&amp;ws_ab_test=searchweb0_0,searchweb201602_9_10065_10130_10068_10547_319_317_10548_10696_453_10084_454_10083_10618_10307_537_536_10131_10132_10133_10059_10884_10887_321_322_10103,searchweb201603_51,ppcSwitch_0&amp;algo_expid=a17999a0-6bae-47dc-a83e-00acdd14b474-0&amp;algo_pvid=a17999a0-6bae-47dc-a83e-00acdd14b474
```

---
## \#23 Posted by: Andy87 Posted at: 2019-05-03T14:04:43.672Z Reads: 52

```
Thx! Those are the ones I expected.
```

---
## \#24 Posted by: Toby-Aus Posted at: 2019-05-04T10:02:34.813Z Reads: 47

```
Somewhat finished just need second motor and install wider belts.

![20190504_174806|690x388](upload://icuwfMFBHbHCZ6Lww47nKXd0kps.jpeg) 

![20190504_174222|690x388](upload://bnfcZgh0D0HuAKIOVIYVAKbgm1y.jpeg) 

![40|690x388](upload://lZINquQwQoFBxBH8vQoFq5AdIzV.jpeg)
```

---
## \#25 Posted by: Toby-Aus Posted at: 2019-05-05T02:56:13.010Z Reads: 45

```
Trip around newcatle 11km and used 60% battery  12s 9ah. Very happy

![20190505_105426|690x388](upload://pDPoKhgzKmqv81zBf9AF5WOGaAg.jpeg) ![20190505_105420|690x388](upload://8rs1n3std3knMteeHHfQrG3x1SL.jpeg)
```

---
## \#26 Posted by: TovinoThomas Posted at: 2019-05-05T06:08:31.777Z Reads: 45

```
I have a backfire Ranger X1 which I love to bits but the deck is too flexy for my weight. I'm looking to do a deckswap and I could use all the advice I can get. I talked to a local skate shop and one of the owners was willing [Sarkari Result](https://sarkariresult.onl/) to help me out and his main concern was [Showbox](https://showbox.bio/) that the wires go through the deck.How do I route the cables outside the deck after the swap while maintaining the waterproofness of the board? Also what sort of gaskets should I buy?
```

---
## \#27 Posted by: Andy87 Posted at: 2019-05-05T06:24:10.760Z Reads: 46

```
I‘m not familiar with the ranger, but I would probably drill two holes big enough for 10awg silicon wire, route the wires out and seal it up with silicon or sikaflex after. You can use something like this to protect the wires

https://s.click.aliexpress.com/e/bRGKbdkO

It will not protect 100% but better than nothing.
If it’s a stiff deck you could get a plastic cable channel from your local hardware shop and route the wires through as well.
Depending on the thickness of your deck you could also do it like it was before. Drill through the deck, cut small channels from the top and use braided copper wires which I would than would cover with some sealant and griptape.

There are a lot of opportunities. If you do one of that above I think you also need no new gasket. If you do you can get something like this:


https://s.click.aliexpress.com/e/bq2rlUZM
```

---
## \#28 Posted by: Toby-Aus Posted at: 2019-05-05T10:00:56.556Z Reads: 44

```
you can get breaded heatshrink 
https://www.jaycar.com.au/braided-heatshrink-sleeve-30mm-x-1-2m/p/WH5626
```

---
## \#31 Posted by: Toby-Aus Posted at: 2019-05-05T10:12:47.283Z Reads: 44

```
![19e6c025db54d979b5cfdbcc63082267|690x460](upload://zbTpbZlpFKEbomxXJB0pbwAuQFF.jpeg) 

i assume
 you are talking about the wire that goes between the battery and the control box. the cables must be recessed in the board. when u get the new deck put the cables on the outside and cover them in heat-shrink. you will prob have to do some soldering to pull out the wires from the old board??
```

---
## \#32 Posted by: Toby-Aus Posted at: 2019-05-05T10:30:47.810Z Reads: 42

```
updated files 
12mm aluminium 
![image|690x494](upload://nRAbVd0wLzKcrgxfKsMkyK1VReA.png) 

bottom plate 3mm aluminium, sides and top 6mm polycarb
![image|690x320](upload://mDxGfajo5tJT3E6KN1movDmejUG.png) 


bottom and top plat 3mm aluminium sides 6mm polycarb with depth cuts reducing sections down to 2mm
![image|690x215](upload://lFSvFN1huNhm8brOAOBF4OvxKnK.png) 


12mm for the left 2 and 6mm i think for the other 2 maybe 3mm for the small spacer
![image|690x300](upload://1ZOJAbaCRBUFyMYo89hykjmVchh.png) 

https://www.dropbox.com/sh/to1r10s8xo1ltaq/AADiRlMfGyQ3t6Z5GkHobKNea?dl=0
```

---
## \#33 Posted by: Toby-Aus Posted at: 2019-05-05T12:01:10.161Z Reads: 38

```
https://www.youtube.com/watch?v=C8n8ceZM9qY

i like how this guy uses breaded cable
```

---
## \#34 Posted by: Toby-Aus Posted at: 2019-05-18T13:08:59.008Z Reads: 34

```
Got second motor in the post wow so much more power. double you might say :)

https://scontent.fsyd3-1.fna.fbcdn.net/v/t1.0-9/60340476_2235432843216500_917417362456576000_n.jpg?_nc_cat=101&_nc_ht=scontent.fsyd3-1.fna&oh=c7a458818d71600100c0eeb2a8821c20&oe=5D5C9F89

so got partway through cutting the 90 tooth pulleys and the last metal cutter broke. couldnt wait had to ride it so did other half out of acrylic. will recut latter. 

https://scontent.fsyd3-1.fna.fbcdn.net/v/t1.0-9/60515691_2234882266604891_888718833366335488_n.jpg?_nc_cat=100&_nc_ht=scontent.fsyd3-1.fna&oh=e3a92c4b491285ba9377187792106fd3&oe=5D9C696F

went to 15mm belts and removed the belt tensioner now swinging motor out to tighten belt.
```

---
## \#35 Posted by: TovinoThomas Posted at: 2019-10-03T14:44:33.004Z Reads: 10

```
[quote="TovinoThomas, post:26, topic:90242"]
I have a backfire Ranger X1 which I love to bits but the deck is too flexy for my weight. I’m looking to do a deckswap and I could use all the advice I can get. I talked to a local skate shop and one of the owners was willing [url=https://www.55printing.com/news/printing-and-mailing-holiday-cards-online/]print holiday postcards for mailing[/url] to help me out and his main concern was  that the wires go through the deck.How do I route the cables outside the deck after the swap while maintaining the waterproofness of the board? Also what sort of gaskets should I buy?
[/quote]

Thank you my issue has been solved,...
```

---
