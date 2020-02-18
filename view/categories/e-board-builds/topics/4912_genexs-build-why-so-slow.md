# Genex&rsquo;s Build - Why so slow?

### Replies: 29 Views: 3621

## \#1 Posted by: Genex Posted at: 2016-06-18T04:54:10.272Z Reads: 297

```
I'm going to post my boar specs here and ask for help.

I just got my board built, and it is massively slow.  Lets start with specs.

SK3 5065 236kv motor

120A x-car beast series esc

14t motor pulley, 40t wheel pulley, 70mm wheels.  pulley's, belt, ect are all 5mm

2x 5000mah zippy 3s lipo batteries (series for 6s2p, 24v)

some cheap $20 quanum 3ch rx/tx

I managed a max speed around 6-8 mph max.  I ran it for probably 3/4 mile full throttle at that speed to see if it heated up, and it was barely warm.  Am I missing something?  My end points on my controller seem fine, 24v should theoretically with 70% efficiency give me a bit over 10mph.  I am shooting for 20mph, as you would expect.  I'm not sure how I am supposed to achieve this.  My motor seems to have plenty of torque, so should I be looking at something like a 15 to 36 tooth gear ratio? (fact is, it occasionally jumped the belt at something like half throttle, shame on me for having a loose belt :P) 3-5k rpm seems low for an e-longboard but at the same time the motor itself is max rated for 10s.  I would prefer at all costs to stay at 6s since I have 2 sets of batteries and an esc that is rated for 6s.

Suggestions?
```

---
## \#2 Posted by: Genex Posted at: 2016-06-18T05:00:05.447Z Reads: 285

```
Here is the list of stuff in the same order I listed them above.

Also, that theoretical top speed is from a calculator (can't post more than 2 links :wink:)

alright, heres my stuff. Only the two most important right now since I can only post two links.

http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=18126

http://www.hobbyking.com/hobbyking/store/__77144__HobbyKing_174_8482_X_Car_Beast_Series_ESC_1_8_Scale_120A.html
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-06-20T09:24:02.138Z Reads: 267

```
[quote="Genex, post:37, topic:4152"]
some cheap $20 quanum 3ch rx/tx
[/quote]

Please dont buy the quanum receiver and make the same mistake as me. You will probably regret it! Some guys say that this receiver is good but i really dislike it.

I had many problems to connect it to the esc...
it is not durable too... 

I would recommend the (FlySky, Hobbyking or what else vendor....)  GT2B or GT2E (newer version). It is much more reliable!

[quote="Genex, post:37, topic:4152"]
14t motor pulley, 40t wheel pulley, 70mm wheels.  pulley's, belt, ect are all 5mm
[/quote]

[It seems a bit slow](http://toddy616.blogspot.de/2013/07/electric-skateboard-calculator.html) but that is your decision!
I would use at least 9mm width for the belt etc...
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-06-20T14:00:09.772Z Reads: 244

```
[quote="DeathCookies, post:39, topic:4152"]
14t motor pulley, 40t wheel pulley, 70mm wheels.  pulley's, belt, ect are all 5mm

It seems a bit slow but that is your decision!I would use at least 9mm width for the belt etc...
[/quote]

it also seems like the belts are going to hit the dirt. I wouldn't use a 40T pulley on anything smaller than a 90mm wheel.
```

---
## \#5 Posted by: Genex Posted at: 2016-06-20T16:25:56.658Z Reads: 231

```
Yea, im using 9mm belt.  The 5mm is the pitch.  I purchased from 83mm flywheels and am going to use those instead.  I also am 3d printing a 36T insert for the flywheels so I can get my wheel pulley perfectly centered.  Since I last posted I came upon a few things.  I'm pretty sure the problem is from two root causes.  One being a highly imbalanced wheel.  The bolts I put in are WAY off center and I can tell it is off balance.  I think that is slowing down my top end enough to give me the results im seeing.  Also, my pulley is slightly off center, moving about 2-3mm up and down at it rotates when viewed from the parallel.  I think those two things are causing the low top end.  The off center bolts are probably the main cause, since at the higher rpms that get us to 15-20mph there is much less torque to work with, and even the smallest problem like that can slow us down.  Not 100%, mabye 95% sure, but we will find out.
```

---
## \#6 Posted by: Genex Posted at: 2016-06-20T16:26:11.433Z Reads: 210

```
see above^ :stuck_out_tongue:
```

---
## \#7 Posted by: lowGuido Posted at: 2016-06-20T23:36:43.475Z Reads: 200

```
14:40 ratio is too short in my opinion. try going for a 30T wheel pulley.
thats one reason you are slow, but what about the settings on your ESC? have you set up the low/high voltage shut down correctly?
if you go over/under the thresholds set in the ESC it will just cruise along very slowly.
```

---
## \#8 Posted by: Genex Posted at: 2016-06-20T23:46:00.670Z Reads: 191

```
I agree on the ratio, Im going to shoot for a 14/15 - 36 to start with and then go from there.  I haven't messed with my esc at all, and the stock values it comes with are pretty good for what I can tell.  Here they are.

Cutoff voltage at 3.0v/cell (there is no high voltage shut-down)
Motor timing at normal (on a scale of very low, low, normal, high, very high)  I would make this very high but I don't have a programmer.
Initial accel at high
throttle percent reverse at 60% (have this disabled on the controller)
0% throttle limit
50% braking
0% drag brake (would also change this to 12 or 15%)
Normal motor rotation
4% neutral range (doesn't really apply to anything)
6v BEC output.

None of these really ring a bell.
```

---
## \#9 Posted by: lox897 Posted at: 2016-06-20T23:52:40.813Z Reads: 170

```
Try changing to 3% neutral range
```

---
## \#10 Posted by: lowGuido Posted at: 2016-06-21T00:27:32.315Z Reads: 159

```
could just be gearing then..
```

---
## \#11 Posted by: Genex Posted at: 2016-06-21T06:40:09.325Z Reads: 157

```
I think the wheel pulley being off center in combination with the less than perfectly weighted wheel are causing me problems.  I get my 83mm flywheels tommorow and I will throw those on with a new pulley that is centered to see if that is the root.
```

---
## \#12 Posted by: Mobutusan Posted at: 2016-06-21T07:09:39.973Z Reads: 160

```
Fix your alignment/balance issues first, for sure. And a 16/36 gearing with 97mm wheels should theoretically get you right up around the 20mph mark. 

Our of curiosity, how did you check your esc settings without a programming card? Cause I'd definitely get one of those. I thought I'd only use the card once to initially program it, but I actually find it to be a great tool that I use somewhat often to tweak settings, especially when changing setups.
```

---
## \#13 Posted by: Genex Posted at: 2016-06-21T16:11:20.510Z Reads: 146

```
The esc comes with a manual that lists its default settings along with all of the other available settings.  I would buy a programmer but the x-car beast has a specific plug and the programmers are out of sale constantly.  I haven't seen one for sale anywhere.
```

---
## \#14 Posted by: Genex Posted at: 2016-06-27T00:31:34.499Z Reads: 146

```
Update #1

Changed out the wheel pulley for a 36T which fits into a 83mm flywheel.

This definitely made it faster.  The centered pulley and  slightly higher gear ratio has brought me up to a much better 9-11 mph range.  I even got around 13-14 down a very slight hill.  I am convinced from here on now that my issues reside around my gear ratio.  I am 150 pounds, so weight isn't really an issue.  Even at full power for a good 10 minutes the motor is probably at around 100F max.  Heat isn't a problem.  I plan to switching out my 14T motor pulley for 18T or 20T and keeping my 36T wheel pulley, or possibly changing to a 32T pulley.  If  anyone has suggestions please let me know.  Gear ratio's are my weakness here, since I have no idea what people use.  I feel like my motor simply does not have the rpm's to manage high speed at lower gear ratio's, so I will have to suffice with losing efficiency to gain speed and go for a lower rpm with more torque using a higher ratio.

http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html

The calculator hasn't been accurate yet; it has been about 3-4 mph under.  As is, with my stats, it says I should be getting a 13.8mph speed with 70% efficiency.  (70% is the suggested efficiency)  but I am only around 9-11 max.

So, basically, what do you guys think of these ratio's?  Also, what do you think I should be changing if it isn't ratio's?
Motor on left, wheel on right.

14T to 32T

16T to 32T

20T to 32T

16T to 36T

20T to 36T
```

---
## \#15 Posted by: Genex Posted at: 2016-06-27T00:54:44.829Z Reads: 125

```
Btw, you were right about the ratio being too short.  I listed some ratio's; take a look at them and see what you think.  I am willing to buy a new aluminum motor pulley, but am using 3D printed wheel pulley's, so my options are limited to 40T,36T and 32T.

Obligatory pics coming soon once I get the right ratio and don't have duct tape holding the batteries to the board :smiley:
```

---
## \#16 Posted by: lowGuido Posted at: 2016-06-27T03:03:46.169Z Reads: 127

```
How fast do you want to go?
Personaly id probably go 14:32 from that selection 
However you might want to go faster than me..
The calculator is a rough guide.  Its reasonably accurate but doesnt account for real world situations. Wind, hills etc.

I probably wouldnt go too tall on the ratios id keep it above 2:1 for the sake of your esc. 

Its a trial and error game, find the speed you like and the electronics that can support it.
```

---
## \#17 Posted by: Genex Posted at: 2016-07-29T03:59:58.008Z Reads: 131

```
Update #2 

I've changed the motor pulley to a 20T, and the wheel pulley to a 30T.  This gives me a 2:3 ratio, meaning 3 motor rotations to 2 wheel rotations.

This yields me about 14-16 mph.  I am very happy with that right now.  That speed is as fast as I would like to go, but I have encountered another problem.  I would like more torque.  Which requires me to lower the ratio, and lose speed.  I am keeping the 20T motor pulley as it gives me enough teeth in mesh to never worry about belt skipping.  I am planning on moving to a 40T wheel pulley just to see what happens.  

I am confused, because I am seeing people with 5065 SK3's at 245 kv (ever so slightly higher kv over mine) having no problems getting my speed and higher on a much lower ratio.  15-36 seems common, which is WAY lower than what I am running to get that.

I would like to get more torque out of the setup.  Anyone have any idea's what could be causing me to have to use such a high ratio to achieve this speed?
```

---
## \#18 Posted by: onloop Posted at: 2016-07-29T04:04:28.290Z Reads: 133

```
i made a video about this topic, check it out: 

https://www.youtube.com/watch?v=Ficvq9aLi2Q
```

---
## \#19 Posted by: Genex Posted at: 2016-07-29T04:28:10.271Z Reads: 127

```
Yea, I had watched that when I was beginning my build.  I went with a 236kv SK3 as I was running 6s (24V).

The problem I am having is that other people with nearly identical specs are achieving the speeds I am seeing with a lower ratio than I use to get the same speed.

As a good example: http://www.electric-skateboard.builders/t/karma-v1-apex-40-single-turnigy-sk3-245kv-2x-6s-lipo-tb-6s-120a-esc-tb-mount-83mm-flywheels-nyko-kama-wiiciever/6773/6

This guy is running a 245kv 6364 and 6s and achieved a 41 kph top speed (25mph)

I cannot even achieve 20 (im getting 14-16) with a _higher_ ratio that he is using.  He is using 15-36 and I am using 20-30.  My motor is a 5065 SK3 236kv.

He seems to be having torque issues as well, but the fact remains than he is achieving a higher speed with a lower ratio.  While I have not have the chance to try a lower ratio since I started using a 20T motor pulley, I can't imagine it is going to magically produce me enough torque to get me over my current speed.

My only hints as to why I am not achieving those speeds is one of two things.  One, the roads I ride on are pure crap, fairly rough.  There isn't potholes and land mines by any means, but it isn't glorious fresh paved road either.  The second being that the ratio is so high that I am losing so much torque that I cannot get to the higher speeds.  Doesn't make any sense to me but who knows.  Also, is having a 5065 motor going to limit my top speed that much compared to a 6364?

Any suggestions would be great.  Thanks in advanced.
```

---
## \#20 Posted by: Radium73 Posted at: 2016-07-29T14:51:40.903Z Reads: 114

```
Edit: Sorry read more of the post, my bad

Another thing that might be the issue are your batteries, if you have a voltage meter it wouldn't be a bad idea to check and see if you're actually getting the correct voltage out of your batteries. If it's not that, then it either has to be a fault in your ESC or wonky settings
```

---
## \#21 Posted by: Genex Posted at: 2016-07-31T18:34:21.916Z Reads: 100

```
Yea, I am beginning to narrow things down.  I am planning on getting a VESC eventually, which will give me my answer about my ESC.  Then I plan on getting a SK3 6374 192kv or a 6364 213kv depending on what is in stock.  If for some reason my motor is the issue, then the new ones will have FAR more torque and power.  The 6374 192kv is rated for 2750 watts.  Not bad.

Other than that, the only thing I could imagine being a problem is that my motor mount could be misaligned. It looks to be perfectly square, but I also wasn't the one that welded it.  Regardless, if those two things do not solve my issues, I will buy a motor mount from torque boards.

Im pretty sure it isn't my batteries, as I have tried a different set of Venom batteries and they gave me the same results.
```

---
## \#22 Posted by: Radium73 Posted at: 2016-07-31T18:36:55.355Z Reads: 96

```
Just checking, but are you sure your batteries are joined in Series and not Parallel? A 3s battery with your setup should give the results you are getting
```

---
## \#23 Posted by: Genex Posted at: 2016-07-31T18:42:07.284Z Reads: 105

```
Yea, they are in series.  I plugged just one battery in to be sure, and it ran at half the normal speed.  Thanks for checking though.

Edit-  I am  changing my motor pulley to a 15T one right now since I have nothing better to do, so I will also change my wheel pulley to a 36T one.  Back to the optimal ratio according to most.  I will get back to you on my findings.

Double Edit- I lost my 15T pulley so we are just going to change the wheel pulley to 36T.

Triple Edit- Not much changed.  Slightly lower top speed, slightly more torque.  Going back to original setup.  I am however a bit more confident in the idea that my motor mount is off 90 degrees.  I think I am going to buy a clamp-on motor mount and a Caliber truck so I can get a perfect angle. To me this is just an experiment in finding out what could possibly be decreasing my power so much.  With a 1.5:1 ratio I get a comfortable 16mph top speed, at the expense of torque.  I am REALLY hooked onto this Esk8 thing and can't imagine me dropping the hobby any time soon, so in time I will make this board a monster.
```

---
## \#24 Posted by: Genex Posted at: 2016-08-06T19:10:53.172Z Reads: 83

```
OK,  UPDATE

I burned up my motor.  I was out with some friends and I was pulling them (2 people) for like 2 miles and my motor got WAY to hot.  I had done it before, but apparently we were going up a slight hill this time.  Regardless, my 5065 236kv SK3 is pretty beat up.  I am planning on replacing it, regardless of whether I can fix it or not.  The stator wires don't look like the covering got melted, but mabye it is in the middle.  I'll take it apart and look.

I am looking at a 63mm motor.  I want to keep the single motor design since I am going to college and it will be too bulky with a dual setup.  I do however want a 63mm motor because I would like more torque.  I was looking at literally the only available 63mm on hobbyking rn, which is a 6374 149kv.  BIG motor and LOW kv.  Rated for 2250W with 8mm shaft.

My question is, is this going to be too low of a KV?  With my current setup, I have to replace the motor pulley regardless because the shaft is 8mm, so I will have the option of changing my motor pulley to something different.  I currently have a 20T/30T motor/wheel pulley which works with my current setup.  I can change the wheel pulley to almost anything between 30-44 since it is 3d printed.
```

---
## \#25 Posted by: rockyqms Posted at: 2017-02-02T01:50:51.116Z Reads: 54

```
Did you end up figuring out this issue? I'm working on a similar build and my board is also only running 6-8mph.
```

---
## \#26 Posted by: Genex Posted at: 2017-02-02T07:24:30.926Z Reads: 48

```
Not really,

I switched the motor to a 6374 230kv motor rated for 3200 watts at 52V and it stills goes a slower than i'd like.  Albeit, it has more torque, still no top end.  I attribute it to my esc and assume I won't be able to get around it until I switch to VESC and higher voltage.  I get around 12-16 mph on flat ground with a 6s build.  Motor and esc never even get warm.  

I run a 20t to 34T gear ratio if that matters.

I also daily the board to and from class and it's had the shit kicked out of it and it never stops kicking so i'm happy with the esc.  I will enjoy higher speed and controlled braking in the future though.
```

---
## \#27 Posted by: Tuomalar Posted at: 2017-02-02T08:07:02.460Z Reads: 50

```
That 20T motor pulley is waaaaaay to big. "Standard" is 15/36 and with 34T I would use 14T motor pulley. Use those calculators so you know what is wrong.
```

---
## \#28 Posted by: Genex Posted at: 2017-02-02T23:32:06.502Z Reads: 47

```
There is no standard when you DIY.  Also there is nothing wrong with a 20T pulley, it just decreases torque to increase wheel rpm.  I need top speed, not torque, since I run a 3300 watt motor.  My motor can pull the board out from underneath anyone under 300 pounds at 24v, let alone 52v at a 20/34 ratio.

Are you suggesting a higher gear reduction would increase my top speed? lol

I know 20/34 is not a normal ratio, but it is what I use to get what I need.  My ESC is duty cycle based, and thus lacks some top end speed.  I counter this by lowering the gear reduction to gain back the top speed.
```

---
## \#29 Posted by: Tuomalar Posted at: 2017-02-03T00:16:23.699Z Reads: 43

```
So tou run 6374 230kv motor with 6s battery, 20/34 ratio.  What wheels you use? And van you link that esc? 

I think that gear ratio is too heavy. You get hi speed but your torgue is so bad at top speed that it actually is slower than lighter ratio. For example 15/36 decent amount of torgue and speed with 80mm-90mm wheels. 

You should use same settings as everyone else. Like 15/36 ratio, 80-90mm wheels, 12mm belt, 
190kv/10s or 240/6s motor/battery
```

---
