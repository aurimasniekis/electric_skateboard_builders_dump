# Single Drive RaceStar 5065 200KV&#124;FOCBOX&#124;Zippy 8S&#124;90mm

### Replies: 31 Views: 2368

## \#1 Posted by: EastLosMike Posted at: 2017-11-06T21:44:05.650Z Reads: 241

```
My First Build
<img src="/uploads/db1493/original/3X/2/e/2e61f455a3a41db3a4c8310323e862a1fd300899.jpg" width="374" height="500">
-Main Parts-
RaceStar 5065 200KV from Bangood
<img src="/uploads/db1493/original/3X/4/4/44b937e4feac502dcbe7f50a64679a84a6ad572d.jpg" width="374" height="500">

6 Pin JST connector from Amazon (shout out to @darkkevind for help on identifying this connector)

Caliber II 50 Carbon Motor Mount from @thisguyhere
15 mm Complete Kit 36T Drive & 15T motor from @johnny_261

Bigfoot 90mm from Amazon

FOCBOX from @Yummyblobs

Zippy Flightmax 5000MAH 4S 30C x2 in series to 8S 

DIY Fused XT90 AntiSpark LoopKey  50A cartridge FLF fuse from Autozone(Shout out to @rpasichnyk
 for the idea)
<img src="/uploads/db1493/original/3X/b/e/be1c4c5384ab7e87cd7e0e74a2a6418dfd4001c6.jpg" width="187" height="250"><img src="/uploads/db1493/original/3X/0/b/0b2bdbc495bbfc5a7cd444bbc3ffdd46c536bce1.jpg" width="187" height="250">
<img src="/uploads/db1493/original/3X/1/a/1a8dd79b9b525acf7ec1b976664f77cc0085ce12.jpg" height="250" width="187"> <img src="/uploads/db1493/original/3X/c/2/c2264f29ac4bb0c42ff2f381a4ef8480ccca02e5.jpg" width="187" height="250">
Deck 39”X9.5” Double Kicktail (#CMDK39) from StateShred.com

Does anyone have any tips on configuring FOC on a similar 200kv on 8S 5000MAH? I only find configurations for 12S which I will do at a later time.
```

---
## \#2 Posted by: darkkevind Posted at: 2017-11-06T23:12:47.563Z Reads: 216

```
Hey! You're welcome man! :thumbsup:
```

---
## \#3 Posted by: EastLosMike Posted at: 2017-11-07T00:03:25.479Z Reads: 215

```
When you get a chance do you mind Sharing your FOC Configurations you are currently using on your 200KV setup maybe I can use your configuration as a base. :grin:Configuring the VESC and finding a Enclosure is pretty much all that i have pending!:grinning:
```

---
## \#4 Posted by: darkkevind Posted at: 2017-11-07T00:07:33.447Z Reads: 203

```
Yeah no worries mate.

Watch this space re enclosure... I may have something very cool on the horizon ;)
```

---
## \#5 Posted by: egzplicit Posted at: 2017-11-07T00:21:32.075Z Reads: 197

```
I have a dual on the same motor 5065 (but 140kv) running in FOC on focboxes with @Ackmaniac 3.100 firmware. Just use the wizards for motor detection and u should be good.
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-11-07T00:29:57.834Z Reads: 198

```
good to see it's coming together.

FOC config needs to be done for your specific setup, run steps for FOC detection:

https://www.youtube.com/watch?v=xSCEFK7Zljw

also, i was wondering why you have baby hands, but realize it's your kid's:

<img src="/uploads/db1493/original/3X/f/4/f477161a6c694679193576114763a5b3ad4ed2d1.jpg" width="375" height="500">
```

---
## \#7 Posted by: briman05 Posted at: 2017-11-07T01:01:22.020Z Reads: 183

```
Did you use the red 15t gears from banggood that fit this motor?
```

---
## \#8 Posted by: pat.speed Posted at: 2017-11-07T01:50:33.815Z Reads: 171

```
Nope, in the picture it is a black one
```

---
## \#9 Posted by: EastLosMike Posted at: 2017-11-07T07:36:27.707Z Reads: 166

```
Awesome!Thank you.:)
```

---
## \#10 Posted by: EastLosMike Posted at: 2017-11-07T07:54:37.103Z Reads: 172

```
I tied the default settings but I am not sure if the Battery cutoff start i have is accurate for my 8S setup (5,000MAH 4S 30C 30C x2)

I try to detect/ calculate the Parameters (Measure R and L, Measure A(The motor spins like the video shared by @thisguyhere ) Calc CC Apply>Apply>Write configuration.

When I try using the arrows to spin the motor I get a faint noise and a weak wiggle with absolutely no spin, which leads me to believe something is not right.
<img src="/uploads/db1493/original/3X/a/c/acfe87989890b59ed0dc4d1245bfb24f5cc8d8d3.png" width="690" height="392"><img src="/uploads/db1493/original/3X/1/7/172d60a57bcce63cf4e4d383e03b1a1ed3a1041a.png" width="690" height="400">

@briman05
No I will  be using the pulley from the complete kit i purchased from @johnny_261 

@thisguyhere lol I did not notice my little guys hand until after you pointed it out.
```

---
## \#11 Posted by: egzplicit Posted at: 2017-11-07T09:12:30.871Z Reads: 140

```
[quote="EastLosMike, post:10, topic:37559"]
When I try using the arrows to spin the motor I get a faint noise and a weak wiggle with absolutely no spin, which leads me to believe something is not right.
[/quote]

Did u have the remote connected as well? If I remember correctly I had the same issues using the keyboard while the remote was connected. If you do, try disabling the control mode in the ppm tab. My slave would spin just fine but master vesc only worked from the keyboard once I disabled the remote.

Edited: did you also do the hall sensors detection?
```

---
## \#12 Posted by: egzplicit Posted at: 2017-11-07T09:16:34.197Z Reads: 137

```
@briman05 I used those and they work well. I had to loctite them to the motor shaft (and use a grub screw as well), otherwise I would get a little play and ticking noise. Could be because my grub screw was pointy and the space in the shaft was wider than the screw end. I’ve filled down the pointy bit but also used loctite for good measure.
```

---
## \#13 Posted by: briman05 Posted at: 2017-11-07T13:56:07.793Z Reads: 139

```
The only thing that keeps me from not using the one that bang good sells is that all the others have a key slot and it will not fit the motor shaft because all the gears have a key slot on top of the full shaft head.  You would be solely relying on that screw not snapping in the gear.  I had planned on using loctite on the motor shaft plus on the screw.  I just need to know the size  of set screw I would need.
```

---
## \#14 Posted by: EastLosMike Posted at: 2017-11-07T17:28:27.413Z Reads: 146

```
I made sure I had the mini control off before I setup the motor detection. Should I unplug the receiver completely? 

I didn't get to the hall sensors detection 

These are the PPM tab setting ( I apologize for the crappy pic I took it really quick b4 heading to work)
<img src="/uploads/db1493/original/3X/b/e/be1cf023573825da086f1ca45f2914f708007b0d.jpg" width="666" height="500">
```

---
## \#15 Posted by: egzplicit Posted at: 2017-11-07T17:35:23.749Z Reads: 129

```
TYou had no app so it’s good. When doing detection u wanna make sure the app is set to none  just so it doesn’t interfere with the process.

If you didn’t do the hall sensors detection it could be that it had problems starting, as far as I know without sensors you have to kick push/rotate the motor w bit for it to start (but in FOC it should still spin).

Try redoing motor detection and make sure you apply the settings. Then see if it spins. Try manually rotating the motor a bit before hitting the keyboard or do hall sensors detection as well and set it to hybrid mode.

Also make sure you click both apply buttons!
```

---
## \#16 Posted by: EastLosMike Posted at: 2017-11-07T18:01:52.833Z Reads: 118

```
Thanks man I will give this a shot tonight. I am pretty sure I hit the apply buttons(I went over the dection multiple times from the beginning) however I did not notice a status change at the bottom of the window when applying both the only time I got a notification was when I clicked the write button.

Another question I had was Under FOC> General do I need to change the senseless radio button? I didn't notice any changes made after watching the video so I left it as is.
```

---
## \#17 Posted by: egzplicit Posted at: 2017-11-07T18:07:59.517Z Reads: 127

```
Did you write the configuration to the vesc after clicking both Apply buttons? Maybe you forgot that and never wrote the detected settings into the vesc.

Once you do detection and apply the values, make sure you write them to the vesc then try to spin the motor with the keyboard.

If you want sensors (you do), make sure the hall sensors are plugged in and click the “measure” button under “detect hall sensors” at the bottom left. On the right hand side you should see some numbers after detection. Click apply then again write the configuration to the vesc.

And yes, change that radio button to Hall (and again, make sure you write every change you make).
```

---
## \#18 Posted by: thisguyhere Posted at: 2017-11-07T18:11:16.715Z Reads: 124

```
[quote="EastLosMike, post:10, topic:37559"]
I am not sure if the Battery cutoff start i have is accurate for my 8S setup
[/quote]

from everything i can see, it seems safe cutoff voltage is 3.7, maybe even down to 3.5 per cell.

so multiply that by S count, so 3.7 x 8 = 29.6v for lower cutoff.  maybe even down to 28v.

someone better at lipos may have a better answer, @Namasaki comes to mind.
```

---
## \#19 Posted by: Namasaki Posted at: 2017-11-07T18:35:21.309Z Reads: 124

```
Even 3.6 is fine for low voltage end. 
In fact I would consider that to be conservative.
```

---
## \#20 Posted by: EastLosMike Posted at: 2017-11-07T23:24:52.080Z Reads: 125

```
Appreciate it I will try it again tonight 😊I forgot to mention there is no load on the motor whatsoever  I removed the belt to try to set this up 

@thisguyhere and @Namasaki i will make the suggested settinga and update everyone.
```

---
## \#21 Posted by: EastLosMike Posted at: 2017-11-08T03:54:51.875Z Reads: 127

```
@egzplicit Still no luck i followed the steps 3 timea every time, I made sure to hit Apply and write every time I made any changes. measured the Hall sensors.

The last time around I even tried disconnecting the mini control receiver from the FOCBOX. I also  and trying o spin the motor with my hand before using the arrows.

Edit * Video below

These r ate setting I'm working with now .<img src="/uploads/db1493/original/3X/5/4/549d3f25d54e006da6a575c1e75137262b6e9ec1.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/d/7/d748e5927089c2ed994f34b0c0700bafa02a1d91.jpg" width="666" height="500">

https://youtu.be/Fd54K5C8h3g
```

---
## \#22 Posted by: thisguyhere Posted at: 2017-11-08T03:56:24.518Z Reads: 112

```
why don't u just try bldc for now, just get it running
```

---
## \#23 Posted by: egzplicit Posted at: 2017-11-08T09:13:17.916Z Reads: 111

```
Everything looks alright and it’s very weird that detection works but it still doesn’t spin.

Last night I’ve connected my dual 5065 racerstar to update some settings and I couldn’t spin the motors from the keyboard. But the remote worked just fine. It’s worth you setting the remote as well and try using that instead of the keyboard. Just detect everything again, write the configuration and setup up ppm and try with the remote.
```

---
## \#24 Posted by: EastLosMike Posted at: 2017-11-08T18:37:07.051Z Reads: 104

```
I will give it a try tonight, by the way did you also get the same noise as the video? 

If this does not work I'm  thinking maybe re-flashing the firmware as my last resort.
```

---
## \#25 Posted by: EastLosMike Posted at: 2017-11-08T18:42:36.324Z Reads: 103

```
I want that stealth motor noise using FOC but if I can't set it up tonight I will try BLDC. I see a lot of people mentioning you can't jump from BLDC and FOC is this true?
```

---
## \#26 Posted by: EastLosMike Posted at: 2017-11-09T09:29:24.828Z Reads: 107

```
I was able setup the mini remote and get the motor spinning in BLDC mode with no load...But when I add the belt the wheel does not spin its almost like the motor does not have enough juice to spin. I tried helping it with my hand but that only gives about a half turn before it stops. :( 

I've attached the new setting and Videos <img src="/uploads/db1493/original/3X/7/f/7f2190d5c7c1a6d3a11f2bb0b18f984200d9a92c.png" width="690" height="388"><img src="/uploads/db1493/original/3X/b/d/bdc5f62c4e4835e4e371ad2852dc049242102935.png" width="690" height="388"><img src="/uploads/db1493/original/3X/d/2/d23dad0d83bab8fc957bac4cfb606edf003c0c7e.png" width="690" height="388"><img src="/uploads/db1493/original/3X/3/d/3db7d55d81b82e0ba051c867a7331f2076cfa78e.png" width="690" height="410">

https://youtu.be/KF4qgmgGnCc

https://youtu.be/YA_DR3WwPoA
```

---
## \#27 Posted by: egzplicit Posted at: 2017-11-09T09:50:55.292Z Reads: 100

```
@EastLosMike  your battery cut off start and end are wrong, this will cause the issue forcing the VESC to stop spinning the motor.

In your screenshot you have:

Battery cutoff start: 28v
Battery cutoff end: 30v

First of all cutoff end voltage needs to be lower than the start voltage (by 3v usually). 

Giving you have 2 x ZIPPY Flightmax 5000mAh 4S1P in series, nominal voltage is 29.6v (3.7 * 8). I only know/used li-ion so not sure how low you should go with lipos, but your values are 100% wrong at the moment. 

Lipos have 3.7 nominal voltage and I read minimum voltage is 3.0v. Based on this I would set:

**Battery cutoff start: 27.00v** (that's 3.37v per cell)
**Battery cutoff end: 24.00v** (that's 3v per cell)

**Since 3.0v is the minimum, it might be safer to do 29v (3.6v per cell) start and 26v end ( 3.25v per cell).**

This should hopefully fix your issue.

Edited: what happens now is that your cutoff voltage is at 30v and when you have load on your motor, the voltage drops below that value due to load. Since the voltage drops below your cutoff end, the VESC will limit the amps going into the motor in order to not damage your cells.
```

---
## \#28 Posted by: EastLosMike Posted at: 2017-11-09T20:41:40.363Z Reads: 90

```
Thanks again i will give this a shot tonight maybe this is the same reason FOC was not working :thinking:

@Namasaki
I also noticed by going through some of your settings both ERPM Min and Max should be the same  right(one + and the other -) I just noticed I overlooked this i have different for each.
```

---
## \#29 Posted by: Namasaki Posted at: 2017-11-09T21:54:46.835Z Reads: 90

```
They where the same by default so I have kept them the same.
And be sure to uncheck this setting. It is usually checked by default.
<img src="/uploads/db1493/original/3X/d/c/dc2e5ecced717ca762546d91dcde78fa02229d7a.png" width="244" height="35">
```

---
## \#30 Posted by: EastLosMike Posted at: 2017-11-21T22:11:57.857Z Reads: 87

```
I was able to get my setup working this weekend thanks to suggestions from @yummyblobs 
I set the Battery cut off start to 8v Ran the motor detection successfully  (With the belt installed) Once the detection was complete I changed the Battery cut off start to 28v.

https://youtu.be/rS8sHxzIIFM

I strapped the components inside Tupperware and to the top of the deck and was able to hit 11mph with some speed wobble I believe is to both loose trucks and my foot placement (due to the Tupperware in between my legs lol)I will be ordering some Med Orangatang Nipples bushings to eliminate speedwobbles. Does anyone have experience with these Bushings I'm 150lbs ish and currently debating on the Med purple or Hard Yellow.

https://youtu.be/Ty54ULVl9_E
```

---
## \#31 Posted by: EastLosMike Posted at: 2018-04-30T17:28:37.335Z Reads: 61

```
Quick Update! I Ordered another battery and upgraded to 12S (ordered a helmet too) :smile: and will post a parts list by the end of this week. 

I might need abother set of eyes to confirm my 12s FOC settings. So far I have about 12 miles on 12s but dont feel the torque is all there compared to the old 8S settings.
```

---
