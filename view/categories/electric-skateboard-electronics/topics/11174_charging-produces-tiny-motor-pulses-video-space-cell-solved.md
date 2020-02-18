# Charging Produces tiny motor pulses (Video) Space cell- SOLVED

### Replies: 32 Views: 2118

## \#1 Posted by: CRABOLSKY Posted at: 2016-10-15T11:00:12.203Z Reads: 145

```
I don't think this has been happening since the beginning, but tonight I noticed a strange pulsing noise coming from my my motor while charging. Space Cell, Steez remote, Enertion motor. 
Check this video but turn up the sound to hear it. 
https://www.youtube.com/watch?v=ZomDa6Uec6U

Has anyone come across this before?  I don't think it could be a remote related issue since the remote is obviously off.
```

---
## \#2 Posted by: XIII Posted at: 2016-10-15T11:13:08.424Z Reads: 140

```
My Lcd screen is off. Vesc is off aswell when charging. It seems like yours are both turned on for some reason
```

---
## \#3 Posted by: CRABOLSKY Posted at: 2016-10-15T11:16:52.706Z Reads: 132

```
Mmm curious. I seem to remember reading somewhere that it turns on to monitor the charging. I'd love to know if the screen should actually be on or not? My power switch is in the off position BTW.
```

---
## \#4 Posted by: Luke Posted at: 2016-10-15T11:36:21.160Z Reads: 131

```
if it helps, my screen is off while charging unless i power the space cell on while charging
```

---
## \#5 Posted by: Tarzan Posted at: 2016-10-15T11:47:42.711Z Reads: 126

```
The newer space cells have a different behavior while charging due to the new charge only bms.
The on/off switch should be turned off while charging in both cases.
```

---
## \#6 Posted by: CRABOLSKY Posted at: 2016-10-15T12:15:01.754Z Reads: 120

```
Thanks, that is good to know I figured it was okay... I am just a little thrown by the fact the motor is twitching as it charges.
```

---
## \#7 Posted by: CRABOLSKY Posted at: 2016-10-16T22:39:56.736Z Reads: 98

```
Hey @EnertionSupport @onloop, perhaps you can chime in here. What could be causing this phenomenon? Since its with a defined pattern, I am guessing that its related to the rate that the charge in coming into the system.
```

---
## \#8 Posted by: CRABOLSKY Posted at: 2016-10-18T22:27:59.562Z Reads: 88

```
Can anybody assist in helping me understand whats at play here? I want to make sure there isn't anything nefarious at play here.  @onloop you know this pack and BMS better than anyone can you please offer your thoughts?
```

---
## \#9 Posted by: onloop Posted at: 2016-10-19T22:55:55.658Z Reads: 79

```
this might sound like an unrelated question, but what hand controller do you have?
```

---
## \#10 Posted by: CRABOLSKY Posted at: 2016-10-19T23:23:48.168Z Reads: 75

```
Enertion Steez - which incidentally gave me problems this morning and disconnected during ride. wouldn't connect > switched pack & remote on/off > reconnected and powered on for a few seconds and then disconnected again. Walked the rest of the way.
```

---
## \#11 Posted by: CRABOLSKY Posted at: 2016-10-20T01:28:31.077Z Reads: 70

```
@onloop what do you think?
```

---
## \#12 Posted by: onloop Posted at: 2016-10-20T01:30:55.853Z Reads: 72

```


the problem is not with your battery, it's just some noise/interference with your remote.

you could try a ferrite ring
```

---
## \#13 Posted by: CRABOLSKY Posted at: 2016-10-20T01:41:17.326Z Reads: 72

```

The pulsing of the motor during charging too? 
  
As far as the remote this morning, I am not as confident that it is an interference problem... it has been working proper without any problems up until this morning. But, I will indeed explore the ferrite ring.
```

---
## \#14 Posted by: onloop Posted at: 2016-10-20T02:04:48.808Z Reads: 73

```

turn the battery on & stop charging, does the pulse occur?

if it doesn't you are getting some interference related to the charger.
```

---
## \#15 Posted by: CRABOLSKY Posted at: 2016-10-20T02:26:49.099Z Reads: 73

```

Thanks for your thoughts so far Jason.I haven't tested in that order and will do tonight and report back. 

Interference with the charger will cause a current to be sent through to the motor? The pulsing is the same pattern over and over which feels like like when ever the charger is sending power through to the battery. Or does the charger send through  constant trickle? Another thought, could it be related to the vesc having power (on this BMS) and remote receiver being tricked into thinking it receiving a signal?
```

---
## \#16 Posted by: CRABOLSKY Posted at: 2016-10-20T03:52:44.679Z Reads: 73

```
***Alright I have a big update and solution***

Even though it was very faint, noticed that the pulsing noise was actually happening even with it unplugged and the pack on. I just with the I pulled the cover and discovered that the vesc lights pulsed in the same succession at the pulsing noise. 
https://youtu.be/QLsRAnbdzjU

I knew at this point that it had to be related to the remote somehow, either with the hardware or the settings. When I unplugged the receiver of the remote, the pulsing stopped.   

I took the chip out and this happened. It looks like the module had started to become loose and then finally broke free. I would say this is the cause of this anomaly. Jason, should this be tossed now or do you think it could be re-soldered? 
<img src="/uploads/db1493/original/3X/2/9/29bb9593113d3dcd76abd5b579a2a8522c0a964a.JPG" width="375" height="500">...
```

---
## \#17 Posted by: onloop Posted at: 2016-10-20T03:53:58.860Z Reads: 71

```
IT CAN LIKELY BE RESOLDERED :slight_smile:

add some glue too to prevent the vibrations from destroying it
```

---
## \#18 Posted by: Rye Posted at: 2016-10-21T11:04:14.425Z Reads: 62

```
@onloop would this not be a warranty job Jason? Just curious as if it was me and a circuit board fell apart after minimal use, I'd be asking for a repair or replacement. Only a question mate, I don't want to be smashed for asking on behalf of someone else 👍 I've bought plenty of kit from Enertion and personally haven't had an issue with the quality so far. Generally I've been impressed with enertions corrections if things don't go to plan. Cheers mate.
```

---
## \#19 Posted by: onloop Posted at: 2016-10-21T11:30:59.530Z Reads: 63

```
[quote="Rye, post:18, topic:11174"]
@onloop would this not be a warranty job Jason?
[/quote]

If this was a raptor we would replace it, we offer 12 months instant replacement warranty on all raptors.
As this part has been installed by end user it has a limited 60 days warranty that covers DOA type manufacturing faults.
I know that sucks to say but that's the nature of DIY stuff, there is a limited amount of responsibility left in the vendors hands when they are not the ones doing the final install.

This fault above is commonly related to vibrations together with time, the solder eventually snaps as the weight of the RF chip leverages it up & down & vibrates. I have asked the factory to resolve this issue by changing their design, they didn't really listen. So we are left up to our own to use installation methods that prevent vibration damage.

We found that using glue & a shrink tube sleeve helped make them last longer. Vibrations are actually one of the biggest killers of electronics.

I suppose If the part is returned to us we could try to fix it. There would be a return postage cost. Normally due to the massive ocean between Australia & our customers countries this is rarely a viable option. Australian based customer will do it from time to time, but there is still a postage cost.

Alternatively, it could be sent back to china to the factory that made it, they will resolder it, but postage charges make it non viable.

The good news is this can probably be fixed with some solder & hot glue.
```

---
## \#20 Posted by: Rye Posted at: 2016-10-21T11:52:14.362Z Reads: 54

```
Wow, quite the answer there. Good to know where you stand I guess. Cheers for the quick response.
```

---
## \#21 Posted by: onloop Posted at: 2016-10-21T12:01:20.740Z Reads: 51

```
In simple terms. If we build it we take full responsibility for faults first 12 months. 

If we didn't build it there must be proof it's DOA / manufacturing fault provided in writing/video/photo in first 60 days.

This is the best we can offer at this stage.
```

---
## \#22 Posted by: racidon Posted at: 2016-10-21T12:08:18.061Z Reads: 47

```
[quote="onloop, post:21, topic:11174, full:true"]
In simple terms. If we build it we take full responsibility for faults first 12 months. 

If we didn't build it there must be proof it's DOA / manufacturing fault provided in writing/video/photo in first 60 days.

This is the best we can offer at this stage.
[/quote]
How does one go about proving it though with electronics?
```

---
## \#23 Posted by: onloop Posted at: 2016-10-21T12:22:44.079Z Reads: 50

```
[quote="racidon, post:22, topic:11174"]
How does one go about proving it though with electronics?
[/quote]

in 95% of cases DOA & manufacturing faults will be identified immediately, because they don't work. 
If several weeks of product use have passed & a fault occurs it becomes difficult to prove it is DOA/Manufacturing. Which normally means it is not DOA or Manufacturing fault... Of course, every case is different.

Our long term goal is to offer instant replacement warranty on all faults for 12 months. But it will be on kits that we have assembled, so it starts moving away from DIY.
```

---
## \#24 Posted by: CRABOLSKY Posted at: 2016-10-21T12:44:44.022Z Reads: 48

```
Many thanks for for the flag @Rye and your response @onloop.

To be frank, I don't think that the quality of this remote equals its cost and I can see why you moved on from this one. The receiver and remote have both failed in under 3 weeks of actual riding time. The remote B button came loose (during shipping) which I repaired before I even used it for the first time, and this chip issue happened within the first 60km of riding.  I had it in my possession for over 4 months but its only been actually used for 3 weeks. 

I do understand the necessary limitations you need to put on DIY scenarios... you can't be expected to cover user error or neglect. I for one would have taken Maytec to task over the build quality of this and asked for them to send you replacement parts to have on hand for these scenarios (Raptor or otherwise). 

I will give it my best shot to try and bring it back to life with some amateur-yet inspired soldering. Wish me luck.
```

---
## \#25 Posted by: CRABOLSKY Posted at: 2016-10-24T02:36:20.104Z Reads: 39

```
So after a good 2+ Hours of very finicky soldering I came up with the attached solution. Actually is was @lox897 idea for the jumpers! The pulsing issue seems to have been resolved. 

It looked like there could have been 1 or 2 small areas that potentially could have short circuited but it's works again, with no apparent issues. I've added hot glue across the stress points as well.
```

---
## \#26 Posted by: CRABOLSKY Posted at: 2016-10-24T02:55:48.478Z Reads: 38

```
<img src="/uploads/db1493/original/3X/0/4/0415a75ee5ef1fcc256d5f57ae1c3288a7c7f740.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/d/9/d9c340b4c1b8dddb402f33871a7422b187fd4567.JPG" width="375" height="500">
```

---
## \#27 Posted by: onloop Posted at: 2016-10-24T10:17:08.458Z Reads: 34

```
great work, you should be proud of that effort.
```

---
## \#28 Posted by: CRABOLSKY Posted at: 2016-10-24T10:29:38.047Z Reads: 34

```
Thanks @onloop . I've just been charging it, and the pulsing thing still occurs while charging or just Turned on. It is in the same rhythm as the vesc lights too. Could be the receiver chip is just playing up? 🤔
```

---
## \#29 Posted by: evoheyax Posted at: 2016-10-24T15:52:39.390Z Reads: 29

```
I've had 3 steeze receivers break like this... This, along with the poor braking curve, is why I've moved away from it and I'm now using the mini 2.4ghz remote many are selling on this forum. Had no issues so far with that remote, and it's a fraction of the price.
```

---
## \#30 Posted by: CRABOLSKY Posted at: 2016-10-25T12:05:13.233Z Reads: 28

```
Well @evoheyax I took out the board for a quick blast today and it seems as though the chip has finally given up. Bummer though... thought I'd worked it out with the jumper solution. I am guessing its more than just the connection. Just glad it didn't cut out when going top speed.
```

---
## \#31 Posted by: evoheyax Posted at: 2016-10-25T15:25:07.501Z Reads: 23

```
Bummer, I was hoping this might work. It looks like a nice solder job.

I still haven't found the perfect solution in my mind. I like to solder everything for reliability, and that was easy with the steez. Just de-solder the ppm thing on the receiver, and solder straight through the pcb and straight through the vesc, most reliable connection I've ever had. But as I found out the hard way with the 2.4 ghz mini remote most are using, I tried, but the components as like epoxied to the case of the receiver, and when I tried to get it off, I ripped parts off the receiver board, so you have to using a ppm cable.

I wonder how the nano-x is...
```

---
## \#32 Posted by: CRABOLSKY Posted at: 2016-11-06T11:13:25.157Z Reads: 21

```
Many thanks to @onloop for sourcing a replacement receiver chip for the steeze. 

I've resorted to making my own case and additional hot glue to ensure a well supported chip. 3D printer pen to the rescue. It ain't pretty but it will do. 

<img src="/uploads/db1493/original/3X/2/1/21373fd8839a1fbc1529bec150e0d809a1b4a750.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/3/0/30ccdb3d6f5498cece5ca0a0154f571cbdbdbd64.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/c/c/cc90bf9d8e3955b4b20d08640ca5630a39da1a3d.JPG" width="666" height="500">
```

---
