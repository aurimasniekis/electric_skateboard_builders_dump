# How you burn up ur esc or motor going slowly and despite seeing few amps from the battery

### Replies: 46 Views: 4721

## \#1 Posted by: Hummie Posted at: 2016-05-30T15:04:16.126Z Reads: 264

```
I got this from Rew on Vedder's forum.    I always wondered what volts were doing in a motor....turning into amps

"Say the example of my friends.... They had a motor doing 50V, 10k RPM. at 200A. 10kW. When they run it at 2500RPM, the motor effectively sees only 12.5V, and assuming the 200A max still holds, the maximum power is only 2.5kW. If the battery is still 50V, the motor fries after a while at 50A battery current (200A through the motor). And the motor will tolerate 300A for a while, but you blow up the 300A ESC after a few seconds of 75A battery current. "
```

---
## \#2 Posted by: Namasaki Posted at: 2016-05-30T17:41:18.276Z Reads: 248

```
So, what your saying is that less throttle is less voltage and more throttle is more voltage to the motor, not amps?
If thats true, then we need a gear ratio that allows us to run at full throttle most of the time.
And, assuming that neither voltage or amperage are constant, and the throttle determines the esc's output voltage,
what determines the 3 phase amp draw, load on the motor?
I have a clamp volt/current meter. I'm gonna do some testing on the 3 phase side of the Esc and get back later with my findings.
```

---
## \#3 Posted by: Hummie Posted at: 2016-05-30T18:17:22.024Z Reads: 238

```
I'd like to know what u find on that side of the esc and look forward to reading what you find. Does ur meter record?  It would be good to get a recording of the results under load. Supposedly lots of spikes and a large difference from what goes in. 
The basic thing I'm finding which seems to be widely misunderstood is that increasing your battery voltage doesn't mean you will run the motor or the esc cooler.  You will have a higher top speed, have the ability to kick amps to the motor really quickly.  These are the benefits.  But when it comes to efficiency the closer you are running to the max speed of the motor (volts x kv)  the better.  Efficiency means cooler.  Cooler means greater continuous power
```

---
## \#4 Posted by: Namasaki Posted at: 2016-05-30T18:20:54.836Z Reads: 221

```
This is exactly what onloop has been saying all along. gear ratio and voltage so that full throttle=cruising speed.
This can be difficult to achieve because sometimes I like to go 25-28 mph but not always.
I will do some testing and try to post my findings later today or this evening.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-05-31T06:01:38.492Z Reads: 202

```
Ok, ran some tests using my clamp meter to read voltage and current on the 3 phase going from the Esc to the motor.
What I discovered is that the throttle does indeed control the amount of voltage that goes from the Esc to the motor.
More throttle=more voltage Less throttle = less voltage
With no load on the motor, the current draw form Esc to motor stays mostly constant regardless of the amount of voltage fed to the motor.
I ran these tests with 6s and 12s.
To my surprise, the no load current from Esc to motor was slightly higher with 12s.
1.3 amps at 6s
1.7 amps at 12s
There were momentary spikes in current during rapid acceleration.
And the current did increase substantially as I applied load by squeezing the wheel with my hand.
It did also seem that I was able to ramp up the current more when testing with 12s than with 6s.
Afterwards I went out for a road test, 12s vs 6s.
Climbing the same 10% grade
6s at full throttle went up the hill without slowing down
12s at maybe ½ throttle went up the hill with power to spare( 12s could have gone up faster but I was trying to keep same speed)
Checking the temp of the Esc heat sink, the 12s run made it warmer than the 6s run.
Also to my surprise while going down the hill, the brakes seemed more effective and controllable with 6s
I decided to run the road test again with an inline meter between the battery and dual Esc's. The results are as follows:
6s:
Esc's heat sink temps 84deg
Peak Amp draw from battery  37.38
Peak watts 863
Watt-hour use 1.9

12s:
Esc's heat sink temp: 94deg
Peak amp draw from battery 18.4
Peak watts 898
Watt-hour use 2.1
All road tests where performed with dual TB 12s Esc's and dual TB 6355/230kv motors 16/36 gears and 90mm wheels
After running these tests, I'm not so sure that 12s is such a good idea even with dual motors. Although higher voltage = less amps on the battery side of the Esc, it's appears to be a different story on the motor side.
I was not able to test current on the 3 phase during road tests but it did seem evident during bench tests that more voltage = more current, not less. Guess thats the difference between DC current and 3 phase AC current.
This could very well be the source of our problems with overheating Esc's
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-05-31T06:37:48.508Z Reads: 171

```
Double the amp draw on the 6s vs 12s

And this is how you spend your holiday? Lol hope you had a great one mate!
```

---
## \#7 Posted by: Namasaki Posted at: 2016-05-31T06:55:51.391Z Reads: 174

```
Double amp draw from the battery with 6s but I'm not so sure about the amp draw from the esc to the motor. 
I need to extend one of the 3 phase wires so I can measure the amperes while riding to get  a real comparison.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-05-31T06:59:28.435Z Reads: 169

```
Searching for answers to life's mysteries, 
For example: Why do my Esc's get hot?
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-05-31T07:00:20.093Z Reads: 167

```
This is excellent...This is the start of finding a good standard for what Voltage, ESC and Motor combo would be most ideal under various riding conditions.

I think you are on to something
```

---
## \#10 Posted by: Namasaki Posted at: 2016-05-31T07:16:46.090Z Reads: 163

```
Now that I know for a fact that the Esc regulates the amount of voltage to the motor. I think that we have the right battery voltage when we can go full throttle confidently. I have not been able to do that with 12s.
With my setup I should be running 8s or 10s
Seems like handing the Esc 50 volts and then only allowing it to pass 20-30 volts on to the motor causes it to overheat.  This is a whole new train of thought for me.
I've got some 14t motor pulleys coming tomorrow. I'm gonna swap out my 16t with them so I can feed more voltage to the motors and spin them faster to create more hp without having to go faster. During my bench test it seemed that the faster the motors turned, the more load I had to put on them to make the amps go up. 
Because the motor spinning faster does not increase amp draw. Only applying load does.
```

---
## \#11 Posted by: Hummie Posted at: 2016-05-31T07:25:54.263Z Reads: 167

```
U have so much info it's easier for me to do this:



Ok, ran some tests using my clamp meter to read voltage and current on the 3 phase going from the Esc to the motor.
What I discovered is that the throttle does indeed control the amount of voltage that goes from the Esc to the motor.
More throttle=more voltage Less throttle = less voltage
**if u hold the throttle till the motor fully spins up does the voltsge reading go down or stay the same?**
With no load on the motor, the current draw form Esc to motor stays mostly constant regardless of the amount of voltage fed to the motor.
I ran these tests with 6s and 12s.
To my surprise, the no load current from Esc to motor was slightly higher with 12s.**think that's normal as its a higher speed with the 12s right?**
1.3 amps at 6s
1.7 amps at 12s

There were momentary spikes in current during rapid acceleration. 
And the current did increase substantially as I applied load by squeezing the wheel with my hand.
It did also seem that I was able to ramp up the current more when testing with 12s than with 6s.
Afterwards I went out for a road test, 12s vs 6s.
Climbing the same 10% grade
6s at full throttle went up the hill without slowing down
12s at maybe ½ throttle went up the hill with power to spare( 12s could have gone up faster but I was trying to keep same speed)**great test isolating the voltage**
Checking the temp of the Esc heat sink, the 12s run made it warmer than the 6s run.**which test first? Maybe leftover heat?  Actually this makes sense as esc work less on full throttle**
Also to my surprise while going down the hill, the brakes seemed more effective and controllable with 6s **setting could change this right?**
I decided to run the road test again with an inline meter between the battery and dual Esc's. The results are as follows:
6s:
Esc's heat sink temps 84deg
Peak Amp draw from battery 37.38
Peak watts 863
Watt-hour use 1.9

12s:
Esc's heat sink temp: 94deg
Peak amp draw from battery 18.4
Peak watts 898
Watt-hour use 2.1
It **it makes sense that the 12s would use a bit more watt hours as it's riding at a much lower percent of the no-load**
All road tests where performed with dual TB 12s Esc's and dual TB 6355/230kv motors 16/36 gears and 90mm wheels
After running these tests, I'm not so sure that 12s is such a good idea even with dual motors. Although higher voltage = less amps on the battery side of the Esc, it's appears to be a different story on the motor side.  **.  **its the trade off giving up low speed efficiency for the possible high speed and quick power.  it's worth it to me.  Nice to see its not that inefficient considering how much higher the no-load is with the 12s than 6s. I'll gladly give up a bit of range for the much greater top speed.**     ** 
I was not able to test current on the 3 phase during road tests but it did seem evident during bench tests that more voltage = more current, not less. Guess thats the difference between DC current and 3 phase AC current.
This could very well be the source of our problems with overheating Esc's

**The greater watt hours to get up the hill was pretty insignificant on 12s and the esc heating is likely the fact it's being held to half throttle**
```

---
## \#12 Posted by: Namasaki Posted at: 2016-05-31T07:26:45.571Z Reads: 146

```
LoL I gotta get up in 4 hrs and go to work. 
I better pull the plug now.
```

---
## \#13 Posted by: Hummie Posted at: 2016-05-31T14:15:53.225Z Reads: 146

```
Damn that was hard to highlight. 

Looking forward to to the testing of the phases under load 

To me your results show 12s being ridden even way below its no-load Max rpm is not much more inefficient.   

Maybe you could add more:

The same test with motor temps as well.



the same hill but without limiting your speed on 12s.

Im pretty sure escs run cooler at full speed surprisingly. If u went up the hill using half throttle with the 6s it might be a similar high temp.

FOC esc temp vs bldc 




Great stuff!  Thanks
```

---
## \#14 Posted by: elkick Posted at: 2016-05-31T15:21:02.258Z Reads: 140

```
Typically standard RC ESC's are using duty cycle or voltage control, where the VESC is using current control. 

So the results with the VESC could be different.
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-05-31T16:33:16.705Z Reads: 137

```
would this explain why running those 190kvs at 12S unloaded on my bench gets the motors so damn hot but hauling ass down the trail doesn't get them quite so hot? I'm going purely based on touch, i still need to invest in an IR thermometer, but the fact that i can keep my hand on them probably means they're fine. 

also one easy way to get your VESC to drive your board at grandma's bicycle speed is to limit your current to something low, it will accellerate slowly and the top end will be slower.  

and NOT limiting your current to something reasonable is a great way to make a board almost unridable do to the never ending accelleration issue, but that's also tied into proper throttle signal tuning as well. 

I prefer my boards to have a smooth and predictable acceleration curve as well as the same for braking, and in my experience this means tweaking the current limiting for each board's battery and motor configuration. ITs possible to have some crazy top end without launching into a tree the minute you stand on the damn thing, and its possible to have it set up to where you can easily cruise at half throttle and have that be your fun/cruise speed and still have plenty of throttle left so you can floor it and harass the cyclists by getting into the low 30's mph wise.
```

---
## \#16 Posted by: Hummie Posted at: 2016-05-31T16:49:30.249Z Reads: 132

```
Weird they'd get hot on the bench.  There should barely be any amp draw on the bench regardless of the voltage.  The amp draw should be a bit more with no-load at 12s but still as namasaki showed its not much.  


For some reason whenever I try to do a no-load test using the vesc on the pc by choosing an rpm on the right side of the screen it spins quickly and then stops. Maybe try duty cycle or something? 

Namasaki how'd you get such detailed no-load amperage?

I run 12s with 90kv and amps set to 60 on FOC.  It's great but there's the overheating risk but it's worth it
```

---
## \#17 Posted by: Namasaki Posted at: 2016-05-31T22:55:33.452Z Reads: 125

```
[quote="Hummie, post:11, topic:4008"]
if u hold the throttle till the motor fully spins up does the voltsge reading go down or stay the same?
[/quote]

When I held the throttle steady the voltage remained the same.
```

---
## \#18 Posted by: Namasaki Posted at: 2016-05-31T22:57:45.038Z Reads: 123

```
[quote="Hummie, post:11, topic:4008"]
think that's normal as its a higher speed with the 12s right?
[/quote]


Both 6s and 12s 3 phase amperage  bench tests where conducted at full throttle.
But remember that the current stayed constant regardless of the amount of throttle or Rpm
it only spiked momentarily if throttle was increased quickly. Once the rpm leveled out, the voltage returned to the constant.
```

---
## \#19 Posted by: Namasaki Posted at: 2016-05-31T23:02:37.212Z Reads: 120

```
[quote="Hummie, post:11, topic:4008"]
it makes sense that the 12s would use a bit more watt hours as it's riding at a much lower percent of the no-load
[/quote]


not sure what you mean by this. But these values where obtained during the road test going uphill.
```

---
## \#20 Posted by: Namasaki Posted at: 2016-05-31T23:09:45.056Z Reads: 119

```
[quote="Hummie, post:11, topic:4008"]
The greater watt hours to get up the hill was pretty insignificant on 12s and the esc heating is likely the fact it's being held to half throttle
[/quote]


I'm thinking as well that the extra heat is possibly due to the Esc having to hold voltage back at less than full throttle.
```

---
## \#21 Posted by: Mobutusan Posted at: 2016-06-01T02:05:42.982Z Reads: 114

```
@Namasaki Great work on this. I wonder if the batteries c-rating can possibly have an effect on the heat. Maybe it's harder to control and hold back the power?
```

---
## \#22 Posted by: Namasaki Posted at: 2016-06-01T04:15:47.874Z Reads: 111

```
Hey Shawn, forget what I said before about motor timing and accelerating settings. Those settings where with my hub motors.
I just ran a road test with belt drive 6355's  set at high timing and high acceleration with 12s voltage going up some decent hills and keeping my speed below 16mph. when I was finished, I checked my Esc's and motors and the Esc's where barely warm( only 10 deg more than when I started) and the motors where not even warm.
So Those settings are not the problem. Something else is causing your overheating problems.
On a side note, my brakes where working poorly with normal motor timing and medium acceleration. To be specific, I was coasting downhill and picking up speed and tried to apply a little brake but the brakes would not respond until I had pushed the trigger out farther than normal and then they grabbed suddenly. I noticed that they worked much better with 6s voltage. Anyway, I changed my motor timing to high and acceleration to high and the brakes showed some improvement.
```

---
## \#23 Posted by: Mobutusan Posted at: 2016-06-01T04:53:29.041Z Reads: 109

```
Interesting. You're esc's are mounted out in the open air, right? Would you mind taping some temporary enclosure over your esc's and repeating your test to see if there is any noticeable difference in temps? And I was just thinking, what if the fact that I'm using only one esc is causing it to heat up more? Maybe I just need to run dual to keep each unit's current in check?
```

---
## \#24 Posted by: claudiofiore88 Posted at: 2016-06-01T05:06:35.693Z Reads: 99

```
2 posts were split to a new topic: [Why does my motor cut out for a split sec](/t/why-does-my-motor-cut-out-for-a-split-sec/4092)
```

---
## \#25 Posted by: Namasaki Posted at: 2016-06-01T05:16:51.667Z Reads: 99

```
Your right, running single power and climbing hills. Your gonna get more heat than you would with a dual setup.
I experienced this one day when I was out on a ride and one of my esc's burned up and I had to disconnect it and ride back with one motor/esc. going uphill. when I got back to my car that one esc was way hotter than before.
It's simple, when you run dual, your cutting the load on each motor and esc in half. you could take your esc out of the box and mount it to the deck with a few screws and see if that helps. I honestly don't think it will solve your problem completely. Frankly, I would invest in either TB's 6355 E-board motors or Enertion's R-spec 6355 motors. 
Okay, so there not as cheap as the Hobby King motors. But I believe that you get what you pay for. There motors are specifically designed for E-boards. HK's motors are not. And though with some modification,  they may work, but how well? and for how long? So I'm thinking that your problem might just be the motors your using and using and the single drive setup. You wouldn't happen to live in So. California ?
```

---
## \#26 Posted by: Hummie Posted at: 2016-06-01T05:27:00.218Z Reads: 99

```
disection of the rspec vs Hobbyking stuff has been done a couple of times here. It's a good motor for a board and so are many at Hobbyking.
```

---
## \#28 Posted by: Namasaki Posted at: 2016-06-01T05:43:53.295Z Reads: 98

```
I understand that there are different opinions about these motor options.
I haven't tried any of the hobby king motors so I can't say for sure about them but I have used TB's motors and I run them very hard up a lot of long hills and they never get hot or cause my Esc's to get hot.
I just can't help but believe that motors specifically designed for e-boards have got to be the best option.
But that's just my opinion.
```

---
## \#29 Posted by: Mobutusan Posted at: 2016-06-01T06:38:58.621Z Reads: 95

```
Sorry, I'm up in northern California. Otherwise, I'd love to go ride and do some testing. Btw, what equipment are you using to get these readings? I'm thinking of getting some kind of meter to monitor these things.

I'm gonna try dual hub motors soon, but in the meantime, I might also try running my two 245kv motors together, staggered on one truck, or even try a dual uneven setup with a 260kv SK3 I just picked up. Just to make things even more interesting. 

One more thing for when you're out testing, can you test the effect of limiting throttle to like 80% or something? Maybe limiting your top speed to something more reasonable will allow you to use "full" throttle, and maybe yield interesting results?
```

---
## \#30 Posted by: Mobutusan Posted at: 2016-06-01T07:06:09.869Z Reads: 88

```
And since you're in test mode, do you happen to have different kv motors that you could test and compare?
```

---
## \#31 Posted by: Namasaki Posted at: 2016-06-01T07:21:50.943Z Reads: 89

```
[quote="Mobutusan, post:29, topic:4008"]
One more thing for when you're out testing, can you test the effect of limiting throttle to like 80% or something? Maybe limiting your top speed to something more reasonable will allow you to use "full" throttle, and maybe yield interesting results?
[/quote]

My first Diy setup was dual hub motors with TB 12s Esc's and 12s Lipo. 
I wanted to ease into it so I started at 40% power.
I stayed there for a while. Top speed with the Carvons on that setting was still 20+ mph
You shoul try that and see if it reduces heat. 
I also tried 60, 80 and finally 100%
There was a substantial jump in power from 40 to 60
Not so much difference going from 60 to 80 or 80 to 100
You should try it at 40 and see. 
I'm not sure if that setting limits current or voltage. 
My guess is gonna be voltage because turning it down feels like your running lower voltage.
```

---
## \#32 Posted by: Namasaki Posted at: 2016-06-01T07:24:04.465Z Reads: 84

```
[quote="Mobutusan, post:30, topic:4008, full:true"]
And since you're in test mode, do you happen to have different kv motors that you could test and compare?
[/quote]
I only have the 2 TB 230kv motors
```

---
## \#33 Posted by: Mobutusan Posted at: 2016-06-01T07:29:27.197Z Reads: 82

```
I'm gonna add that to my "to try" list. From your testing results so far, I'd also guess it would reduce the voltage.
```

---
## \#34 Posted by: torqueboards Posted at: 2016-06-03T05:02:41.486Z Reads: 80

```
I'm not no EE but from my experience what overheats the motor is the stress in terrain and/or over throttling and the energy/power has no where to go. That's the quickest way to overheat it. Especially, when running at 12S this is more of an issue versus running at 6S.

Ex. Your board can't move forward but you throttle too hard and drive more power to the motors but it can't go anywhere. That power/energy has to go somewhere (supposedly?)

Maybe someone with more exp in "electronics" might know a bit more.

I had a dual 6S on 5065 280KV and man that thing was quick and didn't overheat much if any. I'd say it's about 70-80% up to a 12S dual setup. It just wouldn't climb as steep of a hill as many times due to being a smaller motor it would get hot "quicker" than a 63mm motor.
```

---
## \#35 Posted by: Hummie Posted at: 2016-06-03T05:13:37.364Z Reads: 82

```
The more I read about 12s vs 6s it's almost the same and the only real difference (assuming they're geared optimally) is on 6s unless you're running high c batteries they will possibly suffer voltage sag as more amps are used with 6s.  A lot of the attraction of high voltsge is a hold-over from when there wasn't such high c rated batteries available.  Now that there are high c batteries there's no reason not to run 6s other than the batteries are more expensive. 
Hopefully I can run a 6s on 200kv and 12s on 90kv test tomorrow.  The motors will likely run very similar temps but maybe the escs will run cooler or hotter. But I hear it can go either way and higher voltsge isn't necessarily more efficient there either

Have you done a comparison ?

But as u say the real inefficiency is too much load for the motor.  Too steep really..or you could say too fat
```

---
## \#36 Posted by: torqueboards Posted at: 2016-06-03T05:19:42.752Z Reads: 83

```
@Hummie that and/or someone goes up a hill and slows the momentum. Then your trying to start from almost a stop in the middle of the hill. That can cause a lot of load/heat too.

I've done a slight comparison but I didn't notice a whole lot of difference. Although, I wasn't testing for amp rating and more so just riding results. 6S, you just need higher KV and a dual/second motor helps.
```

---
## \#37 Posted by: Mobutusan Posted at: 2016-06-03T05:26:30.984Z Reads: 79

```
It seems like dual drive is the way to go to limit amp draw and keep things cooler. I'm gonna have to try that too.
```

---
## \#38 Posted by: torqueboards Posted at: 2016-06-03T05:33:01.101Z Reads: 79

```
If your not climbing any hills though you shouldn't need it at all. Dual motor IMO is only really needed for hills unless you want more traction.
```

---
## \#39 Posted by: Hummie Posted at: 2016-06-03T05:47:59.213Z Reads: 83

```
As you say when you try to get up a hill from a standstill it's the worst.  Riding at as close to top speed is the most efficient and adding a load onto a really slow speed is the worst.   

It's been proven that different voltage systems perform just as efficiently if they're optimized (gears and kv ) but the controllers will perform differently depending on what...bits..they have inside. I'd like to know what the vesc is best at

Even the assumption, which I had, that with a lower voltage set up you won't get quite the kick isn't true.  As long as your batteries can take the amp draw and the esc is suited to the amp draw it's just as good
```

---
## \#40 Posted by: Mobutusan Posted at: 2016-06-03T06:50:59.582Z Reads: 84

```
Do you ever run single drive?
```

---
## \#41 Posted by: torqueboards Posted at: 2016-06-03T06:59:57.511Z Reads: 88

```
[quote="Mobutusan, post:40, topic:4008, full:true"]
Do you ever run single drive?
[/quote]

Yeah, once in a while for testing but I like dual personally. I know some people who enjoy single though.

My single doesn't overheat though. Unless, I try and go up too many crazy hills.

I've even had a friend and we were riding for about an hour and he was fine until I told him let's burn his motor out.

That was climbing about 5-6 steep hills. I think he burned it out though because he lost momentum up a hill. He was a heavier rider and I was surprised his single motor handled what it handled lol. I was riding with my dual setup so mine doesn't get nearly as hot.
```

---
## \#42 Posted by: Mobutusan Posted at: 2016-06-03T07:14:57.824Z Reads: 80

```
@torqueboards What voltage and gearing did you run on single drive? Was this on your 230kv motor? I'm gonna try dual drive soon, and dual hubs, but I really want to sort out my single drive issues first.
```

---
## \#43 Posted by: Mobutusan Posted at: 2016-06-03T07:46:21.881Z Reads: 82

```
And that's interesting that you burned up the motor doing this. My motor isn't going past 110-120°F in the windings, but the esc heatsink is hitting 170-180°F+, all on about 1-2 easy miles. So, if there's excessive resistance or amperage, it seems to be mostly confined to the esc.
```

---
## \#44 Posted by: Okami Posted at: 2016-07-16T07:37:55.219Z Reads: 70

```
Hello everyone! A topic about what is the real amp draw / current needs for a system surfaced on another topic.

 It may not be exactly what this topic is about, but I thought it is related, so someone in the future reading this, might find it interesting. 

----
So, gladly @DeathCookies made a simple template for everyone to enter their data into.

Any feedback / improvements would be great, as I think it is still possible to be changed and should be improved.

Poll for entering Amp draw data:
---
http://gct-hp.de/esk8/index.php
---
<img src="/uploads/db1493/original/2X/f/fb9d17765e8c0f3c9a2a0781eb7ac01a3b2ccbe9.png" width="300" height="300">

----

Feedback can be posted here: 
http://www.electric-skateboard.builders/t/custom-poll/6171
----

if you see ''1'' after the index.php in the link, delete that ''1'' and it should go. Link should look like this: 
---
http://gct-hp.de/esk8/index.php
---

 Dunno why that happens

---
Original discussion / idea about creating such thread started here:
http://www.electric-skateboard.builders/t/sanyo-ncr-18650ga/6140/24?source_topic_id=3116
```

---
## \#45 Posted by: lox897 Posted at: 2016-07-16T08:08:23.411Z Reads: 65

```
Link to the poll doesn't work for me.

EDIT: It works now.
```

---
## \#46 Posted by: Mikenopolis Posted at: 2016-08-29T18:41:20.848Z Reads: 52

```
How does Boosted do what they do with their different speed modes?

I'm new to this hobby and I'm not yet comfortable going full speed (28mph?) 20-22 is roughly where I chicken out and slow back down. I would love to be able to max my speed to let's say 20 with a button and at the same time not fry anything
```

---
## \#47 Posted by: Jinra Posted at: 2016-08-29T19:02:18.525Z Reads: 53

```
Easiest thing to do is just limit it by feel. Only throttle when you want to go faster, otherwise just coast.
```

---
