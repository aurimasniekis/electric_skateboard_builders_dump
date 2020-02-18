# EleSk8 Receiver &#124; The receiver that makes your iPhone into a controller

### Replies: 35 Views: 4484

## \#1 Posted by: hugohammarstrom Posted at: 2016-05-16T17:02:48.156Z Reads: 396

```
I´ve been making a receiver to control electric skateboards for the last couple of weeks. When I first started researching how to build electric skateboards, one of the few things that struck me was that there was no way to use a phone to control the throttle, or more exactly. No way to use iPhones to control the throttle. 

The Receiver that I’ve designed (EleSk8 Receiver) is totally plug and play. You just plug the ESC into one of the two servo ports, open the iPhone app and start riding.

The estimated price for this receiver should be about **$35** (incl. Shipping inside Europe from Sweden) outside Europe another $10

Is this something that the electric skateboarding community is interested in?



----------

<img src="/uploads/db1493/original/2X/b/b47efea1086dcee5448ca5e28d6ae5a18fd7450b.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/7/72ad8f6409f62ff7b5e51e3bc63f2f8343a157de.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/6/656ac19075a512b8c122f8f6e010514b4dc2dc4c.jpg" width="281" height="499">
```

---
## \#2 Posted by: paragon Posted at: 2016-05-16T17:12:46.266Z Reads: 370

```
Very nice, but the issue is interference in crowded areas.  Does it connect via wifi or bluetooth?
```

---
## \#3 Posted by: hugohammarstrom Posted at: 2016-05-16T17:18:19.767Z Reads: 368

```
@paragon Yes that may be an issue. Nothing that I've noticed but I don't live in a crowded area. And yes it does connect over bluetooth.
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-05-16T17:26:25.850Z Reads: 360

```
[quote="hugohammarstrom, post:1, topic:3348"]
one of the few things that struck me was that there was no way to use a phone to control the throttle, or more exactly. No way to use iPhones to control the throttle.
[/quote]

for most of us, that's not a problem that needs fixing. The reason we use GT2Bs, GT2B clones, steez remotes, and other 2.4GHz FHSS remotes is because bluetooth and wifi are notorious signal droppers and prone to being jammed both intentionally and unintentionally. You really want that happening when you're doing 20+ mph down a bike lane?

If you divert your focus to a device that sends useful info, but not throttle control, to the phone screen, I will buy your device. Make something that plugs into the CAN bus on a VESC and sends me info such as RPMs and speed in kph and mph that can easily be installed and easily be paired with a screen and you'll have a clear winner. Seriously, i'll buy that from you and support your new business. I'll buy 5 or 10 of them. 

bluetooth and wifi have no business being anywhere near throttle control though. Its just dangerous.
```

---
## \#5 Posted by: hugohammarstrom Posted at: 2016-05-16T17:42:34.096Z Reads: 322

```
[quote="longhairedboy, post:4, topic:3348"]
You really want that happening when you're doing 20+ mph down a bike lane?
[/quote]

@longhairedboy I understand what you mean :sweat_smile:. And yes, every wireless connection has the risk of failing unexpectedly. But in all the testing that I´ve done the connection have'nt failed a single time.

[quote="longhairedboy, post:4, topic:3348"]
Make something that plugs into the CAN bus on a VESC
[/quote]


That may be something interesting to investigate more into. The problem is that i don't have a VESC...:yum:
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-05-16T17:50:51.934Z Reads: 302

```
Order one now from ollin board company and you'll have it within two weeks. Or wait until Enertion has them on tap which won't be much longer, they ordered a bajillion of them this time. Or i'll sell you one of mine when i get the five i ordered in February. Or i'll GIVE you one  in exchange for allowing me to test and keep your prototypes and help you get them solid. 

I want a true, non-GPS speedometer on my phone, and i want it yesterday. I started building one with hall sensors and an arduino that would detect the magnets in the motor can and do math to get mph, but i just don't have time for that shit.
```

---
## \#7 Posted by: hugohammarstrom Posted at: 2016-05-16T18:00:19.209Z Reads: 284

```
@longhairedboy So what usable data is avalible thru the CAN bus?
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-05-16T18:42:09.019Z Reads: 281

```
@chaka might be a better person to answer that question. I know there's a ton of info available though. Also there are other ports available as well that maybe could or should be used instead, like the UART. I think my buddy teddy was using that on his crazy ass solar powered 12S rig. He had throttle and readouts on his iPhone, so i know for sure it can be done. I'm not 100% on what he was doing or how though, that's something i just never had time to dive into.
```

---
## \#9 Posted by: JLabs Posted at: 2016-05-16T19:07:58.505Z Reads: 260

```
The posisition of the port would require the device to stand streight up, which is not very conventional. Cool Idea tho, I would reconsider port posisitioning
```

---
## \#10 Posted by: hugohammarstrom Posted at: 2016-05-16T19:15:08.941Z Reads: 262

```
@JLabs The receiver is not intended to sit directly on the VESC, I designed it with the intent of using a servo lead between the receiver and the ESC.
```

---
## \#11 Posted by: paragon Posted at: 2016-05-16T20:51:18.536Z Reads: 249

```
That can easily be fixed with 90 degree pin headers.
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-05-16T20:54:28.223Z Reads: 252

```
You would have to have it tested in various locations...not an advocate for phone control because well...it's your phone...and if you drop it..you could break it ... Also, what if the the app on the phone freezes for some reason...yada yada yada....

Reliability is over time in various locations...may be you send one to the community to test for you...each member that is chosen to test passes your device to the next person...and the last person on the list sends it back to you...so far seems the various group buys have gone without a hitch and so far the community has been outstanding in communication and supportive of new ideas (see Breakboard thread: http://www.electric-skateboard.builders/t/brakeboard-rat-disc-brakes-kickstarter/2873?u=michaelinvegas) Also search @jacobbloy and @Hummie threads on the hub motors they sell...

I think certain members of this community can assist you in finding out if "this" is something that the esk8 community would be interested in....Thats from the guy with a background in marketing and business development... Those are my two cents 🤔
```

---
## \#13 Posted by: hugohammarstrom Posted at: 2016-05-16T21:08:51.250Z Reads: 236

```
@Michaelinvegas Great idea! I would love to do that, I just need to finalize the app and upload it to the App Store. 

**If there's someone that are interested please contact me!**
```

---
## \#14 Posted by: jacobbloy Posted at: 2016-05-17T00:07:08.297Z Reads: 222

```
My app has been submitted for approval on iOS and can do phone control using the nunchuk app so you can have ramping and cruise control if u wanted it and you can use a Bluetooth module that costs only $5
```

---
## \#15 Posted by: Iceni Posted at: 2016-05-17T06:12:02.478Z Reads: 213

```
His module is universal though, sends out a ppm signal.
```

---
## \#16 Posted by: bbq870 Posted at: 2016-05-17T11:34:10.400Z Reads: 203

```
looks cool, but I would put my I Phone in the pocket when riding in order not to drop it.
also I´m not sure about the touchscreen trigger, as it gives me no feedback.
```

---
## \#17 Posted by: hugohammarstrom Posted at: 2016-05-17T12:01:08.308Z Reads: 218

```
@bbq870  Yes, the risk of dropping your phone definitely increases if you use it while skateboarding. 
[quote="bbq870, post:16, topic:3348"]
I´m not sure about the touchscreen trigger, as it gives me no feedback.
[/quote]
If you think about it, you get a feedback in form of the wheels spinning :wink:
```

---
## \#18 Posted by: bbq870 Posted at: 2016-05-17T12:12:21.366Z Reads: 214

```
well, you are right, but I meant more of a "mechanical", sensoric feedback. like you release the trigger and it snaps back in the neutral position and whenever your finger goes for the trigger it feels where it is.
(that kind of feedback I mean)
but maybe its possible for this device to use the vibrating feature?


edit:
maybe you show a video of the app, how it works, then its more clear.

ps: 
does your trigger snap back to neutral if I release the touch?
and how accurate do I need to hit the white square (trigger) or can I just touch ANYWHERE on the screen and push forwards? (that would make it "eyes free")
```

---
## \#19 Posted by: hugohammarstrom Posted at: 2016-05-17T12:28:40.875Z Reads: 214

```
[quote="bbq870, post:18, topic:3348"]
but maybe it's possible for this device to use the vibrating feature?
[/quote]

That is a really good idea!

Yes, the trigger snaps back to neutral when you release the touch, and as an answer to your second question. No, you can't touch anywhere on the screen, you need to touch the white thumb area when starting sliding and then you can touch anywhere on the screen as long as you don't release your finger.

A video is a great idea, will do that as soon as I get some spare time!
```

---
## \#20 Posted by: Johan Posted at: 2016-05-17T14:35:04.193Z Reads: 197

```
I'd be up for testing it, I live in Stockholm and I'm soon done with my first build. And if it's good ill buy one.
```

---
## \#21 Posted by: hugohammarstrom Posted at: 2016-05-17T14:45:56.190Z Reads: 182

```
@bbq870 
https://youtu.be/B0CghF6nhtQ

It's worth noting that the app is in beginner mode, and that's why there is such a big neutral range.
```

---
## \#22 Posted by: hugohammarstrom Posted at: 2016-05-17T14:48:28.354Z Reads: 174

```
@Johan Sounds like a plan! I'll contact you via pm.
```

---
## \#23 Posted by: OskarCastrone Posted at: 2016-05-17T18:21:03.487Z Reads: 167

```
I would like to test it too! It sounds like a interesting new control method :D 
I live in Copenhagen, Denmark.
```

---
## \#24 Posted by: Michaelinvegas Posted at: 2016-05-17T18:34:58.812Z Reads: 161

```
Again...not a big advocate of using your phone ... But if you are....I would suggest something like this for your phone

http://www.lovehandle.com
```

---
## \#25 Posted by: hugohammarstrom Posted at: 2016-05-17T18:38:05.224Z Reads: 161

```
@Michaelinvegas Cool product! Yes, some sort of safety strap maybe should be used for safety.
```

---
## \#26 Posted by: Michaelinvegas Posted at: 2016-05-17T18:43:56.734Z Reads: 164

```
I actually got a sample from them...I have one on my phone...and you know what... I use it every day...it's super handy ... I didn't think it would be... It just sticks on...so you can position it for the most secure grip...or dangle you phone by your pinky lol

But def would suggest getting something like this
```

---
## \#27 Posted by: Blasto Posted at: 2016-05-17T19:15:27.981Z Reads: 161

```
what happens when you receive a phone call or a txt msg while riding and accidental answer, the app goes into the back ground... total loss of control?
```

---
## \#28 Posted by: DilatedPupils Posted at: 2016-05-17T19:21:26.606Z Reads: 161

```
Ouch! SYF and maybe shop for a new phone. :cry:
```

---
## \#29 Posted by: hugohammarstrom Posted at: 2016-05-17T19:24:58.484Z Reads: 170

```
@Blasto When the receiver detects a connection loss it automatically puts the ESC into neutral throttle
```

---
## \#30 Posted by: anorak234 Posted at: 2016-06-22T00:10:59.339Z Reads: 163

```
Love the idea @hugohammarstrom , but even when I saw this type of thing with prebuilt eboards I was skeptical... What happens if you drop your phone? Nevertheless I can always buy a life proof case and I'm currently looking for a better controller than my cheap Quanum. When do you think these might be available in the U.S.?
```

---
## \#31 Posted by: DanButcher Posted at: 2016-11-01T20:09:29.873Z Reads: 116

```
Checkout ESP2866, one chip cost around 3$, arduino compatible. Ready to go server/client firmware on http://www.nodemcu.com/. You can send information through UDP without any delay and apllication can have additional functions. It's almost ready to go chip just need some additional code for tunning. You could controll same receiver with external device or phone at same time, even not your phone. And most important it is Wi-Fi so crowded place is not a problem.
```

---
## \#32 Posted by: Iam319 Posted at: 2017-05-04T17:56:41.858Z Reads: 94

```
How do you do this with your app? I can't find an explanation of how to use nunchuck and HM10 at the same time anywhere.
```

---
## \#33 Posted by: jacobbloy Posted at: 2017-05-04T20:07:20.386Z Reads: 94

```
The only way to do a nunchuck and HM-10 is to have 1 vesc connected to the nunchuck. And the second connected to the HM-10. Setup each vesc with a different application.
```

---
## \#34 Posted by: koosgabor Posted at: 2017-09-20T15:21:23.587Z Reads: 62

```
Hi,
I see something in this product, and I'm about to build a new esk8. I would like to give a chance to this receiver. How can I buy it from you?

Gabe
```

---
## \#35 Posted by: fuzzyspikez Posted at: 2018-02-07T07:41:38.930Z Reads: 42

```
Where can we purchase?
```

---
