# Losing some weight

### Replies: 75 Views: 3005

## \#1 Posted by: mptrs Posted at: 2017-08-19T19:53:45.980Z Reads: 362

```
A few months ago I finally finished my first build. It's a Potato deck, with a 190kv APS motor, an UNIK control and two ZIPPY Flightmax 8000mAh 5S1P 30C. All packaged in two 3d printed cases.

Everything is running just fine, never intended to build the board for speed, just for endurance. Haven't really tested all this because I missed my main point of the build and that was a light and nimble board.

I know loosing the big lipos will shave off quite some weight, but don't know what to replace them with and not end up with a granny board.

Can you guys give me some tips on how to decrease the board it's weight?
```

---
## \#2 Posted by: karma Posted at: 2017-08-19T20:00:08.954Z Reads: 338

```
Lipos usually have the highest energy density to weoght ratio so going for liion pack would probably increase the weight.
```

---
## \#3 Posted by: karma Posted at: 2017-08-19T20:00:48.063Z Reads: 325

```
Doesn't seem like your board should be super heavy, how much does it weigh?
```

---
## \#4 Posted by: jammin Posted at: 2017-08-19T20:03:29.469Z Reads: 317

```
You can save a lot of weight on trucks and deck
```

---
## \#5 Posted by: mptrs Posted at: 2017-08-19T20:18:47.399Z Reads: 298

```
To be honest it's just a feeling. When I pick it up I just think by myself this is too heavy for such a small board. Atm I don't have scale that is a able to weigh it, but will get one soon.

What I know is the lipos together are 2 kilo. Right now I'm looking at the possibility to change the 10s to 8s. And maybe lower the Mah cause I won't be going around the world with it hehe.

Thanks for the tip on lipo already having the highest energy density, so I don't need the explore the lion packs.
```

---
## \#6 Posted by: mptrs Posted at: 2017-08-19T20:20:51.858Z Reads: 288

```
Right now I have the Caliber II Fifty like most of the builds. Any tips for replacements?
```

---
## \#7 Posted by: Cobber Posted at: 2017-08-19T20:36:55.177Z Reads: 280

```
[quote="mptrs, post:5, topic:31055"]
What I know is the lipos together are 2 kilo. Right now I'm looking at the possibility to change the 10s to 8s. And maybe lower the Mah cause I won't be going around the world with it hehe.
[/quote]

The thing is bro, if you go to 8s at best you save 20% (400g) battery weight and you could drop down to 2x5000mah which might save you collectively 50% or 1000g but smaller Lipos often start to weigh more so that is really best case scenario.
So for 1kg or the weight of 1L of milk you have to buy 2x new battery and will have 20% less power and 62.5% of the range. To save a kilogram your board will be half what it is now and you have to buy new batteries...

I wouldn't bother :( sorry dude

What does your board weigh now? we could work out a % weight lost, but it will be a low number
```

---
## \#8 Posted by: chuttney1 Posted at: 2017-08-19T22:53:40.977Z Reads: 244

```
Don't bother trying to get lighter longboard trucks. Cast aluminum is cheap. Trucks made of a magnesium alloy is costly. Trucks made of carbon fiber with metal inserts for the axle, kingpin bolt, and pivot nose is even more than the first two. There is no other material lighter than carbon.

You can change your deck to carbon fiber.
```

---
## \#9 Posted by: pennyboard Posted at: 2017-08-19T23:11:18.318Z Reads: 234

```
What motor are you running? If it's a 63mm motor, you are probably not using all the power it can offer so you may want to downsize to a smaller motor, say 50mm. That's the easiest way to lose weight without affecting performance/range
```

---
## \#10 Posted by: Jinra Posted at: 2017-08-19T23:16:20.335Z Reads: 221

```
[quote="karma, post:2, topic:31055, full:true"]
Lipos usually have the highest energy density to weoght ratio so going for liion pack would probably increase the weight.
[/quote]

This is wrong. Li-ion has the best density to weight ratio, LiFePo4 has the worst. Upgrading to li-ion will help a little with weight.
```

---
## \#11 Posted by: pat.speed Posted at: 2017-08-19T23:37:09.792Z Reads: 200

```
The way I see it why not add another few batteries in parallel then you will have a huge range and you'll never need to carry it again. Although you will have to pick it up occasionally when taking it out side and stuff.
```

---
## \#12 Posted by: mptrs Posted at: 2017-08-20T08:32:15.582Z Reads: 190

```
Thanks, these are things I didn't look at. What I'm mostly looking at is the boosted board to at least match that or better. Their board is 15 pounds and has half the range I have now.

Maybe most of my weight is in the board like @chuttney1 mentioned. I'll take a look at that.

@pennyboard I am using a 6355 Sensored. This because I could not find a reliable smaller motor with 190kv at that moment.  

@pat.speed :smile: 

Thanks for all the help, I'll get a weigh in soon. Hope this will give me a better insight.

What is the average board weight here anyways? (maybe a better question)
```

---
## \#13 Posted by: Vanarian Posted at: 2017-08-20T09:24:30.926Z Reads: 191

```
You should cut down wherever you want but the battery. Keep what you have or do the same with Li-ion if you really want but don't cut on it. 

If you have a lathe or CNC access or skills you can try many stuff.

Slice the deck and reinforce remaining layers with carbon fiber ones and / or Kevlar aramide. This should save kilos. Next, choose wheels and trucks accordingly but careful with your use. Smaller wheels are lighter, do you run belt drive or hub motor? If belt drive then get 83mm flywheels and adapt gearing. Replace pulleys with either PETG or aluminum if not the case right now.

Cut unnecessary plastic areas from your connectors (not the whole plastic casing). Get shorter cables or slimmer caoutchouc sleeves around your cables.

Look if you can find titanium bolts for everything (or try and risk the Alu ones if you dare).

As you see, many options are possible I just touched the tip of iceberg. Every part can be lightened to suit your needs if you have patience and ideas.

Easier to shave an ounce everywhere than a whole kilo on a single part. Just like race cars!
```

---
## \#14 Posted by: Cobber Posted at: 2017-08-20T09:32:50.253Z Reads: 174

```
if li-ion have a better density to weight, how come the rc guys are using lipo's then?
```

---
## \#15 Posted by: Vanarian Posted at: 2017-08-20T09:43:35.910Z Reads: 173

```
@Cobber That's because of max continuous amp discharge. It is harder to find Li-ion with high amps. Also RC stuff is mainly low voltage with electronics geared for low voltage high amperage, it is cheaper to do that and weight moved in RC stuff is always lighter than a manned vehicle. 

AFAIK only high discharge 18650/21700 cells able to pull more than 30 amps continuous safely per cell are LG HB2 / HB6 and Samsung 21700-30T. HB2 are 1500mAh, Samsung 30T are 3100mAh.

For each format you will also find other cells with way more capacity but lower amperage.

We have enough space to carry big battery packs though so max amps can be bend however you like it.
```

---
## \#16 Posted by: Cobber Posted at: 2017-08-20T09:46:23.548Z Reads: 155

```
so for the weight li-ion can not discharge the amps...
```

---
## \#17 Posted by: Vanarian Posted at: 2017-08-20T10:08:08.681Z Reads: 155

```
Well yes and no :slight_smile:

Note that I was answering your question as to "why RC hobbyists use Lipo instead of Li-Ion" feel free to calculate by yourself the energy to weight ratio with any 18650 cell vs any lipo cell. A match up between Samsung 25R or LG HG2 (popular builds here) and Hobbyking Turnigy might be a good start. 

I'm personally sold for Li-ion because for my exotic limited space I obtain smaller pack for my Wh goal. I can also modify by simply switching cells models without changing volume. I manage to get more than 3200W continuous in 8S4P from my cells for less than 1.4kg total. All in triangle packs. 
Duh, can't even complain about safety. It is easier to manage 18650 cells for dummy user like me than Lipo.

Though if I wanted to draw 6000W for same size I'd go custom Lipo pack from SMC or Lonestar. And I'd still need bigger space too so not exactly same size.  See, that's yes and no.
```

---
## \#18 Posted by: Cobber Posted at: 2017-08-20T10:46:18.277Z Reads: 149

```
sorry dude I do not understand what you are saying
```

---
## \#19 Posted by: itsmikeholland Posted at: 2017-08-20T11:10:01.718Z Reads: 160

```
I was able to shave some weight by using smaller mechanical parts to offset a larger battery and more powerful motor. Right now Im running 360wh 10s4p block into a single 149kv Turnigy motor. Even with the low kv, I still only ever use half throttle at most. Im going to reduce wheels from 83mm to somewhere in the 70mm's and maybe go with smaller pulleys as well. That will shave weight and also reduce the unneccesary headroom that in 2 years I havent used, hopefully giving me more torque and efficiency. Should also mention that my board is smaller than a pennyboard and also much more lighter weight. Board is surprisingly comfortable to ride and is very maneuverable if you can balance your body weight effectively. Trucks are currently pretty tight to account for speed wobbles, still finding the sweet spot.<img src="/uploads/db1493/original/3X/1/a/1ad85f504b3ebffb6cbce275115f4c65e997ee25.jpg" width="374" height="500">
```

---
## \#20 Posted by: Vanarian Posted at: 2017-08-20T12:30:57.324Z Reads: 150

```
Now that's a neat build, how much does it weight? Looks pretty dangerous and fun too!

@Cobber if you don't get something simple like what I wrote why bother asking about energy density? Just nevermind and build with simple proven parts then.
```

---
## \#21 Posted by: Cobber Posted at: 2017-08-20T12:34:00.606Z Reads: 146

```
on the contrary... I do not have the time... I was being polite!
```

---
## \#22 Posted by: Vanarian Posted at: 2017-08-20T12:34:31.339Z Reads: 141

```
That's alright for me then.
```

---
## \#23 Posted by: Cobber Posted at: 2017-08-20T12:36:20.551Z Reads: 141

```
didn't make sense dude...
```

---
## \#24 Posted by: Vanarian Posted at: 2017-08-20T12:44:58.991Z Reads: 143

```
But it did though. Summary of everything I've written so far : 

What's the point of mounting a 200A lipo battery if your setup only draws 50A? 

Why not trade higher "wasted" amps for higher capacity instead. That was my point. Higher cap for same  weight. 

To each his poison, I could not fit lipos in my build. Li-ion just got the bill done.
That was my point.

BTW we're getting off topic ain't we?
```

---
## \#25 Posted by: itsmikeholland Posted at: 2017-08-20T12:48:09.132Z Reads: 133

```
@Vanarian right now it weighs 13.8 lbs or 6.1 kg. Keep in mind this is with 10s4p Li Ion which makes most of the weight. Its very fun, takes a little getting used to but its by far my favorite board to ride. I like less flex and the mobility.
```

---
## \#26 Posted by: mptrs Posted at: 2017-08-20T16:01:35.390Z Reads: 133

```
Thanks for the tips. Will look at the wheels, right now I have the standard 90mm.

But what I see from most of the comments I should not cut on batteries.

Any more updates on how much your board weighs?
```

---
## \#27 Posted by: Bataleon Posted at: 2017-08-20T17:30:55.146Z Reads: 137

```
@karma is basically correct. Lipos beat li-ion when it comes to energy density (energy per unit volume). However the specific energy (energy per unit mass) of lipos is identical to that of li-ion. Either way, the difference is really small :)

<img src="/uploads/db1493/original/3X/4/3/438fa79b6e02c597d68211a69f8fbbe317d5d6d6.png" width="393" height="499"><img src="/uploads/db1493/original/3X/9/b/9bb05085be81bb88ecef98de860a05b74073d4dc.png" width="375" height="500">

Sources: https://en.wikipedia.org/wiki/Lithium_polymer_battery and https://en.wikipedia.org/wiki/Lithium-ion_battery
```

---
## \#28 Posted by: Jinra Posted at: 2017-08-20T18:14:29.768Z Reads: 127

```
Lipos ARE li-ion. They both use lithium ion technology. But cylinder cell li-ions are much more energy dense than lipos.

Just do the math any literally any hobby lipo pack vs a 18650 cell. Here's an example...

[Turnigy 3s 2200mah 208g pack](https://hobbyking.com/en_us/turnigy-2200mah-3s-20c-lipo-pack.html)

3.7v * 3s * 2.2ah = 24.2 wh per 208g. Which is **117.4 wh/kg**

[Samsung 25r 18650 cell 1s 2500mah 43g](https://www.imrbatteries.com/samsung-25r-18650-rechargeable-battery/)

3.6v * 1s * 2.5ah = 9wh per 43g. Which is **209.3 wh/kg**

This particular liion cylinder cell is nearly twice as dense as a typical lipo battery you'd use for diy.

As for volumetric energy density, you'll find a similar result. However lipos can be configured to be much flatter than any 18650 pack.

@Cobber @karma
```

---
## \#29 Posted by: Cobber Posted at: 2017-08-20T19:31:40.719Z Reads: 122

```
ok... so a pair of [these](https://hobbyking.com/en_us/graphene-6000mah-6s-65c-w-xt90.html) come in at 133.2 wh/kg... but that doesn't matter 
they work perfectly with no sag in extreme use at 12s1p until I hit cut off,
the same can not be said for...
am I missing something?
```

---
## \#30 Posted by: Jinra Posted at: 2017-08-20T20:18:32.532Z Reads: 118

```
This post is about losing weight. I provided an example with math to prove how to effectively lose weight on a board. If you have other questions I suggest making a new thread.
```

---
## \#31 Posted by: Bataleon Posted at: 2017-08-20T20:40:17.054Z Reads: 115

```
@mptrs is running the equivalent of a 10S1P 30C (continuous discharge) 8000mAh lipo. That allows for a theoretical max load of 240A. 25R cells would need a 12P config to reach this level of discharge capability. Surely that is something to consider? :)

@chaka goes as far as building 10s6p packs due to the discharge rates of 18650 cells. That is 2.5 kg of cells.
```

---
## \#32 Posted by: Jinra Posted at: 2017-08-20T20:48:11.590Z Reads: 115

```
Appropriate discharge potential for various setups is an entirely different topic.. We shouldn't be spreading false information, though. That said, there are plenty of people that run 10s3p setups which are fairly lightweight. The discharge advantage has already been talked about in plenty of other threads.
```

---
## \#33 Posted by: lox897 Posted at: 2017-08-21T03:45:31.556Z Reads: 106

```
There's a way to do this. I think it's called working out. Jk
```

---
## \#34 Posted by: Cobber Posted at: 2017-08-21T05:47:45.541Z Reads: 113

```
Yes @Jinra and in context I think lipos provide the lowest weight practical solution. In fact the entire RC industry proves this point.

[quote="Bataleon, post:31, topic:31055"]
25R cells would need a 12P config to reach this level of discharge capability. Surely that is something to consider? :slight_smile:
[/quote]

Yes Baty, that is what I have been alluding to... 
As for false information trying to say discharge is irrelevant is kind of leading someone down the garden path. **_With high discharge you can have a tiny battery that weighs less..._** 

the most practical advice for @mptrs to save weight would be to try out his board with only 1 of his existing Lipo's... still won't really save that much :frowning:
Might be a bit much for his battery depending on rider weight & conditions (hills, wind)... I personally wouldn't.
```

---
## \#35 Posted by: Jinra Posted at: 2017-08-21T05:49:48.755Z Reads: 108

```
You could run a 2P 18650 build with the right ESC configuration, so yes I do think the topic is best saved for something else. There are production boards that run 2P config. Boosted themselves use 1P on a lifepo4 cell..
```

---
## \#36 Posted by: Cobber Posted at: 2017-08-21T05:58:27.890Z Reads: 105

```
Yes by throttling the build you could use a battery that would otherwise be unsuitable...
On topic: I do not think OP should drop the coin on such a battery.
```

---
## \#37 Posted by: Cobber Posted at: 2017-08-21T06:01:14.513Z Reads: 110

```
[quote="itsmikeholland, post:19, topic:31055"]
still finding the sweet spot.
[/quote]
https://www.electric-skateboard.builders/uploads/db1493/original/3X/1/a/1ad85f504b3ebffb6cbce275115f4c65e997ee25.jpg

Mike has the right idea for low weight :joy:
```

---
## \#38 Posted by: itsmikeholland Posted at: 2017-08-21T06:13:36.903Z Reads: 104

```
🙌 13lbs for 360wh 10s4p 149kv 6374 and still dropping! Next step is for lighter wheels, which will need retrofitting for pulleys. also have plans for dual diagonal drive and maybe carbon fiber board because it is already very rigid.
```

---
## \#39 Posted by: Vanarian Posted at: 2017-08-21T13:16:34.291Z Reads: 101

```
Well the point still is, IMHO, OP should not cut on batteries to save weight and he seems to agree. 

Now saying that a higher amp battery allows for smaller battery doesn't mean you crave equal capacity in that smaller battery (read RANGE here) . You only get a small battery able to deliver sufficient power for your build. I think @Jinra explained it better than I did. 

I'm too lazy to do maths for this as it's not thread topic. 

When did it become a Lipo / 18650 contest?
```

---
## \#40 Posted by: karma Posted at: 2017-08-21T13:24:22.576Z Reads: 106

```
Thanks for shining some more light on this @Jinra. I had been going around thinking LiPos had better Energy density but in reality I was wrong. The discharge rate for LiPos are a lot higher than Li-ion but not energy density.
I had to do some calculations and I came up with the same result as you.
The best Wh/Kg ratio I found on normal LiPos was around 164Wh/kg.
The best I found on Li-Ion was around 250Wh/Kg.
THAT IS A HUGE DIFFERENCE.

Here is my conclusion:
If you are going to go for a smaller battery and you are going to draw a lot of power from your setup, LiPos will be better due to the extreme discharge capabilities. Something like a 6S1P/8S1P would be a great example where LiPos are a better option. ( You wouldn't get very far but you could still supply enough power for a little while)
If you are going for a bigger battery like 10S4P where discharge from 4 good Li-Ion cells (Like Samsung 30Q) in parallel can handle the need, it would be better to go with Li-Ion cells since you can get the same Wh for around 65% of the weight of LiPos.
```

---
## \#41 Posted by: mptrs Posted at: 2017-08-29T09:32:38.705Z Reads: 101

```
Finally got a weigh in (because I broke something and while removing the screws I need to start over cause I used red threadlocker).

It's 6.8kg, which is 14.9914lbs. So it's a fraction lighter than the boosted board lol.

Think I might try some lighter wheels, but don't think it's that heavy after all.

Thanks all for the help, got some valuable information and hope it help someone else as well.
```

---
## \#42 Posted by: Jebe Posted at: 2017-08-29T23:21:42.035Z Reads: 98

```
Try a lighter board  - am building on a landyachtz hollowtech prophecy atm, Light AF.
<img src="/uploads/db1493/original/2X/2/212dc3c1c0be2d254ba8195c65d635cf175e973f.jpg" width="690" height="225">
```

---
## \#43 Posted by: sl33py Posted at: 2017-08-30T00:12:22.960Z Reads: 99

```
[quote="Jinra, post:10, topic:31055"]
This is wrong. Li-ion has the best density to weight ratio, LiFePo4 has the worst. Upgrading to li-ion will help a little with weight.
[/quote]

I disagree.  If you compare current capacity as well as Ah - Lipo wins.  If you are *just* looking at Ah - then you can find lighter setups with li-ion, but they will not output the current (C/Amps) of lipo!  

OP - i would look at some of the super small and light lipos.  My favorite super small lipo is the Nanotech 4500mAh 3s (x4 for 12s, or 3 for 9s).  Sacrifice some range, but thin and light, but still 60-75c (*4.5Ah = 250'ish A current capacity (with a grain of salt obviously... marketing)).  End result - very little sag under load.

GL!
```

---
## \#44 Posted by: Jinra Posted at: 2017-08-30T00:59:06.181Z Reads: 96

```
I'm speaking strictly in terms of watt hour per weight, proof is above
```

---
## \#45 Posted by: sl33py Posted at: 2017-08-30T01:05:48.091Z Reads: 93

```
I hear ya Jinra - but power density to me is not only Ah/Wh but also current capacity.  Sag sucks.

tomato tomatoe?
```

---
## \#46 Posted by: Jinra Posted at: 2017-08-30T01:08:42.422Z Reads: 90

```
Yea I gotcha, but i still think that's a topic for other threads, actually threads that have already been discussed. What people find "adequate" for continuous output is subjective and depends on application. Sure a smaller parallel 18650 pack will never output as much as almost all lipos, but watt for kg, it provides more power. Look at all the latest boards, a bunch of them run 10s2p, Meepo, Backfire, Riptide, arc boards, inboard (1P), etc.
```

---
## \#47 Posted by: sl33py Posted at: 2017-08-30T01:16:47.983Z Reads: 90

```
Alright i'll agree to disagree - just one last jab in the ongoing weight/Wh vs usable power...

Panasonic NCR18650A 3100mAh - and only 3$ each!  unfortunately for all that awesome 3100mAh at *only 45.5g!* - they only output 6A...  so power to weight is *spectacular* but unusable...

:stuck_out_tongue_winking_eye:
```

---
## \#48 Posted by: Jinra Posted at: 2017-08-30T01:19:08.037Z Reads: 91

```
But then you got cells like the Samsung 30T also with 3100 mah with 40A continuous. Two in parallel would give you 80A continuous, that should be enough for most people. It's definitely what my board's battery max is set to :slight_smile:
```

---
## \#49 Posted by: Vanarian Posted at: 2017-09-12T19:21:37.038Z Reads: 93

```
Finally !  Btw any hints on where to source them ? Will Samsung release it for non-manufacturers ?
```

---
## \#50 Posted by: Menjos Posted at: 2017-09-20T13:28:22.018Z Reads: 82

```
I'm running a 10s2p configuration on one of my boards, recently replaced the Samsung 25r cells with LGHD2c cells. Slightly less capacity but they stay way cooler and voltage sag is not noticeable. Seems like a good trade-off btw Lipos and higher capacity Li-Ion.
```

---
## \#51 Posted by: darkkevind Posted at: 2017-09-20T13:29:56.634Z Reads: 80

```
I assume you mean HG2s? I'm using those on an 8s4p configuration and I get next to no sag at all :D
```

---
## \#52 Posted by: Jinra Posted at: 2017-09-20T15:04:56.276Z Reads: 82

```
hg2's have more capacity than 25r's not less
```

---
## \#53 Posted by: darkkevind Posted at: 2017-09-20T15:07:12.889Z Reads: 78

```
Yes. I know. HG2s are 3000mah @ 20A, 30q's are 3000mah @ 15A

On a 4p configuration that extra 5A per cell (20A in total) makes a whole load of difference...

It's the difference between a battery than can deliver 80A continuous or 60A continuous.
```

---
## \#54 Posted by: Jinra Posted at: 2017-09-20T15:19:03.791Z Reads: 78

```
he was talking about 25r's, not 30q's
```

---
## \#55 Posted by: NickTheDude Posted at: 2017-09-20T15:32:16.492Z Reads: 87

```
Any idea where to get the Samsung 30T? I couldn't really find them after searching for a bit. I did find these though:
https://liionwholesale.com/products/ijoy-21700-battery-40a-3750mah-flat-top-battery-genuine-and-tested?variant=859373305884

40A is pretty crazy. I wonder if you could go for a 10S1P for a single motor board without much sag. 120 bucks and you get 150Wh and a super dense pack compared most other configurations.
```

---
## \#56 Posted by: darkkevind Posted at: 2017-09-20T15:33:47.852Z Reads: 88

```
Oh! My bad. Sorry I mis-read and confused myself... :confused:
```

---
## \#57 Posted by: FredSaberhagen Posted at: 2017-09-20T15:37:19.787Z Reads: 88

```
*energy to weight, not power to weight.

Power density is much better on most lipos.

They are inversely proportional, for high power you want a "leaky" membrane to deliver high amps, that results in less ability to store charge (lower energy density)

A good example is a capacitor, excellent power density but very poor energy density
```

---
## \#58 Posted by: NickTheDude Posted at: 2017-09-20T15:46:10.235Z Reads: 86

```
This is a good website to visualize that inverse preportionality.

http://www.best18650battery.com/
```

---
## \#59 Posted by: Menjos Posted at: 2017-09-20T17:06:26.866Z Reads: 89

```
Nope, I'm talking about LG HD2c - they are high drain batteries rated at 2200mah and 25A by Mooch:
https://www.e-cigarette-forum.com/forum/threads/lg-hd2c-20a-2100mah-18650-bench-test-results-a-25a-2200mah-battery-better-than-the-hd2.735554/
```

---
## \#60 Posted by: longhairedboy Posted at: 2017-09-20T19:47:16.350Z Reads: 85

```
just to chime in here.. my boards are anywhere from 22 to 25 pounds, but they ranges are in the 30+ mile zone. 

there's no magic. you want range you need lithium. And until they figure out how to cram more electrons in less lithium and do it in a lighter package other than steel cyliders or heavy foil and heatshrink, we're just going to have to use our arm muscles more.
```

---
## \#61 Posted by: Cobber Posted at: 2017-09-21T06:44:21.669Z Reads: 77

```
[quote="FredSaberhagen, post:57, topic:31055"]
*energy to weight, not power to weight.

Power density is much better on most lipos.
[/quote]

_**CHURCH**_
```

---
## \#62 Posted by: Vanarian Posted at: 2017-09-21T10:04:31.759Z Reads: 73

```
@NickTheDude same here I can't wait to get them Samsung 30T. That's some scary power and range there.

@darkkevind Actually I discovered last week that 30Q can handle 20A a bit much better than HG2. HG2 fares better up to 15A, then 30Q takes the lead. Temp discharges are also equal to that of 25R at 20A with WAY better voltage on 30Q. For a 3000mAh cell that's huge.
```

---
## \#63 Posted by: longhairedboy Posted at: 2017-09-22T15:01:22.032Z Reads: 73

```
all of this is why i waited so long to move from the 25R to the 30Q. These cells really are the performance workhorse of the industry right now. Plenty of other cells out there boast more exotic chemistries and the price per cell to go with it but the 30Q cells are the best in m opinion right now for 99% of usage cases on esk8s. IF you're drag racing, yeah, you might want something more explosive but even just street racing a big 30Q pack will ultimately out run a big lipo pack in range and will not be too far behind iit off the mark. And it will defenitely keep up after the mark.
```

---
## \#64 Posted by: Jinra Posted at: 2017-09-23T04:49:56.123Z Reads: 74

```
Just finished my first full work commute on my new 30Q pack.. and holy crap.. it blew away any expectations I had. Just check the numbers

To work 4 miles, slight decline all the way with short (1 block) hills. From work 4 miles with slight **incline** and HEAVY wind resistance.

**Samsung 25R:**
Riding style medium fast to fast (35 mph top speed)
Start 100%
End 35%

**Samsung 30Q:**
Riding style medium fast to fast (slight slower than 35 mph)
Start 100%
End ....**74%**

:scream: assuming I do that 4 times I'd get like 30+ miles! I know what you're thinking, "but you're reading the % not the voltage!" Here's the thing, my voltmeter is conservative and reads 36v as 30% battery left where it's more like 50% left for li-ion 18650's. Taking this in considering I should get even well beyond 30 miles! Though if I were to do a full range test, I'm sure the numbers would be a little more tame. 

**My Setup:**

* 10s4p (36v 12ah / 432wh)
* dual 6355 230kv
* dual Ollin Vesc 4.12 (3.29fw)
* 70/-60/40/-25 currents (changed to -15 regen due to f/w 3.29 braking fix)
```

---
## \#65 Posted by: longhairedboy Posted at: 2017-09-25T11:13:32.798Z Reads: 71

```
you should see what they do to the Evolve GT/GTX bamboo series. Its actually a legit board with a 30Q pack in it which is why i tell people to use those as a default. I've done probably 12 of those mods now and the only unhappy people are those sending me shitty cells from who knows where. 

I think 25Rs with a 100amp BMS and a tuned set of vescs would be great for street racing, but for everything other than that 30Qs just destroy.
```

---
## \#66 Posted by: Menjos Posted at: 2017-09-25T12:22:26.948Z Reads: 70

```
Well, they definitely don't destroy the LGHD2C. On a 10s2p they perform better than a 30Q, plus stay much cooler. I use a 10s2p HD2C pack on one of my boards, and a 10s3p 30Q on another. 25R and 30Q heat up too much on 10s2p for my taste.
```

---
## \#67 Posted by: Acido Posted at: 2017-09-25T12:41:28.557Z Reads: 69

```
or just get some muscle, hehe
```

---
## \#68 Posted by: Cobber Posted at: 2017-09-25T12:48:29.076Z Reads: 69

```
I think LHB lost his first 3 fingers in a band saw free styling decks before his straight edge era... don't think he can count less than three now?
```

---
## \#69 Posted by: Jinra Posted at: 2017-09-25T13:34:28.082Z Reads: 70

```
How much do you charge for the upgrade? Also, are you dropping in 10s4p?
```

---
## \#70 Posted by: longhairedboy Posted at: 2017-09-25T14:06:41.288Z Reads: 74

```
good to know about some cells that do well in small packs. The discharge curve on 25Rs and 30Qs make them better for 4P and up. For 2P you want something a lot more expensive and abuse tolerant. Lots of people use A123 cells or other chemistries in those apps.
```

---
## \#71 Posted by: longhairedboy Posted at: 2017-09-25T14:10:31.814Z Reads: 76

```
$350 plus cells. 

https://longhairedboy.com/collections/all/products/evolve-bamboo-series-gt-battery-mod

I do all the machining, build the pack, wire it in, all ths shit you don't want to and the best part is when you get the board back its got way more range and is a total sleeper. They look exactly how they did when you bought it, no visible modifications. but when you go for a ride you'll notice about 5 more miles of range and almost no voltage sag at all. That's when i use the 30Qs. HG2s sag like shit. 25Rs sag a bit too but not much. 

@Jinra you know it. 10S4P all day in there.
```

---
## \#72 Posted by: NickTheDude Posted at: 2017-09-25T14:15:27.908Z Reads: 74

```
Oooo, that's just the kind of cell I've been looking for. However I was looking through [this chart](https://www.e-cigarette-forum.com/forum/blog-entry/18650-battery-ratings-picking-a-safe-battery-to-vape-with.7447/) and noticed the LG HD4 had the same capacity and a little more discharge. Looking on liionwholesale it seems that their actually cheaper.

Another cell I noticed was the Sony VTC5A. It has the same discharge rate with a little more capacity. Definitely not worth the price IMO but it could be the holy grail for smaller packs if you have the money.

HD2C: https://liionwholesale.com/collections/batteries/products/lg-hd2c?variant=17881459588
HD4: https://liionwholesale.com/collections/batteries/products/lg-hd4-18650-battery-genuine-25a-2100mah-flat-top-wholesale-discount?variant=28023634769
VTC5A: https://liionwholesale.com/collections/batteries/products/sony-vtc5a-2500mah-25a-30a-battery-genuine-tested-flat-top-wholesale-discount?variant=28023302033

Seems to me that you could probably safely get 40A out of a HD4 or VTC5A pack if you're willing to sacrifice some range.
```

---
## \#73 Posted by: longhairedboy Posted at: 2017-09-25T14:43:31.786Z Reads: 69

```
that all looks right to me too. 

Small packs are more challenging to build in my opinion. And most of the challenge is accepting the lack of range. But seriously, a decent small pack can be had if you pay attention to your specific use case and manage your expectations when making the decision on cells. When you get below 4P, you really have to think about what you're going to be doing with the board most of the time.

Cruising? lower output higher capacity cells means that you'll get more range but you'll need to manage your speed. The best way to do that is get a small BMS and tune your ESC settings low. That will allow the ESC to get the most of your pack. 

Drag racing? high discharge lower capacity cells and just leave all the settings wide open. And get a BMS > 60 amps. Lipo is good here. 

Fast cruising and street racing? reccommend a 3P minimum but if you're going to do this on a 2P i reccommend LiFePo cells from A123 or somethig with a similar discharge curve in regular li-ion. You'll want to pay extra for these cells and look for characteristics that will give you a good balance of speed and range over the whole charge cycle. This is difficult to do which is why i go for 4P and up in this scenario, and most of the "premium" boards are too, such as the Raptor. 

With larger packs you can have speed and range. Buyt with smaller packs you typically have to pick one and build specifically for your use case. Hopefully most of you here will look at that and say "CHALLENGE ACCEPTED."
```

---
## \#74 Posted by: NickTheDude Posted at: 2017-09-25T15:09:39.621Z Reads: 67

```
Haha exactly what I was thinking. I'm going for a small commuter board and my commute is only about 12km there and back so a 10S2P even at 4200mAh should do the trick.

Ill likely end up making a pack out of HD4s and report back.
```

---
## \#75 Posted by: Vanarian Posted at: 2017-09-25T15:21:52.636Z Reads: 67

```
@NickTheDude That thumbnail though.. Hachiroku desu ga!
```

---
