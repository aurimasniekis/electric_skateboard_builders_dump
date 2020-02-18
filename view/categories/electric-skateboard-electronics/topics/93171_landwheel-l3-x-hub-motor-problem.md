# Landwheel L3-X hub motor problem

### Replies: 77 Views: 824

## \#1 Posted by: BearBoi Posted at: 2019-05-08T10:16:48.175Z Reads: 91

```
One of my hub motors stopped spinning. At first I had a problem where one of the motors needs to be in a certain position to "catch" and spin, once it got up to speed it was fine, and never noticeable as long as I kick-started my board. Now I can't get it into gear at all. I can hear the motor spin up as I push the throttle and the hub "twitches", but it's not spinning, not even from a rolling start. if I try to step on the board and give it throttle the controller vibrates and blinks constantly and it's obvious something is broken/loose inside the motor.

I have unplugged the motor from under the battery which lets me run single motor, which works okay, but of course I want dual hub motors. I plugged it back in the other day and got it working somewhat for about 15 minutes until it broke down again.

Any ideas what could cause this? and also any advice on getting the 13mm nut loose inside the hub cap? I got a skate tool with the landwheel which IS thin enough... But they decided to put a thick plastic cover around it which makes it impossible to reach, and I'm worried if I try to file that down the entire tool will break.
```

---
## \#2 Posted by: BearBoi Posted at: 2019-05-09T07:00:01.690Z Reads: 65

```
Here is what I have discovered since this post:

The working motor no longer works when I plug the cables from the wrong side of the ECU. However I can't get the non working motor to spin regardless which part of the ECU it is connected to.

I also noticed the non working motor is "springy" if I turn it slightly it doesn't lock into place, it springs back.
```

---
## \#3 Posted by: KaramQ Posted at: 2019-05-09T07:32:55.415Z Reads: 60

```
I had one, could you send a video of it?
```

---
## \#4 Posted by: dareno Posted at: 2019-05-09T10:07:46.742Z Reads: 66

```
https://www.electric-skateboard.builders/t/landwheel-l3-x-reviews/45697

There is a thread dedicated to this drive.  Search function is still up and running I believe.  
FYI  Please do some trying before creating new topics.  Keep it clean.  Try before you cry.
```

---
## \#5 Posted by: BearBoi Posted at: 2019-05-09T11:19:06.135Z Reads: 59

```
I see your frustration and I apologize for any mistakes on my part, perhaps you are right that I should not have made a new thread, or I should have thought out my post better.

However, that said. I have looked through all major landwheel related threads prior to posting. I didn't find an active thread about issues, and when I looked through topic "Esk8 Electronics" seemed the most relevant. I have looked through the thread you linked. However I didn't think my question fit there as it is mostly for discussing the drive and giving tips and tricks and sharing news. It is a great thread though and I have spent a lot of time on there.

As for testing before I post, I have done a lot of testing. I just never tried cross-wiring the ECU, and I already knew it was "springy" prior to my OP, just forgot to include that part. I have already spent 2 weeks testing and tinkering with my board and hours on Esk8 before posting. Even gone to a hardware store multiple times to get the tools I need to disassemble.

And I have read on this forum that initially V4 shipped with a suitable tool, but found nothing about alternative tools I could use for a newer model, just one post about (possibly) being able to file a thicker one down, but no comment from someone who had tried and succeeded.
```

---
## \#6 Posted by: BearBoi Posted at: 2019-05-09T11:21:24.984Z Reads: 49

```
I will send a video when I get home from work :slight_smile:  
You had "one" what though?
```

---
## \#7 Posted by: KaramQ Posted at: 2019-05-09T11:23:47.223Z Reads: 48

```
I had the l3x and it was a blast but I sold it
```

---
## \#8 Posted by: BearBoi Posted at: 2019-05-09T11:33:00.709Z Reads: 48

```
Okay gotcha :)
```

---
## \#9 Posted by: pkasanda Posted at: 2019-05-09T14:56:37.666Z Reads: 50

```
So, there are two things to try to fix this:

1) Disconnect the sensor wires on the motor that is not functioning properly.  Make sure you are disconnecting the correct sensor wires becasue they usually cross over. Left sensor on the ESC corresponds to right hub.  If this fixes the problem then ride with one sensor wire connected and the other disconnected.  You will not notice much difference in performance compared to original.  The sensor wires assist with take off but they serve no purpose as soon as you have picked up speed.  So one motor fucntioning on sensors is enough so that you don't need to kick start from a stop.
I see that you have tried swapping motor wires to opposite sides of the ESC.  That was a good test.  But if you are connecting the sensor wires when you swap then you are just moving the problem from one side of the board to the other.  If the good motor works on either side of the ESC then you can be hopeful that diconnecting the sensor wire for the trouble motor may resolve your issue.
If you have swapped sides then you have probably already found a way to remove the glue that holds the sensor wire connector together. 
Just in case, here is the easiest way. To disconnect the sensor wire you need to remove the yellow glue.  I find that pinching the glue with the tip of a set of wire cuters works best.  just grab two edges of the glue and squeeze paralell to the connector.  Dont pinch or crush any part of the connector.  Once you crush the glue a bit it will peel right off.

2) The second possibility is a bad solder connection at one of the six motor wire connections.  This is very unlikely if you have tried the good motor on both sides of the ESC and it works on both sides.  Just in case here are the diagnostics to try.  If the connection is still making contact then motor function could be intermittent.  If its completely disconnected then the motor would vibrate in one position.  To test for this fault, pull moderately hard on each connector while holding the wire an inch from the connector.  Pull just hard enough to break the insulation, not hard enough to break copper wire.  If the connector pulls away you had a bad solder connection.  This fault was more likely on the V2's.  Far less likely on the L3-x & V4.

Based on your description, I'd say your problem conforms to the first solution, not the second solution.
```

---
## \#10 Posted by: Kingdom421 Posted at: 2019-05-09T15:43:30.772Z Reads: 38

```
Contact @revel_flo I didn't have a hub key either and they sent me one no problem. Also they don't charge much for repairs if you just send it in. They are a great company with awesome customer service.
```

---
## \#11 Posted by: BearBoi Posted at: 2019-05-09T16:45:23.936Z Reads: 38

```
Thanks a lot :smiley:   :fu: You were spot on with solution 1. the glue was so worn, I didn't even need to grab my wire cutters, I could peel it off with my nail. Glue on the broken side was not fully covering, dust particles have coated the inside of the connector. I suspect it will work again after cleaning and applying new glue, will try that next. I noticed the worn connector before but was not brave enough to peel away the glue previous to your post.

You seem to know a lot, One quick question, been looking for the answer to this everywhere.
Do you know what the different color-coded wires mean? disconnecting the blue wire seems to do nothing, but surely it has a purpose too?
```

---
## \#12 Posted by: BearBoi Posted at: 2019-05-09T16:48:33.634Z Reads: 35

```
Thanks for the reference, I messaged @revel_flo seems this time I don't need to send in anything though :) got it working with @pkasanda helping. Ended up being a bad connection on the sensor wire for the faulty motor. Once I got that fixed it is flawless again.
```

---
## \#13 Posted by: BearBoi Posted at: 2019-05-09T16:50:15.240Z Reads: 38

```
I won't be sending a video anymore, got it working w/ the help I got from this thread already. Ended up being a bad connection for one of the sensors. Got that sorted and it is mint again :smiley:
```

---
## \#14 Posted by: revel_flo Posted at: 2019-05-09T16:51:50.666Z Reads: 39

```
:ok_hand: Still though, if you can get your hands on a hub key I think it would be well worth it. I'd recommend checking and tightening hub motors every 50 miles or so, if possible.
```

---
## \#15 Posted by: pkasanda Posted at: 2019-05-09T16:56:06.944Z Reads: 41

```
[quote="BearBoi, post:11, topic:93171"]
Do you know what the different color-coded wires mean? disconnecting the blue wire seems to do nothing, but surely it has a purpose too?
[/quote]

Orange | Blue | White | Green | Yellow | Black
5V | Thermostat | hall1 | hall2 | hall 3 | GND |

Many consider the blue thermostat wire to be optional, particularly when replacing the landwheel ESC wiht a VESC
 Example...Wireing patern to connect Landwheel hub motors to Maytech VESC
![image|401x409](upload://vflNFfdxFOpl1uFZc4IrIzjsWur.jpeg)
```

---
## \#16 Posted by: BearBoi Posted at: 2019-05-09T17:04:56.814Z Reads: 41

```
Oh cool, thanks. As a programmer I find VESC very intriguing, would be fun to tinker with. But that will have to wait a while.

But I was more referring to the 3 thick wires, ( green | blue | yellow )
```

---
## \#17 Posted by: Mikenopolis Posted at: 2019-05-09T17:19:30.559Z Reads: 41

```
[quote="BearBoi, post:16, topic:93171"]
green | blue | yellow
[/quote]

Those are the PHASE wires
```

---
## \#18 Posted by: BearBoi Posted at: 2019-05-09T17:52:44.133Z Reads: 39

```
https://youtu.be/sc8Nc225Qv8 

Celebrated a bit too soon :sweat_smile:

Yes, unplugging the sensor connector did make it "flawless" for a few seconds of testing. In the video you can hear what sounds like electrical "clicks" from the motor. This video is the last time I had it spin and not just twitch slightly.

I guess I need that hub key even more than I thought.

@pkasanda, @revel_flo @Kingdom421
```

---
## \#19 Posted by: revel_flo Posted at: 2019-05-09T18:00:49.375Z Reads: 33

```
[quote="BearBoi, post:18, topic:93171"]
unplugging the sensor connector did make it “flawless”
[/quote]

Have you tried disconnecting both hall sensor connectors? I think you might have the wrong one disconnected.
```

---
## \#20 Posted by: BearBoi Posted at: 2019-05-09T18:10:22.287Z Reads: 35

```
I did now, both are disconnected, same result :confused:
```

---
## \#21 Posted by: pkasanda Posted at: 2019-05-09T18:21:13.379Z Reads: 30

```
So here is what you want to do.  Leave the hall sensor wires connected to the good motor.  Disconnect the hall sensor to the bad motor.  Then mount the landwheel on a board and see how it works.  The motor wiht the functioning sensors should bump start the motor that has no hall sensor wires.

The purpose of the hall sensors is to get the motors turning so you don't need to kick start.  But one motor with sensors should be enough to get the job done.
```

---
## \#22 Posted by: BearBoi Posted at: 2019-05-09T18:38:11.522Z Reads: 26

```
![IMG_20190509_203151|375x500](upload://vLazgwJwWLG4lc0CZpAgLmQaHUZ.jpeg) 

To clearify, this is a hall sensor, right? I will screw everything in place and go outside with both disconnected and roll down a hill to help it and see what happens.
```

---
## \#23 Posted by: pkasanda Posted at: 2019-05-09T18:44:46.156Z Reads: 26

```
Yes those are the hall sensor wires.  But I suggest you connect the sensor wires for the motor that functions well and disconnect the sensors for the motor that does not function well.  You should get better results than if both motors have no hall sensor wires.

Also, make sure you have not mixed up any of the motor wires or hall sensors wires left to right.  You may need to remove the trucks to trace the wires properly.  Its hard to tell which wires correspond to which motor just from looking at where the motor wires enter the enclosure.

If you've mixed anything up left to right then nothing will turn properly.

You started off saying that one motor was working well.  I did not see that in your video.  The motor that was working well with hall sensors should also work well wheels up without the sensor wires.  So I'm concerned that you may have jumbled the motor wires.
```

---
## \#24 Posted by: BearBoi Posted at: 2019-05-09T19:05:37.620Z Reads: 24

```
The good motor still works well. On the video it's a bit hard to tell because I focus the camera on the bad motor. I will still take off the trucks and properly trace the wires though
```

---
## \#25 Posted by: Kingdom421 Posted at: 2019-05-09T19:11:46.121Z Reads: 24

```
I disconnected my halls on both escs and they still work great infact very smooth.
```

---
## \#26 Posted by: pkasanda Posted at: 2019-05-09T19:26:05.510Z Reads: 24

```
Dring the disassembly, be very careful to protect the Antenna wire and the copper antena film that it terminates on.  WHat you don't wan to have happen is for the shell to fall off and yank the end of the antenna off.  So if you are removing the shell, take a inute to peel the antena film off the shell and stick it to the ESC.  If you damage that antenna then the ESC will be useless.  After you re-assemble, you can move the sticky antenna film back to the inside of the shell.
```

---
## \#27 Posted by: pkasanda Posted at: 2019-05-09T19:35:13.551Z Reads: 25

```
@Kingdom421 is correct.  with the sensor wire disconnected and no load on the motors, the  sensorless operation of the motors should be smooth.  So first check if you have done any left to right reversals.  Then check that none of the motor wires has a broken/intermittent connection.

Earlier, you said that the blue wire did not seem to do anything and it turned out that you were talking about the blue phase wire for one of the motors.  So if there is no difference in the operation of the malfunctioning motor  with or withot the blue motor wire then that wire is broken somewhere.

A BLDC motor needs all three wires.  The ESC times the charge alternately between different pairs of the three wires so that the stator is constantly being pulled towards one set of magnets and pushed away from another set.

If you loose one of the three motor wires then the motor just wiggles instead of turning.

If its gotten worse since you've started playing wiht it, its becasue the broken/intermittent connection has gotten worse.

It could be a bad bullet connector, a bad solder joint to the bullet connector, or a broken wire inside the insullation.
```

---
## \#28 Posted by: BearBoi Posted at: 2019-05-09T23:00:56.220Z Reads: 22

```
Took as much as I could apart. Unscrewed the drive and took of the housing. I don't see any visibly damaged wire. No wires were crossed.

About the blue wire, my bad. I must've gotten things mixed up. Two weeks of daily tinkering with no luck can get to a man's head. I had read about the sensor wire previously and had a faulty memory about me testing with no difference. I tried again today, no matter which wire I pull it has a significant difference on the working motor.

I do still get electric pops from the faulty motor and I did see one small spark on the side towards the trucks. I'm leaning towards the problem being at the solder points to the motor.

It was working for a little bit after unplugging the sensor, but that could very well be random. It has worked a few times before in these 2 weeks. My next step will be going to another hardware store and try to get my hands on a fitting tool.
```

---
## \#29 Posted by: pkasanda Posted at: 2019-05-10T00:38:58.990Z Reads: 20

```
If you take a 10mm or 3/8 inch nut driver, 


![image|690x430](upload://xjNVM7KMXv1uHtKPWvgR3rffLKM.jpeg) 
and sand it down on a belt sander, then you can make your own tool for removing/tightening the axle nut.
```

---
## \#30 Posted by: BearBoi Posted at: 2019-05-10T06:19:00.814Z Reads: 17

```
Looks like the same size as the front wheels. Which is 13mm. Also read on here someone said the hub nut is 13mm.

Anyhow. I took your message to heart and I have messaged a guy in my city renting out power tools and will be renting a belt sander for a day.
```

---
## \#31 Posted by: pkasanda Posted at: 2019-05-10T15:50:53.017Z Reads: 23

```
Correct you are - 13mm or 1/2 inch nut driver, 

Have a cup of water to cool down the nut driver.  If you don't keep it cool, the metal will loose its temper (hardness).  Dry it off before you start sanding again or your sand paper/Emery cloth will disolve.

Best  type f belt sander:

![image|569x471](upload://yx9IXzmaVLnyJOglhylDfCCsGXO.jpeg) 

Might also work but the belt may wear out before you are finished:

![image|436x500](upload://40XR4SGb0Iix4APmkiGcR5wYIIs.jpeg) 

Would be very difficult with one of these becasuse you would have no accuracy:

![image|440x260](upload://1kintczHPvYGoND9K7cFdRonLYv.jpeg) 

The walls need to be ground very thin.
```

---
## \#32 Posted by: BearBoi Posted at: 2019-05-10T16:50:17.423Z Reads: 21

```
Used two different models of belt sanders, an angle grinder, and 3 people helping, a bucket of water and an hour of work to bring down my socket thin enough. Couldn't get the tool down to a working shape...
BUT managed to get the nut off with two screwdrivers, one on either side of the nut and some patience.

Does anyone (preferrably in Europe) have spare parts for a Landwheel?

The problem has been diagnosed...  
That piece of metal I am holding is the bit supposed to be welded to the trucks, it keeps the motor from freespinning. Which explains the times I heard the motor spin but the hub not moving.
Because it was loose it managed to slide and grind off the cables. I need new rear trucks for sure Since the trucks are aluminum I can't really weld it back well. Possibly new motor? hard to solder anything onto those frayed short ends unless it's possible to push out the bearings and expose the wire.

Thanks to everyone for being so helpful so far :slight_smile:  
@pkasanda @revel_flo @Mikenopolis @Kingdom421  
sucks I can't ride my esk8 for at least a couple of weeks though.

![IMG_20190510_182127|187x250](upload://b1Hk5XZJT2tALf0QYCqXGbY0bwY.jpeg) 
![IMG_20190510_182151|187x250](upload://ldB3tJC916qEu0ikQsBsLJRxYcC.jpeg)
```

---
## \#33 Posted by: Mikenopolis Posted at: 2019-05-10T18:43:21.965Z Reads: 21

```
Are the front trucks the same? I remember them having the grooves for the wires. If so can you just use that? Sucks that you are not in the US or a few people might be able to help
```

---
## \#34 Posted by: visnu777 Posted at: 2019-05-10T18:51:55.672Z Reads: 23

```
I might be able to help, I managed to destroy both motors at the same time so I have that truck and no real use for it. I wanted to rewind them but failed to open the cans :(
```

---
## \#35 Posted by: BearBoi Posted at: 2019-05-10T18:58:24.497Z Reads: 22

```
Front trucks are the same except for the bit that broke off mine. It is supposed to be welded on solid to the truck, but mine came loose.

Also, yes being in US/Asia would help now. I'm in Sweden though :/
```

---
## \#36 Posted by: BearBoi Posted at: 2019-05-10T19:05:43.133Z Reads: 24

```
Sorry about your blown motors :(   
You're in Germany, right? I'm in Sweden. Perhaps that could work.  
But are you sure you don't want to try and repair what you have?
```

---
## \#37 Posted by: visnu777 Posted at: 2019-05-10T19:09:23.945Z Reads: 24

```
On the long run yes but it will take some time. When I do I can use a maytech truck or cut a normal truck to fit so you can have the landwheel. I have to get the second motor off the thing though, I printed a petg tool for the nut but it only worked on the first so far....
```

---
## \#38 Posted by: BearBoi Posted at: 2019-05-10T19:50:59.998Z Reads: 25

```
If you manage to print a working tool I would pay extra to have it come w/ the truck. Was an unsuccessful adventure grinding down an existing metal skate tool.  

This is as good as we could get. Hence why I gave up on it and settled for using two screwdrivers
![15575176201176152290281379110760|187x250](upload://gHrLsQGK6FqxgwaQupMpmwt2wQG.jpeg)
```

---
## \#39 Posted by: pkasanda Posted at: 2019-05-10T19:59:17.374Z Reads: 23

```
Do you have a second set of PU for the motors?  THose PU look pretty worn out.  I'm just wondering if you might be better off getting a replacement hub assembly from another manufacturer.  If you could get a complete Landwheel hub assembly that would make sense but with just a set of landwheel trucks, it seems to me your still missing one motor and maybey 2 PU wheel covers.
```

---
## \#40 Posted by: visnu777 Posted at: 2019-05-10T20:07:23.645Z Reads: 23

```
Speaking of which: 😁 I also have a set of MBS at wheels casted on top of a landwheel sleeve 😎 the hubs are awesome, as long as they were alive at least 😂
https://www.electric-skateboard.builders/t/diy-wheel-casting/6546/36
```

---
## \#41 Posted by: pkasanda Posted at: 2019-05-10T20:36:03.140Z Reads: 22

```
[quote="BearBoi, post:38, topic:93171"]
This is as good as we could get. Hence why I gave up on it and settled for using two screwdrivers

![15575176201176152290281379110760.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/7/5/750c16e631b67a11c20ef3605d8df04cb91a4802.jpeg)
[/quote]

I think you would have had much better luck with a Nut Driver.

![image|349x214](upload://am56lgXgU8iQ8Ez37IQjpxRd5bL.jpeg)
```

---
## \#42 Posted by: BearBoi Posted at: 2019-05-11T09:52:33.936Z Reads: 20

```
I do have 2 fresh PU wheels. They just need a bit of sanding on the corners and they are good to go. As for the motors, as long as I can separate the cables on the bad motor it should be fine. That last part might be easier said than done though.

Also, yes. A nut driver would be easier. Problem is I don't own one. And paying for a tool to then (potentially) ruin it is iffy
```

---
## \#43 Posted by: visnu777 Posted at: 2019-05-11T14:09:22.806Z Reads: 20

```
![15575837393205097128529440958356|666x500](upload://4uRRFPeDRqxhghA9ha7DzKXcPCQ.jpeg)
```

---
## \#44 Posted by: pkasanda Posted at: 2019-05-11T18:37:28.128Z Reads: 22

```
@BearBoi
Here is something to consider that I only discovered this morning.

Your ESC may already be damaged if you were using it with a damaged motor or disconnected motor wire.

Just two weeks ago I built a  6 wheel drive skateboard with Landwheels. 

![image|504x142](upload://6FJZSXMzCoH40WjxAM3oauMCW5z.jpeg) 

![image|505x185](upload://yAp68tDOgEYCYcNzdu544Dqnsdj.jpeg) 

I top mounted the third Battery compartment.  I needed to legthen the wires to reach the hub motor.  It worked great for two weeks, then I had motor problems similar to yours.  I traced the problem to one of the motor wires having broken at my solder joint.

![image|511x376](upload://1fJZzQTuieUbfd9AEnmHZJqldry.jpeg) 

I resoldered it this morning but the drive was unusable.  The motors turned but irregularly and they made a tonne of noise.  I tested it with two different sets of Hub assemblies so I know that it is the ESC that is fried.

I just wanted you to think about this before you start shipping used parts internationally.  It looks like you got to ride quite a few kilometers on your L3-x.  With broken trucks, broken motor and a high probability of a damaged ESC, your L3-x may have exceeded its useful life. 

You might want to to start thinking about your next ride.
```

---
## \#45 Posted by: visnu777 Posted at: 2019-05-11T19:30:54.884Z Reads: 20

```
@BearBoi If you decide to leave them be I would like to have the motors 😊 to check if they are dead. I will pay for shipping and if they are still usable I'll pay you 50€.
Alternatively you could have the parts above for 50€ 😁
```

---
## \#46 Posted by: BearBoi Posted at: 2019-05-11T22:40:58.206Z Reads: 19

```
Thanks for the heads up I have admittedly given my landwheel a very rough life. Took some time today too further look over my bad motor. Looks impossible to get a good soldering, I can barely tell which is which and about 1mm is exposed even after pulling with tweezers. And yes your observations are correct, rode maybe 60 miles after noticing initial problems, and when they were severe enough to not keeg going, I unpluged the motor and went another ~20 miles before disassembly. A lot of which on rough terrain. Today I have made up my mind, I will take the expensive lesson and make a DIY board that I make sure to take good care of.

Planning to re-use the housing and batteries (I have 4 batteries) but change the ESC, trucks and motors. Still making up my mind of what to order and how to assemble things, and still learning (any and all advice is appreciated)

Maytech (say) they have a big sale on almost all products. Not sure I believe it though. Looks a bit sketchy and too good to be true...  
Like this hub motor claiming to be a 60% price reduction.
Also I'm a web developer, making e-commerce websites is what I do for a living. Just looks sketchy.

I'm thinking all I need to import is a good Vesc compatible control unit. The rest I can find locally.

https://maytech.cn/collections/in-wheel-hub-motors/products/brushless-hub-motor-hall-sensor-motor-mto9055hbm-100-ha
```

---
## \#47 Posted by: BearBoi Posted at: 2019-05-11T22:53:11.755Z Reads: 22

```
The bad motor is 100% done. spent a couple of hours thinking of ways to revive it. But the exposed wire is just too burnt and short, even after trying to pull on it. The other motor seems fine though from what I can tell. I would gladly send them for 50+ shipping. I just don't think it would be worth it for you.

1 beat up (but working) motor, plus one seemingly totalled motor is probably not worth 50 eur + ~8 in shipping.

As this is my only e-board and the withdrawals are real, expecially right before summer hits. I will be shopping for parts and try to get a working landwheel/DIY hybrid
```

---
## \#48 Posted by: pkasanda Posted at: 2019-05-12T00:41:59.453Z Reads: 21

```
If you want to build a DIY, I recommend against using the landwheel batteries.  The landwheel battereis have a discharge rate that is five or six times what most Eskate batteries supply.  You might end up building a board that accelerates like a slingshot. That may sound cool but Its no fun if you can't stay on.  These were  my results when I combined a VESC+ V2 landwheel hubs plus a Landwheel V4 battery.  Within the hour, my VESC's were also blown.  Teh second problem is that if you to manage to put together a Working DIY, It may be hard to keep your Landwheel battery in working order.  It just takes one incidence of over discharging the battery and its toast.  The Landwheel ESC does a good job of throtteling down the power to prevent over discharge.  I don't think you are going to find the same calculations running in a VESC.

You might find there is a good market for your landwheel bateries from others who have working landwheels but no batteries.  That coud help you to pay for your next board.

If you are on a budget, you might also want to think about a used boosted board.  They last forever and there are lots of used ones for sale becasue riders like to upgrade to newer boosted boards or they decide they want a longer range than they can get from boosted boards.

You can spend a lot less on a used Boosted board than you can spend on a DIY that might break in a week or a month  or maybe 3.

pk
```

---
## \#49 Posted by: visnu777 Posted at: 2019-05-12T02:09:31.597Z Reads: 19

```
Another idea: I'd trade a working used Diyeboard hub kit for the two motors :)
```

---
## \#50 Posted by: BearBoi Posted at: 2019-05-12T09:32:01.872Z Reads: 19

```
For me that would be perfect :open_mouth: what does that kit include in parts?  
Do you want extra money in exchange? Just 2 Landwheel motors for a full kit sounds too good to be true.
```

---
## \#51 Posted by: visnu777 Posted at: 2019-05-12T09:39:24.667Z Reads: 21

```
It's 2 motors and a special truck needed for this kind of hubs. ![1557653924842110387067629271464|666x500](upload://aQSDaGwW7WQS9uFVhr5NM05dpNO.jpeg) the sleeves are swappable.
The landwheel motors are superior, but these are not bad at all. Lots of torque, 70kv, run with up to 12s and stay reasonably cool. Baseplate include if you need it, although I like the landwheel BP for the cable channel so you should use yours 😊
```

---
## \#52 Posted by: BearBoi Posted at: 2019-05-12T10:44:06.349Z Reads: 21

```
Would definitely work for me :) just need to get the second motor off. Could you send me the 3D print files for the tool you made? I'll ask a friend to print one for me.
```

---
## \#53 Posted by: visnu777 Posted at: 2019-05-12T10:52:39.576Z Reads: 21

```
https://we.tl/t-USypGpcO16

I hope this works, never used that service before :) I printed it in petg. If you take my offer you could leave the hanger, I'd take care of it :)
```

---
## \#54 Posted by: BearBoi Posted at: 2019-05-12T11:42:48.426Z Reads: 20

```
I am planning to take your offer :) and sure, I'll ship the broken hanger with the two motors, and the part that broke loose. Maybe possible to weld back in place with the right tools. I got the .stl file successfully.

Do you think the hub kit you have could work temporarily with the stock landwheel ESC before I buy a new one? (Either way I plan to swap it out eventually)
```

---
## \#55 Posted by: visnu777 Posted at: 2019-05-12T12:15:43.314Z Reads: 18

```
Hmm, don't think so, maybe if you manage to find out how the diye hub sensor wires fit the landwheel sensors but it seems that the lw is picky when it comes to that.
```

---
## \#56 Posted by: visnu777 Posted at: 2019-05-12T12:51:19.550Z Reads: 19

```
My intent is: atm I have two broken lw hubs, one even massacred by me with a drill 😁 with your two I have a chance to do the rewinding (worst case) or I'll even manage to repair the broken one and I have a running set of lw hubs again (best case). The diyeboard hubs are just getting dusty in my shelf, I had no plans for them since I got plenty of alternatives so with you they'll have a more meaningful life 😁
```

---
## \#57 Posted by: BearBoi Posted at: 2019-05-12T13:43:01.802Z Reads: 20

```
You don't have an unused esc/remote laying around that I could buy do you? :D
```

---
## \#58 Posted by: visnu777 Posted at: 2019-05-12T14:24:45.885Z Reads: 18

```
No, I'm afraid not :) but you can get these https://www.ebay.de/itm/FLIPSKY-FSESC-50A-V4-12-ESC-for-Skateboard-RC-Car-Boat-E-bike-E-scooter-Robot-F/264254495474?hash=item3d86cb9af2:g:mPwAAOSwKQFb4Y48 for quite cheap, overall experience here in the forum is really good, I run them even at 12s in FOC mode.
```

---
## \#59 Posted by: pkasanda Posted at: 2019-05-12T23:53:02.594Z Reads: 19

```
Have you ever tried them with Landwheel batteries or only wiht conventional Skateboard batteries?
```

---
## \#60 Posted by: visnu777 Posted at: 2019-05-13T03:53:05.921Z Reads: 16

```
Only with normal batteries. Whatever the lw battery is, when you know the cutoff values you could just put them in the vesc and you're fine. Same goes for maximum battery current and charge.

Edit: I just read about your vesc experience @pkasanda you might have done something wrong. The hubs work flawlessly with two or dual vescs. If you ever want to try again I'd be happy to help you.Even a 4wd like in your case would work with can bus and one remote ;)
```

---
## \#61 Posted by: pkasanda Posted at: 2019-05-13T09:20:31.094Z Reads: 15

```
Yes, I know I did stuff wrong.  This was with the V2 Hubs, not the V4/L3x Hubs.  It worked ok sensorless but the acceleration was like I said similar to a slingshot.  it was impossible to stay on the board.  I attribute that to the high discharge rate of the batteries.  Then I tried running with sensors but I had the wires in the wrong order.  Wheels up the motors were spontaneously reversing.  Then the VESCs stopped working.  Having the wrong sensor wire order alone should not damage a VESC because its comon practice to use trial and error to get the sensor order correct.  So I think the battery discharge rate had something or maybey everything to do with the damage to the VESC.  I believe the sucessfull examples  of Landwheel conversions to VESC have all involved conventional batteries.

You and I particpate in the same private thread of Landwheel VESC conversions so you'll know if I'm incorrect.

I'm just trying to save @BearBoi the heart ache of spending $200 on VESCS and hours of soldering only to have the VESCs pop.

You are correct that the VESC's allow you to set minimum voltage.  However, the landwheel ESC's do something special.  They don't just cut off at a minimum voltage, they throttle down the power well before the minimum voltage.  The discharge rate is so fast on the landwheel batteries that it's easy to overshoot the minimum voltage if you are accelerating hard.  

The  some versions of the V4 ESC had big problems with overshooting the minimum voltage.  You would be accelerating on them and then whack! You would loose power so suddenly that the ESC woudl be left suspended in a single phase of the motors.  The wheels would lock up as a result and the riders would be thrown. The lock up would not happen every time. But even the sudden loss of power was enough to throw some riders.  The L3-X ESC made those problems go away becasue it was sucessful in throtteling the acceleration down to prevent the batteries from discharging so rapidly.

THe five minutes that I had V2 Hubs connected to a VESC and a V4 battery suggested that a VESC does not know how to translate the high discharge rate of the land wheel battereis into usable power.

So I stand by my recommendation that the landwheel batteries only be used with the L3-x ESC. 

I know we are both trying to help.  My experience says don't use the landwheel batteries with VESCs.
```

---
## \#62 Posted by: visnu777 Posted at: 2019-05-13T09:27:52.045Z Reads: 13

```
[quote="pkasanda, post:61, topic:93171"]
They don’t just cut off at a minimum voltage, they throttle down the powerwell before the minimum voltage.
[/quote]
The VESC has two values, cutoff start and end. Cutoff start reduces the power softly, the end is the hard cut off. Its actually similar, you just need the right values. :)
```

---
## \#63 Posted by: pkasanda Posted at: 2019-05-13T09:31:45.678Z Reads: 14

```
Do you have any landwheel batteries to try it with?  I'm not saying that its impossible or that I knew enough to perfect the settings.  I'm saying that its risky. @BearBoi seems to be on a budget. 

On the topic of the Minimum voltage start and minimum voltage end settings -- I never got the chance to deplete the Landwheel battery on a VESC becasue the VESCs popped before I had a chance to go anywhere.

Even if the VESCs did not Pop, I would have needed to strap myself down to the board to stay on it during take off.  I managed to stay on for about 3 feet of Wheely before sliding off the back. The board was totally unsafe and completey unusable.

What VESC settings would you have changed in order to moderate the jack rabit starts?
```

---
## \#64 Posted by: visnu777 Posted at: 2019-05-13T09:51:06.251Z Reads: 15

```
No, I got my Landwheel hubs from a friend without the batteries, just the truck and the battery holder (which I gave him back since he wanted to fit a VESC inside). For a start you can set the VESC to conservative settings, like 30A motor max, -30A motor min, 20A battery max, -10A battery min (actually you should set the value half of what your charger delivers for security). Its also important to setup the remote careful, when you run the assistant you have define the range of the throttle, without it you might get the slingshot effect you described.
```

---
## \#65 Posted by: pkasanda Posted at: 2019-05-13T09:52:52.586Z Reads: 17

```
Thanks.  I'll keep it in mind if I tr again.  I have 6 vescs new vescs to experiment with.
```

---
## \#66 Posted by: visnu777 Posted at: 2019-05-13T09:59:29.064Z Reads: 17

```
I could run them with up to 60A motor max., my mistake was that I left them at that values when I went 12s and that at 60A was too much for them, both shorted at the same time when the enamel coating melted :( But in your case you could use 4wd with 30A per motor and get a smooth beast capable of taking any hill :) The landwheel hubs really rock, they have one of the best free rolling capabilities plus high efficiency and torque. Revel should offer these for DIY to make some extra money ;)
```

---
## \#67 Posted by: BearBoi Posted at: 2019-05-13T10:28:54.583Z Reads: 17

```
All very helpful information. Leaning towards re-using the landwheel batteries with very conservative settings from what you have said. Maybe even trying with 20A on the kit I swap for. Still deciding on what ESC to use though. The one you linked doesn't ship from Germany to Sweden "Kein Versand nach Schweden", other than that it looks great. I could order from Hongkong or China. But would like to ideally have all my parts by the end of the month, also that ups the cost. Found a Maytech ESC in Europe for a decent price. But they seem to have a bad REP on eSk8, and my first impressions of their website was negative.

I'm  thinking my budget for an ESC is around 150 eur, including import fees and shipping. Keeping an eye on the used/new parts category here on eks8 builders, but haven't caught any new posts these past 3 days I have been looking.

The hub tool should be printed tonight if all goes well :) my friend tried yesterday but had some problem with the extruder and will give it a shot again today.
```

---
## \#68 Posted by: visnu777 Posted at: 2019-05-13T10:50:37.332Z Reads: 16

```
If you guarantee me that you'll buy them I'll order the ones from ebay and put it in the box with the motors :)
```

---
## \#69 Posted by: BearBoi Posted at: 2019-05-13T10:54:30.122Z Reads: 18

```
That would be perfect :) PM me your PayPal (or any payment method you'd like) and tell me the total and I will send it in advance.
```

---
## \#70 Posted by: BearBoi Posted at: 2019-05-13T12:10:14.428Z Reads: 19

```
With this I have everything I need to get going, except a remote. Any suggestions there? I know i could get a generic 2.4ghz reciever and remote really cheap. Ideally I would like to reuse the landwheel remote though as I am used to the design and it is high quality. But the antenna reciever and the entire ESC has a full coverage coating on it. I haven't seen anyone reusing it. Any idea if it could be done?
```

---
## \#71 Posted by: SkateboardCave Posted at: 2019-05-13T22:57:02.599Z Reads: 18

```
I understand your problem I think your motor is not able to take the pressure. If you have a guarantee, you can change it.
```

---
## \#72 Posted by: BearBoi Posted at: 2019-05-14T05:22:34.329Z Reads: 14

```
Nah, motors were fine. The trucks could not take the pressure. So the welding broke clean off and made the motor mounts act as propellers and chew up all the cables and have them burn to a crisp :confused:
```

---
## \#73 Posted by: deecept Posted at: 2019-05-26T07:11:44.359Z Reads: 13

```
Hi! Did you figure this out? Would any 2.4ghz receiver work on any 2.4ghz remote? I have an evolve R2 remote, and planning to swap the esc for a VESC 6.6. But can't find any information stating that I can source a reviever and the R2 would connect.. Any help would be greatly appreciated
```

---
## \#74 Posted by: deecept Posted at: 2019-05-26T07:12:39.326Z Reads: 13

```
[quote="BearBoi, post:70, topic:93171"]
I know i could get a generic 2.4ghz reciever and remote really cheap. Ideally I would like to reuse the landwheel remote though as I am used to the design and it is high quality.
[/quote]

I mean this...
```

---
## \#75 Posted by: KaramQ Posted at: 2019-05-26T07:12:44.834Z Reads: 14

```
Its not possible
```

---
## \#76 Posted by: BearBoi Posted at: 2019-05-26T07:47:16.649Z Reads: 14

```
No. I'm getting replacement parts for the Landwheel though, so I will be keeping the regular remote for a while
```

---
## \#77 Posted by: deecept Posted at: 2019-05-26T18:19:11.982Z Reads: 13

```
So my only option is any remote with a reciever that is shipped with it? Such a shame.. the R2 works really well. Sorry to hijack AND revive an old thread, friends :slight_smile:
```

---
