# Leisure Industry Features That We Could Implement

### Replies: 178 Views: 2879

## \#1 Posted by: Jc06505n Posted at: 2018-06-17T18:26:47.723Z Reads: 441

```
Edit: The purpose of this thread has shifted a little. 

It's aim is to **recruit, debate, discuss, and fund the, improvement and implementation of features we would like to see on VESC's and ESK8's as a whole.** In order to pull this off we would need a community consensus of what features are wanted over what. If there's enough demand for it, we could possibly provide community funding for it's creation, whether it be for labor, manufacturing, etc. 

It would be up to the individual to work on prototyping and presenting it to the community in for them to be considered.  

For now I'll start a Poll of the first four mentioned features and then add more on as they are suggested. 

[poll type=multiple min=1 max=4 public=true]
* Endless Ride (I.e Mellow AKA Push Assist)
* Lifetime Oddmeter (whether via Remote or External VESC comparable Hardware)
* Push to Start (i.e Meepo, Wowgo, DIYeboard)
* Power Off Via Remote (B.B. does this via Holding the Button and the Trigger Down)
[/poll]

For now lets talk about , what's needed for these to be implemented? 

To keep future discussions sane: If you don't want it, don't vote for it and don't talk about it. As simple as that. You "not seeing the point of it" or "not liking it" does not contribute towards the discussion or aim of this thread.
```

---
## \#2 Posted by: Lospalaz Posted at: 2018-06-17T20:45:36.388Z Reads: 393

```
We do a group buy to hire a programmer to implement the features... =P
```

---
## \#3 Posted by: Jammeslu Posted at: 2018-06-17T22:15:57.257Z Reads: 378

```
Easy way to have diffrent speedmodes that can be used by standard remotes
```

---
## \#4 Posted by: banjaxxed Posted at: 2018-06-17T22:32:40.699Z Reads: 371

```
Good call @Deodand consider stealing a lead with the Unity
```

---
## \#5 Posted by: mikenyc Posted at: 2018-06-18T00:28:40.530Z Reads: 348

```
google assistant or siri to control the board? :joy:
```

---
## \#6 Posted by: longboardshort Posted at: 2018-06-18T02:14:16.632Z Reads: 330

```
I know everyone’s thinking it - auto pilot / self driving mode like cars are testing right now 🤣
```

---
## \#7 Posted by: rsalmon Posted at: 2018-06-18T03:20:57.459Z Reads: 316

```
I think the odometer is such a nice touch and it would be awesome to have it on our DIY boards.
```

---
## \#8 Posted by: Eboosted Posted at: 2018-06-18T03:59:46.029Z Reads: 310

```
How about we all put down a deposit and pay to the first programmer/hardware developer team to accomplish this?

I'd be down with US$ 20
```

---
## \#9 Posted by: skatardude10 Posted at: 2018-06-18T04:22:42.908Z Reads: 302

```
I'm really only interested in endless ride... I'd be down for $10
```

---
## \#10 Posted by: AreaKruzer Posted at: 2018-06-18T04:25:55.218Z Reads: 299

```
The odometer should not be a difficult to code, I should be able to do it, but I will need to know if the VESC is able to output lifetime ERPM(tachometer).

If not, probably you have to implement a microSD breakout that is attached to an arduino, storing each power on's and off's Tac ABS and then doing a calculation like
(Tac ABS / motor pole pairs) / (Wheel pulley teeth/ spur pulley teeth) * (π * diameter of wheels in km)  = distance

Can I ask what is endless ride?
```

---
## \#11 Posted by: AreaKruzer Posted at: 2018-06-18T04:52:30.788Z Reads: 291

```
For example if
TacABS = 1,096,400
Motor pole Pairs = 7

Wheel pulley = 36
Spur pulley = 16

diameter of 97mm wheels in km = 0.000097 km

((1,096,400 / 7) / (36/16)) * (π * 0.000097)
= (156,628.57142 / 2.25) * (0.0003047345)
= 69.612.6984 * 0.0003047345
=  21.213km

May have to simplify the calculation a little when coding it into a microchip like Arduino as we might not be able to represent 0.000097 properly in computer without using too much memory
```

---
## \#12 Posted by: Jc06505n Posted at: 2018-06-18T04:54:51.619Z Reads: 278

```
The only issue in regards to the ERPROM Is that it’s limited to 10000 writes (I believe that’s the write number) , and as @Ackmaniac said , if you were to write every 10Km, once you reach 1000km you would be in trouble.

Edit: I’m not a car guy AT All, how do cars odometer work?
```

---
## \#13 Posted by: AreaKruzer Posted at: 2018-06-18T04:55:38.119Z Reads: 266

```
that is why using a microSD would be a better idea.
```

---
## \#14 Posted by: Jc06505n Posted at: 2018-06-18T04:56:42.407Z Reads: 266

```
Agreed , right now , the only device is see capable of allowing such with connection tot he VESC is vaporware as of his moment (the new Photon LCD product)
```

---
## \#15 Posted by: AreaKruzer Posted at: 2018-06-18T04:59:47.038Z Reads: 268

```
i think it wouldnt be difficult to implement on the firefly remotes as well.

since on the VESC side, there will be an arduino with the NRF module, adding a microSD module shouldn't be too difficult.

if one worries that we are writing too much to the microSD, we can implement a function where if duty cycle is say 0% for 5sec, write it to the microSD once. if duty cycle is more than 0%, write to it maybe once every 30s/60s

we can still display the distance travelled without writing to the microSD. we can perform the writing of distance to the microSD periodically.

So if say the duty cycle is 0%, means the user has stopped. i think we do take more than 5s to bend down and turn off the power anyway.
```

---
## \#16 Posted by: Trdolan03 Posted at: 2018-06-18T05:09:58.265Z Reads: 261

```
Noob question. What is endless ride?
```

---
## \#17 Posted by: AreaKruzer Posted at: 2018-06-18T05:14:58.671Z Reads: 260

```
I googled about it and it seems to be cruise control?
```

---
## \#18 Posted by: koralle Posted at: 2018-06-18T05:15:51.042Z Reads: 264

```
https://youtu.be/AWWLP7TwsDU?t=2m6s
```

---
## \#19 Posted by: Jc06505n Posted at: 2018-06-18T05:18:28.052Z Reads: 262

```
[It’s a bit more](https://amp.reddit.com/r/MellowBoards/comments/5h45bg/what_exactly_is_endless_ride_mode_and_what_can/)

Imagine Riding in germany , you see a couple of cops , you resort to pushing , but the board cooperates , accelerated and metains that speed with you, allowing you to use your Board like a regular Board with an added ump
```

---
## \#20 Posted by: AreaKruzer Posted at: 2018-06-18T05:24:44.995Z Reads: 255

```
I see. So I figured it should be sensing the board upon reaching a said erpm, then do a gradual decay of the erpm
```

---
## \#21 Posted by: pixelsilva Posted at: 2018-06-18T06:13:27.740Z Reads: 236

```
Frigging neat idea. Heck, we should start hiring people to solve the most common challenges and hurdles we daily face inside our hobby.
```

---
## \#22 Posted by: pixelsilva Posted at: 2018-06-18T06:20:11.314Z Reads: 232

```
[quote="Eboosted, post:8, topic:59201"]
How about we all put down a deposit and pay to the first programmer/hardware developer team to accomplish this?
[/quote]

Same. :+1:
```

---
## \#23 Posted by: AreaKruzer Posted at: 2018-06-18T06:28:14.256Z Reads: 235

```
I would be up to do the programming using an Arduino. Where would you guys prefer the odometer to be displayed?

A separate screen that can be mounted to the front area of the board or displayed on a remote?
```

---
## \#24 Posted by: pixelsilva Posted at: 2018-06-18T06:31:51.081Z Reads: 242

```
@Wajdi is already working on his device called [Proton- Digital Instrument and Control Panel Touch Screen](https://www.electric-skateboard.builders/t/proton-digital-instrument-and-control-panel-touch-screen/58664)

![image|625x500](upload://O43Gtjn0A6wVKM6Wm9keQeaBOB.jpg)

![image|625x500](upload://lUsrrxmXnpcqzr8piawxRsyhyqf.jpg)

[https://www.electric-skateboard.builders/t/proton-digital-instrument-and-control-panel-touch-screen/58664](https://www.electric-skateboard.builders/t/proton-digital-instrument-and-control-panel-touch-screen/58664)
```

---
## \#25 Posted by: AreaKruzer Posted at: 2018-06-18T06:34:15.578Z Reads: 228

```
I am aware of that. If we are only displaying odometer and stuff. A smaller OLED screen would be more than sufficient
```

---
## \#26 Posted by: pixelsilva Posted at: 2018-06-18T06:37:17.086Z Reads: 236

```
Some of @Wajdi [Proton- Digital Instrument and Control Panel](https://www.electric-skateboard.builders/t/proton-digital-instrument-and-control-panel-touch-screen/58664) key features are:

* Touch screen - 240x320 2.8"
* Real time telemetry right at your sight all the time ( Speedometer, battery voltage, temperature, traveled distance…)
* Menu with different settings and options to adapt to your own configuration.
* Dual UART port for dual Vesc support
* Firmware updates through built-in micro USB, always up to date with latest Vesc changes.
* Built in LEDs driver with touch color picker, effects, front and back lights
* Easy to access and configurable riding preset modes.
* Benchmark mode
* Configurable sound alerts for low voltage, power on, …
* Miles/Km units
* Ultra fast refresh rate
* Does not require the Photon remote or receiver, works with any standard remote

![image|625x500](upload://90alti9f2G6QOJKTQ57zoHlyTni.jpg)

...we can work with him and include the odometer.
```

---
## \#27 Posted by: Tuomalar Posted at: 2018-06-18T07:24:14.469Z Reads: 209

```
”Endless ride” is a bit weird name for that. IMO it’s more like ”kick assistance”
```

---
## \#28 Posted by: AreaKruzer Posted at: 2018-06-18T09:18:28.050Z Reads: 217

```
I managed to code out the code in an Arduino that have an odometer of up to 100 million km.

I will implement the code into my VESC telemetry to do some testing on bench for that. As I do not have a microSD module, i am unable to code out the reading and writing of the microSD at the moment. The stuff should be coming in next week or so.
```

---
## \#29 Posted by: Wajdi Posted at: 2018-06-18T16:59:07.724Z Reads: 213

```
[quote="pixelsilva, post:26, topic:59201"]
…we can work with him and include the odometer.
[/quote]
But it does already have odometer implemented :wink: 
Lifetime data is stored in an SD card.
```

---
## \#30 Posted by: lennylogs Posted at: 2018-06-18T19:10:41.778Z Reads: 205

```
push to start is a good idea. or id like to be able to turn on my board via the remote
```

---
## \#31 Posted by: koralle Posted at: 2018-06-18T19:35:17.755Z Reads: 196

```
[quote="lennylogs, post:30, topic:59201, full:true"]
push to start is a good idea. or id like to be able to turn on my board via the remote
[/quote]

First world problems........... 

Endless Mode is the most important feature. Haha

And I think one of the easiest to implement. I think if we ask Vedder with a group donation and a pretty please, he might go for it.
```

---
## \#32 Posted by: CHAINMAILLEKID Posted at: 2018-06-18T19:39:10.408Z Reads: 181

```
Push to start and Endless mode would go hand in hand I'd think.
```

---
## \#33 Posted by: Jc06505n Posted at: 2018-06-18T19:41:04.159Z Reads: 184

```
The only issue I have in regards to turn on via remote is that , It would require either 

A) The Reciever to be always on. Even in a low state mode , and than drains battery. I.T’ll Be like having an inboard. Ganna be dead by morning (or at the very least constantly drawing your cells. 
B) a power source that has to be Charge separately. One battery pack is enough to be managed on one board. 

I get the appeal of it (making it like a car with car keys). But on these unpredictable little things, the best solution to work around making the battery work more , the better.
```

---
## \#34 Posted by: Jc06505n Posted at: 2018-06-18T19:43:54.192Z Reads: 181

```
You would have to activate with a remote (most likely the firefly and its derivatives since they are the most customizable in terms of modularity)
```

---
## \#35 Posted by: mikenyc Posted at: 2018-06-18T19:45:08.585Z Reads: 186

```
[quote="pixelsilva, post:22, topic:59201"]
> How about we all put down a deposit and pay to the first programmer/hardware developer team to accomplish this?
[/quote]


wouldn't it be a better idea to up the $ donations to @Ackmaniac  and ask him to do it?
```

---
## \#36 Posted by: Jc06505n Posted at: 2018-06-18T19:49:14.144Z Reads: 182

```
It would , but it’s up to him if he wants to do it. We can maybe hold a “Group Buy” for him to implement this feature in an Escrow Account and give it to him upon release implementation.
```

---
## \#37 Posted by: lennylogs Posted at: 2018-06-18T19:50:11.807Z Reads: 184

```
wow i had no idea "endless ride" was actually a thing. would definitely donate
```

---
## \#38 Posted by: mikenyc Posted at: 2018-06-18T19:51:01.534Z Reads: 186

```
I don't think escrow is necessary lol. He's a pillar in the community
```

---
## \#39 Posted by: pixelsilva Posted at: 2018-06-18T19:52:46.445Z Reads: 187

```
Yeah, and not only that, hire full time engineers, programers and industrial designers to try solve our oldest and most common technological challenges we've face for years.
```

---
## \#40 Posted by: squishy654 Posted at: 2018-06-18T19:53:26.028Z Reads: 191

```
I don't need any of those features, they all seem unnecessary for normal operation and some seem unsafe. What ever happened to removing things to solve problems? Why make it more complex and delicate for nothing but novelty when we barely have robust eskates as it is? I say spend the time, money and energy working on polishing what exists before reinventing the skateboard..

Endless ride? Is this like cruise control so when you fall off it will keep going without load and smash into a pile of kids walking down the street? No thanks..and I don't really want anyone with such a feature on the street near my kid either.

Lifetime oddmeter would make sense if we had robust vehicles that didn't break down all the time needing replaceable parts, in fact most companies cannot even get that right yet, let alone something solid enough to make a lifetime oddmeter useful or relevant...is each part gonna have one, because during the life of the skateboard it will most likely be entirely replaced due to maintenance..instead of making one of these work on making eskates worthy of them 1st..

Push to start? Why? are you people that lazy you cannot be bothered to push a buttom or flip a switch? HAHAHA when I was a kid, we imagined things being so easy we just push buttons to make it happen, we are living in the future I dreamed about and yet you are so lazy it's not good enough? If a board can turn on from motion sensing, then it can turn on at weird times too, like sitting in the truck of my car going over a bump or hitting the wheels on something while carrying it, or worse, turn off while riding because you opened the door to another complex feature having errors or going wrong, when you never needed too...hell I have a board without a switch or loop key, you must plug it in...low and behold it's one of the toughest and most robust builds I own...go figure..this is a feature which will require hardware and software, and be used for a second or two when turning on the board, overall it's a waste of space and weight on the board for a feature than will be used .001% of the time you are using the eskate...it's as novel to me as bluetooth speakers (completely unneeded and unless to the operation of the vehicle for it's purpose). Its like saying the switches or loopkeys are broken and don't work, when they work just fine...stop falling for Chinese factory marketing bull..they are simply trying to make crappy board stand out when they cannot even get the range above 10 miles on a charge...priorities are wack on this one...

Power off via remote? Doesn't evolve already feature this? like when all those people crashed from brown outs or failsafe failure when the remotes disconnect? This just seems like an accident waiting to happen, someone will hit it in error and fly off the board, when they never needed it to begin with...

I believe you shouldn't fix a problem if you don't have a problem. I believe the more components and parts and features anything has, the more can go wrong with it. I enjoy fixing problems by removing things, not adding things. Complexity hurts robustness, and until you have a problem that these features fix, there is absolutely no reason to talk about them...how about talking about rider ability instead, adapting to the eskate and shredding it better than the next guy? Isn't that a more worthy waste of time over developing features no one needs that hurt the overall robustness of your eskate? Sorry, just being honest here..
```

---
## \#41 Posted by: Jc06505n Posted at: 2018-06-18T19:56:33.688Z Reads: 165

```
I only says this because if this thing does lift off, it's going to, eventually, be a regular thing. We might see developers holding "Group Buys" to implement a feature. (sounds ridiculous now, but sinking hours ant free) 

I trust Ack, he's never given me a reason not to, but we do have to set a standard for how we want things thing to move if this thing does happen and many more after. If we don't, I guarantee we'll have another Alex fiasco, only this time, it's all of us.
```

---
## \#42 Posted by: mikenyc Posted at: 2018-06-18T20:02:49.169Z Reads: 165

```
I like the idea of push assist. I don't like calling it endless ride. 

that said, I agree with everything you said. who needs lifetime data? really? what's the point? same goes for push to start? "lol" is my only response to that.
```

---
## \#43 Posted by: mikenyc Posted at: 2018-06-18T20:03:28.065Z Reads: 165

```
why even compare him to alextech?
```

---
## \#44 Posted by: ducktaperules Posted at: 2018-06-18T20:04:01.441Z Reads: 166

```
[quote="squishy654, post:40, topic:59201"]
I believe the more components and parts and features anything has, the more can go wrong with it.
[/quote]

Many boards like boosted have power off via remote but i have never seen a board with power ON from remote. I agree that more features means more things that can go wrong but power switching from remote would have the potential for boards without power buttons. that means less mechanical parts to fail and less holes to drill in waterproof enclosures.

Also endless mode wouldn't be good for everyone but realistically it should be a very easy to implement.
```

---
## \#45 Posted by: Dyspro Posted at: 2018-06-18T20:06:13.043Z Reads: 158

```
@evoheyax was looking to get into programming haha.
```

---
## \#46 Posted by: squishy654 Posted at: 2018-06-18T20:07:03.039Z Reads: 157

```
such a feature requires bi-directional RF communications (as does telemetry)...you cannot tell me that it takes less parts and code to accomplish, I ain't dumb..lol Not to mention battery draining always on hardware...no thanks..
```

---
## \#47 Posted by: trancejunkiexxl Posted at: 2018-06-18T20:07:59.381Z Reads: 155

```
Lots of cool ideas, I would like to see dead zone marker so when I rode through a crappy area, I can get a heads up so I can avoid it and not have to remember .. necessary not really but I donno.. maybe Frequency hopping would be cool
```

---
## \#48 Posted by: mikenyc Posted at: 2018-06-18T20:09:11.309Z Reads: 152

```
Well for starters, you'd need to have an integrated power switch. Last I checked, @Ackmaniac works on the firmware/software, not the hardware. :)
```

---
## \#49 Posted by: squishy654 Posted at: 2018-06-18T20:09:27.570Z Reads: 154

```
I wouldn't mind getting a "overspeed" warning light or beep on my remote, that's a useful and safe feature I could use...I would like to know when I'm over the rpm limit of the motor so I know when I hit the throttle if it's going faster or gonna slow down and buck me off...
```

---
## \#50 Posted by: ducktaperules Posted at: 2018-06-18T20:16:40.292Z Reads: 153

```
I never said it takes less parts or code. 

I was just suggesting that power via remote could have other benefits which might justify the complexity. I would rather some extra hardware than having a mechanical power switch.

And for endless mode we already have cruze control, its just a version of that where the target speed decays over time, doesn't slow you down and if your speed is higher than the target speed then you increase the target speed.
```

---
## \#51 Posted by: skatardude10 Posted at: 2018-06-18T20:16:59.016Z Reads: 155

```
I don't think an endless ride feature would be too much complexity to add to an already complex system though. 

I love pushing around my longboards. I could care less for cruise control honestly, but I'd absolutely love to be able to super push around my best longboard (my eskate) as if it were a featherweight longboard with super ceramic bearings.

Personally, this is a feature that would totally change the game for me. Just the other day I was riding my eskate with some longboarders. It was a pain enough trying to throttle my board just right to where they didn't feel like I was going too fast or too slow, and my board is heavy enough that I don't want to kick it with no power and fall behind. This alone is *not* a reason to add an endless ride feature.... *but* I do see a leasurely cruise around town, not having to hold a remote all the time, whatever, all the use cases combined getting closer to skateboarding in general as reason enough to add such a feature. Essentially a software update that adds such flexibility sounds great. I'm willing to risk a bit more complexity in a compiled binary or hex for that.

TLDR: I want to kick push. But I don't want to kick push 25 extra lbs.
```

---
## \#52 Posted by: squishy654 Posted at: 2018-06-18T20:20:16.298Z Reads: 146

```
If you love pushing around longboards, then why not just go push around longboards? why ruin eskates?

I love to push and pump as well, that's why I own a gbomb and a number of high end boards for doing just that...
```

---
## \#53 Posted by: ksfacinelli Posted at: 2018-06-18T20:24:59.413Z Reads: 142

```
I use an application called Waze for driving information.  I am sure many of you also are aware or use this app.  I think a version for skateboarding could be cool....if you are not familiar with the app do a little research as it is very useful for car drivers.
```

---
## \#54 Posted by: skatardude10 Posted at: 2018-06-18T20:25:35.507Z Reads: 143

```
Because I want to power up hills sometimes.

How is adding an optional firmware feature ruining existing features? 

It's just like, if you don't want to run sensored, don't... It's that simple. If you don't like it, it's not mandatory.. doesn't ruin anything for you right? 

As much as I like pushing around, I always wanted the option to push a remote and fly up the hill instead. If I can have the option, why not both? 

Push the flats, coast downhills, fly uphill... Sounds great to me and is no problem for you if you don't want to use such a feature. How is that ruining eskate for you?
```

---
## \#55 Posted by: CHAINMAILLEKID Posted at: 2018-06-18T20:29:36.119Z Reads: 147

```
[quote="squishy654, post:40, topic:59201"]
Lifetime oddmeter would make sense if we had robust vehicles that didn’t break down all the time needing replaceable parts, in fact most companies cannot even get that right yet, let alone something solid enough to make a lifetime oddmeter useful or relevant…is each part gonna have one, because during the life of the skateboard it will most likely be entirely replaced due to maintenance…instead of making one of these work on making eskates worthy of them 1st…
[/quote]

This is a silly complaint IMO.

First off, You basically already have everything you need for an odometer w/ an electric skateboard. The only thing you really need to do is store that data.

But the main reason its silly is... Cars need maintenance and replacement parts and all that. And we use the odometers as a baseline for everything. Your motor and your wheels and your transmission don't all need their own odometer, you just track them all relative. 

My board has what's trying to be a lifetime odometer. It doesn't quite work exactly as intended. I still really think its a good QOL feature. It's not reliable enough to tell the actual lifetime, but I can check how much I've ridden in a given week, or day. I'm not limited to the trip odometer. Its nice.
```

---
## \#56 Posted by: squishy654 Posted at: 2018-06-18T20:29:51.895Z Reads: 140

```
@skatardude10

you have to be more specific, what feature are you talking about?
```

---
## \#57 Posted by: CHAINMAILLEKID Posted at: 2018-06-18T20:31:40.993Z Reads: 139

```
[quote="squishy654, post:52, topic:59201"]
If you love pushing around longboards, then why not just go push around longboards? why ruin eskates?
[/quote]

Uhh, What?
```

---
## \#58 Posted by: Wajdi Posted at: 2018-06-18T20:32:29.819Z Reads: 138

```
I have actually been discussing endless riding a while back, and been experimenting with it for some time now. It’s not really hard to implement, and was thinking about adding that feature on my upcoming control panel. It still has a lot of processing power left to add many features, if many are interested in endless riding, I will definitely add it.
```

---
## \#59 Posted by: squishy654 Posted at: 2018-06-18T20:33:48.152Z Reads: 135

```
What prevents a eskate from continuing on without a rider in endless mode? anything? because that would get regulated through laws in no time if deemed unsafe to those not on the board..
```

---
## \#60 Posted by: squishy654 Posted at: 2018-06-18T20:36:21.756Z Reads: 134

```
There was already a case of a runaway board in San Fransisco that went full throttle and hit a cable car and then caught fire...just saying the last thing we need is a feature that results in uncontrolled runaway eskates..
```

---
## \#61 Posted by: oyta Posted at: 2018-06-18T20:36:45.665Z Reads: 127

```
But you still have the remote in your hand and touching the break should end the Endless Mode.
```

---
## \#62 Posted by: Jc06505n Posted at: 2018-06-18T20:41:26.476Z Reads: 142

```
[quote="squishy654, post:40, topic:59201"]
I don’t need any of those features,
[/quote]


Nice, no one does. 

[quote="squishy654, post:40, topic:59201"]
they all seem unnecessary for normal operation and some seem unsafe.
[/quote]

ES8's are Unnecessary. Wake up early to Ride that Public Transportation. Everything's unsafe until you make it safe. 

[quote="squishy654, post:40, topic:59201"]
What every happened to removing things to solve problems?
[/quote]

You don't remove things, you make things efficient to solve problem. If i were to remove a BMS because it presented a space problem , I would be fixing the space problem , but opening myself to future issues. 

[quote="squishy654, post:40, topic:59201"]
Why make it more complex and delicate for nothing but novelty when we barely have robust eskates as it is
[/quote]

Because we see these features implemented on industrial skates with little known problems being a result of them. This is a thread for implementing *already used features* in industrial boards.

[quote="squishy654, post:40, topic:59201"]
I say spend the time, money and energy working on polishing what exists before reinventing the skateboard
[/quote]

a portion of this thread actually talks upon hiring engineers and teams to tackle the existing problems we have...

[quote="squishy654, post:40, topic:59201"]
Endless ride? Is this like cruise control so when you fall off it will keep going without load and smash into a pile of kids walking down the street? No thanks…and I don’t really want anyone with such a feature on the street near my kid either.
[/quote]

Probably, same thing as cruise control, so the result of the feature would still occur with or without it's existence. and since there's already mellow riders with those features and there hasn't been reported accidents thus far..

[quote="squishy654, post:40, topic:59201"]
Lifetime oddmeter would make sense if we had robust vehicles that didn’t break down all the time needing replaceable parts, in fact most companies cannot even get that right yet, let alone something solid enough to make a lifetime oddmeter useful or relevant…is each part gonna have one, because during the life of the skateboard it will most likely be entirely replaced due to maintenance…instead of making one of these work on making eskates worthy of them 1st…
[/quote]

Doesn't mean we shouldn't shoot for such a feature... And it's beyond just an odometer. Lifetime data that allow us to see the entire life of the board along with faults, max temp , speed, efficiency, and other data that can contribute to refining the perfect configuration. 

[quote="squishy654, post:40, topic:59201"]
Push to start? Why? are you people that lazy you cannot be bothered to push a buttom or flip a switch?
[/quote]

Ooooor maybe it's nice to push your board , have your remote on and just GO. re-Implementing the SK8 in ESK8...

[quote="squishy654, post:40, topic:59201"]
HAHAHA when I was a kid, we imagined things being so easy we just push buttons to make it happen, we are living in the future I dreamed about and yet you are so lazy it’s not good enough?
[/quote]

Danm, pack it up everyone , more innovation is bad guys!

[quote="squishy654, post:40, topic:59201"]
Power off via remote? Doesn’t evolve already feature this? like when all those people crashed from brown outs or failsafe failure when the remotes disconnect? This just seems like an accident waiting to happen, someone will hit it in error and fly off the board, when they never needed it to begin with
[/quote]

More Like Boosted's proven implementation. I do it everyday making the turn off process a one man unit. It makes sure that i never leave either device on once i get into the grove of doing it everyday, especially when i have to keep it moving from the streets to my work building.

[quote="squishy654, post:40, topic:59201"]
I believe you shouldn’t fix a problem if you don’t have a problem.
[/quote]

I believe you should innovate to higher standards. ESK8 has yet to reach its full potential. 

[quote="squishy654, post:40, topic:59201"]
I believe the more components and parts and features anything has, the more can go wrong with it.
[/quote]


Agreed. Which is why you should work as soon as possible to perfect and make these features an efficient part of the system.

[quote="squishy654, post:40, topic:59201"]
Complexity hurts robustness, and until you have a problem that these features fix, there is absolutely no reason to talk about them
[/quote]

You mean other than the fact that there's a demand for them. This world isn't driven by what's *needed*, but by what's *wanted*. And people obviously want these ,  just as they want a cheaper VESC6, or a Heatsink enclosure or a $900 alternative to a car. 

[quote="squishy654, post:40, topic:59201"]
how about talking about rider ability instead, adapting to the eskate and shredding it better than the next guy?
[/quote]


And you contribute to that, and that's your thing.. But not everyone ride esk8's to be a better rider to the next guy. I ride it because it feels good and i, along with others, believe their experience will be better with these features. 

[quote="squishy654, post:40, topic:59201"]
Isn’t that a more worthy waste of time over developing features no one needs that hurt the overall robustness of your eskate? Sorry, just being honest here…
[/quote]

Hmmmmm no. And so am I
```

---
## \#63 Posted by: squishy654 Posted at: 2018-06-18T20:42:04.142Z Reads: 112

```
[quote="oyta, post:61, topic:59201"]
But you still have the remote in your hand
[/quote]

I cannot tell you how many times I have seen friends bail, hit the ground and the remote flies outta their hands...in fact it's such a thing we prefer tough remotes that can handle it without breaking...I fear there is a lack of experience behind these ideas...in the real word is where I ride...shit happens and safety needs to be considered...shut the doors to unsafe situations and stop opening them up with unsafe feature ideas, think these these things through, run scenarios and ask yourselves if it's really helping anyone...eskates do no require any of these features to operate correctly or safety...adopting unsafe features for novel reasons is asking for trouble...quite literally..
```

---
## \#64 Posted by: skatardude10 Posted at: 2018-06-18T20:42:05.567Z Reads: 118

```
Good point. I think reasonable settings could help with this... A failsafe such as remote connection being lost, or the board during endless ride slowing down on its own similar to a longboard would be good enough.  Even opposed to a longboard that would gain speed down a hill, if you are riding endless mode, your board could slowly slow itself down even going down a hill... 

You can mess up programming your eskate with bad settings, it would be similar enough with an endless ride mode. I don't see much trouble coming from that personally, outside the oddball bad/dumb settings being set.
```

---
## \#65 Posted by: squishy654 Posted at: 2018-06-18T20:43:29.548Z Reads: 115

```
@Jc06505n

You misunderstood much of what I said, I didn't make it past your third or fourth point dude, sorry...
```

---
## \#66 Posted by: Jc06505n Posted at: 2018-06-18T20:43:46.962Z Reads: 118

```
I didn't...I compared the reality of this, this being Group buy for features, ending up like an Alex Fiasco in the future. Maybe I should edit to clarify ?
```

---
## \#67 Posted by: Toughook Posted at: 2018-06-18T20:44:04.612Z Reads: 122

```
Can only think the usefulness of an odometer on a shop bought, unmodified, completely stock eSK8. DIY eSK8 are like 'Triggers Broom' in their lifetime and a figure of total miles ridden will have little practical use on the second-hand market. Sure it might be nice once in a while to check how far you have ridden, but to what end? I just don't see the point except for individual rides, but a plethora of phone apps exist to track your journey anyway.

Endless Ride bothers me. I built an eSK8 so I can travel power assisted. Can't remember the last time I wished I could get out and push on a snowboard 😂

Remote power on. Only if the ON/OFF relay is powered discretely from the main battery pack. 

Push to start. Again, not for me and I agree with the reasons posted above as to why it's a bad idea.

I realise all I'm doing here is being negative, but right now I can't think of anything that isn't a gimmick that needs to be added to what's already available. Maybe front/rear light control from remote, or a horn/warning sound triggered by remote (verbal shouting could be muffled inside a full face helmet) ?

Keep things as simple as possible I say.
```

---
## \#68 Posted by: Jc06505n Posted at: 2018-06-18T20:47:13.219Z Reads: 115

```
[quote="squishy654, post:46, topic:59201, full:true"]
such a feature requires bi-directional RF communications (as does telemetry)…you cannot tell me that it takes less parts and code to accomplish, I ain’t dumb…lol Not to mention battery draining always on hardware…no thanks…
[/quote]


Novice here, But don't we already have that with Remotes (i.e Firefly)? Send a signal to receiver to the VESC to turn off? Again, I'm not an expert in this matter.
```

---
## \#69 Posted by: oyta Posted at: 2018-06-18T20:53:51.530Z Reads: 115

```
[quote="squishy654, post:63, topic:59201"]
I cannot tell you how many times I have seen friends bail, hit the ground and the remote flies outta their hands…in fact it’s such a thing we prefer tough remotes that can handle it without breaking…I fear there is a lack of experience behind these ideas…in the real word is where I ride…shit happens and safety needs to be considered…shut the doors to unsafe situations and stop opening them up with unsafe feature ideas, think these these things through, run scenarios and ask yourselves if it’s really helping anyone…eskates do no require any of these features to operate correctly or safety…adopting unsafe features for novel reasons is asking for trouble…quite literally…
[/quote]
I fully understand your security concerns. However I think they are solvable. I also ride in the real world :wink: but still I think it is possible to implement this kind of feature with sufficient security. This is where the innovation comes in. I don't have the solution now - it demands knowledge of the system, code, development and testing.
```

---
## \#70 Posted by: squishy654 Posted at: 2018-06-18T20:54:16.335Z Reads: 118

```
[quote="Jc06505n, post:68, topic:59201"]
Novice here, But don’t we already have that with Remotes (i.e Firefly)? Send a signal to receiver to the VESC to turn off? Again, I’m not an expert in this matter.
[/quote]

Sure, in fact any bi-directional telemetry remote control will be able to do this if wired to a solid state switch, too easy. I lack such a remote, and some use bluetooth adapters for the communications to a phone or external device, that makes tons of sense to me, while adding the complexity of bi-directional RF for this feature makes zero sense...the firefly has it for a non novel reason, telemetry most likely, so it's already there and you are not making it more complex than it already is...but for 99% of the eskates out there (single way RF comms) there's no point in trying to add it...historically the comms coming from the rx on such systems are weak and unreliable, and I wouldn't put the main power switch on such a unreliable connection...this is why we use 2.4ghxz spread spectrum for control, and bluetooth for telem...bluetooth control riders have experienced many issues in urban environments and it's an unsafe protocol for such use..basically get into transceivers instead of TX and RX, things like data radios...sorry but I would much rather have a purpose built control system, robust and solid as hell, error correction, spread spectrum in an RF that isn't saturated or dealing with a high noise floor in rban environments.,..we are quite literally putting our life in the hands of that RF signal...you might want to learn about how robust it is and how you can make it better before adding features that cripple it..
```

---
## \#71 Posted by: Jc06505n Posted at: 2018-06-18T20:58:04.403Z Reads: 107

```
It seems everyone's having a hard-time grasping a simply concept here cause i keep seeing the same thing: *If your not going to use it don't*. Many don't use Cruise Control but others still do. **You not using a feature is not an excuse for it to not be implemented**... so longs as it's something that someone *can* use, it's merit-able to look at and see if the implementation is worth the integration. 

I love the debating that's going on here, I do,  it's what's needed to progress for both the industry and DIY scene, but people are looking at their side of the picture instead of all of it... The fact is this: ESK8s are going to continue to progress in things that are both needed and un-needed. 

After all, how many of us have a BT Mod in our boards? A Friefly? Lights? Go Pros Attachments? Photon Remotes? None of the above is needed yet were all ready to throw money at them! All i'm saying is , The criticism on implementing "non-needed features" when we buy un-needed things on a daily basis. If you don't want it and it's not for you , keep it stepping, but don't be arguing against the advancement of ESK8's
```

---
## \#72 Posted by: squishy654 Posted at: 2018-06-18T21:03:52.562Z Reads: 103

```
Your definition of "advancement of eskates" and mine are very very different...partly because I realize and accept that we don't even have good decks, trucks and wheels for them yet, let alone robust drive systems and bombproof speed controllers...to me we don't even have a completed eskate to begin adding novelty too...do we ride for hundred or thousands of miles on the DIY builds we already make? sure do...and I still find them lacking in many respects...I'm not against new ideas, innovations and novelty, hell I just put in a 50watt speaker system into my last build, I am no stranger to admitting novelty and useless features...BUT...I believe the time of those wishing to innovate could be better spent on finishing the work already started before working on things we don't need...there's just too much we still need, for me to look for things I don't...
```

---
## \#73 Posted by: Jc06505n Posted at: 2018-06-18T21:05:38.310Z Reads: 109

```
Keep in mind that Odometer here is being used Synchronously for Lifetime Data which includes (Top speed, , list of lifetime faults, lifetime displacement, average and median Efficiency, etc), useful data than can be used for further research and tuning. 

[quote="Toughook, post:67, topic:59201"]
Push to start. Again, not for me and I agree with the reasons posted above as to why it’s a bad idea
[/quote]

Can someone explain to me why this is a bad idea? There's already industrial boards that have this feature no problem and any faults they have are not linked to this feature. If its a safety concern , then like any other feature, it's toggleable by the rider. Simple.
```

---
## \#75 Posted by: ducktaperules Posted at: 2018-06-18T21:08:51.513Z Reads: 118

```
So here is a crazy hopefully PRODUCTIVE idea . . .

Seems like the nRF51822 is becoming the new standard Bluetooth module. It is the only module officially supported by the VESC tool and there are versions avalable from Trampa and Metr as well as avalable code if you want to diy.

The nRF51822 has a butload load of flash memory and is already connected to the Vesc's uart, it could easily be used to store a lifetime mileage. 

The nRF51822 is also designed to be a Bluetooth Low Energy chip. It can act as a BLE beacon transmitting status 10 times a second for less than 220uA (~2 years battery life on a single 18650). It also has its own AtoD and other I/O capability's. some modules such as the Metr Pro by @rpasichnyk and @hexakopter already has "Additional nRF52 pinouts" broken out on the back of the module. 

Imagine a board including this module permanently powered. You could have lifetime odometer that is viewed from an app. If you connect AtoD to your battery the module could shut its self down in low voltage conditions to avoid battery damage. This would also allow battery monitoring whilst charging or whilst the board is off, imagine getting a notification when charging completes :slight_smile: 

Additionally a firefly style remote using another nRF module could easily tell the board to power up or down remotely. The new generations of VESC seem to be starting to include their own antispark switch so its not unreasonable to control this from a spare pin on the nRF. Using the same module for remote and bluetooth would also remove the need to have extra arduinos and rf modules inside the board, removing both complexity and possible interference.

Any CONSTRUCTIVE Thoughts?
```

---
## \#76 Posted by: Jc06505n Posted at: 2018-06-18T21:22:50.491Z Reads: 113

```
[quote="squishy654, post:72, topic:59201"]
Your definition of “advancement of eskates” and mine are very very different
[/quote]

I don't think so, we just have a different way of going about it, You want to stick and refine the fundamentals, i want to take what's proven to work so far, improve it, and then implement it.

[quote="squishy654, post:72, topic:59201"]
good decks
[/quote]

@treenutter says hello...

@Hummie says hello...

[quote="squishy654, post:72, topic:59201"]
trucks
[/quote]

That's subject, Caliber 2's with Skateboard Knowledge Modifications are just fine for ESK8s, unless you cna tell me why they aren't?  

[quote="squishy654, post:72, topic:59201"]
wheels
[/quote]

This I kinda agree but I just see it as wheels wearing out faster than in normal skateboard use. Doesn't make them bad.


And mind you , each of the above have forum members working on perfecting them. But Just because they aren't at perfection doesnt mean we should wait for others to finish up. Screw that, while treenutter is making his awesome decks, I want to refine an appropriate odometer system that allows for a user to visualize their lifetime data and make improvements based on what they see so far, whether its changing gears ratios or trying out a new drive all together. 

While Hummies is making the ultimate Hub motors i want to refine a push to start system that allow ESK8's to feel closer to a Skateboard!  **And we can't make it safe unless we try**  Nothing is perfected unless experimented and tried out for as many times needed. 

I just want you to understand that there's nothing stopping the synchronous development of what's needed and what's wanted. 

So how about this: _Two Threads_, This one will be Dubbed: " Leisure Features We Could Implement " and another " ESK8 Components that need to be improved". Both threads will serve the purpose of **recruiting , debating,discussing, and ultimately funding individual / teams to pursue the prototyping , implementation , and production of their respective purposes.**  

This way what's in need of existing and being improved is being addressed and actively worked on (via funding incentive) instead of waited on , and what's desired is also being created.
```

---
## \#77 Posted by: ducktaperules Posted at: 2018-06-18T21:34:25.239Z Reads: 103

```
"ESK8 Components that need to be improved" is basically every post in this forum where someone is moaning about how shit something is. We don't need anther thread dedicated to that.
```

---
## \#78 Posted by: Jc06505n Posted at: 2018-06-18T21:38:30.033Z Reads: 110

```
The difference would be that it would be the Main, cumulative thread. A sum of what what needs to be approved all in priority by the community. If every post really is "someone [moaning] about how shit something is", then even more reason to have a thread that not only addresses it, but aims to provide a solution (one being community discussion and funding) towards it. I plan on updating these Threads every week with the intentions of making it Publicly editable (Wiki) once it's more organized.
```

---
## \#79 Posted by: skatardude10 Posted at: 2018-06-18T21:59:22.593Z Reads: 117

```
But, the people who program may not be adept at CAD, manufacturing and distribution... and vice versa. Just because some areas may be lacking in innovation doesn't mean that people with other skillsets should stop innovating until people in other areas catch up.
```

---
## \#80 Posted by: lock Posted at: 2018-06-18T22:38:52.119Z Reads: 121

```
[quote="ducktaperules, post:75, topic:59201"]
Seems like the nRF51822 is...
[/quote]

I think the nrf51 has a bit to offer. Cheap, and it’s a SoC, so no need for an Arduino, etc. Started having a play round with Vedder’s code and a cheap oled, basically parts I had left over from my build.

![image|502x500](upload://rllpuT2TTedqz2GvB7rfw6AJZym.jpeg)

No real firm plans as to what I want it to do. Really just wanted to see if it could drive a small oled... Maybe just intercept and display various VESC commands. Guess you could also use it on a remote side. 

Will post a thread/source if I ever get it to do something interesting.
```

---
## \#81 Posted by: brenternet Posted at: 2018-06-18T22:55:23.414Z Reads: 124

```
I'd be down to donate towards programming, I like the idea of endless ride and push to start - they should be relatively simple to achieve?

Just a quick note. If you're against some of the ideas here you can just state that it's not for you and decide not to follow the thread, taking a personal crusade against every idea that is not your own seems counter productive in every sense of the word. You can have apposing views from your peers and still respect theirs.
```

---
## \#82 Posted by: Ackmaniac Posted at: 2018-06-18T23:10:02.166Z Reads: 129

```
Did anybody test the endless ride feature from mellow?
My firmware mod has already a mod that comes close (and if you ask me i think it's even better because it is safer)
To be honest i think they got the idea from me (because they came up with that after i published my idea)
![image|690x442](upload://aXonXRtKGPoYfdd7JNbMueQvtYI.png)

Difference is that you have to pull the throttle and hold it to activate it. Other difference is that it doesn't decrease the speed over time. Only when you become slower than 1500 ERPM from the speed that is set then the speed decreases so that the board doesn't actively accelerate you.
The idea that the board assist you while you push is really nice. But practically i think it is horrible because the boards behavior will be unpredictable and act like it has it's own mind.

Don't know how melow does it exactly unless somebody tells me the opposite. I think this mode is more for marketing and to create the illusion that the board becomes legal (which isn't the case).
```

---
## \#83 Posted by: mikenyc Posted at: 2018-06-18T23:16:20.595Z Reads: 124

```
I had a mellow. It was the best feature of the board. Other than that, it was an underpowered waste of money.

I think I mentioned this to you in our private dialogue. The inability to propel the board without pushing is probably designed to get around laws that prohibit fully electric skateboards, scooters and eBikes. If you can demonstrate that the board won’t function without pushing (and no throttle), then you should be good. The remote is used for braking.

Here’s one link. 

https://techcrunch.com/2018/04/03/nyc-paves-the-way-for-pedal-assist-bike-sharing/

There was another article better describing the law. Basically saying that it can assist up to 20 mph, but it can not maintain that speed on its own without human input. Meaning, it must gradually decline and require more physical activity to increase speed again.
```

---
## \#84 Posted by: skatardude10 Posted at: 2018-06-18T23:16:45.760Z Reads: 125

```
I need to try this mode! I wasn't aware of it! I may remember you mentioning it elsewhere, but I think I thought it was something else... And certainly not just a mode I could set on your app 😎
```

---
## \#85 Posted by: mikenyc Posted at: 2018-06-18T23:29:21.101Z Reads: 126

```
I should add that once you hit the brake, the cruising disengages and you slow to a stop unless you push again.
```

---
## \#86 Posted by: Ackmaniac Posted at: 2018-06-18T23:35:36.815Z Reads: 125

```
When the cruise was already active, how did the board behave when you pushed again. And how did you activate the mode? Just try to explain as detailed as you can. A simple "I had a mellow. It was the best feature of the board" doesn't help much.
```

---
## \#87 Posted by: mikenyc Posted at: 2018-06-18T23:43:02.411Z Reads: 126

```
On the remote, you toggle down to endless mode. This disabled the remotes throttle function. To move forward you stood on the board and pushed like a normal skateboard. On a normal skateboard, if you gave it a good push (and depending on the incline, flatness, or decline) you could coast for maybe 5-15,  20 seconds? This would extend that to maybe 30-40 seconds. If you needed to stop, you could hit the brake, and it would brake as normal, but you would have to kick up to speed again.

I think the key takeaway is that the board eventually stops if you don’t push
```

---
## \#88 Posted by: CHAINMAILLEKID Posted at: 2018-06-19T02:24:15.339Z Reads: 121

```
Ok so reading through the discussion here, I've come up with an unusual idea.

So first imagine a nice tiny little micro cruiser, like maybe 25-27".
 
Just a little get around board, you can fit it in lockers, carry it on the bus or on the train. Its a little under powered to keep it manageable.

But... 

It doesn't have a remote, it doesn't have buttons, it doesn't have nothing.

Its a push to start, augmented coast ( endless ride ) that lets you get around quickly with much less effort.

It also has an "assisted downhill", automatic braking that attempts to keep your speed under ~15-17-ish, helping to get around more safely and not lose control.

It wouldn't need as big of a battery.
It wouldn't need any wireless implementation at all.
Just single cheap hub motor might work if its not too big for the small deck.

Anybody else think that sounds kinda appealing?
```

---
## \#89 Posted by: trancejunkiexxl Posted at: 2018-06-19T02:25:55.100Z Reads: 116

```
at least some kinda mechanical brake and im down :joy:
```

---
## \#90 Posted by: kylem21 Posted at: 2018-06-19T05:23:02.859Z Reads: 115

```
If this panel offered push assist id have to buy it
```

---
## \#92 Posted by: mixedcreation Posted at: 2018-06-19T18:43:32.175Z Reads: 118

```
Agree with you on the Mellow Board.  That is the only feature worth a damn.  The endless mode was actually pleasant.  It was even better when applied to a board with a kicktail, as it seemed it was perfected matched with a skateboard, IMO.  I think just having this feature one a small air travel battery makes this the best small stealth board you could possibly have.  This feature flies under the radar because you must push for it to go at a constant speed that gradually declines.  It was nice.  I don't think I need this feature on every board, but on a small lightweight board, I think it can't be beat.  

@okp has a great video displaying [Endless Ride](https://www.youtube.com/watch?v=Ek56JtT3jD8)
```

---
## \#93 Posted by: Ackmaniac Posted at: 2018-06-19T18:59:34.954Z Reads: 116

```
How does it behave when you push. Does it recognize that you push and stop powering or does it continue while you move your push leg forward and then push.
And how long does it take that it starts to assist power at the new speed? Does it power all the time or does it take a second to assist at the new speed?
```

---
## \#94 Posted by: mikenyc Posted at: 2018-06-19T19:53:08.445Z Reads: 115

```
It matches the speed that you push at, it holds it for a few seconds, and then it slowly decelerates. Deceleration is powered, it's never a free wheel coast unless you activate the brakes, only then do you free wheel.
```

---
## \#95 Posted by: chinzw Posted at: 2018-06-19T20:17:41.454Z Reads: 116

```
That's what this is, minus the "underpowered" part. And i still do use a remote though.

![IMG_20180611_224744|666x500](upload://qSbheNUaoDdG3eIyGTCHPc9Wabn.jpg)
```

---
## \#96 Posted by: Jc06505n Posted at: 2018-06-19T20:27:25.794Z Reads: 115

```
I think the integral park is that the remote is only an entry and exit from this push assist mode, after that, moving is entirely dependent on the kick push you give and how long the system accelerates.
```

---
## \#97 Posted by: chinzw Posted at: 2018-06-19T20:41:33.112Z Reads: 115

```
How do you stop?
```

---
## \#98 Posted by: Ackmaniac Posted at: 2018-06-19T20:55:31.358Z Reads: 114

```
The interesting part is how it behaves while you push. I mean exactly the moment when you push. Because that is the moment you can easily loose balance.
Does it recognise that you push and stop powering or does it continue like when you stood still on it. And when you pushed to a new speed does it take a short moment before you can feel that it powers the motor or does it immediately adjust the motors power to the actual speed.
```

---
## \#99 Posted by: Jc06505n Posted at: 2018-06-19T21:19:45.707Z Reads: 114

```
You use the remote to disengage i believe.
```

---
## \#100 Posted by: ducktaperules Posted at: 2018-06-19T22:06:30.458Z Reads: 119

```
i have not used it personally but this is my understanding:
 - If you are riding at constant speed PID values should be stable with very little**P** (error) but positive **I** (accumulated error) maintaining power.
 - when you remove 1 foot to push it will still be maintaining speed as it will not know you are about to push.
 - As you start to push the speed will increase above the target speed. 
 - Once **current speed > target speed + threshold** then the system will begin to increase the target speed to match the current speed. There must be some sort of threshold so that normal osculations in **P** don't cause target speed to increase. 
 - As current speed and target speed increase together there will be no error so **P** will remain 0 and no more error will be accumulated so **I** will also remain constant. This provides constant but predictable power delivery whilst pushing.
 - once you stop pushing you will start to slow down again. Its likely that as your now moving faster you will need more power to maintain this new speed. This will cause **P** to begin increasing as well as causing **I** to slowly increase. more power will ramp in slowly to keep you at your new target speed.

For this to work I expect they have the **P** value low in this mode. They then also reduce the target speed gradually over time.
```

---
## \#101 Posted by: Jc06505n Posted at: 2018-06-19T22:11:20.923Z Reads: 117

```
Maybe I’m just dumb, but which bullet point is account for that it only holds that Speed for a certain time interval and then it decreases gradually unless a force is applied (in gurssing the Inequality equation)?
```

---
## \#102 Posted by: Cobber Posted at: 2018-06-20T00:03:49.135Z Reads: 119

```
https://youtu.be/AWWLP7TwsDU?t=129

watch from 2:09 

> _speed is slowly decreased at a rate of 30 rotations per second_

> _25kmh max, takes about a minute for the motor assist to stop_
```

---
## \#103 Posted by: mikenyc Posted at: 2018-06-20T01:31:10.177Z Reads: 114

```
It doesn’t add or increase acceleration, it just holds the speed that the wheels get spun up to. There’s no remote input, so if the wheels start spinning faster it tries to keep that speed and will decelerate gradually once it reaches its peak speed.
```

---
## \#104 Posted by: mikenyc Posted at: 2018-06-20T01:33:27.012Z Reads: 113

```
Thanks. This is a great summary.
```

---
## \#105 Posted by: Lionpuncher Posted at: 2018-06-20T03:58:50.389Z Reads: 115

```
 You ended up with the durban enclosure, looks good! Had to choose between that and the coupe for my mini build, chose the latter. Look? s like either was a good choice! 
K, back on topic; @Ackmaniac how much work would it be to alter your cruise control feature to be more like that? Would make a near perfect software absolutely sublime.
```

---
## \#106 Posted by: b264 Posted at: 2018-06-20T04:16:17.813Z Reads: 116

```
[quote="mikenyc, post:35, topic:59201"]
wouldn’t it be a better idea to up the $ donations to @Ackmaniac and ask him to do it?
[/quote]

No -- by far most of the code is written by Benjamin and the Ackmaniac parts aren't as high quality and very, very tiny tweaks by comparison.  I review code as my day job...
```

---
## \#107 Posted by: Wajdi Posted at: 2018-06-20T06:22:13.043Z Reads: 116

```
![Longboard_2018-Jun-20_05-40-36AM-000_CustomizedView9780571581|690x480](upload://jIZsKVLIADMwczp4lKzJSsyGjsB.jpg)

Endless mode is a really cool idea, especially for those that need a stealth ride with smaller batteries and less power consumption. This is what I have so far after gathering information bits from everywhere.

* "Assist." Controls how long the power assist will last in seconds. Default to 30 sec.
* "Threshold" Controls the activation threshold, after pushing and reaching this speed, power assist will kick in.
* "Deceleration" This controls the rate at which the deceleration decay happens. For example at 30 rotations per seconds as the mellow boards have it implemented.
```

---
## \#108 Posted by: Ackmaniac Posted at: 2018-06-20T06:29:12.241Z Reads: 114

```
Thx for making that clear.

Edit: Did you modify your comment. If i remember right it was a bit more spicy.

Anyway, maybe you should then implement a version of the endless mode.
```

---
## \#109 Posted by: mikenyc Posted at: 2018-06-20T16:36:28.496Z Reads: 108

```
He doesn’t care for it. He’s one half of the troll tag team. Ignore him. 

Edit: flagged. Nice!
```

---
## \#110 Posted by: Jc06505n Posted at: 2018-06-20T16:43:46.850Z Reads: 108

```
Just a reminder, Please **don't forget to vote for a feature your interested in via the first post.** If you have features that you see in industrial boards or in general that you would like implemented to the VESC say them and i'll add them to the poll. 

As of right now it seems Endless Mode/Push Assist is popular. If implemented we of course cant name it endless mode. 

@Wajdi Nice! Loving it man, a couple of questions:

1. How far along are you? Do you need assistance? 
2. Whats the release dates on these things? 
3. Estimated Pricing? 
4. Would Push Assist (referring to it to avoid any trademark or copyright infractions) be a release date feature?
```

---
## \#111 Posted by: brenternet Posted at: 2018-06-20T18:41:45.677Z Reads: 104

```
Please add remote development to the vote, even though its a bit late now I'm sure many people feel the current, mostly complicated and unreliable options are weak.
```

---
## \#112 Posted by: Jc06505n Posted at: 2018-06-20T18:46:29.607Z Reads: 106

```
Note this is for features. I can add it but I need a specific feature(s) in regards to remotes (such as connectivity, throttle, hardware, wireless programming, stronger Shells, etc)

Edit: I only ask such because we already have various remotes being developed i.e firefly remotes, firefly derivatives, and Proton remotes.
```

---
## \#113 Posted by: b264 Posted at: 2018-06-20T18:47:58.222Z Reads: 106

```
*Remoteless push assist mode* would be awesome but I've been stuck trying to figure out how to prevent overriding a footbrake with the motors...  Was thinking a tilt sensor but the extreme vibrations make that problematic
```

---
## \#114 Posted by: Jc06505n Posted at: 2018-06-20T18:49:52.981Z Reads: 105

```
[quote="b264, post:113, topic:59201"]
prevent overriding a footbrake with the motors
[/quote]

Can you elaborate here i'm confused. 

Edit: You mean how to make foot braking work instead of having the remote do the breaking?
```

---
## \#115 Posted by: b264 Posted at: 2018-06-20T18:52:14.129Z Reads: 100

```
Yep &nbsp;&nbsp;

The board would need to sense the difference between going up a hill and decelerating -- versus decelerating because a foot is dragging -- and override one but not the other

Also dragging a foot going uphill.  These are real issues and why the only ones implemented use a remote for braking
```

---
## \#116 Posted by: brenternet Posted at: 2018-06-20T19:23:19.897Z Reads: 98

```
The more I think about endless ride the more appealing it gets for a shorter commuter board with a small battery, it'd be light, portable, inexpensive to build and fun to ride while serving a real purpose for people who want it.
```

---
## \#117 Posted by: mikenyc Posted at: 2018-06-20T19:25:51.545Z Reads: 99

```
Yeah this wouldn’t be great on a board with a huge (heavy) battery.
```

---
## \#118 Posted by: CHAINMAILLEKID Posted at: 2018-06-20T20:00:52.752Z Reads: 102

```
I think I've got it figured out.
Two separate pressure sensors / strain gauges in the deck under the grip on the front and back halves of the deck. One for each foot.

One foot on, one foot off would mean its ready to set a new top speed.

Two feet on means its ready to maintain speed.

Two feet off means come to a stop.

Whats crazy is... I think you might be able to do all that with an analog circuit and discrete components.
```

---
## \#119 Posted by: Jc06505n Posted at: 2018-06-20T20:08:18.976Z Reads: 101

```
[quote="CHAINMAILLEKID, post:118, topic:59201"]
Two separate pressure sensors / strain gauges in the deck under the grip on the front and back halves of the deck. One for each foot.
[/quote]


Sounds like Z-board / Starkboard

[quote="CHAINMAILLEKID, post:118, topic:59201"]
One foot on, one foot off would mean its ready to set a new top speed.

Two feet on means its ready to maintain speed.

Two feet off means come to a stop.
[/quote]

So when your just hoping on the board, how do you keep it from moving initially? Footbraking maybe?

Keep in mind many of us ride in the street and you just can't hop off in the middle of the street if a car stops or a pedestrian decides they're the captain now. 

And what about stopping on a hill?

Pressure boards just aren't very applicable in terms of the needed precision of user input.
```

---
## \#120 Posted by: CHAINMAILLEKID Posted at: 2018-06-20T22:47:30.858Z Reads: 105

```
[quote="Jc06505n, post:119, topic:59201"]
Sounds like Z-board / Starkboard
[/quote]

It'd be different. 
Those are like lean to accelerate boards, this is much more simple than that.

[quote="Jc06505n, post:119, topic:59201"]
So when your just hoping on the board, how do you keep it from moving initially? Footbraking maybe?
[/quote]

It won't move until you push it. It doesn't ever accelerate under power.

The sensors aren't for throttle, they'd be more or less just switches that select different modes.
There'd be an AND gate, an OR gate, and a NOT gate.

If you have one foot on the board, the assumption is you're either foot-braking or pushing, so that just lets the wheels freely spin so you can adjust the speed, slowing it down, or speeding it up.

Once you've pushed to the speed you want to go, you put your other foot back on the board, Then it enters push assist mode where it maintains the current speed more or less. This mode would also keep you from speeding up so you can descend hills without going faster than you want to.

And then if neither of your feet are on your board it means you've jumped off, or fallen off, or something like that. So the board responds by easing on a brake. It wouldn't need to be a strong brake because it would only need to be designed to stop the weight of the board w/o a rider.
```

---
## \#121 Posted by: skatardude10 Posted at: 2018-06-20T22:56:29.087Z Reads: 103

```
My board is heavy, I think it'd be nice to allow a 1 amp, or maybe even 0.5A or less, so once the board detects movement up to maybe 10 miles per hour it would very lightly and controllably assist in pushing a heavy board, but at the same time won't take off past a certain point. Maybe that 0.5 - 1A assist could gradually decrease to 0 A over a predefined and customizable speed range, and that push boost amount could be customized to be however high or low you would like (within reason).

So for example, you could set a 0.1A or maybe 5watt boost for 0-5 mph that drops smoothly to 0 at 15 mph if that's how fast you push.

I tried out PID no acceleration today, and while pushing up to speed was rough, the experience was phenomenal. I will be using this mode a lot more for chill rides from now on... Now if (as above), the board would boost that small (maybe even 1 watt) amount to make my board just feel lighter and slowly decelerate, that would be even better 😎... Then whip my phone out, select 2000W when I'm ready to blast up a hill... 😃🤣😀😋😍

You could prevent the board from just taking off on it's own (say accelerating down a hill cause it thinks your pushing and giving that small boost up to your predefined speed) by requiring the rider to hold full throttle for the small boost, coast or push with no power but still doing the coast and decrease in RPMs/time with throttle at neutral and brake when braking.
```

---
## \#122 Posted by: b264 Posted at: 2018-06-20T23:34:52.931Z Reads: 99

```
[quote="CHAINMAILLEKID, post:118, topic:59201"]
One foot on, one foot off would mean its ready to set a new top speed.

Two feet on means its ready to maintain speed.

Two feet off means come to a stop.
[/quote]

This is a great idea.
```

---
## \#123 Posted by: mikenyc Posted at: 2018-06-20T23:41:42.375Z Reads: 99

```
[quote="b264, post:106, topic:59201"]
the Ackmaniac parts aren’t as high quality and very, very tiny tweaks by comparison. I review code as my day job…
[/quote]

Since you're so critical of @Ackmaniac, do you plan on writing it yourself?
```

---
## \#124 Posted by: kylem21 Posted at: 2018-06-20T23:44:44.092Z Reads: 93

```
What makes you say that? I feel like the feature would still be useful in the sense you’re saving a ton of battery and it just sounds hella fun to pump and coast forever
```

---
## \#125 Posted by: mikenyc Posted at: 2018-06-20T23:46:20.117Z Reads: 93

```
Ah, so I just competed a build a 4wd carvon build with a 12s5p pack. It is heavy. Like, really heavy. I had to kick push it a few blocks to get somewhere because my board had some issues. It wasn't fun lol.
```

---
## \#126 Posted by: kylem21 Posted at: 2018-06-20T23:54:56.393Z Reads: 90

```
Yeah that makes sense I didn’t really think of the hassle of pushing a really heavy board. I was thinking of a 2wd 12s4p carvon build on a subsonic talon 37 with a foam core to reduce the weight. Do you think that would be too heavy to pump up to 10mph without struggling too much?
```

---
## \#127 Posted by: mikenyc Posted at: 2018-06-21T00:00:22.283Z Reads: 91

```
It’s the first few pushes that are difficult. Braking with the motor should be fine though.
```

---
## \#128 Posted by: pixelsilva Posted at: 2018-06-21T00:51:52.165Z Reads: 90

```
> @Jc06505n
> 
> After all, how many of us have a BT Mod in our boards? A Friefly? Lights? Go Pros Attachments? Photon Remotes? None of the above is needed yet were all ready to throw money at them! All i’m saying is , The criticism on implementing “non-needed features” when we buy un-needed things on a daily basis. If you don’t want it and it’s not for you , keep it stepping, but don’t be arguing against the advancement of ESK8’s 

....right; like the X-Things, Idlers, XT connectors, 107 uro wheels, carry on handles, LED lights, etc., etc.
```

---
## \#129 Posted by: Jc06505n Posted at: 2018-06-21T00:54:50.442Z Reads: 93

```
[quote="CHAINMAILLEKID, post:120, topic:59201"]
It won’t move until you push it. It doesn’t ever accelerate under power.

The sensors aren’t for throttle, they’d be more or less just switches that select different modes.
There’d be an AND gate, an OR gate, and a NOT gate.
[/quote]

I like it, no... love it. a true push assist board. My only issue is when going downhill. Physics majors , correct me if I’m wrong on this, but if your going downhill even if the motor and stop supplying power , the wheels are still going at that speed , and if steep enough accelerating fast. Because of the power supplied by the motors before hand, you’re maybe going at a speed far faster than you would if you had originally gone down with a regular Board. 

Maybe instead of allowing freeroll, the motors work to slowly , very slowly decelerate based on the curve of the speed you’re going rather than freewheel ? The deceleration would be miniscule enough to be overpowered by the kickpush, but enough to assist in footbraking?
```

---
## \#130 Posted by: skatardude10 Posted at: 2018-06-21T01:01:20.527Z Reads: 97

```
One thing I don't really like about PID no acceleration is the lack of free rolling. 

Like in [my post above,](http://www.electric-skateboard.builders/t/leisure-industry-features-that-we-could-implement/59201/121?u=skatardude10) you could set a max speed for assist, ideally have it push you hardest at lower speeds and taper off to 0 assist at a defined higher speed, so that small assist doesn't send you flying if accelerating down a hill, it will only help until a certain set speed. This way you can freewheel while going faster, like bombing a hill if you like, but still have brakes available. 

With PID no acceleration, it seems to just hold the speed you choose, braking for you going downhill and speeding you up going uphill. I'd love a board that just helps you push a bit by applying some small wattage when accelerating while tapering off that small wattage to zero as speed increases, maintains speed to a certain point, tapers off the speed over time if not accelerating (such as uphill or flats as opposed to rolling downhill), and otherwise freewheels at higher speeds.
```

---
## \#131 Posted by: CHAINMAILLEKID Posted at: 2018-06-21T03:59:16.879Z Reads: 96

```
This might just be a stepper motor thing, but I believe you can set it up so that the motor resists any difference in speed both faster and slower.

If not natively I'm sure there's a way to do it in software.
```

---
## \#132 Posted by: Ackmaniac Posted at: 2018-06-21T06:28:28.009Z Reads: 94

```
If you want that the board doesn't brake when you become faster then you should disable braking for speed control in the PID settings.
This way it will freewheel when you become faster.
```

---
## \#133 Posted by: mikenyc Posted at: 2018-06-21T06:35:17.957Z Reads: 92

```
That sounds nice on paper, but many will argue that they prefer the feeling of free rolling.
```

---
## \#134 Posted by: b264 Posted at: 2018-06-21T09:16:07.265Z Reads: 92

```
[quote="mikenyc, post:123, topic:59201"]
Since you’re so critical of @Ackmaniac, do you plan on writing it yourself?
[/quote]

Sure... but if you're going to pay to expedite it, Benjamin will make it better then I or others will, so you should have him do it instead of me or Ackmaniac.  Why don't you just do it?
```

---
## \#135 Posted by: koralle Posted at: 2018-06-21T10:05:08.294Z Reads: 92

```
I wish this wasn't all vedder vs ackmaniac but vedder with ackmaniac.

The problem with vedder is that he is always very busy and sits in his ivory tower aka vesc-project forum. Over there all the talk is so high-tech that most of us do not feel comfortable.

I love that Ackmaniac hangs out with us and his can-do attitude. The problem is that he could not act so fast and would not get donations if he were working on the official repository together with vedder. This is a pretty lame predicament.
```

---
## \#136 Posted by: tsr Posted at: 2018-06-21T10:13:23.490Z Reads: 92

```
One feature that might be added to the list - braking when battery is fully charged, like discussed in here:
https://www.youtube.com/watch?v=3ZKXtsFEW40

Would be a nice safety feature I think - but i am a esk8 noob, what do you think?
```

---
## \#137 Posted by: koralle Posted at: 2018-06-21T10:19:01.080Z Reads: 90

```
It would be so dope if the vesc had a connection for a silicone heating mat that we can put underneath the griptape as a brake chopper like some mainstream boards have

Not only if the battery is full but also if you go down a hill that is steeper than what your battery should safely charge.
```

---
## \#138 Posted by: b264 Posted at: 2018-06-21T10:22:42.602Z Reads: 90

```
This dump load would need to come from the BMS not the ESC
```

---
## \#139 Posted by: lock Posted at: 2018-06-21T10:24:14.053Z Reads: 91

```
Yeah it'd mean our maximum braking capability would no longer be dependent on what our batteries can handle. Lately I've been thinking about something a little less subtle, like dumping the power to some exposed nichrome wires under the board.

This is basically what I want to see at night :joy: 
https://www.flickr.com/photos/lucidblinks/10465798004/
```

---
## \#140 Posted by: Ackmaniac Posted at: 2018-06-21T10:24:41.018Z Reads: 89

```
They need this because their battery is tiny (100Wh 10S1P if i am right). With a decent battery like 10S4P you don't need that. That is also the reason their brakes won't work anymore at high speeds because the battery current will be too high. Of course they could still allow braking and risk to stress your battery but then they might have too many warranty issues.

In theory with a proper battery you could still have that issue when you charge the battery completely full and roll down a long hill directly from the start. But even then the effect is little with a proper sized battery.
And most chargers (not all) will only charge a 10S battery to somewhere like 41.6V. So there is enough wiggle room.

They just simply needed to find solutions for the undersized battery.
```

---
## \#141 Posted by: tsr Posted at: 2018-06-21T10:28:26.520Z Reads: 90

```
I think I understand - but my impression on this forum is that there are at least some people that also don't have a "decent" battery.... 

I am starting my first build with a 10s2p and am living in a hill area - so i am already curious how this will work out ;)
```

---
## \#142 Posted by: Ackmaniac Posted at: 2018-06-21T10:33:39.603Z Reads: 91

```
If you are a heavy guy and your gearing is high it won't work well. I would recommend 10S3P as a minimum for a weight of like 75kg. Biggest issue are the brakes with small batteries.
With Lipos it is another story of course.
```

---
## \#143 Posted by: tsr Posted at: 2018-06-21T10:51:00.899Z Reads: 91

```
I am 85kg and planning to start with a 15:40 gearing... So we will see - but i don't want to continue here because I don't want to "hijack" this thread^^ But your comments are really appreciated!
```

---
## \#144 Posted by: Slak Posted at: 2018-06-21T11:00:16.992Z Reads: 94

```
There are threads on this forum about this :

https://www.electric-skateboard.builders/t/diy-break-chopper-protection-against-overvoltage-no-cutoff/49823

https://www.electric-skateboard.builders/t/charge-capacitors-instead-of-brake-chopper/52471
```

---
## \#145 Posted by: bevilacqua Posted at: 2018-06-21T11:01:51.193Z Reads: 85

```
7s2p I think. They might be even using some LiFePos....

Edit: they use lion 18650
```

---
## \#146 Posted by: mikenyc Posted at: 2018-06-21T11:02:55.482Z Reads: 88

```
It’s 7s2p. That’s why it’s weak lol

Edit: @bevilacqua beat me by a minute!
```

---
## \#147 Posted by: bevilacqua Posted at: 2018-06-21T11:08:00.694Z Reads: 87

```
quite some sacrifice to put sub 2Ah cells on the Pack.... But well they can take it on a plane. 

Nevertheless I think that even for 3p packs it would be cool to have a BMS with an integrated brake chopper or a sandalone module that sits in between the ESC and the BMS.
```

---
## \#148 Posted by: Ackmaniac Posted at: 2018-06-21T11:08:58.945Z Reads: 91

```
Think it is even worse.

Seems they have 8S1P Panasonic 3500ma 10A discharge cells. And then 350€ for a additional battery pack that has 8 cells which are worth 40€.
```

---
## \#149 Posted by: bevilacqua Posted at: 2018-06-21T11:13:53.967Z Reads: 93

```
![56|551x500](upload://cY94Gwqq2tCLdiDLG0rRqipD0hG.png)

They guys behind it are not dumb. 8s1p on 10A cells would have been a really bad idea. 
Even if most don't agree. Their drive system is very well thought through
```

---
## \#150 Posted by: Ackmaniac Posted at: 2018-06-21T11:27:04.038Z Reads: 91

```
On their website they say the battery has 29.2V. In this case they advertised the 7S battery with fully charged voltage. Means a 10S battery would be advertised by them as a 42V battery.

And to reach the 100 Wh with a 7S2P battery (you convinced me by the picture) they seem to have then 1750ma.
Or they use Samsung 25R and label the battery pack with less Wh then it really has.

So i think it won't take long that they come up with another battery pack that uses 3000ma cells and melk the costumers wallet a bit more.

I am not saying these guys are stupid.
The drive is well thought through. But the manufacturing costs, marketing and margin are also very well thought through.
```

---
## \#151 Posted by: bevilacqua Posted at: 2018-06-21T11:45:18.134Z Reads: 95

```
99/(3,6x2x7)=1,964
Taking into account that the capacity correlates to the discharge rate a 2Ah cell can be really a 1,9Ah cell (weighted at for example 10A cont discharge)...
Nkon example: 


https://www.dropbox.com/s/qj8yjm0wa6nhhvz/Screenshot%202018-06-21%2013.40.50.png?dl=

https://www.dropbox.com/s/xf7jvnfu85r0bgg/Screenshot%202018-06-21%2013.42.59.png?dl=0

https://www.mellowboards.com/out/pictures/zmbwysiwygeditor/General%20Uploads/FACTSHEET%20MELLOW%20BOARDS%202018%20ger.pdf
```

---
## \#152 Posted by: Ackmaniac Posted at: 2018-06-21T11:56:21.198Z Reads: 92

```
Your right. 1750ma were for 8S which i thought first.
```

---
## \#153 Posted by: mikenyc Posted at: 2018-06-21T12:04:17.105Z Reads: 93

```
For those that are interested. Here is a picture of the braking resistor (at least what I think is the braking resistor) in the Mellow. 

![image|666x500](upload://qLLwuXFzuKOUXmYcVadA2C3715m.jpeg)

Inboard has something similar. The difference is theirs is glued to the bottom of the deck in the form of what looks like some flexible copper.
```

---
## \#154 Posted by: mikenyc Posted at: 2018-06-21T12:12:29.073Z Reads: 94

```
Yes and no. I had so many problems with their drive system. It was so complicated. Everything broke. The remote firmware got bricked. When it’s bricked, you can’t shut it off and do a hard reset. After a month, I charged the remote and it was discoverable again, ready to be reflashed OTA. A hard switch would have made this a non issue, as would a less complicated remote lol. (To their credit, they did send me a replacement remote over night, after almost a week of going thru the customer service process) it took a week to get to me because of customs. So 2 weeks down, no remote. A few weeks after I got the board running again, it broke once more. Water had gotten into the drive from wet pavement, and at the same time, the fuse on the charge input blew. Both had to be replaced. Took about 5 -6 weeks for that to come. A week after the replament baftery and drive came (new design for battery and drive to address reports of batteries falling out), my battery got stuck inside the drive and would not come out. Was confirmed that the battery would not come out by their US distributor that I sent the drive to for confirmation. 

I still think they are great guys, and they refunded me for my purchase. But I think they need to simplify things and figure out how to lower the cost of their system.
```

---
## \#155 Posted by: Jc06505n Posted at: 2018-06-21T12:27:06.343Z Reads: 95

```
So I should add a breaking Resistor (for small battery packs) to the list? The only one I can think of capable of doing so in a commercial matter is @Kug3lis. I would like to add him to the discussion if interested. 

It seems the first two features are in the hands of @Wajdi’s upcoming product. Please continue shooting ideas and concerns as they do help I the development process.   

I want to bring up the last two features that have garnered some votes. 

**Turn off Via Remote**

One of the features I love about the B.B. is that you can turn it off via the remote. All you would need to do is hold down the trigger (without the killswitch) while also holding down the power button on the remote. This turns off both the Board and remote. 

In order to have This feature you would need a “Smart Remote”/Telemetry Remote (Proton Remote, Firefly V1 Remote) that communicates with your board beyond just controls. 

1 implementation (using the Firefly) would require using Momentary Switches on both your Board and remote and mimic the way B.B. does it. 

Another implementation (using eithe the firefly or Proton) would be having the board still use a momentary switch, but having a Setting that allows you to set “Turn Off Board with remote”. 

As you can see Momentary Switches are important here one way or another. I believe @Kug3lis is coming out with a Mini Fatboy Antispark that utilizes momentary switches. Do you think this is plausible ? 

What do you guys think? 




(Reminder that this is in for the discussion *for* The feature *Turn Off Via Remote*. Please refrain from comments relating to *I don’t see the point* or * I don’t want his feature* as it does not advance nor contribute to the discussion in any way. If you have no interest in this feature. Don’t talk about it nor do not vote for it in the original post.)
```

---
## \#156 Posted by: mikenyc Posted at: 2018-06-21T12:46:27.951Z Reads: 90

```
Umm. Not him, but @JTAG for braking resistor.
```

---
## \#157 Posted by: Jc06505n Posted at: 2018-06-21T19:23:27.606Z Reads: 85

```
Ah I didn't notice his work, but from the looks of it, he would be the man.
```

---
## \#158 Posted by: Blitz Posted at: 2018-06-21T19:28:34.007Z Reads: 90

```
You do understand that "Push start!"
OR "remote power on" Just means the board is always on right?

I could just leave my loop key in and Use my magic remote to turn the board off and on
whooo 1 step faster than turning your remote on and pushing a board whoououoo



#
EDIT:
correct me if I'm wrong about the Push start= always on,
Maybe they have some epic power switch than turns on when wheels move but seems unlikely for a Chinese board.
```

---
## \#159 Posted by: squishy654 Posted at: 2018-06-21T19:36:37.570Z Reads: 90

```
[quote="Blitz, post:158, topic:59201"]
Maybe they have some epic power switch than turns on when wheels move but seems unlikely for a Chinese board.
[/quote]

Where do think this stupid marketing bullet point came from?? lol
```

---
## \#160 Posted by: Blitz Posted at: 2018-06-21T19:41:14.831Z Reads: 92

```
@squishy654 I don't get what ur saying :thinking:

#
#
#
#
#
Edit:
[quote="squishy654, post:159, topic:59201"]
Where do think this stupid marketing bullet point came from?? lol
[/quote]

I guess China to advertise boards right?
```

---
## \#161 Posted by: Jc06505n Posted at: 2018-06-21T19:49:09.727Z Reads: 96

```
[quote="Blitz, post:158, topic:59201"]
You do understand that “Push start!”
OR “remote power on” Just means the board is always on right?
[/quote]

I don't. My Hypothesis is that Pushing the wheels send a very small dose of power (or what ever happens when you push with a dead board) back to the ESC's The ESC's, whether its a constructor function somewhere or something hardware wise, turns on the system. But just my hypothesis based on my non-existent understanding of well everything. 

But if it is the case it should be easy to test by measuring the battery in incitements against a controlled variable (a esc without this feature). Charged them to the same capacity and if the battery with the Push to start feature averagely has less than the one without, then the board is truly always on.   

I've searched for any explanation from how they work but no one seems to. I have a Dead Meepo (not sure if the ESC is dead i don't think so), and two DIYEboard ESC (one doesn't not turn off no matter that is do) I'm willing to donate for anyone who wants to go wild and figure out how everything works. I'm offering the whole 10s5p kit in case anyone wants to test out the experiment in the paragraph before. 

[quote="Blitz, post:158, topic:59201"]
I could just leave my loop key in and Use my magic remote to turn the board off and on
whooo 1 step faster than turning your remote on and pushing a board whoououoo
[/quote]

The point isn't just taking out an extra step but also having that long board feel of just hopping on that board and **going** . An aspect that at least 8 people have showed interest in so far.
```

---
## \#162 Posted by: Blitz Posted at: 2018-06-21T20:00:43.104Z Reads: 91

```
[quote="Jc06505n, post:161, topic:59201"]
just hopping on that board and **going**
[/quote]

Your remote would have to always be on... OR
press the trigger to turn it on But.. that might go bad.
```

---
## \#163 Posted by: Jc06505n Posted at: 2018-06-21T20:04:58.472Z Reads: 89

```
Keep in regards that I'm only talking about Push to Start. Turn *on* via remote is not a listed feature. Only Turn *off* via remote is listed in the poll and I'm only referring to features listed via the poll. Speaking of, time to update it.

Edit: Question, if i add an option to the poll, will it reset the votes?
```

---
## \#164 Posted by: Vanarian Posted at: 2018-06-21T20:58:19.899Z Reads: 87

```
Yep I confirm, this is being worked on ! @Nordle  have some interesting layouts too !

Edit : I'm also looking to get a soft-latch single push/hold ON/OFF button module working plug n'play ! No more micro disconnections or random accidental shut-off!
```

---
## \#165 Posted by: Nordle Posted at: 2018-06-21T21:44:35.354Z Reads: 86

```
@Kug3lis sells exactly such switches
```

---
## \#166 Posted by: Vanarian Posted at: 2018-06-21T21:51:55.165Z Reads: 90

```
Is it up for sale yet ? & I think he has a combo anti-spark + button, and the FETs he uses are ginormous ! It looks solid but no way I can fit in in my build. I need something thinner deffinitely, even with an external heatsink on top of it.
```

---
## \#167 Posted by: Kug3lis Posted at: 2018-06-21T22:43:25.166Z Reads: 89

```
Soon will be mini version ;) Big version is several batches out already :)
```

---
## \#168 Posted by: Vanarian Posted at: 2018-06-21T23:46:11.702Z Reads: 89

```
Then I look forward to see the mini! That's good news!
```

---
## \#169 Posted by: Jc06505n Posted at: 2018-06-23T14:11:52.855Z Reads: 88

```
Had a chat with @PredatorBoards this morning in regards to How Push to start works in regards to DIYEBOARD esc’s He said:

> Uses back EMF to feed power to a gate and mosfet switch. Basically the same manner as a momentary switch completing the circuit for the mosfet switch.

So it doesn’t seem that Boards are always on^. 

In order for the VESC to implement such a feature here’s what he said: 

![image|422x500](upload://6Iexjz4KERpkfEE5EGJLNBYauyW.jpeg)

Any thoughts ? It seems a Momentary switch is kind of important. Hopefully something solved with @Kug3lis’s upcoming product. 

One last question: does anyone know if adding another option to an already existing poll will erase all the votes? I have a few from others that I need to add above but don’t want to erase the results.
```

---
## \#170 Posted by: Maxid Posted at: 2018-06-23T14:16:53.890Z Reads: 81

```
Regarding push to start you might want to read through this quite recent thread: http://www.electric-skateboard.builders/t/why-is-there-no-on-off-switch-integrated-in-a-vesc/55753
```

---
## \#171 Posted by: Jc06505n Posted at: 2018-06-23T14:46:56.163Z Reads: 87

```
Interesting read didn’t understand some parts but got a general just if it. So as VESC’s are now , (mainly the 4.12s derivatives) it would maybe require upgrades , but potential for the 6 and its derivatives?

It seems there isn’t a software only solution to Push to start, and looking at my DIYEBOARD kit, the esc is directly connected to the switch... 

So what’s needed, if I’m not wrong, is a VESC where the AS is connected directly to the VESC?
```

---
## \#172 Posted by: PredatorBoards Posted at: 2018-06-23T15:25:27.899Z Reads: 86

```
To add to the push-start. It’d be easier if we had a MOSFET switch that respond to and differentiate between high and low signals. When it receives a high signal (should be pretty easily to implement on the VESC), it closes the loop. CANbus wouldn’t me necessary in this case.
```

---
## \#173 Posted by: Saturn_Corp Posted at: 2018-06-23T23:13:45.988Z Reads: 83

```
I use push to start on my board. When I swapped my hardware over to a new deck and enclosure I only included the charging port. Push to start is necessary for me and so much more convenient. I don't know how much battery it uses idle before it turns off though so that could be a concern.
```

---
## \#174 Posted by: Jc06505n Posted at: 2018-06-25T18:36:26.882Z Reads: 80

```
[quote="Saturn_Corp, post:173, topic:59201"]
I don’t know how much battery it uses idle before it turns off though so that could be a concern.
[/quote]

This reminds me of another feature for implementation: *Idle Turn Off*.

@moderators I can't edit the poll for some reason to add new options. it's telling me to ask you guys to do it. Would one of you mind adding these options in and changing the max to 9?:

* Braking Resistor (For Small/Tiny Battery Packs to dump power while going downhill)
* VESC Sleep Mode / Auto Shut Off (Meepo, Wowgo, etc.)
* ESK8 Leaderboards (OneWheel)
* Other (Say them in the thread with detail and they'll be added in, vague and undefined ideas will not)
```

---
## \#175 Posted by: Jc06505n Posted at: 2018-07-01T15:24:08.348Z Reads: 80

```
Nice looks like @JTAG [implemented the push to start feature on his BMS](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/332?u=jc06505n)
```

---
## \#176 Posted by: Kug3lis Posted at: 2018-07-04T13:00:24.575Z Reads: 78

```
Hi, guys just discovered this thread :D

I think I can implement a small module in between vesc and bluetooth module which would count lifetime statistics, and would provide output via same style protocol as vesc does but it would need existing apps to support it or etc if anyone is interested in that kind of thing.

Also I am going to add push to start to FatBoy Mini Sparky Switch
```

---
## \#177 Posted by: TarzanHBK Posted at: 2018-07-04T14:50:05.931Z Reads: 77

```
I think @Ackmaniac and @rpasichnyk could implement that. But should it also be possible to safe the data each time and add it in the app to a lifetime count?
```

---
## \#178 Posted by: Jc06505n Posted at: 2018-07-04T15:34:53.831Z Reads: 75

```
It’s not applicable software wise because the VESC has a ERPROM limit if 100,000 writes , it’ll get filled after 10,000 KM if you write It every 10 meters (my math can be off @Ackmaniac can explain IT better  : 

> [quote="Ackmaniac, post:1404, topic:12286, full:true"]
The issue is that the EEPROM storage of the VESC only has a limited amount of writes (roughly 100000). So it would be possible to track it there but if you save for example every 10 meters then the VESC’s storage might fail after 1000 km because you reached 100000 write cycles. Next problem is that the EEPROm storage can fail or is very likely to fail when you save the data while the VESC get’s disconnected from the battery. Then all the data could be lost.
So in theory it is possible but it also has some risks.
[/quote]

I for one will probably use @Kug3lis device and @Wajdi for double redundancy
```

---
## \#179 Posted by: snowriderau Posted at: 2019-08-26T01:59:49.887Z Reads: 29

```
[quote="Jc06505n, post:19, topic:59201"]
use
[/quote]

Ill take a Fatboy switch if it has push to start!, Thats awesome!
```

---
## \#180 Posted by: snowriderau Posted at: 2019-08-26T02:06:38.870Z Reads: 28

```
Wait, it already has this, need to get one on order.
```

---
