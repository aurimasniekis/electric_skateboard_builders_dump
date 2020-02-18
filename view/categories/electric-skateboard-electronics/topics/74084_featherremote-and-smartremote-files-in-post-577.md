# FeatherRemote and SmartRemote (Files in post #577)

### Replies: 1024 Views: 17396

## \#1 Posted by: StefanMe Posted at: 2018-11-09T20:17:36.574Z Reads: 982

```
Hey guys! Since a while I decided to develop a bit in the remote section and endet up with the FEATHER REMOTE.

![fe978d38-dd0e-4e3c-9dea-d0ea91fb4ec0|690x330](upload://yqSYE0Wb9AJfawsskhPqZNQZXs5.jpeg) 

As @DroidSector decided to go with the TOGO board, I ll stay on the FEATHER M0 RFM69. Two different ways... I think its great, it gives the community more choices and everyone can use the remote with his own preferences.

I put a lot of work onto the code and now can say its stable enough for daily rides. I used the remote now for month and had NEVER any problem with it. I programmed a lot of DEBUG code on the remote to check the connection while riding and I am happy with the results. I never had any issues with the remote from interferences... not down town, not at places with thousands of peoples...

I focused a lot on the safety and stability features... special the ESTOP feature on lost connections (I never had one, but u can try it while switching off the remote while riding...) worked awesome. 
I am also very happy with the "encryption key" handling. Works super smooth and its super safe.

I also tried the different GUI from @DroidSector. It looks super cool, but I think its not that perfect for such a small screen... I ll stay on my clunky big numbers screen. Also because I am not good in designing good looking screen :slight_smile:  

Here are some features:

- 0.96inch OLED with 128x64 with high frequently display update rate to have smooth and accurate informations (every 60ms)
- join settings menu with 5 seconds press on extra button or hold trigger on start up
- trigger can be used as DEADMAN-Switch or CUISE-Control
- vibration feature (Alarm on low battery from Board, Remote battery...)
- extra button to switch between 3 different main Screens 
  - Speed, Distance, Voltage
  - Voltage, Motor amps, Battery amps
  - DEBUG RSSI, cycle time, failed transmissions
- headlight integration by pushing the extra button for 2 seconds
- over 16 updates per seconds from throttle position to PWM output (every 60ms)
- pair up to 200 boards with unique ID
  - one remote will handle all boards by selection the board ID from settings menu

Safety Features:

- automatic generated 16 bytes encryption key (15 bytes for unique key and 16th byte for board selection)
  - after first tun on from remote, it will generate a random 15 byte key
  - every new receiver can be paired from settings menu with the new key and board ID (after first connect, u have to switch on and off the board to acknowledge the new pairing)
- ESTOP automatic slow down until stop - more than 450ms no new values from remote will force the receiver into ESTOPMODE and slow down the trigger value every 50ms by 2/4 (soft/hard) until it reaches 25% break trigger to stop the board safe
  - ESTOP will armed automatically after first valid transmission between remote and receiver
- priority transmission handling! Deactivating display refresh and UART pull if no valid transmission is received until
  - ESTOPMODE is triggered, then display is refreshing again for analysing error
- break light integration with adaptive flash warning
  - if trigger is under middle position the break light will be bright 
  - if trigger is close to full break position the break light will flash
- different riding modes for beginners | intermediate | pros
  - trigger value will be attached to 50% | 75% | 100%
- police mode
  - Trigger value will be cut of at 25%, can be unlocked with button press combination

MANUAL:

https://docs.google.com/document/d/17HkXw-V4jRMWkZ8O-B_I8DazQVeFwYYrkrsUbQE8zrY/edit

STL:

https://www.thingiverse.com/thing:3321282

Here are some pictures of the current status:
The PCB for a nice clean build with JST-PH connections (I ll replace them in the next order with JST-ZH plugs)

![FeatherRemoteDisplay|690x422](upload://MtLOmGemKSaRpNX1mcCeWZjcY7.png) 

![FeatherRemoteOverview|461x499](upload://vmZw2KuDjgHnrdER7Bo3C1f5Zo9.png) 

![IMG_7160|375x500](upload://capqJuKXvE9rNAz4yCNopGcRYid.jpeg) 


The remote also got some bearings inside for a smoother run. I am not a big fan of the plastic slide style...

![16|374x385](upload://jApwnu3GLSJkHfXXSWVe0Pq6I2f.png) 

![59|453x480](upload://p6nJuFKtbuFsA2Ix7MuQ4STgKcv.png)

FeatherRemoteBasic Receiver V0.1:
![FeatherReceiverBasicWiring|690x222](upload://ciZfUZEF6MC9eJZyy0ShXXMVxeQ.png) 

FeatherRemoteAdvanced Receiver V0.1:
![FeatherReceiverAdvancedWiring|690x365](upload://hCalRIsiAjp1BQsZr1rJt04YdRQ.png) 


Side project...
--------------------------------
I am also working on an super super small SMD PCB to convert every remote to an SMART remote. And yes... its fucking small... 25x32mm with JST connection for all u need... close to finish, but need some testing of course :wink:

![48|570x500](upload://k9RGEWNZfwSuQ2iDOMlnI1HTsgZ.png)

So I u have any ideas or suggestions, please let me know. I ll sell one two or three remotes with receivers before I ll release anything to make sure everything works perfect. Its special interesting for people who riding more then one board frequently and want to use the same remote all the time.

Keep calm and eat :hamburger:
```

---
## \#2 Posted by: venom121212 Posted at: 2018-11-09T20:22:24.367Z Reads: 788

```
Really promising stuff! Can't wait to see where this ends up. :sunglasses:
+1 on the beta testing with the new unity
```

---
## \#3 Posted by: evoheyax Posted at: 2018-11-09T21:18:18.984Z Reads: 797

```
This is the remote I've been waiting for... Very nicely done!

If you need any beta testers to give one some abuse, I generally find a way to ride that breaks most stuff.
```

---
## \#4 Posted by: neiru37 Posted at: 2018-11-09T21:22:09.923Z Reads: 771

```
I like that you used JST instead of headers and/or directly soldering the pins, makes things easily modular and replaceable!
```

---
## \#5 Posted by: Silverline Posted at: 2018-11-09T21:51:17.611Z Reads: 718

```
I freaking want one 😍😍😍 are you planning to sell it, as a complete DIY kit ?
```

---
## \#6 Posted by: dougpage Posted at: 2018-11-09T21:57:16.007Z Reads: 680

```
Lol police mode :smile:
```

---
## \#7 Posted by: amazingdave Posted at: 2018-11-09T22:07:09.934Z Reads: 661

```
Love this. Let me know if you want beta test in the U.K. brilliant.
```

---
## \#8 Posted by: walleywalker Posted at: 2018-11-09T22:15:15.519Z Reads: 626

```
Cannot wait until I can buy a few of these off of you. Stoked about this remote.
```

---
## \#9 Posted by: PickSix24 Posted at: 2018-11-09T23:07:04.641Z Reads: 610

```
I’d love to test this
```

---
## \#10 Posted by: Devilmycry Posted at: 2018-11-10T00:54:27.519Z Reads: 602

```
Amazing job man 
I will love to test it 😎😎😎
```

---
## \#11 Posted by: Grolletje Posted at: 2018-11-10T10:36:26.777Z Reads: 572

```
Nice remote, I really like the police mode!
```

---
## \#12 Posted by: Grolletje Posted at: 2018-11-10T10:38:54.564Z Reads: 571

```
How do the lighting features work?
```

---
## \#13 Posted by: bevilacqua Posted at: 2018-11-10T12:00:52.299Z Reads: 583

```
last week I was at Stefan's house and I tested the remote in person. I can confirm that it has a very good ergo-fit, better than the Firefly as it is smaller. What I liked the most is the debug feature, it's the only remote I know that tells you if there where any connection problems. The ball bearings make it also super smooth. 

I'm definitely gonna use it in my personal HAYA board. Super stoked to mount it as soon as my board arrives :D
```

---
## \#14 Posted by: StefanMe Posted at: 2018-11-10T12:41:11.418Z Reads: 608

```
@bevilacqua Aye man! I am looking forward to to place the new receiver PCB into our beautiful deck! And of course I ll order one from u :sweat_smile: take my money :hugs:

@Grolletje there will be some components not he receiver PCB to take care of this. The code is already done and working nicely. I tested it on breadboard with some small LEDs. The total power of headlight and backlight is 36W. Should be enough for a bright night!  
The PCB is also here, but I am still missing some components. On the board is an 42V to 12V regulator capable of 3A current. U can connect parallel to your VESC over screw terminals and drains directly from the battery... 

There will be an "easy" board available with no features except of capacitors and a reset button to reset the address (and of course the JST connector!) and an advanced board with the 12V regulator, headlight, breaklight and buzzer
![IMG_7172|666x500](upload://584nxPJCCJSDBt0CbYdGw04FK9t.jpeg) .

@dougpage I live in Germany, the only country in the entire world where rules existing for small electric vehicles :smile:  

@Silverline yes, I think there will be an diy kit available. BUT I ll send the FEATHER M0 precoded. I don't want to free the code for now. Maybe in the future. 

@all I ll go on with the finish developing this week. I ordert some FEATHERS and will choose 3 testers of the end of the week.  1 in US and 2 in Europe. The price will be 100euro for a set (including everything!). U ll get the money back if u think the thing is shit and u don't like it.
```

---
## \#15 Posted by: Friskies Posted at: 2018-11-10T12:44:55.508Z Reads: 538

```
Put me up for first "tester" in Australia :wink:

It looks fantastic!
```

---
## \#16 Posted by: briman05 Posted at: 2018-11-10T12:54:57.094Z Reads: 533

```
In order to see the settings feature you will need a BT module right. I didn’t see anything about it but just want to clear that up.
```

---
## \#17 Posted by: StefanMe Posted at: 2018-11-10T13:09:18.046Z Reads: 548

```
@briman05 no, i don't need a bluetooth module...  just connect the the JST 5 pin plug to your VESC and go for it.

The settings will be changed at the remote itself in a simple settings menu and the remote will transmit the settings to the receiver via the build in RFM69 module.
```

---
## \#18 Posted by: totalgeek9224 Posted at: 2018-11-10T13:10:49.409Z Reads: 539

```
Can we expect to see video's of it in action? It sounds wonderful and i know that i would really love to see it develop and see it in its current state
```

---
## \#19 Posted by: StefanMe Posted at: 2018-11-10T13:13:00.703Z Reads: 538

```
If @bevilacqua will bring his board here within the next week I guess we ll make a video for u. :grinning:
```

---
## \#20 Posted by: PickSix24 Posted at: 2018-11-10T13:14:47.417Z Reads: 529

```
@StefanMe I’m in the US....:grinning:
```

---
## \#21 Posted by: moone Posted at: 2018-11-10T13:22:45.628Z Reads: 481

```
I'll jump on this ship. 
Couple of Australian testers are definently required. I do 30-50km a day so can help out 😂😂😂
```

---
## \#22 Posted by: Friskies Posted at: 2018-11-10T13:52:47.407Z Reads: 467

```
It makes sense, one of the harshest environments in the world 😛
```

---
## \#23 Posted by: moone Posted at: 2018-11-10T13:56:09.240Z Reads: 463

```
And It's coming into summer so we don't need to worry about the weather!!
```

---
## \#24 Posted by: totalgeek9224 Posted at: 2018-11-10T14:26:42.490Z Reads: 480

```
[quote="StefanMe, post:14, topic:74084"]
The price will be 100euro for a set (including everything!). U ll get the money back if u think the thing is shit and u don’t like it.
[/quote]

Is the the estimated price or beta-tester pricing?

really excited for this project
```

---
## \#25 Posted by: Pedrodemio Posted at: 2018-11-10T14:30:39.599Z Reads: 457

```
Nice work @StefanMe

Would you consider releasing only the case files? I think most of the firefly components would fit, already have all of them, but didn’t found the ergonomics to be perfect (too long)
```

---
## \#26 Posted by: StefanMe Posted at: 2018-11-10T14:57:10.056Z Reads: 454

```
@totalgeek9224  Yes this will be the price for the betas. The later version will be a bit more expensive.

@Pedrodemio yes I can do this... but at the moment I don't have a nice solutions for the ONOFF switch, so there is a little hole on the back. I ll upload them tonight.

@moone @Friskies  that sounds awesome! At the end of the week I ll decide how many beta testers I ll run. maybe there will be two slots for Australia
```

---
## \#27 Posted by: deucesdown Posted at: 2018-11-10T16:29:55.925Z Reads: 437

```
Really nice! So good to see all these remotes being worked on.

If you have haptic for low voltage, can you add for high voltage? It'll be good for those with charge only bms.
```

---
## \#28 Posted by: totalgeek9224 Posted at: 2018-11-10T18:12:46.570Z Reads: 431

```
I believe the haptic for low volts if in regards to the remote, not the board
```

---
## \#29 Posted by: deucesdown Posted at: 2018-11-10T18:29:16.854Z Reads: 423

```
what I mean is, if you're at pack max and you brake, it would be great if it vibrates to let you know you're overcharging.
```

---
## \#30 Posted by: MrCheatak Posted at: 2018-11-12T00:11:48.893Z Reads: 425

```
This will really be a next step for remotes.
Personally, I like the idea with bearings. Holding something that works smooth is pretty a part of the whole experience.
```

---
## \#31 Posted by: murdomeek Posted at: 2018-11-12T00:27:42.617Z Reads: 423

```
cruise control is a great feature i've been looking for! :slight_smile: 

the beginner/intermediate/expert mode is also something i really liked from my chinese board, but havent found any VESC compatible remotes that do this

great job!
Cant wait to follow along on the progress :slight_smile:
```

---
## \#32 Posted by: StefanMe Posted at: 2018-11-12T07:23:50.361Z Reads: 425

```
@deucesdown  Ok, i ll think about this in the next steps... :slight_smile:

@MrCheatak jeah! Thats what i want. A super smooth stable remote that works all the time and makes my life easyer!

@murdomeek should be a very easy function to include... this feature will also be avaible for betas.

Unfortunitly is lost a bit of code from the last days. I screwed up something by handling the data... :( But its not that bad. I ll give u an update later in the evening!

Thanks guys! U keeping me motivated!!
```

---
## \#33 Posted by: moon Posted at: 2018-11-12T07:28:58.567Z Reads: 398

```
Hi did you mention anything about releasing the design files? For the case? I would like to use the step file.
```

---
## \#34 Posted by: StefanMe Posted at: 2018-11-12T10:19:52.194Z Reads: 400

```
Sorry not at the moment... i still got no good place for the ON/OFF switch. I tried to use the DEEP SLEEP mode of the Feather, but it still draws to much current. I think a ON/OFF swtich is needed. 

I ll get some switches later this week and then i will release the STLs.
```

---
## \#35 Posted by: MrCheatak Posted at: 2018-11-12T11:39:22.176Z Reads: 397

```
With all those SMART things, BT, cruise control, vibrations and maybe a little display it'll have almost as much brains as an ESC :joy:
```

---
## \#36 Posted by: moon Posted at: 2018-11-12T17:18:32.450Z Reads: 399

```
Thanks,any chance for the .step file as well? I don't want to 3D print all of it
```

---
## \#37 Posted by: StefanMe Posted at: 2018-11-12T19:16:32.178Z Reads: 460

```
Time for updates!

I got a little setback yesterday, because I lost o lot of data, but I could recode everything...

- ESTOP feature improved / I got some new feature in this function. (Board slows down until -25% throttle until the board stops, tested on full speed... works just great!)
  - added a setup possibility to adjust this feature in three different stages. U can choose between SLOW, HARD and OFF. Nice for people who don't wanna use this function or make it more strong.
  - RECOVER from eStop is simplified! Before u had to switch on and off the board. Now you just can recover by bring back a stable connection for 1 Second and the board can (I count the transmissions within one second and jump into normal mode if a certain amount of transmissions are done in this second!). This is perfect if u just leave u board somewhere outside and went in for a coffee or something. Go out of the shop, grab your board and the board run as before!
  - added a little shield icon to the main screen to always knows that the ESTOP mode is working and the board is safely connected

- Center Death Zone added
  - I added a adjustable area where the trigger will be ignored in the center. Can be adjusted in the settings menu as well

- Riding modes
  - I implemented a simple "Beginner", "Intermediate" and "Pro" mode where the remote calculates independent trigger to throttle output mappings. Means in "beginner" mode u can use the HOLE throttle movement but max trigger will only be converted in an 75%isch throttle... on "Pro" mode it will use a 100% throttle output as normal

- Improved encryption key handling... now it works super smooth to pair a new board! Even switching between different boards is easy as f&&k. Its the first option in the settings menu.

- I changed the trigger to an bigger tactile switch, gives it a nice clicky and stronger feedback!

- still waiting for new ON/OFF switches. I think I got a nice solution for this. Direct solders to the PCB.

- I ll order some new PCBs with slightly improvements... the old ones are still very good! I will start some builds if my Feathers are arriving. Should be within the next days!

And sorry for my excellent englisch :sweat_smile: I try my best!

BOOOOYSCH i am exited!
```

---
## \#38 Posted by: venom121212 Posted at: 2018-11-12T19:26:25.149Z Reads: 442

```
I think there are a ton of us equally excited! Really great to see this component of esk8 finally catching up to the technical advancements around it.
```

---
## \#39 Posted by: StefanMe Posted at: 2018-11-12T20:39:54.755Z Reads: 456

```
Just a fast picture to see how small this thing is! don't take a look on my broken display... the display shows just every second line verticaly... :sweat_smile: Looks awesome in black/sand...

![IMG_7187|375x500](upload://ikYY53FEbjoAWkgluHTYuVonQe7.jpeg)
```

---
## \#40 Posted by: totalgeek9224 Posted at: 2018-11-12T20:43:47.789Z Reads: 448

```
Looks Promising!
```

---
## \#41 Posted by: sharky Posted at: 2018-11-12T20:51:53.449Z Reads: 424

```
Really nice work man👍👍
Can you tell me whicj bearings youre using to smooth the thumb wheel motion?
Kr
```

---
## \#42 Posted by: Grozniy Posted at: 2018-11-12T20:56:21.013Z Reads: 407

```
Just or of curiosity: is it possible to make this remote in aluminium case, attach velcro to one side, and use it as puck in case of fall? Or is completely bs idea?
```

---
## \#43 Posted by: StefanMe Posted at: 2018-11-12T21:00:43.335Z Reads: 408

```
@sharky thanks man! I am using some 8x3x4mm bearings inside.. (4 in total... 1 trigger, 1 retract, 2 thumb wheel)  

@Grozniy good idea... most expensive puck u ll ever own
```

---
## \#44 Posted by: sharky Posted at: 2018-11-12T21:08:48.994Z Reads: 395

```
Great thx man for your help!
```

---
## \#45 Posted by: Grozniy Posted at: 2018-11-12T21:08:54.736Z Reads: 389

```
The idea behind this is when you fall, you don't lose control of the board
```

---
## \#46 Posted by: Pedrodemio Posted at: 2018-11-12T21:20:25.873Z Reads: 388

```
@StefanMe how does the ESTOP behaves if you are applying full throttle or full brake? I have something similar coded in my remote but for now I have to turn on and off the board since I couldn’t find a safe way to resume the command, abruptly doing it can throw you off
```

---
## \#47 Posted by: StefanMe Posted at: 2018-11-12T21:55:38.927Z Reads: 394

```
I have a complex handling with the estop. Took me a while to get this done. 

Depend on settings u have chosen in the settings menu, the board will slow down completely until the break is at -25% throttle. I slow down a virtual throttle and check some internal things... then I make connection checks between remote and receiver and verify the values that are coming in are "safe" within a specified time for a few time. At this time the board is standing still. Then u can throttle again... IF ur are in "soft" mode. If u are in "hard" mode u have to recover with full throttle back for a while. Sounds much easier than it is... u also have to capture some other things like parts where u are not transmitting data... if u are in the menu... but still want the board not go into estop mode ect.
```

---
## \#48 Posted by: StefanMe Posted at: 2018-11-12T21:56:14.583Z Reads: 379

```
What should happen? U mean u destroy the remote and the board will run away? For this I implanted the ESTOP feature
```

---
## \#49 Posted by: Pedrodemio Posted at: 2018-11-12T21:58:53.966Z Reads: 381

```
Thanks a lot, really liked your solution

I’m thinking in doing it so that if the connection is restored the throttle has to be kept neutral for a given time until it is resumed
```

---
## \#50 Posted by: StefanMe Posted at: 2018-11-12T22:01:37.595Z Reads: 378

```
Thats how I do it on the "soft" mode... its more complex, but that's the main idea.

My first version was the same like yours. But it sucks when u are just a few meters away from the board and the board goes into estop, u have to switch on off again.. Blabla... sucks.
```

---
## \#51 Posted by: Pedrodemio Posted at: 2018-11-12T22:04:56.722Z Reads: 379

```
The worst I how mine is currently

It just goes to neutral until the board is reset, I only lóst connection once, but it was scary since I forgot I had it setup that way, almost run over two old dudes
```

---
## \#52 Posted by: StefanMe Posted at: 2018-11-12T22:06:40.647Z Reads: 386

```
I can't understand why there aren't any features like this in the remote section. Show me the result if u are done... would be nice to see a different version how to handle it...
```

---
## \#53 Posted by: Pedrodemio Posted at: 2018-11-12T22:07:29.313Z Reads: 404

```
Will do, there is a lot of other things I have to code first
```

---
## \#54 Posted by: StefanMe Posted at: 2018-11-17T11:49:20.188Z Reads: 418

```
So boysch! little update!

the PCB with receiver and step-down form 42V to 12V for headlights and adaptive break lights is finished. Had a little trouble to find all the components, but now its working great. Check out the short demonstration video!

Of course adjustable from the settings menu... always on, with headlights or off. 

https://youtu.be/Ood2ag2Ke_U
```

---
## \#55 Posted by: totalgeek9224 Posted at: 2018-11-17T11:53:25.445Z Reads: 397

```
Looking awesome!
```

---
## \#56 Posted by: venom121212 Posted at: 2018-11-17T12:18:34.592Z Reads: 394

```
Man this keeps looking better and better! Great work! :+1:
```

---
## \#57 Posted by: myreala Posted at: 2018-11-18T05:49:46.278Z Reads: 384

```
Can I get in on the wait list on this? I so need this.
```

---
## \#58 Posted by: Darkie02 Posted at: 2018-11-18T07:42:34.493Z Reads: 383

```
Loving you work looking so awsome. hoping there will be pre orders soon 😉
```

---
## \#59 Posted by: StefanMe Posted at: 2018-11-18T14:11:48.678Z Reads: 408

```
Hey guys, I did a lot of testing the last days. And I am happy with the results! The Remote is ready for the first orders! 

I want one please fill out the order file. I ll start building after I received the payment. 

- FeatherRemote Advanced
Get the full package, with remote and advanced receiver assembled and ready to start! The advanced features include a receiver PCB with 10s to 12V step down (3A) to use simple and small motorbike breaklights and headlights. Adaptive break light support.

- FeatherRemote Basic 
Get the full package with remote and basic receiver assembled. Includes 5pin JST connector to simply connect the receiver to the VESC/FOCBOX.

- FeatherRemote DIY
Get two PCBs with mounted and precoded Ardunios/FeathersM0 combinations to print or create your own FeatherRemote as u like.

FeatherRemote advanced (FeatherRemote, FeatherReceiver Advanced) 160€
FeatherRemote basic (FeatherRemote. FeatherReceiver Basic) 130€
FeatherRemote DIY (Adafruit Feather precoded with PCB for remote and receiver all other parts must be provided by your own!) 80€

I ll accept 10 orders for the first batch and will support each order on setup ect. For more questions just sent me a message!
```

---
## \#60 Posted by: b264 Posted at: 2018-11-19T00:27:53.383Z Reads: 374

```
Can the throttle be reversed, so away-from-body is brake and towards-body is throttle?

Those of us using trigger remotes can't really even try things like this without that feature

It'd be like borrowing your spouse's car except the throttle and brake pedals are on opposite sides from yours ... then a car pulls out in front of you ... and you instinctively mash the throttle.... despite being in full control the entire time up to that point when your reflexes activated
```

---
## \#61 Posted by: koralle Posted at: 2018-11-19T02:39:17.417Z Reads: 359

```
Theres no good reason, why these parts can't be built into a 3d printed trigger style remote. Someone just needs to model it.
```

---
## \#62 Posted by: StefanMe Posted at: 2018-11-19T10:27:22.899Z Reads: 356

```
Do it ;)

10char
```

---
## \#63 Posted by: Silverline Posted at: 2018-11-19T10:48:59.792Z Reads: 354

```
Yeah... Trigger style would be so nice 😍😍😍 much more control on a MTB
```

---
## \#64 Posted by: StefanMe Posted at: 2018-11-19T11:07:24.848Z Reads: 361

```
If someone made one. i ll create a PCB for it!
```

---
## \#65 Posted by: bevilacqua Posted at: 2018-11-19T14:11:47.660Z Reads: 376

```
I think you just need to flip the wheelknob magnets. Tath way you would reverse the hall-effect
```

---
## \#66 Posted by: StefanMe Posted at: 2018-11-19T21:21:25.617Z Reads: 389

```
Short update! I started to assemble the first batch! 

![IMG_7323|375x500](upload://zPsKuPW2JoPtBBhl76TlNG8S88P.jpeg)
```

---
## \#67 Posted by: Zentaria Posted at: 2018-11-19T21:29:09.144Z Reads: 371

```
How do I know I am one of the first 10?:D
```

---
## \#68 Posted by: StefanMe Posted at: 2018-11-19T21:32:01.741Z Reads: 359

```
U are in the first 10! Payment done? I am currently at 8 orders.
```

---
## \#69 Posted by: Surfer Posted at: 2018-11-19T21:33:59.684Z Reads: 359

```
@StefanMe, can you check, I pm you
```

---
## \#70 Posted by: Surfer Posted at: 2018-11-19T22:03:37.525Z Reads: 368

```
Just one question, the pcb size of the advanced receiver is the same than the basic receiver? Just not populated with all components? Or the basic is smaller?
```

---
## \#71 Posted by: StefanMe Posted at: 2018-11-19T22:09:49.620Z Reads: 373

```
Smaller... less then the half size of the advanced PCB. ![image|667x338](upload://ekhpY0EoFwvYakzvmq00a5O3mcZ.jpeg) 

Tomorrow i hope i have time to make pictures from the small PCB.
```

---
## \#72 Posted by: evoheyax Posted at: 2018-11-19T22:31:02.837Z Reads: 357

```
Looks great, didn't realize it would be so high priced. Is the set down for 10s only?

If so, I might just get a basic and call it a day. I have done the tail lights using arduinos before and it works well. Just take in the pwm and if past a certain value, make the lights brighter. And once it falls down below a certain value, the light dim again. Pretty simple code.
```

---
## \#73 Posted by: sofu Posted at: 2018-11-19T23:15:41.987Z Reads: 346

```
PM'd in the hopes that an advanced version is still available :P
```

---
## \#74 Posted by: PickSix24 Posted at: 2018-11-20T02:02:50.646Z Reads: 338

```
Woo Hooo ! Hopefully one of those is mine :stuck_out_tongue_winking_eye:
```

---
## \#75 Posted by: StefanMe Posted at: 2018-11-20T06:59:02.824Z Reads: 338

```
I ll double check later if a 12s is possible... 

MAYBE u/me have just du exchange an condensator.
```

---
## \#76 Posted by: amazingdave Posted at: 2018-11-20T08:28:19.997Z Reads: 337

```
I’ve just realised that this is not going to work for my 12s board.... 🙁
```

---
## \#77 Posted by: StefanMe Posted at: 2018-11-20T08:51:14.219Z Reads: 342

```
No problem guys! U are in the first batch where is a little bit space for changes.

Looks like i can upgrade some parts for 12s. I have to change at least the diode and one capacitor. I try to organize a board with 12s to test it. I run only on 10s, But i look optimistic!
```

---
## \#78 Posted by: deucesdown Posted at: 2018-11-20T16:41:10.734Z Reads: 339

```
[quote="StefanMe, post:77, topic:74084"]
upgrade some parts for 12s
[/quote]

If you're changing stuff, go to 13s. :slight_smile:
```

---
## \#79 Posted by: totalgeek9224 Posted at: 2018-11-20T16:41:42.061Z Reads: 331

```
Agreed with this, might as well give yourself the headroom
```

---
## \#80 Posted by: Friskies Posted at: 2018-11-20T16:44:56.021Z Reads: 333

```
I will need mine for 12s too pleeeaaase
```

---
## \#81 Posted by: StefanMe Posted at: 2018-11-20T19:01:00.105Z Reads: 316

```
Of course :slight_smile: I went now to **14s. max is 60V**. But I have to test this at first...
```

---
## \#82 Posted by: tricky-fpv Posted at: 2018-11-20T20:15:01.305Z Reads: 309

```
I filled in the form.
How do i know what batch i am in?
```

---
## \#83 Posted by: StefanMe Posted at: 2018-11-20T20:26:44.544Z Reads: 312

```
First batch! 

FIRST BATCH IS CLOSED NOW!
```

---
## \#84 Posted by: tricky-fpv Posted at: 2018-11-20T20:29:10.861Z Reads: 309

```
Awsome:-) lucky me
```

---
## \#85 Posted by: tricky-fpv Posted at: 2018-11-20T22:54:56.313Z Reads: 315

```
Jist as an idea. I used 5volt buzzers on my freestyler drones if battery was low.
Maybe an idea for future to build in a loud buzzer as thay are fairly small with a switch beep beep move b@#$ get out the way lol.
Handy for those moments u need a bell or buzzer
Jist an idea
```

---
## \#86 Posted by: StefanMe Posted at: 2018-11-21T06:01:41.244Z Reads: 312

```
Hey tricky! As u can see on the first feature list, i have already implemented a vibration motor ;) much more reliable as an beeper.
```

---
## \#87 Posted by: tricky-fpv Posted at: 2018-11-21T06:57:54.772Z Reads: 306

```
I mean a beeper for people in front of u like a bell to warn them ypur approaching
```

---
## \#88 Posted by: StefanMe Posted at: 2018-11-21T07:14:53.509Z Reads: 327

```
Ahhhhhh ok, COOL IDEA!!! Like a "horn". (Just use BELTS... they are loud enough :slight_smile: )

I ll think about this! Maybe an make an option where u can use the headlight or breaklight connector to actiave a horn. I see, we need an extra button above the trigger for this...
```

---
## \#89 Posted by: moon Posted at: 2018-11-21T07:27:15.117Z Reads: 336

```
CNC remote, wish me luck ![IMG_20181121_072641|375x500](upload://wT4x81n92qvXFwxpekmgGRfMKyl.jpeg)
```

---
## \#90 Posted by: StefanMe Posted at: 2018-11-21T07:28:45.793Z Reads: 327

```
Oh man! this is sick! 

Guys, can u help me: What is the correct word for the METRIC(KMH) / IMPERIAL(MPH) menu point? I dont find a word to cover this point in the settings...
```

---
## \#91 Posted by: tricky-fpv Posted at: 2018-11-21T07:28:45.891Z Reads: 322

```
Me living in the lowlands thay live and sleep on bycycles dude lol.
And a mini buzzer or horn button would really be great. The 5volt buzzer are not big not extremly loud coukd be better i guess but in the remote like with a button.
Would be frekken handy. Beep beep!
```

---
## \#92 Posted by: moon Posted at: 2018-11-21T07:41:36.966Z Reads: 314

```
What do you mean? 

Miles per hour and kilometers per hour
```

---
## \#93 Posted by: StefanMe Posted at: 2018-11-21T07:44:26.138Z Reads: 318

```
[quote="moon, post:92, topic:74084"]
u
[/quote]

I mean the name of the Setting itself... 

MENU POINT <--
KM/H - MPH
```

---
## \#94 Posted by: totalgeek9224 Posted at: 2018-11-21T07:46:08.009Z Reads: 308

```
Unit selection?
```

---
## \#95 Posted by: totalgeek9224 Posted at: 2018-11-21T07:48:05.002Z Reads: 307

```
I was thinking, how cool it would be to have an integrated flashlight with the remote? 
Aswell as blinker integration like the [Photon Remote](https://www.electric-skateboard.builders/t/photon-addressable-leds/74309/10?u=totalgeek9224).

I know this is gen 1, but i think these would be welcome improvements for the next gen
```

---
## \#96 Posted by: StefanMe Posted at: 2018-11-21T07:52:00.751Z Reads: 309

```
I ll NEVER integrate a blinker... sorry... never. 

BUT flashlight is cool.  Same as horn... But then u need so many ouputs... mosfets... and so on... more cost... 

I think i ll start an poll for this. I think the next gen will have 3 ouputs. Breaklight, Headlight and horn. But lets get the first gen be true and then we can talk about the next gen! :slight_smile:
```

---
## \#97 Posted by: StefanMe Posted at: 2018-11-21T08:26:19.090Z Reads: 338

```
Just a quick update and explanation of the main page:

Here u find on the top left the throttle indicator. Next to it the long bar for the board battery indicator. On the right side the main values (there will be 3 different pages available... at the moment u see voltage, motor amps, battery amps) and on the bottom system indicators like remote battery, headlight status and the ESTOP status.

![remote|375x500](upload://13ITpgXQMVQ11QYi9UxyhjiWMyc.jpeg)
```

---
## \#98 Posted by: Zentaria Posted at: 2018-11-21T09:04:00.081Z Reads: 327

```
Is the Police mode already in the first batch? :)
```

---
## \#99 Posted by: totalgeek9224 Posted at: 2018-11-21T09:12:10.587Z Reads: 331

```
[quote="StefanMe, post:96, topic:74084"]
I ll NEVER integrate a blinker… sorry… never.
[/quote]

How come? 
10char
```

---
## \#100 Posted by: StefanMe Posted at: 2018-11-21T09:23:59.549Z Reads: 323

```
because i dont see any reason for that... i mean... ok... if u find a lot of people how ant it, it ll implement it of course... but it really dont see any reasion for a blinker :grimacing:

So lets say... its not planed in the near future :sweat_smile:
```

---
## \#101 Posted by: StefanMe Posted at: 2018-11-21T10:53:04.387Z Reads: 305

```
PoliceMode is integrated with 3 options:

OFF 

ON on startup and with button combination - on every startup the police mode is activated [Push trigger and throttle back on startup or button in normal mode]

ON only with combination - only on butotn combination the police mode is activated [Throttle full back, hold trigger and push extra button for 0.5 Sec]
```

---
## \#102 Posted by: totalgeek9224 Posted at: 2018-11-21T10:56:20.555Z Reads: 288

```
But what if.....I...want it...? :sweat_smile:
```

---
## \#103 Posted by: StefanMe Posted at: 2018-11-21T12:10:00.584Z Reads: 296

```
HAHA! OK, u got me.

But not on this batch. I ll create PCB for the reciever with different chip. There i ll implement a few more connectors or maybe an WS2812 port to connect an litestripe... :slight_smile: 

But this will happen next year. I put it on the list!
```

---
## \#104 Posted by: totalgeek9224 Posted at: 2018-11-21T12:22:13.869Z Reads: 297

```
:joy::heart_eyes::heart_eyes:
```

---
## \#105 Posted by: PickSix24 Posted at: 2018-11-21T12:51:02.545Z Reads: 303

```
One of my esk8 apps calls that menu metrics
```

---
## \#106 Posted by: venom121212 Posted at: 2018-11-21T13:44:03.493Z Reads: 301

```
Speed units? Yeah I'm struggling here...
```

---
## \#107 Posted by: totalgeek9224 Posted at: 2018-11-21T14:20:50.487Z Reads: 311

```
Need for speed (units)
```

---
## \#108 Posted by: bevilacqua Posted at: 2018-11-23T17:19:31.637Z Reads: 325

```
![image|375x500](upload://4vE2D5QU5dBAp4sEnGGmDzeR89T.jpeg) 

_work in progress_
```

---
## \#109 Posted by: totalgeek9224 Posted at: 2018-11-23T17:20:27.569Z Reads: 317

```
!!! lets goooooo!!!
```

---
## \#110 Posted by: StefanMe Posted at: 2018-11-23T20:04:10.751Z Reads: 326

```
![image|375x500](upload://w34vzn0r2BEbkr809XOMlbVcmd.jpeg) 

Cooperation with HAYA 

@bevilacqua
```

---
## \#111 Posted by: totalgeek9224 Posted at: 2018-11-23T20:07:10.436Z Reads: 315

```
Lookin good! That HAYA deck is a beauty.
```

---
## \#112 Posted by: Surfer Posted at: 2018-11-23T21:11:00.342Z Reads: 321

```
Wow!! my new build is almost fully custom forum cooperative parts :)

Haya deck from @bevilacqua 
FeatherRemote from @StefanMe
ESCapes from @stewii
antiespark push to start from @Martinsp  
metr pro from @rpasichnyk and @hexakopter 
Just missing the Hubs from @Hummie fire up the kickstarter campain bro!
Battery from @Surfer (myself :laughing::laughing:) 

At this pace the next build after this one will be 100x100 forum suppliers! that would be awesome!!!
```

---
## \#113 Posted by: Pedrodemio Posted at: 2018-11-23T21:20:37.554Z Reads: 313

```
I never give much thought about these integrated decks until I see a shot like this, cleanest clean possible
```

---
## \#114 Posted by: rojitor Posted at: 2018-11-23T23:04:41.185Z Reads: 312

```
Kickass build :heart_eyes:
```

---
## \#115 Posted by: DAddYE Posted at: 2018-11-23T23:17:09.555Z Reads: 311

```
Awe! Are those riptide barrels?
```

---
## \#116 Posted by: tricky-fpv Posted at: 2018-11-24T00:48:07.509Z Reads: 315

```
![15430204306208427678188380284202|690x388](upload://a5ksERcPpCm2yyW2ABtSqjZsC9i.jpeg) 

Ready for a good remote;-) dang she look good!
```

---
## \#117 Posted by: PickSix24 Posted at: 2018-11-24T02:03:04.750Z Reads: 309

```
Nice board ! 
How are the remotes coming along ?
```

---
## \#118 Posted by: StefanMe Posted at: 2018-11-24T11:33:40.785Z Reads: 316

```
![IMG_7418|666x500](upload://rGJZ0uJLOL7tZcVV0eCfaqSHKAE.jpeg) 

printing the final version of the top shell for u guys!
```

---
## \#119 Posted by: tricky-fpv Posted at: 2018-11-24T16:59:51.086Z Reads: 310

```
Could u possibly make a photo of the basic reciever. 
So i can get an idea of the fitting in my enclosure
```

---
## \#120 Posted by: StefanMe Posted at: 2018-11-24T17:19:29.427Z Reads: 329

```
Of course! Here is the basic receiver finally assembled.

![image|375x500](upload://ruy9kZfPaEcbo9OunfyjoCvGjQI.jpeg) ![image|666x500](upload://5DAk3TfPr5QdEJ3M75d8aHlu8i3.jpeg) ![image|375x500](upload://6NM2hzyp0x9uBWGitKo6RPCRvXV.jpeg)
```

---
## \#121 Posted by: bevilacqua Posted at: 2018-11-24T17:30:37.006Z Reads: 296

```
O‘tang yellow nipples. But yes, barrels with flat washers
```

---
## \#122 Posted by: Mich21050 Posted at: 2018-11-24T19:02:40.964Z Reads: 290

```
Are you going to publish the gerber files and the code? :slight_smile:
```

---
## \#123 Posted by: StefanMe Posted at: 2018-11-24T19:18:19.841Z Reads: 293

```
No... not in the near future. 

Baba :slight_smile:
```

---
## \#124 Posted by: PickSix24 Posted at: 2018-11-25T00:21:13.908Z Reads: 288

```
Seriously stoked for this remote! Can’t wait 🤣
```

---
## \#125 Posted by: Legacy23 Posted at: 2018-11-25T05:09:35.849Z Reads: 291

```
When will you be accepting more orders?
```

---
## \#126 Posted by: StefanMe Posted at: 2018-11-25T10:02:31.116Z Reads: 294

```
At the moment I only accept order for the DIY kit. 

Includes just the precoded Feather for remote with PCB and the precoded Feather for receiver with PCB. Its just to much work to assemble everything together. I still waiting for some parts that I ordered a while ago. Hope they come in the next days.
```

---
## \#127 Posted by: DAddYE Posted at: 2018-11-25T11:56:16.055Z Reads: 279

```
What should be assembled? Is there any soldering required? Thx
```

---
## \#128 Posted by: StefanMe Posted at: 2018-11-25T12:05:35.178Z Reads: 287

```
Everything needs to be assembled. But only normal THT parts. No SMD. U need to buy some parts like JST connectors, transitors, buttons, capacitors, ssd1306 Oled ect.
```

---
## \#129 Posted by: StefanMe Posted at: 2018-11-25T12:15:56.159Z Reads: 314

```
The remote comes with the paracord lanyard integrated antenna... the antenna is just slipped in the lanyard. I have a huge bunch of colours here :) everybody can choose his own color. Just write a message. If I didn't get a message within the next week I ll just add an pinkish like on the picture :blush: 
![IMG_7464|375x500](upload://oLPPSY0gJkfEnBzTLwCUMmURojA.jpeg) 
![IMG_9633|666x500](upload://3xAhliJLev1qauBscwlY6HJ5aps.jpeg) 

Just right me a message or here:
Roll 5. from left red
or 
sample 3.from left olive

all colours are more dark in real life... they are just shiny vebcuase of the picture 

@walleywalker
@Darkie02
@PickSix24
@Jansen
@Zentaria
@Surfer
@tricky-fpv
@kiryl         
@sofu

I forgot @Friskies 😐😳 SORRY MAN!
```

---
## \#130 Posted by: tricky-fpv Posted at: 2018-11-25T12:26:20.928Z Reads: 286

```
Black for me please
```

---
## \#131 Posted by: Surfer Posted at: 2018-11-25T12:27:07.933Z Reads: 280

```
Ooh! There is a way to have internal antenna? I don't like the lanyard, I always remove it from my gloves or any other gadget if comes with that :)
```

---
## \#132 Posted by: StefanMe Posted at: 2018-11-25T12:33:48.980Z Reads: 277

```
Ok, we can try it with just internal one. If I have connection problems I can add the lanyard by your own...
 U can also simply let hang out the antenna how I do it at the moment.

We just made some test with an metal deck and run into some issue because of the good isolating metal ;) with the lanyard the connection is more then good. So it’s more for safety...
```

---
## \#133 Posted by: Surfer Posted at: 2018-11-25T12:47:28.767Z Reads: 274

```
Perfect! I will try, anyway I have a plan to make a compressed fiber glass lid.
I got a question, I build in the past the firefly remote and I did like it a lot, but I find very long the travel the thumb wheel, is your model similar travel? It can be adjusted? 
And the firefly has two thumb wheels, round, or with nipple, is the same with yours? Anyway no problem I can get rid of the nipple with a file or cutter.
```

---
## \#134 Posted by: StefanMe Posted at: 2018-11-25T13:12:54.872Z Reads: 293

```
Fiberglas lid... I would love to have one of these >D 

I have a nib on the feather remote... but I ll release the STL files today and anyway...  u can make your own thumb wheel if u want. 

The long travel is more a feature... u have more way to control the power of your board... specialy high power boards can be controlled a lot easier. BUT of course... if u want a short travel there should be a way. I can also realise the step files for the wheel and u can customise the mechanical part on top for your preferences!
```

---
## \#135 Posted by: Surfer Posted at: 2018-11-25T13:21:49.883Z Reads: 284

```
Awesome awesome!!😃 For sure I will make more than one lid, I'm thinking even to make different shapes, maybe W ;)
I will let you know!
```

---
## \#136 Posted by: kiryl Posted at: 2018-11-25T13:34:23.312Z Reads: 280

```
I would like the 3th one from the bottom right side. Between the red and purple.
```

---
## \#137 Posted by: PickSix24 Posted at: 2018-11-25T15:02:30.725Z Reads: 281

```
I’ll take black please
```

---
## \#138 Posted by: Ubbiedude Posted at: 2018-11-25T17:42:08.432Z Reads: 272

```
Interesting remote
```

---
## \#139 Posted by: Zentaria Posted at: 2018-11-25T19:49:18.843Z Reads: 274

```
Ill take a blueish one? :D
```

---
## \#140 Posted by: tricky-fpv Posted at: 2018-11-26T00:30:29.289Z Reads: 283

```
Any idea on when thsy will be ready to ship?
```

---
## \#141 Posted by: walleywalker Posted at: 2018-11-26T04:28:48.848Z Reads: 297

```
This one please for mine. ![jpeg%20(JPEG%20Image%2C%204032%C2%A0%C3%97%C2%A03024%20pixels)|195x500](upload://63fYkqTrgeByaTS8TZvD3iNB3z.png)
```

---
## \#142 Posted by: StefanMe Posted at: 2018-11-26T06:40:37.884Z Reads: 287

```
End of the week I guess! Maybe start of the next week. Looks like I have to send the remotes to USA/Australia without batteries... 😐 but I ll check this today! 

Yesterday I tested the additional feature police mode here in Germany 😂😂😂 it worked out... the police man said i should rather drive away then showing him this ultra slow mode 😂
```

---
## \#143 Posted by: Steven1 Posted at: 2018-11-26T10:29:24.705Z Reads: 276

```
I'm so hyped for this. Please let us know when the next batch is available for purchase. 
I'd probably have a use for police mode since it's illegal In the Netherlands as well :sweat_smile:
```

---
## \#144 Posted by: sharky Posted at: 2018-11-26T19:52:15.008Z Reads: 281

```
@StefanMe
Hey man!
thx very much for the info with the bearing for the thumb wheel.
I just installed it to my firefly remote and its really smooth now
following your remote build all the time may ill get one of yours in future ;-)
kr
```

---
## \#145 Posted by: PickSix24 Posted at: 2018-11-26T22:51:44.431Z Reads: 273

```
What size battery are you using. I’ve got a few 1s batteries around that would probably work if shipping becomes an issue. Or there’s always amazon lol
```

---
## \#146 Posted by: StefanMe Posted at: 2018-11-27T09:26:38.118Z Reads: 285

```
@sharky
Hey man! Cool! Yes the bearings are awesome... just just make shure u don’t tighten them too much like I did one times 😂  show us your remote! 

@PickSix24 
It’s the 502535 size... same as original firefly! I ll get I information soon about how to ship the battery’s!
```

---
## \#147 Posted by: sharky Posted at: 2018-11-27T17:00:46.280Z Reads: 297

```
There it is
![IMG_5790|375x500](upload://A4N95TPdTdJXtNH2tdJcxlRgK5V.jpeg) 
Dont laugh about the color it has to match with the board😂
![IMG_5622|666x500](upload://juESCGy0xZkz3HU3KjLTRKiCSEP.jpeg)
```

---
## \#148 Posted by: tricky-fpv Posted at: 2018-11-28T17:36:55.100Z Reads: 288

```
Ready for shipping yet?
Very excited!
```

---
## \#149 Posted by: PickSix24 Posted at: 2018-11-28T18:32:59.329Z Reads: 280

```
Me too !! So glad I got in on this since I’m currently failing at building the firefly nano remote 🤣🤣
```

---
## \#150 Posted by: StefanMe Posted at: 2018-11-28T22:10:16.490Z Reads: 287

```
Sorry was a bit busy the last days! But 

Super close before shipping guys! The last feathers are allready arrived today. I have to pick them up tomorrow! All the other work is done allready. Still waiting for the batteries! Looks like I can send all out on Sunday/Monday!
```

---
## \#151 Posted by: tricky-fpv Posted at: 2018-11-28T22:13:19.076Z Reads: 279

```
Any possiblilty u can make some photos of the remotes with names next to the remote to show everyones remote done.
Pretty excited!
Did u manage to include my nickname on the screen btw? (Tricky)
```

---
## \#152 Posted by: sofu Posted at: 2018-11-28T23:11:19.431Z Reads: 260

```
Feel free to send mine without the battery! I have extra batteries of the same type :smiley:
```

---
## \#153 Posted by: PickSix24 Posted at: 2018-11-28T23:44:14.511Z Reads: 244

```
Ditto, if mine is just waiting on a battery then send it :grinning:
```

---
## \#154 Posted by: StefanMe Posted at: 2018-11-29T08:10:15.263Z Reads: 255

```
@sofu
@PickSix24  

Ok then, i ll send u the remotes this weekend if the batteries are still not here. I ordert them 1.5 months ago... that sucks. 

@tricky-fpv of course, thats not a problem. I can make a picture tomorrow...
```

---
## \#155 Posted by: tricky-fpv Posted at: 2018-11-29T23:26:05.801Z Reads: 246

```
I am desperately needed the remote.
The one i have lost connection and kept accelerating for some reason.
Now when connection is lost it full brakes?!
Really wierd because settings are at 0.00a when connection lost. Have 0 faith in my remote right now:-(
Badly need a good remote
```

---
## \#156 Posted by: Jansen Posted at: 2018-11-30T05:57:26.182Z Reads: 257

```
Hell's yeah! So stoked to get this hopefully sooner than later cause I broke one of my remotes on one of my set ups so I am out from riding that board till this comes. Thanks for the hard work @StefanMe Can't wait to see the pics tomorrow / today :-)
```

---
## \#157 Posted by: StefanMe Posted at: 2018-11-30T07:19:16.392Z Reads: 275

```
I do my best guys! As i saied before i will ship the remotes at the beginning of the next week. :) so latest 5. Dezember.. maybe earlier!

If u riding on limit, i can reccoment you an LC Filter... 
https://www.ebay.de/itm/Mini-L-C-Power-Filter-1A-RTF-LC-FILTER-Special-for-mini-Drone-For-FPV-Video-BC/273539973986?hash=item3fb040c362:g:cOgAAOSwkJZbHioA:rk:7:pf:0
https://www.ebay.de/itm/LC-Filter-FPV-Netzteil-Filter-3AMP-2S-4S-2A-16V-fur-RTF-RC-Quadcopter-RC-Modell/292710831221?hash=item4426ecd475:rk:5:pf:0

On my boards i never had problems..,. but on some boards, the voltage from the 5v VESC is just shit. Even on a focbox. Just pre prepaired :)
```

---
## \#158 Posted by: tricky-fpv Posted at: 2018-11-30T10:09:06.804Z Reads: 262

```
Lc filter? Is that really needed with a focbox??
```

---
## \#159 Posted by: StefanMe Posted at: 2018-11-30T10:15:42.978Z Reads: 269

```
For me not... for my friend it’s needed. We don’t know why. We make some tests within the next days. Strange. 

But the Lc Filter is super tiny and super cheap. Just in case someone need it.
```

---
## \#160 Posted by: tricky-fpv Posted at: 2018-11-30T10:25:03.881Z Reads: 260

```
How many A does the reciever need?
```

---
## \#161 Posted by: StefanMe Posted at: 2018-11-30T10:40:46.027Z Reads: 264

```
0A. 

Its only a few mA. ;) approximately 50mA
```

---
## \#162 Posted by: tricky-fpv Posted at: 2018-11-30T18:41:29.143Z Reads: 267

```
Any photos of the remotes yet?
```

---
## \#163 Posted by: StefanMe Posted at: 2018-12-01T13:36:39.322Z Reads: 273

```
Sorry guys... super busy. Here is one set (the outside Europe set. Just not assambled, because I wait for the batteries. But it looks like they arrived! I ll see it on Monday!

![image|375x500](upload://pK2ctkfySJjPFbivONlzoK1KK1i.jpeg)
```

---
## \#164 Posted by: sofu Posted at: 2018-12-02T19:27:16.049Z Reads: 264

```
Cat! 😻😻😻😻😻
```

---
## \#165 Posted by: StefanMe Posted at: 2018-12-03T10:21:38.019Z Reads: 261

```
Yes i have two cats :smiley: 


So guys! Update about the shipping status! The fucking batteris didnt arrived till now! So i ll order them right now at a local supplier for a fucking high price... . Sorry for the delay. I didnt expect, that it takes more then 2 months to ship the batteries from china. I ll ship the remotes as soon as the batteries arrive... should be wendesday/thursday...
```

---
## \#166 Posted by: tricky-fpv Posted at: 2018-12-03T10:49:49.719Z Reads: 255

```
U have got to be kidding???!!
This really is a letdown:-(
```

---
## \#167 Posted by: StefanMe Posted at: 2018-12-03T10:55:38.311Z Reads: 247

```
Because? I mentioned before that I am sto waiting for the batteries ^^ so what is the problem tricky?
```

---
## \#168 Posted by: tricky-fpv Posted at: 2018-12-03T11:09:51.687Z Reads: 250

```
No worrys mate just was hoping for it to be sent today or tomorrow.
Been. Had a friend build a firefly for me and waiting since july to novmeber for it and he sent it and it dint qork and did a shit job and sent it back and got my money back. Then searced for a good remote and found you.
No worries mate glad u will get the batterys this week.
Just been waiting months for a decent remote
```

---
## \#169 Posted by: StefanMe Posted at: 2018-12-03T11:12:09.092Z Reads: 252

```
The irders startet 15 days ago. I told everyone the build time will be 2-4 weeks. So everything is totally fine. Be more relaxed man ;)

I do my best man! Hope U are happy with the remote! The assembly and everything is super clean because of the PCB. So it should be a good work at all. I am also interested tagt everyone gets a nice remote for his every day ride! :slight_smile:
```

---
## \#170 Posted by: tricky-fpv Posted at: 2018-12-03T11:27:29.647Z Reads: 234

```
I am 100% sure the remote will be fine mate:-)
Very professional and nicely done
High five for the hard work
```

---
## \#171 Posted by: PickSix24 Posted at: 2018-12-03T16:48:33.483Z Reads: 234

```
Feel free to ship mine, I’ve got the batteries you’re using. Either way it’s cool.
```

---
## \#172 Posted by: Jansen Posted at: 2018-12-03T19:38:27.969Z Reads: 240

```
Hells yeah! Can't wait and soooo very stoked for this. Keep up the hard work brotha! Do you have an idea on how long it will take to ship to the US...? I can't remember if you mentioned that somewhere or not....?

Thanks again so much!
```

---
## \#173 Posted by: sofu Posted at: 2018-12-03T21:14:00.244Z Reads: 235

```
Were you able to ship the no battery remotes?
```

---
## \#174 Posted by: Gaza65 Posted at: 2018-12-04T02:58:26.047Z Reads: 239

```
How much for one of these when there ready?
```

---
## \#175 Posted by: reedbryson Posted at: 2018-12-04T03:17:17.735Z Reads: 242

```
I want one!
```

---
## \#176 Posted by: jbruce Posted at: 2018-12-04T04:17:25.643Z Reads: 246

```
yeah, me too!
```

---
## \#177 Posted by: StefanMe Posted at: 2018-12-04T06:41:29.514Z Reads: 247

```
Yes. remotes without batteris goes out tomorrorw! The remotes with batteries as soon as the other batteries arrive. 

@all sorry guys. I want to send the first batch out, get response from all users and then maybe we start a next batch!
```

---
## \#178 Posted by: Gaza65 Posted at: 2018-12-04T07:01:25.789Z Reads: 246

```
Next batch then...
```

---
## \#179 Posted by: Jansen Posted at: 2018-12-04T10:11:06.763Z Reads: 245

```
IS that a for sure departure date you think @StefanMe? Thursday for battery peeps like me....?
```

---
## \#180 Posted by: StefanMe Posted at: 2018-12-04T10:29:29.170Z Reads: 246

```
Yes. I ordered the batteries Monday. 2-4 days delivery time. I guess they ll come tomorrow... we’ll see ;)
```

---
## \#181 Posted by: PickSix24 Posted at: 2018-12-05T01:35:45.414Z Reads: 233

```
any update on the no battery remotes ?
```

---
## \#182 Posted by: StefanMe Posted at: 2018-12-05T07:35:20.752Z Reads: 244

```
Nope. 😛 they’re go out in the evening I guess.. the remotes with batteries go out tomorrow probably
```

---
## \#183 Posted by: StefanMe Posted at: 2018-12-05T22:38:29.344Z Reads: 252

```
![image|666x500](upload://ffQbIn0D9nUGSknK4OJoKQA0L9e.jpeg) 

All batteries arrived! I ll crimp then tomorrow at work and they ll leave my house tomorrow evening ;)
```

---
## \#184 Posted by: Kug3lis Posted at: 2018-12-05T23:30:45.994Z Reads: 254

```
Ahm I haven't read much of this topic, but I just saw that you using 12V voltage regulator probably something like  LM2576 and you will be connecting like lamps and loads more than 0.5A you will definitely will need radiator because those fckers heat up as their efficiency is pretty low like 75% so converting 42V to 12V 3A will be like around 10W of heat produced or etc.

Also, LM2576 has an HV version which has a higher input voltage (60V) than its normal version (40V) so it would work with up to 13S batteries :)

But anyway looks like good design and cool looking remote, it is nice to see innovation happening in remotes section :)
```

---
## \#185 Posted by: sofu Posted at: 2018-12-06T03:55:35.929Z Reads: 243

```
Wait so does that mean all remotes will ship with a battery then? 😅
```

---
## \#186 Posted by: StefanMe Posted at: 2018-12-06T08:16:45.560Z Reads: 248

```
@Kug3lis  
I checked this before, and they didnt heat up that  much... thats strange. I ll check this again. Thanks for the advise. 
I already use the HV version :) thats not the problem. But other components like capacitors and diods are the bottleneck. I upgraded them already.

I like your work! Unfortunitly i missed your black friday thing.

@sofu looks like i ll ship all remotes with batteries. Makes no sense becuase of one or two days to split them
```

---
## \#187 Posted by: Kug3lis Posted at: 2018-12-06T08:28:04.606Z Reads: 241

```
I know... 63V capacitors are freaking huge :D Maybe it was just my use case but idea that around 25% will be let out as heat so keep that in mind :slight_smile:
```

---
## \#188 Posted by: StefanMe Posted at: 2018-12-06T08:34:05.919Z Reads: 233

```
I am always thankful about hints about safety ;)
```

---
## \#189 Posted by: sofu Posted at: 2018-12-06T08:34:43.570Z Reads: 231

```
Sounds good to me! I'm not in a super rush, just curious :slight_smile:
```

---
## \#190 Posted by: tricky-fpv Posted at: 2018-12-06T17:10:10.755Z Reads: 238

```
I am running my headlights off a 20Amp bec:-)
My headlights suck allmost 3Amp
```

---
## \#191 Posted by: tricky-fpv Posted at: 2018-12-06T17:11:24.576Z Reads: 244

```
![20181206_181041|281x500](upload://dbnBu2loKkYuJiRdo641RlnpOha.jpeg)
```

---
## \#192 Posted by: StefanMe Posted at: 2018-12-06T17:11:42.283Z Reads: 236

```
holy shit! Thats a lot! U can also use this 12V output just for control your own BEC. but we ll see...
```

---
## \#193 Posted by: tricky-fpv Posted at: 2018-12-06T17:12:44.640Z Reads: 227

```
I have the basic model from u i believe.
But hey just darn happy to have a good remote soon:-)
Cruise control yihaa
Speed
Voltage
```

---
## \#194 Posted by: Jansen Posted at: 2018-12-06T17:30:00.684Z Reads: 217

```
They going out today hopefully? I sure am hoping!!! Thanks again
```

---
## \#195 Posted by: StefanMe Posted at: 2018-12-06T17:37:35.119Z Reads: 223

```
They go out tomorrow from the company where I work for. They told me its faster than a private shipping. (and just a bit cheaper!) so I hope u ll get the remote soon! I am totally happy when u get those things and give me feedback about stability ect. anyway, the first batch will get updates for sure is we face some problems!
```

---
## \#196 Posted by: Skirra Posted at: 2018-12-06T17:57:03.114Z Reads: 220

```
Have you thought of implementing 18650 battery instead of that little lipo? Would make a lot sense and way better battery life. With fine positsioning the width of the remote would stay same.
```

---
## \#197 Posted by: StefanMe Posted at: 2018-12-06T18:14:55.911Z Reads: 226

```
Hard to fit the battery in... the Feather, display and all the electronics need space... Why not using the 502535? I guess they work fine and have a really long battery life in my opinion.
```

---
## \#198 Posted by: Skirra Posted at: 2018-12-06T18:34:47.272Z Reads: 233

```
[quote="StefanMe, post:197, topic:74084"]
502535
[/quote]

Little lipos tend to degrade in time faster than liions. Also most diy folks out there have some spare 18650 laying around and you can keep one battery charged at all times in case you need quick replacement. This is ofcourse with the idea of taking the battery out if needed. If you look at the electronic cigaret boxes then you can see how small they can be made :slight_smile: 
You can share the .step files. I might have a look into this.
```

---
## \#199 Posted by: Friskies Posted at: 2018-12-06T18:41:57.633Z Reads: 220

```
Seems a bit overkill for the purpose. When do you need a cell that is that large for a controller?
```

---
## \#200 Posted by: StefanMe Posted at: 2018-12-06T19:35:00.633Z Reads: 228

```
its cool if u build in like a software OFF for the remote. because u can switch off the remote into a standby mode, where the remote just needs a few mA. 

I build this into the remote for an power safe mode. If the remote is not connected to a board for more then 10/30 minutes, it switches off to safe battery... in case u forgot to switch it off. Then its cool u still have power after a week or something.
```

---
## \#201 Posted by: tricky-fpv Posted at: 2018-12-06T23:57:57.088Z Reads: 208

```
Excited!!!!
```

---
## \#202 Posted by: Jansen Posted at: 2018-12-07T00:37:45.939Z Reads: 205

```
did your work say how long it takes to get to the US typically by chance? Couple days? Couple weeks?
```

---
## \#203 Posted by: StefanMe Posted at: 2018-12-07T07:58:37.775Z Reads: 204

```
I ask them later. but i think 2 weeks to your door max. Depends on what we have to ship there.
```

---
## \#204 Posted by: PickSix24 Posted at: 2018-12-07T13:22:12.523Z Reads: 197

```
Will we be getting tracking numbers ?
```

---
## \#205 Posted by: StefanMe Posted at: 2018-12-07T13:39:43.044Z Reads: 202

```
I hope. I don’t know till yet.
```

---
## \#206 Posted by: tricky-fpv Posted at: 2018-12-07T13:44:33.553Z Reads: 206

```
The plan is to send them today correct?
From germany right?
```

---
## \#207 Posted by: StefanMe Posted at: 2018-12-07T14:37:38.101Z Reads: 205

```
yes :) they are already in the shipping department in my company
```

---
## \#208 Posted by: tricky-fpv Posted at: 2018-12-07T15:22:03.245Z Reads: 207

```
Whoopwhoop!!!
The end game......
```

---
## \#209 Posted by: tricky-fpv Posted at: 2018-12-08T09:46:47.575Z Reads: 206

```
Any updates? Tracking nrs?
```

---
## \#211 Posted by: StefanMe Posted at: 2018-12-08T10:26:27.563Z Reads: 206

```
Nope.., I ll not get tracking numbers for all remotes. Depend on the country...

I ll get the tracking Nummer on Monday or Tuesday. Takes a bit time. It’s a big company ;)
```

---
## \#212 Posted by: sofu Posted at: 2018-12-10T20:24:42.198Z Reads: 205

```
I hope for our almost $200 sake we will get tracking numbers... shipping packages to big cities is usually atrocious and if (when) something goes wrong it's way easier to get some kind of result with a tracking number than without... 😬Thank you for your hard work though, I hope everything will work out :D
```

---
## \#213 Posted by: StefanMe Posted at: 2018-12-10T20:37:25.504Z Reads: 204

```
I hope so too!!! But they told me all packages are with insurance... so there must be a tracking number. I ll inform u all as soon as I get something! Minimal all remotes outside Europe will have tracking numbers... sorry its a bit strange.
```

---
## \#214 Posted by: sofu Posted at: 2018-12-10T20:48:48.932Z Reads: 207

```
It's ok, you're doing the best you can! Thank you!
```

---
## \#215 Posted by: tricky-fpv Posted at: 2018-12-11T00:40:15.574Z Reads: 208

```
I agree for 150euros or whatever i paid i would expect a tracking nr to be honest.
Would be nice to be able to see when the delivery date is expected:-)
Looking forward to seeing the remote.
So darn sick of my cheapy remote. Dont get me wrong it works but a decent remote will be sooooo nice:-)
```

---
## \#216 Posted by: PickSix24 Posted at: 2018-12-11T02:08:28.838Z Reads: 211

```
Agree, tracking would be really nice. Can’t wait to have a really nice remote.
```

---
## \#217 Posted by: Gaza65 Posted at: 2018-12-11T03:12:11.624Z Reads: 210

```
Still waiting for your remote to come...tell me how much better is this one compared to the one you sent me...and how much are these again...I might put in for the next batch...
```

---
## \#218 Posted by: jbruce Posted at: 2018-12-11T03:13:06.559Z Reads: 210

```
Does this remote have an odometer feature is would you be willing to put that in?
```

---
## \#219 Posted by: StefanMe Posted at: 2018-12-11T06:54:18.242Z Reads: 209

```
I go to the shipping office in our company this evening and ask them again... I also want tracking numbers, because of the expensive parts 😂 

I also send u all some spare springs, if the tension from the spring inside is to strong, u can simply exchange the spring...
```

---
## \#220 Posted by: StefanMe Posted at: 2018-12-11T18:15:21.752Z Reads: 206

```
I got updates!!! Tomorrow u ll get tracking numbers 😂 don’t ask how... I had a big fight with the shipping department 🤦🏻‍♂️
```

---
## \#221 Posted by: PickSix24 Posted at: 2018-12-11T21:35:44.199Z Reads: 201

```
Great news , thanks for following up.
```

---
## \#222 Posted by: Jansen Posted at: 2018-12-11T21:51:22.985Z Reads: 195

```
F)(#*K YES! 

10char
```

---
## \#223 Posted by: Jansen Posted at: 2018-12-11T21:51:50.227Z Reads: 200

```
Any final pics of how they all turned out....? The suspense is killing me!!!!
```

---
## \#224 Posted by: StefanMe Posted at: 2018-12-11T21:57:54.755Z Reads: 201

```
Hmm i think i have some photos ok my other phone... I ll look tomorrow :)
```

---
## \#225 Posted by: StefanMe Posted at: 2018-12-12T17:36:36.800Z Reads: 208

```
Hey guys, I have the papers at home. I am super busy, I ll send u the tracking ids in the night or tomorrow morning... 

https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084

but at the moment i dont have remotes for sale
```

---
## \#226 Posted by: tricky-fpv Posted at: 2018-12-13T08:22:55.747Z Reads: 195

```
Didn.t u send them last week friday?
From germany i shouls have it allready or did somthing go wrong?
Thanks for the tracking anyhows:-)
```

---
## \#227 Posted by: StefanMe Posted at: 2018-12-13T08:43:20.815Z Reads: 194

```
I gave them to the shipping department on Friday... that doesnt mean they are on the way unfortunitly. Thats why i had so much trouble with them. I hope they push it now! But this should go fast now. The parcels are already picked up here!
```

---
## \#228 Posted by: tricky-fpv Posted at: 2018-12-15T09:12:09.876Z Reads: 189

```
Did u find those photos of the finished remotes?
```

---
## \#229 Posted by: tricky-fpv Posted at: 2018-12-15T09:13:23.263Z Reads: 192

```
And did u test them for reliability and connection.
Friend of mine has the photon remote and its very poor with connection:-(
Pretty sad as it was not cheap
```

---
## \#230 Posted by: StefanMe Posted at: 2018-12-15T10:05:46.305Z Reads: 201

```
I made a quick hardware test with all remotes! Includes also the connection to receiver. The connection was good on all remotes! This should not be a problem :slight_smile:

I read a lot about the photon remote... its a very nice remote, but the people have some big issues with it unfortunately. And the guy who build this remote is nearly lost in space and didn't response since weeks. Hopefully he is fine, because building this remotes while u have other pressure from work or whatever can kill u.

Some picture? I ll find some... :) forgot about this!
```

---
## \#231 Posted by: StefanMe Posted at: 2018-12-15T10:08:48.150Z Reads: 223

```
here are some pictures from the build phase

![IMG_7764|375x500](upload://7wuxRc5Lpb2hij2hCdkC8lmPCrW.jpeg)
![IMG_7872|375x500](upload://iF7AmARPxFS9eSj51HUJvNsvYir.jpeg) 
![IMG_7870|375x500](upload://9FNQnAt3u1VC7jFNj2COsBQ6unt.jpeg)
```

---
## \#232 Posted by: kiryl Posted at: 2018-12-15T15:46:55.029Z Reads: 209

```
Hey Stefan ! You said you had tracking id's? Where could I get mine?
```

---
## \#233 Posted by: StefanMe Posted at: 2018-12-15T16:07:53.185Z Reads: 212

```
U didn't get one? I check this tomorrow... I am out of home at the moment. All remotes are already on the way!
```

---
## \#234 Posted by: Zentaria Posted at: 2018-12-15T18:21:55.507Z Reads: 218

```
![IMG_20181215_192048|690x388](upload://iORVtXNLt4jhkpq1b0qOM0fY22U.jpeg)

Already arrived. Lol. Any Guides to install it? Dont want to make anything wrong😂
```

---
## \#236 Posted by: PickSix24 Posted at: 2018-12-15T18:53:06.084Z Reads: 218

```
So jealous, I’m in the US so maybe next week sometime.
```

---
## \#237 Posted by: tricky-fpv Posted at: 2018-12-15T19:18:40.894Z Reads: 219

```
Darnnit where is the remote taking ages.
Was expecting faster from germany to holland.
But seems like snow tonight so riding is not possible anyways.
```

---
## \#238 Posted by: StefanMe Posted at: 2018-12-15T20:05:04.004Z Reads: 218

```
Fuck guys!!! Didn’t expect that they are allready arrived! 

I am drunk at the „Tollwood“!!!

I ll responded tomorrow!! 

![image|375x500](upload://wv3PbRAnYDjywNuhs5RyRy8oYYF.jpeg)
```

---
## \#239 Posted by: StefanMe Posted at: 2018-12-15T20:06:03.388Z Reads: 215

```
Omg I forgot a screw kn your remote?!?! Shit! Man I ll send u some screws!
```

---
## \#240 Posted by: kiryl Posted at: 2018-12-16T20:34:11.404Z Reads: 204

```
You got my tracking code Stefan? :slight_smile: Thanks!
```

---
## \#241 Posted by: StefanMe Posted at: 2018-12-17T06:12:57.236Z Reads: 206

```
I send u a message!
```

---
## \#242 Posted by: tricky-fpv Posted at: 2018-12-18T13:22:05.275Z Reads: 204

```
Dammit! U sent me the wrong one:-(
```

---
## \#243 Posted by: tricky-fpv Posted at: 2018-12-18T13:22:53.936Z Reads: 205

```
I ordered the basic version because i have 0 space in my enclosure man. This is never gonna fit
```

---
## \#244 Posted by: tricky-fpv Posted at: 2018-12-18T13:31:10.424Z Reads: 211

```
![15451393781114511616748438674393|281x500](upload://j2ySLFBEd9wDfAd49hym6KlQD3F.jpeg)
```

---
## \#245 Posted by: totalgeek9224 Posted at: 2018-12-18T13:32:40.553Z Reads: 208

```
..........
u forreal man?
```

---
## \#246 Posted by: tricky-fpv Posted at: 2018-12-18T13:36:52.178Z Reads: 212

```
Yes foreal
The basic reciver is much smaller and i needed and paid for that one but got this one in and i cant use it because i have 0 space 
Really bummed about this:-(
```

---
## \#247 Posted by: tricky-fpv Posted at: 2018-12-18T13:40:40.881Z Reads: 213

```
![IMG_20181215_192048|690x388](upload://iORVtXNLt4jhkpq1b0qOM0fY22U.jpeg) 
Thats the reciver i ordered.
Remote is fantastic i wont lie there really sweet.
Just got the wrong reciever:-(
```

---
## \#248 Posted by: bevilacqua Posted at: 2018-12-18T13:53:06.080Z Reads: 206

```
just send it back, im sure Stefan will send you the correcto one. Mistakes can happen. I've seen you complain way too much... This is not a product you buy from a normal vendor, it is still in developement and all the work is done by one guy: Software, Hardware, 3d Printing etc etc. Thats a ton of work that just consumes a lot of time

The purpose of a thread is to discuss porduct/topic related matters. If you got any personal problem please deal with it via PM instead of posting countless messages, don't be so childish
```

---
## \#249 Posted by: tricky-fpv Posted at: 2018-12-18T13:56:40.906Z Reads: 199

```
I agree and i am not bashing at all. The remote is fantastic i am extremely impressed. Just sucks i cant use it yet. 
Wish i did have space for it but enclosure is tight very tight with space:-(
```

---
## \#250 Posted by: totalgeek9224 Posted at: 2018-12-18T14:02:19.932Z Reads: 199

```
My point is that clearly it was an innocent mistake. He sent you a product with a higher value than what you ordered: he lost money as it is, and perhaps even has someone with the wrong receiver- someone who paid for something more, and received less. Perhaps there's a language barrier, but as @[bevilacqua](https://www.electric-skateboard.builders/u/bevilacqua) said, Stefan is working hard on these and is a one-man team. 
Just next time instead of "Dammit! U sent me the wrong one:-( / I ordered the basic version because i have 0 space in my enclosure man. This is never gonna fit" it could be "Hey man, it seems that you might've sent me the wrong unit, could you get in touch? Thanks"
```

---
## \#251 Posted by: tricky-fpv Posted at: 2018-12-18T14:08:04.928Z Reads: 204

```
Calm your tits guys. 
I agree i could have said it better yes i agree.
Mistakes can be made of course.
Just got very excited to finnaly have a good remote and put it in today. 
Was just very disappointed thats all.
I really wish i had the space to fit it in i really do. But just not gonna work. The remote looks and feels amazing very impressed did a great job!.
And the soldering on the reciever is really good.
```

---
## \#252 Posted by: totalgeek9224 Posted at: 2018-12-18T14:09:30.181Z Reads: 206

```
https://media.giphy.com/media/GBXHuE4ZdXq12/giphy.gif
```

---
## \#253 Posted by: tricky-fpv Posted at: 2018-12-18T14:26:00.921Z Reads: 206

```
Why didnt i make more room in my enclosure! Lol.
Headlight function is pretty sweet i will say
```

---
## \#254 Posted by: StefanMe Posted at: 2018-12-18T14:26:42.526Z Reads: 207

```
@tricky-fpv

i am so sorry :frowning: i can fully understand your disappintment! I ll send u another one tomorrow! I got a spare one at home! That sucks! I checked my private order list and it looks like i made the wrong entry for u! In the order sheet is BASIC RECEIVER and in my list is ADVANCED SELECTED. 

Sorry again.


Thanks  @totalgeek9224 and @bevilacqua
```

---
## \#255 Posted by: tricky-fpv Posted at: 2018-12-18T14:27:49.639Z Reads: 197

```
My bad for attacking the way i did.
(My bad mate sorry)
Whats the spring for?
To make it heavyer on the wheel or losser?
```

---
## \#256 Posted by: StefanMe Posted at: 2018-12-18T14:29:32.509Z Reads: 195

```
If the tension for the remote is to strong, u can cut the spring to your preferred lenght and strength.

The breaklight and headlight feature is really nice... sad that u don’t have enough space for it!
```

---
## \#257 Posted by: totalgeek9224 Posted at: 2018-12-18T14:34:27.981Z Reads: 193

```
Speak of which, when are you gonna do a full length video of this so people can see its full feature set? :smiley:
```

---
## \#258 Posted by: StefanMe Posted at: 2018-12-18T14:50:20.895Z Reads: 212

```
I already startet a little guide... not finished yet. Should be ready until thrusday... :slight_smile:

Maybe i can make a video at the weekend toghether with @bevilacqua . My board is not functional, because of my broken Foxbox. I allready got a replacment but with wrong connector.   Unfortunitly bevilacqua is super busy like me. 

![docx%20-%20Word|391x500](upload://uJOnaIEEfysS9pK6Cl8RVbBacWB.jpeg)
```

---
## \#259 Posted by: totalgeek9224 Posted at: 2018-12-18T14:59:23.933Z Reads: 202

```
If i can help in any way with the write up, let me know!
```

---
## \#260 Posted by: sofu Posted at: 2018-12-18T22:03:08.840Z Reads: 204

```
Hey @StefanMe I'm not sure if I'm the only US person seeing this but it seems there's been no movement on mine for at least 4 days... Is there anything goin on? I know HAYA had issues with exporting to the US...
```

---
## \#261 Posted by: Surfer Posted at: 2018-12-18T22:18:21.454Z Reads: 211

```
Just received mine, omg!! It's really nice ergo feeling! Thumb wheel and killswitch are really pleasant to play with, and the 3d print is really good, mad props for your printing skills bud.
Just couple questions Stefan, don't know why but I can't get rid off the estop, I disable but still in there activated, I tried well, no luck.
Something to improve, the antenna on the Rx didn't last more than 5 minutes, just fell down.
Just quick silicone wire soldering and up & running again.
I'm waiting for your write up about the connections on esc side.
Thanks buddy I like it :)
```

---
## \#262 Posted by: StefanMe Posted at: 2018-12-18T22:28:20.842Z Reads: 203

```
Hmm strange... i ll call them tomorrow! I hope everything is fine.

@Surfer 
Strange... can u try something for me? Just go into settings menu and make all the changes u need (estop, wheel size, throttle ect...) then before u leave the settings menu, switch off the receiver, then switch off the remote. The power on again everything. Does it work now?

Thanks for the advice of the receiver antenna wire... maybe a big drop of hot glue on the solder joint to make the connection more rigid?
```

---
## \#263 Posted by: Surfer Posted at: 2018-12-18T22:39:39.024Z Reads: 191

```
It did not make any difference, all other settings I can change them without any problem, with the regular procedure. ( Is not a problem for me most probably is a nice feature )
About the antenna, the hot glue for sure will help, but I think also better to use a wire with more copper inside.
```

---
## \#264 Posted by: tricky-fpv Posted at: 2018-12-18T22:41:05.170Z Reads: 185

```
I noticed that too. That the green wire on the reciver would not last long. Is any silicone wire usable?
Really love the remote its impressive
```

---
## \#265 Posted by: StefanMe Posted at: 2018-12-18T22:48:04.182Z Reads: 193

```
No that doesn’t make a difference, the amount (thickness) of the cooper inside makes no difference in signal strength... the length of the wire is very important! In EU versions it must
be 15-16cm! In US and AUSTRALIEN it Mist
Be 7.5–8cm

The best wire u can use is a solid wire... but it’s not worth it. I tested it. If u push the menu button, u can cycle to the CONNECTION page. The big value there is the RSSI. The higher the value, the better the connection (starts at -30, critical under -70) keep in mind -30 is higher than -40 ;)

Ok, I ll check this tomorrow...! MAYBE it’s just an visual problem... 

I am not shure that tue message on the remote (E-Stop armed and estop actrivated) is connected to the settings. I ll explain it tomorrow in more detail.
```

---
## \#266 Posted by: Surfer Posted at: 2018-12-18T22:51:57.908Z Reads: 180

```
I mean more copper to hold better the movements in the solder spot.
```

---
## \#267 Posted by: StefanMe Posted at: 2018-12-18T22:54:34.872Z Reads: 184

```
Ah ok, feel free to exchange the wire... sorry, i Never had any issues with that. If your build is finished, add a big shrink tube over the hole receiver except of the plug and the reset button. That should hold the antenna in good place.
```

---
## \#268 Posted by: tricky-fpv Posted at: 2018-12-18T22:56:56.649Z Reads: 191

```
Jist noticed that my tactical switch is not working.
Was working when i got it the afternoon.
But was just trying to change some settings but i can use the trigger switch it will not activate
Any ideas?
```

---
## \#269 Posted by: StefanMe Posted at: 2018-12-18T22:59:29.340Z Reads: 198

```
Hmm u hear the click from the trigger? I write I a pm.
```

---
## \#270 Posted by: tricky-fpv Posted at: 2018-12-18T23:30:48.321Z Reads: 208

```
![15451757872917955302500478462095|281x500](upload://z9H2Qu5PovToeN2eGNbGF5E6Pyv.jpeg) 

As an update was a very simple somthing. The right pin was not soldered so connection was poor. Easy fix:-)
```

---
## \#271 Posted by: PickSix24 Posted at: 2018-12-19T03:19:51.206Z Reads: 207

```
Same thing with mine
```

---
## \#272 Posted by: StefanMe Posted at: 2018-12-19T04:08:38.496Z Reads: 204

```
Strange... can u please add a bit solder to the joint?

It looks like I tried to clean up the solder joint and accedently removed to much solder...
```

---
## \#273 Posted by: StefanMe Posted at: 2018-12-19T07:18:50.381Z Reads: 204

```
Looks like its just a wrong handling in the remote itself. The estop is OFF, but the remote is showing ESTOP ACTIVATED, I ll change the message from ESTOP ACTIVATED to CONNECTION LOST when estop is OFF.

Anyway... keep it activated :slight_smile: its just too cool to deactivate it ;).
```

---
## \#274 Posted by: tricky-fpv Posted at: 2018-12-19T13:33:34.918Z Reads: 201

```
I am noticing if i wish to change trigger to killswitch it says communication failed

?
```

---
## \#275 Posted by: bevilacqua Posted at: 2018-12-19T13:37:17.566Z Reads: 198

```
Hi Sofia, my decks that were sent from germany to the US via regular DHL shipping sat for 5 days in the logistics centre for export shippings. 
Its christmas and therefore logistics hell, could be just that 

@StefanMe  , if you call them you could open a official reclamation, maybe that helps
```

---
## \#276 Posted by: StefanMe Posted at: 2018-12-19T13:46:55.556Z Reads: 194

```
Have u already paired your receiver?

Second point in the setting menu...
```

---
## \#277 Posted by: PickSix24 Posted at: 2018-12-19T13:48:18.033Z Reads: 197

```
Hopefully we see some movement soon on the US remotes 🤞🏻
```

---
## \#278 Posted by: tricky-fpv Posted at: 2018-12-19T13:49:13.531Z Reads: 196

```
I thought changing settings in the remote as such would not be needed to have it connected 
But i do i take it?
```

---
## \#279 Posted by: StefanMe Posted at: 2018-12-19T13:50:22.359Z Reads: 192

```
Some settings need changes in the receiver as well ;)... specially all safety features...
```

---
## \#280 Posted by: tricky-fpv Posted at: 2018-12-19T13:53:45.160Z Reads: 194

```
Can i connect the reciver to a 5volt supply and test it?
The red and black wire correct? To a 5volt
```

---
## \#281 Posted by: StefanMe Posted at: 2018-12-19T13:54:52.736Z Reads: 187

```
no, use the USB to power the receiver...
```

---
## \#282 Posted by: tricky-fpv Posted at: 2018-12-19T14:00:09.783Z Reads: 191

```
Right got it thanks.
And the estop cant be turned off?
```

---
## \#283 Posted by: StefanMe Posted at: 2018-12-19T14:02:35.266Z Reads: 181

```
Yes of course...but I do not recommend it. The remote just shows a wrong message. The message should be “connection lost” instead of “estop activated”
```

---
## \#284 Posted by: Jansen Posted at: 2018-12-19T16:53:20.507Z Reads: 176

```
[quote="sofu, post:260, topic:74084"]
I’m not sure if I’m the only US person seeing this but it seems there’s been no movement on mine for at least 4 days… Is there anything goin on? I know HAYA had issues with exporting to the US…
[/quote]

No me too.... It hasn't done anything besides get picked up and leave for like 5+ days now.... grrrrrrr
```

---
## \#285 Posted by: StefanMe Posted at: 2018-12-19T17:26:41.284Z Reads: 176

```
Sorry guys... o called them and they sailed everything is fine :persevere: he can’t tell me more. I ll call them tomorrow again. Sorry... I used a type of priority package and they told me it should arrive working 6-10 days. Strange that all packages are still here in Germany :frowning:
```

---
## \#286 Posted by: Jansen Posted at: 2018-12-19T17:54:26.045Z Reads: 179

```
[quote="StefanMe, post:285, topic:74084"]
still here in Germany :frowning:
[/quote]

Well shit fuck me... lol. Not your fault. Too dam excited to get it and use it though, especially after seeing these positive reviews people are giving about the quality and shape above. Can't wait even more now, dammit!

They couldn't even give you anything more than that as far as when they might be leaving Germany or when we can expect them to arrive in the US at all....?
```

---
## \#287 Posted by: sofu Posted at: 2018-12-19T20:11:49.292Z Reads: 180

```
No worries, I was only concerned because I have another package shipped on the same day also by DHL that cleared customs in a few hours and is already going to be delivered to me tomorrow, but it wasn't electronics...
```

---
## \#288 Posted by: PickSix24 Posted at: 2018-12-19T20:18:29.169Z Reads: 179

```
Aww bummer, at least it’s on it’s way.
```

---
## \#289 Posted by: PickSix24 Posted at: 2018-12-20T05:41:52.785Z Reads: 198

```
For those in the US , I’ve got some movement !!
![image|281x500](upload://aMOpKOUvi0jM0uuSq3HnToY7WxJ.png)
```

---
## \#290 Posted by: StefanMe Posted at: 2018-12-20T09:27:02.894Z Reads: 196

```
Hey guys! Here is the first version of the manual for the remote...

Big thanks to @totalgeek9224 who wrote this stuff together for me! :green_heart:

https://docs.google.com/document/d/17HkXw-V4jRMWkZ8O-B_I8DazQVeFwYYrkrsUbQE8zrY/edit
```

---
## \#291 Posted by: Darkie02 Posted at: 2018-12-20T22:17:22.391Z Reads: 188

```
Is it just the us ones been held up.

Still waiting in the uk no sign yet but I’m presuming it’s just Xmas rush.
```

---
## \#292 Posted by: Mich21050 Posted at: 2018-12-20T22:22:40.376Z Reads: 188

```
Is there any chance of still getting one? :smile:
```

---
## \#293 Posted by: sofu Posted at: 2018-12-22T09:53:06.776Z Reads: 187

```
My US remote has been processed through New York! Shouldn't be too long now :smiley:
```

---
## \#294 Posted by: PickSix24 Posted at: 2018-12-22T15:44:56.478Z Reads: 180

```
Lucky you !!! Mine still hasn’t hit the US 😢
```

---
## \#295 Posted by: StefanMe Posted at: 2018-12-23T19:47:04.137Z Reads: 180

```
No Sorry... not in the next 1-2 months. I wait for the feedback from the first batch and then we ll see.
```

---
## \#296 Posted by: tricky-fpv Posted at: 2018-12-24T14:06:58.438Z Reads: 186

```
I am trying to wire up my advanced reciever but dont understand the wiring.
I have 5 wires coming out the reciver.
The diagram is very unclear coupd use some help here please thanks
```

---
## \#297 Posted by: tricky-fpv Posted at: 2018-12-24T14:10:16.240Z Reads: 189

```
![1545660581332264086541719215927|281x500](upload://xDkxDCKU1iwq9vitbLoSnTWOsB1.jpeg)
```

---
## \#298 Posted by: totalgeek9224 Posted at: 2018-12-24T14:19:21.296Z Reads: 190

```
Are you referring to the diagram on the instructions? Could you elaborate as i believe it is a descriptive as possible in regards to the pinout of the reciever. 
Furthermore, what VESC do you have? Maybe we can give some specifics for your case :)
```

---
## \#299 Posted by: tricky-fpv Posted at: 2018-12-24T14:21:19.114Z Reads: 193

```
I have Focbox esc.
And my old reciver is connected to the ppm i believe
![15456612530494657950461283660927|281x500](upload://rGJTmLhyZnDoGokjm9cgK3EfIck.jpeg)
```

---
## \#300 Posted by: tricky-fpv Posted at: 2018-12-24T14:27:41.777Z Reads: 196

```
![Screenshot_20181224-152512_Samsung%20Internet|690x388](upload://dUFPD62EbOhqSSIE4pijo0OJLC5.jpeg) 
Is this correct as i show in my photos from top to bottom
```

---
## \#301 Posted by: totalgeek9224 Posted at: 2018-12-24T14:30:55.114Z Reads: 190

```
No it appears it's the other way around. The red and black are the 5v and ground (respectively) as such they should be on the top 
Does that help?
```

---
## \#302 Posted by: totalgeek9224 Posted at: 2018-12-24T14:32:20.737Z Reads: 187

```
I didn't realise this was different between the different reciever, @StefanMe could you send me some photos of the feather advanced so I can implement this
```

---
## \#303 Posted by: tricky-fpv Posted at: 2018-12-24T14:33:22.188Z Reads: 188

```
Thats why i am so confused 
Red and black are +&- mostly. And it shows the basic version in the layout not the advanced
And the pwm is that the white wire from the ppm signal wires i need to use and the other 4 are the uart port as shown here ?![15456619808408717218199525473644|281x500](upload://1Wf9ks0KQ4cnnk2tsgEST0N4j74.jpeg)
```

---
## \#304 Posted by: tricky-fpv Posted at: 2018-12-24T14:34:59.101Z Reads: 186

```
![15456620744787935798608483123919|281x500](upload://om8XoWxyxWCCLVNgeYZ9uKStHRt.jpeg)
```

---
## \#305 Posted by: tricky-fpv Posted at: 2018-12-24T14:38:01.022Z Reads: 181

```
![15456621569386460784422129945200|281x500](upload://orbjMakQWQkVaSmQ3YgJhpoSMOr.jpeg) 
So the orange wire is pwm that connects to the white wire from the ppm port where my old nano is connected is this correct?
And the other 4 to the uart
```

---
## \#306 Posted by: bevilacqua Posted at: 2018-12-24T14:38:45.718Z Reads: 172

```
check the image I uploaded some days ago, I have the same receiver hooked up to a dual FB aswell
```

---
## \#307 Posted by: tricky-fpv Posted at: 2018-12-24T14:39:37.760Z Reads: 172

```
In this topic?
Could u upload the photo again if possible
```

---
## \#308 Posted by: bevilacqua Posted at: 2018-12-24T14:40:39.344Z Reads: 169

```
https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084/235?u=bevilacqua
```

---
## \#309 Posted by: totalgeek9224 Posted at: 2018-12-24T14:40:53.233Z Reads: 178

```
He's Talking about this one 
https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084/235?u=totalgeek9224
But @bevilacqua is this working for you? Because it contradicts the photo Stefan gave me 
 (this one)
https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084/300?u=totalgeek9224
```

---
## \#310 Posted by: bevilacqua Posted at: 2018-12-24T14:41:14.824Z Reads: 171

```
it is indeed...
```

---
## \#311 Posted by: bevilacqua Posted at: 2018-12-24T14:41:42.705Z Reads: 166

```
thats maybe the small receiver
```

---
## \#312 Posted by: tricky-fpv Posted at: 2018-12-24T14:41:44.657Z Reads: 162

```
Ok now i am really confused
```

---
## \#313 Posted by: bevilacqua Posted at: 2018-12-24T14:42:44.432Z Reads: 163

```
well, you are using the big one, am I right? then just copy my setup . That should do the trick :)
```

---
## \#314 Posted by: tricky-fpv Posted at: 2018-12-24T14:42:54.172Z Reads: 162

```
But wait wait.
Lets think.
The white yes should be ppm red and black speaks for its self and yellow orange should be rx tx. That make sense?
```

---
## \#315 Posted by: totalgeek9224 Posted at: 2018-12-24T14:43:08.230Z Reads: 166

```
Hm, well im confused but if it works it works.
@StefanMe i know its Christmas bud, but if you could clarify it would be great! 

Either way, @tricky-fpv, it looks like you have your 5v and ground switched in the photo you uploaded,  
https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084/305?u=totalgeek9224

where the 5v wire is supposed to be on the outside
```

---
## \#318 Posted by: tricky-fpv Posted at: 2018-12-24T14:51:39.254Z Reads: 153

```
Yes that looks correct
```

---
## \#320 Posted by: totalgeek9224 Posted at: 2018-12-24T14:55:18.022Z Reads: 159

```
no 5V should be red as we concluded (somehow) that the Featherbasic and FeatherAdvanced dont share the same pin layout based on orientation

You're personal friends with Stefan, right? Do you think you could consult him and then let us know?
```

---
## \#321 Posted by: tricky-fpv Posted at: 2018-12-24T14:55:41.481Z Reads: 161

```
Yes sorry the red and black are wrong i think?
```

---
## \#322 Posted by: bevilacqua Posted at: 2018-12-24T14:56:46.880Z Reads: 171

```
now im getting confused aswell. I dont have access to my board right now, dont worry he'll respond in some min.
```

---
## \#323 Posted by: StefanMe Posted at: 2018-12-24T14:57:36.526Z Reads: 176

```
![20|690x355](upload://d3FjLlpgD2ZaOSAjuN3N68ehQso.png)
```

---
## \#324 Posted by: sayekim Posted at: 2018-12-24T14:58:22.629Z Reads: 170

```
In this picture the text colours don’t match the wire colours.
```

---
## \#325 Posted by: StefanMe Posted at: 2018-12-24T14:58:54.411Z Reads: 168

```
The connection is exactly the same... just the orientation is wrong (180 degrees turned...)

U can use the same Cable for the small and the big receiver... lineup in the plug is the same. But the plug has an orientation. normal on small receiver, 180 degrees on big receiver.

Never trust colours :slight_smile:
```

---
## \#326 Posted by: hoeksame1 Posted at: 2018-12-24T14:59:37.792Z Reads: 152

```
your picture is not the same as totalgeek9224 send
```

---
## \#327 Posted by: totalgeek9224 Posted at: 2018-12-24T15:00:39.868Z Reads: 147

```
Yes the text colors are representing how it **should** be :)
```

---
## \#328 Posted by: totalgeek9224 Posted at: 2018-12-24T15:01:05.761Z Reads: 154

```
Trust his image, not mine, he is the creator after all
```

---
## \#329 Posted by: hoeksame1 Posted at: 2018-12-24T15:01:23.181Z Reads: 154

```
anyway, dont want to bother.. the remote looks sick ! :slight_smile:
```

---
## \#330 Posted by: StefanMe Posted at: 2018-12-24T15:01:34.591Z Reads: 157

```
No please don't look on colours!!! Some plugs are with different colours lined up! The colours are sometimes random from different manufactures
```

---
## \#331 Posted by: tricky-fpv Posted at: 2018-12-24T15:01:58.356Z Reads: 157

```
Allright got it.
Just the colours dont add up
Easy fix no worries thanks guys.
Just wanna try the remote even if the reciver dont fit in the enclosure
```

---
## \#332 Posted by: StefanMe Posted at: 2018-12-24T15:02:51.402Z Reads: 148

```
U still didn't get the new receiver?
```

---
## \#333 Posted by: sayekim Posted at: 2018-12-24T15:02:53.874Z Reads: 159

```
What do you mean never trust colours?

The wires have colours which I hope you should be able to trust to what they are. 

This is for sure correct. 

orange rx
yellow tx
white ppm
red 5v
black ground

Now if someone could send the correct diagram then you’re golden. 

omfg
```

---
## \#334 Posted by: totalgeek9224 Posted at: 2018-12-24T15:04:35.424Z Reads: 153

```
I did not know this! I'll remove my image and ive added yours into the manual
```

---
## \#335 Posted by: StefanMe Posted at: 2018-12-24T15:05:30.229Z Reads: 163

```
No. because the colours are not always the same. There is no norm for this. Please connect the wires like the picture. 

In future I ll take more care about this and try to match colours red 5v black ground ect.
```

---
## \#336 Posted by: tricky-fpv Posted at: 2018-12-24T15:05:48.706Z Reads: 173

```
![1545663903275791193425982993686|281x500](upload://jmcyMMQp5yVKT3BAWZALqLlyBJX.jpeg)  hell yeah sh works
```

---
## \#337 Posted by: totalgeek9224 Posted at: 2018-12-24T15:06:09.769Z Reads: 167

```
Awesome!!!!
```

---
## \#338 Posted by: StefanMe Posted at: 2018-12-24T15:06:36.737Z Reads: 165

```
looks so sexy :heart_eyes:
```

---
## \#339 Posted by: tricky-fpv Posted at: 2018-12-24T15:07:17.852Z Reads: 171

```
Impressive!
Like the vibration when board is armed too!!
Pleasure mode hahahaha
```

---
## \#340 Posted by: totalgeek9224 Posted at: 2018-12-24T15:07:34.375Z Reads: 171

```
Great work @StefanMe!! I hope this remote takes off
```

---
## \#341 Posted by: StefanMe Posted at: 2018-12-24T15:09:12.717Z Reads: 168

```
Can u please add the new picture for the RemoteAdvanced receiver to the manual? the Basic receiver is correct.

Oh man @totalgeek9224 u are damned fast :) thanks a lot!
```

---
## \#342 Posted by: sayekim Posted at: 2018-12-24T15:09:24.847Z Reads: 168

```
😂
Okay so the colours aren’t always the same but I sure hope you know which colour is which wire for this receiver. That surely matters to know what goes where.
```

---
## \#343 Posted by: swimmydude Posted at: 2018-12-24T15:10:30.906Z Reads: 162

```
I understand colors aren't always universal between manufactures and people but I was pretty sure the general consensus was that gnd was generally black and the positive/live wire was generally red?
```

---
## \#344 Posted by: StefanMe Posted at: 2018-12-24T15:10:42.069Z Reads: 159

```
Why? I don't understand the problem... in the maual is no colours... u have the pinout instead of colours. No one said red is 5v or something. just follow the pinout
```

---
## \#345 Posted by: StefanMe Posted at: 2018-12-24T15:11:26.446Z Reads: 159

```
I didn't get the wires before I lined up the plug on the PCB. I ll take care about this in the future. My fault, that I didn't give attention to this! Sorry guys!
```

---
## \#346 Posted by: tricky-fpv Posted at: 2018-12-24T15:13:33.101Z Reads: 146

```
When u have OCD the wires MUST match up hahahahaha
```

---
## \#347 Posted by: sayekim Posted at: 2018-12-24T15:13:44.008Z Reads: 144

```
I’m was just trying to help. I don’t have this awesome remote. 

So yeah you are of course absolutely right that the colours don’t matter, but that’s only true if these things come without any wires attached to them already right?
```

---
## \#348 Posted by: StefanMe Posted at: 2018-12-24T15:14:17.005Z Reads: 154

```
[quote="sayekim, post:347, topic:74084"]
attached
[/quote]

Just open wires to connect it by your own. Maybe next time its easier to do this also for the people. Then there is no confusion
```

---
## \#349 Posted by: swimmydude Posted at: 2018-12-24T15:15:40.468Z Reads: 160

```
Haha, no worries. The idea is to at least find which side of the wire is which if they at least know what gnd is and hopefully can avoid this whole process of figuring what's what. :laughing:
```

---
## \#350 Posted by: sayekim Posted at: 2018-12-24T15:23:04.517Z Reads: 170

```
My bad. It makes way more sense to what you were saying but still they have a certain colour order on the plug. 

Which is:
orange 
yellow
white
red
black

This usually translates to:

orange rx
yellow tx
white ppm
red 5v
black ground

Can I get a confirmed on that?
```

---
## \#351 Posted by: tricky-fpv Posted at: 2018-12-24T15:27:38.517Z Reads: 160

```
THIS IS SPARTAAA HAHAHA sorry lol.
But yeah makes sense. But easy job to change the wires around
```

---
## \#352 Posted by: PickSix24 Posted at: 2018-12-24T18:53:15.298Z Reads: 158

```
Ahhh all this remote talk , I’m still waiting for mine 🤣🤣, my Metr shipped way after and it arrived today 😢 Very excited for this remote
```

---
## \#353 Posted by: StefanMe Posted at: 2018-12-24T19:18:08.555Z Reads: 158

```
Strange because u also got the priority shipping... maybe because the METR is send by envelope?
```

---
## \#354 Posted by: tricky-fpv Posted at: 2018-12-26T23:42:45.599Z Reads: 164

```
Ok i have been problems changing any settings.
Whenever the remote is paired i try to change settings so i go into the settings amd the remote vibrates and unpairs and i need to repair it to the board. Cant seem to get it working correctly 
Still waiting for the reciver basic one so hoping it will come tomorrow fingers crossed.
No matter what setting i try to change it say communication failed and nothing changes apart from its not paired anymore and i need to re do that process over amd over again.
Bit confused 
Any ideas?
Remote is just badass i love it feels solid and great!
Hoping the basic version will be here tomorrow;-)
```

---
## \#355 Posted by: StefanMe Posted at: 2018-12-26T23:58:13.884Z Reads: 161

```
So remote is paired? U get a message “estop armed?”

Then u go into settings and try to change … for example “cruise control” to “killswitch”? Have u tried to change it a second time? Sometimes the timing from the receiver is not perfect… then u have to try it a second time.
```

---
## \#356 Posted by: tricky-fpv Posted at: 2018-12-27T00:35:51.348Z Reads: 154

```
I tryed it many many times.. every single time i go into settings it vibrstes as in connection lodt. Then i cant change settings if connection id lost
```

---
## \#357 Posted by: StefanMe Posted at: 2018-12-27T00:45:31.671Z Reads: 148

```
The vibration is normal when u join the settings menu. But then u should be able to change every setting. A short press on the MENU button(close to the display) will exit and u to the normal main screen. After a few seconds the estop will be armed again.
```

---
## \#358 Posted by: Jansen Posted at: 2018-12-27T01:01:18.492Z Reads: 156

```
Hey hey brotha, quick couple of questions for you....

I am super new to doing electronic stuff myself, soldering, etc, so please pardon my noob question when it comes to setting the remote up. Got it today though and couldn't be more stoked! Super nice looking and great feeling so can't wait to be using it.

I just started going through the guide you made and was just curious..... am I able to plug the receiver (I got the basic) right into my focbox and then pair it and I'm good to go?

Or what all do I need to do in order to hook this up to my VESC?

What are the extra couple parts you included for just to be certain?

Let me know when you can, hoping to get this set up and go for a ride in the next 30 mins or so if possible.

THanks again so much for your hard work Stefan!
```

---
## \#359 Posted by: totalgeek9224 Posted at: 2018-12-27T01:09:37.236Z Reads: 159

```
I think i may be able to answer some of these questions for you!
1. The only settings that (may) need to be changed for complete functionality on the VESC side are the following 3 things:
 Ensure that the Baud Rate for UART connection is 115200
 Use only CURRENT WITH BREAK, WITHOUT REVERSE
 Set the Control mode to PPM
Furthermore, when connecting to the focbox, know that you're not connecting the ppm cable that comes from the focbox directly into the receiver, but rather using the cable (that I believe is included, this is explained a bit further up and in the instructions in regards to how it's wired)
2. The extra parts that you speak of, I know of only the extra spring, which is used to increase/decrease the "tension" of the thumbwheel to your taste.

Hope that helps!
```

---
## \#360 Posted by: Jansen Posted at: 2018-12-27T01:12:24.575Z Reads: 158

```
[quote="totalgeek9224, post:359, topic:74084"]
Use only CURRENT WITH BREAK, WITHOUT REVERSE
Set the Control mode to PPM
[/quote]

Ok cool, thanks so much, I'll try and do these things right now and let you know how it goes. Am I not able to use watt made anymore then either so I am on the same page....?
```

---
## \#361 Posted by: totalgeek9224 Posted at: 2018-12-27T01:13:38.630Z Reads: 163

```
[quote="Jansen, post:360, topic:74084"]
watt made
[/quote]

Sorry? Im not sure i understand :p
```

---
## \#362 Posted by: Jansen Posted at: 2018-12-27T01:16:17.956Z Reads: 163

```
watt mode.
 only on ackmaniacs bldc tool....
```

---
## \#363 Posted by: StefanMe Posted at: 2018-12-27T01:20:30.494Z Reads: 171

```
I guess he mean “watt mode”. Watt should be also ok... u can give it a try... but be carefull. I never tested it with watt mode. Important
Is, that u use a mode with break and no reverse!

There is a spring to change the tensions if Au don’t like the build in one as @totalgeek9224 mentioned correctly ... a cable to connect to the vesc and very tiny LC-Filter if u have problems with the power supply to the receiver... it helps u if u have freezes or something on the receiver.
```

---
## \#364 Posted by: Jansen Posted at: 2018-12-27T01:28:45.707Z Reads: 174

```
Ok, got those couple things and just read through the guide you did. I didn't see anything about how the cruise control works, am I missing something or is it as simple as click the trigger switch when I want it to lock in at a certain speed.

And again pardon my electronic stupidity (taking my enclosure off now to hook it all up) but it the receiver plug and play or do I need to solder some wires?
```

---
## \#365 Posted by: sofu Posted at: 2018-12-27T06:40:52.111Z Reads: 178

```
Just got the remote, and wow this thing is so quality! Package was opened when it got here though, by customs no doubt, but everything seems to be present and accounted for. 

![IMG_4799|666x500](upload://mkFHKpj46oUYiZc8IUbMe2HTcqX.jpeg) 

(ignore the tear in the display, the refresh rate doesn't play well with my camera...)

I'm just curious though, why are the fets sticking up on one side like that?Is it just space constraints?

Also @StefanMe is it possible to get more advanced receivers if I wanted them :smiley:
```

---
## \#366 Posted by: tricky-fpv Posted at: 2018-12-27T10:34:01.818Z Reads: 174

```
![1545906799798555957351098428832|281x500](upload://amR62D6jBBlV8TlNJGAB4Jt3z6O.jpeg) 
Yeah yeah basic small one is in da house.
Hope this works nicely
```

---
## \#367 Posted by: bevilacqua Posted at: 2018-12-27T12:00:46.547Z Reads: 166

```
[quote="sofu, post:365, topic:74084"]
I’m just curious though, why are the fets sticking up on one side like that?Is it just space constraints?
[/quote]

standing straight they are quite tall, I have to bend mine a bit to fit the deck space/enclosure
```

---
## \#368 Posted by: totalgeek9224 Posted at: 2018-12-27T12:06:07.734Z Reads: 167

```
I think its because there could be a pico speaker behind them, which wouldnt allow for them to be folded back
Furthermore, standing up they have some room to "breath" given that they have nothing to conduct their heat to even if they were folded down. 
If youre feeling risky, i believe its safe to trim the top tabs down using something like a dremel but that **is completely at your own risk**
```

---
## \#369 Posted by: Surfer Posted at: 2018-12-27T12:28:14.990Z Reads: 174

```
@StefanMe, is a vibration feedback build in the remote?
```

---
## \#370 Posted by: PickSix24 Posted at: 2018-12-27T15:40:55.775Z Reads: 172

```
So jealous!!!!! 🤣Mine is still on the east coast somewhere.
```

---
## \#371 Posted by: Mich21050 Posted at: 2018-12-27T15:44:13.575Z Reads: 173

```
Ohh shut up.. I didn't even get one. :rofl:  ,:frowning: 
![](https://media.giphy.com/media/jkYhaCyVaTxqHLk2Yl/200w.gif)
```

---
## \#372 Posted by: tricky-fpv Posted at: 2018-12-27T15:58:29.040Z Reads: 170

```
Update.
Basic rx is in my enclosure and all is perfect 
Remote feels damn solid and works fantastic!!
Really does.
Only thing i could wished for is a small bizzer inside the remote that could work on the trigger as an option for bycycles infront of me as a warning.
That would be the cherry on top for me.
Really did good man with this first batch
High five for the effort dude
```

---
## \#373 Posted by: tricky-fpv Posted at: 2018-12-27T16:01:50.697Z Reads: 172

```
I have the cruise control on the trigger amd it works perfectly!
Warning vibrations work great too one thing i did not think of and this might be a good thing to think about.
I ride with left foot front 
And i ride with remote in my left hand.
So my palm covers the screen.
Did not even think about it but maybe an ootion to think of in the next batch mate
```

---
## \#374 Posted by: StefanMe Posted at: 2018-12-27T17:43:01.459Z Reads: 179

```
@tricky-fpv  Haha I am sorry... of course its a right hand version. Great that everything works. Give us feedback after a few rides what we can improve. 

I also thought about a horn or something, but then we need another button for this... like a splitted trigger... maybe in the future.

@Surfer yes it is :slight_smile:

@Jansen yes its just like that... go for a certain speed on the board and then hold the trigger at the throttle position as u want. The Trigger will lock the trigger position simulated at this point. If u break with the throttle or release the trigger, the cruise will cancel.

U just have to hook up your wiring like in the description manual. Set the Baudrate to 115200 in VESC and learn the new PPM signal like u did on your last remote.   

@sofu yes the its just to safe a little bit of footprint from the PCB. U can cut way the top of the metal part from the fets so safe some height. They are rated for a million amps or something. They will not get warm anyway. 

please before u put everything into place, try the lights and the breaks ect. outside of your board. Just to make sure there is no problem with heat from the step-down as someone before mentioned... I just use some of these LEDs Nichia NSDW570GS-K1 (5x)... its fucking awesome... just great to ride in the city. Of course nothing if u need a real front light. Maybe its better to go for 24v... Let me know your thoughts!
https://www.youtube.com/watch?v=tp5KQ5WFtwQ

here are the risers I created... perfect for TB218 with huge wheels.

I got some PCBs left here, but it think its more clever to rework the PCB because of the size and features. I ll remove the buzzer (I guess I ll not use it) and add a third channel for a horn or whatever.

I also want to replace the huge mosfets at least for the break lights and set them to 800mA max. Its not necessary to use that huge mosfet for backlights.
```

---
## \#375 Posted by: sofu Posted at: 2018-12-27T19:53:13.008Z Reads: 168

```
What voltage are the LEDs supposed to be again?
```

---
## \#376 Posted by: StefanMe Posted at: 2018-12-27T20:08:12.687Z Reads: 170

```
In total unter 12V with series resistor.

I use this setup as headlight:
3xLED NSDW570GS = 10.2V with 70mA plus the series resistor of 25Ohm.
2xLED NSDW570GS = 6,8V with 70mA plus the seriöses restor of 75Ohm (two times 150Ohm in parallel)
```

---
## \#377 Posted by: jbruce Posted at: 2018-12-27T20:15:35.214Z Reads: 169

```
Can I suggest two more things. 1. An odometer feature for your board and 2. A battery percentage or voltage for the battery in the remote. Thanks for all your hard work!
```

---
## \#378 Posted by: StefanMe Posted at: 2018-12-27T20:32:19.707Z Reads: 179

```
If u use the remote with an VESC, it will use the distance from the Vesc to recognise how far u traveled... or do u mean a odometer sensor like in phones?

Battery percentage is already implemented. On the "SPEED" page, the second value is the battery percentage from the board and on all pages is a long bar going from top to bottom to indicate the battery status.

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/8/7/87abcf852e945fa5affd84e4436ecf06a7d15c15.jpeg)
```

---
## \#379 Posted by: sofu Posted at: 2018-12-27T20:37:04.888Z Reads: 174

```
I think he means battery percent for the remote itself, not the board. 

Also just to clarify, you mean 12v is the max voltage for the led? Or do you mean anything below 12v?
```

---
## \#380 Posted by: StefanMe Posted at: 2018-12-27T20:41:50.554Z Reads: 174

```
Ah ok. Thanks

U have a 12V output on the two terminals on the Advanced PCB. U can connect here everything u want. If u have a LED with 12 volt, its just fine. But normally there are only LED with 3,4Volt or something and u have to put them in serials including a series resistor. Every motorbike break light for example will work.  because they managed the LEDs already to fit to 12V.
```

---
## \#381 Posted by: sofu Posted at: 2018-12-27T20:54:22.718Z Reads: 174

```
Got it thanks for clarifying! So excited to put all this together in my Haya! oh is the remote compatible with the Unity? And is it possible to vibrate on fault and show an error code on the display at all?
```

---
## \#382 Posted by: StefanMe Posted at: 2018-12-27T21:13:10.733Z Reads: 171

```
Not at the moment... I had a unity here, but not long enough for checking the handling. But it shouldn't not be that difficult. Lets see when I can implant this and send an update...
```

---
## \#383 Posted by: jbruce Posted at: 2018-12-28T01:12:19.622Z Reads: 168

```
Yeah I meant battery level of the remote itself so you know when it’s almost out of charge. Also by odometer I mean something like a car has which shows the total number of miles the board has ever been driven.
```

---
## \#384 Posted by: tardyparty7 Posted at: 2018-12-28T01:26:35.393Z Reads: 168

```
r u gonna do a second batch anytime soon. if not, how did you make the pcb?
```

---
## \#385 Posted by: totalgeek9224 Posted at: 2018-12-28T11:44:25.705Z Reads: 167

```
Manual has been updated with some links to some more through writeups.
If you dont understand something or would like more detail, let me know!
```

---
## \#386 Posted by: sofu Posted at: 2018-12-28T12:24:24.788Z Reads: 168

```
Is it still the same link? If so it would be great to get documented input/output power specs! For example I think earlier on I remember @StefanMe saying something about the power input for lights being good for 60v but on the pcb it's labeled 36V, so is that still the case? The output's 12V limit and amperage limits per GPIO11/12 should also be documented I think... Otherwise great writeup!
```

---
## \#387 Posted by: totalgeek9224 Posted at: 2018-12-28T12:25:41.002Z Reads: 169

```
Link is still the same, ive just added two other links within the manual for specific use cases. 

As for the power specs of the Advanced, If Stefan gets the specs to me i'll be sure to include them!
```

---
## \#388 Posted by: StefanMe Posted at: 2018-12-28T12:46:53.511Z Reads: 172

```
Not at the moment... still to much work with the first batch. But I ll let you know if there are some plans to create a second batch.

@sofu
At the moment its just rated for 10S. I don't have a 12S battery to try out how good it works with 12S. The only problem are the capacitor close to the input terminal and the huge diode on the bottom right edge. IT SHOULD WORK, but if u want to make sure u don't break anything, we should replace them to even bigger ones. 

The capacitor should be replaced with an even bigger [100uF 63V capacitor](https://www.ebay.com/sch/i.html?_from=R40&_trksid=p2334524.m570.l1313.TR1.TRC0.A0.H0.X100uF+63V.TRS0&_nkw=100uF+63V&_sacat=0&LH_TitleDesc=0&_osacat=0&_odkw=MBR360) and the Diode should be replaced with [MBR360](https://www.ebay.com/sch/i.html?_from=R40&_trksid=m570.l1313&_nkw=MBR360&_sacat=0)

I rate the outputs GPIO11 GPIO12 for 2A total. More Is possible but not recommenced.

We ll update the instructions from time to time to give u as much help as we can.
```

---
## \#389 Posted by: sofu Posted at: 2018-12-28T12:52:21.351Z Reads: 174

```
Hmm this build I'm doing is 12s... if you say it *should* work, should I try it and see? Is it only those components that are likely to get damaged if it doesn't work? Or will other things get damaged?
```

---
## \#390 Posted by: StefanMe Posted at: 2018-12-28T12:55:37.788Z Reads: 171

```
Let me check what could happen... I do little bit of research. Maybe its the best to just order these parts. its just to dangouers... the capacitor is rated for 50V and the DIODE is rated for 42V. That just to close to the edge.
```

---
## \#391 Posted by: sofu Posted at: 2018-12-28T13:10:33.339Z Reads: 168

```
Are these two parts right?

100uF 63V alu-electrolytic cap: https://www.digikey.com/product-detail/en/panasonic-electronic-components/EEU-FC1J101/P10343-ND/266352

MBR360 diode: https://www.digikey.com/product-detail/en/on-semiconductor/MBR360G/MBR360GOS-ND/1477179

Can you mark where they should be replaced?
```

---
## \#392 Posted by: StefanMe Posted at: 2018-12-28T13:18:50.935Z Reads: 172

```
I could recommend this one... https://www.digikey.com/product-detail/en/panasonic-electronic-components/ECA-1JM101B/P19536TB-ND/2688731

This one has a smaller diameter. But with a little bit of pushing the 10mm from you should also be ok. its just a space problem. But normally every 63V 100uF capacitor should work, as far as u can fit it in. 

The diode is just perfect. I am more conserved about the diode to be true. This is the much more important part to exchange. But I still recommend to to exchange both. 

I ll write a small section in the manual about upgrading the receiver to 12S.
```

---
## \#393 Posted by: PickSix24 Posted at: 2018-12-28T22:14:32.383Z Reads: 182

```
![image|375x500](upload://4jcOUlPIBbXkhm8DXUieJaDI6FA.jpeg) My remote finally showed !!! 😁😁 Now I just gotta crack open my board to install. @StefanMe , really nice quality and feel. Thank You. Can’t wait to ride with it.
```

---
## \#394 Posted by: totalgeek9224 Posted at: 2018-12-28T22:52:34.376Z Reads: 180

```
Weird favor, Could you lay out the items that came in the bag and take a photo?
Many thanks!
```

---
## \#395 Posted by: PickSix24 Posted at: 2018-12-28T22:56:11.546Z Reads: 182

```
![image|374x500](upload://51JOl9RLU2k59D6B51OWctOcpc0.jpeg)
```

---
## \#396 Posted by: totalgeek9224 Posted at: 2018-12-28T22:57:06.197Z Reads: 172

```
Thanks! And when you open the bag could you photograph that too?
```

---
## \#397 Posted by: StefanMe Posted at: 2018-12-28T22:59:42.846Z Reads: 168

```
Unboxing porn? 😏😂

The package doesn’t look that nice that’s it worth a picture 😂
```

---
## \#398 Posted by: totalgeek9224 Posted at: 2018-12-28T23:00:54.329Z Reads: 167

```
Nope! not yet ;) 
Trying to get photos of everything included so i can include in the manual :rofl:
```

---
## \#399 Posted by: sofu Posted at: 2018-12-28T23:28:51.079Z Reads: 169

```
@StefanMe is it possible to use larger amperage diode? like 5A? I'm looking at this: https://www.amazon.com/CHANGRUN-Schottky-Barrier-Rectifier-DO-201AD/dp/B07GLP8XGP
```

---
## \#400 Posted by: PickSix24 Posted at: 2018-12-29T00:12:40.573Z Reads: 161

```
I can pose with each part as well if it helps 🤣
```

---
## \#401 Posted by: StefanMe Posted at: 2018-12-29T00:31:46.157Z Reads: 160

```
Yes of course... bigger is better in this case
```

---
## \#402 Posted by: sofu Posted at: 2018-12-29T00:45:07.299Z Reads: 164

```
Does that mean I can run more powerful lights 😋
```

---
## \#403 Posted by: StefanMe Posted at: 2018-12-29T00:47:53.481Z Reads: 168

```
No 😛😬 24W max.
```

---
## \#404 Posted by: dspx Posted at: 2018-12-29T00:56:35.958Z Reads: 178

```
Yes, hand model like so 
![Hands_Federico|400x500](upload://rS1sbpgHLsTnz5qdgjYhABSH2GL.jpeg) 
:joy:
```

---
## \#405 Posted by: sofu Posted at: 2018-12-29T01:24:16.643Z Reads: 177

```
btw I think you might be missing a link on the update guide, there's no link to download the source to compile and upload to the feather...
```

---
## \#406 Posted by: swimmydude Posted at: 2018-12-29T03:37:12.503Z Reads: 170

```
Either you got big hands or your banana scale is broken.
```

---
## \#407 Posted by: StefanMe Posted at: 2018-12-29T12:57:56.580Z Reads: 166

```
No it’s not missing.. I ll send u the code when u want to upgrade your remote. I don’t wanna throw the code out for public at the moment.
```

---
## \#408 Posted by: StefanMe Posted at: 2018-12-29T13:06:29.436Z Reads: 167

```
I am just curious, what are your plans for the lights? Getting crazy with laser beams? :joy:
```

---
## \#409 Posted by: kiryl Posted at: 2018-12-29T14:05:40.809Z Reads: 162

```
My receiver is acting weird. Is the red light supposed to remain on? And my yellow lights doesn't flash either. What can I do?
```

---
## \#410 Posted by: StefanMe Posted at: 2018-12-29T14:09:24.428Z Reads: 160

```
The red light is acting like a break light... so it depends on throttle status. U can ignore the yellow light.

What means weird?
```

---
## \#411 Posted by: kiryl Posted at: 2018-12-29T14:12:40.568Z Reads: 157

```
I can't seem to pair up with the receiver. Remote keeps telling me "Fail, board not paired"
```

---
## \#412 Posted by: StefanMe Posted at: 2018-12-29T14:14:15.805Z Reads: 166

```
Then please switch on the receiver, wait for 10 seconds and push the button on the receiver for 1 second... (that resets the address from the receiver to origin)

Go into Settings menu and choose PAIR NEW BOARD. Then everything should be fine. Switch off remote and receiver and switch on again.

If it doesn't work, write me a private message and I ll help u in detail. :slight_smile:
```

---
## \#413 Posted by: tricky-fpv Posted at: 2018-12-29T17:23:32.524Z Reads: 168

```
I have problems with the advanced one.
Turn on tx then turn on board and try to pair. See if that way works for u.
So far with the basic not one problem so happy:-)
```

---
## \#414 Posted by: sofu Posted at: 2018-12-29T19:02:30.521Z Reads: 174

```
I'm planning on using 12v led strips!

![image|666x500](upload://tYItIILd9FJW48oQU6Ug4hktlnH.jpeg) ![image|666x500](upload://8aoUbmRmeLYjIxZqCkyixrlxztR.jpeg) 

Got some extras for various other places on the board as well :P
```

---
## \#415 Posted by: StefanMe Posted at: 2018-12-29T19:16:38.153Z Reads: 166

```
Be careful while lighting them up on the roll... I heard some bad things about burins flats about this :rofl: How much current one LED draw? 5V? 

I love to see them rolling on the HAYA! :heart_eyes:
```

---
## \#416 Posted by: sofu Posted at: 2018-12-29T19:32:12.541Z Reads: 166

```
Oh not the entire roll of course, they are cuttable strips so I will use sections in places

The strip draws 12v but I haven't measured how much mA the cut sections draw. It's 3 led per cuttable  section so shouldn't be that much...
```

---
## \#417 Posted by: tricky-fpv Posted at: 2018-12-29T22:00:31.251Z Reads: 170

```
The leds use 2A per strip i think
```

---
## \#418 Posted by: sofu Posted at: 2019-01-01T22:50:13.359Z Reads: 174

```
Hey @StefanMe which cap do I replace with the new one?

Just kidding I figured it out!

![image|666x500](upload://44PnpXbdG8H7rv025AQvgO6CeHF.jpeg) ![image|666x500](upload://ceOZ9NbbLiuRQ1DWxVbPrtAfVtu.jpeg)
```

---
## \#419 Posted by: PickSix24 Posted at: 2019-01-01T23:50:19.595Z Reads: 165

```
Still trying to get mine to work. Seems to be having connection issues. Haven’t even been able to ride yet 😢
```

---
## \#420 Posted by: StefanMe Posted at: 2019-01-01T23:58:14.988Z Reads: 168

```
The middle size one! It have 100uF/50V (next to the JST connector)

U already got it :slight_smile: 

@PickSix24if u want we can check tomorrow what’s going on...
```

---
## \#421 Posted by: PickSix24 Posted at: 2019-01-02T00:17:06.885Z Reads: 168

```
Sounds good
```

---
## \#422 Posted by: Darkie02 Posted at: 2019-01-02T02:06:25.173Z Reads: 172

```
Is any one else still wating for remotes to arrive?
```

---
## \#423 Posted by: Darkie02 Posted at: 2019-01-02T02:21:14.874Z Reads: 180

```
Depending on the size of chips but SM5050 are 7.2w or 14.4w or 19w as common but I’ve also used 60w per meter. rolls Are normally 5m but I’ve got some 30 meter long rolls I’ve used in the past that’s been 5v 300A just because it’s small don’t think it’s low amps. If you got some more details I can try to help with the rough load it is if that helps
```

---
## \#424 Posted by: walleywalker Posted at: 2019-01-04T23:27:21.926Z Reads: 176

```
I am. I'm in Chicago, IL
```

---
## \#425 Posted by: Chupacabra Posted at: 2019-01-05T23:24:56.545Z Reads: 174

```
Hey are you selling any completed by any chance ?
```

---
## \#426 Posted by: CheerioCoil Posted at: 2019-01-07T12:51:32.545Z Reads: 169

```
Is there going to be a second batch sometime? Interested in purchasing the basic remote.
```

---
## \#427 Posted by: StefanMe Posted at: 2019-01-08T05:51:08.795Z Reads: 162

```
I ll get some new parts in the next days for testing... then we ll see.
```

---
## \#428 Posted by: StefanMe Posted at: 2019-01-11T04:44:33.672Z Reads: 164

```
I wrote a new Library for Arduino to implement UNITY Support 😬 

I guess @sofu will confirm later that we have UNITY support in the feather remote for telemetry data. 

We did a lot of big fixes the last days! I recommend everyone to do the update! Described in the manual or with my team viewer support!

I also added the TEMP page where I can check your motor and FET-temps as well 😍 maybe we add a alarm for high temperature?
```

---
## \#429 Posted by: sofu Posted at: 2019-01-11T05:02:06.152Z Reads: 164

```
Can confirm telemetry is a go from the Unity! Works great :D awesome job @StefanMe
```

---
## \#430 Posted by: Friskies Posted at: 2019-01-11T05:48:55.896Z Reads: 160

```
I'm still waiting for mine to arrive :frowning:
```

---
## \#431 Posted by: StefanMe Posted at: 2019-01-11T05:49:23.606Z Reads: 163

```
???????? What does the tracking say?
```

---
## \#432 Posted by: Friskies Posted at: 2019-01-11T05:52:25.264Z Reads: 162

```
I'll pm you so the thread doesn't get cluttered.
```

---
## \#433 Posted by: Arek Posted at: 2019-01-12T00:35:35.485Z Reads: 160

```
Any updates on release of PCB files or schematics?
```

---
## \#434 Posted by: StefanMe Posted at: 2019-01-12T11:13:00.085Z Reads: 163

```
Schematics are not available in the manual :slight_smile:
```

---
## \#435 Posted by: Arek Posted at: 2019-01-12T11:40:04.718Z Reads: 167

```
Then sounds like it's the time for reverse engineering :slight_smile:
```

---
## \#436 Posted by: StefanMe Posted at: 2019-01-12T11:57:09.351Z Reads: 174

```
I ll release the PCB Files as soon as I have tested them enough. But u need to be able to handle with 0603 SMD parts...
![IMG_8419|375x500](upload://vQAe17HGD6YU4u8qVFK9JWIRFDe.jpeg)
![IMG_8418|375x500](upload://2Z7XqDbZnttjk3Vs9LZxdhY7HMf.jpeg)
```

---
## \#437 Posted by: Arek Posted at: 2019-01-12T12:06:57.200Z Reads: 170

```
Ah ok fine.
Duh, I'm profesionally soldering SMD prototype PCB xD
That's what I wanted to do, replace with SMD, these sticking out THT components were triggering me.
And these TO220 mosfets flapping in the breeze are going to crack on the joints/pads because of the vibrations, you'll get returns on these :frowning: 

What PCB software do you use?

Why not fit all functions of the big receiver into small PCB?
You just raise that feather dev module up a bit and you can fit a lot of components there.
EDIT: No wait there's no space for these fat connectors xD
```

---
## \#438 Posted by: StefanMe Posted at: 2019-01-12T12:41:37.596Z Reads: 171

```
EasyEDA

Next step is to bring the SAMD21 Chip as standalone onto the PCB... but that's a future project. 

I want to keep the receiver modular... many people want to try out the basic version and upgrade with the extension board.
```

---
## \#439 Posted by: mishrasubhransu Posted at: 2019-01-12T12:59:05.669Z Reads: 161

```
[quote="StefanMe, post:436, topic:74084"]
I ll release the PCB Files as soon
[/quote]
Will wait for them, but if you have spare PCBs--unpopulated ones are fine too-- can I buy them from you?
```

---
## \#440 Posted by: StefanMe Posted at: 2019-01-12T13:09:06.619Z Reads: 161

```
No sorry I ll not sell them. just order them by JLCPCB.com for 2 doller (10 piceces) + shipping
```

---
## \#441 Posted by: Arek Posted at: 2019-01-12T13:51:52.565Z Reads: 166

```
Oh yeah excluding the adafruit module from the BOM would decrease the price and allow you to do things better like add low pass filter after the step-up converter so RF module/IC gets better.
Also pls use type-c port...

Where's the BOM of all the parts?
Can't find in the manual nor first post...
```

---
## \#442 Posted by: totalgeek9224 Posted at: 2019-01-12T13:52:45.039Z Reads: 168

```
Its in the Manual (newly added) 
Just scroll to the bottom!
```

---
## \#443 Posted by: Arek Posted at: 2019-01-12T13:54:19.172Z Reads: 174

```
It's empty
![bom|690x353](upload://23KOARmxLdxKEoYXRK5z7NgqQFU.png)
```

---
## \#444 Posted by: totalgeek9224 Posted at: 2019-01-12T13:54:40.115Z Reads: 166

```
A voice in the distance screams: *"click it"*
```

---
## \#445 Posted by: Arek Posted at: 2019-01-12T13:56:16.835Z Reads: 163

```
OMG WHY YOU DID THIS LIKE THAT GEEK...
Pls just put the bom in there.
```

---
## \#446 Posted by: totalgeek9224 Posted at: 2019-01-12T13:58:30.256Z Reads: 158

```
Figured it wasn't really pertinent to the "Instruction Manual" aspect of that document, and as such, many people referring to that document are there for troubleshooting the product they already have. 

I'll change the text color to blue though so its more clear that its a hyperlink
```

---
## \#447 Posted by: Arek Posted at: 2019-01-12T13:59:24.228Z Reads: 153

```
thats better zach d
```

---
## \#448 Posted by: StefanMe Posted at: 2019-01-12T14:00:47.216Z Reads: 157

```
This BOM is for V0.1! There is no BOM for V0.2/3 at the moment. The new versions is still in development. 

Receiver and extension board is working fine. Just have to test the remote.
```

---
## \#449 Posted by: totalgeek9224 Posted at: 2019-01-12T14:01:06.603Z Reads: 153

```
Very odd usage of names going on here, but alas
Im glad its **Arek** approved
```

---
## \#450 Posted by: Arek Posted at: 2019-01-12T14:03:25.700Z Reads: 160

```
Funny because I approve/modify/upgrade procedures at work as well haha

[StefanMe](https://www.electric-skateboard.builders/u/StefanMe) I'll just order the feather module just in case they send it from another country(which could take some time).
```

---
## \#451 Posted by: ducktaperules Posted at: 2019-01-12T14:14:25.997Z Reads: 167

```
[quote="StefanMe, post:438, topic:74084"]
Next step is to bring the SAMD21 Chip as standalone onto the PCB
[/quote]

I have been considering doing this, it seems like the best option. 
I have been working in KiCad and it alows eagle import. adafruit release all of their design files in eagle format so getting the entire feather design onto your own board is quite an easy task.

also is there any reason that your using the SAMD21 not the 32u4? just wondering if there is a reason other than processor speed?
```

---
## \#452 Posted by: Arek Posted at: 2019-01-12T14:17:20.859Z Reads: 165

```
I also use Eagle, must choice for opensource hobby type projects!
```

---
## \#453 Posted by: StefanMe Posted at: 2019-01-12T14:19:44.165Z Reads: 178

```
I have already done this... but didn't tested it yet. Too much other things to do... I have the PCBs already here.

![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/8/d/8d48fb92fdfc6799fcf99012eb2a2054c13ddee5.png)
```

---
## \#454 Posted by: ducktaperules Posted at: 2019-01-12T14:21:20.972Z Reads: 172

```
nice, this looks sweet
```

---
## \#455 Posted by: StefanMe Posted at: 2019-01-12T14:22:39.306Z Reads: 171

```
For now I just stick on the feather and want to make this a stable product. Then I go for the next step. But my plans already changed about the chip... I want to use the ESP32. Two cores are just awesome. One just for telemetry and the other for all the display handling ect. AND SUPER CHEAP.
```

---
## \#456 Posted by: Arek Posted at: 2019-01-12T14:24:42.587Z Reads: 164

```
I also had the idea of using ESP32 so you use one core for display handling and second one for everything else.
Also It's dirt cheap
```

---
## \#457 Posted by: ducktaperules Posted at: 2019-01-12T14:27:06.211Z Reads: 163

```
yeah, im surprised that no ones has worked out a BT module that would alow direct connection to the metR or the unity yet.
```

---
## \#458 Posted by: StefanMe Posted at: 2019-01-12T14:29:31.569Z Reads: 168

```
A few did... Its not stable enough I think.

I would still go for the RF69 or the NRF24 if I use the ESP32.
```

---
## \#459 Posted by: Arek Posted at: 2019-01-12T14:37:21.110Z Reads: 172

```
And uploads real time data through bluetooth to the smartphone?
Maybe also directions from the GPS navigation to the remote xD
```

---
## \#460 Posted by: StefanMe Posted at: 2019-01-12T15:16:29.738Z Reads: 169

```
Or just make a solid remote...

don't overpower it without having a sold remote. :slight_smile: step by step.
```

---
## \#461 Posted by: Arek Posted at: 2019-01-12T15:20:56.440Z Reads: 174

```
What about receiver that goes directly to the focbox unity?
They have dedicated spot/header under the cover.
```

---
## \#462 Posted by: StefanMe Posted at: 2019-01-12T15:26:26.809Z Reads: 176

```
What do u mean? I am not a fan to put the telemetry on top of crazy powerful mofsets and high currents...
```

---
## \#463 Posted by: Arek Posted at: 2019-01-12T15:28:01.521Z Reads: 179

```
![1534231431|500x500](upload://dk8iNvl9y5NTosJ2HifnvT2cDJF.jpeg)
```

---
## \#464 Posted by: bevilacqua Posted at: 2019-01-12T16:45:56.301Z Reads: 178

```
This is all a 1 man job. I think stefan has enough to do. Piano piano and all will go well

A good/stable/cool remote is the primary goal ;)
```

---
## \#465 Posted by: Arek Posted at: 2019-01-12T16:48:00.364Z Reads: 176

```
I'm just inspiring him for future projects :stuck_out_tongue:
```

---
## \#466 Posted by: Arek Posted at: 2019-01-12T20:47:54.382Z Reads: 182

```
Got mine printed:
![IMG_20190112_175322|690x388](upload://6vZJWrADW3vpyup1jpqrOSXLL65.jpeg) ![IMG_20190112_175415|690x388](upload://qq2iiucZzKhCWWO9Le3JZAxbjTb.jpeg) ![IMG_20190112_194058|690x388](upload://5IelajJASUUSHaniWMO8MXhrDaW.jpeg)

[StefanMe](https://www.electric-skateboard.builders/u/StefanMe) In BOM it say I need JST PH connector but in the listing from the link it shows JST and PH as different types, which one it should be, PH?
```

---
## \#467 Posted by: pookybear Posted at: 2019-01-13T02:31:57.454Z Reads: 175

```
Where do I sign up for the next batch? 😅
```

---
## \#468 Posted by: mishrasubhransu Posted at: 2019-01-13T04:50:38.881Z Reads: 176

```
What are you going to do with the bom? There is not PCB yet right?
```

---
## \#469 Posted by: Touch415 Posted at: 2019-01-13T07:38:30.515Z Reads: 173

```
For real 😔😔😔
```

---
## \#470 Posted by: totalgeek9224 Posted at: 2019-01-13T09:07:30.117Z Reads: 178

```
@pookybear @Touch415  I'm not 100% sure but I think the plan for now is use this as a feedback period from those who have the remote already, and then within a month or so to do another run with the new pcb's and firmware

Of course only @StefanMe can confirm
```

---
## \#471 Posted by: Arek Posted at: 2019-01-13T10:34:08.132Z Reads: 176

```
Some of the parts, like connectors, hall sensor and mechanical parts will be still the same...
```

---
## \#472 Posted by: StefanMe Posted at: 2019-01-13T12:05:49.288Z Reads: 195

```
I want to sell 5 more complete sets with the new versions. Hardware is awesome.

Set includes a full Set:

1 x Feather remote in Black (Extra colours are possible for 15 Euros)
1 x Basic receiver with LC-Filter onboard
1 x Extension board to control break and headlight (12V, total power of 24W)

ALL REMOTES SOLD

![IMG_8445|375x500](upload://kZbiz7pk8o4oW54c0bLVJ2VResZ.jpeg) 
![IMG_8446|375x500](upload://mTAyMQ9KkxqD64LtrTkng7ut5gh.jpeg) 
![IMG_8448|375x500](upload://wmTMqMd8Gr41VRY6WyLAd4uixPM.jpeg) 
![IMG_8447|375x500](upload://1OILKIndrXoWDPTWDKLX4IeIr3M.jpeg)
```

---
## \#473 Posted by: totalgeek9224 Posted at: 2019-01-13T12:36:48.486Z Reads: 181

```
@pookybear @Touch415 check it out!!!
```

---
## \#474 Posted by: Darkie02 Posted at: 2019-01-13T12:59:28.898Z Reads: 183

```
That extension boards is  parity awesome idea
```

---
## \#475 Posted by: jimmymagix Posted at: 2019-01-13T13:23:12.316Z Reads: 184

```
[quote="StefanMe, post:472, topic:74084"]
IMG_8445
[/quote]

Ordered. Do I pay now or on completion? When is the estimated ship date?
```

---
## \#477 Posted by: tardyparty7 Posted at: 2019-01-13T17:28:17.512Z Reads: 179

```
JESUS I NEED TO GET ONE BUT MY PARENTS AREN'T HERE AND I NEED TO DO IT IN PERSON! SON OF A B_____. these are gonna sell out in seconds....... damn't
```

---
## \#478 Posted by: pookybear Posted at: 2019-01-13T17:33:22.160Z Reads: 179

```
Ordered! Trying to PayPal money but I don't know how much. LOL. Too damn excited
```

---
## \#479 Posted by: tardyparty7 Posted at: 2019-01-13T17:33:44.736Z Reads: 176

```
how many r left? lol i have the form filled out, but I need to pay, cough cough parents.
```

---
## \#480 Posted by: tardyparty7 Posted at: 2019-01-13T17:35:00.185Z Reads: 176

```
i don't wanna tell u cause i want one but its 160 + 18 (for shipping) and if you chose color its + 15.
```

---
## \#481 Posted by: pookybear Posted at: 2019-01-13T17:35:53.767Z Reads: 175

```
That too and I found the price. Hahahaha.

I just wanna make sure I got in before I pay.
```

---
## \#482 Posted by: tardyparty7 Posted at: 2019-01-13T17:36:24.982Z Reads: 173

```
:sob:
10char
```

---
## \#483 Posted by: pookybear Posted at: 2019-01-13T17:36:57.040Z Reads: 167

```
He did say black only?
```

---
## \#484 Posted by: tardyparty7 Posted at: 2019-01-13T17:37:38.979Z Reads: 165

```
then what does he mean by "color"
```

---
## \#485 Posted by: pookybear Posted at: 2019-01-13T17:38:04.815Z Reads: 174

```
LOL. This is bad. I need to read better. Way too damn stoked for missing important information. Hahaha
```

---
## \#486 Posted by: tardyparty7 Posted at: 2019-01-13T17:47:34.411Z Reads: 176

```
[quote="pookybear, post:483, topic:74084, full:true"]
He did say black only?
[/quote]

[quote="StefanMe, post: 467, topic: 78084, full:true"]
1 x Feather remote in Black (Extra colours are possible for 15 Euros)
[/quote]

I think u can have dif colors.
```

---
## \#487 Posted by: StefanMe Posted at: 2019-01-13T17:48:14.801Z Reads: 172

```
yes u can just order a different color if u pay for it,
```

---
## \#488 Posted by: StefanMe Posted at: 2019-01-13T17:51:35.931Z Reads: 168

```
Should I keep a slot for u?
```

---
## \#489 Posted by: tardyparty7 Posted at: 2019-01-13T17:52:08.916Z Reads: 175

```
lemme ask my parents, i'll bet they'll say yes but idk, i don't wanna hold ur orders back.
```

---
## \#490 Posted by: StefanMe Posted at: 2019-01-13T17:55:11.298Z Reads: 178

```
Yes I confirm. Its 160Euro + 18Euro shipping and optional 15Euro for a special color.
```

---
## \#491 Posted by: StefanMe Posted at: 2019-01-13T18:51:29.824Z Reads: 177

```
One jumped out. So one more for
Sale guys. Just PM me if u want one.
```

---
## \#492 Posted by: tardyparty7 Posted at: 2019-01-13T23:36:52.032Z Reads: 178

```
payed. :sunglasses:
```

---
## \#495 Posted by: sofu Posted at: 2019-01-14T08:49:39.875Z Reads: 180

```
Guys this is an amazing remote and receiver combo. Tons of features and awesome support from @StefanMe! It even accidentally helped me diagnose an issue I had with my board's batteries 😅

Too bad you missed it @Winfly
```

---
## \#496 Posted by: totalgeek9224 Posted at: 2019-01-14T08:50:52.859Z Reads: 183

```
[quote="sofu, post:495, topic:74084"]
It even accidentally helped me diagnose an issue I had with my board’s batteries
[/quote]

OOoooooh, how did this happen?
```

---
## \#497 Posted by: Winfly Posted at: 2019-01-14T08:51:15.345Z Reads: 185

```
Woooow ok. @StefanMe pls put me next on the list for next batch.
```

---
## \#498 Posted by: sofu Posted at: 2019-01-14T09:00:29.145Z Reads: 181

```
I was hitting 0% battery throttling for some reason even though I was at at least half battery, and the remote was giving me battery warnings. Turns out one of my p groups was dying extremely fast and ended up dead at 0v. Wouldn't have known without the remote warning me with vibration
```

---
## \#499 Posted by: ElectricCoast Posted at: 2019-01-15T03:17:03.863Z Reads: 175

```
When is the next batch @StefanMe?
```

---
## \#500 Posted by: StefanMe Posted at: 2019-01-16T18:10:40.529Z Reads: 178

```
@ElectricCoast I think thats it for now. Ill create a few batches in the future only 5 every time and will give the shematics ect for free... then u can go for your own if u want.

**I did a lot of debugging and bugfixing the last days, I can recommend  everyone to make an update on your remote and receiver. Take a look into the manual for updates.  If u need help give me a shout!**
```

---
## \#501 Posted by: Chalupa_Batman Posted at: 2019-01-16T18:57:50.204Z Reads: 174

```
Any chance you would be willing to do a pre order?so that we know we will definitely be in the next batch.
```

---
## \#502 Posted by: CheerioCoil Posted at: 2019-01-17T14:01:11.665Z Reads: 175

```
oops. I didn't check this thread for 10 days and another small batch was sold. rip.
```

---
## \#503 Posted by: mishrasubhransu Posted at: 2019-01-17T14:06:29.844Z Reads: 168

```
Actually I want to open up my position, but Stefan seems to be busy until Friday and hasn't replied yet.
```

---
## \#504 Posted by: CheerioCoil Posted at: 2019-01-17T15:51:55.859Z Reads: 170

```
@mishrasubhransu By open position do you mean you placed an order and no longer want it? I'd place an order in your stead if it's available. :smiley:
```

---
## \#505 Posted by: tardyparty7 Posted at: 2019-01-17T16:03:18.941Z Reads: 172

```
idk who would wanna give up one of these bad boys. lol
```

---
## \#506 Posted by: StefanMe Posted at: 2019-01-17T17:29:30.143Z Reads: 173

```
Sorry guys am am out for training this week. I ll give u feedback on the weekend. Please be patient.
```

---
## \#507 Posted by: Surfer Posted at: 2019-01-17T22:02:57.944Z Reads: 186

```
Hey Stefan, the update and everything when smooth, thanks a lot for your help
I think the telemetry is fixed, don’t know for sure yet, tomorrow ride to work and test.
What a nice surprise that I got, now is working the 2 motor temp sensors, awesome!!
I think I find one!!! :bug:
The MOSFET, vesc temperature is showing battery volts.
![Screenshot_20190117-224619|250x500](upload://ndPH3yp9nfglFeQtNdHmj0DuaGX.jpeg) ![Screenshot_20190117-224648|250x500](upload://mfG690vtyBJOJmK7a7gHXmQo3Kp.jpeg) 

Awesome work you did it with this remote man!!
Mad props!!!
```

---
## \#508 Posted by: StefanMe Posted at: 2019-01-17T22:04:43.030Z Reads: 177

```
Awesome!

> The MOSFET, vesc temperature is showing battery volts.

This is because I didn't knew what's reasonable to show on this page...

Top: VOLTAGE,
Middle: MOSFET-Temp
Bottom: MOTOR-Temp

On the unity its more clear...

Top: MOSFET-Temp left,
Middle: MOSFET-Temp right
Middle-bottom: MOTOR-Temp left
Bottom: MOTOR-Temp right

I maybe should choose new names for the pages. I think there is no chance to get the second motor temp on the over bus ESCs. On the unity the pages shoes nearly everything... maybe @sofu can make a picture when she has done the
```

---
## \#509 Posted by: sofu Posted at: 2019-01-17T22:16:00.875Z Reads: 170

```
Let me update right now and report back to you. Give me 10min
```

---
## \#510 Posted by: Arek Posted at: 2019-01-17T22:45:59.671Z Reads: 173

```
So you won't upload gerbers yet?
```

---
## \#511 Posted by: sofu Posted at: 2019-01-17T23:03:13.260Z Reads: 188

```
![IMG_5034|375x500](upload://8kDcQf1afJINTsX0bqDXmDKRC10.jpeg) ![IMG_5033|375x500](upload://eRJLEIS2VTbuzHxc9k3wzR1snb3.jpeg) ![IMG_5035|375x500](upload://mPBE142gbwSwNcnMEuszmzWcUam.jpeg) ![IMG_5036|375x500](upload://ybEvswCE5Evk8QAx6bnJ7jcS7Ix.jpeg) 

Unity support looking good!
```

---
## \#512 Posted by: mishrasubhransu Posted at: 2019-01-17T23:14:19.468Z Reads: 172

```
Dude, give him time.
```

---
## \#513 Posted by: Surfer Posted at: 2019-01-17T23:15:43.448Z Reads: 174

```
Thanks @sofu !!
```

---
## \#514 Posted by: Surfer Posted at: 2019-01-17T23:16:42.528Z Reads: 174

```
Or even better, Do It Yourself!
```

---
## \#515 Posted by: Arek Posted at: 2019-01-17T23:18:02.852Z Reads: 183

```
I was but then he showed updated version of what I basically wanted to change and the he said he will release files once finished.
And because he sells this new version I guess it's finished, so I simply asked...
```

---
## \#516 Posted by: mishrasubhransu Posted at: 2019-01-17T23:41:11.502Z Reads: 186

```
Yeah, I paid for the order but no longer want it. 

[quote="tardyparty7, post:505, topic:74084, full:true"]
idk who would wanna give up one of these bad boys. lol
[/quote]

I want to make my own and customize the receiver.
```

---
## \#517 Posted by: kiryl Posted at: 2019-01-19T00:14:50.178Z Reads: 181

```
Anyone has the latest source code? :slight_smile:
```

---
## \#519 Posted by: kiryl Posted at: 2019-01-19T10:06:14.773Z Reads: 180

```
I don't know what happened but my remotes keeps freezing after I uploaded the new code.
```

---
## \#520 Posted by: StefanMe Posted at: 2019-01-19T10:09:02.893Z Reads: 180

```
Did u setup the fist lines in the transmitter.ide/receiver.ide?
```

---
## \#521 Posted by: kiryl Posted at: 2019-01-19T10:12:03.174Z Reads: 180

```
I only changed the vesc to unity.
```

---
## \#522 Posted by: StefanMe Posted at: 2019-01-19T10:16:24.178Z Reads: 174

```
Habe u activated any of the debugging lines?
```

---
## \#523 Posted by: kiryl Posted at: 2019-01-19T10:17:50.060Z Reads: 168

```
No I haven't. The first time I updated the remote it worked perfectly. But Then I saw that I had to change the uart to Unity and then it stopped working and freezing... It does upload perfectly but the remote itself keeps freezing or doesn't display a screen.
```

---
## \#524 Posted by: Surfer Posted at: 2019-01-19T10:41:41.571Z Reads: 172

```
I deleted 2 lines in the header in both transmitter and receiver.ino, installed and working perfectly so far.
Telemetry work awesome!
Btw @StefanMe just curious if the possibility to read both vesc trough can bus is a hardware or software limitation?
Metr.pro got dual data in similar setup.
```

---
## \#525 Posted by: Mich21050 Posted at: 2019-01-19T10:50:03.895Z Reads: 165

```
Noooo where did it go.... :(
```

---
## \#526 Posted by: Arek Posted at: 2019-01-19T14:22:41.253Z Reads: 167

```
Did he uploaded the files and then deleted it? xD
```

---
## \#527 Posted by: Mich21050 Posted at: 2019-01-19T14:23:25.047Z Reads: 173

```
Yes I think so :joy:
```

---
## \#528 Posted by: StefanMe Posted at: 2019-01-19T14:25:00.412Z Reads: 169

```
It was an mistake to upload them here 😜
```

---
## \#529 Posted by: Arek Posted at: 2019-01-19T14:27:44.623Z Reads: 170

```
Quite a shame :frowning:
```

---
## \#530 Posted by: tardyparty7 Posted at: 2019-01-19T22:26:08.911Z Reads: 163

```
what do u mean?
```

---
## \#531 Posted by: Gerrycorrado Posted at: 2019-01-20T09:33:15.547Z Reads: 166

```
I would like to be put on the waiting list for the next batch, smart remote pretty pleasssse. Thanks!
```

---
## \#532 Posted by: Arek Posted at: 2019-01-20T19:39:02.124Z Reads: 180

```
OK no files, can you please just sell the PCBs?
I ordered all the parts already and waiting only for the PCBs :frowning:
```

---
## \#533 Posted by: sofu Posted at: 2019-01-23T03:14:06.842Z Reads: 183

```
Looking good @StefanMe! ![image|666x500](upload://oOxm9cAXYlfGWsHZMQ1lZhLHywu.jpeg)
```

---
## \#534 Posted by: PickSix24 Posted at: 2019-01-23T03:24:54.095Z Reads: 174

```
What are those ! :grinning:
```

---
## \#535 Posted by: sofu Posted at: 2019-01-23T03:46:13.712Z Reads: 172

```
FeatherReceiver Basic + one Advanced modular unit
```

---
## \#536 Posted by: tardyparty7 Posted at: 2019-01-23T03:48:40.628Z Reads: 168

```
why do u have three????!!!!!!!
```

---
## \#537 Posted by: sofu Posted at: 2019-01-23T03:53:29.985Z Reads: 175

```
It's two + one advanced module. You need the basic module otherwise the advanced module won't work. He sent me these because the original I ordered was basically DOA
```

---
## \#538 Posted by: PickSix24 Posted at: 2019-01-23T03:53:44.154Z Reads: 174

```
Nice ! , I’m still waiting for my remote to come back from Stefan. Looking forward to trying out the led control feature
```

---
## \#539 Posted by: sofu Posted at: 2019-01-23T03:54:08.397Z Reads: 183

```
Same haha my LEDs also didn't work to begin with

Edit: phew

![image|666x500](upload://nDnmDIA76rBaXu5jvwrKasIMkk9.jpeg)
```

---
## \#541 Posted by: PickSix24 Posted at: 2019-01-25T17:19:51.094Z Reads: 170

```
Anyone heard from @StefanMe ? Been trying to reach him.
```

---
## \#542 Posted by: bevilacqua Posted at: 2019-01-25T17:22:22.551Z Reads: 168

```
he is back in Town, he should reach out to you shortly
```

---
## \#543 Posted by: totalgeek9224 Posted at: 2019-01-25T17:32:48.547Z Reads: 163

```
Yeah I spoke to him two days ago. Im sure he's just been busy. Anything in particular you need?
```

---
## \#544 Posted by: tardyparty7 Posted at: 2019-01-25T17:49:49.992Z Reads: 163

```
he's really busy i think. He's trying to finish the remotes by this weekend and he also has a job outside of this.
```

---
## \#545 Posted by: PickSix24 Posted at: 2019-01-25T17:56:13.235Z Reads: 163

```
Yeah totally get we all have jobs. I was just looking for an update on my replacement remote from the first batch.
```

---
## \#546 Posted by: totalgeek9224 Posted at: 2019-01-25T17:57:51.337Z Reads: 162

```
Ah I see, Unfortunately I can't help you with that. I can assure you that it's not forgotten, but yeah just gotta wait until he comes back online to get an update
```

---
## \#547 Posted by: tardyparty7 Posted at: 2019-01-25T17:57:51.942Z Reads: 161

```
oh, he said he was finishing it this weekend. ppl who make purchases should probs ask for a phone number or something. (i made a purchase btw 😉)
```

---
## \#548 Posted by: PickSix24 Posted at: 2019-01-25T18:03:43.931Z Reads: 164

```
Ya that’s probably a good idea. My original remote has been at the post office waiting to be picked up for almost 2 weeks, my fear was they would return to sender at some point. It wasn’t cheap to send back.
```

---
## \#549 Posted by: PickSix24 Posted at: 2019-01-25T18:04:37.682Z Reads: 162

```
Just wanted to say Stefan has been super helpful with the remote though.
```

---
## \#550 Posted by: tardyparty7 Posted at: 2019-01-25T18:05:14.745Z Reads: 173

```
oh. he was gone for a while. he may have forgotten about it. plus dif time zones makes it 100 times harder.

edit: nvm he's here!
```

---
## \#551 Posted by: StefanMe Posted at: 2019-01-25T18:07:00.064Z Reads: 172

```
Its not the post office. Its at customs. Different place far away for me and a lot of paper work. 

Doesn't matter for u. u ll get the replacement with the second batch soon. I ll give an update on sunday. Just have to assemble all the remotes.
```

---
## \#552 Posted by: PickSix24 Posted at: 2019-01-25T18:21:37.306Z Reads: 171

```
Awesome ! Thanks for the update.
```

---
## \#553 Posted by: sofu Posted at: 2019-01-25T19:26:59.475Z Reads: 188

```
Pretty awesome! Look forward to getting it y'all!

![image|666x500](upload://dUX9TZBwLYxDNIf2l3gZIyLvqpq.jpeg) ![image|666x500](upload://hPLofowwGhRCsyVNq7IOLG9AnFR.jpeg)
```

---
## \#554 Posted by: Arek Posted at: 2019-01-25T21:09:26.434Z Reads: 177

```
Looks lit xD
How do you call these exact foot clamps? :sweat_smile:

Today got those Adafruit dev modules and will program them but damn including shipping and taxes they are pricey, have to help Stefan with the development of that universal standalone PCB so it will be much cheaper for everyone :stuck_out_tongue:
```

---
## \#555 Posted by: sofu Posted at: 2019-01-25T21:28:21.618Z Reads: 179

```
They’re the Roger Bros. Standard footstop https://www.muirskate.com/longboard/products/69451/rogers-bros-standard-foot-stop
```

---
## \#556 Posted by: Winfly Posted at: 2019-01-25T21:30:57.997Z Reads: 179

```
It's a great piece of Footstop. I can even slip a bit of my shoe sole under for more grip in the back. No more rear leg bouncing around at 25mph because of cracks.
```

---
## \#557 Posted by: Arek Posted at: 2019-01-26T15:13:15.106Z Reads: 181

```
Someone knows where do I get the code for the remotes?
In manual it's called remote.ide but I cannot find it anywhere...
On Github there are only libraries.
```

---
## \#559 Posted by: Arek Posted at: 2019-01-26T21:44:53.802Z Reads: 185

```
There was a unused line in the code saying "by stefanme" so I used it xD
![IMG_20190126_213934|281x499](upload://9qILmmGBq4vPUL4szj2twyO3c3e.jpeg)
```

---
## \#560 Posted by: tardyparty7 Posted at: 2019-01-26T21:45:23.074Z Reads: 182

```
does it work!? i love it! also, where'd u get the code?
```

---
## \#561 Posted by: Arek Posted at: 2019-01-26T21:49:30.042Z Reads: 180

```
What do you mean exactly?
I just connected display to the module, don't have all the parts yet.
For the code you have to PM Stefan
```

---
## \#562 Posted by: tardyparty7 Posted at: 2019-01-26T21:50:20.677Z Reads: 181

```
oh. i thought u finished it! ha!
```

---
## \#563 Posted by: Sn4pz Posted at: 2019-01-27T08:27:56.170Z Reads: 188

```
I don't even remember if I signed up but I know I want to be :man_facepalming:
```

---
## \#564 Posted by: Arek Posted at: 2019-01-28T19:16:58.513Z Reads: 192

```
Phew, who needs PCB...
![ghettoFeatherInside|465x500](upload://2PT73k8MaAzTXSrlkHiDi8PyroP.jpeg) 
![ghettoFeatherAssembled|281x499](upload://8ut1CtAFk2m10ZZE0zwir6cSlI5.jpeg) 

... just kiddin, PCBs are on the way, I was just bored :laughing:


PS Signal solder joints are crap on purpose, so there won't be too much of work with removing these.

**Please don't follow this** :sweat_smile:
```

---
## \#565 Posted by: Mudders Posted at: 2019-01-28T20:55:31.888Z Reads: 181

```
This is my perfect remote, I'm down for 2 on the next run @StefanMe, they look amazing :heart_eyes:
```

---
## \#566 Posted by: tardyparty7 Posted at: 2019-01-28T20:59:46.235Z Reads: 184

```
why don't u just get two receivers instead.
```

---
## \#567 Posted by: bevilacqua Posted at: 2019-01-28T21:04:13.723Z Reads: 179

```
The remote can store the pairing key for hundreds of receivers/boards
```

---
## \#568 Posted by: Mudders Posted at: 2019-01-28T21:06:07.343Z Reads: 184

```
Yep I understand that,  I'm building 2 boards, one for me and one for my son :slight_smile:
```

---
## \#569 Posted by: Arek Posted at: 2019-01-28T21:07:33.407Z Reads: 189

```
In the settings it goes from #0 to #9 so 10 in total, still enough and if you would really need you could just modify the code.
```

---
## \#570 Posted by: sayekim Posted at: 2019-01-28T21:12:08.722Z Reads: 180

```
10 builds... 1 remote... homeless...
```

---
## \#571 Posted by: Sn4pz Posted at: 2019-01-28T21:30:24.422Z Reads: 185

```
Is there any shot of getting one of these before June? I would really love to make this the remote on my board :slight_smile:

@StefanMe plz :rofl:
```

---
## \#572 Posted by: StefanMe Posted at: 2019-01-29T09:44:38.442Z Reads: 179

```
For now i restricted it to 10 boards. But in the future u can use more if u want :stuck_out_tongue:
```

---
## \#573 Posted by: PickSix24 Posted at: 2019-01-31T16:03:26.665Z Reads: 177

```
@StefanMe Any updates ?
```

---
## \#574 Posted by: StefanMe Posted at: 2019-02-01T10:30:55.798Z Reads: 183

```
Ah sorry i Miss the Information... 

I ok finish the remotes this we. They ll go out on Sunday
```

---
## \#575 Posted by: Chupacabra Posted at: 2019-02-01T17:20:14.781Z Reads: 183

```
Please keep us posted once you start to sell completes
```

---
## \#576 Posted by: ventisca1011 Posted at: 2019-02-02T01:51:46.598Z Reads: 182

```
Yay!! im so excited to get mine :smiley:
```

---
## \#577 Posted by: tardyparty7 Posted at: 2019-02-02T02:17:05.283Z Reads: 184

```
wait, u got one? ur not in the chat...
```

---
## \#578 Posted by: Kaly Posted at: 2019-02-02T12:14:28.561Z Reads: 189

```
Too bad I got late to this party :-) 
Great stuff
Will love to get testing this babies 
Should be a great match
```

---
## \#579 Posted by: StefanMe Posted at: 2019-02-02T16:08:52.488Z Reads: 190

```
He got one remote from the guy who jumped out :slight_smile:
```

---
## \#580 Posted by: Arek Posted at: 2019-02-02T16:28:31.162Z Reads: 196

```
Whoa Stefan is back, you busy making these remote, or work, or both? xD

Printed this one for fun, meet the Oreo Remote: :smiley:
![OreoRemoteBottom|690x388](upload://bOeBy8ZcTy2GtpN5Whfg4IzdyYK.jpeg) 
![OreoRemoteTop|690x388](upload://doNfABI25KkmrMT8eRb19imsn2p.jpeg)

That glitch on the front tho :frowning:
```

---
## \#581 Posted by: StefanMe Posted at: 2019-02-02T16:35:29.891Z Reads: 192

```
Haha nice idea... did u manually changed the filament on the third layer? Good idea... have not done this since a few!

Nice print quality!

Working on the remote and normal work. Unfortunately I am sick... so everything is bit harder at the moment! But everything is going well!
```

---
## \#582 Posted by: Arek Posted at: 2019-02-02T16:44:58.296Z Reads: 197

```
Just welder like two meters of black filament to a spool of white filament.
With one hand hold both filaments, with other hand use a lighter and melt both ends, then quickly join them.
When it's still elastic you hold it straight until it cools down, then you use sharp wire cutters to trim the excess off and at the end you finish the joint clean with a knife.

One thing I have to figure out how to get the filament lengt for the first X layers so I don't have to guess.
I had to guess here and as a result front has 3 layers of black and bottom 4 layers.

Thanks, but have to somehow make that stupid Cura slicer not poop random strings when traveling, it almost always destroys the look of the first layer.
Thought it might to do with poor retraction because of crappy bowden tube but when got better one(tighter one) it was getting clogged in the bowden near the heater.
Preferebly will have to get a printer with direct feed, no bowden tube(don't remember how it was called).

Well then get well soon, I have many questions to bother you with and also looking forward to that PCB that doesn't need adafruit module :stuck_out_tongue:
```

---
## \#583 Posted by: StefanMe Posted at: 2019-02-02T16:58:08.747Z Reads: 193

```
This is because u don't make retractions if u don't go over open spaces. So u loose hot filament while traveling from the outline to the "inner outlines" from the OLED. Travel faster with a faster acceleration will help... OR u go for [KLIPPER Firmware](https://github.com/KevinOConnor/klipper) and activate the PRESSURE ADVANCED. This will keep the filament at the right place, doesn't matter where the nozzle is traveling ect. U also have just 1mm retraction on poor Bowden tubes. 

 Why so complicated? Just pause the print where u want to change the color, exchange the filament, and resume the print... super easy. No fusing, no calculation...
```

---
## \#584 Posted by: Arek Posted at: 2019-02-02T17:11:45.685Z Reads: 199

```
Will try to experiment with settings but not sure which option to change in Cura.
If I stop it, printer just freeze in the spot, doesn't retract and some filament gets out and destroys the print also because it's not moving it welds or even destroys the build plate.
```

---
## \#585 Posted by: StefanMe Posted at: 2019-02-02T17:21:55.938Z Reads: 222

```
Cure is just a slicer... the Firmware on the Board in the printer makes the STOP/START/RESUME ect... I guess u are using MARLIN, so check here the PAUSE functions and specially the PAUSE MARCO.

Means, if u press PAUSE on the printer, the FIRMWARE will execute a macro after stopping the print... for example:

Small retract, Raise Z, move printing head to parking position. (These macros I have for KLIPPER, not for MARLIN... they should work there also...)

    [gcode_macro pause]
    gcode:
    	 G90 // absolute
         G92 E0 // set extruder to 0
    	 G1 E-1 F6000 // small retract
    	 G91 // incremental
    	 G1 Z0.2 F200 // move z a little bit
    	 G90 // absolute 
    	 G1 X260 Y220 F12000 // move to parking pos
    	 
    [gcode_macro resume]
    gcode:
    	 G91
    	 G1 Z-0.2 F200
    	 G90
    	 G1 X260 Y220 F12000

    [gcode_macro unloadFilament]
    gcode:	 
    	M109 S220
    	G92 E0
    	G1 E-220 F5000
    	G1 E-755 F3000
    	G92 E0
    	M104 S0
    	
    [gcode_macro loadFilament]
    gcode:	 
    	M104 S230
    	G92 E0
    	G1 E40 F1000
    	G1 E750 F6000
    	M109 S230
    	G92 E0
    	G1 E50 F100
    	G92 E0
    	G4 P10000
    	M104 S0
```

---
## \#586 Posted by: Arek Posted at: 2019-02-02T17:24:48.594Z Reads: 214

```
I add it to the code when flashing the printer I guess, quite a bit of work especially with my ender 3 that doesn't even have a bootloader on it.
Thanks!
```

---
## \#587 Posted by: Chrisjarram Posted at: 2019-02-04T09:20:57.145Z Reads: 224

```
@Stefanme Can't seem to locate the gerbers and firmware source - planning to build one of these and adapt case and fw for a colour oled screen (will happily share changes).. could you please provide updated links as only see the STLs?  Cheers
```

---
## \#588 Posted by: StefanMe Posted at: 2019-02-04T09:44:17.138Z Reads: 236

```
There is no plan go open source yet. maybe in a while. I ll contact u per dm.
```

---
## \#589 Posted by: StefanMe Posted at: 2019-02-07T10:59:26.169Z Reads: 227

```
**FeatherRemote goes OpenSource**

Source Code:
[FeatherRemote SourceCode](https://github.com/StefanMeGit/FeatherM0-Esk8-Remote)

PCBs:
[FeatherRemote PCBs](https://drive.google.com/drive/folders/1WctYzKjjuB0q0rAqc8o84Zw3_9ONQYV5?usp=sharing)

BOM:
[FeatherRemote BOM](https://drive.google.com/drive/folders/1unGQFqhujc1F1axQRts0dKecUKXAGkIH?usp=sharing)

I talked to some developers in the last days and came to the conclusion, that it would be great to make it open source.

I am not a professional programmer and here are some awesome guys who can bring this remote to the next level with nicer menus ect.

U need to be able to handle SMD soldering and 3d-printing.


Have fun
```

---
## \#590 Posted by: PickSix24 Posted at: 2019-02-07T14:20:13.957Z Reads: 215

```
What’s the status on the remotes ?
```

---
## \#591 Posted by: StefanMe Posted at: 2019-02-07T14:59:26.224Z Reads: 213

```
They are 95%done. Just have to reprint some triggers, then they go out.
```

---
## \#592 Posted by: gmurad Posted at: 2019-02-07T23:28:22.783Z Reads: 208

```
Amazing! Thanks for releasing the code and files for this - amazing contribution. I was about to build the Firefly nano but really wanted the ESTOP feature so I will build this one if I can figure everything out. I never did this kind of software development but I work in tech and I know C. Hopefully I can contribute in the future.

With the files you provided am I able to get a PCB made for the transmitter and receiver? If not, is it possible to build this without any custom PCBs like Firefly Nano?
```

---
## \#593 Posted by: auggie246 Posted at: 2019-02-08T02:15:11.035Z Reads: 204

```
Can I order onee as of now?
```

---
## \#594 Posted by: uigiroux Posted at: 2019-02-08T05:38:24.419Z Reads: 201

```
I'd like to order one also!  Is there a sign up sheet or do we just need to PM your?
```

---
## \#595 Posted by: totalgeek9224 Posted at: 2019-02-08T06:14:23.797Z Reads: 203

```
So yeah it's definitely possible to make it work without the PCB. It's just more difficult and not as reliable (arguably). Stefan's included the PCB files so you should just be able to use something like jlcpcb and get them made
```

---
## \#596 Posted by: StefanMe Posted at: 2019-02-08T11:23:24.997Z Reads: 204

```
I definitly will produce one form time to time... But not at the moment. I still  have some remotes to do. 

U definitly can build this remote like  @Arek didi it.  
https://www.electric-skateboard.builders/t/featherremote-and-smartremote-files-in-post-577/74084/564?u=stefanme

But a PCB will make it more safe.
```

---
## \#597 Posted by: Arek Posted at: 2019-02-08T23:41:39.913Z Reads: 209

```
Getting there, 95% finished :slight_smile:
![IMG_20190208_195738|281x499](upload://bwh4YCBitl8LBTSottLFV9el6It.jpeg)  

![IMG_20190208_202703|281x499](upload://ahvvrzem8v0Xagvn8vN2FfxvpiC.jpeg) 
.

Pins have to be very short to not puncture the cell:
![IMG_20190208_202759|690x388](upload://7GdsAkDbCeCWTSIz6Os1qW5bQ1x.jpeg) 

![IMG_20190208_232940|281x499](upload://3aBRvstyPKpmkqUTWrTnlfPTzXh.jpeg)
```

---
## \#598 Posted by: uigiroux Posted at: 2019-02-10T17:35:34.679Z Reads: 194

```
Do you think you'll make another production run before... say April or May?  Won't really be riding reason here for a few more months so I don't mind waiting...
```

---
## \#599 Posted by: banjaxxed Posted at: 2019-02-10T17:48:01.129Z Reads: 193

```
Nice carbonfill?
```

---
## \#600 Posted by: Arek Posted at: 2019-02-10T18:15:34.859Z Reads: 197

```
Nah that's ordinary cheap black PLA
```

---
## \#601 Posted by: willumpie82 Posted at: 2019-02-11T07:03:45.346Z Reads: 199

```
That looks so cool! i'm looking into designing a PCB that has also the controller embedded, hence no piggyback PCB
```

---
## \#602 Posted by: sofu Posted at: 2019-02-11T07:37:46.033Z Reads: 205

```
If anybody's looking to build this remote, keep in mind like @Arek said to keep the soldered pins as flush to the pcb as possible. Otherwise you the pin will puncture the battery and glitch everything mid ride...

![image|666x500](upload://bPJNZ469fb9BdRT6Lv3HtxL0YnM.jpeg)
```

---
## \#603 Posted by: Arek Posted at: 2019-02-11T08:02:23.641Z Reads: 200

```
Also I first trimmed them (with a flush wire cutter) and THEN soldered it, as a result sharp pins are covered with rounded solder.
As a another layer of protection I will add a layer of that fish paper that is intended for battery isolation use.
```

---
## \#604 Posted by: StefanMe Posted at: 2019-02-11T08:28:37.524Z Reads: 206

```
![2019-02-11%2009_50_16-EasyEDA%20-%20A%20Simple%20and%20Powerful%20Electronic%20Circuit%20Design%20Tool|358x500](upload://iMNsTg0oqDcglYyqal9qT9KFUTF.jpeg) 

U mean this :slight_smile:

I just have to make a last review and then i ll go for an order...
```

---
## \#605 Posted by: sofu Posted at: 2019-02-11T09:41:24.460Z Reads: 194

```
Can I be put down for one :stuck_out_tongue:
```

---
## \#606 Posted by: Sn4pz Posted at: 2019-02-11T12:02:03.338Z Reads: 195

```
Oh jeez is this the closest it's gonna get to buying one completely made? :eyes: 

I want I want I want I want
```

---
## \#607 Posted by: yelnats8j Posted at: 2019-02-11T12:33:50.099Z Reads: 194

```
Me want, but I doubt id be able to make it :sleepy:
```

---
## \#608 Posted by: Mudders Posted at: 2019-02-11T13:49:38.674Z Reads: 195

```
I want 2 badly, i think i have next to no chance of making one and it actually working, but i may give it a go just to see.
```

---
## \#609 Posted by: Arek Posted at: 2019-02-11T17:39:08.886Z Reads: 197

```
Those mounting holes on the bottom seem kinda broken, way too close to the PCB, manufacturer may complain.
Did you add a low pass filter for the RF module?
Pls put there USB type-c, it's time to switch from micro :stuck_out_tongue:
Have you used a bit bigger holes for the connectors?
I see all tracks the same width, power lines should be a bit thicker.
Also would be nice to have a SMD antenna.
That USB connector has two big pads, slap 4 tiny vias on each so it will be stronger.
You decided to keep THT hall sensor?
Thought you going for SMD one...
You added 3rd mounting hole, thanks!

Just my 2 cents 🤣
```

---
## \#610 Posted by: StefanMe Posted at: 2019-02-12T08:22:39.171Z Reads: 202

```
> Those mounting holes on the bottom seem kinda broken, way too close to the PCB, manufacturer may complain.

Easy for JLCPCB :stuck_out_tongue: They will tell me this on the review.

>  Did you add a low pass filter for the RF module?

Do u have any document showing its recomented`? I think there is already one on the most RF69 moduls. Any suggestions about inductions and capacty?

> Have you used a bit bigger holes for the connectors?

No, i tested them on my original JST connectors and they are just fine.

> I see all tracks the same width, power lines should be a bit thicker.

Look closer, they are already thicker

> Also would be nice to have a SMD antenna.

I ll think about it... maybe a pcb antenna...

Ah ok thanks!

> You decided to keep THT hall sensor? Thought you going for SMD one…

Look closer again ;)

> You added 3rd mounting hole, thanks!
:grinning:
```

---
## \#611 Posted by: yelnats8j Posted at: 2019-02-14T04:12:37.849Z Reads: 191

```
Has anyone built the pcb them self?
like ordered from PCBways and assembled it?
```

---
## \#612 Posted by: tardyparty7 Posted at: 2019-02-14T04:55:30.579Z Reads: 199

```
scroll up. ⬆️
```

---
## \#613 Posted by: StefanMe Posted at: 2019-02-14T08:03:01.997Z Reads: 204

```
![image|666x500](upload://oFi6wVgxOkKZVG0wnbSjqxq7ojh.jpeg)
```

---
## \#614 Posted by: directC Posted at: 2019-02-14T22:17:38.507Z Reads: 199

```
How much would it cost and how long would it take tro get this remote?
looks very promising
```

---
## \#615 Posted by: X09 Posted at: 2019-02-15T02:51:32.103Z Reads: 195

```
If its available, count me in!
```

---
## \#616 Posted by: Sn4pz Posted at: 2019-02-15T02:52:18.565Z Reads: 196

```
theyre not, unfortunately.... maybe if we all beg hard enough :sob:
```

---
## \#617 Posted by: Gaza65 Posted at: 2019-02-16T10:20:59.888Z Reads: 192

```
Do you sell any that is already binded to receiver ready to go?
```

---
## \#618 Posted by: Chupacabra Posted at: 2019-02-18T18:01:51.013Z Reads: 187

```
@StefanMe Ive been waiting to order forever bro.
```

---
## \#619 Posted by: Sn4pz Posted at: 2019-02-18T18:19:33.882Z Reads: 191

```
I wish he would do another run :L 

If you convince him please PM and let me know :rofl:
```

---
## \#620 Posted by: schofieldbrandon Posted at: 2019-02-20T22:16:06.185Z Reads: 178

```
mild begging :)
```

---
## \#621 Posted by: dcxeternal Posted at: 2019-02-20T22:23:52.972Z Reads: 175

```
OMG this is everything that I want in a DIY remote.  I am new to this hobby. I just got a Meepo NLS last month and I already want to mod it.  Would the display work with Focbox Unity? I would assume so since it can run VESC right?

Please sell a batch of this soon please!!
```

---
## \#622 Posted by: StefanMe Posted at: 2019-02-23T13:26:16.908Z Reads: 172

```
Sorry guys I out for a while here. Got fucked by police. They took my board and two remotes with them. I l ll finish the orders of course and keep u informed.
```

---
## \#625 Posted by: Benjamin899 Posted at: 2019-02-23T14:35:48.445Z Reads: 167

```
@StefanMe jesus, that is my nightmare. still riding outside of view. I just hope the law gets passed soon
```

---
## \#626 Posted by: PickSix24 Posted at: 2019-02-23T15:42:36.857Z Reads: 172

```
That’s sucks man , good luck getting your stuff back.
```

---
## \#627 Posted by: Gaza65 Posted at: 2019-02-28T03:37:06.375Z Reads: 171

```
Do you have any left?
```

---
## \#628 Posted by: tardyparty7 Posted at: 2019-02-28T05:31:36.424Z Reads: 169

```
@StefanMe how'd u do the lanyards?
```

---
## \#629 Posted by: StefanMe Posted at: 2019-02-28T08:46:21.690Z Reads: 168

```
The us versions doesnt have a lanyard. U can simply add one if u want... on the bottom of the remote are two holes for that.
```

---
## \#630 Posted by: tardyparty7 Posted at: 2019-02-28T21:02:50.357Z Reads: 167

```
do u recommend anything?
```

---
## \#631 Posted by: StefanMe Posted at: 2019-02-28T22:02:49.673Z Reads: 165

```
I used Paracord without the inner strands
```

---
## \#632 Posted by: bevilacqua Posted at: 2019-02-28T23:28:54.164Z Reads: 160

```
I used a thin braided cable sleeve.
```

---
## \#633 Posted by: Darkie02 Posted at: 2019-03-03T20:37:00.966Z Reads: 161

```
So what’s happaning about remotes? It’s still not arived. I payed 18 November. The last message iv had was been sent out 2 weeks ago but it’s not arived and still no tracking number. Is any one els in the same situation? I think iv been reasonable and patient but feel otheres should be aware in the community of what’s happening now that it’s been so long.
```

---
## \#634 Posted by: StefanMe Posted at: 2019-03-03T21:06:26.728Z Reads: 165

```
Yeah I am sorry man. The police got my board and two remotes. I ll call them tomorrow when I get back everything, if u want, u ll get a full refound.
```

---
## \#635 Posted by: M.Hboards Posted at: 2019-03-04T00:40:51.086Z Reads: 165

```
@StefanMe any clue when the next batch will be? Also how much have you been selling these at?
```

---
## \#636 Posted by: tomiboi Posted at: 2019-03-05T02:24:30.883Z Reads: 167

```
I'm working on an accessible adaptation of this remote that does not use a 3-D printer... and proto-shields instead of custom PCB :) I found a very well-made hall-sensored, thumb-wheel that I'm going to try out. For a little extra money I can get a dual-sensored version. The additional hall-sensor is a safety redundancy feature. It requires an different power source and signal input on the feather. Could anybody give advice about adjusting the code to accommodate the second hall sensor. There would have to be some kind of signal to indicate that one of the sensors is not working as well. God forbid anybody would be riding around thinking that they have two sensors when, in fact, they only have one:)
```

---
## \#637 Posted by: StefanMe Posted at: 2019-03-05T05:43:33.696Z Reads: 155

```
Haha ok, shoulnt not be a problem to implement this... at least in the code.
```

---
## \#638 Posted by: tomiboi Posted at: 2019-03-06T03:45:17.041Z Reads: 165

```
Thanks for the reply:) And great remote. I have a few remote projects that I am working on using the Feather M0. I look forward to sharing them soon.
```

---
## \#639 Posted by: tomiboi Posted at: 2019-03-06T17:58:51.322Z Reads: 162

```
The initial wiring problem is pretty big. There isn’t a secondary power source. There are plenty of inputs. The ground is common. Just no second power source.. I think. Here is a link to the switch if you or anyone else is interested [https://ruffycontrols.com/msa-series/](https://ruffycontrols.com/msa-series/)
They are used in military and aerospace applications. Accuation and spring force can be customized.
```

---
## \#640 Posted by: Leander Posted at: 2019-03-06T19:32:45.532Z Reads: 162

```
Hello, i was just wondering if there is a schematic for the wireing so i could make my own pcb?
```

---
## \#641 Posted by: Mich21050 Posted at: 2019-03-06T19:33:35.626Z Reads: 167

```
Come on.. Read the title... :slight_smile:
https://www.electric-skateboard.builders/t/featherremote-and-smartremote-files-in-post-577/74084/589?u=mich21050
```

---
## \#642 Posted by: Leander Posted at: 2019-03-06T19:40:21.006Z Reads: 154

```
I read that, but i didnt know if their was a schematic. I clicked on the pcb and there is a gerber file which i could work from but a schematic is better.
```

---
## \#643 Posted by: Touch415 Posted at: 2019-03-09T20:36:45.614Z Reads: 151

```
Got my feather remote in, did a test ride and  it’s amazing how many times this thing disconnect super annoying, it’ll vibrate and show “estop” with a timer,  has anyone had any issues with the remote disconnecting or maybe something is wrong or need to upgrade the software or maybe this remote isn’t made for big cities like SF with lots of interference.. i think I’m going back to my firefly if I can’t fix this problem ..
```

---
## \#644 Posted by: StefanMe Posted at: 2019-03-09T21:06:26.128Z Reads: 144

```
I ll write u per PM
```

---
## \#645 Posted by: jimmymagix Posted at: 2019-03-09T21:11:34.103Z Reads: 148

```
Can you let me know what you said in a PM to me too? 

I bought one in the recent batch but I haven't had chance to use it yet as my board is in pieces until mid April. This is the second occasion in as many days that I've heard that there's issues with the connectivity so I want to get ahead of the curve if there are things I can do to ensure it works, first time.
```

---
## \#646 Posted by: StefanMe Posted at: 2019-03-09T21:18:20.379Z Reads: 149

```
I ll write an guide if u have connection issues...
```

---
## \#647 Posted by: Touch415 Posted at: 2019-03-09T22:16:49.982Z Reads: 162

```
I’m super curious if anyone had this issue with connectivity on the feather remote it’s super annoying riding around with vibrating dildo all the time 😩😩😩  i live in SF with freaking hills would hate for this remote to cut out completely or even at high speeds..  please @StefanMe send over that guide or anything I need to do ...👍🏼
```

---
## \#648 Posted by: pookybear Posted at: 2019-03-09T22:53:57.492Z Reads: 166

```
Yes I did. I had to route my remote antenna to the lanyard holes. This was suggested by the man himself, @StefanMe 

![IMG_20190306_105847|375x499](upload://ICbKhiOPjV5efkYjvovwcOI0XR.jpeg) 

And to be safe, I upgraded receiver antenna to [this](https://www.amazon.com/dp/B01M2BR2ZD/ref=cm_sw_r_other_apap_lqxVB3t1CUPk8). This is on a hummie deck that I believe has CF layers.
```

---
## \#649 Posted by: PickSix24 Posted at: 2019-03-09T22:54:21.277Z Reads: 160

```
I don’t want to speak on your particular issue but my first batch remote did the same thing
```

---
## \#650 Posted by: pookybear Posted at: 2019-03-09T22:56:03.080Z Reads: 161

```
I almost upgraded my remote antenna to that link but routing the remote antenna through the lanyard holes fixed my issue.
```

---
## \#651 Posted by: PickSix24 Posted at: 2019-03-09T22:56:16.715Z Reads: 158

```
Those look to be 2.4ghz , the feather runs on 915
```

---
## \#652 Posted by: pookybear Posted at: 2019-03-09T22:56:35.916Z Reads: 155

```
It is on 915mhz.
```

---
## \#653 Posted by: PickSix24 Posted at: 2019-03-09T22:56:54.204Z Reads: 153

```
I take it you cut the antenna to the proper length
```

---
## \#654 Posted by: pookybear Posted at: 2019-03-09T22:57:15.679Z Reads: 150

```
Yes. 10 charizard

Edit:
I didn't cut any in the internal remote antenna.
```

---
## \#655 Posted by: PickSix24 Posted at: 2019-03-09T22:57:45.088Z Reads: 148

```
Ah got it , just checking. That would be an issue otherwise ! Lol
```

---
## \#656 Posted by: pookybear Posted at: 2019-03-09T22:59:20.848Z Reads: 147

```
I get better reception w the "upgraded" antenna than the stock.
```

---
## \#657 Posted by: pookybear Posted at: 2019-03-09T23:00:37.763Z Reads: 147

```
You got my curious now. Haha. What is this property length you speak of?
```

---
## \#658 Posted by: PickSix24 Posted at: 2019-03-09T23:29:25.966Z Reads: 143

```
I was just saying that every transmission band has a specific antenna wavelength, 2.4 , 5.8 , 915mhz etc
```

---
## \#659 Posted by: pookybear Posted at: 2019-03-09T23:31:53.484Z Reads: 146

```
Oh wavelength. Gotcha.
```

---
## \#660 Posted by: Touch415 Posted at: 2019-03-10T01:54:23.157Z Reads: 150

```
Thanks guys, going to give a shot 👊🏼👊🏼
```

---
## \#661 Posted by: jimmymagix Posted at: 2019-03-10T06:52:39.155Z Reads: 147

```
Can you not just forward me the guide now? I have a carbon GT so connection issues are pretty much guaranteed.
```

---
## \#662 Posted by: bevilacqua Posted at: 2019-03-10T10:05:06.305Z Reads: 147

```
isn't the top lid made out of fiberglass?
```

---
## \#663 Posted by: Arek Posted at: 2019-03-10T10:29:24.170Z Reads: 155

```
Might be working but you still have the wrong antenna.
You shouldn't really use 2.4GHz antenna on a 0.915GHz transmitter.
Search for 915MHz antenna.
I myself put just a piece of wire calculated for my frequency (433) at 1/4 of the wavelength, don't remember but I think it was 16cm, works well 10 meters of range through few walls (in house test).
But still haven't tested it in a real case scenario (esk8) as I'm still waiting for unity...
```

---
## \#664 Posted by: jimmymagix Posted at: 2019-03-10T11:11:17.061Z Reads: 150

```
I don't think so... I think the original Raptor had a carbon fiber enclosure that was replaced with fiberglass. As far as I've found the battery cover is CF. 

I may be mistaken however.
```

---
## \#665 Posted by: pookybear Posted at: 2019-03-10T16:53:49.163Z Reads: 151

```
Yeah, I realized that when I was reading about it last night.

I don't need 10 meters of range though. Stefan made a good point about having a longer range in pm when we were trying to figure the connection out. You would want your remote to activate estop right away in a shorter distance from you just in case it malfunctions so you don't get a runaway skateboard.

Thanks for the heads up.
```

---
## \#666 Posted by: Surfer Posted at: 2019-03-10T17:20:51.910Z Reads: 145

```
Oh yes, that guide / update would be nice, I have micro connection drops, for less than a second or so, since the beginning, but yeah I thought it was because of the haya aluminium lid, but it's not the case, as is now installed the nano X and going strong, no drops. Already play with the antenna, inside, outside, solid copper, stranded copper, longer, shorter... In my case It looks like it has better connection a bit far away.
```

---
## \#667 Posted by: Arek Posted at: 2019-03-10T17:55:25.497Z Reads: 148

```
Just buy some antenna suited for your freq.
And yeah usually better to place antenna outside.
Can also try to change the orientation.
Also if you can go for lower freq. it gets through solid objects better just like sound.

Next custom feather has to have proper quality antenna with proper PCB layout.
```

---
## \#668 Posted by: totalgeek9224 Posted at: 2019-03-10T18:18:49.504Z Reads: 140

```
Could you detail this more? Are you running the latest firmware? And are there conditions that consistently cause the micro drops?
```

---
## \#669 Posted by: StefanMe Posted at: 2019-03-10T19:03:19.425Z Reads: 138

```
What does the dBM values on the CONNECTION page say if u stay on the board? Can u show me the antenna on the remote... Is it outside or inside enclosure?
```

---
## \#670 Posted by: Touch415 Posted at: 2019-03-10T19:23:26.347Z Reads: 149

```
45-50 with the antenna coming out the lanyard, going to try to upgrade the antenna on the receiver on the board  to see if anything changes.. I’m running a carbon deck and enclosure 😬😬😬 but the old faithful nano X works no problem with not one drop out ..
```

---
## \#671 Posted by: StefanMe Posted at: 2019-03-10T19:32:19.274Z Reads: 152

```
WHY?! 40-50dBm is awesome...  don't touch it.
```

---
## \#672 Posted by: Touch415 Posted at: 2019-03-10T19:34:50.095Z Reads: 158

```
![image|375x500](upload://h1NSmreYTKsgiN5lOfkGRfdzw7M.jpeg)
```

---
## \#673 Posted by: StefanMe Posted at: 2019-03-10T19:38:21.636Z Reads: 154

```
My remote works awesome... lets change something :rofl:

Keep it. This is a awesome connection. Everything under 60 is awesome. Under 70 ok.
```

---
## \#674 Posted by: Touch415 Posted at: 2019-03-10T19:42:56.820Z Reads: 144

```
That was the exact same number I had with the antenna inside   the remote  didn’t make any difference in signal, so I’m pretty sure it’s going to be same issue .. il give it a try again👍🏼
```

---
## \#675 Posted by: Arek Posted at: 2019-03-10T20:06:32.589Z Reads: 146

```
Perhaps remote isn't the problem, may be it's problem on the receiver side.
If you have carbon fiber deck then antenna must be outside.
```

---
## \#676 Posted by: StefanMe Posted at: 2019-03-10T20:10:29.077Z Reads: 147

```
No because both values are good... one is the dbm to receiver and the bottom one from receiver to remote.
```

---
## \#677 Posted by: Touch415 Posted at: 2019-03-10T20:32:11.763Z Reads: 145

```
Why does my nano and even firefly work good with my carbon setup ..🤷🏻‍♂️🤷🏻‍♂️ But il give it try and hopefully I get this connection issues worked out because the feather remote is very nice..
```

---
## \#678 Posted by: Arek Posted at: 2019-03-10T20:36:12.770Z Reads: 141

```
Well yeah you're right but he actually made the photo in a postion that he's not riding in, if he's to the side of the board which is the shield then it will have better signal.
```

---
## \#679 Posted by: pookybear Posted at: 2019-03-10T20:38:43.596Z Reads: 139

```
Take a pic of the remote while being on your board (not riding it for safety purposes).
```

---
## \#680 Posted by: pookybear Posted at: 2019-03-10T20:41:53.009Z Reads: 147

```
I just went for a ride. No connectivity issues. Pretty solid now.
```

---
## \#681 Posted by: sofu Posted at: 2019-03-10T20:46:02.667Z Reads: 152

```
I'm fairly certain there's some issue with interference that isn't being seen here. I have the same remote and @Touch415 and I ride together almost every weekend. I got my remote a couple months before he did and I also have the same issues as him. It will start cutting out around certain areas of town but the dbm remains below 60. We're in SF so I can highlight some places where Feather with transmitter and receiver antennas has gotten cutouts but my Firefly based remote with no antenna hasn't:

- Chinatown
- Twin Peaks around the tower
- Embarcadero and Broadway

Would love to see this fixed or figured out, it's a bit annoying :P
```

---
## \#682 Posted by: Touch415 Posted at: 2019-03-10T20:46:46.697Z Reads: 147

```
Nice👍🏼👍🏼,  ....
```

---
## \#683 Posted by: StefanMe Posted at: 2019-03-10T21:18:00.250Z Reads: 142

```
We can give it a try to change the frequency to 868Mhz... maybe it helps.
```

---
## \#684 Posted by: sofu Posted at: 2019-03-10T22:33:49.412Z Reads: 140

```
Is that the euro frequency? I can do the change and see
```

---
## \#685 Posted by: Touch415 Posted at: 2019-03-10T23:24:51.836Z Reads: 139

```
@sofu get on it 😜😜🙏🏼🙏🏼🙏🏼
```

---
## \#686 Posted by: totalgeek9224 Posted at: 2019-03-11T08:03:03.009Z Reads: 134

```
Euro is 433hz, and requires a different feather board I believe, so not quite :p
```

---
## \#687 Posted by: StefanMe Posted at: 2019-03-11T08:19:40.629Z Reads: 139

```
[quote="totalgeek9224, post:686, topic:74084"]
s a differe
[/quote]

The RFM modules are specified for 433Mhz or 868-915Mhz.

@sofu if u find some time, please make some tests... go for 915 with a double lenght antenna. Normaly u use a LAMDA 1/4 Anntenna lenght: ~7,8mm. We Can try to use a LAMDA 1/2 Antenna lenght (stick more out of the remote ect.) with ~15.6mm.

If this doesnt helpt We can try the 868Mhz... EDIT: It looks like this is not allowed in US without an HAM amateuer licence. We could still try it out... 

Both should be valid in US. I ll check this later. 433Mhz is not very good with your RFM Module.

If u really want to make it as best as possible, make the antenna longer and place it on a table a few meters away from the board... then start to cut mm for mm the antenna lenght until u find the lowest dBm. Then do the same on the receiver.
```

---
## \#688 Posted by: sofu Posted at: 2019-03-11T10:01:50.255Z Reads: 133

```
Should I double the length on the receiver as well?
```

---
## \#689 Posted by: StefanMe Posted at: 2019-03-11T10:51:17.120Z Reads: 135

```
why not.... should help. But take a place before where u can veryfi the dBm. To have a reference
```

---
## \#690 Posted by: PickSix24 Posted at: 2019-03-11T17:04:58.402Z Reads: 137

```
Another option for 915mhz are these if they fit. I used these on Nano before with good results

https://express.google.com/u/0/product/3211580873691550647_7536716834951528046_100003215?utm_source=google_shopping&utm_medium=tu_cu&utm_content=eid-lsjeuxoeqt&gtim=CO__lLS4loSaVhDwmc3Ao-m5-ZkBGPDM7QIiA1VTRCiQitbkBTCP29cv&utm_campaign=100003215&gclid=Cj0KCQjwjpjkBRDRARIsAKv-0O1Pxx6BQDrIOC0tU7rTDhGIRVwVakB_AxftEEmX8op07i9MHrZizkgaAovBEALw_wcB
```

---
## \#691 Posted by: PickSix24 Posted at: 2019-03-12T02:11:39.904Z Reads: 144

```
Remote showed up today ! 
![image|375x500](upload://cf5tyMqnh1pQ8mOxGjW4lMqzePq.jpeg)
```

---
## \#692 Posted by: sofu Posted at: 2019-03-12T05:05:08.326Z Reads: 140

```
I also just bought some antenna hardware to test. ufl smd connector, ufl to sma adapter, and a patch antenna just for kicks. We'll see how it goes...
```

---
## \#693 Posted by: PickSix24 Posted at: 2019-03-16T23:26:54.026Z Reads: 134

```
@StefanMe or can anyone walk me through what part of the code needs to be changed to switch between VESC and UNITY uart
Didn’t see anything about this in the update manual
```

---
## \#694 Posted by: totalgeek9224 Posted at: 2019-03-17T10:08:46.957Z Reads: 140

```
Ofcourse!
When you download the Transmitter (remote) code, and load it into the Arduino IDE, the first few lines that you will see are ![09|519x500](upload://6QH18zqwgMaYPOBql1Pk81nle6S.png) 

all you have to do is change it to 

![23|519x500](upload://kOmoj2Nl7n2KVLcuAlatwFH1GFH.png) 

where you've removed the // in front of the #define ESC_UNITY and instead put the // to the ESC_VESC
```

---
## \#695 Posted by: PickSix24 Posted at: 2019-03-17T14:31:13.568Z Reads: 126

```
Awesome thanks, that made it simple. One more question, any reason why after flashing the remote gets stuck at the feather logo ?
```

---
## \#696 Posted by: StefanMe Posted at: 2019-03-17T14:44:31.379Z Reads: 125

```
Can u post a picture of your setup section in the. Code please?
```

---
## \#697 Posted by: PickSix24 Posted at: 2019-03-17T14:56:14.062Z Reads: 133

```
![image|666x500](upload://cAkWikjRDfdd7iV7JL51QYqKekM.jpeg)
```

---
## \#698 Posted by: StefanMe Posted at: 2019-03-17T15:03:04.193Z Reads: 132

```
Looks just fine... and the remote does Lust freue after the Logo? U downloaded the latest code?

Can u try to upload the code again with VESC activated instead of Unity..?
```

---
## \#699 Posted by: PickSix24 Posted at: 2019-03-17T15:08:56.490Z Reads: 130

```
The screen just shows the logo screen, never gets past. 
I’ll switch it back to VESC and try again. Says version 8.0
```

---
## \#700 Posted by: pookybear Posted at: 2019-03-17T15:16:27.248Z Reads: 124

```
What does this do?
```

---
## \#701 Posted by: PickSix24 Posted at: 2019-03-17T15:22:29.747Z Reads: 123

```
No change, still stuck at the boot logo
```

---
## \#702 Posted by: StefanMe Posted at: 2019-03-17T15:24:16.777Z Reads: 120

```
After the logo starts up he want to try to send data. Looks like your RFM Module is not responding. 

Activate DEBUG and DEBUG_TRANSMISSION please. Upload the code and Open the serial Monitor.
```

---
## \#703 Posted by: PickSix24 Posted at: 2019-03-17T15:34:38.879Z Reads: 130

```
![image|374x500](upload://rcvN4R7kMxMCEL8FBgrECgqsEuT.jpeg)
```

---
## \#704 Posted by: StefanMe Posted at: 2019-03-17T15:42:31.077Z Reads: 117

```
Can unter to go directly into settings when u hold the menu button on startup and try to pair? Also with debug activated.
```

---
## \#705 Posted by: PickSix24 Posted at: 2019-03-17T15:44:52.552Z Reads: 114

```
The screen doesn’t light up in debug mode
```

---
## \#706 Posted by: StefanMe Posted at: 2019-03-17T15:54:44.720Z Reads: 119

```
U have to open the serial monitor... or close and open it again.
```

---
## \#707 Posted by: PickSix24 Posted at: 2019-03-17T16:02:42.260Z Reads: 129

```
Not sure if I did it right but this time I see this 
![image|374x500](upload://gz7AajjIOyeqPWwA5TkVepFMNDB.jpeg)
```

---
## \#708 Posted by: StefanMe Posted at: 2019-03-17T16:59:27.037Z Reads: 117

```
Let me.  Check something and we go online tomorrow.
```

---
## \#709 Posted by: StefanMe Posted at: 2019-03-18T08:13:23.968Z Reads: 120

```
Please check the latest code and activate DEBUG and DEBUG TRANSMISSION and show me whats going on in the serialn monitor. I extended the debug code for the RFM module.
```

---
## \#710 Posted by: totalgeek9224 Posted at: 2019-03-18T08:19:19.315Z Reads: 122

```
This is what he's asking you to do (just to confirm) 

The arrow(if you can call it that) is pointing to the button for the serial monitor (the magnifying glass looking one) just in case anyone didn't know.
![34%204|429x500](upload://yPWbdWrE0KGoJrEF53dEe4rvOqK.png)
```

---
## \#711 Posted by: StefanMe Posted at: 2019-03-18T08:26:10.189Z Reads: 120

```
not even I knew that there is this button :rofl:

I always go the long way: Menu, tools, serial monitor...

THX @totalgeek9224
```

---
## \#712 Posted by: Jansen Posted at: 2019-03-18T11:59:33.173Z Reads: 121

```
Just PM'd you @StefanMe Get back to me when you can if you could.
```

---
## \#713 Posted by: PickSix24 Posted at: 2019-03-21T03:31:08.833Z Reads: 123

```
![image|374x500](upload://p7pWTHDiHJlKZm4civcdHGHRcth.jpeg)
```

---
## \#714 Posted by: StefanMe Posted at: 2019-03-21T07:23:06.262Z Reads: 115

```
Looks like the RFM module is broken... :frowning: Strange... Can u please check the inner parts of the remote? Maybe u see something on the PCB. This is horrible. The RFM chip is solderd upside down and very well covered. I never had this before.
```

---
## \#715 Posted by: willumpie82 Posted at: 2019-03-21T07:27:53.222Z Reads: 120

```
or just hit CTRL+SHIFT+M / CMD+SHIFT+M
```

---
## \#716 Posted by: PickSix24 Posted at: 2019-03-21T14:15:46.238Z Reads: 121

```
I’ll take a look when I get home. I believe I still have a few feather boards left over from a firefly project. Are they the same ?
```

---
## \#717 Posted by: StefanMe Posted at: 2019-03-21T19:03:44.702Z Reads: 124

```
Intro to improve the PCB to make it more stable... removed the trigger and soldered it directly to the PCB. Works awesome 💪🏼

I ll release the files soon!

![image|690x388](upload://IC0tgtwIjn3KqOvKeSMa0j0m7Y.jpeg)
```

---
## \#718 Posted by: Jansen Posted at: 2019-03-21T20:12:07.936Z Reads: 119

```
Fuck YEAH! Just for me I hope? LOL. Just PM'd yo too so we can get me back on the road Stefan. Thanks for being on top of it.
```

---
## \#719 Posted by: PickSix24 Posted at: 2019-03-23T17:36:38.841Z Reads: 114

```
@StefanMe you were right. Removed the feather board and found a small resistor missing off the radio module. Installed a new feather board and programmed. Boots right up ! Thank you for the help.
```

---
## \#720 Posted by: StefanMe Posted at: 2019-03-23T17:57:53.926Z Reads: 116

```
WOW really? A missing resistor on the module? Thats strange. Maybe we can find out what resistor it is, then we can solder it onto the module and bring it back to life...
```

---
## \#721 Posted by: PickSix24 Posted at: 2019-03-23T18:31:31.565Z Reads: 119

```
![image|375x500](upload://chQcMv2FST2wOH7mHppIEGVC56.jpeg) 

Looks like it was a factory assembly issue. The arrows point to where the capacitor is misplaced and where it should go. Compared to all my other boards for reference.
```

---
## \#722 Posted by: StefanMe Posted at: 2019-03-23T18:33:07.610Z Reads: 116

```
I can also see a second one maybe missing... on the bottom left. I don't have a feather on hand at the moment. Maybe u can check this?
```

---
## \#723 Posted by: PickSix24 Posted at: 2019-03-23T18:46:23.418Z Reads: 114

```
That one is missing on all my boards
```

---
## \#724 Posted by: pookybear Posted at: 2019-03-26T15:01:47.996Z Reads: 112

```
Running the latest unity firmware here w my feather remote. Telemetry isn't working. Well, I see numbers when I throttle but it goes to xxx digits. It does this also while braking. Battery numbers aren't showing up either.

Just trying to rule out user error here. Is anyone experiencing this?
```

---
## \#725 Posted by: PickSix24 Posted at: 2019-03-26T19:26:19.090Z Reads: 120

```
During the feather board programming, the telemetry has to be setup for either VESC or Unity. It’s possible yours is on VESC, I’m not sure what @StefanMe defaults them to. 
It’s pretty easy to flash it again though, the manual is pretty detailed.
```

---
## \#726 Posted by: pookybear Posted at: 2019-03-26T19:45:34.896Z Reads: 119

```
Got a link to this firmware?
```

---
## \#727 Posted by: PickSix24 Posted at: 2019-03-26T20:40:09.198Z Reads: 115

```
https://docs.google.com/document/d/1o8movyzRRjtOmOapchsGz1GvywfiZTdPu-UPitXVH_4/mobilebasic
```

---
## \#728 Posted by: PickSix24 Posted at: 2019-03-26T20:41:00.727Z Reads: 121

```
https://github.com/StefanMeGit/FeatherM0-Esk8-Remote
```

---
## \#729 Posted by: pookybear Posted at: 2019-03-27T17:15:02.447Z Reads: 119

```
So I'm trying to update my feather remote and receiver to get the telemetry to work on the unity. I followed the steps to updating it except I'm stuck on this step. Where do I find this remote.ide?

![feather|690x388](upload://82AM6daL0RW76Fm5PcSDcuYftaD.png) 

Thanks in advance!

[Link](https://docs.google.com/document/d/1o8movyzRRjtOmOapchsGz1GvywfiZTdPu-UPitXVH_4/mobilebasic) to the steps.
```

---
## \#731 Posted by: Mich21050 Posted at: 2019-03-27T17:17:35.261Z Reads: 115

```
https://www.electric-skateboard.builders/t/featherremote-and-smartremote-files-in-post-577/74084/589?u=mich21050
10dif
```

---
## \#733 Posted by: kiryl Posted at: 2019-03-28T23:40:36.643Z Reads: 111

```
Ok, I got the latest updates for the remote and receiver, but I'm not getting any info displayed on the remote. I have checked settigns and the wires but nothing seems to be working. Anyone knows how to fix it? I'm using an unity
```

---
## \#734 Posted by: pookybear Posted at: 2019-03-29T01:24:13.595Z Reads: 114

```
Have you commented out the 
#define Vesc 

And uncomment
#define unity

Make sure you do this to RF USA also. Upload using Arduino.
```

---
## \#735 Posted by: kiryl Posted at: 2019-03-29T07:33:07.478Z Reads: 112

```
Yes I have done that step in the arduino files. Still no data on my remote. Also, the screen of the remote is black when I turn it on and showing nothing 70% of the time.
```

---
## \#736 Posted by: StefanMe Posted at: 2019-03-29T07:46:00.684Z Reads: 114

```
Can u send me a picture of the remote inside? Per DM please... I want to check something on the PCB.
```

---
## \#737 Posted by: kiryl Posted at: 2019-03-29T09:54:23.757Z Reads: 114

```
I'm at work atm, I will send you a pic this eavening
```

---
## \#738 Posted by: sofu Posted at: 2019-03-30T20:49:44.733Z Reads: 121

```
Well, vibration doesn't take kindly to the components... Everything falling off :P

![image|666x500](upload://xSW9o4sh6pV925R3X6buW5TNTfP.jpeg) 

Ended up having to solder a cap back on the weird way cause I was getting cutouts every 10 seconds without it...

![image|375x500](upload://qcFsA0w7xJdevVrxdSpWrtGaSXI.jpeg) 

Hot glue or silicon your receivers everybody... 

Also I found out the advanced receiver breakout board was draining my battery... ~1V off if I let it sit for a day or two...
```

---
## \#739 Posted by: mishrasubhransu Posted at: 2019-03-30T21:05:48.200Z Reads: 115

```
I have had that once at the very start and since then I aways shock mount my electronics. Never happened again.
```

---
## \#740 Posted by: sofu Posted at: 2019-03-30T21:21:37.336Z Reads: 117

```
@StefanMe what is that cap for? Why do I get cutouts every time I go over a bump without the cap?
```

---
## \#741 Posted by: Arek Posted at: 2019-03-30T21:27:26.720Z Reads: 121

```
Might not have been soldered correctly(dry joint), this package is hard to solder and only proper reflow would do that properly.
But I would prefereably use tantalum capacitors, two 220uF would do the trick as a replacement for that 1000uF electrolytic that fell off, you don't need that much filtering just for a LED regulator.

I actually just put my receiver into a heatshrink tube that is intended for wrapping 18650 cells, should keep that capacitor in place as well:
![IMG_20190330_212359|690x388](upload://d2GSKWTH3ZuMO9hcxVRGGSHDcFk.jpeg)
```

---
## \#742 Posted by: StefanMe Posted at: 2019-03-30T21:30:45.311Z Reads: 117

```
U mean u get cutouts from the missing capacitor on the extension board? 

Its this one:

![image|375x500](upload://s1Cy23GQFibePoyLqjrI76qeLZW.jpeg)
```

---
## \#743 Posted by: sofu Posted at: 2019-03-30T22:16:21.326Z Reads: 116

```
I meant the one that fell off the basic receiver

![image|374x500](upload://3PjVbih8fZSN6JbcI9Kp6ldJ9ma.jpeg)
```

---
## \#744 Posted by: StefanMe Posted at: 2019-03-30T22:39:07.916Z Reads: 109

```
Normally it shouldn't be a problem, but maybe now the coil is to big (for the LC filter) What capacitor are u using?

I use this one:
https://lcsc.com/product-detail/Others_Lelon-OVZ221M1ATR-0606_C311623.html
```

---
## \#745 Posted by: Steven1 Posted at: 2019-03-30T22:45:11.292Z Reads: 108

```
How is everyone fairing with their remote? Is the antenna issue fixed?
```

---
## \#746 Posted by: StefanMe Posted at: 2019-03-30T23:09:43.834Z Reads: 106

```
its not an antenna issue... its an OLED issue.
```

---
## \#747 Posted by: Steven1 Posted at: 2019-03-30T23:29:34.933Z Reads: 106

```
Ok, sry didnt realize.
```

---
## \#748 Posted by: sofu Posted at: 2019-03-31T00:16:55.629Z Reads: 106

```
I use the original one that was on there
```

---
## \#749 Posted by: pookybear Posted at: 2019-03-31T06:59:37.901Z Reads: 107

```
I replaced mine with [this](https://www.amazon.com/dp/B01IR31KF0?ref=ppx_pop_mob_ap_share). Seems to be holding up.
```

---
## \#750 Posted by: Zentaria Posted at: 2019-03-31T11:18:34.854Z Reads: 105

```
Hey guys, having some issues with my remote and board recently. My Remote couldnt find the board and now I updated it and it still cant find it. I tried to pair the Remote with the board again but it doesnt find the board (I did it exactly like in the Manual). Any other tips I could try?
```

---
## \#751 Posted by: StefanMe Posted at: 2019-03-31T13:05:54.544Z Reads: 104

```
Have I set up the same RFM_EU on remote and receiver?
```

---
## \#752 Posted by: Zentaria Posted at: 2019-03-31T13:16:13.088Z Reads: 104

```
By default on the receiver source there was US declared. But I chose EU and it still didn't work. And both says 433.0
```

---
## \#753 Posted by: Zentaria Posted at: 2019-03-31T13:22:30.852Z Reads: 110

```
Oh and I can pair the remote when the Receiver is connected via USB. When I use the VESC standalone it doesnt work. When both (VESC + USB) is connected I still have connection, as soon as I unplug the USB i get disconnected...
```

---
## \#754 Posted by: wafflejock Posted at: 2019-03-31T13:31:03.001Z Reads: 111

```
It may be that the voltage regulator on the VESC responsible for putting out 5V is overloaded (too much amperage to drive the MCU and transceiver reliably) and so when giving it 5V over USB it may be okay.  I use an arduino pro mini 3.3V+nrf24l01 for my custom transmitter/receiver and also have a cap on the power input for the receiver to help avoid brown outs if the nrf24 is taking more power at any point in time.

---

Edited since previous post was edited.
```

---
## \#755 Posted by: Zentaria Posted at: 2019-03-31T13:38:02.629Z Reads: 105

```
Well it worked for a couple of weeks perfectly fine, what could be the cause of this?
```

---
## \#756 Posted by: StefanMe Posted at: 2019-03-31T15:33:01.797Z Reads: 101

```
What did u chose here:

// - Choose board version:
//#define BOARD_V0_1        // BOARD_V0_1 no status LED, Breaklight pin 13, Headlight pin 12, Status led pin 9
#define BOARD_V0_2          // BOARD_V0_2 no status LED, Breaklight pin 13, Headlight pin 12, Status led pin 9

Please try the Bord v02 and Tell me what the red led is doing on USB and on VESC
```

---
## \#757 Posted by: PickSix24 Posted at: 2019-03-31T16:03:00.515Z Reads: 98

```
Went for a long ride yesterday. Hummie deck with carbon fiber , no issues.
```

---
## \#758 Posted by: PickSix24 Posted at: 2019-03-31T16:05:41.308Z Reads: 101

```
OLED issue ?
```

---
## \#759 Posted by: pookybear Posted at: 2019-03-31T16:54:40.503Z Reads: 100

```
My thoughts exactly too. All I had to do on mine was change the antenna. It's pretty solid now.
```

---
## \#760 Posted by: Zentaria Posted at: 2019-03-31T17:33:18.596Z Reads: 104

```
I used v0_2.

The red Light is constantly on when I use the Vesc. 

When I use USB it flashes every second.

(both when the remote is turned off).
```

---
## \#761 Posted by: Sn4pz Posted at: 2019-03-31T17:35:22.245Z Reads: 104

```
Can you link to the post you made about that? If you did make one. Im worried about the connectivity of the remote in my trampa, and would like to have documented working options :D
```

---
## \#762 Posted by: StefanMe Posted at: 2019-03-31T17:43:52.364Z Reads: 101

```
can I show me a picture? Looks like the power connection over the JST connector is not correct. The „blinking“ is correct.
```

---
## \#763 Posted by: pookybear Posted at: 2019-03-31T17:46:07.960Z Reads: 109

```
You should try it first. If it's sketchy, switch out the antenna. Built-in antenna works but not as solid. Well at least around my area. 

Unfortunately, documentation of such "mods" was done through pms. I'll dig up some pics. 

@Touch415 has done this as well. 

![b0668e9cbc20aea305aef83efdbaf437916a7c06_2_750x1000|375x500](upload://8zWiFfubVaYOWitEvKp4y9n1SUV.jpeg) 

This is the only decent pic I have of it. I took it when I was asking Stefan what cap is comparable to what he has/had on my receiver.

I highly suggest shrink warp around the receiver.
```

---
## \#764 Posted by: Sn4pz Posted at: 2019-03-31T17:47:20.274Z Reads: 105

```
[quote="pookybear, post:763, topic:74084"]
I highly suggest shrink warp around the receiver.
[/quote]


Why do things wiggle off occasionally without it on? I cant imagine it helps connectivity?
```

---
## \#765 Posted by: Zentaria Posted at: 2019-03-31T17:48:20.050Z Reads: 100

```
You mean a picture from Receiver to Vesc?
```

---
## \#766 Posted by: StefanMe Posted at: 2019-03-31T17:49:13.940Z Reads: 104

```
Receiver please...
```

---
## \#767 Posted by: pookybear Posted at: 2019-03-31T17:49:26.602Z Reads: 104

```
I mainly did this to protect any unforseen water ingress, which I did a terrible job because some are not even covered. :rofl:

I wanted easy access to the ports.
```

---
## \#768 Posted by: Sn4pz Posted at: 2019-03-31T17:55:05.968Z Reads: 110

```
Hmm ok, I guess I should do that as well :thinking:

Didnt you make a post some time ago asking how to connect the feather remote and a metr module? Im very interested in knowing that process as well :P
```

---
## \#769 Posted by: Zentaria Posted at: 2019-03-31T18:07:39.171Z Reads: 113

```
![IMG_20190331_200655|690x388](upload://dpGzVH0SpZdvzZwinissUw1fdnf.jpeg)
```

---
## \#770 Posted by: pookybear Posted at: 2019-03-31T18:08:07.705Z Reads: 114

```
Super easy with focboxes. Manual is pretty documented on how to do this.

Unity is different. You need to use the internal UART for the remote. I'm having too much fun riding the board. I'll eventually do some testing again to make feather work w internal UART pins and have metr connect through external one.

@sofu has both working. I believe she has remote connected internally and metr externally. This requires a different firmware tho. Look up her haya build thread. It's all there.

Send me your address. I'll send you a few antennas if it doesn't work. I have 2.4ghz antennas as well as 915mhz ones. I'm currently using 2.4ghz antenna. I should really switch but it's working pretty good right now :man_shrugging: I'll eventually switch it but why fix when it's not broken?
```

---
## \#771 Posted by: Sn4pz Posted at: 2019-03-31T18:11:10.860Z Reads: 109

```
Awesome! Pming
```

---
## \#772 Posted by: Touch415 Posted at: 2019-03-31T19:31:08.758Z Reads: 107

```
My thoughts on the feather remote if you live in big cities I don’t recommend this remote at all, real talk unless you like the annoying disconnects.. I upgraded the antenna which help lil and also upgrade the whole charging port since mine was defective which @StefanMe kinda disappears wen you have major issues for $200 not worth the pain.. @sofu receiver fell apart and also had a major disconnect going down a hill 😲 ..
```

---
## \#773 Posted by: StefanMe Posted at: 2019-03-31T19:35:21.264Z Reads: 109

```
U can say a lot about the remote, but u can’t say that I don’t take care of the issues. Anyway. I ll not sell the remote anymore. That’s why I published all the files and di just a very small batch with a very new Version where I can control the issues much better.

It’s a bit strange. I live in a city with 1.3 Million People and dont have any disconnects. Even when @bevilacqua is riding next to me with the exact same remote.
```

---
## \#774 Posted by: pookybear Posted at: 2019-03-31T19:44:57.521Z Reads: 112

```
There are always hiccups w DIY man. Don't let stuff like these discourage you. There could be some unknown variables us USA folks are experiencing that you dont have. You are doing amazing work. I'd buy again from you for sure.

I met up w @thisguyhere because I was having battery issues he sold me. Guess what. It was user error. He found it was my charging port. Damn three prongs. I did continuity check after I soldered. Apparently, the one I used was not meant for charging. Probably ground. It pass the neg continuity check!

We went for a ride around his area. No disconnects!
```

---
## \#775 Posted by: Touch415 Posted at: 2019-03-31T19:46:13.902Z Reads: 107

```
Buy mines 😆👍🏼 Half the price
```

---
## \#776 Posted by: pookybear Posted at: 2019-03-31T19:46:47.026Z Reads: 107

```
Ha. How much? It's good to have a backup.
```

---
## \#777 Posted by: Touch415 Posted at: 2019-03-31T19:51:37.405Z Reads: 102

```
Give me $150 and it’s yours, @sofu upgrade the the whole usb feather and now it works  and charges good👍🏼
```

---
## \#778 Posted by: pookybear Posted at: 2019-03-31T20:04:55.058Z Reads: 107

```
[quote="Touch415, post:775, topic:74084"]
Buy mines :laughing::+1:t3: Half the price
[/quote]

Ha. You said half price. :rofl: :money_mouth_face:
```

---
## \#779 Posted by: Touch415 Posted at: 2019-03-31T20:05:55.461Z Reads: 108

```
 I feel you get annoyed wen people have issues sent you couple pm and never heard from you🤷🏻‍♂️ So I gave up 😔
```

---
## \#780 Posted by: Sn4pz Posted at: 2019-03-31T20:12:19.744Z Reads: 108

```
Hearing about the disconnects is really disheartening 😭 

I really don't want to have to hardwire a controller just to make it safe 😭😂
```

---
## \#781 Posted by: pookybear Posted at: 2019-03-31T20:14:26.284Z Reads: 103

```
You're funny. For an active knowledgeable DIY user, this is pretty ironic. Haha. Just being silly man.
```

---
## \#782 Posted by: Sn4pz Posted at: 2019-03-31T20:18:45.508Z Reads: 105

```
I just want a safe remote 😭
```

---
## \#783 Posted by: Touch415 Posted at: 2019-03-31T20:31:32.155Z Reads: 106

```
Hey it might work for you 👍🏼  But we had 2 feather remote in San Francisco with same issues so it wasn’t just me 😔  wish it worked out because i really like  everything about the remote just need some more testing and tweaking around to be reliable..
```

---
## \#784 Posted by: Touch415 Posted at: 2019-03-31T20:37:17.096Z Reads: 105

```
No doubt anything DIY is sketch 😆😆 just have to be ready for it 😬😬  that’s why it’s good to be honest and post stuff like this to warn other people 👌🏼 And also @StefanMe can perfect it 👊🏼 So it could be a killer remote..
```

---
## \#785 Posted by: pookybear Posted at: 2019-03-31T20:43:17.196Z Reads: 106

```
Exactly my thoughts
```

---
## \#786 Posted by: bevilacqua Posted at: 2019-03-31T20:53:14.220Z Reads: 104

```
I don't have any problems with my remote (well, only user error, but that's normal). Like with everything it's an ongoing R&D project. Testing them WW is a big part of this process, the more user input the better. 

Hey if you only want a remote buy a Gt2b and that's it, right? But if you want something else (way more interesting, at least for me) then stick to the feather and try to sort out your problems with Stefan and the community. He actually puts a LOT of time in the development. Like I already mentioned before: its a one-man job, not a big company. 

Each SW/HW iteration will be better, just stay calm and watch it improve.
```

---
## \#787 Posted by: pookybear Posted at: 2019-03-31T20:55:53.319Z Reads: 101

```
I understand. I don't doubt you at all. Just be patient w Stefan. He'll get that sorted out. :wink:
```

---
## \#788 Posted by: Surfer Posted at: 2019-03-31T22:13:16.343Z Reads: 103

```
Hi @Stefanme
Good news! I just saw the new vesc tool release. 1.08
We can use vesc tool as SWD programmer :slight_smile:
And then flash nrf51 to use it as a remote and data logger.
And the last, here is my question it's possible to swap the feather m0 to feather LE on your remote to make it compatible? I hope it's not too difficult to port the code from m0 to nrf51 and you have interest 😇
```

---
## \#789 Posted by: Arek Posted at: 2019-04-01T06:57:11.691Z Reads: 99

```
If it's a thing maybe just put a micro SD card in the remote xD
```

---
## \#790 Posted by: Friskies Posted at: 2019-04-01T15:17:44.813Z Reads: 97

```
Or Bluetooth? ;P
```

---
## \#791 Posted by: Arek Posted at: 2019-04-01T16:21:26.617Z Reads: 100

```
That would kill the run time, don't forget there's just a tiny battery...
```

---
## \#792 Posted by: Sn4pz Posted at: 2019-04-01T16:22:42.851Z Reads: 106

```
-Please understand I know nothing about remotes and their inner workings-

As I understand, the antenna is the most easily replaced part of the remote if someone wanted to improve connectivity. Are there any 'expensive' (please no 5 million dollar woowoo, Im talking about the 30 - 50 dollar range) antennas that would really step up the feathers game in terms of consistency? I havnt got mine yet, to be be fair, but my local area is a dropout nightmare

Any seller, Ali, Bang, Ama is fine with me, Ive got awhile to wait :+1:
```

---
## \#793 Posted by: StefanMe Posted at: 2019-04-01T16:45:57.768Z Reads: 103

```
I think I don’t need it. I got awesome results in the new design. I ll assemble a US version soon and send it out for testing. Then we ll see how good it is.
```

---
## \#794 Posted by: Sn4pz Posted at: 2019-04-01T16:47:09.688Z Reads: 102

```
Wait theres a new version just after I buy a remote? xd


Could you answer my question please, I dont want to buy a new board or remote. I just want to know what I need to look for in an antenna
```

---
## \#795 Posted by: StefanMe Posted at: 2019-04-01T16:52:37.284Z Reads: 108

```
Not now... but the new version is a lot cheaper and i ll just take the hardware cost if u want to replace it. 

BUT your remote should work perfectly. What problems exactly u have? 😂
```

---
## \#796 Posted by: Sn4pz Posted at: 2019-04-01T16:56:35.333Z Reads: 107

```
[quote="StefanMe, post:795, topic:74084"]
but the new version is a lot cheaper
[/quote]


Interested... damnit x) 

[quote="StefanMe, post:795, topic:74084"]
i ll just take the hardware cost if u want to replace it.
[/quote]

This would be amazing if there are any issues :+1: Ill let you know
```

---
## \#797 Posted by: bevilacqua Posted at: 2019-04-02T15:38:42.881Z Reads: 106

```
Sorry if this question is irrelevant but is your antenna near big phasewires or caps? Did you try istalling a LC Filter? The latter solved my issues
```

---
## \#798 Posted by: Arek Posted at: 2019-04-02T18:23:36.848Z Reads: 110

```
[quote="Sn4pz, post:794, topic:74084"]
Wait theres a new version just after I buy a remote? xd
[/quote]
Small teasers:

Transmitter/remote:
![tra|690x98](upload://tchtzBRLdG90dJhE9qdPa47nfhL.jpeg) 
Stage: designed, PCB made, tesing, ??

Receiver:
![pic|690x318](upload://othoJLeitoOn71p7sCAM9BAdUaU.png) 
Stage: designing

Both don't need expensive Adafruit development module anymore and are cheaper + other extras like built in antenna and low pass filter on the receiver.

Receiver is not "official" and nothing is guaranteed.
```

---
## \#799 Posted by: sofu Posted at: 2019-04-02T20:15:15.831Z Reads: 111

```
afaik no, and neither are mine. I think San Francisco is just a very wirelessly dense city and that results in a lot of interference. I dunno how much being on EU vs US frequency influences things either. 

I think it's likely about packet corruption. Something corrupts the packets transmitted and the receiver reads garbage data. We can very reliably reproduce the cutouts in certain areas and near cell towers which operate around 850MHz or so give or take 50. I was literally unable to move or even push my board on last saturday's ride for a while because every 3 seconds or so the feather could lock brakes because of disconnection. I couldn't even keep it connected long enough to turn off ebrakes. I was around a cell tower at the time, but I was with everybody else (non feather) and nobody else was having issues. They were all using either Boosted remotes (bluetooth) or nano v2 (2.4G?) or those chinaboard remotes (also 2.4GHz).

I think it may be time to switch radio technologies or implement forward error correction for packets received... maybe a hash with each packet received that can be used to reconstruct and crosscheck the packet which can then be used to rebuild the next packet? I'm definitely not a data transmission expert but I was talking with the CEO of Rainway about their forward error correction algorithms. They're able to rebuild each streamed frame basically perfectly at around 40% packet loss and they run their streams over much more noisy and lossy lines than we do. I think that would really improve the experience here...

Not that anybody asked but just my two cents :P
```

---
## \#800 Posted by: Arek Posted at: 2019-04-02T20:30:35.456Z Reads: 110

```
Not an expert either but I believe there has to be some tricks that could be done in the code that would make the communication much less vulnerable to the interference.
But it's something on a much higher level and we would need some help from outside.
Perhaps we could try with some Adafruit forum, because they're the author of the core of this project and they are from NYC as well.
```

---
## \#801 Posted by: StefanMe Posted at: 2019-04-02T21:20:04.964Z Reads: 109

```
Do u have the issues with with a another feather remote next to u?

If u switch off the remote, the brakes will release after 10-15 seconds if u need to push next time. (I implented this in case the remote battery is empty)

I ll go for a good NRF24L01 PA LNA in the next test. I ll send u a set for testing as soon as I got the prototype.
```

---
## \#802 Posted by: sofu Posted at: 2019-04-02T21:40:43.140Z Reads: 112

```
I have these issues no matter what I'm doing or what's next to me. I can reliably lose connection riding by myself in the following areas:
- San Francisco: Chinatown
- San Francisco: SoMa around 4th & Howard
- San Francisco: Downtown around 4th & Market
- San Francisco: Mid Market around Market & Van Ness
- San Francisco: Twin Peaks
- San Francisco: Central Richmond around Balboa & 25th-ish

You're right, I could have switched off the remote, but I was on top of a mountain and would like to have my brakes on the way down :stuck_out_tongue: It's sort of a dangerous situation either way I think... I would rather go down slowly and stop every so often than have to footbrake all the way down...

Please let me know when you get the prototype... I really really want to love this remote :sweat_smile:
```

---
## \#803 Posted by: Chupacabra Posted at: 2019-04-02T22:01:14.530Z Reads: 114

```
the ppm connection on the unity is on another port, not the COMM port. Will I have to just make a 1 pin connection to the SERVO ppm on the unity?

![image|281x500](upload://xLBfcmyMBiQyJ4D6XS6AqKjmasn.jpeg) ![image|375x500](upload://99aRWFUMwaiR0l79echmvN36XUs.jpeg)
```

---
## \#804 Posted by: StefanMe Posted at: 2019-04-02T22:03:32.135Z Reads: 115

```
Yes. Just the single wire go to PPM.

Should be white in your case.
```

---
## \#805 Posted by: Chupacabra Posted at: 2019-04-02T22:08:14.565Z Reads: 117

```
Awesome Thanks! Will test with the unity and get back soon. 

One thing I wanted to point out that whenever the remote comes back from standby mode the screen rotates and I can only see half of it. Turning the remote off and back on fixes the problem. But if it goes into standby the issue comes back.

![image|375x500](upload://wZZTOrjyQ5iznuMgC0zOPKFvIuq.jpeg)
```

---
## \#806 Posted by: pookybear Posted at: 2019-04-02T22:10:32.165Z Reads: 110

```
Mine does the same thing also.
```

---
## \#807 Posted by: Surfer Posted at: 2019-04-02T22:18:36.789Z Reads: 111

```
Mine does it
```

---
## \#808 Posted by: Arek Posted at: 2019-04-02T22:22:22.145Z Reads: 113

```
Here's my cable, 6 pin JST-PH on receiver to 7 pin JST-PH and 3 pin JST-XH on Focbox UNITY, crimped using Engineer PA-09:
![IMG_20190402_231714|690x388](upload://o3JiuFemXTzr5VUb9GOLb0QZqBV.jpeg)
```

---
## \#809 Posted by: Sn4pz Posted at: 2019-04-02T23:42:41.062Z Reads: 114

```
You'll likely get the second version board before I do, as my build is going to be ready around summer time. Please share your findings :D 

On paper the feather is everything I could want, just the idea that just maybe it could go rouge... :sob:
```

---
## \#810 Posted by: Chupacabra Posted at: 2019-04-03T05:58:48.110Z Reads: 118

```
![image|690x419](upload://vGOosdMXmNGP476Ap96v9hlposV.jpeg) 

Thank you so much friend. Your pic has been immensely helpful. The $500 is just my buddy trolling me.
```

---
## \#811 Posted by: Blubbking Posted at: 2019-04-03T08:22:16.252Z Reads: 114

```
Where can i order the new remote ?
```

---
## \#812 Posted by: DEEIF Posted at: 2019-04-07T05:48:09.897Z Reads: 109

```
Where can I get a fully assembled remote?
```

---
## \#813 Posted by: bluegreen Posted at: 2019-04-08T06:47:23.062Z Reads: 105

```
[quote="sofu, post:802, topic:74084"]
I can reliably lose connection riding by myself in the following areas
[/quote]

Wow, I read your post and realized those are the places my remote goes out too!
```

---
## \#814 Posted by: StefanMe Posted at: 2019-04-08T07:17:56.644Z Reads: 108

```
Also a FeatherRemote? Really strange. It looks like in the US are much more interferences on 915Mhz then in the EU with 433Mhz.
```

---
## \#815 Posted by: bluegreen Posted at: 2019-04-08T07:24:07.943Z Reads: 111

```
No sorry it's a 2.4ghz remote but I was just remarking on the areas of interference. In parts of SF I'm curious if it is related to the overhead power cables for the bus. Is there a thread for using higher DB antennas? It seems like most people are using pcb antennas or whip antennas. I'm looking at upgrading to antennas that are higher db than what FCC would otherwise allow.
```

---
## \#816 Posted by: Winkelmann Posted at: 2019-04-08T17:03:23.514Z Reads: 116

```
Hey guys!

So I'm planning a project atm and are sitting and comparing controllers
I've been looking at this one and also these ([nano remote](https://www.electric-skateboard.builders/t/firefly-nano-remote/72916/39), [simple remote](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/83))

and I've seen that there are a few things that really matter!

I love the bigger screen on this remote but I'm a bit scared of the 433 Mhz connection instead of 2,4

I'm trying to build a good quality but not the most expensive board


Is there anyone that knows the answers to these questions:
Is there any specific VESC I should aim for that would work better? I've been looking at this one ([VESC](https://www.mboards.co/collections/escs/products/bldc-esc-4-12))

how long does the battery last in a controller like this one?

Should you rather go with 2,4Ghz!?

Could you modify the components a bit in the controller made by solidgeek and then install this software if you buy a bigger screen?

ill update with a link when I've created the thread for my project!
```

---
## \#817 Posted by: StefanMe Posted at: 2019-04-08T17:13:18.682Z Reads: 118

```
Hi @Winkelmann ! 

I guess there are much less problems in Europe because fo the harder restrictions to frequency ect. The most European peoples doesn't have issues with that. In the US its way harder... maybe the 2.4 Is the choice here... not sure. I am working on a side project to get a 2.4Mhz version working with the Feather Remote. But we can only say more if we give it a good test in the US. Specially the area around @sofu is a hard place.

As soon as I have the first prototype running, I ll let you know. Maybe we should start a community project and not starting developing every person for its own. I am ll to share all my shematics I got now if someone is intersted.

This time I go for an SPI display, because u have less issues with broken communications... on the back is a NRF24L01+ PA LNA transmitter mounted. 

![FeatherRemote2_0back|690x460](upload://wBHAoYmg2YNpKdeCzzlbbZx8VV3.png) ![FeatherRemote2_0front|690x460](upload://nGIETxWeE08WSx9qimXazpuiYSo.png)
```

---
## \#818 Posted by: sofu Posted at: 2019-04-08T17:38:22.307Z Reads: 113

```
Do you lose connection with the nano v2? That's the most reliable one to beat right now I think. That and the Hoyt puck has been 100% solid in SF...
```

---
## \#819 Posted by: Winkelmann Posted at: 2019-04-08T17:58:01.532Z Reads: 114

```
Hey people!

im looking for feedback!

https://www.electric-skateboard.builders/t/project-board-better-than-boosted/89825?u=winkelmann
```

---
## \#820 Posted by: bluegreen Posted at: 2019-04-08T17:58:39.554Z Reads: 117

```
[quote="StefanMe, post:817, topic:74084"]
Maybe we should start a community project and not starting developing every person for its own. I am ll to share all my shematics I got now if someone is intersted.
[/quote]

I'd be interested. I also do electronics manufacturing for a living so maybe I can help if you wanted to get some of these made after the design is ready.

I guess I'm coming into this very late but I'm curious why to use a hall sensor instead of a potentiometer for the throttle?
```

---
## \#821 Posted by: deltazeta Posted at: 2019-04-08T17:59:48.405Z Reads: 116

```
I used this antenna to great success

https://www.aliexpress.com/item/868MHz-915MHz-GSM-IPX-IPEX-1-13-UF-L-Antenna-Built-in-2DBi-8cm-2DBi-IPEX/32862215507.html?spm=a2g0s.9042311.0.0.46ee4c4dfFqHkA

https://www.electric-skateboard.builders/t/firefly-nano-remote/72916/351?u=deltazeta
```

---
## \#822 Posted by: bluegreen Posted at: 2019-04-08T18:11:39.774Z Reads: 112

```
When the antennas come in I'll make another post with results after testing but this is where things get interesting to me. Most pcb or whip antennas are around 2 to 3DBi.

But I've found this one at 5DBi, it's probably too big to be in a transmitter but I'm gonna put it on the receiver:

https://www.digikey.com/product-detail/en/taoglas-limited/FXP70.07.0053A/931-1074-ND/2332701

For the transmitter, I'm going with one of these:

https://www.adafruit.com/product/2308

EDIT: Has anyone experimented with running a receiver that runs on both 433mhz and 2.4ghz at the same time for redundancy?
```

---
## \#823 Posted by: Winkelmann Posted at: 2019-04-08T18:15:05.279Z Reads: 112

```
Hey, thanks for such a fast response! yes that might be a good idea, at the moment im not that up to speed with everything since this project is going to be my first board, but i really appreciate all the feedback!

I'll have to look into it a bit more so I know all the pros and cons,

for example one of my friends expressed his love for the [esp8266](https://www.banggood.com/search/esp8266.html) since it can apparently do everything, haha, but I think the battery consumption would be a problem with that

again, i need to read into everything so i know a bit more what im talking about haha
```

---
## \#824 Posted by: sofu Posted at: 2019-04-08T18:18:55.671Z Reads: 109

```
FWIW when I was testing your board and coming back to you while braking it dropped then reconnected very quickly which is why I ran off the board... though if you didn't have any issues further down on the same road it is certainly handling better than the feather...
```

---
## \#825 Posted by: PickSix24 Posted at: 2019-04-08T18:22:21.299Z Reads: 104

```
@StefanMe I wonder if the issues are isolated to areas like SF, where the radio saturation is very heavy. I’m across the bay and haven’t had any issues. Has anyone else in other areas reported any disconnects ?
```

---
## \#826 Posted by: PickSix24 Posted at: 2019-04-08T18:23:46.454Z Reads: 102

```
@sofu did you ever try this antenna? 
 
https://www.team-blacksheep.com/products/prod:xfrace_ant_915

Maybe I’ll try one out and come on a group ride
```

---
## \#827 Posted by: deltazeta Posted at: 2019-04-08T18:24:23.447Z Reads: 109

```
Yeah i did a quick test myself before we headed down and I had 0 issues in the same area. I'm heavily suspecting you experienced the battery issues that later nearly threw me into a cross walk full of people...
```

---
## \#828 Posted by: sofu Posted at: 2019-04-08T18:29:58.294Z Reads: 105

```
No, but I did go super heavy duty https://www.amazon.com/gp/product/B079YL6SG2/

@deltazeta ooh yeah true... I'm just glad that didn't blow up... you have the worst luck with batteries 😬
```

---
## \#829 Posted by: PickSix24 Posted at: 2019-04-08T18:32:40.940Z Reads: 101

```
Oh wow ! That’s the antenna I used to use when flying FPV drones miles away. Granted I’ve never flown in downtown SF but 915mhz shouldn’t have range problems so close. Wondering if this is just a packet loss issue as stated earlier.
```

---
## \#830 Posted by: bluegreen Posted at: 2019-04-08T18:37:26.590Z Reads: 110

```
One thing to consider those style antennas are heavily polarized so how they are positioned could have an effect. Although, the range on them is huge so if you are just standing on it would be surprised.

The more I think about it, a multi-band receiver would be the coolest, you could do 433, 900 and 2.4 all at the same time. You could prioritize throttle to be on 900 and then put the battery info and other packets on 2.4 but also add throttle data to those packets as well.
```

---
## \#831 Posted by: sofu Posted at: 2019-04-08T18:54:29.537Z Reads: 110

```
I think it is definitely not a signal strength issue, but a packet corruption issue. Hoyt does channel hopping on 2.4GHz. which is a really great idea to reduce packet corruption, plus their packets are way smaller.
```

---
## \#832 Posted by: Touch415 Posted at: 2019-04-08T19:04:38.143Z Reads: 105

```
Selling my feather remote if anyone wants it for $130 ... lmk..
```

---
## \#833 Posted by: StefanMe Posted at: 2019-04-08T19:23:49.446Z Reads: 106

```
@sofu

What MHZ are u using? 

If it’s ecactly 915mhz, we could try a other frequency close to it. 912 for example. Maybe 915mhz is extremely crowded. Maybe this is the big deal here... 

I ll write a short update to change the frequency over the settings tomorrow.
```

---
## \#834 Posted by: sofu Posted at: 2019-04-08T20:21:28.289Z Reads: 101

```
I'm using the USA setting. I'm wondering if maybe I should swap to the EU setting and try that. What cop will be bored enough to try to catch me riding an eskate with a remote running at 8xxmhz...
```

---
## \#835 Posted by: StefanMe Posted at: 2019-04-08T20:23:53.996Z Reads: 100

```
we run on 433Mhz... Your receiver is not able to run this frequency solid. But it should help to just go a very little off from 915Mhz. I ll prepare something and we give it a try.
```

---
## \#836 Posted by: sofu Posted at: 2019-04-08T20:25:10.352Z Reads: 104

```
Ah my bad I keep thinking you guys are 800, yeah I'll wait for you :stuck_out_tongue:
```

---
## \#837 Posted by: deltazeta Posted at: 2019-04-08T20:31:28.990Z Reads: 105

```
If it's any help, the Firefly nano seems to run at 920mhz by default
```

---
## \#838 Posted by: StefanMe Posted at: 2019-04-08T21:52:58.807Z Reads: 116

```
Ahhhh this could be the clue! Going a little out of all the other frequencies. 

@sofu 
I made the frequency now adjustable inside the menu. Just pair the remote and then u can change all the time the frequency from the settings menu. +- 10Mhz. Give it a try with 920Mhz maybe... I don't know. But  maybe the antenna must be shorter or longer for this. But for the test it should work as it is.

I think u just have to update the remote...!

https://github.com/StefanMeGit/FeatherM0-Esk8-Remote

PS: Also the screen is now in the correct orientation after sleep mode... :slight_smile:
```

---
## \#839 Posted by: sofu Posted at: 2019-04-08T22:08:52.205Z Reads: 110

```
OK, I'll go home and try it, maybe do a quick run up twin peaks :stuck_out_tongue:

Jk it is raining 😤
```

---
## \#840 Posted by: lazarus Posted at: 2019-04-08T22:09:25.488Z Reads: 111

```
Does your remote have a radio-only mode, which logs dropped packets and control gaps while you ride using a different (known good) remote? This can be useful both for safer testing, but also since a human rider won't always notice radio interference.
```

---
## \#841 Posted by: Sn4pz Posted at: 2019-04-08T23:04:46.402Z Reads: 110

```
Exactly... Lol I doubt anyone would get flack for it

What is the range of frequencies that we can use for this type of thing?
```

---
## \#842 Posted by: pookybear Posted at: 2019-04-09T07:44:34.747Z Reads: 108

```
Im getting this error updating my receiver:

receiver:48:24: error: VescUart.h: No such file or directory

   #include <VescUart.h>

                        ^

compilation terminated.

exit status 1
VescUart.h: No such file or directory

I was able to update it before this new version.

Edit:
Am I supposed to use rolling gecko or solid greek"s library?
```

---
## \#843 Posted by: StefanMe Posted at: 2019-04-09T07:49:47.532Z Reads: 109

```
Are u running on VESC or UNITY? Have u done the SETUP on top of the Library?

Please check the manual... ! U have to use my VescUart-Library :slight_smile:
```

---
## \#844 Posted by: pookybear Posted at: 2019-04-09T07:50:44.979Z Reads: 109

```
I switched to vesc6 now. So. im upgrading my receiver. I have already updated my remote.

I just need to know which library to use. There are two. Solidgeeks and rolling gecko. 

Apparently, I cant read. Ill look for your library. Got a link by any chance?
```

---
## \#845 Posted by: StefanMe Posted at: 2019-04-09T07:52:22.191Z Reads: 114

```
> Please check the manual… ! U have to use my VescUart-Library :slight_smile:

@pookybear  have to use my library!! 

https://github.com/StefanMeGit/VescUart
```

---
## \#846 Posted by: pookybear Posted at: 2019-04-09T07:52:51.955Z Reads: 106

```
You're ninja edit is quicker than mine. Thanks!!!!
```

---
## \#847 Posted by: pookybear Posted at: 2019-04-09T07:56:00.011Z Reads: 103

```
Updated successfully. Thanks again!
```

---
## \#848 Posted by: StefanMe Posted at: 2019-04-09T08:00:52.118Z Reads: 113

```
I am working on the code...

I have implemented a new option to change the transmitter settings:

There are two value who can highly increase the stability of the remote...
 
` void setRetries(uint8_t retries);`

` void setTimeout(uint16_t timeout);`

U can choose in the settings menu between 5 different modes... maybe one is much better for the critical areas. 

I can recomment 1-5, 6 is more for testing.

The display will maybe also frezze for a few seconds, because i gave the transmission more priority. But the display works normal when u are in the settings menu or lost the connection tottaly.

1. 0/20 (retries/timeout) <- standart
1. 0/40
1. 2/20
1. 5/20
1. 5/40

I ll upload the code later, because i am not at home and i cannot test it.
```

---
## \#849 Posted by: StefanMe Posted at: 2019-04-09T08:14:41.434Z Reads: 112

```
@pookybear if u want to test the new tranmission mode... i created a new branch


https://github.com/StefanMeGit/FeatherM0-Esk8-Remote/tree/testing?files=1
```

---
## \#850 Posted by: pookybear Posted at: 2019-04-09T16:50:40.802Z Reads: 110

```
So....... I'm trying to setup my remote on my vesc6 and its not seeing it. Yes, remote and receiver are paired.

I have done the following to make it work:
* switch remote and controller to a working firmware
* switched rx/tx (I believe this only matters for telemetry. just trying to set my controller endpoints for now). I tried it both ways. Same results.
* tried it on my other vesc6 to rule out my other one. Same thing
* running ackmaniac 1.03 firmware on both vesc6
* did continuity check on jht cables. they all passed

Any special steps I need to do to get this to work?

TIA
```

---
## \#851 Posted by: StefanMe Posted at: 2019-04-09T17:48:20.958Z Reads: 106

```
I am not sure that everything works fine with the ackmaniack software... I can check this later.

the TX must go to RX and the RX to TX. Please make sure the wires are in this order.

Switch off the remote and board, power on the board at first and then switch on the remote. Have u activated UART and set the baud rate on the connected VESC to 115200?
```

---
## \#852 Posted by: pookybear Posted at: 2019-04-09T18:11:48.865Z Reads: 106

```
Yep. Wirings are correct. I switched them since I'm coming from 4.x hw to 6.x hw.

* TX to RX
* RX to TX

I'll try again tho.

My mini remote works. So it has to be my remote. I'll recheck everything again.

Thanks.
```

---
## \#853 Posted by: StefanMe Posted at: 2019-04-09T18:14:34.095Z Reads: 106

```
A wait... u mean not even the PPM works? What are u talking about?

Have u connected the PPM cable ect? What exactly is not working?

To get the remote working u just have to connect PLUS MINUS and the PPM. The other cables for TX RX is just an extra to get live telemetry.
```

---
## \#854 Posted by: pookybear Posted at: 2019-04-09T18:26:44.011Z Reads: 105

```
[quote="StefanMe, post:853, topic:74084"]
A wait… u mean not even the PPM works? What are u talking about?
[/quote]

No ppm signal is being detected by Vesc using wizard.

[quote="StefanMe, post:853, topic:74084"]
Have u connected the PPM cable ect? What exactly is not working?
[/quote]

Yes, PPM is connected.

[quote="StefanMe, post:853, topic:74084"]
To get the remote working u just have to connect PLUS MINUS and the PPM. The other cables for TX RX is just an extra to get live telemetry.
[/quote]

Remote has power. TX and RX and connected correctly. It's just the PPM signal I'm not getting.
```

---
## \#855 Posted by: StefanMe Posted at: 2019-04-09T18:35:48.024Z Reads: 95

```
Please check the PPM connector... I didn't change anything on the receiver side. 

I ll upload the code to my receiver as well to make sure there is no other issue, but i think everything works fine. Can u connect the receiver to the PC and comment the DEBUG and DEBUG_TRANSMISSION out? Then we can see what the receiver is receiving.
```

---
## \#856 Posted by: pookybear Posted at: 2019-04-09T18:42:58.376Z Reads: 97

```
Sure thing. 

I'm trying the official Vesc firmware. After this, I'll try your suggestion.
```

---
## \#857 Posted by: StefanMe Posted at: 2019-04-09T18:47:09.143Z Reads: 98

```
The PPM must work with all firmware... there is no change. Look into the DEBUG. If u need help let me know and we can try a short teamviewer session
```

---
## \#858 Posted by: pookybear Posted at: 2019-04-09T18:53:59.220Z Reads: 103

```
Official Vesc 1.08 does not detect PPM signal either.

Let me load ackmaniac back then Ill shoot you a PM.
```

---
## \#859 Posted by: Surfer Posted at: 2019-04-09T19:16:15.390Z Reads: 96

```
Did you press the RT button? 😁😁😁😁
```

---
## \#860 Posted by: TSJ Posted at: 2019-04-09T19:53:47.508Z Reads: 101

```
@stefanme I printed the V2 parts and noticed that the knob with the nub feature has square magnet holes.  Is that intentional?
```

---
## \#861 Posted by: StefanMe Posted at: 2019-04-09T19:54:38.766Z Reads: 101

```
Yes. There fits square and round magnets in
```

---
## \#862 Posted by: pookybear Posted at: 2019-04-09T20:28:17.444Z Reads: 104

```
It was my cable orientation that was messed up. Somehow when I was switching my vesc out. I didnt make a mental note on how I had it plugged in. I had PPM cable connected from VCC to PPM on Vesc. Yes, I had the one end of the cable connected to UART and the other end connected to PPM port. Yes, I was stupid :see_no_evil::man_facepalming:t4::joy: It should have been receiver PPM to vesc PPM. 

Everything works.

Huge thank you to Stefan for remote support. He looked at the debugging and everything was fine. Woohoo.
```

---
## \#863 Posted by: sofu Posted at: 2019-04-10T00:52:27.138Z Reads: 99

```
@StefanMe which branch do you want me to test? testing or development_..._rfm69?
```

---
## \#864 Posted by: sofu Posted at: 2019-04-10T02:50:21.543Z Reads: 98

```
Ok so I tested the latest "test" branch, went up twin peaks and the remote is basically unusable once you start up twin peaks Blvd. I have a video which I will edit and post when I come back. It's very bad I'm sad to say... Almost didn't make it up. It disconnected like 6 times within 500ft and I tested all transmission modes and changed frequencies a lot.
```

---
## \#865 Posted by: Surfer Posted at: 2019-04-10T05:53:07.541Z Reads: 97

```
Same here, flashed test branch, tested the 3 of different types of transmission and d still a lot of micro drops.
 I thought when I start the riding it was a success because was no drops for 4-5 minutes but then drops start to happen and more and more often until was almost unrideable go to home.
```

---
## \#866 Posted by: StefanMe Posted at: 2019-04-10T06:03:30.297Z Reads: 98

```
Ok  have u tried to change the frequency to 920mhz? Or the other direction 910mhz.

Also u can try to change to a different transmission mode... please check the settings Menü for that.
```

---
## \#867 Posted by: StefanMe Posted at: 2019-04-10T06:04:26.545Z Reads: 96

```
So was is more Bad than before or the same as before?
```

---
## \#868 Posted by: sofu Posted at: 2019-04-10T06:41:24.288Z Reads: 99

```
Yeah I did, I said above I tried even the min and max frequencies as well as all transmission modes. I even recorded just sitting there and watching the remote disconnect and reconnect every few seconds. I’ll get the video up later...
```

---
## \#869 Posted by: Surfer Posted at: 2019-04-10T07:09:25.487Z Reads: 101

```
I think the same behaviour, just I switched on/off in the way back home and it didn't happend the drops again until I was riding for couple minutes and then again lots of drops.
 I'm my case I'm quite sure is not interference related idk, I'm close to take it apart completely and resolder it again.
The thingy is I love this remote!
We will make it work as it should be!😃
Thanks for your support Stefan
```

---
## \#870 Posted by: StefanMe Posted at: 2019-04-10T08:07:24.653Z Reads: 108

```
This sounds like a real interference issue... the must be some really hard transmitters around there. I run the same firmware and dont have any connection issues with the remote. Looking forward to the video! Have u updated the receiver as well? Or just the remote? I made just a very little change here... 

 @surfer take a closer look onto the display... specialy connecter ect. U can also try to disconnect the OLED and start the remote without display by this combination on startup. 

hold trigger
hold menu button 
throttle backwards
```

---
## \#871 Posted by: StefanMe Posted at: 2019-04-10T08:32:54.080Z Reads: 114

```
@lazarus has commited some code for debuging. I ll check this the next days, maybe it help to find out whats the problem. 

Basicly u run the board with another remote on PPM while the feahterRemote is still connected.
```

---
## \#872 Posted by: sofu Posted at: 2019-04-10T18:10:22.739Z Reads: 116

```
Yeah, I updated both

I think I have to switch back to my old remote while I wait for your nrf24 prototype...
```

---
## \#874 Posted by: sofu Posted at: 2019-04-11T08:30:11.772Z Reads: 113

```
Well I did my best

https://youtu.be/_i09nszto_g
```

---
## \#875 Posted by: StefanMe Posted at: 2019-04-11T08:36:59.067Z Reads: 118

```
thx, unfortunitly i cant se anthing... but its strange.

We should try something else... can u battery power the receiver instead of going for the 5V from the VESC? Maybe we have a problem from the power supply here. I ll implement a counter to see lost packasges when u ride... this could be helpfull to find out if its really a connection issue.
```

---
## \#876 Posted by: sofu Posted at: 2019-04-11T08:47:41.614Z Reads: 120

```
Yeah you can't see the display, but you can see the cell towers in the video

https://puu.sh/Dd5px/430c938c60.png

https://puu.sh/Dd5qS/4a68702e05.png

I really don't think it's the power supply. You can see at the end of the video I held it super close and it worked more or less. Plus away from the cell towers I climbed tons of hills without problems.

To be honest I was really scared I was going to crash when I did this test, which is why I was wearing kneepads. And I almost never wear kneepads so that should say something... With all due respect I really don't want to be a guinea pig anymore for this version of the remote and go through that scare again. You can hear my friends laughing in the video but I wasn't. I was pretty on edge. I honestly think it's the transmission frequency that's the problem so I won't test 8-9xxmhz remotes anymore. I'll just wait for you to send the 2.4ghz version before I test it again... if I don't get something else before then.
```

---
## \#877 Posted by: StefanMe Posted at: 2019-04-11T08:50:40.057Z Reads: 111

```
OK, I am very sorry for this. As i said before, i cant test certain places with this crazy interferences. USA is crazy in transmission powers. I ll inform u as soon as i have a 2.4 version.
```

---
## \#878 Posted by: sofu Posted at: 2019-04-11T08:53:33.287Z Reads: 113

```
Thank you Stefan, I really appreciate you trying to help us and I know how frustrating it is when something you work on so hard has crazy issues. I build and ship a super high profile product for a living so I totally understand :) I'll wait patiently for the 2.4ghz version!
```

---
## \#879 Posted by: Sn4pz Posted at: 2019-04-11T10:40:12.198Z Reads: 111

```
Please put me on this list too, the 2.4ghz version would likely do better in my area... Lots of cell towers 🙄😂
```

---
## \#880 Posted by: StefanMe Posted at: 2019-04-11T13:15:27.182Z Reads: 114

```
Guys... I am so sorry about the problems in the us. I ll make some new remotes with 2.4ghz soon and we ll exchange the remotes if we need. But it need some time.
```

---
## \#881 Posted by: Sn4pz Posted at: 2019-04-11T13:16:52.413Z Reads: 117

```
Cant wait to see what you create!

I assume its way too optimistic to hope for a summer release.... Maybe I'll get to wrap it as a Christmas gift for myself :joy: :+1:
```

---
## \#882 Posted by: PickSix24 Posted at: 2019-04-11T14:06:07.801Z Reads: 116

```
The cell tower issue is interesting. I live on the other side of the bay from @sofu and haven’t had any issues. I have a cell tower on my work property ( literally 100ft away from me right now ) I can ride within 15ft of it without issue. Too bad we can’t log while riding.
```

---
## \#883 Posted by: sofu Posted at: 2019-04-11T17:35:39.771Z Reads: 117

```
Typically there are fences around those with plaques on them that say what company operates them and what frequency they operate at. Try looking for that? Maybe it's not a similar frequency?
```

---
## \#884 Posted by: PickSix24 Posted at: 2019-04-11T19:15:37.833Z Reads: 114

```
I’ll take a look, pretty sure it’s a Verizon tower
```

---
## \#885 Posted by: sofu Posted at: 2019-04-11T19:18:56.119Z Reads: 116

```
Verizon runs at around 1700mhz for LTE. It wouldn't interfere with the remote :P
```

---
## \#886 Posted by: Sn4pz Posted at: 2019-04-11T19:24:45.881Z Reads: 113

```
Any idea of the towers near you?
```

---
## \#887 Posted by: sofu Posted at: 2019-04-11T19:34:25.573Z Reads: 119

```
There are two on Twin Peaks, one is a TV and radio tower which I think doesn't really affect a whole lot probably, the other is I *think* the cell tower. There is also an AT&T cell tower on top of a parking garage I used to sometimes skate in, and whenever I get near that garage I just can't use the remote at all anymore cause it's so bad. That tower runs at 850-900 and there's a sign that says if you cross the fence around it you may die 😬
```

---
## \#888 Posted by: Sn4pz Posted at: 2019-04-11T19:40:42.024Z Reads: 118

```
Ugh :sob: 

I live like 5 minutes (on foot) away from an atnt tower 😂😂 

Well I guess I'll see how it plays out
```

---
## \#889 Posted by: Arek Posted at: 2019-04-11T20:14:37.473Z Reads: 124

```
Stefan you have to go visit @sofu and bring with you some scope connected to the receiver's 5V and spectrum analyzer monitoring the ether then go for a ride in those places xD
```

---
## \#890 Posted by: StefanMe Posted at: 2019-04-11T20:16:19.411Z Reads: 127

```
I would love to visit SF...
```

---
## \#891 Posted by: sofu Posted at: 2019-04-11T20:18:44.295Z Reads: 126

```
Well @Deodand is supposed to visit me soon... we will work on the iOS Unity app and analyze the shit out of the spectrums here 🤣
```

---
## \#892 Posted by: Deodand Posted at: 2019-04-11T20:19:17.055Z Reads: 128

```
I'll bring my o-scope :)
```

---
## \#893 Posted by: Arek Posted at: 2019-04-11T20:20:06.959Z Reads: 130

```
Me too but would have to go back to Poland then to Warsaw to get visa and other crap then wait like entire weeks to get the response :sweat_smile:

I wonder should I even bother finishing off that receiver if there is soo much trouble with those RFM69 modules?

@sofu ask him to fix the bluetooth communication loss issue when using Oneplus 3T because I barely can even upload the settings :frowning:
```

---
## \#894 Posted by: sofu Posted at: 2019-04-11T20:22:09.062Z Reads: 124

```
Yep bluetooth firmware is a known issue... Believe me I'm not looking forward to dealing with that either and I'm not even developing for Android :P
```

---
## \#895 Posted by: Arek Posted at: 2019-04-11T20:25:58.022Z Reads: 124

```
That's why I asked you to just ask him so he can do it himself :upside_down_face:

But if it's a know issue then it's fine :stuck_out_tongue:
```

---
## \#896 Posted by: sofu Posted at: 2019-04-11T20:38:31.013Z Reads: 126

```
Yeah I hear ya 100%! Expect improvements there soon...
```

---
## \#897 Posted by: Arek Posted at: 2019-04-11T20:43:53.530Z Reads: 131

```
Awesome!

Now we just need to lure some wireless transmission programming mastermind so you US guys can enjoy the feather remote without the need to change the hardware :stuck_out_tongue:
```

---
## \#898 Posted by: lazarus Posted at: 2019-04-11T22:00:22.953Z Reads: 128

```
I think they run different bands in different areas, and all have LTE in 800s.
```

---
## \#899 Posted by: Sn4pz Posted at: 2019-04-11T22:03:34.864Z Reads: 129

```
Very excited to see what you find.... Your efforts are very much appreciated :smile:
```

---
## \#900 Posted by: sofu Posted at: 2019-04-11T22:13:08.891Z Reads: 132

```
Maybe so, that's probably true. I'm not an expert I just read the signs :P
```

---
## \#901 Posted by: Bardakon Posted at: 2019-04-12T01:37:31.719Z Reads: 134

```
Looks AWESOME!
whats the price?
@StefanMe
```

---
## \#902 Posted by: pookybear Posted at: 2019-04-12T22:28:21.277Z Reads: 135

```
So after two weeks or so waiting for the feather battery, I finally got it today. It was shipped from china. I was so excited to get this built for a friend. I opened it up and guess what. no connector. :man_facepalming: :sob:

Does anyone know what connector do I need to get? I kmow it's pretty tiny. I'm gonna have a blast crimping the damn thing :expressionless:
```

---
## \#903 Posted by: PickSix24 Posted at: 2019-04-12T22:51:35.130Z Reads: 134

```
Jst Ph 2.0 2 pin
```

---
## \#904 Posted by: pookybear Posted at: 2019-04-14T05:12:19.738Z Reads: 137

```
![15552187094511884188974|375x500](upload://xN60Ncwcp7CmtiM89Z0AxCvK1RB.jpeg) 

Getting there!
```

---
## \#905 Posted by: pookybear Posted at: 2019-04-15T05:40:54.293Z Reads: 138

```
@StefanMe 

Is there any way to adjust first initial throttle throw on this remote? It has too much initial dead throw. About 30% ish. I already have dead band set to 2 on remote and 2 on Vesc. It helps when I switched my pos ramp to 0.1. But the initial throw lag is still there.

Is it because of that green area down below? Not the top one for the dead band.
![IMG_20190414_154355|666x500](upload://mbBW6j3M400ImNYyO0icLzTi508.jpeg)
```

---
## \#906 Posted by: sofu Posted at: 2019-04-15T18:06:03.807Z Reads: 134

```
Make sure you calibrate your remote properly so the center in the remote settings is the actual center detected by the remote hall sensor. Then set your input deadband in vesc app settings to something lower. 15% is too much.
```

---
## \#907 Posted by: pookybear Posted at: 2019-04-15T18:35:47.108Z Reads: 140

```
I have. I always calibrate the remote first before I set the Vesc ppm. 

Dead band settings:
* Vesc 2
* Remote 2

I took that pic before I set the dead band to 2.

Edit:
I figured maybe someone knows another trick or two to get rid of the throttle lag more.
```

---
## \#908 Posted by: Lucifer Posted at: 2019-04-15T19:00:19.136Z Reads: 145

```
I had the same issue with the Firefly Nano. The first thing to try is try changing the position of the hall sensor and using better magnets.

I also wanted a longer wheel travel so I spread the magnets apart, and managed to get a better throttle curve by slightly tilting the magnet sideways. After some trial and errors I got a nice throttle response with something like this :

![wheel_|619x500](upload://2fCEQh5JzNAbZr375lOOTSQHzqc.jpeg)
```

---
## \#909 Posted by: pookybear Posted at: 2019-04-15T19:03:49.048Z Reads: 138

```
That's what I was thinking too! OMG. 

Any chance you could share the STL file?
```

---
## \#910 Posted by: pookybear Posted at: 2019-04-15T19:06:49.716Z Reads: 137

```
I'll probably keep the distance of the magnet the same for my preference. Throttle travel is good enough for me. It's the response I want changed.
```

---
## \#911 Posted by: Lucifer Posted at: 2019-04-15T19:08:52.579Z Reads: 140

```
Sure, but this one needs ball bearings and a different spring. Which for the story was fixed with a steel screw directly on the wheel between the 2 magnets, which made a weird hole in the throttle response but I got rid of the issue with a nylon screw :-) I can give you the 3D file if you want or export something else,  let me know what you prefer..
```

---
## \#912 Posted by: pookybear Posted at: 2019-04-15T19:09:55.652Z Reads: 137

```
Pm coming your way.
```

---
## \#913 Posted by: willumpie82 Posted at: 2019-04-16T08:37:23.199Z Reads: 144

```
did anyone look into other hall sensors e.g.

* digital output, less noise due to the AD conversion
* rotary sensor, less suspecable to other magnetic fields, construction has to change sinve the magnet has to be dead center of the knob
```

---
## \#914 Posted by: JulianS Posted at: 2019-04-24T08:05:00.727Z Reads: 139

```
Hey @StefanMe , how is that custom board coming along? :)

Im super interested into the fully integrated solution without going through the feather module. If you need any help I'm at TUM in Garching and UniBW in Neubiberg and have access to a reflow and a pcb mill, happy to help quickly prototype and test stuff! Also can order some parts if you need to test them. I have a solid sample account for TI as well if you need any parts there.
```

---
## \#915 Posted by: sofu Posted at: 2019-04-24T18:47:28.917Z Reads: 139

```
Well my feather receiver straight up died mid braking 🙃Haven't taken my board apart to see what the issue is but I expect whenever I do I'll just switch back to my custom firefly based remote...
```

---
## \#916 Posted by: PickSix24 Posted at: 2019-04-24T19:34:08.895Z Reads: 133

```
If you need a receiver let me know
```

---
## \#917 Posted by: sofu Posted at: 2019-04-24T21:14:46.678Z Reads: 135

```
Thanks, I'll just wait for whenever @StefanMe finishes the nrf24 version and in the meanwhile use my own stuff :)
```

---
## \#918 Posted by: Arek Posted at: 2019-05-12T13:32:49.614Z Reads: 126

```
Would be nice to see what happened to that receiver so we can learn from it and make future designs more robust.
```

---
## \#919 Posted by: kiryl Posted at: 2019-05-19T15:33:11.978Z Reads: 117

```
@StefanMe My remote has not been working for a month, can I please have it repaired or get a refund?
```

---
## \#920 Posted by: Chupacabra Posted at: 2019-05-19T15:43:53.892Z Reads: 116

```
@StefanMe just adding in here that I have had significant cutoff issues with my remote in the past. I had to take the antenna out of the remote case and that caused a major drop in the cutoffs frequency. 

However there are still dark spots where my remote just refuses to respond. I think what happens is that there is frequency connection drops and reconnect at these places.  And because there is estopp enabled, my board does not move at all and I have to push. 

The cutoffs happen near a railway track so I dunno if they have some special train communication towers or something.
```

---
## \#921 Posted by: Jansen Posted at: 2019-06-06T02:35:46.544Z Reads: 97

```
Hey @StefanMe I've sent you 2-3 PM's over the last month or so, are you getting them?

Has anyone heard from Stefan lately and / or does anyone know the status of getting the bugs fixed. I've still only got to use my remote for half of one run and was on the first batch so am hoping Stefan has that small new good batch so that I can send mine back and get a replacement now that my build is done and ready for it.....

LMK what's good @StefanMe  been super patient for months and would really like to get a working remote. Happy to even try the one I have currently if you think the new code might fix my issues..... lmk brotha. PLEASE.
```

---
## \#922 Posted by: tardyparty7 Posted at: 2019-06-06T02:37:01.101Z Reads: 91

```
what bugs? I've haven't used my v2 remote yet. are they in them?
```

---
## \#923 Posted by: dcxeternal Posted at: 2019-06-06T02:38:42.920Z Reads: 90

```
Last heard from him about 2 weeks ago.  Said they were about 80% ready for the 3rd batch but running into some issues with the circuit still.
```

---
## \#924 Posted by: tardyparty7 Posted at: 2019-06-06T02:40:11.290Z Reads: 90

```
i have a second batch so im confused
```

---
## \#925 Posted by: dcxeternal Posted at: 2019-06-06T02:53:23.343Z Reads: 92

```
I mean the 3rd batch then.  Its been quite awhile so I forgot
```

---
## \#926 Posted by: pookybear Posted at: 2019-06-06T04:23:33.620Z Reads: 92

```
What issues do you have? Mine has been working pretty good.

Last time I heard he was going to switch to 2.4ghz instead. He's probably reworking the whole remote. I could be wrong tho
```

---
## \#927 Posted by: dcxeternal Posted at: 2019-06-06T12:54:58.020Z Reads: 90

```
I believe this is the case.
```

---
## \#928 Posted by: gmurad Posted at: 2019-06-06T13:10:02.275Z Reads: 93

```
I believe the original firefly remote which this is inspired by was using nRF24 and 2.4GHz. If this is going back to 2.4GHz I wonder if he will use nRF24 or even nRF52?
```

---
## \#929 Posted by: Jansen Posted at: 2019-06-07T08:11:23.411Z Reads: 98

```
I can't remember now what @StefanMe said the issue with mine is but I think I recall it being something like a defective screen or PCB or something. Did a couple team viewer sessions to let him try to fix it but could never get it to work right. It will just freeze and have to be restarted all of the time and not work for longer than 10-30 seconds, the screen always goes blank or doesn't turn on at all a lot of times too, and something else is wrong as well that I'm not recalling since it's been a month or two now. I just wish I could get some type of response... stefan said to send it back once he's closer to being done with a new version so he can swap it out but he hasn't gotten back with me for around a month or so now. Which isn't usually like him and he was usually pretty good about helping until recently..... where you at @StefanMe !!!!!!!!!!!!!
```

---
## \#930 Posted by: pookybear Posted at: 2019-06-07T08:19:19.696Z Reads: 96

```
It's ok man. You're not alone. I'm actually waiting for my spare receiver.  I stopped asking because I know he's probably busy w school and/or new remote. He did tell me to wait for the updated version.
```

---
## \#931 Posted by: walleywalker Posted at: 2019-06-12T01:55:24.723Z Reads: 95

```
Just wanted to report my trouble with @StefanMe. I've finally reached my wit's end with him and want to caution others before doing business with him. 

In Nov of '18 I paid Stefan €175 for two DIY feather remote kits. I later realized that the kits did not come with any components, so prior to Stefan ever sending me anything we agreed and I paid him an additional €58 in Dec '18 for the components I'd need so I didn't have to scourer the internet for them. 

I received nothing for the next few months, and politely asked Stefan for updates every few weeks. After many repeated requests and two and a half months after sending him over $250 USD months prior, I received a small but well packaged box with zero tracking notification. 

I open the box to find a whole slue of missing items, of which I went back through, counted everything and published to Stefan with this chart. Stefan's myriad of excuses over the prior months, the best he could muster up this time was, paraphrasing "I packed everything in there, it must have been opened or fallen out". I would have believed him if it hadn't had a new excuse for me every week prior for it not being in the mail. 

Anyhow, he's now stopped replying to my messages after repeatedly telling me he'd fix the situation. I believe he has the right intention to do so, I really do. I just think he lacks the time and/or will power to follow-through. I say this cause he's never said one rude thing and was always responsive, though this has been entirely frustrating at the same time. 

Anyways, that's my warning. Don't get burned. If you want to purchase these "project parts" off me, myself incurring a big loss, I'd sell them to any interested party. 

Here's the image of what I received:
![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/0/6/063631907c5b518c608d02f5fb8ae25ea00f1c9b.jpeg)

Here is the list of what I had been promised, including all kinds of missing components from small to large (including an entire Feather basic PCB!) ![](https://www.electric-skateboard.builders/uploads/db1493/original/3X/9/d/9d8665f9faab27f398b0353b9d15b8c68f7a30e7.png)
```

---
## \#932 Posted by: tardyparty7 Posted at: 2019-06-12T02:05:58.176Z Reads: 92

```
[quote="walleywalker, post:931, topic:74084"]
I open the box to find a whole slue of missing items, of which I went back through, counted everything and published to Stefan with this chart. Stefan’s myriad of excuses over the prior months, the best he could muster up this time was, paraphrasing “I packed everything in there, it must have been opened or fallen out”. I would have believed him if it hadn’t had a new excuse for me every week prior for it not being in the mail.

Anyhow, he’s now stopped replying to my messages after repeatedly telling me he’d fix the situation. I believe he has the right intention to do so, I really do. I just think he lacks the will power to follow-through to his word. I say this cause he’s never said one rude thing and was always responsive.

Anyways, that’s my warning. Don’t get burned. If you want to purchase these “project parts” off me, myself incurring a big loss, I’d sell them to any interested party.
[/quote]

When I purchased my remote from him he was very on time and constantly giving updates. I highly encourage people to buy his products as they're high quality and he gave me many updates. @sofu @pookybear have you guys had any contact with him and how are your remotes going? 

Secondly, his profile is hidden, meaning he probably is not very active or he got banned to some extent. @StefanMe has been off the forum lately for reasons we do not know, or i don't know at least.

State the facts, and nothing else. We're all tempted to be mad, especially me, when you feel you've been duped, but state the facts. You don't think somethings could've been opened when shipping to you? I find that believable. Can I see the packaging it was sent in? Was it already opened, not completely shut?
```

---
## \#933 Posted by: pookybear Posted at: 2019-06-12T02:37:25.592Z Reads: 87

```
Nope. Last time I messaged him was about my spare receiver that I have yet to receive. Just asking for an update but no reply. I didn't follow up then as I have no need for it at the moment. Plus, I'm assuming he's working on a newer reliable remote.

I think @bevilacqua might be able to help. He's friends with him I believe.
```

---
## \#934 Posted by: walleywalker Posted at: 2019-06-12T03:07:00.157Z Reads: 85

```
I'm not mad, man. I plainly stated I'm frustrated. 

I'm not sure what you are accusing me of stating? I haven't stated that he's not banned or away, he hasn't replied, that's what's been said. 

I don't have the box anymore, it's been thrown away for months.
```

---
## \#935 Posted by: tardyparty7 Posted at: 2019-06-12T03:13:29.798Z Reads: 83

```
i never accused you of stating anything, i just stated he might be banned.
```

---
## \#936 Posted by: sofu Posted at: 2019-06-12T05:23:03.191Z Reads: 88

```
I haven't heard from him in a while. i switched to other stuff already my featherremote is just sitting there
```

---
## \#937 Posted by: bevilacqua Posted at: 2019-06-12T07:04:54.665Z Reads: 87

```
Stefan is indeed working on a newer remote, I am sure he wants the best for all users who have a feather remote (he still pushes updates, the last one only a couple of days ago), I guess he has decided to not become so active lately, I can understand his decision. 

Give the man some time, you have to understand that this is a development project, not an off the shelf product, entirely coordinated by only one guy. This fact is easily forgotten a lot of times in this forum...


-------------
**To sum up**, Stefan is still alive, working on the next remote gen. (will be a cool one ;) ) and quite busy as far as I know. He'll reach out to you all, in the meantime just use another remote :/
```

---
## \#938 Posted by: Jansen Posted at: 2019-06-12T19:18:36.473Z Reads: 87

```
Completely get all of this @bevilacqua and know guys like him and you helping the DIY scene out are bound to have delays and run into issues and I personally can;t express enough appreciation for what you two and the many others due with your talents so I really do try not to bug and sit as patiently as possible waiting for the updates cause I know you guys want to please backers/supporters you have as soon as you can too. 

All most of us need sometimes is just a little more or better communication at times and I can unknowingly assume that those gestures would/will ease the mob and prolly shut most of us up for another short while. 

And in all honesty, @StefanMe  from the beginning was SUPER good at that part of it and EXTREMELY helpful I know to me so when that changed to not getting any type of response or feedback for long periods at all it was almost a feeling of is he ok.... I was on the first round or remotes and haven't got to use it for more than half a ride so am just anxious to get some type of feedback or possible ETA on when something might be happening. Especially now that my next build is waiting for  that and only that. Will keep making due though and hope to hear something from him soon on the new version. Can't wait to get it and use it.

Thanks again for all you guys do.
```

---
## \#939 Posted by: StefanMe Posted at: 2019-06-12T19:38:16.729Z Reads: 90

```
Sorry guys. have a lot of trouble at the moment I cant give a big answer here. I am working on a new modular version with RFM and NRF module. Much more stable and less loose parts inside. I ll realise the new remote soon and will replace them. Please be patient. here is a little spoiler. 

![PHOTO-2019-05-30-16-26-37|666x500](upload://f9Be0ze0BCnYjlpPPH5GHYpJlXU.jpeg)
```

---
## \#940 Posted by: pookybear Posted at: 2019-06-12T19:46:01.272Z Reads: 89

```
I have no problem waiting at all. Hence, not following up on my receiver. I knew he has something brewing so I stopped bugging him.
```

---
## \#941 Posted by: jimmymagix Posted at: 2019-06-12T19:54:22.437Z Reads: 88

```
Look forward to having it replaced
```

---
## \#942 Posted by: tardyparty7 Posted at: 2019-06-12T19:55:12.822Z Reads: 89

```
is it bad to say i want this one instead of my current one?
```

---
## \#943 Posted by: bsancken Posted at: 2019-06-12T20:56:50.853Z Reads: 92

```
I think that is the point of a new version LOL

@StefanMe Great work on the current gen and thanks for your contributions! Cant wait for the next version, maybe I'll step up and kit together my own for a challenge. (if it will be still as open source as this current one is)
```

---
## \#944 Posted by: tardyparty7 Posted at: 2019-06-12T20:57:43.762Z Reads: 93

```
i have the current gen...
```

---
## \#945 Posted by: bsancken Posted at: 2019-06-12T21:01:17.692Z Reads: 93

```
Sorry if I misunderstood, I have several of these remotes and I love how well they work!
```

---
## \#946 Posted by: bsancken Posted at: 2019-06-16T04:54:10.900Z Reads: 90

```
So would there be any reason 2 remote/receiver pairs wouldn't work in the same vicinity? As in 2 discrete boards + remotes?

I went to ride after swapping in a second remote and as soon as a second remote or receiver was powered up, the first pair would disconnect. I'll have to do more investigating but just curious if there was any inherent issues with more than one in the same airspace... @StefanMe
```

---
## \#947 Posted by: bevilacqua Posted at: 2019-06-16T08:07:50.827Z Reads: 90

```
Look if they are not using the same frequency. 

If that does not work maybe try using the latest development SW of stefans Github. This runs directly via UART (much better) and uses a syncword to verify each package sent. 

Let me/stefan know if you use it so we can guide you in the setup process.
```

---
## \#948 Posted by: KranzeKake Posted at: 2019-06-16T12:19:58.024Z Reads: 90

```
Anyone who is selling this remote?
Please let me know, I will pay good :))
```

---
## \#949 Posted by: jimmymagix Posted at: 2019-06-16T12:54:07.763Z Reads: 91

```
I have a brand new one, with an extension board. Never used. Bought it in March but ended up using an RC remote. 

Where are you located? 

![IMG_20190611_093742|375x500](upload://5hl5KkfbiGX5UjAbkUCeUbvLiQo.jpeg)
```

---
## \#950 Posted by: KranzeKake Posted at: 2019-06-16T15:48:27.578Z Reads: 89

```
Norway, I will pay shipping. Does it come with uart or ppm?
```

---
## \#951 Posted by: bevilacqua Posted at: 2019-06-16T16:54:35.412Z Reads: 88

```
Both, ppm + uart for telemety. The latest beta FW uses only UART, much better in my opinion 

Still in testing phase tough. But it should, in theory, work as well or better than PPM.
```

---
## \#952 Posted by: KranzeKake Posted at: 2019-06-16T16:55:17.598Z Reads: 87

```
Ah great, will it work with my focbox unity?
```

---
## \#953 Posted by: bevilacqua Posted at: 2019-06-16T16:56:42.572Z Reads: 90

```
Yes, stefan himself only uses a unity right now
```

---
## \#954 Posted by: jimmymagix Posted at: 2019-06-16T16:58:00.325Z Reads: 93

```
I've already wired it to work with the Unity (had to add a JST connector to one of the wires) you can see it on the end here. 

I'm in Sweden by the way so ideal. ![IMG_20190611_093729|375x500](upload://fadsIRaZcCSgR1I0ZAvTlpCEszj.jpeg)
```

---
## \#955 Posted by: KranzeKake Posted at: 2019-06-16T17:01:44.075Z Reads: 89

```
That is perfect, if you live close to the border, we can meet at Nordby ahah
```

---
## \#956 Posted by: StefanMe Posted at: 2019-06-18T17:18:11.697Z Reads: 86

```
Please feel free to update to the newest version. 

[GITHUB LINK](https://github.com/StefanMeGit/FeatherM0-Esk8-Remote/tree/development_SMD_PCB)

Please make shure to uncomment the correct definitions for your remote in the HEADER -> SETUP section of transmitter.ino and receiver.ino. If u need some help, let me know.

- PPM over UART (no more flickering in the signal etc.)
- possibility to change between more secure connection by SYCNWORD (please change syncWord manually in transmitter and receiver)
- calibration menu on first init of remote or via settings menu (follow the instruction on screen and acknowledge with TRIGGER or MENU BUTTON)

working hard on the newer Version. We ordered the new PCB for NRF today!
```

---
## \#957 Posted by: Darkie02 Posted at: 2019-06-20T20:10:46.500Z Reads: 83

```
I’m thinking the extension board output voltage to the lights is set by the supply voltage to the module. so if I want to use 3v,5v,12v,42v,50v out put I just need to supply that to the XT30? Can any one confirm this as I’m not fully shore reading thro the posts and Github if iv understood that correct.

If so am I ok using a buck step down.
Some thing like this? https://www.ebay.co.uk/itm/DC-to-DC-Buck-Converter-20-60V-to-12V-2A-24W-Step-Down-Power-Supply-Module/323707451388?hash=item4b5e77b7fc:g:HpYAAOSwiZhccXNg
```

---
## \#958 Posted by: jimmymagix Posted at: 2019-06-20T21:06:08.705Z Reads: 82

```
@StefanMe I sold my remote from the latest batch to @KranzeKake so if he needs help, please do so, or if you release a replacement transmitter etc it should go to him.

Cheers bro
```

---
## \#959 Posted by: StefanMe Posted at: 2019-06-21T17:43:11.283Z Reads: 82

```
The input voltage is up to 10s (on some modules up to 12s) output voltage is always 12V if u want a different voltage u have to use a step up or step down converter on the output. I have never tried it. 12 ist most common for lights. I aways build some LED in row.
```

---
## \#960 Posted by: bsancken Posted at: 2019-06-22T15:13:29.520Z Reads: 85

```
So dumb question, can you indicate what the polarity is supposed to be on the power input of the expansion board? 

Still not done with the post mortem but I connected everything up with a buck converter feeding it 12v but something happened, blew a hole in the voltage reg on the converter, fried the receiver and the focbox that was supplying it power. 

This was running no expansion board fine for awhile, but it seems like it did something bad to the 5v power circuitry and incorrect polarity is the only issue I could see as the buck converter was outputting 12v fine before.(from 10s) I've patched it all up but I'm out of spare receivers so I'd like to make sure its right this time...
```

---
## \#961 Posted by: StefanMe Posted at: 2019-06-22T17:00:32.950Z Reads: 81

```
Sorry to heat that, but how could u plug in the wrong polarity? The Xt30 connector has some + and - signs on it...
```

---
## \#962 Posted by: pookybear Posted at: 2019-06-22T17:19:10.893Z Reads: 79

```
Good to see you back here @StefanMe.  :muscle:t4:
```

---
## \#963 Posted by: KranzeKake Posted at: 2019-06-25T21:13:36.419Z Reads: 76

```
Hi, I just got my remote, I have updated the firmware, but it still wont work, the remote connects and everything, but when I go to remote calibration on my Unity UI, nothing shows up. Here is a video of my wiring, any thoughts? https://youtu.be/tglSDA9oIsI
```

---
## \#964 Posted by: jimmymagix Posted at: 2019-06-25T21:34:50.365Z Reads: 82

```
You've connected the single red wire incorrectly. 

The wire should be connected to the PPM under the Servo (the connector is a double male plug but it will work in the triple female slot anyway if you push it in).

Ensure the red wire is connected to this (attached) ![Screenshot_WhatsApp_20190625-233301|250x500](upload://3sRKjsDHR2BJXOsL9b1PbtiLmSl.jpeg)
```

---
## \#965 Posted by: KranzeKake Posted at: 2019-06-25T21:40:22.343Z Reads: 77

```
Now I feel stupid....
```

---
## \#966 Posted by: tardyparty7 Posted at: 2019-06-25T21:41:51.461Z Reads: 78

```
don't worry, we all do it. when i made my first board I put the remote reciever in the wrong place too.
```

---
## \#967 Posted by: jimmymagix Posted at: 2019-06-25T21:52:26.387Z Reads: 79

```
Trust me, we've all been there (and we'll probably be there again!)
```

---
## \#968 Posted by: Darkie02 Posted at: 2019-06-25T22:42:51.478Z Reads: 77

```
Dose any one know the size of this ppm 3pin JST plug looks bigger than 2.0 of the other ones are.
```

---
## \#969 Posted by: KranzeKake Posted at: 2019-06-25T23:59:32.237Z Reads: 80

```
The remote is awesome, but I have two questions

As you can see in my video: https://youtu.be/GXsiFJB0gPU

1. Why does my PPM jump around when I am not touching the throttle?

2. I do not have any telemetry, why?

Thank you guys so much for your help
```

---
## \#970 Posted by: pookybear Posted at: 2019-06-26T00:34:10.177Z Reads: 80

```
Make sure you have these set:

* 115200bps instead of 9600
* Choose PPM and UART 

As far as PPM jumping around, it could be that your deadband is too low or loose ppm connection? Mine does this too.
```

---
## \#971 Posted by: KranzeKake Posted at: 2019-06-26T01:03:29.814Z Reads: 79

```
115200 is set, and I have PPM and UART, but still no data. Any thoughts @StefanMe ?
```

---
## \#972 Posted by: bsancken Posted at: 2019-06-26T02:30:31.555Z Reads: 84

```
Mine jumps like that too but the positive ramping time basically ignores that.

I noticed your remote batt is "low", is it actually charged? Bc I tried the latest fw and it insisted that my full battery was dead, I had to revert to an older copy to make things happy.
```

---
## \#973 Posted by: StefanMe Posted at: 2019-06-26T06:35:51.038Z Reads: 90

```
STOP guys ;) 

@pookybear go for the latest_stable build on github [GITHUB](https://github.com/StefanMeGit/FeatherM0-Esk8-Remote) .

@KranzeKake
Unity is set up to UART and Baudrate to 115200? Wires are connected to (TX to RX and RX to TX?) Do u have the correct firmware on the receiver and remote? Specialy the part #define ESC_UNITY is important.

Is this a nail bolt down with the antenna into the board? Dont manipulate the antenna. The antenna should have a length of 17.5mm. Not more and not less. 

    // FeatherFly Receiver - eSk8 Remote

    #include <SPI.h>
    #include <Servo.h>
    #include <FlashStorage.h>
    #include <RH_RF69.h>
    #include <RHReliableDatagram.h>

    // --------------------------------------------------------------------------------------
    // -------- SETUP
    // --------------------------------------------------------------------------------------

    // - Activate DEBUG - receiver will not start up when its not connected to pc
    //    and monitor in Arduino IDE is open (Baudrate: 115200)
    //#define DEBUG                 //activate serial monitor
    //#define DEBUG_TRANSMISSION    //activate transmission debugging
    //#define DEBUG_TELEMETRY       //activate UART (telemetry) debugging
    //#define DEBUG_ESTOP           //activate UART (telemetry) debugging
    //#define DEBUG_SETTINGS        //activate settings debugging

    // - Choose frequency:
    #define RFM_EU                // RFM_EU for 415Mhz in Europe
    //#define RFM_USA             // RFM_USA for 915Mhz in USA and AUS

    // - Choose board version:
    //#define BOARD_V0_1        // BOARD_V0_1 no status LED, Breaklight pin 13, Headlight pin 12, Status led pin 9
    #define BOARD_V0_2          // BOARD_V0_2 no status LED, Breaklight pin 13, Headlight pin 12, Status led pin 9

    // - Choose UART protocoll:
    #define ESC_UNITY             // ESC_UNITY for UART communication with a UNITY
    //#define ESC_VESC                // ESC_VESC for UART communication with a VESC 4.12-6.6


    // --------------------------------------------------------------------------------------
    // -------- DO NOT ANYTHING CHANGE FROM HERE
    // --------------------------------------------------------------------------------------

Should be like this....

Dont use the PPM. Go for UART ONLY. Please take a look into the NUNCHUCK settigns.

![2019-06-26%2008_35_07-FeatherRemote%20and%20SmartRemote%20(Files%20in%20post%20%23577)%20-%20Esk8%20Electronics%20-%20Electric|690x494](upload://tFhiq23vJKPC3WP6owCPQrNIxFI.jpeg) ![2019-06-26%2008_34_20-FeatherRemote%20and%20SmartRemote%20(Files%20in%20post%20%23577)%20-%20Esk8%20Electronics%20-%20Electric|690x495](upload://aj93KWOiFn39hQckn8ugcGWIJ0P.jpeg) ![2019-06-26%2008_34_04-FeatherRemote%20and%20SmartRemote%20(Files%20in%20post%20%23577)%20-%20Esk8%20Electronics%20-%20Electric|690x494](upload://kqW0AmY3AvqLSR4EudHsDw9ojdB.jpeg)
```

---
## \#974 Posted by: StefanMe Posted at: 2019-06-26T06:41:17.437Z Reads: 77

```
Holy shit man ;) u connected the receiver on PPM to the POWER of the BATTER (36V)!! @jimmymagix mentioned already.

Just remove the cable and go to UART only mode with the latest firmware please.
```

---
## \#975 Posted by: StefanMe Posted at: 2019-06-26T06:44:10.366Z Reads: 76

```
Its JST XH. i dont know why the use this stupid size. All others are JST PH
```

---
## \#976 Posted by: bevilacqua Posted at: 2019-06-26T08:17:30.397Z Reads: 77

```
I strongly recommend updating to the latest FW

(PPM is the past and UART is the future)
```

---
## \#977 Posted by: pookybear Posted at: 2019-06-26T08:23:55.768Z Reads: 77

```
@StefanMe

So wait. When doing the remote wizard, are we supposed to choose nunchuk instead of PPM with this new firmware?
```

---
## \#978 Posted by: StefanMe Posted at: 2019-06-26T08:26:28.428Z Reads: 77

```
U can use both... but UART ist better of course :) less interferce ect, more precice... (u can remove the PPM wire of course!)
```

---
## \#979 Posted by: pookybear Posted at: 2019-06-26T08:28:51.446Z Reads: 77

```
Badass. Can't wait to try this. Thanks!
```

---
## \#980 Posted by: bevilacqua Posted at: 2019-06-26T09:29:09.441Z Reads: 79

```
Yeah it confused me too, basicly select master vesc -> can_id 0 -> nunchuk and then current no reverse. Thats it, no extra calibration required.
```

---
## \#981 Posted by: Darkie02 Posted at: 2019-06-26T09:37:13.083Z Reads: 79

```
[quote="StefanMe, post:978, topic:74084"]
U can use both… but UART ist better of course :slight_smile: less interferce ect, more precice… (u can remove the PPM wire of course!)
[/quote]
 Is this because the new version is UART only as it’s more stable?

Just ordered JTS XH plugs of e bay as I only have ph ones. O well might as well put it in and then it’s there if I ever use PPM
```

---
## \#982 Posted by: StefanMe Posted at: 2019-06-26T09:40:01.256Z Reads: 77

```
Just forget PPM and the JST XH. Just use the UART over the JST PH. Works like a charm.

PPM is just a little bit more affected by interferces. But its worked fine for me. UART control is a bit more state of the art. And the cruise control works so nice now... just drive as fast as u want (even on 5km/h) release the throttle and hold the trigger and cruise...
```

---
## \#983 Posted by: KranzeKake Posted at: 2019-06-26T11:42:20.838Z Reads: 77

```
I have all that set up I believe.
I honestly dont know what to do @StefanMe 
As you can see in the start of this video: https://www.youtube.com/watch?v=RXIbDHlhMdo&feature=youtu.be , UART ONLY is selected, and Baudrate is set to 115200
But still no signal showing on the FOCBOX TOOL, and no telemetry on my remote
```

---
## \#984 Posted by: StefanMe Posted at: 2019-06-26T12:10:40.821Z Reads: 81

```
Switch RX and TX. Dissconnect the board from power to restart the receiver. If u want we can do a short debug via TeamViewer
```

---
## \#985 Posted by: KranzeKake Posted at: 2019-06-26T12:14:42.814Z Reads: 81

```
How would I go about switching them? Swap the cables in the white connector?
```

---
## \#986 Posted by: StefanMe Posted at: 2019-06-26T13:05:41.356Z Reads: 84

```
As we mentioned before, he had to swtich RX and TX to get the UART data. Looks good now!
```

---
## \#987 Posted by: pookybear Posted at: 2019-06-26T23:49:35.207Z Reads: 83

```
Updated my buddy's remote and receiver. Went pretty well. I like how you get that calibration prompt after you flash the remote. Also the remote / board battery alarm. My friend needed that. He didn't "know he was low on remote battery one night and had to kick push. So funny. :joy:

So far from bench and quick ride test. New firmware took care of the initial throttle throw lag. Smooth! I will test some more tomorrow. Had to go to work.

@StefanMe.
Good job man.

I will ride lots tomorrow and check the connectivity. Will get mine updated as well tonight when I get home.
```

---
## \#988 Posted by: pookybear Posted at: 2019-06-27T00:16:17.039Z Reads: 79

```
One thing I've noticed is the remote battery. Before I updated the remote, battery was full bar. After flashing, it was telling me low battery.
```

---
## \#989 Posted by: bsancken Posted at: 2019-06-27T02:56:10.812Z Reads: 85

```
Yes, this. hoping there is a fix for that. Makes me nervous.

[quote="pookybear, post:988, topic:74084"]
Before I updated the remote, battery was full bar. After flashing, it was telling me low battery.
[/quote]

Edit.  -  Left is current(as of a weekish ago) build   ||||    Right is Old code as of Apr. 20th.

Seems like line 1867 on the left has added step in getting the voltage var.
its multiplying the voltage that is normally just used on the old code. The remoteBatteryFactor is new which has a value of 

    float remoteBatteryFactor = 0.83; //on line 545

    float voltage = uncompvoltage * remoteBatteryFactor;  //on line 1867


![30%20PM|690x237,75%](upload://emEYvi6I9bScaohRiAI1NbttYCE.png)
```

---
## \#990 Posted by: Jansen Posted at: 2019-06-28T01:15:44.151Z Reads: 82

```
Have you received the remote & receiver I sent back to you a couple weeks ago to swap out for me yet @StefanMe ? My unity will be here in a week and that plus your feather remote are the last 2 items of my build so hoping to find out how soon you think you'll be sending the new version over to me.... lmk when you can and thanks again for all the hard work brotha.
```

---
## \#991 Posted by: Jansen Posted at: 2019-07-01T21:24:57.615Z Reads: 82

```
Yolo..... @StefanMe shoot me an update if you could when you have a chance. Just want to confirm you got the remote I sent back to you and find out when I might expect the replacement since my build is done tomorrow and that's the inly thing missing now. Thanks brotha. I DM'd you my new addy too FYI.
```

---
## \#992 Posted by: walleywalker Posted at: 2019-07-02T17:35:15.927Z Reads: 81

```
Would it be possible to swap in an e-paper display in this remote?  Makes for easy visibility in sun-light and at night if it's back-lit.
```

---
## \#993 Posted by: pookybear Posted at: 2019-07-04T04:41:13.742Z Reads: 82

```
Were you able to figure out a better numerical value for the remoteBatteryFactor instead of 0.83? 

Maybe @StefanMe?
```

---
## \#994 Posted by: bsancken Posted at: 2019-07-04T04:43:09.156Z Reads: 81

```
I was just trying to do the work of pointing out where I thought the issue was, I do not trust myself to understand how all that code works together enough to want to suggest a change Lol

I was just hopin to help out @StefanMe
```

---
## \#995 Posted by: pookybear Posted at: 2019-07-04T04:45:50.959Z Reads: 85

```
I was trying to  code it w my noob skillz but it would NOT compile. Shocker, I know :joy::man_shrugging:t4: I just need to figure out how he came up w that value.
```

---
## \#996 Posted by: StefanMe Posted at: 2019-07-04T09:00:21.170Z Reads: 83

```
Easy... i measured two two batteries, connected them to the remote and calibrate it with the factor 0.83.

Maybe this doenst work properly. I ll take a closer look the next days.
```

---
## \#997 Posted by: krazor Posted at: 2019-07-05T12:43:18.255Z Reads: 88

```
Been a little over a month since ive been on the forums and im glad to be back since i moved inner state im finally settled in. got some news to share with you guys also. Was speaing with a mate of mine tonight and got some new Throttles modeled up that he has offered to share with the community. i asked him to make some mods to the current throttle to allow 2 small bearings to be used inside for a smoother throttle. Currently on the printer for first test.


 ![image|619x500](upload://cq1eFk4uCqv5DzBIkH0vZGvuh4x.jpeg)
```

---
## \#998 Posted by: tomiboi Posted at: 2019-07-05T21:35:20.343Z Reads: 83

```
Hey guys:) What would have to be done to get the battery setting on the transceiver to go higher than 12s? Also, I'm having this issue where the speed registers at exactly twice the actual speed. I fixed the problem by cutting the wheel size in half, but I'm worried that it might effect other data outcomes negatively. Any idea what's going on there?
```

---
## \#999 Posted by: bsancken Posted at: 2019-07-09T02:21:51.566Z Reads: 74

```
Any reason after changing receiver boards, my range sucks? I fried one rx feather so I threw in a spare board and now suddenly my range went from being able to be atleast 6ft away to if my leg blocks line of sight to the box that the rx is in, it disconnects. 

I even got the antenna sticking out the bottom of the remote. Didn't modify the length either.
```

---
## \#1000 Posted by: pookybear Posted at: 2019-07-09T04:09:14.283Z Reads: 76

```
Try re-uploading the firmware?
```

---
## \#1001 Posted by: bsancken Posted at: 2019-07-09T04:16:22.244Z Reads: 76

```
I flashed an older version and the newest version as of a week or 2 ago and didn't see changes. Maybe I'll check the latest version.
```

---
## \#1002 Posted by: StefanMe Posted at: 2019-07-09T05:37:46.907Z Reads: 75

```
Did u have the correct frequency? In us u need the 915 Mhz Version. U also have to activate the 915Mhz by uncomment define RFM_USA in transmitter and reciever.

    // - Choose frequency:
    #define RFM_EU                    // RFM_EU for 415Mhz in Europe
    //#define RFM_USA                 // RFM_USA for 915Mhz in USA and AUS
```

---
## \#1003 Posted by: StefanMe Posted at: 2019-07-09T05:42:16.683Z Reads: 76

```
I updated the software to 14s. 

About the speed problem... Can u tell me more about your motor setup? did u set up the motor poles correctly?
```

---
## \#1004 Posted by: pookybear Posted at: 2019-07-09T20:41:11.265Z Reads: 83

```
@bsancken 
I couldn't stand the battery being only at 2 bars plus the annoying warning (which I can easily turn off in the settings menu). Here is my "fix".

***Change line 1866 from:***
```
float uncompvoltage = (refVoltage * 2 / 1024.0) * ( (float)total / (float)samples );
```

***To***:
```
float voltage = (refVoltage * 2 / 1024.0) * ( (float)total / (float)samples );
```

***I deleted these lines from transmitter.ido:***

```
Line 454       float remoteBatteryFactor = 0.83;

LIne 1857                   #ifdef DEBUG_BATTERY
Line 1858                     Serial.print("Battery sample value: "); Serial.println(analogRead(batteryMeasurePin));
Line 1859                   #endif

Line 1862                   #ifdef DEBUG_BATTERY
Line 1863                     Serial.print("Battery average value: "); Serial.println(analogRead(batteryMeasurePin));
Line 1864                   #endif

Line 1867       float voltage = uncompvoltage * remoteBatteryFactor;
Line 1868                   #ifdef DEBUG_BATTERY
Line 1869                     Serial.print("Battery voltage: "); Serial.println(voltage);
Line 1870                   #endif
```

I pretty much deleted the debug parts and "remoteBatteryFactor". I referenced it to the older versions that didn't have these lines. It recompiled and uploaded successfully to my remote. 

Previous version of these set of lines worked pretty good for me. Not sure if this is the correct way to do things. I figured there should be no harm from it due to it only for calibration purposes. I could be wrong.

Use it at your your own risk. I will test it when I get a chance.

![Attach187750_20190709_131424|281x500](upload://6qzWlg7XJspNMiDbjEL1cJj6bvm.jpeg)
```

---
## \#1005 Posted by: bsancken Posted at: 2019-07-14T14:07:40.073Z Reads: 84

```
Been awhile but The remote still needs like line of sight within 3 ft... If I turn my hand or move it, ill disconnect till I move it back causing me to jerk to a stop.
```

---
## \#1006 Posted by: pookybear Posted at: 2019-07-14T18:40:08.741Z Reads: 84

```
So I have been testing the remotes battery for the past few days with the deleted lines above. I can see the bars go down as I use it more and more. When there is only 2 battery bars left, it doesn't go to 1 bar  blinking (this tells you to charge your remote). The remote just turns off. This is probably why @StefanMe added those lines.

So I looked again at the code to try to understand it. Mind you I'm new to this. I can follow the coding but only partially understand it. I had to refer to Arduino's reference to understand the commands. 

I finally came up with remoteBatteryFactor of 0.95 after a number trial and error. Yes, this is with each fully charged remote and using it to discharge until I hit 1 bar battery level. 

How did I come up w this value? I simply use 4 (# of full bars in remote battery indicator) divided by 4.2v (battery fully charged voltage) which yields to 0.95. Logic behinds this is 1 bar of the indicator represents the level of charge. It actually works.
```

---
## \#1007 Posted by: Jansen Posted at: 2019-07-16T20:37:01.933Z Reads: 78

```
Hit me back when you can @StefanMe Appreciate it!
```

---
## \#1008 Posted by: krazor Posted at: 2019-07-18T12:36:57.411Z Reads: 81

```
I ended up building the hardware for the Feather M0 Firefly Nano remote. just wondering what i would need to modify in this code in order to get it running since it uses the same Boards Feather M0 i assume all should be good apart from changing the pins and modifying the input for the second button and the POwer button since this one uses a switch?


Also i cant seem to find the documentation for uploading the code to the remote/reciever. Does anything need to be modified through code or is it all handled through a menu etc?
```

---
## \#1009 Posted by: tomiboi Posted at: 2019-07-19T19:03:45.984Z Reads: 76

```
Sorry, for the delayed response. Thank you for updating the code :) I think the problem may be the motor poles. I have it set to 14.
```

---
## \#1010 Posted by: tomiboi Posted at: 2019-07-20T17:43:34.124Z Reads: 76

```
Has anybody run this with the UNITY and the UNITY app? Were there problems getting telemetry on the remote and app simultaneously? Conflicting baud rates?
```

---
## \#1011 Posted by: bevilacqua Posted at: 2019-07-20T19:20:14.570Z Reads: 75

```
It works with the FB Unity aswell 👍
```

---
## \#1012 Posted by: kiryl Posted at: 2019-07-27T15:30:48.329Z Reads: 72

```
@StefanMe my remote has been broken for 2 months now, can I please get it fixed or sent a new one?
```

---
## \#1013 Posted by: Jansen Posted at: 2019-07-28T19:44:29.344Z Reads: 73

```
Dido. @StefanMe you should have received mine I sent back more than a month ago but still haven't heard back from ya since.... whats the status of getting a new remote that works?
```

---
## \#1014 Posted by: tomiboi Posted at: 2019-07-29T02:10:32.587Z Reads: 73

```
When I upload the newest code as UNITY everything goes just fine, but when I upload as VESC I get an error. I'm sure that I've made a silly mistake. Does anybody have a clue what it might be?

![Annotation%202019-07-28%20200616|419x500](upload://eCfpot7NaaOhg9IHHLmJpt2S3ye.png)
```

---
## \#1015 Posted by: Jansen Posted at: 2019-07-30T19:02:23.690Z Reads: 66

```
Should I just assume I won't be getting a replacement remote at this point or what should one think since there are no longer any replies to PM's or comments here....? Hope all is ok with you @StefanMe Just wondering what's up and still not even sure you got my remote I sent back to you, you should have received it a month or a Lil more ago.
```

---
## \#1016 Posted by: tomiboi Posted at: 2019-07-30T19:14:04.743Z Reads: 65

```
Just be patient, friends. Use a cheap, old-school remote for a while and go have a nice ride. With DIY and open-source projects we're all a part of the process :slight_smile: The journey is the destination. Don't hate me for saying that :upside_down_face:
```

---
## \#1017 Posted by: tomiboi Posted at: 2019-07-30T19:22:53.913Z Reads: 64

```
I resolved this problem. Thanks for all of your great work :slight_smile:
```

---
## \#1018 Posted by: tomiboi Posted at: 2019-07-30T20:14:11.931Z Reads: 63

```
With the newest version of the firmware the trigger seems to be stuck in killswitch. Changing it to cruise has no effect.
```

---
## \#1019 Posted by: walleywalker Posted at: 2019-07-31T20:24:02.124Z Reads: 61

```
Anyone happen to have a 3D .STEP file for the remote?  I want to add soft touch grips to the housing before printing
```

---
## \#1020 Posted by: bevilacqua Posted at: 2019-07-31T20:39:43.269Z Reads: 60

```
its on thingiverse
```

---
## \#1021 Posted by: walleywalker Posted at: 2019-07-31T20:51:21.546Z Reads: 63

```
There's only STL files in the thingiverse set
```

---
## \#1022 Posted by: bevilacqua Posted at: 2019-08-01T05:19:03.951Z Reads: 64

```
oh right... I missed that part
```

---
## \#1023 Posted by: walleywalker Posted at: 2019-08-01T15:33:59.093Z Reads: 67

```
@StefanMe I know you're plugging along on the new design, but I REALLY like the current one. 

Do you think you'll be trying to update the firmware for the current 915 Mhz Feather to implement channel/frequency hopping and stuff to reduce packet loss? 

Or at least have drop-in 2.4ghz parts for the current remote case?
```

---
## \#1024 Posted by: walleywalker Posted at: 2019-08-09T16:24:23.094Z Reads: 61

```
Does anyone know the magnet dimensions? I have a DIY kit and it didn't come with them.

Edit: Is it the 5mm x 5mm like all the other remotes?
```

---
## \#1025 Posted by: pookybear Posted at: 2019-08-10T02:19:23.361Z Reads: 59

```
They should be stated in the BOM. Check first post?

Edit:

I have some left over magnets. I'll measure them.
```

---
## \#1026 Posted by: Qrob Posted at: 2019-08-13T23:35:00.555Z Reads: 54

```
@StefanMe i will pay for this remote if you are doing so
```

---
## \#1027 Posted by: Jansen Posted at: 2019-08-14T21:22:53.893Z Reads: 53

```
Anyone heard from @StefanMe recently at all.....?
```

---
## \#1028 Posted by: tomiboi Posted at: 2019-08-18T21:35:29.583Z Reads: 48

```
@Qrob I sell upgraded full-builds at my website 3sk8esk8.com.
```

---
## \#1029 Posted by: bsancken Posted at: 2019-08-18T23:30:25.454Z Reads: 47

```
I know you have upgraded hardware but is it still based on the feather and the same core transmission code?
```

---
## \#1030 Posted by: tomiboi Posted at: 2019-08-19T00:09:53.790Z Reads: 45

```
Hardware and some electrical engineering pertinent to the throttle have been upgraded. The code is the same. I'm still using 2.4 GHZ RF and feather. Things have been going well. Have you been having issues with the transmission?
```

---
## \#1031 Posted by: tomiboi Posted at: 2019-08-19T01:03:15.209Z Reads: 46

```
I'm curious about the transmission issues. I've really had next to no drops is six months of use. I've got several out there now. The big changes that I made were to the throttle. It's a lot more complicated. The throttle on the original project is pretty simple. It could certainly be causing dips and spikes that could lead to resets.
```

---
## \#1032 Posted by: bsancken Posted at: 2019-08-19T01:05:40.234Z Reads: 45

```
For me I have 2 of Stefan's designs which use 915mhz US feathers and theyre unusable....
If I swing my hand and my leg gets inbetween it'll disconnect.. The antenna is behind a ~5mm plastic wall of the case but that is mounted to the top of my board between my legs.

If I bring my hand up to my chest - disconnect. hold it still - disconnect.
It reconnects fast but it'll just suddenly stop accelerating and that's enough to throw me, especially not good if I'm in traffic.
```

---
## \#1033 Posted by: tomiboi Posted at: 2019-08-19T01:10:08.447Z Reads: 45

```
That sounds very dangerous. Have you had these remotes for a while? Did they ever work well? Have they been dropped?
```

---
## \#1034 Posted by: bsancken Posted at: 2019-08-19T01:16:04.463Z Reads: 48

```
Had one (a), worked pretty good riding around college. 

Fried receiver of (a) after I lost a Focbox, by the time I rebuilt the board (with a spare receiver) there was an update for the code so I updated. 
(same time) Bought a second one for another board (b).

After I got my board together it worked but I started experiencing my first disconnects while riding with (a)
Experiencing same thing on (b)

Rolled back to the initial code that I was using originally(from my downloads)
Neither controller has been the same since. 

Thoughts or suggestions? Haven't been dropped and I assembled/printed everything..

*Edit -------

Also binding (a) to (b) rx and vice versa doesn't help either
```

---
## \#1035 Posted by: tomiboi Posted at: 2019-08-19T01:36:01.749Z Reads: 49

```
I'm using older code as well. The newest code has some issues with the kill-switch. I couldn't turn it off and I hate kill-switches. Externalizing the antenna could never hurt. I upgraded to a uFL antenna because it was cheap and easy. 

So much of what your saying sounds like a connection is wiggling loose in the remote. It sounds almost too crazy to be a basic transmission issue. To cross that off the list, I would inspect the solder joints, especially if you open and close the enclosure a lot. This can cause the little wire joints to crack. Reinforcing the connectors with a dab of hot-glue will help to ensure that they aren't wiggling loose. I hard-soldered and reinforced my joints instead of using connectors. 

Another suspect is the battery. Though these little lipo batteries are extremely convenient for remote-making. They are also kind of shitty, especially the little ones. I don't use the sleep mode because it uses battery and will run it down and ruin it if you don't use your remote for a few days. Maybe try switching out the batteries.
```

---
## \#1036 Posted by: Jonisonvespa Posted at: 2019-08-20T08:28:00.357Z Reads: 47

```
Hello are these available if so how much
```

---
## \#1037 Posted by: Jansen Posted at: 2019-09-04T19:47:23.169Z Reads: 43

```
is it safe to say I'm never going to get my replacement remote after sending mine that didn't work back a couple of months ago and that I'm just out completely in regards to @StefanMe and the feather remote....? Cause that really sucks if so but still no reply in a couple of months now....
```

---
## \#1038 Posted by: Ineedspeed Posted at: 2019-09-06T06:19:44.741Z Reads: 41

```
So are the breaklight now set to function like a cars? Always responding to breaking, but when headlights are on the tailigjts also function as breaklights by getting brighter when triggered?
```

---
## \#1039 Posted by: KranzeKake Posted at: 2019-09-09T12:57:43.479Z Reads: 39

```
Im having major connection problems..... Is it possible to swap the feather board with a bluetooth version, like the Adafruit NRF52832 ?
```

---
## \#1040 Posted by: tomiboi Posted at: 2019-11-17T14:54:14.228Z Reads: 28

```
I had connection issues that were resolved by increasing the amount of external antenna. 3 inches for the 915 model and 6 inches for the 433 model.
```

---
