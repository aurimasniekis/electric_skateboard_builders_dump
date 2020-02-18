# VESC-Project.com is online! Public VESC-Tool download

### Replies: 620 Views: 27293

## \#1 Posted by: trampa Posted at: 2017-09-04T20:39:14.291Z Reads: 1128

```
Hi Builders, we are proud to announce that from now on, the website www.vesc-project.com is online!
It took a very long time time to get to this point, but we think it was worth to taking the time. 
The project now rests on solid foundations to build upon, easing things in future.

What can you expect?
You can access the VESC-Tool download and the forum, other sections will follow soon. Beside a good start into the week you will be able to use the new FW 3.27 with your 4.xx hardware. Your 4.xx will still be a 4.xx, but FOC is a lot better and all the new features, like the input wizards and throttle curves, are available. Note that this update won't make HW 4.x more robust against broken DRVs for certain motors, so if you had problems with a motor and HW 4.x before it is likely to remain.

VESC-Tool is available in various versions. They are all perfectly the same except one tiny detail: If you choose to contribute financially to the growths of the project, you will be granted a status according to your donation. A polished logo and special thanks will always remind you of your big-hearted decision to support the project. A status version of VESC® Tool can be upgraded for 6 months without loosing the status badge.

Users of the original hardware can download VESC® Tool _Original_, entering a code for access that will be supplied with your hardware purchase. 

Users of hardware not having a bootloader installed will profit from using VESC-Tool. Benjamin added a bootloader upload tab that can be found under the firmware section. This way you will be able to use the new firmware without the need to install a bootloader via a st-link programmer. Your USB connection does the job!

The first time you upload the new firmware to a HW4.xx ESC you must select the correct hardware version in VESC Tool, as the old firmware does not tell VESC Tool which hardware version it is. After the first update the hardware will be selected automatically.

Please visit the forum on the vesc-project website and read through the sticky threads in the beta section - especially this one: http://www.vesc-project.com/node/82
Third party hardware and software, such as bluetooth modules and apps, should only be used if the distributor confirms the safe usage in combination with the new FW! Check first, then use! 

Frank
```

---
## \#2 Posted by: Rinzler Posted at: 2017-09-04T20:54:14.827Z Reads: 798

```
[quote="trampa, post:1, topic:32268"]
Users of the original hardware can download VESC® Tool Original, entering a code for access that will be supplied with your hardware purchase.
[/quote]
Can you explain in more detail what do you mean by _original hardware_, and the hardware purchase thing.
Thanks
```

---
## \#3 Posted by: Titoxd10001 Posted at: 2017-09-04T21:08:26.526Z Reads: 773

```
Shoot I selected the wrong hardware version for focbox. How can I change it now? 

Suppose to be 412 right?
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-09-04T21:14:52.414Z Reads: 730

```
in what way foc is better in 4.12. im using 218 foc it is stable at the moment, but does this tool improve over the old?
```

---
## \#5 Posted by: onepunchboard Posted at: 2017-09-04T21:19:29.637Z Reads: 696

```
And btw no mac ver yet i guess.
```

---
## \#6 Posted by: trampa Posted at: 2017-09-04T21:23:07.321Z Reads: 679

```
We offer the original VESC-Project hardware release and there is a VESC-Tool Original version available for this piece of hardware. It's pretty much the same like the other releases but using a different branding and status badge. For the beta phase we excluded the HW 4.xx FW in this version for example. We know our hardware and this enables Benjamin to e.g. set different limits for the configuration that would maybe kill other hardware. 
We will see more different hardware in future and some HW might have different limits. In consequence you need a VESC-Tool more specific for this piece of HW. Houses for courses.....

Frank
```

---
## \#7 Posted by: trampa Posted at: 2017-09-04T21:23:51.007Z Reads: 637

```
Just upload the 4.12 again.

Frank
```

---
## \#8 Posted by: trampa Posted at: 2017-09-04T21:25:19.905Z Reads: 624

```
You should update! 2.xx is outdated. The new FW is a lot better. It's not recommended to use the old FW and BLDC-Tool any more.

Frank
```

---
## \#9 Posted by: trampa Posted at: 2017-09-04T21:26:29.618Z Reads: 613

```
No MAC, sorry. You can run a virtual machine though. Virtualbox should work.

Frank
```

---
## \#10 Posted by: onepunchboard Posted at: 2017-09-04T21:26:48.524Z Reads: 607

```
Thank you Frank!
```

---
## \#11 Posted by: rpasichnyk Posted at: 2017-09-04T21:27:57.269Z Reads: 596

```
I just got it compiled on macOS. Haven't connected to my VESC yet but it looks promising!

<img src="/uploads/db1493/original/3X/a/9/a9af495c64206dd1036f168e6d081a80e94ac007.png" width="690" height="359">
```

---
## \#12 Posted by: Titoxd10001 Posted at: 2017-09-04T21:31:56.274Z Reads: 586

```
I had accidentally uploaded focbox as HW as 48 and now I don't see option to change to 412. Do you mean bootloader tab?
```

---
## \#13 Posted by: Yecrtz Posted at: 2017-09-04T21:41:31.634Z Reads: 574

```
Can I download it without making an account?
```

---
## \#14 Posted by: trampa Posted at: 2017-09-04T21:43:07.637Z Reads: 575

```
No, you need an account.

Frank
```

---
## \#15 Posted by: trampa Posted at: 2017-09-04T21:48:46.364Z Reads: 575

```
Once you uploaded the FW, VESC-Tool will recognize your HW and you will only get suitable FW as an option.
For non-default FW there is checkbox below the FW window. 

Changing the FW if this has happened:

Download FW for HW 4.12:
https://github.com/vedderb/bldc/blob/master/build_all/410_o_411_o_412/VESC_default.bin?raw=true
Use the custom file tab in VESC Tool to upload the firmware.

Frank
```

---
## \#16 Posted by: Titoxd10001 Posted at: 2017-09-04T21:56:10.468Z Reads: 551

```
Won't connect to BLDC tool anymore. Only connects to VESC tool
```

---
## \#17 Posted by: onepunchboard Posted at: 2017-09-04T22:00:31.224Z Reads: 536

```
I use FOCBOX, so is it hw 48 or 412?
```

---
## \#18 Posted by: trampa Posted at: 2017-09-04T22:03:16.215Z Reads: 546

```
It has always been an ordinary 4.12 with Direct FETs. This is exactly the reason why its better to tell your customers what HW version they deal with.

Don't FOC your Box by choosing the wrong FW! 

Frank
```

---
## \#19 Posted by: onepunchboard Posted at: 2017-09-04T22:08:14.589Z Reads: 549

```
Thanks again!
```

---
## \#20 Posted by: qdxiatao Posted at: 2017-09-05T00:46:45.563Z Reads: 544

```
@Frank,Great work!
```

---
## \#21 Posted by: evoheyax Posted at: 2017-09-05T00:56:05.902Z Reads: 516

```
day day has finally come...

@trampa Could you explain at all why this firmware is much better on the 4.12 vesc's than the 2.18 FW? Just curious...
```

---
## \#22 Posted by: Titoxd10001 Posted at: 2017-09-05T01:13:49.469Z Reads: 513

```
Have to be honest. Vesc tool hype is disappointing. As I can tell it does the same as BLDC tool. Just in a "prettier" interface. Has setup wizards but the one I think is useful is ppm input wizard which ackmaniacs extended firmware already has. The motor detection is more "complicated" as it failed first try, had to adjust voltage and erpm. The motor readings are different from BLDC tool so not sure what that means (I used 10amps and 800erpm?). The control modes are the same. For those hoping for DUTY cycle with neutral it didn't happen which is the reason I was looking forward to the tool.  For reverse you cannot set it up so you have to double tap the brakes to engage reverse like hobbywing escs or one step further like @Ackmaniac firmware where you have to decrease erpm to a certain number to safely start reversing (Extended Vesc-tool?) I have not tried the foc tab.

If you're use to BLDC tool, vesc tool seems more complicated because everything has it's own tab. I mention all this because if you switch to VESC tool you cannot go back to BLDC tool without bootloader
```

---
## \#23 Posted by: SeanHacker Posted at: 2017-09-05T01:19:31.079Z Reads: 503

```
I can't even get through an FOC detection with this. Keeps saying "R is 0 Please measure it first." Hmmm.... :frowning:
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2017-09-05T01:22:10.512Z Reads: 501

```
Hey Guys just a fair Warning... As stated in the warning at the beginning of the tool it is still experimental... and **as not been tested** properly by everyone so it might void some waranty... and it seem that you can't go back to old firmware after, without uploading the old bootloader

<img src="/uploads/db1493/original/3X/9/5/954bca7ce19782164eddd717491ab2270dfd2bad.JPG" width="374" height="500">
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2017-09-05T01:23:09.087Z Reads: 484

```
[quote="SeanHacker, post:23, topic:32268"]
I can't even get through an FOC detection with this
[/quote]

I got the same issue... That why until further notice and more test It still as to be consider EXPERIMENTAL.
```

---
## \#26 Posted by: onepunchboard Posted at: 2017-09-05T01:37:54.450Z Reads: 475

```
that's a huge disappointment, I was looking forward to upgrade fmw and make comparison video in FOC performance
```

---
## \#27 Posted by: sl33py Posted at: 2017-09-05T01:58:03.200Z Reads: 487

```
I hear what you are saying Titoxd - but disagree on one major point.  Simplicity to load and connect/configure a VESC.

Sure, i have a linux laptop somewhere - followed step by step Ben's guide and it works well.  But then i had an issue and tried to reload it...  and had issues (like one of the library paths changed)...  So then i need to hunt down one of the ported for windows version - which are super specific on what firmware is on that VESC.  Except i have 9 VESC now...  And only configure one every 5-6 months (once setup - no need ot fiddle w/ it)

So from the simplicity of plug-n-play - i find the new VESC Tool a LOT easier.  I'm a linux noob (but in IT - go figure... MS has paid the bills for years and i stick to Windows).

All i'm trying to say is a few minutes in the new tool were a ton easier - wizard driven setup.  Info on nearly every button.  Explanations of settings, etc.  Far improved.  If you need to fiddle w/ your amps to detect that seems a small price to pay?
```

---
## \#28 Posted by: Titoxd10001 Posted at: 2017-09-05T02:25:01.749Z Reads: 466

```
I didn't like the wizard tbh every page has warnings and popup boxes. In BLDC tool I look at 4 tabs/pages and in vesc tool I have to look at 10 to make same changes. Not a big deal just wanted to mention it. 

As for motor detection what is recommended 
For amps and erpm and duty cycle
```

---
## \#29 Posted by: NAF Posted at: 2017-09-05T03:32:36.107Z Reads: 450

```
Can you upload mac version somewhere? Please. I d love to have it.
```

---
## \#30 Posted by: SeanHacker Posted at: 2017-09-05T03:36:03.566Z Reads: 452

```
He did already. ;)

https://www.electric-skateboard.builders/t/vesc-6-released-and-the-forum-is-open/32265/8?u=seanhacker
```

---
## \#31 Posted by: rich Posted at: 2017-09-05T07:09:43.112Z Reads: 442

```
[quote="JohnnyMeduse, post:24, topic:32268"]
and it seem that you can't go back to old firmware after, without uploading the old bootloader
[/quote]


No, it's very easy to upload "old" FW. In VESC-Tool in the firmware tab you choose custom file and can upload any FW, after upload is done you just need to open the respective BLDC Tool for settings.

BTW I love this VESC-Tool :heart_eyes: and new FW, already used it in FOC on HW4.12 for 400km without problems. 
[quote="Titoxd10001, post:22, topic:32268"]
For reverse you cannot set it up so you have to double tap the brakes to engage reverse like hobbywing escs or one step further like @Ackmaniac firmware where you have to decrease erpm to a certain number to safely start reversing
[/quote]

That's the only point I'm missing, too.... would love to use reverse function but it is too dangerous now.
```

---
## \#32 Posted by: trampa Posted at: 2017-09-05T07:30:07.773Z Reads: 420

```
Exactly! You are not locked! 
We strongly recommend to update to the latest FW, using VESC-Tool.
2.xx is outdated and will get no more updates.
Bugs simply get no fixes. 
Using VESC-Tool, you will be notified if a new Version is available, which is pretty convenient.
You won't miss critical updates and new features.
This way you are always up to date. There will be frequent updates available. You can also write feature requests in the corresponding forum section. We will have a close look at this! This way everyone can help to improve the software. 

Frank
```

---
## \#33 Posted by: NAF Posted at: 2017-09-05T07:30:29.103Z Reads: 402

```
Did you notice any improvements with new FOC ?
```

---
## \#34 Posted by: rich Posted at: 2017-09-05T07:41:55.833Z Reads: 411

```
I know that there are many improvements in FOC with the new FW that's why I gave FOC a try. I've never tried FOC with FW 2.18 because I was afraid to fry my HW so I can't tell you about difference in performance but it seems that FOC is much safer now with the new FW. As said I'm running sensored FOC on HW 4.12 on my dual drive MTB since 400km and fell in love and will never ever go back to BLDC :laughing: , but I switch to VESC 6 soon.

Thanks benjamin, frank & ted for all the time you spent on this!
```

---
## \#35 Posted by: NAF Posted at: 2017-09-05T07:43:30.351Z Reads: 402

```
I am already running FOC ..but it sounds really tempting to try new VESC TOOL. I'll give it a try in a few minutes and ll report back to you guys if there is any noticeable difference.
```

---
## \#36 Posted by: NAF Posted at: 2017-09-05T09:08:26.356Z Reads: 416

```
Ok guys ...everything went smooth as a butter. There were no problems with updating to new firmware. Vesc wizard configuration tool for motor and ppm went quick. It's definitely going to be easy now for anyone who is just starting their adventure with vesc. **But what's most important is FOC !!!**

Nice work Benjamin Vedder. ! **FOC configuration went** super quick but I can already tell that there is a difference between old FOC and new one. I have **Carvon V2.5 single drive** , and FOC with previous BLDC Tool was running great except the fact that at slow press of the trigger on my remote the motor was cogging. Right now after I have setup everything with the new tool, it seems like the cogging is gone. It's all bench testing right now and I need to take the board for a quick ride but in reality FOC works always better when riding than on the bench. So I expect major improvement here. I'll let you know later today after the ride. So far I am pretty impressed. Great job guys.

**_Oh and what's important I have configured everything on MAC with the build from @rpasichnyk so I can confirm the new software works 100% on OSX._**
```

---
## \#38 Posted by: trampa Posted at: 2017-09-05T09:23:30.368Z Reads: 411

```
You have 10 Cells in series, not 40! The P doesn't count. **10**S 4P

Frank
```

---
## \#39 Posted by: NAF Posted at: 2017-09-05T09:24:54.295Z Reads: 410

```
Hahahhaha !! True that ! I guess I got too excited !
```

---
## \#40 Posted by: Pimousse Posted at: 2017-09-05T09:26:10.448Z Reads: 404

```
I repeat it again : thank you very much @trampa and Ben !
You did an amazing job and this public sources release is the proof that convince me I have been a part of a wonderful and promising open-source project. :relieved:
```

---
## \#41 Posted by: Silverline Posted at: 2017-09-05T10:19:23.075Z Reads: 396

```
So what about the so called 'v-tech' boost on 4,12 HW with 'old' 2,18 fw. Is it Better on the new fw ?

I have two focboxes running sk3 outrunners without sensors in bldc at the moment. Any benefits running Them in FOC mode on the new fw, even when they are not sensored ?
```

---
## \#42 Posted by: trampa Posted at: 2017-09-05T10:21:01.333Z Reads: 377

```
FOC em!

Frank
```

---
## \#43 Posted by: Silverline Posted at: 2017-09-05T10:22:54.396Z Reads: 369

```
I think my trampa board is going to be happy then. And the 'v-tech' thing ?
```

---
## \#44 Posted by: trampa Posted at: 2017-09-05T10:24:44.370Z Reads: 369

```
V-Tech? 10Char
```

---
## \#45 Posted by: NAF Posted at: 2017-09-05T10:25:56.406Z Reads: 363

```
yeee what's V-Tech ?
```

---
## \#46 Posted by: GrecoMan Posted at: 2017-09-05T10:26:41.355Z Reads: 359

```
I think l he means the little boost you get when you hit max efficiency on the motor
```

---
## \#47 Posted by: trampa Posted at: 2017-09-05T10:27:50.638Z Reads: 350

```
It's the V-force! Use it.

Frank
```

---
## \#48 Posted by: GrecoMan Posted at: 2017-09-05T10:28:52.192Z Reads: 351

```
It's kinda annoying sometimes when your not expecting it then you get a boost at 25mph, it can be a little scary sometimes
```

---
## \#49 Posted by: trampa Posted at: 2017-09-05T10:34:48.860Z Reads: 350

```
I don't get those boosts, riding motor amp = battery amp. 
Butter smooth! You can also adjust the throttle curves now. 
Really really smooth!
I haven't used BLDC Tool and 2.18 FW for 18 months now....

Frank
```

---
## \#50 Posted by: GrecoMan Posted at: 2017-09-05T10:36:21.245Z Reads: 343

```
Glad it's "fixed"! I'll have to give it a try later today, I was download like 218 yesterday
Ive used ackmaniacs fw for a while so I've already got most of those features. 😉
```

---
## \#51 Posted by: Klattrup Posted at: 2017-09-05T10:36:40.538Z Reads: 353

```
I just tried the free tool option. I have two VESCs from vesc.co.uk and they have no bootloader. I thought I'd try the tool before purchasing.

First off the links I received in my purchase mail did not work - the HTML is broken - it does however tell me that I can re-download from the site directly under _My account_. Those links work, but file gets blocked by my firewall (Sonicwall hardware firewall) that states the files contains a virus **MalAgent.I_13584 (Trojan)** :frowning:

_EDIT:_ Of cause I belive this is a false positive, but if other receives this as well it should be made **very** clear on the page that this can happen but that the file is still safe!
```

---
## \#53 Posted by: rich Posted at: 2017-09-05T12:50:31.209Z Reads: 349

```
[quote="Klattrup, post:51, topic:32268"]
but file gets blocked by my firewall (Sonicwall hardware firewall) that states the files contains a virus MalAgent.I_13584 (Trojan) :frowning:
[/quote]

Yes there's something wrong, I have to deactivate Avast Antivirus otherwise I can't open VESC-Tool. That's since I have it. The avast software automatically send the file to "antivirus labor" for investigation and after a couple of hours they say it should be safe but it still happens everytime I try to open it when the antivirus software is active :worried:
```

---
## \#54 Posted by: NAF Posted at: 2017-09-05T13:00:06.340Z Reads: 338

```
Ok so I did some real life testing ..I went around 10miles to try the new FOC ..and indeed it works a lot better than with the previous firmware. There is finally no cogging on my motor at slow speeds...it just runs buttery smooth almost as if it was sensored. Awesome work.
```

---
## \#55 Posted by: Silverline Posted at: 2017-09-05T14:13:19.354Z Reads: 339

```
Yes exactly, the boost that always comes when you least expect it.

But it sounds like its been cured ?
```

---
## \#56 Posted by: Vanarian Posted at: 2017-09-05T14:48:25.902Z Reads: 347

```
F*ck yeah ! I second this ! Thanks guys.

@trampa Frank I love how enthusiast you are about the features discussed up there, shows a lot about the work and confidence you've put in it. You're making everything in the DIY worth it.
```

---
## \#57 Posted by: Silverline Posted at: 2017-09-05T15:34:33.609Z Reads: 363

```
Just did the update on a regular 4,12 vesc. 

When i check the fw, it says HW 4,10, but i think its the same firmware, even though mine is HW 4.12?
<img src="/uploads/db1493/original/3X/5/f/5f038bd838572f65410131a520816fca3d39a802.jpg" width="690" height="388">

Two quistions though. 

First time FOC user. When i test my motor on the bench in FOC mode (No load) it has some sort of delay when i brake , is this normal , and when i hit the Street this delay Will not happen ?

I have a regular motor without sensors. Is this the right settings , when i want to run it in FOC mode ? (i have done the FOC motor detection values)
<img src="/uploads/db1493/original/3X/0/1/01826bb1bc08b7fb6836a5022d61eb317b479c50.jpg" width="690" height="388">
```

---
## \#58 Posted by: trampa Posted at: 2017-09-05T17:16:16.001Z Reads: 341

```
Usually there is no delay. Did you run both input wizards, motor and app?

Frank
```

---
## \#59 Posted by: Silverline Posted at: 2017-09-05T17:27:53.209Z Reads: 338

```
I did run the FOC motor detection under "general" and the app for my remote.

Just back from a test ride. I`m totally in love in FOC. But again i noticed that when i`m running full duty cycle, and i let go on the throttle to mid. position, their is some sort of delay, same thing happen when i brake, and the let go on the trottle back to mid position. I did not have this delay before on bldc and old firmware.
```

---
## \#60 Posted by: Jinra Posted at: 2017-09-05T17:46:44.598Z Reads: 328

```
Anyone have hard numbers on how much speed you lose with FOC over BLDC?
```

---
## \#61 Posted by: Silverline Posted at: 2017-09-05T17:54:27.884Z Reads: 331

```
On my test ride, i did loose 3 km/h..... And i need to test it more, but i think that i did use a little more juice also. But damn, the board feels so much better
```

---
## \#62 Posted by: onepunchboard Posted at: 2017-09-05T17:57:03.315Z Reads: 330

```
it's tempting to go vesc tool but u said delay. hmm it's  ppm?
```

---
## \#63 Posted by: Silverline Posted at: 2017-09-05T17:59:37.667Z Reads: 320

```
Yes... i did not have that before on BLDC - 2.18 Fw. Maybe it`s just how FOC works with sensorless motor ?
```

---
## \#64 Posted by: onepunchboard Posted at: 2017-09-05T18:00:21.785Z Reads: 323

```
I'm usin foc sensor less but not happeneing for me. also 2.18
```

---
## \#65 Posted by: Silverline Posted at: 2017-09-05T18:02:09.811Z Reads: 326

```
Strange. This is on PPM yes, and the Gt2B remote. Maybe it`s only some settings ? I only did the min, mid and max calibration under App config.

But i love that i don`t have that darn Boost thing anymore :-)
```

---
## \#66 Posted by: trampa Posted at: 2017-09-05T18:05:24.452Z Reads: 318

```
Run the Wizard and see if the same issue happens.

Frank
```

---
## \#67 Posted by: JohnnyMeduse Posted at: 2017-09-05T18:08:55.674Z Reads: 313

```
i just don't remember where (and I don't have my pc in front of me), but you have to change some setting in order to remove that delay
```

---
## \#68 Posted by: Ackmaniac Posted at: 2017-09-05T18:10:01.155Z Reads: 314

```
Does it  ring when I say ppm ramping.
```

---
## \#69 Posted by: Silverline Posted at: 2017-09-05T18:10:35.568Z Reads: 314

```
Interesting :stuck_out_tongue:Now go find your computer :-)
```

---
## \#70 Posted by: JohnnyMeduse Posted at: 2017-09-05T18:12:30.993Z Reads: 302

```
I think it is in advanced setting (could you post a screen shoot)
```

---
## \#71 Posted by: Silverline Posted at: 2017-09-05T18:25:42.217Z Reads: 307

```
Motor settings -> General -> Advance ??

Or, Motor settings -> FOC -> Advanced
```

---
## \#72 Posted by: SORRENTINO Posted at: 2017-09-05T18:31:49.703Z Reads: 310

```
So the boost issue has been fixed with this firmware?
```

---
## \#73 Posted by: onepunchboard Posted at: 2017-09-05T18:36:21.739Z Reads: 310

```
did u figure out foc detection issue?
```

---
## \#74 Posted by: Silverline Posted at: 2017-09-05T18:36:30.575Z Reads: 311

```
All i can say is, that before on BLDC - 2.18 fw, i had the boost. And now it`s gone totally. But i have not tried BLDC on 3.27 fw though.
```

---
## \#75 Posted by: JohnA Posted at: 2017-09-05T18:44:41.166Z Reads: 314

```
Im using the new tool to set up my focboxes, but when I finish using both wizards the esc won't spin the motors. I can go into the ppm tab and see that it is getting the signal from the receiver. And when I do the motor detection it spins the motor, but won't spin from the computer controls or controller. (was setting up in for, but also bldc won't work either) any ideas? @trampa
```

---
## \#76 Posted by: JohnA Posted at: 2017-09-05T18:46:02.394Z Reads: 314

```
the only thing that works is clicking the anchor to engage the brake, and the stop button then disengages it.
```

---
## \#77 Posted by: Silverline Posted at: 2017-09-05T18:48:09.348Z Reads: 317

```
Under App settings -PPM. "Control Type" did you set it to "Current no reverse with brake " And Write to the vesc ?
```

---
## \#78 Posted by: JohnA Posted at: 2017-09-05T18:51:00.850Z Reads: 317

```
<img src="/uploads/db1493/original/3X/d/6/d62716f8023b78c29b5939db4c64b0b899685ba0.png" width="690" height="431">yes I did, heres a picture of ppm tab, have tried other control types and wrote configuration and they didn't work either
```

---
## \#79 Posted by: Silverline Posted at: 2017-09-05T18:52:57.660Z Reads: 301

```
What about App settings -> General -> "App to use" ? Does it say PPM or PPM and UART ?
```

---
## \#80 Posted by: JohnA Posted at: 2017-09-05T18:54:55.133Z Reads: 323

```
<img src="/uploads/db1493/original/3X/3/9/39201d8bc7e9ac03e9602bb37a4315334fb7f316.jpg" width="690" height="431">on ppm, I also tried it on "ppm and UART" with no luck. no faults or anything in terminal, were working prior to the update. Using Gtb2 controller and have the ppm input set
```

---
## \#81 Posted by: JohnnyMeduse Posted at: 2017-09-05T19:03:37.173Z Reads: 324

```
@Silverline

Put this parameter at 0.1 and it should do the trick ... also thanks @Ackmaniac 

<img src="/uploads/db1493/original/3X/6/9/6931c24671717daec9bc6c88905b61bdf4f1e58f.JPG" width="690" height="431">

@onepunchboard no I wasn't able to properly run a motor detection... so I won't be using this software inside a board until further testing
```

---
## \#82 Posted by: JohnA Posted at: 2017-09-05T19:06:51.897Z Reads: 329

```
<img src="/uploads/db1493/original/3X/1/d/1dcaa5e16c9d9654557bd3fa81e71b47c7c20d7e.png" width="690" height="431">Still nothing. thanks for the help though guys @Silverline @Ackmaniac @JohnnyMeduse<img src="/uploads/db1493/original/3X/c/0/c074cfd0806a98cc22716932d995cb6707782df7.png" width="690" height="431">And in other picture you can see it is getting PPM signal as I pull the trigger
```

---
## \#83 Posted by: Silverline Posted at: 2017-09-05T19:10:51.088Z Reads: 306

```
Thanks @JohnnyMeduse

Just to be sure. When i`m running full duty cycle, and let go on the throttle, it has a little delay before the motor starts decrease in rpm`s. Same thing, when i make a full brake, and let go on the trigger to neutral, it holds the brake for a split second, before it stops braking. So do you think the changing the Positive ramping time, will affect both these "symptoms" or do i need to play with the negative ramping time as well ?
```

---
## \#84 Posted by: JohnA Posted at: 2017-09-05T19:12:50.979Z Reads: 310

```
@Silverline could you just need to turn off the median filter? says it delays to reduce noise  "use a median filter on the decoded pulses. Will delay the signal slightly, but rejects outliers caused by noise."
```

---
## \#85 Posted by: Jinra Posted at: 2017-09-05T19:20:12.231Z Reads: 304

```
Why would you even want a positive/negative ramping delay? Couldn't these just be left at 0?
```

---
## \#86 Posted by: JohnnyMeduse Posted at: 2017-09-05T19:21:47.811Z Reads: 300

```
Don't know... I feel the same way...
```

---
## \#87 Posted by: chuttney1 Posted at: 2017-09-05T19:26:45.840Z Reads: 300

```
I'm hoping this works out well for HW 4.7.
```

---
## \#88 Posted by: GrecoMan Posted at: 2017-09-05T19:30:03.420Z Reads: 293

```
Anyone tried FOC with the torque VESC? Stupid question but does this fw make FOC safer for the vesc?
```

---
## \#89 Posted by: Jinra Posted at: 2017-09-05T19:33:53.847Z Reads: 289

```
It's probably too new to say how well this will work on 4.12 VESCs. I have heard of a lot of people blowing their toqueboards VESC with, and even without, FOC.
```

---
## \#90 Posted by: GrecoMan Posted at: 2017-09-05T19:34:35.231Z Reads: 284

```
Lol yep, I’m itching to try FOC but don’t have the money to shell out for a new vesc if my tb one breaks.
```

---
## \#91 Posted by: onepunchboard Posted at: 2017-09-05T19:34:56.331Z Reads: 281

```
New fmw i check th vd's note says improved current detection what not
So im guessing stability update.
```

---
## \#92 Posted by: GrecoMan Posted at: 2017-09-05T19:35:43.356Z Reads: 276

```
Hmmm, I’ll try BLDC on it for now. Later when I get the money for a new vesc, I’ll try FOC on the torque vesc, for science!!
```

---
## \#93 Posted by: Jinra Posted at: 2017-09-05T19:56:53.810Z Reads: 276

```
godspeed...
```

---
## \#94 Posted by: UniqueSnowflakeN27 Posted at: 2017-09-05T20:00:45.247Z Reads: 286

```
As soon as I'm done with my build & confident in how to set up FOC I'll try it on my two Torqueboards VESCs @GrecoMan !
```

---
## \#95 Posted by: UniqueSnowflakeN27 Posted at: 2017-09-05T20:40:59.950Z Reads: 292

```
[Just tried FOC on my Torqueboards VESC and 75KV hub motor, sensorless!](https://youtu.be/6bka49gULmk) There's a big difference in [how it handled compared to the FOC using BLDC Tool!](https://www.youtube.com/watch?v=XG4XvvkLFKw)

It feels like it has more torque. Maybe I've got some settings wrong, but it feels like it's louder now than it was before though... It's not bad, but I'm pretty sure it wasn't as loud as it is now.

It doesn't cog half has bad when on low rpms! Though I'm going to hook up the sensors eventually, so hopefully there will be none of that.

To set the correct eRPM I took voltage * motor KV * magnet pole pairs which gave me 42*75*14=44100 but I rounded it down to 44000. Is that too conservative and how does it effect the perfomance?

[Here's a bonus video](https://www.youtube.com/watch?v=ksmnQYjbnLQ) of it running in BLDC. The cruise controll makes it stall/stutter. Not sure what that is all about.
```

---
## \#96 Posted by: Klattrup Posted at: 2017-09-05T20:47:42.473Z Reads: 298

```
Updated my two 4.12's today. Worked perfectly and the new tool is VERY easy to use with the wizards! Huge applause for Frank, Vedder and friends for making this available to us! :)

I've been running BLDC until now on my 12S eMTB but I decided to try out the much hyped FOC-mode on the new firmware. As a total newb to this mode I found the wizard super helpful once again and motor detection went smooth as butter. After all was set up I immediately found the lower noise attractive and startup from standstill was now finally doable - YAY! :) :) 
The thing is though.. when applying more aggressive throttle I only accelerated slowly and at a certain speed I actually felt at bit of clogging and ups'n'downs in speed until I reached a point where acceleration felt smooth again - I never went really fast as I did not feel comfortable with this.

I tried doing a new round of motor detection but still the same - eventually I switched back to BLDC (still on the new FW) and everything now seems to be like before - and I DO find that insanely fun as I've driven 400 kilometers in the last three weeks on this thing! :D 

Guess I'll try FOC again at a later time when I've read more about it's tweaks and tricks. :)

Again - thank you Frank and Vedder! :+1:
```

---
## \#97 Posted by: mmaner Posted at: 2017-09-05T21:09:42.342Z Reads: 281

```
Are there any updates to the VESC 4.xx firmware that weren't already present in the @Ackmaniac firmware?
```

---
## \#98 Posted by: JohnA Posted at: 2017-09-05T21:14:09.485Z Reads: 287

```
Finally got my focboxes working with the new tool. Only with the BLDC mode, not Foc (any ideas why?). Anyways first ride was very smooth, and the throttle curve behaved perfectly. That was until about half way through my ride on a a full speed pull (36mph) when I realized I didn't have any brakes... I have the gt2b controller so I know it didn't have interference, (also in rural area) so I carved hard to slow down, flipped the on-off switch a few times hoping the brakes would start working. Braced for impact and slid halfway through someones front yard.... no serious injuries, but I noticed on the ride home, any time I do a full throttle pull I loose braking until it slows down to half speed. The battery when this happens is about 36-38v (half empty), parameters are ({for each focbox}motor 100, -60 battery 40, -10 , erpm 60000,-60000, battery cut off start 34v)  so it must be a software issue? No fault codes when I plugged them in.. Beware New software in BLDC mode, may loose brakes.
```

---
## \#99 Posted by: Jinra Posted at: 2017-09-05T21:27:00.323Z Reads: 280

```
There's no benefit in limiting your eRPM ceiling like that, just leave it at 60k and call it a day
```

---
## \#100 Posted by: onepunchboard Posted at: 2017-09-05T22:33:41.525Z Reads: 278

```
in bldc mode focbox tends to hit absolute max amp so if u go like 140 it's better. but ultimate way to solve is either change gear ratio or use foc. 
try rebind controller it might solve
```

---
## \#101 Posted by: Eth67 Posted at: 2017-09-05T23:19:21.267Z Reads: 276

```
I just used the new tool, updated my VESC firmware and set up FOC for the first time. Kind of annoying having to go through the entire set up again but its fine. I also had the delay on the breaks and throttle mentioned earlier but its probably just that FOC will take a little for me to get used to.
My major problem though is that im no longer getting any data through the UART port. I made my own android app to send me data through a bluetooth module and arduino using RollingGeckos library but it literally just wont send data. I set the mode to PPM+UART and baud to 9600 and everything. Any ideas? about to do some investigating.
```

---
## \#102 Posted by: SeanHacker Posted at: 2017-09-06T01:46:43.390Z Reads: 280

```
@trampa and anyone using this... I tried searching the forums here and over at vesc-project but I haven't found any solutions. Every time I tried and to an FOC motor detect it says "R is 0. Please measure it first." And that's as far as I've gotten so far. Any ideas?
```

---
## \#103 Posted by: onepunchboard Posted at: 2017-09-06T02:08:16.515Z Reads: 266

```
re install the tool perhaps?
```

---
## \#104 Posted by: SeanHacker Posted at: 2017-09-06T02:57:55.916Z Reads: 270

```
Tried that. Didn't work. Wanted to try out FOC with this. Bummed...
```

---
## \#105 Posted by: chuttney1 Posted at: 2017-09-06T03:01:34.844Z Reads: 272

```
I don't think to reinstall the tool works. It's literally a standalone application on my Windows 10 pc right now. No executable file to install before using. Someone's gotta look at the code and see if any causes the "R is 0" error.
```

---
## \#106 Posted by: MrHappy Posted at: 2017-09-06T03:11:08.818Z Reads: 271

```
So you can use FOC without sensors on this version?
```

---
## \#107 Posted by: onepunchboard Posted at: 2017-09-06T03:13:03.088Z Reads: 265

```
it always has been. foc don't need sensor.
```

---
## \#108 Posted by: Titoxd10001 Posted at: 2017-09-06T03:14:46.707Z Reads: 267

```
Have the same issue with focbox "R is 0"
```

---
## \#109 Posted by: Jinra Posted at: 2017-09-06T03:40:44.533Z Reads: 268

```
i wonder if that's a focbox exclusive problem
```

---
## \#110 Posted by: Blasto Posted at: 2017-09-06T03:57:26.757Z Reads: 270

```
I got it to work

http://www.youtube.com/watch?v=xKVsb79Jxus
```

---
## \#111 Posted by: onepunchboard Posted at: 2017-09-06T04:16:01.494Z Reads: 265

```
good stuff! whoa 130k! im ganna try tmr 
so u didn't get that r is 0 thing? @Blasto
```

---
## \#112 Posted by: Blasto Posted at: 2017-09-06T04:21:07.721Z Reads: 275

```
[quote="onepunchboard, post:111, topic:32268"]
so u didn't get that r is 0 thing?
[/quote]

That's why i did the video. I didn't play with the settings.

I'm also learning here
```

---
## \#113 Posted by: Blasto Posted at: 2017-09-06T04:40:25.028Z Reads: 275

```
This time with a 6355 tb motor

http://www.youtube.com/watch?v=dB34Cc6ynf0
```

---
## \#114 Posted by: onepunchboard Posted at: 2017-09-06T04:45:57.093Z Reads: 270

```
tnx tnx. BTW what's that gigantic motor for? go cart?
```

---
## \#115 Posted by: Blasto Posted at: 2017-09-06T04:47:05.379Z Reads: 274

```
[quote="onepunchboard, post:114, topic:32268"]
BTW what's that gigantic motor for?
[/quote]

Breaking speed controllers 👹
```

---
## \#116 Posted by: oyta Posted at: 2017-09-06T05:08:52.746Z Reads: 271

```
[quote="Eth67, post:101, topic:32268"]
I made my own android app to send me data through a bluetooth module and arduino using RollingGeckos library but it literally just wont send data. I set the mode to PPM+UART and baud to 9600 and everything. Any ideas? about to do some investigating.
[/quote]

Maybe how you get the data has changed a bit? I see RollingGecko has started a VESC6-branch on his Git. Maybe you need that implemented.

I use PPM+UART with @rpasichnyk Bluetooth-thing and it works good.  @rpasichnyk has the interface changed?
```

---
## \#117 Posted by: Eboosted Posted at: 2017-09-06T06:02:17.611Z Reads: 266

```
How many ERPM did you reach with the Focbox and the 6355 239jv motor? Sorry if you said it on the video, I couldn't hear it

Are you planing to test the new limit on the road?
```

---
## \#118 Posted by: sl33py Posted at: 2017-09-06T06:27:26.789Z Reads: 264

```
[quote="chuttney1, post:87, topic:32268, full:true"]
I'm hoping this works out well for HW 4.7.
[/quote]

Works PERFECT on old hw 4.7 VESC's for me.  I built two boards for my brother w/ old VESC's - one single for his kids, and one dual for him.  Configured with the VESC Tool about a month or 2 now.  I'm a Beta guy and it was simple/easy and worked great!
```

---
## \#119 Posted by: xxlv Posted at: 2017-09-06T10:40:04.645Z Reads: 265

```
Maybe someone is interested, maybe not:

I made a VESC Tool fork without Trademark/Branding and without Warranty/Disclaimer checks and so on. Based on current V0.80

Download for Windows and Linux (i am working on macOs release): https://github.com/derlucas/esc_tool/releases/tag/v0.8

Maybe this helps other vendors of Vescs (even not licensed ones) to be able to use this software without issues.
Think of it as a "reference design" of the SW part.
```

---
## \#120 Posted by: Pimousse Posted at: 2017-09-06T12:06:23.591Z Reads: 256

```
Sorry, but what's the purpose ?
```

---
## \#121 Posted by: artteth Posted at: 2017-09-06T12:34:31.448Z Reads: 257

```
maybe someone can compile 2 and 3miliohm 412hardware and 3.27firmware to experiment with mini vescs ?
```

---
## \#122 Posted by: xxlv Posted at: 2017-09-06T12:47:26.501Z Reads: 261

```
Here i compiled the current 3.27 for 4.12 with 3mOhm and 2mOhm: 

https://trash.ctdo.de/b/59afee4b4db/vesc412_327.zip
```

---
## \#123 Posted by: artteth Posted at: 2017-09-06T12:48:09.538Z Reads: 258

```
wow
super fast
thanks
```

---
## \#124 Posted by: artteth Posted at: 2017-09-06T13:02:05.858Z Reads: 259

```
load new firmware
when in vesc tool it write 1,2 battery amps on bench supply i have 0.12 amps
maybe you wrong with the 0?
3miliohm = 0.003
```

---
## \#125 Posted by: xxlv Posted at: 2017-09-06T13:10:58.656Z Reads: 257

```
I am using this command: 

    make clean && make -j4 build_args="-DHW_VERSION_410 -DDISABLE_HW_LIMITS -DCURRENT_SHUNT_RES=0.0002"

Which is from build_all script with changed resistor value. I have not checked this obviously, but then i suspect even the original FW is not correct.
```

---
## \#126 Posted by: artteth Posted at: 2017-09-06T13:14:53.233Z Reads: 259

```
i dont now how to compile 
all i find is
 hwconf > hw_410 then i found shunt and instead of 0.001 i write 0.003 and then i don't know how to compile
i make all this in this http://www.chibios.org/dokuwiki/doku.php?id=chibios:product:chibistudio:start program
```

---
## \#127 Posted by: xxlv Posted at: 2017-09-06T13:15:41.225Z Reads: 253

```
Jep theems the build scripts are wrong. There are too many zeros. 

here the hopefully correct one:
https://trash.ctdo.de/b/59aff4f077c/vesc_hw412_fw327_0003_0002ohms.zip
```

---
## \#128 Posted by: artteth Posted at: 2017-09-06T13:16:08.096Z Reads: 252

```
[quote="xxlv, post:125, topic:32268"]
RES=0.0002
[/quote]


yes
too many
RES=0.0002
RES=0.002 needed
```

---
## \#129 Posted by: artteth Posted at: 2017-09-06T13:19:14.162Z Reads: 243

```
ok
test
now all ok
thanks
```

---
## \#130 Posted by: pshaw Posted at: 2017-09-06T14:03:36.620Z Reads: 245

```
Not sure if this has been answered already but I see some reports of the speed boost issue being eliminated with this new FW. For those of you that saw this, which esc are you using and what control mode (BLDC, FOC, etc.) ?

From everything I saw the speed boost is actually a HARDWARE issue which I wouldn't think could be solved via software. @Ackmaniac said it had to do with noise on the current sensor which causes duty cycle to ramp from 87% straight to 95% which would cause this boost of speed that can be unnerving st speed.
```

---
## \#131 Posted by: trampa Posted at: 2017-09-06T15:47:30.898Z Reads: 252

```
Hi Lucas, if you run a VESC-Tool Fork, why don't you open up your own tread fork. This one is about VESC-Tool and not about "your" ESC-Tool. 

If vendors of Hardware want to ship their VESC-Project derived ESCs, they can simply use the original FW and point to Benjamin's Website for software downloads and GITHub to stay on the legal side. 

Benjamin can even compile specially branded software for those who want to offer a custom (branded, custom FW) VESC-Tool. This way Vendors do not need to care about updates all the time. Pretty convenient!
Vendors who are thankful for thousands of fours of development work can even can even join a partner program in future.
This way customers can identify supportive vendors in future. For some this "feature" is quite important, simply because project support allows to develop more products (Software and Hardware). These items can be sold again. So it's probably in your interest to support R&D if you sell VESC-Project based Hardware.

Contributions to code, feedback and useful input is also very welcome! There is a forum for that:
http://www.vesc-project.com/forum

And if you feel that VESC-Tool is something that you appreciate: Invite Benjamin on a virtual blonde Beer - he deserves it! All cheers should go in his direction BTW. He is the Yoda of the Software!

Frank
```

---
## \#132 Posted by: Eth67 Posted at: 2017-09-06T17:42:25.799Z Reads: 249

```
See, thats what I thought. I tried the VESC6 branch but it didnt seem to work. However, i did implement it pretty sloppily as I was rushed. I'll try it again when i get home today and report back how it works.
If the other bluetooth apps are working still, i dont think anything could have changed too much. I could never get any of them to work with my bluetooth module though.
```

---
## \#133 Posted by: jujet Posted at: 2017-09-06T18:18:32.784Z Reads: 253

```
Great, I've done the update 4.12 hw and my remote stopped working for some reason. I can control the motor using my PC keyboard, but remote is dead. 

Any idea what might have happened? 

https://www.youtube.com/watch?v=KpvHMtBSZKU
```

---
## \#134 Posted by: trampa Posted at: 2017-09-06T19:03:17.896Z Reads: 249

```
How did you configure your PPM input signal? Via Wizard or manually? If your remote worked before, it should still work using Vesc-tool. Did you set a very low cut off voltage? This will stop the ESC from reacting.

Frank
```

---
## \#135 Posted by: trampa Posted at: 2017-09-06T20:48:09.941Z Reads: 252

```
A new Version is online! Some of the features requested are already implemented now. 
Throttle curves for brakes and acceleration is split now, fixed RT data time scale
and some other minor things....
VESC-Tool will tell you that there is an update. Latest Version now: V0.81

Frank
```

---
## \#136 Posted by: chuttney1 Posted at: 2017-09-06T21:30:35.205Z Reads: 253

```
What about the FOC function on HW4.7 with the new code?
```

---
## \#137 Posted by: onepunchboard Posted at: 2017-09-07T00:42:58.730Z Reads: 254

```
Well, focbox foc R is 0 Error!
```

---
## \#138 Posted by: onepunchboard Posted at: 2017-09-07T00:49:12.585Z Reads: 261

```
and it also loaded 4.10 instead of 4.12
```

---
## \#139 Posted by: Blasto Posted at: 2017-09-07T00:52:16.498Z Reads: 276

```
4.10 and 4.12 is the same hardware, just some slight routing changes
```

---
## \#141 Posted by: onepunchboard Posted at: 2017-09-07T01:01:36.600Z Reads: 289

```
Okay I debugged it. 
It seems like first detection stuck the motor for some reason, so it won't be able to detect from the first place!
U first need to set up the app, PPM for me. write default motor setting than run the motor a bit.
Than come back to motor detection! It works in both BLDC and FOC now,
Phew~

Update, FOC is detected but not working, for bizar reason it shorts the motor and making tiny sound. does not respond to ppm... well BLDC for a while I guess :cry:

Update2: A side from initial setup bug, I noticed there is bug with ppm setting. for FOC it short the motor when connected to Receiver, regardless the remote on or off. It's like a failsafe mod. I couldn't figure out what the cause. But it clearly works well on BLDC. Note: I plugged out receiver to prevent interference when setting FOC.

Notice that I use mac ver,(not official) FOCBOX, sk3 260kv 10s5a, with unloaded motor.

I tested with both 2.18 and Akman's 2.54, both works fine.
And to go back to old fmw, u upload from vesc tool and use old tool.

not too sure if the tool or fmw problem tho
```

---
## \#142 Posted by: trampa Posted at: 2017-09-07T06:20:09.208Z Reads: 280

```
Works. I ran a 4.7 for more than a year in FOC. 

Frank
```

---
## \#143 Posted by: bigben Posted at: 2017-09-07T08:03:39.538Z Reads: 280

```
So, as i'm having trouble now with the new vesc tool getting the sensor values on BLDC do I just ante up and try FOC?? My vescs are the last production enertion before VESC X..
```

---
## \#144 Posted by: WSB Posted at: 2017-09-07T08:05:33.024Z Reads: 273

```
Anybody tested updating a Maytech DRV cooker with this new VESC- Tool ?? 
And if so tested with FOC ?
```

---
## \#145 Posted by: rich Posted at: 2017-09-07T08:17:57.996Z Reads: 271

```
[quote="WSB, post:144, topic:32268, full:true"]
Anybody tested updating a Maytech DRV cooker with this new VESC- Tool ?? 
And if so tested with FOC ?
[/quote]


Yes, bootloader and FW upload works.... tested FOC with my maytech's :joy: everytime hitting the brake results in DRV fault and cut off on both V4.12, forget maytech and buy quality HW, with proper V4.12 FOC works like a charm.
```

---
## \#146 Posted by: trampa Posted at: 2017-09-07T09:31:38.870Z Reads: 259

```
Sensors work a lot better in FOC. Frank
```

---
## \#147 Posted by: WSB Posted at: 2017-09-07T11:30:57.491Z Reads: 257

```
Ok, thanks for the info. But you can at least use custom throttle curves and so on in BLDC mode?
I have a "beater" board with a maytech vesc and the "boost" is really pronounced here, so if this is gone with the tool that would be great. 
Agreed with quality HW in these things.
```

---
## \#148 Posted by: rich Posted at: 2017-09-07T11:34:57.150Z Reads: 255

```
The new FW works in BLDC mode with maytech , FOC not :wink:
```

---
## \#149 Posted by: trampa Posted at: 2017-09-07T11:57:21.495Z Reads: 250

```
It's always good to have FOCtimized HW.

Frank
```

---
## \#150 Posted by: pshaw Posted at: 2017-09-07T15:41:53.303Z Reads: 249

```
Any confirmation to the boost being gone even in hybrid mode? 

Again I thought soeed boost was a hardeare issue not software...
```

---
## \#151 Posted by: jujet Posted at: 2017-09-07T15:46:45.594Z Reads: 257

```
Frank, thanks for your reply

I configured PPM input signal using wizard. My remote did work before, I've been using this board for a week now with no problems. 

Voltage is set for a 10s battery. 

Here you can see some settings too

https://www.youtube.com/watch?v=lggyKaSRDC4

Thanks
```

---
## \#152 Posted by: Silverline Posted at: 2017-09-07T15:53:31.948Z Reads: 246

```
When you set it to "Current with no reverse with brake" Did you remember to hit the "Write app config. " ??
```

---
## \#153 Posted by: Jinra Posted at: 2017-09-07T16:07:59.546Z Reads: 246

```
Did you make sure to choose the app in "App Settings > General > App to use" **AND** choose a control type under "App settings > PPM > Control Type"?

Also whenever your motor doesn't move, avoid pull the throttle all the way like that, easy to way to blow your VESC and/or motor.
```

---
## \#154 Posted by: jujet Posted at: 2017-09-07T17:09:32.573Z Reads: 248

```
Yea, I think this was it. I wasn't changing this setting in both places. Now it works. Thanks guys !

If anyone else has this problem, this is how you set up your remote in the new vesc tool. 

https://www.youtube.com/watch?v=MNLDHgtGVZg
```

---
## \#155 Posted by: Vanarian Posted at: 2017-09-07T17:16:22.553Z Reads: 241

```
Off topic : is that your Z? That's one of my favorite cars period. Liked your post just for that haha
```

---
## \#156 Posted by: ThierryGTLTS Posted at: 2017-09-07T17:31:37.597Z Reads: 238

```
I don't see it's a new version, no visible difference in the name.

Can you explain how to download the new one, please?!

Thierry
```

---
## \#157 Posted by: jujet Posted at: 2017-09-07T17:46:42.324Z Reads: 234

```
Hahahah I wish mate :( oh how I wish this car would be mine
```

---
## \#159 Posted by: trampa Posted at: 2017-09-07T18:19:14.619Z Reads: 240

```
You go to vesc-project.com and choose the Vesc-Tool you want, then click on checkout. I you purchased a status version before, the update is free of charge. There is a "purchased files" section in your account. There you will find all files that you checked out recently.

Frank
```

---
## \#160 Posted by: Klattrup Posted at: 2017-09-07T18:38:57.179Z Reads: 243

```
Just did my first real run with the new firmware. I'm running an Trampa eMTB on 12S with 5800mAh LiPo battery on dual VESC 4.12's in BLDC mode. With the new firmware the boost is **definitely** gone or **very** subtle at most! I feel much safer now and can focus a bit less on the trigger! Awesome! :) I've never been able to start from standstil, but with the new firmware I can now start by pushing the board a bit forward while standing on it - this is very nice aswell.

Regarding the loss of brakes using BLDC I have not had this problem at any time on this run. I'll pay extra attention to this on my next many runs to make sure it's safe. :)

Thanks again Frank and Benjamin! :) :heart_eyes:

Log of the run for those interested: https://metr.at/r/x3iSO
```

---
## \#161 Posted by: The_Dude Posted at: 2017-09-07T21:39:01.627Z Reads: 232

```
12s?
10 char
```

---
## \#162 Posted by: SeanHacker Posted at: 2017-09-08T01:33:44.514Z Reads: 228

```
I'm still unable to get FOC detection working with my FOC boxes. Really wanted to give it a go. I'm still getting the "R is 0. Please measure it first." message every time I try.
```

---
## \#163 Posted by: onepunchboard Posted at: 2017-09-08T01:35:51.320Z Reads: 238

```
[quote="onepunchboard, post:141, topic:32268"]
Okay I debugged it. 
It seems like first detection stuck the motor for some reason, so it won't be able to detect from the first place!
U first need to set up the app, PPM for me. write default motor setting than run the motor a bit.
Than come back to motor detection! It works in both BLDC and FOC now,
Phew~

Update, FOC is detected but not working, for bizar reason it shorts the motor and making tiny sound. does not respond to ppm... well BLDC for a while I guess :cry:

Update2: A side from initial setup bug, I noticed there is bug with ppm setting. for FOC it short the motor when connected to Receiver, regardless the remote on or off. It's like a failsafe mod. I couldn't figure out what the cause. But it clearly works well on BLDC. Note: I plugged out receiver to prevent interference when setting FOC.

Notice that I use mac ver,(not official) FOCBOX, sk3 260kv 10s5a, with unloaded motor.

I tested with both 2.18 and Akman's 2.54, both works fine.
And to go back to old fmw, u upload from vesc tool and use old tool.

not too sure if the tool or fmw problem tho
[/quote]

Try this method, I didn't have good luck but maybe you can. @SeanHacker
```

---
## \#164 Posted by: SeanHacker Posted at: 2017-09-08T01:36:58.392Z Reads: 233

```
I'll give it a try right now. Just sitting here with my board trying to get it figured out. Thanks dude!
```

---
## \#165 Posted by: SeanHacker Posted at: 2017-09-08T01:50:31.293Z Reads: 231

```
I noticed something. I can get a good FOC detection when BLDC is selected in the General tab. But when I select FOC and try a detection is gives me the "R is 0. Please measure it first." message. @trampa Any ideas?

Also. The welcome screen that is only supposed to come up for the initial setup and agreements comes up every single time. Bugfix time. ;)
```

---
## \#166 Posted by: onepunchboard Posted at: 2017-09-08T02:05:51.254Z Reads: 228

```
I think it's more of fmw issue. btw did ur remote work? cuz mine didn't akman said if u use motor saturation to 1% it works but haven't try. and Im ganna stick to 2.54 for a while
```

---
## \#167 Posted by: trampa Posted at: 2017-09-08T07:30:47.079Z Reads: 230

```
Hi Vesc-Toolers, thx for your input! The best way to get issues sorted fast, is to summarize the problems you face on the http://www.vesc-project.com/forum

A you can see there is TODO list and Benjamin really works on that stuff in whenever there is a free minute, so that all your highly appreciated input can find its way into the tool. This way the tool will improve very fast and in a structured way.

http://www.vesc-project.com/node/110

THX again, Frank
```

---
## \#168 Posted by: ThierryGTLTS Posted at: 2017-09-08T10:36:18.128Z Reads: 225

```
Hi Frank,

Thanks for quick answer.

It's just sad that we canno't see any differences between the versions to download.

The name of the file is identical to the "old" one.

Please rename file before putting it to the website!

I'll be better for everybody.

Thierry
```

---
## \#169 Posted by: jujet Posted at: 2017-09-08T10:37:19.761Z Reads: 219

```
It's probably because you can only download the newest version.
```

---
## \#170 Posted by: trampa Posted at: 2017-09-08T10:39:06.929Z Reads: 222

```
Correct! You can't download the old versions. Lets see if Benjamin can ad the version number. I get the point.

Frank
```

---
## \#171 Posted by: Pimousse Posted at: 2017-09-08T12:50:00.552Z Reads: 221

```
Ben's TODO list is an awesome tool to show us how the development is going.
Thanks a lot for that !

I'm agree that the file name should contain the version number.
Mostly on the website because you don't know which version you are downloading (the only way to know is to install and go in "About" tab. Not so convenient ;) ).
```

---
## \#172 Posted by: MontPierre Posted at: 2017-09-08T17:38:08.581Z Reads: 226

```
Any luck @onepunchboard ? I have same problem with FOC set up, i got it to detect thanks to your tip but also in FOC motor does not respond to remote. 

I will be putting this up on VESC TOOL forum.
```

---
## \#173 Posted by: onepunchboard Posted at: 2017-09-08T17:56:26.014Z Reads: 222

```
well I think it's fmw problem. so I'm ganna wait till fix. have u try motor saturation?
```

---
## \#174 Posted by: MontPierre Posted at: 2017-09-08T17:58:01.996Z Reads: 220

```
Nope, sounds scary :) haha
```

---
## \#175 Posted by: onepunchboard Posted at: 2017-09-08T18:08:58.075Z Reads: 219

```
fair enough. yeah I wd wait. till then I'm using the old one
```

---
## \#176 Posted by: MontPierre Posted at: 2017-09-08T18:09:46.871Z Reads: 213

```
I'm happy with BLDC for now. Still waiting for sensored motors anyway :)
```

---
## \#177 Posted by: MontPierre Posted at: 2017-09-09T09:40:34.133Z Reads: 224

```
@onepunchboard I have sent a video of this issue to Benjamin and he will try to reproduce it with his 4.12 hardware - unfortunately doesn't have FocBox on hand to test with.  

Anyone else with " R is 0 " FOC detection error ? If so do you have FocBox or other Vesc?
```

---
## \#178 Posted by: Silverline Posted at: 2017-09-09T15:04:58.534Z Reads: 230

```
Just updated my focboxes to the new firmware. Now i got the same bug saying R is 0 in FOC mode :frowning:
Then i'm jumping back to bldc mode. But the detection allso fails now.

Any idear how i at least can run it in BLDC ?
Thanks

On another node. I was a silver member, but the VESC tool told me their was an update. But i could't find out how to download the new file. I tried downloading the file again under 'my purchase' but that seems to be the same 'old' file. So now i'm a free member, since i dont want to purchase it one more time, just for an updated. 
<img src="/uploads/db1493/original/3X/0/1/01c5e298a03ffb305c627cbc3ae3f71763db47cf.jpg" width="690" height="388">
```

---
## \#179 Posted by: trampa Posted at: 2017-09-09T15:26:49.268Z Reads: 225

```
The R=0 seams to be Enertion HW specific and it seams to depend on the HW revision. I'll chat about that with Ben.

Try to check out the silver again. It should be free of charge in that case. 

Frank

Ps.: Load defaults before you try again.
```

---
## \#180 Posted by: Silverline Posted at: 2017-09-09T15:34:58.628Z Reads: 220

```
Just flashed my focbox again. And with totally default settings, did a motor detection in BLDC, the motor spins up perfectly fine, but when the last part comes, where the motor needs to spin slowly, it`s just jitter like crazy.

I tried to raise the test value from default 5amp to 7amp, without any help :-(

Sk3 6364 / 190kv
10S
```

---
## \#181 Posted by: MontPierre Posted at: 2017-09-09T15:41:31.393Z Reads: 216

```
I did my BLD detection without problems and I also have 10s and Focbox - I did on both firmware versions. Only FOC gives R is 0 error.

Perhaps try wizard and if that fails "manually" in BLDC tab? Have you tried disconnecting and connecting back phase wires?
```

---
## \#182 Posted by: trampa Posted at: 2017-09-09T15:48:36.251Z Reads: 213

```
Drop your issue here and it will be seen.

http://www.vesc-project.com/forum/6

Frank
```

---
## \#183 Posted by: Silverline Posted at: 2017-09-09T15:49:17.268Z Reads: 220

```
I have both done it manually and via the wizzard. It`s a trampa board with 7 inch wheels. I have done the test with the belt on. I will now try without the belt...
```

---
## \#184 Posted by: Blasto Posted at: 2017-09-09T15:49:21.031Z Reads: 225

```
Hw specific issue... not

http://www.youtube.com/watch?v=UjH08vcAs7w

http://www.youtube.com/watch?v=qJ5WUA0bF7U

The tool im using https://www.dropbox.com/s/dw8bt7ehfhteao3/VESC_TOOL_works_W_FB.exe?dl=0
```

---
## \#185 Posted by: Silverline Posted at: 2017-09-09T15:57:02.679Z Reads: 220

```
It's Sound like this in bldc detection
https://www.youtube.com/watch?v=o0fDpFtkeys
```

---
## \#186 Posted by: Blasto Posted at: 2017-09-09T15:58:28.317Z Reads: 218

```
[quote="Silverline, post:185, topic:32268"]
Sound like this in bldc detection
[/quote]

Increase D to 0.1
```

---
## \#187 Posted by: onepunchboard Posted at: 2017-09-09T16:07:12.918Z Reads: 221

```
[quote="onepunchboard, post:141, topic:32268"]
Okay I debugged it. 
It seems like first detection stuck the motor for some reason, so it won't be able to detect from the first place!
U first need to set up the app, PPM for me. write default motor setting than run the motor a bit.
Than come back to motor detection! It works in both BLDC and FOC now,
Phew~

Update, FOC is detected but not working, for bizar reason it shorts the motor and making tiny sound. does not respond to ppm... well BLDC for a while I guess :cry:

Update2: A side from initial setup bug, I noticed there is bug with ppm setting. for FOC it short the motor when connected to Receiver, regardless the remote on or off. It's like a failsafe mod. I couldn't figure out what the cause. But it clearly works well on BLDC. Note: I plugged out receiver to prevent interference when setting FOC.

Notice that I use mac ver,(not official) FOCBOX, sk3 260kv 10s5a, with unloaded motor.

I tested with both 2.18 and Akman's 2.54, both works fine.
And to go back to old fmw, u upload from vesc tool and use old tool.

not too sure if the tool or fmw problem tho
[/quote]
try this. detection works but the ppm is not working
```

---
## \#188 Posted by: Silverline Posted at: 2017-09-09T16:30:28.780Z Reads: 213

```
Thanks guys...

But none of the things working..
ppm works, and i can spin up the motor with my remote.
But BLDC detection fails
No fault or faults in the terminal.

With original FW on focbox (2.18) motor detection in bldc works perfectly fine. Anybody knows where to downloade the original firmware, so i can use vesc-tool, to flash back old fw :-( There must be some sort of bug in the new firmware regarding focbox.
```

---
## \#189 Posted by: onepunchboard Posted at: 2017-09-09T16:53:18.098Z Reads: 214

```
go to enertion website and download the bldc tool. it should be included in the zip file
```

---
## \#190 Posted by: Silverline Posted at: 2017-09-09T16:56:17.522Z Reads: 212

```
Thanks... And i can flash that "old fw" via vesc-tool right ??
```

---
## \#191 Posted by: onepunchboard Posted at: 2017-09-09T17:08:01.004Z Reads: 207

```
yeap. 10 charac
```

---
## \#192 Posted by: MontPierre Posted at: 2017-09-09T17:08:18.227Z Reads: 206

```
yes you can. I would recommend @Ackmaniac software ( BLDC tool) and his custom firmware- a lot of his ideas are implemented in Vesc Tool.
```

---
## \#193 Posted by: Silverline Posted at: 2017-09-09T17:19:50.907Z Reads: 201

```
I would much much rather use the new firmware. It Works perfectly fine on my other board in FOC mode. But my trampa with two focboxes,  it seems to not like at all. Not even bldc.
```

---
## \#194 Posted by: chuttney1 Posted at: 2017-09-09T17:23:15.093Z Reads: 207

```
So I manage to update my HW4.7 to the newest firmware for VESC 6.0. I get the no control response for the PPM function after the update and found the solution is hitting the Input Setup Wizard. Was holding off on FOC due to past issues, but now helps me finally move from a dead stop with a 1.5 gear ratio on a single 149KV  motor and total weight of 78.18 Kg.
```

---
## \#195 Posted by: Silverline Posted at: 2017-09-09T17:35:03.684Z Reads: 209

```
Hey @Blasto Could you uploade your footage in higher resolution ? 240p is just not enough to se what values you came up with, in the end of the first movie ??


UPDATE. So my problem regarding to run the FOC motor detection (R = 0 bug) Seems to have something to do with the receiver. If i disconnect my receiver, i can now run the FOC motor detection without problems. But now as other also have mentioned i can not get my motor to run with my remote, i can se the ppm min / mid / max perfectly fine in the vesc-tool, but the motor is not running.
```

---
## \#196 Posted by: Blasto Posted at: 2017-09-09T18:23:48.264Z Reads: 206

```
I'll re-upload when i connect to wifi,

I set detection current to 6A, min erpm 500, min duty (D) 0.1
```

---
## \#197 Posted by: trampa Posted at: 2017-09-09T18:30:42.285Z Reads: 210

```
Maybe someone with R=0 problem could come to the Trampa Challenge, 23-24ths September at Hales Superbole.
3 Stages with live music, food and beer festival, big ramp flood light competition, official ATBA downhill race and an E-MTB challenge etc....

https://www.google.de/maps/place/Hales+Superbole/@53.0928545,-2.7464383,17z/data=!3m1!4b1!4m5!3m4!1s0x487aec0457aca98d:0xf7eee46fc0162795!8m2!3d53.0928545!4d-2.7442496?dcr=0

Benjamin will be there. Frank
```

---
## \#198 Posted by: MontPierre Posted at: 2017-09-09T18:43:58.002Z Reads: 207

```
@trampa  Frank, I would love to but it is a bit of a drive from London. 

Shall I copy below to VESC Tool forum so Benjamin can see it? Might be important to him. 

 [quote="Silverline, post:195, topic:32268"]
UPDATE. So my problem regarding to run the FOC motor detection (R = 0 bug) Seems to have something to do with the receiver. If i disconnect my receiver, i can now run the FOC motor detection without problems. But now as other also have mentioned i can not get my motor to run with my remote, i can se the ppm min / mid / max perfectly fine in the vesc-tool, but the motor is not running.
[/quote]
```

---
## \#199 Posted by: Silverline Posted at: 2017-09-09T18:47:42.219Z Reads: 204

```
He needs to fix it now, i would like to run my board Tomorrow 😂😂😎
```

---
## \#201 Posted by: MontPierre Posted at: 2017-09-09T19:06:51.660Z Reads: 201

```
Benjamin does not have a FocBox on hand to look into the issue -  hence the invite.
```

---
## \#202 Posted by: JohnnyMeduse Posted at: 2017-09-09T19:10:18.644Z Reads: 198

```
I do not believe it's a FocBox Issue, I Work with @Blasto, the Raptor was problematic at first but we go it to work, after reloading the old firmware and putting back the new one... Which make me believe that it probably a firmware related bug.
```

---
## \#203 Posted by: MontPierre Posted at: 2017-09-09T19:12:14.824Z Reads: 202

```
@JohnnyMeduse  I agree, it is for sure firmware but for Benjamin to see the issue in person, repeat it and debugg it he needs a FocBox :)
```

---
## \#204 Posted by: xxlv Posted at: 2017-09-09T19:18:52.791Z Reads: 207

```
Why should he care about Focbox? He is in cooperation with Trampa (official VESC HW)
```

---
## \#205 Posted by: Silverline Posted at: 2017-09-09T19:21:42.104Z Reads: 205

```
I find it pretty alarming that one of the most used 4,12 vesc, has not been tested. Is it even safe, to run the focbox on the new firmware at the moment ?
```

---
## \#206 Posted by: Ackmaniac Posted at: 2017-09-09T20:09:21.253Z Reads: 202

```
Is there anybody with a 4.12 Vesc (no focbox) where FOC is running with the new Firmware 3.27 or 3.28?
```

---
## \#207 Posted by: trampa Posted at: 2017-09-09T20:10:36.657Z Reads: 202

```
Yes, me for example. Running it since 12 months on a HW 4.12 and 4.7. FOC

Frank
```

---
## \#208 Posted by: trampa Posted at: 2017-09-09T20:11:58.725Z Reads: 204

```
There are a lot of guys from London coming. You could share a ride.

Frank
```

---
## \#209 Posted by: trampa Posted at: 2017-09-09T20:17:37.530Z Reads: 206

```
He needs multiple. All the different Versions. So I thought if guy owning such Hardware could come to Hales, that would be the way forward. Could also be fun.... 

Frank
```

---
## \#210 Posted by: Silverline Posted at: 2017-09-09T20:22:37.604Z Reads: 208

```
Yes...

On my other board i run this vesc in FOC mode without problem on the new vesc-tool http://www.hellray.de/shop/#!/Ab-sofort-als-ESK8-4-12-im-Shop-erhältlich-Available-now-as-ESK8-4-12-in-the-shop-Original-VESC-4-12-made-in-Germany-Ausverkauft-Sold-out/p/56097898/category=15255004

But not so nice on my two focboxes
```

---
## \#211 Posted by: Ackmaniac Posted at: 2017-09-09T20:33:05.823Z Reads: 200

```
Guess 3.27 isn't available since 12 months. 

Anybody else who runs it on 4.12 with the actual public VESC Tool?
```

---
## \#212 Posted by: TranxFu Posted at: 2017-09-09T20:52:54.748Z Reads: 204

```
So what I've read until now is that if you have a FOCBOX there is no reason to switch from ackmaniacs bldc tool ? 
Is there any reason at all ? I have not seen a clear answer yet if this actually makes a difference in riding performance or if its just a more user friendly UI ?
```

---
## \#213 Posted by: Ackmaniac Posted at: 2017-09-09T21:09:53.454Z Reads: 206

```
Well to be honest I don't want to Start a fight. I think it has a nice potential but it isn't there yet. But sooner or later it will be. It seems that most improvements are made in the sensorless startup. And Most work was definately done at Vesc Tool which is a great improvement for developers but for the average user the solution with so many tabs isn't really better than the old One. But people will get used to it.
But it is nice to see that Watt control is now the standard and that throttle curves are also included now. 
Sadly there isn't much more (yet).
```

---
## \#214 Posted by: Blasto Posted at: 2017-09-09T21:09:55.240Z Reads: 211

```
http://www.youtube.com/watch?v=IjMlsQlbz88

Same video but HD
```

---
## \#215 Posted by: JohnnyMeduse Posted at: 2017-09-10T03:06:26.878Z Reads: 213

```
[quote="Silverline, post:195, topic:32268"]
UPDATE. So my problem regarding to run the FOC motor detection (R = 0 bug) Seems to have something to do with the receiver. If i disconnect my receiver, i can now run the FOC motor detection without problems. But now as other also have mentioned i can not get my motor to run with my remote, i can se the ppm min / mid / max perfectly fine in the vesc-tool, but the motor is not running.
[/quote]

I think the problem might be related to the wizard... I got the same issue, so what i've done is:
1- reload the old @Ackmaniac 
2- try a motor detection in @Ackmaniac firmware 
3- go back to the new tool... close the remote and disconnect the can cable... like a noob on is first setup
4-don't give a shit about the wizard 
5-Upload the new firmware
6-Run Foc motor detection --- APPLY the Result--- 
7-Change my Motor setting 
8- change the app setting... and set the remote..
9- Done the same for the slave, except for the app where it is just send status over can
10- close everything... plug the CAN and power back everything
11-now it's working
12-drink a beer, cause that shit had take too much of my time
```

---
## \#216 Posted by: onepunchboard Posted at: 2017-09-10T03:12:11.146Z Reads: 203

```
I get detection but soon as plug the receiver back motor locks.  still would wait for fmw update｢(ﾟﾍﾟ)
```

---
## \#217 Posted by: JohnnyMeduse Posted at: 2017-09-10T03:13:41.522Z Reads: 200

```
did you use the wizard the very first time you plug it in ?
```

---
## \#218 Posted by: onepunchboard Posted at: 2017-09-10T03:17:33.642Z Reads: 197

```
yeap. but after that I change to old fmw couple times and try without wizard. like I said I can do detection. there is interference with receiver
```

---
## \#219 Posted by: Silverline Posted at: 2017-09-10T04:53:20.385Z Reads: 199

```
Same here....
I was hoping i could run my board today on the new firmware. I guess not...
```

---
## \#220 Posted by: bigben Posted at: 2017-09-10T07:13:18.117Z Reads: 197

```
I've set my two enertion vescs up with the new tool on FOC. (compiled mac latest version)
I did this because the new tool was having trouble with detecting the hall sensors.
They so far have worked flawlessly. Weather has been terrible though so haven't had the chance to put too many miles on them. 5 miles?

Mini remote and receiver.
Split receiver signal, both VESCs set up as single drive.
```

---
## \#221 Posted by: trampa Posted at: 2017-09-10T09:29:52.713Z Reads: 201

```
[quote="Ackmaniac, post:213, topic:32268"]
But it is nice to see that Watt control is now the standard and that throttle curves are also included now.
[/quote]

No Watt control in VESC-Tool. You can set a watt limit.

Frank
```

---
## \#222 Posted by: Ackmaniac Posted at: 2017-09-10T09:57:35.546Z Reads: 198

```
Current Control in VESC-Tool does the exactly the same as Watt Control. 
It's implemented in a more generic (smarter) way but the result is the same. 
So only difference is that it is named Current Control now.
Even the watt limits work in exactly the same way.

But i don't understand why you try to deny that.
```

---
## \#223 Posted by: Silverline Posted at: 2017-09-10T10:08:52.174Z Reads: 197

```
So is Benjamin going to have a focbox Soon 😎
```

---
## \#224 Posted by: Pimousse Posted at: 2017-09-10T10:54:59.549Z Reads: 196

```
@trampa, vesc-project.com seems to be down on my side.
Is it just me or something is really going wrong ?
```

---
## \#225 Posted by: Surfer Posted at: 2017-09-10T10:58:41.959Z Reads: 191

```
Down here too....
```

---
## \#226 Posted by: NAF Posted at: 2017-09-10T11:17:38.171Z Reads: 192

```
Me.. FOC runs awesome. A lot better than previous.
```

---
## \#227 Posted by: Cobber Posted at: 2017-09-10T11:23:04.903Z Reads: 196

```
not likely, I doubt loopy will send him one...
```

---
## \#228 Posted by: MontPierre Posted at: 2017-09-10T12:41:01.950Z Reads: 212

```
@onloop any chance of a spare FocBox for Benjamin for testing, debug and fix of "R is 0" error on the Focboxes?

Looks like no one in the area has FocBox to lend :frowning: 

Just an idea ;) 

[quote="trampa, post:197, topic:32268, full:true"]
Maybe someone with R=0 problem could come to the Trampa Challenge, 23-24ths September at Hales Superbole.
3 Stages with live music, food and beer festival, big ramp flood light competition, official ATBA downhill race and an E-MTB challenge etc....

&lt;img src="https://maps.googleapis.com/maps/api/staticmap?maptype=roadmap&amp;amp;center=53.0928545,-2.7464383&amp;amp;zoom=17&amp;amp;size=690x400&amp;amp;sensor=false" width="690" height="400"&gt;

Benjamin will be there. Frank
[/quote]
```

---
## \#229 Posted by: Ackmaniac Posted at: 2017-09-10T13:58:59.517Z Reads: 211

```
Think the problem is in the initialization of the DRV.

First problem with the wizard is that it set's the actual motor type to FOC. And FOC doesn't run so it can't identify the resistance.

Without the wizzard the actual mode is BLDC which let's the motor spin. (So for the moment forget the wizzard)

I was wondering that i got FOC running when FOC was active and i measured the flux linkage again. Afterwards FOC worked. So i checked the code where the difference is but could not find anything that could cause it.

Finally i found the reason why it works with flux linkage. Because during the detection the motor is set to BLDC mode, starts spinning and then switches back to FOC.

But the big difference is that when the motor is still spinning while it switches back to FOC it works.

So i tried by spinning the motor in BLDC and while it is still spinning i switched to FOC and surprise. It works as well.

So i guess there is a problem in the initialization of the DRV8302. (this code has changed)
```

---
## \#230 Posted by: ThierryGTLTS Posted at: 2017-09-10T14:17:29.955Z Reads: 207

```
I use HW4.12, FW3.27 and FOC with no problems.

But I don't use the wizzard (I hate those things because I don't see what it does).

Detection works very quickly, but the R and L are not what I measure with a good LCR meter @ 10kHz, and what I measure are the same values that the manufacturer gives.

It runs well, even at low current and very low speed (Motor with Hall sensors), but it makes noise at more than 15000 ERPM.

Have a Nice W-E.

Thierry
```

---
## \#231 Posted by: Silverline Posted at: 2017-09-10T14:20:26.204Z Reads: 201

```
But is it a focbox ?

I also have another vesc from esk8.de that is working perfect in FOC mode. But my two focboxes dosn't
```

---
## \#232 Posted by: ThierryGTLTS Posted at: 2017-09-10T14:30:21.315Z Reads: 206

```
Yes it's not a FOCBOX!

VESC Project is down and even the Google cache of the 8th of september does not work.

Strange.
```

---
## \#233 Posted by: Silverline Posted at: 2017-09-10T16:19:34.849Z Reads: 204

```
You are right. Maybe it`s an focbox update on the way :-P
```

---
## \#234 Posted by: MontPierre Posted at: 2017-09-10T16:25:08.145Z Reads: 212

```
@trampa Frank - would you be able to pass this on to Benjamin? This looks like very important debug by @Ackmaniac.

Unfortunately vesc tool forum seems to be down so we can't post it there ...   


[quote="Ackmaniac, post:229, topic:32268, full:true"]
Think the problem is in the initialization of the DRV.

First problem with the wizard is that it set's the actual motor type to FOC. And FOC doesn't run so it can't identify the resistance.

Without the wizzard the actual mode is BLDC which let's the motor spin. (So for the moment forget the wizzard)

I was wondering that i got FOC running when FOC was active and i measured the flux linkage again. Afterwards FOC worked. So i checked the code where the difference is but could not find anything that could cause it.

Finally i found the reason why it works with flux linkage. Because during the detection the motor is set to BLDC mode, starts spinning and then switches back to FOC.

But the big difference is that when the motor is still spinning while it switches back to FOC it works.

So i tried by spinning the motor in BLDC and while it is still spinning i switched to FOC and surprise. It works as well.

So i guess there is a problem in the initialization of the DRV8302. (this code has changed)
[/quote]
```

---
## \#235 Posted by: trampa Posted at: 2017-09-10T16:38:30.537Z Reads: 201

```
I mailed Benjamin already and send him a text message. Server should be up and running soon.

Frank
```

---
## \#236 Posted by: chinzw Posted at: 2017-09-11T17:26:52.639Z Reads: 198

```
Im running the latest fw with 4.12 torqueboards, i had the bldc detection issue. What i did was run the motor detection wizzard and that works. But it wont work from the regular UI, just from the wizzard.
```

---
## \#237 Posted by: onepunchboard Posted at: 2017-09-12T16:23:25.068Z Reads: 199

```
focbox foc update.

I had time to use new 0.81 tool. 
disconnect receiver, write bldc config, go to FOC config, flying pass.
soon as i plug receiver, (I didnt even select current brake option) motor high pitched, shorted.
no response from throttle. 
try with motor saturation, but does nothing.

What did I learn: bug seems to do with sending packets from receiver to the vesc. In vesc tool when I try to control with keyboard, it acts to same.

still not working for me going back to 2.54
```

---
## \#238 Posted by: MontPierre Posted at: 2017-09-12T16:49:36.669Z Reads: 199

```
Great debugging! Any chance you can post it on VESC TOOL forum? Benjamin doesn't check here, he only looks at topics on that Forum.

@trampa
```

---
## \#239 Posted by: onepunchboard Posted at: 2017-09-12T17:01:37.413Z Reads: 200

```
i did it already cheers!
```

---
## \#240 Posted by: trampa Posted at: 2017-09-12T19:17:00.371Z Reads: 206

```
The latest FocBox (shipped with R2) worked fine with Vesc-tool. @Jamy tried it. I don't know what the difference in the HW is. A bit strange....

Did I get you right, that keyboard control worked and as soon as you plug the receiver, things go funny.

I think there is a solution, just needs some attention. Would be great to get hold of one, so Ben can test things.

Frank
```

---
## \#241 Posted by: onepunchboard Posted at: 2017-09-12T19:32:00.692Z Reads: 203

```
tnks for reply. 
well let me make it clear.

so no receiver plugged. and try to use keyboard. the keyboard and heart glows to green on vesc tool. heart button is sending live packets to vesc. this cause motor to short. if i turn this off, motor no longer short however I cannot spind the motor anymore.

it could be the motor. may be picky with new fmw. im using sk3 260kv. torquboard motor seems work fine
```

---
## \#242 Posted by: trampa Posted at: 2017-09-12T19:38:20.061Z Reads: 198

```
So the lower KV torque boards motor works with FocBox seamless?
```

---
## \#243 Posted by: onepunchboard Posted at: 2017-09-12T19:42:35.484Z Reads: 202

```
srry i got u wrong. so all the video ive seen working focbox with new fmw FOC mode has lower kv. @Blasto used both R2 and torque board 190kv(i think) 
im not sure i dont have lower kv motor on me.
```

---
## \#244 Posted by: Blasto Posted at: 2017-09-12T19:45:55.479Z Reads: 200

```
the TB motor i had was 230Kv, the massive 9060 motor was also 230Kv, R2 is 85Kv (i think?)
```

---
## \#245 Posted by: trampa Posted at: 2017-09-12T19:49:11.337Z Reads: 202

```
Low KV is always easier to track. 
Are we only talking FOC, or does that funny behavior also occur in BLDC @onepunchboard? 

Frank
```

---
## \#246 Posted by: onepunchboard Posted at: 2017-09-12T19:49:53.189Z Reads: 201

```
BLDC works Fabulous. only Funky in FOC
```

---
## \#247 Posted by: trampa Posted at: 2017-09-12T19:56:28.084Z Reads: 206

```
We are talking about the funky FocBox FOC issue.
I hope there is a solution and it won't take to long. The FOC-code is the one that got most improvements. 

Frank
```

---
## \#248 Posted by: Silverline Posted at: 2017-09-12T20:14:58.626Z Reads: 207

```
I stil think bldc on focbox works a lot better on the new fw. Vs 2.18
So can't wait to try FOC mode :slight_smile:
```

---
## \#249 Posted by: Ackmaniac Posted at: 2017-09-13T00:40:12.672Z Reads: 203

```
In BLDC mode my Motors make a Full brake at low speed (15 km/h) and mid brake with the new Firmware and sensorless 6355. 
And it always takes a short moment before the Motors do a full brake. So you can't really tell when it happens which makes it a bit scary.
Can somebody else verify this behavior?
```

---
## \#250 Posted by: onepunchboard Posted at: 2017-09-13T01:37:52.418Z Reads: 206

```
isnt there ramping delay in ppm tap?
```

---
## \#251 Posted by: SeanHacker Posted at: 2017-09-13T02:43:22.053Z Reads: 201

```
Yep. Same thing here. In BLDC mode braking is fucking scary. There's a pause before it kicks in and when it does if you're full brake on accident things get pretty hairy. I switched back to your firmware immediately.

Dual sensored 6355's.
```

---
## \#252 Posted by: SeanHacker Posted at: 2017-09-13T02:47:39.028Z Reads: 201

```
I've messed with it. But that's not the problem here I don't think. No matter how its set there's a pause. If I full brake it doesn't start braking until after the pause. And then it will brake hard or soft depending on where you finger is on the throttle.
```

---
## \#253 Posted by: crustyxpunk Posted at: 2017-09-13T07:22:09.559Z Reads: 199

```
Do you have a download link available yet?
```

---
## \#254 Posted by: rpasichnyk Posted at: 2017-09-13T07:35:29.800Z Reads: 199

```
Yes http://www.electric-skateboard.builders/t/vesc-6-released-and-the-forum-is-open/32265/22?u=rpasichnyk
```

---
## \#255 Posted by: crustyxpunk Posted at: 2017-09-13T08:01:01.231Z Reads: 203

```
Awesome, Thank you!
```

---
## \#256 Posted by: crustyxpunk Posted at: 2017-09-13T23:24:37.355Z Reads: 208

```
Downloaded @rpasichnyk Mac OS port and got everything working great! currently running a Torqueboards 6374 190kv motor, connected to a Torque Boards VESC powered by a 12s4p battery.  Throttle response is definitely smoother than the previous FW. No more asshole puckering when the random throttle "boost" kicks in.  Apart from that the execution of the tool itself is great and makes things way easier than BLDC tool. Thank you Benjamin, @trampa and @rpasichnyk !!
```

---
## \#257 Posted by: trampa Posted at: 2017-09-14T08:15:11.480Z Reads: 211

```
You can change the positive and negative ramping time in the PPM tab. Easy! You should try it with a slight delay and work yourself down in value until you feel that its comfortable.

Frank
```

---
## \#258 Posted by: bevilacqua Posted at: 2017-09-14T20:42:03.096Z Reads: 209

```
Hi, I updated both of my mytech VESCS (HW 4.12) to the latest 3.28 Firmware. 

Configuration seemed to work just fine, motor values detection etc, but suddenly after the latest vesc tool crashed (Installed today 14.9.17) both of my vesc's won't get recognized by my PC: 
-Blue light On - No red light // No red blinking light

does anyone have the same issue? any solutions? do I need to completely flash my Vesc's? 
" https://www.youtube.com/watch?v=17CSl1iXYE8 "

thank you in advance
```

---
## \#259 Posted by: Silverline Posted at: 2017-09-15T22:04:20.980Z Reads: 205

```
So any news regarding FOC on focbox ?
```

---
## \#260 Posted by: Eboosted Posted at: 2017-09-16T06:34:46.470Z Reads: 204

```
On the legacy BLDC tool I had these settings on my dual VESC setup:

Motor max 65A
Montir min -65A
Battery max 40A
Battery min - 8A

On the new firmware I used the same settings and the braking force at high speed has been drastically reduced. 

Has anything changed in the way the new tool calculate these settings?
```

---
## \#261 Posted by: rich Posted at: 2017-09-16T10:28:38.330Z Reads: 204

```
[quote="bevilacqua, post:258, topic:32268"]
but suddenly after the latest vesc tool crashed (Installed today 14.9.17) both of my vesc's won't get recognized by my PC: 
-Blue light On - No red light // No red blinking light
[/quote]

Blue/white light on is normal, with the new FW there is no more red blinking when switching on. If you use antivirus software, deactivate it before opening VESC-Tool, this is what I have to do to run it.
```

---
## \#262 Posted by: trampa Posted at: 2017-09-16T11:11:42.919Z Reads: 199

```
Not yet, Benjamin needs a FocBox to sort that out.
Hard to say where the issue is without the hardware for testing. 

Frank
```

---
## \#263 Posted by: Silverline Posted at: 2017-09-16T11:17:33.488Z Reads: 199

```
So is anybody sending him one ?
```

---
## \#264 Posted by: trampa Posted at: 2017-09-16T12:05:47.819Z Reads: 201

```
Don't know? We hoped someone wold come to hales, but sadly the event is canceled. If there is someone with a Focbox, especially the older ones, wanting to lend him one, that would be great. I don't know if all versions react the same. So he probably needs one from different batches. Or maybe there is someone who could allow a tunnel to the computer, so he can work on it real time from Sweden.

Frank
```

---
## \#265 Posted by: Silverline Posted at: 2017-09-16T12:19:12.881Z Reads: 204

```
I have one "backup focbox" I can loan him if it is?It`s from one of the newest batches (with the wrong labeling on top) I´m from Denmark, so not a very long way.
My focboxes in my trampa, is screaming FOC at me every time i ride :-P
```

---
## \#266 Posted by: Jinra Posted at: 2017-09-16T15:09:09.746Z Reads: 204

```
I have the same issue on my thread, so far no solution i can see. My guess is that it's using the battery regen braking current even at non regen speeds. I haven't tried it, but i think raising battery regen would help with braking, but, obviously, put the cells at risk.

The reason i think this is because on 2.18 when i hit regen speeds, the braking felt similar to how it feels most of the time in 3.28
```

---
## \#267 Posted by: Jinra Posted at: 2017-09-16T15:10:07.559Z Reads: 199

```
I had the r is 0 bug on my chaka vesc. I fixed it by running detection in bldc then running it on FOC again. No need to change control mode or even write any settings, just do the detection
```

---
## \#268 Posted by: BigBoyToys Posted at: 2017-09-16T16:19:45.863Z Reads: 199

```
I have FOC box's and VESC X's. Ive tried 3.26 and a both without issue.  Also tried it on a TB VESC  at 10S with FOC and lost a DRV.
```

---
## \#269 Posted by: Eboosted Posted at: 2017-09-16T16:22:43.939Z Reads: 201

```
I'm gonna raise the regen from -40A to -50A hope it helps a little with braking force at high speeds, it's impossible to ride this way I feel pretty unsafe, I'll also reduce the battery min from -10A to -8A as braking force at low speeds is too agressive
```

---
## \#270 Posted by: Jinra Posted at: 2017-09-16T16:27:20.400Z Reads: 200

```
I think you got that backwards. I'm saying your braking at high speeds is weak because it's using your battery regen current, so raise that and it should respond better. That's my theory anyway.
```

---
## \#271 Posted by: Eboosted Posted at: 2017-09-16T18:31:23.649Z Reads: 191

```
I'll do that later today, have you got the bluetooth module working on the new firmware in order to modify settings?
```

---
## \#272 Posted by: trampa Posted at: 2017-09-16T18:42:18.575Z Reads: 191

```
That's correct! Battery regen is the value that will adjust your braking performance, as long as motor regen isn't lower than battery regen. -30A is about right to get a good performance. You can set both values (motor/battery) same. Brakes get harder the slower you get. That's the same as you experience in your car - same braking force against less kinetic energy. 

Frank
```

---
## \#273 Posted by: Jinra Posted at: 2017-09-16T18:44:12.830Z Reads: 189

```
Thanks for the confirmation Frank. Could you elaborate on why there is such a dramatic change in braking performance from 2.18 to 3.28? with dual VESCs and -8a battery regen on each VESC and -70A motor min, I had great braking response when below regen speeds.
```

---
## \#274 Posted by: trampa Posted at: 2017-09-16T18:58:19.602Z Reads: 189

```
What do you mean by "below regen speed". You will always push currents towards the battery. You brake, you generate. Are you comparing BLDC 2.18 vs FOC 3.28?

Frank
```

---
## \#275 Posted by: Jinra Posted at: 2017-09-16T19:00:26.741Z Reads: 196

```
You can't regen while braking if the generated voltage by the generator (motor) is lower than the battery's voltage. This should mean that you have to be going full speed or faster in order to regen brake.

This is at least my understanding from reading up on regenerative braking.

If you push current toward's a system with higher voltage, it should just be dissipated as heat anyway

Source: https://www.roboteq.com/index.php/applications/100-how-to/160-understanding-regeneration

> A motor behaves as motor and as generator at the same time. In fact while a motor is 'motoring', that is doing mechanical work, it generates CEMF acting as generator, although the CEMF is lower than the battery voltage so the motor acts as a load and absorbs current.

> In certain situations the CEMF may overcome the battery, in which case the generator component becomes dominant; the motor acts as a generator inverting the direction of its current and forcing it into the battery.
```

---
## \#276 Posted by: trampa Posted at: 2017-09-16T19:06:07.147Z Reads: 194

```
Bit that is at really low speeds only. 

Frank
```

---
## \#277 Posted by: Jinra Posted at: 2017-09-16T19:07:45.640Z Reads: 192

```
why would it be at low speeds? If you have a 40v battery, you need BEMF/CEMF to generate over 40v for it to charge the battery. The only way it generates that much voltage is for it to be traveling faster than full throttle speed.
```

---
## \#278 Posted by: JTAG Posted at: 2017-09-16T20:34:47.999Z Reads: 190

```
I am afraid you are not entirely right. You can see the VESC as a synchronous multi quadrant power supply, it can step down the voltage (from a high battery voltage to a lower motor voltage, normal use)  AND can boost the voltage (from the lower voltage motor to the higher voltage battery, regenerative braking).

So when the VESC reads negative motor / battery currents it does regeneratively brakes and charges the battery.
```

---
## \#279 Posted by: Jinra Posted at: 2017-09-16T20:37:24.872Z Reads: 186

```
thanks for your input! I've been trying to find articles online about this and couldn't source any good information besides the one I posted.

If this is the case, wouldn't this bode even worse for f/w3.28? It means at any given speed a battery min value of -40 has the potential to inject 40 amps of charging current to the battery.
```

---
## \#280 Posted by: JTAG Posted at: 2017-09-16T20:40:48.632Z Reads: 181

```
Sorry, I havent keep track of your issue, I just replied on the regenerative part :stuck_out_tongue:.
```

---
## \#281 Posted by: trampa Posted at: 2017-09-16T20:48:23.316Z Reads: 183

```
Right, that's why an adjustable battery min value exists. As I explained, you max braking performances is dependent on your battery. This is why you go for 3P+ setups and strong cells. A high discharge rated cell usually also performs better at charging. The dilemma of small packs at low voltage is capability to push/swallow Amps. Electric cars run on much higher voltage and have a bigger battery to cope with that. In consequence you can use lower discharge rated cells. Scaling things down to skate size is a challenge and you want to use the best cells possible. Long downhill/uphill sessions may be problematic, especially with low parallel cell count. You could strap an oven plate to your board and fry eggs while doing extended downhill sessions.

Frank
```

---
## \#282 Posted by: Jinra Posted at: 2017-09-16T20:51:07.966Z Reads: 187

```
I get the relationship between regen current and cells. My question is two fold.

1. How is a recommended charge current of 40 amps for a 3P setup okay, if each cell has a rated max charge current of 4 amps. This is 13 amps per cell at the highest regen!

2. Why has the behavior changed from 2.18 and the brakes are now weaker at the same value. Was 2.18 just better in this sense and 3.28 just a downgrade?
```

---
## \#283 Posted by: trampa Posted at: 2017-09-16T20:57:48.733Z Reads: 194

```
Has nothing to do with the version of the software. Conservation of energy again....
No software can dissipate energy into the universe.

Your cells can cope with higher amps, as long as its not a continuous flow for a long period. The longer you abuse them the shorter the life cycle. I rather have a strong brake than super healthy cells. Brakes are safety, healthy cells a bonus. 

If you face very long 40A hills, better upgrade your pack to 6-8P. But: Full is Full and that's the point where you should go up the hill again.



Frank
```

---
## \#284 Posted by: Jinra Posted at: 2017-09-16T21:01:30.356Z Reads: 193

```
I think you're missing my question again. You can have strong brakes at speed AND healthy cells on 2.18 as the braking was great with motor min -60 and battery min -8. On 3.28 it's weak 80% of the time, and it's only strong when you're going jogging speed.
```

---
## \#285 Posted by: Ackmaniac Posted at: 2017-09-17T00:35:56.851Z Reads: 196

```
Found the problem. Benjamin uses the basic of watt control also for braking. That means when he identifies that with the actual duty cycle the full motor brake amps (motor min) can't be reached he reduces the maximum brake current at the motor. 

    - 70A motor min
    -  8A batter min
    - 50% duty cylce
    A maximum of only -16A is allowed (8A battery min / 0,50 duty cycle)
    So for example at 75% brake you can only reach -12A at the motor.

Once it reaches lower duty cycle the brake power increases. That explains a lot and is the root cause for the strange braking behavior. 

This results in a non linear braking which really isn't a good idea. So only chance to have a good brake behavior is to set the battery min ridiculous high which is a bad idea as well.
```

---
## \#286 Posted by: Jinra Posted at: 2017-09-17T01:20:52.401Z Reads: 192

```
YES thank you @Ackmaniac Glad we got an explanation for this.. Non linear braking is exactly what I'm experiencing. Hopefully Benjamin can acknowledge this and fix it in the next version.

@trampa

BTW @Eboosted I tried it out and can confirm setting battery regen ridiculously high (-40) will bring brakes back to normal, though a bit unsafe...
```

---
## \#287 Posted by: Titoxd10001 Posted at: 2017-09-17T01:59:46.965Z Reads: 198

```
I did feel like brakes were weaker and almost got run over by a car by a couple of inches. In part because couldn't stop in time even though I had higher brake settings than before. Switching back to extended bldc tool
```

---
## \#288 Posted by: Jinra Posted at: 2017-09-17T02:00:21.451Z Reads: 192

```
yea I'm thinking of switching back to 2.18 on bldc too

@Titoxd10001 How do you even downgrade? @Ackmaniac's BLDC tool won't even connect. Do you flash his f/w from Vesc tool?
```

---
## \#289 Posted by: Titoxd10001 Posted at: 2017-09-17T04:24:35.082Z Reads: 190

```
I haven't done it yet but from what others say you can upload other firmwares from vesc-tool
```

---
## \#290 Posted by: Eboosted Posted at: 2017-09-17T04:41:51.191Z Reads: 194

```
[quote="Jinra, post:286, topic:32268"]
BTW @Eboosted I tried it out and can confirm setting battery regen ridiculously high (-40) will bring brakes back to normal, though a bit unsafe...
[/quote]

I just updated my current settings, I went from battery min -10A to -20A and motor min from -40A to -30A then went for a test ride, the brakes are much much better now, the braking force is much more linear, however the brakes in FW2.18 were better, not by much though.

I'm gonna try motor min -40A again with -30A for battery min, I'm kinda concerned about those numbers though, they seem to be dangerous for the battery too much current flowing back, I don't understand why FW2.18 had so much braking force with such a low value for battery min such as -8A

What I really need now is a bluetooth app to change the crrent values from the phone, disassembling the enclosure everytime I want to make a change is getting a PIA, has anyone got a working bluetooth app?, I was able to connect, read battery voltage and read values but not change settings.
```

---
## \#291 Posted by: Jinra Posted at: 2017-09-17T04:45:53.468Z Reads: 188

```
Check out the reply i tagged you in. Ackmaniac explained the bug in 3.28
```

---
## \#292 Posted by: Eboosted Posted at: 2017-09-17T04:53:48.909Z Reads: 181

```
I just read it, well doesn't seem to be a bug, just a different way to calculate maximum braking force in amps, so if I increase battery min to -30A and apply 50% DC:

- 40A motor min
- 20A battery min
- 50% DC

-20A battery min / 0.5 DC = -40A at the motor which is the same value I had with FW2.18

I'll try that tomorrow
```

---
## \#293 Posted by: Jinra Posted at: 2017-09-17T05:03:39.308Z Reads: 179

```
Seems like a bug with the calculation to me, As ackmaniac said you'll either have weak brakes or unsafe regen values.
```

---
## \#294 Posted by: trampa Posted at: 2017-09-17T13:52:56.188Z Reads: 175

```
No, that's no bug, that's physics and limits of the cells we can buy today. Conservation of energy is a fact.

Frank
```

---
## \#295 Posted by: JTAG Posted at: 2017-09-17T15:48:54.635Z Reads: 171

```
It is not a bug, and therefore can't be fixed in firmware. It is a wrong configuration / setup.
```

---
## \#296 Posted by: Jinra Posted at: 2017-09-17T15:55:06.930Z Reads: 184

```
if it's not a bug then i guess 2.18/2.54 is just a superior version for me
```

---
## \#297 Posted by: bevilacqua Posted at: 2017-09-17T16:03:22.810Z Reads: 187

```
It indeed was a missing bootloader, I followed Vedder‘s instructions and now both Vescs work again. Nevertheless thank you for your help :)
```

---
## \#298 Posted by: Ackmaniac Posted at: 2017-09-17T18:27:09.622Z Reads: 194

```
Well it depends what you want. I just want a stable brake. Means when i brake gentle at high speed (e.g 25% brake) i want the same brake torque when i brake with 25% at mid and low speed.

Currently the brake is only constant at very low speeds. 

This example below shows the diffrence in brake power at different speeds (duty cycle) at 25% brake with a setting of -70A motor min and -10A battery min. 

<img src="/uploads/db1493/original/3X/e/c/ec37c664a7af0be0cefbe0e4790ca40012cd0aca.png" width="266" height="141">

It is not a bug because it is implemented in a nice way so it was clearly Benjamin's intention to do so. But if you ask me it is simply the wrong way to handle the brake current because it results in a unpredictable braking behavior.
And the only way to avoid this in the 3.28 firmware is by increasing the battery min value to very high values (which most of our battery's can't handle)
And this is fixable in the firmware.
```

---
## \#299 Posted by: BigBoyToys Posted at: 2017-09-17T19:39:26.275Z Reads: 188

```
Ive gone back and forth a couple times. Just flash 2.18/2.54 FW using the VESC Tool. It finishes, disconnects, then reconnects and gives the outdated firmware message at which point you can swap back and connect to to BLDC tool.
```

---
## \#300 Posted by: Vanarian Posted at: 2017-09-17T20:24:57.631Z Reads: 185

```
@Ackmaniac @Jinra thank you guys for pointing this issue. 

Considering I can't jump off my skates in case some braking goes wrong I'd risk hard face-plant. That's not nice despite all the big work done. 

@trampa Frank could you please up the issue toward Benjamin so he can solve it on next versions? Linear throttle and braking inputs mean everything for many including me.
```

---
## \#301 Posted by: Ackmaniac Posted at: 2017-09-17T20:31:58.392Z Reads: 177

```
Linear brake is great. But linear throttle isn't. 

Because in the old bldc-tool the current control mode was like linear throttle. And watt control (new current control) is a throttle that adjusts to the limits.

Sounds strange but that's what feels best and what is also the most controllable.
```

---
## \#302 Posted by: trampa Posted at: 2017-09-17T20:42:10.019Z Reads: 179

```
If you brake hard (e.g. going down a steep hill), you generate a lot of energy and that needs to go somewhere. Without a waste gate, generating heat from the electric energy, wasting it into the air surrounding your board, you need to store it in your battery. The energy needs to go somewhere - either into the battery, or into heat. What you don't want is heating up your motor, since that would make it fail/drop out after reaching a critical temp.

There is no other option, other than storing it. So don't expect strong brakes when you don't allow the energy to be stored in your battery. This has nothing to do with the software you use. No software can magically dissipate energy into the vacuum of the universe. Strong brakes = high amp flow towards the battery if you don't install a highly capable waste gate. Unfortunately we sometimes ride on hot tarmac + air is poor heat conductor. 

I think people have the wrong impression that they could have strong brakes without the need to store the generated energy. 1000W braking is 1000W electrical energy. It makes no sense to give users the wrong impression that they can adjust their values to low Amp settings on the battery side, and have strong and enduring brakes. You need to face the reality. You wouldn't expect a strong acceleration if you'd set battery max to 10A only, would you? Braking is negative acceleration.

Frank
```

---
## \#303 Posted by: Pimousse Posted at: 2017-09-17T20:43:44.762Z Reads: 177

```
@Ackmaniac, you should point this directly on the VESC project forum. ;)
Nice you investigated on this "issue".
```

---
## \#304 Posted by: Silverline Posted at: 2017-09-17T20:54:03.191Z Reads: 182

```
Then i dont understand what 'motor min.' does, when it's 'bat. Min' that determines how much energy to the battery, and therefore All so braking strength in the motors ?

Btw. I find it quite weird, that Benjamin is not on the World biggest Esk8 forum.
```

---
## \#305 Posted by: Ackmaniac Posted at: 2017-09-17T20:54:03.980Z Reads: 185

```
Absolutely right. But still the wrong way to handle the brake power in the software. 
Because it results in unpredictable brakes. Just let Benjamin know that it would be a better way to handle the brake like in the old firmware. 
Strangely when i came with the idea of watt control for brakes in his forum he said himself that it wouldn't make sense to calculate the brake current that way.
```

---
## \#306 Posted by: Maxid Posted at: 2017-09-17T21:52:34.843Z Reads: 193

```
Sounds correct but what is the difference between the old and new methods? The old one worked AND had limits in the regen current. What did the old firmware do to the rest of the energy and why can't the new one do the same thing?
```

---
## \#307 Posted by: SilentException Posted at: 2017-09-17T22:03:59.911Z Reads: 189

```
I'm quite certain I'm going to be corrected on this one but I feel like the old FW just used the min(battery_min, motor_min) as braking current limit, no matter duty cycle. Therefore braking would be linear.
```

---
## \#308 Posted by: Ackmaniac Posted at: 2017-09-17T22:40:56.703Z Reads: 195

```
Battery min was there to set a limit. So when this limit would be exceeded then the brake current is reduced. So at high speeds and a low value the brakes would still be weak but still would work at the battery min limit. And once the duty cycle is low enough it gains brake force and then works on a constant level.

To achieve the battery min brake limit in the new software you need to do a full brake. But when the duty cycle get's too low you quickly brake too hard and the brake strength varies the entire time while the trigger is stable. So you are constantly trying to find the right mount of brake with your finger.

Long story short, the old solution fro braking was better and it is easy to fix in the new firmware if Benjamin decides to do so.
```

---
## \#309 Posted by: SilentException Posted at: 2017-09-17T23:15:10.242Z Reads: 189

```
Funny thing, in the prototyping or thinking phase I would say that current implementation makes much more sense and it is the correct one. But the old version is much better in practice.
```

---
## \#310 Posted by: Eboosted Posted at: 2017-09-18T01:45:38.715Z Reads: 194

```
I'm going back to the old firmware, the new one has too many issues, the unpredictable braking and overcharging the battery are the most important things, the next one is "R is 0" which won't allow me to run FOC on my Focbox. 

This FW might work in the future but for now, it's not ready
```

---
## \#311 Posted by: skslingo21 Posted at: 2017-09-18T01:46:58.659Z Reads: 198

```
WOW just WOW :astonished:

just updated firmware from version 2.18 to version 3.28  on dual 4.12 hardware VESC's on an TRAMPA using the VESC-Tool for the first time. 

Setup was a breeze!!! Hover over virtually anything or look for a question mark and a help box appears!!! 

-New firmware HAD to be updated before VESC-tool would allow full connection to the VESC's. No problem, just BE SURE YOU KNOW WHICH HARDWARE VESC YOU HAVE, mine was 412...
http://www.electric-skateboard.builders/t/what-is-the-difference-between-certain-hw-versions-of-vesc/2629
-Ran motor setup wizard, Breeze!! Help boxes appear often to remind you what parameters are being set and what to prepare for and expect(spinning motors, keep clear etc. SO helpful!)
-Ran controller setup Wizard, which asks whether the current VESC is a master or slave! So easy!! No controller setup was required for the slave! 

**My thanks go out to BENJAMIN VEDDER :innocent: and ALL who made this happen. :punch: A great thing got a lot better.** 

_I run exclusively FOC for its quiet nature. So I cannot compare any differences in BLDC or sensorless. Also this is my opinion, since no real world figures were recorded._ 

Running just the Wizards for setup, using the same settings I ran before, Immediate differences were noted.
1. More powerful
Areas like light brush over 2ft was previously giving me trouble. Also slow starts uphill were difficult to finesse, slowing me until the motors were churning to a standstill. With the update, I tackled brush I would have turned away from, and Ive tackled some huge mounds of grass so far, creeping up them slowly to immitate an unexpected hill climb. 
This, as well as the following will help a great deal with the real rough trails I like to bash!
2. Less cutouts. 
 Both VESCS previously experienced a timeout when jumping and holding the throttle. Also on fast street startups and fast sidewalk bumps. No more! Over 15 miles today on the 3.28 update and did not experience one timeout. This was plaguing my funtime and thought I just needed more HG2's onboard...trailriding was causing major cutouts so I am excited to get padded up and head for the real rough stuff thats gives the belts hell :smiling_imp: 
Finger temperature readings were as usual after long 33km/h stretches (this seems to produce more heat than anything else I do) VESCS are running room temp as always and motors were quite warm to the touch as always. 
<img src="/uploads/db1493/original/3X/9/b/9b6a10be030a0dbff7265c413bd4b70dbf4cf4e1.jpg" width="598" height="448">
```

---
## \#312 Posted by: xxlv Posted at: 2017-09-18T06:12:35.384Z Reads: 188

```
[quote="Silverline, post:304, topic:32268, full:true"]
Btw. I find it quite weird, that Benjamin is not on the World biggest Esk8 forum.
[/quote]

Trampa is holding Benjamin hostage. Frank is the only way he can communicate with us.
```

---
## \#313 Posted by: onepunchboard Posted at: 2017-09-18T06:19:16.937Z Reads: 183

```
Yeah, he is in a secret room with no window.
```

---
## \#314 Posted by: trampa Posted at: 2017-09-18T06:20:45.297Z Reads: 180

```
Drop your comments on the Vedder forum, easy. www.vesc-project.com
Benjamin can't get lost in conversation on multiple forums. There is simply no time for that.

Frank
```

---
## \#315 Posted by: trampa Posted at: 2017-09-18T07:03:16.593Z Reads: 187

```
[quote="Ackmaniac, post:308, topic:32268"]
To achieve the battery min brake limit in the new software you need to do a full brake. But when the duty cycle get's too low you quickly brake too hard and the brake strength varies the entire time while the trigger is stable. So you are constantly trying to find the right mount of brake with your finger.
[/quote]

That is what you experience in any brake, car, bike, motorbike. If you apply 50% brake at high speeds, braking is appropriate, while 50% at low speed is blocking your wheels. Kinetic energy is high at high speed and low at low speeds. In consequence the same brake power works against different levels of kinetic energy. When you use the VESC in an automated environment this allows precise computation of your brake force.

When you brake down your car, you release the brake pedal bit by bit while you slow down to get a constant negative acceleration. 
Battery min/motor min now set the absolute strength of the brake at 100% breaking, which is the correct way to handle it because that is what you'd expect it to regulate. If you want to tweak it, you can use the curves to adjust the behavior of the brake. The brake is now more linear (technically), while the throttle curves allow you to de-linearize it to your needs. Otherwise you'd deal with two curves, which would be a bit funny and not predictable, nor precisely adjustable. 

All you need to do is set up the values correctly and use the throttle curves to get your desired braking behavior. 

Frank
```

---
## \#316 Posted by: rwxr Posted at: 2017-09-18T08:17:50.013Z Reads: 187

```
FYI:
I've just sent Benjamin a FOCBOX with the R=0 error for him to investigate.

Cheers
```

---
## \#317 Posted by: Ackmaniac Posted at: 2017-09-18T08:31:09.359Z Reads: 187

```
I don't want to start a argument here because my intention is to improve the controllability and safety.

But you are wrong. Also for the car. A constant pressure on the brake pedal results in a constant deceleration (negative acceleration). 
And for the VESC a constant brake torque (amps) results in a constant deceleration.
```

---
## \#318 Posted by: landonkun Posted at: 2017-09-18T09:00:59.040Z Reads: 187

```
[quote="Ackmaniac, post:317, topic:32268"]
But you are wrong. Also for the car. A constant pressure on the brake pedal results in a constant deceleration (negative acceleration).
[/quote]

Exactly. When I'm driving my car and depress the brake pedal, the deceleration is constant. Lifting my foot off the brake pedal would cause my car to decelerate less and less...
```

---
## \#319 Posted by: Pimousse Posted at: 2017-09-18T09:03:09.619Z Reads: 191

```
@trampa 
You know that I always supported you and Ben all along this project.
But these last days/weeks, I can't really understand your reaction.
I mean, we are involved in an open source project which means that people can bring contributions.
These may be bugs correction, features coding or simply beta testing. 
Now we receive feedbacks of many people having issue with brakes.
That's a statement, and it's kind of a serious stuff as it makes them going back to FW2.xx (and keep them away from VESC Tool).
But another contributor @Ackmaniac figured out what causes this issue.
Perfect Open Source spirit, isn't it ? ;)

So why do you hide behind theory (and as an energy engineer, I can say that it's even not true) instead of simply take it into account and release a beta FW with Ackmaniac's proposal just for testing ?
If it's worse, back to original and you're right.
If it's better, everybody will be happy to enjoy VESC Tool again and will thank you for having taken into account their request. :slight_smile:
```

---
## \#320 Posted by: trampa Posted at: 2017-09-18T10:42:04.089Z Reads: 192

```
That is all possible Pimousse, but the best way to to contribute is to write something about it on the vesc-project.com forum, or if your skills allow it, do a pull request and suggest some alternative code. Benjamin is happy about it and will look at it and respond and debate it! It's can take a while sometimes, so patience is required.

http://www.vesc-project.com/node/110

I just try to explain why people face weak brakes and Ackmaniac did the same. Sure it's all debatable and hints are taken serious.  If you understand the matter, it's easy to adjust your settings appropriately. The VESC-Tool is being used in all sorts of environments, not only skateboards. It's multi purpose use. Skateboarders love this, robotic guys want that.
In consequence Benjamin is aiming at technically correct solutions, which allow the same adjustments of parameters as before, but in a more sophisticated and precisely adjustable way. People have different demands. You want it this way, another user wants it that way.
The only way forward is the technical correct way allowing appropriate settings for all/most demands.

There is a square relation between kinetic energy and speed! If you apply the same brake force at higher speeds, you gain a lot less negative acceleration (brakes feel weaker) because you work against a lot more kinetic energy. Same for acceleration. 
You can now adjust that behaviour through the use of a curve to fine tune to the desired brake force/acceleration at a certain speed. So you can now compensate things actively, which wasn't possible like that before.
You set your max brake strength first and then you adjust the curve to the desired response over the range of speed you usually travel at. So you now actively de-linearise it to your needs (which might feel more linear to you personally), which gives you better control over your brakes. Options are: ploynominal, normal and exponetial.
You just need to know the feature and use it accordingly and experiment a bit.

Benjamin already split the throttle curves for brake and acceleration, so you can have a very soft acceleration, while adjust for a lot harder brakes. I had no issues to find sweet settings.
He did that because it was requested by multiple users and because it makes sense.

Anyway, we will do some test runs next weekend and will debate it all, and maybe it results in a FW/software tweak, additional feature etc. Benjamin wants to make some videos about correct setups, which will be the way forward for many users. He aims at perfection and that will be the result very soon. So your input is important and in consequence there is a ToDo list online, so you can see that your hints/demands are on the list and being worked on.

http://www.vesc-project.com/node/110

I don't want to fight anyone's ideas, it's about understanding the matter. 
Still opinions can vary, which doesn't mean that your opinion isn't taken into consideration.

Frank
```

---
## \#321 Posted by: Ackmaniac Posted at: 2017-09-18T10:58:21.253Z Reads: 187

```
[quote="trampa, post:320, topic:32268"]
There is a square relation between kinetic energy and speed! If you apply the same brake force at higher speeds, you gain a lot less negative acceleration (brakes feel weaker) because you work against a lot more kinetic energy. Same for acceleration. 
You can now adjust that behaviour through the use of a curve to fine tune to the desired brake force/acceleration at a certain speed. So you can now compensate things actively, which wasn't possible like that before.
[/quote]

And that is where you are wrong. Because with the paddle at a car you apply pressure to the disc brake. And the faster the disc rotates the more energy is transfered into heat. 
For electric motors it is the same. The faster the Motor rotates the higher is the voltage and with a constant current it results in higher watts.

But I am sure Benjamin understands and will identify this as an issue as well. And it also doesn't make any sense for robotics. There the non linear throttle could be a issue but not a linear brake.
```

---
## \#322 Posted by: Pimousse Posted at: 2017-09-18T12:27:46.653Z Reads: 189

```
[quote="trampa, post:320, topic:32268"]
I don't want to fight anyone's ideas, it's about understanding the matter. 
Still opinions can vary, which doesn't mean that your opinion isn't taken into consideration.
[/quote]

Thank you for your answer, it reassures me.

However, I'd like to raise your attention on an important point.
You said :
[quote="trampa, post:320, topic:32268"]
If you understand the matter, it's easy to adjust your settings appropriately. The VESC-Tool is being used in all sorts of environments, not only skateboards. It's multi purpose use. Skateboarders love this, robotic guys want that.
[/quote]
You're now selling VESC6 through your shop.
I can tell you that some of your customers even don't understand the difference between batteries in series or in parallel.
For my part, on the french forum, it consumes A LOT of time to help them, although I wrote tutorials and so on.
So you definitely can't assume that people will figure out which parameter they have to "cheat" to reach the expected brake behaviour. :wink:
VESC Tool is a huge improvement thanks to wizards to help novice getting started with VESCs,
Keep it intuitive af. :slight_smile:
```

---
## \#323 Posted by: trampa Posted at: 2017-09-18T14:44:24.439Z Reads: 182

```
This is why video tutorials are the way forward. If you know the FAQs, you can answer the questions.

Frank
```

---
## \#324 Posted by: Pimousse Posted at: 2017-09-18T15:00:51.120Z Reads: 189

```
If only a day can count more than 24h, I would be pleased to do so. ;)
ATM, every answer to a novice question is added to the tutorial.

But it's already complicated to explain why you put this in motor max, that in battery min, etc.
So if now you have to say "Ok, your battery can handle 20A in regen but there is a trick for having usable brake, so put 34A instead...".
What a mess. :smile:
```

---
## \#325 Posted by: trampa Posted at: 2017-09-18T15:39:10.670Z Reads: 188

```
But that's at least the truth. Your battery has to swallow what you shoot towards it. So a builder can make the decision to go for higher P counts and higher S counts, better cells etc. 

Frank
```

---
## \#326 Posted by: chinzw Posted at: 2017-09-18T17:02:33.937Z Reads: 186

```
Is it just me or does this conversation seem like talking to a wall?
```

---
## \#327 Posted by: trampa Posted at: 2017-09-18T17:30:54.900Z Reads: 189

```
Benjamin and I thought of short episodes, explaining one feature of Vesc tool after another.
This way a new user can simply follow the vids step by step. We will collect the questions, which helps to make short videos. 

Frank
```

---
## \#328 Posted by: Silverline Posted at: 2017-09-18T17:48:41.123Z Reads: 181

```
First step, would be to introduce Benjamin to this forum ;-) Maybe even make him a profile :-P
```

---
## \#329 Posted by: Pimousse Posted at: 2017-09-18T18:04:24.376Z Reads: 181

```
Great !
Anyway, I saw that @Ackmaniac posted a pull request on Github as you suggested. :slight_smile:
```

---
## \#330 Posted by: Eboosted Posted at: 2017-09-19T01:28:39.080Z Reads: 179

```
Can't wait to have @ackmaniac firmware on my FocBox, instead of defending a point of view he always comes up with a solution in matter of hours, if he partners with Benjamin the only winner would be the community
```

---
## \#331 Posted by: L3chef Posted at: 2017-09-19T05:11:35.380Z Reads: 179

```
<img src="/uploads/db1493/original/3X/2/f/2f56df9e21713fe42a2e5f01958b1f61476fa120.jpg" width="600" height="400">
```

---
## \#332 Posted by: TheCheat Posted at: 2017-09-19T05:18:30.697Z Reads: 180

```
Hardly a point of view as much as it was a stubborn decision with no justifiable backing.
```

---
## \#333 Posted by: ThierryGTLTS Posted at: 2017-09-19T07:05:44.990Z Reads: 184

```
Very good idea!!!

Thierry
```

---
## \#334 Posted by: Sapphirinia Posted at: 2017-09-20T17:09:54.227Z Reads: 180

```
Hi guys. I tried setting up my controller with the wizard but when I applied settings the motor started spazzing. I messed with the trim but then I got it to go in one direction but not change based on the trigger position. So it's not stopping or starting with the trigger and I couldn't get it to stop until I turned off the board
```

---
## \#335 Posted by: onepunchboard Posted at: 2017-09-20T17:41:36.115Z Reads: 180

```
re do ppm setting. this solved me that bug before
```

---
## \#336 Posted by: Sapphirinia Posted at: 2017-09-20T20:26:55.369Z Reads: 184

```
That worked. Thanks
```

---
## \#337 Posted by: Pimousse Posted at: 2017-09-22T07:05:06.196Z Reads: 179

```
A new version of firmware is available : FW3.29.
The control has been switched back to pure current control (like 2.18) to fix brake issue.
So those who had the brake issue, you may want to give a try to this new firmware ;)
```

---
## \#338 Posted by: Klattrup Posted at: 2017-09-22T10:54:48.090Z Reads: 171

```
Is this change only for the breaking part or for the acceleration as well? :)
```

---
## \#339 Posted by: hexakopter Posted at: 2017-09-22T10:59:49.072Z Reads: 174

```
I think just breaking has changed. But I am not sure.
Btw. Looks like [http://www.vesc-project.com](http://www.vesc-project.com) is down again.
```

---
## \#340 Posted by: Pimousse Posted at: 2017-09-22T11:24:11.630Z Reads: 178

```
Both.
It's not like 2.54 (watt control for acceleration, current for brake, AFAIK), more like 2.18 (current control accel and brake)

EDIT : you can find firmwares in the vedder's github repo.
```

---
## \#341 Posted by: hexakopter Posted at: 2017-09-22T11:33:25.805Z Reads: 170

```
Thanks for the info. Have used the regen brake on my bike just ones so I dont know the different feelings.
Great to see the sources now on github. Have compiled the new VESC tool now. :slight_smile:
```

---
## \#342 Posted by: ThierryGTLTS Posted at: 2017-09-22T15:04:27.884Z Reads: 170

```
VESC Project website works now!

Thierry
```

---
## \#343 Posted by: Jinra Posted at: 2017-09-22T15:06:20.236Z Reads: 173

```
Glad Ben addressed this, unlike some others that would like to deny the problem exists...
```

---
## \#344 Posted by: BigBoyToys Posted at: 2017-09-22T15:57:44.579Z Reads: 174

```
I got the R=0 error on 1 of 4 TB vesc's last night as well with FW3.28.

My FOC box's also have the R=0 error on FW3.28 but detect just fine on FW3.26.
```

---
## \#345 Posted by: Vanarian Posted at: 2017-09-22T16:34:28.535Z Reads: 178

```
Did he ? Because the Watt control for throttle / acceleration is gone too. Looks like a step backward to me :( 

Best thing would have been to keep acceleration as it was in last FW and just put old braking back.
```

---
## \#346 Posted by: Jinra Posted at: 2017-09-22T16:34:51.842Z Reads: 178

```
addressed =/= fixed :)
```

---
## \#347 Posted by: Eboosted Posted at: 2017-09-22T19:32:13.985Z Reads: 177

```
I'm I missing something? Please give us some more info @jinra
```

---
## \#348 Posted by: Jinra Posted at: 2017-09-22T19:35:02.701Z Reads: 176

```
in 3.29 brakes **seem** to be back to normal (like in 2.18/2.54). I'm using -25A right now, but I'll try dropping it down to -10 again to see how my brakes are. It was a bit weird that this wasn't mentioned in the changelog though, unless it falls within "disabled throttle limit scaling"
```

---
## \#349 Posted by: Pimousse Posted at: 2017-09-22T21:27:19.716Z Reads: 177

```
The best way to figure out that has been changed is yo lokk closely to the code changed.
Github is a powerful tool that allow to quickly focus on what has been added/deleted/changed. ;)

If really needed, it won't be too difficult to compile a custom firmware using Watt mode for accel and current control for brake.
@Ackmaniac wrote the code in his [pull request](https://github.com/vedderb/bldc/pull/41).
```

---
## \#350 Posted by: Eboosted Posted at: 2017-09-23T01:47:06.870Z Reads: 176

```
I just uploaded 3.29 FW, I'm testing in 30 minutes. I'l report back as soon as I get home.

Here are my new settings:

Motor max: 70A
Motor min: - 60A
Battery max: 40A
Battery min: - 25A

Brakes are much better now, almost as much as the 2.54 FW, but still at high speed if you pull the brakes hard you feel less braking power than the old firmware.

There was a huge difference in power delivery going on motor max from 60A to 70A, the 6374s are shining at its best now.

I still feel uneasy pulling such big amount of current onto the battery, I need to make a log as soon as the Bluetooth app starts working
```

---
## \#351 Posted by: Jinra Posted at: 2017-09-23T02:00:14.711Z Reads: 169

```
I think, you'll like it. The brakes are def better, hopefully we get watt control throttle back with different logic for braking.
```

---
## \#352 Posted by: Eboosted Posted at: 2017-09-23T03:33:23.990Z Reads: 167

```
I didn't feel any non-linear braking, maybe Ben changed the braking logic current calculation
```

---
## \#353 Posted by: Jinra Posted at: 2017-09-23T03:38:38.734Z Reads: 164

```
yea he did, it's current control like in 2.18 again
```

---
## \#354 Posted by: crustyxpunk Posted at: 2017-09-23T04:05:57.981Z Reads: 163

```
Did you ever try FOC with the new firmware? I've been running it for a few days and haven't had any issues with my TB vesc. Super smooth!
```

---
## \#355 Posted by: Eboosted Posted at: 2017-09-23T05:40:04.327Z Reads: 162

```
I wonder why didn't Ben corrected the error on setting up FOC. I've heard Ben got a VESC X hope he finds the fix for the dreaded "R is 0 please calculate it first"
```

---
## \#356 Posted by: Jinra Posted at: 2017-09-23T05:42:40.931Z Reads: 165

```
When I ran into that error, I ran BLDC detection (but didn't apply or write), then ran FOC again and it started work. I was using an ollin VESC, however.
```

---
## \#357 Posted by: Eboosted Posted at: 2017-09-23T05:43:35.634Z Reads: 165

```
Are you currently runing FOC?
```

---
## \#358 Posted by: Jinra Posted at: 2017-09-23T05:43:46.846Z Reads: 170

```
yes sir :smile:
```

---
## \#359 Posted by: okp Posted at: 2017-09-23T05:50:44.882Z Reads: 169

```
I ran the 3.26 for around 900km ; I've updated to 3.29 yesterday evening. Will ride the full weekend as its sunny in Paris and report back. 

Just after the update, I went to setup my VESC and going via the Motor Wizard. Everything went fine except on the Hall sensor detection that failed in FOC. So I had to do it outside of the wizard and for some reasons and without changing anything it worked fine on the wizard now. I think I've filmed a video of this.

I'm running 12S4P VTC5A on dual 150kv - no BMS with a 80A fuse (need to get a 100A)
Motor max: 40A
Motor min: - 40A
Battery max: 40A
Battery min: -12A

Cheers.
```

---
## \#360 Posted by: Jinra Posted at: 2017-09-23T05:53:29.370Z Reads: 161

```
Why would you need an 100A fuse with 40A battery max? Even dual you'll never pull 80A continuous and even if you do your fuse still won't blow, at least for a long long time.
```

---
## \#361 Posted by: okp Posted at: 2017-09-23T05:54:11.114Z Reads: 159

```
cause this will enable to move the batt/motor max to 50A as I'm running dual VESC and align to 100A
```

---
## \#362 Posted by: Jinra Posted at: 2017-09-23T05:55:51.183Z Reads: 159

```
ah i see. I'd bet you would never blow the fuse even if you use 100a now. I used 80A (40A x2 vesc) battery max with a 40A fuse just fine up the steepest hills in SF.
```

---
## \#363 Posted by: okp Posted at: 2017-09-23T05:57:25.669Z Reads: 162

```
hehe lucky guy. I blown a 40A fuse with 60/60A on my tests so now I really always align the fuse to the batt max on the VESC although as you said I may be extra careful.
```

---
## \#364 Posted by: Jinra Posted at: 2017-09-23T05:59:46.281Z Reads: 160

```
yea perhaps those big ol AT wheels just pull more current than my comparatively small thane wheels
```

---
## \#365 Posted by: Eboosted Posted at: 2017-09-23T06:15:09.469Z Reads: 162

```
[quote="okp, post:359, topic:32268"]
Motor max: 40A
Motor min: - 40A
Battery max: 40A
Battery min: -12A
[/quote]

Why do you run only 40A motor max? Why not increase it to 60A it even more? I increased the motor max from 60A to 70A on a 12S4P and the torque was insane!

On the new firmware it seems battery min needs to be increased almost double the regular old firmware current in order to keep the same braking power
```

---
## \#366 Posted by: okp Posted at: 2017-09-23T06:52:23.577Z Reads: 159

```
you are limited by the batt max which is 80A (aligned with my fuse) as it's dual. So I align the batt max (40A) per VESC with the motor max per VESC to get everything on the same page. Batt min is regen. 12S4P is 4x6A so 24A : -12 on each VESC.
```

---
## \#367 Posted by: Jinra Posted at: 2017-09-23T06:53:34.359Z Reads: 165

```
Motors can draw more current than the battery max at lower than full duty cycle
```

---
## \#368 Posted by: okp Posted at: 2017-09-23T06:58:52.266Z Reads: 167

```
I have setup an Heavy Duty Eagle tree inline so I'm able to log many things on the ride. Any advice on the settings or tweak so I can report back? I was looking to get a full alignement on batt / motor but any tweak is welcome. I'm using FOC. I'm actually testing the 107mm but can't wait to put the upcoming Trampa wheels on this!

https://www.instagram.com/p/BZJ0U8tB58z/?taken-by=esk8fr
```

---
## \#369 Posted by: Jinra Posted at: 2017-09-23T07:01:10.487Z Reads: 164

```
you'll be safe with 70A, try that out and see how you like it! It'll essentially expand your throttle by 75%
```

---
## \#370 Posted by: okp Posted at: 2017-09-23T07:03:37.723Z Reads: 167

```
on the 12S dual setup FOC it will be (on each VESC)
Motor max: 70A
Motor min: - 40A
Battery max: 40A
Battery min: -12A

right?
```

---
## \#371 Posted by: Jinra Posted at: 2017-09-23T07:12:06.145Z Reads: 166

```
yep, motor min is the inverse opposite and applies braking strength. My rule of thumb is to have motor min 10 less than motor, for inversely equivalent braking/acceleration. So in this case -60 motor min would be what I use, but I wouldn't change it unless you feel like you need stronger brakes.
```

---
## \#372 Posted by: okp Posted at: 2017-09-23T07:13:22.712Z Reads: 165

```
Perfect. Thanks for the tips. I'm gonna adjust that right now and report back. I had in mind that on dual VESC setups everything had to be divided by two but it seems this only applies to batt max/min
```

---
## \#373 Posted by: Jinra Posted at: 2017-09-23T07:14:40.249Z Reads: 161

```
Yea, since the motors are independent (vs battery being 1 thing) you can leave those separate.
```

---
## \#374 Posted by: Silverline Posted at: 2017-09-23T15:22:38.405Z Reads: 160

```

@Jinra
 So you are saying that motor max, should be higher than batt. max ?? 
I run dual setup
And for now, i have set motor max and batt. max on each focbox to 35amp. Do you think that i should increase Motor max ?? Would that give me more torque in the low end ?

Thanks
```

---
## \#375 Posted by: Jinra Posted at: 2017-09-23T15:33:52.429Z Reads: 157

```
yep, try it out 60, is a good number to start at
```

---
## \#376 Posted by: Silverline Posted at: 2017-09-23T15:55:30.960Z Reads: 158

```
Thanks
But i dont understand, if batt. max , is set to 35amp, why motor max 60 amp would give me more torque ?
```

---
## \#377 Posted by: Jinra Posted at: 2017-09-23T15:59:37.580Z Reads: 153

```
Because wattage == power. Your battery is applying a constant voltage to your vesc, but the motors voltage depends on duty cycle. Low duty needs high amps for power.
```

---
## \#378 Posted by: Silverline Posted at: 2017-09-23T16:14:53.754Z Reads: 156

```
Ahhh i se
 So i Still dont pull more than my batt. Max (35 Amp) but more power (Amp/watt) is applied at a lower duty cycle ? Because ohms law says, that lower voltage pulls more Amp, than higher voltage ?
Then why 60amp and not 100amps ?

At let's say 10% duty cycle, do you know what the voltage is, on 10s ?
Then it could be pretty easy to calculate the motor max...

So if i'm driving Up a steep Hill, and giving full throttle, then if my motor max is to low, i would never reach full 95% duty cycle where the motors is giving bat. Max ?
```

---
## \#379 Posted by: Jinra Posted at: 2017-09-23T16:46:31.432Z Reads: 158

```
Too high and you may burn out your motors. You can set it pretty high though. Hummie and some others run 120a motor max. 10% duty on 10s is 3.6v nominal
```

---
## \#380 Posted by: Silverline Posted at: 2017-09-23T17:00:06.551Z Reads: 162

```
Thanks.... it make sense now :-)

Then going from motor max 35amp to 60 amp... should increase my torque / acceleration quite a bit
```

---
## \#381 Posted by: okp Posted at: 2017-09-23T19:29:18.823Z Reads: 168

```
Just did the full circle travel around Paris with a lot of extra kms. Run like a charm. VESC 6 Awesomeness. 

<img src="/uploads/db1493/original/3X/6/b/6b60b1a34c54ceb835ef299aca4821928617d674.png" width="690" height="375">

and a short video as you already knew !

https://www.instagram.com/p/BZZIulYBECy/?taken-by=esk8fr
```

---
## \#382 Posted by: Pimousse Posted at: 2017-09-23T22:07:41.770Z Reads: 163

```
I built an Excel sheet for helping beginners setting their VESC, I should make it public here, maybe it could help.
It simply takes the same rule of thumb as @Jinra : motor max -10A in a limit of -70/70A (I trigerred some over_current @80A).  ;)
```

---
## \#383 Posted by: hexakopter Posted at: 2017-09-23T22:24:31.827Z Reads: 167

```
I saw that there was a discussion about the brakes here a few days ago. I am on FW3.29 now. Can someone of you explain me the strange behavior you can see in the graph starting at 18:21:50?
[https://metr.at/r/65XOy](https://metr.at/r/65XOy)
I dont get why there is a motor current while the current back in the battery is zero.
```

---
## \#384 Posted by: Pedrodemio Posted at: 2017-09-23T23:11:55.385Z Reads: 163

```
@hexakopter  I can say for sure, but in my understanding when you achieve full brake, the VESC is shorting all the phases together, so the energy is dissipated in the windings and not sent to the battery

This only occurs when ERPM is bellow the "max rpm to full brake" and if even at 95% duty cycle the break current measured is lower than the requested brake current

Basically the VESC says, the rider want more brakes but I'm already at my max duty cycle, the current limits have no been triggered, the only thing I can do to increase the braking power is to short the motor
```

---
## \#385 Posted by: Silverline Posted at: 2017-09-24T06:54:57.767Z Reads: 162

```
Thanks... I would like to se that Excel ark :-)
```

---
## \#386 Posted by: Pimousse Posted at: 2017-09-24T08:19:05.768Z Reads: 170

```
I found it. But need to translate from french now. ;)
```

---
## \#387 Posted by: Sapphirinia Posted at: 2017-09-26T22:10:29.863Z Reads: 173

```
Can anyone help me out with the remote settings? For some reason my remote stopped binding and I switched to my old clunky one and I can't get it to control the board.
```

---
## \#388 Posted by: Eboosted Posted at: 2017-09-27T02:02:10.463Z Reads: 178

```
At last I was able to set up my motors in FOC with my FocBox (early version), but when I set App Settings and select Current no reverse with brake and give throttle to the remote my motors won't spin even though I can see the PPM mapping in real time.

[img]https://i.imgur.com/rVSrCdO.jpg[/img]

Is there a trick when setting up FOC?
```

---
## \#389 Posted by: onepunchboard Posted at: 2017-09-27T02:15:40.845Z Reads: 166

```
nope. thats the dead end just like rest of us. no ppm for foc at the moment
```

---
## \#390 Posted by: Eboosted Posted at: 2017-09-27T02:49:46.559Z Reads: 162

```
Shit! Glad to know about it at least, no need to loose 2 more hours
```

---
## \#391 Posted by: Jinra Posted at: 2017-09-27T02:53:44.977Z Reads: 163

```
what are you talking about I've been running ppm on foc 3.29...
```

---
## \#392 Posted by: onepunchboard Posted at: 2017-09-27T03:09:30.706Z Reads: 163

```
is it a focbox? then tell me the solution. why does the motor perma brake when connected to receiver after successful detection. i didnt tried the minor updates(brake fix) but does this makes it work?
```

---
## \#393 Posted by: Jinra Posted at: 2017-09-27T03:11:57.797Z Reads: 170

```
well in his screenshot his mapping is wrong. I noticed this happening with one of my controllers and not a different controller. Probably has more to do with that rather than being a focbox. In that case you just have to record and enter the ppm values manually.

@Eboosted
```

---
## \#394 Posted by: Eboosted Posted at: 2017-09-27T05:23:41.570Z Reads: 173

```
PPM wasn't set at that particular moment, however, trust me, I did set it later and got the same issue, master motor permanently braked, it also releases when selecting BLDC back again.

[quote="onepunchboard, post:392, topic:32268, full:true"]
is it a focbox? then tell me the solution. why does the motor perma brake when connected to receiver after successful detection. i didnt tried the minor updates(brake fix) but does this makes it work?
[/quote]

Yes, I have a FocBox and it does perma brake as soon as I select FOC, no PPM signal transmited to the VESC, no spinning from the wheels.

The procedure to be able to run FOC detection without getting the "R is 0. Measure it first" I used was this:

1. Run Motor Detection Wizard
2. Load default values
3. Select BLDC
4. Use these current settings:
Motor Max 70A
Motor min -60A
Battery Max 40A
Battery Min -25A
5. Set up cutoff start and end, in my case 12S4P
Cutoff start; 36V
Cutoff end: 33.6V
6. Select hall sensors
7. Increase D=0.05 to D=0.1
8. Run BLDC motor detection
9. Hit apply
10. Save motor settings
11. Go to General tab and select FOC
12. Go to FOC tab
13. Hit RL
14. Hit lambda
15. Hit apply
16. Write motor settings
17. Set App Settings for master VESC

After doing all these and try to use the remote, the master motor permanently brakes, feedback from the remote
```

---
## \#395 Posted by: Jinra Posted at: 2017-09-27T05:25:59.925Z Reads: 166

```
does FOC cause it to fully brake when you have both the below settings turned **off**?

App Settings > General > App to Use = No app
App Settings > PPM > Control Type = Off
```

---
## \#396 Posted by: Eboosted Posted at: 2017-09-27T05:29:14.335Z Reads: 171

```
That's a good question, I didn't test that, however even when I fully pull the throttle while I watching the PPM going all the way to 100%

App Settings > General > App to Use = Current no reverse with brake
App Settings > PPM > Control Type = Current no reverse with brake

Motors won't spin, master motor perma braked

As soon as I switch to BLDC motors spin perfectly, no perma brake

Hope this is only a glitch and newer versions are released
```

---
## \#397 Posted by: Jinra Posted at: 2017-09-27T05:30:42.250Z Reads: 170

```
Huh that's pretty weird.. Is this with one VESC no split Y or CAN connection? I'd take those off if you have them to eliminate other factors.
```

---
## \#398 Posted by: Silverline Posted at: 2017-09-27T09:14:36.925Z Reads: 171

```
I have the same problem with my focbox. FOC does not Work... The motor is locked , the moment i connect my receiver to the VESC. I got the R = 0 bug, if the receiver is connected under foc motor detection. So i disconnect the receiver , run the foc motor test with succes, connect the receiver again. And then the motors wont spin. I can all so se the ppm output in gui, and the end and mid points is spot on. So at the moment i run BLDC :-/
```

---
## \#399 Posted by: Ackmaniac Posted at: 2017-09-27T10:46:32.659Z Reads: 168

```
The issue is not related to ppm. FOC simply doesn't work correct.
```

---
## \#400 Posted by: Pimousse Posted at: 2017-09-27T13:22:51.458Z Reads: 168

```
How to explain that people run FOC with PPM flawlessly (like me on 3.28) and others don't ?
It's pretty hard to find a common factors through all these feedbacks.
```

---
## \#401 Posted by: Ackmaniac Posted at: 2017-09-27T13:25:03.473Z Reads: 169

```
Has nothing to do with PPM if you ask me. Seems that high resistance motors work better than low resistance motor. 
Does anybody have the Version 3.26 for 4.12 hardware? Just want to give it a try.
```

---
## \#402 Posted by: Silverline Posted at: 2017-09-27T13:41:59.497Z Reads: 169

```
Before i could get bldc motor test to work on my focbox, i had to play with the test values (sk3 6364 190kv) could it be the same 'problem' with foc motor detection ??
```

---
## \#403 Posted by: Pimousse Posted at: 2017-09-27T13:47:53.146Z Reads: 166

```
To figure out if you're right, it should be interesting if someone with the PPM not working can try to run the motor in FOC through VESC Tool with manual controls.
Because I really don't get why it's so random.
```

---
## \#404 Posted by: trampa Posted at: 2017-09-28T07:51:11.741Z Reads: 166

```
Benjamin tried a FOCBOX that was reported to have the R=0 issue and would not spin up using PPM.

We plugged it into one of our motors and had a straight success using the wizards. No issues!
Motor: 118 KV Trampa

Next step: Higher KV motor test, hoping that the issue can be replicated soon. Benjamin has a couple of motors to try...

If you have a low KV motor to the hand you could simply give it a try.

Frank
```

---
## \#405 Posted by: Silverline Posted at: 2017-09-28T10:09:26.056Z Reads: 165

```
190kv gives me R=0 fail....
```

---
## \#406 Posted by: trampa Posted at: 2017-09-28T10:26:47.633Z Reads: 166

```
We will have a look the next days. The issue needs to be replicated first to see where the problem is exactly.

Frank
```

---
## \#407 Posted by: Jinra Posted at: 2017-09-28T14:06:16.016Z Reads: 165

```
I can get you 3.26 later, but what do you mean by high resistance? Mine is 18 ohm, is that high? FOC/ppm works for me at 230kv
```

---
## \#408 Posted by: Ackmaniac Posted at: 2017-09-28T15:02:46.373Z Reads: 164

```
Just tested with 3.26 and the problems do not exist. So the issue is somewhere in the changes from 3.26 to 3.27. But the sources for 3.26 are not available.
```

---
## \#409 Posted by: ThierryGTLTS Posted at: 2017-09-28T15:41:30.657Z Reads: 166

```
What sources are available now?

It seems to be 3.28!

It could be interesting to keep old sources available for comparison purposes.
```

---
## \#410 Posted by: Jinra Posted at: 2017-09-28T15:42:10.086Z Reads: 169

```
so it happens on 3.27+ for you?
```

---
## \#411 Posted by: Vanarian Posted at: 2017-09-30T14:15:16.483Z Reads: 165

```
@trampa Update for you : 85kv FW 3.28 tested in VESC-Tool : 

BLDC detection works (with jittering at low speed very light weight - has spun fine at bit higher speed during detection)

FOC detection fails with R=0 after VESC-Tool feeds current through the motor for few seconds.

So even with low kv motor there is an issue. I use 8S / 33.6V.
```

---
## \#412 Posted by: Silverline Posted at: 2017-09-30T15:07:46.477Z Reads: 162

```
Tested FW 3.29 on FOCBOX, 70kv hubmotor on 10s. R = O bug as well....
```

---
## \#413 Posted by: BigBoyToys Posted at: 2017-09-30T19:21:56.199Z Reads: 156

```
I have r=0 error on 70kv, 110kv, 130kv and 149kv hub motors with 3.27, 3.28 and 3.29 fw. All motors passed detection just fine on 3.26 which is what I went back to using.
```

---
## \#414 Posted by: Ackmaniac Posted at: 2017-09-30T19:49:31.258Z Reads: 153

```
Does anybody have the source files for 3.26
```

---
## \#415 Posted by: BigBoyToys Posted at: 2017-09-30T20:06:55.963Z Reads: 150

```
Are source files different than what we download from the vescproject.com? I have the vesc tool with 3.26FW if that helps.
```

---
## \#416 Posted by: Silverline Posted at: 2017-09-30T20:28:13.359Z Reads: 150

```
Vesc-project is down, again again again...
```

---
## \#417 Posted by: Vanarian Posted at: 2017-09-30T20:28:25.182Z Reads: 153

```
I wonder if source extraction from compiled VESC-tool 3.26 is possible?

Current sources available on Vedder's github are from 3.28 onwards. 

I had to compile my own FW (my GPIOs are assigned differently from standard on my VESCs) to get it working. 

Anyway if you could send it / host it that would help big yes. I can forward your 3.26 VESC-TOOL to the French forum too.
```

---
## \#418 Posted by: BigBoyToys Posted at: 2017-09-30T20:41:25.564Z Reads: 152

```
@Vanarian

Pm your email address. Ill send it when I get home this evening.
```

---
## \#419 Posted by: MontPierre Posted at: 2017-09-30T21:10:17.654Z Reads: 155

```
@BigBoyToys Could you upload your versions on Dropbox for us and paste links here ? I’m sure few of us would be grateful! Thanks !
```

---
## \#420 Posted by: BigBoyToys Posted at: 2017-10-01T03:31:43.427Z Reads: 157

```
This is 3.26FW for the 4.12 VESCS. 

https://www.dropbox.com/s/nlgb3t4o7ev6rk4/Vesc%206%20Tool%20HW6%203.26fw%20-%20Copy.zip?dl=0
```

---
## \#421 Posted by: NAF Posted at: 2017-10-01T19:59:26.204Z Reads: 163

```
Damn !! I've updated my VESC firmware to 3.28 and it is god damn scary !! I just did 5 miles on it and:

- 3 times during my whole ride there was no braking at all !!!!!!! or the braking was very minimal !! no shit guys ..I never ever had that before. 
- a few times the braking felt laggy as shit...after I press the trigger to brake the braking started to initiate with a little lag
- one time the lag was sudden and almost threw me off the board.

Damn .this is scary ... tomorrow I'll look at my settings and post them here.
```

---
## \#422 Posted by: rpasichnyk Posted at: 2017-10-01T20:57:27.881Z Reads: 161

```
Try 3.29, it's has been around for a while and has something to do with breaks.
```

---
## \#423 Posted by: Graphite Posted at: 2017-10-02T13:22:33.085Z Reads: 155

```
Tested with DIY's Vesc, works fine on BLDC(sensored and not) also works easily with FOC. Really appreciate you guys releasing this, has a lot of information to help out us newer guys with configuring settings.
```

---
## \#424 Posted by: trampa Posted at: 2017-10-02T13:49:42.429Z Reads: 156

```
I'm putting together a detailed step by step VESC-Tool setup slide show. Online in a couple of days.

Frank
```

---
## \#425 Posted by: sirus Posted at: 2017-10-02T16:02:07.830Z Reads: 159

```
I recently bought a Trampa Urban Carver. It came with a VESC SIX (VESC 6) and a Maytech Remote control and receiver ( http://www.trampaboards.com/remote-control--receiver-p-24243.html ).

I have built the board and connected everything, but when I move the switch on the controller the motor moves with a squeel/skweek, for 1/20 of a rotation, then stops and the squealing sound becomes very high.

To get the VESC to function with the remote at all I had to install the VESC Tool for the VESC 6 (http://www.vesc-project.com):
1. I had to update the firmware first.
2. Then, I had to switch the controller type from UART to PPM: Under App Settings > General > App to Use > "PPM" > write to esc

Under App Settings > PPM, I have changed the Control type to the 3 different primary categories available, then rewriten to the ESC, and the motor does the same thing each time, for each selection (Current, duty cycle, PID).

Here are screenshots of the software choices:
https://postimg.org/image/2elccxgkor/
https://postimg.org/image/9p972515u3/

Literally, the motor turns a bit, and then makes a high pitch squaling/sqeeking sound.
Any ideas?
```

---
## \#426 Posted by: sirus Posted at: 2017-10-02T16:34:28.993Z Reads: 150

```
I got this all sorted. Apparently after I completed everything above, all I needed to do was follow the Motor Setup Wizard.
So, change the controller type to PPM, then do motor setup wizard.
```

---
## \#427 Posted by: Silverline Posted at: 2017-10-02T17:47:39.056Z Reads: 150

```
@trampa 
Any news, about the R = 0 bug ??
```

---
## \#428 Posted by: trampa Posted at: 2017-10-02T20:57:58.203Z Reads: 151

```
Hopefully we have a result tonight. Benjamin wanted to test out a couple of motors when he is back home. 
The last two weeks were really busy.... This matter needs a quiet moment. I hope the issue will replicate tonight or tomorrow. Fingers crossed! As mentioned before the F-Box he got went through motor and app Wizard without any issues, although it was reported to have the R=0 issue. Maybe the controller is afraid of Benjamin and decided to give up making trouble when it realized where it currently is.

Benjamin just confirmed that it should not have anything to to with the version of VESC-Tool, since the section caring for motor detection didn't change. 

Frank
```

---
## \#429 Posted by: Silverline Posted at: 2017-10-03T10:27:26.872Z Reads: 152

```
I hope he is working something out. Several motors on FOCBOX give me R=0 bug... High and low KV, no difference. 

Only thing that Work. Is flashing back to 2,18fw, do a foc detection, take a screenshot of the values , flash back to 3,29fw, and put in the numbers manually.
```

---
## \#430 Posted by: Pimousse Posted at: 2017-10-03T12:08:25.664Z Reads: 149

```
What is your HW ?
And which FW version did you updated from ?
```

---
## \#431 Posted by: onepunchboard Posted at: 2017-10-03T14:54:28.929Z Reads: 146

```
it only has version 6 fmw tho
```

---
## \#432 Posted by: Jinra Posted at: 2017-10-03T15:03:35.376Z Reads: 143

```
can you try running a bldc detection, then run FOC detection again, without reflashing fw
```

---
## \#433 Posted by: Silverline Posted at: 2017-10-03T15:57:55.473Z Reads: 140

```
Yes...
dosn`t change a thing....
```

---
## \#434 Posted by: BigBoyToys Posted at: 2017-10-03T16:06:55.460Z Reads: 142

```
Where did you get the vesc tool from? The one I posted?
```

---
## \#435 Posted by: onepunchboard Posted at: 2017-10-03T16:23:32.204Z Reads: 144

```
Yeah, i thought it was fmw bin. but the vesc tool. it only shows up ver 60, nothing for 410
```

---
## \#436 Posted by: BigBoyToys Posted at: 2017-10-03T16:26:01.323Z Reads: 145

```
Ohh that means I posted the one for the VESC6. Ill find the 3.26FW for the 4.12 vesc's and post it. Sorry about that.
```

---
## \#437 Posted by: BigBoyToys Posted at: 2017-10-03T16:28:41.144Z Reads: 150

```
Did you try reading you fw type in the tool after connecting in the limited mode?
```

---
## \#438 Posted by: onepunchboard Posted at: 2017-10-03T16:29:47.247Z Reads: 155

```
No it's okay, no need to srry. ur doing the favor for people. I just thought it would be weird,

And yeah I did but it only showed 60.
```

---
## \#439 Posted by: BigBoyToys Posted at: 2017-10-03T16:46:43.588Z Reads: 163

```
Here is the VESC tool with 3.26 FW for the VESC 4.12 HW.

https://www.dropbox.com/s/0jcbirdvfmhywwt/vesc%206_tool%20-%20Copy.zip?dl=0

Here is VESC Tool original for the VESC6 only.

https://www.dropbox.com/s/nlgb3t4o7ev6rk4/Vesc%206%20Tool%20HW6%203.26fw%20-%20Copy.zip?dl=0
```

---
## \#440 Posted by: NAF Posted at: 2017-10-03T17:50:10.573Z Reads: 150

```
HW 4.12 and 3.28 firmware ..I'll try to update to 3.29 and see if there is a difference.
```

---
## \#441 Posted by: Jinra Posted at: 2017-10-03T17:52:48.858Z Reads: 158

```
3.29 does bandaid the braking issue.
```

---
## \#442 Posted by: Vanarian Posted at: 2017-10-03T18:00:34.418Z Reads: 160

```
@trampa Do you have any hints on how to extract the FW .bin files out from VESC-Tool ? I'd like to try 3.26 on my customs VESCs (currently 3.28 loaded) and need to recompile with proper GPIOs assigned first. 

BTW as said before, 3.28/3.29 upload well and BLDC detection works but I get R=0 in FOC wizard. That's also why I'd like to give a try to 3.26 !

@BigBoyToys Thank you for uploading, that's big help !

Edit : @SilentException thanks for the link but I checked and it seems Vedder's Git it is from 3.28 onwards :confused:
```

---
## \#444 Posted by: SilentException Posted at: 2017-10-03T18:19:13.107Z Reads: 155

```
I can extract them from you but point me to the VESC tool EXE file and tell me what hardware and FW you'd like (4.12, VESC_default.BIN or any other).
```

---
## \#445 Posted by: Vanarian Posted at: 2017-10-03T18:34:09.172Z Reads: 160

```
Great thank you ! Can you try extract FW 4.8 from @BigBoyToys link ? I can work my way from there ! VESC-default.bin is perfect (I'll change values manually if needed)

https://www.dropbox.com/s/0jcbirdvfmhywwt/vesc%206_tool%20-%20Copy.zip?dl=0
```

---
## \#446 Posted by: SilentException Posted at: 2017-10-03T19:11:16.235Z Reads: 163

```
Here she is:

http://ge.tt/4tNbzlm2
```

---
## \#447 Posted by: Vanarian Posted at: 2017-10-03T19:12:34.194Z Reads: 162

```
Man if we meet I owe you a drink.
```

---
## \#448 Posted by: Pimousse Posted at: 2017-10-04T08:31:44.826Z Reads: 159

```
@Vanarian an, Do you want to uncompile the 3.26 bin file to obtain source files ?
```

---
## \#449 Posted by: trampa Posted at: 2017-10-04T15:34:30.652Z Reads: 159

```
I just made tons of screenshots for those who struggle with the setup.
Step by Step through the Wizards...

http://www.vesc-project.com/node/20

Frank
```

---
## \#450 Posted by: Silverline Posted at: 2017-10-04T16:50:29.851Z Reads: 158

```
Nice with some dokumentation.... thumbs up :+1:

Any news about the R = 0 bug..... so i can follow your FOC tutorial ;-) ?
```

---
## \#451 Posted by: rok Posted at: 2017-10-04T22:44:36.704Z Reads: 163

```
I just updated my vesc from 4.12 to 3.29 and everything went with zero problemos. 

I just have this one issue of setting up my controler. I use a PPM(Benchwheel) controler with thumb throtle and i already set it up with wizard but for some reason the throtle distance that is available is very small. I know it prob has to do something with throtle curves that i know nothing about. 
Does anyone have any idea how to set the curves correctly, so that i can actually use the hole wheel of the throtle (i mean half of the wheel, backwards is ofcourse brake, which i think also needs adjusting). 
EXPANDING THE THROTLE. :point_left:
<img src="/uploads/db1493/original/3X/4/3/433bfe3424cf65301538f8febab334f4be266ac8.jpg" width="268" height="500">
```

---
## \#452 Posted by: BigBoyToys Posted at: 2017-10-04T22:50:17.321Z Reads: 154

```
If you used the app wizard I camt imagine why it wouldn't have all the range.
```

---
## \#453 Posted by: Jinra Posted at: 2017-10-04T22:53:36.952Z Reads: 155

```
Because 3.29 changed back to current control to fix the braking. A later version will likely have watt control back with fixed brakes.
```

---
## \#454 Posted by: trampa Posted at: 2017-10-05T06:33:15.779Z Reads: 156

```
@rok @Jinra  Has nothing to do with that. The VESC-Tool has never used "watt control" in the fist place.
You should have the entire throttle way anyway. The power distribution along the throttle way has something to do with your settings. Try setting Motor max Amp = Battery max Amps (if you battery is strong enough) for a linear power distribution along the entire throttle way. You will only get realistic results when you run the board under load. You can't see the result on the bench, since it is a current controlled system. 

Frank
```

---
## \#455 Posted by: Vanarian Posted at: 2017-10-05T14:25:53.636Z Reads: 156

```
@Pimousse Yes ! Even if not grouped correctly I could just arrange the sources. But I kinda filed to extract them for now so that's a stalemate.

@BigBoyToys Actually it is a different fork older than VESC 6 (creator started working on it since 4.8hw versions). Could still benefit from making a VESC 6 variant based on mines and it would work very good though. That's next step once I've ironed mines out and stressed them as much as I need (6xx can only do better IMO with same mods).

My units are LM5109 based (replace the DRVs, good up to 100V) and also have 6-FETs all on one face kinda like VESC 6 and FOCBOX so as easy to cool down. But I don't have Direct-FETs.

I also GPIOs assigned differently (probably due to modular layout, LM drivers + boot and reset buttont to switch between normal USB and DFU-USB connections).

@trampa That's not what @Ackmaniac said and he gains no money from saying it did till 3.28 version.
```

---
## \#456 Posted by: rok Posted at: 2017-10-05T15:01:58.944Z Reads: 153

```
Just did what you said and i noticed no difference. Time to take it for a spin outside, so that i have a better answer for you. 
Thanks though, very nice and user friendly tool! :relaxed:

TESTED
The throtle feels very different under load, i like it. I also like FOC. And turtles  :turtle: :wink: 

I do have one question tho regarding brakes. This may not be the vesc or software problem but rather my settings. When i pull the throtle way back it does break, but does so very slowly, and never totaly stops the motor from spinning. It doesn't blocks it completly is what i mean. How to fix it?
`I am running 10s4p with 200kv motor. I have a motor max set to 60A, brake max to -60A and regen to -16A.`
```

---
## \#457 Posted by: tueboard Posted at: 2017-10-05T16:09:05.512Z Reads: 155

```
i don't know if someone asked it before...

1- it's safe to use this new software with a vesc 4.12 ?

2- if you want to use it in a vesc 4.12 you have to upload another firmware?

thanks
```

---
## \#458 Posted by: Jinra Posted at: 2017-10-05T16:09:48.011Z Reads: 156

```
yes on both
```

---
## \#459 Posted by: trampa Posted at: 2017-10-06T07:19:11.199Z Reads: 162

```
Hi @rok, -16A is not a lot of current for the brakes, so don't expect to much. -60 for the motor regen doesn't help to much if your battery can only swallow 16A. This weakness is dominant at speed and will get better when you slow down.  At top speed your brakes will be limited to -16A, since the motor generates nearly at full system voltage.
The lower the voltage drops on the generator side, the more Amps the motor is allowed generate. 
On the battery side the VESC will scale up the voltage again, lowering the currents back to your 16A battery min value.
This means: If your motor generates 32A at 20V (=640W), your battery could be charged with e.g. 40V, 16A (=640W).

In consequence the battery min pretty much defines your brake power at high speed, while the motor min value becomes more dominant at low speed. The further you spread the values apart, the more you will experience a non linear behaviour of the brakes. 

I will try to make a Duty Cycle manual together with Benjamin to explain the matter in detail.
So do some test runs in an area where you face no obstacles to find your settings.
Battery min is the bottle neck for strong brakes at speed! This is why you want a strong battery pack allowing fast storage of energy. This is why you want a high P count.

The motor brakes will not stop your board totally! It gets better with sensors, but if your board doesn't move, your motor won't spin and can't generate electricity. If it doesn't generate electricity it doesn't create resistance.
VESC-Tool has a feature called "hand brake", actively braking your motor through the use of a current flow through the motor coils, blocking the motor from spinning up. This consumes energy from the battery!
You can't easily activate it from the remote at this stage. 

Frank
```

---
## \#460 Posted by: TarzanHBK Posted at: 2017-10-06T07:41:04.114Z Reads: 157

```
Did i miss the point why Ben can´t just programm the Vesc 6 braking behavior like the 4.12?
So you get the same experience with same settings like before?!
Brakes where beautiful and worked like a charm on 4.12.

My settings look like that on a dual 6355 drive with a 10s4p:
Motor -60A
Bat -12A
Brakes are nice and strong at all speeds and block the motor completly when standstill.

So shouldn´t be a problem to get the same results on VESC 6!
```

---
## \#461 Posted by: Eboosted Posted at: 2017-10-07T01:02:03.696Z Reads: 157

```
Hello guys, I uploaded an incorrect FW version, then in order to correct it I ticked on Show non-default firmwares and now I can't even connect.

I'm having an error Invalid seial port: \\.\COM6

Did I brick my VESC?

Update: I cycled power and now I can connect again, but I can't change the HW version, as soon as I click on connect the Hardware Version List deletes 4.12 and only shows the HW 48
```

---
## \#462 Posted by: Eboosted Posted at: 2017-10-07T01:07:11.849Z Reads: 156

```
How did you fix this issue, I'm having the same issue as you, I incorrectly uploaded the HW Version 48 instead on 4.12. I can't upload the 4.12 hardware version anymore, is there a trick?
```

---
## \#463 Posted by: Titoxd10001 Posted at: 2017-10-07T01:18:42.420Z Reads: 159

```
Download FW for HW 4.12 from vedder github. Use the custom file tab in VESC Tool to upload the firmware

Actually switched back to extended BLDC tool using this method
```

---
## \#464 Posted by: Eboosted Posted at: 2017-10-07T01:26:20.072Z Reads: 164

```
I downloaded VESC_default for hw_410_411_412 from Vedder Github, flashed the firmware and I'm still stuck on hardware 48. Any other ideas?

There are other firmware inside the hw_410_411_412 folder

VESC_0005ohm.bin
VESC_servoout.bin
VESC_ws2811.bin

Should I try those as well?
```

---
## \#465 Posted by: Titoxd10001 Posted at: 2017-10-07T01:30:16.600Z Reads: 162

```
If you upload BLDC firmware and back to vesc-tool firmware it might give you option for 412
```

---
## \#466 Posted by: Eboosted Posted at: 2017-10-07T01:34:54.946Z Reads: 172

```
I tried to use BLDC tool (old software) but I can't even connect, I'm getting this error:

The firmware on the connected VESC is too old. Please update it using a programmer

I'm getting worried, I could use some help
```

---
## \#467 Posted by: Titoxd10001 Posted at: 2017-10-07T01:40:20.011Z Reads: 166

```
After you uploaded BLDC tool firmware from vesc-tool, did you try uploading vesc-tool firmware again?
```

---
## \#468 Posted by: Eboosted Posted at: 2017-10-07T01:44:30.704Z Reads: 165

```
[quote="Titoxd10001, post:467, topic:32268, full:true"]
After you uploaded BLDC tool firmware from vesc-tool, did you try uploading vesc-tool firmware again?
[/quote]

I'm getting confused here bro, You mean uploading the Vedder Firmware 4.12 (from Github) twice using VESC tool?
```

---
## \#469 Posted by: Titoxd10001 Posted at: 2017-10-07T01:49:37.295Z Reads: 163

```
You said uploading file from GitHub didn't work. So it might be possible to upload old BLDC firmware just so you can get the option to switch back to vesc-tool 412 firmware.
```

---
## \#470 Posted by: Eboosted Posted at: 2017-10-07T02:12:45.874Z Reads: 171

```
What I tried is to upload the old BLDC firmware which I downloaded from Github, after uploading it I couldn't select a different hardware just 48.

Ussualy when the firmware is uploaded the VESC reboots itself and you are able to connect in this case when I upload the formware I get disconnected and it's not possible to connect unless I cycle the power from the battery, I wonder if this could cause a failure in the firmware upload.

After I cycle the power I can confirm the FW wasn't uploaded succesfuly.

[img]https://i.imgur.com/uTH35s8.jpg[/img]

I uploaded original 2.18 FW for HW 4.10_4.11_412 
I uploaded ackmaniac 2.54
I uploaded ackmaniac 2.53
I uploaded ackmaniac 2.52

Non e of them worked
```

---
## \#471 Posted by: Surfer Posted at: 2017-10-07T02:24:50.110Z Reads: 163

```
Did you try with st Link programmer?
```

---
## \#472 Posted by: Eboosted Posted at: 2017-10-07T02:26:34.558Z Reads: 163

```
That's what I'm doing right now, I'm trying to find the instructions on them. Furtunately I have an ST Programmer here with me
```

---
## \#473 Posted by: Titoxd10001 Posted at: 2017-10-07T06:13:31.301Z Reads: 158

```
Focbox fried?
```

---
## \#474 Posted by: Eboosted Posted at: 2017-10-07T06:27:43.880Z Reads: 173

```
Hey @Titoxd10001 thanks for your help! Thanks also to @Surfer

I was able to recover my VESC via the ST Link programmer, I'm so happy o bought it from eBay months ago, I might need it sometime, I said a while back.

We'll the issue was, once you program the incorrect hardware version you won't be able to go back to an older firmware, when flashing the firmware you will also flash the bootloader, an incorrect bootloader won't let you flash an old firmware, do you get stuck with a bricked VESC.

The solution is to program an 4.12 FW with a ST-Link and after successfully installing the FW, flash the the Hex file which contains the bootloader, at the beginning o tried to flash the bin file FW only but couldn't update the firmware so after flashing the Hex file everything went back to normal.

Finding the procedure to connect the st link was not easy, I had to watch a video from Jared and then find out the pinout to connect the ST-Link to the VESC, you just need to connect 4 cables 3.3v, GND, SWDIO and SWCLK, all commercial VESCs have these pins labeled at the back of the board, so don't look for a pinout online, you will loose time as me, just plug them with the supplied wires.
```

---
## \#475 Posted by: Titoxd10001 Posted at: 2017-10-07T07:42:47.621Z Reads: 166

```
Strange you had to go through all those steps I was able to change firmwares from vesc-tool. Thought the wrong firmware was the reason your board caught fire
```

---
## \#476 Posted by: Eboosted Posted at: 2017-10-07T14:42:05.076Z Reads: 165

```
Those firmware issues were on my Vanguard build, it's running good now.
```

---
## \#477 Posted by: DimiDec95 Posted at: 2017-10-08T14:03:05.064Z Reads: 166

```
The website seems to be offline to me. Are you guys able to go on it?
```

---
## \#478 Posted by: Silverline Posted at: 2017-10-08T14:10:25.842Z Reads: 166

```
Every time i try that site its always offline
```

---
## \#479 Posted by: DimiDec95 Posted at: 2017-10-08T14:11:58.485Z Reads: 165

```
Damn that sucks. Does anyone have a copy of the latest FW for HW4.12?
```

---
## \#480 Posted by: trampa Posted at: 2017-10-08T14:50:07.607Z Reads: 167

```
Benjamin installs a new powerful server. The site will be online soon. 

Frank
```

---
## \#481 Posted by: qdxiatao Posted at: 2017-10-08T15:51:09.672Z Reads: 163

```
when will the reference hardware design be relleased?
```

---
## \#482 Posted by: ThierryGTLTS Posted at: 2017-10-12T16:57:59.221Z Reads: 164

```
To Frank and Benjamin.

vesc-project.com is down another time.

It seems that the new server didn't solve the problem.

Hope you will find a lasting solution.

Have a Nice Day.

Thierry
```

---
## \#483 Posted by: trampa Posted at: 2017-10-12T17:02:31.602Z Reads: 168

```
It's still on the old one. Online soon...

Frank
```

---
## \#484 Posted by: trampa Posted at: 2017-10-12T20:40:45.666Z Reads: 170

```
When it is back online tonight it's on the new server and fast fibre connection.

Frank
```

---
## \#485 Posted by: Tomer Posted at: 2017-10-16T16:14:48.156Z Reads: 172

```
I just want to confirm the procces of uploading a bootloader to a VESC without a bootloader.

Which version should I choose? 40 & 47 and so on... or the 60?
Then, I should just hit the download button?

<img src="/uploads/db1493/original/3X/d/7/d7957379cdd8faa8e5e54e237f83aa2f0731e53d.png" width="690" height="439">

I tried to search for an answer but couldn't find one, I don't want to mess the VESC... 

Thanks!
```

---
## \#486 Posted by: onepunchboard Posted at: 2017-10-16T16:23:20.008Z Reads: 174

```
Trampa is only maker of ver. 60 @ the moment
```

---
## \#487 Posted by: onepunchboard Posted at: 2017-10-16T16:27:30.432Z Reads: 173

```
@BigBoyToys, managed to use ver 3.26 for my focbox. Thanks

Something must have happened to 3.27 and onward,

@trampa how do I activate, handbrake function? fmw3xx has much better braking power, but also wants to try and decide.
```

---
## \#488 Posted by: Tomer Posted at: 2017-10-17T12:35:25.312Z Reads: 173

```
So I should choose 60 and will be just fine? We are talking on a Maytech VESC btw.
```

---
## \#489 Posted by: rich Posted at: 2017-10-17T13:48:23.354Z Reads: 174

```
60 is vor VESC SIX HW only! You have to choose the first option, I did it with HW 4.12, easy!
```

---
## \#490 Posted by: Tomer Posted at: 2017-10-17T20:12:45.725Z Reads: 174

```
Thanks!

So I uploaded a bootloader (I hope so). To make sure, I want to update the firmware.
My Maytech VESC hardware is 4.12, so in VESC Tool I should choose 410 & 411 & 412, correct?

<img src="/uploads/db1493/original/3X/f/2/f2c1c5ef3e9c06d25c8354c250d4b99ab875ad1a.png" width="690" height="387">
```

---
## \#491 Posted by: Silverline Posted at: 2017-10-17T20:16:18.864Z Reads: 167

```
Yes .... 10 char
```

---
## \#492 Posted by: trampa Posted at: 2017-10-17T20:16:44.896Z Reads: 169

```
Correct! Don't FOC it it up, stay with BLDC if you can. The maytechs are reported to have FOC issues.

Frank
```

---
## \#493 Posted by: Tomer Posted at: 2017-10-17T20:19:46.862Z Reads: 175

```
Will never try... :joy:
I'll sell it one day and get a better quality VESC with FOC compatibility. 

Succes.
<img src="/uploads/db1493/original/3X/4/b/4bb47cfd13fc11f568be326b2ca101826eb24593.png" width="690" height="29">

So if I was able to update the firmware, I assume this VESC has a bootloader now. :innocent:
```

---
## \#494 Posted by: trampa Posted at: 2017-10-17T20:33:06.231Z Reads: 176

```
Yes it has a bootloader now. You can still try FOC with low KV motors and pushing not more than 40A on the motor side.

Frank
```

---
## \#495 Posted by: Tomer Posted at: 2017-10-17T20:39:13.477Z Reads: 176

```
My motors are 210 KV so I guess I shouldn't test it.

By the way, is it possible to downgrade the firmware back to 2.18?
```

---
## \#496 Posted by: trampa Posted at: 2017-10-17T21:59:00.376Z Reads: 175

```
Yes, you can upload the 2.18 FW through the custom FW tab.

Frank
```

---
## \#497 Posted by: telnoi Posted at: 2017-10-18T10:44:18.981Z Reads: 178

```
How is sensorless foc?
Currently using BLDC, but I have the typical cogging if I don't move the board forward slightly upon startup.
```

---
## \#498 Posted by: rok Posted at: 2017-10-18T11:07:18.445Z Reads: 177

```
Its pretty good, i'm on sensorless FOC. Almost zero cogging.
```

---
## \#499 Posted by: landonkun Posted at: 2017-10-19T00:26:18.146Z Reads: 174

```
Just a heads up, doing it the way you showed in your screenshot did NOT upload a bootloader to my Maytech vesc. I had to click on the Bootloader tab and do it that way. I would test to make sure.
```

---
## \#500 Posted by: Tomer Posted at: 2017-10-20T13:23:58.172Z Reads: 175

```
Sorry, didn't quite get it. 
What did you encounter when you tried to upload the bootloader via the tool?
```

---
## \#501 Posted by: Silverline Posted at: 2017-10-20T19:41:31.038Z Reads: 171

```
Heads Up regarding R = 0 bug on focbox : http://vesc-project.com/comment/863#comment-863
```

---
## \#502 Posted by: trampa Posted at: 2017-10-20T20:17:16.756Z Reads: 177

```
Benjamin thinks its sorted. There are also some other tweaks he has done.
The input wizard should be much better now.

The next thing to be implemented is a big thing for all of us! 
A new control mode that will change the way we control our power quite drastic. Surprise surprise....

Frank
```

---
## \#503 Posted by: Jinra Posted at: 2017-10-20T20:19:04.831Z Reads: 171

```
[quote="trampa, post:502, topic:32268"]
A new control mode that will change the way we control our power quite drastic. Surprise surprise....
[/quote]

sounds like he's just turning on watt control again after turning it off from 3.29?
```

---
## \#504 Posted by: trampa Posted at: 2017-10-20T20:38:18.063Z Reads: 174

```
Watt control was never implemented and will never be. Benjamin's opinion about that is quite clear.
We are talking something completely different.

Frank
```

---
## \#505 Posted by: MontPierre Posted at: 2017-10-20T20:39:43.956Z Reads: 175

```
Any sort of timeline on the “surprise”?? I’m getting excited!
```

---
## \#506 Posted by: Jinra Posted at: 2017-10-20T20:39:51.774Z Reads: 175

```
@Ackmaniac ^
```

---
## \#507 Posted by: ThierryGTLTS Posted at: 2017-10-21T11:00:22.227Z Reads: 173

```
Hope it'll be interesting for e-bikes too!!!

Thierry
```

---
## \#508 Posted by: trampa Posted at: 2017-10-21T15:22:29.065Z Reads: 174

```
Oh yes, big time.

Frank
```

---
## \#509 Posted by: ThierryGTLTS Posted at: 2017-10-29T13:05:20.724Z Reads: 167

```
Thanks Frank, and special thanks to Benjamin.

Just tested the 0.84 version with all ADC options, works great.

Thierry
```

---
## \#510 Posted by: trampa Posted at: 2017-10-29T21:11:27.963Z Reads: 171

```
I just updated the manuals on the VESC-Project website: http://www.vesc-project.com/node/178

Benjamin added a new important Feature called ATD.
"Acceleration Temperature Decrease" is a powerful new safety feature and should be used straight away.

http://www.vesc-project.com/node/221

Please have a look at:

Additional settings: Throttle curves, ERPM limits, safety features etc.

http://www.vesc-project.com/node/183

Frank
```

---
## \#511 Posted by: telnoi Posted at: 2017-10-31T10:03:04.461Z Reads: 171

```
Updated, working great.
Suggestion: programmable delay/interpolation or curve for throttle down. As I improve my riding skills and get used to my board, I noticed it tends to throw me forward a bit if I decrease throttle too quickly, since the rough terrain has a constantly changing impact on the rolling resistance it is still difficult to predict what it will do. Now that I am aware of it, I slowly decrease throttle but it would be nice if you can program it to slowly decrease RPM when the throttle is reduced, instead of instantly targeting the new RPM. Don't want that for throttle up.

On a different note, could someone explain why my braking strength is poor when using:
motor max 70
motor min -70
battery regen -10

and good when just changing motor max and min to 60 and -60 respectively? The difference is massive.
```

---
## \#512 Posted by: trampa Posted at: 2017-10-31T15:12:39.632Z Reads: 170

```
If you use PPM you can drop in softer values for the ramping delay. Default is 0.3 and 0.1s (acceleration and brake). Try 0.9 and 0.3s.

-70 might cause stator saturation. 
-10 battery min is very low. Battery min determines the max. braking force at speed (high duty cycle).

Frank
```

---
## \#513 Posted by: ThierryGTLTS Posted at: 2017-10-31T16:23:05.088Z Reads: 174

```
Hi Frank,

In the Help inside VESC Tool, we can read this: "Current control. The output is off when the input is at minimum."

Does it mean that the Output is in High impedance, and/or the controller is in idle/sleep mode?!

I ask this because when in standalone "ADC only App", when I set the potentimeter to 0, the controller consumption is still high, and the motor seems in braking mode (hard to manually rotate) altough I've choosen "simple current mode", no braking or reverse.

Have a Nice Day.

Thierry
```

---
## \#514 Posted by: telnoi Posted at: 2017-10-31T17:18:08.967Z Reads: 170

```
Ramping delay is currently not decoupled for acceleration and braking. Would be a great addition (for me at least).
I have -10 battery min x 2 (dual drive), so far it has been sufficient at motor min -60. I will increase it once I throw out the old li-ion.
```

---
## \#515 Posted by: Jinra Posted at: 2017-11-01T17:13:55.948Z Reads: 174

```
for <v3.3 I had to double my observer gain in FOC to not get over current faults all the time. Do I still need to do that now that 3.3 says this?

>=== FW 3.30 ===
* Activated iterative observer for better operation at high ERPM.
* Check for NAN and truncate some FOC variables.
* Speed controller windup protection improvement
```

---
## \#516 Posted by: telnoi Posted at: 2017-11-23T18:55:45.800Z Reads: 169

```
Switched from BLDC to FOC and the brakes behave differently.
With BLDC, I could precisely control the brake strength with my remote (current no reverse with brake). The further I would pull the leaver into the negative direction, the stronger the brake was.

With FOC, it just appears to go to 100% brake strength immediately.
Firmware 3.31, FOCBOX

Anything I can do to get the old behaviour back whilst using FOC?

edit: just double checked again with BLDC, and the brakes are progressive as opposed to FOC where it's either 100% or nothing.
```

---
## \#517 Posted by: trampa Posted at: 2017-11-24T19:58:45.264Z Reads: 171

```
@teknoi, you need to post your settings to get a relevant answer. I never experienced anything like that. The brakes should be linear in FOC. It depends on your settings though.

Frank
```

---
## \#518 Posted by: telnoi Posted at: 2017-11-24T20:11:20.097Z Reads: 168

```
* dual focbox 3.31
* sk3 149kv

* motor current max 80 A
* motor current max brake -60 A
* Absolute Max current 130 A

* Battery Current Max 50 A
* Battery Current Max Regen -15 A

* PPM current no reverse w brake. Center, min and max correctly configured.

Everything else defaúlt. FOC startup is fine (much better than unsensored BLDC).

Brake test was indoors at very low speed testing startup from a stand still. Just noticed there that the brake strength never changes according to how hard I brake with the controller, where BLDC offers very precise control (not sure if low speed is a determining factor here).
```

---
## \#519 Posted by: egzplicit Posted at: 2017-11-24T21:21:27.562Z Reads: 159

```
[quote="telnoi, post:518, topic:32268"]
Brake test was indoors at very low speed testing startup from a stand still.
[/quote]

This is the problem. When reaching very low speeds, just before stopping, it shorts two of the phasing wires. Try outside from 5km+ speed and it should be fine.
```

---
## \#520 Posted by: trampa Posted at: 2017-11-24T21:37:50.728Z Reads: 167

```
The more you spread apart the Motor Max Brake and Battery Max Regen, the less linear the brake will be. 
The -15A pretty much define the brake force at high speeds, while the -60A Motor Max Braking are getting dominant at low speed. You can compensate that a bit, using the throttle curves, but it is better do use values closer to another.
Your battery needs to be able to cope with the currents you shoot towards it. This is why you want many cells in parallel.
Try riding your board with motor and battery values being the same, then spread apart the values. You will see how this affects linearity. 

Frank
```

---
## \#521 Posted by: chinzw Posted at: 2017-11-24T22:14:09.889Z Reads: 164

```
Why is it that everyone is complaining about the brakes with VESC Tool, but no one had any issues wth BLDC Tool. I don't get it. I have the exact same values that i used on bldc tool, and the brakes are not even close to the same strength as they used to be.
```

---
## \#522 Posted by: trampa Posted at: 2017-11-24T22:52:23.957Z Reads: 168

```
Brake strength depends on how many Amps you allow to be generated and how much your battery can eat Amp wise.
Whatever energy you generate needs to be stored, since the energy can't be evaporated into the universe. If you are at top speed and your motor generates at full voltage (e.g. 40V) and your Battery Regen is -15A, that results in 600W braking power. If you want more braking power you need to set higher Battery Regen values. 
Neither BLDC-Tool, nor VESC-Tool can do magic and evaporate the energy. The amount of braking power is always equivalent to the energy you shoot towards your battery. Since the motor we use are about 85-90% efficient, only a small fraction is converted into heat. VESC-Tool is more precise, so the values you specify resemble the output in real world a lot better. 

Frank
```

---
## \#523 Posted by: chinzw Posted at: 2017-11-24T22:57:28.682Z Reads: 172

```
This is the same reply you posted over and over again. I'm pretty sure we all understand this. But here's the catch: 

**The new firmware has less braking power than the old firmware with the exact same parameters.**

That is what i want an answer for.
```

---
## \#524 Posted by: telnoi Posted at: 2017-11-27T06:32:58.272Z Reads: 168

```
Will give it a shot during the weekend. Thanks for the help.
```

---
## \#525 Posted by: TarzanHBK Posted at: 2017-11-27T07:40:26.836Z Reads: 174

```
so whats different with Vesc tool and the old BLDC tool that brakes changed?
```

---
## \#526 Posted by: trampa Posted at: 2017-11-27T21:45:51.395Z Reads: 188

```
<img src="/uploads/db1493/original/3X/f/a/fa10d7553762bbd1d582b01d1e3043b413da78b6.jpg" width="690" height="490">

http://vesc-project.com/node/234

Frank
```

---
## \#527 Posted by: fedestanco Posted at: 2017-11-28T13:02:35.754Z Reads: 183

```
Hi Frank,
do you have a link where one can find previous versions of the vesc tool? I need the version supporting 3.29 firmware in order to tune [these BMS'](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639)s configuration.
```

---
## \#528 Posted by: trampa Posted at: 2017-11-28T13:24:41.490Z Reads: 184

```
You will have to ask Benjamin on the VESC-Project forum. A direct Link is not available.
Do you need the executable for Windows or Linux?

Frank
```

---
## \#529 Posted by: fedestanco Posted at: 2017-11-28T13:33:18.718Z Reads: 187

```
Windows. 
10 characters
```

---
## \#530 Posted by: trampa Posted at: 2017-11-28T14:44:45.447Z Reads: 191

```
Send me a PM with your e-mail.

Frank
```

---
## \#531 Posted by: BigJerm Posted at: 2017-12-12T06:14:52.937Z Reads: 188

```
Is there a vesc tool for mac?
```

---
## \#532 Posted by: squad Posted at: 2017-12-12T07:32:32.368Z Reads: 188

```
Thanks to @rpasichnyk there is!

 https://github.com/rpasichnyk/vesc_tool/releases
```

---
## \#533 Posted by: twan Posted at: 2017-12-22T05:35:24.953Z Reads: 183

```
Sooo did anyone ever figure out why the breaks are so much weaker than BLDC tool on same settings?
```

---
## \#534 Posted by: onepunchboard Posted at: 2017-12-22T05:43:38.565Z Reads: 182

```
i got no prob with break. im with acmaniac ver. and also og vesc tool. no problem. i set batt min to25
```

---
## \#535 Posted by: ducktaperules Posted at: 2017-12-22T09:45:06.975Z Reads: 182

```
so im running the newest firmware avalable from VESC Tool but i was wondering if there are any apps that support this yet? the best that i have found is @Ackmaniac app in which some things work and some dont. are there any apps that work properly with these firmware's right now?
```

---
## \#536 Posted by: Eboosted Posted at: 2017-12-24T04:06:23.222Z Reads: 183

```
[quote="ducktaperules, post:535, topic:32268"]
the best that i have found is @Ackmaniac app in which some things work and some dont.
[/quote]

What does not work on @ackmaniac FW? I'm running it and have no issues whatsoever
```

---
## \#537 Posted by: Tampaesk8er Posted at: 2018-01-01T19:21:04.197Z Reads: 180

```
Im having issues updating the firmware in the new vesc tool software, after it keeps telling me that i need a programmer to do it, when i do fw update in old bldc tool, i have no issues updating. im using a maytech vesc with bootloader installed in it, i dont want to use achmaniacs software, just want to keep it simple. any suggestions would help.
```

---
## \#538 Posted by: trampa Posted at: 2018-01-01T19:53:49.107Z Reads: 179

```
Have you tried to upload the new FW? 

Frank
```

---
## \#539 Posted by: Tampaesk8er Posted at: 2018-01-01T21:10:27.414Z Reads: 180

```
Thats the issue, Im having issues updating the firmware in the new vesc tool software, after it keeps telling me that i need a programmer to do it, when i do fw update in old bldc tool, i have no issues updating. im using a maytech vesc with bootloader installed in it, i dont want to use achmaniacs software, just want to keep it simple. any suggestions would help.
```

---
## \#540 Posted by: trampa Posted at: 2018-01-01T23:21:30.451Z Reads: 178

```
Actually it should work, so something is funny with your bootloader. 

Frank
```

---
## \#541 Posted by: Tampaesk8er Posted at: 2018-01-02T00:06:43.580Z Reads: 177

```
What should i do, any ideas?
```

---
## \#542 Posted by: trampa Posted at: 2018-01-02T07:59:32.999Z Reads: 180

```
Ideally you want to get yourself a ST-Link V2.
They cost 3-8$ on eBay.

Frank
```

---
## \#543 Posted by: Tampaesk8er Posted at: 2018-01-02T22:53:44.881Z Reads: 178

```
i’m gonna order one, thank you.
In the old bldc tool, when i setup F.O.C mode, what battery settings would be good for cuttoff and end cuttoff for a 10s2p 36v (max. 42V)?
```

---
## \#544 Posted by: TarzanHBK Posted at: 2018-01-03T07:37:43.617Z Reads: 179

```
for all 10s liion batteries:
start cutoff 30V
end cutoff 28V
```

---
## \#545 Posted by: trampa Posted at: 2018-01-03T16:21:00.608Z Reads: 179

```
I would say 3.1V cut off (hard cutoff) is healthy. If you go lower, battery life will suffer. At 3.1V the cell is 95% empty. 

Frank
```

---
## \#546 Posted by: PXSS Posted at: 2018-01-03T17:07:14.363Z Reads: 182

```
Negative. 
It depends on the cell but for 30Qs 3.1v cutoff is 75-85% depleted depending on current draw, 2.8V is 85-95% depleted depending on current draw. The more current you draw, the sooner you’ll hit the limit because of voltage sag and the less percentage will be used.
```

---
## \#547 Posted by: Hansg Posted at: 2018-01-04T21:11:59.621Z Reads: 182

```
do you know if is posibble return to firmware previous. For example if i have the firmware 2.18 i update to 3xx. What diference do you have between firmware 2.18 and the last.
```

---
## \#548 Posted by: trampa Posted at: 2018-01-05T00:48:05.903Z Reads: 184

```
I would recommend to update to the latest FW. 2.18 is outdated. You can upload custom FW from the custom FW tab if you want to downgrade.

Frank
```

---
## \#549 Posted by: Tampaesk8er Posted at: 2018-01-05T21:48:02.211Z Reads: 189

```
Ok, ordered the st link v2, gettn it next week.
now, in f.o.c. (old bldc tool) what are safe numbers for a mono 6374 149kv 10s2p- (Motor max, motor min. regen and Batt. max. Amps, Batt. min. Amps regen)? as always, thanks to all who always help.
```

---
## \#550 Posted by: trampa Posted at: 2018-01-05T22:05:21.533Z Reads: 193

```
I would use 45A max for the Motor and Battery (same value for both if your Battery can handle that). Regen depends on your battery pack. 25-30A regen should be no issue for the HW 4.12. Maytech and FOC gives some users mixed emotions.  Low KV motor and low Amp settings certainly helps to keep the ESC alive. 

Frank
```

---
## \#551 Posted by: Tampaesk8er Posted at: 2018-01-06T13:02:39.435Z Reads: 194

```
** THIS THREAD EXPLAINS THE EXACT SAME ISSUES THAT IM HAVING WHEN I TRY TO UPDATE THE FIRMWARE IN THE NEW VESC TOOL SOFTWARE **

http://vesc-project.com/node/175#forum-topic-top
```

---
## \#552 Posted by: trampa Posted at: 2018-01-07T16:24:28.082Z Reads: 192

```
Well, your ESC has no Bootloader I guess, and I woud simply upload it via VESC-Tool. Worst case outcome if you mess up the botloader section: you need to buy a 3€ ST-Link from Ebay. 

Frank
```

---
## \#553 Posted by: Tampaesk8er Posted at: 2018-01-07T23:49:14.865Z Reads: 190

```
i ordered it from ebay, it comes in this wk. thanks for your help.
```

---
## \#554 Posted by: trampa Posted at: 2018-01-08T10:57:41.671Z Reads: 192

```
You don't need it if the bootloader upload works.

Frank
```

---
## \#555 Posted by: Tampaesk8er Posted at: 2018-01-10T01:07:32.931Z Reads: 201

```
Ok, but it came in today.
![image|669x500](upload://q1p6xifKJLjawQVnH8EwLVOMvY5.jpeg)
```

---
## \#556 Posted by: Tampaesk8er Posted at: 2018-01-11T10:21:49.573Z Reads: 199

```
Can you tell me how to connect the stlink? i dont know where to connect wires (colors) to the st link.
```

---
## \#557 Posted by: trampa Posted at: 2018-01-11T11:03:53.370Z Reads: 205

```
1. Download STlink Utility (http://www.st.com/en/embedded-software/stsw-link004.html)
2. Download the last FW from Benjamin for HW4.12 http://vedder.se/forums/download/file.php?id=6
3. Install STlink Utility (it is inlc. drivers for the STlink)
4. Connenct the STlink to the Vesc with only 3 Pins SWDIO --> IO, GND --> GND, SWCLK --> CLK (NEVER connect the 3.3v pin, RTS no need)
5. Power on the Vesc
6. Open STlink Utility
7. Open the tap TARGET and klick Connect --> the program show you the infos of your VESC
8. Open the Tap FILE and klick open --> search for the file "VESC_default.bin" and select (base address is 0x080E0000)
9. Use the write button (The second on the right)
10. Press Start at the open window --> the programm will flash your Vesc
11.After finisch close the Programm, power off your Vesc and disconnect the STlink
12. Connect the Vesc via USB and open the Vesc Tool to upgrade the FW

Frank
```

---
## \#558 Posted by: Tampaesk8er Posted at: 2018-01-13T23:39:39.935Z Reads: 198

```
  Everything is working excellent now, i really like this new vesc tool, much easier to set everything up, now i can teach my son how to work this new vesc tool, the older software was difficult for him to learn.

I really want to setup F.O.C. but the vesc tool has my battery currents at 34v start cuttoff and 31v end cuttoff, is that safe for foc on a turnigy 6374 149kv?
```

---
## \#559 Posted by: rich Posted at: 2018-01-13T23:58:14.586Z Reads: 195

```
The battery cut off settings are not relevant for FOC but the problem is the maytech hw, you should run BLDC mode only (I tried FOC and can't recommend it)
```

---
## \#560 Posted by: Tampaesk8er Posted at: 2018-01-14T21:58:07.956Z Reads: 192

```
Thank you. What was your experience with foc and maytech vesc, what kind of issues did you have? just curious.
```

---
## \#561 Posted by: rich Posted at: 2018-01-15T14:27:42.482Z Reads: 185

```
Multiple faults and dropouts for several seconds everytime when hitting the brake (even with no load).
```

---
## \#562 Posted by: Surfer Posted at: 2018-01-15T14:29:52.561Z Reads: 184

```
Exactly the same, in blcd rocks
```

---
## \#563 Posted by: Tampaesk8er Posted at: 2018-01-15T17:56:45.856Z Reads: 179

```
Scary. Ok, thanks, bldc it is.
```

---
## \#564 Posted by: gicho Posted at: 2018-01-15T22:08:35.088Z Reads: 181

```
I upgraded my focbox to 3.34 but now having problems with motor detection in bldc mode. It is spinning up the 6374 190kv motor but failing with bad detection result received. Anyone else run into this issue?
```

---
## \#565 Posted by: SpeedyGonzales Posted at: 2018-01-16T12:07:37.719Z Reads: 178

```
Thank you for that.
```

---
## \#566 Posted by: Silverline Posted at: 2018-01-21T17:23:00.167Z Reads: 175

```
Hallo Guys...

Being out of the game for a while. 
With the newest vesc tool /firmware. Is it safe now to run FOC mode on my focboxes ?  (10s build - sk3 6364/190kv) And is the foc motor detection working now for focbox ? Last time i tried , it didn't
Thanks...
```

---
## \#567 Posted by: DK-Odense Posted at: 2018-01-21T17:59:46.607Z Reads: 171

```
Bare se at få den smidt i FOC inden onsdag 😁
```

---
## \#568 Posted by: Silverline Posted at: 2018-01-21T18:06:27.958Z Reads: 174

```
@DK-Odense 
Det var også planen, så det kunne testes / prøves :-)  Men hvis det stadig er lidt beta. Gider jeg ikke ændre endnu, når jeg ved nuværende spiller for mig :slight_smile:
```

---
## \#569 Posted by: Eboosted Posted at: 2018-01-21T18:58:28.283Z Reads: 183

```
Try to raise the low duty current from 0.05 to 0.1
```

---
## \#570 Posted by: Pimousse Posted at: 2018-01-24T12:02:29.361Z Reads: 185

```
Good news : FW 3.34 is now commited on Github. :slight_smile:
```

---
## \#571 Posted by: H_man Posted at: 2018-01-29T09:50:53.558Z Reads: 189

```
Hi, does anyone have the PCB Gerber files for the VESC 4.12 they are willing to share with me? I'm trying to build my own vesc but cannot find any of the PCB files

Thanks.
```

---
## \#572 Posted by: TarzanHBK Posted at: 2018-01-29T09:55:17.587Z Reads: 184

```
https://oshpark.com/shared_projects/ztyE14yF
```

---
## \#574 Posted by: trampa Posted at: 2018-03-21T11:21:47.595Z Reads: 168

```
www.vesc-project.com
```

---
## \#575 Posted by: hyperIon1 Posted at: 2018-03-21T12:18:47.428Z Reads: 166

```
Up your volts to 10 only for the o
```

---
## \#576 Posted by: Blitz Posted at: 2018-03-21T12:33:27.773Z Reads: 166

```
So Guys is this new tool safe or should we stick to the old one? 
Will use focbox  9s in foc
```

---
## \#577 Posted by: JohnnyMeduse Posted at: 2018-03-21T12:52:03.413Z Reads: 170

```
Or use @Ackmaniac :wink:, found out that the brake are also more reliable
```

---
## \#578 Posted by: hyperIon2 Posted at: 2018-03-21T14:00:06.198Z Reads: 164

```
I will check it out.
```

---
## \#579 Posted by: Silverline Posted at: 2018-03-21T19:39:29.120Z Reads: 167

```
Can du describe the difference in the brake feel vesc-tool vs. acmaniacs ? I hate the way the brake feels at low rpm`s on the vesc-tool fw (handbrake thing)
```

---
## \#580 Posted by: Deckoz Posted at: 2018-03-21T20:13:16.555Z Reads: 175

```
In bldc tool and Ack firmware, the braking is progressive.

The standard vesc tool tried to use the full battery negative at all times. 

Meaning as duty cycle goes down amps don't increase to the equivalent wattage capable on motor min. meaning your brakes get weaker the slower you go.

Ie 
Bldc tool /ack esc tool
Motor min -40
Battery min -15

At high rpms braking will be around 15amps, and as duty cycle decreases motor amp regen increases to create the same wattage/torque and progressively slow you down

Stock vesc tool
Battery min -15
Doesn't matter what your motor min is, it won't go above -15 amps, so at low duty cycle you get weak brakes
```

---
## \#581 Posted by: Silverline Posted at: 2018-03-21T20:29:41.013Z Reads: 166

```
What about the handbrake thing ?
```

---
## \#582 Posted by: Deckoz Posted at: 2018-03-21T20:31:24.117Z Reads: 164

```
Handbrake is magnetic flux linkage(position) holding at full stop.

Same between both.
```

---
## \#583 Posted by: Silverline Posted at: 2018-03-21T20:35:55.266Z Reads: 164

```
Hmm okay.... i don`t like it... but i guess i could get use to it.
```

---
## \#584 Posted by: Deckoz Posted at: 2018-03-21T20:37:13.187Z Reads: 165

```
Use an encoder instead of a hall sensor...
```

---
## \#585 Posted by: Silverline Posted at: 2018-03-21T20:44:48.601Z Reads: 162

```
No i mean the handbrake function, introduced in newer vesc-tool firmwares, wich kicks in between 1500 to 0 rpms
```

---
## \#586 Posted by: telnoi Posted at: 2018-03-21T20:56:11.529Z Reads: 165

```
There is supposedly an error in the gui of the vesc tool that does not expose this parameter. Informed frank via this forum, but never received a reply. I use bldc which does not suffer from that issue for some reason.
```

---
## \#587 Posted by: Silverline Posted at: 2018-03-21T21:08:38.400Z Reads: 165

```
Yeah exactly..... i want to change the value..... But i guess it`s the same thing in the Acmaniac fw then ?
```

---
## \#588 Posted by: Deckoz Posted at: 2018-03-21T21:13:19.805Z Reads: 167

```
Yes I know. 

I'm stating it doesn't work well unsensored or with hall sensors. Encoders it holds perfectly...

If you want to change the parameter not in the GUI..just save the XML backup edit it and restore it..
```

---
## \#589 Posted by: Silverline Posted at: 2018-03-21T21:31:30.568Z Reads: 158

```
Yes i know i could do that. But i Was hoping it was made easier in ackmaniack tool
```

---
## \#590 Posted by: Deckoz Posted at: 2018-03-21T21:39:05.119Z Reads: 162

```
Ah..

Either way it still sucks unsensored or with hall sensors... Might as well not even use it unless you have encoders...
```

---
## \#591 Posted by: Silverline Posted at: 2018-03-24T18:25:54.297Z Reads: 160

```
Anybody knows where i can find the release notes for the new vesc-tool/fw 0.89 ??
In other words, what is the difference between 0.88 and 0.89 ??

Thanks
```

---
## \#592 Posted by: fraannk Posted at: 2018-03-24T18:41:44.386Z Reads: 158

```
What does the 2.18 firmware do in regards to the brakes? I'm about to upgrade, and I want it to feel like it does now. Ackmaniacs or stock?
```

---
## \#593 Posted by: trampa Posted at: 2018-03-24T20:00:27.038Z Reads: 158

```
Help >> VESC Tool changelog.

![Change log - Kopie|690x369](upload://6WcGFKKC5BBwhDls7OsIpKk296F.jpg)
```

---
## \#594 Posted by: Silverline Posted at: 2018-03-24T20:01:03.221Z Reads: 153

```
Gotcha.... Cool thanks 😀
```

---
## \#595 Posted by: trampa Posted at: 2018-03-24T20:07:33.109Z Reads: 158

```
Try stock with motor current max brake = battery current max regen, and you will have very nice and linear brakes.
```

---
## \#596 Posted by: fraannk Posted at: 2018-04-02T15:04:42.557Z Reads: 156

```
FOC me, FOC was easy to setup with the new wizards.... Works on my FOCBOX'es. However, it seems to spin up in a weird way. When NOT going easy on the throttle, it spins the motor really slowly, and after a sec or so, I hammers to full speed. Why does it have that 1 sec of spinning really slow? Is it the Positive Ramping time? If so, I would definitely not call that a "ramp". :P The motors are 230Kv uncensored btw. I ran these tests on 4s.
```

---
## \#597 Posted by: trampa Posted at: 2018-04-02T15:06:20.111Z Reads: 154

```
Under strain or on the bench? You need load to figure it out.
```

---
## \#598 Posted by: fraannk Posted at: 2018-04-02T16:50:40.180Z Reads: 155

```
Oh, okay. It was on the bench, so I'll try with some load, thanks :)
```

---
## \#599 Posted by: fraannk Posted at: 2018-04-08T19:47:04.431Z Reads: 153

```
When reading the calculated Kv of the motor, I get this value: ![Capture|492x159](upload://gdxVSdCxHS0bd2bJxAnTUqF81AN.PNG)

How do I get the actual Kv value?
```

---
## \#600 Posted by: RedEagle Posted at: 2018-04-08T19:58:15.719Z Reads: 150

```
First spin up the motors with arrow keys or remote. Then try again.
```

---
## \#601 Posted by: fraannk Posted at: 2018-04-08T20:07:13.398Z Reads: 146

```
That worked. Thank you!
```

---
## \#602 Posted by: fraannk Posted at: 2018-04-09T18:59:40.915Z Reads: 150

```
It seems like I only get the correct value of kv when I type kv in the terminal WHILE giving full throttle. If i stop the motor and wait a bit, it changes the kv value. But when I give full throttle and type kv with a couple sec intervals, i get pretty consistent readings. Any idea why? And which value can I trust? Thanks :)
```

---
## \#603 Posted by: onepunchboard Posted at: 2018-04-09T19:18:59.247Z Reads: 155

```
u can calculate yourself too, u voltage reading and rpm reading
```

---
## \#604 Posted by: TarzanHBK Posted at: 2018-04-10T13:37:22.945Z Reads: 150

```
@Ackmaniac do you know why?
```

---
## \#605 Posted by: Ackmaniac Posted at: 2018-04-10T13:49:03.171Z Reads: 157

```
The motor needs to move for the kv detection because of the observer. Best is to spin up the motor, then release the key and while the motor slows down by itself you should execute the kv command.
```

---
## \#606 Posted by: fraannk Posted at: 2018-04-10T14:23:33.679Z Reads: 156

```
When I let it slow down it became really inaccurate. I could only get consistent calculations while the motor was running :)
```

---
## \#607 Posted by: Shaibazsayed66 Posted at: 2018-04-17T13:07:00.176Z Reads: 163

```
same her i have focbox and facing same problem from the day i brought it
```

---
## \#608 Posted by: Jumpman Posted at: 2018-04-17T13:15:52.822Z Reads: 164

```
Maybe try using [Esc tool](https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116) instead?
```

---
## \#609 Posted by: Blacksheep Posted at: 2018-04-25T07:20:20.777Z Reads: 161

```
How did you get it in Mac?
```

---
## \#610 Posted by: trampa Posted at: 2018-04-25T07:44:00.624Z Reads: 164

```
Please only use the latest VESC-Tool for the now. There has been an issue with the brake operation on over temperature (motor /ESC), which Benjamin just fixed on sunday. Only use the latest version VESC-Tool.
If the fix has been implemented in project forks needs to be asked!
MAC users should use the windows version on their MAC. Please use either Boot Camp, Parallels, VirtualBox, VMWare  to get windows running. 

Frank
```

---
## \#611 Posted by: Pimousse Posted at: 2018-04-25T08:18:26.659Z Reads: 159

```
[quote="trampa, post:610, topic:32268"]
MAC users should use the windows version on their MAC. Please use either Boot Camp, Parallels, VirtualBox, VMWare  to get windows running.
[/quote]

We know you as an Open Source defender knight.
So you might want people to use Linux instead of Windows. :yum:
```

---
## \#612 Posted by: trampa Posted at: 2018-04-25T08:21:09.608Z Reads: 150

```
That would be the best option, sure. Is there a LINUX parallels desktop for MAC? I haven't been using MAC stuff for ages....
```

---
## \#613 Posted by: Pimousse Posted at: 2018-04-25T08:37:52.350Z Reads: 151

```
Paralells desktop is only a sfotware that allows you to build virtual machine.
You can have different VM in the software library.
```

---
## \#614 Posted by: rpasichnyk Posted at: 2018-04-25T08:38:49.714Z Reads: 154

```
No need to use virtualization when native macOS build works perfectly fine. Updated to latest v0.92 https://github.com/rpasichnyk/vesc_tool/releases
```

---
## \#615 Posted by: lock Posted at: 2018-04-25T11:32:26.421Z Reads: 159

```
Wireless firmware upgrades FTW!

[quote="rpasichnyk, post:614, topic:32268, full:true"]
No need to use virtualization when native macOS build works perfectly fine. ...
[/quote]

Only reason I'm still using Parallels+Ubuntu is because the Bluetooth support in your MacOS build seems a little untested. I can scan for my VESC (nrf51) and it'll seemingly find it as it grabs the name of the BTLE device ("VESC BLE UART"), but the address displayed alongside the name is all zeros instead of the usual string of hex. Appreciate this may not be at the top of your priorities.

![image|582x189](upload://vGZHCocV0UABm6y1RcLBEM0BEpk.png)

Log messages from when I try to connect.

    2018-04-25 21:21:19: VESC® Tool 0.91 started
    2018-04-25 21:21:19: Status: Not connected
    2018-04-25 21:21:46: DEBUG (:0 ): BLE scan found device: ""
    2018-04-25 21:21:46: DEBUG (:0 ): BLE scan found device: "VESC BLE UART"
    2018-04-25 21:21:46: DEBUG (:0 ): BLE scan found device: "VESC BLE UART"
    2018-04-25 21:22:11: DEBUG (:0 ): BLE scan finished
    2018-04-25 21:22:56: WARNING (:0 ): construction with remote address is not supported!
    2018-04-25 21:22:56: WARNING (:0 ): BLE error: QLowEnergyController::Error(UnknownRemoteDeviceError)

It'd be nice to use a native MacOS version. Parallels doesn't support the built in BTLE chip in Macs, so in order to use the VESC Tool I have to fire up the VM, and go hunting around for a tiny USB BTLE that does work within parallels.


Also note the debug messages state "VESC® Tool **0.91** started" whereas the official (Ubuntu) build states "VESC® Tool **0.92** started". Not sure if this is an issue or not... The application itself still seems to support FW 3.38.
```

---
## \#616 Posted by: trampa Posted at: 2018-04-25T12:58:26.478Z Reads: 159

```
Please use the 0.92 only! As stated earlier it is the one with all issues fixed.
```

---
## \#617 Posted by: MannyM0E Posted at: 2018-04-25T18:13:38.307Z Reads: 162

```
How do I know if I have the latest vesc tool ? 
I already have the program onto my laptop but don't have internet where I live. Is it like a update for it ?
```

---
## \#618 Posted by: trampa Posted at: 2018-04-25T18:36:00.318Z Reads: 163

```
By version number. 0.92...

Under Help you will finde a changelog.
```

---
## \#620 Posted by: Highwon Posted at: 2018-05-20T10:51:49.145Z Reads: 142

```
Hur installerade du det på mac?
```

---
## \#621 Posted by: rpasichnyk Posted at: 2018-05-21T13:54:43.695Z Reads: 136

```
@Highwon https://github.com/rpasichnyk/vesc_tool/releases
```

---
## \#622 Posted by: Highwon Posted at: 2018-05-21T15:26:38.528Z Reads: 137

```
Du är en legend som fixat det!!!!!
```

---
## \#623 Posted by: adilism Posted at: 2018-06-05T13:58:13.595Z Reads: 126

```
Can anyone comment on using this VESC tool with TB VESC? Also, I have some 2.xx firmware version, can't recall exactly. Can I go straight to the last FW version available?
```

---
## \#624 Posted by: trampa Posted at: 2018-06-05T14:05:37.085Z Reads: 127

```
Yes you can upgrade to lates FW. And you can use any HW 4 with the new VESC-Tool  APP for Android. Firmwares for HW 4 are included.
```

---
## \#625 Posted by: adilism Posted at: 2018-06-05T14:14:30.514Z Reads: 127

```
[quote="trampa, post:624, topic:32268"]
[/quote]

Thank you! Can you please share the FW download link? I can't find it on the vesc project website.
```

---
## \#626 Posted by: trampa Posted at: 2018-06-05T14:29:08.240Z Reads: 133

```
Included in VESC-Tool!

Frank
```

---
## \#627 Posted by: adman Posted at: 2018-09-09T05:03:12.913Z Reads: 96

```
I did this three years ago with disconnecting to soon.   This time it was using all the new software I think.   Charge it to experience.  lol wont be the last
```

---
## \#628 Posted by: MustardTiger Posted at: 2018-12-21T19:52:27.101Z Reads: 63

```
Thank you for this!!!
```

---
