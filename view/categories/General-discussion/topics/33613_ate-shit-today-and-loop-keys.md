# Ate shit today and loop keys

### Replies: 50 Views: 2884

## \#1 Posted by: thisguyhere Posted at: 2017-09-21T02:45:43.789Z Reads: 458

```
power switch on my board had been acting up a bit the last couple days, where it would take like 10 seconds for it turn on after it was switched on.

then this morning i noticed power was cutting out and in, intermittently, for like 5 seconds, then it went along just fine.

so...feeling kinda sketch about my board in general, was going to open it up tonight to diagnose.

but on the way back home from work, i forget about all this, and in the last leg before getting home, there's a slight uphill that's really fun to bomb up, but this time during hard acceleration the power cuts out.  my center of gravity is set well behind the board anticipating the acceleration, and the sudden power cut throws me off at like 25mph.

heel of my hands are burnt off, both knee caps are raw, and left elbow looks like minced meat.  been downing red wine and beer to manage stinging rashes and hurt pride of falling in front of a shit load of people.

had a helmet on tho, so noggin's fine.

not sure what the point of the story is, just wanted to share.

oh, that and i'm going back to loop keys until i can get a hold of some bullet proof anti-spark switches.

edit: it wasn't the switch, it was bms cutting out due to voltage sag.  but the issue with board powering on after like 10 seconds of being switched on still persists.
```

---
## \#2 Posted by: willpark16 Posted at: 2017-09-21T02:49:07.859Z Reads: 431

```
Which switch?
```

---
## \#3 Posted by: thisguyhere Posted at: 2017-09-21T02:54:34.884Z Reads: 420

```
don't want to name specific switch, its vedders design, its the one with two MOSFETs. 

running 12s through it drawing 80a continuous regularly so been burning them out, so I'm using it beyond its design so can't blame whoever made it.
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-21T02:55:48.675Z Reads: 415

```
Your user logo is quite fitting ;)
```

---
## \#5 Posted by: notepad Posted at: 2017-09-21T02:57:24.511Z Reads: 401

```
I had a very simmilar problem,  it turns out the wires going to the switch itself were sub par and had problem with the vibrations degrading them.  Try resoldering new wires onto the switch terminals and check if that works.
```

---
## \#6 Posted by: thisguyhere Posted at: 2017-09-21T03:03:55.653Z Reads: 391

```
gotja, will take a look whenever I feel well enough to look at my board again.
```

---
## \#7 Posted by: Jinra Posted at: 2017-09-21T04:00:54.528Z Reads: 370

```
Ouch, been there done that. Glad you're alright, fix up that board!
```

---
## \#8 Posted by: Brad Posted at: 2017-09-21T04:10:50.066Z Reads: 374

```
I always wear gloves and helmet at a minimum.

These are what I wear, never hurt my hands and it allows me to slide on it.

<img src="/uploads/db1493/original/3X/0/9/097337715cd09da22b9c25bcf469f8134677bb1f.JPG" width="384" height="384">
```

---
## \#9 Posted by: Aeroquiv Posted at: 2017-09-21T04:18:51.199Z Reads: 363

```
They stopped selling those gloves. Their 2nd version is 3 times the price. :laughing:
```

---
## \#10 Posted by: RootedSuperuser Posted at: 2017-09-21T05:02:02.086Z Reads: 364

```
I had the problem with the original Safety Power Switch, made in Germany.
They rate the switch too high, they needed to reduce the rating by 30% and this would qualify  a 10S4P as an OK current flow with enough overhead for the draw needed for long uphill runs. 14S6P is not what it can handle, but it is what it is rated for.
The solder heats up on the PCB, flows up the MOSFET terminal causing a short.
<img src="/uploads/db1493/original/3X/f/b/fbec8f96541097c04af56be46243c718b0f845e0.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/2/c/2cac0600dfc7d93afba3f63be3965d5c8ddb8a3c.jpg" width="281" height="500">


The Vedder can be over built, and in doing so better MOSFET's can be utilised, up to 75Volts 240Amps and beyond..
<img src="/uploads/db1493/original/3X/6/a/6ae5a48c936ddbe291015e9b11abd61372c77a2a.jpg" width="378" height="499">
Where the problem is, I believe, is the thickness of the copper, it can't handle the current and consequently heats up and reflows. The VEDDER PCB needs  MILSTD traces or at least 2½ Oz copper, possibly a redesign to a 2 or 3 layer PCB, possibly even a laser/spot weld instead of silver or lead solder....

The use of various different passive heat sinks is recommended, but the problem still persists that the PCB is heating up past the flow temperature of the solder, and causing a short on the mosfet. The higher capacity mosfet, the need for 6 connections, vs the 2 needed for the SaftyPowerSwitch.
<img src="/uploads/db1493/original/3X/a/f/af7d208c1a3eebb3973c135da5529a90981714bf.jpg" width="570" height="499">

Please, do a close examination of the circuit and post your findings back here.
```

---
## \#11 Posted by: Crossfire Posted at: 2017-09-21T06:17:04.744Z Reads: 324

```
Same here, man. My mosfet switch started acting up too, that s**t needs to function 24/7 100%, so it was taken out and substituted with diy anisparkloop switch with regular XT90, 100ohm resistor and a rocker switch. Bulletproof. Resistor slow charges the caps and loop key powers it to the batttery voltage.
```

---
## \#12 Posted by: Tuomalar Posted at: 2017-09-21T08:24:13.122Z Reads: 306

```
This is why XT-90s is so amazing. Mosfet switches look nice but if you really want bulletproof board then use loopkey.
```

---
## \#13 Posted by: bigben Posted at: 2017-09-21T09:06:53.061Z Reads: 306

```
What gloves are those?
```

---
## \#14 Posted by: Brad Posted at: 2017-09-21T09:18:12.162Z Reads: 308

```
Knox Oryx gloves.

Evolve motor mount snapped and the belt was pushed into the wheel throwing me off at around 36ish km/h.

<img src="/uploads/db1493/original/3X/6/c/6c970dd8d75098d406d8aad75088edba0b59c427.jpg" width="690" height="202">
```

---
## \#15 Posted by: Vanarian Posted at: 2017-09-21T10:19:25.458Z Reads: 301

```
No, don't do this. When you want to cool FETs do as follow instead : 

<img src="/uploads/db1493/original/3X/4/e/4e861c3de9bf34bb0fa5fc79594bd928775d8b79.jpg" width="570" height="499">

BTW it will also help dissipate heat from the PCB.

Thank you for posting the original pic, it will save me precious time when trying to explain it. Keep them FETs cool !

@Tuomalar I know few people who got XT-90S fail on them. They upgraded to custom antisparks or relay solution. Still reliable connector but everything can happen unfortunately.
```

---
## \#16 Posted by: darkkevind Posted at: 2017-09-21T10:20:19.644Z Reads: 284

```
Injury photos or it never happened! Lol
```

---
## \#17 Posted by: mccloed Posted at: 2017-09-21T15:57:32.436Z Reads: 272

```
Sounds like a nasty fall. Hope your ok. You could take a spot next to @psychotiller to recover. I took a nasty spill at 25mph in San Diego and messed up my hip for two weeks. Luckily I was wearing gloves so I didn't mess up my hands too much. My hip took all the impact.
```

---
## \#18 Posted by: psychotiller Posted at: 2017-09-21T16:16:58.412Z Reads: 269

```
Feel better soon brotha!
```

---
## \#19 Posted by: RootedSuperuser Posted at: 2017-09-21T16:28:24.412Z Reads: 275

```
<img src="/uploads/db1493/original/3X/8/c/8cd3d3a5282f485afb13869cee952562e9310d09.jpg" width="343" height="300"> ur phunny....

If you are building from scratch, lap both flat 1st, it works better for thermal adhesive.
You can lap it flat with a 500-1000 grit sharpening stone, **wet** and dry sandpaper works well if it is on a flat surface.
FET's are made from silica (glass), so they take this treatment well,
Not too smooth, you want the thermal adhesive to have some purchase on both surfaces.
<img src="/uploads/db1493/original/3X/b/1/b1a5d6003f36c2969497baf1765384354ae5aa3d.jpg" width="622" height="500">
```

---
## \#20 Posted by: deucesdown Posted at: 2017-09-21T17:32:56.463Z Reads: 256

```
I thought these switches, when they failed, usually go closed circuit (ON)? Scary shit.
```

---
## \#21 Posted by: RootedSuperuser Posted at: 2017-09-21T22:16:18.599Z Reads: 250

```
[quote="deucesdown, post:20, topic:33613"]
when they failed, usually go closed circuit (ON)?
[/quote]

Depends on how they fail. Mine was stuck ON, the solder bridged the MOSFET leads, that's not a problem, the motor is controllable.
Having it power off as you prepare yourself for acceleration ..... Not Good.
```

---
## \#22 Posted by: thisguyhere Posted at: 2017-09-21T22:42:36.319Z Reads: 255

```
[quote="Brad, post:8, topic:33613"]
I always wear gloves and helmet at a minimum.
[/quote]

yea going to start wearing gloves for sure, have been using a helmet.

[quote="RootedSuperuser, post:10, topic:33613"]
The Vedder can be over built, and in doing so better MOSFET's can be utilised
[/quote]

would the directfet switches that goldenHusky's been building qualify?

[quote="darkkevind, post:16, topic:33613, full:true"]
Injury photos or it never happened! Lol
[/quote]

[details=Don't look]
why would you

<img src="/uploads/db1493/original/3X/8/d/8d84449928c6f97d21fc534451fa2d6217ccc9cb.jpg" width="690" height="388">

want to see this

<img src="/uploads/db1493/original/3X/b/e/bee5c140e5ab71afc6492a48725bb70832c39b82.jpg" width="690" height="388">

you sadist

<img src="/uploads/db1493/original/3X/0/a/0ab742764ba398219c211bbac2619fdeda532237.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/8/2/82903a9116d6e38eeea1ba7b81967dfc238cd4fc.jpg" width="690" height="388">
[/details]
```

---
## \#23 Posted by: jmasta Posted at: 2017-09-21T22:51:48.421Z Reads: 256

```
@thisguyhere Sorry to hear about your fall. Wishing you a speedy recovery!

---- 
On the topic of failing anti-spark switches....

It seems as though most of the switches on the market are only using 2 parallel IRF 7730 FETs.  Which really should only be used for 30A continuous, 40A max.  Adding heatsinks helps, but I just don't think it is enough when you're drawing 80A. They are each dissipating about 3.5W per FET, and you want to keep it under 1W generally

I've had a heatsinked dual-FET Vedder/Fechter switch fail twice already, and I usually never pull more than 30A.  Leading up to both switch failures, I also experienced the slow 10 sec power on you mentioned.  I think it is a sign that your switch is about to blow

<img src="/uploads/db1493/original/3X/f/5/f5a85a1991e2813cbd8234239318f4512834b7d5.png" width="690" height="494">
```

---
## \#24 Posted by: psychotiller Posted at: 2017-09-21T23:34:18.288Z Reads: 234

```
We should inspect the switch Joe. Typically, (always as far as I know) the switches fail in the on position which wouldn't have cut power to your board. Voltage sag can cause your bms to reset though which does shut the board down for a split second. 

When you feel a little better lets get together.
```

---
## \#25 Posted by: thisguyhere Posted at: 2017-09-21T23:52:49.890Z Reads: 231

```
yea for sure, i'll come by maybe in a couple weeks, pretty busy this weekend.  i wanted to pickup a couple things anyhow.  i'll let you know.
```

---
## \#26 Posted by: RootedSuperuser Posted at: 2017-09-22T00:40:09.839Z Reads: 240

```
[quote="thisguyhere, post:22, topic:33613"]
going to start wearing gloves for sure, have been using a helmet.
[/quote]

<img src="/uploads/db1493/original/3X/1/2/12075e4422d6f5ef2d081bdffdff7eca6f94da76.jpg" width="392" height="500"> ... Removable hip and knee pads.

Lots of different styles and prices out there.
[https://www.aliexpress.com/item/2016-KOMINE-MOTORPOOL-UBS06-Jeans-Leisure-Motorcycle-men-s-off-road-outdoor-jeans-cycling-pant](https://www.aliexpress.com/item/2016-KOMINE-MOTORPOOL-UBS06-Jeans-Leisure-Motorcycle-men-s-off-road-outdoor-jeans-cycling-pant-Army/32756775973.html?spm=a2g0s.8937460.0.0.1xA2nF)
```

---
## \#27 Posted by: deucesdown Posted at: 2017-09-22T01:14:22.099Z Reads: 229

```
Maybe this too

https://www.amazon.com/Shock-Doctor-Shockskin-Relaxed-Impact/dp/B005C2QQJU/ref=lp_14291681_1_7?s=apparel&ie=UTF8&qid=1506042793&sr=1-7&nodeID=14291681&psd=1

To be serious, after having one nasty fall, helmet and front hand glove minimum. No watch (ouch!), and I'm considering one of those kevlared flannel shirts. Long sleeves anything helps.
```

---
## \#28 Posted by: Sapphirinia Posted at: 2017-09-22T02:36:40.672Z Reads: 219

```
Pics or it didn't happen!
```

---
## \#29 Posted by: jmasta Posted at: 2017-09-22T02:45:42.841Z Reads: 240

```
[quote="psychotiller, post:24, topic:33613, full:true"]
Typically, (always as far as I know) the switches fail in the on position which wouldn't have cut power to your board. **Voltage sag** can cause your bms to reset though which does shut the board down for a split second. 

[/quote]

This is a great point.  Most of the times that my board has cut out under hard acceleration or big hills was due to voltage sag, and the BMS cutting off power for a few seconds. It's a very hard cutoff.  30A to 0A was drastic. I can't imagine a cutoff at 80A
```

---
## \#30 Posted by: thisguyhere Posted at: 2017-09-22T02:50:20.508Z Reads: 242

```
[quote="psychotiller, post:24, topic:33613"]
Voltage sag can cause your bms to reset though which does shut the board down for a split second.
[/quote]

i was thinking about this while walking my dogs, and yes this seems more likely.  a switch wouldn't / shouldn't cut the circuit, right?

per cell voltage was at about 3.25v, max sag i saw at 80amp draw across the pack was 0.5v per cell.  bms lower cutoff is 2.9v, so 3.25-0.5 = 2.75v, below bms cutoff.  so bms must have cutoff before the vesc had a chance to limit current draw, right?

so...there you go.  lesson learned, don't haul ass when pack is below 40%.

one benefit of getting fucked up is my girlfriend is surprisingly pleasant and isn't being too judgmental about me getting drunk.

[quote="Sapphirinia, post:28, topic:33613, full:true"]
Pics or it didn't happen!
[/quote]

c'mon!  it's like five posts above.

https://www.electric-skateboard.builders/t/ate-shit-today-and-loop-keys/33613/22
```

---
## \#31 Posted by: psychotiller Posted at: 2017-09-22T02:58:16.423Z Reads: 216

```
You're a lucky guy! My Lady Friend hates my guts lol
```

---
## \#32 Posted by: thisguyhere Posted at: 2017-09-22T02:58:50.475Z Reads: 209

```
u mean your wife?  or the one of many side hoes?

edit - this is incredibly misogynistic, pardon me it's meant for comedic effect.
```

---
## \#33 Posted by: psychotiller Posted at: 2017-09-22T03:12:26.263Z Reads: 207

```
wasnt too far south..heehee<img src="/uploads/db1493/original/3X/9/9/99588bb8dcaa5d136e756577b846f143cb01cecb.jpg" width="320" height="240">
```

---
## \#34 Posted by: thisguyhere Posted at: 2017-09-22T03:17:16.794Z Reads: 202

```
fkn awesome...
```

---
## \#35 Posted by: RootedSuperuser Posted at: 2017-09-22T03:21:08.881Z Reads: 201

```
The well dressed rider.....
<img src="/uploads/db1493/original/3X/6/4/6426dc750153950619cfd9278ede318c17094a29.gif" width="159" height="370">
```

---
## \#36 Posted by: mccloed Posted at: 2017-09-22T03:32:52.299Z Reads: 198

```
Why are you cringing? :confused:
```

---
## \#37 Posted by: psychotiller Posted at: 2017-09-22T03:41:32.248Z Reads: 196

```
One them was squeezing my dangly bits
```

---
## \#38 Posted by: mccloed Posted at: 2017-09-22T03:42:48.584Z Reads: 199

```
That's uncalled for.
```

---
## \#39 Posted by: psychotiller Posted at: 2017-09-22T03:43:44.253Z Reads: 198

```
...I still liked it hahaha
```

---
## \#40 Posted by: thisguyhere Posted at: 2017-09-22T05:41:56.119Z Reads: 198

```
[quote="psychotiller, post:39, topic:33613, full:true"]
...I still liked it hahaha
[/quote]

u whoore

https://youtu.be/q-R5V5AKvDM
```

---
## \#41 Posted by: darkkevind Posted at: 2017-09-22T07:50:45.373Z Reads: 192

```
Oooh, ouch! *sucks air in thru pouted lips*
That's gonna smart! :confused:
```

---
## \#42 Posted by: Sapphirinia Posted at: 2017-09-22T12:11:37.235Z Reads: 187

```
It links me to this post and I still can't see... Maybe it's because I'm on mobile. By the way, I use the armored Hoodie from revzilla. It looks like a regular zip up Hoodie but I haven't been able to test it because my board hasn't worked really since I bought it. The one time I used @akhlut motor and stuff. I was wearing no protection lol. It was the naked bike ride.
```

---
## \#43 Posted by: mmaner Posted at: 2017-09-22T12:55:43.197Z Reads: 176

```
That's brave :)
```

---
## \#44 Posted by: Mobutusan Posted at: 2017-09-23T18:23:48.652Z Reads: 167

```
Click on "Don't look"
```

---
## \#45 Posted by: Sapphirinia Posted at: 2017-09-25T01:37:05.067Z Reads: 162

```
Thanks, I finally saw it. Ouch. Hope he heals up quick.
```

---
## \#46 Posted by: lowGuido Posted at: 2017-09-25T06:43:27.772Z Reads: 153

```
[quote="thisguyhere, post:1, topic:33613"]
that and i'm going back to loop keys until i can get a hold of some bullet proof anti-spark switches.
[/quote]

smartest move ever.
```

---
## \#47 Posted by: deucesdown Posted at: 2017-10-03T16:18:23.186Z Reads: 132

```
I've been thinking about this, as I do when I read about falls and failures. Do you think if you were aware it was possible for the power cut, to have saved yourself?

Also, was it just power cut, as if your remote had dropped out? Or was there some drag/braking?

I know when I'm bracing for max throttle, I can commit my bodyweight (fun) or I can kind of bend my knees in the ready-for-anything stance. If I'm fully committed leaning over the front of the board, the power cut would probably throw me off. In the other stance, I think I can wave my arms around and recover?

I ask because I'm always trying to anticipate how things will fail and how to minimize death/injury/damage.
```

---
## \#48 Posted by: DougM Posted at: 2017-10-05T03:37:04.092Z Reads: 120

```
See, this is where I think really long boards would help - if the front wheel is essentially right under your front foot you don't stand a chance, but if your front wheel is 6 or 8 inches ahead of you and your stance is wide you won't eat it with just a power cut (I know this from experience).  However, if it goes into brake you're cooked.

I have only ridden 2 regular decks that were electric - one of my own and a Boosted, and the Boosted was very well behaved whereas mine was kind of a donkey but because it was so short I felt I wouldn't have a chance if it kicked due to a power drop.  So I shelved that board and stuck with my ultra-long land yachts.

I also think drop decks help, but maybe that's because they force you to move your foot back from the front truck.

So I would suggest if you're going to go fast or accelerate hard you might consider a longer board.
```

---
## \#49 Posted by: thisguyhere Posted at: 2017-10-05T06:19:11.693Z Reads: 122

```
[quote="deucesdown, post:47, topic:33613"]
Do you think if you were aware it was possible for the power cut, to have saved yourself?
[/quote]

i mean, if i knew it was going to happen, yes.  i could have just gone running.  but i'm riding in a very crowded, dense area so one's attention tends to dart from here to there.

[quote="deucesdown, post:47, topic:33613"]
Also, was it just power cut, as if your remote had dropped out?
[/quote]

it was just a power cut out, the remote i've been using has been bullet proof.  at least i think so, can't confirm because remote was fubar from the fall.

[quote="DougM, post:48, topic:33613"]
you might consider a longer board.
[/quote]

it's a 40" deck, landyachtz tomahawk so it's full sized already.

<img src="https://www.muirskate.com/photos/products/453/product_Landyachtz_Tomahawk_Downhill_Freeride_Longboard_Skateboard_Deck_2012.png" />
```

---
## \#50 Posted by: DougM Posted at: 2017-10-05T15:04:30.175Z Reads: 105

```
@thisguyhere "it's a 40" deck, landyachtz tomahawk so it's full sized already"

Or I could be wrong :-)  

I went back and read that you were under hard acceleration at the time of the cutout, but my boards are all pretty underpowered, so that makes sense.
```

---
