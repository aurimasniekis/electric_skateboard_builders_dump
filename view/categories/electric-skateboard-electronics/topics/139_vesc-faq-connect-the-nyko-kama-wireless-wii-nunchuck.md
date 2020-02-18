# VESC FAQ &#124; Connect The Nyko Kama wireless wii NunChuck

### Replies: 245 Views: 39668

## \#1 Posted by: onloop Posted at: 2015-08-26T04:26:32.653Z Reads: 1165

```

USE AT OWN RISK | INJURY OR DEATH COULD OCCUR
------------------------------------------------------------

**This instruction is for the controller pictured.** It might work with other brands but it might not.





<img src='/uploads/db1493/original/1X/09bddc1f4aa5f6f81ada1a3a79ba73f74b9e0619.jpg'>


----------


1. Disassemble the transmitter/receiver - remove the plastic case & find the wires.
-------------------------------------

<img src="/uploads/db1493/original/1X/f49590f04de13edbbae1f7a9554f0c61bc5ae8d1.jpg" width="640" height="374"> 


----------


2. Double check that all the wires are intact & well soldered onto PCB, then apply some hot glue to strengthen & protect the wires.
-------------------------------------
<img src="/uploads/db1493/original/1X/d1765c0451f1051e6dce6a46b82e16b73969767b.jpg" width="611" height="480"> 


----------


3. Attach the wires to the VESC in this way. Make sure you have a good connection. Soldering & Hot glue is an option to ensure reliability. Otherwise buy the JST connector, the type is. "JST-PH 2MM SPACING" 6pin
-------------------------------------
<img src="/uploads/db1493/original/1X/d56a7d9fbce8d8b25f36c377d9d7394b72652d65.jpg" width="596" height="500"> 


----------


4. Led on the receiver PCB should come on. Do bench test to see if connection & controls are reliable.
-------------------------------------


----------




- This information is provided for fun and learning
- Do not ride an electric skateboard using untested devices. 
- Wear a helmet and protective gear always.


*Special thanks to kwoolf1 for this information*
```

---
## \#2 Posted by: siggs3000 Posted at: 2015-08-26T17:15:17.823Z Reads: 947

```
This is awesome. I was hoping it would be this easy to somehow use the nunchuck. 

Is that white connector part of the Kama receiver and harvested out during the disassembly? Or is it something we need to pick up somewhere. If so, does that type of connector have a name?
```

---
## \#3 Posted by: onloop Posted at: 2015-08-26T23:23:15.366Z Reads: 908

```
the JST type is. "JST-PH 2MM SPACING" 6pin
```

---
## \#4 Posted by: lowGuido Posted at: 2015-08-29T15:38:31.539Z Reads: 883

```
does the nunchuck have the same cruise control functions as the wiiceiver when connected directly to the VESC like this?
```

---
## \#5 Posted by: elkick Posted at: 2015-08-30T19:52:19.885Z Reads: 828

```
Yes, it behaves the same way. And I also never lost connection again, which was sometimes tricky with the wiiceiver.
```

---
## \#6 Posted by: sl33py Posted at: 2015-08-31T01:55:32.151Z Reads: 803

```
Yes - built in:
[img]/uploads/db1493/original/1X/26a4c964c710bb06ad2539d6815a0282342eb558.jpg[/img]
```

---
## \#7 Posted by: lowGuido Posted at: 2015-09-16T11:10:34.769Z Reads: 740

```
hey, a random question for those who use the Nyko Kama. how often do you replace the batteries in the actual nunchuck?
```

---
## \#8 Posted by: Moja Posted at: 2015-09-17T02:58:57.149Z Reads: 719

```
Can I wire up both the Kama and GT2B receiver to the VESC and use which ever one I fancy using at the time or will the two conflict?
```

---
## \#9 Posted by: cmatson Posted at: 2015-09-17T03:16:38.078Z Reads: 709

```
I believe they will conflict, because in the BLDC you must configure it for one or the other. Each time you wanted to change, You'd have to change it on the computer software too.
```

---
## \#10 Posted by: Moja Posted at: 2015-09-17T03:32:39.662Z Reads: 692

```
It's more of a questions of if the hardware will conflict, I'm happy to plug the board in and change the settings in the software when I want to change over. The problem is that I plan to solder the Kama receiver as opposed to using a connector as It may come loose, this means it wont be too easy to disconnect it.
```

---
## \#11 Posted by: cmatson Posted at: 2015-09-17T11:31:56.409Z Reads: 675

```
ahh I see what you're saying now. To be honest, I don't know if that would have any negative affect. I'm betting it will work fine, because if one input is disabled in the settings, than it shouldn't matter what is plugged in. That being said, I haven't tried this, so I don't know anything for sure.
```

---
## \#12 Posted by: treenutter Posted at: 2015-09-23T13:50:02.935Z Reads: 703

```
Thanks for posting this @onloop. I gave it a try last night. I'm still new to soldering and had a tough time with the very small wires involved here. There may be some variation in the way the Nyko Kama is manufactured, I think that the wires connected to my receiver were a little different.

Here's an image of the receiver after I hot-glued the connections on the PCB and stripped the green and blue wires (magnified through my third-hand-tool). I also stripped the wires of my JST connector. Worth noting: the wires soldered to the receiver were very thin and fragile, like the hairs of a unicorn! There was a nylon\plastic filler inside. The nylon burnt away when I tinned the small wire. WARNING: These wires and casing are very easy to burn\melt! 
<img src="/uploads/db1493/original/1X/9be4aad037df34b4677406043010547d9f540015.jpg" width="421" height="500"> 

Here is what it looked like after I soldered all 4 wires to the JST connector and heat-shrinked them. I didn't do a very good job... look at the big balls of solder on two of the connections! The main problem I had was keeping the wires stable while I applied heat to them. It was an ugly process, due to my own lack of skill!
 <img src="/uploads/db1493/original/1X/91690ade2bc9a026cc580a4bc2cf78bce8671e58.jpg" width="690" height="420"> 


After getting them all connected, I added some extra hot glue and a heat-shrink tube to reduce clutter inside my enclosure. 
<img src="/uploads/db1493/original/1X/9735de17158ec6aa901847a5b06ca88422f9d59e.jpg" width="690" height="465"> 

I think I need to re-do this. Even if it works, I don't trust the connections I made to last while riding. Given the frailty of the wires, and my low level of skill,  I'm thinking that I'll remove the hot glue, de-solder the original connections to the receiver, and solder the wires from the JST connector directly to the receiver's PCB.
```

---
## \#13 Posted by: lowGuido Posted at: 2015-09-24T00:19:21.943Z Reads: 663

```
i found this really good tutorial on how to prep and tin a wire properly. 
there is a LOT of rubbish out there. and while you may find some of the steps a little bit anal its worth at least taking note.
http://www.youtube.com/watch?v=0SnOW2VdCTI

here's some tips:
use a good iron.
clean your iron
clean your join
tin everything first
use a small amount of solder to bridge heat into the wire
apply solder to the wire not the iron
clean the flux off
clean your damn iron
"the bigger the blob the better the job" is not a rule
```

---
## \#14 Posted by: treenutter Posted at: 2015-09-24T16:55:28.136Z Reads: 617

```
This is awesome thanks @lowGuido. This guy is a real pro! I've been doing most of these, but I'll admit that I have never cleaned the flux off of my joins. I thought I was using "no clean" flux, it says so on the label!
```

---
## \#15 Posted by: treenutter Posted at: 2015-10-02T14:45:07.678Z Reads: 622

```
@Moja on my setup, with both a GTB2 receiver and the Nyko Kama receiver installed, I can switch between the two just by using BLDC Tool and there doesn't seem to be an issue with leaving them both connected to the VESC. There's a minor power draw being pulled from the inactive receiver, but otherwise no issues that I can detect. 

I'll also note, since it seems to be a concern for some, that after some tests the nunchuck used with VESC seems like a reliable implementation. It connects instantly and I haven't had an issue with it yet. Between the nunchuck and GTB2, I prefer the nunchuck so far. The cruise control seems like it will be really useful, and you can activate reverse on-the-fly.
```

---
## \#16 Posted by: lowGuido Posted at: 2015-10-02T22:32:12.734Z Reads: 605

```
[quote="treenutter, post:15, topic:139"]
Between the nunchuck and GTB2, I prefer the nunchuck so far.
[/quote]

I'm with you on that one. so comfortable and easy. I'm Always on cruise control.
```

---
## \#17 Posted by: treenutter Posted at: 2015-10-05T15:42:42.317Z Reads: 609

```
@lowGuido do you use the Z-button reverse feature? When I bench test it, if I'm holding full-throttle and tap the Z button, it instantly activates the brake and flips to reverse. In practice, does it automatically slow down the rider if that happens? Or, does, uh, just say "eff physics let's reverse!"
```

---
## \#18 Posted by: lowGuido Posted at: 2015-10-05T15:49:29.767Z Reads: 607

```
My Z button is programmed for "boost" mode. I have no reverse so I cant really answer.
I don't really like the Idea of reverse.
```

---
## \#19 Posted by: treenutter Posted at: 2015-10-05T15:59:49.752Z Reads: 612

```
Oh my bad @lowGuido ; I should have mentioned that I'm referring to the nunchuck\VESC paring. I'm guessing you're using the wiiceiver? My question belongs in a VESC thread somewhere :smile:
```

---
## \#20 Posted by: lowGuido Posted at: 2015-10-05T16:19:52.273Z Reads: 616

```
your question is in the right spot. this is a VESC/nunchuck thread.
```

---
## \#21 Posted by: elkick Posted at: 2015-10-05T16:27:07.159Z Reads: 580

```
I use it frequently and it activates only after you came to a standstill. The VESC is not breaking unless you're doing it yourself. It's just going into neutral position.

It's a useful feature for example when you want to step back a little bit when crossing a street and you are waiting for traffic to disappear. Or irritating other people. :smile:
```

---
## \#22 Posted by: treenutter Posted at: 2015-10-05T16:41:32.633Z Reads: 564

```
Thx @elkick that's exactly what I was wondering!
```

---
## \#23 Posted by: lowGuido Posted at: 2015-10-06T17:51:30.162Z Reads: 569

```
@joren check out the information above with regards to the nunchuck dongle. 
I suggest that you do something similar with your wiiceiver soldering the receiver direct to the PCB for optimal reliability.
```

---
## \#24 Posted by: Mitch Posted at: 2015-10-17T05:17:47.620Z Reads: 555

```
Is anyone able to show how to wire the wii receiver to a duel VESC setup?
```

---
## \#25 Posted by: onloop Posted at: 2015-10-17T05:38:27.102Z Reads: 563

```
Check this out 
http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142
```

---
## \#26 Posted by: disastorm Posted at: 2015-10-21T09:18:38.969Z Reads: 534

```
Not sure how useful this is, but I found this thing which I believe can connect into the receiver and expose the pinouts so that you don't have to dismantle the receiver: https://www.sparkfun.com/products/9281

You still have the solder the connections, but it makes it more modular and if you ever need to replace the transmitter/receiver you can just plug it in instead of unsoldering and resoldering.
```

---
## \#27 Posted by: SwissFozz Posted at: 2015-10-21T16:15:52.804Z Reads: 516

```
Even better, couldnt the VESC be redesigned to just take the receiver as a slide on connection? Do away with all the need for wiring, solder connections etc....
```

---
## \#28 Posted by: claudiofiore88 Posted at: 2015-10-21T18:24:12.915Z Reads: 501

```
That thought has crossed my mind as well. Having a built in connector like the wiiceiver would be a good idea for those wanting to retain the integrity of their wireless nunchuck receivers. Couldn't someone just modify his pcb design since it's all open source? I wouldn't be surprised if it's been done already.
```

---
## \#29 Posted by: lowGuido Posted at: 2015-10-21T20:46:38.514Z Reads: 473

```
this is a bad idea guys. it sounds nice, but the socket will introduce a lot of dropouts and general problems.
myself, and almost all of my friends have slammed because of a slide on wiiceiver socket. 

solder on and save lives.
```

---
## \#30 Posted by: disastorm Posted at: 2015-10-21T23:01:19.242Z Reads: 461

```
I have heard about the intermittent issues of the wiiceiver. So are those issues actually due to the wii socket itself losing connection temporarily or is it due to something in the wiiceiver pcb ?

Also does anyone have a guide to dismantle the receiver? Do you just break the plastic ?
```

---
## \#31 Posted by: lowGuido Posted at: 2015-10-21T23:43:02.245Z Reads: 462

```
[quote="disastorm, post:30, topic:139"]
So are those issues actually due to the wii socket itself
[/quote]

Yes.

dismantling the dongle is easy.. they literally just pull apart.. no tools required.
```

---
## \#32 Posted by: disastorm Posted at: 2015-10-22T00:10:35.553Z Reads: 442

```
Ah I see. I tried pulling it apart last night but I couldn't do it. Maybe I need to pull harder.
```

---
## \#33 Posted by: lowGuido Posted at: 2015-10-22T00:40:09.298Z Reads: 437

```
there is a ring over the top of the plug that just slides off and the the 2 halves split apart. just apply brute force..
```

---
## \#34 Posted by: SwissFozz Posted at: 2015-10-22T15:52:34.880Z Reads: 431

```
Yep. You just need to slip the ring off, then slide your nail into the crack and then lever them apart. Nothing more. DON'T go in deep with a knife as the contents inside are all a bit weak and flimsy and could easily be damaged.

Gently does it! Good luck!
```

---
## \#35 Posted by: disastorm Posted at: 2015-10-22T17:26:09.985Z Reads: 429

```
I ended up prying it apart by using a string in the crack and then wrapping it around my hand and pulling it apart.
```

---
## \#36 Posted by: Moja Posted at: 2015-11-03T21:29:56.201Z Reads: 437

```
I've soldered the Nyko PCB to the VESC but I am still getting drop outs, even with lots of hot glue to keep things in place. What other influences would cause the nunchuck to loose connection for short moments? I also have a GT2B receiver hooked up which could potentially be interfering.
Thoughts?
```

---
## \#37 Posted by: lowGuido Posted at: 2015-11-04T05:24:41.721Z Reads: 450

```
Thats strange. In all of my builds i have always used a nyko kama. At first i used the slide on  plug and was getting dropouts.  After soldering I very rarely get any droppouts at all. I went back to riding my original prototype.  And it was dropping out every couple of minutes.  I couldnt believe how bad it was. So i soldered that one on too. And behold no more droppouts. However I have never used a VESC or a GT2B so I cant coment on those.

..one day my VESC will come.

Edit: how good is your soldering. ?  If you have dry joins you may still get droppouts. I am a soldering boss :p so I wouldnt have that problem.
```

---
## \#38 Posted by: trbt555 Posted at: 2015-11-05T19:11:57.223Z Reads: 448

```
Please excuse my ignorance, but what does "solder it to the VESC" mean exactly ?
Is there another way ?
```

---
## \#39 Posted by: lox897 Posted at: 2015-11-05T20:50:16.444Z Reads: 453

```
Yes, use torqueboards wiiceiver. It means that you take the pcb out of the receiver and solder it directly to the vesc. Search up what solder means.
I'm pretty sure this is how it's done let the pro's chime in though.
```

---
## \#40 Posted by: lowGuido Posted at: 2015-11-06T01:49:33.651Z Reads: 458

```
Just scroll up.
All the information is in this thread.
```

---
## \#41 Posted by: trbt555 Posted at: 2015-11-06T08:11:19.302Z Reads: 426

```
If the thread was clear to me I wouldn't be asking the question but thanks anayway.
```

---
## \#42 Posted by: lowGuido Posted at: 2015-11-06T12:10:58.354Z Reads: 426

```
get a soldering iron and solder the wires from the nunchuck receiver on to the VESC circuit board. Or a JST connector to plug in. There are lots of pictures of how to do it in this thread.
there really is all of the information up there. I even posted and instructional video on how to solder
```

---
## \#43 Posted by: siggs3000 Posted at: 2015-11-12T01:52:17.020Z Reads: 422

```
Interestingly it seems that the latest VESC that I just got has a 7-pin connector where the previous 6-pin was located in the image at the top of this thread... From reading the pin descriptions on the bottom of the board, it seems that there's now a pin for "ADC2" and I *think* I can still follow the steps in this thread and just plug my 6-pin female JST in to the 6 pins that are closest to the other port (further from the motor wires)

Does that seem right?
```

---
## \#44 Posted by: kai Posted at: 2015-11-12T02:00:52.705Z Reads: 405

```
Someone posted a pic in another thread. Just search 7 pin connector
```

---
## \#45 Posted by: chaka Posted at: 2015-11-12T02:05:53.901Z Reads: 397

```
Yeah, you got it. Just leave adc2 open.
```

---
## \#46 Posted by: treenutter Posted at: 2015-11-12T02:08:42.149Z Reads: 390

```
@siggs3000 that's correct based on my read of it.
```

---
## \#47 Posted by: siggs3000 Posted at: 2015-11-12T02:08:54.127Z Reads: 398

```
Thanks @chaka

So the pins that I will not be using are:

 - adc2 
 - 5v 
 - adc
```

---
## \#48 Posted by: chaka Posted at: 2015-11-12T02:16:21.763Z Reads: 387

```
Correct! Red-3.3v, Black-GND, Blue-SDX/TX, Green-SCL/RX.
```

---
## \#49 Posted by: treenutter Posted at: 2015-12-03T16:31:09.256Z Reads: 402

```
@lowGuido or maybe @claudiofiore88 or @jacobbloy; to solder the Nyko Kama receiver directly to VESC, do I need to remove the JST connector port? If so, any tips on doing it safely? Once removed, then it's just a through-hole soldering job, like soldering the servo wires to VESC, correct?
```

---
## \#50 Posted by: lowGuido Posted at: 2015-12-03T22:08:34.632Z Reads: 419

```
the best way to do it is to use a desoldering iron such as this one.
<img src='/uploads/db1493/original/2X/1/12116f65d1251c37779838dcc029548c157228e3.jpg'>
gently remove all the solder from each pin and then just slide the connector off the board.

be careful not to lift the tracks!
```

---
## \#51 Posted by: tomtnt Posted at: 2015-12-03T23:56:13.573Z Reads: 406

```
just solder onto the pads on the back of the VESC instead of completely removing the JST connector... I actually do both for redundancy - I solder my nyko receiver to the back of the VESC and also use the JST connector.. seems to work better now.
```

---
## \#52 Posted by: Moja Posted at: 2015-12-14T10:11:33.285Z Reads: 382

```
The new VESC has a 7 pin port where the Nyko PCB attatches to, the previous had 6 pins. Where should I solder the wires to now?
```

---
## \#53 Posted by: trbt555 Posted at: 2015-12-14T11:37:28.732Z Reads: 380

```
[Here][1] you go.


  [1]: http://www.electric-skateboard.builders/t/the-vesc-the-ultimate-bldc-motor-controller/17/48
```

---
## \#54 Posted by: Moja Posted at: 2015-12-14T12:14:03.190Z Reads: 391

```
The wires are green, blue, red and black. That just illustrates plugging a 6 pin connector into a 7 pin port. Im looking for the sequence for the wiring. Without realising there was a 7th pin I soldered it on from bottom to top leaving 2 pins after the red and I get no power to the Nyko PCB.
```

---
## \#55 Posted by: trbt555 Posted at: 2015-12-14T13:49:27.815Z Reads: 393

```
According to the top of this thread:
Red = VCC -> VCC
Black = GND -> GND
Green = Clock -> RX_SCL
Blue =  Data -> TX_SDA

Schematic for 4.11 [here][1].


  [1]: https://github.com/vedderb/bldc-hardware/blob/master/design/BLDC_4.pdf?raw=true
```

---
## \#56 Posted by: Braylon31 Posted at: 2015-12-19T01:35:56.994Z Reads: 393

```
@jacobbloy ..i   got the jst connection pin but the receiver still seems to drop out every now and then is this a issue in the Bdlc tool R should I solder to improve connection also I was thinking maybe it could be a sensor problem I am using a unsensored motor and hall sensors cannot be detected when I do a motor detection..... but it seems to connect somtime when i get to rolling good and the controls kick in but im scared they would lose signal at a crucial time is this a easily fix problem also i would like to add every connection seems pretty secure
```

---
## \#57 Posted by: Braylon31 Posted at: 2015-12-19T01:42:34.178Z Reads: 395

```
Did it loose signal from timt to time i just did mine threw connectors and it goes in and out i thought signal would be a little more solid whats your thoughts?  Please help
```

---
## \#58 Posted by: skillerftwer Posted at: 2015-12-19T19:51:58.110Z Reads: 383

```
Hello everyone,
I soldered my kama PCB to the VESC as instructed. The nunchuck connects instantly without a problem. Unfortunately I can't get the display in the BLDC tool to move from 50%. I have watched Ben's videos and followed along but it still doesn't work. The led on the PCB blinks once when I hit the Z or C buttons but does nothing when moving the joystick. Could this be a problem with the actual nunchuck?
```

---
## \#59 Posted by: lowGuido Posted at: 2015-12-19T19:54:26.894Z Reads: 390

```
I just remembered that I have my wires looped about 6 turns through a toroid. maybe that's why I dont get dropoouts.
```

---
## \#60 Posted by: kai Posted at: 2015-12-19T20:01:58.973Z Reads: 390

```
Can we see some pics of that when you get a chance?
```

---
## \#61 Posted by: treenutter Posted at: 2015-12-19T21:33:27.269Z Reads: 375

```
@skillerftwer it sounds like you've got the receiver wired properly, and that your remote is syncing with your receiver. Have you made sure to select "Nunchuck" on the "App Configuration > General" tab in BLDC Tool? You also have to go to the "App Configuration > Nunchuck Tab" 
and select "Current" or "Current with Reverse." Whenever you make a change in BLDC Tool, you have to "write configuration," and I usually reboot VESC after as well.
```

---
## \#62 Posted by: skillerftwer Posted at: 2015-12-20T03:37:44.619Z Reads: 376

```
@treenutter Thanks for the reply! 
Yep, that's how I was attempting to set it up before. Went back and did those steps again just to be sure but, still nothing. Going to take apart the nunchuck and see if anything is loose. I'll also resolder the connections just to eliminate that possibility.
```

---
## \#63 Posted by: treenutter Posted at: 2015-12-20T04:55:44.172Z Reads: 370

```
@lowGuido does a toroid perform the same function as a ferrite ring?
```

---
## \#64 Posted by: lowGuido Posted at: 2015-12-20T08:14:26.874Z Reads: 372

```
[quote="treenutter, post:63, topic:139"]
toroid perform the same function as a ferrite ring?
[/quote]

yeah, toroid. ferrite ring. same same.
```

---
## \#65 Posted by: skillerftwer Posted at: 2015-12-23T21:27:04.603Z Reads: 370

```
Got a new nyko kama, didn't fix the problem. I think it's the VESC. I had a PPM controller hooked up so I could test ride. This was working just fine up until I tried to connect the new kama... now the PPM powers up like normal and links the receiver to the controller but it won't move off 50% similar to the Kama. I will try another VESC
EDIT: PPM still works fine I just had it plugged in the wrong channel...
```

---
## \#66 Posted by: sgaana Posted at: 2015-12-23T21:54:55.462Z Reads: 377

```

So instead of having to buy a 7 pin connector, I can connect 6 pin to this connector?
<img src="/uploads/db1493/original/2X/6/6dcb879486fed327adee4034fe66edcf8b1d0ec9.png" width="386" height="500">
```

---
## \#67 Posted by: siggs3000 Posted at: 2015-12-24T00:04:22.823Z Reads: 363

```
Yes, as long as you avoid these pins:

adc2
5v
adc
```

---
## \#68 Posted by: kai Posted at: 2015-12-24T00:04:34.613Z Reads: 359

```
No i dont think so bro. You still put it in the 7 pin one.
```

---
## \#70 Posted by: kai Posted at: 2015-12-24T00:14:03.985Z Reads: 362

```
He circled the 6 pin connector in the pic. So no! Dont connect to that one. Just use the 6 pin connector in the 7 pin slot
```

---
## \#71 Posted by: chaka Posted at: 2015-12-24T00:14:16.451Z Reads: 362

```
Hey @siggs3000 Move your 6 pin connector over one pin and you should be able to get a connection. As it is now the dongles 3.3v wire is connected to GND on the VESC. Basically you want to hug the other end of that 7 pin jst port.
```

---
## \#72 Posted by: siggs3000 Posted at: 2015-12-24T00:16:13.282Z Reads: 362

```
Oh son of a bee sting... I'll remove my pic so it's not misleading for future visitors! Thanks @chaka!

(I still want the badwolf when it's ready to rock though :)
```

---
## \#73 Posted by: kai Posted at: 2015-12-24T00:49:19.259Z Reads: 360

```
can someone please post a pic of the 7 pins marked so this isnt so confusing?
```

---
## \#74 Posted by: chaka Posted at: 2015-12-24T01:00:39.511Z Reads: 382

```
Here you go!

<img src="/uploads/db1493/original/2X/1/10551c2b4b035cbc8db66a7f592bdc8f3d23827c.jpg" width="606" height="500">
```

---
## \#75 Posted by: BigAl Posted at: 2015-12-24T01:04:42.548Z Reads: 378

```
I can't take credit for this pic @elkick posted this on my thread.  This works.

Al... 

[URL=http://s276.photobucket.com/user/BigAlinmiami/media/image-2_zpswribd6ro.png.html][img]/uploads/db1493/original/2X/5/5830489892d6f529be4dac94fddebd19705864a0.png[/img][/URL]
```

---
## \#76 Posted by: kai Posted at: 2015-12-24T01:25:28.782Z Reads: 360

```
thanks @chaka and @BigAl  . we needed this in this thread. i did see that pic that was posted on your build thread @BigAl . i just felt it was needed here when people search for this information.
```

---
## \#77 Posted by: sgaana Posted at: 2016-01-10T21:14:37.924Z Reads: 362

```
I have my dual VESC and Nyko receiver powered up. How do I pair my Nyko to the receiver? I read something in this forum  but can't find it!
```

---
## \#78 Posted by: trbt555 Posted at: 2016-01-10T21:32:21.976Z Reads: 368

```
Just push the S button and you should get a steady blue LED.
```

---
## \#79 Posted by: disastorm Posted at: 2016-01-16T08:31:18.576Z Reads: 361

```
My receiver's led isn't turning on. Does that mean something is wrong ? My receiver's pcb ended up being one of the weird non standard ones.
```

---
## \#80 Posted by: Iceni Posted at: 2016-01-16T08:40:33.112Z Reads: 359

```
It should blink when plugged in and switch to a steady light when synced to the controller.

Check to make sure you've plugged the cables to the correct pins.
The pins are marked on the pcb.

Though it can be you got an incompatible one if it's not standard
```

---
## \#81 Posted by: disastorm Posted at: 2016-01-16T08:43:25.347Z Reads: 368

```
everything looks good to me. I guess I'll try getting another nunchuck. The light is supposed to be the one on the receiver right, not the vesc ? There was no diagram for my receiver's pcb so I had to determine which wires were which signals based on where they were located in the actual wii connector. I thought I had done it right, but maybe it was wrong.
```

---
## \#82 Posted by: Iceni Posted at: 2016-01-16T08:56:29.394Z Reads: 337

```
Yes, the recievers light.
I guess the only thing you can do is really doublecheck everything. If everything checks out connectionwise it's propably a dud kama. It's unfortunatly not uncommon.
```

---
## \#83 Posted by: disastorm Posted at: 2016-01-16T08:59:16.472Z Reads: 343

```
I found this thread from endless sphere where someone actually had the exact same receiver as me, and he hooked it up properly ( same way as I did based on the diagram ) and his didn't work either.

https://endless-sphere.com/forums/viewtopic.php?f=35&t=69557

Is it possible that some of the receivers need 5v instead of 3.3v ?
```

---
## \#84 Posted by: Iceni Posted at: 2016-01-16T09:45:12.187Z Reads: 341

```
Doubt it, the wiimote delivers around 3v to it's accessories.
```

---
## \#85 Posted by: disastorm Posted at: 2016-01-16T09:48:14.431Z Reads: 343

```
oh ok, i guess maybe theres just something wrong with that model. Btw has anyone ever tried out this nunchuck? http://www.amazon.com/Z-Chuk-Wireless-Nunchuk-Controller-Nintendo-Wii/dp/B002A1O4RW/ref=sr_1_fkmr0_2?s=videogames&ie=UTF8&qid=1452937067&sr=1-2-fkmr0&keywords=mad+catz+z+chuck
```

---
## \#86 Posted by: Iceni Posted at: 2016-01-16T10:41:56.140Z Reads: 339

```
I ordered two of them, neither worked  on the vesc.
They work really well on the wii though :P
```

---
## \#87 Posted by: sgaana Posted at: 2016-01-16T16:18:42.078Z Reads: 336

```
I have Nyko Kama and a blue light should come on like this:
<img src="/uploads/db1493/original/2X/a/af2bb21184fa7dbf0b73d75620a9874eecab74db.jpeg" width="666" height="500">
I bought two Nyko Kama on eBay.
```

---
## \#88 Posted by: disastorm Posted at: 2016-01-16T18:54:58.778Z Reads: 333

```
[quote="Iceni, post:86, topic:139, full:true"]
I ordered two of them, neither worked  on the vesc.
They work really well on the wii though :P
[/quote]

I see, I found a thread on endless sphere where someone actually said the mad catz z-chuck worked for them.

So I guess maybe all the nunchucks are like that... some of them work and some don't.. really annoying that you have to get lucky to get one that works.

@sgaana Do you know which seller that is? Is there a place to order that will always be a version that works ?
```

---
## \#89 Posted by: elkick Posted at: 2016-01-16T19:48:27.037Z Reads: 324

```
Madcatz nunchuk is not working while directly connected to VESC, maybe people who have tried this were using an additional wiiceicer. In that combination it might work with madcatz. 

I ordered 10 Kama nunchucks from a seller "viedogamesdivawholesale" through eBay, all of them are working.
```

---
## \#90 Posted by: disastorm Posted at: 2016-01-16T20:00:38.346Z Reads: 326

```
[quote="elkick, post:89, topic:139, full:true"]
Madcatz nunchuk is not working while directly connected to VESC, maybe people who have tried this were using an additional wiiceicer. In that combination it might work with madcatz. 

I ordered 10 Kama nunchucks from a seller "viedogamesdivawholesale" through eBay, all of them are working.
[/quote]

great thanks for the info. I'll try that guy out.
 It looks like you were right, the thread I saw was referring to the wiiceiver.
```

---
## \#91 Posted by: lowGuido Posted at: 2016-01-16T20:01:51.233Z Reads: 322

```
anyone in oz wanna go halves in a box of 10? LOL?
```

---
## \#92 Posted by: disastorm Posted at: 2016-01-16T20:03:45.419Z Reads: 316

```
[quote="lowGuido, post:91, topic:139, full:true"]
anyone in oz wanna go halves in a box of 10? LOL?
[/quote]

If you are referring to that ebay user, he also sells the individuals: http://www.ebay.com/itm/Nyko-Wireless-Kama-Nunchuck-Full-Motion-Ergonomic-Controller-for-Nintendo-Wii-/151631307431?hash=item234dee22a7:g:yvEAAOSwEeFVFGO2
```

---
## \#93 Posted by: lowGuido Posted at: 2016-01-16T20:07:17.342Z Reads: 310

```
yeah its way too expensive to pay shipping for just 1.
```

---
## \#94 Posted by: sgaana Posted at: 2016-01-16T20:15:55.519Z Reads: 307

```

I bought a black one from: http://www.ebay.com/usr/eparts-plus-more
Another white one from: http://www.ebay.com/usr/mw-ldub?_trksid=p2047675.l2559
I think it was pure luck that mine are working with VESC.
```

---
## \#95 Posted by: elkick Posted at: 2016-01-16T20:26:00.496Z Reads: 309

```
Due to demand he seem to have increased the price by 50%, they were 13$ when I ordered those some months ago.
```

---
## \#96 Posted by: disastorm Posted at: 2016-01-17T03:41:07.574Z Reads: 317

```
I actually ordered this for same day delivery from amazon and I just got it and it looks like it works ( at least it powers on. I'll have to check to see if it works via BLDC )

http://www.amazon.com/Nyko-Wireless-Kama-Black-Nintendo-Wii/dp/B0047SFGDW/ref=sr_1_1?ie=UTF8&qid=1453002057&sr=8-1&keywords=wireless+nyko+kama

At the time of this writing the seller is "Carpe_Diem" and "Fulfilled by Amazon"
```

---
## \#97 Posted by: Hummie Posted at: 2016-01-17T04:00:12.927Z Reads: 315

```
[quote="disastorm, post:81, topic:139"]
everything
[/quote]


I was using the quanum 22$ from hobby king. It was fine but I kept breaking receivers (3) and the batteries seem to get sucked out by every third or fourth ride.  I broke the third receiver banging it so I hooked up the nunchuck.  I was worried about it to begin with having read things and thought i could get it hard wired and be safe.  I didnt hardwire it.  After being ok for maybe a slow 3 miles I got bolder and a couple of times it would full throttle on me for 2 seconds after I had let go of full throttle and then maybe throw on the brakes!  I don't know if it's from lost connection or not.  I hear Bluetooth is not a safe connection.  I miss my safe 22$ trans and ordered one immediately. 

Is it true the it's going to be inherently unsafe because it's Bluetooth? 

It's a nice control and worked nicely and I adjusted to it quickly and it looks cool and convenient but for me no way.
```

---
## \#98 Posted by: disastorm Posted at: 2016-01-17T06:42:06.859Z Reads: 302

```
Yea I've also been wondering what the effects of dropouts are? I havn't set mine up so I don't know if I'll get them, but what will happen when a connection "drops out" ? Will it immediately brake, accelerate, coast, or what ?
```

---
## \#99 Posted by: trbt555 Posted at: 2016-01-17T09:01:37.780Z Reads: 317

```
Unpredictable at least. Maybe any of those.
If you're using a VESC, there's a safety timeout that will go to neutral or brake when there's no control input but unfortunately we don't know what the Nyko receiver does when it loses signal from the nunchuck. Does it keep sending the last throttle input it was receiving ? Does it just do nothing ? It certainly doesn't have a fail-safe mode like conventional RC receivers have. Those can be programmed to go to a predetermined setting when the signal drops.

I have a nunchuck and haven't had any problems yet.
I replaced the wires on the receiver entirely with longer ones and I put it as far as I could from the controllers. I also put the receiver back in it's case for protection.
It's on the bottom left in this picture:
<img src="/uploads/db1493/original/2X/3/387c821075d50bc4da5fa8a3d6e3df310d67d28a.jpeg" width="375" height="500">
```

---
## \#100 Posted by: disastorm Posted at: 2016-01-17T19:08:57.548Z Reads: 306

```
I see, I just figured if its happened to so many people, maybe they would actually know what happens. Another question is also how do you know when you need to replace the batteries on the nunchuck? There is no display, right, and I imagine you wouldn't want to just randomly run out of batteries while riding around one day. Is there some standard that people follow to replace before it runs out ? Does the nyko nunchuck have any built in method to tell you, like flashing a certain color or something ?
```

---
## \#101 Posted by: lowGuido Posted at: 2016-01-17T19:32:42.863Z Reads: 327

```
I'm about 99% sure any nunchuck dropouts come from not soldering the dongle directly.
if you don't solder the nunchuck dongle you can expect anything from random full throttle to zero response at all.
just expect to street your face any time you ride with a non soldered dongle.

my chuck batteries seem to last for ages. I think I have only replaced them like 2 or 3 times in 800km! 
to be sure I always ride with a couple of AAA's in my pocket.  its not too much baggage. plus its also not too hard to grab a pair from any nearby shop if you did happen to run out.
also I'm fairly sure the LED flashes when they are running low. 
it also flashes if you lose signal.

TLDR:
BAD:
<img src="/uploads/db1493/original/2X/b/bc5ed305da806ecb09f729ed1af4589395c7b254.jpg" width="616" height="500">



GOOD:
http://www.electric-skateboard.builders/uploads/db1493/original/1X/91690ade2bc9a026cc580a4bc2cf78bce8671e58.jpg
```

---
## \#102 Posted by: trbt555 Posted at: 2016-01-17T20:12:39.331Z Reads: 314

```
Yep, the led flashes when the batteries are low.
```

---
## \#103 Posted by: jonathanngkh Posted at: 2016-01-21T17:34:39.831Z Reads: 320

```
Please note that the diagram above doesn't apply anymore, if you're just going by the order of the wire colours, due to changes in the new VESC board.

However, if you follow the label pin names, you'll get it right!

<img src="/uploads/db1493/original/2X/d/d05a3119b1c1fc321a9baba914f73572aca16d39.jpg" width="667" height="500">
```

---
## \#104 Posted by: lowGuido Posted at: 2016-01-21T21:53:22.701Z Reads: 302

```
yeah I wasn't using the image as a wiring reference, just an example of soldering.
if you scroll up the page a bit there is a correct wiring diagram.
```

---
## \#105 Posted by: treenutter Posted at: 2016-01-21T23:42:03.451Z Reads: 306

```
@lowGuido I always that that you wanted us to solder the wires directly to VESC. In the "good" example above, the JST port plugs into VESC. have you had a change of heart? You're the main of soldering advocate on the forum!
```

---
## \#106 Posted by: lowGuido Posted at: 2016-01-22T00:08:51.226Z Reads: 319

```
I was only putting some images that I found in google search. that was not my ideal choice but it was here on the forum already. 
sorry I couldn't find any directly soldered ones.

to be correct I still stand by my "solder all the things" statement
<img src="/uploads/db1493/original/2X/7/7c2b8b63aea0ccd4bb8a7d03af06eb487aab32f6.jpg" width="411" height="400">
```

---
## \#107 Posted by: Ross Posted at: 2016-02-03T09:43:11.613Z Reads: 311

```
Hi tbrt555,

how have you split the power wires in this photograph? They look very neat indeed! Have you just soldered both negatives / positives to the one 5.5mm bullet, or did you find a splitter of some sort? I just soldered all three wires together as neatly as i could, but it took a lot of heat! (8 AWG wire) What gauge is this wire?
```

---
## \#108 Posted by: trbt555 Posted at: 2016-02-03T10:30:45.826Z Reads: 303

```
Its 12AWG wire.
I first stripped both wires and I strapped the cores together using a single strand of copper wire.
I then applied heat and soldered the strapped cores together.
Then I soldered the joined wires to the bullet connector.
```

---
## \#109 Posted by: Ross Posted at: 2016-02-03T11:38:25.860Z Reads: 301

```
Ahhh, thanks. 

Yeah 12 AWG would make things a lot easier! I went with 8 gauge because of all the talk about cable length for FOC. Im sure 10 probably would have been fine though as the cables are very short. Haven't actually tried FOC yet as one of my VESCs died after my first few successful test rides :-( Waiting on a new one now. Was running on 12S lipo, but with heat sinks and active cooling fan. No idea what killed it.
```

---
## \#110 Posted by: treenutter Posted at: 2016-02-03T16:01:45.478Z Reads: 282

```
Got ya @lowGuido.  I still haven't seen a VESC-soldered-to-Kama-reciever image anywhere. It seems like everyone uses the JST port on VESC. Has anyone soldered it directly?
```

---
## \#111 Posted by: lowGuido Posted at: 2016-02-03T16:19:39.552Z Reads: 285

```
I received a pair of VESC's from @chaka a few days ago, and I have ordered 2 Nyko Kama's (along with $40 shipping fee) from amazon, so watch this space..

I should point out, I am not saying that the JST is sub standard or that it wont work. I just believe that on a skateboard the amount of vibration is greater than any of these plugs are designed to handle, and soldering just removes all doubt.
```

---
## \#112 Posted by: Mitch Posted at: 2016-02-22T09:36:33.017Z Reads: 292

```
Has anyone found a problem to the Nyko Kama not activating the motors?

The receiver light turns on and nyko kama remote connects and receives signals as when i push a button on the remote the receiver light flashes on and off, but does not spin the motors.

Using BLDC I can spin either motor just not using the remote.
```

---
## \#113 Posted by: trbt555 Posted at: 2016-02-22T12:04:40.965Z Reads: 289

```
Have you double checked your wiring ?
Did you reboot after setting the Nunchuck app in the BLDC/VESC ?
Can you see the input bar move in BLDC nunchuck tab ?

My Nyko Kama receiver only has one blue led, to indicate signal from the nunchuck.
It only flashes when there's no connection, never when I press a button.
```

---
## \#114 Posted by: onloop Posted at: 2016-02-22T12:47:17.434Z Reads: 285

```
in BLDC tool, app tab, what control method is selected?
```

---
## \#115 Posted by: Haimindo Posted at: 2016-03-25T19:36:56.902Z Reads: 282

```
Wired my dual setup and tried the nunchuck for the first time and at first it worked as it should work. But then I tried the connection by walking to the next room and suddenly it went full thorttle, luckily the board was upside down. Is this normal would the soldering help? I use the chakas pre soldered receiver with jst-plug to vesc
```

---
## \#116 Posted by: torqueboards Posted at: 2016-03-25T19:40:47.877Z Reads: 273

```
@Haimindo - Usually an issue with the Nyko Kama + receiver (bluetooth). Some people have mentioned they soldered it and connection was a lot more stable.
```

---
## \#117 Posted by: trbt555 Posted at: 2016-03-25T21:57:44.943Z Reads: 275

```
Is that behavior repeatable ?
What timeout settings do you have set ?
```

---
## \#118 Posted by: Haimindo Posted at: 2016-03-25T22:26:26.283Z Reads: 270

```
It happened twice. First when I was 3 meters from board and second time when I was just next to it. I'll update the Vescs to the latest firmware and check the settings tomorrow :thumbsup:
```

---
## \#119 Posted by: claudiofiore88 Posted at: 2016-03-25T22:29:32.932Z Reads: 280

```
Jeeze! That's scary.  Think i might ditch the Nunchuck when my VESC's come in and go with @torqueboards remote or something similar. Cruise control isn't necessary.
```

---
## \#120 Posted by: trbt555 Posted at: 2016-03-25T22:30:24.296Z Reads: 284

```
For the record, I've been using a nunchuck for several weeks now without a single hiccup.

Sounds like you may have interference from something indoors.
```

---
## \#121 Posted by: chaka Posted at: 2016-03-25T22:32:41.615Z Reads: 286

```
Yeah thats normal, scary isn't it. It does not do that when you lose connection, oddly enough. So turn it off if you plan on walking away from your board ;)
```

---
## \#122 Posted by: Haimindo Posted at: 2016-03-25T22:34:06.244Z Reads: 268

```
Good to know, I'll try different scenarios tomorrow and report to you guys
```

---
## \#123 Posted by: lowGuido Posted at: 2016-03-25T23:12:06.262Z Reads: 279

```
I have been usinf nyko kama nunchucks for years with no issues. 
I have built 7 boards and all of them use the chucks.
All of them are soldered IF YOU DON'T INTENDED TO SOLDER THEM DONT USE THEM. 
Also I never walk away from my board. Nunchuck is designed for close use. Like a couple of meters soldering wont improve that.
```

---
## \#124 Posted by: massy Posted at: 2016-05-05T23:31:55.821Z Reads: 268

```
So I soldered mine and there were still problems. However I figured out it was the motor wires screwing up the signal. Placing the receiver close to the wires and applying throttle instantly screws up the signal. Moving it 10 cm from the wires and everything is fine. 

It should be added to the guide that the receiver should be AT LEAST 5-10 cm from any wires with lots of current going through. Mine is VERY stable after getting longer wires and relocating it.
```

---
## \#125 Posted by: Bender Posted at: 2016-05-06T00:58:52.446Z Reads: 260

```
would a ferrite ring help with this too?
```

---
## \#126 Posted by: lowGuido Posted at: 2016-05-06T03:05:57.964Z Reads: 276

```
Probably.  I usually run ferrite on all my recievers
```

---
## \#127 Posted by: Trademarc Posted at: 2016-05-12T22:17:32.475Z Reads: 281

```
Has anyone ever used another brand controller? I bought one from GameStop expecting a kama but I got the one in the pic instead. Think it'll work?<img src="/uploads/db1493/original/2X/6/632350a1314feb9567e2968fc969e86890442d15.jpeg" width="375" height="500">
```

---
## \#128 Posted by: lowGuido Posted at: 2016-05-12T22:48:20.382Z Reads: 272

```
im pretty sure only the Nyko Kama and maybe the memorex are tested to work.

having said that if you can find some others that also work go right ahead and post your findings!
(unfortunately most don't work for some reason)

if you have a wired chuck then the data lines are all the same, and should always work. all brands of wired chuck seem to work.
however depending on how the particular brand utilizes their wireless data handshaking to get the data to the dongle will determine if it will work.
It stands to reason that every nunchuck should be able to work, as long as you can convince it that it is indeed talking to a nintendo on the other end and you are in the middle of playing a game.
how you do that? I'm not sure. but I bet there's a way.


TLDR: all the nunchuck data streams are the same and should work. however wireless comms are not the same and may not.
```

---
## \#129 Posted by: Trademarc Posted at: 2016-05-12T22:57:40.219Z Reads: 263

```
Ok, well I've already bought it, so I may as well give it a shot I suppose...
```

---
## \#130 Posted by: lowGuido Posted at: 2016-05-12T23:02:23.276Z Reads: 267

```
Id love to find some new options.. im sick of paying $55 for Kamas shipped from USA.
(even if they are still the best skate controller. haterz :smiling_imp:)
```

---
## \#131 Posted by: Trademarc Posted at: 2016-05-12T23:10:16.445Z Reads: 275

```
I found out I can return it within 7 days, but my other parts don't come in until later this month, so I'm trying to decide whether to risk it and hang onto it and take one for the eSk8 community by possibly finding a cheaper alternative, or just returning it...
```

---
## \#132 Posted by: sgaana Posted at: 2016-05-15T22:24:49.236Z Reads: 273

```
Will this one work?
http://www.ebay.com/itm/New-Wireless-Nunchuck-for-Nintendo-Wii-Wii-U-Black-White-/281867479438?hash=item41a09c698e:g:uBsAAOSwwE5WVjN0
```

---
## \#133 Posted by: Trademarc Posted at: 2016-05-16T00:30:59.325Z Reads: 272

```
Somewhat doubt it, but it's a possibility! If you're willing to give it a shot let us know whether it works or not!
```

---
## \#134 Posted by: sgaana Posted at: 2016-06-02T15:29:13.681Z Reads: 282

```
From @trbt555
<img src='http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/9/910191d0025582762512bf7de175a8182d795a77_1_678x500.jpeg'>
```

---
## \#135 Posted by: stealth71 Posted at: 2016-06-07T16:00:51.545Z Reads: 278

```
I made a video on deconstructing the Nyco Kama and hooking it to the VESC: 
https://www.youtube.com/watch?v=MaMVMDDFsi4
```

---
## \#136 Posted by: XIII Posted at: 2016-06-24T10:58:16.733Z Reads: 262

```
Hey guys, It's hard to get a Nyko Kama here in Eu. 

So should this one work aswell ? 
http://de.aliexpress.com/item/For-wii-nintendo-2-4G-Wireless-nunchuck-nunchuk-game-controller-color-box-free-shipping-cost/32667765187.html?spm=2114.010208.3.310.iQg6Ak&ws_ab_test=searchweb201556_0,searchweb201602_2_10037_10017_404_507_10032_10040,searchweb201603_11&btsid=adf6b3b5-de1a-44fd-85ec-8332b23c1700

As long as it's a wii wireless nunchuck it should work right?
```

---
## \#137 Posted by: Jamy Posted at: 2016-06-24T12:18:34.908Z Reads: 260

```
From what I've read in my research only the Nyko Kama really works correctly out of the box (no extra electronics). But for 18$ it's not a big issue if it doesn't work so I'd give it a shot.

Personally I bought a Logic3 wiimote but I'm just waiting on my VESC before I can try that. I'll give an update in a month or so :slight_smile:
```

---
## \#138 Posted by: lox897 Posted at: 2016-06-24T13:25:17.108Z Reads: 255

```
You might be able to put the custom Nunchuck RF pcb into the remote and use the original joystick+battery. @chaka knows a lot about it, maybe he could give some advice here.
```

---
## \#139 Posted by: JLabs Posted at: 2016-07-03T16:09:26.882Z Reads: 250

```
I purchased it from Amazon and it didn't work
```

---
## \#140 Posted by: mostwanted Posted at: 2016-07-06T22:53:19.357Z Reads: 258

```
i dont know . cannot make promises . thanks for the link . i'm now gonna order a few and test it . thanks THIRTEEN !    


XIII = thirteen right ?
```

---
## \#141 Posted by: mostwanted Posted at: 2016-07-06T22:59:15.473Z Reads: 263

```
so many variety of nunchucks . have you tried it yet ?. post a video once if successful .
```

---
## \#142 Posted by: lox897 Posted at: 2016-07-07T01:12:23.834Z Reads: 255

```
Are you 13?
```

---
## \#143 Posted by: XIII Posted at: 2016-07-07T09:19:20.409Z Reads: 268

```
That will stay a mystery ... 

JK
No i'm not, I'm 22. 
I like the XIII tag because it was my favorite comic book when i was young. Shared the TOP 2 with Largo Winch
https://en.wikipedia.org/wiki/XIII_(comics)
```

---
## \#144 Posted by: Pylonflyer Posted at: 2016-07-13T03:56:33.479Z Reads: 258

```
Quick question:  How do you go about re-centering the throttle position on the Nunchuck?  I had programmed mine for an airplane esc over a year ago and needed to calibrate it all the way down to arm (used a rubber band to hold it down and throttle up as normal).  Now I have VESCs and I can't get it to re-calibrate center and/or endpoints.  Tried the hold C button when turning on but not working.  Is there a setting in the GUI for VESC as well?  I think I got it working once but it reset back to arming only at full back-stick.  Thanks!
```

---
## \#145 Posted by: Jamy Posted at: 2016-07-20T18:01:29.949Z Reads: 261

```
So I just got my VESC from Enertion. Connected my [Logic3 Wireless nunchuck](https://www.amazon.co.uk/gp/product/B002ST1CFI) according to the [VESC 4.12 wiring](http://www.electric-skateboard.builders/t/vesc-4-8-4-12-nyko-kama-wiring/1872/1) and it seems to be recognizing it. (Don't have a motor hooked up yet, but the display bar moves!)

Something to bear in mind with that Nunchuck though is that the receiver has incorrectly colored wires, so certainly double/triple check. (In my case black was 5V and red was ground...)

Here's pictures:
<img src="/uploads/db1493/original/2X/4/48826d70837e02299fc7241bc3addb9160481c1b.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/e/e18688c5dc9594f52ab3fbdde1bf84c09870ec09.jpg" width="666" height="500">

I'll post with updates as soon as I can connect my motor, but I first need to find some solder so I can make this connection permanent. (Damn holidays :P )

EDIT: Just checked range, seems to be around 7 m LoS before it starts to act up (not always receive input)
```

---
## \#146 Posted by: Maxid Posted at: 2016-07-20T18:52:37.118Z Reads: 253

```
Please shield those three pins normally used for the receiver - there already was an issue on somebody's board when the pins shorted on the capacitor board.
```

---
## \#147 Posted by: Jamy Posted at: 2016-07-20T18:57:06.404Z Reads: 252

```
Yeah, I read that. That's certainly planned :)
```

---
## \#148 Posted by: lowGuido Posted at: 2016-07-20T23:06:08.147Z Reads: 250

```
red for ground and black for Vcc thats a good one!
nice to know that there is a different brand chuk that works. nyko kamas are getting harder to find.

im also pretty happy that the new VESC's are coming without the sockets which kinda forces people to solder.

(but still with hall socket? what does that tell you? enertion plans a sensored motor?..)
```

---
## \#149 Posted by: Jamy Posted at: 2016-07-21T00:02:51.617Z Reads: 249

```
> im also pretty happy that the new VESC's are coming without the sockets which kinda forces people to solder.

That and the fact that getting those JXK headers is a pain if you want just one. I ended up ordering 20 from Farnell but had to also add in a new soldering iron and stuff to have the minimum amount for my order >_>
```

---
## \#150 Posted by: lowGuido Posted at: 2016-07-21T00:06:49.522Z Reads: 247

```
LOL I ordered 20 of the 4 pin ones for the canbus connector and ended up gluing a couple of 4's together for other connections..
```

---
## \#151 Posted by: awcany Posted at: 2016-07-24T14:20:13.695Z Reads: 254

```
is there any chance that the nunchuck will work with a 3 pin esc like this?
http://sky-vid.com/wp-content/uploads/2016/01/50-PCS-Sale-30-AMP-ESC-30A-SimonK-Firmware-Brushless-ESC-w-3A-5V-UBEC-Quad-2.jpg
```

---
## \#152 Posted by: sgaana Posted at: 2016-07-24T21:34:21.554Z Reads: 244

```
Don't think so. 
Anyone more knowledgeable please comment.
```

---
## \#153 Posted by: cmatson Posted at: 2016-07-24T22:46:29.718Z Reads: 245

```

Some of the nunchuk receivers can connect to a normal PPM input- I believe torqueboards used to sell one (and maybe still does).
```

---
## \#154 Posted by: Bender Posted at: 2016-07-25T03:25:42.937Z Reads: 245

```
@awcany I think it can, it's called a wiiceiver, designed by Austin Davis (if I remember correctly). I don't think DIY sells them anymore.

I have one, pm me if you want it.
From DIY looks like 3 wires
wp-content/uploads/2014/11/wiiceiver-wireless-wii-nunchuck-instructions.jpg
```

---
## \#155 Posted by: awcany Posted at: 2016-07-27T08:55:02.934Z Reads: 231

```
ok thank you :D
```

---
## \#156 Posted by: awcany Posted at: 2016-07-27T08:57:52.457Z Reads: 230

```
i will wait for the parts to arrive in my country and see if it will work or not , for the moment there is no point to ask you for the wiiceiver ,maybe i will not need it but thank you for the offer :D
```

---
## \#157 Posted by: awcany Posted at: 2016-07-27T09:31:19.810Z Reads: 227

```
can u tell me what should i look for if i will buy a ppm input? does it matter the number of channels?
```

---
## \#158 Posted by: cmatson Posted at: 2016-07-27T14:58:58.947Z Reads: 244

```
Channel number doesn't matter, but you make want to solder the nunchuk dongle  onto the receiver. There is a whole thread about nunchuk receiver, and how to wire everything. 

Just use the forum search, and it'll be one of the top suggestions
```

---
## \#159 Posted by: PLEB Posted at: 2016-07-27T22:03:12.785Z Reads: 246

```
Is this the correct Kama? It looks different from the others.

<img src="/uploads/db1493/original/2X/9/9b142559bf43a0745cd002157e50b7cfdc66b408.jpg" width="281" height="500"><img src="/uploads/db1493/original/2X/9/9c80a5fd150bbf9086a3da509c36e9e45e8131f9.jpg" width="281" height="500">
```

---
## \#160 Posted by: DeathCookies Posted at: 2016-07-28T09:28:32.271Z Reads: 239

```
Yes, that is a working Nunchuk for the VESC.
```

---
## \#161 Posted by: awcany Posted at: 2016-07-28T14:05:21.043Z Reads: 239

```
thank you :D
```

---
## \#162 Posted by: kaiser Posted at: 2016-08-03T14:55:17.262Z Reads: 252

```
Anyone there had success whit this wii nunchuck . dont know what type it is ,, but it says MAR105P121306 on the one little chip 

http://store.43oh.com/%20CC2500-2.4Ghz-RF-Transreceiver-Module

I can't tell if it possible to find the RX TX  on this little thing :/ 

<img src="/uploads/db1493/original/2X/1/1073cf45cc1d62491caf338085e4dd0e723ddefb.JPG" width="666" height="500">
```

---
## \#163 Posted by: Sir.Mighty Posted at: 2016-08-03T18:36:39.766Z Reads: 243

```
@kaiser Can you take a picture of the underside of the pcb and the back of the connector? Or you can look at the pinout of the connector and follow the traces yourself:

https://c2.staticflickr.com/8/7263/7085452395_c6897a4f2d_b.jpg
```

---
## \#164 Posted by: kaiser Posted at: 2016-08-03T19:07:47.507Z Reads: 241

```
<img src="/uploads/db1493/original/2X/e/e17f5b9d33cb15ebf0fe6a481203082351f2e612.JPG" width="666" height="500">
```

---
## \#165 Posted by: kaiser Posted at: 2016-08-03T19:16:13.136Z Reads: 230

```
u are my hero if u can pin out RX and TX .. Helped a lot  whit the picture u send ! Much better power going right this time the little blub is much brighter now! when know for sure where + and - is :D
```

---
## \#166 Posted by: kaiser Posted at: 2016-08-03T20:01:47.439Z Reads: 233

```
Hmm i have  just paced pins inside the SDA to TX and SDL to RX And  GND to GND  and 3.3 v to 3.3 v but it dont seem to work :/
```

---
## \#167 Posted by: lowGuido Posted at: 2016-08-03T23:49:42.781Z Reads: 235

```
you may have your TX and RX wrong way around?
```

---
## \#168 Posted by: elkick Posted at: 2016-08-04T06:06:46.642Z Reads: 236

```
Since it's not a Kama Nunchuk I doubt it will work. They are using different protocols.
```

---
## \#169 Posted by: kaiser Posted at: 2016-08-04T15:33:24.209Z Reads: 236

```
Both ways is tried .. A thing so simple is so hard :D i have now orderd the kama wii from eBay ..
```

---
## \#170 Posted by: PLEB Posted at: 2016-09-20T05:00:23.164Z Reads: 196

```
Hey, on a different topic. Does anyone know what the deadband and ERPM settings do in the App > Nunchuck menu in the BLDC? I can't find anything on it. I know the positive and negative time constants are for "smoothening" out the acceleration and breaking, but the other stuff eludes me.
```

---
## \#171 Posted by: Ultimat3ging3r Posted at: 2016-09-23T01:32:58.002Z Reads: 201

```
**So I have an issue and have looked but can't find the answer. I have a white nyko nunchuck and it's wired different from the diagram I've seen across the board

<img src="/uploads/db1493/original/3X/3/5/358c690e000c46456bd3bb2e04ca8b8798d4fea1.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/0/1/0114f594df1fe6175b7329338e46275cc9b725bd.JPG" width="375" height="500">

Wires from top to bottom are Red white blue green brown
Also I just got my vesc in from enertion but is has no jst port for the receiver. Can I just solder straight to the board or should I buy the port?
```

---
## \#172 Posted by: hamminitup Posted at: 2016-09-23T02:17:14.043Z Reads: 192

```
Sorry for no help, but I have the same Nunchuck and receiver. I remember someone posted some diagrams for wiring in a thread I posted a while back, but there hasn't been a definite answer. I hope someone can help. I am going to need to wire mine up soon.
```

---
## \#173 Posted by: trbt555 Posted at: 2016-09-23T09:37:53.972Z Reads: 189

```
Soldering directly to the PCB is safest and most reliable.

There's no guarantee the wire colors correspond to the "original" Nyko receiver. 
The only way to tell for sure is view them as they were connected to the Wii-plug as shown in post 161 in this thread.
```

---
## \#174 Posted by: Ultimat3ging3r Posted at: 2016-09-23T11:15:10.847Z Reads: 190

```
Thanks for the reply guys I ended up finding out how it was connected and just soldered it to the board. Figured I wouldn't use that spot for anything else.
```

---
## \#175 Posted by: Jamy Posted at: 2016-09-23T20:29:43.084Z Reads: 196

```
After having used a nunchuck for about a month I personally would really advise against using them. The connection isn't always stable and it's not super easy to keep the throttle in a stable location.

Better take the extra costs to get a more e-skate specific controller. Just my 2 cents!
```

---
## \#176 Posted by: hamminitup Posted at: 2016-09-24T02:33:20.407Z Reads: 189

```
Do you mind detailing how you connected it? I have the same nunchuck receiver. Perhaps a diagram? Thanks!
```

---
## \#177 Posted by: Ultimat3ging3r Posted at: 2016-09-24T12:20:30.887Z Reads: 202

```
<img src="/uploads/db1493/original/3X/e/e/ee769c21a5b462ef6788b257899204edefe9d523.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/e/2e6ee14fad93e91c7e7e374917023be227adb3a7.JPG" width="375" height="500">

Red-3.3v
Blue-Rx
Green-Tx
Brown-ground

You can find the port name on one side or other of the vesc

Now I don't know if will work for sure. While testing all the lights came on ( the vesc and receiver) but also testing I made a stupid error and fried my vesc. So now I have everything ready to ride and no vesc. So  be careful and make sure everything in connected well befor adding power. Stupid mistake on my part. 

Hope it helps
```

---
## \#178 Posted by: hamminitup Posted at: 2016-09-24T12:43:27.156Z Reads: 195

```
Ouch. Thanks for the info, though! I hope it works out.
```

---
## \#179 Posted by: Thanhnd Posted at: 2016-10-01T13:08:52.175Z Reads: 192

```
Hi builders.

The cruise control feature not work correctly. Please help me by take a look this and let me know what I should do.

https://youtu.be/j95BaCMUvHE
```

---
## \#180 Posted by: Bender Posted at: 2016-10-01T15:15:31.007Z Reads: 194

```
Had the same problem

this fixed it
[http://www.electric-skateboard.builders/t/vesc-nyko-nunchuck-unstable-cruise/1809/9?u=bender](http://www.electric-skateboard.builders/t/vesc-nyko-nunchuck-unstable-cruise/1809/9?u=bender)
```

---
## \#181 Posted by: Thanhnd Posted at: 2016-10-02T05:58:38.384Z Reads: 185

```
Its works. Thank you so much :smiley:
```

---
## \#182 Posted by: Thanhnd Posted at: 2016-10-09T16:06:32.468Z Reads: 184

```
Hi Builders.

Please check out my issues: 
http://www.electric-skateboard.builders/t/vesc-kama-nunchuck-cant-use-break/10866
```

---
## \#183 Posted by: whitepony Posted at: 2016-10-10T05:08:55.408Z Reads: 184

```
[quote="Jamy, post:175, topic:139"]
and it's not super easy to keep the throttle in a stable location.
[/quote]

youre doing it wrong! if you have the kama, its all about the cruise control button. raw throttle is just used to bring you initially up to speed, later small  adjustments to your speed are done with throttle while holding cruise control, which allows small increments from current speed.

Ive never had dropouts btw, for me it was a very reliable remote until I started to work with full carbon enclosures!

for the kama to be truly enjoyable, I advise to fiddle with the pid control parameter unless they have been changed by benjamin vedder by now to something reasonable. check this: http://vedder.se/forums/viewtopic.php?f=6&t=74&p=571#p340
```

---
## \#184 Posted by: stealth71 Posted at: 2016-10-10T14:21:55.011Z Reads: 173

```
I am still using the Nyco Kama and it has been working great.
```

---
## \#185 Posted by: Bataleon Posted at: 2016-10-15T16:10:43.306Z Reads: 172

```
Has anybody had any luck with other brands of wireless nunchucks, or only the Nyko Kama?
```

---
## \#186 Posted by: rtasca Posted at: 2016-11-03T16:47:43.297Z Reads: 175

```
<img src="/uploads/db1493/original/3X/b/9/b9be0c97555ff3059f3b153dd9ce7ed4db98ecec.png" width="245" height="478">

<img src="/uploads/db1493/original/3X/f/4/f4db65eb0de834c745647e749971742827e9fc94.png" width="469" height="373">

has anyone tried this one? certainly a cheap copy! what are the odds ??
```

---
## \#187 Posted by: lox897 Posted at: 2016-11-03T19:19:31.341Z Reads: 158

```
The nyko kama is the one everyone uses
```

---
## \#188 Posted by: XIII Posted at: 2016-11-03T19:32:08.321Z Reads: 160

```
could everyone who has a reliable Nyko kama, take a picture of the receiver and your vesc? 

If I shield my vesc with alumium , I have 0 dropouts. So now i'm curious where you placed your receivers to have no issues with the EMI of the vesc.
```

---
## \#189 Posted by: AbdeTy Posted at: 2016-11-04T23:30:34.173Z Reads: 155

```
i just got that one as well , is it working fine for you ?
```

---
## \#190 Posted by: rtasca Posted at: 2016-11-05T00:19:32.205Z Reads: 156

```
I haven't bought it yet. copied the picture from my local online market website. I'm sure this is not an original deal so I wanted to be sure before I bought it.
```

---
## \#191 Posted by: AbdeTy Posted at: 2016-11-05T00:54:35.822Z Reads: 164

```
well , i already have it but haven't tried it yet , it seems like an original Nyko product not a copy but i guess either it is a different version than the one everyone uses i dont know if its newer or older , the packaging shows 2008 also i opened the receiver and it has way more chips and electronics than the normal ones everyone has here i dont know if thats good or bad lol if you are interested i can take some pictures for you
```

---
## \#192 Posted by: trbt555 Posted at: 2016-11-08T12:54:07.121Z Reads: 170

```
[quote="XIII, post:188, topic:139"]
could everyone who has a reliable Nyko kama, take a picture of the receiver and your vesc?
[/quote]


I put the receiver as far as I could from the VESCS.
Zero dropouts for past 10 months and counting.
<img src="/uploads/db1493/original/3X/4/b/4b01a83dd816f211d40ce75f96b319812884ae06.jpg" width="666" height="500">
```

---
## \#193 Posted by: XIII Posted at: 2016-11-08T14:37:39.823Z Reads: 164

```
I increased length aswell...  No solution for dropouts.  Since I use the spacecell the wii dongle is still really close to my battery cells.  
Maybe high current is an issue. 
Going to solder some capacitors now to the vcc and gnd of the reciever.  Maybe this helps in some sort of way.  

I guess wrapping the reciever in aluminium foil won't be good for the bluetooth signal..  ☺️
```

---
## \#194 Posted by: darkkevind Posted at: 2016-11-16T21:13:11.411Z Reads: 151

```
Hey guys, does anyone know why you can't wire up the nyco to your normal receiver? I'm thinking that you just need the RX wired up if you just want accel. brake. with no cruise control etc?
```

---
## \#195 Posted by: trbt555 Posted at: 2016-11-17T08:03:28.113Z Reads: 162

```
[quote="darkkevind, post:194, topic:139, full:true"]
Hey guys, does anyone know why you can't wire up the nyco to your normal receiver? I'm thinking that you just need the RX wired up if you just want accel. brake. with no cruise control etc?
[/quote]


What normal receiver ?
```

---
## \#196 Posted by: Maxid Posted at: 2016-11-17T08:47:01.613Z Reads: 162

```
I guess he means a 2.4Ghz receiver. Probably one of those noobs that has no idea how the Nunchuck works and thinks it is the same as a GT2B.
```

---
## \#197 Posted by: darkkevind Posted at: 2016-11-17T09:02:53.896Z Reads: 158

```
Sorry, I meant to your ESC...
```

---
## \#198 Posted by: Maxid Posted at: 2016-11-17T10:19:32.082Z Reads: 167

```
The Nyko provides a digital and not just a PWM signal.
to do what you want you need either a VESC or this: http://austindavid.com/jm3/index.php/hardware/3-wiiceiver
```

---
## \#199 Posted by: rtasca Posted at: 2016-11-18T23:08:43.987Z Reads: 165

```
did u figure out the wiring on this one?
I seem to have the same receiver here.

edit: nevermind, I found it above, seems the same as I figured out. Now... mine wont turn on. no light. wired it back to test it on a real WII and the light wont come on... I guess this is some kind of sign, Stick with R/C remotes.
```

---
## \#200 Posted by: Ultimat3ging3r Posted at: 2016-11-19T18:10:18.380Z Reads: 159

```
That's what I ended up doing. Got a hobby king remote. Now I'm still waiting on my enertion remote to come in but who knows when that will ever happen.
```

---
## \#201 Posted by: ElectricCommuter Posted at: 2016-11-19T21:04:54.772Z Reads: 163

```
I'm using a wii nunchuck while I'm waiting for my other remote to ship. For some reason if it disconnects the motor goes full throttle I tried searching the forums but couldn't find anything is it just a setting in bldc tool ?
```

---
## \#202 Posted by: Cramps Posted at: 2016-11-19T23:25:34.728Z Reads: 160

```
I'm planning on using an RC remote to begin with just to get up and running, after that I will probably purchase two arduino banks and a receiver/transmitter for each. I'll then empty most of the components from a wii nunchuck and use that as the body of the remote.
```

---
## \#203 Posted by: warpboard Posted at: 2016-11-20T15:41:53.290Z Reads: 154

```
Has anyone found a fix to the Nyko Kama not activating the motors?

The receiver light turns on and nyko kama remote connects and receives signals as when i push a button on the remote the receiver light flashes on and off, but does not spin the motors.

Using BLDC I can spin either motor just not using the remote.
```

---
## \#204 Posted by: rtasca Posted at: 2016-11-23T00:14:19.517Z Reads: 147

```
thats exacltly what I decided to do today. I even have one 3.3 and one 5v pro minis left over. going to buy 2 BT modules.
```

---
## \#205 Posted by: Mitch Posted at: 2016-11-29T03:08:01.573Z Reads: 149

```
Anyone based in Sydney and willing to help with finishing my build thats been put on hold for a few months now! Just need to get the nyko kama connected.... willing to pay for your services.
```

---
## \#206 Posted by: OleksiiF Posted at: 2017-02-28T16:48:13.581Z Reads: 144

```
Hi! 
i have a problem, looks like when i push "c" button, i have something wrong and instead on holding speed, i have some sort of interference. when motor spins, and i press"c" button, motor makes horrible noise (like it tries to do couple commands in same time)

if i press"c"  button from stand still, motor starts to spinning with some constant speed, and if i try to change it with trigger motor makes horrible noise (like it tries to do couple commands in same time) again

here is connection. I double checked wire colours. i have 7pin port, instead if 6 pin.
Where am i making a mistake? 

<img src="/uploads/db1493/original/3X/a/f/afc936eab9e377861f0dba4cba348cc7684d6606.jpg" width="666" height="500">
```

---
## \#207 Posted by: UniqueSnowflakeN27 Posted at: 2017-02-28T19:34:10.319Z Reads: 140

```
What VESC version is that? Which software version?

Here's a pic of mine. I followed this guide and it worked perfectly fine.

<img src="/uploads/db1493/original/3X/c/7/c7a1e2fd410f34670ee35dd068c274a7c503d7ac.JPG" width="690" height="459">
```

---
## \#209 Posted by: OleksiiF Posted at: 2017-02-28T20:57:17.193Z Reads: 139

```
4.12
i use Extended BLDC-TOOL with Watt Control Mode

could i damage a receiver? 
i soldered everything, tested it, everything worked fine,
than i hot-glued it, 
got a problem,
melted glue
took picture<img src="/uploads/db1493/original/3X/3/1/3194c0ee9e5fd4a0a6dfbed21ca154c170750140.jpg" width="674" height="500">
```

---
## \#210 Posted by: Montiey Posted at: 2017-02-28T21:22:15.192Z Reads: 136

```
How is it wired on the VESC side? Also, just be sure that there are no bridged joins on the receiver (including the rest of the circuitry). Other than that, your problem is most likely due to EMF interference from the VESC / motor, or wiring.
```

---
## \#211 Posted by: OleksiiF Posted at: 2017-02-28T21:29:17.971Z Reads: 135

```
the problem is, that in some point it worked fine. and im doing everything in the same way.

any ideas how to fix this?
there is no bridges on receiver,
```

---
## \#212 Posted by: Montiey Posted at: 2017-02-28T22:07:41.123Z Reads: 132

```
Hmm.. Perhaps you changed a setting in BLDC tool? Maybe disabled Nunchuk control? Or possibly the remote or the receiver is damaged. If you're confident that the receiver is good, and it's connected to the vesc good, then I would start looking at your settings, or the remote.
```

---
## \#213 Posted by: OleksiiF Posted at: 2017-02-28T22:12:15.471Z Reads: 129

```
Ill start with the settings, thanks.
Receiver looks solid, no visual defects
```

---
## \#214 Posted by: Montiey Posted at: 2017-03-01T00:07:16.533Z Reads: 132

```
It could be the batteries in the remote Are they fresh? Swap them out for AAA's that are at least 1.4v, just to make sure we aren't missing anything here.
```

---
## \#215 Posted by: OleksiiF Posted at: 2017-03-01T11:34:38.941Z Reads: 131

```
Remote is brand new, batteries too (stock). Have it for 2 weeks, made only tests
```

---
## \#216 Posted by: OleksiiF Posted at: 2017-03-01T11:37:35.542Z Reads: 136

```
Well, i reinstalled firmware, applied settings, and problem stayed the same(

its 100% hardware problem.
its impossible that it shows "over_voltage" error when gt2b and nyko receiver are connected in the same time with no reason 

problem ether  in receiver or in vesc. but how to fond out where exactly? the good thing that gt2b works perfrctly
```

---
## \#217 Posted by: Montiey Posted at: 2017-03-01T19:18:45.759Z Reads: 133

```
In BLDC Tool, go to the "Terminal" tab, then type "faults" and hit enter. This will list all the faults… What shows up? 

And just to clarify, you _have_ tested the GT2B and the Kyko with the fresh firmware? What hardware and software versions are you running now?
```

---
## \#218 Posted by: brun Posted at: 2017-03-13T04:32:32.154Z Reads: 140

```
I just finished my prototype radio setup using NRF24L01 for wireless but connected to the VESC via an Arduino Pro Micro that is emulating the Nunchuck I2C slave communication protocol.  So the VESC will think it's taking to a Nunchuck so the Vesc Nunchuck app should work, but with a better radio that isn't susceptible to EM interference (assuming that is the problem and not power brown out)  Bench testing this week.  

Although the nunchuck has a serious cut-out flaw, but the current VESC Nunchuck "app" is miles ahead of PPM app in terms of smooth power and breaking.  I've use both ways with every BLDC setup imaginable and could not get PPM to come close to the Nunchuck which has Ramping Time constant control.  I asked B Vedder why he didn't include it for PPM and he said he just never got around to it because he uses the Nunchuck mostly.

I heard that the VESC 6.0 Firmware (compatible with VESC 4.xx) is coming out sometime soon and will include the ramping setting for PPM as well.  Long overdue in my opinion.
```

---
## \#219 Posted by: jbruce Posted at: 2017-03-13T06:34:36.169Z Reads: 142

```
What you're doing is very cool! Is there a possibility of you selling these?
```

---
## \#220 Posted by: brun Posted at: 2017-03-13T14:32:20.583Z Reads: 142

```
Well I have to make it work first.  Probably not, but I'll publishing everything.  VESC 6.0 firmware will solve this problem IMO...and everyone using a standard remote will be able to use ramping.
```

---
## \#221 Posted by: jbruce Posted at: 2017-03-13T15:58:49.401Z Reads: 142

```
you're right but cruise control and to be able to change direction with the remote is pretty nice.
```

---
## \#222 Posted by: Iam319 Posted at: 2017-04-30T15:27:04.881Z Reads: 136

```
What would a GT2B do? Sorry if that's a dumb question. @Moja
```

---
## \#224 Posted by: Boca Posted at: 2017-07-07T03:17:26.826Z Reads: 111

```
Is there a way to connect the dual VESC by connecting Rx and Tx of master and Slave VESC?
```

---
## \#226 Posted by: Jamy Posted at: 2017-08-14T12:51:58.987Z Reads: 94

```
Make sure your solder connections are good?
```

---
## \#227 Posted by: Maxid Posted at: 2017-08-14T12:57:41.690Z Reads: 96

```
The logic3 is not actually working the way it should is it? So far AFAIK the only nunchuck that works is the Nyko
```

---
## \#228 Posted by: Jamy Posted at: 2017-08-14T12:58:44.137Z Reads: 98

```
I had a logic 3 on my original board and it worked fine. Just doesn't have the range necessary which makes it drop out often. (At least mine did)
```

---
## \#229 Posted by: Maxid Posted at: 2017-08-14T13:00:31.789Z Reads: 92

```
And with not enough range you mean you standing on top of the board was already too far away? Otherwise this would be amazing news - the logic3 is much easier to get than a nyko

Edit: well I checked and in Europe it is actually not easier to get :cry:
```

---
## \#230 Posted by: Jamy Posted at: 2017-08-14T13:04:58.222Z Reads: 97

```
It dropped out every so often, and I had it so it would break slowly if it loses connection. I had to put that connection timeout to 3 seconds (So it would keep the same accel value for 3 seconds before starting to break) which was scary. 

So a few weeks later I got [one of these](https://www.aliexpress.com/item/Wholesale-New-arrival-2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32678995218.html) (from a group buy, not necessarily this manufacturer. And I've felt much safer with it than the nunchuck, so I chucked the nunchuck in the bin of chuckable items.
```

---
## \#231 Posted by: jabot88 Posted at: 2017-08-27T15:52:08.629Z Reads: 101

```
Hi to everyone!
I am new to this forum and to electric skateboards.
I decided months ago to build a electric skateboard. I ordered the pieces and now I have all of them at home.
I have bought a VESC and a wireless nunchuck controller, but when I opened my VESC I discovered that it's different from the ones I see here, so I don't know how to connect it.
The wireless controller board it's clearly marked, so I need to know the 6 pin layout of my VESC board.

Thanks in advance

Here are some pics of the VESC and the controller:
<img src="/uploads/db1493/original/3X/9/a/9aff6cfd4060cb1ff81aae9706e3b46aeb2a1d26.jpg" width="499" height="499">
```

---
## \#232 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-27T16:17:33.935Z Reads: 98

```

@jabot88  Looks just like mine, albeit more chinese. [Here's the video I followed to get it hooked up.](https://www.youtube.com/watch?v=MaMVMDDFsi4) He's got some good links as well to this forum where Onloop have a guide as well.
```

---
## \#233 Posted by: Maxid Posted at: 2017-08-27T17:56:27.822Z Reads: 99

```
"Any" wireless nunchuck will not work - you need the Nyko kama or get a different remote
```

---
## \#234 Posted by: Jan2000 Posted at: 2017-08-30T01:45:33.780Z Reads: 100

```
Hey everyone,
i have the same kama reciver, like in post 170 and connected it like in post 176 but the controller is not connecting. If I connect the reciver to a normal Wii-Remote it works fine. Anyone has an idea what i could do?<img src="/uploads/db1493/original/3X/a/9/a9a94a03f052c62ee3df94e6641364150f02bd89.jpg" width="500" height="500">
```

---
## \#235 Posted by: machadolab Posted at: 2017-09-12T17:26:01.898Z Reads: 102

```
Hey all, I've been working on a solution to allow nunchuck to act as a simple R/C receiver for my electric skateboard. If all goes well, I will offer it for sale soon. But in my journey, I have bought 7 nunchucks, and only 1 has worked! I figured I would share my experience here in case it helps someone else on a similar path:

<img src="/uploads/db1493/original/3X/c/2/c25ae44a5325000308e71df45312aadffe18ed84.jpg" width="506" height="500">

Nunchucks that HAVE NOT WORKED:

* amazon.com/gp/product/B0015FRA0W - Branded as Intec
* amazon.com/gp/product/B001C7B8Y2 - Branded as Yobo
* amazon.com/gp/product/B002TSL7XK (not pictured) - No name, didn't hold a charge, thrown away
* amazon.com/gp/product/B0012R58LG - White Branded Nyko Kama, Item number on receiver: 87027-E14 - Have both ones sold in the 'slim' vertical package as well as the 'wide' packaging. And both 'smooth' ones (see image above) and the white one with 'ridges', similar to the black kama.

(New forum user, so I wasnt able to use actual URL links above :/ )

The ONLY wireless nunchuck's that has worked is the Nyko Kama BLACK - sold as item 87111.
 http://www.ebay.com/itm/Nyko-Wireless-KAMA-For-Nintendo-Wii-Black-8-/382171140439


For what its worth, I am a software engineer, and I have played around with no less than 4 different "sample codes" and arduino libraries. I have implemented a couple different 'handshake' routines, tried with and without encryption and scoured wiibrew.org for detailed protocol documentation. Its unclear why only the black nyko kama works, but that's what I have found. My guess is earlier versions of the white nyko kamas have the same internals as the black kamas, but more recent white kamas have had some change made to them. Just a theory, and would explain why there are posts online in arduino forums about how they have their white nyko kama working with their projects.

Hope this helps.

-Mike
```

---
## \#236 Posted by: skslingo21 Posted at: 2017-09-21T00:55:58.982Z Reads: 98

```
My Nyko kama worked fine for my VESC, but when stuffed back in the noisy (RF interference) Speed Controller box, it would hold commands, and disengage randomly. A perfect storm for an E-board.
It never made it off the stand.
 My next build will have to make use of the kama I have. It WILL be SOLDERED to the Master vesc, leads shielded, and large ferrite ring in place. Mounted as far away from any source of RF interference as well.  :confounded:
The range in my manual stated <1meter?
here it is next to my trusty 2.4 handheld radio. Its been operated around alot of other RC radios, and various small model radios without any interference mishaps, I cant say its power is low enough to be legal in all countries though..
<img src="/uploads/db1493/original/3X/8/8/88317f0a2d0e3f5a765b69f3395c32f6b54509ac.jpg" width="666" height="500">
```

---
## \#237 Posted by: lucasbuckleynz Posted at: 2017-10-21T08:44:32.132Z Reads: 86

```
hi, 
i have bought this same nunchuck but it doesn't seem to work, it is the third wii nunchuck we have bought the one you suggested, another nonbranded one and a wired nunchuck. should we expect at least the wired one to work? 
i have a 4.12 VESC board with 2.16 software. do you have any idea why it wouldnt work i believe the pins we have connected to are correct, is there anything you did to make it work?
thanks lucas
```

---
## \#238 Posted by: raven Posted at: 2017-10-30T14:02:45.324Z Reads: 83

```
I have this one<img src="/uploads/db1493/original/3X/1/2/1219220edd19718460297e0dc7583c858d5fed3e.jpeg" width="375" height="500">
```

---
## \#239 Posted by: raven Posted at: 2017-10-30T14:05:28.111Z Reads: 81

```
Pull the wires out and solder or use a female pin to your vesc. Am waiting for XT90 connector and see what happens
```

---
## \#240 Posted by: raven Posted at: 2017-10-30T14:08:07.559Z Reads: 88

```
<img src="/uploads/db1493/original/3X/6/e/6eded6cc00aab6a6e7592268224b630a21d9ba45.jpg" width="375" height="500">
Will hot glue later. Still need to see if it works
```

---
## \#241 Posted by: linkedtim Posted at: 2017-10-30T18:23:58.006Z Reads: 89

```
So this tutorial 'worked' for me with this controller:
https://www.amazon.com/gp/product/B0047SFGDW/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1
The VESC I own is:
collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller
Unfortunately this is past tense because the connection was cutting out, which I attributed to not having soldered the connections. I put about 10 miles on the board before this started happening so wen't back to solder everything and suddenly I wasn't able to get the joystick or the C/Z button to react. The receiver lights up and connects, but I'm not getting any wheels turning when using it. When connected via BLDC, I have no issue using the keyboard to turn the wheels. This was happening with the I2C ports so I went back to square 1 with the wiimote I originally had working via: 
https://github.com/the-raspberry-pi-guy/skateboard
but now that setup isn't turning the wheels either using the servo connections. 
Could I have fried something on the board that would stop any signal reception?
```

---
## \#242 Posted by: raven Posted at: 2017-11-12T04:10:57.065Z Reads: 77

```
I have this problem with firmware and the dongle that I rewired seems to be working. Will have to wait and find out.
```

---
## \#243 Posted by: linkedtim Posted at: 2017-11-12T23:47:30.373Z Reads: 74

```
Hi Raven, so you think its a firmware related issue? Do you have the same VESC? What alteration did you make that seems to be working?
```

---
## \#244 Posted by: raven Posted at: 2017-11-13T00:34:12.799Z Reads: 74

```
It’s fixed now after some tweaking. Don’t think hall sensor fail really matter.
```

---
## \#245 Posted by: raven Posted at: 2017-11-13T00:39:49.286Z Reads: 76

```
Loose connection is what I suspect. I just set mine up. Check battery connection if soldered properly using a multimeter. Check battery is good. Vesc should come with firmware already. Go back to BLDC and detect motor again.
```

---
## \#246 Posted by: Flapjackz Posted at: 2018-01-08T03:29:15.345Z Reads: 66

```
Hey guys, I would like to share my solution. After reading for 2 days and trying everything suggested from changing settings to measuring voltage on the 3.3v pin on the vesc I decided that is was probably to close to the esc (hot glued to the top) I soldered in 9 inches of wire and moved as far away from the vesc and to the edge of my board and it now runs smooth as silk without any cut outs whatsoever.
```

---
## \#247 Posted by: Donson Posted at: 2018-01-26T23:35:38.307Z Reads: 67

```
it dosnt work......in german caled "zittern" 
my nunchuck is diferent

can somone help me?![20171220_234553|281x499](upload://augTa0LLpP5OWDjcfD0HKUJ1uF7.jpg)
```

---
## \#248 Posted by: banjaxxed Posted at: 2018-01-28T22:54:32.564Z Reads: 69

```
I blew a receiver just like that, it's a short waiting to happen or already happened which would explain no bueno
```

---
## \#249 Posted by: MotorMouth Posted at: 2018-05-16T19:55:39.565Z Reads: 54

```
Hey, this is quite cool; one thing that might make it easier:
https://www.adafruit.com/product/345
This breaks out the data, clock, power and ground pins directly from the Nunchuk plug so you don't have to do any disassembling or hot-gluing.
```

---
