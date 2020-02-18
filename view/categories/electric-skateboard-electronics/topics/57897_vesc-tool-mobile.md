# VESC-TOOL Mobile

### Replies: 82 Views: 4544

## \#1 Posted by: trampa Posted at: 2018-06-05T10:31:32.041Z Reads: 569

```
Good Morning E-SKATERS! 

Benjamin has worked on a mobile friendly VESC-Tool since a while now. 
Whenever he found a minute he coded some bits and now we see some nice results.
He started a thread about it on his VESC-Project.com website. If you are interested, you can find his post here: https://vesc-project.com/node/234

I will post some screenshots here for everyone to look at. Things are not yet 100% polished up and some more stuff is waiting to be implemented. Work in progress....
The VESC-Tool mobile can configure pretty much anything you can configure with the desktop VESC-Tool versions. 

- motor detection 
- app configuration 
- radio setup and calibration / mapping
- changing all parameters / tune your board on the go
- display of real time data (master and slave)
- wireless firmware updates 
- connection to master and slave via CAN, using only one wireless module
- give your board a name to avoid confusion and wrong connections.

Current App solutions worked with standard wireless modules that didn't provide a high data transfer rate.
Benjamin has written a **custom firmware** for NRF51822 chipsets. He never goes down the simple and easy route, he wants things to work sweet and perfectly. So it's is not simply a USB-UART bridge, the software decodes and encodes the packets to get the maximum possible data throughput and reliability. This makes a big difference!

Since regular wireless modules do not work with VESC-Tool mobile, you will need a module that has the new firmware flashed onto it.  We provide a simple and easy to use dongle if you want to get started immediately. http://www.trampaboards.com/nrf-dongle-p-25516.html

Your mobile device should be running ANDROID and it should have Bluetooth 4 standard. 
Android 7 or later is recommended.
iOS s not supported since Apple doesn't allow Open Source Software in the Apple store.

**Where can I find the VESC-Tool mobile? And how do I install it?**

Simply create an account on vesc-project.com and add any VESC-Tool version to your basket. Finish the checkout and then click on "purchased files" in the top right section of the website. You will find an Android.ZIP folder there. Download the ZIP folder to your device and unzip it. The folder contains two files:

- vesc-tool_full.apk 
- vesc_tool_mobile.apk

The vesc_tool_full.apk will install the full VESC-Tool, featuring the same user interface as you already know it. This is good for tablets. The vesc_tool_mobile version is for smartphones. 

You may need to go to your device settings and allow the app installation from **unknown source**.
Your ESC should be configured to use PPM and UART (APP-Settings >>General). So you may need to use a USB cable to change that setting. Hopefully this will be the last time you will use a cable to configure your board.

**Here are some screenshots:**

On the bottom of the App you will find **WRITE** and **READ** buttons and the magic **three little dots**.

![VESC-Tool_Mobile_11|546x500](upload://y5yXalbUYSXBdANiz1eMCXanfB2.jpg)

![VESC-Tool_Mobile_22|546x500](upload://urESw5T8rWVXlyAKj3IBdntzAbi.jpg)

**If you would like to honour Benjamin's work, please consider to purchase one of the VESC-Tool versions that has a [donation](https://www.paypal.com/donate/?token=6_Ma33A1pHp0wRScJgxplbqSlsAGx2EFYJkBoMnFqh77MsU1r0W3fXO_OTT3KGLzZ9lxqW&country.x=US&locale.x=US) included. He does all the heavy lifting for the community and we think it's fair to invite him on a beer once in a while.**  **We spend little sums on silly stuff every day. This new App is so useful, it's worth to send Ben a little motivator to allow him to bang on stuff harder.** 

Frank
```

---
## \#2 Posted by: laurnts Posted at: 2018-06-05T11:24:26.347Z Reads: 425

```
Does it support Android 8? because that is what is all about.
```

---
## \#3 Posted by: lock Posted at: 2018-06-05T11:24:56.392Z Reads: 414

```
[quote="trampa, post:1, topic:57897"]
iOS s not supported since Apple doesn’t allow Open Source Software in the Apple store.
[/quote]

Actually iOS isn't supported because the Qt Serial Port library the VESC Tool uses isn't available for iOS. You could still have an iOS version and just not distribute it through the App Store (eg; release the source), it's not real hard to open up an Xcode project and click the build button... 

It's only GPL'ed code that falls foul of the App Store, most other open source licenses are fine. You'd honestly struggle to find an app in the App Store that *didn't* have open source code in it.

From a business perspective you want those iOS users, they're the ones with all the cash 😉
```

---
## \#5 Posted by: trampa Posted at: 2018-06-05T11:27:44.709Z Reads: 385

```
Android 7 or later.
```

---
## \#6 Posted by: linsus Posted at: 2018-06-05T11:44:05.592Z Reads: 373

```
I can vouch that its legit! Feels just like on a PC but in smaller format. Super handy
```

---
## \#7 Posted by: linsus Posted at: 2018-06-05T11:46:16.556Z Reads: 358

```
Its more that Ben despises Apple. Not that it cant be done. 😅
```

---
## \#8 Posted by: trampa Posted at: 2018-06-05T11:47:46.970Z Reads: 351

```
It can't be done respecting the GPL. So he doesn't put to much effort into it.
BTW, Github is now Microsoft...
```

---
## \#9 Posted by: lock Posted at: 2018-06-05T12:27:29.357Z Reads: 339

```
Dammit, VESC Tool on my novelty sized iPad would be so nice. It’s probably a fair call given the GPL issue, just not one I want to hear.

Wonder how an Apple related pull request would go. There’s a the Qt Serial Port library that the VESC Tool currently uses (doesn’t support iOS), but there’s also a Qt Bluetooth library that does support iOS. Solution would be to port it over, but that’s going to a change a chunk of the VESC Tool 😕.

[quote="trampa, post:8, topic:57897"]
Github is now Microsoft…
[/quote]
I’m just going to keep telling myself this is fine 😂.
```

---
## \#10 Posted by: trampa Posted at: 2018-06-05T12:39:08.110Z Reads: 319

```
There are alternatives...
```

---
## \#11 Posted by: briman05 Posted at: 2018-06-05T12:40:20.500Z Reads: 312

```
this would be very awesome
```

---
## \#12 Posted by: trampa Posted at: 2018-06-05T12:42:24.711Z Reads: 302

```
 e.g. GitLab
```

---
## \#13 Posted by: Dook Posted at: 2018-06-05T13:44:22.593Z Reads: 301

```
Downloaded software anatomy tablet and when I try to open the .apk file I get the error message "There was a problem parsing the package. Downloaded a second time and got the same error message. Any ideas ? cheers
```

---
## \#14 Posted by: trampa Posted at: 2018-06-05T14:04:39.747Z Reads: 291

```
Old Android version?
```

---
## \#15 Posted by: 12meterkuk Posted at: 2018-06-05T14:05:13.803Z Reads: 288

```
It only works with the bt module that you sell? Does it work with hm-10 modules?
```

---
## \#16 Posted by: Dook Posted at: 2018-06-05T14:07:02.184Z Reads: 285

```
yep, have 5.1.1. will update. cheers
```

---
## \#17 Posted by: trampa Posted at: 2018-06-05T14:09:33.108Z Reads: 283

```
If you can flash it with Benjamin's FW, and do some soldering, you can use any NRF 51822 module.
Some people struggle, so we made a batch to get them started. Also the quality of the modules vary. Some are just crap, others work quite well. We designed it to work seamless.
```

---
## \#18 Posted by: Acido Posted at: 2018-06-05T14:21:37.741Z Reads: 274

```
We probably have a month untill its ruined like everything they buy
```

---
## \#19 Posted by: Maxid Posted at: 2018-06-05T14:50:38.437Z Reads: 277

```
AFAIK they have done a pretty good job with Xamarin
```

---
## \#20 Posted by: Deodand Posted at: 2018-06-05T21:40:54.592Z Reads: 272

```
I'm pretty sure the serial port library also isn't compatible with android. The android version of the vesc-tool only supports bluetooth access I believe. I do think some development effort is still required just to wrap and test an ios version though but not a ton. The x-code method isn't too involved but you need an apple computer and a bit of experience. You'd severely limit your user base if this was the only way to access the app on iphone. 

The GPL license is definitely incompatible with the apple app store based on what I've read. Apparently the owner of the license could release under dual license to allow an IOS version to be distributed in the app store specifically which is what some gpl licensed softwares have done. Is vedder the sole owner of the vesc-tool? How many people would have to be tracked down to enable distribution in the app store through dual license?
```

---
## \#21 Posted by: b264 Posted at: 2018-06-05T22:42:15.059Z Reads: 258

```
[quote="Deodand, post:20, topic:57897"]
Is vedder the sole owner of the vesc-tool?
[/quote]

The GPL states the public owns it, and nobody may steal it from them, including Apple.
```

---
## \#22 Posted by: trampa Posted at: 2018-06-05T22:43:16.700Z Reads: 247

```
Vedder and Apple are no good friends and he coded his stuff alone. He owns the copyright for his code.
Benjamin is very serious about what he is doing and he is very serious about the GPL-license. E-skaters better get an Android phone sooner than later.
```

---
## \#23 Posted by: b264 Posted at: 2018-06-05T22:45:51.882Z Reads: 240

```
Apple and freedom are fundamentally incompatible at the very core.  This is one manifestation of that.  You can run the tool on an Apple laptop ;-P  (for now)
```

---
## \#24 Posted by: lock Posted at: 2018-06-05T22:55:58.796Z Reads: 242

```
True, you can’t go back on the GPL. But if Vedder was the sole copyright he could give an alternate license. He’s not though, as others have made contributions and there’s no mention that you hand over copyright when making a contribution.

@Deodand ha, the official docs make no mention of this support, I swear it previously stated partial support for Android 😬. [Here’s a thread](https://forum.qt.io/topic/77240/qt-serial-port-android-ios-will-it-work) with some indication it existed. Looks like that support may be getting dropped, may mean a port over to the Bluetooth module needs to happen regardless of iOS support.
```

---
## \#25 Posted by: b264 Posted at: 2018-06-05T22:57:03.625Z Reads: 232

```
Actually the GPL covers all of that
```

---
## \#26 Posted by: Deodand Posted at: 2018-06-05T22:57:15.584Z Reads: 231

```
Serial port already doesn't work on android. If you use a phone variant you use bluetooth anyways.

Its true though that QT partially supports serial on android but it doesn't work on many many phones and the mobile version of the vesc-tool doesn't have a serial connect button.
```

---
## \#27 Posted by: myreala Posted at: 2018-06-05T23:11:56.654Z Reads: 227

```
Can anyone give me some instructions on how to flash the Vedder's firmware to a hm10 module?
```

---
## \#28 Posted by: Kug3lis Posted at: 2018-06-05T23:13:45.152Z Reads: 232

```
Sorry but it\'s not for HM-10 modules they are based on CC25** MCU :cry: 

https://slack-imgs.com/?c=1&url=https%3A%2F%2Fmedia0.giphy.com%2Fmedia%2FoOX5qIDkzDjeo%2Fgiphy-tumblr.gif
```

---
## \#29 Posted by: lock Posted at: 2018-06-06T03:29:38.184Z Reads: 226

```
I don't know why, but just kind of assumed it used that serial port library for Bluetooth connections too. There's a single line in the Qt Creator project file you need to comment out to not import this module, after that there's a few methods that need to be removed that wouldn't work on iOS anyway.

Then you get this...
![vesc_ios|690x459](upload://NrhkbUoPXNPn669iipOoscRKpW.jpg)

I don't have my iPad handy, just the simulator, but layout looks a lot more usable on the iPad.  I'm guessing this is because I haven't told it to use the mobile specific layout.

![image|690x455](upload://nDpcoigVSkkPtKta31xOS9n4LMy.jpg)

Will try to connect it later on tonight when I get home. There's a stack of warnings being printed out, and I'd be very surprised if it worked first time. Still promising for the 5 minutes (excluding the hours it took to download Qt) effort I put in.
```

---
## \#30 Posted by: Deodand Posted at: 2018-06-06T03:58:55.561Z Reads: 224

```
Cool, I've been playing around with this code for awhile. Let me know if you get hung up on something.
```

---
## \#31 Posted by: district9prawn Posted at: 2018-06-06T08:11:33.676Z Reads: 224

```
Just flashed a nrf module. Very easy everything is done just need to run the script.
```

---
## \#32 Posted by: lock Posted at: 2018-06-06T14:36:08.764Z Reads: 226

```
Didn't work first time on iOS, but I'd be worried if it did.

There's a 'kind of' bug in the Bluetooth code on MacOS/OSX, I say kind of as its not really a bug more that BT support was never tested on MacOS. This same bug affects iOS. I'd really like to get this fix into the official repo as I'm currently running the VESC Tool in an Ubuntu VM with a USB dongle, whereas I could just use a native MacOS build and the inbuilt Bluetooth. I haven't tested it, but am pretty sure the Mac issue is fixed.

I did test it on my iPad though :sunglasses:
https://www.youtube.com/watch?v=nhTX6tVuagI

Lots of little issues; UI rendering, have to click through license agreement each launch, where to save motor/app config files, etc. As I said before it's in a pretty good state considering how little effort it took.
```

---
## \#33 Posted by: Pimousse Posted at: 2018-06-06T14:47:52.171Z Reads: 218

```
I'm also a Mac user, and need to have a Ubuntu VM as well.
Could you make a pull request of your changes ?
```

---
## \#34 Posted by: lock Posted at: 2018-06-06T14:54:04.035Z Reads: 207

```
Yeah. Will tidy it up over the weekend and do a bit of testing just to make sure it doesn't break other platforms, etc.
```

---
## \#35 Posted by: Deodand Posted at: 2018-06-07T00:54:03.090Z Reads: 198

```
You might be aware of this but commenting or un-commenting #CONFIG += build_mobile in the .pro file will build the mobile UI. In my opinion this UI needs a lot of love before it will feel good to use but it is at least workable on the phone screen.
```

---
## \#36 Posted by: lock Posted at: 2018-06-07T01:46:33.325Z Reads: 203

```
That's good to know. I've spent a bit of time looking through the VESC protocol stuff, but the UI and QT Creator is something new to me.

VESC Tool UI does look to be lagging a lot of the other options available, but it seems like the right spot to focus development. There's probably 5-6 apps on this forum that all seem to do the same thing but not everything we want, it'd be nice if it was a little less fractured. 

Of course the GPL issue gets in the way a bit. One possible workaround would be to distribute a compiled ipa/app file, would skip the requirement to install Qt (16GB WTF!) and maybe even Xcode. BUT, they'd still need to signup for a dev account (free) and jump through a bunch of provisioning hoops and these can be a real PITA.

Honestly, as you stated above Vedder needs to get in contact with all other contributors/copyright holders and ask for different licensing terms for this to end up on iOS 'proper'. I'd go so far as to say he should also require copyright assignment (just like Qt does). Oh and someone will need to get him on a Mac with iPhone/etc for testing. Probably won't hold my breath...
```

---
## \#37 Posted by: Deodand Posted at: 2018-06-07T03:51:14.033Z Reads: 201

```
Yeah imagine if your software had a bug that you knew how to fix that prevented a large percentage of your user base from using it. Then you just told people rather than fixing it to just buy different $500+ electronics. 

[quote="lock, post:36, topic:57897"]
Oh and someone will need to get him on a Mac with iPhone/etc for testing. Probably won’t hold my breath…
[/quote]

I think if Vedder could figure out the legal side he could rely on someone to help him test/debug the ios implementation, obviously it can't be too insane if it only took you a bit to get one semi-functioning. I can't imagine there would be a huge outcry against a careful dual license to enable app store distribution and maintain GPL everywhere else. Licensing isn't my area of expertise though :slight_smile:
```

---
## \#38 Posted by: PeterMcKane Posted at: 2018-07-02T19:30:38.767Z Reads: 187

```
Is this new VESC tool software compatible and work well with the Maytech VESC?
```

---
## \#39 Posted by: trampa Posted at: 2018-07-03T06:58:04.168Z Reads: 182

```
Hi, Benjamin always assures max compatibility with all Hardware revisions. Latest Firmware for all Hardware revisions is included.
It's lots of extra work for Benjamin to make this happen. If you like the App please consider to give Benjamin some support. 

Frank
```

---
## \#40 Posted by: High-roller Posted at: 2018-07-03T08:32:40.549Z Reads: 179

```
Hey, I'm confused: which Bluetooth modules besides the trampa one work with the mobile vesc-tool, and what exactly do I have to do to get them to work?
I have one of @JLabs modules which I'm hoping I can use with this.
```

---
## \#41 Posted by: trampa Posted at: 2018-07-03T09:51:27.890Z Reads: 202

```
Our modules have a custom Firmware, written by Benjamin, and they have the correct connectors and pin connections. So that is plug and play for our VESC 6. We ordered more connection cables so that you can connect them to any HW 4.xx ESC (plug and play). Cables should arrive within the next weeks. 
You can also use the current cable, get yourself a female JST-PHR 7 Pin connector and pop that onto the cable ends. A needle does the trick to get the individual cables out of the 8 Pin connector we supply. No big issue, 5 mins job.
Frank
```

---
## \#42 Posted by: hexakopter Posted at: 2018-07-03T13:58:28.277Z Reads: 197

```
[quote="High-roller, post:40, topic:57897"]
which Bluetooth modules besides the trampa one work with the mobile vesc-tool, and what exactly do I have to do to get them to work?
[/quote]

Besides trampas bluetooth module you could also use Metr Pro that works out of the box with the VESC tool. It comes with a cable so it is plug and play. You can find more infos about that module here:
https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780

The other option would be to buy a "standard" nRF51822 module and some sort of programmer on eBay/etc. and flash it with Benjamins firmware like it is described here: [https://github.com/vedderb/nrf51_vesc](https://github.com/vedderb/nrf51_vesc)

The standard HM-10 modules will not work with the mobile VESC Tool.
```

---
## \#43 Posted by: trampa Posted at: 2018-07-03T14:00:40.721Z Reads: 183

```
Hi Hexacopter, did you incorporate Benjamins FW into your new module?

Frank
```

---
## \#44 Posted by: hexakopter Posted at: 2018-07-03T14:03:43.554Z Reads: 183

```
No. With Metr Pro we are using a different chip (not the nRF51822) that is running its own written firmware.
```

---
## \#45 Posted by: trampa Posted at: 2018-07-03T14:07:24.356Z Reads: 181

```
I Know that you use the NRF52 series. I was just wondering how you make it compatible to VESC-Tool BLE if you are not using Benjamin's initial FW code base.
```

---
## \#46 Posted by: mmaner Posted at: 2018-07-03T14:14:59.610Z Reads: 178

```
frank is sniffing for blood again...
```

---
## \#47 Posted by: Pimousse Posted at: 2018-07-03T14:25:00.648Z Reads: 185

```
Frank, did you know that it exists a french town called Vesc ??

I may help you to write a letter in French to sue the mayor until he changes the name of this (sin) city and gives attribution to the VESC Project.

https://en.wikipedia.org/wiki/Vesc

If I can help making the world fairer and better, count me in. :)
```

---
## \#48 Posted by: trampa Posted at: 2018-07-03T14:33:12.813Z Reads: 177

```
They are probably more into farming and tourism than making motor controllers and software (-;
```

---
## \#49 Posted by: Sn4pz Posted at: 2018-07-03T15:19:21.197Z Reads: 180

```
woosh? :laughing:
```

---
## \#50 Posted by: Trdolan03 Posted at: 2018-07-03T18:54:19.555Z Reads: 179

```
So what is the consensus on an IOS version?
```

---
## \#51 Posted by: trampa Posted at: 2018-07-03T19:05:15.502Z Reads: 184

```
As long as Apple doesn't change its App Store policies iOS versions are not GPL compatible. 
Since Benjamin published his code under the terms of the GPL, iOS users have an issue.
```

---
## \#52 Posted by: Jc06505n Posted at: 2018-07-03T20:01:56.099Z Reads: 180

```
It's possible, someone just needs to build it in Xcode and release it
```

---
## \#53 Posted by: defyent Posted at: 2019-05-24T08:11:17.007Z Reads: 102

```
is there any more information on this somewhere?
```

---
## \#54 Posted by: trampa Posted at: 2019-05-24T08:18:41.631Z Reads: 104

```
It does not work with HM-10, which is super slow compared to NRF 52xxx Bluetooth 5.
Get a proper dongle, which will last you for ever. This is your bridge to the App and the remote and upcoming equipment.
```

---
## \#55 Posted by: defyent Posted at: 2019-05-24T08:33:07.121Z Reads: 103

```
lol what a waste of time, next we'll be having to flash our network cards or buy specific ones to access the internet. How bad is this software that is requires a custom firmware on a bluetooth module?
```

---
## \#56 Posted by: defyent Posted at: 2019-05-24T11:04:59.820Z Reads: 98

```
Is this some ploy to force people into buying an overly priced bluetooth module through trampa? $35 for a $5 module?
```

---
## \#57 Posted by: trampa Posted at: 2019-05-24T11:50:29.335Z Reads: 98

```
What do you think how much time is involved to code all the software?
FW for module, SWD Prog feature in VESC-Tool, remote and App connectivity etc.
For 5$ you can't even get the raw module (without PCB, assembly, flashing, testing etc.)
Products usually cost more than the raw material involved.
```

---
## \#58 Posted by: JensSjogren Posted at: 2019-05-24T12:22:25.810Z Reads: 99

```
The price for the trampa dongle is roughly the same as the Metr module which is intended for the Metr app, nothing wrong here. Like previously said the programmers behind theese apps put a lot of hours into this, basicly the price of the dongle justifies you to use a premium firmware.
```

---
## \#59 Posted by: taz Posted at: 2019-05-24T12:24:17.004Z Reads: 97

```
You are joking right?

In any case, VESC is an open source project. You can always make your own version of the tool to connect with smoke signals or whatever makes you happy.
```

---
## \#60 Posted by: Sn4pz Posted at: 2019-05-24T12:30:12.235Z Reads: 97

```
And it pays for itself in convenience! I don't have a trampa specific one, but just having to open an app that feeds important information to the user is invaluable 👍
```

---
## \#61 Posted by: trampa Posted at: 2019-05-24T12:31:37.868Z Reads: 98

```
And wireless setup, FW updates etc.
```

---
## \#62 Posted by: Sn4pz Posted at: 2019-05-24T12:33:25.930Z Reads: 98

```
Ah, see I didn't even know it was capable of that. I only have experience with an HM10 module. :p
```

---
## \#63 Posted by: JensSjogren Posted at: 2019-05-24T12:38:19.622Z Reads: 98

```
I like the trampa dongle and vesc-tool app quite a lot, never has connection issues like the HM-10 modules ive tried has. However i miss a logging feature in the app that saves all the data from each ride so you can go back and see top speed, wattage, consumption etc. If i'm not completely blind It only logs the data in real time, any information if this will be added in upcoming FW updates?
```

---
## \#64 Posted by: trampa Posted at: 2019-05-24T12:40:39.558Z Reads: 104

```
Possible. One thing after another (-:
Now that the APP is working sweat like a dream, there is time to think about it.
Vedder and i banged hard on many things in the last months, including the remote.
That alone was quite a bit of work.
```

---
## \#65 Posted by: defyent Posted at: 2019-05-24T13:01:15.456Z Reads: 100

```
those modules don't need custom firmware. my point is that software which requires a specific piece of firmware on a specific piece of hardware serves no purpose other than locking people into that hardware. The idea that optimized encoding for something simple (not easy, simple) is a pretense. It's funny that the author doesn't like apple, considering he's adopted apple's exact business model ;)
```

---
## \#66 Posted by: taz Posted at: 2019-05-24T13:02:12.557Z Reads: 102

```
@trampa

My phone only seems to record while the screen is on. I have played with background app settings etc but can't get it to record apart from the start and end of the ride while I have the screen on.

Any ideas?
```

---
## \#67 Posted by: trampa Posted at: 2019-05-24T18:24:25.606Z Reads: 99

```
[quote="JensSjogren, post:63, topic:57897"]
However i miss a logging feature in the app that saves all the data from each ride so you can go back and see top speed, wattage, consumption etc.
[/quote]

Voila!

![Screenshot_20190524-200231|312x500](upload://dLXcDbtK3yRAgF9sQVrCDElrFGy.png)
```

---
## \#68 Posted by: EssEnn Posted at: 2019-05-24T21:01:30.247Z Reads: 88

```
I have found the logging to never saves the files and you have to manually set the destination folder and start the logging everytime you connect anyway. 

RT data is mostly usless while riding as Im not going to look at my phone all the time. Reviewing logs with GPS co-ords is way more helpful.
```

---
## \#69 Posted by: BigBrit Posted at: 2019-05-24T21:10:29.130Z Reads: 91

```
I have found the same.
```

---
## \#70 Posted by: defyent Posted at: 2019-05-25T00:59:58.086Z Reads: 82

```
so the mobile app is open source too?
```

---
## \#71 Posted by: McLovinsQuads Posted at: 2019-06-14T02:09:46.997Z Reads: 69

```
So just got the mobile version hooked up, got stuff setup and learning how to navigate it, how do you have it read out mph instead of km/h? Thanks jimmy
```

---
## \#72 Posted by: trampa Posted at: 2019-06-14T07:02:20.955Z Reads: 69

```
There is no button yet, but you can cheat it a bit by entering a wrong wheel diameter. 

example: 

8 inch wheel =198mm

198mm /1.60934 = 123mm

By entering 123mm instead of 198, you get miles instead of Km.
The display will still show Km, but you will know its miles. 

Benjamin will ad a feature to switch from metric to imperial soon.

Frank
```

---
## \#73 Posted by: Silverline Posted at: 2019-06-14T07:58:11.810Z Reads: 66

```
Does this module connect to the same physical port on the vesc, as where ADC 1 and ADC 2 needs to be connected ?
```

---
## \#74 Posted by: trampa Posted at: 2019-06-14T08:06:37.853Z Reads: 63

```
Yes, COMM. But you would use RX/TX and not the ADC 1 / 2 / 3
```

---
## \#75 Posted by: Silverline Posted at: 2019-06-14T08:40:02.483Z Reads: 61

```
Okay, so i have to split the wire (comm and maybe 3.3v/5v ) in order to use them at the same time ?
The link dosnt work at the moment : http://www.trampaboards.com/vesc-accessories-c-1468.html But this is the same module, that works with the wand right ??

And the vesc tool have a log function now, and real time data like til metr app right ??
```

---
## \#76 Posted by: trampa Posted at: 2019-06-14T08:49:38.625Z Reads: 59

```
We work on that!

Frank
```

---
## \#77 Posted by: Xenon Posted at: 2019-06-14T12:06:56.981Z Reads: 57

```
it looks like loging file must set to sdcard but i have no sdcard slot on my phone.
![Screenshot_20190614-140213|230x500](upload://xEMjvEnyp4ZQNWylpCVKMkNj5Rx.jpeg) 

or i do something wrong?

ups forgot the app permissions
```

---
## \#78 Posted by: McLovinsQuads Posted at: 2019-06-14T12:56:54.990Z Reads: 57

```
Awesome! Thanks for the reply! 

Jimmy
```

---
## \#79 Posted by: McLovinsQuads Posted at: 2019-06-14T12:59:20.530Z Reads: 59

```
I get the same message if I try to select that box. I went in and gave the app storage permissions but still get that notification
```

---
## \#80 Posted by: Xenon Posted at: 2019-06-14T13:07:24.550Z Reads: 56

```
click choose log file and select a folder (Downloads) this works for me.
```

---
## \#81 Posted by: McLovinsQuads Posted at: 2019-06-14T13:23:36.568Z Reads: 56

```
I’ll give that a shot! I also just found out I can put an sd card in my phone also. first android and it’s only for this app hahaha so still learning how it works and features lol
```

---
## \#82 Posted by: trampa Posted at: 2019-06-14T14:34:03.179Z Reads: 56

```
https://forum./t/help-with-my-stupid-bluetooth-module-new-vesc-tool-2019/1969/25?u=trampa
```

---
## \#83 Posted by: McLovinsQuads Posted at: 2019-06-14T14:59:08.484Z Reads: 54

```
Yeah that wand is high on the want list hahaha, I’m thinking I’ll be able to slide past the boss/wife and get in on that preorder 🤤 my Android was free luckily but the wife says when I’m walking from the shop to house with two phones it looks like I’m up to no good 🤣🤣🤣
```

---
