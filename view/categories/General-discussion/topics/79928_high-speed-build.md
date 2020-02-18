# High Speed Build

### Replies: 79 Views: 699

## \#1 Posted by: Phillisuper Posted at: 2019-01-04T23:40:44.392Z Reads: 189

```
So I am trying to decide what to use for my first build and am looking for advice.  I decided to build a board because no production board offered quite what I wanted.  I plan on using this board to commute on a 35 mph road so my speed goal is at least 40 mph on the top end,preferably 45.  I also want a range of at least 25 miles per charge.  I plan on building my own battery with Samsung 30Q's.  I am thinking 10s4p or 12s4p.  My problem comes when I get to the VSEC and Motors.  I want to use atleast 97mm wheels and gearing down to a 2:1 reduction.  I plan on having a dual motor set up.  My real questions are, should I use one VSEC or 2.  Also, should I go with a higher Kv for my motor or no?  I know that I have the potential to reach higher speeds with a higher Kv motor, but with larger wheels and the gear ratio I am worried about losing too much torque (all the roads here are flat, I'm more worried about over taxing the motors by removing that much torque).  Any suggestions for motors and VSEC? Also do you think the battery, gear reduction, and wheel size will get me to the 40-45 in the real world (im 155 lbs)?  Thanks for your help.
```

---
## \#2 Posted by: Benjamin899 Posted at: 2019-01-04T23:56:22.391Z Reads: 175

```
ok that range for that speed with that battery is not possible. If you drive it that fast you burn alot.
This calculator will help you with that.
https://calc.3dservisas.eu/
Each motor need one controller.
```

---
## \#3 Posted by: Phillisuper Posted at: 2019-01-04T23:59:23.459Z Reads: 169

```
What would you recommend for the battery? How many cells can you run parallel?
```

---
## \#4 Posted by: Benjamin899 Posted at: 2019-01-05T00:01:19.932Z Reads: 167

```
how many you want. I suggest you read the FAQ's and search around.
```

---
## \#5 Posted by: mynamesmatt Posted at: 2019-01-05T00:08:27.704Z Reads: 161

```
https://www.electric-skateboard.builders/search
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-01-05T00:09:17.238Z Reads: 153

```
omg where did you find this?!one?

![](http://i.imgur.com/sW22vPs.gif)
```

---
## \#7 Posted by: venom121212 Posted at: 2019-01-05T00:11:46.138Z Reads: 146

```
It's the funny shaped Q at the top :wink:
```

---
## \#8 Posted by: mynamesmatt Posted at: 2019-01-05T00:20:39.225Z Reads: 143

```
no idea!1!1!1 i happened to click it one day!
```

---
## \#9 Posted by: Sn4pz Posted at: 2019-01-05T00:21:28.543Z Reads: 142

```
AmAzInG !!1111111one!11SINGULARUNIT1
```

---
## \#10 Posted by: taz Posted at: 2019-01-05T00:24:20.866Z Reads: 137

```
I am not sure you are realising what you are getting yourself into.
Riding an electric skateboard at 40-45mph around cars commuting is a sure way of getting yourself seriously injured.
```

---
## \#11 Posted by: Skunk Posted at: 2019-01-05T00:25:02.041Z Reads: 135

```
Obviously it's recommended to use the search function cuz most of this information is out there.
Sometimes people will hand feed you the answers and sometimes the guys will Hackle you like this.
Don't take it personally, keep thick skin.

If you searched and searched and searched and honestly can't find your answer 
Ask here https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/3099

If it's a topic that has never been discussed then a new thread is appropriate.

I think going your gonna want bare minimum at 12d6p.
Keep in mind that's going to take a while to charge so if you plan on making that trip more than once a day you better have a few hours in between
```

---
## \#12 Posted by: Trdolan03 Posted at: 2019-01-05T00:38:37.884Z Reads: 128

```
Go Vesc 6 for this thing. And yes, you are going to need at least 6p. Do you have downhill experience?? 45mph is crazy
```

---
## \#13 Posted by: Jacobee Posted at: 2019-01-05T00:49:17.641Z Reads: 127

```
In my opinion if you want to go 35+ mph on roads with cars maybe consider an ebike. It'll be more stable. But if you do want a electric skateboard you're going to want dual (for better breaks just as much as the better acceleration). Probably 12s5 or 6p and dual 6374s.
```

---
## \#14 Posted by: Phillisuper Posted at: 2019-01-05T01:01:15.555Z Reads: 127

```
I am using it to commute at university, the majority of the time I will be a 25 (because most roads there are that limit).  The reason I want the ability to go that speed is incase I want to go somewhere close like the drug store or a restaurant, I dont want to have to move my car (parking is really bad at LSU).  The limit on that road is 35 so my primary goal is to go 35.  If i am maxing out at 35 though cars are going to try to pass me and then I really am in serious danger.  I would prefer to have the ability to move a bit faster should I need to.  I have full biker gear (full face helmet, leather jacket, pads) I am trying to mitigate risks as much as I can.  The way I see it though, I'm safer going the speed of the cars around me than going slower than them and having them trying to pass me.
```

---
## \#15 Posted by: Phillisuper Posted at: 2019-01-05T01:05:30.575Z Reads: 124

```
I have a little, I live outside New Orleans so the only hill I have is the bridge that crosses the intercoastal water way.  the fastest I've gone to date though is just over 30.  So would a Vesc 6 be better then running two Vesc 4s?
```

---
## \#16 Posted by: Jacobee Posted at: 2019-01-05T01:26:35.015Z Reads: 122

```
You'll probably want a focbox unity. They're super robust. You can read about @longhairedboy 's experience with it. Idk about vesc 6s. If ou really want a vesc 6 you can either get them from trampa at about $300 a piece or get a dual vesc 6 from flipsky for about $270.  Idk how good  quality the flipsky are tho.
http://www./2018/12/21/my-time-with-enertions-unity-beta-1-foc-motor-controller/
```

---
## \#17 Posted by: Benjamin899 Posted at: 2019-01-05T01:32:41.806Z Reads: 121

```
ok that is not rly practical. If you want to go that fast and you always slap on your gear, you are probably faster with a car. Also have you ever riden that fast? As a commuter that board will be heavy and big. But at the end it is your decision.
```

---
## \#18 Posted by: tardyparty7 Posted at: 2019-01-05T01:45:10.957Z Reads: 122

```
if this is ur first board, thats pretty challenging. Going that fast might get u hurt if you've never ridden a eboard. i was wanting a top of the line board really fast and really good range but then i was **practical.** (plus im 12 so going 30mph is pretttyyyyy stooooopiiiidddd to do.) anyways, u can go 35, but the range won't be that good. if u want a board thats super good, get a @longhairedboy or a @Kaly board thats top of the line. If u wanna build something somewhat close, ur gonna need a hella good battery.
```

---
## \#19 Posted by: Phillisuper Posted at: 2019-01-05T01:45:28.294Z Reads: 118

```
Its not about it being faster to get there with my car, its about moving my car.  My res-hall doesn't have its own lot so it's a hastle to find a decent spot if I leave in the middle of the day.  The only time it is easy to find a spot is between 7 and 12 when the majority of the bar hopping is going on.  I know its gonna be heavy, I have another board I use to get to classes, this one is meant to take me to destinations that require transit on a high speed limit road.  I am hoping to keep it below 30 lbs (25 would be great)
```

---
## \#20 Posted by: Phillisuper Posted at: 2019-01-05T01:47:35.130Z Reads: 118

```
This will be my 3rd eboard, just my first diy.  Plus I'm 19 so my teenage mind refuses to take no for an answer lol.
```

---
## \#21 Posted by: tardyparty7 Posted at: 2019-01-05T01:48:39.416Z Reads: 109

```
ohhhh, u should've put that up there. (or i didn't read carefully). what boards? that'll give us ur experience in a nutshell. and how long have u had them/miles?
```

---
## \#22 Posted by: Phillisuper Posted at: 2019-01-05T01:54:14.063Z Reads: 108

```
I own a Koowheel (yes a very shitty chinese board) which only got like 23 mph.  My newest board is the Backfire Galaxy 2S which I have gotten 26 out of.  Ive been long-boarding  since I turned 16, but didn't pick up eboarding until just over a year ago.  Im certainly more seasoned in long-boarding than I am in DIY.  The whole reason I got into this idea was because I didnt want to buy a Boosted Stealth or Evolve GTX (boosted didnt have desired specs and I hear evolve's are anything but reliable).
```

---
## \#23 Posted by: tardyparty7 Posted at: 2019-01-05T01:54:26.585Z Reads: 107

```
also, 10s4p will not get u close to that range and speed. 12s4p maybe will get u closer. u'll need a better battery than that. get a 13sSomething or maybe this will get u closer: 
https://longhairedboy.com/collections/all/products/high-powered-electric-skateboard-battery-pack-43v-12s5p-samsung-inr18650-30q

 a 12s8p is really good and @eboosted makes some good enclosures that can go with Trampa's Holypro deck:
https://www.eboardsperu.com/product/12s8p-flexible-battery-pack-for-hs11-holypro-ds-enclosure/
https://www.eboardsperu.com/product/trampa-hs11-holypro-35-ds/
```

---
## \#24 Posted by: Phillisuper Posted at: 2019-01-05T01:56:06.660Z Reads: 102

```
I plan on making my own battery, perhaps a 13s6p, as I see the focbox unity can apparently handle it
```

---
## \#25 Posted by: tardyparty7 Posted at: 2019-01-05T01:58:11.955Z Reads: 101

```
[quote="Phillisuper, post:22, topic:79928"]
and I hear evolve’s are anything but reliable
[/quote]

yeah basically. even the jump of 26 to 30 is huge, or at least the feeling. now going 40 on a car might not seem crazy speeds, but think abt it. ur standing on a deck: a helmet and armour are the only things blocking u from the concrete. 

how fast have u gone on a longboard before? not an eboard but a longboard.
```

---
## \#26 Posted by: Phillisuper Posted at: 2019-01-05T01:59:43.428Z Reads: 94

```
A bit above 30.  I didn't have a speed app up but my friend that was driving behidn me to keep me from getting hit said we were above 30 the majority of the time.
```

---
## \#27 Posted by: tardyparty7 Posted at: 2019-01-05T02:01:24.808Z Reads: 92

```
damn. well i think ur ready but 45 would turn my legs to jelly. :rofl: i think u've done ur research well, but 45 speed and 25 range is almost impossible with todays tech. i think u could get a really high top speed but a meh range.
```

---
## \#28 Posted by: Phillisuper Posted at: 2019-01-05T02:03:52.175Z Reads: 92

```
I really don't need 25, it is more of a "perfect set up" scenario.  15 would do fine
```

---
## \#29 Posted by: Phillisuper Posted at: 2019-01-05T02:04:53.297Z Reads: 89

```
the furthest I actually plan on taking it is like 4 miles, I just want extra so I'm not running out of juice on the way back
```

---
## \#30 Posted by: Skunk Posted at: 2019-01-05T02:05:23.105Z Reads: 89

```
Theres really not a large number for members gearing thier boards for above 35mph.
Just a few above 40mph.
Lots of out boards will. But most chose to gear towards acceleration. 
So you need to go 35+ because of traffic?.  I take it you'll be riding in the middle of the road than?
```

---
## \#31 Posted by: Skunk Posted at: 2019-01-05T02:06:28.287Z Reads: 90

```
I totally get making sure you have extra battery so you're never be without. luckily you have multiple boards so you should always have one charging.
Keep in mind. Bigger battery longer charge.
```

---
## \#32 Posted by: tardyparty7 Posted at: 2019-01-05T02:06:31.613Z Reads: 91

```
oh. idk what i was doing but i put in ur battery and 2wd and 30:15 (2:1) and got 44.95 mph and 14.5 range. u just check it out:

https://calc.3dservisas.eu/?Tc_NCsIwEATgd8lZJDFpq16j9KQECvZue4hgbKBH8d3dmcaf27fL7mzyVFcf1V7db9NDraQ4S2HXtXj2ndhYMggd5TGgtWZxQGWqxZjZLH1mGmFGBiLy314OXYnLgUsQo2xFolmT36Ah-pI0xKNoq8kL1h2cfElKfHbDXphgR_7uJ882hsd-BnUDt6fPb8a25ziIazutXm8=
```

---
## \#33 Posted by: Phillisuper Posted at: 2019-01-05T02:07:01.028Z Reads: 89

```
That is the plan, I'd prefer to move the same speed as the cars so they regard me as another vehicle, not half their speed and end up getting clipped when they pass me.
```

---
## \#34 Posted by: Skunk Posted at: 2019-01-05T02:08:22.801Z Reads: 86

```
Do you know what the laws are for e powered things in your state?
Going 20s on a board doesn't get cops attention very often. going 35 + in the middle of the road does
```

---
## \#35 Posted by: tardyparty7 Posted at: 2019-01-05T02:12:27.540Z Reads: 88

```
from www.evelo.com site:

#### **DEFINITION OF ELECTRIC BIKE:**

The state of Louisiana (LA) defines electric bikes as a motorized bicycle with pedals and propelled by human power with a helper motor or both. The motor must be rated no more than 50cc, have an automatic transmission and designed to have a maximum speed of not more than 25mph on flat surface.
```

---
## \#36 Posted by: tardyparty7 Posted at: 2019-01-05T02:13:08.297Z Reads: 85

```
good luck my dude.
```

---
## \#37 Posted by: Phillisuper Posted at: 2019-01-05T02:14:46.866Z Reads: 87

```
From what I can tell they are not mentioned whatsoever.  There is no statutes about (electric vehicles).  The closest I could find were laws on mopeds and The laws certainly don't apply to these (and even if they did, the law was have a valid license which I have)
```

---
## \#38 Posted by: Skunk Posted at: 2019-01-05T02:16:52.145Z Reads: 87

```
There are no esk8 laws in Oregon but I fall under moped laws of non-motorized vehicles be default
```

---
## \#39 Posted by: tardyparty7 Posted at: 2019-01-05T02:17:14.216Z Reads: 91

```
look up :point_up:
```

---
## \#40 Posted by: Jacobee Posted at: 2019-01-05T02:17:31.860Z Reads: 90

```
Exactly so it's a grey area. A cop will see you going about 20 through campus and not think much. But by going 35+ through traffic and they are more inclined to pull you over. All it takes is one asshole cop to pull you over and confiscate your board.
```

---
## \#41 Posted by: Skunk Posted at: 2019-01-05T02:18:58.790Z Reads: 85

```
I think you're better off building a board that gets solid low thirties and good range and just take a different roundabout route
```

---
## \#42 Posted by: Saturn_Corp Posted at: 2019-01-05T02:19:26.928Z Reads: 81

```
This board will probably weigh 30 lbs or more due to all the cells you need to strap to it. 

Don't run stop signs and red lights or topple over old ladies at crosswalks and police probably won't care. Often that is the case.
```

---
## \#43 Posted by: dareno Posted at: 2019-01-05T02:19:48.847Z Reads: 82

```
There is a huge difference between 30mph and +40.  I mean huge.  The slightest movement or weight change can have a catastrophic result if you don't know what you're doing.   Riding +40 on roads with cars is tantamount to suicide if you are inexperienced.  Small rocks can undo you, sticks will see you in the air and going that fast your manoeuvrability is severely hindered. My advice is to build a 30mph board with torque.  Lots of torque and stick to the bike lanes.
```

---
## \#44 Posted by: Skunk Posted at: 2019-01-05T02:20:32.413Z Reads: 80

```
You really don't think a cops going to Blink an eye at someone on a skateboard trying to keep up with traffic in the middle of the road going over 35 miles per hour?
```

---
## \#45 Posted by: Phillisuper Posted at: 2019-01-05T02:21:34.773Z Reads: 81

```
I am taking a roundabout route, its a two lane road with a 35 speed limit rather than the highway with a 55 speed limit.  I just want the extra speed incase I need it.  I intend to stay closer to the 35 mark.
```

---
## \#46 Posted by: Phillisuper Posted at: 2019-01-05T02:22:08.630Z Reads: 81

```
They tend to not down here.  SO long as you dont speed they really don't care
```

---
## \#47 Posted by: dareno Posted at: 2019-01-05T02:23:22.577Z Reads: 82

```
[quote="Phillisuper, post:45, topic:79928"]
I just want the extra speed incase I need it.
[/quote]

Lies.  Absolute bold faced lies.  You want a 40mph board because you are 19 and indestructible.  :rofl:
I was exactly the same and still am tbh.  :sunglasses:
```

---
## \#48 Posted by: Phillisuper Posted at: 2019-01-05T02:24:31.298Z Reads: 81

```
I'll just say I'll drive my board like I drive my car, if there is something infront of me I'll go the speed its going ;)
```

---
## \#49 Posted by: dareno Posted at: 2019-01-05T02:25:30.717Z Reads: 80

```
Just be careful sunshine thats all I'm saying and all I can say as my latest set up does that shit.
```

---
## \#50 Posted by: Skunk Posted at: 2019-01-05T02:25:53.480Z Reads: 75

```
Hopefully people where you live are good drivers. Im fucking nuts and i don't trust other drivers at those speeds to ride with traffic.
```

---
## \#51 Posted by: Phillisuper Posted at: 2019-01-05T02:26:40.992Z Reads: 72

```
I'll be sure to keep that in mind
```

---
## \#52 Posted by: Saturn_Corp Posted at: 2019-01-05T02:27:10.069Z Reads: 70

```
I suppose it can vary widely across the world for many factors buy generally yes. 35 is a bit fast but like @Phillisuper said it wouldn't be the for the majority of the trip. You do have to be very careful at those speeds though especially in an urban environment.

How's the traffic where you live Phil?
```

---
## \#53 Posted by: Skunk Posted at: 2019-01-05T02:27:46.698Z Reads: 73

```
[quote="Phillisuper, post:37, topic:79928"]
The laws certainly don’t apply to these (and even if they did, the law was have a valid license which I have)
[/quote]

They do in my state.  Anything over 25 needs a license and registration.
```

---
## \#54 Posted by: Phillisuper Posted at: 2019-01-05T02:29:40.428Z Reads: 74

```
It depends on the time of day.  I live in the Capital city so afternoons are really bad on the highway.  Since I stay on the smaller roads though and they only really go to and from the college/surrounding neighborhoods we really only get traffic on the weekends when everyone is either coming from or going home.
```

---
## \#55 Posted by: tardyparty7 Posted at: 2019-01-05T02:30:20.419Z Reads: 73

```
just talk to @Skunk abt his injuries.
```

---
## \#56 Posted by: Phillisuper Posted at: 2019-01-05T02:30:25.321Z Reads: 74

```
I'll look into that.  I know a few officers so ill ask and if they aren't sure I'll get in contact with the DMV
```

---
## \#57 Posted by: Skunk Posted at: 2019-01-05T02:31:01.710Z Reads: 77

```
Hey what can i say.  I live for adrenaline
```

---
## \#58 Posted by: tardyparty7 Posted at: 2019-01-05T02:31:04.364Z Reads: 77

```
no don't. then'll they'll find u and take ur boards. jk
```

---
## \#59 Posted by: Phillisuper Posted at: 2019-01-05T02:31:54.388Z Reads: 77

```
I only live in New Orleans part time since i board at LSU.  The big one will stay up there so the NO cops can't get it lol
```

---
## \#60 Posted by: Skunk Posted at: 2019-01-05T02:33:56.838Z Reads: 79

```
In reality the cops aren't worried about you or your safety going those speeds, they're worried about you causing an accident in traffic at those speeds.
And if you cause an accident you don't exactly have skateboard insurance to cover the damages.....
```

---
## \#61 Posted by: tardyparty7 Posted at: 2019-01-05T02:34:33.134Z Reads: 76

```
no, not skateboard insurance, medical insurance and life insurance.
```

---
## \#62 Posted by: mynamesmatt Posted at: 2019-01-05T02:35:26.770Z Reads: 76

```
[quote="Skunk, post:11, topic:79928"]
Sometimes people will hand feed you the answers and sometimes the guys will Hackle you like this.
[/quote]

aren't you the epitome of exactly this
```

---
## \#63 Posted by: Skunk Posted at: 2019-01-05T02:36:03.758Z Reads: 77

```
I do both.... lol depends on my mood
```

---
## \#64 Posted by: tardyparty7 Posted at: 2019-01-05T02:36:49.028Z Reads: 75

```
i think he does it when they're experienced or have been on this forum long enough.
```

---
## \#65 Posted by: Skunk Posted at: 2019-01-05T02:37:49.442Z Reads: 74

```
Im a nood and haven't been here a year yet lol
```

---
## \#66 Posted by: dareno Posted at: 2019-01-05T02:38:27.934Z Reads: 74

```
He does it because sometimes hes a miserable bastard. :wink:
```

---
## \#67 Posted by: Friskies Posted at: 2019-01-05T02:53:16.074Z Reads: 74

```
I'll try and word this a bit differently for you. 

We aren't trying to discoutage you because we are jelous. We say don't do it because it's outright dangerous. All these people have chimed in because they are concerned that you will end up with a board that goes super fast, you jump on it and lose control and seriously injure or even kill yourself in a traffic incident. 

By the sounds of it you have a couple of production boards and yes, some of them can go decent speeds but none of them are even close to what you are looking at doing. There are a few here that came from downhill and I can guarantee myself **Once you hit 35mph, you do not want to have a wobble or obstacle in front of you**.

Just take a moment and see what other have done and are building. I'm looking forward to seeing your build thread. It will be awesome seeing another diy board in the scene :smile:
```

---
## \#68 Posted by: Phillisuper Posted at: 2019-01-05T02:59:29.332Z Reads: 66

```
I know y'all are just looking out for me lol.  I more want to do it just to do it.  I will likely do just that, ride above 35, get a speed wobble and never ride it again (or crash who knows lol).  If it makes sense, I want to build it to go as fast and as far as possible and see what happens.  We'll see where it goes though.  Build thread will likely not happen for a while because the FB unity will take several months to ship.  Maybe ill post when I build my 13s6p batter.
```

---
## \#69 Posted by: Skunk Posted at: 2019-01-05T03:27:10.418Z Reads: 69

```
https://www.electric-skateboard.builders/t/usa-canada-focbox-unity-gb-extra-units-available/65080/122?u=skunk
```

---
## \#70 Posted by: Trdolan03 Posted at: 2019-01-05T03:37:39.845Z Reads: 72

```
Here is my advice in terms of the actual board. You want bindings and pneumatics on 16” trucks. At those speeds, you need the wider trucks for stability. And bindings are crucial to recovering from bad roads. Would never go faster than 25 without bindings. Pneumatics will get better traction which will be paramount for you.
```

---
## \#71 Posted by: Phillisuper Posted at: 2019-01-05T04:15:32.520Z Reads: 71

```
Thanks, do you have a specific truck you recommend from experience? Although I've done a little downhill my main area of familiarity is with cruiser boards.
```

---
## \#72 Posted by: Trdolan03 Posted at: 2019-01-05T05:32:17.890Z Reads: 68

```
I’ve used all of the @trampa 16” trucks with good success. @MBS also makes great quality trucks.
```

---
## \#73 Posted by: Lunasi Posted at: 2019-01-05T05:43:57.351Z Reads: 68

```
Careful, 45mph will give you the wobbles, watch me ride at that. 

https://youtu.be/b_uqtqzmRPQ?t=595
```

---
## \#74 Posted by: Trdolan03 Posted at: 2019-01-05T05:55:51.953Z Reads: 69

```
That is the basis of my recommendation. To try and avoid speed wobbles by getting super wide trucks and smooth pneumatics
```

---
## \#75 Posted by: Skunk Posted at: 2019-01-05T06:30:28.090Z Reads: 67

```
I think there's a point where wide becomes less stable tho too.
Look at any downhill longboarding truck. They rock 179mm and under.
Pneumatic definitely have better grip. But they cut your range by a noticeable amount.
```

---
## \#76 Posted by: sayekim Posted at: 2019-01-05T08:11:12.729Z Reads: 72

```
Going 40-45 is crazy fast on a board. I have gone max 35 and I don’t plan to go faster any longer like I used to think I would. 

This is not because it isn’t doable but because it’s gonna hurt when you fall and you might break a bone or two not to mention get run over since you are going to do it on a road. 

Be sure to put on that gear every time and never once think you’ll be fine without any of it ever. 

I have fallen going 23mph from a wobble I caught from an edge on a bike path and all I was wearing was a half shell skate helmet and no other gear. This broke my shoulder socket, blade, collarbone, and a few ribs which resulted in my lung collaps too.  

Here is how it looks to put a little reality into your perspective. 

![image|375x500](upload://k2ZkFLvKmXYVA2bPLvJ2dKzLcq7.jpeg) 

![image|666x500](upload://zmzUS6wTXDpR1hJu31P5qhgVbFw.jpeg) 

Luckily I was wearing jeans pants and jacket or I would have had serious road burn too. 
It was a full on sideways dive and slide into my left side. My head luckily hardly touched the ground since I automatically make sure of that when I fall appearently. 
I never ride without full body armor and full face helmet since and knee pads too. 

I also never have to ride on roads since there are plenty of bike paths to go around here in the Netherlands. 

Having said all this I do look forward to this fast build of yours. 

I run a 12s6p 30q with 6374 maytech motors on a 15/36 gearing on 97mm which gives me a nice and comfortable 32mph top speed. 
The acceleration is awesome and it’s all I care for now. Even going from 20 to 30 kicks ass. 

I use escape for controller. 
Settings are:
80 motor max
-60 motor min
60 batt max
-30 batt min

Range I still need to test further but with the current 41F and occasional 30mph sprints but usually 25 mph constants I get just 25 miles out of the battery and I need to stay under 20 for the last 5 miles until the battery is empty at 34 volts. 

I expect it to be at least 25% better with warmer temperatures.
```

---
## \#77 Posted by: Arzamenable Posted at: 2019-01-05T08:18:37.056Z Reads: 70

```
I touch low 30s taking off with traffic here and there. The jump to 40 is crazy. I only do it in empty, especially flat parking lots, and then Post to Instagram my runs for good measure. 👍
```

---
## \#78 Posted by: Phillisuper Posted at: 2019-01-05T14:13:11.501Z Reads: 63

```
Wide trucks are meant for carving though.  Smaller trucks allow less leverage and thus minor adjustments make less difference?  Right?
```

---
## \#79 Posted by: youseekcota Posted at: 2019-01-13T04:53:58.174Z Reads: 44

```
Just completed a Torqueboards Pro3 12s4p dual 6374 belts geared 14-36 on 97mm wheels. Today I checked my top speed by gps, and It's a fraction over thirty.

Second the fullface helmet, knees, body armor and sliding gloves. Yesterday I had a crash that would have sent me to the ER, but instead I just hopped back on and kept going.
```

---
