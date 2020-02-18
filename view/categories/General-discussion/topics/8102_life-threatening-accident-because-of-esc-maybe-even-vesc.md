# Life-threatening accident because of ESC (maybe even VESC)?

### Replies: 171 Views: 12276

## \#1 Posted by: Maxid Posted at: 2016-08-22T07:41:28.173Z Reads: 980

```
Just read in the news that a German guy was hospitalized with life-threatening injuries because he rode his esk8 and it suddenly stopped for no apparent reason. Threw him off the board onto the street and he did not have a helmet (which is stupid I know). 
It seems like this issue of sudden breaks that throw you off the board is quite common (at least this article is not the first time I heard about it) and we were just lucky that nobody got hurt like this until now.

Please stay safe and wear a helmet!

Edit: Oh and here is the link to the German news
http://www.ruhrnachrichten.de/staedte/werne/Lebensgefahr-36-jaehriger-Werner-stuerzt-mit-frisiertem-Skateboard;art942,3093951
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-22T07:44:09.594Z Reads: 880

```
As if Germany needed another excuse to enact more restrictive esk8 laws...

I hope it's not someone we know here :anguished:
```

---
## \#3 Posted by: Maxid Posted at: 2016-08-22T07:45:50.571Z Reads: 871

```
I know :cry:

On the other hand this could get the attention needed to start at least a conversation about how to make them safe and legal. Also it gives you perspective that the electronics we use today are in no way safe and potentially very dangerous. VESC issues can be life-threatening when they happen at the wrong time.

Right now I just hope he gets well soon...
```

---
## \#4 Posted by: elkick Posted at: 2016-08-22T09:17:18.426Z Reads: 828

```
The title is misleading, there is no reason mentioned. Hope the guy gets well soon again.

Had the same experience with the winning remote yesterday: full stop while accelerating at high speed. No coasting, full stop (blocked wheels) - and that's very dangerous!

I suspect those remotes are getting unreliable when the battery is getting empty. Else they work fine if fail safe is applied correctly. But in this situation it behaved as if fail safe wasn't working. Need to look into that.
```

---
## \#5 Posted by: Maxid Posted at: 2016-08-22T09:26:52.474Z Reads: 782

```
Yeah - sorry the question mark was supposed to go behind the entire sentence not just VESC.

Reason I did this was to get the attention on the topic that the ESCs we use are not safe. Read it a couple of times now that users had this issue with their VESCs - so wanted to show that this is a really big problem. At the time of writing I did not think of the receiver to be potentially dangerous as well. Never had any problem with my GT2B - experienced sudden breaking on my ESC however several times. But you are obviously right.
```

---
## \#6 Posted by: TarzanHBK Posted at: 2016-08-22T09:48:29.861Z Reads: 745

```
same experience here from yesterday. remote was nearly empty and i got a full stop, luckily i was only about 10 km/h!
```

---
## \#7 Posted by: Raf Posted at: 2016-08-22T09:51:45.023Z Reads: 726

```
what remote was this?
```

---
## \#8 Posted by: lox897 Posted at: 2016-08-22T09:52:08.090Z Reads: 706

```
@whitepony Did you hear about this?
```

---
## \#9 Posted by: Tweakdout Posted at: 2016-08-22T10:41:30.739Z Reads: 691

```
Some how we need to be aware of the speed and how to control a fall,  Do we have a tethered wired connected remote available... ????
```

---
## \#11 Posted by: Nordle Posted at: 2016-08-22T14:24:33.010Z Reads: 654

```
..maybe even user error instead of esc or vesc.
```

---
## \#12 Posted by: barajabali Posted at: 2016-08-22T14:40:04.110Z Reads: 646

```
That's scary no joke.
```

---
## \#13 Posted by: mishrasubhransu Posted at: 2016-08-22T14:57:00.533Z Reads: 644

```
I see that many people have build their arduino based receiver and transmitter. They/I could program the receiver in such a way that that sudden braking never happens. Even if the transmitter malfunctions and transmits instant braking signal, the receiver will produce a smoother braking commands that a rider can manage. 

Sudden acceleration((that can throw you off board too) is already managed by VESC but could be useful with other esc. So again the receiver can be programmed not to give out high acceleration signal.
```

---
## \#14 Posted by: Skitzor Posted at: 2016-08-22T15:05:32.195Z Reads: 622

```
Would you mind screwing that thing open and see if we can fit a more powerful battery in there?  (thinking 800mah). I'm on the verge to buy three of them and getting kind of worried by the reports people are making
```

---
## \#15 Posted by: Maxid Posted at: 2016-08-22T15:08:08.313Z Reads: 619

```
Arduinos are NOT known for their reliable connection and stable performance. So using an Arduino will probably increase the risk of these issues even more.
```

---
## \#16 Posted by: Nordle Posted at: 2016-08-22T15:15:38.314Z Reads: 612

```
Genuine chips are reliable.
```

---
## \#17 Posted by: mishrasubhransu Posted at: 2016-08-22T15:16:22.433Z Reads: 605

```
Umm, it will depend on how you wire them and stuff. If you solder your connection or use reliable connector(like on VESC) there WONT be any problems. At the heart of an Arduino is an AVR AtMega micro-controller, which you basically program. If your program is correct and connections strong, it will behave as you ask it to. 

If you connect the receiver like in the image below, yeah they WILL be unreliable

<img src="/uploads/db1493/original/2X/7/772901def7e600c4ab3cc53e6e716bb4abe545b6.jpg" width="690" height="273">
```

---
## \#18 Posted by: DougM Posted at: 2016-08-22T15:28:04.685Z Reads: 595

```
If we had a small group of good developers that could either fork or augment Vedder's VESC source we could add code that introduces rules for unexpected behavior, like going from full accelerate to full brake the code could transition a little more slowly.

My arduino (Teensy actually) code does this on acceleration but not brake.  It sets the acceleration rate internally rather than a straight link to the trigger - so if you go from zero to full power instantly it spreads it out across some hundreds of milliseconds.

But it would be a whole lot more reliable to do it in VESC than in your controller or driver software and also would be standard across all builds that use VESC.

DougM
```

---
## \#19 Posted by: elkick Posted at: 2016-08-22T15:29:37.273Z Reads: 560

```
I had it open a few times but didn't take pictures. It's a 500mAh in there and normally it lasts for days. I was riding yesterday for more than 5 hours and it was not fully charged. I think fully charged it wouldn't have happened. Nevertheless, it's bad. 

The VESC is 100% safe with it's timeout setting and will let you coast at any unforeseen event. But it has to relay on the data input from the device in your fingers. 

Now, if there is garbage sent by the remote it's difficult for the VESC to cope with it! The remote is sending random full stop commands when it shouldn't as soon as the battery becomes weak.
```

---
## \#20 Posted by: Maxid Posted at: 2016-08-22T15:31:11.896Z Reads: 548

```
This thread is not the place to discuss this but so far I have not seen one thread about an arduino development for this type of thing where there is no mention of signal loss or other problems.
So it seems to me that so far nobody was able to come up with a bullet-proof solution. Even the VESC itself was reported to randomly reboot...
```

---
## \#21 Posted by: devin Posted at: 2016-08-22T17:06:03.888Z Reads: 558

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#22 Posted by: sl33py Posted at: 2016-08-22T17:18:54.712Z Reads: 533

```
[quote="Maxid, post:5, topic:8102"]
the ESCs we use are not safe.
[/quote]


Let's be clear here.  **

## Skateboarding is dangerous.  Electric skateboarding is even more dangerous (more speed).

**.  If you don't know what you are doing - don't do it.  If you still choose to do it - accept that you are doing something dangerous and do what you can to mitigate the risk (like  - staying in the safest area to skate possible and not riding in traffic), and riding at a speed you feel you can control (like swerve/avoid and stop).

People need to be responsible for their own choices and don't expect safety when riding on top of a toy at 20+mph!  Wear protective gear appropriate for the speeds you want to go (like downhill folks wear if you want to go that fast), and ride speeds you feel you can safely stop at.

I also Paraglide, and when folks ask "is it safe?" - "No.  It's as safe as i can make it.  And I fly in conditions i am confident i can handle, or stay on the ground if in doubt."  Safety gear and training and practice - but it's still not safe.  Staying on the ground is safe - but not as much fun!  (cloudbase - can't even describe it properly)

/rant
```

---
## \#23 Posted by: Maxid Posted at: 2016-08-22T18:56:01.927Z Reads: 503

```
With this attitude there would be no airbags, ABS, ESP or any other safety equipment/technology.
Why are you even wearing a helmet when "you know what you are doing".
This is not that simple!

"do what you can to mitigate the risk" includes letting people know and starting discussions about the topic. It should also remind the people involved in the development that they can save lives. It should also remind people that a certain type of ESC is safer than others - right now I don't have the feeling that the VESC is the safest ESC out there. It should be but (to me after reading of multiple issues) it is not. So which one is actually better? We don't know - and that needs to change!

Edit: Obviously this could also be related to receivers - then there should also be a discussion about them. We should not wait for the first active forum member to die because of issues like this and should start talking/improving the situation regarding safety - and not just increasing speed or range.
```

---
## \#24 Posted by: Hummie Posted at: 2016-08-22T18:59:17.281Z Reads: 477

```
bet it's the receiver.  I had tons of stuff like this happen with the nunchuck and hadn't soldered connections.  Or when battery gets disconnected with vesc brakes can slam on.
```

---
## \#25 Posted by: Raf Posted at: 2016-08-22T19:28:52.320Z Reads: 473

```
if ti is the receiver does anyone know what receivers are most likely to cause this issue. What known receivers are there in the esk8 community and what one tend to fail. This way we can help to rule out some options. If we find one receiver has no problems we can ask the community if their board has ever cut out like this and then see whether its the VESC or R/T
```

---
## \#26 Posted by: DougM Posted at: 2016-08-22T19:58:30.723Z Reads: 473

```
@elkick,

re: your comment "The VESC is 100% safe with it's timeout setting "

with all due respect this is not true.  I (and a couple of other people) had a runaway where the controller stopped sending serial commands and the VESC did not time out.  It continued to execute the last command, which unfortunately in my case caused the board to continue to accelerate uncontrolled.  

I posted here and emailed Vedder, but got no response.

I do think we as a group and as a sport are maturing to the point where a little introspection into safety is likely to help more and more people and very probably will save someone's life.

@mishrasubhransu suggested that the people doing Arduino controllers should get together and share best practices - I think this is a great idea.
```

---
## \#27 Posted by: CSN Posted at: 2016-08-22T20:02:08.586Z Reads: 427

```
Seems like a lot of people getting dumped from a wheel locking up.

Does this only occur on belt drives? or do hub setups also get wheel lockup sometimes?
```

---
## \#28 Posted by: sl33py Posted at: 2016-08-22T20:04:55.619Z Reads: 434

```
You are being contrary.  I understand what you're saying about airbags, abs, etc.  but those are all part of mitigating risk.  Yeah - start the discussion.  But it's not likely a VESC issue here - most likely the Tx/Rx.  Why i use a GT2b - less prone to these issues.

I disagree that certain ESC's are safer than others.  A properly setup ESC (or VESC) with a reliable Tx/Rx setup is just as safe as a similarly setup ESC.  Now, before you jump on that - this also equals same setups for brakes, acceleration, etc.  Some ESC's have limited control of those settings.  But once configured safely, for your skill (some like more acceleration, some like more braking force) - it again is up to the rider to choose how to operate it as safely as possible.

And gear was already mentioned - nowhere did i suggest to not wear gear.  Quite the opposite.

@CSN - i think the wheel lockup is related to the Tx/Rx, not ESC.  Folks with this issue should comment with what they are using to confirm.  The timeout issue is definitely concerning - but a fair point to consider is does a normal hobby RC ESC also have this timeout?
```

---
## \#29 Posted by: stuxtruth Posted at: 2016-08-22T20:17:51.828Z Reads: 422

```
My winning remote keeps losing connection and i have to brakes. So I had to bail at high speed more than once yesterday.
```

---
## \#30 Posted by: Raf Posted at: 2016-08-22T20:25:26.925Z Reads: 441

```
I am creating this POLL to see if we can see what controllers will be more likely to have a problem. I think this will help us figure out the most secure/safe controller for our boards and maybe help solve this problem

[poll]
* Psycotiller's Winning Controller - PROBLEM
* Psycotiller's Trigger Mini Controller - PROBLEM
* Enertion's Thumb Stick Controller - PROBLEM
* DIY's Trigger Mini Controller - PROBLEM
* Hobbyking's G2TB Controller - PROBLEM
* Nyko Kama Wii Nunchuck Controller - PROBLEM
[/poll]
```

---
## \#31 Posted by: sl33py Posted at: 2016-08-22T20:27:08.546Z Reads: 422

```
[quote="DougM, post:26, topic:8102"]
I (and a couple of other people) had a runaway where the controller stopped sending serial commands and the VESC did not time out.  It continued to execute the last command, which unfortunately in my case caused the board to continue to accelerate uncontrolled.
[/quote]


Hey @DougM - what controller are you using?  This sounds really scary and i'm curious if it's Tx/Rx specific?  Would be great to confirm the culprit.
```

---
## \#32 Posted by: jdotfite Posted at: 2016-08-22T20:31:17.857Z Reads: 430

```
I had an accident last September on my DIY board that messed me up pretty bad and possibly, permanently. 

I had been riding a Boosted for two months without issues and without a helmet.  I wear a helmet when on my snowboard/scooter/etc, but for some reason, I didn't rush to buy or even put a lot of thought into wearing one while riding an electric skateboard. 

I bought a kit from dexter @diyelectricskateboards.  Had a few issues from the get go with the kit, but dexter was great and after some parts back and forth, I got it up and running.  One day I went out and was making adjustments and testing it around the neighborhood.  At one point, I went down a small hill at a low speed (maybe under 10mph) and had been holding the brake on the FlySky. That would be one of the last moments I remember from that day.

I woke up to a stranger asking me questions and an ambulance pulling up.   I spent the next few days in the hospital in a daze. I suffered a traumatic brain injury, internal/external bleeding.  

A few days out of the hospital I sat down to eat lunch and I noticed my food tasted horrible.  After 20 min of trying to figure out what hell was going on, I came to the sad conclusion that I was no longer able to smell or taste.  A few days after that, I noticed I was having trouble whistling for my dog.  Over the next week, half of my face became increasingly difficult to manipulate, to the point that it began to affect my speech.  Luckily, it stopped getting progressively worse one day and over the next week, began to slowly go back to normal.

Now here I am, almost one year later.  I look and feel the normal, but I haven't not been able smell or taste a single thing since my accident.  There is a good chance I will never have the ability to smell or taste again.  

I bought a helmet and recently grew the balls to take a look a the skateboard again.  It seems to have connection issues and the brakes will randomly give out and not work at all.  

I have no memory of the accident, but based on my injuries, it was clear I felt straight back.  My best guess is that the brakes gave out and I wasn't expecting it. 

LEARN FROM ME, WEAR A HELMET.
```

---
## \#33 Posted by: DougM Posted at: 2016-08-22T20:43:15.236Z Reads: 388

```
@sl33py

Linkie..

[Runaway Longboard](http://www.electric-skateboard.builders/t/runaway-elongboard/4812) 

let me know if you need more details
```

---
## \#34 Posted by: paragon Posted at: 2016-08-22T20:44:43.430Z Reads: 393

```
could also be the bms overcurrent or temp shutoff
```

---
## \#35 Posted by: devin Posted at: 2016-08-22T20:59:42.461Z Reads: 405

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#36 Posted by: Nordle Posted at: 2016-08-22T21:07:56.110Z Reads: 392

```
no, then it would freewheel, and not brake hard-.-
```

---
## \#37 Posted by: Hummie Posted at: 2016-08-22T21:41:06.190Z Reads: 396

```
I think youre quick to jump to it being the controller.  if we all had hardwired throttles really doubt we'd have problems.  I've been through a lot of transmitters and they're a constant source of danger.  why not go to vedder's site and tell him since you're so concerned and see what he says.   really doubt its the escs.
```

---
## \#38 Posted by: TarzanHBK Posted at: 2016-08-22T21:56:00.339Z Reads: 397

```
guys its not the vesc! its due to the winning remote on low battery! im using a x-car beast 150A esc and having the same issue when the battery is low. its always happends then. just keep your remote battery charged!
```

---
## \#39 Posted by: mason Posted at: 2016-08-22T22:10:39.261Z Reads: 404

```
guys please keep this thread constantly updated to get the exposure it deserves.
```

---
## \#40 Posted by: Nordle Posted at: 2016-08-22T22:19:26.095Z Reads: 405

```
Looks like we need a batttery upgrade for winning remotes^^
```

---
## \#41 Posted by: Raf Posted at: 2016-08-22T22:23:35.244Z Reads: 410

```
I think maybe someone should perform some tests with these remotes at full battery and low battery to see how they affect the boards. Anyone with a few different remotes that wouldn't mind doing this?
```

---
## \#42 Posted by: Jinra Posted at: 2016-08-22T22:46:45.863Z Reads: 380

```
I got too afraid to use my winning remote to do stuck throttle/unresponsive brakes. Been going great so far on my benchwheel remote though. I think the winning remote needs caps.
```

---
## \#43 Posted by: mason Posted at: 2016-08-22T23:11:54.756Z Reads: 398

```
I hope to god that Enertions remote (supposedly winning revised) will have the proper revisions to ensure reliable performance.
```

---
## \#44 Posted by: Sean555 Posted at: 2016-08-22T23:36:51.379Z Reads: 396

```
@torqueboards is your nano remote a modified winning remote?  Hoping it is because I want to order one
```

---
## \#45 Posted by: torqueboards Posted at: 2016-08-23T03:38:52.584Z Reads: 374

```
@Sean555 I haven't noticed any issues besides improper installation. Typically, it can almost happen with any other remote as well.
```

---
## \#46 Posted by: RunPlayBack Posted at: 2016-08-23T04:50:12.515Z Reads: 378

```
Your story hits really close to home, almost identical TBI that happened to my friend but at a higher speed. He also has lost his sense of smell because of the nerves in front of the skull getting damaged. I think this thread is turning into a witch hunt to single out one component but it really goes beyond that. The tech is evolving at such a rapid pace while safety awareness takes a back seat. If you look at all of the major commercial eboard companies, they each have either a video or still with non helmeted riders, some with very little to no experience. I think the DIY community will always be a step ahead in safety but it will take more than just fine print and text disclaimers to get the general public aware of the risk ladder.

I'm personally very thankful that you shared your story on your recovery. Most people will never think it will happen to them, until it does or it happens to a loved one and suddenly the world changes forever.
```

---
## \#47 Posted by: jdotfite Posted at: 2016-08-23T05:14:19.910Z Reads: 366

```
Thank you. Really sorry to hear about your friend. Sounds like a similar situation.  Mind if I ask how long ago his accident was? Has he also recovered well, aside from the anosmia?

It's hard to explain to someone what it's like to not be able to taste or smell whatsoever. It really starts to bum me out if  I think how it may be like this the rest of my life. Could have been worse though, I guess.  I'm holding out hope, I've read there are cases where it can come back, even years later. I hope for the best for your friend as well.
```

---
## \#48 Posted by: lilracerboi Posted at: 2016-08-23T05:26:55.921Z Reads: 379

```
I know with standard car ESCs, it'll slam on the brakes for a brief moment if the PPM signal cable is disconnected from the receiver in any way. I found that out when I fell at full speed while using the Wiiceiver. Thankfully my board was around 3-4 mph under 20 and I just slid on my stomach. I immediately blamed the Wiiceiver as it has more exposed connections and my case at the time was pretty open.

Haven't really tested that on the VESC, but what I do know is something similar happened while I would be holding the brakes for awhile. Could be overcurrent or something. Just a few weeks ago it kind of did it again when my Space Cell was on it, but not as hard as the car ESC.
```

---
## \#49 Posted by: RunPlayBack Posted at: 2016-08-23T05:31:20.033Z Reads: 399

```
Here's the thread I made that goes into pretty deep detail about the accident which then then turns into helmet safety:

http://www.electric-skateboard.builders/t/why-helmet-safety-has-become-my-1-priority/4288

He is doing better, pretty much a miracle he survived. We literally just had dinner a few hours ago and he mentioned that the doctors said he may not regain his sense of smell. Recently he's also been having weird tingling sensations in his neck and legs when he lowers his chin to his chest. He got an MRI and it came up clear so it may be some temporary lingering effects. But again everyone is different. The human brain is incredibly complex.

He doesn't really remember much about the accident but for me it's one of the worst things I've had to witness. Although we've ruled out any hardware errors, the fact that someone I care about got hurt on something I built really destroyed me for awhile. And while he looks pretty much normal from the outside looking in, it's still an ongoing recovery. I'm almost done with my 20 minute documentary that will hopefully bring more awareness to ESK8 safety which includes some pretty graphic footage of what went down. It was a tough thing to edit but it's helped me come to peace with my guilt.

Keep your head up brother, you aren't alone and just remember someone who reads your story will think twice about hopping on their board without a helmet.
```

---
## \#50 Posted by: Tweakdout Posted at: 2016-08-23T05:54:22.172Z Reads: 353

```
I think we need to explore a hard line connection... with some sort of quick release option, not to get dragged under a bus...board and all...
```

---
## \#51 Posted by: chinzw Posted at: 2016-08-24T05:25:19.465Z Reads: 347

```
Im sitting here on the couch with hands, elbows and hip with no skin because of something like this. In my case, the remote stopped responding and the ESC went full throttle, i had to bail at about 30km/h. Im still trying to figure out what went wrong, but until i can be 100% sure it wont happen again the board is staying in the closet.
```

---
## \#52 Posted by: devin Posted at: 2016-08-24T15:15:53.631Z Reads: 344

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#53 Posted by: chinzw Posted at: 2016-08-24T15:48:26.128Z Reads: 336

```
I dont have a VESC, just a Turnigy Trackstar 150A
```

---
## \#54 Posted by: Jinra Posted at: 2016-08-24T15:50:14.465Z Reads: 338

```
what you mind sharing what remote you were using?
```

---
## \#55 Posted by: ajaynagra Posted at: 2016-08-24T15:55:25.045Z Reads: 340

```
Does anything like the boosted board cause problems like this?
```

---
## \#56 Posted by: Raf Posted at: 2016-08-24T15:58:38.346Z Reads: 346

```
i also wonder if anyone has ever had any of these problems with @onloop enertion board, @longhairedboy boards  or other DIY pre made boards. I wonder what we are doing wrong if there are allready DIY boards made that don't have these issues but use the same components.
```

---
## \#57 Posted by: Kaly Posted at: 2016-08-24T17:30:23.833Z Reads: 352

```
This behavior happened to my a year back when I was using the wiiceiver, the issue was that a cellphone tower high jacked the signal and the board just blasted down the road. 

[quote="Raf, post:56, topic:8102"]
I wonder what we are doing wrong
[/quote]

The only thing a lot of us are doing wrong is not taking the time to get to know the board, our environment, identifying the electromagnetic interference hot spots around us and a lot of other factors that you notice once you start riding a eBoard. 

As of now I can tell  the location of most major interference hotspot in my area and avoid the area or behave accordingly to the situation. 

by not following a learning progression we put our self in great danger because this boards are not toys.
```

---
## \#58 Posted by: chinzw Posted at: 2016-08-24T18:37:18.873Z Reads: 331

```
[quote="Jinra, post:54, topic:8102, full:true"]
what you mind sharing what remote you were using?
[/quote]

Hobbyking GT2-E
```

---
## \#59 Posted by: Raf Posted at: 2016-08-24T19:03:07.141Z Reads: 332

```
Do you know if there is a difference between that one and GT2B??
```

---
## \#60 Posted by: chinzw Posted at: 2016-08-24T19:57:43.465Z Reads: 340

```
[quote="Raf, post:59, topic:8102, full:true"]
Do you know if there is a difference between that one and GT2B??
[/quote]

from what i gather its the same, but without the rechargeable batteries. I might be wrong tough.
```

---
## \#61 Posted by: Weberp7593 Posted at: 2016-08-24T21:05:31.888Z Reads: 345

```
Thats why i always wear a helmet.
ESCs and alsmost all electric components are not 100% Safe.
And we dont know what he build. Maybe it was an 30A ESC who burned...
```

---
## \#62 Posted by: longhairedboy Posted at: 2016-08-25T02:07:26.115Z Reads: 333

```
I street test all my builds. If this kind of shit happens it happens to me first and not the customer. I have the scars to prove it.
```

---
## \#63 Posted by: cantstopme Posted at: 2016-08-25T03:14:08.129Z Reads: 335

```
well that's horrible. you can beat me for this, but I think this DIY stuff is just too dangerous. When you have a factory board, at least they gone through alot of testing and you get reviews from other users by time. I mean I do understand there is a certain narcissistic sensation in these custom builds but is it worth putting your life on the line?
```

---
## \#64 Posted by: sl33py Posted at: 2016-08-25T03:22:17.864Z Reads: 342

```
[quote="cantstopme, post:63, topic:8102"]
, but I think this DIY stuff is just too dangerous.
[/quote]


Ever hear of "face plant" and the boosted and Yuneec BT board hacks?  There was malicious BT setups that could either completely take over (and hit full brakes or full throttle), or simply overwhelm the BT signal at will.  And i know boosted patched - but while can't take over, nothing stopping someone from overwhelming/saturating BT to kill your connection.  

It's not DIY vs Factory - skateboarding and esk8 is dangerous.  Wear gear, ride within your skills, pick the best setup you can and be cautious.
```

---
## \#65 Posted by: Hummie Posted at: 2016-08-25T05:55:00.300Z Reads: 322

```
Prebuilt boards don't have anything that we can't build and do better. True they're generally more reliable but they are using often the same electronics as us.  Maybe you didn't know.   The vesc.  2.4 or Bluetooth.  Nothing especially safe in their stuff.  I think it comes down to more shrink wrap and duct tape honestly and making sure connections are solidly done
```

---
## \#66 Posted by: longhairedboy Posted at: 2016-08-25T11:40:53.739Z Reads: 322

```
factory boards don't test every single unit prior to shipping. When you buy a factory board its fresh and clean and just assembled. Its never even seen the street. Maybe they have tested a reference model for hundreds of hours, and maybe they have tested the individual components and have done the math to calculate a tolerable rate of failure vs the profits they can make and the amount of insurance they can afford. So when they do fail, its a systemic failure and they affect hundreds of people. 

I can't afford any of that shit happening or i'l be ruined. So i ride them myself first. If i tear up my ass and palms  then its time to tweak something or find a new part vendor or whatever it takes.
```

---
## \#67 Posted by: Raf Posted at: 2016-08-25T11:50:55.926Z Reads: 326

```
I love this, not the fact your getting hurt cause that sucks. But the fact that you thoroughly test them to make sure they are working to a high level standard. I feel this is very important for the seller and buyer.

I wonder if us as the community could come up with a formula that works 100%. So you just buy the pieces, set them up and go. They would have to be very specific pieces but i think this could be one step closer to getting a reliable board. This would mean that it would take the freedom out of making your own specific board. But maybe a formula for new people who are looking to make this a hobby, we could make a starter board for them to build and learn about the parts and how they work and the dangers and safety of eboards and once they have that one built, they can use aspects of this formula to build there own custom one.

Just an idea
```

---
## \#68 Posted by: ajaynagra Posted at: 2016-08-25T12:11:01.970Z Reads: 327

```
Maybe logs everyone's builds that have failed on a spreadsheet and from there we can see what's happening and what is the common problem
```

---
## \#69 Posted by: longhairedboy Posted at: 2016-08-25T12:49:39.522Z Reads: 344

```
The most persistent issue i've had so far is with boxes, believe it or not. My old boxes would tear at the bolt holes after a while of heavy usage. I never noticed this in my own boards, but it was brought to my attention yesterday by my son who apparently doesn't miss anything at all ever that now my own Scarlet has worn-through bolt holes on a few of the bolt locations which have shown up since he started riding it everywhere every day. He says i baby my boards. Maybe I do, maybe that's why they didn't show up for me until they were in the customers hands. He likes to keep me honest about it too, since he posted it to instagram to tell me about it. LOL

I have already started outsourcing my FG boxes and the new ones are way tougher, but on occasion they have air bubbles in them that can eventually present cosmetic flaws as the surface cracks away over the bubble. As the evolution continues i'll likely move to another manufacturer who will do a vac bagging process using kevlar or something equally better than FG or maybe even send a deck off to have some cad work done and do injection molded boxes that conform to my deck's profile. 

One thing i won't likely do however is move to smaller boxes, i want people to be able to add whatever crap they want to in there and have plenty of room for it. If my cell packs die and they want to fill it with LiPos or even double the 18650 count with thier own home-made packs they should be able to do it. They should also be able to add BECs and lights and blutooth trancivers for the VESCs and anything else they can imagine. 

All of this is just an example of somethig i've had to work through. 

Other things i've had to work through: Bad eswitches, bad BMSs, bad volt meters/fuel gauges, fried VESCs, bad remote receivers, bad remotes... oh and one charger literally caught fire. I decided to keep it instead of RMAing it so that i can try to determine what actually happened, but i suspect it was a failed 110v/220v auto-switch thingy. 

The worst thing i've dealt with personally that wasn't reported by a customer was me repeatedly being thrown from a board while using a winning remote. My hands are still healing. You have to go through the pairing process on those precisely or the fail safes won't work and if it loses signal it will lock up the wheels. I don't understand it, but that's what happens. I've never ever had that happen with a steeze or GT2B or any other remote i've tried. If the winning is binded correctly though its fine. 

Another issue i've learned about is with the steezes. They all seem to come defaulted to channel 1 (or maybe its 2). I've since started rotating the channels with each new build so that they're all spread across the channel range. My son and I were out simultaneously testing a raptor repair and a new build i was doing and we found ourselves controlling each other's boards. It was a weird, intermittent behavior that didn't seem like interference at first, we didn't really have to be very close for it to happen since the range on those guys is like 30 feet or something similar to a playstation controller, and it didn't always behave the same way, but it did present serious issues. That could be catastrophic if two friends decided to both buy boards from me so they can ride together.
```

---
## \#70 Posted by: mason Posted at: 2016-08-25T14:14:12.403Z Reads: 299

```
[quote="longhairedboy, post:69, topic:8102"]
and we found ourselves controlling each other's boards
[/quote]

Damn.
I don't know why I'm not suprised.
```

---
## \#71 Posted by: longhairedboy Posted at: 2016-08-25T14:22:26.541Z Reads: 308

```
To clarify, we found ourselves intermittantly interfereing with each others boards in a way that was seriously inconvenient but potentially dangerous. 

For example, we were cruising >30 feet apart and everything was fine, but he would approach me from behind and i would slow a little to let him pass. As he was approaching my board would start to act like it had bad gasoline. That's really the only way to describe the symptom. It was sputtering. then when he applied the brakes, the sputter got worse and graduated to a stutter with minor lurching. 

We re-paired our rides and remotes, first nearby each other, then well over 100 feet apart. The problem didn't go away until i realized they were on the same channel and i bumped mine up a channel. Then the problem went away completely and we were cruising side by side at fun speed with no issue at all.
```

---
## \#72 Posted by: sl33py Posted at: 2016-08-25T16:53:53.567Z Reads: 315

```
[quote="longhairedboy, post:69, topic:8102"]
repeatedly being thrown from a board while using a winning remote.
[/quote]


I feel that poor tx/rx (and physical disconnects of Rx to ESC from vibrations or similar) communication and disconnects is the most dangerous part of esk8.  Since behavior varies from brakes, to acceleration, to (if you're lucky) just free-wheeling!  I've experienced one "blip" on my Marbel where the remote lost connection for about 1/4 second - which equaled me trying to "run it out" around 16-18mph (unsuccessfully, but slowed to a good tumble and unhurt besides a small skinned elbow), and multiple disconnects on a Kama/Wiiceiver.  In a stretch along a ton of apartments w/ lots of wifi interference.  

I plan to replace the kama w/ another thumb throttle option - hopefully the baby buffalo is small enough to fit her hands (her preference vs trigger), and at her slow speeds (no joke around 8mph tops) it's never been a problem.  But it's luckily just a pause and then going again, not brakes or acceleration.  

@longhairedboy - that steeze remote channel issue is terrifying.  Bad enough to have interference, but to inadvertently control another board on a set channel is frightening.  As more people ride and meetups w/ other esk8 folks - how many channels are there to avoid stepping on eachother?

On safety gear note, i got a new pair of riding gloves w/ pucks.  No i'm not sliding, but if i do eat it riding, i consistently land palm down and usually roll (somewhat well...), so while my wrist guards are great - they are a bit more of a PITA (need to remove my watch... hot and sweaty partially up my forearm, etc.)  Vs gloves - still hot, but easier to put on and protects my palm's impact point (admittedly also less impact absorption on the wrist itself).  Holesom (super great company!!  Talked w/ guy to check sizing of gloves and they sent a hand written thank you note and extra stickers - just good customer service) - got their "cords" glove.
```

---
## \#73 Posted by: longhairedboy Posted at: 2016-08-25T18:41:09.901Z Reads: 295

```
it is terrifying. Its enough to make me question everything i'm trying to do here. I'm not 100% how many channels the steeze has. I'm going to try and track down some documentation on it or at least ask Maytech to send me everything they have.

Jason posted this back in february, but i didn't see it until i started googling shit last week:
http://www.electric-skateboard.builders/t/enertion-raptor-change-the-radio-channel-on-hand-controller-steeze/1314
```

---
## \#74 Posted by: Photorph Posted at: 2016-08-26T17:02:16.791Z Reads: 286

```
Wondering why you don't use Gt2B with modified enclosures? from what I've been reading they are supposedly the most reliable remote/receivers.
```

---
## \#75 Posted by: Jinra Posted at: 2016-08-26T17:18:59.955Z Reads: 286

```
The reason I don't is because I prefer thumb controls over trigger.
```

---
## \#76 Posted by: Raf Posted at: 2016-08-26T18:08:01.717Z Reads: 284

```
Maybe there is a way to turn GT2b from trigger to thumb scroller, I think it could be the next evolution of the gt2b
```

---
## \#77 Posted by: Jinra Posted at: 2016-08-26T18:23:10.987Z Reads: 283

```
Maybe! That'd be interesting to see. I'm happy with my current thumb controller though.
```

---
## \#78 Posted by: Maxid Posted at: 2016-08-26T20:17:16.220Z Reads: 292

```
http://www.electric-skateboard.builders/t/gt2b-baby-buffalo-mod-case-3d-printable-thumb-throttle-case/4694
```

---
## \#79 Posted by: chinzw Posted at: 2016-08-27T01:49:48.168Z Reads: 304

```
So, i did some investigating today (haven't touched the board since the accident) and i found no loose cables. So i went ahead and started testing all fail options while on full throttle, remote cuts out (turning it off) and wire comes off (yanking it). If the remote cuts off, the receiver keeps the last throttle for about 5 seconds and then goes to failsafe throttle, in my case coasting (probably what happened to me, i just bailed before); Now if the cable come off, thats a nasty one, the ESC goes into brake mode , not sure what % of braking it is, i just know the motor stops instantly (didnt try this with me on the board for obvious reasons).
```

---
## \#80 Posted by: elkick Posted at: 2016-08-27T06:40:18.287Z Reads: 305

```
Seems to be a problem of your ESC:  in a RC car this behavior would make sense. But not on a longboard. Seems that the SW of the ESC was made for RC cars.
```

---
## \#81 Posted by: Xusia Posted at: 2016-08-31T05:05:28.532Z Reads: 338

```
I had a similar accident caused by a failure where the board just suddenly stopped and I was ejected.  I was wearing my full motorcycle leathers with full face helmet and still hurt fairly badly (I had internal injuries).

I think the issue here is far more than just wearing protection (which you should obviously do) - it's a drive train problem.  So long as a failure can result in the drive train locking up, thereby stopping the board and ejecting the rider, protection may not be enough.

Rather, I think the answer is to outfit the drive train with a back-torque limiting system (in the motorcycling world, this is called a slipper clutch).  This would eliminate regenerative braking (and reverse, if you set it up that way), but allow the drive train to continue to "coast" even if the motor locks up.  Having suffered injuries already, I'd happily trade regenerative braking for this added safety.

I've thought up a couple designs that integrate a back-torque limiting system into the wheel pulley, but I lack the skills to finish the design or make the part.  I'd be happy to share my thoughts with anyone who will serious consider making them - I'd be the first to put one on my board!  :slight_smile:
```

---
## \#82 Posted by: Namasaki Posted at: 2016-08-31T06:22:06.278Z Reads: 318

```
I believe this is the most reliable remote/reciever ever! 
I have used it with TB ESC and VESC and never had any unexpected braking or accelerating.
I can turn on my board jump on and start rolling down the hill and then turn on the remote and hit the throttle or brakes and it works perfectly. I can turn the remote off at any time and the board just sits there patiently waiting for me to turn it back on. Sure I have lost connection a couple times, maybe interference but when that happened the board just coasted like it was off and I just turned the remote off and back on and it was reconnected instantly.
Maybe it's the receiver. It just goes to neutral when theres no signal.
diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/torqueboards-2-4ghz-mini-remote-controller/
```

---
## \#83 Posted by: racidon Posted at: 2016-08-31T08:09:37.108Z Reads: 325

```
Due a personal issue I ran into recently (multiple actually), I'll be taking a look into some safety measures. My day to day job involves developing software and problem solving. I think the main one that should be used at the moment is a clutch system on all the motors at the shaft itself. 
Why?
If the remote fails and you have a Pi or Arduino or some form of processor to enable a slow and safe brake that's all good. But how do you prevent shorted wires in your electric motor? The ways I can think are to measure values from each phase and cut the connection when something unexpected happens, but what do you do if the short is internal and impractical to have a sensor placed with a switch? You need a mechanical interface to disconnect the motor from the wheels themselves. It would work the same as an electric drill works. They have clutches on their shafts to prevent you breaking your wrist when too much torque is transferred. This does introduce a mechanical part that does wear away especially if mistreated, but is much more disposable than life itself.

That's my first step I will be taking. Another will be to create some monitoring software that tracks anything and everything I can. To hopefully even embed ESC and ABS into our esk8s. It's not really that hard, it's mostly about getting the information, processing it and acting on it fast enough that you don't create more issues.
```

---
## \#84 Posted by: cjoliver Posted at: 2016-08-31T16:06:40.412Z Reads: 312

```
Idk what remote you're using, but after using the winning remote for a little I've noticed that if the controller disconnects at any moment whether it be it's too far away from the board or you turn it off or battery cuts off the motor goes HAM and goes full power
```

---
## \#85 Posted by: t1m0007 Posted at: 2016-08-31T16:53:53.222Z Reads: 308

```
hey man- there's a fix for this. You have to rebind the remote. I've followed these instructions and tested fail-safe by turning off the remote while at full throttle (bench and real-world) It keeps going for about half a second then coasts to stop. Here:
http://www.electric-skateboard.builders/t/problems-that-have-occurred-and-how-to-prevent-them/1937/22?u=t1m0007


I will say, I have personally experienced the sticky throttle issue with the Winning remote. its definitely just jenky/cheap construction. If I pull down all the way toward brake, then it seems to "reset" the stick and the stickiness goes away. The torque response is not constant with this remote. There must be some play between the throttle mechanism and the plastic thumb stick. I think I'm going to eventually switch to the Benchwheel controller after @jinra finishes being the guinea pig.
```

---
## \#86 Posted by: Xusia Posted at: 2016-09-01T01:53:17.862Z Reads: 297

```
To be clear, the issue I experienced was NOT a remote failure - it was multiple shorts in the electronics & motors.  No amount of monitoring or rebinding would have made any difference.

The back-torque limiting system I was referring to is a mechanical design and effectively only allows torque to be applied in one direction (forward).  This is why such a system precludes electric brakes (and of course, regenerative braking) and reverse.  There are other skateboard brakes available though.
```

---
## \#87 Posted by: julian46 Posted at: 2016-12-03T18:40:27.639Z Reads: 243

```
we are also having problems with November 2016 Evolve GT boards (carbon and bamboo) and their remotes / drop outs, stuck acceleration, delays in throttle and braking response - I was wondering if DIY was actually better (because you can update firmware and replace the radio link yourself)
```

---
## \#88 Posted by: julian46 Posted at: 2016-12-03T18:44:04.718Z Reads: 250

```
I think getting a totally reliable radio link is the holy grail of electric skateboards, DIY or Prebuilt / factory releases - everything else seems easier by comparison - all the development seems to be in other areas - I guess its just easier to use a radio link already in production - what about one of the higher end RC protocols from Spektrum, Futaba, Taranis, Jeti etc - not perfect but well developed...
```

---
## \#89 Posted by: DougM Posted at: 2016-12-03T20:33:34.590Z Reads: 244

```
XBee.  Designed exactly for this sort of thing.
```

---
## \#90 Posted by: Rye Posted at: 2016-12-03T20:36:34.224Z Reads: 243

```
Hard to go past GT2B remotes
```

---
## \#91 Posted by: mclightning Posted at: 2016-12-03T20:44:50.820Z Reads: 250

```
I used Arduino Mini Pro and Arduino UNO. I am switching to Teensy these days. Because I use multiple serial ports, reading data from UART, writing and reading from Bluetooth, debug writing to Serial. 

Arduino has huge latency on serial communication compared to Teensy. It literally becomes unusable, if code is doing anything more than read number from bluetooth apply PWM to VESC. 

I had some accidents due to Arduino. It didn't cause much trouble luckily. Thanks to my plastic motor mount setup, it just breaks apart in any crash onto wall, saving me from runaway board problem.
```

---
## \#92 Posted by: flatsp0t Posted at: 2016-12-03T20:44:51.787Z Reads: 239

```
I totally back this up. I have at least 1500 kilometres on my GT2Bs and never had any signal issue, even in crowded places with lots of interference.
```

---
## \#93 Posted by: TeleRando Posted at: 2016-12-03T20:45:13.862Z Reads: 237

```
I'm just starting to experiment with XBee. Hoping it is the answer to my remote requirements.
```

---
## \#94 Posted by: Keenan Posted at: 2016-12-03T22:41:56.858Z Reads: 231

```
Could one just disable the braking altogether? I've never needed brakes on a longboard.
```

---
## \#95 Posted by: 2-alex-2 Posted at: 2016-12-03T23:18:05.673Z Reads: 239

```
Everyone needs red to learn to fall like this guy. 

https://www.facebook.com/Sk8road/videos/10154510926666113/
```

---
## \#96 Posted by: Mrmoonlight Posted at: 2016-12-03T23:19:15.519Z Reads: 238

```
You can minimize braking by adjusting your VESC settings. Certain setups have lower braking power as well. My Carvon V2 single has enough braking power to keep your board under control, but doesn't give that sudden jerk that throws you.
```

---
## \#97 Posted by: 2-alex-2 Posted at: 2016-12-03T23:22:30.536Z Reads: 239

```
Also if your using 2.4ghz RC controller like gt2b then they have built in failsafe to stop rc from running away and need to set that to neutral aligned with vesc settings.
```

---
## \#98 Posted by: CaptainMerricka Posted at: 2016-12-04T00:04:31.914Z Reads: 237

```
 I too knew a guy in high school who ended up in a coma after longboarding a mild hill. But I still don't wear a helmet regularly just cruising on my push board. 
Now we are strapping 2hp motors to boards and haulin' ass around what used to be safe flat ground. People seem lulled into a sense of safety because they are cruising flat ground?

The community needed someone to instill the values of safety gear and I can say your doc filled that need for me. Helmet? Check. Always while E-skating. 
Your courage to put together a film has saved lives.  The eskate community needs to continue to spread your doc, and others stories, to get the community to truly embrace safety gear.
```

---
## \#99 Posted by: pyttroll Posted at: 2016-12-04T01:53:10.055Z Reads: 230

```
Would it be possible to modify existing remotes to include a "dead-switch" which would use a different transmitting/receiving frequency/technology than the original remote and would just shut the power off whenever it's pressed? You'd probably need another power source as well...
```

---
## \#100 Posted by: marcoluz Posted at: 2016-12-05T10:17:08.813Z Reads: 225

```
Thanks for sharing your story. I´ll hope you will get better and better over the time. Search for scenar devices, "maybe" it will help you in getting full recover. Wish you all the best!!
```

---
## \#101 Posted by: Malibujv Posted at: 2017-02-13T21:09:38.252Z Reads: 225

```
I've had this happen on two separate boards and the one accident was near fatal! I was on the Santa Monica bike path going full speed when I had an esc failure.  The brakes engaged and sent me flying!  I broke my back, hip, both feet, hand and tons of Stitches.  Both of the boards had high quality car escs.  I am not sure if the Vesc does the same but would love to know because if not...that is a reason to buy it.  I never ride full speed anymore and when I see guys that do it makes me cringe.

I want to add a helmet will protect your head but there are still many other vulnerable parts of the body as you can see from my accident.  Does this mean I now ride with full gear?  No, but I ride slower and 15-18 mph is still plenty quick!
```

---
## \#102 Posted by: Ackmaniac Posted at: 2017-02-13T21:28:52.072Z Reads: 216

```
I can recommend to buy a motorcycle jacket with elbow, shoulder and back protector. There are many on the market which looks like a normal jacket. And for our speeds a textile Jacket is enough. And these protectors make such a big difference. 
Last time my board send me flying at 40 km/h i only got some scratches and a painful hand because my gloves were shit.
And when i look at the jacket i don't want to think of how my body would have looked like without it.
```

---
## \#103 Posted by: Malibujv Posted at: 2017-02-13T22:06:30.973Z Reads: 209

```
Great idea!  I'm going to buy it.  Do you also wear wrist protection?
```

---
## \#104 Posted by: Ackmaniac Posted at: 2017-02-13T22:36:59.095Z Reads: 214

```
No I don't. Maybe that's a good idea. 
And for me the most important protector beside the helmet is the back protector. Just imagine you go flying and land with your back first on the sidewalk.
And always wear a helmet. I had 2 bad crashes with  my Longboards and both would have ended badly without the helmet because that was the part that took the biggest impact. 
And don't underestimate the speed. I had a crash with a motorcycle into a car at 55 km/h and broke my spine,  hip,  each rip on the left side multiple times,  destroyed the joint in my shoulder and knee and lost a kidney and don't forget all the inner bleeding at different organs. And I am not made of glass. 
Once I went to a new doctor and showed him the x-ray and CT pictures. He got really load and angry because he thought I am a medicine student and want to make a joke on him. He said he sees 3 different injuries that would be enough to let that person die. He only beleaved me after he saw the scars of the surgerys.
So just take the protection a bit more serious. And you have to be aware that when you crash in a car at 50 km/h it is 8 times the force than if you would crash with 25 km/h.
```

---
## \#105 Posted by: lowGuido Posted at: 2017-02-14T00:28:08.307Z Reads: 203

```
wrist is important, but I have trouble holding the controller with wrist guards on..
```

---
## \#106 Posted by: Malibujv Posted at: 2017-02-14T02:26:25.304Z Reads: 205

```
I agree, but at this point I have screws & bolts in my wrist and hand and trying to figure out a doable solution.  After a dozen surgeries, I'd hate to break the hardware in those areas and have to go through more surgeries.  Remarkably I'm still riding!  Don't know if I'm foolish or just addicted:)
```

---
## \#107 Posted by: ArmandR Posted at: 2017-02-14T02:33:15.336Z Reads: 200

```
So your esc shut down and your brakes flew you off the board? Do you think if you would have fallen in a safer way you would have avoided those injuries?
```

---
## \#108 Posted by: lilracerboi Posted at: 2017-02-14T02:43:26.557Z Reads: 202

```
I've been using a VESC ever since that crash and I can confirm it coasts if the connection breaks. I repeat, it does NOT brake upon connection loss.
```

---
## \#109 Posted by: Malibujv Posted at: 2017-02-14T22:06:07.913Z Reads: 195

```
I fall pretty well.  Always have, but when the brakes engaged, the jerk alone screwed up my back and nothing could have helped that. I do believe if I was wearing gear it would have prevented a ton of stitches and some of the broken bones. It was summer in Santa Monica and I was in shorts and a tshirt.  I blame myself for that and no excuse.  With that being said...I still will never cruise at 30mph.  Not even with gear.  A lot of people have questioned why Casey Neistat does not wear a helmet or gear and I have the answer for that.  He hasn't had a really bad fall yet.
```

---
## \#110 Posted by: Malibujv Posted at: 2017-02-14T22:09:21.267Z Reads: 192

```
This is great news!  I do know from building drones there are multiple failsafes to set.  One in the controller, receiver, and flight controller(which obviously does not apply).
```

---
## \#111 Posted by: RogerD Posted at: 2017-02-15T16:24:09.725Z Reads: 193

```
I've had one lockup and that was in the early days - due to insecure motor wires - one touched another and caused a glitch. Not too fast.

You may notice in other threads that I gear my boards down to not go over 22-25 mph - physically - even if the electrics went wide open the board can't go any faster.

I mostly ride at speeds where I can get off in an emergency.

Must wear my helmet more...
```

---
## \#112 Posted by: composites_r_awesome Posted at: 2017-02-23T22:21:55.110Z Reads: 188

```
I've eaten the bush couple times due to brakes not responding on Steez, but you get used to handle every braking with backup option
```

---
## \#113 Posted by: ekitesurfer Posted at: 2017-05-24T12:20:02.612Z Reads: 183

```
I got streeted the other day, and it sucks! I was running dual vesc x, benchwheel, v 2.5's. The only thing that I can think of that might have contributed to it is the fact that I was messing around with the settings in the day or so before this happened. I dont have the board with me right now, but I believe I set it up like this: 
Motor max 40,
motor min -40
Batt max 20 
batt min -8
absolute max 130

I know my batt max setting is a bit low. When it happened I was pretty much going full throttle up a hill. What happens when you exceed the Batt max setting?
```

---
## \#114 Posted by: longhairedboy Posted at: 2017-05-24T12:25:10.139Z Reads: 178

```
nothing. It throttles it and doesn't allow any more current than that to get through, basically.
```

---
## \#115 Posted by: ekitesurfer Posted at: 2017-05-24T12:28:54.304Z Reads: 177

```
That is what I thought would happen...  Now I lost faith in my esk8's.... The board worked fine before and after this happened, so Idkwtf.
```

---
## \#116 Posted by: longhairedboy Posted at: 2017-05-24T12:31:00.642Z Reads: 180

```
[quote="ekitesurfer, post:115, topic:8102"]
Now I lost faith in my esk8's
[/quote]

only those you trust can betray you. 

in this situation my immediate reflex is to blame the remote. I've got more faith in carvons and vesc-xs than i ever would a benchwheel remote.
```

---
## \#117 Posted by: ekitesurfer Posted at: 2017-05-24T12:34:33.250Z Reads: 179

```
This is the first issue I have had with them, I have a couple benchwheel's.... It is shitty that we are forced to trust our lives to a $40 POS from china. Is there such thing as a bombproof remote?
```

---
## \#118 Posted by: NAF Posted at: 2017-05-24T14:37:19.274Z Reads: 177

```
What was the remote brand ? Also did anyone ever had problems with MINI REMOTE ? It seems like it's one of the TOP reliable remotes out there.
```

---
## \#119 Posted by: will_manners Posted at: 2017-05-24T14:49:29.774Z Reads: 175

```
Can't speak from longterm experience but so far mine has been perfect. The general consensus is that it's right up there in terms of reliability with the GT2B
```

---
## \#120 Posted by: NAF Posted at: 2017-05-24T14:50:15.242Z Reads: 166

```
Mine too !! It works like a charm to be honest. It never broke the signal..it just always works.
```

---
## \#121 Posted by: longhairedboy Posted at: 2017-05-24T16:52:14.964Z Reads: 170

```
[quote="ekitesurfer, post:117, topic:8102"]
Is there such thing as a bombproof remote?
[/quote]

Steeze with mods can withstand impact and in my opinion is as reliable as the GT2Bs regarding drop outs and safety stuff. I have them for $75 and if you find a better price from a retailer i'll match it. 

GT2Bs are the king of reliability. The form factor sucks though, so choose your mod wisely and be carful when you install it. If you stick with the original trigger remote, don't drop it too much. I've shattered probably 5 of them. They do just go right back together though with some hot glue or tape. they're $20 at hobby king.
```

---
## \#122 Posted by: markyoe Posted at: 2017-05-24T16:53:18.427Z Reads: 164

```
How's the reliability of the Steez remote? Have you ever lost connection when riding and did that lead to something bad? I realize the failsafe has a part in this, but I'm just wondering about the Steez.
```

---
## \#123 Posted by: longhairedboy Posted at: 2017-05-24T16:59:20.560Z Reads: 167

```
never. I have been streeted and injured by remotes though, so i know it happens. 

I've used steezes, winnings, GT2Bs, mini remotes like the one on DIY, even off brand generic GT2B like 2.4ghz clones.

The winning is the only one that has thrown me. 

Steezes just stop controlling the board. That means if you loose connection, you're coasting. They don't continue to send the same signal, when they drop its the same as letting off the throttle. They don't lock up the wheels or send arbitrary signals. there is a situation where an unfamiliar rider may accidentally trigger cruise control then wonder why the board just keeps going but that can be resolved with education. GT2Bs and the other ones i mentioned, again in my experience, do the same. Winnings are really the outlier in remotes as far as failing badly.
```

---
## \#124 Posted by: fedestanco Posted at: 2017-05-24T17:46:30.770Z Reads: 164

```
Have you documented somewhere the mods you apply to the steez? If so could you please link tye thread? Thanks.
```

---
## \#125 Posted by: longhairedboy Posted at: 2017-05-24T17:58:07.498Z Reads: 162

```
not yet. Basically i reinforce the microswitches on the PCB behind the plastic AB switches. I haven't done this yet with the retail ones, but the ones i ship with my boards i've done a few like that. 

i just use some epoxy and tape to create a bit of hard plastic behind the momentary switch so that it doesn't mechanically tear itself off the solder pad during particular impact patterns, such as landing on its nose when its thrown or people smashing them in by pressing them way too hard. 

But it looks like none of that will be an issue much longer, when i run out of these i'm getting the new ones, probably with my logo on them. Then i will begin throwing them and seeing what happens to those guys like we do in my shop.
```

---
## \#126 Posted by: fedestanco Posted at: 2017-05-24T18:04:26.623Z Reads: 160

```
I received their email advertisind the new ones. The price is much lower, about half, so I hope the didnt cut corners on the quality of the pcb; hope they just found a cheaper plastic case.
```

---
## \#127 Posted by: longhairedboy Posted at: 2017-05-24T18:08:57.777Z Reads: 161

```
the original price of the steeze had zero to do with cost of parts and everything to do with markup. I just now got dealer pricing on those and i suspect even that is a 300% markup over cost. 

They probably just priced them aggressively. 

if they found a cheaper plastic case it better not be the kind the GT2Bs are made of. Plastic that hard can crack and shatter on impact. The steezes just bounce and occasionally break their AB microswitches.
```

---
## \#128 Posted by: Mrmoonlight Posted at: 2017-05-24T18:52:46.182Z Reads: 160

```
This is how I modded my Steeze after my AB buttons broke. I haven't had a need for my "B" button, so I only added one button. May add a second later. I also cut off the tab that pushes the cruise control button. 

<img src="/uploads/db1493/original/3X/8/7/879795d398e5477c6a3a8dc8e4c63908a6e6bf7a.JPG" width="375" height="500">
```

---
## \#129 Posted by: longhairedboy Posted at: 2017-05-24T19:07:47.213Z Reads: 153

```
that's pretty damned clever. That rugged momentary looks like it could take a beating.
```

---
## \#130 Posted by: fedestanco Posted at: 2017-05-24T19:18:54.877Z Reads: 162

```
Probably I found out why the price dropped so much: they are now selling a generic one that is not produced by them.
Actually it is so cheap that somebody is selling it along with a chinese esk8 for 60$.

<img src="/uploads/db1493/original/3X/2/b/2b96a8b22576c5c709607ef35f88b1c8551c765b.jpg" width="500" height="500">

And this is the one maytech displays, which looks identical to me:
<img src="/uploads/db1493/original/3X/1/a/1a24c7af075d978e7f6efce11f7cdc048cc19538.png" width="690" height="388">
Dont get me wrong, if it is cheap and reliable this could easily become the best remote out there.

Edit: the shape is a bit different actually.
```

---
## \#131 Posted by: Mrmoonlight Posted at: 2017-05-24T19:19:26.298Z Reads: 157

```
Been through a few drops and held up fine. Plus I got a bag of them for a couple bucks. If it brakes, it's a 5 minute fix.
```

---
## \#132 Posted by: longhairedboy Posted at: 2017-05-24T19:22:24.523Z Reads: 158

```
hmmm..... this is all starting to make more sense.
```

---
## \#133 Posted by: Hummie Posted at: 2017-05-24T19:33:35.794Z Reads: 166

```
I got the steez before. Setting it up was a bit more complicated.  Receiver was much bigger and an exposed circuit board. I was really disappointed in the throttle variability, and going down steep hills if I hit full
brake and then wanted to decrease braking I had to go all the way back to no brakes then apply again. Very annoying and others have had the same problem.  Then I threw it once and it was done.  Felt good in the hand though and the slider worked well accelerating 

The mini on the other hand I throw all the time, batteries last forever, always great reception, tiny receiver, cheap, doesn't feel like thin cheap plastic, has the wheel as another possible control of throttle and brake.  And most important to me it has very good smooth progressive brakes and acceleration 
I didn't like steez
```

---
## \#134 Posted by: ekitesurfer Posted at: 2017-05-25T04:28:28.578Z Reads: 153

```
I already have all of the remotes. When I recover from ptsd (post traumatic streeting dilemma) the mini remote is going to get another shot and my roll is going to be slowed. Maybe I hit a rock or something that I didn't see? 97mm wheels and 20mph usually rolls over most everything. Going to leave the benchwheel on another board and ride it slow, if I catch ptsd again I will post it here. For now   l guess I will hope it was a hidden rock....
```

---
## \#135 Posted by: ekitesurfer Posted at: 2017-07-05T05:08:59.464Z Reads: 151

```
I got streeted again. New APS remote, dual 2.5 carvons, dual vesc x, ackmaniac firmware. I was crossing a 4 lane highway and my board locked up in the middle, now I have some new abrasions on top of my old ones. Here are my master vesc settings, anyone have any advice?<img src="/uploads/db1493/original/3X/3/7/374b0bb0ad85b6ef5eb75cfb908d084eb93a1e3e.png" width="690" height="388"><img src="/uploads/db1493/original/3X/7/8/78315789a06605402d36d10c7f528b219c3bf376.png" width="690" height="388"><img src="/uploads/db1493/original/3X/4/7/4707e0658542592114096bfe915c7b53240675bf.png" width="690" height="388"><img src="/uploads/db1493/original/3X/6/3/63d9981f1bfb3106e3b77878b6412bffc8722d19.png" width="690" height="388">
```

---
## \#136 Posted by: ekitesurfer Posted at: 2017-07-05T05:09:48.807Z Reads: 153

```
slave vesc settings:

<img src="/uploads/db1493/original/3X/b/3/b37b43f44fb785b6a6bfdb405e6ed72f433883b2.png" width="690" height="388"><img src="/uploads/db1493/original/3X/d/f/df7e9074c4b69d04ec85dd776a7705a1030ecb69.png" width="690" height="388"><img src="/uploads/db1493/original/3X/5/d/5d730616c7569aa0c6807a7d05e3d879b9ce0995.png" width="690" height="388"><img src="/uploads/db1493/original/3X/9/f/9f4c66466aa8c43019e974bce776d195bdffb13a.png" width="690" height="388">
```

---
## \#137 Posted by: Blasto Posted at: 2017-07-05T05:21:24.878Z Reads: 147

```
[quote="ekitesurfer, post:135, topic:8102"]
I was crossing a 4 lane highway and my board locked up in the middle
[/quote]

Can you test your fail safe?

Ppm mode disabled on the master, tick the ppm display, squeeze full throttle and hold it, shut off your remote.
Does the ppm go back to 1.5ms?

A rock in the motor would abruptly stop you in your tracks also
```

---
## \#138 Posted by: ekitesurfer Posted at: 2017-07-05T05:32:00.072Z Reads: 145

```
goes back to 1.52.. no rocks in the motor.....
```

---
## \#139 Posted by: Jinra Posted at: 2017-07-05T06:38:07.071Z Reads: 151

```
Two things that may or may not be related to your issue.

1. Battery regen seems a bit high for Li-ion, are you running 10s4p li-ion? If so, most 18650's have a max charge rating of 4A which means you should have -8A for each ESC max for 4p.

2. Your control mode on slave VESC should be disabled, not on watt mode. Your neutral PPM is also slightly off (it shows 51% on your BLDC tool); this is just a nit picky thing, but shouldn't be the cause of your braking issue.

Does the braking feel like both motors are full on braking? Or does it perhaps feel like only one of the motors is full on braking? This could be an issue with a loose CAN connection.
```

---
## \#140 Posted by: ekitesurfer Posted at: 2017-07-05T06:49:44.803Z Reads: 141

```
Thanks for the reply. 

1. Ok, I will tone it down to -8, but I dont think this would cause my brakes to lock up? I was barely on the brakes when this happened. Last time this happened I was cruising up a hill, definitely not on the brakes...
2. Good to know, I will change that, but as the board worked well for many miles, I doubt these are factors..

The braking feels as if I am rolling along one moment having a great time, and the next I am lying in the middle of the highway with abrasions on top of abrasions. I taped the shit out of my can bus, those connections are not going anywhere...
```

---
## \#141 Posted by: Jinra Posted at: 2017-07-05T07:02:38.162Z Reads: 146

```
Maybe try split servo for a bit to see how that works for you
```

---
## \#142 Posted by: lrdesigns Posted at: 2017-07-05T07:13:41.970Z Reads: 149

```
[quote="ekitesurfer, post:135, topic:8102"]
I got streeted again.
[/quote]

I don't know if this issue is what caused you to get streeted, unless it was at max speed but you definitely don't want to use "limit ERPM with negative torque" this will apply brake force when you get to the ERPM limit. It can be observed on the bench, throttle up to max rpm and it will go BAP BAP BAP and start shaking wildly. With it off it will just be smooth. I also like to use the soft limit in the PPM tab with like 55k start and 60k end. 

If your motor KV is low and you never get to ERPM max then it does not matter.
```

---
## \#143 Posted by: ekitesurfer Posted at: 2017-07-05T07:18:58.242Z Reads: 147

```
That box was checked by default, and I am not using bldc, so I didn't think it mattered... I will uncheck it. I was basically kind of coasting about 15mph/ slightly braking when this streeting happened. I don't think I have ever hit that limit
```

---
## \#144 Posted by: Mrpositive Posted at: 2017-07-05T09:26:52.977Z Reads: 152

```
Hi guys reading this thread from the start and being half way through my first build. I have realised that i need to invest in safety gear.Which  I would have never really thought of  using   during my teenage skateboarding years.But now  seeing that basically were using hi powered rc cars in skateboard form and strapping our selves on top.that we are seeing what we have all probably seen from our childhood memories growing up that rc cars dont behave normally at the best of times an we seem to have trusted them somewhere along in time to put ourselves on them.How ever i think now we just need to put in some fail safe systems and safety pecautions and we will b fine.I was thinking something like the switch people are using to turn the esc on between the battery and esc maybe we can tap into that wirelessly at the controller rather than a switch on the enclosure.
perhaps a one way clutch as mentioned.Or no brakes in esc but mechanical braking like they have in some down hill board operated by foot.just some ideas really love this site thanks guys
```

---
## \#145 Posted by: ekitesurfer Posted at: 2017-07-05T16:23:15.086Z Reads: 146

```
I would like to note that i know for a fact that ackmaniacs app was not connected to my phone at the time of this streeting, so the Bluetooth module was just waiting i guess? The first streeting i do not recall if my app was connected to the board or not...
```

---
## \#146 Posted by: wafflejock Posted at: 2017-07-05T20:20:06.693Z Reads: 154

```
Depending on your controller, receiver, and the ESC there are fail safes that you can activate to keep yourself safer.  I made my own controller with an arduino pro mini 3.3v 8MHz and dirt cheap nrf24L01 modules so I have experience first hand with putting in fail safes and doing thorough testing and the result of not doing that.

First some things you can do.  Test everything.  Configure the VESC so it goes idle if the receiver stops sending a signal or it doesn't get through for whatever reason (In the App Configuration see Timeout (when no control signal is received)).  If you want it to brake as well you can configure it there but prefer going idle in any case since I don't live in a hilly area usually friction is enough to slow me down.  Next disconnect each part one by one while you are driving the motor with the board upside down on a table, make sure regardless of what you disconnect the board always goes idle.

In my case since I made my own PCB at home for connecting the arduino and nrf modules I ended up having a solder joint eventually come loose (after more than 6 months of it working fine).  The wire that was connecting the nrf module to the PCB was used for the MISO signal, but when that happened the library I was using for reading data from the connection reads the data value as 255.  Technically the radio was still connected so the call to .available() returned true but when trying to read the data when the pin disconnected it must have just floated high and went full throttle.  The board crashed into a wall then the half with the motor attached kept going down the street about a half a block before it decided to take a right and bounced over a curb into a parking lot.  Luckily through all of that nothing of any value aside from my board got any sort of damage, but it could have been a lot worse.  After that happened I brought the electronics home and started testing pulling each pin between the PCB and the NRF board to see what happens if any given pin comes loose and found the problem, I worked around the issue in my code (basically 0 or 255 is never considered valid only 1-254).  I also had issues with using 5V 16MHz Nano boards because the VIN on those is higher than what the BEC on the ESC provides so they would brown out, could have used the direct 5V but needs 3.3V for the nRF boards... long story short I found out I needed to be using the 8MHz 3.3V variation of the boards.

After getting through those issues I've had a really solid connection with the custom controller for more than 6 months.  I just got a very small batch of PCBs made (was as cheap to get 2 as 10 so 10 it was).  Not to say it was an easy and safe road but just to give you an idea of the kind of thing that could go wrong (granted most receivers are one PCB with mostly smd components but connections can still be vibrated loose).

Regarding switches the loop key is a good reliable way to physically break the connection it just needs to be easy to reach from the top of the board (biggest problem with mine is being tucked too far under but slight modification to the enclosure design will fix that.

---
  
Also worth checking out corrosion-x can be used for water proofing most electronics (still need to just physically keep the batteries from getting drenched)
```

---
## \#147 Posted by: brun Posted at: 2017-07-19T23:04:25.860Z Reads: 130

```
Have to hard disagree.  I have that remote and got tossed at 20mph when it spazzed out and pumped full brake on me and I went flying.  Haven't ridden since.
```

---
## \#148 Posted by: brun Posted at: 2017-07-19T23:11:48.787Z Reads: 137

```
Improving the remote-esc connection is good but doesn't solve the complete problem.  Specifically what the vesc should do even if it thinks it got a valid signal... like full-brake command when going at cruising speeds... a level of braking that no one would ever intentionally deliver.  The vesc should never obey this command and instead deliver a ramping brake no matter what signal it thinks it got.  In my case the vesc got a very brief but in its mind a valid short pulse width signal and blindly applied full brake and tossed me. Fixing the remote to each connection may reduce these false signals.  But if the remote potentiometer goes bad ( like mine) you are still hosed.
```

---
## \#149 Posted by: wafflejock Posted at: 2017-07-19T23:18:26.604Z Reads: 138

```
You're right there's almost always some way things can fail in a non safe way just saying there are things you can put in place.  Agree it would be good if the ESC was smarter about how the braking is applied but I believe if you limit the current for regen braking it should also effectively reduce the ability for it to lock up? (dunno maybe not)  With the Median filter on the PPM input from the receiver it should basically ignore any small glitches but like you said if a potentiometer goes bad for some reason (chemicals start eating the resistor, something mechanically breaks or disconnects) and you can still get a stream of signals telling it to do the wrong thing.

---

This is part of the reason I'm a big fan of a loop key being accessible from the top of the board it won't save you in all cases but at least if you manage to stay on it while it goes haywire you have some last ditch way to kill everything.
```

---
## \#150 Posted by: Namasaki Posted at: 2017-07-20T00:16:56.039Z Reads: 131

```
That remote has fail safe and if you set it up correctly it will just go to neutral if it disconnects which is very rare.
It may be another factor that caused your brakes to come on like a setting in the Vesc.
For example, using negative torque to limit erpm.
```

---
## \#151 Posted by: psychotiller Posted at: 2017-07-20T00:18:47.812Z Reads: 133

```
You could, and I know this is unheard of, run your board without brakes and footbrake or shutdown slide just like the caveboarders did.
```

---
## \#152 Posted by: brun Posted at: 2017-07-20T03:14:24.629Z Reads: 136

```
Good idea and Probably best for a runaway situation.  The uncommmanded instant-brake issue comes on too fast to react.  I was airborne instantly.
```

---
## \#153 Posted by: Namasaki Posted at: 2017-07-20T04:33:46.304Z Reads: 141

```
Someone else was having this issue a while back. Not sure but I think it was @Hummie
```

---
## \#154 Posted by: lrdesigns Posted at: 2017-07-20T04:44:40.577Z Reads: 145

```
What do you think we are... [quote="psychotiller, post:151, topic:8102"]
caveboarders
[/quote] ?
```

---
## \#155 Posted by: Hummie Posted at: 2017-07-20T05:25:28.961Z Reads: 145

```
.  Most dangerous for me has been receiver malfunctions from a bad connection.  I had a receiver that had problems when the wires jiggled and it would do either full acceleration or locking brakes
```

---
## \#156 Posted by: trancejunkiexxl Posted at: 2017-07-20T15:53:02.475Z Reads: 141

```
good to know all these things, definitly going to get some diversity with my hardware and start testing/checking everythinggg.. once i can actually ride again and put pads on, my flesh heals slow =|
```

---
## \#157 Posted by: Jinra Posted at: 2017-07-20T15:54:45.787Z Reads: 148

```
Servo + hot glue!
```

---
## \#158 Posted by: machadolab Posted at: 2018-02-12T00:57:17.071Z Reads: 133

```
Reviving an old thread because its good to have a reminder about safety.

My board suddenly went into full throttle mode and wouldn't respond to controls and I had to bail. Its a Nyko Kama setup with the Nyko receiver directly wired i2c into the VESC. After getting home and putting bandages on, I looked at the board and noticed the SDA wire to the Nyko receiver had broke off. Must have been making intermittent connection but then finally broke while throttle was high. I was able to reproduce it by holding the SDA wire back together, restarting the VESC, go full throttle, then remove the SDA wire - full throttle on the motor even when thumbstick is released. Obviously it needs the SDA wire to tell VESC im no longer at high throttle, but would be nice if there was some sort of detection of bad data (as all i2c read bytes would be the same when there is no SDA present). Seems like a detectable, even if rare, situation.

Skinned up,

-Mike
```

---
## \#159 Posted by: psychotiller Posted at: 2018-02-12T02:04:37.710Z Reads: 130

```
I had my dongle come loose in the riverbed one time. Same thing happened. There's no tried and true fail-safe with the nyko Kama.
```

---
## \#160 Posted by: GrecoMan Posted at: 2018-02-12T02:05:56.562Z Reads: 136

```
[quote="psychotiller, post:159, topic:8102"]
dongle
[/quote]

bwahahahahahahahahaha sorry I just can’t keep it together when people say dongle 🤣🤣
```

---
## \#161 Posted by: Deckoz Posted at: 2018-02-12T05:18:33.613Z Reads: 141

```
What's better is if you got an email it would have said Dingo Danglys Dongle. @GrecoMan
```

---
## \#162 Posted by: machadolab Posted at: 2018-02-14T21:42:07.664Z Reads: 134

```
As part of my 'what the fuck happened' testing, I walked out of range as well as just simply pulled the nyko receiver cable, and both times the board immediately went to neutral, which seemed good. So yeah, one lesson ive learned (multiple times now) is that e-skateboards take a ton of punishment and vibrations, so I should have hot glued or done some other strain-relief of the wires soldered into the nunchuck receiver breakout board.
```

---
## \#163 Posted by: psychotiller Posted at: 2018-02-15T01:16:12.241Z Reads: 130

```
Yeah...Mine went ballistic. Not neutral
```

---
## \#164 Posted by: Acidfie Posted at: 2018-04-10T17:56:02.780Z Reads: 105

```
sorry for digging this thing out but:

**how do you program your VESC that it does a full-stop when signal is lost?!?**

my remote disconnected two times, and everytime my board just rolled on and i did a stop with my foot or a slide.. like what the f***
```

---
## \#165 Posted by: onepunchboard Posted at: 2018-04-10T17:58:33.614Z Reads: 104

```
you can find failsafe feature on ppm setting. u can set how much brake u want to set to when sognal is lost
```

---
## \#166 Posted by: Acidfie Posted at: 2018-04-10T17:59:13.718Z Reads: 104

```
then why do people type in there 100A? i have 1A on every vesc..
```

---
## \#167 Posted by: onepunchboard Posted at: 2018-04-10T18:00:39.714Z Reads: 104

```
not sure. i dont use this function i just put 0 i rather use foot stop. sudden decceleration threw me off couple times so
```

---
## \#168 Posted by: Sebike Posted at: 2018-04-10T18:01:02.897Z Reads: 103

```
It's in the ackmaniac esc tool thread
```

---
## \#169 Posted by: Acidfie Posted at: 2018-04-10T18:04:07.151Z Reads: 101

```
any search words so i can look for it? do not want to scroll down 500 posts for a maybe very simple answer
```

---
## \#170 Posted by: Sebike Posted at: 2018-04-10T20:10:04.594Z Reads: 84

```
I believe it's in the first post maybe? "Failsafe" might be a good word to search for
```

---
## \#171 Posted by: Acidfie Posted at: 2018-04-10T20:16:39.340Z Reads: 87

```
found it thanks!
```

---
## \#172 Posted by: banjaxxed Posted at: 2018-04-10T21:07:09.484Z Reads: 77

```
An independent organisation would be really useful in post accident esk8 diagnosis, I doubt the authorities have the skill, it would really help in these cases...here's hoping
```

---
