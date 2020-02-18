# VESC tool on FOCBOX

### Replies: 24 Views: 3545

## \#1 Posted by: karma Posted at: 2017-09-17T19:03:03.617Z Reads: 374

```
In the middle of building my board and next up is to config my 2 FOCBOXES.
I have both the BLDC tool from Enertions website and the new VESC-tool. After having a look around in both programs I feel that the VESC-tool has a lot more info when it comes to setup and the different settings. Is there any pros/cons to using the VESC-tool instead of the BLDC tool? Has anyone tried programming FOCBOXES yet with the VESC-tool?
```

---
## \#2 Posted by: XIII Posted at: 2017-09-17T19:15:04.805Z Reads: 369

```
it's the same program with a different user interface, I believe
```

---
## \#3 Posted by: Rinzler Posted at: 2017-09-17T19:15:18.528Z Reads: 366

```
You should really read this thread, people are having problems with FOCBOX-es because of VESC Tool.
http://www.electric-skateboard.builders/t/vesc-project-com-is-online-public-vesc-tool-download/32268
```

---
## \#4 Posted by: Sebike Posted at: 2017-09-17T19:20:24.022Z Reads: 346

```
Why not just use the extended bldc tool by @Ackmaniac that has a lot of the features that vesc tool has?
```

---
## \#5 Posted by: Silverline Posted at: 2017-09-17T19:22:01.210Z Reads: 333

```
At the moment i run my focboxes with the new VESC-tool/firmware. I can`t get FOC mode to work , so i`m running in BLDC mode. Even though i`m looking forward to be able to run FOC, i think they run grate on BLDC as well.
```

---
## \#6 Posted by: BigBoyToys Posted at: 2017-09-17T19:28:21.523Z Reads: 322

```
Im running FOC with the VESC Tool, 12S and FOC with Torqueboard 130KV hubs. No issues
```

---
## \#7 Posted by: karma Posted at: 2017-09-17T20:13:17.526Z Reads: 312

```
THe extended BLDC tool doesn't come with all the nice information about all values, doesn't come with setup wizard. However I think going with the extended version later on when I have everything up and running is on my list. 
I want to start off east on the setting and mods on my first 2 FOCBOXES.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-09-17T20:36:22.668Z Reads: 292

```
[quote="karma, post:7, topic:33352"]
THe extended BLDC tool doesn't come with all the nice information about all values,
[/quote]

The extended BLDC tool does come with a load of explanation when you pass your mouse over.... It's more complete than the actual BLDC tool.
```

---
## \#9 Posted by: karma Posted at: 2017-09-17T20:37:28.035Z Reads: 280

```
Oh really? Didn't know that! I will head over to the post and start reading again.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-09-17T20:40:30.816Z Reads: 290

```
Not everything is detail, but enough to help... 

<img src="/uploads/db1493/original/3X/a/3/a3f05acd4dd6308b03b58ce44ce536eaed26881a.JPG" width="374" height="500">
```

---
## \#11 Posted by: Sebike Posted at: 2017-09-17T20:44:04.530Z Reads: 280

```
Don't know how complete the vesc tool is when it comes to explaining the settings, but extended has info for most settings I believe. 

Does have a guide/setup wiz for setting up FOC mode as well. I used this to setup my FOCBOX (single drive) and it runs smooth with no issues.
```

---
## \#12 Posted by: RiGo Posted at: 2017-10-17T03:28:50.194Z Reads: 255

```
I'm out of the loop a bit with this. I'd like to upgrade the FW on my FOCBOXes but don't know if the new VESC tool is working with FOC yet.

I read through [this thread](https://www.electric-skateboard.builders/t/vesc-project-com-is-online-public-vesc-tool-download/32268/20) but it looks like it still hasn't been solved? Is that case?
```

---
## \#13 Posted by: Maxid Posted at: 2017-10-17T03:31:00.063Z Reads: 246

```
Get the new Ackmaniac-ESC-Tool! FOC on Focboxes has been solved
```

---
## \#14 Posted by: RiGo Posted at: 2017-10-17T04:19:48.774Z Reads: 236

```
Yeah, I'm aware of that. But with the VESC-tool it hasn't? Is that what you're saying?

The reason I ask is because I wanna use [this iOS app](https://www.electric-skateboard.builders/t/new-version-2-0-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340) and it's not compatible with Ackmaniac's tool.
```

---
## \#15 Posted by: Maxid Posted at: 2017-10-17T06:38:02.732Z Reads: 225

```
The new Ackmaniac-ESC-Tool tool is based on the vesc tool and not bldc tool anymore. The app should be updated in a couple days I guess (if it is not already compatible)
```

---
## \#16 Posted by: RiGo Posted at: 2017-10-17T06:49:51.945Z Reads: 222

```
[quote="Maxid, post:15, topic:33352, full:true"]
The new Ackmaniac-ESC-Tool tool is based on the vesc tool and not bldc tool anymore. The app should be updated in a couple days I guess (if it is not already compatible)
[/quote]

I was already aware of everything you've typed in both your responses. But my question remains unanswered.

Has the FOC bug with FOCBOXes been fixed in Vedder's VESC-tool?
```

---
## \#17 Posted by: trampa Posted at: 2017-10-17T07:24:47.428Z Reads: 214

```
We had no issues passing a FOC-Box that was reported not to work. We tried several motors and PPM input devices.
All combinations worked so far. Simply give it a try. Use lower voltage when doing the detection avoid any issues (e.g. 3S battery). Should work just fine. If not: come back here or better: use the vesc-project forum and post your comment there.

Frank
```

---
## \#18 Posted by: BigBoyToys Posted at: 2017-10-17T08:45:04.431Z Reads: 211

```
He shared what he found was the problem

[quote="Ackmaniac, post:101, topic:35116, full:true"]
Took me a couple of days and a lot of testing, debugging and analyzing. Some ADC values get initialized incorrect in the first moments the FOCBOX starts (maybe the direct fets are too fast at startup).  After that it works fine.
[/quote]
```

---
## \#19 Posted by: RiGo Posted at: 2017-10-17T09:22:20.102Z Reads: 205

```
Thanks. I'll give it a go. If it doesn't work then I'll install Nico's firmware. Hopefully Vedder will fix the problem too. It would be nice if he pulled Nico's code.
```

---
## \#20 Posted by: Maxid Posted at: 2017-10-17T16:01:41.037Z Reads: 200

```
If you are aware of everything: did you actually check if the app works with the new Ackmaniac-ESC-Tool versions? I guess it will work as is - would be counterintuitive if he changed the protocol and commands
```

---
## \#21 Posted by: RiGo Posted at: 2017-10-17T20:50:11.861Z Reads: 193

```
I checked and it doesn't:

[quote="emmaanuel, post:58, topic:32340, full:true"]
Hi RiGo,

The app is compatible with standard VESC firmware (v2.18 and 3.27, 3.28 and the latest : 3.29) and Ackmaniac firmware(v2.53 and v2.54).

But at this moment the app is not compatible with the new @Ackmaniac fork based on 3.x version, because it's too hard to follow changes he is doing.

I hope he will use GitHub like the others to make it easier and add back support to his great job. 
If this change, I'll update the compatible version list in the 1st post.
[/quote]
```

---
## \#22 Posted by: Maxid Posted at: 2017-10-21T08:28:46.680Z Reads: 181

```
Seems like your problem will be solved soon
http://www.electric-skateboard.builders/t/new-version-2-0-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340/62?u=maxid
```

---
## \#23 Posted by: RiGo Posted at: 2017-10-21T21:05:10.646Z Reads: 166

```
Thanks for the heads up.
```

---
## \#24 Posted by: dAeM0N1K3 Posted at: 2017-11-03T02:26:48.659Z Reads: 139

```
[quote="Maxid, post:13, topic:33352"]
Ackmaniac-ESC-Tool
[/quote]

Guys, I just flashed my brand new FOCBOX's with the firmware included in the Ackmaniac-ESC-Tool. All was going well and I was going through the standard motor setup wizard and was running through the resistance parameter test when on the first test both FOCBOXs stopped working and are no longer powering on. Please help, I freaking out about them being fried. I just bought these things for $280. How can I get them back on?
```

---
