# New Raptor 2 Remote

### Replies: 79 Views: 613

## \#1 Posted by: Eskate444 Posted at: 2019-04-09T10:39:41.121Z Reads: 163

```
Hello Esk8ers,

I have the Raptor 2, the remote works perfectly, however on R-Spec mode, it has too much power for the small range of the remote throttle.

Do you have any recommendations for a new remote? I would prefer a "gun" style trigger one with smooth range of motion for the throttle, as the Raptor's one is a bit jumpy it can make you fall of the board anytime you tap it.

Thanks
```

---
## \#2 Posted by: DavidBanner Posted at: 2019-04-09T10:46:19.429Z Reads: 156

```
My advice is to spend some time on the board with the Nano-X remote and get used to it. It won't take long until you get used to the short throw.

But if you are set on moving on to a new remote then the mini trigger is popular for good reason. I started off with that remote on my first board but I much prefer a thumb throttle after using one for a while.

![remote_trigger_2%5B1%5D|500x500](upload://kHc68gJLbM32iRuE0FPdQG7j7UP.jpeg)
```

---
## \#3 Posted by: Eskate444 Posted at: 2019-04-09T10:52:48.822Z Reads: 146

```
Is the mini trigger smooth? the finger does not get tired after holding it?

Im not sure how long it takes getting used to the nano X remote, maybe i will give it a few more rides and see how it goes before changing.

Its just that Raptor 2 has alot of power (for me, i am new to Esk8) and it can be unpredictable.
```

---
## \#4 Posted by: rey8801 Posted at: 2019-04-09T10:55:41.877Z Reads: 136

```
I guess your Raptor has unity or focbox. Then connect to the relative vesc tool or unity app and regulate the throttle and braking curve. I have nano-x as well and I agree that the excursion is limited but if you regulate the throttle becomes really good.
```

---
## \#5 Posted by: DavidBanner Posted at: 2019-04-09T10:56:27.605Z Reads: 137

```
[quote="Eskate444, post:3, topic:89916"]
Is the mini trigger smooth? the finger does not get tired after holding it?
[/quote]

yes it's very smooth, nice long throw. Haven't had any finger tiredness, it's a very light throttle.

[quote="Eskate444, post:3, topic:89916"]
ts just that Raptor 2 has alot of power (for me, i am new to Esk8) and it can be unpredictable.
[/quote]
To be fair it's probably the user that is unpredictable in this case :)  There is a learning curve in e-skate. It's about building up muscle memory and learning throttle control. It's all about small smooth movements of the thumb. You also need to learn to put your weight on the front foot during acceleration and on the back foot when braking. It takes a little time but you will get there.
```

---
## \#6 Posted by: Eskate444 Posted at: 2019-04-09T10:56:37.220Z Reads: 124

```
Can you take some screenshots of your remote settings from the tool you use please? I can use BLDC tool for nano x enertion
```

---
## \#7 Posted by: rideTastic Posted at: 2019-04-09T10:56:42.573Z Reads: 123

```
you need to calibrate your remote before any ride. I had the same problem but with the calibration it works now.
```

---
## \#8 Posted by: Eskate444 Posted at: 2019-04-09T10:57:25.664Z Reads: 117

```
I calibrate always, that is not the issue...
```

---
## \#9 Posted by: rey8801 Posted at: 2019-04-09T11:01:30.835Z Reads: 110

```
if you use BLDC tool (really old version of vesc tool) I guess you have focbox. If it is still under warranty then fine like that otherwise you better download ackmaniac or new vesc tool firmware and flash it in the focbox. Since the BLDC tool there were many and many updates that made the ride way better adn remote more adjustable. I am not even sure you can adjust the throttle curve in the BLDC tool. It is a more recent feature.
So first of all, Raptor still under warranty?
```

---
## \#10 Posted by: Eskate444 Posted at: 2019-04-09T11:05:05.218Z Reads: 103

```
Board is not under warranty, and yes it had dual focboxes.

Enertion has their own BLDC tool i believe, which i have downloaded and opened, but never changed any settings.
```

---
## \#11 Posted by: rey8801 Posted at: 2019-04-09T11:15:35.303Z Reads: 103

```
Enertion has his own now with unity, but before it's just a BLDC tool. Focbox is compatible with all the firmware out there. So either you download this one https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAANyC-yQCMeveA7errNRnYqa?dl=0&preview=ACKMANIAC_ESC_TOOL_3_103.zip (Ackmanianc one) or the original Vesc tool from the website https://vesc-project.com/vesc_tool

Both of them work pretty well. I have been using the Ackmaniac version for a over a year and I like it a lot. SInce you can then pair it with a cheap HM-10 module and swap setting from your phone. Vesc tool ask a more expensive module to do that. Ackamaniac will work fine, trust me :wink:

Once downloaded it from the dropbox, open on your PC (only windows). Connect your focbox (master first) as you usually do and follow this simple tutorial. The software will tell you that your focbox firmware is to old so you have to update to the correct one
![image|690x359](upload://fP8wM00mHJX3cAnwXHJuE1wGy3v.png) 
Under firmware select 410 &411 ecc and flash it. Takes 5 second.
![image|690x342](upload://9TS3xM9MaQx5ouJo2S7mr1YvTXC.png) 

Turn off and on again the vesc and reconnect it 
Now follow this tutorial 
https://www.youtube.com/watch?v=v1glLDO-EjA&t=3s
Set first the Master side (ID 0)
Then turn off, disconnect and do the same on the slave side. Always use the wizard.
When you have done with it I will tell you how to adjust the remote. 
Maybe seems a lot but it's like 5 minutes procedure if you know what to do. You are not using the whole potential of your board, just to be clear. I do not know the standard setting on a Raptor but I guess they are a bit conservative.
Ah before do everything read the setting on the BLDC tool of Motor max, Motor min, Battery max and Battery min. So you can apply the same ones later. At least at the beginning.
This passage will give you way more control then change the remote.
Good luck!
```

---
## \#12 Posted by: b264 Posted at: 2019-04-09T11:16:44.972Z Reads: 98

```
[quote="rideTastic, post:7, topic:89916"]
you need to calibrate your remote before any ride
[/quote]

You only need to calibrate it once.

https://forum./t/how-to-bind-the-mini-remote/95
```

---
## \#13 Posted by: Bjork3n Posted at: 2019-04-09T11:19:40.884Z Reads: 95

```
Ackmaniac is the best fw out there, use it :slight_smile:

Smooth throttle all the way!
```

---
## \#14 Posted by: rey8801 Posted at: 2019-04-09T11:21:23.298Z Reads: 94

```
no he is talking about the nano-x. I believe
```

---
## \#15 Posted by: Eskate444 Posted at: 2019-04-09T11:22:35.565Z Reads: 88

```
Man thank you for all the information that you took your time!

There is one problem however, on my master FocBox the usb plug has broken, maybe i can solder it back on... but i am not sure..

Also, my board can already connect to the Ackmaniac ESC monitor from google play store... it allows me to change some settings like create custom motor settings etc..  but i'm not sure where to find throttle settings
```

---
## \#16 Posted by: Eskate444 Posted at: 2019-04-09T11:23:39.205Z Reads: 82

```
This is the one i can connect to and change settings 

https://play.google.com/store/apps/details?id=ackmaniac.vescmonitor&amp;hl=en_AU
```

---
## \#17 Posted by: Bjork3n Posted at: 2019-04-09T11:26:23.510Z Reads: 83

```
That's not the same. You're still using the standard fw and it's prone to be jerky. 
Ackmaniac fw is a lot easier to control and makes it easy to deliver the power to the ground without falling off. 
I use ack 3.102 and Foc mode
```

---
## \#18 Posted by: rey8801 Posted at: 2019-04-09T11:29:19.064Z Reads: 85

```
from the Ackmaniack app where you make a new mode there is a voice called throttle curve or special curve, something like that . there you can adjust it. Although if you do not run the Ackmaniac software on yuor Focbox then it won't apply the setting. You need it's own software installed.

To connect without USB, no problem, you can connect to the vesc with the usb and move to the other vesc via CAN bus. Search for it. or you can use a TCP connection through the app. The latest works but it's a bit unstable so not always works at first try. Both PC and phone has to be under same wifi or hotspot from phone and close to the board.
Anyhow on the forum is all written.

![image|690x324](upload://eXd25GU6evH49pJpnAlSxB8Wcap.png) 
Here where to do the connection via can. You connect to the vesc with USB. Then flash that one. Then under connection you see forward via can to. If set correctly ID 0 is the master ID 1 is the slave. so put ID 0 and press CAN-->
You should see the classical green bar lower right that tells you are connect to the master vesc now. IT should also tell you that the firmware is too old ecc... flash the master too. Then follow the tutorial, just keep in mind you have to go to master first via CAN.
```

---
## \#19 Posted by: Eskate444 Posted at: 2019-04-09T11:33:31.811Z Reads: 77

```
I still dont understand man, you are saying i can connect via USB to my slave focbox, and then from that same USB via the software on my computer i can switch to master focbox?

If i can, that would be great since i dont have to buy another focbox just to update firmware.

You also have a Raptor 2? how different is the feel of the board after flashing new firmware?
```

---
## \#20 Posted by: rey8801 Posted at: 2019-04-09T11:35:08.694Z Reads: 80

```
I don't have a Raptor too, but I used a lot of VESC ecc... believe me that the latests firmware are worth it. Above I add a paragraph showing where to find the CAN connection.
```

---
## \#21 Posted by: Eskate444 Posted at: 2019-04-09T11:35:24.043Z Reads: 77

```
No worries, i see what you mean now after you have edited it,

I will try this and get back to you. Much appreciated man.
```

---
## \#22 Posted by: Eskate444 Posted at: 2019-04-09T11:36:09.228Z Reads: 74

```
Do you have a raptor man? how different is it after you flashed?
```

---
## \#23 Posted by: AlanZhou Posted at: 2019-04-09T11:38:27.867Z Reads: 73

```
No you have to calibrate Everytime you connect the nano x @b264  or else it will be very jerky, @Eskate444 when your remote first connects, full throttle and full break and your remote will be calibrated, do this with your board up
```

---
## \#24 Posted by: DavidBanner Posted at: 2019-04-09T11:43:56.384Z Reads: 74

```
as @AlanZhou said you definitely need calibrate the nano-x every time it's turned on before turning on the board. 

I forgot a few times and the board started rolling off without me on it.
```

---
## \#25 Posted by: AlanZhou Posted at: 2019-04-09T11:46:23.591Z Reads: 68

```
@DavidBanner well I just learned something, I thought the board had to be on to do calibration 😂
```

---
## \#26 Posted by: DavidBanner Posted at: 2019-04-09T11:49:28.348Z Reads: 68

```
definitely calibrate the nano-x before turning your board :slight_smile:

this is from enertion's instructions:
This process is simple, but  **needs to be done before each time you ride.**

If you've ever experienced the throttle control on the Nano-X being too sensitive, or your wheels are spinning with no input from the remote, forgetting this step is most likely the reason why.

**1. Turn on the Nano-X**

**2. Push throttle full-forward, full back then leave center**

![Photo_Apr_13__2_09_34_PM.jpg|497x373](https://enertionboards.zendesk.com/hc/article_attachments/360000348336/Photo_Apr_13__2_09_34_PM.jpg)

![Photo_Apr_13__2_09_39_PM.jpg|496x372](https://enertionboards.zendesk.com/hc/article_attachments/360000348276/Photo_Apr_13__2_09_39_PM.jpg)

![Photo_Apr_13__2_09_47_PM.jpg|495x371](https://enertionboards.zendesk.com/hc/article_attachments/360000348316/Photo_Apr_13__2_09_47_PM.jpg)

**3. Turn on the skateboard**

**4. Wait for green light on Nano-X to become solid (indicates connection)**

**5. Check Acc/Brake function before riding**

That's it, you're done! Now get out there and RIDE!
```

---
## \#27 Posted by: Eskate444 Posted at: 2019-04-09T11:50:42.188Z Reads: 60

```
I have managed to connect via TCP mate, but i got this error message:

![Untitled|690x375](upload://uLVwC0lQUB9hTnpkoGRFfPkQTSj.png) 

I am scared to mess up my original settings from enertion... since i dont have warranty i wont be able to get help from them if i change the wrong settings

Is there any way to backup my settings?
```

---
## \#28 Posted by: AlanZhou Posted at: 2019-04-09T11:51:08.488Z Reads: 57

```
If you don't know what your doing don't mess with vesc settings, because that's not the issue
```

---
## \#29 Posted by: Eskate444 Posted at: 2019-04-09T11:51:45.019Z Reads: 57

```
[quote="Eskate444, post:27, topic:89916"]
I am scared to mess up my original settings from enertion… since i dont have warranty i wont be able to get help from them if i change the wrong settings

Is there any way to backup my settings?
[/quote]

This is what im afraid of 

"I am scared to mess up my original settings from enertion… since i dont have warranty i wont be able to get help from them if i change the wrong settings

Is there any way to backup my settings?"
```

---
## \#30 Posted by: AlanZhou Posted at: 2019-04-09T11:52:30.353Z Reads: 54

```
No, except for a screenshot
```

---
## \#31 Posted by: AlanZhou Posted at: 2019-04-09T11:52:46.991Z Reads: 56

```
Just calibrate your remote that'll fix the sensitivity
```

---
## \#32 Posted by: Eskate444 Posted at: 2019-04-09T11:53:40.871Z Reads: 49

```
I have calibrated it mate, trust me i do that everytime i start the remote.

People on here are saying newer versions of VESC firmware are better so i am interested in flashing to newer ones
```

---
## \#33 Posted by: AlanZhou Posted at: 2019-04-09T11:54:09.005Z Reads: 48

```
Then it's you.
```

---
## \#34 Posted by: AlanZhou Posted at: 2019-04-09T11:54:29.802Z Reads: 46

```
You can't handle the torque, you don't have the skill yet, rspec is no problem for me and I have to crank up the settings to 80a for it to feel fun to me
```

---
## \#35 Posted by: Eskate444 Posted at: 2019-04-09T11:56:15.497Z Reads: 47

```
That might be the problem, i admit to being new to skating in general.

Are you using the nano x still? Have you changed decks?
```

---
## \#36 Posted by: AlanZhou Posted at: 2019-04-09T11:57:25.073Z Reads: 45

```
No I run the raptor hubs on 12s and even tried the nano x for a bit
```

---
## \#37 Posted by: DavidBanner Posted at: 2019-04-09T11:58:36.644Z Reads: 48

```
@Eskate444 keep at it man, you will get used to the board a lot quicker than you think. But at the same time it's good you are nervous and treating the Raptor 2 with respect , take it slow, enjoy the process and don't push yourself too far out of your current comfort level and you should be golden and avoid injury.
```

---
## \#38 Posted by: rideTastic Posted at: 2019-04-09T12:03:07.144Z Reads: 45

```
yes i was talking about the nano-x
```

---
## \#39 Posted by: rey8801 Posted at: 2019-04-09T12:04:55.151Z Reads: 49

```
man that is correct, no error there. I also mentioned 3 times. you will get the message that your firmware is too old and you have to flash the new one. Did you watch the video ? Just watch it once and if you think it is to difficult then don't do it.

It's true that you have to get use to the board, but I have used 5 remotes so far and nano-x is reliable but it's true that has short range of motion. I find myself better by adjusting the throttle curve. As I said up to you.
```

---
## \#40 Posted by: rey8801 Posted at: 2019-04-09T12:08:15.313Z Reads: 51

```
Anyhow you can save your setting is not true that you can only take screenshot. Anyhow there isn't too much to save. As I mentioned motor max, motor min, battery max and battery min. To me if you know whihc battery you have and Raptor I believe is a 10s4p 30Q battery then the setting can be

each VECS
- Motor max 60A
- Motor min -60A (guessing, not sure about the Raptor motor, but I guess this one are feasible)
- Battery max 40A
- Battery min -8A

Start from here and adjust while riding.


EDIT:
One thing I gave for sure since it is not under warranty anymore. When did you get your Raptor and how long have you been skating an eboard?
```

---
## \#41 Posted by: Eskate444 Posted at: 2019-04-09T12:11:44.306Z Reads: 46

```
I will change the firmware, at the moment i am just taking screenshots of the Ackmanic settings that show my original settings.

I will save these screenshots and then apply the firmware like you said in the video.
```

---
## \#42 Posted by: DavidBanner Posted at: 2019-04-09T12:12:13.428Z Reads: 46

```
I'm not so sure playing with the FOCBOX / Unity settings is such a good idea given that @Eskate444 is so early on his journey to esk8 elite status.

It may be better to speak to the support team at enertion who are probably best placed to give appropriate advice. 

@CarlCollins  what do you think?
```

---
## \#43 Posted by: Eskate444 Posted at: 2019-04-09T12:13:08.003Z Reads: 44

```
I have had the board for about 1 month now, i bought it used from someone and the warranty is finished.

I have been Eksating 1 month.
```

---
## \#44 Posted by: Eskate444 Posted at: 2019-04-09T12:14:18.129Z Reads: 44

```
![2|690x175](upload://yoDXQDMPE2sK2r4vw1mO0Q1LbhH.png)
```

---
## \#45 Posted by: Eskate444 Posted at: 2019-04-09T12:15:19.837Z Reads: 42

```
Appreciate the advice bro, if i can change the throttle setting only i would be happy with it, as Rey8801 mentioned it can be "smoother" it may help me.
```

---
## \#46 Posted by: rey8801 Posted at: 2019-04-09T12:16:49.605Z Reads: 40

```
Ah ok, then flashing the firmware is ok, but the main problem is that you are not still able to handle it. I didn't know you were so new to esk8. Use the remote in low spec and increase only at due time. Meanwhile read about it and you will find yourself more prepare once ready.

@DavidBanner is Raptor is not under warranty anymore. Focbox or unity is just a normal vesc nothing that needs a special setting. Anyhow I was just inform him about the possibility, since for me not knowing is never an answer :grin: We are in a DIY forum after all.
```

---
## \#47 Posted by: rey8801 Posted at: 2019-04-09T12:19:34.155Z Reads: 40

```
How can be that Raptor has battery max 60 and -20A ? That is something weird. Where did you get this values?
```

---
## \#48 Posted by: AlanZhou Posted at: 2019-04-09T12:23:48.298Z Reads: 39

```
No it's 30a and -10 a for each vesc
```

---
## \#49 Posted by: AlanZhou Posted at: 2019-04-09T12:24:14.556Z Reads: 39

```
60 and -20 is for the unity cause it is basically two esc's
```

---
## \#50 Posted by: rey8801 Posted at: 2019-04-09T12:24:30.845Z Reads: 39

```
Ah that makes more sense.
```

---
## \#51 Posted by: AlanZhou Posted at: 2019-04-09T12:24:59.944Z Reads: 40

```
-20 on both vesc will destory the bms or the battery 🤣
```

---
## \#52 Posted by: rey8801 Posted at: 2019-04-09T12:25:20.196Z Reads: 38

```
yep but it has focbox that is why I was surprise. Probably he is taking the wrong screenshot form the default setting of the vesc tool and not from the vesc itself. 

@Eskate444 do you know someone that you can visit and knows about esk8? or better built a board already?
```

---
## \#53 Posted by: AlanZhou Posted at: 2019-04-09T12:26:10.231Z Reads: 37

```
Yup I assume that too, he probably didn't press the read button
```

---
## \#54 Posted by: Eskate444 Posted at: 2019-04-09T12:37:16.499Z Reads: 35

```
I have to say again THANK YOU TO ALL for the help received, this community is amazing.

From the replies, i can tell everyone here has a pure passion for Esk8, otherwise there would not be this much interest or help.

I hope to one day become a good Esk8er and build my own board very soon.
```

---
## \#55 Posted by: Eskate444 Posted at: 2019-04-09T12:38:00.323Z Reads: 35

```
I am in Sydney Australia mate, the Esk8 scene is not too big, i will build my own board very soon as soon as i can handle the raptor and get my skating skills up to scratch.
```

---
## \#56 Posted by: rey8801 Posted at: 2019-04-09T12:39:39.147Z Reads: 37

```
Well there are several guys from Australia. You will see that yuu are not alone. I am from EU, so knows the feeling, but we will get there :wink:
```

---
## \#57 Posted by: DavidBanner Posted at: 2019-04-09T12:39:55.966Z Reads: 41

```
[quote="Eskate444, post:55, topic:89916, full:true"]
I am in Sydney Australia mate, the Esk8 scene is not too big, i will build my own board very soon as soon as i can handle the raptor and get my skating skills up to scratch.
[/quote]

pop over to Jason's house, he's in the Gold Coast, as Australia is so small it should be a short walk :rofl:
```

---
## \#58 Posted by: rey8801 Posted at: 2019-04-09T12:40:18.825Z Reads: 37

```
Of you do it please make a video :grin:
```

---
## \#59 Posted by: Eskate444 Posted at: 2019-04-09T12:40:36.039Z Reads: 36

```
LOL ride the Raptor from Sydney to his house... for sure until that time i will become a really good skater... all those KM's haha..
```

---
## \#60 Posted by: rey8801 Posted at: 2019-04-09T12:41:06.952Z Reads: 37

```
Do you have problem in the slow mode too?
```

---
## \#61 Posted by: DavidBanner Posted at: 2019-04-09T12:41:38.203Z Reads: 35

```
lol! I've driven from Sydney to the Goldcoast, it's a looong journey. But a great experience, stopping to surf (badly) at the awesome beaches along the way.
```

---
## \#62 Posted by: Eskate444 Posted at: 2019-04-09T12:43:27.996Z Reads: 34

```
Slow mode is actually amazing, i can push the throttle all the way, and its really smooth accelerating.

However, they said something in the remote is "limited" to 80% in slow mode, so the braking power is much reduced.

I have tried different modes in Ackmaniac bluetooth app, and find the intermediate mode pretty good also.

I believe the issue with me is, the board is powerful and i am new to skating, so its not a good match until i can learn to handle it.
```

---
## \#63 Posted by: rey8801 Posted at: 2019-04-09T12:48:32.307Z Reads: 33

```
yeh slow mode use 85% of the throttle both in acceleration and brakes which sucks. Then adjust the setting only by reducing motor max and battery max so that you can have R-spec and do not fly. 
Although I don't think that changing settings from the ackmaniack app will work. As I said you need is own firmware on the vesc.
```

---
## \#64 Posted by: Eskate444 Posted at: 2019-04-09T12:50:27.847Z Reads: 33

```
Changing settings from Ackmaniack app does work, when i press intermediate or beginner mode, it changes how the board reacts.

However it defaults back to original when i turn the board off and i need to select mode again, but it works when i do that.
```

---
## \#65 Posted by: rey8801 Posted at: 2019-04-09T12:51:44.377Z Reads: 29

```
in that case on the main page of the app after changed the mode if you keep press on the mode it will tell you " do you want to set current mode as default one?" YEs and the setting stays

in mode creator at the bottom you have special curve to adjust the throttle.
```

---
## \#66 Posted by: Eskate444 Posted at: 2019-04-09T12:55:02.756Z Reads: 26

```
Damn man i never knew the save default setting existed, will do that for sure!

At the moment, the default R Spec is Max M 80A, Min M -50A. Max B 30A, Min B - 10 A (it is in "current" mode)

Can you recommend a setting for a beginner which is not too slow but has good braking?
```

---
## \#67 Posted by: Eskate444 Posted at: 2019-04-09T12:55:47.951Z Reads: 27

```
I do not see any mode creator for throttle curve
```

---
## \#68 Posted by: rey8801 Posted at: 2019-04-09T12:56:41.182Z Reads: 29

```
if you would have the ackmaniac firmware you could sett the watt but in your case try

Motor max 30A
battery max 20A

If braking are fine stay like that if you want more bring Motor min to -60A.
```

---
## \#69 Posted by: rey8801 Posted at: 2019-04-09T12:57:59.359Z Reads: 31

```
In mode creator

Use special throttle curves
![vescmonitor|281x500](upload://a1rWAkSZ0fvHFVz2HwcbxUoe1bZ.png)
```

---
## \#70 Posted by: Eskate444 Posted at: 2019-04-09T12:58:11.031Z Reads: 32

```
I have found the special throttle curve from mode setup, i am making custom mode now.

I will take a screenshot for you to show my settings
```

---
## \#71 Posted by: Eskate444 Posted at: 2019-04-09T12:58:57.883Z Reads: 30

```
Also, i can change to watt mode from current and also can put "reverse" function... it seems i dont need to change firmware to access this from ackmaniac
```

---
## \#72 Posted by: rey8801 Posted at: 2019-04-09T12:59:44.122Z Reads: 34

```
yes I know but better stay with current mode. I am pretty sure watt mode is not supported in the BLDC tool. Once upgrade the firmware then definitely watt mode. To understand now current mode doesn't exist anymore.
```

---
## \#73 Posted by: Eskate444 Posted at: 2019-04-09T13:06:56.002Z Reads: 38

```
![screengrab-20190409-230506|281x500](upload://oCFAds18ufcuphYLPHLFviyDJdl.jpeg) 

What is difference between watt and current?

These are settings you recommended.
```

---
## \#74 Posted by: Eskate444 Posted at: 2019-04-09T13:09:38.131Z Reads: 36

```
![screengrab-20190409-230849|281x500](upload://gJLcIfyprLYnJQmniMw4u4FJPKd.jpeg)
```

---
## \#75 Posted by: rey8801 Posted at: 2019-04-09T13:30:40.427Z Reads: 37

```
in this way you have lower acceleration and more instant brakes, is that what you wanted?
Anyhow is too much. First try with the reduce current settings and try it maybe is already enough. Then reduce the throttle buy way less. use natural exponentianl function and starts with - 8 for instance. It affects a lot.
```

---
## \#76 Posted by: Eskate444 Posted at: 2019-04-09T13:33:57.518Z Reads: 36

```
This is the default throttle settings from Ackmaniac, i have not changed anything in them.

It is night time now, i will have a look and test these settings tomorrow and give you an update for sure man, much appreciate the knowledge you give!
```

---
## \#77 Posted by: rey8801 Posted at: 2019-04-09T13:43:42.955Z Reads: 35

```
Try first without the thottle curve. Then if you still do not like it apply a less invasive one as I suggested. then adjust base on feeling, but I ma sure the adjust current setting will already do the trick.

No problem man, any time :wink:
```

---
## \#78 Posted by: Eskate444 Posted at: 2019-04-10T10:13:44.928Z Reads: 25

```
Hi mate, i tried your settings tonight on a cruise ride.

They are amazing, i now have complete control of the board, and the braking is amazing also.

I did not use a custom throttle curve, just the default.

I used Watt mode instead of current.

I will stay on these settings for 1 month, and then increase power by 5 on each.

Also, the battery is amazing, i cruised for 1.5 hours and it went down from 70 to 35%.
```

---
## \#79 Posted by: rey8801 Posted at: 2019-04-10T10:27:44.863Z Reads: 25

```
good happy of that. Battery is extended now since you use less power.
I thought you don't need the throttle curve anymore since you reduce the power.
watt mode I am 9% sure that you can also deactivate it since the BLDC tool on the vesc doesn't know how to read it
```

---
