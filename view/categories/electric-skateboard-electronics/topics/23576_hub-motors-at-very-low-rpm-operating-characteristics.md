# Hub motors at very low rpm - operating characteristics

### Replies: 30 Views: 2008

## \#1 Posted by: mfidelman1 Posted at: 2017-05-20T23:54:41.448Z Reads: 162

```
Hi folks.  I'm busily designing a motorized walker (the kind old folks use) - essentially, a very wide electric board with handrails.  The key thing being that it will operate at very low speeds (4mph max).  My 96-yo dad has been jonesing to add power to his walker, so I'm trying to oblige.

I've worked out a design using a standard belt drive, with a very high gear reduction ratio - but, for all the obvious reasons, I'd much rather build around a dual hub motor configuration.  The thing is, that implies the motors turning at roughly 400rpm at 4mph (if I did the math right).  The Maytech hub motors are rated at 60KV so, that implies that I'll be running between maybe 1.5v - 8v and pretty high currents.

Does anybody have any experience/data/power curves for how these things run at low revs, with different rider weights?  I've seen these things accelerate from a standing stop - so they can obviously generate the necessary torque - but what low speed operation implies for power consumption, and for optimal battery specs, is beyond me.

Any thoughts?

Thanks!
```

---
## \#2 Posted by: treenutter Posted at: 2017-05-21T04:01:19.046Z Reads: 147

```
Glad to see this question come up because low speed control is something we don't talk about much here. 

Will you use VESC?
```

---
## \#3 Posted by: mfidelman1 Posted at: 2017-05-21T13:15:45.415Z Reads: 129

```
Re. VESC:  Probably.  

Though... I'm thinking very simple controls.  Either on/off button for each motor, or a off/low/high toggle for each - with tank steering.  It's been suggested that a basic servo tester might be sufficient.
```

---
## \#4 Posted by: Hummie Posted at: 2017-05-21T19:11:49.180Z Reads: 112

```
How good is his hearing?  The vesc is more expensive but can be super quiet. And at those slowest speeds you'd definately want sensors added in the motor.  I'd think you'd be more interested in these things than the motor efficiency at such low speed as you'll use so little power it's not worth thinking about. 
How would these work on the walker exactly?  Might as well add a platform on it and just ride it maybe
```

---
## \#5 Posted by: mfidelman1 Posted at: 2017-05-21T21:01:10.798Z Reads: 99

```
Hearing is not great.   Good point.

Re. how it would work, I'm looking at two options, both have platforms (the whole point is to ride!).
1.  Basically a platform with a dual-hub motor skateboard truck underneath, and a pair of casters, bolted to the walker frame.  (An oddly shaped e-skateboard bolted to a walker frame.)

2. uumotor makes some nice-looking hub-motor-tire combinations, designed for scooters - which could just replace the wheels on the walker.  Still need a platform to stand on, but all it needs are some unpowered wheels.

By the way - I understand that you make hub motors - where can I find info on them?
```

---
## \#6 Posted by: Hummie Posted at: 2017-05-21T21:22:07.223Z Reads: 91

```
I was trying to say if sound is important you can run the vesc in foc and quieter than all others. 

I don't have any motors now and will in the near feature but they're way more powerful and over-built than what you'd need unless your dad wants to bomb up hills on his walker at 30mph.  Is he that kinda guy? I'll post stuff on my site steelhubs.com in a couple weeks when they're ready 
 
I'm trying to imagine how you'd set it up: casters in the rear I imagine.  Maybe that would work fine but I still wonder.  It would be annoying to have to slow down and then redirect the walker towards a new direction all the time to turn. Does it have to be a walker?  If only it could turn.
```

---
## \#7 Posted by: mfidelman1 Posted at: 2017-05-21T22:16:42.323Z Reads: 83

```
I'm thinking tank steering.  Dual motors, selective application of power.  Should work either with replacement front wheels, or with a dual-up truck at the rear of the platform.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2017-05-21T22:36:01.246Z Reads: 83

```
Why are you running such low voltage? ? ? 

[quote="mfidelman1, post:1, topic:23576"]
I'll be running between maybe 1.5v - 8v and pretty high currents.
[/quote]
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2017-05-21T22:38:10.579Z Reads: 73

```
Also...hub motors...if you run to low a voltage it will be like a car starting in 2nd or 3rd gear at start up....you don't want this and will likely eventually burn out the motor pushing high currents through it
```

---
## \#10 Posted by: mfidelman1 Posted at: 2017-05-21T23:26:17.371Z Reads: 72

```
Perhaps I need to understand the motors better.  I was under the impression that rpm is a function of applied voltage.  Or am I missing something?
```

---
## \#11 Posted by: lowGuido Posted at: 2017-05-22T02:51:46.735Z Reads: 68

```
I dont think hub motors are what you are looking for. If you run a belt drive you can gear down so that you can get the desired speed without stressing the motor(s)

Dont be scared of belt drive its not that hard to maintain.
```

---
## \#12 Posted by: Hummie Posted at: 2017-05-22T04:42:41.357Z Reads: 66

```
depending on the load your dad wants to put on the motor you may need either a controller that can put out a lot of amps or one that can put out a huge amount.  But the motor should be able to perform as good as 12s I believe.  When using a standard brushless esc the voltage the motor sees is an "effective voltage" much lower than the pack voltage.  Hooking 50 volts directly to the motor would be a huuuuge current.  Ohms law math would tell it. 

Amps seem to be the only value in an inductor motor coil
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2017-05-22T04:49:56.667Z Reads: 66

```
It's is.....but...the higher voltage is like eating spinach for Popeye the sailor...so spinning at low speed takes very little amps....which is better for the motor ....at the voltage you noted...the wheels wouldn't even spin ..... 

At the very least use a 6s system....I think those maytechs are rated for that also you'll need a sensored motor setup to avoid the motor bog down or chatter starting from zero mph .... it will make it a smother start
```

---
## \#14 Posted by: Hummie Posted at: 2017-05-22T17:37:08.625Z Reads: 58

```
As long as there's enough voltage to put amps into the motor determined by ohms law, which is very little voltage needed since the motor resistNce is very low, you can put many amps into a motor and get the same performance as with high voltage.  Same heat produced. Same torque produced.

If u put a very high amp esc on the motor and set it's limits high amps it will work.  And ironically be slightly more efficient than with high voltage due to being run at a higher duty cycle while low speed
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2017-05-22T18:21:16.066Z Reads: 55

```
Yeah but it's not a good idea .... it's on the verge of ridiculous to try .... 


Don't do it ...it's stupid 


Rethink your plan
```

---
## \#16 Posted by: Hummie Posted at: 2017-05-22T19:05:28.476Z Reads: 51

```
theres nothing rediculous or stupid about it and as long as the esc can put out the amps it will perform just as well if not better.

  if you used the vesc and low voltage you will likely hit an over-temp shut down from using so many amps and you will still have low torque as the vesc has programing that limits the motor amps to 120.  (120 motor amps at 5% duty cycle or 5% of max speed when using 48 volt battery will only give you about 2.5 "effective volts" and add that up and youre at only 300 watts)

 if you use the vesc and use high voltage it will work fine just be a bit inefficient but you will have the torque and power you want. 
 if you use a 12v esc that can do 200 amps you will be the slightest bit more efficient and probably have even more torque than the vesc even with high voltage because of the 120 motor amp limit.

 Have you ever seen a 12v car battery running a car starter-motor go-kart?  they can be crazy powerful at low voltage if the amps are put in.  there isn't any extra heat and high voltage is cooler in power lines but not a motor
```

---
## \#17 Posted by: mfidelman1 Posted at: 2017-05-22T19:19:01.745Z Reads: 52

```
Re. motors being "overbuilt."  can you elaborate in two regards:

1. Basic horsepower.  I'm thinking that, at low speeds, with a walker frame attached, there's going to be a good amount of mechanical drag - so the thing won't coast a lot.  That suggests that the motors will have to run for long periods, with all the wear and heat involved.

2. Ability to run for long periods with no maintenance.

Any comments on these?  Thanks!
```

---
## \#18 Posted by: Hummie Posted at: 2017-05-22T19:22:15.456Z Reads: 52

```
if youre using castor wheels as the other two non-hub motors it wont be much drag.  
unless youre doing steep hills or going very fast I doubt you'll have any heat issues even if going for long periods.  you wont be using much wattage on a walker likely.  
hub motors have less maintenance needed.

you wont need anything "overbuilt" in terms of power or mechanically other than an overbuilt esc if you use low voltage
```

---
## \#19 Posted by: Hummie Posted at: 2017-05-22T21:02:58.757Z Reads: 49

```
But I agree and he should get a low kv motor and higher voltage and the vesc. He will lose out on something any other way i think.  get vesc on foc program at all costs It's an interesting question bringing up kind of abstract understanding of how the esc and motors work and I think I have it right and hope someone who has a different understanding explains

 @mfidelman1  are u saying ur going to drag the walker?  I still don't think it would be a problem to run it continuously with any hub motors out there and they won't overheat. Unless he were to ride on the walker and it's dragging.  Don't know what ur plan is really.
```

---
## \#20 Posted by: Michaelinvegas Posted at: 2017-05-22T21:07:53.679Z Reads: 47

```
He's not talking about 12v

He states 1.5v to 8v and based on that info I say shit idea
```

---
## \#21 Posted by: Hummie Posted at: 2017-05-22T21:22:13.708Z Reads: 42

```
Yea finding an esc that does enough amps, they all do more volts because it's impractical. But other than being practica and talking only of electrical efficiency in the motor and esc, if he were limited to an 80kv hub motor, and he wanted to also use 8 volts, and wanted to be as efficient as possible.  ..there's a simplified facet of efficiency and how u want to be riding as close to around 85% of the "no-load "speed.   There maybe be other losses in the wiring if it weren't fat but for the motor ideally I think it would be low voltage..in at least this one regard.  But overall I could be totally wrong and at that high amperage the losses in the esc and maybe even the motor would be greater.  Any naysayers?
```

---
## \#22 Posted by: Michaelinvegas Posted at: 2017-05-22T21:26:14.749Z Reads: 45

```
But practical is what is needed here....no need to invent new stuff... Just need to apply the available products to his needs...there is plenty of expertise here that can get him to feasible solution that is simple and cost effective
```

---
## \#23 Posted by: Michaelinvegas Posted at: 2017-05-22T21:27:26.896Z Reads: 43

```
Do you have a basic drawing of how you want this to look?
```

---
## \#24 Posted by: mfidelman1 Posted at: 2017-05-22T22:16:12.475Z Reads: 40

```
That was a mistake in my math and understanding of how KV ratings work.  Suggestions are welcome.
```

---
## \#25 Posted by: Michaelinvegas Posted at: 2017-05-22T22:56:24.696Z Reads: 42

```
Keep it simple....
 
You biggest issue and concern is being able to keep it at a low speed, with lots of torque 

The vesc with @Ackmaniac program should be able to manage the motor power and speed .... even if you had a simple 10s lipo set up in a pouch ... even at that high a voltage you can get it to creep along (use sensored motor set up)
```

---
## \#26 Posted by: Ackmaniac Posted at: 2017-05-22T23:37:33.538Z Reads: 40

```
So i guess what you need is something that has a decent amount of torgue at very low speeds.
Just to keep it relatively cheap and easy i think the best idea would be to have big wheels with a very high gearing.

A 6S LiPo would be good because it is easy to get and chargers are also cheap.
Then go with sensored motors with as low kv as possible.

If you have later on a gearing of 12/40 and a 140kv motor you will reach 6 km/h (4 mph) at around 8V.
With a 6S battery this will be at 34% duty cycle.
All in all this should be more than enough.

Then you can attach a thumb remote to the frame so that your father can control it. And by fine tuning it should be possible for him to control it to his needs.
The bigger problem i see is that when all of this can roll then it won't give him much support when he looses balance. And i think that is the main reason for a walker.

Wheels: 97 mm blank wheels on ebay (25$ only USA)
Motor: 140kv Evolve motors from china (50$ a peace)
Battery: 6S LiPo (? ebay)
Charger: IMax B6 (25$ for a clone)
```

---
## \#27 Posted by: Hummie Posted at: 2017-05-23T00:46:37.112Z Reads: 34

```
[quote="mfidelman1, post:24, topic:23576"]
of
[/quote] @mfidelman1 what is this thing your planning to make. No drawing.

Damn my writing is unreadable above. And probably wrong besides.
What are the losses in the esc vs motor ?? In my experience no over temp on the vec just overheat motors. The losses in the vec are very small I think.
```

---
## \#28 Posted by: mfidelman1 Posted at: 2017-05-23T01:20:06.702Z Reads: 36

```
take a look at https://www.youtube.com/watch?v=1FSWf8vG0kI&t=18s333 at around 1:34

now that was built from a canabalized rascal scooter, but the same idea - what I haven't decided yet (and will probably determine from experimentation) is whether to 
a. power the front wheels (e.g., using scooter type wheel motors)
b. put an e-skateboard truck underneath the platform (with your kind of hub motors)

The choice is coming down more to one of parts availability.
```

---
## \#29 Posted by: Hummie Posted at: 2017-05-23T02:33:37.642Z Reads: 35

```
Watched the video.  I think the possibility of using a skate truck if it were already there alway, part of the walker, in front, and a caster wheel at either side.  A four wheeler that worked kind of like a tripod is what I like. It would be nice if u could weld a frame. that could take a while.  I have no idea how to do it but could be awesome.  Grandpas speeding all over with overpowered silent vecs n hub motors on Harley skate choppers.
```

---
## \#30 Posted by: mfidelman1 Posted at: 2017-05-23T12:16:26.931Z Reads: 27

```
Well... I have visions of grandmas racing the things, but... :slight_smile: 

As to construction.  My dad really wants to convert the walker he already has - basically clamp on a platform that holds all the power components, mounted on a hinge at the front, so it can fold up the same way the current walker does.  Skate truck(s) and motors would be on the bottom of the platform.

My concerns keep coming back to battery capacity and heat, when running the motors at low revs, and low efficiency.
```

---
