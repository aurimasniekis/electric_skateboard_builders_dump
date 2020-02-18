# Barrel Connector goes :boom: What is the best charge connector?

### Replies: 91 Views: 1244

## \#1 Posted by: bluegreen Posted at: 2019-05-05T21:34:13.515Z Reads: 271

```
![20190505_141201|375x500](upload://3WPhPxADhgjTmuXIZvyANvC3YDE.jpeg) 

I want to explain this is not my proudest moment, but there are a few things to learn from what I did, and also some interesting observations about barrel jacks like this.

So things I learned:

* Do not measure voltage from a barrel port with multi meter probes regardless of how careful you think you can be about not creating a short.

![20190505_142100|375x500](upload://2BTQLWlYWNzBkmMi1IP68te8YVT.jpeg) 

* This is not an anti-spark type connector. I don't think I actually made physical contact between the two conductors, I think a spark crossed the air gap. This is less of a concern when using the actual barrel jack as it uses a plastic insulator to prevent this. However, on to lesson number 3:

![20190505_142034|375x500](upload://iHiIQrpMpAfuqFBdjv4yhxUF2Im.jpeg) 

* If a spark does occur then the resulting ionized air (plasma) will continue to conduct resulting in an arc-flash condition that continues until the internal post of the connector is fully consumed!!! :boom: :fire:

* Most Interesting to me: The resulting chamber that remains and the fact that there is still voltage on the barrel and the little nub that is left... It left a got damn floating plasma ball inside the connector until I blew it out! It wasn't just fire because... I was watching waiting for it to burn itself out... but it was self perpetuating. Cool, my board is now an ion generator.

So what now? Different more safe connector is what. What is the recommended charge connector style? GX16-3?

Honestly, I don't think barrel connectors are safe for esk8 at all.

EDIT: a 5a fuse on the charging port wouldn't be a bad idea either.
```

---
## \#2 Posted by: b264 Posted at: 2019-05-05T21:40:49.344Z Reads: 246

```
Always fuse the charge port. Always.

https://www.mouser.com/ProductDetail/576-099707.5WXN
```

---
## \#3 Posted by: J0ker3366 Posted at: 2019-05-05T21:57:51.831Z Reads: 243

```
In all fairness to barrel jacks, ive never had one fry on me for any reason. The only time i ever really hear of them frying is when people use a multi meter on the charge port, or just lack the knowledge to properly build a battery. In your case it was the first. 

[quote="bluegreen, post:1, topic:92895"]
regardless of how careful you think you can be about not creating a short
[/quote]

You should have taken your own advice... Dont blame a part that works fine when you caused it to fail.

But a fuse is a great idea. On the negative side. Like @b264 preaches. Over and over again.

[quote="J0ker3366, post:3, topic:92895"]
Over and over again.
[/quote]

And youve been here long enough to have seen it posted. I rhink you only have yourself to blame bruv. But i wish you safe journey building/repairing.

Edit: So maybe you havent been long enough lol. Just checked your profile. My bad bruv.
```

---
## \#4 Posted by: b264 Posted at: 2019-05-05T22:25:02.324Z Reads: 216

```
To be fair, how do you think I know to suggest fusing the charge port?  :smirk:  Might have melted a few things myself once upon a time.
```

---
## \#5 Posted by: bluegreen Posted at: 2019-05-05T22:31:13.826Z Reads: 219

```
First off, I already admitted this was my fault.

Secondy, I just went ahead and searched every datasheet I could find on these connectors and they are rated for 20 to 24 volts. So they are being used out of specification, and these are the failure modes you can expect.

That's all I was pointing out. Yeah it ~~probably~~ wouldn't have exploded had I not had a piece of conductive metal near the port. I guess my concern is what if something metal whacked the connector while I was riding.

I mean, for example you could use an XT60 where you should be using an XT90 but you'll only experience the learning lesson after something goes wrong. The connector on it's own isn't the problem it's the application and HOW it fails.

EDIT: I'd like to say that the connector is fine while CONNECTED. The insulation resistance is rated for 500 volts. The problem is the higher voltage increases the potential for the spark. And yes of course, with a good fuse in there the fuse should blow before any appreciable damage is done to the connector.

UPDATE: RIP Multimeter
```

---
## \#6 Posted by: deucesdown Posted at: 2019-05-05T23:47:47.684Z Reads: 198

```
XLR is good if you have room. Popular with ebikes.
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2019-05-06T01:29:16.009Z Reads: 198

```

[quote="bluegreen, post:5, topic:92895"]
I guess my concern is what if something metal whacked the connector while I was riding.
[/quote]
There's a reason these things exist![image|459x457](upload://4keMzOwJ4UNDM7BP0qWkEofUzeW.jpeg)
```

---
## \#8 Posted by: bluegreen Posted at: 2019-05-06T01:30:09.624Z Reads: 190

```
Yah true, they are more important than I realized.

Damn, people salty AF about this.

It's almost like people wait on this forum for someone to make a mistake just to have a good time roasting them. I've learned my lesson and won't be sharing anything like this again you monsters.
```

---
## \#9 Posted by: b264 Posted at: 2019-05-06T02:28:52.527Z Reads: 187

```
I've done the same thing, though not as badly, on more than 1 occasion, and it's one of many reasons I suggest to use [fuses](https://www.mouser.com/ProductDetail/576-099707.5WXN) and to never stick multimeter probes in barrel jacks.

Also this, use these

![20190505_212656|690x388](upload://gXxvbBWZAcH43j40R04EDBKZtfP.jpeg)
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-05-06T02:39:17.619Z Reads: 187

```
[quote="bluegreen, post:5, topic:92895"]
you could use an XT60 where you should be using an XT90 but you’ll only experience the learning lesson after something goes wrong
[/quote]

This is irrelevant and chances are you will melt the wire before you melt a xt60 in almost any build....
```

---
## \#11 Posted by: Frenchy Posted at: 2019-05-06T02:40:04.451Z Reads: 184

```
[quote="bluegreen, post:8, topic:92895"]
I’ve learned my lesson and won’t be sharing anything like this again you monsters.
[/quote]

LMFAO 😂 10jason
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-05-06T02:40:21.051Z Reads: 181

```
[quote="bluegreen, post:8, topic:92895"]
Damn, people salty AF about this.
[/quote]

Nah we're not salty we just considering how......
```

---
## \#13 Posted by: b264 Posted at: 2019-05-06T02:40:43.329Z Reads: 185

```
[quote="bluegreen, post:8, topic:92895"]
won’t be sharing anything like this again you monsters.
[/quote]

Just remember, you are helping other people not make the same mistake.  There is no shame in helping people.
```

---
## \#14 Posted by: AlanZhou Posted at: 2019-05-06T02:43:10.100Z Reads: 182

```
The best connector in my opinion for size and amperage is a gx 16-4, there's 4 pins and each pin set can handle 5a so if you use 2 pins for negative and two for positive you can do effectively do 10A rated up to 1500v AC

^though I don't know how much I trust the 1500v AC rating
```

---
## \#15 Posted by: ARetardedPillow Posted at: 2019-05-06T02:48:24.677Z Reads: 173

```
I push 9 amps through barrels with no issues
```

---
## \#16 Posted by: b264 Posted at: 2019-05-06T02:50:01.495Z Reads: 173

```
My barrels get warm at 4A, ice cold at 2A
```

---
## \#17 Posted by: AlanZhou Posted at: 2019-05-06T02:52:42.896Z Reads: 171

```
@b264 what size? @ARetardedPillow uses 5.5 2.5, and they are really nice
```

---
## \#18 Posted by: b264 Posted at: 2019-05-06T03:02:19.218Z Reads: 172

```
5.5mm x 2.1mm standard ones.  You can get them rated up to 7A but most are rated at 5A.  The 7A ones are really long.
```

---
## \#19 Posted by: AlanZhou Posted at: 2019-05-06T03:03:44.620Z Reads: 173

```
Huh 5.2 x 2.5 are rated up to 7a and they are normal sized
```

---
## \#20 Posted by: ARetardedPillow Posted at: 2019-05-06T03:07:49.822Z Reads: 174

```
I use 5.5x2.1s for anything 10s, and anything above that 2.5s.

I have those THICC ones that's full metal, they don't advertise it as "high" amp but I pushed 9amps through them without getting a tad bit warm.
```

---
## \#21 Posted by: bluegreen Posted at: 2019-05-06T03:37:47.239Z Reads: 165

```
I'd like to reiterate it's not the current carrying capacity that is the issue here. It's the fact that once you start going north of 36 volts the spark gap starts to become a factor.

The other issue that I really didn't like so much was once there was a spark, because the positive conductor is entirely surrounded by the negative conductor the spark easily propagates into a runaway arc-flash.

What I'm saying is that just based on the fault condition of this connector (of runaway frying itself to death), is pretty extreme compared to using the GX16-3. I've noticed that chargers that are UL certified on amazon all have the 3 prong connector at voltages above 8s, so I'm not really that far in outer space here.

I think the main reason people are picking at me is because yes the fault condition is initiated by poking things where they don't belong. But again, the whole reason I posted this was not because I obviously bridged the conductors. It was because there is arc flash potential with this connector.
```

---
## \#22 Posted by: LukePL Posted at: 2019-05-06T03:48:13.355Z Reads: 156

```
Thank you for shareing!!! @bluegreen
I had few things reminded/explained.
```

---
## \#23 Posted by: MD84 Posted at: 2019-05-06T04:16:21.757Z Reads: 150

```
That is really interesting. I would have not thought an arc flash would propagate at <50v. I suppose once the air in that relatively small gap is ionized it is possible. 

The big takeaway here is to always fuse your charge port. An xt60 would be a fine option for a charge port?
```

---
## \#24 Posted by: Darkie02 Posted at: 2019-05-06T04:58:17.050Z Reads: 151

```
Thanks for posting I found it is usefull and a reminder of what can happen if you exceed the manufactures limits and just because most people do doesn’t mean you won’t have any issues. 

In my searches so fare it seems there’s a few options but nothing ideal yet all have done issue 

Rosenberger magnetic connector
Perfect if it wasn’t so large.


GX 16 4
(Pins rated to 5amp shouldn't connect live)


XT 60/30
(Exposes pins on board shouldn’t connect live)

XLR 
Large connector 

Barrel Connector
Ali exspress takes ratings by playing darts and other people believe it’s true an post it online. You wouldn't trust the 18650 cell rating so why do you trust their barrel rating! (some one pleas prove me wrong with real proper tests over 5 amps)

I’m planing on using the GX 16 6 pin as sensor wire connectors on next build see how I like the connector then decide if I’m going XT30 or GX 16 4pin for charge think the locking part might be annoying in the GX 16
```

---
## \#25 Posted by: MD84 Posted at: 2019-05-06T05:09:00.881Z Reads: 145

```
For xt60 what do you mean by exposes pins and shouldn't connect live? I would suggest female plug. Don't all of these plugs have exposed conductors?

I don't worry about connecting a charger to a live battery because it is regulated low current.
```

---
## \#26 Posted by: Jinra Posted at: 2019-05-06T05:28:05.660Z Reads: 142

```
I feel like you need MUCH **MUCH** more voltage to starting arcing across air. The traces on the vescs are sometimes a millimeter or less apart running our max battery voltages, and it doesnt start arcing, let alone the 2-3~ millimeters from DC post to wall
```

---
## \#27 Posted by: bluegreen Posted at: 2019-05-06T05:40:48.015Z Reads: 141

```
The arc was created by the spark I made when tapping it with the multimeter. It would have created ionized gas itself, and also sent small metal particles flying through the air.

On it's own there is yeah, NO WAY that an arc can form on it's own. That's why it has that crazy high AC rating.

Maybe it would be worth SCIENCE to reproduce the problem so y'all can understand this thing was like a blow torch for 5 seconds.
```

---
## \#28 Posted by: MD84 Posted at: 2019-05-06T05:49:41.424Z Reads: 139

```
Yes, I was thinking a recreation is in order. I wonder what was the resistance of that plasma circuit. I feel like the circuit would not sustain in open air with that same gap. Something about the cavity and cylindrical shape of the barrel jack probably helps maintain the conductive atmosphere.
```

---
## \#29 Posted by: bluegreen Posted at: 2019-05-06T05:59:16.443Z Reads: 139

```
[quote="MD84, post:28, topic:92895"]
cavity and cylindrical shape
[/quote]

Maybe it was just a freak of nature thing, but yeah it was surreal to watch. Well, first I was having a panic attack because I was really concerned that the battery itself was going to blow up because this had created a hard short.

But after realizing I had no way of stopping it, and deciding if I should throw it in the bath tub or not the fire finally went out and it was still smoking. But there was a little purple blue ball in there, and I thought, oh that must be the rest of the plastic melting. Under closer inspection, it just kept going and dancing around, so I blew it out and then had a heart attack and died.

If you have seen a plasma lighter:
![image|600x338](upload://67M2bhSna8lZVulR1dxoxQl0iWt.jpeg) 

It looked exactly light that but a little sphere inside the chamber.

Now that I read own post, you are going to think I was on drugs. I SWEAR MAN.

If I had a safe place to do this, I would totally do it again in the name of science. What even is a safe place to do destructive testing of lipos? Does anyone have a giant parking lot I can use? #mythbusters
```

---
## \#30 Posted by: Hummie Posted at: 2019-05-06T06:17:19.928Z Reads: 133

```
The tenderloin I bet we can blow stuff up.  If u can shoot up and take a crap on the sidewalk we can get away with a little blown ion cell.  
I saw a nasa paper where they were essentially blowing up stuff and got cells to a super high voltage and want to do that.  Too exciting not to.
```

---
## \#31 Posted by: TowerCrisis Posted at: 2019-05-06T06:22:11.944Z Reads: 129

```
lol what? I never realized you were from SF
```

---
## \#32 Posted by: bluegreen Posted at: 2019-05-06T06:22:25.184Z Reads: 126

```
Oh, I mean, I'm sure we could do it once, but I'm thinking of actually doing this proper where we could have scientific instruments like a TABLE or SAFETY GOGGLES. I actually mentioned #mythbusters because they got to use the old decommissioned oakland airfield.
```

---
## \#33 Posted by: Hummie Posted at: 2019-05-06T06:26:50.067Z Reads: 125

```
We could have a skate meetup where we bring our old cells! @TowerCrisis.  We should all meet at noisebridge sometime
```

---
## \#34 Posted by: bluegreen Posted at: 2019-05-06T06:28:16.325Z Reads: 124

```
Does nb have an outside?

I just realized my apartment has a ROOF. You can't catch buildings on fire from the TOP can you?
```

---
## \#35 Posted by: b264 Posted at: 2019-05-06T06:29:10.079Z Reads: 126

```
[quote="Darkie02, post:24, topic:92895"]
Barrel Connector Ali exspress takes ratings by playing darts and other people believe it’s true an post it online. You wouldn’t trust the 18650 cell rating so why do you trust their barrel rating! (some one pleas prove me wrong with real proper tests over 5 amps)
[/quote]

OMG don't buy connectors from the 'baba -- buy them from digikey if you're serious.  Yes, all the ratings there are science-based.
```

---
## \#36 Posted by: Hummie Posted at: 2019-05-06T06:29:36.237Z Reads: 120

```
Roof sounds ideal. They don’t have one we can use at noisebridge.  Sure could be figured w no fire.  I’ve got a 10 amp power supply.
```

---
## \#37 Posted by: b264 Posted at: 2019-05-06T06:29:50.030Z Reads: 118

```
[quote="Jinra, post:26, topic:92895, full:true"]
I feel like you need MUCH **MUCH** more voltage to starting arcing across air. The traces on the vescs are sometimes a millimeter or less apart running our max battery voltages, and it doesnt start arcing, let alone the 2-3~ millimeters from DC post to wall
[/quote]

I agree with you @Jinra -- but I might add that those traces aren't insulated solely by air.
```

---
## \#38 Posted by: bluegreen Posted at: 2019-05-06T06:30:54.158Z Reads: 122

```
@hummie heck this kickstarter. Lets just start an esk8 business so we can have a warehouse for testing.

EDIT: I would feel OK doing this on the roof of my office in China, worse things have been done there.

UPDATE: I just realized the office is moving into a former parking garage, I think I need to continue development overseas.
```

---
## \#39 Posted by: TowerCrisis Posted at: 2019-05-06T06:32:12.015Z Reads: 121

```
Hah I'm actually gonna be in SF tomorrow meeting up with a friend. Once I'm done with her I'd actually be down to set some shit on fire but idk when that time'll come around. Also thanks for the tip about noisebridge, that place sounds cool.
```

---
## \#40 Posted by: Hummie Posted at: 2019-05-06T06:36:18.262Z Reads: 118

```
If any and all of u want to get dinner tomorrow somewhere in the mission the food is good and we could plan our fires. 
@DAddYE I think is sf too
```

---
## \#41 Posted by: bluegreen Posted at: 2019-05-06T06:36:46.589Z Reads: 104

```
How did my barrel fire thread turn into a meetup thread?
```

---
## \#42 Posted by: Jinra Posted at: 2019-05-06T06:37:08.131Z Reads: 103

```
Pretty sure I've seen some vescs without conformal coating
```

---
## \#43 Posted by: b264 Posted at: 2019-05-06T06:37:40.017Z Reads: 100

```
The solder mask is what I was referring to actually, but conformal coating makes it even more.
```

---
## \#44 Posted by: TowerCrisis Posted at: 2019-05-06T06:42:20.903Z Reads: 107

```
I'll bring a spare 30T. Should make for a good firecracker.


In regards to the original post, I'm not a fan of 5mm barrel jacks. There ought to be a safer standard in esk8 with our higher voltages and currents.
```

---
## \#45 Posted by: b264 Posted at: 2019-05-06T06:51:33.055Z Reads: 113

```
Safer, sure.  But more convenient?  It better be just as convenient :smiley:

The GX16-3 are a huge pain in the ass.  At least, if you want them water resistant while unplugged.
```

---
## \#46 Posted by: bluegreen Posted at: 2019-05-06T07:04:45.468Z Reads: 111

```
![image|500x500](upload://m6xs5VdEQ5NrU4jQ9FmLyvZ4Kh1.jpeg) 

Would these not work?
```

---
## \#47 Posted by: TowerCrisis Posted at: 2019-05-06T07:12:29.439Z Reads: 110

```
Those do, however they don't solve the issue with the middle prong being uninsulated.

Also, never use ones with metal caps like that. One guy on the forum burnt his plug down (just like OP) once it touched the port at a weird angle and sparked between the outer housing and the prong.
```

---
## \#48 Posted by: bluegreen Posted at: 2019-05-06T07:20:41.416Z Reads: 108

```
While the prongs on the inside are uninsulated, there is only a linear arc path as opposed to a planar arc path. (The arc can form in a full 360 degrees around the pin of a barrel connector)

This linear distance is like 4 to 5 times greater than the inside of the barrel gap as well.


Yeah I don't think the metal cover should be used. It would be best if it was a machine plastic with a gasket inside.

They exist, It's a military spec connector, and I'm looking for a good picture of one.
```

---
## \#49 Posted by: b264 Posted at: 2019-05-06T07:27:11.177Z Reads: 109

```
That one on the left I have and it works fine, but it's a motherfucker to screw and unscrew because sand and debris gets in the threads, it's like threading a bolt with wet fine sand on the threads.

And it doesn't last much longer than a stinky fart because the metal it's made out of is cheese chinesium.  You have to constantly replace those metal lids.
```

---
## \#50 Posted by: b264 Posted at: 2019-05-06T07:28:29.877Z Reads: 108

```
[quote="TowerCrisis, post:47, topic:92895"]
Also, never use ones with metal caps like that. One guy on the forum burnt his plug down (just like OP) once it touched the port at a weird angle and sparked between the outer housing and the prong.
[/quote]

Oh and I've also shorted them out before but I fuse the charge ports... so it's not a huge deal.  Just have to take the skate apart and fix it if you drunk-short the charge port
```

---
## \#51 Posted by: lrdesigns Posted at: 2019-05-06T07:46:03.490Z Reads: 108

```
If you want a durable connector Id go for XT60, but make sure its fused and non of your other devices use XT60 so they cant cross streams. 3D print a dust cap. Edit, use a blanked off male plug for the dust cover, like a loop key without the electrical connection. 

https://media.giphy.com/media/3o72FiKtrMAjIb0Rhu/giphy.gif
```

---
## \#52 Posted by: bluegreen Posted at: 2019-05-06T07:46:07.846Z Reads: 106

```
[quote="b264, post:50, topic:92895"]
take the skate apart and fix it
[/quote]

https://www.amazon.com/LGEGE-Electrical-Mounted-Holder-Stereo/dp/B01DBL1F80/ref=sr_1_1_sspa?keywords=panel+mount+fuse+holder&amp;qid=1557128709&amp;s=gateway&amp;sr=8-1-spons&amp;psc=1

I thought about using one of these but I'm like, wow if I need to get at the fuse easy I'm doing something wrong.

EDIT: Probably also a good idea to inspect nothing else blowed up.
```

---
## \#53 Posted by: b264 Posted at: 2019-05-06T07:47:20.708Z Reads: 104

```
That adds another hole in the enclosure, which is one more place water can get inside.  I prefer these little things soldered in and stuck to something with JB Weld

https://www.mouser.com/ProductDetail/576-099707.5WXN
```

---
## \#54 Posted by: bluegreen Posted at: 2019-05-06T07:48:05.935Z Reads: 109

```
Since I'm sticking with the first thing that shows up on amazon or ebay build:

https://www.amazon.com/Everything-Automobiles-Assorted-Inline-Holders/dp/B01E5MM63C/ref=sr_1_2_sspa?keywords=fuse+holder&amp;qid=1557128864&amp;s=gateway&amp;sr=8-2-spons&amp;psc=1
```

---
## \#55 Posted by: bluegreen Posted at: 2019-05-06T07:54:34.223Z Reads: 116

```
By the way this used to be my job this is where whatever "qualifications" I have come from:

![image|604x453](upload://4pRiXryzz2NyMijzf5I1IRRarZZ.jpeg)
```

---
## \#56 Posted by: Darkie02 Posted at: 2019-05-06T08:01:17.023Z Reads: 112

```
It still sparks and exposed pins if a coin flicks up of falls on them it could short the battery. If you use the female it have to stick out a lot or not be sealed so the male case can go over the out side of the female yell case.
```

---
## \#57 Posted by: bluegreen Posted at: 2019-05-06T08:12:33.193Z Reads: 114

```
MMM It is not cheap, but that looks quality.

![image|690x469](upload://i8BGYT7HHjIjxDrG8iikYQqcNbg.jpeg) 


https://www.amazon.com/CERRXIAN-Waterproof-Soldering-Connector-Equipment/dp/B07H55V345/ref=asc_df_B07H561M9V/?tag=hyprod-20&amp;linkCode=df0&amp;hvadid=312172921394&amp;hvpos=1o3&amp;hvnetw=g&amp;hvrand=1888115161617650191&amp;hvpone=&amp;hvptwo=&amp;hvqmt=&amp;hvdev=c&amp;hvdvcmdl=&amp;hvlocint=&amp;hvlocphy=9031939&amp;hvtargid=pla-669130214565&amp;th=1

The downside, besides price: Installation Hole: Φ21mm
```

---
## \#58 Posted by: TowerCrisis Posted at: 2019-05-06T08:40:48.401Z Reads: 110

```
That's just the problem though. That looks like a NICE beefy port that surely is durable.

The problem is that the female side should be the panel mount version. They're switched.

The side that is always live should not have the exposed pins. The charger should, especially since they're already current limited to 2 or 4 or whatever amps you charge at. That would prevent any kind of sustained arc flash.
```

---
## \#59 Posted by: Michaelppainter Posted at: 2019-05-06T09:01:31.834Z Reads: 114

```
I use a dc5.5 barrel connector to charge to 10s at 2amps but I admit I've sometimes wondered about what would happen if it shorted... At the moment I cover the pin with shrink-wrap and abit of electrical tape when our riding. Can anyone tell me where you get those rubber dust covers you all seem to be using?
```

---
## \#60 Posted by: taz Posted at: 2019-05-06T09:05:22.989Z Reads: 117

```
They come with the connectors

https://www.ebay.com/itm/10PC-Waterproof-plastic-5-5mm-X-2-1mm-DC-socket-mounting-Power-Chargers-Nut-022/141240061934?ssPageName=STRK%3AMEBIDX%3AIT&amp;_trksid=p2057872.m2749.l2649
```

---
## \#61 Posted by: Michaelppainter Posted at: 2019-05-06T09:54:41.291Z Reads: 106

```
Awesome cheers dude! I've spend so long looking but never typed "waterproof"! Ordered
```

---
## \#62 Posted by: mynamesmatt Posted at: 2019-05-06T10:10:48.388Z Reads: 104

```
[quote="AlanZhou, post:14, topic:92895"]
gx 16-4
[/quote]

I've got a similar plug. idk what it is but it looks like a variant of the gx connector.  I've pushed 41.9v @9a through this and it was just fine. It works super good in conjunction with my range extender as the plug never falls out :D
https://www.jaycar.com.au/2-pin-line-female-microphone-connector/p/PS2014
```

---
## \#63 Posted by: Hannes Posted at: 2019-05-06T10:23:19.388Z Reads: 103

```
For someone that isn't too into electronics where should the fuse be? Somewhere on the positive lead on the charge port?
```

---
## \#64 Posted by: MD84 Posted at: 2019-05-06T11:01:18.160Z Reads: 101

```
If you have a positive lead and a negative lead coming from your battery, just pick either wire, cut it, and place your fuse inline with that wire. It doesn't matter which wire.
```

---
## \#65 Posted by: sk8l8r Posted at: 2019-05-06T11:21:21.451Z Reads: 105

```
Im happy with this connection I've been using has a screw cap but plastic at least

https://www.ebay.com/itm/SP13-Waterproof-IP68-Chassis-Panel-Mount-Circular-Aviation-Plug-Cable-Connector-/171318772490?oid=172382452044
```

---
## \#66 Posted by: MD84 Posted at: 2019-05-06T11:40:43.255Z Reads: 107

```
![1557142360611260600471|666x500](upload://5l8HW2pyUNEymFwT43HEUE4A6Ra.jpeg) 

![15571423957041452630900|666x500](upload://xn4n1ZBKHSo1zq7XvQG8q88zpYK.jpeg) 

I had these for a different project but thought they had a place in this thread. One is a small panel mount circuit breaker and the other is an amphenol connector. It seems to have the correct orientation. I don't have the flange mount female side anymore. 

Amphenol PT06A-8 series

![PT02A-8-2S_sml|200x200](upload://6RftcPiLY450MTMSgvMpyMge2SB.jpeg)

Speaking of wind farms, I was the high voltage reliability engineer for a renewables company. I worked in Oregon in Shepards Flats and other areas out west.
```

---
## \#67 Posted by: xsynatic Posted at: 2019-05-06T11:48:40.729Z Reads: 103

```
Ha. That happened to me too. I just build myself a new one. Cost me 3-4 bucks.
```

---
## \#68 Posted by: totalgeek9224 Posted at: 2019-05-06T11:55:13.240Z Reads: 104

```
This is why we need an esk8 pioneer to design a good connector, like a bulked up magsafe would be nice
```

---
## \#69 Posted by: Darkie02 Posted at: 2019-05-06T14:02:33.528Z Reads: 103

```
Or a quick search for a E  vehicle standers there’s even a 60v 10amp version it’s just so big and expensive

https://www.rosenberger.com/en/products/automotive/ropd.php
```

---
## \#70 Posted by: banjaxxed Posted at: 2019-05-06T14:09:54.700Z Reads: 102

```
I flipped one of these through seawater puddles left it covered in sand and generally treated it like shit all last summer without issue 

https://s.click.aliexpress.com/e/d2BW21K
```

---
## \#71 Posted by: Battosaii Posted at: 2019-05-06T14:56:06.304Z Reads: 99

```
Damn been running 8a in my barrel connector for months now. I never noticed any unusual heat from thw connectors.
```

---
## \#72 Posted by: Bjork3n Posted at: 2019-05-06T15:03:39.649Z Reads: 101

```
When you guys say fuse, do you suggest using a fuse even if you use bms for discharge? 
If so where should i put it? after the charge plug inside the enclosure? Will this work? ![s%C3%A4kringsh%C3%A5llare|499x500](upload://bRYqhqN9CVjMjEzJt3c3WfnbYp2.jpeg)
```

---
## \#73 Posted by: pjotr47 Posted at: 2019-05-06T15:29:48.856Z Reads: 101

```
https://nl.aliexpress.com/item/1Set-WP20-4Pin-Waterproof-Chassis-Panel-Mount-Aviation-Plug-Cable-Connector-Plug-Socket-30A-500V/32764198104.html?spm=a2g0s.9042311.0.0.27424c4dSSxB25

Spec is 30A so I think 20A would be possible
```

---
## \#74 Posted by: AlanZhou Posted at: 2019-05-06T16:02:24.665Z Reads: 97

```
I dislike fuses as if they blow I will have no brake's or power....

Just use a fuse for charging, either fuse the positive lead or the negative lead of the charge port
```

---
## \#75 Posted by: b264 Posted at: 2019-05-06T17:56:40.462Z Reads: 95

```
Coonect the fuse between the C- on the BMS and the negative charge port
```

---
## \#76 Posted by: pixelsilva Posted at: 2019-05-06T18:36:24.133Z Reads: 92

```
> @J0ker3366 
> 
> Like @b264 preaches.

https://gifimage.net/wp-content/uploads/2018/04/preaching-gif-5.gif
```

---
## \#77 Posted by: pixelsilva Posted at: 2019-05-06T18:44:47.857Z Reads: 90

```
[quote="bluegreen, post:8, topic:92895"]
It’s almost like people wait on this forum for someone to make a mistake just to have a good time roasting them. I’ve learned my lesson and won’t be sharing anything like this again you monsters.
[/quote]

https://edge.ua.edu/wp-content/uploads/2014/02/elasticband.gif
```

---
## \#78 Posted by: J0ker3366 Posted at: 2019-05-06T19:24:27.449Z Reads: 90

```
@bluegreen 

[quote="pixelsilva, post:77, topic:92895"]
It’s almost like people wait on this forum for someone to make a mistake just to have a good time roasting them
[/quote]

When they make it so easy, one cant help but to wait lol.

Just remember, as long as you learned something, then no harm done 
![joker------------wallpaper-10579258|562x500](upload://9sw27uMRzEkz3hM8CuTxXyfDs4u.jpeg)
```

---
## \#79 Posted by: Sebike Posted at: 2019-05-06T19:39:52.435Z Reads: 85

```
so you could technically cool some beers with your plugs given they are charged with 2 amps? pictures or it didn't happen.
```

---
## \#80 Posted by: bluegreen Posted at: 2019-05-06T20:18:48.312Z Reads: 82

```
Ooo baby, look at this one!

https://www.ebay.com/itm/CNLINKO-Connector12V-10A-Waterproof-IP65-DC-Power-Gold-Plated-2Pin-Welding-Cable/153151512243?_trkparms=aid%3D555018%26algo%3DPL.SIM%26ao%3D1%26asc%3D57476%26meid%3D7c5ff3b3f2ac4f00ba5bf5df39408018%26pid%3D100005%26rk%3D4%26rkt%3D12%26mehot%3Dpp%26sd%3D171318772490%26itm%3D153151512243&amp;_trksid=p2047675.c100005.m1851

10 amps at 400 volts, nice.
```

---
## \#81 Posted by: bluegreen Posted at: 2019-05-06T20:31:21.643Z Reads: 80

```
A more affordable option:

https://www.ebay.com/itm/SD13-13mm-2P-Flanged-Waterproof-Aviation-Cable-Connector-Socket/231932184413?epid=1567428174&amp;hash=item36003c475d:g:si8AAOSwdbZa2H6K

SD13 I think is the homeboy.

![image|500x500](upload://qmJelbsiy18k36Fa4jnja2SfeY3.jpeg)
```

---
## \#82 Posted by: Surfer Posted at: 2019-05-06T20:56:09.556Z Reads: 74

```
The best I could find after hours researching:
http://www.switchcraft.com/Category.aspx?Parent=943
```

---
## \#83 Posted by: banjaxxed Posted at: 2019-05-06T21:29:29.907Z Reads: 71

```
Yep they are good, 13mm and carry 10A iirc. Plus you can probe the bejasus outta them
```

---
## \#84 Posted by: MD84 Posted at: 2019-05-07T11:34:27.975Z Reads: 67

```
Just make sure to get written consent before probing...
```

---
## \#85 Posted by: totalgeek9224 Posted at: 2019-05-07T12:10:34.823Z Reads: 70

```
Here are some conectors ive found when browsing Digikey

https://www.digikey.com/product-detail/en/switchcraft-inc/EN3P2FX/SC1844-ND/1289362

https://www.digikey.com/product-detail/en/conxall-switchcraft/4182-2SG-300/SC1231-ND/526196

https://www.digikey.com/product-detail/en/amphenol-industrial-operations/PT02A-8-2S/PT02A-8-2S-ND/2510802

https://www.digikey.com/product-detail/en/amphenol-industrial-operations/97-3102A-12S-3S/97-3102A-12S-3S-ND/340859

https://www.digikey.com/product-detail/en/lemo/EGG.1B.302.CLL/1124-1337-ND/3597385


EDIT: Is a new plug really necessary? What if we just started implementing diodes inline to our fuses on the charge plug, so that the plug would be unable to short?
```

---
## \#86 Posted by: bluegreen Posted at: 2019-05-08T05:49:11.577Z Reads: 57

```
![20190507_223945|666x500](upload://qiFXncwU87wn3qiwBZxZD0R9teR.jpeg) 

A handy little tool.
```

---
## \#87 Posted by: J0ker3366 Posted at: 2019-05-08T05:54:47.064Z Reads: 53

```
@b264 if you built it, they will copy you.

Just wait. Flipsky is soon to have their own lol.
```

---
## \#88 Posted by: J0ker3366 Posted at: 2019-05-08T05:57:36.348Z Reads: 57

```
[quote="bluegreen, post:86, topic:92895"]
A handy little tool.
[/quote]

Try shortening your wire
![20190507_235631|375x500](upload://7hJQJ9aEQNFEJBFBZrdvygmVNRQ.jpeg)
```

---
## \#89 Posted by: b264 Posted at: 2019-05-08T06:01:51.540Z Reads: 57

```
![20181118_205522|690x345](upload://2ALCWQbs3EAurHFeENQBbfwilmA.jpeg) 

Top one is @Skunk's

Right one is my first one, bottom one is my 12S LiFePO4 one

:arrow_down: and this is mine that I use all the time

![20190209_213044|690x388](upload://bBVwsZ9wm9SfO8CNaUHjqP6UCEj.jpeg)
```

---
## \#90 Posted by: bluegreen Posted at: 2019-05-08T06:34:49.477Z Reads: 53

```
Nice! I had thought about 3d printing something but JB weld seems to work pretty well too! I hadn't thought about having both female and male on there, that's pretty cool.

I just hooked it up this way because because I just had these pigtails with tinned ends didn't want to fiddle with it, just got it today.
```

---
## \#91 Posted by: b264 Posted at: 2019-05-08T06:52:31.439Z Reads: 54

```
I think @mmaner went that direction and 3D printed one.
```

---
