# VESC won&rsquo;t smoothly drive a SK3-6374 motor in a custom Sinclair C5 project? Please help

### Replies: 64 Views: 5795

## \#1 Posted by: ian.davidson Posted at: 2016-09-13T18:47:45.263Z Reads: 344

```
I have a VESC issue which I’d be so grateful if someone could be help on and highlight the error of my ways.

I’m using an SK3-6374-168kv motor off 8S (32V) to power a small electric trike. In fact, it’s a ‘Sinclair C5’ if anyone remembers these? :slight_smile:

http://bright-cars.com/uploads/sinclair/sinclair-c5/sinclair-c5-17.jpg

The Sinclair C5 has 16” wheels so the motor is geared down 15:1 to provide a top speed of 17 MPH (off 32V); easy for a 2000W electric motor?

Before the VESC I was using a huge Castle Creations Phoenix Edge 200A ESC. This worked ‘ok’ but I got that nasty ‘cogging/stuttering’ sound when starting from a standing-still, or if I opened the throttle too quickly when on the move. When it wasn’t ‘cogging/stuttering’ though, the Sinclair C5 accelerated rapidly. Using this ESC’s data-logging capabilities, at times the motor was shown to peak at 200-300A though!

After doing some Googl’ing I stumbled across the VESC which seemed to answer all my prayers. However, try as I might it’s proving to be much worse than the CC Phoenix Edge 200A ESC

I’ve read all the FAQ’s and watched all the videos. Every configuration step completes perfectly , exactly as documented, but the end results are just very poor.

The motor is EXTREMELY jumpy /stuttery and the VESC easily cuts-out when the current maxes out at my pre-configured 80A. This confuses me, as I thought the VESC would ‘manage’ the current up to the configured maximum, but from the live data you can see it just goes straight to the max configured current (80A) and then after a jumpy/stuttery 3 seconds, cuts out.

What is happening? Everyone is saying the VESC is silky smooth from stand-still, but my experience is the polar opposite? Even when I’m on the move when I try to gently accelerate the motor jumps and shutters. With no load on the motor (i.e. the rear-wheels lifted off the ground), it’s perfect.

I would be delighted to share my config file if it would help.
```

---
## \#2 Posted by: kampfhahn Posted at: 2016-09-13T18:59:22.606Z Reads: 306

```
How much does this vehicle weight?
Which remote are you using?
How does driving feel after you pushstarted your vehicle?
```

---
## \#3 Posted by: chinzw Posted at: 2016-09-13T18:59:42.939Z Reads: 301

```
Im pretty sure 80A is over the VESC ratings
```

---
## \#4 Posted by: ian.davidson Posted at: 2016-09-13T19:34:31.765Z Reads: 301

```
Thanks for your reply!

The vehicle weighs 45kg (100lb) - I weigh 77kg (170lbs) - so approx 122kg (270 lbs) all inc.

To put things in context, when the Sinclair C5 was released in 1985 it had a tiny 250W / 12V motor and was capable of 12-14 MPH. It was also advertised to take a rider up to 95kg (210 lbs) in weight.

The VESC control input comes from a PPM signal (although why all the VESC docs/software call it PPM I'm not sure, as it's PWM). For testing therefore I'm simply using a servo-tester.

Even from a 'rolling-start' it's no different. For example, if I get the vehicle up to 5 MPH and then open the throttle the motor just cogs/stutters/jumps for a couple of seconds (accelerating the vehicle marginally) and then the VESC cuts out, presumably because it's maxed out at 80A for too long. If I wait a couple more seconds, the VESC will work again.
```

---
## \#5 Posted by: ian.davidson Posted at: 2016-09-13T19:36:19.583Z Reads: 276

```
Yes, I think it's officially rated to 60A, but I simply thought I'd try upping this slightly to 80A since I was getting no joy at 60A.

60A @ 32V (1920W)  'should' be more than ample though... if it works.
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-09-13T19:41:55.126Z Reads: 270

```
Would it be possible to use twin motors in this thing? I would try a lower KV motor, and if possible, two of them. I'll bet a pair of SK3 6374 149KVs would do it. I'll bet you could get it to start from a standstill then as long as you weren't on a hill.
```

---
## \#7 Posted by: ian.davidson Posted at: 2016-09-13T19:51:13.305Z Reads: 272

```
It just seems so odd how a 30-year-old brushed 250W / 12V motor can do it with ease, yet a correctly geared (15:1) 2000W 32V brushless motor, can't ?

By doubling up the SK3 6374, I would be chucking 4000W (over 5HP) at the problem... to do 17 MPH ?

I must be missing something, as all these videos I see of folk's skateboards pulling away smoothly and quietly (and probably geared for faster than 17 MPH), and yet mine can barely get this vehicle moving at all.

So confusing :pensive:
```

---
## \#8 Posted by: kampfhahn Posted at: 2016-09-13T19:52:25.457Z Reads: 258

```
When the VESC is set up perfectly, you have good and smooth acceleration, even from a standstill. The problem is to get to this sweetspot. Using a remote with only a small lever travel like the Winning remote, you only have a very small "window" between stuttering and the VESCs failsafe. In my case this window is only about 2mm on my Winnings lever. Even with no load on the deck my VESC failsafes when i push the remote too fast.

Don´t know your servo-tester but i assume you set it up correctly to match 0-50-100% in the "Display" area of the PPM Tab in BLDC tool? Do you have a "real" remote like the GT2b to test your setup again?

How many teeth do your gears have btw?
```

---
## \#9 Posted by: mattdig Posted at: 2016-09-13T19:57:11.393Z Reads: 249

```
The Amp rating of the VESC (or any ESC) is all about temperature. From Enertion's site:
"Up to 240A for a couple of seconds or about 50A continuous depending on the temperature and air circulation around the PCB"

So you can burst up to 240A without issue for hard acceleration or braking, and cruise around 50A. But if you put active cooling on the VESC you can push past that.
```

---
## \#10 Posted by: ian.davidson Posted at: 2016-09-13T20:40:23.787Z Reads: 242

```
Thanks again for your message - I truly do appreciate everyone's thoughts on this...

Indeed, my PPM (*cough* PWM) is correctly set-up and displays correctly in the Display area. I've tried "Current no reverse" and "Duty cycle no reverse". The servo-tester requires a full 360' rotation to operate the throttle, so there's actually quite a lot of resolution there.

On the face of it, if yours is failsafe'ing too, does this not suggest something isn't quite right there too? Sorry, just thinking out aloud now :) If the VESC cuts-out due to hitting the max current configured, why instead does it not just 'manage' this by automatically backing the current back down?

My gearing is actually two fold... 12:60 on a belt and then 9:26 on a chain, so the end result it's actually 14.44:1
```

---
## \#11 Posted by: ian.davidson Posted at: 2016-09-13T20:41:18.783Z Reads: 229

```
That's really great insight Matt - thanks for sharing this.

I'm guessing the VESC will protect itself from overheating?
```

---
## \#12 Posted by: kampfhahn Posted at: 2016-09-13T20:56:46.651Z Reads: 232

```
[quote="ian.davidson, post:10, topic:9544"]
On the face of it, if yours is failsafe'ing too, does this not suggest something isn't quite right there too? Sorry, just thinking out aloud now :slight_smile:
[/quote]

I think that my current limits in the BLDC tools motor configuration are set too conservatively, but since i never accelerate from standing still and i don´t have problems with it while riding, i don´t waste time seeking for the cause.

Maybe @devin can help here since he´s the expert of the VESCs current settings and in getting much torque at low rpms.
```

---
## \#13 Posted by: treenutter Posted at: 2016-09-13T21:02:31.372Z Reads: 221

```
@ian.davidson just checking - did you run through motor detection with BLDC Tool?
```

---
## \#14 Posted by: Titoxd10001 Posted at: 2016-09-13T21:03:24.482Z Reads: 219

```
If it's one of those big brushed motors they have more torque than brushless at least from a standstill. For something so heavy sensored motors might help but dual motors would be better to distribute load.
```

---
## \#15 Posted by: elkick Posted at: 2016-09-13T21:12:24.916Z Reads: 214

```
What are your max input voltage and cutoff start/end values?

Could you please post some screenshots of your values in BLDC/FOC and Advanced tab? 

It might be easier to help you that way.
```

---
## \#16 Posted by: mattdig Posted at: 2016-09-13T21:14:45.253Z Reads: 200

```
I assume it would, the VESC is pretty smart and has lots of safety cutoffs built in, but I don't know for sure.
```

---
## \#17 Posted by: devin Posted at: 2016-09-14T01:27:02.090Z Reads: 205

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#18 Posted by: kampfhahn Posted at: 2016-09-14T06:22:33.914Z Reads: 192

```
Actually @ian.davidson is the one who needs help since he started this thread. I´m almost happy with my setup. Don´t want to mix up things here.
```

---
## \#19 Posted by: ian.davidson Posted at: 2016-09-14T06:25:19.778Z Reads: 194

```
Sorry chaps, I've yet to work out how to 'quote' a preview post here - but yes @treenutter, I've been through every set-up process possible with BLDC, any every process completed perfect, as described in the FAQ, to shown on one of the instruction videos.
```

---
## \#20 Posted by: ian.davidson Posted at: 2016-09-14T06:27:28.860Z Reads: 197

```
@titoxd10001 Ironically, one of the reasons the Sinclair C5 was such a momentous failure when released in 1985, was becuase the 250W electric motor was so under-powered, but then that was (and I think still is) the 'legal' limit for electric vehicles here in the UK (without tax, licence etc.)
```

---
## \#21 Posted by: ian.davidson Posted at: 2016-09-14T06:32:13.017Z Reads: 190

```
@devin @elkick @kampfhahn Thanks again to everyone in this thread, I'll post some screen-shots of my BLDC setup at the weekend, as the Sinclair C5 is left somewhere else.

I have my laptop with BLDC on here, but I need to 'read' the settings off the VESC again before I can post them. I'll do so at the weekend. I sincerely appreciate everyone's input here... I'm so happy to have found you guys! :slight_smile:
```

---
## \#22 Posted by: kampfhahn Posted at: 2016-09-14T06:33:00.028Z Reads: 190

```
The max. power of a motor doesn´t say a word about how much torque it can provide. There are other factors like the magnets and windings  that affect the ammount of torque.

Nevertheless, regarding the crazy reduction of 14.4:1, i´m sure that it´s not a torque/power but just a setup issue here. Like @elkick mentioned, we could help you best when you´d post some screens of your setup.
```

---
## \#23 Posted by: ian.davidson Posted at: 2016-09-14T06:52:23.842Z Reads: 204

```
For the geeks among us (yes, I'm one!) I just thought I'd share a bit more about my Sinclair C5 project. I'm actually turning a 1985 Sinclair C5 into a electric + gas-turbine 'hybrid' Sinclair C5 !!  :D

The gas-turbine part works flawlessly and drives the Sinclair C5 up to 50 MPH (yes it's scary), but the issue with gas-turbine engines is that they have a huge throttle-lag. i.e. you get power 3+ seconds after you've requested it, as it takes time to spool up.

I therefore now have an electric motor (SK3-6374) driving the wheels in parallel with the gas-turbine engine. After 17 MPH (giving the gas-turbine plenty of time to spool up), the electric motor automatically switches off, but is not then back-driven by the gas-turbine due to an inline one-way bearing.

The electric motor 'should' therefore give me instant acceleration from 0-17 MPH and then the gas-turbine seamlessly takes over from there.

Here's is a video of my Sinclair C5 with just the gas-turbine engine (filmed before I had the idea of pairing this up with an electric motor). The audio is quiet, so please turn everything up to the max to hear the engine.
 
https://www.youtube.com/watch?v=EZX_16OojKk
```

---
## \#24 Posted by: longhairedboy Posted at: 2016-09-14T15:01:04.254Z Reads: 184

```
LMAO holy shit i can't beleive i'm seeing a gas turbine sinclair. You just made my day bro. 

I kind of want to build something like this from scratch now.
```

---
## \#25 Posted by: Titoxd10001 Posted at: 2016-09-14T17:07:28.557Z Reads: 171

```
Wow 50mph is insane. What I meant to say is brushless has more power for sure but from my experience brushed motors do better at slow speeds. Most people push to start on their boards and sensors help for slow speeds like evolve and boosted. Almost 300lbs is a lot of load on one vesc to start from stop imo.
```

---
## \#26 Posted by: ian.davidson Posted at: 2016-09-14T20:06:42.076Z Reads: 175

```
@longhairedboy @Titoxd10001 Yes, it's a little crazy (not worth doing otherwise :slight_smile: ) but it all works perfectly... All that is but what 'should' be the easiest part, the electric motor.

I'll certainly post screen-grabs of my BLDC settings at the weekend, so maybe (hopefully) someone can diagnose an issue from these. Fingers crossed!

As a couple of people have suggested, maybe I need to invest in a sensored motor. Has anyone tried the sensor boards on the below website? The website says they will work with SK3-63 motors.

http://e0designs.com/products/hall-effect-sensor-adapter/

With my original Castle Creations 200A ESC, the motor jumping/stuttering/cogging was very noticeable/audible (didn't sound nice) but it did take off like a rocket from a stand-still. The CC logging software did though register (at times) 300A, although the motor (only rated at 80A) seemed to handle it fine. I guess it was only ever in short bursts so it wasn't an issue.

Therefore, maybe if I simply upped the VESC limits to 200A, I might get the desired result?
```

---
## \#27 Posted by: Titoxd10001 Posted at: 2016-09-17T03:57:18.100Z Reads: 162

```
Have you done more testing? I think you're asking to much from a vesc. Eboards have urethane wheels that roll by just looking at them wrong so they're easy on the vesc. I assume those wheels are rubber so I would venture to say the Sinclair is more like some of the MTBs on here. I think the general consensus is that the vesc 4.xx can't handle the amp output as some of the car escs. Also the weight might be an issue. Are you able to test if the Sinclair is able to start well without a rider? I'm not an expert  but this is the information I gathered from this forum and some of the veterans might have more input. I want this project to succeed because it looks awesome
```

---
## \#28 Posted by: ian.davidson Posted at: 2016-09-17T15:33:01.193Z Reads: 178

```
@Titoxd10001 Thank you for thoughts and support!
 
What I'm asking of VESC though is really no different to powering an electric bicycle... does the VESC get used for electric bikes too? 

Trying it today, the sensation I get is that the VESC/motor combination has plenty of power, if only the motor wasn't jumping/stuttering insistently and the VESC cutting-out when I quickly open the throttle. 

I've not yet workout 'what' is triggering the cut-out; current-draw or VESC temperature. The VESC doesn't feel hot (or even warm) and it's so fast to cut-out when the throttle is quickly opened that I don't think it really has time to get hot.

Below are screen-grabs of my current settings...

<img src="/uploads/db1493/original/3X/3/8/38b4ce66bb28c6ca55b2f0dc7abc8b7c7cbf1d08.PNG" width="690" height="414"><img src="/uploads/db1493/original/3X/0/d/0d811d0fcfeb3f5bb534672c7132db0a933e167f.PNG" width="690" height="414"><img src="/uploads/db1493/original/3X/4/0/40cffbaed13a6535c9a50a76704743e6ca2e3b80.PNG" width="690" height="414"><img src="/uploads/db1493/original/3X/d/a/daa4088d6f37521a35b2b121a22c524acaee7b33.PNG" width="690" height="414"><img src="/uploads/db1493/original/3X/3/6/360abc5b8875f6e7742d27958e6954f75669fc91.PNG" width="690" height="414">
```

---
## \#29 Posted by: elkick Posted at: 2016-09-17T18:07:32.368Z Reads: 140

```
You are having the max current ramp step bug in your firmware. You should update your VESC with the new bug free version of 2.18.
```

---
## \#30 Posted by: kampfhahn Posted at: 2016-09-17T18:20:07.301Z Reads: 135

```
Are two different 2.18 out there?
```

---
## \#31 Posted by: michaeld33 Posted at: 2016-09-17T18:21:15.693Z Reads: 136

```
I have a problem with my hub motors with a VESC which won't let it work unless you give it a push to start it, without it, it just jitters. It has to do with the MAX CURRENT RAMP STEP.
```

---
## \#32 Posted by: elkick Posted at: 2016-09-17T18:33:36.348Z Reads: 138

```
There was an error in the first version end of June on GitHub. It has been corrected beginning of July.
```

---
## \#33 Posted by: ian.davidson Posted at: 2016-09-17T18:41:20.733Z Reads: 139

```
Thank you again everyone!

So this is the correct link for latest 2.18 firmware? http://vesc.net.au/BLDC-TOOL/Firmware/
```

---
## \#34 Posted by: elkick Posted at: 2016-09-17T19:03:05.360Z Reads: 143

```
Yes, that one will work.

You might need to rename the 4.10 version to VESC_default.bin.
```

---
## \#35 Posted by: ian.davidson Posted at: 2016-09-18T12:05:03.916Z Reads: 148

```
I've updated my VESC to the latest 2.18 firmware and while it does seem better (must less susceptible to tripping out), it's still stuttering A LOT. You can definitely feel that the 'potential' of power is there, but it's so hard to deploy because of all the motor stutter.

As a few have already suggested, I'm now convinced for this project a quality **sensored** motor is needed.

Therefore, could I please ask what is the current 'top brand' of low KV sensored motors? :)

I'm looking for something around 2000W in the 150-200kv range and one which is already known to play nicely with the VESC. I will be running it off 8S (32V).
```

---
## \#36 Posted by: i2oadsweepei2 Posted at: 2016-09-18T12:54:12.908Z Reads: 145

```
Diyelectricskateboard has 170kv and 190kv 6355 sensors motors in stock. Also 6374 190kv and maybe 170kv on the way. Not sure about the 170kv's. 
category/electric-skateboard-parts/electric-skateboard-motors/

This is a pretty interesting project. I know this is a help thread, but will you be making a build thread so we can see under the hood?

This may sound dumb and the circumstances are different as well as the equipment (high powered rc cars). I've only experienced cogging with poor solder joints and in some cases arcing, but those were wet or damp conditions. Is there any chance of a cold solder joint? Just asking.

Kevin
```

---
## \#37 Posted by: psychotiller Posted at: 2016-09-18T13:44:03.737Z Reads: 148

```
This is bad ass!!!! I think you should seriously put hall sensors in your motor. Once you do, you'll feel smooth start ups and acceration. The other alternative as mentioned above would be to just buy a sensored motor from Torque.
```

---
## \#38 Posted by: ian.davidson Posted at: 2016-09-18T21:01:59.863Z Reads: 166

```
Thanks for the link and info on  @i2oadsweepei2 !!

I've just found this motor here in the UK too, but they're currently out of stock. Does anyone have any experience of Alienpowersystems.com - good company/products?

http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-170kv-3200w/

I'm happy all of the power connections are secure. The 'cogging' / 'shuttering' is (I imagine) a consequence of the motor just no knowing in which direction to turn, until it's turning (catch 22). A sensored motor should resolve this.

I'll definitely do a in-depth video of how it all works when it's finished. Thanks to the help of everyone here, hopefully shouldn't be too long now :slight_smile:
```

---
## \#39 Posted by: kampfhahn Posted at: 2016-09-19T07:11:51.524Z Reads: 168

```
Refering to @devin s "available power near 0 rpm" theory i still think that you don´t need a new motor to get this thing running but only the right settings. You already did the FOC detection and with this values @devin maybe can calculate the right settings to get as much watts as possible even with low rpms.
```

---
## \#40 Posted by: ian.davidson Posted at: 2016-09-30T21:03:46.629Z Reads: 162

```
My new **sensored** motor arrived today! :slight_smile: 

http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-130kv-3200w/

However, I now see I need to buy a suitable cable to mate the sensor connector from the motor to the one on the VESC, (as they're currently both the same gender) so I doubt I'll have a solution to this, this weekend. Doh!
```

---
## \#41 Posted by: RogerD Posted at: 2016-10-01T09:03:37.423Z Reads: 170

```
I don't think your jerkiness is a symptom of over current ( thermal protection). I built a board that overheated and the cut offs are total. Not jerky. The esc stops completely then requires a wait before it will go again.

Jerky indicates a configuration problem or a loose motor wire.  I tested an esc with a servo tester with no issues.

I'm also surprised that sensored motors are being recommended when the whole point of the vesc is smooth starts with unsensored motors...   You can get smooth starts with sensored car escs and motors....

I'm 90kg. One of the boards I ride is 20kg. Single sk6364 245 kv motor. Vesc. Smooth and powerful.
```

---
## \#42 Posted by: ian.davidson Posted at: 2016-10-01T16:43:18.243Z Reads: 165

```
Agreed. The jerky/coggy issue I'm encountering is not over-current, but I can induce the VESC over-current cut-out if I'm really brutal with the accelerator. As you say, it cuts-out completely and then you have to wait a 2-3 seconds for it to start again.

I've now tried the below motors (all off 8S) and they all act the same. I have also tried the VESC and a Castle Creations 200A ESC and there's no two ways about it, the CC 200 ESC works much better (but still not perfect), but then the data-logging tools for the CC ESC report it passing up to 300A to the motor!

* Turnigy SK3-6364-245kv	
* Turnigy SK3-6374-168kv
* Alien 6374 130kv

My new Alien 6374 130kv motor has hall-sensors, but I've yet to try this crucial part as I've just realised that the mating half for the 6-pin JST-PH sensor connector on the VESC seems to be rather uncommon, and from eBay available from China only?

http://www.ebay.co.uk/itm/361530056190
```

---
## \#43 Posted by: elkick Posted at: 2016-10-01T16:52:42.836Z Reads: 155

```
I could send you those if you want me to. But you'd owe me a beer! :slight_smile:
```

---
## \#44 Posted by: ian.davidson Posted at: 2016-10-01T17:04:36.776Z Reads: 152

```
I've just found the cable on your website - perfect !! :)

Ahh, I've now noticed the shipping cost to the UK :worried:
```

---
## \#45 Posted by: elkick Posted at: 2016-10-01T17:08:42.687Z Reads: 155

```
No way, we'll have to postpone that beer though!  I'll send you one on Monday anyway. It's public holiday here on Monday, so it will be processed by German post on Tuesday, but still better than China. :slight_smile:

You don't have order it, I'll send you that for free (there's a min. order limit in the shop system).
```

---
## \#46 Posted by: ian.davidson Posted at: 2016-10-01T17:11:32.492Z Reads: 159

```
Wow, that really is super-kind of you - thank you so very, very much!

I would be delighted to pay, it's just the shipping cost for a tiny cable had me a little concerned ;)
```

---
## \#47 Posted by: ian.davidson Posted at: 2016-10-02T08:20:09.061Z Reads: 176

```
I've just found these **before** (no sensors) and **after** (sensors) videos with the VESC, so my hopes are high!

**No sensors**
https://www.youtube.com/watch?v=g480W5hZhpc

**Sensors**
https://www.youtube.com/watch?v=a5hTa3RwJjY
```

---
## \#48 Posted by: ian.davidson Posted at: 2016-10-15T17:51:01.244Z Reads: 162

```
Thanks to the very kind David from esk8.de, I now have a mating-half cable assembly to the VESC PCB's hall sensor connector! :slight_smile: 

I neatly spliced this inline with the sensor wires on my Alien 6374 130kv motor, making sure +5v (pin 1 - red) and GND (pin 6 - black) were at the correct ends of the connector. However, with no steer on the 4 remaining wires (white, yellow, green, blue) I simply matched these to the same colour wires that were on the Alien 6374 motor.

Clicking "Measure" under "Detect Hall Sensor" caused the motor to slowly rotate in one direction and then again in reverse, but sadly always returned a - hall sensors not detected - type error message.

I tried this several times with the same result, so unplugged the hall sensor connector from the VESC and pondered for a bit...

I truly can not think of anything I might have done wrong after this, but since removing this connector something has clearly gone awry, as I think my VESC has died!

Albeit for a yellow LED my VESC now does nothing and the ARM CPU (with the QC PASSED sticker on) gets extremely hot! Has anyone else experienced a VESC failure result in this CPU getting hot? :worried: 

<img src="/uploads/db1493/original/3X/e/5/e513ad6c35177435c2721d7aff949d7e419e08fa.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/9/e/9ef025bad5ac8d3cdebf568c711a10bbb704f2fd.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/5/5/55a4d870757afcea73e30a5c803bcec60d9e7ad6.JPG" width="666" height="500"

<img src="/uploads/db1493/original/3X/3/5/354d78ea8a234afe6b23df990f15b05582b86937.JPG" width="666" height="500">
```

---
## \#49 Posted by: elkick Posted at: 2016-10-15T18:27:59.733Z Reads: 151

```
Normally mixing up the sensor cables should not have that effect.

Since APS is using the same factory to produce their motors, it might be that our layout should work:

http://www.esk8.de/tutorials-d-e-f/hall-sensor-configuration/

Their color coding was very weird until some weeks ago!
```

---
## \#50 Posted by: ian.davidson Posted at: 2016-10-16T06:39:13.291Z Reads: 149

```
Many thanks again, I'll do some more testing with the insight you've kindly provided.

My motor arrived on 19th Sept, so I'm 'hoping' it aligns with your "after 01 Sept" diagram, as the "before 01 Sept" diagram (showing Red being GND and Yellow being +5v) might well have been the cause of (I think) my now dead VESC
```

---
## \#51 Posted by: Titoxd10001 Posted at: 2016-10-16T07:26:58.200Z Reads: 154

```
Have you seen this https://youtu.be/ZDW6k__ms6M
```

---
## \#52 Posted by: ian.davidson Posted at: 2016-11-12T16:58:34.832Z Reads: 151

```
So the challenges continue… so I’m seeking some more advice from this fab forum. :)

My new Alien 6375 130kv 'sensored' motor is much smoother, especially when pulling away from standstill. FOC is also much nicer than BLDC, but in my enthusiasm I upped the “Motor max” current too far and blew one of the power transistors. 100% my fault – Doh!

I ordered another VESC and everything was fine for about a minute until I blew its 5v regulator circuit. Again 100% my own fault;  a bit esoteric, but I shouldn’t have had the VESC’s 5v (red wire) connected to the rest of the Sinclair’s C5 5v circuit. A dumb oversight on my part.

So I have ANOTHER new VESC, but am now getting the following 2 oddities…

* I can connect to the VESC via USB fine; read settings, write settings and log realtime data – all fine! However, the moment any throttle input is given (either manually, or by one of the VESC commands e.g. the BLDC tab “Start detection”) the VESC reboots. It does this even with no motor connected. I’ve tried it off 10S and 5S, no difference – the moment any throttle input is given, the VESC just reboots. :confused:

* The mosfet temperature sensor report -75’C !?

Any thoughts folks?

Many thanks!
```

---
## \#53 Posted by: chinzw Posted at: 2016-11-15T07:10:39.741Z Reads: 140

```
First, i think at this point you should get a rework station, for less than 100$ you can get one, plus a few drv8302 (5$ a pop) and a few stm32 (10$ a pop), then just replace the blown ones and you get back 2 working VESC.

Im not sure why you're getting negative readings on the temp, but its either a faulty NTC Thermistor or the STM32 chip.
```

---
## \#54 Posted by: rtasca Posted at: 2016-11-15T08:47:56.627Z Reads: 135

```
Hey, I know you from somewhere, ha.  http://fpvlab.com/forums/showthread.php?7083-ZII-Project-Hello-Kitty
```

---
## \#55 Posted by: ian.davidson Posted at: 2016-11-15T21:15:39.935Z Reads: 126

```
Ha! Busted! :)
```

---
## \#56 Posted by: ian.davidson Posted at: 2016-11-15T21:39:06.927Z Reads: 132

```
Many thanks chinzw for your input, it's greatly appreciated.

I am now on my 4th dead/faulty VESC. :pensive:

1. After some time the ARM CPU just died. The CPU now gets VERY hot. When working, the temperature read -75’C
2. I upped the max current too far and blew a power transistor. MY FAULT
3. I didn't disconnect the VESC’s 5v output and it was wired in parallel with another 5v supply. MY FAULT
4. USB disconnects the moment ANY throttle input is given. Temperature reads -75’C

I accept responsibility for 2 of the 4 failures (although #3 really shouldn't have killed an ESC), but 2 were absolutely of not my doing.

Since the VESC is open-source, is it possible there are some manufacturers who simply don't have the same quality control as others?

Is there a 'gold standard' of VESC supplier?
```

---
## \#57 Posted by: chinzw Posted at: 2016-11-15T22:12:50.195Z Reads: 123

```
I've paralleled 5v from arduino to vesc a bunch of times while fiddling and developing my battery monitor, still going strong.

Does the vesc that disconnects from usb still power the motor? Or apart from disconnecting from usb it also doesnt work? Try measuring the 5v rail when you push the throttle and watch for any drop in voltage.

The best VESC manufacturer is @chaka (Ollin board). I dont have one of his vescs, but its common consensus in the forums that his are the best quality and he has amazing warranty and customer service.
```

---
## \#58 Posted by: ian.davidson Posted at: 2016-11-16T21:07:43.308Z Reads: 126

```
I absolutely agree. Although not recommended, paralleling up the +5v supply from different sources rarely does any harm, but sadly it did with one of my VESCs. After a few minutes it just died and probing the PCB, no longer could I find any +5v on it.

With my current VESC (with the USB and temperature issue) I guess I’ve not actually tried to see if it powers the motor… but I doubt it.

Even with no motor attached (therefore no current load) any throttle input (either manually or from BLDC) causes the VESC to immediately reboot. I’ve put a scope on the +5v and it doesn’t drop at any stage. The reboot is almost like a software reboot – a firmware crash if you will.

Thanks for the tip-off about @chaka I’ll certainly take a look at those, but I’m now very wary of the VESC having spent £500 and not really got a lot.

I see Alien do some large, sensored, ESCs. Maybe I need to look at one of those, but the logging capabilities of BLDC are outstanding and hard to walk away from.

http://alienpowersystem.com/product-category/esc/ev-esc/
```

---
## \#59 Posted by: chaka Posted at: 2016-11-16T22:13:03.127Z Reads: 133

```
I am a little too pressed for time to read this entire thread but please don't let your first impression with the VESC get you down. There are huge differences in quality of manufacturing in open source hardware.  If built with care the VESC is very robust and reliable.
```

---
## \#60 Posted by: ian.davidson Posted at: 2017-01-20T21:44:53.147Z Reads: 125

```
If this post is better placed elsewhere, please say…

Having had 4 x VESC die (2 x my fault, 2 x sub-standard VESC) I decided to change tact and buy a completely different speed controller. This time I bought a KLS6018S from Kelly Controls

http://kellycontroller.com/kls6018s24v-60v240asinusoidal-brushless-motor-controller-p-1339.html

Alas though, the challenges continue, but thanks to the brilliant post-sales support from Kelly Controls we’ve realised why it’s not working…

With my Alien 6374 sensored motor there appears to be a big offset between the hall-sensor pulse and the back EMF waveform. The hall-sensor pulse should start where the waveform passes 0v and end where the waveform passes back through 0v again. From the scope photo below, it's clear this isn't the case.

Does anyone have any experience on this to confirm that what I'm seeing below (i.e. this notable offset) definitely isn't right?

<img src="/uploads/db1493/original/3X/9/c/9c6f8e9149692ecab9747a455b7787c64e757ec0.jpg" width="666" height="500">

I took the motor apart, but the hall-sensor PCB is actually glued into place. Even if I could rotate it, I think the hall-senor would then hit into the windings. i.e. it's current rotational position is really the only place it can be.

<img src="/uploads/db1493/original/3X/c/a/ca190f723d89b35ef7ce695acddf27e491ed105e.jpg" width="666" height="500">
```

---
## \#61 Posted by: ian.davidson Posted at: 2017-01-21T16:19:24.234Z Reads: 118

```
STOP PRESS: I've managed to rotate the PCB holding the 3 hall-sensors just a few millimeters and now the hall-sensor pulse and the back EMF waveform are perfectly aligned... fingers crossed! :slight_smile:<img src="/uploads/db1493/original/3X/7/4/74559833922614d9443c68fb4861789cddc133ee.JPG" width="666" height="500">
```

---
## \#62 Posted by: bigben Posted at: 2017-01-21T17:52:46.499Z Reads: 121

```
Good luck and fingers crossed!
```

---
## \#63 Posted by: ian.davidson Posted at: 2017-01-23T07:42:50.631Z Reads: 121

```
That was it... it now works !! :smile:

The KLS6018S from Kelly Controls drives this motor super-smoothly; it's low-RPM, but high torque control is wonderful. I can set the throttle at 10% and the Sinclair C5 will crawl over rough-grass and up hills without me having to apply any sporadic extra throttle. 

I need to integrate/blend the control of the electric motor in with the gas-turbine engine, but since I now have the motor under control, this shouldn't be too difficult.

It makes me wonder though if some of my VESC failings could have been due to the hall-sensor misalignment in this motor, as the VESC surely can't have been able to drive it efficiently like this.
```

---
## \#64 Posted by: banjaxxed Posted at: 2017-12-05T10:45:49.417Z Reads: 60

```
Sorry to dig this up from the crypt but there may be others like myself who pondered how to do this and the es8.de has the perfect answers

http://www.esk8.de/tutorials-d-e-f/hall-sensor-configuration/
```

---
