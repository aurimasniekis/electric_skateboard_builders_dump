# US - Bestech CHARGE ONLY BMS modules

### Replies: 358 Views: 10862

## \#1 Posted by: thisguyhere Posted at: 2017-11-09T03:59:18.111Z Reads: 593

```
Blowing away original post and restarting.

Not mentioning names, but some people (scepterr, b264) were angry about the original module choice so I asked bestech for additional quotes for various modules:

[<img src="/uploads/db1493/original/3X/0/8/08c493f6881c09e9e1d63eb1778a6ccb9b5ccf6f.png" width="406" height="161">](https://docs.google.com/spreadsheets/d/1fy1qrXsWBjezUsNjHDqh9TCwYJUH0eAjia_phJU15r4/edit?usp=sharing)

Price indicated above is raw price, it will be a little more once shipping + fees are added in.

Please cross reference the above with detailed specsheets here: 
https://drive.google.com/drive/folders/1f1BTzym0hYBpPfozk-HwCv91F3VqeOFA?usp=sharing

Once you've decided, please fill out this form.

If ordering more than one model, just submit it again for the other modules.

https://goo.gl/forms/inoDRKYJXR9npjEI2

@gravitycarve
@702vegas
@deucesdown
@Mobutusan
@Jreamer

everyone listed here, sorry but can you please resubmit?

--------------

**Order is paid for, see here for finishing details**:

https://www.electric-skateboard.builders/t/us-bestech-charge-only-bms-modules-25-or-so-shipped/37797/115

--------------

Dec 11 edit:

Ordered some more, please see here to order:

http://esk8life.com/
```

---
## \#2 Posted by: gravitycarve Posted at: 2017-11-09T04:02:30.316Z Reads: 436

```
I'll take 2. Not sure what I'll do with 2 but you know.
```

---
## \#3 Posted by: scepterr Posted at: 2017-11-09T04:06:01.076Z Reads: 426

```
@briman05 @Space_Cowboy
You guys want me to get one for you?
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-11-09T04:06:12.142Z Reads: 420

```
just edited post, please record yours in the form, thanks
```

---
## \#5 Posted by: Space_Cowboy Posted at: 2017-11-09T04:10:22.331Z Reads: 400

```
hey literally just sent you a PM.  Yes I'll take one thanks
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-11-09T04:13:14.777Z Reads: 370

```
on my first attempt i burnt it out, so it's good to have a backup.
```

---
## \#8 Posted by: scepterr Posted at: 2017-11-09T04:19:18.159Z Reads: 349

```
@thisguyhere did you see the size on that one?
I think this would be a better option and higher charge current in smaller package
 http://batterybms.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D190.html
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-11-09T04:20:30.740Z Reads: 319

```
i basically asked them for the least expensive charge-only module, but let me ask about this one.
```

---
## \#10 Posted by: b264 Posted at: 2017-11-09T04:24:19.404Z Reads: 317

```
[quote="scepterr, post:8, topic:37797"]
I think this would be a better option and higher charge current in smaller package
[/quote]

Yeah, the only reason I didn't pull the trigger on this is because it's not a rectangle and I'd prefer it to be the size of either 1, 2, 3, or 4 18650 cells for ease of packing an enclosure
```

---
## \#11 Posted by: scepterr Posted at: 2017-11-09T04:24:47.822Z Reads: 286

```
I'm pretty sure that'll be rectified shortly 😉
```

---
## \#12 Posted by: b264 Posted at: 2017-11-09T04:26:20.696Z Reads: 282

```
[quote="scepterr, post:11, topic:37797, full:true"]
I'm pretty sure that'll be rectified shortly
[/quote]

Right on, when I get back from my skate I might have to join in then ;-P
```

---
## \#13 Posted by: koralle Posted at: 2017-11-09T04:38:35.060Z Reads: 269

```
Guys, can someone give me (noob :) a quick rundown, why it is okay for my battery to have a charge only bms? Is discharging monitored by Focbox? I am guessing the advantage is the smaller size of the bms?
```

---
## \#14 Posted by: scepterr Posted at: 2017-11-09T04:42:30.971Z Reads: 269

```
You set battery limits in the software so you limit how much current it can possibly draw and you can install a fuse incase of some catastrophic failure.  
Using discharge through BMS can cause a myriad of issues and just one more thing to fail, for our purposes the discharge on BMS acts basically as a fuse, since we already set battery limits in software, you just can't be careless and enter ridiculous numbers
```

---
## \#15 Posted by: ShutterShock Posted at: 2017-11-09T04:43:30.304Z Reads: 273

```
Aw man I'm trying to get one that has discharge too cuz I want that protection.  That's too bad
```

---
## \#16 Posted by: scepterr Posted at: 2017-11-09T04:44:55.768Z Reads: 280

```
Protection
<img src="/uploads/db1493/original/3X/c/6/c6091bf922b3182f4b6beb96008a5ff7ac6311da.jpg" width="483" height="500">
```

---
## \#17 Posted by: ShutterShock Posted at: 2017-11-09T04:45:51.777Z Reads: 276

```
hahahah I meant over-discharge protection but that is quite the loop key
```

---
## \#18 Posted by: scepterr Posted at: 2017-11-09T04:46:37.290Z Reads: 269

```
You set voltage cutoff's in software too..
And you would typically always set them higher than the BMS so the BMS wouldnt shutoff your board...so not using the BMS over discharge protection
```

---
## \#19 Posted by: deucesdown Posted at: 2017-11-09T04:47:01.957Z Reads: 281

```
[quote="thisguyhere, post:1, topic:37797"]
over charge to be set at 4.1v
[/quote]

How does this work exactly? I'm thinking a bulk charger (not psu), if set to 4.2v/cell, will maintain constant current until 4.2v/cell, then switch to constant voltage. If bms kicks in overcharge at 4.1v, we never get to the CV part of the charge?

When does balancing kick in?

So then, if using a 4.2v/cell bulk charger with the bms set to 4.1v cutoff, assuming the balancer kicks in, it'll have to deal with the full current of the bulk charger as it's always in constant current phase, and the 84ma/cell balancer probably won't get a chance to completely balance before overcharge protection kicks in. Am I crazy?

So then the charger _needs_ to be adjusted to slightly below the overcharge cutoff of the BMS. And it can't be an adjustable PSU like meanwell, because adjusting the PSU voltage to perfectly match the BMS overcharge cutoff sounds difficult at best.

Am I overthinking this?

Anyway, I'm in, thanks.

Can you dig up some adjustable bulk chargers to match? ;)

Oh can these BMS's parameters be adjusted by user?
```

---
## \#20 Posted by: scepterr Posted at: 2017-11-09T04:48:55.020Z Reads: 252

```
90% of the laptop style 42V2A I've seen have a pot inside that'll let you tune the voltage

BMS config is set at the factory,can't tweak anything afterwards
```

---
## \#21 Posted by: deucesdown Posted at: 2017-11-09T04:53:33.642Z Reads: 261

```
@scepterr do you think I'm crazy on the rest of that post, or fairly accurate?

Lol my 2A and 4A charger has 3 pots, the 3rd one I tried adjusted the voltage, don't know what the other 2 do but for sure I didn't put them back where they started. I've found the voltage quite a pain to adjust precisely, especially on the 4A chargers... Maybe because I messed with the mystery pots lol.

I guess I need an adjustable DC load sigh.
```

---
## \#22 Posted by: scepterr Posted at: 2017-11-09T04:56:18.911Z Reads: 254

```
They need to be adjusted at load, if idle it'll be all wonky 
Just get one of those drok dc-dc cccv regulators, it's the only thing I use to charge everything, got 7 built and in use by people :wink:
https://www.electric-skateboard.builders/t/programmable-supply-power-60v-15a-35/36797/6?u=scepterr
Perfect for 12S at 4.1V per cell ^^
The 5A version is about $30
```

---
## \#23 Posted by: ShutterShock Posted at: 2017-11-09T05:04:16.484Z Reads: 246

```
Well yeah, that is true but in my experience the cell balance is bad when only using the VESC, with the BMS it seems to keep them at exactly the same voltage through the discharge.  Also, I do have them set higher, the BMS cutoff is like 3.3 or 3.4 so it wouldn't be great if the VESC didn't work anyway
```

---
## \#24 Posted by: scepterr Posted at: 2017-11-09T05:06:44.570Z Reads: 236

```
The BMS doesn't do anything on the discharge other than limit total current, I don't know why that would have an affect on cells, I haven't personally experienced that
```

---
## \#25 Posted by: ShutterShock Posted at: 2017-11-09T05:07:57.351Z Reads: 221

```
Huh weird. I thought it did.  Maybe not, but when I have checked after riding, they were all at the same voltage
```

---
## \#26 Posted by: scepterr Posted at: 2017-11-09T05:09:26.429Z Reads: 217

```
All of mine always are balanced without BMS on discharge, like I gotta use the multimeter that goes to .000 to see a difference lol
```

---
## \#27 Posted by: ShutterShock Posted at: 2017-11-09T05:10:52.048Z Reads: 219

```
Oh huh well then maybe I would be fine with just charge configuration.  Have you ever had any issues?  I am gonna be using it with lipos from hk
```

---
## \#28 Posted by: scepterr Posted at: 2017-11-09T05:13:23.213Z Reads: 223

```
Well I've never had an issue with charge only, but numerous with discharge through BMS. 95% of my battery experience is with cylindrical cells but I don't see any reason why lipo would be any diff
My experience with lipos is replacing them for cylindrical cells 🤣
```

---
## \#29 Posted by: ShutterShock Posted at: 2017-11-09T05:14:17.360Z Reads: 212

```
Well that is good to hear.  Maybe I will jump on this then.  The 60A discharge one I was gonna get from SuPower was gonna be like $47
```

---
## \#30 Posted by: deucesdown Posted at: 2017-11-09T05:14:18.991Z Reads: 219

```
This type of stuff is cool, but no termination, so gotta time it?
```

---
## \#31 Posted by: scepterr Posted at: 2017-11-09T05:17:25.959Z Reads: 226

```
Yeah it sits at like 50ma, maybe lower dont remember, I actually got the Bluetooth/USB one recently but haven't had a chance to play with it, maybe some more options there
Ive always charged below 4.2(4.1-4.15) per cell so I've never seen it as an issue

Ok just peaked at the manual and it looks pretty sweet, you can remotely turn it off, a simple Android app for remote control shouldn't be an issue..
Manual for drok Dctodc with bt/usb
https://drive.google.com/file/d/1UtPSRGAUvnJDpIltCEDwrTPdMZd3vQ51/view?usp=drivesdk
```

---
## \#32 Posted by: koralle Posted at: 2017-11-09T05:22:41.791Z Reads: 221

```
okay thanks for the explanation! this forum is fkin blazing. I am building a 10s4p 30q battery so I guess I'm participating in the gb.
So is this a solid recommended charger?
https://www.amazon.com/dp/B01HEU0GX4/
```

---
## \#33 Posted by: scepterr Posted at: 2017-11-09T05:27:26.163Z Reads: 207

```
Only if used with the drok Dctodc regulator, that's a power supply for it not a battery charger itself
```

---
## \#34 Posted by: adamm Posted at: 2017-11-09T05:29:52.241Z Reads: 202

```
Im interested in a BMS but I live in Canada is there any way you could ship to Canada as well?
```

---
## \#35 Posted by: ShutterShock Posted at: 2017-11-09T05:42:37.332Z Reads: 201

```
Wouldn't it just stop charging once the battery reached the voltage of the charger?
```

---
## \#36 Posted by: scepterr Posted at: 2017-11-09T05:43:46.876Z Reads: 196

```
What are you referring to?
```

---
## \#37 Posted by: ShutterShock Posted at: 2017-11-09T05:45:35.791Z Reads: 199

```
Sorry I meant that when you connect the power supply to the bms input, will the BMS not just stop charging the battery once it reaches the power supply voltage or are you saying you have to time it and wait?
```

---
## \#38 Posted by: scepterr Posted at: 2017-11-09T05:50:14.109Z Reads: 204

```
For Lithium charging it's a 2 step process, first constant current(cc) stage, the charger sends max current with voltage matching battery voltage till "full" voltage, second step, constant voltage(CV) stage, with fixed "full" voltage the current is gradually decreased till 10% of the max charge current
A power supply does none of this, you could technically charge a Lithium battery with a power supply but not for long...and a 48V power supply will charge to 48V...kaboom
```

---
## \#39 Posted by: ShutterShock Posted at: 2017-11-09T05:52:27.635Z Reads: 199

```
Oh crap I didn't know that.  So then how is everyone doing it with the laptop power supplies?  I have never seen anything about having to regulate it
```

---
## \#40 Posted by: scepterr Posted at: 2017-11-09T05:52:56.369Z Reads: 198

```
Lmao, they look like laptop power supplies....they are NOT laptop power supplies

FYI, almost all laptop power supplies are 19.4V
```

---
## \#41 Posted by: ShutterShock Posted at: 2017-11-09T05:54:44.955Z Reads: 209

```
Sorry for all the questions, but this is new stuff to me.  No one else has seemed to bring this up haha

Makes sense, I always figured there was a difference between a laptop power supply and a charging brick.

I have one that says lithium ion charger on it, and is labeled at 42V and 2A, will that just work by itself?
```

---
## \#42 Posted by: scepterr Posted at: 2017-11-09T05:57:18.898Z Reads: 192

```
Yep just plug into bms, you might need to lower max voltage using the pot(assuming it has one) on the PCB in the charger, if the BMS will have lower cutoff voltage
```

---
## \#43 Posted by: ShutterShock Posted at: 2017-11-09T05:59:26.874Z Reads: 194

```
Ah okay gotcha.  Makes sense!  Thank you for the useful information.  I'm guessing I would want to set it to the max charge of my lipos, so either 4.2*10 or 4.1*10 - 42V exactly or 41V?
```

---
## \#44 Posted by: Wilsonliang777 Posted at: 2017-11-09T06:03:46.220Z Reads: 197

```
I am interested in buying 2.   Pls let me know when it's time to pay.  I am in the US. Ca
```

---
## \#45 Posted by: scepterr Posted at: 2017-11-09T06:05:21.553Z Reads: 203

```
Yeah that's it. 
I think charging any lithium to 4.2 is harmful and a bit silly, I've never encountered a mass production device, like every laptop on the planet, charge above 4.15 per cell. There is simply no benefit at 4.1-4.2, you only lose cycles and with lipos early puffing.
```

---
## \#46 Posted by: thisguyhere Posted at: 2017-11-09T06:52:51.537Z Reads: 207

```
[quote="scepterr, post:8, topic:37797"]
I think this would be a better option and higher charge current in smaller package
 http://batterybms.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D190.html
[/quote]

this module doesn't go up to 12s

[quote="b264, post:10, topic:37797"]
I'd prefer it to be the size of either 1, 2, 3, or 4 18650 cells for ease of packing an enclosure
[/quote]

i think these may fit the bill:

http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D122.html
http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCB-D205V1.html
<s>http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D108.html</s>
<s>http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D284V1.html</s>

<img src="/uploads/db1493/original/3X/0/a/0a4bcf306ca5692967de769ad8a7d54a4fbf04dc.png" width="230" height="61">

i've asked pricing for each, waiting on response.

[quote="Jinra, post:66, topic:37133"]
My dual stack tiny red ones are great
[/quote]

was just advised these are available only up to 10s...bull :poop:
```

---
## \#47 Posted by: scepterr Posted at: 2017-11-09T06:53:55.902Z Reads: 181

```
Well could still get those for 10S
I'll have a look at 12S options

http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D108.html

http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCB-D245.html
```

---
## \#48 Posted by: b264 Posted at: 2017-11-09T06:57:12.342Z Reads: 183

```
[quote="thisguyhere, post:46, topic:37797"]
was just advised these are available only up to 10s
[/quote]

Some of us want more range and less sag on our rocket powered murder boards  
  
I'm looking at 10S
```

---
## \#49 Posted by: thisguyhere Posted at: 2017-11-09T07:07:46.637Z Reads: 180

```
ok, for 10s then we can get PCM-D190, no problem.

PCM-D108 is discontinued:

<img src="/uploads/db1493/original/3X/0/9/094047f01efbb2f6e71c8765ab9f388e2cfd9877.png" width="690" height="155">

[quote="b264, post:48, topic:37797"]
Some of us want more range and less sag on our rocket powered murder boards
[/quote]

that's fine, i just found end of charge voltage to be lacking so stepped up to 12s.  a 12s4p is has eight more cells than 10s4p but it's just stronger all through the charge range.
```

---
## \#50 Posted by: Jinra Posted at: 2017-11-09T07:08:35.331Z Reads: 178

```
Here's my 12s order (discharge only)

<img src="/uploads/db1493/original/3X/2/5/25c2bf112232a2913da8b52f3ed80412e0ca7584.png" width="353" height="500">
```

---
## \#51 Posted by: b264 Posted at: 2017-11-09T07:10:10.394Z Reads: 170

```
[quote="thisguyhere, post:49, topic:37797"]
that's fine, i just found end of charge voltage to be lacking so stepped up to 12s.  a 12s4p is has eight more cells than 10s4p but it's just stronger all through the charge range
[/quote]

You can ride a 12S5P and I'll take a 10S6P  :stuck_out_tongue:
```

---
## \#52 Posted by: thisguyhere Posted at: 2017-11-09T07:12:38.787Z Reads: 171

```
when did you order this?
```

---
## \#53 Posted by: Jinra Posted at: 2017-11-09T07:13:00.782Z Reads: 165

```
beginning of september.
```

---
## \#54 Posted by: scepterr Posted at: 2017-11-09T07:13:18.620Z Reads: 161

```
What about this one
http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCB-D245.html
```

---
## \#55 Posted by: Jinra Posted at: 2017-11-09T07:16:11.196Z Reads: 160

```
The reason I didn't go with that one is that it's a bit high at 1.5cm and the balance leads face upward meaning you need even more headroom to have it fit.
```

---
## \#56 Posted by: thisguyhere Posted at: 2017-11-09T07:16:48.363Z Reads: 163

```
ignored anything above 15a charging, who's got a 20a charger?  the more capable the module, i'm thinking the pricier it'll be (assuming of course).

and what @Jinra said.
```

---
## \#57 Posted by: b264 Posted at: 2017-11-09T07:17:34.962Z Reads: 171

```
[quote="thisguyhere, post:49, topic:37797"]
ok, for 10s then we can get PCM-D190, no problem.
[/quote]

Huh?  You mean HCX-D190?  Or do you have a link
```

---
## \#58 Posted by: scepterr Posted at: 2017-11-09T07:19:36.820Z Reads: 170

```

http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/BMS-D140.html
L75mm*W65mm*T8mm
```

---
## \#59 Posted by: thisguyhere Posted at: 2017-11-09T07:20:47.698Z Reads: 165

```
http://batterybms.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D190.html
```

---
## \#60 Posted by: thisguyhere Posted at: 2017-11-09T07:24:28.911Z Reads: 166

```
dammit max, i already feel bad about the million questions i'm asking.

i'll sneak this one in after i get a response.
```

---
## \#61 Posted by: scepterr Posted at: 2017-11-09T07:25:01.237Z Reads: 162

```
Lol it's their job
```

---
## \#62 Posted by: b264 Posted at: 2017-11-09T07:25:51.392Z Reads: 152

```
[quote="thisguyhere, post:60, topic:37797, full:true"]
dammit max, i already feel bad about the million questions i'm asking.

i'll sneak this one in after i get a response.
[/quote]

Next time you ask a question, wait 4 hours before you press "Send" incase you need to edit it LoLzz
```

---
## \#63 Posted by: Jinra Posted at: 2017-11-09T07:26:19.424Z Reads: 150

```
why not just use mine :P mine has a nice housing too
```

---
## \#64 Posted by: b264 Posted at: 2017-11-09T07:27:11.916Z Reads: 149

```
Look at [this thing](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCB-D275.html)
```

---
## \#65 Posted by: scepterr Posted at: 2017-11-09T07:27:24.947Z Reads: 145

```
Oh it's perfectly fine, I'm just giving options to see which is gonna be cheaper...never know
```

---
## \#66 Posted by: Jinra Posted at: 2017-11-09T07:28:27.034Z Reads: 140

```
350 x 33 mm :joy:
```

---
## \#67 Posted by: thisguyhere Posted at: 2017-11-09T07:30:59.781Z Reads: 145

```
i blew a little bit of air through my nose...good one.

[quote="scepterr, post:65, topic:37797"]
I'm just giving options to see which is gonna be cheaper
[/quote]

they really need to publish their prices, a catalog of sorts, so donna doesnt kill me with her thoughts.
```

---
## \#68 Posted by: Jinra Posted at: 2017-11-09T07:32:41.366Z Reads: 152

```
I know that feel

<img src="/uploads/db1493/original/3X/d/a/da1a4e248f8c5e82ba6896e15cdeb430bbe97b2f.png" width="557" height="132">
```

---
## \#69 Posted by: scepterr Posted at: 2017-11-09T07:42:52.068Z Reads: 150

```
A catalog? Are you crazy? It's not like they're selling anything...

Not a single BMS seller lists prices...I don't get it
```

---
## \#70 Posted by: Titoxd10001 Posted at: 2017-11-09T07:45:20.137Z Reads: 142

```
Might be interested in a 12s bms
```

---
## \#71 Posted by: Tamatoa Posted at: 2017-11-09T08:34:01.208Z Reads: 142

```
Hi would you be willing to ship outside of US? 
I am not in Europe either so I did not ask in the other group buy, USA is closer and USPS can ship where I live.
```

---
## \#72 Posted by: thisguyhere Posted at: 2017-11-09T08:38:09.994Z Reads: 139

```
where are you located?

yes, i have shipped international, cost is a bit higher but possible.
```

---
## \#73 Posted by: Tamatoa Posted at: 2017-11-09T08:57:38.113Z Reads: 130

```
I live in Tahiti - French Polynesia postcode 98702.
```

---
## \#74 Posted by: thisguyhere Posted at: 2017-11-09T08:59:21.590Z Reads: 133

```
ok!  should not be problem.

please take a look at the original post to see which module you'd like.

thanks.
```

---
## \#75 Posted by: b264 Posted at: 2017-11-09T08:59:31.826Z Reads: 138

```
[quote="thisguyhere, post:1, topic:37797"]
Not mentioning names, but some people (scepterr, b264) were angry
[/quote]

LoL, I wasn't angry.  I just didn't want a round one.  No hard feelings broski.  Too hard to play tetris with a round bms
```

---
## \#76 Posted by: thisguyhere Posted at: 2017-11-09T09:00:38.831Z Reads: 140

```
yea i just kidding, if anyone's angry it's the nice lady at bestech that's taking all this abuse from us.

:thumbsup:
```

---
## \#77 Posted by: scepterr Posted at: 2017-11-09T09:11:24.644Z Reads: 143

```
My info is in, I went with 122 for 12s and 190 for 10s
And I'm very grateful you're willing to deal with China lol, I get new grey hairs everytime I do

This happened to me just last month
https://www.electric-skateboard.builders/t/us-interest-in-8s-9s-10s-bms-charger-kit/35528/17
```

---
## \#78 Posted by: Luuke Posted at: 2017-11-09T09:51:53.342Z Reads: 137

```
But 48V 2A oder 4A should be good for 12S, right?
You would charge every cell up to 4V, which is better for the cells. But you would loose slightly some usable capacity.
```

---
## \#79 Posted by: scepterr Posted at: 2017-11-09T09:54:10.340Z Reads: 140

```
No....it still doesn't do the 2 step process, nor any shut off because it's not a charger it's a power supply, it will supply current until the battery explodes or it burns up
```

---
## \#80 Posted by: koralle Posted at: 2017-11-09T11:27:27.752Z Reads: 137

```
arrrrr I don't know sh*t about bmsses. Now there is a choice :( help pls: which one is best for 10s4p 30q?
```

---
## \#81 Posted by: longhairedboy Posted at: 2017-11-09T12:13:57.345Z Reads: 137

```
get the one with the 10amp charge current but get a 4amp charger. IT will stay cooler during charge and last a little longer because of it. Then if you ever decide to increase your pack size later you can reuse the BMS with a larger charger.
```

---
## \#82 Posted by: Luuke Posted at: 2017-11-09T12:48:40.698Z Reads: 139

```
Are you serious??
That's not possible
```

---
## \#83 Posted by: stormboard1 Posted at: 2017-11-09T13:03:55.029Z Reads: 135

```
EU shiping possible?
```

---
## \#84 Posted by: koralle Posted at: 2017-11-09T13:45:26.853Z Reads: 133

```
My brother is taking my parts to Europe dec 19. If you want, he can take yours too.
```

---
## \#85 Posted by: Lionpuncher Posted at: 2017-11-09T15:43:00.198Z Reads: 148

```
I'll bite. I'm in for a D90. Added to the doc (hopefully it worked) shipping to Canada. Let me know if that's an issue. 
Thanks for doing all the front end work @thisguyhere! Let me know when you need monies.
```

---
## \#86 Posted by: deucesdown Posted at: 2017-11-09T15:49:19.459Z Reads: 148

```
@thisguyhere omg you were supposed to pick the best ones lol.

I took a quick look at the spec sheets, they all look just about identical! the D190 (10s 10a) and the D205V1 (12s 15a) _seem_ like obvious winners, smaller (though double high) and higher charge current.

If you need thin the white ones (D140) are smaller and have the sense wires coming out 1 side only. And are rated for 10a charge. Well okay the D122 is a bit smaller, 5mm, but 12s 5a.

Does this sound about right?

e-switch doesn't really matter on a charge-only bms (EDIT unless you're powering auxiliary stuff through the discharge port)

And Joe I want to order like 2 of this and 2 of that. can't do that on the new form. Do you a form submission per bms type?
```

---
## \#87 Posted by: Ronny_CTS Posted at: 2017-11-09T16:26:27.798Z Reads: 140

```
I'll in for a 12S BMS...just need to do a little reading first so see which i'll choose.
```

---
## \#88 Posted by: thisguyhere Posted at: 2017-11-09T17:04:20.040Z Reads: 149

```
[quote="deucesdown, post:86, topic:37797"]
Do you a form submission per bms type?
[/quote]

yea just submit multiple entries for each module type:

[quote="thisguyhere, post:1, topic:37797"]
If ordering more than one model, just submit it again for the other modules.
[/quote]
```

---
## \#89 Posted by: ShutterShock Posted at: 2017-11-09T18:26:25.512Z Reads: 143

```
No problemo, this is much more organized.  The D190 looks good to me, just re-submitted.
```

---
## \#90 Posted by: thisguyhere Posted at: 2017-11-09T18:32:51.175Z Reads: 144

```
sure but obviously, higher end cost
```

---
## \#91 Posted by: b264 Posted at: 2017-11-09T19:32:53.463Z Reads: 140

```
When is the cutoff for getting in?
```

---
## \#92 Posted by: briman05 Posted at: 2017-11-09T19:43:42.998Z Reads: 138

```
http://www.batteryspace.com/smart-charger-2-0a-for-37v-li-ion-polymer-rechargeable-battery-pack-worldwide---ce--.aspx

I think this is what you would want to look for.
```

---
## \#93 Posted by: ShutterShock Posted at: 2017-11-09T19:45:00.885Z Reads: 136

```
Yeah you're right, I have a very similar model
```

---
## \#94 Posted by: thisguyhere Posted at: 2017-11-09T20:06:00.998Z Reads: 135

```
great question, it'd be great we can get the quote done tonite and send pmt tomorrow

still waiting on the following to resubmit order:

@702vegas
```

---
## \#95 Posted by: deucesdown Posted at: 2017-11-09T20:08:43.535Z Reads: 131

```
Thanks for the ping, done
```

---
## \#96 Posted by: thisguyhere Posted at: 2017-11-09T20:10:04.338Z Reads: 132

```
I was watching the form responses in real time as you were adding yours in, :thumbsup:
```

---
## \#97 Posted by: deucesdown Posted at: 2017-11-09T20:10:51.693Z Reads: 134

```
Yeah I saw creepily my handle disappearing off your reminder message lol. I have to get my hands on some 30q...
```

---
## \#98 Posted by: SORRENTINO Posted at: 2017-11-09T20:25:41.126Z Reads: 133

```
So we would want to get a charger with cv set to 49.2v?
```

---
## \#99 Posted by: thisguyhere Posted at: 2017-11-09T20:38:12.917Z Reads: 133

```
or just a 12s charger, or 50.4 will work too, the bms will limit it
```

---
## \#100 Posted by: SORRENTINO Posted at: 2017-11-09T20:39:42.396Z Reads: 135

```
Ok thanks!!!
```

---
## \#101 Posted by: deucesdown Posted at: 2017-11-09T20:40:03.283Z Reads: 133

```
Will the BMS limit it, or just cut off all power ("over charge protection" implies it'll shut off charging)
```

---
## \#102 Posted by: thisguyhere Posted at: 2017-11-09T20:42:47.822Z Reads: 132

```
what do u mean cut off all power?

I have a bestech bms with overcharge release set to 4.1v per cell, or 49.2v for the pack.

I also use a 50.4v charging brick, and once charge reaches 49.2v, the bms stops charging. 

not sure if that answers your question.

edit

I think I understand the question now that its rephrased. my answer is I'm not sure, i just know the pack voltage stops increasing. someone more clever than I may be able to answer, in fact I think there was a discussion about it earlier on in this thread.

I do notice that the charging brick gets hot while charging, but once its reached max voltage it cools down and the led indicator on the brick changes from red to green
```

---
## \#103 Posted by: b264 Posted at: 2017-11-09T20:44:49.131Z Reads: 125

```
He may be asking if it will continue to draw power and burn it off as heat after charging is complete, or if it will stop drawing power
```

---
## \#104 Posted by: gravitycarve Posted at: 2017-11-09T21:14:58.609Z Reads: 129

```
@thisguyhere got it figured I should get two different models.
```

---
## \#105 Posted by: Ronny_CTS Posted at: 2017-11-09T21:44:39.712Z Reads: 123

```
Just locked myself in for 2x D205V1 12S.
```

---
## \#106 Posted by: Mobutusan Posted at: 2017-11-09T21:51:00.362Z Reads: 123

```
Ok, I'm in for a 190-12s and 140-10s unit.
```

---
## \#107 Posted by: deucesdown Posted at: 2017-11-09T22:04:01.499Z Reads: 122

```
I'm gonna STFU now, stop infecting this thread with my paranoia.
```

---
## \#108 Posted by: thisguyhere Posted at: 2017-11-09T22:07:46.882Z Reads: 122

```
i see your D122 cancel, replacing with D140, got it
```

---
## \#109 Posted by: b264 Posted at: 2017-11-09T22:57:30.769Z Reads: 125

```
How can we confirm that we are on the list
```

---
## \#110 Posted by: thisguyhere Posted at: 2017-11-09T22:58:27.512Z Reads: 135

```
https://docs.google.com/spreadsheets/d/1mI2EouPFCvXliL9fKCx2SsKmCA5FVcXDZKMV-HB4_0w/edit
```

---
## \#111 Posted by: Wilsonliang777 Posted at: 2017-11-09T23:33:26.760Z Reads: 133

```
Would need 2x 10s  bms.  Pls
```

---
## \#112 Posted by: thisguyhere Posted at: 2017-11-09T23:37:24.160Z Reads: 137

```
ok have u read the original post on this thread?
```

---
## \#113 Posted by: Wilsonliang777 Posted at: 2017-11-09T23:47:44.114Z Reads: 140

```
Got it.   Submitted my request
```

---
## \#114 Posted by: thisguyhere Posted at: 2017-11-10T00:25:26.072Z Reads: 167

```
I'm going to cut this off at 9pm pst so i can get a final invoice tonight and paid. 

thank u for participating, will follow up with final cost
```

---
## \#115 Posted by: thisguyhere Posted at: 2017-11-11T02:47:43.911Z Reads: 174

```
i was going to PM everyone but it's making me enter each person's name one at a time:

<img src="http://andrewjrivers.com/wp-content/uploads/2015/08/Notime.jpg" width="250px" />

here's the final invoice:

<img src="/uploads/db1493/original/3X/b/c/bc58c3507720ab39c305b6fd0206e7343885d9c3.png" width="500">

it's basically $3 per module fee, that includes the $1 i'm charging for my troubles.  deal with it.

<img src="/uploads/db1493/original/3X/3/a/3a1167e92308ee5ba3ca4c26b544bbf5936f5e7a.gif" width="150">

i've already paid the invoice, it'll probably be another 2-3 weeks before they get to me.

feel free to send over your payment, at your leisure:

paypal email: 
igbad@hotmail.com

venmo: 
@thisguyrighthur

btc: 
13DspXZfB6CUHCcf92oSkZnQq7sCA5uaWS

please make sure to include your handle in the payment notes, something like "thiguyhere bms."

here's everyone final cost (click on image to see breakdown), make sure to use higher amount if sending goods & services:

[<img src="/uploads/db1493/original/3X/c/c/ccdd8d0f91691699f2de8ac3d4e4957510359146.png" width="373" height="423">](https://docs.google.com/spreadsheets/d/1xycS6pENHta2bCrR8BNF3TQLa7lD2qiqOIMcD6aejCY/edit?usp=sharing)
```

---
## \#116 Posted by: ShutterShock Posted at: 2017-11-11T20:30:41.600Z Reads: 149

```
Paid, guess I will see it in a month or so?
```

---
## \#117 Posted by: scepterr Posted at: 2017-11-11T20:53:31.297Z Reads: 146

```
Gonna be sooo many carvon v4 30q beauties in a couple months......🤩
```

---
## \#118 Posted by: Hummie Posted at: 2017-11-11T21:09:25.099Z Reads: 149

```
https://m.ebay.com/itm/3S-13S-Lithium-Battery-Balanced-Function-Board-For-18650-Polymer-Battery/332160632043?rmvSB=true&ul_ref=http://rover.ebay.com/rover/1/711-53200-19255-0/1?icep_ff3=2&pub=5575011129&toolid=10001&campid=5337662261&customid=open_22625&icep_item=332160632043&ipn=psmain&icep_vectorid=229466&kwid=902099&mtid=824&kw=lg&srcrot=711-53200-19255-0&rvr_id=1361489141187&_mwBanner=1&ul_noapp=true
Cheap. Got 4. Good review.  Don’t know what you guys are getting but this is just the balance function. On constantly.
```

---
## \#119 Posted by: scepterr Posted at: 2017-11-11T21:49:30.369Z Reads: 138

```
`1.Features:4.2V balanced function`
It only balances at a full charge of 4.2V per cell
```

---
## \#120 Posted by: Hummie Posted at: 2017-11-11T21:54:06.987Z Reads: 136

```
thanks I see that now.  and it does a low current discharge so there's still a danger of overcharging a cell with the one I posted if youre charging too fast.  still pretty awesome though.
```

---
## \#121 Posted by: scepterr Posted at: 2017-11-11T21:55:48.003Z Reads: 141

```
I've used those before with the larger through hole resistors modded to ceramic resistors to top balance my PowerWall banks
```

---
## \#122 Posted by: Hummie Posted at: 2017-11-11T22:11:28.646Z Reads: 139

```
ooo awesome to hear someone who knows how to do that.  You think I could wing that?  just replace the resistor with...what you think?  I got 4 so am ok with screwing one or two to learn.
```

---
## \#123 Posted by: scepterr Posted at: 2017-11-11T22:20:45.471Z Reads: 137

```
Do you have any of the through hole ones or just the smd resistor ones? Need the through hole ones to be able to carry higher current
```

---
## \#124 Posted by: thisguyhere Posted at: 2017-11-12T00:40:04.690Z Reads: 136

```
hopefully less, but last bms order took a solid three weeks to arrive.

oh, and i got your mailing address,thanks for sending that over.
```

---
## \#125 Posted by: ShutterShock Posted at: 2017-11-12T06:37:49.815Z Reads: 125

```
Sweet.  No problem!
```

---
## \#127 Posted by: stormboard1 Posted at: 2017-11-12T21:18:19.534Z Reads: 123

```
interested in few 10s d140's or is this closed can pay instant
```

---
## \#128 Posted by: thisguyhere Posted at: 2017-11-12T22:05:31.929Z Reads: 123

```
I ordered extras anticipating just this. 

where are you located?
```

---
## \#129 Posted by: stormboard1 Posted at: 2017-11-12T22:26:50.545Z Reads: 125

```
cool I'm in Ireland but uk or Ireland which ever cheaper shipping
```

---
## \#130 Posted by: thisguyhere Posted at: 2017-11-12T22:28:34.147Z Reads: 122

```
so you need three of D140 modules, 10s?

i believe shipping will be about $15.
```

---
## \#131 Posted by: stormboard1 Posted at: 2017-11-12T22:33:22.519Z Reads: 120

```
would that shipping be within Europe or from states?
```

---
## \#132 Posted by: thisguyhere Posted at: 2017-11-12T22:40:23.668Z Reads: 129

```
[quote="stormboard1, post:131, topic:37797"]
ping be within Europe or from states?
[/quote]

from US to Ireland
```

---
## \#133 Posted by: stormboard1 Posted at: 2017-11-12T22:42:02.363Z Reads: 131

```
aw shit customs will make it not worth it..
```

---
## \#134 Posted by: louwii Posted at: 2017-11-12T22:59:20.716Z Reads: 129

```
I might take one but I still need to figure out my setup.
I'm thinking going for two 5S1P 5000mAh batteries with a 190kV motor and a VESC. A charge only BMS makes total sense but I need to get my head around the electrical wiring for that kind of setup. I found so much information that I don't know what's good and what's not.
```

---
## \#135 Posted by: koralle Posted at: 2017-11-12T23:39:55.682Z Reads: 128

```
[quote="louwii, post:134, topic:37797"]
I found so much information that I don't know what's good and what's not
[/quote]

this happens to me so often here  and it drives me insane.
```

---
## \#136 Posted by: louwii Posted at: 2017-11-12T23:42:13.573Z Reads: 121

```
Haha ! I'm glad I'm not the only one.
```

---
## \#137 Posted by: koralle Posted at: 2017-11-12T23:42:31.508Z Reads: 123

```
 having mine sent to my bro in LA and then brought to Europe 19th Dec. if you want, he can take yours aswell and send them to you from Amsterdam.
```

---
## \#138 Posted by: stormboard1 Posted at: 2017-11-13T00:14:36.736Z Reads: 120

```
sounds perfect ya
```

---
## \#139 Posted by: stormboard1 Posted at: 2017-11-13T00:15:49.663Z Reads: 123

```
I get 2 10s d140's
```

---
## \#140 Posted by: Ronny_CTS Posted at: 2017-11-13T14:47:08.638Z Reads: 125

```
Payment sent! :grin:
```

---
## \#141 Posted by: Sk8Board Posted at: 2017-11-13T15:01:10.181Z Reads: 127

```
@thisguyhere Do you have any  D140s [10s] or D190s [10s] or any other 10s ones for sale.
```

---
## \#142 Posted by: thisguyhere Posted at: 2017-11-13T17:57:11.701Z Reads: 128

```
no more 10s for me, sorry.

any extras i've got are 12s D140 units.
```

---
## \#143 Posted by: deucesdown Posted at: 2017-11-13T19:02:19.356Z Reads: 124

```
paid, thanks!
```

---
## \#144 Posted by: Lionpuncher Posted at: 2017-11-14T20:23:21.080Z Reads: 126

```
So i couldn't find anywhere if the balance wires come with these pcb's. Can anybody clarify this for me?
Also, where could i buy pins and connector heads if i wanted to make my own?
```

---
## \#145 Posted by: thisguyhere Posted at: 2017-11-14T20:31:20.240Z Reads: 127

```
hey ship with balance wires, or they did in previous orders.

let me make sure.
```

---
## \#146 Posted by: MaxAssist Posted at: 2017-11-16T08:15:35.614Z Reads: 117

```
Payment sent, thanks again dude
```

---
## \#147 Posted by: scepterr Posted at: 2017-11-16T08:34:19.819Z Reads: 122

```
If anybody got 10s and needs 12s let me know
```

---
## \#148 Posted by: thisguyhere Posted at: 2017-11-16T21:18:59.091Z Reads: 120

```
[quote="Lionpuncher, post:144, topic:37797"]
So i couldn't find anywhere if the balance wires come with these pcb's. Can anybody clarify this for me?
[/quote]

<img src="/uploads/db1493/original/3X/1/3/134846c616e21c4580ac346490f14feb4b636126.png" width="670" height="377">
```

---
## \#149 Posted by: Ronny_CTS Posted at: 2017-11-17T08:41:08.523Z Reads: 121

```
Does anybody know at what voltage do these BMS start to balance? I'm considering using a charger with a reduced end voltage to extend battery cycle life. 

For instance if i stop charging the 10S pack at 40.5V (4.05V per cell), will the BMS still do its job while charging the pack to this voltage?
```

---
## \#150 Posted by: thisguyhere Posted at: 2017-11-17T08:47:57.467Z Reads: 118

```
these bms are set for 4.1v overcharge release, so just keep it plugged in, they'll stop when each P pack reaches 4.1v
```

---
## \#151 Posted by: b264 Posted at: 2017-11-18T06:18:45.281Z Reads: 119

```
[quote="thisguyhere, post:150, topic:37797"]
they'll stop when each P pack reaches 4.1v
[/quote]

Will a regular, unmodified 42V charger turn green when it's done?  Or what do we need to do for that?
```

---
## \#152 Posted by: thisguyhere Posted at: 2017-11-18T06:54:10.749Z Reads: 119

```
yes it will.

I have a 12s bms, set to 4.1v cutoff. my 50.4v charger turns green when pack voltage reaches 49.5v (49.5/12 = 4.125v per cell).

so it appears the bms will stop drawing power once it's reached max charge.
```

---
## \#153 Posted by: b264 Posted at: 2017-11-18T07:07:15.315Z Reads: 122

```
That's great because I can't find a 42V 1.8A (2A if I have to) adjustable charger to save my life.  I'm convinced they aren't sold...
```

---
## \#154 Posted by: thisguyhere Posted at: 2017-11-18T07:35:19.479Z Reads: 117

```
yea you're good, I'm using one of these super generic, cheapo 2amp laptop brick charger looking things, not modified or anything

http://www.electric-skateboard.builders/t/12s-2amp-laptop-style-charger-30-shipped/29728
```

---
## \#155 Posted by: Ronny_CTS Posted at: 2017-11-18T07:54:18.911Z Reads: 110

```
Thank you for your answers! You've made my day! This was exactly the solution i was searching for!
```

---
## \#156 Posted by: scepterr Posted at: 2017-11-18T08:15:28.178Z Reads: 114

```
Did the BMSs ship yet?
```

---
## \#157 Posted by: thisguyhere Posted at: 2017-11-18T09:01:38.736Z Reads: 114

```
not yet, last time it took about a week before shipping
```

---
## \#158 Posted by: thisguyhere Posted at: 2017-11-24T02:32:59.611Z Reads: 123

```
guess what's in the mail

<img src="/uploads/db1493/original/3X/8/4/84bbd4ef5390c797fd49b060a8e25ad89bc1dd94.png" width="281" height="500">
```

---
## \#159 Posted by: GrecoMan Posted at: 2017-11-24T02:37:03.060Z Reads: 110

```
gonna have to drop out, ive already got three other 10s bms’s in a drawer 😋
```

---
## \#160 Posted by: Emerson Posted at: 2017-11-24T03:27:08.009Z Reads: 109

```
Got a spare 12S inbound?
```

---
## \#161 Posted by: thisguyhere Posted at: 2017-11-24T03:35:39.131Z Reads: 107

```
yea I got extra 12s, just confirm and I'll mark you down
```

---
## \#162 Posted by: louwii Posted at: 2017-11-24T03:35:57.038Z Reads: 111

```
I'm looking for an 8S BMS if there's any available.
```

---
## \#163 Posted by: thisguyhere Posted at: 2017-11-24T03:39:05.831Z Reads: 116

```
sorry, no 8s in this order. just 10 and 12
```

---
## \#164 Posted by: Emerson Posted at: 2017-11-24T03:45:03.068Z Reads: 113

```
Confirmed, let me know the price and I'll PayPal you in the morning.
```

---
## \#165 Posted by: Wilsonliang777 Posted at: 2017-11-24T03:57:06.602Z Reads: 119

```
I ordered 2 D140 - 10S but I only need one.  If anyone needs a D140 - 10S pls let me know.  But any how.   I will still send money for  2 if no one take a my extra D140 - 10S.   

Thank you
```

---
## \#166 Posted by: scepterr Posted at: 2017-11-24T04:07:33.908Z Reads: 106

```
I'll take it..
```

---
## \#167 Posted by: Mobutusan Posted at: 2017-11-24T06:47:31.355Z Reads: 107

```
@thisguyhere Can you put me next on the list for another 10s BMS if someone drops out? Kind of realizing more that I need a second 10s instead of the 12s I'm down for.
```

---
## \#168 Posted by: thisguyhere Posted at: 2017-11-24T15:53:07.495Z Reads: 103

```
you got it, I'll make a note of it
```

---
## \#169 Posted by: wtkumar Posted at: 2017-11-24T20:10:21.526Z Reads: 101

```
Hey I'd like to get a 10s one off of you, but I have 2 (most likely really basic) questions?
Can I use a 10s bms with only 8s?
What does the Max Charge Amp change? is it just the speed it takes the batterie to charge?

EDIT: if the max charge current doesn't change too much, I'd be down to buy @Wilsonliang777 D140
```

---
## \#170 Posted by: wtkumar Posted at: 2017-11-24T20:14:07.068Z Reads: 103

```
I may be able to buy your extra D140

info in the last post to this thread
```

---
## \#171 Posted by: thisguyhere Posted at: 2017-11-25T18:05:51.941Z Reads: 114

```
[quote="Emerson, post:164, topic:37797, full:true"]
Confirmed, let me know the price and I'll PayPal you in the morning.
[/quote]

got you down, please see [tracking sheet](https://docs.google.com/spreadsheets/d/1xycS6pENHta2bCrR8BNF3TQLa7lD2qiqOIMcD6aejCY) to see you totals and pmt info.

[quote="Wilsonliang777, post:165, topic:37797"]
I ordered 2 D140 - 10S but I only need one.  If anyone needs a D140 - 10S pls let me know.  But any how.   I will still send money for  2 if no one take a my extra D140 - 10S.
[/quote]

[quote="scepterr, post:166, topic:37797, full:true"]
I'll take it..
[/quote]

@scepterr, can we give @Wilsonliang777's extra 10s bms to @Mobutusan? i know you claimed it first but you've got two 10s coming your way.  spread the love...

[quote="wtkumar, post:169, topic:37797"]
Can I use a 10s bms with only 8s?
[/quote]

you CANNOT use a 10s bms for 8s pack.  change your pack to a 10s or you will have to source a 8s bms yourself.

https://docs.google.com/spreadsheets/d/1xycS6pENHta2bCrR8BNF3TQLa7lD2qiqOIMcD6aejCY
```

---
## \#172 Posted by: scepterr Posted at: 2017-11-25T18:11:05.281Z Reads: 103

```
Yeah he can take it
```

---
## \#173 Posted by: thisguyhere Posted at: 2017-11-25T18:15:36.045Z Reads: 110

```
ok, everything's been updated:

https://docs.google.com/spreadsheets/d/1xycS6pENHta2bCrR8BNF3TQLa7lD2qiqOIMcD6aejCY
```

---
## \#175 Posted by: thisguyhere Posted at: 2017-11-25T18:18:15.013Z Reads: 103

```
yup, that's been taken care of, thx
```

---
## \#176 Posted by: psychotiller Posted at: 2017-11-25T18:24:23.758Z Reads: 103

```
I'll take 4 of the d-190's
```

---
## \#177 Posted by: thisguyhere Posted at: 2017-11-25T18:30:54.515Z Reads: 104

```
too late! they're all gonners, unless some saint wants to give up their extras.
```

---
## \#178 Posted by: psychotiller Posted at: 2017-11-25T18:32:49.446Z Reads: 106

```
Naw That's cool.

I had some ordered and they said they were going to combine my shipment with some others I had ordered..And wouldn't you know it!? -They didn't ship them.
```

---
## \#179 Posted by: thisguyhere Posted at: 2017-11-25T18:40:15.397Z Reads: 109

```
dammit donna, get your shit together.
```

---
## \#180 Posted by: Sk8Board Posted at: 2017-11-25T18:41:44.029Z Reads: 106

```
Anymore 10s ones
```

---
## \#181 Posted by: wtkumar Posted at: 2017-11-26T01:24:15.937Z Reads: 104

```
I'm new to esk8 so bear with me.

Does this mean I'm down for a 10s?

Cause I'll be needing one. (I'm changing my build from 8s to 10s)
```

---
## \#182 Posted by: Sk8Board Posted at: 2017-11-26T01:29:16.011Z Reads: 101

```
You only need a bms if you don't want to detach your batteries every time to charge. If you want to be able to plug in your board any time and let it charge then get a bms
```

---
## \#184 Posted by: thisguyhere Posted at: 2017-11-28T04:15:39.586Z Reads: 117

```
<img src="/uploads/db1493/original/3X/7/2/724dc4b0cc042053a04c4a290c97aaa4038c5b1b.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/a/8/a8a11521e78a447c0927066a981115c182750166.jpg" width="344" height="500">

sorry about the shit quality, camera phone's jacked right now.

everything arrived today and just spent some time packing everything up.

everyone mentioned here, you're good to go, it'll be in the mail tomorrow:

b264
deucesdown
Emerson
gravitycarve
koralle
MaxAssist
Ronny_CTS
scepterr
ShutterShock
SORRENTINO
Tamatoa
Wilsonliang777

haven't received payment from this group yet.  i may have missed it, please kindly send me payment details if already sent (make sure to include shipping address):

@Jreamer
@Mobutusan
@ThermalM16
```

---
## \#185 Posted by: scepterr Posted at: 2017-11-28T04:37:15.433Z Reads: 118

```
Timing couldn't be more perfect 😋
<img src="/uploads/db1493/original/3X/1/3/13e976bfc10e99976270fa86a83931736902345d.jpg" width="690" height="430">
```

---
## \#186 Posted by: Lionpuncher Posted at: 2017-11-28T04:45:09.452Z Reads: 114

```
Pm'd ya brother.
```

---
## \#187 Posted by: Wilsonliang777 Posted at: 2017-11-28T04:47:29.624Z Reads: 109

```
Payment for 1 mbs sent
```

---
## \#188 Posted by: ShutterShock Posted at: 2017-11-28T04:57:52.102Z Reads: 100

```
Woooot thanks my guy!
```

---
## \#189 Posted by: mmaner Posted at: 2017-11-28T04:58:33.061Z Reads: 103

```
If you have any extra I could use 1.
```

---
## \#190 Posted by: thisguyhere Posted at: 2017-11-28T05:23:56.460Z Reads: 105

```
let me get everything out, then do a postmortem and see what's left. 

u looking for a 10 or 12s?
```

---
## \#191 Posted by: onepunchboard Posted at: 2017-11-28T05:28:50.190Z Reads: 114

```
Srry @thisguyhere, I didn't realized the deal went on. Thought it won't make it... if you a puchsed for me that's okay, I will pay. How much do I owe you? I don't even know which I Bought lol. let me know, link me to payment.

looks like i owe 29 correct?
```

---
## \#192 Posted by: thisguyhere Posted at: 2017-11-28T05:50:17.815Z Reads: 116

```
no worries, if you don't need there are people in line.

so you decide, if you need it, it's yours.  otherwise i'll give it to someone else.
```

---
## \#193 Posted by: onepunchboard Posted at: 2017-11-28T06:04:56.129Z Reads: 117

```
okay you can give it to someone else, im not so interested. 


if nobody wants in the end tho, I will pay for that

Thanks!
```

---
## \#194 Posted by: mmaner Posted at: 2017-11-28T13:04:06.166Z Reads: 121

```
[quote="thisguyhere, post:190, topic:37797"]
10 or 12s?
[/quote]

10s, thanks for checking.
```

---
## \#195 Posted by: thisguyhere Posted at: 2017-11-29T00:37:25.370Z Reads: 114

```
had a day like this today:

https://new2.fjcdn.com/gifs/Everyday+problems_690247_4723564.gif

couldn't make it to the post office today, everyone's stuff will be put in the mail first thing tomorrow.

tracking #s to follow later tonight.
```

---
## \#196 Posted by: GhettoFab.rictation Posted at: 2017-11-29T04:59:40.641Z Reads: 108

```
Any gb still open for the d140?
```

---
## \#197 Posted by: Fabar Posted at: 2017-11-30T01:15:13.431Z Reads: 117

```
oh man!!! I'm late to this thread!!  do you have a 10S BMS ... plleeeasseee?
```

---
## \#198 Posted by: onepunchboard Posted at: 2017-11-30T01:29:47.601Z Reads: 123

```
nop dont have . @thisguyhere  has. and it is 12s bms. i
```

---
## \#199 Posted by: thisguyhere Posted at: 2017-11-30T04:42:11.301Z Reads: 132

```
@Fabar
@wtkumar
@Blacksheep
@dotruongq
@mmaner
@GhettoFab.rictation

apologies in advance if i missed someone.

the following modules are remaining:

<img src="/uploads/db1493/original/3X/7/c/7c68c6e8d248727f1f2025e1507d6938b86689f2.png" width="147" height="101">

you can find spec sheets here:

https://drive.google.com/drive/folders/1f1BTzym0hYBpPfozk-HwCv91F3VqeOFA?usp=sharing

shipping is $4 if ordering less than 4, $7 for 4 and above.

paypal igbad@hotmail.com
```

---
## \#200 Posted by: Fabar Posted at: 2017-11-30T05:19:46.110Z Reads: 124

```
thanks @thisguyhere... may I ask a stupid question?  It's my first time building... so... I read the entire thread but couldn't figure it out .. .why buy only a charge BMS... and not this HCX-D223V1 that has e-switch...
```

---
## \#201 Posted by: thisguyhere Posted at: 2017-11-30T05:25:17.406Z Reads: 127

```
great question.

the 223 module is an excellent bms.  it handles both charge and discharge, many people have used it in their builds, myself included.  it's actually smarter to use this module as it will keep your pack balanced during discharge as well.

the reason i've gone away from this module is

1. it's bulky
2. new, high quality cells tend to drift very little, or at all, so keeping them balanced at all times may not be necessary
3. voltage sag can cause the bms reset, which cuts power leading some [serious problems](https://www.electric-skateboard.builders/t/ate-shit-today-and-loop-keys/33613/30)
4. it's cheaper
```

---
## \#202 Posted by: Fabar Posted at: 2017-11-30T05:36:20.047Z Reads: 123

```
really thank you for your explanation.... so I think I'm going to get one of this for 10S ..... so... than I need to get also an e-switch right?....   I'm going to use this 5 packs of 2S lipo 60c that Namasaki posted.... so .. I'm missing something?  :S
```

---
## \#203 Posted by: thisguyhere Posted at: 2017-11-30T05:37:24.527Z Reads: 121

```
these modules have no eswitch. they power on when circuit is completed, or in other words turned on
```

---
## \#204 Posted by: Fabar Posted at: 2017-11-30T05:51:57.462Z Reads: 126

```
Sorry my lack of knowledge but ..... I couldn't understand if I need an e-switch or not....and which charger are you using......  or how did you put everything together... :S  ...  

Until now I have my motors 6374 sk3, 5 batteries 2S 60C hard pack, vescs from TB...... I was going to buy the bestech 233 and plug everything like Namasak did.... but I lost track with this option that you have......looks better... but I'm not sure how to make it...
```

---
## \#205 Posted by: GhettoFab.rictation Posted at: 2017-11-30T06:08:52.999Z Reads: 123

```
Do you know any advantages or disadvantages bewteen the d140 12s and the other crazy named 12s bms(d205v1)? I'm intimidated by the other bms afraid it might fry my electronics lol. Want to buy d140 from you so far (12s).. edit:d205v1
```

---
## \#206 Posted by: thisguyhere Posted at: 2017-11-30T07:09:01.456Z Reads: 127

```
@Fabar you have a lot more to research.  i don't think this is the appropriate place to go into pack building 101.  do some more research, please.

[quote="GhettoFab.rictation, post:205, topic:37797"]
I'm intimidated by the other bms
[/quote]

don't be, it serves the same purpose, works identical, just different form factor is all.
```

---
## \#207 Posted by: Fabar Posted at: 2017-11-30T07:20:10.120Z Reads: 124

```
hahaha... I went from  "great question"  to   "do some more research" in a blink of an eye... hehehe... 

ok ok.. I'm reading .... but didn't get it... when you said that...... one of the advantages is  "4. it's cheaper"  since the e-switch + this BMS would be higher than an 233....   ok.. I'll keep researching...
```

---
## \#208 Posted by: GhettoFab.rictation Posted at: 2017-11-30T07:33:17.079Z Reads: 117

```
If you research the switch is easily found here for cheaper I know of two sellers
```

---
## \#209 Posted by: Fabar Posted at: 2017-11-30T07:52:35.284Z Reads: 118

```
thanks!! now I got the point that you said....also intimidated.......... even checking the datasheet...not sure the difference between D190 or D140......
```

---
## \#210 Posted by: GhettoFab.rictation Posted at: 2017-11-30T07:57:08.553Z Reads: 119

```
Honestly I have 12s split into 6s each charging on the prophet sport 2 and it charges up to 6a (which I recommend 2.5 on each battery) and it's easy plug and push button then tells me each cell voltage imo I might stay where I am.
```

---
## \#211 Posted by: Sender Posted at: 2017-12-01T14:13:34.145Z Reads: 123

```
I'll take a 10s 140 and a12s 140 if still available
```

---
## \#212 Posted by: scepterr Posted at: 2017-12-01T20:52:58.042Z Reads: 132

```
Got the goodies, already in use 😋
<img src="/uploads/db1493/original/3X/d/b/db7beec3bf65ef5cbd619b921ac6f14fc50d8212.jpg" width="375" height="500">

If anybody is curious about installing the D190 it has only B1-B10 balance leads, B0/B- is the same

One other tip you can save some height by removing the screws holding the fets and solder the fets to PCB, this way the back side is actually flat
<img src="/uploads/db1493/original/3X/a/0/a0743728a0f61ab1839621225453c32f9cb77fe7.jpg" width="666" height="499">
```

---
## \#213 Posted by: thisguyhere Posted at: 2017-12-01T21:22:28.441Z Reads: 124

```
[quote="scepterr, post:212, topic:37797"]
Got the goodies
[/quote]

that got there super fast.
```

---
## \#214 Posted by: thisguyhere Posted at: 2017-12-01T21:22:49.704Z Reads: 124

```
[quote="Sender, post:211, topic:37797, full:true"]
I'll take a 10s 140 and a12s 140 if still available
[/quote]

yes they're available for you, dipping into one of my 140-12s for ya, payment details are a few posts up
```

---
## \#215 Posted by: scepterr Posted at: 2017-12-01T23:13:47.324Z Reads: 121

```
Just to clarify all the BMS were set to 4.1V end voltage correct?
```

---
## \#216 Posted by: thisguyhere Posted at: 2017-12-01T23:32:41.075Z Reads: 124

```
yep, pls check the spec sheet, says release voltage 4.125
```

---
## \#217 Posted by: scepterr Posted at: 2017-12-01T23:36:51.259Z Reads: 122

```
Charged up to 41.5 timing how long itll take to bring down to 41.25
```

---
## \#218 Posted by: thisguyhere Posted at: 2017-12-01T23:39:03.379Z Reads: 120

```
4.125 * 12 = 41.5
```

---
## \#219 Posted by: scepterr Posted at: 2017-12-01T23:39:56.791Z Reads: 121

```
Im on 10s 😉
And it's 49.5 for 12
```

---
## \#220 Posted by: thisguyhere Posted at: 2017-12-01T23:44:40.791Z Reads: 128

```
o my bad, duh its 49.5

you should see 41.25 as final pack voltage then, yea let it chill out for a bit, its should be draining now. 

my 12s shows 49.5 after an overnite charge.
```

---
## \#221 Posted by: Wilsonliang777 Posted at: 2017-12-02T10:19:18.183Z Reads: 123

```
Thank you I got bms.
```

---
## \#222 Posted by: Ronny_CTS Posted at: 2017-12-02T13:43:26.684Z Reads: 125

```
Got my BMS's as well! Thanks a lot for all your help! @thisguyhere  You da man!!!
```

---
## \#223 Posted by: b264 Posted at: 2017-12-04T19:17:21.595Z Reads: 128

```
10S is sold out
```

---
## \#224 Posted by: thisguyhere Posted at: 2017-12-04T19:35:14.693Z Reads: 134

```
i wanted to keep some to myself but you all are too much.

in the original 50 module purchase, there's a small balance remaining so i can order some more.

i'm thinking 140-10s and 140-12s modules, 10 of each.
```

---
## \#226 Posted by: SORRENTINO Posted at: 2017-12-08T15:31:07.297Z Reads: 126

```
Did you do a new order yet for 10s or have any left over?
```

---
## \#227 Posted by: thisguyhere Posted at: 2017-12-08T19:02:14.551Z Reads: 126

```
no more 10s leftover but 12 more on the way, should be here in about a week or so
```

---
## \#228 Posted by: SORRENTINO Posted at: 2017-12-08T19:04:13.255Z Reads: 129

```
Ok, Put me down for a 10s :)
```

---
## \#229 Posted by: saul Posted at: 2017-12-08T22:59:12.690Z Reads: 127

```
I want one! for 10s.
```

---
## \#230 Posted by: gogomrrobot Posted at: 2017-12-08T23:15:06.784Z Reads: 125

```
1 x 10s and 2 x 12s. Just send payment? Do you have an updated google doc for this next round
```

---
## \#231 Posted by: PredatorBoards Posted at: 2017-12-10T16:11:40.689Z Reads: 125

```
Got a spare 10S BMS?
```

---
## \#232 Posted by: dg798 Posted at: 2017-12-10T16:25:10.406Z Reads: 123

```
Anymore 12s that’s bypassed for discharge?
```

---
## \#233 Posted by: Orin635 Posted at: 2017-12-10T16:36:47.989Z Reads: 117

```
Anything for 6s?
```

---
## \#234 Posted by: thisguyhere Posted at: 2017-12-10T21:36:40.979Z Reads: 121

```
nothing for 6s

none right now but got some more d140 10 and 12 modules on the way, should be about a week now. 

setting up a shopping cart bc its a pia to do by hand.
```

---
## \#235 Posted by: gogomrrobot Posted at: 2017-12-10T22:34:08.758Z Reads: 123

```
@thisguyhere hey 👋 dude... so wait for the cart 🛒... or send you cashitos now? I need at least 1 x 12S 140
```

---
## \#236 Posted by: Blacksheep Posted at: 2017-12-10T23:09:59.284Z Reads: 130

```
Where do I put the fuse ?
```

---
## \#237 Posted by: thisguyhere Posted at: 2017-12-11T00:08:13.162Z Reads: 128

```
wait pls, I'll try to have it running tomm. and your module is secured either way, if cart doesn't come together in time you'll still get one.
```

---
## \#238 Posted by: thisguyhere Posted at: 2017-12-12T05:40:28.673Z Reads: 135

```
ok, shopping cart's up: http://esk8life.com/

please go make your purchase there, i'm done keeping track of things by hand.

@gogomrrobot
@dg798
@PredatorBoards
@saul
@SORRENTINO

if i'm delivering by hand, or if you order multiple, i'll refund you excess shipping.  i only need $3 to ship up to 4 bms.  trying to figure out shipping by weight but it's not accurate at all.
```

---
## \#239 Posted by: PredatorBoards Posted at: 2017-12-12T06:00:02.544Z Reads: 136

```
You better hold to that 1-day premium shipping XD
```

---
## \#240 Posted by: thisguyhere Posted at: 2017-12-12T06:01:01.045Z Reads: 140

```
ha, not this time. units are en route from china, probably another week or so.
```

---
## \#241 Posted by: PredatorBoards Posted at: 2017-12-12T06:03:24.651Z Reads: 141

```
alright cool. I've put in my San Diego address, however I will be flying up to the Bay Area on the 20th. Here's to hoping the BMS will arrive before I take off.
```

---
## \#242 Posted by: gogomrrobot Posted at: 2017-12-12T12:46:21.575Z Reads: 141

```
Ordered.

Question and this is my first experience with non-discharge... charge only BMS so obviously want to experiment -- this thing seems to wire identically like a discharge BMS... am I not mistaken? (but I guess when discharging it skips and BMS control)


<img src="/uploads/db1493/original/3X/2/a/2a69b08faf071946a249ddf6b079f9e1a659f525.jpg" width="491" height="499">
```

---
## \#243 Posted by: thisguyhere Posted at: 2017-12-12T18:01:49.950Z Reads: 134

```
yea just follow the diagram, just ignore the LOAD bit.
```

---
## \#244 Posted by: louwii Posted at: 2017-12-20T01:40:55.036Z Reads: 130

```
What's the shipping cost for Canada ?

EDIT: Oh wait, is this gonna work for Lipos ? Because Li-ion and Lipos have a different max-charge voltage.
```

---
## \#245 Posted by: SORRENTINO Posted at: 2017-12-20T02:02:52.687Z Reads: 152

```
Lipos and li-ion have same max charge to 4.2v per cell. The discharge voltage is different. 3.6 is average for Lipo and li-ion I think is 3.2 or lower

Edit...I misread your comment. You get the appropriate charger with max amp per your cell chemistry. If that is what you are worried about but usually most people charge 2c for li-ion or lipos to be on the safe side.
```

---
## \#246 Posted by: louwii Posted at: 2017-12-20T02:04:21.015Z Reads: 158

```
I thought the max for Li-ion was 4.1V. Not a big difference though, I agree.
Regarding discharge, I knew but it's not important as the BMS is for charge only. :slight_smile:
```

---
## \#247 Posted by: thisguyhere Posted at: 2017-12-20T02:05:07.501Z Reads: 156

```
correct, you can use these modules for lipos, just make sure you lower cutoff is set appropriately in the vesc

to answer yout question, $10 to canada
```

---
## \#248 Posted by: thisguyhere Posted at: 2017-12-20T02:06:17.234Z Reads: 153

```
[quote="louwii, post:246, topic:37797"]
max for Li-ion was 4.1V
[/quote]

they're specd for 4.2, but only charging to 4.1 increases longevity
```

---
## \#249 Posted by: louwii Posted at: 2017-12-20T02:10:11.196Z Reads: 149

```
I'm in.
I tried to add the 10S to my cart http://esk8life.com/bestech-d140-10s but it says out of stock ?
```

---
## \#250 Posted by: thisguyhere Posted at: 2017-12-20T02:25:45.456Z Reads: 142

```
Yea I disabled it for the time being, let me figure out canada shipping and add one more so you can order it. 

Please be aware though I'm still waiting on them to arrive.
```

---
## \#251 Posted by: louwii Posted at: 2017-12-20T03:11:24.004Z Reads: 140

```
No problem. I'm leaving for the holidays anyway, so it would have to be shipped in January, if you're ok with that.
```

---
## \#252 Posted by: gogomrrobot Posted at: 2017-12-21T23:17:50.979Z Reads: 142

```
[quote="thisguyhere, post:250, topic:37797, full:true"]
Yea I disabled it for the time being, let me figure out canada shipping and add one more so you can order it. 

Please be aware though I'm still waiting on them to arrive.
[/quote]

Do we have an ETA on these?  Also, I also need one more unit... but cart doesn't let you because disabled business.

Thanks!
```

---
## \#253 Posted by: thisguyhere Posted at: 2017-12-21T23:19:35.019Z Reads: 136

```
later tonight, bms arrived today, let me get a count and I'll update
```

---
## \#254 Posted by: stormboard1 Posted at: 2017-12-22T00:02:10.151Z Reads: 141

```
have the bms' arrived from my order @thisguyhere
```

---
## \#255 Posted by: thisguyhere Posted at: 2017-12-22T00:24:50.389Z Reads: 144

```
what's your zip?
```

---
## \#256 Posted by: thisguyhere Posted at: 2017-12-22T02:25:44.839Z Reads: 149

```
stock has been replenished, you should be able to put them on order now.

thanks.
```

---
## \#257 Posted by: gogomrrobot Posted at: 2017-12-22T02:44:57.044Z Reads: 160

```
Thanks! got my tracking #. Also ordered another 10S unit btw -- cart works

:)
```

---
## \#258 Posted by: TeslaAlex Posted at: 2017-12-25T20:06:03.548Z Reads: 182

```
Planning on buying one D140 12s BMS from [esk8Life.com](http://esk8life.com/bestech-d140-12s) :slight_smile:

Could you just explain a bit more precisely were the ESC positive and negative wires would go? And what sort of balance connectors should be used from the battery to the BMS?
```

---
## \#259 Posted by: thisguyhere Posted at: 2017-12-25T20:29:20.401Z Reads: 181

```
this is a pretty good diagram of bypassed bms.

also, the bms comes with balance leads.

<img src="http://www.electric-skateboard.builders/uploads/db1493/original/3X/b/9/b936f8425b380f4a00f464f5fa9e88b247e30056.png" />
```

---
## \#260 Posted by: TeslaAlex Posted at: 2017-12-25T23:03:35.412Z Reads: 179

```
I just made a schematic with my Lipos. Is the wiring correct?

<img src="/uploads/db1493/original/3X/3/f/3fca65dfa254f4ca5867151908a1f0d8751d4eb6.png" width="690" height="341">
```

---
## \#261 Posted by: thisguyhere Posted at: 2017-12-26T03:53:56.010Z Reads: 180

```
looks ok, just take your time when wiring up the balance leads.  i haven't worked with lipos before.

balance lead 1 should be pack voltage, the drop down in voltage each subsequent series.

only thing i can see, as it's diagrammed, your voltmeter will always be on.  be sure to move the voltage neg wire after the loop key.
```

---
## \#262 Posted by: TeslaAlex Posted at: 2017-12-26T10:14:16.882Z Reads: 183

```
I made a new, simpler one. In this curcuit the voltmeter will only be on when the xt90 anti-spark is plugged in. The female/male parts are 5.5mm bullets. 

<img src="/uploads/db1493/original/3X/b/7/b70cc826c455000061273e4d32e717d7ee77e9ae.png" width="690" height="464">
```

---
## \#263 Posted by: TeslaAlex Posted at: 2017-12-26T16:19:43.874Z Reads: 177

```
After some reading I understood that on some BMS´s the black balance wire from battery 4 (which is not used in the diagram above) should be connected to the B- port. Does this have to be done on the Bestech 140D 12s BMS?
```

---
## \#264 Posted by: thisguyhere Posted at: 2017-12-26T19:02:01.823Z Reads: 181

```
no, not that I'm aware of, bms diagram doesn't indicate that. 

I would just attach the charge wires directly to your main power leads, save some connectors. but wiring looks accurate.
```

---
## \#265 Posted by: ZackoryCramer Posted at: 2018-02-16T01:51:24.418Z Reads: 195

```
Do you think you’re going to host another pcm group buy soon? 🧟‍♂️
```

---
## \#266 Posted by: thisguyhere Posted at: 2018-02-16T03:42:13.252Z Reads: 192

```
as of now, no not really.
```

---
## \#267 Posted by: b264 Posted at: 2018-02-16T03:43:00.193Z Reads: 197

```
[quote="ZackoryCramer, post:265, topic:37797, full:true"]
Do you think you’re going to host another pcm group buy soon?
[/quote]

China is closed for holiday until next month
```

---
## \#268 Posted by: thisguyhere Posted at: 2018-02-22T16:52:22.600Z Reads: 196

```
I need to order some bms for some random projects so can fit in additional bms' in this order.

I'd like to limit the models to the D140, you can see the specs here:

http://esk8life.com/bestech-d140-10s
http://esk8life.com/bestech-d140-12s

if you've had a burning need for a different module, please let me know, i can ask.  but getting a spec and quote for each different module adds to lead time.

bestech is back in business on feb 25.
```

---
## \#269 Posted by: Sender Posted at: 2018-02-22T17:14:48.751Z Reads: 176

```
I definitely need at least 1 more 10s and a couple 12s's.  Maybe more if I mess up the one I already have. Lol.  BTW, did you get the nickel out? I never saw a tracking number.  Just itching to fire up my spot welder!  Thanks for helping out the community!
```

---
## \#270 Posted by: scepterr Posted at: 2018-02-22T17:18:56.702Z Reads: 170

```
I'll take 2 each
```

---
## \#271 Posted by: thisguyhere Posted at: 2018-02-22T17:31:55.871Z Reads: 167

```
this shipping service i'm using is supposed to send out tracking details as they're created but it's been spotty, not sure why.

it was dropped in the mail two days ago but it's still not showing status: 9400110298370379790337		

i'm sure you'll get it in a couple days.
```

---
## \#272 Posted by: mmaner Posted at: 2018-02-22T17:36:51.544Z Reads: 165

```
I'll take 1 of each if you still have stock.
```

---
## \#273 Posted by: GrecoMan Posted at: 2018-02-22T17:53:17.458Z Reads: 153

```
i’ll take a 10s
```

---
## \#274 Posted by: thisguyhere Posted at: 2018-02-22T17:54:22.289Z Reads: 150

```
none on hand now, can you wait a few weeks for them to arrive?
```

---
## \#275 Posted by: mmaner Posted at: 2018-02-22T18:04:09.881Z Reads: 148

```
sure, I have a 10s to do what I need to now.  Whenever you have them handy, thanks.
```

---
## \#276 Posted by: Scoo_B_SK8 Posted at: 2018-02-23T06:01:40.299Z Reads: 153

```
mark me down for a 10s please
```

---
## \#277 Posted by: Sender Posted at: 2018-02-24T03:26:08.774Z Reads: 159

```
I know this is not the place for this exactly...BUT, I know the D140 comes in 11s. Does anyone know where to get an 11s charger besides Alibaba? The places I keep finding have only 10 or 12 s chargers.  I feel like it might be nice to run 11s, as it is a little more in the safe zone with 190kv, but will have a bit more punch than 10s... suggestions?
```

---
## \#278 Posted by: scepterr Posted at: 2018-02-24T03:54:07.542Z Reads: 160

```
11S 😉
![IMG_20180223_225329|666x500](upload://ABZeAq8Fk6suvJineFzQ1sigE8.jpg)
```

---
## \#279 Posted by: Sender Posted at: 2018-02-24T03:58:07.501Z Reads: 155

```
I read through that whole thing... a little intimidating TBH.
```

---
## \#280 Posted by: thisguyhere Posted at: 2018-02-24T03:58:50.000Z Reads: 157

```
I've always wondered, is ok to use a higher voltage supply, so like a 12s brick to charge a 10s pack since the bms would limit voltage.
```

---
## \#281 Posted by: scepterr Posted at: 2018-02-24T03:59:26.498Z Reads: 153

```
You'de burn the bms it would limit till it died
```

---
## \#282 Posted by: thisguyhere Posted at: 2018-02-24T04:00:12.839Z Reads: 150

```
yup, using the exact same thing. 

@Sender it's not too bad, menu isn't very intuitive but once you play around with it for a couple hrs it'll seem obvious
```

---
## \#283 Posted by: thisguyhere Posted at: 2018-02-24T04:00:40.932Z Reads: 149

```
yea that's what I figured.
```

---
## \#284 Posted by: scepterr Posted at: 2018-02-24T04:01:38.322Z Reads: 142

```
It won't be able to limit the full current still going at 42, vs a 10s charger where current starts dropping at 42, would hit overvolt and shunt till something burned
```

---
## \#285 Posted by: scepterr Posted at: 2018-02-24T04:03:05.714Z Reads: 138

```
It's a couple of wires and you can get the Bluetooth one and control it from a computer
```

---
## \#286 Posted by: Sender Posted at: 2018-02-24T04:05:15.633Z Reads: 136

```
Ok cool, I'll revisit that thread and put together a parts list and confirm it.  The bluetooth does sound pretty sweet... thanks guys
```

---
## \#287 Posted by: ARetardedPillow Posted at: 2018-02-24T04:05:43.621Z Reads: 134

```
Mark me down for a 10s and ship it to @scepterr to save on shipping lol
```

---
## \#288 Posted by: ShutterShock Posted at: 2018-02-24T09:30:56.386Z Reads: 137

```
Sighhh I think I burned my 10s one, it won't charge anymore.  I will take a 10S
```

---
## \#289 Posted by: GrecoMan Posted at: 2018-02-25T01:53:38.436Z Reads: 139

```
i’m in the same boat ☹️
```

---
## \#290 Posted by: thisguyhere Posted at: 2018-02-25T02:10:16.280Z Reads: 136

```
put the order in last night, takes about 3 weeks to arrive. I'll update here then
```

---
## \#291 Posted by: dg798 Posted at: 2018-03-04T19:10:51.404Z Reads: 130

```
anymore 12s bms coming in??
```

---
## \#292 Posted by: stormboard1 Posted at: 2018-03-04T19:13:29.871Z Reads: 138

```
any 12s/10s going? just used one in my build and works great
```

---
## \#293 Posted by: dg798 Posted at: 2018-03-04T19:15:04.104Z Reads: 140

```
i will take a 12s bms if possible
```

---
## \#294 Posted by: thisguyhere Posted at: 2018-03-04T19:28:47.286Z Reads: 138

```
got both 10s and 12s en route, should be a couple weeks
```

---
## \#295 Posted by: dg798 Posted at: 2018-03-04T19:29:33.372Z Reads: 132

```
can i be reserved for a 12s
```

---
## \#296 Posted by: stormboard1 Posted at: 2018-03-04T19:32:45.712Z Reads: 139

```
1 x 10s and 1 x 12s please
```

---
## \#297 Posted by: dg798 Posted at: 2018-03-04T19:36:38.461Z Reads: 137

```
please put on hold for 1 12s BMS
```

---
## \#298 Posted by: GrecoMan Posted at: 2018-03-04T19:42:15.752Z Reads: 134

```
dude you’ve said it three times
```

---
## \#299 Posted by: dg798 Posted at: 2018-03-04T19:42:47.742Z Reads: 137

```
i know im a bit obsessed lol
```

---
## \#300 Posted by: ggalisky Posted at: 2018-03-06T22:37:47.982Z Reads: 127

```
Hello I would Like to buy a 10s 80amp BMS
```

---
## \#301 Posted by: thisguyhere Posted at: 2018-03-06T22:39:04.263Z Reads: 123

```
sorry, i'm not your person then, i get charge only bms.

@mmaner i think is gearing up for a charge / discharge group buy
```

---
## \#302 Posted by: mmaner Posted at: 2018-03-06T22:41:55.853Z Reads: 116

```
still waiting on BesTech to confirm.
```

---
## \#303 Posted by: GrecoMan Posted at: 2018-03-06T22:52:16.520Z Reads: 117

```
so are you just gonna put these on your site and start a brawl for who gets them? or are you keeping track of the people that said they wanted them?
```

---
## \#304 Posted by: mmaner Posted at: 2018-03-06T22:53:39.250Z Reads: 121

```
I'm just gonna post them here and it'll be 1st come 1st served.
```

---
## \#305 Posted by: GrecoMan Posted at: 2018-03-06T23:02:03.496Z Reads: 126

```
was wondering about the charge only bms’s
```

---
## \#306 Posted by: thisguyhere Posted at: 2018-03-06T23:15:31.362Z Reads: 132

```
we're going to do it lord of flies / battle royale style where the strong eat the weak.

no, jk, i took a count then ordered more on top of that so there should be plenty to go around unless some asshat orders more than what they originally requested.
```

---
## \#307 Posted by: GrecoMan Posted at: 2018-03-06T23:17:02.065Z Reads: 137

```
damn. was really lookin forward to beating someone up over a bms.
```

---
## \#308 Posted by: thisguyhere Posted at: 2018-03-07T19:45:00.426Z Reads: 137

```
looks like modules are set to arrive tomorrow:

![image|690x393](upload://bYCLrGrOHUctvufvBYm4OrG1s4k.png)

made them available in the store for purchase: http://esk8life.com

@Sender
@scepterr
@mmaner
@GrecoMan
@Scoo_B_SK8
@ShutterShock
@dg798
@stormboard1
```

---
## \#309 Posted by: GrecoMan Posted at: 2018-03-07T19:50:25.865Z Reads: 124

```
can you reserve one? don’t have money but will soon
```

---
## \#310 Posted by: thisguyhere Posted at: 2018-03-07T19:56:11.886Z Reads: 124

```
no prob ......
```

---
## \#311 Posted by: scepterr Posted at: 2018-03-07T20:08:44.378Z Reads: 122

```
$14.30 shipping on 4pcs?
```

---
## \#312 Posted by: koralle Posted at: 2018-03-07T20:23:21.908Z Reads: 127

```
@thisguyhere which cutoff voltages are you using this time?
```

---
## \#313 Posted by: thisguyhere Posted at: 2018-03-07T20:58:08.591Z Reads: 135

```
wat, no that ain't right.

messed around with the shipping so it's more accurate but it appears it's had the opposite affect.  give me a minute.

[quote="koralle, post:312, topic:37797"]
which cutoff voltages are you using this time?
[/quote]

same as before, 4.08v

![image|690x105](upload://hl6tAdJ4xzfhsdaAMuI6TCz7YN2.png)
```

---
## \#314 Posted by: scepterr Posted at: 2018-03-07T21:02:30.372Z Reads: 132

```
No worries, using first class mail?
Cheapest tracked option as far as I'm aware
```

---
## \#315 Posted by: thisguyhere Posted at: 2018-03-07T21:04:54.535Z Reads: 131

```
yep, for anything under 9oz it's first class, which is the same as priority but priced lower.

anything above 9oz is priority.

anyway, fixed.  just refresh your cart it should be reflected.
```

---
## \#316 Posted by: GhettoFab.rictation Posted at: 2018-04-08T11:02:00.394Z Reads: 122

```
Hey I bought your d140 12s bms and it only has two mosfets on it will everything be ok? And for charge only wouldn't I bypass bms? Idk if the diagram on the site is right, I am human though so try to take what I say with a grain of salt hah
```

---
## \#317 Posted by: thisguyhere Posted at: 2018-04-08T17:38:37.282Z Reads: 123

```
that's why its charge only, charge rated at 10a max.

that diagram better be right, dafuq it'd be a disaster if it isn't, I've already setup a few packs according to that diagram.
```

---
## \#318 Posted by: koralle Posted at: 2018-04-08T17:50:39.509Z Reads: 127

```
Do all your charge only bms also get crazy hot once the battery is fully charged? The mosfets are cool but this small row of of 100ohm resistors gets so hot within no time, I can't touch it.
```

---
## \#319 Posted by: koralle Posted at: 2018-04-08T17:58:33.999Z Reads: 125

```
Have checked all the cell pack voltages and they are balanced to .01V
```

---
## \#320 Posted by: ShutterShock Posted at: 2018-04-08T18:27:22.236Z Reads: 122

```
I ended up getting an ebay one, I will no longer need this one.  Thanks though!
```

---
## \#321 Posted by: thisguyhere Posted at: 2018-04-08T19:31:32.588Z Reads: 128

```
oh man, I haven't checked not sure how hot they get. 

but that's what they do, over charge then discharge via resistors to balance.
```

---
## \#322 Posted by: koralle Posted at: 2018-04-08T19:35:02.469Z Reads: 128

```
Ordered this badboy now so I can keep the bms furnace far away from my battery and also measure cell drift without removing my enclosure plus bms insulation.

![2018-04-08 21_33_40-SP2110 , waterproof connector 12 pin plug socket, high voltage current cable con|486x429](upload://lwvdOyeyJ7SuqdKLX0ztbcTxx7U.png)
```

---
## \#323 Posted by: landonkun Posted at: 2018-04-10T03:22:54.401Z Reads: 121

```
Any more of these left? Either 10S or 12S?
```

---
## \#324 Posted by: thisguyhere Posted at: 2018-04-10T03:38:29.835Z Reads: 118

```
10s still going on

http://esk8life.com/
```

---
## \#325 Posted by: Bender Posted at: 2018-04-11T12:26:47.640Z Reads: 115

```
So probably a silly question but can the e switch work on a charge only setup?
```

---
## \#326 Posted by: mmaner Posted at: 2018-04-11T12:32:59.112Z Reads: 117

```
[quote="Bender, post:325, topic:37797"]
can the e switch work on a charge only setup
[/quote]

Unfortunately, no.
```

---
## \#327 Posted by: SORRENTINO Posted at: 2018-04-11T14:20:35.998Z Reads: 114

```
Yes they get super hot. Hot enough to burn your skin :slight_smile:
```

---
## \#328 Posted by: koralle Posted at: 2018-04-11T14:22:30.710Z Reads: 118

```
makes me wonder about the bms's longevity ...
also I don't like if things inside my enclosure get hot :rage: I think from here on out I'll always use charge only BMS and keep it seperate with 12pin charging connector.

I have heard too much about heat having a negative effect on battery charge cycles.
```

---
## \#330 Posted by: thisguyhere Posted at: 2018-04-11T15:58:22.235Z Reads: 120

```
i'll test this d140 module and see how hot they get.
```

---
## \#331 Posted by: Ronny_CTS Posted at: 2018-04-11T16:39:11.687Z Reads: 121

```
I haven't tried out my D205V1 yet so i have no idea how hot they get.
```

---
## \#332 Posted by: Sender Posted at: 2018-04-11T17:38:54.447Z Reads: 120

```
You have a link for this guy?
```

---
## \#333 Posted by: koralle Posted at: 2018-04-11T17:41:24.235Z Reads: 127

```
https://www.aliexpress.com/item/SP2110-P12-12pin-waterproof-connector-plug-socket-high-voltage-current-cable-connector/32383806279.html

Haven't received it yet so I can not attest to the quality but will let you know as soon as it arrives.
```

---
## \#334 Posted by: dg798 Posted at: 2018-04-11T22:52:54.744Z Reads: 127

```
my d140 doesnt get hot at all
```

---
## \#335 Posted by: Minim Posted at: 2018-04-12T05:13:41.293Z Reads: 118

```
When are you expecting the D140-12S back in stock?
```

---
## \#336 Posted by: thisguyhere Posted at: 2018-04-12T07:00:00.087Z Reads: 126

```
sorry no plans for another order any time soon, i only get them as they're needed, not really running a business selling these.
```

---
## \#337 Posted by: E1Allen Posted at: 2018-05-26T06:07:45.700Z Reads: 113

```
So the 12s d140 BMS.  Will the boosted charger which is 54.4v work or do you need 50.4?

Edit: I believe the answer is no. I used the search thingy with different words this time.
```

---
## \#338 Posted by: thisguyhere Posted at: 2018-05-26T15:35:49.120Z Reads: 108

```
you could but shouldn't. 

BMS will cut power but power supply will keeep supplying current since it's set to 54v. bms would bleed off current in form of heat through resistors so wouldn't be safe long term.
```

---
## \#339 Posted by: dg798 Posted at: 2018-05-27T01:22:26.968Z Reads: 104

```
Is it normal for the bms to get really really hot while charging
```

---
## \#340 Posted by: b264 Posted at: 2018-05-27T01:23:26.679Z Reads: 107

```
Not really hot.  Slightly warm just before the end of charging.
```

---
## \#341 Posted by: dg798 Posted at: 2018-05-27T01:39:01.293Z Reads: 108

```
Mine gets hot to the touch
```

---
## \#342 Posted by: dg798 Posted at: 2018-05-27T02:48:47.296Z Reads: 110

```
It charges and all but it gets really hot and all voltages are right and in order
```

---
## \#343 Posted by: Eboosted Posted at: 2018-05-29T23:13:46.413Z Reads: 111

```
Is this still open?

I want 5 of them
```

---
## \#344 Posted by: Sender Posted at: 2018-05-30T00:47:09.098Z Reads: 113

```
@Eboosted I think @JLabs has an order in for some 10s and 12s bypass BMSs
```

---
## \#345 Posted by: Eboosted Posted at: 2018-05-30T01:05:15.704Z Reads: 115

```
Nice @jlabs would you send me a quote for 5 units?
```

---
## \#346 Posted by: thisguyhere Posted at: 2018-06-26T19:52:25.102Z Reads: 109

```
got some more modules in case anyone needs them:

http://esk8life.com/
```

---
## \#347 Posted by: Blix Posted at: 2018-06-26T20:18:22.277Z Reads: 105

```
I would need one in Europe, sorry.
If somebody is purchasing a 12s bms from Europe, write me a message, we can order together!
```

---
## \#348 Posted by: JonathanLau1983 Posted at: 2018-06-26T21:46:43.930Z Reads: 103

```
You going for a bypass BMS? I need a 12S bypass BMS in UK
```

---
## \#349 Posted by: Sender Posted at: 2018-06-27T06:08:36.893Z Reads: 96

```
Thanks @thisguyhere I tried to grab a 12s the other day, but you were out... perfect timing!
```

---
## \#350 Posted by: L3chef Posted at: 2018-06-27T08:07:09.047Z Reads: 94

```
10s charg only intress in eu.
```

---
## \#351 Posted by: thisguyhere Posted at: 2018-06-27T16:11:36.206Z Reads: 92

```
sent it out today!
```

---
## \#352 Posted by: Battosaii Posted at: 2018-06-27T16:44:22.000Z Reads: 87

```
I picked up a 12s charge only thank you!
```

---
## \#353 Posted by: thisguyhere Posted at: 2018-06-27T16:49:22.555Z Reads: 88

```
excellent, it'll be in the mail tomorrow.
```

---
## \#354 Posted by: Blacksheep Posted at: 2018-06-27T18:13:28.156Z Reads: 92

```
Can someone help me where do the balance wires go ![image|281x499](upload://1Hl397lPk4iHweOSauY3WlrLWAw.jpg)![image|375x500](upload://1hAucgcxI9FpDcASVowK5uLv0j4.jpeg)![image|375x500](upload://iJWEunOddNuSpNV1C2o6c9HQuEf.jpeg)
```

---
## \#355 Posted by: Sender Posted at: 2018-06-27T18:48:14.694Z Reads: 88

```
![20180627_134716|273x500](upload://A4vaCcH0F1Xi3t3JGV3v7oHhSgA.jpg)

Obviously depending on how you wire it...
```

---
## \#356 Posted by: Blacksheep Posted at: 2018-06-27T18:49:45.771Z Reads: 84

```
Thanks so much I was confused because it’s usually 13 wires thanks so much
```

---
## \#357 Posted by: b264 Posted at: 2018-06-27T18:50:48.112Z Reads: 84

```
Zero is the one he didn't mark, that's the 13th one.  But you should ALWAYS verify the voltage with a multimeter before making the balance connection.
```

---
## \#358 Posted by: Sender Posted at: 2018-06-27T18:52:01.964Z Reads: 84

```
This BMS has 12 wires for 12 cells.
```

---
## \#359 Posted by: Blacksheep Posted at: 2018-06-27T18:52:05.256Z Reads: 86

```
But there is no 13 wire
```

---
## \#360 Posted by: b264 Posted at: 2018-06-27T18:52:36.810Z Reads: 85

```
The 13th wire is probably the big "B-" wire
```

---
## \#361 Posted by: Sender Posted at: 2018-06-27T18:53:58.635Z Reads: 88

```
Yeah, exactly.  Of course it is "there" just that is how this one is labled.  Just to not confuse things.  This is where the 12 balance wires go for this BMS, B- goes to, well, B-.
```

---
## \#362 Posted by: b264 Posted at: 2018-06-27T19:16:22.529Z Reads: 90

```
Some BMS have B0 through B12 for 13 balance wires, but the bottom one is electrically the same as B-.  In fact, if you're using them for charge-only and they have 13 wires, it's likely you don't even need to hook up B- on those BMSs
```

---
## \#363 Posted by: akhlut Posted at: 2018-06-27T19:30:52.176Z Reads: 101

```
@thisguyhere

Ordered!
```

---
## \#364 Posted by: thisguyhere Posted at: 2018-09-01T03:30:26.600Z Reads: 83

```
got some more 10s and 12s modules in, in case anyone needs them.

[bkb](https://buildkitboards.com/collections/batteries/products/bestech-d140-charge-only-bms) has them too.

http://www.esk8life.com/bestech-d140-10s

http://www.esk8life.com/bestech-d140-12s
```

---
