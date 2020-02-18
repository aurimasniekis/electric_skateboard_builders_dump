# FOCBOX UNITY &#124; Support, Setup &amp; Troubleshooting

### Replies: 2212 Views: 40108

## \#3 Posted by: Bjork3n Posted at: 2018-12-12T16:33:29.185Z Reads: 979

```
So is it advised to use the focbox tool instead of the bldc 2.18fw that came with the focbox?
Should you upgrade to this FW (23.40,23.41)?
```

---
## \#4 Posted by: Blasto Posted at: 2018-12-12T16:38:07.532Z Reads: 966

```
No do not update your single Focbox'es to 23.41. **The Unity tools (Focbox UI and Focbox tool) and Firmware will only work for the Unity hardware.**

the single focbox still stays with the BLDC tool, VESCTool  or other compatible 3rd party applications
```

---
## \#5 Posted by: Bjork3n Posted at: 2018-12-12T16:39:14.972Z Reads: 923

```
ok! Thanks for the quick response Blasto!
```

---
## \#6 Posted by: juanmik Posted at: 2018-12-12T18:39:57.306Z Reads: 890

```
Can you get 12v for led light?
```

---
## \#7 Posted by: Blasto Posted at: 2018-12-12T18:51:55.799Z Reads: 871

```
Dont know who you are addressing your question... but no. It’s battery voltage that is comming out of the Aux
```

---
## \#8 Posted by: juanmik Posted at: 2018-12-12T19:05:41.766Z Reads: 866

```
If you do not know do not speak. the unity has several free bays JST, but I do not know if it's only 5v or it can have 12v.
EDIT: I do not speak English. I did not want to be impolite. sorry.
```

---
## \#9 Posted by: Blasto Posted at: 2018-12-12T19:06:42.997Z Reads: 851

```
No there’s no 12V

And i didnt know who you were addressing your message because you replied to yourself
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-12-12T19:08:07.100Z Reads: 843

```
[quote="juanmik, post:1316, topic:64944, full:true"]
If you do not know do not speak. the unity has several free bays JST
[/quote]

https://media.giphy.com/media/Vg0JstydL8HCg/giphy.gif

There is no 12V output and there is no 5V output that you could connect your lamps

EDIT: better don't connect anything to Unity apart battery meter to that aux port
```

---
## \#11 Posted by: Blasto Posted at: 2018-12-12T19:15:19.610Z Reads: 793

```
The 5V output can handle under 1A, too little for any lights. That is what kugelis means
```

---
## \#12 Posted by: b264 Posted at: 2018-12-12T19:28:07.507Z Reads: 790

```
@juanmik plugging a light into any of that is a bad idea. It's a better idea to use a separate system.

If you want to pull 5V from the Unity against the advice of everyone, there is +5V for the servo wire (that connects to remote receiver).  But, I would not pull more than a few hundred milliamps from it.  You can kill your Unity.

If you wanted to use that 5V as a digital signal to turn on another system, that's better than pulling the lighting power from it.
```

---
## \#13 Posted by: Deodand Posted at: 2018-12-12T20:18:18.658Z Reads: 757

```
Pulling too  much amps from 5V shouldn't permanently damage anything, but it will cause the unit to shutoff/reset until the drain is removed.
```

---
## \#14 Posted by: billappleton Posted at: 2018-12-13T01:33:31.031Z Reads: 713

```
Having fun with Unity! A few questions.

 First, I turned on "push to start" but it doesn't seem to work yet. How long do I push to start? Can the power switch be connected? Or must it be disconnected?

I accepted the default values for cutoff start, cuttoff end, and discharge currents, max motor current, etc. Is there a better way to set these values?

My board screams. Screams. I'm afraid to ride it. Can you provide some ballpark values for this? 12S4P, 200Kv Motors

Thanks
```

---
## \#15 Posted by: Blasto Posted at: 2018-12-13T01:51:37.827Z Reads: 676

```
For push to start, takes a few good sustained pushes for the mcu to latch.

I would only perform the motor detection then leave all the other value default... they are pretty descent
```

---
## \#16 Posted by: billappleton Posted at: 2018-12-13T01:58:39.082Z Reads: 659

```
It all seems to work.... I noticed on the motor detection one motor has a little different values than the other. The diagrams are different: one has a dot in the circle arrow the other does not. Does that make sense?
```

---
## \#17 Posted by: Blasto Posted at: 2018-12-13T02:03:09.863Z Reads: 665

```
Yeah that makes sense. The diagram is a visual representation of the previous foc hall table

One of your hall sensors inside your motor might be wonky. But i think, need @Deodand to confirm, you only need 2 out 3 sensors operational for a good startup. As long as the hall detection is consistent, you’re good
```

---
## \#18 Posted by: billappleton Posted at: 2018-12-13T02:34:34.784Z Reads: 649

```
here is the picture

![Screenshot%20(5)|690x388](upload://9y28fCXLvp7cy2HX2hH0BGgJNvS.jpeg)
```

---
## \#19 Posted by: Blasto Posted at: 2018-12-13T02:39:01.518Z Reads: 633

```
Ah, your halls tables look perfectly normal, nothing wonky there
```

---
## \#1 Posted by: onloop Posted at: 2018-12-13T02:44:47.718Z Reads: 1055

```
**This thread is dedicated to helping users setup & use the Focbox Unity.**

![image|500x500](upload://65ytsuWqL4jW8li0Gct1UiysrBa.jpeg) 

![Unity-In-Box-Setup-GuideArtboard-2|357x500](upload://mNJ85iYJBE8amHkN1Ilbhj5kE9A.jpeg) 


https://youtu.be/C7MtbMTKrOs

The FOCBOX unity is extremely simple & fast to set up, however, it's new & very different when compared to other similar products in the market, This difference can be confusing and often make it "seem" harder to set up.

**If you need help please ask questions in this thread.**
```

---
## \#2 Posted by: onloop Posted at: 2018-12-13T02:45:34.647Z Reads: 836

```
:white_check_mark: :calling: **FOCBOX UNITY SOFTWARE & APPS** 
[**FOCBOX UI (Android)**](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/android_build/FOCBOX_UI_1.0.apk)
[**FOCBOX UI (Windows)**](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_UI_1.0.exe)
[**FOCBOX TOOL (Windows)**](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_TOOL_1.0.exe)
[**FOCBOX UI (Sources)**](https://github.com/EnertionBoards/FOCBOX_UI)
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2018-12-13T02:48:59.528Z Reads: 622

```
Correct me If I'm wrong @billappleton

but I think he is referring to this

![image|398x499](upload://9LC1hJpJmqUisNax2Rb7YZilrLZ.jpeg)
```

---
## \#21 Posted by: Blasto Posted at: 2018-12-13T02:51:24.983Z Reads: 576

```
Ah right, means one motor is being reversed in order to run is the correct direction
```

---
## \#23 Posted by: billappleton Posted at: 2018-12-13T13:40:40.452Z Reads: 575

```
Can I fix that? Should I fix that?
```

---
## \#24 Posted by: Blasto Posted at: 2018-12-13T13:54:44.845Z Reads: 571

```
No, nothing to fix really (nothing is broken). Thas why you were prompted to hand spin the wheels in the proper direction
```

---
## \#25 Posted by: billappleton Posted at: 2018-12-13T14:29:23.563Z Reads: 569

```
I switched some motor wires and got them in the same direction, someone can do that if they want them the same. I was wondering if this affects roll to start, will investigate. Otherwise great experience with the software!
```

---
## \#26 Posted by: Blasto Posted at: 2018-12-13T14:36:18.646Z Reads: 556

```
No it does not affect the roll to start. In future firmware revisions, we want to have a roll to start sensitivity level. Because depending on the motor Kv, not all systems are the same
```

---
## \#27 Posted by: Deodand Posted at: 2018-12-13T16:13:11.095Z Reads: 544

```
The software is designed to automatically detect motor direction. Regardless of motor directionality the motors reverse conduct into the controller.

Essentially mosfets have an internal diode and any time any phase voltage increase beyond it's dropout voltage (typically a volt or two max) They will reverse conduct. So any time any one of the phase voltage amplitude exceed a few volts they put current back into the unity. Enough current and the unit turns on and latches on if you have push to start enabled.
```

---
## \#28 Posted by: billappleton Posted at: 2018-12-13T16:38:43.340Z Reads: 531

```
Push to start works great, i just had to get used to it. 

BTW your QR Code points here: https://www.enertionboards.com/focbox-unity-help-support-guide-info/

Might want to update that for people who are not on the forum -- needs to point to the downloads, at least.

One other bit of feedback. The software tells you that you need a firmware update but does not really tell you to go do it on the firmware tab. 

:slight_smile:
```

---
## \#29 Posted by: Deodand Posted at: 2018-12-13T16:41:50.291Z Reads: 510

```
@billappleton Thanks! This is great feedback we will get this fixed in the next release and update that link.
```

---
## \#30 Posted by: MannyM0E Posted at: 2018-12-13T18:52:04.780Z Reads: 511

```
Idk if it was already brought up, any apps for IOS ?
```

---
## \#31 Posted by: ElectricCoast Posted at: 2018-12-14T02:13:50.120Z Reads: 507

```
I plugged both of my unities into my computer and tried both supplied usb c cables but the unities are not connecting to my computer.  I am certain that this may be a driver issue.  Can someone give me some guidance on how to rectify this issue?
```

---
## \#32 Posted by: Deodand Posted at: 2018-12-14T02:18:23.084Z Reads: 522

```
[quote="Andy12, post:14, topic:20471"]
maybe these pics will help
.![|304x459](//www.electric-skateboard.builders/uploads/db1493/original/3X/2/5/259491417845a6107bc967fd950dc8da7da7a6fe.PNG)![|236x275](//www.electric-skateboard.builders/uploads/db1493/original/3X/0/e/0ed7baa0a7a6c1f6faf9cade81db00d47b712d90.PNG)![|455x146](//www.electric-skateboard.builders/uploads/db1493/original/3X/4/8/48146dca8dfa4bfcb18b2060318b2b1d39f7d729.PNG)![|523x208](//www.electric-skateboard.builders/uploads/db1493/original/3X/d/8/d85a6ef48b3db345784d61e03414ebb5edda72b9.PNG)![|436x455](//www.electric-skateboard.builders/uploads/db1493/original/3X/2/3/23544789c4bbf89aa0d8d8e764f9f39afb582fd8.PNG)
[/quote]

Try this maybe? Haven't run into this issue.
```

---
## \#34 Posted by: billappleton Posted at: 2018-12-15T00:12:03.926Z Reads: 467

```
I would like to see power curve adjustments. This might be the job if the remote, but anyway Unity might be able to do it. For example, I would like more power earlier and less sensitivity at the top
```

---
## \#35 Posted by: hexakopter Posted at: 2018-12-15T00:17:01.489Z Reads: 468

```
Isn't that already possible with the Focbox Tool? Not the restricted Focbox UI for easier use but the full tool.
```

---
## \#36 Posted by: Deodand Posted at: 2018-12-15T00:24:53.228Z Reads: 486

```
![Screenshot_20181214-162333|230x500](upload://mcU2yjY7s1QpCCEXeEvL7NhhimP.jpeg) 

The tune throttle curves button here should have what you are looking for.

Something like this would make it punchier in the low range:

![Screenshot_20181214-162707|230x500](upload://e3UUkwI3eu9MpPidnMUbtii1WS3.jpeg)
```

---
## \#37 Posted by: billappleton Posted at: 2018-12-15T01:07:21.073Z Reads: 441

```
Killer! I will give it a try

Would be very helpful if the axis of the graph were labeled, then we would know what was being adjusted thanks !

Even better if you could plot the output.
```

---
## \#38 Posted by: CarlCollins Posted at: 2018-12-15T01:36:58.733Z Reads: 442

```
I think left slider is X-axis and right slider is Y-axis
in normal cases graphs work like that (Not sure about Polynomial Functions)
```

---
## \#39 Posted by: billappleton Posted at: 2018-12-15T01:45:20.700Z Reads: 452

```
No, I mean which axis is the remote percent and which is the power output. I got it, but graphs have to have axis labeled for them to have meaning. Sorry not trying to nitpick.
```

---
## \#40 Posted by: Blasto Posted at: 2018-12-15T01:46:37.130Z Reads: 462

```
X axis is the % of the throttle

Y axis is the % of the output
```

---
## \#41 Posted by: Deodand Posted at: 2018-12-15T01:47:32.965Z Reads: 468

```
X axis (horizontal) remote input y axis throttle output. Kind of relying on inuition here but yeah... Could label.

The labels really cluttered the layout and made the graph too tiny. I'll probably do an overlay tutorial at  some point. Sliding the sliders reveals what they do effectively I think.
```

---
## \#42 Posted by: billappleton Posted at: 2018-12-15T01:50:17.630Z Reads: 468

```
I understand cluttering the layout. You could call out x vs y under the title. 

By the way, the power curve of my new board is way better now! This is an important feature.
```

---
## \#43 Posted by: Deodand Posted at: 2018-12-15T01:51:00.387Z Reads: 438

```
Yeah, that's a good idea thanks.
```

---
## \#44 Posted by: SJG717 Posted at: 2018-12-15T06:42:58.461Z Reads: 442

```
@Deodand got my Unity installed and will test soon. Thing is sick! Thank you for building it! One thing I noticed while setting up in the app is that if I choose a custom voltage cutoff (say 39 and 36V for my 12S battery) it switches to 11s(while keeping custom voltage values) after applying settings, which then sways the battery percentage in the HUD making it inaccurate. Not a big deal but wanted to mention. Thanks again can't wait to ride this thing soon!
```

---
## \#45 Posted by: Deodand Posted at: 2018-12-15T07:09:18.707Z Reads: 439

```
hmmm strange I'll investigate and fix.
```

---
## \#46 Posted by: nuttyjeff Posted at: 2018-12-15T07:14:23.692Z Reads: 444

```
Is it possible for to turn the unity on and off via an seperate antispark rather than the integrated one?
```

---
## \#47 Posted by: Deodand Posted at: 2018-12-15T07:32:15.178Z Reads: 446

```
you can just short the pins of the momentary switch (the two white wires on the included switch)  and the unit will be put into always on mode.
```

---
## \#48 Posted by: nuttyjeff Posted at: 2018-12-15T08:40:17.894Z Reads: 457

```
![IMG_20181215_163942|666x500](upload://zrZ2ZuekYyB5ztfdetXNu2lV8s5.jpeg) 

Didn't want to destroy your beautiful button wires, did i get this right?

I just need to plug that into the Unity?
```

---
## \#49 Posted by: Deodand Posted at: 2018-12-15T17:02:56.205Z Reads: 443

```
Yep! It will still be anti-spark protected with this plugged in as well. You will lose the auto-shutdown feature and push to start.

That length wire should be fine for the switch by the way, it would show pretty quickly in testing if it wasn't as you'd notice the switch LED flickering etc. It wouldn't break the unit just give it false positives on the switch being pressed. I think the new capacitor we added will prevent this being an issue.
```

---
## \#50 Posted by: SJG717 Posted at: 2018-12-15T23:44:39.262Z Reads: 449

```
@Wajdi @Deodand Just a quickie update, Unity working great with ppm remote. Hooked up my photon and seem to be missing telemetry on UART. Not sure if it's the remote or unity. The amp reading is also wacky. Thanks guys! ![IMG_20181215_173914|375x500](upload://gBsVmB5qQzQpPwyX6DH1aDn6kel.jpeg)
```

---
## \#51 Posted by: Blasto Posted at: 2018-12-16T00:09:32.119Z Reads: 430

```
The uart protocol slightly changed on the unity since it is sending information of 2 motors.
```

---
## \#52 Posted by: lemntl Posted at: 2018-12-16T00:18:22.834Z Reads: 430

```
will the unity work with the AS5047 encoder?
```

---
## \#53 Posted by: Deodand Posted at: 2018-12-16T00:25:49.211Z Reads: 432

```
It can but a rework is required similar to other vesc based designs. I also haven't finished coding in firmware support for motor 2 for encoders, but it shouldn't be very difficult to do.
```

---
## \#54 Posted by: billappleton Posted at: 2018-12-16T15:46:28.630Z Reads: 440

```
Would this throttle curve increase throttle AND breaking when the slider is near zero?

In other words, the graph shows breaking to the left of zero and throttle to the right, correct?

Sorry to belabor this...

![curvy|338x500](upload://bTN9QRvfOCDWAiPcVllCWrhslt7.jpeg)
```

---
## \#56 Posted by: Deodand Posted at: 2018-12-16T16:25:27.602Z Reads: 439

```
Yes, -0 to -100 is the negative range of the throttle. Positive values cause a harder start/stop near 0 and negative provide a softer start/stop near 0 throttle.
```

---
## \#57 Posted by: trampa Posted at: 2018-12-16T21:17:13.359Z Reads: 457

```
The Unity fork of VESC-Tool mobile has the help files excluded as far as I can see. 
In the original VESC-Tool you will find a lot of info clicking on the **?** or HELP.
The mobile version for Android is nearly a full VESC-Tool but with a different UI structure. 
Benjamin also integrated the HELP files into the mobile VESC-Tool to help people find some basic answers. 
For good reasons he didn't integrate the throttle curves into the mobile frontend though. 
I have no clue why the Help files have been stripped from the Unity Fork of VESC-Tool mobile.

If you need answers you can always go to the matching setting in VESC-Tool or VESC-Tool mobile and click on the **?** or HELP.  You will see that it is easy to find the corresponding settings in the official releases. 

X-Axis = throttle value
Y-Axis = output value

You can choose polynomial, natural and exponential functions. 

Most of the time it is better to leave the throttle curves untouched and use the **pos/neg ramping time** to soften or sharpen the throttle response. This setting can be found in **App Settings >> PPM >> General**.

The most important thing that has an effect on the throttle response are the **Current settings** for Motor Max, Motor max Regen, Battery Max and Battery max Regen. Using symmetric settings for Motor and Battery Currents makes your vehicle respond most linear to the throttle stick. 
Bad example: Many people have used very high **Motor Max Regen** settings (-80A) while using very low **Battery Max Regen** settings (-10A), thinking that their battery can't handle a short inrush of high Amps. This will result in very very weak brakes at speed which get very very aggressive when you slow down a bit. Users have then tried to compensate that extreme non linear behaviour using the throttle curves, not understanding that they should rather have used symmetric settings for **Motor MAX Regen** and **Battery Max Regen** ( eg. -30A and -30A) to resolve the matter. In such a case the curves will not really help to resolve the issue of weak brakes at speed! 
Conclusion:
It is important to have the most relevant settings right before trying to use a second set of "expert" settings that influences the behaviour again. If your Motor- and Battery Current settings cause a non linear response to your throttle input, **you start to overlay curves with curves** when playing around with throttle curve settings. **That is extremely uncontrollable.** 
This is why Benjamin didn't integrate the throttle curves into the more simple mobile UI. 

Throttle curves are not the most useful feature in skateboarding. You can use them to fine tune your setup, once everything else is setup to react perfectly linear. Two shunt designs like VESC 4 and derivates do not react linear to the throttle input by design!  Using the throttle curves can make things worse, especially in the range between 60 and 100% throttle. 

![VESC-Tool%20throttle%20curves|690x367](upload://tSQBnCoDva3Xz8vjqiXl598qVS0.jpeg) 
![VESC-Tool%20throttle%20curves_2|625x443](upload://y0pKNEXL8wJPRy4Eh66IrTB8Cbo.jpeg) 
![VESC-Tool%20throttle%20curves_3|625x350](upload://gtbylClhWeM1VwsAdeeSj0Szci0.jpeg)
```

---
## \#59 Posted by: briman05 Posted at: 2018-12-17T05:28:17.862Z Reads: 421

```
Anyone test the unity with racerstar motors had an issue with sensor detection on bldc tool wanted to know if that issue carried over
```

---
## \#58 Posted by: onloop Posted at: 2018-12-17T12:04:08.805Z Reads: 339

```
8 posts were merged into an existing topic: [Help with battery and vesc settings](/t/help-with-battery-and-vesc-settings/39593/3)
```

---
## \#60 Posted by: onloop Posted at: 2018-12-17T12:05:02.957Z Reads: 377

```
This thread is specifically about focbox troubleshooting, please stay on topic.
```

---
## \#61 Posted by: billappleton Posted at: 2018-12-17T13:33:39.331Z Reads: 388

```
The QR Code still points here: https://www.enertionboards.com/focbox-unity-help-support-guide-info/

This page should redirect to your new help desk site here: https://enertionboards.zendesk.com/hc/en-us/categories/360000073116-FOCBOX-Unity

:slight_smile:
```

---
## \#62 Posted by: onloop Posted at: 2018-12-17T13:49:28.935Z Reads: 378

```
Eventually we will have enough resources to make all elements of our business picture perfect ;)

For now we just have to deal with a blank page.
```

---
## \#63 Posted by: Wajdi Posted at: 2018-12-17T17:09:23.205Z Reads: 383

```
Seems like the protocol changed, anyone have a link for the source code?
```

---
## \#64 Posted by: Blasto Posted at: 2018-12-17T17:20:27.795Z Reads: 385

```
https://github.com/EnertionBoards/bldc
```

---
## \#65 Posted by: billappleton Posted at: 2018-12-18T14:37:53.813Z Reads: 396

```
Hi All,

I am having trouble "taming" my new build with 12S4P and 6369 200kv motors. The board has a tendency to throw you off the back if you accelerate too quickly. Maybe I shouldn't have named it "Hellboy."

I have fooled around with throttle curves, but also read the post from @trampa carefully when he discusses PPM and Motor / Battery Max / Regen. Currently I am at the default FOCBOX Unity settings of 60 and 30 amps,

Is there a different setting I should try? I need a better understand of what the current settings do and what baseline / best practices are helpful setting up Unity for a custom board.

Thanks in advance
```

---
## \#66 Posted by: brenternet Posted at: 2018-12-18T14:52:21.695Z Reads: 383

```
Just getting real simple, what remote are you using, does the throttle have enough throw for you to smooth it out with your finger?

Your setup is relatively beefy, I think most of us just learned to not fall with the power! Probably not ideal
```

---
## \#67 Posted by: billappleton Posted at: 2018-12-18T15:01:50.135Z Reads: 392

```
I am using the Hoyt Puck for the remote. I would say it is very sensitive. I am an experienced skater, but for example, yesterday I was going slowly and maybe jiggled the remote wheel a little and wham -- on my back. The board can do this at high speed too, although I am more diligent there.
```

---
## \#68 Posted by: JohnnyMeduse Posted at: 2018-12-18T15:19:48.194Z Reads: 384

```
Isn’t there suppose to be 3 different mode on this remote?
```

---
## \#69 Posted by: brenternet Posted at: 2018-12-18T15:22:32.345Z Reads: 381

```
Yeah I'd put the puck up there with the better ones based on reviews here.
```

---
## \#70 Posted by: DAddYE Posted at: 2018-12-18T15:34:18.545Z Reads: 381

```
Just increase the ramping time in the ppm section.
```

---
## \#71 Posted by: Blasto Posted at: 2018-12-18T15:39:21.529Z Reads: 395

```
Few ways to tweak your settings,

opinion 1:

lower your current settings. ex: try motor max 50 min -50, batt max 40 min -20

opinion 2:

play with the throttle curve, smooth out the lower portion of the ppm curve with the exponential curve

example:
![image|573x423](upload://cknL2COxh2jQ5cvLQtj9g3gCTsn.png)
```

---
## \#72 Posted by: billappleton Posted at: 2018-12-18T15:46:11.399Z Reads: 381

```
@johnnyMeduse yes, there are 3 modes, I have been trying that, I tend to end up in mode 3 (fastest) because of hills... 

@blasto I will try option 1 fur sure. I wish I had detailed explanations on what those terms mean exactly.  For example, where is / what is the PPM section?

On the throttle curve, the suggested curve above seems to push the acceleration problem into faster speeds. Instead of an explosion at 5 miles per hour, now I get one at 20. I think this is what Frank meant by saying the power curve was of limited usefulness.
```

---
## \#73 Posted by: Deodand Posted at: 2018-12-18T16:07:57.476Z Reads: 383

```
Keep in mind the throttle curves input is amount of throttle not speed. But yeah I like to keep mine at -10 %, -10%. 

You ran the **remote config→calibration** in the setup to get min and Max for your remote when it was in the fastest mode? This might be your problem I have tested a hoyt remote here and the timing of it was a bit strange. I'll be adding some more notes/steps to guided setup with the next release to explain more things quickly without walls of long text. 

If you ran min/max calibration in a slow mode with the remote it could definitely mess up your sensitivity.
```

---
## \#74 Posted by: 701Superjet Posted at: 2018-12-18T16:24:16.809Z Reads: 383

```
Under the motor temp limits tab in the
Unity app. What is the motor beta slider for? Thanks!
```

---
## \#75 Posted by: Deodand Posted at: 2018-12-18T16:28:46.379Z Reads: 389

```
If your motor has a thermistor in it for measuring temperature then beta is just a property of that thermistor. See here:

https://www.ametherm.com/thermistor/ntc-thermistor-beta

If your motors don't have a sixth wire coming out of them plugging into the Hall port don't worry about it. If they do and you don't know the beta value contact your supplier. If they don't know you can stay with the default beta value, disable motor temp throttling, or run some experiments to determine beta on your own
```

---
## \#76 Posted by: billappleton Posted at: 2018-12-18T16:58:28.317Z Reads: 406

```
Hera are my current settings. Also the motor has 6 wires, this one here: https://psychotiller.com/product/sensored-6365-200kv-motor

![Screenshot%20(7)|690x396](upload://5KclVEnyZPNPGiJwXXg944XZq3m.png)

![Screenshot%20(9)|690x392](upload://7mbPa7B5lgzZnb2oYrlKpxn6MDy.png)

 ![Screenshot%20(10)|537x499](upload://5GZGxJSTAd6AjOD4PVrAis0q4ke.png)

 ![Screenshot%20(11)|690x363](upload://lDwIzk8ZE5OXtUx7jLNnFiZHoPd.png) 

![Screenshot%20(8)|690x472](upload://wJ9AloAfh8NsmQwsweoONTx5xuI.png)

 ![Screenshot%20(12)|690x395](upload://fxoYgUteGGNygKvW4uyxguje2g5.png)
```

---
## \#77 Posted by: Deodand Posted at: 2018-12-18T17:04:17.657Z Reads: 367

```
![Screenshot_20181218-090008__02__01|690x394](upload://uJu4PN6p6pBFmI5Xji1qFsavZEp.jpeg) 

Are you touching your remote here?  It's reading out -19% for some reason which is strange. I'd re-run the calibrate routine making sure it's in the highest speed mode. A screenshot of that submenu would be helpful too if you are still having issues.
```

---
## \#78 Posted by: billappleton Posted at: 2018-12-18T17:13:15.434Z Reads: 349

```
Yep. Talking to Hoyt about that. They are wondering if it is old firmware.
```

---
## \#79 Posted by: Deodand Posted at: 2018-12-18T17:15:02.239Z Reads: 354

```
One of those four buttons on it is a little Trim pot I think. Could try twisting that maybe? Probably shouldn't mess with their debugging process I guess :smile:.

I'll see if I can find a window of time to fiddle with my hoytt (@Blasto 's remote that I stole in vegas) today and see what I find.
```

---
## \#80 Posted by: 701Superjet Posted at: 2018-12-18T17:18:32.461Z Reads: 348

```
I assume the beta value is listed on the spec sheet for the thermistor. I have a couple TB 6374 190kv. I will take the bell off later to see what thermistor they use if some quick googling fails to give results.
```

---
## \#81 Posted by: Deodand Posted at: 2018-12-18T17:22:48.970Z Reads: 348

```
I doubt a visual inspection will yield much. Maybe try asking the guys at torque boards they should know. @Lunasi any idea what the beta value of TB 6374 motors thermistors are?
```

---
## \#82 Posted by: Blasto Posted at: 2018-12-18T17:26:00.236Z Reads: 358

```
Ah yes there’s a trim on the hoyts remote, it’s the bottom right button, it’s a little rocker switch.

@billappleton try to trim up the signal by pressing the trim button up, you want to get the idle position to 0%

Do it while connected to the tool, you will see the graph move
```

---
## \#83 Posted by: billappleton Posted at: 2018-12-18T18:13:20.206Z Reads: 375

```
Hi @Blasto, I had the same thought, but the Trim button on the remote does NOT change the -19% number, going up or down either way.

Response from Hoyt: "I’m not familiar with the FOCBOX Unity user interface so I’m uncertain if it’ll work the same way as a Vesc Tool.  The following process is how to set up the Hoyt RC with Vesc Tool.  Not sure if this sheds light on what may be happening in your situation. 

The Vesc Tool has a set up wizard for the remote control. Set the RC on Mode 2 and then go through the set up wizard. Don’t need to adjust or tweak anything. Modes 1-3 were calibrated in the RC firmware based on VESC default settings so no further calibration is required.

There will be (should be) no braking when the throttle is not engaged."

Should I calibrate on Mode 2 for Unity? Is the trim working / not working?
```

---
## \#84 Posted by: JohnnyMeduse Posted at: 2018-12-18T18:31:47.148Z Reads: 351

```
[quote="billappleton, post:83, topic:77861"]
Should I calibrate on Mode 2 for Unity? Is the trim working / not working?
[/quote]

I would say give it a try.
```

---
## \#86 Posted by: Blasto Posted at: 2018-12-18T19:05:16.512Z Reads: 350

```
sorry for the mega edit @Deodand found it was a display error, the  center position is being properly measured in the app
```

---
## \#87 Posted by: Lunasi Posted at: 2018-12-18T19:33:42.007Z Reads: 348

```
They're 10k thermistors
```

---
## \#88 Posted by: Deodand Posted at: 2018-12-18T20:27:24.682Z Reads: 343

```
Any ballpark guess on the beta value? Or a part number on the thermistors?
```

---
## \#89 Posted by: deucesdown Posted at: 2018-12-18T20:38:22.797Z Reads: 354

```
If it's not some unity/gui bug...

[quote="DAddYE, post:70, topic:77861, full:true"]
Just increase the ramping time in the ppm section.
[/quote]

Bill, I think another approach is to change how fast the current is allowed to change. This way you keep the power but it comes on more slowly. This will affect brake response too. Basically the reverse of this:

https://www.electric-skateboard.builders/t/better-throttle-performance-through-more-responsive-ramping/29356

Another thing you can try is another remote, something you're familiar with, to establish a baseline. If you're not familiar with any, the mini 2.4ghz has a nice response and is cheap.

Otherwise, if the total power is just too much, I'd keep halving the motor and battery max until you get to a comfortable level.
```

---
## \#90 Posted by: 701Superjet Posted at: 2018-12-18T23:32:49.643Z Reads: 333

```
Wasn’t there an unofficial way to get the unity app on an iOS device?
```

---
## \#91 Posted by: Jc06505n Posted at: 2018-12-19T01:04:10.463Z Reads: 342

```
@Kug3lis @Deodand can’t get the unity to connect wirelessly to the unofficial Mac tool, it only connects if I click connect usb even though nothing’s connecTed and it time out after a while
```

---
## \#92 Posted by: Deodand Posted at: 2018-12-19T01:31:03.813Z Reads: 348

```
I doubt bluetooth will work correctly on mac without some fiddling. USB is a good first step, you have a unity plugged in over usb? A bit confused by your statement.
```

---
## \#93 Posted by: Jc06505n Posted at: 2018-12-19T01:48:12.081Z Reads: 339

```
that's the thing, if i click connect Bluetooth it wont connect, but if i click connect usb it will connect over Bluetooth for a few moments
```

---
## \#94 Posted by: Blasto Posted at: 2018-12-19T01:49:22.178Z Reads: 331

```
Give me an hour, i’ll try out the mac version
```

---
## \#95 Posted by: Jc06505n Posted at: 2018-12-19T01:53:11.916Z Reads: 334

```
Did a screen record that I can send, it takes a while till it connect but it eventually does
```

---
## \#96 Posted by: Blasto Posted at: 2018-12-19T02:07:08.436Z Reads: 338

```
I was able to connect using the mac version. However had to do a little work around.

Problem: the UI doesnt recongnize new serial connections

Work around:

Using an old version of the vesctool or bldc tool, connect to it, it will give heck about the version. Quit that program, now you can use the focbox UI. 

I think the problem is fairly simple to fix. @Kug3lis ?
```

---
## \#97 Posted by: Deodand Posted at: 2018-12-19T02:07:53.762Z Reads: 325

```
Might be my fault to... some kind of compatibility fix I didn't add.
```

---
## \#98 Posted by: ducktaperules Posted at: 2018-12-20T11:23:58.798Z Reads: 341

```
hey, is there any documentation on the correct operation of the switch and how its supposed to work?

I received my unity yesterday and have it powered up on the bench but i feel like my switch is not working correctly. 

When i press it to power up the unity the the led ring lights dim. once powered up, pressing the button again causes the led to flicker brighter in an seemingly random manner. holding doesn't seem to shut down the unity 90% of the time.

https://photos.app.goo.gl/zhRVTG5VG73kuNpKA
```

---
## \#99 Posted by: Blasto Posted at: 2018-12-20T13:50:11.635Z Reads: 328

```
Yeah that switch is faulty, @CarlCollins will hook you up with a new one
```

---
## \#100 Posted by: CarlCollins Posted at: 2018-12-20T13:51:09.190Z Reads: 333

```
@ducktaperules
Drop a message to me on the forum with your order ID, I will arrange one for you
```

---
## \#101 Posted by: briman05 Posted at: 2018-12-20T16:43:37.092Z Reads: 331

```
Could the issue with the mac version of the tool be caused by the fact that mac os has gotten rid of open GL/ open CL its supported but you need to basically develop it in Apple's Metal library
```

---
## \#102 Posted by: Shanian79 Posted at: 2018-12-21T01:07:42.874Z Reads: 326

```
I have a Bluetooth remote from a Blitzart board and want to use it with my Unity. Any ideas how to pair them and set it up?
```

---
## \#103 Posted by: brenternet Posted at: 2018-12-21T01:08:31.767Z Reads: 334

```
I gave you a rare heart for this
```

---
## \#104 Posted by: Sn4pz Posted at: 2018-12-21T01:10:16.614Z Reads: 348

```
how *gracious* of you :rofl:
```

---
## \#105 Posted by: brenternet Posted at: 2018-12-21T01:13:07.185Z Reads: 336

```
No heart for you :unamused:
```

---
## \#106 Posted by: Sn4pz Posted at: 2018-12-21T01:13:43.497Z Reads: 343

```
just pissing in your cereal :kissing:
```

---
## \#107 Posted by: Blasto Posted at: 2018-12-21T01:48:08.956Z Reads: 352

```
Not possible sorry.
```

---
## \#108 Posted by: bandrews510 Posted at: 2018-12-21T17:24:25.198Z Reads: 353

```
Is traction control already enabled with Unity. The motors seem to spin at different speeds, how do I sync the erpm of the motors like on focbox and vesc tools of past?
```

---
## \#109 Posted by: Deodand Posted at: 2018-12-21T17:25:39.127Z Reads: 341

```
Nah that feature will be in an upcoming FW update, currently it isn't implemented.
```

---
## \#110 Posted by: StefanMe Posted at: 2018-12-21T20:20:52.190Z Reads: 333

```
Is there any chance to use the BLUETOOTH module with METR? I need the UART port for my FeatherRemote and want to use METR at the same time...
```

---
## \#111 Posted by: Jc06505n Posted at: 2018-12-21T21:48:30.075Z Reads: 340

```
[quote="Deodand, post:774, topic:64944, full:true"]
Answered above in the thread in more detail, but we didn’t come to an agreement unfortunatley so the module is not compatible with metr. We will work to add some logging functionality within our app.
[/quote]

10 charchar
```

---
## \#112 Posted by: Slinge Posted at: 2018-12-22T20:47:11.946Z Reads: 328

```
Is  it possible to remove the power switch? I want it to power on as soon as I power the battery.
```

---
## \#113 Posted by: Shanian79 Posted at: 2018-12-22T22:29:17.842Z Reads: 329

```
Does the 5v JST port need to be enabled? I just got my unity and have a 5v ESC fan that I want to power from it, but I'm not getting any voltage.
```

---
## \#114 Posted by: danwooller Posted at: 2018-12-22T22:31:18.109Z Reads: 327

```
Answered a few days ago, looks like you just short the switch.
```

---
## \#115 Posted by: StefanMe Posted at: 2018-12-22T22:56:01.580Z Reads: 320

```
No... it’s on all the time. U mean the UART? Port?
```

---
## \#116 Posted by: Linny Posted at: 2018-12-23T04:41:40.244Z Reads: 313

```
I have an issue with the JST 2 pin on the bottom right of the Unity, I connected it to my battery indicator and it does not seem to turn on when everything else is.
```

---
## \#117 Posted by: BruSkater Posted at: 2018-12-23T04:46:42.549Z Reads: 305

```
Did you wire it correctly? The jst cable that I have puts the black cable on the voltage pin (according to the diagram that came in the unity's box)... I though it was weird
```

---
## \#118 Posted by: Linny Posted at: 2018-12-23T07:11:28.351Z Reads: 311

```
Okay my mistake, i had the wires swapped, swapped it back and it works now! Thanks!
```

---
## \#119 Posted by: GreasyGearsWRX Posted at: 2018-12-24T18:02:16.372Z Reads: 317

```
So are us iPhone people just waiting for an app to operate/view the unity through? It would be really sweet right now to be able to view my battery voltage!
```

---
## \#120 Posted by: Scream Posted at: 2018-12-24T18:22:24.668Z Reads: 330

```
Has anyone successfully got the unity working with a firefly remote? I believe PPM is working fine for me but I understand there is a change in the UART protocol, and maybe that is what is preventing getting good telemetry data. Does that mean I should make a change to the receiver code somewhere?

Mine works for controlling the board (really well I might add) but I’m not getting telemetry. Pretty sure the baud rates match (11520).

I also tried switching rx and tx wires on the receiver. I either get nothing, or garbage data. I have 5V, GND and PPM plugged into the servo port then just the rx and tx wires wired on a jst plug which is plugged into the comm port of the unity.
```

---
## \#121 Posted by: Deodand Posted at: 2018-12-24T18:35:28.797Z Reads: 337

```
Line 166 here is the order of the new values output:

https://github.com/EnertionBoards/bldc/blob/unity/commands.c

I meant to make a new packet with dual motor data and leave the legacy packet there but I kind of forgot to finish that before launch. If you peak at line 1077 you can see I have the new packet created I just never reverted the old packet structure.
```

---
## \#122 Posted by: deucesdown Posted at: 2018-12-24T21:50:12.810Z Reads: 315

```
If I understand correctly, this breaks all 3rd party stuff that attaches to UART?

The natural followup question: can you revert to legacy packet, and push out a new build?
```

---
## \#123 Posted by: Deodand Posted at: 2018-12-24T23:04:38.587Z Reads: 328

```
Honestly, the get_values packet has changed quite a few times if I'm not mistaken. I think a lot of stuff already has support for multiple get_values  formats so it's a matter of adding unity support. 

I could make that change but I'm not sure on it. I don't want someone feeling like the values part works with a legacy tool then writing config values from a non-compatible app and bugging their setup.  Some of the vesc uart stuff isn't terribly reliable.

But yeah if enough people want it I'll change it.
```

---
## \#124 Posted by: Sn4pz Posted at: 2018-12-24T23:06:27.237Z Reads: 336

```
Firefly remote users salute you o7
```

---
## \#125 Posted by: jadatmag Posted at: 2018-12-26T20:26:06.585Z Reads: 329

```
I think I found a bug in the FOCBOX Tool @Deodand 

After doing the Motor Setup Wizard for the first time and selecting Hall sensors from the dropdown it says in the FOC tab that Sensormode 1 = Hall Sensor and Sensor Mode 2 = Sensorless.

So I think it only sets Hall sensors for one motor in the wizard. I replicated it 2 times and just went on to do the motor detection in the FOC tab.

Great work by the way!

EDIT: Oh maybe it's just me:

It says Bad Foc Hall detection result received in the Hall Sensors tab
```

---
## \#126 Posted by: Deodand Posted at: 2018-12-26T20:28:57.540Z Reads: 321

```
Ah yeah thanks that makes sense I'll get it fixed next update.
```

---
## \#127 Posted by: Scream Posted at: 2018-12-26T20:30:54.723Z Reads: 316

```
Anyone having issues connecting over Bluetooth? I’m on PC, the UI connects fine over USB. My laptop connects to the Unity Bluetooth, but the UI just keeps saying scanning. Is there a step I’m missing?

I can provide more details as and when required.
```

---
## \#128 Posted by: jadatmag Posted at: 2018-12-26T20:42:41.543Z Reads: 332

```
It says "Bad Foc Hall detection result received" in both the Motor Setup Wizard and the Hall sensors tab under FOC.

I have the older Silver R-spec motors, do you see any values that are off?

The motors spin just fine when using my remote at slow speeds without any load on them. As if they are just working good.

![image|655x499](upload://jQKDPJEEN7VR2gSx8durBQDvZBI.png) 

![image|654x500](upload://kMx2k2BYJ83PIdiHwMYCyLf5v7G.png)
```

---
## \#129 Posted by: Deodand Posted at: 2018-12-26T20:46:01.324Z Reads: 301

```
yeah sorry the pc app/tool bluetooth didnt work reliably enough for me to include in this release.
```

---
## \#130 Posted by: Deodand Posted at: 2018-12-26T20:46:55.164Z Reads: 309

```
Yeah ignore that error message, another bug. Your detection completed successfully.
```

---
## \#131 Posted by: jadatmag Posted at: 2018-12-26T20:56:57.650Z Reads: 310

```
Not quite sure who could update this but the telemetry on my Photon remote doesn't work in combination with the Unity. I'll post in the Photon topic if this is the wrong place ![image|375x500](upload://znDrNAza8tUzB3gtFU9CWumnDKO.jpeg)
```

---
## \#132 Posted by: Jc06505n Posted at: 2018-12-26T21:04:16.615Z Reads: 309

```
[quote="SJG717, post:50, topic:77861"]
@Wajdi @Deodand Just a quickie update, Unity working great with ppm remote. Hooked up my photon and seem to be missing telemetry on UART. Not sure if it’s the remote or unity. The amp reading is also wacky. Thanks guys!
[/quote]

[quote="Blasto, post:51, topic:77861, full:true"]
The uart protocol slightly changed on the unity since it is sending information of 2 motors.
[/quote]

[quote="Wajdi, post:63, topic:77861, full:true"]
Seems like the protocol changed, anyone have a link for the source code?
[/quote]

10 char char
```

---
## \#133 Posted by: Deodand Posted at: 2018-12-26T21:05:24.917Z Reads: 309

```
[quote="Deodand, post:121, topic:77861"]
Line 166 here is the order of the new values output:

[github.com ](https://github.com/EnertionBoards/bldc/blob/unity/commands.c)

#### [EnertionBoards/bldc/blob/unity/commands.c](https://github.com/EnertionBoards/bldc/blob/unity/commands.c)

```
/*
 Copyright 2016 Benjamin Vedder	benjamin@vedder.se

 This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 */

#include "commands.h"
#include "ch.h"
#include "hal.h"
```

This file has been truncated. [show original](https://github.com/EnertionBoards/bldc/blob/unity/commands.c)

I meant to make a new packet with dual motor data and leave the legacy packet there but I kind of forgot to finish that before launch. If you peak at line 1077 you can see I have the new packet created I just never reverted the old packet structure.
[/quote]

10 character
```

---
## \#134 Posted by: jadatmag Posted at: 2018-12-26T21:08:24.706Z Reads: 282

```
so much help everywhere, I love you guys
```

---
## \#135 Posted by: Scream Posted at: 2018-12-26T21:19:27.083Z Reads: 282

```
All good, at least I know it’s not user error!
```

---
## \#136 Posted by: AlexBE Posted at: 2018-12-26T23:35:29.921Z Reads: 282

```
@Deodand, would you prefer bugs/feature requests here or via Github?
```

---
## \#137 Posted by: Shanian79 Posted at: 2018-12-27T19:28:58.051Z Reads: 286

```
To fix the Bluetooth function, what exactly do I need to copy/paste into the terminal to fix this? Is it the whole code string noted above or just specific lines. 

Sorry...Never played with this code stuff before and I dont want to brick my unity. Any help would be appreciated!
```

---
## \#138 Posted by: Jc06505n Posted at: 2018-12-27T19:35:27.550Z Reads: 284

```
They code outlined above is for how the UNITY does UART so that people like @rpasichnyk and @Wajdi can make the unity compatible with their applications. 

From what I can see unless the blizart remote has a reciever , you cannot use it with any vesc.
```

---
## \#139 Posted by: Shanian79 Posted at: 2018-12-27T19:50:49.614Z Reads: 277

```
Thanks. I realize that, I am just trying to be able to connect to it with the Unity PC app via Bluetooth.
```

---
## \#140 Posted by: Jc06505n Posted at: 2018-12-27T20:12:06.760Z Reads: 290

```
On PC connecting to Bluetooth should work so long as your PC has Bluetooth abilities. When you scan does nothing pop up? 

Though Also note: 

[quote="Scream, post:127, topic:77861"]
Anyone having issues connecting over Bluetooth? I’m on PC, the UI connects fine over USB. My laptop connects to the Unity Bluetooth, but the UI just keeps saying scanning. Is there a step I’m missing?
[/quote]

[quote="Deodand, post:129, topic:77861, full:true"]
yeah sorry the pc app/tool bluetooth didnt work reliably enough for me to include in this release
[/quote]

So while scanning may not “work” connecting via BT should still be viable
```

---
## \#141 Posted by: Shanian79 Posted at: 2018-12-27T20:54:44.701Z Reads: 277

```
My laptop connects to the BT, however it does not let me connect to the board through the unity UI. Only "Connect USB" is available. The "Connect Bluetooth" button is greyed out.
```

---
## \#142 Posted by: Jc06505n Posted at: 2018-12-27T20:57:01.839Z Reads: 272

```
Hmmm can we see screenshots ?
```

---
## \#143 Posted by: Shanian79 Posted at: 2018-12-27T21:02:40.486Z Reads: 286

```
![Unity%20UI%20Screen%20Shot|690x380](upload://f5TUBljeldUL59wYqZ4MylA5rPt.jpeg)
```

---
## \#144 Posted by: Shanian79 Posted at: 2018-12-27T21:02:56.388Z Reads: 328

```
![Unity%20UI%20Screen%20Shot%202|690x266](upload://wFmR0ljsUs70hbkuOYjMRgz3nzi.jpeg)
```

---
## \#145 Posted by: Shanian79 Posted at: 2018-12-27T21:03:53.597Z Reads: 317

```
PC shows Unity BLE 1.1 as paired, but not connected, after initial connection/pairing.
```

---
## \#146 Posted by: Jc06505n Posted at: 2018-12-27T21:58:16.182Z Reads: 314

```
And you’ve tired forgetting the unity and connecting via the tool right ?
```

---
## \#147 Posted by: Shanian79 Posted at: 2018-12-27T22:10:00.589Z Reads: 317

```
Yeah I've tried. On the UI connection screen there is a drop down option labeled "connection" but has no options. 

When you scan for Bluetooth, it says "scanning" but nothing ever comes up.
```

---
## \#148 Posted by: Deodand Posted at: 2018-12-27T22:16:34.209Z Reads: 320

```
Bluetooth on the PC doesn't work at all for now. Only from the phone can you BT to it. Technically I have a Windows 10 compatible version where BT works but Bluetooth on Windows in general is really buggy so I didn't release it yet.
```

---
## \#149 Posted by: Rod12579 Posted at: 2018-12-28T12:56:02.600Z Reads: 317

```
I haven’t set up my unity yet but I will be soon.. but to be clear can I use either the focbox tool or the ui (windows)..??🤔 also if anyone knows where I can get these bullet adapters that came with the unity that would be awesome... 🤙🏾 ![image|666x500](upload://eIkkYfjSuNwP3aIRC52age7nrm1.jpeg)
```

---
## \#150 Posted by: venom121212 Posted at: 2018-12-28T12:58:53.999Z Reads: 306

```
3.5mm bullet connectors. Amazon, eBay, local hardware. Take your pick.
```

---
## \#151 Posted by: Rod12579 Posted at: 2018-12-28T13:24:24.433Z Reads: 313

```
Yeah but the ones that came with the unity seems to be a bullet connector adapter from 3.5 to 5.5.. I couldn’t find the same ones on amazon... ![image|375x500](upload://8UIu1QCoeGD9USLsZqBa3Uyfwu8.jpeg)
```

---
## \#152 Posted by: venom121212 Posted at: 2018-12-28T13:25:50.940Z Reads: 304

```
Oh my mistake. Take a 3.5 and a 5.5mm bullet and the back end of the 3.5 conveniently slides right in the back end of the 5.5. Add a dab of solder and some heat shrink and you have a professional adapter.
```

---
## \#153 Posted by: Rod12579 Posted at: 2018-12-28T13:33:28.649Z Reads: 301

```
Ok cool...Thanx 🤙🏾 Would u happened to know about the 1st question I asked about the unity? Can I use the tool or the ui users choice?
```

---
## \#154 Posted by: venom121212 Posted at: 2018-12-28T13:40:25.445Z Reads: 304

```
Unity app is easiest if you're android. If not, plug into windows.
```

---
## \#155 Posted by: Rod12579 Posted at: 2018-12-28T13:40:58.569Z Reads: 300

```
Ok thanx got it... 🤙🏾
```

---
## \#156 Posted by: venom121212 Posted at: 2018-12-28T16:03:13.796Z Reads: 293

```
Also it's super lame that I didn't get any if these included with my unity :confused: oh well I guess I learned that bullet trick from it.
```

---
## \#157 Posted by: DougM Posted at: 2018-12-28T16:14:46.707Z Reads: 291

```
[quote="billappleton, post:65, topic:77861"]
Maybe I shouldn’t have named it “Hellboy.”
[/quote]

 I made the same mistake naming mine "Widowmaker"
```

---
## \#158 Posted by: billappleton Posted at: 2018-12-28T16:19:09.790Z Reads: 286

```
Nice! In my case lowering the motor max from 60 to 50 amps helped a lot with the dragster acceleration
```

---
## \#159 Posted by: DougM Posted at: 2018-12-28T19:38:25.067Z Reads: 295

```
[quote="billappleton, post:158, topic:77861"]
lowering the motor max from 60 to 50 amps
[/quote]

The downside to that I think is the decrease in hill climbing ability.  But I guess range goes up so it's a trade-off.
```

---
## \#160 Posted by: Markuss Posted at: 2018-12-28T20:01:29.625Z Reads: 299

```
Need some help here pls.
whar should i do?


![22|690x388](upload://zLHFD8AktkhekPkM4lETBJIYhVk.png)
```

---
## \#161 Posted by: Blasto Posted at: 2018-12-28T20:07:08.733Z Reads: 290

```
You have a Unity right? If so, Go to the firmware tab and click the upload firmware button
```

---
## \#162 Posted by: Shanian79 Posted at: 2018-12-28T22:28:28.769Z Reads: 287

```
Question on The Enertion Nano remote paired with the Unity. The switch for slow and R-Spec modes. Are the parameters for each mode adjustable using the Unity Tool?
```

---
## \#163 Posted by: 701Superjet Posted at: 2018-12-29T02:57:52.186Z Reads: 285

```
Is data logging still in the works for the unity?
```

---
## \#164 Posted by: AlexBE Posted at: 2018-12-29T06:41:56.606Z Reads: 286

```
My guess is no. The nano receiver outputs a dumb PPM signal. The switch change just limits the PPM output. (I hope I'm wrong and there is some way to get more smart signals via the various switches and buttons.)
```

---
## \#165 Posted by: GreasyGearsWRX Posted at: 2018-12-29T09:14:06.513Z Reads: 273

```
Still hoping to get Bluetooth support for windows or iPhone support. I woukd seriously not like to have to remove this enclosure!
```

---
## \#166 Posted by: Esk88 Posted at: 2018-12-29T09:27:40.329Z Reads: 270

```
double on that iPhone support if you need help raising money to do it I'm sure 10dollars per person and people may throw in some cash so we don't have to find an android every time we wanna fix our ride
```

---
## \#167 Posted by: Esk88 Posted at: 2018-12-29T09:28:56.209Z Reads: 268

```
also does anyone know where I can get a replacement switch online or the name of this one because I think mine stopped working the little button is at a tilt and doesn't properly turn the board off without pressing down increadibly hard
```

---
## \#168 Posted by: GreasyGearsWRX Posted at: 2018-12-29T09:51:14.352Z Reads: 261

```
yeah I'm with @Esk88! I would be happy to throw some money at it to expedite the process!
```

---
## \#169 Posted by: jadatmag Posted at: 2018-12-29T14:09:05.752Z Reads: 259

```
This is very much true.

Wifi cards with included bluetooth modules have pestered me for many years. Most problems get fixed with an external usb bluetooth adapter. Might be worth looking into and advised when flashing firmware over bluetooth from PC.
```

---
## \#170 Posted by: epss4 Posted at: 2018-12-29T18:50:59.675Z Reads: 251

```
I never receive those with my unity -__-
```

---
## \#171 Posted by: epss4 Posted at: 2018-12-29T21:23:46.764Z Reads: 252

```
Do someone here have recommendation for fixing the unity to the deck ?? Thanks you!
```

---
## \#172 Posted by: Scream Posted at: 2018-12-29T21:35:48.877Z Reads: 259

```
Just strong double sided tape is working for me. 

But if you wanted to go fancy you could pick up some longer (say 40mm) M2 bolts and some inserts. Remove the bolts on the Unity, one at a time, and use the longer bolts to fix the Unity to the deck. Please note I am only guessing the dimensions for these bolts! 

Re. the connectors, there should be some 3.5mm male bullet connectors in the pack. They’re not adaptors, they’re to solder on to your motor phase wires.

If you don’t want to change the connectors on your motor some people have been making adaptors using the connectors that came with the unity. You can pick up some 5mm female connectors and shove the 3.5mm male plugs in the other end - apparently it’s a snug fit. Add a bit of solder for guaranteed connection and, most importantly, heat shrink any exposed surface.
```

---
## \#173 Posted by: brenternet Posted at: 2018-12-29T21:43:50.534Z Reads: 260

```
[quote="epss4, post:170, topic:77861, full:true"]
I never receive those with my unity -__-
[/quote]

Guys, that's not an adapter. It's just a male 3.5mm bullet that happens to slide into a 5.5mm.

Every unity came with them.
```

---
## \#174 Posted by: randuin Posted at: 2018-12-29T23:11:54.452Z Reads: 265

```
Just got the Unity setup and it was working well until I closed the lid and now it is doing this

https://www.youtube.com/watch?v=Gr6lYQ3Hen4&feature=youtu.be
```

---
## \#175 Posted by: Blasto Posted at: 2018-12-29T23:13:06.950Z Reads: 265

```
My guess here is your hall sensors, may you have accidentally swapped the ports?
```

---
## \#176 Posted by: randuin Posted at: 2018-12-29T23:14:19.767Z Reads: 259

```
Hrmmm I've actually redone the calibration and test since putting it back together. Would this not solve the problem?
```

---
## \#177 Posted by: Blasto Posted at: 2018-12-29T23:16:15.794Z Reads: 256

```
Well the sensors need to be in their respective port, it will pass the test. Double check that and redo a calibration
```

---
## \#178 Posted by: epss4 Posted at: 2018-12-30T00:07:44.917Z Reads: 255

```
Thanks man :)!
```

---
## \#179 Posted by: venom121212 Posted at: 2018-12-30T00:34:11.758Z Reads: 252

```
Speak for yourself. Mine came with only male 3.5mm bullets.
```

---
## \#180 Posted by: Blasto Posted at: 2018-12-30T00:35:54.716Z Reads: 250

```
It only comes with 3.5mm bullets
```

---
## \#181 Posted by: venom121212 Posted at: 2018-12-30T00:37:23.183Z Reads: 253

```
Fine by me. I wasn't expecting them. I had just seen 2 people now saying the adapters were included.
```

---
## \#182 Posted by: epss4 Posted at: 2018-12-30T00:39:45.234Z Reads: 247

```
Me 2..not the female
```

---
## \#183 Posted by: venom121212 Posted at: 2018-12-30T00:43:39.400Z Reads: 253

```
Just to clarify, did your unity come with the 5.5mm female bullets? Not a big deal, just curious now.
```

---
## \#184 Posted by: Blasto Posted at: 2018-12-30T00:44:19.790Z Reads: 253

```
[quote="venom121212, post:183, topic:77861, full:true"]
Just to clarify, did your unity come with the 5.5mm female bullets?
[/quote]

No only 3.5mm male
```

---
## \#185 Posted by: venom121212 Posted at: 2018-12-30T00:46:22.412Z Reads: 249

```
I agree with your statement that the unity is shipped with only the 3.5mm male. That is prefectly fine with me :slight_smile: I am disputing nothing.
```

---
## \#186 Posted by: Jc06505n Posted at: 2018-12-30T00:46:51.990Z Reads: 242

```
I was Lowkey hoping you would ask one more time jsut so blasto could use the “you dense motherfucker” meme
```

---
## \#187 Posted by: venom121212 Posted at: 2018-12-30T00:48:41.329Z Reads: 244

```
Dumbass I didn't ask him a single time. I asked the guy who originally posted about it asking where he could get more that **IN HIS WORDS** "came with the unity". I clearly stated I was just curious if **he** got them. Read then post.
```

---
## \#188 Posted by: brenternet Posted at: 2018-12-30T01:00:20.804Z Reads: 244

```
Fuckin' Justin. **GOD.**
```

---
## \#189 Posted by: Jc06505n Posted at: 2018-12-30T01:15:29.507Z Reads: 262

```
[quote="venom121212, post:187, topic:77861"]
Dumbass
[/quote]

![takeiteasyman](https://i.imgur.com/jpip1hU.jpg)

[quote="venom121212, post:187, topic:77861"]
I didn’t ask him a single time.
[/quote]

Notice the lack of "him", "he", "she", or "it"  when I said 

[quote="Jc06505n, post:186, topic:77861"]
hoping you would ask one more
[/quote]

Notice how the hope was not related to whom you was asking but how many times you commented on the topic , 

[quote="venom121212, post:179, topic:77861, full:true"]
Speak for yourself. Mine came with only male 3.5mm bullets.
[/quote]

[quote="venom121212, post:181, topic:77861, full:true"]
Fine by me. I wasn’t expecting them. I had just seen 2 people now saying the adapters were included.
[/quote]

[quote="venom121212, post:183, topic:77861, full:true"]
Just to clarify, did your unity come with the 5.5mm female bullets? Not a big deal, just curious now.
[/quote]

Also notice how what i said was a joke

[quote="Jc06505n, post:186, topic:77861, full:true"]
I was Lowkey hoping you would ask one more time jsut so blasto could use the “you dense motherfucker” meme
[/quote]

Meme in question: 
![](https://i.kym-cdn.com/entries/icons/original/000/013/005/3mLydMU.png)

I'll try to keep in mind that New York Humor isn't taken very well everywhere, my fault for any upsets made
```

---
## \#190 Posted by: brenternet Posted at: 2018-12-30T01:24:21.088Z Reads: 242

```
Calm down now, this is a non issue.

It comes with 3.5mm male ends (similar to your willy size) to match the super tiny female ends on the unity. This was a nice and unexpected little addition from our boys at enertion.
```

---
## \#191 Posted by: Scream Posted at: 2018-12-30T01:29:18.171Z Reads: 243

```
Guys I just got my unity and it didn’t include the gold plated top cover.

...I’m adding heat sinks to my trucks in retaliation.
```

---
## \#192 Posted by: billappleton Posted at: 2018-12-30T01:30:46.625Z Reads: 241

```
I got a bunch of extra stuff with mine
```

---
## \#193 Posted by: randuin Posted at: 2018-12-30T07:11:23.745Z Reads: 241

```
This was it! Thanks!
```

---
## \#194 Posted by: mikenyc Posted at: 2018-12-30T17:21:58.697Z Reads: 244

```
Got around to setting up the unity today. Getting an error about the firmware being too old. When I try to upload the firmware on the firmware tab, it fails and gives me the same error. Any ideas?

Note the FW Data Write Timeout 

@Blasto 

@Deodand

 ![40%20PM|690x459](upload://ujxfBd1zK9HfQg0bfEXzdxKHSKE.png)
```

---
## \#195 Posted by: CarlCollins Posted at: 2018-12-30T18:22:04.294Z Reads: 234

```
@mikenyc
Connecting Unity via Bluetooth or USB-C?
```

---
## \#196 Posted by: mikenyc Posted at: 2018-12-30T18:29:45.625Z Reads: 237

```
Bluetooth. USB-C to USB-C on this brand new pixel slate does nothing when tapping on the USB button. Is there a connection log avail to see where it’s failing?

Tried it on 2 different Unity’s. Same result. It’s either a device setting or a bug in the app.
```

---
## \#197 Posted by: CarlCollins Posted at: 2018-12-30T18:32:35.935Z Reads: 234

```
Are you available for a quick team viewer session?
I think I am able to solve it
```

---
## \#198 Posted by: mikenyc Posted at: 2018-12-30T18:33:19.783Z Reads: 230

```
TeamViewer on an Android Pixel?

Edit: no shit, didn’t know that existed
```

---
## \#199 Posted by: mikenyc Posted at: 2018-12-30T18:35:52.084Z Reads: 228

```
Just installed it
```

---
## \#200 Posted by: CarlCollins Posted at: 2018-12-30T18:35:53.909Z Reads: 233

```
@mikenyc
On Windows PC, it will be best
```

---
## \#201 Posted by: mikenyc Posted at: 2018-12-30T18:36:35.873Z Reads: 230

```
I don’t have windows, and I don’t have my Mac here
```

---
## \#202 Posted by: mikenyc Posted at: 2018-12-30T18:37:42.285Z Reads: 235

```
I just PM’d you the ID
```

---
## \#203 Posted by: Deodand Posted at: 2018-12-31T15:55:16.183Z Reads: 242

```
For reasons unknown I've been unable to get the usb-c to usb-c working. The firmware timeout thing seems to happen on certain tablets phones gotta figure out why still. Sometimes I've found improving the reception path between unity and phone can help but not always. 

I can get a mac version built in the next few days that will be most stable way to update firmware of USB C. Ultimately the plan is to get a local app built which will have much better stability.
```

---
## \#204 Posted by: Indiangummy Posted at: 2018-12-31T16:39:42.895Z Reads: 249

```
Do I need to do anything different during setup if I'm running just one motor on the unity?
```

---
## \#205 Posted by: Deodand Posted at: 2018-12-31T17:46:55.243Z Reads: 241

```
You just need to use the tool and not the app unless you have a spare motor you can plug in during setup. I need to patch the app to allow single motor detection to pass.
```

---
## \#206 Posted by: Indiangummy Posted at: 2018-12-31T17:51:40.556Z Reads: 240

```
Alirght thanks. I took one look at the tool and went back to the app 🤣🤣. I assume I can still run foc with one motor?
```

---
## \#207 Posted by: Deodand Posted at: 2018-12-31T17:58:49.711Z Reads: 245

```
Yeah everything will work great, if you just have a spare motor you can plug in during detection it will pass in the app. Then just unplug the second motor and be sure the leads for motor two are secured down and electrically insulated from one another. 

If you wait about 1-2 weeks I'll be pushing an update with a bunch of bugfixes for things we have found this being one, it will just throw a warning instead of an error saying only one motor was detected successfully.
```

---
## \#208 Posted by: brenternet Posted at: 2018-12-31T18:12:57.621Z Reads: 237

```
I've not opened up my unity boxes yet Jeff!

Will we be able to update via the app?
```

---
## \#210 Posted by: Deodand Posted at: 2018-12-31T18:29:20.621Z Reads: 242

```
yeah the update I am referring to will be the app. So far no pressing bugs in the unity firmware have been found. Probably the next firmware update will come when I find a solution to smooth out low speed braking
```

---
## \#211 Posted by: chopper064 Posted at: 2019-01-02T04:08:25.673Z Reads: 244

```
Still having issues with Hall sensor detection. Tried 2 completely different motors (maytech 6374 170Kv and TB 6380 170Kv) and brand new Hall sensor wires as well. Everytime I run through the motor wizard it tells me the hall sensor detection failed. I saw where @Deodand said it was a bug and the detection completed successfully but that is clearly not the case with mine. One motor seems to work fine and the other tends to go in the opposite direction sometimes, studders sometimes then works sometimes. I was told by @CarlCollins that it was your form of "traction control" in FOC mode and yet today Rizwan told me the unity default is BLDC. Perhaps I'm wrong but that seems to be conflicting info. 

I have sent an email with the links to the videos to support@enertionboards.com. It appears to only happen to a single motor at a time and when I switch the leads the opposite motor is then affected.

I was told it was going to be escalated but my original inquiry was over a week ago with Carl and then again a few days ago with Eric and now again today with Rizwan.

Waiting for a resolution in hopefully a very timely manner.
```

---
## \#212 Posted by: Rod12579 Posted at: 2019-01-03T03:37:31.558Z Reads: 234

```
So yeah I can’t get a good detection on my motor as well using the unity tool (FOC)... when asked to spin the motor by hand....any solutions to this??
```

---
## \#213 Posted by: Blasto Posted at: 2019-01-03T04:09:06.938Z Reads: 243

```
[quote="chopper064, post:211, topic:77861"]
It appears to only happen to a single motor at a time and when I switch the leads the opposite motor is then affected.
[/quote]

Sounds like one of your motors sensor pcb is a bit wonky. Just to be sure, you cannot swap both sensor connectors, each sensor must go to it's respective port, left phases go with left port, right phases go with right port.

[quote="Rod12579, post:212, topic:77861"]
I can’t get a good detection on my motor as well using the unity tool (FOC)… when asked to spin the motor by hand…any solutions to this??
[/quote]

might need faster spinning, try doing the detection with the drive train on. The flux linkage is calculated with the back emf, if not enough back emf is created, that step will fail
```

---
## \#214 Posted by: danwooller Posted at: 2019-01-03T13:10:13.505Z Reads: 240

```
I have an issue where flooring the throttle causes one motor to stutter or run backwards slowly. Wind in gently and all is well.

I've swapped over each component progressively and the problem stays with one side of the Unity. Also removed the sensors with the same result.

Anyone seen this?

The motors are brand new TB6355s.![IMG_20190103_131339|666x500](upload://caschuAQoWbZ2wLlLVhvbx5qxZF.jpeg)
```

---
## \#215 Posted by: Blasto Posted at: 2019-01-03T14:09:45.859Z Reads: 236

```
Sounds like you are always in unsensored mode. Do you perform a motor detection every time you do a swap?

Do you get a good detection from the sensors, you seem to have spliced all the wires.
```

---
## \#216 Posted by: danwooller Posted at: 2019-01-03T15:02:15.951Z Reads: 236

```
I run through the quickstart every time I make a change. The splice is because the JST on the 6355 is a different size. the sensors all populate in setup. I've swapped those cables as well, issue doesn't move.
```

---
## \#217 Posted by: deucesdown Posted at: 2019-01-03T15:23:44.535Z Reads: 232

```
Did you just connect the unity's bullets right to the MT60? Haha.
```

---
## \#218 Posted by: Blasto Posted at: 2019-01-03T15:58:41.521Z Reads: 238

```
what results do you get in the hall sensor detection?

![image|407x499](upload://hG5DfTVKeadGMhcCFKMJfYmiSux.png)
```

---
## \#219 Posted by: danwooller Posted at: 2019-01-03T16:26:16.797Z Reads: 232

```
OK, I have a fix. I couldn't connect the android app in my phone, so used my old Nexus 9 and ran the guided setup again. All working perfectly now. So I guess there's something in my Windows 10 setup that was sending duff config to one side. Thanks for taking the time to help @Blasto

 @deucesdown yep, do you have a problem with that?
```

---
## \#220 Posted by: Blasto Posted at: 2019-01-03T17:02:03.334Z Reads: 233

```
Interesting, you were using usb with win10?
```

---
## \#221 Posted by: danwooller Posted at: 2019-01-03T17:26:14.108Z Reads: 235

```
Yep, cable from the box
```

---
## \#222 Posted by: billappleton Posted at: 2019-01-03T17:49:04.154Z Reads: 233

```
I am wondering about the release date of the next version, and firmware. do we have one?
```

---
## \#223 Posted by: Indiangummy Posted at: 2019-01-03T20:29:53.385Z Reads: 234

```
anyone using the hoyt remote with the unity? im trying to calibrate the remote but when i do the calibration through the app it the center stays at 33% i cant get the center of the throttle to 0%

Eidt: @billappleton did you have any luck with the hoyt?
```

---
## \#224 Posted by: billappleton Posted at: 2019-01-03T21:03:03.427Z Reads: 238

```
YES, Jeffrey said that is a "visual display bug" in the software interface. For some reason my readout says -19%. I did not see this problem in the WIN TOOL software. I would recommend calibrating on Mode 3 and proceeding as if nothing was wrong. But that is why (among other reasons) I was asking about new firmware/software to address some of these issues.
```

---
## \#225 Posted by: Indiangummy Posted at: 2019-01-03T21:55:00.891Z Reads: 245

```
Got it thanks. I went on a test ride and it felt normal so I think it is just a visual bug.
```

---
## \#226 Posted by: Indiangummy Posted at: 2019-01-03T22:39:48.395Z Reads: 236

```
Also @Deodand I can't seem to be able adjust voltage cutoff's. That option is greyed out for me.
```

---
## \#227 Posted by: Deodand Posted at: 2019-01-03T23:30:32.117Z Reads: 237

```
you select custom from drop down menu if you want to adjust. Otherwise just select number of cells in your pack.
```

---
## \#228 Posted by: Indiangummy Posted at: 2019-01-03T23:51:41.986Z Reads: 236

```
yeah the drop down menu is greyed out for me. it only lest me select the number of cells.
```

---
## \#229 Posted by: Deodand Posted at: 2019-01-03T23:56:06.984Z Reads: 231

```
under number of cells one of the selections is custom voltage. select that it becomes un-greyed
```

---
## \#230 Posted by: Indiangummy Posted at: 2019-01-03T23:57:57.263Z Reads: 231

```
ahhh ok thanks! am dumb :grinning:
```

---
## \#231 Posted by: 701Superjet Posted at: 2019-01-04T22:19:15.210Z Reads: 236

```
I also can't get my remote to calibrate to zero. I can trim it out but then I can't get full brake or throttle. I'd love to be able to calibrate the max inputs and also manually set the neutral point.  To get the full throttle and brake my netural point is about 20%.  @Deodand will this be in the next firmware update? I sure would appreciate it! Sorry I posted this in the main Unity form as well.
```

---
## \#232 Posted by: 701Superjet Posted at: 2019-01-04T22:21:48.719Z Reads: 231

```
Is there a way to read the battery amps being pulled from the pack? I'm going to buy a watt meter but if the Unity can tell me then that would be great!
```

---
## \#233 Posted by: accrobrandon Posted at: 2019-01-08T23:51:32.095Z Reads: 228

```
does the unity have any type of conformal coating on it? I was looking at mine and it has a mild sheen (or something) and was just wondering if that was the case... thx
```

---
## \#234 Posted by: Deodand Posted at: 2019-01-08T23:53:13.729Z Reads: 229

```
yes it does, this is a last line of defense against water ingress.
```

---
## \#235 Posted by: accrobrandon Posted at: 2019-01-08T23:55:34.641Z Reads: 231

```
cool thx... i had my bottle ready to glaze it over but no need to do double work... guess ill just have to find something else to water proof and give me that sense of "daily accomplishment" ;)
```

---
## \#236 Posted by: kalebludlow Posted at: 2019-01-09T00:09:13.136Z Reads: 229

```
Damn I bet that makes @b264 very happy
```

---
## \#237 Posted by: b264 Posted at: 2019-01-09T00:20:36.141Z Reads: 238

```
[quote="accrobrandon, post:233, topic:77861, full:true"]
does the unity have any type of conformal coating on it? I was looking at mine and it has a mild sheen (or something) and was just wondering if that was the case… thx
[/quote]

I bet the sheen glows under blacklight ;-)
```

---
## \#238 Posted by: jippijuk Posted at: 2019-01-10T07:18:23.263Z Reads: 234

```
Its NOT extremely simple , in my experience its NOT true .

where to read  any manual how to get connection between unity and microsoft software ?

bluetooth is paired but no connection...

USB says serial port error - what the heck is this ?
please  any help before i put a stihl chainsaw engine on my board , lol
```

---
## \#239 Posted by: Scream Posted at: 2019-01-10T08:56:23.905Z Reads: 229

```
Bluetooth doesn’t work except on android.

Sounds like a driver issue with USB - I’m sure someone will chime in with some help with that.

Have you tried the chat on the enertion website?
```

---
## \#240 Posted by: CarlCollins Posted at: 2019-01-10T20:56:31.233Z Reads: 235

```
Windows Users can follow this guide if they are having issues with the COM Port Registering and having Serial port I/O error on the tool
https://enertionboards.zendesk.com/hc/en-us/articles/360000691035-Unity-is-showing-Serial-Port-I-O-error-in-Windows-using-FOCBOX-Tool-or-UI-What-should-I-do-
```

---
## \#241 Posted by: jippijuk Posted at: 2019-01-11T06:03:43.346Z Reads: 231

```
Carl is the Camp , he helped me and fixed the connection . big thanks to carl and you , suggesting .
```

---
## \#242 Posted by: jippijuk Posted at: 2019-01-11T06:22:45.544Z Reads: 238

```
Ok, my usb connection seams stable. now I would like to know where to read the manual or anything to get info about how to setup the nude sexy " unity" ?
Because the 2 min wizard set up does NOT work. 
Ive tried this and both motors are rattling like earthquake 9.
the experimental IOS iMac version works better . the only thing I can not ( or better don't know how to fix ) is with the iOS experimental version is , both wheels are spinning with different RPM's, starting and braking of spinning is not synchrony of both wheels.
So, that's why I spend money to get a Laptop Microsoft win 10 extra for my Board- expensive marriage ,lol 
so the specs are:
- two  ZIPPY Flightmax 5000mAh 5S1P 40C in series - so 10C
-two Turnigy D5035-125KV Sensored Brushless Motor
- 8 inch wheels
- HK-GT2B ( sucks, but works for now)
I'm open to any help.
```

---
## \#243 Posted by: CarlCollins Posted at: 2019-01-11T06:29:11.436Z Reads: 228

```
Would like to have a team viewer session to investigate,
Let me know what time suits you the best
```

---
## \#244 Posted by: jippijuk Posted at: 2019-01-11T07:09:41.918Z Reads: 228

```
now?
BTW my computer guy confessed _ im the administrator at my laptop
```

---
## \#245 Posted by: epss4 Posted at: 2019-01-11T13:12:02.030Z Reads: 229

```
You have the ios app??
```

---
## \#246 Posted by: briman05 Posted at: 2019-01-11T14:57:10.012Z Reads: 224

```
You can use a mico usb panel mount and have it on the outside so you dont have to take of the enclosure every time.
```

---
## \#247 Posted by: dougpage Posted at: 2019-01-11T17:34:59.626Z Reads: 217

```
This might have been already answered but I can't find it. How do you set a max speed on a unity through the focbox ui?
```

---
## \#248 Posted by: Deodand Posted at: 2019-01-11T18:44:42.753Z Reads: 215

```
Something I need to add still.
```

---
## \#249 Posted by: billappleton Posted at: 2019-01-11T19:03:54.368Z Reads: 208

```
I wish the ramp accelerate and ramp break time were in the standard interface also. Maybe have an “advanced” tab to keep the ui clean
```

---
## \#250 Posted by: epss4 Posted at: 2019-01-11T19:06:56.166Z Reads: 208

```
How can i get the experimental ios app :)? 
Thanks
```

---
## \#251 Posted by: jippijuk Posted at: 2019-01-11T21:30:12.470Z Reads: 208

```
I contacted Carl at the enertion page . I try to find the link and than sending it to you . I tried this on my IMac it works kind of . Result is every time different. Also both wheels spinning with different RPMs, start and stop not synchronized, don’t know how to fix this . Bought a cheap Microsoft laptop and try to work with this
```

---
## \#252 Posted by: CarlCollins Posted at: 2019-01-11T21:59:09.498Z Reads: 206

```
@epss4
Will share once I have it :slight_smile:
```

---
## \#253 Posted by: CarlCollins Posted at: 2019-01-11T21:59:41.250Z Reads: 206

```
@jippijuk
I am availble now for team viewer session, Inbox me on forum
```

---
## \#254 Posted by: jippijuk Posted at: 2019-01-11T22:06:49.490Z Reads: 204

```
Hi Carl , sorry I’m at work and can’t leave . 2pm here . Could leave in 3hours and at home in 3:5 hours . Would that work ?
```

---
## \#255 Posted by: jippijuk Posted at: 2019-01-11T22:09:16.392Z Reads: 200

```
I’m logged in here with my phone , try to find some info , screen shots, any help to set up my unity . But can not find anything . And the self detection from the unity does not work .
```

---
## \#256 Posted by: CarlCollins Posted at: 2019-01-11T22:24:28.961Z Reads: 198

```
Let me know whenever you reach home
```

---
## \#257 Posted by: jippijuk Posted at: 2019-01-11T22:35:18.348Z Reads: 198

```
I. Promise champ
```

---
## \#258 Posted by: jippijuk Posted at: 2019-01-12T02:12:00.634Z Reads: 202

```
ready when you are , thanks for waiting
```

---
## \#259 Posted by: Sn4pz Posted at: 2019-01-12T02:13:55.219Z Reads: 201

```
@CarlCollins :arrow_up: :)
```

---
## \#260 Posted by: CarlCollins Posted at: 2019-01-12T02:29:26.486Z Reads: 203

```
Ready now, inbox the ID and password of teamViewer
```

---
## \#261 Posted by: jippijuk Posted at: 2019-01-12T02:31:58.069Z Reads: 200

```
rrrretelklh so ist es
```

---
## \#262 Posted by: Sn4pz Posted at: 2019-01-12T02:33:24.113Z Reads: 208

```
You should delete this, I would be worried of remote highjack

use PM for private chats![image|690x254](upload://sSPyP53X7Icjv09jtaZjr1ICQXX.png)
```

---
## \#263 Posted by: CarlCollins Posted at: 2019-01-12T02:33:41.785Z Reads: 202

```
You should be inboxing that information man
```

---
## \#264 Posted by: Sn4pz Posted at: 2019-01-12T02:34:57.411Z Reads: 206

```
Just noticed, your bio link is wrong :) 

I noticed the , in the screenshot :rofl:

Im on a roll :crazy_face:
```

---
## \#265 Posted by: jippijuk Posted at: 2019-01-12T02:35:22.864Z Reads: 207

```
its deleted 
and I was wondering why you asking this here
```

---
## \#266 Posted by: CarlCollins Posted at: 2019-01-12T02:36:18.093Z Reads: 200

```
@jippijuk
I specifically asked you to inbox the credentials,
i am not on chats because of my off days
```

---
## \#267 Posted by: jippijuk Posted at: 2019-01-12T02:37:33.511Z Reads: 197

```
I have zero clue what inboxing is, man. My skills are at a different area ...
```

---
## \#268 Posted by: CarlCollins Posted at: 2019-01-12T02:38:00.563Z Reads: 201

```
@Sn4pz Posted a screenshot about it
open my profile, click message (blue box)
```

---
## \#269 Posted by: Sn4pz Posted at: 2019-01-12T02:38:30.458Z Reads: 206

```
okies     

char
```

---
## \#270 Posted by: danwooller Posted at: 2019-01-15T12:44:37.402Z Reads: 208

```
I've lost power to the battery meter. It showed up while initially setting up, but now I'm testing and putting the final parts together, it's dead. I've got three and all are dead.

Is there a fuse that I could have blown?

![_SX425_|425x425](upload://7n2BedAmdmuVjZCIS5vh3GXJfoq.jpeg)
```

---
## \#271 Posted by: Blasto Posted at: 2019-01-15T15:22:40.179Z Reads: 204

```
R88 right beside the connector is a 300mA fuse, if it's blown it would need to be replaced. Those LCD's take less than 10mA, either the polarity was wrong or there's a problem with your LCD. The fuse would have not blown for nothing.
```

---
## \#272 Posted by: Battosaii Posted at: 2019-01-15T15:38:12.997Z Reads: 205

```
Tried it out but I have to update my OSX on my old MacBook pro to use the Unity software.
```

---
## \#273 Posted by: Battosaii Posted at: 2019-01-15T15:38:53.684Z Reads: 204

```
Will the UI be updated to show all 4 motors if we run 4wd?
```

---
## \#274 Posted by: danwooller Posted at: 2019-01-15T16:43:11.168Z Reads: 207

```
@Blasto thanks for that. Is that user replace or RTB? I can't see the fuse, I presume it's under what looks like thermal paste and I don't want to start dismantling for no reason.
```

---
## \#275 Posted by: deucesdown Posted at: 2019-01-15T16:47:56.483Z Reads: 209

```
[quote="Blasto, post:271, topic:77861"]
The fuse would have not blown for nothing.
[/quote]

https://www.youtube.com/watch?v=298QWlHtNaQ
```

---
## \#276 Posted by: Blasto Posted at: 2019-01-15T16:49:22.612Z Reads: 207

```
it's a 0603 pcb mounted fuse, circled in red

![image|375x295](upload://2mkvj017NedvZLYhBKEjdq9qPlI.jpeg) 

[acceptable replacement](https://www.digikey.ca/product-detail/en/bourns-inc/SF-0603FP0375F-2/SF-0603FP0375F-2CT-ND/8635560) or just short it out with a small wire
```

---
## \#277 Posted by: Blasto Posted at: 2019-01-15T16:58:47.583Z Reads: 206

```
thanks for that, had a good laugh, "oh no i didn't spill anything on my laptop never ever"  *tons of water damage*

Luckily the fuse did blow to prevent any further damage :+1:
```

---
## \#278 Posted by: danwooller Posted at: 2019-01-15T19:22:40.925Z Reads: 205

```
@Blasto that's fantastic, above and beyond.

There was thermal paste over that, it looks far too small for my dodgy eyes to get out. Bridged it with a screwdriver and no joy.
```

---
## \#279 Posted by: Battosaii Posted at: 2019-01-16T18:25:48.530Z Reads: 209

```
Made some adapters and hooked up my Unity and wow it's so simple and clean. I am running and older version of OSX so the Unity Tool does not work on my laptop but I did the entire set up on my Android phone and everything worked flawlessly. 

@onloop I'm actually impressed this product lives up to the Hype. I asked my self why I would buy a Unity before my Focboxes blew up and now I understand just how much better and convenient the Unity is.
```

---
## \#280 Posted by: mikenyc Posted at: 2019-01-17T23:51:10.098Z Reads: 205

```
@Deodand what's the power output for the led on the power switch? instructions for button that i have says i need to add a resistor if the source is > 3v
```

---
## \#281 Posted by: Blasto Posted at: 2019-01-17T23:52:55.825Z Reads: 209

```
No need for a resistor, it’s on the Unity

![image|690x388](upload://uAneONcL35J8d56bbZO8YiWZp8Y.jpeg) https://www.electric-skateboard.builders/uploads/db1493/original/3X/6/c/6cada3ce16220ada71529f4ae26ee5626cfdf2bb.jpeg
```

---
## \#282 Posted by: Arzamenable Posted at: 2019-01-18T17:05:26.584Z Reads: 208

```
The unity is great so far! 

Only constructive comment to add, maybe the FOC_UI program could have a higher top speed than 35mph. Even if it’s the 1% of folks needing to see those numbers. The hardware certainly seems to support the 1% which is more than anyone could ask for. 🤙
```

---
## \#283 Posted by: Deodand Posted at: 2019-01-18T17:23:44.182Z Reads: 208

```
Sure I'll make it an option in the settings tab.
```

---
## \#284 Posted by: Ian-mountainboard Posted at: 2019-01-18T19:14:34.550Z Reads: 206

```
would anyone recommend this for a mountain board or should i just buy 2 max 6 esc's
```

---
## \#285 Posted by: SeanHacker Posted at: 2019-01-18T19:35:35.225Z Reads: 202

```
Probably the 3rd or forth time you've asked this in these threads. So I'll try and help you out. Sure it is. But so are other vescs. Depends on what you're looking for features wise, size of the units, durability, ect... Pull the trigger dude
```

---
## \#286 Posted by: Sn4pz Posted at: 2019-01-18T19:35:58.845Z Reads: 199

```
mate, we all have recommended the Unity

Not to be mean or anything, I just dont see why youre asking again :thinking:

Obviously if you want it asap - ordering through the Enertion website is going to take awhile, unless you find someone selling theirs from the preorder or if they had some other option - go with the max 6
```

---
## \#287 Posted by: Ian-mountainboard Posted at: 2019-01-18T19:44:56.826Z Reads: 198

```
Ok. Sorry it's just a lot of money and just trying to get a wide spectrum of reviews and thoughts so I can make the right deshion the first time. Dident mean to piss anyone off.
```

---
## \#288 Posted by: Sn4pz Posted at: 2019-01-18T19:51:33.543Z Reads: 202

```
Youre not making anyone angry, we just dont like to repeat ourselves :joy: 

I think that your money is wasted on the max 6 when the Unity is only slightly less (regular retail price)

The customizability of it

The design is vastly superior

Foc mode(not sure if the max has this, but I mean come on who doesnt love the idea of silent zoomies) 

and most importantly the support behind it, Blasto and Carl are the only reasons I was comfortable with the purchase, I knew and still know that if something happens out of the norm, I can depend on the customer service I need for an item like this

e: also Ive heard mixed reviews about the breaks on the max 6, some are either very jarring or others seem to have it dialed in perfectly.... I wouldnt take the chance to have one unit that functions well and one that doesnt :crazy_face:
```

---
## \#289 Posted by: Ian-mountainboard Posted at: 2019-01-18T20:01:41.615Z Reads: 189

```
Ok ive made up my mind and im buying the max 6 tonight
```

---
## \#290 Posted by: Ian-mountainboard Posted at: 2019-01-18T20:02:06.746Z Reads: 194

```
Jk😂

Defiantly unity
```

---
## \#291 Posted by: sofu Posted at: 2019-01-19T00:58:48.776Z Reads: 189

```
Is the motor settings per motor or altogether? I would assume the battery settings is altogether, so if I did 30A on each focbox previously, that means I should do 60A battery max here right?
```

---
## \#292 Posted by: Deodand Posted at: 2019-01-19T01:03:46.719Z Reads: 188

```
Yea, that's correct.
```

---
## \#293 Posted by: sofu Posted at: 2019-01-19T01:23:01.016Z Reads: 189

```
So the motor setting is per motor?
```

---
## \#294 Posted by: Deodand Posted at: 2019-01-19T01:36:57.436Z Reads: 187

```
Ah sorry misread a bit, yeah motor setting is per motor and battery setting is all together.
```

---
## \#295 Posted by: Rod12579 Posted at: 2019-01-19T02:41:55.478Z Reads: 198

```
So according to my set up @ 50a battery max = to 25a per focbox?? 🤔![image|243x500](upload://qIEIW0VY8YoNFWHelB35ohGAPh5.jpeg)
```

---
## \#296 Posted by: Ian-mountainboard Posted at: 2019-01-19T03:08:37.331Z Reads: 197

```
Don't mean to draw the discussion to another topic but enertion support told me that if I buy the unity now I will receive it late February early March. should I expect that to be true or will the wait be longer?
```

---
## \#297 Posted by: CarlCollins Posted at: 2019-01-19T03:20:57.786Z Reads: 196

```
It's accurate in case of Unity shipments
```

---
## \#298 Posted by: Shanian79 Posted at: 2019-01-19T07:47:22.759Z Reads: 197

```
What’s the ETA for next Unity_UI firmware update?
```

---
## \#299 Posted by: sofu Posted at: 2019-01-19T17:24:49.303Z Reads: 197

```
So somebody else I know and myself has been having this weird issue where if I accelerate too hard, the motor stutters. But if I accelerate slightly not as hard, everything is fine. I'm at battery 80a -30a, motor 95a -60 stock non testing firmware. I'm a bit at a loss as to what the issue is. Confirmed on regular focboxes that my hardware is good.
```

---
## \#300 Posted by: JohnnyMeduse Posted at: 2019-01-19T17:31:19.068Z Reads: 192

```
What Motor do you use?
```

---
## \#302 Posted by: JohnnyMeduse Posted at: 2019-01-19T17:36:07.021Z Reads: 190

```
Those are rated for 65A... trying to push 95A into it might not be good...
```

---
## \#303 Posted by: Indiangummy Posted at: 2019-01-19T17:36:47.688Z Reads: 190

```
Sorry I could be wrong. I'm guessing she's talking about her haya build but I'm not sure. @sofu can you confirm?
```

---
## \#304 Posted by: Indiangummy Posted at: 2019-01-19T17:40:22.222Z Reads: 186

```
Also i think  that's 95A for both motors. So it would be 47.5A per motor
```

---
## \#305 Posted by: JohnnyMeduse Posted at: 2019-01-19T17:41:34.175Z Reads: 192

```
setting are per motor... so it is 95A for each one

[quote="Deodand, post:294, topic:77861, full:true"]
Ah sorry misread a bit, yeah motor setting is per motor and battery setting is all together.
[/quote]
```

---
## \#306 Posted by: sofu Posted at: 2019-01-19T17:49:38.154Z Reads: 199

```
6880s. As far as I'm aware they're rated for 65A continuous which I'm far below, and on acceleration where it stutters I never draw above 50A per. It's not about the motors anyways, since my friend is using sk8s and has the same issue...
```

---
## \#307 Posted by: JohnnyMeduse Posted at: 2019-01-19T17:53:30.771Z Reads: 201

```
[quote="sofu, post:306, topic:77861"]
65A continuous
[/quote]

I don't think it is continuous look more like MAX amp... 60A is continuous I think

![image|345x425](upload://qk1fFMVHcqBaQvLpS1ustaxabfF.jpeg)

MIght not be about the motor, but having the wrong setting for the motor won't help ether, since the motor might not like the overload current.
```

---
## \#308 Posted by: Deodand Posted at: 2019-01-19T17:55:57.784Z Reads: 192

```
Does the stuttering trigger any faults?
```

---
## \#309 Posted by: sofu Posted at: 2019-01-19T17:56:16.131Z Reads: 196

```
Not as far as i know

Edit: Troubleshooting with Jeff in dm to not spam this thread, will post solution!

Edit 2: Have various suggestions, will run through them and post results
```

---
## \#310 Posted by: sofu Posted at: 2019-01-19T18:11:08.252Z Reads: 192

```
You're seemingly correct about the specs actually, though I was told different by a seller on Ali. I'll go with the specs sheet after all on this one...
```

---
## \#311 Posted by: sofu Posted at: 2019-01-19T19:13:15.806Z Reads: 193

```
Ok so the solution is: if you're running FOC sensored, under FOC hall sensor detection set unsensored erpm to 15% more than stock. I have mine at 4500 now and I can pull as hard as I dare without issue. Thanks so much for the quick solution  @Deodand!
```

---
## \#312 Posted by: Silverline Posted at: 2019-01-19T20:29:35.729Z Reads: 193

```
Is this "bug" going to be fix'd in a future update ?
```

---
## \#313 Posted by: Blasto Posted at: 2019-01-19T20:41:51.131Z Reads: 199

```
This is native to the vesc fw, @Deodand was thinking of a way to have that paremeter automatically adjusted with the motor detection. So it is in the works
```

---
## \#314 Posted by: jadatmag Posted at: 2019-01-20T13:17:06.721Z Reads: 206

```
Will we be able to set a different "Beta Value for Motor Thermistor" for each motor in the future update? @Deodand 

Silver motors on a Raptor 2.0 with thermal throttling disabled, took me 5 minutes to get these temps:
![607d2f1e5cf6dbc435b725eacf095400efc69619|264x500](upload://dLA2EoUdxkObkqXTVCft3g3QnJ7.jpeg)

The only solution I have left is to put back my focboxes and flash ackmaniac's firmware to set beta value's that aren't limited to 4-thousand-something
```

---
## \#315 Posted by: goldrabe Posted at: 2019-01-20T13:22:46.120Z Reads: 203

```
What Beta have you set it at?
5 min. sounds too fast for so much heat.
@barajabali what is the correct Beta we should set the motors at?
```

---
## \#316 Posted by: jadatmag Posted at: 2019-01-20T13:51:54.312Z Reads: 199

```
It's currently at stock. My motors temps differ so much that they need to be calibrated individually. Or is one motor really getting so much hotter? Anyway, I don't have the tools or know how to find/calibrate the right number for the Beta value's for left and right.

I don't think a single higher Beta Value for both motors can fix the throttling issues the followings setups should be experiencing:
* Old Raptor 2's with silver replacement motors
* Raptor 2.0 with silver motors
* Raptor 2.1
* Kit buyers

Calibration within a controlled temperature or external temp read out will be necessary.
```

---
## \#317 Posted by: goldrabe Posted at: 2019-01-20T14:09:09.880Z Reads: 195

```
My motor temps where differing similar to yours, I got told that the heelside motors run always hotter.
The default Beta seems to be wrong and Enertion is working on it. But 5 min to 150°C is ridiculous fast and seems to be wrong from my experience.
```

---
## \#318 Posted by: jadatmag Posted at: 2019-01-20T14:22:07.937Z Reads: 199

```
Well the thing is. I have two broken silver motors that only run well uncensored. So Bara send me two new silver motors. The temps you see in the screenshot are from the two new silver motors. Their temperature difference is really big.

So I switched the new silver motor with the 152 Celcius in the screenshow to one of the old Silver motors that doesn't run censored very well.

With the same testing conditions the temperature now only differs about 5 Celcius between the two motors. A temperature difference that seems more logical to me.

So maybe the motor temps really vary that much or maybe the calibrations numbers should be different per every unique motor. Maybe only my 152 Celsius motor is really far off or maybe many more are. I don't know. Not much data to find.

Nothing to find on how to properly calibrate the Beta value. I also don't understand how calibration can be done with a single number. You would atleast need 2 calibration points. One for let's say 10 Celsius and other one for 50 Celsius. A third calibration point will get you even better results.

I there a Beta Value Captain in the house?
```

---
## \#319 Posted by: epss4 Posted at: 2019-01-20T15:11:16.372Z Reads: 187

```
Hi man ! That suck :confused: do you think your motor really get this hot , or its just the software that is bad reading the temp?
```

---
## \#320 Posted by: jadatmag Posted at: 2019-01-20T15:38:25.339Z Reads: 187

```
I'm pretty sure it's a wrong temperature readout.

When I was at a groupride @sayekim had a temp gun with him and he measured something like 50 Celsius on the axle while my Unity app on android was saying 100 Celsius.
```

---
## \#321 Posted by: barajabali Posted at: 2019-01-20T15:38:34.689Z Reads: 185

```
Hello! There will be an update shortly with firmware changes but if you want you can change the beta to 3900 and the temp throttling to 70 start and 165 end
```

---
## \#322 Posted by: jadatmag Posted at: 2019-01-20T15:53:09.240Z Reads: 188

```
Will this also fix the 34 Celsius difference between my 2 motors? Will there be a guide on individual motor temp sensor calibration? Or do I have a single weird motor?

Sorry for all the questions :sweat_smile: I have this huge groupride coming on Feb 5th where we will be renting a go-cart track for 5 hours with 50+ e-boarders and wanne rock that track :smiley:
```

---
## \#323 Posted by: barajabali Posted at: 2019-01-20T15:55:29.547Z Reads: 187

```
I would wait to try the new firmware fix, if that doesnt solve the temp difference then it may be a hardware fault. What is likely happening is that the other motor isn't actually getting much hotter, the sensor is just reading that since the beta is incorrect.
```

---
## \#324 Posted by: Deodand Posted at: 2019-01-20T17:56:02.943Z Reads: 194

```
Can you post a screenshot of your motor calibration in the app? Curious if the winding resistance has a difference (would cause a temperature difference).
```

---
## \#325 Posted by: jadatmag Posted at: 2019-01-20T18:45:31.136Z Reads: 203

```
![1|264x500](upload://2CsMyFzbIchhaj6IFP7M5A0WtwE.png) ![2|264x500](upload://4YOAthozDXMy21G81glpfkLFKGz.png)
```

---
## \#326 Posted by: LanSolo Posted at: 2019-01-20T21:25:39.936Z Reads: 203

```
What would be the best config for 
2x 6374 170kv
10s5p lg 
thanks
```

---
## \#327 Posted by: briman05 Posted at: 2019-01-20T21:30:48.713Z Reads: 200

```
What OS X do you have.
```

---
## \#328 Posted by: Battosaii Posted at: 2019-01-20T23:35:24.322Z Reads: 196

```
I'm running Sierra I need to upgrade to Mohave
```

---
## \#329 Posted by: briman05 Posted at: 2019-01-21T01:55:01.526Z Reads: 191

```
So focbox tool won’t work on anything that isn’t Mohave?

I guess it’s a good thing I didn’t get the unity because I am on El Capitan because I’m running CS6
```

---
## \#330 Posted by: Battosaii Posted at: 2019-01-21T02:24:50.143Z Reads: 198

```
I actually use my Samsung Galaxy s8 plus to set up my board now lol. It's nice to be able to to do motor detection on the fly now.
```

---
## \#331 Posted by: briman05 Posted at: 2019-01-21T02:28:43.090Z Reads: 196

```
I have a iPhone so I’m f’ed all around
```

---
## \#332 Posted by: Shanian79 Posted at: 2019-01-22T21:07:05.096Z Reads: 203

```
Forgive me if this has already been covered, but I'm new to Esk8 scene, I have a lot of experience with ESC and Motor dynamics from years of building R/C Heli's, but some aspects of these ESK8 controllers are new to me so I have a few questions. Any insight is very much appreciated.

1. I have a Unity with R-Spec kit running on 12C1P. I am wondering what exactly "Motor Thermal Throttling" is. Its enabled on my current build, but I have no idea what it actually does or what I should look for when deciding the settings for max motor temp and whatever Motor Beta is. 

2. When I'm riding and back off the throttle to coast, there is more drag from the motors than I want. Is this controlled by the Max Breaking Regen Current Settings?
```

---
## \#333 Posted by: epss4 Posted at: 2019-01-22T21:15:30.983Z Reads: 196

```
Hey man! So the motor temp throttle is when your motor reach the temperature (the one you set) is will decrease power to let the motor cool down ...i think you should set it at 100C-110C ... for your second question i have no idea :confused:
```

---
## \#334 Posted by: trampa Posted at: 2019-01-22T21:41:18.698Z Reads: 192

```
1. https://vesc-project.com/node/183 (You need 15% temp headroom for the brakes!)
2. That is the natural drag of the motors when you coast. No setting will make that any better.
```

---
## \#335 Posted by: AToasterOfDoom Posted at: 2019-01-23T00:55:41.032Z Reads: 193

```
Is it possible to run a single motor on the unity without damaging anything? I broke a motor mount so I'm down to one motor for a few days.
```

---
## \#336 Posted by: Blasto Posted at: 2019-01-23T00:58:29.002Z Reads: 191

```
yes it is possible, just isolate properly the dangling phase leads (electrical tape for temporary use)
```

---
## \#337 Posted by: Indiangummy Posted at: 2019-01-23T01:04:12.178Z Reads: 198

```
Yes but as it stands right now you will have to use the tool for motor detection. Unless you have a spare motor then do motor detection through the app and unplug the spare motor afterwards. @Deodand is working on an update to make this possible through the app.
```

---
## \#338 Posted by: Aero Posted at: 2019-01-28T20:51:04.559Z Reads: 190

```
During motor detection does it make a difference if you leave the belts or gears in place? Thanks
```

---
## \#339 Posted by: Blasto Posted at: 2019-01-28T20:57:42.444Z Reads: 193

```
I would probably recommend leaving the drive train ON. It gives you a mechanical advantage when performing the manual wheel spin (determines wheel direction and flux linkage)
```

---
## \#340 Posted by: Aero Posted at: 2019-01-28T21:23:03.703Z Reads: 186

```
Ok, many thanks.
```

---
## \#341 Posted by: mackann Posted at: 2019-01-28T21:35:29.671Z Reads: 192

```
Wait so it's possible to make a motor wizard with "load" to the motor axle? Before with vesc it was always recommended and very hard to finish motor wizard without removing the belt or gear so the motor could spin free without any roll resistence.
```

---
## \#342 Posted by: Blasto Posted at: 2019-01-28T21:41:52.928Z Reads: 193

```
[quote="mackann, post:341, topic:77861"]
Wait so it’s possible to make a motor wizard with “load” to the motor axle?
[/quote]

Yes, in the guided setup, there's a prompt that ask you to hand spin the wheel in the forward direction.  Because it is attached to the drive train,  hand spinning the wheel will make the motor spin very fast, thus generating enough back emf to calculate the flux linkage.
```

---
## \#343 Posted by: mackann Posted at: 2019-01-28T21:45:55.443Z Reads: 191

```
Oh that's great!
Just mounted apart 6 gear drives because I forgot to run the motor wizard before I assembled it 😂😅 But this is great then I do not have to worry about forgetting to do so before in future.
```

---
## \#344 Posted by: jippijuk Posted at: 2019-01-31T10:47:19.904Z Reads: 204

```
I'm asking for some help, links where I could read basic understandings of the unity setting abbreviations and getting the most of my setup. Im not commenting on enertion support here.
Regarding my board,
-  2 Motor Turingy 5035 125kv
- 2 zippy lipo 5000 40c in serie = 10C
- mountain board mbs comp95, 8'' wheels, 72 teeth wheel side, 16 motor side, chain driven
- unity 
the experimental IOS version doesn't work here, so I bought a microsoft laptop specially for my board  ( what ever is needed to ride the board,lol)
So the problem is after several tests and tries - one motor is running always slower, starting with delay . This is visible in the software focbox UI in HU . Motor 2 is getting less Volt only till full throttle .
The values in motor calibration are always different for each motor .
Is this normal?  Where can I read what these values and abbvrevations mean ? Can I change the max RPM? ![IMG_1734|374x500](upload://kDr5VkrLZW8Nuupbkz1XDXmcLKb.jpeg) ![IMG_1735|374x500](upload://wDhe1togd5Y4zUYDXkXNKOmvvQk.jpeg) 
Thank you for any help , I appreciate any progress input .
```

---
## \#345 Posted by: Blasto Posted at: 2019-01-31T13:29:51.817Z Reads: 191

```
[quote="jippijuk, post:344, topic:77861"]
* 2 Motor Turingy 5035 125kv
* 2 zippy lipo 5000 40c in serie = 10C
* mountain board mbs comp95, 8’’ wheels, 72 teeth wheel side, 16 motor side, chain driven
[/quote]

Those motors are very small for a mountain board. But anyways not the point here.

We can see in the motor detection one of the motors has considerably less inductance making me think the Kv of each could be different, thus the motor speed difference.


Honestly i dont think 5035 will handle 8” tires very well. Might end up overheating and shorting out.
```

---
## \#346 Posted by: Blasto Posted at: 2019-01-31T14:57:54.540Z Reads: 190

```
What you can try, is lower your motor current to 40A
```

---
## \#347 Posted by: jippijuk Posted at: 2019-01-31T15:32:55.606Z Reads: 187

```
Thank you , I will try this. 
In october when I started to gather all information for ordering parts and reading here for many nights ,Ive found this Motor as suitable with lots of torque. But Anyway, what motor in your opinion would fit better for 8" tires and my constellation . I spend now so much money (lol) and don't mind to buy new motors,  want to do it right . And having fun with DIY and rinding :smile:
I noticed that the torque is not really impressive from those 5035. And I thought with my set up is something wrong . Max speed is 34km , range 10k trail and sometimes I'm want more torque .
```

---
## \#348 Posted by: Blasto Posted at: 2019-01-31T15:50:58.188Z Reads: 186

```
on 8" pneumatics,  i'd go for 6374 motors, could probably get away with smaller 6355's, but it will be somewhat sluggish with 6355's.
```

---
## \#349 Posted by: jippijuk Posted at: 2019-01-31T23:57:59.281Z Reads: 188

```
Thank you for your advice , there are different rpm variations of this 6374  available. 146, 168 and the 195. Which one would you use for 8” wheels . I don’t want crazy speed but good torque even in lower speed.
Ok , I kind of assume this question is silly because of my ratio.
Offroad calculation in my case ( and in mind I have three sets of motor sprockets 14, 15, 16teeth)
would you rather go with the 146 kv or 168kv? Is it better to max out these motors to have the advantage of the momentum with the 146 kv or getting the 168 kv an running this motor in max on 80%?  chain driven is always more friction I think but just rock immortal against gravel and dirt .
 Oh , I just checked , all 6374 running on 12C . And I have now 3 new sets of 10C ( because my 5035 are running on 10c) .... any chance for me with the 10C packs to get more torque and little more speed?
```

---
## \#350 Posted by: pookybear Posted at: 2019-02-01T05:53:37.135Z Reads: 189

```
@Deodand 

Is there a firware revision for us who wants to use metr Bluetooth w the feather remote? I was told by @sofu that to get both working, it needs a different firmware.
```

---
## \#351 Posted by: danwooller Posted at: 2019-02-01T13:30:05.191Z Reads: 189

```
Just had a bit of time to look at my dead battery meter. I have 2.3V at the meter, so I don't think it's the fuse.

Can anyone tell me if that's the correct voltage on the two pin connector with a meter attached?
```

---
## \#352 Posted by: PickSix24 Posted at: 2019-02-01T13:59:44.581Z Reads: 190

```
@Deodand Ran into an issue setting up my unity. Ran the setup wizard. While testing on the bench one of my motor will change direction on its own between throttle pulls.
```

---
## \#353 Posted by: fourchette Posted at: 2019-02-01T14:09:06.788Z Reads: 195

```
hello,
I am trying to send rpm commands from a microcontroller to each motor of focbox unity but i struggle.
it seems through app/ppm the same pwm is used to move the two motors synchronously. the foc_openloop / foc_openloop2  (through usb) do not work for me either because i am trying to send erpm target values not current values. 
how should i proceed ?
thanks
```

---
## \#354 Posted by: Deodand Posted at: 2019-02-01T17:59:10.373Z Reads: 186

```
@fourchette Hey I have a FW that supports independent dual channel PPM. It uses one of the pins fro the seven pin header as the input. Would that work for your application?
```

---
## \#355 Posted by: Deodand Posted at: 2019-02-01T18:03:27.417Z Reads: 193

```
@PickSix24 If you are running sensorless motors this corresponds to a bad motor spinup. If you are kickpushing your skateboard off the line before throttling it wont impact your ride. It does indicate a less than optimal motor calibration however. I'd try running motor config again to get the best values. If you want to go more in depth you can download the full tool and  play with motor config-> FOC ->sensorless-> openloop ERPM. You can try increasing this value a bit to get better spinup.
```

---
## \#356 Posted by: pookybear Posted at: 2019-02-01T18:34:41.855Z Reads: 193

```
Do I initially have to connect the unity to PC via USB before I could pair the Bluetooth?

This is what I'm getting everytime I try to connect to it via bluetooth. 

OnePlus 3T
Android 7.1.1

![Screenshot_20190201-103150|281x500](upload://vOPb8a4cZR7mT9D2Dp0xKr2dH6X.jpeg)
```

---
## \#357 Posted by: Deodand Posted at: 2019-02-01T18:41:22.652Z Reads: 180

```
No need to pair. Connect to it from the app.
```

---
## \#358 Posted by: PickSix24 Posted at: 2019-02-01T20:44:24.610Z Reads: 183

```
I’ll try running the setup again. They are sensored motors and the values are pretty equal between the two. Thanks
```

---
## \#359 Posted by: Deodand Posted at: 2019-02-01T20:48:42.765Z Reads: 179

```
post a screenshot of motor config when it runs
```

---
## \#360 Posted by: Jc06505n Posted at: 2019-02-01T23:16:57.606Z Reads: 191

```
Does his mean that my sensors aren’t being detected , I’m using new motors that haven hit the road yet 

![image|317x500](upload://npHELwdjTkoCze2z86kdADWC6pn.jpeg)
```

---
## \#361 Posted by: Blasto Posted at: 2019-02-01T23:43:47.665Z Reads: 183

```
Yeah your halls aren’t being detected at all
```

---
## \#362 Posted by: colinphotovideo Posted at: 2019-02-02T00:22:54.634Z Reads: 189

```
One of my motors won’t detect the hall sensor too but they worked fine before...just transferred from dual focbox to Unity?? 🤔
```

---
## \#363 Posted by: pjotr47 Posted at: 2019-02-02T17:54:12.072Z Reads: 197

```
I see that the bleuthooth in the Windows program don’t work? I have running my trampa but I must change my direction. I don’t want to unscrew 24 screws :sweat_smile:![image|375x500](upload://xAYic6TxBxFATDcO1VEdCKfrSoF.jpeg)
```

---
## \#364 Posted by: PickSix24 Posted at: 2019-02-02T18:19:42.474Z Reads: 190

```
Loose sensor adapter connection. Ran it again and now it’s perfect !
```

---
## \#365 Posted by: GreasyGearsWRX Posted at: 2019-02-04T00:24:32.256Z Reads: 188

```
Is there a ETA on firmware update? Is IOS support coming as well? @Deodand
```

---
## \#366 Posted by: PickSix24 Posted at: 2019-02-04T01:04:02.583Z Reads: 194

```
Anyone have their unity working with metr ?
```

---
## \#367 Posted by: mccloed Posted at: 2019-02-04T01:05:24.512Z Reads: 196

```
Yup! Works great.
```

---
## \#368 Posted by: PickSix24 Posted at: 2019-02-04T01:26:58.708Z Reads: 196

```
:wink:let me rephrase, would anyone mind sharing the settings needed to get it connected. I’ve got my metr connected @9600 but still not seeing and data in the app
```

---
## \#369 Posted by: Indiangummy Posted at: 2019-02-04T01:31:00.981Z Reads: 194

```
Is your metr on the latest FW?
```

---
## \#370 Posted by: PickSix24 Posted at: 2019-02-04T01:46:10.093Z Reads: 194

```
Yes, first thing I did was update it.
```

---
## \#371 Posted by: fourchette Posted at: 2019-02-06T14:07:13.996Z Reads: 197

```
in the end, we reverted back to two separate single VESCs and talk to each of them through UART.

but i would rather use the focbox unity instead with UART. then from microcontroller, then spent different erpm commands to each motor.

=> how can i do that?
```

---
## \#372 Posted by: Deodand Posted at: 2019-02-06T22:20:55.650Z Reads: 202

```
Similar to how you send a command to single vesc you issue the same command over uart to unity but send two current values in the command packet for motors 1&2.

This is normal vesc commend structure snippet:

    case COMM_SET_DUTY:
		ind = 0;
		mc_interface_set_duty((float)buffer_get_int32(data, &ind) / 100000.0);
		timeout_reset();
		break;

	case COMM_SET_CURRENT:
		ind = 0;
		mc_interface_set_current((float)buffer_get_int32(data, &ind) / 1000.0);
		timeout_reset();
		break;

This is unity:

     case COMM_SET_DUTY:
        ind = 0;
        cmd1 = (float)buffer_get_int32(data, &ind) / 100000.0;
        cmd2 =(float)buffer_get_int32(data, &ind) / 100000.0;
        mc_interface_set_duty(cmd1,cmd2);
        timeout_reset();
        break;

      case COMM_SET_CURRENT:
        ind = 0;
        cmd1 = (float)buffer_get_int32(data, &ind) / 1000.0;
        cmd2 =(float)buffer_get_int32(data, &ind) / 1000.0;
        mc_interface_set_current(cmd1,cmd2);
        timeout_reset();
        break;

You can see it reads an extra value from the command packet and that is  the only difference. You'll have to modify the library you use to interface and add in an additional argument to send.
```

---
## \#373 Posted by: murloc992 Posted at: 2019-02-07T08:10:58.170Z Reads: 180

```
@Deodand

What kind of thermistor in the motors Unity expects? I am planning to add custom thermistors in my motors.
```

---
## \#374 Posted by: Blasto Posted at: 2019-02-07T13:53:11.355Z Reads: 186

```
10k, the beta is adjustable
```

---
## \#375 Posted by: BOIE Posted at: 2019-02-07T17:00:05.909Z Reads: 194

```

Hello I really hope someone can help me I just received my focbox unity and I don't know what settings to put in I have a power truck system from diyeboards.com here's the link to the exact system I have http://www.diyeboard.com/10s5p-360wh-battery-esc-dual-motor-belt-drive-power-truck-kit-p-590.html?zenid=ccfb10065bfc4a7693f1781c08260676 I'm a noob anybody's help will be greatfuly appreciate it.
```

---
## \#376 Posted by: Jaydawg56 Posted at: 2019-02-08T20:14:34.205Z Reads: 192

```
Quick question about the 2-pin aux plug on the unity...

The pin is labeled "batt +" in the unity diagram. So does that mean is passes full battery voltage or something like 5V?  I want to use that pin to pass batt voltage to my volt meter, but am not sure what current is passed. 

Thanks for the assist!
```

---
## \#377 Posted by: PickSix24 Posted at: 2019-02-08T23:28:30.285Z Reads: 190

```
It passes full battery voltage. I use it for a voltage display.
```

---
## \#378 Posted by: venom121212 Posted at: 2019-02-08T23:29:51.580Z Reads: 190

```
Good to know, so it'll work with the new maytech  split trigger R2 receiver very nicely.
Exxxxcellllent.
```

---
## \#379 Posted by: Jaydawg56 Posted at: 2019-02-08T23:31:44.318Z Reads: 186

```
Gyeah! Reason why I asked. Gotta get that maytech batt indicator going
```

---
## \#380 Posted by: venom121212 Posted at: 2019-02-08T23:32:30.361Z Reads: 187

```
Do you have the receiver on you? I've heard it's just a single wire coming off for battery but want to see for myself.
```

---
## \#381 Posted by: Jaydawg56 Posted at: 2019-02-08T23:34:15.061Z Reads: 190

```
Yep. Feed the wire through and solder down. 

![image|374x500](upload://fAlnbqOfPzEv1gaGW4ceoo117IN.jpeg)
```

---
## \#382 Posted by: Deodand Posted at: 2019-02-08T23:35:32.067Z Reads: 184

```
Not too pretty is it?
```

---
## \#383 Posted by: venom121212 Posted at: 2019-02-08T23:35:40.282Z Reads: 185

```
Cool so if I just crimp a jst ph 2 pin to the positive, it should be plug and play. Probably ought to ground as well
```

---
## \#384 Posted by: Deodand Posted at: 2019-02-08T23:36:08.428Z Reads: 183

```
The ground will be common don't think I'd worry about it.
```

---
## \#385 Posted by: venom121212 Posted at: 2019-02-08T23:36:41.580Z Reads: 185

```
I almost wish I didn't ask for a picture :face_vomiting:

Good thing it'll be hidden
```

---
## \#386 Posted by: Makio13 Posted at: 2019-02-09T00:14:07.646Z Reads: 189

```
Can you use the regular vesc tool(and the update coming out) with the unity?
```

---
## \#387 Posted by: Deodand Posted at: 2019-02-09T00:29:03.878Z Reads: 191

```
Nope! But trust I'll keep a close eye on the changes and integrate the features that make sense :smile: Excited to see vedder pushing forward even if it's in a slightly different (but parallel) direction.  I expect there will be lots of stuff we can share. Love his foc_openloop detection routine very clever, think I might take a look and add as an option for super high kv motors for instance. I love the hand-spin for most eskate motors though.
```

---
## \#388 Posted by: drangboards Posted at: 2019-02-09T10:44:56.285Z Reads: 190

```
![image|298x500](upload://a1EUPCyeZNdF1Kyrs981cDt4TDd.png) 

I am not sure which tool to use to set this up.  can I get some help?
```

---
## \#389 Posted by: CarlCollins Posted at: 2019-02-09T11:15:52.690Z Reads: 180

```
Already provided you the right tool to program it, now it will work with FOCBOX UI app as well @drangboards
```

---
## \#390 Posted by: drangboards Posted at: 2019-02-10T09:59:27.444Z Reads: 185

```
Dude, this thing is a missile!  I need to raise the braking power.  You imagine I can handle doing that on my own?  I can't remember what it is set at.
```

---
## \#391 Posted by: taz Posted at: 2019-02-10T10:37:19.776Z Reads: 190

```
![20190210_123605|243x500](upload://nvgdg3I4YHRI6QKn3dsvfekhWnY.jpeg) 

Think of Bat regen as your high speed brakes and motor brake current as your low speed brakes.
```

---
## \#392 Posted by: drangboards Posted at: 2019-02-10T10:50:57.741Z Reads: 186

```
How about this then?  It was already -15 and -30...  It feels weak at that. ?
![image|295x500](upload://qtmjoQY0kLo1Vht69ai6EE4qb2B.png)
```

---
## \#393 Posted by: Blasto Posted at: 2019-02-10T16:36:31.829Z Reads: 186

```
I was asked this question via pm, since i think this info should be public.

Q: 
Motor: 270Kv N5055 outrunner 1400W
Battery: 10S2p sanyo 30A continuous
What are the recommended settings?

A:
Motor max: 30A
Motor min: -30A
Batt max: 30A
Batt min: -10A
```

---
## \#394 Posted by: CarlCollins Posted at: 2019-02-10T20:07:22.709Z Reads: 185

```
@drangboards
You just need to adjust the braking current, make sure your remote is set to R-Spec mode
```

---
## \#395 Posted by: Deodand Posted at: 2019-02-10T21:06:43.072Z Reads: 191

```
![image|690x461](upload://8ZW1KRIU0Dpv4EDaoR5XczJg74n.jpeg)
 
Switch on the back of the remote should be down position.
```

---
## \#396 Posted by: jippijuk Posted at: 2019-02-11T04:46:57.580Z Reads: 193

```
question about unity settings and different power out come for motor1 and motor2.

For the records my setup was the following:
-mountain board, 8" tires, 
-chain driven 72 -16, 
-turingy 5035 125kv, 
-two 5s lipos 5000mAh 40C in series
I'm careful and very precise with connections and soldering
used the focboxUI
and after several tries ( I mean several) Motor 2 was always slow starting , with less RPM's
I was able to ride my board for four or five test rides and figured  that this motors are too small. 
Asking for help at the enertion support and here at the forum and been told , 
the Hall sensors at motor2 are might damaged. Ok.
In the meantime I ordered new motors - 6374 149kv , installed them and funny thing , same thing happen with the new setup. Motor 2 starts rotating  with a delay and slow rpm's.
Maybe the new motor got Hall sensor problems as well.
So I was curious and switched both new 6374 motors. 
 same thing happen.
I need some help here to understand  what's going on .
What ever motor is connected to the my unity port  motor2 side gets a different performance than motor1 side.
Funny thing is - I can see the different torque performance at my tires - even after 5 rides 20 k , motor1  has way less thread.
I started to play a little at Focbox_tool_1.0 , but couldn't figured out .
Ive got a message " bad fox hall detection results received" but this happens with three different motors. And one of the motors 6374 I received this message was placed on motor1 port at the unity and is was good.
Im asking for help.
```

---
## \#397 Posted by: Deodand Posted at: 2019-02-11T05:11:42.286Z Reads: 187

```
Can you make a little video showing the tests on the bench? As much information showing how its wired up plugged in etc.
```

---
## \#398 Posted by: drangboards Posted at: 2019-02-11T06:12:14.190Z Reads: 184

```
How to connect to Bluetooth? Turn on board? Hit a button on the remote? I can’t find this information anywhere.
```

---
## \#399 Posted by: pookybear Posted at: 2019-02-11T06:18:57.139Z Reads: 183

```
Turn board on
Open app
Hit scan
Choose unty
Connect
```

---
## \#400 Posted by: goldrabe Posted at: 2019-02-11T06:20:12.471Z Reads: 182

```
You need the Focbox UI on your phone, turn on your board then hit the Bluetooth connection tab.
With windows bluetooth is still not working.
```

---
## \#401 Posted by: goldrabe Posted at: 2019-02-11T06:22:34.205Z Reads: 180

```
Beat me to it. :heart:
```

---
## \#402 Posted by: goldrabe Posted at: 2019-02-11T06:32:16.760Z Reads: 186

```
Have you checked the Unity itself, any burn marks behind the sensor wire connector on the PCB?
![16|602x500](upload://b5KQQwhRYqiwQP4u1flSKfpppFU.jpeg)
```

---
## \#403 Posted by: drangboards Posted at: 2019-02-11T07:08:12.997Z Reads: 183

```
Gosh thanks guys. Maybe this cell phone doesn’t want to find it then. It might be too old.
```

---
## \#404 Posted by: CarlCollins Posted at: 2019-02-11T11:14:58.541Z Reads: 185

```
@drangboards
What is your Cell phone Android version?
I think the Unity app only support 4.4 or above
```

---
## \#405 Posted by: danwooller Posted at: 2019-02-11T11:47:13.485Z Reads: 188

```
My Nexus 6 didn't find the Unity, now have Pixel 2 that works. I think old phones even with a new OS have a problem.
```

---
## \#406 Posted by: CarlCollins Posted at: 2019-02-11T17:39:06.977Z Reads: 200

```
Confirm the bluetooth module version of the phone, it must be above 4
```

---
## \#407 Posted by: CarlCollins Posted at: 2019-02-11T17:39:51.378Z Reads: 199

```
@Deodand
Looks like you have to add legacy Bluetooth protocols support in the next firmware of Unity
```

---
## \#408 Posted by: danwooller Posted at: 2019-02-11T17:53:19.183Z Reads: 199

```
Nexus 6 has Bluetooth 4.1
```

---
## \#409 Posted by: rey8801 Posted at: 2019-02-11T19:34:02.507Z Reads: 203

```
Guys simple questions but I do not want to go through 400 posts. When I set the motor max/min battery max/min are they referring to one side only and they they will be time 2 for a dual set up, like in the Vesc tool configuration, or they are already the summ of two and then they will be divided 2? The motors looks single but the battery max/min seems already double. Thx
```

---
## \#410 Posted by: Jaydawg56 Posted at: 2019-02-11T19:40:02.236Z Reads: 206

```
Had the same question and found the answer buried in this thread.  Jeff and blasto have both answered with for batt max/min that is a single setting reserved for both motors.   Motor max/min values will be PER motor. If you stare at the slider on the unity UI, you can see the values for the battery  is singular and the motor is for each.
```

---
## \#411 Posted by: mackann Posted at: 2019-02-11T19:47:16.604Z Reads: 203

```
If you for example have a 12s4p 30Q that can do 80A you set 80A battery max, if your motors can hold for example 65A you set 65 motor max.
And if you would go 4wd with 2 unitys it would be 40A battery max and 65A motor max
```

---
## \#412 Posted by: rey8801 Posted at: 2019-02-11T19:54:49.083Z Reads: 200

```
@mackann @Jaydawg56 Thanks guys! I htought so. You made super clear! Thanks a lot. Some of you attached a hm-10 bluetooth module? is it enoght to pair the 5v, gnd, rx, tx in the right order between bluetooth and module, plus set UART 9600 to get the telemtry data with @Ackmaniac 's app?
```

---
## \#413 Posted by: Jaydawg56 Posted at: 2019-02-11T19:57:27.945Z Reads: 196

```
Yesterday I connected and recorded a few rides with the HM-10 plugged into the UART port (and enabled in the UNITY UI). MY HM-10 is from BKB and I assume yours is setup the same?  I recorded my sessions with XMATIC which should be no different than Ackmaniac
```

---
## \#414 Posted by: rey8801 Posted at: 2019-02-11T20:07:22.120Z Reads: 196

```
yeh all this module are the same. Thanks man!
```

---
## \#415 Posted by: pookybear Posted at: 2019-02-11T20:41:24.291Z Reads: 204

```
Maybe it is appropriate to post here instead of the noon thread.

Does anyone know why i get hard brakes when I stand the throttle? It happened twice now. 1st time I ate it. Lol. This time I was able to save my ass.

Here are the settings.

![Screenshot_20190211-123537|281x500](upload://9049ZjBFl4A17T7DIYmmpoqu2ed.jpeg) 

I'm using the mini remote. Am I hitting the cutoff or somehow my remote throttle gets whacked when I stab it.
```

---
## \#416 Posted by: Deodand Posted at: 2019-02-11T21:47:59.239Z Reads: 197

```
Remote calibration is more important to see than the motor settings for this issue. Which mini remote specifically?
```

---
## \#417 Posted by: pookybear Posted at: 2019-02-11T21:53:08.508Z Reads: 201

```
Found my issue. It was the motor. If I'm not gradual w the throttle, motor on the right of the video work as it should. But if I was to pull the trigger hard, it cogs. Thanks tho. 

https://youtu.be/Iaf5yY-4DVs
```

---
## \#418 Posted by: colinphotovideo Posted at: 2019-02-11T23:03:27.427Z Reads: 195

```
Mines the same as this and one motor won’t detect hall sensors either like yours
```

---
## \#419 Posted by: pookybear Posted at: 2019-02-11T23:05:15.892Z Reads: 194

```
Mine detects every single time. No errors whatsoever. Weird.
```

---
## \#420 Posted by: Deodand Posted at: 2019-02-11T23:05:36.983Z Reads: 195

```
Your hall sensors on the right motor aren't detected. Possible that they are damaged/ not connected correctly, note how the 3 circle dots aren't spaced evenly as on the left motor.
```

---
## \#421 Posted by: pookybear Posted at: 2019-02-11T23:06:10.442Z Reads: 197

```
I see. I tried sensorless settings w FOC. Same results.
```

---
## \#422 Posted by: Deodand Posted at: 2019-02-11T23:07:24.289Z Reads: 198

```
If you want to run sensor-less you should download the full tool and change the "open loop rpm" value in the sensor-less tab to something a bit higher.
```

---
## \#423 Posted by: pookybear Posted at: 2019-02-11T23:09:20.619Z Reads: 203

```
Nah. I'll just get a new motor unless Jared has an idea how to fix this. Plus, I like sensored.

Here's a pic. You're right it isn't detected.
![Screenshot_20190211-150730|281x500](upload://caVLuZTbLytTWnPERqK0KkSYW5k.jpeg)
```

---
## \#424 Posted by: Deodand Posted at: 2019-02-11T23:18:59.509Z Reads: 194

```
swap motors and halls to confirm its the motor real quick. if motor 2 is still faulty than something weird is happening.
```

---
## \#425 Posted by: pookybear Posted at: 2019-02-11T23:21:17.092Z Reads: 197

```
I will. Big kid stuff now. Heading to work. Will update you most likely tomorrow.
```

---
## \#426 Posted by: rey8801 Posted at: 2019-02-11T23:34:16.727Z Reads: 202

```
Do you also guys have the bug that if you change the battery cutoff then also the number of cells changes? Which is the latest firmware version? I have 23.41
```

---
## \#427 Posted by: Deodand Posted at: 2019-02-11T23:52:40.013Z Reads: 206

```
Feature not a bug haha. Coded that up.
```

---
## \#428 Posted by: rey8801 Posted at: 2019-02-11T23:56:06.858Z Reads: 204

```
Don't get me wrong the unity is really pretty. Super easy and smooth setup. These are details. You are doing really well.
Am I using the later firmware? 23.41?
```

---
## \#429 Posted by: Deodand Posted at: 2019-02-12T00:12:07.279Z Reads: 200

```
Think so but I'm uploading a release tonight or tomorrow morning early so I'd recommend jsut updating FW then.
```

---
## \#430 Posted by: venom121212 Posted at: 2019-02-12T00:45:30.564Z Reads: 196

```
Setting up my unity now but I'm very dumb when it comes to settings I should set. No discredit to you, the UI is wonderful. I just have no frame of reference as this is my first vesc based product. Anyone free to help?
```

---
## \#431 Posted by: Deodand Posted at: 2019-02-12T00:46:07.727Z Reads: 191

```
pm me or ask here my friend.
```

---
## \#432 Posted by: Sn4pz Posted at: 2019-02-12T01:26:06.560Z Reads: 187

```
Think we could post specs and you give us an idea of what to set? :thinking:
```

---
## \#433 Posted by: jippijuk Posted at: 2019-02-12T04:16:26.115Z Reads: 182

```
How to get a video imported here ? dropbox link?
```

---
## \#434 Posted by: jippijuk Posted at: 2019-02-12T04:34:36.967Z Reads: 181

```
there are mono burn marks, Ive checked .
still searching how to import the video .https://www.dropbox.com/s/9e3yz3vb5dubi97/IMG_1812.MOV?dl=0
```

---
## \#437 Posted by: Blasto Posted at: 2019-02-12T06:03:34.560Z Reads: 188

```
The behavior you are seeing is perfectly normal, one motor takes slight more current to turn than the other. Do too many factors, friction in chain, bearings, slightly different motor parameters etc. Once passed the 4-5A mark, both wheels spin freely.

You can also see that the wheel that stops first is the one that requires more power to turn. 

[quote="jippijuk, post:396, topic:77861"]
I can see the different torque performance at my tires - even after 5 rides 20 k , motor1 has way less thread.
[/quote]

Could this be you heel side?

To show video, you simply need to paste the youtube link it will embed itself in the post
```

---
## \#438 Posted by: pookybear Posted at: 2019-02-12T09:53:52.421Z Reads: 194

```
@Deodand @CarlCollins
 Is the USB plug on the unity supposed to soldered? Mine came off ![1549965172551662979762|375x500](upload://cRDemllHW0LtKk3kbcs0QNtxClf.jpeg)
```

---
## \#439 Posted by: venom121212 Posted at: 2019-02-12T13:34:39.549Z Reads: 191

```
What is the difference in baud rate settings for the unity in regards to the nano-x remote? 
My only knowledge of baud is information throughput yet both seem to work with the nano remote.
```

---
## \#440 Posted by: rey8801 Posted at: 2019-02-12T13:41:02.510Z Reads: 190

```
Usually baud rate refers to the UART port and therefore like metr module or HM10 bluetooth module. Nano-X use PPM signal which is another thing.
```

---
## \#441 Posted by: venom121212 Posted at: 2019-02-12T13:50:31.585Z Reads: 194

```
Got it, thank you. I thought it was odd under remote config but that makes more sense now.
```

---
## \#442 Posted by: rey8801 Posted at: 2019-02-12T13:59:52.002Z Reads: 190

```
yeh also in vesc tool is under remote configuration. There are several types of remote. Like firefly ask the uart port to get the telemetry data from the vesc. If you only have the nano-x you can disable the uart port.
```

---
## \#443 Posted by: jippijuk Posted at: 2019-02-13T04:15:05.861Z Reads: 189

```
Thanks for your help . But it can't be the motor with bearings and parameters. Because same thing happen with my 5035 motors. Also I switched both 6374 motors with motor#1 and motor#2 output from the unity, and same thing is happen with what ever motor I connect to unity outlet #2. I loosened up the chain also. It is not really good to see in the video but final RPM's from both wheels are really different ,visible with my eyes for sure.
So it seams to me its has not much to do with the motors or the chain .
And yes , its my heel side correct . Another test Ive done - trying to simulate a brake on both wheels with a glove - the available torque on motor #1 is incredible high. motor#2 is so weak that it doesn't take much effort to stop the spinning
```

---
## \#444 Posted by: Blasto Posted at: 2019-02-13T04:25:17.981Z Reads: 181

```
[quote="jippijuk, post:443, topic:77861"]
trying to simulate a brake on both wheels with a glove
[/quote]

prob not the best approach lol, be carefull

only other thing i can think of is maybe a flaky solder joint on the bullet connector of the phases Unity side... that's just a shot in the dark, maybe worth checking

can you show your motor detection results? a bad joint would show there
```

---
## \#445 Posted by: jippijuk Posted at: 2019-02-13T06:42:15.399Z Reads: 182

```
yeah, the glove test is not really a reliable scientific test, lol  but I looking for more clues.

actually I was thinking building two rollers with a adjustable measurable brake - to test under resistance ( not sure the right term , me ESL)

I checked optic and measured the bullet connectors , all good . All JST connections are very clean ,nothing bend
![IMG_1813|374x500](upload://8pZ8cVMgqmE1P8F8CE3cz81L6AQ.jpeg) 
any other tests I could do ? The FocboxUI is limited and basic, so I can not change settings for each motor . But the Focbox_tool allows this. what parameter should I work or play with for motor#2 ?
```

---
## \#446 Posted by: CarlCollins Posted at: 2019-02-13T07:49:31.920Z Reads: 178

```
@pookybear
Where are you located, let's solve this issue
```

---
## \#447 Posted by: murloc992 Posted at: 2019-02-13T08:00:52.498Z Reads: 183

```
https://www.electric-skateboard.builders/t/focbox-unity-official/64944/1944?u=murloc992

Just in case it's more logical to ask this here.
```

---
## \#448 Posted by: pookybear Posted at: 2019-02-13T08:17:25.878Z Reads: 189

```
I already shipped the unity back for replacement per your helpdesk team today.
```

---
## \#449 Posted by: CarlCollins Posted at: 2019-02-13T18:29:59.113Z Reads: 194

```
Great!

10chars
```

---
## \#450 Posted by: rey8801 Posted at: 2019-02-13T18:32:38.278Z Reads: 194

```
Guys is the push to start function working for you?
```

---
## \#451 Posted by: CarlCollins Posted at: 2019-02-13T18:33:24.095Z Reads: 192

```
It works for everyone but you have to push the board little harder (depending on the time settings)
```

---
## \#452 Posted by: rey8801 Posted at: 2019-02-13T18:35:05.101Z Reads: 190

```
Ah ok perfect. Thx! Although I don't have any time widow for the push to start. It's on or off only.
```

---
## \#453 Posted by: CarlCollins Posted at: 2019-02-13T18:35:57.715Z Reads: 189

```
you can see it in FOCBOX UI app if you have Unity
```

---
## \#454 Posted by: rey8801 Posted at: 2019-02-13T18:37:27.752Z Reads: 195

```
I see un the unity app but I don't have any special setting, only on / off


![ui|281x500](upload://srrLjAFEqjHAovvPUJ2rBAgW9aX.png)
```

---
## \#455 Posted by: CarlCollins Posted at: 2019-02-13T18:38:30.061Z Reads: 188

```
Ahh! My bad, you just have to push it harder :stuck_out_tongue:
```

---
## \#456 Posted by: rey8801 Posted at: 2019-02-13T18:43:43.123Z Reads: 191

```
Ok no problem. Fine for me :grin:
```

---
## \#457 Posted by: mackann Posted at: 2019-02-13T19:31:08.633Z Reads: 196

```
Is there any way to make the push to start a little easier to activate? I find it hard to start to, the speed needed is a little to mutch thene prefered
```

---
## \#458 Posted by: rey8801 Posted at: 2019-02-13T20:05:56.796Z Reads: 196

```
I guess is firmware based. Maybe in the next update they can make it more sensible.
```

---
## \#459 Posted by: billappleton Posted at: 2019-02-13T20:20:52.371Z Reads: 196

```
I thought push to start was hard to activate, but give it two pushes and then wait, let the remote go to zero, and then give it some power, the board will start right up. If you keep pushing and pushing and have the remote past zero it can be frustrating.
```

---
## \#460 Posted by: Deodand Posted at: 2019-02-13T22:06:22.350Z Reads: 198

```
The push to start is not firmware based. As the wheels roll the back emf in motors generates enough current to charge the bulk caps and turn on the mcu. If the top speed of your board is super high it will take a bit of speed to get there. For 10s it's about 7 percent of Max speed sustained for 1-2 seconds.
```

---
## \#461 Posted by: rey8801 Posted at: 2019-02-16T00:28:28.520Z Reads: 196

```
I see there is a new firmware update. What to aspect from it? Thx
```

---
## \#462 Posted by: jadatmag Posted at: 2019-02-16T01:01:57.842Z Reads: 193

```
The 'Beta Value for Motor Thermistor' has been changed from 3380 to 4100. This number should calibrate the temp sensor so that the readings the Unity gets are correct.

The throttle start temp has now been set to 100 celsius and the throttle stop has been set to 170 celsius.

With these two settings combined the Raptor 2.1/Unity should start throttling the motors wayyyyy later then before. In my case it would just stop responding to throttle after 5 minutes of aggressive riding. I hope this solves it all.


If you follow [the official guide](https://enertionboards.zendesk.com/hc/en-us/articles/360000774196-How-to-Update-the-Unity-for-a-Raptor-2-1-or-DIY-Board-VIA-Android-OR-Windows-PC) please be aware that the 'Battery Current Max Regen will be set to -30. And I'm not sure the 10s4p 30q pack can handle that. But I'll just go with the recommended settings.
```

---
## \#463 Posted by: rey8801 Posted at: 2019-02-16T01:08:05.065Z Reads: 185

```
Thanks for the info. I changed the min battery to what suits my battery pack :wink:
```

---
## \#464 Posted by: jadatmag Posted at: 2019-02-16T01:14:20.234Z Reads: 190

```
Hmmm, kinda weird.

When using the Windows Focbox_UI_1.1 and try to set the max allowed motor temp to a custom number the max is 135 C.

![image|505x500](upload://iLHppugfdlSxJuB2HmLatb96Dsb.png)
```

---
## \#465 Posted by: rey8801 Posted at: 2019-02-16T01:18:25.030Z Reads: 183

```
Same in the app
```

---
## \#466 Posted by: Deodand Posted at: 2019-02-16T01:19:56.780Z Reads: 182

```
It's not a bug. It just sets the min/Max to +- 35 of what is there.
```

---
## \#467 Posted by: rey8801 Posted at: 2019-02-16T01:21:58.160Z Reads: 182

```
You probably already mentioned but are you planning to include an app to collect and share telemetry data through the nrf module? Because for the moment except metr, that I don't have, I can not collect the unity performance.
```

---
## \#468 Posted by: jadatmag Posted at: 2019-02-16T02:15:41.291Z Reads: 184

```
So maybe a nice feature request would be to add two bars. One for start and one for stop.
```

---
## \#469 Posted by: 701Superjet Posted at: 2019-02-16T02:24:43.191Z Reads: 189

```
So what's the Latest FW version?
```

---
## \#470 Posted by: rey8801 Posted at: 2019-02-16T05:34:14.508Z Reads: 187

```
23.42 I believe
```

---
## \#471 Posted by: 701Superjet Posted at: 2019-02-16T05:53:57.375Z Reads: 186

```
Cool. Have it now. Man I was hoping for some more changes than that.
```

---
## \#472 Posted by: rey8801 Posted at: 2019-02-16T06:49:58.713Z Reads: 186

```
Experience told me that the more you change the more you need to fix. In software development better take small steps. I am sure updates will come
```

---
## \#473 Posted by: 701Superjet Posted at: 2019-02-16T14:47:37.095Z Reads: 184

```
I just need a minor update so my board doesn't take off an kill someone. Really scary. If I turn my board on by it's self right at 30 sec it goes to full throttle.
```

---
## \#474 Posted by: goldrabe Posted at: 2019-02-16T14:54:39.808Z Reads: 182

```
Your PPM settings are messed up! Try to load the default values in the Focbox Tool for your PPM settings and then calibrate the remote and reciever once more. If that doesn´t solve your issue then your reciever might be too close to some wires with high amp draw.
```

---
## \#475 Posted by: 701Superjet Posted at: 2019-02-16T15:03:32.998Z Reads: 188

```
Everything is fine if I turn my remote on. Rides like normal, and failsafe works good. I can turn my remote off and it won't take off on me. It's only if I turn the board on only. For example when my daughter pushed the button and I didn't know it had this problem. Lucky no one got hurt. But I do think your on to something with the remote settings. To get a full 100 to -100 during remote calibration my neautral point ends up being somewhere around 20%. If I trim my gt2b remote out to where it has a value of 0 for a midpoint I only get 80% throttle. Under normal circumstances this is working great ( although my OCD wants the midpoint at zero) I have a feeling when my board is turned on by it's self it defaults to this and messes with it.
```

---
## \#476 Posted by: Jaydawg56 Posted at: 2019-02-16T15:04:42.763Z Reads: 186

```
Are you sure? I just updated mine and it is reading 23.41  am I referencing the right window (unity UI, bottom of firmware tab)
```

---
## \#477 Posted by: 701Superjet Posted at: 2019-02-16T15:05:13.492Z Reads: 175

```
I'm on 23.42 now.
```

---
## \#478 Posted by: rey8801 Posted at: 2019-02-16T15:05:58.822Z Reads: 178

```
yep just did it last night. 23.42
```

---
## \#479 Posted by: Jaydawg56 Posted at: 2019-02-16T15:06:56.438Z Reads: 175

```
Got it. Might need to look at mine again haha
```

---
## \#480 Posted by: 701Superjet Posted at: 2019-02-16T15:07:46.761Z Reads: 174

```
I did mine with the app and had to delete the app and re download to get the update.
```

---
## \#481 Posted by: rey8801 Posted at: 2019-02-16T15:08:51.551Z Reads: 174

```
ah well before you have to update the app that for sure. Go in our market place and update it. @Jaydawg56
```

---
## \#482 Posted by: goldrabe Posted at: 2019-02-16T15:16:06.808Z Reads: 178

```
I haven´t used this particular remote but the usual calibration process is that you are not triming your remote but rather have the Focbox tool let do the calibration. After you click apply your your neutral point should be in the middle. Sorry I don´t have the tool in front of me so the apply button might be called something else. I hope it makes sense to you.
```

---
## \#483 Posted by: Jaydawg56 Posted at: 2019-02-16T15:21:41.901Z Reads: 174

```
Yea. Just uninstalled and reinstalled the UI. Says I need to update! Haha
```

---
## \#484 Posted by: 701Superjet Posted at: 2019-02-16T15:21:50.769Z Reads: 171

```
No worries. I appreciate the help. I can not touch the trim, do the calibration, and my netural point will be at 20%. I think this is because the gt2b remote has more throttle travel than brake travel.  I was hoping the update would let me manually set the netural point.
```

---
## \#485 Posted by: 701Superjet Posted at: 2019-02-16T15:22:32.619Z Reads: 168

```
Glad you got it! Ya mine said it was up to date but it wasn't. Cool!!
```

---
## \#486 Posted by: murloc992 Posted at: 2019-02-16T15:31:31.891Z Reads: 170

```
_Sweats profusely in GT2B..._ :disappointed_relieved:

(I have GT2B, but haven't tried to do calibration yet..)
```

---
## \#487 Posted by: jimmymagix Posted at: 2019-02-16T16:57:34.813Z Reads: 183

```
Guessing this means two of my hall sensor wires are either not present or shorted? Can anyone clear up which. I'm going to remove each wire in turn from the JST to see which the culprits are.

Alrwsdy switched the over in case it was a problem on the port on the box. It isn't. ![Screenshot_FOCBOX_UI_20190216-175243|250x500](upload://8peQjCDEkqqVcQ5cNJ8broZ7eEH.png)
```

---
## \#488 Posted by: Deodand Posted at: 2019-02-16T17:07:22.339Z Reads: 179

```
Should be Hall 3 I think
```

---
## \#489 Posted by: jimmymagix Posted at: 2019-02-16T19:55:01.253Z Reads: 189

```
I've tried since measuring the continuity on all wires and they all are apparently functional. I've tried with changing the phase wire combinations and get different hall outputs. 

Is this to be expected? If the hall wires leading from the motor show no continuity faults then the issue is internal to the motor, correct? 

Can you confirm that the image representing the Hall sensor in this case means that there's a short between two wires OR does it represent that the input from two wires is missing completely? 

![Screenshot_FOCBOX_UI_20190216-200459|250x500](upload://fDt6dLH6pOu2mq7qE07NNVko9Om.png) ![Screenshot_FOCBOX_UI_20190216-200723|250x500](upload://x8nsuHBosemIo15dZRx5RL9k5gQ.png)
```

---
## \#490 Posted by: Deodand Posted at: 2019-02-16T21:15:35.005Z Reads: 175

```
2 of your hall sensors are fine and 1 is broken.
```

---
## \#491 Posted by: Deodand Posted at: 2019-02-16T21:22:13.436Z Reads: 181

```
This is a problem with your remote not the unity. Can pretty much guarantee if you scope your receiver something wonky is going on with its PPM when you power up. We'd have a lot more people reporting this issue otherwise. The issue with the 20% thing is just a graphical issue in the app that I forgot to patch, oops :disappointed_relieved: You can download the full tool and configure your remote from there to confirm. 

 The GT2B is a pretty commonly used remote though so I'm a bit surprised to here this.  @murloc992 can you update us on if you get this same dangerous behavior?  

Not a lot to do on the unity because I can't just ignore PPM commands...  If its one spurious signal on power up it should time out.
```

---
## \#492 Posted by: 701Superjet Posted at: 2019-02-16T21:22:42.049Z Reads: 174

```
Tighten the pins in the hall sensor connector.
```

---
## \#493 Posted by: 701Superjet Posted at: 2019-02-16T21:24:06.440Z Reads: 176

```
I have had this with two different gt2b remotes on my board alone. My friend has a gt2b remote and his board does the exact same thing. Like I say if the remote is on it Acts like normal and everything is silky smooth. No glitches. It's only if the board is powered first and not the remote. At exactly 30 seconds it goes to full throttle.
```

---
## \#494 Posted by: Deodand Posted at: 2019-02-16T21:25:56.428Z Reads: 171

```
There's a trim pot on the remote side? And you are cranking it a lot so the neutral signal with the remote turned off is no longer in the +- 15% dead zone?

FYI the neutral point gets autoset correctly and just displays wrong. Just set the trim to 0.
```

---
## \#495 Posted by: 701Superjet Posted at: 2019-02-16T21:28:58.286Z Reads: 176

```
Yes. In order to get +-100% travel the netural point rest at about 19%. When the remote is on the board is happy with that netural point (even though I'd rather have it at zero) the fail safe on the remote also works good and the board doesn't take off.
```

---
## \#496 Posted by: Blasto Posted at: 2019-02-16T21:29:14.275Z Reads: 173

```
You guys setting the failsafe on the gt2b?
```

---
## \#497 Posted by: 701Superjet Posted at: 2019-02-16T21:29:30.525Z Reads: 171

```
Yes. Failsafe works perfect.
```

---
## \#498 Posted by: Deodand Posted at: 2019-02-16T21:33:17.080Z Reads: 174

```
Set trim to 0, re-run remote calibration and ignore the display percent. It should correctly read your remote setup. You can also just run remote calibration in the full tool ([download here](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_TOOL_1.1.exe)) and it will correctly display throttle.
```

---
## \#499 Posted by: 701Superjet Posted at: 2019-02-16T21:34:30.426Z Reads: 172

```
I'll do that and test it out. Good idea. Just don't like the idea of not getting full throttle. Already at 100A motor current and would take more if I could get it.
```

---
## \#500 Posted by: Deodand Posted at: 2019-02-16T21:36:48.318Z Reads: 169

```
The thing takes three values low max, center, and top max. These are read correctly in the app when you run calibration. The issue is just that the display read out is between max and min and doesn't account for center value. Just need to fix the plot in the app but it is computed correctly in FW. You will get the full +- 100 throttle if you just run calibration normally with trim set to 0.
```

---
## \#501 Posted by: 701Superjet Posted at: 2019-02-16T21:38:11.436Z Reads: 170

```
Awesome awesome! I'll try that and report back on here. Thank you!
```

---
## \#502 Posted by: Flashgod224 Posted at: 2019-02-16T21:49:24.581Z Reads: 175

```
Are there any developments to differentiating each unity when we are in close proximity of others? I know that as soon as winter ends here, we will have a lot of riders on unities here. Any feature that locks our unit to our device (or passcode) or that can help us name our unities would be nice. Thanks :)
```

---
## \#503 Posted by: Deodand Posted at: 2019-02-16T22:04:32.390Z Reads: 178

```
Yeah we will be taking a hard look at the BLE firmware very soon. We did enable over the air firmware updates for the module (requires special signing file for compiled fw to be flashed) so this feature will be coming but it's going to take some time as we want to build up an infrastructure to support BLE fw updates and customizations through the UI.
```

---
## \#504 Posted by: drone001 Posted at: 2019-02-16T22:12:56.686Z Reads: 177

```
is that a XT-60 connection, if so can it be changed to a XT-90?
```

---
## \#505 Posted by: 701Superjet Posted at: 2019-02-16T22:25:02.320Z Reads: 186

```
Ok I have ran calibration with it trimmed to zero. It's looking much better. I was too focused on the endpoints as well as the center. It has a zero midpoint now. However after after 30 seconds of the board on only it still goes to full throttle. I appreciate your help. I have pinned it down to the receiver now. It will not do it with it unplugged. The set failsafe on the receiver times out after 30seconds and defaults to something different. I set it up with slight brake for testing. If I connect remote and turn it off after 30sec the brake turns off and then defaults to 0 input. This is also the case if I turn only the board on. It applies the failsafe brake I set for 30sec and then for some reason after it goes to full throttle. I'll do some research and if need be make a new post for the GT2b. I'm least making serious progress on the problem now. Thank you so much for the help!!
```

---
## \#506 Posted by: billappleton Posted at: 2019-02-16T23:35:43.286Z Reads: 180

```
Please fix the remote midpoint issue
```

---
## \#507 Posted by: GreasyGearsWRX Posted at: 2019-02-16T23:58:34.223Z Reads: 185

```
So no iPhone support with the firmware update? 😔
```

---
## \#508 Posted by: murloc992 Posted at: 2019-02-17T17:59:05.790Z Reads: 204

```
@Deodand 

I just tested my GT2B and it literally goes to 100% throttle in a very short stroke of the remote.

I have calibrated the PPM in the app, it stays at 25% default, I assume it's the visual bug, but the acceleration curve happens in 2mm of the controller pull. :smiley:

The calibration data:

![image|575x207](upload://dcMwyZAz1fE59zCTAHW9Q3eO7X0.png) 

Throttle peaks at 40% of the input. So only 15% of the real input?

EDIT: I think it might be just no-load shenanigans. Sad that it's not really possible to test throttle curves without a load. :slight_smile:

https://www.youtube.com/watch?v=sk2ldPtm09Y
```

---
## \#509 Posted by: epss4 Posted at: 2019-02-17T23:53:52.795Z Reads: 201

```
Is the thermal throttle is better with the update??
```

---
## \#510 Posted by: jadatmag Posted at: 2019-02-18T22:56:47.887Z Reads: 209

```
Yes, light years better.

The throttling is very gradual and I couldn't get the board to become slow.

On this groupride I rode my board from full to empty without any major slowdowns. I'm back to the front of the pack.

https://youtu.be/6pTYCpL6yjI
```

---
## \#511 Posted by: rey8801 Posted at: 2019-02-19T08:18:11.601Z Reads: 197

```
@Deodand maybe it would be useful only for me, but would be possible to implement the voltage reading with a sensibility up to 0.1V? I don't have another volt meter connected and the rough 1V reading it's ok but not really precise. Should be an easy update. Maybe configurable through the Focbox tool so that who doesn't want it won't even notice the difference
```

---
## \#512 Posted by: erwintol1999 Posted at: 2019-02-19T09:19:31.168Z Reads: 194

```
I will place my ESC in the battery box in the middle of my board I use for my setup dual 6s 60c 8000mah lipo battery I run them in series dual 6374 170kv sensorless 2800w also I need to setup the focbox unity but I don’t know how an what settings I should use also I want to disable the reverse function should I go to an professional or can I do it by my self if I know the right settings sorry for my bad English.
```

---
## \#513 Posted by: aaront Posted at: 2019-02-20T05:28:25.351Z Reads: 190

```
I had my Unity arrive and it's on my board. 
I've noticed that the bluetooth connection is shotty at best. It randomly disconnects from the FOCBOX app on Android. Certainly not stable enough to (even though I wouldn't recommend) updating the firmware as it suggests.
But the frustrating part is that when I have it on HUD mode, or even just configuring the testings, I find myself having to go back to the setup screen and tapping "connect". I found it incredibly difficult to setup the Remote because when I went to calibrate, it would disconnect midway through loading the calibration function. 

This has been tested with both a Nexus 6P and a Samsung S9 Plus - anyone else having similar experiences with the bluetooth in the Unity?
```

---
## \#514 Posted by: Deodand Posted at: 2019-02-20T05:31:39.808Z Reads: 184

```
The bluetooth reliability is certainly something that needs some work especially for longer sessions when riding, but the level of connectivity issues you describe sounds mroe extreme than my experience. Do you have a metal or carbon fiber enclosure?
```

---
## \#515 Posted by: aaront Posted at: 2019-02-20T05:34:46.349Z Reads: 183

```
Nope - straight up ply. The issue still exists even when the cover is not on, too. As an example, when I tried yesterday to update the firmware, it got to to max 6.5%. Would not go past 6.49 and would fail anywhere from 1%
Again, I know updating firmware over Bluetooth isn't the best option, but I was in a jam. In the end, had to go out and buy another USB Type C cable (other one was left at the workshop)
```

---
## \#516 Posted by: 701Superjet Posted at: 2019-02-20T05:39:18.512Z Reads: 181

```
I've had issues with my Bluetooth as well. Google Pixel 3 XL. It works.. and I did update the firmware with it.. but I usually have to kill the app completely and re connect several times to get stuff done.
```

---
## \#517 Posted by: aaront Posted at: 2019-02-20T05:47:08.231Z Reads: 188

```
@701Superjet Glad it's not just me experiencing it, but mine does sound a little worse than yours, I guess.

I might give it another go tonight and might also record it to show here..

My other question I have is, when will the kick-to-start threshold be lowered? I've heard it requires significant speed before the board will turn on using that feature (like 9mph+) - I would rather not risk the opportunity of not having brakes down a hill in town. 
I reckon maybe 2kmh, or even a configurable limit would be much better. Leave it to riders choice.
```

---
## \#518 Posted by: Deodand Posted at: 2019-02-20T05:54:36.182Z Reads: 182

```
This is something that can't and therefore won't be changed. It is determined in hardware but mine works reliably. do you leave the house and immediately bomb a hill? My board (raptor 2.1) turns on with two good kick pushes. The key is just sustaining a small amount of speed.
```

---
## \#519 Posted by: aaront Posted at: 2019-02-20T06:02:15.191Z Reads: 183

```
Maybe I will give it another try. Unfortunately yes, the moment I leave my house, I am bombing a hill - no joke. I live on pretty much the steepest street in our CBD :joy: Not the place I want to test my faith every day. I like to think I have some healthy skepticism when I'm dealing with the speeds we end up reaching and crappy roads and drivers, so the more risk I can avoid reasonably, I will.

I will try the sustained speed and see if that helps the experience. The Raptor 2.1 is using the Unity, yeah?

My friends ESC turns on a little too rapidly I think - the moment the wheels move, it's on. A happy medium would be good.
```

---
## \#520 Posted by: 701Superjet Posted at: 2019-02-20T06:11:56.723Z Reads: 182

```
I have found my kick to start works off one kick. Maybe takes 5 feet / 1.5 meters to light the button and 15 feet/ 4.5 meters for it to actually boot up and connect. I hate the cheap esc's with a touchy kick to start. I'm always bumping a wheel turning them on by accident. Not a huge deal but really annoying to me.
```

---
## \#521 Posted by: goldrabe Posted at: 2019-02-20T06:21:52.691Z Reads: 180

```
I had the same experience as you, after I did a hard reset of my phone the Bluetooth connection is much better.
```

---
## \#522 Posted by: aaront Posted at: 2019-02-20T06:32:15.121Z Reads: 178

```
Hmm, okay I will give that a try - mainly because the phone I am using is **only** being used for this - but I don't have high hopes given it's been two, very different devices that have had the same result. Thanks for the suggestion though!
```

---
## \#523 Posted by: Deodand Posted at: 2019-02-20T07:16:01.797Z Reads: 181

```
You might want to check that the BLE module is secured well to the connector inside the case. The double sided foam tape typically holds it in there well but on some units where I remove the module and put it back I've gotten some times where it wasnt seated well. Bit of hot glue fixed it for me.
```

---
## \#524 Posted by: aaront Posted at: 2019-02-20T07:27:56.868Z Reads: 183

```
awesome, will try that too, thanks. That will be tomorrows job. Hopefully it's as simple as that, causing the issue.
```

---
## \#525 Posted by: mackann Posted at: 2019-02-20T08:40:46.894Z Reads: 188

```
Here is a test i did, after found out not to use the throttle before it works good:
https://www.youtube.com/watch?v=3kOAhaibqxg
```

---
## \#526 Posted by: Jomant Posted at: 2019-02-23T19:01:22.334Z Reads: 192

```
Hi everybody.

Got a Raptor 2.1 which connects to the Android app without any problems. If I run the desktop app and try to find it within it. Nothing!

I went into Win 10 Bluetooth settings and paired it this way. Now its connected shows up in Device Manager and shows as paired in the Win Settings. That App still don't see it. Try to open the App with elevated Admin Right....Still no go. 

Does anybody know  what can cause this, or what I forgot? 

Focbox_UI_1.1
```

---
## \#527 Posted by: Deodand Posted at: 2019-02-23T19:03:09.702Z Reads: 187

```
BLE on windows isn't supported at the moment.
```

---
## \#528 Posted by: Jomant Posted at: 2019-02-23T19:04:30.331Z Reads: 187

```
wow thx for the quick reply. ;)
```

---
## \#529 Posted by: jadatmag Posted at: 2019-02-24T01:30:43.306Z Reads: 203

```
Today on another group ride I took the effort to read temps again. And with some more aggressive riding the throttling was worse. One motor is getting hot way faster than the other one.

![ui|264x500](upload://q9KdzrgVA8IVhBRIfBi6oras6p7.png) 

Afther this I pushed it with some sprints to compare temps.

![IMG_0556|375x500](upload://cK95FR9R3g6Yn4lFT4ikjEpLJ9W.jpeg) 

We were never able to measure an outside temp of higher than 67. Even when they were 130 on the sensor a few sprints later.

![ui|264x500](upload://4NswJ5SfBOrLxmWmuF0UG4Y71HO.png) 


At this point it was slower than a meepo and Ownboard again, torque wise not speed. I was making short sprints to achieve these temps. (that's the worst case scenario)

I wonder how throttling will be when it's 25 celsius outside. If the one motor wouldn't heat up as fast as it does throttling might be less as the 'good' motor has so much to compensate it also throttles up faster.

If you don't take short sprints the board performs good. Not in a drag race, it would need to be pretty cool to be relevant/win, inclines might a problem too havn't tested

https://www.youtube.com/watch?v=D7EGT3nMQSY
```

---
## \#530 Posted by: goldrabe Posted at: 2019-02-24T02:58:12.271Z Reads: 185

```
Did you took readings on the truck and the silver part towards the kingpin of the motors too?
```

---
## \#531 Posted by: jadatmag Posted at: 2019-02-24T09:54:01.382Z Reads: 185

```
Yes, all lower than 67 at any point. The Measured point is actualiteit the hottest we could find. Inside, outside, truck.
```

---
## \#532 Posted by: epss4 Posted at: 2019-02-24T14:30:11.228Z Reads: 179

```
So its seem like its still bad reading of the temp from the hardware.... i dont think the motor is twice hot inside from the outise ... (67vs 130)
```

---
## \#533 Posted by: Pedrodemio Posted at: 2019-02-24T17:41:27.570Z Reads: 178

```
In my experience the core of the motors (windings) can be way hotter than the outside
```

---
## \#534 Posted by: epss4 Posted at: 2019-02-24T19:03:11.278Z Reads: 183

```
hi![26|690x90](upload://zvHAStKLohyWDRuokyJSXnD1e06.png) 
maybe someone can help me here , i have the 2.1 hub motor from enertion and the number from them are not the same ,is it normal to have this difference between them ?
Thanks
```

---
## \#535 Posted by: Mich21050 Posted at: 2019-02-24T19:04:43.485Z Reads: 183

```
Looks good to me. Just some minimal difference but @Deodand knows best... :slight_smile:
```

---
## \#536 Posted by: CarlCollins Posted at: 2019-02-24T20:16:40.358Z Reads: 182

```
@epss4

You have to roll motors as hard as you can, single time in forward direction to get the equal values.
Also, Make sure the bullet connector configuration is identical for both motors.

I fixed this issue on my Raptor recently, I think this applies to DIY setup as you are using Enertion Drive kit
```

---
## \#537 Posted by: epss4 Posted at: 2019-02-24T22:07:42.339Z Reads: 175

```
Ok i will try! Where can i get the 23.42 update with mac ?? 
Thanks ! :)
```

---
## \#538 Posted by: pookybear Posted at: 2019-02-24T22:13:41.435Z Reads: 180

```
Look at your hall sensor icon. To the right of the picture, it only has two. The left has 6. Bad hall sensor? This is just my assumption.

Mine exhibited only one sensor on my one motor. Weird thing is it passed motor detection and all but I had trouble stabbing the trigger. It cogged badly. 

My inquiring mind wants to know.

Maybe the expert enertion dudes could verify this.
```

---
## \#539 Posted by: Blasto Posted at: 2019-02-24T22:36:52.018Z Reads: 176

```
Click on the picture, everything seems fine
```

---
## \#540 Posted by: pookybear Posted at: 2019-02-24T22:42:23.215Z Reads: 175

```
I stand corrected. Thanks.
```

---
## \#541 Posted by: Blasto Posted at: 2019-02-24T22:44:06.917Z Reads: 178

```
[quote="pookybear, post:538, topic:77861"]
Mine exhibited only one sensor on my one motor. Weird thing is it passed motor detection and all but I had trouble stabbing the trigger. It cogged badly.
[/quote]

This was with a R2 drive? Were the sensors in their respecfull connector and not swapped?
```

---
## \#542 Posted by: pookybear Posted at: 2019-02-24T22:53:12.259Z Reads: 190

```
Nope. DIY stuff. Let me dig up my screenshot....

![Screenshot_20190211-150730|281x500](upload://caVLuZTbLytTWnPERqK0KkSYW5k.jpeg) .
```

---
## \#543 Posted by: rsalmon Posted at: 2019-03-03T16:48:31.987Z Reads: 189

```
Guys, I am experiencing some strange behavior with the unity under full throttle.

My setup is dual maytech 190kv 6355 sensorless motors.

I know it’s normal for sensorless motors to stutter at startup, but in my case even after a few pushes, it sutters once I punch the throttle.

So far it didn’t happen when I eased into the throttle, slowly accelerating.

In one instance it even ran for a bit and then it stuttered with a bit of speed already. Making it super dangerous since I was leaning forward and not expecting it at all.

Would you say this is normal? @Blasto @Deodand @CarlCollins?
```

---
## \#544 Posted by: Blasto Posted at: 2019-03-03T17:05:02.371Z Reads: 184

```
I don’t know what your motor currents are set at, but for 6055 should be in between 40 and 50A.
```

---
## \#545 Posted by: rsalmon Posted at: 2019-03-03T17:11:45.041Z Reads: 189

```
I left it at the default 60a since the motors are rated for 65a. It’s this model:
![image|384x384](upload://avwnVeSECTEVP8gHS1qr4GE0xjI.jpeg) https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTuxneY39NRJJ_mEzQ0PFun4_1TEwbB6VmKGSxVEEgDeybm3BfCBMNjL3KXiw
```

---
## \#546 Posted by: Blasto Posted at: 2019-03-03T17:13:49.985Z Reads: 186

```
Might be best if you posted your settings from the ui including your motor detection results

Inclding the type of battery you have
```

---
## \#547 Posted by: rsalmon Posted at: 2019-03-03T17:45:39.327Z Reads: 195

```
Here it is
![Screenshot_20190303-143849|281x500](upload://hdV2ecru2EB4gLPW2m0KIQgMEho.png) 
![Screenshot_20190303-143906|281x500](upload://4d4VymJJlo3bTOKip5MFzh02Tv.png) 

As for the battery, right now since I'm travelling I'm using two 5s turnirgy 5000mah 30c in series.
```

---
## \#548 Posted by: Blasto Posted at: 2019-03-03T20:02:34.160Z Reads: 192

```
Is it possible that it is your belts that are skipping?
```

---
## \#549 Posted by: rsalmon Posted at: 2019-03-03T21:35:12.032Z Reads: 196

```
It’s not belt skipping, first because of the noise and second because the motor kinda locks and throws off my balance.

I will try to record a video.
```

---
## \#550 Posted by: drone001 Posted at: 2019-03-04T22:34:04.999Z Reads: 197

```
Any pics on how to mount the Unity. It looks like the heat sink is on the bottom of the unit (I'm not speaking about the top heat sink). exactly where the mount screws are. Am I to mount the unit with the primary heat sink flush with the deck/enclosure, will I need to add an additional heat sink?
```

---
## \#551 Posted by: Deodand Posted at: 2019-03-04T22:42:08.583Z Reads: 195

```
In most e-skate applications the unity is fine without additional cooling. You can confirm this by checking temperatures in the app after a hard ride. Anything under 60-70C means you are well in the zone where no throttling due to motor driver heat is occurring.
```

---
## \#552 Posted by: drone001 Posted at: 2019-03-04T22:48:45.183Z Reads: 193

```
so is it ok to mount it with the primary heat sink flush or should there be some clearance?
```

---
## \#553 Posted by: Deodand Posted at: 2019-03-04T23:01:58.001Z Reads: 195

```
Yeah, I'm lazy and just mount it with some VHB tape to the wood, not exactly best practice but gets the job done and works fine until you need to remove the unit :smile:
```

---
## \#554 Posted by: Blasto Posted at: 2019-03-05T00:08:54.894Z Reads: 193

```
[quote="Deodand, post:553, topic:77861"]
Yeah, I’m lazy and just mount it with some VHB tape to the wood
[/quote]

Barbaric..
```

---
## \#555 Posted by: Blasto Posted at: 2019-03-05T00:14:04.698Z Reads: 197

```
![image|528x500](upload://uG0bnk1F3JSeJZC146XNwOq8adr.jpeg)
```

---
## \#556 Posted by: drone001 Posted at: 2019-03-05T01:34:28.821Z Reads: 190

```
are the mount holes on the heat sink?
```

---
## \#557 Posted by: Blasto Posted at: 2019-03-05T01:38:44.343Z Reads: 188

```
Yeah the 4 holes that are 44X15mm are M3 blind holes
```

---
## \#558 Posted by: drone001 Posted at: 2019-03-05T01:41:17.871Z Reads: 196

```
thx. I don't think i want my unit mounted flush like that.....I just got an idea this may be epic. thx again man.
```

---
## \#559 Posted by: venom121212 Posted at: 2019-03-05T01:50:47.672Z Reads: 199

```
If it's aluminum heat sink fins sticking out of your enclosure like a shark fin spoiler, that's my idea

Whoever flagged this is a supreme choch. I know who you are, I know you know who you are, and I know you know that I know who you are. Game on.
```

---
## \#560 Posted by: pookybear Posted at: 2019-03-05T01:52:03.696Z Reads: 196

```
@Deodand @CarlCollins

Will the next update include an option for the users to change the baud rate on the other UART port/s?
```

---
## \#562 Posted by: drone001 Posted at: 2019-03-05T01:55:04.569Z Reads: 195

```
ok ok ok...you got me!!
```

---
## \#563 Posted by: drone001 Posted at: 2019-03-06T01:28:15.209Z Reads: 188

```
What is the UART port and what is it used for. I've searched high and low and I can not find a clean cut description as to what it is.
```

---
## \#564 Posted by: pookybear Posted at: 2019-03-06T02:02:11.911Z Reads: 192

```
https://en.m.wikipedia.org/wiki/Universal_asynchronous_receiver-transmitter

Simpler terms:
 - means of communication between Vesc and a device.
 - usages: telemetry, changing settings wirelessly.
```

---
## \#565 Posted by: drone001 Posted at: 2019-03-06T03:26:14.939Z Reads: 183

```
beautiful...thx a million man.
```

---
## \#566 Posted by: jippijuk Posted at: 2019-03-06T09:37:50.800Z Reads: 187

```
Replacement main switch for the unity ? There was no confirmed info about the specs at Eneretion support live chat I could get . I damaged my switch and need a replacement .
Would this work? -https://www.amazon.ca/gp/product/B07HFXNRQJ/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1

There is a laser imprint at my old switch -3V . I would appreciate details . Thank you .
```

---
## \#567 Posted by: ninTHIENdo Posted at: 2019-03-06T12:44:36.408Z Reads: 197

```
![image|281x499](upload://n8XzAFa8fi6HFK1UaCKCpX7iNgx.jpeg) 

Looks like we missed February.....
```

---
## \#568 Posted by: rey8801 Posted at: 2019-03-06T13:59:45.097Z Reads: 201

```
Guys, just for information. Does someone know if they start shipping the early March batch?
```

---
## \#569 Posted by: mackann Posted at: 2019-03-06T18:16:48.617Z Reads: 235

```
If anyone is going 4wd here is a demonstration of using 5v on canbus connector for on and soon off with only one button:
https://youtu.be/vipPn5gwtSk
```

---
## \#570 Posted by: rey8801 Posted at: 2019-03-06T18:19:47.993Z Reads: 234

```
Did you find a pin or something to connect a voltmeter to the unity that it get turned off when the unity is off?
```

---
## \#571 Posted by: mackann Posted at: 2019-03-06T18:23:16.148Z Reads: 238

```
Im not sure I understand your question, there is a connector for batterymeter on Unity, 2pin on the motor cable side:
![Screenshot_20190306_192211|350x499](upload://xI2eHupVLSi3GEEAN169qOUTRSp.jpeg)

It gives the voltage of the battery and is powered of when the Unity is of
```

---
## \#572 Posted by: rey8801 Posted at: 2019-03-06T18:26:19.062Z Reads: 223

```
Ah ok my bad
Appparetnly didn't look close enough to it. Thanks!
```

---
## \#573 Posted by: Blasto Posted at: 2019-03-06T20:29:28.670Z Reads: 216

```
Dope, @Deodand we need some CAN shutdown my man
```

---
## \#574 Posted by: Deodand Posted at: 2019-03-06T21:38:36.962Z Reads: 215

```
Yea, I'll get on it.
```

---
## \#575 Posted by: Silverline Posted at: 2019-03-07T19:18:05.928Z Reads: 218

```
Yeah... I was also told shipping in February...im still waiting since November.. i guess its a enertion thing....
```

---
## \#576 Posted by: GreasyGearsWRX Posted at: 2019-03-08T00:37:40.803Z Reads: 221

```
Have you guys at enertion or any unity owner been having issues with the unity’s momentary switch causing power dropouts or cutouts? I’ve had intermittent cutouts for a few weeks and only brief almost instantaneous cutouts. I thought it was remote dropouts (Hoyt) until today when I powered the board and the remote on and could not spin the wheels for almost 30 seconds until I tossed the board onto its wheels when I’m assuming the impact with the ground caused a reconnection somewhere allowing me power. Also to further the momentary switch’s possibility of being the cause is the fact that it doesn’t always glow when it is on. Sometimes even tapping the enclosure with my finger vibrates the switch enough for the LED to flicker on or off. Any help would be appreciated!
```

---
## \#577 Posted by: epss4 Posted at: 2019-03-08T00:39:43.005Z Reads: 213

```
I think you have loose connection in your enclosure ....if i was you i would open the enclosure and chek ... power cutoff can be fatal mate...
```

---
## \#578 Posted by: GreasyGearsWRX Posted at: 2019-03-08T00:50:10.277Z Reads: 208

```
Already checked all the electrical connections. Whatever is left is isolated into the unity and the switch! I’m about to open it up again and see what’s going on!
```

---
## \#579 Posted by: epss4 Posted at: 2019-03-08T00:55:19.821Z Reads: 207

```
I did get few bad switch in the past , not with the unity but your problem can be in the switch it self  for sure man !im pretty sure @CarlCollins can help you with this :)
```

---
## \#580 Posted by: GreasyGearsWRX Posted at: 2019-03-08T01:01:17.713Z Reads: 206

```
Okay great thanks dude!
```

---
## \#581 Posted by: billappleton Posted at: 2019-03-08T02:42:53.066Z Reads: 210

```
Hi all, I am setting up the new Maytech R2 style remote with Unity. I am calibrating everything the way I did with the Hoyt Puck. In this case however, the Maytech does not run the motors until exactly 50% on the trigger. If I lift my finger off the trigger, and the motors are off, then the wheels are braking hard, they cannot be turned by hand. What is going on?
```

---
## \#582 Posted by: CarlCollins Posted at: 2019-03-08T04:41:43.509Z Reads: 213

```
Can you confirm what push to start values you have set on Unity and power button press seconds?
```

---
## \#583 Posted by: billappleton Posted at: 2019-03-08T05:00:17.734Z Reads: 206

```
Kick push to start is on

Inactive until shutdown is 10 min

Power press for shutdown is 1.5 sec
```

---
## \#584 Posted by: GreasyGearsWRX Posted at: 2019-03-08T08:34:23.729Z Reads: 215

```
I will look tomorrow sometime. Unless the iOS app is out and can view this I’m going to require removing my complex enclosure bolts and manually connecting to the unity 😕 Is the iOS app out by chance yet? I may have missed it. 

I am very confident those values are set at or within 10% of defaults. I feel this way because the board operated beautifully for a couple months but it’s reliability has been slowly degrading over time likely as the power switch has seen tons for vibrations and some water.
```

---
## \#585 Posted by: mackann Posted at: 2019-03-08T09:28:11.482Z Reads: 228

```
Anyone knows what could cause overcurrent cutout?
I have alot of boards and they all work fine with unity, I checked every connection for bad connection but all is fine. I tried change the battery and bms on the board but still same error when going full throttle. I have the exact same setup on another board and no problem. The setup is 12s4p with dual 6374 motors. 80A battery and 68A motor. 

The only thing I have not changed is the Unity and motors, could it be something wrong with it? It's working fine if I don't go full throttle. 

![Screenshot_20190308_102701|346x500](upload://xNfxMKdxcg2PwNnV0gFXIiKkyds.jpeg) ![Screenshot_20190308_102634|356x500](upload://yOnIAz2mqJJ7m5WXrggtvdIphwz.jpeg)
```

---
## \#586 Posted by: CarlCollins Posted at: 2019-03-08T20:39:38.823Z Reads: 207

```
Looks like your motors and remote need calibration
Hoyt remote has really hard to calibrate with Unity, 
Make sure you are using FOCBOX Tool (not UI) for extensive calibrations

I would also like to assist you remotely if the issue still persists.
```

---
## \#587 Posted by: CarlCollins Posted at: 2019-03-08T20:40:54.203Z Reads: 208

```
There are likely chances that water impacted the receiver, unplug, clean and re-plug the receiver
also iOS app isn't out yet, we will notify once we have it out
```

---
## \#588 Posted by: CarlCollins Posted at: 2019-03-08T20:42:24.834Z Reads: 215

```
Looks like values are little high 
try reducing them and also make sure you calibrate the remote pulse as well

I think then this issue will be fixed

This happens also when one or more motors are faulty
```

---
## \#589 Posted by: billappleton Posted at: 2019-03-09T00:09:11.988Z Reads: 221

```
Hi Carl, Figured this out. With the new Maytech R2 style MTSKR1805WF the guided calibration will work. BUT you have to calibrate the trigger and then the brake. In other words, squeeze the trigger, and the brake. This new remote works greate with Unity after that!
```

---
## \#590 Posted by: GreasyGearsWRX Posted at: 2019-03-09T00:33:10.723Z Reads: 219

```
No water has penetrated the enclosure but I do plan to reseat all my connections while I have it opened up! Keep you posted. What’s the lead time on a momentary switch for the unity from you guys?
```

---
## \#591 Posted by: CarlCollins Posted at: 2019-03-09T14:53:26.607Z Reads: 208

```
Glad to hear you figured it out
```

---
## \#592 Posted by: CarlCollins Posted at: 2019-03-09T14:54:12.630Z Reads: 206

```
I am not sure if you already contacted support for the switch but you have to do it if your switch is faulty
```

---
## \#593 Posted by: drangboards Posted at: 2019-03-10T01:26:39.190Z Reads: 212

```
This might be the correct thread for this question.  

Is this ok?

![image|443x499](upload://8ngLgAgpSFtlXPzSpkJPjAlvjEG.png)
```

---
## \#594 Posted by: venom121212 Posted at: 2019-03-10T01:57:48.863Z Reads: 199

```
Mine was way way off. That should be fine. You can also manually match them using the focbox tool
```

---
## \#595 Posted by: drangboards Posted at: 2019-03-10T02:03:35.877Z Reads: 199

```
Well one of the two motors is having some sort of issue spooling up...  Would manually matching them solve that ride ability issue? 

What do these numbers mean anyways?
```

---
## \#596 Posted by: Deodand Posted at: 2019-03-10T02:05:56.533Z Reads: 195

```
it's akin to the motor kv kind of, essentially its volts/ (rad/s) or Newton-meters (torque) / amps (motor current). 0.5 is probably the incorrect value.
```

---
## \#597 Posted by: drangboards Posted at: 2019-03-10T02:10:48.928Z Reads: 200

```
Yeah, the .5 motor is the one not having issues spooling up. 
That would stand to reason.  Assuming the left right is constant in the HUD and the motor configs...  In real life, they are on the opposite sides.
```

---
## \#598 Posted by: drangboards Posted at: 2019-03-10T02:14:21.948Z Reads: 197

```
It also happens to be that the motor in question makes more noise when free spinning it....  I am wondering what could cause the KV rating to be high or watever, and then also cause the noise and the drive ability...
```

---
## \#599 Posted by: Deodand Posted at: 2019-03-10T02:20:55.884Z Reads: 203

```
the hand spin detection is the part of detection routine that measures that number, make sure you run the calibration and give it a nice firm spin.
```

---
## \#600 Posted by: drangboards Posted at: 2019-03-10T02:21:29.579Z Reads: 203

```
I have mastered doing that, and the results I am getting are very consistent.
```

---
## \#601 Posted by: venom121212 Posted at: 2019-03-10T02:46:55.088Z Reads: 200

```
Match the Flux linkage numbers like I mentioned and try again. Should run like butter
```

---
## \#602 Posted by: drangboards Posted at: 2019-03-10T02:47:24.246Z Reads: 200

```
Ok, I do'nt know how, gonna go back in right now, and see if I can figure it out.
```

---
## \#603 Posted by: venom121212 Posted at: 2019-03-10T02:56:19.117Z Reads: 201

```
Download the focbox tool, not the UI of you are having this issue. It allows you to manually set the values when motor detection doesn't work exactly right
```

---
## \#604 Posted by: drangboards Posted at: 2019-03-10T02:56:43.865Z Reads: 197

```
Already have it yo.
```

---
## \#605 Posted by: drangboards Posted at: 2019-03-10T02:57:36.426Z Reads: 207

```
![image|558x500](upload://gkq9eN3KvTcn2eUgSqa4ov3FT4H.png)

So for some reason I am getting good results in this tool, but not in the other tool...

Gonna go see if this works better before getting into the other app. 



On a side note can anyone speak to the use of the app for iphones, Xmatic?  $3 bucks, and I can maybe do this shit without pulling the enclosure off...

She's riding well again.  Strange results.
```

---
## \#606 Posted by: rsalmon Posted at: 2019-03-11T02:40:43.612Z Reads: 201

```
I am having the same exact issue during full throttle. If eventually you find a fix, please let us know.
```

---
## \#607 Posted by: Deodand Posted at: 2019-03-11T03:31:18.170Z Reads: 209

```
I think a couple other people have encountered the same issue. I haven't pinpointed the exact cause but it seems to be occuring at that low speed transition from hall sensors to sensorless operation with large motors,  can you try using the full tool and changing the following parameter: 

![image|690x387](upload://jtJkPegknSZVNWBydZmG4fIyvPq.png) 

to something like 4500 instead of 3500 and let me know if that addresses the issue? 

Sorry to those wrestling with the bug, I'm working on a FW release now I'll do my best to pin down the cause and fix it.
```

---
## \#608 Posted by: Deodand Posted at: 2019-03-11T03:33:51.290Z Reads: 197

```
Thanks for the info, something funny must be going on with the app I'll investigate... is this on the pc?
```

---
## \#609 Posted by: rsalmon Posted at: 2019-03-11T03:53:30.997Z Reads: 206

```
In my case I am running sensorless motors already. Do you think that parameter would have any effect?
```

---
## \#610 Posted by: Deodand Posted at: 2019-03-11T04:11:52.724Z Reads: 217

```
You might try playing with this parameter instead for sensorless: 

![image|690x392](upload://x07NnbqU3RxLjNC0kxIoyVXi7q0.png) 

Just to confirm is this issue happening at higher speeds? If so it's possible it is something completely different, have you tried typing "faults" in the terminal after you ride and experience a dropout without powering off? 

[quote="rsalmon, post:543, topic:77861"]
In one instance it even ran for a bit and then it stuttered with a bit of speed already. Making it super dangerous since I was leaning forward and not expecting it at all.
[/quote]

What qualifies as a bit of speed? 

Also don't forget to check some things like good wiring with motor conenctors, do you also feel certain it isn't related to dropouts of the remote? If the dropouts occur specifically only during max throttle it would seem to not be remote related but figured I would double check.
```

---
## \#611 Posted by: rsalmon Posted at: 2019-03-11T04:21:14.246Z Reads: 216

```
[quote="Deodand, post:610, topic:77861"]
Just to confirm is this issue happening at higher speeds?
[/quote]

Maybe over 20km/h already? Unfortunately, I don't have telemetry to back up my claims.

[quote="Deodand, post:610, topic:77861"]
“faults”
[/quote]

It happens at low speeds without causing a fault. If I push one or two times and then try to full throttle, it stutters. But if I push and then gradually accelerate, it goes fine.

However, I tried to reproduce the problem at speeds higher than just a few pushes, and I got the same fault as @mackann:

![image|281x500](upload://puoB4IcMVwFWw5t8UXaxCIBQOD9.png) 

[quote="Deodand, post:610, topic:77861"]
What qualifies as a bit of speed?
[/quote]

Between 20-30km/h

[quote="Deodand, post:610, topic:77861"]
Also don’t forget to check some things like good wiring with motor conenctors,
[/quote]

It seems to be all good, but I will certainly double check again.

[quote="Deodand, post:610, topic:77861"]
do you also feel certain it isn’t related to dropouts of the remote? If the dropouts occur specifically only during max throttle
[/quote]

I've ridden for maybe 100km already, going easy on the throttle and didn't experience a dropout. It seems to be exclusively related to full throttle.
```

---
## \#612 Posted by: DerelictRobot Posted at: 2019-03-11T04:29:47.178Z Reads: 190

```
[quote="CarlCollins, post:586, topic:77861"]
remote need calibration Hoyt remote has really hard to calibrate with Unity
[/quote]

Could you expand on this?
```

---
## \#613 Posted by: Deodand Posted at: 2019-03-11T05:21:33.801Z Reads: 193

```
Great this info is really helpful, thanks. I think the low speed dropouts may be related to the parameter I pointed out to you. The overcurrent issue is interesting and warrants investigation. It's always motor 1 throwing crazy high currents (132 amps)?
```

---
## \#614 Posted by: drangboards Posted at: 2019-03-11T06:07:06.488Z Reads: 191

```
Deodand it is on pc yes windows 7

Do you also recommend I raise the open loop erpm?
```

---
## \#615 Posted by: Deodand Posted at: 2019-03-11T06:17:00.617Z Reads: 190

```
No the raptor 2 hubs should be good as is.
```

---
## \#616 Posted by: mackann Posted at: 2019-03-11T09:00:30.956Z Reads: 198

```
Thanks will try that, it have happend one time on high speed to, going around 40km/h on a board that can do 65km/h and using full throttle and it got a over current cut out to. So havnt dare to try more on that board in high speed, but it happens almost every time on stand still /very low speed when going full throttle. But the strange is that its only on this board and no other board I have with Unity so I start to think it's just this Unity. I don't know if we dare to try more on this Unity, I already broken my bone in shoulder and my friend crashed in high speed with it.. I got a suggestion it could be a broken bulk capacitors, have not checked that yet, do you think it could be that?
```

---
## \#617 Posted by: rsalmon Posted at: 2019-03-11T14:21:15.863Z Reads: 198

```
[quote="Deodand, post:613, topic:77861"]
The overcurrent issue is interesting and warrants investigation. It’s always motor 1 throwing crazy high currents (132 amps)?
[/quote]

I can't say for sure yet. I need to reproduce more times but I am a bit afraid of it since it almost always result in an accident.
```

---
## \#618 Posted by: Blasto Posted at: 2019-03-11T15:16:35.345Z Reads: 197

```
Yeah wait until you get back in town, we will look at this together
```

---
## \#619 Posted by: EXEET Posted at: 2019-03-12T10:42:18.081Z Reads: 193

```
Time to get finished with the winterproject. Everything but BMS is ordered. Any idea on witch to buy? The specs on the board is: Focbox, 12S12P VTC6, Torqueboards 6380 80a. I guess the best solution is to just use the BMS on charging? How do i connect this correct? Or will i destroy the batteries du to no voltage cut? Cheers
```

---
## \#620 Posted by: Sn4pz Posted at: 2019-03-12T11:23:27.084Z Reads: 198

```
You should make a separate thread, your post doesn't really belong here
```

---
## \#621 Posted by: Ckarg Posted at: 2019-03-12T16:51:22.744Z Reads: 208

```
I have posted this question over in the DieBieMS and waiting to see if @JTAG has any comments but though I would see if anyone here could shed some light on this. 

I was wondering how should I wire my CAN on the unity too, two(2) DieBieMS’? I am also wanting to be able you utilize the push-to-start and power switch as a manual option.

My thoughts are to parallel the Can from the Unity to the two DieBieMS’ (canH - canH, canL - canL, 5v - 5v, GND - GND, and the 5v to can enable). Or would it just be better to wire it in series, Unity to first DieBieMS, then Daisy chained to the second DieBieMS via the second CAN port to the second DieBieMS?

That leads to my next question of where to connect the power switch? Either the one that came with the unity on the Unity, or the one that came with the DieBieMS to the DieBieMS’. If I connect it to the DieBieMS’ I have to disable push-to-start on the Unity but might be able to overcome that by using the push-to-start from the DieBieMS’. Otherwise, I connect it to the Unity but have a hard time understanding how I am able to power it up if the DieBieMS’ aren’t on and thus no system power.

Sorry if this is off topic but it kind of relates to setting up the unity.![20190309_121931|243x500](upload://6NLq3eAKBo2YODiJ79tVDD0lkaL.jpeg)
```

---
## \#622 Posted by: Bas1 Posted at: 2019-03-16T22:42:16.944Z Reads: 197

```
Hello can you help me to setup up the focbox unity I have an dual 6s lipo 60c 8000mah 480a total I run them in series I have s dual 6374 149kv sensorless 70a motor max total and 12awg xt60 series cable and extension cable what is the ideal setting for my setup also i want to disable the reverse function
I'm new to esk8 so please help me!!
```

---
## \#623 Posted by: murloc992 Posted at: 2019-03-17T17:30:28.583Z Reads: 193

```
Are the mounting holes in Unity stopped by the plate? Also how deep are they?
```

---
## \#624 Posted by: ZachTetra Posted at: 2019-03-17T17:57:40.687Z Reads: 199

```
I’m running KooWheel hubs with a 10s2p battery and a Unity (it’s only temporary, I’m not wasting the Unity).  At speed it will start braking when I push the throttle up, it does it kinda randomly starting at 10mph and I can’t get past 17mph.  It running sensor less FOC because the leads for the sensors are gone

Suggestions?
```

---
## \#625 Posted by: Deodand Posted at: 2019-03-17T17:59:30.640Z Reads: 200

```
@murloc992 I believe teh holes are not through hole, off the top of my head think 3-4mm 

@ZachTetra  Redo your remote calibration possibly, what remote are you using? If it is nano-x make sure to run calibration in r-spec mode not slow mode.
```

---
## \#626 Posted by: ZachTetra Posted at: 2019-03-17T18:08:50.303Z Reads: 201

```
It’s just a mini remote I got used, ran the detection and range stuff and it didn’t care for it.  It also just shakes if I touch the throttle when it is starting from stopped and it whines when I bench test it
```

---
## \#627 Posted by: Deodand Posted at: 2019-03-17T19:03:59.341Z Reads: 201

```
You should contact support to get some help walking through setup @CarlCollins
```

---
## \#628 Posted by: CarlCollins Posted at: 2019-03-17T19:38:50.654Z Reads: 201

```
Replied to your PM
```

---
## \#629 Posted by: Shaun Posted at: 2019-03-17T19:52:57.369Z Reads: 212

```
Hi guys, my Unity is on it’s way to me (quicker than I expected as I thought I missed the 2nd batch) and I want to get the battery side of my build sorted. I need a BMS but I’m confused what the Unity offers in terms of battery protection/monitoring and I don’t want to over spec the BMS and double up on functionality if I don’t need to.
```

---
## \#630 Posted by: Jc06505n Posted at: 2019-03-17T19:57:58.014Z Reads: 207

```
Any BMS will do , If anything you would want double redundancy in case stuff go badOn one end. 

Because the unity provides batter cutoff , this allows many people to go the charge only route. If you don’t want to have to deal with balancing your battery after a while, get a discharge BMS.
```

---
## \#631 Posted by: Shaun Posted at: 2019-03-17T19:59:22.895Z Reads: 202

```
Thanks mate. Any recommendations? I’m going 10s.
```

---
## \#632 Posted by: Shaun Posted at: 2019-03-17T21:29:30.821Z Reads: 203

```
What remotes work with the Unity? I just need something cheap to get me up and riding for the minute.
```

---
## \#633 Posted by: Sn4pz Posted at: 2019-03-17T21:31:38.537Z Reads: 201

```
Anything that isn't a remote with fancy Bluetooth with work 'out of the box'(with minor adjustments, like 0ing ppm at neutral throttle)

G2b

Mini

Nano x

I think those are the main (good) ones
```

---
## \#634 Posted by: Shaun Posted at: 2019-03-17T21:59:26.903Z Reads: 200

```
Thank you!
```

---
## \#635 Posted by: CarlCollins Posted at: 2019-03-18T06:06:56.968Z Reads: 200

```
Unity comes with the battery protection system already so all you need to do is get any charge only BMS.
Any 2.4 Ghz remote will work with it.
```

---
## \#636 Posted by: Shaun Posted at: 2019-03-19T21:26:34.120Z Reads: 193

```
Do I need an antispark or switch between the battery and the Unity?
```

---
## \#637 Posted by: Mich21050 Posted at: 2019-03-19T21:27:15.208Z Reads: 191

```
NO. That has been answered one bazillion times already... :slight_smile:
```

---
## \#638 Posted by: Sn4pz Posted at: 2019-03-19T21:28:33.703Z Reads: 198

```
https://media1.tenor.com/images/5a2524041fbb9f67c577ff4e1018745e/tenor.gif?itemid=9196308

oh no you got Michael tight :laughing:

srsly tho lol, control F and discourse even works with you to search the entire thread, and not just  whats on your screen.
```

---
## \#639 Posted by: Mich21050 Posted at: 2019-03-19T21:29:35.699Z Reads: 193

```
Yeah... and a fucking awfull day... :slight_smile: :joy:
(Sorry @Shaun)
```

---
## \#640 Posted by: murloc992 Posted at: 2019-03-19T21:31:50.195Z Reads: 193

```
A loopkey never hurts if you want to fully disconnect your battery, just saying. :slight_smile:
```

---
## \#641 Posted by: Shaun Posted at: 2019-03-19T21:34:29.068Z Reads: 191

```
Apologies. So basically you can directly connect a battery to the Unity and it will do everything (accurately manage current draw from the battery if set correctly, Regen, switch the power on and off without any draw when it’s off, act as the anti spark)? 

Enertion need to include these basic questions in their FAQ section on their website for noobs like me.
```

---
## \#642 Posted by: murloc992 Posted at: 2019-03-19T21:35:25.956Z Reads: 192

```
Not sure about idle current draw, maybe it is zero, but some antisparks were known to draw some current even after being "off", so I'd add a loop key just in case when you go away for a longer time without riding.
```

---
## \#643 Posted by: Shaun Posted at: 2019-03-19T21:38:19.785Z Reads: 197

```
No offence taken! 😂
```

---
## \#644 Posted by: Sn4pz Posted at: 2019-03-19T21:45:22.413Z Reads: 203

```
I believe the Unity drains, but not alot. its almost negligible: 

https://www.electric-skateboard.builders/t/fatboy-antispark-0-5w-draw/85036/9?u=sn4pz

https://www.electric-skateboard.builders/t/fatboy-antispark-0-5w-draw/85036/15?u=sn4pz

@Shaun
```

---
## \#645 Posted by: Shaun Posted at: 2019-03-19T21:48:09.076Z Reads: 198

```
Thanks guys!
```

---
## \#646 Posted by: Shaun Posted at: 2019-03-19T21:48:27.341Z Reads: 203

```
Thank you!
```

---
## \#647 Posted by: Deodand Posted at: 2019-03-19T22:52:00.047Z Reads: 209

```
You can leave your unity plugged in on a discharged battery for several months without issue. Any charge in the battery extends that to the years time frame where it isn't worth thinking about. 

It handles all anti-sparks functionality onboard.

Quick math: typical 10 Ah battery (4 parallel cells) discharged to 3.1V (unity cutoff) has 10 percent capacity left. 1Ah/0.00001 amps = 11.4 years
```

---
## \#648 Posted by: murloc992 Posted at: 2019-03-20T05:48:26.075Z Reads: 211

```
No need for a

![image|678x234](upload://1Vzshxv6edpVPcxTSwanAAqdfYP.jpeg) 

then. Good to know, cleaner setup. :smiley:
```

---
## \#649 Posted by: pookybear Posted at: 2019-03-25T20:35:25.899Z Reads: 216

```
Has anybody here having trouble changing motor Max and min using the app? 

Workflow:

* Hit scan
* Choose unity
* Connect
* Click config tab
* Click read current config
* Change parameters
* Click apply updated config.

Nothing. Any ideas?
```

---
## \#650 Posted by: mackann Posted at: 2019-03-25T21:15:25.880Z Reads: 213

```
Probably bad Bluetooth connection(will be improved next update I think) , try using USB cable
```

---
## \#651 Posted by: pookybear Posted at: 2019-03-25T21:33:39.994Z Reads: 211

```
Yup. Been doing cable. Sucks tho because I would have to always open my enclosure. :disappointed_relieved:

Can't wait for the new app. Hopefully, it will have modes that we can easily switch out.
```

---
## \#652 Posted by: Goldcoastguy Posted at: 2019-03-26T00:34:48.683Z Reads: 218

```
![Screenshot_20190326-103012|243x500](upload://hjW07SYQCVF6LpO3gOlhg6NdZo5.jpeg) ![20190326_102809|375x500](upload://alXq10FEc2smalfrr4b2oygQ437.jpeg) 

![20190326_103259|375x500](upload://vzZmzo9K21Dn1TsMkxmn6AEkiAi.jpeg) 

Flux measurement failed, first time using focbox tools can't seem to get it working 😅
```

---
## \#653 Posted by: Blasto Posted at: 2019-03-26T01:12:52.479Z Reads: 197

```
Install your belts and spin the wheels
```

---
## \#654 Posted by: mackann Posted at: 2019-03-26T06:50:58.852Z Reads: 202

```
You could buy a metr bluetooth and use that app to change the settings if you don´t want to wait.
https://metr.at/shop It supports Unity and have a lot of cool features
```

---
## \#655 Posted by: pookybear Posted at: 2019-03-26T06:57:42.237Z Reads: 208

```
I have it. My feather remote is using the uart port. I could use the internal one but I need to be able to switch baudrate. This requires a "custom firmware" that doedand provided. I know this because sofu has it and provided the link to share with deodands permission of course.

I just need to get off my lazy @$$ and make a connector for the internal pinouts so I could connect my feather remote there and use the external for the metr. I believe this is what sofu has in her haya.
```

---
## \#656 Posted by: brently Posted at: 2019-03-26T13:57:19.361Z Reads: 211

```
I'm having the same issue on from dead stop launches. Like you said no issues if I ease on to it just if I try and launch it'll shutter after launching. Makes predicting behavior from a stop hard. Have you been able to fix it? I'm running pretty much the same settings as you at the moment but the issue occurs pretty no matter what I make the Max Battery and Max Motor currents. 

My set up is: 12s6p Samsung 30Q, BMS specs in pic below, 4:1 gear drive, 8'' pneumatics, dual 6384 sensored 200kv motors. 

![image|674x500](upload://sPHIkOFfxI6xDJvfWwLBN1Yl165.jpeg)
```

---
## \#657 Posted by: rsalmon Posted at: 2019-03-26T14:16:25.439Z Reads: 209

```
In my case since my motors are sensorless, increasing Openloop ERPM parameter has helped, at least on the bench. We haven't had the chance to test on the street yet.

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/e/7/e74b6140cc3f93bf1e8834dfa67ead5311bd13e8.png)

Have you tried this suggestion?
https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/607
```

---
## \#658 Posted by: Goldcoastguy Posted at: 2019-03-27T07:36:16.869Z Reads: 197

```
Hi thanks for the reply,  I tried with belts on first and I've tried a motor off my spare board with the same message 😅
```

---
## \#659 Posted by: Blasto Posted at: 2019-03-27T11:19:07.843Z Reads: 196

```
What kv are those motors?
```

---
## \#660 Posted by: Goldcoastguy Posted at: 2019-03-27T18:50:48.167Z Reads: 198

```
They are Turnigy G160 290kv I also tried a Diye 270kv 5055
```

---
## \#661 Posted by: Blasto Posted at: 2019-03-27T19:01:11.403Z Reads: 205

```
that's quite a high KV for a low gear reduction... might want to look in to a lower Kv around 190

anyhow, for high Kv motors, it is better you have you belts on and you need to give the wheel a real good spin
```

---
## \#662 Posted by: Goldcoastguy Posted at: 2019-03-28T04:04:20.158Z Reads: 209

```
Ok spinning the wheels super fast worked! Definitely prefers a little push to start. 

![received_2159876547463417|666x500](upload://lac5Pcjm8lasOe5fSLYYA6maVuC.jpeg)
```

---
## \#663 Posted by: rey8801 Posted at: 2019-03-29T12:52:06.490Z Reads: 206

```
ok we all know the DRVspecs ecc...but I would like to know. Did someone already tried the unity for hundreds km/miles with a 13s battery? We need a brave tester :grin:
```

---
## \#664 Posted by: mackann Posted at: 2019-03-29T12:57:45.595Z Reads: 206

```
Working on it..
```

---
## \#665 Posted by: Arek Posted at: 2019-03-30T15:04:25.246Z Reads: 204

```
Hi, app looses communication with the unity after short time or when I try to upload the configuration, nothing updates and I have to reconnect many times, bluetooth led on the controller is lit all the time.
I'm using OnePlus 3T running android 8.0.0.
```

---
## \#666 Posted by: pookybear Posted at: 2019-03-30T15:09:10.612Z Reads: 208

```
[quote="Arek, post:665, topic:77861"]
Hi, app looses communication with the unity after short time or when I try to upload the configuration, nothing updates and I have to reconnect many times, bluetooth led on the controller is lit all the time. I’m using OnePlus 3T running android 8.0.0.
[/quote]

Same thing happens to me. OnePlus 7.1.2 here though. Perhaps, it's our phone? I have use the same phone to change settings when I was using my dualfocbox running metr pro though. 

I've noticed it mostly happens when I change motor settings. It "hangs" then does nothing.
```

---
## \#667 Posted by: janpom Posted at: 2019-03-30T22:19:20.278Z Reads: 198

```
I just installed Xmatic and tried connecting to my new Unity. It worked just fine, which is both great and worrying. Shouldn't there be some kind of pairing process? Does this mean that anyone with a bluetooth device and correct software can connect to my Unity and change my settings? I wouldn't quite appreciate that. @Deodand?
```

---
## \#668 Posted by: mackann Posted at: 2019-03-31T17:40:13.826Z Reads: 198

```
Yes they can, atleast for the moment. The only way is to unplug the Unity Bluetooth module and buy a metr pro module and use that app instead to protect you from anyone changing your settings
```

---
## \#669 Posted by: janpom Posted at: 2019-03-31T17:45:49.482Z Reads: 200

```
That's pretty bad. @Deodand please fix that. This is a serious vulnerability.
```

---
## \#670 Posted by: mackann Posted at: 2019-03-31T18:10:57.742Z Reads: 204

```
This have been for all kind of vesc modules, nothing new that their is no protection against it.
My gues is that they are working on it but i dont think its so easy to implement. If you dont want to wait buy a metr for ~40usd
```

---
## \#671 Posted by: janpom Posted at: 2019-03-31T18:35:07.740Z Reads: 206

```
Yeah, but the BT module is built into the Unity. It's what you get as a part of the package that you pay for and thus it's reasonable to expect  certain security standards will be met. Having to use Metr is not an acceptable workaround for me even though I have one.
```

---
## \#672 Posted by: janpom Posted at: 2019-03-31T18:59:05.727Z Reads: 206

```
I thought about it for a bit. What I would do as a minimal dev effort fix would be release a version of the FW that only allows reads over UART. It would forbid all writes over UART. You would have to use USB to change settings once you install that FW. People would still have the option to use the unrestricted FW if they want to keep the flexibility of being able to change settings over BT (and at the same time they like to live dangerously).
```

---
## \#673 Posted by: colinphotovideo Posted at: 2019-04-01T14:19:38.971Z Reads: 198

```
I'm using the Unity switch but also have my battery using an e-switch. If I take out the power switch connected to the battery and solder the wires together will this allow me to use only the Unity to power on and off?

Just want to double check thanks 👌🏻
```

---
## \#674 Posted by: venom121212 Posted at: 2019-04-01T15:05:44.972Z Reads: 199

```
A picture of the e switch will help to make sure but all 2 wire switches I've come across just close the circuit when pressed and open it when closed.
```

---
## \#675 Posted by: xjet Posted at: 2019-04-01T17:28:11.551Z Reads: 202

```
I received my unity last week and over the weekend I installed it in my build. I have a honor view 10 running android pie. I used the focboxui android app to set this up. I scanned bluetooth and connected. I updated the firmware. I ran through the config all seamed normal.  Motor setup and ppm set all looked like they went through, saved the config, but one motor was running  in reverse. I also had bad stuttering on the motors. I did the same on the pc app through usb and it is working. Just wondering if I am doing something wrong or bug? And 😈 for post 666....
```

---
## \#676 Posted by: venom121212 Posted at: 2019-04-01T17:47:04.806Z Reads: 201

```
There's a small circle/arrow in the app. Click that and it will reverse that motors direction
```

---
## \#677 Posted by: xjet Posted at: 2019-04-01T17:55:24.604Z Reads: 200

```
I did try that and wrote the config with no change. The motors were wonky too... stuttering sounded weird etc. The pc app did fix it all for me so not a huge deal. The Unity is bad ass btw...
```

---
## \#678 Posted by: venom121212 Posted at: 2019-04-01T18:10:51.659Z Reads: 197

```
Hmm weird. Yeah I'm enjoying it. Glad it worked out for you!
```

---
## \#679 Posted by: AlanZhou Posted at: 2019-04-02T01:52:50.578Z Reads: 204

```
Seems enertion is in a hurry, didn't get a instruction manual with one of my unitys, now I don't know how to use it 🤨😂
```

---
## \#680 Posted by: Jaydawg56 Posted at: 2019-04-02T01:57:12.892Z Reads: 205

```
Still waiting on mine which was ordered in Dec.
```

---
## \#681 Posted by: drone001 Posted at: 2019-04-03T02:41:19.937Z Reads: 208

```
Can I change this connector to fit the Unity, if so does anyone know where I can find them?[20190402_212819|374x500](upload://tGc2d3UaSel4hocnf2DLdxpRZxy.jpeg) ![20190402_212819|374x500](upload://tGc2d3UaSel4hocnf2DLdxpRZxy.jpeg)
```

---
## \#682 Posted by: Blasto Posted at: 2019-04-03T02:45:37.710Z Reads: 206

```
Jst zh 6 pins, you can get some adapters or a pig tail from ebay

Dont forget to insulate those phases leads.
```

---
## \#683 Posted by: drone001 Posted at: 2019-04-03T02:47:17.577Z Reads: 203

```
indeed..just sizing things up for now....waiting on parts. thx
```

---
## \#684 Posted by: PickSix24 Posted at: 2019-04-03T02:48:44.865Z Reads: 210

```
https:///collections/electrical-connectors/products/vesc-sensor-wires
```

---
## \#685 Posted by: drone001 Posted at: 2019-04-03T02:50:43.674Z Reads: 203

```
beautiful.....putting my order in now...thx bruh!!
```

---
## \#686 Posted by: CarlCollins Posted at: 2019-04-03T04:29:50.757Z Reads: 199

```
@AlanZhou

That's strange, I always thought you might have the basic knowledge of ESCs already as you are on the forum quite a bit.
```

---
## \#687 Posted by: AlanZhou Posted at: 2019-04-03T11:51:24.967Z Reads: 201

```
Lol I was joking
```

---
## \#688 Posted by: mackann Posted at: 2019-04-03T17:39:10.180Z Reads: 199

```
I think Carl did to 😂
```

---
## \#689 Posted by: AlanZhou Posted at: 2019-04-03T18:00:40.964Z Reads: 205

```
It sounded so formal 🤣
```

---
## \#690 Posted by: CarlCollins Posted at: 2019-04-04T09:21:47.985Z Reads: 204

```
It''s kind of Serious joke :stuck_out_tongue:
```

---
## \#691 Posted by: rideTastic Posted at: 2019-04-04T09:31:36.062Z Reads: 209

```
I have the same problem with my raptor 2.1. According to Bara I get a replacement motor. Should I until then turn off all Hall sensors completely?

I exchanged the 6pin cables connected to the Unity for each other. It is still the same motor affected. That means it should be a defective cable from the motor?

![55914113_323812868499900_5680617341616914432_n|243x500](upload://pLrtJFUH3je0XeHOSZNrTNnGeSu.jpeg)
```

---
## \#692 Posted by: sayekim Posted at: 2019-04-04T10:24:50.733Z Reads: 204

```
In a dual esc setup you can run one sensored and the other unsensored and with canbus use the traction control to have a smooth start like both are sensored. 

I have it setup like this because one of my motors hall censor detection gave a bad result. I think it’s fried, the sensor at least. Not the motor. 

I guess this works with the unity too?
```

---
## \#693 Posted by: rideTastic Posted at: 2019-04-04T15:13:16.865Z Reads: 209

```
I don't know. I think the best would be to just keep riding and wait for the replacement engines? 

I also sometimes have a stuttering wheel in Rspec mode. This doesn't happen in slow mode. Does this have anything to do with the defective hall sensors?

https://www.youtube.com/watch?v=q-kTvdwvCS0

This is what it looks like in the tool ![20190404_165233|374x500](upload://n27xyGBvy8ey079QuyLLTYiumTg.jpeg)
```

---
## \#694 Posted by: Lex Posted at: 2019-04-04T21:56:06.216Z Reads: 201

```
Hy mate... did you find a solution for the Firefly remote to your R2 ??
```

---
## \#695 Posted by: Scream Posted at: 2019-04-04T22:44:54.529Z Reads: 203

```
I did fiddle with the code a bit. But no, I never got unity data showing on the firefly screen. 

I know the unity is working with the firefly nano, so basically I tried to replace the relevant firefly code with the relevant code from the firefly nano. Whatever I did left the remote functional, but didn’t bring up any useful data for the remote. In the end I gave up and bought the new flipsky remote. I don’t regret it, but it is a shame to waste my wooden/aluminium firefly chassis.

I can share my progress later, when I get home. Someone might be able to point out where I went wrong.
```

---
## \#696 Posted by: Lex Posted at: 2019-04-04T22:47:24.349Z Reads: 195

```
Thanks for the reply... No stress at all. I'm happy when you can send it duering the weekend. im curious. THX
```

---
## \#697 Posted by: danepoostain Posted at: 2019-04-05T01:10:54.654Z Reads: 189

```
ok im super lost. where and how do i get the unity app for windows?
```

---
## \#698 Posted by: AlanZhou Posted at: 2019-04-05T01:12:38.713Z Reads: 192

```
Dig in the files it's in there

Its not a program it's just a file
```

---
## \#700 Posted by: danepoostain Posted at: 2019-04-05T01:18:44.980Z Reads: 189

```
where tho? 

what files?
```

---
## \#701 Posted by: AlanZhou Posted at: 2019-04-05T01:30:33.664Z Reads: 186

```
its in the folder \
windows_build
```

---
## \#702 Posted by: CarlCollins Posted at: 2019-04-05T01:50:34.960Z Reads: 186

```
Here: https://enertionboards.zendesk.com/hc/en-us/articles/360000660795-Windows-Tool-for-Unity
```

---
## \#703 Posted by: Bas1 Posted at: 2019-04-05T07:48:02.971Z Reads: 198

```
So if I use the Standard setup guide in the standard tool It automatically will run it in foc. if I want it in bldc I need to use the advance setup tool?.
https://youtu.be/C7MtbMTKrOs
```

---
## \#704 Posted by: venom121212 Posted at: 2019-04-05T13:42:59.189Z Reads: 208

```
@Deodand I was able to capture a few errors I've been dealing with, hopefully you can help.

![Screenshot_20190405-093624|236x500](upload://dEyojdLSdKvND6CKYHaRgj4pUk1.jpeg) ![Screenshot_20190405-093634|236x500](upload://2hguB9rK3kM1d6u1X5diHSGxH6P.jpeg)


When letting off of throttle and then re-engaging, I often get the sound of the motor clicking and then not responding. I notice the unity throws off a flashing light whenever this happens. It has happened on 3 remotes now. 

https://youtu.be/fTXOV4pCoEw

Particularly scary when throttle doesn't re-engage when I need to stop.
```

---
## \#705 Posted by: zManiac Posted at: 2019-04-05T20:11:55.686Z Reads: 198

```
I keep getting this calculate error L2 is 0. Please measure it first. Dose anyone know what it is?
```

---
## \#706 Posted by: plasteroid Posted at: 2019-04-07T03:27:51.443Z Reads: 199

```
Hi all - after a long winter and other distractions, finally getting around to setting up my Unity.

I was reading here on the forum, that I should not update the Firmware???  Is that right? 

Whereas when I try to go to Motor Settings, I getting this prompt- and cannot proceed...

Sorry if this has been answered...

![image|690x397](upload://gRg6yZJPyTiQMnkEyuVRYmbG51W.png)
```

---
## \#707 Posted by: Blasto Posted at: 2019-04-07T03:32:48.614Z Reads: 194

```
You are using the proper tool for the hardware you have. You can proceed to update the firmware.
```

---
## \#708 Posted by: Silverline Posted at: 2019-04-07T08:14:19.164Z Reads: 195

```
Enough talk about that damn warranty....

This is how the unity should have come in the first place for diy builders. 

Longer motor wires,
4mm banana plugs,
Xt90

No warranty I know.... But this is a DIY builders forum, I am the warranty...
![IMG_20190407_100843609|690x388](upload://9YVDor0j0ozjc4VXJhdxumEJEB4.jpeg)
```

---
## \#709 Posted by: Meeep Posted at: 2019-04-07T08:29:53.624Z Reads: 191

```
Hey y'all was finally able to try and set up my unity but I can't get the thing to connect to my desktop via USB-C. Tried some different cables and ports on my computer but it's like its not there.
```

---
## \#710 Posted by: Gerrycorrado Posted at: 2019-04-07T08:52:11.818Z Reads: 208

```
We urgently need answers to all above questions iso some of the questions.
Had stuttering yesterday too. Will firstly lower the amp values and try again. Ah and look for the traction control (thought it was always on, seems not haha)
```

---
## \#711 Posted by: Marsl187 Posted at: 2019-04-07T21:10:46.727Z Reads: 206

```
Hey guys,
I'm using the Unity on my Mountainboard Build and almost suffered a horrible crash today because of a sudden **cutout** at hard accelerating like @mackann told.

I guess I almost had 45km/h+ on the clock so it did occur quite late. But yeah threw me off almost, glad I hat my bindings...
Also I have these stutters when full accelerating from a dead stop sometimes. 

My settings are:

* Motor Max 80A
* Battery Max 60A
* Motor Min -60A
* Battery Min -30A

So I guess the settings are quite conservative. 

Does anyone have found out more about these problems? 

I'm a bit scared now to try again and try to reproduce the error...
```

---
## \#712 Posted by: Ubbiedude Posted at: 2019-04-07T21:12:16.355Z Reads: 202

```
Did you hook it up to a charged battery?
```

---
## \#713 Posted by: Deodand Posted at: 2019-04-07T21:39:59.481Z Reads: 198

```
Yeah we are investigating this, it's currently my number one priority. What motors are you running? Can you share a screenshot of your motor config?

Were you able to check faults as mackann?
```

---
## \#714 Posted by: Meeep Posted at: 2019-04-07T21:42:50.556Z Reads: 190

```
lol yes, always good to start with the basics though. I ended up contacting Enertion support through the site. I think the usb-c connector is bad. Hopefully they will take care of it. The box had one noticeable dent in it so maybe it's USPS's doing :roll_eyes:
```

---
## \#715 Posted by: Deodand Posted at: 2019-04-07T21:44:08.252Z Reads: 189

```
You're using tha usb A to usb C cable that came in the box?
```

---
## \#716 Posted by: Meeep Posted at: 2019-04-07T21:45:14.792Z Reads: 186

```
Yessir, tried the one that came with my pixel 2 phone too.
```

---
## \#717 Posted by: Deodand Posted at: 2019-04-07T21:46:58.802Z Reads: 183

```
device show up in the control panel when you plug/unplug?
```

---
## \#718 Posted by: Meeep Posted at: 2019-04-07T21:50:04.606Z Reads: 182

```
Tbh I would have to double check that. But I don't believe so. In the FOCBOX tool only COM 1 shows up and gives the error "Cannot read firmware. Please make sure port is assigned to focbox" or something like that.
```

---
## \#719 Posted by: Deodand Posted at: 2019-04-07T21:52:59.928Z Reads: 181

```
I'd double check, if a device shows up but says something like "unrecognized" it can just be a driver issue. If no device shows up at all then it's probably a faulty port. But every unity is connected through USB twice before passing QC so it shouldn't be possible unless your box was absolutely crushed by something.
```

---
## \#720 Posted by: Meeep Posted at: 2019-04-07T22:00:36.671Z Reads: 180

```
I just double checked on there is nothing showing up on the control panel... Bluetooth connected fine. Turns on fine.
```

---
## \#721 Posted by: Deodand Posted at: 2019-04-07T22:03:40.256Z Reads: 181

```
That's disappointing, by chance plug into another random computer just as a final check? Does seem to be a bad connection there though.
```

---
## \#722 Posted by: Meeep Posted at: 2019-04-07T22:05:23.097Z Reads: 185

```
I have my macbook here, would it show up/suffice for testing this? I am using my Windows 10 desktop currently.
```

---
## \#723 Posted by: Deodand Posted at: 2019-04-07T22:17:11.451Z Reads: 180

```
Sure something should show up in the devices. (Don't know Mac very well)
```

---
## \#724 Posted by: Meeep Posted at: 2019-04-07T22:18:09.174Z Reads: 180

```
Just checked and nothing shows. Using the same cable I connected my Pixel phone and it did register but couldn't connect.
```

---
## \#725 Posted by: Deodand Posted at: 2019-04-07T22:19:36.968Z Reads: 179

```
Not sure how this unit got through our test jigs :angry: sorry this is causing you annoyance.
```

---
## \#726 Posted by: Meeep Posted at: 2019-04-07T22:23:21.347Z Reads: 182

```
Hey, don't be too hard on yourself! This is a great product, going through the guided setup was very painless. I actually crashed last week (got hit by a car) so I have plenty of time to have it resolved. I already chatted with support and sent them a video as per their request this morning. Thank you Jeffery, your help is deeply appreciated. 

Anything else I should do?

EDIT: I just wanted to clarify that I have not used the Unity other than setting up and bench testing. I re-read my post and saw that it wasn't clear. Forgive me for any confusion that might of caused.
```

---
## \#727 Posted by: Marsl187 Posted at: 2019-04-07T23:15:37.094Z Reads: 181

```
Thanks for your effort! I like the Unity quite much, I already ordered a second one for another build. I hope it is not a hardware issue as it seems not occurring at every user.

Here are my settings:

![Unity_Settings|334x500](upload://kKkUaWwyF9XGncBlKSbNubgoJza.png) 

I'm running two Turnigy SK8 6374 192 kV motors. And I am on 12S not 10 like in the picture...

Unfortunately I wasn't able to check the faults as I am an iPhone user and it turned itself off till I was home... Maybe I can reproduce this behavior by pushing a car away or so..
```

---
## \#728 Posted by: Deodand Posted at: 2019-04-07T23:18:09.486Z Reads: 177

```
Thanks for sharing the settings screen, very helpful. 

On your BMS are you running charge only or discharge? You have 12s selected in unity settings normally?
```

---
## \#729 Posted by: AlanZhou Posted at: 2019-04-07T23:20:32.112Z Reads: 179

```
Erm xt 90 is not needed 4mm bullets are also overated you will almost never discharge enough amps to cause damage to the stock config that's why enertion does not ship it that way and also because they use the stock config for the raptor 😂
```

---
## \#730 Posted by: venom121212 Posted at: 2019-04-07T23:32:58.664Z Reads: 183

```
@deodand please shoot me a pm whenever you want to troubleshoot my problem above. Very annoying issue. 

https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/704?u=venom121212
```

---
## \#731 Posted by: Marsl187 Posted at: 2019-04-07T23:35:02.150Z Reads: 178

```
The BMS is for charging only. 

Normally yes, but I had problems by installing a new remote so I ran again trough the setup guide, seems like I forgot to change that setting. Battery was full when to error occurred, it should be able to deliver 90A without problems. 

Any possibility that the error was caused by the wrong voltage settings?
```

---
## \#732 Posted by: Deodand Posted at: 2019-04-07T23:37:31.425Z Reads: 172

```
Probably not if battery was fully charged and the BMS was bypassed.
```

---
## \#733 Posted by: Deodand Posted at: 2019-04-07T23:39:24.008Z Reads: 183

```
How many flashes? I'm assuming you mean a flashing red? Sounds like a fault is being thrown if you catch the number of flashes that is the fault number. Better yet get it to throw the fault and without power cycling connect to the app and type "faults" in the terminal. 

Sorry I have been out of town last week got a bit behind on answering people.

Edit: just saw screenshots :smile:
```

---
## \#734 Posted by: Deodand Posted at: 2019-04-08T04:28:18.626Z Reads: 183

```
@Marsl187 @mackann @rsalmon I think I have targeted the issue and fixed it. Initial testing looks good (thanks @sofu) really sorry that anyone had to experience this (the specific issue mostly effects large high kv motors 6374+ 190 kv+) and depends on winding resistance. 

A new app will go live in 1-2 days and a firmware update should fix it. A few other fun little bits in there as well :slight_smile:
```

---
## \#735 Posted by: mackann Posted at: 2019-04-08T05:16:21.260Z Reads: 180

```
Great, cant wait to try it. What was the problem or how did you fix it?
```

---
## \#736 Posted by: Deodand Posted at: 2019-04-08T05:31:53.113Z Reads: 182

```
changed something in the detection routine that I shouldn't have and it skewed detection of resistance for larger motors slightly. My mistake, I need to accumulate a more complete host of test motors before making these types of changes. Live and learn.
```

---
## \#737 Posted by: egzplicit Posted at: 2019-04-08T10:15:23.006Z Reads: 176

```
Glad the issue was found. I just received my unity and it seems a great piece of kit but I am worried that these software bugs can have a big impact on a rider health 😁. My trampa uses 6374 and 190kv so I can assume if I was to switch to the unity today, I would have been impacted by this issue.

We need to make sure firmware changes are properly tested before going live due to... health and safety reasons 😏
```

---
## \#738 Posted by: sayekim Posted at: 2019-04-08T10:24:55.706Z Reads: 171

```
This is exactly the sort of reason why I wouldn’t wanna be a first batch guinea. 

I’m leaning towards just buying some vesc 6. Surely they are tried and tested. Right?
```

---
## \#739 Posted by: murloc992 Posted at: 2019-04-08T10:25:41.720Z Reads: 169

```
Kind of glad all of my parts are not there yet to kill me before dangerous bugs are ironed out. :smiley:
```

---
## \#740 Posted by: venom121212 Posted at: 2019-04-08T13:38:55.382Z Reads: 165

```
Eh every device/user/situation is different. I've been full throttling my 6374 190kv motors regularly and have had no issue with the first batch of Unities. 

Regardless, good to hear about updates focused on safety!
```

---
## \#741 Posted by: Deodand Posted at: 2019-04-08T15:15:53.641Z Reads: 174

```
All I can do is be honest about the issue, fixes should be released by today. Being a DIY builder/rider in general carries these risks unfortunately as it's somewhat impossible to test every possible permutation of a build under all riding styles. I did actually test with this style motor, but it only occurs on certain motors under heavy current. We tested the unity with a pretty wide variety of builds before launch, I think we had about 20 beta testers but unfortunately this slipped through. I'm pretty sure we even have riders with these specific motors and no issue present so it might be one of those variance things where certain motors/unities at the tips of the bell curves were causing issues.  

These aren't excuses just trying to explain the situation. I will always be striving to setup more thorough test procedures to ensure safety.
```

---
## \#742 Posted by: mackann Posted at: 2019-04-08T15:44:18.287Z Reads: 172

```
Yes, I have 6 test boards with almost all same motors and setup, but only 1 did have this problem. So I understand it must be hard to test/find/fix this problem.
```

---
## \#743 Posted by: briman05 Posted at: 2019-04-08T16:32:39.033Z Reads: 174

```
Maybe a bigger batch of beta testers in the future in different climates/ evironments and areas of the world.  Twenty beta testers is a good amount but a hot and humid beach area would have a different response to the electronics than a person in a warm area with low humidity and hills.
```

---
## \#744 Posted by: Silverline Posted at: 2019-04-08T17:37:24.376Z Reads: 177

```
Just got my Unity up an running... i have two questions though....

1. In the Focbox UI, when is set the "Max battery discharge current" is this in total or pr. side/motor ??

2. With my old focboxes when i switch off the remote (simulating failsafe) it would just free roll. But on the Unity the motors brakes pretty massiv, throwing me of the board. Any where in the UI, i can change that ??
```

---
## \#745 Posted by: Deodand Posted at: 2019-04-08T17:45:18.918Z Reads: 174

```
1) its total

2) Hard to answer without seeing the behavior of the ppm signal when the remote is switched off (different remotes have different behavior). There are some advanced options relating to this in the full tool but not the app currently.
```

---
## \#746 Posted by: Silverline Posted at: 2019-04-08T17:50:48.920Z Reads: 176

```
1. Okay thanks.... maybe a little confusing... since the motor max is pr. motor, but battery max is in total. Maybe a note about that in the app ? (maybe its bacause i´m use to setting up two seperate focboxes)

I have problems connecting via BLE modul in the full tool.... But i guess i have to take the board apart in order to connect via micro usb then......
Its the "golden standard" remote Flysky GT2B.... its pretty insane how much braking power it throws when going in to failsafe mode, much stronger braking power than braking on the remote manually .
```

---
## \#747 Posted by: murloc992 Posted at: 2019-04-08T17:52:32.429Z Reads: 173

```
[quote="Silverline, post:746, topic:77861"]
Its the “golden standard” remote Flysky GT2B…
[/quote]

I will add that throttle goes to 1500 when idle. I don't think my unity does that though. Did you calibrate it properly?

https://www.youtube.com/watch?v=sk2ldPtm09Y

Can be seen that it free rolls.
```

---
## \#748 Posted by: Deodand Posted at: 2019-04-08T17:54:16.632Z Reads: 175

```


[quote="murloc992, post:747, topic:77861"]
throttle goes to 1500 when idle
[/quote]

does this mean 1.5 ms? if so the unity should idle just fine.
```

---
## \#749 Posted by: murloc992 Posted at: 2019-04-08T17:54:35.935Z Reads: 172

```
[quote="Deodand, post:748, topic:77861"]
if so the unity should idle just fine.
[/quote]

Added old video, it does indeed.
```

---
## \#750 Posted by: Silverline Posted at: 2019-04-08T18:00:00.137Z Reads: 182

```
This is when the throttle is in idle (mid. Pos.)
No matter how many times i calibrate. It stays at 46%
![Screenshot_20190408-195734|236x500](upload://4DT5Mn7toONQaSlBUjCvq2xZEWT.png) 

And this is when i turn off the remote
![Screenshot_20190408-195741|236x500](upload://etekTIQF3IbpdZVDyaii5bQ1feC.png)
```

---
## \#751 Posted by: Deodand Posted at: 2019-04-08T18:01:47.582Z Reads: 170

```
I  need to improve the interface here,I'd go ahead and calibrate with the full tool so you can see more information and figure out what exactly is going.
```

---
## \#752 Posted by: murloc992 Posted at: 2019-04-08T18:02:33.980Z Reads: 167

```
Seems to go to 0 instead of 1500. That's weird. It should be in the 1000-2000 range even when off.. I have three and all act the same
```

---
## \#753 Posted by: Silverline Posted at: 2019-04-08T18:04:49.553Z Reads: 169

```
Sorry guys.... I just did the calibration again.... now in idle.... it stays at -9%, and when I power off the remote its just free roll like i want :slight_smile:
```

---
## \#754 Posted by: murloc992 Posted at: 2019-04-08T18:05:35.676Z Reads: 163

```
Somebody forgot to pull on the brakes when calibrating.. :smiley:
```

---
## \#755 Posted by: Silverline Posted at: 2019-04-08T18:06:13.010Z Reads: 164

```
No forgot the push "save" :blush::blush:
```

---
## \#756 Posted by: murloc992 Posted at: 2019-04-08T18:06:49.822Z Reads: 166

```
Happens. Now go and free roll! Free roll forever! :laughing:
```

---
## \#757 Posted by: Deodand Posted at: 2019-04-08T18:07:53.701Z Reads: 164

```
Thanks for the added help @murloc992
```

---
## \#758 Posted by: Silverline Posted at: 2019-04-08T18:34:11.846Z Reads: 168

```
Just did a test ride..... Very very nice...  Love the unity.... Awesome. So fast and easy to change settings with the Focbox app.

I have escapes (vesc 6 clones) on my other trampa build...... And i must say that the Unity is more smooth to me, and keeping the motors cooler.
```

---
## \#759 Posted by: RobPBody Posted at: 2019-04-08T19:13:59.485Z Reads: 170

```
@Deodand Hi all, new builder here. I have my Unity, and when I'm going through the motor setup (Sensor-less), I see an Error after the "Spin Wheels Forward" stating failure to detect. And when I go to the HUD screen after finishing and applying settings, once I get to maybe 20-30% throttle, there's a popping sound. There is no load at the time. Looking at the bullet connectors, there's charring on 1 of the three motor connects on each motor. I have the maximum at 60a both for Battery and Motor. Any troubleshooting ideas?
```

---
## \#760 Posted by: sayekim Posted at: 2019-04-08T19:53:52.495Z Reads: 173

```
[quote="Deodand, post:741, topic:77861"]
All I can do is be honest about the issue
[/quote]

That’s all we want here and it to be fixed of course. Bad for business perhaps but that’s only because it’s not the norm.

The vesc firmware gets constant updates too still ironing out bugs as it goes along.
```

---
## \#761 Posted by: pjotr47 Posted at: 2019-04-08T20:05:32.489Z Reads: 172

```
Yeah :wink: 

![image|690x388](upload://lu2EKUHYi2rMc3FtiXuAKXiyQs3.jpeg)
```

---
## \#762 Posted by: Silverline Posted at: 2019-04-08T20:13:39.371Z Reads: 167

```
Amen m8....
```

---
## \#763 Posted by: Aero Posted at: 2019-04-08T20:41:36.716Z Reads: 169

```
Does anyone use Metr modes to change settings? I’m wondering if this is safe to use with the Unity?
```

---
## \#764 Posted by: goldrabe Posted at: 2019-04-08T20:51:13.787Z Reads: 171

```
Metr. works for me, but I have changed settings only once.
```

---
## \#765 Posted by: Deodand Posted at: 2019-04-08T21:07:00.037Z Reads: 172

```
Maybe double check you have good solder joints on those connections? Are you giving the wheels a good strong hand spin during calibration?

example of handspin here: 

https://youtu.be/MqVXMM8iahM?t=367
```

---
## \#766 Posted by: accrobrandon Posted at: 2019-04-10T00:37:05.380Z Reads: 168

```
Hi,

been rocking this unity for a few days now. still havent gotten push to start to work..and with pnuemies its more effort than i want... read some post that say you gotta push hard a good few time perhaps even getting up to 7-9mph? if so thats way too much effort... so as some have mentioned perhaps a "sensitivity" slider?? aside from that everything else is good!
```

---
## \#767 Posted by: Meeep Posted at: 2019-04-10T01:34:28.850Z Reads: 162

```
Please! Please! I really liked being able to kick spin the wheels on my meepo esc. Then drop it down and go. Sure, sometimes I accidentally turned it on but it had an audible beep to let you know.
```

---
## \#768 Posted by: venom121212 Posted at: 2019-04-10T01:51:47.286Z Reads: 163

```
Man I haven't even tried this setting because of the trouble I've seen urethane users having. I'm going to try out push to start tomorrow just for kicks (pun intended and landed)
```

---
## \#769 Posted by: accrobrandon Posted at: 2019-04-10T02:24:29.722Z Reads: 162

```
yeah meepo was hella easy... a quick extension of the leg and it turned on, shouldnt be any harder than that!
```

---
## \#770 Posted by: accrobrandon Posted at: 2019-04-10T02:25:30.642Z Reads: 168

```
yeah it tried on a part of the street that was a mild downhill so i could get a couple good pushes and hope to roll easier and even at low chill coast...didnt turn on =/
```

---
## \#771 Posted by: goldrabe Posted at: 2019-04-10T03:05:04.895Z Reads: 172

```
I pushed my board without being on it, that worked.\
Anyway I hated the push to start meepo ESC, it was way too easy to engage it and could have led to trouble if your remote would sit in a pocket pushed. Let alone the annoying beep.
```

---
## \#772 Posted by: accrobrandon Posted at: 2019-04-10T03:08:57.204Z Reads: 170

```
...but now i have to ask... why would your remote be in your pocket AND turned on? ..but the boards off? =P if my board is laying flat on the ground that usually means its ready to ride at a moments notice haha
```

---
## \#773 Posted by: Meeep Posted at: 2019-04-10T03:11:38.372Z Reads: 167

```
You are right. I got into the habit of always turning the remote off. I think the meepo manual says to do that idk.
```

---
## \#774 Posted by: goldrabe Posted at: 2019-04-10T03:13:16.537Z Reads: 166

```
Sometimes I like to push in pedestrian areas etc. All kind of shit can happen. Once I put my board just down on the street and the ESC engaged before I pulled out the remote.\
Give the feet push a try, worked for me.
```

---
## \#775 Posted by: Deodand Posted at: 2019-04-10T03:37:27.374Z Reads: 172

```
Just to be clear the push to start feature is hardware defined (not software) so a hardware change would be required to adjust threshold unfortunately. There's probably a way we could change the hardware to make it more adjustable for future revisions. I have a few ideas to test. The push to start was just kind of a bonus feature that came with our switch topology, personally I find the autoshutoff to be much more useful since I'm a bit forgetful :slight_smile: 

We prioritized preventing the switch from drawing passive current in the off-state over allowing it to be software controlled.
```

---
## \#776 Posted by: huntercasillas Posted at: 2019-04-10T06:25:44.002Z Reads: 170

```
What is required to make push to start work? Does it work on belt driven boards or only hubs?
```

---
## \#777 Posted by: Deodand Posted at: 2019-04-10T06:28:02.588Z Reads: 173

```
Kinda depends on your setup, the most important parameters would be theoretical top speed of your build and passive rolling resistance. Essentially you need to push to generate a few volts of back emf, so it depends on motor kv (V/rpm) gear reduction and wheel diameter as to what speed you need to push and sustain for roughly 1-2 seconds while the system boots.
```

---
## \#778 Posted by: Aero Posted at: 2019-04-10T06:36:55.249Z Reads: 173

```
Hey @Deodand, any update on the sudden cutout during acceleration issue? (Really liking the Unity but this has me concerned) thanks!
```

---
## \#779 Posted by: mackann Posted at: 2019-04-10T07:47:43.126Z Reads: 181

```
Tell me about it :smile: :joy: 
![IMG_20190403_140222|666x500](upload://6AXQ8YoTzl0INmOociKueeVCI2j.jpeg) ![IMG_20190403_141937|374x500](upload://emzxGnIlVH5GxumS2uDg4kSN1tf.jpeg)
```

---
## \#780 Posted by: mackann Posted at: 2019-04-10T07:50:53.661Z Reads: 176

```
I think it will be fixed in the new firmware that releases this week ( I guess you have 6374+ motor and 190+kv) ?
```

---
## \#781 Posted by: Aero Posted at: 2019-04-10T10:00:52.160Z Reads: 175

```
Wow, that’s a lot of unities :joy: I’m running 6374’s and 190kv.
```

---
## \#782 Posted by: PickSix24 Posted at: 2019-04-11T05:04:23.564Z Reads: 175

```
@Deodand will the next update allow us to change the uart baudrate or is the only option the custom firmware ? I’d like to be able to use the second uart.
```

---
## \#783 Posted by: pookybear Posted at: 2019-04-11T05:17:39.293Z Reads: 173

```
I second this. Well a little late now. Sold my unity today.
```

---
## \#785 Posted by: PickSix24 Posted at: 2019-04-11T12:37:48.593Z Reads: 178

```
Does the windows app allow you to change the baudrate on the uart where the built in Bluetooth is ?
```

---
## \#786 Posted by: ThomasL Posted at: 2019-04-11T12:51:42.542Z Reads: 174

```
Happens as well with the R-Specs hubs
```

---
## \#788 Posted by: Pantata Posted at: 2019-04-11T13:20:17.399Z Reads: 172

```
METR supports unity as far as I know. That app is awesome.
```

---
## \#789 Posted by: PickSix24 Posted at: 2019-04-11T13:39:12.120Z Reads: 179

```
I need a second uart. My remote is on the first and I’d like to use the second for something else. 
There’s custom firmware to do this, just wondering this would be in the latest release @Deodand
```

---
## \#790 Posted by: drone001 Posted at: 2019-04-12T00:56:11.040Z Reads: 178

```
I'm new to this so be kind......i'm building a 12s6p with 6374's 190Kv can someone please give me the scoop on this connectors and wire size business. all of my research says it's a matter of preference.
```

---
## \#791 Posted by: venom121212 Posted at: 2019-04-12T01:06:51.185Z Reads: 180

```
Is this related to the unity specifically or just in general?
```

---
## \#792 Posted by: drone001 Posted at: 2019-04-12T01:09:06.168Z Reads: 184

```
both...primarily the Unity since I own one now.
```

---
## \#793 Posted by: venom121212 Posted at: 2019-04-12T01:18:37.039Z Reads: 185

```
Shoot me a pm with a link to the motors and battery you are using and I'll get you sorted out
```

---
## \#794 Posted by: Ashintar Posted at: 2019-04-12T22:45:53.734Z Reads: 187

```
I've been having an issue where when I go to start Accel the motors attempt to go the other direction then the controller disconnects and i have to hard reset everything to get back running again. This seems super scary considering I like to ride down a lot of hills. I'll try to remember to capture the fault of there is one just curious if anyone else has has a similarl issue
```

---
## \#795 Posted by: drangboards Posted at: 2019-04-13T01:15:39.929Z Reads: 191

```
I have a strange power cut issue on the raptor 2.1.1  Under high throttle conditions, and when I hit bumps, power cuts off.  I do have 1 hot motor lead wire, I believe this is the issue...  We'll see.

The other issue which cropped up last night is the board won't turn off.  I didn't get it wet inside at all.  I charged it overnight and now the power won't shut off.  I replaced the switch and the problem persists.  Even if I unplug the switch, the power comes on as soon as a the bat cables are plugged in.  Where to look for issues? 

This is my daily driver AKA no car, so it's dire.
```

---
## \#796 Posted by: BigZwatt Posted at: 2019-04-13T03:19:51.595Z Reads: 185

```
Hey all I have a diyeboard 10s5p battery. Keda 190kv 6364 2000w 90a max motors.  Im running 36t/16t wheel/motor pulleys . what settings would optomize my setup woth the unity ? Thanks in advance
```

---
## \#797 Posted by: huntercasillas Posted at: 2019-04-13T03:59:08.188Z Reads: 177

```
Can you use the reverse as the break (like the boosted does) with a PPM remote on the unity?
```

---
## \#798 Posted by: BigZwatt Posted at: 2019-04-13T04:33:12.451Z Reads: 180

```
Theres a setting in remote config. You can swap between accel./ reverse accel/brake
```

---
## \#799 Posted by: accrobrandon Posted at: 2019-04-13T05:15:37.265Z Reads: 178

```
Sure...

Motor min/max 60 ... If u really wanted more u could inch toward 90... But youd need a way better battery anyways...

Battery max then min... 50/ 20.... 
I think these are decent values given the battery
```

---
## \#800 Posted by: BigZwatt Posted at: 2019-04-13T05:52:35.577Z Reads: 175

```
Thank you what abour brake regen and braking current??
```

---
## \#801 Posted by: huntercasillas Posted at: 2019-04-13T07:23:00.396Z Reads: 177

```
What type of connector does the unity switch use? These? @CarlCollins 

ACTOO JST SM 5 Pin Connector LED Power Male to Female SM Wire Cable Adapter for 3528 5050 LED Light Strip 10 Pair https://www.amazon.com/dp/B07GGJGB7Q/ref=cm_sw_r_cp_api_i_IAzSCb4932HDP
```

---
## \#802 Posted by: accrobrandon Posted at: 2019-04-13T13:54:47.004Z Reads: 177

```
That's the 20
```

---
## \#803 Posted by: CarlCollins Posted at: 2019-04-13T16:05:41.135Z Reads: 178

```
@Deodand I am little unsure, can you please enlight us? :slight_smile:
```

---
## \#804 Posted by: Deodand Posted at: 2019-04-13T16:09:02.356Z Reads: 179

```
Yes all vertical white plastic connectors are jst-ph 2mm pitch except for the 3-pin PPM (remote) connector which is jst-xh 2.5mm pitch.
```

---
## \#805 Posted by: accrobrandon Posted at: 2019-04-13T16:56:40.471Z Reads: 180

```
if i have any feedback on unity construction is would be to make the wiring longer for the switch. its kinda short once attached to a case.
```

---
## \#806 Posted by: Niall Posted at: 2019-04-13T17:14:04.856Z Reads: 184

```
Have there been any delivery issues with these. I ordered mine but given the long lead times with supply i have cancelled and now am awaitimg refund .
```

---
## \#807 Posted by: CarlCollins Posted at: 2019-04-13T20:17:55.218Z Reads: 189

```
We have refunded your order as I told you that I am going to refund it 100% even if you are out of the initial 7 days safe zone and also you told us that our T & C doesn't have any legal standings.
You are not being funny but it's kinda funny and ignorant as well :slight_smile: 

Also, I have even offered you that we will ship it by the end of May and you will get it before the Mid of June as you said If it's possible but even though you keep denying it.
You don't even try to confirm with our live support before ordering but still as a gesture of goodwill, try to work this out so you can keep your order and have the product.

Let me clear one thing for sure, Every E-commerce system/online sales platform has a Terms and conditions which have legal standings and it's mandatory to follow it when you do purchase from their website. In your case, you have agreed to that terms and conditions at the time of order placement already so you are not able to deny it. (If required, I will share the screenshot to prove this point).

Have a good day
```

---
## \#808 Posted by: Niall Posted at: 2019-04-13T21:32:54.653Z Reads: 180

```
Cheers Carl looking forward to getting this back in my account
```

---
## \#809 Posted by: jbruce Posted at: 2019-04-14T03:23:16.564Z Reads: 179

```
@Deodand is there a feature like in the ackmaniac firmware where reverse works but only after releasing the break and pulling back again? This makes breaking much easier but still allows for reversing.
```

---
## \#810 Posted by: Farklinsburg Posted at: 2019-04-14T05:03:24.327Z Reads: 181

```
@Deodand I have also been trying to fault find the issue of one motor stuttering and cutting out on full acceleration for almost a month now. Dual SK8 6374 192kv.
Any news on when we might see a fix released?
```

---
## \#811 Posted by: mackann Posted at: 2019-04-14T05:22:48.555Z Reads: 178

```
It was released yesterday
```

---
## \#812 Posted by: rey8801 Posted at: 2019-04-14T05:24:35.484Z Reads: 186

```
@Deodand I tried to find an answer myself to don't give you another question to answer. Basically I would like to know if and when you will release a telemetry app for Unity. Probably by using the internal module. I think this aspect will really make Unity outstanding compare to all the other VESC for being complete. Thank you very much.
```

---
## \#813 Posted by: mackann Posted at: 2019-04-14T05:27:14.868Z Reads: 185

```
I think they are and if I remember right for iphone @sofu is already building the app for enertion.
Not 100% but Im almost sure I read it somewhere
```

---
## \#814 Posted by: sofu Posted at: 2019-04-14T05:38:03.468Z Reads: 184

```
That's correct!
```

---
## \#815 Posted by: Farklinsburg Posted at: 2019-04-14T05:42:14.445Z Reads: 183

```
@mackann thanks for the info. The changelog on the Android app still shows 23.42 as the latest. Could you share a link for the latest release.
```

---
## \#816 Posted by: Deodand Posted at: 2019-04-14T06:07:28.045Z Reads: 183

```
Release live tomorrow adding a few little things last minute because I was feeling inspired today :)
```

---
## \#817 Posted by: mackann Posted at: 2019-04-14T06:10:16.188Z Reads: 182

```
It still have the fix for your motor in it, try update it
```

---
## \#818 Posted by: Farklinsburg Posted at: 2019-04-14T06:10:41.067Z Reads: 180

```
Awsome. Thanks for the response and thanks for the great work.
```

---
## \#819 Posted by: Farklinsburg Posted at: 2019-04-14T06:19:51.663Z Reads: 181

```
@mackann yeah i have been running 23.42 and still having the same issues. Also tried to increase  FOC/Hall sensors/Sensorless ERPM to 4500 as previously suggested and getting the same behaviour. All wiring checked, resistance checks of motor windings and also confirmed braking behaviour with short applied to all combinations of phase wires.
```

---
## \#820 Posted by: rey8801 Posted at: 2019-04-14T06:39:42.248Z Reads: 179

```
Ah ok cool! Good luck with it! 
What about Android? Is @Deodand do that part or someone else? Do you when a beta app? I really need it :sweat_smile:
@mackann thanks for let me know about it.
```

---
## \#821 Posted by: mackann Posted at: 2019-04-14T07:37:27.161Z Reads: 178

```
In the url there is a 23.43 firmware with a fix for it
```

---
## \#822 Posted by: drangboards Posted at: 2019-04-14T07:39:57.775Z Reads: 178

```
Unity in raptor 2.1 won’t power down. Momentary switch has been replaced. Any ideas?
```

---
## \#823 Posted by: murloc992 Posted at: 2019-04-14T10:35:08.050Z Reads: 179

```
By the way, guys who have platinum warranty and guys who like their lives: check how well your motor wires are soldered..

![54|690x388](upload://y4yYA9m11n7Fze9sP2XY9MYjF4f.jpeg) 

These two just popped off (can literally see the square shape of the pad) without much heating necessary and were floating above. 2/6 cold solder joints that could probably break away with vibrations..

The square corner on the right cable is all that held it on the pad.
```

---
## \#824 Posted by: taz Posted at: 2019-04-14T11:29:17.072Z Reads: 177

```
This is completely unacceptable.

Enertion should make the factory sort it out and until then change that idiotic warranty clause.
```

---
## \#825 Posted by: Deodand Posted at: 2019-04-14T15:17:43.787Z Reads: 176

```
Thanks for the heads up @murloc992 we will forward these images to the factory and have them apply a bit more heat/flux. 
 

[quote="taz, post:824, topic:77861"]
idiotic warranty clause
[/quote]

There's nothing idiotic about discouraging our potentially inexperienced customer from bringing hot molten lead near a densly populated circuit board and guaranteeing any mistakes they make, our company will cover financially.
```

---
## \#826 Posted by: taz Posted at: 2019-04-14T15:31:38.740Z Reads: 175

```
As far as the wires on the pcb go, I will agree with you.

However, not properly soldered connectors  have been exhibited in multiple occasions in Unities as they come from the factory.

I am really interested to hear how exchanging them or making sure they are properly soldered (which would require the removal of the heat shrink) could damage an esc and be the reason for the warranty to become void.

Escs have been produced a long time before the focboxes and most of them did not even come with connectors.
```

---
## \#827 Posted by: murloc992 Posted at: 2019-04-14T17:02:03.864Z Reads: 179

```
I mean, the motor wires can be accessed only by removing the orange shield and by cutting the heatshrink, no chance of reaching PCB components @Deodand . 

That's all I did, mainly was interested after I saw the cold-soldered bullet photo, but what I saw - matte gray joints with two wires dangling by a thread didn't really boost confidence in the product. Gladly, it's an easy fix to anybody who has a soldering iron, some solder and flux if needed.

In fact three wires were like that:

![00|690x388](upload://kQnBDAhI0CmvVMisuqfHKhCXCjU.jpeg) 

From left: 2,3,5. Especially 3.

I did not take photos after cutting the shrinks sadly, as I did resoldering instantly after seeing what was up.

Disclaimer: I have platinum warranty and work with electronics every day so no risk tbh.
```

---
## \#828 Posted by: jbruce Posted at: 2019-04-14T17:45:05.267Z Reads: 178

```
Hey guys, I just recently updated the firmware on the unity to the latest one using the windows program and now I’m having some problems. When I press the on button, the light on the switch doesn’t go on but the lights on the unity turn on for about 5 seconds and then turn off. If i hold the on button down the unity will stay on but wont be able to connect to a computer or phone through Bluetooth. In the computer program it says "serial port error: the semaphore timeout has expired" When I try to connect through a phone it says "cannot read version firmware" Has anyone else had this problem? I’m not sure what happening or how to remedy and would love some help.
```

---
## \#829 Posted by: Deodand Posted at: 2019-04-14T17:51:07.380Z Reads: 179

```
The bullets/wires are actually ordered pre-assembled separately and then our factory solders them on. So interestingly it's two separate issues there to solve. 

It is disappointing to not see a nice wet solder joint though thanks for the image.
```

---
## \#830 Posted by: Meeep Posted at: 2019-04-14T18:29:13.079Z Reads: 181

```
This is not urgent at all but I sent back my Unity to @barajabali as per Enertion support for a replacement/fix. They said they will be shipping a unit from China when available. Should I interpret "when available" as when batch 3 goes out or do customer support requests get some priority? I can't ride for a while so it doesn't really matter to me but I thought I'd ask here to keep the support line uncluttered. Thank you Enertion team, I hope to test and enjoy your product soon.
```

---
## \#831 Posted by: Deodand Posted at: 2019-04-15T00:18:45.323Z Reads: 181

```
Hey guys, the new release of the UI/tool is live

[Windows UI Download](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_UI.zip)

[Windows Tool Download](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_TOOL.zip)

[Android](https://play.google.com/store/apps/details?id=enertion.focbox.ui&hl=en_US)

I am working on an offical mac release would should be live in a few days :smile: that's how slow this old mac is.

Main additions are better motor ID, better BLE stability, traction control, remote CAN shutdown, and some added config settings for ramping times and traction control in the advanced settings menu for the remote.
```

---
## \#832 Posted by: epss4 Posted at: 2019-04-15T00:40:13.010Z Reads: 182

```
Nice thanks !!!
Does this update fix the cutout problem??
```

---
## \#833 Posted by: Deodand Posted at: 2019-04-15T01:28:11.032Z Reads: 181

```
Yes adjustments to the motor detection should fix that issue.
```

---
## \#834 Posted by: sofu Posted at: 2019-04-15T02:38:13.326Z Reads: 180

```
Somebody else is working on the new Android app. I don't have a beta for external right now but maybe soon...
```

---
## \#835 Posted by: rey8801 Posted at: 2019-04-15T04:22:06.361Z Reads: 179

```
Yeh don't have iphone anyway. Mean time ordered metr module. We'll see it
```

---
## \#836 Posted by: Gerrycorrado Posted at: 2019-04-15T13:40:51.103Z Reads: 176

```
[quote="Deodand, post:831, topic:77861, full:true"]
Hey guys, the new release of the UI/tool is live

[Windows UI Download](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_UI.zip)

[Windows Tool Download](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_TOOL.zip)

[Android](https://play.google.com/store/apps/details?id=enertion.focbox.ui&hl=en_US)

I am working on an offical mac release would should be live in a few days :smile: that's how slow this old mac is.

Main additions are better motor ID, better BLE stability, traction control, remote CAN shutdown, and some added config settings for ramping times and traction control in the advanced settings menu for the remote.
[/quote]

So I noticed the unity android app updates itself automatically (good). Now, I suppose the firmware update towards the Unity is to be done manually? And this with "included firmware" selected? (I always got confused with that one, but looking that the app updated itself, it seems logical that it is the included in the latest app upgrade.)
Then I have to do this as I only did it at first connection. What is funny is that when I connect my phone, it doesnt say anything special. When I connect my buddy his phone (with the app installed lets say 2 weeks after me, for a group ride he would use my board), his phone says the unity runs old software.
```

---
## \#837 Posted by: rey8801 Posted at: 2019-04-15T13:42:20.449Z Reads: 164

```
when you open the app and connect the unity you should get the message that you are using the old firmware. Then go to firmware window and simple press update. 23.43 last update. Did it this morning
```

---
## \#838 Posted by: Gerrycorrado Posted at: 2019-04-15T13:43:45.513Z Reads: 167

```
Well that is not the case for my phone, it was for my buddy. Tested at the Wavre karting event and the day before (as he never ridden before, I dropped of all my stuff bar my phone, so he had to install it to know the batt % as I have no display built in)
```

---
## \#839 Posted by: rey8801 Posted at: 2019-04-15T13:44:35.453Z Reads: 168

```
just check that you are using 23.43 firmware. if not than update the app from google play and try again.
![IMG_20190415_154611|300x500](upload://xxQQU85MAIGYQmeXzv7eYyZfZrS.jpeg)
```

---
## \#840 Posted by: Gerrycorrado Posted at: 2019-04-15T13:46:53.044Z Reads: 161

```
Tja Rey, as I never did the manual firmware flash except when I unpacked the thing a month ago, I guess not :blush: 
Aha, I just remember I have the board with me haha, walking to my car now
```

---
## \#841 Posted by: rey8801 Posted at: 2019-04-15T13:47:28.224Z Reads: 160

```
you always have to do it manually. The app tells you but then flashing it's on your own. If you do it through bluetooth put the phone always awake otherwise the uploading stops while phone locks itself. At least mine does that.
```

---
## \#842 Posted by: venom121212 Posted at: 2019-04-15T13:51:03.581Z Reads: 164

```
:arrow_up: This

Also spin your wheels every few minutes to keep the unity from timing out!

(or just change timeout time, my update took ~10 minutes)
```

---
## \#843 Posted by: rey8801 Posted at: 2019-04-15T13:51:35.087Z Reads: 162

```
i just press the bottom fast once in a while. It also works. Didn't think about the wheels. Thanks
```

---
## \#844 Posted by: rsalmon Posted at: 2019-04-15T14:04:50.704Z Reads: 160

```
@Deodand, my issues seem to be completely fixed with the new firmware. No stutters on my sensorless motors, even with just a tiny push. Hard accelerations also behaving predictably.

Thank you very much for your hard work. And yours too @Blasto.
```

---
## \#845 Posted by: Deodand Posted at: 2019-04-15T16:00:01.791Z Reads: 160

```
Great to hear your stuttering is fixed, thanks for the feedback. 

@venom121212 the latest FW now refreshes the off timer during FW flash so this will be the last update where it's possible for it to autoshutoff (it shouldn't corrupt even if it does but will cancel update). Now to make it keep the phone screen on when pushing FW as well haha. Thought of that last minute and it was more involved than expected since the app isn't native.
```

---
## \#846 Posted by: drone001 Posted at: 2019-04-15T17:06:09.433Z Reads: 163

```
Ok now I'm worried...i see a lot of people complain about bad solder jobs. I have not checked my connections yet. I'm new so I'm worried about failing to identify a bad solder joint......although my skills have improved to finally finish my bullet connectors....I'm still worried![20190414_153338|375x500](upload://qS4jwTxrl07BYy9qIhcUPrILN6U.jpeg)
```

---
## \#847 Posted by: murloc992 Posted at: 2019-04-15T17:09:13.789Z Reads: 163

```
If you have the platinum warranty and feel adventurous, cut the heatshrinks carefully and look if the solder joints are fully covered and shiny. You don't want anything matte, grey and crumbly especially.

Best part, you can re-shrink them if everything looks good.

I see that you step up the connectors through adapters. If you really feel brave, step up the wires to 12AWG and put your connectors on them. :slight_smile:
```

---
## \#848 Posted by: murloc992 Posted at: 2019-04-15T17:14:51.428Z Reads: 162

```
@Deodand

By the way, the cold solders, etc were from the special edition. It's a first batch unity. So I guess subsequent batches might be fine?
```

---
## \#849 Posted by: Sn4pz Posted at: 2019-04-15T17:19:07.826Z Reads: 159

```
I would love to know what the number of cold solder joints were on a larger scale. Especially from someone who sold Unities, and redid the connections (ahem @Jlabs ;) ) but I dont want them to get in trouble with Enertion... :Joy:
```

---
## \#850 Posted by: murloc992 Posted at: 2019-04-15T17:20:08.722Z Reads: 158

```
I think you forgot @mackann too. :smiley:
```

---
## \#851 Posted by: Sn4pz Posted at: 2019-04-15T17:20:31.268Z Reads: 159

```
Good point!
```

---
## \#852 Posted by: JLabs Posted at: 2019-04-15T17:24:30.812Z Reads: 169

```
On the legacy focbox I’d say cold solder joints were around 30-40% (based on the shear number of connectors I changed). 

I probably only swapped connectors on 10 Unity’s and maybe only found one cold solder joint out of 60. Pretty good IMO. 

Entertain said their resellers can change the connections and not void warranty.
```

---
## \#853 Posted by: Sn4pz Posted at: 2019-04-15T17:25:12.608Z Reads: 168

```
[quote="JLabs, post:852, topic:77861"]
Entertain said their resellers can change the connections and not void warranty.
[/quote]


Hot Diggity thats cool. I wasnt aware of that

knowing my luck I was the one bastard with a cold solder joint on their Unity :joy:
```

---
## \#854 Posted by: murloc992 Posted at: 2019-04-15T17:25:43.709Z Reads: 168

```
They assume resellers know what a soldering iron is! :open_mouth:
```

---
## \#855 Posted by: drone001 Posted at: 2019-04-15T17:27:42.922Z Reads: 173

```
thx.....I don't know why I'm so chicken shyt when it comes to soldering. I have NOO faith in my skills. Think i will practice with some 12AWG wire first. maybe get one of those solder practice kits or something. lol
```

---
## \#856 Posted by: murloc992 Posted at: 2019-04-15T17:27:47.559Z Reads: 175

```
[quote="Sn4pz, post:853, topic:77861"]
knowing my luck I was the one bastard with a cold solder joint on their Unity :joy:
[/quote]

May I introduce to you: my friend, _special edition™_  first batch Unity? :joy:

 ![37|690x388](upload://ac1u5TvuQ37VDHOzhNc8KmOQehq.jpeg) 

![32|690x388](upload://uJWTUoWEwWHzz4A9DUy2N1CITxO.jpeg) 

Reversed connector AND cold solder joints.

Fite my luck IRL.
```

---
## \#857 Posted by: murloc992 Posted at: 2019-04-15T17:28:36.873Z Reads: 165

```
[quote="drone001, post:855, topic:77861, full:true"]
thx…I don’t know why I’m so chicken shyt when it comes to soldering. I have NOO faith in my skills. Think i will practice with some 12AWG wire first. maybe get one of those solder practice kits or something. lol
[/quote]

Get some AMTech flux. It does WONDERS.
```

---
## \#858 Posted by: drone001 Posted at: 2019-04-15T17:31:55.042Z Reads: 164

```
thx. just swapped my solder to Kester and what a difference it made. I was using some cheap solder before....ruined 3 sets of bullet connectors. I have flux but again...it's the cheap stuff. checking out this AMtech now. thx again.
```

---
## \#859 Posted by: murloc992 Posted at: 2019-04-15T17:33:03.500Z Reads: 163

```
I am from Europe so I cannot really recommend "international" solder, but I go with some polish unleaded(the full composition is rubbed off :( ) and AMTech flux. Things solder beautifully. Even 10AWG wires.
```

---
## \#860 Posted by: Deodand Posted at: 2019-04-15T17:39:27.406Z Reads: 163

```
Good to hear @JLabs thanks for the feedback! Would be best to see that number be 0 but at least we are moving in the right direction.
```

---
## \#861 Posted by: murloc992 Posted at: 2019-04-15T17:40:37.485Z Reads: 165

```
@Deodand as we work with chinese manufacturing, they do "perfectly" only in first batches, then they tend to cut(time, mostly) on the quality. Let's hope it's the reverse in this case. :slight_smile:
```

---
## \#862 Posted by: Blasto Posted at: 2019-04-15T17:42:26.632Z Reads: 166

```
Those cables are directly from Amass, as they have the proper machines to automate the soldering. We'll still keep a close eye on this.
```

---
## \#863 Posted by: murloc992 Posted at: 2019-04-15T17:43:56.656Z Reads: 170

```
[quote="Blasto, post:862, topic:77861, full:true"]
Those cables are directly from Amass, as they have the proper machines to automate the soldering. We’ll still keep a close eye on this.
[/quote]

Everything can become "lazy", even machines. The main issue I guess are the motor wire solder pads. I literally had one I could have "persuaded" to come off but desoldered anyways, because what the frick. :smiley:
```

---
## \#864 Posted by: drone001 Posted at: 2019-04-15T17:53:18.034Z Reads: 167

```
My "oh no i can't ride" pains would have kicked in immediately.  Lol
```

---
## \#865 Posted by: murloc992 Posted at: 2019-04-15T17:53:46.947Z Reads: 172

```
[quote="drone001, post:864, topic:77861, full:true"]
My “oh no i can’t ride” pains would have kicked in immediately. Lol
[/quote]

Nothing one beer can't fix!

![08|690x388](upload://7XWovRp9ptUJ80krBcjZAr32098.jpeg)
```

---
## \#866 Posted by: drone001 Posted at: 2019-04-15T17:55:58.437Z Reads: 170

```
I wanna get that good as to not worry about things like a bad solder job. just grab a beer and heat up the soldering iron.
```

---
## \#867 Posted by: murloc992 Posted at: 2019-04-15T17:57:32.846Z Reads: 168

```
[quote="drone001, post:866, topic:77861"]
just grab a beer and heat up the soldering iron.
[/quote]

I'd rather check the situation first. Heatshrink is cheap anyways. :slight_smile:
```

---
## \#868 Posted by: drone001 Posted at: 2019-04-15T18:00:18.425Z Reads: 170

```
yeah...yeah..yeah. I'm feeling adventurous now.I'll check mine when i go home...I have shrink wrap...yeah yeah. i'm going for it. thx bruh.
```

---
## \#869 Posted by: venom121212 Posted at: 2019-04-16T18:39:39.739Z Reads: 175

```
Hey @Deodand can you tell me a bit more about how the throttle ramping times and traction control work? 

![Screenshot_20190416-143802|236x500](upload://ar9ewMk40L4MFxVgpDLR9Hymzk0.jpeg)

Very excited to try these out :smiley:
```

---
## \#870 Posted by: Jinra Posted at: 2019-04-16T18:45:21.745Z Reads: 174

```
I use .1/.1 ramping times. It's the amount of time (in seconds) it takes for the throttle to ramp from a given power output to another. Example, if you go from 25% throttle to 50% throttle it'll take .3 seconds (from your picture) to ramp from 25% power to 50% power on the VESC.

Traction control limits power to a wheel if the eRPM delta exceeds a given threshold (Traction CTRL Max eRPM difference on the app)
```

---
## \#871 Posted by: venom121212 Posted at: 2019-04-16T18:50:16.023Z Reads: 173

```
Ok that makes a lot of sense. Really I guess my confusion comes from how the throttle curve and ramp times affect each other.

I assumed that when increasing motor command, I was also increasing ramp time (especially when not linear and on the high end of throttle) . Thank you for the quick reply
```

---
## \#872 Posted by: Jinra Posted at: 2019-04-16T18:51:55.905Z Reads: 172

```
Throttle curves apply varying power depending on throttle position. I am a believer that linear is the best and most predictable curve myself. They both have a direct affect against throttle, but work a bit differently.
```

---
## \#873 Posted by: venom121212 Posted at: 2019-04-16T18:53:11.758Z Reads: 171

```
Thank you for confirming what I have always believed as well. Linear mapping of throttle input to output is most logical and having the acceleration separate is a really nice feature. I'm so excited to try this out!
```

---
## \#874 Posted by: Deodand Posted at: 2019-04-16T18:59:01.013Z Reads: 175

```
Something to clarify here also, ramp time is the time it takes to go from 0 percent throttle to 100 percent throttle. So let's say you move from 25 percent throttle to 50 percent it will only take 1/4 of your ramping time to complete the change. When using current control it sets a limit on the rate of change of acceleration (in physics this is referred to as jerk).

The throttle mapping is just an instantaneous transform from whatever current throttle position is to output command. So this remaps a position to a position where as ramp time is a pretty simple time based filter that prevents rapid changes in acceleration to make the boards behaviour more predictable.
```

---
## \#875 Posted by: rey8801 Posted at: 2019-04-16T19:51:40.727Z Reads: 171

```
So a bit longer ramping time will also help to stop the kick back you get if you release the throttle after decent acceleration since it will smooth down the deceleration curve as well.  Is it right?
```

---
## \#876 Posted by: Mudders Posted at: 2019-04-16T19:53:12.909Z Reads: 172

```
Noob question, i have searched but i think i must be using the wrong terms.

I have updated firmware and gone through the setup ui again.

I'm using a mini remote, when i switch off the remote to simulate signal loss the board goes full throttle, how can i reset the failsafe? I have rebound the remote but no change :confused:
```

---
## \#877 Posted by: FredXanadu Posted at: 2019-04-16T19:53:30.128Z Reads: 167

```
thanks for the OS version :slight_smile:
```

---
## \#878 Posted by: Jinra Posted at: 2019-04-16T19:55:25.730Z Reads: 165

```
I don't think so, neutral throttle would just mean no power delivery to motors
```

---
## \#879 Posted by: rey8801 Posted at: 2019-04-16T19:59:41.190Z Reads: 167

```
Yep but I am talking about when you release the throttle from closer to 100% without braking. In this case I get like a step and not a smooth deceleration. Maybe increase the ramping time affects also that aspect
```

---
## \#880 Posted by: Jinra Posted at: 2019-04-16T20:00:36.977Z Reads: 163

```
I understand, but what you're implying is that it would continue to provide power to the motors at a descending rate, for the given ramping time. I believe it just completely cuts off power once you return to neutral, it's instantaneous. Correct me if I'm wrong @Deodand
```

---
## \#881 Posted by: rey8801 Posted at: 2019-04-16T20:02:20.729Z Reads: 153

```
True. Or maybe takes the 0.3sec imposed but still really fast. Thst behaviour was better with vesc 6 based VESC. Maybe they have diffent way to handle it. For the moment I accommodate the descenting phase and it's ok.
```

---
## \#882 Posted by: Mudders Posted at: 2019-04-16T20:05:37.851Z Reads: 160

```
Sorted, and panic mode off...
```

---
## \#883 Posted by: ninTHIENdo Posted at: 2019-04-16T20:15:51.489Z Reads: 161

```
Stuttering issue fixed on the new firmware, it’s amazing and thank you! had a cutoff issue once that I hadn’t been able to reproduce, and not sure if I can. 124.6 miles on the new firmware so far, on 8 inch pneumatics, 60/-30 bat, 70/-70 motor dual 6374 190kv motors on. 1:4 gear drive.
```

---
## \#884 Posted by: ninTHIENdo Posted at: 2019-04-16T20:19:28.823Z Reads: 160

```
I just bring my thumb slowly back while on the wheel to prevent the kickback. Hardly ever just fully let go of the wheel, that little kick freaks me out every time...
```

---
## \#885 Posted by: rey8801 Posted at: 2019-04-16T20:27:18.353Z Reads: 162

```
I do the same. I thought maybe it can be improved.
```

---
## \#886 Posted by: Deodand Posted at: 2019-04-16T20:30:30.414Z Reads: 171

```
@rey8801  you are correct that increasing the downward ramp time would slow the descending acceleration. @Jinra it does actually take that amount of time to return to 0. This is definitely scary (we all want responsive brakes) and a good reason not to turn the value up very high.  I don't recommend turning up this value to address that issue. 

Vedder's latest FW has a fix where if the throttle position is 0 or greater the larger of the two ramping times is always used. So essentially if you let off the throttle suddenly but not all the way it eases down the acceleration providing that forward lurch. But if you go into braking it allows the brakes to be applied suddenly.... kind of a middle ground. Not really sure if I'm in love with that idea but maybe I'll give it a test run and put it in the next release if it feels nice.
```

---
## \#887 Posted by: rey8801 Posted at: 2019-04-16T20:33:22.903Z Reads: 168

```
Thabk you for the super clear explanation and Vedder's solution seems actually good. Of course your the decision. You are doing great so I trust you. Thank you again
```

---
## \#888 Posted by: Deodand Posted at: 2019-04-16T20:35:53.883Z Reads: 172

```
Yea, it's interesting for sure. I do hate that feeling when my thumb slips off the throttle. I'll test it today maybe and see how it feels. Just worried it might feel unpredictably sudden once you do hit the brakes, we will see.
```

---
## \#889 Posted by: jbruce Posted at: 2019-04-16T20:48:49.777Z Reads: 178

```
quick question: if i set max battery amps to 40A does that mean 40A per motor and max amps will actually be 80A or is the 40A max the max for both motors? I'm curious because i set it to 40 but now under full load my voltage sag is much greater than when i had it set to 40 with a different vesc. This makes me think it might actually be pulling 80A.
```

---
## \#890 Posted by: Deodand Posted at: 2019-04-16T20:50:11.703Z Reads: 177

```
No it's 40 amps total as you expect. Regarding sag make sure your pack is in good health.
```

---
## \#891 Posted by: rey8801 Posted at: 2019-04-16T20:53:13.284Z Reads: 176

```
I think that if it's possible to discriminate when the brakes are not involved as you said it's a promising feature.
```

---
## \#892 Posted by: murloc992 Posted at: 2019-04-16T20:54:33.197Z Reads: 181

```
Make this throttle->idle thingie into a checkbox in the app if possible? :slight_smile: That way people chan choose what they like more.
```

---
## \#893 Posted by: mackann Posted at: 2019-04-17T19:47:24.708Z Reads: 177

```
@Deodand Can confirm that the new firmware fixed the Unity I did have over current cut out with on full throttle. Got a crazy friend to go full throttle a few times from stand still and no cut out on the same board. 👍 Thanks!
```

---
## \#894 Posted by: rey8801 Posted at: 2019-04-17T19:54:33.270Z Reads: 179

```
@mackann definetely the final tester for madness...if it works for him we are all safe :smile:
```

---
## \#895 Posted by: mackann Posted at: 2019-04-17T21:00:16.003Z Reads: 180

```
Today @rpasichnyk was visiting our workshop and fixed so you can now run metr app to do motor setup/wizard! Nice if you dont want to jump between the 2 apps or use iPhone!
```

---
## \#896 Posted by: rey8801 Posted at: 2019-04-17T21:12:23.392Z Reads: 180

```
Does it mean that you got the module to replace the internal unity Bluetooth module? Or what?
```

---
## \#897 Posted by: mackann Posted at: 2019-04-17T21:17:38.244Z Reads: 181

```
In a few weeks i think it will come. The motor setup works with the normal metr on Unity now
```

---
## \#898 Posted by: rey8801 Posted at: 2019-04-17T21:19:47.766Z Reads: 180

```
Damn I just bought 2 days ago 2 metr pro :sweat_smile:
Do you know how to use metr with the internal UART port?
```

---
## \#899 Posted by: Ian-mountainboard Posted at: 2019-04-18T11:36:03.059Z Reads: 183

```
Does it matter which phase wires i plug into my motor?
```

---
## \#900 Posted by: murloc992 Posted at: 2019-04-18T11:36:35.469Z Reads: 184

```
As long as all three are from the same motor you're fine.
```

---
## \#901 Posted by: Ian-mountainboard Posted at: 2019-04-18T12:06:53.192Z Reads: 180

```
Cant u get cogging if the wrong ones r connected?
```

---
## \#902 Posted by: McErono Posted at: 2019-04-18T12:36:04.176Z Reads: 184

```
No the motor will just run in reverse, then you can change any two wires to solve that.

Question, lets say the Hall sensor detection test does pass in focbox tool on some Torqueboards DD motors but the sensor table is just filled with 200 and 255 values and focbox UI does not recognize any sensors. Any ideas what might be the cause? checked sensor adapter cables etc. both motors are exactly the same.
```

---
## \#903 Posted by: JohnnyMeduse Posted at: 2019-04-18T13:10:04.009Z Reads: 182

```
Play with the direction of the motor to see if it is working. I’ve seen some motor with sensor issue that will work in one direction and not the other. You could also try to swap the motor, to see if it is a motor or focbox issue
```

---
## \#904 Posted by: Deodand Posted at: 2019-04-18T16:45:05.318Z Reads: 176

```
Screenshot of the config would help.
```

---
## \#905 Posted by: McErono Posted at: 2019-04-18T17:20:13.727Z Reads: 179

```
First I did just the wizard on focbox ui on my mobile. all good but the sensors. So I tried focbox tool over usb and did the foc hallsensor detection, it passed but as I said the values in the sensor table are invalid. 

Would really apprechiate a TCP bridge or native BT connection with windows on the tool. Its a pita to open the enclosure all the time. And an odometer and stuff would also be welcome but I am sure this is on your radar already.

I will try to switch the motor cables and will take some screenies at the same time.
```

---
## \#906 Posted by: Deodand Posted at: 2019-04-18T17:23:46.380Z Reads: 177

```
If they are all reading 200 it just means all the halls are staying in a single state. That should be counted as a fail. My guess would be your halls are not electrically connected (maybe disconnected 5V or GND) somewhere along the line whether internal to motor or in one of the crimps/interconnects.
```

---
## \#907 Posted by: McErono Posted at: 2019-04-18T17:45:41.528Z Reads: 177

```
They are reading 255 and one of them (on each motor) 200.
```

---
## \#908 Posted by: JohnnyMeduse Posted at: 2019-04-18T17:52:08.544Z Reads: 178

```
Can you post some picture of you setup, also do you use adapter between your motor and the Unity for your sensor?
```

---
## \#909 Posted by: McErono Posted at: 2019-04-18T17:56:51.508Z Reads: 185

```
I will. Yes I use adapter cables and first thing I will try is to use the original torqueboards adapters. At the moment I use these https://shop.elektro-skateboard.de/eigenbau-tuning/zubehoer/727/hall-sensor-adapterkabel-fuer-vesc?number=ESK8B10725

Its not my first board and I had no issues with 6374 motors and 2x vesc but these direct drive sensors in combination with the unity just wont work.
```

---
## \#910 Posted by: JohnnyMeduse Posted at: 2019-04-18T18:00:26.879Z Reads: 185

```
If you test with other motor on the unity, it could help us find out if the problem is from the drive or the unity.
```

---
## \#911 Posted by: McErono Posted at: 2019-04-18T18:03:26.184Z Reads: 188

```
Thank you Johnny! I will switch motor cables, then use different adapter cables and if nothing helps I will try the unity on the 6374 motors.
```

---
## \#912 Posted by: Deodand Posted at: 2019-04-18T18:05:45.338Z Reads: 186

```
Just focus on the sensor wires. Chances are there is something amiss there. Those tiny 1.5mm pitch connectors that the adapters use can easily get damaged/be broken on arrival.
```

---
## \#913 Posted by: McErono Posted at: 2019-04-18T18:42:10.118Z Reads: 177

```
I have 6 adapters. Will report back, thanks guys.
```

---
## \#914 Posted by: JohnnyMeduse Posted at: 2019-04-18T18:46:00.920Z Reads: 178

```
Isshhh will be better if could test with 8 😬😜😜😜
```

---
## \#915 Posted by: McErono Posted at: 2019-04-18T20:09:08.788Z Reads: 191

```
Solved! Guess what:

![Screenshot_20190418-215819|243x500](upload://jpLAp6uiZBYaK1DH4Uv4KkBWTIo.jpeg) 

Torqueboards adapter
![20190418_215203|375x500](upload://t2A60BWPpfvbcEvoVxGsxO4GX04.jpeg) 

Elektro-skateboard adapter
![20190418_215237|375x500](upload://mpn48xOHyv7r6wYcOz8IoTWxAMv.jpeg) 

Are there different hall sensor pin layouts or did the german guys just f*** up?
```

---
## \#916 Posted by: Deodand Posted at: 2019-04-18T20:22:00.508Z Reads: 188

```
Depends what is going on under that shrink wrap.
```

---
## \#917 Posted by: McErono Posted at: 2019-04-18T20:35:24.530Z Reads: 192

```
They are on the plug like that. Im going to pull out that soldering iron and switch the orange and yellow wire so I don't have to deal with these tiny pins.
```

---
## \#918 Posted by: drone001 Posted at: 2019-04-18T21:35:48.552Z Reads: 190

```
i got 3 of those about 2 weeks ago. I first tried to plug them in but could not find my glasses so i figured i'd try later after i found my glasses. I'm going home to check them out.
```

---
## \#919 Posted by: RobPBody Posted at: 2019-04-18T22:37:35.944Z Reads: 197

```
@Deodand I took a video of something with my Unity. One of the motor flashes a negative voltage constantly. At first I thought it was my motor, but today I flashed the new firmware with just the Unity connected to the battery. Not covered to the remote receiver either. Just want to know this won't be a problem when I ride my build.

https://youtu.be/qQuLSQq9PKs
```

---
## \#920 Posted by: Deodand Posted at: 2019-04-18T22:40:00.633Z Reads: 190

```
No it's totally fine. It's just background noise from the sensor readings.
```

---
## \#921 Posted by: dcxeternal Posted at: 2019-04-18T22:47:46.485Z Reads: 199

```
Can someone direct me as to what kinda cable conversion I need to buy to convert the Meepo 5 pin hall sensor connection to the 6 pin the Unity takes? and which wire goes to which terminal please if there is an order.

Also does the 3 power wires have an order too?
Much thanks in advance!
![IMG_20190418_184511|375x500](upload://591g8RcECP6udNYv23WSMg7UPon.jpeg)
```

---
## \#922 Posted by: Jinra Posted at: 2019-04-18T23:03:12.255Z Reads: 200

```
If the meepo uses 6-pin JST-PH 2.0mm pitch headers then you're good to go, if not, I'd just cut/remove the header and solder on wires for the aforementioned header.
```

---
## \#923 Posted by: Deodand Posted at: 2019-04-18T23:05:15.054Z Reads: 201

```
Red and black go to 5v and ground respectively. The other 3 go to the H1-H3 ports the order doesn't matter as it will be detected during calibration. The same goes for the motor leads, the order does not matter.
```

---
## \#924 Posted by: dcxeternal Posted at: 2019-04-18T23:10:34.597Z Reads: 199

```
Thank you @Jinra and @Deodand
Now I know what 6pin to buy and the order to solder.
```

---
## \#925 Posted by: McErono Posted at: 2019-04-19T00:51:13.473Z Reads: 203

```
I realized its not just two wires wrong. Its also reversed or the plug upside down. Strange, they should know.

I think this is the right order. edit: yes now the adapters do work.

![20190419_025026|375x500](upload://npHU4n0KwX0RcPbfUYqsxVn1SwV.jpeg)
```

---
## \#926 Posted by: JohnnyMeduse Posted at: 2019-04-19T00:55:45.355Z Reads: 194

```
If I remember on certain type of vesc 6 derivative the sensor port is reverse. I think the "escape" is one of those.
```

---
## \#927 Posted by: McErono Posted at: 2019-04-19T01:04:06.426Z Reads: 198

```
Oh then that would make sense but they should not sell them as "Hall Sensor Adapter for VESC".
```

---
## \#928 Posted by: DroidSector Posted at: 2019-04-19T04:34:18.241Z Reads: 202

```
Just get 6-pin (or 3+3) connectors in a local shop, no soldering is required. I've also upgraded Meepo NLS with Unity, I guess it's NLS² now :)
```

---
## \#929 Posted by: MasterSpoon Posted at: 2019-04-19T11:13:59.627Z Reads: 204

```
@Deodand it was asked earlier in the this by @lemntl but I can't see where it has been answered

Does the Unity work with the AS5047 encoders ?

From what I can tell on V4 hardware you had to remove some input filters or change some components where V6 hardware the filtering was possibly done software side so worked without mod.

Being that the Unity is based on V4 hardware I'm guessing it won't work out of the box or have you been able to do some kind of magic trickery to have it work ?
```

---
## \#930 Posted by: taz Posted at: 2019-04-19T16:19:41.290Z Reads: 206

```
Does this mean that the temperature sensor on one of the motors is not working?

![Screenshot_20190419-184226|243x500](upload://rQsLCLKXqXCAMiVHWHKwzhvKA2y.jpeg)
```

---
## \#931 Posted by: Deodand Posted at: 2019-04-19T17:20:59.235Z Reads: 200

```
Yeah it's not reading.
```

---
## \#932 Posted by: taz Posted at: 2019-04-19T17:23:57.412Z Reads: 231

```
Thanks. Time to open the enclosure again :roll_eyes:
```

---
## \#933 Posted by: peteprez Posted at: 2019-04-19T22:47:51.525Z Reads: 232

```
Any word on iOS/iPhone app for the go box unity? I know “it’s coming” but where can I watch and wait to get it ASAP? Having to unscrew my enclosure just to tweak things is $&@#. Is there a place I can watch for updates? :slight_smile:
```

---
## \#934 Posted by: morrisxyz Posted at: 2019-04-20T00:10:25.944Z Reads: 234

```
[quote="sofu, post:58, topic:90882"]
Maybe mid June though…
[/quote]

@peteprez Send your bribes to @sofu.
```

---
## \#935 Posted by: sofu Posted at: 2019-04-20T02:35:49.959Z Reads: 234

```
1 billion dollars and I'll send you the current progress (which is not working yet :stuck_out_tongue:)
```

---
## \#936 Posted by: huntercasillas Posted at: 2019-04-20T02:59:04.671Z Reads: 233

```
If you need any help, let me know. I’m an iOS Developer 🤷🏻‍♂️
```

---
## \#937 Posted by: taz Posted at: 2019-04-20T06:41:00.710Z Reads: 230

```
Is there a cheap android smartwatch that can run the Unity app?
```

---
## \#938 Posted by: Ian-mountainboard Posted at: 2019-04-20T16:38:57.160Z Reads: 229

```
I know im late to this thread but do i need to have the power switch pluged into the unity. Then plug in my battery.
```

---
## \#939 Posted by: BigZwatt Posted at: 2019-04-20T20:02:04.839Z Reads: 229

```
Hey all,
Im having an issue. On of my. Motors seems to be kind of cogging but its dofferent than "normal" cogging. Also its not all the time. It happened all of a sudden. 
I screenshotted my config. I will upload a video as well 

![Screenshot_2019-04-20-14-55-16|250x500](upload://HDVen5LgROQoJGgoV6Lg6VNhfj.png)
```

---
## \#940 Posted by: Blasto Posted at: 2019-04-20T20:03:27.428Z Reads: 223

```
did you update you fw to 23.43 (lattest)? Sensorless runs smoother with the lattest.
```

---
## \#941 Posted by: BigZwatt Posted at: 2019-04-20T20:18:04.307Z Reads: 223

```
I did and it seemed better for a day or two and now on motor spins at speed and the pther one spins very slowly.  .
```

---
## \#942 Posted by: BigZwatt Posted at: 2019-04-20T21:13:19.513Z Reads: 224

```
_[Motor problems..](https://youtu.be/V8PVnqdwO-E)_
```

---
## \#943 Posted by: Blasto Posted at: 2019-04-20T21:17:30.734Z Reads: 224

```
You seem to be missing a phase, check you connections
```

---
## \#944 Posted by: Meeep Posted at: 2019-04-22T16:02:37.767Z Reads: 218

```
I just want to shout out @barajabali, @CarlCollins, @Deodand, and the Enertion CS team for fixing my situation. Excitedly setting it up now.
```

---
## \#945 Posted by: Chupacabra Posted at: 2019-04-23T15:46:48.310Z Reads: 223

```
Hi. I am facing an unusual situation that whenever I try to configure my Unity through the Unity Tool. Every time i am done updating the config and I turn the board off, when I turn it on it does not function. It seems that the unity forgets all motor config and starts behaving as if the motors have not been configures at all.

I am only using the tool because the Focbox UI does not have an option of controlling input dead band. That is set to 15% by default in the UI hence the need to use the tool. I have to go back to the UI to configure my motors. Has anyone faced a similar issue?

Another issue I'm having is that whenever I'm drawing telemetry from the UART from the unity, I am unable to update config. As soon as I turn off my feather remote , I am able to write the config.
```

---
## \#946 Posted by: Deodand Posted at: 2019-04-23T15:57:11.672Z Reads: 215

```
Have you reflashed firmware? It sounds like somehow your eeprom (non-volatile memory) isnt getting written correctly during the config write. What pwm freq are you running?
```

---
## \#947 Posted by: Chupacabra Posted at: 2019-04-23T17:49:53.796Z Reads: 209

```
Yes I have the latest firmware. The frequency is 915mhz.
```

---
## \#948 Posted by: Chupacabra Posted at: 2019-04-23T17:51:09.758Z Reads: 212

```
I had the same issue. I found that the issue was that my wires not connected all the way. A loose connection maybe the cause of stuttering.
```

---
## \#949 Posted by: BigZwatt Posted at: 2019-04-23T18:21:01.850Z Reads: 211

```
Ok thank you ill take it apart tonight. Did you see my motor detection screen shot? Could that be why the motor resistsnce is different as well.
```

---
## \#950 Posted by: Chupacabra Posted at: 2019-04-23T21:48:57.281Z Reads: 208

```
Yeah I suspect that might be the issue. Mine wasn't as pronounced as yours but I was getting stutters whenever i started from a complete stop.
```

---
## \#951 Posted by: CarlCollins Posted at: 2019-04-24T14:55:03.858Z Reads: 212

```
How are you flashing the firmware on the unit?
Using Bluetooth protocols or USB?
```

---
## \#952 Posted by: paulocruz1920 Posted at: 2019-04-24T16:51:18.594Z Reads: 222

```
Hi, 
I'm just starting to use FOCBOX UNITY and learn how to.
My goal is to be able to use both speed and torque control in a differential platform with two BLDC hoverboard motors.
I'm using (starting also) ROS to do that and I already found the vesc_drive ROS node and also managed to launch the node, but when i tried to publish the following: **rostopic pub -r 20 /commands/motor/speed -- std_msgs/Float64 3000** happened two things:

1. only one wheel responded;
2. that wheel just kept trembling (didn't spin);

Any of you have tried to do something in this area with FOCBOX UNITY or knows what's wrong ?

Thank you in advance!

![IMG_20190424_174611|666x500](upload://4EMLXMhENQlPcZ77DEZEbYVskKj.jpeg)
```

---
## \#953 Posted by: Deodand Posted at: 2019-04-24T16:54:24.608Z Reads: 210

```
The Ros msg is going to be setup for a standard vesc protocol and the unity is slightly different. You're going to want to look at commands.c in the source code to compare the differences, the main one being two values are sent instead of one.
```

---
## \#955 Posted by: Powadangaboards Posted at: 2019-04-25T12:42:46.804Z Reads: 205

```
This happened to me today.... very scary :/
```

---
## \#956 Posted by: mackann Posted at: 2019-04-25T12:44:21.389Z Reads: 202

```
Do you have the newest firmware? It was a fix for that in it.
```

---
## \#957 Posted by: Powadangaboards Posted at: 2019-04-25T12:46:40.264Z Reads: 206

```
Mine also does this.
```

---
## \#958 Posted by: Powadangaboards Posted at: 2019-04-25T12:47:16.846Z Reads: 207

```
Yes updated to the latest firmware a couple of days ago.
```

---
## \#959 Posted by: BigZwatt Posted at: 2019-04-25T13:40:31.309Z Reads: 199

```
Bluetooth . I installed it with unity u/i android app.
```

---
## \#960 Posted by: CarlCollins Posted at: 2019-04-25T15:49:41.467Z Reads: 200

```
Looks like it's not flashed properly, please use a USB-C cable and Windows PC to perform a flashing again
```

---
## \#961 Posted by: huntercasillas Posted at: 2019-04-25T19:54:10.809Z Reads: 198

```
When updating firmware to the unity, should it be plugged in to the battery or just USB C? I ordered a used one and it should be here soon so I was just curious.
```

---
## \#962 Posted by: venom121212 Posted at: 2019-04-25T20:04:36.340Z Reads: 190

```
The unity needs to be powered up to achieve a comm connection via either pc or mobile.
```

---
## \#963 Posted by: BigZwatt Posted at: 2019-04-26T02:54:06.108Z Reads: 191

```
Ok ill flash it friday at work.  Thank you for your help @CarlCollins I appreciate it.
```

---
## \#964 Posted by: jaxiethreetoes Posted at: 2019-04-26T04:58:39.391Z Reads: 193

```
Hey you funky cats,
I've been experiencing an intermittent fault with my unity, namely random unexpected shutdowns, after which the unit may or may not power up again.
I thought I had it licked when I resoldered a suspect connection to the antispark switch, but it happened again on the way home from work this morning, under moderate acceleration, with 20kg of tools on my back... Got drilled pretty hard and board wouldn't power up again - until it was on the bench, whereupon it fired up first time.

Old mate Occam says it's the switch, so just bypass it and add a loop key, but I'm wondering if there's anything else I should be checking.

Many thanks in advance for any sheddable light,
J3T
```

---
## \#965 Posted by: RobPBody Posted at: 2019-04-26T20:00:44.768Z Reads: 190

```
Can people confirm that Battery Meter connects to the port on the corner of the Unity? I have connected my meter, and nothing happens. When I connect the meter to the Battery Pack, it works. Just received my Unity maybe 3 weeks ago (2nd Batch shipped after February)
```

---
## \#966 Posted by: Jinra Posted at: 2019-04-26T20:06:34.792Z Reads: 191

```
yep, it does. Try taking a voltmeter to the pins **VERY CAREFULLY**. If you're getting 0v you likely blew the fuse on those pins.

You can either replace the fuse or bridge the fuse contacts.
```

---
## \#967 Posted by: Deodand Posted at: 2019-04-26T20:10:27.690Z Reads: 190

```
Might be obvious, but the pins only output voltage when the unity is turned on.
```

---
## \#968 Posted by: RobPBody Posted at: 2019-04-26T20:58:03.902Z Reads: 191

```
@Deodand @Jinra Thanks for the reply. Unity definitely powered up when I connected the meter.
```

---
## \#969 Posted by: ZachTetra Posted at: 2019-04-27T01:48:32.666Z Reads: 189

```
Is there any way to get 7v to 20v off the Unity?  Need a power source for an Arduino micro, it says it runs on 5v but the minimum input is 7v
```

---
## \#970 Posted by: kalebludlow Posted at: 2019-04-27T01:52:33.271Z Reads: 193

```
Your best bet would be a DC-DC buck converter running off the battery to the micro
```

---
## \#971 Posted by: BigZwatt Posted at: 2019-04-27T02:07:35.766Z Reads: 196

```
I need to update my unity on win. Bldc tool when I navigated to the firmware tab I selected update and a warning flashed saying Id brick my unity if I chose the wrong version. Which version do I select . Searched this first but I didnt have any luck
```

---
## \#972 Posted by: Blasto Posted at: 2019-04-27T02:13:06.311Z Reads: 201

```
Use the fw that is embeded in the tool, do not use tge bldc tool. Focbox unity had it’s own

https://github.com/EnertionBoards/FOCBOX_UI/tree/FOCBOX_UI/windows_build
```

---
## \#973 Posted by: BigZwatt Posted at: 2019-04-27T02:59:36.229Z Reads: 202

```
Thank you. My noob just showed itself
```

---
## \#974 Posted by: jmoji Posted at: 2019-04-27T13:53:29.895Z Reads: 200

```
Hey guys, Ive kinda skimmed through this thread for help setting up unity with hoyt remote. Noticed some of you had issues, but never really saw a solution. Ive only tried setting it up with the UI version on android. The problem I am having is when I push the throttle just about halfway, one of the motors starts slowing down until it just stops completely. Its weird because when I go full throttle, both motors spin perfectly fine. Would appreciate any help!
Thanks
```

---
## \#975 Posted by: Deodand Posted at: 2019-04-28T17:10:27.510Z Reads: 195

```
Sometimes one motor can have a bit more drag than the other. Shouldn't happen at half throttle probably, you ran the calibration routine with the latest app? I think I have patched those issues in the UI out. A screenshot of the results on the remote calibration screen would be helpful. Have you tried riding it at all?
```

---
## \#976 Posted by: ninTHIENdo Posted at: 2019-04-29T01:00:34.169Z Reads: 187

```
Anyone else having random cutouts during a hard acceleration after a slight rolling acceleration? I’m on Fw 23.43 on 8inch pneumatics, 70/-70 motor, 60/-30 battery, 12s8p 30q’s. It happens once or twice on a 13 mile ride, doesn’t happen during the high speed constant, just during hard acceleration after a little roll 5% of the time. Not enough to complain about but enough to ask if anyone else is having this issue.
```

---
## \#977 Posted by: Deodand Posted at: 2019-04-29T01:17:30.850Z Reads: 183

```
Sensored? Try tuning your sensorless erpm maybe?
```

---
## \#978 Posted by: jmoji Posted at: 2019-04-29T01:31:44.147Z Reads: 195

```
Yeah its weird, Ive tried re-calibrating it many times and same issue. I have tried riding it and well it seems okay, but you wont really notice one motor going out since the other motor is doing all the work. I noticed this issue when lifting the wheels. ![IMG_2846|640x480](upload://ugCqKH7crjSBqRvQWUjMmzYYysQ.jpeg)
```

---
## \#979 Posted by: jmoji Posted at: 2019-04-29T01:32:22.070Z Reads: 197

```
https://youtu.be/IYyj3bWjBjw
```

---
## \#980 Posted by: ninTHIENdo Posted at: 2019-04-29T01:34:30.408Z Reads: 198

```
Sensored, dual bkb 6374 190kv on a 1:4 kaly gear drive reduction. It’s not a stuttering issue, that was resolved with the firmware, it literally cuts out and then after I regain my balls after my bindings save me its back on running normal. I’ll try tuning the erpm next time I take it apart but thought that was for stuttering.  This was with just the standard fw running guided setup except for changing the battery and motor values.
```

---
## \#981 Posted by: jackluis Posted at: 2019-04-29T01:56:17.079Z Reads: 196

```
Hey guys. My unity started going ghost mode and accelerating on it own with the remote connected and not connected. This started happening right when my power button wires got messed up and lost their solder connection, leaving them connected only through shrink wrap. I resoldered them and the board hasn't done it again. Could these be connected or it is just a coincidence? What else should I check to make sure my board doesn't kill me? I use the nano remote btw.
```

---
## \#982 Posted by: CarlCollins Posted at: 2019-04-29T11:42:17.627Z Reads: 196

```
Check the Remote config tab of your Unity using FOCBOX UI and check the pulsewidth showing 0 or not?
```

---
## \#983 Posted by: Deodand Posted at: 2019-04-29T16:39:56.188Z Reads: 196

```
@jmoji this probably isn't related to the hoytt remote at all. To me it just looks like one of your drives has a bit more friction than the other. Notice on the app the amps to the left and right motor, it's like under 1 amp. This is effectively the torque being applied to the motors with some scaling applied and 1 amp is not much torque at all. So a slight difference in friction on each side could cause a large speed difference but shouldn't cause a noticable difference/problem while riding when your applying 30 amps instead of 1. You can also see the left motor comes to a stop immediatley while the right glides out. You might want to look for friction in the gearing of the left wheel, how does it feel with hand spinning each side in backdrive? Any noticable difference?  Might also be worth noting here that the UI of left vs. right motor here is mirrored for your setup here. The left data is for the right wheel and vice versa. 

You can also turn on traction control in the advanced tab of remote settings and it should make your wheels behave more in sync on the bench like this.
```

---
## \#984 Posted by: Deodand Posted at: 2019-04-29T16:45:32.118Z Reads: 197

```
@jackluis check the integrity of your reciever wires (red white black servo cable) and make sure you have good reciever placement. Sometimes the crimps on those can get loose/damaged if yanked. Make sure the 3 pin plug on the reciever is glued/affixed in place so it can't jiggle. The power switch doesn't have any control over the boards acceleration/deceleration and even if a false shutdown command were sent over the board would continue to behave as normal until you came to a stop. 

The only way it could have impact is some kind of crazy rf interference which seems unlikely to me.
```

---
## \#985 Posted by: Deodand Posted at: 2019-04-29T16:51:06.502Z Reads: 195

```
@ninTHIENdo can you run the faults command from the terminal after you trigger the behavior? It's possible that the sensorless transition doesn't happen smoothly causing a current spike that triggers an overcurrent fault. Luckily this only occurs at that low speed transition from sensored to sensorless driving if that's the cause, but I've found that tweaking the transition rpm can fix this issue sometimes. Can you share a screenshot of your motor config values from the app?
```

---
## \#986 Posted by: huntercasillas Posted at: 2019-04-29T20:25:44.820Z Reads: 189

```
Can you help me tune my throttle curve? I've tried a bunch of different ways, but it seems that the motors don't even kick in until 20% throttle and then from 35% to 100% has no change, it is just constant top speed.
```

---
## \#987 Posted by: Deodand Posted at: 2019-04-29T20:48:47.974Z Reads: 187

```
If this is on bench testing then I'd not worry about it. Think of the throttle as the gas pedal in your car and bench testing as putting your car in neutral. Even if you just slightly touch the gas pedal in neutral it revs your engine to max rpm. Fixing the initial lack of response is due to a property called deadzone, I forgot to add it in the app last release as I planned, but you can still tune it down from the full tool. By default it is set to 15%, this can be tuned down if you calibrate your remote well.
```

---
## \#988 Posted by: jmoji Posted at: 2019-04-29T21:03:54.146Z Reads: 191

```
Yeah that makes sense, but you probably cant see I still have the throttle pushing forward when the right motor goes out. That just doesn't make sense to me. I would understand if I let go of the throttle, one might slow down faster than the other and thats fine. My issue is the right motor cutting off even if I still have medium throttle on it. Hand spinning the motors feels pretty much the same for each. I will play around with the traction control to see if that changes anything.
```

---
## \#989 Posted by: jmoji Posted at: 2019-04-29T21:19:36.154Z Reads: 187

```
@Deodand Traction control did the trick! Both motors run how they are supposed to now! Thanks Jeff!
```

---
## \#990 Posted by: huntercasillas Posted at: 2019-04-29T21:42:17.039Z Reads: 193

```
Well I mean the motors don’t even move till I’m a quarter way up the throttle and then they just seem to go full speed with no precision control after engaging.
```

---
## \#991 Posted by: FranciscoV Posted at: 2019-04-29T23:29:08.644Z Reads: 193

```
Haha.  Enough to put me here that’s for sure 🤣🤣![image|281x499](upload://f6PfYKBQYfXWnKFAgvIm2nMjRpx.jpeg)
```

---
## \#992 Posted by: FranciscoV Posted at: 2019-04-29T23:35:23.132Z Reads: 193

```
Dude. I have the exact same setup as you do (6374 bkb 190kv motors with 4:1 gear ratio and 8” pneumatics) no bindings 😩 and I’m having the same exact issue with my shit.   Damn.   I hope enertion can help us fix this problem because kissing asphalt is not a good thing!!    

I never had that issue when I was running 6374 170kv maytechs.  Any help would be highly appreciated
```

---
## \#993 Posted by: FranciscoV Posted at: 2019-04-29T23:41:09.505Z Reads: 195

```
Damn.   I guess I’m not the only one with bad luck.   Here is my other unity     With this one I get nasty wobbles when reach top speed on my board on maytech 6374s 170kv motors.   It basically throws me off balance if I go over 35mph 

https://youtu.be/PCRvFTVL1Po
```

---
## \#994 Posted by: Eboosted Posted at: 2019-04-30T06:00:54.873Z Reads: 191

```
Hello guys, I'm having a problem with my board hooked to a Unity, however I'm not even sure if the problem is electronic or mechanic. I wonder if anyone had this expecience before. 

I'm runing a 12s4p made of Samsung 30T runing 100A -15A battery regen, if go full throttle I hear a weird sound, like if the belt is skipping or like if one tire looses grip, the board makes a weird push and I fight to not loose control, it feels like if only only on motor spins, I made sure to have the belts very well tighten, so they can't skip I even installed idlers.

Could this be a restriction on the unity because I'm runing very high current, I'm going to make a datalog of both of the wheel speeds in order to see if one wheel is in fact spiking.

Any ideas?
```

---
## \#995 Posted by: mackann Posted at: 2019-04-30T06:03:20.082Z Reads: 188

```
Im running mine in 120A without problems so 100 should be no problem.
Have you newest firmware? Have you traction controll on or off?
```

---
## \#996 Posted by: Eboosted Posted at: 2019-04-30T06:05:04.258Z Reads: 189

```
Traction control is on, I'll try TC off and see how it goes
```

---
## \#997 Posted by: jackluis Posted at: 2019-04-30T13:26:25.391Z Reads: 188

```
The problem stopped once I fixed my power button. My theory is that board was turning off and on and therefore left my nano to connect without doing a calibration. I'm doing a complete rebuild of my board in the next few days and hopefully that discovers any other issues I have. Thanks for all the help!
```

---
## \#998 Posted by: Sn4pz Posted at: 2019-04-30T14:02:32.312Z Reads: 187

```
[quote="FranciscoV, post:992, topic:77861"]
I never had that issue when I was running 6374 170kv maytechs. Any help would be highly appreciated
[/quote]


Not even once? Ill have the same setup essentially
```

---
## \#999 Posted by: FranciscoV Posted at: 2019-04-30T14:07:57.444Z Reads: 180

```
Not even once on 170kv.   Issue started when went to Bkb 6374 190kv motors.  Not with one but both my unities.    
Even on the bench with no load or even belts.      0 to 100% throttle with trigger the power cut out
```

---
## \#1000 Posted by: Blasto Posted at: 2019-04-30T14:34:37.246Z Reads: 182

```
you're running the latest FW? can you share the motor detection parameters.

also what type of remote do you have, almost sounds like you ppm signal is overshooting the maximum pulse width parameter.
```

---
## \#1001 Posted by: FranciscoV Posted at: 2019-04-30T14:53:44.242Z Reads: 187

```
Yes sr.  Latest fw and I’m using Hoyt remote.   Currently using the app on an old android phone but problem persisted even after using a pc
  ![image|375x500](upload://c6VDmzXpT1XvyPceuDFD71Rh8IQ.jpeg) ![image|375x500](upload://hGLPeN5DsdyDXCHaQWs4tUHufKy.jpeg) ![image|375x500](upload://i6v5AcpDj8l9Qnhtrg3CeORT1DV.jpeg)
 https://youtu.be/Y9o6oUNdh0s
```

---
## \#1002 Posted by: Blasto Posted at: 2019-04-30T15:04:32.285Z Reads: 174

```
thanks that is clearer.

strangely your throwing a fault.

just for debug, disconnect the sensors and re-run a motor detection
```

---
## \#1003 Posted by: FranciscoV Posted at: 2019-04-30T15:06:57.640Z Reads: 174

```
Great idea.  I’ll try that once I get home from work.  Keep you posted 
   Thanks brother
```

---
## \#1004 Posted by: mackann Posted at: 2019-04-30T17:08:26.637Z Reads: 175

```
Could you try lowering motor A to 65A and se if its same problem?
```

---
## \#1005 Posted by: FranciscoV Posted at: 2019-04-30T17:34:27.466Z Reads: 176

```
I have not and I will try it BUT let’s say that that works.  Heck.  That would be kinda lame to be stuck at 65 motor max.     Issue that I never had with focboxes.     I known they’re 2 different products but unity was supposed to be better performer than focbox.   Pls correct me if I’m wrong but so far that haven’t been the case.  At least not for me
```

---
## \#1006 Posted by: Blasto Posted at: 2019-04-30T17:35:48.118Z Reads: 177

```
I do agree that would be lame.

other thing to try out is cranking up your absolute max current, since your other currents are very high, this one should follow also

![image|690x396](upload://hNIIWBj8md8NcQQyFhqPM6H62HV.png)
```

---
## \#1007 Posted by: FranciscoV Posted at: 2019-04-30T17:41:36.037Z Reads: 175

```
A piece of info that might be helpful is.   I’m using a Hoyt puck    I can trigger the fault over n over in mode 3 
I have not been able to do that in mode 2 if that makes sense 🤷🏻‍♂️
```

---
## \#1008 Posted by: Blasto Posted at: 2019-04-30T17:45:30.608Z Reads: 179

```
[quote="FranciscoV, post:1007, topic:77861"]
mode 3
[/quote]
 
is mode 3 the fastest mode? side note, make sure the ppm calibration was done in the fastest mode

but back to the ABS max current, set that value to 180-200 in the full tool. will need to connect to a pc.
```

---
## \#1009 Posted by: FranciscoV Posted at: 2019-04-30T17:48:11.015Z Reads: 175

```
That is correct.  Mode 3 is fastest.  And yes.   Remote was calibrated in mode 3 
Checked and it goes as follow 
Mode 1 =33% 
Mode 2 =57% 
Mode 3 =100%


Thanks for all of the help and suggestions btw.   Highly appreciate it
```

---
## \#1010 Posted by: Deodand Posted at: 2019-04-30T17:53:36.258Z Reads: 174

```
I think simply turning up the absolute max current will solve this. Let us know how it goes.
```

---
## \#1011 Posted by: FranciscoV Posted at: 2019-04-30T17:55:27.229Z Reads: 177

```
@Deodand I sure will try that.  Keep you guys posted.   Thanks again everyone.  Learning new shit never gets old 🙂
```

---
## \#1012 Posted by: sayekim Posted at: 2019-05-01T11:06:58.605Z Reads: 170

```
How is that set to 180 absolute max?

I’m running 3.38fw and maximum possible setting is 160. 
Is it the no hw limits version perhaps?
```

---
## \#1013 Posted by: CarlCollins Posted at: 2019-05-01T13:00:33.476Z Reads: 170

```
3.38 is VESC firmware but FOCBOX Unity is pretty different from it :slight_smile:
```

---
## \#1014 Posted by: Deodand Posted at: 2019-05-01T14:21:02.520Z Reads: 168

```
Our hardware max is simply set to 200, it's just a #define in the firmware.
```

---
## \#1015 Posted by: ninTHIENdo Posted at: 2019-05-01T21:22:49.318Z Reads: 168

```
I can’t show the faults, always forget and turn off the board before I take it apart since I’m on iOS. Looks Ike fransiscoV got the same results and I’ll try adjusting the absolute value when I take it apart tonight to re-epoxy and drill some more enclosure inserts 😂🤷‍♂️...I’ll report back on if this fixes the issue in 24-48hrs after the epoxy dries and I can run a thorough test. And I am as well running a Hoyt remote...😂🤣
```

---
## \#1016 Posted by: FranciscoV Posted at: 2019-05-02T01:21:50.941Z Reads: 169

```
Ok.  I have not been able to work on my board yet but my boy @Tello1969 was having the exact same issue with his unity, maytech 190kv 6880s and Hoyt puke.  Spoke with him over the phone and just like @Blasto and @Deodand have suggested I’ve told him bump motor absolute max current from 130 to 180 amps and that seems to have fixed the abs over current issue.   Now let’s have in mind.   This Is based on bench testing.   No belts or wheels on the board.   Let’s hope it stays that way under load.  I mean.  Severe load (like smashing up hills in sf with a hefty 200lbs boy on it)  will report back with results
```

---
## \#1017 Posted by: Deodand Posted at: 2019-05-02T01:25:49.245Z Reads: 172

```
Yeah, let us know.
```

---
## \#1018 Posted by: paulocruz1920 Posted at: 2019-05-02T17:48:34.371Z Reads: 175

```
can you please give me the link to download the node? the node i downloaded doesn't have a commands.c file.

thanks
```

---
## \#1019 Posted by: Deodand Posted at: 2019-05-02T19:07:16.903Z Reads: 174

```
It is in the source code:

https://github.com/EnertionBoards/bldc
```

---
## \#1020 Posted by: ninTHIENdo Posted at: 2019-05-02T19:56:16.654Z Reads: 174

```
Just got the board taken apart and changed those values, I’ll let you know in a few hours how it goes when I take it to the gym and get done if you don’t beat me to it. Gorilla tape works great while epoxy dries...
```

---
## \#1021 Posted by: Marsl187 Posted at: 2019-05-02T20:45:19.525Z Reads: 184

```
@Deodand @FranciscoV I still have that issue too after the fw update. Today was going up a hill under high load for a few minutes. At the end I pulled the trigger to the max which caused a cutout after maybe 5 to 10 seconds. I was able to make a photo of the fault. 


![5dd887be-0746-4946-9e26-d0fad60c5364|236x500](upload://r5cwCw7iXO8Rch6wYJcToNQBhRu.jpeg) 


So changing the absolute max to 180A should be fine? What is the max it can withstand before breaking? Just interested...
```

---
## \#1022 Posted by: FranciscoV Posted at: 2019-05-02T21:23:46.083Z Reads: 184

```
Well. That was the theory at least.   Report back from @Tello1969 say even after that change his board kept having the same issue.     This thing really blows.   This is a big deal since people can get really hurt riding the unity 
Now.  Enertion tech support has been or at least have tried to be helpful.    The can assure that this is just a fw issue.     But problem is    It seems to be affecting a shit load of people 

Let’s hope they can figure this one out before someone gets seriously hurt 😬
```

---
## \#1023 Posted by: huntercasillas Posted at: 2019-05-03T00:31:33.434Z Reads: 184

```
@Deodand is there anywhere I can download an iOS app prototype and sideload it onto my iPhone? Or even the code and then I can build it myself with Xcode. PS if you need any help I develop for iOS.
```

---
## \#1024 Posted by: ninTHIENdo Posted at: 2019-05-03T00:49:31.309Z Reads: 181

```
So far changing it to 180amp max has fixed the cutout issue for me in real life testing. 17-18 miles with lots of stop and go and even through some semi wet grass to spin out a little bit. Will continue reporting back after some more real life testing.
```

---
## \#1025 Posted by: FranciscoV Posted at: 2019-05-03T00:58:53.879Z Reads: 184

```
Just be safe brother.  My problem happens when I punch it from 0 to full throttle. Even when there is no load on the motors
```

---
## \#1026 Posted by: Rudacris Posted at: 2019-05-03T09:36:16.567Z Reads: 190

```
Just got my Kaly 2.0... I want to adjust the braking and acceleration, turn it down a bit! Even when barely pressing the remote to brake, it almost throws me off. I feel like I'm in survival mode while riding it. Maybe great once i get more used to it, but for now, its too much. I'm trying to connect to FocBox Unity app with android on my s9 plus...But when it connects for a split second, it then disconnects and gives this error...does anyone know how to remedy this? Without having to take off the enclosure and using a cord? and, if the only way is with a cord...what needs to be done and how would i do it? Thanks in Advance!

*Update, i learned from Ernesto that he is waiting on an update on unity side. Currently they are different versions. Not sure what is what (newbie). But he said when they provide that update and both versions are the same or something...it should work over bluetooth. Anyway, calibration of remote fixed what i needed for now. The other fine tuning can wait. Now its time to ride! ;) 

![Screenshot_20190503-013136|243x500](upload://vpH8R9lbZKHEI8GNIgpLtuR81VA.jpeg)
```

---
## \#1027 Posted by: paulocruz1920 Posted at: 2019-05-03T10:51:26.730Z Reads: 180

```

Deodand thank you for your help!
```

---
## \#1028 Posted by: Deodand Posted at: 2019-05-03T11:46:43.884Z Reads: 180

```
@Rudacris you might need to open the enclosure and inspect if the BLE module is properly seated in the unity. If it isn't I recommend re-seating  and adding a touch of silicone glue to secure it against vibrations.
```

---
## \#1029 Posted by: Jinra Posted at: 2019-05-03T15:45:47.181Z Reads: 184

```
[quote="Rudacris, post:1026, topic:77861"]
Even when barely pressing the remote to brake, it almost throws me off.
[/quote]

It sounds like you're not calibrating the remote every time you turn it on. If you fail to do so, the slightest throttle will send full throttle/full brake signal to your vesc
```

---
## \#1030 Posted by: Rudacris Posted at: 2019-05-03T17:24:03.099Z Reads: 182

```
Thanks for your quick response! I see. So u think USPS wasnt gentle with my board?! ;p only NYC to Cali ;) I will check that! Thank you!
```

---
## \#1031 Posted by: Rudacris Posted at: 2019-05-03T17:28:57.609Z Reads: 185

```
You know...im gonna give it another shot today. Im so used to turning on my evolve GT board first. And, honestly didnt know anything about needing to calibrate new Nano remote (until last night after reserching the trouble i was having on day 1 with new board) I did see how to do that. Thank you for bringing that up. Ill let u know the difference it makes.
```

---
## \#1032 Posted by: Jinra Posted at: 2019-05-03T17:29:56.574Z Reads: 189

```
It makes a world of difference, I've been using that remote for years. Best practice is to turn the remote on first, full throttle, full brake, then turn on the board.
```

---
## \#1033 Posted by: Rudacris Posted at: 2019-05-03T18:40:29.666Z Reads: 190

```
You are right @Jinra and it did. So much better! With calibration it seems there are 3 modes of braking power now. Without calibration, 1st mode would be full braking. Yesterday, i was fighting to stay on the board. Today, it is everything i hoped for :) thanks for the help!!!
```

---
## \#1034 Posted by: BigZwatt Posted at: 2019-05-04T04:21:37.352Z Reads: 187

```
@Deodand @CarlCollins thank you for your help.
 I flashed the unity.  The cogging at slow speed stopped.
```

---
## \#1035 Posted by: CarlCollins Posted at: 2019-05-04T13:39:38.935Z Reads: 188

```
Awesome

10chars
```

---
## \#1036 Posted by: Powadangaboards Posted at: 2019-05-04T16:43:18.066Z Reads: 186

```
Ok, so third time my board has just completely locked up sending me flying? Only seems to do it when going at speed?

Any one else getting this?
```

---
## \#1037 Posted by: Blasto Posted at: 2019-05-04T17:17:48.665Z Reads: 185

```
Are you using the lattest fw (23.43) What is your setup, screen shot of settings
```

---
## \#1038 Posted by: FranciscoV Posted at: 2019-05-04T20:54:49.441Z Reads: 184

```
@Deodand  Quick update 
Swapped back to 170kv motors and now working fine!   At least seems like it.  
Unity and 190kv motors don’t like each other my guess 🤷🏻‍♂️
I’m yet to bump up my motor absolute max.         “I don’t have a pc”😩
```

---
## \#1039 Posted by: FranciscoV Posted at: 2019-05-04T21:03:20.744Z Reads: 174

```
@Deodand ok. Bench testing On 170kv motors I seem to be able to replicate the fault when I drop the positive throttle ramp up time down to .10 seconds 
All of this done through android app   Best bet would be leave at default!?  .30s??
```

---
## \#1040 Posted by: McErono Posted at: 2019-05-04T22:09:33.237Z Reads: 175

```
I only used the app for my unity setup with torqueboards DD 75kv, latest firmware, 12s4p. I can go full throttle flat, uphill whatever, no cutouts. Whats going on? :flushed:

Is it the hoyt puck? Higher kv motors? Or anything above 65 motor amps?
```

---
## \#1041 Posted by: Jinra Posted at: 2019-05-04T22:15:25.157Z Reads: 178

```
last time this happened on my 4.12 ollin vesc, it was a slow burn DRV failure. Over the next couple months I got more and more issues until the DRV fault finally manifested and I had to replace it.

In the interim, this at least temporarily solved my overcurrent issues
https://www.electric-skateboard.builders/t/focing-around-weak-brakes-and-cutout/33203/107?u=jinra
```

---
## \#1042 Posted by: Blasto Posted at: 2019-05-04T22:35:58.531Z Reads: 181

```
We’re looking into this issue, we have some low inductance motors on order and we’ve built our test case to reproduce the issue. 

Once we’re able to reproduce the issue we’ll be able to isolate and solve it. We already have a few hypotheses, just a mather of time
```

---
## \#1043 Posted by: FranciscoV Posted at: 2019-05-04T23:41:09.128Z Reads: 183

```
Thank you for looking into it 
It blows that both my unities do the same thing.     Problem seems to have begun when 190kv motors were installed 

Also.  There is no issue With 170kv motors @40 amps each even if positive throttle ramp up time is set to .05 sec
```

---
## \#1044 Posted by: Blasto Posted at: 2019-05-04T23:44:31.459Z Reads: 181

```
Can you post all of your settings (including throttle) so i can reproduce the fault
```

---
## \#1045 Posted by: FranciscoV Posted at: 2019-05-04T23:54:02.664Z Reads: 182

```
I use the app 
85a per motor 
Default 12s battery cut out 
110a battery discharge 
Hoyt remote calibrated in mode 3
```

---
## \#1046 Posted by: ShredRedwood Posted at: 2019-05-06T17:33:06.053Z Reads: 184

```
Okay, so I'm not sure what I've got going on here.  When I plug in from my laptop and run the firmware update it seems to update fine. It does disconnect at the end, I'm assuming because the unity is rebooting? I'm still having an issue with a chunky start if I give too much throttle from a stop though. It's not a belt skip, it's like the motor is rumbling. When I connect to the unity from my phone I get told the firmware needs to be updated and then shortly after I lose Bluetooth connection. Any ideas? ![Screenshot_2019-05-06-10-26-15|264x500](upload://2pyXh5hlqDohwk9cxfxKv9BMiEu.png) ![Screenshot_2019-05-06-10-26-44|264x500](upload://7s132Di3oS1j092QCNKdlwlQtBT.png)
```

---
## \#1047 Posted by: Blasto Posted at: 2019-05-06T17:41:35.406Z Reads: 175

```
update your pc software also.

currently i think you have a older pc version versus the app
```

---
## \#1048 Posted by: ShredRedwood Posted at: 2019-05-06T18:02:41.356Z Reads: 178

```
Thanks, that fixed the firmware notification but I'm still getting the BLE error and connection drop shortly after connecting.

Edit: aaaand my motors are spinning opposite directions now

Double edit: not a smart man. Fixed the motor reverse.
```

---
## \#1049 Posted by: McErono Posted at: 2019-05-07T10:49:44.982Z Reads: 184

```
[quote="McErono, post:1040, topic:77861"]
I can go full throttle flat, uphill whatever, no cutouts. Whats going on? :flushed:
[/quote]

Have to correct that. I do have cutouts! But only while going full throttle from standstill. Motoramps do not affect anything, tried 40-80amps.

Time to hook up the Unity over USB but there is something wrong (overall max current?) with the stock app setup.
```

---
## \#1050 Posted by: FranciscoV Posted at: 2019-05-07T19:36:34.799Z Reads: 181

```
Welcome to the club brother.    Slow acceleration ramp up is ok.   You try to take off like a bat out of hell you gonna hit the ground.    There is definitely something going on there!   Many people might not be affected just because they like to ride very conservatively.   There are a few of us that like to push our boards a little harder and that’s when the problem occurs 😩
```

---
## \#1051 Posted by: Deodand Posted at: 2019-05-07T23:05:23.824Z Reads: 177

```
We've got the issue reproduced on our end now, FW update will be out in a few days.
```

---
## \#1052 Posted by: McErono Posted at: 2019-05-07T23:16:17.786Z Reads: 182

```
yes! very very good news! thank you Jeff! :star_struck:
```

---
## \#1053 Posted by: FranciscoV Posted at: 2019-05-07T23:28:45.341Z Reads: 185

```
Question.  How about the battery settings through the app issue.   I like to use custom settings on my soft/hard cutoff   Hit apply then disconnect from the app.  But then when I reconnect to the app again “or someone connects to my unity with their phone on accident”  my battery settings get kicked off to 11 cells!
```

---
## \#1054 Posted by: huntercasillas Posted at: 2019-05-08T02:09:05.578Z Reads: 186

```
Can anyone help me reduce the torque in the settings? If that’s possible. I just took my first build for a test ride and it scared me lol, almost threw me off 3 times because of how quick it accelerates. Maybe the remote throttle needs to be fine tuned? I thought I already had the settings for the most gradual increase possible though.
```

---
## \#1055 Posted by: FranciscoV Posted at: 2019-05-08T02:30:18.582Z Reads: 188

```
What remote are you using!?
```

---
## \#1056 Posted by: huntercasillas Posted at: 2019-05-08T02:42:01.824Z Reads: 183

```
Flipsky VX1
```

---
## \#1057 Posted by: FranciscoV Posted at: 2019-05-08T03:47:05.897Z Reads: 188

```
Ah!!   For some reason I thought you were using a regular nano remote witch requires calibration every time you turn it on.  Anyone pls correct me if I’m wrong but that’s not the case with new Flipsky remote 
One thing you could do is start slow on mode 2 on your remote and work your way up to the fastest mode.   New boards can be scary at first but then you get used to them and it’s all good.
```

---
## \#1058 Posted by: Deodand Posted at: 2019-05-08T19:54:03.347Z Reads: 181

```
@huntercasillas  You want to just turn down max motor amps.
```

---
## \#1059 Posted by: huntercasillas Posted at: 2019-05-08T23:34:45.787Z Reads: 181

```
Just tried and felt the same. It seems smooth in the beginning on the throttle if I go very slow but then it gets to like half way up the throttle and wants to jump to max speed and jolts me back making me think I’m going to fall.
```

---
## \#1060 Posted by: huntercasillas Posted at: 2019-05-08T23:44:11.805Z Reads: 180

```
Here's the current throttle curve settings.

![Throttle|423x500](upload://vOw5e6MhAeupZ8yvGvZyfWWdcdL.jpeg)
```

---
## \#1061 Posted by: Jinra Posted at: 2019-05-08T23:52:19.189Z Reads: 178

```
are you using PPM, and if so what are your PPM values (min/max/center). Also when you do a live reading does it go up smoothly?
```

---
## \#1062 Posted by: huntercasillas Posted at: 2019-05-08T23:56:08.498Z Reads: 181

```
Yes. It says -100 1 and 100
```

---
## \#1063 Posted by: huntercasillas Posted at: 2019-05-08T23:56:33.359Z Reads: 181

```
Does like the voltage go up smoothly?
```

---
## \#1064 Posted by: huntercasillas Posted at: 2019-05-08T23:59:10.721Z Reads: 185

```
![image|666x500](upload://g3MnDVsKBIB8rnFKhwjGpxbpZsY.jpeg)
```

---
## \#1065 Posted by: Jinra Posted at: 2019-05-08T23:59:17.242Z Reads: 178

```
Does the PPM value go up and down smoothly
```

---
## \#1066 Posted by: huntercasillas Posted at: 2019-05-09T00:01:18.130Z Reads: 180

```
Yes it does.
```

---
## \#1067 Posted by: huntercasillas Posted at: 2019-05-09T00:03:05.894Z Reads: 176

```
From 30% throttle to 100% is just max speed
```

---
## \#1068 Posted by: Jinra Posted at: 2019-05-09T00:03:41.867Z Reads: 176

```
Are you talking about on the bench?  because that's completely normal. When applied current overcomes present load, it'll always try to spin at max duty cycle
```

---
## \#1069 Posted by: huntercasillas Posted at: 2019-05-09T00:05:46.453Z Reads: 173

```
Yeah. Okay that’s good then
```

---
## \#1070 Posted by: huntercasillas Posted at: 2019-05-09T00:08:27.250Z Reads: 171

```
It just feels like there’s no adjustment. It’s either not going or it’s full speed
```

---
## \#1071 Posted by: Deodand Posted at: 2019-05-09T00:08:55.849Z Reads: 175

```
Set your torque curve back to like -10% on both sides and then decrease the motor amps according to taste from there. Your torque curve is too curved.
```

---
## \#1072 Posted by: Jinra Posted at: 2019-05-09T00:09:27.154Z Reads: 178

```
It behaves differently when you're actually riding it because load is much higher. VESCs/FocBox control current not duty cycle life common ESCs. Treat it more like a car gas pedal.
```

---
## \#1073 Posted by: huntercasillas Posted at: 2019-05-09T00:10:22.921Z Reads: 177

```
Okay I’m doing that and going for a test ride now. Thanks!
```

---
## \#1074 Posted by: huntercasillas Posted at: 2019-05-09T00:18:22.906Z Reads: 176

```
I took it for a test ride and let's say I put the throttle at 5% or whatever percentage where the motors kick in and start moving... I keep my thumb in the same place, but my unity just keeps giving the motors more until I'm at full speed. I can't cruise at lower speeds unless I give it gas and then release the throttle and coast off the inertia. Ideally I would want to be going half max speed when my throttle is half activated.
```

---
## \#1075 Posted by: Jinra Posted at: 2019-05-09T00:20:02.318Z Reads: 180

```
That's not how current control works. You'd have to be more clear about percentages because 5% wouldn't actually move it at all since the default dead zone is 15%. Once you move past 15% it'll start moving, but like i said, if applied current overcomes load, it'll go to max speed. I'd recommend leaving throttle curve as linear
```

---
## \#1076 Posted by: huntercasillas Posted at: 2019-05-09T00:23:07.061Z Reads: 180

```
Yeah that's why I said or whatever percentage where the motors kick in. I was just throwing in a low percentage of 5 to say I had barely moved the throttle forward. That's really unfortunate. How are the hobby wing ESC and boosted board ESC able to keep speed linear with the throttle? like 50% max speed at 50% throttle. I assumed the unity would be able to do the same thing.
```

---
## \#1077 Posted by: Jinra Posted at: 2019-05-09T00:25:30.452Z Reads: 180

```
One of the main points of the VESC was to offer a superior control mode (which is current control). You can set it to kind of similar using duty cycle control (in the full desktop tool) but it's an inferior mode and will keep your speed at whatever throttle position your at at all times (neutral means it will try to bring to board to a complete stop).

I suggest you try it out and get used to it before judging it
```

---
## \#1078 Posted by: huntercasillas Posted at: 2019-05-09T04:32:16.074Z Reads: 182

```
I will give it more time. But how do you cruise at slower speeds? Do you just push on the throttle and then let go and repeat?
```

---
## \#1079 Posted by: Jinra Posted at: 2019-05-09T04:56:00.955Z Reads: 181

```
yea, but you should be able to find an equilibrium between your current path and throttle position where it will just maintain the speed, unless the terrain changes (incline/decline)
```

---
## \#1080 Posted by: huntercasillas Posted at: 2019-05-09T05:02:05.587Z Reads: 180

```
I couldn’t from my limited experience so far. As soon as the motors engage it builds up to full speed. Doesn’t matter how much I push on the throttle.
```

---
## \#1081 Posted by: Jinra Posted at: 2019-05-09T05:03:13.323Z Reads: 180

```
It might be worth lowering the deadband, which you can only do with the full Windows version of the focbox tool (not focbox ui)
```

---
## \#1082 Posted by: huntercasillas Posted at: 2019-05-09T07:37:13.228Z Reads: 178

```
Is there a way to use duty cycle mode but only brake when the throttle is reversed/pulled back and have it coast when at the neutral position?
```

---
## \#1083 Posted by: danwooller Posted at: 2019-05-09T08:30:48.376Z Reads: 180

```
This is what mine is like, it's an animal compared to my WowGo.
```

---
## \#1084 Posted by: legend27 Posted at: 2019-05-09T09:58:46.157Z Reads: 177

```
Are you running single motor?
```

---
## \#1085 Posted by: huntercasillas Posted at: 2019-05-09T14:35:25.658Z Reads: 171

```
Dual 6354 190kv
```

---
## \#1086 Posted by: huntercasillas Posted at: 2019-05-09T18:59:29.964Z Reads: 178

```
I did a bunch more testing and it’s better once you get used to it. I just think the throw on my remote is either too sensitive or short
```

---
## \#1087 Posted by: Jinra Posted at: 2019-05-09T19:11:43.583Z Reads: 176

```
I use the same remote and it's perfect for me. I prefer shorter throws
```

---
## \#1088 Posted by: Bas1 Posted at: 2019-05-09T20:31:18.174Z Reads: 174

```
does anyone know how i can fix this focbox Unity. engines goes full throttle for a few seconds and stop running. probably i used wrong settings.
https://m.facebook.com/groups/135826490339055?view=permalink&id=391159741472394
```

---
## \#1089 Posted by: Blasto Posted at: 2019-05-09T20:40:20.529Z Reads: 173

```
seems like the ppm calibration was done in a "slow" mode. Redo you ppm calibration on the Unity, make sure you remote is in a "fast" mode while doing the calibration.

Edit:I just looked at the videos w sound, your ppm calibration is not set correctly

On the remote, make sure you are in esk8 mode (dont ask me how i dont know)

On the unity app:
Go to the remote settings and hit “calibrate”, press max throttle (release) then press max brake, release, hit OK then apply. You should see a message at the bottom “mc configurations applied”
```

---
## \#1090 Posted by: Bas1 Posted at: 2019-05-10T07:33:53.328Z Reads: 172

```
Thanks for helping yes i will try to calibrate again. think I didn't press full throttle and full brakes I hope this is the issue.
```

---
## \#1091 Posted by: ShueBox Posted at: 2019-05-11T02:21:35.557Z Reads: 171

```
Happening to me as well - stock settings and every other setting mentioned in this thread. Then it would go as far as turning my battery off, I guess the BMS cut it for protection but I have no idea... yet.
```

---
## \#1092 Posted by: Touch415 Posted at: 2019-05-11T02:52:50.583Z Reads: 172

```
@EnertionSupport. Needs to get on this ASAP
```

---
## \#1093 Posted by: FranciscoV Posted at: 2019-05-11T03:14:43.583Z Reads: 173

```
Damn!!   It really suxs   I know @Deodand is working on a possible solution but it isn’t for sure that it will fix the problem 100%
Hopefully he wants share that possible solution with you 😬
What I’ve done to still be able to ride my board and somehow be safe is I’ve gone back to 170kv motors and done my settings pretty conservative 
No racing people off a dead stop because that’s when shit hits the fan.    Good luck brother and please be safe.     I’m crossing my fingers enertion will be able to pin point the issue and take care of it once and for all!!    Riding in conservative setting sure suxs big Time 🤣🤣
```

---
## \#1094 Posted by: FranciscoV Posted at: 2019-05-11T03:17:00.017Z Reads: 166

```
It kinda blows when 3 out of 3 boards you own run on unities 🤣🤣.    And then to top it off you still have a spare unity just laying around in case one of your unities go bad 😩🤣
```

---
## \#1095 Posted by: Jinra Posted at: 2019-05-11T03:47:44.366Z Reads: 170

```
Did you try my bandaid fix of halving or doubling the observer gain
```

---
## \#1096 Posted by: FranciscoV Posted at: 2019-05-11T06:42:48.726Z Reads: 167

```
Unfortunately I have not!
Since I don’t own a pc I was hoping to borrow one and get it done over the weekend!
Normally I do my programming with an old android phone.  The Mac version of the tool for my computer is not yet available 😩
```

---
## \#1097 Posted by: Jinra Posted at: 2019-05-11T06:46:13.460Z Reads: 166

```
You could get a cheapo windows tablet

https://www.amazon.com/8-inch-Touchscreen-Processor-Bluetooth-Refurbished/dp/B073XV8GV1/ref=sr_1_6?keywords=windows+tablet&amp;qid=1557557103&amp;refinements=p_36%3A100-13000&amp;rnid=386442011&amp;s=electronics&amp;sr=1-6#customerReviews
```

---
## \#1098 Posted by: FranciscoV Posted at: 2019-05-11T06:57:28.653Z Reads: 169

```
Yeah.  I might end up doing just that.   Ima try to get it done this weekend.  I will also have to switch back to 190kv motors witch is when the issue becomes more apparent.    I’ll report back!!   Thanks again for the help 👍🏼
```

---
## \#1099 Posted by: ShueBox Posted at: 2019-05-11T16:06:07.908Z Reads: 175

```
[quote="FranciscoV, post:1093, topic:77861"]
ally suxs I know @Deodand is working on a possible solution but it isn’t for sure that it will fix the problem 100% Hopefully he wants share that possible solution with you :grimacing: What I’ve done to still be able to ride my board and somehow be safe is I’ve gone back to 170kv motors and done my settings pretty conservative No racing people off a dead stop because that’s when shit hits the fan. Good luck brother and please be safe. I’m crossing my fingers enertion will be able to pin point the issue and take
[/quote]

I'm using 149kv turnigy motors. I think I may have resolved it - or I haven't repeated it yet today when I am intentionally trying to. Will follow up later once I've had time to mess around a bit more!
```

---
## \#1100 Posted by: Blasto Posted at: 2019-05-11T16:10:51.891Z Reads: 171

```
We’re actually found a fix, we’re busy doing an extensive sanity check to make sure we didnt fuck anything else up
```

---
## \#1101 Posted by: ShueBox Posted at: 2019-05-11T18:01:23.553Z Reads: 173

```
Awesome, ready to put bigger motors on lol
```

---
## \#1102 Posted by: Meeep Posted at: 2019-05-12T01:27:32.912Z Reads: 181

```
I am having an issue with motor detection. I was riding along at 22mph and suddenly lost power and brakes. Tried turning the remote off/on, same with the Unity to no luck. The Unity would power on and the remote would work but when I give it full throttle the motor doesn't go very fast and my battery "sags" from 45% to 0% on the UI. 

I tried to running motor detection again and keep getting "L2 is 0. Please measure it." on 3 different motors. At first I thought my motor went bad but now I'm worried the Unity is acting up and have no idea what to do. I already had a Unity sent back because of a faulty USB-C port and really don't know what's wrong. :persevere:
```

---
## \#1103 Posted by: murloc992 Posted at: 2019-05-12T07:34:59.964Z Reads: 180

```
Tried my board yesterday. All I can say about unity:

* Silent
* Smooth
* Cuts out at 55kmh making me partially disabled for life(pop went the knee) 
* Extreme acceleration even at 30 motor amps

11/10

Edit:

Suggestive photo of an exploded knee.
[spoiler]![34|690x388](upload://3tK91m48mtMFeVwQmNK0lPMEu5N.jpeg) [/spoiler]
```

---
## \#1104 Posted by: FranciscoV Posted at: 2019-05-12T16:29:01.127Z Reads: 176

```
Damn!   They should recall these damn things!!  They’re nice but sure are dangerous 

I tried using my cousins laptop to program mine yesterday in hopes to patch the issue up but trying to connect to usb c was useless.   So I’m at square one waiting on a permanent solution to the huge amount of issues people are having with unities.   Let’s hope it happens sometime soon because honestly this Shit is scary    

Pls be safe guys
```

---
## \#1105 Posted by: SeanHacker Posted at: 2019-05-12T16:34:30.083Z Reads: 176

```
[quote="FranciscoV, post:1104, topic:77861"]
They should recall these damn things!
[/quote]

If only Jason's pride didn't get in the way and blind him. Unfortunately it's never going to happen based on the past. This sucks boys. Stay safe and suit up! Ugh...
```

---
## \#1106 Posted by: Toughook Posted at: 2019-05-12T16:37:09.831Z Reads: 181

```
Just installed unity and reassembled my board with 6" AT wheels. Battery is 10s5p 30Q, with bestech 80A bms. Dual 6374 190kv motors.

Can sometime please assess these provisional settings for me ? Anything glaringly obvious that is wrong? Thanks !

![Screenshot_20190512-173222|243x500](upload://vxc9iGEs5gGz8WzJqiukEuBz80S.jpeg) ![Screenshot_20190512-173253|243x500](upload://vwd4DAtOea38pu6etKg5k2jBwRp.jpeg)
```

---
## \#1107 Posted by: SeanHacker Posted at: 2019-05-12T16:38:24.907Z Reads: 176

```
[quote="murloc992, post:1103, topic:77861"]
* Cuts out at 55kmh making me partially disabled for life(pop went the knee)
[/quote]

I've had the same thing happen at 30mph using Enertion products. I almost lost my life. Hoping you recover enough to jump back into it dude. More testing needs to happen prior to shipping these things to customers. I've been screaming this to Enertion for a couple years now. But $$$ is the end goal (or only goal) it seems. Pretty sad. Sorry this happened to you too.
```

---
## \#1108 Posted by: Slydunan Posted at: 2019-05-12T16:42:05.394Z Reads: 185

```
What were your settings? Mine had cutouts under load as well, and my theory is that its due to mismatching battery/motor settings. Originally i set it according to the setup video on the main post, where motor amp is equal to battery limit, like so on a 12s4p

![Screenshot_2019-05-12-12-39-13|230x500](upload://79TwRjUNK1rLe24pjx1DzKoBuDn.png)  

But when riding and looking at the hud, both motors would exceed 35 amps. If these are 35 for each motor, the 70 amp total exceeds the 60 amp battery limit, which could explain the cutouts. So now im setting the motor limit to half the battery limit. No more cutouts so far.

![Screenshot_2019-05-12-12-39-21|230x500](upload://gZaEFkScgEpIiQtKymicYfhbCue.png)
```

---
## \#1109 Posted by: McErono Posted at: 2019-05-12T16:43:04.919Z Reads: 176

```
Question is was that fault there from the beginning or was it introduced with the latest firmware? Either way enertions betatester suck! Noone tested the unities at their limits? Noone ever hit full throttle from stand-still? :roll_eyes:

At this point every buyer should at least have received an email from enertion support to be careful until a fix is available.

@Slydunan I tried 40 to 80 motor amps and had cutouts... will try 30 amps but thats hilariously slow isnt it?
```

---
## \#1110 Posted by: murloc992 Posted at: 2019-05-12T16:51:00.410Z Reads: 174

```
The bottom picture is exactly what my settings were. I read about this before, religiously. :confused: About all the bugs, workarounds etc. and still got slapped. I will wait for the official statement. Having first ride ruin your life is kind of fucked to say the least.
```

---
## \#1111 Posted by: murloc992 Posted at: 2019-05-12T17:02:46.085Z Reads: 175

```
I can guarantee they will not respond. No liability. "You're just bad". Then apparently injured bad people start piling up because the perfect product is a flop. First ride with this deck, possibly last ride ever. I am grateful for this firmware bug.
```

---
## \#1112 Posted by: JKUK Posted at: 2019-05-12T17:20:06.417Z Reads: 178

```
Anyone know why I have one motor that accelerates more than the other? I have tried adjusting the belt which slightly improved however it is still an issue.

Also what are the mWb numbers for and does it matter that they are different?

![Screenshot_20190512-180218|236x500](upload://qFKFTLAgIzE239mKQ2AhvHgkaIk.jpeg) 


Thanks
```

---
## \#1113 Posted by: McErono Posted at: 2019-05-12T17:32:15.143Z Reads: 176

```
@JKUK Are you riding or just benchtesting? Numbers look good but try higher motor amps. If you are benchtesting its quite normal not to have in sync running motors.

@murloc992 30 motor amps and unsensored? Damn I will use my TB vescs until this shit is sorted.
```

---
## \#1114 Posted by: murloc992 Posted at: 2019-05-12T17:39:49.842Z Reads: 176

```
60 battery and 30 motor. Unsensored. Didn't even stutter from idle start. Apparently the hardest part was going at the same high speed for more than 10 seconds.
```

---
## \#1115 Posted by: Deodand Posted at: 2019-05-12T17:47:55.699Z Reads: 174

```
@murloc992 sorry to hear about your knee man. I've personally injured my shoulder on one of my DIY builds as well and it sucks. I understand your upset and I'm truly sorry if the unity played a part in it. 

That being said, it is a diy build and we'd need more information to figure out if that's exactly where the failure was.  The behaviour you describe of it just cutting out for no reason at speed is a bit different from the three other people we have with some cutout issues under acceleration. There is always a risk going the DIY route as it's impossible for us to test every possible setup that people might build. I know it's frusterating that the board failed on you but I do think pinning all blame on the unity without more investigation is unfair :man_shrugging:. But I get that the world sucks right now, hope your knee can makes a full recovery.
```

---
## \#1116 Posted by: murloc992 Posted at: 2019-05-12T17:53:34.393Z Reads: 170

```
I wish I could quote, but am on mobile.

I was accelerating the moment it cut off. This doesn't take me from the same group of people.

Also I wonder why I haven't heard about cutouts in other Vescs? People have died and never wrote to the forums again?

Also my planned settings were 120 batt and 60 motor when I wanted to test hill climb. Ofc it barfed at 50% of that while going straight. Would have been even more fun during the climb, huh. 

Also will you add the knee firmware upgrade guide? Your support might know sth about this funny encounter.

Edit:

Choose DIY, product tries to kill you, your fault. The bug will get fixed. Still your fault. All hail Enertion. The fire dousing is all you can do.
```

---
## \#1117 Posted by: Sender Posted at: 2019-05-12T17:54:08.631Z Reads: 166

```
I still think @Powadangaboardshas nicer legs.

But it might be nice to snuggle that big soft knee. Probably feels like a boob. Mmmmm.
```

---
## \#1118 Posted by: murloc992 Posted at: 2019-05-12T17:54:26.859Z Reads: 165

```
Motherducker. It's not really that soft. Tbh gelatinous.
```

---
## \#1119 Posted by: Deodand Posted at: 2019-05-12T17:56:22.763Z Reads: 166

```
@Toughook your settings look good to me. 

@JKUK accelerating more on the bench isn't an issue, but you should turn up your motor Amps from 10 I would guess. Does depend on your build but accel will probably be pretty weak I'd guess. 

@slydunan you can think of the motor controller as an inverter. So summing the motor currents to compare to the battery current only makes sense if they were at 100% speed. Essentially the power in needs to equal power out:

     Volts_batt*Current_batt = Volts1*current1 + Volts2 * current2

1 and 2 denoting motors 1 and 2.
```

---
## \#1120 Posted by: Sender Posted at: 2019-05-12T17:56:31.702Z Reads: 167

```
That's a bit disappointing TBH
```

---
## \#1122 Posted by: Kellag Posted at: 2019-05-12T18:58:49.201Z Reads: 168

```
Sender was about to buy a ticket to Lithiaunia 😆
```

---
## \#1123 Posted by: Quiles Posted at: 2019-05-12T20:34:26.762Z Reads: 166

```
i was about install Unity on my friends board...i think i will set aside for now.

@Deodand - I understand it's DIY world...but, is there something between the builds that can relate to each other? maybe motors?/batt's?/remote controller?etc...Any clue to begin to isolate the issue.
```

---
## \#1124 Posted by: murloc992 Posted at: 2019-05-12T20:37:20.998Z Reads: 166

```
He would be greatly underwhelmed by quality of the bike paths/sidewalks we have here. Beer and girls are another story tho.
```

---
## \#1125 Posted by: Sender Posted at: 2019-05-12T21:23:55.106Z Reads: 168

```
Are all the issues with people running 12s? Is that known?  Would be a good place to start...
```

---
## \#1126 Posted by: Toughook Posted at: 2019-05-12T21:29:22.813Z Reads: 169

```
I went for first proper test run tonight with the settings posted a little higher up thread. Whilst I'm OK and didn't fall, a couple of times at low speed i got some random acceleration 'twitches' which were very strange, and a little scary. 

'Fortunately, after reading the above posts, something else (mechanical) broke on my board forcing me to ditch that build into my car boot and grab my budget build for rest of evening.

Anyone else had these twitches ?
```

---
## \#1127 Posted by: SeanHacker Posted at: 2019-05-13T02:38:59.219Z Reads: 168

```
@Deodand

First and foremost, I love you. I think you're a major asset to this community and to Enertion. You've got a style that I like. You always seem open and honest. Got a serious question/questions dude. How much testing prior to release was done before sales of the Unity? Firmware, Software, and hardware? Is there anywhere we can see videos, pics, screenshots? What the process?
```

---
## \#1128 Posted by: banjaxxed Posted at: 2019-05-13T08:17:27.196Z Reads: 171

```
This is very unfortunate and probably avoidable had Enertion made available a simple test jig available to the developer

A frame with rollers that the driven wheels can spin. That has a hinge allowing it to be inclined on the forward end so as to simulate hills. Lastly a hydraulic jack inverted above with a padded board on a heim joint to simulate differing rider weight

Then go crazy after every F/W change 

After that JP full rider test, no helmet exception to pay for sins that must be atolled for

No idea where the .builders thread is
https://forum./t/esk8-dynometer-rolling-road/300?u=magharees

Hey @Blasto this looked very promising did you finish it? 

https://www.electric-skateboard.builders/t/esk8-dyno-testing/18168?u=banjaxxed

Another interesting idea
https://www.electric-skateboard.builders/t/electric-skate-bike-dyno-build/3167?u=banjaxxed
```

---
## \#1129 Posted by: Static Posted at: 2019-05-13T16:07:25.515Z Reads: 164

```
I think I have to add my anecdote to the mix. Last month I was testing a build using a 12s4p 30q+ unity + dual 6380s. I had a right side motor lock at speed that skewed the board and tossed me. It was so unexpected given the riding conditions that I assumed it had to be a phase short somewhere, but there was nothing. Starting to think it could have been the Unity. 

Still a bit worried to test this again even with the updated firmware

![image|347x500](upload://rAoiim3OxeUkcIhhwdzk72lJd64.jpeg)
```

---
## \#1130 Posted by: murloc992 Posted at: 2019-05-13T16:46:44.426Z Reads: 166

```
https://media.giphy.com/media/12NUbkX6p4xOO4/giphy.gif
```

---
## \#1131 Posted by: Deodand Posted at: 2019-05-13T21:13:40.014Z Reads: 166

```
@Static about 29 days ago we released a FW update which fixed most (but apparently not all) of the problems with larger motors. Were you running this latest FW when you experienced the issue? 

https://github.com/EnertionBoards/FOCBOX_UI/commits/FOCBOX_UI

I think we have found a solution to the cutouts a few people are experiencing but we are working on setting up/completing some more thorough testing to make sure it fully addresses the issue and doesn't introduce any other complications.

It's also important to separate out the issues, not everyone that experiences a cutout will have the root cause be the same thing. We all know how many different components within our boards can cause power drops: remote cutouts, loose wires connections, discharge BMS etc. The easiest way to identify if the unity is the root cause is to run "faults" in the terminal and post the result. The cutout issue we are working on a fix for is specifically related to the "ABS_OVER_CURRENT_FAULT".  

@SeanHacker I've been over a lot of the beta testing and stuff we did before launch you probably have read about it already, if not you can search through some of those old threads. I'm pretty comfortable with the amount of testing we did, of course more testing is always better  but unfortunately at some point you just have to launch the product. In hindsight I can see a few tests that could have identified some of the problem areas we have been wrestling with and in the future we will implement some processes to get better coverage of the diverse set of hardware the unity is used with.
```

---
## \#1132 Posted by: FranciscoV Posted at: 2019-05-13T21:20:23.087Z Reads: 169

```
Would any of these help!?  ![image|281x499](upload://z2D2IPTKM16OIpC3Chz7wkMndMe.png) ![image|281x499](upload://dwTJuxwFcVo2Ke02rpV8YE1Ctoy.png) ![image|281x499](upload://5TEsrX79Lg1ZGjcroi3KHqxjjxI.png)
```

---
## \#1133 Posted by: murloc992 Posted at: 2019-05-13T21:41:33.853Z Reads: 161

```
Nah, Enertion needs more blood, before testing measures are implemented. :sweat_smile:
```

---
## \#1134 Posted by: Static Posted at: 2019-05-13T22:17:31.609Z Reads: 164

```
I'm almost positive I wasn't running the updated firmware as this was just before the update release. My inspection of the board didn't reveal anything as a root cause visually- I'm fairly conscious of securing things well. Was puzzled for a while so it's good to have a potential fix.

Are faults stored between power cycles? If so, I'll check for faults.
```

---
## \#1135 Posted by: AndresIGC Posted at: 2019-05-13T22:28:17.960Z Reads: 160

```
What app and bt module are those?:grinning:
```

---
## \#1136 Posted by: Jinra Posted at: 2019-05-13T22:30:17.769Z Reads: 163

```
While I agree that Enertion should fix these problems, does no one remember all the problems with other iterations of non-focbox VESCs? They were plentiful with burning DRV's and the like all over the place. In 2017 my Ollin VESC failed hard and gave me a concussion that has had permanent effects on my brain. Issues like these have been around since the debut of the VESC.

This was that fall
https://www.youtube.com/watch?v=qATEOV21nxE
```

---
## \#1137 Posted by: FranciscoV Posted at: 2019-05-14T00:15:24.025Z Reads: 158

```
Xmatic app for iPhone n cheap hmsoft module 

App will also connect to stock unity module.
```

---
## \#1138 Posted by: huntercasillas Posted at: 2019-05-14T00:25:40.686Z Reads: 160

```
Will turning the motor amps down also reduce top speed?
```

---
## \#1139 Posted by: Deodand Posted at: 2019-05-14T01:00:35.528Z Reads: 166

```
Not by much. Current is proportional to torque and and speed to voltage. But obviously at max speed the motor has to overcome some resistance so if your max current is too low it can impact speed.
```

---
## \#1140 Posted by: huntercasillas Posted at: 2019-05-14T01:16:48.534Z Reads: 165

```
The acceleration is just way too much for me, but I’m comfortable going fast when it builds smoothly up to it. If my finger slips or moves too fast it’s dangerous. I’ve got 18t pulleys and 36t on the wheels. Today I accelerated too fast, fell forward and violently dislocated my arm from my shoulder. Got some nasty road rash too. I’m just scared and don’t know how to fix it to make it more safe. 

![image|505x500](upload://hOhadFKMBd26Nvyb9zJMWCTaim6.jpeg)
```

---
## \#1141 Posted by: Jinra Posted at: 2019-05-14T01:25:55.911Z Reads: 163

```
Lower your motor max man, or set your PPM min/max values to below what they actually are. Hope you recover well, and sorry to hear!
```

---
## \#1142 Posted by: venom121212 Posted at: 2019-05-14T01:31:37.691Z Reads: 169

```
Ouch!

Do you have the positive throttle ramping time option on your setup app? 

![Screenshot_20190513-213024|236x500](upload://4aaCH1PhHSJE3WVuf2vXf2DWzCe.jpeg)

I'd suggest making that longer (to the right)
```

---
## \#1143 Posted by: lrdesigns Posted at: 2019-05-14T01:41:22.644Z Reads: 169

```
For people with issue of GT2B going to throttle after 30sec or so when the board is turned on but not the remote. 

I have figured out the root cause of the issue after using GT2B for two years. I was very annoying until I got to the bottom of it, now it works perfect. The issue led to me almost running down a random pedestrian with the board going full zombie. 

The problem starts with custom cases and/or using the steering pot, the center point ends up being pretty far off 1500ms. And then the receiver has its own 1500ms fail safe if the remote is not turned on, this causes the issue.

If the board is turned on but NOT the remote, the programed fail safe is not activated, instead the gt2b receiver has its own fail safe that goes to 1500ms after 30 seconds or so, it can not be changed. If your vesc is not setup with 1500 as neutral it will go to throttle. But if you turn on the remote first it will use the fail safe you previously setup and will work fine with your vesc setup.

The ONLY way to solve the issue is to adjust the trim pots on the remote so that neutral is 1500ms, you may even need to adjust the internal trim pots. Then after that set up your vesc end points. Then set the fail safe button on the receiver.

Now if you turn on the board and not the remote, the receiver will go to 1500ms after some time and no problem will happen.

You can check the behaviour on the bench with wheels up while looking at the PPM mapping tab.
```

---
## \#1144 Posted by: huntercasillas Posted at: 2019-05-14T01:44:33.398Z Reads: 163

```
I don’t have that option no. I only have a Mac and iPhone. I tried to use a virtual machine to run the windows version but it never recognized the unity being connected.
```

---
## \#1145 Posted by: goldrabe Posted at: 2019-05-14T01:44:54.542Z Reads: 165

```
Yes my board with the Unity has jolts or twitches too. It feels like the throttle delays a bit. It's most apparent after coasting and accelerating after a push start. I thought it's related to remote, reciever and disassembled the board, couldn't find anything wrong with the reciever. The placement worked without any interference issues before. I set the board aside for now and will do the complete setup again when the next firmware update will be available.
```

---
## \#1146 Posted by: Jinra Posted at: 2019-05-14T01:45:02.868Z Reads: 161

```
If you can find someone with an android phone, it'll only take a sec to configure it
```

---
## \#1147 Posted by: huntercasillas Posted at: 2019-05-14T01:47:11.638Z Reads: 161

```
You’re also describing my experience, if I release the throttle and I’m coasting and want to go a bit faster it jolts when it starts to accelerate.
```

---
## \#1148 Posted by: huntercasillas Posted at: 2019-05-14T01:47:40.986Z Reads: 158

```
Yeah, but I won’t be riding for about a month so no rush haha
```

---
## \#1149 Posted by: Jinra Posted at: 2019-05-14T01:49:25.024Z Reads: 157

```
I think it'd be easier for all of us to understand if you can take a video of the issue. I havne't used the Unity on any DIY's but I've test rode a bunch of Raptor 2.1's without any of this "twitching" issue
```

---
## \#1150 Posted by: huntercasillas Posted at: 2019-05-14T01:54:49.688Z Reads: 155

```
Maybe it’s a hub vs belt situation since raptors have hub motors? I don’t know I can try but it’s dangerous to film that and I can’t until next month when I’m healed
```

---
## \#1151 Posted by: Jinra Posted at: 2019-05-14T01:55:47.904Z Reads: 156

```
Good luck with the recovery man :sweat: Maybe you can try filming sometime at low speed sitting down
```

---
## \#1152 Posted by: goldrabe Posted at: 2019-05-14T03:17:34.459Z Reads: 155

```
It will be not recognizable on video. The thing is if you push the throttle harder it gets less obvious. Since I didn't, don`t have this issue with my other VESC's it's not boosting my confidence.\
It could be something related to drive trains with gears, that was one of the issues I didn't had with the Raptor hubs.

*Edit @Deodand do you have any idea what could be the cause except PPM?
```

---
## \#1153 Posted by: Jinra Posted at: 2019-05-14T03:31:35.207Z Reads: 156

```
Maybe it's some kind of interference (maybe on the unity) that causes PWM signal to twitch up and down a bit from actual position? hmm

What remote are you using?
```

---
## \#1154 Posted by: Kellag Posted at: 2019-05-14T03:39:02.364Z Reads: 161

```
![This%20is%20fine%2013052019203837|606x420](upload://4SuH5r0cRB2UlqWN4CXYYm54QwE.jpeg)
```

---
## \#1155 Posted by: Balth81 Posted at: 2019-05-14T03:39:44.587Z Reads: 158

```
I also have had issues of cut outs under hard acceleration.. no accidents to date but sketchy as .. always when I am pushing it hard not even up hill. I am running 12s5p 30q with dual Tb 6374 190kv .. I thought it was just because I’m 120kg but apparently not ... I will try turning up the absolute max settings to see if it helps I have learnt to ride expecting it at some point I have done heaps on km’s on the unity and the cut out has only happened maybe 5 times .. usually when I am pushing the speed past 50km/h .. I am running latest firmware.. I also notice it tends to occur on long runs of acceleration as in not when I am racing around short streets turning and flooring to full throttle then braking hard and accelerating..
```

---
## \#1156 Posted by: FranciscoV Posted at: 2019-05-14T03:45:18.822Z Reads: 158

```
It sounds to me that you’re having the same issue as a few of us are.  Fault code Abs over current will shut off your power and launch off the board during hard acceleration making you kiss the ground pretty hard 
This is definitely becoming a big issue for unity users.  

I’d highly recommend unity users to turn down their settings and ride pretty damn conservative at least until the issue gets sorted out 

So far 2 serious injuries have been reported!  both both of them seem to have been related to the same issue.  @murloc992 and now @huntercasillas.   I got lucky I didn’t break anything during my fall!
```

---
## \#1157 Posted by: FranciscoV Posted at: 2019-05-14T03:46:18.597Z Reads: 157

```
Hahaha   You sure are very creative jr. 🤣🤣🤣
```

---
## \#1158 Posted by: Jinra Posted at: 2019-05-14T03:48:48.627Z Reads: 156

```
hunter's issue doesn't sound the same. He's not use the acceleration of higher powered ESCs like the VESC and its variants and has posted a lot on not being able to control hard acceleration.
```

---
## \#1159 Posted by: FranciscoV Posted at: 2019-05-14T03:51:52.597Z Reads: 157

```
[quote="huntercasillas, post:1140, topic:77861"]
Today I accelerated too fast, fell forward and violently
[/quote]
@Jinra I might be wrong but ☝️ That says otherwise
```

---
## \#1160 Posted by: Sn4pz Posted at: 2019-05-14T03:53:16.943Z Reads: 152

```
Sigh 

Do I really have to buy a 6.xx trampa vesc to feel safe 😫
```

---
## \#1161 Posted by: FranciscoV Posted at: 2019-05-14T03:58:21.570Z Reads: 154

```
That sounds about right 🤣🤣.
```

---
## \#1162 Posted by: goldrabe Posted at: 2019-05-14T04:04:49.237Z Reads: 155

```
I use the new Flipsky remote, will try to replicate the issue with the Nano X. Before the latest Unity firmware update I had issues with cogging at full speed, but those are gone now. Maybe it could also be sensor related because it's only noticeable at low speeds and after coasting.
```

---
## \#1163 Posted by: goldrabe Posted at: 2019-05-14T04:08:54.392Z Reads: 156

```
Just buy the ESCapes which are floating around, at 300$ for a dual it's a steal, by far the best ESC I have used. I wish @stewii would be still around here.
```

---
## \#1164 Posted by: Sn4pz Posted at: 2019-05-14T04:10:07.350Z Reads: 152

```
I really want to get rid of my Unity now, but I paid a little too much to sell it for any reasonable amount

My build is going to be done in a month and a half.... what are the odds this will be fixed by then 🤔🤔🤔 ( @goldrabe rhetorical obv, I don't expect you to have an answer)
```

---
## \#1165 Posted by: huntercasillas Posted at: 2019-05-14T04:18:11.485Z Reads: 150

```
I also use the VX1 remote
```

---
## \#1166 Posted by: Jinra Posted at: 2019-05-14T04:18:27.713Z Reads: 150

```
sure but he has a dozen other posts talking about how the remote is too sensitive. You can still be sent flying by not knowing how to properly stand or control the board.
```

---
## \#1167 Posted by: huntercasillas Posted at: 2019-05-14T04:21:54.576Z Reads: 157

```
That’s true I don’t know if it’s the same issue, but I’ve been riding for over a year with a boosted and hobbywing ESC and never had even close to a fall. Everything has been smooth as butter on those. I got into DIY so I could have a boosted with a larger battery, but doesn’t seem like any DIY VESC is the same as those two.
```

---
## \#1168 Posted by: goldrabe Posted at: 2019-05-14T04:23:15.661Z Reads: 157

```
The issues will be fixed for sure, with the small footprint and build in everything it can be a decent product. However Enertions resources are limited and this gets even more hampered by the issues they have with their suppliers for the Raptor. But as mentioned above, people should be made aware that the Unity is not safe for certain setups! They should have sent out a newsletter or warning mass mail.
```

---
## \#1169 Posted by: Jinra Posted at: 2019-05-14T04:24:01.917Z Reads: 159

```
It's hard to tell if it's a configuration issue, defective part, or user error for your setup. It'd be easier to help in person, but VESCs in general offer WAY more power than the hobbywing and boosted ESCs while maintaining an incredibly smooth throttle, but as you already know the way it delivers power is different than mosts ESCs. You very well might have a hardware defect, but it sounds like your issues are independent of Francisco's
```

---
## \#1170 Posted by: Andy87 Posted at: 2019-05-14T04:27:09.662Z Reads: 162

```
@lrdesigns i use only gt2b remotes and never had any issues besides that you need to program the fail safe ones. Good point, I will double check that in the evening. So, if I just switch on the board but not the remote the receiver sent his own fail safe signal after 30s right?

From where you bought your gt2b? Hobbyking or other source? I heard the hk gt2b are slightly different. Not sure in which points thou.
```

---
## \#1171 Posted by: Balth81 Posted at: 2019-05-14T04:28:11.952Z Reads: 157

```
Just ride it man.. seriously gear up and get on it .. I ride with the issues most days of the week and up till today didn’t know if it was unity or not.. I have done over 500km’s on it most of it riding at min 40-55km/h ... I know when it will likely kick(error out) so just be prepared when I am pushing it .. it has been reliable except for the 5 times it’s tried to buck me... nothing in life is perfect
```

---
## \#1172 Posted by: murloc992 Posted at: 2019-05-14T04:35:36.591Z Reads: 151

```
There's at least 4 versions of Gt2B. Some of them don't even have channel 3. Some of them have a non latching channel 3. Some of them have no failsafe, some have it slow, some have it instant. :smiley:
```

---
## \#1173 Posted by: Andy87 Posted at: 2019-05-14T04:38:48.046Z Reads: 153

```
Any way to identify which is which? Maybe via serial number or something?
```

---
## \#1174 Posted by: goldrabe Posted at: 2019-05-14T04:39:26.085Z Reads: 152

```
Then it might be related to the remote rather than the Unity. But my issue is different from yours. I can accelerate as smooth as with a boosted or hobbywing ESC. It's just those small delays, will see soon if it happens with the Nano X too. Your issue sounds more like it could be a calibration or setup problem.
```

---
## \#1175 Posted by: huntercasillas Posted at: 2019-05-14T04:45:56.055Z Reads: 150

```
I set it up and posted my configuration settings here and made them what was recommended for the remote, motor amps, throttle curve, and everything else.
```

---
## \#1176 Posted by: lrdesigns Posted at: 2019-05-14T04:52:51.649Z Reads: 156

```
It's only an issue if your remote control is not setup to the have the center point at 1500ms. So some people never have the issue. I think it more likely when you have a custom case or a thumb style case. 

Say you build a custom cased gt2b, its mid point is 1400 ms, then you adjust your vesc PPM range to make that work, all is good if you setup your fail safe by pressing the button on the receiver, this will make the fail safe 1400ms. But for reasons I can not figure out if the the remote is never turned on (but the board is) the receiver has its own fail safe of 1500ms that comes on by itself in around 30 - 60s if the remote is never turned on. 

I guess its not a dumb design if you assume no one is going to take the guts out and put it in a different case. 

Yeah I get my GT2B's from hobby king.
```

---
## \#1177 Posted by: murloc992 Posted at: 2019-05-14T05:03:15.486Z Reads: 154

```
Well. Turn the trim inside to make neutral 1500..? That way no discrepancy.
```

---
## \#1178 Posted by: lrdesigns Posted at: 2019-05-14T05:05:06.833Z Reads: 155

```
[quote="murloc992, post:1177, topic:77861, full:true"]
Well. Turn the trim inside to make neutral 1500…? That way no discrepancy.
[/quote]

Yes this is the fix. 

There is outer trims and if that is not adequate there is two internal trims.
```

---
## \#1179 Posted by: FranciscoV Posted at: 2019-05-14T05:08:16.923Z Reads: 156

```
Yeah.  It could very well be a different issue.  I still ride my board and everything seems to perform well! except for when I get on it too hard and HOLD it for a while.   But now I’m being extra cautious about it.  Heck.  Right before I ate it the other day I went up twin peaks @ full throttle most of the way going up and have had no issues    
Yesterday was trying to trigger the fault code by riding on grass from dead stop to 100% throttle and not once I was able to trigger the fault 
  My guess is that it happens once I hit certain speed at 100% throttle 🤷🏻‍♂️
```

---
## \#1180 Posted by: Jinra Posted at: 2019-05-14T05:09:06.949Z Reads: 155

```
I hear ya, ever since my concussion, I've been super wary of blasting the throttle.
```

---
## \#1181 Posted by: FranciscoV Posted at: 2019-05-14T05:14:04.996Z Reads: 154

```
😩😩😩 I have faith you guys will figure this one out!   I Freaken love my unities. They’re so damn easy to work with and convenient   I really don’t wanna go back to other vescs haha 
Till then conservative riding it is lol
```

---
## \#1182 Posted by: Deodand Posted at: 2019-05-14T05:15:24.482Z Reads: 154

```
Yeah guys, keep in mind that this is a support thread. There are A LOT of unities in the wild and we have maximum 10 people reporting about this issue, of which I think 3 have confirmed through fault codes the same issue that @FranciscoV is reporting.  This is DIY, glitches will happen whether they are due to the ESC, wiring, remote battery etc. Stay safe and always try to suit up especially on new untested builds. We all have a shared responsibility to try and make eskate as safe as it can be. @Blasto and I are hard at work doing some diagnostics on what's going wrong with this specific fault code.
```

---
## \#1183 Posted by: Andy87 Posted at: 2019-05-14T05:16:05.726Z Reads: 155

```
[quote="lrdesigns, post:1176, topic:77861"]
Yeah I get my GT2B’s from hobby king
[/quote]

alright, i keep that in mind and will double check that. just got a hk gt2b the last days i plan do make a mod for. good to know! thx!
```

---
## \#1184 Posted by: FranciscoV Posted at: 2019-05-14T05:17:23.731Z Reads: 155

```
Oh yeah.   For the record.  I’m not complaining.  I just want people to be aware of the issue we’re having with our unities and hopefully save someone from what could be a pretty ugly outcome!
```

---
## \#1185 Posted by: FranciscoV Posted at: 2019-05-14T05:22:05.451Z Reads: 154

```
Totally agree with you my brother and I understand exactly where you’re coming from!    We’re being patient because we know you guys are working on it and the problem will eventually get fixed 👍🏼
```

---
## \#1186 Posted by: Gerrycorrado Posted at: 2019-05-14T06:57:33.880Z Reads: 155

```
Keep in mind that not everyone will do the hassle of contacting you guys. Not everyone knows this site, has Facebook, speaks English,...
As ex TL of an international helpdesk (96% on CSQ's :stuck_out_tongue:), there is a huge difference between the helpdesk figures and real life (in my case corridor). People are lazy and some (i think a lot) will simply stop using your product when issues iso going through the lengthy process of having their item fixed. (i was at helpdesk 7 years, currently 13 years at the same client acting as release coord, so im the last step before software is pushed into live)
```

---
## \#1187 Posted by: RyuX Posted at: 2019-05-14T07:40:02.161Z Reads: 158

```
So since I am also waiting for my Unity to ship.. this thread made me kinda worry...

Is there a list or compilation of the faults with regards to battery/motor setup so we can collect some data and see if there is a pattern in any of the configurations/parameters or hardware ?

I really don't feel comfortable waiting for a firmware fix if there is a clear pattern then I will just change my board setup for the time being..

Have a good day
```

---
## \#1188 Posted by: Toughook Posted at: 2019-05-14T07:49:36.180Z Reads: 158

```
I use the Maytech Mini V2, the very same one I used on my previous dual Focbox CANbus setup. Never felt anything like this before. It happened three times, each twitch was whilst I was going slow (less than 10mph) and each time the twitch was instantaneous - in that it wasn't enough to throw me off, but required me to rebalance extremely quickly. I've skated all my life so was able to 'style it out' to a degree.... but it unnerved me to say the least. I haven't ridden it since so don't know if it's a consistent fault, or whether it was interference, but I ride the same place each time (the coastal path) and have never suffered interference before, making me think it's the unity since I have changed nothing else.

Like others I really want to like this vesc. It is small, the app is great and specs on paper at least suit my needs perfectly. I'm afraid that problems like mine are too sketchy and unscientific (in that I can only say what happened to me and the way it 'felt' rather than provide fault data or anything). How do Enertion go about fixing these sort of things ? I'm basically scared to ride it now, but will persevere, albeit in a full bubble wrap suit for the time being...... (full pads, body armour and helmet obvs)
```

---
## \#1189 Posted by: goldrabe Posted at: 2019-05-14T08:17:18.263Z Reads: 156

```
That describes exactly how it is, my board is stored away too.\
I will let you know how it turned out with the Nano X.  
@Jinra do you know if the Maytech and Flipsky remotes are a similar design?
```

---
## \#1190 Posted by: DJase Posted at: 2019-05-14T09:21:59.805Z Reads: 156

```
Well I'm waiting on my unity to ship as many here are and it will be for my first diy. I'm getting concerned there needs to be more beta testing before this unit is officially ready. Hardware or firmware if people are getting hurt due to the unity there should be some awareness from enertion even if it's only a dozen out of a thousand riders. I've been a skater for 10 years and I've never been scared of riding my boards because I can expect then to perform exactly how they always have. This makes me reconsider my purchase until the issue is locked down. If I don't know what to expect on each ride how can I feel comfortable and truly enjoy the product as intended. A sentiment I'm sure many of you share. I'm not trying to bash anyone but this seems like an important issue that can't just be glossed over and archived in this forum until fixed.
```

---
## \#1191 Posted by: Toughook Posted at: 2019-05-14T09:35:20.534Z Reads: 157

```
agreed ! I'm going to go out on one more ride with this unity. If I get just one more 'twitch' of the throttle that I didn't make myself then I'm going straight back to dual focbox over CAN until there's a firmware patch. I need the confidence I had with this previous setup if I'm going to ride fast again. I'm 45, a father and a business owner. Can risk that for a faulty vesc.
```

---
## \#1192 Posted by: Sn4pz Posted at: 2019-05-14T11:01:10.807Z Reads: 159

```
Have fun breaking your bones lmao

Take all the chances you want.... 🤔🤷
```

---
## \#1193 Posted by: murloc992 Posted at: 2019-05-14T11:14:14.727Z Reads: 159

```
You know how in Raptor commercial they say "Life's too short to push". Let's make it even shorter. :laughing:
```

---
## \#1194 Posted by: venom121212 Posted at: 2019-05-14T11:40:51.826Z Reads: 155

```
My batch 1 unity has had zero issues. It has worked flawlessly like I expected it to and I am more than happy with it. 

Just trying to even this thread out... Clearly people only come here to get support on issues and it sounds very negative around here.
```

---
## \#1195 Posted by: murloc992 Posted at: 2019-05-14T11:42:43.406Z Reads: 155

```
I mean, mine worked perfectly too until all planets aligned(acceleration, speed). I waited for the firmware update before testing even. It was not enough. I am not mad, I am disappointed(way too much hype). This can make people disabled, hurt, even killed. That's all.
```

---
## \#1196 Posted by: venom121212 Posted at: 2019-05-14T11:50:38.576Z Reads: 157

```
I feel you and it sucks. Please don't take any of my comments personally, I'm only observing from the outside. I generally like you and your humor style.

Again, not referring to your case personally: I know that there are sudden cutouts that happen on builds without unities as well. It will be interesting to see how many of these incidences can be fixed via unity FW update and how many are caused by any of the other number of reasons a cutout could happen. 

I know your wiring is perfect, it's the *others* I worry about.

https://giphy.com/gifs/adventure-time-jake-55LHldKfHj4be
```

---
## \#1197 Posted by: murloc992 Posted at: 2019-05-14T11:56:55.228Z Reads: 158

```
I didn't take it personally, I evened it out(you could say we stand at the both edges of being skeptical about which side is actually bad, I got hit, you try to find out wtf, both irritated somewhat). :smiley: 

I just hope by the time I (and @Powadangaboards , the guy who got it three times and didn't learn) heal there will be a FW update that addresses this cutout issue. If there's none, I will sell my platinum warranty first batch unity with XT90 and 12AWG motor wires to somebody else. :smiley: I still loved it tho. Just my smile was quickly turned upside down. :smiley:

Also wiring, there's not that much wiring if I recall correctly. That's a perfect thing about it. Small, everything is there to just plug in and use. :smiley:  

My board is being ridden by a friend now, he didn't try going above 45, so he still didn't cut and soaked all the enjoyment I could have :frowning: Seems to be related to speeds over 50..

_Wait.. my unity is the special edition.._
```

---
## \#1198 Posted by: Balth81 Posted at: 2019-05-14T12:17:39.583Z Reads: 157

```
Mine is first edition and it cuts at speed my mates whose is also first has no issues he is running same battery and motors he has ridden at 65km/h for good lengths so not sure what the deal is except that he is 30kg lighter than me which is why I put it down to load..
```

---
## \#1199 Posted by: murloc992 Posted at: 2019-05-14T12:18:36.359Z Reads: 157

```
[quote="Balth81, post:1198, topic:77861"]
except that he is 30kg lighter than me which is why I put it down to load…
[/quote]

Well I am kind of THICC too, 90KG. Friend is way lighter. Might be load too. :thinking:
```

---
## \#1200 Posted by: Jinra Posted at: 2019-05-14T13:09:13.999Z Reads: 156

```
I don't use the maytech remotes so not sure, but pretty sure it's a different oem
```

---
## \#1201 Posted by: FranciscoV Posted at: 2019-05-14T13:34:32.157Z Reads: 158

```
🤣🤣 ![image|480x358](upload://ohR8McaMmUDHk0HLTPUjFqxvKIf.gif)
```

---
## \#1202 Posted by: murloc992 Posted at: 2019-05-14T13:40:05.935Z Reads: 158

```
When you get close to advertised power figures Unity goes:

https://media1.tenor.com/images/50fc2e15ea8c697e054d91a33810f6d4/tenor.gif?itemid=12272844
```

---
## \#1203 Posted by: venom121212 Posted at: 2019-05-14T13:50:30.598Z Reads: 159

```
70kg rider, 10s battery data point here.

Bring on all the statistics!
```

---
## \#1204 Posted by: Toughook Posted at: 2019-05-14T13:56:49.800Z Reads: 157

```
95kg rider, 10s battery. 

Got the acceleration "twitches". At low speed, low accel.
I haven't pushed for top end yet so can't comment on the other cut outs people are posting.
```

---
## \#1205 Posted by: murloc992 Posted at: 2019-05-14T13:58:19.445Z Reads: 158

```
90kg rider, 12s battery.

S A D B O I S kind of results.
```

---
## \#1206 Posted by: epss4 Posted at: 2019-05-14T14:54:25.275Z Reads: 155

```
12s5p/ 80kg  /raptor 2.1 motor 
No problem at all
```

---
## \#1207 Posted by: linsus Posted at: 2019-05-14T15:11:56.889Z Reads: 158

```
Hmm, for the people that had failures at higher speeds/power, do you run belt setups?
```

---
## \#1208 Posted by: murloc992 Posted at: 2019-05-14T15:12:19.961Z Reads: 157

```
Belts for now, was aiming at chains later.
```

---
## \#1209 Posted by: linsus Posted at: 2019-05-14T15:16:32.009Z Reads: 157

```
I've kinda avoided getting into a discussion about this cause this is a enertion forum and I normally keep my drama to a minimum. But since people are getting hurt.

But when disscussing the unity hardware design with Vedder long time back he was abit surprised that the unity managed to keep up with the number of calculations per second, given that it runs a single MCU for two motors. A belted setup naturally has a bigger calculative load since it spins faster than a hub motor and I quote: "It should probably be fine for a hub motor tho, which I guess is thier main use"

Thats the reason for the previous question. Only a theory tho, I have 0 proof.
```

---
## \#1210 Posted by: murloc992 Posted at: 2019-05-14T15:17:36.627Z Reads: 154

```
https://media.tenor.com/images/457e9a1149ebf9426938f45ca61d5cbf/tenor.gif

I mean 168kV motors with 15:60 gearing, with 154mm wheels hit ~57k ERPM. Would this still hurt?
```

---
## \#1211 Posted by: Jinra Posted at: 2019-05-14T15:21:02.309Z Reads: 152

```
Interesting, though it doesn't explain the low speed jitters that some are experiencing.
```

---
## \#1212 Posted by: murloc992 Posted at: 2019-05-14T15:21:42.607Z Reads: 152

```
But might explain high speed crap outs when ERPM hits bigger numbers.

But still, I haven't heard of the bioboards guys dying. They hit 85KM/h.
```

---
## \#1213 Posted by: taz Posted at: 2019-05-14T15:23:33.023Z Reads: 151

```
Actually, I recall he did have an accident due to a cutout and broke something.
```

---
## \#1214 Posted by: Toughook Posted at: 2019-05-14T15:23:47.625Z Reads: 156

```
[quote="murloc992, post:1212, topic:77861"]
I haven’t heard of the bioboards guys dying. They hit 85KM/h.
[/quote]


This is precisely what is puzzling me. These guys are running 4wd Unity setups on perhaps the most expensive and high performing board out there to buy off the shelf right now. All 6374 Dual (x2) geared drives. Surely someone would have karked it by now if they were playing up that badly. What's their secret ?
```

---
## \#1215 Posted by: murloc992 Posted at: 2019-05-14T15:23:52.820Z Reads: 155

```
Wot. I missed that then. Sad.. :frowning:
```

---
## \#1216 Posted by: taz Posted at: 2019-05-14T15:24:38.940Z Reads: 158

```
https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/616?u=taz

To clarify, I have no idea if it was the Unity's fault.
```

---
## \#1217 Posted by: Jinra Posted at: 2019-05-14T15:25:47.567Z Reads: 159

```
to be fair a 4wd setup is running 2 MCUs
```

---
## \#1218 Posted by: murloc992 Posted at: 2019-05-14T15:25:51.905Z Reads: 159

```
I think that's the old bug that was presumably fixed with the latest update.
```

---
## \#1219 Posted by: Toughook Posted at: 2019-05-14T15:26:31.175Z Reads: 159

```
[quote="taz, post:1216, topic:77861"]
its only on this board and no other board I have with Unity so I start to think it’s just this Unity
[/quote]


well I have a spare Unity in the drawer. Maybe I should swap it out and try to replicate things with that ? The problem one is from the very first batch (I ordered on day#1) and the other is from a Black Friday deal..... ?
```

---
## \#1220 Posted by: taz Posted at: 2019-05-14T15:27:25.304Z Reads: 158

```
Don't quote me. This post was by @mackann .
```

---
## \#1221 Posted by: Toughook Posted at: 2019-05-14T15:27:55.606Z Reads: 157

```
I quoting your quote :-)
```

---
## \#1222 Posted by: craigthemachine Posted at: 2019-05-14T16:28:59.928Z Reads: 160

```
Let’s make that 3 injuries. I had this happen to me, couple weeks back. Got road rash but recovering fairly good.
```

---
## \#1223 Posted by: craigthemachine Posted at: 2019-05-14T16:30:36.879Z Reads: 162

```
![image|375x500](upload://fqkVKNcedNNnHTC9yUIM3J1bF1D.jpeg) ![image|281x500](upload://y5PHrapILkzNaXaWHjO87XvXqHM.jpeg)
```

---
## \#1224 Posted by: FranciscoV Posted at: 2019-05-14T16:31:31.408Z Reads: 162

```
In the other hand.   Problem seems more visible when switching over to higher kv motors.   In my case went from 170kv to 190kv n that’s when hell broke loose!!
```

---
## \#1225 Posted by: FranciscoV Posted at: 2019-05-14T16:34:54.249Z Reads: 161

```
Damn!   That looks painful brother.   I got some of that myself but not as bad as you did 😬
```

---
## \#1226 Posted by: murloc992 Posted at: 2019-05-14T16:36:39.241Z Reads: 162

```
Higher KV means more ERPM. Does that mean that the MCU cannot keep up? Only the guys who made it work will tell..
```

---
## \#1227 Posted by: FranciscoV Posted at: 2019-05-14T16:40:17.106Z Reads: 162

```
I think it will be just fair that enertion focuses into fixing the issue and give us all a new raptor each for our troubles 🤣🤣
```

---
## \#1228 Posted by: murloc992 Posted at: 2019-05-14T16:44:11.433Z Reads: 161

```
I'd be happy if they just paid my MRI and ER bills. :smiley:
```

---
## \#1229 Posted by: FranciscoV Posted at: 2019-05-14T16:45:47.595Z Reads: 162

```
I’ll sell my raptor once I get it and give the money to help pay for your medical expenses lmao
```

---
## \#1230 Posted by: craigthemachine Posted at: 2019-05-14T16:46:13.333Z Reads: 162

```
Yea could have been worse, I can’t stress the importance of a helmet and safety gear. Lucky I wore my Kevlar jeans. I’m actively watching this trend for a solution. For now, I’m NOT using the board with the unity. Thankfully I have 3 other boards to choose from 😜. Stay safe people.
```

---
## \#1231 Posted by: Deodand Posted at: 2019-05-14T16:51:54.858Z Reads: 166

```
It isn't a problem with erpms, we've tested well beyond anything you guys are hitting. The MCU has plenty of cycles to manage both motors as it runs two different alternating controllers at 10kHz (20 kHz pwm) . For reference a standard vesc can easily run a control loop at around 35 kHz (70 kHz pwm).  There is still about 40 percent of the CPU left available even when spinning two motors. The CPU cost doesn't change as erpms increase. I dove very deep into this topic when I first started designing the unity.

The reason we are seeing faults on higher kv motors has to do with the motor time constant. The lower this number is the faster the time constant of the motor and the sharper the current spikes can be in the windings. Since the ABS_OVERCURRENT fault has to do with a large measured current spike it makes sense that large and high kv motors which have lower winding resistance and high inductance are susceptible. Tuning the current controller bandwidth of these larger motors has shown effective in testing at eliminating the spikes but we are just working to get some more test results to confirm the initial findings.

Writing this quickly from my phone so apologies if there's small errors.

Also just to be clear we have loads of people running 8085s and 6374s 190kv on belts with high amperage with no over-current behaviour present. We will get this sorted though 👍
```

---
## \#1232 Posted by: huntercasillas Posted at: 2019-05-14T17:21:50.606Z Reads: 164

```
I feel you man, this is what my arm looks like too but I can’t take a picture since it was dislocated and is bandaged up in a sling.
```

---
## \#1233 Posted by: murloc992 Posted at: 2019-05-14T18:14:59.279Z Reads: 169

```
@Deodand

I don't know if you seen this, but this happened straight after the cut-off:

[quote="murloc992, post:6496, topic:63248, full:true"]
The cogging part was interesting tho. It cogged both motors even if I held the motors by hand or didn’t with the board upside down, no matter the throttle amount. Cogging was more intense at 100% of throttle. Then I headed to the ER, wasn’t feeling like making a video of the cogging for some reason.
[/quote]

After the cutoff the board couldn't ride and cogged at any throttle(increasing cogging intensity (identical on both motors) with throttle, even without load) until reconnecting the battery or restarting the unity, unsure. Couldn't really focus myself then.
```

---
## \#1234 Posted by: Deodand Posted at: 2019-05-14T18:29:05.868Z Reads: 165

```
Thanks for the info... that is strange indeed. Do you have traction control enabled? There really shouldn't be any memory effects on the unity side which would cause cogging after a fault, but it is possible the DRV latched a fault so one motor would not spin at all and the second one would be speed limited due to traction control I guess. But from your description this doesn't sound accurate.
```

---
## \#1235 Posted by: murloc992 Posted at: 2019-05-14T18:30:33.465Z Reads: 160

```
I had default traction control enabled, so nothing custom. It's really weird. I was hoping I will ride back while adrenaline lasts, but I couldn't. :confused: My friend is using the board for two days now, no major speeds over 45 and nothing happened, he weighs less tho.
```

---
## \#1236 Posted by: Deodand Posted at: 2019-05-14T18:31:24.552Z Reads: 162

```
When you noticed this cogging, did both wheels seem to be spinning/cogging?
```

---
## \#1237 Posted by: murloc992 Posted at: 2019-05-14T18:33:22.066Z Reads: 170

```
When I walked to the board which just stood there and pretty much mocked me. :smiley: I slid/sprinted 100+ meters, then walked(crawled) back. When I came back I stood on it and it stuttered more intensively regarding to throttle and didn't move. I flipped it upside down because of frustration and pain, it cogged the same. I held one motor, other one spun, cogged, spun, cogged. I released the motor I held, both cogged in the speed of the throttle. Weird a f.
```

---
## \#1238 Posted by: Deodand Posted at: 2019-05-14T18:36:49.185Z Reads: 169

```
Can I organize a new replacement unity shipped to you and you mail me yours? Memory effects like you describe might indicate something electrically amiss. Chances are its fine but I want to inspect it myself and see if there's anything amiss and on the off chance anything is you will have a new and properly working one.
```

---
## \#1239 Posted by: murloc992 Posted at: 2019-05-14T18:38:56.507Z Reads: 169

```
I mean I could, but this will cost us both a lot.. Remember a 260€ unity cost me 400€ because of import taxes, I bet shipping back to Australia will not cost below 40€ at least. We can organize this ofc, I just hope I will not lose more time because of that, I am still in healing, but you know..

Best to hit me on PM I guess.
```

---
## \#1240 Posted by: FranciscoV Posted at: 2019-05-14T18:46:53.010Z Reads: 162

```
That exact same thing happened to my unity twice in one day.    Shit was running and for no reason it went back to default settings where I had to reconfigure the whole thing.   Once after I did the settings with my buddy’s pc and another time through the app.
```

---
## \#1241 Posted by: AgressivStreetLamp Posted at: 2019-05-14T22:19:06.940Z Reads: 161

```
Should I be worried?
Planning to build a MTB with dual 7374, @149 KV.... Mostly for dirt trail shenanigans.
Is this thing gonna kill me? 
What are alernatives? two single focbox?
```

---
## \#1242 Posted by: RyuX Posted at: 2019-05-14T23:57:59.046Z Reads: 160

```
I guess reading all of this lower KV Motors should be "safer".
Also if you have a MTB you also have a binding and will not fly off directly when you get a cutout.
Just remember to wear safety gear until everything is figured out.
```

---
## \#1243 Posted by: Powadangaboards Posted at: 2019-05-15T14:32:47.388Z Reads: 159

```
its really putting a shitter on the completion of my board..... i have check everything time and time again, connections, making sure the motors are connected correctly, making sure theirs no damage to any wires!? just makes me not want to ride it!
```

---
## \#1244 Posted by: Powadangaboards Posted at: 2019-05-15T14:34:23.716Z Reads: 162

```
i run belt setup yes
```

---
## \#1245 Posted by: Powadangaboards Posted at: 2019-05-15T14:38:26.882Z Reads: 164

```
Fuck..... :/ i hope your recovering quick dude....
```

---
## \#1246 Posted by: craigthemachine Posted at: 2019-05-15T14:52:46.667Z Reads: 162

```
Thanks bro. I’m about 90% recovered. 👊🏽
```

---
## \#1247 Posted by: Powadangaboards Posted at: 2019-05-15T15:04:57.848Z Reads: 161

```
i would like to do the same if possible?
```

---
## \#1248 Posted by: MrDGOrman Posted at: 2019-05-15T15:06:41.585Z Reads: 158

```
I've heard people having problems with the Unity and their 12s battery packs? Motors cutting off randomly etc.

I'm trying to see if getting a Unity would be worth while or if getting another single FOCBOX would be better?
```

---
## \#1249 Posted by: Powadangaboards Posted at: 2019-05-15T15:07:02.381Z Reads: 157

```
Another thing i forgot to mention after the cutout, the remote setting were all reversed? i have to re-calibrate to get them correct.
```

---
## \#1250 Posted by: AgressivStreetLamp Posted at: 2019-05-15T16:37:36.747Z Reads: 155

```
Wondering the same thing. It doesnt sounds like people are having issues with dual focbox setups
```

---
## \#1251 Posted by: murloc992 Posted at: 2019-05-15T16:39:26.729Z Reads: 156

```
Sadly, as harsh as it sounds, I think the 'ol reliable name of the original FocBox was used as bait to market/sell Unity. The first one was good, how could the second one be even a bit worse(Hype: Engaged)? People really assumed the same, even better levels of reliability and performance for sure. :confused:
```

---
## \#1252 Posted by: AgressivStreetLamp Posted at: 2019-05-15T16:41:32.201Z Reads: 151

```
If I preordered last week, which generation am I getting? Any idea:?
```

---
## \#1253 Posted by: murloc992 Posted at: 2019-05-15T16:42:28.028Z Reads: 152

```
Batch 3 or 4.
```

---
## \#1254 Posted by: MrDGOrman Posted at: 2019-05-15T16:42:34.112Z Reads: 157

```
So basically, those who have the Unity feel it's actually a little bit under rated and not as good as hyped? Maybe it'll be worth it in 6 months time when they've got rid of the original stuff, but for now - classic single drive FOCBOXs are better?
```

---
## \#1255 Posted by: FranciscoV Posted at: 2019-05-15T16:44:27.969Z Reads: 155

```
It’s getting hot in here 🤣🤣
```

---
## \#1256 Posted by: FranciscoV Posted at: 2019-05-15T16:51:04.647Z Reads: 156

```
Let’s be patient guys.   @Deodand is working on a solution to the issues.    He has updated my unity with an experimental fw and so far so good.  Need to put some more time on my board to make sure the problem has been taken care of
```

---
## \#1257 Posted by: Battosaii Posted at: 2019-05-15T17:01:42.986Z Reads: 156

```
I have a Unity from batch 1 and i absolutley love it and can see everywhere the original Focbox was improved. I also have a unity from batch 2 but its still in the box i have not installed it yet i hope nothing is wrong with it.
```

---
## \#1258 Posted by: murloc992 Posted at: 2019-05-15T17:07:51.290Z Reads: 154

```
I don't think you will see issues if you don't push it. Pushing = 12S and quite a bit of acceleration and high speed. Let's just see if experimental changes fixes that. I might eat my knee, but I am still quite afraid to stand on the board again, just because a Unity is there. I haven't ever bailed so hard in my life, so I am a bit spooked for the future of using it.
```

---
## \#1259 Posted by: Jinra Posted at: 2019-05-15T17:10:55.075Z Reads: 156

```
I honestly don't think it has anything to do with 12s, just high current; or rather, false positives for over current. Either on 10s or 12s, hard acceleration **or** high speeds can trigger OC faults as I experienced my Ollin VESC. Perhaps the issue is exacerbated by high eRPM, but again, high eRPM is not exclusive to 12s.

Fixes are underway guys, let's hold the pitchforks until then.
```

---
## \#1260 Posted by: murloc992 Posted at: 2019-05-15T17:12:26.990Z Reads: 161

```
[quote="Jinra, post:1259, topic:77861"]
Fixes are underway guys, let’s hold the pitchforks, until then.
[/quote]

http://pitchforkemporium.github.io/products/

You can always pre-oder some pitchforks. :smiley:
```

---
## \#1261 Posted by: FranciscoV Posted at: 2019-05-15T17:18:40.717Z Reads: 158

```
Yup.   You’re 100% right     And that’s all I have left to do.   Accelerate from 0 to at least 35mph 😬
Falling because of a faulty unit can be traumatizing lol
```

---
## \#1262 Posted by: murloc992 Posted at: 2019-05-15T17:19:39.758Z Reads: 160

```
So you're telling me, they forwarded the testing to you? I'd prefer to see enertion guys testing this on their own fur, not on "beta-testers" aka clients. :thinking:
```

---
## \#1263 Posted by: FranciscoV Posted at: 2019-05-15T17:21:18.498Z Reads: 162

```
Haha.   I just happen to be near by and know a couple of people who work on these issues.  That’s all.
```

---
## \#1264 Posted by: murloc992 Posted at: 2019-05-15T17:22:18.541Z Reads: 164

```
I just hope you're well equipped:

![image|500x500](upload://bicFehHYySoSrVJteTtOlmZCLaY.jpeg)
```

---
## \#1265 Posted by: FranciscoV Posted at: 2019-05-15T17:22:50.096Z Reads: 160

```
In fact.   If enertion wants my board to conduct further testing I’ll be more than happy to have it shipped anywhere within the states haha
```

---
## \#1266 Posted by: Jinra Posted at: 2019-05-15T17:25:13.064Z Reads: 163

```
If they wanted to test it they'd probably tell you to give it to me or sophia
```

---
## \#1267 Posted by: FranciscoV Posted at: 2019-05-15T17:27:49.081Z Reads: 160

```
Hahah.  You’re right.   Do you want it??  😁
```

---
## \#1268 Posted by: Jinra Posted at: 2019-05-15T17:30:21.538Z Reads: 160

```
I'll let you know if Jeff wants us to test it.
```

---
## \#1269 Posted by: Battosaii Posted at: 2019-05-15T17:50:28.554Z Reads: 160

```
Yea not pushing it is not me lol

12s8p, 4wd 6374 lol
```

---
## \#1270 Posted by: murloc992 Posted at: 2019-05-15T18:00:17.222Z Reads: 162

```
I mean, you might as well just learn to fly with a sweet ride like that. :smiley:
```

---
## \#1271 Posted by: Battosaii Posted at: 2019-05-15T18:36:22.765Z Reads: 160

```
Well for testing id rather put the batch 2 focbox for the rear motors and my tested good one up front. Having a front wheel lock up can be deadly while you can sometimes ride out a rear lock up depending on speed.
```

---
## \#1272 Posted by: Sn4pz Posted at: 2019-05-15T18:40:53.989Z Reads: 156

```
Will you swap the motors to the front as well? That might play an important role in isolating the issue
```

---
## \#1273 Posted by: Battosaii Posted at: 2019-05-15T19:14:38.015Z Reads: 162

```
Well i never had an issue im just worried i will and id rather the rear lock up. Front motors have been ridden on for a while they work fine.
```

---
## \#1274 Posted by: murloc992 Posted at: 2019-05-15T19:16:18.771Z Reads: 161

```
Just turn the board around and change the spinning direction. :smiley:
```

---
## \#1275 Posted by: Skunk Posted at: 2019-05-15T19:51:16.930Z Reads: 160

```
[quote="Battosaii, post:1271, topic:77861"]
Having a front wheel lock up can be deadly while you can sometimes ride out a rear lock up depending on speed.
[/quote]

The one thing that worries me about my fwd build lol
```

---
## \#1276 Posted by: taz Posted at: 2019-05-15T19:58:48.830Z Reads: 163

```
In that case you just:

https://youtu.be/c1f7eZ8cHpM?t=167
```

---
## \#1277 Posted by: venom121212 Posted at: 2019-05-15T21:04:08.915Z Reads: 161

```
I love my unity. There has been a small number of issues. Unfortunately these issues seem to only manifest at high speed. I accelerate quite quickly and go much zoom and have had no issue. It is a wonderful piece of equipment in my book / experiences.

I believe it's 3 or 4 unities who have had this issue out of all the ones sold (that number, I do not know).

@Deodand any way we can get a ballpark percentage fail rate?
```

---
## \#1278 Posted by: McErono Posted at: 2019-05-15T21:19:34.762Z Reads: 163

```
I still have jerkiness like cutouts while hitting full throttle at standstill with my unity/torqueboards DD combination but I had a look into the terminal/faults tab and no fault was registered.

the reported issues kind of ruin the ride... it’s always in the back of my head while riding :pensive:
```

---
## \#1279 Posted by: Jinra Posted at: 2019-05-15T21:22:22.267Z Reads: 158

```
How do the cutouts behave? Like you full throttle then the board cuts out and does nothing while you're still holding full throttle? Or is it momentary? Or some other behavior?
```

---
## \#1280 Posted by: goldrabe Posted at: 2019-05-15T21:22:27.604Z Reads: 163

```
Does it feel like a delay in throttle?
```

---
## \#1281 Posted by: goldrabe Posted at: 2019-05-15T21:25:22.625Z Reads: 164

```
There are more then that, but most got fixed after the last firmware update. Even some Raptor 2.1 had this issues.
```

---
## \#1282 Posted by: McErono Posted at: 2019-05-15T21:30:33.752Z Reads: 159

```
full throttle, board accelerates for like a second then the cutout happens. very short like a tenth of a second but creates a hard jolt. then it continues accelerating. Most of the time it feels like just happening on one motor. during the cutout the motor makes this bangging sound.
```

---
## \#1283 Posted by: Jinra Posted at: 2019-05-15T21:39:19.274Z Reads: 165

```
Sounds like perhaps a sensor isn't reading correctly. Do you have a picture or settings of the sensor values handy?
```

---
## \#1284 Posted by: McErono Posted at: 2019-05-15T21:45:59.842Z Reads: 165

```
Yes. As long as I am not hitting full throttle the acceleration is perfectly smooth not like unsensored.

![Screenshot_20190418-215819|243x500](upload://jpLAp6uiZBYaK1DH4Uv4KkBWTIo.jpeg)
```

---
## \#1285 Posted by: Jinra Posted at: 2019-05-15T21:52:37.067Z Reads: 165

```
Hm.. looks normal. I'm able to blast the throttle on all the raptors I've test ridden so far, but they have lower resistance (and maybe inductance) than yours.
```

---
## \#1286 Posted by: McErono Posted at: 2019-05-15T21:53:45.557Z Reads: 165

```
I had a raptor 2.1 in january with a few issues but there were no cutouts at all.
```

---
## \#1287 Posted by: venom121212 Posted at: 2019-05-15T21:57:41.754Z Reads: 167

```
I feel like many separate issues are being lumped into your definition of "this issue"

The issue in question is high kv motor specific, not raptor and unity in general having any problem.
```

---
## \#1288 Posted by: Deodand Posted at: 2019-05-15T21:58:12.376Z Reads: 165

```
You may want to play with the sensorless ERPM transition in the full tool... I'm going to add the setting to the app next release with the patch for the ABS_OVER_CURRENT
```

---
## \#1289 Posted by: goldrabe Posted at: 2019-05-15T22:20:30.679Z Reads: 167

```
No I am referring to this specific issue with cutouts after hard acceleration. Not all people reported their problems here.\
As for the Raptor owners Enertion was generous enough to inform them to update their firmware for safety via Instagram.\
It's good that you like the Unity, I like this ESC too, I think it's still better to make people cautious then to tell everything is alright to avoid future injury.
```

---
## \#1290 Posted by: venom121212 Posted at: 2019-05-15T22:25:54.204Z Reads: 168

```
[quote="goldrabe, post:1289, topic:77861"]
better to make people cautious then to tell everything is alright to avoid future injury
[/quote]

Assuming these are the only 2 options in this conversation is a problem of its own. I think what I requested earlier was entirely fair: the accurate number of unity failure rates. Data and science!
```

---
## \#1291 Posted by: Powadangaboards Posted at: 2019-05-16T06:52:31.396Z Reads: 170

```
Im in the same boat bro! i think ill go back to cycling my bike until the issue is resolved!
```

---
## \#1292 Posted by: Powadangaboards Posted at: 2019-05-16T06:57:53.538Z Reads: 170

```
this is exactly what happened to me 3 times. a very quick and hard jolt that sent me soaring like an eagle!!
```

---
## \#1293 Posted by: murloc992 Posted at: 2019-05-16T07:04:52.306Z Reads: 173

```
I wonder if having a foot binding(no heel, just a slide-in bind) would help in this situation if the board actually recovers after the sudden jolt?
```

---
## \#1294 Posted by: Powadangaboards Posted at: 2019-05-16T07:13:17.403Z Reads: 176

```
would be a great way to whip lash!
```

---
## \#1295 Posted by: murloc992 Posted at: 2019-05-16T07:14:53.229Z Reads: 173

```
Ah, right.. Sad. :smiley:
```

---
## \#1296 Posted by: murloc992 Posted at: 2019-05-16T08:01:11.484Z Reads: 169

```
Add ability to limit max speed while you're at it. :slight_smile:
```

---
## \#1297 Posted by: Knaspast Posted at: 2019-05-16T08:10:38.268Z Reads: 169

```
What would you guys estimate that the delivery time would be if i ordered it yesterday? Any timeframe at all would be appreciated.
```

---
## \#1298 Posted by: sybercid Posted at: 2019-05-16T08:45:21.306Z Reads: 174

```
I asked the same question last week with the live chat thing on their website. The exact quote was

"If you order now, you will get it by End of June hopefully"
```

---
## \#1299 Posted by: Knaspast Posted at: 2019-05-16T08:58:00.329Z Reads: 173

```
Alright, a bit long then, but reasonable i suppose. Cheers
```

---
## \#1300 Posted by: Andy87 Posted at: 2019-05-16T09:32:37.292Z Reads: 174

```
[quote="Deodand, post:1231, topic:77861"]
Also just to be clear we have loads of people running 8085s
[/quote]

@Deodand i guess the people running a unity on 8085 motors are not from the forum? any changes? I really would like to have a small conversation with one or the other, as I´m owner of 8085 motors as well, so I´m interested what there thoughts about this combination.
```

---
## \#1301 Posted by: venom121212 Posted at: 2019-05-16T11:47:58.698Z Reads: 166

```
Just mentally preparing you to expect mid July based off the prior track record of batches. I hope I'm wrong!
```

---
## \#1302 Posted by: ducktaperules Posted at: 2019-05-16T11:55:31.750Z Reads: 165

```
I agree with @venom121212 in my experience . . .

_"get it by end of June"_ 

roughley translates to  . . . 

_"we will have STARTED shipping orders from this batch by end of June , but it may take a few weeks for us to ship the whole batch and it will take another week or so in shipping"_
```

---
## \#1303 Posted by: linsus Posted at: 2019-05-16T12:06:38.604Z Reads: 165

```
They didint specify which year. Thats the trick ;)
```

---
## \#1304 Posted by: McErono Posted at: 2019-05-16T12:39:25.997Z Reads: 166

```
anyone with an idea why that is? why would it take so long to manufacture a batch of unitys... I'm not saying it :wink:
```

---
## \#1305 Posted by: Andy87 Posted at: 2019-05-16T12:41:15.224Z Reads: 171

```
the quality control takes ages... you know.... :tipping_hand_man::stuck_out_tongue_winking_eye:
```

---
## \#1306 Posted by: murloc992 Posted at: 2019-05-16T12:57:30.444Z Reads: 173

```
[quote="Andy87, post:1305, topic:77861"]
quality control
[/quote]

Sorry, what is quality control again? That dirty sticker under the Unity, same like on things from Wish?

![Screenshot_20190516-160121|281x500](upload://vFpDh8T6j3JyIyDCcLaB80kJsnz.png)

One of those even looks.. familiar..
```

---
## \#1307 Posted by: venom121212 Posted at: 2019-05-16T13:17:39.088Z Reads: 169

```
I think those are just saying that the stickers themselves passed QC inspection :rofl:
```

---
## \#1308 Posted by: murloc992 Posted at: 2019-05-16T13:21:02.940Z Reads: 167

```
Omfg you just fucking didn't.. :laughing:
```

---
## \#1309 Posted by: venom121212 Posted at: 2019-05-16T13:27:13.585Z Reads: 171

```
Shhhhh 

https://media.giphy.com/media/kI8ssGids8uWs/giphy.gif
```

---
## \#1310 Posted by: murloc992 Posted at: 2019-05-16T13:32:57.125Z Reads: 173

```
All good. Lying in bed for 4 days already like:

https://media1.tenor.com/images/52d4680025568821b7f05bd3ffd5bebd/tenor.gif?itemid=6118892
```

---
## \#1311 Posted by: Don Posted at: 2019-05-16T19:21:11.423Z Reads: 170

```
Order March, they said April...then changed to May, now changed to June.... still waiting..
```

---
## \#1312 Posted by: McErono Posted at: 2019-05-16T19:59:24.470Z Reads: 166

```
thats enertion. "end of month" is the standard answer you get.
```

---
## \#1313 Posted by: Darkie02 Posted at: 2019-05-16T21:42:11.790Z Reads: 167

```
So after a lot of reading I’m still none The wiser to what the issue is and what setups have them. As it’s not restricted to just 12s or high kv motors as a outsider id have a guess at sensor tolerance and as it’s seems to be consistently happening under high loads (hard acceleration heavier people) not max speed or max duty cycle is heat part of the issue Has any one with non sensor motors had the issue? Has any one worked out how to get the fault to regularly happen? I’m stuck with the unity as thay messed up the legacy focbox orders by impersonating ostriches and burying there heads a in the sand. Want to know what I need to avoid to make unity's work.

Could this also be related to the power spikes crashing the BT modular is the a regulator issue that is powering the chips with a noisy power supply. I’m no electronics engineer so wouldn't even know we’re to start to rule any of these things out but that’s what comes to mined from what iv picked up so fare.
```

---
## \#1314 Posted by: goldrabe Posted at: 2019-05-17T00:46:52.702Z Reads: 167

```
It happens also to non sensored setups as @murloc992 `s setup.\
Since the last firmware update most of the setups having this issue got fixed and @Deodand  is working on it to fix the remaining too.\
As far as I know, the first issue was caused by a not ideal motor detection.
```

---
## \#1315 Posted by: Sn4pz Posted at: 2019-05-17T00:52:01.160Z Reads: 168

```
Would lowering the max available duty cycle help at all in this case? If its high loads, why not just block yourself from reaching that high in the powerband

I get you guys want to go fast but until theres a concrete fix, I dont understand why anyone would chance it
```

---
## \#1316 Posted by: Jinra Posted at: 2019-05-17T00:55:16.586Z Reads: 161

```
For Francisco it happens on hard acceleration even at low speeds
```

---
## \#1317 Posted by: Blasto Posted at: 2019-05-17T01:19:20.757Z Reads: 166

```
@FranciscoV  is sending his board to @Deodand i believe for a final sanity check.  So far so good on @FranciscoV’s side

Also mad props to francisco for being so generous for helping nail this down
```

---
## \#1318 Posted by: rsalmon Posted at: 2019-05-17T16:10:53.136Z Reads: 166

```
[quote="Darkie02, post:1313, topic:77861"]
Has any one with non sensor motors had the issue?
[/quote]

I am running sensorless and since the latest firmware my board has been running flawlessly. Did a few hundred kilometers already with zero issues.
```

---
## \#1319 Posted by: Ashintar Posted at: 2019-05-17T22:30:22.664Z Reads: 165

```
Same been running the tb dd 90kv 12s with no issues sensorless.
```

---
## \#1320 Posted by: McErono Posted at: 2019-05-17T23:08:37.185Z Reads: 166

```
You have no cutouts while hitting full throttle from standstill? Damn, same setup only on 75kv tbdd and sensored.
```

---
## \#1321 Posted by: Ashintar Posted at: 2019-05-17T23:30:19.674Z Reads: 165

```
I just kick push before ramping up the thottle. The only issue I had was pre the last firmware. A couple times when I started to accel like the first second the power would just cut out and had to reset the power cycle the board
```

---
## \#1322 Posted by: mikenyc Posted at: 2019-05-18T23:43:45.475Z Reads: 156

```
@Blasto @Deodand hey guys, does the latest firmware on GitHub support powering on and off a slave unity over canbus?
```

---
## \#1323 Posted by: Blasto Posted at: 2019-05-18T23:56:42.265Z Reads: 159

```
Yep, set one master, one slave, master has switch and ppm
```

---
## \#1324 Posted by: huntercasillas Posted at: 2019-05-19T00:25:11.878Z Reads: 162

```
I turned positive throttle ramping time all the way to 1.0 and turned down my motor max and min to 30A and it’s definitely smoother, but I still get small jerks when I’m at full speed and release the throttle or when I’m accelerating at lower speeds and want to go faster. It’s definitely less noticeable and not as severe as before though.
```

---
## \#1325 Posted by: venom121212 Posted at: 2019-05-20T23:36:12.532Z Reads: 166

```
New issue popped up today...

Went for a casual ride earlier, nothing out of the ordinary. Charged board up when done. I just hopped on to ride again and my motors are juttering and spinning at very slow speeds and different directions.

I've rerun motor detection a few times and keep getting the wheels spinning opposite directions faster. 

![Screenshot_20190520-193246|236x500](upload://tO53BLQ9zt6dpVyyMutr6mrXhWe.jpeg)

Finally was able to reset connection and everything seems OK. 

Any reason settings would suddenly disappear? No disconnections were made between rides.
```

---
## \#1326 Posted by: DerelictRobot Posted at: 2019-05-20T23:47:52.841Z Reads: 163

```
[quote="Deodand, post:1231, topic:77861"]
Also just to be clear we have loads of people running 8085s and 6374s 190kv on belts with high amperage with no over-current behaviour present.
[/quote]

As a data point, because I'm interested in getting this sorted out for people having issues:

* 4:1 Helical Geardrive
* 6374 190kv motors
* 12S4P battery, bypass BMS
* 90 motors/80 battery amps

I've had zero issues beyond the mild cogging issues from cold start, which was resolved with the last firmware update. No cut outs to speak of in about 2000 miles on this Unity.
```

---
## \#1327 Posted by: RyuX Posted at: 2019-05-21T05:23:15.423Z Reads: 161

```
Same here.. ordered early March.. still waiting

My whole board project is on halt because of the Focbox.. so when they find one more excuse to not ship end of this month then I will just cancel the order.
```

---
## \#1328 Posted by: RyuX Posted at: 2019-05-21T05:24:09.440Z Reads: 159

```
Its funny cause its true...

![image|690x125](upload://gFtXEc2MqPpUbMGnqjjUkW6dA4d.png)
```

---
## \#1329 Posted by: murloc992 Posted at: 2019-05-21T05:32:19.237Z Reads: 160

```
Sounds like the stuttering I had after the crash. Amazing. :confused:
```

---
## \#1330 Posted by: venom121212 Posted at: 2019-05-21T11:28:12.036Z Reads: 162

```
If the settings were instantly reset on the unity while riding, I would expect a very similar outcome.

@RyuX good luck canceling the order... If they've done any "prep" for your order, it's a done deal and canceling will most likely result in enertion store credit aka E-coin aka Jason Dollars.

I would honestly expect mid June to early July as earliest possible ship dates based on track record.
```

---
## \#1331 Posted by: Balth81 Posted at: 2019-05-21T11:53:06.719Z Reads: 161

```
I took my unity out and up to 40mph on Sunday it went like a dream no issues at all rode my 12s for like 2 hours right down till it started throttling due to low voltage about 30km of thrashing it .. I have never had it lose settings or anything my mate who also has batch 1 unity was riding at similar speed with me and he has never had any issues... we are both using nano-x remotes..when I had it try buck me it was warmer weather don’t know if that makes much of a difference... I wouldn’t hesitate buying another ...
```

---
## \#1332 Posted by: murloc992 Posted at: 2019-05-21T13:09:42.466Z Reads: 161

```
I understand that yours is flawless and failing unities are like 1 percentile, but they are still there.. Just lets hope nobody else got one of those too..
```

---
## \#1333 Posted by: rsalmon Posted at: 2019-05-21T15:53:54.831Z Reads: 166

```
I think he’s only trying to balance this thread out a little bit. People having issues tend to be more vocal.

Someone researching about the unity may find this thread and think the product is plagued with bugs when in reality there are lots of people running it without issues.

And the best thing is the issues are being addressed as we speak.
```

---
## \#1334 Posted by: murloc992 Posted at: 2019-05-21T16:00:16.400Z Reads: 163

```
[quote="rsalmon, post:1333, topic:77861"]
And the best thing is the issues are being addressed as we speak.
[/quote]

No updates, not in the slightest from enertion is not what I call issues being addressed, but whatever floats your boat.
```

---
## \#1335 Posted by: rsalmon Posted at: 2019-05-21T16:02:16.431Z Reads: 165

```
From what I've been seeing, @Blasto and @Deodand reply to this thread almost daily. They are the engineers developing and testing the new firmware. 

I wouldn't call that no updates.
```

---
## \#1336 Posted by: murloc992 Posted at: 2019-05-21T16:03:39.232Z Reads: 165

```
Replying to issues(like bad cabling or settings) that are not related to ones that hurt people. I mean, sure dude. :man_shrugging:
```

---
## \#1337 Posted by: Gerrycorrado Posted at: 2019-05-21T16:06:09.933Z Reads: 165

```
![IMG_20190521_175949_822|500x500](upload://x4wegWApLLFM5axqSPoIgyImeuw.jpeg)
Please fix this
```

---
## \#1338 Posted by: murloc992 Posted at: 2019-05-21T16:07:06.177Z Reads: 164

```
Just need a firmware update.

![image|344x310](upload://lTWXrNDSKsKMx2pxpU2Ore3pCZp.png) 

How bad was it? :confused:
```

---
## \#1339 Posted by: Gerrycorrado Posted at: 2019-05-21T16:08:42.161Z Reads: 162

```
40kmh i guess, 6355 190kv, mbs rear wheels, 107 front. Cut out sent me flying
```

---
## \#1340 Posted by: murloc992 Posted at: 2019-05-21T16:09:17.840Z Reads: 163

```
Hopefully you didn't heck up your knee very badly? :confused:
```

---
## \#1341 Posted by: Jinra Posted at: 2019-05-21T16:09:31.685Z Reads: 164

```
did you happen to get any error codes?
```

---
## \#1342 Posted by: Gerrycorrado Posted at: 2019-05-21T16:12:13.808Z Reads: 165

```
I was concentrated on not dying so no codes. Still had a 10min commute to my car (yes i normally do wear gloves and a motorcycle jacket. Both were still in my car at the tire comp)
Helmet was good, but twisted my neck a bit 😂
```

---
## \#1343 Posted by: craigthemachine Posted at: 2019-05-21T16:18:51.176Z Reads: 164

```
Aww shit... Wish you a speedy recovery dude.
```

---
## \#1344 Posted by: Deodand Posted at: 2019-05-21T16:53:12.497Z Reads: 171

```
Sorry on lack of updates guys. Been busy working not writing responses on the forum. I read all the posts always but there isn't much value in me posting "still working". I have the firmware patch tested by a few more people and it seems to have eliminated the issue. More in depth explanation below for those interested. 

We've done some testing to confirm that on the few builds experiencing the issue under a large spike in throttle we see some kind of short lived resonant spikes in the shunt readings. Testing has suggested the spikes are not actually current spikes in the shunts but we still need to investigate further to find and eliminate the cause of the spikes in the ADC reading.  We have found that simply making the abs_over_current fault harder to trigger by requiring it to be sustained continuously for a hundredth of a second seems to completely eliminate the cutouts and the spikes don't seem to cause any cogging to the commutation etc. 

I've decided to release this as a patch while we investigate further. I'm working on the release of the update of the app today/tomorrow so you guys should have the firmware update by then if things go smoothly.
```

---
## \#1345 Posted by: Gerrycorrado Posted at: 2019-05-21T21:39:17.835Z Reads: 169

```
Broken arm close to the elbow. 2 weeks out to start with. Just came out of the ER
```

---
## \#1346 Posted by: murloc992 Posted at: 2019-05-21T21:53:36.965Z Reads: 168

```
Unity Hungers.. Speedy recovery to you.. :confused:
```

---
## \#1347 Posted by: DJase Posted at: 2019-05-21T22:42:42.367Z Reads: 169

```
I'd say there are enough injuries now to send out a warning email at the very least to unity users. Until the firmware is completely tested and proven to be safe this is hazardous as hell!
```

---
## \#1348 Posted by: McErono Posted at: 2019-05-21T22:58:51.950Z Reads: 169

```
Is it two weeks ago I suggested action on enertions side? Lets hope for a newsletter after the firmware is released... like they did a few weeks ago :roll_eyes:
```

---
## \#1349 Posted by: epss4 Posted at: 2019-05-22T00:02:41.947Z Reads: 171

```
Guys cool down the update with the fix is coming out really soon they said ,probably this week! i think that’s why they don’t have published something on this yet .
Sorry to hear that @Gerrycorrado it really  suck to broke something in the beginning of the season :frowning:  !
```

---
## \#1350 Posted by: Gamer43 Posted at: 2019-05-22T00:43:33.943Z Reads: 173

```
[quote="Deodand, post:1344, topic:77861"]
We’ve done some testing to confirm that on the few builds experiencing the issue under a large spike in throttle we see some kind of short lived resonant spikes in the shunt readings. Testing has suggested the spikes are not actually current spikes in the shunts but we still need to investigate further to find and eliminate the cause of the spikes in the ADC reading. We have found that simply making the abs_over_current fault harder to trigger by requiring it to be sustained continuously for a hundredth of a second seems to completely eliminate the cutouts and the spikes don’t seem to cause any cogging to the commutation etc.
[/quote]


Sounds like noise on the analog rail or analog ground.

I know you've probably already done this, but can you ensure there are no ground loops in the PCB?

Also, is the 3.3V rail that supplies the analog circuitry (MCU VREF, current shunt amps) generated by an LDO, buck converter, charge-pump, or precision voltage reference?

Some precision 3.3V references (some from microchip) can supply up to 25mA, which is enough to drive three current shunt amps, and the STM32F405RG's analog circuitry.
```

---
## \#1351 Posted by: lrdesigns Posted at: 2019-05-22T00:50:31.649Z Reads: 172

```
Did anyone report the issue from batch 1 unities? Most of the ones I saw where batch 2.
```

---
## \#1352 Posted by: FranciscoV Posted at: 2019-05-22T00:57:52.352Z Reads: 171

```
I know that feeling brother.  I’m sorry that happened to you.   Shit can be traumatizing 😒
```

---
## \#1353 Posted by: FranciscoV Posted at: 2019-05-22T01:03:13.678Z Reads: 167

```
I have had the issue with both my unities. One came from batch one and the other was second batch.   Just be careful.
```

---
## \#1354 Posted by: lrdesigns Posted at: 2019-05-22T01:03:26.835Z Reads: 168

```
[quote="Deodand, post:1344, topic:77861"]
We have found that simply making the abs_over_current fault harder to trigger by requiring it to be sustained continuously for a hundredth of a second seems to completely eliminate the cutouts and the spikes don’t seem to cause any cogging to the commutation etc.
[/quote]

Wow a hundreth of second is a long time? How often does it normally read the current per second, 1000?
```

---
## \#1355 Posted by: Gamer43 Posted at: 2019-05-22T01:19:41.053Z Reads: 167

```
Closer to ten (twenty) thousand times ;)

And it does this simultaneously for two motors.
```

---
## \#1356 Posted by: bigben Posted at: 2019-05-22T05:51:17.184Z Reads: 166

```
This sucks Gerry, Will have that enclosure for you to work on soon. Should be back over in the next month. 
Heal up well.
```

---
## \#1357 Posted by: Gerrycorrado Posted at: 2019-05-22T09:12:23.774Z Reads: 164

```
Ghoh.. I'm not in a hurry anymore haha
6 weeks out. And then swapping everything back to maytech..
```

---
## \#1358 Posted by: pjotr47 Posted at: 2019-05-22T10:27:42.530Z Reads: 165

```
[quote="epss4, post:1349, topic:77861"]
cool down the update
[/quote]

Cool down? Mate.... if you sell products you must ensure that these are safe for the people who use it. 

After they have know off this problem, they should have informed every buyer of this problem within a few days.  If you want to do even better for your customers, you should arrange a bug fix within a few days-weeks. And stop selling the unity until it is completely safe. 

And yeah it is possible that there are bugs. It is a new item. But just don’t be a company who don’t tell the normal costumers about it. 

Enertion start to look more and more like a Chinese company who only want your dollars. Not more not less. The problem is always for the costumer. Same thing with the Focbox and killed CAN connection. They don’t tell buyers it is important to power on both focbox’s at the same time. And if you kill them it it totally your fault because you have to know it. 

I only sell my batteries when I am sure they are safe to use. I don’t gonna sell batteries where I think they are not safe.
```

---
## \#1359 Posted by: McErono Posted at: 2019-05-22T10:35:36.696Z Reads: 157

```
Everyone that buys anything from Enertion gets an invitation to post a trustspot review in an email - use it!
```

---
## \#1360 Posted by: Andy87 Posted at: 2019-05-22T10:36:23.171Z Reads: 160

```
To be fair, better a bit time for a bug fix than one which just make things worse.
[quote="pjotr47, post:1358, topic:77861"]
And stop selling the unity
[/quote]
Well they still sell them but luckily they take long for delivery, so let’s hope they fix everything till the next batch get shipped

[quote="pjotr47, post:1358, topic:77861"]
Focbox and killed CAN connection
[/quote]
Yeah that’s a pity, but fixed in the lates version they sold. They also didn’t tell us officially that that issue was fixed.

Don’t get me wrong, I want them to fix what ever issues they have as soon as possible, but I also think they can’t make magic now and better they test there fixes now instead of making it even worse with a quick fix release.
```

---
## \#1361 Posted by: McErono Posted at: 2019-05-22T10:38:27.382Z Reads: 155

```
new firmware should be available tonight but who is brave enough to test it to the limits? @FranciscoV
```

---
## \#1362 Posted by: murloc992 Posted at: 2019-05-22T10:42:52.514Z Reads: 155

```
The developers of the update of course. Enertion should test it on their own fur. Because fixing shit in production is kind of unacceptable, when it hurts clients.
```

---
## \#1363 Posted by: McErono Posted at: 2019-05-22T10:44:29.210Z Reads: 156

```
they probably don‘t have all affected setups :no_mouth:
```

---
## \#1364 Posted by: murloc992 Posted at: 2019-05-22T10:44:52.621Z Reads: 161

```
I think several got shipped. So let them try those shipped setups. For science.
```

---
## \#1365 Posted by: sayekim Posted at: 2019-05-22T10:46:35.094Z Reads: 163

```
Yeah this is the problem. 

Also there are so many variables as in board setup that may affect results too. 

A test rig should be made that simulates an actual person riding. 

I like to gun it from standstill with 60 batt amps and 80 motor amps (190kv May tech, 12s6p) but after this threw me off once and almost threw me off a few times because of fw3.40 abs max current flaw on escapes I now am much more cautious to do this. More like I’d rather not unless I’m feeling stupid.
```

---
## \#1366 Posted by: Powadangaboards Posted at: 2019-05-22T10:59:33.095Z Reads: 164

```
Hope your recovering quickly dude....
```

---
## \#1367 Posted by: Powadangaboards Posted at: 2019-05-22T11:05:35.593Z Reads: 163

```
I have been advised by doctors and physio not to get back on my board as I have torn all ligaments in my right knee and herniated my lower disc in my back... oh well Eskate was fun while it lasted but put and end to my skating days.... thanks @EnertionSupport
```

---
## \#1368 Posted by: pjotr47 Posted at: 2019-05-22T11:14:20.448Z Reads: 168

```
[quote="Andy87, post:1360, topic:77861"]
To be fair, better a bit time for a bug fix than one which just make things worse.
[/quote]

Correct! But a bit time in "enertion time" is for us a long time. They had told that a IOS app was coming soon. Now it is coming but at the end off the year :laughing:

[quote="Andy87, post:1360, topic:77861"]
Don’t get me wrong, I want them to fix what ever issues they have as soon as possible, but I also think they can’t make magic now and better they test there fixes now instead of making it even worse with a quick fix release.
[/quote]
Indeed, but at this moment the untiy bug start to go to the same circumstance like the wheel issue from the Dutchies.

I don't know how much people there is working behind the scene for a firmware fix and I know Deodand will have the knowledge to fix the issues. But sometimes it is better to 
to hire an additional programmer who can also take a extra look in the firmware. [spoiler]But maybe there is no money for it, so they have to do again some deals on products for extra cash[/spoiler]


Also don't get me wrong, but I have respect for enertion because they are launching a new product. But If you know there is something wrong, at least tell it to your costumers. And works so hard as you can to fix the issue.

BTW: I have a broken antispark switch on the unity, I have placed something on my insta story about it. Enertion send me a message with "contact the costumer service". I still haven't done that, 
because I know what's coming, "We can't give you any warranty, You have changed the bullet connectors, 60days is over and you have bought it from a forum member". The unity has only 600km on it. The antispark is no big deal because I have a e-switch on the BMS.

But I feel sorry for the people who have a store and who are thinking about selling it in the future. 
Because the warranty issues are almost always for their account.


But I fully hope that enertion will do their best so that this does not have to happen
```

---
## \#1369 Posted by: murloc992 Posted at: 2019-05-22T11:16:55.624Z Reads: 164

```
[quote="Powadangaboards, post:1367, topic:77861"]
I have torn all ligaments in my right knee and herniated my lower disc in my back…
[/quote]

Oh my fucking god.. :frowning:
```

---
## \#1370 Posted by: rey8801 Posted at: 2019-05-22T11:18:15.140Z Reads: 166

```
Man that so bad... :tired_face: Things can radically change so fast. I am truly really really sorry for what happened to you.
```

---
## \#1371 Posted by: murloc992 Posted at: 2019-05-22T11:19:24.881Z Reads: 164

```
Guess what is Enertion(mostly applies to the white knights too) going to say about it?

NEW FIRMWARE! SRY GUYS!
```

---
## \#1372 Posted by: Gerrycorrado Posted at: 2019-05-22T11:24:20.668Z Reads: 169

```
Well.. I have 3 expensive book shelves now. And im not even talking about my psycho build which will be delivered tomorrow.. With a unity in it

![IMG_20190521_235735_698|500x500](upload://3zVaGWlgplcKsywbHFoP6zXcccs.jpeg)
```

---
## \#1373 Posted by: Powadangaboards Posted at: 2019-05-22T11:33:53.852Z Reads: 170

```
I’ll have my parts up for sale very soon (except the unity - I will take pride in burning it!!!) just take care guys!!
```

---
## \#1374 Posted by: rey8801 Posted at: 2019-05-22T11:36:29.076Z Reads: 170

```
To be honest I totally understand why many of you are angry about it, although we gave for sure that Unity won't have problems while the VESC are by far the most delicate part and the one with higher chance of failures. I personally never believed that Unity will be perfect ( I have 2 of them) straight away and I treat it as I treat a Flipsky Vesc ecc... The difference is that @Deodand and @Blasto are really focused on it, while with the other companies we basically can not communicate. That is the reason why I replaced my vesc with Unities. So I totally understand the bad feeling related, and It is super important report back the problems we all have. Although I do not think that claim that they are doing all wrong will help a lot. At the end they can do much more than try to fix the problems while they happen. I am not try to justify them, I am only say that at the end they the best option we have now in term of cost/support and development. For instance, I was throw into space from a Flipsky 6.6 vesc, luckily at around 35kmh, and in that case I can only take the hit and can not do anything to avoid it in future. While with Unity we can at least try to improve the product for our own safety. Of course for Enertion Unity is first a product to sell, but if it gets better I call it a win win for both.
```

---
## \#1375 Posted by: Gerrycorrado Posted at: 2019-05-22T11:38:00.204Z Reads: 168

```
Nope. Nope nope nope
```

---
## \#1376 Posted by: rey8801 Posted at: 2019-05-22T11:38:25.056Z Reads: 168

```
Damn! So bad. I thought you told me you won't buy Unity since was too soon...I guess you were right. Bad that you changed idea at the end. I am really sorry to see people hurt.
```

---
## \#1377 Posted by: venom121212 Posted at: 2019-05-22T11:45:12.014Z Reads: 170

```
I feel like the unity is becoming much like a Tesla:

1) polarizing love or hate for concept
2) "high end" commodity
3) great performance, sans the crazy accidents that hit the news
4) constant willingness of team to work on safety updates

Personally, I don't trust any system until it's been more or less proven perfect. I wouldn't own a Tesla or autonomous car until all major bugs are ironed out. I bought a first order unity before these issues arose and it's been working great. If I saw these issues before purchase, I doubt I would buy one. I have a 3rd batch one on the way (maybe? Hopefully?) that I'm going to feel very uneasy riding until it's tested ok.

My $0.01. Sorry don't have 2 cents to give.
```

---
## \#1378 Posted by: Sn4pz Posted at: 2019-05-22T11:47:11.863Z Reads: 168

```
If anyone wants to go in together on the VESC 6s.... let me know :P 

I mean yeah.... Unity.... wooo :joy:
```

---
## \#1379 Posted by: venom121212 Posted at: 2019-05-22T11:50:18.841Z Reads: 168

```
No but I am watching that serious focer like a hawk. 3 boards fully made between Christmas and the end of summer does wonders for the wallet and my company is at a pivotal point right now.
```

---
## \#1380 Posted by: Sn4pz Posted at: 2019-05-22T11:52:38.584Z Reads: 170

```
That's the vesc6 variant from Shaman, right? His naming convention confuses me. 

He said that design would take until July. Im hoping it comes out earlier :P
```

---
## \#1381 Posted by: murloc992 Posted at: 2019-05-22T12:01:15.643Z Reads: 171

```
To be honest I'd trust Tesla more.

Unity is falling a tier below Chinese dual VESCs with current issues. I just hope there weren't any deaths or near-death injuries either outside of the forums or inside and they just can't tell us about the situation, well, because typing is not really possible at the given moment under given circumstances..
```

---
## \#1382 Posted by: dareno Posted at: 2019-05-22T13:04:59.247Z Reads: 174

```
I was a major naysayer of the focbox initially because of the whole canbus deal but now would not use anything else.  I think enertion dropped a massive bollock in releasing the unity too soon and cancelling the focbox too soon.   It will be the industry standard eventually but if they can weather the storm, well that remains to be seen
```

---
## \#1383 Posted by: Toughook Posted at: 2019-05-22T13:11:55.747Z Reads: 176

```
been said before but I really want to know what Bioboards' solution to this is ? They have single and dual Unity setups in their 80kph boards and seem to be selling them to the public as finished items.

I've got 2x Unitys in 2x builds, both of which are (slightly) out of action until the weekend. This thread is scaring me. I had the throttle spikes at low speed last time I rode/tested (a week ago), and then something unrelated broke down so I stopped for the day then and haven't ridden since. Currently got no confidence in the Unity at the moment and very tempted to install dual Focbox over CAN until the community is happy things are OK. I'm lucky I've got the option (6x focboxes in trhe drawer), but what happens to people without that luxury ?
```

---
## \#1384 Posted by: FranciscoV Posted at: 2019-05-22T13:52:55.332Z Reads: 178

```
Way ahead of you brother.  We did a little bit of testing and so far so good 

I went from a stand still to 100% throttle on a very very steep incline.   Did it several times and had no issues.    Later on got on 100% throttle from stand still to up to 35mph no issue.    Been riding a little bit on the aggressive side and so far so good.   
Again.  I’m not saying your patch works perfect or has fixed the issues 100%  but I haven’t had any problems since fw was updated with it  🤷🏻‍♂️
```

---
## \#1385 Posted by: venom121212 Posted at: 2019-05-22T13:58:17.072Z Reads: 176

```
So you're getting a free unity for braving the testing right? :wink:
```

---
## \#1386 Posted by: FranciscoV Posted at: 2019-05-22T14:03:03.560Z Reads: 175

```
😂🤣🤣.  I wish.   I like Riding my board that’s all
```

---
## \#1387 Posted by: jackluis Posted at: 2019-05-22T16:50:45.202Z Reads: 174

```
I just switched from 190kv 6355 TB motors to 170kv 6380 motors and now I cant preform motor calibration with the android app. It only works via PC now. I heard the mobile unity tool doesnt like big motors with low kv, is this true? I am running 10s btw.

Also, after programming the motors via the Windows tool they cog a bit at startup.
```

---
## \#1388 Posted by: venom121212 Posted at: 2019-05-22T16:55:50.428Z Reads: 172

```
I'm running 200kv 6369 motors with no issue. Setup worked for me 95% of the time. Make sure you're phone screen isn't timing out and move the wheels every few minutes on the board to keep the unity awake. A FW update fixed the unity time out during setup but you may not have it yet.
```

---
## \#1389 Posted by: jackluis Posted at: 2019-05-22T16:58:11.655Z Reads: 170

```
I heard spinning the motors faster when doing the setup can help, is this true? Also your motors are 200kv, i heard this was an issue with big low kv motors.
```

---
## \#1390 Posted by: venom121212 Posted at: 2019-05-22T17:00:42.986Z Reads: 171

```
Oops jumbled up the words. I haven't heard of setup issues on 170kv motors but I've found that the pc connection works flawlessly and offers more options to customize. Android app is only useful for changing basic settings on the go. I wish they'd unlock more config tools for the app.
```

---
## \#1391 Posted by: trampa Posted at: 2019-05-22T17:46:58.203Z Reads: 173

```
[quote="rey8801, post:1374, topic:77861"]
while the VESC are by far the most delicate part and the one with higher chance of failures
[/quote]

For sure not. Maybe clones are delicate, VESCs are proven to be rock solid.
```

---
## \#1392 Posted by: rey8801 Posted at: 2019-05-22T17:59:01.206Z Reads: 170

```
What I meant is compare to the other mechanical parts. It's the electronic core. You will always find more VESC mistake than snapping trucks ecc. 

I can not speak for the one you sell since it's the closest to Vedder's work. For sure it's really relialable but can not be 100% failure proof. Other reliable (V) ESCs work well but they do fail. 
I would like to see the real data polled form all the VESC and VESC derivate out there. At the end only the numbers tell the truth
```

---
## \#1393 Posted by: Gamer43 Posted at: 2019-05-22T19:44:50.469Z Reads: 168

```
I'm just curious, is trampa a paid representative of the company or just an extremely passionate fan of the company?
```

---
## \#1394 Posted by: murloc992 Posted at: 2019-05-22T19:45:44.093Z Reads: 168

```
He just likes to join in on the salt pouring of a 'competitor' I guess. 'It's not the VESC that's bad, it's Enertion' or something along these lines. :smiley:
```

---
## \#1395 Posted by: Jinra Posted at: 2019-05-22T19:47:48.303Z Reads: 168

```
Definitely not the orignal VESC4, that thing died easily on FOC with the stock BOM.
```

---
## \#1396 Posted by: trampa Posted at: 2019-05-22T20:48:24.218Z Reads: 164

```
I just don't like if totally different things are thrown in one pot. 
Each device out there has its own name and reputation.
```

---
## \#1397 Posted by: murloc992 Posted at: 2019-05-22T20:49:32.483Z Reads: 166

```
That's perfectly reasonable. Reputation for one device is this thread itself.. :smiley:
```

---
## \#1398 Posted by: Halbj613 Posted at: 2019-05-22T21:37:25.665Z Reads: 164

```
Hi probably this question has been asked before.

Still not sure about it though?

Is it safe and clever to run the unity on 12s (some people say yes some say no) trying to make sure no cutouts or anything!!

Please help

Thank you in advance
```

---
## \#1399 Posted by: murloc992 Posted at: 2019-05-22T21:48:14.694Z Reads: 163

```
I'd say hold until the cutout issue is solved..
```

---
## \#1400 Posted by: Halbj613 Posted at: 2019-05-22T21:49:19.842Z Reads: 163

```
Will that be in the software or the actual unity

Already ordered unity in Easter sale so will I need to order a new one or just update this one
```

---
## \#1401 Posted by: Halbj613 Posted at: 2019-05-22T21:49:37.247Z Reads: 165

```
I’m guessing you also mean it hasn’t been solved
```

---
## \#1402 Posted by: murloc992 Posted at: 2019-05-22T21:54:04.143Z Reads: 163

```
It's a firmware issue. If it gets solved, then push it.
```

---
## \#1403 Posted by: Halbj613 Posted at: 2019-05-22T21:55:09.446Z Reads: 165

```
Is there any future plan to solve it or is that not really happening anytime soon

Also will it be unusable or is there a way of limiting it
```

---
## \#1404 Posted by: venom121212 Posted at: 2019-05-22T21:58:57.738Z Reads: 167

```
Try checking out the focbox unity support thread!

https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861

Oh wait... That's this thread and you just don't care to search/read.

Take my hand child, 

**@FranciscoV has been testing the latest version of FW that's hoping to solve this. So far it looks good. They'll push an update when it's more tested and stable**

https://giphy.com/gifs/adventure-time-cartoon-network-tzg9DbKxwj9eM
```

---
## \#1405 Posted by: Halbj613 Posted at: 2019-05-22T22:00:29.640Z Reads: 163

```
I have looked but it’s pretty hard to go through all 1500 posts

Is there anyway to flag key posts for newcomers to find key info on a thread
```

---
## \#1406 Posted by: venom121212 Posted at: 2019-05-22T22:04:03.879Z Reads: 160

```
Unfortunately no. You can personally bookmark posts to recommend or use later. A mod can pin a banner topic to the top (doesn't really apply here) like the esk8 events are currently doing. The thread creator can edit the first post to reflect major changes.
```

---
## \#1407 Posted by: Halbj613 Posted at: 2019-05-22T22:04:52.508Z Reads: 159

```
They should make something where you can press to see key parts of the thread
```

---
## \#1408 Posted by: pjotr47 Posted at: 2019-05-22T22:05:22.916Z Reads: 163

```
Mate, you were were talking about no added photos in my topic. But you don’t take the time to read my text in the topic. 

Please read.... & read again. If you had read this topic.  even the last 100 post then you knew this was a firmware problem
```

---
## \#1409 Posted by: Halbj613 Posted at: 2019-05-22T22:06:38.151Z Reads: 160

```
Still think mods should come up with my idea
```

---
## \#1410 Posted by: pjotr47 Posted at: 2019-05-22T22:07:24.630Z Reads: 163

```
Bruh.... this forum is running on a discourse server. The mods can’t change that much.

Btw: you are skipping my text about the last 100 post you had to read in this topic.
```

---
## \#1411 Posted by: Halbj613 Posted at: 2019-05-22T22:08:11.489Z Reads: 166

```
Ah ok

Do you know when this firmware update will be released
```

---
## \#1412 Posted by: pjotr47 Posted at: 2019-05-22T22:09:02.555Z Reads: 168

```
 [quote="Halbj613, post:1411, topic:77861"]
Do you know when this firmware update will be released
[/quote]

[spoiler]You want a slap?[/spoiler]

Read the last 100 post and you will know

Edit: to help you a 14year old kid out.... we don’t know exactly when the new firmware comes out. We all hope ASAP. But I think when you will have your unity at home the firmware will be fixed
```

---
## \#1413 Posted by: venom121212 Posted at: 2019-05-22T22:09:51.104Z Reads: 167

```
I just can't...
```

---
## \#1414 Posted by: DJase Posted at: 2019-05-22T22:22:18.586Z Reads: 168

```
This is not bombastic my dude
```

---
## \#1415 Posted by: RyuX Posted at: 2019-05-23T00:14:21.360Z Reads: 167

```
Hmm.. nah don't need any of these enertion coins..
So not holding a shipping date and selling a "unfinished" product is not a reason to cancel an Order ?
Jesus - seems like Enertion is the new Apple.

I am being paranoid even with normal high quality VESCs where people don't report accidents, how the hell am I supposed to ever feel comfortable with the unity ?

I had two crashes which traumatized me already - I need rock solid things
```

---
## \#1416 Posted by: venom121212 Posted at: 2019-05-23T01:04:04.007Z Reads: 165

```
Meh take it for what it is... Do you see news reports of teslas driving well? Nah, only crashing or almost crashing. Similar story here I think. I've got 2000+ miles on my unity driving in all fashions and configurations I can and haven't had the sudden cutout issue.

Definitely sucks that it has happened a few times but I wouldn't let it scare you away from the product entirely. Best of luck regardless.
```

---
## \#1417 Posted by: Deodand Posted at: 2019-05-23T02:33:15.012Z Reads: 161

```
Hey guys, app update and firmware is all built and seems to be working great. I'm going to give everything a nice long test ride tomorrow (was raining a lot today) and then I will push the update :smile:
```

---
## \#1418 Posted by: SeanHacker Posted at: 2019-05-23T03:25:38.082Z Reads: 168

```
[quote="Halbj613, post:1407, topic:77861, full:true"]
They should make something where you can press to see key parts of the thread
[/quote]

What if you pushed that button and the only key parts were:

* Penis
* Use the search function
* ESK8 Roofies (Not sure if this is a thing... Yet ;))
* Penis

That might not be very helpful. Just saying. I would just search this topic with words that you want to ask as keywords and it will usually lead to search function gold. You'll get it. We believe in you dude! ;)

[quote="RyuX, post:1415, topic:77861"]
seems like Enertion is the new Apple.
[/quote]

Yes. It's horrible. I know. But what can we do... Ugh...
```

---
## \#1419 Posted by: RyuX Posted at: 2019-05-23T05:44:19.682Z Reads: 172

```
Yeah well on one Hand I can perfectly understand Enertion.

It is very hard to test every different aspect of your product - however if you design a product that can cause injuries you will have to invest a lot of money in Quality Assurance with Test Setups - Street Simulation Setups and long time tests under extreme conditions.

I wouldn't mind if I just bought it straight off the shelf - no wait time whatever... But on one hand it get's pushed so hard, shipping dates don't hold, then they even make a special take 2 for a special price promotion while not even shipping the other ones.

I wouldn't mind paying more for a device that went through all sorts of testing and that is rock solid. So I decided to buy 2x Trampa VESC6 in the meantime - they will anyways arrive before the unity and I don't have to worry as much.

I mean the unity seems very cool on paper - the price is right - but even if an error only affects 1% of the people. How does it sound if you jump out of a plane with a parachute and it says that it works 99% of the time.. Would not do it for me..

Timeout and current related issues just have to have enough safety margin straight out of the gate to cover most common setups - reading all the posts here I didn't see anything extra special... only a low KV motor like it's actually quite common on 12S Setups.

I wish Enertion the best to fix this issue - but yeah once I get it I will directly sell it and hopefully will be able to cover my costs (some devices are just too good to be true).

:tired_face:
```

---
## \#1420 Posted by: RyuX Posted at: 2019-05-23T05:46:29.640Z Reads: 166

```
whats your battery and motor setup if I may kindly ask ?

It strikes me as very odd that we don't already have a shared excel sheet with all the data related to the crashes. I mean.. that's the first thing I would do to troubleshoot and see a pattern
```

---
## \#1421 Posted by: Toughook Posted at: 2019-05-23T07:19:33.015Z Reads: 167

```
[quote="RyuX, post:1420, topic:77861"]
It strikes me as very odd that we don’t already have a shared excel sheet with all the data related to the crashes.
[/quote]


well if you would be so kind as to read/trawl this thread and collate the info into a spreadsheet I'm sure the members (and possibly Enertion) would be very happy to read it :-) 

I'm testing 'for the team' another unity on TB DD (90kv 10s) this weekend. If I don't report back then you know it went badly...... (add me to the 'plucky losers' category)
```

---
## \#1422 Posted by: RyuX Posted at: 2019-05-23T08:08:06.405Z Reads: 167

```
Well actually I read the whole thread and not all people gave an exact statement about their Setup. It just seemed that most had a 12S Setup and a low kv motor.
```

---
## \#1423 Posted by: murloc992 Posted at: 2019-05-23T08:08:08.715Z Reads: 173

```
To add a brighter note, my knee actually lucked out and I haven't torn anything except for a small, non-dislocated break at my tibia and a baker's cyst. I will kick unity to bits once I heal. Maybe on video too.

Tho, the MRI says RIP. :laughing:

![image|690x393](upload://pvQyF1BelKNWi3VUJ3pHEa38Hbl.jpeg)
```

---
## \#1424 Posted by: Komamtb Posted at: 2019-05-23T08:16:17.734Z Reads: 173

```
This product should be top notch, how on earth can you sell something, that sends people flying..? Really, how do you allow yourselfs that? The smallest issue can be life or death.
```

---
## \#1425 Posted by: venom121212 Posted at: 2019-05-23T11:31:45.528Z Reads: 170

```
Dual sensored 6369 200kv motors from psychotiller. 

10s5p li ion Samsung 30q pack.
```

---
## \#1426 Posted by: murloc992 Posted at: 2019-05-23T13:51:48.551Z Reads: 174

```
By buying Unity you get into a lottery draw for fancy medical gear:

![image|690x388](upload://rwueh9ymTdlTVHU3J83NcPais6t.jpeg)
```

---
## \#1427 Posted by: mmaner Posted at: 2019-05-23T14:23:46.257Z Reads: 172

```
[quote="Halbj613, post:1407, topic:77861, full:true"]
They should make something where you can press to see key parts of the thread
[/quote]

Are you serious?  Who is this mythical 'they' your talking about?  You could do what everyone else does and read, that is my suggestion.  

I don't understand this new climate of 'spoon feed me so I don't have to do any research, plus I'm gonna be offended if you don't'.
```

---
## \#1428 Posted by: Gerrycorrado Posted at: 2019-05-23T16:08:12.919Z Reads: 170

```
@Deodand what setup are you going to test with?
Can you please confirm on which setups this can happen? Until i had my own accident i was under the impression it happens at +50kmh. If i would have been warned (simple reply in this topic would have helped me alr) i would have taken it easy. I live in a flat area, 10s, max 46kmh so i assumed i was not affected (aaaah the hud does display +50kmh. Wrong at least. Shit, i should have considered that.. )
```

---
## \#1429 Posted by: murloc992 Posted at: 2019-05-23T17:12:49.147Z Reads: 172

```
HUD needs to be calibrated by spinning the wheels 10 times. Not really actual right now, but it needs to be done to show approximately correct speed. :slight_smile:
```

---
## \#1430 Posted by: Tyesk8 Posted at: 2019-05-23T19:51:23.728Z Reads: 174

```
[quote="RyuX, post:1419, topic:77861"]
but yeah once I get it I will directly sell it and hopefully will be able to cover my costs (some devices are just too good to be true).
[/quote]


I'm assuming you paid using your credit card. If so open up a dispute as that is what I would do and get your money back. They haven't shipped the product and aren't even close, you can back out. You're under no obligation to receive a product that has been paid for and hasn't even shipped yet.
```

---
## \#1431 Posted by: Toughook Posted at: 2019-05-23T21:16:21.636Z Reads: 172

```
@Deodand great that you are working/testing a potential fix. My question is how will we receive this update? Will the app get updated via the Google Play store, or does the app just communicate directly with the servers, downloading the file/patch next time i connect to the UNITY with an Internet connection?

As you say the update is imminent I'm holding off fully testing my new build until it's release.... Hopefully won't be too long the wait?
```

---
## \#1432 Posted by: Deodand Posted at: 2019-05-23T22:30:23.950Z Reads: 174

```
You'll need to download the latest version of the app. You'll want it anyways since there are a couple fun little things to play with. I actually just got done pushing it. 

One change is the addition of the sensorless ERPM transition for hall sensor setups. If you are getting some weird low speed stuttering (consistently around a few mph) it can sometimes mean the transition point from hall sensors to sensorless operation is off. Play with the sensorless ERPM transition threshold tends to fix this. 

Here are the download links:

[Focbox UI windows](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_UI.zip)

[Focbox tool windows](https://github.com/EnertionBoards/FOCBOX_UI/raw/FOCBOX_UI/windows_build/FOCBOX_TOOL.zip)

[Android App](https://play.google.com/store/apps/details?id=enertion.focbox.ui)
```

---
## \#1433 Posted by: Toughook Posted at: 2019-05-23T22:51:06.624Z Reads: 175

```
Thank you. The low speed stuttering is exactly the issue i experienced. I never got the chance to go fast as something else (unrelated) broke down so i stopped for the day. Not ridden since as waiting for some support/fixes. Really hope your new update addresses the issues i had, and the other more serious ones outlined above by some less fortunate riders than me !

I really want to love the UNITY. It promises much 🤞😁🤞
```

---
## \#1434 Posted by: Gerrycorrado Posted at: 2019-05-24T08:08:47.777Z Reads: 176

```
[quote="Gerrycorrado, post:1428, topic:77861, full:true"]
@Deodand what setup are you going to test with?
Can you please confirm on which setups this can happen? Until i had my own accident i was under the impression it happens at +50kmh. If i would have been warned (simple reply in this topic would have helped me alr) i would have taken it easy. I live in a flat area, 10s, max 46kmh so i assumed i was not affected (aaaah the hud does display +50kmh. Wrong at least. Shit, i should have considered that.. )
[/quote]

? Bumpedibump
```

---
## \#1435 Posted by: Gerrycorrado Posted at: 2019-05-24T08:28:52.438Z Reads: 172

```
Updated the app but According to the change log, no bug fixes? Issue is still there then @Deodand?
```

---
## \#1436 Posted by: Toughook Posted at: 2019-05-24T08:51:29.330Z Reads: 173

```
Report Back : 

Still alive. First full test after new firmware and so far so good. 10s5p on dual belt 6374 / 107mm. I have to say that this is the first time I've ever ridden my main board in FOC having opted for kick-push-to-go BLDC when I had Focboxs CAN inside. Forgive my enthusiasm here, since most of you run FOC anyways, but OMG what a difference. Standing starts, silent running, butter smooth throttle and decent brakes. OK I took it easy and didn't push any limits (on a busy industrial estate during the day) but this thing just handled amzingly. It was like a 100% new board, and if it didn't look the same on the outside then I would swear it wasn't my build :-) 

I tried to replicate the stutters I'd had previously, doing the same low speed throttle then coast then throttle routine and as far as I can tell it's gone away now. Need more miles to confirm of course, but given it was doing it all the time before, and isn't now, things are looking good.

Still in a slight state of shock at how good my board is now - and I thought it was pretty amazing before - so I'm off for a lie down in my office......
```

---
## \#1437 Posted by: McErono Posted at: 2019-05-24T11:03:06.524Z Reads: 168

```
Still 23.43 here in EU region, last update April 14.
```

---
## \#1438 Posted by: rey8801 Posted at: 2019-05-24T11:04:07.889Z Reads: 169

```
I am in Belgium and got the 23.44. check on Google Play
```

---
## \#1439 Posted by: Gerrycorrado Posted at: 2019-05-24T11:17:35.452Z Reads: 171

```
23.44 but changes mentioned on google store do not mention bug fixes..
```

---
## \#1440 Posted by: McErono Posted at: 2019-05-24T11:51:40.743Z Reads: 177

```
Just updated! Maybe there was just a slight delay in the Swiss playstore.

Going to test this tonight as Jeff thinks thats the reason for my cutouts from standstill.

_Added an advanced motor settings window for tuning pwm freq, sensorless erpm transition for boards with hall sensors_
```

---
## \#1441 Posted by: Toughook Posted at: 2019-05-24T12:10:15.204Z Reads: 178

```
I agree that they should state 'bug fixes' but I suspect in doing so they would then incriminate themselves and accept that the unit was 'faulty' in the first place. I'm no legal expert, it's just a hunch, but I reckon they would argue they are 'improving' things rather than fixing them.

Either way, my unity works better after the update. For the moment, at least, I'm happy with the update.
```

---
## \#1442 Posted by: murloc992 Posted at: 2019-05-24T12:11:16.324Z Reads: 176

```
[quote="Toughook, post:1441, topic:77861"]
I suspect in doing so they would then incriminate themselves and accept that the unit was ‘faulty’ in the first place
[/quote]

They would add fuel to a lawsuit that could come up if hurt people unite(haha, unity). :smiley:
```

---
## \#1443 Posted by: Gerrycorrado Posted at: 2019-05-24T12:38:53.836Z Reads: 174

```
Euh, deo already posted they found an issue, so that's too late..
```

---
## \#1444 Posted by: Gamer43 Posted at: 2019-05-24T15:41:22.655Z Reads: 176

```
Is the switchover a hard switchover? Or does it run the observer for a bit and waits until the sensored and sensorless speed estimators agree on a value before making the switch? If not, does the switchover have hysteresis?
```

---
## \#1445 Posted by: Deodand Posted at: 2019-05-24T16:38:51.537Z Reads: 182

```
 @Gerrycorrado Look at the firmware changelog not the app changelog.

@Gamer43 it's coded by vedder, the estimator is always running and then whenever the rpms cross the threshold (plus some added hyst) the halls are used to add a correction to the estimation. 

Look at line 2844 of this file if you wanna see implementation of hall correction, it's pretty fun:

https://github.com/vedderb/bldc/blob/master/mcpwm_foc.c
```

---
## \#1446 Posted by: epss4 Posted at: 2019-05-25T02:05:52.960Z Reads: 183

```
So i just did the new firmware update but now it look like it don’t  detect sensor from one motor ... it was fine before the update :frowning: !! And both motor seem to roll perfectly fine like if they were sensored..i did re install the unity app and reflash the new firmware but nothing’s change ...is it possible that the update make this ? @Deodand  ![image|281x500](upload://sRu4a8nOKBh1sy2BPvKodaoNk5a.jpeg)
```

---
## \#1447 Posted by: Gerrycorrado Posted at: 2019-05-25T10:02:19.300Z Reads: 180

```
@Deodand can you still pretty please let me know with what setup you have tested? Thx
```

---
## \#1448 Posted by: glyphiks Posted at: 2019-05-25T11:07:34.314Z Reads: 179

```
Bajaboards do it with straps, seems to work

https://youtu.be/HD2Pt-elGX8
```

---
## \#1449 Posted by: banjaxxed Posted at: 2019-05-25T11:23:45.131Z Reads: 176

```
Looks ok, they even have a quasi rider weight simulation built in using those tie-downs, all very rudimentary for checks. A better one in the factory he says.

The point being is you can test a wide range of load/power on a bench which is essential when QA’ing controller software. You can’t just go for a ride and expect what you experience to cover all use cases. Multiple test mules with differing hardware which can be dropped onto a jig is the way to go, probably even just a truck mule with the exception of a 4wd or two
```

---
## \#1450 Posted by: McErono Posted at: 2019-05-25T11:41:33.352Z Reads: 175

```
My TBDD sensors are fine after the update but I couln't test... raining again. Worst May ever...
```

---
## \#1451 Posted by: epss4 Posted at: 2019-05-25T12:52:03.014Z Reads: 172

```
One of my sensor wasn’t connect properly... thanks anyway man
```

---
## \#1452 Posted by: Gerrycorrado Posted at: 2019-05-25T20:46:49.269Z Reads: 178

```
So, can we get some test results from real people then?

  [poll type=regular results=always]
* Yes, tested and all ok
* Yes, tested. Still an issue (please comment) 
* No, haven't tested yet
[/poll]

Thx
```

---
## \#1453 Posted by: venom121212 Posted at: 2019-05-25T21:25:37.772Z Reads: 175

```
I think this is a great idea but belongs in a separate thread as the top post so it doesn't get buried. I can make one if you like or you can. Make sure FW version tested is in the title if you make it.
```

---
## \#1454 Posted by: murloc992 Posted at: 2019-05-25T21:26:34.706Z Reads: 180

```
I think this is just for the newest firmware. We would have a literal ton of threads every update. :slight_smile: Let it be here I guess and bookmark it?
```

---
## \#1455 Posted by: venom121212 Posted at: 2019-05-25T21:31:12.425Z Reads: 181

```
That's what I'm saying.. Make one thread for the new FW update with the vote up top.

That would just be one thread created instead of people accidentally missing post #1439 in this thread specifically. Don't fight me, just let it happen.
```

---
## \#1456 Posted by: murloc992 Posted at: 2019-05-25T21:49:39.395Z Reads: 179

```
Not fighting, at first the reply wasn't as elaborate, so I guess I missed a quick edit. Yup, in this case, that would be good. :stuck_out_tongue:
```

---
## \#1457 Posted by: Marsl187 Posted at: 2019-05-25T21:59:05.354Z Reads: 179

```
I updated the firmware yesterday. The issue in my case happend at hard acceratimg, but like after 5s of full throttle.
For testing I have a really steep hill where I can go full throttle for very long without getting that fast. The hill is a dirt track btw.

So I went there to test again and I can say:

The issue is NOT solved. 

But it was different this time. After the cutout just one motor was working. The other wasn‘t spinning but braking worked. After restart the unity all was working again.
I’m not sure if both motors cut out or just the one. As I remember after the other cutouts I had I didn‘t need to restart the unity to get the motors spinning again. 

So maybe this might be a different issue? Please help @Deodand 

I wasn‘t able to read out the failure because I‘m on iPhone but will go there next week again with a friend and will try to reproduce! (If that helps)
Tracktion loss might play a role here..
```

---
## \#1458 Posted by: venom121212 Posted at: 2019-05-25T22:26:17.452Z Reads: 174

```
Yes, please retry if you can with traction control on and off so we have more data!
```

---
## \#1459 Posted by: Marsl187 Posted at: 2019-05-25T22:36:38.532Z Reads: 174

```
Is it on or off by default? Cannot change that via the app right? Maybe I should bring my computer then :smiley:
```

---
## \#1460 Posted by: venom121212 Posted at: 2019-05-25T22:37:38.970Z Reads: 176

```
You can change via the app surprisingly. It is off by default I believe. Thank you for your testing. 

I have a really steep hill (one way road, not supposed to go up it) in my nearby park. I want to try this scenario as well. Do you start from a stop or are you already going full throttle into the hill?
```

---
## \#1461 Posted by: Jaydawg56 Posted at: 2019-05-25T22:38:49.966Z Reads: 174

```
Off by default. At least mine was
```

---
## \#1462 Posted by: McErono Posted at: 2019-05-25T22:55:41.780Z Reads: 176

```
Yes off is default and you can enable it in the app. I have the same issue... even on flat streets (weight maybe). We need to test the new advanced options in the motor menu. Are you running with sensors? @Marsl187
```

---
## \#1463 Posted by: Marsl187 Posted at: 2019-05-25T23:11:17.435Z Reads: 181

```
Have you tried the update already?
Yes with sensors. 

My test hill is 25% average for 300m. The steepest part has 33%, there I can go full trottle. Hard to ride there because it is like a meadow with two deep ruts and many stones. I will make a photo next time :smiley:
```

---
## \#1464 Posted by: McErono Posted at: 2019-05-25T23:15:40.914Z Reads: 180

```
Update installed but not tested yet due to rain. My cutout was like after a second of full throttle from stand still but afterwards the board does accelerate normally. no reboot necessary.

When I ride into a steep hill (crazy steep) I can hit full throttle but I am not sure I hit full throttle for more than 5 sec at a time.

 Jeff thinks this is a sensored to sensorless transition issue.
```

---
## \#1465 Posted by: Toughook Posted at: 2019-05-25T23:48:06.675Z Reads: 183

```
I rode 25km today with zero issues. My problem was stuttering at low (carving) speeds where it would blip the accelerator without warning. I tried to replicate the scenario today but couldn't. This is a plus from me.
```

---
## \#1466 Posted by: jmoji Posted at: 2019-05-26T15:10:22.559Z Reads: 185

```
So I was out riding yesterday, when all of a sudden my board just shut off for some reason. Maybe a short? Luckily I wasn't going too fast and kind of up hill, so no injury. When I try pushing the power switch, the led comes on for about 3 secs then turns off. I checked voltage from my batteries and everything seems fine. Unity just wont stay on. Is there a way to check if maybe a fuse got blown or something?
```

---
## \#1467 Posted by: venom121212 Posted at: 2019-05-26T16:42:15.197Z Reads: 184

```
Did you have a low voltage cutoff set in your bms or unity? Were you running up hill when it happened?
```

---
## \#1468 Posted by: colinphotovideo Posted at: 2019-05-26T16:42:29.318Z Reads: 185

```
This happened to me as well! Hope we find the fix soon
```

---
## \#1469 Posted by: murloc992 Posted at: 2019-05-26T16:56:22.091Z Reads: 188

```
His Unity doesn't turn on anymore. :smiley: Sounds like blown switch circuitry..

[quote="venom121212, post:1467, topic:77861"]
Were you running up hill
[/quote]

[quote="jmoji, post:1466, topic:77861"]
I wasn’t going too fast and kind of up hill
[/quote]
```

---
## \#1470 Posted by: venom121212 Posted at: 2019-05-26T17:00:53.411Z Reads: 184

```
Clearly he ninja edited it before you got here... I would never look over something so blatantly :sweat_smile:
```

---
## \#1471 Posted by: murloc992 Posted at: 2019-05-26T17:06:46.007Z Reads: 189

```
1:1 on ninja edits. :smiley:
```

---
## \#1472 Posted by: McErono Posted at: 2019-05-26T17:15:14.935Z Reads: 191

```
What batteries are you guys running? Sometimes the unity resets itself after a fault and the cell count may not be correct = unity thinks cells are in danger.

Same happens after a firmware update. Unity sets the cellcount back to 10s despite you had 12s before the update.
```

---
## \#1473 Posted by: Deodand Posted at: 2019-05-26T17:28:54.125Z Reads: 193

```
What happens if you hold the power switch in? Does it stay on? If it does can you try connecting to it when the power switch is held?
```

---
## \#1474 Posted by: Deodand Posted at: 2019-05-26T18:29:42.394Z Reads: 200

```
@Marsl187 thanks for reporting back on your issue, sorry for delayed response. Finally found a short window to work on some of our new projects (can't wait to announce) but I get kind of deep into the debugging process there and its hard for me to switch focus (my brain is dumb like that).

Can you confirm on the firmware page you see version 23.44 (latest update) and while you are there a screenshot of your config for battery/remote/motors is always useful to us. If this behavior surfaces again a screenshot of the faults command would be very helpful.
```

---
## \#1475 Posted by: Marsl187 Posted at: 2019-05-26T18:50:49.557Z Reads: 199

```
Yes, I updated to the latest before the ride. Settings are the same as in post 717 of this topic. Will go there again next week and will try to reproduce and screenshot it with a friends phone. May take until Thursday...
```

---
## \#1476 Posted by: jmoji Posted at: 2019-05-26T20:31:31.450Z Reads: 194

```
it does stay on if I hold it in. Tried connecting to app, but I get a connection error.
```

---
## \#1477 Posted by: colinphotovideo Posted at: 2019-05-26T20:50:54.112Z Reads: 195

```
@Deodand Also with the same issue and unable to connect. Tried it with the power wires shorted to so its always on mode but no lights or anything still.
```

---
## \#1478 Posted by: RyuX Posted at: 2019-05-27T02:19:39.797Z Reads: 201

```
I would love to test the new firmware but...

![image|490x356](upload://7umq36SrhzlnCfl3DfLmQajd1Wb.jpeg)
```

---
## \#1479 Posted by: drangboards Posted at: 2019-05-27T07:37:21.461Z Reads: 201

```
Does anyone know what red and blue dim flashing lights on the unity means if anything? The unity went about a week without powering off and then stopped.
```

---
## \#1480 Posted by: goldrabe Posted at: 2019-05-27T09:51:11.118Z Reads: 199

```
Got around installing the new Firmware, the low speed stuttering is gone even without having to play with sensorless ERPM transition!
```

---
## \#1481 Posted by: McErono Posted at: 2019-05-27T10:38:20.898Z Reads: 204

```
I can confirm! cutouts at acceleration from stand still are gone by the firmware update itself (no settings touched).

@Deodand Thank you Jeff! Great work!
```

---
## \#1482 Posted by: Mikenopolis Posted at: 2019-05-27T16:58:27.128Z Reads: 192

```
Too lazy to search. Can the firmware update be done by phone app or only computer?
```

---
## \#1483 Posted by: murloc992 Posted at: 2019-05-27T16:59:51.078Z Reads: 193

```
Phone too. Extremely slow, but doable. Do not let your phone sleep throughout that time.
```

---
## \#1484 Posted by: Gerrycorrado Posted at: 2019-05-27T17:02:22.815Z Reads: 193

```
Actually goes pretty fast (on my phone at least, if that makes a diff). 
Make sure your unity sleep time is high enough. If you get an error, simply try again.
```

---
## \#1485 Posted by: venom121212 Posted at: 2019-05-27T17:10:40.662Z Reads: 195

```
[quote="Gerrycorrado, post:1484, topic:77861"]
unity sleep time
[/quote]

Supposedly this is fixed to not time out when updating. I still rolled my wheels every few minutes lol
```

---
## \#1486 Posted by: Gerrycorrado Posted at: 2019-05-27T17:30:14.929Z Reads: 193

```
Ah good to know!
```

---
## \#1487 Posted by: Slydunan Posted at: 2019-05-27T17:42:51.640Z Reads: 193

```
Is there any way to measure your speed in the hud app? I dont see any options for gearing/wheel size so the speed in the hud seems pointless. Not to mention it only goes to 35mph.
```

---
## \#1488 Posted by: murloc992 Posted at: 2019-05-27T17:47:29.975Z Reads: 191

```
Click the gear icon(middle right) on the speed/battery display. Click Test ERPM. Spin the wheel exactly 10 full revolutions. Set wheel diameter. Or first set the diameter, then spin. Can't recall.
```

---
## \#1489 Posted by: Chase Posted at: 2019-05-27T20:16:15.709Z Reads: 188

```
Glad to see these are beginning to get sorted out. I never reported, but I had the same issues as @Toughook. It would damn near knock me off but my stupidity kept me on just preparing for when it does happen. Along with a different motor issue I put mine aside. It’ll be nice when I can get home to test the new updates. Gotta admit, starting a month back in posts this morning had me scared sick (and mad I sold my focboxes), but I’m hoping things will be more positive going forward. I’ve been lucky enough at this point (sometimes pushing 30mph) with no helmet or shoes but it’s not if I’ll fall, it’s when. Really investing in A full deckoz safety setup. I’ll just have force myself to put it on every time.
```

---
## \#1490 Posted by: McErono Posted at: 2019-05-27T21:06:43.443Z Reads: 187

```
Whatever you do ALWAYS put on that helmet! Please!

I have no issues anymore pushing the board hard after 23.44 firmware. I hope this is it and we can all enjoy our unitys from now on.
```

---
## \#1491 Posted by: goldrabe Posted at: 2019-05-27T21:15:20.370Z Reads: 186

```
Enertion still recommends using USB and computer. Whilst bluetooth stability improved, I personally  wouldn´t trust it for firmware updates. The Focbox Tool is the version where you have the most control and which is most similar to the VESC Tool.
```

---
## \#1492 Posted by: Jaydawg56 Posted at: 2019-05-27T21:26:43.299Z Reads: 185

```
Agree. I’ve had the most success with usb connect vice Bluetooth.  Sometimes I can’t even tell if it wrote to the unity with the Bluetooth (hangs or doesn’t give me the confirmation down below).
```

---
## \#1493 Posted by: RyuX Posted at: 2019-05-28T00:24:40.816Z Reads: 188

```
Well that would be good news. So maybe the shipping delay is a good thing - I let you brave guys figure out all of the firmware bugs before then :smiley:
```

---
## \#1494 Posted by: mikenyc Posted at: 2019-05-28T00:57:06.100Z Reads: 187

```
I wonder if the new metr module fixes the Bluetooth connectivity issues with the unity. @rpasichnyk
```

---
## \#1495 Posted by: McErono Posted at: 2019-05-28T08:37:39.758Z Reads: 180

```
thats another point I have to mention. Before 23.44 my stock unity BT module would loose connection all the time while riding. Now it stays connected.
```

---
## \#1496 Posted by: mackann Posted at: 2019-05-28T08:54:38.891Z Reads: 183

```
I have a test metr unity and it works good after a few days of testing, it always have good connection and dont "freeze" when trying to write app/motor settings like the standard can do sometimes. But their is a baundrate problem that make it disconnect for a short time sometimes. I think they already solved it or is working on it. Easiest would be if they would allow with the app to choose baundrate for the internal Bluetooth to @Deodand
```

---
## \#1497 Posted by: rey8801 Posted at: 2019-05-28T09:34:43.757Z Reads: 179

```
That would be really useful. Maybe an advance window where only who dare can modify some more parameters. So Unity app will stay user friendly, but with some advancer features. Unlock the developer tabs :joy:
```

---
## \#1498 Posted by: sayekim Posted at: 2019-05-28T17:00:09.150Z Reads: 180

```
I hope it is resolved too as anyone else who doesn’t want to fear riding because of chance of streetface due to unity fault. 

What surprises me is the lack of ride logs from the ones that have had streetface because of this. 

I always log every ride with the metr pro exactly for these kind of possible issues. I need to be able to troubleshoot what goes wrong when it does. May that be my fault or hardware or software
```

---
## \#1499 Posted by: murloc992 Posted at: 2019-05-28T17:32:20.033Z Reads: 176

```
I bet you wouldn't log it after you get smashed. At least getting to the ER was my #1 priority back then.
```

---
## \#1500 Posted by: Gerrycorrado Posted at: 2019-05-28T18:10:02.569Z Reads: 176

```
I hope  deo saw you post i pmmed him where you discussed the cuurent over amp stuf
```

---
## \#1501 Posted by: mackann Posted at: 2019-05-28T18:11:41.154Z Reads: 177

```
I did have ride log with metr, it was abs overcurrent cut out when I crashed and broke my scapula and got elbow out of joint and needed to do a surgery to screw it togheter. Have been of the board for over 3 month now but in 2 weeks i will be back 😁🛹..  I hope I did not lose my confidence when I step on again ...! But still need 1 year rehab before its good, but atleast my bone is healed now. My cut of problem was fixed in the update before this 👍
```

---
## \#1502 Posted by: Chase Posted at: 2019-05-28T18:47:20.066Z Reads: 173

```
Damn man how fast was the fall at?
```

---
## \#1503 Posted by: mackann Posted at: 2019-05-28T19:09:10.670Z Reads: 168

```
Thats the fun part. A few weeks before I bailed in 40mph but slided it out with no damage at all thanks to protection (that was not any fault on board) then this happend in almost stand still.. Its like I wish it happend on high speed so I could blame myself for going to fast haha 😂
```

---
## \#1504 Posted by: Powadangaboards Posted at: 2019-05-28T19:10:19.258Z Reads: 171

```
The issue is not fixed!!!!!!! i had a friend tom test out the board this evening and the board cut out on him from stand still to hard exceleration after a couple of seconds..... this shit is dangerous guys, is it going to take a death for you to recall? witnessing it happen to another person is nuts! the stopping jolt is fucked up.
```

---
## \#1505 Posted by: murloc992 Posted at: 2019-05-28T19:11:33.452Z Reads: 170

```
Fucking shit.. and I was optimistic to ride my Unity after I healed because of the fixes. VESC6 deal is sealed.
```

---
## \#1506 Posted by: sayekim Posted at: 2019-05-28T19:13:47.695Z Reads: 169

```
Was it an absolute maximum current fault?

This happened to me every time I was testing on fw3.40 on focbox with dual setup via canbus. I set limit to 160 amps for each and as soon as the total of both focbox reached this it would be triggered which should not be happening. 
I went back to fw3.38 and now I could exceed 160 amps total again which should be how it is. 

https://www.electric-skateboard.builders/t/vesc-3-40-absolute-maximum-current-problem-dual-with-canbus/79267?u=sayekim
```

---
## \#1507 Posted by: Powadangaboards Posted at: 2019-05-28T19:14:16.565Z Reads: 164

```
yea indeed.... fucking shit!  i want a refund on my focbox! this shit just isn't on, if you have bought a foxbox and it hasnt been shipped, cancel your order, dont risk it guys!!!!
```

---
## \#1508 Posted by: Powadangaboards Posted at: 2019-05-28T19:19:44.394Z Reads: 167

```
im not sure, im not a techy when it comes to this, i put my trust in enersion that the product would work!
```

---
## \#1509 Posted by: mackann Posted at: 2019-05-28T19:20:51.394Z Reads: 164

```
I understand you are angry, but there is always a risk on any electric skateboard it will fail and probebly not all ppl writing with cutouts have problems related to unity, there is other things that can cause it to, im sure they will fix it, but ofc it sucks to get damage before..
```

---
## \#1510 Posted by: Powadangaboards Posted at: 2019-05-28T19:21:51.662Z Reads: 171

```
![61023918_415922832588691_88132857762938880_n|241x500](upload://ccB4KvURIw3GxoJfPgg7z8880J5.jpeg)
```

---
## \#1511 Posted by: Powadangaboards Posted at: 2019-05-28T19:24:30.280Z Reads: 169

```
i never had this issue with my Evolve board, Ever! never had it with my 2 focbox either. im just not impressed with how this is being handled right now
```

---
## \#1512 Posted by: murloc992 Posted at: 2019-05-28T19:24:59.576Z Reads: 175

```
No offence, I understand your point fully but take a look at this PoS:

![04|690x388](upload://kdQqB2OZdK9JnclRV2Oou2gzVkV.jpeg) 

3D printed wheels, used and beat SK3 motor, printed pulley(duh), shit car ESC, shitty used LiPo batteries.

(Don't forget shitty wiring full of hot glue and electrical tape.)

It never fucking failed. Ever.

Solid as a rock.

Even at ~55km/h.

![image|377x350](upload://qAJp38sxpLEn1bDqVOc7pwN0OKm.png) 

If this piece of shit that cost the same as a single Unity could survive. Why can't a "top class" controller be stable and survive?
```

---
## \#1513 Posted by: Blasto Posted at: 2019-05-28T19:33:31.536Z Reads: 168

```
I think it's worth you create your thread so we can help debug the issue. (tag me so i get notified) (or the entire process will just become a mess if done in this thread)

 describe your entire setup, photos help. Explain what is going on, is it a "cut out" or do the wheels lock?
```

---
## \#1514 Posted by: McErono Posted at: 2019-05-28T19:37:33.098Z Reads: 171

```
[quote="sayekim, post:1506, topic:77861"]
Was it an absolute maximum current fault?
[/quote]

My cut outs are gone. They never triggered a fault in the terminal.

If you are expecting a cut out its an easy test to just hit full throttle on a small incline or even flat. If you are not expecting it, its horrible and dangerous af.
```

---
## \#1515 Posted by: Jinra Posted at: 2019-05-28T19:49:49.742Z Reads: 171

```
Just wanna point out that the last thread I read of a "unity cutout" injury wasn't even because of the unity and was instead the remote. Until we get more clarity on to what @Powadangaboards's fault was, I don't think it's fair to conclude that the Unity was at fault.
```

---
## \#1516 Posted by: Powadangaboards Posted at: 2019-05-28T19:50:35.668Z Reads: 168

```
I have tested the board without no one on it and it does cut out on max acceleration, it only seems to be on r-spec, slow mode seems fine. 

I have a video but cant upload it....
```

---
## \#1517 Posted by: Jinra Posted at: 2019-05-28T19:50:56.645Z Reads: 169

```
What f/w are you on?
```

---
## \#1518 Posted by: Blasto Posted at: 2019-05-28T19:51:05.667Z Reads: 167

```
ok... recalibrate your remote, **make sure you are in R-spec** mode when doing so.

so what is happening is you probably calibrated in "slow mode". so when you flip the switch in R-spec, the ppm signal is able to overshoot the max travel, causing the unity (or any vesc based esc) to think that it is a bad signal.

this "cutout" will not throw a fault, will just bring the throlle back to zeros
```

---
## \#1519 Posted by: Powadangaboards Posted at: 2019-05-28T19:51:44.906Z Reads: 168

```
it is the unitys fault, i have tried this with out with the mini remote, same thing. this is a unity issue NOT remote.
```

---
## \#1520 Posted by: Jinra Posted at: 2019-05-28T19:53:17.794Z Reads: 164

```
I never said it was the remote, I'm saying you should post some faults on here so we can see what it is.

Also include f/w version
```

---
## \#1521 Posted by: Powadangaboards Posted at: 2019-05-28T19:54:08.792Z Reads: 163

```
latest firmware, downloaded it earlier today for my mate to test.
```

---
## \#1522 Posted by: Jinra Posted at: 2019-05-28T19:54:53.762Z Reads: 159

```
It'd be more clear if you posted the actual version number so we're on the same page, also faults since you said you can reproduce it.
```

---
## \#1523 Posted by: Powadangaboards Posted at: 2019-05-28T19:55:34.900Z Reads: 161

```
apologies, ready your comment wrong ;)
```

---
## \#1524 Posted by: Powadangaboards Posted at: 2019-05-28T19:56:28.455Z Reads: 162

```
 23.44 10chars
```

---
## \#1525 Posted by: craigthemachine Posted at: 2019-05-28T19:57:16.182Z Reads: 161

```
I agree. Because if more than half of us, had the fault, no longer experiences the fault. Then, I would expect to see data that supports throwing people in panic mode again.
```

---
## \#1526 Posted by: McErono Posted at: 2019-05-28T19:57:17.831Z Reads: 159

```
Wait..  r-spec mode? You have a raptor 2.1 with cut outs?! Thats news for me! :flushed:
```

---
## \#1527 Posted by: Blasto Posted at: 2019-05-28T19:57:44.120Z Reads: 163

```
he might be using a nanoX
```

---
## \#1528 Posted by: niuva Posted at: 2019-05-28T19:57:54.510Z Reads: 165

```
Well, upgraded to 23.44 and Bluetooth still cuts out on voltage spikes (?), even during bench testing by fiddling with the controller, accelerating and braking.
Disconnects both from my laptop while using the Foxbox Tool 1.3 and Xmatic app on my phone.

https://www.electric-skateboard.builders/t/focbox-unity-official/64944/2592?u=scream
```

---
## \#1529 Posted by: Jinra Posted at: 2019-05-28T19:58:29.933Z Reads: 164

```
Can you post the fault? I'm curious to see which one you're getting.
```

---
## \#1530 Posted by: murloc992 Posted at: 2019-05-28T19:58:59.302Z Reads: 160

```
Oh I heard about this somewhere else.. It sounded like a.. hardware issue.. :blush:

_Something about voltage spikes, ground loops, yadda yadda.._
```

---
## \#1531 Posted by: niuva Posted at: 2019-05-28T19:59:43.602Z Reads: 160

```
Which was supposed to be fixed with a "firmware update" :thinking: :joy:
```

---
## \#1532 Posted by: Powadangaboards Posted at: 2019-05-28T20:00:04.020Z Reads: 159

```
yes using a nano x and a mini 2.4hz
```

---
## \#1533 Posted by: McErono Posted at: 2019-05-28T20:00:24.462Z Reads: 158

```
I was surprised my BT was stable after the update because jeff mentioned it is hardware related and they were looking into a new revision of the module.
```

---
## \#1534 Posted by: Blasto Posted at: 2019-05-28T20:01:14.019Z Reads: 160

```
Please try re-calibrating the PPM settings in R-spec. i'm pretty certain this is your issue
```

---
## \#1535 Posted by: Powadangaboards Posted at: 2019-05-28T20:01:36.943Z Reads: 156

```
I will give this a go
```

---
## \#1536 Posted by: Chase Posted at: 2019-05-28T20:01:39.157Z Reads: 155

```
Watching this thread like a hawk. I have three of these that I’m too paranoid to use.
```

---
## \#1537 Posted by: murloc992 Posted at: 2019-05-28T20:02:40.689Z Reads: 155

```
You can't fix unity with a newer module when a spike/ground loop makes the entire unit crap out for a short time. :smiley:
```

---
## \#1538 Posted by: McErono Posted at: 2019-05-28T20:02:49.921Z Reads: 163

```
[quote="Chase, post:1536, topic:77861"]
that I’m too paranoid to use.
[/quote]

Just shows you are not stupid!
```

---
## \#1539 Posted by: McErono Posted at: 2019-05-28T20:03:35.696Z Reads: 162

```
Just the BT disconnects. He was not talking about unity cut outs :wink:
```

---
## \#1540 Posted by: Powadangaboards Posted at: 2019-05-28T20:04:11.441Z Reads: 164

```
https://www.youtube.com/watch?v=H1SWgC9eyh4&amp;feature=youtu.be
```

---
## \#1541 Posted by: Blasto Posted at: 2019-05-28T20:05:03.723Z Reads: 162

```
yep, that is the exact behavior of a bad ppm calibration
```

---
## \#1542 Posted by: Powadangaboards Posted at: 2019-05-28T20:06:36.040Z Reads: 164

```
Thanks @Blasto i will recalibrate and let you know the outcome
```

---
## \#1543 Posted by: Blasto Posted at: 2019-05-28T20:07:01.600Z Reads: 162

```
dope, make sure to hit apply on your new settings :slight_smile:
```

---
## \#1544 Posted by: niuva Posted at: 2019-05-28T20:14:38.657Z Reads: 159

```
No faults :roll_eyes:
```

---
## \#1545 Posted by: Powadangaboards Posted at: 2019-05-28T20:15:11.351Z Reads: 161

```
Nope.... issue not resolved with ppm calibration!
```

---
## \#1546 Posted by: murloc992 Posted at: 2019-05-28T20:17:33.955Z Reads: 161

```
Got any other remotes? So that you can replicate it with another one. (I am in the same boat and curious.)
```

---
## \#1547 Posted by: Jinra Posted at: 2019-05-28T20:18:22.834Z Reads: 159

```
What are the ppm values you're inputting? And could you please post the fault.
```

---
## \#1548 Posted by: murloc992 Posted at: 2019-05-28T20:19:58.302Z Reads: 159

```
There won't be a fault if the unit craps out. Imagine that the MCU just freezes from something.. like.. electrical, that shouldn't be happening.
```

---
## \#1549 Posted by: Jinra Posted at: 2019-05-28T20:20:42.416Z Reads: 160

```
Well the fault prior to the fix was over current. Wondering if he still gets that.
```

---
## \#1550 Posted by: rey8801 Posted at: 2019-05-28T20:27:29.763Z Reads: 160

```
You probably do it but do you calibrate the nano X everytime you turn it on?
Sequence turn on remote 
Full throttle, full brakes, realease it


Then turn on board.
```

---
## \#1551 Posted by: Sn4pz Posted at: 2019-05-28T20:29:10.203Z Reads: 162

```
Does it matter which order I calibrate the remote in? I've always done brake and then full throttle

The remote has worked fine thus far... But I would like to know for the future :P
```

---
## \#1552 Posted by: rey8801 Posted at: 2019-05-28T20:29:26.604Z Reads: 161

```
I follow the label on the remote
```

---
## \#1553 Posted by: Bas1 Posted at: 2019-05-28T20:30:32.799Z Reads: 158

```
After updating the fw 23.44 right motor is in reverse how is that possible??? I updated the fw with my phone should I try to update with a other phone?
```

---
## \#1554 Posted by: rey8801 Posted at: 2019-05-28T20:31:01.228Z Reads: 157

```
Just redo the motor calibration. Takes 3 sec
```

---
## \#1555 Posted by: Powadangaboards Posted at: 2019-05-28T20:31:35.552Z Reads: 156

```
I have followed @Blasto instructions and same thing, no faults found?? im stumped.  @rey8801 i always follow pairing sequence or my board fails to connect.
```

---
## \#1556 Posted by: rey8801 Posted at: 2019-05-28T20:32:36.669Z Reads: 157

```
It's not a pairing sequence it's for the remote to calibrate the full throttle range. It has no memory. Pairing should work no problem in any case. Otherwise something else is wrong.
```

---
## \#1557 Posted by: Blasto Posted at: 2019-05-28T20:32:59.690Z Reads: 161

```
If lets say the calibration was done in “slow mode” the extremes of the ppm would be somewhere near 1.3 to 1.7 ms.

So any remote you use other than the remote in slow mode will go over the extremes
```

---
## \#1558 Posted by: Bas1 Posted at: 2019-05-28T20:34:39.779Z Reads: 160

```
I did and when it turn automatically they are both spinning in the right direction. I will test tomorrow again.
```

---
## \#1559 Posted by: rey8801 Posted at: 2019-05-28T20:36:39.487Z Reads: 163

```
For the motor calibration you have to hand spin the motors. It tells you when in the app. It's to tell the vesc the right direction. Doesn't matter the automatic spinning
```

---
## \#1560 Posted by: Sn4pz Posted at: 2019-05-28T20:37:44.068Z Reads: 166

```
Sorry for the dumb question, but you hit the nail on it's head and now I'm really curious. 

I did calibrate my remote in slow mode, thinking it was fast mode. Am I losing any of my braking ability due to this? As far as I understand it's only acceleration/top speed that is impacted by this?

I really don't feel like opening my enclosure again
```

---
## \#1561 Posted by: Bas1 Posted at: 2019-05-28T20:38:22.478Z Reads: 161

```
Oké thanks I didn't look at my screen so that's why it went wrong.
```

---
## \#1562 Posted by: rey8801 Posted at: 2019-05-28T20:39:23.690Z Reads: 161

```
Why don't you use the Bluetooth to calibrate it? It's sketcky to calibrate in slow mode. When you go to race mode you use 25% over the limits. Slow mode limit the range of around 75%
```

---
## \#1563 Posted by: rey8801 Posted at: 2019-05-28T20:40:16.841Z Reads: 158

```
Yeh I thought Unity was the easiest thing to calibrate it but I guess Enertion should make a tutorial video or maybe it's out there already. I found it really easy . Normal vesc tool has way more steps to do.
```

---
## \#1564 Posted by: Sn4pz Posted at: 2019-05-28T20:50:08.584Z Reads: 162

```
I jumped on the convo as you guys were talking about the nano-x, my spud is just running some 4.xx vescs... lol
```

---
## \#1565 Posted by: McErono Posted at: 2019-05-28T20:51:55.358Z Reads: 163

```
I did calibrate my maytech in slowmode once - it did exactly the same as powadangas board. Could ride a few meters, cut out.

The cut outs from standstill I and others are talking about are (were! They are gone) different. You hit full throttle under load (no issues benchtesting), board accelerates, cutout combined with a horrible sound for a fraction of a second, board continues accelerating. Others discribed it as stuttering.

As for the motor running in wrong direction after setup - the unity does get it wrong sometimes. Repeat calibration or hit the grey/black spot in the HUD to change direction.
```

---
## \#1566 Posted by: murloc992 Posted at: 2019-05-28T20:53:08.263Z Reads: 165

```
Or you could also call it a MCU crap out. :smiley:
```

---
## \#1567 Posted by: Deodand Posted at: 2019-05-28T20:53:57.827Z Reads: 166

```
Calling something what it isn't doesn't really make any sense, does it?
```

---
## \#1568 Posted by: niuva Posted at: 2019-05-28T20:54:56.142Z Reads: 163

```
The "fix" was supposed to make it reconnect after a bluetooth crapout, instead of staying disconnected. Some are reporting it has been fixed but I'm definitely not one of them. 🤷‍♂️
I'm hoping the @rpasichnyk  Metr Unity module would stay connected once I get my hands on one to replace the stock first batch Unity one.
```

---
## \#1569 Posted by: murloc992 Posted at: 2019-05-28T20:55:08.191Z Reads: 162

```
Settings getting reset, stutters after cutouts. I dunno. Maybe.
```

---
## \#1570 Posted by: McErono Posted at: 2019-05-28T21:00:30.198Z Reads: 167

```
Yeah... a cut out. thats a fairly wide range of things and causes.

[quote="rey8801, post:1562, topic:77861"]
Slow mode limit the range of around 75%
[/quote]

62% in my case with the maytech/eskating.eu remote.
```

---
## \#1571 Posted by: murloc992 Posted at: 2019-05-28T21:00:33.661Z Reads: 166

```
Trust me, I am spooked by my Unity more than it looks like. Wish I only got a bluetooth crapout, not a full brake settings reset followed by stuttering motors crapout. :smiley:
```

---
## \#1572 Posted by: Jinra Posted at: 2019-05-28T21:05:32.715Z Reads: 166

```
FWIW I've experienced my fair share of overcurrent cutouts, and it never really full braked for me even though it really does feel that way. Even suddenly cutting off and coasting can feel like hard braking when you're accelerating, even though it's neutral coasting.
```

---
## \#1573 Posted by: rey8801 Posted at: 2019-05-28T21:06:52.133Z Reads: 166

```
Yeh not sure about the numbers, that's why I wrote about. I tested long time ago. Never use slow mode anyway. I don't like that reduces the brakes too. No sense. Then I prefer to lower the max values
```

---
## \#1574 Posted by: McErono Posted at: 2019-05-28T21:08:37.378Z Reads: 166

```
Exactly! Agreed.

It happened the first time I used the maytech... manuals are for... you know. Had no idea whats what :sweat_smile:
```

---
## \#1575 Posted by: Jinra Posted at: 2019-05-28T21:12:44.005Z Reads: 162

```
when you get the problem to occur and go to the app terminal and type "faults" you dont get anything back? Reminder that it has to be done right after you get the fault as faults clear through power cycling.
```

---
## \#1576 Posted by: McErono Posted at: 2019-05-28T21:20:21.209Z Reads: 159

```
No faults after my described cutouts in the terminal. Still they are gone after the firmware update.
```

---
## \#1577 Posted by: Jinra Posted at: 2019-05-28T21:24:15.273Z Reads: 161

```
[quote="Sn4pz, post:1560, topic:77861"]
I did calibrate my remote in slow mode, thinking it was fast mode. Am I losing any of my braking ability due to this? As far as I understand it’s only acceleration/top speed that is impacted by this?
[/quote]

@McErono I'm not sure if you're aware of this, but there's a bug even on official VESCs where if you exceed the PWM value, it will cutout. So if you calibrate on slow mode and get 1.6 ms PWM max for example and use that, then switch to a faster mode and get 2.0ms on the remote, you'll cut out after exceeding 1.6ms.

This is still present on the Unity but is slated to be patched in an upcoming f/w release.
```

---
## \#1578 Posted by: Sn4pz Posted at: 2019-05-28T21:27:11.759Z Reads: 162

```
Thanks for the tip! Im almost certain Ive programmed it in slow mode, but I was really tired and I cant be certain. 

Is this something I can test while the board is belly up? I cant ride today, its been raining on and off :/
```

---
## \#1579 Posted by: Jinra Posted at: 2019-05-28T21:29:32.674Z Reads: 161

```
I think you can bench test it, try it and let us know!
```

---
## \#1580 Posted by: Balth81 Posted at: 2019-05-28T21:30:05.169Z Reads: 168

```
When I first built my board I had a few issues with random stuttering on hard acceleration this was fixed by swapping the phase wires around .. I hope those getting this have at least tried it because mine looked like it was all good most of the time but occasionally it would reverse one motor when hard acceleration... by switching up the phases this issue completely resolved. I have since marked the phases that work for me so I don’t get them mixed up again.

I also at one point found once of the plugs on a phase had been loose so had caused carbon to build up..
```

---
## \#1581 Posted by: McErono Posted at: 2019-05-28T21:31:36.226Z Reads: 169

```
Yes I know thats why I described my cutouts again - powadangas are similar to a wrong calibrated remote. And mine are fixed with firmware 23.44 :+1:

[quote="McErono, post:1565, topic:77861"]
I did calibrate my maytech in slowmode once - it did exactly the same as powadangas board. Could ride a few meters, cut out.

The cut outs from standstill I and others are talking about are (were! They are gone) different. You hit full throttle under load (no issues benchtesting), board accelerates, cutout combined with a horrible sound for a fraction of a second, board continues accelerating. Others discribed it as stuttering.
[/quote]
```

---
## \#1582 Posted by: Sn4pz Posted at: 2019-05-28T21:32:58.814Z Reads: 166

```
Just did! As expected with the wheels up, I cant tell that anything is different between slow and fast mode via sight or sound. There was no kind of cut out or anything 'fun'

I think I must have calibrated it correctly... I guess :joy: 

I guess I'll report back tomorrow when I can *ʰᵒᵖᵉᶠᵘˡˡʸ* ride...
```

---
## \#1583 Posted by: Jinra Posted at: 2019-05-28T21:33:52.850Z Reads: 168

```
You should measure inductance, resistance, and flux linkage for each order of phases, one of my motors failed and had double the resistance on one order, and normal resistance on the other orders. Maybe this is the case for you?
```

---
## \#1584 Posted by: McErono Posted at: 2019-05-28T21:35:04.172Z Reads: 164

```
Without load (you) they feel and sound identical!
```

---
## \#1585 Posted by: MasterSpoon Posted at: 2019-05-28T23:57:19.837Z Reads: 176

```
Maybe I'm missing something obvious here but why isn't there a bug report template ?

There seems to be a lot of people saying "I have an issue" but without information I can't see how @Deodand can be expected to replicate, diagnose or fix the issue. Like if your phone, computer, car, whatever is playing up and you take it to the shop you give them a description of what the issue is and they can inspect the item to try replicate the issue and check hardware / setup / ect but being that it's not practical to have boards sent away for diagnostics I think the more info provided the better.

Eg.

Description of fault ?

What were the conditions when the fault occured ?

Any fault codes ?

Have you been able to replicate the fault ?

Firmware version you are running ?

How was the unity programmed (phone or PC) ?

What hardware are you using ? Battery specs - cells used, size, BMS and if bypassed / motors - brand, model, kv, if using sensors / remote - which remote and how it's connected / the rest - gear ration, wheels, rider weight if applicable, ect

Screen shots of setup / motor detection screen ?

This should not only give much more information to hopefully be able to replicate and diagnose the issue but will also work to inform others if they might also potentially have an issue or not. I'm not sure how far back you can edit posts but also either going back and editing or posting a copy of the bug report when fixed with details of the fix. Like if @McErono cutout was fixed with the latest firmware it would be important for people to know if they have similar setups that they need to update the firmware straight away.
```

---
## \#1586 Posted by: RyuX Posted at: 2019-05-29T00:02:24.902Z Reads: 173

```
Good to know ?!?! I am getting a bit "pissed off" with this company.

![image|690x144](upload://4JkADjuJfD1jWR32gFHa2ZmGQ2Y.png)
```

---
## \#1587 Posted by: McErono Posted at: 2019-05-29T00:31:45.562Z Reads: 170

```
The guys are all very friendly (sadly not very helpful tho) they don't make enertions rules. We all know who does.

If you want stuff done speak to carl. He is closest to the management.
```

---
## \#1588 Posted by: LEE Posted at: 2019-05-29T00:44:09.666Z Reads: 173

```
Switching modes on Nano-X only causes mistakes. I don't know what the switch means.
I think it is better to fix it to R-SPEC mode and adjust the power with Batt.MAX.
```

---
## \#1589 Posted by: Jinra Posted at: 2019-05-29T00:44:54.396Z Reads: 171

```
it's a PWM limiter which limits max throttle to 70%~ and min throttle to 30%~. The latter of which is kind of dumb, but there it is.
```

---
## \#1590 Posted by: Chase Posted at: 2019-05-29T01:20:48.189Z Reads: 176

```
Wtf. The problem is finding out if there is still a firmware issue may cost you your life. So this means if we cancel pending orders they will try to keep 20%?!
```

---
## \#1591 Posted by: rey8801 Posted at: 2019-05-29T04:14:33.076Z Reads: 176

```
Yep they will
```

---
## \#1592 Posted by: Gerrycorrado Posted at: 2019-05-29T09:18:25.949Z Reads: 179

```
![MVIMG_20190524_181349|375x500](upload://rM9H4Hwr92YsXBY8yTdqyV7xWlY.jpeg)
Last week.. Running the at the time latest fw (fw got updated 2 or 3 days after,so for clarity current fw is NOT what i was running) .
```

---
## \#1593 Posted by: RyuX Posted at: 2019-05-29T11:17:30.638Z Reads: 179

```
Get well soon man. 

Glad Enertion has fixed all the firmware issues two months ago.
```

---
## \#1594 Posted by: CarlCollins Posted at: 2019-05-29T11:47:23.913Z Reads: 181

```
[quote="niuva, post:1528, topic:77861"]
Well, upgraded to 23.44 and Bluetooth still cuts out on voltage spikes (?), even during bench testing by fiddling with the controller, accelerating and braking. Disconnects both from my laptop while using the Foxbox Tool 1.3 and Xmatic app on my phone.
[/quote]

Is it possible to share the fault codes or a video of the issue?
```

---
## \#1595 Posted by: trampa Posted at: 2019-05-29T11:51:59.613Z Reads: 180

```
[quote="Jinra, post:1577, topic:77861"]
I’m not sure if you’re aware of this, but there’s a bug even on official VESCs where if you exceed the PWM value, it will cutout.
[/quote]

**This is wrong info!** VESC FW does not do this. I always configure in slow mode and switching to fast only makes the throttle very responsive and short. However, we recommend to always configure in FAST mode!

The described issue happens if you use Ackmanicks modified FW and his ESC-Tool, since it is programmed to activate failsafe when signal goes beyond 100+x %. 

For given reasons, we never implemented such a behaviour, because false calibration of remote would cause unexpected cutouts at speed. We don't recommend to use modified FW since these  "useful hacks" can have downsides you you don't expect to happen. A Fast/Slow switch on a PPM remote is a really bad idea!  A failsafe that is triggered at 120% signal is also a bad idea. The combo of both is potentially hurtful.  Power output should always be changed in the Configuration of the ESC. 

Benjamin knows his code front to back, and he knows why he doesn't  implement certain features that appear useful but come with drawbacks or risks.  A fork always bears the risk that modifications are made without deeper knowledge of the matter. VESC-Tool is a **highly complex software** and only Vedder himself knows all the corners and dependencies. Some things might work for certain HW combinations, but users plug together all sorts of things and expect the system to work.
```

---
## \#1596 Posted by: CarlCollins Posted at: 2019-05-29T11:56:08.965Z Reads: 177

```
I might like to inspect your board myself, let me know so we can arrange a session.
Looks like I have to investigate further by myself.
```

---
## \#1597 Posted by: McErono Posted at: 2019-05-29T12:35:31.651Z Reads: 181

```
[quote="trampa, post:1595, topic:77861"]
The described issue happens if you use Ackmanicks modified FW and his ESC-Tool, since it is programmed to activate failsafe when signal goes beyond 100+x %.
[/quote]

hmm its happening on the unity so no ACK involved or is it? there was a time when ACK was doing some work for enertion...

anyway I will give the stock VESC firmware another try. Heard the throttle response has improved a lot (main reason for ACK was very smooth throttle and brake at the time).

@trampa btw. I did ask a few question per email (enclosure related and ply number for an orrsom etc.) like a week ago. never got an answer. should I try again?
```

---
## \#1598 Posted by: trampa Posted at: 2019-05-29T12:40:24.470Z Reads: 183

```
I'm not addressing Unity FW. I have no clue if this "useful feature" found its way in there.
@Deodand will know.
In any case, a remote calibrated in slow should not cause cutouts, only you switched it to fast. 
I just wanted to create awareness because many use Ack and might not know that there is a potential issue for combo x+y +setting w. 

I'm out here.
```

---
## \#1599 Posted by: Quiles Posted at: 2019-05-29T12:56:30.129Z Reads: 187

```
[quote="trampa, post:1595, topic:77861"]
VESC-Tool is a **highly complex software** and only Vedder himself knows all the corners and dependencies.
[/quote]

You talk as its a good thing to only one person KNOWS everything, FRONT to back...etc.

Well, thats a shame a project of this size, concentrated under only one person. If for Gods sake, something happens to him we are all fuc#$#ed.
```

---
## \#1600 Posted by: Quiles Posted at: 2019-05-29T12:59:48.450Z Reads: 185

```
i think you should focus your sell pitch as community...the community is bigger for VESC, more contributions...etc. Thats way more important.
```

---
## \#1601 Posted by: trampa Posted at: 2019-05-29T13:13:02.130Z Reads: 184

```
I didn't say that! Working on one release together surely has benefits.
If the capable brains decide to run separate forks without having contact 
to the man behind the massive code base, it doesn't really help to solve this issue. 

In this case Vedder wrote a massive software pretty much without anyone else involved.
It's a case of logic, that he has the deepest knowledge. 

https://vesc-project.com/Ethos
```

---
## \#1602 Posted by: venom121212 Posted at: 2019-05-29T13:58:03.777Z Reads: 183

```
Don't worry, I've heard Frank's basement is quite lovely this time of year
```

---
## \#1603 Posted by: Jinra Posted at: 2019-05-29T15:19:10.153Z Reads: 189

```
[quote="trampa, post:1595, topic:77861"]
I always configure in slow mode and switching to fast only makes the throttle very responsive and short.
[/quote]

You realize that makes no sense right? If you limit PPM to an arbitrary number like 70% and configure maximum to **be** 70%, and suddenly switch over to the full 100% range, it's not going to do jack to your throttle. And yes this DOES happen on official firmware, at least on early 3.xx firmware when it happened to me.
```

---
## \#1604 Posted by: trampa Posted at: 2019-05-29T15:42:07.287Z Reads: 188

```
If 70% remote output signal gives 100% throttle (calibration in slow mode), you get 100% power at 70% trigger in fast mode. At full throttle you get over 120% signal, which triggers fail safe in Acks FW mod.
```

---
## \#1605 Posted by: FranciscoV Posted at: 2019-05-29T17:15:05.309Z Reads: 193

```
![12aW6JtfvUdcdO|226x309](upload://rk1PUnk8uGgq04uhMvEmP9INZan.gif)
```

---
## \#1606 Posted by: Powadangaboards Posted at: 2019-05-30T05:48:09.401Z Reads: 189

```
Had no faults show up, @Blasto ran time through this and shown no faults.
```

---
## \#1607 Posted by: niuva Posted at: 2019-05-30T17:06:45.390Z Reads: 187

```
Excuse the squeaky belts 🤣
No fault codes. First disconnect happens at 17 sec and second one at 1min.
10S battery with charge only BMS, so there is no middle man between the battery and Unity. The connection freezes/drops regardless what device I connect to it. For demonstration here I’m using my iPhone X and Xmatic app. Seems like the freeze happens usually when braking.
https://youtu.be/gt7Y6TbieIQ
```

---
## \#1608 Posted by: McErono Posted at: 2019-05-30T17:20:53.742Z Reads: 184

```
@Deodand I've set the shut down switch duration to 1.5sec but I can just push the switch once and the unity shuts off. Bug?
```

---
## \#1609 Posted by: taz Posted at: 2019-05-30T18:00:34.344Z Reads: 184

```
The same thing happens to mine.
It seems the time instead of controlling how long the button needs to be pressed for the unity to turn off it is just a delay timer.

If you set it at eg 5sec and press momentarily the switch,  the unity turns off after 5sec.

Definitely a bug that needs fixing.
```

---
## \#1610 Posted by: Blasto Posted at: 2019-05-30T18:03:03.845Z Reads: 182

```
noted guys, will look in to it and get that fixed asap
```

---
## \#1611 Posted by: FredXanadu Posted at: 2019-05-31T12:01:47.506Z Reads: 181

```
Hello, I would like to know if the unity app is running on Android GO ?
I only own a Iphone, need to find a cheap phone dedicated to the unity...
thanks
```

---
## \#1612 Posted by: glyphiks Posted at: 2019-05-31T15:27:31.260Z Reads: 179

```
Have you seen the metr bluetooth module?

https://forum./t/metr-pro-unity-bluetooth-module/1383?u=surferofdirt
```

---
## \#1613 Posted by: RobPBody Posted at: 2019-05-31T15:49:15.555Z Reads: 179

```
Hi all,

What's the drill bit size used to make the hole in a enclosure for the Anti-Spark switch included with the unity?
```

---
## \#1614 Posted by: legend27 Posted at: 2019-05-31T16:26:39.989Z Reads: 183

```
Pretty sure I read somewhere it was 12mm.
```

---
## \#1615 Posted by: McErono Posted at: 2019-05-31T17:23:00.892Z Reads: 181

```
Yeah someone from Enertion said 12/13mm.

I always drill smaller and use one of these to make it perfect:

![s-l400|400x400](upload://19aAMhwZBxOuDwmX4BAC5RUx6G9.jpeg)
```

---
## \#1616 Posted by: Deodand Posted at: 2019-05-31T17:59:45.167Z Reads: 185

```
@trampa Just so you are aware the current vesc FW actually does have this behavior.  You can look at line 51 of the servo decoding file in the repository to see it. Essentially if the PPM length is greater than 120% of the max value you set then it sends out a signal of -1 instead of the PPM value which simply causes the throttle to turn off.  I.e. if you calibrate in slow mode its going to see a value greater than 120% max in rspec and cut if you max throttle. 

https://github.com/vedderb/bldc/blob/master/servo_dec.c
```

---
## \#1617 Posted by: Blasto Posted at: 2019-05-31T20:48:51.358Z Reads: 183

```
I’m not able to replicate the bug, seems to work on my side.

Do you mind doing a quick video?
```

---
## \#1618 Posted by: taz Posted at: 2019-05-31T21:42:53.075Z Reads: 185

```
Will this do?

https://youtu.be/vVk8l9w5cHU
```

---
## \#1619 Posted by: jmoji Posted at: 2019-05-31T23:15:39.600Z Reads: 185

```
I still cant get my unity to stay on. Is there a way to test my unity with a meter to see if there is a short or something? I honestly dont get what could be wrong. Like I said, turns on for maybe 3 sec then shuts off.
```

---
## \#1620 Posted by: Deodand Posted at: 2019-06-01T00:07:10.813Z Reads: 182

```
I think maybe the firmware did not flash correctly? The microcontroller on the unity is the thing that takes over and keeps the unity turned on after you power it up, so if the firmware isn't running it won't  keep the unit powered up. Do you Have access to an st-link flasher? You can buy them on Amazon for like $8 I think. I can link you a firmware image to flash with that.
```

---
## \#1621 Posted by: jmoji Posted at: 2019-06-01T02:06:13.757Z Reads: 179

```
I dont have access to that. Can you provide a link for that please
```

---
## \#1622 Posted by: Hatman30 Posted at: 2019-06-01T08:03:27.923Z Reads: 177

```
Very mundane but I just unplugged my e switch to get it through a hole in my deck and I forgot which way round the wires go. Is it white white red black, or white white black red ? Thx ... doh!
```

---
## \#1623 Posted by: Linny Posted at: 2019-06-01T08:06:41.987Z Reads: 177

```
@Deodand im getting calibration issues when running the set up again. When i click calibrate for the remote, it will pause at the 'please wait' part for very long. Hence im unable to do the set up properly. Im using the first batch unity.

Edit, reinstalled the app fixed it
```

---
## \#1624 Posted by: ducktaperules Posted at: 2019-06-01T10:52:47.279Z Reads: 180

```
Thats a great find. 

Im impressed you found a bug like that in such "**highly complex software**" considering "only Vedder himself knows all the corners and dependencies". 

Im actualy quite Suprised that @trampa missed this considering "Benjamin knows his code front to back". I guess even the VESC6 "can have downsides you you don’t expect to happen".

Im sure there will be a speedy update for the VESC to fix these “useful hacks” seeing as "false calibration of remote would cause unexpected cutouts at speed" and could be "potentially hurtful".

Maybe next time @trampa wont give others like Ackmanick a roasting "without deeper knowledge of the matter".
```

---
## \#1625 Posted by: FredXanadu Posted at: 2019-06-01T15:43:33.918Z Reads: 181

```
Hi, someone can post the unofficial Unity mac tool link please ?
I can't find it. thanks
```

---
## \#1626 Posted by: Blasto Posted at: 2019-06-01T16:06:27.537Z Reads: 181

```
Unfortunately the mac tool would be out of date if you find it
```

---
## \#1627 Posted by: Battosaii Posted at: 2019-06-01T17:01:11.888Z Reads: 183

```
Yep it is. I have dual boot on my macbook pro because my car tuning software works only on windows and now i use windows for this too lol
```

---
## \#1628 Posted by: ducktaperules Posted at: 2019-06-01T20:58:20.995Z Reads: 184

```
@Deodand,  i went out on my board today for its maiden run and i may have encountered one of the unity issues that others have been reporting. i dont believe its related to the over current fault that others have reported. Im not trying to stoke the fire here, just work out what happened. If its useful I was recording with metr when this happened.

I was riding along at around 15 mph constant power and applied some more throttle to pull away. Mid acceleration i felt the power suddenly cut to coasting. luckily I was using bindings which probably saved me from a good case of face pavement. As soon as i thought to reapply power it was working again so i carefully pulled back into the car park and stopped logging. 

At this point my friend (who had seen me have a bit of a wobble but was keen to try my new board) stepped onto the board. He pulled away in the car park (with some heavy throttle) and no less than 20m away the throttle sharply cut again and he went straight over the front (probably doing about 12mph). Unfortunately i was not still data logging the second time this happened.

My Settup: 
I have a batch 1 unity which is powered directly from a 12s4p 30q pack (bms bypass). Battery currents were set to 80/-20A and motors set to 30/-60. Other than that all settings were at defaults. I did a firmware update this morning to the latest with all the recent bug fix's. im running maytech 6880 motors 190kv with a 5to1 gear drive and 6.5 inch street wheels. Only other info that might be relevant is that im a big guy but i wouldn't expect this to matter to much with the motor currents set this low.

Logs: (https://metr.at/r/UmU1a)
After reviewing the log it seems that all temperatures seemed reasonable and there were no fault codes shown in metr. I believe the cut out happened at around 5:53 in the logs (maybe +/- 10 seconds.

@Deodand  Is there any way to record a log file of everything that is happening in the unity app or only with metr? 

@rpasichnyk the "duty cycle" shown in the metr log, what exactly is that? is it remote pwm duty cycle or motor duty cycle?
```

---
## \#1629 Posted by: murloc992 Posted at: 2019-06-01T21:04:06.682Z Reads: 179

```
Just be careful with the Unity. I wouldn't have trusted any new firmware fixes until I saw deo himself ride on video, high speed, high accel from standstill, etc. to confirm it works and is fixed. Even then, it could be staged settings. It just sends shivers down my spine thinking about some of the injuries. I prefer to still have my legs and arms, and especially no screws inside my bones.

Glad you're okay though.. We need less face pavement cases..

Your METR log seems so "noisy". No faults too?

Could it be the remote?
```

---
## \#1630 Posted by: ducktaperules Posted at: 2019-06-01T21:22:18.027Z Reads: 179

```
what do you mean by "noisy"? 

this log is over the course of an hour with a quick pub stop in the middle, might explain why it has such sharp spikes. Its annoying that i cant seem to find a way to zoom into the log and look at it in more detail cause im sure the more detailed data is there somewhere. @rpasichnyk is that possible in any manual way?
```

---
## \#1631 Posted by: murloc992 Posted at: 2019-06-01T21:23:20.345Z Reads: 178

```
Yup, that must be the timescale. I think I saw logs before that allowed to scroll to right way more and shown smoother peaks, that's why I asked.
```

---
## \#1632 Posted by: ducktaperules Posted at: 2019-06-01T21:49:29.333Z Reads: 178

```
ok so i accidental found that you can zoom in on the metr log by dragging over a section of the timeline to select it.

After looking at it closely i think it happened at 05:52:35, here's how it went down: 
 - So im stopped waiting for my boosted friend to catch up. 
 - At 05:52:24 I start to accelerate at the full 30A per motor as he goes past so that i can match his speed. 
 - At 05:52:30 i let off the throttle and coast at about 12mph alongside his boosted board which is stuck on the eco limiter. 
 - At 05:52:33 i decide its time to smoke him and start to accelerate away at 30A per motor again.
 - At 05:52:36 i suddenly loose power and brown trouser myself.
 - By 05:52:39 I have mentally recovered enough to check if i still have throttle control or if i killed it forever.

![metr|641x500](upload://onVDOSwJCRGAIgT9uzQJ8O3MtOU.png)

EDIT: just realised its not that useful without the Key. light red is current (im assuming battery), dark red is motor current, brown is speed & light blue is duty cycle.
```

---
## \#1633 Posted by: Deodand Posted at: 2019-06-01T23:19:50.069Z Reads: 176

```
Yes, I don't think the currents you were pulling anywhere in this log present any kind of problem. What remote/reciever are you using? The description of the cutout sounds a bit different from what others mention. Typically a cutout of the natre you describe would be accompanied by a fault report if it was the unities doing. Without a reported fault I'm inclined to think the unity isn't receiving a ppm command for whatever reason... that actually could be an interesting value to add to logging, could help a lot of people pinpoint where the issue is coming from. 

Can you open up your build and play around with your remote/ppm cable to make sure everything in that chain is solid?
```

---
## \#1634 Posted by: ducktaperules Posted at: 2019-06-01T23:30:11.481Z Reads: 183

```
So I'm coming round to the idea that this might have been caused by the previously mentioned bug regarding badly calibrated remotes.

I have the Maytech remote that has 2 speed settings. It defaults to "slow mode" when you turn it on then you can manually change to full speed. The slow mode limits to ~70% ppm at full forward throttle.

When I updated the firmware this morning it would have cleared all the settings so I must have recalibrated the remote during setup. If I turned the remote on to do this then I might not have set it to full power mode before calibration.

This would make sense because it was reliable for most the day and I kept it in slow mode for the range. On that last straight we all switched to higher power to use up the battery before getting back to the car. Then I had that cutout and thought "maybe I should take it easy" so turned it back to low till i got back to the car. 

Then my friend wants a go, I think "bet he wants to feel the power" and put it back in full throttle mode. He promptly gets a good case of StreetFace.

Seems like this could be easy to do accidently without noticing when you do firmware updates and I wonder how many others have done a similar thing without realising.

@Deodand maybe an easy "fix" for this could be made in the app so that after throttle calibration if the maximum ppm value is less than 1.8ms the is a popup or warning saying something like "low max throttle detected, is your remote set to full throttle range?". User could say "yes but apply anyway" or "repeat calibration". Its not likley to break anyone's setup but might save a few people from bad calibrations that result in tasting the pavement.
```

---
## \#1635 Posted by: Deodand Posted at: 2019-06-01T23:36:53.034Z Reads: 178

```
I like the idea of a ppm warning thanks for the suggestion. I'm going to patch that behavior next week as the throttle dropping seems more dangerous than simply an over-sensitive throttle with early saturation.
```

---
## \#1636 Posted by: ducktaperules Posted at: 2019-06-01T23:38:03.584Z Reads: 182

```
[quote="Deodand, post:1633, topic:77861"]
that actually could be an interesting value to add to logging
[/quote]

I think this would be very useful. Black box logging in most drones captures this and it's very useful it see if the controller is at fault or the reciever. 

With the frequent firmware updates (and therefore remote recalibrations) I could see how this could be happening suddenly to users that haven't had problems before.
```

---
## \#1637 Posted by: Deodand Posted at: 2019-06-01T23:40:53.912Z Reads: 183

```
Well hopefully its a nice simple fix, thanks for the feedback. Keep us updated on what you find.
```

---
## \#1638 Posted by: Hatman30 Posted at: 2019-06-02T11:48:41.369Z Reads: 177

```
Can anybody tell me how to update the unity to its latest firmware pls? Thx
```

---
## \#1639 Posted by: ducktaperules Posted at: 2019-06-02T12:01:45.381Z Reads: 181

```
Went out for some more riding today. no more random cut-outs which was good so it looks like it was remote calibration. I did have another issue tho. I parked up at the local pool for a swim and after i came out and powered up my board my motors wouldn't spin properly.

https://photos.app.goo.gl/Z7bhoqHVQ1143W5J7

Tried a power cycle but still the same. Opened the unity app and did a read config to find that all motor calibration values and hall sensor data had been lost. All other settings were there jut not motor calibration. Did the calibration again successfully but couldn't get it to write calibration values. After a few calibration attempts it finally wrote the values and everything went back to working again.

After that i rode for another 8 miles without a problem.
```

---
## \#1640 Posted by: goldrabe Posted at: 2019-06-02T12:11:11.676Z Reads: 180

```
You need the latest Focbox UI or FOCBOX Tool, @Deodand linked it a few comments further up. Then hit the Firmware tab select the Firmware and hit Upload. It's recommended to do this via USB if you have a Windows machine available.
```

---
## \#1641 Posted by: Balth81 Posted at: 2019-06-02T12:21:57.151Z Reads: 176

```
@Deodand I had a couple random resets to default values now happened again today after putting in a new controller.. re ran set up and all is well like @ducktaperules said it takes a few goes to get it happening via Bluetooth.. it’s always been when i
I have just turned it on.. for me the giveaway is that the remote won’t work as ppm is turned off again.. it’s a bit annoying.. on a side note I will say the flipsky vx1 remote works great with the unity and cruise control is a fun feature for just rolling along at a slow speed .. I find it more comfortable than my nano-x as well..
```

---
## \#1642 Posted by: Toughook Posted at: 2019-06-02T12:27:48.578Z Reads: 175

```
I also use the Maytech MINI remote with 2x settings Slow/Fast. For the Unity I calibrated in Fast Mode, and the difference when riding in Slow mode afterwards is definitely the stated 70% of full throttle, with a much gentler accel curve.

The odd thing for me is my previous setup was a dual Focbox over CAN and I know I didn't calibrate in Fast Mode for this because I was a total noob back then and didn't even know the remote had a fast mode !! Remote didn't come with any instructions and I just 'winged it' using the BLDC Tool and got things going. About a month later I read about the extra mode and started using that all the time and NEVER had a cut out or anything, not once, and I didn't do any recalibrating either. Why would the old FocBox not be susceptible to this behaviour but the UNITY is so affected by it ?
```

---
## \#1643 Posted by: Hatman30 Posted at: 2019-06-02T12:35:34.347Z Reads: 173

```
I’ve only got a Mac . Any options ? Thx
```

---
## \#1644 Posted by: goldrabe Posted at: 2019-06-02T12:40:33.978Z Reads: 172

```
Android phone?\
Friend with a Windows machine?\
The App for Mac is under it's way but will take some more weeks until completion. Are you still on the very first Firmware?
```

---
## \#1645 Posted by: Hatman30 Posted at: 2019-06-02T12:43:34.420Z Reads: 174

```
Yup
Installed using a mac wuth unofficial software
```

---
## \#1646 Posted by: Hatman30 Posted at: 2019-06-02T12:44:03.697Z Reads: 174

```
10char.....
```

---
## \#1647 Posted by: Hatman30 Posted at: 2019-06-02T12:51:05.762Z Reads: 174

```
Yup . Any issues I should know about ?
```

---
## \#1648 Posted by: goldrabe Posted at: 2019-06-02T13:00:52.240Z Reads: 173

```
The new Firmware requires the new Tool or UI someone needs to update this for Mac, as far as I know you are stuck at the moment.\
```

---
## \#1649 Posted by: Deodand Posted at: 2019-06-02T16:24:41.856Z Reads: 174

```
I'll have a look into the EEPROM code to see if I can track down what' causing bad reads.
```

---
## \#1650 Posted by: Hatman30 Posted at: 2019-06-02T18:25:14.195Z Reads: 172

```
how long until an IOS app? As im currently running on stock firmware.
```

---
## \#1651 Posted by: venom121212 Posted at: 2019-06-03T03:15:19.677Z Reads: 173

```
This happened to me as well... EXACTLY as you described. The app wouldn't write the configuration after I reran motor detection. It finally wrote after 5 minutes of sheer confusion. Nothing abnormal happened the ride before.
```

---
## \#1652 Posted by: niuva Posted at: 2019-06-03T04:01:00.974Z Reads: 185

```
According to Enertion newsletter, this fall.
![image|323x499](upload://8R9XUWjB897m47JclyEmtQeSC17.jpeg)
```

---
## \#1653 Posted by: McErono Posted at: 2019-06-03T08:29:55.060Z Reads: 181

```
Latest Newsletter https://mailchi.mp/enertionboards/enertion-newsletter-volume-10-issue-2544885?e=e5102c3c33
```

---
## \#1654 Posted by: FranciscoV Posted at: 2019-06-03T12:04:52.355Z Reads: 181

```
Oh yeah.  “Minor bug fixes” No big deal 🤣🤣🤣 ![image|281x499](upload://pkrH7c0Dj39pL7j4e8RNhISMvNf.jpeg)
```

---
## \#1655 Posted by: billappleton Posted at: 2019-06-03T13:41:05.182Z Reads: 180

```
My board runs great, but I haven’t updated Unity in months. Should I update to the new firmware?
```

---
## \#1656 Posted by: epss4 Posted at: 2019-06-03T13:58:46.866Z Reads: 180

```
Yes
10char
```

---
## \#1657 Posted by: Jaydawg56 Posted at: 2019-06-04T01:58:02.668Z Reads: 179

```
Ha. You and me both. No issues whatsoever, almost a little scared to update the firmware.
```

---
## \#1658 Posted by: venom121212 Posted at: 2019-06-04T02:33:18.014Z Reads: 181

```
@billappleton  @Jaydawg56

Same boat. Updated 3 days ago and still no issues.

https://giphy.com/gifs/adventure-time-thumbs-up-jake-the-dog-HaC3m9r4JFjPi
```

---
## \#1659 Posted by: McErono Posted at: 2019-06-04T10:11:57.911Z Reads: 173

```
23.44 firmware, no issues (anymore) so far.
```

---
## \#1660 Posted by: Toughook Posted at: 2019-06-05T10:50:48.953Z Reads: 175

```
@Deodand hi there. I'm happily running a batch 1 & 2 Unity right now on fairly standard settings. Since the FW update things seem to have settled down thankfully so I'm now looking at the more nuanced part of tweaking in the APP.

I can't find a concise and clear explanation of what are, and what the benefits are, to changing things like Positive Throttle Ramping Time for example, or what happens during a Thermal Throttle. Do I need Traction Control ? 

Is there a proper manual somewhere that I've overlooked where these things are explained ? 

![Screenshot_20190605-113911|243x500](upload://2ZAEEyMCrmagpUrAyztvksm0scj.jpeg) ![Screenshot_20190605-114003|243x500](upload://m5ADYeFJ18SDwtWqVzH6nNJRl5M.jpeg) 

Thanks, Tony
```

---
## \#1661 Posted by: LEE Posted at: 2019-06-05T11:12:22.201Z Reads: 176

```
https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/874

Slow ramping times are good for high torque drives and 4WD.
Fast ramping times are suitable for slow-responsive drives such as direct drives and high gear drives.
In addition, setting of ramping time is effective, even when you release the throttle and shift to neutral.
Drives with high back torque may wobble the board when the throttle is released.
By slowing down the ramping time, you can suppress the momentary wobble caused by the acceleration on and off.

I also want to hear about thermal throttle and traction control.
```

---
## \#1662 Posted by: McErono Posted at: 2019-06-05T11:22:18.754Z Reads: 170

```
Thermal throttle is a safety feature for the motors. Reaching the limit - current drops. But not all motors have thermal sensors.

TC - equals rpm out between motors. The erpm limit decides when TC is engaging. Sometimes you have equal speced motors but one is just behaving different than the other. Or you loose traction on one motor for whatever reason... this is when TC comes in handy
```

---
## \#1663 Posted by: LEE Posted at: 2019-06-05T11:35:38.672Z Reads: 170

```
Is traction control like a limited slip differential?
Is traction control a function to suppress wheel spin by setting the difference in rotation between left and right?
Will I get a diff lock when I turn off traction control?
I'm sorry to ask a lot of questions.
```

---
## \#1664 Posted by: ducktaperules Posted at: 2019-06-05T13:59:51.662Z Reads: 169

```
if traction control is off then its similar to having an open diff where wheel speeds don't affect each other at all. 

With traction control on there is a maximum Erpm difference allowed between the wheels. The allowed erpm difference is for cornering where one wheel might go faster than the other. Once this erpm limit difference is exceeded it assumes that one wheel has lost traction so diverts power to the slower wheel which should still have grip.

i guess enabling traction control and setting the max erpm limit to 0 would be the same as locking the diff.
```

---
## \#1665 Posted by: LEE Posted at: 2019-06-05T16:32:21.992Z Reads: 167

```
@McErono @ducktaperules
Thank you for your detailed explanation.:smile:
```

---
## \#1667 Posted by: ShredRedwood Posted at: 2019-06-06T23:35:14.895Z Reads: 168

```
Welp, I sampled the fine flavors of my first eboard turd sandwich today.  Managed to wash it out at around 25mph, so it wasn't the fault of the Unity.  After the crash though, I flipped the board back over and she seemed to ride at least somewhat fine.  Stopped a mile later when I realized the mount for my box that holds the unity was bent and bent it back into place.  When I gave my throttle a tap to check things, the motors just twitched like they were having a seizure.  Did a power cycle and things rode seemingly okay to get it the last few miles home. After tending to my road rash I got back to the board and my right wheel was locking up or just not spinning when I hit the throttle.  So I plugged the unity in and ran a motor calibration.  Noticed this is more than a bit off.  Does this mean that my sensor is just broken? After a calibration it still rides but that motor is a little jittery from a stopped start. ![that's%20not%20supposed%20to%20look%20like%20that|690x333](upload://rBOEJjp5YjNVmepdeMsqcVymYpa.png)
```

---
## \#1668 Posted by: Balth81 Posted at: 2019-06-06T23:49:45.944Z Reads: 166

```
I would first check the sensor cables if this is loose or damaged it could cause bad connection and ruin the detection
```

---
## \#1669 Posted by: ShredRedwood Posted at: 2019-06-07T00:11:47.491Z Reads: 164

```
Thanks for the reply. I thought I'd checked them but after a closer look it looks like a single wire got pulled from the connector.  So that's an easy fix.
```

---
## \#1670 Posted by: jackluis Posted at: 2019-06-07T14:32:50.230Z Reads: 162

```
I just lost an entire battery pack because my unity let it drop to 25v. These are the settings I had

![Screenshot_20190607-102615|243x500](upload://lf3zxUqtyVy5Pk4B4VlNV1KlGOR.png)
```

---
## \#1671 Posted by: Sn4pz Posted at: 2019-06-07T14:54:58.041Z Reads: 157

```
Your picture isnt viewable

How did it get to 25v? Did you let it sit? Or was this during riding?
```

---
## \#1672 Posted by: Jinra Posted at: 2019-06-07T15:11:25.523Z Reads: 157

```
To be fair the Unity isn't a BMS and doesn't really have any BMS features. You should be using a BMS or be more diligent about leaving it on. If your complaint is about the switch failing and the unity being constantly on, then that's a different matter.

What series pack are you running? If you're at 10s or lower your pack should still be fine.
```

---
## \#1673 Posted by: FranciscoV Posted at: 2019-06-07T15:20:28.118Z Reads: 157

```
Unity seems to be under heavy enemy fire after reported incidents and fw issues!      To be fair.   Mines have been working just fine after latest fw update.   Woohoo 🤘🏼🤘🏼
```

---
## \#1674 Posted by: epss4 Posted at: 2019-06-07T15:22:02.816Z Reads: 154

```
Mine work perfectly too , i will buy another now if they have them in stock
```

---
## \#1675 Posted by: jackluis Posted at: 2019-06-07T15:28:04.951Z Reads: 153

```
Its a 10s. And this happened while riding. The Unity let me keep riding past the 31v cutoff I set in the app. The battery wont charge now either.
```

---
## \#1676 Posted by: Jinra Posted at: 2019-06-07T15:31:15.376Z Reads: 153

```
BMS probably doesn't want to charge because voltage is low, but the pack likely isn't dead. Just measure each group to see what voltage they're at, these cells are tested down to 2.5v per cell.
```

---
## \#1677 Posted by: Jinra Posted at: 2019-06-07T15:33:41.860Z Reads: 151

```
What were your LVC start/end settings? You should've experienced a scaling decrease in power from the start LVC to end LVC.
```

---
## \#1678 Posted by: jackluis Posted at: 2019-06-07T15:37:41.911Z Reads: 154

```
It happened while riding, here's the pic![Screenshot_20190607-102615|243x500](upload://lf3zxUqtyVy5Pk4B4VlNV1KlGOR.png)
```

---
## \#1679 Posted by: jackluis Posted at: 2019-06-07T15:38:52.072Z Reads: 153

```
![Screenshot_20190607-102615|243x500](upload://lf3zxUqtyVy5Pk4B4VlNV1KlGOR.png)
```

---
## \#1680 Posted by: jackluis Posted at: 2019-06-07T15:39:27.042Z Reads: 147

```
how would you recommend I charge them back up?
```

---
## \#1681 Posted by: murloc992 Posted at: 2019-06-07T15:39:46.823Z Reads: 151

```
[quote="Jinra, post:1672, topic:77861"]
To be fair the Unity isn’t a BMS and doesn’t really have any BMS features.
[/quote]

[quote="CarlCollins, post:635, topic:77861, full:true"]
Unity comes with the battery protection system already so all you need to do is get any charge only BMS. Any 2.4 Ghz remote will work with it.
[/quote]

I LOVE contradictions.
```

---
## \#1682 Posted by: Jinra Posted at: 2019-06-07T15:40:04.381Z Reads: 152

```
You could bypass the BMS to charge until you get to a voltage that the BMS will accept (about 30v+)
```

---
## \#1683 Posted by: jackluis Posted at: 2019-06-07T15:40:17.874Z Reads: 154

```
sounds like Enertion owes me a battery :eyes:
```

---
## \#1684 Posted by: Jinra Posted at: 2019-06-07T15:41:29.650Z Reads: 155

```
The unity only really has LVC which is the only BMS-like feature, but yea, it doesn't have full fledged BMS features. Unsure as to why LVC was ignored by unity in @jackluis's case.
```

---
## \#1685 Posted by: Blasto Posted at: 2019-06-07T15:41:56.681Z Reads: 152

```
What is the voltage in the HUD?
```

---
## \#1686 Posted by: murloc992 Posted at: 2019-06-07T15:42:52.513Z Reads: 152

```
[quote="Jinra, post:1684, topic:77861"]
Unsure as to why LVC was ignored by unity in @jackluis’s case.
[/quote]

Everything about Unity is "Unsure" tbh. I am happy it works for other people, don't get me wrong. I just feel that risk is still there.
```

---
## \#1687 Posted by: Blasto Posted at: 2019-06-07T15:43:34.290Z Reads: 150

```
if the pack is unbalanced, the total voltage of the pack may be within the range of the LCV, but if one pack is low, the bms maybe preventing charging
```

---
## \#1688 Posted by: Jinra Posted at: 2019-06-07T15:43:47.317Z Reads: 153

```
I wouldn't say that. I'm not an engineer and can only speak to features I know of on VESCs and the Unity.
```

---
## \#1689 Posted by: Jinra Posted at: 2019-06-07T15:44:16.274Z Reads: 150

```
Ah that's true, though that's a huge inbalance if that's the case.

@jackluis You think you can measure each parallel group to see the voltages?
```

---
## \#1690 Posted by: jackluis Posted at: 2019-06-07T15:45:14.899Z Reads: 149

```
thanks appreciate it. I am going to replace the battery anyway just in case.
```

---
## \#1691 Posted by: jackluis Posted at: 2019-06-07T15:46:47.217Z Reads: 148

```
Yes, once I get into the shop but idk when that will be.
```

---
## \#1692 Posted by: jackluis Posted at: 2019-06-07T15:47:09.018Z Reads: 152

```
25v 10char
```

---
## \#1693 Posted by: LEE Posted at: 2019-06-07T15:49:55.974Z Reads: 151

```
Stop riding if it falls below 3.4V per P group.
This will avoid some troubles.
Using a voltage tester and measuring the voltage of each P group may indicate the cause.
```

---
## \#1694 Posted by: McErono Posted at: 2019-06-07T15:52:02.576Z Reads: 154

```
The unity app HUD says 25volts (you switched the HUD from % to volts) and the 31volt cutoff was ignored while riding?! 

Anyone else? I never rode my board near the cutoff but if one unity is doing it all would.
```

---
## \#1695 Posted by: Blasto Posted at: 2019-06-07T15:53:58.153Z Reads: 153

```
[quote="McErono, post:1694, topic:77861"]
(you switched the HUD from % to volts)
[/quote]

I would have a good chuckle if that is not the case
```

---
## \#1696 Posted by: McErono Posted at: 2019-06-07T15:56:46.420Z Reads: 149

```
Just curious.. we had it all :yum: exactly 25volt looks strange... 25.6v something you know .
```

---
## \#1697 Posted by: jackluis Posted at: 2019-06-07T16:28:05.993Z Reads: 151

```
It is 25.something I just can't remember cause I checked it before I left to work this morning. This new battery isn't gonna pay for itself
```

---
## \#1698 Posted by: Sn4pz Posted at: 2019-06-07T16:34:52.737Z Reads: 157

```
I have a hard time believing that the Unity, even for what it is, allowed your battery to hit 25v. I would do multimeter tests on your balance wires to check your P groups.

I don't know what BMS you're using, but isn't 2.8 a common number for Overdischarge protection(for li-ion)? I can't see why your BMS would let the cells discharge to 25v :thinking:
```

---
## \#1699 Posted by: Jaydawg56 Posted at: 2019-06-07T16:44:01.006Z Reads: 153

```
Guess you’ll never be buying one again then, haha
```

---
## \#1700 Posted by: Jaydawg56 Posted at: 2019-06-07T16:47:11.023Z Reads: 151

```
No, my unity worked as advertised.  I hit the 31v hard cutoff and crawled home the last 2 miles because of it. That feature is working fine
```

---
## \#1701 Posted by: McErono Posted at: 2019-06-07T18:20:15.513Z Reads: 154

```
You have a BMS in there? Charge only or charge and discharge BMS?
```

---
## \#1702 Posted by: RobPBody Posted at: 2019-06-07T18:35:14.310Z Reads: 154

```
Hey All,

Can someone point me to
A link to buy a new Anti spark
Switch for the Unity? Looking for the same model that ships with the Unity.
```

---
## \#1703 Posted by: Jinra Posted at: 2019-06-07T18:52:06.022Z Reads: 153

```
The unity has a built in switch. You wouldn't need an antispark. If you don't like the momentary switch that the Unity comes with, you can use any SPST/SPDT power switch, but you will have to adjust the timeout of the Unity to 1.5s
```

---
## \#1704 Posted by: jackluis Posted at: 2019-06-07T19:06:55.256Z Reads: 149

```
Charge only. Just bought a 60a charge/discharge BMS , not trusting the unity anymore.
```

---
## \#1705 Posted by: Slydunan Posted at: 2019-06-07T19:11:38.534Z Reads: 154

```
Does anyone constantly get this error when scanning the bluetooth? More than half the time when im trying to connect ill get this error, and i have to restart the app multiple times to get it to scan and connect. Usually it takes 2-5 additional attempts but yesterday it kept repeating this error 10-15 times before it actually worked.

![Screenshot_2019-06-07-15-07-13|230x500](upload://xZ9ePVA0r0VONQDzbEmfO8I1kho.png)
```

---
## \#1706 Posted by: McErono Posted at: 2019-06-07T21:22:24.607Z Reads: 148

```
BT is rockstable for me since fw 23.44.
```

---
## \#1707 Posted by: Balth81 Posted at: 2019-06-07T21:31:57.221Z Reads: 155

```
I get this issue heaps with my unity..it’s worse if I’m connected to my metr module usually if I disconnect it the unity app connects ok.. 

[quote="Slydunan, post:1705, topic:77861, full:true"]
Does anyone constantly get this error when scanning the bluetooth? More than half the time when im trying to connect ill get this error, and i have to restart the app multiple times to get it to scan and connect. Usually it takes 2-5 additional attempts but yesterday it kept repeating this error 10-15 times before it actually worked.

![Screenshot_2019-06-07-15-07-13|230x500](upload://xZ9ePVA0r0VONQDzbEmfO8I1kho.png)
[/quote]
```

---
## \#1708 Posted by: Balth81 Posted at: 2019-06-07T21:43:16.605Z Reads: 156

```
[quote="jackluis, post:1704, topic:77861, full:true"]
Charge only. Just bought a 60a charge/discharge BMS , not trusting the unity anymore.
[/quote]

@jackluis I will say this 60amp May not be enough for your board as your voltage will spike above it and shut down the bms take this from someone who has a charge / discharge bms if it’s not a smart bms you could be in for some trouble too as you won’t onow why it’s turned the battery off until you can get a multi meter on it.. I now have 100amp charge/discharge smart Bluetooth bms and have discharge set to 150a max and don’t get any cut outs.. the other fun thing you get with this style bms connected charge/discharge is cut outs when the battery is close to full and you go down hill at start of your ride ... it will sometimes push it past the full charge and trigger overcharge protection turn your board off and leave you to foot break... bottom line is you need to really know your stuff to set the bms up properly.. I read through all your posts and agree with the others it seems very odd that the unity would let you get to 25v my guess would be that the battery it’s self has and issue like a broken weld/solder somewhere causing a group to not be connected.. but your first step like the others said is to test from the balance leads .. the only reason it won’t charge is due to the bms fail safe being triggered which you can’t tell if it’s not smart.. I had a bms issue where it wouldn’t charge because the cells became unbalanced due to the balance plug coming partially loose and unbalancing the cells past the tolerance..  I have taken my unity right down to 0 and never has it dropped below the specified voltage.. to charge back up as some others have said bypass the bms to bring back to 30v ish but be careful as if there is other issues it could further unbalance the battery..
```

---
## \#1709 Posted by: jippijuk Posted at: 2019-06-07T22:12:37.048Z Reads: 156

```
After updating my unity with 1.3 , first ride after during the ride the unity just shut down. After a couple min turned back on without any doing and continued the ride . At the end I could not turn of the unity , the switch is not responding at all . After disconnecting power and reconnect- the switch turns the unity on normal , but can not turn of . Upload firmware again , resetting- same thing happen . Is that a bug problem as well ?
```

---
## \#1710 Posted by: Deodand Posted at: 2019-06-08T00:24:16.052Z Reads: 150

```
Can you please share a video with the switch not working and the behavior plugging/unplugging battery?

I think the mechanical switch might be the culprit.
```

---
## \#1711 Posted by: Slydunan Posted at: 2019-06-08T00:44:01.562Z Reads: 152

```
Once its connected it seems stable but all of the versions have had problems getting connected
```

---
## \#1712 Posted by: McErono Posted at: 2019-06-08T00:47:51.531Z Reads: 154

```
galaxy s9plus, no issues connecting at all. in fact its connecting really fast and every time. 2nd batch unity.
```

---
## \#1713 Posted by: billappleton Posted at: 2019-06-08T02:40:38.230Z Reads: 155

```
Updated the firmware, rides great.
```

---
## \#1714 Posted by: RobPBody Posted at: 2019-06-08T02:43:52.621Z Reads: 155

```
Thanks for you reply. I just want a replacement power button that comes with the Unity.
```

---
## \#1715 Posted by: Deodand Posted at: 2019-06-08T03:42:43.038Z Reads: 155

```
The switch is something we sourced in china, I can't seem to find anywhere that sells it in ones or twos. Just to be clear though its just a small momentary switch that passes a signal (almost no power), the circuitry on the unity takes that signal and switches a larger circuit on that lets power through.
```

---
## \#1716 Posted by: Namasaki Posted at: 2019-06-08T03:44:31.980Z Reads: 153

```
That sounds like the same type of switch the hover boards used.
They are available on eBay.
I think I have a couple laying around

![IMG_9544|375x500](upload://80MUzKi3scZhxcGcKcsm6952wzh.jpeg)

Does this look like the one on the Unity?
```

---
## \#1717 Posted by: nuttyjeff Posted at: 2019-06-08T04:21:37.198Z Reads: 146

```
The one on the unity is MUCH smaller.
```

---
## \#1718 Posted by: LEE Posted at: 2019-06-08T04:32:10.632Z Reads: 152

```
![image|666x500](upload://zeeP4IYmkp9r6JrltvK8wWHp2GU.jpeg) 
The small switch on the right is the Unity switch.
```

---
## \#1719 Posted by: Namasaki Posted at: 2019-06-08T04:53:55.395Z Reads: 153

```
I see, it has a very short barrel.
```

---
## \#1720 Posted by: Deodand Posted at: 2019-06-08T05:23:46.387Z Reads: 153

```
Yes, it's what made me love that switch. Such a small envelope. Many hours searching to track that guy down.
```

---
## \#1721 Posted by: RobPBody Posted at: 2019-06-08T05:55:42.118Z Reads: 151

```
[quote="Deodand, post:1715, topic:77861"]
e
[/quote]

The Unity has 4 cables.
```

---
## \#1722 Posted by: LEE Posted at: 2019-06-08T14:12:37.041Z Reads: 151

```
The small switch has expanded the design range of the ESK8 build. Built-in anti spark switch. And by integrating XT60 into one, I can use many batteries.
```

---
## \#1723 Posted by: FranciscoV Posted at: 2019-06-08T20:07:52.363Z Reads: 151

```
Just got finished a new board.  20 miles in and had one of my motor cut out at 35mph under light load.   Got some wobbles but pulled it off.   Unfortunately I wasn’t logging in any data.   Idk if there was a fault code or not.  
Let’s hope this is just user error 😬

Oh yeah.  Running latest fw in this unity as well.   Sketch AF
```

---
## \#1724 Posted by: Gerrycorrado Posted at: 2019-06-08T20:14:19.157Z Reads: 147

```
Please try again and report back (wear protection! Not only your helmet like me..)
```

---
## \#1725 Posted by: Jinra Posted at: 2019-06-08T21:38:26.202Z Reads: 145

```
You only need two
```

---
## \#1726 Posted by: Marsl187 Posted at: 2019-06-08T22:55:53.727Z Reads: 150

```
I have news!

[quote="Marsl187, post:1457, topic:77861"]
The issue is NOT solved.

But it was different this time. After the cutout just one motor was working. The other wasn‘t spinning but braking worked. After restart the unity all was working again. I’m not sure if both motors cut out or just the one. As I remember after the other cutouts I had I didn‘t need to restart the unity to get the motors spinning again.
[/quote]

I wasn't able to reproduce the fault. Was hitting the hill 4 times but nothing. Kinda strange because I haven't changed something since the last time (still newest fw). 

Anyway, seems like it is solved (at least for me) with the latest fw. 

But just out of **curiosity**:

Do you have any idea what the described behavior could have caused? @Deodand

Thank you for your work already! :)
```

---
## \#1727 Posted by: LEE Posted at: 2019-06-08T23:43:22.407Z Reads: 154

```
I also encountered the same symptoms.
It is cut off only for a moment when accelerating at approximately 50km/h or more.
I did not fall, but there was a slight wobble.
It happens about once in one riding.
Whenever it happens, it's over 50km/h when the throttle is on.
This happened with both traction control on and off.
When I put the throttle back to neutral, then I ran as normal.
It is likely to occur when accelerating while maintaining the throttle on for about 4 to 5 seconds.
In order to avoid this, it returns to neutral in about 2 seconds during acceleration and throttles on again.
At high speeds, I avoid throttling on as long as possible.
The firmware is 23.44.
```

---
## \#1728 Posted by: 701Superjet Posted at: 2019-06-09T00:17:35.913Z Reads: 151

```
I also have motor cutout under hard acceleration.
So Ive been out of the game for awhile. I have a first batch Unity. I run 10s5p, 190kv,  75 battery amps, 100 motor amps, street setup... i forget the gearing but i like it low to accelerate quickly. top speed is only 26mph or so. maybe 14t motor and 38t wheel with 97mm wheels I think. From a low speed maybe 3mph or so under full throttle the motors completely cut out. When I first brought this up to enertion I was told it was the motor temperature feature and to increase the values.  That was right after the Unity came out though. Ive been busy with life and haven't messed with my board in quite awhile. After Jumping on here and reading through a month of posts I find that this is a much more common issue. Has the latest FW fixed this problem? I don't see as may posts on it after the FW has been released so im assuming so.. I gotta update when I get home. I just don't want to test it. lol.
```

---
## \#1729 Posted by: LEE Posted at: 2019-06-09T00:26:21.377Z Reads: 151

```
I own two boards that use Unity.  And one without motor temperature sensor certainly has no cut off.
I doubt the temperature sensor.
I turn off the temperature sensor or try changing the settings.
```

---
## \#1730 Posted by: 701Superjet Posted at: 2019-06-09T00:40:24.913Z Reads: 150

```
Agree. It sounds like same issues others have had during high current loads.
```

---
## \#1731 Posted by: Touch415 Posted at: 2019-06-09T05:43:52.736Z Reads: 148

```
This blows 😔😔😔 big time ..
```

---
## \#1732 Posted by: FranciscoV Posted at: 2019-06-09T06:38:22.026Z Reads: 151

```
Exactly my case   2 times today both happened at 35mph   Got some wobbles but no falls.    After that I took it easy and avoided taking it 35mph.    Man.  This is all bad.  To top it off damn Bluetooth connection keep dropping so no faults recorded 
  I feel like I’m riding on eggshells!   board rides fine at cruising speed.   
Get aggressive for a decent period of time and good luck.
```

---
## \#1733 Posted by: LEE Posted at: 2019-06-09T06:59:33.904Z Reads: 150

```
Is your new board a 190KV motor?
My board is a 12s, 220KV motor.
Of the boards I own, the one with no momentary cutoff is the 90 KV torque boards DD board.
Could erpm also be a factor in the momentary cutoff?
```

---
## \#1734 Posted by: mackann Posted at: 2019-06-09T07:08:50.459Z Reads: 149

```
Try increase absolute maximum current to 180A per unitys. Try also disable motor thermal thottling (your 4wd will never get that warm anyway)
```

---
## \#1735 Posted by: Balth81 Posted at: 2019-06-09T07:09:37.015Z Reads: 151

```
Weird I literally had my board 12s5p with dual 190kv 6374’s maxed out with latest version and I get no cuts or drops anymore.. I was riding full throttle maxed at 55km/h for several km’s straight didn’t reduce the throttle at all ... I weigh 120kg’s too so it was working hard I rode for a total of 10km before going for a max speed run on a fun stretch of road.. I would be checking phase wires to see if there is any bad connections as in the early days with unity had a solder break on a phase and carbon up the connection still ran but did weird stuff occasionally like stutter at speed or cog on bench test when going full throttle suddenly and when you accelerate a second time it would go normal.. worth ruling out some of the simple stuff first if you haven’t already
```

---
## \#1736 Posted by: LEE Posted at: 2019-06-09T08:15:58.071Z Reads: 144

```
Thanks for your advice.
I will apply that setting on the next ride.
When I touch the motor, the 4WD is a little bit warmer.
It is almost impossible to get heat damage and it is completely different from 2WD.
When compared at the same speed, the 2WD motor is very hot.
That there is no concern about the heat of the motor is also a merit of 4WD.:grin:
```

---
## \#1737 Posted by: Gerrycorrado Posted at: 2019-06-09T08:17:52.801Z Reads: 142

```
If this fixes the issue, it should be set by default.. Must have been tested eh @Deodand?
```

---
## \#1738 Posted by: mackann Posted at: 2019-06-09T09:18:32.894Z Reads: 143

```
I dont think disable motor thermal thottling make any different. But absolute maximum current can do it if you have high motor A and low absolute maximum current
```

---
## \#1739 Posted by: anders Posted at: 2019-06-09T10:21:09.420Z Reads: 144

```
Have you checked how much voltage sag you have at high load and also your esc temp, I had my remote reciever close to my single focbox and got cutouts only at high power after separating and shielding the reciever no more cutouts. Now I run unity and so far so  good although never go faster than 28mph.
```

---
## \#1740 Posted by: Namasaki Posted at: 2019-06-09T14:09:15.506Z Reads: 140

```
I have 2 builds where the receiver is mounted in between 2 Vesc 4.12  with very little space between and never a problem. 
The receivers are 2.4ghz not Bluetooth
```

---
## \#1741 Posted by: Namasaki Posted at: 2019-06-09T14:16:38.777Z Reads: 142

```
Agree with @mackann
Absolute Max current is a last resort fail safe that you’ll want to set high enough so that it never gets triggered.
```

---
## \#1742 Posted by: Namasaki Posted at: 2019-06-09T14:25:26.156Z Reads: 144

```
This is a screen shot from the BLDC tool.  
I don't know it the Vesc tool has the option to use negative torque to limit erpm but if it does, it needs to be unchecked or disabled.

![28%20AM|593x235](upload://w4uXEJe4nVXRcPScoC0wohUx6a2.png)
```

---
## \#1743 Posted by: FranciscoV Posted at: 2019-06-09T14:34:37.196Z Reads: 143

```
My new board runs on 12s6p 190kv motors. 
Fun factor.  It happened When I wasn’t even full throttle. I was around 50% just a little bit on the aggressive side.   Erpm might be a big factor on this!   Who knows.  All I know is that it happened @35mph both times,  hit 34.5 the day before and had no problem 
I seem to be able to take off from a dead stop with some aggressive throttle.  No problem.   It cruises and rides great up until I hit 35.   Who knows 🤷🏻‍♂️
```

---
## \#1744 Posted by: murloc992 Posted at: 2019-06-09T14:44:35.316Z Reads: 146

```
35 mph.. ~56km/h.. My issue also arose from trying to sustain ~55km/h(~35mph). 12S6P and 170kV motors with 1:4 gearing.
```

---
## \#1745 Posted by: Namasaki Posted at: 2019-06-09T14:46:34.030Z Reads: 147

```
Sounds like you could have an erpm issue.  
One thing to be aware of is that the rated KV of motors is not always the true KV.  
@Jinra wrote a very good article about that.  
Your 190kv motors could be higher or lower than 190kv.  
But Lets say they are 190kv.  
190kv x 50.4v x 7 = 67032 erpm. 
If the unity has an erpm limit of 60000 then your over the limit.

Here is the article on realistic KV

https://www.electric-skateboard.builders/t/realistic-kvs-and-you/23346
```

---
## \#1746 Posted by: FranciscoV Posted at: 2019-06-09T14:59:24.587Z Reads: 147

```
Yeah.   Interesting thing is after the ride @Touch415 and I did a little bit of testing on a thread mill “our ghetto dyno” with me on the board we were able to full throttle it and had no cut outs under load. Shit sure sounds scary lol.  Unfortunately we were not able to read speed due to Bluetooth connection issues haha
```

---
## \#1747 Posted by: murloc992 Posted at: 2019-06-09T15:11:58.246Z Reads: 148

```
My brickphone never lost contact with the Unity though. I don't think my friends old samsung lost it either. Might be the modules..
```

---
## \#1748 Posted by: rideTastic Posted at: 2019-06-09T18:35:32.259Z Reads: 149

```
lol i was riding today until 5% battery and now my raptor 2.1 only charges until 75%. Maybe i had the same?
```

---
## \#1749 Posted by: McErono Posted at: 2019-06-09T19:03:45.367Z Reads: 149

```
His battery is not loading at all. Yours looks more like a BMS issue? Last year a few raptors weren't charging to 100%.
```

---
## \#1750 Posted by: jackluis Posted at: 2019-06-09T19:53:23.472Z Reads: 151

```
Thanks for all the input, I will be checking out my battery to look for broken welds. Could you tell me where I can buy a BMS like the one you mentioned?
```

---
## \#1751 Posted by: mackann Posted at: 2019-06-09T20:46:48.274Z Reads: 149

```
I think Unity have a standard erpm limit of 100k or 120k if I remember right so that value should it never hit
```

---
## \#1752 Posted by: Balth81 Posted at: 2019-06-09T21:06:20.074Z Reads: 155

```
[quote="jackluis, post:1750, topic:77861, full:true"]
Thanks for all the input, I will be checking out my battery to look for broken welds. Could you tell me where I can buy a BMS like the one you mentioned?
[/quote]

This is the one I use with the Bluetooth module but it’s worth getting USB too as Bluetooth only lets you change some settings but pc let’s you fully customise.. then you can just maintain with the Bluetooth..
```

---
## \#1753 Posted by: murloc992 Posted at: 2019-06-09T21:22:03.788Z Reads: 149

```
But is it per motor or combined? I am leaning towards combined..
```

---
## \#1754 Posted by: mackann Posted at: 2019-06-09T21:27:27.269Z Reads: 149

```
Per motor 10 char
```

---
## \#1755 Posted by: Namasaki Posted at: 2019-06-09T22:14:36.448Z Reads: 155

```
[quote="mackann, post:1751, topic:77861"]
I think Unity have a standard erpm limit of 100k or 120k
[/quote]


Are they based on Vesc 6 technology ?
```

---
## \#1756 Posted by: ajplant96 Posted at: 2019-06-09T22:54:37.808Z Reads: 157

```
Okay so my current and hopefully final issue with setting up my unity is that at high speeds applying the brake suddenly rather than gradually, the brakes seem to short out or something like that. I’m trying to work through the settings atm but will try my other remote and check the calibration also this morning. Some details about the build:

Battery is 10s4p using 2600mah cells
BMS is 10s rated for 60a
Motors are 5065 140kv racerstar 
Remote is flipsky vx1 (preferred) but I do have the nano-x also which I’m yet to test after the last of my issues were dealt with
```

---
## \#1757 Posted by: Balth81 Posted at: 2019-06-09T23:16:21.944Z Reads: 155

```
I run both of those remotes and the braking is fine for me love the vx1 .. I am using standard calibration with +30% on the right hand side board handles great..
```

---
## \#1758 Posted by: deucesdown Posted at: 2019-06-09T23:41:27.734Z Reads: 156

```
[quote="ajplant96, post:1756, topic:77861"]
nano
[/quote]

Did you calibrate the remote (move throttle full travel both directions) before takeoff? It's a known thing with nano x
```

---
## \#1759 Posted by: ajplant96 Posted at: 2019-06-09T23:55:57.652Z Reads: 152

```
The issue is happening with the flipsky remote, nano is my spare atm so haven’t actually touched that for this testing yet.
```

---
## \#1760 Posted by: Ashintar Posted at: 2019-06-10T00:16:37.433Z Reads: 150

```
has anyone had the high speed cut out issue running sensorless?
```

---
## \#1761 Posted by: Balth81 Posted at: 2019-06-10T00:18:42.132Z Reads: 151

```
[quote="ajplant96, post:1759, topic:77861, full:true"]
The issue is happening with the flipsky remote, nano is my spare atm so haven’t actually touched that for this testing yet.
[/quote]

Make sure you calibrate in top speed mode (red) on the remote... the vx1 really works well love the cruise control feature..
```

---
## \#1763 Posted by: Aries Posted at: 2019-06-10T00:21:01.690Z Reads: 150

```
Hi may i how did you tune the cruise control feature? mine just keeps increasing speed till it hit the max. Does not maintain the speed at all. Any specific setting?
```

---
## \#1764 Posted by: LEE Posted at: 2019-06-10T01:13:20.553Z Reads: 161

```
![image|666x500](upload://iQPAbeA327oEqWjzEXDOWjqtS9j.jpeg) ![image|666x500](upload://kFYt5e3JECG4kjtBgmsJQDHoOQS.jpeg) 

When connecting to FOCBOX Tool, Absolute Max Current was already set to 180A.
Both master and slave.
Also, Erpm was set to 140,000.
![image|281x500](upload://tmu97ghPP27MDcqqxHZqAU1vGTg.png) 
The motor thermal throttle has been turned off.  I will try in a few days.
```

---
## \#1765 Posted by: ajplant96 Posted at: 2019-06-10T02:25:38.559Z Reads: 149

```
Yeah, made sure too. I like the idea of cruise control but mine seems to either accelerate when I try to use it or start slowing down. Doesn’t wanna hold a constant speed for some reason.
```

---
## \#1766 Posted by: LEE Posted at: 2019-06-10T03:06:07.456Z Reads: 149

```
Even in my case, it was not full throttle.
It happens in a similar speed range.
But will it hit Erpm 60,000 at 35mph?
I have the same suspicion on my board.
```

---
## \#1767 Posted by: lrdesigns Posted at: 2019-06-10T03:19:51.526Z Reads: 152

```
Someone correct me if I am wrong but I don't think the Vesc 4.12 60k eprm limit was a hard limit, its just that above that the DVR becomes inefficient leading it to overheat and burn out. So if you had an issue you would have a dead vesc. Not give cut outs or errors.

Plus it has been stated that Unity does not have such a 60k limit its over 100k.
```

---
## \#1768 Posted by: LEE Posted at: 2019-06-10T03:36:09.595Z Reads: 151

```
Erpm may also be the cause, but I think the possibility is low.
Absolute Max Current was 180A from the beginning.
Other than that, I can only think of a thermal throttle and a remote control connection.
```

---
## \#1769 Posted by: LEE Posted at: 2019-06-10T03:43:08.880Z Reads: 155

```
I don't know if this works, but I set the cutoff start to 39.6 V.Cut off from 3.3V per cell.
Does the VESC Cutoff start wabble the board when the throttle is on?
```

---
## \#1770 Posted by: Balth81 Posted at: 2019-06-10T03:54:59.725Z Reads: 154

```
If you meant wobble then no it doesn’t wobble the board when it’s in Low power mode just goes very slow with reduced braking .. fastest I could get it was 25 km/h [quote="LEE, post:1769, topic:77861, full:true"]
I don't know if this works, but I set the cutoff start to 39.6 V.Cut off from 3.3V per cell.
Does the VESC Cutoff start wabble the board when the throttle is on?
[/quote]
```

---
## \#1771 Posted by: mackann Posted at: 2019-06-10T10:56:09.102Z Reads: 153

```
Looks like you are running battery A 10A on that picture? It looks very low
```

---
## \#1772 Posted by: LEE Posted at: 2019-06-10T11:13:00.067Z Reads: 154

```
The speed reaches 63kph with Batt Max 10A.
There is something I do not understand for a long time.
Everyone likes high Battery Max.
But I can not control it so much.
If two Unitys, total 20A.Is this correct?
Also, can this setting be a factor that causes a cutoff at high speeds?
```

---
## \#1773 Posted by: mackann Posted at: 2019-06-10T11:19:12.916Z Reads: 157

```
Nice, didn't know it was possible with that low value. I gues it could make a problem, not cut of but alot lower torque on higher speed, because on low speed you would still have some torque but on higher speed it will have almost no power with that low.
I suggest raise it to at least 40A per Unity (it will be 80A total then with 4wd) I run mine in 60A per Unity (total 120A)
```

---
## \#1774 Posted by: LEE Posted at: 2019-06-10T11:28:24.465Z Reads: 157

```
Total 120A.:scream:
I am not confident I can control it…
You are a superman.
understood.
Pull up the battery amp setting.
```

---
## \#1775 Posted by: Jinra Posted at: 2019-06-10T13:03:00.080Z Reads: 155

```
Are you serious? 63kph with 10amps? That's pretty crazy :thinking:
```

---
## \#1776 Posted by: murloc992 Posted at: 2019-06-10T13:04:20.363Z Reads: 158

```
![image|500x500](upload://jWJr1iZQBSbre4ir3z3V10x2dyI.png) 

I bet this is on his deck.
```

---
## \#1777 Posted by: LEE Posted at: 2019-06-10T13:27:58.179Z Reads: 154

```
2 Unitys.
4WD.
Total 20A.
```

---
## \#1778 Posted by: murloc992 Posted at: 2019-06-10T13:28:39.519Z Reads: 154

```
33S20P AAA battery pack.
```

---
## \#1779 Posted by: LEE Posted at: 2019-06-10T14:54:32.080Z Reads: 159

```
https://metr.at/r/HJ1gP

It is a log of torque boards DD, 90KV,110mm.
At this time, the setting is 20A, but the maximum is 40A in the log.
Why is this?
```

---
## \#1780 Posted by: oyta Posted at: 2019-06-10T17:53:40.093Z Reads: 149

```
2 * Unity each with 20A battery max = max 40A total battery amps?
```

---
## \#1781 Posted by: Jinra Posted at: 2019-06-10T18:17:04.887Z Reads: 150

```
He said 2 running 10a battery max
```

---
## \#1782 Posted by: Jinra Posted at: 2019-06-10T18:18:23.005Z Reads: 153

```
Maybe the battery max setting for each unity is doubled because of two motors? Then multiplied by 2 unities for 40a
```

---
## \#1783 Posted by: mackann Posted at: 2019-06-10T18:23:36.362Z Reads: 154

```
No, if it like his picture its 10A per unity, = 20 battery A total, will try later on my Thorium X4 to just for sience 😁
```

---
## \#1784 Posted by: Jay1 Posted at: 2019-06-10T18:46:13.804Z Reads: 154

```
Hey @CarlCollins  ! When i bought my unity 03 march , enertion told me i will receive it in april , now last time i chek with you it was june , why the shipping time have double and do you thnk it possible i really receive it in june for sure or its impossible …im really sad because that the only thing and i think some guy receive it but not me. Thanks you my order number is 25369
```

---
## \#1785 Posted by: Jinra Posted at: 2019-06-10T18:49:13.845Z Reads: 153

```
How else would you explain his 40a pull then :thinking:
```

---
## \#1786 Posted by: LEE Posted at: 2019-06-10T19:09:24.093Z Reads: 150

```
Torque boards DD is one Unity.2WD.
```

---
## \#1787 Posted by: McErono Posted at: 2019-06-10T19:14:34.509Z Reads: 149

```
Hmm strange, if you show current in your metr log you can see that its limited to 40amps and it is running a lot on that limit
```

---
## \#1788 Posted by: mackann Posted at: 2019-06-10T19:14:43.039Z Reads: 152

```
Metr log is not same board as the 10A picture
```

---
## \#1789 Posted by: LEE Posted at: 2019-06-10T19:18:40.240Z Reads: 156

```
https://metr.at/r/9rEjB
This is a log of 2 Unitys, 4WD.
At this time, I was limited to 10A or 14A.
However, it is data that seems to ignore the restriction.
I do not understand well.
It is set by the app of Unity and data is acquired by metr.
And it is this board that a momentary cutoff occurs at 50km/h or more.
The motor is not so hot.It's hard for this board to trigger thermal protection.
```

---
## \#1790 Posted by: LEE Posted at: 2019-06-10T19:40:07.681Z Reads: 153

```
Also, since there is no motor temp sensor on the torque boards DD, motor temp is 0.

For battery max amps and logs, there may be something wrong with my metr configuration.
As a cause of the cut off at high speed, I think it is either the thermal throttle on/off or the low setting of the battery max amp so far.
The absolute max amp was 180A from the beginning.
```

---
## \#1791 Posted by: mackann Posted at: 2019-06-10T19:49:22.049Z Reads: 150

```
Go for a test after change it and se, but please be careful and have good protection
```

---
## \#1792 Posted by: LEE Posted at: 2019-06-10T19:58:34.851Z Reads: 156

```
![image|638x500](upload://x7aTQK7qT8CCOTIU06Eo06SSdlA.jpeg) 
Torque boards DD.

![image|638x500](upload://qn4xZ8VrUOYfXJVM8BKcLfVj1IR.jpeg) 
2 Unitys 4WD.

I think that the setting of the motor and gear ratio and the wheel size is not wrong.
GPS and Unity speeds are almost identical.
```

---
## \#1793 Posted by: mackann Posted at: 2019-06-10T20:03:44.048Z Reads: 153

```
Looks good and correct
```

---
## \#1794 Posted by: LEE Posted at: 2019-06-10T20:03:56.144Z Reads: 161

```
![image|256x500](upload://5I9NUc6bQe123Ksyy8Rhtu1KgZS.jpeg) 
As I do not understand English well, I do not understand the meaning of this setting well.
```

---
## \#1795 Posted by: CarlCollins Posted at: 2019-06-11T01:16:43.449Z Reads: 156

```
@Jay1
Apologize for that man! we already released the newsletter with the possible ETA, I think we will make it as per that :slight_smile:
```

---
## \#1796 Posted by: mackann Posted at: 2019-06-11T04:32:36.652Z Reads: 165

```
That is correct settings for dual unity 👍
```

---
## \#1797 Posted by: trampa Posted at: 2019-06-11T07:47:09.428Z Reads: 161

```
No, the Unity is not VESC 6 based. 
Original VESC 6 has three phase shunts with shunt amplifiers and adjustable voltage and current filtering.
This allows the ESC to be very linear and run high RPM motors reliably at max voltage rating.
Unity has two battery side shunts, like VESC 4.xx, Focbox and other VESC 4 based designs. 

There are other differences in design, like dedicated processor vs shared processor and power stage layout, FET choice etc. 

If you are interested in more details:
https://vesc-project.com/node/403
```

---
## \#1798 Posted by: Gerrycorrado Posted at: 2019-06-11T08:16:16.207Z Reads: 156

```
@Deodand any updates on firmware evolution? (tagging you as it "seems" from above the cutout has not been solved.)
```

---
## \#1799 Posted by: CarlCollins Posted at: 2019-06-11T10:49:33.029Z Reads: 158

```
@Gerrycorrado

Have you updated your Unity to 23.44 (the latest one)?
```

---
## \#1800 Posted by: Gerrycorrado Posted at: 2019-06-11T11:04:33.019Z Reads: 157

```
Yes carl, i have. Not that that makes a difference as i cannot ride eh.. I broke my elbow running 23.43 as reported in ticket 80198. 
Im simply pointing jeffrey to the reports just above. Also 44.
As he mentioned he is very busy, i expect him not to followup on a thread just like that, hence the tag ;)
```

---
## \#1801 Posted by: CarlCollins Posted at: 2019-06-11T11:06:09.062Z Reads: 153

```
Looks like to see the real results we have to upgrade the firmware to the latest and then try it again!
But after your recovery (if possible)
```

---
## \#1802 Posted by: Gerrycorrado Posted at: 2019-06-11T11:11:28.791Z Reads: 155

```
Carl, to be honest.. I broke bones. I hope you realize that concrete is not soft and it will take weeks for my to recover. 
If you scroll up you see someone who is still able to ride and has logging capabilities with what it seems still cutout issues on 44. I prefer you ask that person to be honest.
I did offer jeffrey to send all my stuff to fatdaddy (including all my spare 'large' engines so @tricky-fpv could run tests) , but that was last week or week before and seemed not needed as he was finalizing 44 (which  was released 2 days after). I have updated to 44 a couple of days ago so my settings on which i had my accident, are lost
```

---
## \#1803 Posted by: CarlCollins Posted at: 2019-06-11T11:14:06.434Z Reads: 153

```
I understand and I strongly hope for you to have the speedy recovery mate!
I think Jeff will answer him because there are always multiple factors involved in each and every case, because every case has it's own uniqueness, I hope you understand what I meant!

So, we will troubleshoot and update you guys here if it's the fault with the Unity or with something else!
```

---
## \#1804 Posted by: McErono Posted at: 2019-06-11T11:16:03.751Z Reads: 149

```
Hope to get my metr module tomorrow. I have not had any issues with 23.44 but I never hit more than 48kmh/30mph. Some suspect 35+mph to be where issues start.
```

---
## \#1805 Posted by: Gerrycorrado Posted at: 2019-06-11T11:17:37.983Z Reads: 148

```
40kmh is where i had my issue. But im 100kg geared up.
Carl, i hope al issues are gone when i can ride again, otherwise i will be obligated to go elsewhere..
```

---
## \#1806 Posted by: CarlCollins Posted at: 2019-06-11T11:21:04.073Z Reads: 149

```
I do understand man and we are struggling on daily basis to solve each and every issue and make this product as much durable as possible!
```

---
## \#1807 Posted by: Gerrycorrado Posted at: 2019-06-11T11:32:32.379Z Reads: 151

```
Me too with physical therapy 🤣
Until then im +1.000euro in orange paper weights. For the moment all confidence is gone eh. And i was a true believer (otherwise i would not have bought 2+psychobuild+1 (yes, your records show 2 still being processed as the last combo order contains 1 for a buddy))
But i still believe in Deodand..
```

---
## \#1808 Posted by: Deodand Posted at: 2019-06-11T14:23:49.422Z Reads: 155

```
Hey @Gerrycorrado, to the best of my knowledge it seems the issues with the over current are solved. I see some people have reported a couple weird intermittent issues but it seems clear to me the behavior is caused by something else (no reported faults that I know of anyways and very different described behavior). 

If you want me to make some kind of promise that the skateboard you built yourself that I've never seen before will never fail again, well obviously I can't. To do so would be reckless. This sport is dangerous, gear up stay safe and manage your speed. Maybe devise a way to stress test your setup safely. For my part I'll continue doing as much as I can to identify/solve any reported issues. I do feel fairly confident saying an over-current fault shouldn't be the cause of a cutout anymore. 

On that note, if you guys are reporting behavior please try to give as much info as possible. Run "faults" command if you can, logged data is also a help too. I think everyone should also take a moment to remember that there's more than just the unity between you and the board running correctly. Try to troubleshoot and inspect everything (remote, battery, wiring, receiver, motors and unity) in the chain if you experience any weird intermittent issues and report back on what you did. It helps greatly to narrow down any reported issues so we can identify the cause. Photos of your setup showing the wiring and components and screenshots of the app  to show your settings always help too.
```

---
## \#1809 Posted by: FranciscoV Posted at: 2019-06-11T15:14:06.711Z Reads: 158

```
Man.  You must be under a ton of pressure after reading everything we write and complain about in this thread!    Man.  I love my unities, but it’s becoming really really hard to trust them!  

Enertion not giving a shit about injuries makes it even harder!  

Let’s face it.   Who wants a board that is limited to riding conservative at all times not knowing what the outcome will be!!    One thing is for sure.   I don’t!!!          I like to full throttle my shit here n there and apparently that might or might not be an option for Many of us.   

Long story short.   I totally understand why people are getting frustrated about the subject.  I really hope you guys can figure this one out before something really really bad happens to someone in here 

Riding gear can only do so much to protect riders
```

---
## \#1810 Posted by: Deodand Posted at: 2019-06-11T17:26:24.256Z Reads: 158

```
[quote="FranciscoV, post:1809, topic:77861"]
Enertion not giving a shit about injuries makes it even harder!
[/quote]

Seriously man? Of course we care, you realize enertion is like 10 total people on a good day? I get so tired of people demonizing our company when we are just out here trying to develop new exciting products for this community. We will always do our best to patch any bugs that get reported to us ASAP. There has been a recent spike of people prematurely jumping to conclusions on weird behavior with their boards. We need to make sure and identify all the specific behaviors and treat them separately and accordingly. Not just go ME TOO ME TOO and lump all issues into the same vein. The vast majority of unities are out in the wild working great, so we need to identify what about your specific setup is causing issues. 

[quote="FranciscoV, post:1809, topic:77861"]
Let’s face it. Who wants a board that is limited to riding conservative at all times not knowing what the outcome will be!!
[/quote]

Nobody wants that, so lets figure out how to get your setup bulletproof and bug free (like one of the hundreds of other people running unities) before you push it to the limit. 

[quote="FranciscoV, post:1732, topic:77861, full:true"]
To top it off damn Bluetooth connection keep dropping so no faults recorded I feel like I’m riding on eggshells! board rides fine at cruising speed.
[/quote]

Even if the bluetooth were to drop the faults would still be reported. As long as the unity isn't power cycled the faults remain in memory. If you aren't seeing any faults after the behavior than your unity would either be hard resetting (you'd notice complete loss of power for about 5 seconds) or no faults are being triggered. Are the motors cogging? 

@701Superjet make sure to update your firmware it should fix the issue.  

@LEE I have a metr module here as well I'll invesigate the weird battery current logging you are seeing. As an aside I would not recommend running such an asynchronous battery and motor max current, it will produce weird non-linear throttle behavior that will probably not be very predictable feeling.
```

---
## \#1811 Posted by: McErono Posted at: 2019-06-11T17:30:28.105Z Reads: 157

```
@Deodand don't wear yourself out on some frustrated and ignorant posts. Most of us do fully respect your effort AND most of us have no issues anymore.
```

---
## \#1812 Posted by: FranciscoV Posted at: 2019-06-11T18:56:57.773Z Reads: 155

```
Oh brother!!
```

---
## \#1813 Posted by: FranciscoV Posted at: 2019-06-11T19:05:08.454Z Reads: 160

```
Believe me when I say I mean no disrespect my man.   I respect your work since the day you started helping with my other board.   I know you’re working hard to get things going!      That doesn’t eliminate the fact that my equipment is still having issues!   Again.  Different board, different unity and different issue.  
Yeah.  She runs good as long as I keep it below 35.  Dear god if I try to go faster than that!!  most likely I will get hurt!    

I invite everyone to push their unity a little harder than they usually do.   Let me know how it goes.    

Be aware.   Many people don’t report because they don’t even know the problem exists 

Hate me if you want.   I’m just talking based on my personal experience.    

Cheers 🍻
```

---
## \#1814 Posted by: Balth81 Posted at: 2019-06-11T19:41:55.831Z Reads: 165

```
[quote="FranciscoV, post:1813, topic:77861, full:true"]


I invite everyone to push their unity a little harder than they usually do.   Let me know how it goes.    


[/quote]

Since the latest update and I posted this before I have ridden my board at full throttle for several km straight with the current gearing max speed is sitting at 55km/h but previously gearing I had it up to 65 km/h. I weigh 120kg’s myself and with gear and backpack would be pushing 130 kg’s. Dual 6374 190kv Tb motors 12s5p 30q with with full Bms. I no longer have any issues.. previously I was able to get the over current kicker to occur when pushing it for a decent period of time. I also previously back in January as mentioned in another post had an issue with a cold solder breaking on a phase wire and causing a dodgy connection .. which also caused the board to cog when under load. I would say I’m one of the few who put as much load and hard riding through their unity consistently. I even run the throttle at +30% for more aggressive acceleration. I built my board to be a monster because I knew no production board would deliver close to what I wanted..except maybe a bio board @mackann has very similar style build to my board.. but these didn’t exist when I started building ... I run full custom riptide bushes which were a massive upgrade and enabled me to ride to the max.. I have had a few close calls at high speed and seen people come off in front of me.. but it won’t stop me pushing the limits.. I have spent many hours honing my build and refining every part .. I have confidence in my unity. I also have 2 friends locally with them who weigh less but also push their boards to the limits and they have no issues either... 

We have just gone in to winter here which sucks as it means not so much riding.. pre winter I commuted to and from work on my board daily.. 

Hope that helps..
```

---
## \#1815 Posted by: rideTastic Posted at: 2019-06-11T19:51:14.058Z Reads: 173

```
I still "support" you guys
My raptor 2.1 has a defective hall sensor. Bara immediately sent me an exchange motor. Unfortunately it hasn't arrived yet. Maybe it's not up to you but it would be cool to get it soon. Besides, my BMS has given up the spirit and bara has just initiated me an exchange. Hopefully it will also arrive and not like my replacement motors which have been stuck somewhere for a month.

I have mixed feelings. Actually, you have always helped me directly but unfortunately nothing has arrived so far and the stories from the internet from other customers are sometimes very negative and frighten off

and somethings you did were really not good but i don't want to offtopic this thread

![Screenshot_20190611-214633_Gallery|243x500](upload://qJKA0qYp3kWwRzSecuoHa5l5Tcs.jpeg) !+
![20190611_215304|375x500](upload://8wm46fgv90dprNiqrnPM1FDcNdS.jpeg)
```

---
## \#1816 Posted by: niuva Posted at: 2019-06-13T20:44:24.564Z Reads: 169

```
All of a sudden today my Unity (FW 23.44) with stock BT (First batch 1.1) module now gets stuck on "Connecting to Vesc" in Xmatic app. Had been working before.  In the Xmatic bluetooth settings I can connect to the Unity BT module just fine, but it doesn't show the telemetry data anymore. I sent my debug log via the Xmatic app. Rebooted my phone (iOS) and re-installed the app. I doubt that this has anything to do with the communication between the phone and the Unity BT, but instead the BT module not being able to communicate with Unity. Also cannot connect to the desktop tool anymore.

Ripped open my enclosure and stuck an old HM-10 module in there and works fine. 🤔

@Deodand is it possible that the voltage spikes are frying the Unity BT modules? No communication between the (first batch) SKB369 nRF52 module and Unity via RX/TX due to something being fried?

I'd buy a new SKB369 module and replace the old one by soldering it on the BT PCB, but since the stock one is (probably) loaded with custom firmware I doubt it would be of any use, since starting to program my own NRF modules is not something I'm looking forward to. Starting to consider buying a Metr Unity module, but worried my Unity will fry that too.

Not sure anymore in which thread to post this, Xmatic or Unity troubleshooting. Posting in both.
Also made an Enertion support ticket.

Log from Xmatic app:
https://pastebin.com/UZxpeWHW
```

---
## \#1817 Posted by: DJase Posted at: 2019-06-13T21:00:51.413Z Reads: 162

```
I was thinking the chips could be getting fried too but I am not versed enough in motor controllers to assume that. I ended up grabbing the metr unity because of the bt issues some have and that I couldn't get my old android working so I'm stuck with ios atm. Great question to ask though
```

---
## \#1818 Posted by: Balth81 Posted at: 2019-06-13T21:45:13.513Z Reads: 170

```
I could never get xmatic to ever connect to my unity so I just got a metr module instead.. I’m shocked it worked at all.. can you connect via normal android app?
```

---
## \#1819 Posted by: niuva Posted at: 2019-06-13T21:47:45.768Z Reads: 169

```
I don't own an Android device so I can't test that. Nor does Enertion yet provide an official iOS app. (Which is in the works and supposed to be released this fall.)

Been using Xmatic for quite some time now, regardless of the Uniity bluetooth issues I've been having. Today it just decided to stop working.
```

---
## \#1820 Posted by: rsalmon Posted at: 2019-06-14T01:37:36.992Z Reads: 166

```
[quote="Deodand, post:1810, topic:77861"]
If you aren’t seeing any faults after the behavior than your unity would either be hard resetting (you’d notice complete loss of power for about 5 seconds) or no faults are being triggered.
[/quote]

Hey Jeff, out of curiosity, what could possibly cause a hard reset during a ride?
```

---
## \#1821 Posted by: accrobrandon Posted at: 2019-06-14T17:58:25.528Z Reads: 167

```
Just updated to new firmware... I dont remember what the values were when i setup unity a few months ago BUT should i be concerned about the hall values (or lack of) on motor 1 compared to 2?

![Capture%20_2019-06-14-12-43-44~2|467x499](upload://i7RTtYagxSuAGFkhalehfEeRnKO.png)
```

---
## \#1822 Posted by: Silverline Posted at: 2019-06-14T19:57:38.166Z Reads: 160

```
When mine did that... I did the motor calibration again. And when the gui ask you for spin the wheels manually, i did it more agressive. That did help....
```

---
## \#1823 Posted by: accrobrandon Posted at: 2019-06-14T20:37:21.341Z Reads: 158

```
Yeah u know what was wierd i had to do calibration a few times... The first couple times after spinning em the direction i wanted these bitches were both spinning reverse what i told it... Weird right? 3rd time it was back to.normal...
```

---
## \#1824 Posted by: Blasto Posted at: 2019-06-14T21:32:11.821Z Reads: 165

```
Check your sensor cable connection, seems to be wonky. It shouldn't be intermittent
```

---
## \#1825 Posted by: accrobrandon Posted at: 2019-06-14T21:36:40.931Z Reads: 164

```
Hopefully its just at the unity... Im rear mounted and everything else is stuffed in braid hose =\
```

---
## \#1826 Posted by: Darkest Posted at: 2019-06-15T17:40:23.221Z Reads: 166

```
my Remote receiver has exploded, now my question is the Unity been damaged?  I see no damage on the Unity.![IMG_20190615_183317|666x500](upload://wUHNdezlEFTLml8KyVk0DuUrAWF.jpeg) ![IMG_20190615_183312|666x500](upload://nm4B8YkfGXwrpsq6EbWQEjmj6iQ.jpeg) ![IMG_20190615_182848|666x500](upload://oC99zyNDMwhyBHurmH8oTMGNDym.jpeg)
```

---
## \#1827 Posted by: Shaun Posted at: 2019-06-15T21:52:02.943Z Reads: 162

```
Any advice welcome. Just built my first DIY, plugged everything in, configured the Unity, everything appears to work but I seem to be lacking torque when testing on the bench (I can grab hold of the wheels and stop them spinning). What have I done wrong? I'm using a mac and the fairly standard Unity tool. 

Setup - 10s3p 30Q, Bestech D345 BMS (60A) wired for discharge, 2 x 190kv 6364 Keda sensored motors.
```

---
## \#1828 Posted by: McErono Posted at: 2019-06-16T09:18:52.835Z Reads: 162

```
take it for a real ride. I can hold 12s 6374 motors no problem on the bench.
```

---
## \#1829 Posted by: Shaun Posted at: 2019-06-16T20:30:28.877Z Reads: 161

```
Sorted. Works fine on the road.
```

---
## \#1830 Posted by: RyuX Posted at: 2019-06-17T09:24:51.530Z Reads: 163

```
@CarlCollins

Are you censoring your customers now ?

![image|447x80](upload://yTTci7H5P5CGQYVCgYQsAenpYcS.png) 


![image|690x215](upload://89y1KpdMBed1XrmikRFroZMYfUW.png) 


I am still waiting for a solution for my Order - I demand an Answer!

This is just unacceptable how you treat your customers
```

---
## \#1831 Posted by: McErono Posted at: 2019-06-17T09:42:03.383Z Reads: 159

```
I can tell you a thing or two about it... in my case its about a raptor 2.1 refund. Its staggering...
```

---
## \#1832 Posted by: RyuX Posted at: 2019-06-17T09:45:38.613Z Reads: 158

```
Well basically the set my order on "stop" or "hold" because I told them that I will open a dispute - which I later recalled because they said it will ship on Friday (two weeks ago).

In the End nothing shipped on Friday and they didn't reply to any of my E-Mails for 9 days.

I will reopen the dispute however this is a long process because on my Bank I have to do it via a Form.
I think they just try to push it out of the timeframe long enough so that I can't get a refund or anything.
```

---
## \#1833 Posted by: McErono Posted at: 2019-06-17T09:47:58.895Z Reads: 157

```
Right exactly what they do. Paid 2178aud preorder a year ago... but its no use talking here. I will talk on the other forum freely.
```

---
## \#1834 Posted by: RyuX Posted at: 2019-06-17T09:49:55.551Z Reads: 158

```
What other Forum ?
```

---
## \#1835 Posted by: McErono Posted at: 2019-06-17T09:50:18.584Z Reads: 154

```
Where all top users went...
```

---
## \#1836 Posted by: Sn4pz Posted at: 2019-06-17T10:41:28.074Z Reads: 156

```
Just put your foot down with your CC please. They want your business, and will bend enertion over to get the money you deserve.

Complaining here is like politely asking a robber for your money back, it's pointless.
```

---
## \#1837 Posted by: McErono Posted at: 2019-06-17T10:47:43.714Z Reads: 159

```
In the EU you have mostly 30days for a chargeback after that you are on your own. Believe me I tried...
```

---
## \#1838 Posted by: Sn4pz Posted at: 2019-06-17T10:54:26.009Z Reads: 158

```
Jeez, that's the policy with your credit card? 

Are their policies different for lack of delivery of the product? There has to be a way to receive 100% (not 80) of your money 🤔
```

---
## \#1839 Posted by: McErono Posted at: 2019-06-17T11:05:04.051Z Reads: 156

```
I am afraid it is. Visa and Mastercard = Viseca, 30day chargeback possibility.
```

---
## \#1840 Posted by: CarlCollins Posted at: 2019-06-17T13:40:08.244Z Reads: 159

```
About the censorship, I am not censoring anyone!
And about your order shipment, I think I already replied to it. Please check
```

---
## \#1841 Posted by: CarlCollins Posted at: 2019-06-17T13:40:19.790Z Reads: 160

```
I also replied to your message
```

---
## \#1842 Posted by: RyuX Posted at: 2019-06-17T13:55:25.852Z Reads: 164

```
No you didn't.

This is the last message received from Enertion 9 days back.

I then send the message from my online banking app as evidence and never heard a thing since then.


![Screenshot_20190617-205351_Gmail|281x500](upload://w9QEOz12CBtNWQYpi1MlBH15I2u.jpeg)

I also sent two more emails after that and no response.


The thread was closed and unlisted which kind of makes it a censoring because it will not show up anymore.
```

---
## \#1843 Posted by: banjaxxed Posted at: 2019-06-17T14:13:19.723Z Reads: 162

```
It’s end of July for shipping now according to mail statement, the outsourced support via chat/mail is gone and it’s no big loss frankly, waste of $$ plugged, hope it helps production. Quick response is gone but maybe more accuracy in replies
```

---
## \#1844 Posted by: McErono Posted at: 2019-06-17T14:43:53.561Z Reads: 163

```
I need real answers not formal replies. I need my money. Enertion has 2178 of my AUD for a year now and I have nothing (other than a 71usd shipping bill I paid to return my raptor and was never refunded).
```

---
## \#1845 Posted by: CarlCollins Posted at: 2019-06-17T15:28:56.612Z Reads: 158

```
Will provide as soon as I have it :slight_smile: @McErono
```

---
## \#1846 Posted by: CarlCollins Posted at: 2019-06-17T15:29:31.248Z Reads: 157

```
Replied to your concern on another thread.
```

---
## \#1847 Posted by: auveele Posted at: 2019-06-18T07:33:06.503Z Reads: 154

```
Hi,

yesterday we complete our first build.
Focbox, 10S5P battery, two TB 6374 190Kv

We pair the remote, upgrade the focbox firmware and set up the focbox through FOCBOX UI.
This are our config:
* Motor máx: 80A
* Motor min: -30A
* Battery max: 75A
* Battery min: -20A

And my issue is..
When I put the throttle to max, I see in the FOCBOX UI HUB, the max power to motors are 7V and 8A.

Where could the problem be?
```

---
## \#1848 Posted by: Balth81 Posted at: 2019-06-18T07:51:18.841Z Reads: 149

```
If your bench testing low amp draw is normal as there is no load on the motors.. they spin at max speed.. with little effort..
```

---
## \#1849 Posted by: auveele Posted at: 2019-06-18T07:55:35.195Z Reads: 148

```
I've also tried it mounted on it, 85Kg.
He makes the attempt, but he does not move me.
```

---
## \#1850 Posted by: Balth81 Posted at: 2019-06-18T08:18:22.690Z Reads: 151

```
Can you take screen shots of your Config and hud view with the battery voltage. It will help us see what’s happening.. also are you running a discharge bms?
```

---
## \#1851 Posted by: auveele Posted at: 2019-06-18T08:20:28.407Z Reads: 152

```
No, I'm not running discharge BMS, only charge.

I would post screenshoots this evening, I'm at work now, and I don't have any info here.
```

---
## \#1852 Posted by: Balth81 Posted at: 2019-06-18T08:27:30.143Z Reads: 154

```
It sounds to me like your battery voltage settings are wrong maybe not set to 10s or are set custom.. but need to see what it’s set as in Config.. I run 12s5p same motors and similar settings except I run -55a on motors to increase my braking and it’s awesome but I’m a heavy guy.. :) shouldn’t be too much wrong hopefully..
```

---
## \#1853 Posted by: auveele Posted at: 2019-06-18T08:37:45.741Z Reads: 155

```
I have 10S battery settings..

And what is your battery max?
75A too?
```

---
## \#1854 Posted by: Balth81 Posted at: 2019-06-18T08:42:32.179Z Reads: 160

```
Actually I run battery discharge at 50amp..
```

---
## \#1855 Posted by: Balth81 Posted at: 2019-06-18T08:43:09.082Z Reads: 156

```
You ran motor detection before setting the amps right?
```

---
## \#1856 Posted by: auveele Posted at: 2019-06-18T08:44:57.344Z Reads: 160

```
Yes, I follow the initial guide in the App.
I don't set up the focbox by the BLDC TOOL, only with the FOCBOX UI.
Maybe I need to set up something more...
```

---
## \#1857 Posted by: Balth81 Posted at: 2019-06-18T08:54:37.373Z Reads: 156

```
App (ui) works fine to do full set up.. maybe re run the full set up and make sure it all sticks ..
```

---
## \#1858 Posted by: auveele Posted at: 2019-06-18T08:56:42.797Z Reads: 159

```
I will try again this evening, and comment with the results!

Thanks a lot!
```

---
## \#1859 Posted by: Dams Posted at: 2019-06-18T14:05:52.988Z Reads: 157

```
Hello, I am beginner on this world, I replaced all electronic parts from my old Koowheel electric skateboard, by new 2x 350W Skubull Hub motors and powered by the Unity from Enertion, the accelaration is fantastic, maybe dangerous for me. But I have an big and dangerous issue, with the remote control (Enertion Nano-X Hand Controller), when I start to brake, sometime braking does not work or sometimes jerks.This problem appears more at high speed. I try to change parameters on the Unity, but nothing change. Is somebody met this issue ?
```

---
## \#1860 Posted by: McErono Posted at: 2019-06-18T14:56:10.688Z Reads: 160

```
Let us know your unity settings of the motor and battery tab in the unity app. And what kind of battery you are running.

You do calibrate the remote everytime before you switch the board on? (Power up remote, full throttle, full brake, power up board)

Make sure you did the initial app remote calibration in r-spec fast mode (mode switch in down position).
```

---
## \#1861 Posted by: McErono Posted at: 2019-06-18T20:03:58.960Z Reads: 162

```
[quote="Deodand, post:987, topic:77861"]
Fixing the initial lack of response is due to a property called deadzone, I forgot to add it in the app last release as I planned
[/quote]

Can‘t find it in the latest 23.44 either. not implemented yet Jeff? I just installed my Hoyt puck and 15% deadzone is a lot with the puck for whatever reason.
```

---
## \#1862 Posted by: Deodand Posted at: 2019-06-18T20:50:56.055Z Reads: 159

```
Update will be released this week, I'll add this in as well.
```

---
## \#1863 Posted by: McErono Posted at: 2019-06-19T01:48:35.314Z Reads: 159

```
:flushed: Jeff your avatar! Jeff has been assimilated! :joy: :checkered_flag:
```

---
## \#1864 Posted by: Deodand Posted at: 2019-06-19T01:54:34.879Z Reads: 165

```
There is no Jeff. We are all enertion and all is enertion, praise be to him.
```

---
## \#1865 Posted by: auveele Posted at: 2019-06-19T08:08:14.185Z Reads: 166

```
Hi, yestarday issue was solved.
It was a bad contact of the loopkey, in the anti-spark XT90.

Yesterday we did the first test and it's great.
```

---
## \#1866 Posted by: deucesdown Posted at: 2019-06-19T15:05:19.421Z Reads: 160

```
https://i.ytimg.com/vi/j3Z4GYgWh4I/maxresdefault.jpg

;)
```

---
## \#1867 Posted by: McErono Posted at: 2019-06-20T20:31:53.123Z Reads: 155

```
@CarlCollins 

I wrote Bara a message about my faulty Unity switch but he is not responding. 

Switch does not work sometimes. Can‘t turn on or off the board. Other times its working fine. the nice haptic clicky sound is gone so maybe its not sealed properly anymore? wires and soldering joints are fine.

How do I get a new switch?
```

---
## \#1868 Posted by: Deodand Posted at: 2019-06-20T20:46:49.278Z Reads: 152

```
No clicking seems like a mechanical failure we've seen with some of these switches. There's been a slight mechanical redesign on the internals of the switches for the next batches of unities which should improve reliability there. Are you in the US?
```

---
## \#1869 Posted by: McErono Posted at: 2019-06-20T20:58:00.181Z Reads: 153

```
Switzerland :sweat_smile:
```

---
## \#1870 Posted by: CarlCollins Posted at: 2019-06-20T21:56:47.708Z Reads: 154

```
@McErono

Deodand will be able to ship one to you. @Deodand
```

---
## \#1871 Posted by: TommyCnc Posted at: 2019-06-20T22:27:55.931Z Reads: 158

```
Hey I'm having an issue with my setup I thought it was motor related but seems to be vesc. It acts  erratically. Hold throttle in (slightly) and motors judder then pull me in one direction. Let off throttle, pull again and it judderes and pulls me in the other. Random direction each time. I've run the setup on the android app multiple times and i keep ending up with the same problem. Sometimes change the settings slightly and end up with a squeel and  _drv error.  Control is set to forward/brake so no idea why I'm going both directions with throttle. Please help 😂😭![ui|241x500](upload://jeZO8Q3XxKFBcFMGbPmM6Rfj1j6.jpeg) ![ui|241x500](upload://kWs6qpW5QvhjTM9RHJHnAUelAcw.jpeg)  20000mah 12s (2x6s series) maytech waterproof remote.  I'm thinking of fitting horns to my board and turning it into a rodeo 😜
```

---
## \#1872 Posted by: Balth81 Posted at: 2019-06-20T22:49:44.623Z Reads: 152

```
First it looks like your App isn’t connected?? Your max battery amp is massive .. 120a is huge are you in mountain board or something? I’m 120kg and only run it at 50a and max out my speed everywhere.. when you run Config are you running it the controller in max mode during calibration? I assume your running the newest firmware etc.. your ppm should be at 0 if it’s not doing anything.. motors cogging could also be broken solder (bad connection) on a phase plug or if you have the wrong motor linked to the wrong sensor..
```

---
## \#1873 Posted by: TommyCnc Posted at: 2019-06-20T23:06:19.990Z Reads: 152

```
My app keeps disconnecting, unsure why. I keep having to re connect. Yes mountain board but I just set max battery amps at 120 as Its well within my battery capability, I've tried turning it down and hasn't made any difference. Also my motor max is actually 100amps but I've turned them down too. Controller settings are set OK so I think I was probably holding throttle when I took that screen shot. Solder could well be an issue. I'm the worst solderer! But I did test my wires on a multi meter which showed they were OK but maybe the solder could still be an issue? I noticed my battery amp draw on the app was only maxing around 20 amp even on full throttle and motors were reading up to 100amps (when set to 100) but only around 4 volts, is this normal? I doubt it 🤔. Ive just read upto about message 700 in this thread and a lot of messages about stuttering motors but none about the motors changing direction. Thanks for your reply Balth81

I think I'm running the newest firmware, I have this error come up every time I update After the board has definately been connected through the firmware update. I can't see which firmware I'm running though on the app. [ui|241x500](upload://4xth3yy4lyJXoGA4FTNzBhLtANk.jpeg)![ui|241x500](upload://4xth3yy4lyJXoGA4FTNzBhLtANk.jpeg)
```

---
## \#1874 Posted by: ajplant96 Posted at: 2019-06-20T23:30:57.208Z Reads: 146

```
So when my battery is fully charged and I need to brake the Unity cuts the brakes with like an over current protection message. Is there any way to work around that or do I just have to deal with not having brakes for the first few km of my rides?
```

---
## \#1875 Posted by: venom121212 Posted at: 2019-06-20T23:32:25.464Z Reads: 152

```
Check out rheostatic brakes from @hyperIon1. You wire them in parallel to the battery so over voltage regen gets burned off as heat
```

---
## \#1876 Posted by: ajplant96 Posted at: 2019-06-21T01:08:04.646Z Reads: 152

```
Refuse to shop with them now, too much f*cking around after buying incompatible motors from them and them ditching the conversation when trying to reach a resolution. Plus their site vanished anyway.
```

---
## \#1877 Posted by: accrobrandon Posted at: 2019-06-21T01:16:09.767Z Reads: 151

```
might not be the unity cutting brakes... ive found that with a bestech bms or a discharge bypass that brakes dont cut... but using a cheap bms tends to result in a brake cut out on a full charge....
```

---
## \#1878 Posted by: ajplant96 Posted at: 2019-06-21T01:55:38.016Z Reads: 152

```
Interesting, mine's a generic 10s 60a supposed to be charge only but my new battery builder is saying it's discharge too
```

---
## \#1879 Posted by: Deodand Posted at: 2019-06-21T02:09:15.219Z Reads: 155

```
@ajplant96 

[quote="ajplant96, post:1874, topic:77861"]
with like an over current protection message.
[/quote]

Where are you seeing this message? The unity doesn't have any over-voltage protection unless you are spiking to like 57+ volts (very bad on 10s) 

@TommyCnc I think the bluetooth isn't working correctly within the app and motor config is never being applied. Can you use a desktop and run setup through usb or use a friends android phone? I'm working on an update for the bluetooth firmware that should address this but it'll be a bit till it is ready.
```

---
## \#1880 Posted by: ajplant96 Posted at: 2019-06-21T02:10:51.950Z Reads: 152

```
It's popping up on the HUD under the speedo, etc. Will try to get a photo of it next time I see it but I'll be switching battery/BMS in a couple of weeks so with any luck that'll solve it.
```

---
## \#1881 Posted by: venom121212 Posted at: 2019-06-21T02:53:15.258Z Reads: 154

```
Sorry about your experience. Maytech sells them on eBay or aliexpress.

I have noticed the site down for a while now...
```

---
## \#1882 Posted by: TommyCnc Posted at: 2019-06-21T07:28:27.421Z Reads: 152

```
I'll try get my head around the pc app tonight and program that way. I did try for a few mins last night but I had the same connection issues. I clicked connect and it said connected followed by disconnected a few seconds later every time, but I will persist and try again today and let you know if its solved my issues. Thanks for the reply
```

---
## \#1883 Posted by: drone001 Posted at: 2019-06-26T17:59:55.679Z Reads: 153

```
when I release the throttle after accelerating...there's like a jerk. it's like it releases the power abruptly if that makes sense.
```

---
## \#1884 Posted by: McErono Posted at: 2019-06-26T20:13:22.830Z Reads: 148

```
Thats normal. You have to release throttle slowly.
```

---
## \#1885 Posted by: murloc992 Posted at: 2019-06-26T20:19:39.638Z Reads: 145

```
VESC6 doesn't have this jolt after pinging the remote instantly to neutral. :man_shrugging:
```

---
## \#1886 Posted by: McErono Posted at: 2019-06-26T20:21:25.987Z Reads: 153

```
Yeah my vesc 4.12 board with ack firmware doesn't jolt either. Its a unity thing. Not a fault but its cutting power much faster.
```

---
## \#1887 Posted by: RobPBody Posted at: 2019-06-27T01:18:39.848Z Reads: 154

```
@Deodand Hey, 

Here's something that I just noticed on my unity. Video linked showing issue. Just looking for possible fix for this. 

https://youtu.be/N5-m1e8uTr8
```

---
## \#1888 Posted by: pookybear Posted at: 2019-06-27T01:30:48.070Z Reads: 155

```
Play with your negative ramping.
```

---
## \#1889 Posted by: Deodand Posted at: 2019-06-27T01:35:05.787Z Reads: 157

```
@RobPBody That motor just has slightly more friction. How many motor amps are you running? The command you are sending is a torque not a speed, so if one motor takes slightly more torque to overcome friction than the other the one that begins moving will speed up to full speed while the other is stuck in place. This doesn't really cause any issues in the real world when riding as you will be pumping significantly more motor amps than whatever is running on the bench.
```

---
## \#1890 Posted by: RobPBody Posted at: 2019-06-27T21:08:59.271Z Reads: 152

```
Thank you for your prompt reply. It does have an effect riding because the motor kicks in at full throttle while riding, and it feels similar to someone kicking the motor side of my board, creating a speed wobbles effect in the back.
```

---
## \#1891 Posted by: deucesdown Posted at: 2019-06-27T22:08:32.567Z Reads: 153

```
@RobPBody can you swap the phase wires for left motor and right motor? If the glitch stays with the motor, it's probably as @Deodand said, difference between motors. But if the glitch follows the speed controller side, I'm inclined to believe it's an issue with the Unity?
```

---
## \#1892 Posted by: RobPBody Posted at: 2019-06-27T22:30:29.728Z Reads: 154

```
It's following the speed controller. In the video, I'm testing a new motor, same results. When I get a chance, I'll check the solder joints for the effected side.
```

---
## \#1893 Posted by: Deodand Posted at: 2019-06-27T23:00:07.864Z Reads: 156

```
Hey, yeah it definitely shouldn't be kicking like that, sounds strange.  You didn't answer my question, what motor amps are you running? Can you provide a screenshot of your motor config page?
```

---
## \#1894 Posted by: drone001 Posted at: 2019-06-28T02:21:44.713Z Reads: 154

```
is that in the Unity app?
```

---
## \#1895 Posted by: drone001 Posted at: 2019-06-28T02:24:38.823Z Reads: 154

```
thx, I was having that same issue.
```

---
## \#1896 Posted by: pookybear Posted at: 2019-06-28T02:31:58.423Z Reads: 155

```
Vesc tool. Not sure if it's in the app. I sold my unity a while ago but that's what fixed the jerking when you let off the throttle. Negative ramping is available on all Vesc tool.
```

---
## \#1897 Posted by: drone001 Posted at: 2019-06-28T04:39:23.094Z Reads: 152

```
so am i lowering it or increasing it.
```

---
## \#1898 Posted by: pookybear Posted at: 2019-06-28T04:50:07.206Z Reads: 150

```
Go from 0.2 to 0.3. then try it.
```

---
## \#1899 Posted by: drone001 Posted at: 2019-06-28T04:51:24.569Z Reads: 154

```
got it....thx bruh
```

---
## \#1900 Posted by: sofu Posted at: 2019-06-28T16:42:25.930Z Reads: 155

```
Heads up: Focbox iOS and Android app post is up here for those interested 

https://www.electric-skateboard.builders/t/official-focbox-nexus-for-ios-android/97450
```

---
## \#1901 Posted by: drone001 Posted at: 2019-06-28T23:21:36.191Z Reads: 153

```
what can cause studdering while accelerating hard? It happened during setup but didn't have a load on it so i thought it was from that. after completing the board...it's definitely a studder
```

---
## \#1902 Posted by: Meeep Posted at: 2019-06-28T23:39:46.467Z Reads: 147

```
Sensored or sensorless?
```

---
## \#1903 Posted by: drone001 Posted at: 2019-06-28T23:57:32.205Z Reads: 149

```
Sensored........
```

---
## \#1904 Posted by: Meeep Posted at: 2019-06-29T04:05:29.074Z Reads: 150

```
If it happened during setup I can only advise you to check your phase/sensor connections and their insulation then run the setup tool via windows with usb-c. This is assuming you set up with the app via phone but any bad detection can do weird things.
```

---
## \#1905 Posted by: drone001 Posted at: 2019-06-29T14:50:04.134Z Reads: 149

```
thx bruh.... I have to go inside my enclosure again :grimacing: . honestly after riding last night I think I maybe pushing up on the remote. i didn't get it at all after doing the fw upgrade despite it not giving me a warning.
```

---
## \#1906 Posted by: niuva Posted at: 2019-06-29T17:52:18.093Z Reads: 150

```
[quote="niuva, post:1816, topic:77861"]
Also made an Enertion support ticket.
[/quote]
To which no one has answered in two weeks. ☹️🥺

ID  #21710
```

---
## \#1907 Posted by: Chase Posted at: 2019-06-29T19:15:47.296Z Reads: 149

```
I’ve stayed silent for the most part but if I don’t have a shipping notice by the second week of July I’m calling my card company and going vesc6. Not trying to threaten or be a dick......it’s just enough is enough. I hope they can turn things around but I’m starting to feel stupid when I believe so many missed release dates
```

---
## \#1908 Posted by: CarlCollins Posted at: 2019-06-29T20:37:37.910Z Reads: 144

```
May I have the ticket ID?
```

---
## \#1909 Posted by: Eskate444 Posted at: 2019-06-29T22:18:12.489Z Reads: 146

```
When did you buy?
```

---
## \#1910 Posted by: SkateYS Posted at: 2019-06-29T23:32:31.398Z Reads: 153

```
🔺🔺🔺🔺I think that the Unity UI program needs a "Step up"! The user should not have to rely on what's marked on his battery, what the motor vendor said the motor can handle or his own imagination to setup the FOCBOX UNITY. It's not safe and there are so many people just guessing settings just to build a powerful board. However no matter how good a VESC is, it can fail. That's why the VESC tool asks you for Number of battery cells, capacity, motor size, size of motor and wheel pulleys and wheel size, then runs a motor detection to figure what's the best for your setup. Of course, you can setup manually if you know exactly what you're doing. I haven't seen an official introduction or setup video online which should exist considering how expensive this controller is. Letting noobs guess their own settings could result in many failure reports making the unity look untrusty! 🤷‍♂️
```

---
## \#1911 Posted by: Deodand Posted at: 2019-06-29T23:47:16.715Z Reads: 156

```
@SkateYS have you actually used the FOCBOX UI yet? 

[quote="SkateYS, post:1910, topic:77861"]
The user should not have to rely on what’s marked on his battery,
[/quote]

Selecting the number of series cells in your pack is the same thing as what you do in vesc tool. I don't really see a difference here.

[quote="SkateYS, post:1910, topic:77861"]
what the motor vendor said the motor can handle
[/quote]

The vesc tool just makes a ballpark estimate that isn't necessarily better than a vendors suggestion. I have some plans to have similar suggested current rating in future releases.

We have a guided setup button in the app. Press it and follow the instructions it is really quite simple to use. That said we are hard at work further simplifying the process but it is already quite streamlined and safe. You can go into the vesc tool support thread and find an equal number of confused individuals, everyone needs a little help sometimes. 

Delivery times are something we are definitely 100% focused on fixing. To my knowledge units should be shipping out this week, really sorry that anyone has had to wait so long for their units. After that we have plans in place which should eliminate these huge delays and get things delivered in a punctual manner. If everything goes as planned we will let the results of fast shipped units do the talking :smile:
```

---
## \#1912 Posted by: SkateYS Posted at: 2019-06-30T00:07:02.458Z Reads: 149

```
[quote="Deodand, post:1911, topic:77861"]
Selecting the number of series cells in your pack is the same thing as what you do in vesc tool. I don’t really see a difference here.
[/quote]

You can't see the difference? Your number of cells just tells your VESC what voltage you are about to use! Battery max is about current, how many amps the battery can deliver safely (something many people get wrong by guessing or relying on written C rating)

[quote="Deodand, post:1911, topic:77861"]
vesc tool just makes a ballpark estimate that isn’t necessarily better than a vendors suggestion.
[/quote]
That ballpark estimate from my experiences worked better than any setup I made myself during my couple of years of building and the battery or motor vendors don't suggest you VESC settings! He shows off his product performance (That's why 50C means 50C or less) and those huge motors said 80Amps and VESC says 60amps by actually testing it. 

[quote="Deodand, post:1911, topic:77861"]
go into the vesc tool support thread and find an equal number of confused individuals
[/quote]
I'm not confused at all! This was a customer suggestion to a huge community he is part of. It will not only help noobs (I'm probably one too) and even professionals to keep the unity reputation outstanding!
```

---
## \#1913 Posted by: Chase Posted at: 2019-06-30T01:51:29.801Z Reads: 146

```
Prior to Easter during the sale. I’m not trying to be a dick or rush the process, it’s just at some point, believing all these shipment dates.......
```

---
## \#1914 Posted by: niuva Posted at: 2019-06-30T05:03:25.302Z Reads: 148

```
#21710


[spoiler]10char[/spoiler]
```

---
## \#1915 Posted by: epss4 Posted at: 2019-06-30T16:20:29.093Z Reads: 151

```
Hi guys , im running Raptor 2.1 motor on 12S , and i really don't like my throttle curve and can't find the sweet spot ... will you mind sharing your throttle curve 
or @CarlCollins maybe you have a standar setting for this configuration?can you help me please 
Thanks !
```

---
## \#1916 Posted by: drone001 Posted at: 2019-06-30T16:43:06.022Z Reads: 159

```
How can I set my Unity to just shut off and refuse to even operate when i reach a certain battery percentage/voltage?
```

---
## \#1917 Posted by: Meeep Posted at: 2019-06-30T19:17:21.753Z Reads: 159

```
In the FocBox APP you are going to go to "Config" > "Battery Limits" > "Series Cells" > "Custom voltages." or just go to the battery tab in the full tool. 

"Cutoff start" is when the ESC reduces power and "cutoff end" is when the board will no longer accelerate (i think braking still works but I'm not positive on that.)
```

---
## \#1918 Posted by: deucesdown Posted at: 2019-06-30T19:59:35.182Z Reads: 150

```
Vesc reduces power linearly between cutoff start and cutoff end.
```

---
## \#1919 Posted by: venom121212 Posted at: 2019-06-30T20:00:06.005Z Reads: 154

```
So it throws you on your face at the end of a ride?

Just kidding but seriously consider it
```

---
## \#1920 Posted by: drone001 Posted at: 2019-06-30T21:37:57.520Z Reads: 150

```
lol, that'll probably be better than a dead battery. I'm reading up on this voltage cutoff and start thing now.  is 40.8 cutoff start and 37.2 cutoff end good for a 12s?
```

---
## \#1921 Posted by: CarlCollins Posted at: 2019-07-01T11:53:57.399Z Reads: 152

```
[quote="niuva, post:1914, topic:77861"]
21710
[/quote]

It's the order ID, I need your Support ticket ID
```

---
## \#1922 Posted by: CarlCollins Posted at: 2019-07-01T11:55:07.143Z Reads: 156

```
I am not running my Raptor with 12s so I don't know what settings will be perfect for you.
But I prefer to set the curves around 20-30% horizontal and vertical.
```

---
## \#1923 Posted by: niuva Posted at: 2019-07-01T12:10:03.975Z Reads: 156

```
![40|690x327](upload://vjnWGav3WmbfFFQCc1RBlwKN3jE.png) 

:man_shrugging: Well it's the only ID I have.
The email title cuts off after the U. :frowning:
```

---
## \#1924 Posted by: SkateYS Posted at: 2019-07-01T18:01:59.789Z Reads: 152

```
     🔺Settings Very flexible! If you have a very good range (High capacity cells), then set higher cutoff voltage to go easy on your batteries. They will have more recharge cycles over time!

For 18650 batteries:
 
12s : cutoff end = 38.4v

 10s : cutoff end = 32v



For lipo batteries:

 12s : cutoff end = 40.8v

 10s : cutoff end = 34v
```

---
## \#1925 Posted by: FredXanadu Posted at: 2019-07-01T21:05:01.549Z Reads: 154

```
Hello, i have a problem with my unity. 

Everything was fine and after a charge i can't start anymore my unity ?
No led, no power, nothing... Do you know what can be happen ?
Thanks
```

---
## \#1926 Posted by: drone001 Posted at: 2019-07-01T21:35:56.405Z Reads: 152

```
I had mine set to defaults 40.8 start 37.2 and I still managed to fry the battery. is 45-40 to extreme?
```

---
## \#1927 Posted by: Deodand Posted at: 2019-07-01T22:03:29.875Z Reads: 155

```
Check the integrity of the switch wires maybe?
```

---
## \#1928 Posted by: FredXanadu Posted at: 2019-07-02T01:03:42.218Z Reads: 155

```
il already switch the switch... nothing happen.
```

---
## \#1929 Posted by: SkateYS Posted at: 2019-07-02T04:00:31.699Z Reads: 153

```
45v to 40v sounds good to me! What's your setup? Battery config, bms? A bms failure can still show fully charged battery but no current! So the load will not power on
```

---
## \#1930 Posted by: drone001 Posted at: 2019-07-02T04:09:11.221Z Reads: 151

```
12s6p with an Unity, 6374s, 42-16t soon to be 60-16t.
```

---
## \#1931 Posted by: SkateYS Posted at: 2019-07-02T04:13:15.322Z Reads: 155

```
Some 18650 cells can even be safely discharged down to 3v per cell! (In the long run it's not good tho), I think you re pretty good when it comes to cutoff
```

---
## \#1932 Posted by: SkateYS Posted at: 2019-07-02T04:14:53.382Z Reads: 154

```
switching to 60 - 16t for more torque huh!
```

---
## \#1933 Posted by: drone001 Posted at: 2019-07-02T04:15:32.678Z Reads: 151

```
:grin: yaaaaassss. lol
```

---
## \#1934 Posted by: SkateYS Posted at: 2019-07-02T04:18:41.542Z Reads: 152

```
Make sure not to drop too much on speed tho! But the 12s should help a lot with that! That new gearing will also increase slightly your range and produce less heat on the controllers! Batteries could relax a bit more
```

---
## \#1935 Posted by: drone001 Posted at: 2019-07-02T04:21:50.996Z Reads: 152

```
thx, waiting on belts should have them soon. i hear 60-16t is so much better.
```

---
## \#1936 Posted by: SkateYS Posted at: 2019-07-02T04:24:27.748Z Reads: 154

```
Yup! If you got a sick C rating on that battery and some low KV motors, you could probably bust some willies when you go crazy on take off 😎
```

---
## \#1938 Posted by: deucesdown Posted at: 2019-07-02T06:34:26.756Z Reads: 160

```
[quote="drone001, post:1926, topic:77861, full:true"]
I had mine set to defaults 40.8 start 37.2 and I still managed to fry the battery. is 45-40 to extreme?
[/quote]

https://static.rcgroups.net/forums/attachments/4/3/7/3/1/a6360793-197-Lipoly%20Voltage%20vs.%20State%20of%20Charge.jpg?d=1388084339

from https://www.rcgroups.com/forums/showpost.php?p=28048839&postcount=7

There's really no energy below 3.65v/cell. If you want your lipos to live long, set cutoffs way higher, and tweak as you get more experience with our packs. Stay far away from 0%, as some of your cells will get there earlier than others.

If your cutoff-end was at 40v (3.33v/cell), that's way low.

Plus at least I've found, the last 1/3 or so of the charge on a pack don't seem to have the same punch. Voltage sags down a lot.

So if I were you, as a starting point, I'd set cutoff start at around 40% of the pack (3.8/cell, 45.6v for 12s) and cutoff end at maybe 25% (3.75/cell, 45v for 12s). If you hit cutoff, keep track of how many amp-hours go back in when you charge, then tweak the cutoff if you think it's too conservative.

You can also charge to say 4.15v/cell to lengthen pack life.
```

---
## \#1939 Posted by: McErono Posted at: 2019-07-02T19:58:54.989Z Reads: 154

```
Jeff means you should dismantle the shrinktubes on the switch. Maybe a solderjoint or wire is broken. Make sure after you fixed it to give the switch enough room so it wont be squished at the back by anything. The connections there are very fragile.
```

---
## \#1940 Posted by: drone001 Posted at: 2019-07-03T04:18:29.391Z Reads: 155

```
wow, thx.  I think I understand how these battery packs work.
```

---
## \#1941 Posted by: Tello1969 Posted at: 2019-07-03T23:41:11.156Z Reads: 151

```
How do I connect via Bluetooth? Having issues connecting ![image|666x500](upload://bBsuYGwzN1jl50LABfnHC3PsZx5.jpeg)
```

---
## \#1942 Posted by: goldrabe Posted at: 2019-07-04T00:09:31.432Z Reads: 150

```
Are you on a PC? In Windows Bluetooth is not working, you need to connect the ESC with USB. Bluetooth works only on Android.
```

---
## \#1943 Posted by: CarbonV Posted at: 2019-07-04T18:34:52.502Z Reads: 148

```
Hi guys, when pushing my stick full trottle on 6s and generic hubs I am only using 6A according to the app and getting 22kmh max speed, is that to be expected or is something wrong? 
![Screenshot_20190704-194444|250x500](upload://j568EAUvZGdMKOOYvLaCOgPUUsH.jpeg)
```

---
## \#1944 Posted by: rsalmon Posted at: 2019-07-04T18:59:17.515Z Reads: 143

```
If thats on the bench, unweighted, it actually looks a bit on the high side.

If thats while riding, then you got some pretty efficient hubs.

The Unity will pull whats necessary to overcome the resistance. If you're bench testing, there is not much resistance, it requires very little current to reach max speed.
```

---
## \#1945 Posted by: CarbonV Posted at: 2019-07-04T19:42:07.299Z Reads: 143

```
That was indeed while riding, I do only weigh 64kg plus the board is pretty light and sleek so guess I am good then? :smile:
```

---
## \#1946 Posted by: rsalmon Posted at: 2019-07-04T19:43:50.279Z Reads: 147

```
Nice!

You will see much more current being pulled while accelerating instead of maintaining top speed.
```

---
## \#1947 Posted by: CarbonV Posted at: 2019-07-04T19:49:43.305Z Reads: 141

```
Correct! Thank you for answering :grin:
```

---
## \#1948 Posted by: goldrabe Posted at: 2019-07-04T23:36:08.965Z Reads: 143

```
@Deodand I was one of the guys who had jolts in low speeds after coasting. The last firmware update fixed it for some time, but sadly the jolts returned after around 100-150 mi of usage. This time it's not only after coasting it occurs when starting and maintaining a certain speed also.  My metr.pro module gives also strange ESC temperature readings when the board is idle. I was told that could be caused by the MCU. Any advice or insight would be appreciated.
```

---
## \#1949 Posted by: Blasto Posted at: 2019-07-05T01:10:41.332Z Reads: 147

```
The metr log would be helpfull
```

---
## \#1950 Posted by: goldrabe Posted at: 2019-07-05T02:11:09.239Z Reads: 151

```
Here is the metr.log. The ESC temperature goes down to -273 when the board is idle. I will check for interferences loose connections etc. The strange thing is that the readings where off from the beginning without the jolts. Before the Firmware update it was the same, after motor detection and setup the board works fine for some miles an then the jolts start to happen and are getting stronger each ride.\
![51|281x500](upload://nURqMNjdDHOiXC30NZQEAEH1F1n.jpeg) 
Here is the full log.\
https://metr.at/r/nqmD3
```

---
## \#1951 Posted by: ajplant96 Posted at: 2019-07-05T11:04:29.895Z Reads: 146

```
So I was just out on a group ride on my revived (thanks to the unity) Evolve Carbon GT. Suddenly my speed was limited and attempting to accelerate more than like 5km/hr caused a jerking motion before the unity shut down. Anybody experienced something similar before? Kinda worried as I spent $500 on this to fix the problem of a broken $2000 board in the first place.
```

---
## \#1952 Posted by: venom121212 Posted at: 2019-07-05T13:11:14.134Z Reads: 144

```
Were you close to battery cutoff?
```

---
## \#1953 Posted by: ajplant96 Posted at: 2019-07-05T20:55:31.703Z Reads: 145

```
Battery was at 38% (showing 34.8v), I actually discovered that the remote receiver (Flipsky VX1) was overheating as soon as powered on so I think that could be the issue though and have contacted them about it.
```

---
## \#1954 Posted by: Balth81 Posted at: 2019-07-05T21:49:28.055Z Reads: 144

```
Odd I have the unity and vx1 never had any heat issues on the receiver. Are you using the factory battery?? If you haven’t done battery upgrade your probably getting the famous evolve sag and hitting the cut off ..
```

---
## \#1955 Posted by: mackann Posted at: 2019-07-05T22:06:26.468Z Reads: 148

```
Have you got push to start work with vx1 and Unity?
```

---
## \#1956 Posted by: Balth81 Posted at: 2019-07-05T22:18:31.819Z Reads: 149

```
To be honest I haven’t tried will give it a go later on and let you know ... I can’t see why it wouldn’t work.. have you had issues?
```

---
## \#1957 Posted by: ajplant96 Posted at: 2019-07-05T23:30:00.771Z Reads: 150

```
Battery was upgraded before I switched anything else out from Evolve’s electronics but not a great quality battery hence swapping for 30q cells next week, so could still be sag, but that heat issue does have me concerned. If it’s the remote receiver I’ve still got a spare nano-x for the time being anyway.
```

---
## \#1958 Posted by: mackann Posted at: 2019-07-06T05:09:02.406Z Reads: 149

```
Yea, using button to power on Unity it connects flawless to the remote. But push to start works to turn on Unity but for some reason it dont connect to the remote when started with push to start (it work on same board if I use Nano x)
```

---
## \#1960 Posted by: ajplant96 Posted at: 2019-07-06T05:19:28.360Z Reads: 146

```
Is there any way to make the unity actually remember custom voltage settings? Tried to lower my cutoff from 34v to 32v and it keeps switching to the 9 cells setting when I restart the app to check if it retained the information I’d put in...
```

---
## \#1961 Posted by: mackann Posted at: 2019-07-06T05:20:59.110Z Reads: 147

```
Do you push apply updated config after changing? Its not reseting for me.
```

---
## \#1962 Posted by: ajplant96 Posted at: 2019-07-06T05:23:28.370Z Reads: 147

```
Yes, applied every time on about 5 attempts so far. Disconnected, closed the app, turned off the board, then it’s set to 9 cells when I check again or the last time back to standard 10 cells with 34v cutoff begin.
```

---
## \#1963 Posted by: mackann Posted at: 2019-07-06T05:24:38.719Z Reads: 145

```
Do you get the green config msg that it did write succefully? If not try with usb cable to do it. Bluetooth can be a little bad sometimes when writing config.

You could change another settings and se if it resets to, example motor A. If it dont its probebly a strange bug with custom voltage, if it does reset motor A to you probebly not succefully write the config.
```

---
## \#1964 Posted by: goldrabe Posted at: 2019-07-06T07:06:02.392Z Reads: 146

```
It did the same with me, lowering to 32V cutoff displays 9S even after hitting write. @mackann my VX1 also don´t connect with push to start.
```

---
## \#1965 Posted by: Balth81 Posted at: 2019-07-06T07:27:22.085Z Reads: 147

```
Have you tried doing it in the full vesc tool as opposed to the app?
```

---
## \#1966 Posted by: ajplant96 Posted at: 2019-07-06T10:22:20.415Z Reads: 147

```
Just did (perks of an IT roommate when you’re a mac user...) It still reverts to 9 cells rather than staying labelled as a custom voltage setting but seems to be finally accepting my desired settings of 32v cutoff start and 30v for cutoff end.
```

---
## \#1967 Posted by: ajplant96 Posted at: 2019-07-06T10:54:07.667Z Reads: 147

```
Ah okay, I guess that's normal then. As long as it allows me the extra juice allowance that shouldn't be a problem. I was on a group ride using the AT setup for the first time in ages last night expecting about 25km-28km range and had it power down just at 20km so that sucked.
```

---
## \#1968 Posted by: goldrabe Posted at: 2019-07-06T12:55:25.845Z Reads: 149

```
Be careful with those settings if you have a charge only BMS. The default cutoff values are the healthiest for total battery cycle life. Who knows how accurate the Unity reads the Voltage?
```

---
## \#1969 Posted by: ajplant96 Posted at: 2019-07-06T21:47:35.538Z Reads: 156

```
Well if 18650 cells are okay with 30v cutoff and it basically cuts off at the cutoff begin setting which used to be the complete cutoff setting it should be okay
```

---
## \#1970 Posted by: rey8801 Posted at: 2019-07-10T06:00:41.821Z Reads: 154

```
@Blasto @Deodand hello! I would need your help to address one problem. I have 2 unity got last March or April. One of the 2 has now problem. One side won't recognize sensor anymore, no matter which motor I use for detection. Also run them sensorless still has a problem and most of the time causes cloggs on the motor on that side. Do you know what can it be due? And how to fix? Do you have a repair center?
Thanks a lot! I need the Unity back in my life 😁

![IMG_20190710_000558|281x500](upload://fstlA8whiENwxiPAC7QItnFg5Z6.jpeg)
I removed the silicon cover and didn't see anything burnt
```

---
## \#1971 Posted by: Blasto Posted at: 2019-07-10T06:20:27.040Z Reads: 148

```
None of the halls show up?  Could indicate a connection issue with the 5V or gnd on the connector. Have a peek at the pins of the connector. Could probe it to make sure pwr and gnd are present

If 2 out of 3 halls show up (you would see an asymmetrical pattern in the hall diagram) that would take a closer inspection of the rc filter circuit and mcu legs.

Try to look for debris that shouldn't be there
```

---
## \#1972 Posted by: rey8801 Posted at: 2019-07-10T06:26:46.026Z Reads: 151

```
none of them. I get a dark yellow circle, like when it's sensorless. I am gonna check the 5v and gnd, just 5 sec
```

---
## \#1973 Posted by: rey8801 Posted at: 2019-07-10T06:38:33.514Z Reads: 154

```
Here we go
https://youtu.be/YYWabzg26GE
JST seems ok


And I do not see any debris. It looks new.
```

---
## \#1974 Posted by: Deodand Posted at: 2019-07-10T15:43:11.699Z Reads: 154

```
Does the motor move slow and smoothly when the detection runs?
```

---
## \#1975 Posted by: rey8801 Posted at: 2019-07-10T16:22:32.784Z Reads: 156

```
The side that now is broken does the detection but do not read the hall sensors. I think it moves as smooth as the other side. Slow and smooth. With pitch sounds at the beginning.
Other thing the faulty side now tends to go in the other direction after detection and also cloggs during ride. So can be that it's not just the sensor the problem.
```

---
## \#1976 Posted by: Deodand Posted at: 2019-07-10T16:42:16.972Z Reads: 161

```
Can you provide a screenshot of the detected parameters after you run your detection? A video of the detection process running would also be helpful just to confirm everything seems to be running normally.

It's possible to experience the cogging described on sensorless if the detection is a bit off, for now lets figure out what's up with the sensors not being detecting. Strange issue since everything looks ok voltage wise, and swapping motors maintains problem.
```

---
## \#1977 Posted by: rey8801 Posted at: 2019-07-10T18:06:42.402Z Reads: 154

```
ok I will make the video. I am saying that that side is broken because I used the unity before and was ok. SInce I connect the new motors then the problem started and now even with the old motors that side do not detect the sensor properly. I will make the video with different combination to show it. In case do you do repair on the Unity?
```

---
## \#1978 Posted by: Blasto Posted at: 2019-07-10T18:09:44.298Z Reads: 157

```
just a sanity check, also add to your list of actions, perform a motor detection with the sensors plugged in the opposite port. **do not run your motors in this fashion, it is just to see if the problem stays in the same place**

where are you located?
```

---
## \#1979 Posted by: rey8801 Posted at: 2019-07-10T18:10:45.160Z Reads: 155

```
ah right good idea I will try. Unfortunatelly EU, but I have parcels going out to US in case. No problem.
```

---
## \#1980 Posted by: Blasto Posted at: 2019-07-10T18:12:48.586Z Reads: 158

```
[quote="rey8801, post:1979, topic:77861"]
Unfortunatelly EU
[/quote]

:frowning:, shipping back and forth would be expensive... i'm pretty sure we can debug remotely, even though it would take a bit more effort
```

---
## \#1981 Posted by: rey8801 Posted at: 2019-07-10T18:37:12.775Z Reads: 153

```
Ok good. But if it is broken I can ask a friend to do tt but prefer people that actually made it. I can ship a Unity to you with 20 Euro not a big deal.
```

---
## \#1982 Posted by: ajplant96 Posted at: 2019-07-11T03:02:36.755Z Reads: 152

```
Anybody else have the settings on their unity change randomly? My brakes changed from -30 to -60/regen from -15 to -30 and motors changed to reverse
```

---
## \#1983 Posted by: Deodand Posted at: 2019-07-11T03:09:32.322Z Reads: 153

```
Are you using any other phone apps with your unity?
```

---
## \#1984 Posted by: FranciscoV Posted at: 2019-07-11T04:36:44.427Z Reads: 149

```
That has happened to me a few times with different unities.   I have had to re run motor detection and reconfigure everything including battery settings
```

---
## \#1985 Posted by: ajplant96 Posted at: 2019-07-11T04:40:00.250Z Reads: 148

```
Yes, Xmatic. Which doesn’t stay connected either.
```

---
## \#1986 Posted by: ajplant96 Posted at: 2019-07-11T04:41:05.171Z Reads: 153

```
Also with a 10s5p (Samsung 30q cells) how high would you recommend max settings for the braking anyway? Been told -30/-15 regen but that feels weak
```

---
## \#1987 Posted by: McErono Posted at: 2019-07-11T10:33:42.184Z Reads: 153

```
4amps regen per p cell is safe. Try -60 max brake (low speed braking) current and -20 regen (high speed braking). Should result in pretty strong brakes.
```

---
## \#1988 Posted by: ajplant96 Posted at: 2019-07-11T21:18:06.603Z Reads: 156

```
Excellent, thank you!
```

---
## \#1989 Posted by: ajplant96 Posted at: 2019-07-12T10:26:49.263Z Reads: 147

```
Anybody else had their unity cut out, lock the brakes and throw them off at 35km/hr before? No longer turns on after making a sparking/shorting sound. Emailed support so will see what they say but that kinda sucked, haha.
```

---
## \#1990 Posted by: drangboards Posted at: 2019-07-12T17:11:50.144Z Reads: 151

```
So I just got an android phone...  Paired up and watched to see any changes during the battery cut out I've been seeing under throttle conditions.  The battery gauge drops rapidly down past 10% and the cut out occurs just after that, and after the cut out happens, power returns and the battery meter goes right back up.  Charging also seems to be taking extra time.  Any ideas as to what is happening here, or what is wrong?
```

---
## \#1991 Posted by: deucesdown Posted at: 2019-07-12T19:01:57.764Z Reads: 151

```
Sounds like discharge bms cutting output?
```

---
## \#1992 Posted by: drangboards Posted at: 2019-07-12T19:11:30.299Z Reads: 155

```

Are you saying maybe the problem is the BMS, (because it is new) or that the problem could be in the motors, say it is getting too much heat, and cut out is occuring rapidly?  I forgot to be looking at my motor temps during this test, but I noticed, at ambient, one of the motors reads a higher temp by about 10 Celsius.
```

---
## \#1994 Posted by: rey8801 Posted at: 2019-07-13T12:57:19.187Z Reads: 158

```
Hi! Here the test you asked me :grin:

https://www.youtube.com/watch?v=5frfTe_SRf4

Let me know what do you think about it. Thx a lot!
```

---
## \#1995 Posted by: deucesdown Posted at: 2019-07-13T15:23:39.647Z Reads: 157

```
I said BMS because, when watching ackmaniac app, when I pull the loop key I see the voltage go down over a 1-2 second span until the vesc can't power itself. This sounds like what you're experiencing.

I don't think it's any temperature cutoff, as that would not drop the indicated pack voltage.

Based on your description so far, it sounds like under load, your pack is dropping in voltage enough for the BMS to invoke Low Voltage Cutoff, and shut down the output. This could happen because of bad cells, bad p-group, or bad connections.

This is just a possibility to consider though. There are lots of variables when troubleshooting.
```

---
## \#1996 Posted by: egzplicit Posted at: 2019-07-13T16:15:43.270Z Reads: 153

```
[quote="deucesdown, post:1995, topic:77861"]
I said BMS because, when watching ackmaniac app, when I pull the loop key I see the voltage go down over a 1-2 second span until the vesc can’t power itself.
[/quote]

Thats the capacitors discharging, all vescs do that when powered down.
```

---
## \#1997 Posted by: drangboards Posted at: 2019-07-13T21:14:26.085Z Reads: 155

```
[quote="deucesdown, post:1995, topic:77861"]
This is just a possibility to consider though. There are lots of variables when troubleshooting.
[/quote]

Do you have any suggestions for further testing to figure this out?  My local friend said let's tear into the battery and check for breaks in the welds somewhere.  Also I'll be pulling off the internals and checking all those connections maybe a lose connection somewhere.  Remembering that this also happens when I run over some bumps, but maybe that's just the timing...
```

---
## \#1998 Posted by: Meeep Posted at: 2019-07-14T19:48:31.087Z Reads: 152

```
I know this has been asked and brought up before but I am slightly concerned. I just finished my 10s4p samsung 30q pack and set the Battery Max to 30 amps and the Motor max to 35 amps. 

I maxed the throttle and saw the battery amps spike to ~55 amps. Why is this happening? I thought the Battery Max was a hard limit with a little leeway for small spikes. This seems large to me. Is it because of my motor settings? I am not that concerned considering the safe limit for my pack is 60 amps and the absolute limit is 80 amps. 

I would appreciate any input because I am trying to keep my pack happy and healthy! Thank you! :slight_smile:
```

---
## \#1999 Posted by: deucesdown Posted at: 2019-07-14T20:30:33.890Z Reads: 164

```
[quote="drangboards, post:1997, topic:77861"]
Do you have any suggestions for further testing to figure this out?
[/quote]

Hey I think you should start a thread, this is a bit too off topic now :slight_smile:

[quote="Meeep, post:1998, topic:77861"]
I maxed the throttle and saw the battery amps spike to ~55 amps. Why is this happening?
[/quote]

Hehe do you think the esc didn't respect amp limits, or do you think it's giving false readings? Or both.
```

---
## \#2000 Posted by: Meeep Posted at: 2019-07-14T22:57:55.547Z Reads: 164

```
I'm not sure. I know Enertion has said that the battery amp is not an absolute limit and it can spike higher for a few seconds (which is what happened in my case, albeit much higher than I would imagine) and that the Battery Limit is for both sides of the vesc so 30 amps would be like setting two VESC's to 15 amps but it *appears* that the 30 amp limit is per side but again as Enertion states, the Unity battery amp limit is *supposed* to be a total limit.
```

---
## \#2001 Posted by: KOMODO Posted at: 2019-07-14T23:35:25.011Z Reads: 168

```
Hey all! I'm trying to update my Raptor 2.1 Firmware but after a short time the Android app on my Samsung Note 4 loses connection!... "BLE error: ConnectionError" Any ideas?? :sob:
```

---
## \#2002 Posted by: goldrabe Posted at: 2019-07-15T00:17:35.803Z Reads: 167

```
The best and most reliable way is to open the enclosure and do the firmware update via USB cable with a Windows machine.\
In the latest firmware the bluetooth connection is stabilized and should give you less headache than now.
```

---
## \#2003 Posted by: Meeep Posted at: 2019-07-15T02:45:47.025Z Reads: 163

```
Alright, went out for another ride. Changed the amp limit from 30 -> 20 and the max amps I saw was 40. SO I guess the Unity setting is "per VESC." Because that's pretty damning to me.

Unrelated, I was unable to write or read any settings on the app for a bit and the only fix was to restart my phone.
```

---
## \#2004 Posted by: deucesdown Posted at: 2019-07-15T03:02:09.546Z Reads: 163

```
Wow that's interesting, definitely contrary to what was repeatedly stated, that battery amps is total for both sides.
```

---
## \#2005 Posted by: McErono Posted at: 2019-07-15T09:44:57.253Z Reads: 165

```
Motor amps set at 70a and battery max at 60a.

Thats what I got:
https://metr.at/r/lhc9k

70.9A battery, 134.2A motor
```

---
## \#2006 Posted by: SteveS33 Posted at: 2019-07-20T18:10:46.097Z Reads: 160

```
Sorry if I'm not posting my question in the right spot. Need a little help setting up my Unity from the app. I'm trying to put in custom voltage cutoffs for my diye 10s5p (31V and 41.8V). It doesn't seem to keep when I try writing it to the board. Every time I reconnect it has reset itself to the default 12s voltages. Am I doing something wrong?
```

---
## \#2007 Posted by: Deodand Posted at: 2019-07-20T19:36:45.563Z Reads: 161

```
It is just a bug that causes it to display that way sorry, it rounds to the nearest cutoff in the display but in reality it is maintaining the settings unless you write a config over it. I'll have a fix for this in the next release.
```

---
## \#2008 Posted by: KOMODO Posted at: 2019-07-20T23:59:49.864Z Reads: 163

```
Hey goldrabe, Thanks for the speedy reply! :grinning:

For anybody else searching for similar info here is the link I used to download the UnityFOCBOX UI onto my Windows 10 PC... (v1.3 which I assume is the latest Version??)

https://enertionboards.zendesk.com/hc/en-us/articles/360000660795-Windows-Tool-for-Unity

Initially I was trying to use the BLDC Tool which gave me an error when trying to connect to the board but the UnityFOCBOX UI connected to the board via USB C with no issues & now the Bluetooth connection between the Raptor 2.1 & Unity UI App on my phone is perfect...
```

---
## \#2009 Posted by: KOMODO Posted at: 2019-07-21T22:47:35.490Z Reads: 159

```
Quick Update: So AFTER screwing the enclosure back onto the board I realised the power was cutting out at full throttle when in R-Spec mode. :unamused: I had calibrated the remote incorrectly; i.e whilst in beginner mode & not R-Spec mode.

There is also still bluetooth connection issues on the Unity UI with my phone (Samsung Note 4) but luckily (after a few attempts) I could just about manage to calibrate the remote again before loosing Bluetooth connection. :sweat_smile:

My Samsung tablet seems to hold Bluetooth connection OK but it would be great if somebody can solve the connection issue with the Samsung Note 4...?

Hopefully this will help someone expirencing similar issues in the future. :nerd_face::+1:
```

---
## \#2010 Posted by: ChristianT Posted at: 2019-07-22T06:57:36.160Z Reads: 152

```
Does the Unity run also with Vesc tool and ackmaniac?
```

---
## \#2011 Posted by: L3chef Posted at: 2019-07-22T07:00:58.026Z Reads: 151

```
Ackmaniacs firmware doesn't support dual motors on one mcu. You need Unitys firmware.
```

---
## \#2012 Posted by: ChristianT Posted at: 2019-07-22T07:10:49.394Z Reads: 153

```
°crying° °sad° :frowning:
```

---
## \#2013 Posted by: Richcan Posted at: 2019-07-22T15:08:20.976Z Reads: 151

```
There should be motor temp sensors but I think on first batch they did not work properly, but second batch supposed to work?
```

---
## \#2014 Posted by: venom121212 Posted at: 2019-07-22T15:09:44.153Z Reads: 147

```
Motor temp sensors work fine on my first batch unity
```

---
## \#2015 Posted by: SteveS33 Posted at: 2019-07-22T15:14:37.939Z Reads: 149

```
Thanks for the reply! I'll keep an eye out for the next update
```

---
## \#2016 Posted by: McErono Posted at: 2019-07-22T19:08:01.169Z Reads: 146

```
yes thats how it is.
```

---
## \#2017 Posted by: LEE Posted at: 2019-07-22T22:42:07.241Z Reads: 142

```
Unity has no problem.The problem is the first batch TBDD.
```

---
## \#2018 Posted by: Richcan Posted at: 2019-07-23T00:14:23.777Z Reads: 143

```
Cool! I ordered TB DD’s second batch. I ordered the 90KV they sent me the 75KV so I’m in the process of sending back. And on the waiting list for Focbox on back order also!
```

---
## \#2019 Posted by: drone001 Posted at: 2019-07-23T19:42:31.248Z Reads: 146

```
i have an issue with my Unity now I think. While I’m breaking towards the tail end of the break for about .5 seconds it seems the breaks release and then reapply themselves…since it’s the tail end of the break it does not throw me off or anything just feel weird AF. also i get the same thing when accelerating about a .5 second period it feels the like it skips, or like the breaks were grazed. any ideas. I did notice my steering trim was off on my remote. 23.44 FW, 190Kv 6374 maytech, 12s6p
```

---
## \#2020 Posted by: sleekjazz Posted at: 2019-07-24T03:04:49.403Z Reads: 150

```
[quote="Blasto, post:682, topic:77861"]
Jst zh 6 pins
[/quote]

Will this work with the sensor plug on Alien Power system motors?
```

---
## \#2021 Posted by: legend27 Posted at: 2019-07-24T12:16:04.903Z Reads: 152

```
Hey everyone!

I'm having a small issue with my unity. Motor side 2 doesn't want to detect my motors hall sensors.

I've tried swapping motor & sensor cables (not swapping which port they go into on the unity) to the other side and it's always side 2 that doesn't detect the hall sensors.

I've also tried putting the sensor cable (phase wires included) that goes in side 1 over to side 2 (swapping the port that the connector goes into) and then the unity detects the hall sensor for side 1. Still not side 2 though. That's why i'm pretty comfortable to say the the motors are not the issue. They are also brand new.

The result of this is that motor side 2 runs sensorless. The board is ride-able and has okay startup but it's pretty annoying to know that one side is sensorless... I've enabled traction control which compensates the issue on startup a bit even though it's still noticeable.

**Does anyone know what can be causing this?**

I'm sure I forgot to post some important information to figure this out, so feel free to ask :) 

I'm also using some adapters from my motor to the unity and I have confirmed both works by swapping connectors around like mentioned above.

**TL;DR: One side of my unity doesn't detect the hall sensors.**

Any help is much appreciated and may you have a wonderful day :slight_smile:

edit:

Im using firmware 23.44 on version 1.3 Focbox UI on windows.

I've also tried the unity android app and metr app and none of them detects the hall sensor.
```

---
## \#2022 Posted by: venom121212 Posted at: 2019-07-24T14:15:13.048Z Reads: 151

```
If you're feeling mildly brave/curious, peel back the orange silicone on the unity and take a look at the solder job on the motor 2 sensor connector. Does it feel loose to you at all? 

My original unity had an issue with mismatched flux linkage measurements that ended up just being a badly soldered resistor.
```

---
## \#2023 Posted by: legend27 Posted at: 2019-07-24T16:19:29.276Z Reads: 152

```
Looks absolutely fine. Not loose or anything.

![image|666x500](upload://aWTn8JiNXcRaRQkHVZcSbvnHGt7.jpeg) 

It’s probably also worth saying I already voided my warranty. I soldered new bullet connectors :open_mouth:
```

---
## \#2024 Posted by: murloc992 Posted at: 2019-07-24T16:20:21.034Z Reads: 146

```
Last time I asked bullets were fine. Even XT90 was fine. Only if you have the platinum warranty that is.
```

---
## \#2025 Posted by: legend27 Posted at: 2019-07-24T16:27:25.263Z Reads: 146

```
I have platinum and I was told bullet connectors were NOT okay. Idk tbh. Let’s just say warranty is not voided then :joy:
```

---
## \#2026 Posted by: drone001 Posted at: 2019-07-24T16:39:29.589Z Reads: 146

```
what causes cogging......
```

---
## \#2027 Posted by: legend27 Posted at: 2019-07-24T16:41:31.354Z Reads: 145

```
Are you running sensored or unsensored?
```

---
## \#2028 Posted by: drone001 Posted at: 2019-07-24T16:42:40.114Z Reads: 143

```
sensored.....
```

---
## \#2029 Posted by: legend27 Posted at: 2019-07-24T17:35:09.521Z Reads: 142

```
Are your sensors detected correctly?

Maybe you can make a video of the coughing?
```

---
## \#2030 Posted by: drone001 Posted at: 2019-07-24T17:39:37.791Z Reads: 147

```
yes they are always detected without a problem.....it's barley noticeable..more of a feeling than something you can see. feels like someone grazed the breaks...not enough to throw me but enough for me to feel it. it only happens at low speeds and while long breaking.
```

---
## \#2031 Posted by: drone001 Posted at: 2019-07-24T20:14:44.564Z Reads: 151

```
I swapped the batteries in my remote and went out to do the video and it's gone again....i didn't get the cogging thing not one time. My clamp slipped on me  again so i had to end that ride. Good thing my press-ons from SeanHacker were delivered today. could a low remote battery cause that?
```

---
## \#2032 Posted by: goldrabe Posted at: 2019-07-24T21:02:01.025Z Reads: 145

```
Did you swapped batteries, or is your remotes battery low?\
Low battery on the remote can cause misbehavior.\
You say it's most prominent when braking?
```

---
## \#2033 Posted by: rideTastic Posted at: 2019-07-24T21:04:11.966Z Reads: 143

```
How accurate is the consumption indicator of the unity app?

I have a 12S4P 30Q pack and fully charged it shows 92% (49.3V). After 15km i have 52% left (unity app indicator) and a consumption of 11.7Wh/km. 

I dont think i could made 44km (518Wh/11.7Wh/km).
```

---
## \#2034 Posted by: drone001 Posted at: 2019-07-24T21:13:51.119Z Reads: 141

```
more so while accelerating at slow speeds. I have the torque boards 2.4 MHz remote so i was using some off name batteries i swapped those out for new ones.
```

---
## \#2035 Posted by: goldrabe Posted at: 2019-07-24T21:26:28.679Z Reads: 142

```
With the new batteries cogging is gone now?\
```

---
## \#2036 Posted by: drone001 Posted at: 2019-07-24T21:29:07.382Z Reads: 143

```
yes i think so. I only made it about 7 blocks before my motor mount clamp slipped ...AGAIN and had to end the ride. I don't even know if the batteries were low or not. i did notice the light blinked a couple of times this morning after arriving at the  job. It happened on my way to work a couple of times.
```

---
## \#2037 Posted by: goldrabe Posted at: 2019-07-24T21:34:28.310Z Reads: 142

```
Bad reciever placement can also cause misbehavior. Is the blinking light you saw indicating the remotes signal or battery state?
```

---
## \#2038 Posted by: drone001 Posted at: 2019-07-24T21:38:32.364Z Reads: 147

```
I'm not sure i fired off a message to torque boards asking ...the light blinks when pairing so i would guess the one light is for the signal. where's a good spot for the receiver. right now it's next to the Unity in the area where it plugs in.
```

---
## \#2039 Posted by: goldrabe Posted at: 2019-07-24T21:47:49.618Z Reads: 149

```
I guess you mean where the main discharge leads from your battery plugs into the Unity?\
Try to place the reciever as far as possible from any wires carrying high currents as your phase wires from the motors and main discharge leads, also try to get some distance between the Unity and reciever. Some people make long extension wires and are placing the reciever in the front of the enclosure.
```

---
## \#2040 Posted by: drone001 Posted at: 2019-07-24T21:53:47.612Z Reads: 149

```
ok cool..you are correct it's right next to the main battery cable. back into the enclosure I go. Thx bruh I will try that.
```

---
## \#2041 Posted by: drone001 Posted at: 2019-07-24T22:53:25.120Z Reads: 151

```
ok on my way home i noticed something, it only happens during the first 10 mins of the ride then it's fine. it's still happening but it's really smoothed out now if that makes sense. i also floored it up 2 steep hills without it happening. it's more so at low speeds when i feel it.
```

---
## \#2042 Posted by: goldrabe Posted at: 2019-07-24T23:24:27.428Z Reads: 150

```
I have the same issue, but sadly no one could point me in the right direction. I moved my reciever all the way to the front of my enclosure, but it still persists. In my case it seems like the same. I get cogging either when fully charged or when I am short before the battery cutoff starts, e.g. at 36 to 35V with 10S battery. @Blasto do you have any further suggestions?
```

---
## \#2043 Posted by: drone001 Posted at: 2019-07-25T01:25:30.730Z Reads: 152

```
All i did was remove my enclosure and now my Unity is not powering on anymore. lol...WTF i didnt even touch anything....I had a feeling it was something up with this Unity.
```

---
## \#2044 Posted by: goldrabe Posted at: 2019-07-25T05:28:48.172Z Reads: 152

```
Your switch is still properly connected?
```

---
## \#2045 Posted by: atlasdev Posted at: 2019-07-25T06:32:33.962Z Reads: 156

```
Hi, I'm having an issue where one of my motor is making a bit of noise. Does anyone know how you can fix that? It's not an issue with the PPM configuration, as it's using UART. A friend of mine (not in the esk8 world, just general motors) says this happens when motors are running sensorless. Could this have anything to do with that? The sensor wires are connected. 

My current motor configuration:

![498-1024|243x500](upload://x8Q7N4ngPuS8BQFsqPHJPcFIvJY.jpeg) 

https://www.youtube.com/watch?v=4G7u5KMo12M
```

---
## \#2046 Posted by: ricardo Posted at: 2019-07-25T07:30:51.608Z Reads: 149

```
is there a lag response on your Photon?
```

---
## \#2047 Posted by: atlasdev Posted at: 2019-07-25T07:53:27.152Z Reads: 150

```
I don't think so? I'm not sure what you mean.
```

---
## \#2048 Posted by: drone001 Posted at: 2019-07-25T14:10:05.649Z Reads: 151

```
yes it is...I jumped the switch and the Unity powered on so something is up with that switch. in addition to that i also have this weird cogging effect going on. I'm scared to ride this thing.
```

---
## \#2049 Posted by: drone001 Posted at: 2019-07-25T14:13:48.533Z Reads: 150

```
I had something like that and i found my sensor wires were swapped. Something is up with motor 2 shouldn't the black dot be there as well.
```

---
## \#2050 Posted by: venom121212 Posted at: 2019-07-25T15:04:21.727Z Reads: 153

```
Black dot just signifies that you manually told it to switch direction of that motor (in case one is spinning the wrong way)

I got confused and thought it was not picking up the sensor the other day. If the sensor isn't detected, the 2 pictures next to "HALL" will be blank.
```

---
## \#2051 Posted by: drone001 Posted at: 2019-07-25T15:45:07.723Z Reads: 153

```
thx...cool, got it. I have to remember that one.
```

---
## \#2052 Posted by: drone001 Posted at: 2019-07-25T20:19:52.802Z Reads: 156

```
I wondered the same thing.....if you find out could you post here.
```

---
## \#2053 Posted by: drone001 Posted at: 2019-07-25T20:20:36.283Z Reads: 150

```
anyone know the voltage rating for the momentary switch for the unity. looking for a replacement.
```

---
## \#2054 Posted by: TommyCnc Posted at: 2019-07-26T09:02:55.707Z Reads: 151

```
I've got an issue and pretty sure it's motor related rather thank unity, could someone suggest what may be the issue. I've only put two hours riding on these motors from new. Motors both spin freely by hand. Unity motor  Detection spins right motor correctly but left hardly moves. ! Also when I'm walking the board back to the car. Left motor has a negative amps value and right has positive. Thanks in advance  for any advice [ui|241x500](upload://mqMQJ0u2q1O6RyykANJDzfIOzUd.jpeg)![ui|241x500](upload://mqMQJ0u2q1O6RyykANJDzfIOzUd.jpeg)
```

---
## \#2055 Posted by: venom121212 Posted at: 2019-07-26T12:55:36.829Z Reads: 153

```
Your resistance on that side compared to the other is insane. I've never seen a result that bad.

24 mOhm vs 1042.

Also, motor 2 isn't detecting the sensor wire. That's reflected by the weird yellow symbol next to HALL

Normal values look more like this:

![Screenshot_20190716-144936|236x500](upload://lH3LvQvdAUVSn98rN3KV8TfcSw3.jpeg)

Also your Flux measurement (measured in Webers) is pretty mismatched.

Make sure your motor 2 is wired up correctly and try again. If you get similar results, swap motors left to right and see if the issue follows the motor or the unity ports.
```

---
## \#2056 Posted by: Jagden Posted at: 2019-07-26T15:49:34.921Z Reads: 164

```
Can't connect from Android to Focbox Unity.
Android app tried from Google Play and APK from GITHUB (1.2.1) and also from Enertion site.
Unity firmware: 23.44
Focbox Tool on Windows works.
Any idea ?
I heard that 1.3 fixes this issue, but can't find the APK, any link ?

![Capture%20(1)|689x389](upload://7jAAyzM16K21wKEfleVEKLBT5y9.png) ![Screenshot_20190726-184102|243x500](upload://jRJsp79KVKZGOSlAowQbNa5Namg.jpeg)
```

---
## \#2057 Posted by: niuva Posted at: 2019-07-26T21:31:08.599Z Reads: 168

```
My fried Unity Bluetooth module [spoiler]v1.1[/spoiler] kindly got replaced by Enertion. Now it manages to connect to the Unity via RX/TX again. Thank you!

The connection dropout was not fixed though by a new BLE module, which apparently is rumoured to be caused by the high polling rate of the Unity. Dropouts happen even with the official Unity Nexus app beta. So in other words, the bluetooth is still completely unusable on my end. :frowning:

So I guess the only option left for me is to compile my own Unity firmware with lower Uart baud rate and flash the NRF52 module with [Vedders NRF firmware](https://github.com/vedderb/nrf52_vesc) and see what happens. 🤔
```

---
## \#2058 Posted by: Deodand Posted at: 2019-07-26T23:13:08.902Z Reads: 168

```
There is a patch coming for this in like a week if you just want to wait.
```

---
## \#2059 Posted by: niuva Posted at: 2019-07-26T23:15:59.626Z Reads: 171

```
Woop! 
This bluetooth issue has been bugging me ever since I got my hands on my 1st batch Unity.

I'll wait for the patch and report back. :slight_smile:
```

---
## \#2061 Posted by: FredXanadu Posted at: 2019-07-27T02:26:03.645Z Reads: 173

```
@EnertionSupport i send you an email 8 days ago, could you please answer me #21171 ?
```

---
## \#2062 Posted by: atlasdev Posted at: 2019-07-27T11:11:12.940Z Reads: 174

```
Do you might know what's going on here @EnertionSupport @CarlCollins @adrianenertion @barajabali or @Deodand ?
```

---
## \#2063 Posted by: marcmt88 Posted at: 2019-07-28T22:26:56.471Z Reads: 168

```
Any help would be greatly appreciated.  3 issues:

1- Going thru the guided conf. After clicking on the "Apply Updated Config", can not continue to remote setup because "Ok" tap is gray out.  Only hitting ESC key allows me to move on with remote setup

2-  Remote calibration does not response to either throttle forward or backward.  Nano remote was confirmed to be connected with solid red light on Rx.

3-  "Hud Config" in setting:  "Test ERPM -> RPM" did not return any values other than "0" after manually turning one of the wheel 10x as instructed.
```

---
## \#2064 Posted by: Jagden Posted at: 2019-07-29T06:03:55.477Z Reads: 174

```
Since I have another Unity, I’ve tested it.
Regardless the firmware, I am able to connect via Bluetooth perfectly fine, no issues.
Appears to be that the Bluetooth module of the first Unity is fucked :frowning: Anyone had not so good experience with the BT module on Unity as well ? What can be done ? Is the first Unity completely useless now without BT ? connecting via cable seems to be working ok.
```

---
## \#2065 Posted by: NineLives Posted at: 2019-07-31T18:52:02.883Z Reads: 168

```
I currently have a support ticket waiting for advice on error:could not read firmware version make sure selected port belongs to focbox when connecting via android app. It originally worked fine and then just started getting this message. I too can connect fine by USB.
```

---
## \#2066 Posted by: Jagden Posted at: 2019-07-31T19:55:31.581Z Reads: 166

```
I think the BT module on the board is dead. It was dead from the start and never worked before. Enertion are ignoring completely on support tickets (no single response) in days/weeks. Don't wanna slander, but sadly this is the case.
```

---
## \#2067 Posted by: GeraldSwerdfegger Posted at: 2019-07-31T21:59:39.789Z Reads: 167

```
I am also having trouble writing updated configs as per your first issue.
```

---
## \#2068 Posted by: marcmt88 Posted at: 2019-07-31T22:26:03.836Z Reads: 167

```
Issues resolved:  when updating configs, Unity does not like it with the metr pro board on its comm platform.  Switch back to their original comm board before updating configs.  Re-install metr pro only after all configs are performed.
```

---
## \#2069 Posted by: GeraldSwerdfegger Posted at: 2019-07-31T23:03:49.505Z Reads: 165

```
yeah I was using the Metr Pro bluetooth module too.
```

---
## \#2070 Posted by: marcmt88 Posted at: 2019-08-05T18:28:58.117Z Reads: 156

```
My Unity switch also stop working, could no longer turn off no matter how long I press in.  Did you get it resolved or found a replacement?
```

---
## \#2071 Posted by: atlasdev Posted at: 2019-08-06T12:58:35.809Z Reads: 156

```
Hi, my unity keeps disconnecting and stops responding to commands. I'm trying to flash the firmware again in an attempt to resolve it, but this keeps timing out. When I start it up the error led flashes once. What could cause this?
```

---
## \#2072 Posted by: TommyCnc Posted at: 2019-08-07T11:24:21.596Z Reads: 157

```
My unity resets itself back to factory settings now and again. Batteries left plugged in. Is this common fault? Means I have to re run motor Detection and set battery type up.
```

---
## \#2073 Posted by: venom121212 Posted at: 2019-08-07T12:15:23.624Z Reads: 156

```
Happened once to me randomly, hasn't happened since. Updated your firmware?
```

---
## \#2074 Posted by: TommyCnc Posted at: 2019-08-07T12:20:10.832Z Reads: 160

```
There may be a new update but was current about a month ago. Will have to check. Weird that it holds settings when I disconnect batteries and charge them but a few hours between rides and it resets sometimes. Unless there's something I've missed about holding power button for too long resets it ? That's all I can think of
```

---
## \#2075 Posted by: Ixf Posted at: 2019-08-07T12:30:07.950Z Reads: 158

```
Thanks for posting this finding.  
Thats good to know
```

---
## \#2076 Posted by: drone001 Posted at: 2019-08-07T13:19:27.730Z Reads: 158

```
My switch died on me as well. I replaced it with
Ulincos Momentary Pushbutton Switch U16B1 1NO Silver Stainless Steel Shell with Blue LED Ring Suitable for 16mm 5/8" Mounting Hole (Blue) https://www.amazon.com/dp/B01G00GHQY/ref=cm_sw_r_cp_apa_i_x9SsDb46X0FHW
```

---
## \#2077 Posted by: venom121212 Posted at: 2019-08-07T16:50:14.184Z Reads: 159

```
That's an interesting thought. @Deodand anything like that programmed in to the switch?
```

---
## \#2078 Posted by: s5300 Posted at: 2019-08-08T17:54:18.538Z Reads: 162

```
@CarlCollins
@adrianenertion

FOCBOX Unity app on Android stopped working out of the blue. Just instantly crashes whenever I press connect. Any ideas? Already re-installed completely.
```

---
## \#2079 Posted by: esk8.austria Posted at: 2019-08-09T04:53:37.116Z Reads: 161

```
does anyone else have the problem that they can't connect to the android app?

I get a BLE Error: ConnectionError
```

---
## \#2080 Posted by: Marsl187 Posted at: 2019-08-09T18:23:56.152Z Reads: 158

```
Hey @Deodand

I have some problems with new motors on the Unity and just want to be sure that the noise is not an electrical noise which is produced by the Unity trough the motor.

See/Listen here:

https://youtu.be/7X8T8Dx00Lk

It is definitely not in the drivetrain itself. I get this when the motors and the Unity is warm (50 degrees or more) and after a few seconds (like in the video) on full throttle. I changed the motors (have 4 of them) but all doing this. I also think (not sure) it might be always just the right side of the Unity. 

Is this possibly some noise due to cut down (current or temperature)? Or can the definitely say this can not be caused by the Unity?

Did anyone else experience some noise?
```

---
## \#2081 Posted by: niuva Posted at: 2019-08-12T19:26:13.244Z Reads: 149

```
[quote="Deodand, post:2058, topic:77861, full:true"]
There is a patch coming for this in like a week if you just want to wait.
[/quote]

Any update on this?
```

---
## \#2082 Posted by: Shanian79 Posted at: 2019-08-14T03:06:34.587Z Reads: 147

```
So I’m having issues. Running a Unity with the DIY Raptor motor kit and nano remote. I got all in January. All has been fine up until the last two times I rode. Suddenly it’s very glitchy. Runs fine for about a minute, then starts to surge/cut out in short 1/2 second pulses, then sometimes cuts out all together when braking. Happens with throttle and brake. It’s not a battery issue as I’ve tried three other packs with the same result. Twice it’s started doing it then a full forward power surge hits and threw me off. I’ve installed the latest updates, but issue still exists. Has anyone else had this? Any help is greatly appreciated.
```

---
## \#2083 Posted by: rsalmon Posted at: 2019-08-14T18:34:58.041Z Reads: 143

```
Are you calibrating your remote every time you turn it on? 

Did you run PPM calibration in fast mode?
```

---
## \#2084 Posted by: Shanian79 Posted at: 2019-08-14T21:15:47.275Z Reads: 143

```
Yes. Initial calibration was done in R-spec mode, and calibrate Nano every time.
```

---
## \#2085 Posted by: fnfoged Posted at: 2019-08-14T23:59:42.912Z Reads: 141

```
Can you please explain  what you mean by keeping track of the amp-hours that go back in when charging. How can I use that to determine how far I can set my cutoff? I'm trying to dial in my 12s 10,000 mah lipo that I got with my trampa.
```

---
## \#2086 Posted by: fnfoged Posted at: 2019-08-15T01:07:46.978Z Reads: 141

```
I'm getting 1.99A at 45.31 volts. I had my cutoff at 44.4 volts and my range was subpar. ![20190814_210202|281x500](upload://3rKV9DjgNO8ia5AK84WSBbt0q9t.jpeg)
```

---
## \#2087 Posted by: deucesdown Posted at: 2019-08-15T17:28:22.714Z Reads: 136

```
[quote="fnfoged, post:2085, topic:77861"]
explain what you mean by keeping track of the amp-hours that go back in when charging
[/quote]

Say you have a 10Ah pack. Let's say conservatively you're hoping to get 70% of your pack. That's 7Ah. Conservative because packs have less punch at lower states of charge, and you really don't want to hit or get close to 0% on any of the lipo cells.

Charge your pack to 100%, and ride until you hit cutoff. At this point you expect to have discharged most of the energy from your pack. Charge to 100% again, and note how many amp hours go back in. If you put 7Ah back in, you hit your goal of 70%. If you only put 2Ah back in, something is very wrong. Either your cutoff settings are way too conservative, or the pack is not behaving well under load (bad connections, weak cells, old pack, etc).

Hope that helps.
```

---
## \#2088 Posted by: birds Posted at: 2019-08-15T21:18:11.874Z Reads: 136

```
[Video](https://drive.google.com/file/d/17jTpoN2cUlrKEx9W6aAqFwboq6qG0WAw/view?usp=sharing)
I just got my focbox connected, using mostly the default config. What could be causing my motors to behave like this? it won't spin a full rotation and constantly goes backwards/forwards in the jerky motion, making a weird noise.
```

---
## \#2089 Posted by: SanderG Posted at: 2019-08-16T11:46:30.197Z Reads: 136

```
So im trying to connect some sensors to my motor, im connecting it to GND and TEMP, it shows up in the app but only when i heat it up, if it cools down again there is no value. How can i make this work? Or do i need a different kind of sensor?

![image|281x500](upload://mDvvRyKmEVZ1xd1ObiouhS66IQI.jpeg)
```

---
## \#2090 Posted by: NineLives Posted at: 2019-08-16T23:31:10.673Z Reads: 137

```
Did support ever get back to you? They asked me for a picture of the unity with the orange cover pulled back which I sent them nearly a month ago now and not heard a thing.
```

---
## \#2091 Posted by: Jagden Posted at: 2019-08-17T13:22:40.603Z Reads: 137

```
Answer in private.
```

---
## \#2092 Posted by: PixelatedPolyeurthan Posted at: 2019-08-18T11:37:23.303Z Reads: 138

```
@Deodand my unity's power switch has a little problem. I can't fit it back in the JST connector, it just will not stay there. ![20190818_133059-01|666x500](upload://A0Am01h0l0I9AhKnN0mSNUmRzmj.jpeg)
```

---
## \#2093 Posted by: venom121212 Posted at: 2019-08-18T13:10:36.790Z Reads: 135

```
You can try bending the pin on the other side out a bit if you have a small tool. Then it will catch in the plastic square on the terminal.
```

---
## \#2094 Posted by: PixelatedPolyeurthan Posted at: 2019-08-18T13:15:33.639Z Reads: 137

```
@venom121212 normally the metal connector has a tiny flap that catches the plastic square. the little flap broke i think.. not me though it was like this out of the box.
```

---
## \#2095 Posted by: deucesdown Posted at: 2019-08-18T15:30:27.682Z Reads: 133

```
Seems enertion isn't doing support at the moment :( your best bet is to scavenge a jst ph terminal (with wire) from somëhing else and splice it on. That is if you don't have a crimper and terminals.
```

---
## \#2096 Posted by: PixelatedPolyeurthan Posted at: 2019-08-18T16:25:16.698Z Reads: 138

```
[quote="deucesdown, post:2095, topic:77861"]
Seems enertion isn’t doing support at the moment :frowning:
[/quote]

from what i read when they do it all is good... and then there are times where you get no answers for months lol

well funnily i have ordered some already because i f**ked my sensor cable from my evolve but banggood takes some time haha. i think i will put in in the connector and then tape all the wires so it does not pop out. once connected to the unity it should be unlikly to pop out
```

---
## \#2097 Posted by: Sn4pz Posted at: 2019-08-18T17:17:07.472Z Reads: 140

```
Bust out the hot glue, should be enough to hold it till the new ones come in... 

I feel like tape would allow for some wiggle room, who knows what would happen if it pops out under full throttle.
```

---
## \#2098 Posted by: Marsl187 Posted at: 2019-08-19T14:33:30.176Z Reads: 150

```
Hello again,

I can now definitely say that the error/sound is caused by the Unity!

[quote="Marsl187, post:2080, topic:77861"]
See/Listen here:

[Turnigy Sk8 6374 149kv Noise](https://www.youtube.com/watch?v=7X8T8Dx00Lk)

[/quote]

It seems like the Unity can't calculate the values anymore or so and cuts out therefore. See the screen recording from the life data:


https://youtu.be/UlBy4jZMMfY


The moment motor 2 is getting negative current is when the noise starts to occur. I'm still holding trottle at this moment, no braking or so. Also the noise just comes from motor 2, no matter which motor I use. So there is definitely a problem with the right side of my Unity!

Please address this issue and help me to solve it. @Deodand @CarlCollins @EnertionSupport

Some details which might help you:

Motors: Turnigy SK8 6374 149kV
Battery: 12s discharge current 70A

Configuration here:

![unity%20error|334x500](upload://tRqZXs2JcrT91x0kUDRnbp3qCUY.png)
```

---
## \#2099 Posted by: TommyCnc Posted at: 2019-08-20T16:10:36.968Z Reads: 143

```
I had this exact same noise on hard throttle when I was testing the board on the ground. The sound is coming from unity. Not sure why. It stops the motor pulling when that sound is happening too right? No  definitive solution tho other than mines  settled down after a lot of re setups and wire checking.
```

---
## \#2100 Posted by: ducktaperules Posted at: 2019-08-23T08:16:50.921Z Reads: 142

```
@Deodand I had my batch 1 unity clear all its settings again today. It’s happened a few times now and it’s fucking annoying.

Been riding for days without making any settings changes. Ride home from work fine. Board shuts its self down due to inactivity after a while when i get home. half hour later i Give board to gf to practice on, she powers it up and gets on but it don’t go no where, motors just twitching. open up unity app and unity forgot all it’s motor calibration and battery safety cutouts. But some how remote is still calibrated and it looks like app settings are still set but all battery and motor values have been reset including hall tables and motor flux measurements.

Then cause app is not always reliable it connect. I did a read and did a motor calibration. But then it wouldn't let me do a write to save that data, button was just grayed out. was still getting real time data for wheel speeds and could do a read but it wouldn't let me write. did multiple power cycles of the board, and my phone. some times it wouldn't let me write, others wouldn't let me read or write. Spend half hour fucking about trying to get it working before it finally writes motor calibration. It’s been fine again since.

When this happened previously i wrote it off as firmware bugs due to early software but im running the latest and its been quite a while now so im beginning to think it might be a hardware problem.

Have you heard of this before? i know of a few on the other forum that are having similar issues. 

Is this being caused by a software or hardware issue? could it be a bad eeprom on my unity?

Im keen to get it sorted out cause i dont want to get stranded miles away from home.
```

---
## \#2101 Posted by: venom121212 Posted at: 2019-08-23T12:46:30.462Z Reads: 131

```
Interesting point if information... I have only let the unity auto shut down once and I think it was the one time it reset the settings as well. 

Is there a way to store a good config file on my phone and load the entire profile at once if this happens again?
```

---
## \#2102 Posted by: ducktaperules Posted at: 2019-08-23T13:17:11.530Z Reads: 135

```
i believe you can do a full config save in metr. i have never tried it but thats actually a good idea. i would be interested to see if it also saves all the hall tables and other motor settings. maybe @rpasichnyk would know?
```

---
## \#2103 Posted by: rpasichnyk Posted at: 2019-08-23T13:37:09.890Z Reads: 143

```
Yes, Metr -> Expert -> Read -> ... menu -> Save.

![33|317x474](upload://AnDza59wAwSbwtVqxFvWRZujku5.png) 

Saves motor configuration (with hall tables and everything) and app configuration (with PPM pulsewidth and everything) :slight_smile:
```

---
## \#2104 Posted by: PixelatedPolyeurthan Posted at: 2019-08-25T05:56:16.435Z Reads: 136

```
Hi again.
I have two issues 

My Unity/motors are playing up.
When i throttle, 3/5 times one motor won’t spin. They both have the same tension. it happens with both motors, just as much the left as the right. The motor jitters a bit… goes back and forth 1cm at a time quite fast then if i let go of the throttle again it ‘‘frees’’ up and works normally.

I have a maytech eskate remote on it and it only has one speed mode… fucking supersonic. as soon as i start pushing the throttle it goes straight to 50km/h. i have calibrated the remote and meddled with the settings a bit but nothings makes a big difference.

Btw these are bench-tests. I have not tried riding it yet.
And also i have not plugged in motor sensors because these are stock evolve motors and the connectors are different.
Any help is appreciated as always!!:kissing_heart:
```

---
## \#2105 Posted by: PixelatedPolyeurthan Posted at: 2019-08-25T10:00:30.983Z Reads: 136

```
https://forum./t/noob-question-thread-ask-your-questions-here/126/2893?u=pixelatedpolyeurthan
```

---
## \#2106 Posted by: atlasdev Posted at: 2019-08-25T11:01:32.383Z Reads: 141

```
What's up with Enertion support? I'm waiting for a reply to a support ticket for over two weeks (again).
```

---
## \#2107 Posted by: accrobrandon Posted at: 2019-08-27T00:51:52.725Z Reads: 144

```
I think this was asked before but now I'm curious from real world testing...so I currently had a motor die...so I'm running single till I figure it out...

So if max battery amps are set is it split or does unity know when your running single? Or do I need to double the max battery value? On dual this is easy... Lets say 30q 4p you set your max between 60-80 ..so 30-40 per motor. But since I'm running single I left it at 70amp... Now based on meter I havent even gotten close to 40amps at best.... Granted I'm running 20/60 on AT, and single is lame as shit at that rate... But if there were 70 available amps for a single.motor shouldnt I feel more pop? It starts to roll like I'm in some sort of beginner mode.
Thoughts?

https://metr.at/r/ogrWK
```

---
## \#2108 Posted by: PixelatedPolyeurthan Posted at: 2019-08-30T09:12:11.633Z Reads: 130

```
@accrobrandon If you still don't know you can ask in the noob question thread here. This thread's activity is on and off.
https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559
```

---
## \#2109 Posted by: atlasdev Posted at: 2019-08-30T13:29:50.667Z Reads: 139

```
Does anyone know how to connect an stlink to the Unity? For flashing the bootloader again. My gut says it's the black female header package where the Bluetooth module sits in, but I don't know the exact pins.
```

---
## \#2110 Posted by: atlasdev Posted at: 2019-08-31T09:02:24.544Z Reads: 141

```
I found the pinout, and it's connecting just fine now.

Now my issue becomes to find the hex of the bootloader, does anyone have it? @Deodand I was told you should have it. I tried [this one](https://github.com/EnertionBoards/FOCBOX_UI/blob/FOCBOX_UI/res/bootloaders/UNITY.bin), but now the board does not turn on (blue light turns on, but turns off about 5 seconds later)
```

---
## \#2111 Posted by: Meeep Posted at: 2019-09-01T02:13:14.500Z Reads: 142

```
I've read that the Unity battery max is total but looking at the app with dual drive set to 25amps I consistently see 45-50amps on acceleration so.... idk to be honest.
```

---
## \#2112 Posted by: Shaun Posted at: 2019-09-01T20:08:15.947Z Reads: 143

```
So I went to use my skateboard today but the Unity wouldn’t power on. I have been using it regularly for the past few months without issue. Power supply is good (10S), momentary switch is good (continuity on all cores and the switch makes/breaks when operated). I used it three days ago for about 15 minutes with no issue. Powered it down and put it away (at 37.5V) and didn't put it on charge. Just gone to use it and it’s got no life whatsoever. Battery supply is still at 37.5V.

Any help/ideas would be appreciated.
```

---
## \#2113 Posted by: Valantis Posted at: 2019-09-01T20:32:37.700Z Reads: 144

```
Hi I have the Nord H2c
I know it's not the most advanced board but I'm having issues with my skateboard and would like some advice. 

My board is able to go backwards but for some reason it won't accelerate. I'm not sure if it's the remote or something more serious. Does anyone have any ideas what I should or can do? Thank you

https://youtu.be/a4HKnbXwN6M
```

---
## \#2114 Posted by: venom121212 Posted at: 2019-09-02T13:44:21.336Z Reads: 138

```
Try swapping any 2 of the motor's 3 phase wires. This reverses direction. Is your board meant to have forward and reverse?
```

---
## \#2115 Posted by: FredXanadu Posted at: 2019-09-02T19:17:11.555Z Reads: 133

```
Same problem, Jeff kindly try to help me on the forum and i had a ticket from Enertion since months, no answer from them...
```

---
## \#2116 Posted by: Shaun Posted at: 2019-09-02T19:27:52.186Z Reads: 139

```
I’ve had a response from Enertion. This is what it said ...

*Due to huge demand for our customer support resources, we currently cannot provide technical support for focbox unity configurations with 3rd party items.*

*Please check these forum posts about this subject: https://www.electric-skateboard.builders/search?q=focbox%20unity*

*If you don't find the answer you should post about it in the forum and see if someone else in the community can provide some assistance.*

*If you can take a quick picture of the circuit board and reply to this ticket, we might be able to give some advice to whether it has some blown components and what those components are etc.*

I can’t see any visible problem with mine. All components look OK (I have 16 years experience with electrical systems). 

I was quite shocked at their reply to be honest.

Cheers,
Shaun.
```

---
## \#2117 Posted by: Shaun Posted at: 2019-09-02T19:29:08.006Z Reads: 140

```
If anyone else would like to have a look at the photos and suggest anything? ... ![image|666x500](upload://qH4IAcdccr4UK3y814g0gEJ2L1L.jpeg) ![image|666x500](upload://eOMeuQgLFBm1c7JUR0UskTzfgm2.jpeg)
```

---
## \#2118 Posted by: atlasdev Posted at: 2019-09-02T21:15:14.390Z Reads: 138

```
Here you are. The only thing I can see is that yellowish something around the usb-c port. Do you know what that might be? Is that some custom mod?
```

---
## \#2119 Posted by: Shaun Posted at: 2019-09-02T21:19:38.895Z Reads: 141

```
No, it’s appears to be factory applied. Some type of resin, possibly.
```

---
## \#2120 Posted by: FredXanadu Posted at: 2019-09-02T21:57:15.599Z Reads: 137

```
same for my unity all the components looks look ok...
by the way, i paid for the 1 year instant-replace warranty :slight_smile:
@EnertionSupport could you help me  ?
```

---
## \#2121 Posted by: CarlCollins Posted at: 2019-09-02T22:31:20.843Z Reads: 137

```
Initiate a ticket and if you have platinum warranty on it, you will get a unit replaced without any questions (1st time)
```

---
## \#2122 Posted by: FredXanadu Posted at: 2019-09-02T22:58:34.880Z Reads: 141

```
Thanks @CarlCollins for your fast answer.
I already have a ticket #81797 and filled the form...
```

---
## \#2123 Posted by: CarlCollins Posted at: 2019-09-03T00:07:18.345Z Reads: 141

```
[quote="FredXanadu, post:2122, topic:77861"]
81797
[/quote]

Can you initiate a new one as all of the old are closed as we are on the new system now
```

---
## \#2124 Posted by: Valantis Posted at: 2019-09-03T00:11:53.442Z Reads: 142

```
first thank you for your interest and for the help you have given me !!

 More specifically the problem that I have suddenly encountered while using the skateboard,
 I bought this skateboard and didn't make it myself.

I have tried to change directions with the reverse (you asked me if i have) and again i had not front movement and just my brakes were operating normally in both directions. 

I would like your opinion again.
Thanks![15674694512184857643110735980962|281x500](upload://6FFqkAeFQ5xs8yL2gB5XOqSmZ3s.jpeg)
```

---
## \#2125 Posted by: venom121212 Posted at: 2019-09-03T00:21:51.522Z Reads: 136

```
Try holding down the reverse button for a few seconds instead of tapping it.

If that doesn't work, try holding the reverse button while you power on the remote.
```

---
## \#2127 Posted by: Chase Posted at: 2019-09-03T01:13:35.384Z Reads: 138

```
My bad didn’t see the third party thing. Ignore last post
```

---
## \#2128 Posted by: Grabacr Posted at: 2019-09-05T00:58:32.018Z Reads: 141

```
Hey, I've been having the same issue you had. Did you ever find a solution? I've been looking for three weeks and still haven't figured it out.
```

---
## \#2129 Posted by: Valantis Posted at: 2019-09-05T04:07:20.564Z Reads: 141

```
Thanks I fixed!!😁😁
```

---
## \#2130 Posted by: Kerrymann Posted at: 2019-09-12T03:07:37.892Z Reads: 136

```
I have been doing a lot of testing with the focbox Unity and it's been very impressive.  But for my next step I need to display and record some key data streams from the unity.  Specifically: (Battery voltage, Motor voltage, Motor Amperage, RPM, Throttle, FET temperature, Motor temperature).  I am currently reading and recording this data with an arduino but would really like to get a bluetooth option.  I have tried the enertion Andoid app via bluetooth but the UI HUD gives very little data and doesn't record.   I have done a fair bit of searching and there are options but they appear to only work with aftermarket Bluetooth modules and I would really like and option that works with the Unity bluetooth module.  And finally I would like to record and display the information from 6 different Unities at the same time (yes, I am running 12 motors!).  Suggestions?

Thanks in advance,
Kerry
```

---
## \#2131 Posted by: Richcan Posted at: 2019-09-12T04:05:29.567Z Reads: 133

```
What’s the best way to mount this Unity? In the Case? So it not sliding all over the place?
```

---
## \#2132 Posted by: brently Posted at: 2019-09-12T14:28:05.373Z Reads: 138

```
Is this chip fried? I dunno how it could have happened, my settings are super low on a 10s2p vtc6 battery. 

Question open to anyone obviously, the Unity went completely unresponsive then wouldn't turn on after I was spinning up the motors after fixing some belt tension issues. 

 ![image|375x500](upload://lfbsRRWtn2N0WOxW5CG8L525CSc.jpeg) ![image|375x500](upload://zdt8QUQyFmURGqsDuaPANFZYdUk.jpeg)
```

---
## \#2133 Posted by: PixelatedPolyeurthan Posted at: 2019-09-12T17:05:17.334Z Reads: 133

```
The [Metr Pro](https://www.electric-skateboard.builders/t/metr-pro-unity-bluetooth-module/95494) is what you need. It is fully compatible with the Unity and records everything you possible need to know

https://metr.at/shop
@rpasichnyk

@brently you should ask this in the [Noob Question Thread](https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/1) because this thread is rarely active.
```

---
## \#2134 Posted by: Kerrymann Posted at: 2019-09-12T17:36:32.969Z Reads: 133

```
Thanks.  I had seen that but it requires the aftermarket Bluetooth module (I would need 6 of them) and I don't know if the program will work with more than one at the same time. I would really like and option that works with the Unity bluetooth module.
```

---
## \#2135 Posted by: PixelatedPolyeurthan Posted at: 2019-09-12T17:40:26.016Z Reads: 134

```
Ah yes, i missed that last bit. Better ask also on the Noob Question Thread. I am not aware of anything that could attach to 12 boards and interact and share info on the same device.
```

---
## \#2136 Posted by: brently Posted at: 2019-09-12T18:22:09.991Z Reads: 134

```
thanks was hoping to get the attention of some enterion reps which I know isn't always the easiest
```

---
## \#2137 Posted by: Kerrymann Posted at: 2019-09-12T18:55:41.773Z Reads: 134

```
Thanks, I will try there.
```

---
## \#2138 Posted by: bigH Posted at: 2019-09-14T17:26:01.814Z Reads: 129

```
Please Help. My board is mostly working. Motors calibrated successfully. Upgraded firmware.

One motor spins smoothly and makes that sweet sweet sound, the other one does not. It makes this ugly rattling noise.

https://youtu.be/dzvp31ZA8_I

[direct link](https://youtu.be/dzvp31ZA8_I)
```

---
## \#2139 Posted by: Steven1 Posted at: 2019-09-14T18:06:14.357Z Reads: 124

```
Try unplugging the sensor cables. That did it for me.
```

---
## \#2140 Posted by: bigH Posted at: 2019-09-14T18:31:27.890Z Reads: 123

```
Unplugging the sensor cable makes the motor itself stutter and not move properly. I'm going to try switching the motors on the foc to see if that changes the situation.
```

---
## \#2141 Posted by: bigH Posted at: 2019-09-14T18:39:51.136Z Reads: 121

```
Tried swapping the motors and the issue occured with the other motor this time. Maybe it's an issue with the unity. Going to try redoing the setup and maybe re-doing the setup.
```

---
## \#2142 Posted by: bigH Posted at: 2019-09-14T18:52:21.374Z Reads: 125

```
I put everything back together (sensors included) and it now works, _but_ I have this issue:
![image|680x500](upload://vtQccouUUAtlXNWWeJJ43X1zK0K.png) 

1. what does it mean to have a yellow ring?
2. why are both the boxes below red?
```

---
## \#2143 Posted by: PixelatedPolyeurthan Posted at: 2019-09-14T18:54:27.823Z Reads: 124

```
I am not sure about the red boxes but motor 2 does not receive any signal from the sensor.
```

---
## \#2144 Posted by: ElectricCoast Posted at: 2019-09-14T19:07:33.038Z Reads: 124

```
Life got in the way on me with using the unity until today but I can tell you that the STMicroeltronics virtual com port is not visible on device manager.
```

---
## \#2145 Posted by: bigH Posted at: 2019-09-14T19:32:28.155Z Reads: 128

```
I got it fully working, sensors and all. The issue was a vesc connector had come loose, the pin wasn't sticking all the way thru, so pushing it in helped.

Thanks everyone for the help!

H
```

---
## \#2146 Posted by: ElectricCoast Posted at: 2019-09-14T19:50:56.832Z Reads: 133

```
This is so dang frustrating.  I posted back in December that I couldn't get my either of my unities to connect via usb.  Deodand had me check to see if I had virtual com port from STMicroelectronics in my device manger in my ports tab.  I have been sitting here with 2 brand new never used before unities and I can't get them to communicate via usb.  I don't and I can seem to figure out how to fix this problem.  I'm stuck and can't ride.  Can someone give me hand on this.  I'd appreciate it.!  Com port 8 is the USB cable but it doesn't create a virtual com port.  I have tried to figure out how to remove and reinstall the STM driver but I am not having any luck.
 [Unity%20USB%20issue|690x388](upload://mpsRerMnnEVFvNkWkCe5g0FHeAl.png)
```

---
## \#2147 Posted by: deucesdown Posted at: 2019-09-15T16:34:09.102Z Reads: 130

```
Easy things to try... try another computer, or a few other computers. Try the bluetooth module with the android app.

Fixing driver issues can be very frustrating. Sometimes another box will *just work*, then you can work on the drivers with less pressure.

Oh, is the unity plugged into a battery pack and turned on?

Edit: also try a bunch of usb cables
```

---
## \#2148 Posted by: Hiifi Posted at: 2019-09-21T21:10:58.894Z Reads: 127

```
Hey All, if anyone can help me with setup I would greatly appreciate it, I’ve been reading this thread the past 2 days and now I’m even more confused. 

I want substantially less harsh power delivery and braking. Turning the max batt current and motor current down doesn’t help. I brought down from the stock 60 setting all the way to 10.

My setup : Dual 270KV sensorless with 10s2p

I have both the Max and mins set to 10 and -10
I turned my throttle ramping all the way up (1s positive and .5s negative)

The board is NOT a smooth ride, my $50 eBay ESC works better. 

Also just to note one wheel definitely gets more power than the other.![image|374x500](upload://2BKSLvPIq1VuXnnh67U6hPaUMea.jpeg)
```

---
## \#2149 Posted by: Hiifi Posted at: 2019-09-21T21:15:17.777Z Reads: 123

```
Also, this is the HUD Reading at full throttle.. is this correct for these settings ?![image|374x500](upload://px37Ivxe80rnoatZkis2ZikGi8G.jpeg)
```

---
## \#2150 Posted by: Blasto Posted at: 2019-09-21T21:52:58.567Z Reads: 123

```
Increase your motor amps to 50 and -50A
```

---
## \#2151 Posted by: mackann Posted at: 2019-09-21T21:54:40.855Z Reads: 122

```
Change your motor A to 40 and motor regen - 40, also increase your battery A to 25.
Also you run sensor less so expect a little "un smooth" start
```

---
## \#2152 Posted by: Hiifi Posted at: 2019-09-21T22:16:26.082Z Reads: 124

```
Ok changing the amps does not help. I tried it at 50 and -50 and also 40 and -40... 
It seems that the motors are getting all the way to full speed when the throttle only shows 30ish percent and the rest is not even being used
```

---
## \#2153 Posted by: mackann Posted at: 2019-09-21T22:21:36.986Z Reads: 125

```
On bench or on street?
```

---
## \#2154 Posted by: Hiifi Posted at: 2019-09-21T22:30:45.901Z Reads: 127

```
Both, it seems like it wants to just take off around 1/3 to 1/2 throttle. 

Am I understanding the settings wrong or are you not able to limit the overall power? Turning the max values down should limit the power shouldn’t it? Mine does not seem to change it
```

---
## \#2155 Posted by: mackann Posted at: 2019-09-21T23:11:13.873Z Reads: 125

```
On the bench you will reatch top speed in 2 sek with 20% throttle, on the street with you on you will not.

Also on 25% throttle you will soner or later reatch topspeed if its not uphill, if you want to limit topspeed you need to set erpm limit with the full Windows tool for Focbox Unity. 

Battery current max A= high speed acceleration 

Motor current max A = low speed acceleration 

Motor current regen = low speed braking power 

Battery current max regen = high speed braking
```

---
## \#2156 Posted by: Hiifi Posted at: 2019-09-21T23:14:47.925Z Reads: 123

```
Thank you! I will try the ERPM limit

Is there a way to make the throttle not increase over time ? Where holding it in position will keep that speed?
```

---
## \#2157 Posted by: mackann Posted at: 2019-09-21T23:15:38.278Z Reads: 123

```
No its not
```

---
## \#2158 Posted by: Hiifi Posted at: 2019-09-22T01:57:09.808Z Reads: 124

```
I have battery and motors both set to -40 and 40 and it now stutters when I try to take off.. any idea why?
```

---
## \#2159 Posted by: Deodand Posted at: 2019-09-22T03:17:24.505Z Reads: 125

```
Did you run motor calibration at these current settings?
```

---
## \#2160 Posted by: deucesdown Posted at: 2019-09-22T06:50:44.705Z Reads: 128

```
I just want to say, it's good to see you guys. :slight_smile:

@Blasto @Deodand
```

---
## \#2161 Posted by: PixelatedPolyeurthan Posted at: 2019-09-22T09:04:15.729Z Reads: 132

```
[quote="Hiifi, post:2158, topic:77861"]
and it now stutters when I try to take off… any idea why?
[/quote]

Normal. That is because you are running sensorless. If you run sensorless the motors will always ''jitter'' from a stand still. you need to push start with out sensors. if you don't want to push to start then get motors with sensors. :wink:
```

---
## \#2162 Posted by: venom121212 Posted at: 2019-09-22T15:24:47.626Z Reads: 132

```
@Deodand,

How soon do you think profiles option will be implemented on the unity?

I have 2 unity powered boards and my wife just started riding. It'd be nice to not have to change motor settings and throttle curves back and forth every time.
```

---
## \#2163 Posted by: PixelatedPolyeurthan Posted at: 2019-09-22T17:04:22.757Z Reads: 132

```
[quote="venom121212, post:2162, topic:77861"]
I have 2 unity powered boards and my wife just started riding
[/quote]

@Deodand a wife is one thing, your 60+ y/o father is another. I think such a feature is a must.
It would make the whole experience much better, *and safer* given how ''dangerous'' eskating already is.
```

---
## \#2164 Posted by: Deodand Posted at: 2019-09-22T17:27:24.604Z Reads: 137

```
I'm working on a big update, profiles is definitely top of the list.
```

---
## \#2165 Posted by: PixelatedPolyeurthan Posted at: 2019-09-22T17:42:33.578Z Reads: 134

```
Thank you @Deodand :v:
```

---
## \#2166 Posted by: venom121212 Posted at: 2019-09-22T22:23:45.156Z Reads: 133

```
Excellent. I'm still loving both of my unitys and have had no issues with either :+1:
```

---
## \#2167 Posted by: venom121212 Posted at: 2019-09-23T15:13:47.654Z Reads: 139

```
Actually for accuracy's sake, I've had one small issue with one unity. It completely forgot motor detection settings after powering board on. This had only happened once, but last night it happened again. Very annoying but again, pre configured profiles would hopefully fix that quickly. Unless it's a motor detection issue and those values can't be force written without redoing detection.
```

---
## \#2168 Posted by: Svenny Posted at: 2019-09-23T19:51:39.522Z Reads: 137

```
has anyone tried hooking the unity up to a flipsky vx1??? i tried over the weekend no luck with it, i got through a majority of the setup but after everything was said and done the remote did nothing, am i missing something, i gave up sorta quick to be honest lol
```

---
## \#2169 Posted by: Deodand Posted at: 2019-09-23T22:45:20.172Z Reads: 136

```
using uart or ppm?
```

---
## \#2170 Posted by: Svenny Posted at: 2019-09-23T23:17:59.908Z Reads: 136

```
Uart is the connector I have
```

---
## \#2171 Posted by: Deodand Posted at: 2019-09-24T00:43:04.168Z Reads: 139

```
![Screenshot_20190923-173952|230x500](upload://rIiZItVfg0uZNbYQy3W9T4Oua77.jpeg) 

Make sure you set your uart correctly here. Not sure what baud flipsky is running. I'd guess 115200.
```

---
## \#2172 Posted by: Crashmaster Posted at: 2019-09-24T03:51:29.440Z Reads: 133

```
The Non Vesc version of the VX1 will work in ppm.
```

---
## \#2173 Posted by: Hiifi Posted at: 2019-09-24T19:06:51.185Z Reads: 136

```
Hey, just wanted to note that re calibrating the motors fixed the stuttering and although I have sensorless motors, I have never experienced the stutter minus when the motors were not calibrated. Always take off from a dead stop even up hills.
```

---
## \#2174 Posted by: PixelatedPolyeurthan Posted at: 2019-09-24T19:27:38.453Z Reads: 135

```
That is truely odd. I will ask my friends if they know. Glad to know you back up and running :smiley:
```

---
## \#2175 Posted by: Svenny Posted at: 2019-09-26T14:11:12.915Z Reads: 131

```
i went ppm and it works perfect now, thanks guys
```

---
## \#2176 Posted by: auveele Posted at: 2019-09-27T17:31:49.499Z Reads: 135

```
Hi!
 I had the focbox unity since before summer. I works perfect and this week I wanna change my remote.
When I connect the focbox to my computer to calibrate the remote with FOCBOX TOOLBOX, I changed some values, and I reset the config to default.

After that, I calibrate the remote, and works perfect, instead the motor dont get to much velocity. Then I reboot the focbox and it dont start again!
I'm scared with this. I dont know what is the problem, aparently everything is right
```

---
## \#2177 Posted by: Quiles Posted at: 2019-09-29T22:51:38.047Z Reads: 134

```
Hi guys - for the records, same here. I lost all my configs. Today was my first ride with Unity. Everything was fine, until i stopped in the park for maybe 30min (i think unity did the auto shutdown)....i turned on and motor was weird. Looked at the app and all configurations was gone...even my battery configs.

I am with metr for unity installed.
```

---
## \#2178 Posted by: venom121212 Posted at: 2019-09-30T13:44:18.281Z Reads: 136

```
This has happened to me twice now, super annoying. Just out of curiosity, did you have any issues with your power button while turning the board back on right before it lost the configs?

Both times I've had the issue, the power button was unresponsive a few times before turning the board on successfully.
```

---
## \#2179 Posted by: Quiles Posted at: 2019-09-30T14:00:51.463Z Reads: 133

```
Not that i noticed...will check next time. When you loose settings, did the board auto shutdown?
```

---
## \#2180 Posted by: venom121212 Posted at: 2019-09-30T14:44:57.157Z Reads: 132

```
No, but it has only happened when the board has been off and then turned back on.. never while riding. Very odd indeed.
```

---
## \#2181 Posted by: Quiles Posted at: 2019-09-30T14:56:28.845Z Reads: 131

```
Yeap...same here.
```

---
## \#2182 Posted by: Xenon Posted at: 2019-10-03T12:54:49.183Z Reads: 126

```
Same problem here any sulotion on that problem ?
the motor is ok testet it on a vesc with no problem.
```

---
## \#2183 Posted by: Quiles Posted at: 2019-10-03T23:33:15.722Z Reads: 128

```
New firmware just released. It seems this is resolved.
```

---
## \#2184 Posted by: Gerrycorrado Posted at: 2019-10-04T14:47:00.115Z Reads: 131

```
Did someone already had the opportunity to test the new fw? If so which setup.
Have an event on Sunday and not sure if i should update or not :slight_smile:
```

---
## \#2185 Posted by: ElectricCoast Posted at: 2019-10-04T22:19:46.210Z Reads: 132

```
It was the computer.  I used another one.
```

---
## \#2186 Posted by: Hiifi Posted at: 2019-10-09T03:47:47.560Z Reads: 128

```
Will we be able to configure / calibrate with Bluetooth and Iphone or Mac any time soon? Sucks to take the enclosure off every time
```

---
## \#2188 Posted by: Airwolf Posted at: 2019-10-10T08:07:35.031Z Reads: 123

```
Hello,
I was wondering if You ever found a solution to your issue which was described as: 
"BLE Error and connection drop shortly after connecting" ?

I am having the same issue. I think I need to re-position my Focbox Unity as it is currently pressed against the underside of my Battery Pack. I believe this is messing up the Bluetooth Signal Reception from the Focbox Program on my Cell Phone.

So again, did You ever find a solution to your "BLE Error and connection drop shortly after connecting"? 

Thanks in advance for any comments you may be able to provide about this.
```

---
## \#2189 Posted by: izzyjac Posted at: 2019-11-11T20:47:01.935Z Reads: 104

```
Hi, I my battery LCD doesn't seem to be working when it's connected to the FOCBOX unity.
I have it plugged into the 2-pin JST port and the LCD simply does not power on when I turn the Unity on. Do I need to configure something in the UI?

I am quite sure the LCD works because when connected directly to the battery it turns on.

This is the LCD I have: www.amazon (dot) com/gp/product/B07DMK9PKK/ref=ppx_yo_dt_b_asin_title_o05_s00?ie=UTF8&psc=1
```

---
## \#2190 Posted by: Airwolf Posted at: 2019-11-12T21:05:48.287Z Reads: 104

```
Hey buddy,
I think the 2 pin jst thing on the Focbox Unity only supplies 5 volts DC, while the LCD Battery monitor says it functions at 6-63 volts DC.

So it might be that you are 1 volt under the minimum voltage to make the LCD monitor function.

There's a number of ways to remedy this. One quick test would be to put a 1.5 volt AA battery in line with the LCD meter and connect that to the 2 pin jst in the orientation that results in about 6.5 volts. 

But you would probably be better off using a rechargeable 9 volt seperate from the skateboards battery pack and separate from the focbox. 

A rechargeable 9 volt will be light weight and compact and will theoretically function down to 6 volts. Also, by not connecting anything else to the jst 2 pin on the Focbox, it is likely you will improve the life of the Focbox simply because you are adding another system to it if you tap in to it for power.

Best of luck. 
In Summary, try a separate battery providing at least like 9 volts since the LCD is 6 to 63 volt device.

If needed for some signals to work properly in terms of communicating between the Focbox and the LCD's sensor, you can run a single wire from the negative terminal of the 2 pin jst connector on the Focbox or  the negative side of the skateboards battery pack, or any negative wire connected to the Focbox probably. 

Then connect that new wire from the negative to the negative terminal of your auxiliary battery pack for the LCD screen. As long as they have shared negative, they should be able to communicate. ( This last part might not be necessary, but if the LCD monitor doesn't seem to work right the first time you hook it up, you might want to try having a wire between the negative terminal of the Skateboards battery and the negative terminal of the LCD monitors separate, dedicated battery, a 9 volt for example.

And if you really want to have the LCD monitor come on and off with the Focbox, you could get a small 5 volt DC  relay from Amazon or eBay and use that to connect and disconnect the LCD monitor to the 9 volt battery.
```

---
## \#2191 Posted by: izzyjac Posted at: 2019-11-12T22:04:22.694Z Reads: 96

```
Thanks so much for the speedy reply!

My goal is to have the battery LCD display the battery voltage of the skateboard and turn on/off with the skateboard. What do you think would be the best way to do this?
```

---
## \#2192 Posted by: Airwolf Posted at: 2019-11-12T22:14:56.276Z Reads: 95

```
Bro,
I didn't look at the Amazon ad very closely until now.

What I said before is probably not exactly right.

If the LCD Monitor only has 2 wires, then they probably are supposed to be connected to the battery pack "+" and the Battery pack "-" directly
```

---
## \#2193 Posted by: Airwolf Posted at: 2019-11-12T22:16:20.013Z Reads: 94

```
See because the LCD Monitor goes from 6 to 63 volts, then it must be directly measuring the battery pack voltage. Similar to how you would connect a multi meter to measure the voltage of the battery pack.

You probably do not need to connect anything to the 2 jst pins unless
```

---
## \#2194 Posted by: Airwolf Posted at: 2019-11-12T22:19:00.648Z Reads: 96

```
If the LCD Monitor only has 2 wires, then you can just connect to the main 2 wires carrying power to and from the battery pack. These are usually big red and big black wire. Furthermore, the black is negative.

I assume that it is probably ok to just leave the LCD Monitor on all the time. But if you want to have it come on and off, the easiest way would be to put a very small toggle switch or any little  switch that has an on and am off position in line with the lcd Monitor.

Actually, I just remembered seeing somewhere that the jst 2 pin connector on the Foc box unity may be turned on and off witha button on the hand held remote control for the skateboard. You might want to check that out.

Otherways to get it to come on and off with the Focbox Unity would require a Transistor or a small relay, both that operate on 5 volrt or less and 15o ma or less.


If your still working on figuring this out, can you reply with the number of wires that come from the LCD monitor, and what they are called in the instructions.

That would make it more clear.

Also, you might want to look in the forums by searching for Focbox 2 pin or jst, the fewer words the better.

Someone should have figured out how that connection functions and mentioned it somethwherr in the forums.

In any case, if you can get the jst 2 pin to come on and off with the hand held  remote, or if you can verify that it comes on automatically when the Focbox Unity is powered on, then you can install a small relay or Transistor that the jst pin activatesn or deactivates, and then use the switching ability to connect or disconnect 1 of the LCD monitors wires to the plus or minus wire from your battery pack.
```

---
## \#2195 Posted by: Balth81 Posted at: 2019-11-12T22:30:02.091Z Reads: 91

```
When I ran an battery lcd display it was from the 2pin jst on the unity it’s not 5v or anything it’s same voltage as battery and is a great spot to run it from depending on what lcd you have its amp draw may be too much but shouldn’t be likely.. it might be a faulty lcd you can test by connecting directly to battery positive and negative also have you checked you wired it up correctly? I don’t use one anymore and use the jst on unity to give the board battery level to my remote
```

---
## \#2196 Posted by: Airwolf Posted at: 2019-11-12T22:39:38.364Z Reads: 90

```
Whoa, you learn something new every day. I figured the jst 2 pin was a small 5 volt supply. If it actually is the same voltage as the battery pack, maybe use a multimeter to see what the voltage on the 2 pin jst is to begin with! And also, does it turn on and or off when the unity is powered on or off. That would be a good place to start... Sorry for writing a novel there Buddy! There are some good conceprsi n there though  lol. Have a nice day
```

---
## \#2197 Posted by: Airwolf Posted at: 2019-11-12T22:49:51.756Z Reads: 93

```
Hey there is another post on here where a guy had it wires back wards because the black wire needed to be connected to + and the Red  wire to -. So it mightbe as simple as trying it with the 2ires connected the other way. Just try it connected the other way real quick, for like 1 second. If it turns on goodt,if not, disconnect it again right quick..
```

---
## \#2198 Posted by: izzyjac Posted at: 2019-11-12T22:52:09.377Z Reads: 95

```
I have connected it to the battery directly and it works perfectly fine there. 

The LCD only has two wires (black&red) so there are only really two ways to wire it to the jst. I've tried both and neither worked :/ 

You said you had the battery voltage/percent sent to your remote? How did you configure it? Perhaps it is similar to how I could configure it to go to the jst

I'll post a picture of it connected to the unity when I get home
```

---
## \#2199 Posted by: Balth81 Posted at: 2019-11-12T23:10:41.052Z Reads: 99

```
Yep it’s only 2 Wires but if polarity is wrong then it won’t work .. my remote a flipsky vx1 has the ability to display the battery voltage on it by connecting the transceiver to a positive power source.. I also found the lcd on the board quite in accurate I much prefer the remote and metr app / module.
```

---
## \#2200 Posted by: Crashmaster Posted at: 2019-11-13T21:32:57.399Z Reads: 96

```
As mentioned above. The 2 pin Jst is actual voltage. Max load is 150ma and it is fused at 300ma.
Mine is hooked up to the 2 pin Jst. I bought the connector with wires that fit the Unity, but these are the opposite on polarity when connected to the Unity. 
I had to depin it and switch them. 
The meter is accurate as I compared it to my fluke meter, and the voltage is the same on the Hud menu on the Unity app.![1113191311_Film1|666x500](upload://2znLqJSHEcrStOmTCV2W5616COf.jpeg) ![1113191312_Film1|666x500](upload://n2XjoRLrppeovlsXpPjGpUtf9hX.jpeg) 
This is my 3rd meter due to vibrations. that makes it go wonky.
Mounted it better and so far so good this one is lasting. 
Good thing these are cheap to buy.
```

---
## \#2201 Posted by: izzyjac Posted at: 2019-11-14T20:46:34.000Z Reads: 95

```
I also have been having an issue with remote calibration. When I go to calibrate it the ppm display is either still or stuttering up and down, regardless of how far I've pulled the throttle. 
I have a pretty generic remote. It's a copy of a remote that I had that worked well on another board.  https://www.amazon.com/gp/product/B07GDGDTFR/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&th=1

I not sure what the issue is. Based on the light on the receiver the remote and receiver are indeed paired. 

Have you been able to get your problem figured out?
```

---
## \#2202 Posted by: CarlCollins Posted at: 2019-11-14T20:52:54.692Z Reads: 96

```
Can you share a video of the fluctuation you are getting on PPM Pulse width bar?
```

---
## \#2203 Posted by: venom121212 Posted at: 2019-11-14T22:21:10.869Z Reads: 97

```
Whaaaat no lol. The 2 pin aux port is for a battery meter. Therefore it measures the same voltage of the battery.

To be entirely accurate, the 2 pin aux port reads 1 volt lower than battery.

![20191112_214319|281x500](upload://267nYpPDQM9y8sQ0pUmOUxPBI4g.jpeg)
![20191112_214242|281x500](upload://exc3vQwvHqtfs5wbOpbDVgk1ihm.jpeg)
![Screenshot_20191112-214400|236x500](upload://dPFPA87gzCNlMpEdd9lzXR9b57o.jpeg)
```

---
## \#2204 Posted by: izzyjac Posted at: 2019-11-14T23:43:12.289Z Reads: 97

```
I think we have the exact same battery LCD, except mine is not working no matter which way I put the wires.

Did you do anything else besides simply plug it in to the 2pin port?![image|666x500](upload://bYw6exsfcsPSSe8vJwOBng2z5Xc.jpeg) ![image|666x500](upload://yHnRv7PJr3czuwLmkcLiwgXgQ8k.jpeg)
```

---
## \#2205 Posted by: izzyjac Posted at: 2019-11-14T23:44:47.483Z Reads: 93

```
Here is the video
https://youtu.be/HvcXkUNlcT8
```

---
## \#2206 Posted by: barajabali Posted at: 2019-11-15T00:37:34.875Z Reads: 94

```
You have blown the LCD fuse. You can repair this yourself by replacing the fuse or just bridging the two pads where the blown fuse is.
```

---
## \#2207 Posted by: izzyjac Posted at: 2019-11-15T01:46:47.726Z Reads: 98

```
do you mean the fuse in the LCD or in the FOCBOX unity?
It works fine when connected directly with the battery ![image|666x500](upload://lrB8FbgfyjMsPZs34BhjGCzCHo6.jpeg)
```

---
## \#2208 Posted by: barajabali Posted at: 2019-11-15T01:56:27.104Z Reads: 96

```
The unity has a fuse for the lcd
```

---
## \#2209 Posted by: Mikenopolis Posted at: 2019-11-15T03:09:49.254Z Reads: 96

```
Look at you. Being an Enertion support even though Jason is being an a$$hat 👏👏👏 appreciate you being an esk8squad support member.
```

---
## \#2210 Posted by: barajabali Posted at: 2019-11-15T03:35:13.735Z Reads: 102

```
Haha thanks man. Yea you know it just kills me that all these nice people who supported Enertion by purchasing a board are being plainly ghosted. 

I have the knowledge, let me clean up this fuck up of a companies mess.
```

---
## \#2211 Posted by: MustardTiger Posted at: 2019-11-15T05:10:52.158Z Reads: 103

```
Do I need to use the switch that came with my unity? I have a torqueboards battery that has an on/off switch integrated into the battery?
```

---
## \#2212 Posted by: Mikenopolis Posted at: 2019-11-15T05:51:59.482Z Reads: 105

```
What do you mean use the unity switch. You mean the push button that plug into it?

You can semi permanently connect that jst connector with a wire so the unity is always on. And the battery button would be the on/off
```

---
## \#2213 Posted by: MustardTiger Posted at: 2019-11-16T02:24:32.696Z Reads: 106

```
Yeah I meant the push button switch that came in the box. Wasn’t sure if maybe the the battery needed to be turned on before the unity. So I just need to bridge the the 2 pins labeled MOM on the switch port?
```

---
## \#2214 Posted by: Mikenopolis Posted at: 2019-11-16T03:07:06.166Z Reads: 111

```
Yup. That’s how you do it if you want to use a loop key instead as well
```

---
## \#2215 Posted by: izzyjac Posted at: 2019-11-16T23:54:13.017Z Reads: 109

```
When I try to calibrate my remote with the Unity the ppm bar is stuttering and not at all responding to the throttle. Does anyone know why this is happening?

here is a video:
https://www.youtube.com/watch?v=HvcXkUNlcT8
You can see the blue light on the receiver is solid (not blinking) so that means it is paired with the remote. 

this is the remote: https://www.amazon.com/gp/product/B07GDGDTFR/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&th=1
```

---
## \#2216 Posted by: Blasto Posted at: 2019-11-17T00:26:56.917Z Reads: 108

```
Your remote is not binded to your receiver
```

---
## \#2218 Posted by: venom121212 Posted at: 2019-11-23T14:26:16.075Z Reads: 104

```
Your factory just offers flipsky parts... I didn't say anything about wanting or needing anything?
```

---
## \#2219 Posted by: cool_rollerblader Posted at: 2019-11-30T05:33:50.759Z Reads: 95

```
![ui|250x500](upload://rtd4cDCg0bzodPUBGyZ3mpWCxRm.jpeg) 

Looks like I have a sad motor. Does the Unity have the ability to definitively diagnose that or should I get a mate over with an oscilloscope?
Pretty impressed with the Unity interface and bluetooth reliability but it's a bit hard to appreciate it with a shagged motor and not way to get a replacement.
```

---
## \#2220 Posted by: drone001 Posted at: 2019-12-02T03:06:35.044Z Reads: 94

```
when i do a setup on the unity everything works except when i do a “apply updated config” app just hangs. I get the same thing both on the pc version as well as the android version. FW is up to date. Aiso i get the same thing with the Unity Metr pro as well as the original bluetooth module. any idea what it could be?
```

---
## \#2221 Posted by: Balth81 Posted at: 2019-12-02T03:19:11.950Z Reads: 93

```
I had similar issues with the metr make sure the metr app is disconnected when applying updates
```

---
## \#2222 Posted by: drone001 Posted at: 2019-12-02T03:33:51.257Z Reads: 105

```
had to my own metr pro firmware update and it works just fine now...thx for pointing me in the right direction.
```

---
## \#2223 Posted by: Freakboard Posted at: 2019-12-09T18:12:21.069Z Reads: 106

```
Hi dear @Deodand by ertion , 

I wait for two items unity ( preorder ) in the last Mail you say shipping  in November , but we have Dezember . And the last Mail what this ? ![image|231x500](upload://8l0Xv1m6UekldF64laLhpU9lwuG.jpeg) ![image|231x500](upload://ciWzqEF3dkq43CyaW7My8OpGTnu.jpeg) ![image|231x500](upload://yWPo5eFZxVxhU0UwTLZzhv8Gy9i.jpeg) jenson never gif my a answer to my question. 

Thanks for help my
```

---
## \#2224 Posted by: PixelatedPolyeurthan Posted at: 2019-12-09T18:37:02.214Z Reads: 104

```
@Freakboard 

@deodand does not work for enertion anymore, sorry to say.
Why did you buy from enertion when everyone knows the company is going down and nobody is being delivered what they ordered???
```

---
## \#2225 Posted by: Freakboard Posted at: 2019-12-09T19:23:14.003Z Reads: 102

```
Thanks dear 
I had no information,@jasonEnertion karma will fix it
```

---
## \#2226 Posted by: dildoritos Posted at: 2020-01-03T23:30:40.130Z Reads: 77

```
Someone please help!!

https://youtu.be/jWUc1GQUMg8

I just updated the firmware... how do I go back?? Or is this possibly some other problem?

Please, thank you,
Karl
```

---
## \#2227 Posted by: Pantata Posted at: 2020-01-04T00:47:04.398Z Reads: 78

```
Hey man, that is not a unity problem, that is either a faulty remote or you just need to do recalibrate your remote in the unity app. That thing with full throttle is a fail safe. DO NOT EVER use your board witth a remote where the fail switch is set to anything but neutral. Look up online how to set the fail safe to neutral position. Then open the remote calibration tab in your unity app and see If the ppm signal is jumping by itself. If it is then you need to change the remote or the receiver. ANyways try recalibratin the signal via the app.
```

---
## \#2228 Posted by: Pantata Posted at: 2020-01-04T00:48:50.376Z Reads: 79

```
You need to do motor detection and remote calibration after each fw update...
```

---
## \#2229 Posted by: Pantata Posted at: 2020-01-04T00:52:55.579Z Reads: 81

```
how to set failsafe on the mini remote:
"I’d like to add that there is a failsafe trigger position (the throttle value used if signal is lost briefly). To set this, you leave the receiver and transmitter on after releasing the bind button – at that moment you set all the controls to the “failsafe” position you want them in if signal is lost. The moment you remove the bind key, the failsafe position is recorded for both channels. Then turn everything off and back on. You should be rocking and rolling."
```

---
## \#2230 Posted by: Clay123 Posted at: 2020-01-07T22:54:46.477Z Reads: 77

```
Hey guys. Recently replaced a focbox in my r2. After replacing it everything worked. However, I was going to adjust some settings and was prompted to update the firmware on my vescs in the FOC tool and without thinking downloaded the unity firmware. The board no longer works and I am wondering if there is a way I can remove the firmware and replace it with the correct firmware?
```

---
## \#2231 Posted by: Pantata Posted at: 2020-01-14T20:59:28.538Z Reads: 67

```
Can't you upload a different fw via the windows tool? Either vesc tool or vesc tool for unity...?
```

---
## \#2232 Posted by: Airwolf Posted at: 2020-01-15T01:39:40.737Z Reads: 63

```
Yeah, I am not sure about this one because I have been out of the loop for a minute.

I do know that if your hardware is OK, but there is basically any problem with the firmware, you can order an STM 16 / STM 32 USB Degugging tool from Ebay or Amazon for about $15.

Then, with this little device that plugs in to your USB Port of your computer, Uou can basically "Reinitialize" the Focbox Unities entire program memory to the point write before you need to install the firmware.

There is an excellent tutorial on doing this on Esk8 News. It is called "Focbox Unity not booting, You are not alone". Search for that on Google and it will be the first thing to come up.

Yeah. So for $15 and a few days wait, you can get a brand new start with the Focbox Unity on the Softqare and Firmware side. 

It may take a while to figure out the program that comes with the stm link 16/32 module, but it does work on Foxbox Unity.

One last thing. If your Foxbox Unity is not working right and there does not appear to be anything wrong with any thing on the circuit board, disconnect it from power for like an hour or so. Tou could discharge the 4 big capacitors I'd you know how, but it isnt absolutely essential.

Then, spray the hell out of the Focbox Unity pcb with a product called "QD Electronics Cleaner" which is available in most auto parts stores. Try and shoot the fluid in between little the pins on little micro chips and IC's etc that you re mounted on the pcb.

Then, let the unity dry for like a full day, or as long as it takes until you are absolutely sure it is dry.

Then, connect a proper voltage to the Unity with nothing else attached and see if the correct LED's come on. 

If they do, go ahead and reprogram the Unity with the STM Link 32 module. 

After you have successfully reloaded the file using the STM 32, turn off the focbox. 

Reinstall the focbox in your skateboard.

Try to connect to your focbox using the bluetooth with the  "Focbox UI" app on your cell phone,. As soon as the bluetooth connection is made, you will be prompted to install new Firmware if needed. 

Be careful not to have your power to the Unity go off while the firmware is being loaded or you'll have to take a step back to the STM link and do that little process again.

Also, if you want to reduce the complication of the tasks your Unity will be responsible for the first time you go through the Guided Setup, you could choose to leave the Ribbon Cables that go to your Motor Wheels disconnected the first time through and then go for. Test ride and make sure everything seems ok. This leaves the hall sensors and the motor wheel temperature sensors out of the system initially which means there are fewer things to cause an issue.

Your board will still work without them, it will just be a bit less fine control below 3 miles per hour, but exactly the same after that.

Assuming your board works fine for a few rides, then you could reconnect the Ribbon cables and go through the Guided Setup on your Cell Phone with Focbox UI app again and it will reestablish the connection to those other sensors. 

If something goes wrong at this point, you will have a pretty good idea what the problem is. If everything is OK, go for a ride. 

P.S. Dont buy used tires for your electric skateboard. Even if they look OK. Recommend waiting for new ones to come in; )
```

---
## \#2233 Posted by: TheFlash Posted at: 2020-01-23T03:48:19.981Z Reads: 48

```
Hey guys, I'm having trouble using the Stlink v2 to reinstall the firmware and or bootloader on the focbox unity. thanks for any and all help.
```

---
## \#2234 Posted by: Jasonkimberson Posted at: 2020-01-29T19:24:24.242Z Reads: 37

```
Have the unity lock up issues been resolved?
```

---
## \#2235 Posted by: Gerrycorrado Posted at: 2020-02-02T09:25:41.675Z Reads: 29

```
Amp over current? Yes.
```

---
