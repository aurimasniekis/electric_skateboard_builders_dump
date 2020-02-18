# (UPDATE)Not enough power or lost of it? ENERTION BUILD

### Replies: 81 Views: 4326

## \#1 Posted by: joeadams101 Posted at: 2016-08-04T05:47:16.495Z Reads: 211

```
**2nd UPDATE PLEASE HELP** After adjusting the settings again... Charged up my board and decided to test it out, praying that everything will be fine now. Current Weather 98 F. I Changed my Max Motor from 60 to 45, I kept everything else the same. Thinking that might help the "overheating" issue. After cruising for 5 minutes literally, started loosing power. Will not make uphills at all(flats was fine but a bit of uphill and started dying). The motor was very hot, I could not keep my hand for more than 3 seconds. I seriously feel that there is something wrong with the numbers in the programming of the VESC or this motor doesn't play well with my setup(although Enertion advertises it does works, but haven't provided the numbers as to what input in the Vesc settings to make it a stable system) I have provided answers to all the question (wheel size, rider weight, motor, battery(all down below)) On top of that I started having weird behaviors from the board, it was accelrating it self and such(see the 2nd video below).  I am running out of answers, someone please help. Here is a video of it happening and pics of my set up again... 

<img src="/uploads/db1493/original/2X/8/8d5bea57d9972a319836f471f4cf7460121b4250.JPG" width="666" height="500">

<img src="/uploads/db1493/original/2X/2/2f1ae72fec5b44563b6b7c7dbf8deabc220ffda3.JPG" width="666" height="500">


Videos:
https://youtu.be/SeiRkaW-270
https://youtu.be/orkakY0zvi8
https://youtu.be/4CVONzfYRjM




**_UPDATE_**: I went cruising after having adjust the VESC settings like @onloop suggested. Motor max current : 60 A, battery max current: 50A  and battery cutoff start 33 V. Everything was going fine and after about 15-20 minutes starrted going uphill and again I was litle throttle in and went full throttle and no change it kept getting slower and slower. I stepped off the board for about 5 minutes and went on flat and it was working fine again.... I really don't know what else to try but this is getting frustrated since I haven't been able to enjoy the board ever since I got it. Any suggestions? Battery was at 40%.



Original:
Hey guys my board is having lost of power in my opinion. I was crushing around no problems(was going uphill for like 5 mins not too steep at all), after 10-20 minutes, i will be half throttle and usually when i push it to full I will feel the impulse like its got more power, this time it just stayed at the same speed and going a little uphill just got to the point where it couldn't continue anymore. I turned off the board and control and turned them back on and bam power was back but then it lost it again. Has this happened to anyone? Battery was at 50%. Using Space cell 3 , exertion standard vest, exertion 6372 r spec and gt2b control. Here are my specs.


<img src="/uploads/db1493/original/2X/b/b0e58a1d4cb54aec285f4974b3ad3f2e3a96f80b.png" width="690" height="409">
<img src="/uploads/db1493/original/2X/4/450c0ccd513d4f097a9e25bbd4b9831e191012ab.png" width="690" height="369">
<img src="/uploads/db1493/original/2X/1/18e8e54993ebb0e02f304d773187ce6b8bd61581.png" width="690" height="366">
```

---
## \#2 Posted by: onloop Posted at: 2016-08-04T06:00:47.061Z Reads: 184

```
turn up your motor max current to 60A
turn your battery max current to 50A
```

---
## \#3 Posted by: Namasaki Posted at: 2016-08-04T06:38:11.422Z Reads: 179

```
Do you set the battery max current to match the batteries constant current capability or its peak current capability?
```

---
## \#4 Posted by: onloop Posted at: 2016-08-04T06:40:38.713Z Reads: 176

```

constant, otherwise it could damage the battery
```

---
## \#5 Posted by: joeadams101 Posted at: 2016-08-04T06:49:39.319Z Reads: 171

```
Sorry those specs were outdated. The current motor max is at 60A the battery was at 40A. So i put the battery at 50A anything else I might need to change?
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-04T06:55:41.551Z Reads: 164

```
did you solder on female 5.5mm bullets yet? Or are you still plugging the bare leads into the male connectors?
```

---
## \#7 Posted by: joeadams101 Posted at: 2016-08-04T06:56:36.027Z Reads: 164

```
they are soldered.
```

---
## \#8 Posted by: onloop Posted at: 2016-08-04T07:42:09.459Z Reads: 158

```
battery cut off start is really high.

set it at 33v
```

---
## \#9 Posted by: Mrmoonlight Posted at: 2016-08-04T18:14:23.217Z Reads: 133

```
I'm having the same issue. Same problem with braking that you mentioned in another post too. 
Tried a bunch of different settings and matched Runplayback's who has my exact setup and still having the same problems.

My brakes cut out when my battery is fully charged. Same thing, brakes for a fraction of a second, then nothing. I tested it with my computer attached and was able to get a fault reading. Once I'm below 90%, my brakes work fine at -40 regen. 

For power cutting out, my VESC is running hot. Heatsinks helped, but haven't solved the issue. Working with Enertion support to try and figure it out, but haven't found a solution yet. They said they haven't seen any such issues and to open up a thread to see if anyone in the community has any insight. So far no resolution, but since it seems you are experiencing something similar it might help us get to the bottom of this.

Here's my thread:
http://www.electric-skateboard.builders/t/braking-issue-with-fully-charged-battery/6730
```

---
## \#10 Posted by: joeadams101 Posted at: 2016-08-04T20:28:52.822Z Reads: 119

```
Yup you are having the same Issues I am. The brakes work fine after adjusting the max input voltage. Still having the loose of
Power issue. Will try again tonight with @onloop recommendation of bat max
```

---
## \#11 Posted by: joeadams101 Posted at: 2016-08-05T05:35:04.941Z Reads: 114

```
**_UPDATE_**: I went cruising after having adjust the VESC settings like @onloop suggested. Motor max current : 60 A, battery max current: 50A and battery cutoff start 33 V. Everything was going fine and after about 15-20 minutes starrted going uphill and again I was litle throttle in and went full throttle and no change it kept getting slower and slower. I stepped off the board for about 5 minutes and went on flat and it was working fine again.... I really don't know what else to try but this is getting frustrated since I haven't been able to enjoy the board ever since I got it. Any suggestions? Battery was at 40%.
```

---
## \#12 Posted by: michaelcpg Posted at: 2016-08-05T07:27:02.896Z Reads: 112

```
If it's anything like what has been happening to me with my single 6374 motor then it could well be the VESC overheating when going up longer hills. If you haven't already, then put some heatsinks on your VESC. From my experience, FOC mode seems to produce noticeably less heat than BLDC mode but you run the risk of getting a DRV fault like many others in this forum have, including myself.
```

---
## \#13 Posted by: Alex Posted at: 2016-08-05T16:18:41.022Z Reads: 110

```
sounds like you need some heat sinks
```

---
## \#14 Posted by: joeadams101 Posted at: 2016-08-06T23:43:05.911Z Reads: 108

```
Anyone can tell me some vesc settings to prevent this overhearting issue? I dont care if I loose power.
```

---
## \#15 Posted by: onloop Posted at: 2016-08-06T23:52:56.330Z Reads: 112

```
answer these questions.

rider weight?
wheel size?
wheel pulley teeth?
motor pulley teeth?

ALSO, picture of your setup.

Have you watched this?
https://www.youtube.com/watch?v=eakga9Bzj9E
```

---
## \#16 Posted by: joeadams101 Posted at: 2016-08-06T23:55:55.629Z Reads: 110

```
I have watched it. Was riding only flat today and it happened. @onloop 

170 lbs
83mm
Enertion 12m pulley
Enertion 6372 r motor
Enertion space cell 3 with enertion enclosing
Enertion vesc

Pictures of vesc settings in original thread.

<img src="/uploads/db1493/original/2X/e/e01194cb4c54bbb20fafc3901fa24abd5b8faf0a.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/8/8ffc0920b420a0c45bd51c71c5f0298652e9fd90.jpg" width="375" height="500">
```

---
## \#17 Posted by: t1m0007 Posted at: 2016-08-07T01:03:49.871Z Reads: 102

```
Have you run some bench tests on this? Didn't you recent have to pull the motor apart?-- have you done another motor detection since?
```

---
## \#18 Posted by: joeadams101 Posted at: 2016-08-07T01:04:41.357Z Reads: 100

```
that was my friends motor. I havent. How do I do that?
```

---
## \#19 Posted by: Dedbny Posted at: 2016-08-07T01:10:07.761Z Reads: 100

```
I wouldnt have thought for your weight it wouldnt have an issue going up hills. Those motors are torque.
```

---
## \#20 Posted by: joeadams101 Posted at: 2016-08-07T01:10:35.330Z Reads: 103

```
It happened on flat today...
```

---
## \#21 Posted by: Dedbny Posted at: 2016-08-07T01:40:57.648Z Reads: 107

```
If you dont care about loss of power maybe reduce erpm max. Might help.


24,500 erpm will get 20-24km/h 
36,000 erpm is 30km/h 
18,000erpm and amp limit at 20amp will give for a very basic board 16km/h not huge acceleration power.
```

---
## \#22 Posted by: joeadams101 Posted at: 2016-08-07T01:47:23.722Z Reads: 105

```
Whats the difference between ppm and ppm/uart? I had it on ppm/uart and it was working fine before
```

---
## \#23 Posted by: Jinra Posted at: 2016-08-07T01:56:31.567Z Reads: 107

```
Nice motor connections! Much better than what you showed me before :) Make sure the belt is not too tight. Too tight = more stress = more heat. You can run motor detection can be done in the BLDC/FOC page on BLDC tool. You need to do this anytime you change motors, or during initial setup.
```

---
## \#24 Posted by: joeadams101 Posted at: 2016-08-07T02:09:39.020Z Reads: 113

```
@Jinra i got these results

<img src="/uploads/db1493/original/2X/4/432c4cf8f70ae1167241bb3460e96ee6289ccaea.png" width="689" height="80">
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-07T02:14:18.230Z Reads: 109

```
Great! now put the intergrator limit and BEMF coupling results in the corresponding fields above. I would run the test 5 times and average it out. Round the integrator limit down to the closest multiple of 5 and the BEMF coupling down to the closest multiple of 50.
```

---
## \#26 Posted by: joeadams101 Posted at: 2016-08-07T02:18:19.024Z Reads: 110

```
@Jinra    okay so this is what I have right now. Replacing with average. The right side correct? Also could this be contributing to the heating issue?

<img src="/uploads/db1493/original/2X/2/2ae09eb3f0d0591d3cd2e15673c884e55f20a0ac.png" width="690" height="452">
```

---
## \#27 Posted by: Jinra Posted at: 2016-08-07T02:19:32.055Z Reads: 97

```
your BEMF coupling is varying by 100? I'd re-run detection with no load (no pulleys or belts) on the motor for more accurate results.
```

---
## \#28 Posted by: joeadams101 Posted at: 2016-08-07T02:27:30.876Z Reads: 98

```
I took everything off. After 6 times the avg is 610
```

---
## \#29 Posted by: Jinra Posted at: 2016-08-07T02:28:34.259Z Reads: 101

```
Cool, so set the coupling to 600. It could be contributing to why it's overheating. It definitely shouldn't be over heating on flats at your weight. Like I said, make sure the belt isn't too tight.
```

---
## \#30 Posted by: joeadams101 Posted at: 2016-08-07T02:29:29.313Z Reads: 101

```
@Jinra alright. The belt is not that tight. Also Do you know the difference between PPM and PPM/UART?
```

---
## \#31 Posted by: Dedbny Posted at: 2016-08-07T02:30:50.268Z Reads: 109

```
Also If your setting your motors erpm any higher the 40k it is better to just tick soft erpm limit as it will be a lot better for the motors.

Suggets you try @Jinra help first. Im no expert. Just my thoughts on maybe trying other options. You need to break the things down as to what might fix it.
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-07T02:32:15.445Z Reads: 108

```
I don't know the technical details, but I know UART is used for bluetooth communications in some boards and ESCs. GT2B uses PPM, so just set it to that. I also noticed your max current ramp gain is too high, set it to .004 and write config. Just FYI there's a glitch on most BLDC tools that will mutliply the value by 10 every time you write in the motor config tab. The default value is .04 which is why you want to set it to .004 before you write.
```

---
## \#33 Posted by: joeadams101 Posted at: 2016-08-07T02:33:47.057Z Reads: 106

```
@Jinra ok adjusting now. What is the erpm stuff? Is it too high right now?
```

---
## \#34 Posted by: Jinra Posted at: 2016-08-07T02:36:16.548Z Reads: 106

```
You're not hitting the eRPM limit, so you're fine. You can limit it if you feel like you're going too fast, but it won't be efficient for your system.
```

---
## \#35 Posted by: joeadams101 Posted at: 2016-08-07T02:37:11.495Z Reads: 109

```
@Jinra  Okay. What set up are you using? I feel I need to adjust the motor setting better to not overheat. What do you think with my setup?
```

---
## \#36 Posted by: Jinra Posted at: 2016-08-07T02:40:14.488Z Reads: 105

```
I use dual OM5065 motors at 10s, so not very relevant to your setup. But something is configured wrong if your VESC is overheating from flats.
```

---
## \#37 Posted by: joeadams101 Posted at: 2016-08-07T02:40:50.595Z Reads: 106

```
@Jinra Yeah thats what I think.....Take a look at my setup again.


<img src="/uploads/db1493/original/2X/b/b4717c0f801b1d7eba7f57f36f92569327476196.png" width="690" height="405">
```

---
## \#38 Posted by: Jinra Posted at: 2016-08-07T02:49:35.641Z Reads: 95

```
That page looks good to me
```

---
## \#39 Posted by: joeadams101 Posted at: 2016-08-07T02:50:51.959Z Reads: 95

```
@Jinra Which other will you like to see?
```

---
## \#40 Posted by: Jinra Posted at: 2016-08-07T02:51:39.269Z Reads: 94

```
as long as you put the int limit and bemf coupling correct I think you're good to go. Try it out.
```

---
## \#41 Posted by: joeadams101 Posted at: 2016-08-07T02:52:16.013Z Reads: 95

```
@Jinra Should I average the int limit?
```

---
## \#42 Posted by: Jinra Posted at: 2016-08-07T02:52:41.376Z Reads: 94

```
Average and round down to the closest 5 like I said
```

---
## \#43 Posted by: joeadams101 Posted at: 2016-08-07T02:59:40.286Z Reads: 92

```
testing now.
```

---
## \#44 Posted by: onloop Posted at: 2016-08-07T04:43:53.704Z Reads: 91

```
make sure there are no internal shorts inside the motor, the way you currently have the phase wires puts more stress onto the motor wires when the trucks turn...

if the motor is shorting it could cause the vesc to overheat.
```

---
## \#45 Posted by: Mrmoonlight Posted at: 2016-08-07T05:27:47.210Z Reads: 92

```
Just wondering since I'm having basically the same issue. This is my first DIY build so I'm a bit new to working through all the VESC settings. Are adjusting ERPM limits, averaging BEMF coupling results,... something that everyone does or should be doing to get their board up and running properly?
```

---
## \#46 Posted by: Jinra Posted at: 2016-08-07T05:31:13.651Z Reads: 92

```
Motor detection is something EVERYONE should be doing for a DIY build. The fields it detects are integrator limit and BEMF coupling which you need to adjust according to detection. eRPM limits can largely be left alone unless you want to go slower at full throttle, or if you're hitting the eRPM celing of ~60k.
```

---
## \#47 Posted by: Mrmoonlight Posted at: 2016-08-07T06:38:00.247Z Reads: 89

```
I've done the motor detection in both BLDC and FOC modes and I just hit apply and didn't manually make any adjustments. I've been running in FOC mode. I seem to be getting better performance over BLDC. Should I be making further adjustments according to the results or should it autofill when I hit apply? I'm on the FW 2.17/2.18 version of BLDC tool. I adjusted my ERPM limits on the App Configuration/PPM tab, but not anywhere else. 

I just feel like I'm missing something somewhere. I've been making a lot of adjustments, checking temps, running tests,... but nothing but adding heatsinks has made any difference and my board is still cutting out on flats. Kind of just wondering if this is a beginner DIY sort of thing and everyone else is just thinking, "yeah, I remember when I went through that." or if I'm having an actual issue. Sort of like when my little sis first starting using strobe lights in her photography. Me and one of my photographer friends had a good laugh when she couldn't figure out why there was a black bar at the bottom of all her images. 

Mainly trying to decide at what point I should start buying additional hardware so I can start swapping parts to isolate the issue or seeing if I need to explore sending some parts in for assessment/repairs.
```

---
## \#48 Posted by: Jinra Posted at: 2016-08-07T06:41:36.669Z Reads: 81

```
Could you remind me what setup you have? Do you have your own thread detailing these issues? Best not to hijack this one.
```

---
## \#49 Posted by: Mrmoonlight Posted at: 2016-08-07T06:49:05.156Z Reads: 81

```
Don't mean to hijack this one. joeadams101 and I are pretty much having the exact same issue although are setups are a little different. Both running a Space Cell 3 and Enertion VESC, but he has the Enertion Motor and I'm using a Carvon V2. I'm also about 35lbs lighter.

My thread is: 
http://www.electric-skateboard.builders/t/braking-issue-with-fully-charged-battery/6730
```

---
## \#50 Posted by: Jinra Posted at: 2016-08-07T06:51:38.614Z Reads: 77

```
Ah I remember this. It seems like yours happens when you brake correct? I think @joeadams101 happens when he accelerates.
```

---
## \#51 Posted by: Mrmoonlight Posted at: 2016-08-07T06:57:41.326Z Reads: 75

```
Braking is one of my issues, but that one is sort of solved. I just have to keep my battery under 90% charge  or keep my regen at -10 or less for my brakes to work. The other issue is the same. After 20min or so of riding, my VESC heats up and power cuts out. Happens much sooner if I do any sort of incline.
```

---
## \#52 Posted by: Jinra Posted at: 2016-08-07T06:59:16.298Z Reads: 74

```
The two problems might be related. Have you done as @elkick suggested and replaced the caps? I have a suspicion myself that you have failing cells in your pack. Do you have another power source to test with? Maybe some lipos?
```

---
## \#53 Posted by: Mrmoonlight Posted at: 2016-08-07T07:08:41.876Z Reads: 78

```
That's my issue. I don't have another setup to test and I don't want to go and start doing major work on my VESC's and void my warranty. Worked with Enertion support and they directed me to open up a thread and see if I could find some additional insight here. It was great advice since I've narrowed down my problem to an overheating VESC and my motor regen settings, but I still haven't found a solution. I know they're busy as all hell over there so it's taking some time, and I don't want to be pushy, but I've had my board setup for over a month and I just wanna ride it!!!
```

---
## \#54 Posted by: Jinra Posted at: 2016-08-07T07:09:38.091Z Reads: 77

```
Could you do me a favor and tell me what voltage your caps are?
```

---
## \#55 Posted by: Mrmoonlight Posted at: 2016-08-07T07:19:49.865Z Reads: 78

```
Unfortunately I don't have my board with me. Only have pics of my VESC, but none of them show the voltage of my Caps
```

---
## \#56 Posted by: Jinra Posted at: 2016-08-07T07:22:12.873Z Reads: 76

```
Hm, I was just wondering if you're running the 50v caps on the VESC compared to the normal 63v ones.
```

---
## \#57 Posted by: Mrmoonlight Posted at: 2016-08-07T07:34:09.326Z Reads: 76

```
Maybe an appropriate time to move this over to my thread. Posting a pic of it there if you can possibly tell from that.
```

---
## \#58 Posted by: joeadams101 Posted at: 2016-08-07T08:24:05.784Z Reads: 79

```
@onloop what will be the correct way to put the phase wires in the space cell enclosure you sell, which is the one I have?
```

---
## \#59 Posted by: Jinra Posted at: 2016-08-07T08:40:40.575Z Reads: 77

```
you want the phase wires going towards the truck and curving back into the space cell.
```

---
## \#60 Posted by: trbt555 Posted at: 2016-08-07T14:02:27.076Z Reads: 75

```
For what it's worth, I had the same issue a few weeks ago. I thought it was overheating but after upping the temp limits with 20degC the issue went away.
I'm guessing calibration of temp sensing was off somehow.
```

---
## \#61 Posted by: Blasto Posted at: 2016-08-07T14:24:08.571Z Reads: 78

```
[quote="trbt555, post:60, topic:7104"]
Upping the temp limits by 20degC the issue went away.
[/quote]

I think this suggestion is worth trying.
```

---
## \#62 Posted by: onloop Posted at: 2016-08-07T14:51:35.033Z Reads: 85

```
Also. (This might sound obvious)  Please make sure your belt isn't too tight. And make sure your wheel nut isn't too tight.. do you use a bearing spacer?

The wheel should feel like It can rotate without too much resistance from the motor. Too tight and you put extra load on motor which equals heat.

The best way to judge belt tightness is to loosen it fully. Now Slowly increase the tension until you feel a difference in tension at the wheel.. The first moment the "feeling" of resistance appears at the wheel you have now just reached the correct tension. There should be no feeling of tightness/resistance.
```

---
## \#63 Posted by: joeadams101 Posted at: 2016-08-07T17:12:38.950Z Reads: 79

```
@trbt555 what was yours originally set to?
```

---
## \#64 Posted by: trbt555 Posted at: 2016-08-07T18:59:19.385Z Reads: 79

```
Currently set to 120°/140°.

I had another similar problem just last night, reduced power with no obvious reason. I checked literally everything but couldn't find the cause.
I eventually swapped out my R-SPEC for a spare one and the problem was solved. I haven't opened it up yet. A bit disappointed the motor gave out so soon, these are not cheap.
```

---
## \#65 Posted by: onloop Posted at: 2016-08-08T00:06:26.411Z Reads: 75

```
[quote="onloop, post:44, topic:7104"]
make sure there are no internal shorts inside the motor,
[/quote]

Check this.
```

---
## \#66 Posted by: Jinra Posted at: 2016-08-08T00:35:20.758Z Reads: 75

```
I had him check this already through PM
```

---
## \#67 Posted by: joeadams101 Posted at: 2016-08-14T01:47:46.023Z Reads: 71

```
BUMP. Original post updated
```

---
## \#68 Posted by: Jinra Posted at: 2016-08-14T01:54:36.440Z Reads: 71

```
Sounds like your esc is overheating. Can you provide the following:

* Your weight
* Gearing ratio
* incline of hills your riding and length of hills

Given that you're able to hold your motor for ~3 seconds, I wouldn't say it's overheating as much as your ESC is. I've had my single motor uphill get pretty hot, but it was still running. I wasn't able to even touch it for a second, the thing was burning!
```

---
## \#69 Posted by: joeadams101 Posted at: 2016-08-14T02:01:38.041Z Reads: 78

```
170lbs
where do I get the gear ratio from?
this street: https://www.google.com/maps/place/22213+Newhall+Ranch+Rd,+Santa+Clarita,+CA+91350/@34.4251442,-118.5217542,191m/data=!3m2!1e3!4b1!4m13!1m7!3m6!1s0x80c287a3276ed123:0x3fa4a00b3b219e2f!2s22497+Breakwater+Way,+Santa+Clarita,+CA+91350!3b1!8m2!3d34.424402!4d-118.522406!3m4!1s0x80c287a2e8b7830b:0x3c56512ada2f95b0!8m2!3d34.424756!4d-118.5251686

ps: I was riding flat at first and i just literally went to the uphill for like 2 minutes.....


and this trail

https://www.google.com/maps/place/Santa+Clara+River+Trail,+Santa+Clarita,+CA+91351/@34.4222055,-118.5176287,191m/data=!3m2!1e3!4b1!4m5!3m4!1s0x80c287bbc18443e9:0x6aa1f858e139b484!8m2!3d34.4222044!4d-118.5170815
```

---
## \#70 Posted by: Jinra Posted at: 2016-08-14T02:09:53.954Z Reads: 72

```
Looks like you're using an Enertion wheel pulley? If so, thats 36T. Whats your motor pulley? I think your riding environment might be too much for a single 55mm motor.
```

---
## \#71 Posted by: joeadams101 Posted at: 2016-08-14T02:21:53.415Z Reads: 71

```
I am using all enertion parts. 6372 motor, enertion wheel pulley, enertion, motor mount, enertion space cell 3, enertion vesc...
```

---
## \#72 Posted by: Jinra Posted at: 2016-08-14T02:27:14.296Z Reads: 64

```
That's a 6372? Looked like a 6355 to me.
```

---
## \#73 Posted by: joeadams101 Posted at: 2016-08-14T02:28:06.580Z Reads: 63

```
yup 6372 lol

suggestions....? I've tried about everything...
```

---
## \#74 Posted by: Jinra Posted at: 2016-08-14T02:53:04.230Z Reads: 59

```
One more thing to check is your belt tension, if it's too tight it'll definitely cause overheating. Try to be as loose as possible without belt skipping at hard brake/acceleration.
```

---
## \#75 Posted by: joeadams101 Posted at: 2016-08-14T03:10:34.679Z Reads: 55

```
Yup I have done that.
```

---
## \#76 Posted by: Jinra Posted at: 2016-08-14T03:14:53.462Z Reads: 63

```
I know you're recording video for testing but try not to throttle when the motor is chugging slowly like that. You can and will break your motor and/or VESC. Try mounting your VESC outside somehow and going for a ride. When you notice the slow down try to see if your VESC is hot. Normal cut off start is 80 degrees. 

I'm guessing that if you try mounting it outside you won't see the problem as early since it's not insulating heat within the enclosure, and would be air cooled by just riding.
```

---
## \#77 Posted by: joeadams101 Posted at: 2016-08-14T03:16:17.433Z Reads: 68

```
Yeah I know, this is the first time I do that just to show. Curious on how to do that...
```

---
## \#78 Posted by: joeadams101 Posted at: 2016-08-14T03:18:03.910Z Reads: 67

```
Wonder a way to cool off the system inside
```

---
## \#79 Posted by: Jinra Posted at: 2016-08-14T03:18:08.452Z Reads: 70

```
The alternative is to get it chugging again and immediately take off the enclosure to check temps. You could use 4 screws instead of 8 to test with.
```

---
## \#80 Posted by: joeadams101 Posted at: 2016-08-14T03:19:11.792Z Reads: 73

```
If it is overheating and I bet it is. I wonder how to fix that issue....
```

---
## \#81 Posted by: Jinra Posted at: 2016-08-14T03:24:04.614Z Reads: 73

```
Going for a dual setup would help significantly. Reducing gearing ratio might help as well. Cheapest option would be to add heat sinks to the Mosfets of the Vesc http://www.ebay.com/itm/30PCS-Aluminum-Heatsink-Cooler-Adhesive-Kit-for-Cooling-Raspberry-Pi-New-/131760090486?hash=item1ead836d76:g:nhoAAOSwZ8ZW8fmY.

Maybe also cut a hole in the enlosure to stick the heat sinks out of.
```

---
