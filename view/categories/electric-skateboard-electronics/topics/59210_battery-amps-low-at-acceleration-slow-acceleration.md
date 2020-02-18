# Battery Amps low at acceleration, slow acceleration

### Replies: 46 Views: 680

## \#1 Posted by: franky0581 Posted at: 2018-06-17T19:48:01.925Z Reads: 163

```
Hello ESK8 Builders,
I am using a Maytech VESC and a Maytech MTO5065-70-HA motor in combination with a 10S3P battery with own BMS.

I have set the Motor Max to 55A and the battery max to 40A.
Using the app of Ackmaniac I can see that during full acceleration the motor Amps are not going higher than around 20A.
The acceleration is very slow also.
Shouldn't the motor amps not achieve more or less the max amps defined in the VESC? I wonder why the amps are not getting higher even if push the remote control to 100%.

I calibrated the remote control in the VESC, so I believe this is not the issue.

Any hints or explanation from you guys is highly appreciated.

Thanks & Regards
Frank
```

---
## \#2 Posted by: Silverline Posted at: 2018-06-17T21:44:15.206Z Reads: 150

```
How about the voltage ? Does it sag a lot, under acceleration ?
```

---
## \#3 Posted by: franky0581 Posted at: 2018-06-18T06:11:48.769Z Reads: 134

```
No voltage sag during acceleration.
```

---
## \#4 Posted by: rey8801 Posted at: 2018-06-18T06:42:43.967Z Reads: 127

```
Hi! Which cells are you using for the battery? Ackmaniac software usually works based on the watt instead of current. Could you please post your setting in the VESC tool or VESC app? Anyhow the max value you set will be reached only during really fast accellaration or on steep hills. I also never reach the max values set and in any case it will be just a peak of current. In order to understand you can also post a telemetry data if you use the app.
Other thing to know is if you use the BMS for charge only or also for discharge. If it's also for discharging which one are you using? Specs?
Third thing single 5063 motor is rest her small so you can not aspect a speedster from it. I hope you are light otherwise you can think to move to a single 6374 motor.
Let we know.
```

---
## \#5 Posted by: franky0581 Posted at: 2018-06-18T22:10:33.855Z Reads: 102

```
I appreciate a lot your feedback. I will post the settings from the BLDC tomorrow.

My main question is if I should see when starting from zero speed and fully accelerating for a few seconds the max motor current as programmed in the VESC or not? If yes, can it be because of the small motor that the maximum programmed motor current is not achieved?

Thanks for the advice of the 6374 motor. Do you know if there exist any torque diagrams for these kind of motors in general?

Thanks a lot and Best Regards
Frank
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-06-18T22:29:27.563Z Reads: 94

```
you also need to calculate the wh of your battery since ackmaniac throttle is centered around that.
```

---
## \#7 Posted by: franky0581 Posted at: 2018-06-18T22:44:51.257Z Reads: 92

```
Sorry, maybe for clarification. I just use the Ackmaniac app to see the live data. I am still making the programming in the BLDC tool. I have not changed to Watt Mode.
```

---
## \#8 Posted by: xclr8r Posted at: 2018-06-19T06:00:12.681Z Reads: 85

```
Which remote are you using?  My remote has a slow mode on it that basically cuts the amperage the motor receives by half what I’ve got my FOC Box programmed at. Screenshots of your settings would be helpful.
```

---
## \#9 Posted by: franky0581 Posted at: 2018-06-19T06:13:37.523Z Reads: 82

```
http://www.maytech.cn/en/maytech-mtskr1712-e-skateboarding-mini-wireless-remote/11032.html

I use this remote from Maytech.. I put it on the "fast mode" LED flashing with higher frequency and in this Setup I am adjusting the bandwith in the BLDC Tool to ensure it reaches 100% & 0%. 
This should be fine or?

My main question is if I should see during acceleration that the maximum motor amps are achieved or if it is normal that the values I see in the datalogger are way below?

Thanks
```

---
## \#10 Posted by: rey8801 Posted at: 2018-06-19T06:44:27.902Z Reads: 72

```
In my case I never reach the max watt or current I set. I have seen people reached with belt drive system but I am using hub motors and they are not capable of the power the battery can provide. It is true that what matter is the battery current, because that is where the limit is. I would say that for a single motor 5063 you probably saturate the stator without the need of drain all the current available, that's why your motor amp doesn't reach the max value even during hard acceleration. You should also check the battery amp, maybe you reach the max value there.
Covering the motor mapping curve you won't find anything like that in the datasheet. Although what matter is the stator size so 6374 bigger stator = more wattage. There are plenty of good motor. You can find also second hands one on the forum and you save some money. Torque Board, HobbyKing, BKB, Maytech, Esk8 motors are all good.
```

---
## \#11 Posted by: xclr8r Posted at: 2018-06-19T22:10:17.170Z Reads: 64

```
That’s the same remote I have as well. Alternate between slow and fast mode to test it. Watch your real-time amps at full acceleration in each mode to see how they differ. Obviously the motor will pull less amps when remote is in slow mode.
```

---
## \#12 Posted by: Pantata Posted at: 2019-02-12T22:35:49.190Z Reads: 57

```
I am trying to figure out the same thing. How can one achieve better acceleration? Volts are according to speed so I cannot do anything there and my focboxes are not reaching max motor amps, nor max battery amps. The thing is even when accelerating from a standstill under full throttle I only get like 45 amps into my motors. I thought max throttle means max possible amps into the motor (as pre-set) My wattage is set to 15000 as default as I don't need to limit that but how does it show on the remote that is "watt" based and not amp based. In other words how the hack do I make my board use more motor amps? :) My max wattage according do vesc data was around 1800w. I ride 12s dual 6355 3500w motors with preset 70a for each motor and 30a battery amps for each motor. So I am reaching a little over half of the power I have set.
```

---
## \#13 Posted by: Flashgod224 Posted at: 2019-02-13T00:08:02.879Z Reads: 52

```
Sometimes you don't need that much amps to do the job, from a standstill it might be 45a, from a standstill on a hill going up it may be more. 6355 motors don't feel as torquy as 6374 motors from my experience, I was never able to get to a full stop on dual 6354 motors (190kv). Now I run my pneumatics and dual 6374's, geared at 60t/18t and I can get to full stops.

Some motors can't do the job efficiently especially 50xx motors and just make heat instead of actual work. Think you should consider having bigger motors, the same concept for hub motors. Hubs are smaller in general, only Hummies, R-spec hubs are the biggest hubs on the market imo that have a major impact. If you are looking to break the 40km/h barrier then bigger motors are the way, because after that much speed you need more amps from the battery to keep the motor accelerating faster. (also bigger motors means they can handle much more current) And that's why I tell all my diy friends that the most expensive part of a board is batteries because it = torque in the end game.

For reference I run 10s5p 30Q cells, dual 6374 motors and 6" Haggy pneumatics. I've gone past 55km/h as of recent with this set up, definitely will be more during warmer weather.
```

---
## \#14 Posted by: Pantata Posted at: 2019-02-13T01:00:40.322Z Reads: 47

```
Thanks for the reply, bigger motors definitely will do better. And I agree with what you are saying but still what you say about motor amps doesn't make sense to me. If my unit would give more amps to my motor If I was going more uphill than there would be some kind of acceleration limit cause it shouldn't care whether I am going uphill or not. It should give max power with max throttle, it shouldn't decide what to give, that wouldn't make sense. How would anyone be able to achieve anything over 2000w If the voltage stays the same and amperage in motors doesn't go above 40-50 amps and battery amps barely reach 50 when they are set to 60... Everything has room yet the power available is not being achieved so something somewhere must be limiting that. I am running 12s4p 30q, 6,5 inch trampas so we are really close. 18/62t
```

---
## \#15 Posted by: Flashgod224 Posted at: 2019-02-13T01:59:49.954Z Reads: 49

```
so 40amps of play per motor maximum, but still like I said, to actually DO the work to get you up to speed takes much less amps because the motor is bigger. That being said, the only thing that takes up more amps on an esk8 is start up, but even then once it gets up to speed it takes less amps to ramp up depending on your throttling. On my Focbox Unity I run batt 50/-20 and motor 60/-55, which is plenty of torque in my opinion when I don't get voltage sag. It doesn't take 2000watts to get you from 0-100, the bigger the motor the more efficient it is because it produces less heat and more work done than having a smaller motor. 

Smaller motors will produce more heat under a load which causes them to lose efficiency. If you pull a heavy load then the motors will probably put out more wattage. AmpsxVolts = Watts. Reguardless, if you program your vesc for much higher settings (+60 amps) you will feel much more power/torque but remember that they are just limits to what you program your board to do. 

**Voltage**  - Think of it like how big a muscle is
**Amps**  - Think of it as how much energy you can send to that muscle

You don't need more amps if your muscles are already big, but if you put in more amps then the work will be done faster but energy depleting faster. There is no acceleration limit, you just need to adjust your throttle curve up to give your self more power for acceleration
```

---
## \#16 Posted by: Pantata Posted at: 2019-02-13T02:07:33.448Z Reads: 42

```
My problem is not not having torque :) My problem is wanting more and more torque and I still don't understand why the motor doesn't get more amps. I get all the stuff about bigger motors and heat loss (though it would be nice to see some data cause there are many facts and many of them are not important... For ex. the difference in power loss due to heat built up the moment I start accelerating between 6355 and 6374 might be really negligible. But I don't know so data is needed) Pulling a heavier load will consume more watthours but it should have nothing to do with how many amps are given to motors when full throttle is applied. The only difference should be me, as a lighter guy, accelerating faster. Motor outputs whatever it outputs, it doesn't discriminate between light and heavy guys or one going uphill or downhill. If I am applying more power than using the motor amps/battery amps should keep raising. With 100% throttle I should be getting maximum of what is capable. You get what I am saying right?
```

---
## \#17 Posted by: Flashgod224 Posted at: 2019-02-13T02:10:00.294Z Reads: 38

```
Ye I understand, maybe it's just that you don't have that amounts of amps to give yourself the full power you desire. If you ran Lipos then you would probably get what you want because of the amount of amps it can output. 12s4p doesn't sound like it will get you more torque than you can already/have achieved.
```

---
## \#18 Posted by: Pantata Posted at: 2019-02-13T02:11:06.504Z Reads: 39

```
The only thing that would make sense to me is that my battery is not capable of giving more than 50 amps at a time... Is it possible? 4p 30q samsung. Does the immediate discharge value go down over time as well and do you know how much?
```

---
## \#19 Posted by: Flashgod224 Posted at: 2019-02-13T02:11:45.955Z Reads: 37

```
It should be 60amps continuous and 80amps maximum
```

---
## \#20 Posted by: Pantata Posted at: 2019-02-13T02:11:58.606Z Reads: 39

```
But then there is the fact that when you are accelerating from a standstill since you are only getting like 0,5v to your motors then 70amps should be no problem to give to the motor. the battery amps are only like 10 per motor at the beginning with full throttle.
```

---
## \#21 Posted by: Flashgod224 Posted at: 2019-02-13T02:21:58.882Z Reads: 40

```
Hmm, if I am thinking about this carefully,  when you start from a standstill and throttle 0-100 then you will achieve the maximum torque you can get with your motors (also assuming you run FOC meaning start up is efficient). Though, running BLDC will dump amps aimlessly giving an insane amount of power to the motors not caring about the load at all. But still in the end it takes X amount of power to make a motor turn. If you had infinite amps to dump and a VESC to be able to dump that much into a motor, then your motor will henceforth be heating up as well as giving you your torque with the limit being the motor's capabilities. 

skip to 2:45
https://www.youtube.com/watch?v=boBT9NsGcUc
Trampa Streeet Carver:
6374 190KV Motors
12S4P Battery on Samsung 30Q
16/40T
100mm MBS wheels shaved at 95mm

Sector 9 Bintang
6355 230KV Motors
10S4P on Samsung 30Q
15/40T ABEC 11 Flywheels 97mm
```

---
## \#22 Posted by: Flashgod224 Posted at: 2019-02-13T02:38:16.937Z Reads: 38

```
Oh and forgot to put but the reason why bigger is better, is because bigger motor= bigger magnets which is bigger pole = more torque.
```

---
## \#23 Posted by: Pantata Posted at: 2019-02-13T09:51:02.272Z Reads: 37

```
Yeah I should but I don't. Running FOC like yourself. That's what I mean, I should get max power when the throttle is pressed all the way. That's why my confusion why it doesn't use more motor amps when it is not even close to the limit and yet I wanna accelerate harder and am already pressing the gas full way, yet not reaching any limits... I do not have infinite amps but I am satisfied with those 70a if possible :)
```

---
## \#24 Posted by: Pantata Posted at: 2019-02-13T10:47:48.297Z Reads: 38

```
Thanks for the video, there doesn't seem to be a big difference in acceleration between you two, after a few seconds your friend then keeps going full power and you back off, right?  Will get those 6374 motors. Meanwhile still need to find out why the motors aren't getting the full motor amperage at roll outs. Thank you again.
```

---
## \#25 Posted by: Flashgod224 Posted at: 2019-02-13T12:42:44.898Z Reads: 39

```
I don't take credit for the vid, it's one that I saw a long while ago.

What's your vesc settings? I think maybe you haven't given it enough juice to give the acceleration you want.
```

---
## \#26 Posted by: Pantata Posted at: 2019-02-13T12:52:12.209Z Reads: 37

```
What else is there except for motor amps, battery amps, wattage limit... The thing is I used to have much more torque, I know that was with urethane wheels but my max speed is almost the same and I ride with 70PSI trampas that are hard as a rock. I can feel I lost acceleration in past week or something like that. It's weird, I switched to regular vesc firmware where the throttle control is AMP based, not that it should matter, but wanna see If there is a difference.
```

---
## \#27 Posted by: Flashgod224 Posted at: 2019-02-13T12:55:24.369Z Reads: 38

```
That does sound very odd, if you have the same top speed then I assume that you have geared the drives to have the best amount of torque to accommodate for the larger wheel size. 
I don't have this issue, but it just got better when I switched from 6354 to 6374.
```

---
## \#28 Posted by: Pedrodemio Posted at: 2019-02-13T13:26:11.558Z Reads: 36

```
You should definitely be getting max current on the motors at full throttle 

How are your voltage cutoff configured? And do you have any ramping set for the remote?
```

---
## \#29 Posted by: Sn4pz Posted at: 2019-02-13T13:31:01.708Z Reads: 40

```
sounds like its maybe entering cutoff :thinking:
```

---
## \#30 Posted by: Pantata Posted at: 2019-02-13T19:43:58.295Z Reads: 40

```
Hi, I have it set for the regular cutoff for 12s that vesc tool offers. I don't get full motor amps even with full battery right at the beginning. I switched to default vesc firmware today and was looking through metr.at data and my motor amps did raise. Yesterday I had 2 times around 110a and today I had 5 times around 130. Which is reaching the limit for 2*68a per motor I have pre-set. SO my motor amps did raise after switching firmwares. But still I expect to get full motor amps every time I am going slow or standing still and pressing the throttle at full. So more confusion now... I have reached the motor amps but only a few times and also firmware affected my output... I tried long start on a slight uphill with full throttle for like 5 seconds, the first thing after fully charging my battery. I only reached 117a  (those 130 reached were later on during the ride so If it was battery potential or something it wouldn't be able to give more amps later on with more drained battery. I kept thinking about ramping time, will that affect motor amps? I have it set to the default values, haven't messed with it.
```

---
## \#31 Posted by: Pedrodemio Posted at: 2019-02-13T19:47:41.655Z Reads: 36

```
Could share the Metr logs and screenshots of the VESC tool?
```

---
## \#32 Posted by: Pantata Posted at: 2019-02-13T19:53:11.023Z Reads: 37

```
https://metr.at/r/sBDdm this is with ackmaniac firmware. 
https://metr.at/r/jwlwG   this is with regular vesc firmware

You can see higher motor amps with regular firmware.
Both had the exact same settings.
```

---
## \#33 Posted by: Sn4pz Posted at: 2019-02-13T20:39:07.402Z Reads: 35

```
I think you would want the WATT CONTROL mode or whatever its called, but PLEASE do research for those modes before you use them, as Ive heard about breaking being VASTLY different on that mode VS BLDC ( as soon as you turn the throttle down)
```

---
## \#34 Posted by: Pantata Posted at: 2019-02-13T20:40:48.932Z Reads: 34

```
I love the ackmaniac's watt control mode but as you can see I am getting more than 10% less motor amps with ackmaniac firmware in comparison with regular vesc firmware. Watt control is better and smoother I must say but wha'ts up with the motor amps being lower
```

---
## \#35 Posted by: Sn4pz Posted at: 2019-02-13T20:41:32.674Z Reads: 33

```
When dialing in your remote via PPM do you calibrate it?
```

---
## \#36 Posted by: Sn4pz Posted at: 2019-02-13T20:42:12.444Z Reads: 34

```
e: im an idiot nevermind
```

---
## \#37 Posted by: Pantata Posted at: 2019-02-13T20:42:28.644Z Reads: 35

```
Yes I do calibrate it. I will try to shorten the ramping time but still the amp differences in watt control vs amp control is weird
```

---
## \#38 Posted by: Sn4pz Posted at: 2019-02-13T20:43:11.236Z Reads: 34

```
any shot you can just factory reset with regular firmware? IE what it came with?
```

---
## \#39 Posted by: Pantata Posted at: 2019-02-13T20:44:09.367Z Reads: 34

```
that's what I did, that's the regular default vesc fimrware. max motor amps went to more than 10 percent more. Still not using max motor amps every time I pull the trigger to full from a slow speed or standstill. Only a few times has it come close to the max as per the data shown.
```

---
## \#40 Posted by: Sn4pz Posted at: 2019-02-13T20:48:05.675Z Reads: 35

```
so odd. Im sorry I cant help any more, I dont know all that much about VESC

It sounds silly but have you thought about the FW_NO_LIMITS or whatever its called? The software that removes all built in MAX values, and sometimes enables VESC users to run their HW normally
```

---
## \#41 Posted by: Pantata Posted at: 2019-02-13T23:03:53.517Z Reads: 29

```
I do have the firmware on my harddrive though I thought that is for when you wanna do something crazy :) would have to look into that. Thanks for all the advice man, much appreciated.
```

---
## \#42 Posted by: Sn4pz Posted at: 2019-02-13T23:08:26.242Z Reads: 29

```
please be careful when using the no limits if you do, your vesc is placed in 'manual' mode, you control everything. make sure to put the batt and motor amps lower for the first ride, just so you dont have it take off from under you :joy:
```

---
## \#43 Posted by: Santino Posted at: 2019-02-14T02:01:35.757Z Reads: 29

```
70 amps might be too much for 6355 motors, stator might get overload and efficiency might be lost. Unfortunately, for more torque you need bigger motors (6374 for example), adequate gear ratio for torque, and high C discharge battery.... Also a good quality Esc to push more amps. Just my thoughts...
```

---
## \#44 Posted by: Pantata Posted at: 2019-02-14T22:01:30.227Z Reads: 26

```
Ok so my story short. After almost crashing at 50 km/h yesterday after going back from ackmaniack's fw to the regular amp control default vesc fw and being so freaking lucky I went straight back to ackmaniac's firmware. Now the amps are a little higher and reaching almost their limits so it seems to be fine. Also first time ever I played with the ramping time and let me say, why isn't it mentioned everywhere that lowering the positive ramping time is the equivalent of "doubling" your acceleration? It's crazy, literally I can't believe what change from 0,3s to 0,2s did. It has crazy accel now, don't need bigger motors. Glad I tried that. So cheers to ramping time!Though it might be obvious to some, the ramping time does crazy miracles. Thanks everyone
```

---
## \#45 Posted by: Pedrodemio Posted at: 2019-02-14T22:09:47.935Z Reads: 26

```
That's why I asked about the ramping, if they are high you won't see peak current in most situations
```

---
## \#46 Posted by: Pantata Posted at: 2019-02-14T22:11:22.172Z Reads: 27

```
Yeah, you had a good question :) That's the info... You might not hit peak current as you go higher with the ramping time... All about the ramping time... thank you :)
```

---
