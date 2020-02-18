# How to control acceleration?

### Replies: 42 Views: 4577

## \#1 Posted by: mmaner Posted at: 2016-11-27T18:08:56.717Z Reads: 291

```
On a lot of the prr-built boards there is a "beginners" mode.  That is essential where when you activate the trigger/switch/button fully (meaning full throw/pull) the acceleration is gradual, I assume over a 20 to 30 second period.  Is this possible with a VESC or standard ESC like the FTV 120 or Mamba Monster 2?
```

---
## \#2 Posted by: Alextech Posted at: 2016-11-27T18:25:22.404Z Reads: 290

```
In most cases you can start by limiting motor amps. This will limit how many amps the motor can possibly pull creating a slower acceleration. You can also tweak the acceleration curve but I do not have much experience with that but plenty of users can help with that.
```

---
## \#3 Posted by: mmaner Posted at: 2016-11-27T19:11:17.502Z Reads: 281

```
I've played with the acceleration curve in the Mamba Monster 2 but I don't remember a AMP setting.  I'll go look and see.
```

---
## \#4 Posted by: Okami Posted at: 2016-11-27T19:15:28.105Z Reads: 275

```
There is this thing called ''throttle ramp control''.. It was mentioned in Arduino thread..

Though, one guy who made it,  has not shared a lot of info about it on the forum..

That is a bit disappointing, as I think it would be vastly useful for a lot of ppl..

---

In short.. It would allow to set how quickly acceleration is gained - increased, without interfering with the esc. You would connect this module after the receiver, right between receiver and esc..

The guy who had built it, had 3 or so modes for it already.. it involved some tinkering but Im sure someone could go ahead and make a simpler, kit module to sell / share.
```

---
## \#5 Posted by: Okami Posted at: 2016-11-27T20:36:52.374Z Reads: 250

```
see this:

http://www.instructables.com/id/The-New-and-Improved-Brushless-Electric-Scooter-Po/?ALLSTEPS

Search '' throttle ramping ''

---
Here's the post / thread where it is discussed:

http://www.electric-skateboard.builders/t/dorian-wiskow-emtb-build-trampa-holypro-17-e-toxx-belt-drive-twin-sk3-6374s-twin-max6-escs-6s-16-000mah-lipo/10859/13

--
If you are handy with arduino, perhaps you can make something up that regulates/ shapes the signal from the remote..
```

---
## \#6 Posted by: SimosMCmuffin Posted at: 2016-11-27T20:52:41.415Z Reads: 213

```
So you mean putting an additional module between the receiver and ESC, which only does ramping for the ppm control signal?

Pretty easy thing to make, but to give the user some kind of control what kind of ramping aggressiveness they want is really the bothersome part. And then you want to give both acceleration and deceleration their own ramps.
```

---
## \#7 Posted by: Okami Posted at: 2016-11-27T21:07:06.890Z Reads: 192

```
Yep, it is for ppm signal. 

Author of the module also mentioned that it is a bit hard to dial in the correct settings and that some interface should be made.

I think @EssEnn was also asking questions and asked if it was possible to adjust the timing/ramps with a simple potentiometer. Though, it seems it never made out to a more productive discussion but I do hope this topic does surface once more.. since there are still a lot of esc's which are not very ''user friendly'' or also.. you need to adjust speed/acc modes on the go (to give it other ppl) - not depending on what esc you use :)
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2016-11-27T21:13:33.347Z Reads: 187

```
Not quite sure, but I remembered seeing something like this at hobbyking:

https://hobbyking.com/en_us/turnigy-3-channel-servo-speed-direction-regulator.html

Not sure if it would work the same, but for off the shelf  product.
```

---
## \#9 Posted by: Okami Posted at: 2016-11-27T21:15:09.571Z Reads: 188

```
Cool! Did not know such thing was available!

Is there anyone who would be willing to try this out?

 Including @mmaner ..

---

Here's what it does:

> One potentiometer sets the down transition time for all outputs another sets the up time & the third can reverse one output, to cater for physically mirrored servos.

https://hobbyking.com/en_us/turnigy-3-channel-servo-speed-direction-regulator.html

But more info on the topic and is this somewhat useful for us.. would be great
```

---
## \#10 Posted by: EssEnn Posted at: 2016-11-27T23:48:34.443Z Reads: 175

```
I just bought one and should be with my in 3-4 days time. I'll give it a test and see how it works. 

I have had to put my Arduino project to one side, way too much going on at work right now that needs my attention. I'll pick it back up when things have calmed down in the new year.
```

---
## \#11 Posted by: mmaner Posted at: 2016-11-28T02:46:01.692Z Reads: 167

```
I appreciate all the input. @EssEnn let me know how it goea, I'd really like to implement this for my kid.  I'll post if I find anything else.
```

---
## \#12 Posted by: saul Posted at: 2016-11-28T09:09:27.469Z Reads: 167

```
[quote="Okami, post:5, topic:13769"]
If you are handy with arduino, perhaps you can make something up that regulates/ shapes the signal from the remote..
[/quote]

this keeps coming up recently.
I have arduinos, servos right in front of me....lets see how far i get before i get distracted...
```

---
## \#13 Posted by: Luke Posted at: 2016-11-28T10:14:53.321Z Reads: 155

```
If we're looking for the simplest option for a beginner mode the benchwheel remote has a 50% max throttle function which works quite well with beginners
```

---
## \#14 Posted by: onloop Posted at: 2016-11-28T12:22:06.362Z Reads: 149

```
Also. There is a new BLDC tool that offers throttle curve control. It can achieve a similar result.
```

---
## \#15 Posted by: mmaner Posted at: 2016-11-28T13:43:22.695Z Reads: 161

```
@saul Im looking forward to what you come up with. 
@Luke I have been trying to get a benchwell remote, they are currently out of stock.  I'll try that when I can get one.
@onloop I assume that is a VESC tool?  Would you mind linking to the info?
```

---
## \#16 Posted by: DeathCookies Posted at: 2016-11-28T13:55:23.902Z Reads: 165

```
[quote="mmaner, post:15, topic:13769"]
I assume that is a VESC tool?  Would you mind linking to the info?
[/quote]

This thread here:
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286
```

---
## \#17 Posted by: mmaner Posted at: 2016-11-28T22:05:02.260Z Reads: 154

```
Here's one available in the US, and what Ill prolly get depending on the results @EssEnn gets. 

https://www.amazon.com/dp/B00P4VIG74/ref=wl_it_dp_o_pC_S_ttl?_encoding=UTF8&colid=6CC4IY62S5BU&coliid=I34T9KX94M3CIV
```

---
## \#18 Posted by: EssEnn Posted at: 2016-11-28T23:02:32.708Z Reads: 144

```
I got the email this afternoon saying it had shipped so it should be with me tomorrow with any luck otherwise Wednesday. ,
```

---
## \#19 Posted by: im-done Posted at: 2016-11-28T23:02:56.722Z Reads: 140

```
the way i did what you are speaking of is i set my max amps to 40 and my motor is rated for 60 amp max pull. this gives a slow acceleration to help new riders. im using a sk3 5055
```

---
## \#20 Posted by: Okami Posted at: 2016-11-28T23:05:30.166Z Reads: 140

```
Has anyone invented a way to adjust the parameters using an app or so? Im not very knowing about the vesc.. but just wanted to make sure is it possible or not..
```

---
## \#21 Posted by: mmaner Posted at: 2016-11-28T23:07:58.121Z Reads: 139

```
@im-done I dont think I can do that with the Castle Mamba Monster 2.  Settings below...
<img src="/uploads/db1493/original/3X/e/5/e501d50c6db231db53ec2c410f50135e98205754.png" width="446" height="500">
```

---
## \#22 Posted by: im-done Posted at: 2016-11-28T23:10:40.482Z Reads: 128

```
yes now that i think about it you should be able to with the throttle curve! thanks never even thought about the curves.
```

---
## \#23 Posted by: mmaner Posted at: 2016-11-28T23:12:15.498Z Reads: 126

```
Ive got it adjusted as well as I can but when you hit the throttle full the board still rockets forward.  The acceleration curve is great for control of the speed but not so much for the actual ramp up.
```

---
## \#24 Posted by: im-done Posted at: 2016-11-28T23:14:40.700Z Reads: 123

```
that makes sense kinda because its just musher in the center of the range than drops off. i used that on my radio to help me start the bard and not die, but i know amp draw settings on the vesc will work for what you are doing.
```

---
## \#25 Posted by: mmaner Posted at: 2016-11-28T23:18:10.053Z Reads: 119

```
@im-done That's cool, I'm going to go with a VESC when I get my aluminum deck rebuilt, I just don't want to change the electronics too much until I know what issues Im going to have.  With the enclosure I printed I'm going to have some creative wiring getting everything connected inside 3x1.5 inches.
```

---
## \#26 Posted by: EssEnn Posted at: 2016-11-30T15:18:53.604Z Reads: 106

```
@Okami & @mmaner - The little gubbin just arrived and I will give it a little test tomorrow night!
```

---
## \#27 Posted by: mmaner Posted at: 2016-11-30T15:29:42.310Z Reads: 108

```
@EssEnn thank yousir, I am looking forward to hearing how it goes.  This could be the answer to getting my wife back on a board, therefore letting me skate more as well :slight_smile:
```

---
## \#28 Posted by: TarzanHBK Posted at: 2016-11-30T15:29:59.625Z Reads: 108

```
bring your punch control rate down. That adjusts your startup power.
```

---
## \#29 Posted by: mmaner Posted at: 2016-11-30T15:31:20.731Z Reads: 105

```
I have tried that, I started at 100% and decreases at 20% increments to 20%.  The only change I saw was the ability to start without kick off.  At 60% the board would still throw me, at 40% it wouldn't move without a kick.
```

---
## \#30 Posted by: TarzanHBK Posted at: 2016-11-30T15:33:56.770Z Reads: 102

```
ok funny behavior :D
what about the value above? max forward power?
```

---
## \#31 Posted by: mmaner Posted at: 2016-11-30T15:50:42.216Z Reads: 97

```
That doesn't effect the rate of acceleration, only the top out of acceleration.  Ive experimented with my ESC (Castle MM2) pretty extensively, I dont think there's a way to make it slow the throttle ramp up.  I'd love to be wrong, I just dont think its there :).
```

---
## \#32 Posted by: EssEnn Posted at: 2016-12-01T23:03:29.132Z Reads: 91

```
@Okami & @mmaner I got home from work late and the GF banned me from playing with my new toy in the house. I'm going to test it with a servo and see how it works once she gets to bed ;) I might hook up my Arduino as well so I can see the change in PWM signal. Reading into what I have seen and learnt I have a feeling the best to expect will be that it will dampen inputs more than anything as it ramps down as well as up and you can't control them separately.
```

---
## \#33 Posted by: ElectricCommuter Posted at: 2016-12-02T01:47:32.222Z Reads: 90

```
Hi guys I am having a weird problem and was wondering if you could help out I hooked up my torque board remote and the throttle is controlled with the wheel not the trigger any thoughts
```

---
## \#34 Posted by: mmaner Posted at: 2016-12-02T02:10:13.017Z Reads: 88

```
Put the tx/Rx lead on ch2
```

---
## \#35 Posted by: Okami Posted at: 2016-12-02T20:00:22.484Z Reads: 91

```
I think you Can contol both.. im not sure what was the third setting.. some said something about the reverse or something.. you can click reviews to get some more info but it was confusing as there were airplane people mostly discussing it..
```

---
## \#36 Posted by: Okami Posted at: 2016-12-06T20:48:59.708Z Reads: 83

```
Ok I assume It got stock.. though, dont forget to publish the results!
```

---
## \#37 Posted by: EssEnn Posted at: 2016-12-17T16:04:47.940Z Reads: 77

```
Sorry for going dark but work got very very busy. People leaving, new staff and holidays. 

I have had a little play with the device and you can't adjust the ramp up and down separately. Which is a shame but makes sense for what it is designed to do. It does add a bit of a buffer to the inputs which is good but not good when you need to break quickly. 

I'm going to have to look at the Arduino idea again when Christmas is over. I found out that a friends brother actually codes C++ and he said he would be happy to spend an evening with me to go over the project sometime in Jan with any luck.
```

---
## \#38 Posted by: mmaner Posted at: 2016-12-17T16:18:50.143Z Reads: 74

```
I got one too, haven't even hooked it up yet.  Have had battery pack issues.  I'll play with it next week when. My new Zippy come in.
```

---
## \#39 Posted by: saul Posted at: 2016-12-17T22:30:29.491Z Reads: 76

```
[quote="EssEnn, post:37, topic:13769"]
I'm going to have to look at the Arduino idea again when Christmas is over. I found out that a friends brother actually codes C++ and he said he would be happy to spend an evening with me to go over the project sometime in Jan with any luck.
[/quote]

I did some tests with Arduino and a servo. I was able to get a nice ramp up/down, but then I got carried away and messed it up. The good news is its very doable, top speed limiting, ramp up, ramp down, and even separate brake ramps. 
I'll try to clean up the code and post a demo later.
```

---
## \#40 Posted by: Ackmaniac Posted at: 2016-12-17T22:52:40.409Z Reads: 77

```
So what do you really want to achieve. It would be possible to implement rampings to the PPM Handling of the VESC. But do you want a very slow ramping or do you want a short ramping to prevent that the board kicks of if you pull the trigger fully by accident?
```

---
## \#41 Posted by: saul Posted at: 2016-12-18T01:36:30.679Z Reads: 69

```
I think its some of both. pretty sure your firmware mods did most of this But i haven't tried it out yet.
also looking for more general solutions that would work for any esc not just vesc.
```

---
## \#42 Posted by: EssEnn Posted at: 2016-12-18T03:49:25.135Z Reads: 67

```
@Ackmaniac Both and not just for the VESC but any ESC. Also an easy mode for beginners with a limit on max throttle. I want it to be tune-able so you can not only adjust the ramp speed but the ramp curve. I terrified to let anyone else ride my board because it is so easy to give it a little too much throttle and hurt yourself. 

@saul What ever code you have, please let me see it. I'm pretty good at CTRL C & V ;) and I might be able to get something working. I'm no coder at all but I'm good at solving problems.
```

---
