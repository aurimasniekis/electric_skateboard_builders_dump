# UART Splitter for VESC Based ESCs

### Replies: 71 Views: 2434

## \#1 Posted by: Ricco Posted at: 2019-05-21T18:59:31.478Z Reads: 313

```
Hey guys,

By request of @bsancken and others on this fourm, I've created a UART Splitter for connecting multiple add-on devices to VESC based motor controllers.

---

**TYPES:**

There are two types currenlty in the works. The two way splitter allows 2 devices to share a single UART port of a VESC based ESC. LEDs on the back of the splitter indicate when communication is taking place on any of the 3 UART ports.

<div align=center>

![UART%20Splitter%201-2%20All%20Views|654x500](upload://pmNEDYYc4X5I2WFeBUWkWyrYFAv.jpeg)

**1:2 UART Splitter**
</div>

[spoiler].[/spoiler]

The three way splitter allows 3 devices to share a single UART port of a VESC based ESC. LEDs on the top of the splitter indicate when communication is taking place on any of the 4 UART ports.
<div align=center>

![UART Splitter 1-3 All Views.JPG](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/9/594446b6a74b5d225e4594a38c7ea5e23c7e187d.jpeg)

**1:3 UART Splitter**
</div>

---

**DEMOS:**

<div align=center>

![](https://media.giphy.com/media/idLNFICM8hcP3fvBFG/giphy.gif)
![](https://media.giphy.com/media/S663OrysTpIcYJhROo/giphy.gif)

![](https://media.giphy.com/media/fAnLgVopn3K1A8LG4E/giphy.gif)
</div>

---

**TESTED DEVICES AND FEATURES:**

ESCs:

* FOCbox  (FW v3.38 @ 115200 baud)

ADD-ONs:

* [Metr Pro Bluetooth Module](https://www.electric-skateboard.builders/t/metr-pro-next-gen-bluetooth-module/57780/) 
  * Basic Telemetry
* [DAVEga Display](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509/)
  * Basic Telemetry
  * ESC Motor Settings Info
* [TelTail Lighting System](https://www.electric-skateboard.builders/t/beta-testers-needed-teltail-lights-ttl-interactive-eskate-lighting-system/86912/)
  * Motor Data Plotting
  * Reactive Tail Light

There is plenty more testing that needs to be performed before I start selling any but I wanted to start a thread now to share the project with you guys and get your input on a some key aspects of the final product.
```

---
## \#2 Posted by: Ricco Posted at: 2019-05-21T19:01:54.868Z Reads: 263

```
The next device I will be testing with is a Firefly remote. That will exhaust all of the add-on that I own so any other devices will need to be tested by others when I begin beta testing.
```

---
## \#3 Posted by: janpom Posted at: 2019-05-21T19:14:39.024Z Reads: 250

```
Nice! I volunteer for beta testing. I recently found out that with my dual ESCapes, if I connect Metr to the master and DAVEga to the slave, it doesn't work very well. They seem to somehow interfere with each other. I might very well make a good use of the splitter. I'm happy to pay for the tested sample and/or do the assembly if needed.
```

---
## \#4 Posted by: Wisp Posted at: 2019-05-21T19:17:40.145Z Reads: 238

```
Keeping an eye on this as well! This really helps people with single motor setup :slight_smile:
```

---
## \#5 Posted by: mishrasubhransu Posted at: 2019-05-21T20:08:43.848Z Reads: 220

```
Nice! Are all functions of metr pro retained? Like CAN forwarding TCP/IP etc?
```

---
## \#6 Posted by: Kug3lis Posted at: 2019-05-21T21:31:20.144Z Reads: 208

```
Are you properly buffering packets and responding in between devices or just split uart (same lines to two different ports) into two devices? Because if you split in two ways I am interested how everything works without collision detection :)

I have already worked on splitting vesc to be controlled by more than one device but I have done that on nodejs level so not much help for embedded but its doable in arduino level too you just need 3 uarts :D

https://i.gyazo.com/da6d886130ee970a5cbab53aa17445f9.mp4

All the code is here:

https://github.com/mark48evo
```

---
## \#7 Posted by: pookybear Posted at: 2019-05-22T00:02:37.196Z Reads: 175

```
Subscribed.
```

---
## \#8 Posted by: Ricco Posted at: 2019-05-22T04:05:41.680Z Reads: 179

```
[quote="janpom, post:6632, topic:63248"]
I wonder how well it works with Metr’s TCP/IP bridging.
[/quote]

[quote="mishrasubhransu, post:5, topic:94552"]
Are all functions of metr pro retained? Like CAN forwarding TCP/IP etc?
[/quote]

So far I've only tested the most basic functionality of the Metro Pro module. The TCP/IP bridge is a great point to bring up and I will try my best to get it working as well. I don't believe it should be too hard but we'll see as I have no experience with it :P I dont have a setup to test the CAN forwarding but since that is one of the common commands in the VESC UART communication I believe it should work. That would be a good one to have a beta tester try out.

@janpom Consider your spot reserved :P maybe the interference issue your faced with is due to CAN forwarding. If you turn that off in the Metr app does it start working well?

@Kug3lis, I do buffer packets and act as a middle man :slight_smile:
```

---
## \#9 Posted by: Ricco Posted at: 2019-05-22T04:11:39.230Z Reads: 165

```
I am also considering making a 3 way splitter version since I would like to connect up a DAVEga, TTL system, and a Firefly remote in my board. Would enough people be interested in a three way splitter for me to make some up? The two way splitter could be stacked up to get three devices connected but then the propagation delay of messages from the furthest removed devices may cause issues.
```

---
## \#10 Posted by: bsancken Posted at: 2019-05-22T06:03:02.415Z Reads: 167

```
My Ideal use case would be your proposed 3x setup with a Feather based remote instead of firefly! I'm willing to do assembly also if needed, working on another project for a car that has me doing smd level soldering. Count me in for beta testing!
```

---
## \#11 Posted by: sami Posted at: 2019-05-22T06:20:44.892Z Reads: 158

```
Very nice project for the single drive guys like me with a firefly and wanting to have metr app as well... Following
```

---
## \#12 Posted by: rey8801 Posted at: 2019-05-22T06:27:25.529Z Reads: 154

```
Really nice! I tought it won't be possible. Great idea!
```

---
## \#13 Posted by: Ricco Posted at: 2019-05-22T16:01:59.594Z Reads: 157

```
Ok, I'll make some 3 way splitters and test those out soon. What are your thoughts on the form factor of the 3 way splitter? There are a few options I can think of:
1. I can lay it out in a similar way to the 2 way splitter and just put 2 device connectors next to each other on one side of the board, but that would make it pretty wide and board space wouldnt be used efficiently.
2. I can put one connector on each end of each side. This would mean one of the devices would plug in on the same side as the ESC, possibly making it less ideal for positioning devices in a your enclosure. This option would be smaller than the first and would probably look the cleanest, but I dont think it would be the most efficient use of board space still.
3. I can put 3 connectors on one side of the board, but instead of placing the 2 device connectors next to each other, the connectors would be placed facing out 3 different edges of the board. This design would be pretty awkward to place inside a build since one device would plug in at 90deg for the others but it would probably be the most efficient in terms of board space. 

@sami, @rey8801, @pookybear, @Wisp, Thanks for the support! :blush:
```

---
## \#14 Posted by: Ricco Posted at: 2019-05-22T16:25:33.443Z Reads: 147

```
One more thing I need people's input on is what I should do about the fact that VESC 6 based ESCs have the TX and RX pins swapped relative to v4.12 HW based ESCs. I am going to try implementing automatic detection and configuration of these pins on the software, but in the case that I cannot, what should I do? Should I provide a dip switch that can be used to swap the TX and RX pins? Or is there another method you would like me to use that is better?
```

---
## \#15 Posted by: rey8801 Posted at: 2019-05-22T16:32:41.775Z Reads: 143

```
Why no just leave it as it is and then if someone has the pins reverse it just reverse them on the jst or whatever connector they use. For metr doesn't Metter since it recognizes TX and RX automatically.

For the other question I think the solutions I see are like your 3rd one and maybe another idea is place one pin connection on the other side. So for instance the one from the vesc on one side, the flip the pcb and split it in 2 parralle UART ports.
```

---
## \#16 Posted by: Ricco Posted at: 2019-05-22T16:43:16.695Z Reads: 141

```
That is definitely an option, I am just thinking of how to make it as user friendly as possible. THe dip switch option would be a little easier than swapping the pins in the JST connector, but implementing the auto detection like Metr is definitely ideal.

For the layout, I believe what you are describing is what I am doing with the 2 way splitter right now. I need to post a render of the board from fusion but, the tool has a bug and isn't rendering the PCB correctly. I'm waiting on autodesk to fix the bug :disappointed: I'll have to draw my ideas out to make them clearer.
```

---
## \#17 Posted by: Vanarian Posted at: 2019-05-22T16:51:41.428Z Reads: 135

```
Didn't know this was an issue before and I might actually need one too I think ! Nice, keep up the good work.
```

---
## \#18 Posted by: pookybear Posted at: 2019-05-22T16:56:14.299Z Reads: 133

```
It's very easy to switch pins around. Running vesc6 here. Either way we can make it work.

Thank you for doing this.
```

---
## \#19 Posted by: rey8801 Posted at: 2019-05-22T17:13:38.806Z Reads: 135

```
Just out of curiosity do you think this will work with like metr and firefly remote on the same UART? I though they could not work together since both are sending and receiving info at the same time
```

---
## \#20 Posted by: PickSix24 Posted at: 2019-05-23T05:28:46.153Z Reads: 133

```
I’d be interested in a three way splitter
```

---
## \#21 Posted by: Kug3lis Posted at: 2019-05-23T10:57:22.298Z Reads: 127

```
It is software (packet) level splitting, aka when one device sends a packet it will send to vesc receive response and send it back to that device if at that moment another device sent a packet it will be delayed until previous device gets finished and etc :) Because of speeds there shouldn't be much lags

This is kinda like your home network switch or router or etc works :)
```

---
## \#22 Posted by: rey8801 Posted at: 2019-05-23T12:28:51.783Z Reads: 120

```
This a game changer! So if I split the JST connected to the UART port in 2. I can connect both the devices. At the end a millsec delay in the telemetry won't change the world.
```

---
## \#23 Posted by: Kug3lis Posted at: 2019-05-23T12:32:31.266Z Reads: 124

```
No no... You need some kind of device which would run logic in front of devices which would decide who receives what
```

---
## \#24 Posted by: rey8801 Posted at: 2019-05-23T12:33:31.403Z Reads: 122

```
Ah ok missed that point. My bad :sweat_smile: It makes sense.
```

---
## \#25 Posted by: Ricco Posted at: 2019-05-23T16:02:15.558Z Reads: 121

```
@PickSix24 What are your thoughts on the layout options of the 3 way splitter I described above?

@Kug3lis thanks for giving the clear and accurate explanation of what the device is doing :slight_smile:
```

---
## \#26 Posted by: Ricco Posted at: 2019-05-23T16:04:54.143Z Reads: 124

```
With each of the splitters I plan to include a 7 pin JST female to female cable for connecting to an ESC. Should this cable be 2 or 6 inches?

[poll type=regular results=always public=true]
* 2 inches
* 6 inches
[/poll]
```

---
## \#27 Posted by: PickSix24 Posted at: 2019-05-23T18:09:36.024Z Reads: 120

```
I think layout option 2 is the best. For me space is always the issue so whatever makes it the most compact.
```

---
## \#28 Posted by: Ricco Posted at: 2019-05-24T03:45:24.736Z Reads: 120

```
Ya, thats what I am leaning towards as well. It's not the most compact it could get in terms of device size, but the cables would sit nicely in a build which is probably the most important when trying to cram everything in.
```

---
## \#29 Posted by: Ricco Posted at: 2019-05-29T13:38:15.489Z Reads: 113

```
I ordered the v2 PCBs for the 2 way splitter and the v1 PCBs for the 3 way splitter last night. I should be recieving them mid next week. It will likely take me a week or two to solder them up and test them. Once I am happy with the results, I will begin beta testing. I currently have 5 people waiting to become beta testers. I think I will do between 10 and 15 testers max.

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-2/88821/1319?u=ricco
```

---
## \#30 Posted by: Wisp Posted at: 2019-05-30T07:29:36.691Z Reads: 102

```
Damm, looks good! Nice and small.
You can put me up for testing as well if you want [EU]
```

---
## \#31 Posted by: bsancken Posted at: 2019-05-30T15:03:19.838Z Reads: 99

```
@Wisp I clicked on the notification for this thread and read your name as part of the title and thought oh cool! He named the project something, thats a cool name! The Wisp UART splitter lolol
```

---
## \#32 Posted by: Ricco Posted at: 2019-05-30T16:34:28.445Z Reads: 100

```
@Wisp Thank you. I've added you to the list :slight_smile:

@bsancken Haha nope still just plain old UART Splitter. Name suggestions are welcome as I have no ideas for this :stuck_out_tongue:
```

---
## \#33 Posted by: Ricco Posted at: 2019-06-19T12:52:40.435Z Reads: 88

```
As a quick update, I will likely begin shipping out units for beta testing in the first week of July.
```

---
## \#34 Posted by: Ricco Posted at: 2019-07-02T17:52:31.432Z Reads: 86

```
Unfortunately, due to a family emergency this last weekend, I was not able to complete the updates to the UART Splitter FW in the time frame I wanted. I was going to finished the updates and start shipping units before I leave for vacation tomorrow, but I will not be able to now. I will be back next Tuesday (7/9), will finish up the FW, and will begin shipping the beta kits shortly after.
```

---
## \#35 Posted by: Wisp Posted at: 2019-07-03T05:38:28.946Z Reads: 84

```
No worries! It's still a hobby ;)
```

---
## \#36 Posted by: StickyBlue Posted at: 2019-07-04T12:41:08.506Z Reads: 80

```
Also keen for a 1:3 :blush:
```

---
## \#37 Posted by: xsynatic Posted at: 2019-07-04T13:00:40.225Z Reads: 81

```
Did i miss the Option to be a Beta tester? ^^
```

---
## \#38 Posted by: Ricco Posted at: 2019-07-05T04:24:09.289Z Reads: 81

```
Nope, not at all. I'll put you and @StickyBlue down to be contacted when I start shipping beta kits next week :)
```

---
## \#39 Posted by: Ricco Posted at: 2019-07-11T05:32:31.090Z Reads: 84

```
I made some more progress today in implementing the changes needed before beta testing, but I also ran into a new issue.

When getting the Firefly remote to work, I realized that it communicates using 5v not 3.3v logic levels. The SAMD21 pins arent 5v tolerant (even though I've had no issue with 5v so far) but this can be solved by using series resistors on the RX pin of the external device ports.

The issue I'm having trouble figuring out is that the RX pin of the Firefly is getting pulled up to 5v internally, and when the splitter tries driving that pin low, it only pulls it down to ~2v. This isn't always low enough for the Firefly receiver to recognize the 0 bits. Does anyone have ideas on how I can fix this in the receiver SW (possibly by removing the pull-up) or in HW?
```

---
## \#40 Posted by: Ricco Posted at: 2019-07-12T05:38:22.122Z Reads: 82

```
I figured out the cause of the issue with sending data to the Firefly reciever. The reciever is based on an [arduino clone](https://robotdyn.com/nano-v3-atmega-328-usb-ttl-ch340g-micro-usb.html) which has a USB to Serial convert IC on board. That IC pulls the RX and TX pins up to 5v with a 1k resistor no matter what pin configuration the micro is programmed with. This combined with the fact that the SAMD21 drives it’s UART TX output has the configuration below means that the RX pin of the reciever is monitoring the middle of a voltage divider and cannot be pulled lower than ~2v.

![image|480x186,75%](upload://jyyEpMx765NFnuVoFEN4IBIRNek.png) 

I would like to make the splitter as plug n’ play as possible and requiring a logic level shifter for certain devices like this defintely wouldnt fit that, but it seems thats the only option atm.
```

---
## \#41 Posted by: Wisp Posted at: 2019-07-12T08:21:49.123Z Reads: 72

```
I'm I correct that this only an issue if you mix 3.3V with 5V devices? Annoying issue but a lot off track for the current concept, no?
```

---
## \#42 Posted by: Ricco Posted at: 2019-07-12T13:52:01.415Z Reads: 78

```
This issue is actually present with an even more specific group of devices, ones that use 5v logic and have pull-up resistors attached to the UART RX pin. However, that group of devices covers most arduino based projects that communicate with the esc since the majority of arduinos have a USB to serial convert on them.

Since there are a number of arduino based projects out there that could benefit from the splitter, I dont think it's out of scope for the project. But since the only solution I see right now is to implement an open drain output on the TX pin of each device port. A logic level shifter will have to be used until I can revise the design.
```

---
## \#43 Posted by: Ricco Posted at: 2019-07-14T18:49:18.032Z Reads: 76

```
Now that Im getting everything together for shipping beta units, its time for a poll to decided the name of the device :smiley:

[poll name=poll2 type=regular results=on_vote public=true]
* USbR
* Uriccosplit
* uSplit
* Splart
[/poll]
New name suggestions are still welcome but I cant add them to the poll :confused: I can make a new poll if needed.

I posted the same poll on [](https://forum./t/uart-splitter-4-vesc-based-escs/3754/34). Please only vote once, either here or there. The name will be decided by adding up both polls.
```

---
## \#44 Posted by: Ricco Posted at: 2019-07-16T05:21:47.181Z Reads: 76

```
The first batch of beta tester units are almost ready to ship :smiley:

![20190716_005330_HDR|610x500,75%](upload://nSrEWlh5XFzK2ABRgL28lO7Ivv7.jpeg) 

@bsancken @Wisp @Flasher @bigmisan
```

---
## \#45 Posted by: willumpie82 Posted at: 2019-07-22T07:33:35.261Z Reads: 72

```
Would be a cool addition to have a CAN-bus <=> uart interface as well... this way you could theoretical connect unlimited devices. next step would be for makes to include a UART2CAN bridge onto theire projects :sunglasses:
```

---
## \#46 Posted by: Kug3lis Posted at: 2019-07-22T09:23:19.674Z Reads: 76

```
[quote="willumpie82, post:45, topic:94552"]
Would be a cool addition to have a CAN-bus <=> uart
[/quote]

Yeah, I was thinking similar thing this weekend to use CAN to uart bridge as you can send same commands via CAN but I would not trust it for doing remote controls because of delays and etc..
```

---
## \#47 Posted by: willumpie82 Posted at: 2019-07-22T10:26:40.481Z Reads: 79

```
yeah, I would not use it for safety related stuff (Remote) although CAN protocol is more reliable than simple UART, hence look what the world is using in cars ;-). I bridged my dual VESC 4.12 with a CAN wire as well (=remotecontrol/sync)
```

---
## \#48 Posted by: Ricco Posted at: 2019-07-23T14:17:56.864Z Reads: 77

```
Beta testing is now underway :grin: 

There are currently 6 testers with the splitter in hand. Because shipping to Europe is expensive, there are 2 more testers waiting for any other European testers to join. This would bring down shipping cost.

If anyone is interested in becoming a beta tester, please PM me.
```

---
## \#49 Posted by: Flasher Posted at: 2019-07-24T05:49:01.490Z Reads: 80

```
[quote="Ricco, post:48, topic:94552"]
6 testers with the splitter in hand
[/quote]

Make that 5. Mine is to arrive somewhere around the end of the week :slight_smile:
```

---
## \#50 Posted by: Ricco Posted at: 2019-07-28T20:40:09.832Z Reads: 78

```
The naming poll is now closed. The tally from both sites with duplicates removed is:

* uSplit - 14
* Splart - 9
* Uriccosplit - 2

Thank you to all who voted :)
```

---
## \#51 Posted by: annihil8ted Posted at: 2019-08-18T07:22:17.039Z Reads: 71

```
Is there any update on this? :)
```

---
## \#52 Posted by: Ricco Posted at: 2019-08-19T04:33:03.137Z Reads: 68

```
There are now 11 beta testers and the last beta unit is shipping out tomorrow :slight_smile: 

I've made some improvements to the FW too:
* Added auto rx/tx pin assignment to the ESC port (working on adding it to the device ports)
* Added auto baud rate detection
* Made numerous reliability improvements

I'm going to quote PCB assembly for the splitters this week. That way, once beta testing is concluded I can order a large batch of them for sale :)
```

---
## \#53 Posted by: Ricco Posted at: 2019-08-21T17:21:06.286Z Reads: 68

```
Now that all beta testing units are shipped out, I want to get an idea of how many people are interested in purchasing a uSplit once they are available.

If you would like to purchase a uSplit, please fill out this survey: https://www.surveymonkey.com/r/5MWPFC6

This will help me to know how many units to order for PCB assembly :)
```

---
## \#54 Posted by: RyEnd Posted at: 2019-09-13T00:36:04.519Z Reads: 62

```
Bumping this so the survey gets more traffic.
```

---
## \#55 Posted by: skyon16 Posted at: 2019-09-18T14:33:17.089Z Reads: 57

```
When do you think you will start selling these?

How well did it work with the firefly remote?
```

---
## \#56 Posted by: Ricco Posted at: 2019-09-18T15:07:32.130Z Reads: 60

```
[quote="skyon16, post:55, topic:94552"]
When do you think you will start selling these?
[/quote]
Testing is still being performed, but I will be ordering the first batch of 50 3-way uSplits sometime next week. The lead time from my supplier is 15-20 days, so I would estimate at least 3 weeks from then till I receive them. In the mean time I will work to get all the documentation ready and my site updated with the shop listing.

Once I receive and test them. I will make the listing on my site active and send a message to all the people who filled out the survey to let them know it's available.

Currently, the survey indicates 41 units will be purchased right away, leaving 9 remaining in the first batch. If anyone would like to ensure they get a uSplit in the first batch and has not filled out the survey, I suggest they do so within the week.


[quote="skyon16, post:55, topic:94552"]
How well did it work with the firefly remote?
[/quote]

The uSplit is not currently compatible with the firefly remote. You can read my replies above to learn exactly why it does not, but long story short; the firefly has pull-ups to 5v on rx and tx making it incompatible without modification. I also have not gotten the time yet to modify my firefly receiver to test if it works after removing the pull-ups.
```

---
## \#57 Posted by: annihil8ted Posted at: 2019-10-01T21:42:21.109Z Reads: 52

```
@Ricco, happy to help out as a beta tester here too! haha your projects and ideas are all so interesting and exciting!
```

---
## \#58 Posted by: Ricco Posted at: 2019-10-02T06:57:49.826Z Reads: 51

```
Thanks that means alot! :blush: I dont need anymore testers, but I will be selling the uSplit soon. I see you filled out the survey, so if you still want one in a few weeks when I make the listing active, then it is all your's :slight_smile:
```

---
## \#59 Posted by: Ixf Posted at: 2019-10-15T16:48:01.982Z Reads: 48

```
Any updates?  Eagerly awaiting to get my paw on one :)
```

---
## \#60 Posted by: Ricco Posted at: 2019-10-21T04:09:21.588Z Reads: 48

```
Hey sorry for the delay, I was waiting to hear back from the company assembling the boards to respond. The first batch of 50 uSplits have been ordered. The assembly company has produced the boards and have ordered the parts. Once the parts arrive, they will assemble one sample part and send it to me. If I approve, then they will assemble the remaining parts and ship those out. It is hard to say how much longer the assembly will take, but it was quoted with 3 weeks lead time and I ordered last week. I would tack on another week and a half for shipping.

There are still a couple potential FW bugs that the beta testers and I are looking into, but the HW has not been an issue. That's why I was comfortable ordering the 50 assembled units. The FW will continue to be worked on while the boards are getting assembled. That way the FW can be completely ready by the time the boards arrive :slight_smile:
```

---
## \#61 Posted by: Ixf Posted at: 2019-10-21T14:04:21.106Z Reads: 47

```
Stupid question.. is this compatible with unity?
```

---
## \#62 Posted by: Ricco Posted at: 2019-10-21T16:40:18.549Z Reads: 47

```
Yes it is. All VESC based ESCs use a standard communication scheme, so it works with any of them :slight_smile:
```

---
## \#63 Posted by: Ixf Posted at: 2019-10-21T16:44:29.702Z Reads: 46

```
Lovely how do I reserve one? I heard you got 9 left :p
```

---
## \#64 Posted by: Ricco Posted at: 2019-10-21T17:36:01.642Z Reads: 47

```
All 50 of the first batch have been claimed on the survey now, but any remaining (its possible some poeple wont follow through) will be first come first serve. For anyone that needs one after the first batch sells out and before the second batch arrives, I could hand assemble them for a small added fee :slight_smile:
```

---
## \#65 Posted by: Ricco Posted at: 2019-11-08T15:20:01.387Z Reads: 48

```
The first sample board shipped out today and should arrive monday :smiley: If everything checks out (from the sample pictures it looks like it will), then they will build the rest of the 50 boards and ship them out. I’m estimating it will be 2 weeks from Monday until I get the full order.
```

---
## \#66 Posted by: Ricco Posted at: 2019-11-12T04:07:40.003Z Reads: 48

```
The sample part arrived today :partying_face:  All solder joints look good and it functions properly so I've given them a go on the rest of the parts :smiley: 

![image|690x402,75%](upload://oMNNgBaQmFzoZz04K4hNEZLarHb.jpeg)
![image|690x410,75%](upload://bscQKUVP0l9qxEuIwi1q3zJ1YOi.jpeg)  

@lxf, @Thorlex, and anyone who has reached out through PMs about getting one of the uSplits, as you probably know, all of the first batch is claimed atm. However, since I just got the PCBs for v1.1 HW I am thinking that I can hand solder up some of those for people who want uSplits before I order more assembled boards. This would give me a good sized group of testers for the v1.1 HW and allow me to verify that the updates didnt introduce any issues.

The changes made in the v1.1 HW are very minor:
1. Resistors were added in series with the UART RX and TX signals to protect the ESC and other connected devices from damage if the uSplit happens to become powered when the other devices are not. This is an unlikely scenario since the uSplit is powered from the comm port of the ESC, but it is still a possibility.

2. The "boot" button was replaced with a circuit that automatically puts the uSplit into bootloader mode when a USB cable is connected.

I will get a survey going to collect everyone's info for the hand soldered v1.1 uSplits if people are interested in that.
```

---
## \#67 Posted by: Ricco Posted at: 2019-11-12T17:24:32.172Z Reads: 49

```
Since there people were receptive over on [the forum that shall not be named] I created the survey for v1.1 HW. 

Here it is: https://www.surveymonkey.com/r/DZF365R
```

---
## \#68 Posted by: Ricco Posted at: 2019-12-12T16:26:08.791Z Reads: 45

```
I have now reached out to everyone that filled out the first and second surveys and have shipped out most of the 50 units.

Right now I have  **6 uSplits left**  to be sold. If you would like one, please DM me.

The price is $30 per uSplit + shipping, tax, and paypal fees
```

---
## \#69 Posted by: Ricco Posted at: 2020-01-09T00:51:12.833Z Reads: 23

```
I recently posted FW v0.7 to the uSplit downloads page of my site. This FW fixes a couple know bugs in the uSplit FW. Anyone that has recently purchased the uSplit should follow the instructions [here ](http://solidcircuits.net/usplit-documentation/) to update your uSplit. If any other issues are found, PM me with details so I can start on those :slight_smile:
```

---
## \#70 Posted by: Kro Posted at: 2020-01-22T01:22:17.998Z Reads: 17

```
I can't send a personal message yet, but I would love a uSplit. Would like to try it with the flipsky remote and Bluetooth with a 4.12
```

---
## \#71 Posted by: Ricco Posted at: 2020-01-22T02:12:58.884Z Reads: 16

```
You can send me an email at support@solidcircuits.net with the quantity you want, paypal email, and full address to get the order started :slight_smile: It should work well for your setup. I know some users are already using it with the VX1 remote.
```

---
