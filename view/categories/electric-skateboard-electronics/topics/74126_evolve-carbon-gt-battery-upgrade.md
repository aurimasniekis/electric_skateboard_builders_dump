# Evolve Carbon GT battery upgrade

### Replies: 78 Views: 3572

## \#1 Posted by: Marsen Posted at: 2018-11-10T03:18:17.824Z Reads: 276

```
G'Day all, since doing a Bamboo GT battery upgrade I have been busy building batteries for other esk8er's as well as looking into designs for range extenders and numerous other projects. I was also asked to fit upgraded batteries to a couple of Carbon GT boards which I was keen to do. First thing I did was watch Kevin Dark's YouTube video on the upgrade. Then when I opened up the first board found a different type of BMS. This is an older style and wider than the now used version.![20181104_120708%5B1%5D|690x388](upload://lSLucbITxmuhZ3Muqr94PFVb0Ws.jpeg) 
The top board has the wider BMS, the bottom one has the slimline one
![20181104_120725%5B1%5D|690x388](upload://wGhr5XTGM6OfHc5r0wwlYBDtbhk.jpeg) 
I checked out a few threads and posts and realised the only way this 10S5P was going to fit was with a spacer. I checked out Zero form Designs here in Perth as Charlie (Guy whose board it is) said they do one. After a quick look jumped on the PC and knocked one up on FreeCAD and uploaded to my printer. 
![20181104_103023%5B1%5D|690x388](upload://4NOxsyTnVvcSEYAkFYz9PbzAhyv.jpeg) 

30 mins later......

![20181104_111920|690x388](upload://u6FB2eO8UZufcW9hcJSjYICcdnJ.jpeg) 
As Charlie said when I sent him the pic "Farout !! Yeah that's Sweet azz "
The rest of the fit out was easy as this created stacks of room for the BMS and plugs.
![20181107_134849%5B1%5D|690x388](upload://ely6iasFvC8kPIPjnmCNVdKiYbx.jpeg) 
Insulated the esc and BMS with Kapton high temp insulation tape and the foam padding that comes with the BMS. Just needs tidying up, BMS and wires securing and all done. The heat sink needs longer screws because of the spacer which are easily sourced.
![20181107_135148%5B1%5D|690x388](upload://rFS4b0ljC0rJ4aC3wVXSHMHwigu.jpeg) 
Feed back from Charlie is he's a very very happy man!  Way more range and powered up those hills without any lag. I'd like to take all the credit but really it should go to Samsung for that wonderful little gem the 30Q.
The second build was in my opinion harder as things are a tight fit getting that smaller BMS in without using a spacer. Soldered on the new battery and gently squeezed it in. I trimmed the shrink wrap on the battery as every tenth of a mm was needed. made sure all was well insulated and taped down. 
![20181104_141111|690x388](upload://hVJtSKuZRApH0N9CWqTBLmHgKEu.jpeg)
```

---
## \#2 Posted by: maker Posted at: 2018-12-09T06:09:55.291Z Reads: 216

```
30q batterys are only good for 15A so they are not acceptable for a 3 or 4p pack for the evolve GT board as they can pull up to 80A at full noise. as well you say you use 0.2mm nickel strap x3 plus 4mm2 tinned copper braid. what width is you nickel strip and your braid. by my calcs you are very under rated for the GT. as far as i can see no one sells 4mm2 copper braid less than 2mm thick.  i can tell you with those dimensions it will not fit. evolve made sure people people wouldnt be able to retro fit 18650 batterys to there CGT with out spending big dollars on copper welding techniques to keep the width down. also a tip, dont make the mistake that many have and choose to not insulate the outer edges of your pack sufficently so as to be able to fit your pack in a CGT. the Carbon fibre is conductive. you are basically installing the batteryinto a metal box with a thin layer of soft easily scrathed laquer on it. vibration = fire in a poorly insulated carbon board battery.
```

---
## \#3 Posted by: b264 Posted at: 2018-12-09T06:26:21.345Z Reads: 207

```
There is *no way* the Evolve GT boards pull 80 battery amps -- I'd like to see that measured to believe it.
```

---
## \#4 Posted by: kalebludlow Posted at: 2018-12-09T06:27:30.413Z Reads: 203

```
Yeah my understanding was closer to 40A in total, especially considering Evolve uses some trash cells
```

---
## \#5 Posted by: dareno Posted at: 2018-12-09T06:36:19.857Z Reads: 206

```
[quote="maker, post:2, topic:74126"]
they can pull up to 80A at full noise.
[/quote]

Thats too funny.  My 12s 4p is set on 80 amps max and it makes a cgt look like a toy.  Like some real world specs to back up that statement.  Also the 30q is actually good for 20 amp regardless of the spec sheet.  Whats your set up?  Oh and welcome to the forum.
```

---
## \#6 Posted by: pixelsilva Posted at: 2018-12-09T07:02:53.371Z Reads: 202

```
Still don't understand why people keep fighting with the CGT tight space?? :roll_eyes: Clean up the dang space guys!! Clear all that up. Put the largest battery you can possibly fit there. From one end of the enclosure to the other. The whole thing!! And someone pleaseeee 3D print a second 'enclosure' underneath for all the BMS, VESCs, heat sink, cabling, connectors (sort of the same way you did that heat sink spacer, 'stacks of room' for all components I already mentioned!

Same thing but larger! Enlarge the dam thing. What's the big deal?? ... :point_down:

![image|690x388](upload://nEFAACXrOtq2G4X7kCUdKf6Jz18.jpeg) 

C'monnn guys!! I've seen more difficult challenges solved here.
```

---
## \#7 Posted by: Marsen Posted at: 2018-12-09T07:10:41.363Z Reads: 196

```
80A? Have you seen the Evolve BMS. It only has 4 power MOSFETS no way are they going to handle 80A for more than a few seconds, they also use 14 AWG for their power connections which converts to 2mm2 which as it's a high temp insulation will give you 45A capacity. I think you may want to direct a few of your questions to Evolve and see what they say about under rated connections and electronics.
I as well as numerous others have fitted 18650 packs into CGT's quite easily. I have high temp Kapton tape, then reinforced pvc tape (same as Evolve) followed by the same PVC heat shrink that Evolve uses. The Bamboo boards you do need to trim the screw posts to get these batteries to fit but that is easily done. My interconnections are at the center of each P group so the Nickel strips are only carrying at max half the load of each P group.
```

---
## \#8 Posted by: Marsen Posted at: 2018-12-09T07:29:29.894Z Reads: 190

```
To add to my last, the can of the cell has 0.5mm steel ends. Steel is only 10% as conductive as Copper and 50% as conductive as Nickel. Anyone fancy doing the Math on the current carrying capacity of the cell can?
```

---
## \#9 Posted by: Fiori Posted at: 2018-12-09T08:19:01.183Z Reads: 191

```
Iv'e already done it. All the files are on my thingiverse.![bottom|690x312](upload://7sdf6MYFjkhFFNskLCtfaHHOTb1.jpeg)
```

---
## \#11 Posted by: maker Posted at: 2018-12-09T08:34:53.318Z Reads: 184

```
the space issue isnt length its width.
```

---
## \#12 Posted by: maker Posted at: 2018-12-09T08:35:55.299Z Reads: 183

```
37A per motor
80A momentarily. still i would not be selling and putting my name on a battery that could burn 2k down the drain knowing my setup doesnt allow for those momentary currents. as long as you know then il be on my way. like i said im not here to ruin your party. just being the annoying becareful guy.
```

---
## \#13 Posted by: kalebludlow Posted at: 2018-12-09T08:39:26.601Z Reads: 180

```
I would genuinely love to see some testing of this stuff, because it would show Evolve as being more powerful than we all thought
```

---
## \#14 Posted by: maker Posted at: 2018-12-09T08:43:33.439Z Reads: 180

```
maths wont be ness in this case as common sense will suffice. the can thickness and material is irrelevant since the current path is a whole half a millimeter...... not half a meter.
```

---
## \#15 Posted by: Fiori Posted at: 2018-12-09T08:47:28.014Z Reads: 173

```
The esc only pulls 65A max I'm pretty sure. So I think a 4p pack would be fine.
```

---
## \#16 Posted by: maker Posted at: 2018-12-09T08:50:47.277Z Reads: 176

```
if the 30Q was good for 20A it would be marketed as such. trust me. there is a reason they write maximum ratings on electronic items. something to do with thousands of hours of controlled tests , its very boring yeah why dont we just change the specs of all electrical components to suit our needs... hmm i wonder...? screw it, my mate steve said they are good for 100A so thats what il tell people they are good for. what does LG and samsung know anyway, complete amateurs that bunch.
```

---
## \#17 Posted by: Fiori Posted at: 2018-12-09T08:59:34.137Z Reads: 180

```
My friend, have you read even the data sheet? 20A is safe according to the MFG..... These tests were done by Samsung, not your buddy Steve. 

It wont start a fire. It will effect your amount of charge cycles. But most fires are caused from bad insulation/shorts. 

https://eu.nkon.nl/sk/k/30q.pdf

![](https://gyazo.com/8917972bcc57d0a0b6b55815456c47b4.png)
https://gyazo.com/8917972bcc57d0a0b6b55815456c47b4
```

---
## \#18 Posted by: maker Posted at: 2018-12-09T09:10:17.715Z Reads: 167

```
you missed some information here friend... note the highlighting over the 20A heading? what do you suppose thats there for?
```

---
## \#19 Posted by: Marsen Posted at: 2018-12-09T09:14:12.962Z Reads: 171

```
![SAMSUNG%2030q%20DISCHARGE%20TEST|690x485](upload://3pI68hMSHXQiPsk8z6aiUvyLg8H.jpeg) 
Still doesn't alter the fact that Samsung do test at 20A as well as 22A. If this wasn't safe why would they publish results under such test conditions.
```

---
## \#20 Posted by: maker Posted at: 2018-12-09T09:15:09.652Z Reads: 167

```
....the remotes have a hidden feature that will show you current draw on each motor in real time. but good to see people are confidently commenting on stuff they have no experience or knowledge on. looks like im really missing out not sitting on a forum all day.
```

---
## \#21 Posted by: Fiori Posted at: 2018-12-09T09:15:42.399Z Reads: 165

```
I do have a remote and have done testing myself.
```

---
## \#22 Posted by: maker Posted at: 2018-12-09T09:17:50.219Z Reads: 158

```
because thats what manufacturers do.... they test to make there products fail to determine safe parameters for there products then they write the safe working load on the spec sheet.... am i seriously answering this question rn... look guys im out. its been fun. as usual the forum is just an echo chamber for people with similar thoughts and not the place of research that some people think it is. good luck. dont rek your selves
```

---
## \#23 Posted by: dareno Posted at: 2018-12-09T09:19:52.106Z Reads: 156

```
Missing you already
```

---
## \#24 Posted by: Fiori Posted at: 2018-12-09T09:20:26.151Z Reads: 155

```
Look I don't want you to leave. I feel like we are having a forum discussion, that's what we do here. So please don't feel attacked.
```

---
## \#25 Posted by: Skunk Posted at: 2018-12-09T09:21:29.263Z Reads: 147

```
If 30q aren't that great what is?
```

---
## \#26 Posted by: Fiori Posted at: 2018-12-09T09:22:20.142Z Reads: 144

```
I'm agreeing with you that the ESC draws upwards of 65 AMPS. But I'm disagreeing that runnning 30Q's at 20A's is a fire hazard.. 

Evolve claims it draws "60-80A at times". Video here(timestamped): https://youtu.be/hIEj9ylmKRI?t=110
```

---
## \#27 Posted by: dareno Posted at: 2018-12-09T09:31:25.747Z Reads: 143

```
Dude hes not saying they're not great, hes saying they shouldn't run at 20 amps.  Cool.  Then got all silly when he got corrected.  Love a discussion but if hes not mature enough to come in here and behave like an adult then good riddance.  Think the discussion went sideways earlier due to confusion over continuous and peak.  Lets just put it down to inexperience and leave it there.  Mate stay and read and expand your horizons.  Seriously we are not here to bag you out just to give you some insight into different opinions and experiences.
```

---
## \#28 Posted by: pixelsilva Posted at: 2018-12-09T09:38:13.573Z Reads: 154

```
Rant... :point_down:

> @maker 
> 
> wow. some really emotionaly upset people here. sorry ladys i didnt mean to upset your tea party.

> like i said im not here to ruin your party. just being the annoying becareful guy.

> but good to see people are confidently commenting on stuff they have no experience or knowledge on.

> looks like im really missing out not sitting on a forum all day.

> as usual the forum is just an echo chamber for people with similar thoughts and not the place of research that some people think it is. good luck. dont rek your selves

> am i seriously answering this question rn… look guys im out. its been fun.

.
.
:point_down:

http://www.livemaguk.com/wp-content/uploads/2015/01/Trolling-and-cyber-bullying.gif
```

---
## \#29 Posted by: moone Posted at: 2018-12-09T09:41:46.256Z Reads: 142

```
@Marsen is a Robotics Engineer that has built a whole battery to power his house, is a valuable member of the community, and someone you can call up for a chat if you had a question about anything battery related. He has made several batteries for people here in Perth that are unmatched in quality. 

And your qualifications are @maker?......
```

---
## \#30 Posted by: xilw3r Posted at: 2018-12-09T10:37:16.199Z Reads: 144

```
I would just like to note the temperature of 99 degrees C after a 20A discharge :smiley:
but 20A peaks are definitelly not an issue here.
@maker mate, i work with 18650's. we make and test modules, I understand the wishing for safety, but I honestly dont see the reason, or rather your argument, on why these cells are bad for such a use case which is clearly with in their capabilities according to numerous tests
```

---
## \#31 Posted by: brenternet Posted at: 2018-12-09T12:17:11.184Z Reads: 136

```
I'm so sad I missed this guy and his salty snatch 😂

This forum is composed of thousands of builds of "real world" experience from people of all walks of life. Including professionals in all fields.

Coming on here and squatting your vagina straight down into the sand in your very first post is likely going to see you leaving real soon.
```

---
## \#32 Posted by: Pedrodemio Posted at: 2018-12-09T14:39:01.911Z Reads: 128

```
The remote explicitly says it’s motor current? Battery current is completely different from motor current at times unless you are driving at 100% duty cycle on the controller

Just curious
```

---
## \#33 Posted by: Battosaii Posted at: 2018-12-09T15:06:48.910Z Reads: 125

```
damn it i missed the drama again.

gona have to make my own drama. hmmm 

- The Raptor 2 is slow

- Evolve carbon decks break or crack 100% of the times

- You will never be satisfied at 10s

- Hub motors are not the future
```

---
## \#34 Posted by: mmaner Posted at: 2018-12-09T15:26:07.136Z Reads: 123

```
[quote="maker, post:2, topic:74126"]
30q batterys are only good for 15A so they are not acceptable for a 3 or 4p pack for the evolve GT board as they can pull up to 80A at full noise.
[/quote]

You need to read more before making statements like that, which is wrong BTW.
```

---
## \#35 Posted by: Bjork3n Posted at: 2018-12-09T15:39:24.052Z Reads: 120

```
You are playing with fire my friend....:joy:
```

---
## \#36 Posted by: mmaner Posted at: 2018-12-09T15:49:11.252Z Reads: 119

```
I agree, except hummie hubs are epic.  I've never ridden another hub motor that I wouldn't imeadiatly get rid off.
```

---
## \#37 Posted by: b264 Posted at: 2018-12-09T17:11:51.250Z Reads: 119

```
[quote="maker, post:12, topic:74126"]
the annoying becareful guy.
[/quote]

We'll have to fight for that spot :smirk:
```

---
## \#38 Posted by: Mich21050 Posted at: 2018-12-09T17:12:52.236Z Reads: 116

```
@maker May I give you a small advice... don't fight with @b264 :joy: :
No offence.. I think you are a great guy :slight_smile:
```

---
## \#39 Posted by: b264 Posted at: 2018-12-09T17:15:28.102Z Reads: 122

```
[quote="maker, post:20, topic:74126, full:true"]
…the remotes have a hidden feature that will show you current draw on each motor in real time. but good to see people are confidently commenting on stuff they have no experience or knowledge on. looks like im really missing out not sitting on a forum all day.
[/quote]

That current draw is "motor amps" and it's the positive half of a duty cycle.  So you might have 80A for 2 microseconds and 0A for 7 microseconds and the remote will say 80A ... but the "battery amps" here is 17.8A after the ESC filter capacitor
```

---
## \#40 Posted by: brenternet Posted at: 2018-12-09T17:17:58.299Z Reads: 120

```
Stop with the common sense! He has the cheat codes to get into the secret level on the evolve remote!
```

---
## \#41 Posted by: billappleton Posted at: 2018-12-09T17:24:47.101Z Reads: 124

```
i started down the trail of upgrading my evolve battery. but the esc is proprietary and questionable. and the motors aren't that great. and people worry about the remote. ended up using my supercarve trucks, some gears, and the abec 107s.
```

---
## \#42 Posted by: Marsen Posted at: 2018-12-10T03:57:35.860Z Reads: 115

```
Are you serious! where's your evidence for those statements. Do you know what you're talking about ? You shouldn't come on here talking about stuff you know nothing about.......
```

---
## \#43 Posted by: Marsen Posted at: 2018-12-10T03:58:53.100Z Reads: 117

```
:rofl::rofl::rofl::rofl::rofl::rofl::rofl::rofl::rofl::rofl::rofl::rofl:
Is that drama enough
```

---
## \#44 Posted by: dareno Posted at: 2018-12-10T07:42:50.446Z Reads: 118

```
:joy::joy::joy:
Too good
```

---
## \#45 Posted by: dareno Posted at: 2018-12-10T07:47:30.806Z Reads: 117

```
[quote="Battosaii, post:33, topic:74126"]
* Evolve carbon decks break or crack 100% of the times
* You will never be satisfied at 10s
[/quote]

There are effigies of you now with pins in and @b264 is planning his reply for the 10s thing. 
:notes: Baby come back :notes:
```

---
## \#46 Posted by: drone001 Posted at: 2018-12-29T22:33:14.171Z Reads: 109

```
Ok I own a CGT and I'm ready to do a battery upgrade. I've been reading for 2 weeks now about battery upgrades. I'm thinking about doing a 10s8p (10s4p*2). Any thoughts....suggustions?
```

---
## \#47 Posted by: Marsen Posted at: 2018-12-29T22:46:17.160Z Reads: 112

```
How you planning on getting it to fit in? Routing, spacer or both?
I built a 10S10P for a guy so the battery is not a problem to make. There was a guy in Perth making 20mm spacers but he had gone off line. I have just bought a cnc router to make enclosures and spacers but that's not setup yet. Have to build it first. You can get the stl files online if you have a 3D printer. If you have that sorted then I don't see any issues with the idea.
```

---
## \#48 Posted by: billappleton Posted at: 2018-12-29T23:01:33.081Z Reads: 108

```
@eboosted has a universal enclosure that will fit the Evolve GTX deck.
```

---
## \#49 Posted by: drone001 Posted at: 2018-12-30T01:31:32.872Z Reads: 110

```
I plan to build or buy an enclosure to go underneath the board. The reason for breaking the battery up into 2 10s4p packs. that 10s10p sounds really sweet. I want to keep my evolve carbon deck (I love the deck) but eventually I'll replace the ESC with a dual FSESC 6 6 or an  Unity.
```

---
## \#50 Posted by: drone001 Posted at: 2018-12-30T01:35:31.100Z Reads: 109

```
wow.....thx these enclosures look great.
```

---
## \#51 Posted by: Marsen Posted at: 2018-12-30T01:55:57.272Z Reads: 107

```
Carbon GT. Sorry was thinking of the BGT.
```

---
## \#52 Posted by: billappleton Posted at: 2018-12-30T01:56:28.711Z Reads: 105

```
Check out my Hellboy build thread. This is an Evolve on acid. I really like the feel of Evolve, but wanted to maximize.
```

---
## \#53 Posted by: drone001 Posted at: 2018-12-30T02:06:47.880Z Reads: 103

```
that's bad ass bruh....how's that Unity and the 12s4p working for ya? that's my ideal set up CGT AT with unity. I'm concerned that 12s4p will not be enough. How's the range, torque and top speed?
```

---
## \#54 Posted by: drone001 Posted at: 2018-12-30T02:18:48.726Z Reads: 98

```
is it really as easy as they show in the videos....setting up the Unity?
```

---
## \#55 Posted by: billappleton Posted at: 2018-12-30T02:32:17.582Z Reads: 103

```
The Unity has been great, yes very easy to set up. 12s4p on Unity with dual 200kw motors is brutal. I lowered the motor max from 60 to 50 amps to stop the dragster acceleration. I haven’t ever floored it yet. If you get close it will throw you off the back. Not sure about the range but based on the charge time it is big. The board is very smooth and silent. Still has that Evolve carve though.
```

---
## \#56 Posted by: mmaner Posted at: 2018-12-30T02:34:27.641Z Reads: 103

```
Have you tried an acceleration curve yet?
```

---
## \#57 Posted by: billappleton Posted at: 2018-12-30T02:46:35.061Z Reads: 102

```
I have. Still tweaking and riding. :)
```

---
## \#58 Posted by: mmaner Posted at: 2018-12-30T02:48:42.090Z Reads: 103

```
Cool, I usually start around -20/-20 and tweak from there. Good luck.
```

---
## \#59 Posted by: maxshop Posted at: 2019-01-16T10:36:27.145Z Reads: 95

```
With the spacer and moving down the esc i should expect connection dropouts or better connectivity with the remote? Plan to use and 10s5p
```

---
## \#60 Posted by: Sn4pz Posted at: 2019-01-16T12:59:42.605Z Reads: 96

```
If you're upgrading the battery throw out the garbage stock electronics and spend the extra 350 for a reliable dual esc, controller and loopkey
```

---
## \#61 Posted by: maxshop Posted at: 2019-01-16T13:37:53.885Z Reads: 101

```
I had 0 dropouts in i think 5000km. I was thinking about dropouts because i heard some people have them and if i move controller down wouldn't like to have them.

If i could have R2 remote with another esc/controller i would change if dropouts appear. I just love R2
```

---
## \#62 Posted by: pixelsilva Posted at: 2019-01-17T02:10:21.866Z Reads: 104

```
For you all, @hyperIon1 & @hyperIon2 offer printing batt spacer for Evolve boards!

https://www.hyperionesk8.com
```

---
## \#63 Posted by: hyperIon1 Posted at: 2019-01-17T02:29:07.148Z Reads: 107

```
Yes, 
3D printed riser for the Bamboo GTX will accomidate a 10s5-6p with evolve bms and system (add focbox duel heatsink) and go full conversion or next level with ![IMG_1096|690x320](upload://cCBjOC37dJ7veZnlMCfIAfn9D44.jpeg)
 ![IMG_0931|375x500](upload://eG0djdZwMajuUMgESOkzaWpmB5c.jpeg) ![IMG_0932|375x500](upload://l6TYxV5GS7pvSbzocMJgbqZE1nM.jpeg) 
![IMG_1158|666x500](upload://hPzRjFFmizg1WyqhD4Y4uUR37vW.jpeg) 

![IMG_1157|666x500](upload://cO8P46FOlOp4m5STWISNZZBbMkf.jpeg) 
  a unity heatsink on a Carbon GT

![IMG_1159|666x500](upload://hb2c8abUDLip5TToXKr969Zt5iC.jpeg) 
![IMG_1160|666x500](upload://23PjGXlkgSSvWZRjR68cpZSyfNB.jpeg)
```

---
## \#64 Posted by: pixelsilva Posted at: 2019-01-17T02:40:05.267Z Reads: 98

```
:point_up_2: With that minuscle d124 bms there's space for even a 12s4p!
```

---
## \#65 Posted by: hyperIon1 Posted at: 2019-01-17T03:28:09.746Z Reads: 100

```
yes, that's my original replacement 10s4p in the pic,  I started the upgrades with it and OG system and now it's like a MOB truck in a Cadillac
```

---
## \#66 Posted by: Goonman Posted at: 2019-01-21T10:37:12.805Z Reads: 95

```
I made a video of the evolve pulling absolute max 40amp from the battery.
```

---
## \#67 Posted by: asuras Posted at: 2019-04-17T07:40:05.389Z Reads: 71

```
Hi @hyperIon1, I'm looking to replace my ESC/BMS in my carbon GT with something better, at this stage looks like I'm going with a FOCBox Unity just for simplicity. It looks like you milled out part of the carbon enclosure (around the leftmost FOCBOX mounts) in that install - why is this? And I also I see you removed the FOCBox enclosure, is there a reason for this too?

And lastly, I'm assuming that you ditched the FOCBox heatsink and remounted it to the stock Carbon heatsink yeah?

Mostly curious if I should do the same and what the reasoning is...
```

---
## \#68 Posted by: Arzamenable Posted at: 2019-04-17T08:28:16.343Z Reads: 71

```
![image|666x500](upload://hBJ5RWyrengspAAP2wOY7u4kASj.jpeg) 

The unity has a tiny footprint. I cut away at my deck at earlier iteration of this. It’s seen vesc6s, dual focboxs, 4.12s, fesc 6.6 dual. Board mods were made for those chubsters. 

I now have to go back and fill in the holes. #unityproblems.
```

---
## \#69 Posted by: Arzamenable Posted at: 2019-04-17T08:31:16.352Z Reads: 62

```
The stock sink is optimal for the unity. Mine were all cut up, luckily I found an orphaned one in Dave's garage.
```

---
## \#70 Posted by: asuras Posted at: 2019-04-17T10:04:54.718Z Reads: 60

```
That looks like a killer setup! One thing I'm a bit gutted about going with the Unity is that it doesn't have traction control like the fsesc 6.6 dual, and looking at the dimensions of the fsesc 6.6 dual I couldn't see how I could fit one in to that enclosure without some serious carving into the carbon deck which seems like a bad idea... but you managed somehow?
```

---
## \#71 Posted by: Jaydawg56 Posted at: 2019-04-17T10:19:50.705Z Reads: 57

```
Traction control was added by Jeff in this last unity update.
```

---
## \#72 Posted by: asuras Posted at: 2019-04-17T10:26:04.759Z Reads: 60

```
oh sweet, they should put that on the website...
```

---
## \#73 Posted by: Arzamenable Posted at: 2019-04-17T20:03:06.198Z Reads: 62

```
Do you find traction control helps? Seems like a cool feature. I used it awhile back. I would disable it to see which wheel and motor was acting up and forgot to reenable, going forward, probably won’t add in more complexity. 

I cut out an opening at the front of the deck for the 6.6 sink. Widened it later to fit a second stock evolve sink and put a unity on it. 

There is only one hint of a crack on the side of deck where it starts to taper in. From an old wreck in two years ago. This board is stamped “2016”. Still rolling.
```

---
## \#74 Posted by: asuras Posted at: 2019-04-18T00:26:35.167Z Reads: 58

```
Wow that's awesome, I would have thought that cutting into the carbon pretty much anywhere would seriously compromise the strength of it. Can you cut out any part of the battery enclosure? Or just the parts that are already super thin? (like where the ESC heatsink sits)

I haven't ever ridden a board with traction control but I've had plenty of experience with my GT instantly fishtailing when it goes over a change in surface at speed, especially with the stock A/T wheels and especially going from tarmac -> grass/dirt. I'm pretty confident that traction control would solve that issue, and would also make a big difference on trail skating too. I already changed my tyres to MBS knobbies which  is a massive improvement on those surfaces so I'm keen to see how they also go with TC.
```

---
## \#75 Posted by: Arzamenable Posted at: 2019-04-18T01:03:19.767Z Reads: 53

```
The second esc cut removed thin material. Probably shouldn’t get into the sides where the top cover sits.
```

---
## \#76 Posted by: hyperIon1 Posted at: 2019-04-19T00:08:29.523Z Reads: 49

```
that GT carbon has been through many upgrades to test what you can do, at one point I had duel FB and the custom heatsink needed the room to fit properly
```

---
## \#77 Posted by: asuras Posted at: 2019-04-25T14:50:22.288Z Reads: 47

```
Hey @Fiori I couldn't find that STL on your thingiverse? Unless its the focbox mount? I'm looking to add space to my CGT to put a focbox unity + full bms next to my 10s5p that marsen built for me. I've made an STL myself, but don't have easy access to a printer so kinda hoping to find a tried and tested STL that will give me some roomage...
```

---
## \#78 Posted by: Fiori Posted at: 2019-04-25T20:12:34.216Z Reads: 46

```
Hey man. The compartment i have under my CGT is attached to the focbox holder I made(i made it modular). 

Exactly which part were you looking for? I can get you any files you need.
```

---
## \#79 Posted by: Wizeartz Posted at: 2019-07-01T03:04:46.152Z Reads: 32

```
I'm laser-cutting GT spacers in 6mm at the moment for 10S4P upgrades, I can probably source 10mm too no doubt. Across the ditch in New Zealand, only about NZD$12 to ship.
```

---
