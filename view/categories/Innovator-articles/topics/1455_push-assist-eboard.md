# Push Assist eBoard?

### Replies: 25 Views: 4126

## \#1 Posted by: laurnts Posted at: 2016-02-19T11:06:28.594Z Reads: 219

```
Hi eBoarders. I've been wondering for a while if someone has already made a push assist electric longboard? I know this sound ridiculous but from my understanding that eBike (Pedelec) pedal assist bike are totally legal in EU, it might be possible to do just the same for an electric longboard. Not quite sure though how the mechanics / electronics suppose or would do when the board starts rolling (maybe push 1 - 2 seconds more) but it can be quite adjusted the same as an eBike I suppose.

My question now also if VESC can support this functionality? As we now push the board our self and get assisted, it should be way more efficient in terms of distance as well as no more pulsing / cogging on start.

Opinions / Suggestions of experts here are welcome!
```

---
## \#2 Posted by: Tarzan Posted at: 2016-02-19T11:12:12.592Z Reads: 218

```
I think it is problematic to divide between pushing and rolling down a hill.
From my point of view it is hard to realize but interesting!
```

---
## \#3 Posted by: longhairedboy Posted at: 2016-02-19T12:12:43.027Z Reads: 212

```
something like this may be better accomplished by a more passive system involving permanent magnet motors instead of electrical ones. it would involve a fair amount of linkage, but no batteries. There would also need to be some kind of braking mechanism to keep things from spinning when you're not actually on it, because mag motors basically act like perpetual motion machines which aren't supposed to exist, and yet here we are. I guess it depends on your timeframe for "perpetual." They'll spin for years until the fields weaken. But it would have to be oriented sideways, be as wide as the bottom of your deck, and not very thick. IT wouldn't take you up hill on its own but it would probably allow you to glide on flats for much longer than usual. It would likely be a bit noisy too because of the linkage. And you could totally take it on a plane because 0 watt hours. 

https://www.instagram.com/p/1kzluVhBvp/?taken-by=longhairedboy
```

---
## \#4 Posted by: laurnts Posted at: 2016-02-19T14:02:32.451Z Reads: 188

```
Well this is not actually an answer I was expecting :P but it's super cool. I love perpetual motion, been watching some but still application to it is so limited due to the law of energy. Since we require some force to push our self forward with longboard, there wouldn't be much energy to continue the motion.

But really I would like to see this feature on VESC. At the moment my current ESC could assist me pushing my board without holding the throttle by just configuring my remote to send ie: 1600 gauss (100 gauss more compared to stationary). I am thinking if its possible for VESC to track BEMF input to decide how much power it needs to supply back to the motor.

Ie: if you push hard, motor spins hard = VESC Detect = motor assist spins fast
if you push lightly, motor spins slow = VESC Detect = motor assist spins slow
Then you can have a remote that only have on / off (turn on assist / turn off assist) as it's hard for the electronics to decide wether you would like to stop or having hills to climb.
```

---
## \#5 Posted by: barajabali Posted at: 2016-02-19T14:29:49.244Z Reads: 180

```
if were ditching electronics then i would use a flywheel in some way.  Each wheel would have a lot of mass on the outer portion of it, centrifical force would aid the wheels in spinning longer with load.  The mass would have to be pretty significant though...and youd need some big wheels, maybe on an off road board with 6-8 inch wheels?

Not exactly 'assist' just thought itd be cool. I guess you could call it an iboard, if i stands for inertia
```

---
## \#6 Posted by: trbt555 Posted at: 2016-02-19T14:42:20.614Z Reads: 179

```
Hall sensors on the motor to detect the mechanical rpm, use that input as the setpoint for a PID rpm control loop ?
Push once, board will maintain the speed reached. Push twice, board will maintain that speed.
Just thinking out loud.
```

---
## \#7 Posted by: longhairedboy Posted at: 2016-02-19T14:50:46.074Z Reads: 175

```
I think you underestimate the force provided by modern neodymium magnets. The magnets currently used in electric skateboard motors are smallish compared to what could be used in a magnet motor and still fit under a board. 

This is a huge proof of concept, but it could potentially be scaled. 
http://youtu.be/epLOEaoPMFU


but your idea would totally work with some clever firmware programming of VESC and some sensored motors to go along with it. But it would be virtually indistinguishable from regular electric skateboards and would therefor sort of defeat the purpose of differentiation for legal purposes. 

I like the idea of flywheels also, but i'm not sure how you would initially store the energy.
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-02-19T14:56:06.157Z Reads: 162

```
@trbt555 i think you may have just stumbled on to a whole new idea of how to control these boards at lower "run out" speeds. I love this idea.  VESC would sense how fast you're going when you push, then simply maintain that. Then when you start dragging your foot or simply stomp down to stop, it would need to sense that very very quickly as well and drop speed to zero.
```

---
## \#9 Posted by: trbt555 Posted at: 2016-02-19T15:57:28.991Z Reads: 158

```
Yeah that would be pretty cool, kinda like hands-free perpetual steez.
I could probably pull this off in an Arduino.
I actually might give it a try.
```

---
## \#10 Posted by: laurnts Posted at: 2016-02-19T16:09:15.647Z Reads: 160

```
@trbt555 That is exactly what I meant! when you push your board it senses the speed of the motor and continue to push on that speed and that is an assist! And its always in humanly power speed range (ofc we can apply speed limiter to the assists and gradually slowdown on over speed).

I am thinking of when it's pushed it maintains that speed for 3 - 5 seconds (timed) before the motor gradually slow down. And still braking is required, don't know how this could be done, but normal longboard pushed with normal speed also don't have brakes so it won't be an issue.

This could work for people like "me" who still like to kick push and cruise nicely in town without breaking a sweat. Provide that liveliness of longboarding feeling while hardly noticeable by anyone who would try to stop you.

---

@longhairedboy I have seen this youtube video and that he demonstrate this machine in TU Delft. But I still don't understand why we can't harvest this technology or at least some company try to build in for a larger scale operation as it could save tons of energy consumption.
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-02-19T17:14:08.442Z Reads: 149

```
[quote="laurnts, post:10, topic:1455"]
it could save tons of energy consumption.
[/quote]

you just answered your own question.

When something wonderful comes along with the potential to take us from mad max oppressive classist chaos to star trek socialist utopia, rich old white people get nervous and start doing what they can to stabilize their portfolios, which usually means suppressing ideas, making sure people don't get funding, and smearing the individual all over media. And sometimes buying the tech in order to shut it down for good.
```

---
## \#12 Posted by: cmatson Posted at: 2016-02-19T18:14:29.644Z Reads: 147

```
I'm starting to really like this idea with the RPM sensing.. 

Especially having a controller free board without foot pads like the zboard:

Maintaining your speed for a couple seconds, dragging your foot to slow down.. seems like the perfect cruiser. 

You could also have a pretty small motor and much smaller battery since again, it would be doing minimal effort and wouldn't have to be powering you at all times.
```

---
## \#13 Posted by: laurnts Posted at: 2016-02-19T18:47:21.688Z Reads: 141

```
I don't trust ZBoard way of controlling the longboard, I think it's dangerous (my perspective). Especially for beginner rider as you want to stop eventually you accelerating due to wrong posture. Also on higher speed repositioning / keep positioning legs at same spot all the time are not that flexible.

Pretty sure VESC combined with hall sensor have enough computational power to measure and process the assisting function. Also for braking I think it's easier if VESC could detect sudden drop in motor rpm and then slowly applying brakes strength depending on the rpm of the motor. Hence on faster speed it slows down longer (longer braking distance) than slower speed (shorter braking distance).

After all it still would be nice if throttle input are active all the time in case of downhill braking / hill climbing is required, then just push on the stick all the way.

I am actually curious what Vedder would think about this :smiley:
```

---
## \#14 Posted by: lox897 Posted at: 2016-02-19T19:23:37.643Z Reads: 130

```
Great idea @trbt555 This would be a great feature for an eboard. Hope you can get it done, and make sure to make a thread! Good luck!
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-02-19T19:52:19.908Z Reads: 135

```
on downhill a gyroscope would be a good idea so that it can sense when its gaining RPM due to an incline as opposed to being pushed. That way it doesn't continuously try to match speed on a down slope as the board is speeding up due to gravity. 

not that a typical dual drive setup really picks up a ton of speed on a downhill with no throttle. in my experience the drag from the motors is kind of nice for keeping things from getting out of hand. When i want things to get out of hand downhill i'll whip out my Gravity push board and make sure they get out of hand properly.
```

---
## \#16 Posted by: trbt555 Posted at: 2016-02-19T20:22:34.932Z Reads: 135

```
A push assist board wouldn't have a max speed you can't jump off and run out.
How fast can you push a skateboard on level terrain ?
That would be the max speed, so when you hit a downhill, it couldn't get out of hand.
```

---
## \#17 Posted by: lowGuido Posted at: 2016-02-19T22:21:28.745Z Reads: 129

```

this is a pretty cool idea... and really easy to do!
I think I'm going to have to do this as a project!
```

---
## \#18 Posted by: lowGuido Posted at: 2016-03-05T11:14:27.858Z Reads: 122

```
Well i set my hackbboard up for push assist today and results are promising. I need some more parts to make it more solid. But this could be one of my favourite controls yet!
```

---
## \#19 Posted by: trbt555 Posted at: 2016-03-05T11:16:58.810Z Reads: 123

```
Could you post details please ?
```

---
## \#20 Posted by: laurnts Posted at: 2016-03-06T00:14:31.710Z Reads: 124

```
Yea I agree we need some details on what you did @lowGuido :smiley:
```

---
## \#21 Posted by: lowGuido Posted at: 2016-03-06T00:36:24.154Z Reads: 121

```
all in good time! it is just proof of concept at the moment, I need to make some minor adjustments and then I will get a video up!
```

---
## \#22 Posted by: vince.fab Posted at: 2016-03-06T00:45:11.025Z Reads: 121

```
Awesome!  Can't wait for details!
```

---
## \#23 Posted by: lowGuido Posted at: 2016-03-10T10:58:23.374Z Reads: 123

```
Video in my build thread.
http://www.electric-skateboard.builders/t/low-guidos-hack-board-for-science/870/41
```

---
## \#24 Posted by: orkunturkey Posted at: 2017-10-04T10:24:56.443Z Reads: 52

```
I know I am bringing back this discussion from a long time ago, but I was wondering how it would be possible to use a permanent magnet AC motor in a skateboard application? Any ideas?
```

---
## \#25 Posted by: Cobber Posted at: 2017-10-04T10:31:55.964Z Reads: 49

```
yes I think a good 250w push assist board could make target/walmart global distribution numbers... not that I would ever buy one.

If you think you can get one going before christmas, you will make more money than jason...
```

---
