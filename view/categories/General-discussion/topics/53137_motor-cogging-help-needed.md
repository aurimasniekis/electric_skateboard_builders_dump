# Motor cogging, help needed!

### Replies: 20 Views: 1315

## \#1 Posted by: Jaydan Posted at: 2018-04-22T17:07:28.038Z Reads: 202

```
hey guys, 

i'm having an issue with my board which i never experienced before. when i pull the throttle the motor starts cogging at a constant 'speed' (if that makes any sense). the vesc does not give any errors. max power according to vesc monitor is 11W forward and 125W backward which is nowhere near the limits.
initially i thought that it would be due to one of the phase wires having no connection. however, i tried touching two of the phase wires at a time to see if i get a resistance when turning the motor and this was the case for every combination.
unfortunately, i can't connect the vesc to the bldc tool right now to sort out any issues with my remote but will do that later on!

specs of my board:
-VESC 4.12 from  @esk8 
-Turnigy SK3 6374 192kv
-Benchwheel remote
-2x Turnigy or Turnigy 5S 5000mAh 20C battery in series

let me know if you have any idea what could be wrong..
thanks!
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-04-22T17:24:52.702Z Reads: 184

```
Are you running sensored or sensorless? FOC or BLDC? Does is cog at a low speed or high speed?
```

---
## \#3 Posted by: Jaydan Posted at: 2018-04-22T18:00:38.919Z Reads: 176

```
sensorless, bldc and cogging at any Speed :wink:
```

---
## \#4 Posted by: ShutterShock Posted at: 2018-04-22T19:50:35.773Z Reads: 169

```
You gotta get connected to your bldc tool to see whats going on.  You can learn a lot from the realtime data tab.  Also, check your battery cutoff and balancing.  Are you running through a bms? 

I had an issue a while back where I forgot to plug a balance lead into my bms and it freaked out and did this weird cogging thing like you're talking about.  Also check all your battery lead connections.
```

---
## \#5 Posted by: leroy Posted at: 2018-04-23T02:32:54.665Z Reads: 161

```
I agree.
You need the information to diagnose the problem properly, 

My cogging issues are usually caused by bad connections in the motor leads, 
I really suck with a soldering iron.
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2018-04-23T04:32:09.343Z Reads: 143

```
Pics please

Of everything
```

---
## \#7 Posted by: E1Allen Posted at: 2018-04-23T06:44:11.278Z Reads: 130

```
I had cogging issues when one of my motor sensors quit working.  Didn't really matter speed.
```

---
## \#8 Posted by: Jaydan Posted at: 2018-04-23T08:06:51.228Z Reads: 122

```
this is what the realtime data looks like when i gradually increase throttle:![Unbenannt1|690x370](upload://kFIJ0SN3Z7oJOOsF9xYZXioBehQ.png)![Unbenannt|690x370](upload://9UAhTUPz45WWWFsqwYoJfg7xkwQ.png)
i used my remote because interestingly enough the inputs from the bldc tool didn't do anything. motor was cogging all the time. reached full throttle at about 12 sec and kept it like that until my motor gave me smoke signs begging me to stop.

so obviously the root of the problem is the motor. now i'm wondering why this is happening and if i can do anything about it without having to buy a new motor. any ideas?

edit: some pictures of the motor
![IMG_20180423_101239|375x500](upload://xyZ6nlk5jSWTvhcl9u4W8dKeCA7.jpg)![IMG_20180423_101156|375x500](upload://pRVGzXzxb323pqQ8KFwa8bzB0gB.jpg)![IMG_20180423_101311|666x500](upload://9spcXo0Dz4xJbEiMQqGUH6GRIw7.jpg)
looks to me like some of the stator wires might be in contact. would this explain the cogging?

oh, and thanks so much for all the previous replies!! :heart_eyes:
```

---
## \#9 Posted by: E1Allen Posted at: 2018-04-23T08:33:33.916Z Reads: 112

```
Are any of the three phase wires touching anything?
```

---
## \#10 Posted by: Jaydan Posted at: 2018-04-23T08:58:56.322Z Reads: 112

```
negative..
```

---
## \#11 Posted by: Jaydan Posted at: 2018-04-25T12:00:59.364Z Reads: 106

```
bump!

10 chars
```

---
## \#12 Posted by: Acklavidian Posted at: 2018-04-25T12:13:33.146Z Reads: 107

```
1 or 2 motors?
```

---
## \#13 Posted by: Acklavidian Posted at: 2018-04-25T12:24:46.958Z Reads: 107

```
I would post some screenshots of your vesc settings.

[quote="Jaydan, post:8, topic:53137"]
reached full throttle at about 12 sec and kept it like that until my motor gave me smoke signs begging me to stop.
[/quote]
How long did it take to smoke?
Smoke to me means either: 
* Friction
* Short
* Current Overload

You'll have to disassemble the motor. I feel like if you have seen smoke emitting from the motor then it should be fairly obvious where the problem is once the motor is disassembled.
```

---
## \#14 Posted by: Jaydan Posted at: 2018-04-28T13:07:53.038Z Reads: 104

```
Sorry to keep you waiting! It took about 25s at full throttle until the smoke started. however, during this time the motor always did a slight rotation (approximately 1/15 of a full rotation) and stopped again at a really fast pace. this is probably why there are these beautiful sinus curves in the realtime data.

regarding the three things you mentioned:
friction - unlikely. can turn the motor by hand without any unusual resistance
short - very likely.
current overload - not the case (see realtime data)

some more pictures of my vesc settings and close-ups of my vesc:![config1|690x370](upload://z7jm3RTQfMewJ7UH53St2hgRJpQ.png)

![IMG_20180428_144404|375x500](upload://elR8c7MgDTIUp8EDn2zIQALfY09.jpg)

![IMG_20180428_144541|666x500](upload://lR0ch4B0VXfQyNHj1CNCgAl8MYW.jpg)

![IMG_20180428_144555|666x500](upload://xXvCyLwnqGcLoHNJlLGXIPU4BIy.jpg)

the settings have never caused any trouble and the vesc seems fine. except maybe for that green fluid at the solder joints. what is that actually?

in my opinion the cogging occurs due to loose motor wiring causing a short inside the motor. in fact it's wound so loosely that i can move some of the loops around with a screwdriver. this shouldn't be the case, right?
unfortunately, disassembling the motor means destroying my motor mount which is why i am still reluctant to do that. and unfortunately #2, i don't have a second motor for testing.
```

---
## \#15 Posted by: fuelre Posted at: 2018-05-02T13:32:55.724Z Reads: 91

```
you cant control the VESC by the BLDC Tool because you have a remote connected and your app config is on PPM input -> set it to disable and it works threw the keys on your keyboard.

is the screenshot done with the board on your bench or under load?
is it possible to do the motor detection?
```

---
## \#16 Posted by: Jaydan Posted at: 2018-05-03T08:36:51.931Z Reads: 77

```
gotcha! it's been awhile since i last played around with the bldc tool and totally forgot about that setting. didn't change anything about the outcome though. i still get the same stuttering when using my keyboard.

the data stems from bench testing. also motor detection doesn't work. just tried to do one but the bldc tool gave me a 'detection failed' error.
```

---
## \#17 Posted by: fuelre Posted at: 2018-05-03T10:41:14.401Z Reads: 74

```
as Acklavidian mentioned, you have probably a short or a break in the cables.
if you have a multimeter meassure the resistance of all phases to each other and compare the values
```

---
## \#18 Posted by: Jaydan Posted at: 2018-05-03T13:58:09.059Z Reads: 73

```
already did that. got the same resistance (0.01) on all phase wires. however, the guys over on rcgroups.com noted, that there might be a difference too small to measure with most multimeters. additionally i measured the resistance between phase wires and stator and got no reading.
```

---
## \#19 Posted by: Jaydan Posted at: 2018-12-12T15:45:48.020Z Reads: 49

```
since i am still having issues it's unfortunately time to revive this thread. here is whats going on at the moment:

i've got 2 ESCs (brandnew FOCBOX + older 4.12 confirmed to be alright by @Martinsp) and 2 brandnew motors. the old sk3 is definitely dead. however, no matter which combination of esc and motor i try the motors are at times still cogging. sometimes they work fine and motor detection works. yet, they are especially likely to cog when i go full throttle at once using my remote or applying 5k-10k or above within the BLDC tool. 

this behavior seems really odd to me. initially, i thought that a new esc and motor would solve my issues. unfortunately, this has not been the case.

any ideas? so far, i only bench tested the board and don't feel comfortable taking it to the street.
```

---
## \#20 Posted by: legend27 Posted at: 2018-12-12T16:25:38.529Z Reads: 47

```
Try to run it in FOC sensored. I also have the same problem and made a thread about it. You might be able to find a solution in the thread.

https://www.electric-skateboard.builders/t/motor-cogging-on-startup-with-load/75592?u=legend27
```

---
