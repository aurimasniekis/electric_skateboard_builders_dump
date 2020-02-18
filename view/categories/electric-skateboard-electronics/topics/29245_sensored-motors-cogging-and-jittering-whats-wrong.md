# Sensored motors cogging and jittering - WHAT&rsquo;S WRONG?

### Replies: 80 Views: 4523

## \#1 Posted by: rich Posted at: 2017-07-31T21:52:43.398Z Reads: 375

```
I’m really desperate because my system is not working properly.
I run dual V4.12 with sensored 136kv trampa motors on my e-mtb but I have huge problems with cogging on startup. Even on concrete there is cogging but I can start from a dead stop (if it’s flat, uphill no way), on any other surface it is almost impossible to start, even on grass slightly downhill I can’t move from zero. That totally kills a lot of fun with this great trampa mountainboard and I really don’t know what this could be because I’ve tried everything possible I can imagine. 

Any suggestions welcome, I think I need some experts!

What I’ve tried so far:

4 different V4.12 with no difference in cogging
2 different brands of sensored motors - same cogging
Tested all 6 possible phase wire combinations - always same cogging
Different length of phase wires and servo wires (3 different cables tested)
several times checked all power cables, connectors and phase wire cables.
Tried different remote control and receiver (who knows, but same as always)

more details:
I run my dual V4.12 with FW 2.18 (tried FW 3.26 and FW 2.54, too - same cogging) in BLDC Mode (hybrid - traction control - slave via CAN bus). Tried different start up boost settings up to 0.1, motors get more punchy but still cogging. When going reverse same cogging, higher amp settings in BLDC Tool brought no results, too. There are no problems with motor and hall sensor table detection in BLDC Tool. The motor sensors are working, there is a difference compared to sensorless mode. I’ve also tried sensored mode but same cogging as always.

remaining setup info: 
10s 10Ah Lipo Turnigy Graphene (150A discharge/50A charge)
200mm wheels, pulleys 15/66 HTD5M 15mm belts
Anti spark switch
Steez remote

Here a video of my cogging motors so you can see the annoying start up performance (plus test ride):

https://www.youtube.com/watch?v=RFA9374i2pk&t

I didn’t change anything special beside startup boost in BLDC Tool.
But who knows maybe you’ll discover a wrong setting or you know what to tweak. Here we go: 

<img src="/uploads/db1493/original/3X/5/e/5e0711c4f26a9d8c5751d50cf0bfbd5f494bf5fb.PNG" width="690" height="310"><img src="/uploads/db1493/original/3X/1/6/16b72c6dadefc94381c6c728cb03ee3acdf2a644.PNG" width="689" height="176"><img src="/uploads/db1493/original/3X/b/a/ba70966a279c452ee106d0cec583ee8cacb2e5b8.PNG" width="690" height="267"><img src="/uploads/db1493/original/3X/c/2/c2ddb6a762ea915e9a259778a16fe0230f67ef6d.PNG" width="690" height="213"><img src="/uploads/db1493/original/3X/e/1/e16e068f5e7c1931d4279608a9c9ef76cc9fffa9.PNG" width="690" height="307">

If someone has an idea what’s wrong, let me know, thanks!
```

---
## \#2 Posted by: lox897 Posted at: 2017-07-31T21:56:37.588Z Reads: 317

```
Are you sure you wired the Hall sensors properly? Please show some pictures of the wiring. Try changing it to sensored. Make sure you do a motor detection without the belt. I'm no expert too hehe
```

---
## \#3 Posted by: rich Posted at: 2017-07-31T22:10:33.885Z Reads: 319

```
I didn't change the wiring, just soldered extensions (80 cm), but I've tried it with different lengths of extensions and also with no extension directly plugged to the V4.12. In BLDC tool the hall table automatically changes to my table when clicking APPLY after motor detection. But wouldn't BLDC tool give me an error in case of wrong wiring?

<img src="/uploads/db1493/original/3X/1/d/1dcbf8e3a0871d3fa98fa7526afb615d814bcd2e.jpg" width="690" height="388">

And I tried sensored mode, no difference in cogging.
```

---
## \#4 Posted by: JLabs Posted at: 2017-07-31T22:32:39.833Z Reads: 299

```
After clicking apply did you write the config? If not it wouldn’t have saved the values that you just detected
```

---
## \#5 Posted by: rich Posted at: 2017-07-31T22:40:55.248Z Reads: 304

```
Yes I clicked write config every time..... also I compared the saved hall table after reading config with a further motor detection, it's the same.
```

---
## \#6 Posted by: Sander Posted at: 2017-07-31T23:22:15.612Z Reads: 304

```
Not giving enough power could result in cogging(seems strange since its sensored), maybe adjust the minimum duty cycle?
```

---
## \#7 Posted by: rich Posted at: 2017-08-01T00:36:47.326Z Reads: 298

```
Do you know a safe setting for minimum duty cycle to change? Don't wanna fry my new V4.12 ( that's my 5th and 6th V4.12 on this build within 2 weeks, the first 4 are faulty)
```

---
## \#8 Posted by: Jinra Posted at: 2017-08-01T00:45:26.854Z Reads: 287

```
Just FYI start up boost pretty much IS minimum duty cycle. Vedder recommends no higher than .15.

I know it's pretty obvious, but you made sure to do separate hall sensor detections for each VESC/motor pair right?
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-08-01T00:52:43.845Z Reads: 288

```
4.12 are not the best at power delivery so you'll probably overheat it quickly but have you tried raising your motor amps.
```

---
## \#10 Posted by: rich Posted at: 2017-08-01T01:47:32.697Z Reads: 292

```
@Jinra  Ah, ok thanks! My highest start up boost setting was 0.1. The motors got more punchy after startup but same cogging.

[quote="Jinra, post:8, topic:29245"]
but you made sure to do separate hall sensor detections for each VESC/motor pair right?
[/quote]

Yes, I set up each V4.12 before connecting the CAN bus and make dual settings. Also I've tried the performance of single V4.12 with one motor, makes no difference.in cogging. 

I did minimum 50 motor/hall sensor detections the last 2 weeks with six V4.12 (no joke). My first 2 flier 4.12 had broken hall sensor ports and temp sensors, I switched to maytech 4.12, one of them had broken hall sensor port, too (cold solder joint, could resolder) but maytech SUCKS!!!!!!!!!! BAD BAD performance :sob: So I took my last money (I mean some future money :joy:) and bought 2 quality PCB's 4.12 from @esk8 but unfortunately there is no difference in cogging (but in performance).

[quote="Titoxd10001, post:9, topic:29245, full:true"]
4.12 are not the best at power delivery so you'll probably overheat it quickly but have you tried raising your motor amps.
[/quote]

I know 4.12 are not best for MTB use but I have plenty of power with this setup if it's not too steep in offroad conditions and I don't start from standstill again :wink: My enclosure has holes for some air and I can ride for 1,5h without problems (full charge). My max mosfet temp was about 70 degrees (ok once 80 degrees), i'll add heatsinks or thermal silicone in the future but this cogging kills me right now.

My highest max motor and batt amp settings were 60A (like trampa motor is rated). My battery is good for 150A cont. so I could try motor max 80A and batt max 70A and see if there is a difference (and if motors getting too hot)

I think a dual V4.12 must handle a startup without cogging (with sensored motors). Strange is that it's exactly the same cogging in sensorless mode as in sensored or hybrid. But i can feel that the sensors are working in sensored/hybrid mode, there is a difference in performance but not in start from a standstill. Weird.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-08-01T01:57:02.900Z Reads: 248

```
Try raising the motor max amps. 50a motor max is really low.
Raising the motor max will give you more power at low speed and when starting off.
Find out what the max amp rating is for your motors and set it there.
I run 80a motor max on my dual street boards
```

---
## \#12 Posted by: rich Posted at: 2017-08-01T02:08:20.109Z Reads: 254

```
The motors are rated for 60A max as far as I know. @trampa suggest not to go higher than 50A motor max. that's why i set 50A but I'll definitely try to raise it (60A made no difference). Can I harm the motors with higher max amp settings than the motor is rated for? But I think I won't hit this amps in real life (when I trust my app)
```

---
## \#13 Posted by: Namasaki Posted at: 2017-08-01T02:16:57.878Z Reads: 250

```
I have tried running mine at 100a but that caused them to run hotter so I backed it down to 80a
You can raise yours and then stop and check your motors to see if they are getting too hot.
Note: if your riding in 100F weather, they are gonna be hot just because of the ambient temp.

What are the size and power specs on those motors?
```

---
## \#14 Posted by: rich Posted at: 2017-08-01T02:30:17.732Z Reads: 243

```
6364 136kv 7 pole BLDC Motor 2400W
Internal Magnetic Hall Sensors on Axle Shaft

http://www.trampaboards.com/136-kv-2400w-dc-brushless-motor-6364-61-p-12967.html
```

---
## \#15 Posted by: Namasaki Posted at: 2017-08-01T02:43:39.772Z Reads: 239

```
These motors have HAL and Temp sensors so the Vesc should monitor the temp for you.
I would raise it to 60a and see if that stops the cogging and if if gets better but not completely gone then I would start ticking it up 65,70,75 until the cogging stops. Then let the vesc monitor the heat.
```

---
## \#16 Posted by: rich Posted at: 2017-08-01T03:17:42.545Z Reads: 245

```
[quote="Namasaki, post:15, topic:29245"]
These motors have HAL and Temp sensors so the Vesc should monitor the temp for you
[/quote]

In Vesc-Tool with FW 3.26 i can monitor the motor temp but in BLDC Tool and FW 2.18 not. I don't really know why there is motor start end end temperature setting because as far as I know FW 2.18 can't read motor temp. But I use my fingers as motor temp sensors :joy:
```

---
## \#17 Posted by: Namasaki Posted at: 2017-08-01T04:31:04.995Z Reads: 237

```
I used this to check temp on my hub motors, Haven't had to worry about heat on my belt drive motors.
https://www.amazon.com/gp/product/B00DMI632G/ref=oh_aui_detailpage_o07_s00?ie=UTF8&psc=1
```

---
## \#18 Posted by: flywithgriff Posted at: 2017-08-01T05:46:57.920Z Reads: 227

```
If you extended the sensor wires, make sure the wires are in the right order. Often the motors come with a smaller plug on them and when requiring the correct plug into the sensor wires the colors do not match. This could very well be your issue.
```

---
## \#19 Posted by: Jinra Posted at: 2017-08-01T05:49:19.606Z Reads: 227

```
I assumed they were in the right order given that detection actually works and the values look correct to me. However, I guess it's worth checking.

@rich Keep in mind that most motors have a different order of sensor wires than the VESC takes.
```

---
## \#20 Posted by: lrdesigns Posted at: 2017-08-01T06:43:13.991Z Reads: 233

```
After watching your video it sounds like the sensors may be working but just not properly from 100% stand still. There is that kind of gear noise when they first start to move, I get that from censored mode at low speed. My board does the same it will not start from 100% stand still but half a push and it will get moving. Its still much smoother than un-censored mode. Maybe try un-sensored mode to see if there is any difference, that will tell you if the censors are working. 

If my boards is not loaded the wheels will always start from stand still and always in the correct direction, no jittering like un-censored. And the minimum rpm is lower than un-sensored. 

As to how to fix the issue I don't know, but I do think the guys saying start up torque too low are onto something.
```

---
## \#21 Posted by: rich Posted at: 2017-08-01T14:24:55.824Z Reads: 224

```
@Namasaki good idea, i have a temperature gun.

@flywithgriff and @Jinra,  on the trampa motors there are already JST 2mm pitch female connectors.  

The motor has this assignment (written in manual):
ground (black)
phase C (orange)
phase B (white)
phase A (green)
temp (blue)
+5 Volt (red)

Beside the fact that the orange cables are brown on my motors (no problem at all) it’s exactly the same pin assignment as on the hall sensor ports on V4.12, the wiring is right (and my extensions).

[quote="lrdesigns, post:20, topic:29245"]
My board does the same it will not start from 100% stand still but half a push and it will get moving
[/quote]

Well , that's what I do for now but it's not really funny to do that on mountainboard with bindings :wink: I've tried all modes, the sensors are working, it's much smoother at low speed compared to sensorless mode but same cogging.
```

---
## \#22 Posted by: Jinra Posted at: 2017-08-01T14:33:16.699Z Reads: 208

```
Typically, by convention, white is temp. i wonder if this is a mistake in your manual, or if the manufacturer designed it this way.
```

---
## \#23 Posted by: rich Posted at: 2017-08-01T14:45:18.489Z Reads: 207

```
It's designed that way (only the orange cable is brown in my case, or I have bad eyes :joy:) here the original motor JST female:

<img src="/uploads/db1493/original/3X/1/3/1330748eb9fa94181d4f4d56d570a000edb50676.jpg" width="690" height="388">

And blue is 100% the temp because on my Smescs 4.12 (shitty maytech esc) i've tried FW 3.26 and could see the motor temp realtime date in Vesc-Tool, so just the cable colors differ, not the pin assignment.
```

---
## \#24 Posted by: Jinra Posted at: 2017-08-01T14:49:20.298Z Reads: 198

```
If everything else is correct then i guess it must be your motors. Hall sensors aren't exactly the most precise thing and can cog as well. I run 120 degree halls on mine, and i occasionally get slight cogging, but it works very well most of the time.
```

---
## \#25 Posted by: rich Posted at: 2017-08-01T14:58:52.705Z Reads: 195

```
That's why i've tried sensored 6364 190kv maytech motor, too (of course with motor detection, apply and write config) Weird that this maytech motor has exactly the same cogging and sounds equal while cogging as the trampa motors, only when spinning the sound changes. Furthermore I could try sensored 6355 APS motors but I doubt it's a motor problem.
```

---
## \#26 Posted by: Jinra Posted at: 2017-08-01T15:03:03.374Z Reads: 190

```
How about try turning off traction control
```

---
## \#27 Posted by: rich Posted at: 2017-08-01T15:19:28.881Z Reads: 190

```
Yes actually it's disabled but no difference. Also tried all 6 possible phase wire combinations as you wrote in a different thread.
```

---
## \#28 Posted by: Silverline Posted at: 2017-08-01T15:24:42.008Z Reads: 186

```
What remote are you using ? Have you tried with another model ? Or a ferrit ring on the ppm cable.
```

---
## \#29 Posted by: rich Posted at: 2017-08-01T15:31:51.811Z Reads: 187

```
I have a steez remote but also tried a old GT2 remote but same cogging.
What do you mean with ferrit ring on the ppm cable?
```

---
## \#30 Posted by: Jinra Posted at: 2017-08-01T15:36:40.963Z Reads: 191

```
Ferrite rings resolve signal issues.. which doesn't look like what you're experiencing. I'm at a loss on this. Have you tried removing load (take off belt) to see if it cogs?
```

---
## \#31 Posted by: rich Posted at: 2017-08-01T15:42:37.102Z Reads: 181

```
The motors don't cog with belts. So without standing on the board there is no cogging at all and the startup is supersmooth. But when i'm on the board (74kg) there is always cogging.
```

---
## \#32 Posted by: Silverline Posted at: 2017-08-01T16:18:44.700Z Reads: 180

```
Im a newbie. But i had some sort of jittering problem with my winning remote. Also shouldn't max erpm be 60.000 to protection the Drv ?
```

---
## \#33 Posted by: Jinra Posted at: 2017-08-01T16:19:31.171Z Reads: 176

```
He won't go anywhere near 60k erpm, so it doesn't really matter.
```

---
## \#34 Posted by: flywithgriff Posted at: 2017-08-01T16:46:51.737Z Reads: 170

```
I just watched your video and do not see your vesc. Are they mounted in the battery box? How long are your battery wires from battery to vesc and how long are phase wires from vesc to motors? This could be your problem.
```

---
## \#35 Posted by: Jinra Posted at: 2017-08-01T16:53:05.797Z Reads: 170

```
My wires are like 20 inches and they work fine.
```

---
## \#36 Posted by: trampa Posted at: 2017-08-01T16:57:11.913Z Reads: 171

```
Hi @rich, how long are your cables? 
The 136kv is good with 60A if you use temp sensors. On a twin you will hardly push 60A.

Frank
```

---
## \#37 Posted by: rich Posted at: 2017-08-01T19:46:10.763Z Reads: 181

```
I’m not sure if the length of the battery cables are measured starting from the battery itself or from the connectors of the battery cables. But if measured from battery wire connectors I’m below 20 cm / 8 inch (as you see on the pic I have an anti-spark switch between battery and V4.12’s (but also tested it without this switch)

Well, I’m one of the world champions regarding phase and hall sensor wire lengths.
The phase wires are 12 AWG and about 80 cm / 32 inch
The hall sensor extensions are 22 AWG and about 85 cm / 33.5 inch
But I’ve tried it with 20 cm / 8 inch phase wires and 10 cm / 4 inch hall sensor extension, too. Hmmm but only with the maytech 4.12’s. Their performance is not like it should be (very poor quality) so I try the short cables with the new @esk8 controller now, who knows?

<img src="/uploads/db1493/original/3X/0/8/081adfa3945bdc124610f8d60a5afd75124f2033.jpg" width="690" height="388">

@flywithgriff yes, as you can see they share the same enclosure. The battery is inside a lipo safe bag and seperated with 0.5mm aluminium sheet from the V4.12's and the top cover has 2 holes above the controllers. In case of rain i close the holes with fabric tape but anyway, this enclosure is splashproof only, not waterproof.
```

---
## \#38 Posted by: marcuscrackus Posted at: 2017-08-01T19:57:23.550Z Reads: 178

```
Hi I am having the exact same problem as you. Just got my E-MTB with 136kw Trampa motors. i have 4.12 maytech vescs, still working....

I have just received delivery of the Vesc 6 so will be installing them next week, would be good to see if it solves the problem. I have been watching Jems Kappel's video on you tube using vescs and he is wheel spinning on grass, mine won't even start on grass.

Seems to be no torque in the motor at low speeds and i want torque, not top speed.
```

---
## \#39 Posted by: rich Posted at: 2017-08-01T20:34:22.272Z Reads: 178

```
[quote="marcuscrackus, post:38, topic:29245"]
i have 4.12 maytech vescs, still working....
[/quote]


Uuuuuuh, do you use the FW 2.18 which is uploaded from maytech? My maytech ones had both the max current ramp step bug (everytime you read or write configuration it gets multiplied by 10). When I read configuration first time, the setting was 40.0 instead of 0.004. Check this before you fry your V4.12!
And let me know how VESC SIX performs with this motors, i think i'll need them, too in the future.

But I have a lot of power at low speeds but not at startup.

[quote="marcuscrackus, post:38, topic:29245"]
I have been watching Jems Kappel's video on you tube using vescs and he is wheel spinning on grass, mine won't even start on grass.
[/quote] Yeah I know that video but it's not comparable to his "normal wheelies" I think he prefers raw power of car esc's on mtb and as far as I know @Nowind even mostly use sensorless motors on his builds. Well I don't even know if he likes smooth startups :joy: (Isch don't think so) cogging seems no problem with car esc and full throttle.
```

---
## \#40 Posted by: trampa Posted at: 2017-08-01T20:35:00.700Z Reads: 181

```
Hi, there is plenty of torque. I think your sensor cables are the issue. To long and maybe you use connectors in between. Try to use short cables and no extension connectors. The longer your cable, the thicker it should be. Long cables have a much higher resistance. If your cables get to long you need to amplify/smoothen the signal, using a small PCB, designed for the job. Shielding the cable is also wise.

Frank
```

---
## \#41 Posted by: rich Posted at: 2017-08-01T20:51:01.822Z Reads: 182

```
[quote="trampa, post:40, topic:29245"]
there is plenty of torque
[/quote]

That's true, I confirm that 100%, it is so powerful that I think this beast could kill me one day :joy:
But at startup it's a tweeting bird right now. 

I'll check it again with short cables, I just need to stop writing, lol....
```

---
## \#42 Posted by: marcuscrackus Posted at: 2017-08-01T20:55:24.433Z Reads: 175

```
Yes noticed the wrong settings, one was 40 and one was 50. they are now back to the origonal settings. 

Frank the Sensor cables on mine are not extended. I am going to try the 13 tooth pully this weekend, Ted sent me some over with my Vesc 6's which i hope to have in next week. I will be talking with Sanjoy to match his settings on the Vescs.
```

---
## \#43 Posted by: trampa Posted at: 2017-08-01T21:21:53.317Z Reads: 172

```
@sanjoy s board runs like a treat. 

Frank
```

---
## \#44 Posted by: Jinra Posted at: 2017-08-01T21:22:55.915Z Reads: 169

```
[quote="rich, post:39, topic:29245"]
When I read configuration first time, the setting was 40.0 instead of 0.004
[/quote]

.04 is the default value btw not .004
```

---
## \#45 Posted by: rich Posted at: 2017-08-01T21:31:02.496Z Reads: 159

```
you're right, my bad.
```

---
## \#46 Posted by: flywithgriff Posted at: 2017-08-01T22:24:36.065Z Reads: 156

```
I would be willing to bet your problem is in your wire lengths. You have tried just about everything else.
```

---
## \#47 Posted by: Petertaylor Posted at: 2017-08-02T01:17:54.698Z Reads: 155

```
Wondering if it's to do with belt tension. I could see a scenario with startup problems if the belts are too tight. Most pulleys aren't totally round either, so it's possible the belt feels good in one spot but too tight in another. Is there the chance to reduce belt tension just a smidgen?
```

---
## \#48 Posted by: benwong Posted at: 2017-08-02T01:27:48.887Z Reads: 163

```
my EMTB having slightly cogging while start up on concrete, and more serious on grass. 
using sensor hybrid mode. i try take some video to show.
```

---
## \#49 Posted by: flywithgriff Posted at: 2017-08-02T01:34:24.540Z Reads: 165

```
The torque this setup should produce would eliminate it being belt tension or slightly out of round pulleys.
```

---
## \#50 Posted by: rich Posted at: 2017-08-02T23:28:12.070Z Reads: 166

```
@trampa  @esk8 @flywithgriff @Jinra
I tried it again with 30 cm / 12 inch phase wires and 15 cm /  6 inch hall sensor extension with one motor. I'm waiting for someone yelling "hidden camera", I think these wires can't be too long. I'm frustrated now, leaving the country for 3 days and get a fresh mind but I really don't know what to do.

https://www.youtube.com/watch?v=-E1rOFEzJzc
```

---
## \#51 Posted by: Jinra Posted at: 2017-08-02T23:33:59.887Z Reads: 171

```
Yea, I didn't think it was the wire length. Honestly pretty sure it's just a mixture of load and the inaccuracy of hall sensors in general. You'd probably get less cogging with both VESCs setup, and a bit more aggressive of a start on throttle.

At least from the video, it's about what I'd expect in a 120 degree hall setup on AT single.
```

---
## \#52 Posted by: rich Posted at: 2017-08-02T23:50:23.553Z Reads: 170

```
@Jinra  The cogging with dual is just the same. The motor has a lot of torque and i can start like a rocket if someone give me a push from behind :joy: I only had sensorless motors before and the difference is nice but not on startup. I wonder why people with VESC 6 and these motors have buttersmooth startups, it's the same 120 degree hall sensor??? Like it is I can't go offroad (or never stop).Everytime I have to push it like a longboard but with one foot strapped, I could brake a leg while pushing, I felt down several times and hurt my legs. Try to push a mountainboard in offroad conditions strapped. It feels more scary than riding :wink: 

But i saw @laurnts is using HW4.12 with 118kv trampa motors, but I think with FOC.
So laurnts, how is your startup performance and did you test it in BLDC mode? Would be very interesting.
```

---
## \#53 Posted by: Jinra Posted at: 2017-08-03T00:00:47.985Z Reads: 173

```
i don't doubt the torque of the motor, but load can still be an issue for the motor to startup. As an anecdote, I've noticed more stuttering on my larger 63mm motors (sensored) than on my 50mm (sensored).

How is belt tension, not too tight correct?
```

---
## \#54 Posted by: rich Posted at: 2017-08-03T00:04:07.181Z Reads: 171

```
it's quite loose, never had belt slipping. But cogging is the same with more tension, makes no difference.
```

---
## \#55 Posted by: lrdesigns Posted at: 2017-08-03T00:30:58.183Z Reads: 177

```
You mentioned you tried 4 different vesc's but are they different brands? Which brands did you try? I have the same issue on a street board with maytech's. 

Edit, if your wondering I'm using Ackmaniac's firmware. I installed a bootloader. So the firmware does not fix the issue.
```

---
## \#56 Posted by: rich Posted at: 2017-08-03T00:45:14.372Z Reads: 175

```
Well, meanwhile I've tried six V4.12 :joy:. The first two are FLIER, ordered from scramboards with broken temp sensors and hall sensor ports. But first i didn't recognize that the hall sensor table detection failed. No 3 and 4 are MAYTECH, one of them had broken hall sensor port, too, @JohnnyMeduse found the cold solder joint on one pin in the picture I've posted in a different thread. After resoldering it worked but the maytech 4.12 have strange behaviour and are poor quality, I've tried 3 different FW and everytime other/new problems (2.18 was best). Both maytech FW 2.18 had max current ramp step bug. No 5 + 6 are from esk8.de, good quality and performance but all 6 V4.12 have same cogging no matter if sensored, hybrid or sensorless, the cogging is always the same as in sensorless mode.
```

---
## \#57 Posted by: rich Posted at: 2017-08-03T01:28:42.984Z Reads: 171

```
Got a reply from Benjamin Vedder in the Vesc-Project forum. He says that startup performance is better with FOC and should work with low kv motors like trampa. So next week I'll give FOC a try (but with the maytech first), if I fry them I don't really care anymore..... I'll let you know!
```

---
## \#58 Posted by: lrdesigns Posted at: 2017-08-03T01:43:16.071Z Reads: 173

```
[quote="rich, post:56, topic:29245"]
No 5 + 6 are from esk8.de, good quality and performance but all 6 V4.12 have same cogging
[/quote]

Ok good to know its not a brand specific issue. 

Edit; I am running 140kv so I guess its related to very low kv motors?

I spoke to maytech directly and they said not to run foc, but some users had success, I think it depends on the motor and settings if it survives.

Did you try the hip wiggle move to get the board moving without putting a foot down?
```

---
## \#59 Posted by: rich Posted at: 2017-08-03T02:31:32.962Z Reads: 175

```
Funny that in the manual of maytech 4.12 FOC is a own chapter :joy: But I read in this forum there are wrong and missing parts on the maytech pcb's that's why people fry them. Normally I would not try FOC on maytech but I'll try it next week with FW 3.26 and FOC for science! But to be honest, I think they gonna die.....[quote="lrdesigns, post:58, topic:29245"]
Did you try the hip wiggle move to get the board moving without putting a foot down?
[/quote]

Yes, that's my move on grass when it's flat :laughing:
```

---
## \#60 Posted by: Blasto Posted at: 2017-08-03T03:20:49.310Z Reads: 183

```
I skimmed through the thread.

How do you configure each vesc? Via CAN fwding or via usb one at a time?

If you use CAN fwding, you will overwrite the hall table of the slave and not have the proper hall table on your slave. So the slave will gogg and with tracking control it will prevent the master from turning. Once you hit a certain erpm, the sensors are ignored.

Edit: nvm, don't think this is the issue, just saw the last video
```

---
## \#61 Posted by: rich Posted at: 2017-08-03T03:27:57.477Z Reads: 200

```
[quote="Blasto, post:60, topic:29245"]
How do you configure each vesc? Via CAN fwding or via usb one at a time?
[/quote]

I configured each vesc standalone with their usb, afterwards connected CAN.
```

---
## \#62 Posted by: rich Posted at: 2017-08-07T20:06:35.123Z Reads: 191

```
:grin::laughing::smile::joy::sunglasses:! IT'S WORKING LIKE A CHARM NOW!
Thanks for input @trampa @esk8 @Jinra @Namasaki @flywithgriff @Blasto @Titoxd10001 @Irdesigns Silverline, Sander, JLabs, Petertaylor, lox897!

As benjamin vedder said, the solution is so simple: FOC!!!!!!!! I use FW3.26 in sensored FOC mode and my sleeping lion is awake! Roooooarr! The difference in start up performance is not like day and night, it's a complete different universe compared to sensored/hybrid mode in BLDC.! I am so happy after the last disappointing weeks, I can't stop smiling when i push the throttle :heart_eyes: and I can't hear the motors anymore, wicked! It's still a beast with motor max / batt max. 40A, lol., can't wait to test it outside soon!

@Irdesigns @marcuscrackus @benwong, sensored motors like FOC, not BLDC! 
I've tried first FOC with my maytech 4.12's, everytime I brake there is a DRV fault and cut off on both V4.12's no matter which settings. So i put my esk8.de 4.12's on FOC and didn't have any faults or cut offs so far, they seem to like FOC like me :grin:

As evidence I'll post a video here within the next days so you can see the awesome startup performance of my new trampa lion!!! What is cogging? never heard about :joy::joy::laughing:
```

---
## \#63 Posted by: flywithgriff Posted at: 2017-08-07T21:26:03.848Z Reads: 184

```
Awesome man! Glad it's working for you now! Def post a video.
```

---
## \#64 Posted by: trampa Posted at: 2017-08-07T22:45:45.331Z Reads: 178

```
Congratulations! You are now a FOCer!

Frank
```

---
## \#65 Posted by: rich Posted at: 2017-08-07T22:52:09.457Z Reads: 177

```
I would say I'm a motherFOCer frank :joy: I can't resist to test it now outside, it's night but 
I have bright offroad lights and don't wake my neighbours with FOC :laughing:
```

---
## \#66 Posted by: trampa Posted at: 2017-08-07T22:53:47.952Z Reads: 175

```
Happy FOCing in the dark! Don't kill yourself. 

Frank
```

---
## \#67 Posted by: benwong Posted at: 2017-08-08T00:38:30.653Z Reads: 180

```
Good to hear you man.  
I try FOC once in benchtest. It is quiet. 
But i switch back to BLDC, just worry will fried my VESC. I am happy with BLDC so far. But maybe future will try FOC. 

I  yet free to take some video showing the cogging. 
Let me do it today~~
```

---
## \#68 Posted by: rich Posted at: 2017-08-08T03:12:41.343Z Reads: 177

```
[quote="trampa, post:66, topic:29245"]
Happy FOCing in the dark!
[/quote]

I could FOC all day and night, It was FOCing great! 

I'm back from my 12km nightFOC and can't stop to grin. I've tested startup from standstill on different terrains, grass, crushed rock, mother earth and everything else I've found on my way. Everytime butter smooth startup from zero to hero! Starting uphill from standstill no problem at all! Even when I rolled backwards on a hill I could start forward..... I'll be back and FOC around a lot!

2 days ago I thought I will never ever use my heelstraps because it's too dangerous. But now I can't wait to mount my FOCstraps! :stuck_out_tongue_winking_eye: When I reached home I connected my V4.12's to VESC-TOOL and checked for faults in terminal, I was scared but "No faults registered since startup" :grin:
```

---
## \#69 Posted by: trampa Posted at: 2017-08-08T22:02:00.073Z Reads: 169

```
The new VESC-Tool is FOCing amazing, isn't it.
Once public, there will be a lot more FOCers on this planet. You should feel how FOCing amazing the new VESC FW is in combination VESC SIX.
The old 4.12HW can't make use of new FW features. They run better then ever, but not as good as the new HW designs.

Frank
```

---
## \#70 Posted by: rich Posted at: 2017-08-10T22:11:26.498Z Reads: 166

```
Here the promised video, wanted to make a short one, now it's almost 15 minutes :joy: comparing FOC and BLDC mode. But don't worry, the startup performance part is in the beginning :wink:

https://youtu.be/ptlHqK7kqCA
```

---
## \#71 Posted by: flywithgriff Posted at: 2017-08-10T22:21:43.160Z Reads: 167

```
Awesome video man!! Can't wait to have mine up and running foc.
```

---
## \#72 Posted by: flywithgriff Posted at: 2017-08-27T02:41:52.744Z Reads: 156

```
Finally got my setup rolling. But guess what, COGGING! And im already running FOC.
```

---
## \#73 Posted by: rich Posted at: 2017-08-27T05:35:47.212Z Reads: 155

```
Oh no! Cogging at start up only or during riding as well?
You have FOCBOX, isn't it? Just to get sure, you have sensored motors and chose "sensored" FOC, right?
Did you extend your sensor wires with JST connectors?
```

---
## \#74 Posted by: flywithgriff Posted at: 2017-08-27T13:48:37.656Z Reads: 151

```
Just on startup and you are correct on the FOCBOX's. My motor max is currently at 40 so I'm assuming I may have to bring it up to 60 or so.
```

---
## \#75 Posted by: Deckoz Posted at: 2017-08-27T14:08:59.212Z Reads: 146

```
Have you tried setting the min eRPM higher? Min erpm is like min throttle on quads. When min throttle is to low sometimes the motors cog because the back emf is to low. For example

Stock is min erpm150. I have mine set to 307. This allows my motors to start without cogging in both bldc and foc.
```

---
## \#76 Posted by: flywithgriff Posted at: 2017-08-27T16:04:05.851Z Reads: 140

```
I wasn't aware this was even a thing to be adjusted. I will look into it for sure.
```

---
## \#77 Posted by: rich Posted at: 2017-08-28T21:07:01.601Z Reads: 136

```
[quote="flywithgriff, post:74, topic:29245"]
My motor max is currently at 40 so I'm assuming I may have to bring it up to 60 or so
[/quote]


I am afraid that won't change anything :disappointed:

Do you use sensor wire extensions (with connector) or is it directly plugged to FOCBOX?
```

---
## \#78 Posted by: flywithgriff Posted at: 2017-08-28T21:29:42.963Z Reads: 136

```
I upped the motor min to -60 and max to 60. No more problems. My sensor wires run directly from motor to FOCBOX connector.
```

---
## \#79 Posted by: rich Posted at: 2017-08-28T21:33:11.504Z Reads: 136

```
I am glad that it works for you now :grinning: didn't expect that increasing motor max solved it.
```

---
## \#80 Posted by: flywithgriff Posted at: 2017-08-28T21:38:43.436Z Reads: 136

```
I think maybe motor min helped me out.
```

---
