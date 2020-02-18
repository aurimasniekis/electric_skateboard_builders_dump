# E-switch on BMS

### Replies: 92 Views: 8992

## \#1 Posted by: SirDiff Posted at: 2016-11-22T17:53:10.875Z Reads: 581

```
Hi guys, as many of you may know, there's a group buy going on right now for some batteries in Europe, which is quite a rare thing. Since the manufacturer lets us take a design, and I noticed that many people are asking for a good battery with a bms in a compact form factory, I was wondering if any of you has a diagram (or can make a quick one) for one like this from @denton 
 <img src="/uploads/db1493/original/3X/6/7/67b170dac19b4d6fa557f49b4809d6950193025a.JPG" width="666" height="500">
I would do this by myself but I know nothing about batteries :smile: 
Thank you very much :)

THIS IS NOW A DISCUSSION ABOUT PUTTING A MOSFET E-SWITCH ON THE BMS
```

---
## \#2 Posted by: denton Posted at: 2016-11-22T17:59:53.635Z Reads: 554

```
Here is the website I picked up my BMS from
[http://www.batterysupports.com/lion-lipo-nbsp-36v-nbsp-10s-c-32_41.html](http://www.batterysupports.com/lion-lipo-nbsp-36v-nbsp-10s-c-32_41.html)
They have this wiring Diagram that I followed for this battery. 
I would recommend one of the BMS that have a built in power switch.

<img src="/uploads/db1493/original/3X/7/e/7e0622aa91f97e8cb73d46234f6a4cf0f1a3a196.jpeg" width="689" height="363">
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-22T18:12:22.276Z Reads: 530

```
Just FYI batterysupports can actually add an e-switch for you on their BMS's
```

---
## \#4 Posted by: SirDiff Posted at: 2016-11-22T18:13:48.571Z Reads: 514

```
Are you sure? @fedestanco has a group buy with e-switchs on the bms
```

---
## \#5 Posted by: Jinra Posted at: 2016-11-22T18:14:27.919Z Reads: 499

```
Yes, but you have to reach out to Lilian directly to have her add the e-switch to the BMS.
```

---
## \#6 Posted by: SirDiff Posted at: 2016-11-22T18:24:57.932Z Reads: 491

```
I don't think the bms in the group buy is from batterysupports, so at the moment that's not a priority, I think. E-switches are cool though, hope it will be possible to have one :wink:
```

---
## \#7 Posted by: denton Posted at: 2016-11-22T18:24:59.096Z Reads: 475

```
DANGIT! 
If I would have known that I would have had it done.... Well.... You live and learn I guess. 
That would have saved me a lot of trouble.
```

---
## \#8 Posted by: fedestanco Posted at: 2016-11-22T19:21:55.210Z Reads: 470

```
The bms itself is an e-switch: it can turn off the battery for several reasons: voltage errors/ amp errors/ temperature threshold....
When it comes to add a physical button the options are 2:
1) there is a spot on the bms board designated to add one on-off switch (like the bms on my thread)

2)You make the bms think something is going wrong: for example you can 
short the temperature switch/ fake a failure in one of the balancing wires/....

All the options mentioned work in the same way since the reaction in the board is simply the activation of the mosfets.
```

---
## \#9 Posted by: SirDiff Posted at: 2016-11-22T19:27:43.851Z Reads: 449

```
So you're the one who adds the switch in your GB?
```

---
## \#10 Posted by: fedestanco Posted at: 2016-11-22T19:38:44.086Z Reads: 456

```
Yes, I asked the manufacturer to leave the soldering spots (for the switch) free, so that I can solder an on off switch with a better design (the original was red and rectangular).
```

---
## \#11 Posted by: denton Posted at: 2016-11-22T20:37:03.649Z Reads: 451

```
Is there a place where I can actually do that on the board I already have?

<img src="/uploads/db1493/original/3X/7/f/7f8c074f125c1e1893cd84e26721bf64a526aa99.png" width="535" height="399">
```

---
## \#12 Posted by: longhairedboy Posted at: 2016-11-22T20:42:24.200Z Reads: 443

```
woah, really? I traied earlier this year and she just kept sending me to a different product. 

Can i get my usual 12S 60Amp favorite with an integrated eswitch? 

oh Lillian....
```

---
## \#13 Posted by: fedestanco Posted at: 2016-11-22T20:54:50.070Z Reads: 442

```
<img src="/uploads/db1493/original/3X/7/d/7d8f12842442809eb35f5400806948fc0fc9257c.png" width="301" height="500"> 
the 2 spots in the circle should be designated for e-switch/temperature switch. If you could provide me with hi-res pictures I could confirm what I am saying.
```

---
## \#14 Posted by: denton Posted at: 2016-11-22T20:58:54.597Z Reads: 416

```
I will later, thank you!
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-11-22T21:00:32.676Z Reads: 423

```
WHAT IS THIS UNDOCUMENTED MADNESS. 

So If I short that the BMS will power down?
```

---
## \#16 Posted by: Jinra Posted at: 2016-11-22T21:12:29.851Z Reads: 428

```
So Lilian told me you connect the switch like this,

<img src="/uploads/db1493/original/3X/3/e/3e5bead081c422bef71b7fb14682ec7fa783755a.jpg" width="690" height="368">

However, she said the BMS would have to be modified first before you can do this.
```

---
## \#17 Posted by: Jinra Posted at: 2016-11-22T21:17:44.520Z Reads: 424

```
Here's some of the email thread

<img src="/uploads/db1493/original/3X/e/6/e6050e23e3147e5f59b2e214aa83aea6bdd7ce4e.jpg" width="690" height="445">
```

---
## \#18 Posted by: fedestanco Posted at: 2016-11-22T21:19:24.812Z Reads: 423

```
I will try to explain: 
When it comes to print a circut, although the bms company has several models of the same bms (the standard, the fancy one with an e-switch....), they manufacture just 1 type of printed board; all the fancy add ons will be added later.

These 2 spots (see pic) could have served 2 functions:
1)temperature switch
2) e switch
ACCORDING TO THE ONE (function) THEY PICKED, YOU HAVE TO OPERATE IN 2 DIFFERENT WAYS TO ADD YOUR E SWITCH

1)spots designated for **temperature switch**: 
IN THE NORMAL CONDITION, current DOES flow through the temperature switch. 
TO GET THE BMS IN "ALARM MODE" (to turn off the battery) you will need to OPEN THE CIRCUIT: remove the resistance next to the spots (see pic). <img src="/uploads/db1493/original/3X/f/d/fde474191ffe2f07b66e074895d0ac27491a7b0b.jpg" width="690" height="443">

2)If the spots are meant to be for an e-switch, it couldn't be easier: just short them to turn off the battery.

I hope this will help you build better packs.
```

---
## \#19 Posted by: JuniorPotato93 Posted at: 2016-11-22T21:48:33.140Z Reads: 408

```
Could this be tested with a BMS that is not 100% functional. Because someone should with extra BMS's from prior builds or with a  burnt out component should give this a try and let us know because this is a game changer.
```

---
## \#20 Posted by: Eboostin Posted at: 2016-11-23T02:47:20.074Z Reads: 399

```
When this change is made, does the BMS switch have to be on to charge the battery?
```

---
## \#21 Posted by: JuniorPotato93 Posted at: 2016-11-23T02:49:35.754Z Reads: 368

```
I'm gonna say yes as that disables the balancing functionality of the BMS
```

---
## \#22 Posted by: Eboostin Posted at: 2016-11-23T02:51:29.546Z Reads: 379

```
Bummer, that's the reason why I didn't do e-switch since I don't want the rest of the components on during charging.
```

---
## \#23 Posted by: SirDiff Posted at: 2016-11-25T20:23:03.999Z Reads: 371

```
So does any of you have a diagram like this? :slight_smile:
```

---
## \#24 Posted by: ajaynagra Posted at: 2016-11-25T20:28:36.552Z Reads: 379

```
I can use a picture dont worry
```

---
## \#25 Posted by: denton Posted at: 2016-11-30T00:26:55.244Z Reads: 378

```
Was this where you said the wires need to go for the switch install on the BMS?
<img src="/uploads/db1493/original/3X/9/6/96c8690a13e4ad338093ceef1378ad50cfce4514.jpg" width="666" height="500">

Im working on trying to replace my Mosfets on my electric switch and digging this out has me like,..... um... no!
<img src="/uploads/db1493/original/3X/4/0/4063c6059939ec0acf3d6efc719f7eb928a7b6d4.JPG" width="666" height="500">
```

---
## \#26 Posted by: PXSS Posted at: 2017-01-31T01:49:48.053Z Reads: 350

```
Subbed. (I've been trying to find this thread for a few weeks now)

@Jinra, did you ever get the "modified" BMS?
I just got mine in the mail and will play with switching it, but I didn't know I had to request a modified BMS... Maybe I can populate the proper parts of the board
```

---
## \#27 Posted by: SirDiff Posted at: 2017-01-31T13:43:46.836Z Reads: 340

```
Updated the title, I would turn this post into a discussion about the eswitch, but I cannot edit the post anymore
```

---
## \#28 Posted by: lox897 Posted at: 2017-02-06T02:57:05.676Z Reads: 328

```
Please tell me the exact title you would like and I will change it for you. @SirDiff
```

---
## \#29 Posted by: lowGuido Posted at: 2017-02-07T19:32:03.842Z Reads: 317

```
Its funny because I have been sitting here this whole time thinking "why do all these people with BMS add an extra MOSFET switch when they already have one?"
and then I see this thread.
```

---
## \#30 Posted by: SirDiff Posted at: 2017-02-07T20:06:55.969Z Reads: 323

```
I think "E-switch on BMS" could be clear enough. Maybe also make the original post little and add at the end a bigger "THIS IS NOW A DISCUSSION ABOUT PUTTING A MOSFET E-SWITCH ON THE BMS"
```

---
## \#31 Posted by: jrpwit Posted at: 2017-03-24T02:36:41.682Z Reads: 323

```
So will adding a switch to these two pads create an e-switch?
<img src="/uploads/db1493/original/3X/f/e/fe0526f6aabd67ad97cd63d653b2eb1f6058e837.jpg" width="666" height="500">
 I just want some confirmation because my battery support bms is not modified but @fedestanco said these pads could be used as a switch.
```

---
## \#32 Posted by: smurf Posted at: 2017-03-24T07:43:59.954Z Reads: 313

```
I just got this same BMS.
When I first saw the 2 holes. 
That was the first thing I thought of.
Is that where the switch connects to?
It looks like a few things are missing and that's not how the external switch would work. It would be jumped permanently.
I'm still just guessing but those 2 holes look like the spot for a led lamp and the empty pads are for it's resistor . I hope I'm wrong but that smd stuff is so small it's hard for me to follow. If I had the diagram I could figure it out or maybe it's the temperature alarm but You should be able to cut/switch any balance wire and it should do a protection power off. But who knows what that would do you might have to unplug the whole thing to get it to reset.
```

---
## \#33 Posted by: lowGuido Posted at: 2017-03-24T08:38:57.802Z Reads: 289

```
I don't think it is as simple as just adding a switch to an empty hole.
you need to find the FET's that are responsible for the low voltage cutoff (which I'm going to assume is most of them) and then turn off the gate. or gates as the case may be.
basically you need to have a switch (and possibly some related circuitry) that will simulate a low voltage situation and turn the output off.
make sense?
```

---
## \#34 Posted by: smurf Posted at: 2017-03-24T08:46:35.334Z Reads: 282

```
On second look 
Mine is missing 2 transistors and 2 resistors.

If you cut the power to pin 4 it's going to stop working.
```

---
## \#35 Posted by: TarzanHBK Posted at: 2017-03-24T09:24:13.087Z Reads: 303

```
Is there a better/safer way to use a vedder switch over a BMS switch?
Should be the same thing in simply shutting down mosfets right?
Also does a BMS switch provide the same current rush-in protection? Should be to, due to the mosfets?

I´m getting a BMS with switch and would like to add a nice LED switch. So all you have to do is close the circuit with the two wires - so should be done somehow with a switch.

-_out of my brain directly to the paper - by TarzanHBK_
:monkey:
```

---
## \#36 Posted by: fedestanco Posted at: 2017-03-24T13:05:35.624Z Reads: 298

```
Could you get a better picture please, so I can see components and traces?
```

---
## \#37 Posted by: makevoid Posted at: 2017-03-25T20:20:05.845Z Reads: 300

```
this should be one w/o modifications 

I got two from [NL](http://www.ebay.co.uk/itm/152385098820?_trksid=p2060353.m1438.l2649&ssPageName=STRK%3AMEBIDX%3AIT) - they should be the [supower ones](http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html)
I'm using other two in my [two builds](http://bit.ly/mkv3) but they're currently in the enclosures and shrinkwrapped 


<img src="/uploads/db1493/original/3X/4/9/4990229ab658d60f4623f2b8a67a7e57cd63172c.jpg" width="690" height="323">


<img src="/uploads/db1493/original/3X/3/0/30d4b43a047b526e9c542fae569ed9dfd6e396fb.jpg" width="689" height="335">
```

---
## \#38 Posted by: fedestanco Posted at: 2017-03-25T20:37:24.023Z Reads: 294

```
Still not able to see the traces. It would be great if you could put a flashlight behind the circuit, while taking the picture from the front. Like this:<img src="/uploads/db1493/original/3X/5/c/5ce8f28a25ed18a335d0c702786c01e861c3b558.jpg" width="281" height="500">

And please focus on these zones: <img src="/uploads/db1493/original/3X/b/c/bc8c15df0b44efbd04556fca277d2586871af586.png" width="301" height="500">
```

---
## \#39 Posted by: smurf Posted at: 2017-03-25T21:54:53.744Z Reads: 286

```
https://www.instagram.com/p/BSE7AgTlwLf/


https://www.instagram.com/p/BSE7TGtFWYB/
```

---
## \#40 Posted by: jrpwit Posted at: 2017-03-26T03:46:33.147Z Reads: 283

```
I actually tested the two holes with a switch an they did nothing. I have no idea what they do :confused:. Sorry @fedestanco I actually have it enclosed into my enclosure rn. I'm to lazy to pull it out...

@lowGuido I think I understand. I will do some testing with it once I get my build done. For now I am using an loop key.

Thanks for the info guys!
```

---
## \#41 Posted by: fedestanco Posted at: 2017-03-26T12:35:16.651Z Reads: 271

```
It is clear from the picture that on your bms one of the 2 holes connects to nothing. To make it work you should add 2 resistors I guess (too complicated).
```

---
## \#42 Posted by: smurf Posted at: 2017-03-26T18:08:19.821Z Reads: 273

```
Those two medium size holes by Q13 and Q15 do they complete the alarm circuit? Or the large hole by the 205 and Q13
```

---
## \#43 Posted by: fedestanco Posted at: 2017-03-26T18:32:52.919Z Reads: 279

```
My wild guess is this: <img src="/uploads/db1493/original/3X/1/b/1badce4872bda6afa35ebc4a6ce7d53dac9bc34f.png" width="597" height="500">

But ,again, it seems risky and complicated.
```

---
## \#44 Posted by: rpn314 Posted at: 2017-03-26T18:34:42.654Z Reads: 270

```
Not so wild IMHO. The ones by Q13 and Q15 looks like large vias, and my guess is you add Q13 (a transistor that looks to be missing here) and 2 resistors above it (from the orientation of this picture) and then the two holes (which look to be actual holes, not vias) to the left of the resistors would be your switch wires

Basically, the switch would control Q13 directly, which would control Q15 and the rest of the circuit. Not sure how, but that's my guess given that configuration.

Does anyone have one with the switch attached? We could pretty easily determine it the layout, and the transistor and resistors needed.
```

---
## \#45 Posted by: smurf Posted at: 2017-03-26T19:09:52.861Z Reads: 261

```
I imagine that actual resistors used are determined by which temperature probe and the desired temperature number.

@raphaelchang  @JTAG
Do you guys know where the switch would go?
```

---
## \#46 Posted by: TarzanHBK Posted at: 2017-04-24T21:56:22.038Z Reads: 247

```
You guys with an E-switch on BMS!
Wired everything up today and gave it a go, measured everything, and all good so far. But. If E-switch is off, I still have 2,5V on the BMS output. Seems like something is wrong. Does some of you have one and could measure output current.
I´m using the same 77A 10S BMS that @ajaynagra and @fedestanco bought in group buys.
```

---
## \#47 Posted by: mmaner Posted at: 2017-04-24T22:10:23.003Z Reads: 239

```
I had the same thing, I think its just when you put a load on it that you get the reading.  Multi-meter counts as a load.  Regardless I didn't like the BMS so I pulled it off and replaced it with a BesTech 10s BMS.
```

---
## \#48 Posted by: SirDiff Posted at: 2017-04-24T22:14:55.373Z Reads: 236

```
Why don't you like it? For its bulkiness or something else?
```

---
## \#49 Posted by: TarzanHBK Posted at: 2017-04-24T22:18:34.562Z Reads: 236

```
Also battery won't charge if the switch is off! I don't wanna have my board on the whole time while loading!
So wtf e-switch! ?
```

---
## \#50 Posted by: mmaner Posted at: 2017-04-24T22:19:13.101Z Reads: 235

```
I don't like that it would bleed voltage for any reason when off and that it was freekin massive 😀
```

---
## \#51 Posted by: Eboostin Posted at: 2017-04-24T22:21:11.568Z Reads: 225

```
Don't all BMS bleed voltage? If you were going to leave for a long time, ideally you'd just disconnect the BMS
```

---
## \#52 Posted by: mmaner Posted at: 2017-04-24T22:27:56.974Z Reads: 237

```
They might but I just didn't understand why this one would supply power under any load even when the switch was off.  As I was gonna have to jump through hoops to house it's size I just decided to do away with it.
```

---
## \#53 Posted by: smurf Posted at: 2017-04-25T00:35:57.195Z Reads: 245

```
My guess is there

https://www.instagram.com/p/BTSdNbUFzqA/
```

---
## \#54 Posted by: fedestanco Posted at: 2017-04-25T00:46:30.307Z Reads: 234

```
I tested 4 different bmss from china. They all bled voltage, but when I used a 5amp fuse to test current, voltage dropped and the fuse remained intact.
Yes @TarzanHBK ,bms-on while charging sucks very much. For this and a lot of other reasons I would love to see some badass bmss (like jtag's) get funds to reach the market...
@smurf If I had that board on my bench, I probably would have tried shorting 90% of the f**ing holes to get the holy switch function 😄.
```

---
## \#55 Posted by: TarzanHBK Posted at: 2017-04-25T05:00:19.189Z Reads: 226

```
Hmm that sucks... I think I'll add a second switch to disconnect the vescs, so they won't fry over time due to constant low current
```

---
## \#56 Posted by: Eboostin Posted at: 2017-05-10T02:30:49.635Z Reads: 220

```
Has anyone figured out the definitive way to add an e-switch to the supower (battery supports) BMS? I am going to use the e-switch and unplug the vescs while charging. Not going to have room for a separate anti-spark switch and would prefer something more elegant than the XT-90S
```

---
## \#57 Posted by: Eboosted Posted at: 2017-05-10T02:58:12.191Z Reads: 224

```
IMO this mod it's not worth it at all, If you guys find the way to add the e-switch you will requiere to power on your battery while it takes a charge, if you are willing to do that and leave your board turned on all night (if you forget to turn it off) or stay standed up besides the board until it reaches 100% SoC,  then yeah go ahead and add the e-swtich, otherwise just get an antispark switch and forget about it.
```

---
## \#58 Posted by: Jinra Posted at: 2017-05-10T02:59:34.994Z Reads: 221

```
I really wonder where Enertion got their Space cell BMS, it's literally like 3x7cm and has a built in e-switch that doesnt require the board to be on to charge.
```

---
## \#59 Posted by: Eboosted Posted at: 2017-05-10T03:11:02.300Z Reads: 220

```
There are many things Enertion or Evolve won't ever tell us, but if you know the right people you could get your hands on whatever electronic device you could think of.

Nevertheless, we need to look further in China, there must be something for us there
```

---
## \#60 Posted by: Jinra Posted at: 2017-05-10T03:13:33.516Z Reads: 217

```
I've looked at a ton of places, but even the smallest 10s BMS's I find are quite a bit larger than the SCP BMS. The search continues...
```

---
## \#61 Posted by: Eboostin Posted at: 2017-05-10T04:07:27.233Z Reads: 192

```
It has value but sounds like not your setup.

I have a disconnect to the vesc. If I can get the e-switch to work, then I eliminate the need for the anti-spark which takes up more room and is one more potential failure point.
```

---
## \#62 Posted by: Stefan Posted at: 2017-05-10T12:29:46.247Z Reads: 195

```
I have a batterysupports 10s bms with e-switch functionality integrated. Since i am still waiting for parts to arrive i have not really tested it but i can tell that with the e-switch switched off i still get around 9v on the output. That's why i don't trust it and will use an external e-switch.
If you want i can upload some pictures.
```

---
## \#63 Posted by: Eboostin Posted at: 2017-05-10T14:14:31.604Z Reads: 191

```
That would be great, if you don't mind uploading some pics. @Stefan

 Bummer it still puts out 9v...
```

---
## \#64 Posted by: SirDiff Posted at: 2017-05-10T14:16:03.928Z Reads: 192

```
Don't external mosfet switches need constant power as well?
```

---
## \#65 Posted by: TarzanHBK Posted at: 2017-05-10T14:21:42.132Z Reads: 194

```
9V is massive! Mine is outputting about 2,5V.
With 9V I would be afraid to power up my Vescs..
```

---
## \#66 Posted by: Stefan Posted at: 2017-05-10T14:26:32.571Z Reads: 192

```
I have not connected it to a vesc yet. Maybe the voltage will drop once connected to the vesc, but eiterway i don't trust it.
```

---
## \#67 Posted by: TarzanHBK Posted at: 2017-05-10T14:27:49.157Z Reads: 198

```
yah..maybe put a bit of load on it and see if it drops down a bit
```

---
## \#68 Posted by: Stefan Posted at: 2017-05-10T14:28:26.775Z Reads: 216

```
<img src="/uploads/db1493/original/3X/7/c/7c5238fd554ff0de6247184990320bebf6393996.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/7/27675539602d635cec90d5fedf38378dd5eb62ca.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/b/7/b7b9386d35ba913ea9bd165a397ec2851e3bedf1.JPG" width="666" height="500">
```

---
## \#69 Posted by: longhairedboy Posted at: 2017-05-10T14:38:50.079Z Reads: 208

```
 i'll just keep doing this. One switch to cut the power when i want, and one behind that to cut it in an overload or undervoltage situation. If the vedder switch fails into the on position like they do sometimes on rare occasion, then the BMS will cut power when the voltage runs too low from draining too much. 

https://www.instagram.com/p/BTh_40Mlakh/?taken-by=longhairedboy
```

---
## \#70 Posted by: Eboostin Posted at: 2017-05-10T14:44:26.174Z Reads: 206

```
Thank you! Could you take one more pic close up so i can read the numbers?
```

---
## \#71 Posted by: Eboostin Posted at: 2017-05-10T14:45:15.320Z Reads: 211

```
I asked Lilian at Supower how to add a switch. She said this is all that has to be done. I have not tried it yet.

I think the picture, the wiring she provided is telling the BMS that there is something wrong with the 10th pack so the BMS shutoff charging/discharging. 

In the wiring example that @Stefan provided, I believe that is where they would put a thermistor, telling the BMS that the pack is too hot.  

<img src="/uploads/db1493/original/3X/f/b/fb419327375a0a3579286c4099b9e5d5e85909e7.jpg" width="690" height="471">
```

---
## \#72 Posted by: Stefan Posted at: 2017-05-10T14:53:32.791Z Reads: 205

```
Which numbers do you mean?

In your picture the switch is connected at a different spot than mine. I bought mine through ebay and left a message to enable the e-switch functionality and they mounted the switch leads at a different spot..
```

---
## \#73 Posted by: Eboostin Posted at: 2017-05-10T15:09:52.954Z Reads: 203

```
I need the numbers off the resistors. I'm going to try both spots and see which works better

<img src="/uploads/db1493/original/3X/c/f/cf9ac82a9dcefde6b2f1b4673a57a4b32b79d79d.JPG" width="375" height="500">
```

---
## \#74 Posted by: Stefan Posted at: 2017-05-10T15:19:02.920Z Reads: 191

```
Did you try to zoom in the picture? I can read them very well (the two resistors you marked in your picture). They are 102 and 205.
```

---
## \#75 Posted by: Eboostin Posted at: 2017-05-10T15:24:17.932Z Reads: 191

```
Thank you! I had originally looked on my mobile and it wasn't working. Tried on my computer and can read them clearly.
```

---
## \#76 Posted by: Eboostin Posted at: 2017-05-12T16:21:59.286Z Reads: 189

```
I was thinking about this and could you set the vesc minimum input voltage to 10v instead of 8v? Then the VESC would be off and it wouldn't matter if it was putting out 9v. Also, I was reading on some of the ebike forums that even though some BMS put out a voltage when off, they don't put out any current and when a load is connected, it drops to 0v.
```

---
## \#77 Posted by: TarzanHBK Posted at: 2017-05-12T17:17:52.451Z Reads: 197

```
I just tested this and it´s right. With only the BMS attached I get 3,4V when off.
I hooked up the rest of the system, so assembled everything and messured again and it´s only 0,11V now.
```

---
## \#78 Posted by: longhairedboy Posted at: 2017-05-12T17:24:50.874Z Reads: 198

```
electricity is so weird.
```

---
## \#79 Posted by: TarzanHBK Posted at: 2017-05-12T17:29:46.129Z Reads: 192

```
It´s like water, you have to flow with it
-Bruce Lee :monkey:
```

---
## \#80 Posted by: longhairedboy Posted at: 2017-05-12T17:35:57.205Z Reads: 194

```
or in this case, its more like my oldest son. Sitting there on the couch with a lot of potential but as soon as i put a work load on him the potential collapses.
```

---
## \#81 Posted by: Eboostin Posted at: 2017-05-12T21:42:56.205Z Reads: 181

```
:joy:

10 characters
```

---
## \#82 Posted by: ACIN Posted at: 2017-05-16T06:26:20.338Z Reads: 187

```
Same problem, just with the 12S BMS.
Has anybody tried the method with the switch on the transistor in the corner with that model?

And can somebody explain to me like I'm five what behavior wiring it like this will result in? Will anything beyond the BMS still be able to draw current when the switch is open? Does the BMS balance cells all the time or only when charging or only when the switch is closed? How does doing this compare to putting a Antispark between the BMS and the Battery or the Vesc respectively?
Sorry normally I wouldn't ask so many fundamental questions and just try it but I want to be extra sure I'm not damaging anything.
```

---
## \#83 Posted by: jrpwit Posted at: 2017-05-16T18:53:19.273Z Reads: 183

```
I want to know too! 😀
```

---
## \#84 Posted by: Bender Posted at: 2017-05-16T22:36:21.402Z Reads: 187

```
Me toos 
Need to know
```

---
## \#85 Posted by: smurf Posted at: 2017-05-17T00:41:43.938Z Reads: 195

```
The finished lithium-ion battery has two main parts including lithium cells and BMS (battery management system).Lithium cell is consists of a positive electrode plate,separator,negative plates,electrolyte.The positive electrode ,the separator and the negative plate would or laminated together ,and then filling electrode batteries made after the packaging.But many people do not know the function of lithium battery protection board (BMS).BMS is to protect overcharge,over discharge and output short-circuit to happen.

Over discharge protection:When the battery is about to run out to a minimum value of the voltage,BMS will shut down the output voltage, and battery can not continue to discharge .Finally product will power off as well.

Overcharge protection:When the product at the time to charge the battery voltage reaches the maximum voltage,the BMS will automatically power off ,showed not continue to charge the full to arrive a protective effect.

Short circuit protection:When the battery is accidentally short circuit ,The BMS will automatically shut down within a few milliseconds ,not power on.Then it will be okay if positive and negative come together.This short circuit protection does not cause an explosion.


Over-current protection:The BMS has a maximum current limiting,and different products are not the same.When the discharge over current protection value,MBS will automatically shut down as well.

Basically the BMS is a alarm system. When a condition gets out of range it sets off the alarm cutting power to the mosfets.
```

---
## \#86 Posted by: ACIN Posted at: 2017-05-23T19:37:00.114Z Reads: 189

```
Well yeah, that was pretty clear but thanks anyway - what we aren't very sure about yet is how you can implement a mechanical switch within a [12S Batterysupports BMS](http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html).

One proposition was that you would solder the switch to the outer transistor in the top left corner of the board.
But even if that works it isn't known what behavior this will result in (what does it even mean if a BMS is turned "off"?)
- see quoted post:
> And can somebody explain to me like I'm five what behavior wiring it like this will result in? Will anything beyond the BMS still be able to draw current when the switch is open? Does the BMS balance cells all the time or only when charging or only when the switch is closed? How does doing this compare to putting a Antispark between the BMS and the Battery or the Vesc respectively?
> Sorry normally I wouldn't ask so many fundamental questions and just try it but I want to be extra sure I'm not damaging anything.
```

---
## \#87 Posted by: Eboosted Posted at: 2017-05-24T15:15:39.087Z Reads: 180

```
If you ever discover the way to make this e-switcg work, you will have to turn the battery/board on in order to charge/balance the battery.

Is it worth it?, not for me at all
```

---
## \#88 Posted by: ACIN Posted at: 2017-05-24T21:03:25.259Z Reads: 184

```
sigh, antispark it is
```

---
## \#89 Posted by: i2oadsweepei2 Posted at: 2018-07-08T19:22:33.008Z Reads: 105

```
I picked up a Supower 60amp 12s lip ion bms last week. I asked them to install the switch. My hopes were up. Maybe for good reason? Please look at the pics there is an extra resistor installed on mine along with the switch. Fingers crossed 🤞 I’m not sure if I will have it together today or not. I like the BMS because of its size.

![image|374x500](upload://edKzOry8mcuE37NWO21ohPgPrhJ.jpeg)

![image|375x500](upload://myawIUCejQnfbesno7399BNuU7s.jpeg)

![image|375x500](upload://jNra1vjMxqvIn9FZ3ZUynzNjiIO.jpeg)

![image|375x500](upload://rB3O7Qc7kaTh4JQ2rt2EKm0wtri.jpeg)
```

---
## \#90 Posted by: i2oadsweepei2 Posted at: 2018-07-08T22:50:30.722Z Reads: 91

```
No joy. It didn’t work.
```

---
## \#91 Posted by: TowerCrisis Posted at: 2018-08-03T12:52:26.438Z Reads: 73

```
That is very peculiar.

The PCB layout on that should have had a small mosfet or transistor, i'm not sure which, where they put the diode to bridge the two runs. Not sure if that's a retrofit or if it's assembled wrong.

I've got the same BMS, I'm hoping to be able to retrofit an e-switch to mine. The BMS DOES have short circuit protection, so it definitely has the ability to switch off... I'll inspect the traces with a flashlight and report back with a possibile solution. I'll likely tack on some wires, likely onto an existing component on the board so I can artificially trigger a short circuit or temp or over voltage protection.
```

---
## \#92 Posted by: i2oadsweepei2 Posted at: 2018-08-03T15:35:47.541Z Reads: 70

```
That would be great news. I have already committed to the anti spark. But that could be used in the event of an emergency.
```

---
