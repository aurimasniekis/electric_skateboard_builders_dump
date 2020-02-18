# Why is there no on/off switch integrated in a VESC

### Replies: 84 Views: 3729

## \#1 Posted by: Maxid Posted at: 2018-05-17T09:46:24.356Z Reads: 411

```
Hey guys,

after buying a Lou board I want to replace the ESC with a Focbox I have around.
What bothers me though is that in order to turn the VESC off/on I have to use an AntiSpark switch somewhere in my circuit. Why is that though? Why doesn't the VESC have a small switch that can turn the power supply for its "brain" components off or on? The current can't be high so even the tiniest switch would suffice.
There should be no need for an AS when I only rarely disconnect the battery. The Lou even has a push to wake the ESC function - that is awesome and eliminates an additional part.

What i also don't understand is why even a redesign of VESC6 like [img]http://www.electric-skateboard.builders/uploads/db1493/original/3X/7/0/702e9bf0eabdee5cc3fdf271a04f1dfcc659946a.jpg[/img] uses additional FETs just for the sake of turning the VESC on and off - is that really necessary?

Well I hope someone can help me understand - there is probably a reason and I really want to know.
```

---
## \#2 Posted by: linsus Posted at: 2018-05-17T09:52:40.578Z Reads: 392

```
[quote="Maxid, post:1, topic:55753"]
Why doesn’t the VESC have a small switch that can turn the power supply for its “brain” components off or on? The current can’t be high so even the tiniest switch would suffice.
[/quote]

What? you mean a switch to the MCU only?.. you want constant voltage delivery onto the input?. This sentence doesnt make any sense to me.

[quote="Maxid, post:1, topic:55753"]
What i also don’t understand is why even a redesign of VESC6 like uses additional...
[/quote]

That redesign doesn't have anything to do with the original HW verision. I cant see any Fets for switching on that card?. The mechanical switch on the board is for different voltage on the hall sensor input.
```

---
## \#3 Posted by: b264 Posted at: 2018-05-17T10:02:27.585Z Reads: 383

```
[quote="linsus, post:2, topic:55753"]
I cant see any Fets for switching on that card
[/quote]

We never saw the bottom and so it's hard to say for sure, but it appears they did add FETs for power switching, the three devices under `www.flipsky.net` on the PCB
```

---
## \#4 Posted by: Maxid Posted at: 2018-05-17T10:25:38.927Z Reads: 378

```
[quote="linsus, post:2, topic:55753, full:true"]
What? you mean a switch to the MCU only?.. you want constant voltage delivery onto the input?. This sentence doesnt make any sense to me.
[/quote]

Why shouldn't there be a constant voltage on the "input" as long as any power to the brain components is switched off? Does that damage anything? What will be damaged?

[quote="linsus, post:2, topic:55753, full:true"]
That redesign doesn't have anything to do with the original HW verision. I cant see any Fets for switching on that card?. The mechanical switch on the board is for different voltage on the hall sensor input.
[/quote]
Hm? the three fets on top close to the XT-connector are just an AS - the fets for the motor are on the opposite side (there are 12 of them - see post below). The switch is supposed to be wired and not pictured.
```

---
## \#5 Posted by: Maxid Posted at: 2018-05-17T10:26:33.835Z Reads: 339

```
yes we did see the bottom
http://www.electric-skateboard.builders/t/new-vesc-from-china-seems-like-not-only-maytech-is-making-vescs-now/5207/180
```

---
## \#6 Posted by: linsus Posted at: 2018-05-17T10:59:08.202Z Reads: 324

```
[quote="Maxid, post:4, topic:55753"]
Why shouldn’t there be a constant voltage on the “input” as long as any power to the brain components is switched off? Does that damage anything? What will be damaged?
[/quote]

Introducing a constant voltage-source on the drain?.. Not sure how big the leakage and what dissipation and wear that equals to, or what even happens when you roll the board in off mode with live battery wires, but no. you want as good isolation as possible in Power applications. Especially in off-mode. I can't think of any obvious benefits to this proposal.
```

---
## \#8 Posted by: Maxid Posted at: 2018-05-17T12:11:28.470Z Reads: 299

```
I don't understand :( Why would it be worse than having the AS FETs exposed to the constant voltage? There must be a way to isolate the brain components so that they don't see any voltage when off no?
```

---
## \#9 Posted by: linsus Posted at: 2018-05-17T12:47:12.292Z Reads: 291

```
The main purpose of the AS is to limit inrush currents. You wont have that function at all without altering the VESC. The AS also provides a safe Power of stage where the VESC is physically disconnected from the battery. You wont have that either.
```

---
## \#10 Posted by: Acido Posted at: 2018-05-17T12:47:43.247Z Reads: 281

```
i do not think that the lou board handles 2500w 
strong batteries=huge currents=boom in shitty parts
```

---
## \#11 Posted by: Maxid Posted at: 2018-05-17T12:51:44.238Z Reads: 277

```
A normal AS can't handle 2500W. 50A continuous is the max any AS can handle.
```

---
## \#12 Posted by: Acido Posted at: 2018-05-17T12:52:27.923Z Reads: 269

```
I was talking about ESCs with integrated "AS" or an on off switch
```

---
## \#13 Posted by: Maxid Posted at: 2018-05-17T12:53:05.975Z Reads: 257

```
Why would I have inrush currents when the capacitor stays connected to the battery?
```

---
## \#14 Posted by: Maxid Posted at: 2018-05-17T12:55:09.575Z Reads: 252

```
Doesn't matter though no? 2500W is a crazy amount of power and even VESC based systems can't handle that with the standard AS we have today.

BTW: When talking AS I do not mean loop keys - that's a different story.
```

---
## \#15 Posted by: TowerCrisis Posted at: 2018-05-17T12:59:15.966Z Reads: 241

```
Crazy? Idk man my current build I'm working on is 4400 watts at peak power draw. There are 5055 motors that can easily draw 2000 watts.
```

---
## \#16 Posted by: Maxid Posted at: 2018-05-17T13:02:13.727Z Reads: 236

```
If your system would draw 4400W continuously do you know how fast your battery would be empty?
With a 10S4P of 30Q cells you have 12Ah*36V=432Wh --> 432Wh/4400W=not even 6 minutes.
Your components would melt by the way - don't believe marketing terms! Just because a motor can draw such power it does not mean you are actually ever using it. The VESC can't handle it and a normal battery can't handle it. And peak usage is an irrelevant number and does not mean anything.
```

---
## \#17 Posted by: esk8jpn Posted at: 2018-05-17T13:08:02.692Z Reads: 227

```
Is BMS with switch an alternative solution to Anti-Spark Switch?
```

---
## \#18 Posted by: Maxid Posted at: 2018-05-17T13:09:03.503Z Reads: 221

```
it's even bigger than an AS so no. I want to simplify not add even more complexity. I usually don't use BMSs in my builds - I find them unnecessary.
```

---
## \#19 Posted by: TowerCrisis Posted at: 2018-05-17T13:17:32.063Z Reads: 232

```
I'm talking about peak power draw.

Also, 2500 watts of battery current is easily within the realm of possibility of exceeding. That's 50 amps from a 50 volt battery.

I'm not just believing in marketing terms. My last build using a 10S2P lipo had peaks of 60 A. I opted to use a loop key because I was worried about longevity of an antispark.

And regarding why vesc's don't have integrated antisparks:
A VESC is designed for DIY pick and choose parts. To appeal to more users it's not included. If a user does not want to use an antispark, they simply don't have to. Adding an integrated antisparks to a VESC is is just going to take up more size, about as much as an external antispark would be anyways.

A business isn't going to go that route, because it's simply not appealing to consumers. Adding more components that can fail onto one PCB is going to cost DIYers more in the long run, as your repair costs and likelihood of failiure go up.
```

---
## \#20 Posted by: Maxid Posted at: 2018-05-17T13:31:22.033Z Reads: 233

```
As I said peak is meaningless, especially not when talking about the AS situation.

Also i don't believe that to be the reasons why the VESC has no AS built in.

I'd love to hear what actual electronics pros like @JohnnyMeduse or @SimosMCmuffin have to say on this topic.
```

---
## \#21 Posted by: linsus Posted at: 2018-05-17T14:24:34.095Z Reads: 250

```
Im an EE by occupation :zipper_mouth_face:
You seem hard to convince however. Not sure how I can explain things in an easier manner.
```

---
## \#22 Posted by: Colson003 Posted at: 2018-05-17T14:35:29.921Z Reads: 245

```
@Maxid have you seen the group buy @longhairedboy is doing for the new 100a maytech vesc? It has a built in switch like you’re talking about.
```

---
## \#23 Posted by: trampa Posted at: 2018-05-17T14:51:35.862Z Reads: 247

```
As an EE you know why you want the switch to be a separate part, especially if the switch isn't designed very well and will fail very soon, going to permanent ON mode. It would make more sense to integrate the switch into a BMS.
```

---
## \#24 Posted by: DevinG Posted at: 2018-05-17T14:54:45.983Z Reads: 244

```
...intergated antoispark from the vesc? Would that work idk just throwing pennies...
```

---
## \#25 Posted by: Maxid Posted at: 2018-05-17T15:22:50.818Z Reads: 231

```
You just seem not very constructive. Bashing the idea seems weird - there are ESCs out there already that have this functionality. So it must work somehow. Why can't the VESC do it? You also never answered the inrush question.
```

---
## \#26 Posted by: Blasto Posted at: 2018-05-17T15:26:33.322Z Reads: 222

```
It’s definably possible, proper gate protection and thermal protection is a must have. These are the two main reason why “anti spark” switches blow
```

---
## \#27 Posted by: linsus Posted at: 2018-05-17T15:48:35.415Z Reads: 203

```
You mean having charged caps on your inlet and then flipping the switch? Ofcourse things will happen. Sure, caps draw current to preserve charge in an attempt to keep voltage. But its essensially a big ball of energy waiting for something to happen. The AS increases the "turn on time" by slowly turning on the FETs. 
You cant accomplish this with the powermosfets controlling the motor. You would need separate FETs if you must have it integrated on the same card. On the subject of power electronics especially the driving of the FETs for motor control, its a very critical design aspect, using them for a combined purpose will only give you a headache.
```

---
## \#28 Posted by: Maxid Posted at: 2018-05-17T15:54:10.230Z Reads: 198

```
I stll don't get it. Why would I need FETs to turn on slowly? I don't need AS protection - this is not what this is about. My question is about having an on/off switch on the VESC directly.
```

---
## \#29 Posted by: linsus Posted at: 2018-05-17T15:59:40.254Z Reads: 198

```
The FETs on the AS turn on slowly, when they're "off" (Vgs < Vgth) the FETs has high impedance(Mega Ohms). By slowly increasing the Vgs the impedance falls, enabling the current to flow after awhile they're fully open(mOhms). Simply doing Off->On will produce the in-rush current we're so desperatly trying to avoid. 

If you want a yes or no answer. Yes, it is possible to intergate a functioning switch on the card. But you shouldnt use the Switching FETs alone for that purpose.
```

---
## \#30 Posted by: Kug3lis Posted at: 2018-05-17T16:33:12.827Z Reads: 182

```
If the mosfets wouldn't turn on slowly capacitors will consume over 500A current and blow the mosfets ;) that's is a problem of most anti spark switches big capacitive loads :) that's why you have sparks when you plug in because that large current inrush into vesc capacitors without any limitations...
```

---
## \#31 Posted by: Maxid Posted at: 2018-05-17T16:37:04.446Z Reads: 185

```
I don't want to use any FETs. Keep the capacitor connected to the battery for all I care --> no inrush.

@Kug3lis AS is not part of my question/this topic. I know how it works and I would like to not need one anymore.
```

---
## \#32 Posted by: Kug3lis Posted at: 2018-05-17T16:39:06.737Z Reads: 178

```
Then capacitors are useless because the additional tracks switches and etc will destroy their ESR capabilities ;)
```

---
## \#33 Posted by: Maxid Posted at: 2018-05-17T16:43:37.334Z Reads: 175

```
Why do hobby ESCs have this functionality then? :thinking: If the capacitors would be useless I guess the Chinese manufacturers would remove them to save cost - but they don't. Hobby ESCs also don't look like they have additional FETs built-in just for the switch. 
How are Roxxy ESCs able to do it for example?

@linsus I also found this statement from https://electronics.stackexchange.com/questions/304842/high-side-rc-esc-switch 
>This is a fundamentally bad idea. Electronic switches always have loss, and ESCs already put two in series with the motor, which have to be carefully chosen to minimize this. You now want to add a third, and of course circuit topology means you need to do it on the more difficult high side where P channel is weak and N channel means complexity. Instead, look to improving the control signal to the existing FETs. It usually comes from a microcontroller and typically is only enabled by an arming sequence. Replacement firmware is available for common implementations. 

I know too little about the electronic details but isn't he saying that you actually should do it the way i proposed?
```

---
## \#34 Posted by: linsus Posted at: 2018-05-17T17:10:46.626Z Reads: 176

```
[quote="Maxid, post:33, topic:55753"]
I know too little about the electronic details but isn’t he saying that you actually should do it the way i proposed?
[/quote]

Yeah, sort of. I get what hes coming from. With the added FET switch and losses etc, you just have to weight pros and cons. My guess is that even with that solution implemented he'd have a highcurrent on/off switch to still be able to completly separate from the source.

On the VESC the gate driver is the DRV chip. Now, I wont say I'm familiar with how the switching is controlled from the MCU. I try to stay far away from code. But hes proposing to do the turning on as a separate sequence through the MCU. Which will require you to do some software magic. 

If you google inrusher limiters they're pretty much in any application that draws a high current, often as a separate unit. If you've spent top bucks on some nice components you'd want to protect them for some pennies extra. 


If your really passionate about the subject go to vedders forums and ask, I'm sure you'll be provided with a comprehensive enough answer. 

Regarding the Caps, they need to be as close to the ESC as possible for best effect. One of thier benefits is keeping voltagespikes as smooth as possible during operation. Guess you'd call it decoupling somehwhat. 

I have one e-board(HW 4.10) with just a simple mechanical switch, no AS. Works alright.  you can even hear the "pop" from the current when turning on, but if/when the FETs finally blows, I'll only have myself to blame.
```

---
## \#35 Posted by: Kug3lis Posted at: 2018-05-17T17:39:18.837Z Reads: 173

```
It's hard to argue with person with little electrical engineering background (didn't wanted to be rude).

Regarding the post you found that's why I implement N channel high side switch which here at least no one is selling :) 

https://www.electric-skateboard.builders/t/selling-fatboy-sparky-switch-v1-0-300v-6s-14s-anti-spark-switch/54128

[quote="linsus, post:34, topic:55753"]
Regarding the Caps, they need to be as close to the ESC as possible for best effect. One of thier benefits is keeping voltagespikes as smooth as possible during operation. Guess you’d call it decoupling somehwhat.
[/quote]

Capacitors used and placed close to switching circuit is that because of their low ESR they can provide current spike faster than battery would which makes everything in waveform department much nicer you can find many videos on youtube about esc and capacitors :)
```

---
## \#36 Posted by: b264 Posted at: 2018-05-17T17:51:50.185Z Reads: 158

```
[quote="Maxid, post:11, topic:55753, full:true"]
A normal AS can’t handle 2500W. 50A continuous is the max any AS can handle.
[/quote]

Not the new one from @Kug3lis it's 300A continuous and it's overbuilt for a reason.
```

---
## \#37 Posted by: longhairedboy Posted at: 2018-05-17T18:28:03.137Z Reads: 150

```
because the BMS is  a better place for it if you simply can't stand having a discreet unit. 

because the switch will only turn off the ESC and none of the other stuff you've plugged into your pack via BEC/SBEC/UBEC unless that's included with the ESC. 

integrated power switches in ESCs are a great solution for minimal LiPo builds, however.
```

---
## \#38 Posted by: Maxid Posted at: 2018-05-17T19:15:25.794Z Reads: 147

```
He said himself it can do 50A and needs active cooling for higher current.

Edit: checked the thread again - it's 100A
```

---
## \#39 Posted by: Kug3lis Posted at: 2018-05-17T19:21:39.169Z Reads: 150

```
Lol, I said without radiator at 50A constant mosfet is warm, and yes for higher **CONSTANT** currents you need active cooling, because if you knew a bit about electricity you would calculate how much energy is dissipated as heat, you think at 100A there will be like simple part and it will do it without any cooling you are really wrong :D

[quote="Maxid, post:38, topic:55753"]
Edit: checked the thread again - it’s 100A
[/quote]

Point me where I said its only 100A? :D I have personally run over 300A using my lipos without any problem just needed to use a big as fan to cool it down ;) But for esk8 loads which currents are pulses this active cooling is not required if you not going to pull 100A for like 1min non stop
```

---
## \#40 Posted by: Maxid Posted at: 2018-05-17T19:23:54.186Z Reads: 145

```
Woah - all I said was that you need active cooling for higher currents. That's what you say in that thread. Not sure what your post is trying to tell me here. If you want to hear that you have the best AS available - you probably do. But I am not going to spend 70+€ for an AS on a second hand Lou board.
```

---
## \#41 Posted by: b264 Posted at: 2018-05-17T19:24:57.358Z Reads: 142

```
higher _constant_ currents, I think
```

---
## \#42 Posted by: Kug3lis Posted at: 2018-05-17T19:25:26.920Z Reads: 136

```
I don't suggest to buy for you ;) You just said there is no AS that can do more than 50A :) 

Myself I don't run switch as my build is just battery pack on board I just disconnect cable in the end I will use bms ;)
```

---
## \#43 Posted by: Maxid Posted at: 2018-05-17T19:27:19.331Z Reads: 144

```
True - it's frustrating when everyone is bashing the idea when I still don't understand the reason why. Hobby ESCs have done it and to me this is something a fancy ESC like the VESC should also have. How does Boosted solve this? Do they have a separate AS?
```

---
## \#44 Posted by: Kug3lis Posted at: 2018-05-17T19:29:12.235Z Reads: 144

```
Can you point out the ESC because apart new focbox and Chinease6 I dont know any with AS ;)

Boosted used BMS with switch, many modern BMS has switches inside if you don't ditch discharge part of it :)
```

---
## \#45 Posted by: Maxid Posted at: 2018-05-17T19:30:05.254Z Reads: 139

```
Just look at the Roxxy ESC that @Nowind was using in the early days. It could handle more current than VESC 4.12. And again: it's not about AS but on/off switch.
```

---
## \#46 Posted by: Kug3lis Posted at: 2018-05-17T19:31:48.595Z Reads: 133

```
Oh those switches just switch power to MCU, they don't disconnect whole ESC from power its super simple :) it could drain power over time from your battery :)
```

---
## \#47 Posted by: Maxid Posted at: 2018-05-17T19:33:52.467Z Reads: 129

```
Which is what I want for the VESC - the entire thread is just about exactly this. That's  why I don't understand the negativity. This should be simple to implement and the manufacturer should then have people decide if they want to use it or not. Give me two pins I can solder a switch to and I'd be happy.
```

---
## \#48 Posted by: Kug3lis Posted at: 2018-05-17T19:37:20.457Z Reads: 131

```
You had to state it that you want power switch only mcu not whole ESC :D I suggest to ask mods to delete this fight scene and create a new topic with exactly discussion about switching only power to the processor or in vesc case to DRV so it wouldn't generate 

@moderators
```

---
## \#49 Posted by: Kug3lis Posted at: 2018-05-17T19:37:57.350Z Reads: 126

```
P.S. Thank for this idea I will try to implement this in my next ESC design iteration :D
```

---
## \#50 Posted by: Maxid Posted at: 2018-05-17T19:40:32.970Z Reads: 128

```
My initial post does state that I just want to switch the brain components. Then I got into an argument with @linsus who thinks it's a bad idea to have the voltage connected all the time and the entire thing went South into a discussion about AS. I basically just want a fancy sleep mode in which the VESC does only use microamps and the receiver or BT module etc is off. That's how it should be for commuter boards that get charged often anyway. My actual hope was for a savy guy like you to come along and point out that you can already do that by shorting two pins or whatever. That would have been awesome.
```

---
## \#51 Posted by: Kug3lis Posted at: 2018-05-17T19:45:09.700Z Reads: 125

```
I am simple guy pull xt90 from battery pack done, my board is so primature at the moment, I just don't have time and resources sit down and finish all the small projects for it plus I am switching now to Evo project so its also hassle with 12S15P pack :D
```

---
## \#52 Posted by: Maxid Posted at: 2018-05-17T19:46:34.729Z Reads: 124

```
Loop key would only be a backup for me. The advantage of the Lou is its stealthiness and that would get destroyed with a large XT90 accessible on the outside.
```

---
## \#53 Posted by: Kug3lis Posted at: 2018-05-17T19:47:30.861Z Reads: 121

```
My stealthiness ends 200m ahead of me then people turn heads and drops jaws then I overtake sports car at red lights to change lanes :D
```

---
## \#54 Posted by: mmaner Posted at: 2018-05-17T19:49:04.956Z Reads: 123

```
I have found that the XT90s loop key is the most reliable switch available.  I've burned up at least 6 Anti-Spark switches & 2 BMS switches.  I'm done with Anti-Spark switches and I mostly use charge only BMS's now, so the field is a bit barren :slight_smile:.
```

---
## \#55 Posted by: Maxid Posted at: 2018-05-17T19:49:50.632Z Reads: 121

```
Wouldn't you then also profit from having a VESC built in switch? :wink:
```

---
## \#56 Posted by: Jc06505n Posted at: 2018-05-17T19:52:59.844Z Reads: 125

```
[quote="longhairedboy, post:37, topic:55753"]
integrated power switches in ESCs are a great solution for minimal LiPo builds, however.
[/quote]

[quote="longhairedboy, post:37, topic:55753"]
because the BMS is  a better place for it if you simply can’t stand having a discreet unit.
[/quote]

For my folks like me who need a ELI5 in this thread of intelligence and fuckery
```

---
## \#57 Posted by: mmaner Posted at: 2018-05-17T19:54:25.722Z Reads: 123

```
I don't see at as outlandish, but what happens when you have x2 VESC's or lights or USB charger, etc?.  The only practical use I see is when it's a small lipo build with a single VESC.  

Also, and this is what scares me, it's likely that a swich built into a VESC will use the same tech as an Anti-Spark switch...what happens when fails?
```

---
## \#58 Posted by: longhairedboy Posted at: 2018-05-17T19:55:54.023Z Reads: 123

```
[quote="Jc06505n, post:56, topic:55753"]
intelligence and fuckery
[/quote]

myriad, indeed.
```

---
## \#59 Posted by: Maxid Posted at: 2018-05-17T20:03:34.581Z Reads: 117

```
Which is why I said in the beginning that this is motivated by the Lou board. 5V rails etc. should be switched in the best case. So lights and stuff can stay connected and don't draw any power.
```

---
## \#60 Posted by: mmaner Posted at: 2018-05-17T20:04:05.289Z Reads: 118

```
Im not arguing with you brother, just offering insight.
```

---
## \#61 Posted by: Maxid Posted at: 2018-05-17T20:07:42.809Z Reads: 118

```
Didn't mean to come off hostile - I am sorry.

Boy this thread is getting to me.
```

---
## \#62 Posted by: mmaner Posted at: 2018-05-17T20:11:11.606Z Reads: 113

```
Its all good, I dig it, folks get invested and things get hairy.  Sometimes you just have to walk away.
```

---
## \#63 Posted by: BooYA Posted at: 2018-05-17T20:48:37.673Z Reads: 118

```
An on/off switch would be a cool feature to avoid complexity and losses.
I mean, having 3 fets in series vs 2 and only have to worry about thermal dissipation of the esc is a lot easier!
Also, the point about lights and BEC etc. Doesn't make any sense as a super tiny FET controlled by the MCU is so easy to implement in a BEC circuit.
Actually in many hobby ESCs the BEC is controlled by MCU and you can change its voltage in software.
```

---
## \#64 Posted by: BooYA Posted at: 2018-05-17T20:56:04.156Z Reads: 121

```
Also switching off only the MCU means very little energy is consumed as I often let my Lipos plugged in my RCs for days if not weeks and never noticed a voltage drop
```

---
## \#65 Posted by: BooYA Posted at: 2018-05-17T21:02:41.018Z Reads: 114

```
On the other hand, in most products involving ESCs and batteries, the power state is controlled by the BMS and not the ESC : e-bikes, commercial e-boards, and even DJI drones.
Must be a reason to this, probably fool-proofness
```

---
## \#66 Posted by: pat.speed Posted at: 2018-05-17T21:02:58.202Z Reads: 117

```
I have also never noticed a voltage drop when I was using car esc and left my lipos plugged in
```

---
## \#67 Posted by: TowerCrisis Posted at: 2018-05-18T00:20:54.698Z Reads: 108

```
That's likely the case for many designs, although I'm sure that ESC manufacturers advise against leaving batteries plugged in for a reason.
```

---
## \#68 Posted by: akelly Posted at: 2018-05-18T00:36:07.685Z Reads: 112

```
Wow I found this thread just now through Google, what timing. I was thinking about how wasteful it is to have a set of FETs in the BMS that have to handle the full current, since the VESC can do current limiting, all we need the BMS for is to check the voltage of each cell, and do balancing when you're charging.

So I was wondering if we could use a very low current BMS, not run any current through it, and just connect the BMS output to an input on the VESC to put the VESC in sleep mode. [Looks like Benjamin has thought about a sleep mode](http://vedder.se/forums/viewtopic.php?t=224), VESC 4 would take some significant modifications because the battery voltage measurement divider draws 1mA and cannot currently be disconnected, and was talking about putting it on the VESC 6, but I don't see a sleep mode connector on it.

Anyway, all you people wanting an antispark circuit built into the VESC know that antispark connectors exist now right? With a precharge resistor connected to the tip of the contact? [They're pretty great.](https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html?___store=en_us)
```

---
## \#69 Posted by: Barbara Posted at: 2018-05-18T03:43:02.731Z Reads: 115

```
The ESC6 we produce include spark switch and XT90 connector maybe you will interested. Below is the model picture of esc6 and can shipping out with waterproof aluminum case next Friday.
![image|666x500](upload://rnnnZP9qNGJaEmgf92zuYIvDWuM.jpg)
![image|666x500](upload://3I1OcedqlySVHyAoSX5ejjU8nyh.jpg)
```

---
## \#70 Posted by: esk8jpn Posted at: 2018-05-18T05:09:03.724Z Reads: 111

```
@Barbara

ESC6? VESC6?
Please tell me the dimensions of that aluminum case.
```

---
## \#71 Posted by: Barbara Posted at: 2018-05-18T05:12:52.925Z Reads: 108

```
The dimensions is 100mm*92mm
```

---
## \#72 Posted by: Maxid Posted at: 2018-05-18T05:25:23.124Z Reads: 111

```
I feel like this is the only helpful post in this thread that actually addresses my initial point. Thanks for the link - seems like Vedder was indeed thinking the same what I was thinking. Sad to hear that it can't be added easily to a Focbox or other 4.12 versions.
```

---
## \#73 Posted by: SimosMCmuffin Posted at: 2018-05-18T05:47:50.827Z Reads: 111

```
With regards to your actual question (I also understood it as an AS question first as well).

If the hardware is meant to support real "sleep mode" functionality with the Bus rail powered, then some special measures need to be taken to limit the "sleep mode" quiescent currents, if the desired current draw is meant to be in the microamp range.

Actual "sleep mode" could either be done via software or hardware, with "sleep mode" disabling and turning off, as much of the other circuitry as possible, but keeping the MCU powered and in a low-power mode. 
Hardware solution would be to for example to be able to hookup a switch to the DRV8301's "EN_BUCK" pin, which by pulling it low shuts off of the buck converter and by letting it float re-enables it. This might be un-ideal, as it would hard reset the MCU with possible erroneous  operation.

"Why is there no on/off switch integrated in a VESC"
Wasn't deemed necessary or other solution were found to be better/simpler.
```

---
## \#74 Posted by: esk8jpn Posted at: 2018-05-18T05:54:26.944Z Reads: 111

```
@Barbara

Thank you!
The switch seems to be better connected by a cable than it is fixed to the case.
Everyone wants to install the switch in the enclosure.
```

---
## \#75 Posted by: akelly Posted at: 2018-05-18T08:21:26.511Z Reads: 111

```
[I'll just quote Benjamin Vedder.](http://vedder.se/forums/viewtopic.php?t=224)

> Putting the STM in sleep mode and disabling everything that can be disabled can probably bring the consumption down to below 200 µA for almost everything, the only problem is that the input voltage measurement divider will still draw a bit over 1 mA at 50V input (the blue LED will also consume a bit, but it is not needed). Shutting the buck converter down with the enable pin will turn the 200 µA to something like 2 µA, but the 1 mA still remains. To deal with that it would be necessary to switch off the voltage divider, which requires two small FETs and a few resistors (just using a FET on the low side does not help since the clamping doide in the stm will still sink the current). Adding the two FETs and an input for a power switch could be worth it though, if triggering the switch from software is possible.

Personally I don't see any issues with a hard shutdown of the MCU. Break out the voltage regulator enable pin and tie it to your power switch and/or BMS output signal. The power LED runs on the 3.3V rail, so that'll turn off too.

I did some digging and found a couple options for the voltage divider. [This circuit](https://jeelabs.org/2013/05/17/zero-powe-battery-measurement/) only adds one FET instead of two, but you need to set the voltage divider so that the analog input is low enough that the gate gets above the gate threshold voltage, severely limiting your possible analog input range and resolution.
![image|186x258](upload://xVfl3w8cvvRocRTqMVFO1ICPpnF.jpg)

The other option is to use really huge resistor values, so the current draw is acceptable for long term storage, and then use a capacitor to store that voltage to allow it to be read by the ADC. To get under 1uA at 50V means 50 MOhm total for the voltage divider. The good thing is that the VESC already has a capacitor here, meaning we can just swap the resistors and capacitor for much larger ones and be good to go. Got to make sure the sample rate on this isn't too high though.
https://jeelabs.org/2013/05/16/measuring-the-battery-without-draining-it/

This actually seems like a doable path now, if not something one could recommend widely because of the delicate soldering required.
```

---
## \#76 Posted by: Maxid Posted at: 2018-05-18T08:26:08.657Z Reads: 102

```
love it - keep the ideas coming. this thread might be good for something after all :tada: You think this could be retrofitted to existing VESCs somehow?
```

---
## \#77 Posted by: BooYA Posted at: 2018-05-18T10:06:57.279Z Reads: 104

```
Guys, even if the consumption in sleep mode is about 1mA it means it would take more than a year to empty a 10Ah pack!
If you let your discharged battery in sleep mode ( let's say between 5% and 10% remaining capacity) we are dealing with an order of time of about a month, and I recall that leaving batteries fully discharged for extensive periods of time is not recommended, it should be stored at 60% ( aka about 8 months of sleep mode)
Don't know about you but I personally check/charge my board every three days...
Let's implement this feature!
```

---
## \#78 Posted by: Maxid Posted at: 2018-05-18T10:20:02.871Z Reads: 101

```
For extended periods of time I would mechanically disconnect the battery anyway. this is for situations where you ride your board every day on your commute - you'd then have to charge it every couple days so 1mA would not be noticeable.

I'm with you: 
>Let’s implement this feature!
```

---
## \#79 Posted by: trampa Posted at: 2018-05-18T14:35:09.386Z Reads: 99

```
And if you have an issue with your ESC and need to de-power fast (e.g. ESC suddenly starting to smell funny, accident etc.) what will you do? You will pull your saftey cutoff loop (a switch already) or deactivate your separate mosfet switch (another switch). Having a massive battery you will need a feature that allows you to separate the battery from the other electronics fast. Even if you have a switch inside the ESC, you still need a separate one, or a loop key for safety reasons. More switches - more complicated - more sources for potential issues. KIS is the way forward. Keep It Simple. The best part in a design is the part you can strip from your design.
```

---
## \#80 Posted by: Maxid Posted at: 2018-05-18T14:47:20.710Z Reads: 98

```
I am pretty sure that on a Lou board I'd have the battery disconnected just as fast (if not faster) than I would have removed the loop key. There is a difference between high power eMTBs and commuter boards. I know that as a DIYer I also tend to overbuild and rather use pneumatics etc. but the board that is built that way is not ridden nearly as often as the chinese crap commuter board that is lightweight and stealthy.
I need something that is hidden from view and the VESC does not offer that - which is a shame as it could clearly be added without too much hassle. Leave the decision which feature to use then up to the user.

Also to me KIS would be to not have to rely on an additional part (=whatever version of switch) that might fail but have it integrated into the ESC.
```

---
## \#81 Posted by: Deodand Posted at: 2018-05-18T16:12:16.569Z Reads: 92

```
Why are we talking about keep-it-simple design in regards to a low-side n-channel mosfet switch like its some space age technology no one fully understands? We already have a fully integrated FOC motor controller to maximize efficiency, this thing in no way is KIS design and its awesome. I'll take the intelligent designs of bold engineers over the designs of an over-cautious KIS engineer any day. There is literally 6 other low side and 6 other high side mosfet switches in every dual drive eskate board. Statistics will tell you adding one more shouldnt have a big impact on reliability. Trouble is somehow the designs of these guys just havent recieved the same attention as the vesc to maximize reliability. I think a few people have started to get them right now though. 


The main reason not to do it with existing vescs is that many people use two and having two parallel switches to drive is a bit strange but would probably work fine. A lot of people had problems with anti-spark switches because the fets are mounted to a tiny pcb with improper thermals. Additionally they may use the switch in a scenario it wasn't properly designed for. By integrating the power switch onto the motor driver, you know exactly the peak power the switch needs to handle as it is connected right there to the motor driver. You can also sink heat identically to how heat is removed from the other fets . You can just use the same amount of fets you use in the motor driver and know that they will generally see less heat anyways since motor amps>= battery amps. The wiring is also hard to screw up since it is pretty much just connect power to the vesc and plug in your switch.

I do also like the idea of a logic voltage switch. FYI there is an enable switch on the buck regulator of the drv8301 that you could break out to a 2 pin connector to achieve this functionality. Very clean and simple solution and the vesc itself shouldnt kill your battery for at least a few months I'd guess. This solution could get annoying for those with peripheral components connected to battery voltage though as those would need to be independently switched. For instance my battery voltage monitor would be too much passive drain. Perhaps a 2 pole switch controls both a low power battery voltage output on the board and the enable pin on the buck.
```

---
## \#82 Posted by: Maxid Posted at: 2018-05-18T17:33:35.665Z Reads: 88

```
[quote="Deodand, post:81, topic:55753, full:true"]
The main reason not to do it with existing vescs is that many people use two and having two parallel switches to drive is a bit strange but would probably work fine.
[/quote]

Wouldn't a single dpst switch already solve the two vescs in parallel issue?
```

---
## \#83 Posted by: akelly Posted at: 2018-05-18T17:55:28.957Z Reads: 86

```
You're like the fifth person to suggest the enable pin on the DRV now. I think you could connect the enable pins together between two VESCs without any issues, only thing I'm worried about is noise. The problem is the pin on the DRV are really freaking small to solder to. Hint hint, anyone making VESC 4 derivatives.

I'm less concerned with efficiency or simplicity for simplicity's sake, and more concerned with cost. Duplicating the high current FETs seems wasteful.

I was thinking about making my own BMS with all the features I wanted, and then I found the like 5 BMS projects on this forum already, and the amount of discussion in those threads is a little overwhelming. I'll have to do an analysis to see if there are any significant ways to improve over those.
```

---
## \#84 Posted by: Deodand Posted at: 2018-05-18T18:16:43.652Z Reads: 85

```
A SPST switch wired to both VESCs would probably also work for the two switches thing. Its just a  bit decentralized which makes it a bit weird from a design perspective. But that is just my opinion. 

Yeah, it really depends what the cost of your FETs are for the tradeoff. In general it will probably add 1-2 USD to the BOM cost depending. So after markup it does add some non-trivial cost. The thing is that in the event of software/hardware issues it is nice to have an independent circuit from the DRV8301 that cuts power completely...  Hard to say if that holds any merit without a lot of hardware failure mode testing. I imagine the fuse should blow during this scenario anyway.

It really is just a systems question and I think many answers here are good answers with trade-offs. My point is just that integrating the power switch onto the VESC as a lowside FET switch offers some interesting advantages, and will definitely draw less parasitic current in the off state; storing your board while your abroad etc. doesn't require you to open up your board and unplug the battery. 

I do agree with the OP that it is strange that a high end motor driver designed for electric skateboards requires you to go out and buy/build a separate power switch that can handle an unknown capacitive load during switching. Saying "just use a loop key" seems to be missing the point.   Its a bit complex for a newbie. You should be trying to offer an integrated and simple solution for your customers where possible and this seems like low hanging fruit to me to improve peoples DIY experience.
```

---
## \#85 Posted by: BooYA Posted at: 2018-05-20T13:25:27.961Z Reads: 74

```
Typical trampa post, nothing constructive or helpful ...
As you are in business with Vedder and the VESC project, you would be better addressing this potential feature and giving some insight :)
Also if the ESC starts burning, having a separate switch won't change the end result, it's not like you're faster than any electrical event. For example, even if you short your battery in any way, all the components and soldering would melt and open the short way before you have the time to disconnect. 
Or simply use a fuse...
```

---
