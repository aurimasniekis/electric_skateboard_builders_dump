# Did I just brick my Focbox? Heeelllppppp!

### Replies: 88 Views: 1307

## \#1 Posted by: taz Posted at: 2018-10-07T13:25:48.801Z Reads: 288

```
Ok, I updated my Focboxes to 3.40FW, run the motor wizard and the input setup wizard.
The update was performed using the TCP bridge on the metr.at app.
Everything seemed to work fine.
I started experimenting with throttle curves (no belts attached), I am not sure what happened but at some point everything stopped responding.

Now my master focbox can't connect to the VESC tool.

The slave connects fine with the USB or with the metr module (if I connect the module to the slave)
It does not matter whether I try to connect via the metr pro module or directly with a USB cable.

Before anyone asks me, I did not at any time disconnect the CAN cable.

I have my new SurfRodz with psychotiller mounts and six shooters coming tomorrow and the bloody thing does not work (AGAIN :face_with_symbols_over_mouth:)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-07T13:32:00.138Z Reads: 271

```
There are any red lights blinking on the one which not respond?
```

---
## \#3 Posted by: taz Posted at: 2018-10-07T13:33:50.594Z Reads: 264

```
No, only the blue light is on, same as the other one.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-07T13:36:53.493Z Reads: 261

```
Guess you already restarted it many times.
Did you try to disconnect the can bus and get connection if it’s a single unit?
The usb cable work on the other focbox, so it’s not the reason...
Maybe also try to disconnect the bt module and try only to connect via usb.
```

---
## \#5 Posted by: taz Posted at: 2018-10-07T13:37:32.374Z Reads: 250

```
I have tried all of that. Nothing worked.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-07T13:38:11.179Z Reads: 244

```
St v2 link would be an option.
```

---
## \#7 Posted by: brenternet Posted at: 2018-10-07T13:39:46.215Z Reads: 244

```
Check then actual usb port on the focbox. Make sure there's a solid connection. I had to remove a bit of material on my plug to get it to connect reliably
```

---
## \#8 Posted by: taz Posted at: 2018-10-07T13:47:28.364Z Reads: 236

```
I have tried multiple USB cable, some with a longer connector.
However it is definitely not the port since even the metr.at pro module does not work.
```

---
## \#9 Posted by: taz Posted at: 2018-10-07T13:49:28.617Z Reads: 233

```
Yeah, I have thought about that.
Unfortunately I do not have one and it would take weeks from one to arrive from China.
Even then I hope flashing a new bootloader and firmware would solve the problem.
Anyway it seems I am screwed :disappointed:
```

---
## \#10 Posted by: craigthemachine Posted at: 2018-10-07T13:49:57.051Z Reads: 230

```
This is the exact same fucking thing that happen to my Focbox two days ago. The Metr Pro fucked it. However the only thing I did was to “read” motor config. It gave an error, and what you know. Master went only blue lights.
```

---
## \#11 Posted by: taz Posted at: 2018-10-07T13:50:36.617Z Reads: 211

```
Did you manage to repair it?
```

---
## \#12 Posted by: craigthemachine Posted at: 2018-10-07T13:51:54.497Z Reads: 214

```
My board was working perfect , until I open the app and did read config.
```

---
## \#13 Posted by: Andy87 Posted at: 2018-10-07T13:52:49.952Z Reads: 218

```

Where you located?

https://www.amazon.com/Aideepen-ST-Link-Programming-Emulator-Downloader/dp/B01J7N3RE6/ref=mp_s_a_1_5?ie=UTF8&qid=1538920320&sr=8-5&pi=AC_SX236_SY340_QL65&keywords=st+v2+link&dpPl=1&dpID=41u9nyzYQoL&ref=plSrch
```

---
## \#14 Posted by: craigthemachine Posted at: 2018-10-07T13:53:40.582Z Reads: 213

```
![image|374x500](upload://qgT7fUNOfQE0fm2KVbL4b0Vkew.jpeg)
```

---
## \#15 Posted by: craigthemachine Posted at: 2018-10-07T13:54:08.080Z Reads: 208

```
Waiting on the St-link.
```

---
## \#16 Posted by: taz Posted at: 2018-10-07T13:54:12.138Z Reads: 208

```
Crap, I did the same thing to check if all my config was sent to the focboxes.
I got a message saying the app is not yet compatible with the firmware and next it did not work.
I never thought it could have caused the problem.
```

---
## \#17 Posted by: taz Posted at: 2018-10-07T13:56:07.090Z Reads: 205

```
That is exactly what I am seeing.
```

---
## \#18 Posted by: craigthemachine Posted at: 2018-10-07T13:56:23.604Z Reads: 203

```
I had ack 3.102. It worked with the app, I got data , etc etc . But this happen at the modes area. 

I was looking to make a mode. So I did “read” It loaded the information. Then gave an error. And disconnected.
```

---
## \#19 Posted by: craigthemachine Posted at: 2018-10-07T13:59:39.103Z Reads: 204

```
Well I did most of the research. Apparently you get the 

1. Get a st-link
2. Wire it to the box
3. Download the utility 
4. Load hex file 
5. Load default VESC firmaware 
6. Update firm of your choice via USB. 

Hopefully that works, either way I looking purchase another Focbox soon.
```

---
## \#20 Posted by: DAddYE Posted at: 2018-10-07T14:02:41.528Z Reads: 201

```
Happened to me the same on Flipsky 6.6. I think right after I read the configuration from metr.
```

---
## \#21 Posted by: craigthemachine Posted at: 2018-10-07T14:03:51.598Z Reads: 191

```
Yes. Did you get yours going ?
```

---
## \#22 Posted by: DAddYE Posted at: 2018-10-07T14:04:58.757Z Reads: 185

```
Nope. St-link did not work. It couldn’t connect at all on one of them. The other one was still working.
```

---
## \#23 Posted by: taz Posted at: 2018-10-07T14:05:42.812Z Reads: 186

```
That is not good
```

---
## \#24 Posted by: brenternet Posted at: 2018-10-07T14:06:43.813Z Reads: 181

```
@rpasichnyk has anyone spoken to you about this?
```

---
## \#25 Posted by: craigthemachine Posted at: 2018-10-07T14:06:48.301Z Reads: 174

```
that sucks. It should. It better work . Wtf
```

---
## \#26 Posted by: DAddYE Posted at: 2018-10-07T14:07:55.445Z Reads: 170

```
@rpasichnyk do you think metr can be the culprit here?
```

---
## \#27 Posted by: DAddYE Posted at: 2018-10-07T14:09:21.767Z Reads: 168

```
It is a Flipsky. So.. different.  Hopefully focboxes are more resilient
```

---
## \#28 Posted by: craigthemachine Posted at: 2018-10-07T14:14:05.247Z Reads: 170

```
I’m 100% percent sure it was. I remember in detail what I did. I wanted to create a mode from my existing settings. 

I’m not sure if me having ack 3.102 firmware and using his app , rather than using his firmware to read was the problem.
```

---
## \#29 Posted by: craigthemachine Posted at: 2018-10-07T14:14:28.836Z Reads: 174

```
![image|281x499](upload://dhaqSuTdZp4S0n46iB2TrMOvGuk.jpeg)
```

---
## \#30 Posted by: taz Posted at: 2018-10-07T14:18:50.980Z Reads: 166

```
Will this ST-link be ok?

https://www.amazon.co.uk/ST-Link-automatic-downloader-programming-simulator/dp/B0722WMDFQ/ref=sr_1_1?ie=UTF8&qid=1538920657&sr=8-1&keywords=st-link+v2

It seems to be the only one I can get this week (albeit at a premium 30 Euros :rage:)
```

---
## \#31 Posted by: trancejunkiexxl Posted at: 2018-10-07T14:35:37.272Z Reads: 158

```
U can probably borrow one from somebody
```

---
## \#32 Posted by: craigthemachine Posted at: 2018-10-07T14:39:29.847Z Reads: 159

```
From what I understand, they are all the same if there are V2.
```

---
## \#33 Posted by: taz Posted at: 2018-10-07T16:02:26.578Z Reads: 162

```
Ok. I ordered an ST-Link V2 from Amazon.fr

https://www.amazon.fr/ST-Link-Automatique-simulateur-Programmation-T%C3%A9l%C3%A9chargement/dp/B0722WMDFQ/ref=sr_1_1?s=electronics&ie=UTF8&qid=1538927311&sr=1-1&keywords=st-link+v2

Supposedly it will be here on Wednesday so we will know if uploading the bootloader fixes the problem.
```

---
## \#34 Posted by: taz Posted at: 2018-10-07T16:19:26.858Z Reads: 157

```
These f**ckers are getting more and more frustrating.
It seems on the Focbox you have to connect directly on the PCB

https://www.electric-skateboard.builders/t/help-with-focbox-firmware-bootloader-upgrade-vesc-tool/34810/45?u=taz

I mean come on, I flew RC helis and esk8s  are starting to get on my nerves more than they did.
```

---
## \#35 Posted by: telnoi Posted at: 2018-10-07T16:36:06.719Z Reads: 152

```
Might luck out with a simple pin header.
```

---
## \#36 Posted by: dg798 Posted at: 2018-10-07T16:57:07.362Z Reads: 148

```
Did you try to just reflash the firmaware on both of them from the vesc tool?
```

---
## \#37 Posted by: ARetardedPillow Posted at: 2018-10-07T17:06:07.249Z Reads: 147

```
Metr.pro also fucked over @never4getf150forums board
```

---
## \#38 Posted by: craigthemachine Posted at: 2018-10-07T17:19:30.389Z Reads: 149

```
USB won’t detect “blue” light only Focbox.
```

---
## \#39 Posted by: Kug3lis Posted at: 2018-10-07T17:36:27.497Z Reads: 149

```
I dont think u suppose to flash firmware via metr..
```

---
## \#40 Posted by: taz Posted at: 2018-10-07T17:41:46.055Z Reads: 148

```
Well you can.
You can either do it through the app directly or use the phone as a TCP bridge.
The firmware update was successful. Something else happened and bricked the vesc.
Now if what you are saying if it was a good idea then I guess I agree with you.
I will do all my future settings via cable.
```

---
## \#41 Posted by: Kug3lis Posted at: 2018-10-07T17:43:21.684Z Reads: 144

```
Well looks like either ur bootloader was overwritten / flashing firmware failed because of lost connection or etc lost byte and etc.
```

---
## \#42 Posted by: taz Posted at: 2018-10-07T17:46:52.215Z Reads: 142

```
Definitely something went wrong.
However it was not during the firmware upgrade which was successful for both vesc.
After the firmware upgrade I proceeded with the motor and connection wizards and everything was working perfectly.
```

---
## \#43 Posted by: Kug3lis Posted at: 2018-10-07T17:48:26.620Z Reads: 143

```
Oh sorry as I skimemd i thought u flashed and it bricked :)
```

---
## \#44 Posted by: craigthemachine Posted at: 2018-10-07T19:07:38.395Z Reads: 143

```
Is doing the read settings flashing firmware ? 🤷🏽‍♂️ You got me confused af.
```

---
## \#45 Posted by: garseng Posted at: 2018-10-07T19:18:07.510Z Reads: 141

```
I have issue with metr as well. mine is vesc6, everything was working until i used one of the modes in metr. Both vesc was acting weirdly. I just re-flash my vescs and everything is working again.

I did emailed @rpasichnyk regarding this issue, he suggested not to use the modes features until he find the solution. and this was somewhere around 3 weeks ago.
```

---
## \#46 Posted by: DAddYE Posted at: 2018-10-07T19:35:40.000Z Reads: 137

```
Mine after flashing the modes was stuttering when starting
```

---
## \#47 Posted by: garseng Posted at: 2018-10-07T19:36:28.373Z Reads: 138

```
yeah..i had those as well
```

---
## \#48 Posted by: never4getf150forums Posted at: 2018-10-08T01:14:34.349Z Reads: 130

```
actually redoing the settings directly through the metr fixes the issue, for some reason it seems like adding the metr after settings are added manually thru focbox directly causes the module to load it's own incorrect settings, but changing the settings through the module itself seems to working great so far..

i know it may not make much sense, but it's worked fine for me so far, and i've ridden 25~ miles..
```

---
## \#49 Posted by: craigthemachine Posted at: 2018-10-08T02:15:57.096Z Reads: 121

```
It doesn’t, tried that countless times.
```

---
## \#50 Posted by: craigthemachine Posted at: 2018-10-08T02:18:34.620Z Reads: 123

```
![image|281x499](upload://hPEeGt1V6g8w9bv31IBdjEowIJc.jpeg) ![image|375x500](upload://ibgAx6XJMEkGjzlUXuu64YW5fMh.jpeg)
```

---
## \#51 Posted by: craigthemachine Posted at: 2018-10-08T02:20:20.004Z Reads: 115

```
The metr shows connected, but it doesn’t allow you to make changes to the master when it’s in “blue” light mode only.
```

---
## \#52 Posted by: taz Posted at: 2018-10-08T07:49:47.456Z Reads: 109

```
Same thing here.
```

---
## \#53 Posted by: rpasichnyk Posted at: 2018-10-08T08:22:44.057Z Reads: 113

```
I am willing to help with this bricking issue, please get logs from Settings -> Show Logs (send to support@metr.at)

I also have 2 pieces ST-Link V2 that I can send from Sweden if you think you can help me  reproduce the problem.
```

---
## \#54 Posted by: taz Posted at: 2018-10-08T09:53:13.680Z Reads: 108

```
Email with log file sent.
```

---
## \#55 Posted by: craigthemachine Posted at: 2018-10-08T13:45:39.362Z Reads: 107

```
I think I might have did the app reset. Either way I sent whatever information was there.
```

---
## \#56 Posted by: CarlCollins Posted at: 2018-10-08T14:02:08.142Z Reads: 104

```
@taz
Have you tried this?
Remove the plastic cover of the FOCBOX and check the points of the USB port, clean it up. Connect it to the PC/MAC using MicroUSB cable and let us know if you are able to get connection detection
```

---
## \#57 Posted by: Andy87 Posted at: 2018-10-08T14:04:16.254Z Reads: 105

```
It’s also not connecting to Bluetooth.
So I would assume it’s not the port which is broken. Or can a dirty port influence the connectivity with the Bluetooth module too?
```

---
## \#58 Posted by: craigthemachine Posted at: 2018-10-08T14:05:32.972Z Reads: 103

```
Correct. It’s not the USB.
```

---
## \#59 Posted by: taz Posted at: 2018-10-08T14:05:42.383Z Reads: 101

```
The problem is not the USB port because then the metr pro module would still work.
```

---
## \#60 Posted by: CarlCollins Posted at: 2018-10-08T14:16:57.611Z Reads: 99

```
@taz
Sometime's when there is an error or any short part on the PCB of the FOCBOX, the settings get reset. So the best way to ensure that is to connect it using USB. I think bluetooth settings are reset.
It happens many times.
```

---
## \#61 Posted by: taz Posted at: 2018-10-08T17:38:50.445Z Reads: 88

```
Just opened the focbox.
Did not notice any shorts, blew it clean just in case.
Unfortunately it still does not work.
Let's hope the st-link does the trick.
The fact that I have to connect it directly to a glue covered PCB does not make the job easy 😐
```

---
## \#62 Posted by: craigthemachine Posted at: 2018-10-08T17:54:28.754Z Reads: 87

```
I soldered little pins on mine. I used pins from little LeD diodes. Can send a picture later. Used a needle to poke the holes clean.  Seems overkill, but just Incase I have to do this all over again.
```

---
## \#63 Posted by: rpasichnyk Posted at: 2018-10-08T20:15:28.808Z Reads: 81

```
[quote="taz, post:59, topic:70433, full:true"]
The problem is not the USB port because then the metr pro module would still work.
[/quote]

This is not entirely correct. In theory if you disable UART, Metr Pro will not work but USB will. Did you make sure that your USB cable can be used for data transfer and not just charging? Can be checked by using this USB cable with some Android phone for file transfer, for example.
```

---
## \#64 Posted by: taz Posted at: 2018-10-08T20:21:39.406Z Reads: 80

```
I have 2 focboxes.
On one everything works perfectly but not on the other one.
In any case I tried different cables but none of them worked.
Yes, all my USB cables can be used for data transfer.
```

---
## \#65 Posted by: craigthemachine Posted at: 2018-10-08T21:04:29.436Z Reads: 79

```
I second this. This is not an USB issue. I do believe we rule that out early on in the discussions.
```

---
## \#66 Posted by: CarlCollins Posted at: 2018-10-08T22:20:15.464Z Reads: 80

```
@taz
Can you please share the images of the PCB here?
Front and back required
```

---
## \#67 Posted by: rpasichnyk Posted at: 2018-10-09T07:46:44.234Z Reads: 83

```
I received logs from @taz and I can confirm that VESC stopped responding for some reason during TCP Bridge session. I can't see exactly when VESC stopped responding, because log file contains only data coming from the computer (one side). I will add logging for the other direction as well.

My guess that it was here and the last command that you did was Write App Configuration (02a310)
```
[I 14:05:45.550] read: 02a31000000003e8000000000100c8020403466a(20)
[I 14:05:45.559] read: 60003e19999a3f84189340029fbe3fc4bc6a0101(20)
[I 14:05:45.569] read: 0000000000000000023e99999a3dcccccd010145(20)
[I 14:05:45.576] read: 3b8000003e19999a3f6666664040000040000000(20)
[I 14:05:45.584] read: 3f66666640400000010100000000000000000000(20)
[I 14:05:45.592] read: 0000023e99999a3dcccccd0000453b800001f400(20)
[I 14:05:45.600] read: 01c200013e19999a3f6666663e99999a453b8000(20)
[I 14:05:45.608] read: 0000000000000000020000453b80000203010003(20)
[I 14:05:45.615] read: 4cc6c70001101e03(8)
[I 14:05:45.674] read: 02011fe3de03(6)
[I 14:05:46.289] read: 02011fe3de03(6)
[I 14:05:46.373] read: 02011fe3de03(6)
[I 14:05:46.749] read: 02011fe3de03(6)
[I 14:06:42.959] Setting PositionSource.active to true
[I 14:06:48.249] TCP disconnected 0xbf0bb198
[I 14:06:48.267] new TCP connection 0xdd92e340
[I 14:06:48.643] read: 020100000003(6)
[I 14:07:13.525] Setting PositionSource.active to false
[I 14:07:13.544] unpair: device=0xbfb53240, esc=0xbfa7af70
[I 14:07:13.544] pair: device=0xbfb53240, esc=0xc35fbb00
[I 14:07:13.545] Ask.startRt()
[I 14:07:13.552] virtual TCP::~TCP()
[I 14:07:13.553] TCP disconnected 0xdd92e340
[I 14:07:30.845] [NRF_LOG] <warning> app: RT TIMED OUT 1

[I 14:07:31.359] [NRF_LOG] <warning> app: RT TIMED OUT 1

[I 14:07:31.869] [NRF_LOG] <warning> app: RT TIMED OUT 1

[I 14:07:32.350] [NRF_LOG] <warning> app: RT TIMED OUT 1
```
```

---
## \#68 Posted by: taz Posted at: 2018-10-09T17:36:23.693Z Reads: 82

```
Should I be looking at anything in particular?

![20181009_202202|375x500](upload://ePyPD9tlTETPFOV6oynq2kzC1qr.jpeg) 

![20181009_202125|374x500](upload://rp0gLYYp8yfoTQhyAn2GcmY9Xep.jpeg)
```

---
## \#69 Posted by: taz Posted at: 2018-10-09T20:40:11.895Z Reads: 77

```
Ok, I received the st-link one day early so went to town.
![20181009_222529|375x500](upload://qCcjg68SPhAdBkyi8kECe6EXGQL.jpeg) ![20181009_222514|374x500](upload://mv27siJ5HxPgWT4QhHLayRY3XKP.jpeg) 

Soldered 3 pins ( DIO - GND - CLK) , 2 from one side of the PCB and 1 from the other side since otherwise the connector would not fit so close together.
Uploaded the boot loader then the firmware.bin and then proceeded with the VESC tool as usual.
Soldering the pins was a bitch due to all the silicone on the PCB.
@CarlCollins you should really do something about this. Having to solder on a PCB to upload the bootloader is not what I would consider appropriate.
Anyway, the bloody thing now works.
```

---
## \#70 Posted by: Kug3lis Posted at: 2018-10-09T20:44:14.927Z Reads: 77

```
I don't think it is focbox issue... Never had focbox clearing itself or etc thing to happen.
```

---
## \#71 Posted by: taz Posted at: 2018-10-09T20:49:12.932Z Reads: 78

```
I did not mean it was a foxbox issue.
Why this happened I have no idea, maybe it was the metr pro module, maybe it was something I did wrong.
The fact is that the esc was bricked and instead of just opening the case and connecting to some pins I had to solder pins directly on a silicone covered area of the PCB.
```

---
## \#72 Posted by: Kug3lis Posted at: 2018-10-09T20:52:03.589Z Reads: 75

```
Well it's really rare case when you would need to reflash the bootloaders... It's purpose to be always available and its flashed only once in manufacture place so that's why you should be even happy it has holes, most other electronic devices has some test points scattered throughout the board.
```

---
## \#73 Posted by: taz Posted at: 2018-10-09T20:53:53.473Z Reads: 75

```
If you read this thread and all the other threads in this forum you will see I am not the only one to have this happen to his vesc based esc.
```

---
## \#74 Posted by: Andy87 Posted at: 2018-10-09T20:55:03.001Z Reads: 73

```
Nice to hear that everything working now again 👍
```

---
## \#75 Posted by: craigthemachine Posted at: 2018-10-09T20:55:37.602Z Reads: 72

```
I was thinking the same thing. Having pins there by default would have been nice. either way, great news I heard all day! I got to wait one more day for me st-link.
```

---
## \#76 Posted by: craigthemachine Posted at: 2018-10-09T20:57:18.173Z Reads: 75

```
Yes agree, to some extent. Having something is better than nothing. But yea, would have been better if they just included a pin section.
```

---
## \#77 Posted by: Kug3lis Posted at: 2018-10-09T21:07:11.180Z Reads: 75

```
I am saying that this is more related to common item in all those issues: Using metr to reprogram parameters or flash it and etc things. I don't use it so I can't tell anything more :)

Guessing from log I think it entered write app config command, was writing remaining bytes and when disconnected then connected back and wrote bytes of new command which continued the same command which was opened before disconnection and overwrote some stuff in memory or etc can't tell more as I don't remember how vesc handles commands anymore. But I think the issue is that app disconnected in the middle of the command and when started sending new command bytes to same opened command byte command or etc :thinking:
```

---
## \#78 Posted by: CarlCollins Posted at: 2018-10-09T21:26:03.650Z Reads: 73

```
@taz
Glad that everything is back in working order again!
For the ST-Link flashing, actually, FOCBOX comes with the pre-installed bootloader and 2 out of 10 people only suffer to this rare condition.
Also, FOCBOX is initially a Raptor 2 replacement item.
```

---
## \#79 Posted by: taz Posted at: 2018-10-09T21:31:24.758Z Reads: 74

```
[quote="CarlCollins, post:78, topic:70433"]
and 2 out of 10 people only suffer to this rare condition.
[/quote]

I would not call a condition that happens to 20% of the FOCBOX owners rare.
```

---
## \#80 Posted by: CarlCollins Posted at: 2018-10-09T21:37:24.893Z Reads: 77

```
@taz
As per my knowledge and experience while working with Enertion. 
Condition is quite rare because most of the customers use USB connection to flash firmware without any issues.
```

---
## \#81 Posted by: craigthemachine Posted at: 2018-10-09T21:38:21.119Z Reads: 76

```
Makes sense. But the same thing happen to me. However, I only did “read” . No write commands. So I guess it’s read and write. There’s obviously and issue/bug with the app mode change section.  The developer is looking into it,  We only sharing experience so it can be promptly resolved.
```

---
## \#82 Posted by: Kug3lis Posted at: 2018-10-09T22:06:41.267Z Reads: 74

```
[quote="taz, post:79, topic:70433"]
I would not call a condition that happens to 20% of the FOCBOX owners rare.
[/quote]

One thing you can't blame FocBox as its only hardware... It's software and it can affect any vesc ;)
```

---
## \#83 Posted by: craigthemachine Posted at: 2018-10-11T02:55:10.828Z Reads: 67

```
I’m back in business fellas ! Zoom zooom!
```

---
## \#84 Posted by: Jc06505n Posted at: 2018-10-11T23:54:28.995Z Reads: 64

```
Basically just happened to me , TCP thing and everything
```

---
## \#85 Posted by: craigthemachine Posted at: 2018-10-12T00:10:34.150Z Reads: 65

```
That sucks. Hopefully you can get an st-link,?get you back on the road soon.
```

---
## \#86 Posted by: chrischo1996 Posted at: 2019-03-23T21:07:25.375Z Reads: 55

```
Exact same thing happened to me, I changed some settings in Vesc tool mobile, switched to metr.pro and read configurations, turned off and on the board to confirm everything worked, and the master side of my Flipsky 6.6 Dual was dead, no green led only blue. For those of you who had the same issue as me, please pm to walk me through the steps of reviving it. I understand I have to purchase a stlink v2 but I'm lost from there despite trying to search for a clear tutorial. Thanks in advance.
```

---
## \#87 Posted by: chrischo1996 Posted at: 2019-03-23T21:09:38.741Z Reads: 54

```
Can I pm you my logs, maybe take a look and see if I did anything wrong? Thanks.
```

---
## \#88 Posted by: banjaxxed Posted at: 2019-03-24T00:52:21.927Z Reads: 42

```
I used some pin headers without soldering them in (although you can if you want)

Just slightly pressed against the pcb holes and uploaded the hex..worked fine
```

---
