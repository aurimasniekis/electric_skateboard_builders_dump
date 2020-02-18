# And now for somthing completely different - Pedal car Esk8

### Replies: 22 Views: 760

## \#1 Posted by: Dagad Posted at: 2019-02-06T02:27:27.802Z Reads: 292

```
![image|666x500](upload://yA9oORVaHBBYW0AWkEF4raO1sDB.jpeg) ![image|666x500](upload://cz8isVMZIqJIVv4SSdr2VONQYUd.jpeg) ![image|666x500](upload://spXE5ctiTqb2vq3XdQ1RbTgeGDF.jpeg) I just joined the forum.  I am building a 1960s pedal car into a motorized car as a birthday gift for my son.  

The dimensions of the body are very small:

12.5" wide (inside dimensions at back wheels)
34" long
24" wheelbase
7" wheels
car body w/o drivetrain weighs ~10lbs

I tried to build it up using small go-cart parts but it just wasn't working unless I put the wheels several inches outside the body and it changed the look too much.  It's just such a narrow body.  

After digging around online - It turns out some Esk8 parts would fit in it very nicely!
I'm completely new to the industry - here's what I've figure out so far:

-evolve makes a 305mm wide truck/axle that would fit really well in the back.  
-evolve also happens to sell 7" pneumatic tires (though I know others do too)
-I am going to build an aluminum frame (chassis) for it and it will have go-cart style steering in front (not a skateboard truck in front)

Goals of the build:

-configurable to at least two speeds ~12MPH (for small kids) and ~20MPH (for big kids)
-dual motor
-great slow speed response -TORQUE!  
-great maneuverability at low speed with good stop and go throttle modulation
-I prefer a wired throttle (foot throttle) but would settle for something else
-I do unfortunately have a budget - and I don't even want to share it as it will likely discourage advice - but I do  want a solid build.
-I prefer using my ~1,000 watt hours of Milwaukee power tool batteries as the battery source if possible.  

I am ready to buy parts today as I only have a couple of weeks. . . .

Need to settle on axle, mounter mounts, motors, computer, batteries, and then get it shipped and build it as quick as possible.  

I have poked around the for sale section but there is a LOT there to sift through and figure out for a new guy...

How would you guys do this unique build???

DAGAD
```

---
## \#2 Posted by: mmaner Posted at: 2019-02-06T02:38:08.714Z Reads: 256

```
Sounds like a cool project. Pics would help. There was a guy that made some 3d printable drill battery mounts, but u can't remember who. 

I'm not sure it wouldn't be better to use an Arc 200 and a single motor driving the 2 rear wheels. 
Those things handle 200 about, so I'm reasonable sure it will do the job. I have 2 Arc 200s in an esk8 running 6 inch pnumatics (6 shooters) and I can't hit full throttle from a stand still, it either throws me or I have rubber on the road. 

Also, maybe look for some older DC mountain boards for parts, the trucks are massive, might even with for the rear axle. They are like 22 inches maybe?  @longboardshort might have some laying around for cheap.
```

---
## \#3 Posted by: wafflejock Posted at: 2019-02-06T02:49:56.030Z Reads: 235

```
What's the total Watt output on one of the batteries?  I'm a pretty light guy (maybe a little heavier than a 6 year old but not if he's a big 6 year old) and when cruising around can get up to 11A (higher at times I'm sure but that's the stats I'm looking at right now, and that's a peak... average is around 3-5A) current draw at 40V, if you are going up hills or dealing with more friction etc. then the current draw is going to go up to overcome all of that.  Basically would say you probably want to be able to pull 400W from the batteries at least for a short time in order to get an optionally fast and still torquey ride.

The foot control shouldn't be a problem I found ones for ebikes with throttle on a bar control, worst case scenario you could just adapt one of those.  There are ones that put out analog control signal and VESC has analog input, if you are using budget ESC then need to see what kind of input it accepts for throttle control.  If you read the forum you'll see most everyone uses some version of the VESC for configuration and relatively long life of the ESC if setup and taken care of properly.  Also pretty easy to use an arduino to do the analog to PWM signal which is what most ESCs will accept as input, still would suggest VESC for the current control options, regen braking, can configure for only going forward or braking but no reverse (or if you want to get fancy find a way to allow them to throw it in reverse).
```

---
## \#4 Posted by: Dagad Posted at: 2019-02-06T06:54:28.519Z Reads: 181

```
@mmaner  @wafflejock Thanks so much for the quick and helpful replies  

Earlier today I did see the 3d printable battery mount. . . . . .Though because of post from wafflejock now i'm wondering if these batteries are designed to draw enough amps.  The two biggest batteries I have are 18V 9Ah.  I read that they each have fifteen 18650s with three in parallel and five in series.  I also have various other smaller batteries packs.   

I read online that these 9Ah packs are "high demand" but it doesn't say the amp draw they are capable of.  I was able to find info on their new 12Ah pack.  They claim that the tool can draw 15amps (the same as a corded tool might draw).   So based on that info - the 9Ah pack might allow 10-12 amps draw?  

If I wire two packs in serious I think that makes 36Volts and 9Ah.  If I understand this right, I could also use my two 5Ah packs and put them in parallel and now have 36volts and 14Ah.  Though I think that might just make them last longer - not necessarily allow more current to flow.  (And some advise against mixing different amp hour packs)
```

---
## \#5 Posted by: Dagad Posted at: 2019-02-06T07:18:00.594Z Reads: 171

```
@mmaner - Regarding the Arc200 - I had to look it up - looks like a high-end controller for $300.  Though my understanding is I would need two for a dual drive - $600 in computers is a lot - if It did both motors I would be interested as it looked like a great controller (though I do have zero controller experience)

You mentioned I should drive both wheels with a single motor - were you suggesting a "live axle" style of build where the two wheels are locked together like most go-carts?  I was trying to avoid this because I would lose my low speed maneuverability.  Also - I know how to do this with a large keyed shaft and keyed go-cart wheels but have not seen it done with mountain board style wheels.  are there keyed hubs available?  Or did I miss what you're saying completely.  

Regarding the axle - if I understood you correctly, you recommend an extremely wide (22") axle. 
 I'm not looking for an axle that places the wheels outside the body - I've found a few that are around 12" wide and that will place the new wheels almost exactly where the original wheels are which is what I think will look best.
```

---
## \#6 Posted by: wafflejock Posted at: 2019-02-06T15:10:54.108Z Reads: 156

```
Yeah you're on the right track with looking at the number of cells and number of cells in parallel, that along with the "bus" or wires between the cells and from the cells to the place power is being drawn are going to be the limiting factors.  Ultimately best way to know is to test, but you could end up damaging the battery in the process of finding its limit.  If you have 3P and each cell can deliver max 5A then can deliver 15A with all three in parallel.  You're correct in that increasing Wh is effectively increase in capacity but voltage is what drives rpm and amperage is what drives torque (in a simplified view of things).  Increase in Wh isn't necessarily an indication that the max discharge (A) is increased but it's typically the case because to increase Wh without increasing voltage you add cells in parallel effectively adding more "buckets" to draw the current from.

If you use a programmable esc and can limit amperage there then you should be able to do some testing and see if the batteries voltage sag down under load at different amperage slowly stepping it up (hard part is always having it under load while monitoring things but can use Bluetooth module on vesc or make a "poor man's Dynamo" couple of skate trucks upside down and/or shoe you don't care about to act as brake on the wheel/motor).

If it turns out one battery isn't enough you could always put them in parallel the risk is basically always in running some cells that are in series to different voltages and having some go way too low while under load and/or over discharging the cells (too high amp draw), putting more in parallel helps mitigate that issue though too.

---

Also sounds all correct to me with regard to putting in series increasing voltage most people here target somewhere in the 8-12S range to keep the current out of the batteries and through components as low as it can be without being over the max voltage supported by the speed controller (also need to account for kv of motor and gearing or pulley ratios with regard to max speed and torque). Lots of calculators around to help guesstimate things but really get your data by putting rubber to the road.  I don't really see an issue mixing different mah capacity batteries the only thing is to have the same voltage on cells connected in parallel or they will self balance (discharge one into the other), and you don't want any given cell to drop below 3.0V, usually 3.3V or 3.5V, depends on chemistry and cell construction, average across cells is used as a cut off voltage to prevent letting any given one getting too low (once over discharged a cell will lose capacity, won't fully charge and could be more dangerous while charging so usually means battery rebuild or replace which is costly either way).
```

---
## \#7 Posted by: Dagad Posted at: 2019-02-06T23:18:09.950Z Reads: 116

```
@wafflejock
Thanks for the helpful reply!  I am going to give the two 18V 9Ah Milwaukees a try.

I have another possible direction with the build.  Much less expensive - Backfire has 6.5" hub motors with tires for $100 each.  The ride will be stiff but the diameter will probably be OK.  900 watt motors is what they say.  Also - should be good for low end torque - and easy to mount.  Not sure the drawbacks beside being heavy and not as smooth of a ride?   What do you guys think?  What's the drawback?  Are they too loud or not strong enough?  I would probably get their controller - unless  you guess recommend I don't????  I would be willing to spend money on a nice controller if it's do-able for a new guy to set up in an hour or two.
```

---
## \#8 Posted by: b264 Posted at: 2019-02-06T23:27:08.167Z Reads: 112

```
I think @KaramQ might have a DC motor that might work
```

---
## \#9 Posted by: KaramQ Posted at: 2019-02-06T23:30:16.882Z Reads: 111

```
Sorry, I actually sold the dc motor to @ZachTetra
```

---
## \#10 Posted by: ZachTetra Posted at: 2019-02-07T00:06:20.439Z Reads: 111

```
How much do you want a 36V brushed motor with the ESC?  I was gonna put it on a nickelboard but I'm already working on something else so I'd be willing to resell it
```

---
## \#11 Posted by: KaramQ Posted at: 2019-02-07T00:24:02.977Z Reads: 109

```
Really interesting build, not sure how you would add a foot pedal for acceleration. What I can tell you is I would not recommend using those drill battery’s. Turningy sells some cheap battery’s that I think would be perfect for this. Stoked to hear more about this build. Also hobby king offers cheap motors, but if you want torque buy some @psychotiller motors
```

---
## \#12 Posted by: mmaner Posted at: 2019-02-07T01:11:57.791Z Reads: 96

```
The reason I suggested the Arc 200 is because you can push enough amps to turn 2 wheels without loosing torque.  Plus you can have reverse, sensors, anything you can have with a VESC.  Yes, its expensive, but for high amp draw applications its just about unbeatable.

If you use a standard 63, 80 or 88mm motor you can remove the shaft and replace it with a longer shaft so you can run 2 pulleys.  Regarding the axle, I dont know.  I would junk the existing drive train and start over.  Probably use something that has removable axles so you can modify the width to whatever you want, like Surf Rodz or whatever.

Battery wise, I would just go with lipos, maybe 6 2s 8000mah or something, that will give you a 12s pack with mad amp delivery.
```

---
## \#13 Posted by: wafflejock Posted at: 2019-02-07T03:37:24.963Z Reads: 90

```
Gotcha will look into that one only have hands on with the vesc and a few rc car escs (aside from quadcopter escs)... Have seen James the xrobots guy on YouTube and a few others using the "oDrive" think that's more of a alpha/beta thing still, the arc200 looks nice but maybe a bit pricey.

Agree LiPo pouch batteries are probably the best way to keep the battery relatively cheap and still able to easily supply the amps needed.  Also use case probably isn't long distance trips so swapping batteries for extra range seems reasonable.
```

---
## \#14 Posted by: PatRocks Posted at: 2019-02-07T03:44:40.755Z Reads: 86

```
Loving the MPFC ref
```

---
## \#15 Posted by: Dagad Posted at: 2019-02-07T06:46:52.679Z Reads: 81

```
You guys rock - I really appreciate everyone piping in - extremely helpful for someone that's green.  

Looks like power tool batteries will not be used.  Lipo pouches make sense and @wafflejock is correct this tiny car will not be used as transportation - just for playing in the yard, driveway, sidewalk, park, soccer fields, etc.  and a smaller pack or swappable packs are fine.  

@mmaner thanks for explaining that controller a little more - I didn't realize it was in fact the most economical way to get monstrous torque.  Very cool.  

@zachtetra thanks for offering the motor - honestly I have no idea if I want it.  I've heard brushless is quieter, and better, smaller too perhaps - I'm not sure.   If it meets my goals above and it's quiet enough then yes I would consider it.   Though I don't want one wheel drive - If i use a single motor I'll have it power both wheels.
```

---
## \#16 Posted by: Cieszyn Posted at: 2019-02-07T16:17:56.260Z Reads: 66

```
Look at hoverboards wheel, they come really cheap from used toys, you can control them with cheap 350w Chinese bldc ebike controller.
I ve seen a build like that on some forum, but really can't find it now. However such wheels would do around 10mph - plenty fast for backyard but not possible to go near 20 mph.
```

---
## \#17 Posted by: dareno Posted at: 2019-02-07T19:56:24.920Z Reads: 58

```
Oh my friend if you were over here I would drop off my sons wiggles remote car for butchering.  I got it for him when he was 2 and put him in it and he crapped his pants and never touched it again.  lol
I upgraded the battery to a lipo and it works fine.  Btw have you checked the value of that pedal car?  Got a sneaking suspicion they are worth a mint.
```

---
## \#18 Posted by: b264 Posted at: 2019-02-08T02:31:22.561Z Reads: 52

```
[quote="Dagad, post:15, topic:83307"]
this tiny car will not be used as transportation - just for playing in the yard, driveway, sidewalk, park, soccer fields, etc.
[/quote]

If that's the case, do you really need two wheel drive?  If you have mechanical friction brakes on the front wheels, I think 1 wheel drive would be plenty.  Not joking.

A single 6374 drive train would be fine, plenty of power for this sort of thing.

You don't want this to be able to beat a Mustang off the line, right?
```

---
## \#19 Posted by: Dagad Posted at: 2019-02-09T08:40:28.278Z Reads: 54

```
@b264  Thanks for asking - the answer is No, it doesn't really need two wheel drive.  But if I was going to go one wheel drive (or live-axle two wheel drive), I likely would have already built it with non-esk8 parts as I can actually FIT a single larger scooter motor in the 12.5" that I have to work with - for example, I could use this motor: 

https://www.goldenmotor.com   (click BLDC on the left and scroll down to 3KW motor)

alternatively, I use this to drive one wheel directly:

https://www.milwaukeetool.com/Products/Power-Tools/Fastening/Impact-Drivers/2757-22

But to answer your question, It's kinda a personal thing - I really don't want to power just one wheel.  I grew up with muscle cars as well as four-wheel drive off-roading vehicles and both are significantly hindered by a single powered wheel. . . so it probably comes from that.   

Also - could use extra torque for several other reasons including: lively starts- using on the bumpy grass a fair amount - also part of our driveway is steep - also, It's not just for kids, I want a full size adult (me!) to be able to sit on it and goof-off.

Low speed maneuverability is also much worse when both wheels share the same axle (you can't easily turn sharp) so a single motor live axle set up is out - that brings me to an esk8 style set up - a small motor powering each wheel and the width of the whole setup is narrower that 12.5".

That said, I was searching through posts yesterday and I did see a board with an unusual set up - dual large motors - one was hanging in front of the axle, and the other behind the axle - I had never considered this and it does open up some options for me:-)
```

---
## \#20 Posted by: Dagad Posted at: 2019-02-09T09:06:13.040Z Reads: 50

```
@dareno - because of you I looked up wiggles car on youtube (didn't know what it was).  Turns out its a power wheels style plastic car.  Some dad added a gear box/motor to one and was running it on 18 volts.  Little kid was doing wheelies and having a great time!  

https://www.youtube.com/watch?v=sbVNKYzxI8E

That is kinda what I had in mind - but that car is probably maxing out at 10mph which is fine if I can keep it cheap - but if I'm gonna spend more than a couple hundred dollars on it, I want it to go faster :-)
```

---
## \#21 Posted by: Dagad Posted at: 2019-02-09T09:21:19.117Z Reads: 49

```
@Cieszyn

Thanks - I was thinking the same thing - hover wheels would be an inexpensive way to complete the build.  a few days ago I was going to order the backfire ranger wheels because they said they were 900w - but they more I look around, I feel that number may be over inflated because every comparable board is advertising 350w with the same specs - so not sure what to believe.  It would be worth it to me to spend $100 per motor/wheel if it was the right motor for this little build i'm doing. . . I'm actually really attracted to hub motors

I heard they are much heavier - negative
They seem wimpy because low voltage - negative
I heard they are much quieter - big positive
I heard they are much more water proof - positive (very rainy here year round)
No pneumatic tires available in my size - negative

If these worked - I would be willing to go four wheel drive to get enough torque - what do you guys think - should I build it up with hoverboard wheels?  

If I pair the hoverboard wheels with a quality controller, up the volts, and give them plenty of amps - are these worthwhile?  

I'd LOVE to try them if it's not a waste of time. . .
```

---
## \#22 Posted by: Cieszyn Posted at: 2019-03-07T03:16:50.366Z Reads: 34

```
I've build hoverboard wheels skateboard 4WD. I actually just connected 2 of them because it was a lot of torque already, I used the other two for extra braking. They are designed to go 10mph @ 36V. If you decide to overvolt them to 48-60V you will go faster, but you could easily destroy the motor if you dont limit the current. You could probably buy a pair from broken toy for 20-40$ (I payed less that  20$ for mine) so they are muuuuch cheaper than what available. Worth only if you accept the speed limit, other than that they are perfect.
```

---
