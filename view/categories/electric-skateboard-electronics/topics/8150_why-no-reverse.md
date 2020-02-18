# Why no reverse?

### Replies: 49 Views: 5094

## \#1 Posted by: t1m0007 Posted at: 2016-08-23T04:10:39.772Z Reads: 546

```
Serious question- Why doesnt anyone use the reverse function on the VESC? The only person I've seen use it over current control with brake is Vedder himself and that's in his video. Can anyone shine some light on this? I only ask because i have this vision of using the force to make the board return to me...... :joy:
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-08-23T04:17:32.794Z Reads: 544

```
Why do you need reverse?
```

---
## \#3 Posted by: Pantologist Posted at: 2016-08-23T04:18:29.475Z Reads: 543

```
Kinda pointless honestly... Going in reverse while on the board is not easy anyways.
```

---
## \#4 Posted by: t1m0007 Posted at: 2016-08-23T04:18:32.298Z Reads: 537

```
for the force, man.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-08-23T04:19:10.310Z Reads: 532

```
Hahahah 

Actually it's a valid reason lol
```

---
## \#6 Posted by: oriol360 Posted at: 2016-08-23T04:19:16.272Z Reads: 527

```
in my opinion, reverse Is only good for that one feature you just described... or showing off to people that you have an electric board.
I have never seriously used reverse on a board while riding it. And I do not want my board to try and start going in reverse when i just want to brake while moving at a low speed.
Brake only FTW.
Reverse is pretty gimmicky.
```

---
## \#7 Posted by: t1m0007 Posted at: 2016-08-23T04:19:44.132Z Reads: 520

```
meh- i can ride switch on my snowboard and skateboard pretty easily.  I understand the gut reaction "why?" but what I'm asking is why not? Is there depleted braking performance? Has anyone done it??
```

---
## \#8 Posted by: paul775 Posted at: 2016-08-23T04:20:31.614Z Reads: 510

```
I think @longhairedboy uses it on his board builds. Not sure if he does it on every one though
```

---
## \#9 Posted by: t1m0007 Posted at: 2016-08-23T04:21:46.582Z Reads: 497

```
I guess I should re-frame the question--- is there any detriment to performance in using it? more likely to blow the VESC? Too much return current? Shitty Braking? Too touchy? just curious here. I have nothing to do but ask questions at this point while im waiting on parts to arrive.
```

---
## \#10 Posted by: oriol360 Posted at: 2016-08-23T04:21:59.578Z Reads: 479

```
Nevermind what I just said! Reverse would be very useful when I finally learn to do 180 stand up slides on my board!
```

---
## \#11 Posted by: Titoxd10001 Posted at: 2016-08-23T04:34:31.529Z Reads: 467

```
There is no pause from brake to reverse on the vesc like a hobbywing ESC where you have to hit the brake twice to reverse so it's kind of dangerous on a vesc.
```

---
## \#12 Posted by: whitepony Posted at: 2016-08-23T04:47:41.083Z Reads: 456

```
its very convenient with no reverse when youre standing at a road and just dont want the board to coast forward -> full brake, done!

im using pure current control (with reverse) on my jet spud for 180S - its great for that, but a bit weird in urban traffic scenarios when you have to stand still somewhere. until those superlow rpms, reverse is just "current no reverse with braking" anyway, just under an erpm cutoff the motor actually goes into reverse with the vesc.

when you are just riding from A to B and carving, current no reverse with brakes is much better imo. and if you are used to that mode, its takes a while to get adjusted to pure current control, cause at least i am simply used to brake when you stand still ... and then a reverse board goes full throttle backwards. lead to a few awkward moments :joy:
```

---
## \#13 Posted by: Jinra Posted at: 2016-08-23T05:17:50.366Z Reads: 424

```
What @whitepony said. I tried reverse before, but quickly realized I never used it. It's easier to just full brake while waiting at a light and not worry about suddenly jolting backwards from the reverse kicking in. I don't think it'd be wise to get used to using reverse anyway as you may end up bracing the wrong way sometime..
```

---
## \#14 Posted by: Michaelinvegas Posted at: 2016-08-23T05:52:11.583Z Reads: 404

```
[quote="t1m0007, post:4, topic:8150, full:true"]
for the force, man.
[/quote]

That's all he needs to explain guys lol

Good enough for me
```

---
## \#15 Posted by: Titoxd10001 Posted at: 2016-08-23T05:55:51.982Z Reads: 381

```
Yeah when I had hobbywing it was fun to whistle at my board and say "come here boy" like if it was a dog
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2016-08-23T06:00:31.262Z Reads: 375

```
I do it.... I ain't gonna lie


Come here boy...come on lol
```

---
## \#17 Posted by: itsmikeholland Posted at: 2016-08-23T06:03:41.900Z Reads: 365

```
because if there's ever an issue where I need to suddenly get off the board, I can immediately stop the board from flying backwards or forwards when I fall.
```

---
## \#18 Posted by: Michaelinvegas Posted at: 2016-08-23T06:11:33.657Z Reads: 361

```
I have to admit...there has been a few times that I was that wasn't diligent and the board started to roll away from me ... 

I'm lazy
```

---
## \#19 Posted by: longhairedboy Posted at: 2016-08-23T12:50:04.449Z Reads: 344

```
regardless of how it works internally, behaviorally the brakes go into effect prior to reverse. While it doesn't behave exactly like a car ESC, it isn't going to peel out in reverse and throw you while you are still moving forward. It will slow you down first then try to move you backwards. How it behaves is dictated mostly by your regen and motor min settings and partially by some crap in those other panels i totally don't understand yet. 

i like having reverse. If i drop something and have to walk back to get it, i can just bring my board back to me. Also i like being able to switch stance and just go backwards when i can't turn around for whatever reason. 

And sometimes you just miss the water fountain by a few feet and just want to back up a little.
```

---
## \#21 Posted by: SimosMCmuffin Posted at: 2016-08-23T13:55:39.827Z Reads: 332

```
In my motor controller, I programmed reverse into it and then day later I removed it from the firmware, because I realized I wasn't going to use it ever. Sure it was fun testing it, pushing the board forward and then having it return back to you, but other than that I didn't feel the feature was needed.
```

---
## \#22 Posted by: barajabali Posted at: 2016-08-23T14:20:05.830Z Reads: 311

```
Another valid reason: 

I don't have reverse on my mountain board because I haven't set it on my esc's but I know it would be super helpful considering sometimes I get myself in a jam and need to hop to turn around since my feet are strapped in
```

---
## \#23 Posted by: Weberp7593 Posted at: 2016-08-24T21:09:18.786Z Reads: 273

```
do you have a link to a ESC like that?
(Double Brake for Reverse).
```

---
## \#24 Posted by: oneafrikan Posted at: 2016-08-24T21:12:09.272Z Reads: 268

```
there's a YouTube video of Vedder reversing... so think there is a reverse coming (edit: with VESC), if not already..?
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-24T21:12:58.768Z Reads: 268

```
The VESC already has reverse, some people, such as myself, just don't use it.
```

---
## \#26 Posted by: Titoxd10001 Posted at: 2016-08-24T21:20:44.048Z Reads: 267

```
Any hobbywing ESC should have double brake for reverse I personally used the xerun and quicrun which are limited to 6s but i think they have a 8s model now.
```

---
## \#27 Posted by: mason Posted at: 2016-08-24T21:58:08.416Z Reads: 258

```
with 180 slides being the only practical use I can thinkof, has anyone here actually DONE a slide with our huge, soft wheels? I find it impossible unless it has just rained. Even then it is extremely difficult.
```

---
## \#28 Posted by: Mrmoonlight Posted at: 2016-08-24T22:31:23.460Z Reads: 243

```
There's a couple hard turns I make that are a bit sandy/pebbly (is that even a word?) on my regular commute where I sometimes do a quick slide. I'm sure a much better skater could pull off a 180, but them 90mm Flywheels stick like glue. They don't let up so easily.
```

---
## \#29 Posted by: IceNine Posted at: 2016-08-24T22:43:44.194Z Reads: 241

```
I tried reverse when I was bench testing with a Nunchuck controller and there was a VERY disturbing issue.  When cruise control was pressed it only reversed when the board was stopped and cruise was released, which is as expected.  The serious problem was, if you were using direct throttle control it was able to reverse with a touch of the Z button even when at full speed.  Maybe it was just because there was almost no load on the bench but it seemed extremely dangerous and I like it when my teeth stay in my mouth.
```

---
## \#30 Posted by: laurnts Posted at: 2016-08-24T23:46:04.255Z Reads: 228

```
Vedder uses reverse for the test purpose, I doubt he ride with reverse. Most people dont use reverse because of a safety issue. Jittering or accidental reverse while going forward could cause two things. One you kissing aspath real hard, two you blow ur vesc.

However I think most people have no reverse so that it could coast when throttle is positioned in the middle. This becomes less important issue if you have a special remote that could offset the middle position of the throttle (special settings).
```

---
## \#31 Posted by: Jinra Posted at: 2016-08-25T00:06:42.823Z Reads: 225

```
You can still coast with throttle in the middle, but only with current control. Both Duty Cycle and PID brake at netural. I used current with reverse for a while, but didn't find myself using reverse much so I turned it off. Didn't really many problems with it.
```

---
## \#32 Posted by: elkick Posted at: 2016-08-27T12:12:54.146Z Reads: 217

```
I I'm using reverse quite often, especially on the eMTB. As you mentioned it, since your feet are strapped on the board it's easier to get yourself free again if you're stuck.

I also  enabled it on some street boards just for fun and to use the board with dual front wheel drive from time to time. And to annoy people. :slight_smile: 

It only works with the Nunchuk though.
```

---
## \#33 Posted by: Vishnu Posted at: 2017-08-01T22:52:45.308Z Reads: 156

```
I had a boosted board for about  a month and the reverse feature was really great as it give you confidence you can stop at any speed. 
Is it hard for boards to be setup this way?
```

---
## \#34 Posted by: Jinra Posted at: 2017-08-01T22:53:51.863Z Reads: 160

```
Why would a reverse-less board not give you confidence to stop at any speed? It's exactly the same thing.
```

---
## \#35 Posted by: Vishnu Posted at: 2017-08-01T23:16:13.378Z Reads: 153

```
The way the boosted board is it allows you to gradually put on brake power.
```

---
## \#36 Posted by: Jinra Posted at: 2017-08-01T23:16:56.181Z Reads: 151

```
The Vesc does as well
```

---
## \#37 Posted by: Vishnu Posted at: 2017-08-01T23:18:17.172Z Reads: 150

```
so is there a way to setup the vesc to go in reverse when putting on brakes ..?
```

---
## \#38 Posted by: Jinra Posted at: 2017-08-01T23:21:07.989Z Reads: 151

```
Well no ESC "goes in reverese to brake", included boosted board. The ESC brakes first and when eRPM is low enough it applies torque in the opposite direction. Until that point, the motors act as a generator rather than trying to push the motor the opposite way. 

To answer your question, you can have forward/reverse just like Boosted Board on the VESC.
```

---
## \#39 Posted by: Vishnu Posted at: 2017-08-01T23:49:20.271Z Reads: 146

```
Ok great thanks
How do we set this up on a vesc?
```

---
## \#40 Posted by: Jinra Posted at: 2017-08-01T23:54:18.975Z Reads: 150

```
Really easy, just use the "Current" control mode. Everything else in the Vesc can be configured normally.
```

---
## \#41 Posted by: chsknight Posted at: 2017-08-02T02:57:18.177Z Reads: 148

```
Because I like to hold down the brake :sweat_smile:
```

---
## \#42 Posted by: Titoxd10001 Posted at: 2017-08-02T04:17:06.443Z Reads: 147

```
If you want reverse you want to use ackmaniacs firmware. He added a feature that you have to double tap the brake to go in reverse and can only do so when you're basically stopped. Also you could limit negative erpm (-12k) plus uncheck box apply brake for max erpm. So reverse will be predictable and much slower than your forward top speed
```

---
## \#43 Posted by: Spikelittlejohn Posted at: 2018-02-20T04:34:22.149Z Reads: 119

```
My golf skate caddy has reverse and 4 speeds, 
Video of it here. https://youtu.be/BR6OEiCvqSk

It is special purpose, built like a tank, heavy,  the reverse is great on a golf course, get in a tight spot, back up, get free, ![20180218_223447|690x388](upload://vDYutotCvgOL5wuvlsvUqDPZB4J.jpg)42v 30ah
12 mph, 2 rounds of golf per charge.
Use at campground now mostly.
Speed limit there anyway!![20180216_184953|281x500](upload://5GnhPIKcgg414jQ6Hq5AEr8z31k.jpg)
150 of these in the battery.
```

---
## \#45 Posted by: b264 Posted at: 2018-02-20T04:44:47.694Z Reads: 117

```
Does it use VESC?
```

---
## \#46 Posted by: ZackoryCramer Posted at: 2018-02-20T04:47:53.130Z Reads: 118

```
I use just "current" mode on Vesc. When you break and come to a complete stop, you will go backwards. I almost one time got my board yanked under me because I broke and stopped too hard. :rofl:
```

---
## \#47 Posted by: Spikelittlejohn Posted at: 2018-02-20T13:19:29.988Z Reads: 100

```
I think so, but proprietary, I believe.
Look here, I am just starting in electric board repair.
Mine Out of warranty, LOL
https://youtu.be/JkJaYsB8vf4

It is programmable, the bms on the battery was too, but died, replaced with 80a 10s
```

---
## \#48 Posted by: PredatorBoards Posted at: 2018-02-20T21:12:25.318Z Reads: 89

```
I use reverse for my builds. Honestly it would be nice if there was trigger button I can hold down to engage current no reverse brake only mode. Basically so then I can hold the brakes when I'm on a hill.
```

---
## \#49 Posted by: Deckoz Posted at: 2018-02-20T21:24:56.784Z Reads: 88

```
[quote="longhairedboy, post:19, topic:8150"]
reverse and throw you while you are still moving forward
[/quote]

Depends on how hard the wheels are. Boosted with kegels has tossed me a couple times because I'm so light it breaks traction and just goes straight reverse... So just be warry of wheel duro  if you plan to use reverse, it can make for unpredictable slides...
```

---
## \#50 Posted by: ARetardedPillow Posted at: 2018-02-20T21:36:52.129Z Reads: 85

```
I wonder if there is a way to switch between reverse and normal throttle using the channel 3 button on the nano x
```

---
## \#51 Posted by: Spikelittlejohn Posted at: 2018-02-20T21:59:24.197Z Reads: 79

```
My controler, has a pistol grip, and a switch on top to change from off to foward and reverse.
Made for getting around a golf course safe, I thinj it can be turned up, investigating, LOL
```

---
