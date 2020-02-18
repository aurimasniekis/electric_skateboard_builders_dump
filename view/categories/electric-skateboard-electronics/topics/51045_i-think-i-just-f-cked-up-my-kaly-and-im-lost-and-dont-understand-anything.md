# I think I just f#cked up my Kaly, and I&rsquo;m lost and don&rsquo;t understand anything

### Replies: 65 Views: 1871

## \#1 Posted by: ItsJinvy Posted at: 2018-04-03T05:59:09.476Z Reads: 385

```
Note, this board was not purchased from Ernesto, but a DIY Kaly I bought here on the forum. The build log for this board is right here:

http://www.electric-skateboard.builders/t/landsharks-trampa-trampa-urban-carver-vertigo-trucks-dual-6374-190kv-12s4p-vesc-x/19113

It was running perfectly fine for over a month up until last week when it just died on me. My friend was riding it when all of a sudden it wouldn't connect to the remote. I thought the batteries in it died, so I replaced them only to find out it didn't. Then the remote wasn't powering on because the batteries weren't connecting all the way in it's compartment to touch the positive and negative side, which I ended up breaking a piece off to try to make them connect. So whether or not the remote was a problem to begin with, it ended up being one.

But I did buy a new Thumb remote from torqueboards that arrived today. An hour ago when I was looking inside the board, I had one vesc unplugged from the anti spark swich. Well when the board was on, I ended up plugging it in and I heard a spark, and now no vescs will power on. So I'm not sure if I just fried both of them? I'm so lost right now and don't know where to begin. Located in the bay area, would love to meetup with someone to receive help in person if possible please. ![Kaly|243x500](upload://s5wwaN5Zmi3Dl1SpRavUl6Zbh3L.jpg)
```

---
## \#2 Posted by: Acido Posted at: 2018-04-03T07:28:56.807Z Reads: 355

```
Did you check the ESCs?
```

---
## \#3 Posted by: trampa Posted at: 2018-04-03T08:22:34.523Z Reads: 351

```
Y-PPM or CAN-Bus setup?
```

---
## \#4 Posted by: telnoi Posted at: 2018-04-03T08:41:09.410Z Reads: 336

```
Master is written on one of the vescs,  which probably means canbus was used.
This thread contains all the info you need if that is the case. 

https://www.electric-skateboard.builders/t/have-i-focked-my-focboxs/30428
```

---
## \#5 Posted by: DanSkates Posted at: 2018-04-03T09:21:54.172Z Reads: 305

```
Hey @ItsJinvy sounds like you got caught out the same way I did. How are your soldering skills? Mine were awful at the time (they’re much better now) and I managed to remove both canbus transceiver chips and the VESCs worked straight away. Be careful if you’re not experienced though as I basically chopped the legs off mine and then removed the legs after and ended up losing a pad in the process which will make it tricky to put them back on if ever I decided I wanted to. They work fine running in series with the split Y PPM cable but it will mean you lose traction control (if that was enabled) but most people can’t tell the difference. It isn’t really recommended to run split PPM but a lot of people do an mine work the same after the mod. 

If you’re soldering is not good you could always buy the new chips (see linked thread) and take them into a computer shop or anyone who specialises in SMD repairs and just have them both replaced. I would imagine this is the only damage and you’ll be back in action. There may even be someone in your area from the community who can help.

Good luck! Here if I can help in any way.
```

---
## \#6 Posted by: ItsJinvy Posted at: 2018-04-04T01:02:27.991Z Reads: 236

```
Thank you so much! I just saw a link to your post above. I'm honestly in such a money pit right now I feel. This is actually my second Kaly which is down. Today while riding my other Kaly, I took a first nasty fall, and I've been riding for almost two years now. Fell going around 25 to 30mph...

It hurts like a bitch, and I'm honestly thinking of selling them which I really don't want to do. The one I fell on still works, but it feels shaky and unstable now :(
```

---
## \#7 Posted by: ItsJinvy Posted at: 2018-04-04T01:03:04.993Z Reads: 231

```
Canbus

10 chars
```

---
## \#8 Posted by: ItsJinvy Posted at: 2018-04-04T01:03:18.788Z Reads: 227

```
I did, they aren't powering on
```

---
## \#9 Posted by: ItsJinvy Posted at: 2018-04-04T01:10:12.844Z Reads: 224

```
Did you remove the chips and replace them? Or just remove the chips?
```

---
## \#10 Posted by: Deckoz Posted at: 2018-04-04T01:17:18.878Z Reads: 217

```
Sounds to me like you killed the antispark... Or canbus...

Please wear pads. Hope you feel better.
```

---
## \#11 Posted by: dg798 Posted at: 2018-04-04T02:10:36.335Z Reads: 206

```
Check for faults on vesc terminal if they can connect to ur computer
```

---
## \#12 Posted by: ItsJinvy Posted at: 2018-04-04T02:20:15.669Z Reads: 197

```
It wont connect to my computer
```

---
## \#13 Posted by: ItsJinvy Posted at: 2018-04-04T02:20:31.949Z Reads: 191

```
Not even sure, I kind of just want to sell it. And will do
```

---
## \#14 Posted by: dg798 Posted at: 2018-04-04T02:29:14.576Z Reads: 188

```
If it doesn’t even turn on it’s definitely not a drv issue. I’d assume you can’t revive it. Sorry for the harsh news but that’s probably the case.
@drvwizard any input
```

---
## \#15 Posted by: DanSkates Posted at: 2018-04-04T05:18:41.296Z Reads: 183

```
Hey, I'm sorry to hear of your injuries.  I recently fell on my eMTB wearing full pads and still managed to fracture my pelvis!  Hurts.  Like.  A. Bitch.  But you gotta get back on the horse brother!  Each time you fall, you learn.  Just be sure to buy the right protection and try and avoid the same mistakes in future.

Ref, the canbus chips - yeah I just removed them, plugged the VESCs back in and they worked.  Have you removed the canbus cable connecting them too?  Like the others hear have suggested, ensure you've not blown a fuse or something too.  Are the VESCs soldered together or can you check them independantly?
```

---
## \#16 Posted by: ItsJinvy Posted at: 2018-04-04T05:48:58.384Z Reads: 180

```
Damn! How is your pelvis now?

I see, I haven't unplugged anything actually. I don't even know where all the cords and cables are going too, its so overwhelming! And I'm not sure how to check if I've blown a fuse. I can check them independently. I've been riding for almost two years, but I've got no idea how everything works. I would just need to take those off you think? Everything like disconnected, and I updated the Vesc X's before it happened. I don't know all the settings and stuff to make in the Vesc tool and stuff afterwards unfortunately. This was just a cool board I saw and I wanted it and it was awesome
```

---
## \#17 Posted by: DanSkates Posted at: 2018-04-04T06:14:35.445Z Reads: 170

```
Thanks @ItsJinvy - it's getting much better, but still hurts when I fall.  I love freestyle too much which means I fall alot!  But grass is way more forgiving than concrete! :slight_smile:

Can you post some pictures of your VESCs so we can diagnose?  We can likely help you fault find obvious stuff remotely.
```

---
## \#18 Posted by: ItsJinvy Posted at: 2018-04-04T06:24:18.101Z Reads: 180

```
Glad to hear Dan!

Haha yeah that pavement was rough, cracked my TSG Pass so I'm glad I had that on!

Board was on unfortunately when I connected an anti spark switch from the battery (or wherever the other end leads to) to the Vesc and all hell went loose :( 

Pics below. Hope it helps:

![1THUwgK|243x500](upload://xGDieuJ81vjnvjaSmdbHjftP5Fr.jpg)![ByHwHhL|243x500](upload://dFxjiUMu5RFXt1mbtMk2k8kOjdE.jpg)![FToUx0Z|243x500](upload://bjL0aZUGFceaic6ZBY08bq05asD.jpg)![HJ1Iz2b|243x500](upload://rpM30cTSn3wijDDovozRyKOzwQ.jpg)![TWHWgkX|243x500](upload://nUIkgBqwyaa303jJCjTwudNU6tw.jpg)![2x53Z41|243x500](upload://xyFbZ1mLwruTfba6njjWesqBH0i.jpg)
```

---
## \#19 Posted by: DanSkates Posted at: 2018-04-04T06:28:07.482Z Reads: 175

```
Strange that Kaly has one upside down, I'm guessing that's so the motor wires line up symetrically.  have a look at the pic below from another thread here:

![image|666x500](upload://2SLsXuqFcwepphUNJniVihaVNQl.jpg)

That's the cable connecting the 2 FOCBOXs which you need to remove.  You say you've removed the chips already?
```

---
## \#20 Posted by: ItsJinvy Posted at: 2018-04-04T06:29:56.067Z Reads: 170

```
I think one is upside down to help them both fit inside the enclosure. I'll remove that cable right now. And I have not removed those chips yet nor opened it up
```

---
## \#21 Posted by: DanSkates Posted at: 2018-04-04T06:35:06.988Z Reads: 168

```
Ah...ok.  If it is the canbus chips then you won't see any benefit until they're removed...I'd get someone to assist with this if you're unsure.  I'm in Oz otherwise I'd help.
```

---
## \#22 Posted by: ItsJinvy Posted at: 2018-04-04T06:35:40.739Z Reads: 166

```
Are they hard to remove? I just break off the joints at which they're soldered?
```

---
## \#23 Posted by: Acidfie Posted at: 2018-04-04T07:29:15.564Z Reads: 168

```
is this tin from soldering?

sorry to say that but this wiring looks really unprofessional..

![22|584x500](upload://8CwfHGx5WomCXKRC5JnEsjLw92a.jpg)
```

---
## \#24 Posted by: ItsJinvy Posted at: 2018-04-04T07:30:58.969Z Reads: 164

```
Nah that's not it nor tin
```

---
## \#25 Posted by: mikenyc Posted at: 2018-04-04T07:46:19.476Z Reads: 161

```
That doesn’t look like @Kaly’s work
```

---
## \#26 Posted by: Acidfie Posted at: 2018-04-04T08:14:50.827Z Reads: 160

```
i don't see any order of the cables, looks they're just thrown in there and glued. 

don't want to attack you or kaly but yeah, thats just my 2 cents..
```

---
## \#27 Posted by: Cobber Posted at: 2018-04-04T08:30:33.386Z Reads: 157

```
[quote="DanSkates, post:19, topic:51045"]
Strange that Kaly has one upside down
[/quote]

It isn't one of Kaly's builds Dan, neither of Jinvy's urban carvers are... for some reason Jinvy just keeps calling them a "Kaly"? :thinking:
```

---
## \#28 Posted by: Acidfie Posted at: 2018-04-04T08:33:19.773Z Reads: 150

```
[quote="ItsJinvy, post:1, topic:51045"]
Note, this board was not purchased from Ernesto, but a DIY Kaly I bought here on the forum. The build log for this board is right here:

    Landshark's Trampa | Trampa Urban Carver | Vertigo Trucks | Dual 6374 190kv | 12s4p | Vesc-X Esk8 Builds
[/quote]

ah now i get it, this explains it. if i would go commercial and my wiring would look like this, now wonder it'll fail at some time.

yet, this is still some **super bad wiring work.**
```

---
## \#29 Posted by: telnoi Posted at: 2018-04-04T08:35:29.641Z Reads: 153

```
it's a bit of a mess alright...to get this thing working again, you need to take out the VESCs anyway. Just remove the cheap glue and get that shit out of the enclosure. 

Relatively certain you get it all working again if you send it in for VESC repair. I would not recommend just removing the canbus chip, since this is VESC 6. Split ppm will supposedly cause issues. Only alternative to that which will not cause issues is running with dual receivers.

Makes no sense for us to try and make sense of the wire & glue mess.
```

---
## \#30 Posted by: ElskerShadow Posted at: 2018-04-04T08:37:50.488Z Reads: 146

```
My wirings are even worst than this , I feel bad !
```

---
## \#31 Posted by: trampa Posted at: 2018-04-04T08:48:08.886Z Reads: 147

```
[quote="telnoi, post:29, topic:51045"]
since this is VESC 6
[/quote]

Its a HW 4.12 at heart, and that is why the CAN chip blows when connecting only one ESC.
A SIX would not have had any issue.
```

---
## \#32 Posted by: telnoi Posted at: 2018-04-04T08:52:57.019Z Reads: 144

```
misread & was confused due to X (i guess this is in older focbox). 

If this thing is 4.12, the canbus chip can be removed and you can run split ppm for a cheap fix.
```

---
## \#33 Posted by: Acidfie Posted at: 2018-04-04T08:53:56.997Z Reads: 147

```
CANBUS could be teared apart or ripped out of the CANBUS port/the JST on the Slave VESC


![11|516x500](upload://8NcZKLpD5i3AzkJbTfGB8NUSECC.jpg)
```

---
## \#34 Posted by: DanSkates Posted at: 2018-04-04T11:52:34.327Z Reads: 145

```
Ahhaaaaaaa that makes sense!  I saw a video of Kaly building a board a week or so ago and the inside was even more beautiful than the outisde (if that's even possible!).

![12|690x431](upload://dQDhAuEskMbWYg0CpSvRusezlmx.jpg)

Look at those packs :heart_eyes::heart_eyes::heart_eyes:

NOTE:  I'm putting this here so people do not confuse a true @Kaly build with a build made out of Kaly parts.  I mean no disrespect to the original builder, but the majority of us build boards with good parts and do our very best.  And then there are those who create true works of art that we ride.  Kaly is one of those people and his work shouldn't be confused with that of a mere mortal. :innocent:
```

---
## \#35 Posted by: Jebe Posted at: 2018-04-04T12:03:33.753Z Reads: 137

```
Canbus chips fried. Done it myself :frowning:
```

---
## \#36 Posted by: Bjork3n Posted at: 2018-04-04T12:10:35.810Z Reads: 134

```
If canbus is causing so much problems why do people insist of using it? 
Split ppm is far more reliable...

I also fried a vesc using canbus for no reason.
```

---
## \#37 Posted by: RedEagle Posted at: 2018-04-04T12:28:12.403Z Reads: 133

```
You've either blown the can bus or the stm chip. 
Remove the can bus or replace the stm. In case of the stm you most likely have a short on the 5v rail.
```

---
## \#38 Posted by: Acidfie Posted at: 2018-04-04T12:32:24.163Z Reads: 132

```
it is stupid to not use canbus, it should **NOT** fail
```

---
## \#39 Posted by: hornet90 Posted at: 2018-04-04T12:40:48.127Z Reads: 131

```
The meaning of kaly is beautiful
```

---
## \#40 Posted by: DanSkates Posted at: 2018-04-04T12:47:22.517Z Reads: 130

```
Oh yeah!! Just looked it up. An extremely apt name 😊
```

---
## \#41 Posted by: mikenyc Posted at: 2018-04-04T12:51:41.045Z Reads: 128

```
haha, maybe kaly has better name recognition now.
```

---
## \#42 Posted by: mikenyc Posted at: 2018-04-04T12:54:09.106Z Reads: 127

```
is that really what it means? @kaly you are SO VAIN!
```

---
## \#43 Posted by: hornet90 Posted at: 2018-04-04T12:55:34.245Z Reads: 128

```
It's a Greek name meaning beautiful
```

---
## \#44 Posted by: hornet90 Posted at: 2018-04-04T12:56:12.960Z Reads: 125

```
If you made a board that looked that good what would u call it....trampa should have called it kaly
```

---
## \#45 Posted by: Bjork3n Posted at: 2018-04-04T13:19:20.084Z Reads: 128

```
Well im not alone with vesc failing with canbus connetion...
```

---
## \#46 Posted by: Acidfie Posted at: 2018-04-04T13:52:05.885Z Reads: 126

```
then maybe its the connection not correctly fixed. vibration? check it from time to time
```

---
## \#47 Posted by: Deckoz Posted at: 2018-04-04T13:57:01.761Z Reads: 131

```
The reason canbus would fail here is 

[quote="ItsJinvy, post:1, topic:51045"]
had one vesc unplugged from the anti spark swich. Well when the board was on,
[/quote]

If you power one and not the other...this is a known issue. 

Likely vibrated loose
```

---
## \#48 Posted by: Acidfie Posted at: 2018-04-04T14:11:31.576Z Reads: 125

```
so if you set canbus to true in the vesc settings and power the vesc on without a connected canbus, you likely will fry your vesc?
```

---
## \#49 Posted by: trancejunkiexxl Posted at: 2018-04-04T14:21:34.887Z Reads: 124

```
i wasn't exactly sure about what behavior not to do with can, so i did split ppm.. just a little bit of lagg though
that was the impression i got though
```

---
## \#50 Posted by: Deckoz Posted at: 2018-04-04T14:35:31.043Z Reads: 125

```
Only if the CanBuS wire is connected...

Canbus can be on and the CanBuS wire disconnected and only one esc powered on for example, bench setup I config both without the wire connected.. then later I wire them all together and power them up together.

But if canbus is on, and CanBus is connected, and you only power one esc. The CanBuS chip will likely pop.
```

---
## \#51 Posted by: Acidfie Posted at: 2018-04-04T14:36:54.488Z Reads: 121

```
strange behaviour, that doesn't make sense to me, but okay good to know.

what if the canbus disconnects while riding?
```

---
## \#52 Posted by: Deckoz Posted at: 2018-04-04T14:38:19.675Z Reads: 123

```
Disconnect is fine... You just won't have your slave...

It's when one esc is off and leeching power via the cables.

I tape/glue my canbus cables in... Either way the issue with can chips is power leeching when all devices on the bus don't have their own dedicated power source.
```

---
## \#53 Posted by: Acidfie Posted at: 2018-04-04T14:43:31.584Z Reads: 122

```
but still i don't understand why this can fry your chip..
```

---
## \#54 Posted by: mmaner Posted at: 2018-04-04T14:44:15.001Z Reads: 131

```
[quote="Deckoz, post:52, topic:51045"]
I tape/glue my canbus cables in
[/quote]

Hot glue FTW!  I put a drop on all my small cable connections...sensor, PPM, bluetooth, etc.  It's easy to pop off when you need to do maintenance but keeps cables in place very well.
```

---
## \#55 Posted by: ItsJinvy Posted at: 2018-04-04T14:54:28.111Z Reads: 136

```
Hey guys, sorry I keep calling it a Kaly. I have two boards. One of them actually is a Kaly.nyc (right) The other one I guess is a custom Trampa made from Kaly parts (left), which is why I also keep calling it a "Kaly.nyc."

![IMG_20180225_080547|281x500](upload://n5IFG5ULoQjwSgp74bZL6EYo72X.jpg)

The one on the right is the actual "Kaly.nyc" The one on the left is this board:

http://www.electric-skateboard.builders/t/landsharks-trampa-trampa-urban-carver-vertigo-trucks-dual-6374-190kv-12s4p-vesc-x/19113

Which I bought here on the forum.

It seems I need to remove the chips and run it split ppm? I already removed the canbus wire
```

---
## \#56 Posted by: Deckoz Posted at: 2018-04-04T14:54:41.034Z Reads: 131

```
The signal wire, itself is a varying voltage to produce data. 

Send varying voltage data over the CanBuS wire without the other can chip powered and the can chip will try to leach current to power the can chip. This is to much current for the source can chip to handle. It's not designed as a power rail, it's an IC component. So poof
```

---
## \#57 Posted by: ItsJinvy Posted at: 2018-04-04T15:00:34.687Z Reads: 127

```
Also it seems I should just remove all the glue and get everything out of the enclosure for now?
```

---
## \#58 Posted by: hornet90 Posted at: 2018-04-04T20:18:44.535Z Reads: 118

```
Is the real kaly running ok I'm lost
```

---
## \#59 Posted by: ItsJinvy Posted at: 2018-04-04T20:43:06.619Z Reads: 117

```
Yes lol, it just feels shaky and unstable because I fell down yesterday on it for the first time ever
```

---
## \#60 Posted by: Kaly Posted at: 2018-04-05T18:10:17.411Z Reads: 103

```
Hi there man 
You should have give me a call :wink:

That wiring is not safe, please send the DIY one to me and I’ll re-do all wiring ( imperative ) and Battery, can’t have you riding on THAT,  is a bit sketchy.
```

---
## \#61 Posted by: Kaly Posted at: 2018-04-05T18:11:17.998Z Reads: 103

```
Just making it tidy :blush:
```

---
## \#62 Posted by: ItsJinvy Posted at: 2018-04-05T18:20:08.745Z Reads: 99

```
Will do! Thank you Ernesto. I took a big fall on my other one and going to be taking a break for a while. I can use my time healing up and getting them back in good condition. I'll give you a call later today :slight_smile:

Thank you so much!
```

---
## \#63 Posted by: Sebike Posted at: 2018-04-05T18:27:04.547Z Reads: 102

```
Props!  :fist:t4:
```

---
## \#64 Posted by: spooled Posted at: 2018-04-05T21:05:07.764Z Reads: 95

```
Amazing! Can't wait for mine :smile:
```

---
## \#65 Posted by: topcloud Posted at: 2018-04-06T05:19:10.578Z Reads: 83

```
![s-l1600|690x405](upload://fVeB9DWxl83Drm4bJqXBsQxOgxp.jpg)

best.
```

---
