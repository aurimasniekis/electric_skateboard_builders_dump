# Remote options seem terrible

### Replies: 52 Views: 3079

## \#1 Posted by: pshaw Posted at: 2017-07-22T13:46:22.650Z Reads: 321

```
The only remote I've used on an e-board so far has been a boosted board remote. At first I thought it seemed kind of cheap feeling. My buddy got the enertion nano remote for his DIY board and I was shocked at how cheap it felt. It made my boosted remote look like the nicest remote of all time haha. 

What is up with the garbage remote selection we have for DIY boards?!? Has anyone retrofitted the guts into a boosted board remote? There has GOT to be something better than these cheap toy feeling remotes.
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-07-22T14:10:48.038Z Reads: 311

```
[quote="pshaw, post:1, topic:28279"]
nano remote for his DIY board and I was shocked at how cheap it felt.
[/quote]

It might feel cheap for your taste, but it is still one of the most reliable remote out there.
```

---
## \#3 Posted by: pshaw Posted at: 2017-07-22T14:11:14.989Z Reads: 305

```
Is there any way to modify the wheel so that it is smoother and better to use? @JohnnyMeduse
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-07-22T14:12:10.493Z Reads: 300

```
did your friend calibrate it before using it ?
```

---
## \#5 Posted by: Alan_Smithee Posted at: 2017-07-22T14:18:06.048Z Reads: 303

```
Shameless plug for a pretty decent remote:
https://www.electric-skateboard.builders/t/new-maytech-mtskr1712-remote-receiver-42-shipping/26981/13
```

---
## \#6 Posted by: pshaw Posted at: 2017-07-22T15:33:48.713Z Reads: 305

```
I'm just talking about overall feel of the remote
```

---
## \#7 Posted by: darkkevind Posted at: 2017-07-22T15:44:52.592Z Reads: 298

```
The Benchwheel remote is what I use and it's the best I've used so far. Good weight, good strong feel and responsive potentiometer.

<img src="/uploads/db1493/original/3X/1/6/16058e294fb6347a36b9c96c3e5b49b0a8026a27.png" width="202" height="249">

For cheapness and reliability, you can't go wrong with the mini remote, except you need to remove the wheel and it's a little on the bulky side.

<img src="/uploads/db1493/original/3X/e/c/ec70ab91c40cc0258ee13a0362349009935c95be.png" width="275" height="183">
```

---
## \#8 Posted by: evoheyax Posted at: 2017-07-22T15:58:21.325Z Reads: 290

```
The mini remote has been great for me...

A bit larger than desired, but it works out of the box (no adjusting the settings to get the correct throttle range), is cheap, and I've never had a drop out from it.
```

---
## \#9 Posted by: William_Trojel Posted at: 2017-07-22T15:59:15.123Z Reads: 283

```
I have heard that it uses a lot of batteries is it true?
```

---
## \#10 Posted by: evoheyax Posted at: 2017-07-22T16:08:57.095Z Reads: 289

```
not at all. Haven't changed batteries in 3 months, lol. And I ride daily, at least a few miles.

Takes 2 double AA, runs them in series at 3v. As long as you turn it off, your fine.

Others have told me there batteries seem to last forever also.

I've used a few of them and never any issues.

I can tell you I love this remote so much that when we ship complete boards, this will likely be the remote we will use (maybe a new case, but same internals, because they are rock solid)
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-07-22T16:12:12.966Z Reads: 284

```
I have used several remotes and my opinion is as follows:

GT2B: a great remote with no signal dropouts. However, it is large and cumbersome for riding. There are several case mods but I do not personally like them.

Nano: Small and compact but signal drop outs are very frequent when around other Bluetooth signal sources. Very unreliable and quite dangerous!

Mini: Great Remote. Practically smaller version of the GT2B.

Benchwheel: A great remote with no dropouts. Small and compact, easy to ride with.

In my opinion, for thumbwheel control use the benchwheel. For trigger finger control use the mini.
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-22T17:01:42.821Z Reads: 264

```
nano v2 (nano x as well) has been super reliable for me. Only shitty thing is you have to calibrate each time you turn it on.
```

---
## \#13 Posted by: wafflejock Posted at: 2017-07-22T17:10:02.402Z Reads: 260

```
Not a realistic option unless you really want to make your own, but made my own posted code and PCB schematics (Eagle 8.1.1 files) here:

https://github.com/shusain/eskatecontroller

Runs off 1 1S LiPo the Arduino is the 3.3V 8MHz pro mini variant so it can operate on voltages as low as the discharged 1S LiPo can go.  Literally have left it on for days before by accident and still has power, I put a 800 mAh battery in there and it uses about 10-20mA of current so should last somewhere between 40 and 80 hrs before a recharge.
```

---
## \#14 Posted by: Sander Posted at: 2017-07-22T20:56:56.115Z Reads: 246

```
[quote="pshaw, post:1, topic:28279"]
There has GOT to be something better than these cheap toy feeling remotes.
[/quote]

Im working on it...
```

---
## \#15 Posted by: wafflejock Posted at: 2017-07-22T21:02:52.234Z Reads: 240

```
Speaking of that did you get your custom nrf boards in yet also what's the cost per unit on those?
```

---
## \#16 Posted by: Sander Posted at: 2017-07-22T21:10:29.744Z Reads: 239

```
Haven't ordered them yet, have no use for them in this version ;)
The cost depends on the Nrf chips, they are expensive in small quantities. They cost around 3.5 Dollars for only 1.

So for one nrf pcb with the componets is around <7$ and u usually uses two so ~15$, the cap antenna is the one doing it expensive.
```

---
## \#17 Posted by: wafflejock Posted at: 2017-07-22T21:15:00.963Z Reads: 238

```
Gotcha yeah I ask because the ones that are out there are done at such a massive scale (and probably skipping a lot of Q&A and general component quality control) but can get them between $0.50-$2 a piece if you buy 10 or more so hard to turn away from that.  I've been thinking over putting together some charge circuitry in some LED risers but the TP4056 does the job and is already dirt cheap because of the economy of scale (my guess is if you make 100,000 or more the price gets to where you can sell them for what they're sold for).

http://www.inkocean.in/nrf24l01-24l01-wireless-module-upgrade-bulk-purchase-pricing
```

---
## \#18 Posted by: Sander Posted at: 2017-07-22T21:17:10.760Z Reads: 225

```
But the problem with the nrf smd they have a TERRIBLE range, maybe top 1 meter.
```

---
## \#19 Posted by: wafflejock Posted at: 2017-07-22T21:18:42.146Z Reads: 228

```
That's not true really, mine works from about a half a block away if I have the settings on max for transmission and have a capacitor on there.  Usually I run them on the min broadcast strength which does only go a few meters in clear line of sight but can easily be blocked by any bags of water (people's bodies).
```

---
## \#20 Posted by: Sander Posted at: 2017-07-22T21:43:48.093Z Reads: 230

```
I am talking about the small SMD NRF, if you have two of them connected to eachother your range wont be over 2 metres.

<img src="/uploads/db1493/original/3X/6/7/675d45c1ce199e8a8703e954403c79602aff2458.png" width="500" height="500">
```

---
## \#21 Posted by: wafflejock Posted at: 2017-07-22T21:46:19.435Z Reads: 224

```
https://www.youtube.com/watch?v=juJ8yOPrZew

I'm at least three meters away have the same kind with the antennae built in and I have it using the min

    radio.setPALevel(RF24_PA_LOW);    //Set power level, lower consumes less power but is more easily obstructed

If I set it to max I can walk at least half a block down before I think I start to lose signal (or my hearing just isn't good enough).

Typically when I'm off the board I want it to stop too so it's sort of an extra "safety" measure for it to eventually lose signal and not making more noise on the 2.4GHz band when you stay low power.  New routers like Ubiquity and the like use 5GHz short range but good quality signals for most of the transmission and then use hard lines or 2.4GHz to a central hub because the 2.4GHz band is generally too congested everywhere.
```

---
## \#22 Posted by: Sander Posted at: 2017-07-22T21:53:43.690Z Reads: 210

```
No way I will get the same range with the smd nrf, I know about the PA, but I didnt use the capacitors.
```

---
## \#23 Posted by: wafflejock Posted at: 2017-07-22T21:55:27.113Z Reads: 218

```
Yeah definitely makes a difference when powering it from the arduino because the little spikes of extra juice it can pump through the antennae is more than what the Arduino can really keep supplying. Search for capacitors on this page, also the page in general helped me to get started with using this radio/chip:

https://arduino-info.wikispaces.com/Nrf24L01-2.4GHz-HowTo

I don't doubt the "real" antennae will do better than the embedded solution either just saying I don't know if it's worth it for this application.  Your design is super compact and would be easy to surface mount to other boards so it still has some advantages if you need something super micro but just hard to beat the price on the mass produced ones.

---

Also I still think adding a low power MCU with the nrf chip and breakouts like I have on mine would be great then it's all just one board for what we need here but not as multipurpose and probably price will still be a bit higher (maybe not when you count assembly and programming though).
```

---
## \#24 Posted by: Sander Posted at: 2017-07-22T22:06:20.298Z Reads: 207

```
> radio.setPALevel(RF24_PA_LOW); will be only 10 feet (3 meters) or so. But reliable

I have it on MAX, there is my problem ;)

Well you said you only get around 3 meters.

[quote="wafflejock, post:23, topic:28279"]
beat the price on the mass produced ones.
[/quote]

Not really the goal, the goal is to create an everyday use remote that has reliable connection. :slight_smile:

[quote="wafflejock, post:23, topic:28279"]
Also I still think adding a low power MCU with the nrf chip and breakouts like
[/quote]

Why should I add a MCU? Just wondering ;)
```

---
## \#25 Posted by: wafflejock Posted at: 2017-07-22T22:10:34.261Z Reads: 205

```
For doing a built in analog to digital converter and doing the interfacing to the nrf chip from the potentiometer and ESC.  You have basically a voltage divider with any sort of potentiometer and need to read that analog 0-VCC as a digital value (on ATMEGA328P chips it's a 10-bit ADC so you get 0-1024) from the potentiometer then send that using the nrf chip to the other board that receives it and needs to write a PWM signal to the ESC to tell it what throttle to go.  The board I made just has the three pin breakouts for connecting to the potentiometer and the ESC.  Since you're already looking at getting assembly done if you baked the ATMEGA328P or something similar that can both read the potentiometer and write to the ESC and talk to the nrf chips then you have everything baked onto one PCB (could even get surface mount potentiometer maybe I dunno).

---

Also even with these cheapo NRF boards my controller has been reliable the biggest problems I ran into were due to bad soldering on my part and a bit of weirdness that can happen when the MOSI pin gets disconnected and everything else is still connected (reading available() reports all good and reading data reports 255 on the receiver, but fixed it by only accepting values in the range of 1-254, still gives 125 steps of throttle up and throttle down and the data is a simple 8 bit stream nothing to parse).

---

I'm also using the voltage regulator on the Arduino for the power coming from the ESC or in the controller from the battery and need the tx/rx breakouts for programming.

---

Also consumers are price conscious (to some degree though Apple continually proves this wrong), so even if your remote turns out better it will cost considerably more for you to make it than some already decent competition that's out there (stuff mentioned above that is not great but not completely awful and cheap).   If you just make it for you that's all good but if you plan to sell to others you'll be doing it at a huge loss I think unless you think of price (assembly, shipping, customer service, etc.).
```

---
## \#26 Posted by: NAF Posted at: 2017-07-23T08:08:35.761Z Reads: 190

```
Yupp thats true. Cant wait for @Sander 's remote.
```

---
## \#27 Posted by: tueboard Posted at: 2017-07-23T11:56:20.676Z Reads: 185

```
Koowheel - nano - benchwheel - mini - gt2b

<img src="/uploads/db1493/original/3X/d/2/d2065f31f6472cf8f69afefdfaf1e80f4a7b0a64.jpg" width="666" height="500">

My favourites benchwheel and mini
```

---
## \#28 Posted by: wafflejock Posted at: 2017-07-23T16:08:33.627Z Reads: 185

```
Not to be ageist but look at the recent posts about alextech and realize this is the first attempt at developing a product and bringing it to market, keep you expectations set appropriately.  Don't get me wrong Sanders design so far is super impressive, but it took me 6months before I encountered the MOSI issue mentioned above, if I had gone straight to market without using mine for a year that problem would have never been caught, also were dealing with stuff here that requires fcc approval if it's sold assembled and programmed so there are legal things to deal with beyond the engineering (personally decided to give up pursuing building this because of all the legal issues, sold as a kit that needs assembly and programming can get around some of that but lots of potential to get sued or otherwise legally screwed here it seems)
```

---
## \#29 Posted by: evoheyax Posted at: 2017-07-23T16:34:32.873Z Reads: 182

```
Just set up an llc. Worst that can happen is you loss your llc's assets. Won't affect your personal stuff.

Honestly, we need people with knowledge and balls to bring to market better remotes. Not for reliability, but minimal data like speed and distance on the controller would be nice, along with modes (via vesc settings)

I looked at your stuff the other day and was pretty impressed. :P
```

---
## \#30 Posted by: wafflejock Posted at: 2017-07-23T16:49:56.843Z Reads: 179

```
I have an s-corp already for web development business, an llc is fine for protecting you personally from getting sued assuming you do all your paperwork correct and everything is legit, but that takes some time and effort as well otherwise things don't hold up in court if you make an error and xyz's lawyer's are better than yours.

Initially I thought the existing ones on the market were better than they are but have seen a lot of recent posts since I've been participating in the forum more recently about people having weird and seemingly dumb issues with remotes due mostly to dumb defaults (no failsafe by default and such things).  So I see there is definitely lots of room for improvement not to mention all the bells and whistles @Sander has been working on.

Personally opted to go with just what's necessary, this way no other BS to do, just get a throttle signal send it, receive it and use it, no other BS to do.  I had ordered one of those OLEDs but took a couple months to get here and don't really know what I would display on it that I can't get from looking at the board since it has a voltmeter on there and that's pretty much what I need to know... I ordered a metr module that should get here tomorrow and the interface and data gathering there already seems great.

Keep in mind again I do want to see this thing made eventually and I do think you can do better than everything currently available, just need to set expectations appropriately and not rush into something only to regret it, think if you take time with developing/testing/working out any potential legal issues then you have an awesome product.
```

---
## \#31 Posted by: lunasicc Posted at: 2017-07-23T17:01:54.505Z Reads: 163

```
Mad munkey gt2b enclosure from @FLATLINEcustoms..
The thread can now be closed:joy::joy:
```

---
## \#32 Posted by: NAF Posted at: 2017-07-23T17:12:45.916Z Reads: 173

```
All we actually need is a KIT with 3d printed enclosure...thus I don't understand why everyone tries to develop their own remote instead of taking super reliable GT2b or Mini Remote and just add additional functionality. This solution would legally cover you 100%.
```

---
## \#33 Posted by: wafflejock Posted at: 2017-07-23T17:24:18.653Z Reads: 174

```
Well that's sort of what I made but didn't think to try and get it to fit in an existing remote figured just make it as small as possible then design a shell to wrap around it... what you say makes good sense though.
```

---
## \#34 Posted by: evoheyax Posted at: 2017-07-23T17:32:50.954Z Reads: 173

```
Been saying this for a while... 100% agreed!
```

---
## \#35 Posted by: wafflejock Posted at: 2017-07-23T17:56:27.722Z Reads: 169

```
Also I've seen some mixed things on these remotes I think where the potentiometer is crappy I forget which particular remote it was honestly, but sort of silly if the shell isn't ideal and made with good components in the first place.  I can pocket mine which I see as a big advantage, never tried one of the thumb wheel remotes so no point of reference to compare there but I like the trigger style remote.

---

Also mine is basically a first iteration on the shell some other people are working on shells using the same guts.
```

---
## \#36 Posted by: NAF Posted at: 2017-07-23T19:46:28.633Z Reads: 154

```
I really doubt you've heard bad things about GT2b or Mini Remote.. These two are simply amazing. I've got Mini Remote ..no problems pairing the remote ..batteries last forever...I'have never lost signal not even once and i ride in the city all the time..and trigger works super precisely. The only drawback is that it would be nice to have good looking 3d mod.
```

---
## \#37 Posted by: wafflejock Posted at: 2017-07-23T20:21:30.676Z Reads: 147

```
Thought it was the gt2b where people said it was hit or miss on the potentiometer under the trigger failing but would have to do some searching around here to confirm.  Have also heard a lot of positive things about both just saying I'm not sure if any of them is ideal, would need to buy them all to compare really but pretty much leaving it to others to design the shell, I might redo my own as well but already seen some promising options out there.
```

---
## \#38 Posted by: pshaw Posted at: 2017-07-23T22:47:32.244Z Reads: 149

```
From what I've seen so far it looks like the following are pretty promising....

Benchwheel 
Gt2b w/ mad munkey enclosure
Mini

Like I said I haven't used anything other than a thumb wheel so I'm interested to see what the trigger would be like!
```

---
## \#39 Posted by: Jinra Posted at: 2017-07-23T23:18:35.666Z Reads: 155

```
Add Nano v2 to the list. Benchwheel + Nano v2 are the only remotes for so far. I'm a fan of thumb control since I have more control with it. There's a reason game console controllers have the thumbs for the analog stick ;)
```

---
## \#40 Posted by: pshaw Posted at: 2017-07-24T00:03:38.103Z Reads: 161

```
@Jinra nano v2? Got a good place to order from US?
```

---
## \#41 Posted by: Jinra Posted at: 2017-07-24T00:12:09.393Z Reads: 158

```
torqueboards has them, or on ebay here

http://www.ebay.com/itm/Mini-Remote-Controller-w-Receiver-Electric-Skateboard-Longboard-2-4GHz-US-Seller/172680052651
```

---
## \#42 Posted by: pshaw Posted at: 2017-07-24T00:35:33.638Z Reads: 153

```
Ugh.... have to calibrate min and max EVERY time you turn it on. 

I find it so hard to believe the remote area is so lacking as it is so crucial in my mind. Give me a remote that has a rechargeable battery, I can look at both remote batt and board batt, auto off... etc. 

Maybe I'm just spoiled by Boosted but these seem like pretty obvious features to have lol
```

---
## \#43 Posted by: Jinra Posted at: 2017-07-24T00:39:19.982Z Reads: 154

```
Yea that's the one bad thing about the remote, though I've gotten used to just fiddling with the throttle every time I turn it on now. The only thing I **really** care about is reliability which the two remotes I use now are delivering. With 10s4p I never really have to look at my battery levels, and the battery on the remotes lasts for weeks.
```

---
## \#44 Posted by: pshaw Posted at: 2017-07-24T00:50:42.071Z Reads: 152

```
So what is the list of remotes that don't have to be calibrated every time?
```

---
## \#45 Posted by: Jinra Posted at: 2017-07-24T00:53:24.459Z Reads: 152

```
Only the Nano v2 and Nano-x have this draw back.
```

---
## \#46 Posted by: tueboard Posted at: 2017-08-08T00:48:48.943Z Reads: 145

```
i don't know if someone posted this, looks cool

https://www.youtube.com/watch?v=x0iw8KbLJnc
```

---
## \#47 Posted by: Bensaida Posted at: 2017-08-08T02:19:34.580Z Reads: 145

```
The new genesis remotes are copies of the boosted remote, and are specially designed for the genesis boards. They have haptic feedback and a nice grip
```

---
## \#48 Posted by: chaka Posted at: 2017-08-08T13:34:38.200Z Reads: 144

```
You are thinking of the quanum remote. It is terrible, the pots drift constantly. The GT2B is the most reliable option out right now. Pair it with the Mad Munkey enclosure and you wont be disappointed!
```

---
## \#49 Posted by: pshaw Posted at: 2017-08-08T14:28:26.048Z Reads: 142

```
[quote="chaka, post:48, topic:28279, full:true"]
You are thinking of the quanum remote. It is terrible, the pots drift constantly. The GT2B is the most reliable option out right now. Pair it with the Mad Munkey enclosure and you wont be disappointed!
[/quote]

Seems like trigger style would be really bad considering it is natural to tighten your grip when getting squirly. No?
```

---
## \#50 Posted by: chaka Posted at: 2017-08-08T14:43:18.724Z Reads: 136

```
First thing you should do is learn to fall, you don't want to make a fist when getting personal with asphalt and you also want to make sure you are not making unintentional movements from fear or panic. It is second nature for me to get my palms out when things go sideways. Having a puck in your non throttle hand is also a good idea.  A trigger style remote feels more natural and offers less fatigue.  Above all else the gt2b has proven to be the most reliable connection.
```

---
## \#51 Posted by: Ulfberht Posted at: 2017-08-08T21:46:12.432Z Reads: 132

```
There's also the Mastercho Mod that works with the GT2B internals. No USB relocation required. 15% Carbon Fiber reinforced ABS filament. :grinning:
http://www.ebay.com/itm/GT2B-Electric-Skateboard-Controller-Housing-Case-Enclosure-BLACK-/252496558132?hash=item3ac9f7b834:g:Ys4AAOSw5UZY~XFz
```

---
## \#52 Posted by: Jedi Posted at: 2017-08-08T23:27:23.246Z Reads: 124

```
By far the best remote, the forgotten remote: the Wiiceiver. This remote is the best for one reason: cruise control. It's so easy, just hold the trigger finger button to cruise. For 90% of my ride, my grip is closed around the remote, no lifted fingers. I can swap hands without changing speed. It's also ergonomic and has an extra button for customization, like powering lights. Ha I sound like I'm selling them. Doesn't the vesc have a built in wiiceiver? I don't know why people stopped using them. I've never had the dropout issues others complained about.

<img src="/uploads/db1493/original/3X/a/1/a12645328fb8b219e8e8796ae26ecb942f063a97.PNG" width="620" height="410"> 

As for new remotes, I'd like to see one built into the housing of a flashlight. Like those cheap aluminum led gas station flashlights, with a joystick on one end and flashlight on the other. Oh and with a digital speedometer and battery gauge.

<img src="/uploads/db1493/original/3X/2/6/26e69829290db984abd3953090443c1b13b6ec3c.JPG" width="499" height="500">
```

---
