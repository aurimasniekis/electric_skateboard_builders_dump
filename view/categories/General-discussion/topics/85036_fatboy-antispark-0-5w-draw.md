# FatBoy antispark 0.5W draw

### Replies: 79 Views: 784

## \#1 Posted by: nuttyjeff Posted at: 2019-02-22T00:42:00.669Z Reads: 249

```
Yeah, having that problem with the FatBoy antispark right now. Didn't realise that it'll draw 0.5W on while my board was off, 10s3p batt almost died from it, from 2 weeks of being idle.
```

---
## \#2 Posted by: Kug3lis Posted at: 2019-02-22T01:25:07.790Z Reads: 238

```
Do you guys think that computers on standby also don't consume power until you turn it on? 🤦‍♂️ Maybe earth is flat too?

10s3p 30q is a month not a two weeks (333Wh/0.5Wh = ~28 days) if you storing your board for these kind of periods if I were u I would disconnect battery from everything...
```

---
## \#3 Posted by: Deodand Posted at: 2019-02-22T01:29:33.671Z Reads: 232

```
0.5W though? That's like 10 mA of leakage current. Really bad, I assume your switch doesn't leak that badly?
```

---
## \#4 Posted by: Kug3lis Posted at: 2019-02-22T01:31:09.671Z Reads: 225

```
It's not leaking anything it's power consumption on off state (vreg and logic) 5mA
```

---
## \#5 Posted by: Deodand Posted at: 2019-02-22T01:32:35.910Z Reads: 221

```
Well that's shit then. Redesign your switch lol.
```

---
## \#6 Posted by: Kug3lis Posted at: 2019-02-22T01:34:04.215Z Reads: 217

```
Well I don't give a fck u want cheap have cheap ldo vreg :D
```

---
## \#7 Posted by: Deodand Posted at: 2019-02-22T01:36:11.009Z Reads: 211

```
Are you saying that an expensive power switch should leak 5ma? I'm pretty confused. All I know is if I designed a power switch then realised it consumed that much in off state I'd bin the design and start over.
```

---
## \#8 Posted by: Kug3lis Posted at: 2019-02-22T01:36:59.375Z Reads: 210

```
Go confuse urself more ;)
```

---
## \#9 Posted by: nuttyjeff Posted at: 2019-02-22T01:39:47.896Z Reads: 209

```
Exactly. The unity doesnt consume any power (or neglible power consumption) even after leaving my board idle for 2 weeks.. I'd say that 0.5W of idle consumption is too much, but to each his own.
```

---
## \#10 Posted by: Deodand Posted at: 2019-02-22T01:40:44.316Z Reads: 208

```
For reference I think it draws 2-3 uA. So roughly 2000 times less.
```

---
## \#11 Posted by: Kug3lis Posted at: 2019-02-22T01:42:13.479Z Reads: 208

```
Yeah right 3uA xD
```

---
## \#12 Posted by: nuttyjeff Posted at: 2019-02-22T01:42:20.497Z Reads: 214

```
[quote="Kug3lis, post:167, topic:31872"]
10s3p 30q is a month not a two weeks (333Wh/0.5Wh = ~28 days)
[/quote]

Do you store your board at 42V? Facepalm.

I said my 10s3p got drained to 0 in 2 weeks. No where did I state that it was from a full charge because I sure as hell don't store my boards at full charge. 

Edit: I have over 10 boards and hence store them at 60% charge for each to preserve battery life. It is obvious that there are times where I neglect riding some boards for weeks or months at end, and having a passive 0.5W drain isn't ideal. I can't imagine being alone in this dilemma. I'm sure there are some who are sesonal riders and don't ride in the winter.

[quote="Kug3lis, post:167, topic:31872"]
Do you guys think that computers on standby also don’t consume power until you turn it on? :man_facepalming: Maybe earth is flat too?
[/quote]

It's not a matter of whether it consumes power, it's a matter of how much it consumes and what an acceptable limit is.
```

---
## \#13 Posted by: Kug3lis Posted at: 2019-02-22T01:43:09.883Z Reads: 210

```
I store my board at 240V does it matter?
```

---
## \#14 Posted by: nuttyjeff Posted at: 2019-02-22T01:43:59.732Z Reads: 205

```
Whatever floats your boat.
```

---
## \#15 Posted by: Deodand Posted at: 2019-02-22T01:45:52.202Z Reads: 206

```
Sorry checked datasheet, 9uA. My mistake. So just about 1000 times less.
```

---
## \#16 Posted by: Kug3lis Posted at: 2019-02-22T01:47:29.235Z Reads: 209

```
Well the switches are different in the first place but ur switch aka unity still wasn't delivered since last autumn...
```

---
## \#17 Posted by: nuttyjeff Posted at: 2019-02-22T01:49:52.500Z Reads: 216

```
[quote="Kug3lis, post:181, topic:31872"]
unity still wasn’t delivered since last autumn…
[/quote]

1. The first batch of Unitys have been delivered. I own one.

2. That isn't the point. We're merely pointing out that a drain of 0.5W is too high on idle. If you don't want to anything about it, that's fine. 

Side note, your attitude regarding this matter is really off putting. I find you constantly critizing designs of others (e.g. flipsky), but when someone brings up a concern on one of your designs, you get super defensive. Not cool.

[quote="Kug3lis, post:171, topic:31872, full:true"]
Well I don’t give a fck u want cheap have cheap ldo vreg
[/quote]

Edit: i don't think this is the right place to address this particular concern. I'm sorry @goldenHusky for de-railing your thread. If a moderator could kindly address this (either by deleting the messages or moving it to a seperate thread, that'll be most appreciated.) @anorak234 @mmaner @treenutter thanks!
```

---
## \#18 Posted by: deucesdown Posted at: 2019-02-22T04:07:48.389Z Reads: 198

```
Well I'm glad I clicked on this thread. 0.5w passive drain for a power switch is worthy of notice when purchasing especially on what would be considered a high end item. Draining $300 packs dry in a month is way no bueno. I have a couple of these for future projects, and certainly would have made sad and angry faces at some point had I not seen your post.

Thanks @nuttyjeff I consider your post a PSA.

@Kug3lis you owe your customers better. At least a warning. It's hard to continue to support your products if you don't share stuff like this.
 
@goldenHusky sorry for cluttering your thread. I'm excited to see the pre-charge circuit. I wasn't sure if I was being dumb when I made this post 

https://www.electric-skateboard.builders/t/new-open-source-antispark-switch/82154/32?u=deucesdown

EDIT

Adding some math.
0.5w at say 10s fully charged is .5w/42v == 0.012a.
4p 30q pack is 3000mah*4 == 12ah.
12ah / 0.012a == 1000hr.
1000hr / 24h = 41.67 days to drain down to 0% (about 6 weeks).
```

---
## \#19 Posted by: rich Posted at: 2019-02-22T07:36:57.039Z Reads: 190

```
I'm afraid this forum needs a new rule against "customer bashing", can't believe these rude words.

@nuttyjeff I just checked the voltage on my 10s4p with connected standard vedder antispark switch. I didn't ride the board since 5 months and the total voltage decreased max. 0.2V - 0.4V, could be even less.

On my MTB I have a 3way directFET antispark switch from @goldenHusky (I pull up to 100A on 12s, works great) and I didn't ride for 2 months, too. There is no noticeable voltage drop (maybe 0.1V or less).

That's the first time I read that an antispark switch drains a battery within weeks. This is very bad and should not exist.
```

---
## \#20 Posted by: b264 Posted at: 2019-02-22T07:47:00.537Z Reads: 189

```
[quote="nuttyjeff, post:177, topic:31872"]
Do you store your board at 42V? Facepalm.

I said my 10s3p got drained to 0 in 2 weeks no where did I state that it was from a full charge because I sure as hell don’t store my boards at full charge.
[/quote]

For people who use these as tools and not toys, boards get stored "charged".  Do you store your car with all the gasoline drained out?  Fuck no... because you might need it at any moment...

So if a system can't be stored at full charge, then it's defective for my purposes.  A car that couldn't be parked with more than a half-tank would be defective also.

Sure, if a board breaks down I won't charge it until it's repaired.  But to suggest that storing these uncharged is normal or correct is hilarious.  I don't make these to look at, I make them to ride.
```

---
## \#21 Posted by: nuttyjeff Posted at: 2019-02-22T07:58:55.031Z Reads: 186

```
[quote="b264, post:189, topic:31872"]
For people who use these as tools and not toys, boards get stored “charged”. Do you store your car with all the gasoline drained out? Fuck no… because you might need it at any moment…
[/quote]

I store most of my boards at 60% simply because I have alot of them and storing them at full overtime damages the cells. (Correct me if i'm wrong). Would you then advise me to store them all at full charge...?

As far as I know, cars can be stored at a full tank of gas or half a tank without any detrimental effects, the analogy falls short there.
```

---
## \#22 Posted by: b264 Posted at: 2019-02-22T08:04:03.740Z Reads: 182

```
If your boards aren't ready to ride, then they are toys.

When you use these as transportation, you will understand.

It's no different than having a car that takes 3 hours to start.  It's not practical.  If a battery can't be stored full, then it's a shitty battery.  Shitty batteries exist.  Maybe that's one reason I like LiFePO4.
```

---
## \#23 Posted by: nuttyjeff Posted at: 2019-02-22T08:08:25.029Z Reads: 179

```
[quote="b264, post:191, topic:31872"]
If your boards aren’t ready to ride, then they are toys.
[/quote]

Storing a board at 60% makes it unridable? I dont get it.
```

---
## \#24 Posted by: Kug3lis Posted at: 2019-02-22T09:41:19.039Z Reads: 181

```
[quote="deucesdown, post:187, topic:31872"]
@Kug3lis you owe your customers better. At least a warning. It’s hard to continue to support your products if you don’t share stuff like this.
[/quote]

I don't understand what to share? How the fck do you expect a device to stay in stand by mode and listen when the board starts pushing or **momentary button** is pressed and turn everything on, not the latching switch which turns on everything and keeps the power on but is dumb as fck as it doesn't have any logic at all. Yes, I could have made it eat no current at all, but would you pay a few times more for it? No, you would all cry how it is super expensive and shit. Efficient parts dc/dc converters and etc cost money, and you guys always complaining that everything is expensive so for god sake please don't cry.

I am not sure but every switch which uses momentary button and something like PTS will have the same issue.

[quote="rich, post:188, topic:31872"]
I’m afraid this forum needs a new rule against “customer bashing”, can’t believe these rude words.
[/quote]

Well, good thing I stopped making new stuff for **this forum** as no one in this forum even appreciate people doing hard work to make something good for this community, just fcking bashing everyone around and complaining about every fcking single bit. This community went from super innovative and creative to let's find another issue and bash someone about it.

[quote="rich, post:188, topic:31872"]
There is no noticeable voltage drop (maybe 0.1V or less).
[/quote]

It's latching switch there shouldn't be any drop at all...

[quote="rich, post:188, topic:31872"]
That’s the first time I read that an antispark switch drains a battery within weeks. This is very bad and should not exist.
[/quote]

Well if it should not exist then I can just stop selling it because I am not going to spend any more hours of my precious personal time to create stuff for the community who doesn't appreciate anything. Don't forget esk8 DIY market is not thousands of customer but at least a few hundreds, and all those purchases not even compensate for the time people spend innovating and creating products for this community.

No wonder people are leaving this place. You can consider me switching off pretty soon too, as I am not going to share my thousands of hours of programming and designing on ESC with this community which will just find another thing to complain about.

Aurimas
```

---
## \#25 Posted by: rich Posted at: 2019-02-22T10:20:56.590Z Reads: 164

```
[quote="Kug3lis, post:193, topic:31872"]
no one in this forum even appreciate people doing hard work to make something good for this community
[/quote]

I don't know the previous history why you think like that. I'm sure many people appreciate you hard work and like your products. I personally never had items from you but I'm sure they are good quality. And you had a title :wink:

I heard your switch is reliable, didn't know it starts when pushing which is great.
I think the main point is that customers should know about the fact that they MUST disconnect the battery e.g. in winter break. I just imagine someone coming back home after 3 weeks holidays and the battery is dead :unamused:
```

---
## \#26 Posted by: Andy87 Posted at: 2019-02-22T10:54:18.921Z Reads: 167

```
oh @Kug3lis , why so angry?
just understand our site too.
we are no engineers and don´t understand things like that.
how can we know how much energy your switch use on standby? ... I should now start to research data sheets of components you used? come on... not really please.
Is it a big problem to add a small notification on your website? one sentence "disconnect from battery when not charging for more than 2 weeks" and you save out of any claims. 
If people don´t read it, it´s there problem.

I´m sure people appreciate your work and the work of your paps.
you can read it here multiple times!
It´s up to you on which comments you set your focus.
There always fanboys and hater. That´s not only in this community.
You created what you think is how it should be with all your products. If other people don´t like it or say something about the design than you can just ignore it, or have a look if there is some truth in it and you can improve your product.
No need to get crazy about it.

[quote="Kug3lis, post:193, topic:31872"]
Don’t forget esk8 DIY market is not thousands of customer but at least a few hundreds, and all those purchases not even compensate for the time people spend innovating and creating products for this community.
[/quote]
That´s very true words, but you wouldn´t be here if you wouldn´t enjoy riding. Maybe things changed in your life in the past month, but don´t tell us you spend all your free time just to create products for only us.
you made it for you too.
because you was not happy with what you could get on the market and wanted to make it better!
Nobody force you to do anything for us here.
It´s your free decision what you are doing with your free time.
always!

@goldenHusky sorry for that and @mmaner or @anorak234 it´s really time that this topic is split from the original post.
```

---
## \#27 Posted by: brenternet Posted at: 2019-02-22T15:08:08.522Z Reads: 139

```
Obligatory post calling Kugs a dickhead.

Just doing my duty for our community.
```

---
## \#28 Posted by: moon Posted at: 2019-02-22T15:24:56.446Z Reads: 136

```
Was about to tag you
```

---
## \#29 Posted by: amazingdave Posted at: 2019-02-22T15:28:05.697Z Reads: 134

```
I wondered where my battery was leaking to.... a heads up would have been nice.
```

---
## \#30 Posted by: linsus Posted at: 2019-02-22T16:07:20.494Z Reads: 129

```
Just put a disclaimer, **use at own risk, study schematic, check dissipation factors etc etc**
```

---
## \#31 Posted by: 3DServisas Posted at: 2019-02-22T16:09:06.549Z Reads: 132

```
This switch is not full disconnect from battery its device which helps you to turn on/off board quicker than other ways.

In normal occasion you will have BMS which would protect your battery from full discharge and full mechanical disconnect from the battery for storing long term.

The device consumes less or around 5mA which in normal uses cases shouldn't disturb much of your daily usages and in long term you always want to disconnect your battery from any switch as they can not be trusted. What if when you storing your board for long term and randomly MOSFET dies because of manufacturer issue and your 3kW battery pack shorts and burns your apartment to the ground? I wouldn't trust any device connected to big battery packs without supervision and protections.

Yes it was our mistake of not mentioning this kind of detail, but like I mentioned before in normal configuration and usage this kind of power consumption would not matter much. You can't have all together.

P.S. Battery disconnect is most important feature in any project it can be car, bike, board or any other electric device u always must have a quick way to disconnect power from everything in case of emergency.
```

---
## \#32 Posted by: DerelictRobot Posted at: 2019-02-22T16:12:47.745Z Reads: 130

```
[quote="Kug3lis, post:2, topic:85036"]
Do you guys think that computers on standby also don’t consume power until you turn it on? :man_facepalming: Maybe earth is flat too?
[/quote]

I managed to fat finger a like on your post without realizing it last night. It was not intentional, and I'd like to take the accidental click back but I cannot.

Why am I going through the trouble of telling you this?

Your attitude sucks. I had items in my cart all the way up to checking out and then I saw this. This isn't a bluff, your system even sent me an email asking if I still wanted them via PayPal.

Customer service and representation matters a lot these days. You're doing a disservice to all the great work your dad is doing by coming on here and acting like an entitled know-it-all. Based on your EE designs, perhaps you could do with a bit more humility.
```

---
## \#33 Posted by: nuttyjeff Posted at: 2019-02-22T16:15:54.352Z Reads: 134

```
[quote="3DServisas, post:31, topic:85036"]
Yes it was our mistake of not mentioning this kind of detail
[/quote]

Thanks for admitting to the mistake. I appreciate it.

[quote="3DServisas, post:31, topic:85036"]
What if when you storing your board for long term and randomly MOSFET dies because of manufacturer issue and your 3kW battery pack shorts and burns your apartment to the ground? I wouldn’t trust any device connected to big battery packs without supervision and protections.
[/quote]

Correct me if I'm wrong, but isn't there a fuse to prevent this?
```

---
## \#34 Posted by: topcloud Posted at: 2019-02-22T16:18:25.322Z Reads: 133

```
Guys, please, let's pause for a moment.

Whether or not a 0.5W draw for an always-on standby switch is appropriate for esk8 is purely subjective.

This is not a design flaw, or boon.  It simply is what it is.  3DServisas has stated they omitted this detail and that's understandable.

The question should simply be, is there a bypass requested in the next version for people who wish to store their boards, long-term and not use them.

Thank you, team.  This is a good post, we do not need emotions - just solutions.  

I own one and I've never thought to leave my board sitting that long - yet thanks for the reminder for me to charge my bikes, because they've been sitting all winter.
```

---
## \#35 Posted by: Kug3lis Posted at: 2019-02-22T16:21:08.503Z Reads: 131

```
[quote="DerelictRobot, post:32, topic:85036"]
Your attitude sucks. I had items in my cart all the way up to checking out and then I saw this. This isn’t a bluff, your system even sent me an email asking if I still wanted them via PayPal.

Customer service and representation matters a lot these days. You’re doing a disservice to all the great work your dad is doing by coming on here and acting like an entitled know-it-all. Based on your EE designs, perhaps you could do with a bit more humility.
[/quote]

Well looks like I will be leaving this forum as everyone here are pussies who get offended on simple things :) Well no wonder, back in the beginning was forum was much better but oh well :slight_smile:

P.S. I don't care if you going to buy it or not I hate when people threaten you on something like I am sitting here and crying that you not going to buy stuff. Btw there is no one else selling 35º risers for trampa/mbs trucks so if you going to ditch your project idea because someone told you that you are a bit of pussy maybe its time to man up a bit ;)
```

---
## \#36 Posted by: DerelictRobot Posted at: 2019-02-22T16:23:09.413Z Reads: 125

```
[quote="Kug3lis, post:35, topic:85036"]
Btw there is no one else selling 35º risers for trampa/mbs trucks so if you going to ditch your project idea because someone told you that you are a bit of pussy maybe its time to man up a bit
[/quote]

Or it's entirely possible that as an adult engineer, I'm capable of machining them myself and was buying them from you guys to support the DIY community, as I do with a lot of gear.

This is your bed dude. You made it.
```

---
## \#37 Posted by: Kug3lis Posted at: 2019-02-22T16:23:38.526Z Reads: 123

```
Just go machine not crying here ;)
```

---
## \#38 Posted by: DerelictRobot Posted at: 2019-02-22T16:24:25.754Z Reads: 127

```
[quote="Kug3lis, post:35, topic:85036"]
Well looks like I will be leaving this forum as everyone here are pussies who get offended on simple things
[/quote]

The irony of this isn't lost to the adults in the room.

Don't let the door hit ya kid.
```

---
## \#39 Posted by: nuttyjeff Posted at: 2019-02-22T16:24:34.528Z Reads: 134

```
[quote="Kug3lis, post:35, topic:85036"]
Well looks like I will be leaving this forum as everyone here are pussies who get offended on simple things
[/quote]

Dude.. scroll up... You were literally the first to get offended... :man_facepalming:
```

---
## \#40 Posted by: 3DServisas Posted at: 2019-02-22T16:25:34.738Z Reads: 134

```
[quote="nuttyjeff, post:33, topic:85036"]
Correct me if I’m wrong, but isn’t there a fuse to prevent this?
[/quote]

If you have a fuse in your set up then yes it would prevent this kind of thing but our switch doesn't have integrated fuse for size concerns as it's easier to embed fuse inline.

Not forget that fuses not always help.
```

---
## \#41 Posted by: nuttyjeff Posted at: 2019-02-22T16:29:07.863Z Reads: 133

```
[quote="3DServisas, post:40, topic:85036"]
If you have a fuse in your set up then yes it would prevent this kind of thing but our switch doesn’t have integrated fuse for size concerns as it’s easier to embed fuse inline.
[/quote]

Ah, I noted that your switch didn't have a fuse. All good on that front, it was pretty obvious to me haha.

[quote="3DServisas, post:40, topic:85036"]
Not forget that fuses not always help
[/quote]

Care to elaborate?
```

---
## \#42 Posted by: Blasto Posted at: 2019-02-22T16:29:35.824Z Reads: 132

```
It’s pretty easy to get the OFF power conssumption in uA range.

If you share your schematic i can give you a hand
```

---
## \#43 Posted by: 3DServisas Posted at: 2019-02-22T16:32:19.257Z Reads: 128

```
We can make it draw 0 when it is off but would like to pay extra for it? Everything is possible to make, but you people always complaining that it is too expensive.

We can make it so switch would make u coffee when u turn on it :laughing:
```

---
## \#44 Posted by: Blasto Posted at: 2019-02-22T16:34:45.433Z Reads: 127

```
I’m talking about a few passive components, it’s shouldn’t change the bom price.

But i can also get rekt’d
```

---
## \#45 Posted by: 3DServisas Posted at: 2019-02-22T16:37:09.777Z Reads: 125

```
It is nice that you are suggesting, but you don't know our switch design and how it works. It is not a few extra passive components.
```

---
## \#46 Posted by: Blasto Posted at: 2019-02-22T16:40:22.600Z Reads: 124

```
Canadian sorry, just trying to lend a hand. What do i know
```

---
## \#47 Posted by: 3DServisas Posted at: 2019-02-22T16:41:08.417Z Reads: 127

```
I dont mind you trying to lend a hand, but I would love to see how u would turn off/on power rail with few passive components :D
```

---
## \#48 Posted by: amazingdave Posted at: 2019-02-22T16:41:20.249Z Reads: 130

```
Manners....
```

---
## \#49 Posted by: Blasto Posted at: 2019-02-22T16:54:56.205Z Reads: 131

```
![image|560x300](upload://bx9H3sOLTi9sjJeC8kmETUW3cPN.png) 

your welcom
```

---
## \#50 Posted by: 3DServisas Posted at: 2019-02-22T16:57:59.558Z Reads: 130

```
Yes, this is nice example if your switch is using MCU...
```

---
## \#51 Posted by: DerelictRobot Posted at: 2019-02-22T16:59:03.794Z Reads: 128

```
[quote="3DServisas, post:50, topic:85036, full:true"]
Yes, this is nice example if your switch is using MCU…
[/quote]

An MCU can cost less than a few dollars to add to a BOM. Especially if they're fire and forget.
```

---
## \#52 Posted by: 3DServisas Posted at: 2019-02-22T17:00:28.074Z Reads: 126

```
[quote="DerelictRobot, post:51, topic:85036"]
An MCU can cost less than a few dollars to add to a BOM. Especially if they’re fire and forget.
[/quote]

Everything is cheap if you only consider BOM price.
```

---
## \#53 Posted by: DerelictRobot Posted at: 2019-02-22T17:01:06.174Z Reads: 127

```
[quote="3DServisas, post:52, topic:85036"]
Everything is cheap if you only consider BOM price
[/quote]

In device manufacturing at any quantity, it's king.

MCUs can do a lot for very little, I have found they save time and effort again and again as they often allow for simple yet smart design choices at a minimal cost to BOM. Unless you're talking about the firmware development, which I consider negligible with this level of complexity of device.
```

---
## \#54 Posted by: Blasto Posted at: 2019-02-22T17:03:20.827Z Reads: 127

```
guess it would be possible to have a latching circuit to get rid of the mcu, like you said, i don't know your circuit. i'm just guessing best practice.
```

---
## \#55 Posted by: 3DServisas Posted at: 2019-02-22T17:06:46.196Z Reads: 130

```
Well yes, but manpower and etc things cost money too. Some device design would cost more than BOM for 1M devices ;) Everyone can buy a part but not everyone can make that part work like intended and specialist get paid to do it.

[quote="DerelictRobot, post:53, topic:85036"]
which I consider negligible with this level of complexity of device.
[/quote]

Try to explain that to any EE company by telling it is just a simple switch or any other professional engineering company that it is pretty simple.

Let's not discuss this any further as this topic is completely not related to the issue.

[quote="Blasto, post:54, topic:85036, full:true"]
guess it would be possible to have a latching circuit to get rid of the mcu, like you said, i don’t know your circuit. i’m just guessing best practice.
[/quote]

We already have solution for this but at the moment to throw away whole stock is not wise so maybe in future we will update it. Right now it works like it should, and many people have no issues with it.
```

---
## \#56 Posted by: DerelictRobot Posted at: 2019-02-22T17:10:40.313Z Reads: 127

```
[quote="3DServisas, post:55, topic:85036"]
Try to explain that to any EE company by telling it is just a simple switch or any other professional engineering company that it is pretty simple.

Let’s not discuss this any further as this topic is completely not related to the issue.
[/quote]

By responding to this, you're inviting discussion. Unless you're saying you just don't want to discuss this within this thread. Either way I'll just say this:

So you don't think I'm entirely talking opinion out my ass: 

I lead hardware development for a device technology company for my day job. I disagree, but the MCU vs static/passive design argument is often a generational one. Personally, I wouldn't consider running a modern 'EE company' without an embedded engineer on staff.
```

---
## \#57 Posted by: 3DServisas Posted at: 2019-02-22T17:13:13.861Z Reads: 125

```
[quote="DerelictRobot, post:56, topic:85036"]
By responding to this, you’re inviting discussion. Unless you’re saying you just don’t want to discuss this within this thread. Either way I’ll just say this:
[/quote]

I am sorry my english is not really good, I am going back to works so I dont have time anymore to discuss this.
```

---
## \#58 Posted by: DerelictRobot Posted at: 2019-02-22T17:14:00.200Z Reads: 125

```
Totally understood! Thanks for taking the time today to discuss your design and products. 

I appreciate it.
```

---
## \#59 Posted by: sayekim Posted at: 2019-02-22T17:36:50.755Z Reads: 130

```
Wow. 

Did you know that the roll to start antispark from @Martinsp also slowly drains the battery?

I bet most do. 

A note stating how much it drains is all I need and then be done with it. 

@Kug3lis @3DServisas your pulleys rock. 

Sure peoples could be posting a bit less arrogant. Let’s admit to being guilty to that or anything else that was offensive or something else and move on.
```

---
## \#60 Posted by: Reelop19 Posted at: 2019-02-22T17:43:55.113Z Reads: 131

```
I should start welding up my 35 degree risers to sell. Looks like some bridges are burning.
```

---
## \#62 Posted by: brenternet Posted at: 2019-02-22T19:01:32.585Z Reads: 126

```
[quote="Kug3lis, post:35, topic:85036"]
Well looks like I will be leaving this forum as everyone here are pussies who get offended on simple things
[/quote]

Don't let the door hit your entitled ass on the way out
```

---
## \#63 Posted by: AlanZhou Posted at: 2019-02-22T19:10:58.125Z Reads: 126

```
Why are you guys so frickin angry?..... most commercial lion products run flat within 30 days anyway, the boosted V1 is a good example if the battery got low because you either left it at 100% and it drained to 0% or you rode it to 40% and left it there for a month then there would have been no way to charge it except forcing current through the motors to charge the a123 cells. (or just send the board to get replaced)

if you don't check up on your eboards often (1-2 weeks) then your asking for a disaster... or if you're super worried just buy one of those storage voltage maintainers.

^or i just sound super dumb
```

---
## \#64 Posted by: Quiles Posted at: 2019-02-22T19:15:05.033Z Reads: 124

```
It's not only esk8 technology is in it's infancy - some vendors are also. And that has nothing to do with cutting edge technology.

The feeling that i'm doing a favor to a vendor buying their highlighly premium/expensive products kills me.
```

---
## \#65 Posted by: meesie Posted at: 2019-02-22T20:37:38.061Z Reads: 118

```
![image|192x128](upload://rIaQlY2dsIQb805u8QXVz7jiBHZ.gif) 

Me, reading this thread.
```

---
## \#66 Posted by: deucesdown Posted at: 2019-02-22T21:12:57.805Z Reads: 117

```
[quote="3DServisas, post:31, topic:85036, full:true"]
This switch is not full disconnect from battery its device which helps you to turn on/off board quicker than other ways.

In normal occasion you will have BMS which would protect your battery from full discharge and full mechanical disconnect from the battery for storing long term.

The device consumes less or around 5mA which in normal uses cases shouldn’t disturb much of your daily usages and in long term you always want to disconnect your battery from any switch as they can not be trusted. What if when you storing your board for long term and randomly MOSFET dies because of manufacturer issue and your 3kW battery pack shorts and burns your apartment to the ground? I wouldn’t trust any device connected to big battery packs without supervision and protections.

Yes it was our mistake of not mentioning this kind of detail, but like I mentioned before in normal configuration and usage this kind of power consumption would not matter much. You can’t have all together.

P.S. Battery disconnect is most important feature in any project it can be car, bike, board or any other electric device u always must have a quick way to disconnect power from everything in case of emergency.
[/quote]

This is the perfect response, and I believe would have made everyone happy (along with a note on the product listing on the website). Thank you!

That temper tantrum that preceded this though... I don't think I need to add anything....
```

---
## \#67 Posted by: Kug3lis Posted at: 2019-02-22T21:16:48.347Z Reads: 113

```
[quote="brenternet, post:62, topic:85036"]
Don’t let the door hit your entitled ass on the way out
[/quote]

I am sorry but urs is already overtaken the whole forum so no way I am going to get hit ;)
```

---
## \#68 Posted by: Blasto Posted at: 2019-02-22T21:51:49.500Z Reads: 114

```
[quote="sayekim, post:59, topic:85036"]
Did you know that the roll to start antispark from @Martinsp also slowly drains the battery?
[/quote]

@martinsp should consider my above circuit in his future revs, he can add a diode branch for the P2S feature.

Power conssumption if the off position should be as low as possible, it is not normal to drain a battery when an item is not in use
```

---
## \#69 Posted by: mishrasubhransu Posted at: 2019-02-22T21:55:26.081Z Reads: 112

```
It has been my observation that people who always offer destructive criticism don't take constructive criticism very well. Oh the irony.
```

---
## \#70 Posted by: deucesdown Posted at: 2019-02-22T22:20:40.381Z Reads: 116

```
[quote="Blasto, post:68, topic:85036"]
Power conssumption if the off position should be as low as possible, it is not normal to drain a battery when an item is not in use
[/quote]

http://www.quickmeme.com/img/62/6246fe3bcc028ed8c8b265039fd34bd26fba0897518b8b669319c5886e890ce8.jpg
```

---
## \#71 Posted by: Reelop19 Posted at: 2019-02-22T22:30:55.239Z Reads: 113

```
Considering the topic is it safe to assume this is how nerds dispute each other?
```

---
## \#72 Posted by: AlanZhou Posted at: 2019-02-22T22:31:20.272Z Reads: 112

```
Yep..... this is why normal people just watch.... i dont understand half of what these guys are talking about.
```

---
## \#73 Posted by: Blasto Posted at: 2019-02-22T22:43:54.815Z Reads: 107

```
Bunch of savages
```

---
## \#74 Posted by: DerelictRobot Posted at: 2019-02-22T22:58:30.918Z Reads: 107

```
[quote="Reelop19, post:71, topic:85036, full:true"]
Considering the topic is it safe to assume this is how nerds dispute each other?
[/quote]

**Autistic screeching intensifies**
```

---
## \#75 Posted by: Sn4pz Posted at: 2019-02-22T23:00:38.339Z Reads: 110

```
No one better for that than Pepe
![](https://i.kym-cdn.com/photos/images/original/000/915/652/b49.gif)
```

---
## \#76 Posted by: ervinelin Posted at: 2019-02-23T01:04:04.264Z Reads: 104

```
I recently swapped out my Spud's antispark and rolled back to an XT90AS after I found out my 10S2P pack had drained to zero when left idle.

I tried two different antispark switches, both leaked or rather consumed power when off.

Both were brand new... Ironically my older generation ones never exhibited this problem thus I never expected this to be an issue.

So yah if the switch is going to consume power when it's off. At least let the consumer know.
```

---
## \#77 Posted by: Martinsp Posted at: 2019-02-23T01:19:22.105Z Reads: 103

```
Hello everyone, 
I just got back from the shop and read my emails, been a bit too busy past few days. I will reply to all my PMs in the morning.
I will also do the measurements, Im planning to measure what I would consider the worst case scenario of what you described. Measure the input current/power from the battery while the switch is OFF and the output of the switch is shorted to include leakage current. If youd like to see something measured let me know so I can do it...

The switch will consume power all the time, that simply is because there is a micro-controller that needs to be powered so it can respond to the input (push button for example). The only way you could get absolute zero current is by using relays because mosfets have leakage current when OFF and no active micro-controller just a push button that when closed energizes the coils. I was thinking about such a design because it is simple and pretty bullet proof as far as the switch goes but it would be very bulky for electric skateboard needs...

EDIT: just measured it here are the results: https://www.electric-skateboard.builders/t/push-to-start-switch-out-now/60879/195?u=martinsp
```

---
## \#78 Posted by: nuttyjeff Posted at: 2019-02-23T01:51:00.560Z Reads: 101

```
[quote="Martinsp, post:77, topic:85036"]
The only way you could get absolute zero current is by using relays because mosfets have leakage current when OFF and no active micro-controller just a push button that when closed energizes the coils. I was thinking about such a design because it is simple and pretty bullet proof as far as the switch goes but it would be very bulky for electric skateboard needs…
[/quote]

I think the ideal solution would be something like the unity has. A momentary push button antispark solution with negligible power consumption.

[quote="nuttyjeff, post:12, topic:85036"]
It’s not a matter of whether it consumes power, it’s a matter of how much it consumes and what an acceptable limit is.
[/quote]

^ I don't know the ins and outs of how this works, but I'd implore the antispark designers of the community to work towards this implementation.  I mean no offence to anyone, i simply **think** that the current AS switches can be improved, seeing as there is already one out there that does the job perfectly. (The only issue is that you have to buy 2 vescs along with it and for those running a 1WD build, it's not a viable option.)

As for the current AS switches that consume a noticable about of power, it'll be nice to leave a note on your website (or wherever) to indicate its power drain. There are some with small battey packs (think 20 cells or lesser) who use your anti-sparks, and 0.5W or similar of power drain is quite unacceptable. (I'm not saying Martinsp's switch drains 0.5W, will wait on his reply on the power drain of his switch)

@Martinsp Thanks for steping into the discussion, would love to hear your thoughts on it.
```

---
## \#79 Posted by: ervinelin Posted at: 2019-02-23T02:06:56.420Z Reads: 99

```
Is this consumption of power only for the PTS style switches only or even the older generation ones?

I have two of your switches. The old one with the big automotive fuse and a newer generation (non-PTS). Old one works fine. New one killed my 10S2P apparently.
```

---
## \#80 Posted by: mmaner Posted at: 2019-02-23T04:04:53.447Z Reads: 93

```

```

---
