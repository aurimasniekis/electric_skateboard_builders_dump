# Is 245kv motor good enough for e-mountainboard? 6S setup, 9inch wheels, 210lbs

### Replies: 39 Views: 5090

## \#1 Posted by: Okami Posted at: 2016-06-01T10:39:50.247Z Reads: 342

```
Hello there! Im quite new here, althrough been reading quite a lot lately about all the different nooks and crannies involved in building one.

I'm planning on building e-mountainboard, _mono drive, with 6s batteries and probably FVT 120A controller._ 

What im not so sure about yet is - which motor should I take?
----------
Right now, I am mostly convinced I should be good with Turnigy Aerodrive **SK3 - 6364-245kv**.

I would aim for **19mph (30kph) speed**.

I am 210 pounds (95kg), not that tall (5.74 ft / 1.75m) and the wheels are probably going to be the 9inch ones. Regular skate trucks unfortunately, the board is going to be Scrub  Silver Reef Series II. I'm also living in quite flat area. The only sort of ''hills'' would be the very low slope of some of the bridges. 
 

As I am not the lightest guy on earth, would like to know if the power rating for e-mountainboard is enough or I need even lower kv rating motor.


----------

If this is somewhere already discussed, I would be glad to reach that resource, because as of right now I am kind of troubled, because for longboards people tend to use 1:3 gear ratio, but for mountainboards it tends to be as high as 1:5 or so. 

So yeah, any help would be great, as I would like to build a board which is capable of pushing me forward, at the same time being able to reach the earlier mentioned 19mph / 30kph.

If you got any other great recommendations for what motors to choose from, I would be greatful.

The only alternative I've found right now is the tacon ones, althrough also seems hard to source them. Plus, can someone direct me to a resource which deals with how much impact has the lenght of the motor?
```

---
## \#3 Posted by: Okami Posted at: 2016-06-01T13:19:56.622Z Reads: 318

```
Thanks for the input. Uh, yeah I know that the extra weight im having is no good.. 

Still have to find a good 10s-12s controller then.. since Im not so sure now then... what should my aims should be, relating to the overall specs of the board..

I hoped I could get away with 6s Esc and 6s battery setup.. It will drive the cost quite high, if I choose to go with the 10s or 12s setup.

I have a plan that I should probably upgrade to dual setup some time later, so if it would not work out that good I would probably scrap the idea about the 6s setup.. But right now unfortunately im just willing to build a ''start'' setup to try things out.. If I would be willing to spend much more money on the build, I would probably go with 10s.. It's just a shame that these controllers cost close to 150$ and that to increase battery from 6s to 10s, also cost extra.

Anyways.. thanks for the suggestion to go with 190kv
```

---
## \#4 Posted by: psychotiller Posted at: 2016-06-01T13:30:08.166Z Reads: 300

```
I weigh 200 (sometimes 220 haha) this board in the video is 6s with a 245kv Tacon on pneumatics, geared 17t/42t...
This whole "low kv/high voltage thing" is pretty much bullshit. As long as you run an ESC that can handle the amps you'll be fine! 
https://www.youtube.com/watch?v=8Ri5eswBeq0
```

---
## \#5 Posted by: Okami Posted at: 2016-06-01T13:32:56.711Z Reads: 294

```
Great, someone with 6s setup and 245kv. 

There seems to be a confusion between how much torque you really need for the job..

 As I am planning to use it mostly on streets or hard packed trails (no sand or any other soft ground) and almost no hills or inclines, then the question remains the same - how low should I go with the kv rating.. because you can easly adjust that with pulley ratios.
```

---
## \#6 Posted by: psychotiller Posted at: 2016-06-01T13:37:12.330Z Reads: 280

```
Right! My advice though with 9" wheels is to make sure you get your gearing right. I run 6" wheels so usually I gear at 14t/60t. you'll probably want bigger gears. Also, when you're ready get a second motor and you'll be good to go on rougher terrain.
```

---
## \#7 Posted by: Okami Posted at: 2016-06-01T13:39:10.191Z Reads: 283

```
Yeah, I already ''played'' with the calc. I have not made my mind on what the final gearing will be, since the board has not arrived yet and Im not sure how big wheel pulley I can fit onto the wheel. But Im confident that I can adjust later the torque / speed proportion, if needed.

Btw - what is the max speed you get out of your thing? The calc shows only like 25kph / 16mph. Have you tested how fast does it go? 
<img src="/uploads/db1493/original/2X/8/81993e37a500d4b258f6c47e0e177dfcefaad328.png" width="370" height="457">

Plus, - can you give info on what size should I take? I see some people using 50 motors.. The only difference I dont like is that the shaft size is 6mm, instead of 8mm as 63's have.
```

---
## \#8 Posted by: psychotiller Posted at: 2016-06-01T14:21:00.887Z Reads: 263

```
My 6 inch wheels are 150mm. 

Yours would be 229mm and it's going to change your top speed as well as efficiency

You'll need a 63mm motor for sure. 8mm shaft
```

---
## \#9 Posted by: treenutter Posted at: 2016-06-01T15:03:20.764Z Reads: 257

```
[quote="Okami, post:1, topic:4106"]
9inch ones
[/quote]

@Okami most of the mountainboard wheels I know of are standard 8", is that what you mean? I think that most here believe that as wheel size increases, you need to aim for greater reduction ratios and higher KV in order to get good torque. But as @psychotiller points out, if your ESC can handle high Amps this is less critical.

My build is in-between an e-mountainboard and standard build, with 5 inch pneumatics (127mm). I use 14/60, with the same motor you're planning to use, an SK3 6364 245KV at 8S. I weight 150 pounds and this build eats hills and easily exceeds your desired top speed. 

If you can, I'd suggest VESC and 8S or 10S. I'm sure 6S will be enough to get you around, but I also think that you'd enjoy the extra power when you need it or want it.

Regarding the calculators and top speed, I find that they provide a rough guide and real-world speeds are much higher. According to the calculators, my top speed should be 18MPH, but I regularly get to 21.5 MPH and that's with the RPM capped to limit speed! If it I uncap it, I'm sure I'd hit around 25MPH or faster.

http://www.electric-skateboard.builders/t/the-village-build-s9-faultine-paris-195mm-sk3-6764-diyes-mount-8s-vesc-127mm-pneumatic-wheels/292
```

---
## \#10 Posted by: Okami Posted at: 2016-06-01T15:17:38.577Z Reads: 238

```
Thanks for info. Will take a look around. Yes, I've been thinking about the VESC as many others have did before me haha.. but for now it seems I would stick with some controller capable of 6s.. till my budget gets bigger and I get the real feel of what I expect from the e-board..

[quote="treenutter, post:9, topic:4106"]
most of the mountainboard wheels I know of are standard 8",
[/quote]

I still have to receive my board but I was also impressed that it originally comes with 9 inch tires and im not sure if the previous guy has changed anything. Although, it do come with 5 bolt rims, so it may 8in after all.

[quote="psychotiller, post:8, topic:4106"]
You'll need a 63mm motor for sure. 8mm shaft
[/quote]

Yeah, you are not the first one to tell me this.. Although, it is a hard choice, since it can make 50 usd difference, If I order 5065-236kv or 6374 - 192kv and I still got to order quite many other parts, so these 50 usd do make a difference, especially because import tax may be added, if I take the more expensive one - 6374.

Plus I'm still not sure should I take 192kv or something like 240kv, because of the bigger wheels I might got for my board.
```

---
## \#11 Posted by: psychotiller Posted at: 2016-06-01T15:50:49.623Z Reads: 212

```
Think of it this way. You can go the cheaper way now, but your board will most likely suck. So, in the end, after you spend a smaller amount of money on parts you won't want to use, you'll end up spending more money on the parts you needed in the first place.

Also, don't get a vesc. It cant handle the amps you are going to pull with that wheel size. Get an EZrun max 6 or max 5.
```

---
## \#12 Posted by: Okami Posted at: 2016-06-01T15:55:16.458Z Reads: 208

```
[quote="psychotiller, post:11, topic:4106"]
EZrun max 6
[/quote]

Yes, I see your point there.. 50 bucks wont matter that much in the long run.. if after, say 2-3 months, I will want something better.. but will have to adjust everything to fit the new model.. 

Yeah, VESC amp ratings seem to be a little bit troublesome, but a lot of people do use it despite this limitation.. which of course is greatly outweighted by the options VESC offers.. I suppose it works Ok in Dual setup, though.

Will take a look at these EZ controllers, I heard of them but could'nt get a working link where to buy them yet.. 

As said before, my initial plan was to use FVT 120A.. but the very chinese origin and look, do gives a thought that it may burn up at some point..
```

---
## \#13 Posted by: psychotiller Posted at: 2016-06-01T16:01:15.778Z Reads: 191

```
The vesc is amazing if you're not pulling a ton of amps. Nobody getting outstanding results with the vesc is running a single drive setup on 9" pneumatics. Nobody. 

Trust me. None of the programming benefits of the VESC will matter to you. Because you'll burn it out on your first ride.
```

---
## \#14 Posted by: Okami Posted at: 2016-06-01T16:04:26.947Z Reads: 189

```
Ok, thanks for advice. Was not aiming for it yet, anyways.. I hope that someone makes another (higher amp) version some time in the future, for the ones more power hungry :) 

I am well aware of the cogging and high amp draw during start up.. so I have already accepted the idea of kick starting the board.. but there's still some long road to take till I get a working board.. so will see :)

Someone should make a diagram of the wheel sizes, rider weights, suitable motors etc.. haha.. that would make it a lot easier.. to figure out the best config :)
```

---
## \#15 Posted by: psychotiller Posted at: 2016-06-01T16:05:06.199Z Reads: 180

```
Alright good luck!
```

---
## \#16 Posted by: Okami Posted at: 2016-06-01T16:07:10.974Z Reads: 186

```
Thanks.. although, you still did not reveal how fast your board goes(?)

I hope this is not some kind of insider secret. for those who cannot reach 40kph to be proud enough, as many boards I suspect reach the earlier mentioned 30kph and are totally happy with that.
```

---
## \#17 Posted by: psychotiller Posted at: 2016-06-01T16:09:30.617Z Reads: 178

```
Oh! It goes a lot faster than 40kph. I changed my gearing to 12/60 and it will cruise at 32mph (50kph?)
```

---
## \#18 Posted by: treenutter Posted at: 2016-06-01T16:11:03.469Z Reads: 186

```
[quote="psychotiller, post:11, topic:4106"]
Also, don't get a vesc. It cant handle the amps you are going to pull with that wheel size. Get an EZrun max 6 or max 5.
[/quote]


I'm sure the EZrun max 5or 6 will work perfectly, and I certainly value all of @psychotiller's advice since he's helped me a ton! 

But I think that VESC would be able to power a build like this really well, especially if 8S or 10S is used instead of 6S.

Trampa and Scram are using VESC on their lines of complete e-mountainboards.

http://www.trampaboards.com/electro-mountainboard-p-12669.html
https://www.scramboards.com/es-scram-board-2wd.html

What I am I missing? (not a rhetorical question!)
```

---
## \#19 Posted by: psychotiller Posted at: 2016-06-01T16:15:24.804Z Reads: 174

```
A single, squishy 9" pneumatic driven wheel is going to be super inefficient. It's going to constantly be pushing the vesc past its comfort zone even at 10s. I think it would be a different story with a dual set up. @treenutter is right about scram, but I'm not sure I've seen anything other than 8" wheels being used.
```

---
## \#20 Posted by: Okami Posted at: 2016-06-01T16:24:12.895Z Reads: 180

```
Yeah, I might switch to 8in later on, as it seems rim can stay the same, only the tire changes its size. 

[quote="psychotiller, post:17, topic:4106"]
I changed my gearing to 12/60 and it will cruise at 32mph (50kph?)
[/quote]

Hah, that's some killer speed!

I'm no expert, but I also think that with 2 motors also the ESC's should divide their load.. but who knows, would need to compare the power ratings for both setups to check that out..
```

---
## \#21 Posted by: DilatedPupils Posted at: 2016-06-01T16:24:26.986Z Reads: 173

```
I used fvt 6s with 6374 149kv on my Trampa, I'm 170lbs and it topped at 13mph. 
Then switched to 12s vesc with the same motor,  And I love it. 
Gearing is 10:60 . 
6374 192kv should be better. Dual drive is a definite must for off roading though.
```

---
## \#22 Posted by: Okami Posted at: 2016-06-01T16:29:15.373Z Reads: 169

```
Yeah, that's the reason why I am bit afraid of the 192kv motor..

<img src="/uploads/db1493/original/2X/8/893f7062c47d298ed454775d2adc4773a3eb19da.png" width="335" height="123">

That's an estimate for your setup (the mentioned FVT 120 and 1:6 ratio)
```

---
## \#23 Posted by: DilatedPupils Posted at: 2016-06-01T16:30:52.308Z Reads: 162

```
That was my speed with 149kv with 6sfvt
```

---
## \#24 Posted by: Okami Posted at: 2016-06-01T16:33:10.134Z Reads: 163

```
Ok, did you had different gearing back then? Because If I dont push myself to get better controller, I might also give a try to FVT 120.. So yeah, I just entered your setup to check how reliable the calculations are..
```

---
## \#25 Posted by: DilatedPupils Posted at: 2016-06-01T16:43:16.761Z Reads: 162

```
Same gearing. But it could also be the app I used to get my speed. If you do get the fvt, don't forget to Get a programming card.
If I had to do it again,  I would use ezrun esc like @chaka said, and go 8s with 6374 192kv.
```

---
## \#26 Posted by: chaka Posted at: 2016-06-01T16:45:13.937Z Reads: 157

```
Remember 8s on an ezrun only works with lifepo cells and you have to be sure you don't charge it higher than 28v.
```

---
## \#27 Posted by: DilatedPupils Posted at: 2016-06-01T16:46:20.429Z Reads: 155

```
What do you mean? You can't run 8s lipo on ezruns?
```

---
## \#28 Posted by: chaka Posted at: 2016-06-01T17:02:56.915Z Reads: 153

```
I was using the ezrun 150pro, I forgot they have an 8s version now.
```

---
## \#29 Posted by: Okami Posted at: 2016-06-01T19:39:19.568Z Reads: 147

```
Did you try to program FVT 120 using computer?  I think I saw somewhere that you can program it using computer.. only though, you probably seem some sort of programmer for that.. dunno where to get that.
```

---
## \#30 Posted by: Okami Posted at: 2016-06-01T19:41:44.655Z Reads: 150

```
Ok, then I suppose it is been decided, that I should go for the 6374 192 kv or go for the alien power systems 220kv 5065 one:

http://alienpowersystem.com/shop/brushless-motors/alien-5065-sensored-outrunner-brushless-motor-220kv-2200w/

It is just between 192kv and 245kv, has 8mm shaft + it is **sensored**! So yea, if the smaller size and smaller amp ratings is not an obstacle, this one seems as a good alternative to sk3 6374. What do you think?


----------
[quote="DilatedPupils, post:25, topic:4106"]
If you do get the fvt, don't forget to Get a programming card.
[/quote]

Did you try to program FVT 120 using computer? I saw somewhere a manual but Im not sure how easy it is to get the right software to program it and does it need a special cable or not..
```

---
## \#32 Posted by: DilatedPupils Posted at: 2016-06-01T20:10:20.392Z Reads: 141

```
You can program it with just the card or with a computer. They should have the programming card available where you purchase your esc.

http://www.rcjuice.com/lcd-program-card-for-fvt-car-esc-s.html

An eskate firmware is also available for a more smooth acceleration which works really good for eskate, but not so much for emtb, imo.
```

---
## \#33 Posted by: paragon Posted at: 2016-06-01T20:13:46.367Z Reads: 139

```
Try @torqueboards 63mm sensored motor; it looks promising.
 product-category/electric-skateboard-parts/electric-skateboard-motors/
```

---
## \#34 Posted by: Okami Posted at: 2016-06-01T20:49:28.475Z Reads: 139

```
These seem to be perfect.. with being sensored, 80a, 8mm shaft, + all the durability they claim

too bad, shipping to EU costs 40 bucks.. That makes it a bit disappointing.
```

---
## \#35 Posted by: torqueboards Posted at: 2016-06-02T01:53:18.428Z Reads: 139

```
@Okami - I'll try and look for cheaper options. I prefer everyone international get their shipments sooner w/ tracking.
```

---
## \#36 Posted by: psychotiller Posted at: 2016-06-02T02:05:07.106Z Reads: 144

```
You can run 8s lipo on the new ezrun max 6 or max 5
```

---
## \#37 Posted by: Okami Posted at: 2016-06-02T07:13:47.919Z Reads: 140

```
Ok, so I found some other posts which answer some of the important e-mtb questions. I hope nobody is going to be mad for putting that info on this thread.


----------


**63mm vs 50mm**, depending on riding conditions

[quote="torqueboards, post:2, topic:95"]
A 63mm for a single should always be slightly better. The main reason because of the bigger motor it can handle and disperse heat better. A 50mm will be more lightweight and as a single is more ideal for flat ground. A 63mm single for uphill would be recommending. I would recommend more along the lines of a 6374 versus a 6354 but both are still better because of the amount of heat it can disperse faster.

Of course, low KV and higher gearing for more torque is ideal if you are climbing hills on a single motor.

For complete flat ground, any of the motors should work with decent gearing and no hot motors.

If the motors are hot, just up the gearing ratio to accommodate more torque and the motors won't be as hot.
[/quote]
```

---
## \#38 Posted by: Michaelinvegas Posted at: 2016-06-02T09:07:07.566Z Reads: 137

```
Posting your own research to share is a good thing...even if it's a different thread...most people don't dig deep enough...
```

---
## \#39 Posted by: Jpadillaff Posted at: 2017-09-18T17:56:04.803Z Reads: 62

```
I am running a single setup with a vesc and it runs perfect. I have not had one problem and it runs very efficiently. I weigh 230 it pulls hills super easy. I have 6374-240kv motor with 11/62 tooth sprocket setup 10s battery and 8in pneumatic tires.
```

---
## \#40 Posted by: psychotiller Posted at: 2017-09-18T18:21:32.193Z Reads: 64

```
10s? 240kv? Talk to me in a month or 2.
```

---
## \#41 Posted by: Jpadillaff Posted at: 2017-09-30T23:30:35.389Z Reads: 54

```
Lol its been longer than 2 months what was supposed to happen at 2 months?
```

---
