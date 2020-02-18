# Bluetooth HM-10 not discoverable on Android 8.0/8.1 Oreo

### Replies: 71 Views: 10143

## \#1 Posted by: GunnarK Posted at: 2017-10-28T11:01:14.977Z Reads: 379

```
The topic has made some developments in which it became clear that  hm-10's are not to be paired with like a Bluetooth speaker for instance due to the Bluetooth profile BLE.
HOWEVER the question remains why I can't find the module using an app like VESC Connect on my Nexus 5x running 8.0 and 8.1.

For ease of use/understanding, below is the original topic:

--------------

Hi there,

I am trying to connect my phone(s) to the HM-10 module on my board.
The module is connected to the VESC and there is a red LED blinking, so far so good!

But trying to connect to it using my Nexus 5X running Android 8.1 (previously 8.0, but didn't work either) is not possible since I can not find it at all..
<img src="/uploads/db1493/original/3X/1/1/1173ccd840392047a8bf3c804a2824eca9916233.png" width="281" height="500">

Using my old Samsung S4 running 7.1.2 custom ROM LineageOS I am able to find the module but when trying to pair to it I get the message
> Pairing rejected by BT05

<img src="/uploads/db1493/original/3X/d/d/dd74cc0cee32778d71857bfe492baca8b47ab5e5.png" width="281" height="500">

Is there any setting I need to change? Maybe something on the VESC?
My VESC setting for **Controller ID is set to 2**, maybe this needs to change?

Keywords:
not connecting, bluetooth, HM-10, HM10
```

---
## \#2 Posted by: Jumpman Posted at: 2017-10-28T11:17:32.564Z Reads: 324

```
I have no clue how any of these things work, but maybe you can understand something from the following link?  Could be the module?

[https://blog.yavilevich.com/2017/03/mlt-bt05-ble-module-a-clone-of-a-clone/](https://blog.yavilevich.com/2017/03/mlt-bt05-ble-module-a-clone-of-a-clone/)
```

---
## \#3 Posted by: GunnarK Posted at: 2017-10-28T11:43:00.658Z Reads: 317

```
Thanks for this link!
I should have searched BT05 myself.. hehe

According to this article I have the CC41-A

> Here is a comparison of the responses to “AT+NAME” with the default name set in the module:

> “CC41-A”:

> +NAME=BT05
> “MLT-BT05”:

> +NAME=MLT-BT05

Will have a better look at this article shortly, although it doesn't seem to have a solution for this problem.
Will google it shortly as well!
```

---
## \#4 Posted by: Deckoz Posted at: 2017-10-28T12:28:12.611Z Reads: 300

```
There's no reason to pair the device.

Just open the app, the app will find it and connect.

The reason is the Bluetooth tx/RX pins aren't sending normal Bluetooth data that the phone understands. Its sending UART over the air, the app is the other end of the UART connection. 

Just forget the technicalities and open the app with your skateboard turned on and search for the Bluetooth device in the app.
```

---
## \#5 Posted by: Pimousse Posted at: 2017-10-28T17:05:23.229Z Reads: 276

```
Since I updated my Nexus 5X to Android 8, no more bluetooth connection with none of my BT modules (metr.at included).
I'm considering downgrading the phone to Android 7, so much troubles with 8.0. :confused:
```

---
## \#6 Posted by: GunnarK Posted at: 2017-10-28T20:11:15.957Z Reads: 271

```
Tried that but scanning with metr.at didn't work
Thanks for the insights though!
```

---
## \#7 Posted by: GunnarK Posted at: 2017-10-28T20:16:03.787Z Reads: 266

```
Damn that sucks..
But using my Samsung S4 running 7.1.2 I can not find it when I scan with Metr app
```

---
## \#8 Posted by: Jumpman Posted at: 2017-10-28T20:23:27.414Z Reads: 257

```
Did you get it recently?  If so, then look at the end of the Metr thread.
```

---
## \#9 Posted by: GunnarK Posted at: 2017-10-28T21:26:38.258Z Reads: 253

```
I got it somewhere in August but just finished my build.
I didn't get the module from @rpasichnyk, but from @fottaz. Could this be a problem?

I tried VESC Connect but I couldn't find the module either.
```

---
## \#10 Posted by: Jumpman Posted at: 2017-10-28T21:50:05.361Z Reads: 245

```
Sorry, I don’t know.  I thought you had to get a special module for Metr?
```

---
## \#11 Posted by: fottaz Posted at: 2017-10-28T21:59:12.998Z Reads: 244

```
Its Just an hm 10 man, the same as what he's using. 

I dont know where you saw the baud rate since you have never been to the UART Tab of bldc. First of all, go to the UART Tab and see what baud rate is setted up.
```

---
## \#12 Posted by: GunnarK Posted at: 2017-10-28T22:02:00.636Z Reads: 240

```
I thought as well, but @fottaz says on his website that it's possible..

Hi @fottaz I had seen that tab, but I thought you meant another page. Couldn't remember there was an individual page for UART hehe
```

---
## \#13 Posted by: fottaz Posted at: 2017-10-28T22:19:57.091Z Reads: 237

```
Lol ok dont worry! At this point I would suggest you to try flashing Ackmaniac and installing his app, I've never had any pairing issue with It! Tomorrow I'll try with metr and my current Android version and let you know! Stupid question, isnt your phone with hidden bluetooth right :)?
```

---
## \#14 Posted by: GunnarK Posted at: 2017-10-28T22:24:21.300Z Reads: 243

```
Okay I managed to pair with the board BUT only with my old Samsung S4 running Android 7.1.2 and using Jacob's VESC app 'VESC Connect'. Scanning for the module inside the app instead of the phones bluetooth settings

Not desirable but it works. The battery on my S4 is terrible :joy:

@fottaz Looking forward to your findings! :slight_smile:  
Flashing ackmaniac's firmware requires a bootloader and thus some wire thingy to accomplish, right?
My phone is discoverable, but that shouldn't make a difference since the search happens from my phone not the other way around
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-10-28T22:25:43.655Z Reads: 237

```
noo[quote="GunnarK, post:14, topic:36713"]
Flashing ackmaniac's firmware requires a bootloader and thus some wire thingy to accomplish, right
[/quote]

nope.
pretty sure theres a guide on here on getting a bootloader through VESC-Tool
ill put it up here if I can find it

EDIT: found it - http://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752/80
```

---
## \#16 Posted by: fottaz Posted at: 2017-10-28T22:31:07.909Z Reads: 235

```
try connecting it to the ackmaniac bldc tool, if bootloader is installed (90% of maytech have it installed), the software will tell you if it's possible and will suggest to upgrade it.
```

---
## \#17 Posted by: GunnarK Posted at: 2017-10-28T22:36:46.532Z Reads: 227

```
Cool will try immediately!
```

---
## \#18 Posted by: fottaz Posted at: 2017-10-28T22:42:03.441Z Reads: 230

```
remember Buad Rate to 9600 for that
```

---
## \#19 Posted by: GunnarK Posted at: 2017-10-28T22:47:23.236Z Reads: 247

```
<img src="/uploads/db1493/original/3X/f/c/fc4d52f4f89960a0542f5597d3bb1b676e98c372.png" width="690" height="323">

So far so good, but the firmware is a little bit tricky. I went to the firmware tab and browsed to my downloads folder where the 'ackmaniac-firmware.zip' and unpacked folder are located. What file do I have to select?
I can not select the complete zipfile

I assume one of the following? VESC is version 4.12, installed firmware is 2.18
<img src="/uploads/db1493/original/3X/6/f/6f4e3552461e059a36a686f0cba96afc54eb73bb.png" width="690" height="364">

EDIT: read on this thread that I need one file from ackmaniac's dropbox: VESC_Ackmaniac_Mod_2_54.bin.
Will have a look at this firmware later
[quote="Ackmaniac, post:1, topic:12286"]
Here are some additional install instructions. Read them before please:

Be aware that this is only for Hardware Version 4.10 or above (VESC-X as well).

Important: You have to flash the Firmware with this modified BLDC-Tool.

Open the downloaded BLDC-Tool
Upload (Flash) the new Firmware File "VESC_Ackmaniac_Mod_2_54.bin" which is available in the Dropbox link.
Adjust the settings of your VESC. I would not recommend to use a saved config. It would be better and safer to set the values manually. So you should make screenshots of your old setup or write it down.
It is always possible to flash back to Vedders original Firmware.
[/quote]
```

---
## \#20 Posted by: Deckoz Posted at: 2017-10-29T00:13:37.544Z Reads: 232

```
Did you buy a metre.at module?

If I'm not mistaken the developer has programmed the Bluetooth Mac addresses into his app. So you'll need to purchase a module from him

If you purchased from him, modules before a couple months ago ran 115200 baud, the new ones are 9600 baud I believe.

@rpasichnyk Hey Roman maybe you can help if  he did purchase from you...
```

---
## \#21 Posted by: GunnarK Posted at: 2017-10-29T08:23:57.942Z Reads: 215

```
Hi I did not buy the module from Roman.

I've read that Roman programmed his modules or something so they work with his Metr app. But the things that I read about it on his forum were from some time ago. And there were all sorts of discussions about licensing so I thought (since fottaz's website says it works with his modules too) he had made his app public and is earning some money through donations by now..

Looks like that's not the case

Fottaz is looking into it so we'll see! 👌😁
```

---
## \#22 Posted by: Deckoz Posted at: 2017-10-29T13:47:28.698Z Reads: 207

```
If you bought a module that wasn't from Roman. It won't work.. No amount of looking into it is gonna change that. As you can't add the mac address of your module into the software( metre.at)
```

---
## \#23 Posted by: GunnarK Posted at: 2017-10-29T17:24:10.532Z Reads: 209

```
I understand. But that is if your story about MAC addresses is correct.
I will not be making any decisions on what is correct for now and wait till fottaz has an explanation.
```

---
## \#24 Posted by: Deckoz Posted at: 2017-10-29T17:44:56.656Z Reads: 208

```
You can wait for fotaz all you want. He didn't develop metre.at, Roman did.

I own two metre modules, and have tried doing simple renames of extra hm10 i haveBluetooth devices with "AT" serial commands to set the Bluetooth device name to match his "metr-XXX" naming. It won't do anything even with the same name as another module. The only other option on these HM10s is to pull the Mac address off and use that to lock down connectivity within the application if you dont want people using an app without your module.

If you dont believe me, hook up your hm10 to a FTDI adapter, open the serial console in arduino IDE @ the baud rate of the module, run the AT commands to set the name, AT to set baurdrate (115200) and AT save. 

Try all you want, you won't get anywhere unless you can rewrite the Mac addresses

As well if you look at metre.at on google play you can see the version revision history. Roman publishes a new version almost daily. Anytime a new module is sold a new version is released to accommodate additional mac addresses. You really think he updates the software daily with bug fixes? Doubtful.
```

---
## \#25 Posted by: SeanHacker Posted at: 2017-10-29T18:11:13.373Z Reads: 199

```
You won't be connecting to the Metr app unless you purchased a module from the creator. He states this very clearly in his thread. Use @Ackmaniac firmware/app if you'd like to use your bluetooth module to change/monitor your vesc's. 

_**"Full disclosure:**_

_**I've spent a lot of time and energy designing and implementing the apps including the web part. I've thought carefully about the business model and how to make the apps future-proof​:moneybag:. I decided to make the apps free and earn money by selling the bluetooth modules. Thats why I've built some protection that only allows apps to work with my modules. Other modules most likely won't work. This also helps me to provide best user experience and ease of use. The modules I sell are no soldering required™ pre-configured© plug and play® solution."**_
```

---
## \#26 Posted by: GunnarK Posted at: 2017-10-29T21:34:05.410Z Reads: 195

```
Guys take it easy. I fully understand what you are saying. I study computer science including hardware engineering so I know a few things about AVR/Atmegas and Arduino to say the least
I talked to fottaz and want to give him the opportunity to sort things out.
That's all

I have read the full disclosure a few days ago but already had bought the module from fottaz while he stated it should work with Metr. I didn't know at that time it was Mac address specific

[quote="Deckoz, post:24, topic:36713"]
You really think he updates the software daily with bug fixes? Doubtful.
[/quote]
I doubt that just as much
```

---
## \#27 Posted by: GunnarK Posted at: 2017-10-29T21:37:56.589Z Reads: 184

```
A bigger issue is WHY am I not able to connect to the HM-10 in any way using my Nexus 5X running Android 8.1/8.0?

@Pimousse is having the same problem so it seems to be OS related, but why? And is there a workaround preferably one without the need of root access
```

---
## \#28 Posted by: Deckoz Posted at: 2017-10-29T21:57:18.754Z Reads: 174

```
Hm10s by default are non discoverable/pairing BLE UART over air.

They aren't designed to be "paired" with. And shouldn't show up in androids Bluetooth pairings. Older phones with pre bluetooth v4+ the BLE devices would show up. But BLE devices are not designed to show up in the Bluetooth pairings of android.
```

---
## \#29 Posted by: GunnarK Posted at: 2017-10-29T22:24:32.943Z Reads: 175

```
Alright so it seems. Thanks for confirming that
I will look into Android 8 vs BLE and report back here. Or do you have any insights into this issue, @Deckoz?
```

---
## \#30 Posted by: GunnarK Posted at: 2017-10-29T22:53:56.851Z Reads: 182

```
I have created a topic on the Google support forum.
Could become very handy I hope!

https://productforums.google.com/forum/m/#!category-topic/nexus/connecting-to-networks-and-devices/nexus-5x/QxcbWBsnvWc
```

---
## \#31 Posted by: danielz Posted at: 2017-10-30T00:10:54.291Z Reads: 178

```
Indeed this is normal the HM10 low power bluetooth device. Any app designed for low powered bluetooth devices will see it and connect for you.

My Sony Z5 sees is but wouldnt pair, which left me scratching my head for a while. Opened up ACKMANIAC-ESC Monitor and bam, it found and connected to it instantly.

Im using 7.1.1
```

---
## \#32 Posted by: GunnarK Posted at: 2017-10-30T06:16:31.328Z Reads: 171

```
I have made some changes to the topic to be more aimed at the problem (Android 8 vs HM-10) since it has become clear that BLE devices aren't supposed to show up in your phones Bluetooth settings.

Thanks for double-confirming this @danielz!
```

---
## \#33 Posted by: Pimousse Posted at: 2017-10-30T07:48:09.686Z Reads: 171

```
It seems that Google is working on a fix for bluetooth, but mostly focused on BT headphones issues.
Same for Wifi, I have so many trouble with it, consuming a lot more of mobile data (issue also known by Google).
Do the 8.1 update correct some of these issues ?
My phone sticks to 8.0 and says that I'm up to date...
```

---
## \#34 Posted by: scepterr Posted at: 2017-10-30T09:18:27.881Z Reads: 173

```
I can confirm the OnePlus 3T on 8.0.0 does not work, 7.x.x was fine. Will update if anything changes
```

---
## \#35 Posted by: Sebike Posted at: 2017-10-30T09:38:12.856Z Reads: 175

```
Didn't read the whole thread tbh and don't know of this is relevant for you, but for me the ackmaniac app doesn't find the hm 10 unless both BT and GPS is turned on on my sony xperia.
```

---
## \#36 Posted by: GunnarK Posted at: 2017-10-30T11:11:30.082Z Reads: 181

```
Hi @Pimousse AFAIK I don't have any issues with Wifi, but I cant say anything about Bluetooth since I don't own bluetooth headphones.
Here is a screenshot from my data usage this month running on Android 8.1. I have a data limit of 5GB
<img src="/uploads/db1493/original/3X/b/3/b39757d8e892d6747fa6c87d034c461bc85b62ab.png" width="345" height="500">
Measured with the app Data Usage Monitor (non root)

In my opinion Android 8.1 runs flawlessly and much faster. Gives this feeling I got a brand new phone. I definitely recommend.
You do have to sign up for the beta program, but that is fairly easy these days. Just register your phone here, thats all
http://www.android.com/beta
Okay it's beta software but as long as I'm using it I haven't got into any problems. Downgrading is as easy as unregistering your device on the same page

@scepterr once I find out it works with a upcoming update I will let you know in this topic :wink:  

@Sebike this wasn't discussed before so good to know !
```

---
## \#37 Posted by: GunnarK Posted at: 2017-12-09T16:03:50.909Z Reads: 161

```
Has anyone tried the official 8.1.0 update which was launched a few days ago to see if BLE is fixed?
Can't find any answers with my quick Google search
```

---
## \#38 Posted by: trancer23 Posted at: 2017-12-09T20:37:53.703Z Reads: 165

```
@GunnarK i dont have this module, but i use a bt05-a module for other apps.  I can confirm STILL BROKEN in 8.1
```

---
## \#39 Posted by: GunnarK Posted at: 2017-12-10T15:44:43.468Z Reads: 163

```
@trancer23 what device do you have? Apparently the official 8.1 is only available to pixel 2 (XL) and Nexus 6p
```

---
## \#40 Posted by: trancer23 Posted at: 2017-12-10T16:05:59.059Z Reads: 172

```
I have a pixel 2 (not xl) on verizon. I was on the developer beta build, and got a notice to update to the official.

My build is Android 8.1.0 Security Patch level: December 5, 2017
```

---
## \#41 Posted by: scepterr Posted at: 2017-12-30T07:14:19.147Z Reads: 165

```
Just got an update on my OnePlus 3T, still 8.0.0 but Bluetooth WORKS! 😃😃😃
<img src="/uploads/db1493/original/3X/c/5/c5b64c58f5f4d1d12f918147da897cdb4c8adf1a.jpg" width="281" height="500">
```

---
## \#42 Posted by: vjsharpeyes Posted at: 2018-01-03T07:03:14.607Z Reads: 147

```
New Pixel owner also looking for answers on this. Any Pixel owners managed to get it working?
```

---
## \#43 Posted by: Acido Posted at: 2018-01-03T16:29:24.687Z Reads: 145

```
Download some ble check app to see if your phone has ble
```

---
## \#44 Posted by: Acido Posted at: 2018-01-03T16:31:06.907Z Reads: 144

```
Just download ackmaniacs app and it should connect without pairing

Its BLE usually not visible in bluetooth options as I know
```

---
## \#45 Posted by: mmaner Posted at: 2018-01-03T16:52:46.901Z Reads: 146

```
[quote="vjsharpeyes, post:42, topic:36713, full:true"]
New Pixel owner also looking for answers on this. Any Pixel owners managed to get it working?
[/quote]

I have a 1st gen pixel and its always worked.  I have an upgrade to the Pixel 2 sitting here on my desk, just haven't moved to it.  Took it out of the box, did a rudimentary setup, connected to the @Ackmaniac VESC app, no problems.  Both of my pixels are on Verizon, not sure if that matters or not, but any info helps I guess.
```

---
## \#46 Posted by: scepterr Posted at: 2018-01-03T16:55:23.485Z Reads: 143

```
What version of Android does it have?

@Acido that's not the issue there's a bug in Android 8 that breaks some BLE functionality
```

---
## \#47 Posted by: mmaner Posted at: 2018-01-03T16:58:00.254Z Reads: 142

```
The phone immediately requested an update as soon as I turned it on, its currently at 8.1 and works.  I did not try it with the original load.
```

---
## \#48 Posted by: GunnarK Posted at: 2018-01-03T17:28:25.965Z Reads: 147

```
So @mmaner you are running the official build. Not a beta?

I currently running 8.1 beta on Nexus 5x, it should receive a new patch in a few days if I'm correct. Hopefully there's a fix in that, otherwise I might revert back to 8.1 official

@Acido that is not the issue. Nonetheless worth mentioning. I didn't know this in the first place either..!
```

---
## \#49 Posted by: mmaner Posted at: 2018-01-03T17:58:59.707Z Reads: 144

```
[quote="GunnarK, post:48, topic:36713"]
So @mmaner you are running the official build. Not a beta?
[/quote]

Official, i don't typically root anymore, too much time involved :slight_smile:
```

---
## \#50 Posted by: vjsharpeyes Posted at: 2018-01-04T06:42:40.639Z Reads: 143

```
Yeah the app says it detects a low power BT but always fails to connect.
```

---
## \#51 Posted by: vjsharpeyes Posted at: 2018-01-04T06:43:52.902Z Reads: 139

```
Hmm...how frustrating. Maybe it's an XL 2 issue. The app says it finds it, but cannot connect.
Wait, I don't need to unpair it from my old phone do I?
```

---
## \#52 Posted by: mmaner Posted at: 2018-01-04T12:56:53.134Z Reads: 140

```
I don't know, it's worth a try.
```

---
## \#53 Posted by: GunnarK Posted at: 2018-01-05T19:45:41.016Z Reads: 140

```
You don't need root to run beta software for Google Beta Program.
You can sign up your Google phone at android.com/beta
```

---
## \#54 Posted by: GunnarK Posted at: 2018-01-05T19:47:50.999Z Reads: 142

```
Don't know either.

I am not even able to find the module with my Nexus 5X running 8.1 beta with November patch
```

---
## \#55 Posted by: vjsharpeyes Posted at: 2018-01-07T00:03:50.799Z Reads: 143

```
Nothing at all? My finds it (or maybe another BLE device around my apartment) but then says fails to connect. How frustrating. Glad I didn't trade in the old phone just yet.
```

---
## \#56 Posted by: GunnarK Posted at: 2018-01-15T08:07:42.422Z Reads: 139

```
Nope nothing..
Sounds like that's less of an annoyance than being able to find it but unable to connect 😅
```

---
## \#57 Posted by: MartyMcFly88 Posted at: 2018-02-21T19:00:58.813Z Reads: 142

```
Same here, updated to oreo, suddenly no chance of finding Module... worked perfectly before :(
```

---
## \#58 Posted by: Forum1234 Posted at: 2018-03-26T03:09:34.612Z Reads: 145

```
Is not fixable by App. It's a problem with the firmware of the bluetooth module (HM10) and the stronger bluetooth error tolerance in Android 8.x (OREO).

So a new FW for the bluetooth module is needed, it's buggy. 

See this link for more information:
https://e2e.ti.com/support/wireless_connectivity/bluetooth_low_energy/f/538/p/670467/2472298

Or search for "hm-10 oreo TI android bluetooth" in your prefered search engine.

The used bluetooth module is called HM-10, which includes a chip (CC2541) from TI (Texas Instruments).
```

---
## \#59 Posted by: Skitzor Posted at: 2018-04-16T15:31:34.932Z Reads: 133

```
We need more ppl on this issue

EDIT: Already found an important note from android which the DEVs could look in to

> Android 8 includes changes that bring both good and bad news. The bad news is that the existing workarounds will no longer work to let you detect beacons when you app is not in the foreground. The good news is that new APIs give you new ways of doing these same detections,

http://www.davidgyoungtech.com/2017/08/07/beacon-detection-with-android-8
```

---
## \#60 Posted by: MartyMcFly88 Posted at: 2018-04-18T21:23:43.705Z Reads: 128

```
Would different bluetooth module help?
```

---
## \#61 Posted by: Emerson Posted at: 2018-05-22T00:59:22.834Z Reads: 121

```
The proper module works with Android 8.0+. I'm running one on Android P right now. 

HM-10 Transparent Serial Port Bluetooth 4.0 Modules Bluetooth Serial Port With Logic Level Transformation
http://s.aliexpress.com/FJBJJ3qI
```

---
## \#62 Posted by: GunnarK Posted at: 2018-05-23T21:32:31.784Z Reads: 118

```
There you go. The module is at fault, not Android 8
```

---
## \#63 Posted by: Tron Posted at: 2018-06-16T16:14:52.779Z Reads: 110

```
Problem solved !, I could not connect to my HM-10 with my Pixel or Nexus 5 running on Android 8.0, I ordered the Bluetooth 4.0 Modules, and now it works like a charm.

HM10 not compatible with Android 8.0
![HM-10|666x500](upload://kou3z3r2KuJeEKUDQCCFs270Clm.jpg)

Bluetooth 4.0
![0|544x377](upload://yaO4AHvkDGxFVlB1fvFrCcsjBUs.jpg)
```

---
## \#64 Posted by: mmaner Posted at: 2018-06-17T00:20:28.093Z Reads: 109

```
Link plz. 

(10c)
```

---
## \#65 Posted by: Tron Posted at: 2018-06-17T16:08:25.169Z Reads: 104

```
Here is the link of the Bluetooth 4.0, it will work with Android 8.0 and above.

https://www.aliexpress.com/item/HM-10-Transparent-Serial-Port-Bluetooth-4-0-Modules-Bluetooth-Serial-Port-With-Logic-Level-Transformation/32238168582.html?spm=a2g0s.9042311.0.0.2c1c4c4dSZHfC7
```

---
## \#66 Posted by: GunnarK Posted at: 2018-09-13T18:48:34.004Z Reads: 76

```
IT WORKS!

But not on Android Oreo. I have Android 9.0 Pie Open Beta installed on my OnePlus 6. It's not flawless. You have to manually resize the tiles and the red/green connection icon is invisible/below tabbar.

I have to further test it but it seems to work with reading values and stuff

EDIT: red/green connection icon had to reset itself I guess. Restarting Metr fixed it.

![Screenshot_20180914-093117|236x500](upload://hHLE67tomOsnrdoaO5NE2dT2rbE.jpg)
```

---
## \#67 Posted by: Sigorr Posted at: 2018-09-30T01:18:38.783Z Reads: 67

```
https://www.youtube.com/watch?v=OhCjzZ6xsVA

Hello anyone know what I’m doing wrong I bought this of banggood
```

---
## \#68 Posted by: thisguyhere Posted at: 2018-09-30T15:45:08.227Z Reads: 65

```
the hm10 clones, which is probably what u have, do not work with android Oreo

https://blog.yavilevich.com/2018/04/should-you-throw-away-your-cc41-hm-10-clones-now-that-android-8-is-here/

if u got an early model hm10, make sure tx and rx are crossed
```

---
## \#69 Posted by: kalebludlow Posted at: 2018-12-15T05:43:21.260Z Reads: 44

```
Do we know if the clones work on Android Pie?
```

---
## \#70 Posted by: Friskies Posted at: 2018-12-15T09:09:25.858Z Reads: 40

```
Pretty sure it's a firmware thing so..... Roll the dice and see what happens?
```

---
## \#71 Posted by: Friskies Posted at: 2018-12-15T09:12:28.961Z Reads: 40

```
I wonder if he knows how much a build like that will actually end up costing though. I hope you didn't recommend more than 10s to him
```

---
