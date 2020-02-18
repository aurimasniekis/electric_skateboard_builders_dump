# When will a motor move you?

### Replies: 77 Views: 1827

## \#1 Posted by: Acidfie Posted at: 2018-03-09T22:30:16.473Z Reads: 261

```
since the whole esk8 thing started, almost everyone is using a longboard with motors of 50 or 63 diameter.

but the real question here is, a nearby project i am thinking of building an electric skateboard (not the longboard). so 50mm wheels or smaller. a normal standard skateboard.

it should not be fast, it should be easy to carry, lightweight and it should **move me**.

so mechanics and stuff is not the problem, but i am concerned about the motors - so here is the question.

how can i find out which is the smallest possible motorsize i can use? sure the gear ratio also plays a role but this i can change. so 30 in dia? 35? outrunner?

i think 15-20km/h is the perfect and comfortable speed to move for citys and stuff.
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-03-09T22:41:43.743Z Reads: 244

```
50mm wheels will be extremely hard to do, and it may not be possible at all. You will have to use tiny pulleys, and the motors won't have a lot of power either. Another problem will be the kv of the motors. 
Its very hard to find a 3542 (for example) motor with a kv lower than 1000. Which is obviously waaay to high for our needs. 
These are just some of the problems you`ll have...
To be honest I dont really see the point of electrifying something with smaller wheels than 83mm, but that just me..
```

---
## \#3 Posted by: Acidfie Posted at: 2018-03-09T22:45:34.734Z Reads: 235

```
this is why i am asking here, i am playing with that thought, what if the gearing ratio is very high and then the kv from the motor shouldnt be a problem, or not?
```

---
## \#4 Posted by: pat.speed Posted at: 2018-03-09T22:45:45.568Z Reads: 220

```
Alien power systems might have motors of that size
```

---
## \#5 Posted by: Alex.Scheff Posted at: 2018-03-09T22:50:42.397Z Reads: 218

```
Maybe [this](http://alienpowersystem.com/shop/brushless-motors/aps-4260s-sensored-outrunner-brushless-motor-300kv-1600w/) work for you or you use [hub motors](http://www.electric-skateboard.builders/t/eu-group-buy-cheap-hub-motor-set-90-mm-new-price-collecting-orders-4-10-taken/42647)
```

---
## \#6 Posted by: FredrikHems Posted at: 2018-03-09T22:52:26.599Z Reads: 210

```
Thats the problem.. You can't really go lower than 10t on the motor pulley. And if you want 20km/h top speed, you will need an 80T pulley on the 50mm wheel (6s 1000kv setup), which obviously doesn't work..
```

---
## \#7 Posted by: Acidfie Posted at: 2018-03-09T22:53:11.605Z Reads: 204

```
what about a direct gear drive?
```

---
## \#8 Posted by: FredrikHems Posted at: 2018-03-09T22:55:51.147Z Reads: 198

```
You mean direct drive? Lets say you use the motor linked over (4260 300kv), then you`ll have 4mm of clearance to the ground... And the kv is still waaay too high, unforntnantly
```

---
## \#9 Posted by: aigenic Posted at: 2018-03-09T23:13:53.943Z Reads: 186

```
I do not recommend you to use so small wheels, you will end up replacing them...
But if you insist then I recommend you to use **HTD3 gears and belts** instead of HTD5...you will have more room for different ratios, but you will loose some torque transmission...
I think you will be able to squeeze 50mm motor , as far as I know there arent any mount for 42mm motors, so you would have to make one yourself :/ 

I would go for 270kv 5065 motor with 15/36 15mm HTD3 belt drive with 6s Battery...if you want more power you would have to place second motor diagonally (on the other truck) ([Calculations](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":270,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":50}|))

Problems you might notice: 
YOu will have to make your own pulley for the wheel...I mean making your own holes in bought pulley and wheels...the wheels wont probably last long...

Be prepared that you will have to modify your trucks for your custom motor mount and to fit the pulley...Hope you have experience with making stuff :)
```

---
## \#10 Posted by: chuttney1 Posted at: 2018-03-09T23:16:59.205Z Reads: 160

```
If having done your physics homework you have been able to find out how much force it would take to pull yourself from resting. Gearing it easy peasy once you know that first number.
```

---
## \#11 Posted by: aigenic Posted at: 2018-03-09T23:24:19.721Z Reads: 154

```
Also if you want to make your life easier, and you dont want to drill in your wheels you can buy roller skate wheels like [these](https://www.skates.com/Sure-Grip-Sweet-and-Low-Speed-Wheels-58mm-x-38mm-p/sgsweetw58.htm) (arent they sweet?) because they have holes in the core, that would make your life easier, you could just 3D print the pulley and go ;) 

I have never ever seen anyone do that, so it would be funny :D :D :D I dont see reason why it wouldnt work :D 

I dont know about any skateboard wheels with holes in core, which are as small :/
```

---
## \#12 Posted by: b264 Posted at: 2018-03-09T23:46:48.149Z Reads: 140

```
[quote="FredrikHems, post:8, topic:48640"]
You mean direct drive?
[/quote]

@Acidfie  said "gear", so he does *not* mean direct drive.  Direct drive would either be hub motors or inline motors like Carvon.
```

---
## \#13 Posted by: FredrikHems Posted at: 2018-03-09T23:53:21.385Z Reads: 131

```
Yeah, i tought so too, but there is alot of confusion around the forum about what «direct drive» really is.. So its kinda hard to tell what a person mean, if you dont know him/her.
```

---
## \#14 Posted by: b264 Posted at: 2018-03-10T00:03:02.249Z Reads: 124

```
There is no confusion, it's all spelled out with a quick search.  Gears are not direct drive.  They might be gear drive or cog drive or a transmission, but they aren't direct drive.  That's what hub motors and inline motors are.

https://en.wikipedia.org/wiki/Direct_drive_mechanism
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-03-10T09:36:35.419Z Reads: 112

```
I know that when gears are involved, its not a «direct drive», but there is alot of people around here thinking that it is
```

---
## \#16 Posted by: Acidfie Posted at: 2018-03-11T21:43:15.518Z Reads: 92

```
its geared, so still you have the chance to use 3 gears.

still, the question ist how much torque do i need to move a human beeing on the board.

saw this page here [CLICK](https://www.xootr.com/power-to-move-a-person.html)

it says, about 200-300 watts, so i think 2 outrunner should do the job with the right gearing, or not?
```

---
## \#17 Posted by: FredrikHems Posted at: 2018-03-11T22:06:47.021Z Reads: 83

```
As I have mentioned earlier its not the power that will be the limiting factor in the first place, its the whole Kv/V/Gearing/50mm wheels. If you can find a 40/32xx motor with a kv of around 100, then maaaybe.. But you likely won't, because they dont exist as far as I know. Also the riding performance won't be any good with such small motors.
```

---
## \#18 Posted by: Acidfie Posted at: 2018-03-11T22:12:47.761Z Reads: 80

```
whats the matter with the kv? still i think a motor with about 500-800 would be powerful enough if it will be geared up enough. motor turns faster but is geared down
```

---
## \#19 Posted by: ZackoryCramer Posted at: 2018-03-11T22:19:48.871Z Reads: 79

```
[quote="Acidfie, post:18, topic:48640"]
500-800 would be powerful enoug
[/quote]

Yea, up to 7mph. You lose a lot of torque the faster you go, and torque bottlenecks your power.
```

---
## \#20 Posted by: Acidfie Posted at: 2018-03-11T22:24:52.995Z Reads: 72

```
did you just calculate this? still i think 10 km/h would be enough for such a cheap build, since it moves me faster than walking
```

---
## \#21 Posted by: Acidfie Posted at: 2018-03-11T22:27:52.272Z Reads: 63

```
just found that little piece: [CLICK](https://www.mhm-modellbau.de/part-314990.php?gclid=EAIaIQobChMIiOb0n6jl2QIVBuEbCh0YwweTEAkYASABEgKduvD_BwE)

35x30 300kV
```

---
## \#22 Posted by: PXSS Posted at: 2018-03-11T22:29:18.880Z Reads: 59

```
Now you need to gear it down 3:1 roughly.
```

---
## \#23 Posted by: FredrikHems Posted at: 2018-03-11T22:31:33.868Z Reads: 57

```
That thing can pull like 7A/140w, its even less than most quadcopter motors...
```

---
## \#24 Posted by: b264 Posted at: 2018-03-11T22:32:46.926Z Reads: 63

```
[quote="Acidfie, post:21, topic:48640"]
just found that little piece: [CLICK](https://www.mhm-modellbau.de/part-314990.php?gclid=EAIaIQobChMIiOb0n6jl2QIVBuEbCh0YwweTEAkYASABEgKduvD_BwE)
[/quote]

This is much better as

just found [that little piece](https://www.mhm-modellbau.de/part-314990.php?gclid=EAIaIQobChMIiOb0n6jl2QIVBuEbCh0YwweTEAkYASABEgKduvD_BwE)

You should never have "click here" on anything.  It is a hallmark of bad design.  In EVERY case, you can make it beter by removing the thing that says "click here" or "click" or "tap" or "here".  It's like having a keyboard where the M is not written on the key, but off to the side, with an arrow pointing to the key that says "push there"
```

---
## \#25 Posted by: Acidfie Posted at: 2018-03-11T22:33:40.446Z Reads: 62

```
the question is to find the best kV/power ratio.

since you mostly need torque only for the start, when the board's moving it shouldnt be this high.
```

---
## \#26 Posted by: PXSS Posted at: 2018-03-11T22:36:08.767Z Reads: 61

```
6S is the max battery you can use.
For a top RPM of 7560. 
Geared down 3:1 yields a max RPM 2520RPM
With 50mm wheels, that is 14.75mph.
```

---
## \#27 Posted by: Acidfie Posted at: 2018-03-11T22:36:20.452Z Reads: 60

```
hey smartypants, the only thing you did in this thread is to correct people. how about beeing productive and helping with the real question?
```

---
## \#28 Posted by: Acidfie Posted at: 2018-03-11T22:38:01.829Z Reads: 60

```
seems pretty alright, since it should'nt be a highspeed thing.

i don't really know if the people on here only care for speed - but for me that looks just like this.

ever stood on a normal skateboard? ever drove more than 20km/h on a skateboard? try it, you never want to do it again.
```

---
## \#29 Posted by: b264 Posted at: 2018-03-11T22:38:06.226Z Reads: 59

```
The smallest motors I've used were 5065 and they are more than enough power.  I don't know, I suppose it's directly related to the hills you want to be able to make it up ... because even the tiniest motor will be able to keep you rolling on level ground.

So, what kind of hill do you need to take?
```

---
## \#30 Posted by: PXSS Posted at: 2018-03-11T22:39:55.650Z Reads: 59

```
[quote="Acidfie, post:28, topic:48640"]
seems pretty alright, since it should’nt be a highspeed thing.

i don’t really know if the people on here only care for speed - but for me that looks just like this.
[/quote]
I'm just doing the math dude... 
No need to get defensive. 

[quote="Acidfie, post:28, topic:48640"]
ever stood on a normal skateboard?
[/quote]
Way to be rude to the one person who was trying to help.
```

---
## \#31 Posted by: Acidfie Posted at: 2018-03-11T22:40:09.125Z Reads: 57

```
i do not think about hillclimbing at all, only small gradients, just for cruising around the city -everything here is flat, maybe 2% or 3%..

it should move me in the city from a to b, not for long distances or sth. like you would use a normal skateboard for.
```

---
## \#32 Posted by: b264 Posted at: 2018-03-11T22:41:44.964Z Reads: 55

```
Get a motor rated at 500W max, and drive it at 200W max.
```

---
## \#33 Posted by: Acidfie Posted at: 2018-03-11T22:42:43.227Z Reads: 52

```
please do not take it down the wrong pipe, i never meant to be verabally abusive to you.

i just talking about the facts, i stood many years on a normal skateboard, i just think most people here did not, so they dont know how it is to go fast on those tiny things.
```

---
## \#34 Posted by: b264 Posted at: 2018-03-11T22:49:12.118Z Reads: 52

```
Try [this 750kv 3639](https://hobbyking.com/en_us/turnigy-3639-brushless-motor-750kv.html) and let us know how it goes.  I'd try driving it at 5S

You'll probably have to kick-push to start moving but it might keep you moving pretty well.

edit: it says 3S voltage in the specs, try that
```

---
## \#35 Posted by: PXSS Posted at: 2018-03-11T22:49:50.142Z Reads: 54

```
I've been riding skateboards for 14yrs on and off now. I've done plenty of park skating as well as dh for a while now. I know what it feels like.

---

7A max for the motor at 300kv gives you a max torque of 0.023Nm. Geared 3:1 means 0.07Nm
```

---
## \#36 Posted by: PXSS Posted at: 2018-03-11T22:52:35.472Z Reads: 55

```
[quote="b264, post:34, topic:48640"]
Try this 750kv 3639 and let us know how it goes.  I’d try driving it at 5S
[/quote]
According to hk, max voltage is 3S which might be too low.
E: I just saw your edit
```

---
## \#37 Posted by: Acidfie Posted at: 2018-03-11T22:54:12.688Z Reads: 54

```
i think the only way to find out which motor is the best is trying. i think staying with 30-40mm diameter outrunner would be enough. need to look for a gearing now, think ill start with plastic gears since this will be the most often swapped part to find the right ratio..
```

---
## \#38 Posted by: PXSS Posted at: 2018-03-11T22:54:55.449Z Reads: 55

```
The main issue is still gearing...
How do you gear it down enough? 
Does hk make cheap planetary gear boxes??? I've only ever used Kontronik and Reisenauer, which are prohibitedly expensive. 

Then, how do you attach to the wheel?
```

---
## \#39 Posted by: b264 Posted at: 2018-03-11T22:55:56.850Z Reads: 51

```
[quote="PXSS, post:38, topic:48640"]
How do you gear it down enough?
[/quote]

3 axles :slight_smile:
```

---
## \#40 Posted by: PXSS Posted at: 2018-03-11T22:57:13.466Z Reads: 51

```
Ew. No. That'd be ugly
```

---
## \#41 Posted by: Acidfie Posted at: 2018-03-11T23:00:28.990Z Reads: 51

```
closed gearbox? 

1. trial and error with different gears/motors

2. designed and nice looking gearbox
```

---
## \#42 Posted by: b264 Posted at: 2018-03-11T23:02:17.941Z Reads: 50

```
I would demonstrate that there's actually a problem before trying that.  750kv on only 3S may be good with normal 2.5:1 - 3:1 gearing and 97mm wheels
```

---
## \#43 Posted by: FredrikHems Posted at: 2018-03-11T23:06:04.378Z Reads: 49

```
The problem here is that he wants 50mm wheels...
```

---
## \#44 Posted by: PXSS Posted at: 2018-03-11T23:06:08.100Z Reads: 46

```
[quote="b264, post:42, topic:48640"]
750kv on only 3S may be good with normal 2.5:1 - 3:1 gearing and 97mm wheels
[/quote]
Why would it be any different from a 50mm wheel?
If anything higher gearing would help the torque
```

---
## \#45 Posted by: b264 Posted at: 2018-03-11T23:07:03.027Z Reads: 45

```
Wheel size directly affects the gear ratio.
```

---
## \#46 Posted by: PXSS Posted at: 2018-03-11T23:07:21.973Z Reads: 48

```
I think it's doable. Its a cool challenge from an engineering standpoint. 

I would do a 2 stage planetary gearbox. 13:1 from 750kv+
```

---
## \#47 Posted by: PXSS Posted at: 2018-03-11T23:08:35.029Z Reads: 48

```
Explain. I don't see it. 
The only thing it affects in my head is the size of the gear you can mount
```

---
## \#48 Posted by: b264 Posted at: 2018-03-11T23:09:50.542Z Reads: 49

```
The circumference of the wheel is directly affected by wheel diameter, and the wheel circumference is the amount of ground covered per one revolution.
```

---
## \#49 Posted by: FredrikHems Posted at: 2018-03-11T23:10:13.207Z Reads: 49

```
2 stage = double as expensive :joy: Its definetely possible, but i dont see it efficient or proctical in any kind of way.
```

---
## \#50 Posted by: Acidfie Posted at: 2018-03-11T23:12:07.598Z Reads: 53

```
i am not talking here about efficency. i am talking here about of doability. since you never testet it, why would you know it doesnt work?
```

---
## \#51 Posted by: PXSS Posted at: 2018-03-11T23:12:26.367Z Reads: 51

```
I swear I've seen them on rc airplanes before. I have a reisenauer one but it cost €300 lol. I'm sure there must be a cheap one on hk or aliexpress or something!

Reisenauer doesn't make the 13:1 anymore either
```

---
## \#52 Posted by: PXSS Posted at: 2018-03-11T23:13:45.961Z Reads: 52

```
Right, but it doesn't increase the torque. The purpose of gearing down would be to increase torque and usable throttle range.
```

---
## \#53 Posted by: b264 Posted at: 2018-03-11T23:14:00.550Z Reads: 49

```
I don't think you need that.  Driving a 750kv motor from 3S is a similar ratio to driving a 225kv motor on 10S.  Just gear it down about 3:1 and use a big wheel, like 97mm.  It should be pretty close to good.  Adjust from there if you need to.  If you need more torque, decrease the wheel to 83mm.  For more speed, increase it to 107mm.
```

---
## \#54 Posted by: FredrikHems Posted at: 2018-03-11T23:14:44.986Z Reads: 50

```
[quote="FredrikHems, post:49, topic:48640"]
Its definetely possible
[/quote]
 
@Acidfie bruh...
```

---
## \#55 Posted by: Acidfie Posted at: 2018-03-11T23:19:11.672Z Reads: 47

```
the question is how good
```

---
## \#56 Posted by: PXSS Posted at: 2018-03-11T23:26:09.409Z Reads: 50

```
[quote="b264, post:53, topic:48640"]
Driving a 750kv motor from 3S is a similar ratio to driving a 225kv motor on 10S.
[/quote]
Yes but the motors we are talking about cannot put out as much torque as a larger one. 

Eg:
6374 sk3 200kv on 10S geared 3:1 can put out 1.2Nm
The 3639 motor you linked at 3S, geared 3:1 can put out 0.14Nm

[quote="b264, post:53, topic:48640"]
Adjust from there if you need to.  If you need more torque, decrease the wheel to 83mm.  For more speed, increase it to 107mm.
[/quote]
Changing your wheel diameter does not change the amount of torque the motor puts out. It affects your speed at a set RPM but not the torque.

---
E: I guess a larger wheel hs more inertia and therefore requires more torque to get rolling than a smaller one, but I imagine this is not that significant
```

---
## \#57 Posted by: Grozniy Posted at: 2018-03-11T23:26:16.500Z Reads: 46

```
I don't see anyone giving importance to shaft diameter. The one you posted is 5mm and previous one is 4mm. Is it not important?
```

---
## \#58 Posted by: Hummie Posted at: 2018-03-11T23:26:54.632Z Reads: 46

```
U could get a scorpion motor kit and get a small motor w a low kv made and that would be nice.  Or rewind something. Otherwise it’ll be a loud big gear n risking bottoming the motor out also and bottoming the gear out. Or too few teeth and early deterioration or slipping.  Maybe there’s a nice gearbox out there though that would suit
```

---
## \#59 Posted by: PXSS Posted at: 2018-03-11T23:28:48.029Z Reads: 44

```
Not really. As long as the pinion doesn't slip on the shaft it should be good. The only times I've seen that happen is with 3mm shafts.
```

---
## \#60 Posted by: b264 Posted at: 2018-03-11T23:37:30.226Z Reads: 46

```
[quote="PXSS, post:56, topic:48640"]
Changing your wheel diameter does not change the amount of torque the motor puts out.
[/quote]

The amount of torque the motor puts out doesn't matter.  The only thing that matters is the amount reaching the ground.  Changing wheel size drastically affects the gearing ratio.

Also OP stated hills don't matter.  I'm well aware that this will be weak.  I intentionally suggested it that way based upon what the OP has asked for.
```

---
## \#61 Posted by: PXSS Posted at: 2018-03-11T23:43:12.643Z Reads: 48

```
[quote="b264, post:60, topic:48640"]
The amount of torque the motor puts out doesn’t matter.
[/quote]
Yes it does. Motors have a stall torque. If that is not enough to move you, then the motor will burn out. That's the whole point of gearing. It's not only to get it to a reasonable RPM range.

[quote="b264, post:60, topic:48640"]
I’m well aware that this will be weak.  I intentionally suggested it that way based upon what the OP has asked for.
[/quote]
I think this motor won't turn at all and just stall unless geared properly
```

---
## \#62 Posted by: b264 Posted at: 2018-03-11T23:57:46.730Z Reads: 43

```
[quote="PXSS, post:61, topic:48640"]
Motors have a stall torque. If that is not enough to move you, then the motor will burn out. That’s the whole point of gearing. It’s not only to get it to a reasonable RPM range.
[/quote]

If the motor doesn't have enough torque to move you, you kick-push and allow it to maintain your roll.
```

---
## \#63 Posted by: Cobber Posted at: 2018-03-12T02:56:32.862Z Reads: 40

```
[quote="Hummie, post:58, topic:48640"]
U could get a scorpion motor kit and get a small motor w a low kv made and that would be nice...
[/quote]

You know of anywhere offering that service Hummie?
```

---
## \#64 Posted by: Hummie Posted at: 2018-03-12T03:01:43.823Z Reads: 42

```
you could do it.  id do it for you if you really want.  I don't know of a service but if someone asked on rcgroups I bet you could find someone.

 id like to try to see how low I could get the kv  but I'm too busy now and maybe next week!!
```

---
## \#65 Posted by: b264 Posted at: 2018-03-12T03:49:26.130Z Reads: 44

```
[quote="PXSS, post:61, topic:48640"]
Motors have a stall torque. If that is not enough to move you, then the motor will burn out.
[/quote]

That's also why I suggested running a 500-600W motor at 200 Watts
```

---
## \#66 Posted by: PXSS Posted at: 2018-03-12T04:26:03.827Z Reads: 44

```
Not really all that helpful. 

![image|504x288](upload://8nV5coPl51F0qthTV1L3U85ZHti.png)
This is what a bl motor curve looks like. 
If the motor is rated for 500W, that will be at the max power condition, which is not max torque conditions. Max torque is on the far right of the graph above. Max Efficiency is at high RPM/low torque. 

So yes, while 200W may be enough to push someone. The motor might not even put that out in high torque/low rpm conditions. Not only that but you are also running in a very inefficient point so the motor migh still overheat. That's the point of gearing a motor down using a gearbox. So that you can keep the motor at it's max efficiency range while the torque is enough for the application.
```

---
## \#67 Posted by: b264 Posted at: 2018-03-12T05:17:28.965Z Reads: 42

```
So what motor/gearing/voltage/current/wheel_size do you recommend?

That's what I don't see
```

---
## \#68 Posted by: PXSS Posted at: 2018-03-12T11:19:59.615Z Reads: 43

```
[quote="b264, post:67, topic:48640"]
So what motor/gearing/voltage/current/wheel_size do you recommend?
[/quote]
I'd try a 35-40mm motor in the 1200kv range that can do 6S with this gearbox:
http://www.integy.com/st_prod.html?p_prodid=21379&p_catid=374&ratesortby=New#.WqZgzCspCEc

I knew they existed! Freaking rock crawlers. 

That plus 50mm wheels on a 1:1 should get 13mph tops and hopefully plenty of torque.
```

---
## \#69 Posted by: Cobber Posted at: 2018-03-12T11:30:05.663Z Reads: 44

```
I'm waiting for the day the park skaters discover the skateboard version of a trials motorcycle. Something light with lots of torque (small battery) something you can trick on, manual forever... you could drive out of sketchy landings... who knows... but I look forward to that day!

https://youtu.be/GoxJP306ZE0
imagine that in a skate park?
```

---
## \#70 Posted by: b264 Posted at: 2018-03-12T11:33:19.264Z Reads: 44

```
[quote="PXSS, post:68, topic:48640"]
50mm wheels
[/quote]

Fitting a pulley to that will be an interesting task...
```

---
## \#71 Posted by: Tuomalar Posted at: 2018-03-12T11:36:09.451Z Reads: 43

```
HTD3 might work due to smaller teeths
```

---
## \#72 Posted by: Acido Posted at: 2018-03-12T15:07:52.201Z Reads: 44

```
ESCs are a problem then
```

---
## \#73 Posted by: MoeStooge Posted at: 2018-03-12T16:55:24.357Z Reads: 39

```
I can make you what you want. 35mm motor can, 2000w 1500kv Inrunner. 58t spur on a 9 t pinion steel on steel gear drive on a 50mm wheel. 25mph and torque enough to spin the rear wheel at will.  If your interested send me a PM..
```

---
## \#74 Posted by: lowGuido Posted at: 2018-03-12T18:19:14.159Z Reads: 36

```
https://www.boardworld.com.au/uploads/forum-images/33801-14a6ddf281/33801_1420448336.jpg

I did this once. just for fun. 
I think I'm actually going to build a proper version of it with an enclosure instead of tape LOL.
```

---
## \#75 Posted by: Acidfie Posted at: 2018-03-12T18:47:52.380Z Reads: 36

```
Motor? gearing? hows the driving? distance to the ground?

give us some informations hah
```

---
## \#76 Posted by: Hummie Posted at: 2018-03-12T19:00:22.472Z Reads: 38

```
i did a park board with caliber trucks and risers and fit a tacon 63 motor no problem.  or better yet get a kick tail and put it under that and no riser needed probably.
```

---
## \#77 Posted by: lowGuido Posted at: 2018-03-12T19:04:09.616Z Reads: 38

```
it's a SK3 5055 280kv motor, with a 12T motor pulley and a 30T wheel pulley.
its sketchy at speed.
I have never been a longboarder so I felt good on the board, but I wanted to go fast with stability. so I put the drive gear onto another deck (40") and have been riding it ever since.
```

---
