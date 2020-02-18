# Making the A200S 16s 200A, high powered VESC HW6

### Replies: 51 Views: 3162

## \#1 Posted by: uigiroux Posted at: 2018-03-30T14:51:42.863Z Reads: 286

```
On the vesc-project.com website they have a page that details different builds using the VESC software. 
This link shows all the ones that are being worked on.
https://vesc-project.com/forum/6

The first two look the most promising, especially the very first one.  This thread is about that first one for the A200S 16S 200A.  This is the link specifically for the A200S 16s 200A:
https://vesc-project.com/node/339

![Screenshot_20180330-091101|408x500](upload://zemTaKyzTv7tOujteaxqvs5S8Or.jpg)
![Screenshot_20180330-091209|473x500](upload://rWjajziVLmEK6kfr24jci6RWhlg.jpg)

One of the first submissions detailing what the project is has a link to the schematics and BOM files so one could reproduce this if they wanted. 
https://github.com/TechAUmNu/A200S

These are being made in small batches, I believe they have 20 made so far and are selling them for £400, or $561.96, and will increase to £450, or $631.84, so they're quite expensive and only getting more so... 

![Screenshot_20180330-092135|538x500](upload://5dNnAMZzxW9dpXROVJ6wL4XLudo.jpg)

With the recent success of the ESCape and B-Box, which are produced and sold for more than half, and in the DIY kits, almost a quarter the cost of the VESC 6, I was wondering if anyone might be able to try and reproduce this high powered VESC, which would allow powering motors up to 16s, and from private messages I've had with the maker, he says it is actually capable of even 18s, but a bit safer in 16s, but with more testing, and possibly some small modifications,  it could be made to support up to 18s regularly.

![Screenshot_20180330-092110|497x500](upload://xZGboShIEgCS1YpzJrSYDEKitkf.jpg)

https://youtu.be/MMx283VQcVY

I know the majority of the DIY community has no need for an ESC that goes above 12s, but that doesn't mean there aren't any who do want this, but for most of us, paying that kind of money for just one ESC simply isn't feasible...  Now I certainly am not able to make one of these, let alone even understand the schematics, but I have to believe that if it's possible to make a HW6 VESC for the prices that our independent developers have shown it's possible to do, well then I have to believe that the same applies to this higher powered VESC.  Now I'm sure this one will be a bit more expensive than the ESCape or B-Box, but I am hoping that the amount of savings that is potentially possible by remanufacturing this in the same way as the ESCape and B-Box were developed will make this something that many of us could soon consider and not break the bank getting one.

If we're able to have these types of high powered ESC's and thus could use much more powerful motors like an 80100 for example, well, I think that would be a big step forward in this hobby.  You could have one 80100 with a shaft long enough to power both wheels, thus only requiring one ESC.  That would save you money, and simplify setup because you wouldn't have to fiddle with connecting two ESC's and require less cable as well.

Anyways, I just thought I'd bring this up and see if anyone else is interested in something like this?  I would love to have a few of these, and I don't think I'm the only one.  :slight_smile:
```

---
## \#2 Posted by: Hummie Posted at: 2018-03-30T15:24:57.551Z Reads: 239

```
seem pretty big and it's rare I hear of people having temp shut-downs with standard vescs and even if it did happen I think you could just add a better airflow or heatsink and put out much more power.  it's not 16s, which is pretty nice, but otherwise seems overkill.  I haven't hit an overtemp shut=down yet.  

 you can use a 80mm motor with a standard vesc and likely get far and fast without a need for more power I bet
```

---
## \#3 Posted by: ducktaperules Posted at: 2018-03-30T15:26:40.303Z Reads: 231

```
The heatsync design is great. I like the idea of stacking them and also the cutouts for the capacitors.
```

---
## \#5 Posted by: uigiroux Posted at: 2018-03-30T15:40:26.461Z Reads: 222

```
Well yes you can power an 80mm diameter motor with 12s and a regular VESC, but they are rated up to 18s, so to get the full power and potential, I'd want to power it that way.

I'm mainly bringing this up in response to what you described Derek's board was powered by and I thought he had some sort of high powered ESC for one of his builds, most likely that one it sounds like..
```

---
## \#6 Posted by: uigiroux Posted at: 2018-03-30T15:42:26.565Z Reads: 212

```
Also the things your saying that don't happen with certain motors is cause we're only using up to a certain size motor and only able to power the big ones not to their full potential.  If we had this as an option there'd be a bunch of new builds with people using much larger motors I imagine..
```

---
## \#7 Posted by: Hummie Posted at: 2018-03-30T15:43:38.065Z Reads: 204

```
the voltage rating of motors has more to do with it's bearings and how fast it can spin.  the insulation on the actual magnet wire will do far more.   often they will put a voltage limit but it more so has to do with the possibly high currents that would come from such a high voltage.  so the voltage limits are not real voltage limits

I wonder what the motor amp and battery amp limit setting are on that big vesc variant you posted.
```

---
## \#8 Posted by: uigiroux Posted at: 2018-03-30T15:45:17.008Z Reads: 196

```
Oh, well still I would like to have these available.. Lol
```

---
## \#10 Posted by: Hummie Posted at: 2018-03-30T15:46:33.143Z Reads: 189

```
I think with the right lipos you could get that power
```

---
## \#11 Posted by: uigiroux Posted at: 2018-03-30T15:48:31.604Z Reads: 189

```
I'm not saying we need this for that specific reason, just, I'd like to be able to go 14s on a few things and can't with the current ESC's.  That's pretty much why I brought this up.  So if you want to power a motor to a certain voltage, you can.
```

---
## \#13 Posted by: Acido Posted at: 2018-03-30T16:01:08.552Z Reads: 190

```
Get a bigger battery!
```

---
## \#14 Posted by: uigiroux Posted at: 2018-03-30T16:06:49.102Z Reads: 191

```
Jesus guys, if your just going to say rude stuff, you can kindly not comment.  Also saying "not trying to be rude" is kinda pointless if the very next thing your say is rude!  It doesn't give you a blanket of protection making others think "oh well he said 'not trying to be rude' so he isn't being rude, he's a nice guy".  Seriously like WTF is your problem. I've been skating more than half my life which for some members is longer than they've been alive.  This is my first build I'm working on now and I'm simply asking some questions, none of which I could find any answers in the search option.  So I terribly sorry if this thread has somehow upset your day and ruined your life somehow.  Man, any time I ask a question someone has to say some ignorant garbage like that.  Really productive contribution let me just say!  I don't go around belittling new Esk8 people just because they asked a question that I may think should be obvious.  It's called common courtesy, if you can't abide by this simple little practice of being polite, then don't comment.
```

---
## \#15 Posted by: uigiroux Posted at: 2018-03-30T16:11:44.343Z Reads: 181

```
Also I was just using a 80xxx motor as an example.  I mean we could run a 6384 at 14s.
```

---
## \#17 Posted by: uigiroux Posted at: 2018-03-30T16:33:18.423Z Reads: 180

```
Thanks guys real mature...
```

---
## \#19 Posted by: uigiroux Posted at: 2018-03-30T16:36:54.352Z Reads: 179

```
Regardless, your comments have nothing to do with the topic.
```

---
## \#20 Posted by: Kug3lis Posted at: 2018-03-30T16:41:13.496Z Reads: 177

```
I mean I was kinda similar bigger power all the better, but nowadays I am not even using the whole potential of my 6384 motors cause it's way too much power to handle ;)
```

---
## \#21 Posted by: uigiroux Posted at: 2018-03-30T16:42:18.037Z Reads: 183

```
What kind of setup are you running them on?  Battery size, belt /gear?
```

---
## \#22 Posted by: Kug3lis Posted at: 2018-03-30T16:42:40.807Z Reads: 187

```
12S 24Ah 65C 5:1 170kv inner gear drive train :)
```

---
## \#23 Posted by: uigiroux Posted at: 2018-03-30T16:44:44.782Z Reads: 174

```
Nice!  What kinda top speed does that get you??  I'm really interested in these inner gear direct drives.
```

---
## \#24 Posted by: uigiroux Posted at: 2018-03-30T16:46:16.174Z Reads: 178

```
Yeah I think that design is really clever, especially for not being fully sealed.
```

---
## \#25 Posted by: uigiroux Posted at: 2018-03-30T16:49:54.194Z Reads: 172

```
Couldn't some of those obscenely powerful tattu lipos provide that kind of power?
https://www.genstattu.com/22000mah-lipo.html
```

---
## \#26 Posted by: treenutter Posted at: 2018-03-30T17:02:02.487Z Reads: 176

```
[quote="uigiroux, post:14, topic:50654"]
if your just going to say rude stuff, you can kindly not comment
[/quote]


Yes, this^

There is always a way to frame a comment to be constructive instead of insulting...

For example, "do you even skate?" could be reframed as : "Based on my experience skating, I've never needed xyz. Could you explain how xyz will be useful to you?"

Online communication is different than in-person communication; it's hard to convey the humor in a comment that is summarily negative. This works IRL w your voice or with facial expressions and body language. It doesn't work here.

@GrecoMan @Surfer give it a try; challenge yourselves to frame your comments in a way that is respectful to the OP. Even if it seems like the comment is forced from your perspective. You won't get flagged as often and the discussion will be better.
```

---
## \#27 Posted by: Namasaki Posted at: 2018-03-30T17:16:21.564Z Reads: 168

```
[quote="uigiroux, post:25, topic:50654"]
Couldn’t some of those obscenely powerful tattu lipos provide that kind of power?
[/quote]

@PatRocks uses the high capacity Tattu Lipos and has had really good results. 
He flys up some crazy steep hills and has minimal sag. And he was only running 8s at the time!
```

---
## \#28 Posted by: uigiroux Posted at: 2018-03-30T17:19:41.619Z Reads: 165

```
Wow!  Just one 8s or 2 4s?  They are really expensive though, lol.  Seems like they're probably worth it though!
```

---
## \#29 Posted by: Namasaki Posted at: 2018-03-30T17:26:49.652Z Reads: 154

```
He was running two 4s in series but now he has added another 4s and is running 12s!
I’ll bet he would be very interested in a 16s 200a Vesc.
```

---
## \#30 Posted by: uigiroux Posted at: 2018-03-30T17:30:10.684Z Reads: 157

```
Yes!  Someone else agrees, lol.  I knew I wasn't the only one who could be interested in this!  How many mAh are each of his 4s? I'm wondering what 12s lion configuration that would be comparable to..?
```

---
## \#31 Posted by: PatRocks Posted at: 2018-03-30T17:40:07.231Z Reads: 156

```
I'm running the 22000mAh 25c 4s blocks x3. I got them used, from a guy with a good reputation on eBay for around 150$ each. They are excellent, I charge about once a month, with a hobby charger😎. Couldn't be happier with them, so much so that when they eventually get old and crotchety I'm going to shell out the $400+ each to replace them.
```

---
## \#32 Posted by: PatRocks Posted at: 2018-03-30T17:45:34.964Z Reads: 155

```
It would take a lot. And it would be bigger and heavier than the lipo pack.
```

---
## \#33 Posted by: uigiroux Posted at: 2018-03-30T17:48:44.788Z Reads: 159

```
Wow so you have a $1200 battery!,? Impressive.
```

---
## \#34 Posted by: PatRocks Posted at: 2018-03-30T17:56:01.515Z Reads: 162

```
Sorta. They're not what a brand new lipo is like, but discharging from 4.1v/c to 3.7 I'm only seeing about a 0.1 voltage difference between the cells. Aaand that's after accidentally over discharging down to 2.73 v/c, which is usually fatal for lipos.

As I mentioned, I got them for $450 altogether. Was a steal
```

---
## \#35 Posted by: Hummie Posted at: 2018-03-30T18:04:25.675Z Reads: 152

```
tattu told me they sell their 2nd class stuff to hobbyking
```

---
## \#37 Posted by: PatRocks Posted at: 2018-03-30T18:05:51.980Z Reads: 153

```
I almost forgot, @deucesdown got a few from the same guy, in the same condition, and did a bunch of science on them. We talked about it in my build thread:
http://www.electric-skateboard.builders/u/deucesdown
```

---
## \#39 Posted by: PatRocks Posted at: 2018-03-30T18:08:08.785Z Reads: 148

```
Que?? As in, at a second class quality discount?? I  might be interested...
```

---
## \#41 Posted by: uigiroux Posted at: 2018-03-30T18:11:45.343Z Reads: 148

```
Dude, I didn't once say I needed an 18s board, I said it would nice to have the option.  Others seem to agree, so why do you have to bring this up again.
```

---
## \#42 Posted by: uigiroux Posted at: 2018-03-30T18:12:19.891Z Reads: 148

```
Once again, can we stay on topic?
```

---
## \#43 Posted by: Blitz Posted at: 2018-03-30T18:13:04.045Z Reads: 148

```
Yo we not the enemies act like this and nobody will care about your topic It will go cold.
```

---
## \#44 Posted by: Deckoz Posted at: 2018-03-30T18:14:17.166Z Reads: 147

```
The only reason for 18s would be a mountain board with big ass tires(10"+), with a sub 50kV motor on heavy reduction to climb steep ass hillls, or dune skating. 

Otherwise, what's the point?
```

---
## \#45 Posted by: ZackoryCramer Posted at: 2018-03-30T18:15:16.360Z Reads: 145

```
Is smaller kv(with appropriate gear) always better for higher torque/speed? Is there an optimal ratio?
```

---
## \#46 Posted by: PatRocks Posted at: 2018-03-30T18:16:13.455Z Reads: 143

```
Electric surfboards!!
```

---
## \#47 Posted by: uigiroux Posted at: 2018-03-30T18:17:27.505Z Reads: 143

```
I never said you were the enemies, but you guys keep like making fun of me because what, I haven't built a Esk8 yet, and rather than sink to that level and insult back, I simply ask that at stay on topic and if your going to be rude then kindly don't bother commenting.  This is hardly an issue that I've created.  If you guys keep bringing it up and then an admin comes and agrees with me and says to be polite and stay in topic, I think that just further backs me up.
```

---
## \#48 Posted by: uigiroux Posted at: 2018-03-30T18:18:04.761Z Reads: 142

```
Yes I've been looking into those and e-foils and they do use that much power.
```

---
## \#49 Posted by: Deckoz Posted at: 2018-03-30T18:19:25.843Z Reads: 142

```
Plus y'all gotta remember, human impedence gives us right around ~48v and under being safe to touch.

Those pushing 12s+ have the possibility of shock hazard.

Your asking for a system capable of killing you while performing maintenance... 

Just reminding you of a hazard to be aware of.. lol
```

---
## \#51 Posted by: GrecoMan Posted at: 2018-03-30T18:22:49.388Z Reads: 136

```
what about me?
```

---
## \#53 Posted by: uigiroux Posted at: 2018-03-30T18:24:49.785Z Reads: 139

```
Ok, sorry if I wasn't specific, but I was also trying not to further stray from the topic by naming people individually.  REGARDLESS, can we move forward and quit with the pissing contest, member bashing?  Some people here actually are trying to discuss the topic, so please, can we just focus on the topic...
```

---
## \#54 Posted by: Deckoz Posted at: 2018-03-30T18:25:41.867Z Reads: 141

```
(post withdrawn by author, will be automatically deleted in 24 hours unless flagged)
```

---
## \#56 Posted by: uigiroux Posted at: 2018-03-30T18:27:20.921Z Reads: 143

```
Ok good job guys, super mature.  Peace.
```

---
## \#57 Posted by: Hummie Posted at: 2018-03-30T18:28:45.194Z Reads: 143

```
I meant that tattu told me they sell directly but their second class stuff ends up at hobbyking.  if you buy from them directly in bulk you can get a discount but their stuff is expensive as you know
```

---
## \#60 Posted by: Hummie Posted at: 2018-03-30T18:31:24.567Z Reads: 148

```
or I meant to put that post in the other thread.

but in this thread....the vesc was designed for eboards.  you can put it on an eboard or with this thing a bike or whatever.   considering how many vescs blow up maybe this is the safest bet for a board.
```

---
## \#61 Posted by: Kug3lis Posted at: 2018-03-30T18:32:30.965Z Reads: 146

```
I would like to build like 48S ESC with 20A capability for decent 4kW/motor setup it would be really efficient and nano size with no heatsinks required but also ducking deadly as 200VDC is deadly. Of course, this would require ~50KV motor and I still have no idea how motor would react to 200VDC :) All the components would look like small XT60 connectors, 3mm bullets :D
```

---
## \#62 Posted by: b264 Posted at: 2018-03-30T18:32:38.811Z Reads: 150

```
[quote="uigiroux, post:42, topic:50654, full:true"]
Once again, can we stay on topic?
[/quote]

I'm sorry, but this is hilarious
```

---
## \#64 Posted by: treenutter Posted at: 2018-03-30T19:08:12.202Z Reads: 139

```

```

---
## \#65 Posted by: treenutter Posted at: 2018-03-30T19:09:32.582Z Reads: 140

```
@Deckoz @GrecoMan @Surfer @uigiroux there seems to be a lot of confusion here so I'm locking the thread until I can sort out 13 flags just created. Let's try to keep civil.
```

---
