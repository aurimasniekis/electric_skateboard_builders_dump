# Chaka&rsquo;s VESC repair log

### Replies: 77 Views: 7614

## \#1 Posted by: chaka Posted at: 2016-01-29T06:32:43.148Z Reads: 623

```
Now that I am servicing/repairing VESC's I thought I might keep a log of the various failures and solutions. I hope it may become useful for anyone attempting to repair a VESC on their own.

I will do my best to keep this thread updated and document how I bring these beautiful pieces of hardware back to life.
```

---
## \#2 Posted by: chaka Posted at: 2016-01-29T09:48:04.511Z Reads: 595

```
The latest VESC I have repaired was a pretty common short circuit failure caused by an exposed wire.

If you are lucky and only shorted the ppm header/ 3 pin servo connector, then sometimes you can replace the tvs diode and all will be well. More often then not a short will cause the stm chip to fail and possibly the drv8302 mosfet driver. 

This VESC was reported to have been shorted and the led's were not lighting up anymore. The vesc was indeed unresponsive upon arrival. When powered the voltage regulator would heat up signaling a short circuit had developed somewhere.

 I was doubtful that the vreg had failed but to be sure, I used canned air to frost the board and carefully watched the stm processor as I powered the board once again. Sure enough the stm chip quickly thawed the frost signaling it had developed a short and needed to be replaced. Sure, using canned air seems crude but, as I recently found out from other community members, is a very sound way of detecting hot spots and shorts.

After replacing the stm chip with a hot air station the vesc once again came back to life when powered. Of course it being a fresh chip it was in need of firmware and the bootloader. After it was flashed I attempted to run motor detection with the bldc-tool and it failed. I checked the terminal for faults and as I suspected it was the drv8302. 

Another round on the hot air station with a fresh driver and our once dead VESC was back in business! 

<img src="/uploads/db1493/original/2X/e/e32eec67e2b77f0a983f4da1f0c7ccdc55d805d0.jpg" width="690" height="486">
```

---
## \#3 Posted by: trbt555 Posted at: 2016-01-31T08:30:13.476Z Reads: 485

```
Hi @chaka, I'm looking for a tip:
When you remove the MCU or the DRV, there's still little mounds of solder on the pcb pads, which -in my experience- makes it diffcult to keep the replacement chip alingned with te pads. How do you cope with that ?
Thanks.
```

---
## \#4 Posted by: NIK Posted at: 2016-01-31T09:46:20.966Z Reads: 481

```
From my experience with surface mount soldering, you can use SOLDER WICK to absorb residual solder and re-apply new solder afterwards. Solder wick also came in many sizes. Cheers
```

---
## \#5 Posted by: chaka Posted at: 2016-01-31T15:48:11.374Z Reads: 472

```
I actually place the chip while the solder is still in its molten state. I do not recommend this to anyone who hasn't placed at least a few hundred of these chips though. Don't worry I preheat the chip before doing this. ;)

Another method I use is by using "no-clean" flux and letting it dry till it gets tacky. This helps keep the chip in place while I apply hot air. The chip always ends up moving a bit when the solder begins to flow so some final alignment is necessary at that point.

 You do need to be sure to apply enough heat before aligning since you can lift some pads if the solder re-solidifies while in the process.
```

---
## \#6 Posted by: chaka Posted at: 2016-02-09T01:42:20.405Z Reads: 444

```
After having repaired several VESC's from other manufactures we regret to announce we will only be providing a repair service for existing customers on Ollin made VESC's.

We are seeing too many quality control issues and cannot bring them up to our standards without completely rebuilding with quality components on fresh pcb's. We may offer some sort of salvage service in the future to those stuck with bunk VESC's, giving a credit for the few usable components that match Vedder's BOM. It might add up to a $15 to $20 savings.
```

---
## \#8 Posted by: zblad Posted at: 2016-08-31T20:30:07.245Z Reads: 374

```
I have a vesc that flashed no problem but when I hooked up a 12v battery I noticed some smoke... I believe the LEDs or the blue one atleast still comes on.  Would you recommend replacing the small 32bit processor, And do you think anything else is fried?
```

---
## \#9 Posted by: chaka Posted at: 2016-08-31T21:14:38.919Z Reads: 364

```
Check the tvs diode, that is what is probably heating up. If it is you will want to check the stm chip it could have some bridged legs or faulty like you are thinking.
```

---
## \#10 Posted by: zblad Posted at: 2016-09-01T01:32:09.269Z Reads: 357

```
So i put a different stm chip on and I can flash the vesc successfully and have a blue led but I removed the motor driver. but when I hook the battery up I get no lights is this because I removed the motor driver? I have no clue how I'm going to get another one on because it's hard to tell if the pad is soldered underneath.  Is there a diode that could have went bad and that's why I have no power lights when a battery is hooked up? Basically does the motor driver have to be on for the vesc to get power with a battery?
```

---
## \#11 Posted by: chaka Posted at: 2016-09-01T01:34:15.456Z Reads: 353

```
The drv chip has a buck converter that supplies the 5v rail. When the programmer is attatched the 5v is supplied by the usb.

Upload some photos when you get a chance.
```

---
## \#12 Posted by: zblad Posted at: 2016-09-01T01:46:14.836Z Reads: 359

```
<img src="/uploads/db1493/original/2X/e/e071ef4be0d210d4891b5eb0e5eb11e2d933899b.jpeg" width="375" height="500"> 
here is a picture if I replace the drv is there anything else that could be bad
```

---
## \#13 Posted by: chaka Posted at: 2016-09-01T02:12:36.951Z Reads: 344

```
It is hard to be sure but it looks like there is a lot of residual solder paste on the pcb. You may want to give it a good Iso alcohol bath after you replace the drv chip. That could have been the initial cause of the 5v short.

I use a 10x loupe to check the pins. Do you have one you can use?
```

---
## \#14 Posted by: zblad Posted at: 2016-09-01T02:38:24.946Z Reads: 337

```
No not really sure what that is and should I just take like a tooth brush and alcohol and scrub the pins on the stm n drv?
```

---
## \#15 Posted by: chaka Posted at: 2016-09-01T02:48:32.190Z Reads: 334

```
Yeah that would work but I took another look and it looks like the solder paste under the mosfets did not flow properly. You may want to add some liquid flux and use the hot air machine to get those areas to flow. It can be a difficult area due to the extra mass of the mosfets soaking up most of the heat.
```

---
## \#16 Posted by: zblad Posted at: 2016-09-01T11:41:25.565Z Reads: 318

```
How hot do I dare turn my reflow station up I don't want to damage the component or the pcb board
```

---
## \#17 Posted by: zblad Posted at: 2016-09-01T13:04:58.989Z Reads: 301

```
I'm hoping tonight to resolver the drv on I'll take pictures of that and the mosfets before I try power it with a battery... I don't own a power supply but am starting to consider buying one
```

---
## \#18 Posted by: zblad Posted at: 2016-09-01T16:19:12.461Z Reads: 289

```
Probably a dumb question but the mosfets not being soldered by the back would that cause it not to connect to the PC? Also if I bought a power supply would that shut down if there was a short and prevent stuff being fried?
```

---
## \#19 Posted by: chaka Posted at: 2016-09-01T16:52:24.150Z Reads: 295

```
No but it will cause hardware faults. The residual solder paste could cause the issues you were having.
```

---
## \#20 Posted by: zblad Posted at: 2016-09-01T17:05:42.462Z Reads: 312

```
<img src="/uploads/db1493/original/2X/0/02be086ceb6e63518074a8d23fb575169bdc0cb5.jpeg" width="375" height="500">

Resoldered the drv on and this is how it turned out also fixed the mosfets but I don't know if I dare plug it into a battery
```

---
## \#21 Posted by: chaka Posted at: 2016-09-01T17:17:05.958Z Reads: 302

```
You could try using a pair of 9v alkaline batteries in series. I haven't tried it but I don't think they have enough amperage to fry the vesc. I single 9v might work but it is very close the the low voltage threshold and my throw fault codes
```

---
## \#22 Posted by: zblad Posted at: 2016-09-01T17:53:02.889Z Reads: 286

```
I looked for bridges with a magnify glass but didn't see any but that doesn't mean anything I have learned.  So let me get this straight if I had the power supple I would the current to what?  And then if there was a short the power supply would stop supplying power to the vesc. Basically it's a safety fuse
```

---
## \#23 Posted by: zblad Posted at: 2016-09-01T17:56:02.988Z Reads: 283

```
Sorry one more question in bedders directions he loads a boot-loader onto the bed is this necessary? When I flash the firmware always flashes and takes a few seconds but the boot loader only seems to flash if I unplug the vesc and plug it back in.
```

---
## \#24 Posted by: zblad Posted at: 2016-09-01T22:00:56.766Z Reads: 270

```
So I flashed the vesc hooked up a 9v to power and waited five second but never get the red flashed led I do not get this
```

---
## \#25 Posted by: hexakopter Posted at: 2016-09-11T18:10:39.039Z Reads: 269

```
@chaka Do you have experience what components die when the 12s voltage touches the 5v line because of a lead fracture? I think the 5v to 3.3v LDO is destroyed, but I hope the STM is save, because it sits "behind" this LDO. I am also not 100% sure if that have killed my drv8302.
Maybe also others here have experience what dies in that special case.
Would be cool to know, before I investigate a lot of time in fixing.
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2016-09-11T18:22:59.367Z Reads: 292

```
The 5v is provide by the DRV, so it is most likely to be burn, also you might want to check the can traceiver (it is also highly sensible)
```

---
## \#27 Posted by: ralphy Posted at: 2016-11-27T03:06:23.566Z Reads: 254

```
Are you in the US? Mine toasted and i need to know what the heck happenend. Have you seen this failure ?<img src="/uploads/db1493/original/3X/a/4/a4548394f560ef47a343c79dc7b054625f6ed106.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/7/f/7f1c767510ccd96292c2752c285dabcdd180081f.jpg" width="375" height="500">
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2016-11-27T03:37:20.649Z Reads: 240

```
@ralphy wow it is missing half the capacitor.... this is what cause your problem... It had create a overvoltage on the remaining capacitor, wich can easily blow them, like what happen to c40
```

---
## \#30 Posted by: Quinlanbrown Posted at: 2016-11-27T15:14:51.486Z Reads: 241

```
I wired my vesc backwards so when I plugged it in it was a atomatic short now no lights or anything show up want do I need to replace to fix it and could you give me a link to those parts?
```

---
## \#31 Posted by: chaka Posted at: 2016-11-27T15:44:21.276Z Reads: 248

```
You likely burned some traces and the drv chip with reverse polarity.
```

---
## \#32 Posted by: rtasca Posted at: 2016-11-27T18:51:09.550Z Reads: 241

```
WIll anyone be willing to sell a DRV chip in Europe? I have a friend coming from Portugal in Dec.
```

---
## \#33 Posted by: Glenn Posted at: 2016-12-02T10:46:11.937Z Reads: 240

```
Hey Chaka I have a vesc that failed and would like repaired but was wondering what I'm looking at as far as price goes. It's from enertion.
```

---
## \#34 Posted by: mason Posted at: 2016-12-02T12:41:41.635Z Reads: 235

```
He doesn't repair other companies vescs
```

---
## \#35 Posted by: noob Posted at: 2016-12-03T03:12:30.851Z Reads: 237

```
Hey could you fix my vesc, i dont know what is wrong with it.

I configured all the settings in the Bldc tool and had the vest running in foc

everthing was working great and i could control the motor with my ppm controller

them next time i tried the throttle (board was on its back entire time) the red light flashed three times

the i began to carry it to the other room and hit the throttle one more time by accident and the vesc sparked and smoke came out
after further inspect i thing dmv chip is fried
wont power on and no lights or anything but caps arent damaged
```

---
## \#36 Posted by: willpark16 Posted at: 2016-12-03T06:07:09.864Z Reads: 232

```
Fox has hurt many a vesc not recommended for 4.12
```

---
## \#37 Posted by: rpn314 Posted at: 2016-12-03T16:14:33.398Z Reads: 235

```
If it's not powering on anymore and you're not seeing any lights I think that's more than a DRV issue. My experience is DRV blown just means the motors won't roll and you'll see flashing red lights, but the microcontroller should still be working fine (ie power on and lights are working). No lights would indicate something else fried as well.
```

---
## \#38 Posted by: noob Posted at: 2016-12-03T20:46:15.843Z Reads: 229

```
oh, thank you for the info
```

---
## \#39 Posted by: noob Posted at: 2016-12-03T20:48:08.129Z Reads: 223

```
so is it not possible to run foc on 4.12?
also what hardware versions are recommended and where can i find more info about it
```

---
## \#40 Posted by: willpark16 Posted at: 2016-12-03T23:34:26.353Z Reads: 224

```
Kind of a hit or miss
```

---
## \#41 Posted by: rpn314 Posted at: 2016-12-04T00:27:31.988Z Reads: 230

```
VESC 4.12 is the newest as of right now (6 is in late development, arrival probably by early-mind 2017). So basically, you're in the best position to run it, as it is definitely possible on 4.12, but FOC can be very finicky. It's extremely easy to not set it up right, and unless it is set up perfectly, you can very easily fry something (the DRV chip most of the time). I'm still using BLDC for that reason.
```

---
## \#42 Posted by: noob Posted at: 2016-12-04T09:18:24.716Z Reads: 225

```
thanks for the help :) might come back here soon with more questions
```

---
## \#43 Posted by: chaka Posted at: 2016-12-05T15:53:42.990Z Reads: 217

```
FOC works well with auto detection on large sk3 motors but not much else. FOC also knocks your top speed down a little.  Personally, I really like the sound of dual motors in bldc mode. You get a really nice chorus effect during acceleration.

If you have a blown DRV from FOC use then one of the DRV legs will likely be fused to the pcb and you will need surgical like precision to remove it without pulling the pcb trace off the board when you remove the chip.

I am really sorry for not offering repair services on VESC's from other vendors but they always seem to fail again after little use due to many variables.

Sorry for the lack of presence on the forums lately everyone. We are logging nearly 16 hours a day in the shop right now finishing[ FreeRide](http://www.ollinboardcompany.com/product/dual-esc-integrated-power-system-longboard-deck) pre-orders. Doesn't leave much time for anything else. :laughing:
```

---
## \#45 Posted by: jrlowe24 Posted at: 2017-01-07T03:19:05.881Z Reads: 181

```
When using my VESC, after riding it for a good 40 miles, I took out my board to ride it and didnt mount down the motor wires so they grinded on the motor and shorted the VESC blowing the DRV chip. I removed the DRV chip, and it seems to be the only thing that got blown since when i plug it in, I still get lights. Is there a way I can send you my VESC for a repair?
```

---
## \#46 Posted by: willpark16 Posted at: 2017-01-07T03:21:22.342Z Reads: 175

```
what kind is it
```

---
## \#47 Posted by: chaka Posted at: 2017-01-07T04:00:53.393Z Reads: 168

```
Sorry James, we only provide warranty/repair service on hardware we build. 

You might find someone willing to tackle this around the forums.
```

---
## \#48 Posted by: jrlowe24 Posted at: 2017-01-07T04:03:13.485Z Reads: 168

```
It is from DIYElcetricSkateboard
```

---
## \#49 Posted by: willpark16 Posted at: 2017-01-07T04:09:50.890Z Reads: 170

```
Hate to speak for him but he won't repair one of those also I don't recommend diyepectric boards if u want my honest opinion
```

---
## \#50 Posted by: willpark16 Posted at: 2017-01-07T04:10:29.119Z Reads: 165

```
If u need one buy and axle
```

---
## \#51 Posted by: jrlowe24 Posted at: 2017-01-07T04:12:08.999Z Reads: 160

```
The VESC is essentially the exact same as the pictures Ive seen throughout this thread though
```

---
## \#52 Posted by: willpark16 Posted at: 2017-01-07T04:13:09.960Z Reads: 160

```

Yes but he doesn't stand behind his products he just sells them and if they stop working he kinda leaves u out to dry

Edit also a warranty for a vesc is very important along with a vendor who will provide support
```

---
## \#54 Posted by: jrlowe24 Posted at: 2017-01-07T04:18:04.672Z Reads: 163

```
is there anyone on the forum that would fix it for money?
```

---
## \#55 Posted by: mmaner Posted at: 2017-01-07T04:18:05.383Z Reads: 164

```
Dexter offers a warranty as well, it's just extra. About the same cost as Ollins if you buy the warranty.  Personally Dexter has always been very helpful to me and stood behind his products.
```

---
## \#56 Posted by: mmaner Posted at: 2017-01-07T04:18:41.643Z Reads: 161

```
Message @JohnnyMeduse, he does VESC repair.
```

---
## \#57 Posted by: chaka Posted at: 2017-01-07T04:23:58.634Z Reads: 164

```
> Yes but he doesn't stand behind his products he just sells them and if they stop working he kinda leaves u out to dry

You have no reason to start bagging on Dexter. This VESC was working and failed due to rider error. Keep the threads clean and give Dexter a little more respect.
```

---
## \#58 Posted by: willpark16 Posted at: 2017-01-07T05:07:13.242Z Reads: 168

```
i offered an opinion take it how you want too but at the end of the day its an opinion
```

---
## \#59 Posted by: JohnnyMeduse Posted at: 2017-01-07T05:17:27.033Z Reads: 170

```
Yep... @jrlowe24 message me... I can probably do it.

Thank @mmaner 😊
```

---
## \#60 Posted by: willpark16 Posted at: 2017-01-07T07:35:36.600Z Reads: 174

```
since many community members think it inappropriate for me to tell you my opinion I will let you know that I also had some products from him work fine and my own opinion in this sense doesn't affect the reason your vesc stopped working. So in regards to ur vesc send it off to @JohnnyMeduse but shipping may be a killer for you depending on where you are. I do highly reccomend axle for a vesc at an affordable price with a good warranty and good service. @zmoney . also you can contact dexer @torqueboards and maybe he can work out a repair for 60 bucks or something. Best of luck!
```

---
## \#61 Posted by: slugit Posted at: 2017-03-23T00:52:32.633Z Reads: 157

```
Hi there... 1st post, so ill do my best...
Im retrofitting a chinese mountainboard as one of the controllers failed...
I have 2 vedder 4.12 vesc, intending to connect via cannbus...
Now for the problem..!
I had them wired for power, but not interconnected, had them (loosely, yes i know, stupid) assembled in the case in a sort of square, L to reverse L format,caps at 90deg...
Connected the power, all good....
Then i went to plug in the usb...
There was a tiny little spark as one of the capacitor legs touched one of the last 2 pins of the 'P1' connector either pin 'MP' or '5v' (cant quite read all the letters/positioning..)
The LED went out, no comms over USB...
Can anyone tell me what ive probably killed, and what i need to replace..?
Many Thanks,

Jay
```

---
## \#62 Posted by: GhettoFab.rictation Posted at: 2017-11-11T23:35:34.104Z Reads: 118

```
@chaka <img src="/uploads/db1493/original/3X/7/8/78aaf568bfcd3c2d58957778e9c8b154934b4bb4.jpg" width="666" height="500">
```

---
## \#63 Posted by: GhettoFab.rictation Posted at: 2017-11-11T23:36:13.180Z Reads: 120

```
Possible repair on ollin vesc? There's a bunch going on here
```

---
## \#64 Posted by: GhettoFab.rictation Posted at: 2017-12-24T01:27:09.835Z Reads: 106

```
@chaka how do I go about your servicces and how much are they? no lights come on during power up and mosfets looks like goners
```

---
## \#65 Posted by: GhettoFab.rictation Posted at: 2017-12-24T01:33:15.508Z Reads: 102

```
[quote="willpark16, post:52, topic:1151, full:true"]
Yes but he doesn't stand behind his products he just sells them and if they stop working he kinda leaves u out to dry

Edit also a warranty for a vesc is very important along with a vendor who will provide support
[/quote]

interesting though because I haven't had a response from @chaka quite yet about the warranty or Prices for repairing one of his vesc..
```

---
## \#66 Posted by: willpark16 Posted at: 2017-12-24T01:38:22.519Z Reads: 104

```
2 year warranty when you buy from him and the repair price is apart of that warrant you can read a bit more on the forum and have had that question answered
```

---
## \#67 Posted by: willpark16 Posted at: 2017-12-24T01:39:13.777Z Reads: 102

```
He repairs his vesc but he Does not repair those from other manufacturers
```

---
## \#68 Posted by: GhettoFab.rictation Posted at: 2017-12-24T01:40:38.727Z Reads: 104

```
so you're talking about backing a product then say I need to figure out his prices hah.. Anyway I know 2 year warranty, but mine won't be all the way covered and need him to quote me based off of what happened to it.
```

---
## \#69 Posted by: GhettoFab.rictation Posted at: 2017-12-24T01:41:03.746Z Reads: 101

```
right ollin's right?
```

---
## \#70 Posted by: GhettoFab.rictation Posted at: 2017-12-24T01:42:10.783Z Reads: 105

```
look at the date of the my picture's post.. that's a long time for no response...
```

---
## \#71 Posted by: willpark16 Posted at: 2017-12-24T01:48:08.212Z Reads: 106

```
Well have u tried his website? There is a unique button labeled "contact" try it out
```

---
## \#72 Posted by: GhettoFab.rictation Posted at: 2017-12-24T02:17:21.231Z Reads: 105

```
hey you know instead of talking to him about it on here I'll talk to him on there that's an amazing idea.. I'm already in the process of finding someone else to repair, unless overseas shipping and repair cost all together are somehow less than someone in my country repairing it.. Anyway just wanted to make a statement as far as communication on here. If you are going to make money off of a community and be held as a leader of a community then it's crappy to forget someone or leave them hanging for more than a month (which chaka has made amazing support happen here as I've seen before, idk what happened to me though :cry:). I just wanted a response jesus even a rude response is better than none when I posted OVER a month ago.... But hey what do I know.. Just a guy trying to get his stuff working right. I appreciate chaka and his support, but damn a month sucks as hard as a hooker on dollar night..
```

---
## \#73 Posted by: willpark16 Posted at: 2017-12-24T02:45:13.672Z Reads: 102

```
He isn't on here much
```

---
## \#74 Posted by: GhettoFab.rictation Posted at: 2017-12-24T04:22:13.799Z Reads: 100

```
Shit. Well I will just have to go with plan a.
```

---
## \#75 Posted by: GrecoMan Posted at: 2017-12-24T22:12:47.630Z Reads: 90

```
he is no longer on this forum at all.
```

---
## \#76 Posted by: GhettoFab.rictation Posted at: 2017-12-24T22:40:04.081Z Reads: 89

```
what?! must be doing good if that's the  case. That explains that though.
```

---
## \#77 Posted by: GrecoMan Posted at: 2017-12-24T23:11:24.780Z Reads: 93

```
said he’ll no longer be posting or checking this forum due to contractual reasons
```

---
## \#78 Posted by: GhettoFab.rictation Posted at: 2017-12-24T23:21:03.053Z Reads: 93

```
hm I wouldn't have done that if I was him. That's money left on the table imo. That sucks though
```

---
## \#79 Posted by: seanray007 Posted at: 2018-04-25T02:33:58.965Z Reads: 68

```
hey do you have vesc for sale
```

---
## \#80 Posted by: Mathias Posted at: 2018-04-25T02:36:27.195Z Reads: 67

```
@chaka has long gone. Don't expect him to reply here, sorry!
http://www.electric-skateboard.builders/t/merry-christmas-and-goodbye/41826
```

---
## \#81 Posted by: briman05 Posted at: 2018-04-25T11:44:23.444Z Reads: 55

```
I would contact him through Olin boards website. There was someone who was selling one.
```

---
