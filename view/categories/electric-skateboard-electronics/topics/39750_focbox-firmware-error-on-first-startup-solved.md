# Focbox firmware error on first startup (SOLVED!)

### Replies: 48 Views: 2683

## \#1 Posted by: High-roller Posted at: 2017-11-30T08:59:15.596Z Reads: 264

```
So there I am, finally ready to power up the focboxes I bought back in mid-June which I'm now trying unsuccessfully to connect to the bldc tool for the first time. It gives an error saying "no firmware read response".
I tried this guy's solution:
http://www.electric-skateboard.builders/t/vesc-problems-no-firmware-read-response-buffer-eraser-timed-out/25014
...no change in status.
So then I looked at this guy:
http://www.electric-skateboard.builders/t/help-with-first-time-setup-vesc-no-led-blinks-on-startup-no-firmware-read-response/33637/2
...still nothing, though I do have a two wire voltmeter, which is showing 0.0 percentage while volts are 34.4v.
I have the focbox securely connected to the battery and the receiver, which is powered on properly. Leds on the focbox indicate power (blue) and signal (green) but I still get no response other than that error.
I though maybe I had to connect both focboxes (unlikely, but what the hell), still the same. 
Also tried downloading the bldc tool again from enertion.
Anybody have any ideas? Please, I'm so close to finishing!




Four days later.....SOLVED!
It turns out that the usb cable wasn't pushed in all the way, partly because the opening FOCbox cover is quite narrow and the socket is set a little too far inside. You may need to remove the cover and enlarge the hole (see @yaca's photo).
Sometimes it really is the simplest things...
```

---
## \#2 Posted by: scepterr Posted at: 2017-11-30T09:04:51.191Z Reads: 236

```
Are you choosing the right COM port?
```

---
## \#3 Posted by: High-roller Posted at: 2017-11-30T09:07:18.922Z Reads: 227

```
All I have is COM5.
```

---
## \#4 Posted by: telnoi Posted at: 2017-11-30T09:08:07.459Z Reads: 221

```
I'd also give the vesc-tool a shot (available on OSX in case you use that, you'd have to search the thread for that build).
Running my dual focbox using their firmware/no issues.
```

---
## \#5 Posted by: scepterr Posted at: 2017-11-30T09:09:49.710Z Reads: 214

```
Does it show up after you plug it in, are you hitting the refresh button?
```

---
## \#6 Posted by: High-roller Posted at: 2017-11-30T09:10:54.467Z Reads: 207

```
@telnoi Ordinary pc here. I figured I'd start with the most basic one, but okay. here goes...
@scepterr it connects for about five seconds and then goes to error. refresh does nothing.
```

---
## \#7 Posted by: scepterr Posted at: 2017-11-30T09:11:59.534Z Reads: 196

```
Oh well that's the first mention that it does connect and then fails...that's different issue

Does anything happen in device manager when it errors in bldc tool, like is the device disconnecting/reconnecting?
```

---
## \#8 Posted by: Sebike Posted at: 2017-11-30T09:14:59.813Z Reads: 189

```
Did you try the (ackmaniac version of) vesc tool that has the connect feature that searches through available com ports?
Did st driver install successfully?
```

---
## \#9 Posted by: High-roller Posted at: 2017-11-30T09:19:12.192Z Reads: 186

```
Not that I can see. All I can see is the COM5 and I'm not sure that's where it is. where would it appear in the manager?
```

---
## \#10 Posted by: High-roller Posted at: 2017-11-30T09:20:32.137Z Reads: 188

```
It installed fine, but doesn't seem to have made a difference. I'm trying to avoid ackmaniac's since I wanted to start as simply as possible, without firmware updates or anything extra.
```

---
## \#11 Posted by: High-roller Posted at: 2017-11-30T09:31:01.611Z Reads: 180

```
Alright, vesc-tool says "Could not autoconnect. Make sure that the USB cable is plugged in and that the VESC is powered." Done and done.
Granted, my USB cable is kind of old, but I've never had problems with it before. I'm also not sure now whether it's really the firmware or just an old cable.
```

---
## \#12 Posted by: telnoi Posted at: 2017-11-30T09:34:51.973Z Reads: 168

```
If all goes well, it should tell you that your firmware is out of date/not compatible.
Since you have intermittent connection issues on two(?) vescs, I would try a new cable first..different usb port, or even another pc.
```

---
## \#13 Posted by: scepterr Posted at: 2017-11-30T09:41:28.510Z Reads: 162

```
Have you used that cable for data before or only charging
```

---
## \#14 Posted by: High-roller Posted at: 2017-11-30T09:47:58.122Z Reads: 174

```
Yes, both vescs have the same problem. I guess I'm buying a new cable...
@scepterr I bought it second-hand because I needed a long one for an arduino project. It worked well enough for data transfer there, though it's certainly not 3.0.
```

---
## \#15 Posted by: telnoi Posted at: 2017-11-30T09:48:56.834Z Reads: 171

```
additional note. The usb cable might not be plugged in all the way. Some mentioned that the ''new'' focbox design makes it impossible for some usb cables to connect properly/they are too thick.
```

---
## \#16 Posted by: High-roller Posted at: 2017-11-30T10:05:14.251Z Reads: 173

```
I was using two of those adapter ports, so I wouldn't have to open my enclosure every time I needed to work on the vescs. I just tried a USB phone cable which definitely works for data transfer and plugged it in directly. Still getting the same error.
What do you mean by too thick?
```

---
## \#17 Posted by: yaca Posted at: 2017-11-30T10:18:38.580Z Reads: 174

```
I had to cut a bit from the casing of the focbox for to have a connection with the usb phone cable. The cable didn't go in completely. Or you cut a bit from the cable plug if this is the problem.
```

---
## \#18 Posted by: High-roller Posted at: 2017-11-30T10:24:53.386Z Reads: 167

```
Could you send me a picture?
```

---
## \#19 Posted by: yaca Posted at: 2017-11-30T10:38:21.682Z Reads: 168

```
<img src="/uploads/db1493/original/3X/2/7/27070e7363e5b4cdc950083fa0c77be7806cdd56.jpg" width="667" height="500">
```

---
## \#20 Posted by: High-roller Posted at: 2017-11-30T13:24:05.149Z Reads: 158

```
Let's see...
So far Iv'e removed all usb devices from my pc (including COM5), used a different cord, rebooted multiple times, scanned for plug&play devices in my device manager- which freezes my pc, which then needs yet another reboot. Tried it on another laptop, turns out that one doesn't have COM5, couldn't even find any device. Nothing has worked yet.
A big shout out to Eric from Enertion support who connected remotely to my pc to try and help me with all this. Thanks man!
The vescs still definitely work, they just don't connect for some reason.
```

---
## \#21 Posted by: yaca Posted at: 2017-11-30T13:49:12.076Z Reads: 151

```
Are you sure, the plug is completely in the socket? It sounds like your computer doesn't recognize when you plug in the cable.
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2017-11-30T13:53:51.813Z Reads: 146

```
@high-roller can you tell more about your setup and post some picture. 

Are you attempting a dual or single setup?

What battery?


What Motor?

...

Also are the blue LED light up on the Focboxes ?

Regards
JF
```

---
## \#23 Posted by: High-roller Posted at: 2017-11-30T16:37:54.460Z Reads: 148

```
I'm attempting a dual build. 
So two FOCboxes, two sk3 6374 motors 190kv.
Battery is 10s5p , cells are 25r if that matters.
The blue power LEDs light up for both just fine, as do the green signal LEDs.
Let me know what you need pictures of.
@yaca I tried a phone cable directly on the vescs, and got a connection for about five seconds before I got the error, so I don't think it's a a problem of physical contact.
```

---
## \#24 Posted by: Blasto Posted at: 2017-11-30T16:45:49.921Z Reads: 143

```
I’ve seen bad usb cables to cause the device show up as “unknown” or to get a bad firmware version read out. Not sure if this is the case, but easy to get a new cable
```

---
## \#25 Posted by: High-roller Posted at: 2017-11-30T17:18:43.795Z Reads: 138

```
True enough. I'm taking it to a friend tomorrow who also has FOCboxes and see if he can figure it out. I guess we'll also check the cable.
```

---
## \#26 Posted by: High-roller Posted at: 2017-12-01T12:11:21.280Z Reads: 134

```
What Com port does everyone use to connect? COM5? I was told to remove it by Enertion support and now I can't connect at all.
```

---
## \#27 Posted by: yaca Posted at: 2017-12-02T22:09:00.835Z Reads: 126

```
In my case it's COM12. Did you already talked with your friend about your problem and tried to connect your focbox to his computer?
```

---
## \#28 Posted by: High-roller Posted at: 2017-12-02T22:28:08.371Z Reads: 124

```
Not yet, hoping tomorrow or monday. Out of curiosity I tried connecting without plugging in the usb, and I got the same error- "No firmware read response" . Is it possible that they came without firmware and I have to flash them again? Unlikely, I know, but still...
```

---
## \#29 Posted by: yaca Posted at: 2017-12-02T22:45:49.502Z Reads: 120

```
In my opinion your computer doesn't recognize your focbox when you plug in the cable. In my case my pc gives me a sound when I plug in the cable and gives also a sound  after disconnecting.  Just to be sure, your focbox is powerd on (battery is connected)  when you try to connect?
```

---
## \#30 Posted by: High-roller Posted at: 2017-12-02T22:55:43.966Z Reads: 115

```
Yes, the blue power led is lighting up and I'm not getting any red LEDs or anything to indicate a problem. It just connects for a couple of seconds and then gets the error. I've never had this happen with any plug & play hardware before.
```

---
## \#31 Posted by: JohnnyMeduse Posted at: 2017-12-02T22:59:05.097Z Reads: 113

```
Which Firmware are you using and on which device ?
```

---
## \#32 Posted by: High-roller Posted at: 2017-12-02T23:02:59.219Z Reads: 111

```
I'm not sure which firmware, though I bought them in june so I imagine it's not outdated. Since I can't read it from the vesc-tool I don't know.
what device are you referring to?
```

---
## \#33 Posted by: JohnnyMeduse Posted at: 2017-12-02T23:19:06.607Z Reads: 105

```
There is few VESC-Tool out there... which one are you using ? (where did you download it). And on which family of device PC or MAC ?
```

---
## \#34 Posted by: High-roller Posted at: 2017-12-02T23:23:01.733Z Reads: 107

```
I tried the bldc-tool downloaded from enertion's site, akmaniac's bldc-tool, and the vesc-tool, all on a pc running windows 10.
```

---
## \#35 Posted by: JohnnyMeduse Posted at: 2017-12-02T23:31:48.702Z Reads: 108

```
I know there is some issue on MAC for Ackmaniac firmware, since I've never heard of any Issue with windows, my best guess is the same as @blasto, and is pointing to the USB cable.
```

---
## \#36 Posted by: High-roller Posted at: 2017-12-02T23:36:38.023Z Reads: 108

```
That's the thing, I tested the cable for data transfer on my phone and it worked perfectly.
```

---
## \#37 Posted by: JohnnyMeduse Posted at: 2017-12-02T23:38:28.091Z Reads: 106

```
have you try to connect it without the enclosure on the Focbox.
```

---
## \#38 Posted by: High-roller Posted at: 2017-12-02T23:42:26.854Z Reads: 108

```
You mean the cover of the focbox itself? I havn't tried that. I know @yaca solved his connection problem by grinding off some of the covering. If you really think the plug isn't reaching in far enough?
```

---
## \#39 Posted by: JohnnyMeduse Posted at: 2017-12-02T23:45:31.007Z Reads: 107

```
yeah, The cover could be too thick with certain USB Cable.
```

---
## \#40 Posted by: High-roller Posted at: 2017-12-03T00:09:18.875Z Reads: 113

```
Well, I feel kinda stupid now, since a couple of you said early on it was a bad connection. Notice the difference between these two?
<img src="/uploads/db1493/original/3X/0/9/0956a9c6195c7047f4c1f301223f85f11e4b9e59.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/c/2/c26b3ee78a8def941781a2fef62dfa46cc9242e3.jpg" width="375" height="500">
The top photo is after I pushed it in all the way, the bottom is how I saw it once the cover was off. I did indeed have to push it in a bit further.
It connected right away on the bldc-tool (version 2.18 bty), both akmaniac's and the vesc-tool timed out the first time, second time they connected and told me I need to update my firmware. I guess I'll take what I can get.
Thanks very much everybody!
@onloop could you see about maybe enlarging the USB opening to ensure full connection on future FOCboxes?
```

---
## \#41 Posted by: Mikenopolis Posted at: 2017-12-03T02:22:35.361Z Reads: 104

```
Do yourself a favor and just strip some plastic off a mini and micro USB cable. I have strip down ones just so they are guaranteed to fit and also bend a bit easier into tight spaces
```

---
## \#42 Posted by: High-roller Posted at: 2017-12-03T11:07:42.132Z Reads: 101

```
Done! They're not pretty but they work. And they're extensions, so I won't have to remove the enclosure every time.
<img src="/uploads/db1493/original/3X/6/0/60cf910f05511303cc7517d15219733351d6978c.jpg" width="375" height="499">
```

---
## \#43 Posted by: yaca Posted at: 2017-12-03T11:23:07.209Z Reads: 100

```
Glad you solved the problem. But I'm wondering why you ignored our advices a few days ago, because we clearly told you the solution.
```

---
## \#44 Posted by: High-roller Posted at: 2017-12-03T13:23:49.319Z Reads: 95

```
Mostly because I was afraid of damaging a 200$ piece equipment.
```

---
## \#45 Posted by: Lambjr088 Posted at: 2019-03-31T01:00:49.323Z Reads: 28

```
Can anyone on here help me ive tried all the above and i still get the same error. I dont have to money to buy a unity or even to fix this i really hope its a simple problem. But with my luck lately
```

---
## \#46 Posted by: High-roller Posted at: 2019-03-31T03:17:48.648Z Reads: 23

```
Which error exactly? The "no firmware read response" one?
Are you using the vesc tool or the old bldc tool?
```

---
## \#47 Posted by: Lambjr088 Posted at: 2019-03-31T15:32:21.044Z Reads: 22

```
I dont know how but it got fixed. I switched from the vesc-tool to bldc-tool and got the same error code but once i switched back to vesc-tool it read fine. Very strange lol
```

---
## \#48 Posted by: High-roller Posted at: 2019-03-31T16:40:29.280Z Reads: 19

```
Happy to help I suppose...🤔
It's possible that you just needed to make sure the USB cable was pushed in all the way, that's what my problem was. Apparently FOCboxes are known to have this issue.
I suggest you keep using the new vesc tool, the setup wizard really helps in making sure you have the right settings. Just check a video tutorial if you're not sure.
Finally, remember to set your erpm to 60000! The wizard doesn't do this so make sure you take care of it before you disconnect from your PC.
```

---
