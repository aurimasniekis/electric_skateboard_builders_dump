# For you guys with powerful boards, how about an acceleration ramp?

### Replies: 37 Views: 2641

## \#1 Posted by: mainstreet Posted at: 2017-03-23T06:12:49.019Z Reads: 269

```
I'm not talking about limiting current so the acelleration is less but the ramping of the acceleration over a time period, maybe a second or two so the rider can brace for it.  

I'm running a 5500W board and it can be jerky if I'm not careful. I'm building a 6200W hill climber and I'd love to ramp the acelleration / beaking on the Vesc. It's would be nice  to limit sharp changes in acceleration to suit the rider and make a safer board more ridable board. Maybe like this:

When you pin it forward the acceleration or currently will increase over a short time period. 

When you reduce the throttle or release the throttle, acceleration will ramp  down to a coast over a short time period. 

When you brake it would ramp to the negative acelleration. You may want this to have a shorter ramp for braking responsiveness but to still be ridable. 

When you release brakes, it would release over a time period vs that jerky feeling when you let go from braking. 

What do you guys think?
```

---
## \#2 Posted by: rpn314 Posted at: 2017-03-23T06:15:59.352Z Reads: 254

```
Have you read through the firmware mod that @Ackmaniac is doing? Sounds pretty similar to what you're proposing.
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2017-03-23T06:16:44.788Z Reads: 248

```
A vesc and @Ackmaniac program think works similar
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-23T06:32:10.482Z Reads: 247

```
Sounds like your talking about some type of response delay. Kinda like when your driving a car with stick shift and your in a high gear  cruising  and you stomp the gas pedal but the car increases speed slowly.
```

---
## \#5 Posted by: PXSS Posted at: 2017-03-23T06:40:17.052Z Reads: 237

```
Ugh. I absolutely hate that. 
I recommend playing around with the throttle curve maybe? I'm not sure how commands work on the vesc but if it's a PID then you could definitely tune it to be mushier
```

---
## \#6 Posted by: mainstreet Posted at: 2017-03-23T06:57:07.905Z Reads: 219

```
Yeah. That's it. @PXSS.  If you wanted it mushy, you could; I don't but you could do that. I'm talking about much shorter ramps where you could tune the ride to be less jerky, more glide, but still responsive with no power limitations. I'm talking about powerful boards here. 

Imagine driving a car and you take your foot off the gas quickly, you don't have a jerk as the acceleration stops. Now it would be different if you were surfing on the roof and feel it as you adjust your stance. 

Since some if us are surfing these really powerful boards, I think some acceleration ramp would help over powered machines be much more approachable yet still responsive. More refined.
```

---
## \#7 Posted by: Maxid Posted at: 2017-03-23T07:14:45.230Z Reads: 206

```
Isn't the title misleading? You are not looking for an acceleration curve but to have interpolation between throttle states.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-03-23T07:24:47.810Z Reads: 204

```
Well, my firmware mod changes the throttle curve. What you want is a throttle ramping. But it's already there in the Nunchuk controls. 
@mainstreet So best for you is to get a nunchuk or a nrf controller.
```

---
## \#9 Posted by: mainstreet Posted at: 2017-03-23T08:22:09.836Z Reads: 203

```
Ok. So not quite. I get the throttle curve and how the position of the controller throttle can be calculated to mean an Esc throttle value based on a curve or slope/ramp. 

Please allow me to add context. 

The main issue I'd like to solve, when I ride my powerful board, is I have to slowly let go of the throttle or it feels jerky. Like when I pin it and I let go of the throttle. I'm used to it but it's not what I want people to experience when they ride my boards. 

It is a throttle state change with time variable. If you let go of the throttle the motors freewheel, the rider stops accelerating and it feels like the brakes are tapped. It can be unnerving for a rider at high  speeds. 

If you ramp or curve the throttle with a time variable say 1 sec or so the feeling of stopping accelerating would be smoothed out to the coast.

In the automation world I work in, we use these functions to make motors move smoothly. When the program calls for MAX speed, we adjust the acceleration of the motor gradually over a short period of time. Not to be confused with the speed or rpm but the value of the acceleration; the rate at which the speed increases or decreases. 

Make sense?
```

---
## \#10 Posted by: Nordle Posted at: 2017-03-23T08:26:38.565Z Reads: 193

```
5,5kW and 6,2kW? Just curious what battery are you using?
```

---
## \#11 Posted by: Maxid Posted at: 2017-03-23T08:40:49.642Z Reads: 190

```
Yeah - you are describing what I mean by throttle interpolation. You don't want to go instantaneous from one to the other but smooth the transition.
This is not an acceleration curve so the title is still misleading for me.

I do have to add that letting go of the throttle does result in no jerking on my board - maybe you should also look into the efficiency of your gear setup. On my hub motors I just coast.
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-03-23T08:59:44.384Z Reads: 183

```
Just let us know what motors you are going to use for your hillclimber and what remote you are using. And as i said already. The Nunchuk has the function of ramping.
But to me it sounds like you might overstress your batterys and that could be a reason for the jerky feeling. Or you have a bad setup for the VESC. Because when the VESC starts to limit the power and you give full power those little jerky situations can happen.
```

---
## \#13 Posted by: Gromok Posted at: 2017-03-23T11:30:32.928Z Reads: 168

```
I have been looking for that sort of thing as well so you are not alone, mainstreet.

I wish to build a board that is capable massive wattage by using VTC6 in 10s6p or 12s5p configuration and VTC6 has 15c and max of 30c with 80 degrees cutoff meaning it could peak as much as 7,560 watts. ( not sure if I can use "c" as amps in the v*a=w equation? )
```

---
## \#14 Posted by: saul Posted at: 2017-03-23T12:27:42.607Z Reads: 162

```
you have the numbers right, but the wrong units. vtc6 and most 18650 have output in Amps. 15a and 30a max current. but you end up with about half the capacity at those rates. 

why do you guys want that much Power? theres no torque increase past the saturation point.
just stressing your batteries....

half the power is enough to scare you and embarrass any complete...
```

---
## \#15 Posted by: Gromok Posted at: 2017-03-23T12:56:07.226Z Reads: 164

```
Thanks for clearing that up. Was just talking about how it is possible to crank out that much wattage with VTC6, but I do not intend to push it that far up.

I plan to cap the absolute limit to 80 amps thus each motor gets maximum of 40 amps each. 

The reason why I know that is more than enough power for me is that I have an Evolve GT Bamboo and also I know that the GT peaks out at 1100 watts meaning max of only 550 watts each motor and we know how strong GT mode is :stuck_out_tongue_winking_eye: ( Found that info on Evolve forums )

My board will be more powerful than that obviously, so still interested in ways of making control buttery smooth!!
```

---
## \#16 Posted by: trampa Posted at: 2017-03-23T13:24:12.293Z Reads: 158

```
Hi @mainstreet, VESC-Tool has some more settings to allow more control over the throttle. In some cases you would want to be able to react fast to unforeseen obstacles. A delay would not help in that case. 
If I read your post correctly, you want to use a VESC, right? You may want a VESC 6 in that case, running the all new firmware and being adjusted by VESC-Tool. My personal V6 board rides very smooth - but its a beast at the same time. 
Truth is: If you gear down a lot, brakes get more effective. 
Some people like it ultra direct and others like the butter.
I can let go the throttle without the board trying to throw me off. 

Frank
```

---
## \#17 Posted by: mainstreet Posted at: 2017-03-23T18:07:42.269Z Reads: 161

```
@Nordle I am using: 

LiFePO4 8s2p Prismatic Pouches
30C Discharge at 16Ah

My 6364 motors are the limiting component in my system protected by the VESC current settings. 

Who knows what the real current is in the system when the board runs but I weigh 260lbs and it has no problem on steep hills. I tried to over spec as much as I could. 

I had a 10C Lipo pack on this same board and it was gnarly in comparison.
```

---
## \#18 Posted by: mainstreet Posted at: 2017-03-23T18:26:54.723Z Reads: 165

```
[quote="Ackmaniac, post:12, topic:19531"]
But to me it sounds like you might overstress your batterys and that could be a reason for the jerky feeling. Or you have a bad setup for the VESC. Because when the VESC starts to limit the power and you give full
[/quote]

OK so my hill climber build is:

2x 6374 190Kv Sensored from Tourque Boards

I have 2x VESC that I am contemplating a mineral oil bath for cooling. I wanted to see how the temp runs before going to all that trouble. From a fabrication-porn standpoint I like it. 

Here is my current battery pack spec I did a few months ago. 

<img src="/uploads/db1493/original/3X/a/b/ab0342a74140e055b477c198c47284bc57bf2e89.png" width="504" height="361">
```

---
## \#19 Posted by: Ackmaniac Posted at: 2017-03-23T18:54:57.136Z Reads: 160

```
And what are your VESC settings? Screenshots please.
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-03-23T19:00:09.339Z Reads: 162

```
[quote="trampa, post:16, topic:19531"]
Truth is: If you gear down a lot, brakes get more effective.
Some people like it ultra direct and others like the butter.I can let go the throttle without the board trying to throw me off.
[/quote]

This. Pulley ratio and wheel height have at least as much to do with the feel of braking and acceleration as VESC settings do. 

Taller wheels on smaller pulleys make the brakes smooshy and the acceleration smoother, where smaller wheels on larger pulleys make the acceleration harder and the brakes stiffer. 

You can of course make noticeable differences with VESC settings, but there is also a lot of magic in the gearing and wheel height.
```

---
## \#21 Posted by: Mrmoonlight Posted at: 2017-03-23T20:11:56.993Z Reads: 150

```
That's what I was thinking. Gearing ratios and wheel size at high speeds can cause the board to feel like it's braking when you release the throttle. With single gears, we're using our motors at high rpms to attain more speed, but once we let off the trigger, compression brakes take over. Just like running your car at higher rpms in lower gears. 

Like Maxid, I solved this by switching to hubs. Since there's no gears, you just coast when you let off the throttle regardless of how fast you're going. Acceleration and braking are more responsive and at the same time, smoother. With a geared setup, I imagine the closer you get to a 1:1, the less compression you will feel when you let off the throttle. When I was riding a belt drive, I would let off the throttle slowly when at high speeds to avoid jerking.
```

---
## \#22 Posted by: mainstreet Posted at: 2017-03-23T20:48:26.599Z Reads: 145

```
I get what you are saying. The board coasts pretty good. Its no pusher but you get the picture. 

Think about it this way. When you are accelerating the rider experiences, lets say, .5G of acceleration. When the throttle is released the rider suddenly feels 0G. Its not a negative G in the other direction, but the sudden decrease to zero G, or near zero after taking in the inevitable drag that some you have alluded to. 

By ramping the acceleration down to zero in this scenario over a second or so, it would make for a smoother ride.

As I mentioned in near the top, braking could have a little or no time delay for obvious performance/emergency reasons mentioned by @trampa. I totally get that. 

I appreciate everyone's feedback. Its really helpful to gather everyone's experience.
```

---
## \#23 Posted by: Mrmoonlight Posted at: 2017-03-23T21:14:03.106Z Reads: 139

```
If your boards not a pusher, it's not a good coaster. I sometimes push my board because I enjoy it. It's a totally different feel.
```

---
## \#24 Posted by: laurnts Posted at: 2017-03-24T18:46:54.543Z Reads: 130

```
Increasing the ppm median timing in Vesc will smoothen it out. The median timer in vesc by default if im not mistaken is 5 seconds. So it will average the last 5 seconds throttle position. If you increase it by 10 seconds it will really smoothen it out nicely.
```

---
## \#25 Posted by: Stef Posted at: 2017-03-24T21:50:43.564Z Reads: 127

```
This is probably the easiest effective solution to implement without needing custom code.

As a Mechanical Engineer I would limit the 'jerky feel'  by limiting the jerk which is actually the time derivative of acceleration or 'change of acceleration'. Jerk on a E-board sucks because you need to lean forward or backward to counterbalance acceleration or braking, meaning that if you apply throttle (acceleration) very quickly, you have to adjust your leaning angle very quickly too, so it feels unstable and hard to balance. Averaging the throttle works as a low pass filter so it limits the jerk.
```

---
## \#26 Posted by: Ackmaniac Posted at: 2017-03-25T02:07:23.937Z Reads: 123

```
Did you try to use my firmware mod and adjusted the throttle curve? This would make a huge difference. And please post screenshots of your settings.
```

---
## \#27 Posted by: mainstreet Posted at: 2017-03-27T16:57:39.351Z Reads: 111

```
I haven't had a chance to check it out. Sounds interesting for sure.
```

---
## \#28 Posted by: mainstreet Posted at: 2017-03-27T22:06:15.083Z Reads: 106

```
@Stef - Yes exactly, the change in acceleration. This is why it is really felt on the more powerful boards. Thanks for understanding grade 10 physics. :D
```

---
## \#29 Posted by: Stef Posted at: 2017-03-27T22:20:59.040Z Reads: 107

```
Credit of the idea goes to laurnts, i just second it with some physics :) 
Im building a short wheelbase 2x 6355 board so will probably also use this method to tame it a little bit.
```

---
## \#30 Posted by: PXSS Posted at: 2017-03-27T22:33:07.767Z Reads: 104

```
@mainstreet, If we had access to the PID controller, we would be able to control the throttle response way better. Once the summer rolls around my gf will give the VESC a go to produce a better controller. 
She's a CS/ME major with controls background so it should be a fun project.
```

---
## \#31 Posted by: Duffman Posted at: 2017-03-28T07:46:14.255Z Reads: 94

```
... or you could simply use the appropriate parameter of the VESC:

Motor Configuration / Advanced / **Max current ramp step**

<img src="/uploads/db1493/original/3X/5/b/5b3f64a3306483f468cb175a46701ddc2051c41d.jpg" width="345" height="194">

This parameter controls how fast the motor current can raise and therefore how fast the force that accelerates you can increase. If you lower this value, from default of 0,04 to 0,001 or even less you can pull the trigger completely and the power of the board builds up slowly until maximum is reached.
```

---
## \#32 Posted by: mainstreet Posted at: 2017-03-28T17:32:29.670Z Reads: 90

```
[quote="Duffman, post:31, topic:19531"]
nt can raise and therefore how fast the force that accelerates you can increase. If you lower this value, from default of 0,04 to 0,001 or even less you c
[/quote]

Wow. Yeah. That could be part of it. The challenge is that you may want more variables to make it more ridable. But that description reads like a solution to item 1. I outlined below. 


To be clear and beat the dead horse :)

**Accelleration** - Acceleration is defined as the rate at which an object (skater) changes its velocity (speed). An object is accelerating if it is changing its velocity (speed).

As I see it there are four states where you may want the acceleration to be ramped.

**1. Forward** - The rate at which acceleration is increased in the forward direction. 
_ie when you pin the throttle_

**2. Forward Decrease** - The rate at which acceleration is reduced in the forward direction. 
_ie when you release the throttle and it snapps  to middle_

**3. Braking** - The rate at which acceleration is increased in the negative direction while braking. 
_ie you may wan this to be a very steep ramp to the brakes are responsive but not so much that you get thrown off yet still have full braking power after the ramp time._ 

**4. Braking Decrease** - The rate at which acceleration is decreased in the negative direction while braking.
_ie when you release your brakes, it can be done over a short period of time to make it less jerk_y.

I know we have all learned to feather our throttle thumbs for a smooth ride but when the boards get more powerful they begin to act like less like a refined product and become much less approachable to less experienced riders. Now I know there are lots of little arguments like why is a less experienced ride on such a powerful board, but I think the main driver for me is to create a technically refined and approachable boards.

Again, guys, appreciate all the great conversation here.
```

---
## \#33 Posted by: PXSS Posted at: 2017-03-28T20:37:22.740Z Reads: 85

```
Research PID controllers. They do exactly that. 

The proportional gain controls how fast you reach your command. Think of it as a spring, the stiffer it is the faster it will pull to it's commanded position. 

The derivative gain dampens the command. So think about that spring without a damper, you'll reach your command, most likely overshoot and then oscillate about the commanded position. With a damper, it'll decrease the oscillations over time and reach a steady state faster

Your integral gain looks at the error between your command and where you are, if there is a difference between where you ended up and where you commanded then it'll shrink that over time. 

By adjusting gains you can fine tune how fast your board responds, not overshoot the commanded position and remove any oscillations that might be happening. 

<img src="https://upload.wikimedia.org/wikipedia/commons/3/33/PID_Compensation_Animated.gif" width="345" height="194">
```

---
## \#34 Posted by: mainstreet Posted at: 2017-03-29T18:13:21.594Z Reads: 79

```
[quote="PXSS, post:33, topic:19531"]
justing gains you can fine tune how fast your board responds, not overshoot the commanded position and remove any oscillations that might be
[/quote]

@PXSS Yeah I'm quite familiar with PID from the automation work I do. Is the VESC capable of the functions required to calculate it with without bogging down the processor?

I cant help but think a simple linear relationship between acceleration and time may work well given the calculation is so much more light-weight in the VESC processing.

One consideration when using PID is that you will be constantly changing your target value as the throttle is adjusted. It may prove to processor intensive in respect to all the other routines the VESC is running. 

Just a thought.
```

---
## \#35 Posted by: Ackmaniac Posted at: 2017-03-29T19:25:35.841Z Reads: 75

```
Give my firmware mod a try and then we can talk about something that might can be changed. And please also post your VESC settings to have some real numbers.
```

---
## \#36 Posted by: PXSS Posted at: 2017-03-29T20:24:25.472Z Reads: 75

```
Pretty sure it's more than capable. Have you seen the tiny quadcopter flight controllers??? They're like .5"x.5" and run PIDs on throttle, roll, yaw, and pitch at 8kHz on a 16bit processor
```

---
## \#37 Posted by: Okami Posted at: 2017-03-30T02:22:51.695Z Reads: 70

```
@PXSS Can u give a more explanatory answer as what PID is?

Im starting to witness a delay in my remote's signal vs what the car esc does (yes, not owning a vesc unfortunately)..

Im not sure but i think at the beginning of using the board / riding it, **there was no delay!**

--

Do you have any ''explanations'' on why else the delay might be caused?

I can only set the trim on the remote itself, im using mini remote, which is 2.4ghz.. Do you think it can be modded with the help of some other componenets to adjust the signal or delay?

I've heard that for ''trimming'' a simple resistor can be placed in chain with the potentiometer, **thus 'creating beginner mode'' for the remote**.. not sure is it possible to modulate the signal or make other adjustments in such a simple way..

--

**What Im refering to 'delay' is that power starts to be delivered (esc - motor responds) only 1-2 seconds after I have sqeezed the trigger,**

 I've been planning on re-setting the 0 and high / low point of the remote once again but Im a little bit afraid, since last time it took some time before I managed to set it right and get it working..

----
My 2nd guess as why Im experiencing delay is that maybe there is a problem with antenna wire? Im sort of having it outside of power cables, so it is not in direct contact.. 

The only problem is, Im not having it in straight line up in the air but it is layed sideways along the enclosure.. though this did not cause problems before so Im not 100% sure it is just the antenna which is delaying / messing with the signal
```

---
