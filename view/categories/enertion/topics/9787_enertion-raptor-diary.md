# Enertion Raptor Diary

### Replies: 135 Views: 7151

## \#1 Posted by: Alexander Posted at: 2016-09-18T11:31:54.760Z Reads: 344

```
My new Raptor duel is such a beauty to behold!! It just arrived on Friday (now Sunday) and unfortunately I've had two pretty gnarly falls already which from my layman's perspective I think is due to an issue with this Winning remote cutting in and out (and/or a VESC setting issue). Or that's how it feels like anyhow. I'll be accelerating from a push start and then the forward thrust stops without me moving my thumb back, a moment later it'll reengage at FULL POWER. The first time this happened as I fell back I tried to brake but it didn't do anything and my Raptor shot off under some parked car splitting my carbon fiber - this was on my very first ride! Had to superglue it :'( Check it out:

<img src="/uploads/db1493/original/3X/0/f/0f7f8bce809a218ae97b098c3619a85cb489ab60.jpg" width="690" height="388">

What I have since figured out is that the board accelerates to full throttle when the thumb-stick it only pushed about 15% forwards of its potential travel. I'm hoping this can be fixed by tweaking some VESC settings in the BLDC thingy. Here are a couple screen grabs of the current settings, let me know if you see anything glaringly wrong, any advise is MUCH appreciated!

<img src="/uploads/db1493/original/3X/d/5/d50950d9c5568860a42336166ab4b0716ade9bc3.jpg" width="690" height="387"><img src="/uploads/db1493/original/3X/c/a/ca92758d39ef0b7f0c6740be3b605e184b0b6141.jpg" width="690" height="387"><img src="/uploads/db1493/original/3X/7/6/76c1bc38ebb78caee3b30608782679c7f8029d80.jpg" width="690" height="387"><img src="/uploads/db1493/original/3X/7/4/7453345d710c19aed695926d535a2d67f7021701.jpg" width="690" height="387">
```

---
## \#2 Posted by: Ackmaniac Posted at: 2016-09-18T11:45:09.439Z Reads: 300

```
First thing that i see is that you have the firmware with the bug. So please update the firmware to the latest available file. (the firmware version itself didn't change)

Make sure that you set the value of max current ramp step to 0.0400.
<img src="/uploads/db1493/original/3X/a/a/aa69cc356ec385f915313dc57e8eeda3494c4c35.jpg" width="690" height="366">

If that still didn't help you are a light guy and the acceleration is too much for you then lower the Motor max to maybe 50 or 40. And if the overall power is too much then lower the Battery max to 20 or 15. 
Motor influences the acceleration especially at lower speeds and battery the top power.

The cutouts you have are because of the remote. It looses connection. So it continues with the last speed it could detect from the remote for another second and then it get's a signal again. make sure that your receiver in the board isn't covered or touched by any wires where high currents flow.
```

---
## \#3 Posted by: Alexander Posted at: 2016-09-18T11:47:57.506Z Reads: 284

```
https://youtu.be/bPqXhp_Sjqc
```

---
## \#4 Posted by: Alexander Posted at: 2016-09-18T11:49:26.462Z Reads: 281

```
I don't really have any choice bc there's not so much space. The battery/power cable touches loads of stuff... <img src="/uploads/db1493/original/3X/7/e/7e71a66fd1ba2c6f0ee2544519d6c37112cca653.jpg" width="281" height="500">
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-09-18T11:56:28.286Z Reads: 271

```
If you have the same behavior than in the video then forget it. Because that is without load. So try it again with you on the board. Because it takes only like 70 watts to spin the wheels freely at full speed and 15% throttle with your settings means around 324 watts (60 motor amps max * 0,15 % throttle * 36 nominal voltage = 324 watts)
And that only for a single motor.
```

---
## \#6 Posted by: Alexander Posted at: 2016-09-18T12:07:50.390Z Reads: 262

```
Thank you for all your assistance. I hear what you're saying about load influencing the motors. But regardless of load surely they should only hit top speed when the thumb-stick is pushed all the way forwards no? Shouldn't it be linear regardless of load?
```

---
## \#7 Posted by: Jinra Posted at: 2016-09-18T12:10:43.307Z Reads: 265

```
That's not how current control works. Think of it like a gas pedal on a car. Make sure you fix the max current ramp step. There are a bunch of other people have problems with the winning remote. If i were you, I'd replace it.
```

---
## \#8 Posted by: Alexander Posted at: 2016-09-18T12:11:12.276Z Reads: 261

```
Also how do I go about updating the firmware you first mentioned? I've updated everything else you suggested.
```

---
## \#9 Posted by: Alexander Posted at: 2016-09-18T12:12:03.356Z Reads: 256

```
As soon as Enertion has stock I'm going to order one of their newer remotes. Can see on their site it'll be in soon.
```

---
## \#10 Posted by: Jinra Posted at: 2016-09-18T12:13:57.464Z Reads: 256

```
I wouldn't want to be an early adopter given that it's made by the same company. Get a reliable one like the gt2b and wait for reviews of the nano-x before committing.

To update firmware, download bldc tool and use the firmware folder in there for the source. You can update from within BLDC tool.
```

---
## \#11 Posted by: Alexander Posted at: 2016-09-18T12:14:39.548Z Reads: 252

```
And yes I'm not a heavy guy (60kg soaking wet) but I live in a VERY hilly area.. Got this duel specifically to blast up these steep hills..
```

---
## \#12 Posted by: Ackmaniac Posted at: 2016-09-18T12:16:19.811Z Reads: 254

```
Your described behavior happens in duty cycle moad but current mode is different. Rouphly you set the power from 0 to 2220watts (37volts x 60 motor amps) with the throttle. 
(To all others, (especially devin) i know it is a bit more complicatedbut let's keep it simple here)

Let's compare it to your car. When you are in Idle and push the pedal 50 % it will still ramp up to the rpm limit. Because 50% is enough power to reach that. At least at a carburetor controlled engine.

But just step on the board and try it. When you push the throttle 15% then it will be very different to 100% throttle.
I haven't ridden a raptor but i guess 15% throttle at a start up is fun and 100% throttle at a startup is pain.
```

---
## \#13 Posted by: Alexander Posted at: 2016-09-18T12:21:03.350Z Reads: 254

```
Sorry where do I find the source file to do this firmware update from?

<img src="/uploads/db1493/original/3X/e/f/ef4f700cfdf655b30eeaecd8f06a8e3caf43a0bd.jpg" width="690" height="387">
```

---
## \#14 Posted by: Jinra Posted at: 2016-09-18T12:23:57.919Z Reads: 238

```
http://vesc.net.au

Re download, reinstall, then find it under c:\program files (x86)\BLDC\firmware. Exact location might be different, I'm going off memory
```

---
## \#15 Posted by: Alexander Posted at: 2016-09-18T12:24:25.457Z Reads: 230

```
Also do I need to adjust these settings on both VESCs or doing it on this one does it all?
```

---
## \#16 Posted by: Ackmaniac Posted at: 2016-09-18T12:24:34.763Z Reads: 236

```
Have a look here. And save your motor settings before that. But change the value to 0.0400 before you save it.
And write down the application settings. because after a Firware update the values will be lost.

http://www.electric-skateboard.builders/t/vesc-faq-firmware-bug-pre-august-2016-please-upgrade/8018
```

---
## \#17 Posted by: Alexander Posted at: 2016-09-18T12:41:26.541Z Reads: 223

```
Haha, now you tell me ;) Just did the Firmware update... But they don't seem to be lost... everything's still there thankfully. 

One last question plz @Ackmaniac, do I need to adjust these setting on both VESCs individually or having done it on one will it "tell/control" the other? Bc one is easy to get the lil usb thingy into and one is inaccessible as it's stuck close to the casing.
```

---
## \#18 Posted by: Ackmaniac Posted at: 2016-09-18T13:59:09.898Z Reads: 229

```
You have to do that to both. but you can connect to the second one when you set the dropbox value to 1 which is marked in red and enable Can Fwd. That means you connect to the second via the first one. But i am not sure if you can update the firmware this way. better connect to the second one via usb just to be sure.

<img src="/uploads/db1493/original/3X/5/3/5344a7541b26bcd9aad78f795fc7528817ab2bae.png" width="690" height="394">
```

---
## \#19 Posted by: Alexander Posted at: 2016-09-18T14:35:38.725Z Reads: 226

```
So I just got back from trying out these new settings, to begin with everything was working like a dream, but then... no connection and, WAM! There's definitely a connection issue with my remote. It totally drops connection and then when it comes back it blasts at full throttle and puts me on my ass. Just really hurt my knee!! Probably not able to skate for a week or two now.
```

---
## \#20 Posted by: Alexander Posted at: 2016-09-18T14:47:27.070Z Reads: 229

```
On the plus side I made a new friend as I bumped into @mrjonnyjones on the Brighton seafront right now on his e-skate. We went for about 200m cruise together before this latest issue happened. He even saw my remote lose connection as he was right next to me and then watched as it came back full blast and saw me roll on the floor after badly twisting my knee hopping off. So there's a fellow e-skater who can fully back up my account of what happened. Here's a pic of our boards together  I just took while recovering/preparing for the walk home. <img src="/uploads/db1493/original/3X/5/c/5cb1f28497afcdf64cb7f34c43cb4829dde6e142.jpg" width="690" height="388">
```

---
## \#21 Posted by: Jinra Posted at: 2016-09-18T14:51:58.419Z Reads: 221

```
you need to rebind to reset neutral throttle position. This won't fix the connection issues but won't make your board go full speed when it disconnects. Like I mentioned, the remote is nothing but problems.

http://www.electric-skateboard.builders/t/2-4ghz-nano-remote-in-stock-30-pcs-usa-50-free-priority-shipping-international-45-shipping/5017/191?u=jinra
```

---
## \#22 Posted by: Alexander Posted at: 2016-09-18T15:06:15.599Z Reads: 211

```
Yeah I'm not going out on it with this remote again. In a fair bit of pain lol. Going to order the GT2B and the "GT2B Electric Skateboard Controller Enclosure" so it's not so offensive to look at ;)
```

---
## \#23 Posted by: Ackmaniac Posted at: 2016-09-18T15:08:58.163Z Reads: 218

```
If you want to spent a bit less time and have something that works without modifications then get the mini remote.

https://de.aliexpress.com/item/2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32607181070.html?spm=2114.13010608.0.82.DXpgnp

Don't have one yet but i ordered it and all people are very happy with it.
```

---
## \#24 Posted by: Alexander Posted at: 2016-09-18T15:09:45.495Z Reads: 218

```
Which one is more dependable? Thats all I care about right now really.
```

---
## \#25 Posted by: Ackmaniac Posted at: 2016-09-18T15:13:00.532Z Reads: 210

```
You remember this sentence. Wasn't my intention.

[quote="Ackmaniac, post:12, topic:9787"]
I haven't ridden a raptor but i guess 15% throttle at a start up is fun and 100% throttle at a startup is pain.
[/quote]
```

---
## \#26 Posted by: Spek Posted at: 2016-09-18T16:11:07.837Z Reads: 201

```
I'd be so mad if I recieved a complete board shipped with a known bug that can cause injury. Good luck. 3 days with my gt2b and no issues, highly recommend and the enclosure mI'd was easy
```

---
## \#27 Posted by: Ackmaniac Posted at: 2016-09-18T16:15:12.121Z Reads: 196

```
I guess the gt2b and the mini remote are more or less the same when it comes to reliability.
```

---
## \#28 Posted by: Spek Posted at: 2016-09-18T16:17:35.275Z Reads: 192

```
Yeah it would appear that way
```

---
## \#29 Posted by: Alexander Posted at: 2016-09-18T16:45:54.350Z Reads: 199

```
Getting mad doesn't help anyone dude.. Sure it's disappointing but c'est la vie. Just hope I get a little discount when ordering a replacement Raptor deck. And that I can get either this or another remote working consistently with zero disconnections in the imminent future. I've just been advised by Jason to try re-binding it. Gonna give that a go, but regardless can't test it for few days till my knee's recouped. Probably going to order a GT2B!

Update: just ordered that "mini remote"
```

---
## \#30 Posted by: mrjonnyjones Posted at: 2016-09-18T16:48:18.715Z Reads: 195

```
Great to meet you dude! :smiley:

I was so excited to see a fellow e-sk8er in the wild, haha!  The Raptor is so sick, genuinely an epic board!... I just really hope you can get the remote control issues sorted.  Whilst I was driving home I did have a thought:  For the time being I can't see any reason why you couldn't get hold of the [same remote as I have](https://www.aliexpress.com/item/2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32607181070.html)...  Just to see how you get on with it, then we can ride together again when your knee is better.  We could then see how our boards both behave with the same remote/receiver setup.
```

---
## \#31 Posted by: Alexander Posted at: 2016-09-18T17:17:20.850Z Reads: 206

```
I've JUST ordered one like yours @mrjonnyjones .aka "the mini remote":

"Thank you for your payment!

AliExpress will process verification on your payments authorization within 24 hours. Once the payment pass verification, we will receive your payment and your supplier will start to prepare your order. If the verification failed, you will be notified via email.
Payment Successful: ￡32.58
Order Processing Time: 7 Days"
```

---
## \#32 Posted by: mrjonnyjones Posted at: 2016-09-18T18:22:35.261Z Reads: 209

```
Good lad!  I've had zero issues with the remote.  It's super comfortable and you'll be able to control the board better.
```

---
## \#33 Posted by: Alexander Posted at: 2016-09-18T18:52:45.569Z Reads: 212

```
is there much trigger travel distance between 0/resting and full accelerate? assuming pulling the trigger in like firing a gun is accelerate with this one.. unlike the Winning remote where you push up w/your thumb.. 

And does it have a lead antenna I see in this pic? Hard to tell the way its positioned.. hope so, so the conection is solid! <img src="/uploads/db1493/original/3X/b/3/b36c3ebe29877259049a7d01ab31cb3b6270c574.jpg" width="690" height="388">
```

---
## \#34 Posted by: michaeld33 Posted at: 2016-09-19T02:49:25.187Z Reads: 198

```
I have a bunch of them, much more travel distance than the winning, it's very good. And yes, that is a wire antenna on the receiver.
```

---
## \#35 Posted by: mrjonnyjones Posted at: 2016-09-19T07:09:22.997Z Reads: 192

```
Basically what @michaeld33 said mate :slight_smile:  Decent amount of travel, full throttle is ALL the way back, into the main body almost, braking is very controllable too.
```

---
## \#36 Posted by: FlashNova Posted at: 2016-09-19T08:05:51.596Z Reads: 192

```
Has anybody not had any issues with their raptor? It seems everywhere I go on this forum people are still having problems. Which is bummer, cause i wanted to buy one. I debated on buying a Raptor or Carbon GT for months before going the DIY route. But the Raptor is like $1800 after taxes. I honestly felt ashamed of my homemade board at first, like I couldn't afford a real board. But I'm glad I went DIY, I haven't fallen off of my board once.
```

---
## \#37 Posted by: Photorph Posted at: 2016-09-19T08:09:40.744Z Reads: 187

```
Yea that's true, I am seeing a lot of raptor issues, which is sad.  Even the one I had is having issues, the remote lost sync and despite attempting all methods it won't connect to the board.  Enertion has been responding, but it takes 4 days per reply.  

I think Enertion needs to stop with these winning remote variations.  Just use the most reliable remote out there, which is the GT2b.  They need to up there quality control.  They need to assemble each one to perfection, and make sure all the soldering is done perfectly.  Doing all that will cause them a lot less headache in the long run, and it will make the customer experience better as well.
```

---
## \#38 Posted by: Alexander Posted at: 2016-09-19T10:33:32.769Z Reads: 179

```
Even with my temporary remote issues I would HAPPILY recommend the Raptor bro, especially for anyone who likes extreme sports! This thing is honestly amazing!!! It's a complete rocket, I totally underestimated it's brutishness, it's honestly "not a toy" - it's in a completely different class. I'd say the same thing for say a Koenigsegg, or the Pagani Zonda, whereas something like an M3 or 911 is a toy - if you catch my drift. One demands far greater respect. If you want the most exhilarating complete and an e-skate you wont grow board with, get yourself the Raptor Duel, trust!
```

---
## \#39 Posted by: Photorph Posted at: 2016-09-19T10:42:48.142Z Reads: 179

```
as long as it keeps working it's great! lol.  Sucks that you had the remote issue though, I hope enertion resolves it quickly.
```

---
## \#40 Posted by: Alexander Posted at: 2016-09-19T10:44:10.108Z Reads: 187

```
I completely agree that Enertion needs to FULLY test each Raptor that goes out the door for all known issues, maybe even over a week or something, they definitely need a more stringent quality-control period prior to shipping. Though this is obviously tough when customers like me are emailing non-stop hassling them to ship... so I get it from all perspectives. They are doing a great job with their current resources imo!

Foremost the remote/connection dependability is of paramount importance to both enjoyment and safety. Especially with something as powerful as the Raptor Duel someone could easily get seriously hurt if it's not configured and working as they expect. And yes, having people like me with easily avoidable issues, it eats into their profit margins, so is annoying for all parties.
```

---
## \#41 Posted by: Alexander Posted at: 2016-09-19T10:57:34.172Z Reads: 177

```
Enertion have kindly offered to send me one of their new nano-x remotes free of any charge. Though I'd already decided to go with and ordered "the mini" remote as it's been tried and tested by this community with great feedback, and it has an antenna, so I'm confident it will resolve my connection problem. There's really not too much for Enertion to do with my case, other than helping me with settings and such, and they're very fast at responding to my emails. Jason even responded to one on Sunday... I honestly cannot fault their customer service in any way. I'm just hoping they give me a "VIP club" discount on a replacement Raptor deck outer casing when I decide to swap mine out. This damaged carbon fiber is giving me bad dreams lol It's soo beautiful but this ghastly ding is killing me :unamused:
```

---
## \#42 Posted by: FlashNova Posted at: 2016-09-19T10:57:50.453Z Reads: 179

```
I say just get a GT2B and call it a day. They are super reliable and only cost $30 on amazon. It would be much faster and less of a hassle than trying to get Enertion to replace your remote.
```

---
## \#43 Posted by: Alexander Posted at: 2016-09-19T10:59:00.598Z Reads: 189

```
Already ordered "the mini" remote yesterday... 

This one: https://de.aliexpress.com/item/2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32607181070.html?spm=2114.13010608.0.82.DXpgnp8

"Status:
The seller has shipped your order
Reminder:
Your order should arrive within 7-15 Days," :)
```

---
## \#44 Posted by: Alexander Posted at: 2016-09-19T11:40:37.891Z Reads: 185

```
Just had an interesting idea: I think I'm gonna try attaching "the mini" remote's receiver to the underside of my Raptor's lid, then drill a small hole to thread this antenna through and have it secured under the grip-tape... this way connection should be SOLID. (n yes I understand when removing the lid in future I'll need to be careful and unplug the receiver cable to fully remove it, tho once set up right I don't see why I would ever need to remove it..)
```

---
## \#45 Posted by: onloop Posted at: 2016-09-19T11:51:34.514Z Reads: 188

```
[quote="FlashNova, post:36, topic:9787"]
Has anybody not had any issues with their raptor?
[/quote]

Plenty of people have working raptors. It just most people decide to talk about it publicly on the forums if they have a fault, if there is no fault they don't say much.

We have sold just under 150 raptors since November 2015. As a small business running out of a garage in Australia we are very grateful for support of our customers. I think people can see that we are working hard to to build the best eboard in the market and that's why people across the globe have chosen to support us.

There were definitely some teething problems in the first batch. There were some motors that had excess wires inside which eventually rub together due to vibrations. There were some raptors that had carbon fiber lids replaced with new (free of charge) lids that didn't block rf signals. There have been some other random issues too. But that is normal for a product like this. Even if we spent a week testing each one problems can still occur once the product is being used. 

To give some perspective, Evolve has issues, boosted too, marbel has tons of issues.... I don't think there is one brand without a report of a fault.

What is most important is warranty. We offer 12 months instant replacement on anything faulty. We also have repair agents in Europe and US.  

We will also be offering special upgrade options to the first 150 raptor customers, this is very important as we are a very agile business that is constantly developing and innovating and we don't want to leave our customers behind. 

So if you like industry leading warranties, industry leading top speed, free world wide shipping, modular design to make maintanence easy, latest technology upgrades at massively discounted prices.... the raptor might be a good choice.
```

---
## \#46 Posted by: mrjonnyjones Posted at: 2016-09-19T13:25:00.145Z Reads: 172

```
Fair play to you Jason (and staff), I was so stoked to see @Alexander's Raptor in the flesh on Sunday, mean machine.  Motors sounded awesome and the whole package is brilliant.  I think it's just one of those things, technology and innovations sometimes come with problems... but it's good to know you're on top of things when issues arise.
```

---
## \#47 Posted by: treenutter Posted at: 2016-09-19T13:39:48.113Z Reads: 174

```
@Alexander I agree w this! GT2B is currently the most reliable and robust. Rechargable battery and field-tested. I went through 3 different remotes before I finally bought a GT2B and I've never had a dropout since I switched.

[quote="FlashNova, post:42, topic:9787"]
I say just get a GT2B and call it a day.
[/quote]
```

---
## \#48 Posted by: Alexander Posted at: 2016-09-19T13:43:05.637Z Reads: 175

```
That is SO TRUE! and we as a community often overlook this fact. Of all the big fully-financed companies producing e-skates right now, the one I and many others have chosen (for good reason) is the Enertion Raptor, that's made in some dude's garage with like 4 employees, n a dog.. :) I think that's quite a feat just in itself and worth mentioning again. Serious props J!! Your dedication and passion for what you've created is very evident and I for one will do all I can to support Enertion's continued success. I don't drink anymore but if I did I'd cheers to that!
```

---
## \#49 Posted by: Alexander Posted at: 2016-09-19T13:48:38.641Z Reads: 177

```
More so than "the mini"? Is there anyway to compare their safety/connection records? A few people above said they are identical in this aspect... So I've already ordered "the mini". How do their internals differ? Because their receivers looks similar and they both have antennas. Which seems like a very necessary component..
```

---
## \#50 Posted by: treenutter Posted at: 2016-09-19T14:13:17.528Z Reads: 175

```
Sorry @Alexander I hadn't read the whole thread to see that you bought the mini... the mini is good, I have one and it doesn't drop. GT2B has a rechargeable battery and more configurable features, but the mini does a good job. Side-by-side, GT2B is has a higher build quality in my view, and is meant for more advanced RC usage, which is probably why it is so reliable for esk8.
```

---
## \#51 Posted by: flatsp0t Posted at: 2016-09-19T15:15:34.221Z Reads: 182

```
I have about 1000 miles on each of them, and no drop outs so far.
So , just go with what you like more...

Edit:
The gt2b is too large, so you would need to mod it.
The mini is much more comfortable in that way.
```

---
## \#52 Posted by: Alexander Posted at: 2016-09-19T16:45:54.447Z Reads: 184

```
Thanks brother. That was my deciding factor funnily, so I've ordered the mini. Following it on DHL tracking currently. Will probably still have a few questions tho when it comes time to install and set it up I'm sure.
```

---
## \#53 Posted by: Alexander Posted at: 2016-09-20T08:51:40.568Z Reads: 156

```
So my "mini" remote system coming from Hong Kong is taking foreeeverrrr to arrive, yes I know I only ordered it yesterday but I can see they now need 7 days before even giving it to DHL for some ungodly reason, SO, in the meanwhile I've just ordered a GT2B via Amazon that arrives tomorrow, holla at ur Raptor :) I'm so not a patent dude, really need to work on that lol
```

---
## \#54 Posted by: Ackmaniac Posted at: 2016-09-20T11:39:31.475Z Reads: 150

```
My mini came after a week. I order a lot via aliexpress and normally it needs 3 weeks but this one came by express with free shipping.
```

---
## \#55 Posted by: Alexander Posted at: 2016-09-21T06:50:27.271Z Reads: 153

```
[quote="Ackmaniac, post:16, topic:9787"]
save your motor settings before that. But change the value to 0.0400 before you save it.And write down the application settings. because after a Firware update the values will be lost.
[/quote]

Is there a difference between "motor settings" and "application settings" because when I did the Firmware update on the Master VESC all my motor settings remained... (just curious if I've missed something).
```

---
## \#56 Posted by: Alexander Posted at: 2016-09-21T06:58:36.957Z Reads: 157

```
I think you were very lucky in that instance bro, my mini's DHL tracking info still says "Shipment information received", not even package* received. So DHL in HK haven't even began processing it through their system yet. For all I know dude is in his sweatshop cranking out mine/more as we speak lol. Regardless today I got that first-cellphone-ever lookin remote coming :) (TR3B or whatever its called) So can get on with some long overdue playing.
```

---
## \#57 Posted by: Alexander Posted at: 2016-09-21T18:33:25.382Z Reads: 153

```
***YAYYY SUCCESS*** [insert happy dance] ***!!*** Just came back from my first proper ride with no connection issues or problems whatsoever, she worked like a dream!! This Raptor is **so** much fun!! I imagine many electric skateboards give you a similar feeling, reminiscent to snowboarding in many ways, but being able to blast up steep hills is absolutely incredible. LOVE THIS RAPTOR!! Totally going make a video of me blasting up some gnarly hills in the coming days,
```

---
## \#58 Posted by: Alexander Posted at: 2016-09-24T16:45:29.399Z Reads: 161

```
**(Day 3) Raptor Report:**

I F&%KING *LOVE* THIS THING!!! Just WOW!! The Raptor Duel is a caged *beast* just waiting to be unleashed.

If you're a fairly light guy like me (60kg fully clothed) there's absolutely no way you'll need to ride this thing on max settings and that in itself is a BEAUTIFUL thing. Instead of having to cane the shit out your board and it's components to achieve an exhilarating cruising-about speed, you just have to give it maybe 50% of the Raptors potential and you'll be FLYING!! Even up the steepest/longest hills. Where I live it's seriously hilly and this thing just laughs at them, like *"is that all?!"* lol. Plus the noise these two motors make sound like a fighter jet taking off, in every way this has exceeded my expectations, dramatically! 

I took it up to London yesterday on the train and rode it like one would a motorbike through the city, such fun!! Totally kept up with the flow of traffic, no slower than any of the pizza delivery scooters. London is definitely an e-skate friendly city. Everyone was super nice and amazed at what the Raptor was capable of.

Cruising through Knightsbridge on my way into Hyde Park there were the typical incredibly wealthy young middle-easterners driving about in their super/hyper-cars, yet many were more interested, at least in that moment, in the Enertion Raptor :) I wouldn't be surprised if those last few VIP Club places were taken by customers from London now, at all. Had I been wearing an Enertion T-Shirt I'm sure Jason would be inundated with new Raptor orders (@onloop , that's not a bad idea actually, get promo/PR street teams Raptering through cities wearing Enertion garb, asap!!).

I raised my Motor Max and Battery Max BLDC settings slightly today. 40 and 20 respectively - Now she's perfect!! Her name's Sammy btw ;) Lots of video's to follow in the coming days. Guess I'll just add to this thread whenever I post. One love all
```

---
## \#59 Posted by: rodriguejoe1 Posted at: 2016-09-24T19:18:59.857Z Reads: 152

```
[quote="Alexander, post:58, topic:9787"]
Her name's Sammy btw
[/quote]

Please don't tell us she goes to bed with you...:heart_eyes:
```

---
## \#60 Posted by: Alexander Posted at: 2016-09-24T19:25:33.521Z Reads: 147

```
Haha she is pretty god damn sexy ;) Named in the same vein you'd name a yacht though.
```

---
## \#61 Posted by: Cloud_Gnash Posted at: 2016-09-24T20:56:38.716Z Reads: 141

```
Youre making me more and more jealous for mine to arrive. Glad youre enjoying it! And cant wait to see the videos. Youre using the HK GTB2 for now right? No drop outs anymore? Im sure youre turning some heads around london on that thing...and i'm definitely going to want and copy your settings
```

---
## \#62 Posted by: Alexander Posted at: 2016-09-24T23:01:32.018Z Reads: 140

```
Yeah exactly, ever since I installed the GT2B she's been a dream to ride, now that it consistently responds as I expect. The connection's about 99% perfect to be totally honest, the signal does drop out very occasionally, but its instantly reconnected each time so far without any fanfare. Having the correct Firmware certainty helps I'm sure also. Plus the GT2B has two lights on it, a red one that signals its turned on and a green one that signals a solid connection, so it's easy to see. I have "the mini" remote arriving on Monday and I'm in two minds about even using it.. Certainly in no rush for the time being.

edit: Got my GT2B via Amazon (.co.uk) next day delivery. It's "the mini" remote that I ordered from HK (Hong Kong), DHL tell me it's arriving Monday.
```

---
## \#63 Posted by: Lebram Posted at: 2016-09-25T07:43:05.297Z Reads: 137

```
[quote="Alexander, post:62, topic:9787"]
GT2B
[/quote]


why such a big remote ?

i thought it came with a different smaller remote?
```

---
## \#64 Posted by: Alexander Posted at: 2016-09-25T09:05:48.828Z Reads: 144

```
The "Winning" remote which it came with was not working as it should, it was disconnecting and reconnecting pretty frequently. Alone not such a big issue but this was compounded by the fact, unbeknownst to me at the time, my VESC had the buggy Firmware which makes incremental acceleration steps with 1000x more power than recommended ("40" rather than "0.040" in the settings), which put me on my ass 3 or 4 times before I figured out what was going on. As I was understandably wary about trusting the Winning remote again I opted to go with the remote with the best track record I could find (w/fast delivery) - the GT2B. Enertion have kindly offered to send me a free new nano-x remote when their new stocks arrives. Though if it lacks an antenna (and/or is made by the same Winning remote/receiver company) I'll be hesitant to install it, at least until it's been comprehensively tested by the community. Also I'm now a fan of the lights on the GT2B, I like having the visual conformation that I've got a solid connection. As I say this "mini remote" I ordered from Hong Kong is arriving tomorrow according to DHL but I'm not sure I'll even bother with it. Not right away anyhow. Very pleased how Sammy is performing atm and don't wanna mess her up unnecessarily ya-know.

Also this large remote in my hand if often the thing people see first that makes them realise I'm on an electric board. I think there's some safety in this aspect because they then anticipate me to act somewhat differently to a traditional skateboard/longboard. There's functionality plus's and aesthetic negatives to having such a big remote. But I know what's important to me now..
```

---
## \#65 Posted by: Alexander Posted at: 2016-09-25T09:23:18.400Z Reads: 133

```
@mrjonnyjones you still coming down to the beach today dude?

Anyone else in the UK that wants to come for a cruise down by Brighton Beach is also most welcome to join!! Gonna make this a Sunday event each weekend (we get nice weather) from now on.
```

---
## \#66 Posted by: mrjonnyjones Posted at: 2016-09-25T09:38:40.490Z Reads: 135

```
I REALLY wanted to dude, however I've had a load of work come in that needs my immediate attention, totally down for next Sunday though! :smiley:  Have fun if you venture out today!

EDIT:  Epic idea regarding making this a weekly thing, motivation to get projects finished and for people to (potentially) travel to ride along the sea front!
```

---
## \#67 Posted by: Cloud_Gnash Posted at: 2016-09-29T20:07:06.898Z Reads: 133

```
Where are these mythical videos?! Would definitely help those of us waiting for our raptors to arrive. Cheers!
```

---
## \#68 Posted by: Dedbny Posted at: 2016-09-29T22:18:18.013Z Reads: 131

```
PGlad you had a solution that gives you surety in rider safety. The issue with the shipped remote was a problem and you were lucky not to seriously injure yourself more if the erratic acceleration. I hope others arent having the same problem Batch 4. By now the remotes should have been sorted, but understand Enertion were looking for a small remote, but reliable connection is probably more important. So GTB2 looks ungly but works.

Post some vids. When you can.
```

---
## \#69 Posted by: Alexander Posted at: 2016-09-30T16:37:04.935Z Reads: 133

```
So the weather's been pretty shitty here the past week, any runs I've done have been short and sweet. Just hasn't been "nice out" / filming weather, plus I'm moving house. Don't stress dude, video's to follow 100% (when we get some more sun).

Using the GT2B has been painless so far, it's internals seem solid. But I need to configure it more, basically everything works great other than I have to move the trigger maybe 15% before it bites. Like there's some dead space in the start of the throttles travel movement. I think this can be tweaked but I forget how.. ?
```

---
## \#70 Posted by: Blasto Posted at: 2016-09-30T16:56:25.165Z Reads: 133

```
[quote="Alexander, post:69, topic:9787"]
there's some dead space in the start of the throttles travel movement. I think this can be tweaked but I forget how.. ?
[/quote]

make sure your signal is well centered and then you can tweek your deadband
<img src="/uploads/db1493/original/3X/1/b/1b9268175766776f6a08bed28edb6a68f780acd7.png" width="161" height="77">
```

---
## \#71 Posted by: Alexander Posted at: 2016-09-30T17:17:24.754Z Reads: 122

```
I did this but still had the dead space..

ps: what did you mean by "make sure your signal is well centered"?
```

---
## \#72 Posted by: Blasto Posted at: 2016-09-30T17:21:44.125Z Reads: 122

```
your min and max settings, 

put the PPM disable, write, tick the display, squeeze full throttle, take note of the value, squeeze full brake , take note of the value.

enter those values in the min max, enable your ppm "current no reverse with brake", write
```

---
## \#73 Posted by: Alexander Posted at: 2016-09-30T17:22:19.292Z Reads: 128

```
Thank you!!!
```

---
## \#74 Posted by: Blasto Posted at: 2016-09-30T17:25:17.813Z Reads: 127

```
it's also worth noting your neutral value, the vesc calculates the neutral value (MIN+MAX)/2 , just make sure your values are balanced, this way you can reduce your deadband
```

---
## \#75 Posted by: Alexander Posted at: 2016-10-02T09:17:42.688Z Reads: 130

```
Another Sunday group ride in along the Brighton seafront and surrounding area. So far it's just @mrjonnyjones and myself I believe but ANYONE is welcome to join - So long as you can keep up :)

The weather forecast this afternoon is full SUN

Victoria - Brighton is only 55 mins on the train for all our London eSk8ers.. Common down! 

One Love


ps: @Blasto I fixed that deadband issue, thank you!
```

---
## \#76 Posted by: mrjonnyjones Posted at: 2016-10-02T12:45:44.440Z Reads: 123

```
A few issues with @Alexander's board this afternoon...

 https://youtu.be/lr25Y5RiPd4
```

---
## \#77 Posted by: spottyjohn Posted at: 2016-10-02T14:59:57.011Z Reads: 128

```
I In the R/C aircraft world you must NEVER have the TX off whilst the RX is powered.
Reason being is just what you're experiencing here,- the vehicle bursting into life due to other signals/phones for example.
Looking at what was happening before the TX was switched off I'd say the TX was loosing contact with RX perhaps low battery in TX? Either way the ESC must be configured to cut power when signal is lost and perhaps configure 'soft start' to prevent all your problems at the beginning of this thread.
Perhaps take a look at an RC instruction manual (Futaba or Spektrum) to get an idea of how/what/why they all work.
I don't know either of the TX's you've been using but the 'proper' (expensive) r/c TX's all have what's known as 'expo' to slow/soften the stick/triggers response around the neutral position. I've moved from London Last year to the Badlands of Oxfordshire but if you could bear spending time with a fossil I'd be up for a day in Brighton. I'm holding it down in Bournemouth today 😀.
I've got a V1.
```

---
## \#78 Posted by: mrjonnyjones Posted at: 2016-10-02T18:20:37.103Z Reads: 123

```
You make some interesting points, we didn't swap batteries in the GT2B. We did swap out the GT2B and installed the Mini remote and receiver and it seemed to work well. Few little bugs still but I'll let @Alexander fill you in :slight_smile:
```

---
## \#79 Posted by: chinzw Posted at: 2016-10-02T19:18:19.124Z Reads: 129

```
The motors spining when the remote is off is the failsafe not being properly set up.
The other issue when moving the remote is the deadband is too small to any little change in resistance makes the motors spin.
They're pretty basic things that anyone getting into DIY esk8s should know.
```

---
## \#80 Posted by: Alexander Posted at: 2016-10-03T07:48:09.596Z Reads: 134

```
That's good to know, many thanks!! I may actually go back to the GT2B as I preferred it's trigger motion. The other thing that troubles me, is that at "high speeds" there reaches a point where I hit this turbo or "power-band" as it used to be called on my motocross bike. Basically once I'm at about 20mph my acceleration is no longer linear, I get this sudden JOLT of force, this sent me flying yesterday after we parted ways @mrjonnyjones unfortunately. My Bern helmet can't arrive soon enough now, though it was my hip that took the impact, bloody painful. No more skating (or walking more than 50 yards lol) for few days now.

@chinzw, so you're saying to increase the deadband (from 0 to what approx) to resolve that remote issue? I found that on my BLDC tool I couldn't get the deadband to go higher than "1"... it seemed locked in place kinda. 

Then also how does one set up the failsafe properly so than if/when the remote turns off or runs out of batteries all that happens is that I coast to a stop (/no sudden braking or acceleration)?
```

---
## \#81 Posted by: Alexander Posted at: 2016-10-03T08:08:48.954Z Reads: 130

```
Dude totally come on down to Brighton!! You really seem to know what you're talking about :) Would love some assistance getting this thing perfectly configured to my weight/environment etc. Lunch/pizza on me!!

You mentioned "soft start" as a possible solution to sudden jolt acceleration (although now this isn't a problem as the "max current ramp step" bug issue has been resolved): 

A) How do I best configure this soft start?

B) Is this or something similar able to prevent the "power boost" I get once the motors reach optimum efficiency at around 20mph? (I think that's why its happening anyway).

Also I don't mind spending money on a proper/expensive remote that has all the bells n whistles, is there one you recommend?
```

---
## \#82 Posted by: mrjonnyjones Posted at: 2016-10-03T13:14:06.547Z Reads: 124

```
Ah dude, that sucks you went flying again, NEED to get this board sorted... it's badass but has a sting to it at the moment ;-)
```

---
## \#83 Posted by: chinzw Posted at: 2016-10-03T16:46:44.978Z Reads: 129

```
The deadband is in "ms" so a value of 1 would be the whole range of the throttle pretty much since they usually go from 1ms to 2ms. In the BLDC tool when you set Display on, set the deadband to about 0.25 and press the throttle very gently, there should be quite a bit of movement before the motor actually reacts.
As for the failsafe just leave the remote in neutral and use the included plastic pin to press and hold the failsafe button on the receiver, it should blink a few times when its set. Once you do that, go full throttle (with the board upside down ofc!) and turn off the remote, it should coast to a stop.
```

---
## \#84 Posted by: Alexander Posted at: 2016-10-04T12:51:40.599Z Reads: 130

```
Cheers dude!! That makes sense. All set up now. I've just reinstalled the GT2B as I prefer it's trigger travel plus it's rechargeable.

Also marginally lowered my motor max and battery max to 42 and 22 respectively in BLDC. Hoping this is right for my weight now. 45 and 25 was too powerful and 40 and 20 was "not enough".. fingers crossed!
```

---
## \#85 Posted by: Alexander Posted at: 2016-10-04T14:37:15.726Z Reads: 125

```
I wanted to say a ***BIG*** **THANK YOU** to Jason and the Enertion fam (@EnertionSupport & @onloop) for sending me a replacement Raptor shell which arrived today. 

I can now verify first-hand the Raptor's warranty and associated customer service is really up there. A faulty initial setup caused a little raptor damage and they have instantly sent me a replacement no questions asked, didn't even charge me shipping!!! **BEST** E-SK8 WARRANTY!!!
```

---
## \#86 Posted by: Cloud_Gnash Posted at: 2016-10-04T17:15:18.488Z Reads: 120

```
I'd be interested to hear if the 42/22 works better for you, and if you ever figure out how to tame that second 'boost' after 20 mph. As a slightly heavier guy than you (~85kg) i think i may go with the 45/25 setting. Does this mainly effect the top speed or acceleration? Glad to hear you got a new shell, the Raptor is too sexy to have damage like you did on day 1.
```

---
## \#87 Posted by: Alexander Posted at: 2016-10-04T17:31:14.668Z Reads: 122

```
So I actually lowered those two settings specifically in order to lessen the jolt when I hit that 'boost', otherwise she was absolutely fine. Better than fine even! When I hit the 'boost' before (at 40/20) it wasn't powerful enough to really put me off balance, although it was a nasty shock, whereas with 45/25 it did. At 85kg I think 45/25 will be perfect for you @Cloud_Gnash . 

Yeah completely stoked Enertion sent me this replacement shell, really pleased I chose to go with the Raptor/Enertion!! As I said on one other thread, this is the first time I've ever felt that I've under paid for a product, like it's "worth" so much more than I paid. This is frequently how I feel riding it, and that's something I've literally never felt about any other product I've bought.
```

---
## \#88 Posted by: Cloud_Gnash Posted at: 2016-10-04T18:07:40.165Z Reads: 115

```
Did enertion give you a shipping confirmation when it was sent? Trying to figure out if my board is in this shipment or the oct 10 one.

Thanks, and glad youre enjoying it!
```

---
## \#89 Posted by: Alexander Posted at: 2016-10-04T18:20:23.203Z Reads: 114

```
Yeah Enertion always email when an item is shipped which includes a link to the relevant tracking stuff. 

You'll have yours soon dude I'm sure. It's totally worth the wait!
```

---
## \#90 Posted by: VirtuallyChris Posted at: 2016-10-05T03:35:15.949Z Reads: 115

```
Not sure if you know this or not, but I know I'm in the "After September 30th" Batch, so does this mean that they will have shipped my batch out by October 10th since that's when the next batch begins? There could be no coloration with the batch start vs next batch start date, but I was just curious if anyone knows :open_mouth:

Either way I'm super excited and I know for sure it'll be worth the wait! I'll be doing lots of YouTube videos on it when I receive it, that's for sure.
```

---
## \#91 Posted by: Alexander Posted at: 2016-10-05T06:23:27.158Z Reads: 119

```
All I know for-sure is they get built, tested and shipped in batches of 20. If you follow Enertion on Instagram (https://www.instagram.com/enertionboards/) you can often see them building Raptors and sometimes this helps get a feel for shipping times (it did on my order). Just hang tight bro, it'll be with you soon no doubt.
```

---
## \#92 Posted by: Alexander Posted at: 2016-10-07T06:25:58.381Z Reads: 121

```
Of all the luck in the world... I now have a faulty GT2B remote lol (these remotes really seem to be the weak link in the chain). It's like it has a loose connection or something where it's as-if you've flicked the power switch off and on again, it looses all power and then comes back depending if I wiggle/move my hand (and yes its fully charged). SO.. I've just found and ordered a Sanwa MX-V remote which looks perfect, as in their words "Two are better than one! This is why the MX-V has been equipped with an additional RX-37W receiver." This is what I was talking about in my comment on the Raptor 2.0 thread, about having a back-up channel. Will report back on it's reliability and usability. Forth time's a charm ;) 

Here's where I found it cheapest: http://www.modelsport.co.uk/sanwa-mx-v-with-waterproof-receiver-set-rx-37w/rc-car-products/395264
```

---
## \#93 Posted by: Cloud_Gnash Posted at: 2016-10-07T18:32:42.194Z Reads: 115

```
Hope this one works out for you...i think I'm just going to try my luck with the Winning(with full safety gear) until the Nano-X is ready
```

---
## \#94 Posted by: DWiskow Posted at: 2016-10-08T19:09:41.121Z Reads: 120

```
I have experienced a similar problem on an eMTB I built with Dual MAX6 ESCs, twin SK3 6374 motors and 6s 16,000mAh battery . . . **_my solution was to develop a small board/firmware that I have placed in between my receiver and the ESCs to 'manage' the PWM signal._**

Effectively, when the remote PWM signal is increased, my board/firmware ramps up the speed to that requested in a series of smaller steps over time (i.e an acceleration curve). This means that, even if you slam your remote to full from neutral, the acceleration is 'managed' so that you have a smooth (and safe) increase rather an immediate leap/'jerk' to the higher speed/power. In a similar manner when the brake is applied, this too is deployed in a smooth (and safe) way.

When there is a loss of signal from the remote, my board/firmware sees this as a sudden and massive reduction that is then managed to effect a smooth deceleration to a stop. Should the remote suddenly cut back in, rather than causing a 'jerk' that throws the rider off, the my board/firmware transitions this into to a smooth acceleration and increase in speed.

Since I  built my board/firmware into my eMTB, I have experienced no issues of the type you describe and **_I now enjoy a relaxed riding experience as smooth as butter_** . . . effectively, I have 'tamed the monster' to a degree that my children can now ride the eMTB smoothly and easily.
```

---
## \#95 Posted by: chinzw Posted at: 2016-10-12T00:54:00.093Z Reads: 109

```
Any chance you'd want to share schematics/code for this?
```

---
## \#96 Posted by: Alexander Posted at: 2016-10-31T10:58:30.614Z Reads: 106

```
Well I think it's time for another update:

THIS. THING. IS. AMAZING. 

With each new mile I log my confidence grows, accelerating faster and carving harder. My love for Sammy is now a very real thing at this point - She's just incredible!! Such brute force yet once you're familiar also very delicate and sensitive. Popping out to the shops has honestly never been so enjoyable :) Also that "boost" I kept referring too was actually the beginning of the real acceleration. It's like there's 2 gears, a "slow" one that takes you up to about 18mph, then you hit this power-band and WAM, you better be leaning forwards as she takes off lol But what fun.

Now I'm more confident I shall be making a few videos. Long overdue but on the way. Watch this space..
```

---
## \#97 Posted by: Cloud_Gnash Posted at: 2016-10-31T15:22:31.175Z Reads: 101

```
I have to agree with the reviewer that said "Its the most fun you can have with your clothes on". The Raptor is amazing. On my first 5 or 6 rides I've kept the Motor Max at 40 and Batt max at 22 and Its a thrill. Like you, I'm gaining confidence and finding my exact stance the more miles I log. I've been throwing some pretty decent hills at it and I just zoom up at what I would estimate is around 20 mph. I just turn the VESCS up to 45/25 and will do some experimenting this week. 

My right motor was ever so slightly mis-aligned so I took an allen wrench to it and shifted it over. Realized that thread locking the motor mounts is absolutely necessary due to the vibrations at >20 MPH, as it came loose a few times. Should by all set with the threadlock now. 

A strange thing I've encountered is one motor inexplicably stopping working. I dont think it's ever happened while riding, but when tuning and engaging the motors without a load it has happened a few times. After about 10 seconds the second motor will turn back on like nothing happened. Pretty strange
```

---
## \#98 Posted by: Nate Posted at: 2016-10-31T16:37:06.143Z Reads: 102

```
Hey dude, did your Raptor come with a handle bar?
```

---
## \#99 Posted by: Alexander Posted at: 2016-10-31T18:21:11.549Z Reads: 105

```
If you're talking about the carry handle then yes. I got a silver one. Though it's not what I'd describe as comfy to use, it slices into my fingers anytime I use it for more than a few seconds, it forces me to keep swapping hands otherwise. Been meaning to buy some black tennis handle wrap to try n soften its edges, gonna do that now :) One love
```

---
## \#100 Posted by: themegak Posted at: 2016-10-31T20:02:30.155Z Reads: 101

```
i would pay good money for that board.  any way you could sell me one ?  I've been using a winning remote for a little while now and haven't had any issues but am afraid i'm due for an issue at some point.  Having your board would greatly ease my riding experience.
```

---
## \#101 Posted by: magnetvox Posted at: 2016-11-01T04:22:07.116Z Reads: 97

```
I think you might be the nicest guy on this forum. I like the way your balance views on some of the set backs you suffered ultimately resulted in positive outcomes (especially with the vendor). The forum could use more of that logic sometimes (both ways, between vendors and customers).
```

---
## \#102 Posted by: Dedbny Posted at: 2016-11-01T05:51:50.428Z Reads: 94

```
New cutom handle coming. Timo is working on one. He will post as soon as he can redo a set after his hols.
```

---
## \#103 Posted by: Nate Posted at: 2016-11-01T07:49:23.809Z Reads: 99

```
Ya but having them is more useful than it sounds. The grip tape on my Raptor keep scratching my suits and pants when I'm carrying it so having handles would be helpful. Thanks dude, stay safe out there! 

Hey @onloop can you comment on what the status is for customer who never receive the handles with their Raptors? This is the 6 or 7th times I've ask this questions without a definitive answer.
```

---
## \#104 Posted by: onloop Posted at: 2016-11-01T07:54:42.026Z Reads: 101

```
Email will@enertionboards.com and he will send one out.
```

---
## \#105 Posted by: Alexander Posted at: 2016-11-06T08:49:36.841Z Reads: 99

```
So riding home last night about half mile from my house Sammy died :sob: I thought it was peculiar because I usually got home with about 35%+ still in the tank/battery, and I hadn't rode any further than previous days. The first thing I did was plug it in, but the light on the charger didn't go red. Next I checked the fuse, not blown but I swapped it out just to be safe. Then I thought if this is the first time it's gone ALL the way to 0% maybe it needs some time, so I left it overnight. This morning, still at 0%.... 

It's getting much colder here now, don't know if that played any part. I was on a flat and doing about 25mph at the time. Thankfully she just coasted to a stop, and pushing was actually easier than I thought it would be.

Edit: now that I think about it this has actually been somewhat gradual. Starting about 10 days ago I noticed in the morning the battery was not at 100% (after charging all night) but rather 95 or 98%, very close, but wasn't making it to 100% regardless of length of charging time. I assumed this was not a biggie but now I think it may have been a warning sign that this was about to happen. 

Here's a lil video of her (@onloop & @EnertionSupport): 

https://www.youtube.com/watch?v=NY7n5dHtLSY
```

---
## \#106 Posted by: Dedbny Posted at: 2016-11-06T09:49:41.929Z Reads: 97

```
That is really weird. Something must be wrong with the battery if you changed the fuse. Assume the chargers fine. The screen does show 0%, but maybe theres a little there left for thats to work. Go to Enertion support. You should get a response back next week. It is Sunday here at the moment,
```

---
## \#107 Posted by: ddoke25 Posted at: 2016-11-07T19:40:30.070Z Reads: 97

```
Same issue here. Still able to charge it but wont get above 90% with a total range of 6 miles.  Going to send mine in this week to support.  Haven't had it as bad as you where it won't charge at all but I feel like it may be headed that direction... 
Hopefully they can work some magic and bring both of our power packs back to life! It's going to be a bummer having to push for while but I am counting on Enertion to pull through on this one and to get us back on the road.
```

---
## \#108 Posted by: Cloud_Gnash Posted at: 2016-11-07T22:53:58.715Z Reads: 96

```
The exact same thing just happened to my battery...wont change past 90% anymore
```

---
## \#109 Posted by: Dedbny Posted at: 2016-11-08T02:42:43.290Z Reads: 99

```
I think you guys are in batch 4. Mine is fine. No issues with charging or the switch issues that some had with the push button batch 1.

Wonder whether there was a change made to the bms or battery cells.  Are you  guys using standard or fast charger.  Ive used both no probs.
```

---
## \#110 Posted by: Nate Posted at: 2016-11-08T02:44:04.998Z Reads: 96

```
Could be weather related also. Everyone here living in cooler region now right?
```

---
## \#111 Posted by: Dedbny Posted at: 2016-11-08T08:30:06.584Z Reads: 94

```
But would that be the reason why it isnt charging. I would have thought colder temperature would just mean quicker loss of power.
```

---
## \#112 Posted by: Nate Posted at: 2016-11-08T09:30:46.031Z Reads: 92

```
Possible. Even on my iPhone I had a hard time charging it last winter. Probably has to do with some of the changes Enertion made to the battery system. Just had a new space cell installed on my Raptor and the thing switched to voltage instead of showing percentage after I charged up to 90%.
```

---
## \#113 Posted by: ddoke25 Posted at: 2016-11-08T19:18:48.457Z Reads: 94

```
I have and use both chargers (fast charger at home and standard when I am on the move) and I live in CA, it never really gets cold here.  I'm still riding with a t shirt.

Still operational but can't really go anywhere without charging it after ~20min of riding time. ~ 6 miles is all I get.
```

---
## \#114 Posted by: Nate Posted at: 2016-11-08T19:52:07.940Z Reads: 94

```
It's kinda weird it's happening within the same timeframe across a few Raptors. Gotta be some kind of correlation here.
```

---
## \#115 Posted by: Dornacht Posted at: 2016-11-08T20:05:45.409Z Reads: 97

```
Well I live in Minnesota so I can do a full test of my scarce cell pro 4 😅
```

---
## \#116 Posted by: Dedbny Posted at: 2016-11-08T20:06:47.289Z Reads: 105

```
Think its the batch 4 batteries. Also iIm getting 15.5 miles or 25km 1.5 hrs ride time av,mbut weigh 60kg. With varied elevation and speed. 

Onloop would have tested the range for specs and he weighs over 90kg or there abouts.

Just think it could be this last batch of batteries. Maybe other batch 4 Raptor owners can also update their experience on the battery.

I would say those that received their boards in August onwards.
```

---
## \#117 Posted by: Alexander Posted at: 2016-11-12T21:51:57.264Z Reads: 102

```
OMG the Raptor TWO... This. Changes. Everything :) Absolutely pre-ordering one! It's gonna be hard to top Sammy but we'll see. These things are way too much fun. The saga continues..


IF YOU WANT A RAPTOR TWO - Grab yours at www.EnertionRaptor.com and enter "100RAPTOR2" at checkout for a $100 discount!

<img src="/uploads/db1493/original/3X/4/5/4547c09ee4c7184d0fe0988f3f0bea47314c546d.jpg" width="500" height="500">
```

---
## \#118 Posted by: Dedbny Posted at: 2016-11-13T11:21:55.852Z Reads: 98

```
Has your battery issue been sorted? What was the outcome and did you work out the cause.
```

---
## \#119 Posted by: Alexander Posted at: 2016-11-13T11:41:25.960Z Reads: 101

```
I took it to my local shipping shop but they said it couldn't be sent via air without some special license, especially as it was faulty. And via sea would mean I had to pay for an entire pallet, which was silly money. So I'm waiting for the Enertion Customer Service to check with their shipping department/specialists. Rather annoying... back to spending £30/day on taxis. Tho the weather is getting pretty nasty now (even tho today's lovely out) so if it was to go wrong, Nov/Dec is the "best" time. Will update when I know more.
```

---
## \#120 Posted by: Dedbny Posted at: 2016-11-13T11:54:00.499Z Reads: 97

```
Cant you take public transport.
```

---
## \#121 Posted by: Alexander Posted at: 2016-11-13T12:38:19.399Z Reads: 96

```
Nope. For various reasons this does not work for me.
```

---
## \#122 Posted by: chinzw Posted at: 2016-11-13T20:37:08.361Z Reads: 94

```
Why would you ship the entire board when only the battery is faulty? Instead of spending 30 quid a day just order a replacement battery straight away and save some money, then when you figure out how to send it, just send the broken battery for a refund.
```

---
## \#123 Posted by: Alexander Posted at: 2016-11-14T08:54:32.077Z Reads: 91

```
It was only the battery and charger I was attempting to send.

Enertion has the ***best*** warranty in the business so I'm not concerned at all. They always come through!
```

---
## \#124 Posted by: Cloud_Gnash Posted at: 2016-11-14T17:32:00.711Z Reads: 89

```
Did you send it in for repair? Mines down to a max charge of 89% but im not sure if the total range is effected. Gonna hit up enertion support to try and send it in for repair. Good thing i have a spare :) BTW I'd highly recommend raptor owners try the MBS all terrain wheels. Now my board eats things like train tracks, sand/gravel patches and big cracks in the pavement for breakfast

<img src="/uploads/db1493/original/3X/7/b/7b06e382bda55ad89f1c1c41ac95603983f186af.jpg" width="281" height="500">
```

---
## \#126 Posted by: ddoke25 Posted at: 2016-11-14T20:01:53.881Z Reads: 87

```
Have not sent it in yet; haven't had the time.  Enertion Support sent me an address in Florida to send it to, they said they would pay for shipping.  Going to try and send it out today if I can, if not tomorrow. 

Support told me it would be a 1-2 week turnaround from them receiving my battery.

Wish I had a spare battery, its going to be a cold couple weeks without my Raptor. @Cloud_Gnash
```

---
## \#127 Posted by: Alexander Posted at: 2016-12-08T09:34:41.347Z Reads: 78

```
Update: After having no luck shipping my broken SpaceCell back for repair I came into some luck. Enertion's EU repair dude happened to be coming to the UK and I got it to him, Enertion have just sent me notice of a new one being shipped to me now. THIS IS AWESOME!!!! For anyone following my thread this is now a replacement Raptor Carbon Deck and now a replacement SpaceCell, at zero cost to me!! That's over 700 US Dollars of stuff... Thank you @onloop and @EnertionSupport you have a client for life. Never before have I had such great support/warranty with anything I've ever bought.
```

---
## \#128 Posted by: Alexander Posted at: 2016-12-08T09:41:23.555Z Reads: 80

```
Sammy's younger Brother The Raptor 2 seems to be really popular!! My referral code www.EnertionRaptor.com is getting lots of play! Though I'm a little confused about how the orange numbers correlate to the lower figures... if anyone could answer this I'd love to know? 

<img src="/uploads/db1493/original/3X/8/2/8288f39771000441aa1682af8f8734247751936a.png" width="667" height="350">
```

---
## \#129 Posted by: Dedbny Posted at: 2016-12-08T09:48:35.000Z Reads: 79

```
Hopefully we all dont have to wait 270days for the kickback.
```

---
## \#130 Posted by: Alexander Posted at: 2016-12-08T09:49:04.747Z Reads: 81

```
that I'm not so worried about. Makes complete sense when considering business cash-flow dynamics. And as I say, Enertion have been completely honorable in all their dealings with me, there's no question about their trustworthiness.
```

---
## \#131 Posted by: Evan Posted at: 2016-12-08T10:04:27.026Z Reads: 80

```
How about the drive system? Have you ever got stuff stock into your belt or pulleys? I've been annoying by them all the time.
```

---
## \#132 Posted by: Smithster Posted at: 2016-12-08T12:16:56.629Z Reads: 77

```
Nice one Alex with all those referrals should be able to pay for the R2.
```

---
## \#133 Posted by: onloop Posted at: 2016-12-08T12:25:14.995Z Reads: 81

```
Congrats on the referals.. I am very thankful.

to give some answers.

1. We can't pay the commission until the end user has the product. Otherwise people can cancel an get the refund and we also have lost the commission payments.

2. People may click your link and buy a product that's is not raptor 2. This will count as purchase. But there will not be any commissions.

Hope that helps.
```

---
## \#136 Posted by: ddoke25 Posted at: 2016-12-09T22:37:27.803Z Reads: 69

```
Glad to here your issue is getting resolved.Here's my update: Sent my battery in Nov 16th, and was contacted by support 2 weeks later letting me know that the battery is indeed dead and will be sending me a new one. Been a week and a half now and I haven't heard anything since (told me they would give me a tracking number as soon as they had one) but hopefully I will be getting one soon. (Its been wet here but a gutless Raptor has been staring me down from across the room)
Also, anyone have any luck/ info on the Nano-X getting to R1 owners? Can't seem to get any from support. @onloop
```

---
## \#137 Posted by: onloop Posted at: 2016-12-09T22:40:52.561Z Reads: 71

```
[quote="ddoke25, post:136, topic:9787"]
Can't seem to get any from support. @onloop
[/quote]

hi, 

sorry if i didn't see your message. it's normally always better to email support@enertionbaords.com

there are three consignments in transit of nano-x. US, EU & AUS

they will arrive next week.
```

---
## \#138 Posted by: ddoke25 Posted at: 2016-12-09T22:46:20.172Z Reads: 70

```
Been communicating with support@enertionboards.com for some time now and always go to them first to keep spam off the thread.

Thanks for the update and clarity, hope to see everything in soon.
```

---
