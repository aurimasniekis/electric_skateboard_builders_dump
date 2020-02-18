# I&rsquo;m having trouble updating firmware

### Replies: 37 Views: 789

## \#1 Posted by: Gannet Posted at: 2019-07-13T22:48:13.322Z Reads: 128

```
I have two vesc 6 plus units on a trampa holy pro. Twin 154Kv motors. 2x 6s 25c 10Ah lipo (12s 10Ah).
My problem is when I update the firmware from 3.57 to 3.58 it uploads. I wait for the lights to stop flashing and some , reboot and the vesc still has the old firmware 3.57 
I'm using my laptop with vesc tool 1.16
I tried to do it with my phone app and get the same thing. 
I'm a newbie at this and not great with computers or programming 
![20190714_102147|281x500](upload://iKPDLnQxbgwZc8GTeQFe3evVdXS.jpeg) 
![20190710_153838|690x388](upload://yLldvKptBRiYq5snBhW1NnHGmKZ.jpeg) 
Thanks for any help in advance,  I'm going crazy here
```

---
## \#2 Posted by: Treezie Posted at: 2019-07-13T23:41:11.528Z Reads: 108

```
I am having exactly the same problem and I have read that people other than yourself are too. When I updated to the 3.58 it reverts to 3.57. Also I can't get on to the VESC website, it appears to be down at the moment.
```

---
## \#3 Posted by: Gannet Posted at: 2019-07-14T00:11:26.613Z Reads: 104

```
Cheers for putting me out of my misery, no boarding today then :frowning: 
Does anyone know how these feet things work, is it still one foot in front of the other ?
```

---
## \#4 Posted by: Treezie Posted at: 2019-07-14T03:20:13.453Z Reads: 99

```
No problem! Let me know if you have any developments, I will do the same. Cheers, Luke.
```

---
## \#5 Posted by: r3vilo Posted at: 2019-07-14T15:49:32.117Z Reads: 92

```
Same problem. 3.57 at the moment. Also after updating - seems to write new firmware - but after reconnect its still 3.57. ... I tried everything except USB connection. Only Bluetooth via Android app and PC VESC tool over TCP bridge.
```

---
## \#6 Posted by: mohitkorganji Posted at: 2019-07-14T18:41:25.816Z Reads: 83

```
I've been trying to get on the website. It's been 3 days since I have tried. I have the download file, but it wont work because its copied and I think you have to download from the website for another device. Is this being fixed because I need to change my board settings?😥😥😪😪😢
```

---
## \#7 Posted by: kchxaz Posted at: 2019-07-15T04:09:28.380Z Reads: 78

```
Glad I'm not the only one having those issues. I was pulling my hair out I was getting so frustrated with it. Still, not very comforting to not have a fully functioning VESC tool. 

I got my setup to the point I could ride it but I'm FOC in PPM mode and don't know if the two are related but my motors shudder horribly if I am not already pushing to max foot speed before hitting the throttle on the remote. I get this rapid pushing/pulling on the belts and it tears all the way through the whole board...Wish there was a setting to fix that issue
```

---
## \#8 Posted by: Gannet Posted at: 2019-07-16T00:55:04.453Z Reads: 72

```
I've had some success, I opened a old vesc tool on my tablet, 1.13 and reloaded the firmware 3.57 (yes not 3.58)
My board is running again,  I'm calling it a win :sunglasses: 

Hopefully the vesc project web site comes back online soon!

The phone app won't work as it wants new firmware and the board has only got half power (that is most likely me not knowing how set the vesc properly)  but that's enough for a well needed ride :smiley:
```

---
## \#9 Posted by: trampa Posted at: 2019-07-16T01:13:01.394Z Reads: 69

```
If the update doesn't work, you should try and re-upload the bootloader. The bootloader upload is the TAB next to the Firmware upload. 
After uploading the bootloader, upload the new FW. Only do one VESC to try! If it works, do the other VESC. 

The vesc server is down for a technical reason. Benjamin is still in France, after visiting the esk8 event. He's back on the 22. July and will fix the server connection.
```

---
## \#10 Posted by: Gannet Posted at: 2019-07-16T04:14:01.665Z Reads: 65

```
Just tried the bootloader  reboot then  firmware 3.58 update reboot and 3.57 is still loaded.
It was worth a try :frowning:
```

---
## \#11 Posted by: trampa Posted at: 2019-07-17T01:58:55.692Z Reads: 65

```
Stange! Can you run the SWD Prog feature?
This allows you to use one VESC to program another VESC. Both VESCs need to be interconnected via their SWD Ports. IO to IO, CLK to CLK and GND to GND. No other pins are connected. Power both VESCs, run SWD Prog in VESC tool desktop, click on connect, select VESC 6, hit upload. Now one VESC flashes the other VESC with the latest FW.
```

---
## \#12 Posted by: Treezie Posted at: 2019-07-18T02:34:02.112Z Reads: 56

```
FYI: VESC website is back online. I haven't had a chance to try the firmware update yet. I will let you know how I go when I get home.
```

---
## \#13 Posted by: Treezie Posted at: 2019-07-18T06:24:11.341Z Reads: 57

```
I just retried it since the website is back online and still no cigar. Not sure what we are doing wrong but it keeps reverting to 3.57.
```

---
## \#14 Posted by: Gannet Posted at: 2019-07-18T08:30:23.198Z Reads: 53

```
I don't have a SWD cable. Don't know how flashing one vesc to the other is going to help if both separately won't update FW.
I open to trying it tho.
```

---
## \#15 Posted by: Gannet Posted at: 2019-07-18T08:44:24.401Z Reads: 52

```
Bugger,  does your board run still on 3.57? 
My still works but I had to use vesc tool 1.13 to upload 3.57 which makes my board work.
If I use 1.15 or 1.16 to upload 3.58 my will only run slow / 10kmh max speed.
```

---
## \#16 Posted by: Treezie Posted at: 2019-07-18T09:49:47.092Z Reads: 50

```
Unfortunately, no. It's a brand new build so it's never been operational before. Is there anyway I could get my hands on an older version of the software to configure the motors? Or will it still continue to search for firmware version 3.58?
```

---
## \#17 Posted by: r3vilo Posted at: 2019-07-18T12:01:50.788Z Reads: 50

```
I tried it also today again. Same issue. Still on 3.57. Also uploading bootloader again does nothing. I mean, it seams it does something, Signal LED on Focbox and Metr.Pro blinks also like it's tranferring data, but after that process, it's still the same. Updating seems not to work.

Now I am thinking it is not a thing of VESC-Tool or Vedder's website, because I tried also the Ackmaniac ESC Tool, and wanted to upload Ackmaniac firmware. Therefore I opened my enclosure and connected via USB. Bluetooth was not successful before, so I tried it with cable.

Result: The same. Still 3.57, not the 3.103 or something from Ackmaniac. Same procedure. It seems to write after pressing the upload button, but after restart/reconnect both VESCs are still running with 3.57.

So... IMO I tired everything. And because also uploading Ackmaniac firmware does not work, it has nothing to do with VESC-Tool, Benjamin's server or vesc-project.com. ... Ackmaniac is a different software, from a different guy on a differnt server. It HAS TO work. But it doesn't. Seems like 3.57 cannot be overwritten or something. Maybe the files are read-only and you have to be Admin to overwrite lol. Idk. ... Does everybody in this forum has this problem at the moment? Is anybody with 3.57 able to update right now? That would be interessting.
```

---
## \#18 Posted by: trampa Posted at: 2019-07-19T19:32:55.515Z Reads: 47

```
The entire software needs to be re-written via SWD port. I will help you to get this sorted. 
Drop me a PM.
```

---
## \#19 Posted by: r3vilo Posted at: 2019-07-19T23:33:59.231Z Reads: 45

```
You mean that SWD method you described above? That one VESC programs the other? Like @Gannet said, I also don't understand how that should work. I have two VESCs and I am not able to update one of them. So, as you said @trampa , the software needs to be re-written.  But both VESCs are running fw 3.57, which needs to be re-written, if you are right. Why should it work?

I can try this and I appreciate your help but I don't get the point. A small explanation would be nice. Just what happens in that process. I want to know the background, I want to learn and understand. At the moment, for me, it makes no sense.
```

---
## \#20 Posted by: r3vilo Posted at: 2019-07-20T14:07:33.647Z Reads: 45

```
OK, watched a video where Benjamin is explaining SWD prog.

I think I got it. As I wrote the last post above, I thought - because firmware update is not possible - connecting both VESCs cannot do nothing, because both VESCs need new firmware.

But after watching this video I think I got it. Because USB connection is there you get the original firmware to your VESCs. It's all about the SWD port on the VESC, because it's only working over this port.

OK, then I need a cable, because I don't want to cut mine :slight_smile:

Thanks, @trampa
```

---
## \#21 Posted by: Gutta Posted at: 2019-07-20T14:29:09.467Z Reads: 42

```
I got the same issue, wont upgrade to 3.58....
And im not able to make it work at 3.57 either :frowning:
```

---
## \#22 Posted by: trampa Posted at: 2019-07-20T18:17:39.553Z Reads: 42

```
We should have a SWD PROG cable soon. I will check the stock on Monday. Another method is using the ST-Link V2 which can be found for cheap in online auctions. Just make sure to buy one stocked in your country, not coming from the other side of the planet.
```

---
## \#23 Posted by: Gannet Posted at: 2019-07-22T11:23:32.789Z Reads: 40

```
I've got 3.58 loaded :slight_smile: 

Ok this time the first thing I did was to turn the Volume up on my laptop so I can hear when the upload is done about 30 seconds to a minute after uploading then 10 seconds after lights stop flashing.

This is what I had to do.

I had to use a SWD cable 80mm x 3pin only.
Use a older vesc tool  1.13.
Connect .
SWD prog. Connect.  Vesc6. Upload
Reboot (and pull out usb as it can still get power from it).
Do the same to the other vesc.
Reboot.
Vesc tool 1.16.
Connect .
Firmware update . All.
Wait for sound.  then 10 seconds .
Reboot.
:slight_smile:
```

---
## \#24 Posted by: trampa Posted at: 2019-07-22T11:28:40.516Z Reads: 39

```
This how it works (minute 5:40 onwards):
https://www.youtube.com/watch?v=PFFiVxFHDM4
```

---
## \#25 Posted by: Gutta Posted at: 2019-07-22T14:23:08.952Z Reads: 39

```
Thanks for the fix. But for me I have to wait until new fw release I guess. I dont have any swd cable :confused:
```

---
## \#26 Posted by: Gannet Posted at: 2019-07-22T19:01:27.890Z Reads: 37

```
I don't think a new FW will do it.
Go to a RC model shop and get some plugs. I had to solder the wires to make a SWD  cable. You only need 3 wires/ 3pin plug.
Even try some local RC clubs .
Good luck
```

---
## \#27 Posted by: Gannet Posted at: 2019-07-22T19:15:40.197Z Reads: 35

```
![20190722_201244|281x500](upload://b2VUkXx7R7GXiZjYe2OkyPyyW73.jpeg)
```

---
## \#28 Posted by: Treezie Posted at: 2019-07-22T22:02:34.987Z Reads: 32

```
Thank you for the update. @trampa I am using a Dual FSESC4.20, would I need to use a ST-Link V2 to reprogram mine?
```

---
## \#29 Posted by: trampa Posted at: 2019-07-23T08:36:16.958Z Reads: 28

```
If it has two SWDs, you should be able to flash one side with the other. 
Their customer support should be able to help you.
```

---
## \#30 Posted by: Gutta Posted at: 2019-07-23T19:55:08.013Z Reads: 28

```
I took a 12s balancingwire and tore it apart. I hope Its going to work. Thanks for the advice! 

First time touching the vesc, so im not rly sure about this :D Its supposed to be connected to batteries when I plug it into the computer? Just one vesc to computer? And then find old vesctool?
Fck I dont know what im doing. :(
```

---
## \#31 Posted by: Gannet Posted at: 2019-07-24T10:39:12.939Z Reads: 30

```
Eek
Watch the video above 
And read my write up again.

The cable goes between the vesc's  SWD port.
The 3 middle pins. clk to clk. Gnd to gnd and IO to IO
Vesc power via your board batteries. 
Unplug everything else.
Connect laptop with usb cable ( make sure the usb cable is a data cable. Some are power only)
Watch the video again
Good luck
```

---
## \#32 Posted by: Gutta Posted at: 2019-07-24T16:31:48.745Z Reads: 26

```
Do you have a link to Vesctool 1.13? Cant find it, only for android :(

Edit: Fw updated! It did work on the new version of Vesc Tool, fyi :) 

Thanks a lot Gannet and Trampa. Rly appreciate it.
```

---
## \#33 Posted by: Treezie Posted at: 2019-07-25T06:31:10.618Z Reads: 26

```
Still no success for me. I have connected the SWD cable and no include firmware appears when I connect through the SWD menu. I am really at a loss as to what to do.
```

---
## \#34 Posted by: Gannet Posted at: 2019-07-25T06:36:45.277Z Reads: 26

```
I had the same with vesc tool 1.16 I had to use vesc tool  1.13 to do the SWD program
```

---
## \#35 Posted by: Gannet Posted at: 2019-07-25T06:42:52.923Z Reads: 25

```
https://send.firefox.com/download/e90152ebd9af150b/#AbTRs3Yee3K4Pgs51_Fj7w
```

---
## \#36 Posted by: Treezie Posted at: 2019-07-25T10:16:41.728Z Reads: 22

```
@Gannet I owe you a carton, mate. That worked like a charm. Interestingly I tried 1.1 to no avail but version 1.3 rectified the issue. Thanks again! Shout out to @trampa too. I appreciate it fellas.
```

---
## \#37 Posted by: kchxaz Posted at: 2019-08-15T10:38:54.667Z Reads: 18

```
[Using VESC tool 1.13, also tried 1.08; F/W 3.57 down graded from 3.58] 

Tried this per the video by Ben. Failed. So have power to both VESC's (two Flipsky Dual 6.6), right? Check. ok, USB data cable is plugged in and connected to main "good" VESC that I'm flashing from, I place the VESC tool in SWD mode by clicking on the tab to the left of the screen. Then connected the SWD cable to my good VESC, then connected SWD cable to other dual VESC. *There are no light's like you see on Ben's VESC (Don't know why I don't have them, I thought he was flashing a 6 also...?)*. I then click connect on the right side of the SWD screen but nothing happens like what happens on Ben's screen. I got nothing. And I'm very frustrated. Ever since I upgraded to 3.58 firmware nothing but MAJOR issues with this POS. Even after rolling back and using an older tool.

Can anybody see what I did wrong?
```

---
