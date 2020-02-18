# Hazard &gt; Hummie Deck &amp; Hubbs, x2 FocBox, 12s4p 30Q (charge only) battery, Hoyt Puck remote

### Replies: 95 Views: 2013

## \#1 Posted by: mmaner Posted at: 2018-11-21T14:14:32.867Z Reads: 453

```
I feel like I've said this a lot lately, but I don't typically post build threads anymore unless its something unique.  The last 2 builds have been pretty unique.

This build has been dubbed "Hazard" because of the grip & speed, plus it lulls you into a sense of comfort and then you realize your going 35 mph...and that can be hazardous :metal:. 

This is not the first time I've built on 80 +/- mm platform, but its the first time that I've felt it was successful.  These wheels...mutha f#$%er, I don't know where to start.  They roll over debris like 100mm wheels, they are very cushy, soak up a lot of vibration, at 77mm wide they grip like glue.  Excellent wheels.  

I really hope hummie gets an 83/77mm Centrax wheel with a usable core, its a game changer.  I even have a set on one of my push boards.

On to the build pr0n!

![IMG_20181119_213157_1542685130312|690x288](upload://mxoshRdWXbIiYHOIEvuYqvACyVF.jpeg) 
![IMG_20181119_213403_1542685077690|690x290](upload://ihNP8dw3bmkAjPWBD2r1P1rcKve.jpeg) 
![IMG_20181119_213339_1542685102382|690x341](upload://4zRFulEEwSPiytljgGEf8NWXt4n.jpeg) 

Here's the build sheet, If anyone wants links or whatever, just let me know.

![hazard-%20build%20sheet|659x500](upload://6XujK5TB9XaIcSiSyiqkGTNdxuf.jpeg) 

This is a screen shot of the spreadsheet I use to define performance values.  It's not perfect, but I have tweaked it to my personal results and preferences.  I'm not sure about the range estimate though.  I rode 9 miles last night, had 75% battery left.  I'm using a gear ratio of 1:1 so that may need to be adjusted.

![hazard-%20esk8%20data|690x456](upload://qd9QccHMX2kyRQar4HB3kAfKOzS.jpeg) 

Im running 60a motor & 40a battery and this thing hits 35 mph with my fat ass on it, so I am hesitant to up the motor amps to 100a.  I am running sensorless FOC & set the switching frequency to 30,000 KHz per @hummie's advice and it is quiet, so very quiet.  This is the stealthiest board I've ever built.

The last thing I want to talk about, the power switch.  I didn't get a very pic of it.  But if you look at the last of the build pics you can see it in the side of the board towards the rear.  I stole that idea from @bigben.  I'll post a better pic of the switch later.

Its a 10mm switch, I used a 10mm bit from the outside, just barely angled up until I had a slot all the way through into the enclosure.  I filled the slot with epoxy and taped it off until it cured. I know that switch isn't coming out with anything but a drill :slight_smile:.
```

---
## \#2 Posted by: Sender Posted at: 2018-11-21T14:16:51.163Z Reads: 363

```
I absolutely love the split color on the front and rear wheels, just gorgeous!
```

---
## \#3 Posted by: Sender Posted at: 2018-11-21T14:18:33.240Z Reads: 353

```
Have you played around with amp settings much yet?
```

---
## \#4 Posted by: mmaner Posted at: 2018-11-21T14:21:04.266Z Reads: 346

```
I have, I had some issues getting the brakes just right.  At -20a they are just too soft, so I kept bumping it up (or rather down) and finally just put it at -60a and its a little hard now but I like hard brakes.  After I get some ride time in Im gonna bump the motor to 100a and see what it can do, but I imagine it will be too much for me.  I hit 35 mph last night and still had throttle left.
```

---
## \#5 Posted by: venom121212 Posted at: 2018-11-21T14:21:28.035Z Reads: 330

```
Lovely build. I've been trying to search for @Hummie decks because I like the look of them so much (already looking at build 2 when build 1 is finishing up). Does he/she have a site? Also what do you like about that hoyt Puck remote? Their site gives no info about features/why it's on the pricier end.
```

---
## \#6 Posted by: mmaner Posted at: 2018-11-21T14:21:55.577Z Reads: 306

```
Did you notice I used inserts?  I figured you would instantly see the missing philips head sheet metal screws and rejoice :slight_smile:,
```

---
## \#7 Posted by: PXSS Posted at: 2018-11-21T14:24:12.712Z Reads: 286

```
Sweet build
```

---
## \#8 Posted by: mmaner Posted at: 2018-11-21T14:26:59.504Z Reads: 298

```
Thank you :).  @Hummie does most of his selling here on the forum, you can PM him for specifics as he is great about answering questions.  

These decks, I have 2, are in my top 10 now.  The concave is a little mild for me, but its very comfortable.  The drop is perfect, just behind and below the base plate when drop mounted. 

The Hoyt Puck is my new favorite remote, performance wise.  I cannot say about longevity as I've only had it for a couple of weeks.  Its got a really long travel, so speed control is greatly increased over most other available remotes.  The construction is very solid.  I've had one disassembled and its pretty genius the way they built it.  Its just all around 'tight' for lack of a better word.  The only complaint I have is the interface of the wheel pin to the pot is a little weak, but a drop of epoxy and that problem is gone.
```

---
## \#9 Posted by: Sender Posted at: 2018-11-21T14:27:13.036Z Reads: 282

```
Of course I noticed! That build looks just awesome! 

I can't freggin wait to try that beast!  

So -60 motor, what about regen?

How smoothe is the startup on FOC sensorless?
```

---
## \#10 Posted by: Sender Posted at: 2018-11-21T14:29:03.134Z Reads: 273

```
[quote="mmaner, post:8, topic:75472"]
The only complaint I have is the interface of the wheel pin to the pot is a little weak, but a drop of epoxy and that problem is gone.
[/quote]

I second this for sure.  However, Hoyt is now reinforcing said piece with epoxy before shipping, so it should be of absolutely no concern!
```

---
## \#11 Posted by: mmaner Posted at: 2018-11-21T14:30:06.987Z Reads: 255

```
I've got regen at 40a per FocBox, 80a battery max total.  I thought about upping it a little to see if that changed brake performance, but honestly I'm pretty happy with the brakes now and don't like to throw more amps at the pack than it can handle.

Startup is great with sensorless FOC, its just like it has sensors.  That being said, if you pointed slightly uphill and just stand and hit the trigger, you have to hit it pretty good or it just stutters.  I kick off most of the time anyways, it takes more juice to get those first few RPM's than almost anything else, so saves a lot of battery.
```

---
## \#12 Posted by: mmaner Posted at: 2018-11-21T14:30:59.449Z Reads: 266

```
[quote="Sender, post:10, topic:75472"]
I second this for sure. However, Hoyt is now reinforcing said piece with epoxy before shipping, so it should be of absolutely no concern!
[/quote]

I didn't know that, good on them.  I talked to Edwin about that, I hadn't realized they were making changes to correct it.
```

---
## \#13 Posted by: Sender Posted at: 2018-11-21T14:34:08.022Z Reads: 273

```
Yup, this is how they are reinforcing the prongs.  It is exactly what I did on mine.

![IMG_20181121_083210_786|281x500](upload://baV1tXU5ctQgi8EtwAQ2FOe2Z1Q.jpeg) 

It would be fine without it, but it is a good place to add a bit of robustness.
```

---
## \#14 Posted by: mmaner Posted at: 2018-11-21T14:35:42.093Z Reads: 258

```
That's exactly what I did too.  I couldn't fix one as the piece is missing in action, but I preemptively reinforced the one I have now.
```

---
## \#15 Posted by: ElectricCoast Posted at: 2018-11-21T14:46:51.919Z Reads: 256

```
The board looks amazing.
```

---
## \#16 Posted by: harrypzee Posted at: 2018-11-21T14:55:21.447Z Reads: 251

```
@mmaner amazing build! I love it when ppl get creative with grip tape. This is one of the coolest grip tape designs I’ve seen! Builds like this make me unsatisfied with my plain old arbor board lol.
```

---
## \#17 Posted by: mmaner Posted at: 2018-11-21T15:00:33.749Z Reads: 255

```
I love arbor decks, I currently have 2.  A Sizzler Groundswell & a Dropcruiser Flagship.  Its hard to mess with the beauty of those decks :slight_smile:.
```

---
## \#18 Posted by: harrypzee Posted at: 2018-11-21T15:11:08.628Z Reads: 253

```
True! The grass is always greener lol. I love how arbor shows off the wood instead of hiding it away.
```

---
## \#19 Posted by: totalgeek9224 Posted at: 2018-11-21T17:50:36.938Z Reads: 248

```
Could you share that spreadsheet template, i have one but its nowhere as nice so please let me steal it 
thanks :p
```

---
## \#20 Posted by: braeden.dilger1 Posted at: 2018-11-21T17:52:32.949Z Reads: 248

```
Love that griptape, sweet build man
```

---
## \#21 Posted by: totalgeek9224 Posted at: 2018-11-21T17:55:25.943Z Reads: 238

```
On a different note, im seriously liking this build (bookmarked it lol) 
Making me consider something besides a emtb because i love the incognito look (and them phat tires)

Super clean build
![](https://i.imgur.com/ok3WXfD.gif)
```

---
## \#22 Posted by: mmaner Posted at: 2018-11-21T18:14:22.981Z Reads: 234

```
[quote="totalgeek9224, post:19, topic:75472"]
Could you share that spreadsheet template
[/quote]

Certainly, this is the latest version.

https://www.dropbox.com/s/or953wbt176zknh/MASTER%20esk8%20data%20-%20TEST.xlsx?dl=0
```

---
## \#23 Posted by: totalgeek9224 Posted at: 2018-11-21T18:15:20.914Z Reads: 222

```
You truly are the **bearded angel**
```

---
## \#24 Posted by: mmaner Posted at: 2018-11-21T18:16:24.335Z Reads: 228

```
I've built a couple of eMTB's and they are just not for me.  I hate it too because I really like building them.  This is probably the best thane build I have right now, I love it.  I doubt I'll ever get away from 6 shooters, but I like having thane too.  

This one is, unintentionally, very stealth as far as it being electric.  I mean with the grip you can see it a mile off, but other than the glow from the switch and volt meter you really have to look hard to see its powered.  I like that too :slight_smile:.
```

---
## \#25 Posted by: mmaner Posted at: 2018-11-21T18:17:18.340Z Reads: 225

```
[quote="totalgeek9224, post:23, topic:75472, full:true"]
You truly are the **bearded angel**
[/quote]

Thats funny. Ive always told my wife if I ever got super powers I wanna big ass set of black wings.  I need @psychotiller to make that upgrade kit :slight_smile:.
```

---
## \#26 Posted by: psychotiller Posted at: 2018-11-21T18:22:10.005Z Reads: 207

```
I'm on it!!
```

---
## \#27 Posted by: mmaner Posted at: 2018-11-21T18:22:21.118Z Reads: 212

```
Hell Yeah! :slight_smile:
```

---
## \#28 Posted by: totalgeek9224 Posted at: 2018-11-21T18:23:21.199Z Reads: 218

```
See, the issue is that i completely understand that. eMTB's are super capable and are like the trucks of esk8s, they take a beating and so anything you need them to, but Builds like this or some with the Evo are just more classic of a skate. You hop on those and cruise and enjoy it, whereas a eMTB just has something lacking in that division. 
As for building, eMTBs are so forgiving and you can just cram them with batteries, electronics, and other fun stuff. Everything else you need to be meticulous and crafty
```

---
## \#29 Posted by: totalgeek9224 Posted at: 2018-11-21T18:23:40.472Z Reads: 203

```
Group buy when ready :joy::joy::joy::joy::joy:
```

---
## \#30 Posted by: totalgeek9224 Posted at: 2018-11-21T18:24:05.764Z Reads: 200

```
Not too late for Secret Santa gift... ;)
```

---
## \#31 Posted by: mmaner Posted at: 2018-11-21T18:27:41.752Z Reads: 214

```
The thing I can't get used too or comfortable with is the height plus turning radius on an eMTB.  I've come too the conclusion that I like carves better than speed or off-road capability.  Also, my bludgeon with 6 shooters has been in the mid a couple of times, not deep or fast, but it was fun and it is doable.

I meant to mention, the Paris 195 v2's that @Hummie is using are surprisingly carvy and stable, even at speed.  I hit 35 mph last night and had zero wobble on good asphalt.  I didn't stay there long because it was dark, but I have  a lot of confidence in it.   

When @Hummie starts building for the kickstarter I'm gonna crack him about a thaneless set at a lower KV and figure out how to get 6 shooters on there.  I think I can do a little mill work on a set of 6er's and a little welding and make it happen pretty easy.
```

---
## \#32 Posted by: mmaner Posted at: 2018-11-21T18:28:25.663Z Reads: 203

```
[quote="totalgeek9224, post:29, topic:75472"]
Group buy when ready :joy::joy::joy::joy::joy:
[/quote]

Sorry dude, only for me.  You can have a set after I wear the new off, and rob a couple of banks :slight_smile:.
```

---
## \#33 Posted by: totalgeek9224 Posted at: 2018-11-21T18:29:51.702Z Reads: 195

```
now THAT will be a project to see
```

---
## \#34 Posted by: evoheyax Posted at: 2018-11-21T18:29:53.276Z Reads: 199

```
@mmaner Dave had made a set for me. But he said he can't find the original files, so I'm waiting for him to redo them. Once he sends me the files again, I'll have the machined. I'm hoping hummie has 4 more stators left so I can wind some 40 kv motors.
```

---
## \#35 Posted by: evoheyax Posted at: 2018-11-21T18:31:22.446Z Reads: 197

```
They also have a mistake on them that needs fixing.
```

---
## \#36 Posted by: totalgeek9224 Posted at: 2018-11-21T18:33:20.714Z Reads: 215

```
You know what, you can keep them. 
Ive got these bad boys 
![](http://www.strangehistory.net/blog/wp-content/uploads/2016/12/fairy-wings.jpg)
Each color adds an extra km/h
sorta like racing stripes, but cooler
```

---
## \#37 Posted by: mmaner Posted at: 2018-11-21T18:33:43.861Z Reads: 207

```
Thats cool, I cant wait to see them.  I remember seeing you post about them.  I just figured you let it go since I didn't hear anymore.  Hummies with 6er's would be epic.
```

---
## \#38 Posted by: mmaner Posted at: 2018-11-21T18:34:24.837Z Reads: 217

```
If I see you in those, I'm gonna make fun of you.  I'll be jealous since you can fly and all, but I'm still gonna make fun on you :slight_smile:.
```

---
## \#39 Posted by: totalgeek9224 Posted at: 2018-11-21T18:35:58.581Z Reads: 226

```
![](https://pbs.twimg.com/media/DO25xK5UMAApKw6.jpg)
```

---
## \#40 Posted by: mmaner Posted at: 2018-11-21T18:36:52.896Z Reads: 221

```
ROFL, that's good stuff :slight_smile:
```

---
## \#41 Posted by: dareno Posted at: 2018-11-21T19:33:21.260Z Reads: 192

```
Another coffee break masterpiece?  Really excited about those hubs.  As always a flawlessly presented board.
```

---
## \#42 Posted by: mmaner Posted at: 2018-11-21T19:38:07.253Z Reads: 195

```
I wish, I've been building this board for months 😀. Thank you though.
```

---
## \#43 Posted by: deucesdown Posted at: 2018-11-21T22:25:35.887Z Reads: 196

```
I'm gonna read the rest of the thread later but wth. 35mph on 12s? I'm running 13s voltage and barely tickle 30. Is my pack weak sauce? :(

I think @Winfly  was also stuck at 30mph on 13s4p 30q.

Did you get a special wind or something?

Thanks for posting, lovely.
```

---
## \#44 Posted by: mmaner Posted at: 2018-11-21T22:30:39.375Z Reads: 193

```
no special wind, just surface and settings I guess.  Ive got my battery max at 60a on both FocBox's, and charge only BMS.
```

---
## \#45 Posted by: deucesdown Posted at: 2018-11-21T22:34:18.221Z Reads: 189

```
I really should read before posting more but, that's 30a per cell? Are you acttually pulling that much? Cray cray :)  theortically my pack's specs say 140a burst. I might have to try, for science.
```

---
## \#46 Posted by: mmaner Posted at: 2018-11-21T22:35:30.477Z Reads: 183

```
I dont think so, prolly 20'ish, but I'd have to look at the logs to be sure.  Ill do some more testing this weekend and post the results, but she be fassssssst :slight_smile:.
```

---
## \#47 Posted by: 257 Posted at: 2018-11-21T23:08:35.109Z Reads: 188

```
Awesome job on this man it looks amazing :smiley: 
I think this is the last straw for me.. I need a 12s hummie build
```

---
## \#48 Posted by: mmaner Posted at: 2018-11-21T23:12:46.763Z Reads: 199

```
I appreciate it.  I would encourage anyone to get hummie hubbs.  I actually did the math.

> x2 motors = $180.00
> x2 motor mounts = $120.00
> x2 motor pulleys = $10.00
> x4 belts (x2 extras) = $12.00
> x2 wheel pulleys = $60.00
> x1 wheels (x4) = $80.00
> x1 trucks (x2) = $50.00
> Total = $512.00 + Shipping

This is just average to low end pricing on the individual components, not even close to the quality you CAN get.  Hummie Hubbs are actually economical, especially for the quality.
```

---
## \#49 Posted by: Hummie Posted at: 2018-11-21T23:20:05.691Z Reads: 196

```
itd be nice to see what kv they are on the bldc tool.  there was a bit of variance but it could only come from the rotor side as the stator side is like a clone at 9 turns on each motor.  maybe a bit less glue giving a bigger airgap, or magnets a bit overhanging the stator teeth,  I wonder.
```

---
## \#50 Posted by: mmaner Posted at: 2018-11-22T01:32:02.233Z Reads: 188

```
I'll get that data next I'm I have the enclosure off. I'll probably do some tuning Friday, so likely then.
```

---
## \#51 Posted by: evoheyax Posted at: 2018-11-22T03:03:12.912Z Reads: 176

```
It’s true but the price needs to be higher. $500 is about the cost, and that’s with free labor.
```

---
## \#52 Posted by: Winfly Posted at: 2018-11-22T03:27:28.691Z Reads: 178

```
Great build. Loves the grip tape. I only taped the front and back where I put my feet. And the CF glossy in the middle looks gorgeous. 

Are you sure you hit 35? I checked the kv last week, it's on spec 75kv ish. 13s put me at 32mph top at 52-53v haven't went full throttle at full charge yet. Would be nice to see some telemetry.

Wheels are definitely great. I would say I have put on 2-300 miles, no chip at square edge at all. 

So you are at -20 batt min for brake? I'm @ -12 and they are strong as hell. I get wobble and thrown ofd if I full brake at speed. On the other hand. I recommend switching custom bushings and pivot cup. The stock ones are too soft.
```

---
## \#53 Posted by: psychotiller Posted at: 2018-11-22T03:47:47.215Z Reads: 163

```
I think I need to raise the prices on components...Is that what you're saying?
```

---
## \#54 Posted by: mmaner Posted at: 2018-11-22T03:55:12.655Z Reads: 160

```
You prolly should, just weed out the ass hats 😀
```

---
## \#55 Posted by: Skunk Posted at: 2018-11-22T03:59:35.399Z Reads: 159

```
Wait.
You have $50 trucks, $80 wheels and motors under $200 a set?  :thinking: :grin:
```

---
## \#56 Posted by: psychotiller Posted at: 2018-11-22T04:01:20.778Z Reads: 163

```
Who me? Check with "thewheelcompany"
```

---
## \#57 Posted by: mmaner Posted at: 2018-11-22T04:12:30.917Z Reads: 180

```
[quote="Winfly, post:52, topic:75472"]
Are you sure you hit 35
[/quote]
I'm relying on telemetry, but it felt like 35 😀. 

[quote="Winfly, post:52, topic:75472"]
haven’t went full throttle
[/quote]
I still had throttle left. I wasn't watching the speed, that's the top speed reported by the app. 

[quote="Winfly, post:52, topic:75472"]
I’m @ -12 and they are strong as hell.
[/quote]
I wonder what the difference is?  -12 is usually where I start testing at, that was so light it was scary for me. I assumed it would be close and had to foot brake down hill at 20 mph 😀. 

[quote="Winfly, post:52, topic:75472"]
switching custom bushings and pivot cup
[/quote]
Yeah, I usually spend a couple of weeks dialing in my bushings. It's been awhile since I've ridden Paris 195s but I still like them, way more that C2s.
```

---
## \#58 Posted by: Winfly Posted at: 2018-11-22T04:30:43.548Z Reads: 175

```
That 35 could be from you spinning it with motors off the ground. it reads 36-37 for me when I do that. I guess I have never tested full brake at 20mph down a hill lol. That sounds hella dangerous to me.
```

---
## \#59 Posted by: mmaner Posted at: 2018-11-22T04:34:16.574Z Reads: 175

```
I don't really do that, I'm not a fan of bench tests or letting motors run crazy, always a load. 

At -20 my brakes are pretty good, gradual and not locked. At -12 it barely slowed. 

I'm thinking my kv may be higher, that might account for the speed. The @Ackmaniac so is reporting 88kv for the motor attached to the FOC box I have the BT module on. I'll check it in the VESC tool later this week.
```

---
## \#60 Posted by: Winfly Posted at: 2018-11-22T04:39:28.561Z Reads: 175

```
Hmm. Maybe you got a rare one.
```

---
## \#61 Posted by: Colson003 Posted at: 2018-11-22T04:43:18.429Z Reads: 159

```
What's the acceleration like compared to your other boards?
```

---
## \#62 Posted by: mmaner Posted at: 2018-11-22T04:58:26.532Z Reads: 162

```
I typically use a throttle curve to control the acceleration. I am in this instance as well. It's smooth, but different than a belt drive. 

I really need more ride time before I can reliably compare it to belt drive, gear drive, etc.
```

---
## \#63 Posted by: mars Posted at: 2018-11-22T08:17:12.652Z Reads: 167

```
[quote="mmaner, post:1, topic:75472"]
I don’t typically post build threads anymore unless its something unique.
[/quote]

Dear Mr Bearded Angel,

   Just wondering what it would take for you to give up your day job?

   Do you take trade-ins? :wink:

Beautiful build mate...can @sender fly a drone with camera or vice versa....
```

---
## \#64 Posted by: mmaner Posted at: 2018-11-22T14:21:53.825Z Reads: 160

```
It would take a lot for me to give up my day job, I make pretty good money 😀. 

Next time me and sender ride Im taking the drone my secret Santa sent me and getting lots if video. Prolly take multiple boards too.
```

---
## \#65 Posted by: Sender Posted at: 2018-11-22T14:31:09.856Z Reads: 154

```
Hell yeah! We will rip it up!
```

---
## \#66 Posted by: totalgeek9224 Posted at: 2018-11-22T14:49:16.330Z Reads: 158

```
There's that Hummie deck GB right now and this build is making me consider 'do I really need the only 100£ I've got saved right now?'
```

---
## \#67 Posted by: Skunk Posted at: 2018-11-22T14:51:36.654Z Reads: 152

```
I love my hummie deck. Not alot of decks out there built with esk8 in mind.
I know mmaner has more than one.
```

---
## \#68 Posted by: mars Posted at: 2018-11-22T15:07:31.600Z Reads: 160

```
We all love our @Hummie decks....:heart_eyes: 100£ saved already your good to go..:+1:

Sender and mmaner ripping it up...Yeah Baby!!!!

With a couple of strafing runs thrown in hahaha

I'll even buy a copy...lol
```

---
## \#69 Posted by: briman05 Posted at: 2018-11-22T15:10:49.434Z Reads: 161

```
You must have a room filled with your boards cause it seems like you are always building. How is that Luna switch. I saw it and that it could be a good switch figuring a ebike would pull more amps than a board.
```

---
## \#70 Posted by: mmaner Posted at: 2018-11-22T15:48:08.203Z Reads: 162

```
I have a stack of decks and boxes of parts, it's a little ridiculous 😀. 

I had high hopes for the luna AS switch, but I had 1 die on me the other day. I have pretty much given up in AS switches, I rely on XT90-S loop keys for the most part.
```

---
## \#71 Posted by: mmaner Posted at: 2018-11-22T16:01:55.039Z Reads: 175

```
Headlights, hell yeah 😀
![IMG_20181122_092509_1542902402035|503x499](upload://tcfCm0NUmsLeFGfP4qrRFqdpBZV.jpeg)

A pic of her in the wild.
![IMG_20181122_092516_1542902432880|340x500](upload://7E0UAs5YYIy6iellhfPtEs12jHg.jpeg)
```

---
## \#72 Posted by: briman05 Posted at: 2018-11-22T16:17:20.056Z Reads: 157

```
Loop keys don’t fail or atleast at a lot less of a rate. I like the look of a button or switch but I want reliability. Maybe the unity will change that just have to wait and see what everyone says
```

---
## \#73 Posted by: mmaner Posted at: 2018-11-22T16:37:42.113Z Reads: 161

```
Yeah, I agree. Loop keys wear out but they rarely fail. I like the ease of an actual seitch and the backlit switches look cool. But as an industry we just aren't there yet unfortunately.
```

---
## \#74 Posted by: BruSkater Posted at: 2018-11-22T16:59:28.108Z Reads: 161

```
Have you tried the BKB AS switch? They will be on sale for BF and they have an instant replace warranty... Wonder how good they are.

P. S. @mmaner please remember to print my xt90 pieces! :grimacing:
```

---
## \#75 Posted by: Pedrodemio Posted at: 2018-11-22T17:05:41.160Z Reads: 161

```
You guys have to stop doing these hummie based builds, makes me want one, that grip tape is sick, really like the contradiction in that, the stealthiest build possible wire a really eye catching design

Looking forward to the telemetry with the hubs, did you do any range test?
```

---
## \#76 Posted by: mmaner Posted at: 2018-11-22T18:02:41.820Z Reads: 163

```
I haven't but I will, they look good. I'm printing them now, the panel mount is done 😀.
```

---
## \#77 Posted by: mmaner Posted at: 2018-11-22T18:03:44.656Z Reads: 167

```
Thanks, I thought the grip came out well too 😀.
```

---
## \#78 Posted by: mmaner Posted at: 2018-11-22T23:25:29.303Z Reads: 169

```
I've never done a bushing setup that was perfect the 1st time, but I think this may be it. 

![IMG_20181122_170923_1542928704032|690x370](upload://AfelA8GGHBzHhTm5nEDd1lbFViw.jpeg) 

Board Side Front > Riptide Krank 96a Barrel
Street Side Front > Riptide APS 92.5a Cone
Board Side Rear > Riptide Krank 96a Barrel
Street Side Rear > Riptide Krank 93a Barrel

I used a cupped washer on rear board side, flat washer on rear street side, cupped washers front both sides. 

It's incredibly carvy, like TKP carvy.  I only got to mph in this run but there was no sign of wobble.  I'll hit some smooth asphalt tomorrow or Saturday when I'm all padded up and can peg the throttle and get some metrics.

@Alphamail do you see anything that could be better, wrong or that needs changing?
```

---
## \#79 Posted by: Alphamail Posted at: 2018-11-23T06:09:17.894Z Reads: 154

```
Thank you, just ramp up your speed progressively to get used to the new dynamics and let me know if you are having any issues.
```

---
## \#80 Posted by: banjaxxed Posted at: 2018-11-24T11:53:58.015Z Reads: 153

```
I want to see ‘follow me’ drone footage of you and @Sender doing your esk8 aerial dogfight display, goggles and all
```

---
## \#81 Posted by: dougpage Posted at: 2018-12-12T02:16:21.516Z Reads: 135

```
Any updates on your settings and your bushing setup? Are you sticking with the stock bushings? And how did you mount your enclosure? Thanks
```

---
## \#82 Posted by: mmaner Posted at: 2018-12-12T02:27:28.545Z Reads: 142

```
I haven't changed anything, it's perfect 😀. 

I'm running 60 motor amps and 60 battery amps with -60 breaking

[quote="dougpage, post:81, topic:75472"]
bushing setup?
[/quote]

This is my bushing setup

[quote="mmaner, post:78, topic:75472"]
Board Side Front &gt; Riptide Krank 96a Barrel
Street Side Front &gt; Riptide APS 92.5a Cone
Board Side Rear &gt; Riptide Krank 96a Barrel
Street Side Rear &gt; Riptide Krank 93a Barrel
[/quote]

To mount the enclosure I used 4mm inserts with 4mm socket button head bolts and stainless fender washers.
```

---
## \#83 Posted by: banjaxxed Posted at: 2018-12-12T06:37:28.884Z Reads: 124

```
Great detail as always thank you Mr Maner, I will be cogging some notes on the Hummie setup as a baseline, maybe drop the brakes a little for me
```

---
## \#84 Posted by: Hummie Posted at: 2018-12-12T07:17:05.149Z Reads: 125

```
I didnt see it back in the thread but switching the foc frequency to 30k will make it really quiet.
```

---
## \#85 Posted by: dareno Posted at: 2018-12-12T11:35:54.465Z Reads: 130

```
[quote="Hummie, post:84, topic:75472"]
foc frequency to 30k will make it really quiet.
[/quote]

Why is quiet a thing?  I love the fact my latest thing screams.  Seriously on full strap it sounds like twin turbines are having a party back there.  Why is quiet better?
```

---
## \#86 Posted by: mmaner Posted at: 2018-12-12T12:48:10.351Z Reads: 127

```
I like the sound it makes 30khz, it's almost star wars 😀
```

---
## \#87 Posted by: Hummie Posted at: 2018-12-12T15:56:48.538Z Reads: 130

```
To each their own but you should try 30k just to hear it.
```

---
## \#88 Posted by: mikedv Posted at: 2019-01-14T14:52:47.771Z Reads: 105

```
Suggestion for a deck to be electrified by @mmaner (if not already done)  :slight_smile:![8ad55438d9690768c001390e3726166e|203x499](upload://qb5QXHbZMsl6AzbTSbNRoOoNk6O.jpeg)
```

---
## \#89 Posted by: mmaner Posted at: 2019-01-14T15:11:48.176Z Reads: 104

```
That's kinda awesome, where did you find that?
```

---
## \#90 Posted by: mikedv Posted at: 2019-01-14T15:43:22.159Z Reads: 99

```
Ill look it up this evening iam not at home at the moment. This one is also funny
https://www.amazon.com/Santa-Skateboards-Jeremy-Weird-Beard/dp/B00LM3IABU
```

---
## \#91 Posted by: mikedv Posted at: 2019-01-14T15:44:28.732Z Reads: 98

```
At first I thought it was yours 😊
```

---
## \#92 Posted by: mmaner Posted at: 2019-01-14T15:54:23.342Z Reads: 99

```
I found it, google image search :).  Both of those are cool.  Ive seen the furry one before, it looks neat but I cant imaging actually riding it then going home and having to wash its hair :).
```

---
## \#93 Posted by: Sender Posted at: 2019-01-14T16:13:37.035Z Reads: 98

```
What is that dude in Alabama that makes those crazy custom boards?
```

---
## \#94 Posted by: mmaner Posted at: 2019-01-14T16:24:03.322Z Reads: 101

```
Naw, its this guy...
https://www.designboom.com/art/interview-with-illustrator-mr-bingo-07-02-2014/

Your thinking of http://bearwalker.com.  Good guess tho.
```

---
## \#95 Posted by: briman05 Posted at: 2019-01-14T16:48:46.512Z Reads: 92

```
Bear walker does some insane cnc boards.  But that hair/beard is insane on that deck from mr bingo.  That took some serious time.
```

---
