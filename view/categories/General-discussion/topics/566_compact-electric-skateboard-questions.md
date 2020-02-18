# Compact Electric Skateboard questions

### Replies: 25 Views: 3803

## \#1 Posted by: PennE Posted at: 2015-11-23T15:05:02.253Z Reads: 164

```
Hi all,
first post on the forum but I've been lurking and reading around for a while now.
I'm a First-year Product Design student at Falmouth University,
looking to build a compact E-board for commuting and general everyday use, and
have a few questions before I start out.
To clarify, before anyone asks, I am not new to brushless power systems (6 years building multirotor aircraft), 
nor am I new to building skateboards (10+ years making my own decks and selling custom setups).
I am, however, inexperienced in combining the two.

The design is for a 24" "penny" style deck, running four small motors similar to the kind we use on small scale multirotors, rather than one or two larger ones. The hope is that this will allow for an overall lighter build for the same power output,
while also reducing torque steer and improving grip. Are there any glaring issues with this layout? haven't seen many 4wd boards around and I'm not really sure why, am I missing something?

I'm looking at using four 28-14 500kv motors on 4s, with two 4000mAh lipo packs in parallel. Based on my research so far it looks like (??) this should be a decent setup, and should achieve about 2.1KW at the wheels(525W/motor) which is of course overkill for a small board so I'd need some sort of soft-start on the escs. Mainly just want that much power for climbing hills since both here (penryn, cornwall) and at home (san francisco) I live in very hilly areas.

As for ESCS, I'm not sure where to start. I originally considered going with R/C car escs, for the high peak current rating and (albeit non-regenerative) braking, but I'm now thinking I should look for something more application specific.
Any advice on this? Somewhat lost as to where to start on this front.

Planning to use Darkwolf's GT2B mod for control.

Below is a render from my conceptual cad model of the board, just to give an idea of what I'm going for here. (belts and wiring aren't pictured because they slow down the render about 100-fold.)
<img src="/uploads/db1493/original/2X/9/9d3e461094a6e4584f16ff8535c312ee717ed58b.jpg" width="666" height="500">
```

---
## \#2 Posted by: kai Posted at: 2015-11-23T15:23:04.360Z Reads: 160

```
are your 4 motors lighter then 2 bigger ones? you also now have 2 more mounts, belts and hubs ect. will it really be lighter? did you already do that calculation? just wondering since you are going for a light board. you will also have 4 esc's and more wires. say you decide to use the vesc as your esc... 480usd later just on the esc's you need =O. I want to see a 4wd penny board though!
```

---
## \#3 Posted by: locktight Posted at: 2015-11-23T16:42:03.475Z Reads: 156

```
if you are going for 4wd then you will have to use 4 escs and four motors. i think a good place to draw from in this build will be the quadrocopter industry. they have to keep things as light and power effective as possible a good website for this is http://www.getfpv.com/ they have some really cool small escs and good motors. i have been hearing good things about avroto motors and cobra motors they are a little expensive but are really high quality. you will have to make your own lightweight small motor mounts. i personally think if i were to try and make a compact board i would go for single wheel drive but a 4wd compact board would be sick.

good luck, Hans
```

---
## \#4 Posted by: cmatson Posted at: 2015-11-23T17:33:56.660Z Reads: 150

```
I think the reason you don't see more 4wd drive boards is because you need to have 4 of basically everything... That can get expensive really fast. In your case, you are compensating by going with the smaller motors, less powerful battery, etc, while still getting the same power as a normal 2wd board (I'm still not sure about your hill climbing goals in San Francisco, but hey, you never know until you try!)

I still think you could just get the same performance, with less weight, and lower costs if you used two motors.

You'd need less esc's, less motors (I know, they will weigh more) and you'd only have two motor pulley setups as apposed to 4. I think fiddling with 4 belt drives is where your weight savings are going to go out the window, and just overcomplicates everything, but who knows, I haven't seem it done before!

So I think in theory this is a really solid concept, but will just have to wait until real world performance to see if it's worth it. I'm a little skeptical about the hill climbing, but again, that depends on a lot of factors like gearing, weight or rider, etc.  

it's definitely something new, which is always cool to see.
```

---
## \#5 Posted by: longhairedboy Posted at: 2015-11-23T18:30:51.014Z Reads: 148

```
@cmatson is dead on here. unless you plan on using hub motors on all four wheels and creating some kind of stack of ESCs... and how many watt-hours can you cram on a board that size with 4 ESCs... 

my advice is twin hub motors and as many power cells as you can layer in behind those dual ESCs. If the deck is thick enough you could try embedding some of the electronics into the deck so that you could layer some fat-n-flat prismatic cells on top of them... 

Whatever happens, this will be a good one to watch.
```

---
## \#6 Posted by: PennE Posted at: 2015-11-23T21:06:07.535Z Reads: 151

```
I'm pretty experienced in the quad industry, that's actually where I got the idea to do it this way in the first place,
as re-purposing the motors designed for ~300-400mm sized racing quads would give me four 500-550 watt motors for under $15 a pop, and escs rated for continuous draw of 60 amps on 4-5s lipo, with active braking (albeit not regenerative) for about the same (the ones I'm currently looking at cost $17 each).
making motor mounts isn't a huge issue, I've got access to a couple 3-axis cnc mills through the university, and they have a 6-axis arriving in about a month.
also, if people on here are working on custom motor controllers (just started reading up on the vesc), you should look at some of the custom firmwares for multirotor escs, like blheli or simonk, along with oneshot. Most people building multirotors these days are running escs with 499hz tick rate, which allows for incredibly smooth and low-latency control of the motors.
The only thing I can really see that I lose by going with multirotor hardware is regenerative braking... I don't know much about it but anyone have rough figures of the percentage of the range you can generally expect to gain  by having regenerative braking?
```

---
## \#7 Posted by: cmatson Posted at: 2015-11-23T21:13:14.411Z Reads: 143

```
Regen braking won't make a huge difference, and I definitely wouldn't worry over it. It's a 'nice to have' but no where near a 'need to have'
```

---
## \#8 Posted by: PennE Posted at: 2015-11-23T21:17:00.294Z Reads: 150

```
Thanks so much for all the responses guys, really looking forward to this project and already loving this community
finished a rough part-out of the electronics and so far it's coming out to around $170 for four 28-15 400kv 500-550W motors,
four 60 amps escs that I'll be writing a custom firmware for based on the blheli source code, but adding active braking, a gt-2b that I'll be doing darkwolf's mod on, and two 5s 4ah packs that I'll be splitting up and soldering into a custom pack to fit within the housing.

Bonus, I got a bit bored in my cad lecture today so here's a few more concept renders in alternate materials.
<img src="/uploads/db1493/original/2X/f/f227d6105b4d12c05b05fa1f01ae4dd2a6575224.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/0/093c640c681afb1796c07869e24ee62992bba8a2.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/f/f7edf974dd06a9e10a19c5b764ea7abb83369baa.jpg" width="690" height="388">
```

---
## \#9 Posted by: kai Posted at: 2015-11-23T21:18:26.424Z Reads: 141

```
sounds like you got it all figured out. cant wait to see your results!
```

---
## \#10 Posted by: onloop Posted at: 2015-11-23T21:38:43.542Z Reads: 142

```
I like that your thinking outside the box, we need more people willing to try new concepts and considering the reasonably low cost you mentioned for the motors & ESC it seems like a viable project... also your area of expertise is using those smaller components, so you will be able to effectively gauge how they perform and make educated decisions better than others who don't have the knowledge! 

I would suggest 3mm pitch belts, near 5;1 reduction ratios... the belts will need to be 15mm wide.

Drivetrain something like:
12T motor pulley
60T wheel pulley
83mm Wheel
500kv
15volts

= 7400rpm
23km/h 

I suppose this all depends on how fast you want to go? 23km/h is fairly slow. Maybe need 6S batteries.

It should have impressive torque whilst running at fairly high RPM and hopefully with the high reduction ratios with less load on the motors overheating will be minimized.
```

---
## \#11 Posted by: PennE Posted at: 2015-11-23T22:04:57.452Z Reads: 134

```
Thanks so much.
Since I've gotten most of my experience from aircraft power systems the reduction ratios and belt drive systems are where I lack knowledge, and you've literally just given me all the information i had been trying to figure out in one post.
not really looking to go much faster than that, 23km/h is about the fastest I'd want to go on this thing, at least at first. it's a 24" deck after all. and the low speed with ~2kw of power should be really nice for climbing hills too.
I'm gonna order the parts in a couple days, and I'll start posting pics of the build as it progresses.
thanks for all the help everyone!
```

---
## \#12 Posted by: locktight Posted at: 2015-11-23T22:12:58.961Z Reads: 129

```
Can you list exactly which parts you are using? I love howmuch you can do on the quadrocopers now. With the naze 32 the possibilities are endless. It's kind of like what the vesc has done for our community.
```

---
## \#13 Posted by: onloop Posted at: 2015-11-23T23:52:59.969Z Reads: 128

```
also you might want to read this 

http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53
```

---
## \#14 Posted by: siggs3000 Posted at: 2015-11-24T03:37:06.728Z Reads: 126

```
This could be a really cool build. If this sort of mini board is feasible for (what seems to be) a really reasonable price compared to the longboards all of us are using, everyone would want to have one to keep in their trunk, dorm room, office, etc. 

They would be light, cheap and they don't need to be crazy fast (in fact going fast on a Penny is terrifying) so they really make a lot of sense. 

I was originally thinking that this was a perfect case for hubmotors (or maybe just one hub motor) but maybe this way could be even better. Looking forward to seeing it.
```

---
## \#15 Posted by: onloop Posted at: 2015-11-24T03:45:55.282Z Reads: 122

```
Also, if you use really small motors, that also means the wheel diameter can be much smaller so the total weight goes down as a result, big wheels are heavy, also you get more torque too.
```

---
## \#16 Posted by: longhairedboy Posted at: 2015-11-24T12:47:25.852Z Reads: 115

```
Its packing over 2000 watts of motors onto an 18 volt, 8ah lipo penny board. we're looking at what.. 144ish watthours ... what kind of range were you expecting? With a top speed of 14mph it seems like a 150 lb man might get about 4-7 miles out of it if you kept it around 10mph? a little kid could probably haul ass on this thing half the day. 

seems like the ideal board for dicking around in the park or letting your kids ride around with you. and it probably won't take long to charge, either. This has a ton of potential and i might buy one if they go to market.
```

---
## \#17 Posted by: locktight Posted at: 2015-11-24T14:42:36.878Z Reads: 112

```
I wonder how this would effect the weight to power ratio. This allows you to have a relatively small low voltage battery but still get some decent speed with the high kv motors which leads to a small light board, however you would have to add the weight and space(not really that much) for 4 escs and the 4 motor mounts which if you make the mounts light and small this difference would be almost eliminated. I might have to try and take the plunge as well this is an interesting idea that inwould like to try. I think chaka and a few others touched on in the 4wd electric skateboards thread (didn't have any full blown designs like here). If I do build one  I might yolo it and hook up the space cell. EAT MY DUST!!!
```

---
## \#18 Posted by: PennE Posted at: 2015-11-24T15:03:19.746Z Reads: 115

```
I'd be careful hooking up a space cell, the small, relatively high kv motors are usually not intended for more than 4-5s, maybe 6s lipo.
```

---
## \#19 Posted by: PennE Posted at: 2015-11-24T15:09:46.955Z Reads: 123

```

[quote="onloop, post:15, topic:566, full:true"]
Also, if you use really small motors, that also means the wheel diameter can be much smaller so the total weight goes down as a result, big wheels are heavy, also you get more torque too.
[/quote]

yep, current design is for 60mm wheels.

[quote="longhairedboy, post:16, topic:566"]
and it probably won't take long to charge, either.
[/quote]
depends on the final charging setup. If I try to have a charger built into the board it would have to be a small, probably <1A charger, so charge times would not be great, but that would allow a really simple system of just plugging in a dc power supply.
if I use a proper external li-po charger, it could be charged in under two hours without wearing down the battery.

[quote="siggs3000, post:14, topic:566"]
This could be a really cool build. If this sort of mini board is feasible for (what seems to be) a really reasonable price compared to the longboards all of us are using, everyone would want to have one to keep in their trunk, dorm room, office, etc.
[/quote]
cost of the one-off (not including labor of course) looks like it'll come in under $350, so if that works out and we can set up an effective way of producing them in decent quantities, and therefore buying components in bulk (currently hoping if the prototype works well to take it to kickstarter sometime in 2016) we could probably have commercial versions going for between $300 and $450 while still turning around enough profit to make it commercially viable.
```

---
## \#20 Posted by: evoheyax Posted at: 2015-12-07T17:18:57.756Z Reads: 121

```
I share your desire for a small and light board. I am currently using a ~30 inch board with a single motor and dual batteries.

The one question I didn't see by skimming through the posts was what kind of range and top speed you expect?

The idea of fitting as much as I can into the least space possible has lead to towards the VESC and Hub motors.

I am studying computer science, not design or engineering, and thus, I have little CAD. And that is my limiting factor, but I see the concept of build a board, slightly thinker, with the components inside of the board rather than in a compartment under it. Then, 3d printing such board.
```

---
## \#21 Posted by: Okami Posted at: 2017-01-22T15:45:44.995Z Reads: 60

```
Any news on this one? How has it progressed?
```

---
## \#22 Posted by: faithfulpuppy Posted at: 2017-01-22T18:38:53.267Z Reads: 59

```
i'm interested in how this turned out. You there @PennE?
```

---
## \#23 Posted by: Trans-amers Posted at: 2017-01-22T19:11:22.620Z Reads: 58

```
If I had the tools to make a board, I'd go for the design like bolt motion, which has a super cool look imo.
```

---
## \#24 Posted by: PennE Posted at: 2017-01-24T18:51:48.969Z Reads: 46

```
Quick update since I've ignored this thread a long time:
project is currently sidelined due to discovering some inherent issues with the high kv motors, namely their lack of torque. They can maintain solid speeds (23-25mph) but acceleration is practically non-existent due to lack of torque, and maximum hill grade was 4-5% before the motors were just stalling out. wouldn't recommend this setup.
```

---
## \#25 Posted by: Okami Posted at: 2017-01-24T22:16:46.862Z Reads: 40

```
mh so 400kv is way too up in the sky.. 300kv is what is the highest here, I think..

270-300kv.
```

---
