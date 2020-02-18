# Focbox mosfet explosion

### Replies: 40 Views: 2023

## \#1 Posted by: Whitehawk Posted at: 2018-02-13T19:16:09.773Z Reads: 337

```
Hi guys, do you think I can fix that ?

The focbox was pretty new, only used 2 or 3 times..

![IMG_20180212_220432|666x500](upload://5Qj5kSXCUpo2NrFXvkgMi3gYq5t.jpg)
```

---
## \#2 Posted by: scepterr Posted at: 2018-02-13T19:22:44.047Z Reads: 324

```
I wouldn't trust that pcb, even if it could be functional again
```

---
## \#3 Posted by: Martinsp Posted at: 2018-02-13T19:23:37.382Z Reads: 320

```
Hi, 
when a direct FET is blown in this way (violent I guess would be the best word) there is no exact way to tell if it is repairable until the FET is removed. This is because it all deprends on the pads underneath it. If they survived then yes you can repair it fairly easily if the pads are burned away then you can not really repair it. Also there might  be other traces that are burned so check that too.

EDIT: first step would be cleaning the PCB with some alcohol and examining the it further.
```

---
## \#4 Posted by: SOICDIP Posted at: 2018-02-13T19:24:50.829Z Reads: 304

```
What are your battery and current limit settings? FOC?
```

---
## \#5 Posted by: TarzanHBK Posted at: 2018-02-13T19:40:19.400Z Reads: 298

```
Well looks like you already cleaned away a much bigger mess there.
Did you throw it in a puddle under load?
Looks like it got destroyed from shit coming in
```

---
## \#6 Posted by: Martinsp Posted at: 2018-02-13T19:41:14.856Z Reads: 286

```
Yeah it looks like some water damage, you can see the case has a stain too in the background.
```

---
## \#7 Posted by: longhairedboy Posted at: 2018-02-13T19:57:28.965Z Reads: 278

```
i peed on it. I was skating along, just peeing on everything like i always do, when i saw him riding around and I peed on his board. I made sure to get the back real good by the phase leads and i also hit the box a few times before i had to make a quick getaway.
```

---
## \#8 Posted by: rok Posted at: 2018-02-13T20:03:54.677Z Reads: 271

```
You shouldn't take a piss at every thread you see, and your tag should definitely not be a "pissing skater" :point_up_2:
```

---
## \#9 Posted by: longhairedboy Posted at: 2018-02-13T20:30:30.378Z Reads: 261

```
![caution-esk8-urine|500x500](upload://9ShMWVcu6fMVYknIcNxueTRUIVU.png)
```

---
## \#10 Posted by: TarzanHBK Posted at: 2018-02-13T20:38:06.221Z Reads: 257

```
well seems like you ate sand again and peed it all over this thing..
I already see @JohnnyMeduse cleaning up that mess..
```

---
## \#11 Posted by: rok Posted at: 2018-02-13T20:38:16.795Z Reads: 252

```
I name you,

![original-15617-1446128823-11|360x240](upload://u1p1R3dJX9QRaWTtLYTfsKTaZ4f.jpeg)
```

---
## \#12 Posted by: Blasto Posted at: 2018-02-13T20:42:50.733Z Reads: 250

```
don't think this is salvageable, looks like it was exposed to salty road juice.

copper looks blown away

![image|342x500](upload://380T3L9BcwV2vhnhLXzbkogGFox.jpg)
```

---
## \#13 Posted by: chuttney1 Posted at: 2018-02-13T20:45:59.091Z Reads: 241

```
Why does the PCB area with mosfets look weird like it has liquid damage or something? What voltage did you run this at?
```

---
## \#14 Posted by: longhairedboy Posted at: 2018-02-13T20:46:36.828Z Reads: 238

```
there was definitely water/crud ingress. That's probably what blew it up.
```

---
## \#15 Posted by: TarzanHBK Posted at: 2018-02-13T21:06:33.622Z Reads: 231

```
i wouldn´t use it anymore, even if you change that mosfet, you still have corrosion on all other pads, which will lead to more faults like that in the future.
```

---
## \#16 Posted by: Martinsp Posted at: 2018-02-13T21:08:36.763Z Reads: 226

```
I think that you will need to replace all 6 because it is possible that if they are not dead yet they are on their way. The one you circled has most probably burned the pads underneath so remove it first, if it is good you may be able to fix it. So as of now you most probably have 6 fets, gate resistors and possibly DRV (maybe not if you are lucky, sometimes fets dont destroy DRV when they get damaged)
```

---
## \#17 Posted by: Whitehawk Posted at: 2018-02-13T21:47:26.321Z Reads: 225

```
Salt water ? That's a possibility :sweat_smile::laughing:

![playa|690x387](upload://A4cPbuoIASK9KaD4HpIwnTgF8gv.png)

All fet seems damaged :/

![IMG_20180213_223213|690x192](upload://wN5BkvPMLvi6Jz5jqijKbqpweMo.jpg)

Will do something more waterproof next time !
```

---
## \#18 Posted by: Martinsp Posted at: 2018-02-13T21:49:28.044Z Reads: 216

```
Yours dont seem to be as bad as OP`s
```

---
## \#19 Posted by: Whitehawk Posted at: 2018-02-13T21:53:05.262Z Reads: 213

```
OP's ? and how to desolder that shit ?
```

---
## \#20 Posted by: Martinsp Posted at: 2018-02-13T21:57:36.977Z Reads: 209

```
OP = original poster, the person that created the topic/thread

Hot air soldering station/iron is the right tool for the job.
```

---
## \#21 Posted by: Martinsp Posted at: 2018-02-13T21:59:04.273Z Reads: 198

```
Oh I just noticed that you can actually see that the traces underneath are burned/destroyed so the one on the left is done :/ You might be able to repair the one on the right using the working mosfets from the one on the left though.
```

---
## \#22 Posted by: Whitehawk Posted at: 2018-02-13T22:01:02.946Z Reads: 201

```
The right is working, just to compare with the burned focbox at left ^^

This board cost me a lot, a dual sleeping lion lost during shipping, now a burned new focbox.. 
But I want more power, I need to try vesc6.. but cost to much $$$ holly shiiiiiiit
```

---
## \#23 Posted by: Martinsp Posted at: 2018-02-13T22:03:51.188Z Reads: 203

```
Oh I see,

Other users iterations might be cheaper if it is a necessity for you.
```

---
## \#24 Posted by: Whitehawk Posted at: 2018-02-13T22:11:10.241Z Reads: 196

```
Stewii vesc6 clone ? It's recent, is it reliable ? ;)
```

---
## \#25 Posted by: ducktaperules Posted at: 2018-06-24T21:24:48.949Z Reads: 155

```
Did you ever resolve this. It looks like I have the same problem. Think I'm going to attempt a repair job. Anyone have a part number for the fets used?
```

---
## \#26 Posted by: Martinsp Posted at: 2018-06-24T21:38:03.358Z Reads: 153

```
I am not sure anymore how this was resolved but before you order the transistors, remove the burnt one/s to see if there is no damage to the PCB. If there is your device may unfortunately be unrepairable. Just so you dont unnecessarily buy the mosfets and end up not using them
```

---
## \#27 Posted by: SeanHacker Posted at: 2018-06-24T21:48:50.212Z Reads: 148

```
All esk8ers need extra MOSFETs laying around dude. ;)
```

---
## \#28 Posted by: Martinsp Posted at: 2018-06-24T21:53:48.241Z Reads: 155

```
Well yeah that is true.

Btw, you should check the gate resistors so that you can order them at once so you dont need to pay shipping twice.
```

---
## \#29 Posted by: JTAG Posted at: 2018-06-24T22:27:18.671Z Reads: 154

```
I recognise this, can you please help me repair this?
![IMG-20180528-WA0001|690x388](upload://2V5pQOkDCz6gGCYfEPWC1CKFzdS.jpg)
```

---
## \#30 Posted by: Martinsp Posted at: 2018-06-24T22:32:03.706Z Reads: 152

```
Did you try flashing the firmware? I think that thats the issue :D :D
```

---
## \#31 Posted by: TarzanHBK Posted at: 2018-06-25T06:24:26.543Z Reads: 139

```
that´s a classical "turn it off and on again"!
```

---
## \#32 Posted by: banjaxxed Posted at: 2018-06-25T10:31:29.063Z Reads: 135

```
Sad DirectFET syndrome

![image|487x500](upload://lIqShdsjIRfQnTqBQESWD0PTD4w.jpg)
```

---
## \#33 Posted by: ducktaperules Posted at: 2018-06-25T19:44:02.169Z Reads: 117

```
Mine does not look quite that bad. Im hoping most of the damage is superficial. its clear that the top right fet is damaged but i think the other 5 are ok. 

![IMG_20180619_172925|666x500](upload://oJMIUeLPHY8hPMEsB8IC2SqEEqI.jpg) 

Is there any easy way to test them without removing them?
```

---
## \#34 Posted by: Martinsp Posted at: 2018-06-25T22:25:45.006Z Reads: 108

```
You can test continuity between positive input and each phase wire, do the same with negative input.
```

---
## \#35 Posted by: ducktaperules Posted at: 2018-06-26T12:40:37.782Z Reads: 91

```
Just had some time to look at this in more detail. This is what the FET damage looked like under the TIM.

![IMG_20180619_172858|666x500](upload://rTxfWmWmmXcVxrRgXBUR41G7hze.jpg)

After cleaning up I start to get some clues as to whats happened.

![IMG_20180626_110444|666x500](upload://k60RLG8nVD63AdMDuE3RSaIu029.jpg)

Looks like the PCB has corroded and copper had been exposed on some areas. Also the edge of the FET seems to be corroded here. Maybe a short between the FET housing and copper has occurred.

![IMG_20180626_110743|690x399](upload://ke2utLMgAw6pCAlcIoKy8mse8KH.jpg)

Decided to remove the fet and asses the damage.

![IMG_20180626_111536|554x500](upload://j9QmP1y97diGd76MXmItUp2CunI.jpg)

Yep, that defenatley looks done.

![IMG_20180626_111830|426x500](upload://tzADyMV0JWrolqcOB5yVVoQe37U.jpg)

The board dident look great either. So I tried again to clean it up.

![IMG_20180626_112123|514x500](upload://7KOPMSiaoCQcuSVrm4Ex5ttcchY.jpg)

This actually doesn't look too bad. It looks like the PCB has worn down to the copper in a few areas. Maybe this is caused by vibration or maybe water ingress? not 100% sure. also cant work out how to check the other FETS without removing them which i don't really want to do if i can avoid it.

So I plan to re coat the bare copper areas again some how then replace the FET. 

Also if anyone with the same problem ends up here in the future then this is the datasheet for the replacement FET: https://www.infineon.com/dgdl/irf7749l2pbf.pdf?fileId=5546d462533600a40153560445e71ca2
I ordered replacement pack of 4 from RS for £12.

Wish me luck :)
```

---
## \#36 Posted by: Martinsp Posted at: 2018-06-26T15:45:24.970Z Reads: 81

```
I think that what you are saying as a scenario of what happened is possible, another option/explanation would be that there was a short due to water possibly and the copper heated up before/while the fet was burning and that cause the solder mask to peel off or loosen so when you cleaned it you rubbed it off. Either way, it looks very promising! I have not had most success with covering bare copper like this with UV curable solder mask, any other air drying masks did not work for me, just peeled off during soldering.

Nice pictures BTW, is that from a microscope or?
```

---
## \#37 Posted by: ducktaperules Posted at: 2018-06-26T16:08:49.397Z Reads: 77

```
pics just from my phone put in the eye-cup of a microscope, with much effort to keep things aligned :)
```

---
## \#38 Posted by: andtuanlaza Posted at: 2019-11-17T18:42:56.896Z Reads: 25

```
my focbox have IRF7759 mosfet.   you find in ALIEXPRES and EBAY    and 

https://www.reichelt.com/de/en/mosfet-n-ch-75v-26a-3-3w-directfet-l8-irf-7759-p137882.html
```

---
## \#39 Posted by: andtuanlaza Posted at: 2019-11-17T18:46:45.935Z Reads: 26

```
![IMG_20191117_024306|281x500](upload://s6Op3BeuBG6l6GOeZRRl8s6EWZl.jpeg) ![IMG_20191117_024416|281x500](upload://7qNwDd3Ri0OztLVFlWBfD30jiSt.jpeg)
```

---
## \#40 Posted by: andtuanlaza Posted at: 2019-11-17T18:48:26.831Z Reads: 26

```
in my case.   Two diferent Firware.   one firnware 3.3 master and ackmaniac 3.1xx slave


Is posible this a mistake??????????
```

---
