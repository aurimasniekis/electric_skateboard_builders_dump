# VESC 6 released and the forum is open

### Replies: 36 Views: 7108

## \#1 Posted by: oyta Posted at: 2017-09-04T20:05:13.958Z Reads: 547

```
The VESC 6 forum is now open!

http://www.vesc-project.com/

And the GitHub is updated with files!
https://github.com/vedderb/vesc_tool
https://github.com/vedderb/bldc

:slight_smile: :slight_smile:

Benjamin writes tonight:

> VESC Tool has been a huge amount of work and there are also many updates and new functions in the firmware. I will work on a reference hardware design in the next days. It will essentially be the same as the VESC6, but a square PCB with SMD electrolytic capacitors, mounting holes and a few other changes. It should work as a PCB only and not require a case for mounting. Hopefully people can adapt it easily if they want to make different cases
```

---
## \#2 Posted by: rolexbene Posted at: 2017-09-04T20:27:57.037Z Reads: 454

```
[quote="oyta, post:1, topic:32265"]
now
[/quote]

Is this not possible to run on Mac? seems to be Linux and Windows only.
```

---
## \#3 Posted by: UniqueSnowflakeN27 Posted at: 2017-09-04T20:38:34.894Z Reads: 438

```
At first I was a little baffled to see the 20€ price tag on the VESC Tool Platinum, but what the hell. Vedder has done some great work and I'll happily pay him to use his program.

One question though, in the product description it says "... You will be able to download the latest platinum status version of VESC Tool **for six months.**" 

So it's a subscription to get updates, but once I have them I can use them for however long I want?
```

---
## \#4 Posted by: marsrover001 Posted at: 2017-09-04T20:41:11.345Z Reads: 416

```
Scroll down, the tool is free. It's a kludgy way of asking for donations.
```

---
## \#5 Posted by: akhlut Posted at: 2017-09-04T20:42:05.314Z Reads: 410

```
Yeah, just read that.  Looks like it'll be like flair on the vesc forum.  Might even get your questions answered faster.  I have zero problem with this structure.  Wish he had set up a patreon or something a long time ago.
```

---
## \#6 Posted by: oyta Posted at: 2017-09-04T20:43:13.462Z Reads: 405

```
@UniqueSnowflakeN27  You can scroll down on the page and find the free version. It is only an option to support the project.

@rolexbene No MacOs version. I use Mac and utiliZe VirtualBox with Ubuntu. Works great!
```

---
## \#7 Posted by: rolexbene Posted at: 2017-09-04T20:45:41.206Z Reads: 496

```
[quote="UniqueSnowflakeN27, post:3, topic:32265"]
once
[/quote]

No it's free for life if you want, you just get a badge next to your username in the forum for 6 months for donating.
```

---
## \#8 Posted by: rpasichnyk Posted at: 2017-09-04T21:42:43.952Z Reads: 482

```
I compiled a macOS version, it runs fine, but I haven't tried to connect VESC to it yet. You can try if you are brave @oyta @rolexbene @onepunchboard https://github.com/rpasichnyk/vesc_tool/releases (vesc_tool.zip)
```

---
## \#9 Posted by: onepunchboard Posted at: 2017-09-04T21:44:36.790Z Reads: 470

```
Thanks man! I'm not doing it now, just wanted pick in. XD but eventually
```

---
## \#10 Posted by: onepunchboard Posted at: 2017-09-04T21:56:55.830Z Reads: 463

```
I just found this,

under debug console
WARNING (:0 ): Execution of PAC script at "http://wpad/wpad.dat" failed
```

---
## \#11 Posted by: oct0f1sh Posted at: 2017-09-04T23:47:20.867Z Reads: 431

```
May be a dumb question but can you use the VESC tool with an older VESC? One that's not a VESC 6?
```

---
## \#12 Posted by: JLabs Posted at: 2017-09-04T23:52:43.938Z Reads: 384

```
Yes you can, and it’s considered an upgrade to use it over the BLDC tool
```

---
## \#13 Posted by: cwazy1 Posted at: 2017-09-04T23:57:08.571Z Reads: 360

```
I'm not quite understanding how it is an upgrade to use vesc tool over bldc tool with 4.12HW and 2.18FM? The only advantage would be its upgraded UX?
```

---
## \#14 Posted by: JLabs Posted at: 2017-09-04T23:58:22.916Z Reads: 345

```
Have a read around the VESC forum.. Benjamin said it was better with FOC especially. I’m not exactly sure of the specifics yet
```

---
## \#15 Posted by: cwazy1 Posted at: 2017-09-05T00:04:54.910Z Reads: 347

```
Well, per Franks post, FOC is only better if upgrade to the new 3.27 FW running on 4.12 HW. It is not the tool itself that will grant better FOC-ing (heh)

> _You can access the VESC-Tool download and the forum, other sections will follow soon. Beside a good start into the week you will be able to use the new FW 3.27 with your 4.xx hardware. Your 4.xx will still be a 4.xx, but FOC is a lot better and all the new features, like the input wizards and throttle curves, are available. Note that this update won't make HW 4.x more robust against broken DRVs for certain motors, so if you had problems with a motor and HW 4.x before it is likely to remain._

What I didn't understand is if it is **required** to upgrade to 3.27FW on 4.12HW in order to use vesc tool.
```

---
## \#16 Posted by: UniqueSnowflakeN27 Posted at: 2017-09-05T06:26:58.126Z Reads: 308

```
Yeah, I saw that. But I thought the free version was like a lite version or something.
```

---
## \#17 Posted by: rich Posted at: 2017-09-05T07:02:47.586Z Reads: 314

```
[quote="cwazy1, post:15, topic:32265"]
What I didn't understand is if it is required to upgrade to 3.27FW on 4.12HW in order to use vesc tool.
[/quote]

Yes, you have to update FW to use VESC-Tool but you can upload bootloader (or upload different FW but then you can't use vesc tool for settings)
```

---
## \#18 Posted by: MontPierre Posted at: 2017-09-08T10:01:43.841Z Reads: 287

```
@rpasichnyk will your compiled Mac version have updates? Have you been able to re compile new update?
```

---
## \#19 Posted by: rpasichnyk Posted at: 2017-09-08T10:42:25.343Z Reads: 285

```
Yes I plan to build 0.81 for macOS. Though I hope at some point it will be possible to download from the official website. I am willing to help with that.
```

---
## \#20 Posted by: trampa Posted at: 2017-09-08T10:59:11.743Z Reads: 282

```
:wink: Frank
```

---
## \#21 Posted by: xxlv Posted at: 2017-09-08T14:54:21.933Z Reads: 279

```
The new way for managing parameters and (de-)serialisation is well made and really cool. I like it. Thank you Benjamin. Very easy to extend. I can finally implement my Pedelec App. :)
```

---
## \#22 Posted by: rpasichnyk Posted at: 2017-09-08T16:54:26.327Z Reads: 270

```
https://github.com/rpasichnyk/vesc_tool/releases/tag/v0.81 ping @MontPierre
```

---
## \#23 Posted by: MontPierre Posted at: 2017-09-08T16:55:47.238Z Reads: 260

```
@rpasichnyk :kissing_closed_eyes:
```

---
## \#24 Posted by: MontPierre Posted at: 2017-09-08T17:13:19.507Z Reads: 257

```
Wow. BLDC Mode with SK3 6374 190kv Sensorless motor and no cogging ( bench test). Just WOW! 

EDIT - thats because I habe changed minimum duty Cycle from 0.5% to 0.8% ( Motor->General->Advanced)

Waiting for my sensored motors to brave FOC on focbox!
```

---
## \#25 Posted by: ThierryGTLTS Posted at: 2017-09-09T08:37:24.020Z Reads: 256

```
Hi XXLV,

I'm very interested by your Pedelec app.

What sensor will you use to detect crank movement?

Have a Nice Day.

Thierry
```

---
## \#26 Posted by: NAF Posted at: 2017-09-12T05:13:20.517Z Reads: 232

```
Thank you !!!
```

---
## \#27 Posted by: telnoi Posted at: 2017-10-03T13:30:36.739Z Reads: 219

```
Thanks for the OSX version. Are you planning on updating it to 3.29?
```

---
## \#28 Posted by: rpasichnyk Posted at: 2017-10-03T13:41:40.284Z Reads: 224

```
Done already https://github.com/rpasichnyk/vesc_tool/releases , v0.82
```

---
## \#29 Posted by: Pimousse Posted at: 2017-10-03T13:45:35.723Z Reads: 228

```
Sorry @rpasichnyk, I didn't get why you forked official VESC Tool.
Is it to make it work with your app ?
Or some kind of improved version ?
```

---
## \#30 Posted by: rpasichnyk Posted at: 2017-10-03T13:58:12.801Z Reads: 226

```
I forked it to make it compile on macOS. I did some small pull requests and all of them were accepted upstream. I keep this fork just to have Releases section where people can download VESC Tool for macOS. It is 100% the same functionality as official, except there is no official version for macOS.
```

---
## \#31 Posted by: NAF Posted at: 2017-10-03T15:27:40.391Z Reads: 211

```
Huge thanks dude for keeping OSX version alive !! Finally I can update to 3.29. We will see how the breaking is gonna work now.
```

---
## \#32 Posted by: gogomrrobot Posted at: 2017-10-03T20:13:22.602Z Reads: 204

```
Yes thanks @rpasichnyk for the OSX version :)
```

---
## \#33 Posted by: PDXroses Posted at: 2017-12-06T02:39:25.121Z Reads: 189

```
Dude!  Thank you!
```

---
## \#34 Posted by: PDXroses Posted at: 2017-12-06T03:07:18.378Z Reads: 193

```
Sorry.  One more question.  If I choose to, I can configure the firmware on a blank VESC the old way (that's on Vedder's site).  Correct?
```

---
## \#35 Posted by: jacklondon Posted at: 2018-09-14T19:32:19.448Z Reads: 111

```
[quote="rpasichnyk, post:28, topic:32265"]
https://github.com/rpasichnyk/vesc_tool/releases
[/quote]

what version of osx do I need to run for this to work? No luck on 10.9
```

---
## \#36 Posted by: rpasichnyk Posted at: 2018-09-15T11:15:24.741Z Reads: 96

```
The minimum required version of macOS is 10.10
```

---
