# Focbox factory mishap?

### Replies: 77 Views: 2717

## \#1 Posted by: Exiledd_Top Posted at: 2018-04-01T18:52:02.322Z Reads: 332

```
As you guys know I have a 4wd drive , anyways was riding like usual when I noticed one of my motors wasent spinning so I got home open the sucker up and at first I thought I fried the motor or something. I swapped the vesc and motor work , so then I thought DRV error because FOC hooked it up to computer no error code but won't supply power to the motor , things that I noticed when I opened it the heatsink for the phase wire chips the sticker was not taken off at factory and potentially ruining my phase wire connections I did solder my connections and resolderd my connections to check still nothing , my only conclusion was the sticker was ever taken off and the phase wire chips were never cooled .
Anyone else want to chime in a conclusion. Also I noticed that the vesc does not blink red/purple on start up like the other 3 vesc.
Things that bother me even if it was factory fault I got 4.5bullet connectors so I won't get a replacement so if anyone is willing to sell Me a focbox pm please need one.
![20180401_114127|374x500](upload://f59thU5PHc7U1srAYOSaRYcWeeX.jpg)
![20180401_114306|374x500](upload://nGLw7P1qiyaTCG9RXRi0SOwBrqr.jpg)
![20180401_114317|374x500](upload://rSAeMCDjhVJx7oqoKg7W6HRMFuM.jpg)
![20180401_114340|374x500](upload://8akplk2PSpZri1OzFD07M9aZPG0.jpg)
![20180401_114405|666x500](upload://3sKxV3l36vWeTjUQ97cn56kd9ah.jpg)
```

---
## \#2 Posted by: Deckoz Posted at: 2018-04-01T19:01:06.672Z Reads: 309

```
Your DRV is burned.. pin 29... Your buck regulator is dead so the stmf4 isn't getting power.

Replace the drv and it will likely be ok.

![Screenshot_20180401-150222|281x500](upload://pQjNJZ0Y7sHDt0h7RHLuXh0NsMO.jpg)
```

---
## \#3 Posted by: threebysix Posted at: 2018-04-01T19:11:09.111Z Reads: 300

```
oh woah, nice catch
```

---
## \#4 Posted by: skatardude10 Posted at: 2018-04-01T19:16:40.124Z Reads: 297

```
Second post I've seen here about these stickers not removed. This is a thermal pad, right? So when my two focboxes come tomorrow, I assume it would be wise to check that this has been done... eh?
```

---
## \#5 Posted by: mikenyc Posted at: 2018-04-01T19:16:49.582Z Reads: 300

```
![31 PM|206x231](upload://uarapqM5zngYlCIPgR0PqxXbe01.png)
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-04-01T19:18:51.895Z Reads: 290

```
I'll just buy another one fix the other one later but no one has them selling rn , I also had conservative settings dam 32amps bat and 65amps on motors. Can't be water damage my enclosure is sealed with weather sealing
```

---
## \#7 Posted by: Deckoz Posted at: 2018-04-01T19:20:59.101Z Reads: 289

```
Your D4 looks miscolored too.

![Screenshot_20180401-151223|281x500](upload://q9ShnKXgzcR03gEweNjZQhFJQtq.jpg)

Which is part of the buck circuit

![Screenshot_20180401-151623|281x500](upload://4X0k6o7XrtB6GIc4JyI8r2TOzR1.png)

![Screenshot_20180401-151932|281x500](upload://kA5Lj85mmrpZW0esVsv0Nb3zzrD.png)
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2018-04-01T19:21:54.707Z Reads: 267

```
D4 is Alright... It is the right component.
```

---
## \#9 Posted by: Deckoz Posted at: 2018-04-01T19:22:34.626Z Reads: 264

```
Im just going off pictures. You are the wizard :)
```

---
## \#10 Posted by: Blitz Posted at: 2018-04-01T19:23:01.237Z Reads: 262

```
should I open my focbox and make sure that the sticker on the heatsink is really gone?
My only worry being about thermal performance.
```

---
## \#11 Posted by: mikenyc Posted at: 2018-04-01T19:25:26.071Z Reads: 250

```
when things like this happens, are the factories responsible? it really messes things up for the company selling them.
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2018-04-01T19:25:35.394Z Reads: 244

```
Yeah, why not !!! It look like someone got too drunk during Chinese new year, and wasn't up to the task when he went back to work.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2018-04-01T19:27:14.655Z Reads: 246

```
[quote="mikenyc, post:11, topic:50891"]
it really messes things up for the company selling them.
[/quote]

Yeah, but what can you do about it, Sadly those kinds of thing are meant to happen when you ramp up production.
```

---
## \#14 Posted by: mikenyc Posted at: 2018-04-01T19:28:07.801Z Reads: 247

```
i would hope that the factory offers a warranty to enertion, considering the final product bears a sticker saying QC passed
```

---
## \#15 Posted by: mikenyc Posted at: 2018-04-01T19:31:35.902Z Reads: 250

```
check this out... from my raptor 2

edit: wait, actually, not from the raptor 2. this was the housing from the vesc i removed to replace the raptor 2 because the usb came off and needed to be resoldered.

![E528A2D6-261A-4E2C-AEDB-BC1657D0A637|375x500](upload://7wBsjBOb25e6CGPf1Gf64GiQDiV.jpeg)
```

---
## \#16 Posted by: Deckoz Posted at: 2018-04-01T19:32:00.914Z Reads: 247

```
But what about all this road debris on the fets?

![Screenshot_20180401-153120|281x500](upload://5QuclyNuzzXxgAdz4VNVMBXpOWm.jpg)
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2018-04-01T19:33:18.550Z Reads: 244

```
QC is Passed on the PCB not the assembly, and these kind of issue are pretty hard to find upon test and visual inspection since it doesn't really affect the functioning and it is a place where you can't really see it easily.

Yeah, I saw those, That the kind of things that screw you over.
```

---
## \#18 Posted by: Blitz Posted at: 2018-04-01T19:33:22.448Z Reads: 242

```
Can someone tell me what tool Do i need to open the back?
```

---
## \#19 Posted by: mikenyc Posted at: 2018-04-01T19:33:57.267Z Reads: 241

```
just unscrew it and then see if the sticker is on there, it's not hard
```

---
## \#20 Posted by: Blitz Posted at: 2018-04-01T19:34:10.792Z Reads: 242

```
-___- what tool.
```

---
## \#21 Posted by: mikenyc Posted at: 2018-04-01T19:34:26.510Z Reads: 225

```
lol... i think it's a 2mm hex
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2018-04-01T19:35:12.586Z Reads: 226

```
2,5mm hex :wink:

Edit: you can also use a flat screwdriver a dremel and a torch, but I could ended up not being covert by the warranty after :man_shrugging:
```

---
## \#23 Posted by: Blitz Posted at: 2018-04-01T19:36:35.520Z Reads: 226

```
Looks like my smallest hex doesn't go into the screw..
```

---
## \#24 Posted by: mikenyc Posted at: 2018-04-01T19:38:24.237Z Reads: 226

```
[quote="JohnnyMeduse, post:22, topic:50891"]
torch
[/quote]

TORX

do not use a torch! lol
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2018-04-01T19:39:14.842Z Reads: 217

```
:crazy_face::crazy_face::crazy_face: :man_facepalming:
```

---
## \#26 Posted by: ROFEN13 Posted at: 2018-04-01T19:41:24.972Z Reads: 217

```
Haha I read this and thought " yeah, of course it wouldn't be covered anymore. It will be  puddle."
```

---
## \#27 Posted by: SeanHacker Posted at: 2018-04-01T19:49:05.292Z Reads: 220

```
I'm not sure this would be considered "ramping up" production. It's more like they started a new season with already paid for product by the consumer (in nice words). When a company has customers make a prepayment (just look at the great Cyber Monday sale for instance ;) ) it wouldn't be considered ramping up. It would be considered a "group buy" in simple terms here on the forum. We all just waited 4 months for these products when they were supposed to be "in stock". They weren't in stock. There's nothing to ramp up. They are only catching up at this point. :)
```

---
## \#28 Posted by: Blitz Posted at: 2018-04-01T19:49:58.752Z Reads: 235

```
Instructions unclear opened bank safe.
```

---
## \#29 Posted by: SeanHacker Posted at: 2018-04-01T19:52:03.391Z Reads: 236

```
Make sure your thermal pads are on guys. Looks like they didn't pay attention to that also. 

Before...
![IMG_20180401_120727|375x500](upload://fCTRtoiyV110maKjToiJJCo2hNB.jpg)

After...
![IMG_20180401_120856|375x500](upload://1KiLG8ElpzFoUgy10gttw7nkM6t.jpg)
```

---
## \#30 Posted by: Blitz Posted at: 2018-04-01T19:52:39.371Z Reads: 220

```
I'm so gonna do a thermal paste swap.
```

---
## \#31 Posted by: SeanHacker Posted at: 2018-04-01T19:55:01.463Z Reads: 218

```
I'm not sure, but I think the thermal pads might be more efficient. @JohnnyMeduse would know way more about that though. He knows vescs very well.
```

---
## \#32 Posted by: Blitz Posted at: 2018-04-01T19:56:26.685Z Reads: 223

```
I got left  Pc thermal paste and If your into computer overclocking then you thermal paste makes a difference.

Like when Intel used/uses crap thermal paste from the Die to the plate on witch the heatsink lands on,
Well, people changed that to liquid metal some just high-quality paste and they say 20 degrees improvement.
```

---
## \#33 Posted by: SeanHacker Posted at: 2018-04-01T19:59:05.552Z Reads: 226

```
I'm into computers a little bit. Lol. Just didn't know for sure how these FETs would do compared to the padding in this application. Let me know how it works for you. I'm really curious. 

![IMG_20180317_142021|375x499](upload://wqFJ1NriPbWHdzDVZO4SsbNJ1NR.jpg)
```

---
## \#34 Posted by: JohnnyMeduse Posted at: 2018-04-01T19:59:12.301Z Reads: 221

```
Hey DUDE.... you do realize that first I not only referring to Enertion. But Instead, I'm using my experience to provide accurate information about the struggle of Rampin up production, in a field I've been working for the past 12Year, these kind of issue are happening to any growing companies who are trying to outsource their production.

[quote="Blitz, post:32, topic:50891, full:true"]
I got left  Pc thermal paste and If your into computer overclocking then you thermal paste makes a difference .
[/quote]

i won't recommend using something like since it has to be evaluated first to make sure the dielectric is sufficient not to short everything at high current. If you want to use it it is at you OWN risk.
```

---
## \#35 Posted by: Blitz Posted at: 2018-04-01T19:59:40.822Z Reads: 209

```
My paste is  non-conductive. I know at own risk, It's more of an idea Probably won't do it.
"is metal-free and non-electrical conductive which eliminates any risks of causing short circuit"
```

---
## \#36 Posted by: SeanHacker Posted at: 2018-04-01T20:01:57.606Z Reads: 210

```
I know dude. It wasn't a personal attack or anything. Just speaking from a business standpoint. Enertion has been one big kickstarter campaign since the reveal of the R2. It doesn't take a genius to figure that out. Just look at their posts, videos, and everything else. They're screaming it at us. I was just stating the obvious I guess. Sorry.
```

---
## \#37 Posted by: JohnnyMeduse Posted at: 2018-04-01T20:02:57.293Z Reads: 206

```
But also paste won’t have the same sort of thermals conductivity, since there is a gap between the fet and the heat sink.
```

---
## \#38 Posted by: Deckoz Posted at: 2018-04-01T20:06:08.342Z Reads: 214

```
[quote="SeanHacker, post:29, topic:50891"]
Before…
[/quote]

Your making me want to check mine now...

It's been fine as it's been cold out...but now I'm curious lol
```

---
## \#39 Posted by: Acidfie Posted at: 2018-04-01T20:07:16.508Z Reads: 218

```
just to be clear, if you're using 4WD with 4 VESC i really **CANT** imagine burning your drv b/c of overheating. this looks more like the street debris that @deckoz said.

also, because of the direct fets are very efficient and produce less heat than the normal fets.

also this: ![29|690x441](upload://rAdehof3ymuaVsvRTXPOZ02vJ4g.png)
```

---
## \#40 Posted by: Exiledd_Top Posted at: 2018-04-01T20:11:20.107Z Reads: 215

```
Given that I ride at 35mph to 40mph going to school and then two big hills my motors get but not to the touch. Enclosure is weather sealed but guess things happen trying to look for a focbox rn anyone willing to sell me one pm me please
```

---
## \#41 Posted by: b264 Posted at: 2018-04-01T20:16:12.590Z Reads: 204

```
[quote="Blitz, post:35, topic:50891"]
“is metal-free and non-electrical conductive which eliminates any risks of causing short circuit”
[/quote]

... straight from company marketing department whose only goal is for you to click "Buy", no matter what
```

---
## \#42 Posted by: Acidfie Posted at: 2018-04-01T20:17:50.662Z Reads: 206

```
still, you're using 4WD splitting up that load on 4 motors, i think you do not weight that much? 170lbs at max?

so drawing about 60 amps max would be split up to 15 amps per 1 motor, no way your fets overheat. **this is just a estimate from me**

so, i had the same thing my vesc shortet b/c of street debris from no protection against dust. you will likely get some metal parts inside your enclosure, i sometimes see metal parts on my motors. so i would say get some compressed air, blow your 3 vesc, and seal them.
```

---
## \#43 Posted by: Exiledd_Top Posted at: 2018-04-01T20:22:47.291Z Reads: 208

```
[quote="Acidfie, post:42, topic:50891"]
so drawing about 60 amps max
[/quote]
My battery doesn't pull 60 amps buddy that would be a joke, 120 amps(12s6p 30q BMS bypassed ) is what it pulls with each vesc at 32 bat 65amps on motors 
Anyways I just Want clarify am not attacking enertion or anything just wanted to know what was wrong and if my hypothesis was right.
Also the vesc that died was in the back so it could have bin debris but I dout it.
I will take a look at my other vescs and clean them ty for the advice
```

---
## \#44 Posted by: Acidfie Posted at: 2018-04-01T20:31:40.328Z Reads: 199

```
just to clarify this, you will never ever draw more than 60-80 amps continuous from your battery, i dont know why people always think this. do you have a metr software or a telemetry data logger?

i never talked about the maximum you can draw from your battery (from where should i know), i made a estimated amount of drawing amps when youre on your way to school and getting up that hill. you will never ever draw 65 amps per vesc **CONTINUOUSLY** this is just the peak value.

well i misread, that are your settings yes, this is a software LIMIT and the maximum value you set up. this does not mean youre pulling always this high amount of power from your bat or deliver to your motor.

it really doesnt matter how big your battery is because your splitting up the power on 4 motors, this just means it can deliver 6*20A = 120 amps, yes.

not even mine pulls that much and i weigh about 200 pounds and can easily getting up some steep hills with dual drive.
```

---
## \#45 Posted by: banjaxxed Posted at: 2018-04-01T20:32:00.625Z Reads: 189

```
Don't you need the crush of a silicone pad if it's important you can swap it out for better rated GPU pad of the same thickness
```

---
## \#46 Posted by: Deckoz Posted at: 2018-04-01T20:36:11.892Z Reads: 197

```
[quote="Acidfie, post:44, topic:50891"]
i dont know why people always think this
[/quote]

I agree with most of what you've said.. but pulling 100+ amps from a battery is pretty easy to do. Start from a stand still and floor it up a hill..(a steep hill not a bitch hill)


Plus his amp limit is really 32a per esc.. so up a hill as duty increases hell just max the battery amps.. but still 32 battery amp is chump change for the focbox..
```

---
## \#47 Posted by: Acidfie Posted at: 2018-04-01T20:40:36.916Z Reads: 193

```
yes sure, you're totally right! but that is not what i meant. 

imagine having a 4wd board. now doing a start with maximum acceleration 0 - 40kph. this is what happens:

BAT amps will spike to lets say 120 AMPS

getting divided to 4 Focboxes

means every focbox getting about 30 Amps

i think a focbox can handle 32 amps (this is maximum power he can get with this board) continuously with ease while not getting overheatet.

so in this conclusion, the burnt drv is not from overheating because pulling to much amps.
```

---
## \#48 Posted by: Deckoz Posted at: 2018-04-01T20:43:06.607Z Reads: 188

```
Yep I completely agree with all of that..


But it definitely is possible to pull what your battmax is in lower rpms as it's really in efficient (0-70% efficiency). So what ever your batt max is setup for if you give it full throttle up a hill, provided you don't overheat. You will pull your battmax.
```

---
## \#49 Posted by: Acidfie Posted at: 2018-04-01T20:53:51.500Z Reads: 186

```
absolutely correct. thank you for your informations.

this conclusion leads me to let @Exiledd_Top clean his vescs and get a good dust sealing for his focboxes. because this metal debris from the street will likely induce a short, just think of a little splinter got on the drv pins - boom fried!

this is no recommendation to not remove the plastic foil of the focbox. mostly this will be a PE-LD foil which has a very low thermal conductivity of k=0.1 - 0.4 W/mK, but since the foil is very thin it is likely that it wont isolate the heat on the fets, which means it will isolate a defined amount of heat but not everything. the focboxes also have limits for the temperature which means if the mosfet temp is reached the focbox will likely shut down.
```

---
## \#50 Posted by: mmaner Posted at: 2018-04-01T21:03:19.463Z Reads: 182

```
Did you check with @longhairedboy?  I thought he had some. Also check with @JohnnyMeduse, he can repairs your dead in and may have some to sell.
```

---
## \#51 Posted by: Exiledd_Top Posted at: 2018-04-01T21:12:25.956Z Reads: 185

```
[quote="mmaner, post:50, topic:50891"]
Did you check with @longhairedboy?  I thought he had some.
[/quote]

He's on backorder, trying to buy, two day shipping type of thing and be up and running within like wensday, fixing it will take 1-2 weeks which I will do but need another one you know lol.
```

---
## \#52 Posted by: mmaner Posted at: 2018-04-01T21:13:46.179Z Reads: 179

```
I can dig it, been there myself. If I had an extra I'd send it your way. I'll look around see what I have, may have something.
```

---
## \#53 Posted by: JohnnyMeduse Posted at: 2018-04-01T21:16:33.471Z Reads: 178

```
Send me the defective one I will repair it !
```

---
## \#54 Posted by: Exiledd_Top Posted at: 2018-04-01T21:19:21.973Z Reads: 181

```
Someone already offered to repair it. Its okay the repairing part rn is not the issue is getting a new one within 4 days and then repairing it the old one.
```

---
## \#55 Posted by: GrecoMan Posted at: 2018-04-01T21:30:01.641Z Reads: 178

```
you want a chaka vesc? it’s got no heatsink but runs like a dream
```

---
## \#56 Posted by: MannyM0E Posted at: 2018-04-01T21:30:15.151Z Reads: 177

```
I also just got 2 focbox and after reading this I instantly went to checked to and see if tape was removed.
```

---
## \#57 Posted by: Exiledd_Top Posted at: 2018-04-01T21:31:28.159Z Reads: 179

```
Were u located
```

---
## \#58 Posted by: GrecoMan Posted at: 2018-04-01T21:32:21.533Z Reads: 182

```
MI

i can ship tomorrow
```

---
## \#59 Posted by: Mobutusan Posted at: 2018-04-01T22:05:32.778Z Reads: 178

```
I might be able to spare one. I'll PM you.
```

---
## \#60 Posted by: ThermalM16 Posted at: 2018-04-02T19:32:27.653Z Reads: 171

```
@Exiledd_Top sorry to hear about the bad luck with your FOCBOX. It looks like Enertion has assigned me to your case. I have all of the parts in stock for the repair, so I'm going to try to have it repaired and on its way back to you within  day or so of receiving it.
```

---
## \#61 Posted by: skatardude10 Posted at: 2018-04-02T22:24:51.541Z Reads: 168

```
Just checked my two new focboxes fresh from Hong Kong and both thermal pads were properly applied with the film removed. They weren't positioned exactly ideal, but plenty good enough. Moved them a tad for the slightly better coverage regardless. Good to know this isn't happening to every focbox.
```

---
## \#62 Posted by: Exiledd_Top Posted at: 2018-04-04T23:44:08.995Z Reads: 170

```
Hey guys just a friendly reminder I just purchased a focbox from a forum memeber brand new and the sticker was not peeled either, make sure to check your guys focbox if it was peeled or not. I understand mishaps.

![IMG_1169|669x499](upload://aNixRdI47K7bGjjZH5KDv0m8Ziq.JPG)
![IMG_1170|669x499](upload://czU0KWebwJaQmuYm5QzKtLUIb03.JPG)
```

---
## \#63 Posted by: Mobutusan Posted at: 2018-04-05T04:08:18.914Z Reads: 167

```
@Exiledd_Top Well, I had to go check the other FOCBOX that came with that one and sure enough, sticker was still there. This one and the one you have were delivered early-mid January, and I'm guessing they must have been from the actual "in-stock" FOCBOX's from Cyber Monday. 
![20180404_183623|666x500](upload://8X02DPWdx6EWYaqc9bGMHRlc09o.jpg)

I checked 2 of the other 4 FOCBOX's I ordered the day after Cyber Monday that didn't show up until around March, and the sticker is removed on those. I think these must be from the newer batch and newer factory, since the serial numbers on them look different. 
![20180404_185400|666x500](upload://ixpx8rDZjFmTSW2ICrsnpyE45II.jpg)
```

---
## \#64 Posted by: CCU Posted at: 2018-04-06T11:22:13.295Z Reads: 158

```
Thanks you all for letting me know!
I opened my Focbox and the thermal pad in mine isn´t big enough to cover the fets. Would have hated to destroy it and have to send it back. Glad I just received it and is still in the testing fase.

I emailed Enertion and the complete response was "the thermal pad is 2mm thick." Would have been nice if they had offered to send out a new pad.
Yes, the thermal pad is rather inexpensive. But buying a single pad plus shipping runs about 20 euro, which as a student isn´t nothing. Plus it is their mistake. Shouldn´t really have to pay for fixing it.

Also I find it quite odd that they didn´t even ask for a serial number too identify where the problem came from. Makes it look like the don´t even care about there own product..
```

---
## \#65 Posted by: cypa9904 Posted at: 2018-04-06T12:24:30.190Z Reads: 152

```
Can you tell me what it does?
```

---
## \#66 Posted by: SeanHacker Posted at: 2018-04-06T12:34:05.069Z Reads: 154

```
It's a thermal pad that transfers heat from the fets to the heatsink. That sticker should've been taken off at the factory and not left on.
```

---
## \#67 Posted by: telnoi Posted at: 2018-04-07T02:28:48.230Z Reads: 139

```
Mine (bought last year) were fine, though the soldering of two phase leads was sub par. Wire was frayed/not enough solder.
```

---
## \#68 Posted by: hyperIon1 Posted at: 2018-04-07T04:03:12.969Z Reads: 140

```
ok, after reading this thread I went to my stock and found all have the clear sicker. so the conclusion is thats bad and reduces the transfer of heat?
```

---
## \#69 Posted by: Exiledd_Top Posted at: 2018-04-07T05:05:51.192Z Reads: 138

```
Yes, suppose to transfer heat but if there not contacting then its not really transferring the heat from the mother board
```

---
## \#70 Posted by: mikenyc Posted at: 2018-04-07T12:37:49.512Z Reads: 130

```
i bet all these thermal pad oversights are from one guy on the assembly line. someone needs to go to china and crack the whip
```

---
## \#71 Posted by: Mobutusan Posted at: 2018-04-07T20:55:41.416Z Reads: 123

```
That's what I was wondering, and why I posted the pics with the different serial numbers (fonts). I _think_ the ones with the thermal pad issue could have come from the old factory; the same one that supposedly lied about having 500 units in stock for black Friday. Maybe that factory had issues extending beyond just lies about available stock. Hope it's nothing more than the pad stickers though.
```

---
## \#72 Posted by: JohnnyMeduse Posted at: 2018-04-07T21:03:18.886Z Reads: 122

```
They are all from the same factory, they didn’t change their PCB factory.
```

---
## \#73 Posted by: Mobutusan Posted at: 2018-04-07T21:17:10.695Z Reads: 122

```
Oooh, I thought they changed factories after the black Friday fiasco and had to fight and wait to get their hands on the remaining, finished inventory. So, they just fired all the factory staff that were working on FOCBOX production? I'm still trying to understand how/why my 158xx FOCBOX order came in January, but my 153xx FOCBOX order came close to March, and what really went on behind the scenes with Enertion.
```

---
## \#74 Posted by: JohnnyMeduse Posted at: 2018-04-07T21:31:12.687Z Reads: 121

```
They fired the staff that was working on the Raptor, but since they where in charge on getting all other production going in different factories, you can guess that was where the nightmare began. The new team is using the same factory for the Focbox assembly, but they might have change a few processes (which could include serial number).

And believe me they are probably getting accountable for the mistakes that are happening, with the transfer pad.
```

---
## \#75 Posted by: Quiles Posted at: 2018-04-08T12:18:59.098Z Reads: 111

```
Same here. The sticker was still there. ![20180408_091020|666x500](upload://mrmVf57y3mXE39TBb9n3FEyR2vv.jpg)
```

---
## \#76 Posted by: ethel Posted at: 2018-04-12T00:15:23.146Z Reads: 102

```
:sweat:

![IMG_0460|375x500](upload://1ouf3Wq2atAIykFmz0gjd12gy7e.jpg)!

![IMG_0459|375x500](upload://58OnDEppLmFLClq35UOlUQgQe3S.jpg)!

![IMG_0461|375x500](upload://7cjCeNCgPOiPOIaGaOlAb30TrNY.jpg)
```

---
## \#77 Posted by: briman05 Posted at: 2018-04-20T21:36:46.003Z Reads: 83

```
Since a lot of people had the clear film still on there Focboxes I had to check mine to give myself peace of mind and I didn’t have the film but the thermal os was slightly off on one of them
```

---
