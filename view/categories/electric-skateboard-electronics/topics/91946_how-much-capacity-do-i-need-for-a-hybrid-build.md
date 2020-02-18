# How much capacity do I need for a hybrid build?

### Replies: 67 Views: 456

## \#1 Posted by: Michal Posted at: 2019-04-27T12:50:01.007Z Reads: 169

```
I've been trying to find the answer to this fo quite some time now, but i couldn't seem to find anything. How much capacity do I actually need? I don't want to overpay for too much capacity, but i also don't want to have too little range. I wnat my range to be at least 15 km, I weight 72kg and I'll be using dual Turnigy sk8 6374 193kv motors.
```

---
## \#2 Posted by: Grozniy Posted at: 2019-04-27T12:51:29.197Z Reads: 160

```
What wheels?
```

---
## \#3 Posted by: Michal Posted at: 2019-04-27T12:52:48.566Z Reads: 159

```
Bergmeister from haggy (150mm pneumatics)
```

---
## \#4 Posted by: Grozniy Posted at: 2019-04-27T12:52:58.446Z Reads: 160

```
Noice choice
```

---
## \#5 Posted by: Michal Posted at: 2019-04-27T12:53:57.535Z Reads: 153

```
Yeah, they look really awsome.
```

---
## \#6 Posted by: Grozniy Posted at: 2019-04-27T12:54:47.956Z Reads: 149

```
So it will be at least 20wh/km.
20x15=300wh.
3.7v x 3ah x 10S x 3P = 333wh , that's for 30Q cells
```

---
## \#7 Posted by: Blitz Posted at: 2019-04-27T12:55:23.821Z Reads: 150

```
[quote="Grozniy, post:6, topic:91946"]
3.7v
[/quote]
I wouldn't be to sure  about that as the nominal
highest on 18650s  I've personally seen is 3.65
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-04-27T12:56:09.779Z Reads: 139

```
E: Im gonna eat my hat. 

It actually does say 3.6 on the top 3 websites from google, but I know I've seen 3.7 when on other forums (drones, a few times on endless sphere)
```

---
## \#9 Posted by: Michal Posted at: 2019-04-27T12:57:07.601Z Reads: 137

```
So i need at least a 300wh battery?
```

---
## \#10 Posted by: Blitz Posted at: 2019-04-27T12:57:16.317Z Reads: 130

```
3.7 for lipos I just checked Q30s are 3.6 (nominal)

but maybe 3.7 is somehow used to get the wh's???
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-04-27T12:58:29.605Z Reads: 124

```
edited my post a second before you replied :P
```

---
## \#12 Posted by: Grozniy Posted at: 2019-04-27T12:59:37.748Z Reads: 123

```
So at least you need 10s3p 30Q pack. That's li-ion.
Or at least 300wh lipo
```

---
## \#13 Posted by: Blitz Posted at: 2019-04-27T13:00:50.779Z Reads: 118

```
3p would sag In my head I like to calculate effective range and anything left I count as slug range.

and with dual motors oof 3p not enough for sure.
```

---
## \#14 Posted by: Michal Posted at: 2019-04-27T13:02:12.965Z Reads: 113

```
How about a 10s4p?
```

---
## \#15 Posted by: Blitz Posted at: 2019-04-27T13:02:35.803Z Reads: 113

```
Sounds like a good solid standard.
```

---
## \#16 Posted by: Michal Posted at: 2019-04-27T13:04:40.946Z Reads: 112

```
Would a 12s3p also work? Since it has a higher wh than a 10s3p
```

---
## \#17 Posted by: Blitz Posted at: 2019-04-27T13:05:02.552Z Reads: 113

```
Sure but chances are your going to use the same gearing

 I mean I don't know how the Esc works but I bet it's going to be less efficient

going slower on a board thats now because of the higher voltage geared for a higher speed.

Now that's all I'm going to say I still have more opinionated thoughts on that but without knowing how the esc converts the voltage etc I can't say anything more.
```

---
## \#18 Posted by: Michal Posted at: 2019-04-27T13:14:09.627Z Reads: 109

```
Would i get more range if i used 6364 motors for example?
```

---
## \#19 Posted by: Blitz Posted at: 2019-04-27T13:21:35.011Z Reads: 105

```
Your getting into the whelms of advanced esk8 knowledge.

I've read the debates on bigger or smaller motors and if weight is not an issue then the motors you have are totally fine if not better in some peoples opinion.
```

---
## \#20 Posted by: Grozniy Posted at: 2019-04-27T13:23:03.419Z Reads: 101

```
At the end, bigger battery is better. Makes the pack last longer, less sag, more range
```

---
## \#21 Posted by: Blitz Posted at: 2019-04-27T13:24:41.195Z Reads: 94

```
[quote="Grozniy, post:20, topic:91946"]
Makes the pack last longer, less sag, more range
[/quote]
:arrow_up::arrow_up::arrow_up:

This, batteries normally  have a bit more capacity (per cell) if you pull less current
```

---
## \#22 Posted by: Michal Posted at: 2019-04-27T13:25:24.545Z Reads: 92

```
Allright, I think I got what i was looking for. Thanks a lot for the quick answers.
```

---
## \#23 Posted by: riverside.rider Posted at: 2019-04-27T13:27:49.259Z Reads: 93

```
Hi michal
I am using 10s4p (Samsung 30Q) with 2x 6374 190kv Motors....I get a range of 30-35km with the bergmeisters (15:60 gearing ratio) pumped at 5 bar on flats...
My gf said I should lose a few kg (am now at 78kg)

Edit: my gf also said I ride like a granny....(below 40km/h) so if you go nuts then / all terrain then of course your range would be less. But personally I would not go below 10s4p
```

---
## \#24 Posted by: Michal Posted at: 2019-04-27T13:31:48.485Z Reads: 91

```
30-35km!? that's awsome! that's more than double of what I originally planned. Thanks so much for the info.

Also what is the discharge rate of Samsung 30q 18650? I was originally planning to go with with lipos that have a higher discharge than li-ion, paired with a daual fsesc 6.6 that is 100a continous. I was thinking i could downdrade to something like a dual 4.40 plus to save some money. Is this correct thinking or am i completely wrong?
(i'm going a bit off topic, but i didn't want to start a new topic just for this)
```

---
## \#25 Posted by: captclearleft Posted at: 2019-04-27T13:42:11.880Z Reads: 90

```
Hey there Michal,
I just finished a similar build, and I weigh 70kg.  
I went with two 6355 motors, as I was printing my own gears, and the 6374s looked like it might be tight getting them in between my TB210s.  

I am using 3 [4s 5ah Lipos](https://hobbyking.com/en_us/turnigy-heavy-duty-5000mah-4s-60c-lipo-pack-w-xt-90.html)  (as a 12s1p) - I get 16km range.  I was actually hoping for more, but alas, that is what I get.

![drgBoard|375x500](upload://fBF0A8Mg42prBIadTRTEnsMHH7R.jpeg)
```

---
## \#26 Posted by: Michal Posted at: 2019-04-27T13:47:09.075Z Reads: 83

```
Look awsome man. 32km of range, only 5ah? Could I expect something similar with 6474 motors if i would go with lipo instead of li-ion?
```

---
## \#27 Posted by: captclearleft Posted at: 2019-04-27T13:48:57.704Z Reads: 77

```
Shoot, I am so sorry.  Bad at math.  Oh the US standard is Ca Rap...  I get 10 Miles, that is 16 km on this board....  So sorry
```

---
## \#28 Posted by: Michal Posted at: 2019-04-27T13:53:09.242Z Reads: 74

```
I actually wanted 15 km originally so that is actually fine. I could go a little higher, to 6-8ah maybe to be safe.
```

---
## \#29 Posted by: captclearleft Posted at: 2019-04-27T13:53:41.291Z Reads: 73

```
I was pretty disappointing with my range.  I switched from 60t gears (16x60) to 42t gears (16x42) to see if that would help.  I might get a little more range, but my riding has been in different areas.  I know I get 16km for sure.  I am looking at trying to pack more battery underneth at the moment.

@Michal I am hoping that you get better range with the bigger motors.  Next week - I am taking the motors off my board, and I am going to try a single 6374 with (16x50 gears).  I need at least 24km range, or I have to carry extra batteries...
```

---
## \#30 Posted by: Grozniy Posted at: 2019-04-27T14:04:38.070Z Reads: 71

```
10S4P 30Q pack is going to be great, plenty of members use it
```

---
## \#31 Posted by: Michal Posted at: 2019-04-27T15:02:50.036Z Reads: 69

```
Do li-ion have enough dicharge? Becuase the dual fsesc 6.6 has max 100a continuous (tham i am planning to use), same as the motors.
```

---
## \#32 Posted by: Dirt_Bag Posted at: 2019-04-27T15:51:32.486Z Reads: 67

```
10s5p or 6p or 12s5p or 4p. This will give you a fair bit of range and not be a massive pack
```

---
## \#33 Posted by: Dirt_Bag Posted at: 2019-04-27T15:54:46.069Z Reads: 61

```
If you build a pack out of 30q cells you probably want 6p. If you use something like a vtc5 or vt5a you can get by with 5p or 4p. I can build you a 10s pack if you want.
```

---
## \#34 Posted by: taz Posted at: 2019-04-27T15:56:16.400Z Reads: 62

```
You are joking right?
A 12s5p with 30Q cells is not enough for dual 6374?

Also let's not forget that the guy started with 15km required range.
```

---
## \#35 Posted by: Dirt_Bag Posted at: 2019-04-27T15:58:35.018Z Reads: 60

```
It gives you 50a per motor continuous. But he won't pull that for too long. I have seen full blow trampa mtbs with a 5p 30q.

Edit: if you search the word "trampa" almost every build is 4p and 5p. Unless you are doing serious offroading you will be fine
```

---
## \#36 Posted by: taz Posted at: 2019-04-27T16:03:56.991Z Reads: 60

```
A 5p can give 50 battery amps per motor. He won't even pull that on the road. 

The only time he may pull that is if he is heavy and decides to do repeated standing starts to top speed on a steep hill in which case the last of his problems will be the 5p battery.

MTBs are a different story, FWIW I do have a Trampa with a 12s7p 30q but this is not what the OP asked about.
```

---
## \#37 Posted by: Dirt_Bag Posted at: 2019-04-27T16:05:10.479Z Reads: 60

```
I cant tell if you are agreeing or not...
```

---
## \#38 Posted by: taz Posted at: 2019-04-27T16:07:44.653Z Reads: 57

```
I am not agreeing with your statement that a 5p with 30Q cells will not be enough. A 4p 30Q pack will be more than enough for his required 15km range without any considerable sag taking into consideration his weight (72kg) and the type of board he wants to build.
```

---
## \#39 Posted by: Dirt_Bag Posted at: 2019-04-27T16:14:53.690Z Reads: 57

```
Theres been a misunderstanding. Im saying a 5p pack is plenty for 95% of riders. You never pull the max motor current unless you ride like a lunatic while offloading uphill lol
```

---
## \#40 Posted by: taz Posted at: 2019-04-27T16:20:33.230Z Reads: 54

```
I sort of agree with that statement, however I pull the max motor current all the time. This is different to pulling the max battery current.
Uphill offroading does take a lot more out of all the components, hence the reason why most actual eMTB  go for big liion packs or smaller high discharge lipo packs.

How did we end up discussing mountainboards? This is not what the original question was about.
```

---
## \#41 Posted by: Battosaii Posted at: 2019-04-27T16:20:44.095Z Reads: 45

```
10s4p or 12s4p would give you what you want with some leg room to actually ride fast the entire 15km ride. 

3p would be cutting it close with those wheels
```

---
## \#42 Posted by: Michal Posted at: 2019-04-27T16:22:43.621Z Reads: 46

```
So with 10s4p i would go the whole 15km with decent speed, with a little extra "slow range"?
```

---
## \#43 Posted by: taz Posted at: 2019-04-27T16:24:28.215Z Reads: 49

```
Yes. However as already mentioned, a bigger battery is always better up to the point it become too heavy for your application.
```

---
## \#44 Posted by: Dirt_Bag Posted at: 2019-04-27T16:24:49.722Z Reads: 52

```
Idk tbh. Lets not derail it anymore. :sweat_smile:
```

---
## \#45 Posted by: Michal Posted at: 2019-04-27T16:25:15.867Z Reads: 54

```
I don't really have the budget for a bigger battery 

Since the fsesc 6.6 wouldn't be able to pull more than 50a from the battery, could i shange to something like the dual 4.20 plus or even something like this?
https://www.mboards.co/collections/escs/products/dual-belt-driven-motor-esc
```

---
## \#46 Posted by: taz Posted at: 2019-04-27T16:26:00.575Z Reads: 51

```
Then go for the 10s4p and don't look back. It will be more than enough for what you described.
```

---
## \#47 Posted by: Dirt_Bag Posted at: 2019-04-27T16:26:01.982Z Reads: 50

```
I can build you a pack for cheaper than most. If you are interested....
```

---
## \#48 Posted by: taz Posted at: 2019-04-27T16:26:55.209Z Reads: 51

```
Are you in the EU?
```

---
## \#49 Posted by: Michal Posted at: 2019-04-27T16:28:04.906Z Reads: 49

```
How much would you charge for it?
```

---
## \#50 Posted by: Michal Posted at: 2019-04-27T16:28:23.126Z Reads: 49

```
I'm in Norway
```

---
## \#51 Posted by: Dirt_Bag Posted at: 2019-04-27T16:29:15.238Z Reads: 47

```
Oh man. I cant ship international without very expensive hazmat labels. The cost would be absurd.
```

---
## \#52 Posted by: Michal Posted at: 2019-04-27T16:30:11.159Z Reads: 48

```
Bummer, that's allright.
```

---
## \#53 Posted by: Dirt_Bag Posted at: 2019-04-27T16:31:32.844Z Reads: 51

```
I could violate a few laws and risk a 275k fine... but i think that might be a bad idea. Shipping legally would be close to $250 usd
```

---
## \#54 Posted by: Michal Posted at: 2019-04-27T16:33:20.913Z Reads: 48

```
Yeah, don't risk the fine, 250usd isn't a lot less than a whole new battery, so no.
```

---
## \#55 Posted by: taz Posted at: 2019-04-27T16:36:10.187Z Reads: 48

```
[quote="Michal, post:45, topic:91946"]
Since the fsesc 6.6 wouldn’t be able to pull more than 50a from the battery
[/quote]

This is not correct.
```

---
## \#56 Posted by: Dirt_Bag Posted at: 2019-04-27T16:37:28.055Z Reads: 48

```
It can pull nearly 100a from the battery for a long time. I use a dual 6384 mtb and it maxes out the vesc and it handles it great
```

---
## \#57 Posted by: Michal Posted at: 2019-04-27T16:38:25.669Z Reads: 48

```
I was mistaken then, thanks for clarification.
```

---
## \#58 Posted by: Michal Posted at: 2019-04-27T16:51:56.558Z Reads: 47

```
But is it 100a per motor or total?
```

---
## \#59 Posted by: Dirt_Bag Posted at: 2019-04-27T16:56:56.218Z Reads: 49

```
dual fsesc 6.6 is 100a per motor, so 200a total. its an absolute beast. I run it in 12s foc and it hasnt had a single issue since i bought it nearly a year ago
```

---
## \#60 Posted by: Michal Posted at: 2019-04-27T16:58:13.024Z Reads: 49

```
Just to clarify, the li-ion battery is able to supply that?
```

---
## \#61 Posted by: Dirt_Bag Posted at: 2019-04-28T15:33:10.190Z Reads: 34

```
It depends on your battery. Its really overkill for anything but an all terrain build to need more than about 50 amps per motor
```

---
## \#62 Posted by: Michal Posted at: 2019-04-28T15:35:06.315Z Reads: 36

```
But don't 10s4p lithium ions have 40a per motor? Isn't that a bit too little?
```

---
## \#63 Posted by: Dirt_Bag Posted at: 2019-04-28T18:30:27.770Z Reads: 31

```
Its not to bad tbh. 40a goes a long ways.
```

---
## \#64 Posted by: Michal Posted at: 2019-04-28T18:34:05.679Z Reads: 29

```
Do you think I should go lipo maybe? For higher discharge. The esc I'll be using (dual fsesc 6.6) has 100a per motor and wouldn't the be kind of wasting its power?
```

---
## \#65 Posted by: Dirt_Bag Posted at: 2019-04-29T05:29:04.926Z Reads: 25

```
You really dont need it. At 40a per motor with dual 6374s, you will be thrown from the board if the floor it. If you are worried, add one more p group to your pack. You wont be dissapointed unless you are doing absurd offroad stuff

If you want even more torque, buy the 149kv sk3 instead. Most people dont need high speed anyway
```

---
## \#66 Posted by: Michal Posted at: 2019-04-29T06:29:40.313Z Reads: 24

```
Do you know a reputable supplier for li-ion packs? I was looking at the mboards packs but those only go up to 4p.
```

---
## \#67 Posted by: xsynatic Posted at: 2019-04-29T10:36:00.317Z Reads: 19

```
I'm looking for a pack too.

Not sure if i want 12s5p or 10s5p. 
I currently use a single sk3 6374 but will Switch to dual 6374 with MBS 8" tires. The minimum range i want is 35km.
```

---
