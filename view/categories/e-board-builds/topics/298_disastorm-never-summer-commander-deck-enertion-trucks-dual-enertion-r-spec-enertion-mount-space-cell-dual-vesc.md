# Disastorm &#124; Never Summer Commander Deck &#124; Enertion Trucks &#124; Dual Enertion R-Spec &#124; Enertion Mount&#124; Space Cell &#124; Dual VESC

### Replies: 67 Views: 9136

## \#1 Posted by: disastorm Posted at: 2015-10-10T04:40:45.679Z Reads: 296

```
Hello, I was recently thinking about building an electric longboard to use as local transportation here in san francisco. I'm new to boarding and don't really have experience with either electric or non-electric boards. I could probably just buy a pre-made one but I thought it would be interesting to build my own. Anyway, I've been reading up on building an electric longboard via some sites and forums and wanted to see what people think of the following:

enertion Space CELL battery - seems really convenient since it comes with charging stuff, voltage display, battery management system, and on/off switch

carvon dual hub motors

dual VESC - Anyone know what the best place to get it is? I've seen it on various sites like enertionboards.com and ollinboardcompany.com

It seems different people make VESC, but they are all the same device right?

As I am also new to boarding, I don't know all the differences between different board shapes and whatnot- although I've read through the guide on here and muirskate.com 
It seems its best to get a top mount, stiff, with not much concave ?

Do you guys think any of these will be suitable for an electric longboard?
https://www.muirskate.com/longboard/decks/70202/never-summer-2015-commander-longboard-skateboard-deck-w-grip ( this one seems to have some concave )
https://www.muirskate.com/longboard/decks/70490/omen-sunsets-longboard-skateboard-deck-w-grip

Also, it seems VESC can connect with the wireless Nyko Kama Wii Nunchuck? How exactly do you connect them together? Also if you have 2 VESC, can a single Nunchuck control both of them ?

And I saw someone used a screw box for an enclosure, so I was thinking I would try that for everything except the battery, since the Space Cell seems like its already in its own enclosure.

Is there anything else I need to know?

Thanks.
```

---
## \#2 Posted by: lox897 Posted at: 2015-10-10T05:11:35.106Z Reads: 258

```
VESC are all the effectively the same. Get the commander board. Lots of people get VESC from enertion, marcin on endless sphere and jacobbbloy on endless sphere. Have a look at the for sale (new) section on endless sphere.
As for the nyko kama you can connect with wiiceiver or connect directly to board with some soldering (the soldering method seems to loose connection LESS)

Screw box would be cool. Or you could get psychotillers abs enclosures. Coming along well, nice job! Be sure to make a build thread when you get some parts! PS: What motor mount are you getting?
```

---
## \#3 Posted by: lox897 Posted at: 2015-10-10T05:12:29.765Z Reads: 248

```
Connect the VESC over CANBUS or get a Servo Y splitter. One nunchuck can control both motors yes.
```

---
## \#4 Posted by: emotiva Posted at: 2015-10-10T05:22:17.158Z Reads: 262

```
Full disclosure: I have yet to assemble a board, so don't take my reply as gospel. That said, I've spent an inordinate amount of time reading about it lately, and think I can help with some of your questions. 

[quote="disastorm, post:1, topic:298"]
It seems different people make VESC, but they are all the same device right?
[/quote] Broadly, yes, but the version number and state of completion might vary depending on who you purchase from. For instance, I ordered one from Enertion (V 4.8) while Jason was away, and have recently been notified that he's cancelled the latest run of 4.8 to move on to Vedder's latest 4.10 version. Some sellers are still offering 4.8. How significant the changes are to general experience, I'm unsure, but there's a change log on GitHub as well as a post somewhere about it. I can try to track it down if you can't find it. My impression is that it's a small but non-trivial iteration.

[quote="disastorm, post:1, topic:298"]
Also, it seems VESC can connect with the wireless Nyko Kama Wii Nunchuck? How exactly do you connect them together?
[/quote]

VESC can utilize the Nyko Kama nunchuck. This might be helpful: http://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139 . From what I've read, some people have experienced intermittent connectivity issues except in the cases where they soldered the jst connector wires directly to the receiver. Of the 3 or so reports I've read of a soldered receiver, connectivity has been reported as completely reliable. The other popular option is the Hobby King 2.4GHz GTB2 or Flysky transmitter/receiver, which seems to be universally well-regarded with respect to reliability, though it's larger and lacks a cruise control fuction. Lots of posts regarding both of these setups exist.

[quote="disastorm, post:1, topic:298"]
Also if you have 2 VESC, can a single Nunchuck control both of them ?
[/quote]

2 VESCs can be connected via CAN bus connection and controlled by a single nunchuck.

[quote="disastorm, post:1, topic:298"]
Do you guys think any of these will be suitable for an electric longboard? ... And I saw someone used a screw box for an enclosure, so I was thinking I would try that for everything except the battery, since the Space Cell seems like its already in its own enclosure.
[/quote]

All I can personally offer, here, is that it's a good idea to measure / map out your hardware layout to determine how much space you need to mount it all (allowing for motor mounts, enclosure, etc) and make sure the board you buy can accommodate it. It seems to me that boards in the 38" and up range are generally safe, but of course, it's really the wheelbase size that matters. Some successful builds have been achieved with shorter boards. Also, a flat-ish, stiff deck will simplify hardware mounting. Don't forget to consider clearance needed to avoid scraping your components on the ground (e.g. drop down / drop through boards will be more likely to cause clearance issues but are possible with larger wheels). 

I'm sure others will help answer your remaining questions and address anything I might be incorrect about.
```

---
## \#5 Posted by: onloop Posted at: 2015-10-10T05:37:26.473Z Reads: 218

```
[quote="emotiva, post:4, topic:298"]
My impression is that it's a small but non-trivial iteration.
[/quote]

@emotiva firstly let me say that was a great reply... its detailed answer like this that help make our forum awesome!

Regarding the Version v4.8 to v4.9 to v4.10 it's actually some of the biggest changes made yet by BV... but what does it mean in the real world to most of us riding around our eboards?.... not much!..... However everyone is definitely better off with this new version, it is definitely better on a technical level... The VESC product is only getting better!

The v4.10 from enertion (the late october batch) will be the most complete version yet! it will basically be plug & play with the space cell & r-spec motors. I will preload R-SPEC parameters and make all the necessary adjustments for optimal performance with Space Cell.

@disastorm to learn about connecting two vesc together read this: http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142
```

---
## \#6 Posted by: disastorm Posted at: 2015-10-10T06:20:06.284Z Reads: 203

```
Thanks for the info guys. What do you guys think about the belted motors vs hub motors. The hub motors I've seen for sale are on endless sphere forum, but his website is www.carvonskates.com . Is he the main hub motor guy or are there other makers as well ? Is there any disadvantage to them? 

* edit it looks like hes temporarily stopped selling them. In that case, are the R-SPEC motors good to get along with enertion's dual motor mount kit? Are the enertion trucks and wheels neccessary, what is special about them? Are they easier to connect with the enertion r-spec motor?

lox when you say you can connect the nyko kama's receiver directly to the board with soldering, why would someone choose to have a wiiceiver in between then? Does it give additional features?
So using either the Nyko Kama or the GT2B requires the soldering of pcbs together ? Are any of them easier to connect/setup or they are about the same?
```

---
## \#7 Posted by: torqueboards Posted at: 2015-10-10T08:19:49.935Z Reads: 196

```
I ride in SF in around Financial District/Chinatown/North Beach district area. Occasionally, I'll scale close to 30% inclines and I'm usually riding a Dual Diagonal Motor 10S/12S setup which is more then enough to climb hills.

I have pediglide hub motors also but have yet to test them out uphill..

I'm hoping to get another test board built soon so I can test..

Good luck on your build.. See you riding! There's more an more people riding everyday which is interesting..

About a year ago people looked at me like an Alien.
```

---
## \#8 Posted by: disastorm Posted at: 2015-10-10T20:39:30.106Z Reads: 209

```
@onloop  Hey so I am considering buying alot of the stuff from your site, but since your epower kit is no longer offered, the guide video is outdated right?

I found this thread where someone was figuring out how to put together everything: http://www.electric-skateboard.builders/t/enertion-diy-assembly-help/221/21

It looks like there was a set of VESCs that didn't come pre-soldered? Will October's release require any soldering or will it come presoldered? Will it come with an XT-60 connector so it can be easily connected to the Space Cell ?
Also the battery comes with a slow charger (without the upgrade)? How does it work, does it just plug into the wall?

So from reading everything, this seems to be the full process:
Assemble the enertion motors as shown in the youtube video.
Connect each of them to a VESC via bullet connectors. Connect the VESCs together via CANBUS. One VESC should be connected to the wireless receiver. Both VESC power wires with capacitors should be merged together into a single wire ( just solder both of them to the same XT-60 right ? ) which then connects to the Space Cell via XT-60 connector. Finally I guess all that stuff needs an enclosure and then needs to be mounted.

In the previously mentioned thread, someone mentioned that @psychotiller has a nice enclosure made for VESCs and the Space Cell?

Also, since I'm new to this, can you guys tell me if you think there would be any problem using this board: 
https://www.muirskate.com/longboard/decks/70202/never-summer-2015-commander-longboard-skateboard-deck-w-grip

The wheelbase seems pretty sizable, 27.5 - 28.5 inches , the only thing is that there is a concave, although I'm not sure how much of an issue that is.
```

---
## \#9 Posted by: lox897 Posted at: 2015-10-10T21:22:10.175Z Reads: 187

```
Because with wiiceiver there is no soldering required.
```

---
## \#10 Posted by: lox897 Posted at: 2015-10-10T21:23:22.867Z Reads: 187

```
That deck looks good! It has a W concave so you can mount things on the 2 flat bits.
```

---
## \#11 Posted by: disastorm Posted at: 2015-10-10T21:25:57.153Z Reads: 185

```
I see thanks for the info!
```

---
## \#12 Posted by: elkick Posted at: 2015-10-10T21:42:14.886Z Reads: 181

```
Thought he was using a VESC, why should he then buy a wiiceiver? 

If so, to connect the Kama nunchuck receiver to the VESC only 4 small wires need to be soldered.
```

---
## \#13 Posted by: disastorm Posted at: 2015-10-10T21:48:27.897Z Reads: 173

```
Yes that is what I will do. I was asking earlier what the point of using a wiiceiver was and he was just answering saying that I guess some people use it because no soldering is required.

Btw should I get risers or is that not neccessary ?
```

---
## \#14 Posted by: lox897 Posted at: 2015-10-10T22:01:02.341Z Reads: 175

```
I have them but it looks like a giant. They give more clearance though so that's a bonus.
```

---
## \#15 Posted by: disastorm Posted at: 2015-10-10T22:02:47.327Z Reads: 173

```
Well I'm going to use a top mount so I should have enough clearance already right?
```

---
## \#16 Posted by: lox897 Posted at: 2015-10-10T22:06:17.828Z Reads: 172

```
Sorry, I don't really know what a top mount is. I am not much of a skater I like the electronics side more.
```

---
## \#17 Posted by: disastorm Posted at: 2015-10-10T22:23:56.933Z Reads: 180

```
I'm not either. Top mount just means you mount the trucks under the board instead of part of it going through the board.
```

---
## \#18 Posted by: emotiva Posted at: 2015-10-10T22:25:30.570Z Reads: 203

```
[quote="disastorm, post:15, topic:298, full:true"]
Well I'm going to use a top mount so I should have enough clearance already right?
[/quote]

Top-mount will certainly help with clearance. Other than the board shape (drop, etc) and trucks, having enough clearance depends on the size of the wheels, motor mount position, thickness of batteries, and enclosure. Given that the SPACE cell (and the enclosure you referenced) is quite thin, you should be fine, but best to calculate everything and make sure. If you haven't already, see onloop's post here about board shape and space required: http://www.electric-skateboard.builders/t/what-deck-is-best-for-building-your-own-electric-skateboard/30 . He states 170mm needed for mounting motor and wiring. Add that to the length of the enclosure you want to mount and make sure there's enough clearance from front trucks.
```

---
## \#19 Posted by: emotiva Posted at: 2015-10-10T22:29:47.421Z Reads: 213

```
[quote="onloop, post:5, topic:298"]
[Enertion VESC] will basically be plug & play with the space cell & r-spec motors. I will preload R-SPEC parameters and make all the necessary adjustments for optimal performance with Space Cell.
[/quote]

That's great! It will be nice to begin with a common, vetted configuration.
```

---
## \#20 Posted by: disastorm Posted at: 2015-10-10T22:36:16.776Z Reads: 213

```
Are there places to get enclosures or should I just use a random piece of tupperwear or box or something. Also, how do people attach enclosures, batteries, etc to the board, do they bolt them in, glue them, I've something about velcro before also?
```

---
## \#21 Posted by: onloop Posted at: 2015-10-10T22:40:21.069Z Reads: 210

```
@disastorm sounds like you've got it mostly worked out in your head.

There will always be those moments during a build when you get stuck. So you simply need to create a build thread on here and post photos illustrating your questions.

Eventually I'll do a new video showing the latest generation of enertion parts being used to build a complete deck...

Maybe in 2-3 weeks I'll get a chance to do that.

**Read this article about choosing a deck:** 
http://www.electric-skateboard.builders/t/what-deck-is-best-for-building-your-own-electric-skateboard/30
```

---
## \#22 Posted by: disastorm Posted at: 2015-10-10T23:06:45.755Z Reads: 183

```
Thanks. Will the VESCs from later this month come pre soldered and with a XT-60 connector or would I have to do that?
```

---
## \#23 Posted by: onloop Posted at: 2015-10-10T23:08:48.514Z Reads: 184

```
that's the plan!

however don't 100% count on not soldering, there will always be some soldering of something...
```

---
## \#24 Posted by: disastorm Posted at: 2015-10-10T23:09:50.733Z Reads: 176

```
Ok thanks for the info. Yea I'll have to at least solder the nyko wireless receiver anyway.
When you said you will pre-load the RSPEC parameters, does that mean we won't need to do any kind of configuration to the VESC ourselves provided we use those motors?
```

---
## \#25 Posted by: onloop Posted at: 2015-10-10T23:12:41.762Z Reads: 166

```
If you buy the R-SPEC motors, they come with 5.5mm male connectors soldered to the phase wires already, they also have the female connectors included which WILL need to be soldered onto the VESC phase wires...
```

---
## \#26 Posted by: disastorm Posted at: 2015-10-10T23:23:57.905Z Reads: 174

```
Thanks Ok I've think I've decided on almost everything. I guess the last thing is what is the advantage of dual motors over single motors? Is it mainly just for stuff like climbing hills?
```

---
## \#27 Posted by: onloop Posted at: 2015-10-10T23:30:52.690Z Reads: 186

```
please use search more :smile:
http://www.electric-skateboard.builders/t/are-dual-motors-actually-worth-the-extra-cost/21
```

---
## \#28 Posted by: psychotiller Posted at: 2015-10-11T02:23:21.218Z Reads: 189

```
http://m.ebay.com/itm/Low-Profile-Electric-Longboard-Enclosure-/171936689100?nav=SELLING_ACTIVE

There are other shapes and sizes available too. You can search the enclosure threads or search electric longboard on eBay and you'll find them there. Another option would be to make your own vac forming set up. Takes a little practice, time and small investment, but I've found it enjoyable!
```

---
## \#29 Posted by: disastorm Posted at: 2015-10-11T11:01:25.615Z Reads: 186

```
Nice thanks. I'll try to use search more in the future.
Also thanks for the link psychotiller.
```

---
## \#30 Posted by: disastorm Posted at: 2015-10-11T22:56:49.175Z Reads: 185

```
@onloop just ordered everything from your site.
```

---
## \#31 Posted by: sgaana Posted at: 2015-10-12T05:04:37.685Z Reads: 175

```
@disastorm Have you decided which deck to use? How about remote controller?  wireless nyko kama ?
```

---
## \#32 Posted by: disastorm Posted at: 2015-10-12T05:22:09.422Z Reads: 173

```
@sgaana
 
I ordered this deck https://www.muirskate.com/longboard/decks/70202/never-summer-2015-commander-longboard-skateboard-deck-w-grip

Since its  a W Concave, the only issue I might have is I'd have to bolt the enclosure to the bottom instead of using something like tape.

I'm going to go with the Nyko Kama since I like the way it looks and it doesn't really seem to difficult to connect, I just need to solder the receiver wires to the VESC directly.
```

---
## \#33 Posted by: lowGuido Posted at: 2015-10-12T06:11:59.271Z Reads: 162

```
I think that is a good choice. I also think screws are a better choice over tape, as I have seen many e board component failures from not being properly connected to the board.
people underestimate the amount of vibration that a board goes through.
```

---
## \#34 Posted by: ishii106 Posted at: 2015-11-28T00:50:56.428Z Reads: 155

```
So, what happened to the build? 
I'm making my shopping list and this thread was great read ^_^
```

---
## \#35 Posted by: disastorm Posted at: 2015-11-28T11:02:02.664Z Reads: 157

```
I'm still waiting on the November batch of Vesc. I didn't make it for the October one in time.
I have everything else though. I got an enclosure from psychotiller and attached it to the bottom of my board with screws. Since my board has a W shape, there are some gaps, but I don't think its an issue, but if you want to be safe, I'd recommend a flat bottom. I also plan on enclosing the VESCs in heat shrink tubing. I also got a nyko kama and soldered it to one of the JST connectors. I still havn't gotten around to assembling the motors yet, so the final steps are for me to assemble the motors and attach them to the trucks, and then when the VESCs come I should be able to just plug them in ( since I think they come preconfigured with the enertionboards motor settings ) and connect everything together.
```

---
## \#36 Posted by: kai Posted at: 2015-11-28T13:40:39.364Z Reads: 152

```
Lets see some pics bro. Did you screw directly onto the board? Or did you use t-nuts?
```

---
## \#37 Posted by: disastorm Posted at: 2015-12-03T08:08:19.435Z Reads: 181

```
I used nuts without the prongs and instead epoxied them to the board. This was because I was originally worried about the fiberglass, but my friend later told me it looked like the fiberglass may have been only on the bottom and it was thin anyway so I probably could have used t-nuts. 
The griptape came on the deck already so I didn't bother removing it and re-applying on top of the nuts, so the nuts are on top of the grip tape.

Here are some photos ( in the second photo i didn't screw it in, just laid it on top so you can see how it looks, also note I'll need to cut some holes in the enclosure to provide easy access to the power button ) :


 <img src="/uploads/db1493/original/2X/3/3711d6bd667788383e924b47193f0d9d9ad929db.jpg" width="668" height="500"><img src="/uploads/db1493/original/2X/c/c78b9d30f418089236c7ed9d3e1e670801f6fba7.jpg" width="668" height="500"><img src="/uploads/db1493/original/2X/2/2fe97d7b3c4dfae2a0951fe0a902fe301154baf9.jpg" width="668" height="500">
```

---
## \#38 Posted by: kai Posted at: 2015-12-03T12:47:20.085Z Reads: 175

```
Cool man. Looks good. I got the same enclosure too. I was planning on doing the exact same thing(drilling a hole for power button and charge port) and cutting a spot out for the lcd display and glueing a piece of clear plastic so i could see it without removing the enclosure. I got some rubber firewall grommets i was going to put over the power button and charge port but i thought it would still be a pain to access. I ended up gutting my spacecell and extending the wires so i could mount my lcd display,charge port and power switch on the front sides of my enclosure. I think i will just drill a hole for the usb on the vesc and seal that with a grommet since i won't have to access that as much. Looking forward to more updates from your build.
```

---
## \#39 Posted by: ishii106 Posted at: 2015-12-04T22:26:19.846Z Reads: 168

```
Awesome! I need to get my shopping list ready this weekend. This thread helped me a lot  :smile:
```

---
## \#40 Posted by: disastorm Posted at: 2015-12-31T22:01:35.395Z Reads: 174

```
I was just assembling the motor and it looks like the circlip thing is already on the motor ? So does this mean I don't need to put one there? I just need to put one at the end of the shaft after everything is assembled right?

<img src="/uploads/db1493/original/2X/4/4ec7c76ecac76a41c65ff975ee96b58e3eac3bf1.jpg" width="666" height="499">
```

---
## \#41 Posted by: EnertionSupport Posted at: 2015-12-31T22:13:33.916Z Reads: 171

```
By adding another circlip, you prevent the pulley form hitting the CF motor mount. The one at the end of the motor shaft will then prevent the pulley from falling off. 

With both circlips, the pulley will effectively be held in place without the set screw doing all the work.

Check out this video here (circle installation around the 5min point): 
https://www.youtube.com/watch?v=J40FfVTBxVc
```

---
## \#42 Posted by: disastorm Posted at: 2015-12-31T22:18:20.814Z Reads: 162

```
ok thanks that makes sense
```

---
## \#43 Posted by: disastorm Posted at: 2016-01-04T20:08:39.213Z Reads: 173

```
I think I heard somewhere that the recent VESCs came preset with the enertion motor configurations? Is this correct? I just picked up my VESCs today ( was away for the holidays ) and was wondering if I still need to connect them to the PC to configure the Nyko Kama and CANBUS ?

Also noticed that the new VESCs don't have the sockets for the motor to plug directly into, they instead need to be soldered to the wire now ( or maybe they were always like that and the pics I saw were just of ppl that soldered a connector to it )?
```

---
## \#44 Posted by: EnertionSupport Posted at: 2016-01-04T21:04:16.643Z Reads: 174

```
Yes you will still need to use your pc to configure the nunchuk and canbus.

Running a motor detection will give you the same results as the xml file for the R-SPEC motors. That file has since been deleted though because it was for an older version of the BLDC tool. 

Read this thread here about how to properly complete the motor detection. It is very straight forward, and not difficult by any means:
http://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500

Also check out the VESC faq section for threads about the nunchuk and canbus setup: http://www.electric-skateboard.builders/search?context=topic&context_id=298&q=vesc%20faq&skip_context=true
```

---
## \#45 Posted by: lox897 Posted at: 2016-01-05T06:45:13.894Z Reads: 155

```
Seeing as @onloop is busy I'll repost this in all the threads that don't follow the guidelines quoted by onloop here:

In order to make the "E-board Builds" category really easy to search & locate specific builds i am asking that you change your title to something descriptive that better expresses the makeup of your build.
Most of the new build threads tend to end up with a name such as 
"new- noob - noobie - beginner - first - build - help - newb" this becomes hard to keep track of.
I would like to see each build thread with a descriptive title, such as;
Project Name | Deck Name | Trucks | Motor type | Mounting method | Voltage/Battery | ESC
Example
The Samurai | Custom Deck | Paris Trucks | R-SPEC | Custom Mount | 10S | VESC
```

---
## \#46 Posted by: disastorm Posted at: 2016-01-05T07:31:53.414Z Reads: 148

```
Thanks for the info guys. How can I change my topic name though?
```

---
## \#47 Posted by: lox897 Posted at: 2016-01-05T07:41:47.393Z Reads: 147

```
There should be a pencil icon near the title.
```

---
## \#48 Posted by: disastorm Posted at: 2016-01-09T20:59:33.495Z Reads: 152

```
Theres not. I can't edit my first few posts either, perhaps the post/topic is too old. Should I make a new one?

Also sorry 3 more questions. 

1. On the VESC, it comes with some kind of plastic wrap. Is this good for insulation ( like heatshrink? ), or is it just packaging and should be removed ? 
2. When soldering the VESC wires to the female motor connector cups, should I strip the wires first, or is the surface area of the wires already good enough? 
3. I remember seeing a thread before where people were talking about powering the vesc during detection, but I don't remember where the thread is. However, it sounded like onloop thought it should be safe to use the Enertion Battery, but that it might be better to use a configurable power supply. I just wanted to confirm that it is safe to use the battery, or is there a small chance of something bad happening?

Thanks.
```

---
## \#49 Posted by: lox897 Posted at: 2016-01-09T21:27:27.841Z Reads: 146

```
I think we had that problem a while back. @cmatson Do you remember that problem?

Pretty sure you're supposed to keep the plastic on unless you have to solder/fix something on the board that you can't access.

Question 2: Could you take a pic? Might help a bit.

I don't think you're supposed to power the vesc with your batteries while you program it. I haven't got a VESC yet but don't try until you have someone elses advice. If you look at vedders video or search "FAQ" there may be something you can reference to.
```

---
## \#51 Posted by: lox897 Posted at: 2016-01-09T21:44:30.086Z Reads: 139

```
@EnertionSupport How did the tshirt design competition go? I don't think we ever got the results?
```

---
## \#54 Posted by: disastorm Posted at: 2016-01-09T23:40:39.684Z Reads: 146

```
Thanks for the responses guys, that answers all my questions.

You can make this the new title:
Disastorm | Never Summer Commander Deck | Enertion Trucks | Dual Enertion R-Spec | Enertion Mount| Space Cell | Dual VESC
```

---
## \#50 Posted by: cmatson Posted at: 2016-01-11T17:47:51.521Z Reads: 106

```
9 posts were split to a new topic: [Eboard wire type- how much does it matter?](/t/eboard-wire-type-how-much-does-it-matter/970)
```

---
## \#55 Posted by: disastorm Posted at: 2016-04-22T03:58:26.352Z Reads: 112

```
I've been a little lazy, still havn't actually finished this lol.

## I noticed there are 2 of these.

<img src="/uploads/db1493/original/2X/5/5dc06ed6f65fd648a1d779c06901f8e87c7054a4.jpg" width="666" height="500">

## I know one goes here.

<img src="/uploads/db1493/original/2X/a/a6e3f82d04a8aa45f17489005385957d9bf674b2.jpg" width="666" height="500">

## Does the other one go here?

<img src="/uploads/db1493/original/2X/6/67f8f6da862c80999110537b98af0adb9452d68d.jpg" width="666" height="500">
```

---
## \#56 Posted by: treeme Posted at: 2016-04-22T05:10:26.772Z Reads: 102

```
*Note that I have not put a motor set together, but I have watched the enertion motor mount, belt, & pulley instructional guide.

You're correct that one of them goes in the wheel pulley part. My assumption would be that the second bolt is a spare part. Even functionally, I'm not sure what you'd get out of putting a bolt in there.
```

---
## \#57 Posted by: disastorm Posted at: 2016-04-22T07:18:13.527Z Reads: 100

```
yea maybe a coincidence but it does actually fit perfectly in the second spot also, thats why i wasn't sure about it.
```

---
## \#58 Posted by: treeme Posted at: 2016-04-22T13:03:48.782Z Reads: 109

```
Just a thought, but if you check the threading, it might be the same thickness as a camera mount for gopro footage.
```

---
## \#59 Posted by: disastorm Posted at: 2016-04-22T17:53:00.664Z Reads: 112

```
can anyone confirm that the second one is indeed a spare? @EnertionSupport ( please see my question in my previous posts with the images )
```

---
## \#60 Posted by: EnertionSupport Posted at: 2016-04-22T21:11:03.018Z Reads: 119

```
yes, the second one is for the set screw hole on the end of the aluminum mount. 

You can use, or not use it- totally up to you. But if you use it with thread lock, there is a greater chance of your motor mount staying in place over a long amount of time. The only reason not to use it would be if you don't want to damage the paint on the trucks.
```

---
## \#61 Posted by: disastorm Posted at: 2016-04-23T22:35:18.353Z Reads: 117

```
@EnertionSupport Thanks, it fit fine in the second place, but for the intiial place is it supposed to stick out like this?

<img src="/uploads/db1493/original/2X/c/c482c5a40c1fc044a40a3b0287e1987037374fa6.jpg" width="375" height="500">
```

---
## \#62 Posted by: lox897 Posted at: 2016-04-23T22:36:42.943Z Reads: 114

```
Have you tried the black set screw? The black one is smaller and is for the motor pulley.
```

---
## \#63 Posted by: disastorm Posted at: 2016-04-23T22:55:16.508Z Reads: 113

```
@lox897 I found a black screw with some of my other stuff so not sure if its the correct one. I don't see any other black screws though, is this the one?

<img src="/uploads/db1493/original/2X/b/bd407aac10b292f37b58ac108596f63153eb01dd.jpg" width="375" height="500">

Does this also mean that there is just a spare silver screw?
```

---
## \#64 Posted by: lox897 Posted at: 2016-04-23T22:59:18.696Z Reads: 107

```
There are 2 silver screws for the motor mount and 1 screw for the motor pulley. Can you put that next to a ruler so I can see the size?
```

---
## \#65 Posted by: disastorm Posted at: 2016-04-23T23:20:44.397Z Reads: 107

```
@lox897  ah i see, didn't realize there were 2 slots in the trucks mount.

the black one looks around 3mm or so, is that the right one?
```

---
## \#66 Posted by: lox897 Posted at: 2016-04-24T00:25:44.462Z Reads: 105

```
No. My one is about 8mm.
```

---
## \#67 Posted by: disastorm Posted at: 2016-04-24T00:51:54.632Z Reads: 108

```
@lox897 Thanks for the help, it turns out I'm an idiot, I actually assembled that thing awhile ago, it turns out I already put the set screw in there lol.
```

---
## \#68 Posted by: Kaly Posted at: 2016-04-24T14:15:41.698Z Reads: 105

```
LOL , It happens to the best of us ;-)
```

---
## \#69 Posted by: andcar2o9 Posted at: 2016-07-20T23:33:23.950Z Reads: 70

```
What size are they . M4x8mm?
```

---
