# I need an expert with Flipsky&rsquo;s Dual FSESC 4.20

### Replies: 130 Views: 2497

## \#1 Posted by: ADrum707 Posted at: 2019-01-05T23:49:05.507Z Reads: 321

```
I'm having the worst time programming this thing. I don't understand why it's twitchy, or why the remote has nearly no responsiveness - it's either off OR 100% full blast and no in between. I'm so frustrated - I could have now easily paid for a boosted stealth and been just fine. :cry::face_with_symbols_over_mouth::rage:
```

---
## \#2 Posted by: Benjamin899 Posted at: 2019-01-06T00:14:39.208Z Reads: 312

```
well with that little info you probably won't get any help.
```

---
## \#3 Posted by: ADrum707 Posted at: 2019-01-06T00:21:21.747Z Reads: 306

```
I've set my settings according to this: 

https://www.electric-skateboard.builders/t/flipsky-dual-fsesc4-20-info-review/71079

Apparently, these are the max settings this VESC can handle. My gear is: 

10amp hour battery (50 cells, 10s5p) 
2 180kv 2000w motors
nano remote control
and of course this flipsky vesc

My motors twitch, and the remote control doesn't ease in or out. It's either on 100% for more than I've held it for (i.e. I release the remote control and the motors keep on cranking) or they don't respond at all. They also don't respond evenly. Even though they're identical motors purchased at the same time.
```

---
## \#4 Posted by: Acido Posted at: 2019-01-06T00:22:41.236Z Reads: 283

```
Have you tested the throttle while actually standing on the board?
Post some screenshots of your settings
```

---
## \#5 Posted by: ShutterShock Posted at: 2019-01-06T00:25:16.344Z Reads: 273

```
Please recall that for the Enertion Nano-X remote, you MUST calibrate it every time you turn it on.

When you power on the remote, you must push the wheel to full throttle, then full brake, and then let it return to center.  This calibrates it and then you should have your normal throttle response.

Also please make sure to double check all ppm wire connections to ensure they have solid solder joints and such.
```

---
## \#6 Posted by: BigBrit Posted at: 2019-01-06T00:26:34.786Z Reads: 262

```
And to add to ShutterShock you need to do this before you switch the board on!

Remote on
Throttle all the way forward
Breaks fully rearward
Turn board on
```

---
## \#7 Posted by: J0ker3366 Posted at: 2019-01-06T00:28:36.710Z Reads: 255

```
[quote="BigBrit, post:6, topic:80043"]
Remote on
Throttle all the way forward
Breaks fully rearward
Release throttle
Turn board on
[/quote]

&lrm; &lrm;
```

---
## \#8 Posted by: BigBrit Posted at: 2019-01-06T00:29:18.431Z Reads: 251

```
Indeed.  Must let it go back to center.

Tbh the nano X is garbage.  I have two of them and they are crap
```

---
## \#9 Posted by: J0ker3366 Posted at: 2019-01-06T00:39:57.379Z Reads: 244

```
Buy yourself a 2.4 Mini remote. Much more reliable and trustworthy. Plus the Mini is getting more popular with case mods. So you could always re-case it to your liking. Just take the nano out of the equation.
```

---
## \#10 Posted by: ADrum707 Posted at: 2019-01-06T00:53:13.289Z Reads: 239

```
https://www.mboards.co/collections/remotes/products/remote-controller-1

Is this the Nano X? And given the incredibly limited packaging/instructions that come with it, without the help of you guys I never would have known about calibrating it. This one is suppose to have ride modes, which is why I picked it up. But it seems like it’s not worth that if it won’t even do it’s main job. When I’m programming the Vesc, do I also need to calibrate the remote prior to that? If so, it seems like it’s not reliable to keeping settings. Am I crazy?
```

---
## \#11 Posted by: ADrum707 Posted at: 2019-01-06T00:54:16.734Z Reads: 224

```
I’ll add screen shots as soon as I can get back to my windows machine
```

---
## \#12 Posted by: ShutterShock Posted at: 2019-01-06T00:58:01.803Z Reads: 221

```
Oh god... M Boards.  No that's not the nano that I am talking about.  We're talking about the Enertion Nano-X

https://www.enertionboards.com/categories/wireless-hand-controller.html
```

---
## \#13 Posted by: J0ker3366 Posted at: 2019-01-06T00:58:02.529Z Reads: 213

```
When you get to the remote setting portion, turn remote on nd do the full throttle full brake thing. After that, config the remote through vesc tool. "Write to vesc"! Do not turn off controller! Disconnect vesc from tool. See if you get controlability. If you do, just remeber you need to calibrate the remote, full throttle full brake thing when you turn it on.
```

---
## \#14 Posted by: brenternet Posted at: 2019-01-06T00:58:11.611Z Reads: 210

```
[quote="J0ker3366, post:7, topic:80043"]
Remote on
Throttle all the way forward
Breaks fully rearward
Release throttle
Throw shitty remote in bin
Buy Mini remote
Turn board on
[/quote]

Fixed this again
```

---
## \#15 Posted by: J0ker3366 Posted at: 2019-01-06T00:59:46.027Z Reads: 208

```
[quote="brenternet, post:14, topic:80043"]
Remote on
Throttle all the way forward
Breaks fully rearward
Release throttle
Throw shitty remote in bin
Buy Mini remote
Have beer
Turn board on
Drool @ the sexiness
Riiiiiide
[/quote]
&lrm; Good?
```

---
## \#16 Posted by: brenternet Posted at: 2019-01-06T01:01:29.426Z Reads: 201

```
I'll take it
```

---
## \#17 Posted by: ADrum707 Posted at: 2019-01-06T01:37:16.563Z Reads: 201

```
I’ve had nothing but great service @ MBoards, just wish their stuff came with more info. Is there any place aside from the forums where one can learn info? The VESC tool is great, but it still leaves so much left unanswered.
```

---
## \#18 Posted by: mmaner Posted at: 2019-01-06T02:06:12.939Z Reads: 199

```
The difference in the motors speed on the bench is irrelivent. They will equal out after they are setup correctly. 

You need to the Motor setup viabthebwizars on both sides of the VESC and the app setup on both sides if the VESC. Once that's done the motors will run fine. Once your ppm detection is done you will have a usable remote. 

This is not a plug and okay device, no VESC's are. You gotta read to find the answers you are looking for. Use the search function, every question you have has likely been asked before. 

[quote="ADrum707, post:1, topic:80043"]
could have now easily paid for a boosted stealth and been just fine.
[/quote]

Send your stuff back for a refund and go buy a boosted board if that's what you want. There's only a few thousand people here that have boosted boards sitting in the corner because they wanted speed and range.
```

---
## \#19 Posted by: Mazda_bater Posted at: 2019-01-06T02:06:43.402Z Reads: 189

```
Gee they have made things seem confusIng. 
Your hardware seems good although I expect you will still have some issues with the limitations on this Vesc.
I always seem to have success programming the second Vesc first if that makes sense. You need to individually connect to both USB ports.
Step 1 connect to Vesc 2 go though motor setup wizard using the motor detection go through app setup wizard configuring it as a slave with an address of 1 now disconnect 
Step 2 connect to Vesc 1 go through motor setup wizard go through app setup wizard configuring it as a master and making sure remote is set to high speed and reading its range here you need to go through the min max and centre by cycling the remote through its range.  Now disconnect and check to see if your board is now performing as expected.
```

---
## \#20 Posted by: ADrum707 Posted at: 2019-01-06T02:11:34.348Z Reads: 182

```
Yeah I didn’t want a boosted board because I knew better speed and range was out there. I appreciate all the feedback and info, I’m still learning and I want to have a legit board, you guys have all contributed such great info! :grin:
```

---
## \#21 Posted by: ADrum707 Posted at: 2019-01-06T02:12:04.013Z Reads: 175

```
I’ll give this a shot! Thanks! :smile:
```

---
## \#22 Posted by: mynamesmatt Posted at: 2019-01-06T03:07:58.876Z Reads: 175

```
[quote="ADrum707, post:1, topic:80043"]
I could have now easily paid for a boosted stealth and been just fine. :rage::rage::rage:
[/quote]

good lord 😂😂
```

---
## \#23 Posted by: ADrum707 Posted at: 2019-01-06T05:09:46.167Z Reads: 174

```
Is the Mac version of the VESC tool actually legit?

per https://github.com/rpasichnyk/vesc_tool/releases

This would make things a whole lot easier if I didn’t have to use a windows machine…
```

---
## \#24 Posted by: Eboosted Posted at: 2019-01-06T05:50:58.756Z Reads: 170

```
[quote="BigBrit, post:8, topic:80043"]
Tbh the nano X is garbage. I have two of them and they are crap
[/quote]

I never liked the Nano X, however after riding the Raptor 2 for so long made me used to it. I don't think it's crap anymore, you get used to the start up calibration and the thumb trigger. 

I even ordered some of them to replace my Mini Remotes as those are imposible to carry because of the weird big size.
```

---
## \#25 Posted by: BigBrit Posted at: 2019-01-06T08:49:20.302Z Reads: 168

```
I'm still using it too out of lazyness and I still think they are rubbish.im used to it but I think for the money they are a poor choice

The batteries on both of them have puffed and I have had to replace them too.
```

---
## \#26 Posted by: ADrum707 Posted at: 2019-01-06T17:33:05.375Z Reads: 171

```
Here are some screen shots - after playing around in the PPM settings, I got rid of the tick and actually got smoother responses from the motors. 

![Motor%20Config|690x404](upload://dPFBKGhCovvAIaiFbN9YnfvHYCP.png) 
![Voltage%20Limits%201|690x400](upload://bs2jMaQ559hW3MTSUmoz14DpCs5.png) 
![Motor%20Parameters%201|690x405](upload://dZe57KoyqPppSzz7JZnSuLMrFNM.png) 
![Motor%20Parameters%202|690x403](upload://6zesJ1KhiVhU6v4B4vLzhD4LrSt.png)
![PPM%20Settings|690x404](upload://xxSnshadI9wDRsETpMgKM59JjUu.png) 

The trick with PPM settings seem to lie in the centering, min, and max settings right there above the VESC Tool status bar. Still confused by all of the acronyms, but it seems to finally be working the way I'd hoped. Now to get it all crammed into the enclosure and take it for a spin. 

I'd still appreciate all of your feedback, and I apologize for the tantrum in the first post. After working 36 hours and still getting nowhere, my brain was fried and my patience was gone. We can all laugh at how silly that was, and I appreciate those of you who mentioned it. :smile:
```

---
## \#27 Posted by: ADrum707 Posted at: 2019-01-06T17:33:48.562Z Reads: 146

```
Oh also, in case anyone is wondering, it seems that the Mac version of the Vesc tool works just fine for this kind of setup. :sweat_smile:
```

---
## \#28 Posted by: ADrum707 Posted at: 2019-01-06T17:54:18.403Z Reads: 146

```
I’m a bit concerned with the differences in my motor parameters. Should I adjust one to match the other, if so, which one should I match?
```

---
## \#29 Posted by: Andy87 Posted at: 2019-01-06T18:00:02.159Z Reads: 150

```
No, don’t change anything.
You made a motor detection and the values you got as results work only for the motor you made the detection with. It’s ok that they different.
```

---
## \#30 Posted by: ADrum707 Posted at: 2019-01-09T16:07:31.431Z Reads: 141

```
First ride with the new setup

![image|230x500](upload://8qHgFHdzRRpzXWhbWi2bx8zWRCT.jpeg)
```

---
## \#31 Posted by: RedBaron Posted at: 2019-01-09T20:20:16.278Z Reads: 127

```
Your max motor amps are super low for having your battery amps at 50a. You can at the very least bring motor amps to 50a and get much better acceleration at low rpm.
 You should also bring your battery regen down from -40 to -15 or -20 per motor. With a dual setup durring braking you could possibly dump 80amps into ur battery damaging it. A 10s5p battery should handle 30a to 40a of regen no problem.
```

---
## \#32 Posted by: ADrum707 Posted at: 2019-01-09T21:00:37.366Z Reads: 129

```
I was actually thinking my brakes were still a little soft.... I definitely don't want to damage my battery though. I weight about 225, 6'0". I lean back pretty hard when I'm braking, that doesn't seem to help. Maybe I've got a bad motor(s) if the braking is still soft? Maybe my belt tension is off? Thanks for your input btw! :grin:
```

---
## \#33 Posted by: mtuan293 Posted at: 2019-01-09T21:21:09.635Z Reads: 130

```
With that motor settings then yeah. I use 60/-60 on my flipsky 4.20 in BLDC no cutouts.
```

---
## \#34 Posted by: ADrum707 Posted at: 2019-01-09T21:25:10.465Z Reads: 125

```
I'm running everything in FOC - does that make a difference? I also have no idea what either acronym means :confused:
```

---
## \#35 Posted by: mtuan293 Posted at: 2019-01-09T21:26:51.534Z Reads: 127

```
The 4.20 have issues in FOC mode. Re calibrate your motors in BLDC and bump the motors current higher.
```

---
## \#36 Posted by: ADrum707 Posted at: 2019-01-09T21:28:03.312Z Reads: 124

```
I honestly thought the 4.20 was a good vesc, but it seems like it's not based on a lot of people thoughts. What's considered to be the better vesc's out there?
```

---
## \#37 Posted by: mtuan293 Posted at: 2019-01-09T21:29:30.717Z Reads: 123

```
I made the same mistake buying this 4.20. I heard their single 4.12 is decent. Also their 6.6s
```

---
## \#38 Posted by: ADrum707 Posted at: 2019-01-09T21:30:39.423Z Reads: 126

```
What about the Foc box? I've heard about that one... is Flipsky the main manufacturer of quality VESC's and the 4.20 was just a lemon?
```

---
## \#39 Posted by: mtuan293 Posted at: 2019-01-09T21:34:23.087Z Reads: 129

```
Focbox is tried and tested and very reliable. Flipsky is the new comer that’s been around maybe half a year. That’s not to say Flipsky sucks, their 6.6 is good according to people on this forum.
```

---
## \#40 Posted by: RedBaron Posted at: 2019-01-09T21:36:07.677Z Reads: 137

```
Give these settings a try and if you still don't like your brakes, you might have to consider a different gear ratio or wheel size. 

Motor max 50a
Motor max brake -50
Battery max 45
Battery regen -15/-20

Those are just starting points, always stay mindful of your electronics capabilities and adjust from there.
```

---
## \#41 Posted by: ADrum707 Posted at: 2019-01-09T21:36:17.331Z Reads: 130

```
Are there any others that I should consider? I feel like I know nothing, and the only way to figure stuff out is to go on what's here in the forum. 98% opinion. haha
```

---
## \#42 Posted by: mtuan293 Posted at: 2019-01-09T21:36:32.918Z Reads: 135

```
If you’re curious about motor amps settings, here’s a post from another topic
[quote="Deckoz, post:5, topic:66705"]
ESC are basically a buck converter. Varying the duty cycle. You can find lots of my posts on duty cycle. But the answer is simple.

Motor Max 120
Battery Max 50
Voltage 54.6

54.6V * 50A = 2730Watts
2730Watts / 120A = 22.75v
22.75V / 54.6V = 41% duty cycle.

So above 41% duty cycle the motor amperage will drop the meet the maximum battery amperage/wattage.

2730W / (54.6V * 42% Duty) = 119A
2730W / (54.6V * 43% Duty) = 116A

And below 41% the motor amperage can be upto 120A. Meaning more power to the ground during acceleration giving you your maximum output potential throughout the entire band.
[/quote]

Basically the maximum power you have is capped by your source (battery), so at low speed when you accelerate, the ESC will control the motor at low voltage and push higher current to give you that torque. Then as your speed increases, the voltage increases and current will drop to maintain that same power because now you don’t need that much torque to keep you moving. I don’t have any EE background but at least that’s what I understand so far.
```

---
## \#43 Posted by: ADrum707 Posted at: 2019-01-09T21:38:32.972Z Reads: 119

```
I've got Orangatang Kegels - I love them, I'd prolly want to change my gearing - but I don't want to lose too much torque, I need it for the hills in my area.
```

---
## \#44 Posted by: RedBaron Posted at: 2019-01-09T21:39:04.938Z Reads: 121

```
From personal experience the flipsky 6.6dual is awesome. It was super easy to set up in foc. Haven't had any issues so far. We'll see how they stand the test of time.
```

---
## \#45 Posted by: RedBaron Posted at: 2019-01-09T21:41:15.924Z Reads: 122

```
You would want to gear for more torque so you would lose top end if I'm not mistaken.
```

---
## \#46 Posted by: ADrum707 Posted at: 2019-01-09T21:48:16.632Z Reads: 122

```
I'd prefer lots of torque with lots of braking power haha :man_shrugging:
```

---
## \#47 Posted by: mtuan293 Posted at: 2019-01-09T21:50:19.685Z Reads: 123

```
For now with your 4.20 you can increase the motor amp max to 60/-60 or even 80/-80. But ready for the cutout in FOC. I don’t have any issues with that setting in BLDC. Also I have a small 10s2p battery. You have a 5p battery which is a huge plus in terms of current drawing and current dumping for brake.
```

---
## \#48 Posted by: ADrum707 Posted at: 2019-01-09T21:51:43.048Z Reads: 120

```
I'm definitely going to switch over to BLDC - what does that and FOC stand for anyway?
```

---
## \#49 Posted by: mtuan293 Posted at: 2019-01-09T21:52:56.808Z Reads: 123

```
FOC is field oriented control. BLDC is brushless DC. Basically means two ways of making the motor spins. Look into the topic I linked above, people have asked about this already
```

---
## \#50 Posted by: ADrum707 Posted at: 2019-01-09T21:54:15.720Z Reads: 120

```
Will do! Thanks! :D
```

---
## \#51 Posted by: mtuan293 Posted at: 2019-01-09T21:57:28.334Z Reads: 122

```
And I see you have Xmatic app which is perfect to see for yourself. Check the Stats tab and see when you accelerate to start moving the current will be high, then it’ll drop as you gain speed.
```

---
## \#52 Posted by: ADrum707 Posted at: 2019-01-09T22:05:37.696Z Reads: 122

```
I do dig the app - although it's pretty different on battery percentage from what my indicator shows.
```

---
## \#53 Posted by: mtuan293 Posted at: 2019-01-09T22:19:51.432Z Reads: 115

```
It’s because the author programs the mapping of % to voltage level different than your volt meter. I remember he said he based it on 30Q discharge curve. At around 36V my volt meter shows 30% while the app shows like 50% or so, is that the same thing for you?
```

---
## \#54 Posted by: ADrum707 Posted at: 2019-01-09T22:21:05.991Z Reads: 113

```
Nearly identical actually. Is the other indicator I'm using more accurate?
```

---
## \#55 Posted by: mtuan293 Posted at: 2019-01-09T22:29:52.763Z Reads: 115

```
I don’t think so. Most voltmeters are the same if you look at ebay or amazon. But you have the app and reading from your vesc, that’s enough for me lol
```

---
## \#56 Posted by: mtuan293 Posted at: 2019-01-09T22:32:25.072Z Reads: 116

```
Just don’t drain past 3.0V per cell (30V in your case) and you’re good. Critical point is 2.5V. I made a mistake and destroyed mine :|
```

---
## \#57 Posted by: Deckoz Posted at: 2019-01-09T22:47:13.122Z Reads: 121

```
yep basically. Thats just the outline of max power potential. Real world load, has alot more factors and typically no where near the max load

typically the only times you will ever see max or close to max load is 0-10mph digs in wide open throttle, and 30mph+ wind resistance requiring more wattage.

While going WOT at 10-30mph typically significantly less watts then 0-10mph or 30+. 

All in all motor amps just give low duty - high wattage capability to put more power to the ground earlier in the throttle curve.

lol we just had a build poll of best of 2018... if there was a poll for best knowledge acquired in 2018, it would have to be esk8 community finally knowing what duty cycle does...

/thanks deckoz lol 🤔
```

---
## \#58 Posted by: ADrum707 Posted at: 2019-01-09T22:54:58.540Z Reads: 117

```
That's what the cutoffs are for right?
```

---
## \#59 Posted by: mtuan293 Posted at: 2019-01-09T23:03:50.820Z Reads: 115

```
Yes. And the BMS too. But I bypassed my bms for charge only and left the board turned on overnight. I finished charging and turned it on to check voltage with Xmatic, then forgot to turn it off lol
```

---
## \#60 Posted by: mtuan293 Posted at: 2019-01-09T23:07:12.584Z Reads: 118

```
There’s a lot of abstraction that powers our everyday lives and I don’t think many people really care about/interested in how things work under the hood lol. However our community is still a lot more knowledgeable than the average consumers lol. I’ve seen people asked about what to do when belts snap on Boosted subreddit :rofl:
```

---
## \#61 Posted by: ADrum707 Posted at: 2019-01-10T00:03:28.517Z Reads: 113

```
Yeah - I really do appreciate the attention to detail that most folks on here seem to have, they pay attention to the smaller details. Those boosted board people also prolly have never changed their own oil, or know how to wash their car by hand. hahah :rofl::rofl::rofl:
```

---
## \#62 Posted by: mtuan293 Posted at: 2019-01-10T00:16:03.521Z Reads: 115

```
Also abstraction is the tool for business to make more money. After being here for a while you’ll realize that the Mini S, Mini X and Stealth all have the same hardware, just different firmware so that it locks down speed and power
```

---
## \#64 Posted by: Andy87 Posted at: 2019-01-10T19:13:58.512Z Reads: 111

```
Besides the e-switch and the wrong voltage readings
```

---
## \#65 Posted by: mtuan293 Posted at: 2019-01-11T00:10:57.588Z Reads: 110

```
Yeah e-switch is a rip off of Martinsp’s. I purchased the switch from him instead of Flipsky
```

---
## \#66 Posted by: Andy87 Posted at: 2019-01-11T03:44:53.119Z Reads: 107

```
I mean the build in e-switch.
```

---
## \#67 Posted by: ADrum707 Posted at: 2019-01-13T16:44:46.558Z Reads: 108

```
BLDC Settings:

![New%20Motor%20Settings%20BLDC|690x405](upload://zqdP49QeeKmPSlDoUMvPnyA7Vqx.png)
![Cutoff%20limits%20BLDC|690x407](upload://lrbsfMHwznkDg7u9VfTiv6l1yLc.png) ![BLDC%20Settings|690x404](upload://g7N1xYOJ0ApTDT8FA6UWfAXtpXu.png)  

Backed down the battery regen so I'm not risking dumping too much back into it at once. 
We got 6 inches of snow here last night, so I'll have to wait for it to melt down before I can test the new settings.
```

---
## \#68 Posted by: DeathCookies Posted at: 2019-01-13T18:30:53.986Z Reads: 101

```
[quote="mtuan293, post:35, topic:80043"]
The 4.20 have issues in FOC mode
[/quote]

[quote="ADrum707, post:36, topic:80043"]
I honestly thought the 4.20 was a good vesc, but it seems like it’s not based on a lot of people thoughts.
[/quote]


Flipsky does not get much good reviews on this forum.
My Dual FlipskyVesc 4.20 runs perfectly strong in FOC even from standstill. but i did not test max speed yet on that board though.
```

---
## \#69 Posted by: mtuan293 Posted at: 2019-01-13T19:31:56.919Z Reads: 98

```
What’s your setup? Do you have cutout issues?
```

---
## \#70 Posted by: DeathCookies Posted at: 2019-01-13T20:20:49.115Z Reads: 96

```
Dual 270 kv, 10s2p
It is a spare Board. Did not ride much with it but no cutouts so far
```

---
## \#71 Posted by: mtuan293 Posted at: 2019-01-13T21:43:58.868Z Reads: 97

```
That sounds exactly like my setup. Are those 5055 diyeboard motors?
```

---
## \#72 Posted by: DeathCookies Posted at: 2019-01-13T22:04:17.584Z Reads: 96

```
jup, thats correct
```

---
## \#73 Posted by: mtuan293 Posted at: 2019-01-13T22:49:57.628Z Reads: 95

```
How come you don’t have cutout issues? What’s your settings? Have you tried pull full throttle for brake?
```

---
## \#74 Posted by: DeathCookies Posted at: 2019-01-14T08:38:14.479Z Reads: 93

```
[quote="DeathCookies, post:70, topic:80043"]
Did not ride much with it but no cutouts so far
[/quote]

Mhm.... No aggressive Riding with this spare Board yet.
```

---
## \#75 Posted by: Mazda_bater Posted at: 2019-01-14T21:21:21.297Z Reads: 91

```
My flipsky vesc 4.2 dual runs great in foc too, it's only fault is that when it is stressed rather than throttling the output the vesc resets. Most people get on my board with it and find it runs great. 

To me the vesc resets aren't acceptable. 
Although when I look at the history of vesc people have tolerated worse behaviour than I've experienced from other vesc
```

---
## \#76 Posted by: mtuan293 Posted at: 2019-01-15T08:19:10.783Z Reads: 89

```
Well mine run just fine in FOC if I ease on the throttle. However my area has a lot of hills and I fell a few times when it cut out on me while braking. Was not going fast btw, like 5mph
```

---
## \#77 Posted by: DeathCookies Posted at: 2019-01-19T14:59:52.433Z Reads: 88

```
Same for me.
I did a couple Tests and couldnt cut out the dual vesc by slamming the throttle. The only time i get a cut out is when i drove over gravel and my wheel spin through. Even at 10a battery at each vesc.
```

---
## \#78 Posted by: Bjork3n Posted at: 2019-01-19T15:36:14.282Z Reads: 90

```
Dude, you didnt even do the motor detection in the video?
And you need to split the battery max between the two vesc.
You just set your vescs up to draw a total of 120A from the battery... Battery is rated for 60A.

People dont follow this guide.
```

---
## \#79 Posted by: MatrixWriter Posted at: 2019-01-22T00:49:46.411Z Reads: 89

```
It's sensorless motor, so no motor detection is needed and is mentioned in the title.

I did make a mistake about the battery current max since it is combined, I did put a note about it for others to lower it - of course it depends on the battery you use. The other parts of the video and information is correct and accurate.
```

---
## \#80 Posted by: Bjork3n Posted at: 2019-01-22T04:43:31.228Z Reads: 91

```
Motor detection is not done for the sensors primarily (Sure it will detect the sensor config in bldc..). You do motor detection to calculate the motors resistance and to make it run as it should. 

Even if you don't use sensors you still need to do the detection in vesc tool.
```

---
## \#81 Posted by: MatrixWriter Posted at: 2019-01-22T06:57:29.896Z Reads: 86

```
Ah, good to know. I will redo the video as esp. I do not want to feed bad information.

Thanks for your feedback!
```

---
## \#82 Posted by: ADrum707 Posted at: 2019-05-26T23:41:55.601Z Reads: 66

```
Hey there guys! It’s been a few months, but I’m back at it trying to get my board figured out. My wife and I had a baby, that took up all of my time and still for the most part is. 

I’ve finally got a decent suspension and rear axle on the thing, and so it’s back to programming. 

I’ve tried a few different settings and the issues I’m having seem to be:

1.) Next to no power during standing or single push take offs 

2.) Once the motors do take off, they run fast and hard for a second or two, then cutoff and jolt pretty hard

3.) Incredibly hard braking while rolling at high speeds 

OR

reasonable braking at normal speeds, but next to no braking at low speeds. It’s either one or the other. 

4.) The motors don’t seem to pull evenly, one seems to be more responsive than the other even though they’re programmed using the same Vesc tool and same settings (not matched settings, just same set up steps) 

Where/how should I start trouble shooting this?
```

---
## \#83 Posted by: Gamer43 Posted at: 2019-05-27T00:28:49.116Z Reads: 60

```
Are the motors sensored? Also when was the 4.20 purchased? There was a minor hardware change starting March 27th that greatly improved the performance of the 4.20.

What kind of motors are you using (KV rating) and are you running Trapezoidal (BLDC) control or FOC? 

If you could post a picture of both motor and app config settings that would be helpful for troubleshooting.

If you tinkered with the advanced motor settings, that would also be helpful.
```

---
## \#84 Posted by: ADrum707 Posted at: 2019-05-27T00:35:35.579Z Reads: 62

```
The motors are sensorless, and I didn’t know about the update, I’ll have to figure out how to do that as well. (Never updated the firmware before) they are 180kv motors and I’m using FOC setup wizards. I barely understand basic settings, I’d prolly destroy it in the advanced settings lol  but I will definitely post some screen shots later on this evening. Any tips on updating the firmware?
```

---
## \#85 Posted by: Gamer43 Posted at: 2019-05-27T00:40:36.230Z Reads: 62

```
How good are you with a soldering iron? The change was relatively simple, swap out the existing gate resistors for 47 ohm resistors, they are in an 0603 package. Refer to this thread for an explanation https://www.electric-skateboard.builders/t/flipsky-4-20-a-explanation-to-the-mystery-and-how-to-stop-the-cutouts-entirely/87824?u=gamer43.

Basically, problem number 2, the cutouts, is solved by this hardware modification. The ESC can take up to 65 motor amps no problem after the change (there's still a __possible__ dead-time issue, but that has yet to surface on this forum).

If you need any other clarifications please let me know. 

No matter what you do, performance is going to suck at low speeds without sensors. There are some advanced settings to could tinker with to get a marginal improvement, depending on up to what speed the poor performance continues into. 

Normally, just increasing the switching frequency from the default 20khz to 25khz seems to help a lot. (this is an advanced FOC setting). 

The wacky throttle response will need some tuning with current settings and ramping time in app config.
```

---
## \#86 Posted by: ADrum707 Posted at: 2019-05-27T02:04:53.995Z Reads: 52

```
Oh man I’m no good with a soldering iron I might have to have a friend do it for me...

Maybe I misunderstood - it’s a hardware thing, not a firmware thing? Or is it both? 

Sounds like you’re THE guy for this particular VESC. Does the hardware upgrade apply to the dual version as well?
```

---
## \#87 Posted by: Gamer43 Posted at: 2019-05-27T02:35:15.423Z Reads: 48

```
Just hardware. It applies to all FSESC 4.20 single and dual shipped after March 27.
```

---
## \#88 Posted by: ADrum707 Posted at: 2019-05-27T03:13:12.207Z Reads: 45

```
If I can’t do that upgrade immediately, do I risk damaging the VESC?
```

---
## \#89 Posted by: Gamer43 Posted at: 2019-05-27T03:27:56.946Z Reads: 41

```
Nah, but you risk damaging yourself unless you opt for extremely conservative settings.
```

---
## \#90 Posted by: ADrum707 Posted at: 2019-05-27T03:34:43.638Z Reads: 43

```
Haha, I can be conservative - it’s worth waiting if this is a major upgrade. Any recommendations on where to get the new resistors from?
```

---
## \#91 Posted by: ADrum707 Posted at: 2019-05-29T14:45:53.131Z Reads: 41

```
So I updated the Vesc tool, and the firmware on the dual vesc, ran FOC detection, and here are my results. I'm much happier with how the board accelerates now, the brakes are pretty stiff though. They don't ease in like I wish they did. Any recommendations on how I can soften them up a bit? They do come to a good hard stop, and hold, but it's like throwing a brick in front of the wheels at high speeds. Doesn't exactly inspire confidence...

![New%20Update%20specs|296x350](upload://Hl8XhA9Q33Xh6KxFKZyeV4BsQP.png)
```

---
## \#92 Posted by: Gamer43 Posted at: 2019-05-29T15:02:46.711Z Reads: 42

```
Maybe try a throttle curve on the negative side? If that doesn't work you could try lowering the braking current.
```

---
## \#93 Posted by: ADrum707 Posted at: 2019-05-29T15:04:37.888Z Reads: 41

```
I'm a total noob, lol I don't know how to do either of those things :blush:
```

---
## \#94 Posted by: Gamer43 Posted at: 2019-05-29T15:11:05.957Z Reads: 41

```
Oh no wonder the braking is so aggressive, I'm guessing you are using the current limits VESC tool set for you? It sets unreasonably high currents for some reason. You can find these settings in the motor configuration tab, under general, it should be the first tab.
```

---
## \#95 Posted by: ADrum707 Posted at: 2019-05-29T15:17:54.305Z Reads: 43

```
![VESC%20tool%20motor%20settings|690x442](upload://l0wRSXdfJ7S1Nk7OsihIoRpf9kf.png) 

Am I in the right ball park at least?
```

---
## \#96 Posted by: Gamer43 Posted at: 2019-05-29T15:18:59.934Z Reads: 40

```
Yes, that's exactly the parameter I was talking about. Lower it to a value to feel comfortable with.

The throttle curve I was talking about,  that can be found in the app config tab, under general.

Might be better to adjust the throttle curve instead so you still have full braking if you pull all the way back.
```

---
## \#97 Posted by: ADrum707 Posted at: 2019-05-29T15:25:08.341Z Reads: 39

```
So the throttle curve would also affect the braking? Interesting... which parameter am I looking for here? Additionally, when you mentioned I could "lower it" - that value is negative. By lowering it, would I be adjusting to -50? or would lowering it be like -35? Hope that makes sense...

![vesc%20tool%20app%20config%20throttle%20curve|690x441](upload://k6QaNkHayKDbwdxW7x46mZcrTG6.png)
```

---
## \#98 Posted by: Gamer43 Posted at: 2019-05-29T15:26:37.996Z Reads: 39

```
Okay, my bad I think it is actually under ppm. Adjusting it is weird, you select a curve and a scaling factor. Fortunately, it provides a graph of what the curve looks like.

You can adjust acceleration and braking independently actually.
```

---
## \#99 Posted by: ADrum707 Posted at: 2019-05-29T15:37:24.843Z Reads: 37

```
Found it, looks like all the values were set to 0. I'm sorry for all the questions, I just feel so lost with all of this lol

![vesc%20tool%20app%20config%20throttle%20curve|690x443](upload://wghzaChUpMePyhEpmIqEYlbGZhA.png)
```

---
## \#100 Posted by: ADrum707 Posted at: 2019-05-29T15:38:51.327Z Reads: 40

```
Also, once I set it in the app, how do I transfer those settings to the VESC, and will it apply to both sides? The FOC motor setup thing does it all automatically...
```

---
## \#101 Posted by: Gamer43 Posted at: 2019-05-29T15:40:21.335Z Reads: 42

```
Along the right side, hover over the icons until one of them reads "write motor config" and "write app config". Clicking them will update the settings on the controller if the controller is connected to vesc tool.

As for applying to both sides I'm not sure. I never messed with it because the CAN feature of the VESC is rife with bugs. (Maybe it was fixed in the last firmware update, I'm running all mine on older firmware)
```

---
## \#102 Posted by: maddec Posted at: 2019-05-29T15:42:09.557Z Reads: 43

```
Are you using the Flipsky remote via UART? I had a similar issue with Dual FSESC 4.20 Plus.
If you are using this setup you have to run the configuration of the motors before connecting the receiver.
```

---
## \#103 Posted by: ADrum707 Posted at: 2019-05-29T15:42:51.221Z Reads: 47

```
Thanks man! Should I be going negative or positive on the curve with the percentage adjustments? It feels like an advanced level math course haha
```

---
## \#104 Posted by: Gamer43 Posted at: 2019-05-29T15:43:30.955Z Reads: 46

```
Cant remember, sorry, whatever value makes the curve flatter around 0.

And just to be sure, I would update both sides through USB to make sure they have updated settings.
```

---
## \#105 Posted by: ADrum707 Posted at: 2019-05-29T15:44:26.845Z Reads: 44

```
No I'm using this remote: https://www.mboards.co/collections/remotes/products/remote-controller-1

I'll have questions about how to set "ride modes" on this thing later. It has a switch that seems to affect it's behavior in the input wizard, but idk how to make those changes the way I want yet.
```

---
## \#106 Posted by: ADrum707 Posted at: 2019-05-29T15:49:57.247Z Reads: 45

```
I'll try this setting, and as soon as I unplugged from one side and tried to plug into the other side, my usb connector broke off the VESC... I hope I'm not screwed! :weary::weary::weary:![vesc%20tool%20app%20config%20throttle%20curve%20setting%20test%201|690x442](upload://zsBSklLFnmQJeloquv6h91oT4O3.png)
```

---
## \#107 Posted by: Gamer43 Posted at: 2019-05-29T15:52:17.672Z Reads: 43

```
I think updates over CAN are possible, not sure how, though. The other option is to bodge wire a new USB connector. Flipsky had issues with soldering their USB connectors on earlier batches. It seems to be better now.

Ironically enough, the massive ground planes they have in the ESC to improve performance inadvertenly caused cold joints on the USB connector's anchors, so they wouldn't anchor properly. I think they changed their reflow profile or added thermal reliefs to fix that.
```

---
## \#108 Posted by: ADrum707 Posted at: 2019-05-29T15:59:32.838Z Reads: 40

```
I might not have a choice but to buy a new one... the resistor thing seems really difficult. and then re-attaching the USB connector seems even more daunting lol
```

---
## \#109 Posted by: Gamer43 Posted at: 2019-05-29T16:00:41.770Z Reads: 41

```
The USB connector will be easier than the resistor swap. I can tell you from experience xD.
```

---
## \#110 Posted by: ADrum707 Posted at: 2019-05-29T16:04:46.268Z Reads: 43

```
Are you stateside? If I shipped you my stuff could you perform the USB connector repair and the resistor swap?
```

---
## \#111 Posted by: Gamer43 Posted at: 2019-05-29T16:07:43.481Z Reads: 44

```
I am, but the moment I start soldering something thats for someone else I'm gonna make it explode DX.

I'd be willing to do the change for you no charge if I am not financially responsible if it stops working :).
```

---
## \#112 Posted by: ADrum707 Posted at: 2019-05-29T16:15:44.728Z Reads: 42

```
Sounds good, I'll private message you for the details :)
```

---
## \#113 Posted by: ADrum707 Posted at: 2019-05-29T16:17:19.738Z Reads: 44

```
I found a button on the right side of the VESC tool that says "forward communication over can bus" -  do you think if that button is engaged, it will apply changes to both VESC's?
```

---
## \#114 Posted by: Gamer43 Posted at: 2019-05-29T16:17:46.971Z Reads: 44

```
Actually, @JohnnyMeduse a.k.a DRV wizard does VESC repair, he can do this reliably, but not sure how much he would charge for this.
```

---
## \#115 Posted by: Gamer43 Posted at: 2019-05-29T16:18:01.601Z Reads: 42

```
I think the forward communication would.
```

---
## \#116 Posted by: ADrum707 Posted at: 2019-05-29T16:19:03.453Z Reads: 41

```
Cool, I'll reach out to him as well! :) Thanks man!
```

---
## \#117 Posted by: ADrum707 Posted at: 2019-05-29T16:44:44.554Z Reads: 42

```
Update: 

The effects at -25% on the curve were noticeable, but I still wanted a little more ease into the brakes. I moved it to -50% and that's way more comfortable for me. Might go even more to 65% but that will have to wait until either late tonight or early tomorrow. I'll post another update if I make another change! :)
```

---
## \#118 Posted by: Mainsedora Posted at: 2019-05-29T17:34:57.247Z Reads: 41

```
Don't forget to adjust the Battery Current Max Regen to -15 per VESC to  prevent any battery dmg. And that value is responsible for the braking strength of your board.
```

---
## \#119 Posted by: ADrum707 Posted at: 2019-05-30T04:06:54.932Z Reads: 42

```
@Gamer43 

I rode the board quite a bit today. -50% on the curve still doesn’t seem like enough for some of the hills in my area. If I keep adjusting that curve beyond 50% am I losing performance anywhere else or risking damage to another component? 

I also noticed a few cutouts on my brakes and takeoffs - even rolling takeoffs I had cutouts. Will the resistor swap completely eliminate that? 

I don’t want to keep bugging you with every VESC tool and VESC question I come up with, unless you’re okay answering them. If not, is there a resource you’d recommend that taught you about this stuff?
```

---
## \#120 Posted by: Gamer43 Posted at: 2019-05-30T04:20:32.853Z Reads: 43

```
Increasing the throttle curve even more shouldn't cause harm, set to whatever you are comfortable with :).

And yes, the resistor swap will eliminate the cutouts entirely.
```

---
## \#121 Posted by: BillGordon Posted at: 2019-05-30T04:53:08.514Z Reads: 47

```
I had cutouts at anything over 35 motor amps on the early faulty 4.20s. I kept them at 30 most of time. Bit boring, but it worked.
```

---
## \#122 Posted by: ADrum707 Posted at: 2019-05-31T00:40:55.512Z Reads: 41

```
Today’s update: 

I rode at -75% on the throttle curve. Much smoother braking might even go higher!

I ran into a new sound though, the motor sounded like it squealed when I hit the brakes at one point, then took a second or two before they’d re-engage and then the throttle forward kicked on hard and didn’t release with the controller... seemed odd. Is that another resistor issue? Could I have motor damage and not know it?
```

---
## \#123 Posted by: Gamer43 Posted at: 2019-05-31T03:03:58.655Z Reads: 40

```
Sounds like a remote issue, what remote are you using?

Or a CAN bus issue. I personally avoid using CAN. So many, many things are done wrong with CAN on the VESC.

It's a miracle CAN even works.
```

---
## \#124 Posted by: Blasto Posted at: 2019-05-31T03:09:26.570Z Reads: 40

```
[quote="Gamer43, post:123, topic:80043"]
Or a CAN bus issue. I personally avoid using CAN. So many, many things are done wrong with CAN on the VESC.
[/quote]

Interested to hear your take on this, the lack of protection and filters?
```

---
## \#125 Posted by: ADrum707 Posted at: 2019-05-31T03:24:57.521Z Reads: 39

```
This is the remote I’m using:
https://www.mboards.co/collections/remotes/products/remote-controller-1 

I’d much prefer to use something like this instead:
https://www.mboards.co/collections/remotes/products/remote-for-esc

I like that the 2nd remote shows battery life as well as offers different “ride modes” and has a reverse button. My current one is suppose to have a reverse button but it doesn’t work at all. 

Are there better remotes out there I. This small form factor?
```

---
## \#126 Posted by: ADrum707 Posted at: 2019-05-31T03:25:46.711Z Reads: 37

```
I’m also curious how to operate a dual VESC with no canbus...
```

---
## \#127 Posted by: Gamer43 Posted at: 2019-05-31T03:48:30.393Z Reads: 39

```
[quote="ADrum707, post:126, topic:80043, full:true"]
I’m also curious how to operate a dual VESC with no canbus…
[/quote]
split PPM with ORing diodes. If you want, you can drop the oring diodes and just send the PPM signal to both ESCs.

[quote="Blasto, post:124, topic:80043"]
> Or a CAN bus issue. I personally avoid using CAN. So many, many things are done wrong with CAN on the VESC.

Interested to hear your take on this, the lack of protection and filters?
[/quote]

well, first of all, CAN needs shielded twisted pair otherwise you get bit-errors galore (especially in this environment).
I remember reading multiple applications notes saying the CAN-H and CAN-L lines need protection diodes to the positive and negative rails (especially since these devices are used with LOWSIDE switches).
Third, CAN is not UART, so data should not be transmitted on the bus as if it were UART, you'll get bus contentions. 
The way the termination resistors are set up only allows for two devices to be on the bus. 
I have more qualms but can't think of them off the top of my head right now.

If it were fault-tolerant CAN, then maybe this whole setup would be partially forgiven. 

I seriously don't understand why communication wasn't done with I2C in the first place......
```

---
## \#128 Posted by: ADrum707 Posted at: 2019-05-31T14:54:57.900Z Reads: 38

```
If this is a can issue, would it present in a fault code? 

I was out riding this morning with the curve now set to 100% - might sound crazy but hey I like brakes that ease in - I happened to look down when I heard my motor making that sound again.

Only when I apply the brakes after extended throttle times do I notice it. I saw the one motor wasn’t moving at all.
```

---
## \#129 Posted by: Gamer43 Posted at: 2019-05-31T17:30:22.839Z Reads: 36

```
Not sure if the firmware even detects CAN faults. 

I would check to see if each esc and motor works independently using the remote. If they both work fine by themselves, then CAN is the issue.
```

---
## \#130 Posted by: ADrum707 Posted at: 2019-06-16T02:23:20.853Z Reads: 32

```
It’s been a few weeks since my last post - in that time I shipped my VESC to @JohnnyMeduse aka the DRV Wizard, he repaired it and upgraded the resistors in less than 48 hours and return shipped it to me. The whole process took less than 2 weeks time and that included international shipping (USA —> Canada).

I can not express how incredibly happy I am with the services he offered and delivered on! He was responsive, kind, and immediately began working as soon as my order was delivered. He kept me updated every step of the way, and promptly shipped it back when the work was finished! Service like that alone is worth every penny I paid. 

I was able to get the board together, programmed, and tested tonight and the results are incredible. Better all around response from the motors, both acceleration, and braking! By far the best esk8 experience I’ve had yet since I started my build over a year ago! I can’t thank @JohnnyMeduse and @Gamer43 for recommending him enough! 

If your VESC has a problem, give the DRV Wizard a shout! :smile:
```

---
## \#131 Posted by: Gamer43 Posted at: 2019-06-16T03:12:25.744Z Reads: 30

```
Glad we could help :).
```

---
