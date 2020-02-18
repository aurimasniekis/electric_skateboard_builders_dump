# Focbox in FOC mode

### Replies: 105 Views: 6767

## \#1 Posted by: florensvb Posted at: 2017-09-25T15:57:19.207Z Reads: 504

```
Hey guys,

When I first tried FOC I immediately fried my torqueboards vesc, so I got myself a Focbox from enertion. Been riding with it for a few months and havent had any issues so far. I'd like to keep it that way. But the FOC mode just seems soo much nicer that I can't stop thinking about it. Two questions:

1. The sensor cable on my motor ripped off a long time ago. Can I run FOC sensorless? (side question: Could I short my motor because the cable ripped off?) 

2. Is it OK to run FOC on the enertion vesc or am I likely to fry it as well?

And as always: Thanks a bunch guys
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-09-25T15:58:51.356Z Reads: 474

```
Yes and Yes.

It wouldn’t be called the FOCbox if it couldn’t handle FOC 😉
```

---
## \#3 Posted by: Jinra Posted at: 2017-09-25T15:59:43.319Z Reads: 468

```
1. Yes, and probably not, but you should probably secure the ripped leads.

2. Of course, it's the FOC box, just make sure you set it up right and do **not** apply more throttle if the motor doesn't move or acts weird, this is how people blow their VESCs.
```

---
## \#4 Posted by: pjotr47 Posted at: 2017-09-25T16:00:14.455Z Reads: 460

```
1: I ride Foc on a focbox sensorless.
2: I have ride +- 50km with the Focbox on foc and it works fine, its very silent on low speed. The speed top is lower than BLDC but there are solutions for (gears)
```

---
## \#5 Posted by: florensvb Posted at: 2017-09-25T16:00:22.914Z Reads: 446

```
Thats exactly how i blew my VESC!!
```

---
## \#6 Posted by: florensvb Posted at: 2017-09-25T16:01:08.839Z Reads: 441

```
[quote="Jinra, post:3, topic:33934"]
but you should probably secure the ripped leads.
[/quote]

I cant see them anymore. Can you give me a rundown on how to open it up?
```

---
## \#7 Posted by: pjotr47 Posted at: 2017-09-25T16:02:54.092Z Reads: 429

```
What motor do you have?
```

---
## \#8 Posted by: florensvb Posted at: 2017-09-25T16:03:15.783Z Reads: 426

```
products/electric-skateboard-motor-5065-260kv
```

---
## \#9 Posted by: Jinra Posted at: 2017-09-25T16:03:28.601Z Reads: 420

```
Your motor should have a circlip (google if you're not familiar with them) on the shaft near the base. Use circlip pliers to take them off (don't widen them too much or you wont be able to put it back on, or break them). Take out any washers under the circlip. Pull and separate the rotor can from the stator and base plate, you'll need a bit of force to get it out since they're strong magnets. From there you should be able to see the sensor PCB and desolder the leads.
```

---
## \#10 Posted by: florensvb Posted at: 2017-09-25T16:06:00.954Z Reads: 412

```
Seems daunting, that would also mean id have to take off the motor pulley again and thats always such a ***** :D How likely am I to short my motor?
```

---
## \#11 Posted by: Jinra Posted at: 2017-09-25T16:06:36.888Z Reads: 405

```
Well there should be no electricity flowing through the leads since they're not plugged in anyway, you should be fine, it's just not elegant.
```

---
## \#12 Posted by: florensvb Posted at: 2017-09-25T16:10:55.060Z Reads: 400

```
Ok I'll be trying FOC mode soon then and let you guys know how it went. 

Any great tutorials to recommend?
```

---
## \#13 Posted by: Silverline Posted at: 2017-09-25T16:11:54.874Z Reads: 389

```
Just don`t upgrade your focbox to the new vesc-tool fw. Then your focbox is not a focbox anymore. Hope they fix the problem soon....
```

---
## \#14 Posted by: florensvb Posted at: 2017-09-25T16:12:22.118Z Reads: 386

```
no worries, i'll just leave it as it is
```

---
## \#15 Posted by: Jinra Posted at: 2017-09-25T16:14:15.440Z Reads: 388

```
You can always just downgrade it again.
```

---
## \#16 Posted by: florensvb Posted at: 2017-09-25T16:24:25.487Z Reads: 395

```
this a good tutorial? Anything else i might need to watch out for?

https://www.youtube.com/watch?v=xSCEFK7Zljw
```

---
## \#17 Posted by: Mikenopolis Posted at: 2017-09-25T18:59:22.693Z Reads: 390

```
I fried a VESC-X (FocBox) with maybe a mile of testing usage. Not sure what happened but one got a fault and the other didn't with same setting over split ppm. Scared of FOC now, not even because of the cost to repair or replace but the potential danger of failure during an actual ride
```

---
## \#18 Posted by: florensvb Posted at: 2017-09-25T19:11:04.602Z Reads: 388

```
oh man thats scaring me too now haha

i was gonna do it tomorrow morning
```

---
## \#19 Posted by: Crossfire Posted at: 2017-09-25T19:48:37.539Z Reads: 390

```
Well, double check everything before you go test riding. Check for possible motor wire shorts, strippings and what not. Only when you’re 100% confident go at it. Helmet is obligatory. 
I was not afraid of FOC, if you do everything right in BLDC tool (conservative parameters with some help of mathematics) and get the motors to spin and everything sounds right when triggered-it’s miles better than bldc imho.

I had my first test ride today with my dual 6355 190kV sensored with Focboxes in FOC mode over can bus. Well, that’s it, I’m done searching and wondering. It’s brutally beautiful to ride, silent, pulls like a motherf****r and brakes like a sportscar. 

If somebody wants more performance from their single drive, just don’t stress the components even more with OC parameters in BLDC tool. Double the drive. It’s unbelievable.
```

---
## \#20 Posted by: UniqueSnowflakeN27 Posted at: 2017-09-25T20:07:54.963Z Reads: 381

```
[quote="florensvb, post:1, topic:33934"]
When I first tried FOC I immediately fried my torqueboards vesc,
[/quote]

What settings did you have? [I ran FOC on my Torqueboards VESC "without any issues"...](https://www.youtube.com/watch?v=XG4XvvkLFKw)
```

---
## \#21 Posted by: florensvb Posted at: 2017-09-25T20:23:29.725Z Reads: 357

```
I can't remember anymore haha I just did the normal detection from vedder's video
```

---
## \#22 Posted by: florensvb Posted at: 2017-09-25T20:24:18.697Z Reads: 369

```
[quote="Crossfire, post:19, topic:33934"]
if you do everything right in BLDC tool (conservative parameters with some help of mathematics)
[/quote]

Please elaborate my humble friend :smile:
```

---
## \#23 Posted by: scepterr Posted at: 2017-09-25T20:40:55.971Z Reads: 359

```
It's called the focbox cause the vesc name got trademarked...it's a vesc-x which is a vesc 4.12 with a few upgrades. Personally I've found the ollin vesc to be most reliable and guaranteed to have upgraded components.  
I can't recall anywhere near as many incidents of them getting killed in a couple miles compared to focbox

@florensvb doing detection with the battery being used on the board?
```

---
## \#24 Posted by: Crossfire Posted at: 2017-09-25T20:58:34.747Z Reads: 350

```
Well, the usual such as motor and battery specs from which you calculate min and max amps. Beside the FOC motor setup those are practically the most important ones which can make an impact on performance. But as I’ve learned the hard way, more performance equals more cooling. Keep them fets as low temp as possible. Air flow is crucial.

Evolve carbon gt has a text book example of efficient vesc cooling ;)
```

---
## \#25 Posted by: Yecrtz Posted at: 2017-09-25T22:22:44.930Z Reads: 345

```
Using DIY Vesc in FOC on 10s (192kv single) and since last week two FOCboxes in FOC on my Trampa on 12s (149kv dual) without any problems whatsoever. First configured everything in bldc and then switched and configured to FOC. No special firmwares or anything.
```

---
## \#26 Posted by: Mikenopolis Posted at: 2017-09-25T22:28:34.580Z Reads: 345

```
I just took out my FocBox with the fault to send to our DRV Wizard. I noticed these pins on the DRV8302 looks to be soldered together. I wonder if that's my issue....if so, is this user error or manufacturer error? <img src="/uploads/db1493/original/3X/e/e/eedc9efddf9a0216ebc5bd316fc502b4dbca984b.jpg" width="281" height="500">
```

---
## \#27 Posted by: Jinra Posted at: 2017-09-25T22:54:16.330Z Reads: 329

```
those legs are supposed to be bridged as shown
```

---
## \#28 Posted by: Mikenopolis Posted at: 2017-09-25T23:01:20.532Z Reads: 334

```
thanks, good to know. Guess there are no visible signs of damage, no smell, no burn marks, nothing. Off to Canada it goes
```

---
## \#29 Posted by: SeanHacker Posted at: 2017-09-26T00:04:11.479Z Reads: 330

```
I send all my vesc-x's (FOCBoxes) to Canada too. @Blasto is super cool and is probably the only guy next to @JohnnyMeduse that I would want touching my expensive vescs. They both know their stuff.
```

---
## \#30 Posted by: Mikenopolis Posted at: 2017-09-26T00:24:20.938Z Reads: 330

```
"send ALL my vesc-x" hmmm how many is that?! Sounds like they can't be trusted
```

---
## \#31 Posted by: Mikenopolis Posted at: 2017-09-26T02:19:34.772Z Reads: 334

```
From the wizard himself....nothing to see here.

<img src="/uploads/db1493/original/3X/1/6/1603178e68e642b3b1a91dc84531d587ef78559e.jpeg" width="475" height="500">
```

---
## \#32 Posted by: florensvb Posted at: 2017-09-26T11:45:12.924Z Reads: 322

```
Ok guys, just switch to FOC and went on my first ride! Never going back hahahha. Just did the 3 calculations in the Foc tab and hit apply, done. 

Oh hell yeah its soo quiet and smooth. People here in Berlin went from “whats this guy there a 100 metres away doing on that humming machine” to “wohow what just passed me?!” :D 

Few questions:

1. What can i do about the start up stutter?
2. The brakes are also smooth, except for when i get pretty slow, then it just hits the brakes to dead stop.
3. Can i try full throttle now without blowing the thing up? haha

Cheers guys
```

---
## \#33 Posted by: i2oadsweepei2 Posted at: 2017-09-26T12:00:38.251Z Reads: 310

```
I felt the same way when I tried foc the first time. It's so awesome. If your motors are sensored then you can set that up on the vesc-x too. It will start smoothly then. I just did this. You need the proper cable to attach the motor sensor to the vesc. I'm running sensored foc on both of my boards now.


Edit* thought I read something about this and I'm sorry to hear that. It would be prudent to make sure none of those tiny wires are touching each other. There are people who say they have good start up without sensored by tweaking their vesc's.

[quote="florensvb, post:1, topic:33934"]
The sensor cable on my motor ripped off a long time ago. Can I run FOC sensorless? (side question: Could I short my motor because the cable ripped off?)
[/quote]
```

---
## \#35 Posted by: i2oadsweepei2 Posted at: 2017-09-26T12:05:19.170Z Reads: 293

```
I just saw that and edited my post lmao
```

---
## \#36 Posted by: florensvb Posted at: 2017-09-26T12:07:40.675Z Reads: 300

```
yeah haha what kind of vesc settings can i tweak with?

 [quote="Jinra, post:11, topic:33934, full:true"]
Well there should be no electricity flowing through the leads since they're not plugged in anyway, you should be fine, it's just not elegant.
[/quote]

hope thats true hahaha

actually i feel like the startup problem is no big deal cause i can just give one kick but the brakes at low speed are really weird :D
```

---
## \#37 Posted by: i2oadsweepei2 Posted at: 2017-09-26T12:09:41.643Z Reads: 309

```
Perhaps this could help.
This is in ackmaniacs extended firmware.
<img src="/uploads/db1493/original/3X/3/9/39e8ab0fb93d02e825649bf828e7cb920d99814d.JPG" width="669" height="500">
```

---
## \#38 Posted by: i2oadsweepei2 Posted at: 2017-09-26T12:11:06.757Z Reads: 293

```
This is true, I find it a bit unnatural or uncomfortable even not kick pushing to start. So I do it anyway.
```

---
## \#39 Posted by: hornet90 Posted at: 2017-09-26T12:33:26.270Z Reads: 301

```
Im the same i blew a vesc in foc mode
I got a focbox i didnt set up foc yet on it 
But same thing cant stop thing how nice it was
It felt like floating like i had no wheels.....
Im setting up again this week end
```

---
## \#40 Posted by: florensvb Posted at: 2017-09-26T12:45:11.193Z Reads: 301

```
its like floating and only took me a min to set up. no issues after first 2hrs ride
```

---
## \#41 Posted by: Mikenopolis Posted at: 2017-09-26T18:10:35.652Z Reads: 304

```
took me a minute to setup and maybe a block to blow something (DRV fault). One FocBox is on it's way to Canada for repair, the other still works. exact same settings running split ppm. Not sure I want to attempt Foc for a while
```

---
## \#42 Posted by: florensvb Posted at: 2017-09-27T14:07:56.851Z Reads: 293

```
thats sad to hear
```

---
## \#43 Posted by: florensvb Posted at: 2017-09-27T14:08:44.585Z Reads: 293

```
Actually my brakes increase very smoothly until i hit a certain point and baam it slams them all the way... how is that? any ideas? :)
```

---
## \#44 Posted by: GrecoMan Posted at: 2017-09-27T14:21:15.282Z Reads: 293

```
Lower motor min by a bit
```

---
## \#45 Posted by: GrecoMan Posted at: 2017-09-27T14:22:20.202Z Reads: 293

```
<img src="/uploads/db1493/original/3X/b/e/be455618bae645c400c5826759e2ebf00f3562d2.png" width="281" height="499">

I always keep this handy when programming my vesc
```

---
## \#46 Posted by: flywithgriff Posted at: 2017-09-27T14:22:56.727Z Reads: 277

```
Lol I have this exact screenshot!
```

---
## \#47 Posted by: GrecoMan Posted at: 2017-09-27T14:24:12.951Z Reads: 275

```
Guess I’m not the only one 😉
```

---
## \#48 Posted by: florensvb Posted at: 2017-09-27T14:24:13.990Z Reads: 269

```
thanks mate will try straight away haha
```

---
## \#49 Posted by: GrecoMan Posted at: 2017-09-27T14:24:50.698Z Reads: 273

```
Easily the most useful screenshot I have on my phone...

Thanks @Ackmaniac
```

---
## \#50 Posted by: florensvb Posted at: 2017-09-27T17:35:03.258Z Reads: 277

```
Alright, jamming the brakes at low speed is a thing of the past! Though i am not too too happy yet because now the brakes at mid speed seem to have gotten a little too weak and i dont wanna increase my battery regen because its already at 2C. Will tweak around more with the values i guess :) 

One question though: If i tweak around with those values- will i have to repeat the foc detection process every time, or are those independent of each other?
```

---
## \#51 Posted by: GrecoMan Posted at: 2017-09-27T17:40:51.271Z Reads: 279

```
those are independent
```

---
## \#52 Posted by: Jinra Posted at: 2017-09-27T17:42:13.610Z Reads: 282

```
No need to redo detection. Make sure you use firmware 3.29 as it has a bandaid fix for the brakes.
```

---
## \#53 Posted by: florensvb Posted at: 2017-09-27T17:43:02.438Z Reads: 288

```
Ok guys i actually still have questions... for example this post 

http://www.electric-skateboard.builders/t/what-amp-watt-are-most-people-having-success-with-are-10a-18650s-strong-enough/34008/4?u=florensvb

Take a look at my VESC settings:

<img src="/uploads/db1493/original/3X/e/8/e8c1142ea548400796e078049b670fbb7a343c36.png" width="690" height="412">

My motor 

products/electric-skateboard-motor-5065-260kv

My batteries

https://hobbyking.com/en_us/zippy-flightmax-8000mah-4s1p-30c.html

Do my settings seem legit? I do like hard acceleration that's for sure. But don't wanna ruin my batteries or anything else like the focbox haha.

Also: Is there a way to limit the max erpm in foc?
```

---
## \#54 Posted by: Jinra Posted at: 2017-09-27T17:44:15.550Z Reads: 274

```
oh you're using BLDC tool, forget my last message then. For stronger brakes inversely match your motor min to your motor max. You don't need to limit eRPM, but it's on the page you posted if you want to for whatever reason.
```

---
## \#55 Posted by: Mikenopolis Posted at: 2017-09-27T17:44:52.903Z Reads: 270

```
[quote="florensvb, post:50, topic:33934"]
Will tweak around more with the values
[/quote]

That's probably how I killed a FocBox....but just one even though the other is set the same. I checked the motor for shortage and it was fine....anyone have any idea why one would fry but not the other?
```

---
## \#56 Posted by: Jinra Posted at: 2017-09-27T17:45:19.786Z Reads: 258

```
Sounds like your FOCbox was just faulty
```

---
## \#57 Posted by: florensvb Posted at: 2017-09-27T17:46:14.086Z Reads: 257

```
[quote="Jinra, post:54, topic:33934"]
You don't need to limit eRPM, but it's on the page you posted if you want to for whatever reason.
[/quote]

But it says for BLDC only above those settings
```

---
## \#58 Posted by: scepterr Posted at: 2017-09-27T17:46:50.761Z Reads: 249

```
Sadly yes, whether you get a rock solid focbox or one that dies in less than 10 miles just depends on luck.
```

---
## \#59 Posted by: florensvb Posted at: 2017-09-27T17:46:59.479Z Reads: 254

```
[quote="Jinra, post:54, topic:33934"]
oh you're using BLDC tool, forget my last message then. For stronger brakes inversely match your motor min to your motor max.
[/quote]

Should i be using that upgraded version of bldc? it actually makes that much of a difference that youd have different parameters??
```

---
## \#60 Posted by: Jinra Posted at: 2017-09-27T17:47:29.166Z Reads: 255

```
Ah woops, it's on app config > PPM > RPM soft limits.

I had a much better experience on vesc tool 3.xx firmware on FOC, than on 2.18/2.54
```

---
## \#61 Posted by: florensvb Posted at: 2017-09-27T17:48:21.937Z Reads: 253

```
[quote="Jinra, post:52, topic:33934"]
Make sure you use firmware 3.29 as it has a bandaid fix for the brakes.
[/quote]

Ok i am a little daunted by flashing the firmware but i guess i'll have to do that as well :D Is there a vesc-tool for mac?
```

---
## \#62 Posted by: Mikenopolis Posted at: 2017-09-27T17:48:22.683Z Reads: 245

```
so in your more "pro" opinion, I should try FOC again when I get the FocBox back from repair? it's like putting $300 down on a bet...**sigh**
```

---
## \#63 Posted by: florensvb Posted at: 2017-09-27T17:49:15.044Z Reads: 247

```
[quote="Mikenopolis, post:62, topic:33934"]
it's like putting $300 down on a bet...sigh
[/quote]

so true. but i could not resist and i really never ever wanna go back. like it's worth it i guess. but i also should add that i have the extra warranty so they should fix it whatever i do haha
```

---
## \#64 Posted by: florensvb Posted at: 2017-09-27T17:49:55.456Z Reads: 244

```
wow i can't even imagine what could still be better? :D
```

---
## \#65 Posted by: joeadams101 Posted at: 2017-09-27T17:50:54.162Z Reads: 246

```
Thinking about going Foc this weekend. I have 2 focbox's and 6355 dual motors. Do I jist literally change the option for bldc to foc and done?
```

---
## \#66 Posted by: Jinra Posted at: 2017-09-27T17:51:25.048Z Reads: 249

```
FOC has always been a bit of a risk, if you don't want to chance it, just run BLDC
```

---
## \#67 Posted by: florensvb Posted at: 2017-09-27T17:51:41.439Z Reads: 251

```
watch this 

https://www.youtube.com/watch?v=bYYNbxPXNEU&t=234s
```

---
## \#68 Posted by: Jinra Posted at: 2017-09-27T17:52:48.892Z Reads: 244

```
My motors stuttered at high RPM on f/w 2.xx. Also, when I was on the bench at max duty and applied more throttle it changed the pitch of the motor to a lower tone. I think these things would potentially blow my VESC if I used it that way.

With 3.xx both these issues were non existent.

@joeadams101 No you need to redo detection
```

---
## \#69 Posted by: Blasto Posted at: 2017-09-27T17:53:01.330Z Reads: 239

```
[quote="joeadams101, post:65, topic:33934"]
Do I jist literally change the option for bldc to foc and done?
[/quote]

no you need to do the FOC motor detection as well
```

---
## \#70 Posted by: Mikenopolis Posted at: 2017-09-27T17:54:26.895Z Reads: 234

```
a little more. in the FOC tab, there are some measuring and applying, but it's pretty simple...I'll do as @Jinra said and attempt FOC one more time and take the $300 loss if needs be
```

---
## \#71 Posted by: Jinra Posted at: 2017-09-27T17:56:25.783Z Reads: 231

```
I'd say the majority of the way people kill their VESCs is applying too much throttle when things aren't moving or aren't moving correctly. If you set it up and apply a little bit of throttle and it doesn't move, **do not** slam the throttle forward and back like 99% of the videos people post on here. Applying full throttle == applying max current you set. 60A-ish current on a non moving system is an easy way to blow your VESC.
```

---
## \#72 Posted by: Mikenopolis Posted at: 2017-09-27T18:08:17.942Z Reads: 230

```
My first issue was cut out during acceleration, then it was cogging, finally it all seems to be perfect and I got was what I thought was weak brakes, turns out it was because one motor/vesc wasn't working
```

---
## \#73 Posted by: flywithgriff Posted at: 2017-09-27T18:10:14.507Z Reads: 224

```
Exact same issue!!!
```

---
## \#74 Posted by: florensvb Posted at: 2017-09-27T18:11:09.849Z Reads: 229

```
Ok:

1. Where do I get the 3.29 firmware?

2. Can I upload the firmware from my standard bldc tool firmware tab?

3. Where do i get the bldc version for 3.29 -> Should i get the extended bldc?
```

---
## \#75 Posted by: Jinra Posted at: 2017-09-27T18:12:34.968Z Reads: 227

```
vesc-project.com They don't have a compiled version for Mac, though I think someone on here might've compiled the latest release.
```

---
## \#76 Posted by: florensvb Posted at: 2017-09-27T18:14:39.721Z Reads: 225

```
Alright I'll just boot my mac in windows to do it
```

---
## \#77 Posted by: jct1212 Posted at: 2017-09-27T18:19:36.477Z Reads: 227

```
https://github.com/rpasichnyk/vesc_tool/releases

v0.82 there has firmware 3.29 compiled for Mac thanks to @rpasichnyk
```

---
## \#78 Posted by: Mikenopolis Posted at: 2017-09-27T18:31:10.513Z Reads: 225

```
I just downloaded the VESC_Tool 0.82. Did I have to do something like upgrade the firmware of the FocBox before connecting?
```

---
## \#79 Posted by: Jinra Posted at: 2017-09-27T18:33:11.518Z Reads: 227

```
Once you connect it'll work in limited comms mode until you flash 3.29 to the FOCbox
```

---
## \#80 Posted by: florensvb Posted at: 2017-09-28T20:04:26.217Z Reads: 223

```
did you try foc already? :)
```

---
## \#81 Posted by: Mikenopolis Posted at: 2017-09-28T20:08:24.067Z Reads: 232

```
nope. not going to do anything until my vesc comes back. still on it's way to Canada at the moment
```

---
## \#82 Posted by: joeadams101 Posted at: 2017-10-01T17:59:19.007Z Reads: 228

```
Final okay needed!!!

https://www.electric-skateboard.builders/t/one-final-check-before-take-off-need-the-ok/34451
```

---
## \#83 Posted by: Mikenopolis Posted at: 2017-10-07T03:57:49.147Z Reads: 222

```
As Shaggy said. 🎼It wasn't me🎶🎵🎶🎵
<img src="/uploads/db1493/original/3X/c/8/c8325f8bfff71e88e5e6b55081f45bfcc9585b99.jpeg" width="389" height="500">
```

---
## \#84 Posted by: Yecrtz Posted at: 2017-10-13T23:40:01.882Z Reads: 204

```
Yea focboxes and foc.. Big nope. A colleague from work fried (surprisingly just) one of the two focboxes in my freshly made trampa board.

Dual focbox on dual sk3 149kv on 12s. Motor max 45, motor min - 30, batt max 45, batt min - 20. Also did a proper motor detection and all the usual stuff. Very disappointed.. :(
```

---
## \#85 Posted by: florensvb Posted at: 2017-10-14T08:55:44.862Z Reads: 208

```
hm sad to hear :( Ive been running it without problem so far .. Its definitely much much less likely to happen in the focbox than the torqueboards vesc (for example) but it still does happen ..

do you have the extended warranty?
```

---
## \#86 Posted by: i2oadsweepei2 Posted at: 2017-10-14T10:21:58.964Z Reads: 207

```
Been running sensored foc here too on both my boards for quite some time. One board is 8s and one is 12s. So far no issues (knocks on wood). I usually heed the old warning of "If it isn't broke, don't fix it". Is it worth upgrading from 2.54 to the new extended bldc firmware @jinra?
```

---
## \#87 Posted by: florensvb Posted at: 2017-10-14T10:46:03.814Z Reads: 204

```
i am still running the enertion fw :D never changed it
```

---
## \#88 Posted by: Crossfire Posted at: 2017-10-14T11:58:27.281Z Reads: 202

```
Did you monitor the temps? What is the airflow in the enclosure? Possible shorts?
```

---
## \#89 Posted by: i2oadsweepei2 Posted at: 2017-10-14T12:39:17.244Z Reads: 201

```
I've never tried the stock firmware. I swapped it out right away for 2.54.
```

---
## \#90 Posted by: florensvb Posted at: 2017-10-14T13:11:46.554Z Reads: 200

```
[quote="i2oadsweepei2, post:86, topic:33934"]
I usually heed the old warning of "If it isn't broke, don't fix it". Is it worth upgrading from 2.54 to the new extended bldc firmware @jinra?
[/quote]

[quote="Jinra, post:60, topic:33934"]
I had a much better experience on vesc tool 3.xx firmware on FOC, than on 2.18/2.54
[/quote]

That should answer your question :)
```

---
## \#91 Posted by: i2oadsweepei2 Posted at: 2017-10-14T13:36:33.734Z Reads: 195

```
Ah yes. That is probably good advice. Thank you.
```

---
## \#92 Posted by: Yecrtz Posted at: 2017-10-16T11:47:27.632Z Reads: 188

```
Yes monitored temps, never exceeded 49 degrees celcius (peak at most rides). Closed enclosure without any shorts.
```

---
## \#93 Posted by: Crossfire Posted at: 2017-10-16T12:18:43.962Z Reads: 199

```
I'm getting temps around 29C max in the mornings (7C ambient) and around 41C max in the afternoon (21C ambient) - closed but not watertight enclosure.
I'm on 10S, dual FB's with Canbus on FOC. Been driving it for about 2 weeks now, clocked around 80 kilometers so far no problems. I'm trying not to over abuse the parts...

I really hope the setup survives until the winter...it's really odd that these things fail at random. 
I'm still using stock FW. 

It's just a pity to put that much money, time and care into the build and then a 150$ part goes awry so soon. 

What boggles me sometimes is: I've basically set up a similar electronics build as found in the raptor (minus the fuse). Dual FB's, canbus, 10S 30Q , FOC. Theoretically the FB should survive the 12S but why is the raptor 2 only on 10S then? 
So yeah, they have their reasons to use the configuration that they use. And replicating that electronics config should not make things worse...in theory at least.
```

---
## \#94 Posted by: florensvb Posted at: 2017-11-19T16:50:26.908Z Reads: 196

```
Hey guys,

I set up my second build today and am a little stuck on the foc configuration step.

I switched the mode to FOC, hit measure R and L. Did it, done.
Then hit Measure Lambda (Reg: R) but it says Bad Detection Results and does not give me the Lambda value.

What can i do?
```

---
## \#95 Posted by: florensvb Posted at: 2017-11-20T08:07:49.422Z Reads: 186

```
@Jinra sorry for pinging- but youre my Foxbox guru :) do you have any clues what i could do? cheers
```

---
## \#96 Posted by: Jinra Posted at: 2017-11-20T08:49:01.181Z Reads: 185

```
what f/w are you on? does BLDC detection work?
```

---
## \#97 Posted by: florensvb Posted at: 2017-11-20T09:23:58.152Z Reads: 183

```
I am using the standard Enertion fw and a SK3 6364 190kv unsensored motor. BLDC detection also fails
```

---
## \#98 Posted by: Jinra Posted at: 2017-11-20T15:42:48.344Z Reads: 182

```
you might have a motor short or it's hooked up wrong, pics?
```

---
## \#99 Posted by: Mikenopolis Posted at: 2017-11-20T16:17:28.367Z Reads: 189

```
Update on my one failed FocBox on dual Carvon V3 setup (split ppm all settings the same). I had mine fixed, I decided to stay on BLDC for a bit. Everything worked spectacularly, rode about 40 mile on bldc. 

Finally decided to change it to FOC right before SPD2. Test rode it for a mile or so and it worked. Next morning at SPD2 I rode it for maybe 50 yards and one drive stopped working. Opened it up and the same vesc had a fault. Luckily DRVWiard was also there and swapped it out at the end of the day. I’ve gotten 30 mile on FOC now and still working (fingers crossed) I’m thinking I just a bad first batch Vesc-X?
```

---
## \#100 Posted by: florensvb Posted at: 2017-11-20T18:17:40.144Z Reads: 189

```
motor short would be super surprising as its brand new. the first detection step works and the motor spins but then the second fails.

<img src="/uploads/db1493/original/3X/e/5/e57116c964a3837faae64a6745d9714219d3db5b.jpg" width="375" height="500">
```

---
## \#101 Posted by: Jinra Posted at: 2017-11-20T18:24:01.431Z Reads: 181

```
Sometimes the motor mounting screws are too long and can hit the copper and cause a short, maybe check for that?
```

---
## \#102 Posted by: florensvb Posted at: 2017-11-20T18:24:52.115Z Reads: 179

```
mhm thatd also be surprising as the mount and screws are from @fottaz but ill for sure check that as well when i am home and get back to you- cheers
```

---
## \#103 Posted by: Jinra Posted at: 2017-11-20T18:25:38.569Z Reads: 182

```
You'd be surprised. TB's screws tend to be too long and end up shorting the motor.
```

---
## \#104 Posted by: fottaz Posted at: 2017-11-20T19:37:52.698Z Reads: 182

```
My mounts have 10mm bolts, they cannot really touch anything inside
```

---
## \#105 Posted by: florensvb Posted at: 2017-12-13T15:12:15.072Z Reads: 157

```
This problem somehow solved itself. Only thing I changed was to charge the battery all the way up, maybe i should have done that to begin with? Anyways, thanks for the help @Jinra !
```

---
## \#106 Posted by: epss4 Posted at: 2019-02-14T17:42:33.805Z Reads: 49

```
Hey mate ! Did you have any problem with your build with no fuse ? Im looking for doing the exact same as raptor but on 12S and i won’t put a fuse ...any advice for me :)? 
Thanks !
```

---
