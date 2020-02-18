# I screwed up and bought a Flipsky&hellip;now what?

### Replies: 92 Views: 1251

## \#1 Posted by: kchxaz Posted at: 2019-04-03T22:43:58.137Z Reads: 354

```
Against the advice of nearly everyone on this site I did a boneheaded move and bought a Flipsky 6.6 FSESC (not to be confused with the Flipsky 6.6 FSESC Plus) anyways.

I have to live with the repercussions of bad buy so please don't beat this dead horse. In short, my goal was to build a 4WD board and the Flipsky website for the 6.6 FSESC mentions nothing about being unable to support 4WD (but go the the 6.6 'plus' page and it mentions 4WD support), needless to say I spend $550 on FSESC that are useless to me now for my project but here I am trying to salvage something form it which leads me to my question:
 
I have used the VESC tool (even bought the bronze edition) to program and setup the ESC to connect and ride (setup went smoothly) but when I connect and try to ride the board it won't go. It just struggles to do anything but when there is no weight on it, it bolts like a cheetah- WTF?

I am either the dumbest person ever or the Flipsy FSESC is shit
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-04-03T22:47:33.761Z Reads: 342

```
did you get two dual 6.6's or 4 single 6.6's? they all support 4wd if you know what your talking about lol

with 2 x dual 6.6's you use split ppm

with 4x 6.6's you do canbus turning 4 esc basically into 2 dual esc's than you use split ppm
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-04-03T22:48:43.273Z Reads: 338

```
[quote="kchxaz, post:1, topic:89291"]
I am either the dumbest person
[/quote]

i think this quote might be accurate

anyways you prob have your board on sensorless mode which requires a kick off
```

---
## \#4 Posted by: mishrasubhransu Posted at: 2019-04-03T22:55:35.139Z Reads: 318

```
These is nothing wrong with FSESC6.6 except minor voltage sensing issue.
```

---
## \#5 Posted by: kchxaz Posted at: 2019-04-03T23:33:48.638Z Reads: 304

```
No, I have not tried a kick-off. Didn't think it was necessary.

I thought that was the purpose of these types of VESC's - to allow sensorless (which is the type of motor I am using) motors a smooth start-up?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-04-03T23:40:08.207Z Reads: 294

```
yes sensorless requires kick off sensored does not

smooth meaning the acceleration is not jerky
```

---
## \#7 Posted by: kchxaz Posted at: 2019-04-03T23:40:22.417Z Reads: 285

```
And minus the fact that the 6.6 does not support 4WD and the website focusing on the product fails to mention this - that's a pretty big fuck-up. I'm out $550 because of it.
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-04-03T23:48:40.859Z Reads: 278

```
But it does work though

I just cannot tell you how

Instead, please have [this](https://www.electric-skateboard.builders/search)
```

---
## \#9 Posted by: Bobby Posted at: 2019-04-03T23:51:21.154Z Reads: 261

```
Absolutely works.... so does the search button.
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-04-03T23:51:23.256Z Reads: 263

```
[quote="kchxaz, post:7, topic:89291"]
And minus the fact that the 6.6 does not support 4WD
[/quote]

it does support 4wd

you just gotta know how to do it, its preety easy if you were to do a 5 min search
```

---
## \#11 Posted by: b264 Posted at: 2019-04-03T23:51:38.680Z Reads: 255

```
The Flipsky 6.6 FSESC definitely supports 4 wheel drive.

There are many ways to do this.  I recommend having a separate remote receiver for each ESC/motor but there are other ways like Split "PPM" (PWM) and CANBUS.
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-04-03T23:52:01.530Z Reads: 242

```
Feeling artsy, made it a haiku 😂😂

I get bored telling people to use the search function the same way everytime :roll_eyes:
```

---
## \#13 Posted by: Bobby Posted at: 2019-04-03T23:53:52.005Z Reads: 237

```
Aren’t you missing a syllable in the second line?
5-7-5???
```

---
## \#14 Posted by: kchxaz Posted at: 2019-04-03T23:54:27.189Z Reads: 231

```
Please understand the purpose of the post before responding. Thank you
```

---
## \#15 Posted by: Sn4pz Posted at: 2019-04-03T23:55:13.923Z Reads: 226

```
Heh got me. I changed it like 4 times bc I wasn't happy with it

Got sloppy on the last one 🤷
```

---
## \#16 Posted by: Dirt_Bag Posted at: 2019-04-03T23:55:26.019Z Reads: 220

```
well it does show the entire pin out diagram for them.... you could have looked at that
```

---
## \#17 Posted by: Bobby Posted at: 2019-04-03T23:55:35.854Z Reads: 223

```
[quote="Sn4pz, post:8, topic:89291"]
But it does work though

But I will not tell you how

Instead, please have [this ](https://www.electric-skateboard.builders/search)
[/quote]
I think i like your haiku lol. Its a keeper
```

---
## \#18 Posted by: kchxaz Posted at: 2019-04-03T23:56:28.038Z Reads: 220

```
It DO NOT support 4WD per Flipsky. To those of you saying do a search. I did, go learn how to spell.
```

---
## \#19 Posted by: Sn4pz Posted at: 2019-04-03T23:56:57.676Z Reads: 220

```
https://media.tenor.com/images/a4ec68cca56d922d97fc0f8eeadc460d/tenor.gif
```

---
## \#20 Posted by: Bobby Posted at: 2019-04-03T23:57:18.124Z Reads: 216

```
But it so do!!!! Because you not know how no means it no work!!!
```

---
## \#21 Posted by: threebysix Posted at: 2019-04-03T23:58:24.466Z Reads: 210

```
But it does. The answer to how you do it is literally in the first reply by @AlanZhou  LOL
```

---
## \#23 Posted by: AlanZhou Posted at: 2019-04-04T00:01:04.420Z Reads: 204

```
[quote="kchxaz, post:22, topic:89291"]
dumb ass
[/quote]

whoah there
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-04-04T00:01:14.275Z Reads: 203

```
if you want this to go bad i will help you do so.
```

---
## \#25 Posted by: AlanZhou Posted at: 2019-04-04T00:01:31.595Z Reads: 206

```
maybe if you were smart enough to use the search bar your would have found your answer

and apparently dumb enough to think one esc can do 4wd

[quote="AlanZhou, post:2, topic:89291"]
with 2 x dual 6.6’s you use split ppm

with 4x 6.6’s you do canbus turning 4 esc basically into 2 dual esc’s than you use split ppm
[/quote]

where do you see i say one esc can handle 4wd?

who ever said this?
[quote="kchxaz, post:18, topic:89291"]
It DO NOT support 4WD per Flipsky
[/quote]
```

---
## \#26 Posted by: Bobby Posted at: 2019-04-04T00:03:07.011Z Reads: 197

```
Well do what you feel, don’t expect people to help if you cant help yourself.i searched flipsky 4wd and found tons of info including people that have used them and pictures.  believe what you want, my dumbass knows how to research before making false assumptions ✌🏼
```

---
## \#27 Posted by: AlanZhou Posted at: 2019-04-04T00:04:39.435Z Reads: 196

```
atleast i am a dumbass and i know the "basics" of vesc
```

---
## \#28 Posted by: morrisxyz Posted at: 2019-04-04T00:52:11.704Z Reads: 191

```
Makes post asking for help.
Receives help.
Gets mad and insults people.
Win???
```

---
## \#29 Posted by: AlanZhou Posted at: 2019-04-04T00:53:06.058Z Reads: 186

```
nobody wants to even answer these simple questions in the first place :joy:
```

---
## \#30 Posted by: SeanHacker Posted at: 2019-04-04T01:00:34.378Z Reads: 189

```
[quote="morrisxyz, post:28, topic:89291, full:true"]
Makes post asking for help. Receives help. Gets mad and insults people. Win???
[/quote]

To be fair. The 3rd post was this... 
![dumbshitkid|690x247](upload://dZUa4qescMWSD0VMWQNXSM7VEz7.png) 

After asking for help when help is obviously needed I would get pissed in return too. This dumbshit high school bully attitude is getting old around here.
```

---
## \#31 Posted by: SeanHacker Posted at: 2019-04-04T01:02:10.863Z Reads: 182

```
[quote="AlanZhou, post:29, topic:89291"]
nobody wants to even answer these simple questions in the first place :joy:
[/quote]

Are you really this fucking pathetic dude? You should knock it off already. Or does it make you feel better picking on someone asking for help?
```

---
## \#32 Posted by: AlanZhou Posted at: 2019-04-04T01:03:46.634Z Reads: 176

```
[quote="SeanHacker, post:31, topic:89291"]
Or does it make you feel better picking on someone asking for help?
[/quote]

nah im just mad at the fact he called all the people who were helping him dumbasses

^since he called me one im gonna be like one for a sec.
```

---
## \#33 Posted by: AlanZhou Posted at: 2019-04-04T01:04:42.048Z Reads: 173

```
[quote="kchxaz, post:22, topic:89291, full:true"]
I’m not going to argue with your dumb ass. The manufacturer says it doesn’t work. If you can prove otherwise, please, be my guest.
[/quote]

@SeanHacker

i answered him queston if you check post 1
```

---
## \#34 Posted by: SeanHacker Posted at: 2019-04-04T01:06:24.094Z Reads: 176

```
[quote="AlanZhou, post:32, topic:89291"]
nah im just mad at the fact he called all the people who were helping him dumbasses
[/quote]

[quote="kchxaz, post:1, topic:89291"]
I am either the dumbest person ever
[/quote]

[quote="AlanZhou, post:3, topic:89291"]
i think this quote might be accurate
[/quote]

Yep. I can read. The 3rd post here was from you being a total dickhead with no morals at all. I'd get pretty salty too. Give the noobs a break already.
```

---
## \#35 Posted by: AlanZhou Posted at: 2019-04-04T01:07:00.756Z Reads: 166

```
it was a joke and he oviously understood it

[quote="kchxaz, post:5, topic:89291, full:true"]
No, I have not tried a kick-off. Didn’t think it was necessary.

I thought that was the purpose of these types of VESC’s - to allow sensorless (which is the type of motor I am using) motors a smooth start-up?
[/quote]

^his post right after i posted
```

---
## \#37 Posted by: AlanZhou Posted at: 2019-04-04T01:08:40.353Z Reads: 160

```
i was not being pathetic until he called everyone helping him a dumbass
```

---
## \#38 Posted by: SeanHacker Posted at: 2019-04-04T01:08:43.565Z Reads: 160

```
He passed up your comment up and took the moral high ground which is what anyone with a basic 4th grade intellect would do.
```

---
## \#39 Posted by: AlanZhou Posted at: 2019-04-04T01:09:49.958Z Reads: 157

```
am i supposed to add a thousand laughing faces to  symbolize that i was joking?
```

---
## \#40 Posted by: SeanHacker Posted at: 2019-04-04T01:10:06.112Z Reads: 158

```
He didn't call everyone a dumbass. He called @Bobby a dumbass. Fortunately I can read pretty well dude. ;)

No need to play Captain Save a Hoe here. I have faith in @Bobby that he can take care of himself pretty well as far as I've seen. The gang up shit looks ridiculous.
```

---
## \#41 Posted by: KaramQ Posted at: 2019-04-04T01:10:26.458Z Reads: 156

```
I hate to buzz in, but why is there always a heated argument at the beginning of each month
```

---
## \#42 Posted by: AlanZhou Posted at: 2019-04-04T01:10:42.434Z Reads: 154

```
[quote="kchxaz, post:18, topic:89291, full:true"]
It DO NOT support 4WD per Flipsky. To those of you saying do a search. I did, go learn how to spell.
[/quote]

also said this.... i never said one esc could support 4wd.
```

---
## \#43 Posted by: chrischo1996 Posted at: 2019-04-04T01:10:46.955Z Reads: 157

```
Uhm guys? We're all on the same side here, building awesome electric death machines. Let's be nice to the newcomers, as well as everyone else.
```

---
## \#44 Posted by: mishrasubhransu Posted at: 2019-04-04T01:11:57.541Z Reads: 156

```
Problem is when the newcomers have the know-it-all attitude. They don't want to learn, they want things done for them.
```

---
## \#45 Posted by: AlanZhou Posted at: 2019-04-04T01:12:00.751Z Reads: 158

```
[quote="SeanHacker, post:40, topic:89291"]
No need to play Captain Save a Hoe here. I have faith in @Bobby that he can take care of himself pretty well as far as I’ve seen. The gang up shit looks ridiculous.
[/quote]

sure whatever you like :wink:
```

---
## \#46 Posted by: AlanZhou Posted at: 2019-04-04T01:12:34.651Z Reads: 157

```
[quote="mishrasubhransu, post:44, topic:89291, full:true"]
Problem is when the newcomers have the know it all attitude. They don’t want to learn they want things done for them.
[/quote]

@SeanHacker everyone tried to explain to him that 4wd was possible and i even stated all the ways possible
```

---
## \#47 Posted by: SeanHacker Posted at: 2019-04-04T01:12:54.774Z Reads: 151

```
[quote="AlanZhou, post:45, topic:89291"]
sure whatever you like :wink:
[/quote]

I'm pretty sure most here would like. ;)
```

---
## \#48 Posted by: AlanZhou Posted at: 2019-04-04T01:13:06.947Z Reads: 147

```
can we close this thread

tag mmaner?

oh wait you cant close discussion threads
```

---
## \#49 Posted by: AlanZhou Posted at: 2019-04-04T01:15:38.160Z Reads: 144

```
[quote="SeanHacker, post:31, topic:89291"]
Are you really this fucking pathetic dude? You should knock it off already. Or does it make you feel better picking on someone asking for help?
[/quote]

next time i also just go tell the guy to use the search bar :joy:
```

---
## \#50 Posted by: SeanHacker Posted at: 2019-04-04T01:19:00.928Z Reads: 146

```
[quote="AlanZhou, post:49, topic:89291"]
next time i also just go tell the guy to use the search bar :joy:
[/quote]

Why? Seems ridiculous
```

---
## \#51 Posted by: AlanZhou Posted at: 2019-04-04T01:22:17.618Z Reads: 143

```
questions that have been answered thousands of times
```

---
## \#52 Posted by: AlanZhou Posted at: 2019-04-04T01:23:25.298Z Reads: 143

```
i typed in 4wd flipsky and this popped up near the top

https://www.electric-skateboard.builders/t/4wd-builder-room/79306/104
```

---
## \#53 Posted by: Bobby Posted at: 2019-04-04T01:26:03.217Z Reads: 142

```
Who you callin a hoe!?!?
```

---
## \#54 Posted by: AlanZhou Posted at: 2019-04-04T01:26:23.768Z Reads: 142

```
you replied to the wrong person haha
```

---
## \#55 Posted by: Bobby Posted at: 2019-04-04T01:27:27.887Z Reads: 144

```
Sorry lol. @SeanHacker. Who you callin a hoe!?! You dont know me!!!
```

---
## \#56 Posted by: SeanHacker Posted at: 2019-04-04T01:28:27.245Z Reads: 145

```
[quote="AlanZhou, post:51, topic:89291, full:true"]
questions that have been answered thousands of times
[/quote]

[quote="AlanZhou, post:52, topic:89291"]
i typed in 4wd flipsky and this popped up near the top

![|20x20](/user_avatar/www.electric-skateboard.builders/mackann/40/130566_2.png) [4WD builder room](https://www.electric-skateboard.builders/t/4wd-builder-room/79306/104) [General Discussion](/c/General-discussion)
[/quote]

Nice. Good on you dude. In the real world sometimes people are new to a forum or forums in general. They don't even know what a search bar or searching is. Or maybe emotions of a first purchase happens. Or maybe they search under the wrong search terms and can't find what they're looking for. Or something else. These threads only become useful if we help. 

No hard feelings at all on my end dude. I like you. I think I've just had it with the rude shit going on around the forums lately. Just remember when you were brand new. It might help the empathy levels a bit. ;)
```

---
## \#57 Posted by: SeanHacker Posted at: 2019-04-04T01:28:51.318Z Reads: 143

```
[quote="Bobby, post:55, topic:89291, full:true"]
Sorry lol. @SeanHacker. Who you callin a hoe!?! You dont know me!!!
[/quote]

Do I need to tho? :smiley:
```

---
## \#58 Posted by: Bobby Posted at: 2019-04-04T01:29:32.504Z Reads: 140

```
@AlanZhou To be fair, sean has a point. Ive been called worse and couldn’t care less. Guys calls me dumb but says he spent all this money for something that doesn’t work but it clearly does 🤙🏼
```

---
## \#59 Posted by: AlanZhou Posted at: 2019-04-04T01:29:35.363Z Reads: 141

```
[quote="SeanHacker, post:56, topic:89291"]
I think I’ve just had it with the rude shit going on around the forums lately. Just remember when you were brand new. It might help the empathy levels a bit. :wink:
[/quote]

haha its fine, sry got a bit pissed when he spit the term dumbass out
```

---
## \#60 Posted by: Bobby Posted at: 2019-04-04T01:30:24.431Z Reads: 138

```
@AlanZhou My hero!!😍😍
```

---
## \#61 Posted by: AlanZhou Posted at: 2019-04-04T01:31:10.767Z Reads: 134

```
[quote="SeanHacker, post:57, topic:89291"]
Do I need to tho? :smiley:
[/quote]

now im wondering though where he got all the money to buy a lot of parts in a previous thread :wink:
```

---
## \#62 Posted by: AlanZhou Posted at: 2019-04-04T01:31:34.110Z Reads: 130

```
im blame everything on my state test, that shit pissed me off 9 short responses and 2 extended responses
```

---
## \#63 Posted by: Bobby Posted at: 2019-04-04T01:31:59.807Z Reads: 124

```
$5 dollars to see it...
$10 dollars to touch it...
```

---
## \#64 Posted by: AlanZhou Posted at: 2019-04-04T01:32:16.304Z Reads: 124

```
its a scam it cant be that cheap, im suspicious now :roll_eyes::face_with_raised_eyebrow::thinking:
```

---
## \#65 Posted by: skatardude10 Posted at: 2019-04-04T01:36:04.033Z Reads: 127

```
I'm thinking about how these encounters can go better... 

At the turn of the dumbass statement, I'd imagine asking for clarification on the methods discussed would go over much better. Given a good search, I've never seen requests for clarification go down negatively.
```

---
## \#66 Posted by: morrisxyz Posted at: 2019-04-04T02:08:31.186Z Reads: 125

```
Write a bot that automatically replies with search results based on popular keywords.
```

---
## \#67 Posted by: youseekcota Posted at: 2019-04-04T02:52:14.701Z Reads: 131

```
Check out my build, it's rock solid Awd by four FVESCs. I learned from mistakes others had made, made a bunch of mistakes myself and came up with a novel solution.

Love my FVESCs. What's up with the attitude? Look, you don't just blame others or their products, when you just had difficulty figuring it out for yourself. So in answer to your question, it ain't the FLIPSKYs.
```

---
## \#68 Posted by: KaramQ Posted at: 2019-04-04T03:18:07.293Z Reads: 133

```
Hey @Bobby, we got esk8 police on the forum, we got to watch what we say, I’ll never forget the time @venom121212 got me suspended for being a straight up noob
```

---
## \#69 Posted by: goldrabe Posted at: 2019-04-04T03:50:39.876Z Reads: 134

```
The information about how it could work was too short. As someone exposed to VESC's for the first time, split ppm, Canbus and all this terms are not understandable. And on top of that he got wrong information from the vendor. As a noob being deeply disappointed can lead to a rush of emotion. A link to a thread and a more detailed explanation would have helped.
```

---
## \#70 Posted by: Andy87 Posted at: 2019-04-04T06:37:47.088Z Reads: 124

```
To be fair... if you don’t know what is split ppm than better don’t start up building a 4wd...
I‘m all into explaining new people here the basics, but I also think there is a good amount of information here in the forum to find things out by your own. People should understand how things work when they build there boards to don’t fuck up the electronics or even worth crash so somewhere. A 4wd is a powerful board and you should know what you doing when you build one.
I hope the OP as min know what fail save is... if no, than it’s time to let him know before things get south!
```

---
## \#71 Posted by: goldrabe Posted at: 2019-04-04T06:44:43.145Z Reads: 124

```
Yes I agree with you, you are one of the most helpful members here!
Everyone starts somewhere and we should point everyone in the right direction./
Sometimes it needs just a few more words. I love the thread where someone ordered an evolve, cancelled it and got a bunch of great advise.
```

---
## \#72 Posted by: Andy87 Posted at: 2019-04-04T06:51:17.428Z Reads: 128

```
yeah that was a great success and I hope he is pretty happy with the trampa build he started now. was definitly the right decision.

But all this can just take place if also the OP is ready to take on advice and don´t get ignorant to suggestions.
Things like this are easy to missunderstand:

[quote="kchxaz, post:22, topic:89291, full:true"]
I’m not going to argue with your dumb ass. The manufacturer says it doesn’t work. If you can prove otherwise, please, be my guest
[/quote]
```

---
## \#73 Posted by: hiboute Posted at: 2019-04-04T09:14:26.937Z Reads: 127

```
You can also pair a gt2b remote with two receiver. In this case no can connection or split ppm between  the front and back, but your 4wd will work just fine.
```

---
## \#74 Posted by: venom121212 Posted at: 2019-04-04T11:17:09.766Z Reads: 121

```
The hell are you going on about?
```

---
## \#75 Posted by: KaramQ Posted at: 2019-04-04T12:02:02.073Z Reads: 118

```
Remember when I duplicated a thread
```

---
## \#76 Posted by: lrdesigns Posted at: 2019-04-04T12:31:04.538Z Reads: 115

```
I got nothing to add here, except to tell OP that basically all vesc can run 4wd with the right setup. Or prob 12 wheel drive too. 😋
```

---
## \#77 Posted by: linsus Posted at: 2019-04-04T12:40:51.914Z Reads: 110

```
What a sandbox thread, Yes, you can make a 4wd.

Regarding the motor not turning, try searching on the sbuject. Its one of the most common questions. Alot of settings to fiddle with.
```

---
## \#78 Posted by: venom121212 Posted at: 2019-04-04T13:02:11.415Z Reads: 108

```
No but I do remember when you quadruplicated a thread 

https://media.giphy.com/media/WqfoGLc4S0Nws/giphy.gif

I don't have rights to suspend... yet :smirk:
```

---
## \#79 Posted by: AlanZhou Posted at: 2019-04-04T13:19:55.184Z Reads: 105

```
oh shit :joy:
```

---
## \#80 Posted by: Skunk Posted at: 2019-04-04T13:33:46.357Z Reads: 102

```
![Abandon_Thread|300x198](upload://giQOQlphlNHw4ENGBthe5SFrRdY.gif)
```

---
## \#81 Posted by: KaramQ Posted at: 2019-04-04T13:46:12.736Z Reads: 100

```
Well someone flagged me and I got suspended for a day, did I actually quadruple a thread?
```

---
## \#82 Posted by: venom121212 Posted at: 2019-04-04T13:54:31.428Z Reads: 96

```
Yes but I can honestly say it was not I who flagged you. Flagging ends all the fun tollolololol
```

---
## \#83 Posted by: AlanZhou Posted at: 2019-04-04T13:55:20.903Z Reads: 92

```
i got flagged for saying jas** couldn't afford more st*oage
```

---
## \#84 Posted by: KaramQ Posted at: 2019-04-04T13:55:28.040Z Reads: 92

```
Was it really not you
```

---
## \#85 Posted by: venom121212 Posted at: 2019-04-04T13:56:09.459Z Reads: 92

```
100% not. I've got nothing against you brother.
```

---
## \#86 Posted by: KaramQ Posted at: 2019-04-04T13:57:01.111Z Reads: 95

```
That’s good to know, I thought you hated me because of that.
```

---
## \#87 Posted by: L3chef Posted at: 2019-04-04T13:58:40.275Z Reads: 94

```
Jieh, what a thread :grinning:
```

---
## \#88 Posted by: Itsmedant Posted at: 2019-04-04T14:11:45.609Z Reads: 92

```
We learn, we laugh, we criticize.
```

---
## \#89 Posted by: Skunk Posted at: 2019-04-04T14:22:28.734Z Reads: 92

```
[quote="Itsmedant, post:88, topic:89291"]
We learn
[/quote]

Im not sure anyone learned a thing here. Lol

Well, other than karam knows venom doesn't hate him.

OP hasn't replied in a bit. 

Basically dude @kchxaz if a vesc can do one wheel drive. It can do 4wd. You just gotta know how to hook it up. 
If you don't believe us...... cool. Don't care,  it's nobody's job to hold your hand.  Figure it out yourself.  
OR, you can try to hear what people are telling you. 
People here wanna help, even if they are asshats about it.
Good luck with the build.
```

---
## \#90 Posted by: meesie Posted at: 2019-04-05T17:46:23.074Z Reads: 75

```
i have never seen a bigger mess of a thread than this one. holy cow.......

as for staying on topic: 4wd needs 4 separate or 2 dual vescs. did you buy 1 vesc???
```

---
## \#91 Posted by: SeanHacker Posted at: 2019-04-05T17:55:07.923Z Reads: 72

```
[quote="meesie, post:90, topic:89291"]
i have never seen a bigger mess of a thread than this one. holy cow…
[/quote]

You must be new here...
```

---
## \#92 Posted by: meesie Posted at: 2019-04-05T18:04:01.536Z Reads: 72

```
not really but i havent seen a lot of messes yet i suppose. (i use the search bar lol)
```

---
## \#93 Posted by: KaramQ Posted at: 2019-04-05T18:10:51.323Z Reads: 72

```
Kaly vs trampa patent
```

---
## \#94 Posted by: DerelictRobot Posted at: 2019-04-05T18:16:07.680Z Reads: 71

```
[quote="mishrasubhransu, post:4, topic:89291, full:true"]
These is nothing wrong with FSESC6.6 except minor voltage sensing issue.
[/quote]

This. 

I've put 4600 miles on my pair of FSESC 6.6. They're solid. It's the cheaper ones that have had some issues in the past.

Edit: hopefully you didn't get the ones with integrated antisparks. Because there's no good integrated antispark. I ordered them without and got a 'free upgrade' to the integrated antispark version. Womp womp
```

---
