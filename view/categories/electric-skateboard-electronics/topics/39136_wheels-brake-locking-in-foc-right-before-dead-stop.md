# Wheels brake locking in FOC right before dead stop

### Replies: 89 Views: 2066

## \#1 Posted by: Eboosted Posted at: 2017-11-24T04:31:25.064Z Reads: 302

```
I'm runing the latest v0.86 version of BLDC tool in FOC and Focboxes.

Braking is ok but if I continue braking right before a dead stop wheels lock and i get thrown forward, it seems to be a common issue.

How have you guys fixed this?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-11-24T04:37:27.421Z Reads: 279

```
[quote="Eboosted, post:1, topic:39136"]
How have you guys fixed this?
[/quote]


By running BLDC mode.:wink:
```

---
## \#3 Posted by: Eboosted Posted at: 2017-11-24T06:32:48.991Z Reads: 273

```
I'm not sure what happens on BLDC but it gives me hall sensor error only on the slave vesc!

I had to go back to FOC. After testing I found the brakes to be much weaker than previous version, even at batt min -25A and motor min -60A
```

---
## \#4 Posted by: Namasaki Posted at: 2017-11-24T11:42:57.476Z Reads: 247

```
I run BLDC 
No sensors
No canbus (I use split ppm)
And I get no problems 
Good torque 
Good speed
Good brakes
Just kept it simple
```

---
## \#5 Posted by: florensvb Posted at: 2017-11-24T14:44:54.087Z Reads: 231

```
I had the same thing in Foc and fixed it by lowering the Motor Min. It will still work well enough at high speeds but not as crazy at low speeds. Play around with it
```

---
## \#6 Posted by: Sender Posted at: 2018-06-14T05:28:22.242Z Reads: 218

```
 @Eboosted did you ever figure this out? I am having a similar behavior on ack firmware hybrid mode 12s5p. Not that bad at all really, just a little annoying.  I would love for it to be gone though.
```

---
## \#7 Posted by: Eboosted Posted at: 2018-06-14T05:36:47.927Z Reads: 211

```
No. I'm still having this issue.

@ackmaniac told me the issue was low speeds ERPM detection, the firmware just reads zero ERPM and brakes go into full brake
```

---
## \#8 Posted by: Sender Posted at: 2018-06-14T05:55:35.907Z Reads: 210

```
Hmmm, unfortunate.
```

---
## \#9 Posted by: lrdesigns Posted at: 2018-06-14T07:27:01.350Z Reads: 201

```
I had the same issue in BLDC, and it can be fixed by changing the setting "max ERPM at fully brake" to a lower number. 

But I don't think FOC gives you this same setting to mess with?

![image|329x114](upload://taoe3BiMl6VryuBQCUaUSu9sovz.png)
```

---
## \#10 Posted by: Eboosted Posted at: 2018-06-14T15:47:04.784Z Reads: 197

```
Yeah, FOC does not have that feature :disappointed_relieved:
```

---
## \#11 Posted by: Sender Posted at: 2018-06-14T15:50:09.404Z Reads: 197

```
It is odd. I would prefer it never going to complete stop than locking up at 1-2 mph.  But I'll get used to it.
```

---
## \#12 Posted by: Eboosted Posted at: 2018-06-14T17:15:30.943Z Reads: 196

```
I got used to it but everytime my GF rides it, she complains. It's just not perfect as I'd like.

The problem seems to not happen on the Raptor 2 though, they are runing a modified @ackmaniac FW
```

---
## \#13 Posted by: Sender Posted at: 2018-06-14T17:24:24.813Z Reads: 195

```
It really makes me wonder.  As soon as I felt I thought of your post.

There are many dual 12s 6374 builds around.  But I don't see much at all mentioning it besides this...

I am going to get into the settings a but more later. I have to pull off my enclosure anyway as I have my BT module (standard, not METR) hooked up and can connect to the board, but I am getting no telemetry.  Gotta go figure that one out.

Also, off topic,  I am about to lay down some hexagon grip tape on my board.  What process do you use to keep everything so even?
```

---
## \#14 Posted by: Eboosted Posted at: 2018-06-14T17:28:55.277Z Reads: 181

```
[quote="Sender, post:13, topic:39136"]
pic, I am about to lay down some hexagon grip tape on my board. What process do you use to keep everything so even?
[/quote]

Damn, I had all my boards with the same issue, not eworking on the standsr HM10 module, however on my case I can't even connect.
```

---
## \#15 Posted by: Ebisane9 Posted at: 2018-06-14T18:21:10.724Z Reads: 171

```
Hey @Sender Sender, Although I have 10s Dual 6374 I also get a similar issue, for I'm running hybrid bldc and the solution that @lrdesigns suggested is what worked for me. Now with foc, I have no idea. Maybe @Deckoz @mmaner can chime in? They're people i talk to fairly regularly and I know they use FOC.   @JLabs is also good at diagnosing so maybe some VESC/BLDC tool screenshots might be good.
```

---
## \#16 Posted by: Sender Posted at: 2018-06-14T18:24:19.544Z Reads: 166

```
I plan on doing a bit of tweaking and honing to find my sweet spot.  Those 2 guys are my biggest resources on here!

Are you running Ack?
```

---
## \#17 Posted by: Sender Posted at: 2018-06-14T18:28:21.299Z Reads: 161

```
Yeah, I figured if it didn't work, I wouldnt even be able to see the module.

I can connect just no values for telemetry. Funny thing is when I first connected I was getting my voltage.  Then, the next day I could connect but not see any telemetry.

I couldn't take it anymore so I zipped it up and went riding.  I want to believe I will sort it tonight... but the temptation to just go ride is so real.  I still need to find 3 hours to elegantly lay that grip tape....
```

---
## \#18 Posted by: mmaner Posted at: 2018-06-14T18:34:40.206Z Reads: 158

```
I wish I knew, all of my FOC boards do that.  Ive just gotten used to it, dont even think about it anymore.  Its just before full stop.
```

---
## \#19 Posted by: surprisebirthday Posted at: 2018-06-14T18:43:44.976Z Reads: 159

```
Yup, the full brake when going slow happens to me too.  I'm running dual 6374s in Ackmaniac's FOC.  

I did used to run FOC on dual Hummie hubs using 2.18, and I do not recall having this issue if that helps people pinpoint a potential solution.
```

---
## \#20 Posted by: Battosaii Posted at: 2018-06-14T18:46:20.576Z Reads: 161

```
Hmm thays weird that sounds very similar to the braking problem I have with my Raptor 2, once they fix my BMS problem (board wont turn off) I'll try out the board in BLDC and see if the problem persist.
```

---
## \#21 Posted by: Ebisane9 Posted at: 2018-06-14T19:41:14.237Z Reads: 154

```
Yeah i'm running ack. I ran 2.54 then now I run 3.1. for some reason I feel like 2.54 Is undefeated but I can't downgrade sooo.. I just feel like watt no reverse with brake, although it is now apparently named current no reverse with brake, was very different. I'm still getting used to 3.1, it's crazy how much a firmware update can change the feel

Edit: it seems like everyone on foc has the same experience. I got used to it, you will as well. It's just annoying and sounds slightly bad lol
```

---
## \#22 Posted by: skatardude10 Posted at: 2018-06-14T21:36:16.270Z Reads: 152

```
It'd be great for this to go away. 10S dual 6374 FOC and same thing here. Only time my belts skip is the last moment when slowing down... I have to anticipate it so my belts don't skip and wear down the pulleys.
```

---
## \#23 Posted by: lrdesigns Posted at: 2018-06-15T00:23:52.066Z Reads: 152

```
I'm on ackmaniac 2.54 also, its just so nice I don't want to update.
```

---
## \#24 Posted by: ervinelin Posted at: 2018-06-15T12:50:28.150Z Reads: 150

```
I have 3 boards all running FOC. Only my dual 6374 exhibits this problem... 

I just built it, and was kicked off the board as I came to a slow stop down a slope... Tried on flat terrain.. same.. 

Any solution? Will reducing motor min help?
```

---
## \#25 Posted by: Eboosted Posted at: 2018-06-15T15:01:53.739Z Reads: 146

```
No. Reducing motor min won't work.

It seems to happen on boards with bigger size wheels, not sure if it's related. 

What wheels do you have on your dual 6374?
```

---
## \#26 Posted by: ervinelin Posted at: 2018-06-15T15:03:45.758Z Reads: 145

```
8" ATs.. have u tried lowering motor min? Didn't work?
10char
```

---
## \#27 Posted by: Sender Posted at: 2018-06-15T15:04:55.722Z Reads: 142

```
I am rockin 107s...
```

---
## \#28 Posted by: Eboosted Posted at: 2018-06-15T15:06:26.970Z Reads: 140

```
Then it has to do with the wheels or higher reductions, I guess with bigger wheels the speed of the motor is faster on low speeds so its difficult to detect ERPMs
```

---
## \#29 Posted by: Mathias Posted at: 2018-06-15T16:09:37.182Z Reads: 137

```
This sounds like a hall sensor problem. Did you check at what ERPM the motor locks up? If you're still going 1-2 mph while this happens this is probably at the point where the switching from sensorless to sensored FOC happens. 
One of your VESCs had a hall error in BLDC. Did you try if the locking up is also there if you set this VESC or both to unsensored FOC? Also disabling traction control for testing is probably a good idea.
```

---
## \#30 Posted by: Ebisane9 Posted at: 2018-06-15T16:28:43.542Z Reads: 135

```
i use BLDC and no hall errors. i seem to have mitigated the problem via my throttle curve though as i reprogrammed and it doesn't happen anymore. albeit only 1  ride
```

---
## \#31 Posted by: bigben Posted at: 2018-06-15T16:32:33.242Z Reads: 136

```
I get this and I run 97mm wheels. 10s battery 15-36 pulleys FOC. Just a 1mph or so comes to a sudden stop. Just got used to it.
```

---
## \#32 Posted by: Sender Posted at: 2018-06-15T16:33:53.194Z Reads: 134

```
I am running Hybrid mode Ack 3.(mostrecent)

No sensor issues here.  Also happens sub 1mph.
```

---
## \#33 Posted by: Mathias Posted at: 2018-06-15T17:08:06.811Z Reads: 133

```
[quote="Sender, post:32, topic:39136, full:true"]
I am running Hybrid mode Ack 3.(mostrecent)

No sensor issues here. Also happens sub 1mph.
[/quote]

Well, there's the switching to "handbrake" which simply shorts the motors, but this is supposed to happen just before you come to a complete halt. I can see that the speed gets higher when you run an extremely low gear reduction. But it sounded like @Eboosted got the problem at RPMs where the tracking by the hall sensors should still work. That's why I'm asking where exactly it happens. 
But I'm just guessing what one could try to narrow down the problem. If it happens at the sensored/sensorless switching ERPM than tweaking this parameter might improve it.
```

---
## \#34 Posted by: Sender Posted at: 2018-06-15T17:25:42.652Z Reads: 121

```
I will try to get some video later if I remember
```

---
## \#35 Posted by: Eboosted Posted at: 2018-06-15T17:27:56.927Z Reads: 123

```
No issues on 90mm
Subtle lock on 97mm
107mm noticeable
200mm 8" very rough

Does not happewn on the Raptor 2 on 90mm
Does not hapen in BLDC only FOC
```

---
## \#36 Posted by: Mathias Posted at: 2018-06-15T17:37:57.844Z Reads: 130

```
[quote="Eboosted, post:35, topic:39136"]
No issues on 90mm
Subtle lock on 97mm
107mm noticeable
200mm 8" very rough
[/quote]
I see. I'm running 100 mm with 15T/36T, so probably more reduction than you on your 200 mms. But still, I had an issue at low ERPMs recently with locking up at too high ERPM, and I found that a bad hall sensor connector was the problem. 
[quote="Eboosted, post:35, topic:39136"]
Does not hapen in BLDC only FOC
[/quote]
Yeah, that's when I wondered if you tried sensored FOC but sensorless BLDC since you got the hall error there.
```

---
## \#37 Posted by: skatardude10 Posted at: 2018-06-15T19:28:07.869Z Reads: 127

```
Running 15/32 on 107, very noticeable.

Running 20/32 on 107, *very* noticeable
```

---
## \#38 Posted by: Ebisane9 Posted at: 2018-06-15T20:08:09.744Z Reads: 131

```
20/32?

Y bro. Y 😂
```

---
## \#39 Posted by: mmaner Posted at: 2018-06-15T20:53:46.754Z Reads: 133

```
[quote="Ebisane9, post:38, topic:39136"]
20/32?

Y bro. Y :joy:
[/quote]

speed...

(10c)
```

---
## \#40 Posted by: skatardude10 Posted at: 2018-06-15T20:56:35.162Z Reads: 129

```
Speed. 1010
```

---
## \#41 Posted by: Ebisane9 Posted at: 2018-06-15T21:08:11.535Z Reads: 123

```
#TorqueMatterstoo
```

---
## \#42 Posted by: mmaner Posted at: 2018-06-15T21:10:25.447Z Reads: 122

```
It does, and I built a board with this same gear ratio and was not happy with it.  But there are some skinny folks out there that can use it and still get enough torque to go.
```

---
## \#43 Posted by: Ebisane9 Posted at: 2018-06-15T21:12:15.570Z Reads: 124

```
Fair I’m 180 and even on 16/36 I’m dien. Bouts get some 44’s
```

---
## \#44 Posted by: mmaner Posted at: 2018-06-15T21:33:36.749Z Reads: 123

```
single motor or dual?
```

---
## \#45 Posted by: Ebisane9 Posted at: 2018-06-15T21:39:46.173Z Reads: 123

```
Dual 6374’s

Edit: mine isn’t slow but coming from an evolve i like a little bit of a kick. And i use tb vescs so i limit the initial
Kick a little bit with the throttle curves so i don’t pop my babies
```

---
## \#46 Posted by: Scoo_B_SK8 Posted at: 2018-06-15T21:48:35.931Z Reads: 122

```
alternative setup if ran with no brakes in settings, just came across this...

https://www.electric-skateboard.builders/t/mechanical-servo-brake/59051
```

---
## \#47 Posted by: mmaner Posted at: 2018-06-15T21:50:44.791Z Reads: 117

```
I can dig that.  You should be safe at 60/-40/60/-12.  Try that and see if its any better.
```

---
## \#48 Posted by: Ebisane9 Posted at: 2018-06-15T21:51:15.284Z Reads: 118

```
Will give it a pop bro! Cheers!
```

---
## \#49 Posted by: KickMe Posted at: 2018-06-15T22:40:31.110Z Reads: 120

```
Same problem here, dual foc, sensored, foc mode. Breaks abruptly just before stopping from rolling resistance alone. It's annoying.
```

---
## \#50 Posted by: SkaterBoy58 Posted at: 2018-06-15T23:12:26.333Z Reads: 121

```
see my post at
http://www.electric-skateboard.builders/t/vesc-brakes-grabbing-coming-to-stop/46946/7

and how i solved it 

Cheers
```

---
## \#51 Posted by: Pedrodemio Posted at: 2018-06-15T23:18:31.195Z Reads: 115

```
For me it doesn’t happen, or if it happen I’m so used that I don’t usually notice

80mm wheels, 14/34 gearing and 190kv 5055

Could it be VESC 6 vs FOCBOX? Since the later has only two shunts? What are you guys running?
```

---
## \#52 Posted by: ervinelin Posted at: 2018-06-15T23:20:35.243Z Reads: 113

```
Could you share your drive setup? E.g. gearing, wheel size, etc?

I noticed you were running FOC, this hack fixed it for FOC as well?

Thanks in advance, really annoying to be kicked off my board.
```

---
## \#53 Posted by: SkaterBoy58 Posted at: 2018-06-15T23:46:36.811Z Reads: 108

```
yeah FOC   with canbus dual 150KV motors 15T motor cog  66T wheel cog  175 wheels
```

---
## \#54 Posted by: ervinelin Posted at: 2018-06-16T00:06:02.492Z Reads: 107

```
Thanks I applied the hack... Will report back once I have some results...

What's your motor and batt min settings?
```

---
## \#55 Posted by: mmaner Posted at: 2018-06-16T00:26:20.149Z Reads: 108

```
I did some testing on a single motor board. 90mm Flywheel, the insta-stop isn't present., 107mm Flywheels insta-stop is there but very minimal. 6in 6 shooters it's def there. 7.5 in most definitely there. Seems it's all related to wheel size vs low end RPM.
```

---
## \#56 Posted by: ervinelin Posted at: 2018-06-16T00:27:56.743Z Reads: 107

```
Exact same setup just changing wheel size?
```

---
## \#57 Posted by: Mathias Posted at: 2018-06-16T00:30:07.681Z Reads: 108

```
[quote="SkaterBoy58, post:50, topic:39136"]
see my post at

> Have you tried to calibrate your remote controller in the VESC Tool?

and how i solved it

Cheers
[/quote]

That looks interesting. Good job on the workaround :+1:. And I really don't get why VESC tool doesn't let you modify this parameter. I posted a feature request on Benjamin's forum:
https://www.vesc-project.com/node/480
Unless there's something that we're missing here why this parameter should not be changed for FOC, it should be a 5 min job for him to add it for the next VESC tool release. It was probably just forgotten in the rewriting of the tool...
```

---
## \#58 Posted by: Eboosted Posted at: 2018-06-16T00:31:59.861Z Reads: 111

```
@SkaterBoy58 This is a great find man!

Thanks a lot for posting the solution, I'll try as soon as I have time later this week. This is exciting!

@Ackmaniac would you please include this into a future FW update?
```

---
## \#59 Posted by: Mathias Posted at: 2018-06-16T00:57:08.253Z Reads: 119

```
[quote="Eboosted, post:58, topic:39136"]
@Ackmaniac would you please include this into a future FW update?
[/quote]

From the way that @SkaterBoy58 was able to fix it seems firmware already has it implemented. It's really just adding the button to VESC tool.
```

---
## \#60 Posted by: Ackmaniac Posted at: 2018-06-16T01:08:18.306Z Reads: 118

```
Has only an effect in BLDC but not in FOC mode. I can try to expose the value. But no time this weekend. Maybe in the next week.
```

---
## \#61 Posted by: mmaner Posted at: 2018-06-16T01:15:35.802Z Reads: 115

```
Yes sir

10c
```

---
## \#62 Posted by: Eboosted Posted at: 2018-06-16T01:37:54.501Z Reads: 113

```
So you mean @SkaterBoy58 solution will not work?
```

---
## \#63 Posted by: ervinelin Posted at: 2018-06-16T02:52:36.878Z Reads: 112

```
He mentioned he is running FOC though...
```

---
## \#64 Posted by: ervinelin Posted at: 2018-06-16T04:43:58.749Z Reads: 108

```
Reporting back... Hack did not work for me.. still jerks when it comes to a complete stop...

Dual 6374 running FOC on 8" wheels...

EDIT: Also, reducing motor/batt mins didn't work either, feels exactly the same
```

---
## \#65 Posted by: Eboosted Posted at: 2018-06-16T05:06:27.614Z Reads: 108

```
Damn that's heart braking
```

---
## \#66 Posted by: Bjork3n Posted at: 2018-06-16T12:50:48.134Z Reads: 106

```
What happens when you change to this? Does the board not come to a complete stop with this setting? I have belt skip at the end of braking when coming to a complete stop. Would be nice if you could disengage the brake when at say 1-2km/h.
```

---
## \#67 Posted by: lrdesigns Posted at: 2018-06-19T01:01:05.198Z Reads: 104

```
It almost comes to a complete stop like 0.5kmh. But keeps rolling at the end. It brakes really hard as normal but as it approaches 0 the breaking force gets less and less, sort of a soft stop. I think my setting is a bit low, a little higher and I think it would stop. I think you have to find a sweet spot for your motors.
```

---
## \#68 Posted by: ervinelin Posted at: 2018-06-19T04:05:58.111Z Reads: 100

```
Which setting are you referring to? The hack from @SkaterBoy58 ?
```

---
## \#69 Posted by: DAddYE Posted at: 2018-07-16T02:04:34.102Z Reads: 95

```
Same here. I’m on a flipsky with 6.6 Vesc and single Turnigy 6376 (https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html)

Weird that has been so long and yet not fixed :frowning:
```

---
## \#70 Posted by: ervinelin Posted at: 2018-07-16T02:32:46.961Z Reads: 95

```
How large wheels?
```

---
## \#71 Posted by: DAddYE Posted at: 2018-07-16T02:34:23.424Z Reads: 95

```
Flywheels 90mm
```

---
## \#72 Posted by: ervinelin Posted at: 2018-07-16T02:40:44.511Z Reads: 94

```
Strange.. I don't notice this on anything but my 8" wheels...
```

---
## \#73 Posted by: mmaner Posted at: 2018-07-16T02:47:04.765Z Reads: 91

```
I switched to current from watt on my gear drive and it's gone, did the same thing in my bludgeon but it didn't change. This is a weird issue.
```

---
## \#74 Posted by: Sender Posted at: 2018-07-16T02:57:18.524Z Reads: 92

```
I feel it still my my sons 6s3p 14/36 83mm single drive.
```

---
## \#75 Posted by: McErono Posted at: 2018-07-16T12:28:48.224Z Reads: 92

```
Dual 6374 foc, ackmaniac 3.102, 97mm flywheels, 16/36, 12s4p,same issue in watt mode.
```

---
## \#76 Posted by: ervinelin Posted at: 2018-09-03T03:47:32.936Z Reads: 84

```
Digging up a buried thread here...

Any resolution to this issue? Really irritated with my 8" AT board which likes to throw me off the board at very low speeds by locking the wheels.

Other speeds it works just fine, just that very last 1km/h it locks the wheels and flicks me off.
```

---
## \#77 Posted by: Eboosted Posted at: 2018-09-03T03:50:44.632Z Reads: 86

```
Nothing has fixed this issue for me even on my Jet Spud with 85mm caguamas I get this locking up.
```

---
## \#78 Posted by: Pedrodemio Posted at: 2018-09-03T04:13:42.705Z Reads: 87

```
I’m temporarily on single drive and also having this problem now

I can lock the wheel at any speed it not all my weight is on the driven wheel. For it to release I need to release the brake completely 

Yesterday I did a nice slide because of this. Was braking with the wheel locked and decided to turn and full traction was gained. I liked it a lot since I’ve never did slide before 🙃
```

---
## \#79 Posted by: ervinelin Posted at: 2018-09-03T05:49:32.536Z Reads: 89

```
That's odd... why are you getting this with 85mm wheels... I thought this was a "big wheel" issue...

Just out of curiosity, is your spud on 12S? Because the only board I have problems with runs on 12S, the rest are on 10S.

I'm just trying to rule out things one by one..
```

---
## \#80 Posted by: Eboosted Posted at: 2018-09-03T05:55:36.757Z Reads: 90

```
Yes, my Spud has 85mm wheels and I'm runing FOC. It's not a wheel size issue.
```

---
## \#81 Posted by: ervinelin Posted at: 2018-09-03T06:55:21.732Z Reads: 90

```
@mmaner did some tests and he said it's more obvious with larger wheels though.

Is your spud on 12S? I run FOC on all my boards, 90mm, 100mm, 200mm... only the 8" has this problem, at least obvious enough for me to get flicked off.

https://www.electric-skateboard.builders/t/wheels-brake-locking-in-foc-right-before-dead-stop/39136/55?u=ervinelin
```

---
## \#82 Posted by: PXSS Posted at: 2018-09-03T13:27:31.499Z Reads: 91

```
Does anyone have a Bluetooth module on board? Posting the data might help resolve the issue. All of my boards are still on 2.54 iirc but I was going to play with 3.x next weekend. Sounds like Im better at this fw
```

---
## \#83 Posted by: Eboosted Posted at: 2018-09-03T21:57:06.147Z Reads: 84

```
Since I upgraded to Oreo bluetooth modules are completely useless
```

---
## \#85 Posted by: Eboosted Posted at: 2018-09-03T22:45:56.798Z Reads: 86

```
Yeah, Metr works better the generic HM-10 modules are the ones affected by Oreo.
```

---
## \#87 Posted by: DAddYE Posted at: 2018-12-11T03:57:10.333Z Reads: 63

```
Did anyone ask Vedder about this? Maybe it’s worth a shot
```

---
## \#88 Posted by: McErono Posted at: 2018-12-13T14:09:56.283Z Reads: 53

```
I have the problem on 12s and 97mm flywheels.
```

---
## \#90 Posted by: McErono Posted at: 2018-12-24T19:37:39.830Z Reads: 38

```
this does somehow help. tried 300 instead of default 900 and it feels completly different!

https://www.electric-skateboard.builders/t/vesc-brakes-grabbing-coming-to-stop/46946/51?u=mcerono
```

---
## \#91 Posted by: VANFORMER Posted at: 2018-12-24T21:24:01.860Z Reads: 34

```
I had similar issues on my current build but got some help from the local DIYers here in Sydney. 
I am running the following
2x 4.12 TB ESC's
2x 6355 190 kv TB motors
BLDC Setup with sensors 

I found changing the input values worked for me.

![15456864462242095665929617895845|666x499](upload://lshc0mw36qVD9vareUYgdNhhSZb.jpeg)
```

---
## \#92 Posted by: ShutterShock Posted at: 2019-01-29T20:48:18.913Z Reads: 26

```
Another forum user directed me to this link.  Haven't gotten to try it yet, but as soon as I have access to my Arduino at home I plan on doing this.  

https://forum.arduino.cc/index.php?topic=393655.0
```

---
