# Going over options to connect two VESCs to remote

### Replies: 50 Views: 4228

## \#1 Posted by: cryo Posted at: 2017-08-13T06:27:11.454Z Reads: 302

```
So I've been doing a lot of research on how to get dual VESCs working and from what I gather there are 3 options.

1) Split Y ppm
2) CANBUS
3) Benchwheel 2 Channel receiver

After reading that huge thread on y-cable vs CANBUS, I really would like to go with option 3 since both 1) and 2) can potentially damage/kill the VESC. I'm suprised theres not much info on option three but its from this [post](https://www.electric-skateboard.builders/t/benchwheel-remote-receiver/14171/2?u=cryo) by @Luke 

Has anyone with the benchwheel remote tried Lukes way? Is it as simple as connecting the two VESCs to one receiver without having to worry about frying VESC? Also Lukes post seems to reference an older version of the benchwheel receiver since it looks different on aliexpress currently [here](https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-DIY-800MAH-remote-receiver-2-4G-bench-technology-benchwheel/32791243047.html?ws_ab_test=searchweb0_0,searchweb201602_4_10152_10065_10151_10068_10130_10084_10083_10080_10307_10082_10081_10110_10178_10137_10111_10060_10112_10113_10155_10114_10154_10056_10055_10054_10312_10313_10059_10314_10315_10316_100031_10099_10078_10079_10103_10073_10102_10052_10053_10142_10107_10050_10051-10052_10112,searchweb201603_2,ppcSwitch_5&btsid=93beebdc-3a81-4a27-a70a-83d789c68820&algo_expid=76554a39-d9fe-4e73-ade6-f2710f01bf7c-1&algo_pvid=76554a39-d9fe-4e73-ade6-f2710f01bf7c&transAbTest=ae803_3). Not sure if it can still be done.
```

---
## \#2 Posted by: pennyboard Posted at: 2017-08-13T06:31:57.711Z Reads: 290

```
I use the split Y. It has worked great for me, because I made sure to cut the power cable on one of the wires. As long as you do that it should be safe.

The reason I didn't use canbus is that if one vesc dies, it takes the other down with it.
```

---
## \#3 Posted by: cryo Posted at: 2017-08-13T06:36:12.749Z Reads: 287

```
Yea split Y is my secondary option, too many anecdotes of it [frying](https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461/124?u=cryo) and getting broken during a ride. Even if it's recommended by Vedder I'll have to side with peoples experiences on the forum and avoid CANBUS.

Though I would still very much like to try option 3 if possible :sweat_smile:
```

---
## \#4 Posted by: Fatglottis Posted at: 2017-08-13T07:03:48.923Z Reads: 276

```
4) dual Vesc connected to a TeensyLC using UART. 

I have a home made nunchuck with an arduino NANO which communicates with the TeensyLC on the board. The VESCs are running independently of each other. I have all vesc data sent to the remote now. 
I found information about how to achieve this ...some guy named rolling gecho did the base of the code.

it was my second arduino based project and it took some time get it working (but it was lots of fun)
```

---
## \#5 Posted by: cryo Posted at: 2017-08-13T07:22:25.028Z Reads: 261

```
that sounds legit. I do prefer the regular esk8 remotes form factors over nunchuks tho.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-13T07:43:23.047Z Reads: 264

```
Option 4: Multiple receivers with one controller.
The Mini RC controller is able to sinc to and operate multiple receivers.
Zero risk of damage to vesc and maximum redundancy.
This could really simplify quad drive setups.

<img src="/uploads/db1493/original/3X/3/7/37f20873777edffc539257a55a65f6c6adbcce78.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/3X/f/e/fef7aae4ae7086512e2da8f19c844ad4f5b7057c.jpeg" width="375" height="500">

https://youtu.be/eSeTWe-GI8U
https://youtu.be/tmtM8fGZYa0
```

---
## \#7 Posted by: cryo Posted at: 2017-08-13T08:13:34.366Z Reads: 253

```
wow exactly what i was looking for. nice and simple with maximum safety for my precious parts. Even though the remote is ugly as hell i think i will go with this
```

---
## \#8 Posted by: Namasaki Posted at: 2017-08-13T08:17:06.648Z Reads: 256

```
If you remove the wheel and grind down the wheel post, its not as bad.<img src="/uploads/db1493/original/3X/0/7/07761aef580c174094ef1a9446b1a24a0f4305bc.jpeg" width="375" height="500">

You can buy receivers without the remote at torqueboards.
Might not be a bad idea to just buy 2 sets and have a spare remote just in case.
diy-electric-skateboard-kits-parts/2-4ghz-mini-receiver/
```

---
## \#9 Posted by: lrdesigns Posted at: 2017-08-13T08:41:09.925Z Reads: 248

```
Can a GT2b bind to multiple receivers?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-08-13T08:43:33.210Z Reads: 247

```
Cant say for sure because I haven't tested that one but I would not be surprised if it could since its a 2.4ghz transmitter.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-08-13T08:44:58.625Z Reads: 248

```
As far as setting it up. You want to power up and bind each receiver one at a time with the other receiver/s off.
After going through the binding process on each receiver, then you can turn them all on and test it.
```

---
## \#12 Posted by: Tomer Posted at: 2017-08-13T11:41:33.342Z Reads: 239

```
FYI - The Benchwheel receiver showed in Aliexpress is actually the old model, the one Luke uses is the updated version.
```

---
## \#13 Posted by: cryo Posted at: 2017-08-13T12:29:02.772Z Reads: 232

```
ok thanks, good to know. I've decided to go with Namasakis option as its cheaper and easier. Out of curiousity, is the benchwheel setup just plugging two vescs into the receiver?
```

---
## \#14 Posted by: Tomer Posted at: 2017-08-13T13:05:58.698Z Reads: 229

```
I'm interested to know too. I have no idea how this suppose to work.
When I synced my remote, I was able to do it only via channel number 1, if I'm not mistaken.
But when I tried to connect it to the 2nd channel, I wasn't able to sync the remote.
```

---
## \#15 Posted by: flywithgriff Posted at: 2017-08-13T13:17:08.584Z Reads: 227

```
I have a benchwheel from @oriol360 who is MEB and he said that I would be fine running it with dual vesc. Just plug them both in and rock on.
```

---
## \#16 Posted by: Jinra Posted at: 2017-08-13T16:46:47.908Z Reads: 222

```
the benchwheel remote is essentially split ppm. I've never heard of anyone breaking a vesc from split ppm despite trampas claims
```

---
## \#17 Posted by: L3chef Posted at: 2017-08-13T16:53:20.319Z Reads: 217

```
What the heck is that wheel for?
```

---
## \#18 Posted by: Jinra Posted at: 2017-08-13T16:53:47.028Z Reads: 211

```
Turning on an rc car
```

---
## \#19 Posted by: L3chef Posted at: 2017-08-13T16:54:59.368Z Reads: 210

```
Ah ok.
Ten char
```

---
## \#20 Posted by: Namasaki Posted at: 2017-08-13T17:31:39.159Z Reads: 219

```
I'm running split PPM on 2 builds with no issues but I cut the 5v wire from one of the Vesc. 
There has been report of damage when trying to supply 5v from both Vescs.

I would guess that the same is true when connecting 2 Vescs to one receiver.
```

---
## \#21 Posted by: Jinra Posted at: 2017-08-13T17:40:57.245Z Reads: 207

```
Actually the Benchwheel, while having double sets of pins for 2 ESCs, has 1 of the 5v pins cut as well. The pin is there, but supplies no voltage.
```

---
## \#22 Posted by: flywithgriff Posted at: 2017-08-13T18:10:28.211Z Reads: 206

```
Thank you, I was curious about this!
```

---
## \#23 Posted by: SeanHacker Posted at: 2017-08-13T18:12:55.406Z Reads: 204

```
Yes it can. I use one GT2B for to different boards.
```

---
## \#24 Posted by: Silverline Posted at: 2017-08-13T18:17:09.508Z Reads: 208

```
Nice info thanks :slight_smile:
Where do you buy extra receivers ?
```

---
## \#25 Posted by: SeanHacker Posted at: 2017-08-13T18:18:11.099Z Reads: 206

```
https://www.amazon.com/FS-GR3E-Receiver-FS-GT2B-FS-GT3B-FS-GT3C/dp/B00IZUIHPM/ref=pd_sim_21_1?_encoding=UTF8&pd_rd_i=B00IZUIHPM&pd_rd_r=DGMQMFP3TDY7XREDQTMR&pd_rd_w=3MpRv&pd_rd_wg=GbKjW&psc=1&refRID=DGMQMFP3TDY7XREDQTMR
```

---
## \#26 Posted by: bigben Posted at: 2017-08-13T18:56:16.485Z Reads: 200

```
https://www.banggood.com/2_4GHz-Radio-Remote-Controller-Receiver-Transmitter-For-Electric-Skateboard-p-1125575.html?rmmds=search
```

---
## \#27 Posted by: Silverline Posted at: 2017-08-13T19:30:39.074Z Reads: 190

```
Thanks guys. 
Ordered one more flysky rx.
```

---
## \#28 Posted by: cryo Posted at: 2017-08-14T03:18:41.176Z Reads: 189

```
seems @jinra is right, the top 3 pins has the 5v pin closed according to this [pic](https://ae01.alicdn.com/kf/UT8Y2wlX5lbXXagOFbXx.jpg) of the included instructions.

The question now is whether I should cancel my orders and spend an extra 15 on a better looking remote :confounded:
```

---
## \#29 Posted by: lrdesigns Posted at: 2017-08-14T04:46:49.355Z Reads: 192

```
[quote="SeanHacker, post:23, topic:30484, full:true"]
Yes it can. I use one GT2B for two different boards.
[/quote] Thanks good to know! A dual receiver setup sounds like a good extra level of redundancy. Its almost like having a diversity receiver. The hobbyking spare GT2b receiver can be found here. 

https://hobbyking.com/en_us/hobbykingr-tm-gt-2-2-4ghz-receiver-3ch.html
```

---
## \#30 Posted by: Luke Posted at: 2017-08-14T08:31:19.644Z Reads: 191

```
[quote="cryo, post:1, topic:30484"]
I'm suprised theres not much info on option three but its from this post by @Luke
[/quote]
Hey :) It worked with no issues for me. I guess not that many people have benchwheel remotes so not many people tried it. Looks like that dual receiver option is pretty ideal though ! Best of luck with whichever one you end up going with
```

---
## \#31 Posted by: Tomer Posted at: 2017-08-14T08:35:42.840Z Reads: 186

```
Just to double verify - if I connect the 2nd VESC to the Benchwheel receiver, should I cut the 5v cable or I can leave it as it is?

Thanks.
```

---
## \#32 Posted by: Luke Posted at: 2017-08-14T08:39:41.625Z Reads: 181

```
I didnt know anything about this 5v pin. I just had both vescs plugged in as normal as an experiment and it worked. Mind you this was about October last year so the receiver may have changed.
I lost my remote since then and chenged to the mini remote with the wheel on it. I think I prefer the bench wheel however.
```

---
## \#33 Posted by: flywithgriff Posted at: 2017-08-14T12:00:42.274Z Reads: 170

```
Do not cut anything for the benchwheel.
```

---
## \#34 Posted by: High-roller Posted at: 2017-08-14T20:37:18.262Z Reads: 164

```
Glad I found this thread before I hooked up a CANBUS cable to my brand new FOCboxes!
So I've read up on it a bit and I think I understand the danger with the canbus (if one vesc fails, they both do), but what's the risk of the y-cable? Is it just the overpowering because of the two 5v sources, hence cutting one of the wires?
With the canbus, aside from configuring wrong and designating one VESC the slave too early in the process, is there any actual risk?
```

---
## \#35 Posted by: lrdesigns Posted at: 2017-08-14T23:05:13.781Z Reads: 162

```
I don't think any user here reported an issue with y cable on v4 vesc. It just veder said it's a bad idea with vesc 6. 

With y cable you only need one wire PPM to the second vesc and both should be setup as master.
```

---
## \#36 Posted by: torqueboards Posted at: 2017-08-15T03:17:50.180Z Reads: 157

```
@High-roller Canbus works perfectly fine on 2wd.
Canbus can be an issue when running 4wd.
```

---
## \#37 Posted by: High-roller Posted at: 2017-08-15T12:54:38.313Z Reads: 160

```
Thanks for the reassurance. Still, I can't help but worry, now that I know it can happen. Is there any real advantage to it over the y-cable? There are other ways to get real-time data and I don't know how much of a difference having traction control makes.
@Irdesigns what about the FOCbox, which is supposed to be somewhere in between? I think I read somewhere that it's a sort of VESC 5...?
```

---
## \#38 Posted by: mmaner Posted at: 2017-08-15T14:08:13.120Z Reads: 161

```
Telemetry via bluetooth can only be had for both VESC(s) if you use canbus.  Traction control can only be had if you use canbus.  
http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142
```

---
## \#39 Posted by: flywithgriff Posted at: 2017-08-15T14:33:02.008Z Reads: 153

```
I am using the benchwheel so I can just plug both FOCBOX into the receiver. I plan to run a Bluetooth module on one FOCBOX for info. My enclosure is easy to remove so I can tune them without much trouble.

Edit: I do have a canbus cable on my workbench... maybe I should go with canbus... this is a tough decision!
```

---
## \#40 Posted by: High-roller Posted at: 2017-08-15T16:15:53.453Z Reads: 153

```
Let me know what you decide. I don't want to lose two vescs because I didn't connect a cable before naming them or something else equally trivial.
```

---
## \#41 Posted by: flywithgriff Posted at: 2017-08-15T18:06:21.304Z Reads: 149

```
That's the reason I'm cautious of canbus!
```

---
## \#42 Posted by: torqueboards Posted at: 2017-08-16T04:30:11.570Z Reads: 147

```
lol.. Don't touch it! It's a canbus!

You'll be fine..
```

---
## \#43 Posted by: Jinra Posted at: 2017-08-16T04:48:19.207Z Reads: 147

```
watch out!

https://img0.etsystatic.com/020/1/6343239/il_340x270.552777742_oyw4.jpg
```

---
## \#44 Posted by: flywithgriff Posted at: 2017-08-16T12:51:56.053Z Reads: 137

```
lol I'm not literally concerned with the cable. I'm concerned about screwing up the setting and frying a new focbox.
```

---
## \#45 Posted by: High-roller Posted at: 2017-08-16T13:10:05.847Z Reads: 134

```
I'm leaning towards the y-cable option. Maybe I'll switch to the CANbus when I grow up esk8-wise ;-)
```

---
## \#46 Posted by: flywithgriff Posted at: 2017-08-16T13:11:06.047Z Reads: 131

```
The only reason I'm even considering canbus is for using the app for configuring vs taking enclosure off and attaching usb.
```

---
## \#47 Posted by: High-roller Posted at: 2017-08-16T13:13:36.756Z Reads: 128

```
Couldn't you just drill a USB sized hole in your enclosure and position your vesc for it?
```

---
## \#48 Posted by: flywithgriff Posted at: 2017-08-16T13:14:23.801Z Reads: 124

```
I have made extension cables and mounted them in the enclosure in the past. Just trying to clean up the build a bit.
```

---
## \#49 Posted by: Mikenopolis Posted at: 2017-08-23T18:38:30.079Z Reads: 115

```
Don't have a picture of mine. I took shaved off that numb all the way down until it was flat and slapped on an NFC tag. that is set up to open a GPS app on my Android phone
```

---
## \#50 Posted by: RoG17 Posted at: 2019-11-27T10:42:37.240Z Reads: 6

```
Can we pair Excellway® 2.4GHz Radio Remote Controller with HobbyKing® ™ GT-2 2.4Ghz Receiver 3Ch.
```

---
