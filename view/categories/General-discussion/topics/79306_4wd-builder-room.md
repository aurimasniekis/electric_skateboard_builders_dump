# 4WD builder room

### Replies: 123 Views: 1499

## \#1 Posted by: Winfly Posted at: 2018-12-29T11:10:46.056Z Reads: 341

```
How do you route the battery terminal for 4WD? I know for top mounted trampa and MBS all you need to do is parallel battery terminal leads. Have anyone else besides from @mackann done a 4WD on a street deck?

I'm thinking to building a HAYA 4WD with TB DD with my modules. With a lack of a center channel I can't imagine doing a terminal lead split. Also long battery wire produce high inductance and can potentially blow VESC. Something 270uF per ft is required. I'm thinking of opening the series connection at the middle of the pack for the other side of the ESC. Afaik, both sides should read 6s from ground through other ESC and 6s from other ESC back to positive. Is there anything wrong with this design?. Pic TMR.

What i concern most is voltage drop across ESC and uneven load distribution between front and back.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-29T11:14:40.794Z Reads: 309

```
I have just done a top mount quad, but why not to split your battery in two packs?
on for the front, one for the back.
no issues anymore.
```

---
## \#3 Posted by: Winfly Posted at: 2018-12-29T11:15:34.073Z Reads: 306

```
Yeah but but that will require 2 separate BMS and 2 charge port? How does that eork?
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-29T11:17:02.986Z Reads: 303

```
if you go 10s that´s definitly also no issue.
there are super small micro bms.
even with 12s a d140 is not really big and can just be placed on the top of the pack
```

---
## \#5 Posted by: Winfly Posted at: 2018-12-29T11:19:27.080Z Reads: 289

```
Space is not an issue with a 12s4p 4wd on HAYA with my modules. But I do plan on using D140. Just trying to think of a clever way to do this but the more I type the more i realized it might not work.

Cus essentially. If the load distribution is off. When the heavier loaded side need more current, it will need to pull that much through the other ESC.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-12-29T11:20:51.697Z Reads: 264

```
just place the packs in a cyrcle than.
so the main terminal is in the middle of the deck.
same length of wires to both sides.
should be easy peasy
```

---
## \#7 Posted by: Winfly Posted at: 2018-12-29T11:21:34.902Z Reads: 250

```
No channel to wire from middle to the sides. If I use my modules, which I am currently pretty stubborn on.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-12-29T11:23:22.837Z Reads: 248

```
so you have place for a d140 bms, but not for the wires? :thinking:
how tight your modules sitting in the deck?
do you have a picture?
```

---
## \#9 Posted by: Winfly Posted at: 2018-12-29T11:27:31.633Z Reads: 254

```
Don't have a HAYA yet, but here:
https://www.electric-skateboard.builders/t/haya-integrated-deck/68132/928?u=winfly

Module is 76mm wide exactly and 74mm long and 22mm tall.i wanted to do it this way because the balance wire will look so nice.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-12-29T11:29:06.894Z Reads: 241

```
flat copper braid, routed on fishpaper, maybe?
there should be enough space to route them under your packs to each side.
```

---
## \#11 Posted by: Winfly Posted at: 2018-12-29T11:32:37.873Z Reads: 242

```
Not enough height clearance. not a bad idea tho. Can't make the modules shorter unless I redesign the whole think to not use standoffs with I could.

Sorry if it sounds like I'm not buying any of your ideas. They are good but doesn't immediately clicks in my mind.
```

---
## \#12 Posted by: Andy87 Posted at: 2018-12-29T11:35:34.942Z Reads: 228

```
ok, so if you want it not other....
the haya is definitly strong enough to dremel out small chanels of 3mm to place the flat copper in it. 
you can even cover it than with fishpaper or silicon or silicon than fishpaper.
that should be bullet prove!
```

---
## \#13 Posted by: Andy87 Posted at: 2018-12-29T11:42:37.633Z Reads: 219

```
A bit an off topic question.
why you want to build a 4WD and than just go with 4P?
I mean i understand that there is not more space in the deck, but even if you use VTC5A with 35A it´s max 35A per vesc.
With VTC6 or Q30 it would be only 20A and 4WD will also reduce your range at min 20-40%.I don't see a real advantage with it for a street board.
```

---
## \#14 Posted by: Winfly Posted at: 2018-12-29T11:44:50.840Z Reads: 204

```
That I didn't consider.  The 4p modules just looks so nice in the HAYA. and leaves lots of room for 4WD.

Hehehe don't mind me fantasizing a clean AF build. :kissing_heart:
```

---
## \#15 Posted by: Andy87 Posted at: 2018-12-29T11:46:21.274Z Reads: 200

```
what you don't consider?
```

---
## \#16 Posted by: Winfly Posted at: 2018-12-29T11:46:38.853Z Reads: 212

```
The 20% range reduction and the current draw. Do I need that much draw tho. 

Theoretically, you will only draw more than 2WD during acceleration which last for < 10seconds and doing some extreme hill climb. And a little bit less efficient from the rolling resistance.
```

---
## \#17 Posted by: Andy87 Posted at: 2018-12-29T11:51:27.597Z Reads: 217

```
[quote="Winfly, post:16, topic:79306"]
Do I need that much draw tho
[/quote]

if no than quad doesn´t make a sense :sweat_smile:
besides the fact that you through some extra money and parts on the taple, add more stuff that can fail etc....
Don´t get it wrong, I totally can understand if you just want to make a quad because you want one :stuck_out_tongue_winking_eye:
My main reason was also, just because I can... but non the less, there is always the questioning if it makes sense for somebody or not.
```

---
## \#18 Posted by: Winfly Posted at: 2018-12-29T11:54:57.183Z Reads: 215

```
Might build it once for the frame and glory and revert back to 2WD for practical reasons. :stuck_out_tongue_winking_eye:

Unless someone pays top dollar for it.

Otherwise I can build a external pack to charge while riding or modify the lid to easily open and close like my hyperbeast and do swappable.

Can someone agree to disagree that splitting battery in the middle would work.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-12-29T12:02:30.726Z Reads: 206

```
I would split only with higher P groups.
In the first post I forgot that you can use max 4P.
2P would prop. sag really hard.
```

---
## \#20 Posted by: Winfly Posted at: 2018-12-29T12:08:13.154Z Reads: 207

```
Yup, also do you concern about slight difference in voltage between 2 packs. For example, one hits soft cutoff before the other. I guess you can put a huge resistor to parallel the two pack so it slowly even out.
```

---
## \#21 Posted by: Battosaii Posted at: 2018-12-29T12:36:21.052Z Reads: 183

```
Yeah I went from 4p dual to 8p 4wd I just doubled up everything. 

I used splitters but would save space if you wire 2 ESC to one XT90 connector. So you have much less connectors taking up space.
```

---
## \#22 Posted by: Friskies Posted at: 2018-12-29T12:37:06.993Z Reads: 178

```
Mam you know that I sold my haya because it's too tight for 4x4. I would get the Recurve instead so you will have a centre channel for all the electronics. Also I'm sure @chaka can chimme in on the long battery wires as he has been doing dual diagonal for a long time. I also think you'd be better with 5P for 4x4 as you won't have much headroom amp wise with the 4P.
```

---
## \#23 Posted by: Winfly Posted at: 2018-12-29T12:44:36.613Z Reads: 173

```
Where did you split the battery lead from and how long are your battery wire?
```

---
## \#24 Posted by: pat.speed Posted at: 2018-12-29T12:44:50.721Z Reads: 167

```
Can you use those super flat but wide ass cables that boosted uses under there deck, it’s almost like foil. It appears thinner than copper braid
```

---
## \#25 Posted by: Winfly Posted at: 2018-12-29T12:48:07.095Z Reads: 168

```
How wide? Let's assume it's 99% pure solid copper. 12 gauge wire has a cross section of 3.31mm^2.  Let's say I don't pad my battery modules. 0.5mm supposed height left from module, 0.1mm for fish paper insulating the copper strip. So 0.4mm thick copper requires 8.2ish mm wide for 12 gauge equivalent.
```

---
## \#26 Posted by: Battosaii Posted at: 2018-12-29T12:51:21.955Z Reads: 161

```
I have 2 battery leads soldered to the battery one is for the front Focbox and the other for the rear Focbox I used a TB splitter to split the ends to the Focboxes.

I used 10awg wire
```

---
## \#27 Posted by: pat.speed Posted at: 2018-12-29T12:52:11.914Z Reads: 169

```
According to some copper test data I have a 1mm thick, 10mm wide piece of copper will handle 66amps or equivalent to 9awg (I assume standard, not silicone wire)
```

---
## \#28 Posted by: Winfly Posted at: 2018-12-29T12:53:22.189Z Reads: 180

```
How long? And where is the terminal of the battery pack in respect to the deck (on one side of the board, or in the middle)? Did you just ignoring the long battery wire risk?

Also can someone explain where the inductance of copper wire comes from besides the spin of the multistrand bundle?
```

---
## \#29 Posted by: Battosaii Posted at: 2018-12-29T12:55:38.723Z Reads: 181

```
In my set up the wider part is the front so I have my BMS and wires coming out of the front. But the wires are not that long I never had an issue. Just don't make phase wires long. Battery wires have no problems.
```

---
## \#30 Posted by: Riako Posted at: 2018-12-29T12:56:06.447Z Reads: 181

```
![Capturepos|653x500](upload://3Gh5nEucqCMrNJIzOxT8nQNP7HC.jpeg) 
and smash two furrows?
```

---
## \#31 Posted by: Battosaii Posted at: 2018-12-29T12:56:35.783Z Reads: 176

```
Can't say how long exactly but it goes from the front of the battery back to the 2 Focboxes
```

---
## \#32 Posted by: Winfly Posted at: 2018-12-29T12:57:29.484Z Reads: 172

```
I read the oppositem. Let me pull out my bookmark.
```

---
## \#33 Posted by: Skunk Posted at: 2018-12-29T12:57:58.627Z Reads: 169

```
@Battosaii so are you running two 4p batterys? One front one rear?
```

---
## \#34 Posted by: Battosaii Posted at: 2018-12-29T12:58:40.241Z Reads: 173

```
No I'm running one 12s8p it sits in the middle of the 4 Focboxes inside the enclosure.
```

---
## \#35 Posted by: pat.speed Posted at: 2018-12-29T12:58:58.238Z Reads: 184

```
I thought it was the other way around, the phase could be long but battery shouldn’t.
```

---
## \#36 Posted by: Riako Posted at: 2018-12-29T12:59:17.586Z Reads: 190

```
Or like this : 
![Capture1cxv|656x500](upload://81BJiTNKOxyKHvcBg6dRdR0Bmsq.jpeg) 

here : 
![Capture2cdsg|626x298](upload://hw8qNNfx38q995sgrlMVLEMNADK.jpeg)

Edit: with the right tool depth at the wire diameter
```

---
## \#37 Posted by: Battosaii Posted at: 2018-12-29T13:00:28.589Z Reads: 183

```
Long phase wires will cause motors sync problems and will probably at best ride bad and at worst blow a drv. 

If you are worried about long battery wire you can always add some inline capacitors but I didn't need to with Focbox at least.
```

---
## \#38 Posted by: Winfly Posted at: 2018-12-29T13:00:29.220Z Reads: 185

```
Fk. Didn't bookmark it. Can someone link that one very detailed RCforum post on long battery wire v.s. phase wire. It has very good explanation and 3 different solutions.
1. Long phase wire, shot battery wire
2. Caps per length of wire
3. I forgot
```

---
## \#39 Posted by: Skunk Posted at: 2018-12-29T13:03:25.348Z Reads: 182

```
I've been wanting to build a second 12s4p and run two separate batterys with dual focboxes each split ppm to a receiver.  
Front and back would be independent from each other.
```

---
## \#40 Posted by: Winfly Posted at: 2018-12-29T13:04:21.221Z Reads: 177

```
Why????? You better have a good explanation for this.
```

---
## \#41 Posted by: Skunk Posted at: 2018-12-29T13:05:13.425Z Reads: 160

```
Fail safe. Even if one end fails i still have dual drive.
```

---
## \#42 Posted by: Skunk Posted at: 2018-12-29T13:06:15.935Z Reads: 157

```
Plus i already have a 12s4p
```

---
## \#43 Posted by: Andy87 Posted at: 2018-12-29T13:06:23.347Z Reads: 156

```
Even if 3 focboxes fail you still have one 👌
```

---
## \#44 Posted by: Sender Posted at: 2018-12-29T13:07:27.663Z Reads: 162

```
[quote="Skunk, post:42, topic:79306, full:true"]
Plus i already have a 12s4p
[/quote]

Thats the real reason lol
```

---
## \#45 Posted by: Winfly Posted at: 2018-12-29T13:07:31.013Z Reads: 159

```
Love that. If I take off 1 wire depth on each side. This seems to be the best solution.
```

---
## \#46 Posted by: Skunk Posted at: 2018-12-29T13:09:12.407Z Reads: 160

```
Yeah..... ill have a battery so big i can't lift it into my mini van some day.  Then ill sell the van. Maybe then Brian wil be proud
```

---
## \#47 Posted by: Winfly Posted at: 2018-12-29T13:09:52.018Z Reads: 157

```
Still don't like the 2 separate battery idea. 1 bms is so much cleaner
```

---
## \#48 Posted by: Riako Posted at: 2018-12-29T13:11:19.299Z Reads: 159

```
Yes, it let the top of the deck rest on the central wood spine, and yes 2 channel itch side sound perfect. Just find the good tool depth :)

_EDIT :_ You should be abble to find somethink identical with the bearing guide on the other side of the tool for your process ;)
```

---
## \#49 Posted by: Winfly Posted at: 2018-12-29T13:12:27.980Z Reads: 148

```
Thanks guys for helping with theory crafting idk if I will end up doing it :rofl:
```

---
## \#50 Posted by: Skunk Posted at: 2018-12-29T13:13:42.283Z Reads: 151

```
Meh.  I wanna play with a 4wd but probably not a permanent build. I like the idea of splitting it into two boards when im done. 
I guess you have that option regardless because of your compression packs.
I'm not sure how often id drag around a board that heavy.  Rather just have two builds in the end.
```

---
## \#51 Posted by: Winfly Posted at: 2018-12-29T13:14:58.769Z Reads: 147

```
How about 2 short decks that you can fold a truck each and can rejoin into a long deck. :rofl::rofl::rofl:
```

---
## \#52 Posted by: Skunk Posted at: 2018-12-29T13:15:25.857Z Reads: 147

```
007 shit lol
```

---
## \#53 Posted by: Winfly Posted at: 2018-12-29T13:15:47.310Z Reads: 148

```
So you can ride with your date/sprouse when you need to and have a powerful deck to shed.
```

---
## \#54 Posted by: Skunk Posted at: 2018-12-29T13:16:05.978Z Reads: 157

```
I also want a 13s build. Lol
I just wanna skate all the things
```

---
## \#55 Posted by: Winfly Posted at: 2018-12-29T13:18:13.872Z Reads: 164

```
007 ain't shit when you get Bollywood Production.

https://youtu.be/tsRgtaS70WA
```

---
## \#56 Posted by: Skunk Posted at: 2018-12-29T13:19:48.121Z Reads: 159

```
Haven't seen that in a bit lol
```

---
## \#57 Posted by: Battosaii Posted at: 2018-12-29T13:38:32.190Z Reads: 157

```
Yeah 4wd isn't for the faint of heart it's not a cruiser it's a fricken bullet and your better not let it catch you off guard. 

At 75% throttle I beat a Raptor 2 easily and there was a 100lbs+ differece in weight between me and the other rider. It's no joke.
```

---
## \#58 Posted by: directC Posted at: 2018-12-29T14:00:46.032Z Reads: 156

```
On side a you put the battery with + in the front
On side b you put the battery with - in the front

Now you can connect one side together and insert a spliter to the vesc

Am I seeing something wrong?
```

---
## \#59 Posted by: Winfly Posted at: 2018-12-29T14:05:38.981Z Reads: 157

```
Very long wire. Even tho it's not directly connected to the battery. It completes the loop for the power draw. Therefore there's the same amount of amp going through as the battery.
```

---
## \#61 Posted by: Winfly Posted at: 2018-12-29T15:10:49.551Z Reads: 144

```
Voltage difference for top ESC is 0.
```

---
## \#62 Posted by: directC Posted at: 2018-12-29T15:18:35.350Z Reads: 139

```
Isn't it anyway the same voltage? Or am I missing some important electricity knowledge
```

---
## \#63 Posted by: Winfly Posted at: 2018-12-29T16:09:23.589Z Reads: 138

```
It's a very simple mistake. Ignoring wire resistance. Any two point on the same wire has the same electrical potential. So at the top, the +ve and -ve are connected directly together on the same wire. So there's no potential difference across the +,-. 

P.S. Potential difference = voltage.

.
```

---
## \#64 Posted by: banjaxxed Posted at: 2018-12-29T16:12:22.435Z Reads: 129

```
Mmmmm no bueno! 💥
```

---
## \#65 Posted by: directC Posted at: 2018-12-29T16:13:55.410Z Reads: 134

```
acording to human history, i have to make a fire before i make a battery
;)
```

---
## \#66 Posted by: Winfly Posted at: 2018-12-29T16:21:46.058Z Reads: 136

```
My original proposal was to get rid of that portion of wire that connects +ve and -ve of top ESC. Creating 1 big loop with ESC splitting the half's of the cells. If you step back and treat ESC as a black box . Top ESC will see 6s + black box + 6s voltage, so hypothetical 12s voltage with some kind of load (black box magic in the middle). Similarly, the bottom ESC see the same thing. 

Now question is how do we model this black box?
```

---
## \#67 Posted by: banjaxxed Posted at: 2018-12-29T16:27:22.664Z Reads: 127

```
Don’t wink at me, that diagram exhibits a complete basic ignorance on how a battery works 👌

Let’s just patch over what I don’t know by patronizing another, all it takes is an emoji right?😉
```

---
## \#68 Posted by: directC Posted at: 2018-12-29T16:29:36.055Z Reads: 126

```
sorry :grin:
when i'm thinking arround something, i almost always forget something
```

---
## \#69 Posted by: banjaxxed Posted at: 2018-12-29T16:32:23.968Z Reads: 122

```
No offense but I would look at 2wd max if you’re not sure how to wire this. 4wd is not for the unacquainted
```

---
## \#70 Posted by: directC Posted at: 2018-12-29T16:34:04.963Z Reads: 121

```
but how should this make any fire? 
I mean it's just a normal battery with an extra loop thats not beeing used/shut down/how do i call this?
```

---
## \#71 Posted by: Winfly Posted at: 2018-12-29T16:37:46.795Z Reads: 131

```
I mean I know exactly how to wire this with split battery terminal. I was just wondering if anyone with experience had some secret way to make it neat. And brainstorm ideas. Bad ideas better than no idea. There was a fair amount of good info I got out of this theory crafting so the greed of my mind is satisfied atm.
```

---
## \#72 Posted by: banjaxxed Posted at: 2018-12-29T16:38:25.246Z Reads: 123

```
Nice slot/biscuit/groove cutter fits on yer router
```

---
## \#73 Posted by: directC Posted at: 2018-12-29T16:38:33.499Z Reads: 121

```
I think he wrote that to me :grin:
```

---
## \#74 Posted by: banjaxxed Posted at: 2018-12-29T16:38:57.123Z Reads: 125

```
I know you know
```

---
## \#75 Posted by: Winfly Posted at: 2018-12-29T16:39:14.286Z Reads: 129

```
Oh @banjaxxed bruh click reply to him. You got me confused. :flushed:
```

---
## \#76 Posted by: banjaxxed Posted at: 2018-12-29T16:40:17.540Z Reads: 127

```
No I’m not going to play, you will need to read read read, come back look at the diagram above, laugh or blush then hit delete

That is all
```

---
## \#77 Posted by: evoheyax Posted at: 2018-12-29T16:57:28.197Z Reads: 141

```
[quote="Battosaii, post:37, topic:79306"]
Long phase wires will cause motors sync problems
[/quote]

Never had any issues. Back in he day, Chaka told me it would be better to do long motor wires than long battery wires (i.e. put all of the esc's close together. Even then, I had issues with the battery wires being too long. More caps inline fixed it, but it is a real thing. Been riding 4wd for almost 3 years now without any issues.

[quote="Andy87, post:17, topic:79306"]
if no than quad doesn´t make a sense
[/quote]

Quad is great for a couple of reasons. I've lost a motor before, was able to make it back still. Beyond that, you have more and better traction (won't fishtail) and you'll put less wear and tear on your esc's and motors.

4wd is not for everyone. But if you want high speed on steep hills, it's the only way.

Personally, I don't know if 4wd is a good idea for a cruiser or not. It's a lot of power. Doubling the power does not just double acceleration. At some point, it will get significantly more powerful by just upping the watts a little bit. Long boards are better suited for 4wd stability.
```

---
## \#78 Posted by: Winfly Posted at: 2018-12-29T17:02:43.980Z Reads: 128

```
I think ppl should just try 4WD Chinese hubs with FS 4.20 dual. They are under power in 2wd but at 4wd and 30A. They should perform as well as a decent build at a lower cost.
```

---
## \#79 Posted by: Andy87 Posted at: 2018-12-29T17:08:20.887Z Reads: 133

```
If I lose one motor on a dual I still can make it home with one.
All depends on how you set up your board.
In the same way you can don’t make it home with a quad and one broken motor to look from the other side. 
I agree that you have less stress on your escs and your motors but this also again depends on your set up.
If you don’t add up your battery also a quad will not help you with traction on a steep hill.

Let’s say we have a 12s4p battery I can run 40a on two motors or 20a on 4 motors you will not have more power with it.
But with quad you definitely increase your break force.
```

---
## \#80 Posted by: evoheyax Posted at: 2018-12-29T17:14:01.284Z Reads: 134

```
those things can actually do 30 amps per motor? That's 1500 watts per motor. Can't imagine them lasting that on an uphill.
```

---
## \#81 Posted by: Winfly Posted at: 2018-12-29T17:16:33.207Z Reads: 130

```
I mean the FS dual 4.20 can do 30A so perfect for these if you don't want to use those Chinese ESC. If you doubt Chinese hubs 4WD. Have a talk with @pixelsilva.
```

---
## \#82 Posted by: evoheyax Posted at: 2018-12-29T17:16:45.545Z Reads: 120

```
I agree, a bigger battery is better. I have mostly used lipos for this reason. My 12s3p and 12s4p batteries have been disappointing...
```

---
## \#83 Posted by: Winfly Posted at: 2018-12-29T17:19:01.942Z Reads: 125

```
https://www.electric-skateboard.builders/t/bay-area-sale-acton-qu4tro-1-300/77937/30?u=winfly

Fyi I gave it a try with my hummies. Wouldn't go up and stalled. I'm so fking sad right now. I'm pretty sure its because Hummie V4 has terrible low erpm torque since they are not sensored. So it stalled and pulled max amp and the 6.6s gave up
```

---
## \#84 Posted by: evoheyax Posted at: 2018-12-29T17:19:57.225Z Reads: 126

```
Oh I don't doubt performance, especially at 30a, since I run the same settings on my hummie hubs.

I have ran vesc 4's up until now since I only need 30a per motor due to my battery limits.

But now that I have a much larger battery, I can finally up the amps with focboxes. Looking at a min of 50a per motor, to give 200a total. With 84mm wheels, I can't imagine how I will stay on it at full throttle... lol
```

---
## \#85 Posted by: Battosaii Posted at: 2018-12-29T17:27:48.961Z Reads: 126

```
Brakes are another big reason you can stop really fast. But I did have to lower the braking power compared to 2wd cause it was super touchy.
```

---
## \#86 Posted by: pixelsilva Posted at: 2018-12-29T17:30:26.257Z Reads: 138

```
![IMG_20180926_175304|281x500](upload://qQ35FDKC8rQ8WbWI2SsW5ZMXxtL.jpeg) 

600 + miles and counting. Probably not the speediest but no glitches, no lost signal, motors barely warm to the touch. Dust, dirt, wet streets, 100% starts all the time... never let me down. 

![Screenshot_2018-12-13-12-03-09|281x500](upload://15ITTiJcLpZOysnH87On2kiUXcT.png) 

I mean, riding over the worst streets and pavement of Northamerica...

![IMG_20181010_164738|690x388](upload://ifEz74yBoXN7lghhgrQGa60Ct2A.jpeg)
```

---
## \#87 Posted by: Winfly Posted at: 2018-12-29T17:38:24.416Z Reads: 124

```
I'm so sad i right now. Sob

Will do more testing to find out where my bottle neck is.
```

---
## \#88 Posted by: evoheyax Posted at: 2018-12-29T17:48:30.341Z Reads: 126

```
[quote="pixelsilva, post:86, topic:79306"]
I mean, riding over the worst streets and pavement of Northamerica…
[/quote]

What do you mean? We just received a passing score score that puts us in the "good" category for road quality... *rolls eyes*
```

---
## \#89 Posted by: Pedrodemio Posted at: 2018-12-29T17:57:28.774Z Reads: 113

```
What are your current settings? Or they are low or the hubs are saturating badly at higher currents
```

---
## \#90 Posted by: banjaxxed Posted at: 2018-12-29T18:04:47.593Z Reads: 116

```
Rich had no problems with this
https://www.electric-skateboard.builders/t/long-sensor-and-phase-wires/44639/3?u=banjaxxed
```

---
## \#91 Posted by: Winfly Posted at: 2018-12-29T18:09:33.980Z Reads: 118

```
60/-60, 40/-12, FS single 6.6s  at 13s4p, FOC sensor less. Motor peak 150A
```

---
## \#92 Posted by: Winfly Posted at: 2018-12-29T18:12:02.224Z Reads: 128

```
Pretty sure it was saturation. from my metr it slowly gain to 120A and then failed and falls back down. So 60A continuous per motor, which is at 6.6s he limit and setting limit.

Keep in mind it was a 30% grade hill and starting at the foot standing still. So no ramp up. 

Look at the hump at 16:39:25
https://metr.at/r/PQwXm
```

---
## \#93 Posted by: Pedrodemio Posted at: 2018-12-29T18:23:53.103Z Reads: 123

```
If possible try again with some speed, the efficiency of most BLDC motors is completely crap at low % of top speed
```

---
## \#94 Posted by: Winfly Posted at: 2018-12-29T18:25:32.482Z Reads: 120

```
I was trying to copy what @pixelsilva did with his qu4dro. That why I didn't get a speed up before hitting the slope.

 Should I lower min eprm from 150 to something?
```

---
## \#95 Posted by: Andy87 Posted at: 2018-12-29T19:45:27.158Z Reads: 116

```
Me either.
Had long battery wires on one build, long phase wires on the other.
No issues so far.
Both around 50-60cm.
But I use also 8awh for the main battery leads and 10awg for the phase wires.
Guess 10 and 12 would work too, but for me better a bit more than too less
```

---
## \#96 Posted by: pixelsilva Posted at: 2018-12-30T03:06:07.827Z Reads: 111

```
What do you mean with us? 'Us' like in the USA or 'us' like in California? Is very well known that California, and San Francisco in particular, have the worst highways and roads in the USA. Second to none. So true like tomorrow the Sun will rise. :roll_eyes:
```

---
## \#97 Posted by: evoheyax Posted at: 2018-12-30T03:12:14.164Z Reads: 109

```
No SF in particular. It was total bs. But the new outlets ran the headline a few months ago about how our roads have gotten so much better... lol
```

---
## \#98 Posted by: Hummie Posted at: 2018-12-30T03:19:42.284Z Reads: 117

```
@pixelsilva what speed will those motors go at what voltage?  IF the kv is lower they’ll get more torque per amp so if the esc limit is 120 they could be getting a lot more torque per amp.   u could either use an esc that could put out more amps or wind the motor for lower kv. Even if it were to saturate it would still increase torque with increased amps and it wouldn’t go completely to heat. Just the tips of the stator would saturate.


Acton I read is 23mph max speed. What voltage it run?
```

---
## \#99 Posted by: Noob-at-building Posted at: 2018-12-30T03:23:42.339Z Reads: 112

```
[quote="Winfly, post:1, topic:79306"]
I’m thinking to building a HAYA 4WD with TB DD with my modules
[/quote]

 Fucking Overkill much!
Jk love you, Ride safe
```

---
## \#100 Posted by: Winfly Posted at: 2018-12-30T03:30:06.276Z Reads: 117

```
Don't worry, no one knows what they are building until they have all the parts. It was just an idea. Might not end up building it depending on the circumstances when the DD comes out.
```

---
## \#101 Posted by: pixelsilva Posted at: 2018-12-30T03:30:50.336Z Reads: 122

```
C'monnnn!! we just need to head anywhere in the Bay Area and the highways are a disgrace. Dirty, full of trash, not well maintained, old, decaying, ugly.... they look ike they haven't received a major overhaul in decades! President Trump was right when he mentioned the US national infrastructure in general (airports, bridges, highways system, railroads, etc) are wayyy behind what you see elsewhere. Go to Europe, Germany, Scandinavia, Swisstzerland, etc, and you'll see better highways systems. 

San Franciscos 's streets are below many world capitals standards. Heck! my born city (Cali) down in Southamerica has more and much better streets than those here in San Fran, and that one  is three times larger than SF with 100 times less budget. There is no excuse. The Bay Area is home of seven of the worlds ten largest companies on planet Earth; we are talking trillions and trillions of technological powerhouses which makes California the 5th economy of the world. Just Apple alone has the entire budget of a Southamerican country....you telling me all that wealth.... and California has such shitty roads?? You got to be kiding!!
```

---
## \#102 Posted by: Noob-at-building Posted at: 2018-12-30T03:30:58.173Z Reads: 117

```
Yea i mean one is enough unless you wanna go like 100kmh
```

---
## \#103 Posted by: Noob-at-building Posted at: 2018-12-30T03:32:36.011Z Reads: 127

```
Yeahhhhhh, im just going to stick to Australia Roads
```

---
## \#104 Posted by: mackann Posted at: 2018-12-30T09:31:07.154Z Reads: 132

```
Don't have any problem with high inductance, the cables is like 38cm long. Have used both flipsky dual 6.6, flipsky 6.6 single and Unity. All pushed hard on high speed and high erpm and not a single damaged.
Here you can se the cables:
![IMG_20181019_165439_031|624x500](upload://fzZWKxRgvEs19FgncHE4QjiTdnQ.jpeg)
```

---
## \#105 Posted by: evoheyax Posted at: 2018-12-31T18:03:54.461Z Reads: 125

```
Why not stack the vescs? Like this:

![camphoto-1483920592|375x500](upload://tDGqPHvNvyGHriOAzVaURzKAICu.jpeg) 

Then, you can fit more battery! What is that battery btw? Love the work your doing btw!
```

---
## \#106 Posted by: Andy87 Posted at: 2018-12-31T18:14:45.960Z Reads: 119

```
But than he has 6 wires to run to the other side instead of two. If it’s already hard to route 2 wires this option will not work for him.
```

---
## \#107 Posted by: Winfly Posted at: 2018-12-31T18:26:59.984Z Reads: 117

```
theorethically long motor wire is better than long battery wire. Also 6x 12gauge is not that much bigger than his 2x 10? 8? gauge.
```

---
## \#108 Posted by: Andy87 Posted at: 2018-12-31T18:31:14.199Z Reads: 118

```
[quote="Winfly, post:107, topic:79306"]
Also 6x 12gauge is not that much bigger than his 2x 10? 8?
[/quote]

I let just this here
https://www.powerstream.com/Wire_Size.htm
```

---
## \#109 Posted by: Winfly Posted at: 2018-12-31T18:47:24.539Z Reads: 113

```
honestly it looks like he has room. I would rather has symmetry than stacking all on one side. plus I was thinking about doing it on the HAYA. I was just brainstorming and have minimum intend to follow through.
```

---
## \#110 Posted by: evoheyax Posted at: 2018-12-31T22:20:57.329Z Reads: 112

```
I think it looks better like this, but looks don't get you places faster. They don't win races. They don't get you that extra bit of range you need to finish the group ride.

But that's just me personally. I don't like any empty space, lol.
```

---
## \#111 Posted by: drone001 Posted at: 2019-01-27T15:32:58.874Z Reads: 101

```
I agree besides it's something about stacking speed controllers, makes my skin crawl...sorta like finger nails on a chalk board.
```

---
## \#112 Posted by: Sebike Posted at: 2019-01-27T16:20:55.919Z Reads: 100

```
[horror vacui]
```

---
## \#113 Posted by: youseekcota Posted at: 2019-03-01T18:37:51.460Z Reads: 95

```
Great thread! I'm just finishing up my 4wd @torqueboards / @psychotiller build. I'd love to hear what others are using for vesc 6.6 settings. I'm running four vesc 6.6's with a 12s6p lghg2 batteries driving four 6374's with 16-36 gearing on 107mm wheels. I used a PPM splitter to connect the front and rear masters to a single reciever, there are also front and rear slaves, that way I don't use a 4x Can bus which is risky, just two CAN bus cables connect each slave/master pair so I can keep traction control, which is a cool feature of the 6.6. I also use the throttle/brake curves for more more progressive brakes which come on a little softer then become progressively stronger the more you brake. The throttle curve is set up to be the opposite, a strong acceleration which tapers off towards the end which reduces the typical lurch as motors reach full power, it also reduces the risk of voltage sag.

I'm curious what vesc settings people are using for their 4wd setups. I was considering the following: settings for each vesc:

Motor max 80
Battery max 30 (30A*4=120A system total, right?) 
Regen          - 6 (-6*4= -24 system total, right?)

I'll be using the motor wattage limits at first to tone the board down a bit. 

Also, people have talked about inductance issues with extended power cables (I'm running about a foot long 8awg wire to power the front) there was talk in this thread about adding a capacitor to rectify this issue. Anybody have any additional thoughts or experience?
```

---
## \#114 Posted by: banjaxxed Posted at: 2019-03-01T18:41:34.011Z Reads: 93

```
Better to have longer phases than battery leads was my understanding. However placing a large 100v cap close to the 2nd Unity would be a fail safe way of ironing out any fluctuations, presumably the awg of the lead is 12 or even better?
```

---
## \#115 Posted by: youseekcota Posted at: 2019-03-01T18:48:16.121Z Reads: 88

```
Yeah, I've got 8awg all the way to the to the parallel splitters, then 10awg from those to the vescs.
```

---
## \#116 Posted by: banjaxxed Posted at: 2019-03-01T18:52:49.464Z Reads: 88

```
A big 100v cap inline before the 2nd Unity, simple cheap and effective peace of mind
```

---
## \#117 Posted by: gafoot08 Posted at: 2019-08-28T15:07:07.523Z Reads: 64

```
What is the reason for the cap before the 2nd esc?
```

---
## \#118 Posted by: banjaxxed Posted at: 2019-08-28T15:38:59.782Z Reads: 66

```
To store energy in case of a voltage/current drop, the capacitor kicks in. You could supplement the caps with additional caps if using a longer battery cable run
```

---
## \#119 Posted by: gafoot08 Posted at: 2019-08-28T19:32:17.084Z Reads: 69

```
Do you have a rough value for the cap you using?
And also how many caps per cable length perhaps?
```

---
## \#120 Posted by: Skyart15 Posted at: 2019-09-17T17:34:21.143Z Reads: 60

```
i have a question for you, i am thinking of building a board using the flipsky 6.6 singles, how did you connect the canbus, some sort of parallel canbus connector? do you use a single remote and transmitter? any help is much appreciated.
```

---
## \#121 Posted by: Brianr058 Posted at: 2019-09-18T23:00:33.251Z Reads: 54

```
What motors are you using? Hub, DD or belts?
```

---
## \#122 Posted by: Battosaii Posted at: 2019-09-18T23:28:05.785Z Reads: 51

```
Belts.

- 18t motor pulley
- 32t wheels pulley
- TB110mm wheels
- TB 190kb 6374
- Dual Unity
- 12s8p with samsung 30q cells.
```

---
## \#123 Posted by: mackann Posted at: 2019-09-19T13:01:30.202Z Reads: 47

```
Yes you parallell connect them with canbus cable, did solder the cable myself
![4b2b2179eb4cf3c3a5875f1f0f6fecfd0475ab82_2_1332x1000|666x500](upload://ife2xUUrkAAVoe2AshWBsY7iyQE.jpeg)
```

---
## \#124 Posted by: Skyart15 Posted at: 2019-09-19T13:12:15.348Z Reads: 46

```
And this allows for use with a single remote/reciever via uart? Like a vx1
```

---
