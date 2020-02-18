# EXTENDED ACKMANIAC-ESC Tool based on VESC-Tool

### Replies: 874 Views: 40823

## \#1 Posted by: Ackmaniac Posted at: 2017-10-08T18:21:32.170Z Reads: 1598

```
## PPM changes

**Current control is like the old Watt control mode**

Finally, Watt Mode is made especially to give you much more control at higher speeds. At the beginning, you think the VESC has less power but then you learn that you simply have to pull the trigger a bit more. And when you start to carve at higher speeds you will definitely feel the difference. And another advantage is that when you set a watt limit (motor settings) the power feels the same over the whole battery capacity.

"Current" Control Mode works like "Current no reverse with Brake" with the difference that you also have a reverse. The only problem with the standard reverse function is that when you brake hard the wheels can start to spin backward while you still move forward.
.
**To avoid that i added the parameters "Enable maximum ERPM for direction switch"**

<img src="/uploads/db1493/original/3X/7/b/7be5603226b3ada75215271e5c2891a28ca2f7d6.png" width="690" height="235">

When this is enabled and you brake hard then the brakes will work like in "Watt with no reverse". To drive backward you have to release the throttle and brake again. But this only works when you are below the ERPM (4000 in the picture). If you are above it will brake normally again.
When you drive backwards and you are above 4000 ERPM in the backwards direction then it will accelerate backwards and won't brake. If you are below 4000 ERPM backwards and you accelerated shortly to go forward and brake again then it will enable the normal brake again. To drive backwards you have to release the throttle and brake again.
.
How do i find the perfect ERPM for that parameter?_
The best is to go down a hill. Then do a full brake. You will see that the motors are not able at very low speed to stop the board from moving. If the value is set correct you can now release the throttle and brake again and the motors should start to accelerate backwards. If that is not the case then the value is too low. In my tests 4000 ERPM worked very well. For most setups that is like 4 km/h.
-
It sounds complicated but it becomes very intuitive after a short while. If you don't need it to go backwards then just simply use "Watt no reverse with Brake"

**PID speed control no acceleration**

This mode is experimental, when you press the throttle then it only activates the Cruise Control and hold the speed. Brakes work as normal. So there is no acceleration. This might be good to legalize the board in some Countries.

**Offset for Traction Control**

Problem is that the standard firmware always reduces the power at one VESC when traction control is enabled. Because the RPM reading of the VESC is not very precise and can differ by +-400 RPMS. And that means that at 500 updates per second the Current for the VESC bounces a lot. Alos when you make do a curve then the inner wheel is slower than the outer wheel. So the outer wheel will get less power and by this it creates a power steering. To prevent this you can define an offset where the VESC should not reduce the power and deliver the same current to both VESCs. Above that offset, the normal traction control will step in. If you set this to 3000 for the most setups this will not enable traction control if the speed difference between both VESCs is lower than 3 km/h.So the traction control only reduces the power when it is really needed.

## Cruise Control for dual setups via steering channel connected to the second VESC:
At the slave Vesc the steering channel can be connected and in the PPM settings the "Cruise Control via Secondary Channel" can be activated. This enables the cruise control when the throttle is not pulled and the steering channel is turned more than 30% to left or right. In this mode braking is always possible, just to avoid stupid reactions in a shocking moment. And when you pull the throttle the cruise control will also be deactivated to avoid that the throttle is accidentally pulled while cruise control is active and then have a big surprise when cruise control is released. So i hope that i can avoid scary situations.
I recommend to set the Speed control settings in the Advanced tab to 0,00300 for KP and KI and leave KD to 0,00000. 
For cruise control the 2nd ESC need to be connected via can bus and the Slave ESC needs to send the status via can. The Master ESC needs have "Multiple ESCs over Can" enabled.

In the picture above you see that you have additional options when you use the steering to activate the Cruise Control.
You can define what should happen when the Pulsewidth is negative (lower than 50%) or positive (higher than 50%). If you use the motor settings the behavior will be like you set it up in the Motor advanced tab. Otherwise, you can define if you want to allow the speed controller that it can use the brakes if you go faster or not. 
For example it is possible when you steer right that cruise control ´doesn't brake when you are too fast and when you steer left that it dos use the brakes. This way you can use the cruise control for carving and downhill. 

Hint: mostly when you steer right it gives lower signal and when you steer left it gives a higher signal.

## Nunchuk changes
- Nunchuk also has the Offset for Traction Control
- Buttons can be mirrored
- Cruise control is changed so that for a dual drive the speed of both wheels will be taken into account and adjusted individually
- When Current without reverse is used then one button is for cruise with brake and the other for cruise without brake.
- When Current with reverse is used then braking will be disabled during cruise control and can  be activated by short brake pulse while cruise control is active.

## Timeout Behavior
I spent a lot of time to find a good solution to make the board safer when the connection to the remote is lost.
**What is the Issue with the standard firmware?**
When the remote looses the connection the the ESC immediately switches to the defined timeout current after the defined timout time which is mostly 1000ms (1s). in most cases this is 0 A. 
So if it happens during acceleration then the ESC will continue to accelerate for 1s with the last known throttle position and the cut off the power immediately. If the signal comes back now the power will be back imediately. So it can happen that the ESC acdcelerates with 80A, then goes to 0 and back to 80A. 
Mostly this was a very good chance for a very bad crash.
And it got even worse when a brake current is defined when a timeout happens.

The solution i added is a soft ramping from the actual current to the defined timout current. So a brake current can be defined because it will smoothly change from acceleration to braking. And if the signal comes back it will also ramp smoothly to the actual throttle position. So the times when the board wanted to throw you off should be a thing of the past.
And to be able to still push the board the automatic braking will disable itself once the motor comes to a complete stop for 1 second. (Be aware that you should only push the board when the ESC is switched on)

**BUT actually this works out of the BOX for Nunchuk and NRF.**

**For PPM this is also possible**. But it is a bit difficult to set it up and it doesn't work with every remote because the Failsafe signal needs to be adjustable.

**Instructions for PPM with adjustable Failsafe:**
At the mini remote the failsafe is adjustable by removing the bind plug while the throttle is in idle. By this the receiver knows what signal it should send as default if the connection to the remote is lost.
But this looks like a idle position for the ESC. 
So we need to tell the ESC that the signal is lost an this can be achieved by adjusting a failsafe signal that is far below or above the min or maximum signal.

So for example when your remote is adjusted then min and max is like in the next 2 pictures
**Minimum** 
<img src="/uploads/db1493/original/3X/2/0/20577be728a9c8fd0d846eeb06f5f81442e66334.png" width="690" height="96">
**Maximum**
<img src="/uploads/db1493/original/3X/e/4/e4dacb9d5035c5b4672ecb54a9245679820cb40a.png" width="690" height="91">

To set a failsafe signal that is far off i attach the bind plug and turn the potentiometer on the remote totally to the left and pull the throttle 100%. That gives me a signal of 
<img src="/uploads/db1493/original/3X/1/5/155e3f5386e3039724bfcf540cc4691f8941912b.png" width="690" height="89">
In that moment i remove the bind plug to tell the receiver to send this signal if the connection is lost.
Afterwards i turn the poti back to the normal position (best is to adjust min, max and center again). 

When you switch off the remote now you should see the signal that is far off. In my case it shows 170% in brackets (in the picture above). If the signal is above 120% the ESC knows that the signal is lost.
Now you can define a timeout current in the General settings. Safe the settings and let the motor spin with the remote. When the motor spins switch of your remote. Now the motor should brake automatically. 
On the bench it seems that it brakes hard but test it on the street at low speed. You will feel that the bakes apply gently. If you test this during acceleration you will also feel that the acceleration power is ramped down gently and brake increases.
The ramp current is 50A /s decreasing and 20A/s increasing. So from 50A to -15 it would need 1 second to decrease to 0 and then from 0 to -15 it woulkd take 0,75s to -15. If you have dual drive connected via CAn the slave will do the same as long as the same timeout brake current is adjusted.

I recommend to set a brake current of -10A or -15A which will slow you down even downhill. And also the timeout ms should be set to 500ms so that the ramping starts very soon when the connection is lost.

_**It would be cool if you would send me a donation if you think that this timout behavior saved your skin and bones.**_

## Watts Limit usage
IMPORTANT you have to do this for each motor individually, Master and Slave.
If you set this value to 1000 Watts then 25 % throttle will be 250 watts and 100% throttle will be 1000 watts. Of course, the throttle curve will have an influence. 
The battery max has the higher priority, So if the battery max is set to 10A and your battery has 36V then you can only produce 360W maximum. If you set the value to 1000 Watts then you can only use 36 % of your throttle because afterward the battery max blocks a higher power output.
So just make sure that the battery max allows the VESC to produce that many watts. You can also easily limit the VESCs power output with this parameter so that it would be very easy for the kids to ride the board.

## Other changes
- Hall sensor in BLDC mode has a hysterysis which results in a smoother switch from sensor to sensorless mode
- Cruise control works different and smoother than in the standard or previous 2.54 firmware
- FOC for FOXBOX works
- My app is supported
- Brakes can be stronger than acceleration. This way a weak acceleration but strong brakes can be defined which should be safe for kids. 
- For a 4WD different settings can be used for the front and back axle
- ESC-Tool shows in the realtime data graph also the speed and distance based on the settings in the additional information tab. 
- Throttle curves shows more grid lines to better see the effect on the power curve.
- Throttle cuves have one more mode which is called "Expo-Natural"

## [ACKMANIAC-ESC Tool Link](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0)

## [App in PlayStore](https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor)

-

**_And if somebody wants to honor all the work. (many hundred hours)_**
:point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down::point_down:
**[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY) :money_mouth: [Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY) :money_mouth: [Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=GJ59FXYPUQHUY)**
:point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2::point_up_2:

When you want to send a donation then don't use dots. (Germany uses commas). So use full numbers or a comma.
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-10-08T18:26:51.370Z Reads: 1083

```
SWEEEETTT!  Maybe I’ll send a couple dollars over later
```

---
## \#3 Posted by: SilentException Posted at: 2017-10-08T18:45:18.852Z Reads: 1078

```
Stage 2 failsafe? Wishlist item crossed off my wishlist without even asking :) So awesome, gotta try this!
Only the arming procedure missing now (for Nano-X and Nano v2).

BTW, I clicked on donations link but it throws up the error on PayPal side. Might check that out.

Thanks, would give you 10 likes if I could.
```

---
## \#4 Posted by: Paulf Posted at: 2017-10-08T18:48:13.075Z Reads: 1027

```
AMAZING!!! You've been very quick considering everything you've done! The timeout behavior looks like what I was dreaming about ! Looks like the time to switch to Vesc-tool has come. Will definitely give a few bucks when I get the chance!
Thanks
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-10-08T18:53:38.774Z Reads: 935

```
Think i fixed the Donations button
```

---
## \#6 Posted by: MontPierre Posted at: 2017-10-08T18:56:14.363Z Reads: 881

```
Wow! @Ackmaniac does it again!!!
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-10-08T18:56:34.708Z Reads: 858

```
I'm broke but was able to scrounge up 1 euro for you.  Great job!
```

---
## \#8 Posted by: SilentException Posted at: 2017-10-08T18:56:59.093Z Reads: 850

```
Yes, you did ;)
```

---
## \#9 Posted by: Pedrodemio Posted at: 2017-10-08T18:57:26.753Z Reads: 828

```
Nice, does it work with VESC 6? And the updates that Benjamin make on the main branch also get included or you have to manually add them if they are worth?
```

---
## \#10 Posted by: Silverline Posted at: 2017-10-08T19:49:55.881Z Reads: 804

```
Sweet

Regarding "FOC for FOCBOX work" What did you do ? And why do Benjamin not understand whats wrong, when you do :-) ??


Do the Metr app work, with this FW ?
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-10-08T20:01:57.162Z Reads: 782

```
It should also work with VESC 6 (don't have one). All the firmware files are added to the ACKMANIAC-ESC Tool.
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-10-09T06:53:11.952Z Reads: 767

```
When you install the failsafe you should make sure that it works by testing it first on the bench and then at low speed on the street. Be aware that the same failsafe current should be set for Master and Slaves if you have more than one motor.
```

---
## \#13 Posted by: jujet Posted at: 2017-10-09T10:26:08.466Z Reads: 758

```
You should accept BTC donations as well, for people who don't have shitty paypal :smiley:

Thanks for your contribution once more, you're a legend!
```

---
## \#14 Posted by: notger Posted at: 2017-10-09T10:47:40.553Z Reads: 728

```
"cruise control via second..."  is also current mode right ??
```

---
## \#15 Posted by: Ackmaniac Posted at: 2017-10-09T12:38:35.513Z Reads: 731

```
"Cruise Control via Secondary Channel" is only used at the slave ESC. It doesn't give any power commands. It only tells the master if cruise control (tempomat) is active and if enabled that braking is allowed or not at cruise. The master controls the power so it depends which mode is active at the master.
```

---
## \#16 Posted by: Vanarian Posted at: 2017-10-09T12:55:37.299Z Reads: 714

```
@Ackmaniac Could you add the sources of your new ESC-tool and firmwares to the dropbox ?

I wanna run this firmware! (must recompile versions adapted to my VESCs by myself) 

Thanks for your hard work!
```

---
## \#17 Posted by: Esk8HubsUS Posted at: 2017-10-09T12:59:48.691Z Reads: 698

```
Amazing ,thanks Ackmaniac!  ...any chance of a Mac version ?
```

---
## \#18 Posted by: MontPierre Posted at: 2017-10-09T13:50:11.897Z Reads: 712

```
[quote="Esk8HubsUS, post:17, topic:35116"]
any chance of a Mac version ?
[/quote]

@rpasichnyk 🙏🏻🙏🏻🙏🏻🙏🏻
```

---
## \#19 Posted by: SORRENTINO Posted at: 2017-10-09T14:15:27.079Z Reads: 702

```
@Deckoz @pshaw
```

---
## \#20 Posted by: Pimousse Posted at: 2017-10-09T14:59:03.415Z Reads: 718

```
[quote="Ackmaniac, post:1, topic:35116"]
FOC for FOXBOX works
[/quote]

So you finally figured out what was wrong ?
Does Vedder know the bug ?

Anyway, nice job !
Can't wait to look at your sources.
```

---
## \#21 Posted by: notger Posted at: 2017-10-09T16:08:48.279Z Reads: 678

```
@Ackmaniac  do you own a focbox for tying it out ?  

cause im still a bit worried about destroying my new focboxes here, still it seems really amazing what you did here again, thanks
```

---
## \#22 Posted by: Ackmaniac Posted at: 2017-10-09T16:42:28.317Z Reads: 660

```
Tested it with FOCBOX, 4.12 HW, 6355 Motor, 6374 Motor, 28 Pole Hub Motor, NRF remote, PPM remote and Nunchuk. I don't have a VESC 6 but i am confident that it works with it as well.
```

---
## \#23 Posted by: Deckoz Posted at: 2017-10-09T17:38:28.500Z Reads: 649

```
@Ackmaniac is this for the new vesc 3.2X firmware? I'm curious as I've already been running FOC on the FocBox for several hundred miles on the 2.54 release?
```

---
## \#24 Posted by: Fatglottis Posted at: 2017-10-09T17:44:09.339Z Reads: 636

```
Eeeey!! Awesome to see this implementation of the timout behaviour. I remembered that we talked about this briefly in a post one time. After that I actually implemented it myself with arduino and it's a really nice bone saving feature!
Your version will save others bones as well :D
```

---
## \#25 Posted by: TranxFu Posted at: 2017-10-09T17:50:20.516Z Reads: 634

```
Tried it with my FOCBOX. Motor Setup and FOC mode worked out fine. However the PPM Setup wouldnt work out :/ It sets the limit right but whenever it goes into neutral(center) position the motor goes on full duty. Any ideas ?
```

---
## \#26 Posted by: BigBoyToys Posted at: 2017-10-09T18:17:23.683Z Reads: 621

```
Ill give it a try on some VESC 6's later today and report back.
```

---
## \#27 Posted by: Ackmaniac Posted at: 2017-10-09T18:25:47.977Z Reads: 614

```
Just set the min, center and max pulse width right. Then it will work. Otherwise just post screenshots of your settings.
```

---
## \#28 Posted by: Titoxd10001 Posted at: 2017-10-09T18:32:27.972Z Reads: 612

```
Is there a certain erpm and amps we should set for 190kv 6355 motor for motor detection?
```

---
## \#29 Posted by: TranxFu Posted at: 2017-10-09T19:14:22.590Z Reads: 603

```
The pulse width gets set correctly just like in your bldc tool. But even after applying the right values and it shows it as center. If I pull the trigger/Brake all the way it stops but if it goes near the center it start spinning up.
```

---
## \#30 Posted by: Vanarian Posted at: 2017-10-09T19:17:52.923Z Reads: 586

```
Up again can you please attach the source files to your drop box? I can't run your firmware without them.
```

---
## \#31 Posted by: Ackmaniac Posted at: 2017-10-09T19:44:10.349Z Reads: 574

```
Please show a screenshot while the trigger is in center position.
```

---
## \#32 Posted by: Vanarian Posted at: 2017-10-09T20:57:16.818Z Reads: 584

```
I just realized that my inquiry was dumb since you **did** include the Ackmaniac-ESC TOOL sources in the ZIP. Sorry for the bother and insistance but allow me to be more accurate : 

Can you please upload a ZIP with the uncompiled sources of your modded FW / the raw file directory of your modded bldc-master ? 

I'm redundant but I got different assigned GPIOs on my VESCs (and also 0.0005ohms resistors) and need to make mods in few files then compile myself any upcoming FW. Currently I've made variants of original 3.28, 3.29 and a variant of 2.54 based on your older bldc-master directory.
```

---
## \#33 Posted by: Ackmaniac Posted at: 2017-10-09T21:17:40.218Z Reads: 560

```
@The_Dude was so nice to compile it for OSX. You can find it in the Dropbox link.
```

---
## \#34 Posted by: ARetardedPillow Posted at: 2017-10-10T02:56:10.636Z Reads: 543

```
Youre like the Benjamin of vesc tools lol
```

---
## \#35 Posted by: gaetjen Posted at: 2017-10-10T09:16:33.465Z Reads: 550

```
What´s the difference between your "old" 2.54 BLDC version and your new ESC tool version?
```

---
## \#36 Posted by: Vanarian Posted at: 2017-10-10T10:50:43.103Z Reads: 553

```
It is based on 3.xx FW versions instead of older 2.16 modded.

It benefits from Vedder's new FOC algorithm too and adds Ackmaniac's control feature and Bluetooth compatibility.
```

---
## \#37 Posted by: gaetjen Posted at: 2017-10-10T13:10:07.422Z Reads: 554

```
What are the benefits of the new algorithm in comparison to the old one?
```

---
## \#38 Posted by: Vanarian Posted at: 2017-10-10T13:40:00.770Z Reads: 556

```
Better power management, which means a better overall torque/power, a better control, more reliability due to this and less fried DRVs issues (less spikes, better motor sync I think). You manage also more range.
```

---
## \#39 Posted by: emmaanuel Posted at: 2017-10-10T23:08:11.362Z Reads: 554

```
Maybe a stupid question (or maybe I misunderstood something) , but why did you fork the 3.x VESC FW ? It wasn't possible to contribute directly in the VESC projet ? I saw others guys in this forum having pull request accepted in the VESC Project. Better to work all together, no ?

You are doing a great job and you do have very good ideas, but this fork you'll make the support of this FW version harder for mobile application like "eskate VESC for iOS".
```

---
## \#40 Posted by: Deckoz Posted at: 2017-10-10T23:26:32.384Z Reads: 566

```
That's pretty inaccurate.

You see vedder hasn't always merged ack's PRs. But ack has always pulled in the bug fixes to his builds... Acks firmware has always been a little more "complete" and geared toward esk8. Vedder is covering all forms of use cases with the vesc tool.

As well regarding supported iOS/android apps..lol you realize you still need Bluetooth and no one ever changes the UART telemetry right?
```

---
## \#41 Posted by: Michael319 Posted at: 2017-10-11T00:23:13.877Z Reads: 533

```
This is kind of crazy. @Ackmaniac and vedder thank you so much, this is awesome. On previous hw 2.54 I wouldn't pull anywhere near 20A on my pack, now I pull a lot more amps and have insanely more torque on foc. (all of the settings are the same.)
```

---
## \#42 Posted by: emmaanuel Posted at: 2017-10-11T07:21:23.408Z Reads: 527

```

I understand your first point, but this seems to have change with the new version v3.x. There is many contributor in the VESC FW project.

What's wrong with BT and UART telemetry on the "official" FW ?
```

---
## \#43 Posted by: MontPierre Posted at: 2017-10-11T07:37:49.610Z Reads: 516

```
@Ackmaniac any chance to add a tab in the ESC Tool where you can name and save settings? It will be useful to quickly change between “weak” and “powerful “ settings with one click. Currently I can export settings to file but built in button would be much easier. Thanks !
```

---
## \#44 Posted by: Vanarian Posted at: 2017-10-11T10:52:51.748Z Reads: 497

```
@Ackmaniac Any chance that you'll release FW file directories?
```

---
## \#45 Posted by: DanSkates Posted at: 2017-10-11T12:14:16.361Z Reads: 504

```
Hi guys, I really don't want to clutter this beautiful thread but I think I may have just screwed up the firmware update and could really do with some help.  I have a slightly older FOCBOX - V1.3 on the board, have just downloaded the new Extended Ackmaniac-ESC Tool (which looks glorious btw) tried to install the new firmware; I selected 410 & 411 & 412 but it hung on 99.7% and I got the spinning wheel timer on my mac which stayed on for the last 20 mins so I disconnected the FOCBOX and now I don't get the 3 flashing lights on start up (it pauses then just goes to solid green) and it won't connect.  Have a ruined my FOCBOX?  Is there a way back from here?  Happy to set this up as a new topic to not distract from the awesome content on here :sweat: just let me know.

Any help would be hugely appreciated - hopefully any response will help others avoid doing the same, or help resolve the issue.

Thanks guys,

Dan
```

---
## \#46 Posted by: Ackmaniac Posted at: 2017-10-11T12:17:28.841Z Reads: 504

```
I changed many things in the PPM and Nunchuk (NRF) handling. Also the way acceleration and power is handled is different to the original version. Also the Timeout ramping handling needs a lot of changes.

But i realized that it would take forever that my ideas would find it's place in the original. And i simply don't have the time to wait for months and discuss everything to death before something happens. I am more interested in development and finding solutions.
Also Benjamin don't seem to be active on the project in the last couple of weeks (of course i could be wrong here). Also my questions in the VESC-Project forum were never answered by him. 

And the biggest problem are the changes that are needed that all the features of my app work. And i am pretty sure Benjamin isn't interested to implement that stuff only for my app.

Sadly i had to give the tool it's own name because of the Trademark policy's. I would have preferred that it is clearly visible that it is only a extension.

Long story short. I do this for fun and not for business. And to discuss and fight for every little change is no fun for me.
```

---
## \#47 Posted by: Ackmaniac Posted at: 2017-10-11T12:19:00.195Z Reads: 471

```
Just unplug the USB cable, stop the ACKMANIAC-ESC tool and switch off the VESC. Then connect and start everything again. With the new firmware the FOCBOX won't flash 3 times anymore on startup (same as official version)
```

---
## \#48 Posted by: DanSkates Posted at: 2017-10-11T12:30:03.873Z Reads: 464

```
Ok, that's reassuring - hadn't realised that and assumed there was an issue.  The mac version keeps hanging with the spinning wheel but the PC version (cheekily just installed it on my work asset -shhhhh) seems to have picked it back up again showing version 3.100 is installed - am I back in the game?  I guess it would be unresponsive until I set up it again right??  Thanks for the immediate response - you're a legend and I'll be sure to hit the donate button once I get her spinning :blush:
```

---
## \#49 Posted by: Deckoz Posted at: 2017-10-11T12:55:25.112Z Reads: 471

```
Nothings wrong with the telemetry, I'm simply stating your reasoning that other apps will be harder to support is wrong, because none of the Devs have changed the outward packets data set. Only the inward packets for firmware configuration. 
You realize all the 2.xx firmware variations can work with all the phone appa, same thing with all the 3.2x versions, its because there's no value in changing the telemetry data set on the firmware variations...  If you don't do code, let me rephrase it. We have a book called vesc, with a chapter called telemetry. A dev may change the cover of the book or other chapters, but the telemetry stays the same, the words don't change, and the language/formatting doesn't change, so all the apps can still "read" it
```

---
## \#51 Posted by: Ackmaniac Posted at: 2017-10-11T16:25:48.944Z Reads: 480

```
https://www.youtube.com/watch?v=FONN-0uoTHI
Available at BLDC-TOOl and Firmware\ackmaniac-firmware_3_100.zip
```

---
## \#53 Posted by: Pimousse Posted at: 2017-10-11T16:53:56.615Z Reads: 464

```
Amen.
To be honest, I gave up since a while now collaborating with this project.
And I'm really sad. After so many hours spent testing, reporting bugs and more (remember the VESC 6 protocol), and never got any consideration for my requests, I'm figuring out that I wasted a lot of (precious) time. :(
Anyway, as always said and as @Vanarian tells very well : your skills are amazing though.
```

---
## \#54 Posted by: emmaanuel Posted at: 2017-10-11T17:05:20.791Z Reads: 474

```
:slight_smile:
@Deckoz  My turn to say you: it's pretty inacurate.

I'm the autor of the iOS eSkate VESC app:
[http://www.electric-skateboard.builders/t/new-version-2-0-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340](http://www.electric-skateboard.builders/t/new-version-2-0-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340)

I can confirm you, that all the latest version (2.18, 2.54, 3.27) did modify the command interface. And I have specific code for each of this version.

For this reason I'm complaining about seeing a new fork of the FW, because it make our work more difficult. And for the users all this version stream make it difficult to understand and diagnostic compatibility problems.

I can perfectly understand Nicola's answer, and we are all working on that for fun and not for money. 
You know it's easier to work alone than together, but has the proverb say: 
> If you want to go fast, go alone. If you want to go far, go together

Maybe a good solution for everybody, would be to put the ackmaniac extension on Github has a fork of the VESC Project (there are already a lot of fork of the vesc project). This will: 
* permit to Nicolas to keep the freedom of making the choice he want, without loosing time in discussion.
* make easier to follow the modification for the apps developper, like @rpasichnyk and @emmaanuel 
* Clarify the perimeter of the modification done by Nicolas versus the code from Benjamin project
* allow to merge into the VESC project all the good ideas from Nicolas
* allow to keep ackmaniac up to date about all the good ideas from the VESC Project.
```

---
## \#55 Posted by: Deckoz Posted at: 2017-10-11T20:53:10.462Z Reads: 447

```
The command interface is different then the telemetry data set. 

The data set in all 2.x firmwares is the same. The 3.2x firmware data structure is slightly different but not likely to be modified further.

Executing commands over the UART interface is different then the telemetry packet.
```

---
## \#56 Posted by: emmaanuel Posted at: 2017-10-12T02:37:34.929Z Reads: 437

```
Usually I would have let let the discussion here, but it’s‘not accurate...
Even in 2.x the voltage scale has been modified in the ackmaniac 2.54, but you look pretty sure nothing has change... so it’s ok for me but it’s false.... 
so nothing has change and all my code has been added for nothing. It’s easy to tell us what we have to do without realy knowledge about the firmware modification... like Nicolas i’m Stopping to speak about this subject, I’m not going to support this fork anymore until the version are clear enough.
```

---
## \#57 Posted by: trampa Posted at: 2017-10-12T09:59:41.475Z Reads: 456

```
Hi everyone! We will ad an "Ethos" page soon and will provide a section in the VESC-Forum about the VESC-Project itself. This non so much tech related but rather a room to debate the Project itself. 

We will ad a structure to enter feature requests, so that they can be worked in.
This will be a e.g. a table where you can drop in the feature and post a link for further explanation. 
We will then drop the request into a fixed ToDo list that is worked down by priority. Sometimes A needs to be solved before B

The last 6 weeks were very busy and in consequence not everyone got the answers they wanted.
VESC-Tool is just public for a short time now, so don't be to demanding.
We had the summer vacations, a surgery to extract some Titanium, work on the website, 3 x FW revision etc.
Please don't forget that you are many while Benjamin is a single person and he has a full time job at this stage.
We want to encourage other experienced users to help out as well, and keep an eye on posts from others.

This is the way forward: 

If you write code for the VESC-Project:
1. Once the structure is online, drop your request there.
2. ad your user name, so everyone knows who you are. 
3. make a pull request and submit code

If you don't write Code:
1. Once the structure is online, drop your demand there.
2. ad your user name, so everyone knows who you are.
3. Write a post about the feature for further explanation and link this post in the feature list.

**To make it very clear:** Benjamin doesn't like to see those forks for many reasons.

The VESC-Project is a terrible amount of work and VESC-Tool took almost two years to code.
This was only possible with a lot of work after work and a hell of patience.
Like a business, the project has costs to shoulder (e.g. a new server is being installed right now, a high speed glass fibre connection was installed and has a monthly bill, travel expenses, advice, accountant, prototypes, computers etc.)
So far no money went into "paying Ben for the countless hours he banged on stuff" but rather lowering the base cost.
Please note that a fork with some new features still is 99.5% of Benjamin's code and is only possible because he supplied the code under the GPL V3. 

The VESC-Project has the doors wide open as an invitation to work together on a strong single version.
A website has been created to give the project a home. If possible, the door should be used to step in.

To write code that interacts seamless with another you need to know what comes next and which dependencies exist.
This is a very good reason to work together on one version, rather than splitting things apart. 
Forks drift versions apart and therefore create incompatibilities in future. This is either wanted by the fork to create a USPs and divert users to the own fork, or it happens without purpose. 
**Both is not good for the community and the project itself.**

Frank
```

---
## \#58 Posted by: Silverline Posted at: 2017-10-12T10:31:01.540Z Reads: 418

```
To me Benjamin seems pretty 'off the grid' . The vesc-project forum is pretty dead, and Benjamin is not answering many quistions in there. I still find it pretty funny that he is not on the World greatest Esk8 forum. Thats why i like the work Acmaniac is doing in here. He is pretty active, and help a lot when people have quistions. 
And i find it a little bit funny to, that FOC on Focbox is working on his 'forkd version' but still not in the official version. And i like to run FOC. And since nobody seems to know what's is going on in Benjamins head, and any ETA's. I can't wait anymore. I want FOC now 😃

If you want people to use your stuff, you have to be where people are.
```

---
## \#59 Posted by: notger Posted at: 2017-10-12T10:45:32.932Z Reads: 425

```
 @Silverline I wanna echo that.

Sure, Frank i understand what you say about problems of forking.
Still i'm very thankful to @Ackmaniac that he is not as patient as we should be....
and skilled enough to just implement what he wants from a firmware and software.

So actually i do not think that this will get a totally separate fork, @Ackmaniac is just faster in implementing users wishes (or probably his own).

And sure I'm at least aware that VESC-Tool is made by Benjamin and thanks man thats awsome.
But what's the Problem if someone (@Ackmaniac) is developing it further ?  (and that in enormous speed, where do you take all that time Nico ?)

@trampa have you tried @Ackmaniac's Soft/Firmware ? 
If you use ppm, Focbox, Dual-Setup and want FOC, Cruise-Control,.... this Soft/Firmware here is the only choice. Same is valid for the old BLDC-Tool people who had hope that Benjamin would implement new features would have been dissapointed, thanks to Ackamaniac that he went on .

So, peace People
And i also hope that this will get a community Project once, but till then you freay programmers, please keep on developing stuff like you want and think it's the best.
```

---
## \#60 Posted by: linsus Posted at: 2017-10-12T11:39:32.336Z Reads: 419

```
Theres a good reason Ben isnt in alot of forums.

From the start Ben answerd alot of questions if not all. But eventually, answering questions started taking up hours. Even days. For awhile he had hundreds of emails per day to answer. Simply wasn't sustainable. Therefor he chooses to spend most of his day working with his project instead. To bring people like you and me, Amazing hardware and software. 

Alot of people dont know this, but the hardware isnt very unique. The software Ben wrote however, is very sophisticated and has been approached by many companies in order to lock future developments down. Ben has turned down every offer because he belives that the project should be avaible to everyone. So in my personal opinion, donating to anyone but Ben is an absolute insult with the years of work he has put in. If others want to help develop and improve. Thats fine. But it has to be done in a good way, making a separate verision that is based on 95% of the original code is not the way to do this. Especially not on new releases. 

If Frank can provide a bridge between Ben and others in a sufficient way, it would be very dumb to not consider it. After all, we all just want to ride some boards. Don't we?.
```

---
## \#61 Posted by: MontPierre Posted at: 2017-10-12T12:08:18.454Z Reads: 401

```
Well I agree with @linsus and @notger ! Both posts are valid in their own ways.... I would love to have Benjamin implement @Ackmaniac fixes/upgrades/ideas in firmware and Vesc Tool. I totally understand that it takes a lot of time for Benjamin, and it’s har to catch up having full time job, for this reason a lot of us go with @Ackmaniac versions of Tool and Firmware at it comes out quicker and has the features we all want to have. Perhaps somewhere in near future Benjamin can add those features to his work, but since it will take a lot of time we will enjoy @Ackmaniac work. 

@linsus is right - we all should do our best to donate to Benjamin and it honesty most of the code is his.
```

---
## \#62 Posted by: Pimousse Posted at: 2017-10-12T12:12:25.355Z Reads: 411

```
You only look at the emerged part of the iceberg.
If Benjamin had to answer every email, every forum post, every whatever, you would still be waiting for a lonnnng time before enjoying FOC. ;)
Adding a new feature by a pull request is as simply as clicking on a button.
Instead, dealing with dropbox folders (when sources are available) is a pain and consumes time and... wait... oh shit, no more time to answer questions. :slight_smile:  Endless loop.

Forking the project like still kills the Open Source spirit IMO.
(my 2 pennys)
```

---
## \#63 Posted by: longhairedboy Posted at: 2017-10-12T12:44:48.765Z Reads: 404

```
I heard i mentioned before.. but it keeps just getting glossed over so i'm going to mention it again. 

BLDC-Tool is is great. VESC is amazing. It was designed to be a motor controller for esk8s but it has turned into a motor controller for Every Goddamned Thing including Sumo Bots and Power Wheels races. Which is awesome. 

But While BLDC Tool and the vanilla firmware is accommodating Every Goddamned Thing, Ackmaniac's is trying to specifically accomodate esk8s with the needs we have right now specifically for esk8s. 

Not to take anything from Ben or Trampa or anyone else working thier asses off on this, but that is precisely the kind of thing that causes forking and its not like we didn't all see it coming.
```

---
## \#64 Posted by: mmaner Posted at: 2017-10-12T13:04:07.492Z Reads: 386

```
[quote="longhairedboy, post:63, topic:35116"]
Ackmaniac's is trying to specifically accomodate esk8s with the needs we have right now specifically for esk8s. 

Not to take anything from Ben or Trampa or anyone else working thier asses off on this, but that is precisely the kind of thing that causes forking and its not like we didn't all see it coming.
[/quote]

Preach brotha, preach
```

---
## \#65 Posted by: trampa Posted at: 2017-10-12T14:08:47.358Z Reads: 409

```
As you may have noticed, the old Server has issues and needs to be replaced with a new one. That takes time...

Simultaneously there needs to be structure set up for the community to interact in a structured way.
You need to consider that VESC-Tool is set up in a very structured way, so that changes can be made faster.
The goal is to implement updates faster and allow developers to better understand the code base.
In consequence code contributions can be implemented faster.
This was done to allow more contributions, not to fork faster.

I talked to many people with code skills in person earlier this year and asked them to join in and work closer to the project or help out once the project is live. Instead of that we see the current situation, where Benjamin does tons of coding (two years of hard work) for the good of the community to see a forked version just months after the release. 

In the end a day has 24 hours and code contributions need to be reviewed and changed to fit in perfectly. That is a process taking some time. The benefit is a better code base in the end and more compatibility, a consistent documentation and many more.

We are just 2 months away from the release! Priority A is improving the server, set up a structure for contributions and **bang on hardware releases** while adding in new features for the VESC-Tool simultaneously. Give it some time! Rome wasn't build in a day. Now we face the situation that Benjamin will need to implement the features you are so desperate for, instead of finishing the public hardware release. 
It can't be done all at once. But it will happen faster if more people are willing to contribute rather than shooting ahead with their own versions and ideas. In the end users want a version with all the features available they dream of. They want the hardware and code. But it all needs to fit together, code wise and time wise.

Imagine there is a completely new way to manage the power distribution, a lot more user specific and convenient to deal with. In consequence it would make sense to implement that over the modes that we know already. Unfortunately this would affect many sections in the app settings, like throttle curves, timout ramping etc. In consequence you bang on that new mode first and adapt the other settings later.  A, B, C >> clean result

Such things can be implemented faster if everyone knows how to approach this, know A and B and C and skills are coordinated to achieve it. Currently Benjamin bangs on stuff like that and will implement it and Nico has to start all over again and adapt his fork to the new code and in consequence he has tons of work that he could have invested more efficiently if he worked on the original code base in the first place. 

The current situation also makes it less likely that Benjamin will publish his coding schedule, since he would need to fear that forks will try to implement things faster to stitch him out. That is not good for the community and and collaborative approach we all envision.  

OS-Projects live from collaboration and not from coexistence. 

Frank
```

---
## \#66 Posted by: Pimousse Posted at: 2017-10-12T14:14:44.310Z Reads: 366

```
(Are you sure I'm the target of your reply ?)
```

---
## \#67 Posted by: trampa Posted at: 2017-10-12T14:25:37.171Z Reads: 368

```
Sorry, no you are not, there is no target. I just want to explain how things are.
```

---
## \#68 Posted by: mmaner Posted at: 2017-10-12T14:31:13.811Z Reads: 394

```
Im just gonna say this...In large projects, forks happen, there's nothing you can do about it unless you move from open-source.  It may not be palatable to you but its a fact of life.  I would further suggest, this specific fork happened because the original project is not meeting the needs of a lot of people.  

The VESC6 is too far reaching, trying to use the same hardware and software for multiple platforms is unlikely to be successful, there are many examples of this, 1 of which is the COMTEL LCD extravaganza of the early 2000's.  COMTEL bought 9 of the 12 manufacturing facilities in the world that made LCD's.  That left COMTEL and Samsung as the only manufacturers.  COMTEL then reduced the form factors from hundreds of options to 5, the login being manufacturers will buy what we choose to sell.  In the end Samsung made billions and COMTEL went bankrupt, because they kept making 100's of different form factors.

[quote="trampa, post:57, topic:35116"]
The last 6 weeks were very busy and in consequence not everyone got the answers they wanted.
[/quote]
[quote="trampa, post:65, topic:35116"]
the old Server has issues and needs to be replaced with a new one. That takes time...
[/quote]

This has been a constant for this project, specifically the VESC6.  Seems like time management is the real problem you guys are having.  Maybe focus on getting a reliable product to market, the worry about all the "moves-adds-changes".

[quote="trampa, post:57, topic:35116"]
Both is not good for the community and the project itself.
[/quote]

I totally disagree.  I don't think the VESC6 has been to terribly good for the community, at least I havent seen it make any huge advance in available options.  I personally cant do anything with a VESC6 that I cant do with a FOCBox/TB Vesc.  The @Ackmaniac firmware has definitely been a help to thousands of users.
```

---
## \#69 Posted by: notger Posted at: 2017-10-12T14:33:46.392Z Reads: 374

```
Sorry i really don't get it.

Is Benjamin or you Doubting that Nico does his work in a good way, or why are you not just thankful and happy that great work has been done by him.
Probably it has something to do with "Coders-Pride" who did what first, and who did it cleaner.
I don know how @Ackmaniac is looking at it. But Ben could just take Nicos changes, look over them change them if needed and add them to his "Vesc-Tool".

And where is the Open-Source-Spirit if one Person in this case Ben or You? have to "bless" what other people want to have in addition.
```

---
## \#70 Posted by: longhairedboy Posted at: 2017-10-12T14:36:15.506Z Reads: 367

```
It must be terribly difficult trying to balance all of that out, and i can understand the frustration. 

And at this point we're dealing with a process similar to evolution, and the first most organized species out of the sludge may or may not be the survivor of that system. That also has to be frustrating, potentially infuriating. Like when a co-worker steals your spreadsheet and adds a few macros and makes the boss happy. The good news is that the work is done and everyone in the cubicle farm knows who did it. The bad news is that the boss doesn't care who hands it in and has zero loyalty to anything other than his own immediate interest. In this situation, the overall esk8 community is the boss, and they don't care who shows up with the best firmware or where it came from or who's blood and sweat went into it. 

Darwinian competition is ruthless and cold, but it is a very predictable animal. But you know all of this already.
```

---
## \#71 Posted by: trampa Posted at: 2017-10-12T14:56:05.191Z Reads: 359

```
I would say its best if everyone pulls on one side of the string for the good of the community and get things nailed in a structured way. The code base will be better on the long run and the spirit of OS is not Darwinian competition but collaboration. A group of coders all piss in one pot to combine their output to something with volume. 

Frank
```

---
## \#72 Posted by: notger Posted at: 2017-10-12T15:05:58.634Z Reads: 374

```
[quote="trampa, post:71, topic:35116"]
I would say its best if everyone pulls on one side of the string for the good of the community and get things nailed in a structured way. The code base will be better on the long run and the spirit of OS is not Darwinian competition but collaboration. A group of coders all piss in one pot to combine their output to something with volume.
[/quote]

**Sounds Great in theory**

[quote="Ackmaniac, post:46, topic:35116"]
But i realized that it would take forever that my ideas would find it's place in the original. And i simply don't have the time to wait for months and discuss everything to death before something happens. I am more interested in development and finding solutions.
Also Benjamin don't seem to be active on the project in the last couple of weeks (of course i could be wrong here). Also my questions in the VESC-Project forum were never answered by him. 

And the biggest problem are the changes that are needed that all the features of my app work. And i am pretty sure Benjamin isn't interested to implement that stuff only for my app.

**Sadly i had to give the tool it's own name because of the Trademark policy's. I would have preferred that it is clearly visible that it is only a extension.**
[/quote]
```

---
## \#73 Posted by: Pimousse Posted at: 2017-10-12T16:33:40.402Z Reads: 343

```
Please, stop to argue with TM.
Sounds like the Godwin point reached by the old uncle during a sunday family's lunch... :smile:
```

---
## \#74 Posted by: rpasichnyk Posted at: 2017-10-12T18:44:57.496Z Reads: 361

```
@trampa forking is good. Forking is amazing. Developers like it. A lot of open source projects have "Fork me on GitHub" ribbon on the website, this is a good thing! Truth is you can not submit a pull request without doing a fork first. Forking does not mean "not working together".

@Ackmaniac whether you prefer to contribute upstream or not is totally up to you. I can understand if you were dissapointed by one of your pull request being rejected. This happens sometimes. Doesn't mean it's your fault. There can actually be other people who have time to take your code and create a pull request. Or this can be Benjamin himself. One thing that sucks though is that you did not want to share the code despite GPL license. It took multiple attempts and a rant from @Vanarian (thanks, man!) to make this happen, but the attitude is clear. We have been presented with a zip file. It's like spit-in-the-face way of sharing (from the software engineer point of view). Technically this is OK, but doesn't feel good.

My advice would be to put the code on GitHub, make a quick pull request and then walk away with clean hands. I wouldn't stress to much if it gets accepted or not. Other people might be willing to tweak it and shape it until the point it gets in. And you will avoid ranting ;)

Thank you for implementing new features, I am happy to see people excited about them! That's the most important thing after all! :heart:
```

---
## \#75 Posted by: Achmed20 Posted at: 2017-10-12T20:06:57.602Z Reads: 352

```
[quote="rpasichnyk, post:74, topic:35116"]
@trampa forking is good. Forking is amazing. Developers like it. A lot of open source projects have "Fork me on GitHub" ribbon on the website, this is a good thing! **Truth is you can not submit a pull request without doing a fork first.** Forking does not mean "not working together".
[/quote]
nah, thats what branches are for.

technicaly a fork a spearation of the original project which is agoing a different path.
i do understand why they dont like forks, since forks make it pretty hard to be merged again in a later state.

however, if you have many contributors to a project, this usualy also requires a lot of work or "trust". if its a open source project and you planed a specific way allready, then managing those can be rather chalanging. 

i do get why they might be pissed about a fork, but if they dont have documented guidlines and the capacity to manage incoming pull request, then a fork is the natural way.
```

---
## \#76 Posted by: trampa Posted at: 2017-10-12T20:35:06.169Z Reads: 335

```
Sure you need to do a git branch to make pull request, but then the developer can see all changes and the difference in code with ease. The drop box folder we see has no .git folder which makes it hard to see all the changes that have been made. Anyone interested in sharing and enhancing the code should not set hurdles to others. 
Currently there is a "blanket" over the code changes that can only be lifted with a lot of additional effort.
So that is what @rpasichnyk refers to when he says "spit-in-the-face" 

Benjamin can implement stuff without the need of the source, but others might want to look what the difference in code is without the need to manually compare code pages. 

Anyone interested in working on the VESC-Tool anf FW code should use github!

Frank
```

---
## \#77 Posted by: SeanHacker Posted at: 2017-10-12T20:52:17.275Z Reads: 328

```
@trampa 

Have you guys thought about setting up a gerrit instance? Its a great way to include everyone in on code contribution.
```

---
## \#78 Posted by: E-Boarding Posted at: 2017-10-12T21:04:28.283Z Reads: 333

```
I don't like forks, this can get very messy and cause incompatibilities in the future but

Ben and Ack are heading in different directions, a great idealic VESC-Tool that doesn't solve the problems of the esk8-people isn't very helpfull and I see no way Ben is adding all the esk8-specific features in his software ever, this is not the way he wants to go. Even the VESC6 is overkill for esk8 imho, you can do about the same things with a smaller Focbox.

I think a good esk8-fork of the great VESC-do-everything-software(and hardware) is inevitable to get best results for the esk8-communty.

Everyone should Donate Ben and Ack ;)
```

---
## \#79 Posted by: trampa Posted at: 2017-10-12T21:04:57.003Z Reads: 344

```
[quote="SeanHacker, post:77, topic:35116"]
gerrit instance
[/quote]

I will have a look at it . THX for the hint!. As soon as the new server is running tonight, I will ad a "VESC-Project" section to the forum to debate stuff like that. 

Frank
```

---
## \#80 Posted by: Vanarian Posted at: 2017-10-12T21:19:17.417Z Reads: 377

```
How does one make a pull request ? Genuine noob question here. 

@Pimousse @rpasichnyk thank you for your understanding guys. I'm less angry tonight, my head cooled down haha maybe a good time to compile those sources :wink: 

@ackmaniac definitely produces quality work on this project and it must have taken lot of time. Apart from the time & discussion it takes to add a feature, I can understand why Ben might be uptight to add something totally different though.

I mean : it's his baby. It is O-S and he's been at it during his free time for few years now. Realize the sacrifice. Give him some space to breathe, he has his own schedule to make the project grow, specially since it went from "esk8" target to "everywhere".

Anyway here is a proposition which should have been done already ?

- Make an official pull request of the mods
- Fork it too so current code is accessible while waiting for everything to be merged

Ben can easily follow development this way and we still get early access to the new working features while he focuses on his job.
```

---
## \#81 Posted by: Titoxd10001 Posted at: 2017-10-13T01:52:19.098Z Reads: 353

```
FOC works on Focbox with your firmware. TY @Ackmaniac
```

---
## \#82 Posted by: Ackmaniac Posted at: 2017-10-13T02:58:41.740Z Reads: 369

```
You're welcome.
```

---
## \#83 Posted by: CamBo Posted at: 2017-10-13T04:19:11.772Z Reads: 373

```
Using @Ackmaniac's flavor of Vedder's software is the single best improvement I have made to my esk8s.  I applaud both Ben and Nico as my equipment wouldn't be the same without their cumulative contributions.  I owe you both.  

I hope that in the spirit of Open Source, more time is spent focused on development, and less on a quest for control.  

I appreciate that this is job for Ben and a hobby Nico.  

I think there may be a lot of us that are buying from Trampa as a way to support Ben at his new job.  In doing this we have a high expectation of his/Trampa's work.  We are buying a finished product, and I think Trampa's products are pretty polished. As such I spent $$$ on an Urban carver.  

However, I fully admit that I would not have spent any $$$ with Trampa (or anyone else)  if it weren't for Nico's software and his presence on the forum. He answered my noob questions and added software features when I asked him for help.  Pretty amazing service from him as a random stranger on the internet.  I owe you man.

So I hope that Ben and Trampa can keep an open mind about @Ackmaniac's fork.  In my case, it helped them sell an Urban carver and future Vesc's. 

And somehow @Ackmaniac has been stuck doing their customer service for free.   (In my case anyway)
```

---
## \#84 Posted by: linsus Posted at: 2017-10-13T08:48:34.315Z Reads: 366

```
I know ben personally and I have to say hes one of the brightest and most humble persons I've ever met. I understand your reasoning around the "baby" scenario. But frankly I'm sure Ben would be positive to the idea to get more developers involved. Aslong as it does not potentially harm the project in the future. Cause who will be misscredited if not Ben when someones VESC blows up due to software collisions etc? (I know its the users own fault but the avrage guy wont see it that way)

And as some has already mentioned, this is his sparetime project. He has a fulltime job and working on his Ph.d. in parallell to this so hearing everyones opinions and doing quick changes is something that hasn't been possible for him. Breaking his leg in combination to the release of the new VESC didn't improve the situation either. 
I also know from Ben that he has felt discourages to continue working with the VESC several times cause there are so many factors sucking the fun out from what he loves with this project. Lets not let this add to that pile.

I'm all for people like ackamaniac implementing changes and investing thier own time to push the project forward. But I really think it is important to implement this in a good way. I really think breaching that gap is something frank can help with.
```

---
## \#85 Posted by: Ackmaniac Posted at: 2017-10-13T14:50:34.560Z Reads: 344

```
Found a issue with the timeout behavior for PPM for dual drives. Have to investigate that further. So for the moment please don't set a Failsafe signal above the max or below the min value. Will let you know when i fixed the issue. Everything else is working fine.
```

---
## \#86 Posted by: rolexbene Posted at: 2017-10-14T15:21:07.379Z Reads: 346

```
Amazing work @Ackmaniac, been running your old BLDC tool with your android app, and it great to keep track of board stats and change config on the fly.

I have just updated to this new tool and setup in FOC for the first time, running sweet!

My only problem is that the Android app has now stopped working, I updated the firmware to the default from the app (FW3.1, HW410).

Is there something I am missing or does the new firmware just not work with the current Android app?
```

---
## \#87 Posted by: Michael319 Posted at: 2017-10-14T17:39:41.741Z Reads: 342

```
Did you go into uart settings and change the baud?
```

---
## \#88 Posted by: Ackmaniac Posted at: 2017-10-14T18:49:53.779Z Reads: 347

```
You have to use PPM and UART as controller mode and Set a baudrate of 9600. And of course you need the latest Version of the app.
```

---
## \#89 Posted by: rolexbene Posted at: 2017-10-14T19:52:15.859Z Reads: 359

```
Ah ok, that seems obvious now :sob:

Just went for another spin on FOC on my FOCBOX setup, and the board seems to be having a few issues, that nearly took me out. It seems to happen at random but throttle / brake getting stuck on full for like a second, seems like some kind of time out. Also on other occasions vesc seemed to lose connection, like it was resetting. Plugged it into computer when I got home, but no errors??? I know its a bit vague, but any ideas? think I might have to put it back into BLDC on the VESC-tool and test.

On a side note, this only started since the battery has gone down to about 30%, could this be a voltage sag issue??
```

---
## \#90 Posted by: L3chef Posted at: 2017-10-14T20:32:38.006Z Reads: 339

```
Had to look up the word "forking" since I didn't understand it's meaning..I wont post the definition here. But damn.. I never thought you could have so much fun over at github :smile:
```

---
## \#91 Posted by: GrecoMan Posted at: 2017-10-14T20:44:11.374Z Reads: 346

```
lol.

quite the definition...
```

---
## \#93 Posted by: Ackmaniac Posted at: 2017-10-14T21:22:43.913Z Reads: 370

```
**Please update to the new file.** (OSX version isn't updated yet, will add it when available)

I just worked the last 2 days on the timeout ramping for PPM. And now it is working like it should. I highly recommend to update to the latest file i released in my dropbox link. The name is the same but the firmware files which are included are different. Also the Version is still the same (3.100)

If 3.100 is already installed you can update easily by connecting to your ESC, read the settings of the app and the motor and then flash it with the new firmware. After the flash connect to the ESC and directly write the settings which you have read previously. This is possible because the parameters did not change. Do **not** close the ACKMANIAC-ESC Tool in between. If you have a slave repeat the steps for it.

When you think that you have correctly adjusted the timeout parameters (instructions in the first post) you can test it by spinning the motors with the remote and simply switch off the remote. Now the ESC. should start to brake. When this works then you can test it at slow speed when you stand on the board. Simply switch off the remote and you should feel that the ESC smoothly ramps to the adjusted brake current.

I have the settings like in the picture below.
<img src="/uploads/db1493/original/3X/5/7/571a801f1e3058b8d9ab8c9e25ced938ef11f314.png" width="690" height="307">
```

---
## \#94 Posted by: jmasta Posted at: 2017-10-14T22:36:10.057Z Reads: 367

```
[quote="Ackmaniac, post:93, topic:35116"]
The name is the same but the firmware files which are included are different. Also the Version is still the same (3.100)
[/quote]

Appreciate all your hard work!  I have to ask though... What's the advantage of not updating the version number to, say, 3.101 to reflect the revisions?

Reminds me of when the current ramp step bug was discovered, and Ben Vedder fixed it but kept the firmware at 2.18, making it impossible to tell if you had the bugged version without loading it
```

---
## \#95 Posted by: RiGo Posted at: 2017-10-15T05:37:57.361Z Reads: 363

```
[quote="Ackmaniac, post:1, topic:35116"]
Watts Limit usage

IMPORTANT you have to do this for each motor individually, Master and Slave.
[/quote]

Is this still applicable to dual VESC setups connected via CAN? I'm hoping if they're connected via CAN the update happens to both VESCs automatically, no?
```

---
## \#96 Posted by: Ackmaniac Posted at: 2017-10-16T10:33:43.806Z Reads: 355

```
When you update the parameters via the ESC-Tool then no. So you need to setup each motor individually.
When you do the update via my app then all motors which are connected by can (and send their status) are updated.
```

---
## \#97 Posted by: Ackmaniac Posted at: 2017-10-16T10:48:29.809Z Reads: 377

```
Just made some tests with the timeout behavior for PPM and with my Mini remote i set the Timeout to **100 ms**.
By this the ESC reacts very fast if a timeout happens and slowly ramps down. If you let this at 1000 ms (default) the ESC will continue for at least 1 Second with the last command. If this was full throttle there is a good chance that the board will throw you off. 

Sadly the timeout happens most of the time in such a situation. And here is why:
To my experience the reason for a timeout with a PPM remote is mostly a broken antenna on the receiver. This happens during assembling or when we make maintenance in our battery enclosure. Because that cable is always in the way.

So when it is already broken then it sometimes has contact and when it moves a little then not anymore. Or with higher amps comes more interference and that causes the connection loss.
So long story short. It mostly happens when we don't need it (strong acceleration or braking).
And in these situations it is a very high chance for a crash if the board looses the power immediately or if it continues to do full throttle or brake while we released the trigger already. People who had these problems already know what i am talking about.

So with the mini remote i set the timeout to 100 ms so that the trigger doesn't stay at full throttle and reacts really fast.

Please only do this with this firmware and with the latest version. And read the instructions in the first post and test it that the timeout really works with the **correct Failsafe signal**. Please only use a Timeout Brake current if you really understand everything and tested it properly. 
If you don't understand it or your not sure that you set it up correctly then leave it at 0.00 A.

I know that it is a bit complicated but i saw people crash badly because of connection losses. When it is setup correct it is a great safety feature.
```

---
## \#98 Posted by: onepunchboard Posted at: 2017-10-17T07:58:13.201Z Reads: 346

```
quesrion on brake.
i always been able to set higher amp on brake than acc of motor? whts the change on ur fmw? @Ackmaniac
```

---
## \#99 Posted by: Ackmaniac Posted at: 2017-10-17T08:09:38.719Z Reads: 355

```
Yes you are able to set that but it has no effect. Braking was limited by the max amp parameter. So brakes could be weaker or equal but not stronger.
Had to find that out the hard way when i was testing kids mode downhill.
```

---
## \#100 Posted by: egzplicit Posted at: 2017-10-17T08:10:53.015Z Reads: 379

```
@Ackmaniac what was the problem with focboxes and how come your version fixes it?

Thanks for all the work you’ve done when it comes to firmwares.
```

---
## \#101 Posted by: Ackmaniac Posted at: 2017-10-17T08:17:54.988Z Reads: 379

```
Took me a couple of days and a lot of testing, debugging and analyzing. Some ADC values get initialized incorrect in the first moments the FOCBOX starts (maybe the direct fets are too fast at startup).  After that it works fine.
```

---
## \#102 Posted by: Silverline Posted at: 2017-10-17T16:45:17.607Z Reads: 374

```
Great work on the focbox.
```

---
## \#103 Posted by: DanSkates Posted at: 2017-10-21T12:14:35.425Z Reads: 393

```
Ok - I'm sure I'm gonna get a load of grief for this question but I literally cannot find out how to do it and have hunted for the answer and can't find it.  Oh dear.  Here goes - if anyone could answer this quickly and then delete my message it might save me a heap of embarrassment!! :)  

How the hell do I apply minor changes?  

I've run the wizard and applied my settings - all good, but I wanna increase my Absolute max to 155.0A (I guess this could be any change) and apply it - where's the apply button?  I can only read the current setting :(  I'm sure this is so simple and there's a massive red button somewhere I've overlooked - any help hugely, and humbly accepted :blush:
```

---
## \#104 Posted by: i2oadsweepei2 Posted at: 2017-10-21T12:29:39.310Z Reads: 381

```
I haven't seen the new tool, but isn't there a write button? Also is the window maximized or fit to screen? Just a thought. Some day I'll catch up and try the new tool.
```

---
## \#105 Posted by: DanSkates Posted at: 2017-10-21T12:55:47.827Z Reads: 375

```
Thanks for the reply but there's no 'write' button as such in the new tool. The place that resided before now has an 'anchor' icon for full brake and a 'stop' icon.  Besides the minor glitch I'm having you should check out the new tool it's bloody glorious!! Plus FOC on my FOCBOXs is working like a charm!
```

---
## \#106 Posted by: MontPierre Posted at: 2017-10-21T13:06:04.087Z Reads: 392

```
<img src="/uploads/db1493/original/3X/3/b/3b078429cf30a31dd9e0b1d8a6eafaea7513703e.png" width="89" height="1000">

Just hover over each option to see what they do. 

From top you have
Read Motor conf - 
Read Motor Default conf - 
Write motor conf - This should be used for " Minor changes" or Any changes you make

Read App conf-
Read app Defaul conf
Write App conf - for any minor and All changes

i hope this helps :slight_smile:
```

---
## \#107 Posted by: guyguy Posted at: 2017-10-21T13:36:43.023Z Reads: 373

```
Suggestion: Could we have the ramping times set to 0 by default since your fork is primarily for E-Sk8? It's getting buried in the other thread and isn't obvious when upgrading from 2.xx

Thanks!!!

[quote="JohnnyMeduse, post:81, topic:32268"]
Put this parameter at 0.1 and it should do the trick ... also thanks @Ackmaniac
<img src="/uploads/db1493/original/3X/3/4/347bc69d62a4b52173881533b32dd305e42b0406.png" width="690" height="431">
[/quote]
```

---
## \#108 Posted by: i2oadsweepei2 Posted at: 2017-10-21T16:21:43.878Z Reads: 350

```
I plan to try it out eventually. But everything is working great for me here too. Also running foc on my focbox's. Foc is brilliant on watt control. I'm running out of time though in the great white north so I'll probably wait till spring... maybe :slight_smile:
```

---
## \#109 Posted by: guyguy Posted at: 2017-10-21T17:19:49.502Z Reads: 352

```
Was braking changed in this firmware from the original? 

I've noticed my braking was really soft moving to 3.1 I had to increase my bat min settings to get the same braking behavior from 2.54.
```

---
## \#110 Posted by: DanSkates Posted at: 2017-10-21T21:03:01.777Z Reads: 352

```
Holy crap 💩I knew it had to be obvious!  Thanks @MontPierre 👊🏻
```

---
## \#111 Posted by: MontPierre Posted at: 2017-10-26T19:14:24.975Z Reads: 351

```
@Ackmaniac Is Watt mode supported like in Old BLDC Tool? I couldn’t find watt mode in BLDC tab, just Current. If I was to choose Current with break, and limit Watts in Watt limiting field would it work the same way as previously? Also, is there a way to set up curves for breaks and acceleration separately and independently?
```

---
## \#112 Posted by: Ackmaniac Posted at: 2017-10-26T19:24:22.911Z Reads: 355

```
Current control is in the new firmware the same as watt control in the old firmware. 
And you can adjust different throttle curves for acceleration and braking. But that is now also possible in the official version.
```

---
## \#113 Posted by: BigBoyToys Posted at: 2017-10-26T19:31:34.769Z Reads: 353

```
Are Motor detection and satuaration compensation functions that can be incorporated into your app?
```

---
## \#114 Posted by: Lambjr088 Posted at: 2017-10-30T03:28:57.262Z Reads: 358

```
I don't get it fork or no fork. What @Ackmaniac has done and is doing is awesome for us who want to build esk8. From what I have read frank wants to use ackmaniacs file to add the his vesc6 which he trademarked. I may be wrong but for someone who wants. Contributions for others hard work he sure seems to want it for free.
```

---
## \#115 Posted by: Kaly Posted at: 2017-11-01T23:55:59.452Z Reads: 350

```
@Ackmaniac Great work on this Man 
installed on VESC6 and work like a charm Thx
```

---
## \#116 Posted by: egzplicit Posted at: 2017-11-03T11:49:22.512Z Reads: 343

```
@guyguy from what values to what values have you changed the battery min & motor min to match the previous braking power from older firmware? Is this in FOC or BLDC?

@Jinra also mentioned weaker brakes for same values on 3.x firmware.
```

---
## \#117 Posted by: guyguy Posted at: 2017-11-03T13:29:35.452Z Reads: 335

```
batmin was changed to -20 from -12. I run it in FOC. These values don't change when switching between FOC/BLDC.
```

---
## \#118 Posted by: Ackmaniac Posted at: 2017-11-03T15:34:54.454Z Reads: 327

```
Could it be that you didn't directly switch from 2.54 to 3.100. Because if you used the original 3.27 or 3.28 in between then the braking behavior is different.
```

---
## \#119 Posted by: guyguy Posted at: 2017-11-03T15:51:14.729Z Reads: 324

```
Hey, I went directly from 2.54 to 3.100. I was waiting on your 3.xx FW to come out since I trust your work. 

Could be just me; not sure if anyone else experienced this.
```

---
## \#120 Posted by: egzplicit Posted at: 2017-11-03T17:29:55.044Z Reads: 338

```
Well @Jinra said that he kept the same values when using 3.100 by @Ackmaniac and it worked the same as 2.x but did report weaker brakes in the official 3.2x firmware.

I've so far tried my new build with 2.18 BLDC and this weekend I'll update to 3.100 and switch to FOC (on focboxes). Hope the braking behaviour doesn't change as I'm pretty happy with the brake force (I only run -8A battery min and -36A motor min / vesc but i find my brakes are good).
```

---
## \#121 Posted by: Ackmaniac Posted at: 2017-11-03T17:35:20.108Z Reads: 337

```
Did you maybe accidentally change the brake throtte-curve or might have a wrong min pulsewidth value for your ppm remote? Brakes and acceleration should behave more or less the same as in 2.54.
```

---
## \#122 Posted by: guyguy Posted at: 2017-11-03T17:55:13.759Z Reads: 345

```
Throttle curve was the same. Could be pulse-width; it's probably the only value that was different. I re-detected through the wizard. 

Acceleration definitely felt the same.
```

---
## \#123 Posted by: Titoxd10001 Posted at: 2017-11-04T06:00:10.955Z Reads: 360

```
Not sure if I missed but does this tool have the option to not limit erpm with brakes. Set negative erpm for reverse but it jitters when it reaches the max.
```

---
## \#124 Posted by: Ackmaniac Posted at: 2017-11-04T12:13:11.456Z Reads: 355

```
Because it cuts Power completely when it goes above that erpm. Its better to limit it in the app settings. Or you can try the new Firmware which has only the Motor erpm limit and ramps that smoothly.
```

---
## \#125 Posted by: Maxid Posted at: 2017-11-05T10:21:04.175Z Reads: 354

```
Does anybody know what I can do with a Hi-DPI Display?
ESC-tool looks like this on my new computer:
<img src="/uploads/db1493/original/3X/3/8/380a1dc31a6e82a02070c1a0f0da8369d58f65f0.JPG" width="690" height="373">
```

---
## \#126 Posted by: egzplicit Posted at: 2017-11-05T10:53:32.055Z Reads: 337

```
There is a UI scale option in the last section on the left (ACKMANIAC...)
```

---
## \#127 Posted by: Maxid Posted at: 2017-11-05T11:07:23.523Z Reads: 338

```
thanks - however, even at the smallest value of 1,0 the letters in the left column are still clipped.
The rest is usable though so only a cosmetic issue :thumbsup:
```

---
## \#128 Posted by: Youssless Posted at: 2017-11-05T16:53:53.889Z Reads: 337

```
Hey guys, nooby question,

Scratch that, decided to just go for it and upload the 'VESC_Default.bin' to get V3.100.

So... what's the difference between 3.100 and 3.28?

Thanks,

Youssef
```

---
## \#129 Posted by: bsancken Posted at: 2017-11-05T20:32:39.337Z Reads: 325

```
Right click on the program and go into compatability and launch it in low res. mode
```

---
## \#130 Posted by: briman05 Posted at: 2017-11-07T00:56:21.503Z Reads: 321

```
Will this run on Macs?
```

---
## \#131 Posted by: Jinra Posted at: 2017-11-07T01:02:11.739Z Reads: 327

```
Yes there's an osx version in the folder. However it suffers from the same bug as his old tool where it crashes if the vesc reboots.
```

---
## \#132 Posted by: briman05 Posted at: 2017-11-07T01:02:53.347Z Reads: 327

```
So does that kill the focbox?
```

---
## \#133 Posted by: Jinra Posted at: 2017-11-07T01:05:51.772Z Reads: 339

```
no you just have to force close and reopen the app
```

---
## \#134 Posted by: zepton Posted at: 2017-11-10T00:36:08.471Z Reads: 338

```
[quote="Ackmaniac, post:1, topic:35116"]
throttle because afterward the battery max blocks a higher power output.
[/quote]

Do you need to buy a separate bluetooth module to use the Android App?
```

---
## \#135 Posted by: Eboosted Posted at: 2017-11-11T06:20:19.208Z Reads: 337

```
Hello @ackmaniac I wonder if you will work on a firmware to be uploaded via the latest VESC tool, or if you would use the latest current mode firmware to develop a newer version on Watt Mode. 

Do you think the latest Vedder firmware has some improvements over the one developed in this thread?
```

---
## \#136 Posted by: Ackmaniac Posted at: 2017-11-11T13:27:15.576Z Reads: 337

```
Don't know what you mean exactly. The Ackmaniac ESC-Tool firmware files are based on the official firmware (3.29) with the changes i mentioned in the first post of this thread. Current control in this firmware works more or less the same as watt control in my previous firmware mod.
```

---
## \#137 Posted by: mikenyc Posted at: 2017-11-22T13:34:41.264Z Reads: 336

```
anyone else running into an issue on the Mac where the app hangs during FOC motor detection? Clicking on RL spins the motor a bit and buzzes it. Then I get the Mac Beachball pops up, and it hangs there until I force quit. Is this a known issue, @Ackmaniac?

<img src="/uploads/db1493/original/3X/5/2/52f4aa11397518fdd03f9daf51830b835e012e0e.jpg" width="690" height="432">
```

---
## \#138 Posted by: Titoxd10001 Posted at: 2017-11-22T23:04:08.468Z Reads: 332

```
Ackmaniac, what can cause drv error message. Didn't notice anything while riding, wasn't riding to hard and everything seems to be working fine now. Running dual focbox, 6355, 12s

<img src="/uploads/db1493/original/3X/9/c/9cfd95aef0b5129511a72fd03ed49e96e9c0ad05.png" width="243" height="500">
```

---
## \#139 Posted by: wafflejock Posted at: 2017-11-22T23:08:15.523Z Reads: 326

```
This thread looks relevant:
http://www.electric-skateboard.builders/t/vesc-abs-over-current/19426

Appears you have a really high negative current which I think indicates you used the brakes somewhat hard at some point and it peaked over some absolute max value.  Probably nothing to worry about you can set your absolute max higher to avoid the error I think but I don't think it's really a problem so long as the battery and motor max are set at limits that keep those components safe, the absolute max seems to just be a catch all.
```

---
## \#140 Posted by: Ackmaniac Posted at: 2017-11-23T00:09:04.038Z Reads: 327

```
DRV errors are never good. Usually they happen a couple of times again and then your drive gets fried. The over current fault that you get us another story. Sadly in you screenshot the details of that error are not visible. Just tell us your motor, battery and absolue max.
And if you gut the DRV error in FOC you can try to raise the switching frequency to 30000 and hope that it is gone.
```

---
## \#141 Posted by: Titoxd10001 Posted at: 2017-11-23T00:46:02.335Z Reads: 334

```
My settings per focbox are 
Motor:100a... -50a
Battery:40a... -12a
Absolute should be default 130a

Running bldc. Battery is 12s4p 25r. Could it be to much regen no where to go? Getting 12s5p 30q soon. Think I've been getting abs fault need to start monitoring more frequently
```

---
## \#143 Posted by: TarzanHBK Posted at: 2017-11-23T07:39:22.136Z Reads: 336

```
It´s still a thing that some Vesc based ESCs don´t like 12s over time and simply shut down.
```

---
## \#144 Posted by: BigBoyToys Posted at: 2017-11-24T08:38:39.939Z Reads: 341

```
Maybe some esc's but the FOC box handles 12S like a champ.
```

---
## \#145 Posted by: Emerson Posted at: 2017-11-24T12:25:24.041Z Reads: 334

```
I'm having issues connecting to the Bluetooth module with the latest version of Android 8.0.  I've confirmed everything works with an older version. I can't even see the modules on 8.0.  any suggestions?
```

---
## \#147 Posted by: Youssless Posted at: 2017-11-25T16:14:11.780Z Reads: 339

```
@Ackmaniac thanks for your help so far, you've been a real pillar for this community. If I may,  I need to trouble you...

Board rides amazingly well and have 1,500+ miles but todayon the second leg of a ride my board jerked a little after 50m ir did so again almosy throwing me off.

I waited a bit then went home (about 1.5miles) at normal cruising speed and hit 30mph and there were no issues till I saw these at the bottom of the screen when I got home... 

<img src="/uploads/db1493/original/3X/e/1/e155d0664172ac71a8b763f100c7e0526b738896.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/e/a/eaaaeaf9eef720209f253b14a32e254a702a10b9.jpg" width="281" height="500">

Is my DRV gone?
```

---
## \#148 Posted by: Ackmaniac Posted at: 2017-11-25T16:20:22.180Z Reads: 302

```
Seem like that's the case. But I would also Check the Motor. Maybe the motor shorted under vibration. But most likely your DRV has issues.
```

---
## \#149 Posted by: Youssless Posted at: 2017-11-25T16:22:05.789Z Reads: 316

```
Thanks for getting back so quickly. What checks should I do, run it through your tool and see what happens or physically inspect the vesc and motor for anything funny? Both?
```

---
## \#150 Posted by: Ackmaniac Posted at: 2017-11-25T16:24:39.933Z Reads: 316

```
Would do a physical check
```

---
## \#151 Posted by: Youssless Posted at: 2017-11-25T16:32:28.249Z Reads: 332

```
Think I found the issue. Soldering joints was bent because the wires were too long and it was all too tight in my bakong tray of an enclosure. Vibrations eventually caused it to short after so many miles.

<img src="/uploads/db1493/original/3X/1/1/11c978f9bdb8c2e99be1b0bd2b308f3178edfe20.jpg" width="281" height="499">

<img src="/uploads/db1493/original/3X/4/3/43479aaee667650e9f9c630799e5646a477a930a.jpg" width="281" height="499">

The XT-90s connects to the VESC with the ground wire connecting to a female XT-90s for the loop key.

Given that there's a DRV8032 fault code, should I look to get a new VESC despite it getting me home safely? 

Obviously I'll be making new, shorter connections and do a better job of soldering either way.
```

---
## \#152 Posted by: Ackmaniac Posted at: 2017-11-25T16:38:40.487Z Reads: 319

```
Just solder it and try if it still works.
```

---
## \#153 Posted by: inferexcav Posted at: 2017-11-25T21:50:00.313Z Reads: 326

```
@Ackmaniac , hey Nico!
I've spend 1 hour in search of your 3.100.zip fw or higher and only one thing that I found on forums that everyone have that version and there is no link on it at all, only 2.54 which I already installed but I can't work with it cuz i need 3.100.
The only one prove of existence that version it's your comment with video "boi dat escalated quickly" with half of the link under the vid like  \foldername\fwname_3_100.zip  (it wasn't even nor on dropbox, nor on github)
anyone help, thx, that hour marathon search was a disaster
```

---
## \#154 Posted by: yaca Posted at: 2017-11-25T22:49:47.755Z Reads: 327

```
Download ackmaniac-ESC Tool, fw 3.100 is included.
```

---
## \#155 Posted by: Ackmaniac Posted at: 2017-11-25T23:04:30.342Z Reads: 336

```
In the first post of this thread you can find the download link of the ACKMANIAC-ESC Tool which has firmware 3.100 included.
```

---
## \#156 Posted by: Sebike Posted at: 2017-11-25T23:52:36.076Z Reads: 337

```
Trying to set the failsafe for my GT2B remote, but the poti only adjusts maximum to about +125% or -120% with full throttle or full brake. 

Having set the failsafe signal to the +125% value and then loosing connection, the VESC does not interpret this as if signal is lost and instead it goes into full throttle. :fearful:

Is there any way to use this new function of smooth braking even on the GT2B?
```

---
## \#157 Posted by: inferexcav Posted at: 2017-11-25T23:53:41.826Z Reads: 331

```
Sorry m8, this link is new, only one that I found before in your posts always was this link [drop 2.54 ackmaniac](https://www.dropbox.com/sh/t7dl90owz5ccbyl/AADNOs3g9TfYw-VAyYey3hZNa/BLDC-TOOl%20and%20Firmware?dl=0)
But now I'm already okay with new fw, thanks for fast reply, even at night. Is there any way to get new versions of FW in future without painful search (google never will let me found 3rd version of your fw, even forum search was really useless with that question, that's why I was a little bit triggered) Anyway, thank you!
```

---
## \#158 Posted by: Ackmaniac Posted at: 2017-11-26T01:11:49.324Z Reads: 324

```
Just set the failsafe when the pot is at left and a just the normal pulsewidth values when the pot is at the right. It doesn't need to be in the middle.
```

---
## \#159 Posted by: Sebike Posted at: 2017-11-26T01:36:41.319Z Reads: 325

```
I tried that as well, so now with about +145% the vesc still goes to full speed. Is there a setting for where the high signal should be ignored?
```

---
## \#160 Posted by: Ackmaniac Posted at: 2017-11-26T05:08:44.323Z Reads: 320

```
Above 120% it should be ignored.
```

---
## \#161 Posted by: Sebike Posted at: 2017-11-26T11:30:30.767Z Reads: 319

```
Ok. The PPM pulselength mapping reads "ESC tool +145%" and "from ESC +100%" when remote is switched off. Nothing one can do about this then I guess.. Too bad as it sounds like a great feature.

Edit; Tweaked the knobs and buttons and a few reboots later it works; +175% is ignored by the VESC. Setting-wise everything is the same as before and so are the switches and knobs on the remote. Very weird and a bit worrying that same exact settings gives a different reading now.. At least it works right now.
```

---
## \#162 Posted by: PXSS Posted at: 2017-11-26T13:54:50.185Z Reads: 316

```
I thought the failsafe was supposed to be set at 0% throttle? Am I missing something?
```

---
## \#164 Posted by: Ackmaniac Posted at: 2017-11-26T14:12:50.146Z Reads: 332

```
I just explained it in detail in the first post of this thread in this section.
[quote="Ackmaniac, post:1, topic:35116"]
Timeout Behavior

I spent a lot of time to find a good solution to make the board safer when the connection to the remote is lost.
What is the Issue with the standard firmware?
[/quote]
```

---
## \#165 Posted by: SeanHacker Posted at: 2017-12-13T03:00:24.641Z Reads: 346

```
@Ackmaniac Getting this error now when trying to setup my remote. Any idea what's going on?

2017-12-12 18:51:35: Status: Connected (serial) to COM3
2017-12-12 18:51:35: Status: ESC Firmware Version 3.100, Hardware: 410, UUID: 4B 00 41 00 08 51 36 30 34 35 31 38
2017-12-12 18:51:35: Status: MC configuration updated
2017-12-12 18:51:35: Status: App configuration updated
2017-12-12 18:51:42: Status: App configuration updated
2017-12-12 18:51:57: Status: APPCONF Write OK
2017-12-12 18:52:29: Status: App configuration updated
2017-12-12 18:52:43: Status: APPCONF Write OK
2017-12-12 18:53:37: Status: APPCONF Write OK
2017-12-12 18:53:46: Status: APPCONF Write OK
2017-12-12 18:54:17: Status: Applying Pulselengths Failed
2017-12-12 18:54:24: Status: Applying Pulselengths Failed
2017-12-12 18:54:34: Status: Applying Pulselengths Failed
2017-12-12 18:55:22: Status: Serial port error: No such file or directory
2017-12-12 18:55:25: Status: Not connected
2017-12-12 18:56:04: Status: Connected (serial) to COM3
2017-12-12 18:56:04: Status: ESC Firmware Version 3.100, Hardware: 410, UUID: 4B 00 41 00 08 51 36 30 34 35 31 38
2017-12-12 18:56:10: Status: Applying Pulselengths Failed
```

---
## \#166 Posted by: Sebike Posted at: 2017-12-17T11:11:53.309Z Reads: 343

```
Hi!
I tried measuring kv using the kv command in terminal, but ended up with it reading calculated kv 0.00rpm/volt although giving full throttle on the remote. Does this work for you or am I missing something?
```

---
## \#167 Posted by: egzplicit Posted at: 2017-12-17T12:16:55.987Z Reads: 334

```
I tried it yesterday and I got the same thing. Pretty sure it worked in 2.xx
```

---
## \#168 Posted by: dothebart Posted at: 2017-12-23T21:25:43.348Z Reads: 361

```
I've found my way into this thread by looking up what the new figures in the vesc-tool mean and how I can make use of them for my usecase.
I've read my way all through the two threads with lots of messages in them throughout the last two days.

Thus being a little bit late to this "party" let me have some words on this.

Working myself for a company that embraced an open community oriented workflow via github ( https://github.com/arangodb/arangodb )
(Comming from a closed source company) I know that working in the public (everybody being able to stalk you) is quiet a difference and one has to get used to it.

And at least from following the discussions in the first thread, after some pushing it seems to me that ackmaniac followed a more frequent source release series.

After havig done a PR to the vesc myself to make it a little bit more modular ( github.com/vedderb/bldc/pull/28 )
which hopefully will help it become better adoptable to multiple purposes - since my purposes isn't esk8s either.
Speaking of my PR, I'd like to direct at @trampa - it ended up in a mega-commit - github.com/vedderb/bldc/commit/f14115735812938ccd6142bbdcb7e1799c83d69a -
"Showing with 3,500 additions and 477 deletions" whithout feedback to the original PR on the actual release happening;
which I'd consider at least non well behaved or even as rude as others named the way Ackmaniac treated vedders source as well.

I think as percevied from the community (at least for me) Vedder went off into the closet to get a shiny new version with nice features readily available to the community
as it was polished until it was "presenteable" to a broader audience. As I've learned in this thread a broken leg pushed these timelines even more -
I hope vedder that you recovered good from that. We were presented the outcome of these 8 months in a singe git commit to the VESC firmware repository, and a shiny new UI.
While its debateable to work out something until its presenteable, that single commit doesn't attribute 3rd party contributions and stops every community member from having a look at the discrete steps of this development
so that we can learn from these steps. It really voids the open source pragma "release early, release often" 

Similar things can be said about the way Ackmaniac worked with his tremendous efforts in these two threads in the last one and a half year. While you developed nice
features very usefull to the community that use them, you've denied access to your insights you gained with these efforts to your fellow developers,
as I'd like to call vedder and i.e. me now.
If the truck-run-over-factor kicks in, you're leaving us a little less the way alone as the keyboard hacking community experienced with its valuable member Soarer suddenly disappearing:
https://deskthority.net/workshop-f7/xt-at-ps2-terminal-to-usb-converter-with-nkro-t2510.html without a single line of source.

Please Ackmaniac alter your workflow a little to embrace the way git (and gihtub) works. You simply need to push that work that far away from you so others can grab it easily and do it for you - no discussing or wasting of your precious time involved.

The regular github workflow works like this:
 - log into the github.com webpage with your account
 - head over to i.e. github.com/vedderb/bldc/
 - In the upper right you have the "fork" icon - press it.
 - This will create a fork of the offficial firmware repo on your github account - github.com/Ackmaniac/bldc
 - This is now a full featured fork, that can have all features the other repo has.
 - Clone this to your local harddrive using ` git clone github.com/Ackmaniac/bldc.git `
 - this gives you all current changes the local upstream firmware has.
 - You now work with this repo, develop, debug, and once you've found a thing to change, share your wisdom with us:
  - `git commit comm_can.c someotherfile.c -m "I've changed this for the faith of .... " `
  - `git push `
 -  (you may add all your current changes in an initial commit if you want to avoid the work of splitting it into discrete units)
 - now github.com/Ackmaniac/bldc will contain this special change in one commit.
 - once you've done a set of changes, you'd add a tag as others questioned vedder to do here github.com/vedderb/bldc/issues/31
 - I'd suggest you choose a versioning sheme that doesn't increase the vedder versioning, but appends your own version, so everyone can see this is the vedder-base xyz plus your changes:
   - `git tag v3.xxx-Ack-007; git push --tags`
 - now everyone can see the steps of your work leading to a release, and whats actually contained in a release.

Now s.b. else could see - whew - cool Ackmaniac added something we should have in the vedder repo. Lets say this person is me. 

so I'd have my own fork of the vedder repo on github (github.com/dothebart/bldc) which I've cloned to my local repo, which is my current working directory

$ git clone github.com/dothebart/bldc.git
$ cd bldc
### Now I will add the vedder repo to my workingcopy: 
$ git remote add upstream github.com/vedderb/bldc
### and yours:
$ git remote add ackmaniac github.com/Ackmaniac/bldc
### Now I would checkout your stage: 
$ git checkout ackmaniac/master
$ git pull
$ git log --stat
### would show me your commits. I can now cherry-pick them
### I will checkout vedders stage: 
$ git checkout upstream/master 
Previous HEAD position was 1655c11... Merge pull request #19 from pelrun/master
HEAD is now at 47c0826... Fixed CAN baudrate update
### I now branch a PR branch which will go to my dothebart repo:
git branch feature/add_ackmaniac_feature_xyz
git cherry-pick <git commit hash from log>
< fix eventual conflicts by editing >
git commit # now saves _your_ commit with my adjustments with a note that it was your commits with my edits
### I eventually will have to do more changes to make it work, I will `git commit` them... 
git push # will tell me the magic spell to create this branch on github.com/dothebart/bldc

now once I open github.com/dothebart/bldc I will get a popup, " do you want to create a PR to vedder? " I click yes, fill in stuff etc.
Hopefully vedder will get used to the github workflow, discuss on the issue, me changing stuff as requested, he will merge it.
=> your change merged upstream without you having additional effort or to discuss your work.

I hope that opposed to growing a living user community (that i.e. definitely exists around your fork) we also (as @trampa already tried to express) can grow
a lively developer community around the vesc and its ecosystem. I really do think that vedder has to work on his attitude here too, and the code base
of the ecosystem has to evolve in a way that features can grow up in branches (forks), and easily get merged back later on. 

If you need more help about using git or github, feel free to contact me via twitter.com/dothebart , freenode IRC, or phone.
@ackmaniac As you may have found out already I'm native german also, so maybe that could be easier. 

(removed some https'es to workaround my junior membership)
```

---
## \#169 Posted by: Sebike Posted at: 2017-12-24T00:19:20.207Z Reads: 323

```
woah... thats a lot of words in one post!
```

---
## \#170 Posted by: BigBoyToys Posted at: 2017-12-25T23:45:11.826Z Reads: 332

```
[quote="dothebart, post:168, topic:35116"]
(removed some https'es to workaround my junior membership
[/quote]

Did u just admit to hacking our forum to post as a junior memeber? Lol 😒
```

---
## \#171 Posted by: GrecoMan Posted at: 2017-12-25T23:46:47.424Z Reads: 334

```
I give him props lol.  If he was that dedicated he probably deserves to post more :joy:
```

---
## \#172 Posted by: dothebart Posted at: 2017-12-26T15:54:12.998Z Reads: 333

```
I'd vote for whitelisting github urls ;-)
```

---
## \#173 Posted by: Nooby Posted at: 2018-01-06T19:28:40.710Z Reads: 321

```
do you know if it would work with the Vesc1.1 from esk8.de :frowning:(@esk8  )?
```

---
## \#174 Posted by: Seikeau Posted at: 2018-02-04T23:07:48.368Z Reads: 296

```
Can anyone tell me a bit more about the PID Speed control no acceleration?

* Does it keep te speed you push to (when holding the throttle)?
* What speeds can you get to and can you limit the speed to wich it will accelerate?
* Do you need HALL-sensors on your motor for this?
* How 'experimental' is it exactly?
```

---
## \#175 Posted by: b264 Posted at: 2018-02-04T23:10:54.147Z Reads: 294

```
[quote="Nooby, post:173, topic:35116"]
do you know if it would work with the Vesc1.1 from esk8.de :frowning:(@esk8  )?
[/quote]

It should, since they say 
[quote]based on V 4.12[/quote]
on their web app
```

---
## \#176 Posted by: gaetjen Posted at: 2018-02-06T16:40:50.545Z Reads: 295

```
[quote="Seikeau, post:174, topic:35116"]
Does it keep te speed you push to (when holding the throttle)?
[/quote]
Yes, it does. You push the board and then hold the throttle and it keeps the speed

[quote="Seikeau, post:174, topic:35116"]
What speeds can you get to and can you limit the speed to wich it will accelerate?
[/quote]
You can set the speed limit  via the app. I have reached around 20kmh downhill and it kept the speed

[quote="Seikeau, post:174, topic:35116"]
Do you need HALL-sensors on your motor for this?
[/quote]
No, you don´t.

[quote="Seikeau, post:174, topic:35116"]
How ‘experimental’ is it exactly?
[/quote]
Works for me just fine without problems.
```

---
## \#178 Posted by: Apolo Posted at: 2018-02-22T03:05:11.687Z Reads: 274

```
The mac version of the new esc tool crashes every time after flashing firmware. Not a big deal since it still flashes successfully and I can just reboot the tool but I thought i'd just let you know
```

---
## \#179 Posted by: noamlin Posted at: 2018-02-22T18:08:53.212Z Reads: 280

```
hi this looks to be a better tool and i want to use it,
but how do i install it on LINUX?
```

---
## \#180 Posted by: stormboard1 Posted at: 2018-02-28T22:50:43.019Z Reads: 273

```
how do i get this going on my focbox ? just plugged it in have the bldc tool but ackmaniac is suppose be much better..something about i need to flash the focbox?lol.. sorry cant find a guide anywhere

running windows 10
sensored motors and focbox
```

---
## \#181 Posted by: mmaner Posted at: 2018-02-28T23:04:19.581Z Reads: 273

```
Just read through the thread its all there.  Noone is gonna give you a 6 word method, it's more intricate than that, so do the research so you will UNDERSTAND.
```

---
## \#182 Posted by: stormboard1 Posted at: 2018-02-28T23:11:32.412Z Reads: 271

```
ya fair enough looks complicated but gotta be don.
are the correct vesc setting in this?
```

---
## \#183 Posted by: deucesdown Posted at: 2018-02-28T23:15:16.912Z Reads: 274

```
Just so you don't waste time hoping and praying... It sucks but there's 101 ways to blow up a vesc. Every software/firmware/hardware version brings new ways. Because there are so many ways, there are no guides that will keep you 100% safe.

Gonna have to search and read a fuckton ,and hope you've read enough.

And you still might blow it up.

BTW, if I'm wrong about this please shout me down.
```

---
## \#184 Posted by: Jc06505n Posted at: 2018-02-28T23:27:19.660Z Reads: 275

```
That kinda sucks honestly , sure you can research , but if you start researching the wrong shit or missed a part that you weren’t suppose to, you can be out of a good $200 or a headache at the least. Just looking back at the CANBUS vs Split debate, if people didn’t see the comment where you have to cut ground when splitting (I believe that was the solution to that issue) you were straight lining your VESC6’s to the eventual slaughter (if I’m not wrong).

For software like this were there’s a good 2 or 3 similar applications, there really NEEDS to be a quickstep guide or set up guide with a good ELI5 do’s and don’ts. 

I’ve read The thread for VESC-Tool , Enertion’s tool , METR, eSkate VESC, and BLDC Thingamagig ( I am seriously bad with names) and I STILL don’t understand the difference, advantages, and disadvantages of each application against each other. Once I get to configuring my Focboxes I’ll have to reread each thread and guide cause fuck me if I don’t understand the tool more useful for my needs and understanding capacity.
```

---
## \#185 Posted by: stormboard1 Posted at: 2018-02-28T23:28:58.093Z Reads: 274

```
an esk8 vesc tool wizard is needed lol
```

---
## \#186 Posted by: Jc06505n Posted at: 2018-02-28T23:33:21.703Z Reads: 278

```
We just need a software comparison between the tools and I’m kinda surprised there isn’t one, especially when each application is being updated constantly which results in one tool being good for this thing at one point and not being the tool you need at another.
```

---
## \#187 Posted by: sayekim Posted at: 2018-03-01T12:44:23.696Z Reads: 290

```
Yeah I was looking for one too. I just added a guide to my build page. Hope it helps.

https://www.electric-skateboard.builders/t/meepo-esc-to-focbox-blank-double-kick-drop-down-90-mm-hubs-missing-part/44021
```

---
## \#188 Posted by: saybot Posted at: 2018-03-04T13:28:31.996Z Reads: 291

```
Hi, got problem with BLDC settings. Ive got sensored motor so I set in BLDC Sensor mode to: Sensored and when i backward at controller motor behavie very weird. Take a look
https://www.youtube.com/watch?v=IzMhsCd5fLM&feature=youtu.be
```

---
## \#189 Posted by: Ackmaniac Posted at: 2018-03-04T17:12:30.710Z Reads: 290

```
Did you run the hall sensor detection and is the minimum pulsewith in the ppm settings correct?
It also can be that the sensor is placed badly which sometimes leads to a well running motor in one direction and a bad running in the opposite direction.
```

---
## \#190 Posted by: Silverline Posted at: 2018-03-08T18:08:52.177Z Reads: 300

```
Just updated my focboxès from the original 3.28 vesc fw to newest 3.35fw. Now i experiencing exactly this same braking behavior at low rpms : http://www.electric-skateboard.builders/t/vesc-brakes-grabbing-coming-to-stop/46946

Is this the same behavior with the @Ackmaniac FW ?? Or do it have a function, so the vesc dosn`t do full brake the moment i brake slightly at low rpms ??

Thanks
```

---
## \#191 Posted by: Sebike Posted at: 2018-03-10T19:50:00.652Z Reads: 302

```
Was going to calculate kv and went full throttle on the bench. 

Realtime data keeps showing negative values for power, motor and batt amps, and T-motor. That's one cool motor..

![bench|690x100](upload://pe3p2WOSYbCLMEIOxX6zCxMxyVp.jpg)

Any idea why that is?
```

---
## \#192 Posted by: driver Posted at: 2018-03-13T20:53:34.921Z Reads: 284

```
HELP

i updatet the FW, but i choosed hw:48
I have 2 Focboxes, booth are not working anymore :cry:

Is there any solution?
```

---
## \#193 Posted by: Ackmaniac Posted at: 2018-03-13T22:55:28.122Z Reads: 283

```
You have to flash it via a cheap programmer. You will find the info in the forum when you look for it.
```

---
## \#194 Posted by: b264 Posted at: 2018-03-14T14:08:10.769Z Reads: 282

```
@Ackmaniac  Where is this at?  I'd like to run it but I can't find it.  It's not in the dropbox.
```

---
## \#195 Posted by: Ackmaniac Posted at: 2018-03-14T16:07:49.683Z Reads: 281

```
What do you mean?
```

---
## \#196 Posted by: b264 Posted at: 2018-03-14T16:09:47.948Z Reads: 281

```
I only see built versions for Windows and mac but no ESC Tool.  I can't run either of those
```

---
## \#197 Posted by: Ackmaniac Posted at: 2018-03-14T16:19:48.160Z Reads: 289

```
So what do you need?
```

---
## \#198 Posted by: b264 Posted at: 2018-03-14T16:22:09.542Z Reads: 300

```
Ubuntu, or the source and I can build it.  I'd like to check out your mods but never have been able to.  It's not worth using a virtual machine when I can just use the Vedder versions.

What is the github/bitbucket link?
```

---
## \#199 Posted by: Ackmaniac Posted at: 2018-03-14T16:27:24.405Z Reads: 305

```
Source is available on Github.

[Source Code](https://github.com/Ackmaniac/vesc_tool)
```

---
## \#200 Posted by: b264 Posted at: 2018-03-14T17:16:58.558Z Reads: 313

```
[Linux build is available for the Ackmaniac version](https://github.com/b264/vesc_tool/tree/ee3347f84c662751f3492309ac4fc604c6704f7d/build/lin)

edit: [newer one below](https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/335)
```

---
## \#201 Posted by: driver Posted at: 2018-03-14T17:51:26.559Z Reads: 308

```
Do i have to downgrade or how?
```

---
## \#202 Posted by: b264 Posted at: 2018-03-14T17:52:47.766Z Reads: 351

```
I was able to fix that without a programmer, but do not run any motor until you upload the correct firmware.  I also accidentally picked 48 once.  I don't remember how I fixed it, with one of the tools I was able to load the 412 firmware.
```

---
## \#203 Posted by: bevilacqua Posted at: 2018-03-14T18:10:43.792Z Reads: 343

```
You have to completely flash the VESC: New Bootloader and then software. 

Search for „St-Link bootloader“

Edit: http://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752
```

---
## \#204 Posted by: b264 Posted at: 2018-03-14T18:16:09.848Z Reads: 339

```
What I'm saying is I accidentally installed 48 firmware on a FOCBOX and succesfully got 412 firmware flashed onto it *without* using a programmer or uploading a new bootloader.  Unfortunately I don't remember which tool I used; it was a linux build of one of them, and not this one above.
```

---
## \#205 Posted by: bevilacqua Posted at: 2018-03-14T18:18:21.698Z Reads: 337

```
Interesting... I also flashed my vescs with the wrong HW-Fw but didnt manage to resolve it without using a st-link. Would be nice if you remember how, specially for those who dont have a programmer.
```

---
## \#206 Posted by: driver Posted at: 2018-03-14T18:34:51.519Z Reads: 336

```
I can upload a new bootloader, but "..it will destroy bootloader and firmware..updates cannot be done anymore..."

Do or not do?? What does it mean?
Can i destroy it and then install the right firmware??

![Unbenannt|690x422](upload://mB4pxfU4es1QWgZwiK6P10NxYrm.jpg)
```

---
## \#207 Posted by: Silverline Posted at: 2018-03-14T18:58:59.683Z Reads: 310

```
Anybody knows the answer ? Thanks
```

---
## \#208 Posted by: Deckoz Posted at: 2018-03-14T19:01:32.220Z Reads: 316

```
FOC or bldc? 

What's your min rpm before applying full brake set at?
```

---
## \#209 Posted by: Silverline Posted at: 2018-03-14T19:15:36.750Z Reads: 315

```
FOC on motors without sensor.
I have not touch those settings, because i don`t think that the original vesc-tool allows me to change that settings ? What i´m saying is, that i run the settings pretty much stock, besides the motor/battery min/max thing. Do you think that i would get rid of that crappy function, if i flash the ackmaniac fw instead ?
Thanks..
```

---
## \#210 Posted by: b264 Posted at: 2018-03-14T20:17:52.634Z Reads: 311

```
I said no to that question and did not upload a new bootloader
```

---
## \#211 Posted by: saybot Posted at: 2018-03-21T22:23:56.774Z Reads: 307

```
hi, ive got problem with throttle on about 26% motor work on full power, how to change that 50% of throttle = 50% of motor duty etc.? the same is with reverse;/
![Untitled|690x388](upload://3qP0IFLatnWCvSIncYtotjs9HeB.png)
```

---
## \#212 Posted by: Silverline Posted at: 2018-03-21T23:36:10.291Z Reads: 293

```
Is this on the bench, or when riding ?
```

---
## \#213 Posted by: b264 Posted at: 2018-03-21T23:37:25.725Z Reads: 290

```
What is on the "Throttle Curve" tab?
```

---
## \#214 Posted by: Ackmaniac Posted at: 2018-03-21T23:39:09.832Z Reads: 292

```
I know a lot of people want that but it doesn't really make sense. If you expect the motor to turn with 50% speed when at 50% throttle then how much % torque should the motor give when the motor is actually at 10% speed.
```

---
## \#215 Posted by: Eboosted Posted at: 2018-03-22T05:20:16.149Z Reads: 293

```
I wonder if anyone was able to avoid the wheels locking during braking at almost dead stops.

The maximum ERPM for full brake parameter is no longer displayed on the ESC tool.
```

---
## \#216 Posted by: intensivegecko Posted at: 2018-03-22T05:25:14.752Z Reads: 293

```
What's the difference from the esc-tool and bldc tool in the dropbox?
```

---
## \#217 Posted by: saybot Posted at: 2018-03-22T07:19:15.443Z Reads: 299

```
this test is performed in bench. The throttle curve is default.
Im asking also because ive got two level of speed from controller (~75% and 95%)and during riding it not change anything since ive full duty on 26% throttle
```

---
## \#218 Posted by: rey8801 Posted at: 2018-03-22T13:45:22.172Z Reads: 300

```
Probably It's me but with all this different version I got a bit confused about some points. For my build I am using 10s3p 30Q battery, diyeboard hub motors (75Kv, 500W each, rated for 50A continuous current), 2 Maytech vescs  and Nano-X remote. this are my setting for the motors 

![image|690x388](upload://yMAKzS0HXFV6C2QnI20xq5NEvmi.jpg)
PS: I am using @Ackmaniac  ESC tool.

Now my douts:
1- Do you think my setting are ok? motor max, min ecc...
2- I selected current no reverse with brakes and I know it works as watt control mode. During the motor setup wizard I didn't encountered anything where I can set the max watt. Now by looking at the general BLDC configuration I see there is watt limit at the bottom. Could someone please explain me how to do?
3- Is the throttle curve purely experimental or there is a good common starting point?

4- Are the data displayed during the realtime data detection accurated? Because I could get only 20km/h out of them, which is half of what I was aspecting.

Sorry for the questions, I just want to be sure before doing something that I will regret.

Ciao ciao
```

---
## \#219 Posted by: Ackmaniac Posted at: 2018-03-22T20:46:35.355Z Reads: 282

```
Forget bench testing if you want to test how fast you get at different % of throttle. Once you ride the board you will understand that the throttle controls the torque and not the speed.
```

---
## \#220 Posted by: Ackmaniac Posted at: 2018-03-22T20:58:05.966Z Reads: 286

```
_1- Do you think my setting are ok? motor max, min ecc…_
**Battery Current max regen can be increased. With you battery to at least -6 A but i would go even higher to for example -9A in your case (i know that's higher than the max charge current but it will only do that for a couple of seconds when you brake)**

_2- I selected current no reverse with brakes and I know it works as watt control mode. During the motor setup wizard I didn’t encountered anything where I can set the max watt. Now by looking at the general BLDC configuration I see there is watt limit at the bottom. Could someone please explain me how to do?_
**With your battery max setting you are capable of roughly 25A * 36V = 900W. So 2 motors will produce 1800W. But you can also set the value lower if you want. If you want more you also need to increase the battery max because the watts can only be reached if the battery max allows it.**

_3- Is the throttle curve purely experimental or there is a good common starting point?_
**Throttle curve works great. Just give it a try. Try this setup.**
![image|690x378](upload://fp1D5lzTWRcFGTQwBbfce6WbsBv.png)
```

---
## \#221 Posted by: rey8801 Posted at: 2018-03-22T21:16:03.261Z Reads: 273

```
Thank you very very much! Below my thoughts about it:
1- Ok, I will increase it to -6A. As far, as I know it will affect my brake and of course the amount of current I send back to the battery). Is it correct?
2- Perfect so I do not have to set the watt anymore. The battery I use based on real test is capable of 60A costant discharge, I just wanted to be a bit conservative, but if the performance won't be sufficient I will increase it.
3- Great! I will try it out.

Now, I am trying to connect the sensor cable to the vesc. I had to adapt the connection from the motor to the vesc and I can get one motor sensored, while the other one gives me error during the detection. As far as I know what matter are the 5v, Temp and GND correctly placed, while the hall sensors order is not relevant. Is it correct? I see a clear difference in sensored mode, at lower speed the motor starts really smoothly. Thx!
```

---
## \#222 Posted by: Ackmaniac Posted at: 2018-03-22T21:24:39.138Z Reads: 262

```
The pin of the hall sensor cables doesn't matter but 5V and GND needs to be right. And the charge current will increase, that's correct.
```

---
## \#223 Posted by: rey8801 Posted at: 2018-03-22T21:28:25.173Z Reads: 262

```
ok than I do not know why the sensor cables are detected from one vesc but not the other. I will try to switch the motor and see whether is the vesc or the cable. Thx for the help, really appreciated.
```

---
## \#224 Posted by: RedEagle Posted at: 2018-03-22T21:36:31.293Z Reads: 270

```
15000 watts?! That doesn't seem right..
```

---
## \#225 Posted by: rey8801 Posted at: 2018-03-22T21:43:11.386Z Reads: 285

```
HI that's why I am asking here. During the motor wizard you are not able to control that value...only later I notice it. Althought if you click on the ? it tells you that the default value is high to disable it and the other limit are still valid. Is it correct @Ackmaniac?

 ![image|690x388](upload://vcRocTc8OWpyRocKPl695hMpHH.jpg)
```

---
## \#226 Posted by: RedEagle Posted at: 2018-03-22T21:48:38.590Z Reads: 274

```
Allright, then you're sorted.
```

---
## \#227 Posted by: rey8801 Posted at: 2018-03-22T22:15:56.086Z Reads: 282

```
the only thing that I still have to understand is why one vesc doesn't detect the sensor. sensorless they do detect the moto but in sensor mode the motor are detected but the sensors just in one of them. I will switch the motors to see if it is due to the motors or the vescs.
```

---
## \#228 Posted by: RedEagle Posted at: 2018-03-22T22:18:55.517Z Reads: 280

```
I myself haven't been able to test that since I'm running unsensored. Maybe a issue with the wires themselves? Or missing chips on the vescs? Configured uncorrectly?
Lots of factors to be taken into account..
```

---
## \#229 Posted by: rey8801 Posted at: 2018-03-22T22:23:54.623Z Reads: 282

```
Indeed. I was already surprise that for one worked immidiately. On the bench you see the difference at the start. With sensor is way smoother but otherwise I will use it sensorless
```

---
## \#230 Posted by: Ackmaniac Posted at: 2018-03-22T23:02:55.707Z Reads: 284

```
Often it works when you switch the direction of the motor by switching 2 phase wires. That's because of badly placed sensors. If that also doesn't work then the sensors could be broken. Also have one motor where all sensors don't work. Can be testen by checking the voltage at a signal wire of the sensor with a multimeter. Should show 3.3v and 0v depending on the actual magnet position. Just search on YouTube for checking hall sensor signals.
```

---
## \#231 Posted by: rey8801 Posted at: 2018-03-22T23:19:59.656Z Reads: 277

```
Thanks, super useful as usual.
```

---
## \#232 Posted by: Exiledd_Top Posted at: 2018-03-23T15:10:20.249Z Reads: 281

```
I have a question am sure someone here with more experience can help me , I downloaded ackmaniac tool for my 4wd carvon all 4 vesc go get reverse now heres my problem after downloading and setting it up, my previous settings before ackmaniac were
Motor max: 60 
Motor min regen -40
Battery max :32
Battery min (regen): -6
It felt pretty good I would be at 65% throttle and and around 35mph 
After installed I changed up a bit 
Motor max : 65
Motor min regen -45
Battery max :35
Battery min (regen): -6
Now am around 80% throttle and berly around 32mph 
Things that I think are the culprit , I never did the remote test on the new bldc I just transfers those settings feels the same but not sure 
Ran foc detection with wheels on but did the same thing with previous bldc ? 
Any thoughts guys
Using wat for reverse
My build 
Carvon 4wd 
12s6p 30q
4 focbox foc mode
```

---
## \#233 Posted by: b264 Posted at: 2018-03-23T15:24:55.104Z Reads: 269

```
[quote="Exiledd_Top, post:232, topic:35116"]
Ran foc detection with wheels on
[/quote]

I was under the impression that it's better to not even have a pulley on.
```

---
## \#234 Posted by: Ackmaniac Posted at: 2018-03-23T15:31:29.946Z Reads: 272

```
That is because you were using the normal current control.
In my firmware mod current control works like watt control.

In the original firmware the problem is that the board does full power at higher speeds even when you only pull the trigger 50%.
In my firmware 50% trigger only does 50% power.
By this you have more control over the board because you can control the power much better.
I explained this in more detail here
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/171?u=ackmaniac
```

---
## \#235 Posted by: Exiledd_Top Posted at: 2018-03-23T15:53:28.488Z Reads: 262

```
I think am going to revert back to non ackmaniac only wanted because reverse function but having a reverse effect from more control at higher speeds to having control at lower speeds but not reaching top speed
```

---
## \#236 Posted by: Ackmaniac Posted at: 2018-03-23T16:46:53.579Z Reads: 259

```
Pull the trigger simply more to reach full speed.
```

---
## \#237 Posted by: rey8801 Posted at: 2018-03-23T21:44:45.506Z Reads: 278

```
Hi! So at the end I went for BLDC sensorless. Indeed with your throttle curve I see an big improve at low speed (all the test on bench at the moment). I got the Bluetooth today and I install it... The app is crazy! Its possible to set almost everything. Here a screen shoot at max speed. Two question is it normal that I reach 95% of duty at most? Secondly the top speed measured is only 24km/h, is it realist? Thx

![vescmonitor|281x500](upload://pXz0NA5ZpmebQl6Pu6rjZtHGUEs.png)


AH almost forgot about it. When you make new modes is the one at the top that would be in use? If not how can I select which mode to use?

![vescmonitor|281x500](upload://gC4cpdrNtmGjsIs6d16XjYP7IAm.png)
```

---
## \#238 Posted by: Bjork3n Posted at: 2018-03-23T21:51:26.104Z Reads: 258

```
I installed firmware 3.1 today! Can't wait to try it out! 
I have some issues using ackmaniac app, drops out alot. Could be cuz I use the metr module.
```

---
## \#239 Posted by: Ackmaniac Posted at: 2018-03-23T22:41:10.319Z Reads: 264

```
You should go to the settings and adjust the Drive Gear Setup to enter the amount of motor magnets, Wheel size (diameter) Wheel pulley teeth and Motor pulley teeth. by that i can calculate the speed. A hint, a normal 6374 motor or 6355 has 14 Magnets.
Duty cycle of 95% is the maximum a VESC with hardware 4.x can reach.
After you created modes you can select them by clicking on the mode box which will open a popup window where you can select one of your modes.

![image|283x376](upload://4H0cMSmMo71clk6QDNkj3Z6DfJI.jpg)
When it shows default then it is the mode which is stored on the VESC. When you want that one of your modes becomes the new default then you have to click long on the mode box and a popup window will appear which asks you to set the currently active mode as the new default.
You can even swith between FOC and BLDC of you made the motor detection for both modes.
```

---
## \#240 Posted by: rey8801 Posted at: 2018-03-23T22:54:34.385Z Reads: 260

```
Got it for the modes I will try it. For the drive set up I did it. I have dual hub motor (the one from DIYeboard, like meepo hubs). Now I am not sure it was correct.
![vescmonitor|281x500](upload://kECSbYNRIyVH8u9ppk9PO6Kt97R.png)
```

---
## \#241 Posted by: Ackmaniac Posted at: 2018-03-23T23:31:40.995Z Reads: 251

```
Checked some pictures in the internet and it seems the Meepo hubs only have 20 magnets. But not sure if i looked at the right motor. You should try to find out or count by yourself.
```

---
## \#242 Posted by: rey8801 Posted at: 2018-03-23T23:56:21.265Z Reads: 249

```
Ok thx I will check. So just to understand how it is calculate the speed in the app? I mean not the potential but the live streaming one. I thought it is based on the RPM.
```

---
## \#243 Posted by: rey8801 Posted at: 2018-03-24T09:59:43.850Z Reads: 259

```
So I tried again the mode switch and indeed it's super easy :+1:.
1- During the motor wizard in the ESC Tool the max W was automatically set at 15000 (in order to disable it). Therefore the max watt would be calculated based on the max battery (25A in my case), Is it correct?
2- Now in the app by swithcing modes we can set the max watt that replaces the 15000 default one. For instance in my case 25A *37 = 925w. Is it correct to do that or it's better to leave 15000? In my mind the throttle curve is set based on the max watt so If I choose 15000, the VESC will try to reach 15000 at full throttle meaning it would ask at most 925w already at 6.17% of the throttle curve [(935*100)/15000]. SI it correct? Sorry for all the question but I really like it and I would like to understand it better.
3- I checked for the number of poles, someone said that we have to introduce the number of pair poles ( so half of the total), but in my case if I put 14 is like 72Kmh, with 28 56Kmh and so on... In all the case a get 24Kmh max speed... Not really clear this point.

![IMG_20180324_110105|281x500](upload://jy9tHbMeEeJinZJBxNNjCLxOS2r.jpg)

![vescmonitor|281x500](upload://vUFF2Pw32sFUHf6zbsxBQUw8ayN.png)
```

---
## \#244 Posted by: Ackmaniac Posted at: 2018-03-24T13:01:26.601Z Reads: 240

```
In this version of the firmware it will be either limited by the current or by the watts. But i recommend to set the battery max to the max your battery or VESC can handle and the watts to finetune the power output. 
So in your case battery max rto 30A (3P * 20A / 2Motors) and then set the watts to whatever you want. So 1080 should be max fpor yoiur battery and 2 Motors. If you want less power simply change the watts. If you want less power at low speeds you should change motor max.
```

---
## \#245 Posted by: rey8801 Posted at: 2018-03-24T13:07:42.168Z Reads: 237

```
Ah ok now I got it. So basically it takes the limited factor as the max level. It can be either current or watt. Ok I will  do it. My bms has costant discharge current of 60A so probably better to limit a bit the watt to do not run it at the max level, although it will drain 30A just in case of sever hills and not always so it shouldn't be a problem. If I change the parameter in the app does it change it also for the other VESC connect by canbus or do I have to connect the vesc to the vesc tool separately to change the motor max and battery max? Thx you very much.
```

---
## \#246 Posted by: Ackmaniac Posted at: 2018-03-24T13:54:17.295Z Reads: 240

```
You have to connect the app to the master. So if your Bluetooth module is connected to the master it is fine. If connected to the slave you can tell the app to connect to the master via CAN.
So when you change settings on the master it automatically updates all slaves over CAN.
```

---
## \#247 Posted by: rey8801 Posted at: 2018-03-24T13:58:37.077Z Reads: 244

```
My app is connected to the master and the two VESC are connect over CAN so I just need to change it in the app and it will be updated to the slave too. Is it correct? Just as confirmation.
Concerning the measured speed it only reads 24kmh, I hope that it is not the real one, otherwise my setup is crap :joy:
```

---
## \#248 Posted by: Bjork3n Posted at: 2018-03-26T13:33:00.698Z Reads: 239

```
Tested out this firmware today, tested it on a single drive. 
Its smooth and nice def more controllable! 
I do miss some off the aggressiveness but this can be cuz i only tried it with one motor and the last test what with dual.

Im running sensorless but with this fw its like running sensored from a dead stop, its super nice!
Cant wait to test it with dual motors
```

---
## \#249 Posted by: rey8801 Posted at: 2018-03-26T14:02:31.203Z Reads: 238

```
I just want to confirm that if you are running the app on the master vesc and it is connected with the slave, via  CAN, then all the modifications made in the app are updated on the slave too. Cool! No need to open the enclosure to change the vesc setting anymore.
```

---
## \#250 Posted by: Bjork3n Posted at: 2018-03-26T14:09:01.882Z Reads: 244

```
Yeah thats dope! I dont dare to run CAN anymore tough...last time i did a burnt a drv chip.
But it could be that i was had bad luck.

Maybe i will try CAN someday again, that feature is awesome..
```

---
## \#251 Posted by: rey8801 Posted at: 2018-03-26T14:12:14.915Z Reads: 239

```
otherwise you can connect a bluetooth module to each vesc :rofl:
I hope I won't occur in the same problem :disappointed_relieved: why a CAn connection would lead to a DRV error? Just out of curiosity.
```

---
## \#252 Posted by: Bjork3n Posted at: 2018-03-26T14:16:10.310Z Reads: 241

```
Dont know but there are alot of people having issues with can. Do a search and you find tons.
**But there are also people that have great sucess with CAN.**

Im running split ppm at the moment just because of this. 
But i do miss the feature of information from 2 vesc....
```

---
## \#253 Posted by: Silverline Posted at: 2018-03-26T14:36:16.612Z Reads: 239

```
Hey @Bjork3n , so you are saying that you have stutter free motor from dead stop with ackmaniack fw, with sensorles motors? May i ask, what motor you are using, and what settings 😀

Just tested the original vesc fw 3.35 on my board with 2x focbox / sk3 6364 190kv(sensorles), and got at lot of stutter in foc mode from dead stop, almost as much as in bldc mode. Big  disappointment, so i switch back to bldc mode, because i think the responsnes and acceleration/brakes felt better.
```

---
## \#254 Posted by: Bjork3n Posted at: 2018-03-26T14:44:43.447Z Reads: 233

```
Thats correct, its amazing.
Using 6355 190kv motors.  
Motormax 60A
Battery max 30A
Start up boost 0.05 

75kg.

Will post a video in 30min!
```

---
## \#255 Posted by: Silverline Posted at: 2018-03-26T14:50:45.760Z Reads: 237

```
6355 sk3's ? What makes ackmaniack's fw better than stock fw, regarding stutter from 0 km/h on sensorles ?
I think start Up boost : 0.05 is pretty default right ?
My battery max and motor max is the same on mine (on stock vesc fw 3.35)
```

---
## \#256 Posted by: Bjork3n Posted at: 2018-03-26T14:54:57.953Z Reads: 241

```
Dont know but it did notice that the power is not as jerky as with the stock fw. Maybe thats what making it better.
```

---
## \#257 Posted by: Bjork3n Posted at: 2018-03-26T15:06:33.594Z Reads: 245

```
Sensorless start

https://youtu.be/HeSKcLnZazQ
```

---
## \#258 Posted by: Bjork3n Posted at: 2018-03-26T18:20:20.619Z Reads: 245

```
Did some more testing after some charge and still impressed.
If you like to throttle out of corner this Firmware is a must!
Now its all smooth out of the turn, before you had to brace yourself cuz you never knew when the power would kick in!
Amazing work, just amazing....
```

---
## \#259 Posted by: Silverline Posted at: 2018-03-26T18:45:46.337Z Reads: 245

```
deleted 
10 char
```

---
## \#260 Posted by: Bjork3n Posted at: 2018-03-26T18:48:49.028Z Reads: 243

```
Switched to ackmaniac fw from stock fw
```

---
## \#261 Posted by: theviith Posted at: 2018-03-29T23:13:08.316Z Reads: 240

```
quick question, can the 2.54 firmware update from this mod be applied to Vesc-x? I know it works for original vesc but not sure if the vesc-x will work. Has anyone tried it?

Also, huge thanks to @Ackmaniac for making this BLDC tool mod, very nicely done!!
```

---
## \#262 Posted by: Ackmaniac Posted at: 2018-03-30T00:52:37.600Z Reads: 246

```
The version 3.100 is more advanced then 2.54 version. I know it is confusing.
Of course it works with VESC-X a.k.a FOCBOX
```

---
## \#263 Posted by: Bjork3n Posted at: 2018-04-10T05:42:34.463Z Reads: 243

```
Just a quick check before I setup my focboxes, the wizards for both motor and controller works just like in the standard vesc tool? 
No bugs anymore? 
Found a post from a while back saying there was some issues with the wizards and focboxes is this resolved? 
Going to try Canbus again and will use the wizard to get all the settings right . 
Thanks
```

---
## \#264 Posted by: Ackmaniac Posted at: 2018-04-10T06:38:23.380Z Reads: 245

```
My version didn't have a issue with the focbox. Actually I was the one that fixed that problem.
```

---
## \#265 Posted by: Bjork3n Posted at: 2018-04-10T06:47:56.116Z Reads: 245

```
Never fails to impress 👏
```

---
## \#266 Posted by: b264 Posted at: 2018-04-12T15:46:45.023Z Reads: 246

```
[quote="Ackmaniac, post:262, topic:35116, full:true"]
The version 3.100 is more advanced then 2.54 version. I know it is confusing.

Of course it works with VESC-X a.k.a FOCBOX
[/quote]

@Ackmaniac just to be clear, version 3.100 comes [from here](https://github.com/Ackmaniac/bldc/tree/7df7d918124d5e561860ca0589b66710a7dbb01e/build_all), is this correct?
```

---
## \#267 Posted by: Tuomalar Posted at: 2018-04-12T17:57:31.261Z Reads: 242

```
I think it's the one in Dropbox named as ESC-tool (3.100) @b264
```

---
## \#268 Posted by: b264 Posted at: 2018-04-12T17:59:36.788Z Reads: 231

```
@Tuomalar There is no firmware in there and no source code
```

---
## \#269 Posted by: Jumpman Posted at: 2018-04-12T18:43:10.985Z Reads: 233

```
I got mine from the link in the first post, unless you are looking for something else.
```

---
## \#270 Posted by: b264 Posted at: 2018-04-13T00:13:21.120Z Reads: 238

```
I looked there and it's all 2.54

[quote="Ackmaniac, post:262, topic:35116"]
The version 3.100 is more advanced then 2.54 version.
[/quote]

:arrow_up: this is the one I am looking for
```

---
## \#271 Posted by: danielz Posted at: 2018-04-13T00:30:31.860Z Reads: 241

```
https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAAKyJSTlryFplI0fA67Pnt-a/ACKMANIAC-ESC-Tool?dl=0
```

---
## \#272 Posted by: b264 Posted at: 2018-04-13T00:42:48.614Z Reads: 234

```
It's not in there....

Compiled firmware looks like `VESC_default.bin` and firmware looks like `main.c`

This is why I am asking @Ackmaniac since he is recommending this thing which I can't find
```

---
## \#273 Posted by: danielz Posted at: 2018-04-13T00:51:42.768Z Reads: 237

```
install the tool, firmware tab, the latest is there for flashing
```

---
## \#274 Posted by: b264 Posted at: 2018-04-13T00:52:18.958Z Reads: 236

```
I am asking @Ackmaniac.  And what you said is not true because it doesn't run and there is no source.

This [ESC Tool works](https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/200?u=b264) but I can't find the 3.100 firmware he is referring to.
```

---
## \#275 Posted by: danielz Posted at: 2018-04-13T00:53:29.055Z Reads: 233

```
oh you want the source, yes ask him
```

---
## \#276 Posted by: Ackmaniac Posted at: 2018-04-13T06:38:23.360Z Reads: 243

```
https://www.electric-skateboard.builders/t/why-isn-t-acknaniac-s-fw-on-github-edit-i-m-an-idiot/51790/6?u=ackmaniac
```

---
## \#277 Posted by: Rotko Posted at: 2018-04-13T17:44:55.171Z Reads: 257

```
Hi guys, I really need some help, I’m stuck:

Dual per can bus setup (focboxes)
Mini remote
Foc mode

Arranged all this to get cruise control and, ironically I got it alone now:
When I pull the trigger mini start in cruise control mode (have to break to decrease speed), steering wheel doesn’t work.
Advices?

MASTER


![1|690x388](upload://7WzEiznZadpjvkscCtVD4pdnukn.jpg)![2|690x388](upload://j8jxPAb6rTsslVZcFZPdao4oblk.jpg)

SLAVE

![1|690x388](upload://vTOmpPzpChQPdPKIRxZhk5AVnGh.jpg)![2|690x388](upload://cdBnrxS2aBPMCJfQ4Ktf2EvD2H4.jpg)


Binding is ok, I followed this:
https://www.youtube.com/watch?v=ywUfqtKF8Zg

Throttle is in Ch2
And Cruise in Ch3

questions?
```

---
## \#278 Posted by: Ackmaniac Posted at: 2018-04-13T18:01:58.491Z Reads: 236

```
At the master you need your normal control mode like current control and at the slave you need to select the control mode with cruise. So the opposite of yours.
```

---
## \#279 Posted by: Rotko Posted at: 2018-04-13T18:10:27.462Z Reads: 242

```
sorry Ack I changed the photos in order to enhance the quality while you were helping me. Maybe I inverted some photos. But now they are in order. Can you check again?
Because I was sure I had already followed your indications: I set

Master = 0 = "Current no reverse with brakes"
Slave = 1 = "cruise control via slave"

I re-set these value once more to be sure after your comment  and I got a weird behaviour:
just touching the throttle caused the motors to spin at max speed.
Couldn't brake.
I'm clueless
```

---
## \#280 Posted by: Ackmaniac Posted at: 2018-04-13T19:51:22.896Z Reads: 244

```
You need to connect Channel 1 to the slave vesc and not channel 3. 
Just a tip, set a high deadband like 50% for the slave so that cruise really only activates when the wheel is turned a lot. 

By the way, to all Vesc 6 owners. Don't use the ppm cruise function because it can brake your ppm pins. Focbox and other which are based on Vesc 4 hardware seems to be fine.
```

---
## \#281 Posted by: Rotko Posted at: 2018-04-14T08:20:03.052Z Reads: 235

```
Thank you Ackmaniac. It works!!!
```

---
## \#282 Posted by: RyuX Posted at: 2018-04-15T18:16:48.365Z Reads: 238

```
Sorry if thas was covered already, but on this tool how do I set a Soft RPM Limit to limit my maximum speed ?

Thank you
```

---
## \#283 Posted by: Mikenopolis Posted at: 2018-04-17T02:16:50.762Z Reads: 233

```
Sorry if this was already asked. But I couldn’t find it. 

I finally got to the point of this build to program the FocBoxes. Everything went well until I realized the motors were going on the wrong direction. I went to swap the phase wires and the motor just seem to cog. I guess it’s becuase of the hall sensors?

**I know there’s a reverse motor direction function but can find it!** 

I’m running FOC if that makes a difference.
```

---
## \#284 Posted by: b264 Posted at: 2018-04-17T02:19:48.363Z Reads: 225

```
Do the motor detection again after you swap the wires
```

---
## \#285 Posted by: Mikenopolis Posted at: 2018-04-17T02:47:28.784Z Reads: 229

```
Thanks. I’ll try that later. Has it always been like that? I remember just flipping two phase wire did the trick
```

---
## \#286 Posted by: b264 Posted at: 2018-04-17T02:55:35.297Z Reads: 230

```
I think if you are not using sensors it might not matter.  If you are using sensors you'll need to recalibrate everything
```

---
## \#287 Posted by: mmaner Posted at: 2018-04-17T03:02:38.146Z Reads: 238

```
@b264 is right. If you are running for it hybrid you need to redo the detection without wheels mounted for it to be ultra accurate. With bldc it doesn't matter if you switch phase wires assuming there's no obstructions in the can.
```

---
## \#288 Posted by: b264 Posted at: 2018-04-17T03:05:04.077Z Reads: 238

```
[quote="mmaner, post:287, topic:35116"]
without wheels mounted
[/quote]

Wait, what?  I thought there had to be no pullies or anything mounted.  Really, is removing the wheels enough?
```

---
## \#289 Posted by: Mikenopolis Posted at: 2018-04-17T03:05:41.866Z Reads: 230

```
Thanks guys. That was the issue. Didn’t use sensors before. Not having wheels on it.. lesson learned
```

---
## \#290 Posted by: mmaner Posted at: 2018-04-17T03:05:49.347Z Reads: 228

```
No, your right. I'm tired 😄. Nothing should be attached to the motor.
```

---
## \#291 Posted by: goldrabe Posted at: 2018-04-18T02:05:26.511Z Reads: 237

```
Need some help with braking in FOC.

I flashed my 4.12 Vesc´s with the latest 3.100 firmware and did setup FOC sensorless for both Vesc´s and motors.
I am using the Nano remote and the Vesc´s are connected via Canbus, both motors are spinning after a slight push and acceleration is just fine and smooth. In PPM i have set current with no reverse and braking. And my remotes signal is centered. 
But when braking, i just get strong braking for a split second and after that the board coast´s and brakes in a rhythmical pattern but with no braking force at all, i don´t know how to describe it, it´s like a kind of cogging.
I played with battery min. regen. and lowered it down to -7 to no avail.
Sometimes when i accelerate just for a short time the braking works as expected, but if the speed drops beyond a certain amount the board start´s coasting again. When I accelerate to a higher speed the brakes will disengage immediately. This kind of cogging, or whatever i should call it, happens through all the throw of my remote, so the Vesc seems to recieve the signal properly.
Running the same setup in BLDC works just fine.
I hope someone can enlighten me, i really want that silent FOC to be running.
Here in Japan people are jelling and swearing at me because of the noise running BLDC.
```

---
## \#292 Posted by: webst Posted at: 2018-04-18T06:07:28.639Z Reads: 231

```
I never run BLDC but I have similar problems with FOC when going downhill and the regen current of -10 is not enough to stop my (m)ass. Are you trying to brake on flat spot when this happens? What’s your weight?
```

---
## \#293 Posted by: goldrabe Posted at: 2018-04-18T06:26:21.085Z Reads: 241

```
Yeah flat ground. And the speed at that is happening is random.
I just plugged both VESC's in to the Esc tool and saw that both show the f*cking DRV error.
Anyway motor detection still works in both modes and in BLDC everything is working as it should.
```

---
## \#294 Posted by: Ackmaniac Posted at: 2018-04-20T20:11:26.063Z Reads: 253

```
_**NEW ACKMANIAC_TOOL 3.101**_

Just released the new **Version 3.101** of the **Ackmaniac-Tool** which includes the latest changes of Benjamin Vedders original firmware and fixes 2 important issues.

1. By another thread i realized that one of the motors stopped braking when the maximum speed is exceeded like one user reported. This also caused the problem that dual motors did brake uneven when connected by CAN and motor min and motor max had different values. 
With the new firmware you will realize that the brakes feel less strong but you can simply adjust that by increasing the motor min value. Because now they brake with the same power.

2. And the other problem was that the brakes disabled themself when the start of the mosfet or motor temperature was reached. 

Both issues came from the original firmware and i addressed the second problem already in the official VESC forum. The first problem came also from the original firmware but Benjamin never used the function that caused the issues.

Another minor issue is also fixed which let the slave motor brake when you try to enable cruise control while driving backwards (guess nobody noticed that).

I recommend to update the firmware even if it takes some time to setup everything again. Maybe you should first save the settings with the old Ackmaniac-Tool and then load these settings in the new one. But still double check everything. And test the board properly if everything behaves normal after the update.

PS: I realized that when the master and the slave have both "Send status via CAN" activated and the same "Controller Id" then the slave motor can cut out. So please be careful that the master doesn't have this parameter enabled and to be safe give them a different "Controller Id".
```

---
## \#301 Posted by: Ackmaniac Posted at: 2018-04-20T23:00:12.508Z Reads: 237

```
Sorry for deleting posts but i think the update info is important. 
BTW i updated the GIT repository. And Mac version is hopefully coming soon.
```

---
## \#302 Posted by: SeanHacker Posted at: 2018-04-21T00:48:47.636Z Reads: 236

```
Anything change with canbus? Can't seem to get both motors spinning now with the newest firmware.
```

---
## \#303 Posted by: Ackmaniac Posted at: 2018-04-21T01:00:16.276Z Reads: 244

```
Yes the CAN Baudrate needs to be setup now and should be the same on all ESC. 
I recommend 500K. 
And take care that "Send CAN status" is only activated at the Slave and disabled at the master.
And as there are new messages for the CAN Bus all VESC should have the same firmware. So don't try it with only one updated. just flash both and then do the setup.
![image|690x174](upload://xBznrP2zB2YqoSbfv92Y6XRN9um.png)
```

---
## \#304 Posted by: SeanHacker Posted at: 2018-04-21T01:22:40.308Z Reads: 249

```
Thanks dude! I've updated both vescs (I wouldn't not update them both lol) but I still can't get it to work right for some reason. I've been using these same settings for almost two years now. Any ideas or am I missing something?

Master-
![Master2|690x360](upload://r5MjuDkKQYNu3wyvB6Lh4wHFvCY.PNG)![Master|690x360](upload://1ZPQSzXK5MI8I7vkpdknmXj2bmI.PNG)

Slave-
![Slave2|690x360](upload://vjzYcRczlZ9inoo3WpVv6yrYw7c.PNG)![Slave|690x360](upload://b7LsFOAgDSGWdjuxbLKAnr9aF3O.PNG)

https://www.youtube.com/watch?v=6fAhaHdPGf0
```

---
## \#305 Posted by: Ackmaniac Posted at: 2018-04-21T01:28:15.209Z Reads: 232

```
Try to set the "CAN Status rate" to 100 Hz. I am at skype for a couple of minutes, maybe we can have a look together.
And are you sure that you executed the hall sensor detection and applied the values on the motor that jitters?
```

---
## \#306 Posted by: SeanHacker Posted at: 2018-04-21T01:35:38.168Z Reads: 234

```
Yeah. I actually thought it was maybe a bad motor detection at first so I've run them a few times now on each motor. I'm going to going through both motor detections and setup really quick. If I can;t get it going and you wanna skype I'm up for that too. I'll let you know in just a few minutes. Thanks for the help!
```

---
## \#307 Posted by: SeanHacker Posted at: 2018-04-21T01:53:04.302Z Reads: 236

```
So I've done both motor detections and have everything setup correctly as far as I know. Not sure where to go next.

Update-
And once again @Ackmaniac to the rescue! Thanks for the help and getting me back up and running once again dude. You're one of a kind!!!
```

---
## \#308 Posted by: webst Posted at: 2018-04-21T05:54:15.490Z Reads: 227

```
Can you elaborate on solution?
```

---
## \#309 Posted by: Ackmaniac Posted at: 2018-04-21T11:17:56.254Z Reads: 235

```
He was using a Virtual Machine to be able to use Windows. And he had the live relatime data, app data and heat rate enabled. Seems that that was too much for the serial communication so that some of the reads and writes didn't work. After disabling of all the live data it worked without issues.
So if you use the Windows via a Virtual Machine then you should disable all the live data when you change values.
```

---
## \#310 Posted by: fraannk Posted at: 2018-04-22T18:18:08.412Z Reads: 233

```
v3.101 works like a charm in FOC on my FOCBOX'es :+1:
```

---
## \#311 Posted by: b264 Posted at: 2018-04-22T19:44:32.327Z Reads: 237

```
That's closest I've ever heard brushless electric motors sound like an internal combustion engine.  It seriously sounds like a chainsaw.
```

---
## \#312 Posted by: SeanHacker Posted at: 2018-04-22T19:59:58.218Z Reads: 239

```
Yeah man. They were sounding crazy! This is how they sound now though. Thought I'd give FOC a go for a bit and see how much money I can blow. Haha ;)

https://youtu.be/ZDD3w5suYXk
```

---
## \#313 Posted by: AntiPusher Posted at: 2018-04-22T22:41:31.996Z Reads: 234

```
i may have seen skipped something, but can i get this for mac?
```

---
## \#314 Posted by: Emerson Posted at: 2018-04-23T02:29:22.440Z Reads: 234

```
Are there any other BLE modules that can be used instead of the HM-10? My hope is to have better connectivity with Android 8.0+ (or any connectivity really).
```

---
## \#315 Posted by: b264 Posted at: 2018-04-23T02:43:58.964Z Reads: 234

```
[quote="AntiPusher, post:313, topic:35116"]
can i get this for mac
[/quote]

He [posted the source](https://github.com/Ackmaniac/vesc_tool/tree/5581f16503b28cad50273f808659e23330a3979f) if you want to build it for apple.
```

---
## \#316 Posted by: Skifree Posted at: 2018-04-24T03:37:50.531Z Reads: 233

```
The maker of the HM-10 says that it is compatible with 8.0, but the clones or "fakes" as they call them are not reliable with 8.0.

http://jnhuamao.cn/index.asp
```

---
## \#317 Posted by: Emerson Posted at: 2018-04-24T12:35:53.726Z Reads: 232

```
I've purchased from a couple different vendors and they have all been "fake" it seems.  Anyone have a source for legit HM-10 modules?

All of mine have ended up being CC41-A  :frowning:
```

---
## \#318 Posted by: MartyMcFly88 Posted at: 2018-04-24T12:49:57.349Z Reads: 233

```
There is a way of updating the chip on the fake modules which might help,  @SeanHacker  wanted to see if that might help. If you have an arduino you could try this: https://www.youtube.com/watch?v=ez3491-v8Og

But you should read this first: 
https://blog.yavilevich.com/2018/04/should-you-throw-away-your-cc41-hm-10-clones-now-that-android-8-is-here/
```

---
## \#319 Posted by: Blacksheep Posted at: 2018-04-25T02:20:59.841Z Reads: 227

```
is there a mac version ?
```

---
## \#320 Posted by: zepton Posted at: 2018-04-27T20:42:46.727Z Reads: 226

```
I just got a DRV8302 fault when I switched my board to 9S (I plugged in the batteries on the bench I didn’t ride it). It works perfectly fine with 6S, and when I switched back from 9S to 6S it worked as usual…anyone else have this issue?
```

---
## \#321 Posted by: b264 Posted at: 2018-04-28T01:58:22.538Z Reads: 232

```
[quote="Blacksheep, post:319, topic:35116, full:true"]
is there a mac version ?
[/quote]

He [posted the source](https://github.com/Ackmaniac/vesc_tool/tree/5581f16503b28cad50273f808659e23330a3979f) if you want to build it for apple.
```

---
## \#322 Posted by: Blacksheep Posted at: 2018-04-28T02:01:48.689Z Reads: 222

```
I don’t know how hehe
```

---
## \#323 Posted by: b264 Posted at: 2018-04-28T02:04:40.786Z Reads: 222

```
Never a better time to learn.  It's a QT application
```

---
## \#325 Posted by: SeanHacker Posted at: 2018-04-28T02:56:55.598Z Reads: 228

```
https://www.qt.io
```

---
## \#327 Posted by: b264 Posted at: 2018-04-28T06:43:06.697Z Reads: 225

```
Let [the journey](http://bfy.tw/HsaV) begin.  I don't know how either, but if I wanted it bad enough, I'd figure it out.
```

---
## \#329 Posted by: SeanHacker Posted at: 2018-04-28T15:24:30.365Z Reads: 229

```
Just use the free version. Works just fine. I've never used QT before this morning so I'm still learning about it and how things work. But I was able to compile a build for linux (something I need!!!) in about 3-5 minutes or so. I also removed the beginning pages so that I don't have to read it every time I open the app. If I get a few minutes later I'll compile you a Mac build. Gotta go ride before the rain hits!!! 

https://youtu.be/tLRjvG-OSIs
```

---
## \#331 Posted by: sayekim Posted at: 2018-04-29T05:35:25.427Z Reads: 225

```
I’m sticking with 3.1 firmware until metr and perimetr are compatible with 3.101 and until there is a Mac version of the tool. 

Looking forward to this. @Ackmaniac
```

---
## \#332 Posted by: isabar Posted at: 2018-04-29T17:57:46.920Z Reads: 225

```
I am trying to use the latest version of VESC Monitor (V1.85) on a Galaxy S6 (Android 7.0), and although I see the bluetooth module, the second I select it in VESC Monitor, the App crashes.  I didn't have this issue a few weeks ago, so am wondering if there is a bug in the latest updated to VESC Monitor (V1.85).  anyone else seeing this? @Ackmaniac
```

---
## \#333 Posted by: Ackmaniac Posted at: 2018-04-29T18:28:29.723Z Reads: 217

```
Fixed the issue already in the latest version 1.88.
```

---
## \#334 Posted by: BigBrit Posted at: 2018-04-29T18:28:36.736Z Reads: 226

```
3.101 is compatable with Metr mate, using it myself!
```

---
## \#335 Posted by: b264 Posted at: 2018-04-29T18:37:22.324Z Reads: 223

```
I built [the version with 3.101 for linux](https://github.com/b264/vesc_tool/tree/8d6ae44d880b7f649fb9f89671c9ceaf57bab17a/build/lin).  Enjoy
```

---
## \#336 Posted by: isabar Posted at: 2018-04-29T20:43:07.477Z Reads: 224

```
yes. it is now working. Thank you!

However, is there anything you can do to keep the app from crashing/freezing when the VESC is turned off?
@Ackmaniac
```

---
## \#337 Posted by: Ackmaniac Posted at: 2018-04-29T23:29:55.507Z Reads: 227

```
Doesn't happen with my phone. But i will have a look with my other one.
```

---
## \#338 Posted by: Sebike Posted at: 2018-04-30T00:00:08.182Z Reads: 226

```
This might be a stupid question, but if I'd want to have a mode that's using only one motor, would that be possible (and safe for the vesc) by adjusting settings in the app? Like maybe setting batt and motor max to zero but still having it connected and powered on? 

If so, could one use two motors for braking, setting batt and motor min values, but using only one motor for acceleration?

😁
```

---
## \#339 Posted by: SuperBen Posted at: 2018-04-30T00:01:36.367Z Reads: 226

```
If you press back multiple times it will close out correctly, but I get the same freeze when I click the disconnect button, and have to force close to get it running again.

Closing from the switcher when you have continual notification on doesn't work, when happens when you hit disconnect, have to force close
```

---
## \#340 Posted by: Ackmaniac Posted at: 2018-04-30T00:24:28.925Z Reads: 225

```
Wouldn't try. It also doesn't make sense to use only one motor. It should be more efficient to run 2 instead of one if both need to move anyway. Because then they run with half current and that means lower heat losses.
```

---
## \#341 Posted by: b264 Posted at: 2018-04-30T01:01:44.287Z Reads: 227

```
Under certain circumstances it could make sense to run with one motor if there was some sort of malfunction happening and you were trying to get back home.
```

---
## \#342 Posted by: isabar Posted at: 2018-04-30T05:48:54.767Z Reads: 226

```
Also one thing I don't understand why it hasn't been integrated in the VESC firmware:  Right now, every time you powercycle the board, the Watt-hour, Amp-hour, and distance data is lost (rezeroed).  To make a useful battery gauge, that data should be stored in non-volatile EEPROM (on the VESC ST Microcontroller), and only rezeroed either via the app or whenever the voltage of the battery gets above let's say 41.0V (for 10S pack), which indicates that the board has been recharged (just like when you rezero your trip odometer on your car after filling your tank with gas).  Please try to implement this in the VESC firmware and App as it will make the battery gauge a lot more useful.  @Ackmaniac
```

---
## \#343 Posted by: Eboosted Posted at: 2018-04-30T06:00:59.744Z Reads: 223

```
[quote="Eboosted, post:215, topic:35116"]
I wonder if anyone was able to avoid the wheels locking during braking at almost dead stops
[/quote]

@ackmaniac sorry to bring this back again, but is there a fix for this issue? Problem does not happen in BLDC
```

---
## \#344 Posted by: b264 Posted at: 2018-04-30T06:08:49.260Z Reads: 216

```
@Eboosted Could you please describe that a little more?  That sounds like a desirable feature, not a bug.  I'm confused

What exactly is happening?
```

---
## \#345 Posted by: Eboosted Posted at: 2018-04-30T06:32:15.177Z Reads: 214

```
If you run FOC whenever you are braking and are approaching to a dead stop, let's say 2km/hr, the brakes lock themselves at full brake and you get thrown forward.

This doesn't happen on BLDC mode.
```

---
## \#346 Posted by: b264 Posted at: 2018-04-30T06:39:07.070Z Reads: 212

```
If you can adjust the speed the stop happens at, that sounds fucking fantastic for waiting at a red electric traffic signal.  No more throttle, brake, roll back, throttle, brake, roll back, throttle, brake, roll back, throttle, brake, roll back
```

---
## \#347 Posted by: webst Posted at: 2018-04-30T08:51:53.440Z Reads: 208

```
I have the same happening on regular firmware. When approaching to full stop speed wise the wheels blocks itself fully. It doesn't block the wheels when your speed is zero and you have full brake engaged.
```

---
## \#348 Posted by: fraannk Posted at: 2018-04-30T08:57:42.865Z Reads: 206

```
Doesn't happen to me in unsensored FOC on FOCBOX'es :) ackmaniac v3.101
```

---
## \#349 Posted by: Ackmaniac Posted at: 2018-04-30T09:18:44.591Z Reads: 214

```
It is the normal behavior. At slow speed the VESC can't detect the speed of the motor and does a full short when braking. It really depends on your motor at which speed that happens. 
That's the reason some notice it and some not. My firmware mod does the same as the original when it comes o this behavior.
With sensored motors it is much better.
And it also depends on how many cells in series your battery has. Because at braking below 3% duty cycle the VESC will go into that block. And with a 12S battery that happens at 20% higher speed then for a 10S Battery.
```

---
## \#350 Posted by: webst Posted at: 2018-04-30T10:08:12.195Z Reads: 214

```
Thanks for explanation. I have one more problem (regular firmware), braking related. I tested it on 6S which happened to be safer thing to do. When I go downhill freely and speed is higher than highest speed setup can go and try to break slowly it's rapidly slowing to max speed setup allows. I was lucky that I discovered this while going 30kmh and braking slowed me rapidly to like 26kmh (max with 6S) and I managed to keep myself on a deck. Is this how things work, even on your firmware?
```

---
## \#351 Posted by: koralle Posted at: 2018-04-30T10:17:17.860Z Reads: 212

```
This might actually be how I broke my foot 2 weeks ago. I was pondering the whole time wtf happened and decided I must have jerked the lever too hard because I wasn't concentrating but it sure didnt feel that way at the time....
Board locked up at around 45-50kmh and left me chewing asphalt.
```

---
## \#352 Posted by: webst Posted at: 2018-04-30T10:23:50.265Z Reads: 214

```
Sorry to hear that! I believe that problem occurs because of set voltage limits, vesc has max set and it starts decelerating with calculated presets which is basically precalculated ERPM. I hope that this can be  somehow overriden.
```

---
## \#353 Posted by: Kug3lis Posted at: 2018-04-30T10:24:03.661Z Reads: 213

```
and here me who cant even hold still with brakes on 1% incline... But I guess it's only because of 5:1 gearbox
```

---
## \#354 Posted by: Kug3lis Posted at: 2018-04-30T10:28:24.373Z Reads: 219

```
P.S. Would be possible to implement something like hold up like if the board rolls back to apply small throttle to hold it still or etc?
```

---
## \#355 Posted by: Ackmaniac Posted at: 2018-04-30T10:48:00.762Z Reads: 215

```
That was only the case in the old firmwares that started with a 2 like 2.18 or 2.54. In the new ones that start with a 3 that shouldn't be the case anymore.
```

---
## \#356 Posted by: webst Posted at: 2018-04-30T10:55:45.982Z Reads: 212

```
This happend on HW6.4 based Escape, can't check FW version now
```

---
## \#357 Posted by: Ackmaniac Posted at: 2018-04-30T11:28:09.855Z Reads: 212

```
Well also not sure what happens when you go faster than the speed of your battery voltage and motor kv. Think you shouldn't design your system like that when you know you can reach higher speeds.
```

---
## \#358 Posted by: webst Posted at: 2018-04-30T11:31:45.608Z Reads: 206

```
Problem is this is not common knowledge and it has already broken one foot. Is there any way to implement autobraking when speed is higher than system max?
```

---
## \#359 Posted by: Ackmaniac Posted at: 2018-04-30T11:39:01.974Z Reads: 210

```
Bad idea. Means it auto brakes at any time while you are accelerating or free coasting. Was like that in the old versions when you accelerated. If you ask me then the components of your system don't fit to your way of riding.
And it's not sure that this was the reason for the broken foot. And it should be addressed in the vesc-project forum. 

But in theory you should not reach higher speeds than your motor can achieve on the bench when it spins freely.
Because the BEMF (voltage of motor) will be higher than the voltage of the Battery and in this case it can only work as a generator which leads to braking. There is physically not much you can do if you ask me.
```

---
## \#360 Posted by: koralle Posted at: 2018-04-30T11:56:46.251Z Reads: 212

```
Okay. I will do some more research on this. Had not given it any thought tbh. I was gunning down hill at almost 50 and my boards top propulsion speed is 46.6 at full battery. Battery was almost empty at 3.1V

If nothing can be done about this, it should be made super well known to all eskate builders. I also think auto braking is a bad idea. I would prefer completely deactivating braking to just locking the wheels.

Edit: Actually really smooth auto braking to limit your downhill speed to max motor speed would be perfect now that I think about it.
```

---
## \#361 Posted by: webst Posted at: 2018-04-30T13:54:59.091Z Reads: 214

```
When I mentioned autobraking I meant that you cannot go higher than vesc max RPM which should be rather easily implemented as VESC is constantly monitoring motor position through BEMF it should be possible to detect when wheel rotation count is approaching highest for configured voltage and not allow to go beyond that speed by engaging braking with deceleration curve twice or triple times as long as acceleration one (2-3 times less steep). We wouldn't even need place to add wheel diameter or gearing ratio to calculate real speed as it would only need max motor RPM count for selected battery voltage.
```

---
## \#362 Posted by: guyguy Posted at: 2018-04-30T14:49:13.310Z Reads: 216

```
Can't you do that by keeping your throttle engaged?

[quote="chaka, post:20, topic:35005"]
The question about overrunning the ERPM is a good one, you have to be carefull with that. One thing I do is keep my throttle fully engaged when hitting my top speed while going downhill. With the throttle engaged as you reach your top electrical speed you will feel the motors produce drag to keep the speed from increasing any further. If you let off the throttle the motors will free wheel and you could overrun the ERPM
[/quote]
```

---
## \#363 Posted by: Acklavidian Posted at: 2018-04-30T15:34:50.551Z Reads: 209

```
Am I right in my findings that you cannot connect via bluetooth from a desktop computer?
```

---
## \#364 Posted by: koralle Posted at: 2018-04-30T15:48:10.370Z Reads: 208

```
Ehm thanks man I wish I had stumbled upon that post earlier. It should be pinned in the beginner thread actually.

So does this actually charge the battery? If so then what happens if min battery A is hit?

Hows the risk of frying your focbox while doing this?
```

---
## \#365 Posted by: koralle Posted at: 2018-04-30T16:35:11.159Z Reads: 206

```
How is this issue tackled by professional boards like ollin, boosted, @longhairedboy etc?
```

---
## \#366 Posted by: isabar Posted at: 2018-04-30T18:33:07.873Z Reads: 207

```
Still having issues with the VESC MONITOR (V1.89) crashing/freezing when the VESC is turned off.  
Galaxy S6 (Android 7.0).  Tried it on other phones as well. Same issue. 
@ackmaniac
```

---
## \#367 Posted by: Eboosted Posted at: 2018-04-30T18:37:22.163Z Reads: 219

```
[quote="isabar, post:366, topic:35116, full:true"]
Still having issues with the VESC MONITOR (V1.89) crashing/freezing when the VESC is turned off.

Galaxy S6 (Android 7.0).  Tried it on other phones as well. Same issue.

@ackmaniac
[/quote]

If this can be fixed it would be great!
```

---
## \#368 Posted by: koralle Posted at: 2018-04-30T18:46:15.448Z Reads: 213

```
What happens when you suddenly press full throttle while already going faster than your boards max speed? Will that also gently slow you down?
```

---
## \#369 Posted by: Michael319 Posted at: 2018-04-30T19:05:49.477Z Reads: 219

```
When I do this on my sensored board it just ignores the input basically
```

---
## \#370 Posted by: Ackmaniac Posted at: 2018-04-30T19:26:25.012Z Reads: 217

```
When the app crashes you are asked of you want to send the error report. Please do so.
```

---
## \#371 Posted by: isabar Posted at: 2018-04-30T19:32:57.879Z Reads: 212

```
I did send the error report
```

---
## \#372 Posted by: Ackmaniac Posted at: 2018-04-30T19:45:01.116Z Reads: 219

```
Please do me a favour and send it again. And please make sure that you have the latest version 1.89. Because the issue that i think wa reported by you is reported for version 1.88 and in 1.89 that problem should be solved.
```

---
## \#373 Posted by: skatardude10 Posted at: 2018-04-30T19:46:47.867Z Reads: 216

```
For my app crashes after rebooting my board, I just do a quick force stop shortcut and start it back up again and I'm back up and running quickly. 

If I don't have to do this with the new versions, this would be even nicer than this awesome app already is. 😎
```

---
## \#374 Posted by: longhairedboy Posted at: 2018-04-30T20:01:21.855Z Reads: 219

```
[quote="koralle, post:365, topic:35116, full:true"]
How is this issue tackled by professional boards like ollin, boosted, @longhairedboy etc?
[/quote]

I don't ship boards with firmware that has fried things until i can test it and make it not fry things. Unfortunately i don't have a ton of time for testing new stuff, especially things as complex as new firmware before shipping it out to people with little experience in that department, so i'm still on older releases.
```

---
## \#375 Posted by: Ackmaniac Posted at: 2018-04-30T20:05:00.483Z Reads: 213

```
The described issue also happens in older releases in all versions.
```

---
## \#376 Posted by: webst Posted at: 2018-04-30T20:05:21.071Z Reads: 216

```
Can you please check following scenario, preferably on some low speed setup? If what we suspect is true this is problem for all firmware versions. @koralle is pretty sure that is what broken his foot. 

[quote="webst, post:350, topic:35116"]
I have one more problem (regular firmware), braking related. I tested it on 6S which happened to be safer thing to do. When I go downhill freely and speed is higher than highest speed setup can go and try to break slowly it’s rapidly slowing to max speed setup allows. I was lucky that I discovered this while going 30kmh and braking slowed me rapidly to like 26kmh (max with 6S) and I managed to keep myself on a deck.
[/quote]

There has been few comments stating that you shouldn't go freely above your system RPM but for me it's just a design flaw. I want to be able to go down with no motor hum, and safely use brakes.
```

---
## \#377 Posted by: SeanHacker Posted at: 2018-04-30T20:20:11.402Z Reads: 220

```
Thanks for the update dude. Works great as expected! Your app has actually saved me quite a few times now! 

https://youtu.be/d83AcZZM5wk
```

---
## \#378 Posted by: lazopm Posted at: 2018-04-30T21:01:47.853Z Reads: 218

```
@Ackmaniac Would be a good idea to put the compiled application for macos/windows/linux in the github repo's releases.
It would make it easier for people to find the version/OS they need if they don't know how to compile the source code themselves.

Example project with releases: https://github.com/facebook/zstd/releases
```

---
## \#379 Posted by: koralle Posted at: 2018-04-30T22:06:01.369Z Reads: 208

```
So you have not gone down hill faster than your boards can go on your workbench?
```

---
## \#380 Posted by: b264 Posted at: 2018-04-30T23:03:50.147Z Reads: 207

```
@lazopm one million likes to you, sir.  This would make things a lot easier all the way around if everyone used standard open-source workflows.
```

---
## \#381 Posted by: mikenyc Posted at: 2018-04-30T23:17:24.087Z Reads: 211

```
It's diff for each platform though. Seems that I have to write a config file to create a pkg for Mac. I would have published it for everyone, but I also don't think it's great to have a bunch of stray unofficial builds floating around.
```

---
## \#382 Posted by: Ackmaniac Posted at: 2018-04-30T23:47:31.059Z Reads: 210

```
Please have a look again if the issue still exists with version 1.91?
```

---
## \#383 Posted by: b264 Posted at: 2018-05-01T00:38:29.031Z Reads: 216

```
If you used the 0.82 and 3.101 versions of the ESC Tool and the BLDC firmware then I wouldn't call it an "unofficial build" if it's the code @Ackmaniac made.  If you changed the code that matters, then probably yeah.
```

---
## \#384 Posted by: isabar Posted at: 2018-05-01T04:50:58.413Z Reads: 221

```
still have the problem in 1.91 .. and yes I did change the app setting to "do not optimize" for battery life.  Is that what you wanted me to try?  Basically if the VESC is turned off while the app is open, the app freezes and when you turn the VESC back on, it doesn't recover. you need to kill the app and open it again, which is obviously not ideal
```

---
## \#385 Posted by: MartyMcFly88 Posted at: 2018-05-01T09:19:18.364Z Reads: 220

```
Yes, I agree, in theory this shouldn't happen, but if you have hills or a long slope and don't Monitor your Speed constantly.. you should be able to rely on your breaks to slow you down .. But this should maybe go into the vesc forum..
```

---
## \#386 Posted by: longhairedboy Posted at: 2018-05-01T14:59:17.474Z Reads: 224

```
[quote="Ackmaniac, post:375, topic:35116, full:true"]
The described issue also happens in older releases in all versions.
[/quote]

Does it happen in the firmware in 2.18? because that's what i'm using on production boards still. 

@jayx is running version 3.x on his 13S build. Maybe he can chime in here since he keeps blowing shit up and streeting his face. I'm too old for that shit, and most of my customers are total noobs or don't understand any kind of unexpected weirdness.
```

---
## \#387 Posted by: briman05 Posted at: 2018-05-03T11:47:16.320Z Reads: 210

```
@Ackmaniac the wax tool gets locked up on macs when updating firmware and must be force quit. Plus now my motor that was detected by bloc tool is not being detected. How can this happen?
```

---
## \#388 Posted by: Jayx Posted at: 2018-05-06T03:59:21.919Z Reads: 209

```
@koralle depends on your set up. If I did that I would be leaving red skidmarks on the pavements. In BLDC mode it never happens. But it happens very often in some of my FOC set ups.
```

---
## \#389 Posted by: b264 Posted at: 2018-05-06T04:03:27.556Z Reads: 220

```
[quote="koralle, post:368, topic:35116, full:true"]
What happens when you suddenly press full throttle while already going faster than your boards max speed? Will that also gently slow you down?
[/quote]

These sound like the words of a software engineer
```

---
## \#390 Posted by: t0m_r1dd1e Posted at: 2018-05-07T23:11:01.341Z Reads: 213

```
Sorry for the likely dumb question, but I couldn't find it by searching...

Which hardware version and firmware version should I be flashing on my focbox?
```

---
## \#391 Posted by: Ackmaniac Posted at: 2018-05-07T23:23:38.745Z Reads: 213

```
![image|690x163](upload://zs71buTmCtaJ1tExZInqARL0pkf.png)

The FOCBOX is based on the 4.12 Hardware.
```

---
## \#392 Posted by: skatardude10 Posted at: 2018-05-07T23:24:04.422Z Reads: 216

```
Hardware version:  410, 411, 412

Firmware Version: Should only be default. Choose the one default. Correct me if i'm wrong.

Ah Ackmaniac got it first.
```

---
## \#393 Posted by: t0m_r1dd1e Posted at: 2018-05-08T13:38:13.979Z Reads: 218

```
Thanks guys. I'm familiar with VESCs and the previous version of the tool but this is my first time with focbox and this new tool. 

Does motor detection need to be totally smooth? When I put in detection config values from the old tool (6.0a, 600erpm, 0.05), I get successful detection but the second part of detection sounds rough. I've never seen detection sound like that. On stock firmware with the stock tool and the phase wires plugged into the same motor wires, everything is super smooth.
```

---
## \#394 Posted by: Bjork3n Posted at: 2018-05-08T14:15:21.034Z Reads: 216

```
Try raise duty to 0.07 or 0.10. Use a short usb cable as well. Had the same issue on the second part of detection. 
This fixed it for me
```

---
## \#395 Posted by: Ackmaniac Posted at: 2018-05-08T14:17:22.295Z Reads: 217

```
I recommend a duty cycle of 0.15. Then it runs smooth.
```

---
## \#396 Posted by: TarzanHBK Posted at: 2018-05-08T21:39:12.947Z Reads: 214

```
I did a detection today, first time failed. Raised duty to 0.10 - failed. 0.13 worked and everything was buttersmooth👍
```

---
## \#397 Posted by: t0m_r1dd1e Posted at: 2018-05-09T13:43:35.003Z Reads: 215

```
That did the trick. Thanks!
```

---
## \#398 Posted by: Benjamin899 Posted at: 2018-05-09T17:52:23.944Z Reads: 215

```
this is kinda weird but i don't even have the option to chose watt mode. all other modes are there....anyone got an idea
```

---
## \#399 Posted by: rey8801 Posted at: 2018-05-09T17:57:37.455Z Reads: 217

```
In the last firmware current mode works as watt mode
You do not need to select it anymore.
```

---
## \#400 Posted by: fraannk Posted at: 2018-05-10T13:27:15.414Z Reads: 215

```
Hi guys, I'm upgrading my friends Scramboards VESC, and I'm trying to install v3.101 on it, but it keeps saying too old firmware. Is it because of a missing bootloader? It says on Scramboards site that it comes with a bootloader :) Will I break something if I try installing a bootloader from ESC-tool?
```

---
## \#401 Posted by: amazingdave Posted at: 2018-05-11T06:54:12.363Z Reads: 212

```
I can’t get sensored detection to work no matter what I try.... (12s, bdlc, esk8.de direct fet VESC, Dark matter motor) tried the duty up to .15... nothing.
```

---
## \#402 Posted by: b264 Posted at: 2018-05-11T07:39:41.134Z Reads: 210

```
[quote="Benjamin899, post:398, topic:35116, full:true"]
this is kinda weird but i don’t even have the option to chose watt mode. all other modes are there…anyone got an idea
[/quote]

You're probably not running Ackmaniac firmware.  What version is your firmware?
```

---
## \#403 Posted by: Ackmaniac Posted at: 2018-05-11T07:52:06.294Z Reads: 208

```
Try to switch 2 phase wires so that the motor runs in the other direction. Then do the detection again. If that also doesn't work you should check the sensors via Multimeter. And also check the wires if they are at the right pins. But i also have a sensored motor that doesn't work. Checked it with multimeter and the sensors show always the "HIGH" state. On other motors BLDC mode has trouble when the sensors are slightly off.

You can also try to detect them in FOC mode which mostly works better than BLDC. The esk8 ESC shouldn't have isuses in FOC. On once you go FOC you won't go back.
```

---
## \#404 Posted by: amazingdave Posted at: 2018-05-11T08:22:44.021Z Reads: 200

```
I’ve tried switching the phases, tested the halls (they go high sequentially as I rotate the motor) and I’ve checked the pinout... esk8.de warned me that foc is not recommended at 12s.. I can’t afford to blow another VESC!
```

---
## \#405 Posted by: Ackmaniac Posted at: 2018-05-11T09:07:46.704Z Reads: 197

```
Had a look at Scramboards website and it seems that they sell maytech VESC. In this case you can upload the bootloader via the tool and then firmware updates should work. 
To use these VESC in a mountainboard isn't really a smart idea because of FOC problems at the high amps that are needed. In BLDC they should work but you will get Temperature issues.
```

---
## \#406 Posted by: fraannk Posted at: 2018-05-11T10:25:33.661Z Reads: 194

```
So the modified yellow ones is also MayTechs? The ones with a separate MOSFET board and a heatsink? :) It is not being used on a mountainboard nor in FOC, so all good. I’ll try uploading the bootloader, thanks! :slight_smile:
```

---
## \#407 Posted by: Kug3lis Posted at: 2018-05-11T10:37:36.543Z Reads: 194

```
Thinking of trying out your firmware this weekend, is there any need to know tips of using it?
```

---
## \#408 Posted by: Ackmaniac Posted at: 2018-05-11T10:42:09.839Z Reads: 189

```
All seems it is a Maytech. But you also post a picture if you want.
```

---
## \#409 Posted by: Ackmaniac Posted at: 2018-05-11T10:42:59.317Z Reads: 194

```
Most of the infos you need to know is in the first post of this thread.
```

---
## \#410 Posted by: deucesdown Posted at: 2018-05-11T11:00:01.794Z Reads: 207

```
I have some motors that behave this way. I verified halls with a oscope, and tried every combination of phase wires. Won't detect in BLDC mode.

I have some other motors that very rarely would detect in bldc mode, but one time on the road the motors would not spin. Switched to sensorless and all is well.

And I had an incident where one of my phase wires broke and I ended up frying the vesc.

Riding sensorless now and I don't miss it.
```

---
## \#411 Posted by: amazingdave Posted at: 2018-05-11T11:39:32.903Z Reads: 203

```
This firmware is working very well in sensorless, love the watt control mode... I may remove the throttle expo I have on as this doesn’t seem to be useful in watt mode.
```

---
## \#412 Posted by: Bjork3n Posted at: 2018-05-11T11:48:20.343Z Reads: 202

```
I must  agree, im running sensorless and i never have any issues when starting from a standstill.
If i start in a hill and im rolling backwards i do notice that its sensorless tough... 
Never going back to stock fw
```

---
## \#413 Posted by: Benjamin899 Posted at: 2018-05-11T13:05:47.267Z Reads: 203

```
i downloaded the tool from the link at the top from achmaniac and then i went to the firmware tab, selected hardware 410&411&412 and the vesc default.bin. I thought the firmware was included in the new tool.
```

---
## \#414 Posted by: Ackmaniac Posted at: 2018-05-11T13:08:53.629Z Reads: 200

```
In my firmware mods 3.100 and 3.101 current control is Watt control. So there is no option for watt control anymore.
```

---
## \#415 Posted by: Benjamin899 Posted at: 2018-05-11T13:11:19.259Z Reads: 199

```
yes @rey8801 already said it, but you saying it puts me at ease
```

---
## \#416 Posted by: Benjamin899 Posted at: 2018-05-11T15:21:13.089Z Reads: 195

```
do you still need to download the firmware 2.54 out of the old folder (dropbox) or just the tool and the default firmware?
```

---
## \#417 Posted by: rey8801 Posted at: 2018-05-11T15:25:00.981Z Reads: 201

```
From the tool directly. Everything inside. If you read the first posts is reported. Or at least inside the thread.
```

---
## \#418 Posted by: webst Posted at: 2018-05-11T16:26:54.280Z Reads: 199

```
Has anyone tried to update to Ackmaniac's firmware over TCP? I have like million screws to unscrew which I would happily do if this would be an alternative to unscrewing my vescs.
```

---
## \#419 Posted by: isabar Posted at: 2018-05-12T07:08:23.515Z Reads: 200

```
I have noticed that the evolve style motors have very weak hall sensor outputs.  The VESC uses 2.2 kOhm Pullup resistors, which is typical but too strong for some hall sensors, causing a hall sensor low output to actually look high.  For a low to be read as a low, it typically has to be less than 0.6V (on a 3.3V system).  For those types of motors, either run sensorless, or hybrid and you should be ok.
```

---
## \#420 Posted by: TarzanHBK Posted at: 2018-05-13T10:33:31.192Z Reads: 205

```
When you want to run in sensored, watch how your motor behaves during detection. If it spins up fine at first, then stutters at the end, rise the duty higher until it works.
Play a bit with the detection values. It should work if you play around a bit.
Sometimes it helps if you just reconnect everything new and restart the vesc.

If you want, post a video of the failed detection and we try to help you out what you can change to make it work.

I mostly get them to work, but i also had a few that doesn´t, no matter what i tried :neutral_face:
```

---
## \#421 Posted by: Eboosted Posted at: 2018-05-13T16:26:11.073Z Reads: 204

```
I'm having issues trying to connect vesc monitor to all my boards via hm10  since last update, is there anything I missed, didn't want to open the enclosures.

@ackmaniac on a previous post you said it was too difficult to detect the correct ERPM when the motors were spinning at almost dead stops, so the motors went into full brake throwing you forward. Would it possible to never go into full brake by instructing the ESC to a constant value of 1km/hr when the ERPM reads zero, so it doesn't go into full brake?
```

---
## \#422 Posted by: b264 Posted at: 2018-05-13T17:38:51.072Z Reads: 193

```
Some folks don't like putting their feet down at red lights
```

---
## \#423 Posted by: Eboosted Posted at: 2018-05-13T23:26:24.464Z Reads: 200

```
It could go into full brake after 1 second of detecting 0 km/hr, not right away which is where the the brakes lock.
```

---
## \#424 Posted by: mikenyc Posted at: 2018-05-14T00:32:21.685Z Reads: 199

```
i do both.

i also feel like my boards are inconsistent in how they brake at a red light. either they're fully locked until i let go, or they sort of have some free roll while stopped
```

---
## \#425 Posted by: isabar Posted at: 2018-05-14T07:59:16.879Z Reads: 204

```
I have noticed that if I am rolling backwards, I can't accelerate forward. Is there a setting that controls this?
```

---
## \#426 Posted by: Ackmaniac Posted at: 2018-05-14T08:24:10.247Z Reads: 204

```
I understand your idea but that won't work. Issue is that the VESC looses tracking of the motor. You can force the motor to roll with exactly 1km/h. But if the Motor isn't at exactly that speed then you have the same stutter like at start up with a sensorless motor.
```

---
## \#427 Posted by: Ackmaniac Posted at: 2018-05-14T08:25:16.683Z Reads: 203

```
Which control mode do you use? And does the motor stutter when you try to go forward while going backwards?
```

---
## \#428 Posted by: isabar Posted at: 2018-05-14T08:55:18.241Z Reads: 196

```
I am using current control with reverse (hybrid sensored). actually I realize what's happening.  When you roll backwards and try to accelerate forward, it actually brakes.  so the only way to get going forward again is to kick push and then accelerate.  it would be nice if below a certain speed, it would actually try to accelerate and not brake. otherwise you have to kick-push to get going..
@Ackmaniac
```

---
## \#429 Posted by: isabar Posted at: 2018-05-14T08:58:13.205Z Reads: 195

```
Also, I could be wrong, but it seems like on the latest  version of VESC Monitor (v1.94), when trying to switch to FOC, it doesn't actually switch.  Can you check this? Also, it would be nice if the app actually shows whether you are in BLDC of FOC mode.  Right now, you can't be sure 


@Ackmaniac
```

---
## \#430 Posted by: Ackmaniac Posted at: 2018-05-14T09:08:50.939Z Reads: 193

```
Please try to set the control mode "Current no reverse with brake" and tell me if it works as expected?
```

---
## \#431 Posted by: Kug3lis Posted at: 2018-05-14T09:43:49.702Z Reads: 198

```
I have installed firmware yesterday, works almost the same as original just several points I noticed:

* Much better start up sequence doesn't throw of the board
* Hill climbs at lower speeds are like nothing even without full throttle
* It works much better on acceleration/braking compared to original as on original I even use throttle mapping.
```

---
## \#432 Posted by: isabar Posted at: 2018-05-14T15:34:22.039Z Reads: 199

```
same issue with "Current no reverse with brake"
```

---
## \#433 Posted by: Ackmaniac Posted at: 2018-05-14T16:01:45.049Z Reads: 206

```
I mean the acceleration while going backwards.
```

---
## \#434 Posted by: isabar Posted at: 2018-05-14T16:11:36.119Z Reads: 209

```
yes, same issue with  “Current no reverse with brake” .  When rolling backwards, and trying to accelerate forwards, it brakes, but doesn't accelerate. you need  to kick push forward to get it to accelerate forward.
```

---
## \#435 Posted by: driver Posted at: 2018-05-14T18:46:16.869Z Reads: 210

```
hey guys, i was working on ym board i tried to do the detection.

Motor 1, everything runs fine... 
Motor 2 [RL] test ok, Lambda test: no movement...
Hall Sensor detection is fine.
i changed the order of the motorcables to the vesc.. with no result.
Motor 2 runs, but i have the feeling not optimal...

Do you have an idea what i could be.

![2018-05-14 20_41_15-ESC Tool|690x416](upload://wuToWFHz9hvxTLBzPFr01DvS12y.jpg)
```

---
## \#437 Posted by: Ashintar Posted at: 2018-05-14T20:23:12.047Z Reads: 204

```
Is there a way to setup your timeout behavior with a nano-x controller or am I just SOL because of it its autobind?
```

---
## \#438 Posted by: isabar Posted at: 2018-05-15T11:44:10.543Z Reads: 205

```
@Ackmaniac, Can you provide a link to where the .bin firmware file for FW 3.101 (For hardware 4.12) can be downloaded?  I am having a problem upgrading firmware via  VESC-TOOL, so I want to try via ST-Utility.
```

---
## \#439 Posted by: SeanHacker Posted at: 2018-05-15T12:28:10.805Z Reads: 205

```
https://github.com/Ackmaniac/vesc_tool/tree/master/res/firmwares
```

---
## \#440 Posted by: Koppernikus Posted at: 2018-05-25T19:30:06.364Z Reads: 201

```
Could anyone help me?
If I connect my focbox to the esc tool it says that It has to old firmware an I'm in the limited mode to update the firmware.
I downloaded the 2.54.bin from the dropbox and hit the update button in the tool. The tool shows that the fw upload is done. But the board disconnected from the laptop. If I power up the board again it shows again that I have to update the firmware and I'm in the limited mode.
Thanks for helping

Edit: if I read firmware version it shows: Fw: 2.54
```

---
## \#441 Posted by: Ackmaniac Posted at: 2018-05-25T19:37:19.421Z Reads: 199

```
The Esc tool has already the right firmware file. Just select the file for 4.10 4.11 4.12.
Then install the default file. 
Afterwards it should show version 3.101
```

---
## \#442 Posted by: SeanHacker Posted at: 2018-05-25T19:37:42.755Z Reads: 199

```
Just update within the tool. No need to download anything outside of it.

Acks fast. What he said ^^^^
```

---
## \#443 Posted by: Koppernikus Posted at: 2018-05-25T19:47:42.261Z Reads: 198

```
I tried that without the custom file. I choose the hardware version for 410 & 411 & 412 and hit the update firmware button.
Than board disconnects and after 10 sec. I unplug the power and then I powered it up again. Than I reconnect the board in the tool and I'm again in the limited mode. 
What could be wrong?

After the update is done it shows: serial port error: no such file or directory.
```

---
## \#444 Posted by: briman05 Posted at: 2018-05-25T19:58:39.046Z Reads: 197

```
I didnt have any issue when I ran the update firmware.  make sure that  show other updates along with the default box is not checked this will give you the correct file.  Are you running esc tool on mac or PC
```

---
## \#445 Posted by: Koppernikus Posted at: 2018-05-25T20:04:08.775Z Reads: 199

```
I tried it all the time with the default Version.
And I run it on PC.

Could it be that the bootloader is corrupted? Or would I recognize it if the bootloader Isn't working?
```

---
## \#446 Posted by: Ackmaniac Posted at: 2018-05-25T20:26:20.394Z Reads: 197

```
Did you install the bootloader via the Esc tool. Because you shouldn't do that. The focbox comes with a bootloader pre-installed. If that's not what you did then maybe try it with another computer.
```

---
## \#447 Posted by: Koppernikus Posted at: 2018-05-25T21:31:16.927Z Reads: 196

```
It could be that I accidentally tried something in the bootloader field... I think if the bootloader works properly than the focbox turn of after the update and then he should boot up on his own. Am i right? Mine isn't doing that. 
So I think I need to install a new bootloader. But tomorrow i will try it on another PC.
```

---
## \#448 Posted by: Ackmaniac Posted at: 2018-05-25T22:10:37.433Z Reads: 196

```
I think when you messed up the bootloader then you have to flash the focbox via Stlink.
```

---
## \#449 Posted by: Koppernikus Posted at: 2018-05-25T22:22:28.499Z Reads: 201

```
Yes i already Orderd a Stlink.
And on Money i'll try to do that according to that thread:
http://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103

Is that still up to date?
```

---
## \#450 Posted by: Janosh Posted at: 2018-05-26T03:09:59.393Z Reads: 201

```
I have a question about the cruise control and could not find anything helpful so far.
Is it possible to use the Alienpowersystem remote? I don't like the Mini remote and don't want to use a remote with a steeringwheel or the nunchuck
I would prefere just to click a button on the remote.
```

---
## \#451 Posted by: skatardude10 Posted at: 2018-05-28T08:36:32.901Z Reads: 205

```
I notice a difference in breaking with this firmware since changing from 3.100 to 3.101. 

On 3.100, breaking was only very strong at low speeds, never at higher speeds. 

Now though on 3.101, when I first start riding, I get *very* strong breaks at all speeds. This can be a little crazy going 30+ and having such sensitive breaks. I almost feel like I should be worried I am overloading things, but checking the logs, I am not sending more amps back to the battery than I have set. Oddly enough though, once the board gets warmed up a bit, the breaking sensitivity calms down to a much more manageable level at high speeds, but it remains still quite strong at slower speeds. Usually only 5-10% of my ride is spent during that "warm-up" period where breaks are super sensitive.

I don't know if this is a quirk with my setup, the firmware, or if this is how this is supposed to be... but I can live with it for sure- I kind-of like it, and now I have a reason to adjust my breaking curves.
```

---
## \#452 Posted by: Ackmaniac Posted at: 2018-05-28T08:42:00.818Z Reads: 194

```
On 3.101 the brake for the slave motor was fixed so that it brakes at the same amount as the master. Depends on your previous settings how much the difference is but now with 3.101 it brakes equal. Of course it is important that you have the same settings on master and slave. If you want your brakes a bit weaker at high speeds then reduce your batter min (regen).
And if the brake force is too strong in total you should reduce the motor min.
```

---
## \#453 Posted by: b264 Posted at: 2018-05-28T08:43:37.847Z Reads: 203

```
[quote="Ackmaniac, post:452, topic:35116"]
If you want your brakes a bit weaker at high speeds then reduce your batter min (regen).
[/quote]

_increase_ the battery minimum

So, like for example "-25" to "-20"
```

---
## \#454 Posted by: skatardude10 Posted at: 2018-05-28T08:43:56.176Z Reads: 203

```
Ah! That explains it :P
```

---
## \#455 Posted by: Benjamin899 Posted at: 2018-05-28T09:56:26.966Z Reads: 205

```
Yeah that was something i had to get my head around. Your way of thinking is mathematically correct.
```

---
## \#456 Posted by: rey8801 Posted at: 2018-05-29T09:31:41.980Z Reads: 216

```
Hi! I just finished remake my enclosure (fiberglass) and I took the oppurtunity to upload to 3.101 firmware during the process. I used the same parameter as before, but this morning I noticed that when I go full throttle on the fast mode (Nano-x remote) the board loses power for one second. I din't have it this problem before, never had a single drop of signal or power. If I ride in the low speed mode that won't happen. It's sound like some current or watt limit reached but by the chart I am far away from the limit, moreover I never had in the past 1 month and a half that I used the board.
Do you know what It could be? It's quite scary! Thx a lot

![vescmonitor|281x500](upload://zPMXNYPjASWpO4ZRtwGU6Bq3QyW.png)![Picture1ss|280x500](upload://4dvjOdChHXKsMz1tdxbUgGEXo6.jpg)

PS: In the chart you can see when it happend.

Setup:
Diyeboard 90mm hubmotor
2 Maytech VESC
10s3p 30Q battery
Nano-x remote
60A BMS
```

---
## \#457 Posted by: Ackmaniac Posted at: 2018-05-29T09:38:14.558Z Reads: 205

```
Are you sure that you adjusted you ppm pulsewith with the fast mode active?
```

---
## \#458 Posted by: rey8801 Posted at: 2018-05-29T09:43:39.156Z Reads: 224

```
F......K me!!!! You are right!!!! ahahaahh Sorry sorry Sorry :smiley:

That's what happen when yuo set things at 3am...
```

---
## \#459 Posted by: Ackmaniac Posted at: 2018-05-31T20:52:34.155Z Reads: 230

```
**Just released the new Version 3.102:**
- Fixed bug where motor did spin backwards when motor max is lower than motor min.
- Cruise control now takes latest motor amps to start the PID controller instead of starting from zero. 
This way cruise control starts extremely smooth when you accelerate up a hill (or at braking (only NRF)). If you did hold a constant speed uphill before activating cruise control you won't even recognize that it became active. Old behavior always started form 0 and tried to balance the speed. But till you got there you lost already a lot of speed uphill. This way the PID controller could be set up less responsive so that it is even smoother at carving.
- Small change for start of sensorless openloop to take latest detected position instead of position of last calculation. (guess it's not recognizable)

A easy way to update is to following:
- connect to the ESC
- read motor congig
- read app config
- update the firmware
- connect again after 10 seconds
- write motor config
- write app config

then do the same for the slave if it exists. It is important that you don't close the application in between.
or you can save the config via the menu in a xml file and the read it again after you flashed the firmware.
```

---
## \#460 Posted by: b264 Posted at: 2018-05-31T21:16:44.127Z Reads: 221

```
[Version 0.82/3.102 built for Linux](https://github.com/b264/vesc_tool/tree/e05770c4211a02a2c61b03b4b42616d0d1c31183/build/lin)
```

---
## \#461 Posted by: Ebisane9 Posted at: 2018-05-31T23:31:34.830Z Reads: 219

```
mac app always crashes so this is kinda difficult. I've sent numerous error logs in
```

---
## \#462 Posted by: Ackmaniac Posted at: 2018-06-01T00:01:28.866Z Reads: 222

```
Which mac App?
```

---
## \#463 Posted by: Ebisane9 Posted at: 2018-06-01T00:02:22.957Z Reads: 224

```
The compiled Vesc tool
```

---
## \#464 Posted by: Ackmaniac Posted at: 2018-06-01T00:03:34.916Z Reads: 230

```
You mean while firmware update? Yeah that happens. I don't have a MAC so i can't really analyse. If you have a error log that could help. Never seen one.
```

---
## \#465 Posted by: Ebisane9 Posted at: 2018-06-01T00:06:11.516Z Reads: 226

```
During update and anytime the Vesc is rebooted. The Mac application will restart. I’ll see if i can access a log the next time I’m playing around with my vescs
```

---
## \#466 Posted by: SeanHacker Posted at: 2018-06-01T00:43:56.602Z Reads: 225

```
Is this just a ESC-Tool update to Version 3.102? Or Firmware? I'm still getting 3.101 in version 3.102 when flashing the firmware. 

![Screenshot from 2018-05-31 17-40-27|690x434](upload://lRPp85Dd4qfxIxHkSEDhOUMO89H.png)
```

---
## \#467 Posted by: SeanHacker Posted at: 2018-06-01T00:45:03.797Z Reads: 217

```
Tried it out. But it immediately closes when trying to connect. Thanks for compiling this though dude.
```

---
## \#468 Posted by: Ackmaniac Posted at: 2018-06-01T00:55:53.010Z Reads: 215

```
Saw that also by now, seems that i mixed something up with the exe file. Will fix that soon.
```

---
## \#469 Posted by: SeanHacker Posted at: 2018-06-01T00:56:17.289Z Reads: 220

```
Thanks dude!
```

---
## \#470 Posted by: Ackmaniac Posted at: 2018-06-01T01:22:51.908Z Reads: 222

```
Strangely having problems compiling the version with the icon for the tool. So i just added the version without the icon for the moment. Firmware doesn't care about the icon so you can use this one without issues.
Will try to fix the icon version tomorrow.
```

---
## \#471 Posted by: Ebisane9 Posted at: 2018-06-01T01:32:26.349Z Reads: 220

```
guess i gotta download windows for this here macbook
```

---
## \#472 Posted by: SeanHacker Posted at: 2018-06-01T01:33:13.654Z Reads: 218

```
Did you already upload it? Looks like the same version as before.
```

---
## \#473 Posted by: Ebisane9 Posted at: 2018-06-01T01:37:21.875Z Reads: 220

```
Does this VESC tool work on windows 10 as well?
```

---
## \#474 Posted by: SeanHacker Posted at: 2018-06-01T01:38:54.075Z Reads: 219

```
I'm pretty sure it should. I haven't run windows in a decade so I'm pretty out of date with it. I just run a vbox using windows 7 when I need to update firmware.
```

---
## \#475 Posted by: Ebisane9 Posted at: 2018-06-01T01:39:40.930Z Reads: 223

```
Nice i just got vbox and i plan on using that, do i have to switch off live monitoring or something like that for it to work? i remember someone having an error using a virtual machine
```

---
## \#476 Posted by: SeanHacker Posted at: 2018-06-01T01:45:48.880Z Reads: 227

```
Yep. That was me. Ack figured out that using the heartbeat causes some issues when running a vbox. So turn that off when you don't need it because it consumes a lot of the connection.
```

---
## \#477 Posted by: briman05 Posted at: 2018-06-01T03:18:50.833Z Reads: 224

```
My Mac would freeze when I updated the firmware. And I have a solid state drive and upgraded ram so it shouldn’t freeze.
```

---
## \#478 Posted by: Ackmaniac Posted at: 2018-06-01T07:44:20.953Z Reads: 232

```
The file was ok, but now i replaced it anyway with the icon version.
Have fun.
```

---
## \#479 Posted by: SeanHacker Posted at: 2018-06-01T13:15:08.436Z Reads: 235

```
Works now. Thanks again dude!!!

![Screenshot from 2018-06-01 06-40-36|690x291](upload://a4xxWt7whLOngIK3yvxPpa0IPmt.png)
```

---
## \#480 Posted by: Ebisane9 Posted at: 2018-06-01T14:19:43.136Z Reads: 236

```
where did you get windowa 7? do i need cd or iso? microsoft only has windows 10 for free and it seems like bootcamping it is easier...
```

---
## \#481 Posted by: SeanHacker Posted at: 2018-06-01T14:30:52.813Z Reads: 236

```
Here's a version of 3.102 compiled for you linux users out there. 

https://github.com/task650/ackmaniac_esc_tool_linux/blob/master/Version_3.102_Linux/ACKMANIAC-ESC-Tool_Linux

P.S- I totally forgot to set the permissions to executable before upload so just right click it, go to properties, select permissions tab, and then check the Allow executing as a program box. Or just run from terminal like I do. ;)
```

---
## \#482 Posted by: SeanHacker Posted at: 2018-06-01T14:43:04.083Z Reads: 234

```
Sent you a PM.
```

---
## \#483 Posted by: rene Posted at: 2018-06-06T08:08:33.747Z Reads: 232

```
I scanned the whole thread - and found only one mention of VESC 6.

So I am unsure if i could fry my VESC 6. 
Does it work on VESC?
```

---
## \#484 Posted by: Ackmaniac Posted at: 2018-06-06T08:23:42.776Z Reads: 231

```
Should work. Don't use the Cruise via secondary channel for PPM remotes with the VESC 6 (2nd channel connected to slave to give the Cruise control command). Because the ground loops can brake the VESC 6 Hardware. 4.12 Hardware seems to be fine with it. But not many use this feature anyway (I love it).
```

---
## \#485 Posted by: rene Posted at: 2018-06-06T08:26:24.403Z Reads: 234

```
Thanks for the prompt answer.
I am riding eMTB - no cruise control needed.
Just nice WATT mode wanted.

Gruss aus HH!
```

---
## \#486 Posted by: Ackmaniac Posted at: 2018-06-06T08:35:53.307Z Reads: 226

```
Moin Moin :hamburger:
```

---
## \#487 Posted by: rey8801 Posted at: 2018-06-06T08:55:43.207Z Reads: 230

```
Hi, one question it's possible to check for DRV faults on slave vesc while I am connecte to ACKMANIAC-ESC Tool via TCP with your app? I am able to read nad write, detect the slave parameters, I was just wonering whether it's also possible to detect faults? the problem is that since 2 weeks the board acts a bit weird, Sometimes I feel like half of the power is gone and then suddenly it comes back. Tnx
```

---
## \#488 Posted by: rene Posted at: 2018-06-14T17:00:31.418Z Reads: 224

```
Do you plan to integrate the BLE feature of Roman for the Metr Pro Module?

It would also be a great feature for the FW update process to first copy the settings of each VESC and than restore the settings back. motor and app :slight_smile:
```

---
## \#489 Posted by: petter Posted at: 2018-06-17T10:11:48.454Z Reads: 226

```
Soo, I have been trying for some time to get this linux version up and running. 

The normal vesc tool is just a download and then it works, this one however keeps asking for a lot of libraries, mostly from QT.

Since i had a 32bit ubuntu for some legacy reason, i started with getting 64bit debian, then getting QT, then it wanted the newest 2.27 libc thats not in stable in debian so i switched the sources to buster, the testing branch. then it's wanting some plugin, xkc? xkb? Was going about looking for that one when i also was running an upgrade to the buster repo and somehow the installation got messed up so i had to start over. So i feel pretty done with messing with that, any thoughts on this? I was thinking maybe i'll just try compiling it myself

Update: So testing @b264 version i got the same results, could start it without problem but got  "QMetaObject::connectSlotsByName: No matching signal for on_actionESCToolChangelog_triggered()
QObject::connect: No such signal Commands::nrfPairingRes(int)
QObject::connect:  (receiver name: 'nrfPair')
Segmentationfault" on trying to connect.

So i started with nothing and i got most of it left!

Update again:
Alright, so i managed to compile it at it all works now! Man i wish that i would have started with this instead haha.. well, hopefully i learned something
```

---
## \#490 Posted by: b264 Posted at: 2018-06-17T20:12:55.831Z Reads: 209

```
The last version I made didn't work for me, either.  If you make one that works, you should post to github and link from here ;-)
```

---
## \#491 Posted by: mikenyc Posted at: 2018-06-17T20:25:45.222Z Reads: 212

```
I've built a version for Mac, however the release folder contains a bunch of header files. Can I share the compiled application without having to include all of those files? @Ackmaniac
```

---
## \#492 Posted by: b264 Posted at: 2018-06-18T00:09:53.112Z Reads: 209

```
The license says the source code must be included or available upon request.  So unless you want to provide a way to get it, it's easier to include it.  Header files are source code.
```

---
## \#493 Posted by: mikenyc Posted at: 2018-06-18T00:25:12.249Z Reads: 210

```
Yeah, I don't know if it'll run on an environment other than my own.
```

---
## \#494 Posted by: petter Posted at: 2018-06-18T21:32:02.257Z Reads: 215

```
Well, here ya go:
https://github.com/skrutt/Ackmaniac-VESC-tool-build

It's a mess for now, but the compiled binary is in the release folder. i really, really, really hate git for "quick uploads"! Fucking melts my brain, just upload the damn files!!

I was looking at a static linked version, i guess thats what the original vesc tool does? since it's so much bigger and does not ask for any files? I think i could do one of those but it's probably not right according to any open source licenses  so i didn't try it.

Edit: If you try it, tell me if it works :) I might try to maintain a somewhat stable linux version since i want one for myself aswell, and sharing that with others is always fun. Should be simpler also to get it working for others than my own luck trying to get it running!
```

---
## \#495 Posted by: skatardude10 Posted at: 2018-06-19T00:44:43.235Z Reads: 209

```
Trying out PID no acceleration... I select the mode from the BT app, but it doesn't seem to change to the mode I select, or at least behave like I would expect PID no acceleration to work... It just works like current mode regardless. Changing modes works otherwise.

Do I need to configure PID mode in ESC Tool before being able to select it in the app?

Once configured (assuming that's why it doesn't work), can I still swap between PID no acceleration and regular current mode in the app?
```

---
## \#496 Posted by: b264 Posted at: 2018-06-19T05:00:26.957Z Reads: 205

```
Did you write the changes?
```

---
## \#497 Posted by: skatardude10 Posted at: 2018-06-19T05:17:43.063Z Reads: 216

```
I looked through the tool, but for now I don't want to change from current to PID no acceleration in ppm tab, since I prefer current control as my primary. I only tried to make the changes in the BT app, to PID no acceleration from current control. 

Since this didn't work, I will mess around with my ppm settings and ppm mapping tomorrow, and see if changing PID no acceleration to my primary and switching to current control in the BT app will work instead of vice versa.

**Edit:**  I just tried changing to PID no acceleration... it's sweet! I'd love the option to change to this on the fly... But changing to current control mode in the app doesn't work, I am stuck with only PID no acceleration- unable to change back to current control. PPM mapping for current control and PID no acceleration seem to be exactly the same in the ESC tool on PC, so any changes there don't have any effect. 

This might have more to do with the ESC Monitor app at this point... I think I may have found an indication of the problem: Inside the top left box in ESC Monitor (the mode box), I am pretty sure it normally indicates what mode you are in- such as current, current no reverse, Duty, PID, PID no Acceleration, or disabled. No matter what I set my modes to in the ESC Monitor app, when I select the modes i've setup (regardless of control mode), the box always just reverts to disabled, while seeming to default to whatever control mode i've set in ESC tool on the PC, while watt limits, amps, etc all take effect just fine. Maybe if I just disable control modes on the computer, the app will allow me to select a control mode? I'll have to try this tomorrow, it's getting late. Regardless, if I remember correctly, I think the ESC Monitor app used to show the control mode type in the mode screen instead of always saying "Disabled" and reverting to the control mode type from ESC tool.

**Edit 2**: Disabling control modes in ESC Tool made no difference, must be the app... going to make a post there with more details.
```

---
## \#498 Posted by: Ackmaniac Posted at: 2018-06-19T06:42:18.508Z Reads: 206

```
@skatardude10 Looks like you are connected to the slave via the app. If the module is physically connected to the master then you enabled the option in the app to connect to the slave via CAN.
If the module is physically connected to the slave then you need to enable the option in the app to connect via CAN. 
Ppm mode changes only work for the master while current and watt limits can be overwritten also for the slave.
```

---
## \#499 Posted by: skatardude10 Posted at: 2018-06-19T13:42:39.974Z Reads: 200

```
Ah, this makes sense! Thanks for the explanation ack 😎
```

---
## \#500 Posted by: skatardude10 Posted at: 2018-06-20T00:20:51.894Z Reads: 212

```
1: Wait, if slave control mode is set to only uart and takes commands from master (BT connected to master), then why won't changes to control mode  for master work and slave just mirror it since master is just sending data to slave to replicate?

2:  **Solved! It's my nano-x calibration routine!!!**
> I still have the symptom where brakes are very strong starting fresh, regardless of speed to a certain point. If I ride up to higher speed though, everything works as expected. I don't have any issues if I spin my wheels full speed forward and reverse though before hopping on my board. If I spin the wheels full speed both directions, then braking power works as expected. Having the super duper strong brakes symptoms seems 100% linked to how fast the wheels have spun or not since starting up the board. 

3: Have you or anyone here tried using Vedder's vesc tool Android APK to modify firmware settings outside the app? I'm guessing I'd need to flash my HM-10 clone with new firmware for it to even work... I'm wondering if it will ask me to update to the latest VESC tool firmware I stead of your own before making any changes... I'm just trying to think of alternatives to swapping PPM control modes on my setup short of hauling my laptop in my backpack to reprogram it on the road (panel mounted USB on the enclosure is nice, but not *that* nice).
```

---
## \#501 Posted by: deucesdown Posted at: 2018-06-20T00:27:18.616Z Reads: 208

```
[quote="skatardude10, post:500, topic:35116"]
brakes are very strong starting fresh,
[/quote]

Sounds like the well known nano x calibration issue
```

---
## \#502 Posted by: skatardude10 Posted at: 2018-06-20T00:30:02.806Z Reads: 206

```
OH!!!!!!!!

That is it!!!!!!!! I totally forgot about that!!!! I don't calibrate my nano-x every time I start my board!!!!

 I always turn on the board, then the controller. It should be controller first, full throttle, full brake, then turn on board.

**Thank you so much for reminding me!**
```

---
## \#503 Posted by: deucesdown Posted at: 2018-06-20T00:30:38.832Z Reads: 208

```
Haha where's my like? :)
```

---
## \#504 Posted by: Sender Posted at: 2018-06-20T00:31:49.391Z Reads: 203

```
Man it really does some weird shit if you don't calibrate it.... I don't like that at all...
```

---
## \#505 Posted by: skatardude10 Posted at: 2018-06-20T00:31:53.082Z Reads: 207

```
**BAM** *101010*.... Got ya
```

---
## \#506 Posted by: Ackmaniac Posted at: 2018-06-20T06:27:35.531Z Reads: 211

```
It works via the app. So you did connect the module to the master, right? Then check in the app settings of you activated to connect via CAN. If yes then you need to deactivate it because you are already the master. If you still don't see modes then check if your master sends his status via CAN in the vesc settings? That needs to be deactivated. Only the slave should send it's status. When all of this is setup correct then you will be able to change the control mode via the app.
```

---
## \#507 Posted by: skatardude10 Posted at: 2018-06-20T13:59:35.361Z Reads: 215

```
Ah! I do have BT connected to master... And I selected connect to CAN ID 1 in the app. Only slave sends status from ESC tool... Makes sense that I shouldn't select connect to CAN ID 1 in the app. I'll try this tonight, thanks!

**Edit**: that was the issue! I was in the middle of compiling your ESC tool for Android so that I could boot the app, use a Bluetooth mouse on the go to use the full desktop tool on the go connected via tcp to the app to change modes on the fly but this is obviously a million times better. Thanks man!
```

---
## \#508 Posted by: Titoxd10001 Posted at: 2018-06-20T22:41:50.119Z Reads: 218

```
Im having issue connecting esc monitor app to focbox with .102 firmware. Bluetooth connected to master with ppm and uart enabled. App seems to be working fine with other board with .100 firmware. Anyone else having this issue?
```

---
## \#509 Posted by: Ackmaniac Posted at: 2018-06-20T23:01:41.002Z Reads: 219

```
Check the wires (RX to TX and TX to RX) and baudrate od 9600 for standard modules. The BLE module should be connected to 5V.  If you have android 8 then not all bluetooth modules will work.
```

---
## \#510 Posted by: Titoxd10001 Posted at: 2018-06-20T23:36:53.105Z Reads: 232

```
Okay, so it seems like 2 out of 3 of my Bluetooth modules don't connect. One of those use to connect but that's was probably last year before a Android update maybe? My oldest bluetooth module still works, the two newer ones look the same. So I need to get new modules. Thanks.
```

---
## \#511 Posted by: Ackmaniac Posted at: 2018-06-20T23:47:18.628Z Reads: 233

```
or if you have a Arduino you can update them with new firmware. In my app thread there is more info about it.

http://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/710?u=ackmaniac
```

---
## \#512 Posted by: Titoxd10001 Posted at: 2018-06-21T02:11:39.270Z Reads: 232

```
Damn. That's out my skill set. Wonder if anyone would do this in the US.
```

---
## \#513 Posted by: celica39 Posted at: 2018-06-22T01:18:00.757Z Reads: 230

```
hey ,ackmaniac  can you tell if i need the boot loader +firmware to load the 3.102 with my 4.12 vesc because right now i have done 
everything right and my new vesc work but the old one as a problem i never see  , the trottle not respond at all in forward motion but work only backward with 2 push back of the trottle thanks
```

---
## \#514 Posted by: celica39 Posted at: 2018-06-22T02:43:55.627Z Reads: 224

```
problem solve  i have reinstall the default  bootloader and firmware  2.18 with the st-link programmer tool and then upgraded to 2.59  then 3.102 !! both with the usb  ! piece of cake !:smile:
```

---
## \#515 Posted by: Moza Posted at: 2018-06-22T19:54:54.631Z Reads: 219

```
Hi. I am using the ackmaniac vesc monitor with andoid 6 with a hm-10 bluetooth module. Everything is great except I cant change between the modes. I want to restrict the scooter for my kids. I can set the modes up but when I click the box and select a different mode it just remains on default and nothing changes. Does anyone have any ideas please?
```

---
## \#516 Posted by: Ackmaniac Posted at: 2018-06-22T20:13:33.426Z Reads: 208

```
Please make a Screenshot after you changed the mode and a Screenshot of your settings first screen. And do you have my firmware mod or the original firmware?
```

---
## \#517 Posted by: celica39 Posted at: 2018-06-22T23:25:31.656Z Reads: 209

```
hi ,ackmaniac yes lot of change for me  there but again another problem occur and when i put my tx off ,the motors start spinning at full trottle and  i don't have failsafe on my rx .  and its to dangerous to ride like that , the time out is set to 1000ms  right now .
```

---
## \#518 Posted by: Ackmaniac Posted at: 2018-06-23T00:06:35.058Z Reads: 209

```
which remote do you have. pretty sure there is a way to adjust the failsafe.
```

---
## \#519 Posted by: celica39 Posted at: 2018-06-23T02:18:41.659Z Reads: 205

```
![20180622_221814|281x500](upload://7mWcmtvws1YSDAaCURu1R8sgCUm.jpg)
```

---
## \#520 Posted by: celica39 Posted at: 2018-06-23T02:34:13.368Z Reads: 196

```
no buton for failsafe  but maybe a rebind gonna work  , i will try
```

---
## \#521 Posted by: isabar Posted at: 2018-06-23T05:49:24.278Z Reads: 197

```
I am trying to get a better understanding of when watt-hour data gets rezeroed on the VESC and on the app.  I know that every time the VESC is power cycled, the displayed DISTANCE and WATT-HOUR data on the app are rezeroed. However, I noticed that the estimated remaining RANGE seems to use WATT-HOUR data that is not rezeroed when board is power cycled.  This is a good thing, because obviously you may turn off your board mid-ride and not want to lose that data.

So my questions:
1) When is Watt-hour data actually rezeroed (regardless of what's displayed on the app)?  Is it when battery voltage is let's say about 41.9V (an indication that a 10S battery has been fully charged)?

2) Since the consumed Watt-hour data seems to be saved after powercyling the board (as indicated by remaining range), why are you not displaying this non-zeroed data in the app?  It would be nice if the app showed remaining battery capacity based on remaining Watt-hour (not voltage as it does now which is a lot less accurate). In other words, let's say you define the pack as having 100 Watt-hours in the app, and you have consumed 25 watt-hours, then the app should show that you have 75% battery left.  and this data should not be lost or rezeroed upon powercycling.  The only time that this data should be rezeroed is when battery voltage goes above let's say 41.9V (indicating the battery has been fully charged).

Please consider these changes to the VESC firmware/ app, as it would make the battery gauge a lot more accurate.  Is there any reason this hasn't been implemented already? @Ackmaniac
```

---
## \#522 Posted by: isabar Posted at: 2018-06-23T05:53:26.907Z Reads: 187

```
after rebinding your remote, when you pull the bind plug out of the receiver, it will use that state as the failsafe, so adjust the white knob (labeled TH trim) on the remote and  be sure the motor is not moving or braking, and then pull out the bind plug and this state will be remembered as the failsafe.  you can verify this by turning the remote off and making sure the motor doesn't move or brake.
```

---
## \#523 Posted by: celica39 Posted at: 2018-06-23T06:12:51.189Z Reads: 197

```
Yes thanks  l already done it l forgot to reply . for your battery board gauge  if you want a device more accurate device use wattmeter like me and you can disconnect the side load when you want to cut power and the lcd come with a led so its very nice at night also and give perfectly the real amount of mah used of the battery! And watt hour. Time rided . voltage , and only used the ackmaniac app for set my speed or power..![15297344164651060823928|690x388](upload://bSxPjFadpHlA3ML2rAKxm9clMzA.jpg)![20180623_021226|690x388](upload://9YpLdORwLZVVysAfH0P7Yke3VuZ.jpg)
```

---
## \#524 Posted by: isabar Posted at: 2018-06-23T06:40:02.748Z Reads: 193

```
Yes I have used that kind before, but that particular couloumeter also loses all data upon powercycling.  anyway the VESC has the ability to report the same data and why add additional hardware, if the VESC can do it all?  just need to change the firmware/app to report this data.
```

---
## \#525 Posted by: celica39 Posted at: 2018-06-23T06:52:06.765Z Reads: 190

```
i think it's a hardware limitation  not the app limitation  ,for now i trust the old school way with this wattmeter  lol ,
```

---
## \#526 Posted by: Moza Posted at: 2018-06-23T07:17:35.111Z Reads: 203

```
![P_20180623_081140|375x500](upload://rostcATJ8pk8EtEGBYJXvFv1Zof.jpg)![P_20180623_081151|375x500](upload://8GzhpPIZrDg6wq6OnenbAoT1plK.jpg)![P_20180623_081204|375x500](upload://2hjwErmgMNKm0sOdBAjTh0zs0kX.jpg)![P_20180623_081257|375x500](upload://cxspvdFcDbEpBD8ucKDPXjtmWe.jpg)I'm using your firmware for vesc 4.12 (3.102)
```

---
## \#527 Posted by: celica39 Posted at: 2018-06-23T08:30:11.434Z Reads: 196

```
anyway its fun on the go, much more smoother on 3.102 sensorless motor  but the app no keeping the data when i do  the power cycling  and bugging like crazy if i use gps data 
i am not complaint here because ackmaniac is working thousand of hours to fixing update and bug
```

---
## \#528 Posted by: Ackmaniac Posted at: 2018-06-23T09:49:01.348Z Reads: 206

```
You are not connected to the master via the app. In the settings of the app you can select if you want to connect via CAN to another vesc. So if the module is connected to the slave you need to connect via CAN to the master. If the module is already connected to the master then disable that checkbox. 

![Screenshot_20180623-114530|250x500](upload://aWNOMguEabi71CqVlkv9jvLxDax.png)
```

---
## \#529 Posted by: Moza Posted at: 2018-06-23T11:34:27.932Z Reads: 199

```
I only have 1 vesc and the CA
N box is unchecked. It appears that I can read all the data but cant change any if the parameters
```

---
## \#530 Posted by: Ackmaniac Posted at: 2018-06-23T11:42:16.589Z Reads: 206

```
Which firmware do you use? 
If you use mine then please check that "Send CAN Status" is disabled.
![image|690x459](upload://c6gPwwVWXzojkquv2cjyDt7ysMv.png)
```

---
## \#531 Posted by: Moza Posted at: 2018-06-23T11:50:39.435Z Reads: 196

```
Its yours 3.102.  the box is unchecked however the "Can status rate" shows 100Hz. The Baud rate is the same as yours at 500k. Could this be the problem?
```

---
## \#532 Posted by: Moza Posted at: 2018-06-23T12:07:45.670Z Reads: 201

```
Also I am using adc and uart as scooter has a throttle. Could there be a conflict issue?
```

---
## \#533 Posted by: Ackmaniac Posted at: 2018-06-23T14:15:38.317Z Reads: 197

```
That's the problem. The mode changes only work with NRF, Nunchuk and PPM. I never tested with ADC so i also didn't enable mode changes for ADC.
```

---
## \#534 Posted by: Moza Posted at: 2018-06-23T14:59:39.435Z Reads: 208

```
Thank you. Really grateful for your fast responses. At least I know the problem now. I will just change settings with usb. 

If you are interesting in testing mode changes whilst adc is enabled I would be happy to use my setup and report back on my experiences?
```

---
## \#535 Posted by: Ackmaniac Posted at: 2018-06-23T16:40:53.810Z Reads: 216

```
You can also connect with the PC to the vesc via the app.

https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/646?u=ackmaniac
```

---
## \#536 Posted by: Moza Posted at: 2018-06-23T21:07:32.765Z Reads: 216

```
That is cool. Just tried it now. I successfully changed parameters without using usb. Thanks for the advice. 

Its really useful so when kids are on it I can restrict top speed and acceleration. However, when adults want to play I can make things more fun without having to plug in.
```

---
## \#537 Posted by: isabar Posted at: 2018-06-24T07:27:04.414Z Reads: 212

```
Is there a reason you don't just integrate the ability to change all parameters/do motor detection via the app directly?  The TCP feature is really nice, but seems like the slam dunk would be to have it all done via the app.
```

---
## \#538 Posted by: webst Posted at: 2018-06-24T09:37:56.636Z Reads: 218

```
It believe you can if you have metr.at app and module. Don’t know about ackmaniac’s app. Not a problem imo, how many times you do motor detection?
```

---
## \#539 Posted by: Ackmaniac Posted at: 2018-06-24T11:47:55.962Z Reads: 214

```
Normally you do that once and that's it. Of course it could be done via the app but i am not really interested. And as you said it could be done via the App with a TCP connection.
Maybe in the future.
```

---
## \#540 Posted by: isabar Posted at: 2018-06-24T12:38:48.272Z Reads: 207

```
it just would create a simpler interface to do everything via the app.  yes the app is great, but why not take it to the next level..
```

---
## \#541 Posted by: skatardude10 Posted at: 2018-06-24T14:11:56.266Z Reads: 211

```
An easier approach for him might be to setup an Android build environment for his ESC tool. I might end up doing this just for ttheheck of it. I quit mid setup because I figured out the app could do what I wanted, I just had the wrong settings in the app that prevented me from changing modes. Having the full ESC tool on Android I'd pretty cool, then you can do a TCP connection from there directly to the app via 127.0.0.1 all on the same device, no extra work required besides setting up Android compilation.
```

---
## \#542 Posted by: isabar Posted at: 2018-06-24T14:58:57.367Z Reads: 210

```
can you someone post a link to where VESC-TOOL 3.102 for windows can be downloaded?
```

---
## \#543 Posted by: Yoxcu Posted at: 2018-06-25T19:51:57.483Z Reads: 220

```
Hi, i am having a Problem while breaking downhill and i think it is related to riding faster than my setup is capable. 

I did my Motor setup right and have been riding the board >200km. Running in FOC on a single focbox 10s4p 30Q's // 200kv APS motor //normaly the board tops on ~40km/h fully charged // battery min -15A // bestech BMS charge/discharge 20/80A

I was riding  41km/h downhill and wanted to brake slightly but they were super strong and cut out immediately. I tried it 3 times more and it was the same behavior. After the incident i checked the logs and the battery min was -24,5A

So my question is how is it possible for the vesc to break on -24,5A while the setting was on -15A

Thanks in advance![Screenshot_20180625-213250|281x500](upload://kCrnTT8CV29IAZgzu70WUlSlQcc.png)![Screenshot_20180625-215249|281x500](upload://iKBDPALswj8IZjTMYlgYhqgnxDk.jpg)
```

---
## \#544 Posted by: Ackmaniac Posted at: 2018-06-25T20:48:13.018Z Reads: 209

```
Well hard to tell a i see that the first time. Maybe you were going faster than your topspeed you could reach with 95% duty cycle. Could be that the board board acts strange in this situation.
But please also check in the app settings that you didn't accidently st the number of motors to 2.

If you could provoke that situation again and make a video with the app(would be enough when you leave the phone in your pocket). Maybe you can also share your log file to investigate a bit better.
```

---
## \#545 Posted by: koralle Posted at: 2018-06-25T21:28:37.751Z Reads: 219

```
This issue resulted in me breaking my foot a few weeks ago. Still not sure how I can make this more well known among new builders. Posted on the vesc-project forum and ppl said well don't go faster than your boards top speed then. (apparently theres not really a lot to be done) I think a very soft auto braking feature would be nice when you go near and above your top speed. @chaka said you should just continue holding your throttle on 100% then your speed will be limited to your board's max speed even when going downhill. I have not tested this yet because my foot is not fully healed but in the vesc-project forum nobody said it was a bad idea. You are at least the third person reporting this phenomenon so by now I am finally sure I wasn't just imagining things.
I'll post into the wiki at least.
```

---
## \#546 Posted by: koralle Posted at: 2018-06-25T21:41:31.546Z Reads: 215

```
It only happens on some setups/vescs/firmwares dunno. Frank from @trampa actually tested this on his board and said he was able to brake normally without any issues.
```

---
## \#547 Posted by: Yoxcu Posted at: 2018-06-25T22:06:47.807Z Reads: 214

```
My first thoughts were that the BMS is cutting off but then there should be at least an over voltage/any fault. But the breaks were super strong even on the slightest throttle move...

@Ackmaniac i was certainly faster than 95% duty and number of Motors is set to 1 and here is the [Logfile](https://yoxcu.de/uni/longboard/2018-06-24_14-00-59_Link_esc_Data.csv).
I can try to ride the hill again but only in 2 weeks when i'm home again

I will also try @koralle / @chaka 's hint holding the throttle at 100%
```

---
## \#548 Posted by: Ackmaniac Posted at: 2018-06-25T22:49:28.325Z Reads: 212

```
Just had a look at the logs and it happened when you had more than 95% duty cycle. In that moment the vesc tried to apply 95% which resulted in a voltage difference that leaded to the higher brake current.
My advice, change your gearing so that it doesn't happen again.
```

---
## \#549 Posted by: webst Posted at: 2018-06-26T07:59:12.807Z Reads: 203

```
There's also another option when going downhill, at least the one I prefer. I just keep braking very slightly, just to hear the motor hum, it doesn't do much speed wise but allows me to go around 50kmh (10S, 2,25 ratio on 80mm kegels) and  and still have very smooth brakes. I'm not comfortable to go faster so this method should might only work up to this speed.
```

---
## \#550 Posted by: lironch Posted at: 2018-06-27T09:56:16.315Z Reads: 200

```
Has anyone managed to run this on a MAC?
Any tips on where can i find a pre-compiled version or the instructions for compiling it myself?
```

---
## \#551 Posted by: mikenyc Posted at: 2018-06-27T10:58:02.203Z Reads: 205

```
You have to download QT and compile from there
```

---
## \#552 Posted by: briman05 Posted at: 2018-06-29T12:59:46.790Z Reads: 205

```
I have ran this on a macbook pro I did the firmware update and it made my mac freeze after it was done and had to force quit the program but didnt hurt the focboxes.  My mac has a samsung solid state and 10 gb of ram

I believe this is for the mac version as well
https://github.com/Ackmaniac/vesc_tool
```

---
## \#553 Posted by: webst Posted at: 2018-06-29T14:16:49.099Z Reads: 203

```
[quote="briman05, post:552, topic:35116"]
My mac has a samsung solid state and 10 gb of ram
[/quote]
:thinking:
```

---
## \#554 Posted by: Michael319 Posted at: 2018-06-30T08:25:26.079Z Reads: 211

```
As you can see in the picture when instructing the motor to spin "forward" the motor current locks at around 30-35 A. When the motor is instructed to go in reverse, then the motor amps stay consistent with the amps used and continues to increase until over current issues arise. When this happens, reverse feels EXTREMELY POWERFUL, like as if my skateboard had a rocket attached to it (maybe that's how my build is supposed to feel?). I have fixed the overcurrent issue, this issue opened up an error in my foc programming that was fixed. I am still using foc if that could have anything to do with it. Running 12s2p with an Ollin Board Co ESC v1.1.

Any idea is appreciated.

My board is a little slow to accelerrate, so I would love to utilize whatever is happening in reverse.

![Screenshot_2018-06-28-21-25-41|250x500](upload://spbV8sviELqr8DxKZptTNDz9P1d.png)
Clean Graph:
![Screenshot_2018-06-28-21-25-31|250x500](upload://xMR0zFGScV073elJh0Kqc7itTMc.png)
```

---
## \#555 Posted by: Eboosted Posted at: 2018-07-06T00:11:00.151Z Reads: 195

```
I'm getting:

"L is 0. Please measure it first" when runing FOC detection.

Has anyone got this issue sorted on the latest 3.102 FW?
```

---
## \#556 Posted by: PatRocks Posted at: 2018-07-06T00:29:44.681Z Reads: 184

```
Damn I thought that bug was fixed a while ago. You sure you have the newest version?
```

---
## \#557 Posted by: Eboosted Posted at: 2018-07-06T00:52:01.835Z Reads: 189

```
Yes, I do. I tried BLDC mode as well and I can't detect the motor, I'm getting a bad detection error now. So it wasn't the sotware but the ESC
```

---
## \#558 Posted by: PatRocks Posted at: 2018-07-06T01:34:14.807Z Reads: 189

```
Sorry to hear that, I hope you get it worked out. Would you please let us know if (WHEN) you figure out the issue? Best of luck
```

---
## \#559 Posted by: Lionpuncher Posted at: 2018-07-06T04:17:38.789Z Reads: 191

```
Hey guys, wondering if i can get a few suggestions. Installed new ackmaniac fw. Now i can't get any data from the Bluetooth. I try and says esc not connected. Checked wiring, all good. This worked perfectly with bldc tool. Uninstalled the app and reinstalled. Ppm +Uart as far as i can tell as control. Just on a mono drive. App sees the module, but module not getting any info from the vesc. Has anybody had thus problem and found a fix? Gonna hit the hay here. Ill follow up tomorrow. Thanks in advance!
```

---
## \#560 Posted by: mmaner Posted at: 2018-07-06T04:18:57.931Z Reads: 196

```
Did you set the baudrate rate to 9600bps?
```

---
## \#561 Posted by: Lionpuncher Posted at: 2018-07-06T04:23:13.503Z Reads: 198

```
 It appeared to be at that rate. I'm gonna hook it up. Fuck sleep.
Edit: Easy fix. Should have paid closer attention. Forgot to write app configs after changing it. That's a big ole solid DERP. Was only ppm. no uart. K I'm better now. 
Have a god night y'all!
```

---
## \#562 Posted by: PartyPoison Posted at: 2018-07-06T05:59:26.839Z Reads: 200

```
Need help!, im using ackmaniac in 4.12 and its all good, now i have 6.6 and its working (current fw), i tried to update fw with ackmaniac but got I/O error,  i even update bootloader via vesc tool, then update fw but same thing happen, how can i update thw fw?, thanks!
```

---
## \#563 Posted by: chsknight Posted at: 2018-07-06T16:12:35.363Z Reads: 197

```
Increase the duty value from 5 to 8.   Not sure why in VESC tool i had to do this and not in BLDC tool.  

It also seems bugged because sometimes when i re-run the detection it will fail when set to 8 after it was just successful.
```

---
## \#564 Posted by: petter Posted at: 2018-07-07T10:55:21.005Z Reads: 196

```
There is actually a setting in the vesc to counter this, "limit top speed with negative torque" i think it's called. You set the max speed to some value that your board can actually reach and then the vesc will automatically apply the brakes so that you can't go faster that that.
```

---
## \#565 Posted by: PartyPoison Posted at: 2018-07-07T18:44:30.432Z Reads: 196

```
finally got it running to 6.x HW, on my phone it says "ESc not connected",
what should i do?, even re install the app.
```

---
## \#566 Posted by: Benjamin899 Posted at: 2018-07-07T19:23:42.832Z Reads: 194

```
you probably didnt set it up as PPM and UART
```

---
## \#567 Posted by: PartyPoison Posted at: 2018-07-07T19:39:08.788Z Reads: 190

```
i did, maybe its the module, my other board  got connected, ill check it out..
```

---
## \#568 Posted by: Benjamin899 Posted at: 2018-07-07T20:01:32.849Z Reads: 187

```
it the module blinking or constant
```

---
## \#569 Posted by: PartyPoison Posted at: 2018-07-07T20:43:02.854Z Reads: 191

```
Blinking when not connected,
Constant whne connected to the phone (but no data on phone)
```

---
## \#570 Posted by: Minim Posted at: 2018-07-07T20:51:52.651Z Reads: 191

```
Is there a iphone version for the app? I tried to install the app on my samsung s5 but it can't detect the bluetooth module. I updated the phone to Android 8.1 and it still doesn't find the module.. Ios would just be so much easier :D

I see that my device supports bluetooth smart but not peripheral mode. is that the problem?

edit2: forgot to mention that it works fine on a iphone x (yes I have disconnected the iphone app when I try the android)
```

---
## \#571 Posted by: Benjamin899 Posted at: 2018-07-07T20:53:18.155Z Reads: 187

```
i had the same problem, i just forgot to set the connection type from PPM to PPM and UART.
```

---
## \#572 Posted by: PartyPoison Posted at: 2018-07-07T21:01:57.186Z Reads: 191

```
thanks! im gonna re do my vesc setup...
```

---
## \#573 Posted by: Lionpuncher Posted at: 2018-07-08T00:00:16.007Z Reads: 187

```
Had same problem the other night. Setting was only ppm. Selected ppm+uart and remembered to 'write to app '. Worked fine after.
```

---
## \#574 Posted by: Benjamin899 Posted at: 2018-07-10T11:19:16.728Z Reads: 188

```
@Ackmaniac hey i just found an option for max charge in mobile app. Did i understand this correctly that if i charge my board, i have a bms, it will only charge my pack to x,xx volt/cell , so basicly like a programmable bms?
Does it require the the app to be active the entire chargetime or is it more like set it and forget it=?
```

---
## \#575 Posted by: koralle Posted at: 2018-07-10T11:25:55.760Z Reads: 187

```
Nope. I don't know exactly what that setting does or where you found it. I guess it has to do with brake charging. 

It definitely has nothing to do with you charging your battery through the bms.
```

---
## \#576 Posted by: Benjamin899 Posted at: 2018-07-10T11:38:56.683Z Reads: 187

```
when you are connected via bluetooth to your esc, you see all the squares with Speed, Volt, Power, Temp, ect ect, all your real time data from the esc. If you tap volt you get the pop up.
```

---
## \#577 Posted by: Minim Posted at: 2018-07-10T19:44:29.409Z Reads: 190

```
I tried this tool with its firmware yesterday and went from stock current control to ackmaniac current control and now the throttle is mad sensitive.. Before I could go full throttle without problems but now it’s almost throwing me off and it’s very aggressive on the brakes. Settings are as before 60/-60 motor amps, 40/-10 battery amps. Setup is raptor 2 hubs on 12S Escape (vesc6)
```

---
## \#578 Posted by: SageTX Posted at: 2018-07-10T20:00:05.347Z Reads: 194

```
Whaaaaat! Fuckin A! Any idea if Enertion is using your firmware for Raptor 2s? 

I haven't poked around yet, but I use the app for it and it works fine.
```

---
## \#579 Posted by: Ackmaniac Posted at: 2018-07-10T20:26:35.302Z Reads: 196

```
Did you adjust the throttle correctly and did you upload the firmware fo VESC 6? Never had a Escape ESC so have no experience.
```

---
## \#580 Posted by: Minim Posted at: 2018-07-10T20:33:04.508Z Reads: 201

```
I think so. It goes from approx 1000 to 2000us with 1500 as center. It’s rideable but I just feel way less secure on the throttle as it’s so brutal both on and off compared to stock firmware. If I move my thumb slowly it’s no problem :D

Firmware is uploaded and showing as 102 I think it was.
```

---
## \#581 Posted by: Ackmaniac Posted at: 2018-07-10T20:37:11.300Z Reads: 208

```
Question is if it shows the correct hardware version.
The brakes are more powerful because the software calculates the brake power in a different way. Original firmware does it in a strange way which only makes sense when you set motor min and batter min to the same value. But that doesn't make sense when you haven't got a battery that can handle 60A charge current. 
If it is too strong then just reduce the motor amp values and you can also adjust the throttle curve to your needs.
```

---
## \#582 Posted by: Minim Posted at: 2018-07-10T21:04:19.773Z Reads: 207

```
Ok that makes sense. The breaks is only a good thing really I just need to be aware of it but the throttle was a bit notchy. Will try to play some with the throttle curve and maybe try watt control and see if that makes a difference. 

I don’t think anything is wrong it’s just very different :)
```

---
## \#583 Posted by: Wentworth Posted at: 2018-07-18T10:11:05.178Z Reads: 202

```
Hello, I used VESC before. I have only recently discovered this great software. But I will show this warning after connecting. My VESC firmware is 3.38, how can I eliminate this warning? Or ignore it?![%E6%8D%95%E8%8E%B714|690x437](upload://mjPrbedVt8mF74G5z5VFEGlsXD.PNG)
```

---
## \#584 Posted by: Ackmaniac Posted at: 2018-07-18T10:13:10.379Z Reads: 201

```
When you want to use my firmware mod then you also need to install the firmware for that tool. My mod is currently available in version 3.102. 3.38 is the original firmware by Vedder.
```

---
## \#585 Posted by: Wentworth Posted at: 2018-07-18T10:53:26.504Z Reads: 204

```
Sorry, I am stupid. This V4 is the finished product I bought, I don't know how to change the firmware. Forgive me, I am a newbie. Can you give a few pictures or a text description? Thank you for replying to me.
```

---
## \#586 Posted by: briman05 Posted at: 2018-07-18T13:26:33.099Z Reads: 208

```
Click where it says firmware assuming you have a bootloader you will need to know the hardware version of the board like the torque board vesc and focbox are both 4.12 so you would find the selection for your vesc version and load the default firmware.
```

---
## \#587 Posted by: spei Posted at: 2018-07-20T10:39:21.654Z Reads: 207

```
https://www.youtube.com/watch?v=v1glLDO-EjA
```

---
## \#588 Posted by: Wentworth Posted at: 2018-07-20T11:48:26.572Z Reads: 205

```
I'll think about it. Thank you for your reply.
```

---
## \#589 Posted by: Wentworth Posted at: 2018-07-20T11:52:02.395Z Reads: 204

```
I know how to use it on VESC TOOL, but there is something wrong with ESC TOOL.Thank you for your enthusiasm.
```

---
## \#590 Posted by: briman05 Posted at: 2018-07-20T12:39:56.415Z Reads: 205

```
If you know how to use vesc tool the @Ackmaniac tool is pretty much the same.  And saying "I'll think about it" is a little put offish for people who are  trying to help you.  You said your self you are stupid and we are trying to show you how to update your firmware but if you dont want to update your firmware so you can use the tool so forget it
```

---
## \#591 Posted by: Wentworth Posted at: 2018-07-22T08:23:32.515Z Reads: 201

```
Sorry, I will be careful about the way I speak.  Thanks for your reminder
```

---
## \#592 Posted by: Andy87 Posted at: 2018-07-23T09:03:07.633Z Reads: 203

```
I have a problem if I set up my vesc to current mode.
In current mode I can drive forward and backwards.
If I simulate a signal loss by switch of my remote the
break apply and after reaching 4000erpm the wheels start to spin backwards.
How to adjust the settings that in case of signal loss the board will just break or roll out?
My timeout is set to 1000ms and 0A.
I tried it with different remotes. Did fail safe set up of the remote and adjustment in the app settings. So everything should be centered.
```

---
## \#593 Posted by: Ackmaniac Posted at: 2018-07-23T16:53:05.017Z Reads: 204

```
When the timeout current is set to 0 then the timeout does nothing else then giving no throttle. Problem is that the remote receivers fail safe sends a valid signal for going backwards. So please check the signal in the tool when the remote is off and adjust it if it is wrong.
```

---
## \#594 Posted by: Andy87 Posted at: 2018-07-23T21:00:16.872Z Reads: 205

```
ok thx! i found out that on the gt2b remote the trigger poti changed position...
i tried to adjust, but even with max adjustment i still have a small chigger of the motor (better now but not gone).
i run now in current no reverse as it only break a bit when signal los but don't start to move the motor backwards.
```

---
## \#595 Posted by: Ackmaniac Posted at: 2018-07-23T22:16:23.031Z Reads: 207

```
You can also adjust the failsafe far away from the normal positions. To do that turn the poti for example completely to the left and then adjust your pulse width settings. After that turn your poti completely to the opposite direction and increase the pulsewith by holding the trigger to go as far away from the normal pulse with signals as possible. Then adjust the failsafe in that position.
Because if the vesc detect a pulsewith that is more than 20% away from the normal positions it detects it as a signal loss.
And for example for 1.00 min, 1.5 center and 2 max 20% away would be below 0.8 or above 2.2. Hope that is understandable.
```

---
## \#596 Posted by: Andy87 Posted at: 2018-07-25T06:15:51.227Z Reads: 201

```
Still a bit confusing. 
I just don´t get the fail safe signal set to the center position of my pulsewith (min is -11% which still gives a small impulse to the motors).
I don´t understand how to set the failsaife according to your description. I made like this:
1.poti max left 
2.center pulswith with app 
3.poti max right 
4.put the trigger to the max away from pulswith (would be max backwards/break) 
5.switch off vesc plug pairing plug and switch on system in the max trigger position.

I think I got something wrong, as when I do like this the failsaife of the remote is set to 100% break and in current mode it would spin the motors backwards with all they can.
```

---
## \#597 Posted by: Ackmaniac Posted at: 2018-07-25T06:29:57.801Z Reads: 202

```
Here you can see how to adjust the failsafe with the little button on the receiver. No need to switch off the vesc. 
https://youtu.be/uCvlO_oA0_I
```

---
## \#598 Posted by: Andy87 Posted at: 2018-07-25T08:09:06.776Z Reads: 200

```
Thought failsafe on the GT2B is set up like the mini remote in time when it get paired:sweat_smile:
Didn't see the button on the receiver...will check that after work. should be the solution!
Thank you for your time!
```

---
## \#599 Posted by: Sebike Posted at: 2018-07-26T08:50:17.564Z Reads: 202

```
Would keeping the sensors activated  through the ride, FOC mode, (and not switching off over say 2500rpm) heat up the motors or it wouldn't matter to them?
```

---
## \#600 Posted by: Ackmaniac Posted at: 2018-07-26T16:39:55.514Z Reads: 202

```
Vedder says at higher speeds the halls signal wouldn't be fast enough. Never tried and it works great sensorless above 2500. For 12S I recommend a higher switching frequency of 30khz which I always use. I experienced that the motors begin to vibrate with 20khz at high speeds. But it depends on the motor. Most people don't recognize that. But when I try their boards I feel it immediately and after I told them they can hear it as well.
```

---
## \#601 Posted by: PatRocks Posted at: 2018-07-26T17:27:51.455Z Reads: 202

```
Good advice, I'll try that tonight!
```

---
## \#602 Posted by: willumpie82 Posted at: 2018-08-02T07:57:51.927Z Reads: 199

```
@Ackmaniac, what would it involve to create a step-assisted mode (like the slow ebikes) in your firmware? e.g. when the wheels are spinned manually (by a kick) they spin down (assisted) really long (settable by throttle) this is more or less the same as one of the commercial boards but with the difference that it won't keep running that speed forever. as safety feature i would keep the remote control for breaking, the throttle for the amount "support"

update: I See, it is already asked for as endless mode, missed that ;-)
```

---
## \#603 Posted by: Luuke Posted at: 2018-08-02T08:22:39.603Z Reads: 197

```
https://www.electric-skateboard.builders/t/endless-ride-for-vesc/48918
```

---
## \#604 Posted by: Ackmaniac Posted at: 2018-08-02T10:12:41.993Z Reads: 199

```
That mode already exists. When you press the throttle it holds the speed and braking still works. It doesn't accelerate actively. Only difference is that it doesn't decrease the speed over time.

![image|690x463](upload://zDBVAq85Zzrsk6JSib4PBxe4tEb.png)
```

---
## \#605 Posted by: mikenyc Posted at: 2018-08-02T10:25:32.600Z Reads: 187

```
Not requiring the throttle, and decreasing the speed are the key features.
```

---
## \#606 Posted by: Ackmaniac Posted at: 2018-08-02T11:02:10.714Z Reads: 189

```
To not need the throttle is of course possible but too dangerous.
```

---
## \#607 Posted by: mikenyc Posted at: 2018-08-02T11:24:51.541Z Reads: 196

```
Users of the mellow who are mostly new to esk8 seem to have no issue with it though. How is that dangerous?

It's unfair to mischaracterize something as dangerous when it simply doesn't appeal to you, or if it's utility isn't immediately obvious.
```

---
## \#608 Posted by: Jc06505n Posted at: 2018-08-02T13:40:46.483Z Reads: 193

```
Agreeing with Mike here, it's not the same as Endless ride as Decreasing speed and not requiring throttle are **critical** to what the mode is. In this mode the remote should only act as a breaking device. If it was truly dangerous than you would see more reports of incidents in the Mellow Subreddit or even the ESK8 subreddit as a whole (since there's an anti-mellow phase going on).

Edit: And there's also the fact that to move in this mode you have kick push, I hypothesize that kickpushing on ESK8's can prove beneficial results to range, even more so with a mode that takes advantage of it.
```

---
## \#609 Posted by: mikenyc Posted at: 2018-08-02T14:02:48.670Z Reads: 191

```
Would it be difficult to ramp the speed down over time?
```

---
## \#610 Posted by: Ackmaniac Posted at: 2018-08-02T14:35:30.997Z Reads: 203

```
Don't like that the board continues alone when you fell off and loose the remote out of your hand. Next issue is how the board behaves when you push, because you have no control over it.

Lets say you start and push only one time. If the board immediately reacts to the new speed by providing power to hold the speed it would be ok. But if you want to do two pushes the board brings you out of balance when it starts powering while your foot is off to board at the haul off for the second push.

By activating cruise with the throttle it is easy to control the board and let cruise be active whenever you want it. Otherwise you need to adapt to the behavior of the board.

And it wouldn't be difficult to ramp down over time. That's the easiest part.

The hardest part is to find a good soft ramping when the board starts powering to hold your current speed.
But finally i don't want the board to continue holding the speed when you felt off and lost the remote. So you need to pull the trigger to activate cruise control. And by this you can shortly release the trigger when you push and pull it again at your new speed.
```

---
## \#611 Posted by: mikenyc Posted at: 2018-08-02T15:41:30.415Z Reads: 196

```
Why not pull the brake to let it stop. Hold the throttle to allow the board to accelerate. Acceleration is based on how much you push. It decelerates at a specific rate. 

This feature has been discussed over and over in this thread and others many times. I'm fine with you never putting it in. Maybe some day someone more enthusiasm will come along and make a new firmware that everyone will love and will include it. If not, it's not the end of the world.
```

---
## \#612 Posted by: Trdolan03 Posted at: 2018-08-02T17:38:14.474Z Reads: 197

```
@mikenyc There is no need to take digs at @Ackmaniac. He has volunteered his time, and a lot of it, to everyone here. We should be thankful for the features his firmware includes and not mad for what it doesn’t.
```

---
## \#613 Posted by: mikenyc Posted at: 2018-08-02T18:12:06.366Z Reads: 194

```
My remarks are not to be interpreted as digs toward @Ackmaniac. I'm simply pointing out that the subject has been debated ad nauseam with the same questions and the same responses.
```

---
## \#614 Posted by: craigthemachine Posted at: 2018-08-02T18:24:49.477Z Reads: 199

```
Yup, exactly .. we can’t have it all. I can’t  imagine every single change request being completed without adequate need for it.
```

---
## \#615 Posted by: mikenyc Posted at: 2018-08-02T18:38:52.827Z Reads: 201

```
the need, or desire, rather has been expressed by many
```

---
## \#616 Posted by: Ackmaniac Posted at: 2018-08-02T19:25:12.470Z Reads: 201

```
Did you ever try the "PID Speed Control No Acceleration" mode?
```

---
## \#617 Posted by: mikenyc Posted at: 2018-08-02T19:42:02.927Z Reads: 203

```
I will not because it does not decline in speed. What is the point of pushing up to speed on foot if you can not come back down to a speed that you are comfortable pushing at again
```

---
## \#618 Posted by: skatardude10 Posted at: 2018-08-02T19:53:33.110Z Reads: 210

```
I tried it and it's fun! But it's a different kind of fun. There are some quirks that make it interesting when changing the PID values, such as increasing the values to lock you in and pumping off of the cruise control to go faster and reengaging it at the faster speed over and over... It's easy to get going *way too fast* this way real quick... But it's just not the same.

I could see lower values working well with a pure push and coast down mode as it wouldn't jerk you around so much as the higher values.
```

---
## \#619 Posted by: Ackmaniac Posted at: 2018-08-02T20:24:21.012Z Reads: 204

```
Yes you need low values if you want it smooth and high values if you want it to hold the speed quickly. And you are right you can easily pump up to higher speeds this way.
```

---
## \#620 Posted by: willumpie82 Posted at: 2018-08-03T06:50:40.119Z Reads: 205

```
But about the starting push(es), if the board could match the speed that you push (or just a x% below it) and like the mellow board decelerates in n seconds, i guess you wouldn't be thrown off

as a safety precaution I would include the throttle still (or cruisecontrol), this way you can actively control the amount of power (or time). on zero throttle nothing happens (or a settable default current to overcome the boards mechanical friction)
```

---
## \#621 Posted by: Wentworth Posted at: 2018-08-07T02:57:38.803Z Reads: 210

```
If I use V6, which bootloader do I need to burn first?
![image|255x69](upload://2E5tSFiDZE7xrIBdHi2wDRqKG6w.png)
```

---
## \#622 Posted by: briman05 Posted at: 2018-08-07T03:00:24.685Z Reads: 212

```
If you have a Vesc 6 you wouldn’t use any
```

---
## \#623 Posted by: Wentworth Posted at: 2018-08-07T03:35:26.966Z Reads: 218

```
V6 also seems to need to use his bootload. But I don't know which one to use.
![image|690x437](upload://bB2SSHm9f89P9SwSrmZmFgf8D0w.png)
```

---
## \#624 Posted by: Ackmaniac Posted at: 2018-08-07T07:15:26.546Z Reads: 207

```
V6 comes already with a bootloader installed. I would be very surprised if it doesn't.
```

---
## \#625 Posted by: Wentworth Posted at: 2018-08-07T07:47:51.716Z Reads: 207

```
Do you mean that the V6 I bought can be used directly? And I won’t have this problem. I have no problem with VESC TOOL. I started to worry about whether my V6 is fake.
```

---
## \#626 Posted by: Ackmaniac Posted at: 2018-08-07T07:53:39.679Z Reads: 210

```
If you want top use my firmware mod you need to flash it. If you want to use the original you can leave it as it is.
```

---
## \#627 Posted by: Wentworth Posted at: 2018-08-07T10:14:29.970Z Reads: 212

```
How to flash it? I don't know how to use your firmware module. Is there such a teaching link or video?
```

---
## \#628 Posted by: Adam0311 Posted at: 2018-08-07T15:40:33.588Z Reads: 221

```
I would start by doing several “how to flash firmware” searches on here. Then by following up with the people you know have already flashed firmware if you still have specific questions. It’s actually quite easy, although I’ve never flashed a vesc 6.
```

---
## \#629 Posted by: ARetardedPillow Posted at: 2018-08-12T06:59:06.971Z Reads: 225

```
When I tried motor detection it triggered 
The following faults were registered since start:

Fault            : FAULT_CODE_OVER_TEMP_FET
Current          : -2.7
Current filtered : 0.3
Voltage          : 38.42
Duty             : 0.001
RPM              : 3.9
Tacho            : 0
Cycles running   : 0
TIM duty         : 4
TIM val samp     : 1050
TIM current samp : 3150
TIM top          : 4200
Comm step        : 4
Temperature      : 330.57
 ,
This doesn't happen on 2.54, any idea what could be the problem?
```

---
## \#630 Posted by: ARetardedPillow Posted at: 2018-08-12T07:18:12.239Z Reads: 223

```
Also happens with the new vesc tool, using focbox, and this happens on all 3,4, 5 hundred other focboxes aswell,   its getting frustrating as shit

Update: works with flipsky 4.12, doesn't work with focbox
```

---
## \#632 Posted by: Ackmaniac Posted at: 2018-08-12T13:34:07.191Z Reads: 216

```
You have to use the 4.12 firmware for the focbox as well.
```

---
## \#633 Posted by: Minim Posted at: 2018-08-18T23:34:02.086Z Reads: 212

```
Is it possible to upgrade the firmware through a phone with those Bluetooth modules that are commonly used (not the one Benjamin uses)?
```

---
## \#634 Posted by: FranciscoV Posted at: 2018-08-21T19:16:03.363Z Reads: 208

```
Hey everyone.  I’m fairly new in this forum and I’ve done a ton of reading looking for an answer to my problem.  
I’ve recently downloaded the ackmaniac tool and configured both motors and ESCape boxes on my kaly board.   Sensored Foc mode works great only problem is after I did all the work my Bluetooth dongle doesn’t connect to either of my eSkate vesc or ackmaniac app.  2 different phones and nothing works  

Suggestions on how to fix the problem?? 

Any help will be highly appreciated
```

---
## \#635 Posted by: threebysix Posted at: 2018-08-21T19:52:39.465Z Reads: 207

```
did u remeber to connect the Rx and TX on your bt dongle to the TX and Rx in the vesc?
```

---
## \#636 Posted by: FranciscoV Posted at: 2018-08-21T20:10:41.004Z Reads: 210

```
Hi there.  Thanks for the reply.  
Nothing has been disconnected everything is in place.  This happened after I reflashed the escapes with 60 hardware![image|406x500](upload://3Z6gTu38Ply3c9tYAFfU8hcsJHE.jpeg)
Before that everything was working just fine
```

---
## \#637 Posted by: Sender Posted at: 2018-08-21T20:15:54.283Z Reads: 204

```
Hmmmm is the master set to ppm and uart with 9600 baud rate?
```

---
## \#638 Posted by: briman05 Posted at: 2018-08-21T20:24:03.749Z Reads: 202

```
That is exactly what I was going to suggest.
```

---
## \#639 Posted by: FranciscoV Posted at: 2018-08-21T20:39:17.143Z Reads: 215

```
Master set to ppm as for the uart deal I have no idea.  I guess that I would have to check with my computer   As I stated before.  I’m new here and understand some of the definitions can be confusing at times 😂

The only useful info I have is that Ernesto said 

“On the Bluetooth, If you are using the Trampa BLDC tool this feature will not work”
```

---
## \#640 Posted by: Sender Posted at: 2018-08-21T20:47:07.628Z Reads: 216

```
Ok cool.  Make sure the master is set to PPM and Uart (if the BT module is hooked up to the master).  Then make sure the baud rate is set to 9600.
```

---
## \#641 Posted by: FranciscoV Posted at: 2018-08-21T21:01:00.155Z Reads: 218

```
You are the man.  I will go ahead and do that once I get home.   I didn’t know there were more steps to it!   I appreciate it guys.
```

---
## \#642 Posted by: Ackmaniac Posted at: 2018-08-21T22:25:46.457Z Reads: 216

```
You can try it with my firmware mod. 
Currently the app doesn't support the latest official firmwares.
```

---
## \#643 Posted by: FranciscoV Posted at: 2018-08-22T00:51:13.963Z Reads: 230

```
It was just my lack of knowledge.    Had to get help from a friend to reprogram vesc app settings.  
Up and running again
Thanks again for all the support guys.  I appreciate it  👍🏼
```

---
## \#644 Posted by: mmaner Posted at: 2018-08-22T12:59:23.177Z Reads: 233

```
has anyone tried using the Ackimaniac firmware on the Flipsky Dual FSESC4.20 100A?

https://flipsky.net/collections/electronic-products/products/dual-fsesc4-12-100a
```

---
## \#645 Posted by: EssEnn Posted at: 2018-08-22T14:13:50.707Z Reads: 230

```
I will be flashing it when mine arrives. Should be shipping in the next 24-48 hours. I had no issues flashing the 6.6 once I installed the bootloader
```

---
## \#646 Posted by: briman05 Posted at: 2018-08-22T18:30:34.971Z Reads: 228

```
I was wondering the same thing about the firmware. I wish these came with a bootloader installed so it was as simple as the unity.  This looks like a real competitor to the unity I would like to see a side by side comparison of the two
```

---
## \#647 Posted by: jens_c Posted at: 2018-08-25T13:48:03.293Z Reads: 224

```
hi 
I can not change modes with the app i am wondering wy that is the case
```

---
## \#648 Posted by: Ackmaniac Posted at: 2018-08-25T16:50:39.562Z Reads: 223

```
Do you use my firmware mod or the original? And ate you connected to the master or the slave?
```

---
## \#649 Posted by: jens_c Posted at: 2018-08-26T13:57:22.777Z Reads: 224

```
[quote="Ackmaniac, post:648, topic:35116"]
you connected to t
[/quote]

i only have one vesc 
i am using your firmware mod 
i am using ADC if that makes a difrence
```

---
## \#650 Posted by: Ackmaniac Posted at: 2018-08-26T14:04:41.993Z Reads: 227

```
Mode changes are currently not supported for adc. When I find the time I can try to add that as well.
```

---
## \#651 Posted by: jens_c Posted at: 2018-08-26T20:00:45.633Z Reads: 227

```
I would apriciate that!
```

---
## \#652 Posted by: ArnhemAnt Posted at: 2018-08-27T10:15:47.577Z Reads: 231

```
I'm setting up a dual motor build and this is the first time I have had to configure ESC's (ESCapes). I'm running mac and can't seem to find a link to the VESC tool for mac - could someone please clarify if there is one and also where I can download it?
Thanks.
```

---
## \#653 Posted by: Andy87 Posted at: 2018-08-27T12:02:46.386Z Reads: 228

```
https://www.electric-skateboard.builders/t/vesc-tool-ackmaniac-vesc-tool-mac-builds/62840
```

---
## \#654 Posted by: alivedom Posted at: 2018-08-28T14:53:36.256Z Reads: 226

```
I would really appreciate that. Im using ur FW and App for my DIY friction drive Ebike. Im kinda afraid that it will get taken away if i get in a control bc its way too powerfull without limitation. For that id feel more comfortable if i could switch mode to limit max speed and power as fast as possible in case... Thanks for the great work anyway!
```

---
## \#655 Posted by: Benjamin899 Posted at: 2018-08-29T10:13:17.372Z Reads: 215

```
I don't think E-Bike Driver have to fear the Police. You Guys blend in well
```

---
## \#656 Posted by: EssEnn Posted at: 2018-08-29T11:20:35.118Z Reads: 211

```
Just set the restricted settings as default then use the APP to change the mode when you ride. If the coppers grab you just power off the VESC and when they power on to check it will load the default restricted settings.
```

---
## \#657 Posted by: alivedom Posted at: 2018-08-29T11:40:12.622Z Reads: 207

```
oh i was refering to the mode change not working on ADC
```

---
## \#658 Posted by: EssEnn Posted at: 2018-08-29T13:48:27.513Z Reads: 213

```
ahhh.. sorry I should really have read the previous posts. My bad
```

---
## \#659 Posted by: jens_c Posted at: 2018-08-29T20:31:02.390Z Reads: 210

```
same problem over here i'm working on converting adc to ppm to overcome this problem
```

---
## \#660 Posted by: Ackmaniac Posted at: 2018-08-29T21:12:31.179Z Reads: 210

```
I work already on the integration. Maybe i find the time to test it over the weekend.
```

---
## \#661 Posted by: Sender Posted at: 2018-08-30T17:44:28.662Z Reads: 215

```
So I have never used the watt limits.  To do this, I can't just click it in the app right?  Because I have to do it for each motor?  Or can I try it in the app without opening up my enclosure and reprogramming both Vescs?  I am sure this is covered somewhere, but I am having trouble hunting it down.
```

---
## \#662 Posted by: deucesdown Posted at: 2018-08-30T18:14:12.272Z Reads: 214

```
If you set it up as instructed, you can create a "mode" in "Modes Setup" that includes the app mode aka watt/wattNoRevBrake/current/etc.

You can save that mode, and switch to it on the fly. If the canbus stuff is set up properly it'll change on both master and slave vesc. You can long press on the top left box and it'll offer to make the current mode the default (persists across reboots).

This probably belongs in the other thread (https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888)
```

---
## \#663 Posted by: rey8801 Posted at: 2018-08-30T19:37:29.613Z Reads: 213

```
Moreover if you want to check what @deucesdown said you can always connect to the VESC through the app with a TCP connection. Both computer and phone has to be on the same wifi. I find the Hotspot from the phone more stable for this connection. Board as close as possible. In this way you can use the vesc tool without open the enclosure
```

---
## \#664 Posted by: deucesdown Posted at: 2018-08-30T19:45:19.877Z Reads: 209

```
[quote="rey8801, post:663, topic:35116"]
connect to the VESC through the app with a TCP connection
[/quote]

Is this both Vesc-Tool and BLDC-Tool (ackmaniac version)? Or Vesc-tool only?
```

---
## \#665 Posted by: rey8801 Posted at: 2018-08-30T19:45:53.348Z Reads: 209

```
I bet VESC tool only and only the Ackmaniac VESC tool version
```

---
## \#666 Posted by: DeathByBacon Posted at: 2018-08-31T20:00:21.081Z Reads: 207

```
Is it possible to limit speed and acceleration through the APP by making a new mode? I want to be able change to a mode on the fly that a beginner can use or someone who wants to try and "get the feel" of an electric skateboard.
```

---
## \#667 Posted by: spei Posted at: 2018-08-31T20:06:22.201Z Reads: 217

```
[quote="DeathByBacon, post:666, topic:35116, full:true"]
Is it possible to limit speed and acceleration through the APP by making a new mode? I want to be able change to a mode on the fly that a beginner can use or someone who wants to try and “get the feel” of an electric skateboard.
[/quote]


![Screenshot_20180831-220217|281x500](upload://2BCII43Qr4NmCEgaE3dI6FtX31g.jpg)
```

---
## \#668 Posted by: Ackmaniac Posted at: 2018-08-31T22:03:19.590Z Reads: 206

```
Yes of course. Just simply limit the top speed and the motor current for less acceleration. And you can also limit the watts.
```

---
## \#669 Posted by: gigoy Posted at: 2018-09-11T04:34:08.667Z Reads: 195

```
What does the colour orange on "Voltage" mean?
```

---
## \#670 Posted by: Ackmaniac Posted at: 2018-09-11T06:35:35.300Z Reads: 196

```
That the voltage is below the battery cutoff start. So the vesc limits already the power output. When the battery cutoff end is reached the color turns red.
```

---
## \#671 Posted by: gigoy Posted at: 2018-09-11T07:04:13.774Z Reads: 195

```
I ran out of power on my 12s pack

1. swapped it out with a 10s pack
2. powered board on
3. changed battery setup in Android APP to 10s
4. powered board off
5. closed app
6. powered board on
7. opened app 

and "Voltage" is in orange, motors will spin but a lot of stuttering (not "ride-able").

Is there a proper way of doing this?
```

---
## \#672 Posted by: mmaner Posted at: 2018-09-11T15:17:56.732Z Reads: 199

```
Is the 10s pack charged above the cutoff limit?  Did you change the cutoff limit in the config to match 10s?
```

---
## \#673 Posted by: Ackmaniac Posted at: 2018-09-11T15:32:08.925Z Reads: 200

```
@mmaner is right. The cutoff settings need to be changed which the app doesn't do.
```

---
## \#674 Posted by: gigoy Posted at: 2018-09-11T17:17:36.603Z Reads: 200

```
Yeah. I changed it in the Ack-ESC tool and the 10s pack worked.
Lesson learned: The best and simplest way to do battery swaps is to have the same battery configuration for both packs. Or...
I'm curious though, what are the consequences of leaving cut-off start/end at the default 10 and 8?
```

---
## \#675 Posted by: jens_c Posted at: 2018-09-17T18:29:23.322Z Reads: 192

```
@Ackmaniac any progress on mode change for adc?
```

---
## \#676 Posted by: lironch Posted at: 2018-09-20T07:59:56.003Z Reads: 188

```
@Ackmaniac
a small clarification needed, i am working with a focbox flashed by your latest firmware 3.102 and still can't write to the focbox using the old Metr.at module.
From reading here i understood that flashing with version 3.101 or 3.100 should fix that but since i am using a mac and it is hard to find mac compatible complied builds for those versions i want to use the latest 3.102 version UI just with the default.bin file i downloaded from you Github repo looking on the commit history of that folder ([here](https://github.com/Ackmaniac/vesc_tool/tree/5581f16503b28cad50273f808659e23330a3979f/res/firmwares/410_o_411_o_412))

Am I right thinking it should work?
```

---
## \#677 Posted by: ArnhemAnt Posted at: 2018-09-23T03:03:59.859Z Reads: 198

```
I'm having some firmware issues with this program. Trying to set up dual ESCapes over CanBus. Setting up each ESC separately first, with CanBus cable disconnected.
In regards to firmware, the ESC's each connect with no firmware update warnings and I can go through and make all relevant settings, however when I then connect CanBus and try to select "Can Forward" I get an incompatible firmware warning. 
When I go into the firmware tab for each ESC, when they are connected, I only have the option of "60" in the hardware tab, however, when none of the ESC's are connected, the firmware hardware tab shows a number of firmware versions. WTF??
Here is a pic of the firmware tab with no ESC connected.
![ACK_Firmware1|666x500](upload://jvzeXuGXLmcPPdLCIk803wBkyYh.jpeg) 

Here is what it looks like when I have an ESC connected.
![ACK_Firmware2|666x500](upload://gGE9uRFLA9xuC0Bm0aw3ziDtb5O.jpeg) 

When I go to read the firmware on the ESC, this is what it is showing me.
![ACK_Firmware3|666x500](upload://ds0HpeVSLpHgm36nxvxlPrOKv6q.jpeg) 

Anyone able to shed some light on this for me??

Crazy part is that I can run the board with the current setup, over CanBus - got me fucked how or why....
```

---
## \#678 Posted by: sayekim Posted at: 2018-09-23T09:02:23.161Z Reads: 180

```
This problem may occur when both vescs have the same controller id. Check if they do. 
Name one zero and one one and then connect the vesc zero and then can forward to one to connect to one.
```

---
## \#679 Posted by: ArnhemAnt Posted at: 2018-09-23T09:38:19.929Z Reads: 179

```
Thanks. Unfortunately, I've already done that and still no difference.
```

---
## \#680 Posted by: Andy87 Posted at: 2018-09-23T09:46:31.632Z Reads: 195

```
Did you check if the CAN stat is 500hz and the baud rate 500k?
![image|571x500](upload://8xZXBkGmIiCLmYnrWaGIUNlsJUf.jpeg) 

Ignore the red lines...it’s a picture from other topic and the „sent via CAN“ need to be true also
```

---
## \#681 Posted by: ArnhemAnt Posted at: 2018-09-23T10:45:19.104Z Reads: 192

```
I followed the instructions from this video as it explains how to set up CanBus. 
https://www.electric-skateboard.builders/t/how-to-program-canbus-properly-video-tutorial/52606?u=arnhemant

The issue I have (I think) is that my firmware is not synced and I am not sure how to fix that.

I hope this makes some sense. Maybe @Ackmaniac can help out here??
```

---
## \#682 Posted by: Andy87 Posted at: 2018-09-23T10:47:57.527Z Reads: 183

```
But this you can check by read out the fw version of each esc. You showed above on one picture the fm of one. How about the second?
If you flashed the ack. Fw on both they should be the same. Don’t understand how the versions than could be different
```

---
## \#683 Posted by: Snake Posted at: 2018-09-23T16:02:20.365Z Reads: 185

```
Hi Guys,
are there any known issues on the actual Ackmaniac-Firmware in combination with the FocBox?
Is it possible to change values and check telemetrie data from two Focboxes over the Canbus even if the throttle signal for each Focbox comes from a seperate PPM-receiver (one receiver for each Focbox)?
```

---
## \#684 Posted by: mmaner Posted at: 2018-09-23T16:13:13.557Z Reads: 188

```
No issues at all. You can double the values in the settings yo get accurate metrics.
```

---
## \#685 Posted by: Ackmaniac Posted at: 2018-09-23T19:12:53.468Z Reads: 185

```
You know that you need to enter the ID of the other esc you want to reach via CAN? Don't give the same ID for master and slave. Just use 0 for the master and 1 for the slave. Make sure both have the same baudrat settings.
```

---
## \#686 Posted by: fraannk Posted at: 2018-09-23T20:25:53.353Z Reads: 189

```
Hey, how do I get 3.101 instead of 3.102? Seems that 3.102 is incompatible with the standard Metr modules.
EDIT: nvm, seems it's only the modes function, which I don't use anyway. :)
```

---
## \#687 Posted by: ArnhemAnt Posted at: 2018-09-23T21:01:10.440Z Reads: 187

```
I've done that. Master is 0 and slave is 1. When I go to hit Can Forward, that's when I get a firmware error message. As I said above, I don't have the option to select firmware 4.12, I only have the option for 60.
```

---
## \#688 Posted by: Andy87 Posted at: 2018-09-23T21:05:00.606Z Reads: 187

```
You haves escapes, they are hw6.0
If you load the 4.12 firmware you will broke them (you can’t use them than, only if you flash the right fw with a stl v2 link again)
```

---
## \#689 Posted by: ArnhemAnt Posted at: 2018-09-23T21:06:34.842Z Reads: 191

```
Right - stupid me. So in the firmware tab, the 60 is correct then?

Edit: All sorted now. Not sure exactly what I did, or didn't do, but i went back to default and set up each ESCape again on their own, and followed the video from @Deckoz about setting up over CanBus and it is now working. Best part is that I can now also connect via Bluetooth and make changes on the fly. 

Man, am I glad that saga is now all over!!

Thank you to everyone who helped me out with this, in particular, @Andy87 and @Deckoz. You guys are awesome.
```

---
## \#690 Posted by: Andy87 Posted at: 2018-09-24T04:45:33.371Z Reads: 177

```
Nice to hear! Good that it worked out in the end! 👌
```

---
## \#691 Posted by: ArnhemAnt Posted at: 2018-09-24T20:46:07.277Z Reads: 178

```
Thanks man.
Now I have a battery issue. Seems like one of my cells is not balancing. I've sent the battery pack back for repair so it's going to be about a fortnight at least until I can ride again. I'm very fortunate to have had my battery pack built here in Australia by someone who will provide a full warranty on their work (including the parts used).
```

---
## \#692 Posted by: lironch Posted at: 2018-09-25T06:25:13.662Z Reads: 175

```
Just for sake of other builders interested in getting this to work, you can use the 3.102 version available and flash your vesc with the 3.101 version available at ackmaniac's github repo ([here](https://github.com/Ackmaniac/vesc_tool/raw/5581f16503b28cad50273f808659e23330a3979f/res/firmwares/410_o_411_o_412/VESC_default.bin)).
Done it myself and it worked!
```

---
## \#693 Posted by: Snake Posted at: 2018-09-29T08:04:25.735Z Reads: 183

```
...unfortunatly i do not receive any values from the FocBox...
The wiring is ok, the App gets BT-Connction but no values are displayed.
Do i need a spcial FW on the Focbox or should it work with the FW displayed on the pic below...? It´s the "normal" FW uploaded with the VESC-Tool0.95... :roll_eyes::face_with_raised_eyebrow:![Unbenannt|690x468](upload://Ak3VJ3w0fmFiIbGXR9RxfzPfkTD.jpeg) ![IMG_6892|630x500](upload://y5KZby5cfRuFtbDwDWOruwew5LS.jpeg)
```

---
## \#694 Posted by: Maxid Posted at: 2018-09-29T08:06:07.985Z Reads: 175

```
Did you set the focbox to do uart? Do the baudrates match?
```

---
## \#695 Posted by: Snake Posted at: 2018-09-29T08:08:23.807Z Reads: 175

```
...yes
![Unbenannt2|690x56](upload://peIYEIpFDpzDnnNpqzvQbjVdUjW.jpeg) ![Unbenannt1|690x138](upload://dLotVWI7mN9JMeAXbBP0YgWBPDF.jpeg)
```

---
## \#696 Posted by: Maxid Posted at: 2018-09-29T08:10:01.919Z Reads: 171

```
Well does your module really use 9600bps or something else? I had mine set at 115200 for example (After fiddling with the firmware on it via AT+ commands).
I also think that Vedder did some modifications to the original firmware so you obviously should check @Ackmaniac's version to be safe. (Maybe you are already using it - I am not sure from the pic you posted). I think @Pimousse made Vedder aware that his modifications break compatibility.
```

---
## \#697 Posted by: Snake Posted at: 2018-09-29T08:15:22.758Z Reads: 173

```
The module should work - a friend uses the same with 9600bps.
I am using the FW from the VESC-Tool 0.95 at the moment. 
Not the Ackmaniac-Version. Maybe i should try to change the FW.
```

---
## \#698 Posted by: Maxid Posted at: 2018-09-29T08:17:14.508Z Reads: 179

```
Yeah change it to ack's version and report back. If you use stock firmware on the module you should be safe with 9600bps - just wanted to rule out the possibility.

Edit: found @Pimousse post:  https://www.electric-skateboard.builders/t/escape-cant-get-it-talking-to-arduino-via-uart/68630/4?u=maxid
This might apply to the ble module as well.
```

---
## \#699 Posted by: Snake Posted at: 2018-09-29T09:41:11.627Z Reads: 182

```
Ok, thanks for the Information :+1:
I will test the alternative FW. 
But if i change the FW i will loose all parameters, right?
```

---
## \#700 Posted by: Maxid Posted at: 2018-09-29T09:43:40.323Z Reads: 189

```
You mean motor parameters and settings? I think if you read them via VESC tool and then update the firmware without closing the tool, then you can just hit write again and it should set it all for you.  No guarantees though - if I were you I'd just do the config again - it's not like it takes a couple hours.
```

---
## \#701 Posted by: danielz Posted at: 2018-09-29T13:41:46.805Z Reads: 192

```
vesc tool 0.95 fw 3.40 no data for me either anymore, so had to downgrade. In the change log its mentioned, id added to uart, which has broken the apps.
```

---
## \#702 Posted by: butt_stallion Posted at: 2018-10-05T19:02:12.580Z Reads: 200

```
If I install the 410 & 411 & 412 firmware that is included with this ESC tool can I still use the Ackmaniac-BLDC tool to configure it instead of this ESC tool?  I know on the dropbox link the BLDC tool is under a folder labeled, "old"
```

---
## \#703 Posted by: Moza Posted at: 2018-10-06T14:24:26.467Z Reads: 205

```
Hi guys.

Anyone had an issue with losing real time data from vesc on ackmaniac app?

I cant get any real time data from any of my 4.12 vescs anymore (i can with vesc tool and serial link though).

![Screenshot_20181006-132342|281x500](upload://rNAekcSYtjXSKHyUnLciyhZZrRc.png) 

They all worked perfectly and now non of them work. ( I have 3 all from different manufacturer's).

All settings appear to be fine. ( App settings on adc and uart. Uart is set to 9600).

Whenever I connect to ackmaniac app the current limits appear but nothing else. 
Bluetooth module is hm10.

Just wondering if its due to a recent update to the app as all hardware has been replaced and still no luck.

Thanks
Steve.
```

---
## \#704 Posted by: mmaner Posted at: 2018-10-07T14:24:04.287Z Reads: 188

```
Make you don't have any other vesc BT apps open and try again.  If no joy, uninstall reboot reinstall. That usually works for me.
```

---
## \#705 Posted by: Moza Posted at: 2018-10-07T17:27:42.561Z Reads: 200

```
Thanks for the reply.

I have tried to re-install the ackmaniac app but that didn't resolve the issue.

Also, I have the app installed on my phone and tablet. Both were working fine and now both won't work.
```

---
## \#706 Posted by: Pmac Posted at: 2018-10-09T12:35:57.499Z Reads: 206

```
@Ackmaniac just wondering if you could please help.  Do you know if there is a way of getting the Flipsky Bluetooth module to work with your app.

Flipsky have advised that the Bluetooth module they sell will only work with the VESC Tool Android App but I just wanted to see if there was a way to make it work before pulling it out.

It is based of the NRF51 if that means anything to you.

https://flipsky.net/collections/accessories/products/core51822-ble4-0-bluetooth-2-4g-wireless-module-nrf51822-onboard-ws82013
```

---
## \#707 Posted by: Ackmaniac Posted at: 2018-10-09T13:53:43.836Z Reads: 211

```
Never thought about it. Maybe there is a chance, maybe not. Feel free to send me one so that i can have a look at if i find the time. But at the moment my time is very limited so it could take a while.
```

---
## \#708 Posted by: lrdesigns Posted at: 2018-10-26T06:46:04.386Z Reads: 215

```
Hey @Ackmaniac I just switched from your old BLDC Tool firmware to the new ESC Tool with 3.102. 

I run BLDC. Hardware 4.12 maytech.

There was a setting in the old tool called "Max ERPM at full brake" that I really liked. If you lowered the number it made the brakes from mid to low speed really smooth and linear as the speed decreased. Now I find in this speed range it feels like the brakes are increasing in power as I slow down even when keeping the remote brake level constant. So I have to release the brake a little and it feels grabby or like its latching. As I release it a little goes from a lot of brake to basically none. 
![image|403x136](upload://q4pLCd2n8yx7DqeuKZqCUqJTi8N.png) 

Is there any equivalent in the new tool? I don't see anything. 
![image|690x211](upload://7Fgwi2J5pbPR8DS5spfZemZGyAr.png) 

Other than that the new firmware is great, much smoother startup from zero speed. 

Thanks for all the work you put in for the community.
```

---
## \#709 Posted by: Ackmaniac Posted at: 2018-10-26T07:32:33.846Z Reads: 204

```
Please post your motor and battery amp settings.
```

---
## \#710 Posted by: lrdesigns Posted at: 2018-10-29T00:53:50.744Z Reads: 206

```
X2 motors dual. 5065 140kv, 18:36 ratio on 97mm wheels. 12s Lipo. 

I kinda got used to it at mid speed just need to use less brake on the remote. But low speed to stop is still grabby. Also its more weird on a downhill then flat ground. 

![image|387x334](upload://sETeljWBgCqco9l6tpFZUy4q17y.png) 

I did change minimum current and start up boost for cleaner starts. 
![image|618x189](upload://ikF4z7uP1Q02IEWnwPdvC4ips3C.png) 
![image|582x88](upload://74hnTgs9hAjuw8npsRbjyAYYtdT.png)

I had to do an emergency brake from top speed this morning as a car pulled out in front me. It made me think about putting the battery regen higher for some more stopping power at speed.
```

---
## \#711 Posted by: isabar Posted at: 2018-10-29T12:41:24.500Z Reads: 197

```
@Ackmaniac I want to confirm that when using 2 VESCs connected via CANBUS, that if you change to a different MODE (e.g., a mode that limits the top speed to 10 mph) in ESC Monitor App, it will automatically write to both VESCs? 
For this to work properly, can you confirm what settings the following should be set to on Master vs Slave?
1) SEND CAN STATUS? true or false?
2) MULTIPLE ESCS OVER CAN? true or false?
Also when changing Modes via the app, does it matter whether you are connected to the master vs the slave? in either case, will it apply the changes to both Master and Slave?

Also, if you choose to have the mode change now become the default mode (by long pressing in the upper corner window) does this also automatically apply the change to both Master and Slave?

Finally if you switch between BLDC and FOC, does this automatically apply to both Master and Slave?

Thanks in advance for your help with this!
```

---
## \#712 Posted by: pierres Posted at: 2018-10-30T10:29:15.647Z Reads: 192

```
Thanks @Ackmaniac everything worked fine
Two comments 
1)I cannot input more than one digit in the max speed field. 3 is ok but not 30 for example. It worked before... 
2) with two vesc, when using TCP relay (my BT module being on slave uart) Which CAN FW field is active? The one in vesc tool? The one in the app? Both? For example when can fw is activated in the mobile app, what happens when it is active in the vesc tool too?
```

---
## \#713 Posted by: Ackmaniac Posted at: 2018-10-30T21:02:12.348Z Reads: 199

```
@lrdesigns You have already a max regen of -15A for each VESC which should be high enough. Maybe it is a phenomenon of your motors that the VESC can't detect the correct current's at high speed.

@isabar   
1. SEND CAN STATUS? true or false?
Master=false, Slave = true
2. MULTIPLE ESCS OVER CAN? true or false?
Master=true, Slave= false (doesn't matter)
Also when changing Modes via the app, does it matter whether you are connected to the master vs the slave? in either case, will it apply the changes to both Master and Slave?
Only when you are connected to the master. Means you need to see that realtime data of the master. 

And when you overwrite the default it also needs to be connected to the master. Otherwise it only does it for the slave.

@pierres 
[quote="pierres, post:712, topic:35116"]
1)I cannot input more than one digit in the max speed field. 3 is ok but not 30 for example. It worked before…
[/quote]
have no explanation for that. Maybe reinstall the app

[quote="pierres, post:712, topic:35116"]
2) with two vesc, when using TCP relay (my BT module being on slave uart) Which CAN FW field is active? The one in vesc tool? The one in the app? Both? For example when can fw is activated in the mobile app, what happens when it is active in the vesc tool too?
[/quote]
Then simply all are asking the VESC at the same time which can cause trouble. Especially during motor detection you should avoid that.
```

---
## \#714 Posted by: isabar Posted at: 2018-10-31T07:36:44.677Z Reads: 189

```
@Ackmaniac
If you switch between BLDC and FOC, does this automatically apply to both Master and Slave?
```

---
## \#715 Posted by: Ackmaniac Posted at: 2018-10-31T20:03:46.651Z Reads: 184

```
When you send the command to the master then yes.
```

---
## \#716 Posted by: cathode Posted at: 2018-11-01T02:18:44.419Z Reads: 192

```
Hey @Ackmaniac !  Awesome tool you provide !  But i'm struggling a bit with fimwares... if you have some time to share, that's would be nice :slight_smile:

I'm currently using "regular" vesc-tool from vedder website and i'm looking to use the watt-mode i was running on the "old" BLDC-tool Ackmaniac version 'cuz it's was cool.

So I get "_ACKMANAIC_-ESC Tool 0.2" ( --> https://puu.sh/BUhBW/187758e944.png lul) but watt mode didn't showed up, maybe I have to do some extra tweaks before using it but i can't figure them out T-T 

Can you or some other cool users help me out ?
That's would be great :wink: 
Thanks dudes.
```

---
## \#717 Posted by: Ackmaniac Posted at: 2018-11-01T17:27:44.629Z Reads: 189

```
The Current mode is like Watt mode. In the newer firmwares the old current mode doesn't exist anyomre. You can regulate it by the current or by watt in the motor settings.
```

---
## \#718 Posted by: cathode Posted at: 2018-11-01T17:58:00.281Z Reads: 190

```
Copy that ! Hey that's was easy :) thanks
```

---
## \#719 Posted by: lrdesigns Posted at: 2018-11-02T00:46:54.120Z Reads: 197

```
Thanks @Ackmaniac for the advice. But it does not answer my question. I just want to know if the "Max EPRM at full brake" is totally gone from the new ESC Tool? Or if there is an equivalent setting? 

I know you didn't build the new tool, I just thought you might know why this feature is gone?

![image|502x204](upload://7G9FzQiWwFauJS4638wWp5ssM5k.png) 

The "Max EPRM at full brake" only affected the 5 to 0 mph behaviour. I found adjusting it made the brakes very linier, as in as the speed lowered so did the brake force. 

I have gotten used to the feel of the brakes in high and mid speed now with the new tool, so it's not an issue.
```

---
## \#720 Posted by: Vanarian Posted at: 2018-11-05T22:32:31.679Z Reads: 197

```
Hey how do you set it to get smooth brakes? You raise it or you lower it?
```

---
## \#721 Posted by: lrdesigns Posted at: 2018-11-06T00:32:52.708Z Reads: 197

```
Lower than default, I’m on 140kv motors though. I think each motor will behave different.
```

---
## \#722 Posted by: Vanarian Posted at: 2018-11-06T19:21:06.815Z Reads: 200

```
Thanks for the tip. I got pretty low KV overall on my motors, 75kv and 85kv hubs and a pair of 170kv so should have kinda similar effects !
```

---
## \#723 Posted by: Fiori Posted at: 2018-11-07T07:07:31.188Z Reads: 195

```
Did you ever find a solution? I am running into the same issue. I get realtime data intermittently, it was working perfect until the last few updates.
```

---
## \#724 Posted by: MiniChopper4Me Posted at: 2018-11-24T22:56:37.903Z Reads: 185

```
Sorry, I'm really late to the party.  Can I use Ackmaniac FW on Flipsky 4.20 dual?  I like being able to use forward and reverse with brake, and this firmware seems to be the master of that functionality.

Should I just stick to the default or go with this instead? Oh yeah, running 10S BLDC of course.
```

---
## \#725 Posted by: Pantata Posted at: 2018-11-24T22:57:47.010Z Reads: 185

```
Use Ackmaniac definitelly, there are no cons... ANd with the safety brake future and all other stuff, there is no debate :slight_smile:
```

---
## \#726 Posted by: MiniChopper4Me Posted at: 2018-11-24T22:58:36.257Z Reads: 182

```
Thanks, now I just need to read 700 posts.
```

---
## \#727 Posted by: Pantata Posted at: 2018-11-24T22:58:55.977Z Reads: 181

```
lol why? what do you need to know?
```

---
## \#728 Posted by: MiniChopper4Me Posted at: 2018-11-24T22:59:51.445Z Reads: 190

```
lol, just where to download, settings to lookout for etc.  I got the jist of it, just don't want to go to the hospital for being lazy and not reading up :stuck_out_tongue:

Am I correct in that bluetooth modules don't work with the 4.20?
```

---
## \#729 Posted by: Pantata Posted at: 2018-11-24T23:02:12.098Z Reads: 188

```
https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0
```

---
## \#730 Posted by: Pantata Posted at: 2018-11-24T23:03:21.598Z Reads: 183

```
ANd I was having troubles finding the firmware... is this the first time setting up vesc based esc for you?
```

---
## \#731 Posted by: Pantata Posted at: 2018-11-24T23:04:14.994Z Reads: 188

```
Blutooth modules work fine with 4.2, it's just some phones and android versions don't wanna work with the module
```

---
## \#732 Posted by: MiniChopper4Me Posted at: 2018-11-24T23:05:29.515Z Reads: 191

```
No, I set it up using the free vedder ESC.  Not being cheap, just cautious.  I got through my first setup and it works fine, just wanted to start playing with the +es
```

---
## \#733 Posted by: Pantata Posted at: 2018-11-24T23:06:24.707Z Reads: 187

```
I can send you the ackmaniac firmware file If you give me your email.
```

---
## \#734 Posted by: adrienfeve Posted at: 2018-12-09T10:06:03.821Z Reads: 185

```
I am currently using the Vedder's VESC Tool 0.95. I downloaded Ackmaniac ESC-Tool now as I have issues with the bluetooth connection using the original firmware. What is the process to change the VESC firmware to Ackmaniac custom one?
```

---
## \#735 Posted by: skatardude10 Posted at: 2018-12-09T15:49:07.770Z Reads: 185

```
Boot Ackmaniac's ESC tool, connect to the vesc, go to the firmware tab, make sure correct version is selected and hit upload, done 👌
```

---
## \#736 Posted by: adrienfeve Posted at: 2018-12-10T05:48:54.378Z Reads: 180

```
Thanks! Will this override my current vesc settings?
```

---
## \#737 Posted by: skatardude10 Posted at: 2018-12-10T16:15:49.733Z Reads: 178

```
Yes. You can export your current settings and import them after updating I think.
```

---
## \#738 Posted by: jadatmag Posted at: 2018-12-15T15:59:54.583Z Reads: 174

```
Is there a way to change between UART and PPM input from the Android monitoring app?

Would be great so I can switch between my 2 remotes on the fly! Maybe a feature request?

@Ackmaniac
```

---
## \#739 Posted by: Bjork3n Posted at: 2018-12-17T22:43:13.770Z Reads: 171

```
@Ackmaniac Any chance for an updated fw with bluetooth connection support? 
Just to be able to change settings with the Metr pro wihout plugging in that usb wire. I know vesctool 3.4 support this =)
```

---
## \#740 Posted by: jadatmag Posted at: 2018-12-23T01:21:14.621Z Reads: 179

```
My Bluetooth module is connected to my slave Focbox. I can read the settings (speed, amps,volts, etc) fine from the ESC monitor Android app. But whenever I try to write settings (motor max, motor min, etc.) nothing happens. The same happens on the ios apps. Writing doesn't seem possible. Is there some setting I'm overlooking?

Anyone any thoughts on this?

Edit: 1 out of 10 times the ios app does write succesfully. But when I read the settings on PC I see that only one ESC got updated with the new settings.

Edit 2:
there is a can forward function in the ios app so seems logical, still only works 1 outta 10 times
0 outta 10 times with the ESC monitor android app (connect by CAN to ID = 0 which is the master on the ESC monitor android app is checked)
```

---
## \#741 Posted by: Ackmaniac Posted at: 2018-12-23T10:25:48.396Z Reads: 173

```
I don't have a ios app so I guess you are talking about the app of someone else.
```

---
## \#742 Posted by: jadatmag Posted at: 2018-12-23T11:29:29.810Z Reads: 181

```
I think you skimmed my post too fast :stuck_out_tongue: it happens on your ESC monitor android app (reading fine but no writing). As additional info I tell that the iOS app (eskate vesc) doesn't work good either (reading is fine, writing works 1 outta 10 times). The problem I have isn't necessarily located in your app but seems to be somewhere else.

I'm on version 3.102 on the FOC boxes.

And I've seen posts about adding support for writing from slave yesterday but that was from a loooong time ago.

Edit:
Could it be that the reading goes over different wires than the writing? On visual inspection my Bluetooth module wires seem fine though.

Edit 2:
As suggested by emmaanuel I will be looking into a better Bluetooth module.

Edit 3:
I just waterpoof closed my box with hot glue and ducktape, so I'll be looking onto writing from Bluetooth again the next time my board needs maintenance or my new receiver from aliexpress arrives. Thanks a bunch!
```

---
## \#743 Posted by: Ackmaniac Posted at: 2018-12-23T13:57:32.068Z Reads: 176

```
Make sure you are connected to the master when you try to write and writing only works with ppm, nrf or nunchuk remotes. Not adc.
```

---
## \#744 Posted by: jadatmag Posted at: 2018-12-24T16:49:38.069Z Reads: 182

```
Tnx for the help! I decided to order the Metr pro module to have more control at my finger tips. I have the Photon remote connected to my master and like to keep it that way. If this won't work in the end I Will switch back to a ppm remote and switch the photon remote to a different board.

In the meantime I'm trying to set my max motor temp to 125C.

https://youtu.be/k1vCyAVkgNg

It won't let me input something higher than 120 at the end. Am I missing something?
```

---
## \#745 Posted by: Psmrman90 Posted at: 2019-01-03T01:01:20.605Z Reads: 187

```
Any ideas why my ackmaniac doesn't work with my enertion dual vesc?  It is being recognized and able to pair, but once it pairs there is no battery data shown.  Perhaps i need to split them and wire them like two individual vescs, im guessing the capacitor junction/area is where my issue is, but not sure
![Screenshot_20190102-175750|243x500](upload://kLGijdKRjA4dqNufC6RxqVE2yjF.jpeg) 

 ![20190102_175850|243x500](upload://8WH6KCCcgWDVLMOiitGe9om65tF.jpeg)
```

---
## \#746 Posted by: Benjamin899 Posted at: 2019-01-03T01:03:32.964Z Reads: 176

```
sometimes you need to do a reconnect, try it.
```

---
## \#747 Posted by: Psmrman90 Posted at: 2019-01-03T01:12:45.885Z Reads: 187

```
Did, no change.
```

---
## \#748 Posted by: Ackmaniac Posted at: 2019-01-17T14:04:42.876Z Reads: 177

```
I just released a new version 3.103
It enables the possibility to change modes for ADC remotes via the app and fixes a little bug when you use NRF remotes.
It's only a little change and if you don't use nrf or adc remotes then you don't need to update.
```

---
## \#749 Posted by: Ackmaniac Posted at: 2019-01-17T14:06:03.801Z Reads: 180

```
Please check that rx at the module is connected to tx at the vesc and vice versa. And also connect VCC to the 5V pin of the VESC. Then you need to set the baudrate of 9600 at the VESC.
```

---
## \#751 Posted by: Songsta Posted at: 2019-01-26T08:43:08.598Z Reads: 179

```
I can't get the tool working either. I've checked the connections to make sure are correct as give here:

[quote="Ackmaniac, post:749, topic:35116"]
the vesc and vice versa. And also connect VCC to the 5V pin of the VESC.
[/quote]

The only thing that was different was the VCC that was connected to the VCC and now 5V. I've now changed that.

In the ESC tool in Windows I've changed the baud rate to 9600 but still no luck. This is what I keep getting:

![Screenshot_20190126-103924_ESC%20Monitor|243x500](upload://uchStcsrQFgD9guDtU8bwluiACS.jpeg) 


I've updated the firmware too. Any help would be appreciated. I'm stuck using the standard vesc android tool, which isn't great.
```

---
## \#752 Posted by: Songsta Posted at: 2019-01-26T09:25:12.694Z Reads: 172

```
I've got the trampa BLE module. I think that's the reason...
```

---
## \#753 Posted by: taz Posted at: 2019-01-26T09:41:28.286Z Reads: 169

```
I am trying to get ackmaniac monitor to work but I am unsuccessful with both of my boards.
One has a Metr Pro module with Focboxes and 3.40fw and the other the Trampa module with Vesc6 and 3.40fw.
Both work with the android version of the VESC tool and of course the Metr Pro also with the metr app.
```

---
## \#754 Posted by: Ackmaniac Posted at: 2019-01-26T10:05:36.562Z Reads: 171

```
Yes, these modules are different and only work with their own app.
```

---
## \#755 Posted by: Ackmaniac Posted at: 2019-01-26T10:08:10.715Z Reads: 177

```
Both of these modules don't work. Don't know why the metr pro doesn't?
```

---
## \#756 Posted by: taco Posted at: 2019-01-27T08:13:41.668Z Reads: 173

```
This is fantastic, do not hesitate to install the firmware!  I used the latest OSX build to install it on both FOCBOXes in my LaCroix.  The process was painless aside from I forgot to turn on UART again after flashing and completing motor/input configs :slight_smile: so I lost my bluetooth connection for a minute until I figured that out and re-enabled UART. Its a huge improvement over the stock throttle controls which were... downright terrifying as a relative newcomer to eSkates.
```

---
## \#757 Posted by: b264 Posted at: 2019-02-01T09:30:51.241Z Reads: 173

```
Tool with firmware 3.103 for Linux available here

https://github.com/b264/vesc_tool/tree/87849d57a514c0c63bf4cee0e82eab6ab512440c/build/lin
```

---
## \#758 Posted by: butt_stallion Posted at: 2019-02-06T13:45:10.532Z Reads: 171

```
Would this firmware work on the unity?
```

---
## \#759 Posted by: Ackmaniac Posted at: 2019-02-06T15:45:06.028Z Reads: 171

```
No. There is no support for the second motor in my firmware mod.
```

---
## \#760 Posted by: Deakbannok Posted at: 2019-02-10T22:35:16.949Z Reads: 177

```
after i have updated to 3.103 now both of my vescs BLE is not working on both of them.
```

---
## \#762 Posted by: Deakbannok Posted at: 2019-02-14T08:10:06.740Z Reads: 170

```
Yep problem with the FW x.103. Both of my VESC are not working. Cannot connected to UART/BLE.
```

---
## \#763 Posted by: Ackmaniac Posted at: 2019-02-14T08:58:19.994Z Reads: 171

```
Did you test the connectivity with 3.102 shortly before you updated? Because i guess because of the winter you didn't test it for a while and since the last time you used it your smartphone upgraded to android 8 which doesn't work with a lot of  BLE module clones.
But that is only a wild guess. 3.103 works the same as the old version and i have no issues.
```

---
## \#764 Posted by: RyuX Posted at: 2019-02-20T19:57:25.178Z Reads: 160

```
Hey there.
I have a similar problem.
I updated to 3.103 - now I can't connect with the ESC Monitor via bluetooth anymore. Also when connecting over the TCP Bridge I can only Read APP and MOTOR values but when I try to write it will not write to the VESC.
any hints ?
Thanks
```

---
## \#765 Posted by: ron Posted at: 2019-02-21T15:27:55.810Z Reads: 156

```
Hi there!  Is the Ackmaniac FW still the better FW and the way to go? I'm asking for 4.12 and 6.4 HW Versions. I know it was praised a year ago but don't know how this firmware stands to the "original" FWs after a year now.  Thank you very much! :)
```

---
## \#766 Posted by: Deakbannok Posted at: 2019-02-21T15:40:14.781Z Reads: 152

```
When I had 3.102 installed. Everything was working fine. But now all my UART and Bluetooth is not getting any feedback from VESC. I have tried to switch a new BLE and changed BR. Nothing is work.
I need to switch back to 3.102 FW.

Can anyone please provide me an alternative link to download the previous FM
```

---
## \#767 Posted by: Ackmaniac Posted at: 2019-02-21T15:45:53.475Z Reads: 147

```
Did it work directly before you switched to the new firmware or was that some months before? (Asking because of Winter and maybe your Smartphone Android Version changed)
Only think i can imagine is the change in the COMM_GET_VALUES where the controller Id was added which can lead to a new package that was send and your BLE module might get trouble with that. 
Send me a PM with your email and i can send you the previous version to test if it makes a difference
```

---
## \#768 Posted by: Ackmaniac Posted at: 2019-02-21T15:47:51.365Z Reads: 144

```
Do you want to start a fight :crazy_face:?
```

---
## \#769 Posted by: mmaner Posted at: 2019-02-21T15:48:27.327Z Reads: 142

```
Yes &nbsp;
```

---
## \#770 Posted by: mmaner Posted at: 2019-02-21T15:48:40.123Z Reads: 142

```
Yes &nbsp; :)
```

---
## \#771 Posted by: Deakbannok Posted at: 2019-02-21T15:50:00.191Z Reads: 143

```
Yes. It was working fine before I have uploaded to a new FW. I have been using the same phone (NOTE 5)
```

---
## \#772 Posted by: ron Posted at: 2019-02-21T15:58:02.256Z Reads: 158

```
Maybe! :) ... It was a genuine question. Wasn't tracking your FW/Tool the last year so I am kinda not up to date anymore...

So. Is it also recommendable for the 6.4HW based ESCs?

But if you want so: "Leeets get reeeeadyyyyy toooo ruuuuummble" :woozy_face:
```

---
## \#773 Posted by: trampa Posted at: 2019-02-21T16:47:58.073Z Reads: 168

```
VESC-Tool just got a major update with 20K lines of new code. Have a look and compare yourself. If you haven't followed things up for a year, you will need to do some reading. 

https://www.electric-skateboard.builders/t/all-new-2019-vesc-tool-release/83619?u=trampa
```

---
## \#774 Posted by: Ackmaniac Posted at: 2019-02-21T17:02:32.982Z Reads: 173

```
What i saw so far is that the User Interface changed.
The Motor detection changed.
But when it comes to the control of the Motors in FOC (which most use) then the only real change i can see is smoothening of the transition when you brake shortly before you come to a complete stop, which was basically the idea of @Deodand and is a change of less than 10 lines of code.
And i think i saw a change if you use encoders.
So apart from the User Interface there isn't much that has changed yet when you have already a good working setup.
But i have the feeling that Benjamin will concentrate on motor control optimizations in the future now that he has the User Interface as he want's it. Field weakening for higher speeds would be interesting or Field Injection for sensorless motors.

But personally i think my firmware mod is still better when it comes to the controllability and ride and feel of a electric skateboard (watt control, timeout rampening, traction control offset, cruise control with PPM remotes, different power levels for front and back axle for 4wd).

But everybody can judge themself. I don't have a business interest and simply changed the stuff that i didn't like and that i was capable of.

Benjamin is for sure much more talented and has a much bigger knowledge. But i think his focus is on a universal motor controller for all kind of motors (which is impressive) and i focus on controllability of a electric skateboard with a human body on top of it which can't react as fast as a Microcontroller can do.
```

---
## \#775 Posted by: Benjamin899 Posted at: 2019-02-25T20:11:44.930Z Reads: 161

```
i also can't connect my focbox with your tool since the update. I used the USB connection. Mobile app still works.
```

---
## \#776 Posted by: pookybear Posted at: 2019-02-26T01:29:20.271Z Reads: 159

```
Not sure if this was asked before. Version 3.103. Does it have the low speed brake fix?
```

---
## \#777 Posted by: skatardude10 Posted at: 2019-02-26T01:30:02.440Z Reads: 160

```
No

....10char....
```

---
## \#778 Posted by: pookybear Posted at: 2019-02-26T01:33:28.164Z Reads: 156

```
Well. Ummm does it need it? I only ran the fix on my unity.
```

---
## \#779 Posted by: skatardude10 Posted at: 2019-02-26T01:35:20.857Z Reads: 156

```
It's not a deal breaker not having it unless your having an issue with it imo. 

If you run FOC and experience excessively strong brake locking right before stop and it's annoying you, the fix is great to have. Otherwise no
```

---
## \#780 Posted by: sainttjames Posted at: 2019-03-02T11:53:53.520Z Reads: 158

```
@rey8801

Replying to your comment in the Unity thread. 

I have found the @Ackmaniac app/tool completely reliable. No connectivity issues at all... since I bought a new Android phone. My previous Android, a Samsung, had problems all the time.

Now I'm on a OnePlus which is not full of bloatware...I turned off power management for the @Ackmaniac tool and have had no connectivity issues whatsoever.

So, check your phone if your having issues.
```

---
## \#781 Posted by: rey8801 Posted at: 2019-03-02T12:00:08.749Z Reads: 157

```
Hi man. Are you using it with the unity? Because I have been using this app over a year with other vesc and it worked perfectly. I have problem now with the unity which is a known compatibility issue.
```

---
## \#782 Posted by: sainttjames Posted at: 2019-03-02T12:28:49.559Z Reads: 156

```
Hey, 

No, I got two Focboxes running with Ackmaniac firmware and controlling via the app. Doesn't the Unity have its own software?
```

---
## \#783 Posted by: rey8801 Posted at: 2019-03-02T12:40:41.701Z Reads: 160

```
Ah Yeh focbox, vesc 6 ecc are perfect with the app. I was talking about the unity. It is based on vesc software. You have UART port ecc. It's just not optimazide yet. I hopo @Ackmaniac will find the time to make it compatible.
```

---
## \#784 Posted by: sainttjames Posted at: 2019-03-02T12:47:02.188Z Reads: 158

```
Sorry man, I want even aware that people were trying to run the Unity on Ackmaniac's software! My bad.
```

---
## \#785 Posted by: rey8801 Posted at: 2019-03-02T12:52:29.262Z Reads: 160

```
No problem. Thank you for trying to help! Appreciate
```

---
## \#786 Posted by: pookybear Posted at: 2019-03-03T05:15:10.245Z Reads: 161

```
When I activate cruise control on my remote, somehow speed doesn't stay on where I want it. It slowly ramps up to its top speed. Does the firmware have a setting/settings for this?

Feather remote.

Thanks
```

---
## \#787 Posted by: Ackmaniac Posted at: 2019-03-03T09:48:54.026Z Reads: 166

```
Seems that your throttle signal changes when you activate the steering on your remote. Best would be to chack that in the tool. Just connect to the master where your throttle is connected. Activate the throttle realtime and check if the throttle ppm signal changes if you activate the steering channel which is connected to the slave.

If that is the case then it might help to increase the deadband a bit.
```

---
## \#788 Posted by: pookybear Posted at: 2019-03-03T20:19:51.084Z Reads: 162

```
Cruise control is activated on the feather remote via the trigger button. As soon as I set the speed, I let go of the thumb throttle and just press on the trigger button. But this slowly ramps up to the top speed. 

For some reason, I couldn't get the cruise control on my mini remote so I switched to the feather one since I'm going to be mainly using it anyway.

Thanks for the awesome firmware. Donation coming your way as I type this. Appreciate the time and effort you put into this
```

---
## \#789 Posted by: Ackmaniac Posted at: 2019-03-04T00:16:04.684Z Reads: 165

```
Well, I don't really know how the feather remote is doing cruise in detail. Don't have one myself. Is the firmware available? And please check if the throttle signal changes when you press the cruise button via the ealtime app data in the ackmaniac tool.
```

---
## \#790 Posted by: pookybear Posted at: 2019-03-04T01:06:06.063Z Reads: 167

```
I'll do the realtime app data test.

Here's the firmware source:

https://www.electric-skateboard.builders/t/featherremote-and-smartremote-files-in-post-577/74084/589
```

---
## \#791 Posted by: StefanMe Posted at: 2019-03-04T08:20:42.558Z Reads: 164

```
It doesnt work like that... 

My cruise control just simultes a permament PPM signal at the throttle position u pressed the cruise control button like the originals cruise mode from SolidGeek. In Current Control Mode it doesnt really work in low speeds. I ll take a look into the Original VESC Cruise control. DroidSector has done it...
```

---
## \#792 Posted by: b264 Posted at: 2019-03-04T08:47:27.994Z Reads: 175

```
[quote="Ackmaniac, post:774, topic:35116"]
But personally i think my firmware mod is still better when it comes to the controllability and ride and feel of a electric skateboard (watt control, timeout rampening, traction control offset, cruise control with PPM remotes, different power levels for front and back axle for 4wd).
[/quote]

Why not submit these changes to the upstream repo so it's also in Vedder's releases?
```

---
## \#793 Posted by: trampa Posted at: 2019-03-04T10:01:48.077Z Reads: 171

```
[quote="b264, post:792, topic:35116"]
cruise control with PPM remotes
[/quote]

- Cruise control with PPM remotes creates a ground loop and can damage your ESC! Such a feature  should not exist! People potentially blow up their ESCs using that feature. Technically wrong, especially with more different Hardware hitting the market. 
- Timeout ramping could be a good feature if you have a reliable detection of remote cutouts (which highly depends on your remote and receiver) Benjamin will ad that, but priority is a remote connection that does not cut out in the first place and has a safe detection for connection issues. Rather than messing around with subpar black box RC recievers, Benjamin focuses on a nice way to handle the issue.
- different power levels for front and back axle for 4WD (how many 4 WD builds needing such a feature exist in reality?) 4WD torque vectoring would be more handy for such builds. A fixed power level shift is possible already with stock FW.
```

---
## \#794 Posted by: b264 Posted at: 2019-03-04T20:10:35.957Z Reads: 171

```
Not if you use 2 receivers.
```

---
## \#795 Posted by: Bjork3n Posted at: 2019-03-11T18:46:46.457Z Reads: 169

```
Just tried the reverse function (current mode).
Its perfect!
Just like a boosted board!

I had to turn on traction control to get it to work perfectly. 
Super useful. 
Very nice that you can brake fully and keep it "handbraked" and that it only reverses when i press the brake for the second time!
Great work @Ackmaniac
https://youtu.be/Wi5o-pgJ8Kg
https://youtu.be/Tid5HN1I0p0
```

---
## \#796 Posted by: Vanarian Posted at: 2019-03-11T19:27:27.317Z Reads: 163

```
Does the reverse work like a RC car ? Like a "Trigger backwards = Brake then reverse" and " trigger forward = accelerate forward"?
```

---
## \#797 Posted by: Bjork3n Posted at: 2019-03-11T19:28:48.571Z Reads: 164

```
Brake gives brake but if i touch the brake again when stopped it reverses
```

---
## \#798 Posted by: Vanarian Posted at: 2019-03-11T19:30:55.091Z Reads: 166

```
Ok so when you wanna brake while in reverse you press throttle? And it does the same (brake till stop and press again to go forward again)?

Edit : Dumb question but just to be sure ,I had a long day lol
```

---
## \#799 Posted by: Bjork3n Posted at: 2019-03-11T19:39:26.245Z Reads: 167

```
No when i reverse and press foward it brakes and then moves foward. No need to double tap foward.
```

---
## \#800 Posted by: skatardude10 Posted at: 2019-03-11T19:42:29.384Z Reads: 170

```
This is such a nice function to have a stop lights and cross walks... I use it constantly, I couldn't imagine not using it.
```

---
## \#801 Posted by: Bjork3n Posted at: 2019-03-11T19:47:54.418Z Reads: 175

```
I only regret not using it sooner 😂
```

---
## \#802 Posted by: Ackmaniac Posted at: 2019-03-11T21:59:04.894Z Reads: 168

```
Appreciate it, thx.
```

---
## \#803 Posted by: RyuX Posted at: 2019-03-12T16:58:01.081Z Reads: 173

```
Does anyone still have Ackmaniac 3.101 Firmware somewhere ? I would like to use this one as it is supported by the metr.at app - and I can't get the ackmaniac tool to work on my android phone. Thanks
```

---
## \#804 Posted by: Bjork3n Posted at: 2019-03-12T17:21:32.656Z Reads: 173

```
Metr supports Ackmaniac 3.102 fw. 

If you have the old metr module and updated your phone to android 8 the old metr wont work anymore. Then you need the metr pro.
```

---
## \#805 Posted by: RyuX Posted at: 2019-03-12T17:27:23.130Z Reads: 173

```
Thanks for the reply.. I have Android 8 and with Ackmaniac 3.102 I can't write the Modes anymore.. However I tried 3.100 and it works without problems (i have the old metr.at module).
So I wanted to try if 3.101 is working as well as 3.100..
If not I will just stay on 3.100
```

---
## \#806 Posted by: Bjork3n Posted at: 2019-03-12T17:29:35.550Z Reads: 175

```
Thats weird that the old metr module works on android 8. 
 I couldnt even get the old module to connect with my phone with android 8. (Samsung s7).
Got a metr pro and i use the modes feature all the time with the ackmaniac 3.102.

If you use canbus use the 3.101 with the fixed braking problem that the 3.100 had.
```

---
## \#807 Posted by: RyuX Posted at: 2019-03-12T17:34:49.334Z Reads: 165

```
I don't use the canbus - I also have a S7 Edge with the newest Android. So I will keep 3.100 then. It is essential for me to be able to switch to a "locked" mode when my board will only reach a maximum of 16 km/h in Case I ever get pulled by the police.
```

---
## \#808 Posted by: Bjork3n Posted at: 2019-03-12T17:35:57.447Z Reads: 166

```
Yeah i also have a mode called "police". Then the board is slow as a turtle no matter how much you push the throttle :joy:
```

---
## \#809 Posted by: pookybear Posted at: 2019-03-12T17:44:38.543Z Reads: 165

```
So wait. Metro pro works w ackmaniac? FW 3.102? How did you get it to work?
```

---
## \#810 Posted by: Bjork3n Posted at: 2019-03-12T17:45:53.500Z Reads: 166

```
Yes it works? Why wouldnt it? :P 
Metr pro supports most fw´s
```

---
## \#811 Posted by: pookybear Posted at: 2019-03-12T17:47:33.489Z Reads: 165

```
What the... I just checked. I have FW 3.103. I'll play w this again tonight.

Thank you!
```

---
## \#812 Posted by: Moza Posted at: 2019-03-18T18:32:26.096Z Reads: 162

```
Hi guys.

Anyone know if there's been any advance on changing modes for ackmaniac Vesc monitor for Android.

Last time I checked it wasn't possible to change modes when using ADC. (I'm using Bluetooth hm-10 module)

Oh waite, sorry, I've just looked back on the posts and it looks like you can!! Excellent. Update to 3.103.
```

---
## \#813 Posted by: pookybear Posted at: 2019-04-05T19:53:40.050Z Reads: 149

```
I have mixed results on researching whether vesc6 is compatible with ackmaniac firmware. I don't want to try upload it as I don't have ST-Link. 

Is it compatible?
```

---
## \#814 Posted by: rey8801 Posted at: 2019-04-05T22:40:11.474Z Reads: 146

```
I used for months with Flipsky6.6 and it worked fine.
```

---
## \#815 Posted by: pookybear Posted at: 2019-04-05T22:52:08.256Z Reads: 145

```
Yaaasss! So stoked. I really like this firmware.
```

---
## \#816 Posted by: rey8801 Posted at: 2019-04-05T22:53:49.343Z Reads: 144

```
It's really nice. Pity it is not unity compatible.
```

---
## \#817 Posted by: pookybear Posted at: 2019-04-05T22:56:58.212Z Reads: 145

```
Yea. Not really impressed w unity. It's convenient and all but I like redundancy on my setup. Additionally w dual Vesc, you can easily add peripherals w extra ports from the second Vesc. I might be selling mine pretty soon.
```

---
## \#818 Posted by: rey8801 Posted at: 2019-04-05T22:58:56.214Z Reads: 137

```
I keep unity because it save so much space... Enertion will release a similar telemetry app. The question is when? :thinking:
```

---
## \#819 Posted by: pookybear Posted at: 2019-04-05T23:03:41.484Z Reads: 139

```
It does! But I have no issues w space at the moment. :+1:t4:
```

---
## \#820 Posted by: trampa Posted at: 2019-04-06T08:57:22.915Z Reads: 141

```
The telemetry is coded already, Benjamin has nailed that in VESC-Tool. Unity runs of modified VESC code, but they made the decision to create incompatibilities, so that users can't use VESC-Tool. Until you can enjoy the new VESC-Tool features in the Enertion VESC-Tool fork it may take a while, depending on how fast they can integrate the Vedder Code.
```

---
## \#821 Posted by: rey8801 Posted at: 2019-04-06T08:59:11.558Z Reads: 143

```
Thank you for the explanation. So the data are all there, the part missing in the software to show them.
```

---
## \#822 Posted by: trampa Posted at: 2019-04-06T09:07:02.381Z Reads: 147

```
The data has always been there. The question is what you make from the data set and how you display it. Have a look at the mobile VESC-Tool. You have access to all data from all VESCs in an array and the software combines all data from all VESCs to a useful and accurate set of data. This way you don't only use the data from one VESC to project for example estimated range and Wh usage. This bit was a bit tricky to code.
```

---
## \#823 Posted by: rey8801 Posted at: 2019-04-06T09:11:35.513Z Reads: 144

```
I know VESC-tool and I have been using telemetry for a while. I was actually surprise that the current apps don't work with Unity, but yeh I guess is a way to dissociate from the other competitors.
```

---
## \#824 Posted by: trampa Posted at: 2019-04-06T09:25:51.398Z Reads: 149

```
Sure, but most of it is still Vedder Code. The difference is in using a single processor to run two ESCs. This is fundamentally against compatibility and locks you to use a special, modified software fork of VESC-Tool. For app developers it's not a lot of fun to code for different software solutions. In my eyes it's better to work on one consistent software release that is max compatible.
```

---
## \#825 Posted by: rey8801 Posted at: 2019-04-06T10:18:20.227Z Reads: 153

```
Sure I agree. A single software would be the best. But then why dual esc like Flipsky are compatible? I though that the main problem was the HM10 module since with nrf like metr also unity works.
```

---
## \#826 Posted by: trampa Posted at: 2019-04-06T13:20:06.637Z Reads: 155

```
Because these dual ESCs are made in a way that they are software compatible. Two supported processors run two supported DRV chips. The module needs to be NRF 51 or 52 based. HM10 is to slow for FW updates and reliable RT data.
```

---
## \#827 Posted by: mmaner Posted at: 2019-04-06T13:47:43.320Z Reads: 158

```
I think enertion made the decision to build the unity with a single proc for price-ability. It's much cheaper to buy a Unity for a dual motor setup than x2 Trampa VESC's. 

The divergence from vesc tool compatibility is also a product of building a better and cheaper controller. When you force people to change hardware from a solution that has worked for years you can expect some pushback. 

[quote="trampa, post:826, topic:35116"]
HM10 is to slow for FW updates and reliable RT data.
[/quote]

While technically correct your talking about seconds for updates and microseconds for real time data, it's not even a concern.
```

---
## \#828 Posted by: Deodand Posted at: 2019-04-08T15:59:21.009Z Reads: 155

```
The unity uses an nrf52 module anyways for clarity :slight_smile:
```

---
## \#829 Posted by: rey8801 Posted at: 2019-04-08T17:16:29.376Z Reads: 152

```
Is there a way that you make the UART signal for the external port compatible for hm10 module. Like it was for focbox so that other telemetry software would work. At least meanwhile you release the own Unity app for telemetry. I think a lot will appreciate it. I sure will :grin:
```

---
## \#830 Posted by: Deodand Posted at: 2019-04-08T17:28:36.000Z Reads: 152

```
It is already compatible, just set the correct baud rate (9600 for hm10 I think)
```

---
## \#831 Posted by: pookybear Posted at: 2019-04-08T17:32:12.334Z Reads: 149

```
What about the internal one?
```

---
## \#832 Posted by: rey8801 Posted at: 2019-04-08T17:39:32.370Z Reads: 150

```
Yeh I would be happy if that would be enough. I have been using hm module for more then a year and works on all type of vesc. For unity it doesn't. It connect one ofut of 20 times and when is connect the signal drops within 10 sec. I am talking about @Ackmaniac app in my case. Being using the app with vesc 4.12, focbox, Flipsky 6.6 never a problem. I love unity but if would be possible to get it work would be great. I am not the only one that found incompatibility between the two.
```

---
## \#833 Posted by: deucesdown Posted at: 2019-04-09T00:17:58.869Z Reads: 145

```
I remember reading the packet format changed on the unity. The old packet format is available but the app has to make a call for it. So it's up to ackmaniac.
```

---
## \#834 Posted by: pookybear Posted at: 2019-04-10T23:43:30.817Z Reads: 148

```
I finally got a chance to switch from ack 3.103 to 3.102! Ack app works! Woohoo. Thanks

I can connect successfully, change settings and what not. But I am getting error 178 on the main screen. Searched for error 178 on here. Nothing comes up.
```

---
## \#835 Posted by: pookybear Posted at: 2019-04-12T02:58:25.448Z Reads: 149

```
![Screenshot_20190411-152526|281x500](upload://cy2odonE49JYn4sCYGyQLIu4JPs.jpeg) 

Error 178.
```

---
## \#836 Posted by: Ackmaniac Posted at: 2019-04-12T08:31:04.557Z Reads: 145

```
Guess your module has issues sending multiple packages directly after another. that also explains why it doesn't work with version 3.103 where there is a additional packet for the realtime data. But it also could be your phones issue. Maybe test it with another phone if you get Error: 178 as well.
```

---
## \#837 Posted by: Joe1 Posted at: 2019-04-12T20:03:38.265Z Reads: 148

```
Where can I download windows binaries for old versions? 3.100-3.102

I'm trying to use the iPhone eSkate VESC app but I don't think it's compatible with the current version.

Anyone using eSkate VESC on Ackmaniac firmware?

[EDIT] Found the problem, had to set UART baud rate to 115200
```

---
## \#838 Posted by: pookybear Posted at: 2019-04-21T05:29:28.514Z Reads: 142

```
Update:

I tried also a different phone. Same error 178. Everything works but I get that error.
```

---
## \#840 Posted by: Pantata Posted at: 2019-05-06T23:32:04.854Z Reads: 141

```
Could you please tell me where to download specific fw version like 3.102, 3.103? Maybe If I switch fw version the metr pro module will start working cause I can fully only use Metr and perimetr apps with ackmaniac fw, ackmaniac esc tool phone app will show the module but won't connect to it.
```

---
## \#841 Posted by: pookybear Posted at: 2019-05-07T05:47:02.887Z Reads: 137

```
[Here](https://ufile.io/1gfh0uom) you go. Version 3.103 should be in github.
```

---
## \#842 Posted by: Pantata Posted at: 2019-05-07T22:51:44.789Z Reads: 137

```
THank you very much, where do you find these FW versions? I looked everywhere, couldn't find anything pretty much.
```

---
## \#843 Posted by: b264 Posted at: 2019-05-07T22:56:58.602Z Reads: 143

```
https://github.com/Ackmaniac

https://github.com/Ackmaniac/bldc/commits/master

<hr />
<hr />
<hr />

3.103 is in here, called VESC_default.bin

That file can only be used on hardware 4.10, 4.11, and 4.12 ***ONLY***

https://github.com/Ackmaniac/vesc_tool/tree/cec330193339a8550eaeeb353ec16944c1e833a0/res/firmwares/410_o_411_o_412
```

---
## \#844 Posted by: L3chef Posted at: 2019-05-12T18:17:41.591Z Reads: 137

```
Is there a change log anywhere? Think I'm on v3101.. Flashed it last summer ~june-aug..
```

---
## \#845 Posted by: Migro Posted at: 2019-05-15T16:06:39.025Z Reads: 133

```
Im currently trying to upload new firmware but it gives me this message. What am i doing wrong?
Its a focbox
![image|690x23](upload://nvrS0ATE6NQbezxandsVlu3GDzK.png)
```

---
## \#846 Posted by: Jinra Posted at: 2019-05-15T16:18:22.838Z Reads: 132

```
It says that because the focbox restarts when upload is done. Normal behavior. Check the f/w version, it should be whatever you just uploaded.
```

---
## \#847 Posted by: Migro Posted at: 2019-05-15T20:22:53.121Z Reads: 130

```
Ahh thans bud :+1: 
It kept tricking me cause it kept saying old firmware but i see 3.102 is "old" i guess
```

---
## \#848 Posted by: Jinra Posted at: 2019-05-15T21:06:01.679Z Reads: 128

```
You gotta upload the f/w that came with the respective tool you downloaded or the tool will keep thinking it's old
```

---
## \#849 Posted by: Migro Posted at: 2019-05-15T21:48:43.848Z Reads: 130

```
I just went for the newest version of ackmaniac's esc tool. And tried the in app options and a link someone posted with the 3.102?
```

---
## \#850 Posted by: Jinra Posted at: 2019-05-15T21:50:09.102Z Reads: 128

```
the app comes with the firmware, 3.103 is the lates version. If you download it you only need to go to firmware and upload, no need to download any firmware separately.
```

---
## \#851 Posted by: Migro Posted at: 2019-05-15T22:14:10.197Z Reads: 131

```
Tried plugging it in again to see what happens now it doesn't connect. Any idea?
```

---
## \#852 Posted by: Janosh Posted at: 2019-05-23T21:50:10.296Z Reads: 124

```
Is the part in the firmware for the nrf remotes the same as in the original from Vedder? Will the new Vesc remote be supported?
```

---
## \#854 Posted by: ualsteve94 Posted at: 2019-06-07T09:10:29.430Z Reads: 110

```

Quick question(noobie here) duel Focbox setup.  Do I input half the total desired battery max into each Focbox?  40a + 40a if I’m shooting for 80?

Thanks  🙏🏽
```

---
## \#855 Posted by: rey8801 Posted at: 2019-06-07T09:13:10.514Z Reads: 108

```
No motor max is not split. The battery max and min are.
```

---
## \#856 Posted by: ualsteve94 Posted at: 2019-06-07T09:17:14.880Z Reads: 111

```
Whoops .   I meant battery max .   So split the battery max then .   Got it .  Thank you much !  

While your here..   If my motor max is 80a and my battery max is 40a, am I only actually getting 40amps to that motor?
```

---
## \#857 Posted by: rey8801 Posted at: 2019-06-07T09:18:29.941Z Reads: 104

```
No no motor max is different. Leave at the max current allowed from your motor if you want max output. Search in the forum you will find the physics behind it, but basically motor max can be way higher then battery max
```

---
## \#858 Posted by: ualsteve94 Posted at: 2019-06-07T09:25:24.850Z Reads: 103

```
SWEET!   

So here’s a scenario.    I get a battery built.  He uses the “Tiny BMS “ for both charge and discharge.   He tells me set esc to 80a battery max.   I set up the Focboxes and use 80a motor max, and also 80a battery max, on each Focbox.  I rode it until the battery was empty without issue.  Is this perhaps from the BMS protection, or the 130a absolute max setting which brings both Focboxes back down to 65a?
```

---
## \#859 Posted by: trampa Posted at: 2019-06-07T09:27:03.215Z Reads: 104

```
Benjamin's VESC-Tool works for the new remotes and App connectivity. 
Frequent FW updates will be available to unlock new features step by step.
Ben's App will keep you updated and will tell you when new stuff is available.
```

---
## \#860 Posted by: rey8801 Posted at: 2019-06-07T09:30:21.764Z Reads: 103

```
I think something is wrong there. Please list specs:
- Battery type configuration ecc... es 12s4p 30Q cells
- Which BMS...Tiny and high discarge is not possible. I want to see it
- Motor you use.

Then I will tell you :wink:
```

---
## \#861 Posted by: ualsteve94 Posted at: 2019-06-07T09:37:38.347Z Reads: 103

```
12s5p Sanyo 20700B
Tiny BMS s516 - 150A/750A
Duel Focbox-achmaniac firmware 
6374 190kv 3550w

Settings for today’s 22 -mile ride.
Each Focbox-
Motor max 80
Battery max 80
Battery min -60
Regen -20
Absolute max 130a

Focboxes reached a high of 60c and my battery lasted for 22miles/35km.
```

---
## \#862 Posted by: ualsteve94 Posted at: 2019-06-07T09:41:42.140Z Reads: 104

```
I was just trying to figure out what my battery builder meant when he told me set battery max to 80a.    

So he meant 40a on each Focbox then ya?
```

---
## \#863 Posted by: rey8801 Posted at: 2019-06-07T09:41:44.546Z Reads: 107

```
[quote="ualsteve94, post:861, topic:35116"]
Tiny BMS s516
[/quote]

Ah ok TIny is the name :joy: My bad, Anyway it's a 60A discharge BMS that were the 60 you measure comes from.

![image|690x222](upload://125w8qHbC6RhRQGpSjSBp93H60A.png) 

Anyhow if you have 80A total from the battery then split it in 2, same for battery min.
```

---
## \#864 Posted by: ualsteve94 Posted at: 2019-06-07T09:42:59.034Z Reads: 105

```
Perfect.   Thanks a bunch !
```

---
## \#865 Posted by: rey8801 Posted at: 2019-06-07T09:43:03.000Z Reads: 104

```
Depends which VESC you have, single vesc or in case of unity is fused so you set the battery max as single and then it splits it. So telling you 80a max is correct then is up to what you use.
```

---
## \#866 Posted by: ualsteve94 Posted at: 2019-06-07T09:43:54.100Z Reads: 102

```
Ok I see.   I’ll change that in the morning , cutting those values in half then.
```

---
## \#867 Posted by: ualsteve94 Posted at: 2019-06-07T09:44:15.082Z Reads: 101

```
Thanks for your help.  Later skater
```

---
## \#868 Posted by: rey8801 Posted at: 2019-06-07T09:44:37.256Z Reads: 103

```
actually more because if the BMS is limited to 60A no rason to set 40A and put it under stress. Set 30a on each focbox.
```

---
## \#869 Posted by: ualsteve94 Posted at: 2019-06-07T09:45:42.546Z Reads: 103

```
Roger that.   Makes sense.  

Now how much power do you think I’m going to lose now from what I felt on today’s ride?
```

---
## \#870 Posted by: rey8801 Posted at: 2019-06-07T09:48:02.483Z Reads: 104

```
nothing. you never passed that anyway.
```

---
## \#871 Posted by: ualsteve94 Posted at: 2019-06-07T09:49:05.147Z Reads: 105

```
Oh that’s awesome news.    Cuzz it felt like a ROCKET today!
```

---
## \#872 Posted by: ualsteve94 Posted at: 2019-06-07T18:12:17.033Z Reads: 109

```
If I want a tiny bit faster response from my trigger, is slightly adjusting the positive ramping time the best option?  If so, what kind of changes we talking, what would be considered a small increase?  

Thanks 🙏🏽
```

---
## \#873 Posted by: pookybear Posted at: 2019-06-07T21:37:24.194Z Reads: 111

```
Try playing w your throttle curves first.
```

---
## \#874 Posted by: ualsteve94 Posted at: 2019-06-08T06:38:09.756Z Reads: 124

```
(Help me tag Ackmaniac or whoever can help!  I have no idea how to tag someone.. thank you gentlemen!!!)

FUCK ME.   Why did I mess with anything 🙁.  
In mid HIGH SPEED acceleration my motors all of a sudden felt like the brakes where engaged or the motors seizing sending me flying.  I’m home now, full of road rash & seeking some help.   Here is a picture of the fault that my Xmatic app showed after the incident.
![image|281x499](upload://a96h3AvwkN8zE7yo9zTJtJGCZn7.jpeg) 

So I’ve had a Lacroix for about 10 months now.  The only tweak I made at the beginning 10 months ago was moving the motor amps up from 70a to 80a.   It ran flawless for the next 10 months.   The Focboxes where programmed  using the original BLDC tool and the boxes running that old firmware that worked for that tool.  The factory Settings where these here.  Accept the motor amps which I had bumped up to 80a
![image|690x357](upload://hi6avYZ4bTI5p5FxqaxwgwqM6EV.png) 

So I get the itch for more power and I have hyper ion build me a 12s5p.  Sanyo 20700B.   He used the ( Tiny BMS s516 - 150A/750A) and my two original Focboxes.  I get it back & go to program the Focboxes using the bldc tool once again but this time it wouldn’t let me, saying old firmware..  Hyper ion guys already set it up using vesc project changing the firmware.  I couldn’t figure out how to switch back the firmware for that BLDC tool so I ended up reading thru this thread and then using the Ackmaniac ESC tool.  Here are the settings I used.   Yes, 80a batt max on each box.  (Per hyper Ion) 

![image|666x500](upload://iEskafEfCmdpoYHkBLHF9pKhtgu.jpeg) ![image|666x500](upload://kZ3ER37L22OniUFOr9JuXWzjDfa.jpeg) ![image|666x500](upload://8w0GMfQxD2mFpcmT7TrsC66qM82.jpeg) ![image|666x500](upload://kbVhFNoUTo1NBsKd6DBYjGhVvlQ.jpeg) 
![image|666x500](upload://e59IOYjcScWwP9Asc7lSNxK0Bkz.jpeg) ![image|666x500](upload://7Uih8sQKNPi7jvEEZgXscWgZFdB.jpeg) ![image|666x500](upload://sCyo3eBPDRTt6bAam2t6G3fTLdQ.jpeg) ![image|666x500](upload://tIo0tk7srVHg9Ob8Me3EBVjE8uU.jpeg) 

I run the board with those settings for an entire charge.   It actually felt great.   Lots of get up and go in the top end.  She lasted 22 miles before  empty.  No issues during that ride and I pushed it all out plenty times.   Anyhow I get to thinking I should lower the battery Max from what everyone is saying, so I lower it to 60a each box (still much higher than what everyone says it should be but I’m going off my battery builder saying I can use 80a each box.   Anyhow, I also lower the positive ramping to .2, hoping for more instant torque throughout.   I changed that in PPM and then I also changed that in nunchuk.   Don’t have a clue what PPM nunchuk is.   I also then increased my motor Max to 85.   So I lowered the batt max to 60 each box and set motor max to 85a each box.  And lowered  the positive ramping to .2 in PPM & Nunchuk.   

I take it out tonight and not more than two minutes into the ride I’m sent flying thru the air.. it felt like it bogged down or locked up or seized right when my throttle was fully engaged at around 20+ mph.   

What did I do wrong?   How can I get my trusty, reliable esk8 back?    

![image|690x319](upload://rJUrXJXCEuy9FFP7f11E0J5sOJu.jpeg)
```

---
## \#875 Posted by: hexakopter Posted at: 2019-06-08T07:27:44.674Z Reads: 121

```
FAULT_CODE_ABS_OVER_CURRENT means that the VESC was reading a to high current and for safety it shut down.
Both changing "Motor Current Max" to a higher value (to 85A in your case) and lowering "Positive Ramping Time" (to 0.2s in your case) leads to a more aggressive current flowing through your motor and ESC, so that your VESC was reading for a fraction of time a value higher than 130A "Absolute Maximum Current" somehow and shuts down.
I would change back to your settings you had running before without any problems. Always wear some protective gear and test if you get these over current errors on very hard accelerations.
```

---
## \#876 Posted by: ualsteve94 Posted at: 2019-06-08T11:43:14.874Z Reads: 116

```
Will dropping the motor max Down from 85 to 80,  dropping the battery max from 60 to 40 and increasing absolute from 135 to 145 possible keep that from happening again?
```

---
## \#877 Posted by: deucesdown Posted at: 2019-06-08T14:08:24.128Z Reads: 121

```
[quote="hexakopter, post:875, topic:35116"]
and for safety it shut down.
[/quote]

This is what I understand to be normal for abs over current, which is a reboot which takes 3 seconds, but

[quote="ualsteve94, post:874, topic:35116"]
it felt like it bogged down or locked up or seized
[/quote]

If it bogged (lost power), the settings changessshould help, but I don't know if it actually locked the wheels. Do you remember which it was? It should feel *very* different.
```

---
## \#878 Posted by: L3chef Posted at: 2019-06-08T14:51:24.233Z Reads: 120

```
[quote="ualsteve94, post:876, topic:35116"]
increasing absolute
[/quote]

Do not change this value
```

---
## \#880 Posted by: ualsteve94 Posted at: 2019-06-08T17:27:16.163Z Reads: 121

```
Ya It felt like it shut off I guess.
```

---
## \#881 Posted by: ualsteve94 Posted at: 2019-06-08T17:28:37.384Z Reads: 124

```
What’s the trade off for now having my absolute 145?
```

---
## \#882 Posted by: jun1208 Posted at: 2019-06-09T16:35:16.934Z Reads: 124

```
I've read a bit in this thread and noticed that the Flipsksy's BT module wasn't supported back then, may I know has anything changed for that?

Or is it still won't be working with Flipsky's BT module?
```

---
## \#883 Posted by: Ackmaniac Posted at: 2019-06-11T21:35:58.832Z Reads: 122

```
The absolute value is for short spikes. So it can happen that the VESC measures high spikes when it hasto handle high currents. So for example of motor max is set to 80A it can happen that sometimes out of 10000 measurements a second spikes with 100A are measured. And the worse the hardware design of the VESC is (every hardware is different). 
Once the VESC sees the higher current taht the absolute max it will throw an error and shut down immediately. So it is wise to leave some wiggle room between max motor amps and absolute max. But do not set it too high because the absolute max value is there to protect the VESC from too high spikes. But normally 140A should be still fine.
```

---
## \#884 Posted by: isabar Posted at: 2019-06-26T14:02:11.808Z Reads: 106

```
@Ackmaniac  I noticed that in ESC Monitor telemetry screen for Temperature data on the left side there is MAX, then below either Mot or Phi symbol.  Sometimes it changes between the two.  Can you clarify what data is being displayed when Mot vs Phi is showing? and in what situations does it change from "Mot" to "Phi"?
Thanks!
```

---
## \#885 Posted by: EViL3000 Posted at: 2019-06-28T10:16:20.168Z Reads: 104

```
Hey everyone,

first i want to big thanks ackmaniac for his work!!! Really nice to have the option with the android app!

Now to my Problem.
I think i have bricked my two Flipsky 4.12 FESC / VESC.
How and why is a longer story and not the right thread, so to be short.

Can anybody tell me where i find a bin or hex file of the bootloader and firmware (3.102 and 3.103) to flash via a st link v2?

All links i have searched and find on the internet (this forum, youtube, etc.) are down or broken.
I am not able to update via the USB port, cause on both VESCs appears the serial port error "no such file or directory" when i try to update over the ackmaniac vesc tool (same error with the original vesc tool). Maybe all of my 3 USB cable are not able to send data properly, i dont know. 
Thanks for your help!
```

---
## \#886 Posted by: rojitor Posted at: 2019-06-28T11:40:08.925Z Reads: 101

```
http://fishpepper.de/wp-content/uploads/2017/09/VESC_FW_AND_BL_092017.zip
```

---
## \#887 Posted by: EViL3000 Posted at: 2019-06-28T11:47:51.213Z Reads: 101

```
thanks rojitor!

I have found this files, too. I have try´d them, but the bootloader is not for 4.12. I ithink it was 4.6 or 4.8.
```

---
## \#888 Posted by: rojitor Posted at: 2019-06-28T11:51:34.985Z Reads: 105

```
Ye. They're outdated but should wake up your vesc. I used that on my vescs
```

---
## \#889 Posted by: EViL3000 Posted at: 2019-06-28T12:02:32.909Z Reads: 106

```
Ok thanks.

Is there no Link to the current Bootloader and or Firmware as a file? I really need version 3.102 and for testing 3.103.
```

---
## \#890 Posted by: trampa Posted at: 2019-06-28T12:17:58.931Z Reads: 108

```
The latest version of code has to be on Nicos Github. 
If you struggle to get a bootloader: https://github.com/vedderb/vesc_tool/tree/master/res
```

---
## \#891 Posted by: deucesdown Posted at: 2019-06-28T14:44:38.415Z Reads: 103

```
You can flash just about any bootloader, and one it's working flash the firmware of your choice using esc-tool.
```

---
## \#892 Posted by: EViL3000 Posted at: 2019-06-28T20:17:00.222Z Reads: 102

```
the link from Trampa was very useful. Thanks a lot!!!
```

---
## \#893 Posted by: Benjamin899 Posted at: 2019-07-31T09:01:40.075Z Reads: 85

```
i can't get the failsafe to work. After removing the bind key the failsafe signal is not beeing send.
```

---
## \#894 Posted by: Moza Posted at: 2019-08-01T10:07:34.859Z Reads: 86

```
![Screenshot_20190801-110237|690x318](upload://98tat653usTsTQPjEyXPswaxzEo.jpeg) 

Hi.
I'm using an adc throttle on a scooter and I have to twist the throttle about a quarter before I get any response.
I can see on the voltage mapping that it recognises the throttle input from the beginning but the current bar is not moving until quarter throttle.
Is there a way I can fix this?
Thanks in advance.
Steve.
```

---
## \#895 Posted by: sayekim Posted at: 2019-08-01T10:52:22.565Z Reads: 85

```
You can adjust the deadband to zero.
```

---
## \#896 Posted by: pookybear Posted at: 2019-09-18T04:25:09.888Z Reads: 64

```
@Ackmaniac 

Any chance on merging the nrf pairing/code from FW 3.40 or higher to the ackmaniac? It would be so awesome to get the wand to work w ackmaniac fw.
```

---
## \#897 Posted by: alexnz Posted at: 2019-09-18T09:41:24.771Z Reads: 61

```
I've had lots of troubles with the ESC Tool not wanting to connect to the attached VESC. Going mad about those Can't open serial port errors, uninstalling and reinstalling drivers, swapping USB cables, in vain. Until I found out that any instance of Cura (Slicing software for 3D printing) that is open on the PC will try to grab a handle on all available serial ports, preventing the VESC-Tool to access it.... Closing Cura brought instant relief and put an end to my VESC misery.  
Hope this helps others!
```

---
## \#898 Posted by: Titoxd10001 Posted at: 2020-01-14T15:16:33.059Z Reads: 23

```
How's it going @Ackmaniac 

We want you back!
```

---
