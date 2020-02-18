# Why are sensored setups ignored?

### Replies: 123 Views: 16537

## \#1 Posted by: Nasty Posted at: 2016-02-22T05:01:57.010Z Reads: 935

```
The ability to have the FULL control over a brushless motor doesn't seem to catch anyone's interest. I wonder why that is. Its the main reason why the boosted board feels so smooth taking off...help me out guys
```

---
## \#2 Posted by: cmatson Posted at: 2016-02-22T05:11:58.957Z Reads: 920

```
@torqueboards has a sensored esc and motor that I'm using on my next build.

I don't think it's that that are ignored, I think it's that most people are content with the exceptional sensoreless VESC performance. 

Also, most hobby motors (like the turnigy sk3 series) aren't sensored, so you have to search a little harder to find some that are.
```

---
## \#3 Posted by: lowGuido Posted at: 2016-02-22T05:16:59.865Z Reads: 913

```
VESC is also sensor capable.

I just feel that sensors add one more complication that's unnecessary
```

---
## \#4 Posted by: torqueboards Posted at: 2016-02-22T05:27:23.782Z Reads: 904

```
Sensored 100% isn't that great. It's mainly beneficial on start-up. Unsensored on VESC is pretty good.

I made a modification to the VESC PCB to use a standard RC sensor port.

I'm hoping to do more testing with VESC's sensored setup which is actually a sensored/sensorless hybrid since supposedly sensorless is better at higher speeds.
```

---
## \#5 Posted by: Nasty Posted at: 2016-02-22T05:33:22.365Z Reads: 874

```
[quote="cmatson, post:2, topic:1497"]
Also, most hobby motors (like the turnigy sk3 series) aren't sensored, so you have to search a little harder to find some that are.
[/quote]

Totally agree. Its been really hard to find low KV motors that are sensored. But if worst comes to worst,  i found that i am able to attach a hall sensor to most sensorless motors (check this out: http://e0designs.com/products/hall-effect-sensor-board/ ). For a second there, i was starting to think that people have tried, but failed.
```

---
## \#6 Posted by: Nasty Posted at: 2016-02-22T05:36:42.985Z Reads: 845

```
[quote="torqueboards, post:4, topic:1497"]
Sensored 100% isn't that great.
[/quote]

how so? what was your experience?
```

---
## \#7 Posted by: torqueboards Posted at: 2016-02-22T05:41:36.925Z Reads: 810

```
From what I've heard. It's mainly just smoother start-up. It's not as efficient at higher speeds on sensored. There's also a lot more to go wrong. What are you expecting from a sensored motor setup?
```

---
## \#8 Posted by: Nasty Posted at: 2016-02-22T06:04:02.626Z Reads: 797

```
Just that, smoother startup. It just looks more professional. All that twitching looks like shit. One product looks like it was made by a student with his/her associates degree(twitching like its on crack), when the other was made by a masters graduate(smooth operator). I wouldn't normally go the extra mile for a sensored set up, but when its something this obvious, its mandatory in my book. Plus, all of the BIG players in the Eboard game use sensors...
```

---
## \#9 Posted by: trbt555 Posted at: 2016-02-22T06:07:24.548Z Reads: 769

```
IMO its still a skateboard. Push only once and you don't need to worry about twitching.
```

---
## \#10 Posted by: torqueboards Posted at: 2016-02-22T06:17:32.895Z Reads: 760

```
Yeah, you can most definitely run it in sensored mode. Just most people don't mind perhaps.
```

---
## \#11 Posted by: Howser Posted at: 2016-02-22T09:57:59.065Z Reads: 754

```
i would really prefer a sensored setup for the raptor because of the sound difference.
frankly it's a bit embarrassed driving in the city with these screeching motors (especially when braking)..
i'm used to a much more quiet setups so i hope this becomes an option eventually
```

---
## \#12 Posted by: barajabali Posted at: 2016-02-22T13:48:25.025Z Reads: 733

```
I use dual 230kv sensored and I love it. Smooth on any incline. I bet it could pull me up a wall of it had traction lol without twichting
```

---
## \#13 Posted by: barajabali Posted at: 2016-02-22T13:52:22.630Z Reads: 720

```
I agree, on campus I hated when my motors would twitch or when someone would try to use my board and it had a bit of a learning curve because the motors would go crazy under load unless you accelerated slowly. Embarrassing. sensors make it more professional
```

---
## \#14 Posted by: trbt555 Posted at: 2016-02-22T15:16:11.439Z Reads: 702

```
You might want to tweak your settings. I don't own a Raptor but I'm running a single R-spec motor with a VESC and I can get going without twitching from practically standstil. And I weigh 95kg.
```

---
## \#15 Posted by: barajabali Posted at: 2016-02-22T15:30:34.995Z Reads: 679

```
Oh no it's not a raptor just an old board I have
```

---
## \#16 Posted by: trbt555 Posted at: 2016-02-22T15:39:28.373Z Reads: 683

```
Oops, misunderstood.
```

---
## \#17 Posted by: Nasty Posted at: 2016-02-22T15:46:07.438Z Reads: 683

```
That is awesome. What speed controller are you using for the sensored setup? Also, are you running 6s, 8s, 10s?
```

---
## \#18 Posted by: barajabali Posted at: 2016-02-22T15:50:24.362Z Reads: 679

```
Thanks!
Well I'm not a speed demon I like range much more so I only run 6s. I'm also a sucker for a good deal so I run the fvt 120amp esc's. Yes they are sensor capable but no one seems to use them.  They cheap and get the job done pretty well. My max speed is around 25 ish which is plenty fast for me lol
```

---
## \#19 Posted by: barajabali Posted at: 2016-02-22T15:53:32.788Z Reads: 683

```
<img src="/uploads/db1493/original/2X/5/5c42cb29cf5ed3e63814da415140d6a0fec81e65.jpeg" width="375" height="500">

Only problem is the wires that come with the motor, sensor wires, are made of some work hardening plastic and break off really easy. This is how they used to look. So I went and bought silicon wire ones and they work a lot better.
```

---
## \#20 Posted by: Nasty Posted at: 2016-02-22T15:59:11.347Z Reads: 658

```
lol your my hero. Much respect.
```

---
## \#21 Posted by: barajabali Posted at: 2016-02-22T16:04:04.607Z Reads: 647

```
Thank you sir! if you have any questions pm me!
```

---
## \#22 Posted by: treenutter Posted at: 2016-02-22T17:55:38.588Z Reads: 645

```
@Nasty I would use a sensored motor with VESC if there was a single-motor option that had the right specs and price point. 

However, I've found that VESC is pretty smooth from a standstill when uncensored, so I haven't put more thought into it. I agree w @lowGuido that it seems like more complication that wouldn't add too much to performance. As VESC's FOC mode improves, sensored seems to make even less sense.

An $85 63mm 245Kv sensored motor would entice me to try it!
```

---
## \#23 Posted by: EnertionSupport Posted at: 2016-02-22T18:11:48.327Z Reads: 635

```
By giving the motor a little more gas, you can eliminate the jittering on startup. 

A push off is 10x better though, and also helps to keep your balance.
```

---
## \#24 Posted by: torqueboards Posted at: 2016-02-22T18:31:02.619Z Reads: 617

```
@treenutter - I'll have 63mm 230KV which will plug directly into VESC with a modified RC port - for the hall sensor port. Motors are $90 sensored.
```

---
## \#25 Posted by: barajabali Posted at: 2016-02-22T18:42:26.299Z Reads: 609

```
@Nasty These are the motors I use! :grinning:
```

---
## \#26 Posted by: treenutter Posted at: 2016-02-22T18:56:00.373Z Reads: 591

```
Sounds good @torqueboards! I can't wait to see them!
```

---
## \#27 Posted by: treenutter Posted at: 2016-02-22T19:14:30.356Z Reads: 591

```
@Nasty @onloop is right; at first I was a little hesitant to throttle up enough to avoid the jaggies. Once I figured out the throttle curve of my controller, I figured out how to start very smoothly with just a little technique.
```

---
## \#28 Posted by: Nasty Posted at: 2016-02-22T19:51:11.354Z Reads: 577

```
 I do understand how great the VESC performs with sensorless. But in this case I have an option. I think we can all agree on what the better option is. I really think sensors will be a standard in the future.
```

---
## \#29 Posted by: onloop Posted at: 2016-02-23T02:01:35.039Z Reads: 566

```
It is possible to make the R-SPEC with sensors, But I chose not to do it. 

Firstly it increases the retail price of each motor by around $20. 

Secondly, it only does one thing, that is improving start on inclines. It does nothing else positive.

Finally, it reduces high-speed performance so it needs to get disabled at higher RPM if you want the best performance & efficiency

It also adds another layer of complexity that could cause problems. Wires & Connectors & Software.

**To summarise; More expensive, More complex, Giving very-minor advantage - that is made redundant by using your foot to get a small amount of momentum which also aids in balance.**

A good comparison is a manual transmission gearbox vs automatic gearbox in a car.
Trying to hill-start a car with manual gearbox requires some learned skill. Some timing with your feet to apply just enough gas whilst releasing the clutch... otherwise a jerking vibration & stalling of engine will occur.

Automatic gearbox just starts. no skill required.

So which one is better? & why do they still make both options?
```

---
## \#30 Posted by: mccloed Posted at: 2016-02-23T17:59:04.848Z Reads: 537

```
For one, manual transmissions are more fun. :grin: Personally, my favorite board I ride has a sensored SK3 190kv on 6s with an FVT 120a. This board will do 23mph with 20t on the motor and 35t on the 90mm wheels. I weigh about 165lbs and this gets me up some decent hills. I actually got kicked off a board with an unsensored HK 150a esc when I gave it too much throttle. This was not on start up, but accelerating from about 8mph. I sensored that same set up and no more throttle issues. So, sensored definitely has it's advantages. I've kinda become "sensor happy" lately.
```

---
## \#31 Posted by: Hummie Posted at: 2016-02-23T22:27:25.389Z Reads: 524

```
Why don't u put liquid eclectic tape or something on that bare stuff?  If that were me, running at 50 volts especially, I'd be scared to touch my board. 
Nice double plug idea.  

It's quiet without sensors using vesc on foc.  Very quiet.
```

---
## \#32 Posted by: onloop Posted at: 2016-02-23T22:52:07.589Z Reads: 520

```
Your experience is not directly related to the sensors alone, it was because the ESC you have relies on sensors to track the motor position. So that ESC needs Sensors to work well. Just like all other hobby grade ESC.

The VESC however, is different, it doesn't actually need sensors to keep track of the motor speed.

When the motor is rotating while the controller is off, the computations and the direction are tracked. The duty-cycle to get the same speed is also calculated. This is to get a smooth start when the motor is already spinning.

When using the VESC, the only thing the sensors are used for is starting, then they get switch off because it is inefficient.
```

---
## \#33 Posted by: mccloed Posted at: 2016-02-23T22:56:25.689Z Reads: 507

```
I have a board with a VESC. It starts ok, but the sensored board starts even more smooth. I still have yet to try the VESC sensored. That's my next plan.

[quote="onloop, post:32, topic:1497"]
When using the VESC, the only thing the sensors are used for is starting, then they get switch off because it is inefficient.
[/quote]
Correct. In Hybrid mode.
```

---
## \#34 Posted by: RogerD Posted at: 2016-02-23T22:57:02.322Z Reads: 490

```
Running sensorless on normal ESCs runs the risk of motor stalls (when you get "kicked off") - this happens usually when you give too much throttle and the ESC thinks the motor is going much faster than it is (it has to guess) because you've not accelerated fast enough (due to weight, physics etc) - The ESC loses sync with the motor and gets the timing badly wrong.

It is frightening and can be very dangerous at speed. I'm always cautious at top speed just in case it happens. Sensored eliminates this risk.

The VESC seems to handle this fine in sensorless mode but after testing a VESC for a friend, I'm holding off until 

a) it can easily be configured without a laptop (i.e. Bluetooth Android app) as you really do need to be able to program it out on the road.
b) becomes less fragile. Even a firmware misload (wrong version) kills it dead.

I'm running a good old EZRun 150Amp (is the FVT 120 basicallly a knock off?). It runs fine and pulls like a train. It will "almost" pull away from a standstill though I'm used to kick starting now. It's also seemingly bomb proof.

However, the VESC has on particular advantage over car escs - the acceleration is smooth. I can accidentally throw myself of teh back of my board if I carelessly flick the throttle :-)  - the VESC builds up more gradually.
```

---
## \#35 Posted by: mccloed Posted at: 2016-02-23T23:05:41.144Z Reads: 455

```
The FVT 120a is not affiliated with the EZRun.(as far as I know) This is apparent when you hear the screeching brakes of the EZRun and not the FVT. That is the only reason why I preferred it to the EZRun. I think the EZRun is a more reliable ESC, but does not come with the sensored option. And, like I said, I've gone sensor crazy. Sensor every motor!
The VESC's start up is lack luster. If I could figure out how to get it to accelerate like the car ESC's that would be awesome.
```

---
## \#36 Posted by: onloop Posted at: 2016-02-23T23:11:36.890Z Reads: 462

```
[quote="mccloed, post:35, topic:1497"]
The VESC's start up is lack luster.
[/quote]

the VESC has startup boost control, you can dial in exactly how much you need based on your circumstances. You should try it.
```

---
## \#37 Posted by: barajabali Posted at: 2016-02-23T23:12:35.619Z Reads: 454

```
Haha yea I really should cover that up no lie... Thanks!
```

---
## \#38 Posted by: mccloed Posted at: 2016-02-23T23:26:14.270Z Reads: 461

```
I meant acceleration is lack luster. I have startup boost set to 0.1. I read some where that you shouldn't go any higher than that. I should also mention this is a single hub motor.
```

---
## \#39 Posted by: onloop Posted at: 2016-02-23T23:29:00.807Z Reads: 459

```
So its not the VESC, its your drive train.

What Hub motor do you have?
```

---
## \#40 Posted by: mccloed Posted at: 2016-02-23T23:48:36.774Z Reads: 454

```
I have also had the VESC on a geared set up. Same results. I would say it's not the drive train. It's probably the settings. I've gotten it to where I'm satisfied but not ecstatic. This is why I default to the 6s car ESC, but I would like to have an 8s sensored set-up. This is as close as I can get.
```

---
## \#41 Posted by: onloop Posted at: 2016-02-23T23:50:53.264Z Reads: 445

```
You obviously didn't read the raptor thread, most people were complaining the acceleration was too strong.

what voltage?
wheel size?
pulley teeth (m&w)?
Motor KV?
```

---
## \#42 Posted by: mccloed Posted at: 2016-02-23T23:56:59.887Z Reads: 433

```
I did read the raptor thread. Tried those settings to no avail. Maybe i'll take another look...

what voltage? 33.6 - 8s
wheel size? 90mm
pulley teeth (m&w)? none, Hub Motor
Motor KV? 149kv
```

---
## \#43 Posted by: Nasty Posted at: 2016-02-24T00:35:31.754Z Reads: 430

```
[quote="mccloed, post:40, topic:1497"]
This is why I default to the 6s car ESC, but I would like to have an 8s sensored set-up.
[/quote]
 
I just ordered 2 150a sensored ESC's capable of 2-12s, thanks to "Flier electronics". Really hard to find.
```

---
## \#44 Posted by: Nasty Posted at: 2016-02-24T00:36:48.777Z Reads: 412

```
[quote="mccloed, post:38, topic:1497"]
I should also mention this is a single hub motor.
[/quote]

what hub motor are you using?
```

---
## \#45 Posted by: psychotiller Posted at: 2016-02-24T01:07:22.466Z Reads: 403

```
I think it's more a problem of you know what hobby wing and castle was capable of @6s and 8s Matt. Everyone else went to the Vesc from alien, hk, flier, and fvt. And those pretty much suck in comparison
```

---
## \#46 Posted by: mccloed Posted at: 2016-02-24T01:51:57.020Z Reads: 398

```
Carvon single. 

I hate to say it, but, good luck with the Flier ESC's. I've had several of those die for no reason.
```

---
## \#47 Posted by: onloop Posted at: 2016-02-24T02:06:30.081Z Reads: 393

```
You said you had a geared setup. That's what I was referring to.
```

---
## \#48 Posted by: mccloed Posted at: 2016-02-24T05:16:41.045Z Reads: 394

```
No more geared VESC set-up. It was a 295kv 6s, 20t motor, 36t on 83mm wheels.
```

---
## \#49 Posted by: onloop Posted at: 2016-02-24T07:53:56.723Z Reads: 396

```
in your geared system your reduction is very minimal, your KV is high, so this system would not be great for low-speed torque. it may explain the sluggish start.

also the 149kv hubs are similar, not so great for low-speed torque.
```

---
## \#50 Posted by: Nasty Posted at: 2016-02-24T14:17:06.162Z Reads: 386

```
Well that sucks lol, I'm crossing my fingers..
```

---
## \#51 Posted by: mccloed Posted at: 2016-02-24T17:51:52.549Z Reads: 394

```
True, but in both these set-ups the car ESC has done exactly what I wanted/expected. Especially when sensored, and at only 6s. I'm still going to invest time in the VESC, but I will always have my back up ESC's. I'm really anxious to see how the VESC acts when sensored. :smile_cat:
```

---
## \#52 Posted by: torqueboards Posted at: 2016-02-24T19:32:25.569Z Reads: 388

```
Me too.. Sensored VESC should be best of both worlds.
```

---
## \#53 Posted by: lowGuido Posted at: 2016-02-24T21:57:32.954Z Reads: 383

```
All this talk about start up torque.  Why can't people kick?
```

---
## \#54 Posted by: barajabali Posted at: 2016-02-24T22:10:15.962Z Reads: 378

```
Same reason we use eboards in the first place! We don't kick while we ride and now we don't have to when we start up. It's my preference to have good torque always
```

---
## \#55 Posted by: lowGuido Posted at: 2016-02-24T22:33:59.793Z Reads: 375

```
Yeah i get it. But like its my instinctive reaction to just give it that one push as i get on the board anyway. Its super awkward to just stand on the board and not kick.
```

---
## \#56 Posted by: onloop Posted at: 2016-02-24T22:48:15.505Z Reads: 393

```
I know right? next people will want eboards that can move around robotically without them standing on it at all..... *go get me a coffee eboard!*

for me this entire scene is about **enhancing traditional skateboards** so that you can ride up hills and cover vast distances in rapid time with little effort on a super efficient lightweight mode of transport.


ALL THESE FANCY THINGS LIKE
- starting from stationary position on incline without lifting a finger (or foot)
- riding at incredibly slow speeds so you can look *cool* cruising at the beach. (use a normal skateboard)
- brakes that somehow know not to launch you from the deck when you squeeze too hard. (don't ride so fast, or learn how to use the brakes properly)
- Advanced systems that somehow know to correct all your mistakes and prevent you from wiping yourself out. (use your car)


I think people need to stop & consider that the modern eboard is literally 3 years old.... It's a fucking baby in terms of its development...

all this fancy shit only exists because boosted boards raised a massive amount of money and paid engineers & spent 12 months to make it all specifically for their product. 

Lets all just be happy we now have some half decent parts that we can make eboards with... when I started building eboards in my garage 3 years ago everything came from the hobby shop, or cost triple the price it currently does.

so lets just enjoy what we have...
```

---
## \#57 Posted by: barajabali Posted at: 2016-02-24T23:25:59.007Z Reads: 378

```
Well youre thinking about when you first start up and hop on your board, yea i agree it is awkward to just stand on a hover away.  But what about when youre stuck behind a group of slow walking people or you need to come to a almost complete stop but not totally? no reason to kick with extra start up torque.  You can just accelerate at whatever speed you need. 

My mentality is not to impress you guys at all. I am here to get inspired and build my personal board to the best of my ability and use all the resources I can afford and understand how to implement.  That being said, if adding sensors to a board is 'fancy' (its only a 1 plug)  then the vesc is 'fancy' too.  I still use old shitty fvt esc's because its what i can afford and what im comfortable using. 

Im enjoying what i have with what i can do. @onloop
```

---
## \#58 Posted by: onloop Posted at: 2016-02-24T23:47:39.373Z Reads: 386

```
I just don't think sensors are required.

have a look at some of my videos:

In this video, at 2m 7s, I start from stationary up a hill, **no sensors**.
https://youtu.be/hEWHhwSDkug?t=2m7s

in this video, I lift my foot onto the board and accelerate at full speed, **no sensors**.
https://youtu.be/JgKPCrG5Nyc?t=4m27s

this video, come to near stop & start again flawlessly, **no sensors**.
https://youtu.be/o_5Bh4zceGQ?t=36s
```

---
## \#59 Posted by: barajabali Posted at: 2016-02-24T23:59:50.770Z Reads: 374

```
Ive rode for a year without sensors, I completely agree they are not required whatsoever. BUT the fact is that many of the improvements our community makes to our boards are not required. The beauty of this hobby (as any DIY) is that it leaves many topics for customization.  No one is riding my board but me, and if i purchased motors that have sensors built in, and my ESC happens to have a sensor port i'm not leaving the wire dangling, I'm going to use the sensors. 

Maybe demand will change in the future once people try to use sensors on their boards.  Sure maybe its a 'luxury' but an ELECTRIC skateboard is already a luxury. 

all in all, who gives a fuck. lol
```

---
## \#60 Posted by: onloop Posted at: 2016-02-25T00:13:40.939Z Reads: 394

```
[quote="barajabali, post:59, topic:1497"]
all in all, who gives a fuck. lol
[/quote]

the OP does, he wanted to know why they get "ignored"

the simple answer is because they don't do enough to make them worthwhile. People are always crying that things are too expensive... i can make R-SPEC motors with sensors now, but will anyone pay an extra $20? I'm not sure they will.

in the future this might change.
```

---
## \#61 Posted by: barajabali Posted at: 2016-02-25T00:26:22.176Z Reads: 388

```
And I think they are worthwhile. Opinions are an amazing thing.
```

---
## \#62 Posted by: mccloed Posted at: 2016-02-25T00:28:05.763Z Reads: 389

```
I still kick even with sensors. I can sensor a motor for about $5. I've gotten pretty good at it. It's pretty labor intensive and requires a lot of cussing.
```

---
## \#63 Posted by: ambrojohn Posted at: 2016-03-20T18:55:06.434Z Reads: 384

```
From Alien Power System, $80 (£55):
http://alienpowersystem.com/shop/brushless-motors/alien-5065-sensored-outrunner-brushless-motor-220kv-2200w/
```

---
## \#64 Posted by: torqueboards Posted at: 2016-03-20T21:44:27.946Z Reads: 374

```
@ambrojohn - Why when you can get a 6355 230KV for $90 :) product/electric-skateboard-motor-6355-230kv-2650w/
```

---
## \#65 Posted by: mcoyle Posted at: 2016-03-21T23:05:36.312Z Reads: 363

```
Are you using the 230KV from diyelectricskateboard? I have a dual setup with those two as well and my dual VESC just arrived, but the sensored wires won't plug into anywhere on the VESC. are you using a different speed controller?
```

---
## \#66 Posted by: barajabali Posted at: 2016-03-21T23:14:19.799Z Reads: 358

```
I choose not to use the vesc. I'm basic with the fvt esc
```

---
## \#67 Posted by: torqueboards Posted at: 2016-03-22T00:21:42.502Z Reads: 367

```
@mcoyle - The last batch of our motors were with the standard RC port. Latest batch is actually with the JST-PH 2.0mm 6pin port the same on the VESC.

You would have to make an adapter if you got our old batch. If you having a pending order.. which I think you do.. You'll be able to plug in directly.

You can wire it in but you'll need to adjust the settings. I'll try to release more videos in the near future. Otherwise, you'll have to do some digging and testing.
```

---
## \#68 Posted by: mcoyle Posted at: 2016-03-22T03:52:18.349Z Reads: 357

```
The order was placed January 25th and the connector from the motors is too small for the VESC so I'm guessing I'll need to get a converter? Can you redirect me to a converter of this sort?
```

---
## \#69 Posted by: torqueboards Posted at: 2016-03-22T06:45:38.854Z Reads: 364

```
Yeah, you'll need an adapter for the Standard RC Sensor Port to the VESC. You'll also need to match the pin-out.

You would need an adapter with the following:
(Standard RC Sensor Wire) 6pin JST-ZH 1.5mm pitch FEMALE to 6pin JST-PH 2.0mm pitch MALE. (VESC)

Pin-out should also match.
```

---
## \#70 Posted by: Tijmen Posted at: 2016-08-13T16:30:51.425Z Reads: 310

```
Sorry if this has already been answered in this topic, but, the sensored motor I ordered didn't come with ABC markings. How do I know how to connect it correctly to my ESC?
```

---
## \#71 Posted by: mccloed Posted at: 2016-08-13T16:59:10.540Z Reads: 307

```
This is the way I do it. I plug the phase wires and sensor lead in then hit the throttle quickly. If it makes a weird noise or hesitates I switch the phase wires around. Just don't hit throttle too long or you'll fry something. It should end up sounding normal, if they are plugged in correctly.
```

---
## \#72 Posted by: MattCarl Posted at: 2016-08-29T20:38:01.698Z Reads: 297

```
Hey man, I'm using the same motor and ESC as you but as a single drive. I'm curious because I've been nervous to run it sensored (I've been running sensorless) because the diyelectricskateboards website doesn't tell you what the blue black and yellow phase wires correspond to A B C on the ESC. can you simply plug in the sensored cable into the ESC and have it be good to go? Right now I have the phase wires hooked up blue to blue, yellow to yellow, and orange to black? Any insight would be greatly appreciated!
```

---
## \#73 Posted by: Cptanpanic Posted at: 2016-08-30T00:40:43.347Z Reads: 295

```
Here is what @torqueboards gave me

Blue = A
Black = B
Yellow = C
```

---
## \#74 Posted by: popopopop Posted at: 2016-08-30T00:55:55.206Z Reads: 292

```
I have TB's 6355 motor on a TB 6s esc. I blew up the ESC a few weeks ago being stupid. I had the symptom mccloed said above and I guess over did it. The motor cog and I saw faint smoke. I connected it like you did on a second ESC, but it wasn't right. Switch two of your wires now, turn on your esc+ transmitter, then hit the throttle for a second. If it's super smooth, you're good to go. If it cogs up, shut it down and switch wires again. It worked for me, just as mccloed did it.
```

---
## \#75 Posted by: MattCarl Posted at: 2016-08-30T01:14:17.466Z Reads: 285

```
Thank you guys, I'll give it a shot!
```

---
## \#76 Posted by: NNGG Posted at: 2016-08-30T05:57:38.941Z Reads: 281

```
How did you motor handle inclines and torque?
```

---
## \#77 Posted by: popopopop Posted at: 2016-08-30T10:57:31.573Z Reads: 276

```
I don't have a reference to any other eboards, but I'm 190 lbs and it's holding up fine. I use it mainly on flatgrounds around school and bike trails. It's not a commuter board for me, just something I mess around with for fun. I haven't noticed my motor even getting warm yet.
```

---
## \#78 Posted by: longhairedboy Posted at: 2016-08-30T13:50:54.843Z Reads: 277

```
Are we taling about non-VESC setups? I run uncensored R-SPECs with VESCs on all my builds and occasionally an SK3 or two will get in the mix. Just jam the throttle till you start moving and then back off a little once it starts moving. It might stutter for half a second but who cares. 

@onloop life is way to short for that one tiny push for some people i guess lol
```

---
## \#79 Posted by: Jinra Posted at: 2016-08-30T15:49:31.402Z Reads: 263

```
[quote="longhairedboy, post:78, topic:1497"]
I run uncensored R-SPECs
[/quote]

That's lewd
```

---
## \#80 Posted by: treenutter Posted at: 2016-08-30T16:44:23.826Z Reads: 268

```
[quote="onloop, post:32, topic:1497"]
When using the VESC, the only thing the sensors are used for is starting, then they get switch off because it is inefficient.
[/quote]

@onloop @mccloed is this feature is already a part of VESC's firmware? If so that's awesome! 

While personally I don't feel like I need a sensored motor experience, I have a lot of people asking me to try by build. Having to explain to them the startup process, and hope they execute it correctly, is a problem. For DIY'ers VESC startup is good enough, but for a total novice the stutter on startup makes the build feel cheap and dangerous. This is why I'm aiming to use sensored motors in the future. It's not for me, it's so that the ride experience is better for new riders.
```

---
## \#81 Posted by: Jinra Posted at: 2016-08-30T16:47:23.298Z Reads: 262

```
It is! It's the "hybrid" option you see as opposed to "sensored" and "sensorless". I currently run this mode and I love it. I know most the veterans here run sensorless, but I don't get why you wouldn't use it if it's there. I kick off the majority of the time, but sensored can really help when you're trying to kick start up a hill, as you can sometimes get to near stand still before actually accelerating.

Most times I use the sensors is when I have my feet in a nice and comfortable position and I'm too lazy to kick and readjust :P
```

---
## \#82 Posted by: sl33py Posted at: 2016-08-30T17:30:36.454Z Reads: 257

```
I think it's a great option even if you don't use it.  I know on my production board (marbel) and riding Boosted (friend's Dual+) - sensored is really nice at start and on hills.  I still typically kick a time or two - habit.  But on hills and such it's nice.  

All of my DIY's are un-sensored currently, but i'm going to try it on one of them.  Think the GF will like the smoother start.

When slowing down on a hill - does the sensored setup perform better?  may be missinformation, but i'd heard they had better torque on hills?  Anyone can comment that's tried both sensored and unsensored on the same setup?
```

---
## \#83 Posted by: Jinra Posted at: 2016-08-30T17:33:05.083Z Reads: 256

```
I'm actually running 1 sensored 1 sensorless right now because the sensors on 1 of my motors are borked. It doesn't really help slowing down and feels just the same as sensorless. I wouldn't say startup torque is better, but it helps the motor not 'cog' and get confused on how to start rolling, so it may give the illusion of better torque.
```

---
## \#84 Posted by: sl33py Posted at: 2016-08-30T18:10:46.608Z Reads: 253

```
Cool thanks @Jinra!  I guess the only possible advantage is torque uphill - sensored vs not?  

Anyone able to do comparison like Onloop does w/ timer on a set stretch (and uphill would be great)?
```

---
## \#85 Posted by: Jinra Posted at: 2016-08-30T18:13:56.123Z Reads: 253

```
Sensored isn't good for high speeds due to inefficiency (also gets the motors pretty toasty!), so it's only applicable in hybrid mode until it reaches a couple miles per hour depending on how you set it. I doubt you'll really notice any difference seeing as sensorless can't really go uphill without a kick anyway. My motors switch to sensorless at 3mph.

I wouldn't say uphill is the only advantage of sensors. Like I said, I use it for when I have my feet in too comfy of a position for me to want to kick start, so I can stop from a dead start at a light or stop sign.
```

---
## \#86 Posted by: longhairedboy Posted at: 2016-08-30T18:34:57.193Z Reads: 246

```
i do that all the time with no sensors. I guess it depends on the weight or the rider and a number of other things like if you're stopped on a slope or if the road isn't smooth or the voltage you're running maybe as well.
```

---
## \#87 Posted by: Jinra Posted at: 2016-08-30T18:39:31.858Z Reads: 247

```
It works for me in sensorless most the time as well. Occasionally though, I get a bit of cogging from dead start.
```

---
## \#88 Posted by: treenutter Posted at: 2016-08-30T19:02:17.368Z Reads: 246

```
@Jinra Just looked through BLDC Tool and it seems that "hybrid sensor mode" is only available in BLDC mode :( It's not there for FOC, unless I'l missing something.
```

---
## \#89 Posted by: Jinra Posted at: 2016-08-30T19:08:16.989Z Reads: 252

```
FOC has it too. take a look at the sensorless erpm field in the FOC tab. That's the erpm where it kicks it into sensorless.
```

---
## \#90 Posted by: Lizardking0069 Posted at: 2016-08-30T19:17:54.678Z Reads: 250

```
Hey Dexter, I bought from the previous batch with the wrong plug. Is there a way to get an adapter so I can use the sensors? I really don't want to solder all of those wires.
```

---
## \#91 Posted by: Jinra Posted at: 2016-08-30T19:18:50.998Z Reads: 247

```
Didn't the head I sent you work? You just pop off the jst header and place it on tbs motors
```

---
## \#92 Posted by: Lizardking0069 Posted at: 2016-08-30T19:38:37.462Z Reads: 247

```
The plug you sent does not fit the TB Vesc. I'll pm a photo later, maybe I'm missing something.
```

---
## \#93 Posted by: treenutter Posted at: 2016-08-30T19:50:12.185Z Reads: 252

```
[quote="Jinra, post:89, topic:1497"]
take a look at the sensorless erpm field in the FOC tab
[/quote]


Oh thanks @Jinra ! I thought that was an ERPM setting for top speed in FOC mode! How did you figure that out? Is there a VESC feature listing that I'm not finding? Side note: that value must be set pretty low I imagine, like 200 or so?
```

---
## \#94 Posted by: Jinra Posted at: 2016-08-30T20:15:18.020Z Reads: 250

```
It should. All VESCs use standard parts and it fits pretty well as you saw in my build log. There will be 1 pin which wont work since I gave you a 5 pin header. Just take out the red power wire and plug it directly into the 5v pin on the VESC. Use the the 5pin header for the next 5 pins and make sure they're ordered correctly.

See pic: http://www.electric-skateboard.builders/uploads/db1493/original/2X/6/61f1ed89f798b352ad6f17341c0040527e37c30b.jpg

@treenutter It's a setting just for when to kick in sensorless operation similar to how it's labeled in the BLDC tab. The UI could be a bit more clear on this. Make sure you choose the hall sensor mode as well. I haven't played with FOC myself, but this is my understanding on how it works. Default sensorless eRPM is 2000, but I have mine at 6000. I set mine so it cuts off at about 3mph.
```

---
## \#95 Posted by: Lizardking0069 Posted at: 2016-08-31T12:05:37.873Z Reads: 259

```
Well I Connected the sensors to the Vesc yesterday and they now work. I set it up in hybrid mode, but I'm not sure which is the erpm setting for sensored to sensorless transition. 

Anyway, the board now feels even smoother. While before in sensorless there was a bit of cogging at launch, especially at standstill, now there is virtually zero cogging. To me sensors are a must now and I cannot go back. The smooth throttle response combined with almost no cogging make the board feel like a finished product.

Thanks Jinra!
```

---
## \#96 Posted by: SimosMCmuffin Posted at: 2016-08-31T17:55:36.000Z Reads: 257

```
I don't think most people know that Boosted boards use a sensored setup. Although it's not the traditional 3 hall-sensors mounted inside or outside of the motor can. Rather it's a 8.5-bit magnetic rotary encoder (model number AS5134) manufactured by AMS and it is mounted at the end of the motor axle, which is why the boards have the motor/belt covers (IC is embedded in epoxy).

So, why use a rotary encoder IC, which has to be mounted at the end of the motor axle rather than the standard 120 degree hall sensor mounting on the stator? Resolution/precision. Manufacturer's product demo video for the AS5134 embedded below (pretty cool stuff IMHO).

https://www.youtube.com/watch?v=DUrXY2gAct0

https://endless-sphere.com/forums/viewtopic.php?f=35&t=67586 (boosted board disassembly thread)
http://ams.com/eng/Products/Magnetic-Position-Sensors/Angle-Position-On-Axis/AS5134 (AMS AS5134 product page)

I think the hassle of using a sensored setup is worth it, because I believe it gives a better user experience to the customer as long as it's built properly and with proper failsafes. The normal DIYer probably doesn't want anything more complicated than the VESC in sensorless, because it works well enough.
```

---
## \#97 Posted by: Jinra Posted at: 2016-08-31T17:58:57.858Z Reads: 233

```
Agreed, if there rspec had a sensored motor i would consider those motors. The only 63mm motor on my wish list right now is @torqueboards
```

---
## \#98 Posted by: SimosMCmuffin Posted at: 2016-08-31T18:08:49.292Z Reads: 241

```
Have you looked at AlienPowerSystems? They have a very good offering in the 63 mm dia motor department both with sensors and without, although I can understand them being based in UK and you're in the states that you don't prefer them therefore. I plan on updating my current powertrain to their systems in the next iteration and see how they perform.

I'm trying to start my own esk8 company in Finland. I have spec'd 3 bachelor degree thesis works for my university's final year class for battery BMS, remote controller and smartphone app and I hope I can get a team out of them. I personally handle the motor controller, powertrain and board platform design myself. Not sure if we ever make it to the commercial markets, but I hope we at least make it to the DIY markets.
```

---
## \#99 Posted by: Jinra Posted at: 2016-08-31T18:11:52.385Z Reads: 234

```
I've heard iffy reviews of their motors, but either way I'd rather purchase local as it's much cheaper and faster. Plus DIYelectricskateboard is right next to me. I may participate in @JLabs next 63mm sensored group buy if he sets it up within the next month.
```

---
## \#100 Posted by: SimosMCmuffin Posted at: 2016-08-31T18:18:15.407Z Reads: 253

```
What kind of iffy stuff? A google search with "alien power system motor problem" didn't really produce any significant results except that their ESCs might have problems, but not much on the motor side. I am interested in finding out any bigger scale problems they might have. I also couldn't really find any other supplier's in the euro area except them.
```

---
## \#101 Posted by: Jinra Posted at: 2016-08-31T18:19:30.463Z Reads: 240

```
Can't link you to direct reviews, but they were all on this forum. I know @whitepony had some issues with his Alien Power HEV motor, though I'm not sure what the cause of the issue was.
```

---
## \#102 Posted by: SimosMCmuffin Posted at: 2016-08-31T18:30:38.147Z Reads: 261

```
[quote="whitepony, post:17, topic:7258, full:true"]
I have probably put around 250km into that motor by now - my quick conclusion:

positive:
+ lightest 63mm outrunner available to my knowledge (508gr)
+ comes with silicone wires and 5.5mm gold bullet connectors
+ least resistance of all my motors in idle (= best coasting)
+ most silent motor I got when coasting - this thing is just dead somehow, I only hear the belt
+ most balanced motor I got - absolutely no vibration+ comes with a keyway + key
+ cheapest of my motors
+ mostly closed body
+ runs coolest (but this is most likely due to the full aluminium APS mount)

negative:
- 1 out of 2 had that scratching thing, Ill assume its not intended but the motor still really runs well and well balanced at high rpms so Im still not sure what it is
- in FOC mode: noisiest of my motors at full load mid rpm, but it feels like it has somehow become more silent after 250km (or I got used to it)
- shaft is too short for 15mm pulleys and Im not sure if 10mm is necessary
- only 14AWG wires used

especially for the price, its a very nice motor and Ill probably use no2 for my spud freebord! torque is less than my sk6374, but about the same as the 6355 rspec. near impossible to quantify without acceleration tests!
[/quote]

Seems overall like a good motor and if there are any QA problems with larger batches, I will probably just contact APS directly for reclamation. But at this point when I haven't even had one to fiddle around myself, can't say anything for sure. I'm waiting for them to give me the specs of the integrated hall-sensors before I order the first one.
```

---
## \#103 Posted by: sl33py Posted at: 2016-08-31T18:49:43.475Z Reads: 248

```
i believe you can also look at www.esk8.de?

It's been a while, and i hope Bruno has fixed some of the issues, but i also had a horrible experience with APS.  As a result i avoid as possible.  It's a bummer ADS now sells via APS as i need a wider/more t wheel gear swap...

My experience was specific to the crappy Flier/APS dual ESC.  The long story short(long) it took over a month to fix/refund what was miss-represented as an 8s ESC that could only handle 7s (or a low charge on 8s).  It literally _would not work at full 8s voltage_.  So i was unreasonable and asked for a full refund including shipping and no re-stock fee.  Not something i'd normally do except it simply did not work as advertised.  After repeatedly asking he finally edited the link to say 7s ESC so at least the next guy didn't have the same frustration.  The lack of response and having to follow up multiple times, plus taking over a month (i think it was 5-6 weeks) to refund (already sent back) then partially refunded and had to go around and around again to get full refund including s/h...  painful.
```

---
## \#104 Posted by: SimosMCmuffin Posted at: 2016-08-31T18:59:38.475Z Reads: 244

```
I must point this out now, that I'm only concerned about the motor quality, as I will be designing the board's ESC myself.
[quote="SimosMCmuffin, post:100, topic:1497"]
A google search with "alien power system motor problem" didn't really produce any significant results except that their ESCs might have problems, but not much on the motor side.
[/quote]
You got any experience / thoughts on their motors?
```

---
## \#105 Posted by: sl33py Posted at: 2016-08-31T19:01:56.556Z Reads: 245

```
Understood.  I think this relates to customer service which is why i mentioned it.

It does seem like most have a great experience with their motors.  Good quality.  Not sure of warranty, but he has shown willingness to swap and repair other items under warranty until fixed.  Not all bad and not trying to bash APS.
```

---
## \#106 Posted by: whitepony Posted at: 2016-08-31T19:09:36.926Z Reads: 250

```
[quote="sl33py, post:105, topic:1497"]
I think this relates to customer service which is why i mentioned it.
[/quote]


bruno is a nice guy, but OMG, it takes forever to iron out stuff and half of the time it feels like he is reading only half the words of a mail ... and then the parcel FINALLY arrives and half the parts were wrong again, so it all starts over again. Im still waiting for parts of my spud ... wonder if I can ride it before winter with the way things advance with bruno.

I definitely wouldnt order @ APS anymore, if anyone else had the parts I needed. proper 15mm wheel pulleys for abecs, the motor mount is quite unique and allowed my ronin cast vanguard, the antispark uses an SPST switch, which can be bought very cheap and small.
```

---
## \#107 Posted by: makevoid Posted at: 2016-08-31T20:50:43.229Z Reads: 251

```
I have the esk8.de sensored 6374 and it's very good, it's a bit noisy for me to use with BLDC but with FOC it was really really smooth, used as a single motor with a very high motor max and motor min (85A/-70A) on 6S I had a very good experience with a lot of torque and not much heat. The only downside is the pulley mounting system, they suggest to put only green thread-locker on the motor shaft, you have to be careful of not putting too much of it, I would like a keyway/key system or a pulley that is made of only one piece (the flanges are not very solid) so it can be removed easily with a pulley remover if needed. I will try to use it on my current build (8S 15t/36t 97mm wheels) soon.
```

---
## \#108 Posted by: SimosMCmuffin Posted at: 2016-08-31T21:11:11.177Z Reads: 281

```
After looking at the esk8.de and APS motors. I am 90% sure that they are very likely made in the same chinese factory with the only difference being the logo on the side of the can.

Here's a picture from the esk8.de showing all their different motor sizes:
https://dqzrr9k4bjpzk.cloudfront.net/images/7570530/396841132.jpg
http://www.hellray.de/shop/#!/eSk8-de-Motor-esk8-6374-170kV-3-0KW-mit-Sensoren/p/66640990/category=15255001

Now compare those motors to these three from APS:
http://alienpowersystem.com/shop/brushless-motors/alien-6355-outrunner-brushless-motor-130kv-2400w/
http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-170kv-3200w/
http://alienpowersystem.com/shop/brushless-motors/alien-6355-sensored-outrunner-brushless-motor-130kv-2200w/



Both the bottom and the top of the cans are **identical** between the shops. Motor axles are same dia. Bearings look to be the same.
```

---
## \#109 Posted by: Gizmo Posted at: 2017-11-29T15:51:28.438Z Reads: 169

```
Are there any drawbacks to sensored that would result in damaged vescs or motors?
```

---
## \#110 Posted by: Deckoz Posted at: 2017-11-29T16:19:28.177Z Reads: 178

```
So here's my opinion on sensors

-they are great
-they do nothing for the vast majority of your ride. Anything over 1-2mph and they're no longer needed
-yes they do make a difference
-all my builds have and will always have sensors.

So I love a sensored setup as I can come to a soft stop aka Cali Roll, at a stop sign. With sensors. This is a non issue for the transition of speed to basically stopped and moving again. Smooth as butter. Without sensors, I get some cogging.

 In contrast Currently one of the sensors on my dual vanguard has died. So im running half sensored half sensorless with Canbus. A note about this... 

Running a sensorless motor as the master and the sensored motor as the slave. You will still get some cogging, but its not as bad as completely unsensored.

Running the sensored motor as the master and the non sensor motor as the slave, yeilds almost undetectable cogging only during braking close to full stop. Acceleration and take off performance is similar to that of a full sensored setup. And I'm only talking about canbus. Split ppm has no RPM/current telemetry sharing for the control loop, as ppm is external.
```

---
## \#111 Posted by: deucesdown Posted at: 2017-11-29T20:40:16.346Z Reads: 159

```
[quote="Deckoz, post:110, topic:1497"]
So im running half sensored half sensorless with Canbus
[/quote]

traction control is off, I'm guessing?
```

---
## \#112 Posted by: Deckoz Posted at: 2017-11-29T20:59:02.029Z Reads: 161

```
No traction control on, with all...variations
```

---
## \#113 Posted by: danielz Posted at: 2017-11-29T22:55:36.895Z Reads: 157

```
I wasnt able to pull off from a start on my mountainboard with a single sk3 6374. Once i sensored it i was. Ive since upgraded to dual sensored, id never go back to unsensored.

https://www.instructables.com/id/How-to-Add-External-Hall-Sensors-to-a-Turnigy-SK3-/
```

---
## \#114 Posted by: Hummie Posted at: 2017-11-29T23:04:40.203Z Reads: 158

```
how do they effect efficiency?  ha I'm thinking if I do that first little push from stopped I'm going to be more efficient without them.

how durable are they?  it seems they're always breaking from physical vibrations or heat.
```

---
## \#115 Posted by: Deckoz Posted at: 2017-11-30T00:54:15.021Z Reads: 154

```
Efficiency? They aren't used after a certain mph...so overall efficiency is negligible. 

Breaking? Everyone in our group that has them has been fine. My one broke at the base of one of the wires solder connection, and the sensor is epoxied in and I'd rather not pull it out as I dont want to pull the enamel off the windings to fix it...my dumb ass set the motor on the table and it rolled off and I caught it by the sensor wire...  

Sensors is all about start up feel and low rpm control. If ya don't like em don't use em... But for 8 bucks and a few dabs of epoxy...who really complains about $8 sensors on expensive ass builds...not me.
```

---
## \#116 Posted by: b264 Posted at: 2017-11-30T01:15:55.102Z Reads: 153

```
[quote="torqueboards, post:7, topic:1497"]
What are you expecting from a sensored motor setup?
[/quote]

Quiet operation in FOC mode and butter-smooth startup and applying brakes at high speeds does so VERY gradually at first
```

---
## \#117 Posted by: jmasta Posted at: 2017-11-30T01:20:14.258Z Reads: 157

```
What motors and hall sensors are you using?  Did you add them internally?

I just replaced my sensorless motor with another sensorless one, because an equivalent motor with sensors was almost double the price.  I always kick my board out in front of me and then jump on while it's moving, so I couldn't justify paying $45-75 extra just for the sensors. But if I could add them for cheap, why not?
```

---
## \#118 Posted by: Deckoz Posted at: 2017-11-30T01:35:15.806Z Reads: 148

```
Torque boards 6355. I have a replacement sensor sitting here, the original is internal, relatively easy to access, is tucked into the top of the stator., but is epoxied in.

 I'm waiting to replace it with the replacement until the other board is done..in case I accidentally rip the enamel off the windings or the stator core when removing the old epoxied one. 

Either way sensors and installing them is cheap
```

---
## \#119 Posted by: Battosaii Posted at: 2017-11-30T01:36:48.309Z Reads: 157

```
Yea I use the Hybrid mode uses sensors in low rpm and not at speed, so basically for a good start up. I generally always start with a kick push but sometimes I come to a stop sign and I don't get off the board so sensors help in that aspect.
```

---
## \#120 Posted by: Deckoz Posted at: 2017-11-30T01:37:32.696Z Reads: 172

```
Sensors won't do anything for you at any sorts of speed... Its all startup and low end rpm so that the controller can synchronize with the motor while back emf is to low to get accurate readings.


[quote="Battosaii, post:119, topic:1497"]
I come to a stop sign and I don't get off the board so sensors help in that aspect.
[/quote]

Exactly. Sometimes you just wanna hit throttle and go
```

---
## \#121 Posted by: cypa9904 Posted at: 2018-04-13T10:25:39.107Z Reads: 147

```
Hi.
Will sb tell me if this may have a smooth start (FOCBOX, FOC mode)?
1:4.55 gearing, 200mm wheels (mountainboard), two 192kV sensorless motors, 10S battery.
```

---
## \#123 Posted by: Linny Posted at: 2018-10-13T03:58:15.525Z Reads: 73

```
Is it safe to run one sensorless and one sensored? My dual drive has a bad hall error detection so i'm currently running both sensorless. Would be great to have it 'half sensored' if there are no risks.
```

---
## \#124 Posted by: Pedrodemio Posted at: 2018-10-13T04:04:36.297Z Reads: 73

```
No problem, just take easy at first to see how it behaves, if you need a lot of torque at startup you may cog since one motor can’t provide as much torque as teo
```

---
