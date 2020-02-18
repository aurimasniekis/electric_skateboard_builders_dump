# Final parts check before order- 1st build, another vanguard

### Replies: 38 Views: 625

## \#1 Posted by: wwohl602 Posted at: 2019-08-13T10:34:43.327Z Reads: 126

```
Hi Esk8 builders community,

Been reading and researching for quite some time. Could use a second set of eyes before i commit to a few things. There’s a ton of great info here, but the esk8 world is exploding and information gets outdated very fast I’ve learned. 

Purchased an Ownboard W1A in May as a way to get started and have been riding it as my full time commuter in Philadelphia ever since! It’s far from stock because the road vibrations made it nearly unrideable. Currently running 50/44 calibers, a 36” maple deck from amazon and it will remain a commuter for me. I’d like to pick up a new deck to further improve ride quality in the future. [image|375x500](upload://3VEQ43C0IQWIrFMbr4l4eB0O8l2.jpeg) ![image|374x500](upload://54Ozj03q3Ldz13rfT2VWWjmFgHc.jpeg) 
 
I live in Philadelphia and the streets are pretty rough here. Top speed isn’t a priority for me, the 22mph top I have now is too much for these road conditions and a 36” deck in most places. I’m really looking for the bottom and midrange torque and ride comfort. 

I plan to get a new deck, maybe something bamboo to continue improving ride quality for that board as it will remain a commuter. Might even upgrade the ESC if it’s worth it. 

Anyways, I’m ready to start building my second board and could use some help. It’s funded and just waiting for me to hit purchase. Here’s what I have so far:
Vanguard flex 2

Caguamas and 90mm ABEC clones,  caliber 50/44s

Boardnamics mounts 

60 - 30q cells, planning a 3 or 4 p build at 10S
Will 3D print the housings/enclosures

Here’s what Im looking for some reassurance on:
**Torque boards 6354 190kv motors** - these seem to be the highest torque of the 6354s and are sensored.  
Since I’ll be running 85 to 90mm wheels, was thinking 15t motor pulley and 36t wheel. 
**VESC**- eyeing the Flipsky 4.2 and 4.2 dual, any opinions on individual vs dual? There’s so much info- but I believe 4.2 cutouts are limited to 12s and these don’t have the problematic integrated anti spark switch. 
**Antispark switch** - need a recommendation that’s reliable and affordable. 
**BMS**- have seen several, would like to be able to charge at higher than 2A. Still wrapping my head around wiring one that bypasses discharge. 

**Really appreciate your time everyone** as well as all of the great information and support here. 

Eager to get started on this thing. Can’t wait to ride on the flexy deck at faster than kick speed. 

Thanks again 

Bill
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-08-13T11:48:45.084Z Reads: 107

```
You're on track for a decent building so far, I would go straight to 77a Cags over any ABEC clone and possibly a larger wheel if you can (TB 110mm, ABECs, Popocas 90mm, BKB 97mm), TB6355 motors are pretty good and will get you reliable power, the FSESC 4.20 isn't bad as long as you stay at 10s but it's slightly more reliable to get 2 single ESCs and run split PPM.

If you are using the ownboard ESC it needs to be a hub motor or the erpm will be way off

Alternative is get the BKB kit and deck swap it, it's a hella nice kit with a good balance of parts at a great price
```

---
## \#3 Posted by: wwohl602 Posted at: 2019-08-13T13:32:25.620Z Reads: 88

```
Saw the BKB and several others. Even considered the ownboard w2. 

Appreciate the feedback. I’ll order individual VESCs (kinda wanna try them on the ownboard one day too 🤣) as well as the TB motors.
```

---
## \#4 Posted by: rusins Posted at: 2019-08-13T13:53:00.547Z Reads: 87

```
I prefer my 77a caguamas over popocas. At 22mph you have the reaction time needed for bad roads. (That said though I'm upgrading to pneumatics, but mainly because I want to ride in the rain and go fast)

Keep in mind that on standard calibers dual TB 6354 motors will only fit 12mm pulleys.

As for an antispark – it's worth just getting a beefy BMS with discharge and integrated e-switch. Those work reliably, unlike all anti-spark switches on the market currently.
```

---
## \#5 Posted by: captclearleft Posted at: 2019-08-13T15:45:53.334Z Reads: 76

```
I have had good luck with these anti-spark switches:

https://www.electric-skateboard.builders/t/vedder-anti-spark-switches-for-sale-from-18/31847

I use the [Torqueboards Vesc 4.12's](https:///collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller) I have a dual setup 12s, and single setup 10s.  Never had any issues.

Your pulley setup sounds good - That is a standard setup.
```

---
## \#6 Posted by: pundahh Posted at: 2019-08-13T18:19:51.318Z Reads: 67

```
[quote="wwohl602, post:1, topic:100190"]
**Antispark switch** - need a recommendation that’s reliable and affordable.
[/quote]

XT90s loopkey is reliable & cheap as $!@%. I use a bestech d140 for the bms charging at 4a. good luck with the build!
```

---
## \#7 Posted by: wwohl602 Posted at: 2019-08-13T19:55:15.190Z Reads: 60

```
I think the 12mm belts should be fine. I can always pick up an e caliber in the future 

So better to just buy an adequate BMS to discharge through? And the 77a cags is what I have

Realizing I need to pick up a remote too. Might grab one from flipsky
```

---
## \#8 Posted by: rusins Posted at: 2019-08-13T20:08:01.023Z Reads: 58

```
Yes, until @3DServisas resume selling their anti-spark with proper inrush current handling, BMSes with e-switches (or just loop-keys) are the way to go.
```

---
## \#9 Posted by: rusins Posted at: 2019-08-13T20:13:40.382Z Reads: 62

```
Ah nvm, looks like it is available again:
https://shop.3dservisas.eu/collections/fatboy-antispark-switches/products/fatboy-mini-sparky-switch-50a-200a-100v-pre-charged-anti-spark-switch-with-push-to-start

Also Pryside has one in development.

But as you can see from the price, just getting a BMS with an e-switch makes more sense for you.
```

---
## \#10 Posted by: wwohl602 Posted at: 2019-08-13T22:18:54.703Z Reads: 56

```
[quote="pundahh, post:6, topic:100190"]
bestech d140
[/quote]

Ill order a BestTech d140 then

Gonna order the BMS, VESCs and motors tonight. Might get the pulleys from TB as well while im there

Any remote opinions? Flipsky Vx1 maybe
```

---
## \#11 Posted by: pundahh Posted at: 2019-08-13T22:40:53.526Z Reads: 51

```
That BMS is charge only & has no switch by the way. I use xt90s since its only a few bucks and works well. BKB sells the bms if you want to buy from the US

I like the VX1 remote, battery life is a bit poor but you can swap a bigger one in. 

@dickyho  also sells some quality & cheap pulleys. Good value if you want to get a few different wants and play around with gearing ratios.
```

---
## \#12 Posted by: yulaw2k Posted at: 2019-08-13T22:48:11.258Z Reads: 52

```
Flipsky should be having a sale this week.  So I'm buying all my parts from them this weekend. They told me to keep an eye on their website....
```

---
## \#13 Posted by: wwohl602 Posted at: 2019-08-13T22:51:21.509Z Reads: 48

```
[quote="pundahh, post:11, topic:100190"]
1 remote, battery life is a bit p
[/quote]

good to know!
```

---
## \#14 Posted by: wwohl602 Posted at: 2019-08-13T22:51:44.630Z Reads: 47

```
Is there a better BMS? Or can I just run any switch on that BMS
```

---
## \#15 Posted by: pundahh Posted at: 2019-08-13T22:54:06.631Z Reads: 49

```
You can run any switch since it doesn't connect to the BMS, just somewhere in the circuit. Bestech one is reliable, cheap & compact.
```

---
## \#16 Posted by: pundahh Posted at: 2019-08-13T22:54:48.844Z Reads: 49

```
:o thanks for the info i'm thinking of picking up an esc. guess i'm blowing more money this week
```

---
## \#17 Posted by: wwohl602 Posted at: 2019-08-14T05:15:36.949Z Reads: 43

```
![d952acba62e54f9e530d54406bb4299e_1200x|500x500](upload://jYqSEC2xPDg6YyHdDeeZAPkxNHx.jpeg) 
Picked up a new deck for my daily driver board

Have the 6355 190KV motors from Torque Boards in my cart and ready to order. Before I pull the trigger, any options for more affordable pulleys? They offer a 15t/36t combo that will cost me $100 for both sides, which seems like a lot
I have the option of 3d printing the wheel pulleys. All in all it will probably only save me $50, but didn't want to overlook other options
```

---
## \#18 Posted by: pundahh Posted at: 2019-08-14T06:08:11.143Z Reads: 40

```
I think I mentioned earlier @dickyho pulleys. Cheap and quality, rare to come across.

If you message him he waives the eBay fees, comes to about $16 per wheel pulley iirc and $2 for aluminium motor pulley. Steel ones are somewhere $5-8? 

Cheap belts too, $2 per. Only thing is shipping is from China so would be more beneficial if there’s other things you want to pick up from his shop.
```

---
## \#19 Posted by: wwohl602 Posted at: 2019-08-14T06:22:46.385Z Reads: 39

```
Thank you. Had just read that and forgot what thread it was in 🙈 what I get for trying to think on nightshift 

I’ll reach out to him and get the pulleys from him. 280mm belt should work with the boardnamics mount? That’s what comes with the TB setup. They’re cheap through him as well
```

---
## \#20 Posted by: pundahh Posted at: 2019-08-14T06:27:39.978Z Reads: 38

```
Are you using idlers? My friend is running the mount no idlers with 15/36 gearing and uses 270mm length. With idlers probably would be a bit longer (320 maybe).

Oh for the motor pulleys not a bad idea to get a few and try out different gearings :slight_smile:  Ive used both the steel & aluminium ones and have both held up equally as fine.
```

---
## \#21 Posted by: wwohl602 Posted at: 2019-08-14T06:34:48.483Z Reads: 35

```
I didn’t purchase the set with idlers. May have been a mistake in hindsight. 

That’s really why I wanted a cheaper option so I could experiment a bit. I’ve got 85 cags and currently running 90 wheels. May even try some TRAMPA 125s one day. 

But anyways, I’m gonna pick up a few pulley combinations to test with
```

---
## \#22 Posted by: pundahh Posted at: 2019-08-14T06:39:44.071Z Reads: 34

```
I don’t run idlers on either of my builds, they’re fine on 15/36 :slight_smile: belt tension is fairly loose too. I bet you’ll be fine. Looks like your build is turning out great :smiley:

I also hear good things about the torqueboards 110, nice and fat. Plenty of urethane. Though I think my sweet spot is 100mm, 107 is a bit too big and clunky
```

---
## \#23 Posted by: wwohl602 Posted at: 2019-08-14T06:46:18.471Z Reads: 33

```
Yea I’d expect the weigh and rolling momentum of 110s to really start eating at braking performance. 

3D printer is running now prototyping some enclosures and components. I’ll fit everything with the PLA+ I have and reprint in something like PC or a CF infused PETG. I have some ABS around I could use for the parts seeing abuse, but looks like everything in the drivetrain will stay metal
```

---
## \#24 Posted by: pundahh Posted at: 2019-08-14T06:49:18.483Z Reads: 37

```
You can go for a higher gearing with bigger wheels, that way your torque/braking will stay the same.

And yes :smiley: better off leaving everything on the drivetrain metal. What exactly are you planning to use printed?
```

---
## \#25 Posted by: wwohl602 Posted at: 2019-08-14T06:54:38.739Z Reads: 37

```
Was planning to print the wheel pulleys but no reason to unless I’m experimenting with gearing. Those pulleys are affordable enough to stay aluminum

I’ll be printing the enclosures for sure and some small mount items for lights and such. 

@Waiboard has me eyeballing the fusion board right now which has a unique enclosure look with the support ribs. Printing the Vesc enclosure now and will print an alternative from thingiverse and decide which way I’m going. Files will need modified because it’s designed for a 10S2P. 
![image|690x431](upload://in4AGTMXQqK4gmdJH2026rCr1rp.jpeg) 

Biggest item still ahead is building the pack— well, finishing a spot welder to build a pack, then I have a 40 cell pack to build 🤣
```

---
## \#26 Posted by: pundahh Posted at: 2019-08-14T06:59:09.284Z Reads: 37

```
Oh yeah I saw that, nicely built board. There’s some files on thingiverse for vanguard decks if that’s what you’re doing. If you’re going for the battleaxe sector 9 (I think that’s what it is?) i remember seeing a psycho enclosure that looked pretty good. Also great options for kydex/abs/fiberglass enclosures that might be a bit more sturdy. 

Good luck with the pack, check out the battery builders threads here and on the .news forum. No more fires pls :sweat_smile:
```

---
## \#27 Posted by: wwohl602 Posted at: 2019-08-14T07:05:41.997Z Reads: 37

```
Been through the check my battery thread thoroughly! Looking forward to it. My OCD can run wild with getting the wiring and layout perfect. 

The sector nine is going on the ownboard hub deck I’ve been riding. The TB motors are going on the vanguard deck. I have several vanguard enclosures saved on thingiverse, will print one of them too and decide which I like better on the board asthetically

Hitting purchase on the motors. Getting excited! Gonna wait until the weekend for the VESCs in case this flipsky sale happens. Leaning towards their remote as well
```

---
## \#28 Posted by: pundahh Posted at: 2019-08-14T07:13:10.670Z Reads: 36

```
Ah gotcha! Just picked up some eboosted vanguard enclosures myself for my deck :stuck_out_tongue: love the look of them. 

Don’t forget the sensor adaptors for the tb motors if you want to run sensors. Iirc they don’t plug straight into the esc.

Waiting for the sale myself too haha! I had a few mishaps with the vx1 remote but nothing major, mostly user error :stuck_out_tongue:. No disconnects during ride, however me and another user have experience cutouts after stopping. 
- (I.e brake and slow down into interception, stop, accelerate to go and realize remote has been disconnected. Requires remote reboot and pairs again).  

Battery also could be better. Fully recommend still, no disconnections & mid ride & great overall.
```

---
## \#29 Posted by: wwohl602 Posted at: 2019-08-14T07:22:41.975Z Reads: 35

```
Good to know, been reading up on several remotes. 

The eboosted enclosures look great! I just finished building a custom high end 3D printer from scratch, figured I might as well give it a project and maybe some new materials to challenge it. 
I have several variations of JST connectors from assembling that but somehow I feel like I still won’t have the right ones for the VESC haha but yes, planning to use sensors and try FOC
```

---
## \#30 Posted by: pundahh Posted at: 2019-08-14T07:30:12.385Z Reads: 35

```
Yeah, grab the adaptors from torqueboards while you’re at it then. They’re only a few bucks. I think the vesc is a jst6pin if you have that. 

I don’t know jack about 3d printing haha. Hopefully it turns out well :smiley:
```

---
## \#31 Posted by: wwohl602 Posted at: 2019-08-14T08:08:05.962Z Reads: 33

```
Yea, JST connectors come in all sorts of pitches. 3D printing uses a ton of the 3.9, 2.54mm and 2mm pitch. Think I might’ve already read they’re a 6 pin 1mm pitch connector on the VESC 🙄
```

---
## \#32 Posted by: wwohl602 Posted at: 2019-08-14T08:23:15.575Z Reads: 33

```
While I’m thinking about it, any reason to avoid the TB motors as they’re not sealed? Philly is full of tiny pebbles, road salt etc

Would I be better with the flipsky for that feature alone?
```

---
## \#33 Posted by: pundahh Posted at: 2019-08-14T14:19:47.477Z Reads: 29

```
From what I hear torqueboards motors are solid and a lot torquier. Solid guy behind it all too. Flipsky motors are a bit weaker and more mundane. I think you’ll be fine with the torqueboards one
```

---
## \#34 Posted by: wwohl602 Posted at: 2019-08-14T18:21:20.367Z Reads: 29

```
Thanks. Ordered the 6355 190kv from toque boards and some 14T pulleys. 

@dickyho has some 15T motor pulleys and 36T wheel pulleys and belts headed my way. 

Just VESCs and the BMS left now 🙃
```

---
## \#35 Posted by: wwohl602 Posted at: 2019-08-16T06:31:15.798Z Reads: 28

```
Flipsky sale is on! Just picked up two 4.20 VESCs and the VX1 remote. Just need to order the BMS and I can start building :D
```

---
## \#36 Posted by: wwohl602 Posted at: 2019-08-16T17:13:43.030Z Reads: 26

```
Going back to the BMS, seems to be the final missing piece..

For a 10S3P or 4P setup, would something like the Bestech 80 amp work well?
[BKB - Besttech 80amp](https://buildkitboards.com/products/bestech-bms#)

Second problem, anyone have a US supplier of them thats in stock?

Thanks again for all the help guys
```

---
## \#37 Posted by: wwohl602 Posted at: 2019-08-22T07:43:15.139Z Reads: 25

```
Still hunting for a discharge capable BMS with switch that’s available in the US. And still deciding on a spot welder. 

Some parts are showing up though!  Both VESCs, motors and remotes showed up. Really surprised how small the 4.2 minis are
![image|666x500](upload://maRPyMjbi3Uo1xa4ju0mMPMCB2T.jpeg) 

Thanks again for the help. I’ll create a build log once I get my last few pieces. Currently rebuilding my ownboard with a new deck that’s getting a few layers of fiberglass tonight
```

---
## \#38 Posted by: wwohl602 Posted at: 2019-09-19T18:31:16.993Z Reads: 13

```
Hi all,

I’m short two major pieces to this build.
 I’m having a little trouble figuring out the best way to handle the BMS. It’s been recommended to avoid anti spark switches and either wire in a BMS for charge only and bypass the discharge, use a loop key for on off. Or to purchase a BMS with e switch. 
For BMS with e switch, the only option I’m seeing is the bestech 60-80 amp (to handle a max of 4p 30q discharge) and the only place to get them is direct from bestech overseas, with a minimum order of 2 pieces. 

Alternatively, the loop key situation opens the door to BMS modules that cost $15 and are available on amazon 

Lastly, need to pull the trigger on a spot welder. The commercialy available sunkos seem like a bad idea. The boss spot welders look decent but it seems like the Kweld is really the best for 0.15-0.2. Any recommendations here. Kweld is definitely the most expensive- maybe I’ll start a rental program for it here 

Thanks in advance.
```

---
