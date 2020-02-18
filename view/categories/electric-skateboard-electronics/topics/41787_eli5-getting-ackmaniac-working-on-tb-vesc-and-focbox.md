# ELI5 getting Ackmaniac working on TB VESC and FOCBOX

### Replies: 15 Views: 1493

## \#1 Posted by: Jreamer Posted at: 2017-12-23T22:46:41.531Z Reads: 156

```
I am a 5 year old when it comes to programming. I learn quick. If someone could maybe do a brief run down or video of switching over to Ackmanik I would surly use it.
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-12-23T22:47:19.563Z Reads: 156

```
i’m pretty sure there’s a walkthrough on his thread.
```

---
## \#3 Posted by: Jreamer Posted at: 2017-12-23T22:48:15.755Z Reads: 154

```
If you could provide a link it would be super helpful. That thread is so large it is intimidating to go searching through it.
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-12-23T22:48:34.344Z Reads: 147

```
should be in the first post
```

---
## \#5 Posted by: Acido Posted at: 2017-12-23T22:50:37.946Z Reads: 145

```
Ctrl+f and search for what you need
```

---
## \#6 Posted by: Jreamer Posted at: 2017-12-23T22:52:03.288Z Reads: 147

```
I was hoping to have a new thread with a quick rundown of how to get Ackmaniac working for us morons. But I guess that is a lot to ask.
```

---
## \#7 Posted by: Jreamer Posted at: 2017-12-23T22:55:03.823Z Reads: 149

```
For example @longhairedboy fried a VESC trying to detect his motor. I still can't find a simple explanation on how to install and run Ackmaniacs BLDC tool.
```

---
## \#8 Posted by: scepterr Posted at: 2017-12-23T22:58:36.414Z Reads: 146

```
[quote="Ackmaniac, post:1, topic:12286"]
Here are some additional install instructions. Read them before please:

Be aware that this is only for Hardware Version 4.10 or above (VESC-X as well).

Important: You have to flash the Firmware with this modified BLDC-Tool.

Open the downloaded BLDC-Tool
Upload (Flash) the new Firmware File "VESC_Ackmaniac_Mod_2_54.bin" which is available in the Dropbox link.
Adjust the settings of your VESC. I would not recommend to use a saved config. It would be better and safer to set the values manually. So you should make screenshots of your old setup or write it down.
It is always possible to flash back to Vedders original Firmware.

This Firmware has the Version 2.54. So don't be surprised by that. When you start the Modified BLDC-Tool the first time it tells you that the Firmware is not the same. So you have to flash it with my modified firmware. So no mistakes can happen anymore with the Firmware flash.
[/quote]

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#9 Posted by: Jreamer Posted at: 2017-12-23T22:59:22.911Z Reads: 130

```
Hell ya dude. This is what I was looking for! Love you brotha!!!!
```

---
## \#10 Posted by: scepterr Posted at: 2017-12-23T22:59:40.566Z Reads: 127

```
That's what everybody was telling you to search for
This was a one time courtesy, I'll search for you 😛
```

---
## \#11 Posted by: Jreamer Posted at: 2017-12-23T23:00:50.742Z Reads: 124

```
Thank you brother! That thread is different from the one I was looking in. I was looking here
http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---
## \#12 Posted by: scepterr Posted at: 2017-12-23T23:03:06.972Z Reads: 117

```
Yeah that one is for the newer v3.xx firmwares
```

---
## \#13 Posted by: evoheyax Posted at: 2017-12-23T23:06:52.799Z Reads: 112

```
1. Use your current BLDC tool to flash the firmware (connect to vesc, click firmware tab, select .bin file, click upload)
2. Using the new bldc tool, connect to the vesc again. Do a read config on main screen. Set the amp limits and current limits appropriately.
3. Now if you run FOC, life is super simple. You just click the buttons in the correct order, waiting for the motor to finish moving around (keep the motor off the ground for this).
4. If BLDC, click start detection. If it doesn't start spinning, just might need to adjust the current.
5. Click write config. This takes care of your MC Config. Now you need to set your App Config.
6. Click app config and click read config. Select ppm (or ppm+uart if using bluetooth).
7. Set main speed controller to id 0. Then under ppm, use the ppm wizard to balance it correctly if the default settings aren't working well for you (default settings are perfect for the mini trigger).
8. If your using abluetooth module, make sure you set the baud rate correctly under the UART tab (9600 for many)
9. If your doing multiple vescs, on the first vesc (vesc id=0), click "multiple esc's over can" under ppm. And for the other vescs, under app config, the increase the id by one for each vesc, and select "send status over can".
10. Now ride cause your done!
```

---
## \#14 Posted by: Jreamer Posted at: 2017-12-23T23:08:08.712Z Reads: 104

```
Dude you are a god! This is even more perfect. Now when people look for ELI5 Ackmaniac they get this!! So much help for the new members!!! <3
```

---
## \#15 Posted by: Jreamer Posted at: 2017-12-23T23:10:20.426Z Reads: 101

```
<img src="/uploads/db1493/original/3X/a/9/a970ce3e55462d61e21700d60c96b53162501ac5.jpg" width="666" height="500">
Going to be testing out some of your old hubs very soon!!!
```

---
