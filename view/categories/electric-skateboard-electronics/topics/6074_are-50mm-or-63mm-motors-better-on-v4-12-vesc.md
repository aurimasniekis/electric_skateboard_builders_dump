# Are 50mm OR 63mm Motors Better on V4.12 VESC?

### Replies: 94 Views: 8873

## \#2 Posted by: chaka Posted at: 2016-07-13T13:24:57.418Z Reads: 505

```


When the VESC is is set up with a balanced system it is extremely reliable. Of course like any other ESC if you pair it with a huge motor that has a higher current rating than the VESC will handle you will be in dangerous territory and have a temperamental failure prone system. 

Honestly the VESC's biggest weakness is poor business practices and cheap manufacturing.
```

---
## \#3 Posted by: onloop Posted at: 2016-07-13T16:07:06.419Z Reads: 507

```


@chaka is right, running a well balanced system is necessary for stability.

10S. 190kv-200kv. Is the ideal esk8 setup for keeping vesc cool & happy.

Also need to be carefully not to have your reduction ratio's too low. Most people work that out eventually. That will over work the entire drive train and stress the vesc. Especially on the small motors that naturally draw more current as they are much easier to overload.
```

---
## \#4 Posted by: chaka Posted at: 2016-07-13T16:25:13.327Z Reads: 504

```
> Especially on the small motors that naturally draw more current as they are much easier to overload.

This is actually false. If you take two single drives with the same settings and try to climb a steep hill the smaller of the two motors will make it to the top while the larger motor will overheat the VESC.
```

---
## \#5 Posted by: onloop Posted at: 2016-07-14T00:28:10.015Z Reads: 471

```
[quote="chaka, post:52, topic:5629"]
This is actually false. If you take two single drives with the same settings and try to climb a steep hill the smaller of the two motors will make it to the top while the larger motor will overheat the VESC.
[/quote]

Big statement mate, maybe back it up with some evidence. Are you still running 2:1 ratios & riding at 50mph? Those systems will never work well hill climbing.

From my own practical experience smaller (50mm) hobby grade motors heat up much more under load and have less torque per watt. 

Larger hobby grade motors heat up less & deliver more torque for the same wattage. Because larger stator diameters offer a mechanical advantage over the smaller stators. Yes they can handle more current if needed but will heat up less.

For a stable system you need all the elements to be in harmony. You have a track record for pushing the speed limits of eboards beyond a safe & practical level and hence your data is likely skewed based on your inefficient drivetrain designs. I have said it before & ill say it again, speeds over 45Km/h are not practical or safe & definitely stress your electronics.

You are one of the more experienced guys on here & yet you still have not to contributed video test results/data onto the forums so the community can educate themselves further. Maybe now is a good time to prove your claims. You are the resident VESC expert right? why not publish your VESC settings &/or write some tutorials for the community?



_NOTE: It is also worth noting that not all motors are equal. Some big motors are just not that good & Some small motors are good, take a look at boosted boards for instance, small powerful motors that don't get very hot.. The next generation of custom made motors we are designing will set a new standard of what is possible with esk8._
```

---
## \#6 Posted by: chaka Posted at: 2016-07-14T01:51:56.258Z Reads: 446

```
> Big statement mate

Not really, this is common knowledge among rc airplane enthusiasts or anyone who has done a little research into ESC and motor combinations.
```

---
## \#7 Posted by: onloop Posted at: 2016-07-14T03:22:28.304Z Reads: 441

```
[quote="chaka, post:61, topic:5629"]
Not really, this is common knowledge among rc airplane enthusiasts or anyone who has done a little research into ESC and motor combinations.
[/quote]

But we are not building/riding on toy planes, RC plane motors are required to do a completely different task, they are also 1:1 direct drive & most esk8 motors we use are geared, with reduction of 2.5 or more.

RC planes run on a much lower voltage at higher rpm with higher KV motors, not to mention the prop size variable, wing span & wing span area variables, power to weight ratios etc... smaller motors are obviously better when trying to minimise flight weight & maximise thrust whilst keeping constant current draw within the specs of the battery.

The constant current & sustained loads endured by an RC plane during flight would seem to be very different from Esk8 load profiles.

**Can you please educate us how RC plane setups compare with ESK8 Drivetrains? I am more than willing to learn.**

I would say that RC planes are more similar to a hub motor on an ESK8 - However, It is still arguable that the load profile & current draw from a prop & motor during flight is vastly different than what an esk8 motor has to deal with during normal riding conditions. ESK8 don't have a minimum stalling speed and are not always running at minimum constant current draw as required for flight & total weight is not a critical factor.

All i ask is that you provide some evidence.. If smaller motors are magically better for esk8 it should be easy to prove. a watt meter, thermometer, video camera & a hill is all you need.
```

---
## \#1 Posted by: onloop Posted at: 2016-07-14T04:35:27.064Z Reads: 462

```
**FACT or FICTION: Smaller motors are better than bigger motors when using a VESC**

Smaller meaning 50mm Diameter Brushless Outrunners
Bigger meaning 63mm Diameter Brushless Outrunners
Better meaning Less heat? More Reliable?
```

---
## \#8 Posted by: psychotiller Posted at: 2016-07-14T04:40:37.157Z Reads: 409

```
I think smaller motors are going to win on efficiency In a dual format. 
In my head it makes sense.

Fact?
```

---
## \#9 Posted by: Jinra Posted at: 2016-07-14T06:35:59.306Z Reads: 401

```
Is it a coincidence that Evolve uses 50mm motors for their GT? I'd bet it was due to their R&D team finding out that 50mm's work better for what they're trying to achieve. Would love to hear the science behind it all.
```

---
## \#10 Posted by: Maxid Posted at: 2016-07-14T06:38:04.400Z Reads: 398

```
my guess is they are cheaper and still work - so why should they go for bigger motors?
Probably a purely economic decision.
```

---
## \#11 Posted by: Jinra Posted at: 2016-07-14T06:42:58.654Z Reads: 390

```
You don't get to be a big a company in this market with that kind of mentality. The people who go "eh it's cheaper and works" don't usually last long in the business. Given that everything else about their GT was well engineered, I'm sure they made a thought out decision about the motors as well.
```

---
## \#12 Posted by: onloop Posted at: 2016-07-14T06:52:10.399Z Reads: 379

```
[quote="Maxid, post:10, topic:6074"]
my guess is they are cheaper and still work
[/quote]

I think 50mm is fine, especially if you are a lightweight rider and rarely go up hills, you just need to make sure you have appropriate current limits set (e.g. MAX 50A Battery Current or Less per VESC) & a make sure your gearing ratios are appropriate.

However for the money, I would prefer a larger stator, larger copper mass, can handle higher current when needed & can dissipate heat quicker. Larger diameter stators have a mechanical advantage over the smaller ones.
```

---
## \#13 Posted by: Maxid Posted at: 2016-07-14T06:53:05.804Z Reads: 374

```
[quote="Jinra, post:11, topic:6074, full:true"]
You don't get to be a big a company in this market with that kind of mentality. The people who go "eh it's cheaper and works" don't usually last long in the business. 
[/quote]

Care to explain why that should be? The other way around would also not be a wise business decision: using something more expensive that works equally well.
What I am trying to say is: both motors perform probably equally well for our use cases so there is no point to use the bigger and heavier one (especially when you have a dual setup that splits the load). I don't think they did scientific studies to find out which one is actually better and will never do such a thing as long as both options work.
```

---
## \#14 Posted by: Photorph Posted at: 2016-07-14T06:55:50.354Z Reads: 362

```
Can't really comment on which works better with a VESC.  But it's fun watching chaka and onloop argue.
```

---
## \#15 Posted by: Jinra Posted at: 2016-07-14T06:56:55.940Z Reads: 362

```
I hear you, and if it were the case that product A works just as well as product B but was cheaper, I'd totally agree that they would use product A. However, my guess is that 50mm do work better than other motor sizes due to the R&D put into making their GT series boards. And not just because they're cheaper. However, I have no basis or proof for my hypothesis, and will be keeping my eye on this thread for the scientific reasoning to follow :)
```

---
## \#16 Posted by: onloop Posted at: 2016-07-14T07:05:42.120Z Reads: 373

```
[quote="Photorph, post:14, topic:6074"]
watching chaka and onloop argue.
[/quote]

Yes, I suppose it might be entertaining, but my purpose is not to create an argument, it's merely a request for evidence to support claims.

If it is proven that 50mm are better for some reason we can all make better cheaper eboards. 50mm are much cheaper to manufacture than 63mm
```

---
## \#17 Posted by: chaka Posted at: 2016-07-14T07:10:08.513Z Reads: 360

```
A single 63mm motor is great with a high end hobby ESC but the VESC  V4.XX  cannot provide enough throughput to thoroughly enjoy the output of these larger motors.

 If you pair a single 6365mm motor with a VESC on 16/36 tooth on 90mm abecs and try to climb a long somewhat steep hill at full throttle the VESC will overheat fairly quickly and you will come to a stop.  If you do the same with a 5065 motor you will be able to climb at a continuous rate without the VESC overheating.  With gearing this tall on a single drive we are only talking about 5 to 10% grade to get these results.

This is all fairly basic stuff. It is common knowledge that your esc should be capable of handling more current than the motor will pull at max throttle if you want your hardware to last.
```

---
## \#18 Posted by: Maxid Posted at: 2016-07-14T07:11:42.646Z Reads: 346

```
I understand what you mean.
However it would surprise me if they actually did some R&D on the motor. My guess is they just buy the stuff in bulk from a Chinese manufacturer and basically have no say in the process besides color or so. I mean why should they spend huge amounts of their resources on something that apparently already works pretty well (SK3s for example have already proven to be up to the task) when there is so much space for improvements that will actually get them customers (just think of their fancy remote with display or apparently super efficient ESC that increases the range they can get out of a 10S3P battery). But I guess we will never know what actually happens behind the scenes, so I could definitely be wrong with this.

PS: That was actually a kind of pleasant argument we had there. Glad something like this can still happen on the internet.
```

---
## \#19 Posted by: furryfrog Posted at: 2016-07-14T07:13:56.391Z Reads: 333

```
I don't think the RC plane loads are not comparible to an esk8, unless they use varible pitch props so the load can vary at similar rpm's, I am not sure if they use variable pitch props.

Just getting into e sk8's, and brushless motors. Lots of variables to consider. Say both the small and bigger motor have similar specs, (other than the larger motor will have more starting torque and power output) I would say bigger is better if given the same load and the same rpm. Though a smaller motor could have an advantage at certain loads in certain circumstances if geared differently.
```

---
## \#20 Posted by: Maxid Posted at: 2016-07-14T07:17:57.358Z Reads: 336

```
[quote="chaka, post:17, topic:6074, full:true"]
 If you pair a single 6365mm motor with a VESC on 16/36 tooth on 90mm abecs and try to climb a long somewhat steep hill at full throttle the VESC will overheat fairly quickly and you will come to a stop.  If you do the same with a 5065 motor you will be able to climb at a continuous rate without the VESC overheating.  
[/quote]

In your example it will however matter what that rate actually is you are talking about. Full throttle on a 6365 probably means something different than on a 5065. So if I can get the same climbing rate on a 6365 by lowering the throttle will the VESC stay cool? Full throttle is a weird comparison as it does not tell us anything about the relative speeds. To be a fair argument both motors should result in the same absolute climbing rate.
```

---
## \#21 Posted by: chaka Posted at: 2016-07-14T07:19:38.944Z Reads: 327

```
Same rate, but the 5065 climbs faster because the VESC does not overheat.

In this comparison both motors were 170KV at 12s
```

---
## \#22 Posted by: chaka Posted at: 2016-07-14T07:22:12.194Z Reads: 325

```
In a dual configuration you will likely not pull enough power to find this weak link but the 50mm motors are definitely more efficient.
```

---
## \#23 Posted by: furryfrog Posted at: 2016-07-14T07:22:39.627Z Reads: 328

```
As far as the vesc, I see what you guys are saying, a bigger motor will be able to draw more current. Are we comparing two small motors to one big motor? Here is a graph I dug up on the interweb from this article

http://www.edn.com/design/sensors/4406682/2/Brushless-DC-Motors---Part-I--Construction-and-Operating-Principles

Im assuming this to be general to all brushless motos, can we dig up graphs on real world motors that you guys have used? With efficiency and current data as well?

<img src="/uploads/db1493/original/2X/7/70783bd7d0762d17d2421b34c2364bf41dca2938.jpg" width="550" height="347">
```

---
## \#24 Posted by: onloop Posted at: 2016-07-14T07:25:47.000Z Reads: 313

```
[quote="chaka, post:21, topic:6074"]
but the 5065 climbs faster because the VESC does not overheat.
[/quote]

If the current is limited in the VESC firmware why would it get hotter on the larger motor? for the same load & same current surely the larger motor handles the load better?
```

---
## \#25 Posted by: chaka Posted at: 2016-07-14T07:31:27.993Z Reads: 317

```
If you load up a motor on a steep hill it will still overheat the vesc regardless of the current limit. It is definitely harder to induce on a dual drive but possible. You still need to follow some of the guidelines set by the RC crowd. Just because you have a vesc doesn't mean you can be ham handed with your setup if you want an efficient system
```

---
## \#26 Posted by: furryfrog Posted at: 2016-07-14T07:47:44.466Z Reads: 313

```
What's the reason there are no heat sinks on the vescs?, new to esk8's, weight reduction? space? I would assume those mosfet's can get pretty hot?
```

---
## \#27 Posted by: kampfhahn Posted at: 2016-07-14T07:52:24.022Z Reads: 315

```
@chaka: Your words made me a bit doubtful if my planned setup is good for me.

I ordered a 190kv 6355, VESC, 16/36, 10S

[I used a calculator](http://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii) which even involves riders weight and the result was that climbing a 15 percent hill with about 20 kph only takes about 780 watts / 22 amps. So why should the VESC overheat then? My weight is only 65 kilos + board.
```

---
## \#28 Posted by: furryfrog Posted at: 2016-07-14T08:07:49.181Z Reads: 313

```
What is the max no-load speed of the motor your using? Think about gearing it so half your no-load speed is the speed at which you want to go up the hill at, then you will be on the power peak of your motor as well. If in fact that article is correct and that theory can generally be applied to all brushless motors.
```

---
## \#29 Posted by: onloop Posted at: 2016-07-14T08:19:13.456Z Reads: 310

```
[quote="chaka, post:17, topic:6074"]
If you pair a single 6365mm motor with a VESC on 16/36 tooth on 90mm abecs and try to climb a long somewhat steep hill at full throttle the VESC will overheat fairly quickly
[/quote]

I'm not sure what voltage you are running but this 2.25:1 reduction ratio is a bit outside my safety zone, big tax on torque. At 10S you are trying to push the top speed up to 32mph. Wind Resistance will start loading up at this speed (at least on the flats) 

I know you have a need for speed but have you considered running some more reduction to reduce the load on the single motor? maybe 15/36 & 83mm would be a better option? 28mph is still fast and you will have a more reliable system. Less heat.

I wonder if you will draw the same conclusion about motor size with a higher torque gearing ratio?
```

---
## \#30 Posted by: shred Posted at: 2016-07-14T09:46:08.549Z Reads: 297

```
is this really about the physical size of the motor or is it meant to be about the max power output a motor can do? 

@chaka why does it make a difference for the VESC/ESC: if I have a 1800W Motor with VESC setup to support 1800W or if I have a 3000W motor with VESC setup to support only 1800W? Should be the same for the ESC I would guess, as well would guess that the small motor will run hotter, might be that the small motor spins faster though???
```

---
## \#32 Posted by: shred Posted at: 2016-07-14T09:52:47.844Z Reads: 290

```
understood, but if I set the limit to 50A I would have guessed max current draw is limited
```

---
## \#33 Posted by: kampfhahn Posted at: 2016-07-14T09:56:04.337Z Reads: 286

```
Sorry i already realized that my post was bullshit especially because @chaka wrote that while climbing you even can overheat the VESC without reaching the 50a limit. Why that?
```

---
## \#34 Posted by: Jinra Posted at: 2016-07-14T14:08:22.794Z Reads: 286

```
FWIW the Evolve GT has a 2.13:1 reduction and I'm using 97mm wheels on 50mm motors. I ride a lot of hills and it doesn't seem to overheat. Though in this case there are two motors.
```

---
## \#35 Posted by: chaka Posted at: 2016-07-14T14:28:12.796Z Reads: 287

```
>  @chaka wrote that while climbing you even can overheat the VESC without reaching the 50a limit. Why that?

I am not entirely sure why but it seems like the VESC will still allow the motor to pull large amounts of current when loaded heavily. The motor current settings in the VESC should be viewed more as adjusting the throttle and discharge curves rather than absolute limits.

> is this really about the physical size of the motor or is it meant to be about the max power output a motor can do?

> @chaka why does it make a difference for the VESC/ESC: if I have a 1800W Motor with VESC setup to support 1800W or if I have a 3000W motor with VESC setup to support only 1800W? Should be the same for the ESC I would guess, as well would guess that the small motor will run hotter, might be that the small motor spins faster though???

What matters is what the motor pulls when it approaches "stall torque" and that your ESC is able to handle this much power. We also need to be sure our battery systems can handle this much output without heating up if we want our cells to last a long charge/discharge cycle life. The VESC is very good at limiting the current a motor can pull but it is not magic, a motor will still pull huge amounts of current when it approaches a stall scenario. How much it pulls depends on the specs and ratings of the motor.

If you plan on using a big motor with the VESC on a single drive you will want to avoid these stall torque scenarios due to having a top heavy system.  If you want to design a system with a long life and smooth operation you need to make sure you battery and motor controller can  handle the max rating of your motor/s. Sticking two 3000 watt motors on a 10s3p pack with motor controllers rated at 1800 watts continuous is just window dressing.

It has been established for a very long time that you should always have a pack and motor controller that exceed the rating of your motors. 

Well balanced cool running system = Battery>ESC>motor
```

---
## \#36 Posted by: Eboostin Posted at: 2016-07-14T15:40:07.338Z Reads: 264

```
Would two of your 50mm motors paired with a Spacecell 10SP4 be a good combination?
```

---
## \#37 Posted by: chaka Posted at: 2016-07-14T16:04:40.527Z Reads: 263

```
When the pack is new it will work fine but as the pack ages it will build resistance and heat under heavy use. In my experience you want to be able to pull 600 to 800 watts at maximum of 1C to have a long lasting pack. This may seem crazy to some people but we have proven that it is possible to fit a pack this large on a board. This is assuming we are building boards as an investment.

If you are building something just to have fun and do not mind wearing things out a little sooner than expected by all means use smaller high discharge packs. If you want something that will not show signs of wear after only 200 discharge cycles you need to go bigger. The trouble with large packs is space and weight, a 23lb board is not the easiest thing to market either.
```

---
## \#38 Posted by: torqueboards Posted at: 2016-07-14T20:17:53.041Z Reads: 271

```
If anyone stalls in the middle of a steep hill and continues to try and go up the hill from a standstill (especially a steep hill). You crazy :slight_smile: Just don't loose your momentum next time going up the hill.

Nobody, should ever do that and you'll have a higher possibility to burn out your components. Your better off walking the hill for 2-3 minutes then riding once your on top of the hill or buy another motor since you fried it. 2-3 minutes saves your wallet.

That's partly why most of these china boards break. People just abuse these cheap boards but flat ground they are most of the time perfectly fine.

It's not typical anyone is ever going to burn anything out on flat ground. Uphill causes a tremendous amount of heat.

If your climbing uphill, you should expect to be going up the hill w/ momentum on a single motor and/or go dual motor.

IMO the only benefit for the 6355's is they are harder to burn out compared to a single 50mm.

Give anyone a 50mm and more chances or not if they aren't on flat ground. They'll burn it out if they don't use it correctly.

If the board doesn't go anywhere most people will just "throttle, throttle, throttle".

Different parts for different goals...
```

---
## \#39 Posted by: Jinra Posted at: 2016-07-14T20:31:05.949Z Reads: 261

```
Not even just hills. Wind resistance is also a pretty big factor. My GT's motors are just a bit warm when traveling 4 miles in my morning commute up and down hills. However, on the way back home there's a bunch of headwind and by the time I get home, one of my motors is burning hot (the other a bit warm). I always feel bad for my motors when I'm going up a hill at less than desirable speeds because I know it's chugging pretty hard; especially on 2.13:1 gearing.
```

---
## \#40 Posted by: Namasaki Posted at: 2016-07-14T22:32:32.283Z Reads: 257

```
[quote="Jinra, post:39, topic:6074"]
Not even just hills. Wind resistance is also a pretty big factor.
[/quote]
I also have experienced overheating when riding on flat ground into a strong headwind. That was with dual hub motors.
```

---
## \#41 Posted by: onloop Posted at: 2016-07-14T23:51:33.671Z Reads: 269

```
[quote="chaka, post:35, topic:6074"]
How much it pulls depends on the specs and ratings of the motor.
[/quote]

Specifically it depends on the reduction ratio.... the bigger the reduction the less chance of your motor drawing high amps and stalling on hills (depends on rider weight and incline). 

I know i sound like a broken record... but @chaka why don't you try more reduction?...  one single 63mm motor, 2.4 or more reduction with 83mm wheels. Vesc current limit of 50A.

I'll send you an enertion kit so you can try it?
```

---
## \#42 Posted by: JohnnyMeduse Posted at: 2016-07-15T00:11:43.726Z Reads: 262

```
From my personal experience, the first motor that I use was a 5065 from Torqueboard, and was overheating like hell (also totally burn it while climbing a hill), I change it, in the same setup for a 6355 again from Torqueboard  and never any problem after that.
```

---
## \#43 Posted by: chaka Posted at: 2016-07-15T01:23:37.254Z Reads: 263

```
True you can hide a systems short comings with reduced gear ratios and low speeds but it doesn't change the fact that you will have an unbalanced system if using a VESC 4.xx 

It has been well established that a single motor build is better with a 63mm motor but you really should be using a hobby rc type ESC that is rated for at least 150 amps unless you plan on going dual VESC. However I have overheated 6555 motors on a single drive board so it really depends on several factors. 

There are a lot of different ways you can configure a system but everyone should know the VESC isn't designed with enough throughput to power a 3000 watt motor to it's full potential without overheating. Sometime I wonder if you even ride since you were so unaware that the VESC can overheat when limiting the motor current below 50 amps on large 63mm motors. Maybe you just don't push it hard enough?

I think I have explained the reasoning to leave some headroom in your ESC in regards to the motor. Plenty of info on this topic in several other forums, just a google search away.
```

---
## \#44 Posted by: Jinra Posted at: 2016-07-15T01:25:22.463Z Reads: 259

```
I imagine Aus is pretty flat
```

---
## \#45 Posted by: stuxtruth Posted at: 2016-07-15T01:36:50.069Z Reads: 258

```
In America bigger is better. 63mm.
```

---
## \#46 Posted by: t1m0007 Posted at: 2016-07-15T02:03:31.569Z Reads: 259

```
this thread is a completely unhelpful mindfuck for the new guys. thanks fellas
```

---
## \#47 Posted by: cmatson Posted at: 2016-07-15T02:05:28.460Z Reads: 265

```
[quote="chaka, post:43, topic:6074"]
It has been well established that a single motor build is better with a 63mm motor but you really should be using a hobby rc type ESC that is rated for at least 150 amps unless you plan on going dual VESC.
[/quote]

I've **only** run my VESC's on single 6355 motors, and haven't over-heated one. The only VESC problem was a solder joint that vibrated loose...

one is an Rspec on 16/36 gearing 83mm wheels limited to 40 amps with a space cell. 

the other is a torqueboards 230kv 15/36 gearing on 100mm wheels limited to 65 amps on 6s

both go about the same speed, and both are around the same temp after long rides; warm to the touch, easy to hold your hand on the motor and not get burnt. I will say it is mostly all flat ground, but there is wind resistance by the river as others have mentioned, and little hills throughout my usual treck. 

Now, I'm only 140ish pounds, but my dad is now pushing 210, and he'll ride the Rspec board for a couple miles now and then with zero problems.
```

---
## \#48 Posted by: onloop Posted at: 2016-07-15T02:27:37.440Z Reads: 270

```
[quote="chaka, post:43, topic:6074"]
There are a lot of different ways you can configure a system but everyone should know the VESC isn't designed with enough throughput to power a 3000 watt motor to it's full potential without overheating.
[/quote]

but why do you insist on wanting to run 3kw into your esk8? I get it that you want to ride at super fast speeds but you already know that it causes problems with VESC.

[quote="chaka, post:6, topic:636"]
At 30 mph we use almost three times as much wattage as when we travel at 20mph.
[/quote]



You are one of the only people on here who continues to push the VESC past its engineered limits.... that's why you installed heatsinks, right? 

http://www.electric-skateboard.builders/t/ollinboardcos-high-output-vesc/636/4


**But now you claim the issue is 63mm motors?...** 

Why not just use your ESK8 in a safe operating zone with plenty of head room?

Very few people want to ride single motor esk8 up hills at 32mph... I suggest from now on you start publishing your drive train setup & vesc settings with every statement you make, like it or not you are an influencer on this forum, you need to make sure your statements don't confuse the masses.

Personally, I have no intention of riding at the speeds you like to ride at, in urban areas it's just unsafe, it's also well documented that speeds above 45km/h  require a huge increase in power to get small gains. It's inefficient & thats why you have been forced to use such large batteries.

http://www.electric-skateboard.builders/uploads/db1493/original/2X/4/4437677ed1c4f6757388c04806da568136012437.jpg
http://www.electric-skateboard.builders/uploads/db1493/original/2X/0/0586b19bf91f288231ce2c2937f9c80e2920a425.jpg
```

---
## \#49 Posted by: chaka Posted at: 2016-07-15T03:01:55.831Z Reads: 249

```
Here is a nice little instructional blog that may help you understand how to properly balance a system. http://www.modelairplanenews.com/blog/2011/05/29/choosing-a-motor-speed-control-battery-pack-taking-the-mystery-out/

Currently most of us are using the V4.xx of the vesc which has a max constant current of 50amps (1800 watts at 10s) so we need to expand the system requirements from there and work outward to find our motor and battery specs. Once V6.xx becomes available we will be able to use just about any motor we want and just make sure our packs can handle the load. You could of course use a high end car esc now if you wanted.

I completely understand that some lighter riders can zip up hills with ease on just about any setup. At 185-200 lbs I have to say I am jealous. Just accelerating too hard or too frequently will heat up your battery and esc if they are trying to power a motor that can draw more than the system can handle when you are close to 200lbs regardless of gear ratio. Some of us are savages!

It is better to pair the system with a motor close to the same spec and allow the system to self govern. If you have a balanced system and your motor is getting warmer than you want, adjust the gear ratio to reduce the load or go with a dual drive. This goes for 50mm and 65mm motors. You end up with a much more balanced and efficient system.
```

---
## \#50 Posted by: t1m0007 Posted at: 2016-07-15T03:10:41.409Z Reads: 249

```
Gents, I'm going to insert myself here and try to reel this thing in a little and bring it back to the more common ground for people around here that have a more average situation. Self serving? Sure. But I'm going to do it anyway. And, likely it'll be good for the community at large. Both of you gentlemen, @onloop and @chaka are respected figures around these parts and both of you guys have a some great products. Even in this thread you've both conceded some points to the other. I think this 50mm vs 63mm motor discussion is a good one. And i really think to nail this thing down, maybe we should frame it in the context of a single drive motor and eliminate some variables. Shall we?

Let assume a fairly middle of the road setup with middle of the road aspirations. Our guy, let's call him J1m0007, wants a top speed of around 20mph and has hills maxing out at 20% grade in his general area. He's going to build a board in order to work towards those aspirations.

He doesn't want to go face-melting fast.
He doesn't want to climb Mt. Everest.
He doesn't want to spend the next 6 months tinkering with different drive train components.

He's going to buy an average board with average wheels, gearing and power:
83mm Wheels 
36/14T drive for a 2.57 : 1 drive ratio. EDIT! I meant 14t Not 16
10s -- because @onloop and @torqueboards and others make great plug and ride solutions and Li-Ion is dope.

Let's assume J1m is the weight of the average male in the UK for the sake of argument 180lbs (~81Kg).

If you run the numbers here: http://toddy616.blogspot.be/2013/07/electric-skateboard-calculator.html J1m ends up with just the right amount of speed he desires.

J1m could pick @onloop's 190kv 63mm Motor (6372)
http://www.enertionboards.com/electric-skateboard-parts/6374-190kv-electric-skateboard-motor/

or @chaka's 50mm 200kv Motor (5065)
http://www.ollinboardcompany.com/product/om5065-200kv

Both of which recommend the gearing described above for a single motor setup on their product pages.

So, if J1m wanted to meet his criteria in a board AND protect the longevity of his components (VESC, Battery and Motor alike)  heat exposure and related corrosion, which would J1m want to pick and, as @onloop is keen on stressing the importance of, **WHY?**
```

---
## \#51 Posted by: mason Posted at: 2016-07-15T03:11:16.076Z Reads: 232

```
https://media.giphy.com/media/uqPDIEPMODKne/giphy.gif
```

---
## \#52 Posted by: cmatson Posted at: 2016-07-15T03:11:28.718Z Reads: 235

```
[quote="chaka, post:49, topic:6074"]
Here is a nice little instructional blog that may help you understand how to properly balance a system. http://www.modelairplanenews.com/blog/2011/05/29/choosing-a-motor-speed-control-battery-pack-taking-the-mystery-out/
[/quote]

I personally think that planes are going to handle power draw quite differently to skateboards, and wouldn't be throwing that article out here.. maybe an RC car one, but not planes. 

[quote="chaka, post:49, topic:6074"]
Just accelerating too hard or too frequently will heat up your battery and esc if they are trying to power a motor that can draw more than the system can handle when you are close to 200lbs regardless of gear ratio. Some of us are savages!
[/quote]

my dad is over that range, and has a skateboarding/roller blading past- he knows how to ride fast, and does. Not once has he over heated the battery or VESC in the settings above. 

I just don't think as @onloop mentioned that many people want to go 30+ mph uphill.


----------

**My main point:** it seems like before you started selling 50mm motors you never made a fuss about 63's, and the general consensus on the forum was that people should buy the biggest motor they can afford. Now you start selling 50mm motors, and need some way to get people to buy them... how to do that? scare them into believing their VESC will fail with larger motors!!!
```

---
## \#53 Posted by: onloop Posted at: 2016-07-15T03:22:13.435Z Reads: 225

```
Great question, 

Firstly, there is no need to use 16T motor pulleys. It doesn't put more teeth in mesh & it reduces your reduction ratio. I can't think of any reason to use it, unless your centre distance is 53mm or less (which is likely impossible)

You should always try to maximise reduction ratio. 15T - 36T is the perfect setup with 5mm pitch belts at approx 66mm distance. Any smaller than 15T motor pulley and you should try to use an idler to get more teeth in mesh.

**Every 50mm motor i have ever used has failed, mostly due to overheating.**
```

---
## \#54 Posted by: t1m0007 Posted at: 2016-07-15T03:27:19.487Z Reads: 219

```
hey @onloop my bad I meant to type 14t! Thanks man.
```

---
## \#55 Posted by: Ulfberht Posted at: 2016-07-15T04:22:54.821Z Reads: 221

```
LOL....
<img src="/uploads/db1493/original/2X/1/16bb092293fb8372a99269cdd712ee9d62043482.gif" width="226" height="309">
```

---
## \#56 Posted by: NNGG Posted at: 2016-07-15T04:53:52.613Z Reads: 215

```
I hate the new guy they put in to replace Jon
```

---
## \#57 Posted by: Ulfberht Posted at: 2016-07-15T06:19:05.553Z Reads: 224

```
[quote="chaka, post:35, topic:6074"]
It has been established for a very long time that you should always have a pack and motor controller that exceed the rating of your motors. 

Well balanced cool running system = Battery&gt;ESC&gt;motor
[/quote]
I have no intention of getting into an argument, but I believe the point that Chaka is trying to emphasize is NOT that 63mm motors WILL 100% kill your VESC. I believe he is simply trying to outline the fact that the V4.xx VESC are not optimized for larger motors and lack the "headroom" you need to really get the biggest bang for your buck out of 63s. @50A, the current iteration of the VESC is not designed to provide enough juice to coax the full potential out of those motors. So if there is not enough output from the VESC to power them optimally, it just makes a lot more sense that a smaller motor would be more efficient in that regard. It just seems really obvious to me that if the ESC is underpowered that you would not pair it with a motor that is too current hungry. From the link that Chaka posted from Modelairplanenews.com, "It is always better to have an ESC that is rated slightly higher than the amps you really need...," Makes sense to me. This is aside from gear ratios. Yeah, you can def make it work. That was his point as well. Just be aware of the possibilities that an unbalanced electrical system can bring to the party. 
This knowledge could potentially prevent a serious injury as well. Remember the old saying, "Everything is fine, until the day it's not." :wink:
Chaka has been generous enough to give us the inside information that he has accumulated from his studies and practical experience. You can bet that I check his work and cross reference it with as many sources as possible to verify the truth. Every time I do that with something that he has posted either here or on Endless Sphere, I find it to be true and it usually leads me down a very useful path in my studies. This is an opportunity...Not an argument, fellas. Watch and learn!! Test everything and hold tight to the good stuff! 
:smile: :v: 

So based on the known and easy to reference fact that an ESC should be rated to exceed the spec of the motors....Then it's safe to say that  50mm motors are indeed the "better", more efficient, option for use with VESC 4.xx, based on it's rated output limit. 
I think that is a fair statement. :wink:
Real world application you want? You guys have seen this Ollinboardco vid, right? 
Singledrive>5065>170kv@12s and roughly 200lb dude. (Def not little dudes club!) LOL  ....
Owning hills ...  Def worth 3 minutes of our time! 

https://www.youtube.com/watch?v=_KE2TWDCMdc
```

---
## \#58 Posted by: t1m0007 Posted at: 2016-07-15T13:40:08.768Z Reads: 210

```
That video is great but it'd be better if a laser thermometer was beamed at the motors at the end of that run and displayed in the video
```

---
## \#59 Posted by: onloop Posted at: 2016-07-15T15:20:56.249Z Reads: 216

```
[quote="Ulfberht, post:57, topic:6074"]
the current iteration of the VESC is not designed to provide enough juice to coax the full potential out of those motors.
[/quote]

What I have a problem with is the assumption 63mm sized motors need _so-much-more_ power to be efficient/work well, this is unfounded.

Has anyone actually got data to back this theory up?  So why assume that a 63mm motor needs 3kw to operate efficiently?

As @chaka likes comparing esk8 with RC planes it would be worth using some of RC Plane industries common "rules of thumb" when determining how many watts can be fed into a motor without damaging it.

A common rule I have found [HERE](http://www.rcgroups.com/forums/showthread.php?t=1222366) is the **GRAM-to-WATT** rule, it states 2-3 watts per gram of average outrunner motor is the target for safe long-term use, without risk of overheating.

2 Watts Per Gram is run-all-day constant current & 3 watts per gram is pushing the motor and only suitable for Bursts.

I have noted the weight of some common motors and compared that to the rated 50A continuous power output of the VESC

<img src="/uploads/db1493/original/2X/1/19e23643484ba6fc8f606dbbdd3cd66d9e78be52.png" width="391" height="500">

_*THIS IS NOT TAKING CONSIDERATION OF VARIABLES SUCH AS COOLING, MOTOR EFFICIENCIES & REDUCTION_
```

---
## \#60 Posted by: furryfrog Posted at: 2016-07-15T16:45:16.985Z Reads: 213

```
Really like that vid too. Yes, and the temp of the electronics as well. Info on temps of everything when It shuts down going up a hill would be good as well.
```

---
## \#61 Posted by: CSN Posted at: 2016-07-15T16:47:26.395Z Reads: 214

```
In a perfect world what temp data on the motor and vesc need to be monitored?

Would make some interesting graphs to settle the question.
```

---
## \#62 Posted by: chaka Posted at: 2016-07-15T17:31:56.140Z Reads: 218

```
Thanks for the data. Looks like the 50mm motors I am distributing are up to the task!

One very important point you continue to ignore is the fact that motors "pull" power. Another point you may not even be aware of is the fact that everytime you accelerate there is a burst of current, the amplitude of that burt is directly related to the size of the motor you are using. This burst is even more apparent when you apply braking current which explains the prevalence of abs-overcurrent faults on the 4.xx vesc when using larger motors.

The VESC is a wonderful device but it does have limitations and if you go past these limitations too far you are increasing the chances of a hardware related failure due to limits in processor speed in relation to amperage spikes.

@cmatson I have access to every motor available. I chose a 5065mm motor simply because it was a better fit for the V4.xx VESC.  I am not forcing anyone to buy my motors and I still provide repairs for people who run larger motors on the VESC's I build. I have always been open and truthful with my marketing and do my best to stick with the facts rather than fluffy window dressing.

There will always be times when my findings do not jive well with someones marketing strategy and those people will obviously lash out and try to twist the information into an argument. This will not stop me from continuing to push the limits and find the weaknesses of the VESC throughout it's development and I will always freely share my findings.
```

---
## \#63 Posted by: torqueboards Posted at: 2016-07-15T18:02:41.439Z Reads: 209

```
:joy: tears of joy @chaka

jk.. I'm just being a troll.. gotta admit.. They need a popcorn emoji plus a prayer emoji.
```

---
## \#64 Posted by: Ulfberht Posted at: 2016-07-15T19:58:11.976Z Reads: 210

```
[quote="torqueboards, post:63, topic:6074"]
They need a popcorn emoji plus a prayer emoji.
[/quote]@torqueboards

:popcorn:   :pray:

:wink: There ya' go!!
```

---
## \#65 Posted by: Randyc1 Posted at: 2016-07-15T20:11:02.603Z Reads: 204

```
Will these Vesc Over-Heating problems with 63mm motors be greatly diminished or  gone with the Ver 6 vesc?
```

---
## \#66 Posted by: mason Posted at: 2016-07-15T20:12:54.692Z Reads: 201

```
dang I expected @XvDarkVAngelvX to reply
```

---
## \#67 Posted by: XvDarkVAngelvX Posted at: 2016-07-15T21:54:50.995Z Reads: 198

```
Sorry been 😋 working. I thought they did. But if 😱 they have it. I betcha I find 😍 it. Lol
```

---
## \#68 Posted by: onloop Posted at: 2016-07-16T02:05:49.222Z Reads: 207

```
[quote="chaka, post:62, topic:6074"]
Another point you may not even be aware of is the fact that everytime you accelerate there is a burst of current, the amplitude of that burt is directly related to the size of the motor you are using. This burst is even more apparent when you apply braking current which explains the prevalence of abs-overcurrent faults on the 4.xx vesc when using larger motors.
[/quote]

I am fully aware of how it works, that's why I am having this discussion openly with the community, it's so that everyone can better understand your unique findings..... What you keep omitting from your statements is that these are geared systems. Therefore, current burst during acceleration is directly related to the load on the motor, the load is directly related to the reduction ratio & wheel size you are running... not to mention rider weight

- Motors pull more & more current until the load is reduced.
2. Mechanical reduction amplifies torque & reduces motor load.
3. The greater the reduction the less load on the motor & the lower the current peaks (also less load during regen)


[quote="chaka, post:62, topic:6074"]
There will always be times when my findings do not jive well with someones marketing strategy and those people will obviously lash out and try to twist the information into an argument.
[/quote]

This is not my marketing strategy, nor is it meant to be argumentative, if anything it's a public awareness campaign! 

The best way to shut me up is provide some actual data, otherwise I'm forced to call you out.

I have been designing & testing drive trains, selling motors & building eboards for the public for several years now. You have only _just_ started to sell motors last month & it is obvious that your language has rapidly changed to be pro 50mm. With no data to support it. 

What you might not know, I have also sold many 50mm motors in the past..... The reason I stopped selling 50mm motors is due to customers burning them up. This doesn't happen with 63mm motors installed into effecient drive trains. 

**63mm motors don't break VESC - Inefficient drive train design & Bad settings breaks VESC.**
```

---
## \#69 Posted by: CSN Posted at: 2016-07-16T02:24:23.018Z Reads: 203

```
One does wonder why Evolve and Boosted run 50's. 

Cost and weight reasons but maybe some system efficiency as well.

Would still have to think that a 63 has more torque on the low end and maybe more practical for single motor setups.
```

---
## \#70 Posted by: NNGG Posted at: 2016-07-16T02:47:12.821Z Reads: 204

```
I think youre correct. My sheer intuition says that ollinco motors are better as a dual than enertions dual 6355. BUt a Enertion 6374 is much better as a single drive than an ollinco single.

The cheaper dual drive is more efficient and costs less, while being in balance with vesc limitations.
The enertion setup could be just extra materials that are unnecessary. just what I gathered from reading this
```

---
## \#71 Posted by: onloop Posted at: 2016-07-16T02:48:01.237Z Reads: 205

```
[quote="CSN, post:69, topic:6074"]
One does wonder why Evolve and Boosted run 50's.
[/quote]

Boosted have a fairly slow top speed & use fairly high reduction 3.5:1 with small wheels. So they can get away with smaller motors, their system would not work well at higher speeds. They would need bigger motors & More current.

Evolve I can't be sure exactly why they have done it, it could just be to reduce weight. It's also worth noting their default top speed is not very fast. I think people installing the larger wheels & trying to ride as fast as possible will eventually have problems. If not directly with the ESC maybe we will see issues with reduced battery life expectancy. At this stage i don't think anyone knows what the max current that their controller can handle. Maybe they are running higher current than the 50A of VESC

One thing that many of you may not be considering is cost. I could make 3 cheaper 50mm motors for the price of one R-SPEC 6355
```

---
## \#72 Posted by: JohnnyMeduse Posted at: 2016-07-16T02:50:46.746Z Reads: 196

```
I don't think Boosted and Evolve are using VESC, they have their custom ESC, so their motor size are irrelevant, in regard of this Topic.
```

---
## \#73 Posted by: onloop Posted at: 2016-07-16T02:56:32.684Z Reads: 195

```

that's a good point, boosted had the privilege to engineer a controller, motors & drivetrain all together at the same time, so comparing their setup to VESC is not saying much.
```

---
## \#74 Posted by: onloop Posted at: 2016-07-16T02:59:34.883Z Reads: 201

```
[quote="NNGG, post:70, topic:6074"]
My sheer intuition says that ollinco motors are better as a dual
[/quote]

except they don't easily fit on most trucks side-by-side in a rear dual configuration, that is another reason i stopped using 50mm as they tend to be longer.
```

---
## \#75 Posted by: NNGG Posted at: 2016-07-16T03:01:11.995Z Reads: 200

```
Oh, I guess that your moto: over engineer everything. is the best way to go. Especially on shorter trucks
```

---
## \#76 Posted by: t1m0007 Posted at: 2016-07-16T03:10:07.625Z Reads: 208

```
Well, since my comment was more or less ignored I'm going to try again. Is anyone on here in the SoCal area that has access to both a @onloop 63mm RSpec Monodrive and a @chaka 50mm OM5065 Monodrive board?

Both need to be 10s and running a VESC (I don't care whose). Id prefer 80mm or 83mm wheels. And a rider that's average size.

I work in TV. I've got the camera gear. I've got eyes. I've got a sense of touch. I've got a Infrared thermometer. 

lets settle this shit ourselves.

Who's with me?  :muscle:
```

---
## \#77 Posted by: torqueboards Posted at: 2016-07-16T03:10:39.262Z Reads: 204

```
@CSN - 50mm motors are a lot cheaper than 63mm motors. But also because they have ESCs like the VESC which limit amps to the motors.

Because Dual 50mm is great and 63mm isn't necessarily needed for dual motors.

Single 50mm lacks a bit but is doable.

I'd take Dual 50's over Dual 63mm because of weight. I've only ever found them to be an issue for really steep hills. The only downside is they don't have a 5055 which why I made my recent 5055's. It weighs a lot less. The stator was upgraded to a stator of a 5065 motor (40.6mm x 30mm).
```

---
## \#78 Posted by: onloop Posted at: 2016-07-16T03:19:07.403Z Reads: 204

```
[quote="torqueboards, post:77, topic:6074"]
Because Dual 50mm is great
[/quote]

Put a 110kg guy on that and send him up a steep hill...... the word _GREAT_ is not what i would use. More like _HOT_
```

---
## \#79 Posted by: torqueboards Posted at: 2016-07-16T03:22:35.478Z Reads: 205

```
[quote="onloop, post:78, topic:6074"]
Because Dual 50mm is great

Put a 110kg guy on that and send him up a steep hill...... the word GREAT is not what i would use. More like HOT
[/quote]

It would take more than one hill to get it hot. Granted, I do agree if you want to climb 10-20 steep hills back to back the bigger motor does help with heat.
```

---
## \#80 Posted by: chaka Posted at: 2016-07-19T15:20:34.472Z Reads: 199

```
@onloop Just weighed our motors again after discovering our scale wasn't calibrated correctly. Looks like our 50mm motors actually weigh 492 grams. 

So according to your watts per gram rule we get 984 watts @ 2 watts per gram and 1476 watts @ 3 watts per gram. The reality is we are mounting these motors to an aluminum mount which also acts as a heat sink and expands the real world output of motors on eboards unless you for some reason use a material with poor thermal properties like carbon fiber. If that is the case the heat will be isolated to the mass of the motor alone. I can see now why you must have trouble with heat dissipation. If you upgrade your motor mounts and use an aluminum plate your customers will be able to increase loading and use a wider range of gear ratios.

<img src="/uploads/db1493/original/2X/f/fa6cbd48b1a19db1e26d72c2ba1c84cbdf6ea9fd.jpg" width="376" height="500">
```

---
## \#81 Posted by: Jinra Posted at: 2016-07-19T15:50:47.004Z Reads: 194

```
That's a good point.. I hope motors don't burn up haha
```

---
## \#82 Posted by: chaka Posted at: 2016-07-19T16:21:22.866Z Reads: 196

```
I am trying my best! I set up a 12s board with a pair of 200kv OM5065's running 16/36 on 90mm abec and have been riding it as hard as I can. I will continue to use this board as my "daily driver" and see how they fair. I already know these motors are perfect for a lower gear ratio with a top speed around 25 mph. The added benefit of not having exposed windings puts these motor in a whole different category when we start thinking about real world durability.

<img src="/uploads/db1493/original/2X/f/f83021b9a5bf84a601b86230a59f7295386ae054.png" width="690" height="468">
```

---
## \#83 Posted by: Jinra Posted at: 2016-07-19T16:22:15.323Z Reads: 194

```
Nice! I may swap out my enertion mounts for yours once you have them up.
```

---
## \#84 Posted by: onloop Posted at: 2016-07-19T23:24:58.257Z Reads: 190

```
[quote="chaka, post:80, topic:6074"]
I can see now why you must have trouble with heat dissipation.
[/quote]

no problems with heat here buddy.... but thanks for your advice anyway.... 

also, feel free to make a video & get a temperature reading on those motors of yours after some hill climbs... i think the alum heat sink will benefit you.
```

---
## \#85 Posted by: onloop Posted at: 2016-07-19T23:48:00.375Z Reads: 191

```
[quote="Jinra, post:83, topic:6074, full:true"]
Nice! I may swap out my enertion mounts for yours once you have them up.
[/quote]

Just bare in mind that aluminium at 6mm thick will snap eventually.... I know this because i have been designing & building esk8 drive trains for a lot longer than most on this website (Alien & DIY mounts eventually snap). It's also very difficult to make the motor mounting plate thicker than 6mm due to the limited space on a standard 184mm wide truck when mounting dual motors, this might not be a problem with Chaka's motors anyways because they can't be mounted in Dual configuration. So he can probably make thicker plates, or maybe he will use steel as it will still help to wick away his high motor heat.

Pure Carbon fiber plate at 6mm thick has a higher tensile strength and does not get fatigue fractures like aluminium will.

Your best bet is to use motors that don't heat up & use the stronger carbon fiber plate.
```

---
## \#86 Posted by: Jinra Posted at: 2016-07-19T23:53:10.938Z Reads: 186

```
I wonder if it'd be a better design decision to use a carbon fiber/aluminum plate hybrid for esk8 motors. I'm currently running dual diag, but may switch to dual rear if @torqueboards ends up selling a extra wide caliber trucks. I'm a believer in 50mm motors given the great performance of my GT with a ridiculously low 2.13:1 reduction. They do get a little hot sometimes, but nothing as crazy as hub motors. Interestingly enough my toe motor on the GT gets a lot hotter than the heel motor.

I'd like to upgrade to 63mm motors at some point, but by then, the VESC 6.0 will probably be out and make this entire thread obsolete; not to mention the BLDC vs FOC debate!
```

---
## \#87 Posted by: onloop Posted at: 2016-07-20T00:01:34.019Z Reads: 184

```
[quote="Jinra, post:86, topic:6074"]
VESC 6.0 will probably be out
[/quote]

there is no guarantee that the VESC 6.0 will ever be released to the esk8 community.
```

---
## \#88 Posted by: Jinra Posted at: 2016-07-20T00:04:18.358Z Reads: 188

```
Why wouldn't it? That's exactly what it's designed for. Unless your insinuating that he may sell the design to a major manufacturer? I'm willing to bet the project will be community centric, even if it ends up being close sourced.
```

---
## \#89 Posted by: onloop Posted at: 2016-07-20T00:16:20.868Z Reads: 186

```
[quote="Jinra, post:88, topic:6074"]
That's exactly what it's designed for.
[/quote]

well, not really. Vedder is not making his ESC specifically for esk8 community & he never really had intended it to be so popular in this industry, it just happens to be perfect for it though.
```

---
## \#90 Posted by: Nordle Posted at: 2016-07-20T00:22:14.692Z Reads: 192

```
but he's a nice guy, and i think he will make this open source again. and even if he sells his design, someone will sell it to us
```

---
## \#91 Posted by: chaka Posted at: 2016-07-20T00:39:39.122Z Reads: 187

```
Haha! I was wondering who started this rumor. I have been getting emails from people asking me this for the past few weeks.

 The VESC has always been open source and will continue to be open source. Benjamin has been very open about this so I don't know why Jason would start a rumor like this.
```

---
## \#92 Posted by: onloop Posted at: 2016-07-20T01:02:57.110Z Reads: 186

```
[quote="chaka, post:91, topic:6074"]
The VESC has always been open source and will continue to be open source
[/quote]

Don't count your chickens before they hatch brother.

... at this stage it is not available, so there is definitely a chance it won't become available.
```

---
## \#93 Posted by: chaka Posted at: 2016-07-20T01:46:25.576Z Reads: 184

```
When v6 is released I will continue to use these 50mm motors. I really enjoy the added ground clearance and efficiency. I do think 63mm will be great for an off road build!
```

---
## \#94 Posted by: Tomkav Posted at: 2016-08-19T01:49:38.988Z Reads: 151

```
When you say the motor will get hot. Will I feel this on the can or with a sensor? I've been up some decent hills with the Enertion pro+ kit @95kg and I can hold my hand on the can and its warmish and not at all hot.
```

---
## \#95 Posted by: Jinra Posted at: 2016-08-19T02:01:40.225Z Reads: 148

```
The can can get very hot, i once was completely unable to touch it! This can happen on any size motor. Just saying that "hot" can mean pretty toasty. If your motor is just warm to the touch, I wouldn't consider that hot.
```

---
