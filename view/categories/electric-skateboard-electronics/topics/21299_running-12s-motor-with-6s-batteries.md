# Running 12s motor with 6s batteries

### Replies: 38 Views: 2185

## \#1 Posted by: Pafrican Posted at: 2017-04-18T14:37:14.347Z Reads: 160

```
Hey. I'm new to all of this but I've done tons of reading and already bought the components I need, specifically:
- Turnigy Aerodrove SK3 - 6374 149 kv Brushless Outrunner Motor (12s)
- 2 Turnigy Multistar 6s 8000 mAh Lipo Batteries
- VESC 
- FS GT2B 2.4GHz Transmitter/Receiver 
- 14:27 ratio

According to several online calculators I should be getting a weighted top speed of roughly 20mph.

I'm wondering if it's possible to run the motor at 6s.. that way I can link my batteries in parallel instead and double my range. 
It seems like I can configure my VESC (via the BLDC tool) to limit the voltage and current input to the motor. I would configure it to simulate a 6s setup. Is this possible? Will this harm the motor or the VESC? 
I realize my motor will be going half as fast, but cruising at 10mph is fine with me.

Thanks!
```

---
## \#2 Posted by: Maxid Posted at: 2017-04-18T14:48:27.325Z Reads: 150

```
parallel will not double your range.
Energy inside your pack will stay the same.
Actually in series you might see higher range because the efficiency is better at higher voltages.
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2017-04-18T16:32:24.834Z Reads: 140

```
Say what now?
Doubling your capacity and keeping your max speed the same doesn't give you double range?
Paint my fart green while you're at it.

Going faster increases the energy used / kilometer and if you were to travel at 50% speed with the 12S you are operating on the worst possible duty cycle if you're going for efficiency, AKA 50% duty cycle.

@Pafrican I have a very similiar setup to you voltage, motor and gear ratio wise with 6S, SK3 149KV and 15:30 ratio and my board cruises at 100% duty cycle at ~15 mph on flat with 80 mm diameter wheels. Here's some pics in case you're interested http://imgur.com/a/Mjodj
```

---
## \#4 Posted by: Maxid Posted at: 2017-04-18T16:35:52.562Z Reads: 129

```
doubling your capacity will only increase your range if you add another pack in parallel instead of halving your voltage.
It is all about energy in your pack.

20V*10Ah=200Wh which is the same as 10V*20Ah=200Wh
so you don't magically get double the range just because you rewire your batteries (which he was suggesting).

Plus higher current draw at lower voltages will decrease efficiency as higher current generates more heat. Higher voltage is always favorable in terms of efficiency.
```

---
## \#5 Posted by: SimosMCmuffin Posted at: 2017-04-18T16:51:50.156Z Reads: 121

```
I'll agree in the case that he also limits his speed to the same maximum as with the 6S setup.

And here's my point on the efficiency with the VESC at 50% duty cycle, which you would have to do if you want to run the motor at 6S speeds with 12S battery. You get much more heat dissipation in the capacitors, because of the large ripple current, which is at it's maximum at 50% duty
https://youtu.be/x6lPdI9OVQg?t=23m9s
```

---
## \#6 Posted by: Mathias Posted at: 2017-04-18T17:07:50.691Z Reads: 113

```
Do you really think the ripple current are the main factor here? I'm not so sure. The power loss in the FETs is proportional to the current, not to the total power. By going for 12s instead of 6s will cut your resistive loss per output power in half for basically any component of your electronics. Also it will be much better for the LiPos to drain only half the current. This will increase their lifetime and reduce the voltage sag. I don't see any advantage in staying under the maximum voltage that your esc can do. 

The old story: half the voltage, double the current is just as good is only true in context of motor windings/KV. Lower voltage is worse for any other electrical components of your system. Or am I missing something here?
```

---
## \#7 Posted by: Maxid Posted at: 2017-04-18T17:13:43.311Z Reads: 111

```
You are nitpicking. He never said he actually WANTS to lower his speed. He just said that he wants to rewire because he would get double the range - that is wrong and what you should be correcting. 

I simply said that the energy will stay the same and rewiring will not make a difference. 

If you start making assumptions to calculate the exact effects the rewiring has on his range you would need a lot more data. We are simplifying here and in this case higher voltage is more favorable than higher current (plus having the ability to choose higher speeds)
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2017-04-18T17:18:32.852Z Reads: 108

```
The LiPos also drain at half the current each when parallel, because your capacity is doubled and each of them is supplying half the current. The resistive losses in the FETs is dependent on the battery & motor current, with less than 100% duty causing extra losses in the lower FETs.

I guess the best thing would be say to the OP @Pafrican , if you're really not sure then try each configuration and if you're not getting the range you want, go slower. And in the end, it maybe just easier  to wire for the 12S.
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2017-04-18T17:22:57.630Z Reads: 106

```
And the point I was trying to make (rather poorly I guess) that speed impacts range more than anything else. if he were to go **full speed** with the 12S and 6S, the 6S would go double the range. And I actually did some practical tests to test the effect of the traveling speed on your energy consumption / distance. Link to the thread.

https://www.electric-skateboard.builders/t/speed-vs-range-practical-test-results/21015

The 6S just would just limit his max speed lower, so he would get more range out of the pack without feathering the throttle with 12S to travel the same speed. I mean it's just hard to go slower than what the board can do right :smile:
```

---
## \#10 Posted by: Maxid Posted at: 2017-04-18T17:26:25.338Z Reads: 98

```
You actually think he will see a difference in range? The effects will be so small that wind and temperature differences between the days would have larger effects. 

On the level you are taking this to you would also have to check his solder joints and cable thickness for weak spots. What about his anti spark or loop key - they will heat up with more current going through. What about his fuse? Will he need a new and bigger one at his "new" current levels? 
Just stop overcomplicating this!

Edit: just read your new post about higher speeds. Sure wind resistance at higher speeds will eat his battery. But what if he only rides with tail wind? ;)
```

---
## \#11 Posted by: jadatmag Posted at: 2017-04-18T17:28:31.878Z Reads: 92

```
Going half the speed actually decreases your range in most scenerio's.

Air resistance isn't that important at normal e-board speeds and these motors normally gain efficiency near top speed.

Cars do suffer from air resistance and are the most efficient arround 80 km/h. Without air resistance the most efficient speed would be near topspeed. Just like E-boards.
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2017-04-18T17:30:40.989Z Reads: 89

```
And both ways I guess :blush:
```

---
## \#13 Posted by: Maxid Posted at: 2017-04-18T17:31:01.811Z Reads: 87

```
With some people on this forum going for 50-60kmh what are normal eboard speeds to you? Above 30kmh the wind resistance will have an effect
```

---
## \#14 Posted by: SimosMCmuffin Posted at: 2017-04-18T17:33:41.710Z Reads: 85

```
I'll refer to my thread on the effect of speed on energy consumption / distance
https://www.electric-skateboard.builders/t/speed-vs-range-practical-test-results/21015

Also cars are most efficient at a certain motor RPM. As you increase speed your aerodynamic drag increases exponentially as a factor of speed. Cars are just optimized for highway travel at 80 km/h with their gears, so the motor is closest to it's optimum RPM.
```

---
## \#15 Posted by: jadatmag Posted at: 2017-04-18T17:37:54.567Z Reads: 76

```
About 10-22 mph (16-35 km/h) is normal I guess.

The gears of the car tuned for highway speed is a valid point though.

I am still right though :D You will lose range by going half the topspeed on the same motor/battery setup on an e-bourd that doesn't go too fast.

Can't technically back this up though, do we have a captain over here?
```

---
## \#16 Posted by: SimosMCmuffin Posted at: 2017-04-18T17:38:20.850Z Reads: 71

```
It's pretty linear from what I concluded from my own tests with a limited amount of different travel speeds, as I only had 2. but the Wh/km increases very linearly with the travel speed, for example, if you're using 8 Wh/km at 15 km/h then you would be using about 16 Wh/km at 30 km/h. Why is the Wh/km number linear and not exponential? Well when doubling your speed you quadruple the average power needed to travel due to aero drag, but you're also spending only half of the time doing a kilometer for example and that's where the linearity comes from.
```

---
## \#17 Posted by: jadatmag Posted at: 2017-04-18T17:42:19.568Z Reads: 64

```
Reading your thread you seem to be quite the captain yourself.

So I might be wrong here
```

---
## \#18 Posted by: SimosMCmuffin Posted at: 2017-04-18T17:42:55.764Z Reads: 64

```
My practical test proves the opposite... WITH PROOF!

And what you mean with "an e-board that doesn't go too fast"? The aerodynamic drag is always present at low speeds as it is at high speeds.

EDIT: Ok, you read the thread. Thank you. I just thought it was an interesting experiment with useful results to share with the community.
```

---
## \#19 Posted by: Maxid Posted at: 2017-04-18T17:43:44.520Z Reads: 65

```
Without looking at your data (I am on mobile right now): I just doubt that you could actually maintain all conditions the same when doing your tests. You did not ride on a treadmill in a temperature controlled room so all "effects" that you observed in your limited data set might come from something else. I agree that higher speeds will need more energy - but as to what degree and if the dependency is actually linear I have no idea.

But this is all offtopic anyway.
The main point was if he will double the range if he rewires and the answer to that is no.
```

---
## \#20 Posted by: SimosMCmuffin Posted at: 2017-04-18T17:47:14.940Z Reads: 65

```
I have also stated how my tests were performed. I use a quiet road, where there is no need to slow down unnecessarily.  The route is also a forth-and-back route, so it averages the terrain to flat plane and what ever head- or tailwind I had traveling to my turning point, becomes the opposite on the way back. And the results were very even across all runs.
```

---
## \#21 Posted by: Hummie Posted at: 2017-04-18T18:05:43.759Z Reads: 62

```
@ simosmcmuffin this is a long video about the vesc6, what does it say will be the efficiency of running at something like 12s and 15mph vs 6s and 15mph (same setup otherwise)?  so the test being running at half duty cycle vs 100%.
```

---
## \#22 Posted by: SimosMCmuffin Posted at: 2017-04-18T18:26:14.646Z Reads: 60

```
Point was to show how much losses the VESC can experience with high motor currents at 50% and 100% duty as Vedder shows in a few minutes of the timestamp I shared the video with. And I think the blanket statement that running the VESC with higher voltages is more efficient by default is not necessarily true.

Granted, the total average power at 15 mph are not that big, with my tests having about 260 Watts continuous, now even with 6S, it would be just a bit over 11 battery amps. But my point still stands that the VESC is much less efficient at 50% duty as Vedder also states and calculates.

And as for the OP's range needs, just like you @Hummie have said and I quote: "whenever I see an opportunity to push the finger to the metal I do it", so  he might end up traveling a lot faster on the 12S and ending up with less range therefore.
```

---
## \#23 Posted by: Hummie Posted at: 2017-04-18T19:32:27.847Z Reads: 63

```
Thanks. Its just the esc that losses efficiency at lower duty cycle and not the motor right?  I guess I could watch the movie and probably will but can u explain how the duty cycle and frequency are related on the current control program and foc? I read the frequency changes. 
What frequency range is it?

I'm mainly wondering about the frequency as I believe at higher frequencies a ferromagnetic material will become magnetized and be reversing polarity quickly and a hysterisis occurs and ..poof an induction heater.  
The frequency produced by the esc and the current put out by it will be smoothed by the inductance of the motor as it takes time for the magnetic field to build so i think the motor is only exposed to this slower "commutation" frequency regardless of esc frequency and no torque ripple or hysterisis.
```

---
## \#24 Posted by: SimosMCmuffin Posted at: 2017-04-18T20:11:19.010Z Reads: 60

```
Can't say about the variable frequency's effect on efficiency as my current controller is a static frequency at 24 kHz if I remember correctly and the upcoming InstaSPIN controller will also be static frequency.

In my understanding variable frequency drive is more for induction motors and I'm not exactly sure what benefits it brings to the BLDC motors... 

The following code snippet is from the VESC's bldc-master repo, from mcpwm.h file

    #define MCPWM_SWITCH_FREQUENCY_MIN		3000	// The lowest switching frequency in Hz
    #define MCPWM_SWITCH_FREQUENCY_MAX		40000	// The highest switching frequency in Hz
    #define MCPWM_SWITCH_FREQUENCY_DC_MOTOR	25000	// The DC motor switching frequency
```

---
## \#25 Posted by: Pafrican Posted at: 2017-04-18T22:07:18.439Z Reads: 58

```
You're completley right @Maxid, I'm not sure how I overlooked that. 
12s 8000mAh (series) will get me just as far as 6s 16000mAh (parallel).
For anyone that's not sure how:
Let's say that a 12s 8000mAh setup drains in an hour with a constant top speed of 20 mph; which means that my range is 20 miles per charge.
A 6s 16000 mAh setup drains in 2 hours (twice the capacity) with a constant top speed of 10 mph (half the voltage); which means my range will still be 20 miles.
Running with higher voltage means less current draw, so the entire system runs cooler and more effeciently. Seems like series is the way to go for me!

Thanks
```

---
## \#26 Posted by: Hummie Posted at: 2017-04-18T22:08:22.067Z Reads: 56

```
but if you're going slow it's more inefficient at 12s and might as well stay at 6
```

---
## \#27 Posted by: PXSS Posted at: 2017-04-18T23:43:53.383Z Reads: 54

```
@SimosMCmuffin
Where were you 6 months ago when I was starting my build? I let myself get convinced into the high voltage argument even though I never plan my gf to go above 18mph... (limited in bldc... :( )
```

---
## \#28 Posted by: Maxid Posted at: 2017-04-19T05:32:12.036Z Reads: 52

```
So? That going faster drains your battery quicker was always known. High voltage is still the way to go. We have no data on how the duty cycle efficiency changes range (if at all)
```

---
## \#29 Posted by: PXSS Posted at: 2017-04-19T07:59:07.714Z Reads: 48

```
[quote="Maxid, post:28, topic:21299"]
That going faster drains your battery quicker was always known.
[/quote]
Speed is constant. 

[quote="Maxid, post:28, topic:21299"]
High voltage is still the way to go. We have no data on how the duty cycle efficiency changes range (if at all)
[/quote]
Not necessarily. You also have no data on how higher current affects range. Yes we have an equation to correlate resistance to heat produced but I for one have not gone through my whole system and added up resistance, have you?
Efficiency of BLDC at 50% is pretty terrible as far as I remember... I haven't done the math in a few years
```

---
## \#30 Posted by: Maxid Posted at: 2017-04-19T08:20:30.031Z Reads: 49

```
[quote="PXSS, post:29, topic:21299, full:true"]
Yes we have an equation to correlate resistance to heat produced but I for one have not gone through my whole system and added up resistance, have you?
[/quote]
Why would you? assuming the same resistance in either scenarios the high voltage one will produce less heat - as to how much we don't know, just like we don't how the actual effect of the duty cycle efficiency. Why would you then say
[quote="PXSS"]
Where were you 6 months ago
[/quote]
when we have no idea and nobody is going to measure?
@SimosMCmuffin even said he is using his own motor controller - as to how his data correlates to the VESC we also don't know. For me this would be too many variables and I'd stick to the proven solution that is: higher voltage is better than higher current.
```

---
## \#31 Posted by: PXSS Posted at: 2017-04-19T11:41:19.962Z Reads: 43

```
[quote="Maxid, post:30, topic:21299"]
Why would you?
[/quote]
I'm an engineer that is always striving for the best performance. That's why.
```

---
## \#32 Posted by: Okami Posted at: 2017-04-19T12:01:08.465Z Reads: 41

```
@PXSS  Ive heard foc mode is more efficient.

Do u think motor's effiency would affect range such drastically even if speed is higher?

I think it would 'level out'

Let's say - with inefficient motor efficiency and low speed you consume 10wh/km, for example.

Then with higher efficiancy of motor, even when speed is higher (and wind / rolling resistance too), u  might still consume very close to 10wh/km..

At least this.is how.i see it but we need.some hard data for.this..
```

---
## \#33 Posted by: Maxid Posted at: 2017-04-19T12:19:55.411Z Reads: 41

```
This was solely based on measuring the resistance. Even as an engineer striving for the best it is unnecessary to measure the individual resistances of your setup. The higher current scenario will always generate more heat than the high voltage scenario since a resistance of 0 is impossible. 

What you can do (and I agree if you want the best) is find out how much the duty cycle efficiency matters. But in order to do this you also don't need to measure the resistances. You would have to make actual riding tests and compare the ranges with each other (just like what @SimosMCmuffin did at different speeds you would have to do at different voltages and the same constant speed on a dyno if possible)
```

---
## \#34 Posted by: PXSS Posted at: 2017-04-19T14:18:22.311Z Reads: 44

```
[quote="Okami, post:32, topic:21299"]
Ive heard foc mode is more efficient.
[/quote]
Correct. Specially at partial loads. I haven't read much into it since school though and don't really remember how it works.

[quote="Okami, post:32, topic:21299"]
Do u think motor's effiency would affect range such drastically even if speed is higher?
[/quote]

If you are running at 50% duty cycle then definitely. Even my high end RC ESCs ($400 - Kontronik Jive Pro) hate being at 50% duty cycle without lots of airflow. 

What I'm looking into isn't really related to speed though. I know my gf never rides above 18mph, usually more like 12-15mph. Her setup is made to top out around 40mph...

@Maxid
Yes, you are correct that the higher voltage would be more efficient as resistance is not zero. But losses in bldc are significant. I want to say significant enough to offset the high voltage gains. 

I was extremely exhausted last night. I've only gotten 6 hours of sleep over the past 3 days... I realized that I geared her setup wrong... Right now, its 16:36, so top speed ~40mph since shes 110 lbs... If I gear it to 14:44 then top speed will be ~22mph. 

That takes advantage of both high duty cycle and high voltage
```

---
## \#35 Posted by: Maxid Posted at: 2017-04-19T14:29:27.855Z Reads: 42

```
Thank you!
That was going to be my next point: Gearing can make all the difference and was the reason why I could go 35km/h on my first 6S build with a 149kv motor by choosing an "uncommon" ratio of 20/28 for my kegels.

I would love to know how big the losses due to the duty cycle actually are. If someone is ever going to measure or calculate let me know. For the average joe I guess the easiest is still to just go as high of a voltage as possible and then adjust the speed via the gearing.
```

---
## \#36 Posted by: PXSS Posted at: 2017-04-19T15:15:13.914Z Reads: 40

```
If VESC can run on 5S then I can probably still test it as both her and my setup split into 2 5S packs to charge
```

---
## \#37 Posted by: Nordle Posted at: 2017-04-19T15:15:59.065Z Reads: 39

```
It's rated 3S to 12S.
..except enertion 4.13 boards, cause he doubt its clever to save money on caps and so that one is only 10S
```

---
## \#38 Posted by: Hummie Posted at: 2017-04-19T17:11:28.402Z Reads: 33

```
Please do test with the different voltages and same speed. On vedder's site I was told the losses at half duty would be pretty small in comparison to full
And please do a temp test on the motor for both. My batteries are all hard wired. 

I think u can limit the vesc duty cycle to make it a better test
```

---
