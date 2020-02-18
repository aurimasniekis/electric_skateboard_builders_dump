# Who is using FOC and whats your setup?

### Replies: 161 Views: 13850

## \#1 Posted by: whitepony Posted at: 2016-06-09T07:58:41.798Z Reads: 816

```
huhu! I have just a little experience with FOC - tried it in an early stage with nunchuck control and it was completely weird/undriveable - usually worked well for 200m and then just started acting up. months later I tried again on my trampa in order to silence the dual 6374s ... and just fried a vesc directly after 10min of playing. bottom line: Im now too afraid to try FOC again. but I would love to because of the stealth sound.

I would really like to know if someone is successfully running FOC for at least 100km+ without issues and if so, what setup are you using? **battery specs, motor, VESC HW version and controller!**
```

---
## \#2 Posted by: Haimindo Posted at: 2016-06-09T08:15:29.265Z Reads: 762

```
Have not tried it because too afraid to burn the VESC. I'll wait for VESC 5.0 and new setup to give it a try. I know that @RunPlayBack have succesfully used FOC with the single Carvon V2
```

---
## \#3 Posted by: Maxid Posted at: 2016-06-09T08:31:44.391Z Reads: 758

```
I think @Hummie is using FOC as well and can maybe tell us about his experience.
I am also in the same boat: too afraid of frying a VESC since even the manufacturers like @chaka and @elkick are advising against it.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-06-09T08:44:35.745Z Reads: 744

```
I used FOC with a 6S battery and a SK3 213kv motor. It works flawlessly! When i switched to 12S and the SK3 149kv i did not get it running... I dont know why. Maybe because i have VESC HW4.10 which does not have the better capacitor at C18.
Currently my VESC is broken. I will have it repaired these days and have soldered the new capacitor at C18. Then i will try it again.

Noob question: You will do a motor detection with no load. When configurating FOC i should also do it without any load (wheels)?
```

---
## \#5 Posted by: michaelcpg Posted at: 2016-06-09T09:47:21.060Z Reads: 714

```
Been using FOC for a month or so now. No issues so far. My setup is essentially a Raptor mono with a different deck.
```

---
## \#6 Posted by: whitepony Posted at: 2016-06-09T09:52:12.184Z Reads: 706

```
nice! do the raptors come with foc active or bldc?
```

---
## \#7 Posted by: flatsp0t Posted at: 2016-06-09T09:53:11.670Z Reads: 700

```
BLDC, i think they can not afford taking the risk at the moment.
```

---
## \#8 Posted by: Tarzan Posted at: 2016-06-09T13:49:12.256Z Reads: 700

```
Yes the Raptor comes in BLDC mode.
I don't get the FOC hype. Okay the real hype is over after so many people fried there VESCs, but where are the advantages beside the sound?
I heard the Fets get hotter and for that reason its a no-go for me.
```

---
## \#9 Posted by: treenutter Posted at: 2016-06-09T13:51:30.630Z Reads: 745

```
@whitepony I've been using FOC for a while now, about 100+ miles with it and I love it. My setup is here in my build thread. I added a cap to c18 and that seemed to make things run more smoothly. I have VESC HW version 4.7 so the mod improved performance.I had to tinker with the brake settings and startup to optimize it. I love FOC mode and wouldn't go back. I like the quiet operation and somehow it feels more even during acceleration. Using PPM mode for control also worked much better for me than using the native Nunchuck app.

http://www.electric-skateboard.builders/t/the-village-build-s9-faultine-paris-195mm-sk3-6764-diyes-mount-8s-vesc-127mm-pneumatic-wheels/292
```

---
## \#10 Posted by: RunPlayBack Posted at: 2016-06-09T13:51:45.065Z Reads: 724

```
@whitepony @Haimindo yup I've had FOC enabled on both my single and dual boards with no problems. The only time I've had a problem with FOC was when one of my motor phase wires came loose on my dual build which caused it to brake after a full throttle. I prefer it over BLDC because of the stealth since I'm always riding around the city. With Carvon hubs its nearly silent and I get much better battery life on FOC. Here's a rundown of my setups:

<img src="/uploads/db1493/original/2X/a/aa2331fe5e37c2e5a59e2d1a8935a421b8a8b410.png" width="690" height="388">

Carvon V2 Single Hub + 12s1p LiFePO4 + Ollinboard VESC + Torqueboard 2.4ghz Mini Remote
FOC Enabled
Motor Max: 60.00 A
Motor Min: -60.00 A
Bat Max: 40.00 A
Batt Min: -12.00 A
Absolute Max: 130.00 A
Max ERPM: 60000.00
Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 35.20 V
Battery cut off end: 33.20 V
Startup Boost: 0.040
Soft RPM limit:
ERPM limit start: 0.00
ERPM limit end: 60000.00



Carvon V2 Dual Hub + 10s Enertion Space Cell + Ollinboard VESC's + Torqueboard 2.4ghz Mini Remote
FOC Enabled
Motor Max: 60.00 A
Motor Min: -60.00 A
Bat Max: 15.00 A
Batt Min: -12.00 A
Absolute Max: 130.00 A
Max ERPM: 60000.00
Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 35.20 V
Battery cut off end: 33.20 V
Startup Boost: 0.040
Soft RPM limit
ERPM limit start: 0.00
ERPM limit end: 60000.00<img src="/uploads/db1493/original/2X/9/923ee1178491ad163125a0b2a554967cc0a9900d.jpg" width="690" height="388">
```

---
## \#11 Posted by: whitepony Posted at: 2016-06-09T14:01:19.457Z Reads: 650

```
[quote="Tarzan, post:8, topic:4465"]
but where are the advantages beside the sound?
[/quote]

from what I understand, the foc implementation has higher efficiency and the sound is a big deal for me. first of all it adds to the feeling of riding a regular longboard, but most of all it might just be the reason why a policemen does NOT turn his head :yum:
```

---
## \#12 Posted by: treenutter Posted at: 2016-06-09T14:05:09.523Z Reads: 643

```
@whitepony for easy reference I'm using 2x 4S 5000MAh Lipos in series, Sk3 6764 245KV, VESC HW version 4.7 with modded C18, and modded GT2B.

-if you want to try the C18 mod let me know I can mail you a few of the extra caps I have. (you'll need good magnification they are very tiny!)
```

---
## \#13 Posted by: whitepony Posted at: 2016-06-09T14:11:19.030Z Reads: 632

```
[quote="treenutter, post:9, topic:4465"]
Using PPM mode for control also worked much better for me than using the native Nunchuck app.
[/quote]

nice to see you with a high KV SK6374 - gives me hope that a low KV SK6374 (168KV) with 10S might work too. the first carvons used SK6374 Motors if i remember correctly @RunPlayBack (which kv)? 

I also had the impression, that nunchuck & FOC didnt work out at all, but before I could test it with a PPM device, I fried my vesc. Im receiving a german 4.11 C18 modded vesc hopefully this week - basically the same thing I fried on my trampa after 10minutes. ist really itching to try foc, would be the ultimate holiday boarding experience with the superflexy vanguard and a dead silent motor.
```

---
## \#14 Posted by: whitepony Posted at: 2016-06-09T14:13:51.727Z Reads: 596

```
[quote="treenutter, post:12, topic:4465"]
if you want to try the C18 mod let me know I can mail you a few of the extra caps I have. (you'll need good magnification they are very tiny!)
[/quote]

my 2nd FOC test had the C18 mod already - I nearly died trying to get that stupid little thing piggybacked. :confused:
```

---
## \#15 Posted by: treenutter Posted at: 2016-06-09T14:23:10.757Z Reads: 589

```
[quote="whitepony, post:13, topic:4465"]
I also had the impression, that nunchuck & FOC didnt work out at all
[/quote]

I think that the Nunchuck app for vesc has variable results in terms of throttle resolution. I can't tell if it's because some nyko kama's are duds, or if the app itself can't receive the full range of throttle inputs from the device. In either case, I found it much harder to control throttle with the nunchuck; it seemed like it only sent inputs at a few intervals; 0%-50%-100% throttle.

Once I switched to gt2b everything was steez.

[quote="whitepony, post:14, topic:4465"]
I nearly died trying to get that stupid little thing piggybacked
[/quote]

Haha me too! Now that I have a good jeweler's loupe I can see how crooked the cap is, but it still works!
```

---
## \#16 Posted by: elkick Posted at: 2016-06-09T14:41:53.251Z Reads: 568

```
[quote="whitepony, post:13, topic:4465"]
Im receiving a german 4.11 C18 modded vesc hopefully this week
[/quote]

It's a 4.12 and it has been delivered today. We're currently improving speed of delivery. :slight_smile:
```

---
## \#17 Posted by: elkick Posted at: 2016-06-09T15:06:11.179Z Reads: 570

```
To answer you initial question: I am driving FOC on all boards now, with 4.7, 4.10 and 4.12 VESCs since January. But none of the boards is on 12s (4 on 10s, 2 small cruiser on 7s) and when I switched I didn't switch back and forth again between FOC and BLDC, I just stayed with FOC. Never had any issue at all, I'm riding every day, even in rainy conditions.

Most of the fatal failures I observed when people were using FOC with 12s or have switched between FOC and BLDC, sometimes multiple times.. 

I'm not sure what the reasons for those failures are, but I could imagine that for switching the modes you need to do a "factory reset" on all values in between (installing FW again and/or doing a "read default config")  to make sure to start with a clean environment. But again, that's just a guess. 

With 12s I think the risk in general is higher to have voltage peaks beyond the VESCs capabilities. The latest change Ben made to FW 2.18 might also reduce the risk a little bit. Still, FOC is in development and not yet safe for everybody. That's why I recommend not to use it unless you understand all the values within the FOC tab and are able to manage them manually as well.
```

---
## \#18 Posted by: Hummie Posted at: 2016-06-09T15:10:44.232Z Reads: 546

```
I read the battery wire length is more important on FOC.  I'm on 12s FOC and it's been fine.  Vesc is always cool. I left al the default settings other than what I plugged in after the test.  Ran the bldc test first but almost never ran bldc
```

---
## \#19 Posted by: whitepony Posted at: 2016-06-09T16:03:12.139Z Reads: 555

```
@elkick vesc arrived, lightning fast! yea, indeed, I switched between foc and bldc a few times when I fried mine! :open_mouth:

which motors & controllers are you running?
```

---
## \#20 Posted by: elkick Posted at: 2016-06-09T16:24:17.450Z Reads: 563

```
I am using a various motors at the moment: CarvOns V1 and V2 (SK3-6374/149kv), Johns hubmotors with 80kv and 90kv, our own esk8-6355/200kv and esk8-6374/200kv sensored, chinese no-name (Bubblegum Board, in Kid's mode) 5065/245kv, Alien 5065/270kv sensored (now replaced by our own 6255).

Remotes: Badwolf gt2b mod, Mini-Remote 2.4GHz, Kama Nunchuk, 1x Wii-Nunchuk with wiiceiver, Generic (bechwheel) 2.4Ghz Remote.

Cable length were an issue in the beginning, but staying below 30cm I never had a problem anymore.
```

---
## \#21 Posted by: treenutter Posted at: 2016-06-09T16:29:09.459Z Reads: 528

```
[quote="elkick, post:20, topic:4465"]
staying below 30cm I never had a problem anymore
[/quote]

@elkick where do the measurements for the 30cm begin and end? Is it at the start of the battery cable that leads out of the battery pack, or at the connector?

And where does the measurement end? Is it at the cap PCB of the VESC, or the connection on the main PCB?
```

---
## \#22 Posted by: elkick Posted at: 2016-06-09T16:33:45.546Z Reads: 528

```
It's measured typically between cells and capPCB. But this is just my own observation and is also related to the cable quality, thickness and how they are mounted (putting +/- close together when routing them across the board might be a good idea). I tested it several times, and every time I went beyond a certain length I had issues. 

So I don't know if others were experiencing the same. Normally I am using 12AWG HK silicon wire. And the BMS wiring might not add to the whole calculation, since it's only at the - cable.
```

---
## \#23 Posted by: Hummie Posted at: 2016-06-09T16:46:48.735Z Reads: 510

```
If the wires are too long or building the inductance somehow and messing the FOC up....adding caps is a solution right?  
Thicker wires with the the red and black as close as possible as was said is a good start.
```

---
## \#24 Posted by: RunPlayBack Posted at: 2016-06-09T17:25:19.339Z Reads: 495

```
I'm on Carvon V2 like @elkick 149kv. On my 12s1p LiFePO4 I set my bat max to a conservative 40A even though it's rated for 60A. Switched between FOC and BLDC a few times with no errors. I'm also on PPM with the 2.4ghz Mini Remote.
```

---
## \#25 Posted by: Hummie Posted at: 2016-06-09T17:48:05.824Z Reads: 495

```
With the lifepo4 at 3.6 volts for a full charge why not do ...16s?
```

---
## \#26 Posted by: RunPlayBack Posted at: 2016-06-09T18:02:19.159Z Reads: 490

```
I have it on a really small deck, 29" kicktail with roughly 13.5" wheelbase so real estate is kind of sparse at the moment. Mostly it using on very short, flat distances in the city.
```

---
## \#27 Posted by: whitepony Posted at: 2016-06-09T20:56:12.957Z Reads: 492

```
ah well, couldnt help it and set the new vesc up with foc. on the bench it works well, but I have weird behaviour Id like to ask you guys about: Im using ppm current control no reverse with brake, motor sk6374 -> if I go slight throttle the motor will spin up full -> small torque, no load -> full RPM, check! 

now I increase the throttle until max and what happens is the motor is becoming slightly slower (from 41000 ERPM down to 39000 ERPM and the real time data plot shows actually negative power and that its recuperating with about -2A battery current and about -75Watt power. huh?

I highly doubt that :p anyone know whats going on?
```

---
## \#28 Posted by: treenutter Posted at: 2016-06-09T20:59:59.776Z Reads: 481

```
@whitepony I have always found that FOC mode behaves differently than BDLC mode when it's on the bench, and that seems to be true for startup as well as when I try to move through the RPM range. 

I'm sure someone who understands it better could explain why this is, but it's definitely a pattern I've noticed with FOC mode (but it doesn't seem to impact things when I'm actually riding).

I really like @elkick's advice to start configuring FOC from a fresh firmware install, that way no lingering values are impacting your config.
```

---
## \#29 Posted by: treenutter Posted at: 2016-06-09T21:03:03.375Z Reads: 472

```
@elkick thanks! That's really helpful; I might have to reduce the length of some of my cables... I've for a battery arming switch that is adding a lot of length.
```

---
## \#30 Posted by: hexakopter Posted at: 2016-06-09T21:07:39.052Z Reads: 461

```
I think the point with the max erpm is correct. I have read somewhere, that the max erpm is slightly lower in FOC mode than in BLDC mode.
```

---
## \#31 Posted by: whitepony Posted at: 2016-06-09T21:20:07.860Z Reads: 462

```
[quote="hexakopter, post:30, topic:4465, full:true"]
I think the point with the max erpm is correct. I have read somewhere, that the max erpm is slightly lower in FOC mode than in BLDC mode.
[/quote]

i didnt compare BLDC with foc though - what I had was less ERPM at max compared to min throttle without load on the benchtest with negative power consumption. its just weird behavior that I dont understand. :confused:
```

---
## \#32 Posted by: Jinra Posted at: 2016-06-09T21:22:57.038Z Reads: 443

```
do you get the same behavior when throttling to 80-90% of max?
```

---
## \#33 Posted by: Bender Posted at: 2016-06-09T21:23:02.903Z Reads: 448

```
Sounds like what happens when the voltage limit is hit
I've never had that happen on the bench with FOC 
I'm using a Kama 
But I did feel it riding once when my voltage limit was hit
```

---
## \#34 Posted by: whitepony Posted at: 2016-06-09T21:27:06.459Z Reads: 446

```
[quote="Jinra, post:32, topic:4465, full:true"]
do you get the same behavior when throttling to 80-90% of max?
[/quote]

if i go min throttle the motor starts running slowly, the motors own friction is enough that it doesnt hit ERPM max. so if i increase the throttle further, the motor will eventually run into max ERPM very soon with about 50-75Watt power consumption.

from there, increasing throttle will slowly decrease ERPM and decrease power consumption/battery current until the numbers all become negative eventually. this continues until max throttle!
```

---
## \#35 Posted by: NNGG Posted at: 2016-06-10T03:27:50.088Z Reads: 428

```
is the difference between bldc and foc just noise and start up?
```

---
## \#36 Posted by: DeathCookies Posted at: 2016-06-10T11:43:36.715Z Reads: 424

```
And efficiency
```

---
## \#37 Posted by: Hummie Posted at: 2016-06-10T15:27:11.973Z Reads: 426

```
And smoothness
```

---
## \#38 Posted by: RunPlayBack Posted at: 2016-06-10T15:31:07.039Z Reads: 430

```
and ninja-ness
```

---
## \#39 Posted by: whitepony Posted at: 2016-06-10T22:24:57.794Z Reads: 446

```
first 20km maidens ride on my vanguard and FOC was really really awesome, so glad I tried again!!

speccs: VESC HW4.12, software 2.18, motor sk3 6374 168KV, remote 2.4Ghz torqueboard remote!

control ppm, current no reverse with brakes!


highfive @elkick, nice vesc!! :grinning:
```

---
## \#40 Posted by: Hummie Posted at: 2016-06-10T22:42:40.133Z Reads: 448

```
Nice!  Nice to see other people appreciating it's awesomeness. so nice.
```

---
## \#41 Posted by: Jinra Posted at: 2016-06-10T22:43:28.118Z Reads: 440

```
Now I want to try FOC, but i'd be so sad to blow a $170 VESC :fearful:
```

---
## \#42 Posted by: E-Boarding Posted at: 2016-06-11T06:49:15.603Z Reads: 435

```
I wan't to use FOC too but what happens to the VESC when it fries, is it completly destroyed, repairable, what the fuck happens there?
```

---
## \#43 Posted by: Jinra Posted at: 2016-06-11T06:55:43.898Z Reads: 425

```
Usually DRV chip fries
```

---
## \#44 Posted by: Hummie Posted at: 2016-06-11T06:58:50.444Z Reads: 424

```
If u know what ur doing, I don't, u can repair them and it seems not too hard. It's worth the risk.  I don't hear of many people having problems
```

---
## \#45 Posted by: whitepony Posted at: 2016-06-11T09:50:31.678Z Reads: 433

```
gave it another spin and Im really so happy with FOC right now. it feels smoother than BLDC and the silence, especially at startup and low speed is giving the whole board a very natural raw manual longboard feel. like eating something that looks delicious - it just adds to the experience.

couldnt be happier right now, first thing I do when my vanguard is finally finished: update my tesseract c18 modded vesc with 2.18 fresh and set up foc! :heart_eyes:

must say, I always had trouble with nunchuck & FOC combo, so it always left a sour taste whenever I tried foc in the past. now with the 2.4Ghz mini remote, its all working just perfect.
```

---
## \#46 Posted by: Haimindo Posted at: 2016-06-11T10:23:43.719Z Reads: 419

```
Now I want to use FOC too :open_mouth:
```

---
## \#47 Posted by: Bender Posted at: 2016-06-11T15:30:48.817Z Reads: 414

```
Did you ever figure out the bench throttling issue?
```

---
## \#48 Posted by: whitepony Posted at: 2016-06-11T20:28:06.854Z Reads: 427

```
nope, its still like that - I stopped worrying after it ran fine on the road.

rew, one of the vedder.se experts, commented on it though: 

_when you run unloaded, and have "current control" mode, whether you set 10% max current or 99% of max current the motor should spin up to its maximum RPM and then the VESC should see "max PWM reached" and reduce the internal setpoint until things stabilize._

_Your observations indicate that with a bigger current-setpoint the behaviour of the limiting is slightly different. I wouldn't worry about it. If 10% throttle reaches "max RPM" then something is already wrong... (you need a higher battery voltage, a higher Kv motor, or the load has gone missing(*).)_
```

---
## \#49 Posted by: DeathCookies Posted at: 2016-06-12T09:46:03.146Z Reads: 448

```
I currently run FOC with my repaired VESC 4.10 on 12S with SK3 149kv Motor and have no problems at all. If i get problems i will Report back. But now i can drive from stand still with no cogging and "ninja mode". It is just awesome!
```

---
## \#50 Posted by: whitepony Posted at: 2016-06-12T13:21:27.312Z Reads: 455

```
today I did a max range check on my board and I was actually disappointed. for now I would call the "efficiency" of FOC vs. BLDC pretty much a marginal effect or myth. of course there are more factors than the commutation mode involved - I got the same battery, same wheels, same bearings with a different motor and FOC vs. BLDC. my tesseract with BLDC and 190KV 6355 rspecc managed 39km max range while the vanguard with SK6374 and FOC managed 32km. I rode it hard, carved until the wheels slipped, but thats pretty much what I did with the tesseract too. :no_mouth:

ah well, Ill figure it out - next is a max range check with BLDC I think to rule out the commutation mode.

made a quick video of 50A accelerating and -16A braking of the SK6374 with my german FOC vesc. its interesting, cause its only really ninja-silent when its slow and from mid-speed onwards to the max its nearly as loud as bldc. not sure if its simply the sound the motor makes or if the sound can be attributed to the driving ESC?

and no, I didnt fart in the end :joy:
https://www.youtube.com/watch?v=d5_aHvrR85U
```

---
## \#51 Posted by: squad Posted at: 2016-06-12T13:34:43.205Z Reads: 447

```
[quote="whitepony, post:50, topic:4465"]
its interesting, cause its only really ninja-silent when its slow and from mid-speed onwards to the max its nearly as loud as bldc.
[/quote]


Observed the same thing, when I played with FOC for one day and then while switching back to BLDC it fu**ed up two of my VESCs. Silent when going slow, but as loud as BLDC near top speed, which is noticeably slower tho.
```

---
## \#52 Posted by: whitepony Posted at: 2016-06-12T13:40:50.207Z Reads: 430

```
yea, think elkick has established that switching between FOC and BLDC is probably not a good idea. when I try BLDC with this setup, Ill flash the firmware 2.18 again to have a factory new VESC.  :relaxed:
```

---
## \#53 Posted by: RunPlayBack Posted at: 2016-06-12T16:01:55.692Z Reads: 424

```
I'm still unsure if switching between FOC and BLDC causes problems as I've been doing that at least 2-3 times a month since January on both single and dual @chaka VESCs. FOC Ninja silence from startup to top speed is constant on hub motors and "feels" more efficient although I don't have numbers to back that up. For the amount of time I've spent riding on both settings, that "natural" feeling FOC gives is hard to turn down. It may be that FOC is best suited for hubs and BLDC for belt drives. Maybe someone who has both setups can provide some data.
```

---
## \#54 Posted by: Jinra Posted at: 2016-06-12T19:13:20.053Z Reads: 417

```
Does FOC provide a natural feel even for sensored motor setups? I suspect the failures switching between FOC and BLDC are due to legacy settings that haven't been reset from the previous mode. I wonder if re flashing the firmware would prevent these issues.
```

---
## \#55 Posted by: Ulfberht Posted at: 2016-06-12T19:25:53.707Z Reads: 420

```
[quote="whitepony, post:52, topic:4465"]
when I try BLDC with this setup, Ill flash the firmware 2.18 again to have a factory new VESC.
[/quote]

NIce tip! Thanks!
```

---
## \#56 Posted by: Hummie Posted at: 2016-06-14T14:30:59.378Z Reads: 422

```
It's not a FOC specific question because I hear that you can put the same amount of current to the motor with bldc but what motor current are you running the vesc at?  I'm at 60 and read 50 is the max endorsed safe current but people are doing up to 90.  If ever there was an important variable on the vesc in terms of putting out power and protecting the motor and vesc this seems the one
```

---
## \#57 Posted by: whitepony Posted at: 2016-06-14T14:39:59.790Z Reads: 414

```
I got all currents to specifications, i.e. 6374 168KV @ 70A and vesc battery current max at 50A. didnt feel like blowing stuff up again! :stuck_out_tongue_winking_eye:
```

---
## \#58 Posted by: Hummie Posted at: 2016-06-14T15:29:26.771Z Reads: 414

```
Ok 70 to the motor.  I hear the other side from the battery isn't a concern except to protect the battery.   Where'd you come up with the 70 number?  
Do u have it heatsinked or kept cool somehow?  Does it get hot?  I don't want to blow stuff up either!  Did u fix it or get another?
```

---
## \#59 Posted by: whitepony Posted at: 2016-06-14T18:25:05.271Z Reads: 403

```
70A is just the sk3 6374 168KV specifications!
```

---
## \#60 Posted by: Hummie Posted at: 2016-06-14T18:36:09.305Z Reads: 406

```
I'm mor worried about the esc and trying to find if the amp limit is solely heat related.  Guy on vedders site does 90 limit but Rew the vesc expert says 50 recommended.
```

---
## \#61 Posted by: KMeyerson Posted at: 2016-06-14T22:29:04.206Z Reads: 403

```
I second this.

You'll want a heat sink if you're actually pulling any serious amperage through the VESC.

I have been using FOC only on my modified Yuneec board (19.5Amp, -20Amp).  The wires are super short here and very well insulated so its been a great settings test board. 

I've found that if I go full throttle 10s on BLDC I can draw as much as 60Amps but the board was both loud and would shut down from heat. Same voltage on FOC maxes out at 20Amps because the motor would stutter at full throttle (because FOC measures current and high currents seem to be more difficult for it to process) which is why I set my max at 19.5Amps (regen is still safe at -20Amps).  Before I go further, I originally thought my board was disconnecting due to a bad connection when riding, but I rode with a bluetooth chip instead of the Nyko Kama and found that the problem was heat buildup. I'm sending my VESC back to Chaka for a heatsink and clean up this week.

If heat build up still prevents me from riding full throttle every 45 minutes, leaving me stranded for 5-10 minutes as I cool down I'll let y'all know. I look forward to VESC 5.0.


Edit: SENSORLESS FOC
```

---
## \#62 Posted by: Hummie Posted at: 2016-06-15T00:13:48.816Z Reads: 395

```
 on FOC I have no problem sitting on full throttle.  Going up hills it showed 45 or 50 amps from the battery.  Have the limits set to 60 battery 60 motor and I'm hitting the esc to motor amp limit.

Higher voltage runs the vesc cooler.  Not the motor though
```

---
## \#63 Posted by: Alex Posted at: 2016-06-16T17:46:56.510Z Reads: 395

```
that makes sense considering max watt is around 2200 for vesc
```

---
## \#64 Posted by: Maxid Posted at: 2016-06-21T10:51:19.139Z Reads: 385

```
@whitepony just saw on endless that you killed your VESC again. What happened?
```

---
## \#65 Posted by: whitepony Posted at: 2016-06-21T11:24:41.277Z Reads: 379

```
just riding with average load, I dont really know what happened, didnt test motor yet cause I dont have a spare vesc. :'(

I sent it to repair and will go back BLDC once ist back in my hands. screw low speed silence ... :angry:
```

---
## \#66 Posted by: Hummie Posted at: 2016-06-21T11:29:05.458Z Reads: 377

```
 Wish we could find out what's happened.  U have such bad experiences with FOC maybe it's the motor or something else or ur settings.  Were u fully charged or do u have screen shots of ur settings?
```

---
## \#67 Posted by: whitepony Posted at: 2016-06-21T11:32:36.446Z Reads: 369

```
autodetect motor parameters, sanity check values with physics phd, motor ran fine for 350km, you saw the video! 100% sure I did nothing wrong and in fact I set the max currents quite defensively with 50A max battery and 70A max motor current.
```

---
## \#68 Posted by: Hummie Posted at: 2016-06-21T11:36:36.471Z Reads: 371

```
Did it get hot? Was it encased?  Did u check right away?  Anything look blown?  70 to the motor is high according to some
```

---
## \#69 Posted by: whitepony Posted at: 2016-06-21T11:43:56.797Z Reads: 361

```
it wasnt cold, but also not burning hot (hand on enclosure under vesc), so far the 80->100°C soft off in my tesseract is working well since quite a lot of battery chanrges. when the vanguard vesc broke it was also just under medium load at best. :confused:
```

---
## \#70 Posted by: Jinra Posted at: 2016-06-21T15:17:05.825Z Reads: 363

```
who's VESC were you running?
```

---
## \#71 Posted by: Maxid Posted at: 2016-06-22T09:51:35.667Z Reads: 356

```
How much is a DRV replacement in Europe? I want to figure out if its worth a shot to try FOC when my enertion vescs arrive.
```

---
## \#72 Posted by: DeathCookies Posted at: 2016-06-22T10:00:18.092Z Reads: 356

```
About 50€ by the guy in germany, dortmund who helped vedder a lot! Nice costumer service and professional work.
```

---
## \#73 Posted by: Justin Posted at: 2016-06-22T20:46:35.262Z Reads: 351

```
I'm in the process of finishing up my board and looking to for info to configure my board, i'm really interested in FOC-mode because of ninja-stealth (want to be riding low-key). But i was wondering, if you ride dual VESC and it blows, does it blow both of the VESCs? Or is the issue so unknown that its hard to say?
```

---
## \#74 Posted by: Freeflyer Posted at: 2016-06-24T13:02:23.203Z Reads: 351

```
Just switched to FOC mode and really enjoying it.  Almost no cogging from a standstill and seems to have a bit more torque.  But, oh the silence! Its great!.  Running DIY 12s pack through Ollin VESCs (version 4.11 and fw 2.18) and dual Carvon V2 hubs. I flashed the newest firmware to the VESCs (2.18) then followed the usual FOC setup and its working just fine.  Fingers crossed....
```

---
## \#75 Posted by: TheWrongHombre Posted at: 2016-06-24T14:35:33.092Z Reads: 354

```
Welcome to the FOC club @Freeflyer!

I have almost the exact same setup as you.  The only difference is that I haven't flashed to firmware 2.18.  I'm still on 2.17.
```

---
## \#76 Posted by: whitepony Posted at: 2016-06-25T14:05:36.002Z Reads: 356

```
repaired vesc is back, 60€ for a changed drv8302. running bldc again now, tired of killing vescs. currently charging battery on my vanguard for an afternoon run. in the meantime I was riding my tesseract with bldc a lot again - at intermediate to topspeed I must say that bldc is more silent than foc, no idea why but thats how it is.
```

---
## \#77 Posted by: whitepony Posted at: 2016-06-26T19:18:45.167Z Reads: 384

```
gave it a max range tour in BLDC mode, hit 44km and wasnt even in the sub 32V soft off region of my vesc settings. in FOC mode, my battery died at 32km and that was me basically pushing the last 2km in the soft off 30-32V region. :confused:

was going cruise tempo around 23kph average, wide swings so I wouldnt brake too much while carving. the average of the first screenie is off cause I visited my mum in the hospital and didnt switch off the gps thing.
<img src="/uploads/db1493/original/2X/3/3549bb1cb3d2175d136fd3a89d22671308f08863.jpg" width="281" height="500">

the split list shows that quite well:
<img src="/uploads/db1493/original/2X/b/baad8c6a81198bf8517514462567bc3008d8831b.jpg" width="281" height="500">

final battery voltage, just a fraction above the upper battery limit, so I probably couldve cruised another 2km before I had to push the board:
<img src="/uploads/db1493/original/2X/1/1870cf0b81b64726616b797e47f5d3fb9561973f.jpg" width="483" height="500">
```

---
## \#78 Posted by: Hummie Posted at: 2016-06-26T19:27:56.447Z Reads: 359

```
thats counter intuitive.  I thought foc was more efficient.  so it's said.  I'll have to do some testing myself. 42 vs 32km???! that's awful.   were things hot?
```

---
## \#79 Posted by: whitepony Posted at: 2016-06-26T19:34:42.208Z Reads: 367

```
[quote="Hummie, post:78, topic:4465, full:true"]
thats counter intuitive.  I thought foc was more efficient.  so it's said.  I'll have to do some testing myself. 42 vs 32km???! that's awful.   were things hot?
[/quote]

more like 46 vs 32km if you factor in soft off vs. above soft off! I certainly lack statistics - its basically just 2000km+ old 10S4P tesseract bldc cruising tour (40km in softoff) vs. brandnew 10S4P vanguard bldc cruising tour (44km +2km easily before softoff) vs. vanguard foc testing (32km in softoff), the latter on perfect pavement at admittedly slightly larger average speed and harder carving. the others were pure cruise tours on various pavement with more slopes too. otherwise, temperatures were pretty much the same.

would be interesting to see other peoples experience with these 2 modes. I always got a hard time testing that kind of stuff, because I just cant go 20ish kph without carving for 2 hours. :stuck_out_tongue:
 
I rarely hit the battery limit otherwise cause my usual tours are in the 2Xish km regions.
```

---
## \#80 Posted by: lox897 Posted at: 2016-06-27T00:37:58.995Z Reads: 349

```
That is good range. Interesting that FOC isn't more efficient after all. Hope your mum gets better soon!
```

---
## \#81 Posted by: whitepony Posted at: 2016-06-27T04:06:40.835Z Reads: 350

```
its easy to jump to that conclusion, but my rides werent too similar, at least from a carving pov. might have had a much bigger impact than expected! also, maybe motor parameters were not ok or so. ill never be able to test thoroughly though because i wont try foc anymore.
```

---
## \#82 Posted by: whitepony Posted at: 2016-06-27T04:22:57.050Z Reads: 347

```
nice reply on vedder.se: http://vedder.se/forums/viewtopic.php?f=5&t=254#p1623

i shouldve crunched the numbers before jumping to "gut" conclusions! :neutral_face:
```

---
## \#83 Posted by: Hummie Posted at: 2016-06-27T04:45:51.123Z Reads: 349

```
Wow leave it to someone on Vedder's site to figure it out!! Talk about crunching numbers...id have chalked it up to the same maybe but with no math.  One day I'll do a test to see how far I can get on the big bike track here.
```

---
## \#84 Posted by: Bender Posted at: 2016-06-27T12:14:56.082Z Reads: 342

```
That is a fascinating post
So it seems there should be a formula to figure out the best speed for efficency 
Given a particular  are set-up
Seems that 4kmh difference was huge
```

---
## \#85 Posted by: Hummie Posted at: 2016-06-27T16:55:41.480Z Reads: 336

```
I just glanced at the reply in Vedder's site and I'm interested to try to read it but I doubt u can quantify the wind resistance of higher speeds and it's also a huge influence.  It's so easy to change the frontal area by simply bending forward or crouching. I've laid (or lain) on my board going downhill, unpowered, and I can get way farther
```

---
## \#86 Posted by: whitepony Posted at: 2016-06-28T07:40:16.953Z Reads: 345

```
hmmm, interesting - yesterday I made my longer commute trip to and from work and that one has a long semisteep rise, maybe 10%, but over 1km or so. first time I ran that rise with FOC and my new 168KV 6374 motor, the vesc didnt get hot enough so that it would go into soft off strategy after 80°C (which my tesseract always did with 190kv motor). now, with BLDC instead of FOC, the setup got so hot again that the vesc powered down after 80°C.

it seems that in the exact same setup, with the exact same speed uphill, FOC mode ran the vesc cooler than bldc? speaks for a better efficiency of foc. gah, why does it keep killing my vescs :weary:
```

---
## \#87 Posted by: Jinra Posted at: 2016-06-28T14:12:56.152Z Reads: 336

```
i remember reading on vedders site that he needed an extra cap on c18 to prevent errors, though I'm not sure it was the error as yours.
```

---
## \#88 Posted by: Randyc1 Posted at: 2016-06-28T14:48:13.982Z Reads: 340

```
Have you read this, maybe it can help explain ?
 http://www.electric-skateboard.builders/t/the-difference-between-motors-commutation-bldc-vs-foc-trapeziodal-sinosuidal/3002?source_topic_id=419

Seems to say FOC will have less speed ,..but more torque,
```

---
## \#89 Posted by: Hummie Posted at: 2016-06-28T17:31:35.325Z Reads: 346

```
But why are some people blowing chips?  That's the question that doesn't have an answer Randy.  When it works it's great till it's not working.  I'm still going!
```

---
## \#90 Posted by: elkick Posted at: 2016-06-28T18:09:54.136Z Reads: 341

```
Hummiemotors are safe with FOC. :slight_smile:
```

---
## \#91 Posted by: whitepony Posted at: 2016-06-30T20:51:38.940Z Reads: 348

```
call me crazy, but tonight I flashed back to FOC to test the max range again once more. for testing I gave it the beans - full throttle for 20min straight pretty much, including the long 1km 10% rise where BLDC mode usually powers down from overheating. FOC really just pulls up there, no powering down, nothing. impressive :open_mouth:

fingers crossed that this time everything works out - overall FOC rides more enjoyable, against my first impressions its even at mid and highspeed more silent than bldc. basically same motor basis sound, but no high pitched BLDC hum.
```

---
## \#92 Posted by: Jinra Posted at: 2016-06-30T20:53:14.480Z Reads: 339

```
Didn't you say in an earlier post that BLDC was the same loudness as FOC at high speeds?
```

---
## \#93 Posted by: whitepony Posted at: 2016-06-30T20:55:05.396Z Reads: 338

```
well, the motor sound itself is quite loud, in bldc and foc. but the high pitched bldc sound adds ontop of that - more pronounced at low, less audible at intermediate to high speeds, at least for my old ears :stuck_out_tongue:
```

---
## \#94 Posted by: Jinra Posted at: 2016-06-30T20:56:44.354Z Reads: 340

```
I'm surprised you decided to go back to FOC considering your luck with it so far. Hope you don't blow another drv! What VESC are you using btw?
```

---
## \#95 Posted by: whitepony Posted at: 2016-06-30T20:59:08.254Z Reads: 340

```
got 2 backup vescs from my trampa right now - just learnt that the guy who bought it wont pick it up for another 3 weeks :grin:
```

---
## \#96 Posted by: Randyc1 Posted at: 2016-06-30T20:59:08.586Z Reads: 333

```
Does this seem to correspond to the linked article ?  ..Less speed more torque?
```

---
## \#97 Posted by: whitepony Posted at: 2016-06-30T21:03:54.429Z Reads: 332

```
I had less speed than bldc yea, 43kph bldc, 41kph foc on flat straights!

torque is hard to tell, its very similar and hard to be objective when the low speed sound is so different. foc feels very solid and nothing can be heard, bldc hums like an angry bee so it feels more agressive but it certainly isnt. got a fairly steep rise in front of my house and both modes have a hard time getting the board up to speed with 50A battery, 70A motor current max setting.

2 reasons I want foc: temperature most of all since vesc shares the enclosure with my liion cells, and sound is just more pleasant, especially low speed. I came across 2 police patrols this commute week and had a hard time silencing the board with bldc so I wouldnt turn heads (had to reduce speed quick to pretend pushing). :yum:
```

---
## \#98 Posted by: whitepony Posted at: 2016-06-30T21:14:07.211Z Reads: 330

```
now for the this time in FOC motor parameter recognition, I removed the belt to allow the motor to spin freely. it might be something thats just in my head, but it feels the motor runs better, even smoother than first time foc. startup is much better for example. first time foc parameter recognition, the motor had a hard time starting up on its own for the bench test - now it starts really smooth without any hesitation.

could also be the silicone wire mod, which I did without re-doing the FOC parameters - maybe the resistance changed and the motor parameters actually werent ideal?
```

---
## \#99 Posted by: Bender Posted at: 2016-07-01T01:38:34.319Z Reads: 327

```
if you have a chance check out the live ERPM curve in the BLDC tool and compare FOC to BLDC its amazing how smooth FOC is literally, 
and how jagged BLDC is. I have to image that that smoothness is better for the system all around. BLDC is hundreds of little spikes.
```

---
## \#100 Posted by: whitepony Posted at: 2016-07-01T11:12:38.716Z Reads: 353

```
ran another max tour with foc this time: 48km with an estimated average of 23kph, down to 30V and I had to push the last 400m :yum:

also managed a new top speed of nearly 44kph, but that was admittedly slightly downhill. :stuck_out_tongue_winking_eye:

sadly got a severe case of roadrash which explains the "break" in the split table ... ran off the road to get to a bike lane with nearly full speed downhill and the connecting 3meters were pretty much behind a bush, so i couldnt see that it was gravel instead of good old concrete ARGH. :dizzy_face:

<img src="/uploads/db1493/original/2X/4/479e921a4350086154efc96b97542d342f387a42.PNG" width="281" height="500">

<img src="/uploads/db1493/original/2X/0/04cc87e4880d173b3749f1a2bdba14d843ca019e.PNG" width="281" height="500">
```

---
## \#101 Posted by: Ackmaniac Posted at: 2016-07-01T19:03:55.414Z Reads: 321

```
Maybe i found the reson for the blown up VESC's when you switch from BLDC to FOC. In the motor configurations advance tab there is the window for Max current ramp step (at 1kHz).
This value increases by the factor 10 when you press the read configuration button. Wehn you write that value and read it again then it increases again by the factor of 10. In my case it was at **50000**. Default is **0,04**.
**That is a bug in the BLDC Tool 2.18.**

So it is very easy to bring this value up to 50000 by accident. I don't know exactly which impact this value has, but from 0,04 to 50000 doesn't sound healthy.
```

---
## \#102 Posted by: elkick Posted at: 2016-07-01T20:37:08.433Z Reads: 321

```
It has been corrected in github at 27th June, so if you want to upload the newer FW 2.18 you need just to recompile it. 

I'll upload it this evening on my website.
```

---
## \#103 Posted by: Ackmaniac Posted at: 2016-07-01T20:43:23.188Z Reads: 324

```
Currently i am using the windows version. But i will switch to linux. Thanks for the info.
```

---
## \#104 Posted by: Nordle Posted at: 2016-07-21T22:10:58.833Z Reads: 315

```
Now after i finally got my new vesc's, i could finally try FOC.
I like it much, but i have a small lack of torque now. Are there any settings like the ''startup boost'' in BLDC mode was?
```

---
## \#105 Posted by: mason Posted at: 2016-08-08T01:53:22.137Z Reads: 296

```
Did you ever try this again? I'm looking into using FOC with my 12s 149kv 14/36 setup
```

---
## \#106 Posted by: DeathCookies Posted at: 2016-08-08T06:11:46.760Z Reads: 303

```
I did test it... it was as good as earlier. I did not feel any difference but it was stable. Due some time...
(I started and drove about 10 meters and after that nothing more....the VESC did not throw any fault and did not react too....Have to investigate...)

But the FOC detection worked much better and first try with C18!
```

---
## \#107 Posted by: whitepony Posted at: 2016-08-08T07:18:10.497Z Reads: 304

```
after my repaired vesc Im running FOC since about 1000km now without any issues! not sure why it had to break first, but ist fine now! :relaxed:
```

---
## \#108 Posted by: fertito Posted at: 2016-08-08T12:37:23.731Z Reads: 313

```
Hello,
I tested it for some time (nearly 200km) with a 4.12 2.16 firmware version and everything was working fine on flat.
I broke a DRV8302 while breaking downhill, my regen was -20A which was not that much I thought...
Now I'm using BLDC on every board, don't want to spend my time unsoldering DRV8302...
```

---
## \#109 Posted by: kampfhahn Posted at: 2016-09-12T11:32:33.288Z Reads: 297

```
@whitepony

Still everything ok with FOC so far?
```

---
## \#110 Posted by: whitepony Posted at: 2016-09-12T11:46:34.966Z Reads: 301

```
yea :sunglasses:
```

---
## \#111 Posted by: Jinra Posted at: 2016-09-12T11:50:37.865Z Reads: 295

```
What was different about this time but vs previous times where it busted your VESC?
```

---
## \#112 Posted by: whitepony Posted at: 2016-09-12T12:09:41.877Z Reads: 297

```
i really dont know! only difference right now is the 6355 alien motor instead of sk6374, so other motor detection params.
```

---
## \#113 Posted by: kampfhahn Posted at: 2016-09-12T12:12:55.241Z Reads: 306

```
6355 alien sounds great, it´s the same that i use :grin:. Maybe i should give FOC a try. I really want to experience the smoothness compared to BLDC.
```

---
## \#114 Posted by: Hummie Posted at: 2016-09-12T16:07:51.247Z Reads: 299

```
and same length battery wires?  everything exactly the same just the motor difference?  the new vesc is said to be better for bigger motors..maybe that was the problem.
```

---
## \#115 Posted by: whitepony Posted at: 2016-09-13T11:03:26.163Z Reads: 292

```
everything exactly the same, I really dont know why it failed in the first place. actually Im extremely careful with all these small details - all my battery wires are cut to custom length and soldered directly to be a perfect fit. wire thickness is always larger than necessary (10AWG) for smaller impedance and minimum losses. receiver cables are also as short as possible and far away from high current wires, same with the antenna. both fixated with tape to never really rattle around and/or come near the high currents.
```

---
## \#116 Posted by: Jinra Posted at: 2016-09-13T11:19:35.686Z Reads: 296

```
I'm guessing maybe because your smaller motor draws less current than the 6374? Just throwing a shot in the dark.
```

---
## \#117 Posted by: CRABOLSKY Posted at: 2016-09-14T12:00:17.652Z Reads: 289

```
I sure hope not, because when I (finally) get my replacement VESC from Enertion I'll be running FOC on my Enertion 6374
```

---
## \#118 Posted by: Jinra Posted at: 2016-09-14T12:02:15.528Z Reads: 287

```
maybe you'll be fine. FOC just sounds like a lottery to me, which is why i won't be using it until version 6 hits, assuming it works better on it.
```

---
## \#119 Posted by: CRABOLSKY Posted at: 2016-09-14T12:07:02.123Z Reads: 284

```
Yeah man I get it. My plan is to follow @whitepony settings to the letter to increase my chances. Honestly I just preferred the whole experience over BLDC by a good amount. More torque, my enjoyable acceleration and it just sounded nicer.
```

---
## \#120 Posted by: Jinra Posted at: 2016-09-14T12:08:14.263Z Reads: 287

```
Hope your drv survives :)
```

---
## \#121 Posted by: DeathCookies Posted at: 2016-09-14T12:40:58.370Z Reads: 291

```
[quote="CRABOLSKY, post:119, topic:4465"]
it just sounded nicer.
[/quote]

In low rpm it sounds quiter but at high rpm FOC is louder than BLDC...
```

---
## \#122 Posted by: CRABOLSKY Posted at: 2016-09-14T12:45:21.345Z Reads: 292

```
Mmmm I had read that in another thread. I haven't gone above 25-30kph yet. Decisions to be made before I get my next VESC.
```

---
## \#123 Posted by: Mrmoonlight Posted at: 2016-09-14T13:49:06.230Z Reads: 300

```
My setup is dead silent on FOC at higher speeds. I'm also riding hubs, so that might make some difference.
```

---
## \#124 Posted by: JTAG Posted at: 2016-09-14T14:10:56.308Z Reads: 314

```
We have 6 boards (some single a few dual drive) driving around now. all VESC's with FOC running on 6S. We never had a single accident / weird behavior / DRV errors. We even had moments that the capacitor leads broke and we where driving without any input caps.
```

---
## \#125 Posted by: CRABOLSKY Posted at: 2016-09-20T12:52:33.550Z Reads: 275

```
Well it's do or die time... my replacement VESC arrived from Enertion. FOC please do right by me! Interestingly it's come wrapped in solid black shrink and back to the 3 cap version. 

<img src="/uploads/db1493/original/3X/2/d/2d76c8da3f9c91f67fcc5bc444bcf8953a7003e6.JPG" width="666" height="500">
```

---
## \#126 Posted by: Jorge351c Posted at: 2016-09-20T16:56:19.896Z Reads: 266

```
I just built my first board... bought everything from diyelectricskateboard. have a 6374 230kv, 13t/36t pulley setup, 3 zippy 3S 5000mAh batteries in series(9S), controlled through a wii nunchuck. I had it all running okay in BLDC mode for a couple days. I noticed the board would cut out for a second on hard acceleration so I decided I was going to try FOC without  the hall sensor [ waiting for jst connectors from china =( ].... I watched all the videos and did a whoole lot of reading but after trying to set it up the vesc quit working... I think i Fried something... motor wont respond in FOC or BLDC. Nothing from the wii remote or the keyboard... i can still read and write to the vesc, but any commands to the motor result in 3 red flashes =( 

4.10 vesc with 4.18 firmware. Ive re-flashed a few times. current limits are at default... think its time to order another vesc unless i can find someone near Oceanside, CA who knows what they're doing haha
```

---
## \#127 Posted by: kampfhahn Posted at: 2016-09-20T18:46:17.956Z Reads: 263

```
Running FOC since 100 km now without any problems.

10S / VESC 4.12 / 4.18 Firmware / 190 Alien 6355 / 14/36t / Winning Remote
```

---
## \#128 Posted by: Jamy Posted at: 2016-09-20T23:00:37.832Z Reads: 269

```
After the first day of running my build in BLDC mode I really disliked the hard acceleration and deceleration. So I figured I'd give FOC a try.
This is an Enertion VESC (latest). FOC has been working fine ever since. Setup was easy and it goes smooth. I've clocked around 100km as well on mine.
```

---
## \#129 Posted by: mrpj Posted at: 2016-09-21T09:02:26.104Z Reads: 272

```
@Jamy
What motor setup are you using?

@CRABOLSKY
Any first conclusions?

I am currently getting parts for my build and was considering the sk3 6374 168kv (since it was shortly in stock) with 10s (either 3 or 4P) and I am a bit worried now. Really like to run FOC - another option would be to hope that the upcoming vesc is more reliable with this?
```

---
## \#130 Posted by: Jamy Posted at: 2016-09-21T10:40:06.729Z Reads: 268

```
Turning sk3 245kv motor, 6s 10000mAh pack, exertion pulley  system, custom motor mount. I gotta finish my build log so I can just link there :p
```

---
## \#131 Posted by: CRABOLSKY Posted at: 2016-09-21T11:54:28.049Z Reads: 271

```
I've run out of solder... I'll check back in once I am up and running.
```

---
## \#132 Posted by: CRABOLSKY Posted at: 2016-09-25T05:02:40.786Z Reads: 277

```
Maiden voyage
http://www.youtube.com/watch?v=LI0MuMi1A9k
First impressions... incredible. I am loving the torque and acceleration. Topping out at around 38kph which is short of the theoretical 45kph, however I am not sure Iam looking to go much faster. Braking is smooth and confident without any cutouts.
```

---
## \#133 Posted by: psychotiller Posted at: 2016-09-25T05:28:33.700Z Reads: 285

```
I just set up a board today with Sensored FOC.

Specs: 8s5p Li-ion Battery, a single 230kv 6374 motor, 16/36 12mm pulleys and belt on 83mm wheels.

Motor detection worked flawlessly and so did FOC and Hall sensor settings.

I seriously wasn't prepared for the silent take-off from a dead stop. 
Also, I'm amazed at how smooth and fast this board ramps up to top speed. It was a fun test ride today :astonished:<img src="/uploads/db1493/original/3X/6/3/6341037d4ab568883f25e059efdc9fd721d8dcc7.jpg" width="689" height="390">
```

---
## \#134 Posted by: CRABOLSKY Posted at: 2016-09-26T03:13:41.149Z Reads: 280

```
Okay, I had a great first test yesterday with absolutely no apparent issues (battery was at about 70%) Today however after charging to 100% on the space cell I had a 2 dropouts under full acceleration. These are the same dropouts that occurred right before frying my dvr chip last time :slight_frown: 

I took the board out under full (100%) charge last night for 10 min without issue... today the only difference I can think of is rough road under foot? So what could be causing this... I assume that the battery wasn't putting out the same voltage with the cell only charged to 70%?  

My settings are the attached accept I cant recall if I reduced the Batt Max to 40a? @whitepony the only variation per our exchange was setting the Max Input Voltage to 57v per others recommendations for the space cell (could this be the issue)? 
<img src="/uploads/db1493/original/3X/b/b/bbcd086afaa51fd1666bafb1558aef59676ef4b2.png" width="690" height="420">
```

---
## \#135 Posted by: Jinra Posted at: 2016-09-26T03:36:56.687Z Reads: 271

```
Your Regen is too high, but shouldn't cause drop outs. what are the symptoms? you have to power cycle the board, or just wait to reconnect? what remote are you using? which space cell? Regen should be -12 for scp3 and -16 for scp4 max.
```

---
## \#136 Posted by: CRABOLSKY Posted at: 2016-09-26T04:02:31.810Z Reads: 274

```
I am running the 12s3p. Enertion Steez. 

Drop out is experienced as a sharp drop out in power for a quick second. Then I can power back on. Iam pretty certain this isnt a remote connection issue... it's got to be a moment of the vesc hitting a limit and trying to protect itself. 

I am at work but will correct the regen settings for sure. I am pretty sure I followed the above (it's an early screenshot of my theoretical settings before I received my new VESC) could the batt max at 57a be an issue?
```

---
## \#137 Posted by: Jinra Posted at: 2016-09-26T04:11:19.477Z Reads: 272

```
57v max voltage should not be a problem. So you're not running a space cell as you're running 12s? Make sure to fix your battery cutoff as well since those are 10s settings.

The issue does sound like a remote issue, but maybe it's a BMS issue. Are you discharging through the BMS and what is it rated for?
```

---
## \#138 Posted by: CRABOLSKY Posted at: 2016-09-26T05:01:44.268Z Reads: 272

```
Thanks @Jinra... sorry that was a typo. I meant 10s3p (I've got 12s on the brain).

The BMS is the standard with the space cell. As per above you agree that it ins't a remote issue (I think you meant doesn't).? I am not sure exactly what I am looking for, but intuitively it feels like something isn't being "governed" correctly in my settings. That maybe too much voltage being drawn?
```

---
## \#139 Posted by: Jinra Posted at: 2016-09-26T05:11:18.726Z Reads: 272

```
The VESC doesn't "draw" voltage, it accepts whatever voltage is being fed to it and shouldn't fail unless it exceeds max voltage. Regen braking can cause small spikes of voltage, but it shouldn't be hitting the 57v cap. There was no typo, since it does **sound** like a remote issue, but perhaps can be something else.

Try this, next time the issue occurs, do not turn off the board and plug it into your computer. Open up BLDC Tool and type "faults" in terminal to see if there are any reported faults on the VESC. If there isn't, then issue lies somewhere else.. The remote would be my guess since the Space Cell bypasses BMS for discharging.
```

---
## \#140 Posted by: CRABOLSKY Posted at: 2016-09-26T05:39:42.957Z Reads: 265

```
Fair enough... that all make perfect sense. It might just be a coincidence that it feels the similar to my first issue. THe difference here is that the sudden cut-off is much less aggressive. It definitely happens with an abrupt jerk and then comes back once I've let go and reapplied the accelerator   

You know...with all this tweaking I've been thinking about leaving usb cable connected and hanging out of the enclosure until I am 100% confident. Man it could would be cool to have a small female connector built in to the external case.
```

---
## \#141 Posted by: Jinra Posted at: 2016-09-26T05:52:50.561Z Reads: 262

```
[quote="CRABOLSKY, post:140, topic:4465"]
Man it could would be cool to have a small female connector built in to the external case.
[/quote]

Why not do that then! male-to-female extensions aren't hard to find, then just cut a rectangle out and stick it in place.
```

---
## \#142 Posted by: treenutter Posted at: 2016-09-26T13:30:18.793Z Reads: 274

```
[quote="Jinra, post:141, topic:4465"]
Why not do that then! male-to-female extensions aren't hard to find, then just cut a rectangle out and stick it in place.
[/quote]


@jinra @CRABOLSKY if someone finds a weather-proofish m2f connector pls share it. I've gone looking a few times and I didn't find a suitable part, but there's got to be one out there!
```

---
## \#143 Posted by: flatsp0t Posted at: 2016-09-26T13:38:33.840Z Reads: 269

```
Sth like this?:
http://www.usbfirewire.com/parts/rr-wpmb-mbr2-xxgl.html#RR-WPMBF-MBR2-12GL
```

---
## \#144 Posted by: Jinra Posted at: 2016-09-26T15:23:17.148Z Reads: 276

```
You can also get one of these little dust covers

https://www.bestbyte.net/protective-cap-cover-for-mini-usb-port-flush-face-rubber-black.html?utm_source=google_shopping
```

---
## \#145 Posted by: CRABOLSKY Posted at: 2016-09-26T22:48:44.569Z Reads: 271

```
Might take some working to fit it into my enclosure, but this perfect! Great find @flatsp0t
```

---
## \#146 Posted by: Randyc1 Posted at: 2016-09-26T23:44:24.289Z Reads: 277

```
https://youtu.be/GBuTiCdHiWE
Edit: Sorry , ...thought you were looking for water proofing.
```

---
## \#147 Posted by: Jakeii Posted at: 2016-10-03T23:41:35.771Z Reads: 269

```
I've only been running FOC, did the BLDC motor detection, then straight on to FOC detection with out ever riding in BLDC mode!

5000mah 10S (2x5s lipos) with 190kv Alien Power Motor Works like a dream, I've had limited time to test, but went on a 10km ride on relatively flat roads, and went from 42v to 39.1v.
```

---
## \#148 Posted by: CRABOLSKY Posted at: 2016-10-06T22:08:59.354Z Reads: 276

```
Hey @Jinra back on the regen settings, what do you think the real real of frying your cells is with a regen of -20? I've seen people on the forum running anywhere within -12 to maybe -30? I thought this was one of the settings that allowed for additional tuning of your braking force. 

Part of my original upset (on my first VESC) was trying to remedy lack of braking power (and dropouts) under my BLDC settings. @whitepony runs a very similar setup with -20 on FOC. Right now I would say my brakes are absolutely perfect so I am reluctant to start messing around if it's not really needed? Obviously I don't want to prematurely kill my cells!
```

---
## \#149 Posted by: Jinra Posted at: 2016-10-06T22:14:15.506Z Reads: 277

```
Imagine if your charger was 20A. That's basically how you're charging your batteries while regening. Even 4A per cell is already high since normal charging is typically at 1c or lower. I'm using -8A on each vesc (2 vescs) with -45A motor regen per vesc and my braking is perfect.

You likely won't "fry" your cells doing -20A, but it will deteriorate your cells at a faster rate which will lead to a shorter cycle life.
```

---
## \#150 Posted by: CRABOLSKY Posted at: 2016-10-06T22:36:02.958Z Reads: 279

```
That's actually great way to visualize it. Does the amount of breaking force applied vary the level of current back to the battery? By that I mean, full brake force sends the full limit to the cells and lighter touch is a smaller amount?
```

---
## \#151 Posted by: Jinra Posted at: 2016-10-06T22:38:03.970Z Reads: 290

```
Sorry, don't know the answer to that one. However, I have heard long light braking will regen more power than harder short braking. This was info on Boosted's FAQ
```

---
## \#152 Posted by: guyguy Posted at: 2016-11-14T01:24:06.652Z Reads: 283

```
I've been cruising slow-mo around my neighborhood with my daughter who rides her scooter, but the board is embarrassingly loud on the sidewalk. So... I finally took the plunge on FOC after reading for a long time and just took a test ride around the hood. Wow, the stealth, it's more impactful than I thought it would be. My first thought was this is how it electric skateboarding is meant to be. 

I just hope the DRV chip doesn't explode.

https://goo.gl/photos/hWfNj3YLi9JmzmRz8
```

---
## \#153 Posted by: shwill Posted at: 2017-01-01T09:12:31.096Z Reads: 264

```
I've been using FOC I'm relatvly new to this stuff and no expert. After a Vesc replacement (drv) went through settings with Psycotiller Dave  since I was clueless to the process being my first time,sponging up info as I went. I set perameters on my 6355 Torque Boards motors 170kv  to match each other minus hall sensors. Been running board with regular routine maintenance hard for bout a month it's very quiet way faster than needed but controllable.smooth from beggining to top speed which I rarly reach I've hit 26 mph and a little squeeze showed it could go a bit faster for sure if not alot. Can't bust full throttle straight out the gate at least no one that's ridden it has been able to stay in controll with this approach seen two try and they were not successful luckily not to hurt minus a few scrapes.As long as you squeeze it gradually you can go as fast as desired can't see anyone able to use all power available to user  I weigh 170 and I fly no lag up hills 20% think I have a screenshot of set up parameters I'll try to locate so I can post if anyone's interested .I'm not sure what difference is between bldc  and foc I've never ridden bldc to feel the difference.But FOC is rockin so far so good put 20+ miles every day for close to a month straight without problems.Happy New Year .
```

---
## \#154 Posted by: cliofreak Posted at: 2018-01-27T01:02:59.804Z Reads: 148

```
Quick revival of this subject (I'm new).

Ive a 10s4p 30Q running 6374 motor. My Vesc is 4.12 with 3.xx FW.
I have a Mac running VescTool.

*Should I try mode FOC?
*Will I blow my DRV?
*Cross my fingers count to 3?
```

---
## \#155 Posted by: cliofreak Posted at: 2018-01-27T01:07:58.450Z Reads: 152

```
Hey, did this continue to work well? I've no idea of the true potential dangers of blowing DRV chip. Seems to be the only reason to stop me going FOC... 10s4p 6374 single 200kv. Id love the silence though.
```

---
## \#156 Posted by: psychotiller Posted at: 2018-01-27T01:08:47.259Z Reads: 150

```
Still working well.
```

---
## \#157 Posted by: cliofreak Posted at: 2018-01-27T01:13:11.869Z Reads: 153

```
Thanks man. 4.12 Vesc?
```

---
## \#158 Posted by: psychotiller Posted at: 2018-01-27T01:16:10.801Z Reads: 158

```
Yes. It's an ollin
```

---
## \#159 Posted by: Ixf Posted at: 2018-01-31T15:43:23.521Z Reads: 140

```
I run 12s4p on dual focboxes with latest ackmanic's FW.  Haven't had any issues yet.  Funny thing is that I actually blew through 3 vescs in a hurry running BLDC hybrid with default FW that came with the VESC.  Once I went Ackmanic + FOC, its been smooth sailing.
```

---
## \#160 Posted by: nickw1881 Posted at: 2018-04-29T07:35:47.225Z Reads: 105

```
I've been breaking a VESC all day today in FOC mode, blowing up one DRV8302 after another. 3 carcasses on my table now. I'm running a 7.25" propeller in water as a "dyno" to provide a repeatable load on the VESC to measure efficiency. Same problem every time. You'd think I would learn quicker...

Motor: 6374 outrunner
Battery: 12S ~50V
FOC switching frequency: 30kHz.

When the VESCs break in FOC mode and the red led does a 3 flash pattern its the DRV8302 mosfet gate drive power supply that gets broken. Everything else is OK: the logic in the DRV8302 is fine, the DC/DC is fine, STM32F4 is fine. There are no marks on the DRV8302 or burning smell. The only way to identify the problem is measure DRV8302 pin 13. The GVDD output is about .7-1.7V instead of 10-12V.

Everything is fine when I had the motor current limit set to 60A. I could run it for a few minutes as long as I cool down the VESC with compressed air. When the VESC is current limiting, it is also limiting duty cycle. When I set the motor current to 80A and ran it, it broke almost instantly 3 times in a row.

I really think this problem has to do with the gate drive power supply, though I am not sure why higher duty would cause higher gate drive power supply current. The switches have to switch on and off each cycle regardless of how long they are on or off, and it takes the same energy to switch them on and off no matter how much current goes through them. Unloaded, FOC mode throttles up all the way no problem. Is there an engineer or motor drive expert that could shed some light?
```

---
## \#161 Posted by: RedEagle Posted at: 2018-04-29T17:45:52.178Z Reads: 90

```
What vesc are you using?
```

---
